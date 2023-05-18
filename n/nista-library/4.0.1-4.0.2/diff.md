# Comparing `tmp/nista_library-4.0.1.tar.gz` & `tmp/nista_library-4.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nista_library-4.0.1.tar", max compression
+gzip compressed data, was "nista_library-4.0.2.tar", max compression
```

## Comparing `nista_library-4.0.1.tar` & `nista_library-4.0.2.tar`

### file list

```diff
@@ -1,104 +1,103 @@
--rw-r--r--   0        0        0     1117 2023-05-18 08:38:48.865641 nista_library-4.0.1/LICENSE.md
--rw-r--r--   0        0        0     3001 2023-05-18 08:38:48.865641 nista_library-4.0.1/README.md
--rw-r--r--   0        0        0     1556 2023-05-18 08:38:48.865641 nista_library-4.0.1/SAMPLES.md
--rw-r--r--   0        0        0      153 2023-05-18 08:38:48.866641 nista_library-4.0.1/data_point_client/__init__.py
--rw-r--r--   0        0        0       47 2023-05-18 08:38:48.866641 nista_library-4.0.1/data_point_client/api/__init__.py
--rw-r--r--   0        0        0        0 2023-05-18 08:38:48.866641 nista_library-4.0.1/data_point_client/api/data_export/__init__.py
--rw-r--r--   0        0        0     5330 2023-05-18 08:38:48.866641 nista_library-4.0.1/data_point_client/api/data_export/data_export_create_csv_export.py
--rw-r--r--   0        0        0        0 2023-05-18 08:38:48.866641 nista_library-4.0.1/data_point_client/api/data_point/__init__.py
--rw-r--r--   0        0        0     5482 2023-05-18 08:38:48.866641 nista_library-4.0.1/data_point_client/api/data_point/data_point_append_execution_result_data.py
--rw-r--r--   0        0        0     5376 2023-05-18 08:38:48.866641 nista_library-4.0.1/data_point_client/api/data_point/data_point_append_time_series_data.py
--rw-r--r--   0        0        0     5768 2023-05-18 08:38:48.866641 nista_library-4.0.1/data_point_client/api/data_point/data_point_create_area.py
--rw-r--r--   0        0        0     6225 2023-05-18 08:38:48.866641 nista_library-4.0.1/data_point_client/api/data_point/data_point_create_area_message.py
--rw-r--r--   0        0        0     5323 2023-05-18 08:38:48.866641 nista_library-4.0.1/data_point_client/api/data_point/data_point_create_chiller_samples.py
--rw-r--r--   0        0        0     5441 2023-05-18 08:38:48.866641 nista_library-4.0.1/data_point_client/api/data_point/data_point_create_data_point.py
--rw-r--r--   0        0        0     4789 2023-05-18 08:38:48.866641 nista_library-4.0.1/data_point_client/api/data_point/data_point_delete_area.py
--rw-r--r--   0        0        0     4473 2023-05-18 08:38:48.866641 nista_library-4.0.1/data_point_client/api/data_point/data_point_delete_data_point.py
--rw-r--r--   0        0        0     4478 2023-05-18 08:38:48.866641 nista_library-4.0.1/data_point_client/api/data_point/data_point_delete_data_point_cleanup_rule.py
--rw-r--r--   0        0        0     5168 2023-05-18 08:38:48.866641 nista_library-4.0.1/data_point_client/api/data_point/data_point_delete_message.py
--rw-r--r--   0        0        0     5472 2023-05-18 08:38:48.866641 nista_library-4.0.1/data_point_client/api/data_point/data_point_get_data.py
--rw-r--r--   0        0        0     5005 2023-05-18 08:38:48.866641 nista_library-4.0.1/data_point_client/api/data_point/data_point_get_data_point.py
--rw-r--r--   0        0        0     5326 2023-05-18 08:38:48.866641 nista_library-4.0.1/data_point_client/api/data_point/data_point_get_data_point_by_version.py
--rw-r--r--   0        0        0     8928 2023-05-18 08:38:48.866641 nista_library-4.0.1/data_point_client/api/data_point/data_point_get_data_points.py
--rw-r--r--   0        0        0     7699 2023-05-18 08:38:48.866641 nista_library-4.0.1/data_point_client/api/data_point/data_point_get_tags.py
--rw-r--r--   0        0        0     4805 2023-05-18 08:38:48.866641 nista_library-4.0.1/data_point_client/api/data_point/data_point_get_tags_2.py
--rw-r--r--   0        0        0     5296 2023-05-18 08:38:48.866641 nista_library-4.0.1/data_point_client/api/data_point/data_point_list_areas.py
--rw-r--r--   0        0        0     5769 2023-05-18 08:38:48.866641 nista_library-4.0.1/data_point_client/api/data_point/data_point_update_area.py
--rw-r--r--   0        0        0     5397 2023-05-18 08:38:48.866641 nista_library-4.0.1/data_point_client/api/data_point/data_point_update_constant_data.py
--rw-r--r--   0        0        0     5442 2023-05-18 08:38:48.866641 nista_library-4.0.1/data_point_client/api/data_point/data_point_update_data_point.py
--rw-r--r--   0        0        0     5518 2023-05-18 08:38:48.866641 nista_library-4.0.1/data_point_client/api/data_point/data_point_update_data_point_cleanup_rule.py
--rw-r--r--   0        0        0     5262 2023-05-18 08:38:48.866641 nista_library-4.0.1/data_point_client/api/data_point/data_point_update_data_point_unit.py
--rw-r--r--   0        0        0     5369 2023-05-18 08:38:48.866641 nista_library-4.0.1/data_point_client/api/data_point/data_point_update_day_period_data.py
--rw-r--r--   0        0        0     6226 2023-05-18 08:38:48.866641 nista_library-4.0.1/data_point_client/api/data_point/data_point_update_message.py
--rw-r--r--   0        0        0     5381 2023-05-18 08:38:48.867641 nista_library-4.0.1/data_point_client/api/data_point/data_point_update_time_series_data.py
--rw-r--r--   0        0        0     5381 2023-05-18 08:38:48.867641 nista_library-4.0.1/data_point_client/api/data_point/data_point_update_week_period_data.py
--rw-r--r--   0        0        0     2817 2023-05-18 08:38:48.867641 nista_library-4.0.1/data_point_client/client.py
--rw-r--r--   0        0        0      470 2023-05-18 08:38:48.867641 nista_library-4.0.1/data_point_client/errors.py
--rw-r--r--   0        0        0     4795 2023-05-18 08:38:48.867641 nista_library-4.0.1/data_point_client/models/__init__.py
--rw-r--r--   0        0        0     1965 2023-05-18 08:38:48.867641 nista_library-4.0.1/data_point_client/models/append_execution_result_data_request.py
--rw-r--r--   0        0        0     1618 2023-05-18 08:38:48.867641 nista_library-4.0.1/data_point_client/models/append_time_series_request.py
--rw-r--r--   0        0        0     4359 2023-05-18 08:38:48.867641 nista_library-4.0.1/data_point_client/models/area_of_interest_response.py
--rw-r--r--   0        0        0     1858 2023-05-18 08:38:48.867641 nista_library-4.0.1/data_point_client/models/calculation_origin.py
--rw-r--r--   0        0        0     7547 2023-05-18 08:38:48.867641 nista_library-4.0.1/data_point_client/models/constant_data_bucket.py
--rw-r--r--   0        0        0     2965 2023-05-18 08:38:48.867641 nista_library-4.0.1/data_point_client/models/constant_data_point_data.py
--rw-r--r--   0        0        0     2597 2023-05-18 08:38:48.867641 nista_library-4.0.1/data_point_client/models/continuous_location_rest.py
--rw-r--r--   0        0        0      923 2023-05-18 08:38:48.867641 nista_library-4.0.1/data_point_client/models/create_area_message_request.py
--rw-r--r--   0        0        0     2319 2023-05-18 08:38:48.867641 nista_library-4.0.1/data_point_client/models/create_area_request.py
--rw-r--r--   0        0        0     5874 2023-05-18 08:38:48.867641 nista_library-4.0.1/data_point_client/models/data_bucket_base.py
--rw-r--r--   0        0        0     2054 2023-05-18 08:38:48.867641 nista_library-4.0.1/data_point_client/models/data_export_request.py
--rw-r--r--   0        0        0     2702 2023-05-18 08:38:48.867641 nista_library-4.0.1/data_point_client/models/data_point_comment_message_response.py
--rw-r--r--   0        0        0     2016 2023-05-18 08:38:48.867641 nista_library-4.0.1/data_point_client/models/data_point_data_base.py
--rw-r--r--   0        0        0     2418 2023-05-18 08:38:48.867641 nista_library-4.0.1/data_point_client/models/data_point_data_response.py
--rw-r--r--   0        0        0      779 2023-05-18 08:38:48.867641 nista_library-4.0.1/data_point_client/models/data_point_origin.py
--rw-r--r--   0        0        0     3212 2023-05-18 08:38:48.867641 nista_library-4.0.1/data_point_client/models/data_point_request.py
--rw-r--r--   0        0        0     7362 2023-05-18 08:38:48.867641 nista_library-4.0.1/data_point_client/models/data_point_response_base.py
--rw-r--r--   0        0        0     7281 2023-05-18 08:38:48.867641 nista_library-4.0.1/data_point_client/models/day_data_by_hour_transfer.py
--rw-r--r--   0        0        0     7564 2023-05-18 08:38:48.867641 nista_library-4.0.1/data_point_client/models/day_period_data_bucket.py
--rw-r--r--   0        0        0     4321 2023-05-18 08:38:48.867641 nista_library-4.0.1/data_point_client/models/day_period_data_point_data.py
--rw-r--r--   0        0        0      191 2023-05-18 08:38:48.867641 nista_library-4.0.1/data_point_client/models/en_area_type_rest.py
--rw-r--r--   0        0        0      192 2023-05-18 08:38:48.867641 nista_library-4.0.1/data_point_client/models/en_data_bucket_state.py
--rw-r--r--   0        0        0      208 2023-05-18 08:38:48.867641 nista_library-4.0.1/data_point_client/models/en_data_point_existence_dto.py
--rw-r--r--   0        0        0      214 2023-05-18 08:38:48.867641 nista_library-4.0.1/data_point_client/models/en_data_point_state_dto.py
--rw-r--r--   0        0        0      192 2023-05-18 08:38:48.867641 nista_library-4.0.1/data_point_client/models/en_data_point_status.py
--rw-r--r--   0        0        0      250 2023-05-18 08:38:48.867641 nista_library-4.0.1/data_point_client/models/en_data_point_type.py
--rw-r--r--   0        0        0      181 2023-05-18 08:38:48.867641 nista_library-4.0.1/data_point_client/models/en_operator.py
--rw-r--r--   0        0        0     2375 2023-05-18 08:38:48.867641 nista_library-4.0.1/data_point_client/models/file_origin.py
--rw-r--r--   0        0        0     2579 2023-05-18 08:38:48.868641 nista_library-4.0.1/data_point_client/models/get_constant_response.py
--rw-r--r--   0        0        0     3472 2023-05-18 08:38:48.868641 nista_library-4.0.1/data_point_client/models/get_data_request.py
--rw-r--r--   0        0        0      779 2023-05-18 08:38:48.868641 nista_library-4.0.1/data_point_client/models/get_data_response.py
--rw-r--r--   0        0        0     3900 2023-05-18 08:38:48.868641 nista_library-4.0.1/data_point_client/models/get_day_period_response.py
--rw-r--r--   0        0        0     2529 2023-05-18 08:38:48.868641 nista_library-4.0.1/data_point_client/models/get_series_response.py
--rw-r--r--   0        0        0     3227 2023-05-18 08:38:48.868641 nista_library-4.0.1/data_point_client/models/get_week_period_response.py
--rw-r--r--   0        0        0     1176 2023-05-18 08:38:48.868641 nista_library-4.0.1/data_point_client/models/gnista_unit_response.py
--rw-r--r--   0        0        0     1810 2023-05-18 08:38:48.868641 nista_library-4.0.1/data_point_client/models/live_data_origin.py
--rw-r--r--   0        0        0      765 2023-05-18 08:38:48.868641 nista_library-4.0.1/data_point_client/models/location_rest.py
--rw-r--r--   0        0        0     2045 2023-05-18 08:38:48.868641 nista_library-4.0.1/data_point_client/models/point_location_rest.py
--rw-r--r--   0        0        0     3377 2023-05-18 08:38:48.868641 nista_library-4.0.1/data_point_client/models/problem_details.py
--rw-r--r--   0        0        0     1215 2023-05-18 08:38:48.868641 nista_library-4.0.1/data_point_client/models/problem_details_extensions.py
--rw-r--r--   0        0        0     1449 2023-05-18 08:38:48.868641 nista_library-4.0.1/data_point_client/models/remote_origin.py
--rw-r--r--   0        0        0     1247 2023-05-18 08:38:48.868641 nista_library-4.0.1/data_point_client/models/rule.py
--rw-r--r--   0        0        0     9273 2023-05-18 08:38:48.868641 nista_library-4.0.1/data_point_client/models/series_data_bucket.py
--rw-r--r--   0        0        0     3058 2023-05-18 08:38:48.868641 nista_library-4.0.1/data_point_client/models/series_data_point_data.py
--rw-r--r--   0        0        0     1446 2023-05-18 08:38:48.868641 nista_library-4.0.1/data_point_client/models/sub_series_request.py
--rw-r--r--   0        0        0     1214 2023-05-18 08:38:48.868641 nista_library-4.0.1/data_point_client/models/sub_series_request_values.py
--rw-r--r--   0        0        0     1631 2023-05-18 08:38:48.868641 nista_library-4.0.1/data_point_client/models/time_series_period.py
--rw-r--r--   0        0        0     2675 2023-05-18 08:38:48.868641 nista_library-4.0.1/data_point_client/models/time_series_response.py
--rw-r--r--   0        0        0     1219 2023-05-18 08:38:48.868641 nista_library-4.0.1/data_point_client/models/time_series_response_curve.py
--rw-r--r--   0        0        0      923 2023-05-18 08:38:48.868641 nista_library-4.0.1/data_point_client/models/update_area_message_request.py
--rw-r--r--   0        0        0     2674 2023-05-18 08:38:48.868641 nista_library-4.0.1/data_point_client/models/update_area_request.py
--rw-r--r--   0        0        0     1401 2023-05-18 08:38:48.868641 nista_library-4.0.1/data_point_client/models/update_constant_data_request.py
--rw-r--r--   0        0        0     2725 2023-05-18 08:38:48.868641 nista_library-4.0.1/data_point_client/models/update_day_period_request.py
--rw-r--r--   0        0        0     3346 2023-05-18 08:38:48.868641 nista_library-4.0.1/data_point_client/models/update_time_series_request.py
--rw-r--r--   0        0        0     2052 2023-05-18 08:38:48.868641 nista_library-4.0.1/data_point_client/models/update_week_period_request.py
--rw-r--r--   0        0        0     7478 2023-05-18 08:38:48.868641 nista_library-4.0.1/data_point_client/models/week_data_transfere.py
--rw-r--r--   0        0        0     7576 2023-05-18 08:38:48.868641 nista_library-4.0.1/data_point_client/models/week_period_data_bucket.py
--rw-r--r--   0        0        0     3648 2023-05-18 08:38:48.868641 nista_library-4.0.1/data_point_client/models/week_period_data_point_data.py
--rw-r--r--   0        0        0       25 2023-05-18 08:38:48.868641 nista_library-4.0.1/data_point_client/py.typed
--rw-r--r--   0        0        0      974 2023-05-18 08:38:48.868641 nista_library-4.0.1/data_point_client/types.py
--rw-r--r--   0        0        0      944 2023-05-18 08:38:48.869641 nista_library-4.0.1/nista_library/__init__.py
--rw-r--r--   0        0        0     8866 2023-05-18 08:38:48.869641 nista_library-4.0.1/nista_library/nista_connetion.py
--rw-r--r--   0        0        0      915 2023-05-18 08:38:48.869641 nista_library-4.0.1/nista_library/nista_credential_manager.py
--rw-r--r--   0        0        0    12775 2023-05-18 08:38:48.869641 nista_library-4.0.1/nista_library/nista_data_point.py
--rw-r--r--   0        0        0     1683 2023-05-18 08:38:48.870641 nista_library-4.0.1/nista_library/nista_data_points.py
--rw-r--r--   0        0        0     1324 2023-05-18 08:38:48.870641 nista_library-4.0.1/pyproject.toml
--rw-r--r--   0        0        0     5596 1970-01-01 00:00:00.000000 nista_library-4.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1117 2023-05-18 13:57:43.917467 nista_library-4.0.2/LICENSE.md
+-rw-r--r--   0        0        0     6428 2023-05-18 13:57:43.917467 nista_library-4.0.2/README.md
+-rw-r--r--   0        0        0      153 2023-05-18 13:57:43.919467 nista_library-4.0.2/data_point_client/__init__.py
+-rw-r--r--   0        0        0       47 2023-05-18 13:57:43.919467 nista_library-4.0.2/data_point_client/api/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-18 13:57:43.919467 nista_library-4.0.2/data_point_client/api/data_export/__init__.py
+-rw-r--r--   0        0        0     5330 2023-05-18 13:57:43.919467 nista_library-4.0.2/data_point_client/api/data_export/data_export_create_csv_export.py
+-rw-r--r--   0        0        0        0 2023-05-18 13:57:43.919467 nista_library-4.0.2/data_point_client/api/data_point/__init__.py
+-rw-r--r--   0        0        0     5482 2023-05-18 13:57:43.919467 nista_library-4.0.2/data_point_client/api/data_point/data_point_append_execution_result_data.py
+-rw-r--r--   0        0        0     5376 2023-05-18 13:57:43.919467 nista_library-4.0.2/data_point_client/api/data_point/data_point_append_time_series_data.py
+-rw-r--r--   0        0        0     5768 2023-05-18 13:57:43.919467 nista_library-4.0.2/data_point_client/api/data_point/data_point_create_area.py
+-rw-r--r--   0        0        0     6225 2023-05-18 13:57:43.919467 nista_library-4.0.2/data_point_client/api/data_point/data_point_create_area_message.py
+-rw-r--r--   0        0        0     5323 2023-05-18 13:57:43.919467 nista_library-4.0.2/data_point_client/api/data_point/data_point_create_chiller_samples.py
+-rw-r--r--   0        0        0     5441 2023-05-18 13:57:43.919467 nista_library-4.0.2/data_point_client/api/data_point/data_point_create_data_point.py
+-rw-r--r--   0        0        0     4789 2023-05-18 13:57:43.919467 nista_library-4.0.2/data_point_client/api/data_point/data_point_delete_area.py
+-rw-r--r--   0        0        0     4473 2023-05-18 13:57:43.919467 nista_library-4.0.2/data_point_client/api/data_point/data_point_delete_data_point.py
+-rw-r--r--   0        0        0     4478 2023-05-18 13:57:43.919467 nista_library-4.0.2/data_point_client/api/data_point/data_point_delete_data_point_cleanup_rule.py
+-rw-r--r--   0        0        0     5168 2023-05-18 13:57:43.919467 nista_library-4.0.2/data_point_client/api/data_point/data_point_delete_message.py
+-rw-r--r--   0        0        0     5472 2023-05-18 13:57:43.919467 nista_library-4.0.2/data_point_client/api/data_point/data_point_get_data.py
+-rw-r--r--   0        0        0     5005 2023-05-18 13:57:43.919467 nista_library-4.0.2/data_point_client/api/data_point/data_point_get_data_point.py
+-rw-r--r--   0        0        0     5326 2023-05-18 13:57:43.919467 nista_library-4.0.2/data_point_client/api/data_point/data_point_get_data_point_by_version.py
+-rw-r--r--   0        0        0     8928 2023-05-18 13:57:43.919467 nista_library-4.0.2/data_point_client/api/data_point/data_point_get_data_points.py
+-rw-r--r--   0        0        0     7699 2023-05-18 13:57:43.919467 nista_library-4.0.2/data_point_client/api/data_point/data_point_get_tags.py
+-rw-r--r--   0        0        0     4805 2023-05-18 13:57:43.919467 nista_library-4.0.2/data_point_client/api/data_point/data_point_get_tags_2.py
+-rw-r--r--   0        0        0     5296 2023-05-18 13:57:43.919467 nista_library-4.0.2/data_point_client/api/data_point/data_point_list_areas.py
+-rw-r--r--   0        0        0     5769 2023-05-18 13:57:43.919467 nista_library-4.0.2/data_point_client/api/data_point/data_point_update_area.py
+-rw-r--r--   0        0        0     5397 2023-05-18 13:57:43.919467 nista_library-4.0.2/data_point_client/api/data_point/data_point_update_constant_data.py
+-rw-r--r--   0        0        0     5442 2023-05-18 13:57:43.919467 nista_library-4.0.2/data_point_client/api/data_point/data_point_update_data_point.py
+-rw-r--r--   0        0        0     5518 2023-05-18 13:57:43.920467 nista_library-4.0.2/data_point_client/api/data_point/data_point_update_data_point_cleanup_rule.py
+-rw-r--r--   0        0        0     5262 2023-05-18 13:57:43.920467 nista_library-4.0.2/data_point_client/api/data_point/data_point_update_data_point_unit.py
+-rw-r--r--   0        0        0     5369 2023-05-18 13:57:43.920467 nista_library-4.0.2/data_point_client/api/data_point/data_point_update_day_period_data.py
+-rw-r--r--   0        0        0     6226 2023-05-18 13:57:43.920467 nista_library-4.0.2/data_point_client/api/data_point/data_point_update_message.py
+-rw-r--r--   0        0        0     5381 2023-05-18 13:57:43.920467 nista_library-4.0.2/data_point_client/api/data_point/data_point_update_time_series_data.py
+-rw-r--r--   0        0        0     5381 2023-05-18 13:57:43.920467 nista_library-4.0.2/data_point_client/api/data_point/data_point_update_week_period_data.py
+-rw-r--r--   0        0        0     2817 2023-05-18 13:57:43.920467 nista_library-4.0.2/data_point_client/client.py
+-rw-r--r--   0        0        0      470 2023-05-18 13:57:43.920467 nista_library-4.0.2/data_point_client/errors.py
+-rw-r--r--   0        0        0     4795 2023-05-18 13:57:43.920467 nista_library-4.0.2/data_point_client/models/__init__.py
+-rw-r--r--   0        0        0     1965 2023-05-18 13:57:43.920467 nista_library-4.0.2/data_point_client/models/append_execution_result_data_request.py
+-rw-r--r--   0        0        0     1618 2023-05-18 13:57:43.920467 nista_library-4.0.2/data_point_client/models/append_time_series_request.py
+-rw-r--r--   0        0        0     4359 2023-05-18 13:57:43.920467 nista_library-4.0.2/data_point_client/models/area_of_interest_response.py
+-rw-r--r--   0        0        0     1858 2023-05-18 13:57:43.920467 nista_library-4.0.2/data_point_client/models/calculation_origin.py
+-rw-r--r--   0        0        0     7547 2023-05-18 13:57:43.920467 nista_library-4.0.2/data_point_client/models/constant_data_bucket.py
+-rw-r--r--   0        0        0     2965 2023-05-18 13:57:43.920467 nista_library-4.0.2/data_point_client/models/constant_data_point_data.py
+-rw-r--r--   0        0        0     2597 2023-05-18 13:57:43.920467 nista_library-4.0.2/data_point_client/models/continuous_location_rest.py
+-rw-r--r--   0        0        0      923 2023-05-18 13:57:43.920467 nista_library-4.0.2/data_point_client/models/create_area_message_request.py
+-rw-r--r--   0        0        0     2319 2023-05-18 13:57:43.920467 nista_library-4.0.2/data_point_client/models/create_area_request.py
+-rw-r--r--   0        0        0     5874 2023-05-18 13:57:43.920467 nista_library-4.0.2/data_point_client/models/data_bucket_base.py
+-rw-r--r--   0        0        0     2054 2023-05-18 13:57:43.920467 nista_library-4.0.2/data_point_client/models/data_export_request.py
+-rw-r--r--   0        0        0     2702 2023-05-18 13:57:43.920467 nista_library-4.0.2/data_point_client/models/data_point_comment_message_response.py
+-rw-r--r--   0        0        0     2016 2023-05-18 13:57:43.920467 nista_library-4.0.2/data_point_client/models/data_point_data_base.py
+-rw-r--r--   0        0        0     2418 2023-05-18 13:57:43.920467 nista_library-4.0.2/data_point_client/models/data_point_data_response.py
+-rw-r--r--   0        0        0      779 2023-05-18 13:57:43.920467 nista_library-4.0.2/data_point_client/models/data_point_origin.py
+-rw-r--r--   0        0        0     3212 2023-05-18 13:57:43.920467 nista_library-4.0.2/data_point_client/models/data_point_request.py
+-rw-r--r--   0        0        0     7362 2023-05-18 13:57:43.920467 nista_library-4.0.2/data_point_client/models/data_point_response_base.py
+-rw-r--r--   0        0        0     7281 2023-05-18 13:57:43.920467 nista_library-4.0.2/data_point_client/models/day_data_by_hour_transfer.py
+-rw-r--r--   0        0        0     7564 2023-05-18 13:57:43.920467 nista_library-4.0.2/data_point_client/models/day_period_data_bucket.py
+-rw-r--r--   0        0        0     4321 2023-05-18 13:57:43.920467 nista_library-4.0.2/data_point_client/models/day_period_data_point_data.py
+-rw-r--r--   0        0        0      191 2023-05-18 13:57:43.920467 nista_library-4.0.2/data_point_client/models/en_area_type_rest.py
+-rw-r--r--   0        0        0      192 2023-05-18 13:57:43.920467 nista_library-4.0.2/data_point_client/models/en_data_bucket_state.py
+-rw-r--r--   0        0        0      208 2023-05-18 13:57:43.920467 nista_library-4.0.2/data_point_client/models/en_data_point_existence_dto.py
+-rw-r--r--   0        0        0      214 2023-05-18 13:57:43.920467 nista_library-4.0.2/data_point_client/models/en_data_point_state_dto.py
+-rw-r--r--   0        0        0      192 2023-05-18 13:57:43.920467 nista_library-4.0.2/data_point_client/models/en_data_point_status.py
+-rw-r--r--   0        0        0      250 2023-05-18 13:57:43.920467 nista_library-4.0.2/data_point_client/models/en_data_point_type.py
+-rw-r--r--   0        0        0      181 2023-05-18 13:57:43.920467 nista_library-4.0.2/data_point_client/models/en_operator.py
+-rw-r--r--   0        0        0     2375 2023-05-18 13:57:43.921466 nista_library-4.0.2/data_point_client/models/file_origin.py
+-rw-r--r--   0        0        0     2579 2023-05-18 13:57:43.921466 nista_library-4.0.2/data_point_client/models/get_constant_response.py
+-rw-r--r--   0        0        0     3472 2023-05-18 13:57:43.921466 nista_library-4.0.2/data_point_client/models/get_data_request.py
+-rw-r--r--   0        0        0      779 2023-05-18 13:57:43.921466 nista_library-4.0.2/data_point_client/models/get_data_response.py
+-rw-r--r--   0        0        0     3900 2023-05-18 13:57:43.921466 nista_library-4.0.2/data_point_client/models/get_day_period_response.py
+-rw-r--r--   0        0        0     2529 2023-05-18 13:57:43.921466 nista_library-4.0.2/data_point_client/models/get_series_response.py
+-rw-r--r--   0        0        0     3227 2023-05-18 13:57:43.921466 nista_library-4.0.2/data_point_client/models/get_week_period_response.py
+-rw-r--r--   0        0        0     1176 2023-05-18 13:57:43.921466 nista_library-4.0.2/data_point_client/models/gnista_unit_response.py
+-rw-r--r--   0        0        0     1810 2023-05-18 13:57:43.921466 nista_library-4.0.2/data_point_client/models/live_data_origin.py
+-rw-r--r--   0        0        0      765 2023-05-18 13:57:43.921466 nista_library-4.0.2/data_point_client/models/location_rest.py
+-rw-r--r--   0        0        0     2045 2023-05-18 13:57:43.921466 nista_library-4.0.2/data_point_client/models/point_location_rest.py
+-rw-r--r--   0        0        0     3377 2023-05-18 13:57:43.921466 nista_library-4.0.2/data_point_client/models/problem_details.py
+-rw-r--r--   0        0        0     1215 2023-05-18 13:57:43.921466 nista_library-4.0.2/data_point_client/models/problem_details_extensions.py
+-rw-r--r--   0        0        0     1449 2023-05-18 13:57:43.921466 nista_library-4.0.2/data_point_client/models/remote_origin.py
+-rw-r--r--   0        0        0     1247 2023-05-18 13:57:43.921466 nista_library-4.0.2/data_point_client/models/rule.py
+-rw-r--r--   0        0        0     9273 2023-05-18 13:57:43.921466 nista_library-4.0.2/data_point_client/models/series_data_bucket.py
+-rw-r--r--   0        0        0     3058 2023-05-18 13:57:43.921466 nista_library-4.0.2/data_point_client/models/series_data_point_data.py
+-rw-r--r--   0        0        0     1446 2023-05-18 13:57:43.921466 nista_library-4.0.2/data_point_client/models/sub_series_request.py
+-rw-r--r--   0        0        0     1214 2023-05-18 13:57:43.921466 nista_library-4.0.2/data_point_client/models/sub_series_request_values.py
+-rw-r--r--   0        0        0     1631 2023-05-18 13:57:43.921466 nista_library-4.0.2/data_point_client/models/time_series_period.py
+-rw-r--r--   0        0        0     2675 2023-05-18 13:57:43.921466 nista_library-4.0.2/data_point_client/models/time_series_response.py
+-rw-r--r--   0        0        0     1219 2023-05-18 13:57:43.921466 nista_library-4.0.2/data_point_client/models/time_series_response_curve.py
+-rw-r--r--   0        0        0      923 2023-05-18 13:57:43.921466 nista_library-4.0.2/data_point_client/models/update_area_message_request.py
+-rw-r--r--   0        0        0     2674 2023-05-18 13:57:43.921466 nista_library-4.0.2/data_point_client/models/update_area_request.py
+-rw-r--r--   0        0        0     1401 2023-05-18 13:57:43.922467 nista_library-4.0.2/data_point_client/models/update_constant_data_request.py
+-rw-r--r--   0        0        0     2725 2023-05-18 13:57:43.922467 nista_library-4.0.2/data_point_client/models/update_day_period_request.py
+-rw-r--r--   0        0        0     3346 2023-05-18 13:57:43.922467 nista_library-4.0.2/data_point_client/models/update_time_series_request.py
+-rw-r--r--   0        0        0     2052 2023-05-18 13:57:43.922467 nista_library-4.0.2/data_point_client/models/update_week_period_request.py
+-rw-r--r--   0        0        0     7478 2023-05-18 13:57:43.922467 nista_library-4.0.2/data_point_client/models/week_data_transfere.py
+-rw-r--r--   0        0        0     7576 2023-05-18 13:57:43.922467 nista_library-4.0.2/data_point_client/models/week_period_data_bucket.py
+-rw-r--r--   0        0        0     3648 2023-05-18 13:57:43.922467 nista_library-4.0.2/data_point_client/models/week_period_data_point_data.py
+-rw-r--r--   0        0        0       25 2023-05-18 13:57:43.922467 nista_library-4.0.2/data_point_client/py.typed
+-rw-r--r--   0        0        0      974 2023-05-18 13:57:43.922467 nista_library-4.0.2/data_point_client/types.py
+-rw-r--r--   0        0        0     1007 2023-05-18 13:57:43.923467 nista_library-4.0.2/nista_library/__init__.py
+-rw-r--r--   0        0        0    11406 2023-05-18 13:57:43.923467 nista_library-4.0.2/nista_library/nista_connetion.py
+-rw-r--r--   0        0        0     1049 2023-05-18 13:57:43.923467 nista_library-4.0.2/nista_library/nista_credential_manager.py
+-rw-r--r--   0        0        0    15802 2023-05-18 13:57:43.923467 nista_library-4.0.2/nista_library/nista_data_point.py
+-rw-r--r--   0        0        0     1997 2023-05-18 13:57:43.923467 nista_library-4.0.2/nista_library/nista_data_points.py
+-rw-r--r--   0        0        0     1383 2023-05-18 13:57:43.925466 nista_library-4.0.2/pyproject.toml
+-rw-r--r--   0        0        0     7471 1970-01-01 00:00:00.000000 nista_library-4.0.2/PKG-INFO
```

### Comparing `nista_library-4.0.1/LICENSE.md` & `nista_library-4.0.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.1/data_point_client/api/data_export/data_export_create_csv_export.py` & `nista_library-4.0.2/data_point_client/api/data_export/data_export_create_csv_export.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.1/data_point_client/api/data_point/data_point_append_execution_result_data.py` & `nista_library-4.0.2/data_point_client/api/data_point/data_point_append_execution_result_data.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.1/data_point_client/api/data_point/data_point_append_time_series_data.py` & `nista_library-4.0.2/data_point_client/api/data_point/data_point_append_time_series_data.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.1/data_point_client/api/data_point/data_point_create_area.py` & `nista_library-4.0.2/data_point_client/api/data_point/data_point_create_area.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.1/data_point_client/api/data_point/data_point_create_area_message.py` & `nista_library-4.0.2/data_point_client/api/data_point/data_point_create_area_message.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.1/data_point_client/api/data_point/data_point_create_chiller_samples.py` & `nista_library-4.0.2/data_point_client/api/data_point/data_point_create_chiller_samples.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.1/data_point_client/api/data_point/data_point_create_data_point.py` & `nista_library-4.0.2/data_point_client/api/data_point/data_point_create_data_point.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.1/data_point_client/api/data_point/data_point_delete_area.py` & `nista_library-4.0.2/data_point_client/api/data_point/data_point_delete_area.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.1/data_point_client/api/data_point/data_point_delete_data_point.py` & `nista_library-4.0.2/data_point_client/api/data_point/data_point_delete_data_point.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.1/data_point_client/api/data_point/data_point_delete_data_point_cleanup_rule.py` & `nista_library-4.0.2/data_point_client/api/data_point/data_point_delete_data_point_cleanup_rule.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.1/data_point_client/api/data_point/data_point_delete_message.py` & `nista_library-4.0.2/data_point_client/api/data_point/data_point_delete_message.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.1/data_point_client/api/data_point/data_point_get_data.py` & `nista_library-4.0.2/data_point_client/api/data_point/data_point_get_data.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.1/data_point_client/api/data_point/data_point_get_data_point.py` & `nista_library-4.0.2/data_point_client/api/data_point/data_point_get_data_point.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.1/data_point_client/api/data_point/data_point_get_data_point_by_version.py` & `nista_library-4.0.2/data_point_client/api/data_point/data_point_get_data_point_by_version.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.1/data_point_client/api/data_point/data_point_get_data_points.py` & `nista_library-4.0.2/data_point_client/api/data_point/data_point_get_data_points.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.1/data_point_client/api/data_point/data_point_get_tags.py` & `nista_library-4.0.2/data_point_client/api/data_point/data_point_get_tags.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.1/data_point_client/api/data_point/data_point_get_tags_2.py` & `nista_library-4.0.2/data_point_client/api/data_point/data_point_get_tags_2.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.1/data_point_client/api/data_point/data_point_list_areas.py` & `nista_library-4.0.2/data_point_client/api/data_point/data_point_list_areas.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.1/data_point_client/api/data_point/data_point_update_area.py` & `nista_library-4.0.2/data_point_client/api/data_point/data_point_update_area.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.1/data_point_client/api/data_point/data_point_update_constant_data.py` & `nista_library-4.0.2/data_point_client/api/data_point/data_point_update_constant_data.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.1/data_point_client/api/data_point/data_point_update_data_point.py` & `nista_library-4.0.2/data_point_client/api/data_point/data_point_update_data_point.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.1/data_point_client/api/data_point/data_point_update_data_point_cleanup_rule.py` & `nista_library-4.0.2/data_point_client/api/data_point/data_point_update_data_point_cleanup_rule.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.1/data_point_client/api/data_point/data_point_update_data_point_unit.py` & `nista_library-4.0.2/data_point_client/api/data_point/data_point_update_data_point_unit.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.1/data_point_client/api/data_point/data_point_update_day_period_data.py` & `nista_library-4.0.2/data_point_client/api/data_point/data_point_update_day_period_data.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.1/data_point_client/api/data_point/data_point_update_message.py` & `nista_library-4.0.2/data_point_client/api/data_point/data_point_update_message.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.1/data_point_client/api/data_point/data_point_update_time_series_data.py` & `nista_library-4.0.2/data_point_client/api/data_point/data_point_update_time_series_data.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.1/data_point_client/api/data_point/data_point_update_week_period_data.py` & `nista_library-4.0.2/data_point_client/api/data_point/data_point_update_week_period_data.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.1/data_point_client/client.py` & `nista_library-4.0.2/data_point_client/client.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.1/data_point_client/models/__init__.py` & `nista_library-4.0.2/data_point_client/models/__init__.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.1/data_point_client/models/append_execution_result_data_request.py` & `nista_library-4.0.2/data_point_client/models/append_execution_result_data_request.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.1/data_point_client/models/append_time_series_request.py` & `nista_library-4.0.2/data_point_client/models/append_time_series_request.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.1/data_point_client/models/area_of_interest_response.py` & `nista_library-4.0.2/data_point_client/models/area_of_interest_response.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.1/data_point_client/models/calculation_origin.py` & `nista_library-4.0.2/data_point_client/models/calculation_origin.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.1/data_point_client/models/constant_data_bucket.py` & `nista_library-4.0.2/data_point_client/models/constant_data_bucket.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.1/data_point_client/models/constant_data_point_data.py` & `nista_library-4.0.2/data_point_client/models/constant_data_point_data.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.1/data_point_client/models/continuous_location_rest.py` & `nista_library-4.0.2/data_point_client/models/continuous_location_rest.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.1/data_point_client/models/create_area_message_request.py` & `nista_library-4.0.2/data_point_client/models/create_area_message_request.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.1/data_point_client/models/create_area_request.py` & `nista_library-4.0.2/data_point_client/models/create_area_request.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.1/data_point_client/models/data_bucket_base.py` & `nista_library-4.0.2/data_point_client/models/data_bucket_base.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.1/data_point_client/models/data_export_request.py` & `nista_library-4.0.2/data_point_client/models/data_export_request.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.1/data_point_client/models/data_point_comment_message_response.py` & `nista_library-4.0.2/data_point_client/models/data_point_comment_message_response.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.1/data_point_client/models/data_point_data_base.py` & `nista_library-4.0.2/data_point_client/models/data_point_data_base.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.1/data_point_client/models/data_point_data_response.py` & `nista_library-4.0.2/data_point_client/models/data_point_data_response.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.1/data_point_client/models/data_point_origin.py` & `nista_library-4.0.2/data_point_client/models/data_point_origin.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.1/data_point_client/models/data_point_request.py` & `nista_library-4.0.2/data_point_client/models/data_point_request.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.1/data_point_client/models/data_point_response_base.py` & `nista_library-4.0.2/data_point_client/models/data_point_response_base.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.1/data_point_client/models/day_data_by_hour_transfer.py` & `nista_library-4.0.2/data_point_client/models/day_data_by_hour_transfer.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.1/data_point_client/models/day_period_data_bucket.py` & `nista_library-4.0.2/data_point_client/models/day_period_data_bucket.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.1/data_point_client/models/day_period_data_point_data.py` & `nista_library-4.0.2/data_point_client/models/day_period_data_point_data.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.1/data_point_client/models/file_origin.py` & `nista_library-4.0.2/data_point_client/models/file_origin.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.1/data_point_client/models/get_constant_response.py` & `nista_library-4.0.2/data_point_client/models/get_constant_response.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.1/data_point_client/models/get_data_request.py` & `nista_library-4.0.2/data_point_client/models/get_data_request.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.1/data_point_client/models/get_data_response.py` & `nista_library-4.0.2/data_point_client/models/get_data_response.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.1/data_point_client/models/get_day_period_response.py` & `nista_library-4.0.2/data_point_client/models/get_day_period_response.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.1/data_point_client/models/get_series_response.py` & `nista_library-4.0.2/data_point_client/models/get_series_response.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.1/data_point_client/models/get_week_period_response.py` & `nista_library-4.0.2/data_point_client/models/get_week_period_response.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.1/data_point_client/models/gnista_unit_response.py` & `nista_library-4.0.2/data_point_client/models/gnista_unit_response.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.1/data_point_client/models/live_data_origin.py` & `nista_library-4.0.2/data_point_client/models/live_data_origin.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.1/data_point_client/models/location_rest.py` & `nista_library-4.0.2/data_point_client/models/location_rest.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.1/data_point_client/models/point_location_rest.py` & `nista_library-4.0.2/data_point_client/models/point_location_rest.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.1/data_point_client/models/problem_details.py` & `nista_library-4.0.2/data_point_client/models/problem_details.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.1/data_point_client/models/problem_details_extensions.py` & `nista_library-4.0.2/data_point_client/models/problem_details_extensions.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.1/data_point_client/models/remote_origin.py` & `nista_library-4.0.2/data_point_client/models/remote_origin.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.1/data_point_client/models/rule.py` & `nista_library-4.0.2/data_point_client/models/rule.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.1/data_point_client/models/series_data_bucket.py` & `nista_library-4.0.2/data_point_client/models/series_data_bucket.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.1/data_point_client/models/series_data_point_data.py` & `nista_library-4.0.2/data_point_client/models/series_data_point_data.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.1/data_point_client/models/sub_series_request.py` & `nista_library-4.0.2/data_point_client/models/sub_series_request.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.1/data_point_client/models/sub_series_request_values.py` & `nista_library-4.0.2/data_point_client/models/sub_series_request_values.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.1/data_point_client/models/time_series_period.py` & `nista_library-4.0.2/data_point_client/models/time_series_period.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.1/data_point_client/models/time_series_response.py` & `nista_library-4.0.2/data_point_client/models/time_series_response.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.1/data_point_client/models/time_series_response_curve.py` & `nista_library-4.0.2/data_point_client/models/time_series_response_curve.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.1/data_point_client/models/update_area_message_request.py` & `nista_library-4.0.2/data_point_client/models/update_area_message_request.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.1/data_point_client/models/update_area_request.py` & `nista_library-4.0.2/data_point_client/models/update_area_request.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.1/data_point_client/models/update_constant_data_request.py` & `nista_library-4.0.2/data_point_client/models/update_constant_data_request.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.1/data_point_client/models/update_day_period_request.py` & `nista_library-4.0.2/data_point_client/models/update_day_period_request.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.1/data_point_client/models/update_time_series_request.py` & `nista_library-4.0.2/data_point_client/models/update_time_series_request.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.1/data_point_client/models/update_week_period_request.py` & `nista_library-4.0.2/data_point_client/models/update_week_period_request.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.1/data_point_client/models/week_data_transfere.py` & `nista_library-4.0.2/data_point_client/models/week_data_transfere.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.1/data_point_client/models/week_period_data_bucket.py` & `nista_library-4.0.2/data_point_client/models/week_period_data_bucket.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.1/data_point_client/models/week_period_data_point_data.py` & `nista_library-4.0.2/data_point_client/models/week_period_data_point_data.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.1/data_point_client/types.py` & `nista_library-4.0.2/data_point_client/types.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.1/nista_library/__init__.py` & `nista_library-4.0.2/nista_library/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,12 @@
+"""Nista Library
+
+A client library for accessing nista.io
+"""
+
 import logging
 import sys
 
 import structlog
 
 from .nista_connetion import KeyringNistaConnection, NistaConnection, StaticTokenNistaConnection
 from .nista_credential_manager import NistaCredentialManager
