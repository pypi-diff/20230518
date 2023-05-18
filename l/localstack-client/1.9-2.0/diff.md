# Comparing `tmp/localstack-client-1.9.tar.gz` & `tmp/localstack-client-2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/localstack-client-1.9.tar", last modified: Sun Dec  6 13:46:10 2020, max compression
+gzip compressed data, was "localstack-client-2.0.tar", last modified: Thu Mar 23 12:00:17 2023, max compression
```

## Comparing `localstack-client-1.9.tar` & `localstack-client-2.0.tar`

### file list

```diff
@@ -1,15 +1,17 @@
-drwxr-xr-x   0 whummer    (502) staff       (20)        0 2020-12-06 13:46:10.000000 localstack-client-1.9/
--rw-r--r--   0 whummer    (502) staff       (20)      871 2020-12-06 13:46:10.000000 localstack-client-1.9/PKG-INFO
--rw-r--r--   0 whummer    (502) staff       (20)     3185 2020-11-04 08:06:10.000000 localstack-client-1.9/README.md
-drwxr-xr-x   0 whummer    (502) staff       (20)        0 2020-12-06 13:46:10.000000 localstack-client-1.9/localstack_client/
--rw-r--r--   0 whummer    (502) staff       (20)        0 2019-06-08 20:46:10.000000 localstack-client-1.9/localstack_client/__init__.py
--rw-r--r--   0 whummer    (502) staff       (20)     4651 2020-12-06 12:12:34.000000 localstack-client-1.9/localstack_client/config.py
--rw-r--r--   0 whummer    (502) staff       (20)     2470 2020-05-09 08:10:08.000000 localstack-client-1.9/localstack_client/session.py
-drwxr-xr-x   0 whummer    (502) staff       (20)        0 2020-12-06 13:46:10.000000 localstack-client-1.9/localstack_client.egg-info/
--rw-r--r--   0 whummer    (502) staff       (20)      871 2020-12-06 13:46:10.000000 localstack-client-1.9/localstack_client.egg-info/PKG-INFO
--rw-r--r--   0 whummer    (502) staff       (20)      309 2020-12-06 13:46:10.000000 localstack-client-1.9/localstack_client.egg-info/SOURCES.txt
--rw-r--r--   0 whummer    (502) staff       (20)        1 2020-12-06 13:46:10.000000 localstack-client-1.9/localstack_client.egg-info/dependency_links.txt
--rw-r--r--   0 whummer    (502) staff       (20)        6 2020-12-06 13:46:10.000000 localstack-client-1.9/localstack_client.egg-info/requires.txt
--rw-r--r--   0 whummer    (502) staff       (20)       18 2020-12-06 13:46:10.000000 localstack-client-1.9/localstack_client.egg-info/top_level.txt
--rw-r--r--   0 whummer    (502) staff       (20)       38 2020-12-06 13:46:10.000000 localstack-client-1.9/setup.cfg
--rwxr-xr-x   0 whummer    (502) staff       (20)     1165 2020-12-06 12:13:20.000000 localstack-client-1.9/setup.py
+drwxr-xr-x   0 simon     (1000) users      (100)        0 2023-03-23 12:00:17.444707 localstack-client-2.0/
+-rw-r--r--   0 simon     (1000) users      (100)    11357 2023-01-01 23:55:15.000000 localstack-client-2.0/LICENSE
+-rw-r--r--   0 simon     (1000) users      (100)      673 2023-03-23 12:00:17.445706 localstack-client-2.0/PKG-INFO
+-rw-r--r--   0 simon     (1000) users      (100)     4166 2023-03-23 11:56:50.000000 localstack-client-2.0/README.md
+drwxr-xr-x   0 simon     (1000) users      (100)        0 2023-03-23 12:00:17.444707 localstack-client-2.0/localstack_client/
+-rw-r--r--   0 simon     (1000) users      (100)        0 2023-01-01 23:55:15.000000 localstack-client-2.0/localstack_client/__init__.py
+-rw-r--r--   0 simon     (1000) users      (100)     5179 2023-03-23 11:56:50.000000 localstack-client-2.0/localstack_client/config.py
+-rw-r--r--   0 simon     (1000) users      (100)     4637 2023-01-01 23:55:15.000000 localstack-client-2.0/localstack_client/patch.py
+-rw-r--r--   0 simon     (1000) users      (100)     3471 2023-01-01 23:55:15.000000 localstack-client-2.0/localstack_client/session.py
+drwxr-xr-x   0 simon     (1000) users      (100)        0 2023-03-23 12:00:17.444707 localstack-client-2.0/localstack_client.egg-info/
+-rw-r--r--   0 simon     (1000) users      (100)      673 2023-03-23 12:00:17.000000 localstack-client-2.0/localstack_client.egg-info/PKG-INFO
+-rw-r--r--   0 simon     (1000) users      (100)      354 2023-03-23 12:00:17.000000 localstack-client-2.0/localstack_client.egg-info/SOURCES.txt
+-rw-r--r--   0 simon     (1000) users      (100)        1 2023-03-23 12:00:17.000000 localstack-client-2.0/localstack_client.egg-info/dependency_links.txt
+-rw-r--r--   0 simon     (1000) users      (100)       60 2023-03-23 12:00:17.000000 localstack-client-2.0/localstack_client.egg-info/requires.txt
+-rw-r--r--   0 simon     (1000) users      (100)       18 2023-03-23 12:00:17.000000 localstack-client-2.0/localstack_client.egg-info/top_level.txt
+-rw-r--r--   0 simon     (1000) users      (100)      756 2023-03-23 12:00:17.445706 localstack-client-2.0/setup.cfg
+-rwxr-xr-x   0 simon     (1000) users      (100)       60 2023-01-01 23:55:15.000000 localstack-client-2.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `localstack-client-1.9/localstack_client/session.py` & `localstack-client-2.0/localstack_client/session.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,67 +1,109 @@
 from boto3 import client as boto3_client
 from boto3 import resource as boto3_resource
 from botocore.credentials import Credentials
+
 from localstack_client import config
 
 DEFAULT_SESSION = None
 
 
 class Session(object):
     """
     This is a custom LocalStack session used to
     emulate the boto3.session object.
     """
 
-    def __init__(self, aws_access_key_id='accesskey', aws_secret_access_key='secretkey',
-                 aws_session_token='token', region_name='us-east-1',
-                 botocore_session=None, profile_name=None, localstack_host=None):
-        self.env = 'local'
+    def __init__(
+        self,
+        aws_access_key_id="accesskey",
+        aws_secret_access_key="secretkey",
+        aws_session_token="token",
+        region_name="us-east-1",
+        botocore_session=None,
+        profile_name=None,
+        localstack_host=None,
+    ):
+        self.env = "local"
         self.aws_access_key_id = aws_access_key_id
         self.aws_secret_access_key = aws_secret_access_key
         self.aws_session_token = aws_session_token
         self.region_name = region_name
         self._service_endpoint_mapping = config.get_service_endpoints(localstack_host)
 
+        self.common_protected_kwargs = {
+            "aws_access_key_id": self.aws_access_key_id,
+            "aws_secret_access_key": self.aws_secret_access_key,
+            "region_name": self.region_name,
+            "verify": False,
+        }
+
     def get_credentials(self):
         """
         Returns botocore.credential.Credential object.
         """
-        return Credentials(access_key=self.aws_access_key_id,
-                           secret_key=self.aws_secret_access_key,
-                           token=self.aws_session_token)
+        return Credentials(
+            access_key=self.aws_access_key_id,
+            secret_key=self.aws_secret_access_key,
+            token=self.aws_session_token,
+        )
 
     def client(self, service_name, **kwargs):
+        """
+        Mock boto3 client
+        If **kwargs are provided they will passed through to boto3.client unless already contained
+        within protected_kwargs which are set with priority
+        Returns boto3.resources.factory.s3.ServiceClient object
+        """
         if service_name not in self._service_endpoint_mapping:
-            raise Exception('%s is not supported by this mock session.' % (service_name))
+            raise Exception(
+                "%s is not supported by this mock session." % (service_name)
+            )
+
+        protected_kwargs = {
+            **self.common_protected_kwargs,
+            "service_name": service_name,
+            "endpoint_url": self._service_endpoint_mapping[service_name],
+        }
 
-        return boto3_client(service_name,
-            endpoint_url=self._service_endpoint_mapping[service_name],
-            aws_access_key_id=self.aws_access_key_id, region_name=self.region_name,
-            aws_secret_access_key=self.aws_secret_access_key, verify=False)
+        return boto3_client(**{**kwargs, **protected_kwargs})
 
     def resource(self, service_name, **kwargs):
+        """
+        Mock boto3 resource
+        If **kwargs are provided they will passed through to boto3.client unless already contained
+        within overwrite_kwargs which are set with priority
+        Returns boto3.resources.factory.s3.ServiceResource object
+        """
         if service_name not in self._service_endpoint_mapping:
-            raise Exception('%s is not supported by this mock session.' % (service_name))
+            raise Exception(
+                "%s is not supported by this mock session." % (service_name)
+            )
+
+        protected_kwargs = {
+            **self.common_protected_kwargs,
+            "service_name": service_name,
+            "endpoint_url": self._service_endpoint_mapping[service_name],
+        }
 
-        return boto3_resource(service_name,
-            endpoint_url=self._service_endpoint_mapping[service_name],
-            aws_access_key_id=self.aws_access_key_id,
-            aws_secret_access_key=self.aws_secret_access_key,
-            region_name=self.region_name, verify=False)
+        return boto3_resource(**{**kwargs, **protected_kwargs})
 
 
 def _get_default_session():
     global DEFAULT_SESSION
 
     if DEFAULT_SESSION is None:
         DEFAULT_SESSION = Session()
 
     return DEFAULT_SESSION
 
 
 def client(*args, **kwargs):
+    if kwargs:
+        return Session(**kwargs).client(*args, **kwargs)
     return _get_default_session().client(*args, **kwargs)
 
 
 def resource(*args, **kwargs):
+    if kwargs:
+        return Session(**kwargs).resource(*args, **kwargs)
     return _get_default_session().resource(*args, **kwargs)
```

