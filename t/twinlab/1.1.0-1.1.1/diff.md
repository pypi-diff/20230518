# Comparing `tmp/twinlab-1.1.0.tar.gz` & `tmp/twinlab-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "twinlab-1.1.0.tar", max compression
+gzip compressed data, was "twinlab-1.1.1.tar", max compression
```

## Comparing `twinlab-1.1.0.tar` & `twinlab-1.1.1.tar`

### file list

```diff
@@ -1,8 +1,9 @@
--rw-r--r--   0        0        0     1048 2023-04-11 12:00:19.210453 twinlab-1.1.0/README.md
--rw-r--r--   0        0        0      599 2023-05-11 09:39:31.646748 twinlab-1.1.0/pyproject.toml
--rw-r--r--   0        0        0      528 2023-05-11 09:23:20.908327 twinlab-1.1.0/twinlab/__init__.py
--rw-r--r--   0        0        0     6650 2023-05-11 09:39:06.665209 twinlab-1.1.0/twinlab/client.py
--rw-r--r--   0        0        0      505 2023-05-11 09:23:10.154006 twinlab-1.1.0/twinlab/plotting.py
--rw-r--r--   0        0        0      552 2023-05-10 15:28:55.405307 twinlab-1.1.0/twinlab/settings.py
--rw-r--r--   0        0        0     3997 2023-05-11 09:39:06.665507 twinlab-1.1.0/twinlab/utils.py
--rw-r--r--   0        0        0     1726 1970-01-01 00:00:00.000000 twinlab-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1031 2023-05-18 13:40:02.600816 twinlab-1.1.1/LICENSE
+-rw-r--r--   0        0        0     2115 2023-05-18 13:49:12.053818 twinlab-1.1.1/README.md
+-rw-r--r--   0        0        0      932 2023-05-18 13:40:02.603772 twinlab-1.1.1/pyproject.toml
+-rw-r--r--   0        0        0      529 2023-05-18 13:40:02.609012 twinlab-1.1.1/twinlab/__init__.py
+-rw-r--r--   0        0        0     7858 2023-05-18 13:40:02.609191 twinlab-1.1.1/twinlab/client.py
+-rw-r--r--   0        0        0      505 2023-05-11 09:23:10.154006 twinlab-1.1.1/twinlab/plotting.py
+-rw-r--r--   0        0        0      664 2023-05-18 13:40:02.609342 twinlab-1.1.1/twinlab/settings.py
+-rw-r--r--   0        0        0     5762 2023-05-18 15:23:53.182090 twinlab-1.1.1/twinlab/utils.py
+-rw-r--r--   0        0        0     3066 1970-01-01 00:00:00.000000 twinlab-1.1.1/PKG-INFO
```

### Comparing `twinlab-1.1.0/pyproject.toml` & `twinlab-1.1.1/pyproject.toml`

 * *Files 27% similar despite different names*

```diff
@@ -1,13 +1,22 @@
 [tool.poetry]
 name = "twinlab"
-version = "1.1.0"
-description = "Client interface for twinLab"
-authors = ["Alexander Mead <alexander@digilab.co.uk>", "Freddy Wordingham <freddy@digilab.co.uk>"]
+version = "1.1.1"
+description = "Client interface for twinLab machine-learning in the cloud."
+license = "MIT"
+homepage = "https://www.digilab.co.uk/"
 repository = "https://github.com/digiLab-ai/twinLab-client"