```

### Comparing `nista_library-4.0.1/nista_library/nista_credential_manager.py` & `nista_library-4.0.2/nista_library/nista_credential_manager.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,18 @@
 from oauth2_client.credentials_manager import CredentialManager
 from structlog import get_logger
 
 log = get_logger()
 
 
 class NistaCredentialManager(CredentialManager):
+    """Credential Manager to intercept and store OAuth Tokens.
+        .. seealso::
+        Module :py:mod:`nista_connection`
+    """
     def __init__(self, service_information, proxies=None):
         super().__init__(service_information, proxies)
         self.id_token = None
         self.access_token = None
         self.refresh_token = None
 
     def _process_token_response(self, token_response, refresh_token_mandatory):
```

### Comparing `nista_library-4.0.1/nista_library/nista_data_point.py` & `nista_library-4.0.2/nista_library/nista_data_point.py`

 * *Files 13% similar despite different names*

```diff
@@ -15,101 +15,165 @@
     data_point_get_data,
     data_point_get_data_point,
     data_point_update_constant_data,
     data_point_update_time_series_data,
     data_point_update_week_period_data,
 )
 from data_point_client.models import GetConstantResponse, GetSeriesResponse
-from data_point_client.models.append_execution_result_data_request import AppendExecutionResultDataRequest
+from data_point_client.models.append_execution_result_data_request import (
+    AppendExecutionResultDataRequest,
+)
+from data_point_client.models.data_point_response_base import DataPointResponseBase
 from data_point_client.models.append_time_series_request import AppendTimeSeriesRequest
 from data_point_client.models.data_point_request import DataPointRequest
 from data_point_client.models.day_data_by_hour_transfer import DayDataByHourTransfer
 from data_point_client.models.en_data_point_existence_dto import EnDataPointExistenceDTO
 from data_point_client.models.get_data_request import GetDataRequest
 from data_point_client.models.get_day_period_response import GetDayPeriodResponse
 from data_point_client.models.get_week_period_response import GetWeekPeriodResponse
 from data_point_client.models.problem_details import ProblemDetails
 from data_point_client.models.sub_series_request import SubSeriesRequest
 from data_point_client.models.sub_series_request_values import SubSeriesRequestValues
 from data_point_client.models.time_series_response_curve import TimeSeriesResponseCurve
