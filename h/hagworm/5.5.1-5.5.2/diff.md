# Comparing `tmp/hagworm-5.5.1.tar.gz` & `tmp/hagworm-5.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hagworm-5.5.1.tar", last modified: Thu May 18 03:28:26 2023, max compression
+gzip compressed data, was "hagworm-5.5.2.tar", last modified: Thu May 18 11:19:47 2023, max compression
```

## Comparing `hagworm-5.5.1.tar` & `hagworm-5.5.2.tar`

### file list

```diff
@@ -1,95 +1,95 @@
-drwxrwxrwx   0        0        0        0 2023-05-18 03:28:26.941364 hagworm-5.5.1/
--rw-rw-rw-   0        0        0    11362 2023-03-01 02:07:14.000000 hagworm-5.5.1/LICENSE
--rw-rw-rw-   0        0        0     7509 2023-05-18 03:28:26.940362 hagworm-5.5.1/PKG-INFO
--rw-rw-rw-   0        0        0     6065 2023-04-08 01:06:26.000000 hagworm-5.5.1/README.md
-drwxrwxrwx   0        0        0        0 2023-05-18 03:28:26.835363 hagworm-5.5.1/c_extend/
--rw-rw-rw-   0        0        0      847 2023-03-01 02:07:14.000000 hagworm-5.5.1/c_extend/math.c
-drwxrwxrwx   0        0        0        0 2023-05-18 03:28:26.839362 hagworm-5.5.1/example/
--rw-rw-rw-   0        0        0       58 2023-03-01 02:07:14.000000 hagworm-5.5.1/example/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-18 03:28:26.844363 hagworm-5.5.1/example/fastapi_demo/
--rw-rw-rw-   0        0        0       58 2023-03-01 02:07:14.000000 hagworm-5.5.1/example/fastapi_demo/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-18 03:28:26.847362 hagworm-5.5.1/example/fastapi_demo/controller/
--rw-rw-rw-   0        0        0      211 2023-03-01 02:07:14.000000 hagworm-5.5.1/example/fastapi_demo/controller/__init__.py
--rw-rw-rw-   0        0        0      397 2023-03-01 02:07:14.000000 hagworm-5.5.1/example/fastapi_demo/controller/home.py
--rw-rw-rw-   0        0        0      888 2023-05-11 03:07:54.000000 hagworm-5.5.1/example/fastapi_demo/gunicorn.config.py
--rw-rw-rw-   0        0        0     1431 2023-05-17 08:11:13.000000 hagworm-5.5.1/example/fastapi_demo/main.py
-drwxrwxrwx   0        0        0        0 2023-05-18 03:28:26.848363 hagworm-5.5.1/example/fastapi_demo/model/
--rw-rw-rw-   0        0        0       58 2023-03-01 02:07:14.000000 hagworm-5.5.1/example/fastapi_demo/model/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-18 03:28:26.850362 hagworm-5.5.1/example/fastapi_demo/service/
--rw-rw-rw-   0        0        0     3496 2023-03-01 02:07:14.000000 hagworm-5.5.1/example/fastapi_demo/service/__init__.py
--rw-rw-rw-   0        0        0     2096 2023-03-01 02:07:14.000000 hagworm-5.5.1/example/fastapi_demo/setting.py
--rw-rw-rw-   0        0        0      800 2023-05-11 03:07:54.000000 hagworm-5.5.1/example/main_test.py
-drwxrwxrwx   0        0        0        0 2023-05-18 03:28:26.852364 hagworm-5.5.1/hagworm/
--rw-rw-rw-   0        0        0      495 2023-05-17 00:46:02.000000 hagworm-5.5.1/hagworm/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-18 03:28:26.888363 hagworm-5.5.1/hagworm/extend/
--rw-rw-rw-   0        0        0       58 2023-03-01 02:07:14.000000 hagworm-5.5.1/hagworm/extend/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-18 03:28:26.916363 hagworm-5.5.1/hagworm/extend/asyncio/
--rw-rw-rw-   0        0        0       58 2023-03-01 02:07:14.000000 hagworm-5.5.1/hagworm/extend/asyncio/__init__.py
--rw-rw-rw-   0        0        0    16802 2023-05-07 00:52:16.000000 hagworm-5.5.1/hagworm/extend/asyncio/base.py
--rw-rw-rw-   0        0        0     4988 2023-05-07 00:52:16.000000 hagworm-5.5.1/hagworm/extend/asyncio/buffer.py
--rw-rw-rw-   0        0        0     2396 2023-05-11 03:07:54.000000 hagworm-5.5.1/hagworm/extend/asyncio/command.py
--rw-rw-rw-   0        0        0     1356 2023-05-18 02:06:14.000000 hagworm-5.5.1/hagworm/extend/asyncio/etcd.py
--rw-rw-rw-   0        0        0     3194 2023-05-07 00:52:16.000000 hagworm-5.5.1/hagworm/extend/asyncio/event.py
--rw-rw-rw-   0        0        0     1370 2023-05-07 00:52:16.000000 hagworm-5.5.1/hagworm/extend/asyncio/file.py
--rw-rw-rw-   0        0        0     4232 2023-03-01 02:07:14.000000 hagworm-5.5.1/hagworm/extend/asyncio/future.py
--rw-rw-rw-   0        0        0     2603 2023-03-01 02:07:14.000000 hagworm-5.5.1/hagworm/extend/asyncio/mail.py
--rw-rw-rw-   0        0        0     3897 2023-03-01 02:07:14.000000 hagworm-5.5.1/hagworm/extend/asyncio/mongo.py
--rw-rw-rw-   0        0        0    15022 2023-05-07 00:52:16.000000 hagworm-5.5.1/hagworm/extend/asyncio/mysql.py
--rw-rw-rw-   0        0        0    13489 2023-03-01 02:07:14.000000 hagworm-5.5.1/hagworm/extend/asyncio/net.py
--rw-rw-rw-   0        0        0     4149 2023-03-01 02:07:14.000000 hagworm-5.5.1/hagworm/extend/asyncio/ntp.py
--rw-rw-rw-   0        0        0     1768 2023-05-18 01:58:04.000000 hagworm-5.5.1/hagworm/extend/asyncio/pool.py
--rw-rw-rw-   0        0        0    12506 2023-05-07 00:52:16.000000 hagworm-5.5.1/hagworm/extend/asyncio/redis.py
--rw-rw-rw-   0        0        0     7279 2023-05-11 03:07:54.000000 hagworm-5.5.1/hagworm/extend/asyncio/socket.py
--rw-rw-rw-   0        0        0     6170 2023-04-11 07:28:18.000000 hagworm-5.5.1/hagworm/extend/asyncio/task.py
--rw-rw-rw-   0        0        0     1360 2023-03-01 02:07:14.000000 hagworm-5.5.1/hagworm/extend/asyncio/transaction.py
--rw-rw-rw-   0        0        0     3792 2023-03-01 02:07:14.000000 hagworm-5.5.1/hagworm/extend/asyncio/zmq.py
--rw-rw-rw-   0        0        0    22623 2023-05-11 03:07:54.000000 hagworm-5.5.1/hagworm/extend/base.py
--rw-rw-rw-   0        0        0     2365 2023-03-01 02:07:14.000000 hagworm-5.5.1/hagworm/extend/cache.py
--rw-rw-rw-   0        0        0     1839 2023-05-07 00:52:16.000000 hagworm-5.5.1/hagworm/extend/compile.py
--rw-rw-rw-   0        0        0     3857 2023-03-01 02:07:14.000000 hagworm-5.5.1/hagworm/extend/config.py
--rw-rw-rw-   0        0        0     1487 2023-03-01 02:07:14.000000 hagworm-5.5.1/hagworm/extend/crypto.py
--rw-rw-rw-   0        0        0     1792 2023-05-07 00:52:16.000000 hagworm-5.5.1/hagworm/extend/error.py
--rw-rw-rw-   0        0        0     1220 2023-03-01 02:07:14.000000 hagworm-5.5.1/hagworm/extend/event.py
--rw-rw-rw-   0        0        0     4558 2023-05-07 00:52:16.000000 hagworm-5.5.1/hagworm/extend/igraph.py
--rw-rw-rw-   0        0        0     2326 2023-05-07 00:52:16.000000 hagworm-5.5.1/hagworm/extend/interface.py
--rw-rw-rw-   0        0        0    14870 2023-05-13 05:06:56.000000 hagworm-5.5.1/hagworm/extend/logging.py
--rw-rw-rw-   0        0        0     1791 2023-03-01 02:07:14.000000 hagworm-5.5.1/hagworm/extend/media.py
--rw-rw-rw-   0        0        0     1603 2023-05-10 07:58:09.000000 hagworm-5.5.1/hagworm/extend/metaclass.py
--rw-rw-rw-   0        0        0     4500 2023-05-11 03:07:54.000000 hagworm-5.5.1/hagworm/extend/process.py
--rw-rw-rw-   0        0        0      551 2023-03-01 02:07:14.000000 hagworm-5.5.1/hagworm/extend/qrcode.py
--rw-rw-rw-   0        0        0     7235 2023-05-07 00:52:16.000000 hagworm-5.5.1/hagworm/extend/struct.py
--rw-rw-rw-   0        0        0     3758 2023-05-07 00:52:16.000000 hagworm-5.5.1/hagworm/extend/text.py
--rw-rw-rw-   0        0        0     2409 2023-03-01 02:07:14.000000 hagworm-5.5.1/hagworm/extend/trace.py
--rw-rw-rw-   0        0        0     2677 2023-03-01 02:07:14.000000 hagworm-5.5.1/hagworm/extend/transaction.py
--rw-rw-rw-   0        0        0     6411 2023-03-01 02:07:14.000000 hagworm-5.5.1/hagworm/extend/validator.py
-drwxrwxrwx   0        0        0        0 2023-05-18 03:28:26.920364 hagworm-5.5.1/hagworm/frame/
--rw-rw-rw-   0        0        0       58 2023-03-01 02:07:14.000000 hagworm-5.5.1/hagworm/frame/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-18 03:28:26.927362 hagworm-5.5.1/hagworm/frame/fastapi/
--rw-rw-rw-   0        0        0       58 2023-03-01 02:07:14.000000 hagworm-5.5.1/hagworm/frame/fastapi/__init__.py
--rw-rw-rw-   0        0        0     8148 2023-05-07 00:52:16.000000 hagworm-5.5.1/hagworm/frame/fastapi/base.py
--rw-rw-rw-   0        0        0     8494 2023-03-01 02:07:14.000000 hagworm-5.5.1/hagworm/frame/fastapi/field.py
--rw-rw-rw-   0        0        0     1389 2023-03-01 02:07:14.000000 hagworm-5.5.1/hagworm/frame/fastapi/model.py
--rw-rw-rw-   0        0        0     1000 2023-03-01 02:07:14.000000 hagworm-5.5.1/hagworm/frame/fastapi/response.py
--rw-rw-rw-   0        0        0     1304 2023-03-01 02:07:14.000000 hagworm-5.5.1/hagworm/frame/gunicorn.py
--rw-rw-rw-   0        0        0     3846 2023-05-11 03:07:54.000000 hagworm-5.5.1/hagworm/frame/stress_tests.py
-drwxrwxrwx   0        0        0        0 2023-05-18 03:28:26.929362 hagworm-5.5.1/hagworm/static/
--rw-rw-rw-   0        0        0       58 2023-03-01 02:07:14.000000 hagworm-5.5.1/hagworm/static/__init__.py
--rw-rw-rw-   0        0        0   208075 2023-03-01 02:07:14.000000 hagworm-5.5.1/hagworm/static/cacert.pem
-drwxrwxrwx   0        0        0        0 2023-05-18 03:28:26.931363 hagworm-5.5.1/hagworm/third/
--rw-rw-rw-   0        0        0       58 2023-03-01 02:07:14.000000 hagworm-5.5.1/hagworm/third/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-18 03:28:26.933362 hagworm-5.5.1/hagworm/third/consul/
--rw-rw-rw-   0        0        0       58 2023-03-01 02:07:14.000000 hagworm-5.5.1/hagworm/third/consul/__init__.py
--rw-rw-rw-   0        0        0     1288 2023-03-01 02:07:14.000000 hagworm-5.5.1/hagworm/third/consul/config.py
-drwxrwxrwx   0        0        0        0 2023-05-18 03:28:26.939361 hagworm-5.5.1/hagworm/third/rabbitmq/
--rw-rw-rw-   0        0        0       58 2023-03-01 02:07:14.000000 hagworm-5.5.1/hagworm/third/rabbitmq/__init__.py
--rw-rw-rw-   0        0        0     3564 2023-05-07 00:52:16.000000 hagworm-5.5.1/hagworm/third/rabbitmq/consume.py
--rw-rw-rw-   0        0        0     5350 2023-03-01 02:07:14.000000 hagworm-5.5.1/hagworm/third/rabbitmq/publish.py
--rw-rw-rw-   0        0        0     5743 2023-04-12 08:59:35.000000 hagworm-5.5.1/hagworm/third/rabbitmq/rpc.py
-drwxrwxrwx   0        0        0        0 2023-05-18 03:28:26.859363 hagworm-5.5.1/hagworm.egg-info/
--rw-rw-rw-   0        0        0     7509 2023-05-18 03:28:26.000000 hagworm-5.5.1/hagworm.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2211 2023-05-18 03:28:26.000000 hagworm-5.5.1/hagworm.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-18 03:28:26.000000 hagworm-5.5.1/hagworm.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      678 2023-05-18 03:28:26.000000 hagworm-5.5.1/hagworm.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-05-18 03:28:26.000000 hagworm-5.5.1/hagworm.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-18 03:28:26.941364 hagworm-5.5.1/setup.cfg
--rw-rw-rw-   0        0        0     2330 2023-05-17 00:38:12.000000 hagworm-5.5.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-18 11:19:47.457363 hagworm-5.5.2/
+-rw-rw-rw-   0        0        0    11362 2023-03-01 02:07:14.000000 hagworm-5.5.2/LICENSE
+-rw-rw-rw-   0        0        0     7515 2023-05-18 11:19:47.456362 hagworm-5.5.2/PKG-INFO
+-rw-rw-rw-   0        0        0     6065 2023-04-08 01:06:26.000000 hagworm-5.5.2/README.md
+drwxrwxrwx   0        0        0        0 2023-05-18 11:19:47.351362 hagworm-5.5.2/c_extend/
+-rw-rw-rw-   0        0        0      847 2023-03-01 02:07:14.000000 hagworm-5.5.2/c_extend/math.c
+drwxrwxrwx   0        0        0        0 2023-05-18 11:19:47.353362 hagworm-5.5.2/example/
+-rw-rw-rw-   0        0        0       58 2023-03-01 02:07:14.000000 hagworm-5.5.2/example/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-18 11:19:47.359362 hagworm-5.5.2/example/fastapi_demo/
+-rw-rw-rw-   0        0        0       58 2023-03-01 02:07:14.000000 hagworm-5.5.2/example/fastapi_demo/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-18 11:19:47.362362 hagworm-5.5.2/example/fastapi_demo/controller/
+-rw-rw-rw-   0        0        0      211 2023-03-01 02:07:14.000000 hagworm-5.5.2/example/fastapi_demo/controller/__init__.py
+-rw-rw-rw-   0        0        0      397 2023-03-01 02:07:14.000000 hagworm-5.5.2/example/fastapi_demo/controller/home.py
+-rw-rw-rw-   0        0        0      888 2023-05-11 03:07:54.000000 hagworm-5.5.2/example/fastapi_demo/gunicorn.config.py
+-rw-rw-rw-   0        0        0     1431 2023-05-17 08:11:13.000000 hagworm-5.5.2/example/fastapi_demo/main.py
+drwxrwxrwx   0        0        0        0 2023-05-18 11:19:47.363362 hagworm-5.5.2/example/fastapi_demo/model/
+-rw-rw-rw-   0        0        0       58 2023-03-01 02:07:14.000000 hagworm-5.5.2/example/fastapi_demo/model/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-18 11:19:47.364362 hagworm-5.5.2/example/fastapi_demo/service/
+-rw-rw-rw-   0        0        0     3496 2023-03-01 02:07:14.000000 hagworm-5.5.2/example/fastapi_demo/service/__init__.py
+-rw-rw-rw-   0        0        0     2096 2023-03-01 02:07:14.000000 hagworm-5.5.2/example/fastapi_demo/setting.py
+-rw-rw-rw-   0        0        0      800 2023-05-11 03:07:54.000000 hagworm-5.5.2/example/main_test.py
+drwxrwxrwx   0        0        0        0 2023-05-18 11:19:47.366362 hagworm-5.5.2/hagworm/
+-rw-rw-rw-   0        0        0      495 2023-05-18 08:48:52.000000 hagworm-5.5.2/hagworm/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-18 11:19:47.402362 hagworm-5.5.2/hagworm/extend/
+-rw-rw-rw-   0        0        0       58 2023-03-01 02:07:14.000000 hagworm-5.5.2/hagworm/extend/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-18 11:19:47.430362 hagworm-5.5.2/hagworm/extend/asyncio/
+-rw-rw-rw-   0        0        0       58 2023-03-01 02:07:14.000000 hagworm-5.5.2/hagworm/extend/asyncio/__init__.py
+-rw-rw-rw-   0        0        0    16802 2023-05-07 00:52:16.000000 hagworm-5.5.2/hagworm/extend/asyncio/base.py
+-rw-rw-rw-   0        0        0     4988 2023-05-07 00:52:16.000000 hagworm-5.5.2/hagworm/extend/asyncio/buffer.py
+-rw-rw-rw-   0        0        0     2396 2023-05-11 03:07:54.000000 hagworm-5.5.2/hagworm/extend/asyncio/command.py
+-rw-rw-rw-   0        0        0     2432 2023-05-18 10:57:40.000000 hagworm-5.5.2/hagworm/extend/asyncio/etcd.py
+-rw-rw-rw-   0        0        0     3194 2023-05-07 00:52:16.000000 hagworm-5.5.2/hagworm/extend/asyncio/event.py
+-rw-rw-rw-   0        0        0     1370 2023-05-07 00:52:16.000000 hagworm-5.5.2/hagworm/extend/asyncio/file.py
+-rw-rw-rw-   0        0        0     4232 2023-03-01 02:07:14.000000 hagworm-5.5.2/hagworm/extend/asyncio/future.py
+-rw-rw-rw-   0        0        0     2603 2023-03-01 02:07:14.000000 hagworm-5.5.2/hagworm/extend/asyncio/mail.py
+-rw-rw-rw-   0        0        0     3897 2023-03-01 02:07:14.000000 hagworm-5.5.2/hagworm/extend/asyncio/mongo.py
+-rw-rw-rw-   0        0        0    15022 2023-05-07 00:52:16.000000 hagworm-5.5.2/hagworm/extend/asyncio/mysql.py
+-rw-rw-rw-   0        0        0    13489 2023-03-01 02:07:14.000000 hagworm-5.5.2/hagworm/extend/asyncio/net.py
+-rw-rw-rw-   0        0        0     4149 2023-03-01 02:07:14.000000 hagworm-5.5.2/hagworm/extend/asyncio/ntp.py
+-rw-rw-rw-   0        0        0     1570 2023-05-18 08:40:46.000000 hagworm-5.5.2/hagworm/extend/asyncio/pool.py
+-rw-rw-rw-   0        0        0    12506 2023-05-07 00:52:16.000000 hagworm-5.5.2/hagworm/extend/asyncio/redis.py
+-rw-rw-rw-   0        0        0     7279 2023-05-11 03:07:54.000000 hagworm-5.5.2/hagworm/extend/asyncio/socket.py
+-rw-rw-rw-   0        0        0     6170 2023-04-11 07:28:18.000000 hagworm-5.5.2/hagworm/extend/asyncio/task.py
+-rw-rw-rw-   0        0        0     1360 2023-03-01 02:07:14.000000 hagworm-5.5.2/hagworm/extend/asyncio/transaction.py
+-rw-rw-rw-   0        0        0     3792 2023-03-01 02:07:14.000000 hagworm-5.5.2/hagworm/extend/asyncio/zmq.py
+-rw-rw-rw-   0        0        0    22623 2023-05-11 03:07:54.000000 hagworm-5.5.2/hagworm/extend/base.py
+-rw-rw-rw-   0        0        0     2365 2023-03-01 02:07:14.000000 hagworm-5.5.2/hagworm/extend/cache.py
+-rw-rw-rw-   0        0        0     1839 2023-05-07 00:52:16.000000 hagworm-5.5.2/hagworm/extend/compile.py
+-rw-rw-rw-   0        0        0     3857 2023-03-01 02:07:14.000000 hagworm-5.5.2/hagworm/extend/config.py
+-rw-rw-rw-   0        0        0     1487 2023-03-01 02:07:14.000000 hagworm-5.5.2/hagworm/extend/crypto.py
+-rw-rw-rw-   0        0        0     1792 2023-05-07 00:52:16.000000 hagworm-5.5.2/hagworm/extend/error.py
+-rw-rw-rw-   0        0        0     1220 2023-03-01 02:07:14.000000 hagworm-5.5.2/hagworm/extend/event.py
+-rw-rw-rw-   0        0        0     4558 2023-05-07 00:52:16.000000 hagworm-5.5.2/hagworm/extend/igraph.py
+-rw-rw-rw-   0        0        0     2326 2023-05-07 00:52:16.000000 hagworm-5.5.2/hagworm/extend/interface.py
+-rw-rw-rw-   0        0        0    14870 2023-05-13 05:06:56.000000 hagworm-5.5.2/hagworm/extend/logging.py
+-rw-rw-rw-   0        0        0     1791 2023-03-01 02:07:14.000000 hagworm-5.5.2/hagworm/extend/media.py
+-rw-rw-rw-   0        0        0     1603 2023-05-10 07:58:09.000000 hagworm-5.5.2/hagworm/extend/metaclass.py
+-rw-rw-rw-   0        0        0     4500 2023-05-11 03:07:54.000000 hagworm-5.5.2/hagworm/extend/process.py
+-rw-rw-rw-   0        0        0      551 2023-03-01 02:07:14.000000 hagworm-5.5.2/hagworm/extend/qrcode.py
+-rw-rw-rw-   0        0        0     7235 2023-05-07 00:52:16.000000 hagworm-5.5.2/hagworm/extend/struct.py
+-rw-rw-rw-   0        0        0     3758 2023-05-07 00:52:16.000000 hagworm-5.5.2/hagworm/extend/text.py
+-rw-rw-rw-   0        0        0     2409 2023-03-01 02:07:14.000000 hagworm-5.5.2/hagworm/extend/trace.py
+-rw-rw-rw-   0        0        0     2677 2023-03-01 02:07:14.000000 hagworm-5.5.2/hagworm/extend/transaction.py
+-rw-rw-rw-   0        0        0     6411 2023-03-01 02:07:14.000000 hagworm-5.5.2/hagworm/extend/validator.py
+drwxrwxrwx   0        0        0        0 2023-05-18 11:19:47.434363 hagworm-5.5.2/hagworm/frame/
+-rw-rw-rw-   0        0        0       58 2023-03-01 02:07:14.000000 hagworm-5.5.2/hagworm/frame/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-18 11:19:47.442362 hagworm-5.5.2/hagworm/frame/fastapi/
+-rw-rw-rw-   0        0        0       58 2023-03-01 02:07:14.000000 hagworm-5.5.2/hagworm/frame/fastapi/__init__.py
+-rw-rw-rw-   0        0        0     8148 2023-05-07 00:52:16.000000 hagworm-5.5.2/hagworm/frame/fastapi/base.py
+-rw-rw-rw-   0        0        0     8494 2023-03-01 02:07:14.000000 hagworm-5.5.2/hagworm/frame/fastapi/field.py
+-rw-rw-rw-   0        0        0     1389 2023-03-01 02:07:14.000000 hagworm-5.5.2/hagworm/frame/fastapi/model.py
+-rw-rw-rw-   0        0        0     1000 2023-03-01 02:07:14.000000 hagworm-5.5.2/hagworm/frame/fastapi/response.py
+-rw-rw-rw-   0        0        0     1304 2023-03-01 02:07:14.000000 hagworm-5.5.2/hagworm/frame/gunicorn.py
+-rw-rw-rw-   0        0        0     3846 2023-05-11 03:07:54.000000 hagworm-5.5.2/hagworm/frame/stress_tests.py
+drwxrwxrwx   0        0        0        0 2023-05-18 11:19:47.445362 hagworm-5.5.2/hagworm/static/
+-rw-rw-rw-   0        0        0       58 2023-03-01 02:07:14.000000 hagworm-5.5.2/hagworm/static/__init__.py
+-rw-rw-rw-   0        0        0   208075 2023-03-01 02:07:14.000000 hagworm-5.5.2/hagworm/static/cacert.pem
+drwxrwxrwx   0        0        0        0 2023-05-18 11:19:47.446362 hagworm-5.5.2/hagworm/third/
+-rw-rw-rw-   0        0        0       58 2023-03-01 02:07:14.000000 hagworm-5.5.2/hagworm/third/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-18 11:19:47.449362 hagworm-5.5.2/hagworm/third/consul/
+-rw-rw-rw-   0        0        0       58 2023-03-01 02:07:14.000000 hagworm-5.5.2/hagworm/third/consul/__init__.py
+-rw-rw-rw-   0        0        0     1288 2023-03-01 02:07:14.000000 hagworm-5.5.2/hagworm/third/consul/config.py
+drwxrwxrwx   0        0        0        0 2023-05-18 11:19:47.455362 hagworm-5.5.2/hagworm/third/rabbitmq/
+-rw-rw-rw-   0        0        0       58 2023-03-01 02:07:14.000000 hagworm-5.5.2/hagworm/third/rabbitmq/__init__.py
+-rw-rw-rw-   0        0        0     3564 2023-05-07 00:52:16.000000 hagworm-5.5.2/hagworm/third/rabbitmq/consume.py
+-rw-rw-rw-   0        0        0     5350 2023-03-01 02:07:14.000000 hagworm-5.5.2/hagworm/third/rabbitmq/publish.py
+-rw-rw-rw-   0        0        0     5743 2023-04-12 08:59:35.000000 hagworm-5.5.2/hagworm/third/rabbitmq/rpc.py
+drwxrwxrwx   0        0        0        0 2023-05-18 11:19:47.373362 hagworm-5.5.2/hagworm.egg-info/
+-rw-rw-rw-   0        0        0     7515 2023-05-18 11:19:47.000000 hagworm-5.5.2/hagworm.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2195 2023-05-18 11:19:47.000000 hagworm-5.5.2/hagworm.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-18 11:19:47.000000 hagworm-5.5.2/hagworm.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      678 2023-05-18 11:19:47.000000 hagworm-5.5.2/hagworm.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-05-18 11:19:47.000000 hagworm-5.5.2/hagworm.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-18 11:19:47.457363 hagworm-5.5.2/setup.cfg
+-rw-rw-rw-   0        0        0     2336 2023-05-18 08:48:32.000000 hagworm-5.5.2/setup.py
```

### Comparing `hagworm-5.5.1/LICENSE` & `hagworm-5.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `hagworm-5.5.1/PKG-INFO` & `hagworm-5.5.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hagworm
-Version: 5.5.1
+Version: 5.5.2
 Summary: Network Development Suite
 Home-page: https://gitee.com/wsb310/hagworm
 Author: Shaobo.Wang
 Author-email: wsb310@gmail.com
 License: Apache License Version 2.0
 Description: # Hagworm
         
@@ -127,9 +127,9 @@
         * 本项目任何版本不保证没有BUG，商业使用请自行承担风险
         * 如果有任何问题，欢迎与我联系，邮箱wsb310@gmail.com，微信号wsb310
         
 Platform: all
 Classifier: Programming Language :: Python :: 3.8
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: POSIX :: Linux
-Requires-Python: >= 3.8
+Requires-Python: >=3.9, <3.10
 Description-Content-Type: text/markdown
```

