# Comparing `tmp/python-irodsclient-1.1.7.tar.gz` & `tmp/python-irodsclient-1.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-irodsclient-1.1.7.tar", last modified: Tue Mar 28 18:16:12 2023, max compression
+gzip compressed data, was "python-irodsclient-1.1.8.tar", last modified: Thu May 18 18:04:10 2023, max compression
```

## Comparing `python-irodsclient-1.1.7.tar` & `python-irodsclient-1.1.8.tar`

### file list

```diff
@@ -1,93 +1,93 @@
-drwxrwxr-x   0 tgr       (1000) tgr       (1000)        0 2023-03-28 18:16:12.366535 python-irodsclient-1.1.7/
--rw-rw-r--   0 tgr       (1000) tgr       (1000)      595 2018-05-02 17:12:27.000000 python-irodsclient-1.1.7/AUTHORS
--rw-rw-r--   0 tgr       (1000) tgr       (1000)    33456 2023-03-28 18:07:33.000000 python-irodsclient-1.1.7/CHANGELOG.rst
--rw-rw-r--   0 tgr       (1000) tgr       (1000)     2120 2018-02-12 13:07:26.000000 python-irodsclient-1.1.7/LICENSE.txt
--rw-rw-r--   0 tgr       (1000) tgr       (1000)      133 2021-11-24 16:13:23.000000 python-irodsclient-1.1.7/MANIFEST.in
--rw-rw-r--   0 tgr       (1000) tgr       (1000)    64164 2023-03-28 18:16:12.366535 python-irodsclient-1.1.7/PKG-INFO
--rw-rw-r--   0 tgr       (1000) tgr       (1000)    53209 2023-03-26 15:27:35.000000 python-irodsclient-1.1.7/README.rst
-drwxrwxr-x   0 tgr       (1000) tgr       (1000)        0 2023-03-28 18:16:12.358535 python-irodsclient-1.1.7/irods/
--rw-rw-r--   0 tgr       (1000) tgr       (1000)     1366 2021-11-24 16:13:23.000000 python-irodsclient-1.1.7/irods/__init__.py
--rw-rw-r--   0 tgr       (1000) tgr       (1000)     3556 2023-01-19 02:36:57.000000 python-irodsclient-1.1.7/irods/access.py
--rw-rw-r--   0 tgr       (1000) tgr       (1000)     1046 2018-02-04 01:59:15.000000 python-irodsclient-1.1.7/irods/account.py
--rw-rw-r--   0 tgr       (1000) tgr       (1000)     5395 2021-11-24 16:13:23.000000 python-irodsclient-1.1.7/irods/api_number.py
--rw-rw-r--   0 tgr       (1000) tgr       (1000)      995 2018-02-04 01:59:15.000000 python-irodsclient-1.1.7/irods/client_server_negotiation.py
--rw-rw-r--   0 tgr       (1000) tgr       (1000)     3949 2022-03-15 19:53:36.000000 python-irodsclient-1.1.7/irods/collection.py
--rw-rw-r--   0 tgr       (1000) tgr       (1000)     3618 2021-11-24 16:13:23.000000 python-irodsclient-1.1.7/irods/column.py
--rw-rw-r--   0 tgr       (1000) tgr       (1000)    22332 2022-11-19 16:34:10.000000 python-irodsclient-1.1.7/irods/connection.py
--rw-rw-r--   0 tgr       (1000) tgr       (1000)       79 2016-01-07 14:03:09.000000 python-irodsclient-1.1.7/irods/constants.py
--rw-rw-r--   0 tgr       (1000) tgr       (1000)     7200 2022-06-29 02:45:53.000000 python-irodsclient-1.1.7/irods/data_object.py
--rw-rw-r--   0 tgr       (1000) tgr       (1000)    39162 2023-03-26 15:27:35.000000 python-irodsclient-1.1.7/irods/exception.py
--rw-rw-r--   0 tgr       (1000) tgr       (1000)    10060 2022-01-20 20:46:12.000000 python-irodsclient-1.1.7/irods/keywords.py
-drwxrwxr-x   0 tgr       (1000) tgr       (1000)        0 2023-03-28 18:16:12.358535 python-irodsclient-1.1.7/irods/manager/
--rw-rw-r--   0 tgr       (1000) tgr       (1000)      469 2021-11-24 16:13:23.000000 python-irodsclient-1.1.7/irods/manager/__init__.py
--rw-rw-r--   0 tgr       (1000) tgr       (1000)     6389 2023-03-26 15:27:35.000000 python-irodsclient-1.1.7/irods/manager/access_manager.py
--rw-rw-r--   0 tgr       (1000) tgr       (1000)     5072 2022-03-15 19:53:36.000000 python-irodsclient-1.1.7/irods/manager/collection_manager.py
--rw-rw-r--   0 tgr       (1000) tgr       (1000)    23174 2023-03-28 18:06:05.000000 python-irodsclient-1.1.7/irods/manager/data_object_manager.py
--rw-rw-r--   0 tgr       (1000) tgr       (1000)     7119 2022-09-21 18:23:05.000000 python-irodsclient-1.1.7/irods/manager/metadata_manager.py
--rw-rw-r--   0 tgr       (1000) tgr       (1000)     5329 2018-02-04 01:59:15.000000 python-irodsclient-1.1.7/irods/manager/resource_manager.py
--rw-rw-r--   0 tgr       (1000) tgr       (1000)    12007 2023-03-26 15:27:35.000000 python-irodsclient-1.1.7/irods/manager/user_manager.py
--rw-rw-r--   0 tgr       (1000) tgr       (1000)     1593 2021-11-24 16:13:23.000000 python-irodsclient-1.1.7/irods/manager/zone_manager.py
-drwxrwxr-x   0 tgr       (1000) tgr       (1000)        0 2023-03-28 18:16:12.358535 python-irodsclient-1.1.7/irods/message/
--rw-rw-r--   0 tgr       (1000) tgr       (1000)    36963 2023-03-28 18:06:05.000000 python-irodsclient-1.1.7/irods/message/__init__.py
--rw-rw-r--   0 tgr       (1000) tgr       (1000)     1222 2017-04-05 17:18:12.000000 python-irodsclient-1.1.7/irods/message/message.py
--rw-rw-r--   0 tgr       (1000) tgr       (1000)     1167 2017-04-05 17:18:12.000000 python-irodsclient-1.1.7/irods/message/ordered.py
--rw-rw-r--   0 tgr       (1000) tgr       (1000)     3378 2018-09-27 03:15:27.000000 python-irodsclient-1.1.7/irods/message/property.py
--rw-rw-r--   0 tgr       (1000) tgr       (1000)     5592 2022-01-20 20:46:12.000000 python-irodsclient-1.1.7/irods/message/quasixml.py
--rw-rw-r--   0 tgr       (1000) tgr       (1000)     5930 2022-09-21 18:23:05.000000 python-irodsclient-1.1.7/irods/meta.py
--rw-rw-r--   0 tgr       (1000) tgr       (1000)    11131 2023-03-26 15:27:35.000000 python-irodsclient-1.1.7/irods/models.py
--rw-rw-r--   0 tgr       (1000) tgr       (1000)    22154 2022-03-15 19:53:36.000000 python-irodsclient-1.1.7/irods/parallel.py
--rw-rw-r--   0 tgr       (1000) tgr       (1000)     9946 2023-03-26 15:27:35.000000 python-irodsclient-1.1.7/irods/password_obfuscation.py
-drwxrwxr-x   0 tgr       (1000) tgr       (1000)        0 2023-03-28 18:16:12.358535 python-irodsclient-1.1.7/irods/path/
--rw-rw-r--   0 tgr       (1000) tgr       (1000)     3331 2022-09-21 18:23:05.000000 python-irodsclient-1.1.7/irods/path/__init__.py
--rw-rw-r--   0 tgr       (1000) tgr       (1000)     4445 2022-11-19 16:34:10.000000 python-irodsclient-1.1.7/irods/pool.py
--rw-rw-r--   0 tgr       (1000) tgr       (1000)    11022 2021-11-24 16:13:23.000000 python-irodsclient-1.1.7/irods/query.py
--rw-rw-r--   0 tgr       (1000) tgr       (1000)     4768 2023-01-19 02:36:57.000000 python-irodsclient-1.1.7/irods/resource.py
--rw-rw-r--   0 tgr       (1000) tgr       (1000)     3127 2022-01-20 20:46:55.000000 python-irodsclient-1.1.7/irods/results.py
--rw-rw-r--   0 tgr       (1000) tgr       (1000)     7443 2022-01-31 14:40:33.000000 python-irodsclient-1.1.7/irods/rule.py
--rw-rw-r--   0 tgr       (1000) tgr       (1000)    13508 2023-03-26 15:27:35.000000 python-irodsclient-1.1.7/irods/session.py
-drwxrwxr-x   0 tgr       (1000) tgr       (1000)        0 2023-03-28 18:16:12.362535 python-irodsclient-1.1.7/irods/test/
--rw-rw-r--   0 tgr       (1000) tgr       (1000)      726 2018-02-04 01:59:15.000000 python-irodsclient-1.1.7/irods/test/README.rst
--rw-rw-r--   0 tgr       (1000) tgr       (1000)        0 2014-09-05 15:54:22.000000 python-irodsclient-1.1.7/irods/test/__init__.py
--rw-rw-r--   0 tgr       (1000) tgr       (1000)    16120 2023-03-26 15:27:35.000000 python-irodsclient-1.1.7/irods/test/access_test.py
--rw-rw-r--   0 tgr       (1000) tgr       (1000)    14819 2023-03-26 15:27:35.000000 python-irodsclient-1.1.7/irods/test/admin_test.py
--rw-rw-r--   0 tgr       (1000) tgr       (1000)    13309 2022-03-15 19:53:36.000000 python-irodsclient-1.1.7/irods/test/collection_test.py
--rw-rw-r--   0 tgr       (1000) tgr       (1000)     2320 2023-01-19 02:36:57.000000 python-irodsclient-1.1.7/irods/test/connection_test.py
--rw-rw-r--   0 tgr       (1000) tgr       (1000)    70274 2023-03-28 18:06:05.000000 python-irodsclient-1.1.7/irods/test/data_obj_test.py
--rw-rw-r--   0 tgr       (1000) tgr       (1000)     1832 2023-01-19 02:36:57.000000 python-irodsclient-1.1.7/irods/test/exception_test.py
--rw-rw-r--   0 tgr       (1000) tgr       (1000)     2879 2021-11-24 16:13:23.000000 python-irodsclient-1.1.7/irods/test/extended_test.py
--rw-rw-r--   0 tgr       (1000) tgr       (1000)     2660 2018-02-04 01:59:15.000000 python-irodsclient-1.1.7/irods/test/file_test.py
--rw-rw-r--   0 tgr       (1000) tgr       (1000)     1599 2021-11-24 16:13:23.000000 python-irodsclient-1.1.7/irods/test/force_create.py
--rw-rw-r--   0 tgr       (1000) tgr       (1000)     9047 2023-01-19 02:36:57.000000 python-irodsclient-1.1.7/irods/test/helpers.py
--rw-rw-r--   0 tgr       (1000) tgr       (1000)    22120 2023-03-26 15:27:35.000000 python-irodsclient-1.1.7/irods/test/login_auth_test.py
--rw-rw-r--   0 tgr       (1000) tgr       (1000)     7198 2022-01-20 20:46:12.000000 python-irodsclient-1.1.7/irods/test/message_test.py
--rw-rw-r--   0 tgr       (1000) tgr       (1000)    17764 2023-03-28 18:06:05.000000 python-irodsclient-1.1.7/irods/test/meta_test.py
--rw-rw-r--   0 tgr       (1000) tgr       (1000)    15503 2022-03-15 19:53:36.000000 python-irodsclient-1.1.7/irods/test/pool_test.py
--rw-rw-r--   0 tgr       (1000) tgr       (1000)    27994 2022-01-20 20:46:55.000000 python-irodsclient-1.1.7/irods/test/query_test.py
--rw-rw-r--   0 tgr       (1000) tgr       (1000)     3032 2023-01-19 02:36:57.000000 python-irodsclient-1.1.7/irods/test/resource_test.py
--rw-rw-r--   0 tgr       (1000) tgr       (1000)    14829 2022-01-31 14:40:33.000000 python-irodsclient-1.1.7/irods/test/rule_test.py
--rw-rw-r--   0 tgr       (1000) tgr       (1000)     1139 2017-09-03 17:28:09.000000 python-irodsclient-1.1.7/irods/test/runner.py
--rwxrwxr-x   0 tgr       (1000) tgr       (1000)     2827 2022-11-19 16:34:10.000000 python-irodsclient-1.1.7/irods/test/setupssl.py
--rw-rw-r--   0 tgr       (1000) tgr       (1000)      457 2022-11-19 16:34:10.000000 python-irodsclient-1.1.7/irods/test/ssl_test_client.py
--rw-rw-r--   0 tgr       (1000) tgr       (1000)     2866 2021-11-24 16:13:23.000000 python-irodsclient-1.1.7/irods/test/temp_password_test.py
-drwxrwxr-x   0 tgr       (1000) tgr       (1000)        0 2023-03-28 18:16:12.362535 python-irodsclient-1.1.7/irods/test/test-data/
--rw-rw-r--   0 tgr       (1000) tgr       (1000)      168 2021-11-24 16:13:23.000000 python-irodsclient-1.1.7/irods/test/test-data/irods_environment.json
--rw-rw-r--   0 tgr       (1000) tgr       (1000)      169 2021-11-24 16:13:23.000000 python-irodsclient-1.1.7/irods/test/test-data/irods_environment_negative_refresh_field.json
--rw-rw-r--   0 tgr       (1000) tgr       (1000)      126 2021-11-24 16:13:23.000000 python-irodsclient-1.1.7/irods/test/test-data/irods_environment_no_refresh_field.json
--rw-rw-r--   0 tgr       (1000) tgr       (1000)     3528 2022-09-21 18:23:05.000000 python-irodsclient-1.1.7/irods/test/test_paths.py
--rw-rw-r--   0 tgr       (1000) tgr       (1000)    15137 2022-09-21 18:23:05.000000 python-irodsclient-1.1.7/irods/test/ticket_test.py
--rw-rw-r--   0 tgr       (1000) tgr       (1000)    26095 2016-01-07 14:03:09.000000 python-irodsclient-1.1.7/irods/test/unicode_sampler.xml
--rw-rw-r--   0 tgr       (1000) tgr       (1000)     3920 2022-01-20 20:46:55.000000 python-irodsclient-1.1.7/irods/test/unicode_test.py
--rw-rw-r--   0 tgr       (1000) tgr       (1000)    16734 2023-03-26 15:27:35.000000 python-irodsclient-1.1.7/irods/test/user_group_test.py
--rw-rw-r--   0 tgr       (1000) tgr       (1000)     1932 2023-01-19 02:36:57.000000 python-irodsclient-1.1.7/irods/test/zone_test.py
--rw-rw-r--   0 tgr       (1000) tgr       (1000)     3291 2022-09-21 18:23:05.000000 python-irodsclient-1.1.7/irods/ticket.py
--rw-rw-r--   0 tgr       (1000) tgr       (1000)     3433 2023-03-26 15:27:35.000000 python-irodsclient-1.1.7/irods/user.py
--rw-rw-r--   0 tgr       (1000) tgr       (1000)       22 2023-03-28 18:06:05.000000 python-irodsclient-1.1.7/irods/version.py
--rw-rw-r--   0 tgr       (1000) tgr       (1000)      602 2021-11-24 16:13:23.000000 python-irodsclient-1.1.7/irods/zone.py
-drwxrwxr-x   0 tgr       (1000) tgr       (1000)        0 2023-03-28 18:16:12.366535 python-irodsclient-1.1.7/python_irodsclient.egg-info/
--rw-rw-r--   0 tgr       (1000) tgr       (1000)    64164 2023-03-28 18:16:12.000000 python-irodsclient-1.1.7/python_irodsclient.egg-info/PKG-INFO
--rw-rw-r--   0 tgr       (1000) tgr       (1000)     2105 2023-03-28 18:16:12.000000 python-irodsclient-1.1.7/python_irodsclient.egg-info/SOURCES.txt
--rw-rw-r--   0 tgr       (1000) tgr       (1000)        1 2023-03-28 18:16:12.000000 python-irodsclient-1.1.7/python_irodsclient.egg-info/dependency_links.txt
--rw-rw-r--   0 tgr       (1000) tgr       (1000)      110 2023-03-28 18:16:12.000000 python-irodsclient-1.1.7/python_irodsclient.egg-info/requires.txt
--rw-rw-r--   0 tgr       (1000) tgr       (1000)        6 2023-03-28 18:16:12.000000 python-irodsclient-1.1.7/python_irodsclient.egg-info/top_level.txt
--rw-rw-r--   0 tgr       (1000) tgr       (1000)       80 2023-03-28 18:16:12.366535 python-irodsclient-1.1.7/setup.cfg
--rw-rw-r--   0 tgr       (1000) tgr       (1000)     1731 2022-01-20 21:16:42.000000 python-irodsclient-1.1.7/setup.py
+drwxrwxr-x   0 tgr       (1000) tgr       (1000)        0 2023-05-18 18:04:10.221492 python-irodsclient-1.1.8/
+-rw-rw-r--   0 tgr       (1000) tgr       (1000)      595 2018-05-02 17:12:27.000000 python-irodsclient-1.1.8/AUTHORS
+-rw-rw-r--   0 tgr       (1000) tgr       (1000)    33905 2023-05-18 16:34:44.000000 python-irodsclient-1.1.8/CHANGELOG.rst
+-rw-rw-r--   0 tgr       (1000) tgr       (1000)     2120 2018-02-12 13:07:26.000000 python-irodsclient-1.1.8/LICENSE.txt
+-rw-rw-r--   0 tgr       (1000) tgr       (1000)      133 2021-11-24 16:13:23.000000 python-irodsclient-1.1.8/MANIFEST.in
+-rw-rw-r--   0 tgr       (1000) tgr       (1000)    64164 2023-05-18 18:04:10.221492 python-irodsclient-1.1.8/PKG-INFO
+-rw-rw-r--   0 tgr       (1000) tgr       (1000)    53209 2023-03-26 15:27:35.000000 python-irodsclient-1.1.8/README.rst
+drwxrwxr-x   0 tgr       (1000) tgr       (1000)        0 2023-05-18 18:04:10.213492 python-irodsclient-1.1.8/irods/
+-rw-rw-r--   0 tgr       (1000) tgr       (1000)     1366 2021-11-24 16:13:23.000000 python-irodsclient-1.1.8/irods/__init__.py
+-rw-rw-r--   0 tgr       (1000) tgr       (1000)     3556 2023-01-19 02:36:57.000000 python-irodsclient-1.1.8/irods/access.py
+-rw-rw-r--   0 tgr       (1000) tgr       (1000)     1046 2018-02-04 01:59:15.000000 python-irodsclient-1.1.8/irods/account.py
+-rw-rw-r--   0 tgr       (1000) tgr       (1000)     5395 2021-11-24 16:13:23.000000 python-irodsclient-1.1.8/irods/api_number.py
+-rw-rw-r--   0 tgr       (1000) tgr       (1000)      995 2018-02-04 01:59:15.000000 python-irodsclient-1.1.8/irods/client_server_negotiation.py
+-rw-rw-r--   0 tgr       (1000) tgr       (1000)     3949 2022-03-15 19:53:36.000000 python-irodsclient-1.1.8/irods/collection.py
+-rw-rw-r--   0 tgr       (1000) tgr       (1000)     3757 2023-05-18 16:31:52.000000 python-irodsclient-1.1.8/irods/column.py
+-rw-rw-r--   0 tgr       (1000) tgr       (1000)    22332 2022-11-19 16:34:10.000000 python-irodsclient-1.1.8/irods/connection.py
+-rw-rw-r--   0 tgr       (1000) tgr       (1000)       79 2016-01-07 14:03:09.000000 python-irodsclient-1.1.8/irods/constants.py
+-rw-rw-r--   0 tgr       (1000) tgr       (1000)     7249 2023-05-18 16:31:52.000000 python-irodsclient-1.1.8/irods/data_object.py
+-rw-rw-r--   0 tgr       (1000) tgr       (1000)    39162 2023-03-26 15:27:35.000000 python-irodsclient-1.1.8/irods/exception.py
+-rw-rw-r--   0 tgr       (1000) tgr       (1000)    10060 2022-01-20 20:46:12.000000 python-irodsclient-1.1.8/irods/keywords.py
+drwxrwxr-x   0 tgr       (1000) tgr       (1000)        0 2023-05-18 18:04:10.213492 python-irodsclient-1.1.8/irods/manager/
+-rw-rw-r--   0 tgr       (1000) tgr       (1000)      469 2021-11-24 16:13:23.000000 python-irodsclient-1.1.8/irods/manager/__init__.py
+-rw-rw-r--   0 tgr       (1000) tgr       (1000)     6389 2023-03-26 15:27:35.000000 python-irodsclient-1.1.8/irods/manager/access_manager.py
+-rw-rw-r--   0 tgr       (1000) tgr       (1000)     5072 2022-03-15 19:53:36.000000 python-irodsclient-1.1.8/irods/manager/collection_manager.py
+-rw-rw-r--   0 tgr       (1000) tgr       (1000)    23174 2023-03-28 18:06:05.000000 python-irodsclient-1.1.8/irods/manager/data_object_manager.py
+-rw-rw-r--   0 tgr       (1000) tgr       (1000)     7119 2022-09-21 18:23:05.000000 python-irodsclient-1.1.8/irods/manager/metadata_manager.py
+-rw-rw-r--   0 tgr       (1000) tgr       (1000)     5329 2018-02-04 01:59:15.000000 python-irodsclient-1.1.8/irods/manager/resource_manager.py
+-rw-rw-r--   0 tgr       (1000) tgr       (1000)    12337 2023-05-18 16:31:52.000000 python-irodsclient-1.1.8/irods/manager/user_manager.py
+-rw-rw-r--   0 tgr       (1000) tgr       (1000)     1593 2021-11-24 16:13:23.000000 python-irodsclient-1.1.8/irods/manager/zone_manager.py
+drwxrwxr-x   0 tgr       (1000) tgr       (1000)        0 2023-05-18 18:04:10.213492 python-irodsclient-1.1.8/irods/message/
+-rw-rw-r--   0 tgr       (1000) tgr       (1000)    37061 2023-05-18 16:31:52.000000 python-irodsclient-1.1.8/irods/message/__init__.py
+-rw-rw-r--   0 tgr       (1000) tgr       (1000)     1222 2017-04-05 17:18:12.000000 python-irodsclient-1.1.8/irods/message/message.py
+-rw-rw-r--   0 tgr       (1000) tgr       (1000)     1167 2017-04-05 17:18:12.000000 python-irodsclient-1.1.8/irods/message/ordered.py
+-rw-rw-r--   0 tgr       (1000) tgr       (1000)     3378 2018-09-27 03:15:27.000000 python-irodsclient-1.1.8/irods/message/property.py
+-rw-rw-r--   0 tgr       (1000) tgr       (1000)     5592 2022-01-20 20:46:12.000000 python-irodsclient-1.1.8/irods/message/quasixml.py
+-rw-rw-r--   0 tgr       (1000) tgr       (1000)     6136 2023-05-18 16:31:52.000000 python-irodsclient-1.1.8/irods/meta.py
+-rw-rw-r--   0 tgr       (1000) tgr       (1000)    11131 2023-03-26 15:27:35.000000 python-irodsclient-1.1.8/irods/models.py
+-rw-rw-r--   0 tgr       (1000) tgr       (1000)    22154 2022-03-15 19:53:36.000000 python-irodsclient-1.1.8/irods/parallel.py
+-rw-rw-r--   0 tgr       (1000) tgr       (1000)     9946 2023-03-26 15:27:35.000000 python-irodsclient-1.1.8/irods/password_obfuscation.py
+drwxrwxr-x   0 tgr       (1000) tgr       (1000)        0 2023-05-18 18:04:10.217492 python-irodsclient-1.1.8/irods/path/
+-rw-rw-r--   0 tgr       (1000) tgr       (1000)     3331 2022-09-21 18:23:05.000000 python-irodsclient-1.1.8/irods/path/__init__.py
+-rw-rw-r--   0 tgr       (1000) tgr       (1000)     4445 2022-11-19 16:34:10.000000 python-irodsclient-1.1.8/irods/pool.py
+-rw-rw-r--   0 tgr       (1000) tgr       (1000)    11022 2021-11-24 16:13:23.000000 python-irodsclient-1.1.8/irods/query.py
+-rw-rw-r--   0 tgr       (1000) tgr       (1000)     4768 2023-01-19 02:36:57.000000 python-irodsclient-1.1.8/irods/resource.py
+-rw-rw-r--   0 tgr       (1000) tgr       (1000)     3127 2022-01-20 20:46:55.000000 python-irodsclient-1.1.8/irods/results.py
+-rw-rw-r--   0 tgr       (1000) tgr       (1000)     7443 2022-01-31 14:40:33.000000 python-irodsclient-1.1.8/irods/rule.py
+-rw-rw-r--   0 tgr       (1000) tgr       (1000)    13861 2023-05-18 16:31:52.000000 python-irodsclient-1.1.8/irods/session.py
+drwxrwxr-x   0 tgr       (1000) tgr       (1000)        0 2023-05-18 18:04:10.221492 python-irodsclient-1.1.8/irods/test/
+-rw-rw-r--   0 tgr       (1000) tgr       (1000)      726 2018-02-04 01:59:15.000000 python-irodsclient-1.1.8/irods/test/README.rst
+-rw-rw-r--   0 tgr       (1000) tgr       (1000)        0 2014-09-05 15:54:22.000000 python-irodsclient-1.1.8/irods/test/__init__.py
+-rw-rw-r--   0 tgr       (1000) tgr       (1000)    16120 2023-03-26 15:27:35.000000 python-irodsclient-1.1.8/irods/test/access_test.py
+-rw-rw-r--   0 tgr       (1000) tgr       (1000)    14819 2023-03-26 15:27:35.000000 python-irodsclient-1.1.8/irods/test/admin_test.py
+-rw-rw-r--   0 tgr       (1000) tgr       (1000)    13309 2022-03-15 19:53:36.000000 python-irodsclient-1.1.8/irods/test/collection_test.py
+-rw-rw-r--   0 tgr       (1000) tgr       (1000)     4704 2023-05-18 16:31:52.000000 python-irodsclient-1.1.8/irods/test/connection_test.py
+-rw-rw-r--   0 tgr       (1000) tgr       (1000)    71132 2023-05-18 16:31:52.000000 python-irodsclient-1.1.8/irods/test/data_obj_test.py
+-rw-rw-r--   0 tgr       (1000) tgr       (1000)     1832 2023-01-19 02:36:57.000000 python-irodsclient-1.1.8/irods/test/exception_test.py
+-rw-rw-r--   0 tgr       (1000) tgr       (1000)     2879 2021-11-24 16:13:23.000000 python-irodsclient-1.1.8/irods/test/extended_test.py
+-rw-rw-r--   0 tgr       (1000) tgr       (1000)     2660 2018-02-04 01:59:15.000000 python-irodsclient-1.1.8/irods/test/file_test.py
+-rw-rw-r--   0 tgr       (1000) tgr       (1000)     1599 2021-11-24 16:13:23.000000 python-irodsclient-1.1.8/irods/test/force_create.py
+-rw-rw-r--   0 tgr       (1000) tgr       (1000)     9047 2023-01-19 02:36:57.000000 python-irodsclient-1.1.8/irods/test/helpers.py
+-rw-rw-r--   0 tgr       (1000) tgr       (1000)    22120 2023-03-26 15:27:35.000000 python-irodsclient-1.1.8/irods/test/login_auth_test.py
+-rw-rw-r--   0 tgr       (1000) tgr       (1000)     7198 2022-01-20 20:46:12.000000 python-irodsclient-1.1.8/irods/test/message_test.py
+-rw-rw-r--   0 tgr       (1000) tgr       (1000)    21699 2023-05-18 16:31:52.000000 python-irodsclient-1.1.8/irods/test/meta_test.py
+-rw-rw-r--   0 tgr       (1000) tgr       (1000)    15503 2022-03-15 19:53:36.000000 python-irodsclient-1.1.8/irods/test/pool_test.py
+-rw-rw-r--   0 tgr       (1000) tgr       (1000)    28751 2023-05-18 16:31:52.000000 python-irodsclient-1.1.8/irods/test/query_test.py
+-rw-rw-r--   0 tgr       (1000) tgr       (1000)     3032 2023-01-19 02:36:57.000000 python-irodsclient-1.1.8/irods/test/resource_test.py
+-rw-rw-r--   0 tgr       (1000) tgr       (1000)    14829 2022-01-31 14:40:33.000000 python-irodsclient-1.1.8/irods/test/rule_test.py
+-rw-rw-r--   0 tgr       (1000) tgr       (1000)     1139 2017-09-03 17:28:09.000000 python-irodsclient-1.1.8/irods/test/runner.py
+-rwxrwxr-x   0 tgr       (1000) tgr       (1000)     2827 2022-11-19 16:34:10.000000 python-irodsclient-1.1.8/irods/test/setupssl.py
+-rw-rw-r--   0 tgr       (1000) tgr       (1000)      457 2022-11-19 16:34:10.000000 python-irodsclient-1.1.8/irods/test/ssl_test_client.py
+-rw-rw-r--   0 tgr       (1000) tgr       (1000)     2866 2021-11-24 16:13:23.000000 python-irodsclient-1.1.8/irods/test/temp_password_test.py
+drwxrwxr-x   0 tgr       (1000) tgr       (1000)        0 2023-05-18 18:04:10.221492 python-irodsclient-1.1.8/irods/test/test-data/
+-rw-rw-r--   0 tgr       (1000) tgr       (1000)      168 2021-11-24 16:13:23.000000 python-irodsclient-1.1.8/irods/test/test-data/irods_environment.json
+-rw-rw-r--   0 tgr       (1000) tgr       (1000)      169 2021-11-24 16:13:23.000000 python-irodsclient-1.1.8/irods/test/test-data/irods_environment_negative_refresh_field.json
+-rw-rw-r--   0 tgr       (1000) tgr       (1000)      126 2021-11-24 16:13:23.000000 python-irodsclient-1.1.8/irods/test/test-data/irods_environment_no_refresh_field.json
+-rw-rw-r--   0 tgr       (1000) tgr       (1000)     3528 2022-09-21 18:23:05.000000 python-irodsclient-1.1.8/irods/test/test_paths.py
+-rw-rw-r--   0 tgr       (1000) tgr       (1000)    15137 2022-09-21 18:23:05.000000 python-irodsclient-1.1.8/irods/test/ticket_test.py
+-rw-rw-r--   0 tgr       (1000) tgr       (1000)    26095 2016-01-07 14:03:09.000000 python-irodsclient-1.1.8/irods/test/unicode_sampler.xml
+-rw-rw-r--   0 tgr       (1000) tgr       (1000)     3920 2022-01-20 20:46:55.000000 python-irodsclient-1.1.8/irods/test/unicode_test.py
+-rw-rw-r--   0 tgr       (1000) tgr       (1000)    22545 2023-05-18 16:31:52.000000 python-irodsclient-1.1.8/irods/test/user_group_test.py
+-rw-rw-r--   0 tgr       (1000) tgr       (1000)     1932 2023-01-19 02:36:57.000000 python-irodsclient-1.1.8/irods/test/zone_test.py
+-rw-rw-r--   0 tgr       (1000) tgr       (1000)     3291 2022-09-21 18:23:05.000000 python-irodsclient-1.1.8/irods/ticket.py
+-rw-rw-r--   0 tgr       (1000) tgr       (1000)     3487 2023-05-18 16:31:52.000000 python-irodsclient-1.1.8/irods/user.py
+-rw-rw-r--   0 tgr       (1000) tgr       (1000)       22 2023-05-18 16:32:09.000000 python-irodsclient-1.1.8/irods/version.py
+-rw-rw-r--   0 tgr       (1000) tgr       (1000)      602 2021-11-24 16:13:23.000000 python-irodsclient-1.1.8/irods/zone.py
+drwxrwxr-x   0 tgr       (1000) tgr       (1000)        0 2023-05-18 18:04:10.221492 python-irodsclient-1.1.8/python_irodsclient.egg-info/
+-rw-rw-r--   0 tgr       (1000) tgr       (1000)    64164 2023-05-18 18:04:10.000000 python-irodsclient-1.1.8/python_irodsclient.egg-info/PKG-INFO
+-rw-rw-r--   0 tgr       (1000) tgr       (1000)     2105 2023-05-18 18:04:10.000000 python-irodsclient-1.1.8/python_irodsclient.egg-info/SOURCES.txt
+-rw-rw-r--   0 tgr       (1000) tgr       (1000)        1 2023-05-18 18:04:10.000000 python-irodsclient-1.1.8/python_irodsclient.egg-info/dependency_links.txt
+-rw-rw-r--   0 tgr       (1000) tgr       (1000)      110 2023-05-18 18:04:10.000000 python-irodsclient-1.1.8/python_irodsclient.egg-info/requires.txt
+-rw-rw-r--   0 tgr       (1000) tgr       (1000)        6 2023-05-18 18:04:10.000000 python-irodsclient-1.1.8/python_irodsclient.egg-info/top_level.txt
+-rw-rw-r--   0 tgr       (1000) tgr       (1000)       80 2023-05-18 18:04:10.225492 python-irodsclient-1.1.8/setup.cfg
+-rw-rw-r--   0 tgr       (1000) tgr       (1000)     1731 2022-01-20 21:16:42.000000 python-irodsclient-1.1.8/setup.py
```

### Comparing `python-irodsclient-1.1.7/AUTHORS` & `python-irodsclient-1.1.8/AUTHORS`

 * *Files identical despite different names*

### Comparing `python-irodsclient-1.1.7/CHANGELOG.rst` & `python-irodsclient-1.1.8/CHANGELOG.rst`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,19 @@
 Changelog
 =========
 
+v1.1.8 (2023-05-18)
+-------------------
+- [#450] test for setting/getting comments [Daniel Moore]
+- [#377] fix iRODSSession connection timeout [Daniel Moore]
+- [#450] Get property comments from replica object [Gwenael Leysour de Rohello]
+- [#448] protect against bad parameters in modify_password [Daniel Moore]
+- [#442] allow non-default string types in AVU fields [Daniel Moore]
+- [#443] add NotLike (GenQuery 'NOT LIKE') operator [Daniel Moore]
+
 v1.1.7 (2023-03-28)
 -------------------
 - [#435] unregister can target a single replica [Daniel Moore]
 - [#434] metadata calls now require AVU fields to be nonzero-length strings [Daniel Moore]
 - [#431][irods/irods#6921] filter user_id results from R_OBJT_ACCESS through IDs still in R_USER_MAIN [Daniel Moore]
 - [#3] acls.set needs admin=True for some tests [Daniel Moore]
 - [#3] compatibility bump to iRODS 4.3.1 [Daniel Moore]
```