-from data_point_client.models.update_constant_data_request import UpdateConstantDataRequest
+from data_point_client.models.update_constant_data_request import (
+    UpdateConstantDataRequest,
+)
 from data_point_client.models.update_time_series_request import UpdateTimeSeriesRequest
 from data_point_client.models.update_week_period_request import UpdateWeekPeriodRequest
 from data_point_client.models.week_data_transfere import WeekDataTransfere
 from data_point_client.types import Response, Unset
 from nista_library.nista_connetion import NistaConnection
 
 log = get_logger()
 
 # pylint: disable=C0103
 T = TypeVar("T", bound="NistaDataPoint")
 
 
 class NistaDataPoint:
+    """Represents a DataPoint from nista.io
+    :DATE_FORMAT: Format to use for parse dictionaries
+    :DATE_NAME: Column Name for Dates
+    :VALUE_NAME: Column Name for Value
+    """
+
     DATE_FORMAT = "%Y-%m-%dT%H:%M:%SZ"
     DATE_NAME = "Date"
     VALUE_NAME = "Value"
 
+    _data_point_response: Optional[DataPointResponseBase] = None
+
+    @property
+    def data_point_response(self) -> Optional[DataPointResponseBase]:
+        """Loads and interprets the DataPoint if it has not bee loaded.
+        :returns: The DataPoint Details from nista.io
+        """
+        if self._data_point_response is None:
+            self._load_details()
+        return self._data_point_response
+
     @classmethod