+documentation = "https://digilab-ai.github.io/twinLab-client"
+authors = ["DigiLab Solutions Ltd. <info@digilab.co.uk>"]
+maintainers = [
+    "Alexander Mead <alexander@digilab.co.uk>",
+    "Freddy Wordingham <freddy@digilab.co.uk>",
+    "Jordan Hart <jordan@digilab.co.uk>",
+]
+keywords = ["machine-learning", "AI", "cloud", "twinLab", "digiLab"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.9,<3.12"
 pandas = "^1.5.3"
 pydantic = { version = "^1.10.7", extras = ["dotenv"] }
 requests = "^2.28.2"
```

### Comparing `twinlab-1.1.0/twinlab/__init__.py` & `twinlab-1.1.1/twinlab/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,14 +6,14 @@
 from .client import query_dataset
 from .client import list_datasets
 from .client import delete_dataset
 
 # API campaign functions
 from .client import train_campaign
 from .client import query_campaign
-from .client import sample_campaign
+from .client import predict_campaign
 from .client import list_campaigns
 from .client import delete_campaign
 
 # Plotting functions
 from .plotting import get_blur_boundaries
 from .plotting import get_blur_alpha
```

### Comparing `twinlab-1.1.0/twinlab/client.py` & `twinlab-1.1.1/twinlab/utils.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,200 +1,198 @@
 # Standard imports
+import io
+import argparse
+import json
 from pprint import pprint
 
 # Third-party imports
 import requests
 import pandas as pd
 
 # Project imports
-from . import utils
+from .settings import ENV
 
-### Dataset functions ###
+
+PARAMS_COERCION = {  # Convert these names in the params file
+    "test_train_split": "train_test_split",  # Common mistake
+    # "num_train_examples": "train_test_split", # TODO: Think of something better
+}
+TRAIN_CAMPAIGN_CLOUD_URL = "https://cma567qwquixu7bbjcnhbjsxjm0yumvu.lambda-url.eu-west-2.on.aws/"
+TRAIN_CAMPAIGN_STAGE_URL = "https://b7vgjlsn73e7n7kci5rwoxjc7e0pkcqn.lambda-url.eu-west-2.on.aws/"
+
+### Utility functions ###
+
+
+# def unwrap_payload(event: dict) -> dict:
+#     """
+#     Return payload and decode if it is base64 encoded
+#     TODO: Not used yet...
+#     """
+#     if "body" not in event:  # Get body
+#         raise Exception("No body in request")
+#     body = event["body"]
+#     if "isBase64Encoded" in event:  # Decode
+#         if event["isBase64Encoded"]:
+#             body = base64.b64decode(body)
+#     try:  # Parse
+#         payload = json.loads(body)
+#     except:
+#         raise Exception("Could not parse body as JSON")
+#     return payload
+
+
+def get_command_line_args() -> argparse.Namespace:
+    """
+    Parse command-line arguments
+    """
+    parser = argparse.ArgumentParser()
+    parser.add_argument(
+        "server",
+        default=False,
+        help="specify whether to use local or cloud lambda function",
+    )
+    args = parser.parse_args()
+    return args
+
+
+def construct_standard_headers(debug=False) -> dict:
+    headers = {
+        "X-Group": ENV.TWINLAB_GROUPNAME,
+        "X-User": ENV.TWINLAB_USERNAME,
+        "authorizationToken": ENV.TWINLAB_TOKEN,
+        "X-Debug": str(debug).lower(),
+    }
+    return headers
+
+
+def get_server_url(server: str) -> str:
+    """
+    The URL is the dockerised lambda function that's been set up in cloud by alexander
+    """
+    if server == "local":
+        baseURL = ENV.TWINLAB_LOCAL_SERVER
+    elif server == "cloud":
+        baseURL = ENV.TWINLAB_SERVER
+    elif server == "stage":
+        baseURL = ENV.TWINLAB_STAGE_SERVER
+    else:
+        print("Server:", server)
+        raise ValueError("Server must be either 'local', 'cloud', or 'stage'")
+    return baseURL
 
 
-def upload_dataset(dataset_filepath: str, server="cloud", verbose=False) -> None:
+def get_train_campaign_url(server: str) -> str:
     """
-    Upload a dataset to the cloud so that it can be queried and used for training
-    params:
-        dataset_filepath: str; location of csv dataset on local machine
-        server: str; either "cloud" or "local"
-        verbose: bool
+    Get the URL for the train_campaign lambda function
+    These are different to avoid the AWS Lambda 29s gateway timeout
     """
-    # TODO: Allow for uploading pandas dataframes
-    headers = utils.STANDARD_HEADERS.copy()  #  TODO: Is .copy() necessary here?
-    headers["X-Dataset"] = dataset_filepath
-    lambda_url = utils.get_server_url(server) + "/generate_upload_url"
-    r = requests.get(lambda_url, headers=headers)
-    utils.check_response(r)
-    if verbose:
-        utils.print_response_message(r)
-    upload_url = r.json()["url"]
-    if verbose:
-        print(f"Uploading {dataset_filepath}")
-    utils.upload_file_to_presigned_url(
-        dataset_filepath, upload_url, verbose=verbose)
-    process_url = utils.get_server_url(server) + "/process_uploaded_dataset"
-    r = requests.post(process_url, headers=headers)
-    if verbose:
-        utils.print_response_message(r)
+    if server == "cloud":
+        url = TRAIN_CAMPAIGN_CLOUD_URL
+    elif server == "stage":
+        url = TRAIN_CAMPAIGN_STAGE_URL
+    else:
+        url = get_server_url(server) + "/train_campaign"
+    return url
 
 
-def query_dataset(dataset_name: str, server="cloud", verbose=False) -> pd.DataFrame:
+def coerce_params_dict(params: dict) -> dict:
     """
-    Query a dataset that exists on the cloud by printing summary statistics
-    params:
-        dataset_name: str; name of dataset on S3 (same as the uploaded file name)
-        server: str; either "cloud" or "local"
-        verbose: bool
+    Relabel parameters to be consistent with twinLab library
     """
-    url = utils.get_server_url(server) + "/query_dataset"
-    headers = utils.STANDARD_HEADERS.copy()
-    headers["X-Dataset"] = dataset_name
-    r = requests.get(url, headers=headers)
-    utils.check_response(r)
-    df = utils.extract_csv_from_response(r, "summary")
-    if verbose:
-        utils.print_response_message(r)
-        print("Summary:\n", df, "\n")
-    return df
+    for param in PARAMS_COERCION:
+        if param in params:
+            params[PARAMS_COERCION[param]] = params.pop(param)
+    return params
 
 
-def list_datasets(server="cloud", verbose=False) -> list:
-    """
-    List datasets that have been uploaded to the cloud
-    params:
-        server: str; either "cloud" or "local"
-        verbose: bool
-    """
-    url = utils.get_server_url(server) + "/list_datasets"
-    headers = utils.STANDARD_HEADERS.copy()
-    r = requests.get(url, headers=headers)
-    utils.check_response(r)
-    if verbose:
-        utils.print_response_message(r)
-    response = r.json()
-    return response["datasets"]
+### ###
+
+### HTTP requests ###
 
 
-def delete_dataset(dataset_name: str, server="cloud", verbose=False) -> None:
+def upload_file_to_presigned_url(file_path: str, url: str, verbose=False) -> None:
     """
-    Delete a dataset from the cloud
+    Upload a file to the specified pre-signed URL.
     params:
-        dataset_name: str; name of dataset on S3 (same as the uploaded file name)
-        server: str; either "cloud" or "local"
+        file_path: str; the path to the local file you want to upload.
+        presigned_url: The pre-signed URL generated for uploading the file.
         verbose: bool
     """
-    url = utils.get_server_url(server) + "/delete_dataset"
-    headers = utils.STANDARD_HEADERS.copy()
-    headers["X-Dataset"] = dataset_name
-    r = requests.post(url, headers=headers)
-    utils.check_response(r)
-    if verbose:
-        utils.print_response_message(r)
-
-###  ###
 
-### Campaign functions ###
+    with open(file_path, "rb") as file:
+        headers = {"Content-Type": "application/octet-stream"}
+        response = requests.put(url, data=file, headers=headers)
+    if verbose:
+        if response.status_code == 200:
+            print(f"File {file_path} uploaded successfully.")
+        else:
+            print(f"File upload failed")
+            print(f"Status code: {response.status_code}")
+            print(f"Reason: {response.text}")
+        print()
 
 
-def train_campaign(params: dict, campaign: str, server="cloud", verbose=False) -> None:
+def upload_dataframe_to_presigned_url(dataset_name: str, df: pd.DataFrame, url: str, verbose=False) -> None:
     """
-    Train a campaign remotely using twinLab
+    Upload a panads dataframe to the specified pre-signed URL.
     params:
-        params: dict; parameters for training
-        campaign: str; name of this campaign and final trained model (user choice)
-        server: str; either "cloud" or "local"
-        verbose: bool
+        df: The pandas dataframe to upload
+        presigned_url: The pre-signed URL generated for uploading the file.
     """
-    if server == "cloud":
-        url = utils.TRAIN_CAMPAIGN_CLOUD_URL
-    else:
-        url = utils.get_server_url(server) + "/train_campaign"
-    headers = utils.STANDARD_HEADERS.copy()
-    headers["X-Campaign"] = campaign
-    r = requests.post(url, json=params, headers=headers)
-    utils.check_response(r)
+    headers = {"Content-Type": "application/octet-stream"}
+    buffer = io.BytesIO()
+    df.to_csv(buffer, index=False)
+    buffer = buffer.getvalue()
+    response = requests.put(url, data=buffer, headers=headers)
     if verbose:
-        utils.print_response_message(r)
+        if response.status_code == 200:
+            print(f"Dataframe uploaded successfully.")
+        else:
+            print(f"File upload failed")
+            print(f"Status code: {response.status_code}")
+            print(f"Reason: {response.text}")
+        print()
 
 
-def query_campaign(campaign_name: str, server="cloud", verbose=False) -> dict:
+def extract_csv_from_response(response: requests.Response, name: str) -> pd.DataFrame:
     """
-    Print summary statistics for a pre-trained campaign
-    params:
-        campaign_name: str; name of trained model to query
-        server: str; either "cloud" or "local"
-        verbose: bool
+    Extract CSV from response
     """
-    url = utils.get_server_url(server) + "/query_campaign"
-    headers = utils.STANDARD_HEADERS.copy()
-    headers["X-Campaign"] = campaign_name
-    r = requests.get(url, headers=headers)
-    utils.check_response(r)
-    metadata = utils.extract_item_from_response(r, "metadata")
-    if verbose:
-        utils.print_response_message(r)
-        print("Metadata:")
-        pprint(metadata, compact=True, sort_dicts=False)
-    return metadata
+    body = response.json()  # Get the body of the response as a dictionary
+    data = body[name]  # Get the entry corresponding to the field name
+    df = pd.read_json(data, orient="split")
+    return df
 
 
-def list_campaigns(server="cloud", verbose=False) -> list:
+def extract_item_from_response(response: requests.Response, name: str) -> any:
     """
-    List all trained campaigns stored in cloud
-    params:
-        server: str; either "cloud" or "local"
-        verbose: bool
+    Extract CSV from response
     """
-    url = utils.get_server_url(server) + "/list_campaigns"
-    headers = utils.STANDARD_HEADERS.copy()
-    r = requests.get(url, headers=headers)
-    utils.check_response(r)
-    if verbose:
-        utils.print_response_message(r)
-    response = r.json()
-    return response["campaigns"]
+    body = response.json()  # Get the body of the response as a dictionary
+    item = body[name]  # Get the entry corresponding to the field name
+    return item
 
 
-def sample_campaign(
-    filepath: str, campaign: str, server="cloud", verbose=False
-) -> tuple:
+def print_response_headers(r: requests.Response) -> None:
     """
-    Sample a pre-trained campaign that exists on the cloud
-    params:
-        filepath: str; location of csv dataset on local machine for evaluation
-        campaign: str; name of pre-trained model to do the evaluating
-        server: str; either "cloud" or "local"
-        verbose: bool
+    Print response headers
     """
-    # TODO: Rename to evaluate_campaign?
-    # TODO: Allow for uploading pandas dataframes
-    url = utils.get_server_url(server) + "/sample_campaign"
-    files = {"file": (filepath, open(filepath, "rb"), "text/csv")}
-    headers = utils.STANDARD_HEADERS.copy()
-    headers["X-Campaign"] = campaign
-    r = requests.post(url, files=files, headers=headers)
-    utils.check_response(r)
-    df_mean = utils.extract_csv_from_response(r, "y_mean")
-    df_std = utils.extract_csv_from_response(r, "y_std")
-    if verbose:
-        utils.print_response_message(r)
-        print("Mean: \n", df_mean, "\n")
-        print("Std: \n", df_std, "\n")
-    return df_mean, df_std
+    print("Response headers:")
+    pprint(dict(r.headers))
+    print()
 
 
-def delete_campaign(campaign_name: str, server="cloud", verbose=False) -> None:
+def print_response_message(r: requests.Response) -> None:
     """
-    Delete campaign directory from S3
-    params:
-        campaign_name: str; name of trained model to delete
-        server: str; either "cloud" or "local"
-        verbose: bool
+    Print response message
     """
-    url = utils.get_server_url(server) + "/delete_campaign"
-    headers = utils.STANDARD_HEADERS.copy()
-    headers["X-Campaign"] = campaign_name
-    r = requests.post(url, headers=headers)
-    utils.check_response(r)
-    if verbose:
-        utils.print_response_message(r)
+    print("Response:", json.loads(r.text)["message"])
+    print()
+
+
+def check_response(r: requests.Response) -> None:
+    if r.status_code != 200:
+        print("Status code:", r.status_code)
+        print_response_message(r)
+        raise RuntimeError("Response error")
+
+### ###
```