### Comparing `python-irodsclient-1.1.7/LICENSE.txt` & `python-irodsclient-1.1.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `python-irodsclient-1.1.7/PKG-INFO` & `python-irodsclient-1.1.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-irodsclient
-Version: 1.1.7
+Version: 1.1.8
 Summary: A python API for iRODS
 Home-page: https://github.com/irods/python-irodsclient
 Author: iRODS Consortium
 Author-email: support@irods.org
 License: BSD
 Description: =========================
         Python iRODS Client (PRC)
```

### Comparing `python-irodsclient-1.1.7/README.rst` & `python-irodsclient-1.1.8/README.rst`

 * *Files identical despite different names*

### Comparing `python-irodsclient-1.1.7/irods/__init__.py` & `python-irodsclient-1.1.8/irods/__init__.py`

 * *Files identical despite different names*

### Comparing `python-irodsclient-1.1.7/irods/access.py` & `python-irodsclient-1.1.8/irods/access.py`

 * *Files identical despite different names*

### Comparing `python-irodsclient-1.1.7/irods/account.py` & `python-irodsclient-1.1.8/irods/account.py`

 * *Files identical despite different names*

### Comparing `python-irodsclient-1.1.7/irods/api_number.py` & `python-irodsclient-1.1.8/irods/api_number.py`

 * *Files identical despite different names*

### Comparing `python-irodsclient-1.1.7/irods/client_server_negotiation.py` & `python-irodsclient-1.1.8/irods/client_server_negotiation.py`

 * *Files identical despite different names*

### Comparing `python-irodsclient-1.1.7/irods/collection.py` & `python-irodsclient-1.1.8/irods/collection.py`

 * *Files identical despite different names*

### Comparing `python-irodsclient-1.1.7/irods/column.py` & `python-irodsclient-1.1.8/irods/column.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,14 +56,20 @@
 
 class Like(Criterion):
 
     def __init__(self, query_key, value):
         super(Like, self).__init__('like', query_key, value)
 
 