-    def create_new(cls: Type[T], connection: NistaConnection, name: str, tags: List[str]) -> Optional[T]:
+    def create_new(
+        cls: Type[T], connection: NistaConnection, name: str, tags: List[str]
+    ) -> Optional[T]:
+        """Creates a new DataPoint in nista.io
+        :param connection: To be used to connecto to nista.io
+        :param name: The new name of the DataPoint
+        :param tags: List of Tags to add to the new DataPoint
+        :returns: The created DataPoint
+        """
+
         token = connection.get_access_token()
         client = AuthenticatedClient(
-            base_url=connection.datapoint_base_url, token=token, verify_ssl=connection.verify_ssl
+            base_url=connection.datapoint_base_url,
+            token=token,
+            verify_ssl=connection.verify_ssl,
         )
 
         new_id = uuid.uuid4()
-        request = DataPointRequest(name=name, description="", existence=EnDataPointExistenceDTO.FULL, tags=tags)
+        request = DataPointRequest(
+            name=name, description="", existence=EnDataPointExistenceDTO.FULL, tags=tags
+        )
 
         response = data_point_create_data_point.sync(
-            client=client, data_point_id=str(new_id), workspace_id=connection.workspace_id, json_body=request
+            client=client,
+            data_point_id=str(new_id),
+            workspace_id=connection.workspace_id,
+            json_body=request,
         )
 
         if isinstance(response, ProblemDetails):
             log.error(response)
             return None
 
         data_point = cls(connection=connection, data_point_id=new_id, name=name)
         return data_point
 
