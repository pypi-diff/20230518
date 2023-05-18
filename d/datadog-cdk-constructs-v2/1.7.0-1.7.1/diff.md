# Comparing `tmp/datadog-cdk-constructs-v2-1.7.0.tar.gz` & `tmp/datadog-cdk-constructs-v2-1.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datadog-cdk-constructs-v2-1.7.0.tar", last modified: Wed May 17 21:24:43 2023, max compression
+gzip compressed data, was "datadog-cdk-constructs-v2-1.7.1.tar", last modified: Thu May 18 16:00:03 2023, max compression
```

## Comparing `datadog-cdk-constructs-v2-1.7.0.tar` & `datadog-cdk-constructs-v2-1.7.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 david.lee   (503) staff       (20)        0 2023-05-17 21:24:43.121111 datadog-cdk-constructs-v2-1.7.0/
--rw-r--r--   0 david.lee   (503) staff       (20)    11358 2023-05-17 21:24:39.000000 datadog-cdk-constructs-v2-1.7.0/LICENSE
--rw-r--r--   0 david.lee   (503) staff       (20)       23 2023-05-17 21:24:39.000000 datadog-cdk-constructs-v2-1.7.0/MANIFEST.in
--rw-r--r--   0 david.lee   (503) staff       (20)    22507 2023-05-17 21:24:43.120968 datadog-cdk-constructs-v2-1.7.0/PKG-INFO
--rw-r--r--   0 david.lee   (503) staff       (20)    21527 2023-05-17 21:24:39.000000 datadog-cdk-constructs-v2-1.7.0/README.md
--rw-r--r--   0 david.lee   (503) staff       (20)      236 2023-05-17 21:24:39.000000 datadog-cdk-constructs-v2-1.7.0/pyproject.toml
--rw-r--r--   0 david.lee   (503) staff       (20)       38 2023-05-17 21:24:43.121165 datadog-cdk-constructs-v2-1.7.0/setup.cfg
--rw-r--r--   0 david.lee   (503) staff       (20)     1921 2023-05-17 21:24:39.000000 datadog-cdk-constructs-v2-1.7.0/setup.py
-drwxr-xr-x   0 david.lee   (503) staff       (20)        0 2023-05-17 21:24:43.118023 datadog-cdk-constructs-v2-1.7.0/src/
-drwxr-xr-x   0 david.lee   (503) staff       (20)        0 2023-05-17 21:24:43.119396 datadog-cdk-constructs-v2-1.7.0/src/datadog_cdk_constructs_v2/
--rw-r--r--   0 david.lee   (503) staff       (20)    62499 2023-05-17 21:24:39.000000 datadog-cdk-constructs-v2-1.7.0/src/datadog_cdk_constructs_v2/__init__.py
-drwxr-xr-x   0 david.lee   (503) staff       (20)        0 2023-05-17 21:24:43.120641 datadog-cdk-constructs-v2-1.7.0/src/datadog_cdk_constructs_v2/_jsii/
--rw-r--r--   0 david.lee   (503) staff       (20)      475 2023-05-17 21:24:39.000000 datadog-cdk-constructs-v2-1.7.0/src/datadog_cdk_constructs_v2/_jsii/__init__.py
--rw-r--r--   0 david.lee   (503) staff       (20)   133242 2023-05-17 21:24:39.000000 datadog-cdk-constructs-v2-1.7.0/src/datadog_cdk_constructs_v2/_jsii/datadog-cdk-constructs-v2@1.7.0.jsii.tgz
--rw-r--r--   0 david.lee   (503) staff       (20)        1 2023-05-17 21:24:39.000000 datadog-cdk-constructs-v2-1.7.0/src/datadog_cdk_constructs_v2/py.typed
-drwxr-xr-x   0 david.lee   (503) staff       (20)        0 2023-05-17 21:24:43.120276 datadog-cdk-constructs-v2-1.7.0/src/datadog_cdk_constructs_v2.egg-info/
--rw-r--r--   0 david.lee   (503) staff       (20)    22507 2023-05-17 21:24:42.000000 datadog-cdk-constructs-v2-1.7.0/src/datadog_cdk_constructs_v2.egg-info/PKG-INFO
--rw-r--r--   0 david.lee   (503) staff       (20)      523 2023-05-17 21:24:43.000000 datadog-cdk-constructs-v2-1.7.0/src/datadog_cdk_constructs_v2.egg-info/SOURCES.txt
--rw-r--r--   0 david.lee   (503) staff       (20)        1 2023-05-17 21:24:42.000000 datadog-cdk-constructs-v2-1.7.0/src/datadog_cdk_constructs_v2.egg-info/dependency_links.txt
--rw-r--r--   0 david.lee   (503) staff       (20)      161 2023-05-17 21:24:43.000000 datadog-cdk-constructs-v2-1.7.0/src/datadog_cdk_constructs_v2.egg-info/requires.txt
--rw-r--r--   0 david.lee   (503) staff       (20)       26 2023-05-17 21:24:43.000000 datadog-cdk-constructs-v2-1.7.0/src/datadog_cdk_constructs_v2.egg-info/top_level.txt
+drwxr-xr-x   0 david.lee   (503) staff       (20)        0 2023-05-18 16:00:03.341519 datadog-cdk-constructs-v2-1.7.1/
+-rw-r--r--   0 david.lee   (503) staff       (20)    11358 2023-05-18 15:59:59.000000 datadog-cdk-constructs-v2-1.7.1/LICENSE
+-rw-r--r--   0 david.lee   (503) staff       (20)       23 2023-05-18 15:59:59.000000 datadog-cdk-constructs-v2-1.7.1/MANIFEST.in
+-rw-r--r--   0 david.lee   (503) staff       (20)    22507 2023-05-18 16:00:03.341375 datadog-cdk-constructs-v2-1.7.1/PKG-INFO
+-rw-r--r--   0 david.lee   (503) staff       (20)    21527 2023-05-18 15:59:59.000000 datadog-cdk-constructs-v2-1.7.1/README.md
+-rw-r--r--   0 david.lee   (503) staff       (20)      236 2023-05-18 15:59:59.000000 datadog-cdk-constructs-v2-1.7.1/pyproject.toml
+-rw-r--r--   0 david.lee   (503) staff       (20)       38 2023-05-18 16:00:03.341569 datadog-cdk-constructs-v2-1.7.1/setup.cfg
+-rw-r--r--   0 david.lee   (503) staff       (20)     1921 2023-05-18 15:59:59.000000 datadog-cdk-constructs-v2-1.7.1/setup.py
+drwxr-xr-x   0 david.lee   (503) staff       (20)        0 2023-05-18 16:00:03.338432 datadog-cdk-constructs-v2-1.7.1/src/
+drwxr-xr-x   0 david.lee   (503) staff       (20)        0 2023-05-18 16:00:03.339799 datadog-cdk-constructs-v2-1.7.1/src/datadog_cdk_constructs_v2/
+-rw-r--r--   0 david.lee   (503) staff       (20)    98974 2023-05-18 15:59:59.000000 datadog-cdk-constructs-v2-1.7.1/src/datadog_cdk_constructs_v2/__init__.py
+drwxr-xr-x   0 david.lee   (503) staff       (20)        0 2023-05-18 16:00:03.341040 datadog-cdk-constructs-v2-1.7.1/src/datadog_cdk_constructs_v2/_jsii/
+-rw-r--r--   0 david.lee   (503) staff       (20)      475 2023-05-18 15:59:59.000000 datadog-cdk-constructs-v2-1.7.1/src/datadog_cdk_constructs_v2/_jsii/__init__.py
+-rw-r--r--   0 david.lee   (503) staff       (20)   134685 2023-05-18 15:59:59.000000 datadog-cdk-constructs-v2-1.7.1/src/datadog_cdk_constructs_v2/_jsii/datadog-cdk-constructs-v2@1.7.1.jsii.tgz
+-rw-r--r--   0 david.lee   (503) staff       (20)        1 2023-05-18 15:59:59.000000 datadog-cdk-constructs-v2-1.7.1/src/datadog_cdk_constructs_v2/py.typed
+drwxr-xr-x   0 david.lee   (503) staff       (20)        0 2023-05-18 16:00:03.340684 datadog-cdk-constructs-v2-1.7.1/src/datadog_cdk_constructs_v2.egg-info/
+-rw-r--r--   0 david.lee   (503) staff       (20)    22507 2023-05-18 16:00:03.000000 datadog-cdk-constructs-v2-1.7.1/src/datadog_cdk_constructs_v2.egg-info/PKG-INFO
+-rw-r--r--   0 david.lee   (503) staff       (20)      523 2023-05-18 16:00:03.000000 datadog-cdk-constructs-v2-1.7.1/src/datadog_cdk_constructs_v2.egg-info/SOURCES.txt
+-rw-r--r--   0 david.lee   (503) staff       (20)        1 2023-05-18 16:00:03.000000 datadog-cdk-constructs-v2-1.7.1/src/datadog_cdk_constructs_v2.egg-info/dependency_links.txt
+-rw-r--r--   0 david.lee   (503) staff       (20)      161 2023-05-18 16:00:03.000000 datadog-cdk-constructs-v2-1.7.1/src/datadog_cdk_constructs_v2.egg-info/requires.txt
+-rw-r--r--   0 david.lee   (503) staff       (20)       26 2023-05-18 16:00:03.000000 datadog-cdk-constructs-v2-1.7.1/src/datadog_cdk_constructs_v2.egg-info/top_level.txt
```

### Comparing `datadog-cdk-constructs-v2-1.7.0/LICENSE` & `datadog-cdk-constructs-v2-1.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `datadog-cdk-constructs-v2-1.7.0/PKG-INFO` & `datadog-cdk-constructs-v2-1.7.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datadog-cdk-constructs-v2
-Version: 1.7.0
+Version: 1.7.1
 Summary: CDK Construct Library to automatically instrument Python and Node Lambda functions with Datadog using AWS CDK v2
 Home-page: https://github.com/DataDog/datadog-cdk-constructs
 Author: Datadog
 License: Apache-2.0
 Project-URL: Source, https://github.com/DataDog/datadog-cdk-constructs
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

### Comparing `datadog-cdk-constructs-v2-1.7.0/README.md` & `datadog-cdk-constructs-v2-1.7.1/README.md`

 * *Files identical despite different names*

### Comparing `datadog-cdk-constructs-v2-1.7.0/setup.py` & `datadog-cdk-constructs-v2-1.7.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "datadog-cdk-constructs-v2",
-    "version": "1.7.0",
+    "version": "1.7.1",
     "description": "CDK Construct Library to automatically instrument Python and Node Lambda functions with Datadog using AWS CDK v2",
     "license": "Apache-2.0",
     "url": "https://github.com/DataDog/datadog-cdk-constructs",
     "long_description_content_type": "text/markdown",
     "author": "Datadog",
     "bdist_wheel": {
         "universal": true
@@ -22,15 +22,15 @@
     },
     "packages": [
         "datadog_cdk_constructs_v2",
         "datadog_cdk_constructs_v2._jsii"
     ],
     "package_data": {
         "datadog_cdk_constructs_v2._jsii": [
-            "datadog-cdk-constructs-v2@1.7.0.jsii.tgz"
+            "datadog-cdk-constructs-v2@1.7.1.jsii.tgz"
         ],
         "datadog_cdk_constructs_v2": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
```

### Comparing `datadog-cdk-constructs-v2-1.7.0/src/datadog_cdk_constructs_v2/__init__.py` & `datadog-cdk-constructs-v2-1.7.1/src/datadog_cdk_constructs_v2/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -364,14 +364,608 @@
 import publication
 import typing_extensions
 
 from typeguard import check_type
 
 from ._jsii import *
 
+import aws_cdk.aws_lambda as _aws_cdk_aws_lambda_ceddda9d
+import aws_cdk.aws_lambda_nodejs as _aws_cdk_aws_lambda_nodejs_ceddda9d
+import aws_cdk.aws_lambda_python_alpha as _aws_cdk_aws_lambda_python_alpha_49328424
+import aws_cdk.aws_logs as _aws_cdk_aws_logs_ceddda9d
+import aws_cdk.aws_secretsmanager as _aws_cdk_aws_secretsmanager_ceddda9d
+import constructs as _constructs_77d1e7e8
+
+
+class Datadog(
+    _constructs_77d1e7e8.Construct,
+    metaclass=jsii.JSIIMeta,
+    jsii_type="datadog-cdk-constructs-v2.Datadog",
+):
+    def __init__(
+        self,
+        scope: _constructs_77d1e7e8.Construct,
+        id: builtins.str,
+        *,
+        add_layers: typing.Optional[builtins.bool] = None,
+        api_key: typing.Optional[builtins.str] = None,
+        api_key_secret: typing.Optional[_aws_cdk_aws_secretsmanager_ceddda9d.ISecret] = None,
+        api_key_secret_arn: typing.Optional[builtins.str] = None,
+        api_kms_key: typing.Optional[builtins.str] = None,
+        apm_flush_deadline: typing.Optional[typing.Union[builtins.str, jsii.Number]] = None,
+        capture_lambda_payload: typing.Optional[builtins.bool] = None,
+        cold_start_trace_skip_libs: typing.Optional[builtins.str] = None,
+        create_forwarder_permissions: typing.Optional[builtins.bool] = None,
+        decode_authorizer_context: typing.Optional[builtins.bool] = None,
+        enable_cold_start_tracing: typing.Optional[builtins.bool] = None,
+        enable_datadog_logs: typing.Optional[builtins.bool] = None,
+        enable_datadog_tracing: typing.Optional[builtins.bool] = None,
+        enable_merge_xray_traces: typing.Optional[builtins.bool] = None,
+        enable_profiling: typing.Optional[builtins.bool] = None,
+        encode_authorizer_context: typing.Optional[builtins.bool] = None,
+        env: typing.Optional[builtins.str] = None,
+        extension_layer_version: typing.Optional[jsii.Number] = None,
+        flush_metrics_to_logs: typing.Optional[builtins.bool] = None,
+        forwarder_arn: typing.Optional[builtins.str] = None,
+        inject_log_context: typing.Optional[builtins.bool] = None,
+        java_layer_version: typing.Optional[jsii.Number] = None,
+        log_level: typing.Optional[builtins.str] = None,
+        min_cold_start_trace_duration: typing.Optional[jsii.Number] = None,
+        node_layer_version: typing.Optional[jsii.Number] = None,
+        python_layer_version: typing.Optional[jsii.Number] = None,
+        redirect_handler: typing.Optional[builtins.bool] = None,
+        service: typing.Optional[builtins.str] = None,
+        site: typing.Optional[builtins.str] = None,
+        source_code_integration: typing.Optional[builtins.bool] = None,
+        tags: typing.Optional[builtins.str] = None,
+        version: typing.Optional[builtins.str] = None,
+    ) -> None:
+        '''
+        :param scope: -
+        :param id: -
+        :param add_layers: 
+        :param api_key: 
+        :param api_key_secret: 
+        :param api_key_secret_arn: 
+        :param api_kms_key: 
+        :param apm_flush_deadline: 
+        :param capture_lambda_payload: 
+        :param cold_start_trace_skip_libs: 
+        :param create_forwarder_permissions: 
+        :param decode_authorizer_context: 
+        :param enable_cold_start_tracing: 
+        :param enable_datadog_logs: 
+        :param enable_datadog_tracing: 
+        :param enable_merge_xray_traces: 
+        :param enable_profiling: 
+        :param encode_authorizer_context: 
+        :param env: 
+        :param extension_layer_version: 
+        :param flush_metrics_to_logs: 
+        :param forwarder_arn: 
+        :param inject_log_context: 
+        :param java_layer_version: 
+        :param log_level: 
+        :param min_cold_start_trace_duration: 
+        :param node_layer_version: 
+        :param python_layer_version: 
+        :param redirect_handler: 
+        :param service: 
+        :param site: 
+        :param source_code_integration: 
+        :param tags: 
+        :param version: 
+        '''
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__74e095ab68a1ec6a36ad77e9741c22f8922ea76270d93f498ffa8f7846214a75)
+            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
+            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
+        props = DatadogPropsV2(
+            add_layers=add_layers,
+            api_key=api_key,
+            api_key_secret=api_key_secret,
+            api_key_secret_arn=api_key_secret_arn,
+            api_kms_key=api_kms_key,
+            apm_flush_deadline=apm_flush_deadline,
+            capture_lambda_payload=capture_lambda_payload,
+            cold_start_trace_skip_libs=cold_start_trace_skip_libs,
+            create_forwarder_permissions=create_forwarder_permissions,
+            decode_authorizer_context=decode_authorizer_context,
+            enable_cold_start_tracing=enable_cold_start_tracing,
+            enable_datadog_logs=enable_datadog_logs,
+            enable_datadog_tracing=enable_datadog_tracing,
+            enable_merge_xray_traces=enable_merge_xray_traces,
+            enable_profiling=enable_profiling,
+            encode_authorizer_context=encode_authorizer_context,
+            env=env,
+            extension_layer_version=extension_layer_version,
+            flush_metrics_to_logs=flush_metrics_to_logs,
+            forwarder_arn=forwarder_arn,
+            inject_log_context=inject_log_context,
+            java_layer_version=java_layer_version,
+            log_level=log_level,
+            min_cold_start_trace_duration=min_cold_start_trace_duration,
+            node_layer_version=node_layer_version,
+            python_layer_version=python_layer_version,
+            redirect_handler=redirect_handler,
+            service=service,
+            site=site,
+            source_code_integration=source_code_integration,
+            tags=tags,
+            version=version,
+        )
+
+        jsii.create(self.__class__, self, [scope, id, props])
+
+    @jsii.member(jsii_name="addForwarderToNonLambdaLogGroups")
+    def add_forwarder_to_non_lambda_log_groups(
+        self,
+        log_groups: typing.Sequence[_aws_cdk_aws_logs_ceddda9d.ILogGroup],
+    ) -> None:
+        '''
+        :param log_groups: -
+        '''
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__b2299a0a72b8c17837c229cea786d90db2682af81487298b4e2cf18be55f3dc9)
+            check_type(argname="argument log_groups", value=log_groups, expected_type=type_hints["log_groups"])
+        return typing.cast(None, jsii.invoke(self, "addForwarderToNonLambdaLogGroups", [log_groups]))
+
+    @jsii.member(jsii_name="addGitCommitMetadata")
+    def add_git_commit_metadata(
+        self,
+        lambda_functions: typing.Sequence[typing.Union[_aws_cdk_aws_lambda_ceddda9d.Function, _aws_cdk_aws_lambda_nodejs_ceddda9d.NodejsFunction, _aws_cdk_aws_lambda_python_alpha_49328424.PythonFunction]],
+        git_commit_sha: typing.Optional[builtins.str] = None,
+        git_repo_url: typing.Optional[builtins.str] = None,
+    ) -> None:
+        '''
+        :param lambda_functions: -
+        :param git_commit_sha: -
+        :param git_repo_url: -
+        '''
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__313fba2a998cdf3ba070c09b0db7a32884ad3e5a7bb9eeaf8861202b45695e8e)
+            check_type(argname="argument lambda_functions", value=lambda_functions, expected_type=type_hints["lambda_functions"])
+            check_type(argname="argument git_commit_sha", value=git_commit_sha, expected_type=type_hints["git_commit_sha"])
+            check_type(argname="argument git_repo_url", value=git_repo_url, expected_type=type_hints["git_repo_url"])
+        return typing.cast(None, jsii.invoke(self, "addGitCommitMetadata", [lambda_functions, git_commit_sha, git_repo_url]))
+
+    @jsii.member(jsii_name="addLambdaFunctions")
+    def add_lambda_functions(
+        self,
+        lambda_functions: typing.Sequence[typing.Union[_aws_cdk_aws_lambda_ceddda9d.Function, _aws_cdk_aws_lambda_nodejs_ceddda9d.NodejsFunction, _aws_cdk_aws_lambda_python_alpha_49328424.PythonFunction]],
+    ) -> None:
+        '''
+        :param lambda_functions: -
+        '''
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__0803e2c5aafb02535548377e1d71bf561393d99ceb98d9e94251f36f8877c881)
+            check_type(argname="argument lambda_functions", value=lambda_functions, expected_type=type_hints["lambda_functions"])
+        return typing.cast(None, jsii.invoke(self, "addLambdaFunctions", [lambda_functions]))
+
+    @builtins.property
+    @jsii.member(jsii_name="props")
+    def props(self) -> "DatadogPropsV2":
+        return typing.cast("DatadogPropsV2", jsii.get(self, "props"))
+
+    @props.setter
+    def props(self, value: "DatadogPropsV2") -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__09c760f7e7825eca68e7aa97831bccc7713602c7ae04ada36965093ff03a5fde)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
+        jsii.set(self, "props", value)
+
+    @builtins.property
+    @jsii.member(jsii_name="scope")
+    def scope(self) -> _constructs_77d1e7e8.Construct:
+        return typing.cast(_constructs_77d1e7e8.Construct, jsii.get(self, "scope"))
+
+    @scope.setter
+    def scope(self, value: _constructs_77d1e7e8.Construct) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__97e7b5b76f3d9485008479e9714d21001685c73b840230c21221107332409c06)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
+        jsii.set(self, "scope", value)
+
+    @builtins.property
+    @jsii.member(jsii_name="transport")
+    def transport(self) -> "Transport":
+        return typing.cast("Transport", jsii.get(self, "transport"))
+
+    @transport.setter
+    def transport(self, value: "Transport") -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__9fbc38dc0dcc9d23ae91b812a896ee83f74291c635b835f5075d3b2e8f971337)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
+        jsii.set(self, "transport", value)
+
+
+@jsii.data_type(
+    jsii_type="datadog-cdk-constructs-v2.DatadogPropsV2",
+    jsii_struct_bases=[],
+    name_mapping={
+        "add_layers": "addLayers",
+        "api_key": "apiKey",
+        "api_key_secret": "apiKeySecret",
+        "api_key_secret_arn": "apiKeySecretArn",
+        "api_kms_key": "apiKmsKey",
+        "apm_flush_deadline": "apmFlushDeadline",
+        "capture_lambda_payload": "captureLambdaPayload",
+        "cold_start_trace_skip_libs": "coldStartTraceSkipLibs",
+        "create_forwarder_permissions": "createForwarderPermissions",
+        "decode_authorizer_context": "decodeAuthorizerContext",
+        "enable_cold_start_tracing": "enableColdStartTracing",
+        "enable_datadog_logs": "enableDatadogLogs",
+        "enable_datadog_tracing": "enableDatadogTracing",
+        "enable_merge_xray_traces": "enableMergeXrayTraces",
+        "enable_profiling": "enableProfiling",
+        "encode_authorizer_context": "encodeAuthorizerContext",
+        "env": "env",
+        "extension_layer_version": "extensionLayerVersion",
+        "flush_metrics_to_logs": "flushMetricsToLogs",
+        "forwarder_arn": "forwarderArn",
+        "inject_log_context": "injectLogContext",
+        "java_layer_version": "javaLayerVersion",
+        "log_level": "logLevel",
+        "min_cold_start_trace_duration": "minColdStartTraceDuration",
+        "node_layer_version": "nodeLayerVersion",
+        "python_layer_version": "pythonLayerVersion",
+        "redirect_handler": "redirectHandler",
+        "service": "service",
+        "site": "site",
+        "source_code_integration": "sourceCodeIntegration",
+        "tags": "tags",
+        "version": "version",
+    },
+)
+class DatadogPropsV2:
+    def __init__(
+        self,
+        *,
+        add_layers: typing.Optional[builtins.bool] = None,
+        api_key: typing.Optional[builtins.str] = None,
+        api_key_secret: typing.Optional[_aws_cdk_aws_secretsmanager_ceddda9d.ISecret] = None,
+        api_key_secret_arn: typing.Optional[builtins.str] = None,
+        api_kms_key: typing.Optional[builtins.str] = None,
+        apm_flush_deadline: typing.Optional[typing.Union[builtins.str, jsii.Number]] = None,
+        capture_lambda_payload: typing.Optional[builtins.bool] = None,
+        cold_start_trace_skip_libs: typing.Optional[builtins.str] = None,
+        create_forwarder_permissions: typing.Optional[builtins.bool] = None,
+        decode_authorizer_context: typing.Optional[builtins.bool] = None,
+        enable_cold_start_tracing: typing.Optional[builtins.bool] = None,
+        enable_datadog_logs: typing.Optional[builtins.bool] = None,
+        enable_datadog_tracing: typing.Optional[builtins.bool] = None,
+        enable_merge_xray_traces: typing.Optional[builtins.bool] = None,
+        enable_profiling: typing.Optional[builtins.bool] = None,
+        encode_authorizer_context: typing.Optional[builtins.bool] = None,
+        env: typing.Optional[builtins.str] = None,
+        extension_layer_version: typing.Optional[jsii.Number] = None,
+        flush_metrics_to_logs: typing.Optional[builtins.bool] = None,
+        forwarder_arn: typing.Optional[builtins.str] = None,
+        inject_log_context: typing.Optional[builtins.bool] = None,
+        java_layer_version: typing.Optional[jsii.Number] = None,
+        log_level: typing.Optional[builtins.str] = None,
+        min_cold_start_trace_duration: typing.Optional[jsii.Number] = None,
+        node_layer_version: typing.Optional[jsii.Number] = None,
+        python_layer_version: typing.Optional[jsii.Number] = None,
+        redirect_handler: typing.Optional[builtins.bool] = None,
+        service: typing.Optional[builtins.str] = None,
+        site: typing.Optional[builtins.str] = None,
+        source_code_integration: typing.Optional[builtins.bool] = None,
+        tags: typing.Optional[builtins.str] = None,
+        version: typing.Optional[builtins.str] = None,
+    ) -> None:
+        '''
+        :param add_layers: 
+        :param api_key: 
+        :param api_key_secret: 
+        :param api_key_secret_arn: 
+        :param api_kms_key: 
+        :param apm_flush_deadline: 
+        :param capture_lambda_payload: 
+        :param cold_start_trace_skip_libs: 
+        :param create_forwarder_permissions: 
+        :param decode_authorizer_context: 
+        :param enable_cold_start_tracing: 
+        :param enable_datadog_logs: 
+        :param enable_datadog_tracing: 
+        :param enable_merge_xray_traces: 
+        :param enable_profiling: 
+        :param encode_authorizer_context: 
+        :param env: 
+        :param extension_layer_version: 
+        :param flush_metrics_to_logs: 
+        :param forwarder_arn: 
+        :param inject_log_context: 
+        :param java_layer_version: 
+        :param log_level: 
+        :param min_cold_start_trace_duration: 
+        :param node_layer_version: 
+        :param python_layer_version: 
+        :param redirect_handler: 
+        :param service: 
+        :param site: 
+        :param source_code_integration: 
+        :param tags: 
+        :param version: 
+        '''
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__605aaf2fbceb6cc8efeeafa174ece774a500681952f201662eed10acfc3ab544)
+            check_type(argname="argument add_layers", value=add_layers, expected_type=type_hints["add_layers"])
+            check_type(argname="argument api_key", value=api_key, expected_type=type_hints["api_key"])
+            check_type(argname="argument api_key_secret", value=api_key_secret, expected_type=type_hints["api_key_secret"])
+            check_type(argname="argument api_key_secret_arn", value=api_key_secret_arn, expected_type=type_hints["api_key_secret_arn"])
+            check_type(argname="argument api_kms_key", value=api_kms_key, expected_type=type_hints["api_kms_key"])
+            check_type(argname="argument apm_flush_deadline", value=apm_flush_deadline, expected_type=type_hints["apm_flush_deadline"])
+            check_type(argname="argument capture_lambda_payload", value=capture_lambda_payload, expected_type=type_hints["capture_lambda_payload"])
+            check_type(argname="argument cold_start_trace_skip_libs", value=cold_start_trace_skip_libs, expected_type=type_hints["cold_start_trace_skip_libs"])
+            check_type(argname="argument create_forwarder_permissions", value=create_forwarder_permissions, expected_type=type_hints["create_forwarder_permissions"])
+            check_type(argname="argument decode_authorizer_context", value=decode_authorizer_context, expected_type=type_hints["decode_authorizer_context"])
+            check_type(argname="argument enable_cold_start_tracing", value=enable_cold_start_tracing, expected_type=type_hints["enable_cold_start_tracing"])
+            check_type(argname="argument enable_datadog_logs", value=enable_datadog_logs, expected_type=type_hints["enable_datadog_logs"])
+            check_type(argname="argument enable_datadog_tracing", value=enable_datadog_tracing, expected_type=type_hints["enable_datadog_tracing"])
+            check_type(argname="argument enable_merge_xray_traces", value=enable_merge_xray_traces, expected_type=type_hints["enable_merge_xray_traces"])
+            check_type(argname="argument enable_profiling", value=enable_profiling, expected_type=type_hints["enable_profiling"])
+            check_type(argname="argument encode_authorizer_context", value=encode_authorizer_context, expected_type=type_hints["encode_authorizer_context"])
+            check_type(argname="argument env", value=env, expected_type=type_hints["env"])
+            check_type(argname="argument extension_layer_version", value=extension_layer_version, expected_type=type_hints["extension_layer_version"])
+            check_type(argname="argument flush_metrics_to_logs", value=flush_metrics_to_logs, expected_type=type_hints["flush_metrics_to_logs"])
+            check_type(argname="argument forwarder_arn", value=forwarder_arn, expected_type=type_hints["forwarder_arn"])
+            check_type(argname="argument inject_log_context", value=inject_log_context, expected_type=type_hints["inject_log_context"])
+            check_type(argname="argument java_layer_version", value=java_layer_version, expected_type=type_hints["java_layer_version"])
+            check_type(argname="argument log_level", value=log_level, expected_type=type_hints["log_level"])
+            check_type(argname="argument min_cold_start_trace_duration", value=min_cold_start_trace_duration, expected_type=type_hints["min_cold_start_trace_duration"])
+            check_type(argname="argument node_layer_version", value=node_layer_version, expected_type=type_hints["node_layer_version"])
+            check_type(argname="argument python_layer_version", value=python_layer_version, expected_type=type_hints["python_layer_version"])
+            check_type(argname="argument redirect_handler", value=redirect_handler, expected_type=type_hints["redirect_handler"])
+            check_type(argname="argument service", value=service, expected_type=type_hints["service"])
+            check_type(argname="argument site", value=site, expected_type=type_hints["site"])
+            check_type(argname="argument source_code_integration", value=source_code_integration, expected_type=type_hints["source_code_integration"])
+            check_type(argname="argument tags", value=tags, expected_type=type_hints["tags"])
+            check_type(argname="argument version", value=version, expected_type=type_hints["version"])
+        self._values: typing.Dict[builtins.str, typing.Any] = {}
+        if add_layers is not None:
+            self._values["add_layers"] = add_layers
+        if api_key is not None:
+            self._values["api_key"] = api_key
+        if api_key_secret is not None:
+            self._values["api_key_secret"] = api_key_secret
+        if api_key_secret_arn is not None:
+            self._values["api_key_secret_arn"] = api_key_secret_arn
+        if api_kms_key is not None:
+            self._values["api_kms_key"] = api_kms_key
+        if apm_flush_deadline is not None:
+            self._values["apm_flush_deadline"] = apm_flush_deadline
+        if capture_lambda_payload is not None:
+            self._values["capture_lambda_payload"] = capture_lambda_payload
+        if cold_start_trace_skip_libs is not None:
+            self._values["cold_start_trace_skip_libs"] = cold_start_trace_skip_libs
+        if create_forwarder_permissions is not None:
+            self._values["create_forwarder_permissions"] = create_forwarder_permissions
+        if decode_authorizer_context is not None:
+            self._values["decode_authorizer_context"] = decode_authorizer_context
+        if enable_cold_start_tracing is not None:
+            self._values["enable_cold_start_tracing"] = enable_cold_start_tracing
+        if enable_datadog_logs is not None:
+            self._values["enable_datadog_logs"] = enable_datadog_logs
+        if enable_datadog_tracing is not None:
+            self._values["enable_datadog_tracing"] = enable_datadog_tracing
+        if enable_merge_xray_traces is not None:
+            self._values["enable_merge_xray_traces"] = enable_merge_xray_traces
+        if enable_profiling is not None:
+            self._values["enable_profiling"] = enable_profiling
+        if encode_authorizer_context is not None:
+            self._values["encode_authorizer_context"] = encode_authorizer_context
+        if env is not None:
+            self._values["env"] = env
+        if extension_layer_version is not None:
+            self._values["extension_layer_version"] = extension_layer_version
+        if flush_metrics_to_logs is not None:
+            self._values["flush_metrics_to_logs"] = flush_metrics_to_logs
+        if forwarder_arn is not None:
+            self._values["forwarder_arn"] = forwarder_arn
+        if inject_log_context is not None:
+            self._values["inject_log_context"] = inject_log_context
+        if java_layer_version is not None:
+            self._values["java_layer_version"] = java_layer_version
+        if log_level is not None:
+            self._values["log_level"] = log_level
+        if min_cold_start_trace_duration is not None:
+            self._values["min_cold_start_trace_duration"] = min_cold_start_trace_duration
+        if node_layer_version is not None:
+            self._values["node_layer_version"] = node_layer_version
+        if python_layer_version is not None:
+            self._values["python_layer_version"] = python_layer_version
+        if redirect_handler is not None:
+            self._values["redirect_handler"] = redirect_handler
+        if service is not None:
+            self._values["service"] = service
+        if site is not None:
+            self._values["site"] = site
+        if source_code_integration is not None:
+            self._values["source_code_integration"] = source_code_integration
+        if tags is not None:
+            self._values["tags"] = tags
+        if version is not None:
+            self._values["version"] = version
+
+    @builtins.property
+    def add_layers(self) -> typing.Optional[builtins.bool]:
+        result = self._values.get("add_layers")
+        return typing.cast(typing.Optional[builtins.bool], result)
+
+    @builtins.property
+    def api_key(self) -> typing.Optional[builtins.str]:
+        result = self._values.get("api_key")
+        return typing.cast(typing.Optional[builtins.str], result)
+
+    @builtins.property
+    def api_key_secret(
+        self,
+    ) -> typing.Optional[_aws_cdk_aws_secretsmanager_ceddda9d.ISecret]:
+        result = self._values.get("api_key_secret")
+        return typing.cast(typing.Optional[_aws_cdk_aws_secretsmanager_ceddda9d.ISecret], result)
+
+    @builtins.property
+    def api_key_secret_arn(self) -> typing.Optional[builtins.str]:
+        result = self._values.get("api_key_secret_arn")
+        return typing.cast(typing.Optional[builtins.str], result)
+
+    @builtins.property
+    def api_kms_key(self) -> typing.Optional[builtins.str]:
+        result = self._values.get("api_kms_key")
+        return typing.cast(typing.Optional[builtins.str], result)
+
+    @builtins.property
+    def apm_flush_deadline(
+        self,
+    ) -> typing.Optional[typing.Union[builtins.str, jsii.Number]]:
+        result = self._values.get("apm_flush_deadline")
+        return typing.cast(typing.Optional[typing.Union[builtins.str, jsii.Number]], result)
+
+    @builtins.property
+    def capture_lambda_payload(self) -> typing.Optional[builtins.bool]:
+        result = self._values.get("capture_lambda_payload")
+        return typing.cast(typing.Optional[builtins.bool], result)
+
+    @builtins.property
+    def cold_start_trace_skip_libs(self) -> typing.Optional[builtins.str]:
+        result = self._values.get("cold_start_trace_skip_libs")
+        return typing.cast(typing.Optional[builtins.str], result)
+
+    @builtins.property
+    def create_forwarder_permissions(self) -> typing.Optional[builtins.bool]:
+        result = self._values.get("create_forwarder_permissions")
+        return typing.cast(typing.Optional[builtins.bool], result)
+
+    @builtins.property
+    def decode_authorizer_context(self) -> typing.Optional[builtins.bool]:
+        result = self._values.get("decode_authorizer_context")
+        return typing.cast(typing.Optional[builtins.bool], result)
+
+    @builtins.property
+    def enable_cold_start_tracing(self) -> typing.Optional[builtins.bool]:
+        result = self._values.get("enable_cold_start_tracing")
+        return typing.cast(typing.Optional[builtins.bool], result)
+
+    @builtins.property
+    def enable_datadog_logs(self) -> typing.Optional[builtins.bool]:
+        result = self._values.get("enable_datadog_logs")
+        return typing.cast(typing.Optional[builtins.bool], result)
+
+    @builtins.property
+    def enable_datadog_tracing(self) -> typing.Optional[builtins.bool]:
+        result = self._values.get("enable_datadog_tracing")
+        return typing.cast(typing.Optional[builtins.bool], result)
+
+    @builtins.property
+    def enable_merge_xray_traces(self) -> typing.Optional[builtins.bool]:
+        result = self._values.get("enable_merge_xray_traces")
+        return typing.cast(typing.Optional[builtins.bool], result)
+
+    @builtins.property
+    def enable_profiling(self) -> typing.Optional[builtins.bool]:
+        result = self._values.get("enable_profiling")
+        return typing.cast(typing.Optional[builtins.bool], result)
+
+    @builtins.property
+    def encode_authorizer_context(self) -> typing.Optional[builtins.bool]:
+        result = self._values.get("encode_authorizer_context")
+        return typing.cast(typing.Optional[builtins.bool], result)
+
+    @builtins.property
+    def env(self) -> typing.Optional[builtins.str]:
+        result = self._values.get("env")
+        return typing.cast(typing.Optional[builtins.str], result)
+
+    @builtins.property
+    def extension_layer_version(self) -> typing.Optional[jsii.Number]:
+        result = self._values.get("extension_layer_version")
+        return typing.cast(typing.Optional[jsii.Number], result)
+
+    @builtins.property
+    def flush_metrics_to_logs(self) -> typing.Optional[builtins.bool]:
+        result = self._values.get("flush_metrics_to_logs")
+        return typing.cast(typing.Optional[builtins.bool], result)
+
+    @builtins.property
+    def forwarder_arn(self) -> typing.Optional[builtins.str]:
+        result = self._values.get("forwarder_arn")
+        return typing.cast(typing.Optional[builtins.str], result)
+
+    @builtins.property
+    def inject_log_context(self) -> typing.Optional[builtins.bool]:
+        result = self._values.get("inject_log_context")
+        return typing.cast(typing.Optional[builtins.bool], result)
+
+    @builtins.property
+    def java_layer_version(self) -> typing.Optional[jsii.Number]:
+        result = self._values.get("java_layer_version")
+        return typing.cast(typing.Optional[jsii.Number], result)
+
+    @builtins.property
+    def log_level(self) -> typing.Optional[builtins.str]:
+        result = self._values.get("log_level")
+        return typing.cast(typing.Optional[builtins.str], result)
+
+    @builtins.property
+    def min_cold_start_trace_duration(self) -> typing.Optional[jsii.Number]:
+        result = self._values.get("min_cold_start_trace_duration")
+        return typing.cast(typing.Optional[jsii.Number], result)
+
+    @builtins.property
+    def node_layer_version(self) -> typing.Optional[jsii.Number]:
+        result = self._values.get("node_layer_version")
+        return typing.cast(typing.Optional[jsii.Number], result)
+
+    @builtins.property
+    def python_layer_version(self) -> typing.Optional[jsii.Number]:
+        result = self._values.get("python_layer_version")
+        return typing.cast(typing.Optional[jsii.Number], result)
+
+    @builtins.property
+    def redirect_handler(self) -> typing.Optional[builtins.bool]:
+        result = self._values.get("redirect_handler")
+        return typing.cast(typing.Optional[builtins.bool], result)
+
+    @builtins.property
+    def service(self) -> typing.Optional[builtins.str]:
+        result = self._values.get("service")
+        return typing.cast(typing.Optional[builtins.str], result)
+
+    @builtins.property
+    def site(self) -> typing.Optional[builtins.str]:
+        result = self._values.get("site")
+        return typing.cast(typing.Optional[builtins.str], result)
+
+    @builtins.property
+    def source_code_integration(self) -> typing.Optional[builtins.bool]:
+        result = self._values.get("source_code_integration")
+        return typing.cast(typing.Optional[builtins.bool], result)
+
+    @builtins.property
+    def tags(self) -> typing.Optional[builtins.str]:
+        result = self._values.get("tags")
+        return typing.cast(typing.Optional[builtins.str], result)
+
+    @builtins.property
+    def version(self) -> typing.Optional[builtins.str]:
+        result = self._values.get("version")
+        return typing.cast(typing.Optional[builtins.str], result)
+
+    def __eq__(self, rhs: typing.Any) -> builtins.bool:
+        return isinstance(rhs, self.__class__) and rhs._values == self._values
+
+    def __ne__(self, rhs: typing.Any) -> builtins.bool:
+        return not (rhs == self)
+
+    def __repr__(self) -> str:
+        return "DatadogPropsV2(%s)" % ", ".join(
+            k + "=" + repr(v) for k, v in self._values.items()
+        )
+
 
 @jsii.data_type(
     jsii_type="datadog-cdk-constructs-v2.DatadogStrictProps",
     jsii_struct_bases=[],
     name_mapping={
         "add_layers": "addLayers",
         "capture_lambda_payload": "captureLambdaPayload",
@@ -1225,26 +1819,144 @@
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__b5e4df65851315cbd779a7d51db28b4f9f2ff24e8d2030ab94830e4548e02f64)
             check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "extensionLayerVersion", value)
 
 
 __all__ = [
+    "Datadog",
+    "DatadogPropsV2",
     "DatadogStrictProps",
     "IDatadogProps",
     "ILambdaFunction",
     "Node",
     "Runtime",
     "RuntimeType",
     "TagKeys",
     "Transport",
 ]
 
 publication.publish()
 