### Comparing `hagworm-5.5.1/README.md` & `hagworm-5.5.2/README.md`

 * *Files identical despite different names*

### Comparing `hagworm-5.5.1/c_extend/math.c` & `hagworm-5.5.2/c_extend/math.c`

 * *Files identical despite different names*

### Comparing `hagworm-5.5.1/example/fastapi_demo/gunicorn.config.py` & `hagworm-5.5.2/example/fastapi_demo/gunicorn.config.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.5.1/example/fastapi_demo/main.py` & `hagworm-5.5.2/example/fastapi_demo/main.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.5.1/example/fastapi_demo/service/__init__.py` & `hagworm-5.5.2/example/fastapi_demo/service/__init__.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.5.1/example/fastapi_demo/setting.py` & `hagworm-5.5.2/example/fastapi_demo/setting.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.5.1/example/main_test.py` & `hagworm-5.5.2/example/main_test.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.5.1/hagworm/extend/asyncio/base.py` & `hagworm-5.5.2/hagworm/extend/asyncio/base.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.5.1/hagworm/extend/asyncio/buffer.py` & `hagworm-5.5.2/hagworm/extend/asyncio/buffer.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.5.1/hagworm/extend/asyncio/command.py` & `hagworm-5.5.2/hagworm/extend/asyncio/command.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.5.1/hagworm/extend/asyncio/etcd.py` & `hagworm-5.5.2/hagworm/extend/asyncio/etcd.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,51 +1,98 @@
 # -*- coding: utf-8 -*-
 
 __author__ = r'wsb310@gmail.com'
 