-    def __init__(self, connection: NistaConnection, data_point_id: uuid.UUID, name: Optional[str] = None):
+    def __init__(
+        self,
+        connection: NistaConnection,
+        data_point_id: uuid.UUID,
+        name: Optional[str] = None,
+    ):
+        """Load a DataPoint from nista.io
+        :param connection: To be used to connecto to nista.io
+        :param data_point_id: The Unique ID to load the DataPoint
+        :param name: Optional Name to use for this DataPoint
+        """
+
         self.connection = connection
         self.data_point_id = data_point_id
         if name is None:
             self._load_details()
         else:
             self.name = name
 
     def __str__(self):
-        return "NistaDataPoint " + self.data_point_id + " with name " + self.name
+        return "NistaDataPoint " + str(self.data_point_id) + " with name " + self.name
 
     def _load_details(self):
         token = self.connection.get_access_token()
         client = AuthenticatedClient(
-            base_url=self.connection.datapoint_base_url, token=token, verify_ssl=self.connection.verify_ssl
+            base_url=self.connection.datapoint_base_url,
+            token=token,
+            verify_ssl=self.connection.verify_ssl,
         )
 
         data_point = data_point_get_data_point.sync(
             client=client,
             data_point_id=self.data_point_id,
             workspace_id=self.connection.workspace_id,
         )
 
         if data_point is None:
             raise ValueError("Cannot load Datapoint")
 