+class NotLike(Criterion):
+
+    def __init__(self, query_key, value):
+        super(NotLike, self).__init__('not like', query_key, value)
+
+
 class Between(Criterion):
 
     def __init__(self, query_key, value):
         super(Between, self).__init__('between', query_key, value)
 
     @property
     def value(self):
```

### Comparing `python-irodsclient-1.1.7/irods/connection.py` & `python-irodsclient-1.1.8/irods/connection.py`

 * *Files identical despite different names*

### Comparing `python-irodsclient-1.1.7/irods/data_object.py` & `python-irodsclient-1.1.8/irods/data_object.py`

 * *Files 0% similar despite different names*

```diff
@@ -65,15 +65,16 @@
             self.replicas = [iRODSReplica(
                 r[DataObject.replica_number],
                 r[DataObject.replica_status],
                 r[DataObject.resource_name],
                 r[DataObject.path],
                 r[DataObject.resc_hier],
                 checksum=r[DataObject.checksum],
-                size=r[DataObject.size]
+                size=r[DataObject.size],
+                comments=r[DataObject.comments]
             ) for r in replicas]
         self._meta = None
 
 
 
 
     def __repr__(self):
```

### Comparing `python-irodsclient-1.1.7/irods/exception.py` & `python-irodsclient-1.1.8/irods/exception.py`

 * *Files identical despite different names*

### Comparing `python-irodsclient-1.1.7/irods/keywords.py` & `python-irodsclient-1.1.8/irods/keywords.py`

 * *Files identical despite different names*

### Comparing `python-irodsclient-1.1.7/irods/manager/access_manager.py` & `python-irodsclient-1.1.8/irods/manager/access_manager.py`

 * *Files identical despite different names*

### Comparing `python-irodsclient-1.1.7/irods/manager/collection_manager.py` & `python-irodsclient-1.1.8/irods/manager/collection_manager.py`

 * *Files identical despite different names*

### Comparing `python-irodsclient-1.1.7/irods/manager/data_object_manager.py` & `python-irodsclient-1.1.8/irods/manager/data_object_manager.py`

 * *Files identical despite different names*

### Comparing `python-irodsclient-1.1.7/irods/manager/metadata_manager.py` & `python-irodsclient-1.1.8/irods/manager/metadata_manager.py`

 * *Files identical despite different names*

### Comparing `python-irodsclient-1.1.7/irods/manager/resource_manager.py` & `python-irodsclient-1.1.8/irods/manager/resource_manager.py`

 * *Files identical despite different names*

### Comparing `python-irodsclient-1.1.7/irods/manager/user_manager.py` & `python-irodsclient-1.1.8/irods/manager/user_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,20 +4,20 @@
 import warnings
 
 from irods.models import User, Group
 from irods.manager import Manager
 from irods.message import UserAdminRequest, GeneralAdminRequest, iRODSMessage, GetTempPasswordForOtherRequest, GetTempPasswordForOtherOut
 from irods.exception import UserDoesNotExist, GroupDoesNotExist, NoResultFound, CAT_SQL_ERR
 from irods.api_number import api_number