+import asyncio
+
 from contextlib import asynccontextmanager
-from async_etcd3gw import AsyncEtcd3Client, AsyncLock
+from async_etcd3gw import AsyncEtcd3Client as _AsyncEtcd3Client, AsyncLock as _AsyncLock
 from async_etcd3gw.async_client import DEFAULT_PORT, DEFAULT_PROTOCOL, DEFAULT_API_PATH
 
 from .pool import ObjectPool
 
 
+DEFAULT_TIMEOUT = 60
+
+
+class AsyncEtcd3Client(_AsyncEtcd3Client):
+
+    async def lock(self, name, ttl=DEFAULT_TIMEOUT):
+        return AsyncLock(name, ttl=ttl, async_client=self)
+
+
+class AsyncLock(_AsyncLock):
+
+    async def acquire(self, timeout=None):
+
+        if timeout is None:
+            return await super().acquire()
+        else:
+            return await asyncio.wait_for(self._acquire(), timeout)
+
+    async def _acquire(self):
+
+        while not (result := await super().acquire()):
+
+            events, cancel = await self.async_client.watch(self.key)
+
+            async for event in events:
+
+                if event.get(r'type') == r'DELETE':
+                    await cancel()
+                    break
+
+        return result
+
+    async def __aenter__(self):
+        return self
+
+
 class Etcd3ClientPool(ObjectPool):
 
     def __init__(
         self, maxsize, host, *,
         port=DEFAULT_PORT,
         protocol=DEFAULT_PROTOCOL,
         ca_cert=None,
         cert_key=None,
         cert_cert=None,
         timeout=None,
         api_path=DEFAULT_API_PATH,
         key_prefix=None
     ):
 