-        self.name = data_point.names
-        self.data_point_response = data_point
+        if isinstance(data_point, ProblemDetails):
+            log.error(data_point)
+            raise ValueError("Cannot load Datapoint")
+
+        self._data_point_response = data_point
+        self.name = self.data_point_response.name
 
     # pylint: disable=too-many-arguments
     def get_data_point_data(
         self,
         request: GetDataRequest,
         post_fix: bool = False,
         timeout: float = 30,
-    ) -> Union[List[DataFrame], float, Unset, WeekDataTransfere, DayDataByHourTransfer, None]:
+    ) -> Union[
+        List[DataFrame], float, Unset, WeekDataTransfere, DayDataByHourTransfer, None
+    ]:
+        """Retrieves the Data from a DataPoint
+        :param request: Request details for retrieving Data
+        :param post_fix: Append nista.io instance name after DataPoint Name
+        :param timeout: How long to wait for response
+        :return: The DataPoint Data
+        """
+
         token = self.connection.get_access_token()
         client = AuthenticatedClient(
             base_url=self.connection.datapoint_base_url,
             token=token,
             verify_ssl=self.connection.verify_ssl,
             timeout=timeout,
         )
@@ -135,15 +199,17 @@
             if isinstance(curves, list):
                 data_frames = []
                 # pylint: disable=E1133
                 for curve in curves:
                     # pylint: enable=E1133
                     curve_dict = curve.curve
                     if isinstance(curve_dict, TimeSeriesResponseCurve):
