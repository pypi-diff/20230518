# Comparing `tmp/edgeimpulse_api-1.23.0.tar.gz` & `tmp/edgeimpulse_api-1.23.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edgeimpulse_api-1.23.0.tar", max compression
+gzip compressed data, was "edgeimpulse_api-1.23.6.tar", max compression
```

## Comparing `edgeimpulse_api-1.23.0.tar` & `edgeimpulse_api-1.23.6.tar`

### file list

```diff
@@ -1,698 +1,701 @@
--rw-r--r--   0        0        0      377 2023-04-11 17:11:57.751687 edgeimpulse_api-1.23.0/README.md
--rw-r--r--   0        0        0    65903 2023-05-09 16:56:21.134839 edgeimpulse_api-1.23.0/edgeimpulse_api/__init__.py
--rw-r--r--   0        0        0     2752 2023-05-09 16:43:36.481166 edgeimpulse_api-1.23.0/edgeimpulse_api/api/__init__.py
--rw-r--r--   0        0        0   168622 2023-05-09 16:43:35.829189 edgeimpulse_api-1.23.0/edgeimpulse_api/api/admin_api.py
--rw-r--r--   0        0        0   290132 2023-05-09 16:43:35.850299 edgeimpulse_api-1.23.0/edgeimpulse_api/api/allows_read_only_api.py
--rw-r--r--   0        0        0    11231 2023-05-09 16:43:35.867559 edgeimpulse_api-1.23.0/edgeimpulse_api/api/auth_api.py
--rw-r--r--   0        0        0     6235 2023-05-09 16:43:35.874478 edgeimpulse_api-1.23.0/edgeimpulse_api/api/cdn_api.py
--rw-r--r--   0        0        0    27785 2023-05-09 16:43:35.883678 edgeimpulse_api-1.23.0/edgeimpulse_api/api/classify_api.py
--rw-r--r--   0        0        0     7426 2023-05-09 16:43:35.893329 edgeimpulse_api-1.23.0/edgeimpulse_api/api/content_disposition_inline_api.py
--rw-r--r--   0        0        0    72480 2023-05-09 16:43:35.917297 edgeimpulse_api-1.23.0/edgeimpulse_api/api/deployment_api.py
--rw-r--r--   0        0        0    38974 2023-05-09 16:43:35.932859 edgeimpulse_api-1.23.0/edgeimpulse_api/api/devices_api.py
--rw-r--r--   0        0        0   130256 2023-05-09 16:43:35.904773 edgeimpulse_api-1.23.0/edgeimpulse_api/api/dsp_api.py
--rw-r--r--   0        0        0     6435 2023-05-09 16:43:35.943608 edgeimpulse_api-1.23.0/edgeimpulse_api/api/export_api.py
--rw-r--r--   0        0        0    11921 2023-05-09 16:43:35.952040 edgeimpulse_api-1.23.0/edgeimpulse_api/api/health_api.py
--rw-r--r--   0        0        0    49621 2023-05-09 16:43:35.960807 edgeimpulse_api-1.23.0/edgeimpulse_api/api/impulse_api.py
--rw-r--r--   0        0        0   231500 2023-05-09 16:43:35.973402 edgeimpulse_api-1.23.0/edgeimpulse_api/api/jobs_api.py
--rw-r--r--   0        0        0   134972 2023-05-09 16:43:35.988466 edgeimpulse_api-1.23.0/edgeimpulse_api/api/learn_api.py
--rw-r--r--   0        0        0     6483 2023-05-09 16:43:35.999216 edgeimpulse_api-1.23.0/edgeimpulse_api/api/login_api.py
--rw-r--r--   0        0        0    12006 2023-05-09 16:43:36.005624 edgeimpulse_api-1.23.0/edgeimpulse_api/api/metrics_api.py
--rw-r--r--   0        0        0    67457 2023-05-09 16:43:36.014600 edgeimpulse_api-1.23.0/edgeimpulse_api/api/optimization_api.py
--rw-r--r--   0        0        0   300920 2023-05-09 16:43:36.031113 edgeimpulse_api-1.23.0/edgeimpulse_api/api/organization_allow_developer_profile_api.py
--rw-r--r--   0        0        0    63058 2023-05-09 16:43:36.049757 edgeimpulse_api-1.23.0/edgeimpulse_api/api/organization_allow_guest_access_api.py
--rw-r--r--   0        0        0   141131 2023-05-09 16:43:36.063341 edgeimpulse_api-1.23.0/edgeimpulse_api/api/organization_blocks_api.py
--rw-r--r--   0        0        0    91908 2023-05-09 16:43:36.076675 edgeimpulse_api-1.23.0/edgeimpulse_api/api/organization_create_project_api.py
--rw-r--r--   0        0        0   248475 2023-05-09 16:43:36.089644 edgeimpulse_api-1.23.0/edgeimpulse_api/api/organization_data_api.py
--rw-r--r--   0        0        0    58218 2023-05-09 16:43:36.104875 edgeimpulse_api-1.23.0/edgeimpulse_api/api/organization_jobs_api.py
--rw-r--r--   0        0        0    47178 2023-05-09 16:43:36.117394 edgeimpulse_api-1.23.0/edgeimpulse_api/api/organization_pipelines_api.py
--rw-r--r--   0        0        0    45490 2023-05-09 16:43:36.136675 edgeimpulse_api-1.23.0/edgeimpulse_api/api/organization_portals_api.py
--rw-r--r--   0        0        0   224285 2023-05-09 16:56:04.585855 edgeimpulse_api-1.23.0/edgeimpulse_api/api/organization_requires_admin_api.py
--rw-r--r--   0        0        0   134232 2023-05-09 16:56:04.586059 edgeimpulse_api-1.23.0/edgeimpulse_api/api/organization_requires_whitelabel_admin_api.py
--rw-r--r--   0        0        0   258171 2023-05-09 16:56:04.586293 edgeimpulse_api-1.23.0/edgeimpulse_api/api/organizations_api.py
--rw-r--r--   0        0        0    54671 2023-05-09 16:43:36.255985 edgeimpulse_api-1.23.0/edgeimpulse_api/api/performance_calibration_api.py
--rw-r--r--   0        0        0   228112 2023-05-09 16:43:36.273250 edgeimpulse_api-1.23.0/edgeimpulse_api/api/projects_api.py
--rw-r--r--   0        0        0   328783 2023-05-09 16:43:36.301146 edgeimpulse_api-1.23.0/edgeimpulse_api/api/raw_data_api.py
--rw-r--r--   0        0        0    24481 2023-05-09 16:43:36.323360 edgeimpulse_api-1.23.0/edgeimpulse_api/api/requires_sudo_api.py
--rw-r--r--   0        0        0     7730 2023-05-09 16:43:36.335940 edgeimpulse_api-1.23.0/edgeimpulse_api/api/requires_third_party_auth_api_key_api.py
--rw-r--r--   0        0        0    13690 2023-05-09 16:43:36.361801 edgeimpulse_api-1.23.0/edgeimpulse_api/api/supports_range_api.py
--rw-r--r--   0        0        0    35671 2023-05-09 16:43:36.382936 edgeimpulse_api-1.23.0/edgeimpulse_api/api/themes_api.py
--rw-r--r--   0        0        0    43486 2023-05-09 16:43:36.395056 edgeimpulse_api-1.23.0/edgeimpulse_api/api/third_party_auth_api.py
--rw-r--r--   0        0        0    45393 2023-05-09 16:43:36.409546 edgeimpulse_api-1.23.0/edgeimpulse_api/api/upload_portal_api.py
--rw-r--r--   0        0        0   197590 2023-05-09 16:43:36.425047 edgeimpulse_api-1.23.0/edgeimpulse_api/api/user_api.py
--rw-r--r--   0        0        0    42135 2023-05-09 16:43:36.446235 edgeimpulse_api-1.23.0/edgeimpulse_api/api/whitelabels_api.py
--rw-r--r--   0        0        0    29331 2023-05-09 16:43:36.491994 edgeimpulse_api-1.23.0/edgeimpulse_api/api_client.py
--rw-r--r--   0        0        0    15659 2023-05-09 16:43:36.470660 edgeimpulse_api-1.23.0/edgeimpulse_api/configuration.py
--rw-r--r--   0        0        0     5113 2023-05-09 16:43:36.484020 edgeimpulse_api-1.23.0/edgeimpulse_api/exceptions.py
--rw-r--r--   0        0        0    62698 2023-05-09 16:43:48.967094 edgeimpulse_api-1.23.0/edgeimpulse_api/models/__init__.py
--rw-r--r--   0        0        0     2897 2023-05-09 16:43:48.941133 edgeimpulse_api-1.23.0/edgeimpulse_api/models/activate_user_by_third_party_activation_code_request.py
--rw-r--r--   0        0        0     1882 2023-05-09 16:43:48.948229 edgeimpulse_api-1.23.0/edgeimpulse_api/models/activate_user_request.py
--rw-r--r--   0        0        0     2610 2023-05-09 16:43:48.141565 edgeimpulse_api-1.23.0/edgeimpulse_api/models/add_api_key_request.py
--rw-r--r--   0        0        0     1963 2023-05-09 16:43:48.329232 edgeimpulse_api-1.23.0/edgeimpulse_api/models/add_collaborator_request.py
--rw-r--r--   0        0        0     2223 2023-05-09 16:43:49.560131 edgeimpulse_api-1.23.0/edgeimpulse_api/models/add_hmac_key_request.py
--rw-r--r--   0        0        0     2432 2023-05-09 16:43:49.492076 edgeimpulse_api-1.23.0/edgeimpulse_api/models/add_member_request.py
--rw-r--r--   0        0        0     2418 2023-05-09 16:43:48.538531 edgeimpulse_api-1.23.0/edgeimpulse_api/models/add_organization_api_key_request.py
--rw-r--r--   0        0        0     2730 2023-05-09 16:43:48.978798 edgeimpulse_api-1.23.0/edgeimpulse_api/models/add_organization_bucket_request.py
--rw-r--r--   0        0        0     2269 2023-05-09 16:43:49.143407 edgeimpulse_api-1.23.0/edgeimpulse_api/models/add_organization_deploy_block_response.py
--rw-r--r--   0        0        0     2816 2023-05-09 16:43:48.891647 edgeimpulse_api-1.23.0/edgeimpulse_api/models/add_organization_dsp_block_request.py
--rw-r--r--   0        0        0     2248 2023-05-09 16:43:49.290287 edgeimpulse_api-1.23.0/edgeimpulse_api/models/add_organization_dsp_block_response.py
--rw-r--r--   0        0        0     2054 2023-05-09 16:43:48.928840 edgeimpulse_api-1.23.0/edgeimpulse_api/models/add_organization_secret_request.py
--rw-r--r--   0        0        0     2266 2023-05-09 16:43:49.323740 edgeimpulse_api-1.23.0/edgeimpulse_api/models/add_organization_secret_response.py
--rw-r--r--   0        0        0     1949 2023-05-09 16:43:48.752356 edgeimpulse_api-1.23.0/edgeimpulse_api/models/add_organization_secret_response_all_of.py
--rw-r--r--   0        0        0     3834 2023-05-09 16:43:48.414095 edgeimpulse_api-1.23.0/edgeimpulse_api/models/add_organization_transfer_learning_block_request.py
--rw-r--r--   0        0        0     2339 2023-05-09 16:43:49.256638 edgeimpulse_api-1.23.0/edgeimpulse_api/models/add_organization_transfer_learning_block_response.py
--rw-r--r--   0        0        0     4592 2023-05-09 16:43:48.171309 edgeimpulse_api-1.23.0/edgeimpulse_api/models/add_organization_transformation_block_request.py
--rw-r--r--   0        0        0     2325 2023-05-09 16:43:49.787296 edgeimpulse_api-1.23.0/edgeimpulse_api/models/add_organization_transformation_block_response.py
--rw-r--r--   0        0        0     2001 2023-05-09 16:43:48.472878 edgeimpulse_api-1.23.0/edgeimpulse_api/models/add_organization_transformation_block_response_all_of.py
--rw-r--r--   0        0        0     1961 2023-05-09 16:43:49.553468 edgeimpulse_api-1.23.0/edgeimpulse_api/models/admin_add_or_update_sso_domain_id_ps_request.py
--rw-r--r--   0        0        0     2130 2023-05-09 16:43:49.696714 edgeimpulse_api-1.23.0/edgeimpulse_api/models/admin_add_project_user_request.py
--rw-r--r--   0        0        0     3876 2023-05-09 16:43:49.890852 edgeimpulse_api-1.23.0/edgeimpulse_api/models/admin_api_organization.py
--rw-r--r--   0        0        0     2396 2023-05-09 16:43:48.366975 edgeimpulse_api-1.23.0/edgeimpulse_api/models/admin_api_organization_all_of.py
--rw-r--r--   0        0        0     3459 2023-05-09 16:43:49.124926 edgeimpulse_api-1.23.0/edgeimpulse_api/models/admin_api_project.py
--rw-r--r--   0        0        0     6367 2023-05-09 16:43:48.471119 edgeimpulse_api-1.23.0/edgeimpulse_api/models/admin_api_user.py
--rw-r--r--   0        0        0     4953 2023-05-09 16:43:49.687147 edgeimpulse_api-1.23.0/edgeimpulse_api/models/admin_api_user_all_of.py
--rw-r--r--   0        0        0     2262 2023-05-09 16:43:49.296783 edgeimpulse_api-1.23.0/edgeimpulse_api/models/admin_create_organization_request.py
--rw-r--r--   0        0        0     2217 2023-05-09 16:43:49.524116 edgeimpulse_api-1.23.0/edgeimpulse_api/models/admin_get_metrics_response.py
--rw-r--r--   0        0        0     1910 2023-05-09 16:43:49.195974 edgeimpulse_api-1.23.0/edgeimpulse_api/models/admin_get_metrics_response_all_of.py
--rw-r--r--   0        0        0     3046 2023-05-09 16:43:49.065493 edgeimpulse_api-1.23.0/edgeimpulse_api/models/admin_get_organizations_response.py
--rw-r--r--   0        0        0     2746 2023-05-09 16:43:50.008882 edgeimpulse_api-1.23.0/edgeimpulse_api/models/admin_get_organizations_response_all_of.py
--rw-r--r--   0        0        0     2868 2023-05-09 16:43:49.087287 edgeimpulse_api-1.23.0/edgeimpulse_api/models/admin_get_organizations_response_all_of_organizations.py
--rw-r--r--   0        0        0     2243 2023-05-09 16:43:48.937415 edgeimpulse_api-1.23.0/edgeimpulse_api/models/admin_get_sso_domain_id_ps_response.py
--rw-r--r--   0        0        0     1947 2023-05-09 16:43:49.057427 edgeimpulse_api-1.23.0/edgeimpulse_api/models/admin_get_sso_domain_id_ps_response_all_of.py
--rw-r--r--   0        0        0     2914 2023-05-09 16:43:49.589495 edgeimpulse_api-1.23.0/edgeimpulse_api/models/admin_get_sso_settings_response.py
--rw-r--r--   0        0        0     2614 2023-05-09 16:43:49.388619 edgeimpulse_api-1.23.0/edgeimpulse_api/models/admin_get_sso_settings_response_all_of.py
--rw-r--r--   0        0        0     2096 2023-05-09 16:43:48.715765 edgeimpulse_api-1.23.0/edgeimpulse_api/models/admin_get_sso_settings_response_all_of_sso_whitelist.py
--rw-r--r--   0        0        0     2208 2023-05-09 16:43:49.664953 edgeimpulse_api-1.23.0/edgeimpulse_api/models/admin_get_user_ids_response.py
--rw-r--r--   0        0        0     1901 2023-05-09 16:43:49.565227 edgeimpulse_api-1.23.0/edgeimpulse_api/models/admin_get_user_ids_response_all_of.py
--rw-r--r--   0        0        0     2245 2023-05-09 16:43:49.848319 edgeimpulse_api-1.23.0/edgeimpulse_api/models/admin_get_user_metrics_response.py
--rw-r--r--   0        0        0     1938 2023-05-09 16:43:48.438883 edgeimpulse_api-1.23.0/edgeimpulse_api/models/admin_get_user_metrics_response_all_of.py
--rw-r--r--   0        0        0     2452 2023-05-09 16:43:48.159386 edgeimpulse_api-1.23.0/edgeimpulse_api/models/admin_get_user_response.py
--rw-r--r--   0        0        0     2128 2023-05-09 16:43:49.079935 edgeimpulse_api-1.23.0/edgeimpulse_api/models/admin_get_user_response_all_of.py
--rw-r--r--   0        0        0     2807 2023-05-09 16:43:48.626831 edgeimpulse_api-1.23.0/edgeimpulse_api/models/admin_get_users_response.py
--rw-r--r--   0        0        0     2500 2023-05-09 16:43:49.844759 edgeimpulse_api-1.23.0/edgeimpulse_api/models/admin_get_users_response_all_of.py
--rw-r--r--   0        0        0     3087 2023-05-09 16:43:49.091432 edgeimpulse_api-1.23.0/edgeimpulse_api/models/admin_get_users_response_all_of_users.py
--rw-r--r--   0        0        0     2445 2023-05-09 16:43:49.174778 edgeimpulse_api-1.23.0/edgeimpulse_api/models/admin_list_projects.py
--rw-r--r--   0        0        0     2836 2023-05-09 16:43:49.149252 edgeimpulse_api-1.23.0/edgeimpulse_api/models/admin_list_projects_response.py
--rw-r--r--   0        0        0     6072 2023-05-09 16:43:48.731163 edgeimpulse_api-1.23.0/edgeimpulse_api/models/admin_organization_info_response.py
--rw-r--r--   0        0        0     1974 2023-05-09 16:43:49.380275 edgeimpulse_api-1.23.0/edgeimpulse_api/models/admin_organization_info_response_all_of.py
--rw-r--r--   0        0        0     2728 2023-05-09 16:43:50.149075 edgeimpulse_api-1.23.0/edgeimpulse_api/models/admin_update_organization_request.py
--rw-r--r--   0        0        0     2015 2023-05-09 16:43:49.587638 edgeimpulse_api-1.23.0/edgeimpulse_api/models/admin_update_user_permissions_request.py
--rw-r--r--   0        0        0     2339 2023-05-09 16:43:50.171026 edgeimpulse_api-1.23.0/edgeimpulse_api/models/admin_update_user_request.py
--rw-r--r--   0        0        0     2525 2023-05-09 16:43:49.521400 edgeimpulse_api-1.23.0/edgeimpulse_api/models/akida_edge_learning_config.py
--rw-r--r--   0        0        0     3630 2023-05-09 16:43:48.274962 edgeimpulse_api-1.23.0/edgeimpulse_api/models/anomaly_model_metadata.py
--rw-r--r--   0        0        0     2151 2023-05-09 16:43:48.775483 edgeimpulse_api-1.23.0/edgeimpulse_api/models/anomaly_model_metadata_clusters_inner.py
--rw-r--r--   0        0        0     4011 2023-05-09 16:43:49.825590 edgeimpulse_api-1.23.0/edgeimpulse_api/models/anomaly_model_metadata_response.py
--rw-r--r--   0        0        0     4079 2023-05-09 16:43:48.371224 edgeimpulse_api-1.23.0/edgeimpulse_api/models/anomaly_response.py
--rw-r--r--   0        0        0     3812 2023-05-09 16:43:49.365737 edgeimpulse_api-1.23.0/edgeimpulse_api/models/anomaly_response_all_of.py
--rw-r--r--   0        0        0     2044 2023-05-09 16:43:48.558037 edgeimpulse_api-1.23.0/edgeimpulse_api/models/anomaly_response_all_of_axes.py
--rw-r--r--   0        0        0     3029 2023-05-09 16:43:49.472476 edgeimpulse_api-1.23.0/edgeimpulse_api/models/anomaly_trained_features_response.py
--rw-r--r--   0        0        0     2729 2023-05-09 16:43:49.567326 edgeimpulse_api-1.23.0/edgeimpulse_api/models/anomaly_trained_features_response_all_of.py
--rw-r--r--   0        0        0     2375 2023-05-09 16:43:48.385660 edgeimpulse_api-1.23.0/edgeimpulse_api/models/anomaly_trained_features_response_all_of_data.py
--rw-r--r--   0        0        0      506 2023-05-09 16:43:49.089375 edgeimpulse_api-1.23.0/edgeimpulse_api/models/augmentation_policy_image_enum.py
--rw-r--r--   0        0        0     3635 2023-05-09 16:43:48.745297 edgeimpulse_api-1.23.0/edgeimpulse_api/models/augmentation_policy_spectrogram.py
--rw-r--r--   0        0        0     1895 2023-05-09 16:43:48.268208 edgeimpulse_api-1.23.0/edgeimpulse_api/models/autotune_dsp_request.py
--rw-r--r--   0        0        0     2044 2023-05-09 16:43:49.420660 edgeimpulse_api-1.23.0/edgeimpulse_api/models/bounding_box.py
--rw-r--r--   0        0        0     2151 2023-05-09 16:43:48.298417 edgeimpulse_api-1.23.0/edgeimpulse_api/models/bounding_box_with_score.py
--rw-r--r--   0        0        0     2197 2023-05-09 16:43:48.766462 edgeimpulse_api-1.23.0/edgeimpulse_api/models/build_on_device_model_request.py
--rw-r--r--   0        0        0     2433 2023-05-09 16:43:48.314557 edgeimpulse_api-1.23.0/edgeimpulse_api/models/build_organization_on_device_model_request.py
--rw-r--r--   0        0        0     2041 2023-05-09 16:43:48.586351 edgeimpulse_api-1.23.0/edgeimpulse_api/models/change_password_request.py
--rw-r--r--   0        0        0     3701 2023-05-09 16:43:49.268374 edgeimpulse_api-1.23.0/edgeimpulse_api/models/classify_job_response.py
--rw-r--r--   0        0        0     3394 2023-05-09 16:43:49.933258 edgeimpulse_api-1.23.0/edgeimpulse_api/models/classify_job_response_all_of.py
--rw-r--r--   0        0        0     3769 2023-05-09 16:43:48.982468 edgeimpulse_api-1.23.0/edgeimpulse_api/models/classify_job_response_all_of_accuracy.py
--rw-r--r--   0        0        0     2055 2023-05-09 16:43:49.774118 edgeimpulse_api-1.23.0/edgeimpulse_api/models/classify_job_response_all_of_accuracy_total_summary.py
--rw-r--r--   0        0        0     3255 2023-05-09 16:43:48.139578 edgeimpulse_api-1.23.0/edgeimpulse_api/models/classify_job_response_page.py
--rw-r--r--   0        0        0     2948 2023-05-09 16:43:48.201629 edgeimpulse_api-1.23.0/edgeimpulse_api/models/classify_job_response_page_all_of.py
--rw-r--r--   0        0        0     3932 2023-05-09 16:43:48.299379 edgeimpulse_api-1.23.0/edgeimpulse_api/models/classify_sample_response.py
--rw-r--r--   0        0        0     3644 2023-05-09 16:43:48.249601 edgeimpulse_api-1.23.0/edgeimpulse_api/models/classify_sample_response_all_of.py
--rw-r--r--   0        0        0     4783 2023-05-09 16:43:48.659606 edgeimpulse_api-1.23.0/edgeimpulse_api/models/classify_sample_response_classification.py
--rw-r--r--   0        0        0     2597 2023-05-09 16:43:48.294062 edgeimpulse_api-1.23.0/edgeimpulse_api/models/classify_sample_response_classification_details.py
--rw-r--r--   0        0        0     3004 2023-05-09 16:43:49.231690 edgeimpulse_api-1.23.0/edgeimpulse_api/models/convert_user_request.py
--rw-r--r--   0        0        0     2183 2023-05-09 16:43:49.485549 edgeimpulse_api-1.23.0/edgeimpulse_api/models/count_samples_response.py
--rw-r--r--   0        0        0     1859 2023-05-09 16:43:48.180887 edgeimpulse_api-1.23.0/edgeimpulse_api/models/count_samples_response_all_of.py
--rw-r--r--   0        0        0     2255 2023-05-09 16:43:49.360030 edgeimpulse_api-1.23.0/edgeimpulse_api/models/create_block_version_response.py
--rw-r--r--   0        0        0     1938 2023-05-09 16:43:49.829079 edgeimpulse_api-1.23.0/edgeimpulse_api/models/create_block_version_response_all_of.py
--rw-r--r--   0        0        0     2404 2023-05-09 16:43:48.679670 edgeimpulse_api-1.23.0/edgeimpulse_api/models/create_developer_profile_response.py
--rw-r--r--   0        0        0     2125 2023-05-09 16:43:48.168625 edgeimpulse_api-1.23.0/edgeimpulse_api/models/create_developer_profile_response_all_of.py
--rw-r--r--   0        0        0     2387 2023-05-09 16:43:49.281678 edgeimpulse_api-1.23.0/edgeimpulse_api/models/create_device_request.py
--rw-r--r--   0        0        0     2491 2023-05-09 16:43:48.337325 edgeimpulse_api-1.23.0/edgeimpulse_api/models/create_evaluation_user_response.py
--rw-r--r--   0        0        0     2185 2023-05-09 16:43:48.878239 edgeimpulse_api-1.23.0/edgeimpulse_api/models/create_evaluation_user_response_all_of.py
--rw-r--r--   0        0        0     2600 2023-05-09 16:43:48.546634 edgeimpulse_api-1.23.0/edgeimpulse_api/models/create_organization_portal_request.py
--rw-r--r--   0        0        0     2830 2023-05-09 16:43:49.652918 edgeimpulse_api-1.23.0/edgeimpulse_api/models/create_organization_portal_response.py
--rw-r--r--   0        0        0     2551 2023-05-09 16:43:48.455773 edgeimpulse_api-1.23.0/edgeimpulse_api/models/create_organization_portal_response_all_of.py
--rw-r--r--   0        0        0     1990 2023-05-09 16:43:49.727389 edgeimpulse_api-1.23.0/edgeimpulse_api/models/create_organization_request.py
--rw-r--r--   0        0        0     2454 2023-05-09 16:43:49.684503 edgeimpulse_api-1.23.0/edgeimpulse_api/models/create_organization_response.py
--rw-r--r--   0        0        0     2148 2023-05-09 16:43:49.607568 edgeimpulse_api-1.23.0/edgeimpulse_api/models/create_organization_response_all_of.py
--rw-r--r--   0        0        0     2185 2023-05-09 16:43:48.739314 edgeimpulse_api-1.23.0/edgeimpulse_api/models/create_pipeline_response.py
--rw-r--r--   0        0        0     2254 2023-05-09 16:43:48.129896 edgeimpulse_api-1.23.0/edgeimpulse_api/models/create_project_request.py
--rw-r--r--   0        0        0     2378 2023-05-09 16:43:48.834956 edgeimpulse_api-1.23.0/edgeimpulse_api/models/create_project_response.py
--rw-r--r--   0        0        0     2072 2023-05-09 16:43:49.757130 edgeimpulse_api-1.23.0/edgeimpulse_api/models/create_project_response_all_of.py
--rw-r--r--   0        0        0     2276 2023-05-09 16:43:49.701700 edgeimpulse_api-1.23.0/edgeimpulse_api/models/create_signed_upload_link_request.py
--rw-r--r--   0        0        0     2414 2023-05-09 16:43:49.632189 edgeimpulse_api-1.23.0/edgeimpulse_api/models/create_signed_upload_link_response.py
--rw-r--r--   0        0        0     2135 2023-05-09 16:43:48.356629 edgeimpulse_api-1.23.0/edgeimpulse_api/models/create_signed_upload_link_response_all_of.py
--rw-r--r--   0        0        0     2413 2023-05-09 16:43:49.858744 edgeimpulse_api-1.23.0/edgeimpulse_api/models/create_third_party_auth_request.py
--rw-r--r--   0        0        0     2450 2023-05-09 16:43:48.376676 edgeimpulse_api-1.23.0/edgeimpulse_api/models/create_third_party_auth_response.py
--rw-r--r--   0        0        0     2144 2023-05-09 16:43:48.197540 edgeimpulse_api-1.23.0/edgeimpulse_api/models/create_third_party_auth_response_all_of.py
--rw-r--r--   0        0        0     3835 2023-05-09 16:43:48.755282 edgeimpulse_api-1.23.0/edgeimpulse_api/models/create_user_request.py
--rw-r--r--   0        0        0     2393 2023-05-09 16:43:48.516151 edgeimpulse_api-1.23.0/edgeimpulse_api/models/create_user_response.py
--rw-r--r--   0        0        0     2114 2023-05-09 16:43:48.605545 edgeimpulse_api-1.23.0/edgeimpulse_api/models/create_user_response_all_of.py
--rw-r--r--   0        0        0     2919 2023-05-09 16:43:49.022108 edgeimpulse_api-1.23.0/edgeimpulse_api/models/create_user_third_party_request.py
--rw-r--r--   0        0        0     2672 2023-05-09 16:43:49.797348 edgeimpulse_api-1.23.0/edgeimpulse_api/models/create_user_third_party_response.py
--rw-r--r--   0        0        0     2393 2023-05-09 16:43:48.763635 edgeimpulse_api-1.23.0/edgeimpulse_api/models/create_user_third_party_response_all_of.py
--rw-r--r--   0        0        0     4157 2023-05-09 16:43:48.164790 edgeimpulse_api-1.23.0/edgeimpulse_api/models/create_whitelabel_request.py
--rw-r--r--   0        0        0     2438 2023-05-09 16:43:48.795412 edgeimpulse_api-1.23.0/edgeimpulse_api/models/create_whitelabel_response.py
--rw-r--r--   0        0        0     2121 2023-05-09 16:43:48.297462 edgeimpulse_api-1.23.0/edgeimpulse_api/models/create_whitelabel_response_all_of.py
--rw-r--r--   0        0        0     2051 2023-05-09 16:43:49.869628 edgeimpulse_api-1.23.0/edgeimpulse_api/models/crop_sample_request.py
--rw-r--r--   0        0        0     2248 2023-05-09 16:43:49.286621 edgeimpulse_api-1.23.0/edgeimpulse_api/models/crop_sample_response.py
--rw-r--r--   0        0        0     1943 2023-05-09 16:43:48.724258 edgeimpulse_api-1.23.0/edgeimpulse_api/models/crop_sample_response_all_of.py
--rw-r--r--   0        0        0     3292 2023-05-09 16:43:49.401139 edgeimpulse_api-1.23.0/edgeimpulse_api/models/data_explorer_predictions_response.py
--rw-r--r--   0        0        0     3003 2023-05-09 16:43:48.303265 edgeimpulse_api-1.23.0/edgeimpulse_api/models/data_explorer_predictions_response_all_of.py
--rw-r--r--   0        0        0     2838 2023-05-09 16:43:49.769301 edgeimpulse_api-1.23.0/edgeimpulse_api/models/data_explorer_settings.py
--rw-r--r--   0        0        0     2149 2023-05-09 16:43:50.092021 edgeimpulse_api-1.23.0/edgeimpulse_api/models/dataset_ratio_data.py
--rw-r--r--   0        0        0     2111 2023-05-09 16:43:49.017414 edgeimpulse_api-1.23.0/edgeimpulse_api/models/dataset_ratio_data_ratio.py
--rw-r--r--   0        0        0     1898 2023-05-09 16:43:48.234809 edgeimpulse_api-1.23.0/edgeimpulse_api/models/delete_portal_file_request.py
--rw-r--r--   0        0        0     2230 2023-05-09 16:43:48.582322 edgeimpulse_api-1.23.0/edgeimpulse_api/models/dependency_data.py
--rw-r--r--   0        0        0     2280 2023-05-09 16:43:49.038776 edgeimpulse_api-1.23.0/edgeimpulse_api/models/deploy_pretrained_model_input_audio.py
--rw-r--r--   0        0        0     2155 2023-05-09 16:43:48.846167 edgeimpulse_api-1.23.0/edgeimpulse_api/models/deploy_pretrained_model_input_image.py
--rw-r--r--   0        0        0     2155 2023-05-09 16:43:49.838050 edgeimpulse_api-1.23.0/edgeimpulse_api/models/deploy_pretrained_model_input_other.py
--rw-r--r--   0        0        0     2484 2023-05-09 16:43:49.592296 edgeimpulse_api-1.23.0/edgeimpulse_api/models/deploy_pretrained_model_input_time_series.py
--rw-r--r--   0        0        0     2344 2023-05-09 16:43:49.468370 edgeimpulse_api-1.23.0/edgeimpulse_api/models/deploy_pretrained_model_model_classification.py
--rw-r--r--   0        0        0     2780 2023-05-09 16:43:49.406653 edgeimpulse_api-1.23.0/edgeimpulse_api/models/deploy_pretrained_model_model_object_detection.py
--rw-r--r--   0        0        0     2200 2023-05-09 16:43:48.871167 edgeimpulse_api-1.23.0/edgeimpulse_api/models/deploy_pretrained_model_model_regression.py
--rw-r--r--   0        0        0     4339 2023-05-09 16:43:49.704647 edgeimpulse_api-1.23.0/edgeimpulse_api/models/deploy_pretrained_model_request.py
--rw-r--r--   0        0        0     2833 2023-05-09 16:43:48.693741 edgeimpulse_api-1.23.0/edgeimpulse_api/models/deploy_pretrained_model_request_model_info.py
--rw-r--r--   0        0        0     8503 2023-05-09 16:43:50.138263 edgeimpulse_api-1.23.0/edgeimpulse_api/models/deploy_pretrained_model_request_model_info_input.py
--rw-r--r--   0        0        0     8065 2023-05-09 16:43:49.805276 edgeimpulse_api-1.23.0/edgeimpulse_api/models/deploy_pretrained_model_request_model_info_model.py
--rw-r--r--   0        0        0     5596 2023-05-09 16:43:48.903720 edgeimpulse_api-1.23.0/edgeimpulse_api/models/deployment_target.py
--rw-r--r--   0        0        0     1926 2023-05-09 16:43:49.515956 edgeimpulse_api-1.23.0/edgeimpulse_api/models/deployment_target_badge.py
--rw-r--r--   0        0        0      679 2023-05-09 16:43:48.277841 edgeimpulse_api-1.23.0/edgeimpulse_api/models/deployment_target_engine.py
--rw-r--r--   0        0        0     2702 2023-05-09 16:43:49.452469 edgeimpulse_api-1.23.0/edgeimpulse_api/models/deployment_targets_response.py
--rw-r--r--   0        0        0     2395 2023-05-09 16:43:48.671397 edgeimpulse_api-1.23.0/edgeimpulse_api/models/deployment_targets_response_all_of.py
--rw-r--r--   0        0        0     1983 2023-05-09 16:43:49.028496 edgeimpulse_api-1.23.0/edgeimpulse_api/models/development_board.py
--rw-r--r--   0        0        0     2831 2023-05-09 16:43:48.864748 edgeimpulse_api-1.23.0/edgeimpulse_api/models/development_boards_response.py
--rw-r--r--   0        0        0     2531 2023-05-09 16:43:48.318479 edgeimpulse_api-1.23.0/edgeimpulse_api/models/development_boards_response_all_of.py
--rw-r--r--   0        0        0     2030 2023-05-09 16:43:50.119176 edgeimpulse_api-1.23.0/edgeimpulse_api/models/development_keys.py
--rw-r--r--   0        0        0     2400 2023-05-09 16:43:49.739242 edgeimpulse_api-1.23.0/edgeimpulse_api/models/development_keys_response.py
--rw-r--r--   0        0        0     3677 2023-05-09 16:43:48.590530 edgeimpulse_api-1.23.0/edgeimpulse_api/models/device.py
--rw-r--r--   0        0        0     2199 2023-05-09 16:43:48.857980 edgeimpulse_api-1.23.0/edgeimpulse_api/models/device_name_response.py
--rw-r--r--   0        0        0     1920 2023-05-09 16:43:49.071206 edgeimpulse_api-1.23.0/edgeimpulse_api/models/device_name_response_all_of.py
--rw-r--r--   0        0        0     2231 2023-05-09 16:43:49.678742 edgeimpulse_api-1.23.0/edgeimpulse_api/models/device_sensors_inner.py
--rw-r--r--   0        0        0     2094 2023-05-09 16:43:48.782904 edgeimpulse_api-1.23.0/edgeimpulse_api/models/download.py
--rw-r--r--   0        0        0     1912 2023-05-09 16:43:48.683956 edgeimpulse_api-1.23.0/edgeimpulse_api/models/download_portal_file_request.py
--rw-r--r--   0        0        0     2260 2023-05-09 16:43:49.513032 edgeimpulse_api-1.23.0/edgeimpulse_api/models/download_portal_file_response.py
--rw-r--r--   0        0        0     1954 2023-05-09 16:43:49.806167 edgeimpulse_api-1.23.0/edgeimpulse_api/models/download_portal_file_response_all_of.py
--rw-r--r--   0        0        0     2724 2023-05-09 16:43:49.629870 edgeimpulse_api-1.23.0/edgeimpulse_api/models/dsp_autotuner_results.py
--rw-r--r--   0        0        0     2417 2023-05-09 16:43:49.084711 edgeimpulse_api-1.23.0/edgeimpulse_api/models/dsp_autotuner_results_all_of.py
--rw-r--r--   0        0        0     1968 2023-05-09 16:43:49.233950 edgeimpulse_api-1.23.0/edgeimpulse_api/models/dsp_autotuner_results_all_of_results.py
--rw-r--r--   0        0        0     2870 2023-05-09 16:43:48.280724 edgeimpulse_api-1.23.0/edgeimpulse_api/models/dsp_block.py
--rw-r--r--   0        0        0     1834 2023-05-09 16:43:48.135270 edgeimpulse_api-1.23.0/edgeimpulse_api/models/dsp_config_request.py
--rw-r--r--   0        0        0     3092 2023-05-09 16:43:49.444685 edgeimpulse_api-1.23.0/edgeimpulse_api/models/dsp_config_response.py
--rw-r--r--   0        0        0     2813 2023-05-09 16:43:49.411482 edgeimpulse_api-1.23.0/edgeimpulse_api/models/dsp_config_response_all_of.py
--rw-r--r--   0        0        0     3016 2023-05-09 16:43:48.656520 edgeimpulse_api-1.23.0/edgeimpulse_api/models/dsp_feature_importance_response.py
--rw-r--r--   0        0        0     2728 2023-05-09 16:43:48.406736 edgeimpulse_api-1.23.0/edgeimpulse_api/models/dsp_feature_importance_response_all_of.py
--rw-r--r--   0        0        0     2058 2023-05-09 16:43:48.295464 edgeimpulse_api-1.23.0/edgeimpulse_api/models/dsp_feature_importance_response_all_of_features.py
--rw-r--r--   0        0        0     2572 2023-05-09 16:43:49.641321 edgeimpulse_api-1.23.0/edgeimpulse_api/models/dsp_feature_importance_response_all_of_labels.py
--rw-r--r--   0        0        0     2216 2023-05-09 16:43:48.530998 edgeimpulse_api-1.23.0/edgeimpulse_api/models/dsp_feature_labels_response.py
--rw-r--r--   0        0        0     1920 2023-05-09 16:43:48.124709 edgeimpulse_api-1.23.0/edgeimpulse_api/models/dsp_feature_labels_response_all_of.py
--rw-r--r--   0        0        0     2294 2023-05-09 16:43:48.999585 edgeimpulse_api-1.23.0/edgeimpulse_api/models/dsp_group.py
--rw-r--r--   0        0        0     3628 2023-05-09 16:43:49.402960 edgeimpulse_api-1.23.0/edgeimpulse_api/models/dsp_group_item.py
--rw-r--r--   0        0        0     2190 2023-05-09 16:43:48.361660 edgeimpulse_api-1.23.0/edgeimpulse_api/models/dsp_group_item_select_options_inner.py
--rw-r--r--   0        0        0     2195 2023-05-09 16:43:48.464599 edgeimpulse_api-1.23.0/edgeimpulse_api/models/dsp_group_item_show_if.py
--rw-r--r--   0        0        0     4410 2023-05-09 16:43:49.714625 edgeimpulse_api-1.23.0/edgeimpulse_api/models/dsp_info.py
--rw-r--r--   0        0        0     2210 2023-05-09 16:43:49.558228 edgeimpulse_api-1.23.0/edgeimpulse_api/models/dsp_info_features.py
--rw-r--r--   0        0        0     1885 2023-05-09 16:43:48.861838 edgeimpulse_api-1.23.0/edgeimpulse_api/models/dsp_info_performance.py
--rw-r--r--   0        0        0     5144 2023-05-09 16:43:49.544479 edgeimpulse_api-1.23.0/edgeimpulse_api/models/dsp_metadata.py
--rw-r--r--   0        0        0     2025 2023-05-09 16:43:49.274604 edgeimpulse_api-1.23.0/edgeimpulse_api/models/dsp_metadata_included_samples_inner.py
--rw-r--r--   0        0        0     2566 2023-05-09 16:43:50.098569 edgeimpulse_api-1.23.0/edgeimpulse_api/models/dsp_metadata_output_config.py
--rw-r--r--   0        0        0     2531 2023-05-09 16:43:48.461845 edgeimpulse_api-1.23.0/edgeimpulse_api/models/dsp_metadata_output_config_shape.py
--rw-r--r--   0        0        0     5502 2023-05-09 16:43:49.548941 edgeimpulse_api-1.23.0/edgeimpulse_api/models/dsp_metadata_response.py
--rw-r--r--   0        0        0     3019 2023-05-09 16:43:49.203765 edgeimpulse_api-1.23.0/edgeimpulse_api/models/dsp_performance_all_variants_response.py
--rw-r--r--   0        0        0     2729 2023-05-09 16:43:48.300355 edgeimpulse_api-1.23.0/edgeimpulse_api/models/dsp_performance_all_variants_response_all_of.py
--rw-r--r--   0        0        0     2278 2023-05-09 16:43:49.455673 edgeimpulse_api-1.23.0/edgeimpulse_api/models/dsp_performance_all_variants_response_all_of_performance.py
--rw-r--r--   0        0        0     4639 2023-05-09 16:43:50.135686 edgeimpulse_api-1.23.0/edgeimpulse_api/models/dsp_run_graph.py
--rw-r--r--   0        0        0     1899 2023-05-09 16:43:48.567915 edgeimpulse_api-1.23.0/edgeimpulse_api/models/dsp_run_graph_axis_labels.py
--rw-r--r--   0        0        0     2677 2023-05-09 16:43:48.991509 edgeimpulse_api-1.23.0/edgeimpulse_api/models/dsp_run_request_with_features.py
--rw-r--r--   0        0        0     2151 2023-05-09 16:43:49.012850 edgeimpulse_api-1.23.0/edgeimpulse_api/models/dsp_run_request_without_features.py
--rw-r--r--   0        0        0     2030 2023-05-09 16:43:48.436268 edgeimpulse_api-1.23.0/edgeimpulse_api/models/dsp_run_request_without_features_read_only.py
--rw-r--r--   0        0        0     3513 2023-05-09 16:43:49.237918 edgeimpulse_api-1.23.0/edgeimpulse_api/models/dsp_run_response.py
--rw-r--r--   0        0        0     3234 2023-05-09 16:43:48.177430 edgeimpulse_api-1.23.0/edgeimpulse_api/models/dsp_run_response_all_of.py
--rw-r--r--   0        0        0     1969 2023-05-09 16:43:49.854709 edgeimpulse_api-1.23.0/edgeimpulse_api/models/dsp_run_response_all_of_performance.py
--rw-r--r--   0        0        0     4142 2023-05-09 16:43:48.271335 edgeimpulse_api-1.23.0/edgeimpulse_api/models/dsp_run_response_with_sample.py
--rw-r--r--   0        0        0     3875 2023-05-09 16:43:49.855717 edgeimpulse_api-1.23.0/edgeimpulse_api/models/dsp_run_response_with_sample_all_of.py
--rw-r--r--   0        0        0     3342 2023-05-09 16:43:48.476737 edgeimpulse_api-1.23.0/edgeimpulse_api/models/dsp_sample_features_response.py
--rw-r--r--   0        0        0     3042 2023-05-09 16:43:49.096287 edgeimpulse_api-1.23.0/edgeimpulse_api/models/dsp_sample_features_response_all_of.py
--rw-r--r--   0        0        0     2748 2023-05-09 16:43:49.494944 edgeimpulse_api-1.23.0/edgeimpulse_api/models/dsp_sample_features_response_all_of_data.py
--rw-r--r--   0        0        0     2213 2023-05-09 16:43:49.622507 edgeimpulse_api-1.23.0/edgeimpulse_api/models/dsp_sample_features_response_all_of_sample.py
--rw-r--r--   0        0        0     3353 2023-05-09 16:43:48.383817 edgeimpulse_api-1.23.0/edgeimpulse_api/models/dsp_trained_features_response.py
--rw-r--r--   0        0        0     3053 2023-05-09 16:43:48.700506 edgeimpulse_api-1.23.0/edgeimpulse_api/models/dsp_trained_features_response_all_of.py
--rw-r--r--   0        0        0     2773 2023-05-09 16:43:49.114766 edgeimpulse_api-1.23.0/edgeimpulse_api/models/dsp_trained_features_response_all_of_data.py
--rw-r--r--   0        0        0     2205 2023-05-09 16:43:48.344402 edgeimpulse_api-1.23.0/edgeimpulse_api/models/dsp_trained_features_response_all_of_sample.py
--rw-r--r--   0        0        0     1893 2023-05-09 16:43:49.752367 edgeimpulse_api-1.23.0/edgeimpulse_api/models/edit_sample_label_request.py
--rw-r--r--   0        0        0     2656 2023-05-09 16:43:48.897344 edgeimpulse_api-1.23.0/edgeimpulse_api/models/evaluate_job_response.py
--rw-r--r--   0        0        0     2349 2023-05-09 16:43:48.502673 edgeimpulse_api-1.23.0/edgeimpulse_api/models/evaluate_job_response_all_of.py
--rw-r--r--   0        0        0     2099 2023-05-09 16:43:48.225424 edgeimpulse_api-1.23.0/edgeimpulse_api/models/evaluate_result_value.py
--rw-r--r--   0        0        0     2511 2023-05-09 16:43:48.403922 edgeimpulse_api-1.23.0/edgeimpulse_api/models/export_get_url_response.py
--rw-r--r--   0        0        0     2244 2023-05-09 16:43:48.173788 edgeimpulse_api-1.23.0/edgeimpulse_api/models/export_get_url_response_all_of.py
--rw-r--r--   0        0        0     2373 2023-05-09 16:43:48.423761 edgeimpulse_api-1.23.0/edgeimpulse_api/models/export_original_data_request.py
--rw-r--r--   0        0        0     2021 2023-05-09 16:43:49.316402 edgeimpulse_api-1.23.0/edgeimpulse_api/models/export_wav_data_request.py
--rw-r--r--   0        0        0     2206 2023-05-09 16:43:49.457809 edgeimpulse_api-1.23.0/edgeimpulse_api/models/find_segment_sample_request.py
--rw-r--r--   0        0        0     2804 2023-05-09 16:43:49.938004 edgeimpulse_api-1.23.0/edgeimpulse_api/models/find_segment_sample_response.py
--rw-r--r--   0        0        0     2497 2023-05-09 16:43:49.117871 edgeimpulse_api-1.23.0/edgeimpulse_api/models/find_segment_sample_response_all_of.py
--rw-r--r--   0        0        0     2090 2023-05-09 16:43:49.138519 edgeimpulse_api-1.23.0/edgeimpulse_api/models/find_segment_sample_response_all_of_segments.py
--rw-r--r--   0        0        0     2665 2023-05-09 16:43:48.592423 edgeimpulse_api-1.23.0/edgeimpulse_api/models/find_user_response.py
--rw-r--r--   0        0        0     2358 2023-05-09 16:43:49.949197 edgeimpulse_api-1.23.0/edgeimpulse_api/models/find_user_response_all_of.py
--rw-r--r--   0        0        0     2322 2023-05-09 16:43:48.450116 edgeimpulse_api-1.23.0/edgeimpulse_api/models/find_user_response_all_of_users.py
--rw-r--r--   0        0        0     2507 2023-05-09 16:43:49.305952 edgeimpulse_api-1.23.0/edgeimpulse_api/models/generate_features_request.py
--rw-r--r--   0        0        0     2083 2023-05-09 16:43:48.469317 edgeimpulse_api-1.23.0/edgeimpulse_api/models/generic_api_response.py
--rw-r--r--   0        0        0     2698 2023-05-09 16:43:49.724225 edgeimpulse_api-1.23.0/edgeimpulse_api/models/get_all_third_party_auth_response.py
--rw-r--r--   0        0        0     2391 2023-05-09 16:43:49.836351 edgeimpulse_api-1.23.0/edgeimpulse_api/models/get_all_third_party_auth_response_all_of.py
--rw-r--r--   0        0        0     2713 2023-05-09 16:43:48.874359 edgeimpulse_api-1.23.0/edgeimpulse_api/models/get_all_whitelabels_response.py
--rw-r--r--   0        0        0     2406 2023-05-09 16:43:48.179127 edgeimpulse_api-1.23.0/edgeimpulse_api/models/get_all_whitelabels_response_all_of.py
--rw-r--r--   0        0        0     3400 2023-05-09 16:43:48.526451 edgeimpulse_api-1.23.0/edgeimpulse_api/models/get_data_explorer_features_response.py
--rw-r--r--   0        0        0     3122 2023-05-09 16:43:49.025138 edgeimpulse_api-1.23.0/edgeimpulse_api/models/get_data_explorer_features_response_all_of.py
--rw-r--r--   0        0        0     3752 2023-05-09 16:43:49.939692 edgeimpulse_api-1.23.0/edgeimpulse_api/models/get_data_explorer_settings_response.py
--rw-r--r--   0        0        0     2402 2023-05-09 16:43:49.725618 edgeimpulse_api-1.23.0/edgeimpulse_api/models/get_data_explorer_settings_response_all_of.py
--rw-r--r--   0        0        0     2349 2023-05-09 16:43:49.465356 edgeimpulse_api-1.23.0/edgeimpulse_api/models/get_deployment_response.py
--rw-r--r--   0        0        0     2071 2023-05-09 16:43:49.856769 edgeimpulse_api-1.23.0/edgeimpulse_api/models/get_deployment_response_all_of.py
--rw-r--r--   0        0        0     2434 2023-05-09 16:43:49.102024 edgeimpulse_api-1.23.0/edgeimpulse_api/models/get_device_response.py
--rw-r--r--   0        0        0     2137 2023-05-09 16:43:49.682157 edgeimpulse_api-1.23.0/edgeimpulse_api/models/get_device_response_all_of.py
--rw-r--r--   0        0        0     3930 2023-05-09 16:43:49.669095 edgeimpulse_api-1.23.0/edgeimpulse_api/models/get_impulse_blocks_response.py
--rw-r--r--   0        0        0     3630 2023-05-09 16:43:48.378571 edgeimpulse_api-1.23.0/edgeimpulse_api/models/get_impulse_blocks_response_all_of.py
--rw-r--r--   0        0        0     2454 2023-05-09 16:43:48.153007 edgeimpulse_api-1.23.0/edgeimpulse_api/models/get_impulse_response.py
--rw-r--r--   0        0        0     2157 2023-05-09 16:43:49.600280 edgeimpulse_api-1.23.0/edgeimpulse_api/models/get_impulse_response_all_of.py
--rw-r--r--   0        0        0     2374 2023-05-09 16:43:48.987084 edgeimpulse_api-1.23.0/edgeimpulse_api/models/get_job_response.py
--rw-r--r--   0        0        0     2077 2023-05-09 16:43:49.634225 edgeimpulse_api-1.23.0/edgeimpulse_api/models/get_job_response_all_of.py
--rw-r--r--   0        0        0     2650 2023-05-09 16:43:48.131720 edgeimpulse_api-1.23.0/edgeimpulse_api/models/get_jwt_request.py
--rw-r--r--   0        0        0     2431 2023-05-09 16:43:48.931231 edgeimpulse_api-1.23.0/edgeimpulse_api/models/get_jwt_response.py
--rw-r--r--   0        0        0     2152 2023-05-09 16:43:48.210109 edgeimpulse_api-1.23.0/edgeimpulse_api/models/get_jwt_response_all_of.py
--rw-r--r--   0        0        0     2977 2023-05-09 16:43:48.246522 edgeimpulse_api-1.23.0/edgeimpulse_api/models/get_last_deployment_build_response.py
--rw-r--r--   0        0        0     2699 2023-05-09 16:43:49.001503 edgeimpulse_api-1.23.0/edgeimpulse_api/models/get_last_deployment_build_response_all_of.py
--rw-r--r--   0        0        0     2869 2023-05-09 16:43:49.734371 edgeimpulse_api-1.23.0/edgeimpulse_api/models/get_last_deployment_build_response_all_of_last_build.py
--rw-r--r--   0        0        0     2572 2023-05-09 16:43:49.991277 edgeimpulse_api-1.23.0/edgeimpulse_api/models/get_notes_response.py
--rw-r--r--   0        0        0     2265 2023-05-09 16:43:49.610731 edgeimpulse_api-1.23.0/edgeimpulse_api/models/get_notes_response_all_of.py
--rw-r--r--   0        0        0     2561 2023-05-09 16:43:50.037739 edgeimpulse_api-1.23.0/edgeimpulse_api/models/get_organization_data_item_response.py
--rw-r--r--   0        0        0     2237 2023-05-09 16:43:49.766810 edgeimpulse_api-1.23.0/edgeimpulse_api/models/get_organization_data_item_response_all_of.py
--rw-r--r--   0        0        0     3411 2023-05-09 16:43:48.577795 edgeimpulse_api-1.23.0/edgeimpulse_api/models/get_organization_data_item_transform_jobs_response.py
--rw-r--r--   0        0        0     3111 2023-05-09 16:43:48.358801 edgeimpulse_api-1.23.0/edgeimpulse_api/models/get_organization_data_item_transform_jobs_response_all_of.py
--rw-r--r--   0        0        0     3398 2023-05-09 16:43:48.925385 edgeimpulse_api-1.23.0/edgeimpulse_api/models/get_organization_data_item_transform_jobs_response_all_of_transformation_jobs.py
--rw-r--r--   0        0        0     2576 2023-05-09 16:43:49.129988 edgeimpulse_api-1.23.0/edgeimpulse_api/models/get_organization_dataset_response.py
--rw-r--r--   0        0        0     2252 2023-05-09 16:43:49.205865 edgeimpulse_api-1.23.0/edgeimpulse_api/models/get_organization_dataset_response_all_of.py
--rw-r--r--   0        0        0     2603 2023-05-09 16:43:49.615728 edgeimpulse_api-1.23.0/edgeimpulse_api/models/get_organization_pipelines_response.py
--rw-r--r--   0        0        0     2279 2023-05-09 16:43:48.262207 edgeimpulse_api-1.23.0/edgeimpulse_api/models/get_organization_pipelines_response_all_of.py
--rw-r--r--   0        0        0     3670 2023-05-09 16:43:49.804257 edgeimpulse_api-1.23.0/edgeimpulse_api/models/get_organization_portal_response.py
--rw-r--r--   0        0        0     3391 2023-05-09 16:43:48.368930 edgeimpulse_api-1.23.0/edgeimpulse_api/models/get_organization_portal_response_all_of.py
--rw-r--r--   0        0        0     2323 2023-05-09 16:43:48.641831 edgeimpulse_api-1.23.0/edgeimpulse_api/models/get_organization_projects_data_count_response.py
--rw-r--r--   0        0        0     2905 2023-05-09 16:43:48.222227 edgeimpulse_api-1.23.0/edgeimpulse_api/models/get_performance_calibration_ground_truth_response.py
--rw-r--r--   0        0        0     2598 2023-05-09 16:43:48.968017 edgeimpulse_api-1.23.0/edgeimpulse_api/models/get_performance_calibration_ground_truth_response_all_of.py
--rw-r--r--   0        0        0     3012 2023-05-09 16:43:49.061126 edgeimpulse_api-1.23.0/edgeimpulse_api/models/get_performance_calibration_parameter_sets_response.py
--rw-r--r--   0        0        0     2712 2023-05-09 16:43:48.321615 edgeimpulse_api-1.23.0/edgeimpulse_api/models/get_performance_calibration_parameter_sets_response_all_of.py
--rw-r--r--   0        0        0     2722 2023-05-09 16:43:48.192965 edgeimpulse_api-1.23.0/edgeimpulse_api/models/get_performance_calibration_parameters_response.py
--rw-r--r--   0        0        0     2425 2023-05-09 16:43:49.792418 edgeimpulse_api-1.23.0/edgeimpulse_api/models/get_performance_calibration_parameters_response_all_of.py
--rw-r--r--   0        0        0     2922 2023-05-09 16:43:48.493402 edgeimpulse_api-1.23.0/edgeimpulse_api/models/get_performance_calibration_raw_result_response.py
--rw-r--r--   0        0        0     2615 2023-05-09 16:43:48.906713 edgeimpulse_api-1.23.0/edgeimpulse_api/models/get_performance_calibration_raw_result_response_all_of.py
--rw-r--r--   0        0        0     3151 2023-05-09 16:43:48.120847 edgeimpulse_api-1.23.0/edgeimpulse_api/models/get_performance_calibration_status_response.py
--rw-r--r--   0        0        0     2884 2023-05-09 16:43:48.968976 edgeimpulse_api-1.23.0/edgeimpulse_api/models/get_performance_calibration_status_response_all_of.py
--rw-r--r--   0        0        0     3761 2023-05-09 16:43:49.073954 edgeimpulse_api-1.23.0/edgeimpulse_api/models/get_pretrained_model_response.py
--rw-r--r--   0        0        0     3483 2023-05-09 16:43:49.603057 edgeimpulse_api-1.23.0/edgeimpulse_api/models/get_pretrained_model_response_all_of.py
--rw-r--r--   0        0        0     3861 2023-05-09 16:43:48.482718 edgeimpulse_api-1.23.0/edgeimpulse_api/models/get_pretrained_model_response_all_of_model.py
--rw-r--r--   0        0        0     2978 2023-05-09 16:43:48.921780 edgeimpulse_api-1.23.0/edgeimpulse_api/models/get_pretrained_model_response_all_of_model_info.py
--rw-r--r--   0        0        0     3058 2023-05-09 16:43:48.474857 edgeimpulse_api-1.23.0/edgeimpulse_api/models/get_pretrained_model_response_all_of_model_profile_info.py
--rw-r--r--   0        0        0     2397 2023-05-09 16:43:48.524405 edgeimpulse_api-1.23.0/edgeimpulse_api/models/get_public_metrics_response.py
--rw-r--r--   0        0        0     2073 2023-05-09 16:43:49.311287 edgeimpulse_api-1.23.0/edgeimpulse_api/models/get_public_metrics_response_all_of.py
--rw-r--r--   0        0        0     2767 2023-05-09 16:43:49.093541 edgeimpulse_api-1.23.0/edgeimpulse_api/models/get_sample_metadata_response.py
--rw-r--r--   0        0        0     3044 2023-05-09 16:43:50.066364 edgeimpulse_api-1.23.0/edgeimpulse_api/models/get_sample_response.py
--rw-r--r--   0        0        0     2462 2023-05-09 16:43:49.662197 edgeimpulse_api-1.23.0/edgeimpulse_api/models/get_syntiant_posterior_response.py
--rw-r--r--   0        0        0     2184 2023-05-09 16:43:49.636380 edgeimpulse_api-1.23.0/edgeimpulse_api/models/get_syntiant_posterior_response_all_of.py
--rw-r--r--   0        0        0     2414 2023-05-09 16:43:48.883622 edgeimpulse_api-1.23.0/edgeimpulse_api/models/get_theme_response.py
--rw-r--r--   0        0        0     2117 2023-05-09 16:43:48.791284 edgeimpulse_api-1.23.0/edgeimpulse_api/models/get_theme_response_all_of.py
--rw-r--r--   0        0        0     2592 2023-05-09 16:43:48.696606 edgeimpulse_api-1.23.0/edgeimpulse_api/models/get_themes_response.py
--rw-r--r--   0        0        0     2285 2023-05-09 16:43:49.803346 edgeimpulse_api-1.23.0/edgeimpulse_api/models/get_themes_response_all_of.py
--rw-r--r--   0        0        0     2495 2023-05-09 16:43:49.351544 edgeimpulse_api-1.23.0/edgeimpulse_api/models/get_third_party_auth_response.py
--rw-r--r--   0        0        0     2171 2023-05-09 16:43:48.325628 edgeimpulse_api-1.23.0/edgeimpulse_api/models/get_third_party_auth_response_all_of.py
--rw-r--r--   0        0        0     2703 2023-05-09 16:43:49.348854 edgeimpulse_api-1.23.0/edgeimpulse_api/models/get_user_need_to_set_password_response.py
--rw-r--r--   0        0        0     2436 2023-05-09 16:43:49.276646 edgeimpulse_api-1.23.0/edgeimpulse_api/models/get_user_need_to_set_password_response_all_of.py
--rw-r--r--   0        0        0     7432 2023-05-09 16:43:48.485738 edgeimpulse_api-1.23.0/edgeimpulse_api/models/get_user_response.py
--rw-r--r--   0        0        0     5563 2023-05-09 16:43:49.170540 edgeimpulse_api-1.23.0/edgeimpulse_api/models/get_user_response_all_of.py
--rw-r--r--   0        0        0     2395 2023-05-09 16:43:49.711370 edgeimpulse_api-1.23.0/edgeimpulse_api/models/get_user_response_all_of_whitelabels.py
--rw-r--r--   0        0        0     2307 2023-05-09 16:43:48.985303 edgeimpulse_api-1.23.0/edgeimpulse_api/models/get_whitelabel_domain_response.py
--rw-r--r--   0        0        0     2021 2023-05-09 16:43:48.973073 edgeimpulse_api-1.23.0/edgeimpulse_api/models/get_whitelabel_domain_response_all_of.py
--rw-r--r--   0        0        0     2514 2023-05-09 16:43:49.134770 edgeimpulse_api-1.23.0/edgeimpulse_api/models/get_whitelabel_response.py
--rw-r--r--   0        0        0     2217 2023-05-09 16:43:49.377105 edgeimpulse_api-1.23.0/edgeimpulse_api/models/get_whitelabel_response_all_of.py
--rw-r--r--   0        0        0     2776 2023-05-09 16:43:48.563058 edgeimpulse_api-1.23.0/edgeimpulse_api/models/has_data_explorer_features_response.py
--rw-r--r--   0        0        0     2498 2023-05-09 16:43:49.483053 edgeimpulse_api-1.23.0/edgeimpulse_api/models/has_data_explorer_features_response_all_of.py
--rw-r--r--   0        0        0     3738 2023-05-09 16:43:48.430023 edgeimpulse_api-1.23.0/edgeimpulse_api/models/impulse.py
--rw-r--r--   0        0        0     6723 2023-05-09 16:43:48.395069 edgeimpulse_api-1.23.0/edgeimpulse_api/models/impulse_block_version.py
--rw-r--r--   0        0        0     6814 2023-05-09 16:43:49.518363 edgeimpulse_api-1.23.0/edgeimpulse_api/models/impulse_dsp_block.py
--rw-r--r--   0        0        0     1967 2023-05-09 16:43:49.571930 edgeimpulse_api-1.23.0/edgeimpulse_api/models/impulse_dsp_block_organization.py
--rw-r--r--   0        0        0     8976 2023-05-09 16:43:49.436460 edgeimpulse_api-1.23.0/edgeimpulse_api/models/impulse_input_block.py
--rw-r--r--   0        0        0     5612 2023-05-09 16:43:49.107777 edgeimpulse_api-1.23.0/edgeimpulse_api/models/impulse_learn_block.py
--rw-r--r--   0        0        0     2463 2023-05-09 16:43:49.975287 edgeimpulse_api-1.23.0/edgeimpulse_api/models/input_block.py
--rw-r--r--   0        0        0     2456 2023-05-09 16:43:49.047246 edgeimpulse_api-1.23.0/edgeimpulse_api/models/invite_organization_member_request.py
--rw-r--r--   0        0        0     3435 2023-05-09 16:43:48.710995 edgeimpulse_api-1.23.0/edgeimpulse_api/models/job.py
--rw-r--r--   0        0        0     2713 2023-05-09 16:43:49.530854 edgeimpulse_api-1.23.0/edgeimpulse_api/models/job_summary_response.py
--rw-r--r--   0        0        0     2406 2023-05-09 16:43:48.199538 edgeimpulse_api-1.23.0/edgeimpulse_api/models/job_summary_response_all_of.py
--rw-r--r--   0        0        0     2089 2023-05-09 16:43:49.807971 edgeimpulse_api-1.23.0/edgeimpulse_api/models/job_summary_response_all_of_summary.py
--rw-r--r--   0        0        0     2510 2023-05-09 16:43:49.862208 edgeimpulse_api-1.23.0/edgeimpulse_api/models/keras_model_layer.py
--rw-r--r--   0        0        0     2093 2023-05-09 16:43:49.916372 edgeimpulse_api-1.23.0/edgeimpulse_api/models/keras_model_layer_input.py
--rw-r--r--   0        0        0     2101 2023-05-09 16:43:49.626845 edgeimpulse_api-1.23.0/edgeimpulse_api/models/keras_model_layer_output.py
--rw-r--r--   0        0        0     5189 2023-05-09 16:43:49.450460 edgeimpulse_api-1.23.0/edgeimpulse_api/models/keras_model_metadata.py
--rw-r--r--   0        0        0     4922 2023-05-09 16:43:49.655500 edgeimpulse_api-1.23.0/edgeimpulse_api/models/keras_model_metadata_all_of.py
--rw-r--r--   0        0        0     4792 2023-05-09 16:43:49.032909 edgeimpulse_api-1.23.0/edgeimpulse_api/models/keras_model_metadata_metrics.py
--rw-r--r--   0        0        0     3228 2023-05-09 16:43:49.469439 edgeimpulse_api-1.23.0/edgeimpulse_api/models/keras_model_metadata_metrics_on_device_performance_inner.py
--rw-r--r--   0        0        0     2497 2023-05-09 16:43:49.425637 edgeimpulse_api-1.23.0/edgeimpulse_api/models/keras_model_metadata_metrics_on_device_performance_inner_tflite.py
--rw-r--r--   0        0        0      562 2023-05-09 16:43:49.576961 edgeimpulse_api-1.23.0/edgeimpulse_api/models/keras_model_type_enum.py
--rw-r--r--   0        0        0     9556 2023-05-09 16:43:48.137917 edgeimpulse_api-1.23.0/edgeimpulse_api/models/keras_response.py
--rw-r--r--   0        0        0     9289 2023-05-09 16:43:48.521039 edgeimpulse_api-1.23.0/edgeimpulse_api/models/keras_response_all_of.py
--rw-r--r--   0        0        0     3392 2023-05-09 16:43:49.581556 edgeimpulse_api-1.23.0/edgeimpulse_api/models/keras_visual_layer.py
--rw-r--r--   0        0        0     2310 2023-05-09 16:43:49.354640 edgeimpulse_api-1.23.0/edgeimpulse_api/models/keras_visual_layer_type.py
--rw-r--r--   0        0        0     2529 2023-05-09 16:43:48.155759 edgeimpulse_api-1.23.0/edgeimpulse_api/models/last_modification_date_response.py
--rw-r--r--   0        0        0     2239 2023-05-09 16:43:48.412284 edgeimpulse_api-1.23.0/edgeimpulse_api/models/last_modification_date_response_all_of.py
--rw-r--r--   0        0        0     2633 2023-05-09 16:43:49.394003 edgeimpulse_api-1.23.0/edgeimpulse_api/models/latency_device.py
--rw-r--r--   0        0        0     2424 2023-05-09 16:43:48.285774 edgeimpulse_api-1.23.0/edgeimpulse_api/models/learn_block.py
--rw-r--r--   0        0        0      883 2023-05-09 16:43:49.659664 edgeimpulse_api-1.23.0/edgeimpulse_api/models/learn_block_type.py
--rw-r--r--   0        0        0     2788 2023-05-09 16:43:49.556040 edgeimpulse_api-1.23.0/edgeimpulse_api/models/list_api_keys_response.py
--rw-r--r--   0        0        0     2488 2023-05-09 16:43:48.310996 edgeimpulse_api-1.23.0/edgeimpulse_api/models/list_api_keys_response_all_of.py
--rw-r--r--   0        0        0     2682 2023-05-09 16:43:49.657254 edgeimpulse_api-1.23.0/edgeimpulse_api/models/list_api_keys_response_all_of_api_keys.py
--rw-r--r--   0        0        0     2630 2023-05-09 16:43:49.423584 edgeimpulse_api-1.23.0/edgeimpulse_api/models/list_devices_response.py
--rw-r--r--   0        0        0     2333 2023-05-09 16:43:48.128042 edgeimpulse_api-1.23.0/edgeimpulse_api/models/list_devices_response_all_of.py
--rw-r--r--   0        0        0     2726 2023-05-09 16:43:48.644738 edgeimpulse_api-1.23.0/edgeimpulse_api/models/list_email_response.py
--rw-r--r--   0        0        0     2426 2023-05-09 16:43:48.995652 edgeimpulse_api-1.23.0/edgeimpulse_api/models/list_email_response_all_of.py
--rw-r--r--   0        0        0     2918 2023-05-09 16:43:49.151069 edgeimpulse_api-1.23.0/edgeimpulse_api/models/list_email_response_all_of_emails.py
--rw-r--r--   0        0        0     2813 2023-05-09 16:43:49.613264 edgeimpulse_api-1.23.0/edgeimpulse_api/models/list_hmac_keys_response.py
--rw-r--r--   0        0        0     2513 2023-05-09 16:43:49.068490 edgeimpulse_api-1.23.0/edgeimpulse_api/models/list_hmac_keys_response_all_of.py
--rw-r--r--   0        0        0     2381 2023-05-09 16:43:48.821326 edgeimpulse_api-1.23.0/edgeimpulse_api/models/list_hmac_keys_response_all_of_hmac_keys.py
--rw-r--r--   0        0        0     2745 2023-05-09 16:43:48.154012 edgeimpulse_api-1.23.0/edgeimpulse_api/models/list_jobs_response.py
--rw-r--r--   0        0        0     2445 2023-05-09 16:43:48.894624 edgeimpulse_api-1.23.0/edgeimpulse_api/models/list_jobs_response_all_of.py
--rw-r--r--   0        0        0     2200 2023-05-09 16:43:49.193712 edgeimpulse_api-1.23.0/edgeimpulse_api/models/list_models_response.py
--rw-r--r--   0        0        0     1910 2023-05-09 16:43:50.114731 edgeimpulse_api-1.23.0/edgeimpulse_api/models/list_models_response_all_of.py
--rw-r--r--   0        0        0     2921 2023-05-09 16:43:49.781159 edgeimpulse_api-1.23.0/edgeimpulse_api/models/list_organization_api_keys_response.py
--rw-r--r--   0        0        0     2621 2023-05-09 16:43:48.422037 edgeimpulse_api-1.23.0/edgeimpulse_api/models/list_organization_api_keys_response_all_of.py
--rw-r--r--   0        0        0     2760 2023-05-09 16:43:48.550805 edgeimpulse_api-1.23.0/edgeimpulse_api/models/list_organization_api_keys_response_all_of_api_keys.py
--rw-r--r--   0        0        0     2857 2023-05-09 16:43:48.548614 edgeimpulse_api-1.23.0/edgeimpulse_api/models/list_organization_buckets_response.py
--rw-r--r--   0        0        0     2550 2023-05-09 16:43:49.957760 edgeimpulse_api-1.23.0/edgeimpulse_api/models/list_organization_buckets_response_all_of.py
--rw-r--r--   0        0        0     2919 2023-05-09 16:43:49.865148 edgeimpulse_api-1.23.0/edgeimpulse_api/models/list_organization_buckets_response_all_of_buckets.py
--rw-r--r--   0        0        0     2902 2023-05-09 16:43:49.370576 edgeimpulse_api-1.23.0/edgeimpulse_api/models/list_organization_buckets_user_response.py
--rw-r--r--   0        0        0     2595 2023-05-09 16:43:49.122675 edgeimpulse_api-1.23.0/edgeimpulse_api/models/list_organization_buckets_user_response_all_of.py
--rw-r--r--   0        0        0     3039 2023-05-09 16:43:48.507159 edgeimpulse_api-1.23.0/edgeimpulse_api/models/list_organization_buckets_user_response_all_of_buckets.py
--rw-r--r--   0        0        0     3310 2023-05-09 16:43:49.467246 edgeimpulse_api-1.23.0/edgeimpulse_api/models/list_organization_data_response.py
--rw-r--r--   0        0        0     3031 2023-05-09 16:43:48.354519 edgeimpulse_api-1.23.0/edgeimpulse_api/models/list_organization_data_response_all_of.py
--rw-r--r--   0        0        0     3430 2023-05-09 16:43:50.033936 edgeimpulse_api-1.23.0/edgeimpulse_api/models/list_organization_data_response_all_of_data.py
--rw-r--r--   0        0        0     2887 2023-05-09 16:43:49.799213 edgeimpulse_api-1.23.0/edgeimpulse_api/models/list_organization_deploy_blocks_response.py
--rw-r--r--   0        0        0     2587 2023-05-09 16:43:48.341092 edgeimpulse_api-1.23.0/edgeimpulse_api/models/list_organization_deploy_blocks_response_all_of.py
--rw-r--r--   0        0        0     2824 2023-05-09 16:43:48.727217 edgeimpulse_api-1.23.0/edgeimpulse_api/models/list_organization_dsp_blocks_response.py
--rw-r--r--   0        0        0     2524 2023-05-09 16:43:49.742221 edgeimpulse_api-1.23.0/edgeimpulse_api/models/list_organization_dsp_blocks_response_all_of.py
--rw-r--r--   0        0        0     3353 2023-05-09 16:43:48.633278 edgeimpulse_api-1.23.0/edgeimpulse_api/models/list_organization_files_response.py
--rw-r--r--   0        0        0     3074 2023-05-09 16:43:49.430778 edgeimpulse_api-1.23.0/edgeimpulse_api/models/list_organization_files_response_all_of.py
--rw-r--r--   0        0        0     2792 2023-05-09 16:43:48.631303 edgeimpulse_api-1.23.0/edgeimpulse_api/models/list_organization_pipelines_response.py
--rw-r--r--   0        0        0     2485 2023-05-09 16:43:48.302322 edgeimpulse_api-1.23.0/edgeimpulse_api/models/list_organization_pipelines_response_all_of.py
--rw-r--r--   0        0        0     2857 2023-05-09 16:43:49.146056 edgeimpulse_api-1.23.0/edgeimpulse_api/models/list_organization_portals_response.py
--rw-r--r--   0        0        0     2550 2023-05-09 16:43:49.447212 edgeimpulse_api-1.23.0/edgeimpulse_api/models/list_organization_portals_response_all_of.py
--rw-r--r--   0        0        0     2744 2023-05-09 16:43:49.758914 edgeimpulse_api-1.23.0/edgeimpulse_api/models/list_organization_portals_response_all_of_portals.py
--rw-r--r--   0        0        0     3449 2023-05-09 16:43:48.453951 edgeimpulse_api-1.23.0/edgeimpulse_api/models/list_organization_projects_data_response.py
--rw-r--r--   0        0        0     3142 2023-05-09 16:43:48.598792 edgeimpulse_api-1.23.0/edgeimpulse_api/models/list_organization_projects_data_response_all_of.py
--rw-r--r--   0        0        0     2271 2023-05-09 16:43:48.867607 edgeimpulse_api-1.23.0/edgeimpulse_api/models/list_organization_projects_data_response_all_of_projects.py
--rw-r--r--   0        0        0     2723 2023-05-09 16:43:49.132054 edgeimpulse_api-1.23.0/edgeimpulse_api/models/list_organization_projects_response.py
--rw-r--r--   0        0        0     2416 2023-05-09 16:43:48.810832 edgeimpulse_api-1.23.0/edgeimpulse_api/models/list_organization_projects_response_all_of.py
--rw-r--r--   0        0        0     2857 2023-05-09 16:43:48.237357 edgeimpulse_api-1.23.0/edgeimpulse_api/models/list_organization_secrets_response.py
--rw-r--r--   0        0        0     2550 2023-05-09 16:43:48.273355 edgeimpulse_api-1.23.0/edgeimpulse_api/models/list_organization_secrets_response_all_of.py
--rw-r--r--   0        0        0     2265 2023-05-09 16:43:49.729230 edgeimpulse_api-1.23.0/edgeimpulse_api/models/list_organization_secrets_response_all_of_secrets.py
--rw-r--r--   0        0        0     3103 2023-05-09 16:43:48.509267 edgeimpulse_api-1.23.0/edgeimpulse_api/models/list_organization_transfer_learning_blocks_response.py
--rw-r--r--   0        0        0     2803 2023-05-09 16:43:49.802451 edgeimpulse_api-1.23.0/edgeimpulse_api/models/list_organization_transfer_learning_blocks_response_all_of.py
--rw-r--r--   0        0        0     3055 2023-05-09 16:43:48.960973 edgeimpulse_api-1.23.0/edgeimpulse_api/models/list_organization_transformation_blocks_response.py
--rw-r--r--   0        0        0     2755 2023-05-09 16:43:49.278795 edgeimpulse_api-1.23.0/edgeimpulse_api/models/list_organization_transformation_blocks_response_all_of.py
--rw-r--r--   0        0        0     2786 2023-05-09 16:43:49.479725 edgeimpulse_api-1.23.0/edgeimpulse_api/models/list_organizations_response.py
--rw-r--r--   0        0        0     2486 2023-05-09 16:43:50.156386 edgeimpulse_api-1.23.0/edgeimpulse_api/models/list_organizations_response_all_of.py
--rw-r--r--   0        0        0     1937 2023-05-09 16:43:48.818517 edgeimpulse_api-1.23.0/edgeimpulse_api/models/list_portal_files_in_folder_request.py
--rw-r--r--   0        0        0     2713 2023-05-09 16:43:49.570071 edgeimpulse_api-1.23.0/edgeimpulse_api/models/list_portal_files_in_folder_response.py
--rw-r--r--   0        0        0     2416 2023-05-09 16:43:48.915334 edgeimpulse_api-1.23.0/edgeimpulse_api/models/list_portal_files_in_folder_response_all_of.py
--rw-r--r--   0        0        0     2290 2023-05-09 16:43:49.332883 edgeimpulse_api-1.23.0/edgeimpulse_api/models/list_projects.py
--rw-r--r--   0        0        0     2681 2023-05-09 16:43:50.142131 edgeimpulse_api-1.23.0/edgeimpulse_api/models/list_projects_response.py
--rw-r--r--   0        0        0     2553 2023-05-09 16:43:49.059220 edgeimpulse_api-1.23.0/edgeimpulse_api/models/list_public_projects.py
--rw-r--r--   0        0        0     2944 2023-05-09 16:43:48.447216 edgeimpulse_api-1.23.0/edgeimpulse_api/models/list_public_projects_response.py
--rw-r--r--   0        0        0     2815 2023-05-09 16:43:49.404817 edgeimpulse_api-1.23.0/edgeimpulse_api/models/list_public_versions_response.py
--rw-r--r--   0        0        0     2508 2023-05-09 16:43:49.319260 edgeimpulse_api-1.23.0/edgeimpulse_api/models/list_public_versions_response_all_of.py
--rw-r--r--   0        0        0     2290 2023-05-09 16:43:49.834530 edgeimpulse_api-1.23.0/edgeimpulse_api/models/list_public_versions_response_all_of_versions.py
--rw-r--r--   0        0        0     2754 2023-05-09 16:43:48.434023 edgeimpulse_api-1.23.0/edgeimpulse_api/models/list_samples_response.py
--rw-r--r--   0        0        0     2454 2023-05-09 16:43:48.797933 edgeimpulse_api-1.23.0/edgeimpulse_api/models/list_samples_response_all_of.py
--rw-r--r--   0        0        0     3933 2023-05-09 16:43:48.675954 edgeimpulse_api-1.23.0/edgeimpulse_api/models/list_versions_response.py
--rw-r--r--   0        0        0     3633 2023-05-09 16:43:48.296491 edgeimpulse_api-1.23.0/edgeimpulse_api/models/list_versions_response_all_of.py
--rw-r--r--   0        0        0     2353 2023-05-09 16:43:49.977344 edgeimpulse_api-1.23.0/edgeimpulse_api/models/list_versions_response_all_of_bucket.py
--rw-r--r--   0        0        0     2053 2023-05-09 16:43:48.588803 edgeimpulse_api-1.23.0/edgeimpulse_api/models/list_versions_response_all_of_custom_learn_blocks.py
--rw-r--r--   0        0        0     3960 2023-05-09 16:43:48.544127 edgeimpulse_api-1.23.0/edgeimpulse_api/models/list_versions_response_all_of_versions.py
--rw-r--r--   0        0        0     2900 2023-05-09 16:43:49.807044 edgeimpulse_api-1.23.0/edgeimpulse_api/models/log_stdout_response.py
--rw-r--r--   0        0        0     2600 2023-05-09 16:43:49.863249 edgeimpulse_api-1.23.0/edgeimpulse_api/models/log_stdout_response_all_of.py
--rw-r--r--   0        0        0     2441 2023-05-09 16:43:48.653937 edgeimpulse_api-1.23.0/edgeimpulse_api/models/log_stdout_response_all_of_stdout.py
--rw-r--r--   0        0        0     2191 2023-05-09 16:43:48.886874 edgeimpulse_api-1.23.0/edgeimpulse_api/models/log_website_pageview_request.py
--rw-r--r--   0        0        0     2217 2023-05-09 16:43:48.215981 edgeimpulse_api-1.23.0/edgeimpulse_api/models/login_response.py
--rw-r--r--   0        0        0     1911 2023-05-09 16:43:49.526668 edgeimpulse_api-1.23.0/edgeimpulse_api/models/login_response_all_of.py
--rw-r--r--   0        0        0     2521 2023-05-09 16:43:49.690224 edgeimpulse_api-1.23.0/edgeimpulse_api/models/model_prediction.py
--rw-r--r--   0        0        0     2895 2023-05-09 16:43:49.329944 edgeimpulse_api-1.23.0/edgeimpulse_api/models/model_result.py
--rw-r--r--   0        0        0     5046 2023-05-09 16:43:49.931830 edgeimpulse_api-1.23.0/edgeimpulse_api/models/model_variant_stats.py
--rw-r--r--   0        0        0     2128 2023-05-09 16:43:49.300067 edgeimpulse_api-1.23.0/edgeimpulse_api/models/move_raw_data_request.py
--rw-r--r--   0        0        0     2687 2023-05-09 16:43:49.866958 edgeimpulse_api-1.23.0/edgeimpulse_api/models/note.py
--rw-r--r--   0        0        0     2221 2023-05-09 16:43:49.308225 edgeimpulse_api-1.23.0/edgeimpulse_api/models/object_detection_auto_label_request.py
--rw-r--r--   0        0        0     2994 2023-05-09 16:43:49.228078 edgeimpulse_api-1.23.0/edgeimpulse_api/models/object_detection_auto_label_response.py
--rw-r--r--   0        0        0     2705 2023-05-09 16:43:48.443908 edgeimpulse_api-1.23.0/edgeimpulse_api/models/object_detection_auto_label_response_all_of.py
--rw-r--r--   0        0        0     2275 2023-05-09 16:43:49.943411 edgeimpulse_api-1.23.0/edgeimpulse_api/models/object_detection_auto_label_response_all_of_results.py
--rw-r--r--   0        0        0     2368 2023-05-09 16:43:49.624322 edgeimpulse_api-1.23.0/edgeimpulse_api/models/object_detection_label_queue_count_response.py
--rw-r--r--   0        0        0     2051 2023-05-09 16:43:48.649344 edgeimpulse_api-1.23.0/edgeimpulse_api/models/object_detection_label_queue_count_response_all_of.py
--rw-r--r--   0        0        0     2887 2023-05-09 16:43:50.096130 edgeimpulse_api-1.23.0/edgeimpulse_api/models/object_detection_label_queue_response.py
--rw-r--r--   0        0        0     2580 2023-05-09 16:43:49.692689 edgeimpulse_api-1.23.0/edgeimpulse_api/models/object_detection_label_queue_response_all_of.py
--rw-r--r--   0        0        0      621 2023-05-09 16:43:49.779300 edgeimpulse_api-1.23.0/edgeimpulse_api/models/object_detection_last_layer.py
--rw-r--r--   0        0        0     6418 2023-05-09 16:43:49.505508 edgeimpulse_api-1.23.0/edgeimpulse_api/models/optimize_config.py
--rw-r--r--   0        0        0     6871 2023-05-09 16:43:50.073593 edgeimpulse_api-1.23.0/edgeimpulse_api/models/optimize_config_response.py
--rw-r--r--   0        0        0     1920 2023-05-09 16:43:49.416872 edgeimpulse_api-1.23.0/edgeimpulse_api/models/optimize_config_response_all_of.py
--rw-r--r--   0        0        0     2067 2023-05-09 16:43:49.408795 edgeimpulse_api-1.23.0/edgeimpulse_api/models/optimize_config_target_device.py
--rw-r--r--   0        0        0     2271 2023-05-09 16:43:48.190157 edgeimpulse_api-1.23.0/edgeimpulse_api/models/optimize_dsp_parameters_response.py
--rw-r--r--   0        0        0     1964 2023-05-09 16:43:49.853706 edgeimpulse_api-1.23.0/edgeimpulse_api/models/optimize_dsp_parameters_response_all_of.py
--rw-r--r--   0        0        0     2756 2023-05-09 16:43:49.852479 edgeimpulse_api-1.23.0/edgeimpulse_api/models/optimize_space_response.py
--rw-r--r--   0        0        0     2456 2023-05-09 16:43:48.151271 edgeimpulse_api-1.23.0/edgeimpulse_api/models/optimize_space_response_all_of.py
--rw-r--r--   0        0        0     4897 2023-05-09 16:43:48.497594 edgeimpulse_api-1.23.0/edgeimpulse_api/models/optimize_state_response.py
--rw-r--r--   0        0        0     4618 2023-05-09 16:43:48.911371 edgeimpulse_api-1.23.0/edgeimpulse_api/models/optimize_state_response_all_of.py
--rw-r--r--   0        0        0     3419 2023-05-09 16:43:48.536509 edgeimpulse_api-1.23.0/edgeimpulse_api/models/optimize_state_response_all_of_status.py
--rw-r--r--   0        0        0     2366 2023-05-09 16:43:49.748888 edgeimpulse_api-1.23.0/edgeimpulse_api/models/optimize_state_response_all_of_workers.py
--rw-r--r--   0        0        0     2760 2023-05-09 16:43:49.594135 edgeimpulse_api-1.23.0/edgeimpulse_api/models/optimize_transfer_learning_models_response.py
--rw-r--r--   0        0        0     2463 2023-05-09 16:43:50.029359 edgeimpulse_api-1.23.0/edgeimpulse_api/models/optimize_transfer_learning_models_response_all_of.py
--rw-r--r--   0        0        0     4682 2023-05-09 16:43:48.989278 edgeimpulse_api-1.23.0/edgeimpulse_api/models/optimize_transfer_learning_models_response_all_of_models.py
--rw-r--r--   0        0        0     3774 2023-05-09 16:43:48.610928 edgeimpulse_api-1.23.0/edgeimpulse_api/models/organization.py
--rw-r--r--   0        0        0     2359 2023-05-09 16:43:49.578599 edgeimpulse_api-1.23.0/edgeimpulse_api/models/organization_add_data_folder_request.py
--rw-r--r--   0        0        0     2498 2023-05-09 16:43:50.185068 edgeimpulse_api-1.23.0/edgeimpulse_api/models/organization_add_data_folder_response.py
--rw-r--r--   0        0        0     2209 2023-05-09 16:43:50.026449 edgeimpulse_api-1.23.0/edgeimpulse_api/models/organization_add_data_folder_response_all_of.py
--rw-r--r--   0        0        0     8200 2023-05-09 16:43:49.646437 edgeimpulse_api-1.23.0/edgeimpulse_api/models/organization_create_project.py
--rw-r--r--   0        0        0     4778 2023-05-09 16:43:49.082177 edgeimpulse_api-1.23.0/edgeimpulse_api/models/organization_create_project_request.py
--rw-r--r--   0        0        0     2543 2023-05-09 16:43:48.348980 edgeimpulse_api-1.23.0/edgeimpulse_api/models/organization_create_project_response.py
--rw-r--r--   0        0        0     2237 2023-05-09 16:43:50.078669 edgeimpulse_api-1.23.0/edgeimpulse_api/models/organization_create_project_response_all_of.py
--rw-r--r--   0        0        0     2704 2023-05-09 16:43:50.194435 edgeimpulse_api-1.23.0/edgeimpulse_api/models/organization_create_project_status_response.py
--rw-r--r--   0        0        0     2407 2023-05-09 16:43:49.051411 edgeimpulse_api-1.23.0/edgeimpulse_api/models/organization_create_project_status_response_all_of.py
--rw-r--r--   0        0        0     2501 2023-05-09 16:43:48.541194 edgeimpulse_api-1.23.0/edgeimpulse_api/models/organization_create_project_transformation_summary.py
--rw-r--r--   0        0        0     8927 2023-05-09 16:43:49.153475 edgeimpulse_api-1.23.0/edgeimpulse_api/models/organization_create_project_with_files.py
--rw-r--r--   0        0        0     2558 2023-05-09 16:43:49.528604 edgeimpulse_api-1.23.0/edgeimpulse_api/models/organization_create_project_with_files_all_of.py
--rw-r--r--   0        0        0     2886 2023-05-09 16:43:50.061876 edgeimpulse_api-1.23.0/edgeimpulse_api/models/organization_create_project_with_files_all_of_files.py
--rw-r--r--   0        0        0     3476 2023-05-09 16:43:48.664032 edgeimpulse_api-1.23.0/edgeimpulse_api/models/organization_data_item.py
--rw-r--r--   0        0        0     2103 2023-05-09 16:43:48.636415 edgeimpulse_api-1.23.0/edgeimpulse_api/models/organization_data_item_files_inner.py
--rw-r--r--   0        0        0     2517 2023-05-09 16:43:49.649276 edgeimpulse_api-1.23.0/edgeimpulse_api/models/organization_dataset.py
--rw-r--r--   0        0        0     4689 2023-05-09 16:43:48.228220 edgeimpulse_api-1.23.0/edgeimpulse_api/models/organization_deploy_block.py
--rw-r--r--   0        0        0     3646 2023-05-09 16:43:49.502346 edgeimpulse_api-1.23.0/edgeimpulse_api/models/organization_dsp_block.py
--rw-r--r--   0        0        0     3037 2023-05-09 16:43:49.638792 edgeimpulse_api-1.23.0/edgeimpulse_api/models/organization_get_create_projects_response.py
--rw-r--r--   0        0        0     2737 2023-05-09 16:43:48.734907 edgeimpulse_api-1.23.0/edgeimpulse_api/models/organization_get_create_projects_response_all_of.py
--rw-r--r--   0        0        0     5309 2023-05-09 16:43:49.840142 edgeimpulse_api-1.23.0/edgeimpulse_api/models/organization_get_create_projects_response_all_of_jobs.py
--rw-r--r--   0        0        0     5938 2023-05-09 16:43:49.201606 edgeimpulse_api-1.23.0/edgeimpulse_api/models/organization_info_response.py
--rw-r--r--   0        0        0     5648 2023-05-09 16:43:49.362592 edgeimpulse_api-1.23.0/edgeimpulse_api/models/organization_info_response_all_of.py
--rw-r--r--   0        0        0     2458 2023-05-09 16:43:48.239519 edgeimpulse_api-1.23.0/edgeimpulse_api/models/organization_info_response_all_of_default_compute_limits.py
--rw-r--r--   0        0        0     2600 2023-05-09 16:43:49.454030 edgeimpulse_api-1.23.0/edgeimpulse_api/models/organization_info_response_all_of_entitlement_limits.py
--rw-r--r--   0        0        0     2639 2023-05-09 16:43:49.120462 edgeimpulse_api-1.23.0/edgeimpulse_api/models/organization_metrics_response.py
--rw-r--r--   0        0        0     2315 2023-05-09 16:43:48.381760 edgeimpulse_api-1.23.0/edgeimpulse_api/models/organization_metrics_response_all_of.py
--rw-r--r--   0        0        0     3491 2023-05-09 16:43:48.409742 edgeimpulse_api-1.23.0/edgeimpulse_api/models/organization_metrics_response_all_of_metrics.py
--rw-r--r--   0        0        0     6114 2023-05-09 16:43:49.597004 edgeimpulse_api-1.23.0/edgeimpulse_api/models/organization_pipeline.py
--rw-r--r--   0        0        0     2595 2023-05-09 16:43:49.326878 edgeimpulse_api-1.23.0/edgeimpulse_api/models/organization_pipeline_feeding_into_dataset.py
--rw-r--r--   0        0        0     2275 2023-05-09 16:43:49.867883 edgeimpulse_api-1.23.0/edgeimpulse_api/models/organization_pipeline_feeding_into_project.py
--rw-r--r--   0        0        0     2314 2023-05-09 16:43:48.839668 edgeimpulse_api-1.23.0/edgeimpulse_api/models/organization_pipeline_item_count.py
--rw-r--r--   0        0        0     4109 2023-05-09 16:43:49.127860 edgeimpulse_api-1.23.0/edgeimpulse_api/models/organization_pipeline_run.py
--rw-r--r--   0        0        0     4815 2023-05-09 16:43:48.622940 edgeimpulse_api-1.23.0/edgeimpulse_api/models/organization_pipeline_run_step.py
--rw-r--r--   0        0        0     4415 2023-05-09 16:43:49.673964 edgeimpulse_api-1.23.0/edgeimpulse_api/models/organization_pipeline_step.py
--rw-r--r--   0        0        0     2351 2023-05-09 16:43:48.565611 edgeimpulse_api-1.23.0/edgeimpulse_api/models/organization_projects_data_batch_disable_response.py
--rw-r--r--   0        0        0     2344 2023-05-09 16:43:49.842786 edgeimpulse_api-1.23.0/edgeimpulse_api/models/organization_projects_data_batch_enable_response.py
--rw-r--r--   0        0        0     2037 2023-05-09 16:43:49.272525 edgeimpulse_api-1.23.0/edgeimpulse_api/models/organization_projects_data_batch_request.py
--rw-r--r--   0        0        0     4414 2023-05-09 16:43:48.706036 edgeimpulse_api-1.23.0/edgeimpulse_api/models/organization_transfer_learning_block.py
--rw-r--r--   0        0        0      611 2023-05-09 16:43:49.716955 edgeimpulse_api-1.23.0/edgeimpulse_api/models/organization_transfer_learning_operates_on.py
--rw-r--r--   0        0        0     5168 2023-05-09 16:43:49.396759 edgeimpulse_api-1.23.0/edgeimpulse_api/models/organization_transformation_block.py
--rw-r--r--   0        0        0     3889 2023-05-09 16:43:48.126526 edgeimpulse_api-1.23.0/edgeimpulse_api/models/organization_update_pipeline_body.py
--rw-r--r--   0        0        0     3609 2023-05-09 16:43:49.886841 edgeimpulse_api-1.23.0/edgeimpulse_api/models/organization_user.py
--rw-r--r--   0        0        0     2104 2023-05-09 16:43:48.207923 edgeimpulse_api-1.23.0/edgeimpulse_api/models/performance_calibration_detection.py
--rw-r--r--   0        0        0     3434 2023-05-09 16:43:49.041110 edgeimpulse_api-1.23.0/edgeimpulse_api/models/performance_calibration_false_positive.py
--rw-r--r--   0        0        0     3770 2023-05-09 16:43:49.006596 edgeimpulse_api-1.23.0/edgeimpulse_api/models/performance_calibration_ground_truth.py
--rw-r--r--   0        0        0     2477 2023-05-09 16:43:48.220286 edgeimpulse_api-1.23.0/edgeimpulse_api/models/performance_calibration_ground_truth_samples_inner.py
--rw-r--r--   0        0        0     4880 2023-05-09 16:43:48.195374 edgeimpulse_api-1.23.0/edgeimpulse_api/models/performance_calibration_parameter_set.py
--rw-r--r--   0        0        0     2255 2023-05-09 16:43:49.507323 edgeimpulse_api-1.23.0/edgeimpulse_api/models/performance_calibration_parameter_set_aggregate_stats.py
--rw-r--r--   0        0        0     4092 2023-05-09 16:43:48.346595 edgeimpulse_api-1.23.0/edgeimpulse_api/models/performance_calibration_parameter_set_stats_inner.py
--rw-r--r--   0        0        0     3007 2023-05-09 16:43:50.100620 edgeimpulse_api-1.23.0/edgeimpulse_api/models/performance_calibration_parameters.py
--rw-r--r--   0        0        0     2585 2023-05-09 16:43:48.850979 edgeimpulse_api-1.23.0/edgeimpulse_api/models/performance_calibration_parameters_standard.py
--rw-r--r--   0        0        0     2250 2023-05-09 16:43:49.190774 edgeimpulse_api-1.23.0/edgeimpulse_api/models/performance_calibration_raw_detection.py
--rw-r--r--   0        0        0     2366 2023-05-09 16:43:49.666997 edgeimpulse_api-1.23.0/edgeimpulse_api/models/performance_calibration_save_parameter_set_request.py
--rw-r--r--   0        0        0     2412 2023-05-09 16:43:49.540784 edgeimpulse_api-1.23.0/edgeimpulse_api/models/performance_calibration_upload_labeled_audio_response.py
--rw-r--r--   0        0        0     2106 2023-05-09 16:43:48.459050 edgeimpulse_api-1.23.0/edgeimpulse_api/models/performance_calibration_upload_labeled_audio_response_all_of.py
--rw-r--r--   0        0        0     1250 2023-05-09 16:43:48.518226 edgeimpulse_api-1.23.0/edgeimpulse_api/models/permission.py
--rw-r--r--   0        0        0     2211 2023-05-09 16:43:49.643225 edgeimpulse_api-1.23.0/edgeimpulse_api/models/portal_file.py
--rw-r--r--   0        0        0     2413 2023-05-09 16:43:48.666554 edgeimpulse_api-1.23.0/edgeimpulse_api/models/portal_info_response.py
--rw-r--r--   0        0        0     2666 2023-05-09 16:43:49.112406 edgeimpulse_api-1.23.0/edgeimpulse_api/models/pretrained_model_tensor.py
--rw-r--r--   0        0        0     2955 2023-05-09 16:43:49.489624 edgeimpulse_api-1.23.0/edgeimpulse_api/models/profile_model_info.py
--rw-r--r--   0        0        0     2640 2023-05-09 16:43:49.049418 edgeimpulse_api-1.23.0/edgeimpulse_api/models/profile_model_info_memory.py
--rw-r--r--   0        0        0     1918 2023-05-09 16:43:49.413899 edgeimpulse_api-1.23.0/edgeimpulse_api/models/profile_model_info_memory_eon.py
--rw-r--r--   0        0        0     2065 2023-05-09 16:43:49.030552 edgeimpulse_api-1.23.0/edgeimpulse_api/models/profile_model_info_memory_tflite.py
--rw-r--r--   0        0        0     4335 2023-05-09 16:43:49.761255 edgeimpulse_api-1.23.0/edgeimpulse_api/models/profile_model_table.py
--rw-r--r--   0        0        0     2780 2023-05-09 16:43:48.831854 edgeimpulse_api-1.23.0/edgeimpulse_api/models/profile_model_table_mcu.py
--rw-r--r--   0        0        0     2565 2023-05-09 16:43:49.110396 edgeimpulse_api-1.23.0/edgeimpulse_api/models/profile_model_table_mcu_memory.py
--rw-r--r--   0        0        0     2250 2023-05-09 16:43:48.944919 edgeimpulse_api-1.23.0/edgeimpulse_api/models/profile_model_table_mpu.py
--rw-r--r--   0        0        0     2201 2023-05-09 16:43:49.719603 edgeimpulse_api-1.23.0/edgeimpulse_api/models/profile_tf_lite_request.py
--rw-r--r--   0        0        0     3292 2023-05-09 16:43:49.373630 edgeimpulse_api-1.23.0/edgeimpulse_api/models/profile_tf_lite_response.py
--rw-r--r--   0        0        0     6139 2023-05-09 16:43:49.986100 edgeimpulse_api-1.23.0/edgeimpulse_api/models/project.py
--rw-r--r--   0        0        0     3506 2023-05-09 16:43:48.718247 edgeimpulse_api-1.23.0/edgeimpulse_api/models/project_collaborator.py
--rw-r--r--   0        0        0     1895 2023-05-09 16:43:49.550696 edgeimpulse_api-1.23.0/edgeimpulse_api/models/project_collaborator_all_of.py
--rw-r--r--   0        0        0     2416 2023-05-09 16:43:49.789963 edgeimpulse_api-1.23.0/edgeimpulse_api/models/project_data_axes_summary_response.py
--rw-r--r--   0        0        0     2116 2023-05-09 16:43:48.204789 edgeimpulse_api-1.23.0/edgeimpulse_api/models/project_data_axes_summary_response_all_of.py
--rw-r--r--   0        0        0     2281 2023-05-09 16:43:49.053753 edgeimpulse_api-1.23.0/edgeimpulse_api/models/project_data_interval_response.py
--rw-r--r--   0        0        0     1964 2023-05-09 16:43:48.528191 edgeimpulse_api-1.23.0/edgeimpulse_api/models/project_data_interval_response_all_of.py
--rw-r--r--   0        0        0     2235 2023-05-09 16:43:48.301356 edgeimpulse_api-1.23.0/edgeimpulse_api/models/project_data_summary.py
--rw-r--r--   0        0        0     6500 2023-05-09 16:43:49.694743 edgeimpulse_api-1.23.0/edgeimpulse_api/models/project_deployment_target.py
--rw-r--r--   0        0        0     2706 2023-05-09 16:43:49.911504 edgeimpulse_api-1.23.0/edgeimpulse_api/models/project_deployment_target_all_of.py
--rw-r--r--   0        0        0     2780 2023-05-09 16:43:49.265429 edgeimpulse_api-1.23.0/edgeimpulse_api/models/project_deployment_targets_response.py
--rw-r--r--   0        0        0     2473 2023-05-09 16:43:48.243545 edgeimpulse_api-1.23.0/edgeimpulse_api/models/project_deployment_targets_response_all_of.py
--rw-r--r--   0        0        0     2680 2023-05-09 16:43:48.283836 edgeimpulse_api-1.23.0/edgeimpulse_api/models/project_downloads_response.py
--rw-r--r--   0        0        0     2373 2023-05-09 16:43:49.004181 edgeimpulse_api-1.23.0/edgeimpulse_api/models/project_downloads_response_all_of.py
--rw-r--r--   0        0        0    13206 2023-05-09 16:43:50.019435 edgeimpulse_api-1.23.0/edgeimpulse_api/models/project_info_response.py
--rw-r--r--   0        0        0    12939 2023-05-09 16:43:50.070015 edgeimpulse_api-1.23.0/edgeimpulse_api/models/project_info_response_all_of.py
--rw-r--r--   0        0        0     3130 2023-05-09 16:43:48.146193 edgeimpulse_api-1.23.0/edgeimpulse_api/models/project_info_response_all_of_acquisition_settings.py
--rw-r--r--   0        0        0     2723 2023-05-09 16:43:49.883661 edgeimpulse_api-1.23.0/edgeimpulse_api/models/project_info_response_all_of_compute_time.py
--rw-r--r--   0        0        0     2997 2023-05-09 16:43:49.262105 edgeimpulse_api-1.23.0/edgeimpulse_api/models/project_info_response_all_of_data_summary_per_category.py
--rw-r--r--   0        0        0     2808 2023-05-09 16:43:48.505197 edgeimpulse_api-1.23.0/edgeimpulse_api/models/project_info_response_all_of_deploy_settings.py
--rw-r--r--   0        0        0     2339 2023-05-09 16:43:49.754931 edgeimpulse_api-1.23.0/edgeimpulse_api/models/project_info_response_all_of_experiments.py
--rw-r--r--   0        0        0     2285 2023-05-09 16:43:49.820371 edgeimpulse_api-1.23.0/edgeimpulse_api/models/project_info_response_all_of_impulse.py
--rw-r--r--   0        0        0     2726 2023-05-09 16:43:49.253287 edgeimpulse_api-1.23.0/edgeimpulse_api/models/project_info_response_all_of_performance.py
--rw-r--r--   0        0        0     1977 2023-05-09 16:43:49.864194 edgeimpulse_api-1.23.0/edgeimpulse_api/models/project_info_response_all_of_readme.py
--rw-r--r--   0        0        0     2225 2023-05-09 16:43:49.475994 edgeimpulse_api-1.23.0/edgeimpulse_api/models/project_info_response_all_of_show_getting_started_wizard.py
--rw-r--r--   0        0        0     2735 2023-05-09 16:43:48.489172 edgeimpulse_api-1.23.0/edgeimpulse_api/models/project_info_response_all_of_urls.py
--rw-r--r--   0        0        0     2478 2023-05-09 16:43:48.387866 edgeimpulse_api-1.23.0/edgeimpulse_api/models/project_info_summary_response.py
--rw-r--r--   0        0        0     2172 2023-05-09 16:43:48.661914 edgeimpulse_api-1.23.0/edgeimpulse_api/models/project_info_summary_response_all_of.py
--rw-r--r--   0        0        0     3554 2023-05-09 16:43:48.218412 edgeimpulse_api-1.23.0/edgeimpulse_api/models/project_private_data.py
--rw-r--r--   0        0        0     4396 2023-05-09 16:43:48.212167 edgeimpulse_api-1.23.0/edgeimpulse_api/models/project_public_data.py
--rw-r--r--   0        0        0     1928 2023-05-09 16:43:49.211247 edgeimpulse_api-1.23.0/edgeimpulse_api/models/project_public_data_readme.py
--rw-r--r--   0        0        0     2404 2023-05-09 16:43:49.866070 edgeimpulse_api-1.23.0/edgeimpulse_api/models/project_sample_metadata.py
--rw-r--r--   0        0        0     2670 2023-05-09 16:43:48.512971 edgeimpulse_api-1.23.0/edgeimpulse_api/models/project_training_data_summary_response.py
--rw-r--r--   0        0        0     2353 2023-05-09 16:43:49.851192 edgeimpulse_api-1.23.0/edgeimpulse_api/models/project_training_data_summary_response_all_of.py
--rw-r--r--   0        0        0     2316 2023-05-09 16:43:48.853988 edgeimpulse_api-1.23.0/edgeimpulse_api/models/project_version_request.py
--rw-r--r--   0        0        0     2664 2023-05-09 16:43:48.389616 edgeimpulse_api-1.23.0/edgeimpulse_api/models/raw_sample_data.py
--rw-r--r--   0        0        0     3440 2023-05-09 16:43:49.980059 edgeimpulse_api-1.23.0/edgeimpulse_api/models/raw_sample_payload.py
--rw-r--r--   0        0        0     2537 2023-05-09 16:43:50.132826 edgeimpulse_api-1.23.0/edgeimpulse_api/models/rebalance_dataset_response.py
--rw-r--r--   0        0        0     1984 2023-05-09 16:43:49.077427 edgeimpulse_api-1.23.0/edgeimpulse_api/models/remove_collaborator_request.py
--rw-r--r--   0        0        0     1805 2023-05-09 16:43:49.510581 edgeimpulse_api-1.23.0/edgeimpulse_api/models/remove_member_request.py
--rw-r--r--   0        0        0     1867 2023-05-09 16:43:48.964755 edgeimpulse_api-1.23.0/edgeimpulse_api/models/rename_device_request.py
--rw-r--r--   0        0        0     2081 2023-05-09 16:43:48.787878 edgeimpulse_api-1.23.0/edgeimpulse_api/models/rename_portal_file_request.py
--rw-r--r--   0        0        0     1867 2023-05-09 16:43:49.967141 edgeimpulse_api-1.23.0/edgeimpulse_api/models/rename_sample_request.py
--rw-r--r--   0        0        0     1873 2023-05-09 16:43:48.290060 edgeimpulse_api-1.23.0/edgeimpulse_api/models/request_reset_password_request.py
--rw-r--r--   0        0        0     2031 2023-05-09 16:43:49.993681 edgeimpulse_api-1.23.0/edgeimpulse_api/models/reset_password_request.py
--rw-r--r--   0        0        0     1985 2023-05-09 16:43:49.199103 edgeimpulse_api-1.23.0/edgeimpulse_api/models/restore_project_from_public_request.py
--rw-r--r--   0        0        0     2265 2023-05-09 16:43:49.860900 edgeimpulse_api-1.23.0/edgeimpulse_api/models/restore_project_request.py
--rw-r--r--   0        0        0     2669 2023-05-09 16:43:49.936541 edgeimpulse_api-1.23.0/edgeimpulse_api/models/run_organization_pipeline_response.py
--rw-r--r--   0        0        0     2352 2023-05-09 16:43:48.241400 edgeimpulse_api-1.23.0/edgeimpulse_api/models/run_organization_pipeline_response_all_of.py
--rw-r--r--   0        0        0     9637 2023-05-09 16:43:49.585581 edgeimpulse_api-1.23.0/edgeimpulse_api/models/sample.py
--rw-r--r--   0        0        0     2443 2023-05-09 16:43:48.419767 edgeimpulse_api-1.23.0/edgeimpulse_api/models/sample_bounding_boxes_request.py
--rw-r--r--   0        0        0     2000 2023-05-09 16:43:48.331280 edgeimpulse_api-1.23.0/edgeimpulse_api/models/sample_metadata.py
--rw-r--r--   0        0        0     2756 2023-05-09 16:43:48.364292 edgeimpulse_api-1.23.0/edgeimpulse_api/models/save_pretrained_model_request.py
--rw-r--r--   0        0        0     3327 2023-05-09 16:43:49.014830 edgeimpulse_api-1.23.0/edgeimpulse_api/models/score_trial_response.py
--rw-r--r--   0        0        0     3003 2023-05-09 16:43:50.176725 edgeimpulse_api-1.23.0/edgeimpulse_api/models/score_trial_response_all_of.py
--rw-r--r--   0        0        0     2240 2023-05-09 16:43:48.939221 edgeimpulse_api-1.23.0/edgeimpulse_api/models/score_trial_response_all_of_latency.py
--rw-r--r--   0        0        0     1914 2023-05-09 16:43:49.831857 edgeimpulse_api-1.23.0/edgeimpulse_api/models/score_trial_response_all_of_ram.py
--rw-r--r--   0        0        0     2405 2023-05-09 16:43:48.561005 edgeimpulse_api-1.23.0/edgeimpulse_api/models/segment_sample_request.py
--rw-r--r--   0        0        0     2055 2023-05-09 16:43:50.040650 edgeimpulse_api-1.23.0/edgeimpulse_api/models/segment_sample_request_segments_inner.py
--rw-r--r--   0        0        0     3364 2023-05-09 16:43:49.427795 edgeimpulse_api-1.23.0/edgeimpulse_api/models/send_user_feedback_request.py
--rw-r--r--   0        0        0     1981 2023-05-09 16:43:48.352313 edgeimpulse_api-1.23.0/edgeimpulse_api/models/sensor.py
--rw-r--r--   0        0        0     2142 2023-05-09 16:43:49.784037 edgeimpulse_api-1.23.0/edgeimpulse_api/models/set_anomaly_parameter_request.py
--rw-r--r--   0        0        0     7742 2023-05-09 16:43:48.426429 edgeimpulse_api-1.23.0/edgeimpulse_api/models/set_keras_parameter_request.py
--rw-r--r--   0        0        0     1893 2023-05-09 16:43:49.970776 edgeimpulse_api-1.23.0/edgeimpulse_api/models/set_member_datasets_request.py
--rw-r--r--   0        0        0     2049 2023-05-09 16:43:49.676340 edgeimpulse_api-1.23.0/edgeimpulse_api/models/set_member_role_request.py
--rw-r--r--   0        0        0     2219 2023-05-09 16:43:49.771065 edgeimpulse_api-1.23.0/edgeimpulse_api/models/set_optimize_space_request.py
--rw-r--r--   0        0        0     2254 2023-05-09 16:43:49.795002 edgeimpulse_api-1.23.0/edgeimpulse_api/models/set_optimize_space_request_all_of.py
--rw-r--r--   0        0        0     1923 2023-05-09 16:43:50.160864 edgeimpulse_api-1.23.0/edgeimpulse_api/models/set_organization_data_dataset_request.py
--rw-r--r--   0        0        0     1974 2023-05-09 16:43:48.813881 edgeimpulse_api-1.23.0/edgeimpulse_api/models/set_project_compute_time_request.py
--rw-r--r--   0        0        0     2011 2023-05-09 16:43:49.244320 edgeimpulse_api-1.23.0/edgeimpulse_api/models/set_project_dsp_file_size_request.py
--rw-r--r--   0        0        0     1919 2023-05-09 16:43:48.452125 edgeimpulse_api-1.23.0/edgeimpulse_api/models/set_sample_metadata_request.py
--rw-r--r--   0        0        0     1915 2023-05-09 16:43:49.156502 edgeimpulse_api-1.23.0/edgeimpulse_api/models/set_syntiant_posterior_request.py
--rw-r--r--   0        0        0     2140 2023-05-09 16:43:48.935334 edgeimpulse_api-1.23.0/edgeimpulse_api/models/set_user_password_request.py
--rw-r--r--   0        0        0     2536 2023-05-09 16:43:48.479578 edgeimpulse_api-1.23.0/edgeimpulse_api/models/socket_token_response.py
--rw-r--r--   0        0        0     2239 2023-05-09 16:43:49.671542 edgeimpulse_api-1.23.0/edgeimpulse_api/models/socket_token_response_all_of.py
--rw-r--r--   0        0        0     2059 2023-05-09 16:43:48.154903 edgeimpulse_api-1.23.0/edgeimpulse_api/models/socket_token_response_all_of_token.py
--rw-r--r--   0        0        0     1971 2023-05-09 16:43:48.534478 edgeimpulse_api-1.23.0/edgeimpulse_api/models/split_sample_in_frames_request.py
--rw-r--r--   0        0        0     2110 2023-05-09 16:43:48.416147 edgeimpulse_api-1.23.0/edgeimpulse_api/models/staff_info.py
--rw-r--r--   0        0        0     2226 2023-05-09 16:43:49.384625 edgeimpulse_api-1.23.0/edgeimpulse_api/models/start_job_response.py
--rw-r--r--   0        0        0     1909 2023-05-09 16:43:48.184547 edgeimpulse_api-1.23.0/edgeimpulse_api/models/start_job_response_all_of.py
--rw-r--r--   0        0        0     2883 2023-05-09 16:43:49.043931 edgeimpulse_api-1.23.0/edgeimpulse_api/models/start_performance_calibration_request.py
--rw-r--r--   0        0        0     2838 2023-05-09 16:43:49.620351 edgeimpulse_api-1.23.0/edgeimpulse_api/models/start_sampling_request.py
--rw-r--r--   0        0        0     2189 2023-05-09 16:43:49.562078 edgeimpulse_api-1.23.0/edgeimpulse_api/models/start_sampling_response.py
--rw-r--r--   0        0        0     1892 2023-05-09 16:43:49.215786 edgeimpulse_api-1.23.0/edgeimpulse_api/models/start_sampling_response_all_of.py
--rw-r--r--   0        0        0     2492 2023-05-09 16:43:49.207830 edgeimpulse_api-1.23.0/edgeimpulse_api/models/start_training_request_anomaly.py
--rw-r--r--   0        0        0     1967 2023-05-09 16:43:48.264391 edgeimpulse_api-1.23.0/edgeimpulse_api/models/store_segment_length_request.py
--rw-r--r--   0        0        0     2644 2023-05-09 16:43:49.777121 edgeimpulse_api-1.23.0/edgeimpulse_api/models/structured_classify_result.py
--rw-r--r--   0        0        0     2433 2023-05-09 16:43:48.149485 edgeimpulse_api-1.23.0/edgeimpulse_api/models/test_pretrained_model_request.py
--rw-r--r--   0        0        0     3074 2023-05-09 16:43:49.823203 edgeimpulse_api-1.23.0/edgeimpulse_api/models/test_pretrained_model_response.py
--rw-r--r--   0        0        0     2784 2023-05-09 16:43:49.499604 edgeimpulse_api-1.23.0/edgeimpulse_api/models/test_pretrained_model_response_all_of.py
--rw-r--r--   0        0        0     3251 2023-05-09 16:43:48.467085 edgeimpulse_api-1.23.0/edgeimpulse_api/models/theme.py
--rw-r--r--   0        0        0     2239 2023-05-09 16:43:49.099486 edgeimpulse_api-1.23.0/edgeimpulse_api/models/theme_colors.py
--rw-r--r--   0        0        0     2764 2023-05-09 16:43:48.825708 edgeimpulse_api-1.23.0/edgeimpulse_api/models/theme_favicon.py
--rw-r--r--   0        0        0     2586 2023-05-09 16:56:04.586516 edgeimpulse_api-1.23.0/edgeimpulse_api/models/theme_logos.py
--rw-r--r--   0        0        0     2245 2023-05-09 16:43:48.758617 edgeimpulse_api-1.23.0/edgeimpulse_api/models/third_party_auth.py
--rw-r--r--   0        0        0     2031 2023-05-09 16:43:48.769302 edgeimpulse_api-1.23.0/edgeimpulse_api/models/track_objects_request.py
--rw-r--r--   0        0        0     2736 2023-05-09 16:43:49.399328 edgeimpulse_api-1.23.0/edgeimpulse_api/models/track_objects_response.py
--rw-r--r--   0        0        0     2436 2023-05-09 16:43:48.673644 edgeimpulse_api-1.23.0/edgeimpulse_api/models/track_objects_response_all_of.py
--rw-r--r--   0        0        0     4610 2023-05-09 16:43:48.618580 edgeimpulse_api-1.23.0/edgeimpulse_api/models/transfer_learning_model.py
--rw-r--r--   0        0        0     2012 2023-05-09 16:43:48.391825 edgeimpulse_api-1.23.0/edgeimpulse_api/models/transfer_ownership_organization_request.py
--rw-r--r--   0        0        0     2585 2023-05-09 16:43:49.722143 edgeimpulse_api-1.23.0/edgeimpulse_api/models/transformation_block_additional_mount_point.py
--rw-r--r--   0        0        0      588 2023-05-09 16:43:49.731737 edgeimpulse_api-1.23.0/edgeimpulse_api/models/transformation_job_status_enum.py
--rw-r--r--   0        0        0     2578 2023-05-09 16:43:49.460913 edgeimpulse_api-1.23.0/edgeimpulse_api/models/tuner_create_trial_impulse.py
--rw-r--r--   0        0        0     2570 2023-05-09 16:43:48.187129 edgeimpulse_api-1.23.0/edgeimpulse_api/models/tuner_space_impulse.py
--rw-r--r--   0        0        0     3661 2023-05-09 16:43:49.871398 edgeimpulse_api-1.23.0/edgeimpulse_api/models/tuner_trial.py
--rw-r--r--   0        0        0     2304 2023-05-09 16:43:48.829489 edgeimpulse_api-1.23.0/edgeimpulse_api/models/tuner_trial_blocks_inner.py
--rw-r--r--   0        0        0     2028 2023-05-09 16:43:48.629429 edgeimpulse_api-1.23.0/edgeimpulse_api/models/update_job_request.py
--rw-r--r--   0        0        0     2281 2023-05-09 16:43:48.690928 edgeimpulse_api-1.23.0/edgeimpulse_api/models/update_organization_add_collaborator_request.py
--rw-r--r--   0        0        0     2817 2023-05-09 16:43:49.463271 edgeimpulse_api-1.23.0/edgeimpulse_api/models/update_organization_bucket_request.py
--rw-r--r--   0        0        0     2578 2023-05-09 16:43:49.847037 edgeimpulse_api-1.23.0/edgeimpulse_api/models/update_organization_create_empty_project_request.py
--rw-r--r--   0        0        0     2428 2023-05-09 16:43:48.147840 edgeimpulse_api-1.23.0/edgeimpulse_api/models/update_organization_create_project_request.py
--rw-r--r--   0        0        0     2158 2023-05-09 16:43:49.800442 edgeimpulse_api-1.23.0/edgeimpulse_api/models/update_organization_data_item_request.py
--rw-r--r--   0        0        0     2052 2023-05-09 16:43:49.963313 edgeimpulse_api-1.23.0/edgeimpulse_api/models/update_organization_dataset_request.py
--rw-r--r--   0        0        0     2881 2023-05-09 16:43:50.023424 edgeimpulse_api-1.23.0/edgeimpulse_api/models/update_organization_dsp_block_request.py
--rw-r--r--   0        0        0     2724 2023-05-09 16:43:48.778516 edgeimpulse_api-1.23.0/edgeimpulse_api/models/update_organization_portal_response.py
--rw-r--r--   0        0        0     2445 2023-05-09 16:43:49.497518 edgeimpulse_api-1.23.0/edgeimpulse_api/models/update_organization_portal_response_all_of.py
--rw-r--r--   0        0        0     2582 2023-05-09 16:43:49.618134 edgeimpulse_api-1.23.0/edgeimpulse_api/models/update_organization_request.py
--rw-r--r--   0        0        0     3910 2023-05-09 16:43:49.745910 edgeimpulse_api-1.23.0/edgeimpulse_api/models/update_organization_transfer_learning_block_request.py
--rw-r--r--   0        0        0     4734 2023-05-09 16:43:49.801495 edgeimpulse_api-1.23.0/edgeimpulse_api/models/update_organization_transformation_block_request.py
--rw-r--r--   0        0        0     7726 2023-05-09 16:43:49.382472 edgeimpulse_api-1.23.0/edgeimpulse_api/models/update_project_request.py
--rw-r--r--   0        0        0     1877 2023-05-09 16:43:48.918270 edgeimpulse_api-1.23.0/edgeimpulse_api/models/update_project_tags_request.py
--rw-r--r--   0        0        0     2259 2023-05-09 16:43:48.499955 edgeimpulse_api-1.23.0/edgeimpulse_api/models/update_theme_colors_request.py
--rw-r--r--   0        0        0     2729 2023-05-09 16:56:04.586686 edgeimpulse_api-1.23.0/edgeimpulse_api/models/update_theme_logos_request.py
--rw-r--r--   0        0        0     2205 2023-05-09 16:43:49.564036 edgeimpulse_api-1.23.0/edgeimpulse_api/models/update_third_party_auth_request.py
--rw-r--r--   0        0        0     2277 2023-05-09 16:43:48.432099 edgeimpulse_api-1.23.0/edgeimpulse_api/models/update_user_request.py
--rw-r--r--   0        0        0     1886 2023-05-09 16:43:48.997702 edgeimpulse_api-1.23.0/edgeimpulse_api/models/update_version_request.py
--rw-r--r--   0        0        0     2125 2023-05-09 16:43:49.928801 edgeimpulse_api-1.23.0/edgeimpulse_api/models/update_whitelabel_deployment_targets_request.py
--rw-r--r--   0        0        0     2168 2023-05-09 16:43:49.342903 edgeimpulse_api-1.23.0/edgeimpulse_api/models/upload_asset_response.py
--rw-r--r--   0        0        0     1882 2023-05-09 16:43:48.748681 edgeimpulse_api-1.23.0/edgeimpulse_api/models/upload_asset_response_all_of.py
--rw-r--r--   0        0        0     2199 2023-05-09 16:43:48.175550 edgeimpulse_api-1.23.0/edgeimpulse_api/models/upload_readme_image_response.py
--rw-r--r--   0        0        0     2185 2023-05-09 16:43:49.433226 edgeimpulse_api-1.23.0/edgeimpulse_api/models/upload_user_photo_response.py
--rw-r--r--   0        0        0     1872 2023-05-09 16:43:49.470472 edgeimpulse_api-1.23.0/edgeimpulse_api/models/upload_user_photo_response_all_of.py
--rw-r--r--   0        0        0     3291 2023-05-09 16:43:48.266461 edgeimpulse_api-1.23.0/edgeimpulse_api/models/user.py
--rw-r--r--   0        0        0     1991 2023-05-09 16:43:48.652103 edgeimpulse_api-1.23.0/edgeimpulse_api/models/user_by_third_party_activation_request.py
--rw-r--r--   0        0        0     2192 2023-05-09 16:43:49.934440 edgeimpulse_api-1.23.0/edgeimpulse_api/models/user_experiment.py
--rw-r--r--   0        0        0     2709 2023-05-09 16:43:48.993815 edgeimpulse_api-1.23.0/edgeimpulse_api/models/user_organization.py
--rw-r--r--   0        0        0     1844 2023-05-09 16:43:49.487341 edgeimpulse_api-1.23.0/edgeimpulse_api/models/verify_dsp_block_url_request.py
--rw-r--r--   0        0        0     2604 2023-05-09 16:43:49.808910 edgeimpulse_api-1.23.0/edgeimpulse_api/models/verify_dsp_block_url_response.py
--rw-r--r--   0        0        0     2307 2023-05-09 16:43:49.605306 edgeimpulse_api-1.23.0/edgeimpulse_api/models/verify_dsp_block_url_response_all_of.py
--rw-r--r--   0        0        0     2407 2023-05-09 16:43:49.763893 edgeimpulse_api-1.23.0/edgeimpulse_api/models/verify_dsp_block_url_response_all_of_block.py
--rw-r--r--   0        0        0     2708 2023-05-09 16:43:48.842367 edgeimpulse_api-1.23.0/edgeimpulse_api/models/verify_organization_bucket_request.py
--rw-r--r--   0        0        0     2897 2023-05-09 16:43:49.573692 edgeimpulse_api-1.23.0/edgeimpulse_api/models/verify_organization_bucket_response.py
--rw-r--r--   0        0        0     2597 2023-05-09 16:43:49.935426 edgeimpulse_api-1.23.0/edgeimpulse_api/models/verify_organization_bucket_response_all_of.py
--rw-r--r--   0        0        0     2187 2023-05-09 16:43:48.122648 edgeimpulse_api-1.23.0/edgeimpulse_api/models/verify_organization_bucket_response_all_of_files.py
--rw-r--r--   0        0        0     1937 2023-05-09 16:43:49.698568 edgeimpulse_api-1.23.0/edgeimpulse_api/models/verify_reset_password_request.py
--rw-r--r--   0        0        0     3883 2023-05-09 16:43:49.438948 edgeimpulse_api-1.23.0/edgeimpulse_api/models/whitelabel.py
--rw-r--r--   0        0        0     2534 2023-05-09 16:43:48.144096 edgeimpulse_api-1.23.0/edgeimpulse_api/models/whitelabel_admin_create_organization_request.py
--rw-r--r--   0        0        0     2885 2023-05-09 16:43:49.906581 edgeimpulse_api-1.23.0/edgeimpulse_api/models/window_settings_response.py
--rw-r--r--   0        0        0     2585 2023-05-09 16:43:48.161621 edgeimpulse_api-1.23.0/edgeimpulse_api/models/window_settings_response_all_of.py
--rw-r--r--   0        0        0     2848 2023-05-09 16:43:48.231387 edgeimpulse_api-1.23.0/edgeimpulse_api/models/window_settings_response_all_of_window_settings.py
--rw-r--r--   0        0        0    12674 2023-05-09 16:43:36.498560 edgeimpulse_api-1.23.0/edgeimpulse_api/rest.py
--rw-r--r--   0        0        0      975 2023-05-09 16:56:21.131376 edgeimpulse_api-1.23.0/pyproject.toml
--rw-r--r--   0        0        0     1413 1970-01-01 00:00:00.000000 edgeimpulse_api-1.23.0/PKG-INFO
+-rw-r--r--   0        0        0      377 2023-05-16 14:36:24.095652 edgeimpulse_api-1.23.6/README.md
+-rw-r--r--   0        0        0    66201 2023-05-18 15:26:28.795695 edgeimpulse_api-1.23.6/edgeimpulse_api/__init__.py
+-rw-r--r--   0        0        0     2752 2023-05-18 14:36:17.751151 edgeimpulse_api-1.23.6/edgeimpulse_api/api/__init__.py
+-rw-r--r--   0        0        0   168622 2023-05-18 14:36:17.293165 edgeimpulse_api-1.23.6/edgeimpulse_api/api/admin_api.py
+-rw-r--r--   0        0        0   290132 2023-05-18 14:36:17.313616 edgeimpulse_api-1.23.6/edgeimpulse_api/api/allows_read_only_api.py
+-rw-r--r--   0        0        0    11231 2023-05-18 14:36:17.328822 edgeimpulse_api-1.23.6/edgeimpulse_api/api/auth_api.py
+-rw-r--r--   0        0        0     6235 2023-05-18 14:36:17.336574 edgeimpulse_api-1.23.6/edgeimpulse_api/api/cdn_api.py
+-rw-r--r--   0        0        0    27785 2023-05-18 14:36:17.343591 edgeimpulse_api-1.23.6/edgeimpulse_api/api/classify_api.py
+-rw-r--r--   0        0        0     7426 2023-05-18 14:36:17.349695 edgeimpulse_api-1.23.6/edgeimpulse_api/api/content_disposition_inline_api.py
+-rw-r--r--   0        0        0    72480 2023-05-18 14:36:17.372542 edgeimpulse_api-1.23.6/edgeimpulse_api/api/deployment_api.py
+-rw-r--r--   0        0        0    38974 2023-05-18 14:36:17.384168 edgeimpulse_api-1.23.6/edgeimpulse_api/api/devices_api.py
+-rw-r--r--   0        0        0   130256 2023-05-18 14:36:17.359797 edgeimpulse_api-1.23.6/edgeimpulse_api/api/dsp_api.py
+-rw-r--r--   0        0        0     6435 2023-05-18 14:36:17.392104 edgeimpulse_api-1.23.6/edgeimpulse_api/api/export_api.py
+-rw-r--r--   0        0        0    11921 2023-05-18 14:36:17.402726 edgeimpulse_api-1.23.6/edgeimpulse_api/api/health_api.py
+-rw-r--r--   0        0        0    49621 2023-05-18 14:36:17.410771 edgeimpulse_api-1.23.6/edgeimpulse_api/api/impulse_api.py
+-rw-r--r--   0        0        0   231500 2023-05-18 14:36:17.423689 edgeimpulse_api-1.23.6/edgeimpulse_api/api/jobs_api.py
+-rw-r--r--   0        0        0   134972 2023-05-18 14:36:17.437334 edgeimpulse_api-1.23.6/edgeimpulse_api/api/learn_api.py
+-rw-r--r--   0        0        0     6483 2023-05-18 14:36:17.446396 edgeimpulse_api-1.23.6/edgeimpulse_api/api/login_api.py
+-rw-r--r--   0        0        0    12006 2023-05-18 14:36:17.452715 edgeimpulse_api-1.23.6/edgeimpulse_api/api/metrics_api.py
+-rw-r--r--   0        0        0    67457 2023-05-18 14:36:17.461353 edgeimpulse_api-1.23.6/edgeimpulse_api/api/optimization_api.py
+-rw-r--r--   0        0        0   300920 2023-05-18 14:36:17.473518 edgeimpulse_api-1.23.6/edgeimpulse_api/api/organization_allow_developer_profile_api.py
+-rw-r--r--   0        0        0    63140 2023-05-18 14:36:17.489010 edgeimpulse_api-1.23.6/edgeimpulse_api/api/organization_allow_guest_access_api.py
+-rw-r--r--   0        0        0   141131 2023-05-18 14:36:17.499676 edgeimpulse_api-1.23.6/edgeimpulse_api/api/organization_blocks_api.py
+-rw-r--r--   0        0        0    91908 2023-05-18 14:36:17.511138 edgeimpulse_api-1.23.6/edgeimpulse_api/api/organization_create_project_api.py
+-rw-r--r--   0        0        0   255365 2023-05-18 14:36:17.523986 edgeimpulse_api-1.23.6/edgeimpulse_api/api/organization_data_api.py
+-rw-r--r--   0        0        0    58218 2023-05-18 14:36:17.545880 edgeimpulse_api-1.23.6/edgeimpulse_api/api/organization_jobs_api.py
+-rw-r--r--   0        0        0    47178 2023-05-18 14:36:17.553852 edgeimpulse_api-1.23.6/edgeimpulse_api/api/organization_pipelines_api.py
+-rw-r--r--   0        0        0    45490 2023-05-18 14:36:17.562088 edgeimpulse_api-1.23.6/edgeimpulse_api/api/organization_portals_api.py
+-rw-r--r--   0        0        0   230641 2023-05-18 14:36:17.573187 edgeimpulse_api-1.23.6/edgeimpulse_api/api/organization_requires_admin_api.py
+-rw-r--r--   0        0        0   140588 2023-05-18 14:36:17.587790 edgeimpulse_api-1.23.6/edgeimpulse_api/api/organization_requires_whitelabel_admin_api.py
+-rw-r--r--   0        0        0   264527 2023-05-18 14:36:17.602239 edgeimpulse_api-1.23.6/edgeimpulse_api/api/organizations_api.py
+-rw-r--r--   0        0        0    54671 2023-05-18 14:36:17.615791 edgeimpulse_api-1.23.6/edgeimpulse_api/api/performance_calibration_api.py
+-rw-r--r--   0        0        0   228112 2023-05-18 14:36:17.627308 edgeimpulse_api-1.23.6/edgeimpulse_api/api/projects_api.py
+-rw-r--r--   0        0        0   328783 2023-05-18 14:36:17.647205 edgeimpulse_api-1.23.6/edgeimpulse_api/api/raw_data_api.py
+-rw-r--r--   0        0        0    24481 2023-05-18 14:36:17.661499 edgeimpulse_api-1.23.6/edgeimpulse_api/api/requires_sudo_api.py
+-rw-r--r--   0        0        0     7730 2023-05-18 14:36:17.668662 edgeimpulse_api-1.23.6/edgeimpulse_api/api/requires_third_party_auth_api_key_api.py
+-rw-r--r--   0        0        0    13690 2023-05-18 14:36:17.676603 edgeimpulse_api-1.23.6/edgeimpulse_api/api/supports_range_api.py
+-rw-r--r--   0        0        0    35671 2023-05-18 14:36:17.683946 edgeimpulse_api-1.23.6/edgeimpulse_api/api/themes_api.py
+-rw-r--r--   0        0        0    43486 2023-05-18 14:36:17.691236 edgeimpulse_api-1.23.6/edgeimpulse_api/api/third_party_auth_api.py
+-rw-r--r--   0        0        0    45393 2023-05-18 14:36:17.699973 edgeimpulse_api-1.23.6/edgeimpulse_api/api/upload_portal_api.py
+-rw-r--r--   0        0        0   197590 2023-05-18 14:36:17.711589 edgeimpulse_api-1.23.6/edgeimpulse_api/api/user_api.py
+-rw-r--r--   0        0        0    42135 2023-05-18 14:36:17.724452 edgeimpulse_api-1.23.6/edgeimpulse_api/api/whitelabels_api.py
+-rw-r--r--   0        0        0    29331 2023-05-18 14:36:17.758593 edgeimpulse_api-1.23.6/edgeimpulse_api/api_client.py
+-rw-r--r--   0        0        0    15659 2023-05-18 14:36:17.741568 edgeimpulse_api-1.23.6/edgeimpulse_api/configuration.py
+-rw-r--r--   0        0        0     5113 2023-05-18 14:36:17.753838 edgeimpulse_api-1.23.6/edgeimpulse_api/exceptions.py
+-rw-r--r--   0        0        0    62996 2023-05-18 14:36:24.927738 edgeimpulse_api-1.23.6/edgeimpulse_api/models/__init__.py
+-rw-r--r--   0        0        0     2897 2023-05-18 14:36:24.915492 edgeimpulse_api-1.23.6/edgeimpulse_api/models/activate_user_by_third_party_activation_code_request.py
+-rw-r--r--   0        0        0     1882 2023-05-18 14:36:24.918688 edgeimpulse_api-1.23.6/edgeimpulse_api/models/activate_user_request.py
+-rw-r--r--   0        0        0     2610 2023-05-18 14:36:24.521461 edgeimpulse_api-1.23.6/edgeimpulse_api/models/add_api_key_request.py
+-rw-r--r--   0        0        0     1963 2023-05-18 14:36:24.630204 edgeimpulse_api-1.23.6/edgeimpulse_api/models/add_collaborator_request.py
+-rw-r--r--   0        0        0     2223 2023-05-18 14:36:25.222624 edgeimpulse_api-1.23.6/edgeimpulse_api/models/add_hmac_key_request.py
+-rw-r--r--   0        0        0     2432 2023-05-18 14:36:25.188927 edgeimpulse_api-1.23.6/edgeimpulse_api/models/add_member_request.py
+-rw-r--r--   0        0        0     2418 2023-05-18 14:36:24.758600 edgeimpulse_api-1.23.6/edgeimpulse_api/models/add_organization_api_key_request.py
+-rw-r--r--   0        0        0     2806 2023-05-18 14:36:24.932455 edgeimpulse_api-1.23.6/edgeimpulse_api/models/add_organization_bucket_request.py
+-rw-r--r--   0        0        0     2269 2023-05-18 14:36:25.043877 edgeimpulse_api-1.23.6/edgeimpulse_api/models/add_organization_deploy_block_response.py
+-rw-r--r--   0        0        0     2816 2023-05-18 14:36:24.894516 edgeimpulse_api-1.23.6/edgeimpulse_api/models/add_organization_dsp_block_request.py
+-rw-r--r--   0        0        0     2248 2023-05-18 14:36:25.092932 edgeimpulse_api-1.23.6/edgeimpulse_api/models/add_organization_dsp_block_response.py
+-rw-r--r--   0        0        0     2054 2023-05-18 14:36:24.909020 edgeimpulse_api-1.23.6/edgeimpulse_api/models/add_organization_secret_request.py
+-rw-r--r--   0        0        0     2266 2023-05-18 14:36:25.103899 edgeimpulse_api-1.23.6/edgeimpulse_api/models/add_organization_secret_response.py
+-rw-r--r--   0        0        0     1949 2023-05-18 14:36:24.842955 edgeimpulse_api-1.23.6/edgeimpulse_api/models/add_organization_secret_response_all_of.py
+-rw-r--r--   0        0        0     3834 2023-05-18 14:36:24.673395 edgeimpulse_api-1.23.6/edgeimpulse_api/models/add_organization_transfer_learning_block_request.py
+-rw-r--r--   0        0        0     2339 2023-05-18 14:36:25.077522 edgeimpulse_api-1.23.6/edgeimpulse_api/models/add_organization_transfer_learning_block_response.py
+-rw-r--r--   0        0        0     4592 2023-05-18 14:36:24.542098 edgeimpulse_api-1.23.6/edgeimpulse_api/models/add_organization_transformation_block_request.py
+-rw-r--r--   0        0        0     2325 2023-05-18 14:36:25.356972 edgeimpulse_api-1.23.6/edgeimpulse_api/models/add_organization_transformation_block_response.py
+-rw-r--r--   0        0        0     2001 2023-05-18 14:36:24.712206 edgeimpulse_api-1.23.6/edgeimpulse_api/models/add_organization_transformation_block_response_all_of.py
+-rw-r--r--   0        0        0     1961 2023-05-18 14:36:25.218381 edgeimpulse_api-1.23.6/edgeimpulse_api/models/admin_add_or_update_sso_domain_id_ps_request.py
+-rw-r--r--   0        0        0     2130 2023-05-18 14:36:25.307049 edgeimpulse_api-1.23.6/edgeimpulse_api/models/admin_add_project_user_request.py
+-rw-r--r--   0        0        0     3876 2023-05-18 14:36:25.426726 edgeimpulse_api-1.23.6/edgeimpulse_api/models/admin_api_organization.py
+-rw-r--r--   0        0        0     2396 2023-05-18 14:36:24.650804 edgeimpulse_api-1.23.6/edgeimpulse_api/models/admin_api_organization_all_of.py
+-rw-r--r--   0        0        0     3459 2023-05-18 14:36:25.035851 edgeimpulse_api-1.23.6/edgeimpulse_api/models/admin_api_project.py
+-rw-r--r--   0        0        0     6367 2023-05-18 14:36:24.710737 edgeimpulse_api-1.23.6/edgeimpulse_api/models/admin_api_user.py
+-rw-r--r--   0        0        0     4953 2023-05-18 14:36:25.298475 edgeimpulse_api-1.23.6/edgeimpulse_api/models/admin_api_user_all_of.py
+-rw-r--r--   0        0        0     2262 2023-05-18 14:36:25.094520 edgeimpulse_api-1.23.6/edgeimpulse_api/models/admin_create_organization_request.py
+-rw-r--r--   0        0        0     2217 2023-05-18 14:36:25.206470 edgeimpulse_api-1.23.6/edgeimpulse_api/models/admin_get_metrics_response.py
+-rw-r--r--   0        0        0     1910 2023-05-18 14:36:25.059106 edgeimpulse_api-1.23.6/edgeimpulse_api/models/admin_get_metrics_response_all_of.py
+-rw-r--r--   0        0        0     3046 2023-05-18 14:36:25.006644 edgeimpulse_api-1.23.6/edgeimpulse_api/models/admin_get_organizations_response.py
+-rw-r--r--   0        0        0     2746 2023-05-18 14:36:25.463384 edgeimpulse_api-1.23.6/edgeimpulse_api/models/admin_get_organizations_response_all_of.py
+-rw-r--r--   0        0        0     2868 2023-05-18 14:36:25.015921 edgeimpulse_api-1.23.6/edgeimpulse_api/models/admin_get_organizations_response_all_of_organizations.py
+-rw-r--r--   0        0        0     2243 2023-05-18 14:36:24.912537 edgeimpulse_api-1.23.6/edgeimpulse_api/models/admin_get_sso_domain_id_ps_response.py
+-rw-r--r--   0        0        0     1947 2023-05-18 14:36:25.003376 edgeimpulse_api-1.23.6/edgeimpulse_api/models/admin_get_sso_domain_id_ps_response_all_of.py
+-rw-r--r--   0        0        0     2914 2023-05-18 14:36:25.244234 edgeimpulse_api-1.23.6/edgeimpulse_api/models/admin_get_sso_settings_response.py
+-rw-r--r--   0        0        0     2614 2023-05-18 14:36:25.127737 edgeimpulse_api-1.23.6/edgeimpulse_api/models/admin_get_sso_settings_response_all_of.py
+-rw-r--r--   0        0        0     2096 2023-05-18 14:36:24.830699 edgeimpulse_api-1.23.6/edgeimpulse_api/models/admin_get_sso_settings_response_all_of_sso_whitelist.py
+-rw-r--r--   0        0        0     2208 2023-05-18 14:36:25.282248 edgeimpulse_api-1.23.6/edgeimpulse_api/models/admin_get_user_ids_response.py
+-rw-r--r--   0        0        0     1901 2023-05-18 14:36:25.228582 edgeimpulse_api-1.23.6/edgeimpulse_api/models/admin_get_user_ids_response_all_of.py
+-rw-r--r--   0        0        0     2245 2023-05-18 14:36:25.398492 edgeimpulse_api-1.23.6/edgeimpulse_api/models/admin_get_user_metrics_response.py
+-rw-r--r--   0        0        0     1938 2023-05-18 14:36:24.691929 edgeimpulse_api-1.23.6/edgeimpulse_api/models/admin_get_user_metrics_response_all_of.py
+-rw-r--r--   0        0        0     2452 2023-05-18 14:36:24.536901 edgeimpulse_api-1.23.6/edgeimpulse_api/models/admin_get_user_response.py
+-rw-r--r--   0        0        0     2128 2023-05-18 14:36:25.011403 edgeimpulse_api-1.23.6/edgeimpulse_api/models/admin_get_user_response_all_of.py
+-rw-r--r--   0        0        0     2807 2023-05-18 14:36:24.781669 edgeimpulse_api-1.23.6/edgeimpulse_api/models/admin_get_users_response.py
+-rw-r--r--   0        0        0     2500 2023-05-18 14:36:25.395629 edgeimpulse_api-1.23.6/edgeimpulse_api/models/admin_get_users_response_all_of.py
+-rw-r--r--   0        0        0     3087 2023-05-18 14:36:25.019526 edgeimpulse_api-1.23.6/edgeimpulse_api/models/admin_get_users_response_all_of_users.py
+-rw-r--r--   0        0        0     2445 2023-05-18 14:36:25.054320 edgeimpulse_api-1.23.6/edgeimpulse_api/models/admin_list_projects.py
+-rw-r--r--   0        0        0     2836 2023-05-18 14:36:25.046398 edgeimpulse_api-1.23.6/edgeimpulse_api/models/admin_list_projects_response.py
+-rw-r--r--   0        0        0     6072 2023-05-18 14:36:24.835920 edgeimpulse_api-1.23.6/edgeimpulse_api/models/admin_organization_info_response.py
+-rw-r--r--   0        0        0     1974 2023-05-18 14:36:25.124111 edgeimpulse_api-1.23.6/edgeimpulse_api/models/admin_organization_info_response_all_of.py
+-rw-r--r--   0        0        0     2728 2023-05-18 14:36:25.498061 edgeimpulse_api-1.23.6/edgeimpulse_api/models/admin_update_organization_request.py
+-rw-r--r--   0        0        0     2015 2023-05-18 14:36:25.242665 edgeimpulse_api-1.23.6/edgeimpulse_api/models/admin_update_user_permissions_request.py
+-rw-r--r--   0        0        0     2339 2023-05-18 14:36:25.502857 edgeimpulse_api-1.23.6/edgeimpulse_api/models/admin_update_user_request.py
+-rw-r--r--   0        0        0     2525 2023-05-18 14:36:25.205525 edgeimpulse_api-1.23.6/edgeimpulse_api/models/akida_edge_learning_config.py
+-rw-r--r--   0        0        0     3630 2023-05-18 14:36:24.598984 edgeimpulse_api-1.23.6/edgeimpulse_api/models/anomaly_model_metadata.py
+-rw-r--r--   0        0        0     2151 2023-05-18 14:36:24.851792 edgeimpulse_api-1.23.6/edgeimpulse_api/models/anomaly_model_metadata_clusters_inner.py
+-rw-r--r--   0        0        0     4011 2023-05-18 14:36:25.383803 edgeimpulse_api-1.23.6/edgeimpulse_api/models/anomaly_model_metadata_response.py
+-rw-r--r--   0        0        0     4079 2023-05-18 14:36:24.653459 edgeimpulse_api-1.23.6/edgeimpulse_api/models/anomaly_response.py
+-rw-r--r--   0        0        0     3812 2023-05-18 14:36:25.119636 edgeimpulse_api-1.23.6/edgeimpulse_api/models/anomaly_response_all_of.py
+-rw-r--r--   0        0        0     2044 2023-05-18 14:36:24.763822 edgeimpulse_api-1.23.6/edgeimpulse_api/models/anomaly_response_all_of_axes.py
+-rw-r--r--   0        0        0     3029 2023-05-18 14:36:25.178324 edgeimpulse_api-1.23.6/edgeimpulse_api/models/anomaly_trained_features_response.py
+-rw-r--r--   0        0        0     2729 2023-05-18 14:36:25.229822 edgeimpulse_api-1.23.6/edgeimpulse_api/models/anomaly_trained_features_response_all_of.py
+-rw-r--r--   0        0        0     2375 2023-05-18 14:36:24.660736 edgeimpulse_api-1.23.6/edgeimpulse_api/models/anomaly_trained_features_response_all_of_data.py
+-rw-r--r--   0        0        0      506 2023-05-18 14:36:25.017014 edgeimpulse_api-1.23.6/edgeimpulse_api/models/augmentation_policy_image_enum.py
+-rw-r--r--   0        0        0     3635 2023-05-18 14:36:24.840205 edgeimpulse_api-1.23.6/edgeimpulse_api/models/augmentation_policy_spectrogram.py
+-rw-r--r--   0        0        0     1895 2023-05-18 14:36:24.593529 edgeimpulse_api-1.23.6/edgeimpulse_api/models/autotune_dsp_request.py
+-rw-r--r--   0        0        0     2044 2023-05-18 14:36:25.146771 edgeimpulse_api-1.23.6/edgeimpulse_api/models/bounding_box.py
+-rw-r--r--   0        0        0     2151 2023-05-18 14:36:24.613448 edgeimpulse_api-1.23.6/edgeimpulse_api/models/bounding_box_with_score.py
+-rw-r--r--   0        0        0     2197 2023-05-18 14:36:24.849004 edgeimpulse_api-1.23.6/edgeimpulse_api/models/build_on_device_model_request.py
+-rw-r--r--   0        0        0     2433 2023-05-18 14:36:24.624179 edgeimpulse_api-1.23.6/edgeimpulse_api/models/build_organization_on_device_model_request.py
+-rw-r--r--   0        0        0     2041 2023-05-18 14:36:24.773258 edgeimpulse_api-1.23.6/edgeimpulse_api/models/change_password_request.py
+-rw-r--r--   0        0        0     3701 2023-05-18 14:36:25.081640 edgeimpulse_api-1.23.6/edgeimpulse_api/models/classify_job_response.py
+-rw-r--r--   0        0        0     3394 2023-05-18 14:36:25.436661 edgeimpulse_api-1.23.6/edgeimpulse_api/models/classify_job_response_all_of.py
+-rw-r--r--   0        0        0     3769 2023-05-18 14:36:24.933965 edgeimpulse_api-1.23.6/edgeimpulse_api/models/classify_job_response_all_of_accuracy.py
+-rw-r--r--   0        0        0     2055 2023-05-18 14:36:25.349486 edgeimpulse_api-1.23.6/edgeimpulse_api/models/classify_job_response_all_of_accuracy_total_summary.py
+-rw-r--r--   0        0        0     3255 2023-05-18 14:36:24.520564 edgeimpulse_api-1.23.6/edgeimpulse_api/models/classify_job_response_page.py
+-rw-r--r--   0        0        0     2948 2023-05-18 14:36:24.562211 edgeimpulse_api-1.23.6/edgeimpulse_api/models/classify_job_response_page_all_of.py
+-rw-r--r--   0        0        0     3932 2023-05-18 14:36:24.614492 edgeimpulse_api-1.23.6/edgeimpulse_api/models/classify_sample_response.py
+-rw-r--r--   0        0        0     3644 2023-05-18 14:36:24.587004 edgeimpulse_api-1.23.6/edgeimpulse_api/models/classify_sample_response_all_of.py
+-rw-r--r--   0        0        0     4783 2023-05-18 14:36:24.802854 edgeimpulse_api-1.23.6/edgeimpulse_api/models/classify_sample_response_classification.py
+-rw-r--r--   0        0        0     2597 2023-05-18 14:36:24.606667 edgeimpulse_api-1.23.6/edgeimpulse_api/models/classify_sample_response_classification_details.py
+-rw-r--r--   0        0        0     3004 2023-05-18 14:36:25.070786 edgeimpulse_api-1.23.6/edgeimpulse_api/models/convert_user_request.py
+-rw-r--r--   0        0        0     2183 2023-05-18 14:36:25.184303 edgeimpulse_api-1.23.6/edgeimpulse_api/models/count_samples_response.py
+-rw-r--r--   0        0        0     1859 2023-05-18 14:36:24.550576 edgeimpulse_api-1.23.6/edgeimpulse_api/models/count_samples_response_all_of.py
+-rw-r--r--   0        0        0     2255 2023-05-18 14:36:25.116300 edgeimpulse_api-1.23.6/edgeimpulse_api/models/create_block_version_response.py
+-rw-r--r--   0        0        0     1938 2023-05-18 14:36:25.384870 edgeimpulse_api-1.23.6/edgeimpulse_api/models/create_block_version_response_all_of.py
+-rw-r--r--   0        0        0     2404 2023-05-18 14:36:24.816295 edgeimpulse_api-1.23.6/edgeimpulse_api/models/create_developer_profile_response.py
+-rw-r--r--   0        0        0     2125 2023-05-18 14:36:24.541069 edgeimpulse_api-1.23.6/edgeimpulse_api/models/create_developer_profile_response_all_of.py
+-rw-r--r--   0        0        0     2387 2023-05-18 14:36:25.089855 edgeimpulse_api-1.23.6/edgeimpulse_api/models/create_device_request.py
+-rw-r--r--   0        0        0     2491 2023-05-18 14:36:24.633214 edgeimpulse_api-1.23.6/edgeimpulse_api/models/create_evaluation_user_response.py
+-rw-r--r--   0        0        0     2185 2023-05-18 14:36:24.889326 edgeimpulse_api-1.23.6/edgeimpulse_api/models/create_evaluation_user_response_all_of.py
+-rw-r--r--   0        0        0     2600 2023-05-18 14:36:24.761217 edgeimpulse_api-1.23.6/edgeimpulse_api/models/create_organization_portal_request.py
+-rw-r--r--   0        0        0     2830 2023-05-18 14:36:25.277241 edgeimpulse_api-1.23.6/edgeimpulse_api/models/create_organization_portal_response.py
+-rw-r--r--   0        0        0     2551 2023-05-18 14:36:24.701706 edgeimpulse_api-1.23.6/edgeimpulse_api/models/create_organization_portal_response_all_of.py
+-rw-r--r--   0        0        0     1990 2023-05-18 14:36:25.322311 edgeimpulse_api-1.23.6/edgeimpulse_api/models/create_organization_request.py
+-rw-r--r--   0        0        0     2454 2023-05-18 14:36:25.296576 edgeimpulse_api-1.23.6/edgeimpulse_api/models/create_organization_response.py
+-rw-r--r--   0        0        0     2148 2023-05-18 14:36:25.254336 edgeimpulse_api-1.23.6/edgeimpulse_api/models/create_organization_response_all_of.py
+-rw-r--r--   0        0        0     2185 2023-05-18 14:36:24.837898 edgeimpulse_api-1.23.6/edgeimpulse_api/models/create_pipeline_response.py
+-rw-r--r--   0        0        0     2254 2023-05-18 14:36:24.516890 edgeimpulse_api-1.23.6/edgeimpulse_api/models/create_project_request.py
+-rw-r--r--   0        0        0     2378 2023-05-18 14:36:24.871025 edgeimpulse_api-1.23.6/edgeimpulse_api/models/create_project_response.py
+-rw-r--r--   0        0        0     2072 2023-05-18 14:36:25.338887 edgeimpulse_api-1.23.6/edgeimpulse_api/models/create_project_response_all_of.py
+-rw-r--r--   0        0        0     2276 2023-05-18 14:36:25.310187 edgeimpulse_api-1.23.6/edgeimpulse_api/models/create_signed_upload_link_request.py
+-rw-r--r--   0        0        0     2414 2023-05-18 14:36:25.267847 edgeimpulse_api-1.23.6/edgeimpulse_api/models/create_signed_upload_link_response.py
+-rw-r--r--   0        0        0     2135 2023-05-18 14:36:24.644173 edgeimpulse_api-1.23.6/edgeimpulse_api/models/create_signed_upload_link_response_all_of.py
+-rw-r--r--   0        0        0     2413 2023-05-18 14:36:25.408637 edgeimpulse_api-1.23.6/edgeimpulse_api/models/create_third_party_auth_request.py
+-rw-r--r--   0        0        0     2450 2023-05-18 14:36:24.654407 edgeimpulse_api-1.23.6/edgeimpulse_api/models/create_third_party_auth_response.py
+-rw-r--r--   0        0        0     2144 2023-05-18 14:36:24.558605 edgeimpulse_api-1.23.6/edgeimpulse_api/models/create_third_party_auth_response_all_of.py
+-rw-r--r--   0        0        0     3835 2023-05-18 14:36:24.844401 edgeimpulse_api-1.23.6/edgeimpulse_api/models/create_user_request.py
+-rw-r--r--   0        0        0     2393 2023-05-18 14:36:24.747022 edgeimpulse_api-1.23.6/edgeimpulse_api/models/create_user_response.py
+-rw-r--r--   0        0        0     2114 2023-05-18 14:36:24.777894 edgeimpulse_api-1.23.6/edgeimpulse_api/models/create_user_response_all_of.py
+-rw-r--r--   0        0        0     2919 2023-05-18 14:36:24.967975 edgeimpulse_api-1.23.6/edgeimpulse_api/models/create_user_third_party_request.py
+-rw-r--r--   0        0        0     2672 2023-05-18 14:36:25.362312 edgeimpulse_api-1.23.6/edgeimpulse_api/models/create_user_third_party_response.py
+-rw-r--r--   0        0        0     2393 2023-05-18 14:36:24.847709 edgeimpulse_api-1.23.6/edgeimpulse_api/models/create_user_third_party_response_all_of.py
+-rw-r--r--   0        0        0     4157 2023-05-18 14:36:24.540073 edgeimpulse_api-1.23.6/edgeimpulse_api/models/create_whitelabel_request.py
+-rw-r--r--   0        0        0     2438 2023-05-18 14:36:24.859343 edgeimpulse_api-1.23.6/edgeimpulse_api/models/create_whitelabel_response.py
+-rw-r--r--   0        0        0     2121 2023-05-18 14:36:24.611950 edgeimpulse_api-1.23.6/edgeimpulse_api/models/create_whitelabel_response_all_of.py
+-rw-r--r--   0        0        0     2051 2023-05-18 14:36:25.422217 edgeimpulse_api-1.23.6/edgeimpulse_api/models/crop_sample_request.py
+-rw-r--r--   0        0        0     2248 2023-05-18 14:36:25.091325 edgeimpulse_api-1.23.6/edgeimpulse_api/models/crop_sample_response.py
+-rw-r--r--   0        0        0     1943 2023-05-18 14:36:24.833278 edgeimpulse_api-1.23.6/edgeimpulse_api/models/crop_sample_response_all_of.py
+-rw-r--r--   0        0        0     3292 2023-05-18 14:36:25.134238 edgeimpulse_api-1.23.6/edgeimpulse_api/models/data_explorer_predictions_response.py
+-rw-r--r--   0        0        0     3003 2023-05-18 14:36:24.620127 edgeimpulse_api-1.23.6/edgeimpulse_api/models/data_explorer_predictions_response_all_of.py
+-rw-r--r--   0        0        0     2838 2023-05-18 14:36:25.345234 edgeimpulse_api-1.23.6/edgeimpulse_api/models/data_explorer_settings.py
+-rw-r--r--   0        0        0     2149 2023-05-18 14:36:25.482305 edgeimpulse_api-1.23.6/edgeimpulse_api/models/dataset_ratio_data.py
+-rw-r--r--   0        0        0     2111 2023-05-18 14:36:24.966620 edgeimpulse_api-1.23.6/edgeimpulse_api/models/dataset_ratio_data_ratio.py
+-rw-r--r--   0        0        0     1898 2023-05-18 14:36:24.576826 edgeimpulse_api-1.23.6/edgeimpulse_api/models/delete_portal_file_request.py
+-rw-r--r--   0        0        0     2230 2023-05-18 14:36:24.772228 edgeimpulse_api-1.23.6/edgeimpulse_api/models/dependency_data.py
+-rw-r--r--   0        0        0     2280 2023-05-18 14:36:24.974602 edgeimpulse_api-1.23.6/edgeimpulse_api/models/deploy_pretrained_model_input_audio.py
+-rw-r--r--   0        0        0     2155 2023-05-18 14:36:24.876272 edgeimpulse_api-1.23.6/edgeimpulse_api/models/deploy_pretrained_model_input_image.py
+-rw-r--r--   0        0        0     2155 2023-05-18 14:36:25.390387 edgeimpulse_api-1.23.6/edgeimpulse_api/models/deploy_pretrained_model_input_other.py
+-rw-r--r--   0        0        0     2484 2023-05-18 14:36:25.245969 edgeimpulse_api-1.23.6/edgeimpulse_api/models/deploy_pretrained_model_input_time_series.py
+-rw-r--r--   0        0        0     2344 2023-05-18 14:36:25.172992 edgeimpulse_api-1.23.6/edgeimpulse_api/models/deploy_pretrained_model_model_classification.py
+-rw-r--r--   0        0        0     2780 2023-05-18 14:36:25.138773 edgeimpulse_api-1.23.6/edgeimpulse_api/models/deploy_pretrained_model_model_object_detection.py
+-rw-r--r--   0        0        0     2200 2023-05-18 14:36:24.887290 edgeimpulse_api-1.23.6/edgeimpulse_api/models/deploy_pretrained_model_model_regression.py
+-rw-r--r--   0        0        0     4339 2023-05-18 14:36:25.311325 edgeimpulse_api-1.23.6/edgeimpulse_api/models/deploy_pretrained_model_request.py
+-rw-r--r--   0        0        0     2833 2023-05-18 14:36:24.822093 edgeimpulse_api-1.23.6/edgeimpulse_api/models/deploy_pretrained_model_request_model_info.py
+-rw-r--r--   0        0        0     8503 2023-05-18 14:36:25.494275 edgeimpulse_api-1.23.6/edgeimpulse_api/models/deploy_pretrained_model_request_model_info_input.py
+-rw-r--r--   0        0        0     8065 2023-05-18 14:36:25.373235 edgeimpulse_api-1.23.6/edgeimpulse_api/models/deploy_pretrained_model_request_model_info_model.py
+-rw-r--r--   0        0        0     5596 2023-05-18 14:36:24.899038 edgeimpulse_api-1.23.6/edgeimpulse_api/models/deployment_target.py
+-rw-r--r--   0        0        0     1926 2023-05-18 14:36:25.202758 edgeimpulse_api-1.23.6/edgeimpulse_api/models/deployment_target_badge.py
+-rw-r--r--   0        0        0      679 2023-05-18 14:36:24.600649 edgeimpulse_api-1.23.6/edgeimpulse_api/models/deployment_target_engine.py
+-rw-r--r--   0        0        0     2702 2023-05-18 14:36:25.163571 edgeimpulse_api-1.23.6/edgeimpulse_api/models/deployment_targets_response.py
+-rw-r--r--   0        0        0     2395 2023-05-18 14:36:24.811509 edgeimpulse_api-1.23.6/edgeimpulse_api/models/deployment_targets_response_all_of.py
+-rw-r--r--   0        0        0     1983 2023-05-18 14:36:24.970701 edgeimpulse_api-1.23.6/edgeimpulse_api/models/development_board.py
+-rw-r--r--   0        0        0     2831 2023-05-18 14:36:24.884517 edgeimpulse_api-1.23.6/edgeimpulse_api/models/development_boards_response.py
+-rw-r--r--   0        0        0     2531 2023-05-18 14:36:24.625261 edgeimpulse_api-1.23.6/edgeimpulse_api/models/development_boards_response_all_of.py
+-rw-r--r--   0        0        0     2030 2023-05-18 14:36:25.489803 edgeimpulse_api-1.23.6/edgeimpulse_api/models/development_keys.py
+-rw-r--r--   0        0        0     2400 2023-05-18 14:36:25.328120 edgeimpulse_api-1.23.6/edgeimpulse_api/models/development_keys_response.py
+-rw-r--r--   0        0        0     3677 2023-05-18 14:36:24.775127 edgeimpulse_api-1.23.6/edgeimpulse_api/models/device.py
+-rw-r--r--   0        0        0     2199 2023-05-18 14:36:24.879572 edgeimpulse_api-1.23.6/edgeimpulse_api/models/device_name_response.py
+-rw-r--r--   0        0        0     1920 2023-05-18 14:36:25.008393 edgeimpulse_api-1.23.6/edgeimpulse_api/models/device_name_response_all_of.py
+-rw-r--r--   0        0        0     2231 2023-05-18 14:36:25.293396 edgeimpulse_api-1.23.6/edgeimpulse_api/models/device_sensors_inner.py
+-rw-r--r--   0        0        0     2094 2023-05-18 14:36:24.854726 edgeimpulse_api-1.23.6/edgeimpulse_api/models/download.py
+-rw-r--r--   0        0        0     1912 2023-05-18 14:36:24.817952 edgeimpulse_api-1.23.6/edgeimpulse_api/models/download_portal_file_request.py
+-rw-r--r--   0        0        0     2260 2023-05-18 14:36:25.201165 edgeimpulse_api-1.23.6/edgeimpulse_api/models/download_portal_file_response.py
+-rw-r--r--   0        0        0     1954 2023-05-18 14:36:25.374949 edgeimpulse_api-1.23.6/edgeimpulse_api/models/download_portal_file_response_all_of.py
+-rw-r--r--   0        0        0     2724 2023-05-18 14:36:25.266856 edgeimpulse_api-1.23.6/edgeimpulse_api/models/dsp_autotuner_results.py
+-rw-r--r--   0        0        0     2417 2023-05-18 14:36:25.014479 edgeimpulse_api-1.23.6/edgeimpulse_api/models/dsp_autotuner_results_all_of.py
+-rw-r--r--   0        0        0     1968 2023-05-18 14:36:25.071769 edgeimpulse_api-1.23.6/edgeimpulse_api/models/dsp_autotuner_results_all_of_results.py
+-rw-r--r--   0        0        0     2870 2023-05-18 14:36:24.602245 edgeimpulse_api-1.23.6/edgeimpulse_api/models/dsp_block.py
+-rw-r--r--   0        0        0     1834 2023-05-18 14:36:24.518681 edgeimpulse_api-1.23.6/edgeimpulse_api/models/dsp_config_request.py
+-rw-r--r--   0        0        0     3092 2023-05-18 14:36:25.157742 edgeimpulse_api-1.23.6/edgeimpulse_api/models/dsp_config_response.py
+-rw-r--r--   0        0        0     2813 2023-05-18 14:36:25.141504 edgeimpulse_api-1.23.6/edgeimpulse_api/models/dsp_config_response_all_of.py
+-rw-r--r--   0        0        0     3016 2023-05-18 14:36:24.800981 edgeimpulse_api-1.23.6/edgeimpulse_api/models/dsp_feature_importance_response.py
+-rw-r--r--   0        0        0     2728 2023-05-18 14:36:24.668965 edgeimpulse_api-1.23.6/edgeimpulse_api/models/dsp_feature_importance_response_all_of.py
+-rw-r--r--   0        0        0     2058 2023-05-18 14:36:24.608255 edgeimpulse_api-1.23.6/edgeimpulse_api/models/dsp_feature_importance_response_all_of_features.py
+-rw-r--r--   0        0        0     2572 2023-05-18 14:36:25.272874 edgeimpulse_api-1.23.6/edgeimpulse_api/models/dsp_feature_importance_response_all_of_labels.py
+-rw-r--r--   0        0        0     2216 2023-05-18 14:36:24.755441 edgeimpulse_api-1.23.6/edgeimpulse_api/models/dsp_feature_labels_response.py
+-rw-r--r--   0        0        0     1920 2023-05-18 14:36:24.512927 edgeimpulse_api-1.23.6/edgeimpulse_api/models/dsp_feature_labels_response_all_of.py
+-rw-r--r--   0        0        0     2294 2023-05-18 14:36:24.954216 edgeimpulse_api-1.23.6/edgeimpulse_api/models/dsp_group.py
+-rw-r--r--   0        0        0     3628 2023-05-18 14:36:25.135714 edgeimpulse_api-1.23.6/edgeimpulse_api/models/dsp_group_item.py
+-rw-r--r--   0        0        0     2190 2023-05-18 14:36:24.647526 edgeimpulse_api-1.23.6/edgeimpulse_api/models/dsp_group_item_select_options_inner.py
+-rw-r--r--   0        0        0     2195 2023-05-18 14:36:24.705777 edgeimpulse_api-1.23.6/edgeimpulse_api/models/dsp_group_item_show_if.py
+-rw-r--r--   0        0        0     4410 2023-05-18 14:36:25.314351 edgeimpulse_api-1.23.6/edgeimpulse_api/models/dsp_info.py
+-rw-r--r--   0        0        0     2210 2023-05-18 14:36:25.221106 edgeimpulse_api-1.23.6/edgeimpulse_api/models/dsp_info_features.py
+-rw-r--r--   0        0        0     1885 2023-05-18 14:36:24.881905 edgeimpulse_api-1.23.6/edgeimpulse_api/models/dsp_info_performance.py
+-rw-r--r--   0        0        0     5144 2023-05-18 14:36:25.214339 edgeimpulse_api-1.23.6/edgeimpulse_api/models/dsp_metadata.py
+-rw-r--r--   0        0        0     2025 2023-05-18 14:36:25.085205 edgeimpulse_api-1.23.6/edgeimpulse_api/models/dsp_metadata_included_samples_inner.py
+-rw-r--r--   0        0        0     2566 2023-05-18 14:36:25.485254 edgeimpulse_api-1.23.6/edgeimpulse_api/models/dsp_metadata_output_config.py
+-rw-r--r--   0        0        0     2531 2023-05-18 14:36:24.704800 edgeimpulse_api-1.23.6/edgeimpulse_api/models/dsp_metadata_output_config_shape.py
+-rw-r--r--   0        0        0     5502 2023-05-18 14:36:25.215505 edgeimpulse_api-1.23.6/edgeimpulse_api/models/dsp_metadata_response.py
+-rw-r--r--   0        0        0     3019 2023-05-18 14:36:25.061993 edgeimpulse_api-1.23.6/edgeimpulse_api/models/dsp_performance_all_variants_response.py
+-rw-r--r--   0        0        0     2729 2023-05-18 14:36:24.615452 edgeimpulse_api-1.23.6/edgeimpulse_api/models/dsp_performance_all_variants_response_all_of.py
+-rw-r--r--   0        0        0     2278 2023-05-18 14:36:25.165408 edgeimpulse_api-1.23.6/edgeimpulse_api/models/dsp_performance_all_variants_response_all_of_performance.py
+-rw-r--r--   0        0        0     4639 2023-05-18 14:36:25.492825 edgeimpulse_api-1.23.6/edgeimpulse_api/models/dsp_run_graph.py
+-rw-r--r--   0        0        0     1899 2023-05-18 14:36:24.768615 edgeimpulse_api-1.23.6/edgeimpulse_api/models/dsp_run_graph_axis_labels.py
+-rw-r--r--   0        0        0     2677 2023-05-18 14:36:24.950334 edgeimpulse_api-1.23.6/edgeimpulse_api/models/dsp_run_request_with_features.py
+-rw-r--r--   0        0        0     2151 2023-05-18 14:36:24.963156 edgeimpulse_api-1.23.6/edgeimpulse_api/models/dsp_run_request_without_features.py
+-rw-r--r--   0        0        0     2030 2023-05-18 14:36:24.688617 edgeimpulse_api-1.23.6/edgeimpulse_api/models/dsp_run_request_without_features_read_only.py
+-rw-r--r--   0        0        0     3513 2023-05-18 14:36:25.072929 edgeimpulse_api-1.23.6/edgeimpulse_api/models/dsp_run_response.py
+-rw-r--r--   0        0        0     3234 2023-05-18 14:36:24.547399 edgeimpulse_api-1.23.6/edgeimpulse_api/models/dsp_run_response_all_of.py
+-rw-r--r--   0        0        0     1969 2023-05-18 14:36:25.404663 edgeimpulse_api-1.23.6/edgeimpulse_api/models/dsp_run_response_all_of_performance.py
+-rw-r--r--   0        0        0     4142 2023-05-18 14:36:24.595065 edgeimpulse_api-1.23.6/edgeimpulse_api/models/dsp_run_response_with_sample.py
+-rw-r--r--   0        0        0     3875 2023-05-18 14:36:25.405691 edgeimpulse_api-1.23.6/edgeimpulse_api/models/dsp_run_response_with_sample_all_of.py
+-rw-r--r--   0        0        0     3342 2023-05-18 14:36:24.715202 edgeimpulse_api-1.23.6/edgeimpulse_api/models/dsp_sample_features_response.py
+-rw-r--r--   0        0        0     3042 2023-05-18 14:36:25.022296 edgeimpulse_api-1.23.6/edgeimpulse_api/models/dsp_sample_features_response_all_of.py
+-rw-r--r--   0        0        0     2748 2023-05-18 14:36:25.190393 edgeimpulse_api-1.23.6/edgeimpulse_api/models/dsp_sample_features_response_all_of_data.py
+-rw-r--r--   0        0        0     2213 2023-05-18 14:36:25.263534 edgeimpulse_api-1.23.6/edgeimpulse_api/models/dsp_sample_features_response_all_of_sample.py
+-rw-r--r--   0        0        0     3353 2023-05-18 14:36:24.658042 edgeimpulse_api-1.23.6/edgeimpulse_api/models/dsp_trained_features_response.py
+-rw-r--r--   0        0        0     3053 2023-05-18 14:36:24.826281 edgeimpulse_api-1.23.6/edgeimpulse_api/models/dsp_trained_features_response_all_of.py
+-rw-r--r--   0        0        0     2773 2023-05-18 14:36:25.029941 edgeimpulse_api-1.23.6/edgeimpulse_api/models/dsp_trained_features_response_all_of_data.py
+-rw-r--r--   0        0        0     2205 2023-05-18 14:36:24.635893 edgeimpulse_api-1.23.6/edgeimpulse_api/models/dsp_trained_features_response_all_of_sample.py
+-rw-r--r--   0        0        0     1893 2023-05-18 14:36:25.335818 edgeimpulse_api-1.23.6/edgeimpulse_api/models/edit_sample_label_request.py
+-rw-r--r--   0        0        0     2656 2023-05-18 14:36:24.897385 edgeimpulse_api-1.23.6/edgeimpulse_api/models/evaluate_job_response.py
+-rw-r--r--   0        0        0     2349 2023-05-18 14:36:24.738931 edgeimpulse_api-1.23.6/edgeimpulse_api/models/evaluate_job_response_all_of.py
+-rw-r--r--   0        0        0     2099 2023-05-18 14:36:24.572876 edgeimpulse_api-1.23.6/edgeimpulse_api/models/evaluate_result_value.py
+-rw-r--r--   0        0        0     2511 2023-05-18 14:36:24.667142 edgeimpulse_api-1.23.6/edgeimpulse_api/models/export_get_url_response.py
+-rw-r--r--   0        0        0     2244 2023-05-18 14:36:24.543907 edgeimpulse_api-1.23.6/edgeimpulse_api/models/export_get_url_response_all_of.py
+-rw-r--r--   0        0        0     2373 2023-05-18 14:36:24.680349 edgeimpulse_api-1.23.6/edgeimpulse_api/models/export_original_data_request.py
+-rw-r--r--   0        0        0     2021 2023-05-18 14:36:25.102026 edgeimpulse_api-1.23.6/edgeimpulse_api/models/export_wav_data_request.py
+-rw-r--r--   0        0        0     2206 2023-05-18 14:36:25.166287 edgeimpulse_api-1.23.6/edgeimpulse_api/models/find_segment_sample_request.py
+-rw-r--r--   0        0        0     2804 2023-05-18 14:36:25.442474 edgeimpulse_api-1.23.6/edgeimpulse_api/models/find_segment_sample_response.py
+-rw-r--r--   0        0        0     2497 2023-05-18 14:36:25.030817 edgeimpulse_api-1.23.6/edgeimpulse_api/models/find_segment_sample_response_all_of.py
+-rw-r--r--   0        0        0     2090 2023-05-18 14:36:25.042525 edgeimpulse_api-1.23.6/edgeimpulse_api/models/find_segment_sample_response_all_of_segments.py
+-rw-r--r--   0        0        0     2665 2023-05-18 14:36:24.776118 edgeimpulse_api-1.23.6/edgeimpulse_api/models/find_user_response.py
+-rw-r--r--   0        0        0     2358 2023-05-18 14:36:25.446921 edgeimpulse_api-1.23.6/edgeimpulse_api/models/find_user_response_all_of.py
+-rw-r--r--   0        0        0     2322 2023-05-18 14:36:24.697326 edgeimpulse_api-1.23.6/edgeimpulse_api/models/find_user_response_all_of_users.py
+-rw-r--r--   0        0        0     2507 2023-05-18 14:36:25.097495 edgeimpulse_api-1.23.6/edgeimpulse_api/models/generate_features_request.py
+-rw-r--r--   0        0        0     2083 2023-05-18 14:36:24.708953 edgeimpulse_api-1.23.6/edgeimpulse_api/models/generic_api_response.py
+-rw-r--r--   0        0        0     2698 2023-05-18 14:36:25.319485 edgeimpulse_api-1.23.6/edgeimpulse_api/models/get_all_third_party_auth_response.py
+-rw-r--r--   0        0        0     2391 2023-05-18 14:36:25.388958 edgeimpulse_api-1.23.6/edgeimpulse_api/models/get_all_third_party_auth_response_all_of.py
+-rw-r--r--   0        0        0     2713 2023-05-18 14:36:24.888272 edgeimpulse_api-1.23.6/edgeimpulse_api/models/get_all_whitelabels_response.py
+-rw-r--r--   0        0        0     2406 2023-05-18 14:36:24.549264 edgeimpulse_api-1.23.6/edgeimpulse_api/models/get_all_whitelabels_response_all_of.py
+-rw-r--r--   0        0        0     3400 2023-05-18 14:36:24.753551 edgeimpulse_api-1.23.6/edgeimpulse_api/models/get_data_explorer_features_response.py
+-rw-r--r--   0        0        0     3122 2023-05-18 14:36:24.969262 edgeimpulse_api-1.23.6/edgeimpulse_api/models/get_data_explorer_features_response_all_of.py
+-rw-r--r--   0        0        0     3752 2023-05-18 14:36:25.443914 edgeimpulse_api-1.23.6/edgeimpulse_api/models/get_data_explorer_settings_response.py
+-rw-r--r--   0        0        0     2402 2023-05-18 14:36:25.321329 edgeimpulse_api-1.23.6/edgeimpulse_api/models/get_data_explorer_settings_response_all_of.py
+-rw-r--r--   0        0        0     2349 2023-05-18 14:36:25.170470 edgeimpulse_api-1.23.6/edgeimpulse_api/models/get_deployment_response.py
+-rw-r--r--   0        0        0     2071 2023-05-18 14:36:25.407146 edgeimpulse_api-1.23.6/edgeimpulse_api/models/get_deployment_response_all_of.py
+-rw-r--r--   0        0        0     2434 2023-05-18 14:36:25.024700 edgeimpulse_api-1.23.6/edgeimpulse_api/models/get_device_response.py
+-rw-r--r--   0        0        0     2137 2023-05-18 14:36:25.295113 edgeimpulse_api-1.23.6/edgeimpulse_api/models/get_device_response_all_of.py
+-rw-r--r--   0        0        0     3930 2023-05-18 14:36:25.285583 edgeimpulse_api-1.23.6/edgeimpulse_api/models/get_impulse_blocks_response.py
+-rw-r--r--   0        0        0     3630 2023-05-18 14:36:24.655366 edgeimpulse_api-1.23.6/edgeimpulse_api/models/get_impulse_blocks_response_all_of.py
+-rw-r--r--   0        0        0     2454 2023-05-18 14:36:24.530974 edgeimpulse_api-1.23.6/edgeimpulse_api/models/get_impulse_response.py
+-rw-r--r--   0        0        0     2157 2023-05-18 14:36:25.249738 edgeimpulse_api-1.23.6/edgeimpulse_api/models/get_impulse_response_all_of.py
+-rw-r--r--   0        0        0     2374 2023-05-18 14:36:24.947441 edgeimpulse_api-1.23.6/edgeimpulse_api/models/get_job_response.py
+-rw-r--r--   0        0        0     2077 2023-05-18 14:36:25.268899 edgeimpulse_api-1.23.6/edgeimpulse_api/models/get_job_response_all_of.py
+-rw-r--r--   0        0        0     2650 2023-05-18 14:36:24.517800 edgeimpulse_api-1.23.6/edgeimpulse_api/models/get_jwt_request.py
+-rw-r--r--   0        0        0     2431 2023-05-18 14:36:24.910200 edgeimpulse_api-1.23.6/edgeimpulse_api/models/get_jwt_response.py
+-rw-r--r--   0        0        0     2152 2023-05-18 14:36:24.565869 edgeimpulse_api-1.23.6/edgeimpulse_api/models/get_jwt_response_all_of.py
+-rw-r--r--   0        0        0     2977 2023-05-18 14:36:24.585555 edgeimpulse_api-1.23.6/edgeimpulse_api/models/get_last_deployment_build_response.py
+-rw-r--r--   0        0        0     2699 2023-05-18 14:36:24.957385 edgeimpulse_api-1.23.6/edgeimpulse_api/models/get_last_deployment_build_response_all_of.py
+-rw-r--r--   0        0        0     2869 2023-05-18 14:36:25.326866 edgeimpulse_api-1.23.6/edgeimpulse_api/models/get_last_deployment_build_response_all_of_last_build.py
+-rw-r--r--   0        0        0     2572 2023-05-18 14:36:25.459458 edgeimpulse_api-1.23.6/edgeimpulse_api/models/get_notes_response.py
+-rw-r--r--   0        0        0     2265 2023-05-18 14:36:25.256868 edgeimpulse_api-1.23.6/edgeimpulse_api/models/get_notes_response_all_of.py
+-rw-r--r--   0        0        0     2561 2023-05-18 14:36:25.471649 edgeimpulse_api-1.23.6/edgeimpulse_api/models/get_organization_data_item_response.py
+-rw-r--r--   0        0        0     2237 2023-05-18 14:36:25.343788 edgeimpulse_api-1.23.6/edgeimpulse_api/models/get_organization_data_item_response_all_of.py
+-rw-r--r--   0        0        0     3411 2023-05-18 14:36:24.769844 edgeimpulse_api-1.23.6/edgeimpulse_api/models/get_organization_data_item_transform_jobs_response.py
+-rw-r--r--   0        0        0     3111 2023-05-18 14:36:24.645809 edgeimpulse_api-1.23.6/edgeimpulse_api/models/get_organization_data_item_transform_jobs_response_all_of.py
+-rw-r--r--   0        0        0     3398 2023-05-18 14:36:24.907622 edgeimpulse_api-1.23.6/edgeimpulse_api/models/get_organization_data_item_transform_jobs_response_all_of_transformation_jobs.py
+-rw-r--r--   0        0        0     2576 2023-05-18 14:36:25.039197 edgeimpulse_api-1.23.6/edgeimpulse_api/models/get_organization_dataset_response.py
+-rw-r--r--   0        0        0     2252 2023-05-18 14:36:25.063468 edgeimpulse_api-1.23.6/edgeimpulse_api/models/get_organization_dataset_response_all_of.py
+-rw-r--r--   0        0        0     2603 2023-05-18 14:36:25.259049 edgeimpulse_api-1.23.6/edgeimpulse_api/models/get_organization_pipelines_response.py
+-rw-r--r--   0        0        0     2279 2023-05-18 14:36:24.588804 edgeimpulse_api-1.23.6/edgeimpulse_api/models/get_organization_pipelines_response_all_of.py
+-rw-r--r--   0        0        0     3670 2023-05-18 14:36:25.371478 edgeimpulse_api-1.23.6/edgeimpulse_api/models/get_organization_portal_response.py
+-rw-r--r--   0        0        0     3391 2023-05-18 14:36:24.652413 edgeimpulse_api-1.23.6/edgeimpulse_api/models/get_organization_portal_response_all_of.py
+-rw-r--r--   0        0        0     2323 2023-05-18 14:36:24.793219 edgeimpulse_api-1.23.6/edgeimpulse_api/models/get_organization_projects_data_count_response.py
+-rw-r--r--   0        0        0     2905 2023-05-18 14:36:24.571934 edgeimpulse_api-1.23.6/edgeimpulse_api/models/get_performance_calibration_ground_truth_response.py
+-rw-r--r--   0        0        0     2598 2023-05-18 14:36:24.929337 edgeimpulse_api-1.23.6/edgeimpulse_api/models/get_performance_calibration_ground_truth_response_all_of.py
+-rw-r--r--   0        0        0     3012 2023-05-18 14:36:25.005731 edgeimpulse_api-1.23.6/edgeimpulse_api/models/get_performance_calibration_parameter_sets_response.py
+-rw-r--r--   0        0        0     2712 2023-05-18 14:36:24.626593 edgeimpulse_api-1.23.6/edgeimpulse_api/models/get_performance_calibration_parameter_sets_response_all_of.py
+-rw-r--r--   0        0        0     2722 2023-05-18 14:36:24.555288 edgeimpulse_api-1.23.6/edgeimpulse_api/models/get_performance_calibration_parameters_response.py
+-rw-r--r--   0        0        0     2425 2023-05-18 14:36:25.359966 edgeimpulse_api-1.23.6/edgeimpulse_api/models/get_performance_calibration_parameters_response_all_of.py
+-rw-r--r--   0        0        0     2922 2023-05-18 14:36:24.720985 edgeimpulse_api-1.23.6/edgeimpulse_api/models/get_performance_calibration_raw_result_response.py
+-rw-r--r--   0        0        0     2615 2023-05-18 14:36:24.900205 edgeimpulse_api-1.23.6/edgeimpulse_api/models/get_performance_calibration_raw_result_response_all_of.py
+-rw-r--r--   0        0        0     3151 2023-05-18 14:36:24.490526 edgeimpulse_api-1.23.6/edgeimpulse_api/models/get_performance_calibration_status_response.py
+-rw-r--r--   0        0        0     2884 2023-05-18 14:36:24.930353 edgeimpulse_api-1.23.6/edgeimpulse_api/models/get_performance_calibration_status_response_all_of.py
+-rw-r--r--   0        0        0     3761 2023-05-18 14:36:25.009338 edgeimpulse_api-1.23.6/edgeimpulse_api/models/get_pretrained_model_response.py
+-rw-r--r--   0        0        0     3483 2023-05-18 14:36:25.251189 edgeimpulse_api-1.23.6/edgeimpulse_api/models/get_pretrained_model_response_all_of.py
+-rw-r--r--   0        0        0     3861 2023-05-18 14:36:24.717272 edgeimpulse_api-1.23.6/edgeimpulse_api/models/get_pretrained_model_response_all_of_model.py
+-rw-r--r--   0        0        0     2978 2023-05-18 14:36:24.906045 edgeimpulse_api-1.23.6/edgeimpulse_api/models/get_pretrained_model_response_all_of_model_info.py
+-rw-r--r--   0        0        0     3058 2023-05-18 14:36:24.713208 edgeimpulse_api-1.23.6/edgeimpulse_api/models/get_pretrained_model_response_all_of_model_profile_info.py
+-rw-r--r--   0        0        0     2397 2023-05-18 14:36:24.752663 edgeimpulse_api-1.23.6/edgeimpulse_api/models/get_public_metrics_response.py
+-rw-r--r--   0        0        0     2073 2023-05-18 14:36:25.101047 edgeimpulse_api-1.23.6/edgeimpulse_api/models/get_public_metrics_response_all_of.py
+-rw-r--r--   0        0        0     2767 2023-05-18 14:36:25.021007 edgeimpulse_api-1.23.6/edgeimpulse_api/models/get_sample_metadata_response.py
+-rw-r--r--   0        0        0     3044 2023-05-18 14:36:25.475881 edgeimpulse_api-1.23.6/edgeimpulse_api/models/get_sample_response.py
+-rw-r--r--   0        0        0     2462 2023-05-18 14:36:25.280979 edgeimpulse_api-1.23.6/edgeimpulse_api/models/get_syntiant_posterior_response.py
+-rw-r--r--   0        0        0     2184 2023-05-18 14:36:25.269807 edgeimpulse_api-1.23.6/edgeimpulse_api/models/get_syntiant_posterior_response_all_of.py
+-rw-r--r--   0        0        0     2414 2023-05-18 14:36:24.890704 edgeimpulse_api-1.23.6/edgeimpulse_api/models/get_theme_response.py
+-rw-r--r--   0        0        0     2117 2023-05-18 14:36:24.857901 edgeimpulse_api-1.23.6/edgeimpulse_api/models/get_theme_response_all_of.py
+-rw-r--r--   0        0        0     2592 2023-05-18 14:36:24.824890 edgeimpulse_api-1.23.6/edgeimpulse_api/models/get_themes_response.py
+-rw-r--r--   0        0        0     2285 2023-05-18 14:36:25.370092 edgeimpulse_api-1.23.6/edgeimpulse_api/models/get_themes_response_all_of.py
+-rw-r--r--   0        0        0     2495 2023-05-18 14:36:25.112086 edgeimpulse_api-1.23.6/edgeimpulse_api/models/get_third_party_auth_response.py
+-rw-r--r--   0        0        0     2171 2023-05-18 14:36:24.628719 edgeimpulse_api-1.23.6/edgeimpulse_api/models/get_third_party_auth_response_all_of.py
+-rw-r--r--   0        0        0     2703 2023-05-18 14:36:25.110654 edgeimpulse_api-1.23.6/edgeimpulse_api/models/get_user_need_to_set_password_response.py
+-rw-r--r--   0        0        0     2436 2023-05-18 14:36:25.086912 edgeimpulse_api-1.23.6/edgeimpulse_api/models/get_user_need_to_set_password_response_all_of.py
+-rw-r--r--   0        0        0     7432 2023-05-18 14:36:24.718365 edgeimpulse_api-1.23.6/edgeimpulse_api/models/get_user_response.py
+-rw-r--r--   0        0        0     5563 2023-05-18 14:36:25.052933 edgeimpulse_api-1.23.6/edgeimpulse_api/models/get_user_response_all_of.py
+-rw-r--r--   0        0        0     2395 2023-05-18 14:36:25.312829 edgeimpulse_api-1.23.6/edgeimpulse_api/models/get_user_response_all_of_whitelabels.py
+-rw-r--r--   0        0        0     2307 2023-05-18 14:36:24.935779 edgeimpulse_api-1.23.6/edgeimpulse_api/models/get_whitelabel_domain_response.py
+-rw-r--r--   0        0        0     2021 2023-05-18 14:36:24.931305 edgeimpulse_api-1.23.6/edgeimpulse_api/models/get_whitelabel_domain_response_all_of.py
+-rw-r--r--   0        0        0     2514 2023-05-18 14:36:25.041300 edgeimpulse_api-1.23.6/edgeimpulse_api/models/get_whitelabel_response.py
+-rw-r--r--   0        0        0     2217 2023-05-18 14:36:25.123170 edgeimpulse_api-1.23.6/edgeimpulse_api/models/get_whitelabel_response_all_of.py
+-rw-r--r--   0        0        0     2776 2023-05-18 14:36:24.765648 edgeimpulse_api-1.23.6/edgeimpulse_api/models/has_data_explorer_features_response.py
+-rw-r--r--   0        0        0     2498 2023-05-18 14:36:25.182849 edgeimpulse_api-1.23.6/edgeimpulse_api/models/has_data_explorer_features_response_all_of.py
+-rw-r--r--   0        0        0     3738 2023-05-18 14:36:24.683851 edgeimpulse_api-1.23.6/edgeimpulse_api/models/impulse.py
+-rw-r--r--   0        0        0     6723 2023-05-18 14:36:24.665798 edgeimpulse_api-1.23.6/edgeimpulse_api/models/impulse_block_version.py
+-rw-r--r--   0        0        0     6814 2023-05-18 14:36:25.204490 edgeimpulse_api-1.23.6/edgeimpulse_api/models/impulse_dsp_block.py
+-rw-r--r--   0        0        0     1967 2023-05-18 14:36:25.232471 edgeimpulse_api-1.23.6/edgeimpulse_api/models/impulse_dsp_block_organization.py
+-rw-r--r--   0        0        0     8976 2023-05-18 14:36:25.155388 edgeimpulse_api-1.23.6/edgeimpulse_api/models/impulse_input_block.py
+-rw-r--r--   0        0        0     5612 2023-05-18 14:36:25.025923 edgeimpulse_api-1.23.6/edgeimpulse_api/models/impulse_learn_block.py
+-rw-r--r--   0        0        0     2463 2023-05-18 14:36:25.454267 edgeimpulse_api-1.23.6/edgeimpulse_api/models/input_block.py
+-rw-r--r--   0        0        0     2456 2023-05-18 14:36:24.977732 edgeimpulse_api-1.23.6/edgeimpulse_api/models/invite_organization_member_request.py
+-rw-r--r--   0        0        0     3668 2023-05-18 14:36:24.829546 edgeimpulse_api-1.23.6/edgeimpulse_api/models/job.py
+-rw-r--r--   0        0        0     2713 2023-05-18 14:36:25.211162 edgeimpulse_api-1.23.6/edgeimpulse_api/models/job_summary_response.py
+-rw-r--r--   0        0        0     2406 2023-05-18 14:36:24.560716 edgeimpulse_api-1.23.6/edgeimpulse_api/models/job_summary_response_all_of.py
+-rw-r--r--   0        0        0     2089 2023-05-18 14:36:25.377890 edgeimpulse_api-1.23.6/edgeimpulse_api/models/job_summary_response_all_of_summary.py
+-rw-r--r--   0        0        0     2510 2023-05-18 14:36:25.412854 edgeimpulse_api-1.23.6/edgeimpulse_api/models/keras_model_layer.py
+-rw-r--r--   0        0        0     2093 2023-05-18 14:36:25.432046 edgeimpulse_api-1.23.6/edgeimpulse_api/models/keras_model_layer_input.py
+-rw-r--r--   0        0        0     2101 2023-05-18 14:36:25.265848 edgeimpulse_api-1.23.6/edgeimpulse_api/models/keras_model_layer_output.py
+-rw-r--r--   0        0        0     5189 2023-05-18 14:36:25.161992 edgeimpulse_api-1.23.6/edgeimpulse_api/models/keras_model_metadata.py
+-rw-r--r--   0        0        0     4922 2023-05-18 14:36:25.278231 edgeimpulse_api-1.23.6/edgeimpulse_api/models/keras_model_metadata_all_of.py
+-rw-r--r--   0        0        0     4792 2023-05-18 14:36:24.972827 edgeimpulse_api-1.23.6/edgeimpulse_api/models/keras_model_metadata_metrics.py
+-rw-r--r--   0        0        0     3228 2023-05-18 14:36:25.174382 edgeimpulse_api-1.23.6/edgeimpulse_api/models/keras_model_metadata_metrics_on_device_performance_inner.py
+-rw-r--r--   0        0        0     2497 2023-05-18 14:36:25.149936 edgeimpulse_api-1.23.6/edgeimpulse_api/models/keras_model_metadata_metrics_on_device_performance_inner_tflite.py
+-rw-r--r--   0        0        0      562 2023-05-18 14:36:25.235485 edgeimpulse_api-1.23.6/edgeimpulse_api/models/keras_model_type_enum.py
+-rw-r--r--   0        0        0     9556 2023-05-18 14:36:24.519674 edgeimpulse_api-1.23.6/edgeimpulse_api/models/keras_response.py
+-rw-r--r--   0        0        0     9289 2023-05-18 14:36:24.751673 edgeimpulse_api-1.23.6/edgeimpulse_api/models/keras_response_all_of.py
+-rw-r--r--   0        0        0     3392 2023-05-18 14:36:25.238502 edgeimpulse_api-1.23.6/edgeimpulse_api/models/keras_visual_layer.py
+-rw-r--r--   0        0        0     2310 2023-05-18 14:36:25.113568 edgeimpulse_api-1.23.6/edgeimpulse_api/models/keras_visual_layer_type.py
+-rw-r--r--   0        0        0     2529 2023-05-18 14:36:24.535374 edgeimpulse_api-1.23.6/edgeimpulse_api/models/last_modification_date_response.py
+-rw-r--r--   0        0        0     2239 2023-05-18 14:36:24.671922 edgeimpulse_api-1.23.6/edgeimpulse_api/models/last_modification_date_response_all_of.py
+-rw-r--r--   0        0        0     2633 2023-05-18 14:36:25.128983 edgeimpulse_api-1.23.6/edgeimpulse_api/models/latency_device.py
+-rw-r--r--   0        0        0     2424 2023-05-18 14:36:24.604059 edgeimpulse_api-1.23.6/edgeimpulse_api/models/learn_block.py
+-rw-r--r--   0        0        0      883 2023-05-18 14:36:25.280114 edgeimpulse_api-1.23.6/edgeimpulse_api/models/learn_block_type.py
+-rw-r--r--   0        0        0     2788 2023-05-18 14:36:25.219734 edgeimpulse_api-1.23.6/edgeimpulse_api/models/list_api_keys_response.py
+-rw-r--r--   0        0        0     2488 2023-05-18 14:36:24.622588 edgeimpulse_api-1.23.6/edgeimpulse_api/models/list_api_keys_response_all_of.py
+-rw-r--r--   0        0        0     2682 2023-05-18 14:36:25.279184 edgeimpulse_api-1.23.6/edgeimpulse_api/models/list_api_keys_response_all_of_api_keys.py
+-rw-r--r--   0        0        0     2630 2023-05-18 14:36:25.148387 edgeimpulse_api-1.23.6/edgeimpulse_api/models/list_devices_response.py
+-rw-r--r--   0        0        0     2333 2023-05-18 14:36:24.515885 edgeimpulse_api-1.23.6/edgeimpulse_api/models/list_devices_response_all_of.py
+-rw-r--r--   0        0        0     2726 2023-05-18 14:36:24.794772 edgeimpulse_api-1.23.6/edgeimpulse_api/models/list_email_response.py
+-rw-r--r--   0        0        0     2426 2023-05-18 14:36:24.952188 edgeimpulse_api-1.23.6/edgeimpulse_api/models/list_email_response_all_of.py
+-rw-r--r--   0        0        0     2918 2023-05-18 14:36:25.047721 edgeimpulse_api-1.23.6/edgeimpulse_api/models/list_email_response_all_of_emails.py
+-rw-r--r--   0        0        0     2813 2023-05-18 14:36:25.257990 edgeimpulse_api-1.23.6/edgeimpulse_api/models/list_hmac_keys_response.py
+-rw-r--r--   0        0        0     2513 2023-05-18 14:36:25.007499 edgeimpulse_api-1.23.6/edgeimpulse_api/models/list_hmac_keys_response_all_of.py
+-rw-r--r--   0        0        0     2381 2023-05-18 14:36:24.866322 edgeimpulse_api-1.23.6/edgeimpulse_api/models/list_hmac_keys_response_all_of_hmac_keys.py
+-rw-r--r--   0        0        0     2745 2023-05-18 14:36:24.532560 edgeimpulse_api-1.23.6/edgeimpulse_api/models/list_jobs_response.py
+-rw-r--r--   0        0        0     2445 2023-05-18 14:36:24.895937 edgeimpulse_api-1.23.6/edgeimpulse_api/models/list_jobs_response_all_of.py
+-rw-r--r--   0        0        0     2200 2023-05-18 14:36:25.057646 edgeimpulse_api-1.23.6/edgeimpulse_api/models/list_models_response.py
+-rw-r--r--   0        0        0     1910 2023-05-18 14:36:25.488172 edgeimpulse_api-1.23.6/edgeimpulse_api/models/list_models_response_all_of.py
+-rw-r--r--   0        0        0     2921 2023-05-18 14:36:25.354301 edgeimpulse_api-1.23.6/edgeimpulse_api/models/list_organization_api_keys_response.py
+-rw-r--r--   0        0        0     2621 2023-05-18 14:36:24.678958 edgeimpulse_api-1.23.6/edgeimpulse_api/models/list_organization_api_keys_response_all_of.py
+-rw-r--r--   0        0        0     2760 2023-05-18 14:36:24.762955 edgeimpulse_api-1.23.6/edgeimpulse_api/models/list_organization_api_keys_response_all_of_api_keys.py
+-rw-r--r--   0        0        0     2857 2023-05-18 14:36:24.762106 edgeimpulse_api-1.23.6/edgeimpulse_api/models/list_organization_buckets_response.py
+-rw-r--r--   0        0        0     2550 2023-05-18 14:36:25.448980 edgeimpulse_api-1.23.6/edgeimpulse_api/models/list_organization_buckets_response_all_of.py
+-rw-r--r--   0        0        0     2995 2023-05-18 14:36:25.416485 edgeimpulse_api-1.23.6/edgeimpulse_api/models/list_organization_buckets_response_all_of_buckets.py
+-rw-r--r--   0        0        0     2902 2023-05-18 14:36:25.121126 edgeimpulse_api-1.23.6/edgeimpulse_api/models/list_organization_buckets_user_response.py
+-rw-r--r--   0        0        0     2595 2023-05-18 14:36:25.033445 edgeimpulse_api-1.23.6/edgeimpulse_api/models/list_organization_buckets_user_response_all_of.py
+-rw-r--r--   0        0        0     2760 2023-05-18 14:36:24.742740 edgeimpulse_api-1.23.6/edgeimpulse_api/models/list_organization_buckets_user_response_all_of_buckets.py
+-rw-r--r--   0        0        0     3310 2023-05-18 14:36:25.171733 edgeimpulse_api-1.23.6/edgeimpulse_api/models/list_organization_data_response.py
+-rw-r--r--   0        0        0     3031 2023-05-18 14:36:24.641695 edgeimpulse_api-1.23.6/edgeimpulse_api/models/list_organization_data_response_all_of.py
+-rw-r--r--   0        0        0     3430 2023-05-18 14:36:25.470272 edgeimpulse_api-1.23.6/edgeimpulse_api/models/list_organization_data_response_all_of_data.py
+-rw-r--r--   0        0        0     2887 2023-05-18 14:36:25.363256 edgeimpulse_api-1.23.6/edgeimpulse_api/models/list_organization_deploy_blocks_response.py
+-rw-r--r--   0        0        0     2587 2023-05-18 14:36:24.634583 edgeimpulse_api-1.23.6/edgeimpulse_api/models/list_organization_deploy_blocks_response_all_of.py
+-rw-r--r--   0        0        0     2824 2023-05-18 14:36:24.834863 edgeimpulse_api-1.23.6/edgeimpulse_api/models/list_organization_dsp_blocks_response.py
+-rw-r--r--   0        0        0     2524 2023-05-18 14:36:25.329657 edgeimpulse_api-1.23.6/edgeimpulse_api/models/list_organization_dsp_blocks_response_all_of.py
+-rw-r--r--   0        0        0     3353 2023-05-18 14:36:24.790063 edgeimpulse_api-1.23.6/edgeimpulse_api/models/list_organization_files_response.py
+-rw-r--r--   0        0        0     3074 2023-05-18 14:36:25.153078 edgeimpulse_api-1.23.6/edgeimpulse_api/models/list_organization_files_response_all_of.py
+-rw-r--r--   0        0        0     2792 2023-05-18 14:36:24.788405 edgeimpulse_api-1.23.6/edgeimpulse_api/models/list_organization_pipelines_response.py
+-rw-r--r--   0        0        0     2485 2023-05-18 14:36:24.618477 edgeimpulse_api-1.23.6/edgeimpulse_api/models/list_organization_pipelines_response_all_of.py
+-rw-r--r--   0        0        0     2857 2023-05-18 14:36:25.045092 edgeimpulse_api-1.23.6/edgeimpulse_api/models/list_organization_portals_response.py
+-rw-r--r--   0        0        0     2550 2023-05-18 14:36:25.159391 edgeimpulse_api-1.23.6/edgeimpulse_api/models/list_organization_portals_response_all_of.py
+-rw-r--r--   0        0        0     2744 2023-05-18 14:36:25.340448 edgeimpulse_api-1.23.6/edgeimpulse_api/models/list_organization_portals_response_all_of_portals.py
+-rw-r--r--   0        0        0     3449 2023-05-18 14:36:24.700222 edgeimpulse_api-1.23.6/edgeimpulse_api/models/list_organization_projects_data_response.py
+-rw-r--r--   0        0        0     3142 2023-05-18 14:36:24.777027 edgeimpulse_api-1.23.6/edgeimpulse_api/models/list_organization_projects_data_response_all_of.py
+-rw-r--r--   0        0        0     2271 2023-05-18 14:36:24.886317 edgeimpulse_api-1.23.6/edgeimpulse_api/models/list_organization_projects_data_response_all_of_projects.py
+-rw-r--r--   0        0        0     2723 2023-05-18 14:36:25.040343 edgeimpulse_api-1.23.6/edgeimpulse_api/models/list_organization_projects_response.py
+-rw-r--r--   0        0        0     2416 2023-05-18 14:36:24.862331 edgeimpulse_api-1.23.6/edgeimpulse_api/models/list_organization_projects_response_all_of.py
+-rw-r--r--   0        0        0     2857 2023-05-18 14:36:24.579162 edgeimpulse_api-1.23.6/edgeimpulse_api/models/list_organization_secrets_response.py
+-rw-r--r--   0        0        0     2550 2023-05-18 14:36:24.597497 edgeimpulse_api-1.23.6/edgeimpulse_api/models/list_organization_secrets_response_all_of.py
+-rw-r--r--   0        0        0     2265 2023-05-18 14:36:25.323737 edgeimpulse_api-1.23.6/edgeimpulse_api/models/list_organization_secrets_response_all_of_secrets.py
+-rw-r--r--   0        0        0     3103 2023-05-18 14:36:24.744234 edgeimpulse_api-1.23.6/edgeimpulse_api/models/list_organization_transfer_learning_blocks_response.py
+-rw-r--r--   0        0        0     2803 2023-05-18 14:36:25.368452 edgeimpulse_api-1.23.6/edgeimpulse_api/models/list_organization_transfer_learning_blocks_response_all_of.py
+-rw-r--r--   0        0        0     3055 2023-05-18 14:36:24.919993 edgeimpulse_api-1.23.6/edgeimpulse_api/models/list_organization_transformation_blocks_response.py
+-rw-r--r--   0        0        0     2755 2023-05-18 14:36:25.088359 edgeimpulse_api-1.23.6/edgeimpulse_api/models/list_organization_transformation_blocks_response_all_of.py
+-rw-r--r--   0        0        0     2786 2023-05-18 14:36:25.181344 edgeimpulse_api-1.23.6/edgeimpulse_api/models/list_organizations_response.py
+-rw-r--r--   0        0        0     2486 2023-05-18 14:36:25.499433 edgeimpulse_api-1.23.6/edgeimpulse_api/models/list_organizations_response_all_of.py
+-rw-r--r--   0        0        0     1937 2023-05-18 14:36:24.865059 edgeimpulse_api-1.23.6/edgeimpulse_api/models/list_portal_files_in_folder_request.py
+-rw-r--r--   0        0        0     2713 2023-05-18 14:36:25.230867 edgeimpulse_api-1.23.6/edgeimpulse_api/models/list_portal_files_in_folder_response.py
+-rw-r--r--   0        0        0     2416 2023-05-18 14:36:24.903213 edgeimpulse_api-1.23.6/edgeimpulse_api/models/list_portal_files_in_folder_response_all_of.py
+-rw-r--r--   0        0        0     2290 2023-05-18 14:36:25.107660 edgeimpulse_api-1.23.6/edgeimpulse_api/models/list_projects.py
+-rw-r--r--   0        0        0     2681 2023-05-18 14:36:25.496457 edgeimpulse_api-1.23.6/edgeimpulse_api/models/list_projects_response.py
+-rw-r--r--   0        0        0     2553 2023-05-18 14:36:25.004573 edgeimpulse_api-1.23.6/edgeimpulse_api/models/list_public_projects.py
+-rw-r--r--   0        0        0     2944 2023-05-18 14:36:24.695779 edgeimpulse_api-1.23.6/edgeimpulse_api/models/list_public_projects_response.py
+-rw-r--r--   0        0        0     2815 2023-05-18 14:36:25.137215 edgeimpulse_api-1.23.6/edgeimpulse_api/models/list_public_versions_response.py
+-rw-r--r--   0        0        0     2508 2023-05-18 14:36:25.102981 edgeimpulse_api-1.23.6/edgeimpulse_api/models/list_public_versions_response_all_of.py
+-rw-r--r--   0        0        0     2290 2023-05-18 14:36:25.387706 edgeimpulse_api-1.23.6/edgeimpulse_api/models/list_public_versions_response_all_of_versions.py
+-rw-r--r--   0        0        0     2754 2023-05-18 14:36:24.687178 edgeimpulse_api-1.23.6/edgeimpulse_api/models/list_samples_response.py
+-rw-r--r--   0        0        0     2454 2023-05-18 14:36:24.860702 edgeimpulse_api-1.23.6/edgeimpulse_api/models/list_samples_response_all_of.py
+-rw-r--r--   0        0        0     3933 2023-05-18 14:36:24.814559 edgeimpulse_api-1.23.6/edgeimpulse_api/models/list_versions_response.py
+-rw-r--r--   0        0        0     3633 2023-05-18 14:36:24.609563 edgeimpulse_api-1.23.6/edgeimpulse_api/models/list_versions_response_all_of.py
+-rw-r--r--   0        0        0     2353 2023-05-18 14:36:25.455429 edgeimpulse_api-1.23.6/edgeimpulse_api/models/list_versions_response_all_of_bucket.py
+-rw-r--r--   0        0        0     2053 2023-05-18 14:36:24.774158 edgeimpulse_api-1.23.6/edgeimpulse_api/models/list_versions_response_all_of_custom_learn_blocks.py
+-rw-r--r--   0        0        0     3960 2023-05-18 14:36:24.760374 edgeimpulse_api-1.23.6/edgeimpulse_api/models/list_versions_response_all_of_versions.py
+-rw-r--r--   0        0        0     2900 2023-05-18 14:36:25.376374 edgeimpulse_api-1.23.6/edgeimpulse_api/models/log_stdout_response.py
+-rw-r--r--   0        0        0     2600 2023-05-18 14:36:25.413733 edgeimpulse_api-1.23.6/edgeimpulse_api/models/log_stdout_response_all_of.py
+-rw-r--r--   0        0        0     2441 2023-05-18 14:36:24.799398 edgeimpulse_api-1.23.6/edgeimpulse_api/models/log_stdout_response_all_of_stdout.py
+-rw-r--r--   0        0        0     2191 2023-05-18 14:36:24.892923 edgeimpulse_api-1.23.6/edgeimpulse_api/models/log_website_pageview_request.py
+-rw-r--r--   0        0        0     2217 2023-05-18 14:36:24.569259 edgeimpulse_api-1.23.6/edgeimpulse_api/models/login_response.py
+-rw-r--r--   0        0        0     1911 2023-05-18 14:36:25.207419 edgeimpulse_api-1.23.6/edgeimpulse_api/models/login_response_all_of.py
+-rw-r--r--   0        0        0     2521 2023-05-18 14:36:25.299981 edgeimpulse_api-1.23.6/edgeimpulse_api/models/model_prediction.py
+-rw-r--r--   0        0        0     2895 2023-05-18 14:36:25.106253 edgeimpulse_api-1.23.6/edgeimpulse_api/models/model_result.py
+-rw-r--r--   0        0        0     5046 2023-05-18 14:36:25.435113 edgeimpulse_api-1.23.6/edgeimpulse_api/models/model_variant_stats.py
+-rw-r--r--   0        0        0     2128 2023-05-18 14:36:25.095883 edgeimpulse_api-1.23.6/edgeimpulse_api/models/move_raw_data_request.py
+-rw-r--r--   0        0        0     2687 2023-05-18 14:36:25.419523 edgeimpulse_api-1.23.6/edgeimpulse_api/models/note.py
+-rw-r--r--   0        0        0     2221 2023-05-18 14:36:25.099699 edgeimpulse_api-1.23.6/edgeimpulse_api/models/object_detection_auto_label_request.py
+-rw-r--r--   0        0        0     2994 2023-05-18 14:36:25.069830 edgeimpulse_api-1.23.6/edgeimpulse_api/models/object_detection_auto_label_response.py
+-rw-r--r--   0        0        0     2705 2023-05-18 14:36:24.693547 edgeimpulse_api-1.23.6/edgeimpulse_api/models/object_detection_auto_label_response_all_of.py
+-rw-r--r--   0        0        0     2275 2023-05-18 14:36:25.445363 edgeimpulse_api-1.23.6/edgeimpulse_api/models/object_detection_auto_label_response_all_of_results.py
+-rw-r--r--   0        0        0     2368 2023-05-18 14:36:25.264863 edgeimpulse_api-1.23.6/edgeimpulse_api/models/object_detection_label_queue_count_response.py
+-rw-r--r--   0        0        0     2051 2023-05-18 14:36:24.796361 edgeimpulse_api-1.23.6/edgeimpulse_api/models/object_detection_label_queue_count_response_all_of.py
+-rw-r--r--   0        0        0     2887 2023-05-18 14:36:25.483708 edgeimpulse_api-1.23.6/edgeimpulse_api/models/object_detection_label_queue_response.py
+-rw-r--r--   0        0        0     2580 2023-05-18 14:36:25.301611 edgeimpulse_api-1.23.6/edgeimpulse_api/models/object_detection_label_queue_response_all_of.py
+-rw-r--r--   0        0        0      621 2023-05-18 14:36:25.352825 edgeimpulse_api-1.23.6/edgeimpulse_api/models/object_detection_last_layer.py
+-rw-r--r--   0        0        0     6418 2023-05-18 14:36:25.197409 edgeimpulse_api-1.23.6/edgeimpulse_api/models/optimize_config.py
+-rw-r--r--   0        0        0     6871 2023-05-18 14:36:25.479494 edgeimpulse_api-1.23.6/edgeimpulse_api/models/optimize_config_response.py
+-rw-r--r--   0        0        0     1920 2023-05-18 14:36:25.144920 edgeimpulse_api-1.23.6/edgeimpulse_api/models/optimize_config_response_all_of.py
+-rw-r--r--   0        0        0     2067 2023-05-18 14:36:25.140231 edgeimpulse_api-1.23.6/edgeimpulse_api/models/optimize_config_target_device.py
+-rw-r--r--   0        0        0     2271 2023-05-18 14:36:24.553823 edgeimpulse_api-1.23.6/edgeimpulse_api/models/optimize_dsp_parameters_response.py
+-rw-r--r--   0        0        0     1964 2023-05-18 14:36:25.403686 edgeimpulse_api-1.23.6/edgeimpulse_api/models/optimize_dsp_parameters_response_all_of.py
+-rw-r--r--   0        0        0     2756 2023-05-18 14:36:25.402541 edgeimpulse_api-1.23.6/edgeimpulse_api/models/optimize_space_response.py
+-rw-r--r--   0        0        0     2456 2023-05-18 14:36:24.528518 edgeimpulse_api-1.23.6/edgeimpulse_api/models/optimize_space_response_all_of.py
+-rw-r--r--   0        0        0     4897 2023-05-18 14:36:24.724668 edgeimpulse_api-1.23.6/edgeimpulse_api/models/optimize_state_response.py
+-rw-r--r--   0        0        0     4618 2023-05-18 14:36:24.901641 edgeimpulse_api-1.23.6/edgeimpulse_api/models/optimize_state_response_all_of.py
+-rw-r--r--   0        0        0     3419 2023-05-18 14:36:24.757740 edgeimpulse_api-1.23.6/edgeimpulse_api/models/optimize_state_response_all_of_status.py
+-rw-r--r--   0        0        0     2366 2023-05-18 14:36:25.333395 edgeimpulse_api-1.23.6/edgeimpulse_api/models/optimize_state_response_all_of_workers.py
+-rw-r--r--   0        0        0     2760 2023-05-18 14:36:25.247495 edgeimpulse_api-1.23.6/edgeimpulse_api/models/optimize_transfer_learning_models_response.py
+-rw-r--r--   0        0        0     2463 2023-05-18 14:36:25.468822 edgeimpulse_api-1.23.6/edgeimpulse_api/models/optimize_transfer_learning_models_response_all_of.py
+-rw-r--r--   0        0        0     4682 2023-05-18 14:36:24.948998 edgeimpulse_api-1.23.6/edgeimpulse_api/models/optimize_transfer_learning_models_response_all_of_models.py
+-rw-r--r--   0        0        0     3774 2023-05-18 14:36:24.778736 edgeimpulse_api-1.23.6/edgeimpulse_api/models/organization.py
+-rw-r--r--   0        0        0     2359 2023-05-18 14:36:25.236996 edgeimpulse_api-1.23.6/edgeimpulse_api/models/organization_add_data_folder_request.py
+-rw-r--r--   0        0        0     2498 2023-05-18 14:36:25.505988 edgeimpulse_api-1.23.6/edgeimpulse_api/models/organization_add_data_folder_response.py
+-rw-r--r--   0        0        0     2209 2023-05-18 14:36:25.467754 edgeimpulse_api-1.23.6/edgeimpulse_api/models/organization_add_data_folder_response_all_of.py
+-rw-r--r--   0        0        0     2549 2023-05-18 14:36:24.771057 edgeimpulse_api-1.23.6/edgeimpulse_api/models/organization_add_dataset_request.py
+-rw-r--r--   0        0        0     2460 2023-05-18 14:36:25.217409 edgeimpulse_api-1.23.6/edgeimpulse_api/models/organization_add_dataset_request_bucket.py
+-rw-r--r--   0        0        0     8598 2023-05-18 14:36:25.275408 edgeimpulse_api-1.23.6/edgeimpulse_api/models/organization_create_project.py
+-rw-r--r--   0        0        0     5176 2023-05-18 14:36:25.013093 edgeimpulse_api-1.23.6/edgeimpulse_api/models/organization_create_project_request.py
+-rw-r--r--   0        0        0     2543 2023-05-18 14:36:24.638998 edgeimpulse_api-1.23.6/edgeimpulse_api/models/organization_create_project_response.py
+-rw-r--r--   0        0        0     2237 2023-05-18 14:36:25.480631 edgeimpulse_api-1.23.6/edgeimpulse_api/models/organization_create_project_response_all_of.py
+-rw-r--r--   0        0        0     2704 2023-05-18 14:36:25.507115 edgeimpulse_api-1.23.6/edgeimpulse_api/models/organization_create_project_status_response.py
+-rw-r--r--   0        0        0     2407 2023-05-18 14:36:25.001013 edgeimpulse_api-1.23.6/edgeimpulse_api/models/organization_create_project_status_response_all_of.py
+-rw-r--r--   0        0        0     2501 2023-05-18 14:36:24.759499 edgeimpulse_api-1.23.6/edgeimpulse_api/models/organization_create_project_transformation_summary.py
+-rw-r--r--   0        0        0     9325 2023-05-18 14:36:25.050443 edgeimpulse_api-1.23.6/edgeimpulse_api/models/organization_create_project_with_files.py
+-rw-r--r--   0        0        0     2558 2023-05-18 14:36:25.209477 edgeimpulse_api-1.23.6/edgeimpulse_api/models/organization_create_project_with_files_all_of.py
+-rw-r--r--   0        0        0     3034 2023-05-18 14:36:25.474371 edgeimpulse_api-1.23.6/edgeimpulse_api/models/organization_create_project_with_files_all_of_files.py
+-rw-r--r--   0        0        0     3476 2023-05-18 14:36:24.806922 edgeimpulse_api-1.23.6/edgeimpulse_api/models/organization_data_item.py
+-rw-r--r--   0        0        0     2103 2023-05-18 14:36:24.791617 edgeimpulse_api-1.23.6/edgeimpulse_api/models/organization_data_item_files_inner.py
+-rw-r--r--   0        0        0     3529 2023-05-18 14:36:25.276347 edgeimpulse_api-1.23.6/edgeimpulse_api/models/organization_dataset.py
+-rw-r--r--   0        0        0     2767 2023-05-18 14:36:24.782577 edgeimpulse_api-1.23.6/edgeimpulse_api/models/organization_dataset_bucket.py
+-rw-r--r--   0        0        0     4689 2023-05-18 14:36:24.573901 edgeimpulse_api-1.23.6/edgeimpulse_api/models/organization_deploy_block.py
+-rw-r--r--   0        0        0     3646 2023-05-18 14:36:25.195949 edgeimpulse_api-1.23.6/edgeimpulse_api/models/organization_dsp_block.py
+-rw-r--r--   0        0        0     3037 2023-05-18 14:36:25.270726 edgeimpulse_api-1.23.6/edgeimpulse_api/models/organization_get_create_projects_response.py
+-rw-r--r--   0        0        0     2737 2023-05-18 14:36:24.836872 edgeimpulse_api-1.23.6/edgeimpulse_api/models/organization_get_create_projects_response_all_of.py
+-rw-r--r--   0        0        0     5707 2023-05-18 14:36:25.392217 edgeimpulse_api-1.23.6/edgeimpulse_api/models/organization_get_create_projects_response_all_of_jobs.py
+-rw-r--r--   0        0        0     5938 2023-05-18 14:36:25.060994 edgeimpulse_api-1.23.6/edgeimpulse_api/models/organization_info_response.py
+-rw-r--r--   0        0        0     5648 2023-05-18 14:36:25.118181 edgeimpulse_api-1.23.6/edgeimpulse_api/models/organization_info_response_all_of.py
+-rw-r--r--   0        0        0     2458 2023-05-18 14:36:24.580886 edgeimpulse_api-1.23.6/edgeimpulse_api/models/organization_info_response_all_of_default_compute_limits.py
+-rw-r--r--   0        0        0     2600 2023-05-18 14:36:25.164521 edgeimpulse_api-1.23.6/edgeimpulse_api/models/organization_info_response_all_of_entitlement_limits.py
+-rw-r--r--   0        0        0     2639 2023-05-18 14:36:25.031986 edgeimpulse_api-1.23.6/edgeimpulse_api/models/organization_metrics_response.py
+-rw-r--r--   0        0        0     2315 2023-05-18 14:36:24.656525 edgeimpulse_api-1.23.6/edgeimpulse_api/models/organization_metrics_response_all_of.py
+-rw-r--r--   0        0        0     3491 2023-05-18 14:36:24.670350 edgeimpulse_api-1.23.6/edgeimpulse_api/models/organization_metrics_response_all_of_metrics.py
+-rw-r--r--   0        0        0     6114 2023-05-18 14:36:25.248599 edgeimpulse_api-1.23.6/edgeimpulse_api/models/organization_pipeline.py
+-rw-r--r--   0        0        0     2595 2023-05-18 14:36:25.104841 edgeimpulse_api-1.23.6/edgeimpulse_api/models/organization_pipeline_feeding_into_dataset.py
+-rw-r--r--   0        0        0     2275 2023-05-18 14:36:25.420945 edgeimpulse_api-1.23.6/edgeimpulse_api/models/organization_pipeline_feeding_into_project.py
+-rw-r--r--   0        0        0     2314 2023-05-18 14:36:24.872777 edgeimpulse_api-1.23.6/edgeimpulse_api/models/organization_pipeline_item_count.py
+-rw-r--r--   0        0        0     4109 2023-05-18 14:36:25.037576 edgeimpulse_api-1.23.6/edgeimpulse_api/models/organization_pipeline_run.py
+-rw-r--r--   0        0        0     5213 2023-05-18 14:36:24.780789 edgeimpulse_api-1.23.6/edgeimpulse_api/models/organization_pipeline_run_step.py
+-rw-r--r--   0        0        0     4813 2023-05-18 14:36:25.290151 edgeimpulse_api-1.23.6/edgeimpulse_api/models/organization_pipeline_step.py
+-rw-r--r--   0        0        0     2351 2023-05-18 14:36:24.766886 edgeimpulse_api-1.23.6/edgeimpulse_api/models/organization_projects_data_batch_disable_response.py
+-rw-r--r--   0        0        0     2344 2023-05-18 14:36:25.394020 edgeimpulse_api-1.23.6/edgeimpulse_api/models/organization_projects_data_batch_enable_response.py
+-rw-r--r--   0        0        0     2037 2023-05-18 14:36:25.083760 edgeimpulse_api-1.23.6/edgeimpulse_api/models/organization_projects_data_batch_request.py
+-rw-r--r--   0        0        0     4414 2023-05-18 14:36:24.828118 edgeimpulse_api-1.23.6/edgeimpulse_api/models/organization_transfer_learning_block.py
+-rw-r--r--   0        0        0      611 2023-05-18 14:36:25.315683 edgeimpulse_api-1.23.6/edgeimpulse_api/models/organization_transfer_learning_operates_on.py
+-rw-r--r--   0        0        0     5168 2023-05-18 14:36:25.131440 edgeimpulse_api-1.23.6/edgeimpulse_api/models/organization_transformation_block.py
+-rw-r--r--   0        0        0     3889 2023-05-18 14:36:24.514636 edgeimpulse_api-1.23.6/edgeimpulse_api/models/organization_update_pipeline_body.py
+-rw-r--r--   0        0        0     3609 2023-05-18 14:36:25.425777 edgeimpulse_api-1.23.6/edgeimpulse_api/models/organization_user.py
+-rw-r--r--   0        0        0     2104 2023-05-18 14:36:24.564426 edgeimpulse_api-1.23.6/edgeimpulse_api/models/performance_calibration_detection.py
+-rw-r--r--   0        0        0     3434 2023-05-18 14:36:24.975645 edgeimpulse_api-1.23.6/edgeimpulse_api/models/performance_calibration_false_positive.py
+-rw-r--r--   0        0        0     3770 2023-05-18 14:36:24.961612 edgeimpulse_api-1.23.6/edgeimpulse_api/models/performance_calibration_ground_truth.py
+-rw-r--r--   0        0        0     2477 2023-05-18 14:36:24.571001 edgeimpulse_api-1.23.6/edgeimpulse_api/models/performance_calibration_ground_truth_samples_inner.py
+-rw-r--r--   0        0        0     4880 2023-05-18 14:36:24.557037 edgeimpulse_api-1.23.6/edgeimpulse_api/models/performance_calibration_parameter_set.py
+-rw-r--r--   0        0        0     2255 2023-05-18 14:36:25.198633 edgeimpulse_api-1.23.6/edgeimpulse_api/models/performance_calibration_parameter_set_aggregate_stats.py
+-rw-r--r--   0        0        0     4092 2023-05-18 14:36:24.637476 edgeimpulse_api-1.23.6/edgeimpulse_api/models/performance_calibration_parameter_set_stats_inner.py
+-rw-r--r--   0        0        0     3007 2023-05-18 14:36:25.486591 edgeimpulse_api-1.23.6/edgeimpulse_api/models/performance_calibration_parameters.py
+-rw-r--r--   0        0        0     2585 2023-05-18 14:36:24.877503 edgeimpulse_api-1.23.6/edgeimpulse_api/models/performance_calibration_parameters_standard.py
+-rw-r--r--   0        0        0     2250 2023-05-18 14:36:25.055923 edgeimpulse_api-1.23.6/edgeimpulse_api/models/performance_calibration_raw_detection.py
+-rw-r--r--   0        0        0     2366 2023-05-18 14:36:25.283864 edgeimpulse_api-1.23.6/edgeimpulse_api/models/performance_calibration_save_parameter_set_request.py
+-rw-r--r--   0        0        0     2412 2023-05-18 14:36:25.212607 edgeimpulse_api-1.23.6/edgeimpulse_api/models/performance_calibration_upload_labeled_audio_response.py
+-rw-r--r--   0        0        0     2106 2023-05-18 14:36:24.703305 edgeimpulse_api-1.23.6/edgeimpulse_api/models/performance_calibration_upload_labeled_audio_response_all_of.py
+-rw-r--r--   0        0        0     1250 2023-05-18 14:36:24.749163 edgeimpulse_api-1.23.6/edgeimpulse_api/models/permission.py
+-rw-r--r--   0        0        0     2211 2023-05-18 14:36:25.274264 edgeimpulse_api-1.23.6/edgeimpulse_api/models/portal_file.py
+-rw-r--r--   0        0        0     2413 2023-05-18 14:36:24.808392 edgeimpulse_api-1.23.6/edgeimpulse_api/models/portal_info_response.py
+-rw-r--r--   0        0        0     2666 2023-05-18 14:36:25.029060 edgeimpulse_api-1.23.6/edgeimpulse_api/models/pretrained_model_tensor.py
+-rw-r--r--   0        0        0     2955 2023-05-18 14:36:25.187405 edgeimpulse_api-1.23.6/edgeimpulse_api/models/profile_model_info.py
+-rw-r--r--   0        0        0     2640 2023-05-18 14:36:24.999440 edgeimpulse_api-1.23.6/edgeimpulse_api/models/profile_model_info_memory.py
+-rw-r--r--   0        0        0     1918 2023-05-18 14:36:25.142863 edgeimpulse_api-1.23.6/edgeimpulse_api/models/profile_model_info_memory_eon.py
+-rw-r--r--   0        0        0     2065 2023-05-18 14:36:24.971735 edgeimpulse_api-1.23.6/edgeimpulse_api/models/profile_model_info_memory_tflite.py
+-rw-r--r--   0        0        0     4335 2023-05-18 14:36:25.341710 edgeimpulse_api-1.23.6/edgeimpulse_api/models/profile_model_table.py
+-rw-r--r--   0        0        0     2780 2023-05-18 14:36:24.869648 edgeimpulse_api-1.23.6/edgeimpulse_api/models/profile_model_table_mcu.py
+-rw-r--r--   0        0        0     2565 2023-05-18 14:36:25.027899 edgeimpulse_api-1.23.6/edgeimpulse_api/models/profile_model_table_mcu_memory.py
+-rw-r--r--   0        0        0     2250 2023-05-18 14:36:24.916958 edgeimpulse_api-1.23.6/edgeimpulse_api/models/profile_model_table_mpu.py
+-rw-r--r--   0        0        0     2201 2023-05-18 14:36:25.317295 edgeimpulse_api-1.23.6/edgeimpulse_api/models/profile_tf_lite_request.py
+-rw-r--r--   0        0        0     3292 2023-05-18 14:36:25.122203 edgeimpulse_api-1.23.6/edgeimpulse_api/models/profile_tf_lite_response.py
+-rw-r--r--   0        0        0     6139 2023-05-18 14:36:25.458065 edgeimpulse_api-1.23.6/edgeimpulse_api/models/project.py
+-rw-r--r--   0        0        0     3506 2023-05-18 14:36:24.832142 edgeimpulse_api-1.23.6/edgeimpulse_api/models/project_collaborator.py
+-rw-r--r--   0        0        0     1895 2023-05-18 14:36:25.216461 edgeimpulse_api-1.23.6/edgeimpulse_api/models/project_collaborator_all_of.py
+-rw-r--r--   0        0        0     2416 2023-05-18 14:36:25.358433 edgeimpulse_api-1.23.6/edgeimpulse_api/models/project_data_axes_summary_response.py
+-rw-r--r--   0        0        0     2116 2023-05-18 14:36:24.563155 edgeimpulse_api-1.23.6/edgeimpulse_api/models/project_data_axes_summary_response_all_of.py
+-rw-r--r--   0        0        0     2281 2023-05-18 14:36:25.002164 edgeimpulse_api-1.23.6/edgeimpulse_api/models/project_data_interval_response.py
+-rw-r--r--   0        0        0     1964 2023-05-18 14:36:24.754412 edgeimpulse_api-1.23.6/edgeimpulse_api/models/project_data_interval_response_all_of.py
+-rw-r--r--   0        0        0     2235 2023-05-18 14:36:24.616997 edgeimpulse_api-1.23.6/edgeimpulse_api/models/project_data_summary.py
+-rw-r--r--   0        0        0     6500 2023-05-18 14:36:25.305224 edgeimpulse_api-1.23.6/edgeimpulse_api/models/project_deployment_target.py
+-rw-r--r--   0        0        0     2706 2023-05-18 14:36:25.429717 edgeimpulse_api-1.23.6/edgeimpulse_api/models/project_deployment_target_all_of.py
+-rw-r--r--   0        0        0     2780 2023-05-18 14:36:25.080401 edgeimpulse_api-1.23.6/edgeimpulse_api/models/project_deployment_targets_response.py
+-rw-r--r--   0        0        0     2473 2023-05-18 14:36:24.583909 edgeimpulse_api-1.23.6/edgeimpulse_api/models/project_deployment_targets_response_all_of.py
+-rw-r--r--   0        0        0     2680 2023-05-18 14:36:24.603161 edgeimpulse_api-1.23.6/edgeimpulse_api/models/project_downloads_response.py
+-rw-r--r--   0        0        0     2373 2023-05-18 14:36:24.959791 edgeimpulse_api-1.23.6/edgeimpulse_api/models/project_downloads_response_all_of.py
+-rw-r--r--   0        0        0    13206 2023-05-18 14:36:25.465591 edgeimpulse_api-1.23.6/edgeimpulse_api/models/project_info_response.py
+-rw-r--r--   0        0        0    12939 2023-05-18 14:36:25.477563 edgeimpulse_api-1.23.6/edgeimpulse_api/models/project_info_response_all_of.py
+-rw-r--r--   0        0        0     3130 2023-05-18 14:36:24.523477 edgeimpulse_api-1.23.6/edgeimpulse_api/models/project_info_response_all_of_acquisition_settings.py
+-rw-r--r--   0        0        0     2723 2023-05-18 14:36:25.424831 edgeimpulse_api-1.23.6/edgeimpulse_api/models/project_info_response_all_of_compute_time.py
+-rw-r--r--   0        0        0     2997 2023-05-18 14:36:25.078930 edgeimpulse_api-1.23.6/edgeimpulse_api/models/project_info_response_all_of_data_summary_per_category.py
+-rw-r--r--   0        0        0     2808 2023-05-18 14:36:24.740729 edgeimpulse_api-1.23.6/edgeimpulse_api/models/project_info_response_all_of_deploy_settings.py
+-rw-r--r--   0        0        0     2339 2023-05-18 14:36:25.337303 edgeimpulse_api-1.23.6/edgeimpulse_api/models/project_info_response_all_of_experiments.py
+-rw-r--r--   0        0        0     2285 2023-05-18 14:36:25.380627 edgeimpulse_api-1.23.6/edgeimpulse_api/models/project_info_response_all_of_impulse.py
+-rw-r--r--   0        0        0     2726 2023-05-18 14:36:25.076181 edgeimpulse_api-1.23.6/edgeimpulse_api/models/project_info_response_all_of_performance.py
+-rw-r--r--   0        0        0     1977 2023-05-18 14:36:25.415418 edgeimpulse_api-1.23.6/edgeimpulse_api/models/project_info_response_all_of_readme.py
+-rw-r--r--   0        0        0     2225 2023-05-18 14:36:25.179909 edgeimpulse_api-1.23.6/edgeimpulse_api/models/project_info_response_all_of_show_getting_started_wizard.py
+-rw-r--r--   0        0        0     2735 2023-05-18 14:36:24.719613 edgeimpulse_api-1.23.6/edgeimpulse_api/models/project_info_response_all_of_urls.py
+-rw-r--r--   0        0        0     2478 2023-05-18 14:36:24.662257 edgeimpulse_api-1.23.6/edgeimpulse_api/models/project_info_summary_response.py
+-rw-r--r--   0        0        0     2172 2023-05-18 14:36:24.805213 edgeimpulse_api-1.23.6/edgeimpulse_api/models/project_info_summary_response_all_of.py
+-rw-r--r--   0        0        0     3554 2023-05-18 14:36:24.570119 edgeimpulse_api-1.23.6/edgeimpulse_api/models/project_private_data.py
+-rw-r--r--   0        0        0     4396 2023-05-18 14:36:24.568274 edgeimpulse_api-1.23.6/edgeimpulse_api/models/project_public_data.py
+-rw-r--r--   0        0        0     1928 2023-05-18 14:36:25.067619 edgeimpulse_api-1.23.6/edgeimpulse_api/models/project_public_data_readme.py
+-rw-r--r--   0        0        0     2404 2023-05-18 14:36:25.417930 edgeimpulse_api-1.23.6/edgeimpulse_api/models/project_sample_metadata.py
+-rw-r--r--   0        0        0     2670 2023-05-18 14:36:24.745576 edgeimpulse_api-1.23.6/edgeimpulse_api/models/project_training_data_summary_response.py
+-rw-r--r--   0        0        0     2353 2023-05-18 14:36:25.401095 edgeimpulse_api-1.23.6/edgeimpulse_api/models/project_training_data_summary_response_all_of.py
+-rw-r--r--   0        0        0     2316 2023-05-18 14:36:24.878503 edgeimpulse_api-1.23.6/edgeimpulse_api/models/project_version_request.py
+-rw-r--r--   0        0        0     2664 2023-05-18 14:36:24.663732 edgeimpulse_api-1.23.6/edgeimpulse_api/models/raw_sample_data.py
+-rw-r--r--   0        0        0     3440 2023-05-18 14:36:25.456890 edgeimpulse_api-1.23.6/edgeimpulse_api/models/raw_sample_payload.py
+-rw-r--r--   0        0        0     2537 2023-05-18 14:36:25.491577 edgeimpulse_api-1.23.6/edgeimpulse_api/models/rebalance_dataset_response.py
+-rw-r--r--   0        0        0     1984 2023-05-18 14:36:25.010397 edgeimpulse_api-1.23.6/edgeimpulse_api/models/remove_collaborator_request.py
+-rw-r--r--   0        0        0     1805 2023-05-18 14:36:25.199898 edgeimpulse_api-1.23.6/edgeimpulse_api/models/remove_member_request.py
+-rw-r--r--   0        0        0     1867 2023-05-18 14:36:24.923136 edgeimpulse_api-1.23.6/edgeimpulse_api/models/rename_device_request.py
+-rw-r--r--   0        0        0     2081 2023-05-18 14:36:24.856901 edgeimpulse_api-1.23.6/edgeimpulse_api/models/rename_portal_file_request.py
+-rw-r--r--   0        0        0     1867 2023-05-18 14:36:25.451609 edgeimpulse_api-1.23.6/edgeimpulse_api/models/rename_sample_request.py
+-rw-r--r--   0        0        0     1873 2023-05-18 14:36:24.605040 edgeimpulse_api-1.23.6/edgeimpulse_api/models/request_reset_password_request.py
+-rw-r--r--   0        0        0     2031 2023-05-18 14:36:25.461004 edgeimpulse_api-1.23.6/edgeimpulse_api/models/reset_password_request.py
+-rw-r--r--   0        0        0     1985 2023-05-18 14:36:25.060023 edgeimpulse_api-1.23.6/edgeimpulse_api/models/restore_project_from_public_request.py
+-rw-r--r--   0        0        0     2265 2023-05-18 14:36:25.411509 edgeimpulse_api-1.23.6/edgeimpulse_api/models/restore_project_request.py
+-rw-r--r--   0        0        0     2669 2023-05-18 14:36:25.441090 edgeimpulse_api-1.23.6/edgeimpulse_api/models/run_organization_pipeline_response.py
+-rw-r--r--   0        0        0     2352 2023-05-18 14:36:24.582370 edgeimpulse_api-1.23.6/edgeimpulse_api/models/run_organization_pipeline_response_all_of.py
+-rw-r--r--   0        0        0     9637 2023-05-18 14:36:25.240264 edgeimpulse_api-1.23.6/edgeimpulse_api/models/sample.py
+-rw-r--r--   0        0        0     2443 2023-05-18 14:36:24.677345 edgeimpulse_api-1.23.6/edgeimpulse_api/models/sample_bounding_boxes_request.py
+-rw-r--r--   0        0        0     2000 2023-05-18 14:36:24.631850 edgeimpulse_api-1.23.6/edgeimpulse_api/models/sample_metadata.py
+-rw-r--r--   0        0        0     2756 2023-05-18 14:36:24.649121 edgeimpulse_api-1.23.6/edgeimpulse_api/models/save_pretrained_model_request.py
+-rw-r--r--   0        0        0     3327 2023-05-18 14:36:24.964972 edgeimpulse_api-1.23.6/edgeimpulse_api/models/score_trial_response.py
+-rw-r--r--   0        0        0     3003 2023-05-18 14:36:25.504414 edgeimpulse_api-1.23.6/edgeimpulse_api/models/score_trial_response_all_of.py
+-rw-r--r--   0        0        0     2240 2023-05-18 14:36:24.914043 edgeimpulse_api-1.23.6/edgeimpulse_api/models/score_trial_response_all_of_latency.py
+-rw-r--r--   0        0        0     1914 2023-05-18 14:36:25.386294 edgeimpulse_api-1.23.6/edgeimpulse_api/models/score_trial_response_all_of_ram.py
+-rw-r--r--   0        0        0     2405 2023-05-18 14:36:24.764689 edgeimpulse_api-1.23.6/edgeimpulse_api/models/segment_sample_request.py
+-rw-r--r--   0        0        0     2055 2023-05-18 14:36:25.472981 edgeimpulse_api-1.23.6/edgeimpulse_api/models/segment_sample_request_segments_inner.py
+-rw-r--r--   0        0        0     3364 2023-05-18 14:36:25.151455 edgeimpulse_api-1.23.6/edgeimpulse_api/models/send_user_feedback_request.py
+-rw-r--r--   0        0        0     1981 2023-05-18 14:36:24.640375 edgeimpulse_api-1.23.6/edgeimpulse_api/models/sensor.py
+-rw-r--r--   0        0        0     2142 2023-05-18 14:36:25.355672 edgeimpulse_api-1.23.6/edgeimpulse_api/models/set_anomaly_parameter_request.py
+-rw-r--r--   0        0        0     7742 2023-05-18 14:36:24.682030 edgeimpulse_api-1.23.6/edgeimpulse_api/models/set_keras_parameter_request.py
+-rw-r--r--   0        0        0     1893 2023-05-18 14:36:25.452959 edgeimpulse_api-1.23.6/edgeimpulse_api/models/set_member_datasets_request.py
+-rw-r--r--   0        0        0     2049 2023-05-18 14:36:25.291908 edgeimpulse_api-1.23.6/edgeimpulse_api/models/set_member_role_request.py
+-rw-r--r--   0        0        0     2219 2023-05-18 14:36:25.347142 edgeimpulse_api-1.23.6/edgeimpulse_api/models/set_optimize_space_request.py
+-rw-r--r--   0        0        0     2254 2023-05-18 14:36:25.361369 edgeimpulse_api-1.23.6/edgeimpulse_api/models/set_optimize_space_request_all_of.py
+-rw-r--r--   0        0        0     1923 2023-05-18 14:36:25.501181 edgeimpulse_api-1.23.6/edgeimpulse_api/models/set_organization_data_dataset_request.py
+-rw-r--r--   0        0        0     1974 2023-05-18 14:36:24.863733 edgeimpulse_api-1.23.6/edgeimpulse_api/models/set_project_compute_time_request.py
+-rw-r--r--   0        0        0     2011 2023-05-18 14:36:25.074538 edgeimpulse_api-1.23.6/edgeimpulse_api/models/set_project_dsp_file_size_request.py
+-rw-r--r--   0        0        0     1919 2023-05-18 14:36:24.698854 edgeimpulse_api-1.23.6/edgeimpulse_api/models/set_sample_metadata_request.py
+-rw-r--r--   0        0        0     1915 2023-05-18 14:36:25.051525 edgeimpulse_api-1.23.6/edgeimpulse_api/models/set_syntiant_posterior_request.py
+-rw-r--r--   0        0        0     2140 2023-05-18 14:36:24.911232 edgeimpulse_api-1.23.6/edgeimpulse_api/models/set_user_password_request.py
+-rw-r--r--   0        0        0     2536 2023-05-18 14:36:24.716324 edgeimpulse_api-1.23.6/edgeimpulse_api/models/socket_token_response.py
+-rw-r--r--   0        0        0     2239 2023-05-18 14:36:25.288078 edgeimpulse_api-1.23.6/edgeimpulse_api/models/socket_token_response_all_of.py
+-rw-r--r--   0        0        0     2059 2023-05-18 14:36:24.533882 edgeimpulse_api-1.23.6/edgeimpulse_api/models/socket_token_response_all_of_token.py
+-rw-r--r--   0        0        0     1971 2023-05-18 14:36:24.756842 edgeimpulse_api-1.23.6/edgeimpulse_api/models/split_sample_in_frames_request.py
+-rw-r--r--   0        0        0     2110 2023-05-18 14:36:24.674916 edgeimpulse_api-1.23.6/edgeimpulse_api/models/staff_info.py
+-rw-r--r--   0        0        0     2226 2023-05-18 14:36:25.126487 edgeimpulse_api-1.23.6/edgeimpulse_api/models/start_job_response.py
+-rw-r--r--   0        0        0     1909 2023-05-18 14:36:24.551616 edgeimpulse_api-1.23.6/edgeimpulse_api/models/start_job_response_all_of.py
+-rw-r--r--   0        0        0     2883 2023-05-18 14:36:24.976562 edgeimpulse_api-1.23.6/edgeimpulse_api/models/start_performance_calibration_request.py
+-rw-r--r--   0        0        0     2838 2023-05-18 14:36:25.261966 edgeimpulse_api-1.23.6/edgeimpulse_api/models/start_sampling_request.py
+-rw-r--r--   0        0        0     2189 2023-05-18 14:36:25.225076 edgeimpulse_api-1.23.6/edgeimpulse_api/models/start_sampling_response.py
+-rw-r--r--   0        0        0     1892 2023-05-18 14:36:25.068809 edgeimpulse_api-1.23.6/edgeimpulse_api/models/start_sampling_response_all_of.py
+-rw-r--r--   0        0        0     2492 2023-05-18 14:36:25.065139 edgeimpulse_api-1.23.6/edgeimpulse_api/models/start_training_request_anomaly.py
+-rw-r--r--   0        0        0     1967 2023-05-18 14:36:24.590534 edgeimpulse_api-1.23.6/edgeimpulse_api/models/store_segment_length_request.py
+-rw-r--r--   0        0        0     2644 2023-05-18 14:36:25.350969 edgeimpulse_api-1.23.6/edgeimpulse_api/models/structured_classify_result.py
+-rw-r--r--   0        0        0     2433 2023-05-18 14:36:24.526888 edgeimpulse_api-1.23.6/edgeimpulse_api/models/test_pretrained_model_request.py
+-rw-r--r--   0        0        0     3074 2023-05-18 14:36:25.381868 edgeimpulse_api-1.23.6/edgeimpulse_api/models/test_pretrained_model_response.py
+-rw-r--r--   0        0        0     2784 2023-05-18 14:36:25.194560 edgeimpulse_api-1.23.6/edgeimpulse_api/models/test_pretrained_model_response_all_of.py
+-rw-r--r--   0        0        0     3251 2023-05-18 14:36:24.706750 edgeimpulse_api-1.23.6/edgeimpulse_api/models/theme.py
+-rw-r--r--   0        0        0     2239 2023-05-18 14:36:25.023581 edgeimpulse_api-1.23.6/edgeimpulse_api/models/theme_colors.py
+-rw-r--r--   0        0        0     2764 2023-05-18 14:36:24.867392 edgeimpulse_api-1.23.6/edgeimpulse_api/models/theme_favicon.py
+-rw-r--r--   0        0        0     2721 2023-05-18 14:36:24.921406 edgeimpulse_api-1.23.6/edgeimpulse_api/models/theme_logos.py
+-rw-r--r--   0        0        0     2245 2023-05-18 14:36:24.846519 edgeimpulse_api-1.23.6/edgeimpulse_api/models/third_party_auth.py
+-rw-r--r--   0        0        0     2031 2023-05-18 14:36:24.850360 edgeimpulse_api-1.23.6/edgeimpulse_api/models/track_objects_request.py
+-rw-r--r--   0        0        0     2736 2023-05-18 14:36:25.132875 edgeimpulse_api-1.23.6/edgeimpulse_api/models/track_objects_response.py
+-rw-r--r--   0        0        0     2436 2023-05-18 14:36:24.812969 edgeimpulse_api-1.23.6/edgeimpulse_api/models/track_objects_response_all_of.py
+-rw-r--r--   0        0        0     4610 2023-05-18 14:36:24.779706 edgeimpulse_api-1.23.6/edgeimpulse_api/models/transfer_learning_model.py
+-rw-r--r--   0        0        0     2012 2023-05-18 14:36:24.664776 edgeimpulse_api-1.23.6/edgeimpulse_api/models/transfer_ownership_organization_request.py
+-rw-r--r--   0        0        0     2585 2023-05-18 14:36:25.318490 edgeimpulse_api-1.23.6/edgeimpulse_api/models/transformation_block_additional_mount_point.py
+-rw-r--r--   0        0        0      588 2023-05-18 14:36:25.325251 edgeimpulse_api-1.23.6/edgeimpulse_api/models/transformation_job_status_enum.py
+-rw-r--r--   0        0        0     2578 2023-05-18 14:36:25.167364 edgeimpulse_api-1.23.6/edgeimpulse_api/models/tuner_create_trial_impulse.py
+-rw-r--r--   0        0        0     2570 2023-05-18 14:36:24.552585 edgeimpulse_api-1.23.6/edgeimpulse_api/models/tuner_space_impulse.py
+-rw-r--r--   0        0        0     3661 2023-05-18 14:36:25.423826 edgeimpulse_api-1.23.6/edgeimpulse_api/models/tuner_trial.py
+-rw-r--r--   0        0        0     2304 2023-05-18 14:36:24.868384 edgeimpulse_api-1.23.6/edgeimpulse_api/models/tuner_trial_blocks_inner.py
+-rw-r--r--   0        0        0     2028 2023-05-18 14:36:24.783954 edgeimpulse_api-1.23.6/edgeimpulse_api/models/update_job_request.py
+-rw-r--r--   0        0        0     2281 2023-05-18 14:36:24.820442 edgeimpulse_api-1.23.6/edgeimpulse_api/models/update_organization_add_collaborator_request.py
+-rw-r--r--   0        0        0     2882 2023-05-18 14:36:25.168824 edgeimpulse_api-1.23.6/edgeimpulse_api/models/update_organization_bucket_request.py
+-rw-r--r--   0        0        0     2578 2023-05-18 14:36:25.396973 edgeimpulse_api-1.23.6/edgeimpulse_api/models/update_organization_create_empty_project_request.py
+-rw-r--r--   0        0        0     2428 2023-05-18 14:36:24.525142 edgeimpulse_api-1.23.6/edgeimpulse_api/models/update_organization_create_project_request.py
+-rw-r--r--   0        0        0     2158 2023-05-18 14:36:25.364527 edgeimpulse_api-1.23.6/edgeimpulse_api/models/update_organization_data_item_request.py
+-rw-r--r--   0        0        0     2624 2023-05-18 14:36:25.450218 edgeimpulse_api-1.23.6/edgeimpulse_api/models/update_organization_dataset_request.py
+-rw-r--r--   0        0        0     2881 2023-05-18 14:36:25.466788 edgeimpulse_api-1.23.6/edgeimpulse_api/models/update_organization_dsp_block_request.py
+-rw-r--r--   0        0        0     2724 2023-05-18 14:36:24.853185 edgeimpulse_api-1.23.6/edgeimpulse_api/models/update_organization_portal_response.py
+-rw-r--r--   0        0        0     2445 2023-05-18 14:36:25.192943 edgeimpulse_api-1.23.6/edgeimpulse_api/models/update_organization_portal_response_all_of.py
+-rw-r--r--   0        0        0     2582 2023-05-18 14:36:25.260439 edgeimpulse_api-1.23.6/edgeimpulse_api/models/update_organization_request.py
+-rw-r--r--   0        0        0     3910 2023-05-18 14:36:25.330996 edgeimpulse_api-1.23.6/edgeimpulse_api/models/update_organization_transfer_learning_block_request.py
+-rw-r--r--   0        0        0     4734 2023-05-18 14:36:25.366058 edgeimpulse_api-1.23.6/edgeimpulse_api/models/update_organization_transformation_block_request.py
+-rw-r--r--   0        0        0     7726 2023-05-18 14:36:25.125216 edgeimpulse_api-1.23.6/edgeimpulse_api/models/update_project_request.py
+-rw-r--r--   0        0        0     1877 2023-05-18 14:36:24.904587 edgeimpulse_api-1.23.6/edgeimpulse_api/models/update_project_tags_request.py
+-rw-r--r--   0        0        0     2259 2023-05-18 14:36:24.736564 edgeimpulse_api-1.23.6/edgeimpulse_api/models/update_theme_colors_request.py
+-rw-r--r--   0        0        0     2895 2023-05-18 14:36:24.722930 edgeimpulse_api-1.23.6/edgeimpulse_api/models/update_theme_logos_request.py
+-rw-r--r--   0        0        0     2205 2023-05-18 14:36:25.226680 edgeimpulse_api-1.23.6/edgeimpulse_api/models/update_third_party_auth_request.py
+-rw-r--r--   0        0        0     2277 2023-05-18 14:36:24.685902 edgeimpulse_api-1.23.6/edgeimpulse_api/models/update_user_request.py
+-rw-r--r--   0        0        0     1886 2023-05-18 14:36:24.953079 edgeimpulse_api-1.23.6/edgeimpulse_api/models/update_version_request.py
+-rw-r--r--   0        0        0     2125 2023-05-18 14:36:25.433475 edgeimpulse_api-1.23.6/edgeimpulse_api/models/update_whitelabel_deployment_targets_request.py
+-rw-r--r--   0        0        0     2168 2023-05-18 14:36:25.109082 edgeimpulse_api-1.23.6/edgeimpulse_api/models/upload_asset_response.py
+-rw-r--r--   0        0        0     1882 2023-05-18 14:36:24.841494 edgeimpulse_api-1.23.6/edgeimpulse_api/models/upload_asset_response_all_of.py
+-rw-r--r--   0        0        0     2199 2023-05-18 14:36:24.545682 edgeimpulse_api-1.23.6/edgeimpulse_api/models/upload_readme_image_response.py
+-rw-r--r--   0        0        0     2185 2023-05-18 14:36:25.154267 edgeimpulse_api-1.23.6/edgeimpulse_api/models/upload_user_photo_response.py
+-rw-r--r--   0        0        0     1872 2023-05-18 14:36:25.175935 edgeimpulse_api-1.23.6/edgeimpulse_api/models/upload_user_photo_response_all_of.py
+-rw-r--r--   0        0        0     3291 2023-05-18 14:36:24.592040 edgeimpulse_api-1.23.6/edgeimpulse_api/models/user.py
+-rw-r--r--   0        0        0     1991 2023-05-18 14:36:24.797909 edgeimpulse_api-1.23.6/edgeimpulse_api/models/user_by_third_party_activation_request.py
+-rw-r--r--   0        0        0     2192 2023-05-18 14:36:25.437990 edgeimpulse_api-1.23.6/edgeimpulse_api/models/user_experiment.py
+-rw-r--r--   0        0        0     2709 2023-05-18 14:36:24.951271 edgeimpulse_api-1.23.6/edgeimpulse_api/models/user_organization.py
+-rw-r--r--   0        0        0     1844 2023-05-18 14:36:25.185850 edgeimpulse_api-1.23.6/edgeimpulse_api/models/verify_dsp_block_url_request.py
+-rw-r--r--   0        0        0     2604 2023-05-18 14:36:25.379323 edgeimpulse_api-1.23.6/edgeimpulse_api/models/verify_dsp_block_url_response.py
+-rw-r--r--   0        0        0     2307 2023-05-18 14:36:25.252770 edgeimpulse_api-1.23.6/edgeimpulse_api/models/verify_dsp_block_url_response_all_of.py
+-rw-r--r--   0        0        0     2407 2023-05-18 14:36:25.342757 edgeimpulse_api-1.23.6/edgeimpulse_api/models/verify_dsp_block_url_response_all_of_block.py
+-rw-r--r--   0        0        0     2708 2023-05-18 14:36:24.874140 edgeimpulse_api-1.23.6/edgeimpulse_api/models/verify_organization_bucket_request.py
+-rw-r--r--   0        0        0     2897 2023-05-18 14:36:25.233974 edgeimpulse_api-1.23.6/edgeimpulse_api/models/verify_organization_bucket_response.py
+-rw-r--r--   0        0        0     2597 2023-05-18 14:36:25.439569 edgeimpulse_api-1.23.6/edgeimpulse_api/models/verify_organization_bucket_response_all_of.py
+-rw-r--r--   0        0        0     2187 2023-05-18 14:36:24.502566 edgeimpulse_api-1.23.6/edgeimpulse_api/models/verify_organization_bucket_response_all_of_files.py
+-rw-r--r--   0        0        0     1937 2023-05-18 14:36:25.308673 edgeimpulse_api-1.23.6/edgeimpulse_api/models/verify_reset_password_request.py
+-rw-r--r--   0        0        0     3883 2023-05-18 14:36:25.156355 edgeimpulse_api-1.23.6/edgeimpulse_api/models/whitelabel.py
+-rw-r--r--   0        0        0     2534 2023-05-18 14:36:24.522352 edgeimpulse_api-1.23.6/edgeimpulse_api/models/whitelabel_admin_create_organization_request.py
+-rw-r--r--   0        0        0     2885 2023-05-18 14:36:25.428327 edgeimpulse_api-1.23.6/edgeimpulse_api/models/window_settings_response.py
+-rw-r--r--   0        0        0     2585 2023-05-18 14:36:24.538912 edgeimpulse_api-1.23.6/edgeimpulse_api/models/window_settings_response_all_of.py
+-rw-r--r--   0        0        0     2848 2023-05-18 14:36:24.575217 edgeimpulse_api-1.23.6/edgeimpulse_api/models/window_settings_response_all_of_window_settings.py
+-rw-r--r--   0        0        0    12674 2023-05-18 14:36:17.761615 edgeimpulse_api-1.23.6/edgeimpulse_api/rest.py
+-rw-r--r--   0        0        0      975 2023-05-18 15:26:28.792233 edgeimpulse_api-1.23.6/pyproject.toml
+-rw-r--r--   0        0        0     1413 1970-01-01 00:00:00.000000 edgeimpulse_api-1.23.6/PKG-INFO
```

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/__init__.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
-__version__ = "1.23.0" #DO_NOT_CHANGE_REPLACED_BY_BUILD_SCRIPT
+__version__ = "1.23.6" #DO_NOT_CHANGE_REPLACED_BY_BUILD_SCRIPT
 
 # import apis into sdk package
 from edgeimpulse_api.api.admin_api import AdminApi
 from edgeimpulse_api.api.allows_read_only_api import AllowsReadOnlyApi
 from edgeimpulse_api.api.auth_api import AuthApi
 from edgeimpulse_api.api.cdn_api import CDNApi
 from edgeimpulse_api.api.classify_api import ClassifyApi
@@ -495,27 +495,30 @@
 from edgeimpulse_api.models.optimize_transfer_learning_models_response import OptimizeTransferLearningModelsResponse
 from edgeimpulse_api.models.optimize_transfer_learning_models_response_all_of import OptimizeTransferLearningModelsResponseAllOf
 from edgeimpulse_api.models.optimize_transfer_learning_models_response_all_of_models import OptimizeTransferLearningModelsResponseAllOfModels
 from edgeimpulse_api.models.organization import Organization
 from edgeimpulse_api.models.organization_add_data_folder_request import OrganizationAddDataFolderRequest
 from edgeimpulse_api.models.organization_add_data_folder_response import OrganizationAddDataFolderResponse
 from edgeimpulse_api.models.organization_add_data_folder_response_all_of import OrganizationAddDataFolderResponseAllOf
+from edgeimpulse_api.models.organization_add_dataset_request import OrganizationAddDatasetRequest
+from edgeimpulse_api.models.organization_add_dataset_request_bucket import OrganizationAddDatasetRequestBucket
 from edgeimpulse_api.models.organization_create_project import OrganizationCreateProject
 from edgeimpulse_api.models.organization_create_project_request import OrganizationCreateProjectRequest
 from edgeimpulse_api.models.organization_create_project_response import OrganizationCreateProjectResponse
 from edgeimpulse_api.models.organization_create_project_response_all_of import OrganizationCreateProjectResponseAllOf
 from edgeimpulse_api.models.organization_create_project_status_response import OrganizationCreateProjectStatusResponse
 from edgeimpulse_api.models.organization_create_project_status_response_all_of import OrganizationCreateProjectStatusResponseAllOf
 from edgeimpulse_api.models.organization_create_project_transformation_summary import OrganizationCreateProjectTransformationSummary
 from edgeimpulse_api.models.organization_create_project_with_files import OrganizationCreateProjectWithFiles
 from edgeimpulse_api.models.organization_create_project_with_files_all_of import OrganizationCreateProjectWithFilesAllOf
 from edgeimpulse_api.models.organization_create_project_with_files_all_of_files import OrganizationCreateProjectWithFilesAllOfFiles
 from edgeimpulse_api.models.organization_data_item import OrganizationDataItem
 from edgeimpulse_api.models.organization_data_item_files_inner import OrganizationDataItemFilesInner
 from edgeimpulse_api.models.organization_dataset import OrganizationDataset
+from edgeimpulse_api.models.organization_dataset_bucket import OrganizationDatasetBucket
 from edgeimpulse_api.models.organization_deploy_block import OrganizationDeployBlock
 from edgeimpulse_api.models.organization_dsp_block import OrganizationDspBlock
 from edgeimpulse_api.models.organization_get_create_projects_response import OrganizationGetCreateProjectsResponse
 from edgeimpulse_api.models.organization_get_create_projects_response_all_of import OrganizationGetCreateProjectsResponseAllOf
 from edgeimpulse_api.models.organization_get_create_projects_response_all_of_jobs import OrganizationGetCreateProjectsResponseAllOfJobs
 from edgeimpulse_api.models.organization_info_response import OrganizationInfoResponse
 from edgeimpulse_api.models.organization_info_response_all_of import OrganizationInfoResponseAllOf
```

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/api/__init__.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/api/__init__.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/api/admin_api.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/api/admin_api.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/api/allows_read_only_api.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/api/allows_read_only_api.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/api/auth_api.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/api/auth_api.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/api/cdn_api.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/api/cdn_api.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/api/classify_api.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/api/classify_api.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/api/content_disposition_inline_api.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/api/content_disposition_inline_api.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/api/deployment_api.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/api/deployment_api.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/api/devices_api.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/api/devices_api.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/api/dsp_api.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/api/dsp_api.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/api/export_api.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/api/export_api.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/api/health_api.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/api/health_api.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/api/impulse_api.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/api/impulse_api.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/api/jobs_api.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/api/jobs_api.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/api/learn_api.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/api/learn_api.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/api/login_api.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/api/login_api.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/api/metrics_api.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/api/metrics_api.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/api/optimization_api.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/api/optimization_api.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/api/organization_allow_developer_profile_api.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/api/organization_allow_developer_profile_api.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/api/organization_allow_guest_access_api.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/api/organization_allow_guest_access_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -340,15 +340,15 @@
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
 
     @validate_arguments
     def delete_organization_data_item(self, organization_id : Annotated[StrictInt, Field(..., description="Organization ID")], data_id : Annotated[StrictInt, Field(..., description="Data ID")], **kwargs) -> GenericApiResponse:  # noqa: E501
         """Delete data
 
-        Delete a data item. This does not remove the items from the underlying storage.
+        Delete a data item. This will remove items the items from the underlying storage if your dataset has \"bucketPath\" set.
 
         :param organization_id: Organization ID (required)
         :type organization_id: int
         :param data_id: Data ID (required)
         :type data_id: int
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
@@ -368,15 +368,15 @@
         kwargs['_return_http_data_only'] = True
         return self._delete_organization_data_item_with_http_info(organization_id, data_id, **kwargs)  # noqa: E501
 
     @validate_arguments
     def _delete_organization_data_item_with_http_info(self, organization_id : Annotated[StrictInt, Field(..., description="Organization ID")], data_id : Annotated[StrictInt, Field(..., description="Data ID")], **kwargs):  # noqa: E501
         """Delete data 
 
-        Delete a data item. This does not remove the items from the underlying storage.
+        Delete a data item. This will remove items the items from the underlying storage if your dataset has \"bucketPath\" set.
 
         :param organization_id: Organization ID (required)
         :type organization_id: int
         :param data_id: Data ID (required)
         :type data_id: int
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
```

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/api/organization_blocks_api.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/api/organization_blocks_api.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/api/organization_create_project_api.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/api/organization_create_project_api.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/api/organization_data_api.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/api/organization_data_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,14 +28,15 @@
 from edgeimpulse_api.models.get_organization_dataset_response import GetOrganizationDatasetResponse
 from edgeimpulse_api.models.get_organization_projects_data_count_response import GetOrganizationProjectsDataCountResponse
 from edgeimpulse_api.models.list_organization_buckets_response import ListOrganizationBucketsResponse
 from edgeimpulse_api.models.list_organization_data_response import ListOrganizationDataResponse
 from edgeimpulse_api.models.list_organization_files_response import ListOrganizationFilesResponse
 from edgeimpulse_api.models.list_organization_projects_data_response import ListOrganizationProjectsDataResponse
 from edgeimpulse_api.models.organization_add_data_folder_request import OrganizationAddDataFolderRequest
+from edgeimpulse_api.models.organization_add_dataset_request import OrganizationAddDatasetRequest
 from edgeimpulse_api.models.organization_projects_data_batch_disable_response import OrganizationProjectsDataBatchDisableResponse
 from edgeimpulse_api.models.organization_projects_data_batch_enable_response import OrganizationProjectsDataBatchEnableResponse
 from edgeimpulse_api.models.organization_projects_data_batch_request import OrganizationProjectsDataBatchRequest
 from edgeimpulse_api.models.set_organization_data_dataset_request import SetOrganizationDataDatasetRequest
 from edgeimpulse_api.models.start_job_response import StartJobResponse
 from edgeimpulse_api.models.update_organization_bucket_request import UpdateOrganizationBucketRequest
 from edgeimpulse_api.models.update_organization_data_item_request import UpdateOrganizationDataItemRequest
@@ -692,14 +693,161 @@
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
 
     @validate_arguments
+    def add_organization_dataset(self, organization_id : Annotated[StrictInt, Field(..., description="Organization ID")], organization_add_dataset_request : OrganizationAddDatasetRequest, **kwargs) -> StartJobResponse:  # noqa: E501
+        """Add dataset
+
+        Add a new research dataset
+
+        :param organization_id: Organization ID (required)
+        :type organization_id: int
+        :param organization_add_dataset_request: (required)
+        :type organization_add_dataset_request: OrganizationAddDatasetRequest
+        :param async_req: Whether to execute the request asynchronously.
+        :type async_req: bool, optional
+        :param _preload_content: if False, the urllib3.HTTPResponse object will
+                                 be returned without reading/decoding response
+                                 data. Default is True.
+        :type _preload_content: bool, optional
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :return: Returns the result object.
+                 If the method is called asynchronously,
+                 returns the request thread.
+        :rtype: StartJobResponse
+        """
+        kwargs['_return_http_data_only'] = True
+        return self._add_organization_dataset_with_http_info(organization_id, organization_add_dataset_request, **kwargs)  # noqa: E501
+
+    @validate_arguments
+    def _add_organization_dataset_with_http_info(self, organization_id : Annotated[StrictInt, Field(..., description="Organization ID")], organization_add_dataset_request : OrganizationAddDatasetRequest, **kwargs):  # noqa: E501
+        """Add dataset 
+
+        Add a new research dataset
+
+        :param organization_id: Organization ID (required)
+        :type organization_id: int
+        :param organization_add_dataset_request: (required)
+        :type organization_add_dataset_request: OrganizationAddDatasetRequest
+        :param async_req: Whether to execute the request asynchronously.
+        :type async_req: bool, optional
+        :param _return_http_data_only: response data without head status code
+                                       and headers
+        :type _return_http_data_only: bool, optional
+        :param _preload_content: if False, the urllib3.HTTPResponse object will
+                                 be returned without reading/decoding response
+                                 data. Default is True.
+        :type _preload_content: bool, optional
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :param _request_auth: set to override the auth_settings for an a single
+                              request; this effectively ignores the authentication
+                              in the spec for a single request.
+        :type _request_auth: dict, optional
+        :type _content_type: string, optional: force content-type for the request
+        :return: Returns the result object.
+                 If the method is called asynchronously,
+                 returns the request thread.
+        :rtype: tuple(StartJobResponse, status_code(int), headers(HTTPHeaderDict))
+        """
+
+        _params = locals()
+
+        _all_params = [
+            'organization_id',
+            'organization_add_dataset_request'
+        ]
+        _all_params.extend(
+            [
+                'async_req',
+                '_return_http_data_only',
+                '_preload_content',
+                '_request_timeout',
+                '_request_auth',
+                '_content_type',
+                '_headers'
+            ]
+        )
+
+        # validate the arguments
+        for _key, _val in _params['kwargs'].items():
+            if _key not in _all_params:
+                raise ApiTypeError(
+                    "Got an unexpected keyword argument '%s'"
+                    " to method add_organization_dataset" % _key
+                )
+            _params[_key] = _val
+        del _params['kwargs']
+
+        _collection_formats = {}
+
+        # process the path parameters
+        _path_params = {}
+        if _params['organization_id']:
+            _path_params['organizationId'] = _params['organization_id']
+
+        # process the query parameters
+        _query_params = []
+
+        # process the header parameters
+        _header_params = dict(_params.get('_headers', {}))
+
+        # process the form parameters
+        _form_params = []
+        _files = {}
+
+        # process the body parameter
+        _body_params = None
+        if _params['organization_add_dataset_request']:
+            _body_params = _params['organization_add_dataset_request']
+
+        # set the HTTP header `Accept`
+        _header_params['Accept'] = self.api_client.select_header_accept(
+            ['application/json'])  # noqa: E501
+
+        # set the HTTP header `Content-Type`
+        _content_types_list = _params.get('_content_type',
+            self.api_client.select_header_content_type(
+                ['application/json']))
+        if _content_types_list:
+                _header_params['Content-Type'] = _content_types_list
+
+        # authentication setting
+        _auth_settings = ['ApiKeyAuthentication', 'JWTAuthentication', 'JWTHttpHeaderAuthentication']  # noqa: E501
+
+        _response_types_map = {
+            '200': "StartJobResponse",
+        }
+
+        return self.api_client.call_api(
+            '/api/organizations/{organizationId}/dataset', 'POST',
+            _path_params,
+            _query_params,
+            _header_params,
+            body=_body_params,
+            post_params=_form_params,
+            files=_files,
+            response_types_map=_response_types_map,
+            auth_settings=_auth_settings,
+            async_req=_params.get('async_req'),
+            _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
+            _preload_content=_params.get('_preload_content', True),
+            _request_timeout=_params.get('_request_timeout'),
+            collection_formats=_collection_formats,
+            _request_auth=_params.get('_request_auth'))
+
+    @validate_arguments
     def change_dataset_organization_data_items(self, organization_id : Annotated[StrictInt, Field(..., description="Organization ID")], data_ids : Annotated[StrictStr, Field(..., description="Data IDs as an Array")], set_organization_data_dataset_request : SetOrganizationDataDatasetRequest, dataset : Annotated[Optional[StrictStr], Field(description="Selected dataset")] = None, filter : Annotated[Optional[StrictStr], Field(description="Data filter in SQL WHERE format, where you can reference 'dataset', 'bucket', 'name', 'total_file_count', 'total_file_size', 'created' and any metadata label through 'metadata->' (dots are replaced by underscore).")] = None, **kwargs) -> StartJobResponse:  # noqa: E501
         """Change dataset
 
         Change the dataset for selected data items.
 
         :param organization_id: Organization ID (required)
         :type organization_id: int
@@ -1164,15 +1312,15 @@
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
 
     @validate_arguments
     def delete_organization_data_item(self, organization_id : Annotated[StrictInt, Field(..., description="Organization ID")], data_id : Annotated[StrictInt, Field(..., description="Data ID")], **kwargs) -> GenericApiResponse:  # noqa: E501
         """Delete data
 
-        Delete a data item. This does not remove the items from the underlying storage.
+        Delete a data item. This will remove items the items from the underlying storage if your dataset has \"bucketPath\" set.
 
         :param organization_id: Organization ID (required)
         :type organization_id: int
         :param data_id: Data ID (required)
         :type data_id: int
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
@@ -1192,15 +1340,15 @@
         kwargs['_return_http_data_only'] = True
         return self._delete_organization_data_item_with_http_info(organization_id, data_id, **kwargs)  # noqa: E501
 
     @validate_arguments
     def _delete_organization_data_item_with_http_info(self, organization_id : Annotated[StrictInt, Field(..., description="Organization ID")], data_id : Annotated[StrictInt, Field(..., description="Data ID")], **kwargs):  # noqa: E501
         """Delete data 
 
-        Delete a data item. This does not remove the items from the underlying storage.
+        Delete a data item. This will remove items the items from the underlying storage if your dataset has \"bucketPath\" set.
 
         :param organization_id: Organization ID (required)
         :type organization_id: int
         :param data_id: Data ID (required)
         :type data_id: int
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
@@ -4305,22 +4453,22 @@
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
 
     @validate_arguments
-    def refresh_organization_data(self, organization_id : Annotated[StrictInt, Field(..., description="Organization ID")], dataset : Annotated[Optional[StrictStr], Field(description="Selected dataset")] = None, **kwargs) -> StartJobResponse:  # noqa: E501
+    def refresh_organization_data(self, organization_id : Annotated[StrictInt, Field(..., description="Organization ID")], dataset : Annotated[StrictStr, Field(..., description="Selected dataset")], **kwargs) -> StartJobResponse:  # noqa: E501
         """Refresh data
 
-        Update all data items. HEADs all underlying buckets to retrieve the last file information. Use this API after uploading data directly to S3.
+        Update all data items. HEADs all underlying buckets to retrieve the last file information. Use this API after uploading data directly to S3. If your dataset has bucketId and bucketPath set then this will also remove items that have been removed from S3.
 
         :param organization_id: Organization ID (required)
         :type organization_id: int
-        :param dataset: Selected dataset
+        :param dataset: Selected dataset (required)
         :type dataset: str
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :type _preload_content: bool, optional
@@ -4333,22 +4481,22 @@
                  returns the request thread.
         :rtype: StartJobResponse
         """
         kwargs['_return_http_data_only'] = True
         return self._refresh_organization_data_with_http_info(organization_id, dataset, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def _refresh_organization_data_with_http_info(self, organization_id : Annotated[StrictInt, Field(..., description="Organization ID")], dataset : Annotated[Optional[StrictStr], Field(description="Selected dataset")] = None, **kwargs):  # noqa: E501
+    def _refresh_organization_data_with_http_info(self, organization_id : Annotated[StrictInt, Field(..., description="Organization ID")], dataset : Annotated[StrictStr, Field(..., description="Selected dataset")], **kwargs):  # noqa: E501
         """Refresh data 
 
-        Update all data items. HEADs all underlying buckets to retrieve the last file information. Use this API after uploading data directly to S3.
+        Update all data items. HEADs all underlying buckets to retrieve the last file information. Use this API after uploading data directly to S3. If your dataset has bucketId and bucketPath set then this will also remove items that have been removed from S3.
 
         :param organization_id: Organization ID (required)
         :type organization_id: int
-        :param dataset: Selected dataset
+        :param dataset: Selected dataset (required)
         :type dataset: str
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _return_http_data_only: response data without head status code
                                        and headers
         :type _return_http_data_only: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
```

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/api/organization_jobs_api.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/api/organization_jobs_api.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/api/organization_pipelines_api.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/api/organization_pipelines_api.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/api/organization_portals_api.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/api/organization_portals_api.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/api/organization_requires_admin_api.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/api/organization_requires_admin_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -4490,14 +4490,161 @@
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
 
     @validate_arguments
+    def whitelabel_admin_update_theme_device_logo(self, organization_id : Annotated[StrictInt, Field(..., description="Organization ID")], image : Optional[StrictStr] = None, **kwargs) -> UploadAssetResponse:  # noqa: E501
+        """Update theme device logo
+
+        White label admin only API to update the white label theme device logo.
+
+        :param organization_id: Organization ID (required)
+        :type organization_id: int
+        :param image:
+        :type image: str
+        :param async_req: Whether to execute the request asynchronously.
+        :type async_req: bool, optional
+        :param _preload_content: if False, the urllib3.HTTPResponse object will
+                                 be returned without reading/decoding response
+                                 data. Default is True.
+        :type _preload_content: bool, optional
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :return: Returns the result object.
+                 If the method is called asynchronously,
+                 returns the request thread.
+        :rtype: UploadAssetResponse
+        """
+        kwargs['_return_http_data_only'] = True
+        return self._whitelabel_admin_update_theme_device_logo_with_http_info(organization_id, image, **kwargs)  # noqa: E501
+
+    @validate_arguments
+    def _whitelabel_admin_update_theme_device_logo_with_http_info(self, organization_id : Annotated[StrictInt, Field(..., description="Organization ID")], image : Optional[StrictStr] = None, **kwargs):  # noqa: E501
+        """Update theme device logo 
+
+        White label admin only API to update the white label theme device logo.
+
+        :param organization_id: Organization ID (required)
+        :type organization_id: int
+        :param image:
+        :type image: str
+        :param async_req: Whether to execute the request asynchronously.
+        :type async_req: bool, optional
+        :param _return_http_data_only: response data without head status code
+                                       and headers
+        :type _return_http_data_only: bool, optional
+        :param _preload_content: if False, the urllib3.HTTPResponse object will
+                                 be returned without reading/decoding response
+                                 data. Default is True.
+        :type _preload_content: bool, optional
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :param _request_auth: set to override the auth_settings for an a single
+                              request; this effectively ignores the authentication
+                              in the spec for a single request.
+        :type _request_auth: dict, optional
+        :type _content_type: string, optional: force content-type for the request
+        :return: Returns the result object.
+                 If the method is called asynchronously,
+                 returns the request thread.
+        :rtype: tuple(UploadAssetResponse, status_code(int), headers(HTTPHeaderDict))
+        """
+
+        _params = locals()
+
+        _all_params = [
+            'organization_id',
+            'image'
+        ]
+        _all_params.extend(
+            [
+                'async_req',
+                '_return_http_data_only',
+                '_preload_content',
+                '_request_timeout',
+                '_request_auth',
+                '_content_type',
+                '_headers'
+            ]
+        )
+
+        # validate the arguments
+        for _key, _val in _params['kwargs'].items():
+            if _key not in _all_params:
+                raise ApiTypeError(
+                    "Got an unexpected keyword argument '%s'"
+                    " to method whitelabel_admin_update_theme_device_logo" % _key
+                )
+            _params[_key] = _val
+        del _params['kwargs']
+
+        _collection_formats = {}
+
+        # process the path parameters
+        _path_params = {}
+        if _params['organization_id']:
+            _path_params['organizationId'] = _params['organization_id']
+
+        # process the query parameters
+        _query_params = []
+
+        # process the header parameters
+        _header_params = dict(_params.get('_headers', {}))
+
+        # process the form parameters
+        _form_params = []
+        _files = {}
+        if _params['image']:
+            _files['image'] = _params['image']
+
+        # process the body parameter
+        _body_params = None
+
+        # set the HTTP header `Accept`
+        _header_params['Accept'] = self.api_client.select_header_accept(
+            ['application/json'])  # noqa: E501
+
+        # set the HTTP header `Content-Type`
+        _content_types_list = _params.get('_content_type',
+            self.api_client.select_header_content_type(
+                ['multipart/form-data']))
+        if _content_types_list:
+                _header_params['Content-Type'] = _content_types_list
+
+        # authentication setting
+        _auth_settings = ['ApiKeyAuthentication', 'JWTAuthentication', 'JWTHttpHeaderAuthentication']  # noqa: E501
+
+        _response_types_map = {
+            '200': "UploadAssetResponse",
+        }
+
+        return self.api_client.call_api(
+            '/api/organizations/{organizationId}/whitelabel/theme/deviceLogo', 'POST',
+            _path_params,
+            _query_params,
+            _header_params,
+            body=_body_params,
+            post_params=_form_params,
+            files=_files,
+            response_types_map=_response_types_map,
+            auth_settings=_auth_settings,
+            async_req=_params.get('async_req'),
+            _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
+            _preload_content=_params.get('_preload_content', True),
+            _request_timeout=_params.get('_request_timeout'),
+            collection_formats=_collection_formats,
+            _request_auth=_params.get('_request_auth'))
+
+    @validate_arguments
     def whitelabel_admin_update_theme_favicon(self, organization_id : Annotated[StrictInt, Field(..., description="Organization ID")], image : StrictStr, **kwargs) -> GenericApiResponse:  # noqa: E501
         """Update theme favicon
 
         White label admin only API to update the theme favicon.
 
         :param organization_id: Organization ID (required)
         :type organization_id: int
@@ -4638,15 +4785,15 @@
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
 
     @validate_arguments
     def whitelabel_admin_update_theme_logo(self, organization_id : Annotated[StrictInt, Field(..., description="Organization ID")], image : Optional[StrictStr] = None, **kwargs) -> UploadAssetResponse:  # noqa: E501
-        """Update theme logos
+        """Update theme logo
 
         White label admin only API to update the white label theme logo.
 
         :param organization_id: Organization ID (required)
         :type organization_id: int
         :param image:
         :type image: str
@@ -4666,15 +4813,15 @@
         :rtype: UploadAssetResponse
         """
         kwargs['_return_http_data_only'] = True
         return self._whitelabel_admin_update_theme_logo_with_http_info(organization_id, image, **kwargs)  # noqa: E501
 
     @validate_arguments
     def _whitelabel_admin_update_theme_logo_with_http_info(self, organization_id : Annotated[StrictInt, Field(..., description="Organization ID")], image : Optional[StrictStr] = None, **kwargs):  # noqa: E501
-        """Update theme logos 
+        """Update theme logo 
 
         White label admin only API to update the white label theme logo.
 
         :param organization_id: Organization ID (required)
         :type organization_id: int
         :param image:
         :type image: str
```

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/api/organization_requires_whitelabel_admin_api.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/api/organization_requires_whitelabel_admin_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -2445,14 +2445,161 @@
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
 
     @validate_arguments
+    def whitelabel_admin_update_theme_device_logo(self, organization_id : Annotated[StrictInt, Field(..., description="Organization ID")], image : Optional[StrictStr] = None, **kwargs) -> UploadAssetResponse:  # noqa: E501
+        """Update theme device logo
+
+        White label admin only API to update the white label theme device logo.
+
+        :param organization_id: Organization ID (required)
+        :type organization_id: int
+        :param image:
+        :type image: str
+        :param async_req: Whether to execute the request asynchronously.
+        :type async_req: bool, optional
+        :param _preload_content: if False, the urllib3.HTTPResponse object will
+                                 be returned without reading/decoding response
+                                 data. Default is True.
+        :type _preload_content: bool, optional
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :return: Returns the result object.
+                 If the method is called asynchronously,
+                 returns the request thread.
+        :rtype: UploadAssetResponse
+        """
+        kwargs['_return_http_data_only'] = True
+        return self._whitelabel_admin_update_theme_device_logo_with_http_info(organization_id, image, **kwargs)  # noqa: E501
+
+    @validate_arguments
+    def _whitelabel_admin_update_theme_device_logo_with_http_info(self, organization_id : Annotated[StrictInt, Field(..., description="Organization ID")], image : Optional[StrictStr] = None, **kwargs):  # noqa: E501
+        """Update theme device logo 
+
+        White label admin only API to update the white label theme device logo.
+
+        :param organization_id: Organization ID (required)
+        :type organization_id: int
+        :param image:
+        :type image: str
+        :param async_req: Whether to execute the request asynchronously.
+        :type async_req: bool, optional
+        :param _return_http_data_only: response data without head status code
+                                       and headers
+        :type _return_http_data_only: bool, optional
+        :param _preload_content: if False, the urllib3.HTTPResponse object will
+                                 be returned without reading/decoding response
+                                 data. Default is True.
+        :type _preload_content: bool, optional
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :param _request_auth: set to override the auth_settings for an a single
+                              request; this effectively ignores the authentication
+                              in the spec for a single request.
+        :type _request_auth: dict, optional
+        :type _content_type: string, optional: force content-type for the request
+        :return: Returns the result object.
+                 If the method is called asynchronously,
+                 returns the request thread.
+        :rtype: tuple(UploadAssetResponse, status_code(int), headers(HTTPHeaderDict))
+        """
+
+        _params = locals()
+
+        _all_params = [
+            'organization_id',
+            'image'
+        ]
+        _all_params.extend(
+            [
+                'async_req',
+                '_return_http_data_only',
+                '_preload_content',
+                '_request_timeout',
+                '_request_auth',
+                '_content_type',
+                '_headers'
+            ]
+        )
+
+        # validate the arguments
+        for _key, _val in _params['kwargs'].items():
+            if _key not in _all_params:
+                raise ApiTypeError(
+                    "Got an unexpected keyword argument '%s'"
+                    " to method whitelabel_admin_update_theme_device_logo" % _key
+                )
+            _params[_key] = _val
+        del _params['kwargs']
+
+        _collection_formats = {}
+
+        # process the path parameters
+        _path_params = {}
+        if _params['organization_id']:
+            _path_params['organizationId'] = _params['organization_id']
+
+        # process the query parameters
+        _query_params = []
+
+        # process the header parameters
+        _header_params = dict(_params.get('_headers', {}))
+
+        # process the form parameters
+        _form_params = []
+        _files = {}
+        if _params['image']:
+            _files['image'] = _params['image']
+
+        # process the body parameter
+        _body_params = None
+
+        # set the HTTP header `Accept`
+        _header_params['Accept'] = self.api_client.select_header_accept(
+            ['application/json'])  # noqa: E501
+
+        # set the HTTP header `Content-Type`
+        _content_types_list = _params.get('_content_type',
+            self.api_client.select_header_content_type(
+                ['multipart/form-data']))
+        if _content_types_list:
+                _header_params['Content-Type'] = _content_types_list
+
+        # authentication setting
+        _auth_settings = ['ApiKeyAuthentication', 'JWTAuthentication', 'JWTHttpHeaderAuthentication']  # noqa: E501
+
+        _response_types_map = {
+            '200': "UploadAssetResponse",
+        }
+
+        return self.api_client.call_api(
+            '/api/organizations/{organizationId}/whitelabel/theme/deviceLogo', 'POST',
+            _path_params,
+            _query_params,
+            _header_params,
+            body=_body_params,
+            post_params=_form_params,
+            files=_files,
+            response_types_map=_response_types_map,
+            auth_settings=_auth_settings,
+            async_req=_params.get('async_req'),
+            _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
+            _preload_content=_params.get('_preload_content', True),
+            _request_timeout=_params.get('_request_timeout'),
+            collection_formats=_collection_formats,
+            _request_auth=_params.get('_request_auth'))
+
+    @validate_arguments
     def whitelabel_admin_update_theme_favicon(self, organization_id : Annotated[StrictInt, Field(..., description="Organization ID")], image : StrictStr, **kwargs) -> GenericApiResponse:  # noqa: E501
         """Update theme favicon
 
         White label admin only API to update the theme favicon.
 
         :param organization_id: Organization ID (required)
         :type organization_id: int
@@ -2593,15 +2740,15 @@
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
 
     @validate_arguments
     def whitelabel_admin_update_theme_logo(self, organization_id : Annotated[StrictInt, Field(..., description="Organization ID")], image : Optional[StrictStr] = None, **kwargs) -> UploadAssetResponse:  # noqa: E501
-        """Update theme logos
+        """Update theme logo
 
         White label admin only API to update the white label theme logo.
 
         :param organization_id: Organization ID (required)
         :type organization_id: int
         :param image:
         :type image: str
@@ -2621,15 +2768,15 @@
         :rtype: UploadAssetResponse
         """
         kwargs['_return_http_data_only'] = True
         return self._whitelabel_admin_update_theme_logo_with_http_info(organization_id, image, **kwargs)  # noqa: E501
 
     @validate_arguments
     def _whitelabel_admin_update_theme_logo_with_http_info(self, organization_id : Annotated[StrictInt, Field(..., description="Organization ID")], image : Optional[StrictStr] = None, **kwargs):  # noqa: E501
-        """Update theme logos 
+        """Update theme logo 
 
         White label admin only API to update the white label theme logo.
 
         :param organization_id: Organization ID (required)
         :type organization_id: int
         :param image:
         :type image: str
```

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/api/organizations_api.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/api/organizations_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -5287,14 +5287,161 @@
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
 
     @validate_arguments
+    def whitelabel_admin_update_theme_device_logo(self, organization_id : Annotated[StrictInt, Field(..., description="Organization ID")], image : Optional[StrictStr] = None, **kwargs) -> UploadAssetResponse:  # noqa: E501
+        """Update theme device logo
+
+        White label admin only API to update the white label theme device logo.
+
+        :param organization_id: Organization ID (required)
+        :type organization_id: int
+        :param image:
+        :type image: str
+        :param async_req: Whether to execute the request asynchronously.
+        :type async_req: bool, optional
+        :param _preload_content: if False, the urllib3.HTTPResponse object will
+                                 be returned without reading/decoding response
+                                 data. Default is True.
+        :type _preload_content: bool, optional
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :return: Returns the result object.
+                 If the method is called asynchronously,
+                 returns the request thread.
+        :rtype: UploadAssetResponse
+        """
+        kwargs['_return_http_data_only'] = True
+        return self._whitelabel_admin_update_theme_device_logo_with_http_info(organization_id, image, **kwargs)  # noqa: E501
+
+    @validate_arguments
+    def _whitelabel_admin_update_theme_device_logo_with_http_info(self, organization_id : Annotated[StrictInt, Field(..., description="Organization ID")], image : Optional[StrictStr] = None, **kwargs):  # noqa: E501
+        """Update theme device logo 
+
+        White label admin only API to update the white label theme device logo.
+
+        :param organization_id: Organization ID (required)
+        :type organization_id: int
+        :param image:
+        :type image: str
+        :param async_req: Whether to execute the request asynchronously.
+        :type async_req: bool, optional
+        :param _return_http_data_only: response data without head status code
+                                       and headers
+        :type _return_http_data_only: bool, optional
+        :param _preload_content: if False, the urllib3.HTTPResponse object will
+                                 be returned without reading/decoding response
+                                 data. Default is True.
+        :type _preload_content: bool, optional
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :param _request_auth: set to override the auth_settings for an a single
+                              request; this effectively ignores the authentication
+                              in the spec for a single request.
+        :type _request_auth: dict, optional
+        :type _content_type: string, optional: force content-type for the request
+        :return: Returns the result object.
+                 If the method is called asynchronously,
+                 returns the request thread.
+        :rtype: tuple(UploadAssetResponse, status_code(int), headers(HTTPHeaderDict))
+        """
+
+        _params = locals()
+
+        _all_params = [
+            'organization_id',
+            'image'
+        ]
+        _all_params.extend(
+            [
+                'async_req',
+                '_return_http_data_only',
+                '_preload_content',
+                '_request_timeout',
+                '_request_auth',
+                '_content_type',
+                '_headers'
+            ]
+        )
+
+        # validate the arguments
+        for _key, _val in _params['kwargs'].items():
+            if _key not in _all_params:
+                raise ApiTypeError(
+                    "Got an unexpected keyword argument '%s'"
+                    " to method whitelabel_admin_update_theme_device_logo" % _key
+                )
+            _params[_key] = _val
+        del _params['kwargs']
+
+        _collection_formats = {}
+
+        # process the path parameters
+        _path_params = {}
+        if _params['organization_id']:
+            _path_params['organizationId'] = _params['organization_id']
+
+        # process the query parameters
+        _query_params = []
+
+        # process the header parameters
+        _header_params = dict(_params.get('_headers', {}))
+
+        # process the form parameters
+        _form_params = []
+        _files = {}
+        if _params['image']:
+            _files['image'] = _params['image']
+
+        # process the body parameter
+        _body_params = None
+
+        # set the HTTP header `Accept`
+        _header_params['Accept'] = self.api_client.select_header_accept(
+            ['application/json'])  # noqa: E501
+
+        # set the HTTP header `Content-Type`
+        _content_types_list = _params.get('_content_type',
+            self.api_client.select_header_content_type(
+                ['multipart/form-data']))
+        if _content_types_list:
+                _header_params['Content-Type'] = _content_types_list
+
+        # authentication setting
+        _auth_settings = ['ApiKeyAuthentication', 'JWTAuthentication', 'JWTHttpHeaderAuthentication']  # noqa: E501
+
+        _response_types_map = {
+            '200': "UploadAssetResponse",
+        }
+
+        return self.api_client.call_api(
+            '/api/organizations/{organizationId}/whitelabel/theme/deviceLogo', 'POST',
+            _path_params,
+            _query_params,
+            _header_params,
+            body=_body_params,
+            post_params=_form_params,
+            files=_files,
+            response_types_map=_response_types_map,
+            auth_settings=_auth_settings,
+            async_req=_params.get('async_req'),
+            _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
+            _preload_content=_params.get('_preload_content', True),
+            _request_timeout=_params.get('_request_timeout'),
+            collection_formats=_collection_formats,
+            _request_auth=_params.get('_request_auth'))
+
+    @validate_arguments
     def whitelabel_admin_update_theme_favicon(self, organization_id : Annotated[StrictInt, Field(..., description="Organization ID")], image : StrictStr, **kwargs) -> GenericApiResponse:  # noqa: E501
         """Update theme favicon
 
         White label admin only API to update the theme favicon.
 
         :param organization_id: Organization ID (required)
         :type organization_id: int
@@ -5435,15 +5582,15 @@
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
 
     @validate_arguments
     def whitelabel_admin_update_theme_logo(self, organization_id : Annotated[StrictInt, Field(..., description="Organization ID")], image : Optional[StrictStr] = None, **kwargs) -> UploadAssetResponse:  # noqa: E501
-        """Update theme logos
+        """Update theme logo
 
         White label admin only API to update the white label theme logo.
 
         :param organization_id: Organization ID (required)
         :type organization_id: int
         :param image:
         :type image: str
@@ -5463,15 +5610,15 @@
         :rtype: UploadAssetResponse
         """
         kwargs['_return_http_data_only'] = True
         return self._whitelabel_admin_update_theme_logo_with_http_info(organization_id, image, **kwargs)  # noqa: E501
 
     @validate_arguments
     def _whitelabel_admin_update_theme_logo_with_http_info(self, organization_id : Annotated[StrictInt, Field(..., description="Organization ID")], image : Optional[StrictStr] = None, **kwargs):  # noqa: E501
-        """Update theme logos 
+        """Update theme logo 
 
         White label admin only API to update the white label theme logo.
 
         :param organization_id: Organization ID (required)
         :type organization_id: int
         :param image:
         :type image: str
```

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/api/performance_calibration_api.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/api/performance_calibration_api.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/api/projects_api.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/api/projects_api.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/api/raw_data_api.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/api/raw_data_api.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/api/requires_sudo_api.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/api/requires_sudo_api.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/api/requires_third_party_auth_api_key_api.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/api/requires_third_party_auth_api_key_api.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/api/supports_range_api.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/api/supports_range_api.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/api/themes_api.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/api/themes_api.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/api/third_party_auth_api.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/api/third_party_auth_api.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/api/upload_portal_api.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/api/upload_portal_api.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/api/user_api.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/api/user_api.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/api/whitelabels_api.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/api/whitelabels_api.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/api_client.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/api_client.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/configuration.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/configuration.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/exceptions.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/exceptions.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/__init__.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -442,27 +442,30 @@
 from edgeimpulse_api.models.optimize_transfer_learning_models_response import OptimizeTransferLearningModelsResponse
 from edgeimpulse_api.models.optimize_transfer_learning_models_response_all_of import OptimizeTransferLearningModelsResponseAllOf
 from edgeimpulse_api.models.optimize_transfer_learning_models_response_all_of_models import OptimizeTransferLearningModelsResponseAllOfModels
 from edgeimpulse_api.models.organization import Organization
 from edgeimpulse_api.models.organization_add_data_folder_request import OrganizationAddDataFolderRequest
 from edgeimpulse_api.models.organization_add_data_folder_response import OrganizationAddDataFolderResponse
 from edgeimpulse_api.models.organization_add_data_folder_response_all_of import OrganizationAddDataFolderResponseAllOf
+from edgeimpulse_api.models.organization_add_dataset_request import OrganizationAddDatasetRequest
+from edgeimpulse_api.models.organization_add_dataset_request_bucket import OrganizationAddDatasetRequestBucket
 from edgeimpulse_api.models.organization_create_project import OrganizationCreateProject
 from edgeimpulse_api.models.organization_create_project_request import OrganizationCreateProjectRequest
 from edgeimpulse_api.models.organization_create_project_response import OrganizationCreateProjectResponse
 from edgeimpulse_api.models.organization_create_project_response_all_of import OrganizationCreateProjectResponseAllOf
 from edgeimpulse_api.models.organization_create_project_status_response import OrganizationCreateProjectStatusResponse
 from edgeimpulse_api.models.organization_create_project_status_response_all_of import OrganizationCreateProjectStatusResponseAllOf
 from edgeimpulse_api.models.organization_create_project_transformation_summary import OrganizationCreateProjectTransformationSummary
 from edgeimpulse_api.models.organization_create_project_with_files import OrganizationCreateProjectWithFiles
 from edgeimpulse_api.models.organization_create_project_with_files_all_of import OrganizationCreateProjectWithFilesAllOf
 from edgeimpulse_api.models.organization_create_project_with_files_all_of_files import OrganizationCreateProjectWithFilesAllOfFiles
 from edgeimpulse_api.models.organization_data_item import OrganizationDataItem
 from edgeimpulse_api.models.organization_data_item_files_inner import OrganizationDataItemFilesInner
 from edgeimpulse_api.models.organization_dataset import OrganizationDataset
+from edgeimpulse_api.models.organization_dataset_bucket import OrganizationDatasetBucket
 from edgeimpulse_api.models.organization_deploy_block import OrganizationDeployBlock
 from edgeimpulse_api.models.organization_dsp_block import OrganizationDspBlock
 from edgeimpulse_api.models.organization_get_create_projects_response import OrganizationGetCreateProjectsResponse
 from edgeimpulse_api.models.organization_get_create_projects_response_all_of import OrganizationGetCreateProjectsResponseAllOf
 from edgeimpulse_api.models.organization_get_create_projects_response_all_of_jobs import OrganizationGetCreateProjectsResponseAllOfJobs
 from edgeimpulse_api.models.organization_info_response import OrganizationInfoResponse
 from edgeimpulse_api.models.organization_info_response_all_of import OrganizationInfoResponseAllOf
```

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/activate_user_by_third_party_activation_code_request.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/activate_user_by_third_party_activation_code_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/activate_user_request.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/activate_user_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/add_api_key_request.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/add_api_key_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/add_collaborator_request.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/add_collaborator_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/add_hmac_key_request.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/add_hmac_key_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/add_member_request.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/add_member_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/add_organization_api_key_request.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/add_organization_api_key_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/add_organization_bucket_request.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/add_organization_bucket_request.py`

 * *Files 13% similar despite different names*

```diff
@@ -17,22 +17,21 @@
 import json
 
 
 from typing import Optional
 from pydantic import BaseModel, Field, StrictStr
 
 class AddOrganizationBucketRequest(BaseModel):
-    name: StrictStr = Field(..., description="S3 bucket description")
     access_key: StrictStr = Field(..., alias="accessKey", description="S3 access key")
     secret_key: StrictStr = Field(..., alias="secretKey", description="S3 secret key")
     endpoint: StrictStr = Field(..., description="S3 endpoint")
     bucket: StrictStr = Field(..., description="S3 bucket")
-    prefix: Optional[StrictStr] = Field(None, description="Prefix within the bucket")
     region: StrictStr = Field(..., description="S3 region")
-    __properties = ["name", "accessKey", "secretKey", "endpoint", "bucket", "prefix", "region"]
+    check_connectivity_prefix: Optional[StrictStr] = Field(None, alias="checkConnectivityPrefix", description="Set this if you don't have access to the root of this bucket. Only used to verify connectivity to this bucket.")
+    __properties = ["accessKey", "secretKey", "endpoint", "bucket", "region", "checkConnectivityPrefix"]
 
     class Config:
         allow_population_by_field_name = True
         validate_assignment = False
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
@@ -61,17 +60,16 @@
         if obj is None:
             return None
 
         if type(obj) is not dict:
             return AddOrganizationBucketRequest.construct(**obj)
 
         _obj = AddOrganizationBucketRequest.construct(**{
-            "name": obj.get("name"),
             "access_key": obj.get("accessKey"),
             "secret_key": obj.get("secretKey"),
             "endpoint": obj.get("endpoint"),
             "bucket": obj.get("bucket"),
-            "prefix": obj.get("prefix"),
-            "region": obj.get("region")
+            "region": obj.get("region"),
+            "check_connectivity_prefix": obj.get("checkConnectivityPrefix")
         })
         return _obj
```

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/add_organization_deploy_block_response.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/add_organization_deploy_block_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/add_organization_dsp_block_request.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/add_organization_dsp_block_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/add_organization_dsp_block_response.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/add_organization_dsp_block_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/add_organization_secret_request.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/add_organization_secret_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/add_organization_secret_response.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/add_organization_secret_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/add_organization_secret_response_all_of.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/add_organization_secret_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/add_organization_transfer_learning_block_request.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/add_organization_transfer_learning_block_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/add_organization_transfer_learning_block_response.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/add_organization_transfer_learning_block_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/add_organization_transformation_block_request.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/add_organization_transformation_block_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/add_organization_transformation_block_response.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/add_organization_transformation_block_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/add_organization_transformation_block_response_all_of.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/add_organization_transformation_block_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/admin_add_or_update_sso_domain_id_ps_request.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/admin_add_or_update_sso_domain_id_ps_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/admin_add_project_user_request.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/admin_add_project_user_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/admin_api_organization.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/admin_api_organization.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/admin_api_organization_all_of.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/admin_api_organization_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/admin_api_project.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/admin_api_project.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/admin_api_user.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/admin_api_user.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/admin_api_user_all_of.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/admin_api_user_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/admin_create_organization_request.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/admin_create_organization_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/admin_get_metrics_response.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/admin_get_metrics_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/admin_get_metrics_response_all_of.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/admin_get_metrics_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/admin_get_organizations_response.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/admin_get_organizations_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/admin_get_organizations_response_all_of.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/admin_get_organizations_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/admin_get_organizations_response_all_of_organizations.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/admin_get_organizations_response_all_of_organizations.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/admin_get_sso_domain_id_ps_response.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/admin_get_sso_domain_id_ps_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/admin_get_sso_domain_id_ps_response_all_of.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/admin_get_sso_domain_id_ps_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/admin_get_sso_settings_response.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/admin_get_sso_settings_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/admin_get_sso_settings_response_all_of.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/admin_get_sso_settings_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/admin_get_sso_settings_response_all_of_sso_whitelist.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/admin_get_sso_settings_response_all_of_sso_whitelist.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/admin_get_user_ids_response.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/admin_get_user_ids_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/admin_get_user_ids_response_all_of.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/admin_get_user_ids_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/admin_get_user_metrics_response.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/admin_get_user_metrics_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/admin_get_user_metrics_response_all_of.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/admin_get_user_metrics_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/admin_get_user_response.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/admin_get_user_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/admin_get_user_response_all_of.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/admin_get_user_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/admin_get_users_response.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/admin_get_users_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/admin_get_users_response_all_of.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/admin_get_users_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/admin_get_users_response_all_of_users.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/admin_get_users_response_all_of_users.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/admin_list_projects.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/admin_list_projects.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/admin_list_projects_response.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/admin_list_projects_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/admin_organization_info_response.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/admin_organization_info_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/admin_organization_info_response_all_of.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/admin_organization_info_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/admin_update_organization_request.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/admin_update_organization_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/admin_update_user_permissions_request.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/admin_update_user_permissions_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/admin_update_user_request.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/admin_update_user_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/akida_edge_learning_config.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/akida_edge_learning_config.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/anomaly_model_metadata.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/anomaly_model_metadata.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/anomaly_model_metadata_clusters_inner.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/anomaly_model_metadata_clusters_inner.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/anomaly_model_metadata_response.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/anomaly_model_metadata_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/anomaly_response.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/anomaly_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/anomaly_response_all_of.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/anomaly_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/anomaly_response_all_of_axes.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/anomaly_response_all_of_axes.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/anomaly_trained_features_response.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/anomaly_trained_features_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/anomaly_trained_features_response_all_of.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/anomaly_trained_features_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/anomaly_trained_features_response_all_of_data.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/anomaly_trained_features_response_all_of_data.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/augmentation_policy_spectrogram.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/augmentation_policy_spectrogram.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/autotune_dsp_request.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/autotune_dsp_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/bounding_box.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/bounding_box.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/bounding_box_with_score.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/bounding_box_with_score.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/build_on_device_model_request.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/build_on_device_model_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/build_organization_on_device_model_request.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/build_organization_on_device_model_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/change_password_request.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/change_password_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/classify_job_response.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/classify_job_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/classify_job_response_all_of.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/classify_job_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/classify_job_response_all_of_accuracy.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/classify_job_response_all_of_accuracy.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/classify_job_response_all_of_accuracy_total_summary.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/classify_job_response_all_of_accuracy_total_summary.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/classify_job_response_page.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/classify_job_response_page.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/classify_job_response_page_all_of.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/classify_job_response_page_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/classify_sample_response.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/classify_sample_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/classify_sample_response_all_of.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/classify_sample_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/classify_sample_response_classification.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/classify_sample_response_classification.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/classify_sample_response_classification_details.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/classify_sample_response_classification_details.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/convert_user_request.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/convert_user_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/count_samples_response.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/count_samples_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/count_samples_response_all_of.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/count_samples_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/create_block_version_response.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/create_block_version_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/create_block_version_response_all_of.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/create_block_version_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/create_developer_profile_response.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/create_developer_profile_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/create_developer_profile_response_all_of.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/create_developer_profile_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/create_device_request.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/create_device_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/create_evaluation_user_response.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/create_evaluation_user_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/create_evaluation_user_response_all_of.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/create_evaluation_user_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/create_organization_portal_request.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/create_organization_portal_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/create_organization_portal_response.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/create_organization_portal_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/create_organization_portal_response_all_of.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/create_organization_portal_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/create_organization_request.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/create_organization_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/create_organization_response.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/create_organization_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/create_organization_response_all_of.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/create_organization_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/create_pipeline_response.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/create_pipeline_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/create_project_request.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/create_project_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/create_project_response.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/create_project_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/create_project_response_all_of.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/create_project_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/create_signed_upload_link_request.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/create_signed_upload_link_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/create_signed_upload_link_response.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/create_signed_upload_link_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/create_signed_upload_link_response_all_of.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/create_signed_upload_link_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/create_third_party_auth_request.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/create_third_party_auth_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/create_third_party_auth_response.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/create_third_party_auth_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/create_third_party_auth_response_all_of.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/create_third_party_auth_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/create_user_request.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/create_user_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/create_user_response.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/create_user_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/create_user_response_all_of.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/create_user_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/create_user_third_party_request.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/create_user_third_party_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/create_user_third_party_response.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/create_user_third_party_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/create_user_third_party_response_all_of.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/create_user_third_party_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/create_whitelabel_request.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/create_whitelabel_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/create_whitelabel_response.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/create_whitelabel_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/create_whitelabel_response_all_of.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/create_whitelabel_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/crop_sample_request.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/crop_sample_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/crop_sample_response.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/crop_sample_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/crop_sample_response_all_of.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/crop_sample_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/data_explorer_predictions_response.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/data_explorer_predictions_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/data_explorer_predictions_response_all_of.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/data_explorer_predictions_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/data_explorer_settings.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/data_explorer_settings.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/dataset_ratio_data.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/dataset_ratio_data.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/dataset_ratio_data_ratio.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/dataset_ratio_data_ratio.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/delete_portal_file_request.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/delete_portal_file_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/dependency_data.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/dependency_data.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/deploy_pretrained_model_input_audio.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/deploy_pretrained_model_input_audio.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/deploy_pretrained_model_input_image.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/deploy_pretrained_model_input_image.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/deploy_pretrained_model_input_other.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/deploy_pretrained_model_input_other.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/deploy_pretrained_model_input_time_series.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/deploy_pretrained_model_input_time_series.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/deploy_pretrained_model_model_classification.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/deploy_pretrained_model_model_classification.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/deploy_pretrained_model_model_object_detection.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/deploy_pretrained_model_model_object_detection.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/deploy_pretrained_model_model_regression.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/deploy_pretrained_model_model_regression.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/deploy_pretrained_model_request.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/deploy_pretrained_model_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/deploy_pretrained_model_request_model_info.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/deploy_pretrained_model_request_model_info.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/deploy_pretrained_model_request_model_info_input.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/deploy_pretrained_model_request_model_info_input.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/deploy_pretrained_model_request_model_info_model.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/deploy_pretrained_model_request_model_info_model.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/deployment_target.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/deployment_target.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/deployment_target_badge.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/deployment_target_badge.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/deployment_target_engine.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/deployment_target_engine.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/deployment_targets_response.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/deployment_targets_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/deployment_targets_response_all_of.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/deployment_targets_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/development_board.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/development_board.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/development_boards_response.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/development_boards_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/development_boards_response_all_of.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/development_boards_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/development_keys.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/development_keys.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/development_keys_response.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/development_keys_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/device.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/device.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/device_name_response.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/device_name_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/device_name_response_all_of.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/device_name_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/device_sensors_inner.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/device_sensors_inner.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/download.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/download.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/download_portal_file_request.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/download_portal_file_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/download_portal_file_response.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/download_portal_file_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/download_portal_file_response_all_of.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/download_portal_file_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/dsp_autotuner_results.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/dsp_autotuner_results.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/dsp_autotuner_results_all_of.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/dsp_autotuner_results_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/dsp_autotuner_results_all_of_results.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/dsp_autotuner_results_all_of_results.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/dsp_block.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/dsp_block.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/dsp_config_request.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/dsp_config_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/dsp_config_response.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/dsp_config_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/dsp_config_response_all_of.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/dsp_config_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/dsp_feature_importance_response.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/dsp_feature_importance_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/dsp_feature_importance_response_all_of.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/dsp_feature_importance_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/dsp_feature_importance_response_all_of_features.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/dsp_feature_importance_response_all_of_features.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/dsp_feature_importance_response_all_of_labels.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/dsp_feature_importance_response_all_of_labels.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/dsp_feature_labels_response.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/dsp_feature_labels_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/dsp_feature_labels_response_all_of.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/dsp_feature_labels_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/dsp_group.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/dsp_group.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/dsp_group_item.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/dsp_group_item.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/dsp_group_item_select_options_inner.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/dsp_group_item_select_options_inner.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/dsp_group_item_show_if.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/dsp_group_item_show_if.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/dsp_info.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/dsp_info.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/dsp_info_features.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/dsp_info_features.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/dsp_info_performance.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/dsp_info_performance.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/dsp_metadata.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/dsp_metadata.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/dsp_metadata_included_samples_inner.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/dsp_metadata_included_samples_inner.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/dsp_metadata_output_config.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/dsp_metadata_output_config.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/dsp_metadata_output_config_shape.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/dsp_metadata_output_config_shape.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/dsp_metadata_response.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/dsp_metadata_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/dsp_performance_all_variants_response.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/dsp_performance_all_variants_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/dsp_performance_all_variants_response_all_of.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/dsp_performance_all_variants_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/dsp_performance_all_variants_response_all_of_performance.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/dsp_performance_all_variants_response_all_of_performance.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/dsp_run_graph.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/dsp_run_graph.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/dsp_run_graph_axis_labels.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/dsp_run_graph_axis_labels.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/dsp_run_request_with_features.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/dsp_run_request_with_features.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/dsp_run_request_without_features.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/dsp_run_request_without_features.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/dsp_run_request_without_features_read_only.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/dsp_run_request_without_features_read_only.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/dsp_run_response.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/dsp_run_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/dsp_run_response_all_of.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/dsp_run_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/dsp_run_response_all_of_performance.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/dsp_run_response_all_of_performance.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/dsp_run_response_with_sample.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/dsp_run_response_with_sample.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/dsp_run_response_with_sample_all_of.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/dsp_run_response_with_sample_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/dsp_sample_features_response.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/dsp_sample_features_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/dsp_sample_features_response_all_of.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/dsp_sample_features_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/dsp_sample_features_response_all_of_data.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/dsp_sample_features_response_all_of_data.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/dsp_sample_features_response_all_of_sample.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/dsp_sample_features_response_all_of_sample.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/dsp_trained_features_response.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/dsp_trained_features_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/dsp_trained_features_response_all_of.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/dsp_trained_features_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/dsp_trained_features_response_all_of_data.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/dsp_trained_features_response_all_of_data.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/dsp_trained_features_response_all_of_sample.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/dsp_trained_features_response_all_of_sample.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/edit_sample_label_request.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/edit_sample_label_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/evaluate_job_response.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/evaluate_job_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/evaluate_job_response_all_of.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/evaluate_job_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/evaluate_result_value.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/evaluate_result_value.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/export_get_url_response.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/export_get_url_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/export_get_url_response_all_of.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/export_get_url_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/export_original_data_request.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/export_original_data_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/export_wav_data_request.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/export_wav_data_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/find_segment_sample_request.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/find_segment_sample_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/find_segment_sample_response.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/find_segment_sample_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/find_segment_sample_response_all_of.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/find_segment_sample_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/find_segment_sample_response_all_of_segments.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/find_segment_sample_response_all_of_segments.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/find_user_response.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/find_user_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/find_user_response_all_of.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/find_user_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/find_user_response_all_of_users.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/find_user_response_all_of_users.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/generate_features_request.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/generate_features_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/generic_api_response.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/generic_api_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/get_all_third_party_auth_response.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/get_all_third_party_auth_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/get_all_third_party_auth_response_all_of.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/get_all_third_party_auth_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/get_all_whitelabels_response.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/get_all_whitelabels_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/get_all_whitelabels_response_all_of.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/get_all_whitelabels_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/get_data_explorer_features_response.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/get_data_explorer_features_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/get_data_explorer_features_response_all_of.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/get_data_explorer_features_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/get_data_explorer_settings_response.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/get_data_explorer_settings_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/get_data_explorer_settings_response_all_of.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/get_data_explorer_settings_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/get_deployment_response.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/get_deployment_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/get_deployment_response_all_of.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/get_deployment_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/get_device_response.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/get_device_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/get_device_response_all_of.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/get_device_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/get_impulse_blocks_response.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/get_impulse_blocks_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/get_impulse_blocks_response_all_of.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/get_impulse_blocks_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/get_impulse_response.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/get_impulse_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/get_impulse_response_all_of.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/get_impulse_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/get_job_response.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/get_job_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/get_job_response_all_of.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/get_job_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/get_jwt_request.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/get_jwt_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/get_jwt_response.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/get_jwt_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/get_jwt_response_all_of.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/get_jwt_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/get_last_deployment_build_response.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/get_last_deployment_build_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/get_last_deployment_build_response_all_of.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/get_last_deployment_build_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/get_last_deployment_build_response_all_of_last_build.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/get_last_deployment_build_response_all_of_last_build.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/get_notes_response.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/get_notes_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/get_notes_response_all_of.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/get_notes_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/get_organization_data_item_response.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/get_organization_data_item_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/get_organization_data_item_response_all_of.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/get_organization_data_item_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/get_organization_data_item_transform_jobs_response.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/get_organization_data_item_transform_jobs_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/get_organization_data_item_transform_jobs_response_all_of.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/get_organization_data_item_transform_jobs_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/get_organization_data_item_transform_jobs_response_all_of_transformation_jobs.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/get_organization_data_item_transform_jobs_response_all_of_transformation_jobs.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/get_organization_dataset_response.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/get_organization_dataset_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/get_organization_dataset_response_all_of.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/get_organization_dataset_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/get_organization_pipelines_response.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/get_organization_pipelines_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/get_organization_pipelines_response_all_of.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/get_organization_pipelines_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/get_organization_portal_response.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/get_organization_portal_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/get_organization_portal_response_all_of.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/get_organization_portal_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/get_organization_projects_data_count_response.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/get_organization_projects_data_count_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/get_performance_calibration_ground_truth_response.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/get_performance_calibration_ground_truth_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/get_performance_calibration_ground_truth_response_all_of.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/get_performance_calibration_ground_truth_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/get_performance_calibration_parameter_sets_response.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/get_performance_calibration_parameter_sets_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/get_performance_calibration_parameter_sets_response_all_of.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/get_performance_calibration_parameter_sets_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/get_performance_calibration_parameters_response.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/get_performance_calibration_parameters_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/get_performance_calibration_parameters_response_all_of.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/get_performance_calibration_parameters_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/get_performance_calibration_raw_result_response.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/get_performance_calibration_raw_result_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/get_performance_calibration_raw_result_response_all_of.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/get_performance_calibration_raw_result_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/get_performance_calibration_status_response.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/get_performance_calibration_status_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/get_performance_calibration_status_response_all_of.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/get_performance_calibration_status_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/get_pretrained_model_response.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/get_pretrained_model_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/get_pretrained_model_response_all_of.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/get_pretrained_model_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/get_pretrained_model_response_all_of_model.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/get_pretrained_model_response_all_of_model.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/get_pretrained_model_response_all_of_model_info.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/get_pretrained_model_response_all_of_model_info.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/get_pretrained_model_response_all_of_model_profile_info.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/get_pretrained_model_response_all_of_model_profile_info.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/get_public_metrics_response.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/get_public_metrics_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/get_public_metrics_response_all_of.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/get_public_metrics_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/get_sample_metadata_response.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/get_sample_metadata_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/get_sample_response.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/get_sample_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/get_syntiant_posterior_response.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/get_syntiant_posterior_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/get_syntiant_posterior_response_all_of.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/get_syntiant_posterior_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/get_theme_response.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/get_theme_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/get_theme_response_all_of.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/get_theme_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/get_themes_response.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/get_themes_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/get_themes_response_all_of.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/get_themes_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/get_third_party_auth_response.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/get_third_party_auth_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/get_third_party_auth_response_all_of.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/get_third_party_auth_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/get_user_need_to_set_password_response.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/get_user_need_to_set_password_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/get_user_need_to_set_password_response_all_of.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/get_user_need_to_set_password_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/get_user_response.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/get_user_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/get_user_response_all_of.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/get_user_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/get_user_response_all_of_whitelabels.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/get_user_response_all_of_whitelabels.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/get_whitelabel_domain_response.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/get_whitelabel_domain_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/get_whitelabel_domain_response_all_of.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/get_whitelabel_domain_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/get_whitelabel_response.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/get_whitelabel_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/get_whitelabel_response_all_of.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/get_whitelabel_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/has_data_explorer_features_response.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/has_data_explorer_features_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/has_data_explorer_features_response_all_of.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/has_data_explorer_features_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/impulse.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/impulse.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/impulse_block_version.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/impulse_block_version.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/impulse_dsp_block.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/impulse_dsp_block.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/impulse_dsp_block_organization.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/impulse_dsp_block_organization.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/impulse_input_block.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/impulse_input_block.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/impulse_learn_block.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/impulse_learn_block.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/input_block.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/input_block.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/invite_organization_member_request.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/invite_organization_member_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/job.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/job.py`

 * *Files 11% similar despite different names*

```diff
@@ -26,15 +26,16 @@
     key: StrictStr = Field(..., description="External job identifier, this can be used to categorize jobs, and recover job status. E.g. set this to 'keras-192' for a Keras learning block with ID 192. When a user refreshes the page you can check whether a job is active for this ID and re-attach. ")
     created: datetime = Field(..., description="When the job was created.")
     started: Optional[datetime] = Field(None, description="When the job was started.")
     finished: Optional[datetime] = Field(None, description="When the job was finished.")
     finished_successful: Optional[StrictBool] = Field(None, alias="finishedSuccessful", description="Whether the job finished successfully.")
     job_notification_uids: List[StrictInt] = Field(..., alias="jobNotificationUids", description="The IDs of users who should be notified when a job is finished.")
     additional_info: Optional[StrictStr] = Field(None, alias="additionalInfo", description="Additional metadata associated with this job.")
-    __properties = ["id", "category", "key", "created", "started", "finished", "finishedSuccessful", "jobNotificationUids", "additionalInfo"]
+    compute_time: Optional[float] = Field(None, alias="computeTime", description="Job duration time in seconds from start to finished, measured by k8s job watcher.")
+    __properties = ["id", "category", "key", "created", "started", "finished", "finishedSuccessful", "jobNotificationUids", "additionalInfo", "computeTime"]
 
     class Config:
         allow_population_by_field_name = True
         validate_assignment = False
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
@@ -71,11 +72,12 @@
             "category": obj.get("category"),
             "key": obj.get("key"),
             "created": obj.get("created"),
             "started": obj.get("started"),
             "finished": obj.get("finished"),
             "finished_successful": obj.get("finishedSuccessful"),
             "job_notification_uids": obj.get("jobNotificationUids"),
-            "additional_info": obj.get("additionalInfo")
+            "additional_info": obj.get("additionalInfo"),
+            "compute_time": obj.get("computeTime")
         })
         return _obj
```

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/job_summary_response.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/job_summary_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/job_summary_response_all_of.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/job_summary_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/job_summary_response_all_of_summary.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/job_summary_response_all_of_summary.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/keras_model_layer.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/keras_model_layer.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/keras_model_layer_input.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/keras_model_layer_input.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/keras_model_layer_output.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/keras_model_layer_output.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/keras_model_metadata.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/keras_model_metadata.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/keras_model_metadata_all_of.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/keras_model_metadata_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/keras_model_metadata_metrics.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/keras_model_metadata_metrics.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/keras_model_metadata_metrics_on_device_performance_inner.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/keras_model_metadata_metrics_on_device_performance_inner.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/keras_model_metadata_metrics_on_device_performance_inner_tflite.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/keras_model_metadata_metrics_on_device_performance_inner_tflite.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/keras_model_type_enum.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/keras_model_type_enum.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/keras_response.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/keras_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/keras_response_all_of.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/keras_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/keras_visual_layer.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/keras_visual_layer.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/keras_visual_layer_type.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/keras_visual_layer_type.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/last_modification_date_response.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/last_modification_date_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/last_modification_date_response_all_of.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/last_modification_date_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/latency_device.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/latency_device.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/learn_block.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/learn_block.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/learn_block_type.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/learn_block_type.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/list_api_keys_response.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/list_api_keys_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/list_api_keys_response_all_of.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/list_api_keys_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/list_api_keys_response_all_of_api_keys.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/list_api_keys_response_all_of_api_keys.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/list_devices_response.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/list_devices_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/list_devices_response_all_of.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/list_devices_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/list_email_response.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/list_email_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/list_email_response_all_of.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/list_email_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/list_email_response_all_of_emails.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/list_email_response_all_of_emails.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/list_hmac_keys_response.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/list_hmac_keys_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/list_hmac_keys_response_all_of.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/list_hmac_keys_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/list_hmac_keys_response_all_of_hmac_keys.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/list_hmac_keys_response_all_of_hmac_keys.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/list_jobs_response.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/list_jobs_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/list_jobs_response_all_of.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/list_jobs_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/list_models_response.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/list_models_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/list_models_response_all_of.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/list_models_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/list_organization_api_keys_response.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/list_organization_api_keys_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/list_organization_api_keys_response_all_of.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/list_organization_api_keys_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/list_organization_api_keys_response_all_of_api_keys.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/list_organization_api_keys_response_all_of_api_keys.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/list_organization_buckets_response.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/list_organization_buckets_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/list_organization_buckets_response_all_of.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/list_organization_buckets_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/list_organization_buckets_response_all_of_buckets.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/verify_organization_bucket_request.py`

 * *Files 15% similar despite different names*

```diff
@@ -14,66 +14,62 @@
 from inspect import getfullargspec
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Optional
-from pydantic import BaseModel, Field, StrictBool, StrictInt, StrictStr
+from pydantic import BaseModel, Field, StrictStr
 
-class ListOrganizationBucketsResponseAllOfBuckets(BaseModel):
-    id: StrictInt = ...
-    name: StrictStr = Field(..., description="S3 bucket description")
+class VerifyOrganizationBucketRequest(BaseModel):
     access_key: StrictStr = Field(..., alias="accessKey", description="S3 access key")
-    endpoint: StrictStr = Field(..., description="S3 endpoint")
+    secret_key: StrictStr = Field(..., alias="secretKey", description="S3 secret key")
     bucket: StrictStr = Field(..., description="S3 bucket")
-    prefix: Optional[StrictStr] = Field(None, description="Prefix within the bucket")
+    endpoint: StrictStr = Field(..., description="S3 endpoint")
     region: StrictStr = Field(..., description="S3 region")
-    connected: StrictBool = Field(..., description="Whether we can reach the bucket")
-    __properties = ["id", "name", "accessKey", "endpoint", "bucket", "prefix", "region", "connected"]
+    prefix: Optional[StrictStr] = Field(None, description="Optional prefix in the bucket. Set this if you don't have access to the full bucket for example.")
+    __properties = ["accessKey", "secretKey", "bucket", "endpoint", "region", "prefix"]
 
     class Config:
         allow_population_by_field_name = True
         validate_assignment = False
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
         return pprint.pformat(self.dict(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> ListOrganizationBucketsResponseAllOfBuckets:
-        """Create an instance of ListOrganizationBucketsResponseAllOfBuckets from a JSON string"""
+    def from_json(cls, json_str: str) -> VerifyOrganizationBucketRequest:
+        """Create an instance of VerifyOrganizationBucketRequest from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self):
         """Returns the dictionary representation of the model using alias"""
         _dict = self.dict(by_alias=True,
                           exclude={
                           },
                           exclude_none=True)
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> ListOrganizationBucketsResponseAllOfBuckets:
-        """Create an instance of ListOrganizationBucketsResponseAllOfBuckets from a dict"""
+    def from_dict(cls, obj: dict) -> VerifyOrganizationBucketRequest:
+        """Create an instance of VerifyOrganizationBucketRequest from a dict"""
         if obj is None:
             return None
 
         if type(obj) is not dict:
-            return ListOrganizationBucketsResponseAllOfBuckets.construct(**obj)
+            return VerifyOrganizationBucketRequest.construct(**obj)
 
-        _obj = ListOrganizationBucketsResponseAllOfBuckets.construct(**{
-            "id": obj.get("id"),
-            "name": obj.get("name"),
+        _obj = VerifyOrganizationBucketRequest.construct(**{
             "access_key": obj.get("accessKey"),
-            "endpoint": obj.get("endpoint"),
+            "secret_key": obj.get("secretKey"),
             "bucket": obj.get("bucket"),
-            "prefix": obj.get("prefix"),
+            "endpoint": obj.get("endpoint"),
             "region": obj.get("region"),
-            "connected": obj.get("connected")
+            "prefix": obj.get("prefix")
         })
         return _obj
```

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/list_organization_buckets_user_response.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/list_organization_buckets_user_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/list_organization_buckets_user_response_all_of.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/list_organization_buckets_user_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/list_organization_buckets_user_response_all_of_buckets.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/list_organization_buckets_user_response_all_of_buckets.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,27 +13,25 @@
 from __future__ import annotations
 from inspect import getfullargspec
 import pprint
 import re  # noqa: F401
 import json
 
 
-from typing import Optional
+
 from pydantic import BaseModel, Field, StrictInt, StrictStr
 
 class ListOrganizationBucketsUserResponseAllOfBuckets(BaseModel):
     id: StrictInt = ...
     organization_id: StrictInt = Field(..., alias="organizationId")
     organization_name: StrictStr = Field(..., alias="organizationName")
-    name: StrictStr = Field(..., description="S3 bucket description")
     bucket: StrictStr = Field(..., description="S3 bucket")
-    prefix: Optional[StrictStr] = Field(None, description="Prefix within the bucket")
     region: StrictStr = Field(..., description="S3 region")
     whitelabel_id: StrictInt = Field(..., alias="whitelabelId", description="The unique identifier of the white label this bucket belongs to, if any")
-    __properties = ["id", "organizationId", "organizationName", "name", "bucket", "prefix", "region", "whitelabelId"]
+    __properties = ["id", "organizationId", "organizationName", "bucket", "region", "whitelabelId"]
 
     class Config:
         allow_population_by_field_name = True
         validate_assignment = False
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
@@ -65,15 +63,13 @@
         if type(obj) is not dict:
             return ListOrganizationBucketsUserResponseAllOfBuckets.construct(**obj)
 
         _obj = ListOrganizationBucketsUserResponseAllOfBuckets.construct(**{
             "id": obj.get("id"),
             "organization_id": obj.get("organizationId"),
             "organization_name": obj.get("organizationName"),
-            "name": obj.get("name"),
             "bucket": obj.get("bucket"),
-            "prefix": obj.get("prefix"),
             "region": obj.get("region"),
             "whitelabel_id": obj.get("whitelabelId")
         })
         return _obj
```

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/list_organization_data_response.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/list_organization_data_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/list_organization_data_response_all_of.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/list_organization_data_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/list_organization_data_response_all_of_data.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/list_organization_data_response_all_of_data.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/list_organization_deploy_blocks_response.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/list_organization_deploy_blocks_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/list_organization_deploy_blocks_response_all_of.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/list_organization_deploy_blocks_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/list_organization_dsp_blocks_response.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/list_organization_dsp_blocks_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/list_organization_dsp_blocks_response_all_of.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/list_organization_dsp_blocks_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/list_organization_files_response.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/list_organization_files_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/list_organization_files_response_all_of.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/list_organization_files_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/list_organization_pipelines_response.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/list_organization_pipelines_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/list_organization_pipelines_response_all_of.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/list_organization_pipelines_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/list_organization_portals_response.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/list_organization_portals_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/list_organization_portals_response_all_of.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/list_organization_portals_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/list_organization_portals_response_all_of_portals.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/list_organization_portals_response_all_of_portals.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/list_organization_projects_data_response.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/list_organization_projects_data_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/list_organization_projects_data_response_all_of.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/list_organization_projects_data_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/list_organization_projects_data_response_all_of_projects.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/list_organization_projects_data_response_all_of_projects.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/list_organization_projects_response.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/list_organization_projects_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/list_organization_projects_response_all_of.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/list_organization_projects_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/list_organization_secrets_response.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/list_organization_secrets_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/list_organization_secrets_response_all_of.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/list_organization_secrets_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/list_organization_secrets_response_all_of_secrets.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/list_organization_secrets_response_all_of_secrets.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/list_organization_transfer_learning_blocks_response.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/list_organization_transfer_learning_blocks_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/list_organization_transfer_learning_blocks_response_all_of.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/list_organization_transfer_learning_blocks_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/list_organization_transformation_blocks_response.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/list_organization_transformation_blocks_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/list_organization_transformation_blocks_response_all_of.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/list_organization_transformation_blocks_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/list_organizations_response.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/list_organizations_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/list_organizations_response_all_of.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/list_organizations_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/list_portal_files_in_folder_request.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/list_portal_files_in_folder_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/list_portal_files_in_folder_response.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/list_portal_files_in_folder_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/list_portal_files_in_folder_response_all_of.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/list_portal_files_in_folder_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/list_projects.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/list_projects.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/list_projects_response.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/list_projects_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/list_public_projects.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/list_public_projects.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/list_public_projects_response.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/list_public_projects_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/list_public_versions_response.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/list_public_versions_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/list_public_versions_response_all_of.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/list_public_versions_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/list_public_versions_response_all_of_versions.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/list_public_versions_response_all_of_versions.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/list_samples_response.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/list_samples_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/list_samples_response_all_of.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/list_samples_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/list_versions_response.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/list_versions_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/list_versions_response_all_of.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/list_versions_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/list_versions_response_all_of_bucket.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/list_versions_response_all_of_bucket.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/list_versions_response_all_of_custom_learn_blocks.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/list_versions_response_all_of_custom_learn_blocks.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/list_versions_response_all_of_versions.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/list_versions_response_all_of_versions.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/log_stdout_response.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/log_stdout_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/log_stdout_response_all_of.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/log_stdout_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/log_stdout_response_all_of_stdout.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/log_stdout_response_all_of_stdout.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/log_website_pageview_request.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/log_website_pageview_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/login_response.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/login_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/login_response_all_of.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/login_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/model_prediction.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/model_prediction.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/model_result.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/model_result.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/model_variant_stats.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/model_variant_stats.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/move_raw_data_request.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/move_raw_data_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/note.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/note.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/object_detection_auto_label_request.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/object_detection_auto_label_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/object_detection_auto_label_response.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/object_detection_auto_label_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/object_detection_auto_label_response_all_of.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/object_detection_auto_label_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/object_detection_auto_label_response_all_of_results.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/object_detection_auto_label_response_all_of_results.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/object_detection_label_queue_count_response.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/object_detection_label_queue_count_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/object_detection_label_queue_count_response_all_of.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/object_detection_label_queue_count_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/object_detection_label_queue_response.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/object_detection_label_queue_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/object_detection_label_queue_response_all_of.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/object_detection_label_queue_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/object_detection_last_layer.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/object_detection_last_layer.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/optimize_config.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/optimize_config.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/optimize_config_response.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/optimize_config_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/optimize_config_response_all_of.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/optimize_config_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/optimize_config_target_device.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/optimize_config_target_device.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/optimize_dsp_parameters_response.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/optimize_dsp_parameters_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/optimize_dsp_parameters_response_all_of.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/optimize_dsp_parameters_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/optimize_space_response.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/optimize_space_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/optimize_space_response_all_of.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/optimize_space_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/optimize_state_response.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/optimize_state_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/optimize_state_response_all_of.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/optimize_state_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/optimize_state_response_all_of_status.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/optimize_state_response_all_of_status.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/optimize_state_response_all_of_workers.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/optimize_state_response_all_of_workers.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/optimize_transfer_learning_models_response.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/optimize_transfer_learning_models_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/optimize_transfer_learning_models_response_all_of.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/optimize_transfer_learning_models_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/optimize_transfer_learning_models_response_all_of_models.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/optimize_transfer_learning_models_response_all_of_models.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/organization.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/organization.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/organization_add_data_folder_request.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/organization_add_data_folder_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/organization_add_data_folder_response.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/organization_add_data_folder_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/organization_add_data_folder_response_all_of.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/organization_add_data_folder_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/organization_create_project.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/organization_create_project.py`

 * *Files 4% similar despite different names*

```diff
@@ -37,14 +37,16 @@
     project_name: Optional[StrictStr] = Field(None, alias="projectName")
     transformation_block_id: Optional[StrictInt] = Field(None, alias="transformationBlockId")
     builtin_transformation_block: Optional[Dict[str, Any]] = Field(None, alias="builtinTransformationBlock")
     transformation_block_name: Optional[StrictStr] = Field(None, alias="transformationBlockName")
     category: StrictStr = ...
     created: datetime = ...
     output_dataset_name: Optional[StrictStr] = Field(None, alias="outputDatasetName")
+    output_dataset_bucket_id: Optional[StrictInt] = Field(None, alias="outputDatasetBucketId")
+    output_dataset_bucket_path: Optional[StrictStr] = Field(None, alias="outputDatasetBucketPath")
     total_download_file_count: StrictInt = Field(..., alias="totalDownloadFileCount")
     total_download_file_size: StrictInt = Field(..., alias="totalDownloadFileSize")
     total_download_file_size_string: StrictStr = Field(..., alias="totalDownloadFileSizeString")
     total_upload_file_count: StrictInt = Field(..., alias="totalUploadFileCount")
     transformation_parallel: StrictInt = Field(..., alias="transformationParallel", description="Number of transformation jobs that can be ran in parallel")
     transformation_summary: OrganizationCreateProjectTransformationSummary = Field(..., alias="transformationSummary")
     in_progress: StrictBool = Field(..., alias="inProgress")
@@ -52,15 +54,15 @@
     filter_query: Optional[StrictStr] = Field(None, alias="filterQuery")
     email_recipient_uids: Optional[List[StrictInt]] = Field(None, alias="emailRecipientUids")
     pipeline_id: Optional[StrictInt] = Field(None, alias="pipelineId")
     pipeline_name: Optional[StrictStr] = Field(None, alias="pipelineName")
     pipeline_run_id: Optional[StrictInt] = Field(None, alias="pipelineRunId")
     pipeline_step: Optional[StrictInt] = Field(None, alias="pipelineStep")
     operates_on: StrictStr = Field(..., alias="operatesOn")
-    __properties = ["id", "organizationId", "name", "uploadType", "status", "transformJobStatus", "uploadJobId", "uploadJobStatus", "uploadJobFilesUploaded", "projectOwner", "projectId", "projectName", "transformationBlockId", "builtinTransformationBlock", "transformationBlockName", "category", "created", "outputDatasetName", "totalDownloadFileCount", "totalDownloadFileSize", "totalDownloadFileSizeString", "totalUploadFileCount", "transformationParallel", "transformationSummary", "inProgress", "label", "filterQuery", "emailRecipientUids", "pipelineId", "pipelineName", "pipelineRunId", "pipelineStep", "operatesOn"]
+    __properties = ["id", "organizationId", "name", "uploadType", "status", "transformJobStatus", "uploadJobId", "uploadJobStatus", "uploadJobFilesUploaded", "projectOwner", "projectId", "projectName", "transformationBlockId", "builtinTransformationBlock", "transformationBlockName", "category", "created", "outputDatasetName", "outputDatasetBucketId", "outputDatasetBucketPath", "totalDownloadFileCount", "totalDownloadFileSize", "totalDownloadFileSizeString", "totalUploadFileCount", "transformationParallel", "transformationSummary", "inProgress", "label", "filterQuery", "emailRecipientUids", "pipelineId", "pipelineName", "pipelineRunId", "pipelineStep", "operatesOn"]
 
     @validator('upload_type')
     def upload_type_validate_enum(cls, v):
         if v not in ('dataset', 'project'):
             raise ValueError("must validate the enum values ('dataset', 'project')")
         return v
 
@@ -128,14 +130,16 @@
             "project_name": obj.get("projectName"),
             "transformation_block_id": obj.get("transformationBlockId"),
             "builtin_transformation_block": obj.get("builtinTransformationBlock"),
             "transformation_block_name": obj.get("transformationBlockName"),
             "category": obj.get("category"),
             "created": obj.get("created"),
             "output_dataset_name": obj.get("outputDatasetName"),
+            "output_dataset_bucket_id": obj.get("outputDatasetBucketId"),
+            "output_dataset_bucket_path": obj.get("outputDatasetBucketPath"),
             "total_download_file_count": obj.get("totalDownloadFileCount"),
             "total_download_file_size": obj.get("totalDownloadFileSize"),
             "total_download_file_size_string": obj.get("totalDownloadFileSizeString"),
             "total_upload_file_count": obj.get("totalUploadFileCount"),
             "transformation_parallel": obj.get("transformationParallel"),
             "transformation_summary": OrganizationCreateProjectTransformationSummary.from_dict(obj.get("transformationSummary")) if obj.get("transformationSummary") is not None else None,
             "in_progress": obj.get("inProgress"),
```

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/organization_create_project_request.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/organization_create_project_request.py`

 * *Files 12% similar despite different names*

```diff
@@ -28,19 +28,21 @@
     new_project_name: Optional[StrictStr] = Field(None, alias="newProjectName")
     project_api_key: Optional[StrictStr] = Field(None, alias="projectApiKey")
     project_hmac_key: Optional[StrictStr] = Field(None, alias="projectHmacKey")
     transformation_block_id: Optional[StrictInt] = Field(None, alias="transformationBlockId")
     builtin_transformation_block: Optional[Dict[str, Any]] = Field(None, alias="builtinTransformationBlock")
     category: Optional[StrictStr] = None
     output_dataset_name: Optional[StrictStr] = Field(None, alias="outputDatasetName")
+    output_dataset_bucket_id: Optional[StrictInt] = Field(None, alias="outputDatasetBucketId")
+    output_dataset_bucket_path: Optional[StrictStr] = Field(None, alias="outputDatasetBucketPath")
     label: Optional[StrictStr] = None
     email_recipient_uids: Optional[List[StrictInt]] = Field(None, alias="emailRecipientUids")
     transformation_parallel: Optional[StrictInt] = Field(None, alias="transformationParallel", description="Number of parallel jobs to start")
     extra_cli_arguments: Optional[StrictStr] = Field(None, alias="extraCliArguments", description="Optional extra arguments for this transformation block")
-    __properties = ["name", "filter", "uploadType", "projectId", "newProjectName", "projectApiKey", "projectHmacKey", "transformationBlockId", "builtinTransformationBlock", "category", "outputDatasetName", "label", "emailRecipientUids", "transformationParallel", "extraCliArguments"]
+    __properties = ["name", "filter", "uploadType", "projectId", "newProjectName", "projectApiKey", "projectHmacKey", "transformationBlockId", "builtinTransformationBlock", "category", "outputDatasetName", "outputDatasetBucketId", "outputDatasetBucketPath", "label", "emailRecipientUids", "transformationParallel", "extraCliArguments"]
 
     @validator('upload_type')
     def upload_type_validate_enum(cls, v):
         if v is None:
             return v
 
         if v not in ('project', 'dataset'):
@@ -98,14 +100,16 @@
             "new_project_name": obj.get("newProjectName"),
             "project_api_key": obj.get("projectApiKey"),
             "project_hmac_key": obj.get("projectHmacKey"),
             "transformation_block_id": obj.get("transformationBlockId"),
             "builtin_transformation_block": obj.get("builtinTransformationBlock"),
             "category": obj.get("category"),
             "output_dataset_name": obj.get("outputDatasetName"),
+            "output_dataset_bucket_id": obj.get("outputDatasetBucketId"),
+            "output_dataset_bucket_path": obj.get("outputDatasetBucketPath"),
             "label": obj.get("label"),
             "email_recipient_uids": obj.get("emailRecipientUids"),
             "transformation_parallel": obj.get("transformationParallel"),
             "extra_cli_arguments": obj.get("extraCliArguments")
         })
         return _obj
```

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/organization_create_project_response.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/organization_create_project_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/organization_create_project_response_all_of.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/organization_create_project_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/organization_create_project_status_response.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/organization_create_project_status_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/organization_create_project_status_response_all_of.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/organization_create_project_status_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/organization_create_project_transformation_summary.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/organization_create_project_transformation_summary.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/organization_create_project_with_files.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/organization_create_project_with_files.py`

 * *Files 5% similar despite different names*

```diff
@@ -38,14 +38,16 @@
     project_name: Optional[StrictStr] = Field(None, alias="projectName")
     transformation_block_id: Optional[StrictInt] = Field(None, alias="transformationBlockId")
     builtin_transformation_block: Optional[Dict[str, Any]] = Field(None, alias="builtinTransformationBlock")
     transformation_block_name: Optional[StrictStr] = Field(None, alias="transformationBlockName")
     category: StrictStr = ...
     created: datetime = ...
     output_dataset_name: Optional[StrictStr] = Field(None, alias="outputDatasetName")
+    output_dataset_bucket_id: Optional[StrictInt] = Field(None, alias="outputDatasetBucketId")
+    output_dataset_bucket_path: Optional[StrictStr] = Field(None, alias="outputDatasetBucketPath")
     total_download_file_count: StrictInt = Field(..., alias="totalDownloadFileCount")
     total_download_file_size: StrictInt = Field(..., alias="totalDownloadFileSize")
     total_download_file_size_string: StrictStr = Field(..., alias="totalDownloadFileSizeString")
     total_upload_file_count: StrictInt = Field(..., alias="totalUploadFileCount")
     transformation_parallel: StrictInt = Field(..., alias="transformationParallel", description="Number of transformation jobs that can be ran in parallel")
     transformation_summary: OrganizationCreateProjectTransformationSummary = Field(..., alias="transformationSummary")
     in_progress: StrictBool = Field(..., alias="inProgress")
@@ -54,15 +56,15 @@
     email_recipient_uids: Optional[List[StrictInt]] = Field(None, alias="emailRecipientUids")
     pipeline_id: Optional[StrictInt] = Field(None, alias="pipelineId")
     pipeline_name: Optional[StrictStr] = Field(None, alias="pipelineName")
     pipeline_run_id: Optional[StrictInt] = Field(None, alias="pipelineRunId")
     pipeline_step: Optional[StrictInt] = Field(None, alias="pipelineStep")
     operates_on: StrictStr = Field(..., alias="operatesOn")
     files: List[OrganizationCreateProjectWithFilesAllOfFiles] = ...
-    __properties = ["id", "organizationId", "name", "uploadType", "status", "transformJobStatus", "uploadJobId", "uploadJobStatus", "uploadJobFilesUploaded", "projectOwner", "projectId", "projectName", "transformationBlockId", "builtinTransformationBlock", "transformationBlockName", "category", "created", "outputDatasetName", "totalDownloadFileCount", "totalDownloadFileSize", "totalDownloadFileSizeString", "totalUploadFileCount", "transformationParallel", "transformationSummary", "inProgress", "label", "filterQuery", "emailRecipientUids", "pipelineId", "pipelineName", "pipelineRunId", "pipelineStep", "operatesOn", "files"]
+    __properties = ["id", "organizationId", "name", "uploadType", "status", "transformJobStatus", "uploadJobId", "uploadJobStatus", "uploadJobFilesUploaded", "projectOwner", "projectId", "projectName", "transformationBlockId", "builtinTransformationBlock", "transformationBlockName", "category", "created", "outputDatasetName", "outputDatasetBucketId", "outputDatasetBucketPath", "totalDownloadFileCount", "totalDownloadFileSize", "totalDownloadFileSizeString", "totalUploadFileCount", "transformationParallel", "transformationSummary", "inProgress", "label", "filterQuery", "emailRecipientUids", "pipelineId", "pipelineName", "pipelineRunId", "pipelineStep", "operatesOn", "files"]
 
     @validator('upload_type')
     def upload_type_validate_enum(cls, v):
         if v not in ('dataset', 'project'):
             raise ValueError("must validate the enum values ('dataset', 'project')")
         return v
 
@@ -137,14 +139,16 @@
             "project_name": obj.get("projectName"),
             "transformation_block_id": obj.get("transformationBlockId"),
             "builtin_transformation_block": obj.get("builtinTransformationBlock"),
             "transformation_block_name": obj.get("transformationBlockName"),
             "category": obj.get("category"),
             "created": obj.get("created"),
             "output_dataset_name": obj.get("outputDatasetName"),
+            "output_dataset_bucket_id": obj.get("outputDatasetBucketId"),
+            "output_dataset_bucket_path": obj.get("outputDatasetBucketPath"),
             "total_download_file_count": obj.get("totalDownloadFileCount"),
             "total_download_file_size": obj.get("totalDownloadFileSize"),
             "total_download_file_size_string": obj.get("totalDownloadFileSizeString"),
             "total_upload_file_count": obj.get("totalUploadFileCount"),
             "transformation_parallel": obj.get("transformationParallel"),
             "transformation_summary": OrganizationCreateProjectTransformationSummary.from_dict(obj.get("transformationSummary")) if obj.get("transformationSummary") is not None else None,
             "in_progress": obj.get("inProgress"),
```

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/organization_create_project_with_files_all_of.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/organization_create_project_with_files_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/organization_create_project_with_files_all_of_files.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/organization_create_project_with_files_all_of_files.py`

 * *Files 7% similar despite different names*

```diff
@@ -24,15 +24,16 @@
 class OrganizationCreateProjectWithFilesAllOfFiles(BaseModel):
     id: StrictInt = ...
     file_name: StrictStr = Field(..., alias="fileName")
     data_item_id: StrictInt = Field(..., alias="dataItemId")
     data_item_name: StrictStr = Field(..., alias="dataItemName")
     transformation_job_id: Optional[StrictInt] = Field(None, alias="transformationJobId")
     transformation_job_status: TransformationJobStatusEnum = Field(..., alias="transformationJobStatus")
-    __properties = ["id", "fileName", "dataItemId", "dataItemName", "transformationJobId", "transformationJobStatus"]
+    link_to_data_item: StrictStr = Field(..., alias="linkToDataItem")
+    __properties = ["id", "fileName", "dataItemId", "dataItemName", "transformationJobId", "transformationJobStatus", "linkToDataItem"]
 
     class Config:
         allow_population_by_field_name = True
         validate_assignment = False
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
@@ -66,11 +67,12 @@
 
         _obj = OrganizationCreateProjectWithFilesAllOfFiles.construct(**{
             "id": obj.get("id"),
             "file_name": obj.get("fileName"),
             "data_item_id": obj.get("dataItemId"),
             "data_item_name": obj.get("dataItemName"),
             "transformation_job_id": obj.get("transformationJobId"),
-            "transformation_job_status": obj.get("transformationJobStatus")
+            "transformation_job_status": obj.get("transformationJobStatus"),
+            "link_to_data_item": obj.get("linkToDataItem")
         })
         return _obj
```

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/organization_data_item.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/organization_data_item.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/organization_data_item_files_inner.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/organization_data_item_files_inner.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/organization_dataset.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/user_experiment.py`

 * *Files 17% similar despite different names*

```diff
@@ -12,64 +12,62 @@
 
 from __future__ import annotations
 from inspect import getfullargspec
 import pprint
 import re  # noqa: F401
 import json
 
-from datetime import datetime
-from typing import List, Optional
-from pydantic import BaseModel, Field, StrictInt, StrictStr
-
-class OrganizationDataset(BaseModel):
-    dataset: StrictStr = ...
-    last_file_created: datetime = Field(..., alias="lastFileCreated")
-    total_file_size: StrictInt = Field(..., alias="totalFileSize")
-    total_file_count: StrictInt = Field(..., alias="totalFileCount")
-    tags: List[StrictStr] = ...
-    category: Optional[StrictStr] = None
-    __properties = ["dataset", "lastFileCreated", "totalFileSize", "totalFileCount", "tags", "category"]
+
+from typing import Optional
+from pydantic import BaseModel, Field, StrictBool, StrictStr
+
+class UserExperiment(BaseModel):
+    type: StrictStr = ...
+    title: StrictStr = ...
+    help: Optional[StrictStr] = None
+    enabled: StrictBool = ...
+    show_to_user: StrictBool = Field(..., alias="showToUser")
+    __properties = ["type", "title", "help", "enabled", "showToUser"]
 
     class Config:
         allow_population_by_field_name = True
         validate_assignment = False
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
         return pprint.pformat(self.dict(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> OrganizationDataset:
-        """Create an instance of OrganizationDataset from a JSON string"""
+    def from_json(cls, json_str: str) -> UserExperiment:
+        """Create an instance of UserExperiment from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self):
         """Returns the dictionary representation of the model using alias"""
         _dict = self.dict(by_alias=True,
                           exclude={
                           },
                           exclude_none=True)
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> OrganizationDataset:
-        """Create an instance of OrganizationDataset from a dict"""
+    def from_dict(cls, obj: dict) -> UserExperiment:
+        """Create an instance of UserExperiment from a dict"""
         if obj is None:
             return None
 
         if type(obj) is not dict:
-            return OrganizationDataset.construct(**obj)
+            return UserExperiment.construct(**obj)
 
-        _obj = OrganizationDataset.construct(**{
-            "dataset": obj.get("dataset"),
-            "last_file_created": obj.get("lastFileCreated"),
-            "total_file_size": obj.get("totalFileSize"),
-            "total_file_count": obj.get("totalFileCount"),
-            "tags": obj.get("tags"),
-            "category": obj.get("category")
+        _obj = UserExperiment.construct(**{
+            "type": obj.get("type"),
+            "title": obj.get("title"),
+            "help": obj.get("help"),
+            "enabled": obj.get("enabled"),
+            "show_to_user": obj.get("showToUser")
         })
         return _obj
```

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/organization_deploy_block.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/organization_deploy_block.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/organization_dsp_block.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/organization_dsp_block.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/organization_get_create_projects_response.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/organization_get_create_projects_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/organization_get_create_projects_response_all_of.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/organization_get_create_projects_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/organization_get_create_projects_response_all_of_jobs.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/organization_get_create_projects_response_all_of_jobs.py`

 * *Files 14% similar despite different names*

```diff
@@ -33,19 +33,21 @@
     project_id: Optional[StrictInt] = Field(None, alias="projectId")
     project_name: Optional[StrictStr] = Field(None, alias="projectName")
     transformation_block_id: Optional[StrictInt] = Field(None, alias="transformationBlockId")
     builtin_transformation_block: Optional[Dict[str, Any]] = Field(None, alias="builtinTransformationBlock")
     transformation_block_name: Optional[StrictStr] = Field(None, alias="transformationBlockName")
     created: datetime = ...
     output_dataset_name: Optional[StrictStr] = Field(None, alias="outputDatasetName")
+    output_dataset_bucket_id: Optional[StrictInt] = Field(None, alias="outputDatasetBucketId")
+    output_dataset_bucket_path: Optional[StrictStr] = Field(None, alias="outputDatasetBucketPath")
     total_download_file_count: StrictInt = Field(..., alias="totalDownloadFileCount")
     total_download_file_size: StrictInt = Field(..., alias="totalDownloadFileSize")
     total_download_file_size_string: StrictStr = Field(..., alias="totalDownloadFileSizeString")
     total_upload_file_count: Optional[StrictInt] = Field(None, alias="totalUploadFileCount")
-    __properties = ["id", "organizationId", "name", "uploadType", "transformJobStatus", "uploadJobId", "uploadJobStatus", "projectOwner", "projectId", "projectName", "transformationBlockId", "builtinTransformationBlock", "transformationBlockName", "created", "outputDatasetName", "totalDownloadFileCount", "totalDownloadFileSize", "totalDownloadFileSizeString", "totalUploadFileCount"]
+    __properties = ["id", "organizationId", "name", "uploadType", "transformJobStatus", "uploadJobId", "uploadJobStatus", "projectOwner", "projectId", "projectName", "transformationBlockId", "builtinTransformationBlock", "transformationBlockName", "created", "outputDatasetName", "outputDatasetBucketId", "outputDatasetBucketPath", "totalDownloadFileCount", "totalDownloadFileSize", "totalDownloadFileSizeString", "totalUploadFileCount"]
 
     @validator('upload_type')
     def upload_type_validate_enum(cls, v):
         if v not in ('dataset', 'project'):
             raise ValueError("must validate the enum values ('dataset', 'project')")
         return v
 
@@ -95,14 +97,16 @@
             "project_id": obj.get("projectId"),
             "project_name": obj.get("projectName"),
             "transformation_block_id": obj.get("transformationBlockId"),
             "builtin_transformation_block": obj.get("builtinTransformationBlock"),
             "transformation_block_name": obj.get("transformationBlockName"),
             "created": obj.get("created"),
             "output_dataset_name": obj.get("outputDatasetName"),
+            "output_dataset_bucket_id": obj.get("outputDatasetBucketId"),
+            "output_dataset_bucket_path": obj.get("outputDatasetBucketPath"),
             "total_download_file_count": obj.get("totalDownloadFileCount"),
             "total_download_file_size": obj.get("totalDownloadFileSize"),
             "total_download_file_size_string": obj.get("totalDownloadFileSizeString"),
             "total_upload_file_count": obj.get("totalUploadFileCount")
         })
         return _obj
```

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/organization_info_response.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/organization_info_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/organization_info_response_all_of.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/organization_info_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/organization_info_response_all_of_default_compute_limits.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/organization_info_response_all_of_default_compute_limits.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/organization_info_response_all_of_entitlement_limits.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/organization_info_response_all_of_entitlement_limits.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/organization_metrics_response.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/organization_metrics_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/organization_metrics_response_all_of.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/organization_metrics_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/organization_metrics_response_all_of_metrics.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/organization_metrics_response_all_of_metrics.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/organization_pipeline.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/organization_pipeline.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/organization_pipeline_feeding_into_dataset.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/organization_pipeline_feeding_into_dataset.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/organization_pipeline_feeding_into_project.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/organization_pipeline_feeding_into_project.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/organization_pipeline_item_count.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/organization_pipeline_item_count.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/organization_pipeline_run.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/organization_pipeline_run.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/organization_pipeline_run_step.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/organization_pipeline_step.py`

 * *Files 7% similar despite different names*

```diff
@@ -15,32 +15,33 @@
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Any, Dict, Optional
 from pydantic import BaseModel, Field, StrictInt, StrictStr, validator
-from edgeimpulse_api.models.organization_create_project import OrganizationCreateProject
 
-class OrganizationPipelineRunStep(BaseModel):
+class OrganizationPipelineStep(BaseModel):
     name: StrictStr = ...
-    transformation_job: Optional[OrganizationCreateProject] = Field(None, alias="transformationJob")
     filter: Optional[StrictStr] = None
     upload_type: Optional[StrictStr] = Field(None, alias="uploadType")
     project_id: Optional[StrictInt] = Field(None, alias="projectId")
     new_project_name: Optional[StrictStr] = Field(None, alias="newProjectName")
     project_api_key: Optional[StrictStr] = Field(None, alias="projectApiKey")
     project_hmac_key: Optional[StrictStr] = Field(None, alias="projectHmacKey")
     transformation_block_id: Optional[StrictInt] = Field(None, alias="transformationBlockId")
     builtin_transformation_block: Optional[Dict[str, Any]] = Field(None, alias="builtinTransformationBlock")
     category: Optional[StrictStr] = None
     output_dataset_name: Optional[StrictStr] = Field(None, alias="outputDatasetName")
+    output_dataset_bucket_id: Optional[StrictInt] = Field(None, alias="outputDatasetBucketId")
+    output_dataset_bucket_path: Optional[StrictStr] = Field(None, alias="outputDatasetBucketPath")
     label: Optional[StrictStr] = None
+    transformation_parallel: Optional[StrictInt] = Field(None, alias="transformationParallel")
     extra_cli_arguments: Optional[StrictStr] = Field(None, alias="extraCliArguments")
-    __properties = ["name", "transformationJob", "filter", "uploadType", "projectId", "newProjectName", "projectApiKey", "projectHmacKey", "transformationBlockId", "builtinTransformationBlock", "category", "outputDatasetName", "label", "extraCliArguments"]
+    __properties = ["name", "filter", "uploadType", "projectId", "newProjectName", "projectApiKey", "projectHmacKey", "transformationBlockId", "builtinTransformationBlock", "category", "outputDatasetName", "outputDatasetBucketId", "outputDatasetBucketPath", "label", "transformationParallel", "extraCliArguments"]
 
     @validator('upload_type')
     def upload_type_validate_enum(cls, v):
         if v is None:
             return v
 
         if v not in ('project', 'dataset'):
@@ -65,49 +66,48 @@
         return pprint.pformat(self.dict(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> OrganizationPipelineRunStep:
-        """Create an instance of OrganizationPipelineRunStep from a JSON string"""
+    def from_json(cls, json_str: str) -> OrganizationPipelineStep:
+        """Create an instance of OrganizationPipelineStep from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self):
         """Returns the dictionary representation of the model using alias"""
         _dict = self.dict(by_alias=True,
                           exclude={
                           },
                           exclude_none=True)
-        # override the default output from pydantic by calling `to_dict()` of transformation_job
-        if self.transformation_job:
-            _dict['transformationJob'] = self.transformation_job.to_dict()
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> OrganizationPipelineRunStep:
-        """Create an instance of OrganizationPipelineRunStep from a dict"""
+    def from_dict(cls, obj: dict) -> OrganizationPipelineStep:
+        """Create an instance of OrganizationPipelineStep from a dict"""
         if obj is None:
             return None
 
         if type(obj) is not dict:
-            return OrganizationPipelineRunStep.construct(**obj)
+            return OrganizationPipelineStep.construct(**obj)
 
-        _obj = OrganizationPipelineRunStep.construct(**{
+        _obj = OrganizationPipelineStep.construct(**{
             "name": obj.get("name"),
-            "transformation_job": OrganizationCreateProject.from_dict(obj.get("transformationJob")) if obj.get("transformationJob") is not None else None,
             "filter": obj.get("filter"),
             "upload_type": obj.get("uploadType"),
             "project_id": obj.get("projectId"),
             "new_project_name": obj.get("newProjectName"),
             "project_api_key": obj.get("projectApiKey"),
             "project_hmac_key": obj.get("projectHmacKey"),
             "transformation_block_id": obj.get("transformationBlockId"),
             "builtin_transformation_block": obj.get("builtinTransformationBlock"),
             "category": obj.get("category"),
             "output_dataset_name": obj.get("outputDatasetName"),
+            "output_dataset_bucket_id": obj.get("outputDatasetBucketId"),
+            "output_dataset_bucket_path": obj.get("outputDatasetBucketPath"),
             "label": obj.get("label"),
+            "transformation_parallel": obj.get("transformationParallel"),
             "extra_cli_arguments": obj.get("extraCliArguments")
         })
         return _obj
```

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/organization_pipeline_step.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/update_organization_transformation_block_request.py`

 * *Files 21% similar despite different names*

```diff
@@ -13,50 +13,40 @@
 from __future__ import annotations
 from inspect import getfullargspec
 import pprint
 import re  # noqa: F401
 import json
 
 
-from typing import Any, Dict, Optional
-from pydantic import BaseModel, Field, StrictInt, StrictStr, validator
+from typing import List, Optional
+from pydantic import BaseModel, Field, StrictBool, StrictInt, StrictStr, validator
+from edgeimpulse_api.models.transformation_block_additional_mount_point import TransformationBlockAdditionalMountPoint
+
+class UpdateOrganizationTransformationBlockRequest(BaseModel):
+    name: Optional[StrictStr] = None
+    docker_container: Optional[StrictStr] = Field(None, alias="dockerContainer")
+    ind_metadata: Optional[StrictBool] = Field(None, alias="indMetadata", description="Whether to pass the `--metadata` parameter to the container.")
+    description: Optional[StrictStr] = None
+    cli_arguments: Optional[StrictStr] = Field(None, alias="cliArguments")
+    requests_cpu: Optional[float] = Field(None, alias="requestsCpu")
+    requests_memory: Optional[StrictInt] = Field(None, alias="requestsMemory")
+    limits_cpu: Optional[float] = Field(None, alias="limitsCpu")
+    limits_memory: Optional[StrictInt] = Field(None, alias="limitsMemory")
+    additional_mount_points: Optional[List[TransformationBlockAdditionalMountPoint]] = Field(None, alias="additionalMountPoints")
+    operates_on: Optional[StrictStr] = Field(None, alias="operatesOn")
+    allow_extra_cli_arguments: Optional[StrictBool] = Field(None, alias="allowExtraCliArguments")
+    __properties = ["name", "dockerContainer", "indMetadata", "description", "cliArguments", "requestsCpu", "requestsMemory", "limitsCpu", "limitsMemory", "additionalMountPoints", "operatesOn", "allowExtraCliArguments"]
 
-class OrganizationPipelineStep(BaseModel):
-    name: StrictStr = ...
-    filter: Optional[StrictStr] = None
-    upload_type: Optional[StrictStr] = Field(None, alias="uploadType")
-    project_id: Optional[StrictInt] = Field(None, alias="projectId")
-    new_project_name: Optional[StrictStr] = Field(None, alias="newProjectName")
-    project_api_key: Optional[StrictStr] = Field(None, alias="projectApiKey")
-    project_hmac_key: Optional[StrictStr] = Field(None, alias="projectHmacKey")
-    transformation_block_id: Optional[StrictInt] = Field(None, alias="transformationBlockId")
-    builtin_transformation_block: Optional[Dict[str, Any]] = Field(None, alias="builtinTransformationBlock")
-    category: Optional[StrictStr] = None
-    output_dataset_name: Optional[StrictStr] = Field(None, alias="outputDatasetName")
-    label: Optional[StrictStr] = None
-    transformation_parallel: Optional[StrictInt] = Field(None, alias="transformationParallel")
-    extra_cli_arguments: Optional[StrictStr] = Field(None, alias="extraCliArguments")
-    __properties = ["name", "filter", "uploadType", "projectId", "newProjectName", "projectApiKey", "projectHmacKey", "transformationBlockId", "builtinTransformationBlock", "category", "outputDatasetName", "label", "transformationParallel", "extraCliArguments"]
-
-    @validator('upload_type')
-    def upload_type_validate_enum(cls, v):
-        if v is None:
-            return v
-
-        if v not in ('project', 'dataset'):
-            raise ValueError("must validate the enum values ('project', 'dataset')")
-        return v
-
-    @validator('category')
-    def category_validate_enum(cls, v):
+    @validator('operates_on')
+    def operates_on_validate_enum(cls, v):
         if v is None:
             return v
 
-        if v not in ('training', 'testing', 'split'):
-            raise ValueError("must validate the enum values ('training', 'testing', 'split')")
+        if v not in ('file', 'dataitem', 'standalone'):
+            raise ValueError("must validate the enum values ('file', 'dataitem', 'standalone')")
         return v
 
     class Config:
         allow_population_by_field_name = True
         validate_assignment = False
 
     def to_str(self) -> str:
@@ -64,46 +54,51 @@
         return pprint.pformat(self.dict(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> OrganizationPipelineStep:
-        """Create an instance of OrganizationPipelineStep from a JSON string"""
+    def from_json(cls, json_str: str) -> UpdateOrganizationTransformationBlockRequest:
+        """Create an instance of UpdateOrganizationTransformationBlockRequest from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self):
         """Returns the dictionary representation of the model using alias"""
         _dict = self.dict(by_alias=True,
                           exclude={
                           },
                           exclude_none=True)
+        # override the default output from pydantic by calling `to_dict()` of each item in additional_mount_points (list)
+        _items = []
+        if self.additional_mount_points:
+            for _item in self.additional_mount_points:
+                if _item:
+                    _items.append(_item.to_dict())
+            _dict['additionalMountPoints'] = _items
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> OrganizationPipelineStep:
-        """Create an instance of OrganizationPipelineStep from a dict"""
+    def from_dict(cls, obj: dict) -> UpdateOrganizationTransformationBlockRequest:
+        """Create an instance of UpdateOrganizationTransformationBlockRequest from a dict"""
         if obj is None:
             return None
 
         if type(obj) is not dict:
-            return OrganizationPipelineStep.construct(**obj)
+            return UpdateOrganizationTransformationBlockRequest.construct(**obj)
 
-        _obj = OrganizationPipelineStep.construct(**{
+        _obj = UpdateOrganizationTransformationBlockRequest.construct(**{
             "name": obj.get("name"),
-            "filter": obj.get("filter"),
-            "upload_type": obj.get("uploadType"),
-            "project_id": obj.get("projectId"),
-            "new_project_name": obj.get("newProjectName"),
-            "project_api_key": obj.get("projectApiKey"),
-            "project_hmac_key": obj.get("projectHmacKey"),
-            "transformation_block_id": obj.get("transformationBlockId"),
-            "builtin_transformation_block": obj.get("builtinTransformationBlock"),
-            "category": obj.get("category"),
-            "output_dataset_name": obj.get("outputDatasetName"),
-            "label": obj.get("label"),
-            "transformation_parallel": obj.get("transformationParallel"),
-            "extra_cli_arguments": obj.get("extraCliArguments")
+            "docker_container": obj.get("dockerContainer"),
+            "ind_metadata": obj.get("indMetadata"),
+            "description": obj.get("description"),
+            "cli_arguments": obj.get("cliArguments"),
+            "requests_cpu": obj.get("requestsCpu"),
+            "requests_memory": obj.get("requestsMemory"),
+            "limits_cpu": obj.get("limitsCpu"),
+            "limits_memory": obj.get("limitsMemory"),
+            "additional_mount_points": [TransformationBlockAdditionalMountPoint.from_dict(_item) for _item in obj.get("additionalMountPoints")] if obj.get("additionalMountPoints") is not None else None,
+            "operates_on": obj.get("operatesOn"),
+            "allow_extra_cli_arguments": obj.get("allowExtraCliArguments")
         })
         return _obj
```

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/organization_projects_data_batch_disable_response.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/organization_projects_data_batch_disable_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/organization_projects_data_batch_enable_response.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/organization_projects_data_batch_enable_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/organization_projects_data_batch_request.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/organization_projects_data_batch_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/organization_transfer_learning_block.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/organization_transfer_learning_block.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/organization_transfer_learning_operates_on.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/organization_transfer_learning_operates_on.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/organization_transformation_block.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/organization_transformation_block.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/organization_update_pipeline_body.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/organization_update_pipeline_body.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/organization_user.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/organization_user.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/performance_calibration_detection.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/performance_calibration_detection.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/performance_calibration_false_positive.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/performance_calibration_false_positive.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/performance_calibration_ground_truth.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/performance_calibration_ground_truth.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/performance_calibration_ground_truth_samples_inner.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/performance_calibration_ground_truth_samples_inner.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/performance_calibration_parameter_set.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/performance_calibration_parameter_set.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/performance_calibration_parameter_set_aggregate_stats.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/performance_calibration_parameter_set_aggregate_stats.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/performance_calibration_parameter_set_stats_inner.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/performance_calibration_parameter_set_stats_inner.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/performance_calibration_parameters.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/performance_calibration_parameters.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/performance_calibration_parameters_standard.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/performance_calibration_parameters_standard.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/performance_calibration_raw_detection.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/performance_calibration_raw_detection.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/performance_calibration_save_parameter_set_request.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/performance_calibration_save_parameter_set_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/performance_calibration_upload_labeled_audio_response.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/performance_calibration_upload_labeled_audio_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/performance_calibration_upload_labeled_audio_response_all_of.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/performance_calibration_upload_labeled_audio_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/permission.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/permission.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/portal_file.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/portal_file.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/portal_info_response.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/portal_info_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/pretrained_model_tensor.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/pretrained_model_tensor.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/profile_model_info.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/profile_model_info.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/profile_model_info_memory.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/profile_model_info_memory.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/profile_model_info_memory_eon.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/profile_model_info_memory_eon.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/profile_model_info_memory_tflite.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/profile_model_info_memory_tflite.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/profile_model_table.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/profile_model_table.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/profile_model_table_mcu.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/profile_model_table_mcu.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/profile_model_table_mcu_memory.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/profile_model_table_mcu_memory.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/profile_model_table_mpu.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/profile_model_table_mpu.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/profile_tf_lite_request.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/profile_tf_lite_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/profile_tf_lite_response.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/profile_tf_lite_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/project.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/project.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/project_collaborator.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/project_collaborator.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/project_collaborator_all_of.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/project_collaborator_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/project_data_axes_summary_response.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/project_data_axes_summary_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/project_data_axes_summary_response_all_of.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/project_data_axes_summary_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/project_data_interval_response.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/project_data_interval_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/project_data_interval_response_all_of.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/project_data_interval_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/project_data_summary.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/project_data_summary.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/project_deployment_target.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/project_deployment_target.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/project_deployment_target_all_of.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/project_deployment_target_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/project_deployment_targets_response.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/project_deployment_targets_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/project_deployment_targets_response_all_of.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/project_deployment_targets_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/project_downloads_response.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/project_downloads_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/project_downloads_response_all_of.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/project_downloads_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/project_info_response.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/project_info_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/project_info_response_all_of.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/project_info_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/project_info_response_all_of_acquisition_settings.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/project_info_response_all_of_acquisition_settings.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/project_info_response_all_of_compute_time.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/project_info_response_all_of_compute_time.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/project_info_response_all_of_data_summary_per_category.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/project_info_response_all_of_data_summary_per_category.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/project_info_response_all_of_deploy_settings.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/project_info_response_all_of_deploy_settings.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/project_info_response_all_of_experiments.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/project_info_response_all_of_experiments.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/project_info_response_all_of_impulse.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/project_info_response_all_of_impulse.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/project_info_response_all_of_performance.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/project_info_response_all_of_performance.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/project_info_response_all_of_readme.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/project_info_response_all_of_readme.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/project_info_response_all_of_show_getting_started_wizard.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/project_info_response_all_of_show_getting_started_wizard.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/project_info_response_all_of_urls.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/project_info_response_all_of_urls.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/project_info_summary_response.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/project_info_summary_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/project_info_summary_response_all_of.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/project_info_summary_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/project_private_data.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/project_private_data.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/project_public_data.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/project_public_data.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/project_public_data_readme.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/project_public_data_readme.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/project_sample_metadata.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/project_sample_metadata.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/project_training_data_summary_response.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/project_training_data_summary_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/project_training_data_summary_response_all_of.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/project_training_data_summary_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/project_version_request.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/project_version_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/raw_sample_data.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/raw_sample_data.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/raw_sample_payload.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/raw_sample_payload.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/rebalance_dataset_response.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/rebalance_dataset_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/remove_collaborator_request.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/remove_collaborator_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/remove_member_request.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/remove_member_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/rename_device_request.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/rename_device_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/rename_portal_file_request.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/rename_portal_file_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/rename_sample_request.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/rename_sample_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/request_reset_password_request.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/request_reset_password_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/reset_password_request.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/reset_password_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/restore_project_from_public_request.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/restore_project_from_public_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/restore_project_request.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/restore_project_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/run_organization_pipeline_response.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/run_organization_pipeline_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/run_organization_pipeline_response_all_of.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/run_organization_pipeline_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/sample.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/sample.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/sample_bounding_boxes_request.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/sample_bounding_boxes_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/sample_metadata.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/sample_metadata.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/save_pretrained_model_request.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/save_pretrained_model_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/score_trial_response.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/score_trial_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/score_trial_response_all_of.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/score_trial_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/score_trial_response_all_of_latency.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/score_trial_response_all_of_latency.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/score_trial_response_all_of_ram.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/score_trial_response_all_of_ram.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/segment_sample_request.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/segment_sample_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/segment_sample_request_segments_inner.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/segment_sample_request_segments_inner.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/send_user_feedback_request.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/send_user_feedback_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/sensor.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/sensor.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/set_anomaly_parameter_request.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/set_anomaly_parameter_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/set_keras_parameter_request.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/set_keras_parameter_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/set_member_datasets_request.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/set_member_datasets_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/set_member_role_request.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/set_member_role_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/set_optimize_space_request.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/set_optimize_space_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/set_optimize_space_request_all_of.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/set_optimize_space_request_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/set_organization_data_dataset_request.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/set_organization_data_dataset_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/set_project_compute_time_request.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/set_project_compute_time_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/set_project_dsp_file_size_request.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/set_project_dsp_file_size_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/set_sample_metadata_request.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/set_sample_metadata_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/set_syntiant_posterior_request.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/set_syntiant_posterior_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/set_user_password_request.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/set_user_password_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/socket_token_response.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/socket_token_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/socket_token_response_all_of.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/socket_token_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/socket_token_response_all_of_token.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/socket_token_response_all_of_token.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/split_sample_in_frames_request.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/split_sample_in_frames_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/staff_info.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/staff_info.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/start_job_response.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/start_job_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/start_job_response_all_of.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/start_job_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/start_performance_calibration_request.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/start_performance_calibration_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/start_sampling_request.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/start_sampling_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/start_sampling_response.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/start_sampling_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/start_sampling_response_all_of.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/start_sampling_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/start_training_request_anomaly.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/start_training_request_anomaly.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/store_segment_length_request.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/store_segment_length_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/structured_classify_result.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/structured_classify_result.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/test_pretrained_model_request.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/test_pretrained_model_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/test_pretrained_model_response.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/test_pretrained_model_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/test_pretrained_model_response_all_of.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/test_pretrained_model_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/theme.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/theme.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/theme_colors.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/theme_colors.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/theme_favicon.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/theme_favicon.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/theme_logos.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/theme_logos.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,15 +24,16 @@
     primary: Optional[StrictStr] = None
     primary_png: Optional[StrictStr] = Field(None, alias="primaryPng")
     primary_white: Optional[StrictStr] = Field(None, alias="primaryWhite")
     login_logo: Optional[StrictStr] = Field(None, alias="loginLogo")
     login_logo_white: Optional[StrictStr] = Field(None, alias="loginLogoWhite")
     mark: Optional[StrictStr] = None
     mark_white: Optional[StrictStr] = Field(None, alias="markWhite")
-    __properties = ["primary", "primaryPng", "primaryWhite", "loginLogo", "loginLogoWhite", "mark", "markWhite"]
+    device_logo: Optional[StrictStr] = Field(None, alias="deviceLogo")
+    __properties = ["primary", "primaryPng", "primaryWhite", "loginLogo", "loginLogoWhite", "mark", "markWhite", "deviceLogo"]
 
     class Config:
         allow_population_by_field_name = True
         validate_assignment = False
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
@@ -67,11 +68,12 @@
         _obj = ThemeLogos.construct(**{
             "primary": obj.get("primary"),
             "primary_png": obj.get("primaryPng"),
             "primary_white": obj.get("primaryWhite"),
             "login_logo": obj.get("loginLogo"),
             "login_logo_white": obj.get("loginLogoWhite"),
             "mark": obj.get("mark"),
-            "mark_white": obj.get("markWhite")
+            "mark_white": obj.get("markWhite"),
+            "device_logo": obj.get("deviceLogo")
         })
         return _obj
```

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/third_party_auth.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/third_party_auth.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/track_objects_request.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/track_objects_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/track_objects_response.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/track_objects_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/track_objects_response_all_of.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/track_objects_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/transfer_learning_model.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/transfer_learning_model.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/transfer_ownership_organization_request.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/transfer_ownership_organization_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/transformation_block_additional_mount_point.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/transformation_block_additional_mount_point.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/transformation_job_status_enum.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/transformation_job_status_enum.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/tuner_create_trial_impulse.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/tuner_create_trial_impulse.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/tuner_space_impulse.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/tuner_space_impulse.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/tuner_trial.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/tuner_trial.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/tuner_trial_blocks_inner.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/tuner_trial_blocks_inner.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/update_job_request.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/update_job_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/update_organization_add_collaborator_request.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/update_organization_add_collaborator_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/update_organization_bucket_request.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/update_organization_bucket_request.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,22 +17,21 @@
 import json
 
 
 from typing import Optional
 from pydantic import BaseModel, Field, StrictStr
 
 class UpdateOrganizationBucketRequest(BaseModel):
-    name: Optional[StrictStr] = Field(None, description="S3 bucket description")
     access_key: Optional[StrictStr] = Field(None, alias="accessKey", description="S3 access key")
     secret_key: Optional[StrictStr] = Field(None, alias="secretKey", description="S3 secret key")
     endpoint: Optional[StrictStr] = Field(None, description="S3 endpoint")
     bucket: Optional[StrictStr] = Field(None, description="S3 bucket")
-    prefix: Optional[StrictStr] = Field(None, description="Prefix within the bucket")
     region: Optional[StrictStr] = Field(None, description="S3 region")
-    __properties = ["name", "accessKey", "secretKey", "endpoint", "bucket", "prefix", "region"]
+    check_connectivity_prefix: Optional[StrictStr] = Field(None, alias="checkConnectivityPrefix", description="Set this if you don't have access to the root of this bucket. Only used to verify connectivity to this bucket.")
+    __properties = ["accessKey", "secretKey", "endpoint", "bucket", "region", "checkConnectivityPrefix"]
 
     class Config:
         allow_population_by_field_name = True
         validate_assignment = False
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
@@ -61,17 +60,16 @@
         if obj is None:
             return None
 
         if type(obj) is not dict:
             return UpdateOrganizationBucketRequest.construct(**obj)
 
         _obj = UpdateOrganizationBucketRequest.construct(**{
-            "name": obj.get("name"),
             "access_key": obj.get("accessKey"),
             "secret_key": obj.get("secretKey"),
             "endpoint": obj.get("endpoint"),
             "bucket": obj.get("bucket"),
-            "prefix": obj.get("prefix"),
-            "region": obj.get("region")
+            "region": obj.get("region"),
+            "check_connectivity_prefix": obj.get("checkConnectivityPrefix")
         })
         return _obj
```

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/update_organization_create_empty_project_request.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/update_organization_create_empty_project_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/update_organization_create_project_request.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/update_organization_create_project_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/update_organization_data_item_request.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/update_organization_data_item_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/update_organization_dataset_request.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/update_project_tags_request.py`

 * *Files 15% similar despite different names*

```diff
@@ -13,55 +13,53 @@
 from __future__ import annotations
 from inspect import getfullargspec
 import pprint
 import re  # noqa: F401
 import json
 
 
-from typing import List, Optional
+from typing import List
 from pydantic import BaseModel, StrictStr
 
-class UpdateOrganizationDatasetRequest(BaseModel):
-    tags: Optional[List[StrictStr]] = None
-    category: Optional[StrictStr] = None
-    __properties = ["tags", "category"]
+class UpdateProjectTagsRequest(BaseModel):
+    tags: List[StrictStr] = ...
+    __properties = ["tags"]
 
     class Config:
         allow_population_by_field_name = True
         validate_assignment = False
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
         return pprint.pformat(self.dict(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> UpdateOrganizationDatasetRequest:
-        """Create an instance of UpdateOrganizationDatasetRequest from a JSON string"""
+    def from_json(cls, json_str: str) -> UpdateProjectTagsRequest:
+        """Create an instance of UpdateProjectTagsRequest from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self):
         """Returns the dictionary representation of the model using alias"""
         _dict = self.dict(by_alias=True,
                           exclude={
                           },
                           exclude_none=True)
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> UpdateOrganizationDatasetRequest:
-        """Create an instance of UpdateOrganizationDatasetRequest from a dict"""
+    def from_dict(cls, obj: dict) -> UpdateProjectTagsRequest:
+        """Create an instance of UpdateProjectTagsRequest from a dict"""
         if obj is None:
             return None
 
         if type(obj) is not dict:
-            return UpdateOrganizationDatasetRequest.construct(**obj)
+            return UpdateProjectTagsRequest.construct(**obj)
 
-        _obj = UpdateOrganizationDatasetRequest.construct(**{
-            "tags": obj.get("tags"),
-            "category": obj.get("category")
+        _obj = UpdateProjectTagsRequest.construct(**{
+            "tags": obj.get("tags")
         })
         return _obj
```

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/update_organization_dsp_block_request.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/update_organization_dsp_block_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/update_organization_portal_response.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/update_organization_portal_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/update_organization_portal_response_all_of.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/update_organization_portal_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/update_organization_request.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/update_organization_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/update_organization_transfer_learning_block_request.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/update_organization_transfer_learning_block_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/update_project_request.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/update_project_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/update_project_tags_request.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/verify_reset_password_request.py`

 * *Files 13% similar despite different names*

```diff
@@ -13,53 +13,55 @@
 from __future__ import annotations
 from inspect import getfullargspec
 import pprint
 import re  # noqa: F401
 import json
 
 
-from typing import List
+
 from pydantic import BaseModel, StrictStr
 
-class UpdateProjectTagsRequest(BaseModel):
-    tags: List[StrictStr] = ...
-    __properties = ["tags"]
+class VerifyResetPasswordRequest(BaseModel):
+    email: StrictStr = ...
+    code: StrictStr = ...
+    __properties = ["email", "code"]
 
     class Config:
         allow_population_by_field_name = True
         validate_assignment = False
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
         return pprint.pformat(self.dict(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> UpdateProjectTagsRequest:
-        """Create an instance of UpdateProjectTagsRequest from a JSON string"""
+    def from_json(cls, json_str: str) -> VerifyResetPasswordRequest:
+        """Create an instance of VerifyResetPasswordRequest from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self):
         """Returns the dictionary representation of the model using alias"""
         _dict = self.dict(by_alias=True,
                           exclude={
                           },
                           exclude_none=True)
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> UpdateProjectTagsRequest:
-        """Create an instance of UpdateProjectTagsRequest from a dict"""
+    def from_dict(cls, obj: dict) -> VerifyResetPasswordRequest:
+        """Create an instance of VerifyResetPasswordRequest from a dict"""
         if obj is None:
             return None
 
         if type(obj) is not dict:
-            return UpdateProjectTagsRequest.construct(**obj)
+            return VerifyResetPasswordRequest.construct(**obj)
 
-        _obj = UpdateProjectTagsRequest.construct(**{
-            "tags": obj.get("tags")
+        _obj = VerifyResetPasswordRequest.construct(**{
+            "email": obj.get("email"),
+            "code": obj.get("code")
         })
         return _obj
```

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/update_theme_colors_request.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/update_theme_colors_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/update_theme_logos_request.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/update_theme_logos_request.py`

 * *Files 5% similar despite different names*

```diff
@@ -23,15 +23,16 @@
 class UpdateThemeLogosRequest(BaseModel):
     primary: Optional[StrictStr] = Field(None, description="Primary logo URL")
     primary_white: Optional[StrictStr] = Field(None, alias="primaryWhite", description="Primary logo for dark background URL")
     login: Optional[StrictStr] = Field(None, description="Login logo URL")
     login_white: Optional[StrictStr] = Field(None, alias="loginWhite", description="Login logo for dark background URL")
     mark: Optional[StrictStr] = Field(None, description="Mark URL")
     mark_white: Optional[StrictStr] = Field(None, alias="markWhite", description="Mark for dark background URL")
-    __properties = ["primary", "primaryWhite", "login", "loginWhite", "mark", "markWhite"]
+    device_logo: Optional[StrictStr] = Field(None, alias="deviceLogo", description="Device logo URL")
+    __properties = ["primary", "primaryWhite", "login", "loginWhite", "mark", "markWhite", "deviceLogo"]
 
     class Config:
         allow_population_by_field_name = True
         validate_assignment = False
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
@@ -65,11 +66,12 @@
 
         _obj = UpdateThemeLogosRequest.construct(**{
             "primary": obj.get("primary"),
             "primary_white": obj.get("primaryWhite"),
             "login": obj.get("login"),
             "login_white": obj.get("loginWhite"),
             "mark": obj.get("mark"),
-            "mark_white": obj.get("markWhite")
+            "mark_white": obj.get("markWhite"),
+            "device_logo": obj.get("deviceLogo")
         })
         return _obj
```

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/update_third_party_auth_request.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/update_third_party_auth_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/update_user_request.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/update_user_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/update_version_request.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/update_version_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/update_whitelabel_deployment_targets_request.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/update_whitelabel_deployment_targets_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/upload_asset_response.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/upload_asset_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/upload_asset_response_all_of.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/upload_asset_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/upload_readme_image_response.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/upload_readme_image_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/upload_user_photo_response.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/upload_user_photo_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/upload_user_photo_response_all_of.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/upload_user_photo_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/user.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/user.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/user_by_third_party_activation_request.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/user_by_third_party_activation_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/user_experiment.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/verify_dsp_block_url_response_all_of_block.py`

 * *Files 17% similar despite different names*

```diff
@@ -13,61 +13,61 @@
 from __future__ import annotations
 from inspect import getfullargspec
 import pprint
 import re  # noqa: F401
 import json
 
 
-from typing import Optional
-from pydantic import BaseModel, Field, StrictBool, StrictStr
 
-class UserExperiment(BaseModel):
-    type: StrictStr = ...
+from pydantic import BaseModel, Field, StrictInt, StrictStr
+
+class VerifyDspBlockUrlResponseAllOfBlock(BaseModel):
     title: StrictStr = ...
-    help: Optional[StrictStr] = None
-    enabled: StrictBool = ...
-    show_to_user: StrictBool = Field(..., alias="showToUser")
-    __properties = ["type", "title", "help", "enabled", "showToUser"]
+    author: StrictStr = ...
+    description: StrictStr = ...
+    name: StrictStr = ...
+    latest_implementation_version: StrictInt = Field(..., alias="latestImplementationVersion")
+    __properties = ["title", "author", "description", "name", "latestImplementationVersion"]
 
     class Config:
         allow_population_by_field_name = True
         validate_assignment = False
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
         return pprint.pformat(self.dict(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> UserExperiment:
-        """Create an instance of UserExperiment from a JSON string"""
+    def from_json(cls, json_str: str) -> VerifyDspBlockUrlResponseAllOfBlock:
+        """Create an instance of VerifyDspBlockUrlResponseAllOfBlock from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self):
         """Returns the dictionary representation of the model using alias"""
         _dict = self.dict(by_alias=True,
                           exclude={
                           },
                           exclude_none=True)
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> UserExperiment:
-        """Create an instance of UserExperiment from a dict"""
+    def from_dict(cls, obj: dict) -> VerifyDspBlockUrlResponseAllOfBlock:
+        """Create an instance of VerifyDspBlockUrlResponseAllOfBlock from a dict"""
         if obj is None:
             return None
 
         if type(obj) is not dict:
-            return UserExperiment.construct(**obj)
+            return VerifyDspBlockUrlResponseAllOfBlock.construct(**obj)
 
-        _obj = UserExperiment.construct(**{
-            "type": obj.get("type"),
+        _obj = VerifyDspBlockUrlResponseAllOfBlock.construct(**{
             "title": obj.get("title"),
-            "help": obj.get("help"),
-            "enabled": obj.get("enabled"),
-            "show_to_user": obj.get("showToUser")
+            "author": obj.get("author"),
+            "description": obj.get("description"),
+            "name": obj.get("name"),
+            "latest_implementation_version": obj.get("latestImplementationVersion")
         })
         return _obj
```

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/user_organization.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/user_organization.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/verify_dsp_block_url_request.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/verify_dsp_block_url_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/verify_dsp_block_url_response.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/verify_dsp_block_url_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/verify_dsp_block_url_response_all_of.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/verify_dsp_block_url_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/verify_dsp_block_url_response_all_of_block.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/verify_organization_bucket_response_all_of_files.py`

 * *Files 16% similar despite different names*

```diff
@@ -16,58 +16,54 @@
 import re  # noqa: F401
 import json
 
 
 
 from pydantic import BaseModel, Field, StrictInt, StrictStr
 
-class VerifyDspBlockUrlResponseAllOfBlock(BaseModel):
-    title: StrictStr = ...
-    author: StrictStr = ...
-    description: StrictStr = ...
+class VerifyOrganizationBucketResponseAllOfFiles(BaseModel):
     name: StrictStr = ...
-    latest_implementation_version: StrictInt = Field(..., alias="latestImplementationVersion")
-    __properties = ["title", "author", "description", "name", "latestImplementationVersion"]
+    size: StrictInt = ...
+    folder_name: StrictStr = Field(..., alias="folderName")
+    __properties = ["name", "size", "folderName"]
 
     class Config:
         allow_population_by_field_name = True
         validate_assignment = False
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
         return pprint.pformat(self.dict(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> VerifyDspBlockUrlResponseAllOfBlock:
-        """Create an instance of VerifyDspBlockUrlResponseAllOfBlock from a JSON string"""
+    def from_json(cls, json_str: str) -> VerifyOrganizationBucketResponseAllOfFiles:
+        """Create an instance of VerifyOrganizationBucketResponseAllOfFiles from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self):
         """Returns the dictionary representation of the model using alias"""
         _dict = self.dict(by_alias=True,
                           exclude={
                           },
                           exclude_none=True)
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> VerifyDspBlockUrlResponseAllOfBlock:
-        """Create an instance of VerifyDspBlockUrlResponseAllOfBlock from a dict"""
+    def from_dict(cls, obj: dict) -> VerifyOrganizationBucketResponseAllOfFiles:
+        """Create an instance of VerifyOrganizationBucketResponseAllOfFiles from a dict"""
         if obj is None:
             return None
 
         if type(obj) is not dict:
-            return VerifyDspBlockUrlResponseAllOfBlock.construct(**obj)
+            return VerifyOrganizationBucketResponseAllOfFiles.construct(**obj)
 
-        _obj = VerifyDspBlockUrlResponseAllOfBlock.construct(**{
-            "title": obj.get("title"),
-            "author": obj.get("author"),
-            "description": obj.get("description"),
+        _obj = VerifyOrganizationBucketResponseAllOfFiles.construct(**{
             "name": obj.get("name"),
-            "latest_implementation_version": obj.get("latestImplementationVersion")
+            "size": obj.get("size"),
+            "folder_name": obj.get("folderName")
         })
         return _obj
```

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/verify_organization_bucket_request.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/update_organization_dataset_request.py`

 * *Files 19% similar despite different names*

```diff
@@ -13,63 +13,63 @@
 from __future__ import annotations
 from inspect import getfullargspec
 import pprint
 import re  # noqa: F401
 import json
 
 
-from typing import Optional
-from pydantic import BaseModel, Field, StrictStr
-
-class VerifyOrganizationBucketRequest(BaseModel):
-    access_key: StrictStr = Field(..., alias="accessKey", description="S3 access key")
-    secret_key: StrictStr = Field(..., alias="secretKey", description="S3 secret key")
-    bucket: StrictStr = Field(..., description="S3 bucket")
-    endpoint: StrictStr = Field(..., description="S3 endpoint")
-    region: StrictStr = Field(..., description="S3 region")
-    prefix: Optional[StrictStr] = Field(None, description="Optional prefix in the bucket. Set this if you don't have access to the full bucket for example.")
-    __properties = ["accessKey", "secretKey", "bucket", "endpoint", "region", "prefix"]
+from typing import List, Optional
+from pydantic import BaseModel, StrictStr
+from edgeimpulse_api.models.organization_add_dataset_request_bucket import OrganizationAddDatasetRequestBucket
+
+class UpdateOrganizationDatasetRequest(BaseModel):
+    dataset: Optional[StrictStr] = None
+    tags: Optional[List[StrictStr]] = None
+    category: Optional[StrictStr] = None
+    bucket: Optional[OrganizationAddDatasetRequestBucket] = None
+    __properties = ["dataset", "tags", "category", "bucket"]
 
     class Config:
         allow_population_by_field_name = True
         validate_assignment = False
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
         return pprint.pformat(self.dict(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> VerifyOrganizationBucketRequest:
-        """Create an instance of VerifyOrganizationBucketRequest from a JSON string"""
+    def from_json(cls, json_str: str) -> UpdateOrganizationDatasetRequest:
+        """Create an instance of UpdateOrganizationDatasetRequest from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self):
         """Returns the dictionary representation of the model using alias"""
         _dict = self.dict(by_alias=True,
                           exclude={
                           },
                           exclude_none=True)
+        # override the default output from pydantic by calling `to_dict()` of bucket
+        if self.bucket:
+            _dict['bucket'] = self.bucket.to_dict()
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> VerifyOrganizationBucketRequest:
-        """Create an instance of VerifyOrganizationBucketRequest from a dict"""
+    def from_dict(cls, obj: dict) -> UpdateOrganizationDatasetRequest:
+        """Create an instance of UpdateOrganizationDatasetRequest from a dict"""
         if obj is None:
             return None
 
         if type(obj) is not dict:
-            return VerifyOrganizationBucketRequest.construct(**obj)
+            return UpdateOrganizationDatasetRequest.construct(**obj)
 
-        _obj = VerifyOrganizationBucketRequest.construct(**{
-            "access_key": obj.get("accessKey"),
-            "secret_key": obj.get("secretKey"),
-            "bucket": obj.get("bucket"),
-            "endpoint": obj.get("endpoint"),
-            "region": obj.get("region"),
-            "prefix": obj.get("prefix")
+        _obj = UpdateOrganizationDatasetRequest.construct(**{
+            "dataset": obj.get("dataset"),
+            "tags": obj.get("tags"),
+            "category": obj.get("category"),
+            "bucket": OrganizationAddDatasetRequestBucket.from_dict(obj.get("bucket")) if obj.get("bucket") is not None else None
         })
         return _obj
```

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/verify_organization_bucket_response.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/verify_organization_bucket_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/verify_organization_bucket_response_all_of.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/verify_organization_bucket_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/verify_organization_bucket_response_all_of_files.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/whitelabel_admin_create_organization_request.py`

 * *Files 23% similar despite different names*

```diff
@@ -13,57 +13,57 @@
 from __future__ import annotations
 from inspect import getfullargspec
 import pprint
 import re  # noqa: F401
 import json
 
 
-
+from typing import Optional
 from pydantic import BaseModel, Field, StrictInt, StrictStr
 
-class VerifyOrganizationBucketResponseAllOfFiles(BaseModel):
-    name: StrictStr = ...
-    size: StrictInt = ...
-    folder_name: StrictStr = Field(..., alias="folderName")
-    __properties = ["name", "size", "folderName"]
+class WhitelabelAdminCreateOrganizationRequest(BaseModel):
+    organization_name: StrictStr = Field(..., alias="organizationName", description="The name of the organization.")
+    admin_id: Optional[StrictInt] = Field(None, alias="adminId", description="Unique identifier of the administrator of the new organization.")
+    admin_email: Optional[StrictStr] = Field(None, alias="adminEmail", description="Email of the administrator of the new organization.")
+    __properties = ["organizationName", "adminId", "adminEmail"]
 
     class Config:
         allow_population_by_field_name = True
         validate_assignment = False
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
         return pprint.pformat(self.dict(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> VerifyOrganizationBucketResponseAllOfFiles:
-        """Create an instance of VerifyOrganizationBucketResponseAllOfFiles from a JSON string"""
+    def from_json(cls, json_str: str) -> WhitelabelAdminCreateOrganizationRequest:
+        """Create an instance of WhitelabelAdminCreateOrganizationRequest from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self):
         """Returns the dictionary representation of the model using alias"""
         _dict = self.dict(by_alias=True,
                           exclude={
                           },
                           exclude_none=True)
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> VerifyOrganizationBucketResponseAllOfFiles:
-        """Create an instance of VerifyOrganizationBucketResponseAllOfFiles from a dict"""
+    def from_dict(cls, obj: dict) -> WhitelabelAdminCreateOrganizationRequest:
+        """Create an instance of WhitelabelAdminCreateOrganizationRequest from a dict"""
         if obj is None:
             return None
 
         if type(obj) is not dict:
-            return VerifyOrganizationBucketResponseAllOfFiles.construct(**obj)
+            return WhitelabelAdminCreateOrganizationRequest.construct(**obj)
 
-        _obj = VerifyOrganizationBucketResponseAllOfFiles.construct(**{
-            "name": obj.get("name"),
-            "size": obj.get("size"),
-            "folder_name": obj.get("folderName")
+        _obj = WhitelabelAdminCreateOrganizationRequest.construct(**{
+            "organization_name": obj.get("organizationName"),
+            "admin_id": obj.get("adminId"),
+            "admin_email": obj.get("adminEmail")
         })
         return _obj
```

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/verify_reset_password_request.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/organization_add_dataset_request.py`

 * *Files 20% similar despite different names*

```diff
@@ -13,55 +13,63 @@
 from __future__ import annotations
 from inspect import getfullargspec
 import pprint
 import re  # noqa: F401
 import json
 
 
-
+from typing import List
 from pydantic import BaseModel, StrictStr
+from edgeimpulse_api.models.organization_add_dataset_request_bucket import OrganizationAddDatasetRequestBucket
 
-class VerifyResetPasswordRequest(BaseModel):
-    email: StrictStr = ...
-    code: StrictStr = ...
-    __properties = ["email", "code"]
+class OrganizationAddDatasetRequest(BaseModel):
+    dataset: StrictStr = ...
+    tags: List[StrictStr] = ...
+    category: StrictStr = ...
+    bucket: OrganizationAddDatasetRequestBucket = ...
+    __properties = ["dataset", "tags", "category", "bucket"]
 
     class Config:
         allow_population_by_field_name = True
         validate_assignment = False
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
         return pprint.pformat(self.dict(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> VerifyResetPasswordRequest:
-        """Create an instance of VerifyResetPasswordRequest from a JSON string"""
+    def from_json(cls, json_str: str) -> OrganizationAddDatasetRequest:
+        """Create an instance of OrganizationAddDatasetRequest from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self):
         """Returns the dictionary representation of the model using alias"""
         _dict = self.dict(by_alias=True,
                           exclude={
                           },
                           exclude_none=True)
+        # override the default output from pydantic by calling `to_dict()` of bucket
+        if self.bucket:
+            _dict['bucket'] = self.bucket.to_dict()
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> VerifyResetPasswordRequest:
-        """Create an instance of VerifyResetPasswordRequest from a dict"""
+    def from_dict(cls, obj: dict) -> OrganizationAddDatasetRequest:
+        """Create an instance of OrganizationAddDatasetRequest from a dict"""
         if obj is None:
             return None
 
         if type(obj) is not dict:
-            return VerifyResetPasswordRequest.construct(**obj)
+            return OrganizationAddDatasetRequest.construct(**obj)
 
-        _obj = VerifyResetPasswordRequest.construct(**{
-            "email": obj.get("email"),
-            "code": obj.get("code")
+        _obj = OrganizationAddDatasetRequest.construct(**{
+            "dataset": obj.get("dataset"),
+            "tags": obj.get("tags"),
+            "category": obj.get("category"),
+            "bucket": OrganizationAddDatasetRequestBucket.from_dict(obj.get("bucket")) if obj.get("bucket") is not None else None
         })
         return _obj
```

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/whitelabel.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/whitelabel.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/window_settings_response.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/window_settings_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/window_settings_response_all_of.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/window_settings_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/models/window_settings_response_all_of_window_settings.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/models/window_settings_response_all_of_window_settings.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/edgeimpulse_api/rest.py` & `edgeimpulse_api-1.23.6/edgeimpulse_api/rest.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.23.0/pyproject.toml` & `edgeimpulse_api-1.23.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "edgeimpulse-api"
-version = "1.23.0" #DO_NOT_CHANGE_REPLACED_BY_BUILD_SCRIPT
+version = "1.23.6" #DO_NOT_CHANGE_REPLACED_BY_BUILD_SCRIPT
 description = "Python bindings for the Edge Impulse API."
 authors = ["EdgeImpulse Inc. <hello@edgeimpulse.com>"]
 license = "Apache-2.0"
 homepage = "https://edgeimpulse.com"
 documentation = "https://docs.edgeimpulse.com/reference/edge-impulse-api/edge-impulse-api"
 classifiers = [
     "Topic :: Scientific/Engineering :: Artificial Intelligence",
```

### Comparing `edgeimpulse_api-1.23.0/PKG-INFO` & `edgeimpulse_api-1.23.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edgeimpulse-api
-Version: 1.23.0
+Version: 1.23.6
 Summary: Python bindings for the Edge Impulse API.
 Home-page: https://edgeimpulse.com
 License: Apache-2.0
 Author: EdgeImpulse Inc.
 Author-email: hello@edgeimpulse.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
```