-        super().__init__(maxsize, key_prefix)
+        super().__init__(maxsize)
 
         self._config = {
             r'host': host,
             r'port': port,
             r'protocol': protocol,
             r'ca_cert': ca_cert,
             r'cert_key': cert_key,
             r'cert_cert': cert_cert,
             r'timeout': timeout,
             r'api_path': api_path,
         }
 
+        self._key_prefix = key_prefix
+
     async def _create_obj(self) -> AsyncEtcd3Client:
 
         return AsyncEtcd3Client(**self._config)
 
     async def _delete_obj(self, obj: AsyncEtcd3Client):
 
         await obj.close()
 
+    def key(self, _key):
+
+        if self._key_prefix:
+            return f'{self._key_prefix}{_key}'
+        else:
+            return _key
+
     @asynccontextmanager
-    async def lock(self, name, ttl=60) -> AsyncLock:
+    async def lock(self, name, ttl=DEFAULT_TIMEOUT) -> AsyncLock:
 
         async with self.get() as client, await client.lock(self.key(name), ttl) as lock:
             yield lock
```

### Comparing `hagworm-5.5.1/hagworm/extend/asyncio/event.py` & `hagworm-5.5.2/hagworm/extend/asyncio/event.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.5.1/hagworm/extend/asyncio/file.py` & `hagworm-5.5.2/hagworm/extend/asyncio/file.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.5.1/hagworm/extend/asyncio/future.py` & `hagworm-5.5.2/hagworm/extend/asyncio/future.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.5.1/hagworm/extend/asyncio/mail.py` & `hagworm-5.5.2/hagworm/extend/asyncio/mail.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.5.1/hagworm/extend/asyncio/mongo.py` & `hagworm-5.5.2/hagworm/extend/asyncio/mongo.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.5.1/hagworm/extend/asyncio/mysql.py` & `hagworm-5.5.2/hagworm/extend/asyncio/mysql.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.5.1/hagworm/extend/asyncio/net.py` & `hagworm-5.5.2/hagworm/extend/asyncio/net.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.5.1/hagworm/extend/asyncio/ntp.py` & `hagworm-5.5.2/hagworm/extend/asyncio/ntp.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.5.1/hagworm/extend/asyncio/pool.py` & `hagworm-5.5.2/hagworm/extend/asyncio/pool.py`

 * *Files 20% similar despite different names*

```diff
@@ -8,17 +8,15 @@
 from hagworm.extend.base import Utils
 
 
 class ObjectPool:
     """对象池实现
     """
 