-                        data_frame = self._from_time_frames(time_frames=curve_dict.to_dict(), post_fix=post_fix)
+                        data_frame = self._from_time_frames(
+                            time_frames=curve_dict.to_dict(), post_fix=post_fix
+                        )
                         data_frames.append(data_frame)
 
                 return data_frames
 
         if content_type == "GetConstantResponse":
             constant_response = GetConstantResponse.from_dict(jscon_content)
             if constant_response is not None:
@@ -158,16 +224,25 @@
             day_response = GetDayPeriodResponse.from_dict(jscon_content)
             if day_response is not None:
                 return day_response.day_data
 
         return None
 
     def append_data_point_data(
-        self, data: Union[List[DataFrame], float], unit: Optional[str] = None, timeout: float = 5.0
+        self,
+        data: Union[List[DataFrame], float],
+        unit: Optional[str] = None,
+        timeout: float = 5.0,
     ) -> Optional[Response[Union[Any, ProblemDetails]]]:
+        """Append data to an existing DataPoint
+        :param data: To be added to a DataPoint
+        :param unit: The Unit to set on the DataPoint Store
+        :param timeout: How long to wait for response
+        """
+
         token = self.connection.get_access_token()
         client = AuthenticatedClient(
             base_url=self.connection.datapoint_base_url,
             token=token,
             verify_ssl=self.connection.verify_ssl,
             timeout=timeout,
         )
