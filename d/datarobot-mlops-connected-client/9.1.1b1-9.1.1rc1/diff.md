# Comparing `tmp/datarobot_mlops_connected_client-9.1.1b1-py3-none-any.whl.zip` & `tmp/datarobot_mlops_connected_client-9.1.1rc1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,15 +1,15 @@
-Zip file size: 39453 bytes, number of entries: 13
--rw-r--r--  2.0 unx      597 b- defN 23-Mar-27 23:33 datarobot/mlops/__init__.py
--rw-r--r--  2.0 unx      532 b- defN 23-Mar-27 23:33 datarobot/mlops/connected/__init__.py
--rw-r--r--  2.0 unx    94846 b- defN 23-Mar-27 23:33 datarobot/mlops/connected/client.py
--rw-r--r--  2.0 unx     1231 b- defN 23-Mar-27 23:33 datarobot/mlops/connected/enums.py
--rw-r--r--  2.0 unx      900 b- defN 23-Mar-27 23:33 datarobot/mlops/connected/exception.py
--rw-r--r--  2.0 unx    96728 b- defN 23-Mar-27 23:33 datarobot/mlops/connected/mlops_cli.py
--rw-r--r--  2.0 unx     2646 b- defN 23-Mar-27 23:33 datarobot/mlops/connected/upload_tracker.py
--rw-r--r--  2.0 unx    10251 b- defN 23-Mar-27 23:33 datarobot/mlops/connected/url_helper.py
--rw-r--r--  2.0 unx     1536 b- defN 23-Mar-27 23:38 datarobot_mlops_connected_client-9.1.1b1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Mar-27 23:38 datarobot_mlops_connected_client-9.1.1b1.dist-info/WHEEL
--rw-r--r--  2.0 unx       72 b- defN 23-Mar-27 23:38 datarobot_mlops_connected_client-9.1.1b1.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       10 b- defN 23-Mar-27 23:38 datarobot_mlops_connected_client-9.1.1b1.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1275 b- defN 23-Mar-27 23:38 datarobot_mlops_connected_client-9.1.1b1.dist-info/RECORD
-13 files, 210716 bytes uncompressed, 37255 bytes compressed:  82.3%
+Zip file size: 42665 bytes, number of entries: 13
+-rw-r--r--  2.0 unx      597 b- defN 23-May-18 21:10 datarobot/mlops/__init__.py
+-rw-r--r--  2.0 unx      532 b- defN 23-May-18 21:10 datarobot/mlops/connected/__init__.py
+-rw-r--r--  2.0 unx   106180 b- defN 23-May-18 21:10 datarobot/mlops/connected/client.py
+-rw-r--r--  2.0 unx     1231 b- defN 23-May-18 21:10 datarobot/mlops/connected/enums.py
+-rw-r--r--  2.0 unx      900 b- defN 23-May-18 21:10 datarobot/mlops/connected/exception.py
+-rw-r--r--  2.0 unx   110928 b- defN 23-May-18 21:10 datarobot/mlops/connected/mlops_cli.py
+-rw-r--r--  2.0 unx     2646 b- defN 23-May-18 21:10 datarobot/mlops/connected/upload_tracker.py
+-rw-r--r--  2.0 unx    11367 b- defN 23-May-18 21:10 datarobot/mlops/connected/url_helper.py
+-rw-r--r--  2.0 unx     1537 b- defN 23-May-18 21:15 datarobot_mlops_connected_client-9.1.1rc1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-18 21:15 datarobot_mlops_connected_client-9.1.1rc1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       72 b- defN 23-May-18 21:15 datarobot_mlops_connected_client-9.1.1rc1.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       10 b- defN 23-May-18 21:15 datarobot_mlops_connected_client-9.1.1rc1.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1282 b- defN 23-May-18 21:15 datarobot_mlops_connected_client-9.1.1rc1.dist-info/RECORD
+13 files, 237374 bytes uncompressed, 40457 bytes compressed:  83.0%
```

## zipnote {}

```diff
@@ -18,23 +18,23 @@
 
 Filename: datarobot/mlops/connected/upload_tracker.py
 Comment: 
 
 Filename: datarobot/mlops/connected/url_helper.py
 Comment: 
 
-Filename: datarobot_mlops_connected_client-9.1.1b1.dist-info/METADATA
+Filename: datarobot_mlops_connected_client-9.1.1rc1.dist-info/METADATA
 Comment: 
 
-Filename: datarobot_mlops_connected_client-9.1.1b1.dist-info/WHEEL
+Filename: datarobot_mlops_connected_client-9.1.1rc1.dist-info/WHEEL
 Comment: 
 
-Filename: datarobot_mlops_connected_client-9.1.1b1.dist-info/entry_points.txt
+Filename: datarobot_mlops_connected_client-9.1.1rc1.dist-info/entry_points.txt
 Comment: 
 
-Filename: datarobot_mlops_connected_client-9.1.1b1.dist-info/top_level.txt
+Filename: datarobot_mlops_connected_client-9.1.1rc1.dist-info/top_level.txt
 Comment: 
 
-Filename: datarobot_mlops_connected_client-9.1.1b1.dist-info/RECORD
+Filename: datarobot_mlops_connected_client-9.1.1rc1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## datarobot/mlops/connected/client.py