-    def __init__(self, maxsize, key_prefix=None):
-
-        self._key_prefix = key_prefix
+    def __init__(self, maxsize):
 
         self._queue = Queue(maxsize=maxsize)
 
     async def _create_obj(self):
 
         raise NotImplementedError()
 
@@ -43,21 +41,14 @@
             )
 
     @property
     def size(self):
 
         return self._queue.qsize()
 
-    def key(self, _key):
-
-        if self._key_prefix:
-            return f'{self._key_prefix}/{_key}'
-        else:
-            return _key
-
     @asynccontextmanager
     async def get(self):
 
         Utils.log.debug(f'ObjectPool {type(self)} size: {self._queue.qsize()}')
 
         obj = await self._queue.get()
```

### Comparing `hagworm-5.5.1/hagworm/extend/asyncio/redis.py` & `hagworm-5.5.2/hagworm/extend/asyncio/redis.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.5.1/hagworm/extend/asyncio/socket.py` & `hagworm-5.5.2/hagworm/extend/asyncio/socket.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.5.1/hagworm/extend/asyncio/task.py` & `hagworm-5.5.2/hagworm/extend/asyncio/task.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.5.1/hagworm/extend/asyncio/transaction.py` & `hagworm-5.5.2/hagworm/extend/asyncio/transaction.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.5.1/hagworm/extend/asyncio/zmq.py` & `hagworm-5.5.2/hagworm/extend/asyncio/zmq.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.5.1/hagworm/extend/base.py` & `hagworm-5.5.2/hagworm/extend/base.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.5.1/hagworm/extend/cache.py` & `hagworm-5.5.2/hagworm/extend/cache.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.5.1/hagworm/extend/compile.py` & `hagworm-5.5.2/hagworm/extend/compile.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.5.1/hagworm/extend/config.py` & `hagworm-5.5.2/hagworm/extend/config.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.5.1/hagworm/extend/crypto.py` & `hagworm-5.5.2/hagworm/extend/crypto.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.5.1/hagworm/extend/error.py` & `hagworm-5.5.2/hagworm/extend/error.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.5.1/hagworm/extend/event.py` & `hagworm-5.5.2/hagworm/extend/event.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.5.1/hagworm/extend/igraph.py` & `hagworm-5.5.2/hagworm/extend/igraph.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.5.1/hagworm/extend/interface.py` & `hagworm-5.5.2/hagworm/extend/interface.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.5.1/hagworm/extend/logging.py` & `hagworm-5.5.2/hagworm/extend/logging.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.5.1/hagworm/extend/media.py` & `hagworm-5.5.2/hagworm/extend/media.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.5.1/hagworm/extend/metaclass.py` & `hagworm-5.5.2/hagworm/extend/metaclass.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.5.1/hagworm/extend/process.py` & `hagworm-5.5.2/hagworm/extend/process.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.5.1/hagworm/extend/qrcode.py` & `hagworm-5.5.2/hagworm/extend/qrcode.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.5.1/hagworm/extend/struct.py` & `hagworm-5.5.2/hagworm/extend/struct.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.5.1/hagworm/extend/text.py` & `hagworm-5.5.2/hagworm/extend/text.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.5.1/hagworm/extend/trace.py` & `hagworm-5.5.2/hagworm/extend/trace.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.5.1/hagworm/extend/transaction.py` & `hagworm-5.5.2/hagworm/extend/transaction.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.5.1/hagworm/extend/validator.py` & `hagworm-5.5.2/hagworm/extend/validator.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.5.1/hagworm/frame/fastapi/base.py` & `hagworm-5.5.2/hagworm/frame/fastapi/base.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.5.1/hagworm/frame/fastapi/field.py` & `hagworm-5.5.2/hagworm/frame/fastapi/field.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.5.1/hagworm/frame/fastapi/model.py` & `hagworm-5.5.2/hagworm/frame/fastapi/model.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.5.1/hagworm/frame/fastapi/response.py` & `hagworm-5.5.2/hagworm/frame/fastapi/response.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.5.1/hagworm/frame/gunicorn.py` & `hagworm-5.5.2/hagworm/frame/gunicorn.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.5.1/hagworm/frame/stress_tests.py` & `hagworm-5.5.2/hagworm/frame/stress_tests.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.5.1/hagworm/static/cacert.pem` & `hagworm-5.5.2/hagworm/static/cacert.pem`

 * *Files identical despite different names*

### Comparing `hagworm-5.5.1/hagworm/third/consul/config.py` & `hagworm-5.5.2/hagworm/third/consul/config.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.5.1/hagworm/third/rabbitmq/consume.py` & `hagworm-5.5.2/hagworm/third/rabbitmq/consume.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.5.1/hagworm/third/rabbitmq/publish.py` & `hagworm-5.5.2/hagworm/third/rabbitmq/publish.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.5.1/hagworm/third/rabbitmq/rpc.py` & `hagworm-5.5.2/hagworm/third/rabbitmq/rpc.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.5.1/hagworm.egg-info/PKG-INFO` & `hagworm-5.5.2/hagworm.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hagworm
-Version: 5.5.1
+Version: 5.5.2
 Summary: Network Development Suite
 Home-page: https://gitee.com/wsb310/hagworm
 Author: Shaobo.Wang
 Author-email: wsb310@gmail.com
 License: Apache License Version 2.0
 Description: # Hagworm
         
