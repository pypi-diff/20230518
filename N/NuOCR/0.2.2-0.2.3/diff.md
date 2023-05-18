# Comparing `tmp/NuOCR-0.2.2.tar.gz` & `tmp/NuOCR-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "NuOCR-0.2.2.tar", last modified: Tue Feb 28 11:41:45 2023, max compression
+gzip compressed data, was "NuOCR-0.2.3.tar", last modified: Thu May 18 07:56:53 2023, max compression
```

## Comparing `NuOCR-0.2.2.tar` & `NuOCR-0.2.3.tar`

### file list

```diff
@@ -1,45 +1,59 @@
-drwxrwxrwx   0        0        0        0 2023-02-28 11:41:45.045313 NuOCR-0.2.2/
-drwxrwxrwx   0        0        0        0 2023-02-28 11:41:43.564671 NuOCR-0.2.2/NuOCR/
--rw-rw-rw-   0        0        0      221 2023-02-10 07:27:31.000000 NuOCR-0.2.2/NuOCR/__init__.py
--rw-rw-rw-   0        0        0     2838 2023-02-10 18:17:35.000000 NuOCR-0.2.2/NuOCR/admin.py
--rw-rw-rw-   0        0        0      235 2023-02-03 06:00:42.000000 NuOCR-0.2.2/NuOCR/channel.py
--rw-rw-rw-   0        0        0     4923 2023-02-03 06:00:42.000000 NuOCR-0.2.2/NuOCR/extractor.py
-drwxrwxrwx   0        0        0        0 2023-02-28 11:41:43.819711 NuOCR-0.2.2/NuOCR/gRPC_proto/
--rw-rw-rw-   0        0        0      217 2023-02-10 07:27:30.000000 NuOCR-0.2.2/NuOCR/gRPC_proto/__init__.py
-drwxrwxrwx   0        0        0        0 2023-02-28 11:41:43.969761 NuOCR-0.2.2/NuOCR/gRPC_proto/extractor/
--rw-rw-rw-   0        0        0       65 2022-12-22 10:06:10.000000 NuOCR-0.2.2/NuOCR/gRPC_proto/extractor/__init__.py
--rw-rw-rw-   0        0        0     3683 2022-12-13 12:07:32.000000 NuOCR-0.2.2/NuOCR/gRPC_proto/extractor/extractor_pb2.py
--rw-rw-rw-   0        0        0     9046 2023-02-28 11:41:26.000000 NuOCR-0.2.2/NuOCR/gRPC_proto/extractor/extractor_pb2_grpc.py
-drwxrwxrwx   0        0        0        0 2023-02-28 11:41:44.134657 NuOCR-0.2.2/NuOCR/gRPC_proto/io_adaptors/
--rw-rw-rw-   0        0        0       69 2022-12-22 10:06:10.000000 NuOCR-0.2.2/NuOCR/gRPC_proto/io_adaptors/__init__.py
--rw-rw-rw-   0        0        0     3393 2023-01-24 18:21:30.000000 NuOCR-0.2.2/NuOCR/gRPC_proto/io_adaptors/io_adaptors_pb2.py
--rw-rw-rw-   0        0        0    11080 2023-02-28 11:41:25.000000 NuOCR-0.2.2/NuOCR/gRPC_proto/io_adaptors/io_adaptors_pb2_grpc.py
-drwxrwxrwx   0        0        0        0 2023-02-28 11:41:44.357253 NuOCR-0.2.2/NuOCR/gRPC_proto/templated_flow/
--rw-rw-rw-   0        0        0       75 2023-02-10 07:27:31.000000 NuOCR-0.2.2/NuOCR/gRPC_proto/templated_flow/__init__.py
--rw-rw-rw-   0        0        0     3333 2023-02-09 14:32:16.000000 NuOCR-0.2.2/NuOCR/gRPC_proto/templated_flow/templated_flow_pb2.py
--rw-rw-rw-   0        0        0     7931 2023-02-28 11:41:26.000000 NuOCR-0.2.2/NuOCR/gRPC_proto/templated_flow/templated_flow_pb2_grpc.py
-drwxrwxrwx   0        0        0        0 2023-02-28 11:41:44.658450 NuOCR-0.2.2/NuOCR/gRPC_proto/text_processor/
--rw-rw-rw-   0        0        0       75 2023-02-10 07:27:30.000000 NuOCR-0.2.2/NuOCR/gRPC_proto/text_processor/__init__.py
--rw-rw-rw-   0        0        0     1470 2023-02-01 11:25:55.000000 NuOCR-0.2.2/NuOCR/gRPC_proto/text_processor/text_processor_pb2.py
--rw-rw-rw-   0        0        0     4453 2023-02-10 09:31:12.000000 NuOCR-0.2.2/NuOCR/gRPC_proto/text_processor/text_processor_pb2_grpc.py
-drwxrwxrwx   0        0        0        0 2023-02-28 11:41:44.949249 NuOCR-0.2.2/NuOCR/gRPC_proto/user/
--rw-rw-rw-   0        0        0      110 2022-12-22 10:06:10.000000 NuOCR-0.2.2/NuOCR/gRPC_proto/user/__init__.py
--rw-rw-rw-   0        0        0     2029 2022-10-26 12:14:12.000000 NuOCR-0.2.2/NuOCR/gRPC_proto/user/auth_pb2.py
--rw-rw-rw-   0        0        0     2474 2023-02-28 11:41:26.000000 NuOCR-0.2.2/NuOCR/gRPC_proto/user/auth_pb2_grpc.py
--rw-rw-rw-   0        0        0     4286 2023-02-27 12:29:28.000000 NuOCR-0.2.2/NuOCR/gRPC_proto/user/user_pb2.py
--rw-rw-rw-   0        0        0    22209 2023-02-28 11:41:26.000000 NuOCR-0.2.2/NuOCR/gRPC_proto/user/user_pb2_grpc.py
--rw-rw-rw-   0        0        0     4959 2023-02-10 18:17:35.000000 NuOCR-0.2.2/NuOCR/io_adaptor.py
--rw-rw-rw-   0        0        0     2954 2023-02-10 18:17:35.000000 NuOCR-0.2.2/NuOCR/templated_flow.py
--rw-rw-rw-   0        0        0     1158 2023-02-10 18:17:36.000000 NuOCR-0.2.2/NuOCR/text.py
--rw-rw-rw-   0        0        0     1824 2023-02-10 18:17:35.000000 NuOCR-0.2.2/NuOCR/user.py
--rw-rw-rw-   0        0        0      334 2022-09-27 03:34:42.000000 NuOCR-0.2.2/NuOCR/util.py
-drwxrwxrwx   0        0        0        0 2023-02-28 11:41:43.795015 NuOCR-0.2.2/NuOCR.egg-info/
--rw-rw-rw-   0        0        0      538 2023-02-28 11:41:42.000000 NuOCR-0.2.2/NuOCR.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1114 2023-02-28 11:41:42.000000 NuOCR-0.2.2/NuOCR.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-02-28 11:41:42.000000 NuOCR-0.2.2/NuOCR.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2023-02-28 11:41:42.000000 NuOCR-0.2.2/NuOCR.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-02-28 11:41:42.000000 NuOCR-0.2.2/NuOCR.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      538 2023-02-28 11:41:45.013818 NuOCR-0.2.2/PKG-INFO
--rw-rw-rw-   0        0        0     4053 2022-09-22 07:20:26.000000 NuOCR-0.2.2/README.md
--rw-rw-rw-   0        0        0       42 2023-02-28 11:41:45.045313 NuOCR-0.2.2/setup.cfg
--rw-rw-rw-   0        0        0     1130 2023-02-28 11:41:26.000000 NuOCR-0.2.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-18 07:56:53.392330 NuOCR-0.2.3/
+drwxrwxrwx   0        0        0        0 2023-05-18 07:56:53.120329 NuOCR-0.2.3/NuOCR/
+-rw-rw-rw-   0        0        0      300 2023-05-18 07:54:08.000000 NuOCR-0.2.3/NuOCR/__init__.py
+-rw-rw-rw-   0        0        0     3656 2023-05-18 07:04:32.000000 NuOCR-0.2.3/NuOCR/admin.py
+-rw-rw-rw-   0        0        0      235 2023-03-27 09:59:57.000000 NuOCR-0.2.3/NuOCR/channel.py
+-rw-rw-rw-   0        0        0     1815 2023-05-17 09:02:23.000000 NuOCR-0.2.3/NuOCR/extractor.py
+drwxrwxrwx   0        0        0        0 2023-05-18 07:56:53.165618 NuOCR-0.2.3/NuOCR/gRPC_proto/
+-rw-rw-rw-   0        0        0      345 2023-05-17 09:02:23.000000 NuOCR-0.2.3/NuOCR/gRPC_proto/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-18 07:56:53.187086 NuOCR-0.2.3/NuOCR/gRPC_proto/extractor/
+-rw-rw-rw-   0        0        0       65 2023-03-27 09:59:57.000000 NuOCR-0.2.3/NuOCR/gRPC_proto/extractor/__init__.py
+-rw-rw-rw-   0        0        0     3683 2022-12-13 12:07:32.000000 NuOCR-0.2.3/NuOCR/gRPC_proto/extractor/extractor_pb2.py
+-rw-rw-rw-   0        0        0     9046 2023-05-17 08:54:24.000000 NuOCR-0.2.3/NuOCR/gRPC_proto/extractor/extractor_pb2_grpc.py
+drwxrwxrwx   0        0        0        0 2023-05-18 07:56:53.213904 NuOCR-0.2.3/NuOCR/gRPC_proto/io_adaptors/
+-rw-rw-rw-   0        0        0       69 2023-03-27 09:59:57.000000 NuOCR-0.2.3/NuOCR/gRPC_proto/io_adaptors/__init__.py
+-rw-rw-rw-   0        0        0     6399 2023-05-18 07:55:42.000000 NuOCR-0.2.3/NuOCR/gRPC_proto/io_adaptors/io_adaptors_pb2.py
+-rw-rw-rw-   0        0        0    25007 2023-05-18 07:55:52.000000 NuOCR-0.2.3/NuOCR/gRPC_proto/io_adaptors/io_adaptors_pb2_grpc.py
+drwxrwxrwx   0        0        0        0 2023-05-18 07:56:53.237446 NuOCR-0.2.3/NuOCR/gRPC_proto/monitor/
+-rw-rw-rw-   0        0        0       61 2023-05-17 08:56:56.000000 NuOCR-0.2.3/NuOCR/gRPC_proto/monitor/__init__.py
+-rw-rw-rw-   0        0        0     1797 2023-04-05 17:01:43.000000 NuOCR-0.2.3/NuOCR/gRPC_proto/monitor/monitor_pb2.py
+-rw-rw-rw-   0        0        0     9283 2023-05-17 08:56:56.000000 NuOCR-0.2.3/NuOCR/gRPC_proto/monitor/monitor_pb2_grpc.py
+drwxrwxrwx   0        0        0        0 2023-05-18 07:56:53.260427 NuOCR-0.2.3/NuOCR/gRPC_proto/nufarm_poc/
+-rw-rw-rw-   0        0        0       67 2023-05-17 08:56:56.000000 NuOCR-0.2.3/NuOCR/gRPC_proto/nufarm_poc/__init__.py
+-rw-rw-rw-   0        0        0     1617 2023-01-30 11:12:08.000000 NuOCR-0.2.3/NuOCR/gRPC_proto/nufarm_poc/nufarm_poc_pb2.py
+-rw-rw-rw-   0        0        0     4171 2023-05-17 08:56:56.000000 NuOCR-0.2.3/NuOCR/gRPC_proto/nufarm_poc/nufarm_poc_pb2_grpc.py
+drwxrwxrwx   0        0        0        0 2023-05-18 07:56:53.288556 NuOCR-0.2.3/NuOCR/gRPC_proto/preprocessor/
+-rw-rw-rw-   0        0        0       71 2023-05-17 08:56:56.000000 NuOCR-0.2.3/NuOCR/gRPC_proto/preprocessor/__init__.py
+-rw-rw-rw-   0        0        0     4074 2023-05-17 08:12:10.000000 NuOCR-0.2.3/NuOCR/gRPC_proto/preprocessor/preprocessor_pb2.py
+-rw-rw-rw-   0        0        0    13059 2023-05-17 08:56:56.000000 NuOCR-0.2.3/NuOCR/gRPC_proto/preprocessor/preprocessor_pb2_grpc.py
+drwxrwxrwx   0        0        0        0 2023-05-18 07:56:53.314472 NuOCR-0.2.3/NuOCR/gRPC_proto/templated_flow/
+-rw-rw-rw-   0        0        0       75 2023-03-27 09:59:57.000000 NuOCR-0.2.3/NuOCR/gRPC_proto/templated_flow/__init__.py
+-rw-rw-rw-   0        0        0     3375 2023-03-27 10:00:02.000000 NuOCR-0.2.3/NuOCR/gRPC_proto/templated_flow/templated_flow_pb2.py
+-rw-rw-rw-   0        0        0     8097 2023-05-17 08:55:07.000000 NuOCR-0.2.3/NuOCR/gRPC_proto/templated_flow/templated_flow_pb2_grpc.py
+drwxrwxrwx   0        0        0        0 2023-05-18 07:56:53.337203 NuOCR-0.2.3/NuOCR/gRPC_proto/text_processor/
+-rw-rw-rw-   0        0        0       75 2023-03-27 09:59:58.000000 NuOCR-0.2.3/NuOCR/gRPC_proto/text_processor/__init__.py
+-rw-rw-rw-   0        0        0     2413 2023-04-25 06:16:53.000000 NuOCR-0.2.3/NuOCR/gRPC_proto/text_processor/text_processor_pb2.py
+-rw-rw-rw-   0        0        0     8128 2023-05-17 08:56:56.000000 NuOCR-0.2.3/NuOCR/gRPC_proto/text_processor/text_processor_pb2_grpc.py
+drwxrwxrwx   0        0        0        0 2023-05-18 07:56:53.378021 NuOCR-0.2.3/NuOCR/gRPC_proto/user/
+-rw-rw-rw-   0        0        0      110 2023-03-27 09:59:58.000000 NuOCR-0.2.3/NuOCR/gRPC_proto/user/__init__.py
+-rw-rw-rw-   0        0        0     1414 2023-04-25 06:16:53.000000 NuOCR-0.2.3/NuOCR/gRPC_proto/user/auth_pb2.py
+-rw-rw-rw-   0        0        0     2474 2023-05-17 08:55:25.000000 NuOCR-0.2.3/NuOCR/gRPC_proto/user/auth_pb2_grpc.py
+-rw-rw-rw-   0        0        0     4332 2023-03-27 10:00:02.000000 NuOCR-0.2.3/NuOCR/gRPC_proto/user/user_pb2.py
+-rw-rw-rw-   0        0        0    22705 2023-05-17 08:55:31.000000 NuOCR-0.2.3/NuOCR/gRPC_proto/user/user_pb2_grpc.py
+-rw-rw-rw-   0        0        0    15388 2023-05-17 11:23:10.000000 NuOCR-0.2.3/NuOCR/io_adaptor.py
+-rw-rw-rw-   0        0        0     2820 2023-05-17 11:55:52.000000 NuOCR-0.2.3/NuOCR/monitor.py
+-rw-rw-rw-   0        0        0     5896 2023-05-18 07:54:08.000000 NuOCR-0.2.3/NuOCR/preprocessors.py
+-rw-rw-rw-   0        0        0     2732 2023-05-17 11:27:14.000000 NuOCR-0.2.3/NuOCR/templated_flow.py
+-rw-rw-rw-   0        0        0     2052 2023-05-17 11:41:08.000000 NuOCR-0.2.3/NuOCR/text.py
+-rw-rw-rw-   0        0        0     2314 2023-05-17 12:39:27.000000 NuOCR-0.2.3/NuOCR/user.py
+-rw-rw-rw-   0        0        0      334 2023-03-27 09:59:59.000000 NuOCR-0.2.3/NuOCR/util.py
+drwxrwxrwx   0        0        0        0 2023-05-18 07:56:53.158320 NuOCR-0.2.3/NuOCR.egg-info/
+-rw-rw-rw-   0        0        0      538 2023-05-18 07:56:52.000000 NuOCR-0.2.3/NuOCR.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1560 2023-05-18 07:56:52.000000 NuOCR-0.2.3/NuOCR.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-18 07:56:52.000000 NuOCR-0.2.3/NuOCR.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2023-05-18 07:56:52.000000 NuOCR-0.2.3/NuOCR.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-05-18 07:56:52.000000 NuOCR-0.2.3/NuOCR.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      538 2023-05-18 07:56:53.386555 NuOCR-0.2.3/PKG-INFO
+-rw-rw-rw-   0        0        0     4053 2023-03-27 09:59:59.000000 NuOCR-0.2.3/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-18 07:56:53.392330 NuOCR-0.2.3/setup.cfg
+-rw-rw-rw-   0        0        0     1130 2023-05-18 07:56:47.000000 NuOCR-0.2.3/setup.py
```

### Comparing `NuOCR-0.2.2/NuOCR/gRPC_proto/extractor/extractor_pb2.py` & `NuOCR-0.2.3/NuOCR/gRPC_proto/extractor/extractor_pb2.py`

 * *Files identical despite different names*

### Comparing `NuOCR-0.2.2/NuOCR/gRPC_proto/extractor/extractor_pb2_grpc.py` & `NuOCR-0.2.3/NuOCR/gRPC_proto/extractor/extractor_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `NuOCR-0.2.2/NuOCR/gRPC_proto/templated_flow/templated_flow_pb2.py` & `NuOCR-0.2.3/NuOCR/gRPC_proto/templated_flow/templated_flow_pb2.py`

 * *Ordering differences only*

 * *Files 11% similar despite different names*