```diff
@@ -15,14 +15,15 @@
 import logging
 import math
 import os
 import tempfile
 import time
 import warnings
 from contextlib import suppress
+from functools import partial
 
 import aiohttp
 import requests
 
 from datarobot.mlops.common.aggregation_util import convert_aggregated_stats_features_to_dr_format
 from datarobot.mlops.common.aggregation_util import (
     convert_aggregated_stats_predictions_to_dr_format,
@@ -63,14 +64,15 @@
 DATAROBOT_APP_VERSION_WITH_SKIP_AGGREGATION_SUPPORT = DataRobotAppVersion(major=8, minor=0, patch=6)
 
 
 class MMMLimits:
     DATA_REPORTING_MAX_CHUNKS = 100
     DATA_REPORTING_MAX_LINES_PER_CHUNK = 100
     ACTUALS_REPORTING_MAX_LINES = 10000
+    CUSTOM_METRICS_REPORTING_MAX_LINES = 10000
 
 
 class MLOpsClient:
     """
     This class provides helper methods to communicate with
     DataRobot MLOps.
     *Note*: These class methods can only be run from a node
@@ -97,14 +99,15 @@
     RESPONSE_TARGET_KEY = "target"
     RESPONSE_TARGET_TYPE_KEY = "type"
     RESPONSE_MODEL_TARGET_TYPE_KEY = "targetType"
     RESPONSE_LOCATION_KEY = "Location"
     RESPONSE_FULL_API_VERSION = "versionString"
     RESPONSE_API_MAJOR_VERSION = "major"
     RESPONSE_API_MINOR_VERSION = "minor"
+    RESPONSE_CUSTOM_METRIC_ID_KEY = "id"
 
     ASYNC_STATUS_ACTIVE = "active"
     ASYNC_STATUS_ERROR = "error"
     ASYNC_STATUS_ABORT = "abort"
     ASYNC_STATUS_INITIALIZED = "initialized"
     ASYNC_STATUS_RUNNING = "running"
     ASYNC_WAIT_SLEEP_TIME = 2
@@ -600,15 +603,15 @@
         :returns: dataset ID
         :rtype: str
         """
         dataset_id = self.upload_dataset(dataset_filepath)
         self.associate_deployment_dataset(deployment_id, dataset_id, DatasetSourceType.SCORING)
         return dataset_id
 
-    def submit_actuals(self, deployment_id, actuals, wait_for_result=True, timeout=180):
+    async def submit_actuals(self, deployment_id, actuals, wait_for_result=True, timeout=180):
         """
         :param deployment_id: ID of the deployment for which the actuals are being submitted
         :param actuals: List of actuals with schema:
                         Regression: {"actualValue": 23, "wasActedOn": False / True,
                         "timestamp": RFC3339 timestamp, "associationId": "x_23423_23423"}
                         Binary: {"actualValue": "<className>", "wasActedOn": False / True,
                         "timestamp": RFC3339 timestamp, "associationId": "x_23423_23423"}
@@ -651,53 +654,64 @@
                     )
                 )
 
         url = self._url_builder.report_actuals(deployment_id)
         headers = dict(self._common_headers)
         headers.update({"Content-Type": "application/json"})
         data = {"data": actuals}
-        response = requests.post(
-            url, headers=headers, data=json_dumps_bytes(data), verify=self._verify
-        )
-        if response.status_code != HTTPStatus.ACCEPTED:
-            raise DRMLOpsConnectedException(f"Failed to post actuals: {response.text}")
-        if wait_for_result:
-            self._wait_for_async_completion(
-                response.headers[MLOpsClient.RESPONSE_LOCATION_KEY], timeout
+        try:
+            response = await self._session.post(
+                url, headers=headers, data=json_dumps_bytes(data), verify_ssl=self._verify
+            )
+            if response.status == HTTPStatus.NOT_FOUND:
+                raise DRNotFoundException(f"Deployment ID {deployment_id} not found.")
+            if response.status != HTTPStatus.ACCEPTED:
+                message = await response.text()
+                raise DRMLOpsConnectedException(f"Failed to post actuals: {message}")
+            if response.ok:
+                json_response = await response.json()
+                if wait_for_result:
+                    self._wait_for_async_completion(
+                        response.headers[MLOpsClient.RESPONSE_LOCATION_KEY], timeout
+                    )
+                return json_response
+            message = await response.text()
+            raise DRMLOpsConnectedException(f"Call {url} failed; text: [{message}]")
+        except requests.exceptions.ConnectionError as e:
+            raise DRMLOpsConnectedException(
+                f"Connection to DataRobot MLOps [{self._service_url}] refused: {e}"
             )
-        return response
 
     @staticmethod
     def _validate_col_exists(df, col_name):
         if col_name not in df.columns:
             raise Exception(f"Data does not include {col_name} column")
 
     @staticmethod
-    def _get_correct_actual_value(deployment_type, value):
+    def _get_correct_actual_value(value, deployment_type="Regression"):
         if deployment_type == "Regression":
             return float(value)
         return str(value)
 
     @staticmethod
     def _get_correct_flag_value(value_str):
         if value_str == "True":
             return True
         return False
 
-    def submit_actuals_from_dataframe(
+    async def submit_actuals_from_dataframe(
         self,
         deployment_id,
         dataframe,
         assoc_id_col=Constants.ACTUALS_ASSOCIATION_ID_KEY,
         actual_value_col=Constants.ACTUALS_VALUE_KEY,
         was_act_on_col=Constants.ACTUALS_WAS_ACTED_ON_KEY,
         timestamp_col=Constants.ACTUALS_TIMESTAMP_KEY,
         progress_callback=None,
-        wait_for_result=True,
-        timeout=120,
+        dry_run=False,
     ):
         """
         Submit actuals to MLOps App from the given DataFrame.
         This call will specific columns of the DataFrame to extract the association ids,
         actual values of predictions and other information. The data will be submitted to the
         MLOps app chunk by chunk, where the maximal chunk size is 10K lines.
 
@@ -730,75 +744,90 @@
 
         # Renaming the columns in case the columns needed are not in the expected name
         cols_to_rename = {}
         if assoc_id_col != Constants.ACTUALS_ASSOCIATION_ID_KEY:
             cols_to_rename[assoc_id_col] = Constants.ACTUALS_ASSOCIATION_ID_KEY
         if actual_value_col != Constants.ACTUALS_VALUE_KEY:
             cols_to_rename[actual_value_col] = Constants.ACTUALS_VALUE_KEY
-        if was_act_on_col != Constants.ACTUALS_WAS_ACTED_ON_KEY:
+        if was_act_on_col and was_act_on_col != Constants.ACTUALS_WAS_ACTED_ON_KEY:
             cols_to_rename[was_act_on_col] = Constants.ACTUALS_WAS_ACTED_ON_KEY
         if timestamp_col and timestamp_col != Constants.ACTUALS_TIMESTAMP_KEY:
             cols_to_rename[timestamp_col] = Constants.ACTUALS_TIMESTAMP_KEY
         dataframe = dataframe.rename(columns=cols_to_rename)
 
         # Taking only the columns we need for the actuals reporting
         cols_to_take = [Constants.ACTUALS_VALUE_KEY, Constants.ACTUALS_ASSOCIATION_ID_KEY]
-        if timestamp_col:
+        if Constants.ACTUALS_TIMESTAMP_KEY in dataframe.columns:
             cols_to_take.append(Constants.ACTUALS_TIMESTAMP_KEY)
         if Constants.ACTUALS_WAS_ACTED_ON_KEY in dataframe.columns:
             cols_to_take.append(Constants.ACTUALS_WAS_ACTED_ON_KEY)
 
         dataframe = dataframe[cols_to_take]
         # ensure the association ID is a string
         dataframe[Constants.ACTUALS_ASSOCIATION_ID_KEY] = dataframe[
             Constants.ACTUALS_ASSOCIATION_ID_KEY
         ].map(str)
 
-        # Iterating over the rows of the DataFrame and building the actuals list of dictionaries
         deployment_type = self.get_deployment_type(deployment_id)
-        actuals = []
-
-        request_ret_val = None
+        dataframe[Constants.ACTUALS_VALUE_KEY].apply(
+            partial(self._get_correct_actual_value, deployment_type=deployment_type)
+        )
+        if Constants.ACTUALS_WAS_ACTED_ON_KEY in dataframe.columns:
+            dataframe[Constants.ACTUALS_WAS_ACTED_ON_KEY].apply(
+                partial(self._get_correct_flag_value)
+            )
 
+        url = self._url_builder.report_actuals(deployment_id)
+        headers = dict(self._common_headers)
+        headers.update({"Content-Type": "application/json"})
         total_number_of_actuals = len(dataframe.index)
+        start = 0
+        aggregate_payload_size = 0
         requests_sent = 0
-        for index, row in dataframe.iterrows():
-            actual = {}
-            for key, value in row.items():
-                if key == Constants.ACTUALS_WAS_ACTED_ON_KEY:
-                    value = self._get_correct_flag_value(value)
-                if key == Constants.ACTUALS_VALUE_KEY:
-                    value = self._get_correct_actual_value(deployment_type, value)
-                actual[key] = value
-            actuals.append(actual)
-            if len(actuals) == MMMLimits.ACTUALS_REPORTING_MAX_LINES:
+        while start < total_number_of_actuals:
+            end = start + MMMLimits.ACTUALS_REPORTING_MAX_LINES
+            if end > total_number_of_actuals:
+                end = total_number_of_actuals
+            actuals_chunk = dataframe[start:end]
+            data = {"data": actuals_chunk.to_dict(orient="records")}
+            try:
                 start_time = time.time()
-                request_ret_val = self.submit_actuals(
-                    deployment_id, actuals, wait_for_result=wait_for_result, timeout=timeout
-                )
+                if dry_run:
+                    last_response = {"message": "ok"}
+                else:
+                    response = await self._session.post(
+                        url, headers=headers, data=json_dumps_bytes(data), verify_ssl=self._verify
+                    )
+                    if response.status == HTTPStatus.NOT_FOUND:
+                        raise DRNotFoundException(f"Deployment ID {deployment_id} not found.")
+                    if response.status != HTTPStatus.ACCEPTED:
+                        message = await response.text()
+                        raise DRMLOpsConnectedException(f"Failed to post actuals data: {message}")
+                    if response.ok:
+                        json_response = await response.json(content_type=None)
+                        last_response = json_response
+                    else:
+                        message = await response.text()
+                        raise DRMLOpsConnectedException(f"Call {url} failed; text:[{message}]")
                 end_time = time.time()
+                payload_size = actuals_chunk.shape[0]
+                aggregate_payload_size += payload_size
+                start = end
                 requests_sent += 1
-                if progress_callback:
-                    progress_callback(
-                        total_number_of_actuals,
-                        requests_sent * MMMLimits.ACTUALS_REPORTING_MAX_LINES,
-                        end_time - start_time,
-                    )
-                actuals = []
-        if len(actuals) > 0:
-            start_time = time.time()
-            request_ret_val = self.submit_actuals(
-                deployment_id, actuals, wait_for_result=wait_for_result, timeout=timeout
-            )
-            end_time = time.time()
+            except requests.exceptions.ConnectionError as e:
+                raise DRMLOpsConnectedException(
+                    f"Connection to DataRobot MLOps [{self._service_url}] refused: {e}"
+                )
             if progress_callback:
                 progress_callback(
-                    total_number_of_actuals, total_number_of_actuals, end_time - start_time
+                    total_number_of_actuals,
+                    requests_sent * MMMLimits.ACTUALS_REPORTING_MAX_LINES,
+                    end_time - start_time,
                 )
-        return request_ret_val
+        return last_response, aggregate_payload_size
 
     def create_model_package(self, model_info):
         """
         Create an external model package in DataRobot MLOps from JSON configuration
 
         :param model_info: a JSON object of model parameters
         :type model_info: dict
@@ -1246,20 +1275,30 @@
             raise DRMLOpsConnectedException(f"Call {url} failed; text: [{response.text}]")
         except requests.exceptions.ConnectionError as e:
             raise DRMLOpsConnectedException(
                 f"Connection to DataRobot MLOps [{self._service_url}] refused: {e}"
             )
 
     def _make_list_call(self, url, params=None):
+        data = []
         try:
-            response = self._get_url_request_response(url, params=params)
-            if response.ok:
-                return response.json()["data"]
-            else:
-                raise DRMLOpsConnectedException(f"Call {url} failed; text: [{response.text}]")
+            while True:
+                response = self._get_url_request_response(url, params=params)
+                if response.ok:
+                    json = response.json()
+                    data.extend(json["data"])
+                    if json["next"] is None:
+                        return data
+                    else:
+                        url = json["next"]
+                        # Set params = None, because json["next"] will have all params set
+                        # correctly
+                        params = None
+                else:
+                    raise DRMLOpsConnectedException(f"Call {url} failed; text: [{response.text}]")
         except requests.exceptions.ConnectionError as e:
             raise DRMLOpsConnectedException(
                 f"Connection to DataRobot MLOps [{self._service_url}] refused: {e}"
             )
 
     def list_prediction_environments(self, params=None):
         url = self._url_builder.list_prediction_environments()
@@ -1721,15 +1760,14 @@
         payload = self.payload_report_aggregated_prediction_data(
             model_id=model_id,
             aggregated_stats=aggregated_stats,
             timestamp=timestamp,
             batch_name=batch_name,
         )
         payload = json_dumps_bytes(payload, default=default_serializer)
-
         try:
             if dry_run:
                 return {"message": "ok"}
             else:
                 response = await self._session.post(
                     url, headers=headers, data=payload, verify_ssl=self._verify
                 )
@@ -1746,15 +1784,15 @@
                     message = await response.text()
                     raise DRMLOpsConnectedException(f"Call {url} failed; text:[{message}]")
         except requests.exceptions.ConnectionError as e:
             raise DRMLOpsConnectedException(
                 f"Connection to DataRobot MLOps [{self._service_url}] refused: {e}"
             )
 
-    def report_actuals_data(self, deployment_id, actuals, dry_run=False):
+    async def report_actuals_data(self, deployment_id, actuals, dry_run=False):
         """
         Report actuals data for a given deployment.
 
         :param deployment_id: deployment ID to use for reporting
         :type deployment_id: str
         :param association_id: association ID of the record
         :type association_id: str
@@ -1766,20 +1804,140 @@
         :type timestamp: str
 
         """
         try:
             if dry_run:
                 return {"message": "ok"}
             else:
-                self.submit_actuals(deployment_id, actuals)
+                await self.submit_actuals(deployment_id, actuals)
+        except requests.exceptions.ConnectionError as e:
+            raise DRMLOpsConnectedException(
+                f"Connection to DataRobot MLOps [{self._service_url}] refused: {e}"
+            )
+
+    async def report_custom_metrics(
+        self,
+        deployment_id,
+        model_id,
+        buckets,
+        custom_metric_id,
+        dry_run=False,
+    ):
+        url = self._url_builder.report_custom_metrics(deployment_id, custom_metric_id)
+        headers = dict(self._common_headers)
+        headers.update({"Content-Type": "application/json"})
+        payload = json_dumps_bytes({"modelId": model_id, "buckets": buckets})
+
+        try:
+            if dry_run:
+                return {"message": "ok"}
+            else:
+                response = await self._session.post(
+                    url, headers=headers, data=payload, verify_ssl=self._verify
+                )
+                if response.status == HTTPStatus.NOT_FOUND:
+                    raise DRNotFoundException(f"Deployment ID {deployment_id} not found.")
+                if response.status != HTTPStatus.ACCEPTED:
+                    message = await response.text()
+                    raise DRMLOpsConnectedException(f"Failed to post custom metrics: {message}")
+                if response.ok:
+                    # MLOps service returns text/html content in response for POST custom metrics
+                    # But, when stub server tries to return same text/html it is still being
+                    # returned as application/json which messes up this parsing.  The common
+                    # ground is content_type = None => Don't try to parse / interpret the content
+                    # Works for the simpler POST case which returns empty response and 202
+                    json_response = await response.json(content_type=None)
+                    return json_response
+                else:
+                    message = await response.text()
+                    raise DRMLOpsConnectedException(f"Call {url} failed; text: [{message}]")
         except requests.exceptions.ConnectionError as e:
             raise DRMLOpsConnectedException(
                 f"Connection to DataRobot MLOps [{self._service_url}] refused: {e}"
             )
 
+    def _get_correct_custom_metrics_timestamp(self, x, timestamp_format=None):
+        if timestamp_format:
+            micro_ts = datetime.datetime.strptime(x, timestamp_format).strftime(
+                "%Y-%m-%d %H:%M:%S.%f%z"
+            )
+            return micro_ts[0:23] + micro_ts[26:]
+        return x
+
+    async def submit_custom_metrics_from_dataframe(
+        self,
+        deployment_id,
+        model_id,
+        custom_metric_id,
+        input_df,
+        timestamp_col,
+        value_col,
+        timestamp_format=None,
+        dry_run=False,
+        progress_callback=None,
+    ):
+        self._validate_col_exists(input_df, timestamp_col)
+        self._validate_col_exists(input_df, value_col)
+
+        dataframe = input_df[[timestamp_col, value_col]]
+        dataframe[timestamp_col].apply(
+            partial(self._get_correct_custom_metrics_timestamp, timestamp_format=timestamp_format)
+        )
+
+        url = self._url_builder.report_custom_metrics(deployment_id, custom_metric_id)
+        headers = dict(self._common_headers)
+        headers.update({"Content-Type": "application/json"})
+        total_number_of_values = len(dataframe.index)
+        start = 0
+        aggregate_payload_size = 0
+        requests_sent = 0
+        while start < total_number_of_values:
+            end = start + MMMLimits.CUSTOM_METRICS_REPORTING_MAX_LINES
+            if end > total_number_of_values:
+                end = total_number_of_values
+            custom_metrics_chunk = dataframe[start:end]
+            data = {"modelId": model_id, "buckets": custom_metrics_chunk.to_dict(orient="records")}
+            try:
+                start_time = time.time()
+                if dry_run:
+                    last_response = {"message": "ok"}
+                else:
+                    response = await self._session.post(
+                        url, headers=headers, data=json_dumps_bytes(data), verify_ssl=self._verify
+                    )
+                    if response.status == HTTPStatus.NOT_FOUND:
+                        raise DRNotFoundException(f"Deployment ID {deployment_id} not found.")
+                    if response.status != HTTPStatus.ACCEPTED:
+                        message = await response.text()
+                        raise DRMLOpsConnectedException(
+                            f"Failed to post custom metrics data: {message}"
+                        )
+                    if response.ok:
+                        json_response = await response.json(content_type=None)
+                        last_response = json_response
+                    else:
+                        message = await response.text()
+                        raise DRMLOpsConnectedException(f"Call {url} failed; text:[{message}]")
+                end_time = time.time()
+                payload_size = custom_metrics_chunk.shape[0]
+                aggregate_payload_size += payload_size
+                start = end
+                requests_sent += 1
+            except requests.exceptions.ConnectionError as e:
+                raise DRMLOpsConnectedException(
+                    f"Connection to DataRobot MLOps [{self._service_url}] refused: {e}"
+                )
+            if progress_callback:
+                progress_callback(
+                    total_number_of_values,
+                    requests_sent * MMMLimits.CUSTOM_METRICS_REPORTING_MAX_LINES,
+                    end_time - start_time,
+                )
+        return last_response, aggregate_payload_size
+
     def _is_model_package_download_from_registry_supported(self):
         if self._api_major_version > 2:
             return True
 
         if self._api_major_version == 2 and self._api_minor_version >= 25:
             return True
 
@@ -2180,14 +2338,97 @@
                 f"Connection to DataRobot MLOps [{self._service_url}] refused: {e}"
             )
 
     def list_batches(self, deployment_id, params=None):
         url = self._url_builder.list_batches(deployment_id)
         return self._make_list_call(url, params)
 
+    def create_custom_metric(self, deployment_id, cm_info):
+        """
+        Create a custom metric in DataRobot MLOps from JSON configuration.
+
+        :param cm_info: a JSON object of custom metric parameters
+        :type pe_info: dict
+        :returns: custom metric ID of newly created custom metric
+        :rtype: str
+        :raises DRMLOpsConnectedException: if creation failed
+
+        Example JSON:
+
+        .. sourcecode:: json
+
+            {
+              "name": "Prediction Environment Name",
+              "description": "Environment used for developing new models",
+              "platform": "Other",
+              "supportedModelFormats": ["external"]
+
+                "name": "Custom Metric Name",
+                "directionality": "higherIsBetter",
+                "units": "$(thousands)",
+                "type": "average",
+                "baselineValues": 100,
+                "isModelSpecific": True,
+                "description": "",
+            }
+
+        """
+
+        try:
+            if "name" not in cm_info:
+                raise DRMLOpsConnectedException("create_custom_metric(): payload is missing name")
+
+            url = self._url_builder.create_custom_metric(deployment_id)
+
+            headers = dict(self._common_headers)
+            headers.update({"Content-Type": "application/json"})
+            response = requests.post(
+                url, data=json_dumps_bytes(cm_info), headers=headers, verify=self._verify
+            )
+            if response.ok:
+                return response.json()[MLOpsClient.RESPONSE_CUSTOM_METRIC_ID_KEY]
+            else:
+                raise DRMLOpsConnectedException(
+                    f"Call {url} with payload {cm_info} failed; text: [{response.text}]"
+                )
+        except requests.exceptions.ConnectionError as e:
+            raise DRMLOpsConnectedException(
+                f"Connection to DataRobot MLOps [{self._service_url}] refused: {e}"
+            )
+
+    def get_custom_metric_summary(self, deployment_id, metric_id, model_id):
+        url = self._url_builder.get_custom_metric_summary(deployment_id, metric_id)
+
+        # Default end time is rounded down to hour.  Because typical use case will have custom
+        # metrics data couple of hours in future - we add a day to end time
+        end = datetime.datetime.utcnow() + datetime.timedelta(days=1)
+        end_str = end.replace(minute=0, second=0, microsecond=0).strftime("%Y-%m-%dT%H:%M:%SZ")
+        params = {"modelId": model_id, "end": end_str}
+        try:
+            response = self._get_url_request_response(url, params=params)
+            if response.ok:
+                return response.json()
+            if response.status_code == HTTPStatus.NOT_FOUND:
+                if "Custom metric not found" in response.text:
+                    raise DRNotFoundException(
+                        "Metric ID {} not found for deployment ID {}.".format(
+                            metric_id, deployment_id
+                        )
+                    )
+                raise DRNotFoundException(f"Deployment ID {deployment_id} not found.")
+            raise DRMLOpsConnectedException(f"Call {url} failed; text: [{response.text}]")
+        except requests.exceptions.ConnectionError as e:
+            raise DRMLOpsConnectedException(
+                f"Connection to DataRobot MLOps [{self._service_url}] refused: {e}"
+            )
+
+    def list_custom_metrics(self, deployment_id, params=None):
+        url = self._url_builder.list_custom_metrics(deployment_id)
+        return self._make_list_call(url, params)
+
     async def shutdown(self):
         if self.__session is not None:
             await self.__session.close()
 
     def __del__(self):
         if self.__session is not None and not self.__session.closed:
             warnings.warn(
```