@@ -127,9 +127,9 @@
         * 本项目任何版本不保证没有BUG，商业使用请自行承担风险
         * 如果有任何问题，欢迎与我联系，邮箱wsb310@gmail.com，微信号wsb310
         
 Platform: all
 Classifier: Programming Language :: Python :: 3.8
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: POSIX :: Linux
-Requires-Python: >= 3.8
+Requires-Python: >=3.9, <3.10
 Description-Content-Type: text/markdown
```

### Comparing `hagworm-5.5.1/hagworm.egg-info/SOURCES.txt` & `hagworm-5.5.2/hagworm.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 LICENSE
 README.md
 setup.py
 ./c_extend/math.c
-c_extend/math.c
 example/__init__.py
 example/main_test.py
 example/fastapi_demo/__init__.py
 example/fastapi_demo/gunicorn.config.py
 example/fastapi_demo/main.py
 example/fastapi_demo/setting.py
 example/fastapi_demo/controller/__init__.py
```

### Comparing `hagworm-5.5.1/hagworm.egg-info/requires.txt` & `hagworm-5.5.2/hagworm.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `hagworm-5.5.1/setup.py` & `hagworm-5.5.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     author_email=r'wsb310@gmail.com',
     description=r'Network Development Suite',
     long_description=long_description,
     long_description_content_type=r'text/markdown',
     url=r'https://gitee.com/wsb310/hagworm',
     packages=setuptools.find_packages(),
     package_data={r'hagworm': [r'static/*.*']},
-    python_requires=r'>= 3.8',
+    python_requires=r'>=3.9, <3.10',
     install_requires=[
         r'APScheduler==3.9.1',
         r'Pillow==9.0.1',
         r'PyJWT==2.3.0',
         r'PyYAML==6.0',
         r'SQLAlchemy==1.3.24',
         r'aredis==1.1.8',
```