```diff
@@ -1,42 +1,42 @@
-# -*- coding: utf-8 -*-
-# Generated by the protocol buffer compiler.  DO NOT EDIT!
-# source: templated_flow/templated_flow.proto
-"""Generated protocol buffer code."""
-from google.protobuf.internal import builder as _builder
-from google.protobuf import descriptor as _descriptor
-from google.protobuf import descriptor_pool as _descriptor_pool
-from google.protobuf import symbol_database as _symbol_database
-# @@protoc_insertion_point(imports)
-
-_sym_db = _symbol_database.Default()
-
-
-from google.protobuf import empty_pb2 as google_dot_protobuf_dot_empty__pb2
-
-
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n#templated_flow/templated_flow.proto\x12\x14templated_flow_proto\x1a\x1bgoogle/protobuf/empty.proto\"V\n\x0b\x42oundingBox\x12\r\n\x05label\x18\x01 \x01(\t\x12\t\n\x01x\x18\x02 \x01(\x05\x12\t\n\x01y\x18\x03 \x01(\x05\x12\t\n\x01h\x18\x04 \x01(\x05\x12\t\n\x01w\x18\x05 \x01(\x05\x12\x0c\n\x04page\x18\x06 \x01(\x05\"|\n\x0fTemplateRequest\x12\x14\n\x0c\x64ocumentName\x18\x01 \x01(\t\x12\x0e\n\x06\x62\x61se64\x18\x02 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x03 \x01(\t\x12.\n\x03\x62ox\x18\x04 \x03(\x0b\x32!.templated_flow_proto.BoundingBox\"\x1a\n\x08Response\x12\x0e\n\x06status\x18\x01 \x01(\t\"\x0e\n\x0c\x46\x65tchRequest\"[\n\rFetchResponse\x12\x12\n\ndocumentId\x18\x01 \x01(\x05\x12\x14\n\x0c\x64ocumentName\x18\x02 \x01(\t\x12\x0e\n\x06\x62\x61se64\x18\x03 \x01(\t\x12\x10\n\x08mimeType\x18\x04 \x01(\t\"\x81\x01\n\x0e\x45xtractRequest\x12\x12\n\ndocumentId\x18\x01 \x01(\x05\x12\x14\n\x0c\x64ocumentName\x18\x02 \x01(\t\x12\x10\n\x08\x66ileName\x18\x03 \x01(\t\x12\x0e\n\x06\x62\x61se64\x18\x04 \x01(\t\x12\x12\n\nreadStatus\x18\x05 \x01(\x08\x12\x0f\n\x07rawJson\x18\x06 \x01(\x08\"#\n\x0f\x45xtractResponse\x12\x10\n\x08response\x18\x01 \x01(\t\"9\n\rDeleteRequest\x12\x12\n\ndocumentId\x18\x01 \x01(\x05\x12\x14\n\x0c\x64ocumentName\x18\x02 \x01(\t2\xed\x02\n\x17TemplatedFlowController\x12W\n\x0e\x43reateTemplate\x12%.templated_flow_proto.TemplateRequest\x1a\x1e.templated_flow_proto.Response\x12Z\n\rFetchTemplate\x12\".templated_flow_proto.FetchRequest\x1a#.templated_flow_proto.FetchResponse0\x01\x12V\n\x07\x45xtract\x12$.templated_flow_proto.ExtractRequest\x1a%.templated_flow_proto.ExtractResponse\x12\x45\n\x06\x44\x65lete\x12#.templated_flow_proto.DeleteRequest\x1a\x16.google.protobuf.Emptyb\x06proto3')
-
-_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'templated_flow.templated_flow_pb2', globals())
-if _descriptor._USE_C_DESCRIPTORS == False:
-
-  DESCRIPTOR._options = None
-  _BOUNDINGBOX._serialized_start=90
-  _BOUNDINGBOX._serialized_end=176
-  _TEMPLATEREQUEST._serialized_start=178
-  _TEMPLATEREQUEST._serialized_end=302
-  _RESPONSE._serialized_start=304
-  _RESPONSE._serialized_end=330
-  _FETCHREQUEST._serialized_start=332
-  _FETCHREQUEST._serialized_end=346
-  _FETCHRESPONSE._serialized_start=348
-  _FETCHRESPONSE._serialized_end=439
-  _EXTRACTREQUEST._serialized_start=442
-  _EXTRACTREQUEST._serialized_end=571
-  _EXTRACTRESPONSE._serialized_start=573
-  _EXTRACTRESPONSE._serialized_end=608
-  _DELETEREQUEST._serialized_start=610
-  _DELETEREQUEST._serialized_end=667
-  _TEMPLATEDFLOWCONTROLLER._serialized_start=670
-  _TEMPLATEDFLOWCONTROLLER._serialized_end=1035
-# @@protoc_insertion_point(module_scope)
+# -*- coding: utf-8 -*-
+# Generated by the protocol buffer compiler.  DO NOT EDIT!
+# source: templated_flow/templated_flow.proto
+"""Generated protocol buffer code."""
+from google.protobuf.internal import builder as _builder
+from google.protobuf import descriptor as _descriptor
+from google.protobuf import descriptor_pool as _descriptor_pool
+from google.protobuf import symbol_database as _symbol_database
+# @@protoc_insertion_point(imports)
+
+_sym_db = _symbol_database.Default()
+
+
+from google.protobuf import empty_pb2 as google_dot_protobuf_dot_empty__pb2
+
+
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n#templated_flow/templated_flow.proto\x12\x14templated_flow_proto\x1a\x1bgoogle/protobuf/empty.proto\"V\n\x0b\x42oundingBox\x12\r\n\x05label\x18\x01 \x01(\t\x12\t\n\x01x\x18\x02 \x01(\x05\x12\t\n\x01y\x18\x03 \x01(\x05\x12\t\n\x01h\x18\x04 \x01(\x05\x12\t\n\x01w\x18\x05 \x01(\x05\x12\x0c\n\x04page\x18\x06 \x01(\x05\"|\n\x0fTemplateRequest\x12\x14\n\x0c\x64ocumentName\x18\x01 \x01(\t\x12\x0e\n\x06\x62\x61se64\x18\x02 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x03 \x01(\t\x12.\n\x03\x62ox\x18\x04 \x03(\x0b\x32!.templated_flow_proto.BoundingBox\"\x1a\n\x08Response\x12\x0e\n\x06status\x18\x01 \x01(\t\"\x0e\n\x0c\x46\x65tchRequest\"[\n\rFetchResponse\x12\x12\n\ndocumentId\x18\x01 \x01(\x05\x12\x14\n\x0c\x64ocumentName\x18\x02 \x01(\t\x12\x0e\n\x06\x62\x61se64\x18\x03 \x01(\t\x12\x10\n\x08mimeType\x18\x04 \x01(\t\"\x81\x01\n\x0e\x45xtractRequest\x12\x12\n\ndocumentId\x18\x01 \x01(\x05\x12\x14\n\x0c\x64ocumentName\x18\x02 \x01(\t\x12\x10\n\x08\x66ileName\x18\x03 \x01(\t\x12\x0e\n\x06\x62\x61se64\x18\x04 \x01(\t\x12\x12\n\nreadStatus\x18\x05 \x01(\x08\x12\x0f\n\x07rawJson\x18\x06 \x01(\x08\"#\n\x0f\x45xtractResponse\x12\x10\n\x08response\x18\x01 \x01(\t\"9\n\rDeleteRequest\x12\x12\n\ndocumentId\x18\x01 \x01(\x05\x12\x14\n\x0c\x64ocumentName\x18\x02 \x01(\t2\xed\x02\n\x17TemplatedFlowController\x12W\n\x0e\x43reateTemplate\x12%.templated_flow_proto.TemplateRequest\x1a\x1e.templated_flow_proto.Response\x12Z\n\rFetchTemplate\x12\".templated_flow_proto.FetchRequest\x1a#.templated_flow_proto.FetchResponse0\x01\x12V\n\x07\x45xtract\x12$.templated_flow_proto.ExtractRequest\x1a%.templated_flow_proto.ExtractResponse\x12\x45\n\x06\x44\x65lete\x12#.templated_flow_proto.DeleteRequest\x1a\x16.google.protobuf.Emptyb\x06proto3')
+
+_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'templated_flow.templated_flow_pb2', globals())
+if _descriptor._USE_C_DESCRIPTORS == False:
+
+  DESCRIPTOR._options = None
+  _BOUNDINGBOX._serialized_start=90
+  _BOUNDINGBOX._serialized_end=176
+  _TEMPLATEREQUEST._serialized_start=178
+  _TEMPLATEREQUEST._serialized_end=302
+  _RESPONSE._serialized_start=304
+  _RESPONSE._serialized_end=330
+  _FETCHREQUEST._serialized_start=332
+  _FETCHREQUEST._serialized_end=346
+  _FETCHRESPONSE._serialized_start=348
+  _FETCHRESPONSE._serialized_end=439
+  _EXTRACTREQUEST._serialized_start=442
+  _EXTRACTREQUEST._serialized_end=571
+  _EXTRACTRESPONSE._serialized_start=573
+  _EXTRACTRESPONSE._serialized_end=608
+  _DELETEREQUEST._serialized_start=610
+  _DELETEREQUEST._serialized_end=667
+  _TEMPLATEDFLOWCONTROLLER._serialized_start=670
+  _TEMPLATEDFLOWCONTROLLER._serialized_end=1035
+# @@protoc_insertion_point(module_scope)
```