## datarobot/mlops/connected/mlops_cli.py

```diff
@@ -55,38 +55,41 @@
     MLOPS_TRAINING_DATASET_ID = "MLOPS_TRAINING_DATASET_ID"
     MLOPS_HOLDOUT_DATASET_ID = "MLOPS_HOLDOUT_DATASET_ID"
     MLOPS_DEPLOYMENT_ID = "MLOPS_DEPLOYMENT_ID"
     MLOPS_DEPLOYMENT_LABEL = "MLOPS_DEPLOYMENT_LABEL"
     MLOPS_PREDICTION_ENVIRONMENT_ID = "MLOPS_PREDICTION_ENVIRONMENT_ID"
     MLOPS_DATAROBOT_APP_VERSION = "MLOPS_DATAROBOT_APP_VERSION"
     MLOPS_BATCH_ID = "MLOPS_BATCH_ID"
+    MLOPS_METRIC_ID = "MLOPS_METRIC_ID"
 
 
 class Subjects:
     MAIN_COMMAND = "mlops-cli"
     PERF_TEST = "perf"
     PREDICTIONS = "predictions"
     ACTUALS = "actuals"
     MODEL = "model"
     DATASET = "dataset"
     DEPLOYMENT = "deployment"
     PREDICTION_ENVIRONMENT = "prediction-environment"
     SERVICE_STATS = "service-stats"
     BATCH = "batch"
+    CUSTOM_METRICS = "custom_metric"
 
     ALL_SUBJECTS = [
         PERF_TEST,
         PREDICTIONS,
         ACTUALS,
         MODEL,
         DATASET,
         DEPLOYMENT,
         PREDICTION_ENVIRONMENT,
         SERVICE_STATS,
         BATCH,
+        CUSTOM_METRICS,
     ]
 
 
 class Actions:
     UPLOAD = "upload"
     DOWNLOAD = "download"
     CREATE = "create"
@@ -122,26 +125,28 @@
     ACTUALS_ACTIONS = [REPORT]
     MODEL_ACTIONS = [DOWNLOAD, CREATE, GET, LIST, DELETE, REPLACE, DEPLOY]
     DATASET_ACTIONS = [UPLOAD, GET, LIST, DELETE]
     DEPLOYMENT_ACTIONS = [GET, LIST, DELETE, GET_MODEL]
     PREDICTION_ENVIRONMENT_ACTIONS = [CREATE, GET, LIST, DELETE]
     SERVICE_STATS_ACTIONS = [GET]
     BATCH_ACTIONS = [GET, LIST]
+    CUSTOM_METRICS_ACTIONS = [CREATE, GET, LIST, REPORT]
 
 
 SUPPORTED_ACTIONS = {
     Subjects.PERF_TEST: Actions.PERF_ACTIONS,
     Subjects.PREDICTIONS: Actions.PREDICTIONS_ACTIONS,
     Subjects.ACTUALS: Actions.ACTUALS_ACTIONS,
     Subjects.MODEL: Actions.MODEL_ACTIONS,
     Subjects.DATASET: Actions.DATASET_ACTIONS,
     Subjects.DEPLOYMENT: Actions.DEPLOYMENT_ACTIONS,
     Subjects.PREDICTION_ENVIRONMENT: Actions.PREDICTION_ENVIRONMENT_ACTIONS,
     Subjects.SERVICE_STATS: Actions.SERVICE_STATS_ACTIONS,
     Subjects.BATCH: Actions.BATCH_ACTIONS,
+    Subjects.CUSTOM_METRICS: Actions.CUSTOM_METRICS_ACTIONS,
 }
 
 
 class ArgumentsOptions:
     VERBOSE = "--verbose"
     QUIET = "--quiet"
     JSON = "--json"
@@ -186,26 +191,29 @@
     SEGMENT_ATTRIBUTES = "--segment-attributes"
     DATAROBOT_APP_VERSION = "--datarobot-app-version"
     BATCH_NAME = "--batch-name"
     ENABLE_BATCH_MONITORING = "--enable-batch-monitoring"
     BATCH_ID = "--batch-id"
     QUERY_BATCH_SERVICE_STATS = "--service-stats"
     QUERY_BATCH_DATA_DRIFT = "--data-drift"
+    METRIC_ID = "--metric-id"
+    VALUE_COL = "--value-col"
 
 
 class RunMode(Enum):
     PERF_TEST = Subjects.PERF_TEST
     PREDICTIONS = Subjects.PREDICTIONS
     ACTUALS = Subjects.ACTUALS
     MODEL = Subjects.MODEL
     DATASET = Subjects.DATASET
     DEPLOYMENT = Subjects.DEPLOYMENT
     PREDICTION_ENVIRONMENT = Subjects.PREDICTION_ENVIRONMENT
     SERVICE_STATS = Subjects.SERVICE_STATS
     BATCH = Subjects.BATCH
+    CUSTOM_METRICS = Subjects.CUSTOM_METRICS
 
     @staticmethod
     def list_all():
         all_subjects = ""
         for m in RunMode:
             all_subjects = f"{all_subjects} {m.value}"
         return all_subjects
@@ -221,14 +229,15 @@
 ]
 
 
 common_fields_keys = SerializationConstants.GeneralConstants
 deployment_stats_keys = SerializationConstants.DeploymentStatsConstants
 predictions_data_keys = SerializationConstants.PredictionsDataConstants
 external_events_keys = SerializationConstants.EventConstants
+custom_metric_keys = SerializationConstants.CustomMetricStatsConstants
 config_keys = config.ConfigConstants
 
 
 class MLOpsCliArgParser:
     SUBJECT_KEYWORD = "subject"
     ACTION_KEYWORD = "action"
 
@@ -607,14 +616,23 @@
                 ArgumentsOptions.TIMESTAMP_COL,
                 default=None,
                 type=str,
                 help="Name of timestamp column in input data",
             )
 
     @staticmethod
+    def _register_value_col(*parsers):
+        for parser in parsers:
+            parser.add_argument(
+                ArgumentsOptions.VALUE_COL,
+                type=str,
+                help="Name of value column holding custom metrics values",
+            )
+
+    @staticmethod
     def _register_timestamp_format(*parsers):
         for parser in parsers:
             parser.add_argument(
                 ArgumentsOptions.TIMESTAMP_FORMAT,
                 default=None,
                 type=str,
                 help="Format of timestamp column in input data",
@@ -739,14 +757,25 @@
                 default=os.environ.get(EV.MLOPS_BATCH_ID, None),
                 help="Batch ID to use for querying batch statistics (env: {})".format(
                     EV.MLOPS_BATCH_ID
                 ),
             )
 
     @staticmethod
+    def _register_arg_metric_id(*parsers):
+        for parser in parsers:
+            parser.add_argument(
+                ArgumentsOptions.METRIC_ID,
+                default=os.environ.get(EV.MLOPS_METRIC_ID, None),
+                help="Metric ID to use for querying custom metric statistics (env: {})".format(
+                    EV.MLOPS_METRIC_ID
+                ),
+            )
+
+    @staticmethod
     def _gen_parser(subcommand, help_msg, description=None):
         subparser = MLOpsCliArgParser._subparsers.add_parser(
             subcommand, help=help_msg, description=description, formatter_class=RawTextHelpFormatter
         )
         MLOpsCliArgParser._parsers[subcommand] = subparser
         return subparser
 
@@ -889,19 +918,21 @@
         MLOpsCliArgParser._register_arg_json_conf(parser)
         MLOpsCliArgParser._register_arg_dataset_id(parser)
         MLOpsCliArgParser._register_arg_timeout(parser)
         MLOpsCliArgParser._register_arg_search(parser)
         MLOpsCliArgParser._register_arg_limit(parser)
         MLOpsCliArgParser._register_arg_force(parser)
         MLOpsCliArgParser._register_timestamp_col(parser)
+        MLOpsCliArgParser._register_value_col(parser)
         MLOpsCliArgParser._register_batch_name(parser)
         MLOpsCliArgParser._register_arg_enable_batch_monitoring(parser)
         MLOpsCliArgParser._register_arg_batch_id(parser)
         MLOpsCliArgParser._register_arg_service_stats(parser)
         MLOpsCliArgParser._register_arg_data_drift(parser)
+        MLOpsCliArgParser._register_arg_metric_id(parser)
 
         MLOpsCliArgParser._add_perf_subcommand(parser)
         MLOpsCliArgParser._add_predictions_subcommand(parser)
         MLOpsCliArgParser._add_actuals_subcommand(parser)
         MLOpsCliArgParser._add_model_subcommand(parser)
         return parser
 
@@ -1208,14 +1239,21 @@
                 payload[common_fields_keys.MODEL_ID_FIELD_NAME],
                 payload[deployment_stats_keys.NUM_PREDICTIONS_FIELD_NAME],
                 payload[deployment_stats_keys.EXECUTION_TIME_FIELD_NAME],
                 payload[common_fields_keys.TIMESTAMP_FIELD_NAME],
                 dry_run=self.options.dry_run,
                 batch_name=payload.get(common_fields_keys.BATCH_NAME_FIELD_NAME),
             )
+        elif data_type == DataType.CUSTOM_METRIC:
+            await self.mclient.report_custom_metrics(
+                record.get_deployment_id(),
+                payload.get(common_fields_keys.MODEL_ID_FIELD_NAME),
+                payload[custom_metric_keys.BUCKETS_FIELD_NAME],
+                payload[custom_metric_keys.METRIC_ID_FIELD_NAME],
+            )
         elif data_type == DataType.PREDICTIONS_DATA:
             df, assoc_id, predictions, class_names = [None] * 4
             if predictions_data_keys.FEATURES_FIELD_NAME in payload:
                 df = pd.DataFrame.from_dict(payload[predictions_data_keys.FEATURES_FIELD_NAME])
             if predictions_data_keys.ASSOCIATION_IDS_FIELD_NAME in payload:
                 assoc_id = payload[predictions_data_keys.ASSOCIATION_IDS_FIELD_NAME]
             if predictions_data_keys.PREDICTIONS_FIELD_NAME in payload:
@@ -1238,17 +1276,15 @@
                 ),
                 batch_name=payload.get(common_fields_keys.BATCH_NAME_FIELD_NAME, None),
                 dry_run=self.options.dry_run,
             )
 
             row_count = df.shape[0] if df is not None else len(predictions)
         elif data_type == DataType.ACTUALS_DATA:
-            # unlike DEPLOYMENT_STATS and PREDICTIONS_DATA, this is not currently implemented as
-            # async; these records are small so this may be sufficient
-            self.mclient.report_actuals_data(
+            await self.mclient.report_actuals_data(
                 record.get_deployment_id(),
                 payload[Constants.ACTUALS_LIST_KEY],
                 dry_run=self.options.dry_run,
             )
         elif data_type == DataType.PREDICTION_STATS:
             await self.mclient.report_aggregated_prediction_data(
                 record.get_deployment_id(),
@@ -1482,59 +1518,126 @@
         except DRMLOpsConnectedException as e:
             self._log_error_and_exit(e, ExitCode.DR_CONNECTED.value)
         except Exception as e:
             self._log_error_and_exit(e, ExitCode.UNSPECIFIED.value)
         finally:
             self.delete_mclient()
 
+    async def _report_actuals_connected_lib(self, input_df, row_offset):
+        self._log_report_status(input_df, row_offset)
+
+        request_start_time = time.time()
+        res, payload_size = await self.mclient.submit_actuals_from_dataframe(
+            self.options.deployment_id,
+            input_df,
+            assoc_id_col=self.options.assoc_id_col,
+            actual_value_col=self.options.actual_value_col,
+            was_act_on_col=self.options.acted_on_col,
+            timestamp_col=self.options.timestamp_col,
+            dry_run=self.options.dry_run,
+        )
+        request_end_time = time.time()
+        request_elapsed_ms = (request_end_time - request_start_time) * 1000
+
+        logger.debug(
+            "Row offset: {} payload_size: {} time {:.1f}ms".format(
+                row_offset, payload_size, request_elapsed_ms
+            )
+        )
+
+    def _check_actuals_columns(self, actuals_columns):
+        if self.options.actual_value_col not in actuals_columns:
+            raise DRCommonException(
+                f"Actuals value column {self.options.actual_value_col} missing in the dataframe"
+            )
+
+        if self.options.assoc_id_col not in actuals_columns:
+            raise DRCommonException(
+                f"Association ID column {self.options.assoc_id_col} missing in the dataframe"
+            )
+
+    def _report_actuals_async(self):
+        self.event_loop.run_until_complete(self._actuals_dispatcher())
+
+    async def _actuals_dispatcher(self):
+        num_rows, iteration = self.status_tracker.get_status()
+        tasks = list()
+        for input_df_chunk in self.csv_splitter.get_data_chunks():
+            tasks.append(
+                asyncio.create_task(self._report_actuals_connected_lib(input_df_chunk, num_rows))
+            )
+            num_rows = self.csv_splitter.get_current_row()
+            if len(tasks) == self.options.num_concurrent_requests:
+                break
+
+        while not self.csv_splitter.is_all_data_reported():
+            done, pending = await asyncio.wait(tasks, return_when=asyncio.FIRST_COMPLETED)
+            for task in done:
+                tasks.remove(task)
+                input_df_chunk = self.csv_splitter.get_next_chunk_to_report()
+                if input_df_chunk is None:
+                    continue
+                num_rows = self.csv_splitter.get_current_row()
+                new_task = asyncio.create_task(
+                    self._report_actuals_connected_lib(input_df_chunk, num_rows)
+                )
+                tasks.append(new_task)
+                logger.debug(
+                    "Added new task to report actuals from {} to {}".format(
+                        num_rows, num_rows + self.csv_splitter.get_chunk_size()
+                    )
+                )
+
+        # No more data to report, all tasks submitted, but let's wait for their completion
+        logger.info("Done with submitting all tasks; waiting for them to finish now.")
+        await asyncio.wait(tasks)
+        logger.info("Done reporting all actuals.")
+
     def report_actuals(self):
         check_required_parameter(self.options.deployment_id, None, ArgumentsOptions.DEPLOYMENT_ID)
         check_required_parameter(self.options.input, None, ArgumentsOptions.INPUT)
         check_required_parameter(
             self.options.actual_value_col, None, ArgumentsOptions.ACTUAL_VALUE_COL
         )
         check_required_parameter(self.options.assoc_id_col, None, ArgumentsOptions.ASSOC_ID)
 
-        self.create_mclient()
-
         input_df = pd.read_csv(self.options.input)
 
         logger.info("Reporting actuals:")
         logger.info(f"MLOps service:         {self.options.mlops_service_url}")
         logger.info(f"Deployment ID:         {self.options.deployment_id}")
         logger.info(f"Input:                 {self.options.input}")
         logger.info(f"Input rows:            {len(input_df)}")
         logger.info(f"Actual value column:   {self.options.actual_value_col}")
         logger.info(f"Assoc ID column:       {self.options.assoc_id_col}")
         logger.info(f"Was-acted-on column:   {self.options.acted_on_col}")
         logger.info(f"Timestamp column:      {self.options.timestamp_col}")
 
-        def progress_callback(total_nr_actuals, nr_actuals_sent, request_time):
-            logger.info(
-                "Actuals sent: {} / {} : {:.3f} sec".format(
-                    nr_actuals_sent, total_nr_actuals, request_time
-                )
-            )
+        if self.options.status_file:
+            self.status_tracker = MLOpsUploadTracker(self.options.status_file)
+        else:
+            self.status_tracker = MLOpsUploadTracker()
+        skip_rows, _ = self.status_tracker.get_status()
+        try:
+            self.csv_splitter = MLOpsCSVJSONSplitter(self.options.input, skip_rows=skip_rows)
+            self._check_actuals_columns(self.csv_splitter.get_columns())
+        except (pd.errors.EmptyDataError, DRCommonException) as e:
+            self._log_error_and_exit(e, ExitCode.DEFAULT.value)
 
-        request_start_time = time.time()
-        ret_val = self.mclient.submit_actuals_from_dataframe(
-            self.options.deployment_id,
-            input_df,
-            assoc_id_col=self.options.assoc_id_col,
-            actual_value_col=self.options.actual_value_col,
-            was_act_on_col=self.options.acted_on_col,
-            timestamp_col=self.options.timestamp_col,
-            progress_callback=progress_callback,
-            wait_for_result=self.options.wait,
-            timeout=self.options.timeout,
-        )
-        request_end_time = time.time()
-        request_elapsed_ms = request_end_time - request_start_time
-        logger.debug(f"request: {ret_val} : time {request_elapsed_ms:.2f} sec")
-        self.delete_mclient()
+        try:
+            self.create_mclient()
+            self._report_actuals_async()
+        except DRNotFoundException as e:
+            self._log_error_and_exit(e, ExitCode.DR_NOT_FOUND.value)
+        except DRMLOpsConnectedException as e:
+            self._log_error_and_exit(e, ExitCode.DR_CONNECTED.value)
+        except Exception as e:
+            self._log_error_and_exit(e, ExitCode.UNSPECIFIED.value)
+        finally:
+            self.delete_mclient()
 
     def _generate_temp_csv_filename(self, iteration):
         prefix = "/tmp/" + os.path.basename(self.options.input).replace(".csv", "")
         return prefix + str(iteration) + ".csv"
 
     async def _upload_scoring_dataset_batch(self, input_df, row_offset, iteration):
         """Upload a scoring dataset and associate it with a deployment."""
@@ -2186,14 +2289,231 @@
 
     def handle_service_stats(self):
         if self.options.action == Actions.GET:
             self.get_service_stats()
         else:
             self._print_supported_actions(Subjects.SERVICE_STATS)
 
+    def create_custom_metric(self):
+        check_required_parameter(
+            self.options.deployment_id, EV.MLOPS_DEPLOYMENT_ID, ArgumentsOptions.DEPLOYMENT_ID
+        )
+        check_required_parameter(self.options.json_config, None, ArgumentsOptions.JSON_CONF)
+        try:
+            info = self._read_json_config(self.options.json_config)
+        except FileNotFoundError as e:
+            self._log_error_and_exit(e, ExitCode.FILE_NOT_FOUND.value)
+        self.create_mclient()
+        try:
+            metric_id = self.mclient.create_custom_metric(self.options.deployment_id, info)
+            self._print_resource_generic_action(metric_id)
+            logger.info(f"Created Custom Metric ID {metric_id}.")
+        except DRMLOpsConnectedException as e:
+            self._log_error_and_exit(e, ExitCode.DR_CONNECTED.value)
+        except Exception as e:
+            self._log_error_and_exit(e, ExitCode.UNSPECIFIED.value)
+        finally:
+            self.delete_mclient()
+
+    def get_custom_metric(self):
+        check_required_parameter(
+            self.options.deployment_id, EV.MLOPS_DEPLOYMENT_ID, ArgumentsOptions.DEPLOYMENT_ID
+        )
+        check_required_parameter(
+            self.options.metric_id, EV.MLOPS_METRIC_ID, ArgumentsOptions.METRIC_ID
+        )
+        check_required_parameter(
+            self.options.model_id, EV.MLOPS_MODEL_ID, ArgumentsOptions.MODEL_ID
+        )
+        self.create_mclient()
+        self._log_get_action("deployment", self.options.deployment_id, "custom metric")
+        try:
+            if self.options.metric_id:
+                stats = self.mclient.get_custom_metric_summary(
+                    self.options.deployment_id, self.options.metric_id, self.options.model_id
+                )
+            else:
+                raise Exception(
+                    'Please specify either "--metric-id ' "to query for the given custom metric"
+                )
+            self._print_resource_received(self.options.deployment_id, stats)
+        except DRNotFoundException as e:
+            self._log_error_and_exit(e, ExitCode.DR_NOT_FOUND.value)
+        except DRMLOpsConnectedException as e:
+            self._log_error_and_exit(e, ExitCode.DR_CONNECTED.value)
+        except Exception as e:
+            self._log_error_and_exit(e, ExitCode.UNSPECIFIED.value)
+        finally:
+            self.delete_mclient()
+
+    def list_custom_metrics(self):
+        check_required_parameter(
+            self.options.deployment_id, EV.MLOPS_DEPLOYMENT_ID, ArgumentsOptions.DEPLOYMENT_ID
+        )
+        self._log_get_action("deployment", self.options.deployment_id, "list custom metrics")
+        self.create_mclient()
+        self._log_list_action("custom metrics")
+
+        params = {"offset": 0, "limit": 20}
+        if self.options.limit:
+            params["limit"] = self.options.limit
+
+        matched = []
+        try:
+            all_results = self.mclient.list_custom_metrics(
+                self.options.deployment_id,
+                params=params,
+            )
+            if self.options.search:
+                # Custom Metrics list controller does not support "search" parameter, so
+                # we will implement our own basic search
+                for result in all_results:
+                    if self.options.search in result["name"]:
+                        matched.append(result)
+            else:
+                matched = all_results
+            self._print_resources_listed(matched)
+        except DRMLOpsConnectedException as e:
+            self._log_error_and_exit(e, ExitCode.DR_CONNECTED.value)
+        except Exception as e:
+            self._log_error_and_exit(e, ExitCode.UNSPECIFIED.value)
+        finally:
+            self.delete_mclient()
+
+    async def _report_custom_metrics_connected_lib(self, input_df, row_offset):
+        self._log_report_status(input_df, row_offset)
+
+        request_start_time = time.time()
+        res, payload_size = await self.mclient.submit_custom_metrics_from_dataframe(
+            self.options.deployment_id,
+            self.options.model_id,
+            self.options.metric_id,
+            input_df,
+            timestamp_col=self.options.timestamp_col,
+            value_col=self.options.value_col,
+            timestamp_format=self.options.timestamp_format,
+            dry_run=self.options.dry_run,
+        )
+        request_end_time = time.time()
+        request_elapsed_ms = (request_end_time - request_start_time) * 1000
+
+        logger.debug(
+            "Row offset: {} payload_size: {} time {:.1f}ms".format(
+                row_offset, payload_size, request_elapsed_ms
+            )
+        )
+
+    def _check_custom_metrics_columns(self, custom_metrics_columns):
+        if self.options.timestamp_col not in custom_metrics_columns:
+            raise DRCommonException(
+                f"Timestamp column {self.options.timestamp_col} missing in the dataframe"
+            )
+
+        if self.options.value_col not in custom_metrics_columns:
+            raise DRCommonException(
+                f"Custom Metrics Value column {self.options.value_col} missing in the dataframe"
+            )
+
+    def _report_custom_metrics_async(self):
+        self.event_loop.run_until_complete(self._custom_metrics_dispatcher())
+
+    async def _custom_metrics_dispatcher(self):
+        num_rows, iteration = self.status_tracker.get_status()
+        tasks = list()
+        for input_df_chunk in self.csv_splitter.get_data_chunks():
+            tasks.append(
+                asyncio.create_task(
+                    self._report_custom_metrics_connected_lib(input_df_chunk, num_rows)
+                )
+            )
+            num_rows = self.csv_splitter.get_current_row()
+            if len(tasks) == self.options.num_concurrent_requests:
+                break
+
+        while not self.csv_splitter.is_all_data_reported():
+            done, pending = await asyncio.wait(tasks, return_when=asyncio.FIRST_COMPLETED)
+            for task in done:
+                tasks.remove(task)
+                input_df_chunk = self.csv_splitter.get_next_chunk_to_report()
+                if input_df_chunk is None:
+                    continue
+                num_rows = self.csv_splitter.get_current_row()
+                new_task = asyncio.create_task(
+                    self._report_custom_metrics_connected_lib(input_df_chunk, num_rows)
+                )
+                tasks.append(new_task)
+                logger.debug(
+                    "Added new task to report custom metrics from {} to {}".format(
+                        num_rows, num_rows + self.csv_splitter.get_chunk_size()
+                    )
+                )
+
+        # No more data to report, all tasks submitted, but let's wait for their completion
+        logger.info("Done with submitting all tasks; waiting for them to finish now.")
+        await asyncio.wait(tasks)
+        logger.info("Done reporting all custom metrics.")
+
+    def report_custom_metrics(self):
+        check_required_parameter(self.options.input, None, ArgumentsOptions.INPUT)
+        check_required_parameter(
+            self.options.deployment_id, EV.MLOPS_DEPLOYMENT_ID, ArgumentsOptions.DEPLOYMENT_ID
+        )
+        check_required_parameter(
+            self.options.metric_id, EV.MLOPS_METRIC_ID, ArgumentsOptions.METRIC_ID
+        )
+        check_required_parameter(
+            self.options.model_id, EV.MLOPS_MODEL_ID, ArgumentsOptions.MODEL_ID
+        )
+        check_required_parameter(self.options.timestamp_col, None, ArgumentsOptions.TIMESTAMP_COL)
+        check_required_parameter(self.options.value_col, None, ArgumentsOptions.VALUE_COL)
+
+        logger.debug("Reporting custom metrics:")
+        logger.debug(f"MLOps service:         {self.options.mlops_service_url}")
+        logger.debug(f"Input:                 {self.options.input}")
+        logger.debug(f"Metric ID:             {self.options.metric_id}")
+        logger.debug(f"Timestamp column:      {self.options.timestamp_col}")
+        logger.debug(f"Value column:          {self.options.value_col}")
+        logger.debug(f"Timestamp Format:      {self.options.timestamp_format}")
+        logger.debug(f"Dry run:               {self.options.dry_run}")
+
+        if self.options.status_file:
+            self.status_tracker = MLOpsUploadTracker(self.options.status_file)
+        else:
+            self.status_tracker = MLOpsUploadTracker()
+        skip_rows, _ = self.status_tracker.get_status()
+        try:
+            self.csv_splitter = MLOpsCSVJSONSplitter(self.options.input, skip_rows=skip_rows)
+            self._check_custom_metrics_columns(self.csv_splitter.get_columns())
+        except (pd.errors.EmptyDataError, DRCommonException) as e:
+            self._log_error_and_exit(e, ExitCode.DEFAULT.value)
+
+        try:
+            self.create_mclient()
+            self._report_custom_metrics_async()
+        except DRNotFoundException as e:
+            self._log_error_and_exit(e, ExitCode.DR_NOT_FOUND.value)
+        except DRMLOpsConnectedException as e:
+            self._log_error_and_exit(e, ExitCode.DR_CONNECTED.value)
+        except Exception as e:
+            self._log_error_and_exit(e, ExitCode.UNSPECIFIED.value)
+        finally:
+            self.delete_mclient()
+
+    def handle_custom_metrics(self):
+        if self.options.action == Actions.CREATE:
+            self.create_custom_metric()
+        elif self.options.action == Actions.GET:
+            self.get_custom_metric()
+        elif self.options.action == Actions.LIST:
+            self.list_custom_metrics()
+        elif self.options.action == Actions.REPORT:
+            self.report_custom_metrics()
+        else:
+            self._print_supported_actions(Subjects.CUSTOM_METRICS)
+
     def get_batch_statistics(self):
         check_required_parameter(
             self.options.deployment_id, EV.MLOPS_DEPLOYMENT_ID, ArgumentsOptions.DEPLOYMENT_ID
         )
         check_required_parameter(
             self.options.batch_id, EV.MLOPS_BATCH_ID, ArgumentsOptions.BATCH_ID
         )
@@ -2323,14 +2643,16 @@
             self.handle_deployment()
         elif self.run_mode == RunMode.PREDICTION_ENVIRONMENT:
             self.handle_prediction_environment()
         elif self.run_mode == RunMode.SERVICE_STATS:
             self.handle_service_stats()
         elif self.run_mode == RunMode.BATCH:
             self.handle_batch()
+        elif self.run_mode == RunMode.CUSTOM_METRICS:
+            self.handle_custom_metrics()
         else:
             print("No valid subject provided")
             raise SystemExit(ExitCode.INVALID_CLI_INPUT.value)
 
 
 def check_required_parameter(option, env_name, parameter_name):
     if option is None:
```