-from irods.user import iRODSUser, iRODSGroup
+from irods.user import iRODSUser, iRODSGroup, Bad_password_change_parameter
 import irods.password_obfuscation as obf
+from .. import MAX_PASSWORD_LENGTH
 
 logger = logging.getLogger(__name__)
 
-
 class UserManager(Manager):
 
     def get(self, user_name, user_zone=""):
         query = self.sess.query(User).filter(User.name == user_name)
 
         if len(user_zone) > 0:
             query = query.filter(User.zone == user_zone)
@@ -130,14 +130,18 @@
             old_value - the currently valid (old) password
             new_value - the desired (new) password
             modify_irods_authentication_file - Can be False, True, or a string.  If a string, it should indicate
                                   the absolute path of an IRODS_AUTHENTICATION_FILE to be altered.
         """
         with self.sess.pool.get_connection() as conn:
 
+            if old_value != self.sess.pool.account.password or not isinstance(new_value, str) \
+                                                            or not(3 <= len(new_value) <= MAX_PASSWORD_LENGTH - 8):
+                raise Bad_password_change_parameter
+
             hash_new_value = obf.obfuscate_new_password(new_value, old_value, conn.client_signature)
 
             message_body = UserAdminRequest(
                 "userpw",
                 self.sess.username,
                 "password",
                 hash_new_value
```

### Comparing `python-irodsclient-1.1.7/irods/manager/zone_manager.py` & `python-irodsclient-1.1.8/irods/manager/zone_manager.py`

 * *Files identical despite different names*

### Comparing `python-irodsclient-1.1.7/irods/message/__init__.py` & `python-irodsclient-1.1.8/irods/message/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,14 +20,15 @@
                                     SubmessageProperty)
 
 class Bad_AVU_Field(Exception):
     pass
 
 _TUPLE_LIKE_TYPES = (tuple, list)
 
+
 def _qxml_server_version( var ):
     val = os.environ.get( var, '()' )
     vsn = (val and ast.literal_eval( val ))
     if not isinstance( vsn, _TUPLE_LIKE_TYPES ): return None
     return tuple( vsn )
 
 if sys.version_info >= (3,):
@@ -150,14 +151,15 @@
 try:
     # Python 2
     UNICODE = unicode
 except NameError:
     # Python 3
     UNICODE = str
 
+_METADATA_FIELD_TYPES = {str,UNICODE,bytes}
 
 
 # Necessary for older python (<3.7):
 
 def _socket_is_blocking(sk):
     try:
         return sk.getblocking()
@@ -681,15 +683,16 @@
         #   * All fields must each be of type str, except that the units field can be the None object.
         #   * Attribute and Value must be of type str (a Python string) as well as nonzero length.
         for i,arg in enumerate(args):
             error = None
 
             # Raise usage error if any of the AVU fields (args 3 to 5 inclusive) do not meet the above constraints.
             if i in (3,4,5):
-                if type(arg) not in ({str, UNICODE} if i<5 else {str, UNICODE, NoneType}):
+                if type(arg) not in (_METADATA_FIELD_TYPES if i<5
+                                     else {NoneType,}|_METADATA_FIELD_TYPES):
                     error = Bad_AVU_Field("AVU %s (%r) has incorrect type. AVU fields must be strings, except for units, which could be None." % (field_name(i),arg))
                 elif i<5 and not(arg):
                     error = Bad_AVU_Field("AVU %s (%r) is zero-length." % (field_name(i), arg))
             if error is not None:
                 raise error
 
             # If there is no error, set the attribute in the request message.
```

### Comparing `python-irodsclient-1.1.7/irods/message/message.py` & `python-irodsclient-1.1.8/irods/message/message.py`

 * *Files identical despite different names*

### Comparing `python-irodsclient-1.1.7/irods/message/ordered.py` & `python-irodsclient-1.1.8/irods/message/ordered.py`

 * *Files identical despite different names*

### Comparing `python-irodsclient-1.1.7/irods/message/property.py` & `python-irodsclient-1.1.8/irods/message/property.py`

 * *Files identical despite different names*

### Comparing `python-irodsclient-1.1.7/irods/message/quasixml.py` & `python-irodsclient-1.1.8/irods/message/quasixml.py`

 * *Files identical despite different names*

### Comparing `python-irodsclient-1.1.7/irods/meta.py` & `python-irodsclient-1.1.8/irods/meta.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-
+import six
 
 class iRODSMeta(object):
 
     def __init__(self, name, value, units=None, avu_id=None, create_time=None, modify_time=None):
         self.avu_id = avu_id
         self.name = name
         self.value = value
@@ -91,14 +91,20 @@
     def _reset_metadata(self):
         self._meta = self._manager.get(self._model_cls, self._path)
 
     def get_all(self, key):
         """
         Returns a list of iRODSMeta associated with a given key
         """
+        if six.PY2:
+            if isinstance(key, unicode):
+                key = key.encode('utf8')
+        else:
+            if isinstance(key, bytes):
+                key = key.decode('utf8')
         if not isinstance(key, str):
             raise TypeError
         return [m for m in self._meta if m.name == key]
 
     def get_one(self, key):
         """
         Returns the iRODSMeta defined for a key. If there are none,