@@ -188,16 +263,26 @@
                 data_point_id=str(self.data_point_id),
                 json_body=append_request,
             )
 
         return None
 
     def append_data_point_result_parts(
-        self, data: Union[List[DataFrame], float], unit: Optional[str], execution_id: uuid.UUID, timeout: float = 5.0
+        self,
+        data: Union[List[DataFrame], float],
+        unit: Optional[str],
+        execution_id: uuid.UUID,
+        timeout: float = 5.0,
     ) -> Optional[Response[Union[Any, ProblemDetails]]]:
+        """Append data as an execution Result. This method is used for nista.io Internal Execution handling
+        :param data: To be added to a DataPoint
+        :param unit: The Unit to set on the DataPoint Store
+        :param execution_id: the execution ID that this data is assignable to
+        :param timeout: How long to wait for response
+        """
         token = self.connection.get_access_token()
         client = AuthenticatedClient(
             base_url=self.connection.datapoint_base_url,
             token=token,
             verify_ssl=self.connection.verify_ssl,
             timeout=timeout,
         )
@@ -226,21 +311,31 @@
     def set_data_point_data(
         self,
         data: Union[List[DataFrame], float, WeekDataTransfere],
         unit: Optional[str] = None,
         execution_id: Optional[str] = None,
         time_zone: Optional[ZoneInfo] = None,
     ) -> Optional[Response[Union[Any, ProblemDetails]]]:
+        """Replace or Set DataPoint Data with new Data. This bumps the DataPoint Version
+        :param data: To be added to a DataPoint
+        :param unit: The Unit to set on the DataPoint Store
+        :param execution_id: the execution ID that this data is assignable to
+        :param time_zone: The Time Zone of the newly added Data
+        """
         token = self.connection.get_access_token()
         client = AuthenticatedClient(
-            base_url=self.connection.datapoint_base_url, token=token, verify_ssl=self.connection.verify_ssl
+            base_url=self.connection.datapoint_base_url,
+            token=token,
+            verify_ssl=self.connection.verify_ssl,
         )
 
         if isinstance(data, WeekDataTransfere):
-            week_update_request = UpdateWeekPeriodRequest(execution_id=execution_id, unit=unit, week_data=data)
+            week_update_request = UpdateWeekPeriodRequest(
+                execution_id=execution_id, unit=unit, week_data=data
+            )
             return data_point_update_week_period_data.sync_detailed(
                 workspace_id=self.connection.workspace_id,
                 client=client,
                 data_point_id=str(self.data_point_id),
                 json_body=week_update_request,
             )
 
@@ -290,36 +385,44 @@
         dct = data_frame.to_dict()[self.VALUE_NAME]
         for key in dct.keys():
             value = dct[key]
             key_string = key.strftime(self.DATE_FORMAT)
             result[key_string] = value
         return result
 
-    def _from_time_frames(self, time_frames: dict, post_fix: bool, date_format: str = DATE_FORMAT) -> DataFrame:
+    def _from_time_frames(
+        self, time_frames: dict, post_fix: bool, date_format: str = DATE_FORMAT
+    ) -> DataFrame:
         if not isinstance(time_frames, dict):
             raise TypeError
 
         value_column_name = self.name
 
         if value_column_name is None:
             value_column_name = self.VALUE_NAME
 
         if post_fix:
-            value_column_name = value_column_name + "_nista.io_" + str(self.data_point_id)
+            value_column_name = (
+                value_column_name + "_nista.io_" + str(self.data_point_id)
+            )
 
         log.debug("Reading data as Pandas DataFrame")
 
         data_record = []
         for date in time_frames:
             value = time_frames[date]
             data_record.append({self.DATE_NAME: date, value_column_name: value})
 
-        data_frame = pd.DataFrame.from_records(data_record, columns=[self.DATE_NAME, value_column_name])
+        data_frame = pd.DataFrame.from_records(
+            data_record, columns=[self.DATE_NAME, value_column_name]
+        )
 
-        data_frame[self.DATE_NAME] = pd.to_datetime(data_frame[self.DATE_NAME], format=date_format)
+        data_frame[self.DATE_NAME] = pd.to_datetime(
+            data_frame[self.DATE_NAME], format=date_format
+        )
 
         data_frame[value_column_name] = pd.to_numeric(data_frame[value_column_name])
 
         data_frame = data_frame.set_index(data_frame[self.DATE_NAME])
         data_frame = data_frame.drop([self.DATE_NAME], axis=1)
 
         return data_frame
```

### Comparing `nista_library-4.0.1/nista_library/nista_data_points.py` & `nista_library-4.0.2/nista_library/nista_data_points.py`

 * *Files 11% similar despite different names*

```diff
@@ -9,18 +9,28 @@
 from nista_library.nista_connetion import NistaConnection
 from nista_library.nista_data_point import NistaDataPoint
 
 log = get_logger()
 
 
 class NistaDataPoints:
+    """Represents a DataPoint List from nista.io
+    """
     def __init__(self, connection: NistaConnection):
+        """Create a List of DataPoints
+        :param connection: To be used to connecto to nista.io
+        """
+
         self.connection = connection
 
     def get_data_point_list(self) -> Generator[NistaDataPoint, None, None]:
+        """Retrieve a List of DataPoints for a nista.io workspace
+        :return: List of DataPoints found in nista.io workspace
+        """
+
         token = self.connection.get_access_token()
         client = AuthenticatedClient(
             base_url=self.connection.datapoint_base_url, token=token, verify_ssl=self.connection.verify_ssl
         )
 
         data_point_list = data_point_get_data_points.sync(
             workspace_id=self.connection.workspace_id, client=client, existence=[EnDataPointExistenceDTO.FULL]
```

### Comparing `nista_library-4.0.1/pyproject.toml` & `nista_library-4.0.2/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,54 +1,53 @@
 [tool.poetry]
 name = "nista-library"
-version = "4.0.1"
+version = "4.0.2"
 description = "A client library for accessing nista.io"
 license = "MIT"
 
 authors = ["Markus Hoffmann <markus.hoffmann@nista.io>"]
 
-readme = [
-  "README.md",
-  "SAMPLES.md"
-]
+readme = "README.md"
 homepage = "https://nista.io"
 repository = "https://gitlab.com/campfiresolutions/public/nista.io-python-library.git"
 
 packages = [
     {include = "data_point_client"},
     {include = "nista_library"},
 ]
 include = ["LICENSE.md", "data_point_client/py.typed"]
 
 
 [tool.poetry.dependencies]
-python = ">=3.9"
+python = ">=3.9,<4.0"
 httpx = ">=0.15.4,<1.0.0"
 attrs = ">=20.1.0,<23.0.0"
 python-dateutil = "^2.8.0"
 pandas = "^1.3.2"
 oauth2-client = "^1.2.1"
 PyJWT = "^2.3.0"
 structlog = ">=21.0.0,<22.0.0"
 colorama = "^0.4.4"
 keyring = "^23.5.0"
 pyjwt = "^2.6.0"
 
 
 [tool.poetry.dev-dependencies]
+python = ">=3.9,<4.0"
 pytest = "^6.2.5"
 mypy = "<1.0"
 flake8 = "<6.0.0"
 pylint = "<3.0.0"
-black = "<23.0.0"
-openapi-python-client = "<0.14.0"
-typer = "^0.4.1"
 
 [tool.poetry.group.dev.dependencies]
-black = {version = "^22.10.0", allow-prereleases = true}
+black = {version = "^23.0.0", allow-prereleases = true}
+sphinx = "^7.0.1"
+sphinx-markdown-builder = "^0.5.5"
+openapi-python-client = "^0.14.0"
+sphinx-autodoc-typehints = "^1.23.0"
 
 [tool.black]
 line-length = 120
 target_version = ['py38']
 exclude = '''
 (
   /(
```