## datarobot/mlops/connected/url_helper.py

```diff
@@ -64,14 +64,16 @@
     SCORING_CODE_DOWNLOAD = "scoringCode"
     SERVICE_STATS = "serviceStats"
     PREDICTION_STATS = "predictionsOverTime"
     TARGET_DRIFT = "targetDrift"
     PREDICTIONS_ACTUALS_STATS = "predictionsVsActualsOverTime"
     MONITORING_BATCHES = "monitoringBatches"
     PREDICTIONS_OVER_BATCH = "predictionsOverBatch"
+    CUSTOM_METRICS = "customMetrics"
+    SUMMARY = "summary"
 
 
 class URLBuilder:
     def __init__(self, service_url):
         self._service_url = service_url
 
     def deployment(self, deployment_id, force_delete=False):
@@ -238,14 +240,24 @@
         return build_url(
             self._service_url,
             MMMEndpointPrefix.DEPLOYMENT,
             deployment_id,
             MMMEndpoint.ACTUALS_FROM_JSON,
         )
 
+    def report_custom_metrics(self, deployment_id, metrics_id):
+        return build_url(
+            self._service_url,
+            MMMEndpointPrefix.DEPLOYMENT,
+            deployment_id,
+            MMMEndpoint.CUSTOM_METRICS,
+            metrics_id,
+            MMMEndpoint.FROM_JSON,
+        )
+
     def create_prediction_environment(self):
         return build_url(self._service_url, MMMEndpointPrefix.PREDICTION_ENV, None)
 
     def get_prediction_environment(self, pe_id):
         return build_url(self._service_url, MMMEndpointPrefix.PREDICTION_ENV, pe_id)
 
     def list_prediction_environments(self):
@@ -301,7 +313,33 @@
         return build_url(
             self._service_url,
             MMMEndpointPrefix.DEPLOYMENT,
             deployment_id,
             MMMEndpoint.PREDICTIONS_OVER_BATCH,
             batchId=batch_id,
         )
+
+    def create_custom_metric(self, deployment_id):
+        return build_url(
+            self._service_url,
+            MMMEndpointPrefix.DEPLOYMENT,
+            deployment_id,
+            MMMEndpoint.CUSTOM_METRICS,
+        )
+
+    def get_custom_metric_summary(self, deployment_id, metric_id):
+        return build_url(
+            self._service_url,
+            MMMEndpointPrefix.DEPLOYMENT,
+            deployment_id,
+            MMMEndpoint.CUSTOM_METRICS,
+            metric_id,
+            MMMEndpoint.SUMMARY,
+        )
+
+    def list_custom_metrics(self, deployment_id):
+        return build_url(
+            self._service_url,
+            MMMEndpointPrefix.DEPLOYMENT,
+            deployment_id,
+            MMMEndpoint.CUSTOM_METRICS,
+        )
```