```

### Comparing `python-irodsclient-1.1.7/irods/models.py` & `python-irodsclient-1.1.8/irods/models.py`

 * *Files identical despite different names*

### Comparing `python-irodsclient-1.1.7/irods/parallel.py` & `python-irodsclient-1.1.8/irods/parallel.py`

 * *Files identical despite different names*

### Comparing `python-irodsclient-1.1.7/irods/password_obfuscation.py` & `python-irodsclient-1.1.8/irods/password_obfuscation.py`

 * *Files identical despite different names*

### Comparing `python-irodsclient-1.1.7/irods/path/__init__.py` & `python-irodsclient-1.1.8/irods/path/__init__.py`

 * *Files identical despite different names*

### Comparing `python-irodsclient-1.1.7/irods/pool.py` & `python-irodsclient-1.1.8/irods/pool.py`

 * *Files identical despite different names*

### Comparing `python-irodsclient-1.1.7/irods/query.py` & `python-irodsclient-1.1.8/irods/query.py`

 * *Files identical despite different names*

### Comparing `python-irodsclient-1.1.7/irods/resource.py` & `python-irodsclient-1.1.8/irods/resource.py`

 * *Files identical despite different names*

### Comparing `python-irodsclient-1.1.7/irods/results.py` & `python-irodsclient-1.1.8/irods/results.py`

 * *Files identical despite different names*

### Comparing `python-irodsclient-1.1.7/irods/rule.py` & `python-irodsclient-1.1.8/irods/rule.py`

 * *Files identical despite different names*

### Comparing `python-irodsclient-1.1.7/irods/session.py` & `python-irodsclient-1.1.8/irods/session.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 from irods.manager.resource_manager import ResourceManager
 from irods.manager.zone_manager import ZoneManager
 from irods.exception import NetworkException
 from irods.password_obfuscation import decode
 from irods import NATIVE_AUTH_SCHEME, PAM_AUTH_SCHEME
 import threading
 import weakref