+def _typecheckingstub__74e095ab68a1ec6a36ad77e9741c22f8922ea76270d93f498ffa8f7846214a75(
+    scope: _constructs_77d1e7e8.Construct,
+    id: builtins.str,
+    *,
+    add_layers: typing.Optional[builtins.bool] = None,
+    api_key: typing.Optional[builtins.str] = None,
+    api_key_secret: typing.Optional[_aws_cdk_aws_secretsmanager_ceddda9d.ISecret] = None,
+    api_key_secret_arn: typing.Optional[builtins.str] = None,
+    api_kms_key: typing.Optional[builtins.str] = None,
+    apm_flush_deadline: typing.Optional[typing.Union[builtins.str, jsii.Number]] = None,
+    capture_lambda_payload: typing.Optional[builtins.bool] = None,
+    cold_start_trace_skip_libs: typing.Optional[builtins.str] = None,
+    create_forwarder_permissions: typing.Optional[builtins.bool] = None,
+    decode_authorizer_context: typing.Optional[builtins.bool] = None,
+    enable_cold_start_tracing: typing.Optional[builtins.bool] = None,
+    enable_datadog_logs: typing.Optional[builtins.bool] = None,
+    enable_datadog_tracing: typing.Optional[builtins.bool] = None,
+    enable_merge_xray_traces: typing.Optional[builtins.bool] = None,
+    enable_profiling: typing.Optional[builtins.bool] = None,
+    encode_authorizer_context: typing.Optional[builtins.bool] = None,
+    env: typing.Optional[builtins.str] = None,
+    extension_layer_version: typing.Optional[jsii.Number] = None,
+    flush_metrics_to_logs: typing.Optional[builtins.bool] = None,
+    forwarder_arn: typing.Optional[builtins.str] = None,
+    inject_log_context: typing.Optional[builtins.bool] = None,
+    java_layer_version: typing.Optional[jsii.Number] = None,
+    log_level: typing.Optional[builtins.str] = None,
+    min_cold_start_trace_duration: typing.Optional[jsii.Number] = None,
+    node_layer_version: typing.Optional[jsii.Number] = None,
+    python_layer_version: typing.Optional[jsii.Number] = None,
+    redirect_handler: typing.Optional[builtins.bool] = None,
+    service: typing.Optional[builtins.str] = None,
+    site: typing.Optional[builtins.str] = None,
+    source_code_integration: typing.Optional[builtins.bool] = None,
+    tags: typing.Optional[builtins.str] = None,
+    version: typing.Optional[builtins.str] = None,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__b2299a0a72b8c17837c229cea786d90db2682af81487298b4e2cf18be55f3dc9(
+    log_groups: typing.Sequence[_aws_cdk_aws_logs_ceddda9d.ILogGroup],
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__313fba2a998cdf3ba070c09b0db7a32884ad3e5a7bb9eeaf8861202b45695e8e(
+    lambda_functions: typing.Sequence[typing.Union[_aws_cdk_aws_lambda_ceddda9d.Function, _aws_cdk_aws_lambda_nodejs_ceddda9d.NodejsFunction, _aws_cdk_aws_lambda_python_alpha_49328424.PythonFunction]],
+    git_commit_sha: typing.Optional[builtins.str] = None,
+    git_repo_url: typing.Optional[builtins.str] = None,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__0803e2c5aafb02535548377e1d71bf561393d99ceb98d9e94251f36f8877c881(
+    lambda_functions: typing.Sequence[typing.Union[_aws_cdk_aws_lambda_ceddda9d.Function, _aws_cdk_aws_lambda_nodejs_ceddda9d.NodejsFunction, _aws_cdk_aws_lambda_python_alpha_49328424.PythonFunction]],
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__09c760f7e7825eca68e7aa97831bccc7713602c7ae04ada36965093ff03a5fde(
+    value: DatadogPropsV2,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__97e7b5b76f3d9485008479e9714d21001685c73b840230c21221107332409c06(
+    value: _constructs_77d1e7e8.Construct,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__9fbc38dc0dcc9d23ae91b812a896ee83f74291c635b835f5075d3b2e8f971337(
+    value: Transport,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__605aaf2fbceb6cc8efeeafa174ece774a500681952f201662eed10acfc3ab544(
+    *,
+    add_layers: typing.Optional[builtins.bool] = None,
+    api_key: typing.Optional[builtins.str] = None,
+    api_key_secret: typing.Optional[_aws_cdk_aws_secretsmanager_ceddda9d.ISecret] = None,
+    api_key_secret_arn: typing.Optional[builtins.str] = None,
+    api_kms_key: typing.Optional[builtins.str] = None,
+    apm_flush_deadline: typing.Optional[typing.Union[builtins.str, jsii.Number]] = None,
+    capture_lambda_payload: typing.Optional[builtins.bool] = None,
+    cold_start_trace_skip_libs: typing.Optional[builtins.str] = None,
+    create_forwarder_permissions: typing.Optional[builtins.bool] = None,
+    decode_authorizer_context: typing.Optional[builtins.bool] = None,
+    enable_cold_start_tracing: typing.Optional[builtins.bool] = None,
+    enable_datadog_logs: typing.Optional[builtins.bool] = None,
+    enable_datadog_tracing: typing.Optional[builtins.bool] = None,
+    enable_merge_xray_traces: typing.Optional[builtins.bool] = None,
+    enable_profiling: typing.Optional[builtins.bool] = None,
+    encode_authorizer_context: typing.Optional[builtins.bool] = None,
+    env: typing.Optional[builtins.str] = None,
+    extension_layer_version: typing.Optional[jsii.Number] = None,
+    flush_metrics_to_logs: typing.Optional[builtins.bool] = None,
+    forwarder_arn: typing.Optional[builtins.str] = None,
+    inject_log_context: typing.Optional[builtins.bool] = None,
+    java_layer_version: typing.Optional[jsii.Number] = None,
+    log_level: typing.Optional[builtins.str] = None,
+    min_cold_start_trace_duration: typing.Optional[jsii.Number] = None,
+    node_layer_version: typing.Optional[jsii.Number] = None,
+    python_layer_version: typing.Optional[jsii.Number] = None,
+    redirect_handler: typing.Optional[builtins.bool] = None,
+    service: typing.Optional[builtins.str] = None,
+    site: typing.Optional[builtins.str] = None,
+    source_code_integration: typing.Optional[builtins.bool] = None,
+    tags: typing.Optional[builtins.str] = None,
+    version: typing.Optional[builtins.str] = None,
+) -> None:
+    """Type checking stubs"""
+    pass
+
 def _typecheckingstub__c0d4909ff321b27042bd7da99817517e719945ec07952fd9fd3a213ccaf8b9d4(
     *,
     add_layers: builtins.bool,
     capture_lambda_payload: builtins.bool,
     enable_datadog_logs: builtins.bool,
     enable_datadog_tracing: builtins.bool,
     enable_merge_xray_traces: builtins.bool,
```

### Comparing `datadog-cdk-constructs-v2-1.7.0/src/datadog_cdk_constructs_v2.egg-info/PKG-INFO` & `datadog-cdk-constructs-v2-1.7.1/src/datadog_cdk_constructs_v2.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datadog-cdk-constructs-v2
-Version: 1.7.0
+Version: 1.7.1
 Summary: CDK Construct Library to automatically instrument Python and Node Lambda functions with Datadog using AWS CDK v2
 Home-page: https://github.com/DataDog/datadog-cdk-constructs
 Author: Datadog
 License: Apache-2.0
 Project-URL: Source, https://github.com/DataDog/datadog-cdk-constructs
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

### Comparing `datadog-cdk-constructs-v2-1.7.0/src/datadog_cdk_constructs_v2.egg-info/SOURCES.txt` & `datadog-cdk-constructs-v2-1.7.1/src/datadog_cdk_constructs_v2.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -7,8 +7,8 @@
 src/datadog_cdk_constructs_v2/py.typed
 src/datadog_cdk_constructs_v2.egg-info/PKG-INFO
 src/datadog_cdk_constructs_v2.egg-info/SOURCES.txt
 src/datadog_cdk_constructs_v2.egg-info/dependency_links.txt
 src/datadog_cdk_constructs_v2.egg-info/requires.txt
 src/datadog_cdk_constructs_v2.egg-info/top_level.txt
 src/datadog_cdk_constructs_v2/_jsii/__init__.py
-src/datadog_cdk_constructs_v2/_jsii/datadog-cdk-constructs-v2@1.7.0.jsii.tgz
+src/datadog_cdk_constructs_v2/_jsii/datadog-cdk-constructs-v2@1.7.1.jsii.tgz
```