## Comparing `datarobot_mlops_connected_client-9.1.1b1.dist-info/METADATA` & `datarobot_mlops_connected_client-9.1.1rc1.dist-info/METADATA`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datarobot-mlops-connected-client
-Version: 9.1.1b1
+Version: 9.1.1rc1
 Summary: datarobot-mlops-connected-client client to communicate with DataRobot MLOps service
 Home-page: http://datarobot.com
 Author: DataRobot
 Author-email: support@datarobot.com
 Maintainer: DataRobot
 Maintainer-email: info@datarobot.com
 License: DataRobot Tool and Utility Agreement
```

## Comparing `datarobot_mlops_connected_client-9.1.1b1.dist-info/RECORD` & `datarobot_mlops_connected_client-9.1.1rc1.dist-info/RECORD`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 datarobot/mlops/__init__.py,sha256=AKjMKTNwSwhUBVbzAe95rrPT428dkII5aszufDWlEYw,597
 datarobot/mlops/connected/__init__.py,sha256=gtaquSkCXoIY93Uy5hmlx-TbK6pSnDoGPwV-KeoM-DU,532
-datarobot/mlops/connected/client.py,sha256=iviglWayMRAxzDRpcoHrHmmYlSjzbdJRWaFc62-1GJc,94846
+datarobot/mlops/connected/client.py,sha256=TVxqXOa4Yl4yMfU_n76gsuBfH6TpWOos0aSWP9OsqSU,106180
 datarobot/mlops/connected/enums.py,sha256=ygJSPeoZjdYGWMBGJ3X18RumXqCEsnEdGQB6yqpI77g,1231
 datarobot/mlops/connected/exception.py,sha256=2Y-nd3Lbo6abhvyS3nTUPwnS8sGTdk29-kl3gsuUihA,900
-datarobot/mlops/connected/mlops_cli.py,sha256=6movxevCTCpDct9bHBUzDb_8_iRUq_G3lS7ze8T-YF4,96728
+datarobot/mlops/connected/mlops_cli.py,sha256=vqSeMdyFpKfBPvukaC7fiErqDVw8zKiJwRDgNzYHYK4,110928
 datarobot/mlops/connected/upload_tracker.py,sha256=sgMVqBgI7xvXtpLYINqnxaw4AljraDVg5Gg3An8pq3A,2646
-datarobot/mlops/connected/url_helper.py,sha256=AJQKndXVQA5L-yluwXG1-vWKH1ASSo7DzGKjcNGXwh4,10251
-datarobot_mlops_connected_client-9.1.1b1.dist-info/METADATA,sha256=PdplKvXR2gM4C3P_wkw1qZz3tGN4Z-dMTAb1ciao38E,1536
-datarobot_mlops_connected_client-9.1.1b1.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-datarobot_mlops_connected_client-9.1.1b1.dist-info/entry_points.txt,sha256=pjOHN_gQuYzuqbf0AL5S5lcGhDfIlOGElQU2Qduh2mg,72
-datarobot_mlops_connected_client-9.1.1b1.dist-info/top_level.txt,sha256=RTK5ZHErXe7mZUlXWQRjQpqFdWw3qmpF95Lz7ViL2Lc,10
-datarobot_mlops_connected_client-9.1.1b1.dist-info/RECORD,,
+datarobot/mlops/connected/url_helper.py,sha256=hlQP_JC4ACMKqXaN_R6a91M3vUq97aAsVuTRCIZ3vMs,11367
+datarobot_mlops_connected_client-9.1.1rc1.dist-info/METADATA,sha256=FsimiGR4Inq0O84Sr42Jq2tBVnWap-jNG0VehOwSRoo,1537
+datarobot_mlops_connected_client-9.1.1rc1.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+datarobot_mlops_connected_client-9.1.1rc1.dist-info/entry_points.txt,sha256=pjOHN_gQuYzuqbf0AL5S5lcGhDfIlOGElQU2Qduh2mg,72
+datarobot_mlops_connected_client-9.1.1rc1.dist-info/top_level.txt,sha256=RTK5ZHErXe7mZUlXWQRjQpqFdWw3qmpF95Lz7ViL2Lc,10
+datarobot_mlops_connected_client-9.1.1rc1.dist-info/RECORD,,
```