+from . import DEFAULT_CONNECTION_TIMEOUT
 
 _sessions = None
 _sessions_lock = threading.Lock()
 
 def _cleanup_remaining_sessions():
     for ses in _sessions.copy():
         ses.cleanup()  # internally modifies _sessions
@@ -127,14 +128,15 @@
 
     def __init__(self, configure = True, auto_cleanup = True, **kwargs):
         self.pool = None
         self.numThreads = 0
         self._env_file = ''
         self._auth_file = ''
         self.do_configure = (kwargs if configure else {})
+        self._cached_connection_timeout = kwargs.pop('connection_timeout', DEFAULT_CONNECTION_TIMEOUT)
         self.__configured = None
         if configure:
             self.__configured = self.configure(**kwargs)
 
         self.collections = CollectionManager(self)
         self.data_objects = DataObjectManager(self)
         self.metadata = MetadataManager(self)
@@ -228,14 +230,16 @@
     def configure(self, **kwargs):
         account = self.__configured
         if not account:
             account = self._configure_account(**kwargs)
         connection_refresh_time = self.get_connection_refresh_time(**kwargs)
         logger.debug("In iRODSSession's configure(). connection_refresh_time set to {}".format(connection_refresh_time))
         self.pool = Pool(account, application_name=kwargs.pop('application_name',''), connection_refresh_time=connection_refresh_time)
+        conn_timeout = getattr(self,'_cached_connection_timeout',None)
+        self.pool.connection_timeout = conn_timeout
         return account
 
     def query(self, *args):
         return Query(self, *args)
 
     @property
     def username(self):
@@ -290,15 +294,17 @@
 
     @property
     def connection_timeout(self):
         return self.pool.connection_timeout
 
     @connection_timeout.setter
     def connection_timeout(self, seconds):
-        self.pool.connection_timeout = seconds
+        self._cached_connection_timeout = seconds
+        if seconds is not None:
+            self.pool.connection_timeout = seconds
 
     @staticmethod
     def get_irods_password_file():
         try:
             return os.environ['IRODS_AUTHENTICATION_FILE']
         except KeyError:
             return os.path.expanduser('~/.irods/.irodsA')
```

### Comparing `python-irodsclient-1.1.7/irods/test/README.rst` & `python-irodsclient-1.1.8/irods/test/README.rst`

 * *Files identical despite different names*

### Comparing `python-irodsclient-1.1.7/irods/test/access_test.py` & `python-irodsclient-1.1.8/irods/test/access_test.py`

 * *Files identical despite different names*

### Comparing `python-irodsclient-1.1.7/irods/test/admin_test.py` & `python-irodsclient-1.1.8/irods/test/admin_test.py`

 * *Files identical despite different names*

### Comparing `python-irodsclient-1.1.7/irods/test/collection_test.py` & `python-irodsclient-1.1.8/irods/test/collection_test.py`

 * *Files identical despite different names*

### Comparing `python-irodsclient-1.1.7/irods/test/data_obj_test.py` & `python-irodsclient-1.1.8/irods/test/data_obj_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -1687,11 +1687,26 @@
                     os.stat(phys)
         finally:
             # Clean up.
             for d in data_objects: d.unlink(force = True)
             if dir1: self.sess.resources.get(uniq1).remove()
             if dir2: self.sess.resources.get(uniq2).remove()
 
+    def test_set_and_access_data_comments__issue_450(self):
+        comment = unique_name(my_function_name(), datetime.now()) + " issue 450"
+        ses = self.sess
+        with self.create_simple_resc() as newResc:
+            try:
+                d = ses.data_objects.create('/{0.zone}/home/{0.username}/data_object_for_issue_450_test'.format(ses))
+                d.replicate(**{kw.DEST_RESC_NAME_KW:newResc})
+                ses.data_objects.modDataObjMeta({'objPath':d.path, 'rescHier':ses.resources.get(newResc).hierarchy_string},
+                                                {'dataComments':comment})
+                d = ses.data_objects.get(d.path)
+                repl = [r for r in d.replicas if r.resource_name == newResc][0]
+                self.assertEqual(repl.comments, comment)
+            finally:
+                d.unlink(force = True)
+
 if __name__ == '__main__':
     # let the tests find the parent irods lib
     sys.path.insert(0, os.path.abspath('../..'))
     unittest.main()
```

### Comparing `python-irodsclient-1.1.7/irods/test/exception_test.py` & `python-irodsclient-1.1.8/irods/test/exception_test.py`

 * *Files identical despite different names*

### Comparing `python-irodsclient-1.1.7/irods/test/extended_test.py` & `python-irodsclient-1.1.8/irods/test/extended_test.py`

 * *Files identical despite different names*

### Comparing `python-irodsclient-1.1.7/irods/test/file_test.py` & `python-irodsclient-1.1.8/irods/test/file_test.py`

 * *Files identical despite different names*

### Comparing `python-irodsclient-1.1.7/irods/test/force_create.py` & `python-irodsclient-1.1.8/irods/test/force_create.py`

 * *Files identical despite different names*

### Comparing `python-irodsclient-1.1.7/irods/test/helpers.py` & `python-irodsclient-1.1.8/irods/test/helpers.py`

 * *Files identical despite different names*

### Comparing `python-irodsclient-1.1.7/irods/test/login_auth_test.py` & `python-irodsclient-1.1.8/irods/test/login_auth_test.py`

 * *Files identical despite different names*

### Comparing `python-irodsclient-1.1.7/irods/test/message_test.py` & `python-irodsclient-1.1.8/irods/test/message_test.py`

 * *Files identical despite different names*

### Comparing `python-irodsclient-1.1.7/irods/test/meta_test.py` & `python-irodsclient-1.1.8/irods/test/meta_test.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,31 +4,107 @@
 import os
 import sys
 import time
 import datetime
 import unittest
 from irods.meta import (iRODSMeta, AVUOperation, BadAVUOperationValue, BadAVUOperationKeyword)
 from irods.manager.metadata_manager import InvalidAtomicAVURequest
-from irods.models import (DataObject, Collection, Resource)
+from irods.models import (DataObject, Collection, Resource, CollectionMeta)
 import irods.test.helpers as helpers
 import irods.keywords as kw
 from irods.session import iRODSSession
 from six.moves import range
-from six import PY3
+from six import PY2, PY3
 from irods.message import Bad_AVU_Field