### Comparing `NuOCR-0.2.2/NuOCR/gRPC_proto/templated_flow/templated_flow_pb2_grpc.py` & `NuOCR-0.2.3/NuOCR/gRPC_proto/templated_flow/templated_flow_pb2_grpc.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,166 +1,166 @@
-# Generated by the gRPC Python protocol compiler plugin. DO NOT EDIT!
-"""Client and server classes corresponding to protobuf-defined services."""
-import grpc
-
-from google.protobuf import empty_pb2 as google_dot_protobuf_dot_empty__pb2
-from ..templated_flow import templated_flow_pb2 as templated__flow_dot_templated__flow__pb2
-
-
-class TemplatedFlowControllerStub(object):
-    """Missing associated documentation comment in .proto file."""
-
-    def __init__(self, channel):
-        """Constructor.
-
-        Args:
-            channel: A grpc.Channel.
-        """
-        self.CreateTemplate = channel.unary_unary(
-                '/templated_flow_proto.TemplatedFlowController/CreateTemplate',
-                request_serializer=templated__flow_dot_templated__flow__pb2.TemplateRequest.SerializeToString,
-                response_deserializer=templated__flow_dot_templated__flow__pb2.Response.FromString,
-                )
-        self.FetchTemplate = channel.unary_stream(
-                '/templated_flow_proto.TemplatedFlowController/FetchTemplate',
-                request_serializer=templated__flow_dot_templated__flow__pb2.FetchRequest.SerializeToString,
-                response_deserializer=templated__flow_dot_templated__flow__pb2.FetchResponse.FromString,
-                )
-        self.Extract = channel.unary_unary(
-                '/templated_flow_proto.TemplatedFlowController/Extract',
-                request_serializer=templated__flow_dot_templated__flow__pb2.ExtractRequest.SerializeToString,
-                response_deserializer=templated__flow_dot_templated__flow__pb2.ExtractResponse.FromString,
-                )
-        self.Delete = channel.unary_unary(
-                '/templated_flow_proto.TemplatedFlowController/Delete',
-                request_serializer=templated__flow_dot_templated__flow__pb2.DeleteRequest.SerializeToString,
-                response_deserializer=google_dot_protobuf_dot_empty__pb2.Empty.FromString,
-                )
-
-
-class TemplatedFlowControllerServicer(object):
-    """Missing associated documentation comment in .proto file."""
-
-    def CreateTemplate(self, request, context):
-        """Missing associated documentation comment in .proto file."""
-        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
-        context.set_details('Method not implemented!')
-        raise NotImplementedError('Method not implemented!')
-
-    def FetchTemplate(self, request, context):
-        """Missing associated documentation comment in .proto file."""
-        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
-        context.set_details('Method not implemented!')
-        raise NotImplementedError('Method not implemented!')
-
-    def Extract(self, request, context):
-        """Missing associated documentation comment in .proto file."""
-        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
-        context.set_details('Method not implemented!')
-        raise NotImplementedError('Method not implemented!')
-
-    def Delete(self, request, context):
-        """Missing associated documentation comment in .proto file."""
-        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
-        context.set_details('Method not implemented!')
-        raise NotImplementedError('Method not implemented!')
-
-
-def add_TemplatedFlowControllerServicer_to_server(servicer, server):
-    rpc_method_handlers = {
-            'CreateTemplate': grpc.unary_unary_rpc_method_handler(
-                    servicer.CreateTemplate,
-                    request_deserializer=templated__flow_dot_templated__flow__pb2.TemplateRequest.FromString,
-                    response_serializer=templated__flow_dot_templated__flow__pb2.Response.SerializeToString,
-            ),
-            'FetchTemplate': grpc.unary_stream_rpc_method_handler(
-                    servicer.FetchTemplate,
-                    request_deserializer=templated__flow_dot_templated__flow__pb2.FetchRequest.FromString,
-                    response_serializer=templated__flow_dot_templated__flow__pb2.FetchResponse.SerializeToString,
-            ),
-            'Extract': grpc.unary_unary_rpc_method_handler(
-                    servicer.Extract,
-                    request_deserializer=templated__flow_dot_templated__flow__pb2.ExtractRequest.FromString,
-                    response_serializer=templated__flow_dot_templated__flow__pb2.ExtractResponse.SerializeToString,
-            ),
-            'Delete': grpc.unary_unary_rpc_method_handler(
-                    servicer.Delete,
-                    request_deserializer=templated__flow_dot_templated__flow__pb2.DeleteRequest.FromString,
-                    response_serializer=google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
-            ),
-    }
-    generic_handler = grpc.method_handlers_generic_handler(
-            'templated_flow_proto.TemplatedFlowController', rpc_method_handlers)
-    server.add_generic_rpc_handlers((generic_handler,))
-
-
- # This class is part of an EXPERIMENTAL API.
-class TemplatedFlowController(object):
-    """Missing associated documentation comment in .proto file."""
-
-    @staticmethod
-    def CreateTemplate(request,
-            target,
-            options=(),
-            channel_credentials=None,
-            call_credentials=None,
-            insecure=False,
-            compression=None,
-            wait_for_ready=None,
-            timeout=None,
-            metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/templated_flow_proto.TemplatedFlowController/CreateTemplate',
-            templated__flow_dot_templated__flow__pb2.TemplateRequest.SerializeToString,
-            templated__flow_dot_templated__flow__pb2.Response.FromString,
-            options, channel_credentials,
-            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
-
-    @staticmethod
-    def FetchTemplate(request,
-            target,
-            options=(),
-            channel_credentials=None,
-            call_credentials=None,
-            insecure=False,
-            compression=None,
-            wait_for_ready=None,
-            timeout=None,
-            metadata=None):
-        return grpc.experimental.unary_stream(request, target, '/templated_flow_proto.TemplatedFlowController/FetchTemplate',
-            templated__flow_dot_templated__flow__pb2.FetchRequest.SerializeToString,
-            templated__flow_dot_templated__flow__pb2.FetchResponse.FromString,
-            options, channel_credentials,
-            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
-
-    @staticmethod
-    def Extract(request,
-            target,
-            options=(),
-            channel_credentials=None,
-            call_credentials=None,
-            insecure=False,
-            compression=None,
-            wait_for_ready=None,
-            timeout=None,
-            metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/templated_flow_proto.TemplatedFlowController/Extract',
-            templated__flow_dot_templated__flow__pb2.ExtractRequest.SerializeToString,
-            templated__flow_dot_templated__flow__pb2.ExtractResponse.FromString,
-            options, channel_credentials,
-            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
-
-    @staticmethod
-    def Delete(request,
-            target,
-            options=(),
-            channel_credentials=None,
-            call_credentials=None,
-            insecure=False,
-            compression=None,
-            wait_for_ready=None,
-            timeout=None,
-            metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/templated_flow_proto.TemplatedFlowController/Delete',
-            templated__flow_dot_templated__flow__pb2.DeleteRequest.SerializeToString,
-            google_dot_protobuf_dot_empty__pb2.Empty.FromString,
-            options, channel_credentials,
-            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+# Generated by the gRPC Python protocol compiler plugin. DO NOT EDIT!
+"""Client and server classes corresponding to protobuf-defined services."""
+import grpc
+
+from google.protobuf import empty_pb2 as google_dot_protobuf_dot_empty__pb2
+from ..templated_flow import templated_flow_pb2 as templated__flow_dot_templated__flow__pb2
+
+
+class TemplatedFlowControllerStub(object):
+    """Missing associated documentation comment in .proto file."""
+
+    def __init__(self, channel):
+        """Constructor.
+
+        Args:
+            channel: A grpc.Channel.
+        """
+        self.CreateTemplate = channel.unary_unary(
+                '/templated_flow_proto.TemplatedFlowController/CreateTemplate',
+                request_serializer=templated__flow_dot_templated__flow__pb2.TemplateRequest.SerializeToString,
+                response_deserializer=templated__flow_dot_templated__flow__pb2.Response.FromString,
+                )
+        self.FetchTemplate = channel.unary_stream(
+                '/templated_flow_proto.TemplatedFlowController/FetchTemplate',
+                request_serializer=templated__flow_dot_templated__flow__pb2.FetchRequest.SerializeToString,
+                response_deserializer=templated__flow_dot_templated__flow__pb2.FetchResponse.FromString,
+                )
+        self.Extract = channel.unary_unary(
+                '/templated_flow_proto.TemplatedFlowController/Extract',
+                request_serializer=templated__flow_dot_templated__flow__pb2.ExtractRequest.SerializeToString,
+                response_deserializer=templated__flow_dot_templated__flow__pb2.ExtractResponse.FromString,
+                )
+        self.Delete = channel.unary_unary(
+                '/templated_flow_proto.TemplatedFlowController/Delete',
+                request_serializer=templated__flow_dot_templated__flow__pb2.DeleteRequest.SerializeToString,
+                response_deserializer=google_dot_protobuf_dot_empty__pb2.Empty.FromString,
+                )
+
+
+class TemplatedFlowControllerServicer(object):
+    """Missing associated documentation comment in .proto file."""
+
+    def CreateTemplate(self, request, context):
+        """Missing associated documentation comment in .proto file."""
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
+    def FetchTemplate(self, request, context):
+        """Missing associated documentation comment in .proto file."""
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
+    def Extract(self, request, context):
+        """Missing associated documentation comment in .proto file."""
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
+    def Delete(self, request, context):
+        """Missing associated documentation comment in .proto file."""
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
+
+def add_TemplatedFlowControllerServicer_to_server(servicer, server):
+    rpc_method_handlers = {
+            'CreateTemplate': grpc.unary_unary_rpc_method_handler(
+                    servicer.CreateTemplate,
+                    request_deserializer=templated__flow_dot_templated__flow__pb2.TemplateRequest.FromString,
+                    response_serializer=templated__flow_dot_templated__flow__pb2.Response.SerializeToString,
+            ),
+            'FetchTemplate': grpc.unary_stream_rpc_method_handler(
+                    servicer.FetchTemplate,
+                    request_deserializer=templated__flow_dot_templated__flow__pb2.FetchRequest.FromString,
+                    response_serializer=templated__flow_dot_templated__flow__pb2.FetchResponse.SerializeToString,
+            ),
+            'Extract': grpc.unary_unary_rpc_method_handler(
+                    servicer.Extract,
+                    request_deserializer=templated__flow_dot_templated__flow__pb2.ExtractRequest.FromString,
+                    response_serializer=templated__flow_dot_templated__flow__pb2.ExtractResponse.SerializeToString,
+            ),
+            'Delete': grpc.unary_unary_rpc_method_handler(
+                    servicer.Delete,
+                    request_deserializer=templated__flow_dot_templated__flow__pb2.DeleteRequest.FromString,
+                    response_serializer=google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
+            ),
+    }
+    generic_handler = grpc.method_handlers_generic_handler(
+            'templated_flow_proto.TemplatedFlowController', rpc_method_handlers)
+    server.add_generic_rpc_handlers((generic_handler,))
+
+
+ # This class is part of an EXPERIMENTAL API.
+class TemplatedFlowController(object):
+    """Missing associated documentation comment in .proto file."""
+
+    @staticmethod
+    def CreateTemplate(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/templated_flow_proto.TemplatedFlowController/CreateTemplate',
+            templated__flow_dot_templated__flow__pb2.TemplateRequest.SerializeToString,
+            templated__flow_dot_templated__flow__pb2.Response.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
+    def FetchTemplate(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_stream(request, target, '/templated_flow_proto.TemplatedFlowController/FetchTemplate',
+            templated__flow_dot_templated__flow__pb2.FetchRequest.SerializeToString,
+            templated__flow_dot_templated__flow__pb2.FetchResponse.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
+    def Extract(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/templated_flow_proto.TemplatedFlowController/Extract',
+            templated__flow_dot_templated__flow__pb2.ExtractRequest.SerializeToString,
+            templated__flow_dot_templated__flow__pb2.ExtractResponse.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
+    def Delete(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/templated_flow_proto.TemplatedFlowController/Delete',
+            templated__flow_dot_templated__flow__pb2.DeleteRequest.SerializeToString,
+            google_dot_protobuf_dot_empty__pb2.Empty.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
```

### Comparing `NuOCR-0.2.2/NuOCR/gRPC_proto/text_processor/text_processor_pb2.py` & `NuOCR-0.2.3/NuOCR/gRPC_proto/text_processor/text_processor_pb2.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,29 +1,36 @@
-# -*- coding: utf-8 -*-
-# Generated by the protocol buffer compiler.  DO NOT EDIT!
-# source: text_processor/text_processor.proto
-"""Generated protocol buffer code."""
-from google.protobuf.internal import builder as _builder
-from google.protobuf import descriptor as _descriptor
-from google.protobuf import descriptor_pool as _descriptor_pool
-from google.protobuf import symbol_database as _symbol_database
-# @@protoc_insertion_point(imports)
-
-_sym_db = _symbol_database.Default()
-
-
-
-
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n#text_processor/text_processor.proto\x12\x14text_processor_proto\"\x17\n\x07Request\x12\x0c\n\x04text\x18\x01 \x01(\t\"\x1b\n\x08Response\x12\x0f\n\x07summary\x18\x01 \x01(\t2\xb9\x01\n\x17TextProcessorController\x12J\n\tSummarize\x12\x1d.text_processor_proto.Request\x1a\x1e.text_processor_proto.Response\x12R\n\x11SentimentAnalysis\x12\x1d.text_processor_proto.Request\x1a\x1e.text_processor_proto.Responseb\x06proto3')
-
-_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'text_processor.text_processor_pb2', globals())
-if _descriptor._USE_C_DESCRIPTORS == False:
-
-  DESCRIPTOR._options = None
-  _REQUEST._serialized_start=61
-  _REQUEST._serialized_end=84
-  _RESPONSE._serialized_start=86
-  _RESPONSE._serialized_end=113
-  _TEXTPROCESSORCONTROLLER._serialized_start=116
-  _TEXTPROCESSORCONTROLLER._serialized_end=301
-# @@protoc_insertion_point(module_scope)
+# -*- coding: utf-8 -*-
+# Generated by the protocol buffer compiler.  DO NOT EDIT!
+# source: text_processor/text_processor.proto
+"""Generated protocol buffer code."""
+from google.protobuf.internal import builder as _builder
+from google.protobuf import descriptor as _descriptor
+from google.protobuf import descriptor_pool as _descriptor_pool
+from google.protobuf import symbol_database as _symbol_database
+# @@protoc_insertion_point(imports)
+
+_sym_db = _symbol_database.Default()
+
+
+from google.protobuf import empty_pb2 as google_dot_protobuf_dot_empty__pb2
+
+
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n#text_processor/text_processor.proto\x12\x14text_processor_proto\x1a\x1bgoogle/protobuf/empty.proto\"\x17\n\x07Request\x12\x0c\n\x04text\x18\x01 \x01(\t\"\x1b\n\x08Response\x12\x0f\n\x07summary\x18\x01 \x01(\t\"0\n\rSearchRequest\x12\x10\n\x08question\x18\x01 \x01(\t\x12\r\n\x05top_k\x18\x02 \x01(\x05\"K\n\x0eSearchResponse\x12\x12\n\nconfidence\x18\x01 \x01(\x02\x12\x13\n\x0bpage_number\x18\x02 \x01(\x05\x12\x10\n\x08\x66ilename\x18\x03 \x01(\t\"*\n\x06Upload\x12\x10\n\x08\x66ilename\x18\x01 \x01(\t\x12\x0e\n\x06\x62\x61se64\x18\x02 \x01(\t2\xea\x02\n\x17TextProcessorController\x12L\n\tSummarize\x12\x1d.text_processor_proto.Request\x1a\x1e.text_processor_proto.Response\"\x00\x12T\n\x11SentimentAnalysis\x12\x1d.text_processor_proto.Request\x1a\x1e.text_processor_proto.Response\"\x00\x12I\n\x0f\x43ognitiveUpload\x12\x1c.text_processor_proto.Upload\x1a\x16.google.protobuf.Empty\"\x00\x12`\n\x0f\x43ognitiveSearch\x12#.text_processor_proto.SearchRequest\x1a$.text_processor_proto.SearchResponse\"\x00\x30\x01\x62\x06proto3')
+
+_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'text_processor.text_processor_pb2', globals())
+if _descriptor._USE_C_DESCRIPTORS == False:
+
+  DESCRIPTOR._options = None
+  _REQUEST._serialized_start=90
+  _REQUEST._serialized_end=113
+  _RESPONSE._serialized_start=115
+  _RESPONSE._serialized_end=142
+  _SEARCHREQUEST._serialized_start=144
+  _SEARCHREQUEST._serialized_end=192
+  _SEARCHRESPONSE._serialized_start=194
+  _SEARCHRESPONSE._serialized_end=269
+  _UPLOAD._serialized_start=271
+  _UPLOAD._serialized_end=313
+  _TEXTPROCESSORCONTROLLER._serialized_start=316
+  _TEXTPROCESSORCONTROLLER._serialized_end=678
+# @@protoc_insertion_point(module_scope)
```

### Comparing `NuOCR-0.2.2/NuOCR/gRPC_proto/user/auth_pb2_grpc.py` & `NuOCR-0.2.3/NuOCR/gRPC_proto/user/auth_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `NuOCR-0.2.2/NuOCR/gRPC_proto/user/user_pb2.py` & `NuOCR-0.2.3/NuOCR/gRPC_proto/user/user_pb2.py`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,46 +1,46 @@
-# -*- coding: utf-8 -*-
-# Generated by the protocol buffer compiler.  DO NOT EDIT!
-# source: user/user.proto
-"""Generated protocol buffer code."""
-from google.protobuf.internal import builder as _builder
-from google.protobuf import descriptor as _descriptor
-from google.protobuf import descriptor_pool as _descriptor_pool
-from google.protobuf import symbol_database as _symbol_database
-# @@protoc_insertion_point(imports)
-
-_sym_db = _symbol_database.Default()
-
-
-from google.protobuf import empty_pb2 as google_dot_protobuf_dot_empty__pb2
-
-
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x0fuser/user.proto\x12\nuser_proto\x1a\x1bgoogle/protobuf/empty.proto\"\x87\x02\n\x04User\x12\n\n\x02id\x18\x01 \x01(\x03\x12\x10\n\x08password\x18\x02 \x01(\t\x12\x12\n\nlast_login\x18\x03 \x01(\t\x12\x14\n\x0cis_superuser\x18\x04 \x01(\x08\x12\x10\n\x08username\x18\x05 \x01(\t\x12\x12\n\nfirst_name\x18\x06 \x01(\t\x12\x11\n\tlast_name\x18\x07 \x01(\t\x12\r\n\x05\x65mail\x18\x08 \x01(\t\x12\x10\n\x08is_staff\x18\t \x01(\x08\x12\x11\n\tis_active\x18\n \x01(\x08\x12\x13\n\x0b\x64\x61te_joined\x18\x0b \x01(\t\x12\x0e\n\x06groups\x18\x0c \x03(\x05\x12\x18\n\x10user_permissions\x18\r \x03(\x05\x12\x0b\n\x03key\x18\x0e \x01(\t\"\x11\n\x0fUserListRequest\"!\n\x13UserRetrieveRequest\x12\n\n\x02id\x18\x01 \x01(\x03\"/\n\x0bUserRequest\x12\x10\n\x08username\x18\x01 \x01(\t\x12\x0e\n\x06\x61\x63\x63\x65ss\x18\x02 \x01(\t\"K\n\x0fPasswordRequest\x12\x10\n\x08username\x18\x01 \x01(\t\x12\x10\n\x08password\x18\x02 \x01(\t\x12\x14\n\x0cnew_password\x18\x03 \x01(\t\"0\n\nKeyRequest\x12\x10\n\x08username\x18\x01 \x01(\t\x12\x10\n\x08password\x18\x02 \x01(\t\"\x0e\n\x0cTokenRequest\".\n\rTokenResponse\x12\r\n\x05valid\x18\x01 \x01(\x08\x12\x0e\n\x06remark\x18\x02 \x01(\t\"\x1e\n\x0c\x44ropResponse\x12\x0e\n\x06option\x18\x01 \x03(\t\"/\n\x0b\x44ropRequest\x12\x10\n\x08username\x18\x01 \x01(\t\x12\x0e\n\x06option\x18\x02 \x01(\t2\xdb\x06\n\x0eUserController\x12\x39\n\x04List\x12\x1b.user_proto.UserListRequest\x1a\x10.user_proto.User\"\x00\x30\x01\x12.\n\x06\x43reate\x12\x10.user_proto.User\x1a\x10.user_proto.User\"\x00\x12?\n\x08Retrieve\x12\x1f.user_proto.UserRetrieveRequest\x1a\x10.user_proto.User\"\x00\x12.\n\x06Update\x12\x10.user_proto.User\x1a\x10.user_proto.User\"\x00\x12\x38\n\tAddAccess\x12\x17.user_proto.UserRequest\x1a\x10.user_proto.User\"\x00\x12;\n\x0cRemoveAccess\x12\x17.user_proto.UserRequest\x1a\x10.user_proto.User\"\x00\x12\x35\n\x07\x44\x65stroy\x12\x10.user_proto.User\x1a\x16.google.protobuf.Empty\"\x00\x12\x41\n\x0e\x43hangePassword\x12\x1b.user_proto.PasswordRequest\x1a\x10.user_proto.User\"\x00\x12\x37\n\tChangeKey\x12\x16.user_proto.KeyRequest\x1a\x10.user_proto.User\"\x00\x12\x34\n\x06GetKey\x12\x16.user_proto.KeyRequest\x1a\x10.user_proto.User\"\x00\x12\x41\n\x08\x43heckJWT\x12\x18.user_proto.TokenRequest\x1a\x19.user_proto.TokenResponse\"\x00\x12\x43\n\x08\x44ropDown\x12\x1b.user_proto.UserListRequest\x1a\x18.user_proto.DropResponse\"\x00\x12@\n\x0b\x41\x64\x64\x44ropDown\x12\x17.user_proto.DropRequest\x1a\x16.google.protobuf.Empty\"\x00\x12\x43\n\x0eRemoveDropDown\x12\x17.user_proto.DropRequest\x1a\x16.google.protobuf.Empty\"\x00\x62\x06proto3')
-
-_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'user.user_pb2', globals())
-if _descriptor._USE_C_DESCRIPTORS == False:
-
-  DESCRIPTOR._options = None
-  _USER._serialized_start=61
-  _USER._serialized_end=324
-  _USERLISTREQUEST._serialized_start=326
-  _USERLISTREQUEST._serialized_end=343
-  _USERRETRIEVEREQUEST._serialized_start=345
-  _USERRETRIEVEREQUEST._serialized_end=378
-  _USERREQUEST._serialized_start=380
-  _USERREQUEST._serialized_end=427
-  _PASSWORDREQUEST._serialized_start=429
-  _PASSWORDREQUEST._serialized_end=504
-  _KEYREQUEST._serialized_start=506
-  _KEYREQUEST._serialized_end=554
-  _TOKENREQUEST._serialized_start=556
-  _TOKENREQUEST._serialized_end=570
-  _TOKENRESPONSE._serialized_start=572
-  _TOKENRESPONSE._serialized_end=618
-  _DROPRESPONSE._serialized_start=620
-  _DROPRESPONSE._serialized_end=650
-  _DROPREQUEST._serialized_start=652
-  _DROPREQUEST._serialized_end=699
-  _USERCONTROLLER._serialized_start=702
-  _USERCONTROLLER._serialized_end=1561
-# @@protoc_insertion_point(module_scope)
+# -*- coding: utf-8 -*-
+# Generated by the protocol buffer compiler.  DO NOT EDIT!
+# source: user/user.proto
+"""Generated protocol buffer code."""
+from google.protobuf.internal import builder as _builder
+from google.protobuf import descriptor as _descriptor
+from google.protobuf import descriptor_pool as _descriptor_pool
+from google.protobuf import symbol_database as _symbol_database
+# @@protoc_insertion_point(imports)
+
+_sym_db = _symbol_database.Default()
+
+
+from google.protobuf import empty_pb2 as google_dot_protobuf_dot_empty__pb2
+
+
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x0fuser/user.proto\x12\nuser_proto\x1a\x1bgoogle/protobuf/empty.proto\"\x87\x02\n\x04User\x12\n\n\x02id\x18\x01 \x01(\x03\x12\x10\n\x08password\x18\x02 \x01(\t\x12\x12\n\nlast_login\x18\x03 \x01(\t\x12\x14\n\x0cis_superuser\x18\x04 \x01(\x08\x12\x10\n\x08username\x18\x05 \x01(\t\x12\x12\n\nfirst_name\x18\x06 \x01(\t\x12\x11\n\tlast_name\x18\x07 \x01(\t\x12\r\n\x05\x65mail\x18\x08 \x01(\t\x12\x10\n\x08is_staff\x18\t \x01(\x08\x12\x11\n\tis_active\x18\n \x01(\x08\x12\x13\n\x0b\x64\x61te_joined\x18\x0b \x01(\t\x12\x0e\n\x06groups\x18\x0c \x03(\x05\x12\x18\n\x10user_permissions\x18\r \x03(\x05\x12\x0b\n\x03key\x18\x0e \x01(\t\"\x11\n\x0fUserListRequest\"!\n\x13UserRetrieveRequest\x12\n\n\x02id\x18\x01 \x01(\x03\"/\n\x0bUserRequest\x12\x10\n\x08username\x18\x01 \x01(\t\x12\x0e\n\x06\x61\x63\x63\x65ss\x18\x02 \x01(\t\"K\n\x0fPasswordRequest\x12\x10\n\x08username\x18\x01 \x01(\t\x12\x10\n\x08password\x18\x02 \x01(\t\x12\x14\n\x0cnew_password\x18\x03 \x01(\t\"0\n\nKeyRequest\x12\x10\n\x08username\x18\x01 \x01(\t\x12\x10\n\x08password\x18\x02 \x01(\t\"\x0e\n\x0cTokenRequest\".\n\rTokenResponse\x12\r\n\x05valid\x18\x01 \x01(\x08\x12\x0e\n\x06remark\x18\x02 \x01(\t\"\x1e\n\x0c\x44ropResponse\x12\x0e\n\x06option\x18\x01 \x03(\t\"/\n\x0b\x44ropRequest\x12\x10\n\x08username\x18\x01 \x01(\t\x12\x0e\n\x06option\x18\x02 \x01(\t2\xdb\x06\n\x0eUserController\x12\x39\n\x04List\x12\x1b.user_proto.UserListRequest\x1a\x10.user_proto.User\"\x00\x30\x01\x12.\n\x06\x43reate\x12\x10.user_proto.User\x1a\x10.user_proto.User\"\x00\x12?\n\x08Retrieve\x12\x1f.user_proto.UserRetrieveRequest\x1a\x10.user_proto.User\"\x00\x12.\n\x06Update\x12\x10.user_proto.User\x1a\x10.user_proto.User\"\x00\x12\x38\n\tAddAccess\x12\x17.user_proto.UserRequest\x1a\x10.user_proto.User\"\x00\x12;\n\x0cRemoveAccess\x12\x17.user_proto.UserRequest\x1a\x10.user_proto.User\"\x00\x12\x35\n\x07\x44\x65stroy\x12\x10.user_proto.User\x1a\x16.google.protobuf.Empty\"\x00\x12\x41\n\x0e\x43hangePassword\x12\x1b.user_proto.PasswordRequest\x1a\x10.user_proto.User\"\x00\x12\x37\n\tChangeKey\x12\x16.user_proto.KeyRequest\x1a\x10.user_proto.User\"\x00\x12\x34\n\x06GetKey\x12\x16.user_proto.KeyRequest\x1a\x10.user_proto.User\"\x00\x12\x41\n\x08\x43heckJWT\x12\x18.user_proto.TokenRequest\x1a\x19.user_proto.TokenResponse\"\x00\x12\x43\n\x08\x44ropDown\x12\x1b.user_proto.UserListRequest\x1a\x18.user_proto.DropResponse\"\x00\x12@\n\x0b\x41\x64\x64\x44ropDown\x12\x17.user_proto.DropRequest\x1a\x16.google.protobuf.Empty\"\x00\x12\x43\n\x0eRemoveDropDown\x12\x17.user_proto.DropRequest\x1a\x16.google.protobuf.Empty\"\x00\x62\x06proto3')
+
+_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'user.user_pb2', globals())
+if _descriptor._USE_C_DESCRIPTORS == False:
+
+  DESCRIPTOR._options = None
+  _USER._serialized_start=61
+  _USER._serialized_end=324
+  _USERLISTREQUEST._serialized_start=326
+  _USERLISTREQUEST._serialized_end=343
+  _USERRETRIEVEREQUEST._serialized_start=345
+  _USERRETRIEVEREQUEST._serialized_end=378
+  _USERREQUEST._serialized_start=380
+  _USERREQUEST._serialized_end=427
+  _PASSWORDREQUEST._serialized_start=429
+  _PASSWORDREQUEST._serialized_end=504
+  _KEYREQUEST._serialized_start=506
+  _KEYREQUEST._serialized_end=554
+  _TOKENREQUEST._serialized_start=556
+  _TOKENREQUEST._serialized_end=570
+  _TOKENRESPONSE._serialized_start=572
+  _TOKENRESPONSE._serialized_end=618
+  _DROPRESPONSE._serialized_start=620
+  _DROPRESPONSE._serialized_end=650
+  _DROPREQUEST._serialized_start=652
+  _DROPREQUEST._serialized_end=699
+  _USERCONTROLLER._serialized_start=702
+  _USERCONTROLLER._serialized_end=1561
+# @@protoc_insertion_point(module_scope)
```

### Comparing `NuOCR-0.2.2/NuOCR/gRPC_proto/user/user_pb2_grpc.py` & `NuOCR-0.2.3/NuOCR/gRPC_proto/user/user_pb2_grpc.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,496 +1,496 @@
-# Generated by the gRPC Python protocol compiler plugin. DO NOT EDIT!
-"""Client and server classes corresponding to protobuf-defined services."""
-import grpc
-
-from google.protobuf import empty_pb2 as google_dot_protobuf_dot_empty__pb2
-from ..user import user_pb2 as user_dot_user__pb2
-
-
-class UserControllerStub(object):
-    """Missing associated documentation comment in .proto file."""
-
-    def __init__(self, channel):
-        """Constructor.
-
-        Args:
-            channel: A grpc.Channel.
-        """
-        self.List = channel.unary_stream(
-                '/user_proto.UserController/List',
-                request_serializer=user_dot_user__pb2.UserListRequest.SerializeToString,
-                response_deserializer=user_dot_user__pb2.User.FromString,
-                )
-        self.Create = channel.unary_unary(
-                '/user_proto.UserController/Create',
-                request_serializer=user_dot_user__pb2.User.SerializeToString,
-                response_deserializer=user_dot_user__pb2.User.FromString,
-                )
-        self.Retrieve = channel.unary_unary(
-                '/user_proto.UserController/Retrieve',
-                request_serializer=user_dot_user__pb2.UserRetrieveRequest.SerializeToString,
-                response_deserializer=user_dot_user__pb2.User.FromString,
-                )
-        self.Update = channel.unary_unary(
-                '/user_proto.UserController/Update',
-                request_serializer=user_dot_user__pb2.User.SerializeToString,
-                response_deserializer=user_dot_user__pb2.User.FromString,
-                )
-        self.AddAccess = channel.unary_unary(
-                '/user_proto.UserController/AddAccess',
-                request_serializer=user_dot_user__pb2.UserRequest.SerializeToString,
-                response_deserializer=user_dot_user__pb2.User.FromString,
-                )
-        self.RemoveAccess = channel.unary_unary(
-                '/user_proto.UserController/RemoveAccess',
-                request_serializer=user_dot_user__pb2.UserRequest.SerializeToString,
-                response_deserializer=user_dot_user__pb2.User.FromString,
-                )
-        self.Destroy = channel.unary_unary(
-                '/user_proto.UserController/Destroy',
-                request_serializer=user_dot_user__pb2.User.SerializeToString,
-                response_deserializer=google_dot_protobuf_dot_empty__pb2.Empty.FromString,
-                )
-        self.ChangePassword = channel.unary_unary(
-                '/user_proto.UserController/ChangePassword',
-                request_serializer=user_dot_user__pb2.PasswordRequest.SerializeToString,
-                response_deserializer=user_dot_user__pb2.User.FromString,
-                )
-        self.ChangeKey = channel.unary_unary(
-                '/user_proto.UserController/ChangeKey',
-                request_serializer=user_dot_user__pb2.KeyRequest.SerializeToString,
-                response_deserializer=user_dot_user__pb2.User.FromString,
-                )
-        self.GetKey = channel.unary_unary(
-                '/user_proto.UserController/GetKey',
-                request_serializer=user_dot_user__pb2.KeyRequest.SerializeToString,
-                response_deserializer=user_dot_user__pb2.User.FromString,
-                )
-        self.CheckJWT = channel.unary_unary(
-                '/user_proto.UserController/CheckJWT',
-                request_serializer=user_dot_user__pb2.TokenRequest.SerializeToString,
-                response_deserializer=user_dot_user__pb2.TokenResponse.FromString,
-                )
-        self.DropDown = channel.unary_unary(
-                '/user_proto.UserController/DropDown',
-                request_serializer=user_dot_user__pb2.UserListRequest.SerializeToString,
-                response_deserializer=user_dot_user__pb2.DropResponse.FromString,
-                )
-        self.AddDropDown = channel.unary_unary(
-                '/user_proto.UserController/AddDropDown',
-                request_serializer=user_dot_user__pb2.DropRequest.SerializeToString,
-                response_deserializer=google_dot_protobuf_dot_empty__pb2.Empty.FromString,
-                )
-        self.RemoveDropDown = channel.unary_unary(
-                '/user_proto.UserController/RemoveDropDown',
-                request_serializer=user_dot_user__pb2.DropRequest.SerializeToString,
-                response_deserializer=google_dot_protobuf_dot_empty__pb2.Empty.FromString,
-                )
-
-
-class UserControllerServicer(object):
-    """Missing associated documentation comment in .proto file."""
-
-    def List(self, request, context):
-        """Missing associated documentation comment in .proto file."""
-        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
-        context.set_details('Method not implemented!')
-        raise NotImplementedError('Method not implemented!')
-
-    def Create(self, request, context):
-        """Missing associated documentation comment in .proto file."""
-        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
-        context.set_details('Method not implemented!')
-        raise NotImplementedError('Method not implemented!')
-
-    def Retrieve(self, request, context):
-        """Missing associated documentation comment in .proto file."""
-        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
-        context.set_details('Method not implemented!')
-        raise NotImplementedError('Method not implemented!')
-
-    def Update(self, request, context):
-        """Missing associated documentation comment in .proto file."""
-        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
-        context.set_details('Method not implemented!')
-        raise NotImplementedError('Method not implemented!')
-
-    def AddAccess(self, request, context):
-        """Missing associated documentation comment in .proto file."""
-        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
-        context.set_details('Method not implemented!')
-        raise NotImplementedError('Method not implemented!')
-
-    def RemoveAccess(self, request, context):
-        """Missing associated documentation comment in .proto file."""
-        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
-        context.set_details('Method not implemented!')
-        raise NotImplementedError('Method not implemented!')
-
-    def Destroy(self, request, context):
-        """Missing associated documentation comment in .proto file."""
-        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
-        context.set_details('Method not implemented!')
-        raise NotImplementedError('Method not implemented!')
-
-    def ChangePassword(self, request, context):
-        """Missing associated documentation comment in .proto file."""
-        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
-        context.set_details('Method not implemented!')
-        raise NotImplementedError('Method not implemented!')
-
-    def ChangeKey(self, request, context):
-        """Missing associated documentation comment in .proto file."""
-        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
-        context.set_details('Method not implemented!')
-        raise NotImplementedError('Method not implemented!')
-
-    def GetKey(self, request, context):
-        """Missing associated documentation comment in .proto file."""
-        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
-        context.set_details('Method not implemented!')
-        raise NotImplementedError('Method not implemented!')
-
-    def CheckJWT(self, request, context):
-        """Missing associated documentation comment in .proto file."""
-        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
-        context.set_details('Method not implemented!')
-        raise NotImplementedError('Method not implemented!')
-
-    def DropDown(self, request, context):
-        """Missing associated documentation comment in .proto file."""
-        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
-        context.set_details('Method not implemented!')
-        raise NotImplementedError('Method not implemented!')
-
-    def AddDropDown(self, request, context):
-        """Missing associated documentation comment in .proto file."""
-        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
-        context.set_details('Method not implemented!')
-        raise NotImplementedError('Method not implemented!')
-
-    def RemoveDropDown(self, request, context):
-        """Missing associated documentation comment in .proto file."""
-        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
-        context.set_details('Method not implemented!')
-        raise NotImplementedError('Method not implemented!')
-
-
-def add_UserControllerServicer_to_server(servicer, server):
-    rpc_method_handlers = {
-            'List': grpc.unary_stream_rpc_method_handler(
-                    servicer.List,
-                    request_deserializer=user_dot_user__pb2.UserListRequest.FromString,
-                    response_serializer=user_dot_user__pb2.User.SerializeToString,
-            ),
-            'Create': grpc.unary_unary_rpc_method_handler(
-                    servicer.Create,
-                    request_deserializer=user_dot_user__pb2.User.FromString,
-                    response_serializer=user_dot_user__pb2.User.SerializeToString,
-            ),
-            'Retrieve': grpc.unary_unary_rpc_method_handler(
-                    servicer.Retrieve,
-                    request_deserializer=user_dot_user__pb2.UserRetrieveRequest.FromString,
-                    response_serializer=user_dot_user__pb2.User.SerializeToString,
-            ),
-            'Update': grpc.unary_unary_rpc_method_handler(
-                    servicer.Update,
-                    request_deserializer=user_dot_user__pb2.User.FromString,
-                    response_serializer=user_dot_user__pb2.User.SerializeToString,
-            ),
-            'AddAccess': grpc.unary_unary_rpc_method_handler(
-                    servicer.AddAccess,
-                    request_deserializer=user_dot_user__pb2.UserRequest.FromString,
-                    response_serializer=user_dot_user__pb2.User.SerializeToString,
-            ),
-            'RemoveAccess': grpc.unary_unary_rpc_method_handler(
-                    servicer.RemoveAccess,
-                    request_deserializer=user_dot_user__pb2.UserRequest.FromString,
-                    response_serializer=user_dot_user__pb2.User.SerializeToString,
-            ),
-            'Destroy': grpc.unary_unary_rpc_method_handler(
-                    servicer.Destroy,
-                    request_deserializer=user_dot_user__pb2.User.FromString,
-                    response_serializer=google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
-            ),
-            'ChangePassword': grpc.unary_unary_rpc_method_handler(
-                    servicer.ChangePassword,
-                    request_deserializer=user_dot_user__pb2.PasswordRequest.FromString,
-                    response_serializer=user_dot_user__pb2.User.SerializeToString,
-            ),
-            'ChangeKey': grpc.unary_unary_rpc_method_handler(
-                    servicer.ChangeKey,
-                    request_deserializer=user_dot_user__pb2.KeyRequest.FromString,
-                    response_serializer=user_dot_user__pb2.User.SerializeToString,
-            ),
-            'GetKey': grpc.unary_unary_rpc_method_handler(
-                    servicer.GetKey,
-                    request_deserializer=user_dot_user__pb2.KeyRequest.FromString,
-                    response_serializer=user_dot_user__pb2.User.SerializeToString,
-            ),
-            'CheckJWT': grpc.unary_unary_rpc_method_handler(
-                    servicer.CheckJWT,
-                    request_deserializer=user_dot_user__pb2.TokenRequest.FromString,
-                    response_serializer=user_dot_user__pb2.TokenResponse.SerializeToString,
-            ),
-            'DropDown': grpc.unary_unary_rpc_method_handler(
-                    servicer.DropDown,
-                    request_deserializer=user_dot_user__pb2.UserListRequest.FromString,
-                    response_serializer=user_dot_user__pb2.DropResponse.SerializeToString,
-            ),
-            'AddDropDown': grpc.unary_unary_rpc_method_handler(
-                    servicer.AddDropDown,
-                    request_deserializer=user_dot_user__pb2.DropRequest.FromString,
-                    response_serializer=google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
-            ),
-            'RemoveDropDown': grpc.unary_unary_rpc_method_handler(
-                    servicer.RemoveDropDown,
-                    request_deserializer=user_dot_user__pb2.DropRequest.FromString,
-                    response_serializer=google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
-            ),
-    }
-    generic_handler = grpc.method_handlers_generic_handler(
-            'user_proto.UserController', rpc_method_handlers)
-    server.add_generic_rpc_handlers((generic_handler,))
-
-
- # This class is part of an EXPERIMENTAL API.
-class UserController(object):
-    """Missing associated documentation comment in .proto file."""
-
-    @staticmethod
-    def List(request,
-            target,
-            options=(),
-            channel_credentials=None,
-            call_credentials=None,
-            insecure=False,
-            compression=None,
-            wait_for_ready=None,
-            timeout=None,
-            metadata=None):
-        return grpc.experimental.unary_stream(request, target, '/user_proto.UserController/List',
-            user_dot_user__pb2.UserListRequest.SerializeToString,
-            user_dot_user__pb2.User.FromString,
-            options, channel_credentials,
-            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
-
-    @staticmethod
-    def Create(request,
-            target,
-            options=(),
-            channel_credentials=None,
-            call_credentials=None,
-            insecure=False,
-            compression=None,
-            wait_for_ready=None,
-            timeout=None,
-            metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/user_proto.UserController/Create',
-            user_dot_user__pb2.User.SerializeToString,
-            user_dot_user__pb2.User.FromString,
-            options, channel_credentials,
-            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
-
-    @staticmethod
-    def Retrieve(request,
-            target,
-            options=(),
-            channel_credentials=None,
-            call_credentials=None,
-            insecure=False,
-            compression=None,
-            wait_for_ready=None,
-            timeout=None,
-            metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/user_proto.UserController/Retrieve',
-            user_dot_user__pb2.UserRetrieveRequest.SerializeToString,
-            user_dot_user__pb2.User.FromString,
-            options, channel_credentials,
-            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
-
-    @staticmethod
-    def Update(request,
-            target,
-            options=(),
-            channel_credentials=None,
-            call_credentials=None,
-            insecure=False,
-            compression=None,
-            wait_for_ready=None,
-            timeout=None,
-            metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/user_proto.UserController/Update',
-            user_dot_user__pb2.User.SerializeToString,
-            user_dot_user__pb2.User.FromString,
-            options, channel_credentials,
-            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
-
-    @staticmethod
-    def AddAccess(request,
-            target,
-            options=(),
-            channel_credentials=None,
-            call_credentials=None,
-            insecure=False,
-            compression=None,
-            wait_for_ready=None,
-            timeout=None,
-            metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/user_proto.UserController/AddAccess',
-            user_dot_user__pb2.UserRequest.SerializeToString,
-            user_dot_user__pb2.User.FromString,
-            options, channel_credentials,
-            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
-
-    @staticmethod
-    def RemoveAccess(request,
-            target,
-            options=(),
-            channel_credentials=None,
-            call_credentials=None,
-            insecure=False,
-            compression=None,
-            wait_for_ready=None,
-            timeout=None,
-            metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/user_proto.UserController/RemoveAccess',
-            user_dot_user__pb2.UserRequest.SerializeToString,
-            user_dot_user__pb2.User.FromString,
-            options, channel_credentials,
-            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
-
-    @staticmethod
-    def Destroy(request,
-            target,
-            options=(),
-            channel_credentials=None,
-            call_credentials=None,
-            insecure=False,
-            compression=None,
-            wait_for_ready=None,
-            timeout=None,
-            metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/user_proto.UserController/Destroy',
-            user_dot_user__pb2.User.SerializeToString,
-            google_dot_protobuf_dot_empty__pb2.Empty.FromString,
-            options, channel_credentials,
-            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
-
-    @staticmethod
-    def ChangePassword(request,
-            target,
-            options=(),
-            channel_credentials=None,
-            call_credentials=None,
-            insecure=False,
-            compression=None,
-            wait_for_ready=None,
-            timeout=None,
-            metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/user_proto.UserController/ChangePassword',
-            user_dot_user__pb2.PasswordRequest.SerializeToString,
-            user_dot_user__pb2.User.FromString,
-            options, channel_credentials,
-            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
-
-    @staticmethod
-    def ChangeKey(request,
-            target,
-            options=(),
-            channel_credentials=None,
-            call_credentials=None,
-            insecure=False,
-            compression=None,
-            wait_for_ready=None,
-            timeout=None,
-            metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/user_proto.UserController/ChangeKey',
-            user_dot_user__pb2.KeyRequest.SerializeToString,
-            user_dot_user__pb2.User.FromString,
-            options, channel_credentials,
-            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
-
-    @staticmethod
-    def GetKey(request,
-            target,
-            options=(),
-            channel_credentials=None,
-            call_credentials=None,
-            insecure=False,
-            compression=None,
-            wait_for_ready=None,
-            timeout=None,
-            metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/user_proto.UserController/GetKey',
-            user_dot_user__pb2.KeyRequest.SerializeToString,
-            user_dot_user__pb2.User.FromString,
-            options, channel_credentials,
-            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
-
-    @staticmethod
-    def CheckJWT(request,
-            target,
-            options=(),
-            channel_credentials=None,
-            call_credentials=None,
-            insecure=False,
-            compression=None,
-            wait_for_ready=None,
-            timeout=None,
-            metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/user_proto.UserController/CheckJWT',
-            user_dot_user__pb2.TokenRequest.SerializeToString,
-            user_dot_user__pb2.TokenResponse.FromString,
-            options, channel_credentials,
-            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
-
-    @staticmethod
-    def DropDown(request,
-            target,
-            options=(),
-            channel_credentials=None,
-            call_credentials=None,
-            insecure=False,
-            compression=None,
-            wait_for_ready=None,
-            timeout=None,
-            metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/user_proto.UserController/DropDown',
-            user_dot_user__pb2.UserListRequest.SerializeToString,
-            user_dot_user__pb2.DropResponse.FromString,
-            options, channel_credentials,
-            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
-
-    @staticmethod
-    def AddDropDown(request,
-            target,
-            options=(),
-            channel_credentials=None,
-            call_credentials=None,
-            insecure=False,
-            compression=None,
-            wait_for_ready=None,
-            timeout=None,
-            metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/user_proto.UserController/AddDropDown',
-            user_dot_user__pb2.DropRequest.SerializeToString,
-            google_dot_protobuf_dot_empty__pb2.Empty.FromString,
-            options, channel_credentials,
-            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
-
-    @staticmethod
-    def RemoveDropDown(request,
-            target,
-            options=(),
-            channel_credentials=None,
-            call_credentials=None,
-            insecure=False,
-            compression=None,
-            wait_for_ready=None,
-            timeout=None,
-            metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/user_proto.UserController/RemoveDropDown',
-            user_dot_user__pb2.DropRequest.SerializeToString,
-            google_dot_protobuf_dot_empty__pb2.Empty.FromString,
-            options, channel_credentials,
-            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+# Generated by the gRPC Python protocol compiler plugin. DO NOT EDIT!
+"""Client and server classes corresponding to protobuf-defined services."""
+import grpc
+
+from google.protobuf import empty_pb2 as google_dot_protobuf_dot_empty__pb2
+from ..user import user_pb2 as user_dot_user__pb2
+
+
+class UserControllerStub(object):
+    """Missing associated documentation comment in .proto file."""
+
+    def __init__(self, channel):
+        """Constructor.
+
+        Args:
+            channel: A grpc.Channel.
+        """
+        self.List = channel.unary_stream(
+                '/user_proto.UserController/List',
+                request_serializer=user_dot_user__pb2.UserListRequest.SerializeToString,
+                response_deserializer=user_dot_user__pb2.User.FromString,
+                )
+        self.Create = channel.unary_unary(
+                '/user_proto.UserController/Create',
+                request_serializer=user_dot_user__pb2.User.SerializeToString,
+                response_deserializer=user_dot_user__pb2.User.FromString,
+                )
+        self.Retrieve = channel.unary_unary(
+                '/user_proto.UserController/Retrieve',
+                request_serializer=user_dot_user__pb2.UserRetrieveRequest.SerializeToString,
+                response_deserializer=user_dot_user__pb2.User.FromString,
+                )
+        self.Update = channel.unary_unary(
+                '/user_proto.UserController/Update',
+                request_serializer=user_dot_user__pb2.User.SerializeToString,
+                response_deserializer=user_dot_user__pb2.User.FromString,
+                )
+        self.AddAccess = channel.unary_unary(
+                '/user_proto.UserController/AddAccess',
+                request_serializer=user_dot_user__pb2.UserRequest.SerializeToString,
+                response_deserializer=user_dot_user__pb2.User.FromString,
+                )
+        self.RemoveAccess = channel.unary_unary(
+                '/user_proto.UserController/RemoveAccess',
+                request_serializer=user_dot_user__pb2.UserRequest.SerializeToString,
+                response_deserializer=user_dot_user__pb2.User.FromString,
+                )
+        self.Destroy = channel.unary_unary(
+                '/user_proto.UserController/Destroy',
+                request_serializer=user_dot_user__pb2.User.SerializeToString,
+                response_deserializer=google_dot_protobuf_dot_empty__pb2.Empty.FromString,
+                )
+        self.ChangePassword = channel.unary_unary(
+                '/user_proto.UserController/ChangePassword',
+                request_serializer=user_dot_user__pb2.PasswordRequest.SerializeToString,
+                response_deserializer=user_dot_user__pb2.User.FromString,
+                )
+        self.ChangeKey = channel.unary_unary(
+                '/user_proto.UserController/ChangeKey',
+                request_serializer=user_dot_user__pb2.KeyRequest.SerializeToString,
+                response_deserializer=user_dot_user__pb2.User.FromString,
+                )
+        self.GetKey = channel.unary_unary(
+                '/user_proto.UserController/GetKey',
+                request_serializer=user_dot_user__pb2.KeyRequest.SerializeToString,
+                response_deserializer=user_dot_user__pb2.User.FromString,
+                )
+        self.CheckJWT = channel.unary_unary(
+                '/user_proto.UserController/CheckJWT',
+                request_serializer=user_dot_user__pb2.TokenRequest.SerializeToString,
+                response_deserializer=user_dot_user__pb2.TokenResponse.FromString,
+                )
+        self.DropDown = channel.unary_unary(
+                '/user_proto.UserController/DropDown',
+                request_serializer=user_dot_user__pb2.UserListRequest.SerializeToString,
+                response_deserializer=user_dot_user__pb2.DropResponse.FromString,
+                )
+        self.AddDropDown = channel.unary_unary(
+                '/user_proto.UserController/AddDropDown',
+                request_serializer=user_dot_user__pb2.DropRequest.SerializeToString,
+                response_deserializer=google_dot_protobuf_dot_empty__pb2.Empty.FromString,
+                )
+        self.RemoveDropDown = channel.unary_unary(
+                '/user_proto.UserController/RemoveDropDown',
+                request_serializer=user_dot_user__pb2.DropRequest.SerializeToString,
+                response_deserializer=google_dot_protobuf_dot_empty__pb2.Empty.FromString,
+                )
+
+
+class UserControllerServicer(object):
+    """Missing associated documentation comment in .proto file."""
+
+    def List(self, request, context):
+        """Missing associated documentation comment in .proto file."""
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
+    def Create(self, request, context):
+        """Missing associated documentation comment in .proto file."""
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
+    def Retrieve(self, request, context):
+        """Missing associated documentation comment in .proto file."""
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
+    def Update(self, request, context):
+        """Missing associated documentation comment in .proto file."""
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
+    def AddAccess(self, request, context):
+        """Missing associated documentation comment in .proto file."""
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
+    def RemoveAccess(self, request, context):
+        """Missing associated documentation comment in .proto file."""
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
+    def Destroy(self, request, context):
+        """Missing associated documentation comment in .proto file."""
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
+    def ChangePassword(self, request, context):
+        """Missing associated documentation comment in .proto file."""
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
+    def ChangeKey(self, request, context):
+        """Missing associated documentation comment in .proto file."""
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
+    def GetKey(self, request, context):
+        """Missing associated documentation comment in .proto file."""
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
+    def CheckJWT(self, request, context):
+        """Missing associated documentation comment in .proto file."""
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
+    def DropDown(self, request, context):
+        """Missing associated documentation comment in .proto file."""
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
+    def AddDropDown(self, request, context):
+        """Missing associated documentation comment in .proto file."""
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
+    def RemoveDropDown(self, request, context):
+        """Missing associated documentation comment in .proto file."""
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
+
+def add_UserControllerServicer_to_server(servicer, server):
+    rpc_method_handlers = {
+            'List': grpc.unary_stream_rpc_method_handler(
+                    servicer.List,
+                    request_deserializer=user_dot_user__pb2.UserListRequest.FromString,
+                    response_serializer=user_dot_user__pb2.User.SerializeToString,
+            ),
+            'Create': grpc.unary_unary_rpc_method_handler(
+                    servicer.Create,
+                    request_deserializer=user_dot_user__pb2.User.FromString,
+                    response_serializer=user_dot_user__pb2.User.SerializeToString,
+            ),
+            'Retrieve': grpc.unary_unary_rpc_method_handler(
+                    servicer.Retrieve,
+                    request_deserializer=user_dot_user__pb2.UserRetrieveRequest.FromString,
+                    response_serializer=user_dot_user__pb2.User.SerializeToString,
+            ),
+            'Update': grpc.unary_unary_rpc_method_handler(
+                    servicer.Update,
+                    request_deserializer=user_dot_user__pb2.User.FromString,
+                    response_serializer=user_dot_user__pb2.User.SerializeToString,
+            ),
+            'AddAccess': grpc.unary_unary_rpc_method_handler(
+                    servicer.AddAccess,
+                    request_deserializer=user_dot_user__pb2.UserRequest.FromString,
+                    response_serializer=user_dot_user__pb2.User.SerializeToString,
+            ),
+            'RemoveAccess': grpc.unary_unary_rpc_method_handler(
+                    servicer.RemoveAccess,
+                    request_deserializer=user_dot_user__pb2.UserRequest.FromString,
+                    response_serializer=user_dot_user__pb2.User.SerializeToString,
+            ),
+            'Destroy': grpc.unary_unary_rpc_method_handler(
+                    servicer.Destroy,
+                    request_deserializer=user_dot_user__pb2.User.FromString,
+                    response_serializer=google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
+            ),
+            'ChangePassword': grpc.unary_unary_rpc_method_handler(
+                    servicer.ChangePassword,
+                    request_deserializer=user_dot_user__pb2.PasswordRequest.FromString,
+                    response_serializer=user_dot_user__pb2.User.SerializeToString,
+            ),
+            'ChangeKey': grpc.unary_unary_rpc_method_handler(
+                    servicer.ChangeKey,
+                    request_deserializer=user_dot_user__pb2.KeyRequest.FromString,
+                    response_serializer=user_dot_user__pb2.User.SerializeToString,
+            ),
+            'GetKey': grpc.unary_unary_rpc_method_handler(
+                    servicer.GetKey,
+                    request_deserializer=user_dot_user__pb2.KeyRequest.FromString,
+                    response_serializer=user_dot_user__pb2.User.SerializeToString,
+            ),
+            'CheckJWT': grpc.unary_unary_rpc_method_handler(
+                    servicer.CheckJWT,
+                    request_deserializer=user_dot_user__pb2.TokenRequest.FromString,
+                    response_serializer=user_dot_user__pb2.TokenResponse.SerializeToString,
+            ),
+            'DropDown': grpc.unary_unary_rpc_method_handler(
+                    servicer.DropDown,
+                    request_deserializer=user_dot_user__pb2.UserListRequest.FromString,
+                    response_serializer=user_dot_user__pb2.DropResponse.SerializeToString,
+            ),
+            'AddDropDown': grpc.unary_unary_rpc_method_handler(
+                    servicer.AddDropDown,
+                    request_deserializer=user_dot_user__pb2.DropRequest.FromString,
+                    response_serializer=google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
+            ),
+            'RemoveDropDown': grpc.unary_unary_rpc_method_handler(
+                    servicer.RemoveDropDown,
+                    request_deserializer=user_dot_user__pb2.DropRequest.FromString,
+                    response_serializer=google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
+            ),
+    }
+    generic_handler = grpc.method_handlers_generic_handler(
+            'user_proto.UserController', rpc_method_handlers)
+    server.add_generic_rpc_handlers((generic_handler,))
+
+
+ # This class is part of an EXPERIMENTAL API.
+class UserController(object):
+    """Missing associated documentation comment in .proto file."""
+
+    @staticmethod
+    def List(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_stream(request, target, '/user_proto.UserController/List',
+            user_dot_user__pb2.UserListRequest.SerializeToString,
+            user_dot_user__pb2.User.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
+    def Create(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/user_proto.UserController/Create',
+            user_dot_user__pb2.User.SerializeToString,
+            user_dot_user__pb2.User.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
+    def Retrieve(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/user_proto.UserController/Retrieve',
+            user_dot_user__pb2.UserRetrieveRequest.SerializeToString,
+            user_dot_user__pb2.User.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
+    def Update(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/user_proto.UserController/Update',
+            user_dot_user__pb2.User.SerializeToString,
+            user_dot_user__pb2.User.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
+    def AddAccess(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/user_proto.UserController/AddAccess',
+            user_dot_user__pb2.UserRequest.SerializeToString,
+            user_dot_user__pb2.User.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
+    def RemoveAccess(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/user_proto.UserController/RemoveAccess',
+            user_dot_user__pb2.UserRequest.SerializeToString,
+            user_dot_user__pb2.User.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
+    def Destroy(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/user_proto.UserController/Destroy',
+            user_dot_user__pb2.User.SerializeToString,
+            google_dot_protobuf_dot_empty__pb2.Empty.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
+    def ChangePassword(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/user_proto.UserController/ChangePassword',
+            user_dot_user__pb2.PasswordRequest.SerializeToString,
+            user_dot_user__pb2.User.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
+    def ChangeKey(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/user_proto.UserController/ChangeKey',
+            user_dot_user__pb2.KeyRequest.SerializeToString,
+            user_dot_user__pb2.User.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
+    def GetKey(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/user_proto.UserController/GetKey',
+            user_dot_user__pb2.KeyRequest.SerializeToString,
+            user_dot_user__pb2.User.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
+    def CheckJWT(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/user_proto.UserController/CheckJWT',
+            user_dot_user__pb2.TokenRequest.SerializeToString,
+            user_dot_user__pb2.TokenResponse.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
+    def DropDown(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/user_proto.UserController/DropDown',
+            user_dot_user__pb2.UserListRequest.SerializeToString,
+            user_dot_user__pb2.DropResponse.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
+    def AddDropDown(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/user_proto.UserController/AddDropDown',
+            user_dot_user__pb2.DropRequest.SerializeToString,
+            google_dot_protobuf_dot_empty__pb2.Empty.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
+    def RemoveDropDown(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/user_proto.UserController/RemoveDropDown',
+            user_dot_user__pb2.DropRequest.SerializeToString,
+            google_dot_protobuf_dot_empty__pb2.Empty.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
```

### Comparing `NuOCR-0.2.2/NuOCR/templated_flow.py` & `NuOCR-0.2.3/NuOCR/templated_flow.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,69 +1,66 @@
 import json
 from .gRPC_proto.templated_flow import templated_flow_pb2, templated_flow_pb2_grpc
 from .channel import CHANNEL
 import grpc
 
+
 class TemplatedFlow:
     def __init__(self, metadata):
+        self.stub = templated_flow_pb2_grpc.TemplatedFlowControllerStub(CHANNEL)
         self.metadata = metadata
 
     def createTemplate(self, documentName, base64, description, boundingBox):
         try:
-            stub = templated_flow_pb2_grpc.TemplatedFlowControllerStub(CHANNEL)
             request = templated_flow_pb2.TemplateRequest(
                 documentName=documentName,
                 base64=base64,
                 description=description,
                 box=[templated_flow_pb2.BoundingBox(
                     label=i['label'],
                     x=i['x'],
                     y=i['y'],
                     h=i['h'],
                     w=i['w'],
                 ) for i in boundingBox]
             )
-            response = stub.CreateTemplate(request, metadata=self.metadata)
+            response = self.stub.CreateTemplate(request, metadata=self.metadata)
             return json.loads(response.status)
         except grpc.RpcError as e:
             raise Exception('Error ' + str(e.code()) + ': ' + str(e.details()))
 
-
     def fetchTemplate(self):
         try:
-            stub = templated_flow_pb2_grpc.TemplatedFlowControllerStub(CHANNEL)
             request = templated_flow_pb2.FetchRequest()
-            response = stub.FetchTemplate(request, metadata=self.metadata)
+            response = self.stub.FetchTemplate(request, metadata=self.metadata)
             list_data = [{'id': i.documentId,
                           'name': i.documentName,
                           'base64': i.base64,
                           'mimeType': i.mimeType} for i in response]
             return list_data
         except grpc.RpcError as e:
             raise Exception('Error ' + str(e.code()) + ': ' + str(e.details()))
 
     def extractTemplate(self, documentName, documentId, base64, fileName, readStatus=True):
         try:
-            stub = templated_flow_pb2_grpc.TemplatedFlowControllerStub(CHANNEL)
             request = templated_flow_pb2.ExtractRequest(
                 documentId=documentId,
                 documentName=documentName,
                 base64=base64,
                 fileName=fileName,
                 readStatus=readStatus,
             )
-            response = stub.Extract(request, metadata=self.metadata)
+            response = self.stub.Extract(request, metadata=self.metadata)
             return json.loads(response.response)
         except grpc.RpcError as e:
             raise Exception('Error ' + str(e.code()) + ': ' + str(e.details()))
 
     def deleteTemplate(self, documentName, documentId):
         try:
-            stub = templated_flow_pb2_grpc.TemplatedFlowControllerStub(CHANNEL)
             request = templated_flow_pb2.DeleteRequest(
                 documentId=documentId,
                 documentName=documentName,
             )
-            stub.Delete(request, metadata=self.metadata)
+            self.stub.Delete(request, metadata=self.metadata)
             return "Template deleted Successfully"
         except grpc.RpcError as e:
             raise Exception('Error ' + str(e.code()) + ': ' + str(e.details()))
```

### Comparing `NuOCR-0.2.2/NuOCR/user.py` & `NuOCR-0.2.3/NuOCR/user.py`

 * *Files 20% similar despite different names*

```diff
@@ -35,11 +35,22 @@
             return response
         except grpc.RpcError as e:
             raise Exception('Error ' + str(e.code()) + ': ' + str(e.details()))
 
     def login(self):
         try:
             response = self.auth_stub.Login(auth_pb2.LoginRequest(username=self.username, password=self.password))
-            meta = [('jwt-access-token', json.loads(response.token)['token'])]
+            response = json.loads(response.token)
+            meta = [('jwt-access-token', response['token']),
+                    ('user-role', response['role']),
+                    ('user-status', response['status']),
+                    ('username', response['username'])]
             return meta
         except grpc.RpcError as e:
             raise Exception('Error ' + str(e.code()) + ': ' + str(e.details()))
+
+    def dropdown(self):
+        try:
+            response = self.stub.DropDown(user_pb2.UserListRequest(), metadata=self.login())
+            return response.option
+        except grpc.RpcError as e:
+            raise Exception('Error ' + str(e.code()) + ': ' + str(e.details()))
```

### Comparing `NuOCR-0.2.2/NuOCR.egg-info/PKG-INFO` & `NuOCR-0.2.3/NuOCR.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NuOCR
-Version: 0.2.2
+Version: 0.2.3
 Summary: Using NuOCR service via APIs
 Author: Nuvento Systems Pvt. Ltd. (Jigar Makwana)
 Author-email: <makwana.jigar@nuvento.com>
 Keywords: python,NuOCR,OCR
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `NuOCR-0.2.2/NuOCR.egg-info/SOURCES.txt` & `NuOCR-0.2.3/NuOCR.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 README.md
 setup.py
 NuOCR/__init__.py
 NuOCR/admin.py
 NuOCR/channel.py
 NuOCR/extractor.py
 NuOCR/io_adaptor.py
+NuOCR/monitor.py
+NuOCR/preprocessors.py
 NuOCR/templated_flow.py
 NuOCR/text.py
 NuOCR/user.py
 NuOCR/util.py
 NuOCR.egg-info/PKG-INFO
 NuOCR.egg-info/SOURCES.txt
 NuOCR.egg-info/dependency_links.txt
@@ -17,14 +19,23 @@
 NuOCR/gRPC_proto/__init__.py
 NuOCR/gRPC_proto/extractor/__init__.py
 NuOCR/gRPC_proto/extractor/extractor_pb2.py
 NuOCR/gRPC_proto/extractor/extractor_pb2_grpc.py
 NuOCR/gRPC_proto/io_adaptors/__init__.py
 NuOCR/gRPC_proto/io_adaptors/io_adaptors_pb2.py
 NuOCR/gRPC_proto/io_adaptors/io_adaptors_pb2_grpc.py
+NuOCR/gRPC_proto/monitor/__init__.py
+NuOCR/gRPC_proto/monitor/monitor_pb2.py
+NuOCR/gRPC_proto/monitor/monitor_pb2_grpc.py
+NuOCR/gRPC_proto/nufarm_poc/__init__.py
+NuOCR/gRPC_proto/nufarm_poc/nufarm_poc_pb2.py
+NuOCR/gRPC_proto/nufarm_poc/nufarm_poc_pb2_grpc.py
+NuOCR/gRPC_proto/preprocessor/__init__.py
+NuOCR/gRPC_proto/preprocessor/preprocessor_pb2.py
+NuOCR/gRPC_proto/preprocessor/preprocessor_pb2_grpc.py
 NuOCR/gRPC_proto/templated_flow/__init__.py
 NuOCR/gRPC_proto/templated_flow/templated_flow_pb2.py
 NuOCR/gRPC_proto/templated_flow/templated_flow_pb2_grpc.py
 NuOCR/gRPC_proto/text_processor/__init__.py
 NuOCR/gRPC_proto/text_processor/text_processor_pb2.py
 NuOCR/gRPC_proto/text_processor/text_processor_pb2_grpc.py
 NuOCR/gRPC_proto/user/__init__.py
```

### Comparing `NuOCR-0.2.2/PKG-INFO` & `NuOCR-0.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NuOCR
-Version: 0.2.2
+Version: 0.2.3
 Summary: Using NuOCR service via APIs
 Author: Nuvento Systems Pvt. Ltd. (Jigar Makwana)
 Author-email: <makwana.jigar@nuvento.com>
 Keywords: python,NuOCR,OCR
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `NuOCR-0.2.2/README.md` & `NuOCR-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `NuOCR-0.2.2/setup.py` & `NuOCR-0.2.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 # with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
 #     long_description = "\n" + fh.read()
 
-VERSION = '0.2.2'
+VERSION = '0.2.3'
 DESCRIPTION = 'Using NuOCR service via APIs'
 LONG_DESCRIPTION = 'A package that allows to utilize NuOCR sevices through API implementation.'
 
 # Setting up
 setup(
     name="NuOCR",
     version=VERSION,
```