+from irods.column import Like, NotLike
 
 
+def normalize_to_bytes(string, unicode_encoding='utf8'):
+    # Python2 and 3 enumerate bytestrings differently.
+    ord_ = (lambda _:_) if any(x for x in string[:1] if type(x) is int) else ord
+    if not string or ord_(max(x for x in string)) > 255:
+        return string.encode(unicode_encoding)
+    # str->bytes type conversion using element-wise copy, aka a trivial encode.
+    array = bytearray(ord_(x) for x in string)
+    return bytes(array)
+
+def resolves_to_identical_bytestrings(avu1, avu2, key = normalize_to_bytes):
+    avu1 = tuple(avu1)
+    avu2 = tuple(avu2)
+    if len(avu1) != len(avu2):
+        return False
+    for field1,field2 in zip(avu1,avu2):
+        if key(field1) != key(field2):
+            return False
+    return True
 
 class TestMeta(unittest.TestCase):
     '''Suite of tests on metadata operations
     '''
     # test metadata
     attr0, value0, unit0 = 'attr0', 'value0', 'unit0'
     attr1, value1, unit1 = 'attr1', 'value1', 'unit1'
 
+    def test_stringtypes_in_general_query__issue_442(self):
+        metadata = []
+        value = u'a\u1000b'
+        value_encoded = value.encode('utf8')
+        contains_value = {type(value_encoded):b'%%'+value_encoded+b'%%',
+                          type(value):'%%'+value+'%%'}
+        for v in (value, value_encoded):
+
+            # Establish invariant of exactly 2 AVUs attached to object.
+            self.coll.metadata.remove_all()
+            self.coll.metadata['a']=iRODSMeta('a',value)
+            self.coll.metadata['b']=iRODSMeta('b','<arbitrary>')
+            q = self.sess.query(CollectionMeta).filter(Collection.name == self.coll_path)
+            self.assertEqual(len(list(q)),2)
+
+            # Test query with operators Like and NotLike
+            q = self.sess.query(CollectionMeta).filter(Collection.name == self.coll_path,
+                                                       NotLike(CollectionMeta.value,contains_value[type(v)]))
+            self.assertEqual(len(list(q)),1)
+            q = self.sess.query(CollectionMeta).filter(Collection.name == self.coll_path,
+                                                       Like(CollectionMeta.value,contains_value[type(v)]))
+            self.assertEqual(len(list(q)),1)
+
+            # Test query with operators == and !=
+            q = self.sess.query(CollectionMeta).filter(Collection.name == self.coll_path, CollectionMeta.value == v)
+            self.assertEqual(len(list(q)),1)
+            q = self.sess.query(CollectionMeta).filter(Collection.name == self.coll_path, CollectionMeta.value != v)
+            self.assertEqual(len(list(q)),1)
+            metadata.append(self.coll.metadata['a'])
+
+        # Test that application of unicode and bytestring metadata were equivalent
+        self.assertEqual(metadata[0], metadata[1])
+
+    @unittest.skipIf(PY3, 'Unicode strings are normal on Python3')
+    def test_unicode_AVUs_in_Python2__issue_442(self):
+        data_object = self.sess.data_objects.get(self.obj_path)
+        meta_set = iRODSMeta(u'\u1000', u'value', u'units')
+        meta_add = iRODSMeta(*tuple(meta_set))
+        meta_add.name += u"-add"
+        data_object.metadata.set(meta_set)
+        data_object.metadata.add(meta_add)
+        for index, meta in [(m.name, m) for m in (meta_add, meta_set)]:
+            fetched = data_object.metadata[index]
+            self.assertTrue(resolves_to_identical_bytestrings(fetched, meta), 'fetched unexpected meta for %r' % index)
+
+    @unittest.skipIf(PY2, 'Byte strings are normal on Python2')
+    def test_bytestring_AVUs_in_Python3__issue_442(self):
+        data_object = self.sess.data_objects.get(self.obj_path)
+        meta_set = iRODSMeta(u'\u1000'.encode('utf8'),b'value',b'units')
+        meta_add = iRODSMeta(*tuple(meta_set))
+        meta_add.name += b"-add"
+        data_object.metadata.set(meta_set)
+        data_object.metadata.add(meta_add)
+        for index, meta in [(m.name, m) for m in (meta_add, meta_set)]:
+            fetched = data_object.metadata[index]
+            self.assertTrue(resolves_to_identical_bytestrings(fetched, meta), 'fetched unexpected meta for %r' % index)
+
     def setUp(self):
         self.sess = helpers.make_session()
         # test data
         self.coll_path = '/{}/home/{}/test_dir'.format(self.sess.zone, self.sess.username)
         self.obj_name = 'test1'
         self.obj_path = '{coll_path}/{obj_name}'.format(**vars(self))
```

### Comparing `python-irodsclient-1.1.7/irods/test/pool_test.py` & `python-irodsclient-1.1.8/irods/test/pool_test.py`

 * *Files identical despite different names*

### Comparing `python-irodsclient-1.1.7/irods/test/query_test.py` & `python-irodsclient-1.1.8/irods/test/query_test.py`

 * *Files 5% similar despite different names*

```diff
@@ -15,15 +15,15 @@
                           Collection, CollectionMeta,
                           DataObject, DataObjectMeta,
                           RuleExec)
 
 from tempfile import NamedTemporaryFile
 from irods.exception import MultipleResultsFound, CAT_UNKNOWN_SPECIFIC_QUERY, CAT_INVALID_ARGUMENT
 from irods.query import SpecificQuery
-from irods.column import Like, Between, In
+from irods.column import Like, NotLike, Between, In
 from irods.meta import iRODSMeta
 from irods.rule import Rule
 from irods import MAX_SQL_ROWS
 from irods.test.helpers import irods_shared_reg_resc_vault
 import irods.test.helpers as helpers
 from six.moves import range as py3_range
 import irods.keywords as kw
@@ -536,14 +536,26 @@
         qu = self.sess.query(RuleExec.id).filter( Like(RuleExec.frequency,'%1m%'),
                                                   Like(RuleExec.name, '%{unique}%'.format(**locals())) )
         results = [row for row in qu]
         self.assertEqual(1, len(results))
         if results:
             Rule(self.sess).remove_by_id( results[0][RuleExec.id] )
 
+    def test_utf8_equality_in_query__issue_442(self):
+        name = u'prefix-\u1000-suffix'
+        self.sess.data_objects.create(u'{}/{}'.format(self.coll_path, name))
+        query = self.sess.query(DataObject).filter( DataObject.name == name.encode('utf8'),
+                                                    DataObject.collection_id == self.coll.id)
+        self.assertEqual(1, len(list(query)))
+
+    def test_not_like_operator__issue_443(self):
+        name_search_pattern = '%_issue_443.non_matching'
+        query = self.sess.query(DataObject).filter( NotLike(DataObject.name, name_search_pattern),
+                                                    DataObject.collection_id == self.coll.id)
+        self.assertEqual(1, len(list(query)))
 
 class TestSpecificQuery(unittest.TestCase):
 
     def setUp(self):
         super(TestSpecificQuery, self).setUp()
         self.session = helpers.make_session()
```

### Comparing `python-irodsclient-1.1.7/irods/test/resource_test.py` & `python-irodsclient-1.1.8/irods/test/resource_test.py`

 * *Files identical despite different names*

### Comparing `python-irodsclient-1.1.7/irods/test/rule_test.py` & `python-irodsclient-1.1.8/irods/test/rule_test.py`

 * *Files identical despite different names*

### Comparing `python-irodsclient-1.1.7/irods/test/runner.py` & `python-irodsclient-1.1.8/irods/test/runner.py`

 * *Files identical despite different names*

### Comparing `python-irodsclient-1.1.7/irods/test/setupssl.py` & `python-irodsclient-1.1.8/irods/test/setupssl.py`

 * *Files identical despite different names*

### Comparing `python-irodsclient-1.1.7/irods/test/temp_password_test.py` & `python-irodsclient-1.1.8/irods/test/temp_password_test.py`

 * *Files identical despite different names*

### Comparing `python-irodsclient-1.1.7/irods/test/test_paths.py` & `python-irodsclient-1.1.8/irods/test/test_paths.py`

 * *Files identical despite different names*

### Comparing `python-irodsclient-1.1.7/irods/test/ticket_test.py` & `python-irodsclient-1.1.8/irods/test/ticket_test.py`

 * *Files identical despite different names*

### Comparing `python-irodsclient-1.1.7/irods/test/unicode_sampler.xml` & `python-irodsclient-1.1.8/irods/test/unicode_sampler.xml`

 * *Files identical despite different names*

### Comparing `python-irodsclient-1.1.7/irods/test/unicode_test.py` & `python-irodsclient-1.1.8/irods/test/unicode_test.py`

 * *Files identical despite different names*

### Comparing `python-irodsclient-1.1.7/irods/test/user_group_test.py` & `python-irodsclient-1.1.8/irods/test/user_group_test.py`

 * *Files 21% similar despite different names*

```diff
@@ -9,17 +9,17 @@
 from irods import MAX_PASSWORD_LENGTH
 from irods.exception import GroupDoesNotExist, UserDoesNotExist
 from irods.meta import iRODSMetaCollection, iRODSMeta
 from irods.models import User, Group, UserMeta
 from irods.session import iRODSSession
 import irods.exception as ex
 import irods.test.helpers as helpers
+from irods.user import Bad_password_change_parameter
 from six.moves import range
 
-
 class TestGroup(unittest.TestCase):
 
     def setUp(self):
         self.sess = helpers.make_session()
 
     def tearDown(self):
         '''Close connections
@@ -84,15 +84,72 @@
             d['password'] = NEWPASS
             with iRODSSession(**d) as session:
                 self.do_something(session)           # can we still do stuff with the final value of the password?
         finally:
             shutil.rmtree(ENV_DIR)
             ses.users.remove('alice')
 
-    def test_modify_password_with_incorrect_old_value__328(self):
+    def test_modifying_password_at_various_lengths__issue_328(self):
+        ses = self.sess
+        try:
+            pw_lengths = [3,                         # minimum password length
+                          MAX_PASSWORD_LENGTH - 8,   # maximum password length
+                          26]                        # one greater than threshold (See irods/irods#7084)
+
+            # Test different combinations of new and old password lengths
+            tuples_of_old_and_new_password = [('a'*x,'b'*y) for x in pw_lengths for y in pw_lengths]
+            ses.users.create('alice', 'rodsuser')
+
+            for old_pw, new_pw in tuples_of_old_and_new_password:
+                ses.users.modify('alice', 'password',old_pw)
+                # Successful change of own password
+                with iRODSSession(user = 'alice', password = old_pw, host = ses.host, port = ses.port, zone = ses.zone) as user_sess:
+                    user_sess.users.modify_password(old_pw, new_pw)
+                # Test new password is usable
+                with iRODSSession(user = 'alice', password = new_pw, host = ses.host, port = ses.port, zone = ses.zone) as user_sess:
+                    self.do_something(user_sess)
+        finally:
+            ses.users.remove('alice')
+
+    def test_password_corruption_can_be_prevented__issue_448(self):
+        ses = self.sess
+        try:
+            # Threshold value of new password length, at which the server cannot
+            #   properly detect the old-password value is incorrect).
+            #   this is because its descrambled value does not contain space
+            #   for the trailing sixteen character pattern needed by the server to detect a
+            #   valid result for descramble. Of course, it goes ahead and modifies
+            #   the database anyway....so we must screen for this in the client interface.
+            #   (See irods/irods#7084)
+
+            threshold = 25
+
+            max_pw_len = MAX_PASSWORD_LENGTH - 8
+            tuples_of_old_and_new_password = [ ('a'*24,'b'*threshold),
+                                               ('a'*24,'b'*(max_pw_len)),
+                                               ('a'*24,'b'*(max_pw_len + 1)) ]
+            ses.users.create('alice', 'rodsuser')
+            for old_pw, new_pw in tuples_of_old_and_new_password:
+                ses.users.modify('alice', 'password', old_pw)
+
+                # Test that we catch the attempt to change the old password when providing incorrect old password
+                with self.assertRaises(Bad_password_change_parameter):
+                    with iRODSSession(user = 'alice', password = old_pw, host = ses.host, port = ses.port, zone = ses.zone) as user_sess:
+                        user_sess.users.modify_password(old_pw+".", new_pw)
+
+                # Test that we can still change to a valid new password and that the new login is useable.
+                new_pw = new_pw[:max_pw_len] #-> forcing to valid length
+                with iRODSSession(user = 'alice', password = old_pw, host = ses.host, port = ses.port, zone = ses.zone) as user_sess:
+                    user_sess.users.modify_password(old_pw, new_pw)
+                with iRODSSession(user = 'alice', password = new_pw, host = ses.host, port = ses.port, zone = ses.zone) as user_sess:
+                    self.do_something(user_sess)
+        finally:
+            ses.users.remove('alice')
+
+    def test_modify_password_with_incorrect_old_value__issue_328(self):
         ses = self.sess
         if ses.users.get( ses.username ).type != 'rodsadmin':
             self.skipTest( 'Only a rodsadmin may run this test.')
         OLDPASS = 'apass'
         NEWPASS = 'newpass'
         ENV_DIR = tempfile.mkdtemp()
         try:
@@ -103,15 +160,15 @@
             session_factories = [
                        (lambda: iRODSSession(**d)),
                        (lambda: helpers.make_session( irods_env_file = alice_env, irods_authentication_file = alice_auth)),
             ]
             for factory in session_factories:
                 with factory() as alice_ses:
                     alice = alice_ses.users.get(alice_ses.username)
-                    with self.assertRaises( ex.CAT_PASSWORD_ENCODING_ERROR ):
+                    with self.assertRaises(Bad_password_change_parameter):
                         alice.modify_password(OLDPASS + ".", NEWPASS)
             with iRODSSession(**d) as alice_ses:
                 self.do_something(alice_ses)
         finally:
             shutil.rmtree(ENV_DIR)
             ses.users.remove('alice')
 
@@ -414,12 +471,62 @@
         finally:
             if groupadmin:
                 groupadmin.remove()
             # NB: Although created by a groupadmin, the rodsuser must be removed by a rodsadmin.
             if rodsuser:
                 admin.users.remove(rodsuser.name)
 
+    def test_demonstrating_database_password_corruption_in_modify_password__issue_448(self):
+        ses = helpers.make_session()
+        if ses.users.get( ses.username ).type != 'rodsadmin':
+            self.skipTest( 'Only a rodsadmin may run this test.')
+
+        user_alice = None
+        extra="."
+        NEWPASS='1234567890123456789012345'
+        OLDPASS='123456789012345678901234'
+
+        try:
+            user_alice = ses.users.create('alice', 'rodsuser')
+            ses.users.modify('alice', 'password', OLDPASS)
+
+            def alice_login(pw):
+                with iRODSSession(user='alice', password=pw, host=ses.host, port=ses.port, zone=ses.zone) as alice:
+                    home = helpers.home_collection( alice )
+                    alice.collections.get(home)
+
+            alice_login(OLDPASS)
+
+            # Alice makes an unsuccessful attempt at changing her own password.
+            with iRODSSession(user='alice', password=OLDPASS, host=ses.host, port=ses.port, zone=ses.zone) as alice:
+                me = alice.users.get(alice.username)
+                try:
+                    me.modify_password(OLDPASS+extra, NEWPASS)
+                except Bad_password_change_parameter:
+                    pass
+
+            # Whether the server raises an error or not, one would expect that either password in the catalog should
+            # at this point have the desired new value, or it should have been left as it was.
+            # Unfortunately the iRODS server does not guarantee this during the unfiltered use of USER_ADMIN_AN.
+            # (See https://github.com/irods/python-irodsclient/issues/448 .)
+            # Thus, here we make two trials to ensure the condition of integrity.  If neither the old nor the new
+            # password works, 'successes' will stay 0 and the assertion below will fail.  This would indicate the
+            # corruption of the database-stored password that is the subject of this test.
+            successes = 0
+            for password in (OLDPASS, NEWPASS):
+                try:
+                    alice_login(password)
+                except ex.CAT_INVALID_AUTHENTICATION:
+                    pass
+                else:
+                    successes += 1
+            self.assertGreater(successes, 0)
+
+        finally:
+            if user_alice:
+                user_alice.remove()
+
 
 if __name__ == '__main__':
     # let the tests find the parent irods lib
     sys.path.insert(0, os.path.abspath('../..'))
     unittest.main()
```

### Comparing `python-irodsclient-1.1.7/irods/test/zone_test.py` & `python-irodsclient-1.1.8/irods/test/zone_test.py`

 * *Files identical despite different names*

### Comparing `python-irodsclient-1.1.7/irods/ticket.py` & `python-irodsclient-1.1.8/irods/ticket.py`

 * *Files identical despite different names*

### Comparing `python-irodsclient-1.1.7/irods/user.py` & `python-irodsclient-1.1.8/irods/user.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 from __future__ import absolute_import
 from irods.models import User, Group, UserAuth
 from irods.meta import iRODSMetaCollection
 from irods.exception import NoResultFound
 
 _Not_Defined = ()
 
+class Bad_password_change_parameter(Exception): pass
+
 class iRODSUser(object):
 
     def __init__(self, manager, result=None):
         self.manager = manager
         if result:
             self.id = result[User.id]
             self.name = result[User.name]
```

### Comparing `python-irodsclient-1.1.7/irods/zone.py` & `python-irodsclient-1.1.8/irods/zone.py`

 * *Files identical despite different names*

### Comparing `python-irodsclient-1.1.7/python_irodsclient.egg-info/PKG-INFO` & `python-irodsclient-1.1.8/python_irodsclient.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-irodsclient
-Version: 1.1.7
+Version: 1.1.8
 Summary: A python API for iRODS
 Home-page: https://github.com/irods/python-irodsclient
 Author: iRODS Consortium
 Author-email: support@irods.org
 License: BSD
 Description: =========================
         Python iRODS Client (PRC)
```

### Comparing `python-irodsclient-1.1.7/python_irodsclient.egg-info/SOURCES.txt` & `python-irodsclient-1.1.8/python_irodsclient.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `python-irodsclient-1.1.7/setup.py` & `python-irodsclient-1.1.8/setup.py`

 * *Files identical despite different names*

