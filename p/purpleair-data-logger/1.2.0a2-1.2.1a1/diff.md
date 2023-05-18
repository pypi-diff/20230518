# Comparing `tmp/purpleair_data_logger-1.2.0a2.tar.gz` & `tmp/purpleair_data_logger-1.2.1a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "purpleair_data_logger-1.2.0a2.tar", last modified: Sat Feb 18 21:15:24 2023, max compression
+gzip compressed data, was "purpleair_data_logger-1.2.1a1.tar", last modified: Thu May 18 04:50:42 2023, max compression
```

## Comparing `purpleair_data_logger-1.2.0a2.tar` & `purpleair_data_logger-1.2.1a1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-18 21:15:24.519761 purpleair_data_logger-1.2.0a2/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-02-18 21:15:12.000000 purpleair_data_logger-1.2.0a2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    12120 2023-02-18 21:15:24.519761 purpleair_data_logger-1.2.0a2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11586 2023-02-18 21:15:12.000000 purpleair_data_logger-1.2.0a2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-18 21:15:24.519761 purpleair_data_logger-1.2.0a2/purpleair_data_logger/
--rw-r--r--   0 runner    (1001) docker     (123)    21335 2023-02-18 21:15:12.000000 purpleair_data_logger-1.2.0a2/purpleair_data_logger/PurpleAirCSVDataLogger.py
--rw-r--r--   0 runner    (1001) docker     (123)     4136 2023-02-18 21:15:12.000000 purpleair_data_logger-1.2.0a2/purpleair_data_logger/PurpleAirCSVDataLoggerConstants.py
--rw-r--r--   0 runner    (1001) docker     (123)    13124 2023-02-18 21:15:12.000000 purpleair_data_logger-1.2.0a2/purpleair_data_logger/PurpleAirDataLogger.py
--rw-r--r--   0 runner    (1001) docker     (123)    22495 2023-02-18 21:15:12.000000 purpleair_data_logger-1.2.0a2/purpleair_data_logger/PurpleAirPSQLDataLogger.py
--rw-r--r--   0 runner    (1001) docker     (123)    19712 2023-02-18 21:15:12.000000 purpleair_data_logger-1.2.0a2/purpleair_data_logger/PurpleAirPSQLQueryStatements.py
--rw-r--r--   0 runner    (1001) docker     (123)    14388 2023-02-18 21:15:12.000000 purpleair_data_logger-1.2.0a2/purpleair_data_logger/PurpleAirSQLiteDataLogger.py
--rw-r--r--   0 runner    (1001) docker     (123)    14084 2023-02-18 21:15:12.000000 purpleair_data_logger-1.2.0a2/purpleair_data_logger/PurpleAirSQLiteQueryStatements.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-18 21:15:12.000000 purpleair_data_logger-1.2.0a2/purpleair_data_logger/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-18 21:15:24.519761 purpleair_data_logger-1.2.0a2/purpleair_data_logger.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12120 2023-02-18 21:15:24.000000 purpleair_data_logger-1.2.0a2/purpleair_data_logger.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      654 2023-02-18 21:15:24.000000 purpleair_data_logger-1.2.0a2/purpleair_data_logger.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-18 21:15:24.000000 purpleair_data_logger-1.2.0a2/purpleair_data_logger.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-02-18 21:15:24.000000 purpleair_data_logger-1.2.0a2/purpleair_data_logger.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-02-18 21:15:24.000000 purpleair_data_logger-1.2.0a2/purpleair_data_logger.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-02-18 21:15:24.519761 purpleair_data_logger-1.2.0a2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      980 2023-02-18 21:15:12.000000 purpleair_data_logger-1.2.0a2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 04:50:42.591796 purpleair_data_logger-1.2.1a1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-05-18 04:50:33.000000 purpleair_data_logger-1.2.1a1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    17096 2023-05-18 04:50:42.591796 purpleair_data_logger-1.2.1a1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    16581 2023-05-18 04:50:33.000000 purpleair_data_logger-1.2.1a1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 04:50:42.591796 purpleair_data_logger-1.2.1a1/purpleair_data_logger/
+-rw-r--r--   0 runner    (1001) docker     (123)    20652 2023-05-18 04:50:33.000000 purpleair_data_logger-1.2.1a1/purpleair_data_logger/PurpleAirCSVDataLogger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4138 2023-05-18 04:50:33.000000 purpleair_data_logger-1.2.1a1/purpleair_data_logger/PurpleAirCSVDataLoggerConstants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23354 2023-05-18 04:50:33.000000 purpleair_data_logger-1.2.1a1/purpleair_data_logger/PurpleAirDataLogger.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23174 2023-05-18 04:50:33.000000 purpleair_data_logger-1.2.1a1/purpleair_data_logger/PurpleAirPSQLDataLogger.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19714 2023-05-18 04:50:33.000000 purpleair_data_logger-1.2.1a1/purpleair_data_logger/PurpleAirPSQLQueryStatements.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13706 2023-05-18 04:50:33.000000 purpleair_data_logger-1.2.1a1/purpleair_data_logger/PurpleAirSQLiteDataLogger.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14086 2023-05-18 04:50:33.000000 purpleair_data_logger-1.2.1a1/purpleair_data_logger/PurpleAirSQLiteQueryStatements.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 04:50:33.000000 purpleair_data_logger-1.2.1a1/purpleair_data_logger/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 04:50:42.591796 purpleair_data_logger-1.2.1a1/purpleair_data_logger.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    17096 2023-05-18 04:50:42.000000 purpleair_data_logger-1.2.1a1/purpleair_data_logger.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      654 2023-05-18 04:50:42.000000 purpleair_data_logger-1.2.1a1/purpleair_data_logger.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 04:50:42.000000 purpleair_data_logger-1.2.1a1/purpleair_data_logger.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-18 04:50:42.000000 purpleair_data_logger-1.2.1a1/purpleair_data_logger.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-18 04:50:42.000000 purpleair_data_logger-1.2.1a1/purpleair_data_logger.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-05-18 04:50:42.591796 purpleair_data_logger-1.2.1a1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      969 2023-05-18 04:50:33.000000 purpleair_data_logger-1.2.1a1/setup.py
```

### Comparing `purpleair_data_logger-1.2.0a2/LICENSE` & `purpleair_data_logger-1.2.1a1/LICENSE`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2022 carlkid1499
+Copyright (c) 2022 carlkidcrypto
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `purpleair_data_logger-1.2.0a2/PKG-INFO` & `purpleair_data_logger-1.2.1a1/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,75 +1,93 @@
 Metadata-Version: 2.1
 Name: purpleair_data_logger
-Version: 1.2.0a2
-Home-page: https://github.com/carlkid1499/purpleair_data_logger
+Version: 1.2.1a1
+Home-page: https://github.com/carlkidcrypto/purpleair_data_logger
 Author: Carlos Santos
-Author-email: 27721404+carlkid1499@users.noreply.github.com
+Author-email: dose.lucky.sake@cloak.id
 License: MIT
 Keywords: purpleair_data_logger,purple air,purple air data logger,PurpleAirPSQLDataLogger,PurpleAirCSVDataLogger,purple air api,PurpleAirSQLiteDataLogger
 Platform: Windows 32/64
 Platform: Linux 32/64
 Platform: MacOS 32/64
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# purple_air_data_logger
+# Purple Air Data Logger(s) (PADLs)
 
 A set of data logger(s) that will query purple air sensor(s) for data. That data will then be ingested into a TimeScaleDB PostGreSQL database, CSV files, or a SQLite3 database. To use these tools a PurpleAPI key is required. You can get API keys by sending an email to `contact@purpleair.com` with a first and last name to assign them to.
 
-| [![Behave Tests](https://github.com/carlkid1499/purpleair_data_logger/actions/workflows/behave_tests.yml/badge.svg?branch=main)](https://github.com/carlkid1499/purpleair_data_logger/actions/workflows/behave_tests.yml) | [![PyPI Distributions](https://github.com/carlkid1499/purpleair_data_logger/actions/workflows/build_and_publish_to_pypi.yml/badge.svg?branch=main)](https://github.com/carlkid1499/purpleair_data_logger/actions/workflows/build_and_publish_to_pypi.yml) | [![TestPyPI Distributions](https://github.com/carlkid1499/purpleair_data_logger/actions/workflows/build_and_publish_to_test_pypi.yml/badge.svg?branch=main)](https://github.com/carlkid1499/purpleair_data_logger/actions/workflows/build_and_publish_to_test_pypi.yml) |
-| --------------- | --------------- | --------------- |
+| [![Behave Tests](https://github.com/carlkidcrypto/purpleair_data_logger/actions/workflows/behave_tests.yml/badge.svg?branch=main)](https://github.com/carlkidcrypto/purpleair_data_logger/actions/workflows/behave_tests.yml) | [![PyPI Distributions](https://github.com/carlkidcrypto/purpleair_data_logger/actions/workflows/build_and_publish_to_pypi.yml/badge.svg?branch=main)](https://github.com/carlkidcrypto/purpleair_data_logger/actions/workflows/build_and_publish_to_pypi.yml) | [![TestPyPI Distributions](https://github.com/carlkidcrypto/purpleair_data_logger/actions/workflows/build_and_publish_to_test_pypi.yml/badge.svg?branch=main)](https://github.com/carlkidcrypto/purpleair_data_logger/actions/workflows/build_and_publish_to_test_pypi.yml) | [![Black](https://github.com/carlkidcrypto/purpleair_data_logger/actions/workflows/black.yml/badge.svg)](https://github.com/carlkidcrypto/purpleair_data_logger/actions/workflows/black.yml) |
+| --------------- | --------------- | --------------- | --------------- |
 
 ## How to Support This Project
 
-<a href="https://www.buymeacoffee.com/carlkid1499" target="_blank"><img src="https://cdn.buymeacoffee.com/buttons/default-orange.png" alt="Buy Me A Coffee" height="41" width="174"></a>
+<a href="https://www.buymeacoffee.com/carlkidcrypto" target="_blank"><img src="https://cdn.buymeacoffee.com/buttons/default-orange.png" alt="Buy Me A Coffee" height="41" width="174"></a>
 
 ## Installation
 
 You can install the PurpleAir Data Logger via pip.
 
 ```bash
 python3 -m pip install purpleair_data_logger
 ```
 
 You can install PurpleAir Data Logger by cloning down this repo.
 
 ```bash
-git clone https://github.com/carlkid1499/purpleair_data_logger.git
+git clone https://github.com/carlkidcrypto/purpleair_data_logger.git
 cd purpleair_data_logger
 python3 setup.py install 
 ```
 
 ## Usage PurpleAirPSQLDataLogger.py
 
 ```bash
-usage: PurpleAirPSQLDataLogger.py [-h] [-db_drop_all_tables] -db_usr DB_USR [-db_host DB_HOST] -db DB
-                                  [-db_port DB_PORT] [-db_pwd DB_PWD] -paa_read_key PAA_READ_KEY
+usage: PurpleAirPSQLDataLogger.py [-h] -paa_read_key PAA_READ_KEY -paa_write_key PAA_WRITE_KEY
                                   [-paa_single_sensor_request_json_file PAA_SINGLE_SENSOR_REQUEST_JSON_FILE]
                                   [-paa_multiple_sensor_request_json_file PAA_MULTIPLE_SENSOR_REQUEST_JSON_FILE]
+                                  [-paa_group_sensor_request_json_file PAA_GROUP_SENSOR_REQUEST_JSON_FILE]
+                                  [-db_drop_all_tables] -db_usr DB_USR [-db_host DB_HOST] -db DB [-db_port DB_PORT]
+                                  [-db_pwd DB_PWD]
 
 Collect data from PurpleAir sensors and insert into a database!
 
-optional arguments:
+options:
   -h, --help            show this help message and exit
+  -paa_read_key PAA_READ_KEY
+                        The PurpleAirAPI Read key
+  -paa_write_key PAA_WRITE_KEY
+                        The PurpleAirAPI write key
+  -paa_single_sensor_request_json_file PAA_SINGLE_SENSOR_REQUEST_JSON_FILE
+                        The path to a json file containing the parameters to send a single sensor request.
+  -paa_multiple_sensor_request_json_file PAA_MULTIPLE_SENSOR_REQUEST_JSON_FILE
+                        The path to a json file containing the parameters to send a multiple sensor request.
+  -paa_group_sensor_request_json_file PAA_GROUP_SENSOR_REQUEST_JSON_FILE
+                        The path to a json file containing the parameters to send a group sensor request.
   -db_drop_all_tables   Set this flag if you wish to drop all tables before loading in new data. Useful if a database
                         change has happened. Note: Make sure to provide a db_usr with DROP rights. WARNING: ALL
                         COLLECTED DATA WILL BE LOST!
   -db_usr DB_USR        The PSQL database user
   -db_host DB_HOST      The PSQL database host
   -db DB                The PSQL database name
   -db_port DB_PORT      The PSQL database port number
   -db_pwd DB_PWD        The PSQL database password
-  -paa_read_key PAA_READ_KEY
-                        The PurpleAirAPI Read key
-  -paa_single_sensor_request_json_file PAA_SINGLE_SENSOR_REQUEST_JSON_FILE
-                        The path to a json file containing the parameters to send a single sensor request.
-  -paa_multiple_sensor_request_json_file PAA_MULTIPLE_SENSOR_REQUEST_JSON_FILE
-                        The path to a json file containing the parameters to send a multiple sensor request.
+```
+
+Using it with single sensor requests...
+
+```bash
+python3 -m  purpleair_data_logger.PurpleAirPSQLDataLogger -db_usr USER -db_host localhost -db DB_NAME -db_port 5432 -db_pwd PASSWORD -paa_read_key 12345678-1234-1234-1234-123456789123 -paa_write_key 12345678-1234-1234-1234-123456789123 -paa_single_sensor_request_json_file PATH_TO_YOUR_FILE
+```
+
+Using it with multiple sensor requests...
+
+```bash
+python3 -m  purpleair_data_logger.PurpleAirPSQLDataLogger -db_usr USER -db_host localhost -db DB_NAME -db_port 5432 -db_pwd PASSWORD -paa_read_key 12345678-1234-1234-1234-123456789123 -paa_write_key 12345678-1234-1234-1234-123456789123 -paa_multiple_sensor_request_json_file PATH_TO_YOUR_FILE
 ```
 
 ### High Level Design
 
 ![PAA_Data_Logger_Software_Stack.drawio.png](/diagrams/PAA_Data_Logger_Software_Stack.drawio.png)
 
 ### Getting Started
@@ -79,153 +97,234 @@
 3. Install and configure TimescaleDB. <https://docs.timescale.com/install/latest/self-hosted/>
 4. Install and configure Grafana. <https://grafana.com/docs/grafana/latest/setup-grafana/installation/>
 5. Import into your local Grafana instance the dashboard file found [here](./grafana_dashboards/PurpleAirAPI%20(PAA)%20Data%20Logger%20Grafana%20Dashboard-1660355898051.json)
 
 ## Usage PurpleAirCSVDataLogger.py
 
 ```bash
-usage: PurpleAirCSVDataLogger.py [-h] -save_file_path SAVE_FILE_PATH -paa_read_key PAA_READ_KEY
+usage: PurpleAirCSVDataLogger.py [-h] -paa_read_key PAA_READ_KEY -paa_write_key PAA_WRITE_KEY
                                  [-paa_single_sensor_request_json_file PAA_SINGLE_SENSOR_REQUEST_JSON_FILE]
                                  [-paa_multiple_sensor_request_json_file PAA_MULTIPLE_SENSOR_REQUEST_JSON_FILE]
+                                 [-paa_group_sensor_request_json_file PAA_GROUP_SENSOR_REQUEST_JSON_FILE]
+                                 -save_file_path SAVE_FILE_PATH
 
 Collect data from PurpleAir sensors and store it in CSV files!
 
-optional arguments:
+options:
   -h, --help            show this help message and exit
-  -save_file_path SAVE_FILE_PATH
-                        The path to save CSV files in.
   -paa_read_key PAA_READ_KEY
                         The PurpleAirAPI Read key
+  -paa_write_key PAA_WRITE_KEY
+                        The PurpleAirAPI write key
   -paa_single_sensor_request_json_file PAA_SINGLE_SENSOR_REQUEST_JSON_FILE
                         The path to a json file containing the parameters to send a single sensor request.
   -paa_multiple_sensor_request_json_file PAA_MULTIPLE_SENSOR_REQUEST_JSON_FILE
                         The path to a json file containing the parameters to send a multiple sensor request.
+  -paa_group_sensor_request_json_file PAA_GROUP_SENSOR_REQUEST_JSON_FILE
+                        The path to a json file containing the parameters to send a group sensor request.
+  -save_file_path SAVE_FILE_PATH
+                        The path to save CSV files in.
+```
+
+Using it with single sensor requests...
+
+```bash
+python3 -m  purpleair_data_logger.PurpleAirCSVDataLogger -save_file_path SAVE_FILE_PATH -paa_read_key 12345678-1234-1234-1234-123456789123 -paa_write_key 12345678-1234-1234-1234-123456789123 -paa_single_sensor_request_json_file PATH_TO_YOUR_FILE
+```
+
+Using it with multiple sensor requests...
+
+```bash
+python3 -m  purpleair_data_logger.PurpleAirCSVDataLogger -save_file_path SAVE_FILE_PATH -paa_read_key 12345678-1234-1234-1234-123456789123 -paa_write_key 12345678-1234-1234-1234-123456789123 -paa_multiple_sensor_request_json_file PATH_TO_YOUR_FILE
 ```
 
 ## Usage PurpleAirSQLiteDataLogger.py
 
 ```bash
-usage: PurpleAirSQLiteDataLogger.py [-h] -db_name DB_NAME -paa_read_key PAA_READ_KEY
+usage: PurpleAirSQLiteDataLogger.py [-h] -paa_read_key PAA_READ_KEY -paa_write_key PAA_WRITE_KEY
                                     [-paa_single_sensor_request_json_file PAA_SINGLE_SENSOR_REQUEST_JSON_FILE]
                                     [-paa_multiple_sensor_request_json_file PAA_MULTIPLE_SENSOR_REQUEST_JSON_FILE]
+                                    [-paa_group_sensor_request_json_file PAA_GROUP_SENSOR_REQUEST_JSON_FILE] -db_name
+                                    DB_NAME
 
 Collect data from PurpleAir sensors and store it a SQLite3 database file!
 
-optional arguments:
+options:
   -h, --help            show this help message and exit
-  -db_name DB_NAME      The path and name for the SQLite3 database file! i.e database_name.db
   -paa_read_key PAA_READ_KEY
                         The PurpleAirAPI Read key
+  -paa_write_key PAA_WRITE_KEY
+                        The PurpleAirAPI write key
   -paa_single_sensor_request_json_file PAA_SINGLE_SENSOR_REQUEST_JSON_FILE
                         The path to a json file containing the parameters to send a single sensor request.
   -paa_multiple_sensor_request_json_file PAA_MULTIPLE_SENSOR_REQUEST_JSON_FILE
                         The path to a json file containing the parameters to send a multiple sensor request.
+  -paa_group_sensor_request_json_file PAA_GROUP_SENSOR_REQUEST_JSON_FILE
+                        The path to a json file containing the parameters to send a group sensor request.
+  -db_name DB_NAME      The path and name for the SQLite3 database file! i.e database_name.db
+```
+
+Using it with single sensor requests...
+
+```bash
+python3 -m  purpleair_data_logger.PurpleAirSQLiteDataLogger -db_name DB_NAME -paa_read_key 12345678-1234-1234-1234-123456789123 -paa_write_key 12345678-1234-1234-1234-123456789123 -paa_single_sensor_request_json_file PATH_TO_YOUR_FILE
+```
+
+Using it with multiple sensor requests...
+
+```bash
+python3 -m  purpleair_data_logger.PurpleAirSQLiteDataLogger -db_name DB_NAME -paa_read_key 12345678-1234-1234-1234-123456789123 -paa_write_key 12345678-1234-1234-1234-123456789123 -paa_multiple_sensor_request_json_file PATH_TO_YOUR_FILE
 ```
 
 ## Sample JSON Configuration File(s)
 
 The following sample json configuration files can be used with any of the data loggers.
 
-### PAA_SINGLE_SENSOR_REQUEST_JSON_FILE Example
+### PAA Single Sensor Request Example
 
 Out of the parameters listed below only "sensor_index" is required. The others are all optional according to PurpleAirAPI (PAA) documentation. If a field is not being used, mark it 'null' without the single quotes.
 
 ```json
 {
     "sensor_index": 53,
     "read_key": null,
     "fields": null
 }
 ```
 
+Or see this [file](./sample_json_config_files/sample_single_sensor_request_json_file.json) for another example.
+
 > Note: Refer to the PurpleAirAPI (PAA) documentation for more information. <https://api.purpleair.com/#api-sensors-get-sensor-data>
 
-### PAA_MULTIPLE_SENSOR_REQUEST_JSON_FILE Example
+### PAA Multiple Sensor Request Example
 
 Out of the parameters listed below only "fields" is required. The others are all optional according to PurpleAirAPI (PAA) documentation. If a field is not being used, mark it 'null' without the single quotes.
 
 ```json
 {
-    "fields": "A string comma delimited list of fields to retrieve",
+    "fields": "A string comma delimited string of fields to retrieve. i.e fields,name,etc",
     "location_type": null,
     "read_keys": null,
     "show_only": null,
     "modified_since": null,
     "max_age": null,
     "nwlng" : null,
     "nwlat": null,
     "selng": null,
     "selat": null
 }
 ```
 
+Or see this [file](./sample_json_config_files/sample_multiple_sensor_request_json_file.json) for another example.
+
 > Note: Refer to the PurpleAirAPI (PAA) documentation for more information. <https://api.purpleair.com/#api-sensors-get-sensors-data>
 
-> Taken From the PurpleAirAPI documentation:
+The below snippet is taken From the PurpleAirAPI (PAA) documentation:
+
+```plain text
+  Field Type Description
+  fields String
+  The 'Fields' parameter specifies which 'sensor data fields' to include in the response. It is a comma separated list with one or more of the following:
+
+  Station information and status fields:
+  name, icon, model, hardware, location_type, private, latitude, longitude, altitude, position_rating, led_brightness, firmware_version, firmware_upgrade, rssi, uptime, pa_latency, memory, last_seen, last_modified, date_created, channel_state, channel_flags, channel_flags_manual, channel_flags_auto, confidence, confidence_manual, confidence_auto
 
-    Field Type Description
-    fields String 
-    The 'Fields' parameter specifies which 'sensor data fields' to include in the response. It is a comma separated list with one or more of the following:
+  Environmental fields:
+  humidity, humidity_a, humidity_b, temperature, temperature_a, temperature_b, pressure, pressure_a, pressure_b
 
-    Station information and status fields:
-    name, icon, model, hardware, location_type, private, latitude, longitude, altitude, position_rating, led_brightness, firmware_version, firmware_upgrade, rssi, uptime, pa_latency, memory, last_seen, last_modified, date_created, channel_state, channel_flags, channel_flags_manual, channel_flags_auto, confidence, confidence_manual, confidence_auto
+  Miscellaneous fields:
+  voc, voc_a, voc_b, ozone1, analog_input
 
-    Environmental fields:
-    humidity, humidity_a, humidity_b, temperature, temperature_a, temperature_b, pressure, pressure_a, pressure_b
+  PM1.0 fields:
+  pm1.0, pm1.0_a, pm1.0_b, pm1.0_atm, pm1.0_atm_a, pm1.0_atm_b, pm1.0_cf_1, pm1.0_cf_1_a, pm1.0_cf_1_b
 
-    Miscellaneous fields:
-    voc, voc_a, voc_b, ozone1, analog_input
+  PM2.5 fields:
+  pm2.5_alt, pm2.5_alt_a, pm2.5_alt_b, pm2.5, pm2.5_a, pm2.5_b, pm2.5_atm, pm2.5_atm_a, pm2.5_atm_b, pm2.5_cf_1, pm2.5_cf_1_a, pm2.5_cf_1_b
 
-    PM1.0 fields:
-    pm1.0, pm1.0_a, pm1.0_b, pm1.0_atm, pm1.0_atm_a, pm1.0_atm_b, pm1.0_cf_1, pm1.0_cf_1_a, pm1.0_cf_1_b
+  PM2.5 pseudo (simple running) average fields:
+  pm2.5_10minute, pm2.5_10minute_a, pm2.5_10minute_b, pm2.5_30minute, pm2.5_30minute_a, pm2.5_30minute_b, pm2.5_60minute, pm2.5_60minute_a, pm2.5_60minute_b, pm2.5_6hour, pm2.5_6hour_a, pm2.5_6hour_b, pm2.5_24hour, pm2.5_24hour_a, pm2.5_24hour_b, pm2.5_1week, pm2.5_1week_a, pm2.5_1week_b
 
-    PM2.5 fields:
-    pm2.5_alt, pm2.5_alt_a, pm2.5_alt_b, pm2.5, pm2.5_a, pm2.5_b, pm2.5_atm, pm2.5_atm_a, pm2.5_atm_b, pm2.5_cf_1, pm2.5_cf_1_a, pm2.5_cf_1_b
+  PM10.0 fields:
+  pm10.0, pm10.0_a, pm10.0_b, pm10.0_atm, pm10.0_atm_a, pm10.0_atm_b, pm10.0_cf_1, pm10.0_cf_1_a, pm10.0_cf_1_b
 
-    PM2.5 pseudo (simple running) average fields:
-    pm2.5_10minute, pm2.5_10minute_a, pm2.5_10minute_b, pm2.5_30minute, pm2.5_30minute_a, pm2.5_30minute_b, pm2.5_60minute, pm2.5_60minute_a, pm2.5_60minute_b, pm2.5_6hour, pm2.5_6hour_a, pm2.5_6hour_b, pm2.5_24hour, pm2.5_24hour_a, pm2.5_24hour_b, pm2.5_1week, pm2.5_1week_a, pm2.5_1week_b
+  Visibility fields:
+  scattering_coefficient, scattering_coefficient_a, scattering_coefficient_b, deciviews, deciviews_a, deciviews_b, visual_range, visual_range_a, visual_range_b
 
-    PM10.0 fields:
-    pm10.0, pm10.0_a, pm10.0_b, pm10.0_atm, pm10.0_atm_a, pm10.0_atm_b, pm10.0_cf_1, pm10.0_cf_1_a, pm10.0_cf_1_b
+  Particle count fields:
+  0.3_um_count, 0.3_um_count_a, 0.3_um_count_b, 0.5_um_count, 0.5_um_count_a, 0.5_um_count_b, 1.0_um_count, 1.0_um_count_a, 1.0_um_count_b, 2.5_um_count, 2.5_um_count_a, 2.5_um_count_b, 5.0_um_count, 5.0_um_count_a, 5.0_um_count_b, 10.0_um_count 10.0_um_count_a, 10.0_um_count_b
 
-    Visibility fields:
-    scattering_coefficient, scattering_coefficient_a, scattering_coefficient_b, deciviews, deciviews_a, deciviews_b, visual_range, visual_range_a, visual_range_b
+  ThingSpeak fields, used to retrieve data from api.thingspeak.com:
+  primary_id_a, primary_key_a, secondary_id_a, secondary_key_a, primary_id_b, primary_key_b, secondary_id_b, secondary_key_b
 
-    Particle count fields:
-    0.3_um_count, 0.3_um_count_a, 0.3_um_count_b, 0.5_um_count, 0.5_um_count_a, 0.5_um_count_b, 1.0_um_count, 1.0_um_count_a, 1.0_um_count_b, 2.5_um_count, 2.5_um_count_a, 2.5_um_count_b, 5.0_um_count, 5.0_um_count_a, 5.0_um_count_b, 10.0_um_count 10.0_um_count_a, 10.0_um_count_b
+  For field descriptions, please see the 'sensor data fields'. section.
 
-    ThingSpeak fields, used to retrieve data from api.thingspeak.com:
-    primary_id_a, primary_key_a, secondary_id_a, secondary_key_a, primary_id_b, primary_key_b, secondary_id_b, secondary_key_b
+  location_type optional Number
+  The location_type of the sensors.
+  Possible values are: 0 = Outside or 1 = Inside.
 
-    For field descriptions, please see the 'sensor data fields'. section.
+  read_keys optional String
+  A read_key is required for private devices. It is separate to the api_key and each sensor has its own read_key. Submit multiple keys by separating them with a comma (,) character for example: key-one,key-two,key-three.
 
-    location_type optional Number 
-    The location_type of the sensors.
-    Possible values are: 0 = Outside or 1 = Inside.
+  show_only optional String
+  A comma (,) separated list of sensor_index values. When provided, the results are limited only to the sensors included in this list.
 
-    read_keys optional String 
-    A read_key is required for private devices. It is separate to the api_key and each sensor has its own read_key. Submit multiple keys by separating them with a comma (,) character for example: key-one,key-two,key-three.
+  modified_since optional long
+  The modified_since parameter causes only sensors modified after the provided time stamp to be included in the results. Using the time_stamp value from a previous call (recommended) will limit results to those with new values since the last request. Using a value of 0 will match sensors modified at any time.
 
-    show_only optional String 
-    A comma (,) separated list of sensor_index values. When provided, the results are limited only to the sensors included in this list.
+  max_age optional Integer
+  Filter results to only include sensors modified or updated within the last number of seconds. Using a value of 0 will match sensors of any age.
 
-    modified_since optional long 
-    The modified_since parameter causes only sensors modified after the provided time stamp to be included in the results. Using the time_stamp value from a previous call (recommended) will limit results to those with new values since the last request. Using a value of 0 will match sensors modified at any time.
+  Default value: 604800
 
-    max_age optional Integer 
-    Filter results to only include sensors modified or updated within the last number of seconds. Using a value of 0 will match sensors of any age.
+  nwlng optional Number
+  A north west longitude for the bounding box.
 
-    Default value: 604800
+  Use a bounding box to limit the sensors returned to a specific geographic area. The bounding box is defined by two points, a north west latitude/longitude and a south east latitude/longitude.
+
+  nwlat optional Number
+  A north west latitude for the bounding box.
+
+  selng optional Number
+  A south east longitude for the bounding box.
+
+  selat optional Number
+  A south east latitude for the bounding box.
+```
 
-    nwlng optional Number 
-    A north west longitude for the bounding box.
+### PAA Group Sensor Request Example
 
-    Use a bounding box to limit the sensors returned to a specific geographic area. The bounding box is defined by two points, a north west latitude/longitude and a south east latitude/longitude.
+Out of the parameters below `sensor_group_name`, `add_sensors_to_group`, and `sensor_index_list` are custom settings not
+defined in the official PAA documentation. These three setting help drive the `group` request feature.
 
-    nwlat optional Number 
-    A north west latitude for the bounding box.
+`sensor_group_name` - This will be the name assigned to your group. If it doesn't exist already, it will be created.
+Otherwise, the first group matching the name will be used.
 
-    selng optional Number 
-    A south east longitude for the bounding box.
+`add_sensors_to_group` - If true, adds the sensors in the `sensor_index_list`. If false, `sensor_index_list` is ignored.
+
+`sensor_index_list` -  A list of sensor indexes that will be added to your group if they don't already exist.
+
+The rest of the settings are official PAA settings. They are the same as the [### PAA Multiple Sensor Request Example](#paa-multiple-sensor-request-example). Refer above for details.
+
+```json
+{
+    "sensor_group_name": "A Name Goes Here",
+    "add_sensors_to_group": true,
+    "sensor_index_list": [
+        77,
+        81,
+        95079,
+        167897
+    ],
+    "fields": "A string comma delimited string of fields to retrieve. i.e fields,name,etc",
+    "location_type": null,
+    "read_keys": null,
+    "show_only": null,
+    "modified_since": null,
+    "max_age": null,
+    "nwlng" : null,
+    "nwlat": null,
+    "selng": null,
+    "selat": null
+}
+```
 
-    selat optional Number 
-    A south east latitude for the bounding box.
+Or see this [file](./sample_json_config_files/sample_group_sensor_request_json_file.json) for another example.
```

#### html2text {}

```diff
@@ -1,130 +1,176 @@
-Metadata-Version: 2.1 Name: purpleair_data_logger Version: 1.2.0a2 Home-page:
-https://github.com/carlkid1499/purpleair_data_logger Author: Carlos Santos
-Author-email: 27721404+carlkid1499@users.noreply.github.com License: MIT
-Keywords: purpleair_data_logger,purple air,purple air data
+Metadata-Version: 2.1 Name: purpleair_data_logger Version: 1.2.1a1 Home-page:
+https://github.com/carlkidcrypto/purpleair_data_logger Author: Carlos Santos
+Author-email: dose.lucky.sake@cloak.id License: MIT Keywords:
+purpleair_data_logger,purple air,purple air data
 logger,PurpleAirPSQLDataLogger,PurpleAirCSVDataLogger,purple air
 api,PurpleAirSQLiteDataLogger Platform: Windows 32/64 Platform: Linux 32/64
 Platform: MacOS 32/64 Requires-Python: >=3.8 Description-Content-Type: text/
-markdown License-File: LICENSE # purple_air_data_logger A set of data logger(s)
-that will query purple air sensor(s) for data. That data will then be ingested
-into a TimeScaleDB PostGreSQL database, CSV files, or a SQLite3 database. To
-use these tools a PurpleAPI key is required. You can get API keys by sending an
-email to `contact@purpleair.com` with a first and last name to assign them to.
-| [![Behave Tests](https://github.com/carlkid1499/purpleair_data_logger/
-actions/workflows/behave_tests.yml/badge.svg?branch=main)](https://github.com/
-carlkid1499/purpleair_data_logger/actions/workflows/behave_tests.yml) | [![PyPI
-Distributions](https://github.com/carlkid1499/purpleair_data_logger/actions/
-workflows/build_and_publish_to_pypi.yml/badge.svg?branch=main)](https://
-github.com/carlkid1499/purpleair_data_logger/actions/workflows/
+markdown License-File: LICENSE # Purple Air Data Logger(s) (PADLs) A set of
+data logger(s) that will query purple air sensor(s) for data. That data will
+then be ingested into a TimeScaleDB PostGreSQL database, CSV files, or a
+SQLite3 database. To use these tools a PurpleAPI key is required. You can get
+API keys by sending an email to `contact@purpleair.com` with a first and last
+name to assign them to. | [![Behave Tests](https://github.com/carlkidcrypto/
+purpleair_data_logger/actions/workflows/behave_tests.yml/
+badge.svg?branch=main)](https://github.com/carlkidcrypto/purpleair_data_logger/
+actions/workflows/behave_tests.yml) | [![PyPI Distributions](https://
+github.com/carlkidcrypto/purpleair_data_logger/actions/workflows/
+build_and_publish_to_pypi.yml/badge.svg?branch=main)](https://github.com/
+carlkidcrypto/purpleair_data_logger/actions/workflows/
 build_and_publish_to_pypi.yml) | [![TestPyPI Distributions](https://github.com/
-carlkid1499/purpleair_data_logger/actions/workflows/
+carlkidcrypto/purpleair_data_logger/actions/workflows/
 build_and_publish_to_test_pypi.yml/badge.svg?branch=main)](https://github.com/
-carlkid1499/purpleair_data_logger/actions/workflows/
-build_and_publish_to_test_pypi.yml) | | --------------- | --------------- | ---
------------- | ## How to Support This Project [Buy_Me_A_Coffee] ## Installation
-You can install the PurpleAir Data Logger via pip. ```bash python3 -m pip
-install purpleair_data_logger ``` You can install PurpleAir Data Logger by
-cloning down this repo. ```bash git clone https://github.com/carlkid1499/
+carlkidcrypto/purpleair_data_logger/actions/workflows/
+build_and_publish_to_test_pypi.yml) | [![Black](https://github.com/
+carlkidcrypto/purpleair_data_logger/actions/workflows/black.yml/badge.svg)]
+(https://github.com/carlkidcrypto/purpleair_data_logger/actions/workflows/
+black.yml) | | --------------- | --------------- | --------------- | ----------
+----- | ## How to Support This Project [Buy_Me_A_Coffee] ## Installation You
+can install the PurpleAir Data Logger via pip. ```bash python3 -m pip install
+purpleair_data_logger ``` You can install PurpleAir Data Logger by cloning down
+this repo. ```bash git clone https://github.com/carlkidcrypto/
 purpleair_data_logger.git cd purpleair_data_logger python3 setup.py install ```
 ## Usage PurpleAirPSQLDataLogger.py ```bash usage: PurpleAirPSQLDataLogger.py
-[-h] [-db_drop_all_tables] -db_usr DB_USR [-db_host DB_HOST] -db DB [-db_port
-DB_PORT] [-db_pwd DB_PWD] -paa_read_key PAA_READ_KEY [-
+[-h] -paa_read_key PAA_READ_KEY -paa_write_key PAA_WRITE_KEY [-
 paa_single_sensor_request_json_file PAA_SINGLE_SENSOR_REQUEST_JSON_FILE] [-
-paa_multiple_sensor_request_json_file PAA_MULTIPLE_SENSOR_REQUEST_JSON_FILE]
-Collect data from PurpleAir sensors and insert into a database! optional
-arguments: -h, --help show this help message and exit -db_drop_all_tables Set
-this flag if you wish to drop all tables before loading in new data. Useful if
-a database change has happened. Note: Make sure to provide a db_usr with DROP
-rights. WARNING: ALL COLLECTED DATA WILL BE LOST! -db_usr DB_USR The PSQL
-database user -db_host DB_HOST The PSQL database host -db DB The PSQL database
-name -db_port DB_PORT The PSQL database port number -db_pwd DB_PWD The PSQL
-database password -paa_read_key PAA_READ_KEY The PurpleAirAPI Read key -
-paa_single_sensor_request_json_file PAA_SINGLE_SENSOR_REQUEST_JSON_FILE The
-path to a json file containing the parameters to send a single sensor request.
--paa_multiple_sensor_request_json_file PAA_MULTIPLE_SENSOR_REQUEST_JSON_FILE
-The path to a json file containing the parameters to send a multiple sensor
-request. ``` ### High Level Design ![PAA_Data_Logger_Software_Stack.drawio.png]
-(/diagrams/PAA_Data_Logger_Software_Stack.drawio.png) ### Getting Started 1.
-Grab and install Postgresql for your platform.
+paa_multiple_sensor_request_json_file PAA_MULTIPLE_SENSOR_REQUEST_JSON_FILE] [-
+paa_group_sensor_request_json_file PAA_GROUP_SENSOR_REQUEST_JSON_FILE] [-
+db_drop_all_tables] -db_usr DB_USR [-db_host DB_HOST] -db DB [-db_port DB_PORT]
+[-db_pwd DB_PWD] Collect data from PurpleAir sensors and insert into a
+database! options: -h, --help show this help message and exit -paa_read_key
+PAA_READ_KEY The PurpleAirAPI Read key -paa_write_key PAA_WRITE_KEY The
+PurpleAirAPI write key -paa_single_sensor_request_json_file
+PAA_SINGLE_SENSOR_REQUEST_JSON_FILE The path to a json file containing the
+parameters to send a single sensor request. -
+paa_multiple_sensor_request_json_file PAA_MULTIPLE_SENSOR_REQUEST_JSON_FILE The
+path to a json file containing the parameters to send a multiple sensor
+request. -paa_group_sensor_request_json_file PAA_GROUP_SENSOR_REQUEST_JSON_FILE
+The path to a json file containing the parameters to send a group sensor
+request. -db_drop_all_tables Set this flag if you wish to drop all tables
+before loading in new data. Useful if a database change has happened. Note:
+Make sure to provide a db_usr with DROP rights. WARNING: ALL COLLECTED DATA
+WILL BE LOST! -db_usr DB_USR The PSQL database user -db_host DB_HOST The PSQL
+database host -db DB The PSQL database name -db_port DB_PORT The PSQL database
+port number -db_pwd DB_PWD The PSQL database password ``` Using it with single
+sensor requests... ```bash python3 -
+m purpleair_data_logger.PurpleAirPSQLDataLogger -db_usr USER -db_host localhost
+-db DB_NAME -db_port 5432 -db_pwd PASSWORD -paa_read_key 12345678-1234-1234-
+1234-123456789123 -paa_write_key 12345678-1234-1234-1234-123456789123 -
+paa_single_sensor_request_json_file PATH_TO_YOUR_FILE ``` Using it with
+multiple sensor requests... ```bash python3 -
+m purpleair_data_logger.PurpleAirPSQLDataLogger -db_usr USER -db_host localhost
+-db DB_NAME -db_port 5432 -db_pwd PASSWORD -paa_read_key 12345678-1234-1234-
+1234-123456789123 -paa_write_key 12345678-1234-1234-1234-123456789123 -
+paa_multiple_sensor_request_json_file PATH_TO_YOUR_FILE ``` ### High Level
+Design ![PAA_Data_Logger_Software_Stack.drawio.png](/diagrams/
+PAA_Data_Logger_Software_Stack.drawio.png) ### Getting Started 1. Grab and
+install Postgresql for your platform.
 www.postgresql.org/download/> 2. Create two database users. One for Grafana
 with select only privileges. The other for the data logger with only insert/
 create privileges.
 medium.com/coding-blocks/creating-user-database-and-adding-access-on-
 postgresql-8bfcd2f4a91e>,
 www.techonthenet.com/postgresql/grant_revoke.php> 3. Install and configure
 TimescaleDB.
 docs.timescale.com/install/latest/self-hosted/> 4. Install and configure
 Grafana.
 grafana.com/docs/grafana/latest/setup-grafana/installation/> 5. Import into
 your local Grafana instance the dashboard file found [here](./
 grafana_dashboards/PurpleAirAPI%20(PAA)%20Data%20Logger%20Grafana%20Dashboard-
 1660355898051.json) ## Usage PurpleAirCSVDataLogger.py ```bash usage:
-PurpleAirCSVDataLogger.py [-h] -save_file_path SAVE_FILE_PATH -paa_read_key
-PAA_READ_KEY [-paa_single_sensor_request_json_file
+PurpleAirCSVDataLogger.py [-h] -paa_read_key PAA_READ_KEY -paa_write_key
+PAA_WRITE_KEY [-paa_single_sensor_request_json_file
 PAA_SINGLE_SENSOR_REQUEST_JSON_FILE] [-paa_multiple_sensor_request_json_file
-PAA_MULTIPLE_SENSOR_REQUEST_JSON_FILE] Collect data from PurpleAir sensors and
-store it in CSV files! optional arguments: -h, --help show this help message
-and exit -save_file_path SAVE_FILE_PATH The path to save CSV files in. -
-paa_read_key PAA_READ_KEY The PurpleAirAPI Read key -
+PAA_MULTIPLE_SENSOR_REQUEST_JSON_FILE] [-paa_group_sensor_request_json_file
+PAA_GROUP_SENSOR_REQUEST_JSON_FILE] -save_file_path SAVE_FILE_PATH Collect data
+from PurpleAir sensors and store it in CSV files! options: -h, --help show this
+help message and exit -paa_read_key PAA_READ_KEY The PurpleAirAPI Read key -
+paa_write_key PAA_WRITE_KEY The PurpleAirAPI write key -
 paa_single_sensor_request_json_file PAA_SINGLE_SENSOR_REQUEST_JSON_FILE The
 path to a json file containing the parameters to send a single sensor request.
 -paa_multiple_sensor_request_json_file PAA_MULTIPLE_SENSOR_REQUEST_JSON_FILE
 The path to a json file containing the parameters to send a multiple sensor
-request. ``` ## Usage PurpleAirSQLiteDataLogger.py ```bash usage:
-PurpleAirSQLiteDataLogger.py [-h] -db_name DB_NAME -paa_read_key PAA_READ_KEY
-[-paa_single_sensor_request_json_file PAA_SINGLE_SENSOR_REQUEST_JSON_FILE] [-
-paa_multiple_sensor_request_json_file PAA_MULTIPLE_SENSOR_REQUEST_JSON_FILE]
-Collect data from PurpleAir sensors and store it a SQLite3 database file!
-optional arguments: -h, --help show this help message and exit -db_name DB_NAME
-The path and name for the SQLite3 database file! i.e database_name.db -
-paa_read_key PAA_READ_KEY The PurpleAirAPI Read key -
+request. -paa_group_sensor_request_json_file PAA_GROUP_SENSOR_REQUEST_JSON_FILE
+The path to a json file containing the parameters to send a group sensor
+request. -save_file_path SAVE_FILE_PATH The path to save CSV files in. ```
+Using it with single sensor requests... ```bash python3 -
+m purpleair_data_logger.PurpleAirCSVDataLogger -save_file_path SAVE_FILE_PATH -
+paa_read_key 12345678-1234-1234-1234-123456789123 -paa_write_key 12345678-1234-
+1234-1234-123456789123 -paa_single_sensor_request_json_file PATH_TO_YOUR_FILE
+``` Using it with multiple sensor requests... ```bash python3 -
+m purpleair_data_logger.PurpleAirCSVDataLogger -save_file_path SAVE_FILE_PATH -
+paa_read_key 12345678-1234-1234-1234-123456789123 -paa_write_key 12345678-1234-
+1234-1234-123456789123 -paa_multiple_sensor_request_json_file PATH_TO_YOUR_FILE
+``` ## Usage PurpleAirSQLiteDataLogger.py ```bash usage:
+PurpleAirSQLiteDataLogger.py [-h] -paa_read_key PAA_READ_KEY -paa_write_key
+PAA_WRITE_KEY [-paa_single_sensor_request_json_file
+PAA_SINGLE_SENSOR_REQUEST_JSON_FILE] [-paa_multiple_sensor_request_json_file
+PAA_MULTIPLE_SENSOR_REQUEST_JSON_FILE] [-paa_group_sensor_request_json_file
+PAA_GROUP_SENSOR_REQUEST_JSON_FILE] -db_name DB_NAME Collect data from
+PurpleAir sensors and store it a SQLite3 database file! options: -h, --help
+show this help message and exit -paa_read_key PAA_READ_KEY The PurpleAirAPI
+Read key -paa_write_key PAA_WRITE_KEY The PurpleAirAPI write key -
 paa_single_sensor_request_json_file PAA_SINGLE_SENSOR_REQUEST_JSON_FILE The
 path to a json file containing the parameters to send a single sensor request.
 -paa_multiple_sensor_request_json_file PAA_MULTIPLE_SENSOR_REQUEST_JSON_FILE
 The path to a json file containing the parameters to send a multiple sensor
-request. ``` ## Sample JSON Configuration File(s) The following sample json
-configuration files can be used with any of the data loggers. ###
-PAA_SINGLE_SENSOR_REQUEST_JSON_FILE Example Out of the parameters listed below
-only "sensor_index" is required. The others are all optional according to
-PurpleAirAPI (PAA) documentation. If a field is not being used, mark it 'null'
-without the single quotes. ```json { "sensor_index": 53, "read_key": null,
-"fields": null } ``` > Note: Refer to the PurpleAirAPI (PAA) documentation for
-more information.
-api.purpleair.com/#api-sensors-get-sensor-data> ###
-PAA_MULTIPLE_SENSOR_REQUEST_JSON_FILE Example Out of the parameters listed
-below only "fields" is required. The others are all optional according to
-PurpleAirAPI (PAA) documentation. If a field is not being used, mark it 'null'
-without the single quotes. ```json { "fields": "A string comma delimited list
-of fields to retrieve", "location_type": null, "read_keys": null, "show_only":
-null, "modified_since": null, "max_age": null, "nwlng" : null, "nwlat": null,
-"selng": null, "selat": null } ``` > Note: Refer to the PurpleAirAPI (PAA)
-documentation for more information.
-api.purpleair.com/#api-sensors-get-sensors-data> > Taken From the PurpleAirAPI
-documentation: Field Type Description fields String The 'Fields' parameter
-specifies which 'sensor data fields' to include in the response. It is a comma
-separated list with one or more of the following: Station information and
-status fields: name, icon, model, hardware, location_type, private, latitude,
-longitude, altitude, position_rating, led_brightness, firmware_version,
-firmware_upgrade, rssi, uptime, pa_latency, memory, last_seen, last_modified,
-date_created, channel_state, channel_flags, channel_flags_manual,
-channel_flags_auto, confidence, confidence_manual, confidence_auto
-Environmental fields: humidity, humidity_a, humidity_b, temperature,
-temperature_a, temperature_b, pressure, pressure_a, pressure_b Miscellaneous
-fields: voc, voc_a, voc_b, ozone1, analog_input PM1.0 fields: pm1.0, pm1.0_a,
-pm1.0_b, pm1.0_atm, pm1.0_atm_a, pm1.0_atm_b, pm1.0_cf_1, pm1.0_cf_1_a,
-pm1.0_cf_1_b PM2.5 fields: pm2.5_alt, pm2.5_alt_a, pm2.5_alt_b, pm2.5, pm2.5_a,
-pm2.5_b, pm2.5_atm, pm2.5_atm_a, pm2.5_atm_b, pm2.5_cf_1, pm2.5_cf_1_a,
-pm2.5_cf_1_b PM2.5 pseudo (simple running) average fields: pm2.5_10minute,
-pm2.5_10minute_a, pm2.5_10minute_b, pm2.5_30minute, pm2.5_30minute_a,
-pm2.5_30minute_b, pm2.5_60minute, pm2.5_60minute_a, pm2.5_60minute_b,
-pm2.5_6hour, pm2.5_6hour_a, pm2.5_6hour_b, pm2.5_24hour, pm2.5_24hour_a,
-pm2.5_24hour_b, pm2.5_1week, pm2.5_1week_a, pm2.5_1week_b PM10.0 fields:
-pm10.0, pm10.0_a, pm10.0_b, pm10.0_atm, pm10.0_atm_a, pm10.0_atm_b,
-pm10.0_cf_1, pm10.0_cf_1_a, pm10.0_cf_1_b Visibility fields:
+request. -paa_group_sensor_request_json_file PAA_GROUP_SENSOR_REQUEST_JSON_FILE
+The path to a json file containing the parameters to send a group sensor
+request. -db_name DB_NAME The path and name for the SQLite3 database file! i.e
+database_name.db ``` Using it with single sensor requests... ```bash python3 -
+m purpleair_data_logger.PurpleAirSQLiteDataLogger -db_name DB_NAME -
+paa_read_key 12345678-1234-1234-1234-123456789123 -paa_write_key 12345678-1234-
+1234-1234-123456789123 -paa_single_sensor_request_json_file PATH_TO_YOUR_FILE
+``` Using it with multiple sensor requests... ```bash python3 -
+m purpleair_data_logger.PurpleAirSQLiteDataLogger -db_name DB_NAME -
+paa_read_key 12345678-1234-1234-1234-123456789123 -paa_write_key 12345678-1234-
+1234-1234-123456789123 -paa_multiple_sensor_request_json_file PATH_TO_YOUR_FILE
+``` ## Sample JSON Configuration File(s) The following sample json
+configuration files can be used with any of the data loggers. ### PAA Single
+Sensor Request Example Out of the parameters listed below only "sensor_index"
+is required. The others are all optional according to PurpleAirAPI (PAA)
+documentation. If a field is not being used, mark it 'null' without the single
+quotes. ```json { "sensor_index": 53, "read_key": null, "fields": null } ``` Or
+see this [file](./sample_json_config_files/
+sample_single_sensor_request_json_file.json) for another example. > Note: Refer
+to the PurpleAirAPI (PAA) documentation for more information.
+api.purpleair.com/#api-sensors-get-sensor-data> ### PAA Multiple Sensor Request
+Example Out of the parameters listed below only "fields" is required. The
+others are all optional according to PurpleAirAPI (PAA) documentation. If a
+field is not being used, mark it 'null' without the single quotes. ```json
+{ "fields": "A string comma delimited string of fields to retrieve. i.e
+fields,name,etc", "location_type": null, "read_keys": null, "show_only": null,
+"modified_since": null, "max_age": null, "nwlng" : null, "nwlat": null,
+"selng": null, "selat": null } ``` Or see this [file](./
+sample_json_config_files/sample_multiple_sensor_request_json_file.json) for
+another example. > Note: Refer to the PurpleAirAPI (PAA) documentation for more
+information.
+api.purpleair.com/#api-sensors-get-sensors-data> The below snippet is taken
+From the PurpleAirAPI (PAA) documentation: ```plain text Field Type Description
+fields String The 'Fields' parameter specifies which 'sensor data fields' to
+include in the response. It is a comma separated list with one or more of the
+following: Station information and status fields: name, icon, model, hardware,
+location_type, private, latitude, longitude, altitude, position_rating,
+led_brightness, firmware_version, firmware_upgrade, rssi, uptime, pa_latency,
+memory, last_seen, last_modified, date_created, channel_state, channel_flags,
+channel_flags_manual, channel_flags_auto, confidence, confidence_manual,
+confidence_auto Environmental fields: humidity, humidity_a, humidity_b,
+temperature, temperature_a, temperature_b, pressure, pressure_a, pressure_b
+Miscellaneous fields: voc, voc_a, voc_b, ozone1, analog_input PM1.0 fields:
+pm1.0, pm1.0_a, pm1.0_b, pm1.0_atm, pm1.0_atm_a, pm1.0_atm_b, pm1.0_cf_1,
+pm1.0_cf_1_a, pm1.0_cf_1_b PM2.5 fields: pm2.5_alt, pm2.5_alt_a, pm2.5_alt_b,
+pm2.5, pm2.5_a, pm2.5_b, pm2.5_atm, pm2.5_atm_a, pm2.5_atm_b, pm2.5_cf_1,
+pm2.5_cf_1_a, pm2.5_cf_1_b PM2.5 pseudo (simple running) average fields:
+pm2.5_10minute, pm2.5_10minute_a, pm2.5_10minute_b, pm2.5_30minute,
+pm2.5_30minute_a, pm2.5_30minute_b, pm2.5_60minute, pm2.5_60minute_a,
+pm2.5_60minute_b, pm2.5_6hour, pm2.5_6hour_a, pm2.5_6hour_b, pm2.5_24hour,
+pm2.5_24hour_a, pm2.5_24hour_b, pm2.5_1week, pm2.5_1week_a, pm2.5_1week_b
+PM10.0 fields: pm10.0, pm10.0_a, pm10.0_b, pm10.0_atm, pm10.0_atm_a,
+pm10.0_atm_b, pm10.0_cf_1, pm10.0_cf_1_a, pm10.0_cf_1_b Visibility fields:
 scattering_coefficient, scattering_coefficient_a, scattering_coefficient_b,
 deciviews, deciviews_a, deciviews_b, visual_range, visual_range_a,
 visual_range_b Particle count fields: 0.3_um_count, 0.3_um_count_a,
 0.3_um_count_b, 0.5_um_count, 0.5_um_count_a, 0.5_um_count_b, 1.0_um_count,
 1.0_um_count_a, 1.0_um_count_b, 2.5_um_count, 2.5_um_count_a, 2.5_um_count_b,
 5.0_um_count, 5.0_um_count_a, 5.0_um_count_b, 10.0_um_count 10.0_um_count_a,
 10.0_um_count_b ThingSpeak fields, used to retrieve data from
@@ -146,8 +192,26 @@
 updated within the last number of seconds. Using a value of 0 will match
 sensors of any age. Default value: 604800 nwlng optional Number A north west
 longitude for the bounding box. Use a bounding box to limit the sensors
 returned to a specific geographic area. The bounding box is defined by two
 points, a north west latitude/longitude and a south east latitude/longitude.
 nwlat optional Number A north west latitude for the bounding box. selng
 optional Number A south east longitude for the bounding box. selat optional
-Number A south east latitude for the bounding box.
+Number A south east latitude for the bounding box. ``` ### PAA Group Sensor
+Request Example Out of the parameters below `sensor_group_name`,
+`add_sensors_to_group`, and `sensor_index_list` are custom settings not defined
+in the official PAA documentation. These three setting help drive the `group`
+request feature. `sensor_group_name` - This will be the name assigned to your
+group. If it doesn't exist already, it will be created. Otherwise, the first
+group matching the name will be used. `add_sensors_to_group` - If true, adds
+the sensors in the `sensor_index_list`. If false, `sensor_index_list` is
+ignored. `sensor_index_list` - A list of sensor indexes that will be added to
+your group if they don't already exist. The rest of the settings are official
+PAA settings. They are the same as the [### PAA Multiple Sensor Request
+Example](#paa-multiple-sensor-request-example). Refer above for details.
+```json { "sensor_group_name": "A Name Goes Here", "add_sensors_to_group":
+true, "sensor_index_list": [ 77, 81, 95079, 167897 ], "fields": "A string comma
+delimited string of fields to retrieve. i.e fields,name,etc", "location_type":
+null, "read_keys": null, "show_only": null, "modified_since": null, "max_age":
+null, "nwlng" : null, "nwlat": null, "selng": null, "selat": null } ``` Or see
+this [file](./sample_json_config_files/
+sample_group_sensor_request_json_file.json) for another example.
```

### Comparing `purpleair_data_logger-1.2.0a2/purpleair_data_logger/PurpleAirCSVDataLogger.py` & `purpleair_data_logger-1.2.1a1/purpleair_data_logger/PurpleAirCSVDataLogger.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 #!/usr/bin/env python3
 
 """
-    Copyright 2022 carlkid1499, All rights reserved.
+    Copyright 2023 carlkidcrypto, All rights reserved.
     A python class designed to use the PurpleAirAPI for requesting sensor(s) data.
     Data will be inserted into CSV files.
     
     For best practice from PurpleAir:
     "The data from individual sensors will update no less than every 30 seconds.
     As a courtesy, we ask that you limit the number of requests to no more than
     once every 1 to 10 minutes, assuming you are only using the API to obtain data
     from sensors. If retrieving data from multiple sensors at once, please send a
     single request rather than individual requests in succession."
 """
 
-from purpleair_data_logger.PurpleAirDataLogger import PurpleAirDataLogger
+from purpleair_data_logger.PurpleAirDataLogger import (
+    PurpleAirDataLogger,
+    generate_common_arg_parser,
+)
 from purpleair_data_logger.PurpleAirCSVDataLoggerConstants import (
     STATION_INFORMATION_AND_STATUS_FIELDS_FILE_NAME,
     STATION_INFORMATION_AND_STATUS_FIELDS_HEADER,
     ENVIRONMENTAL_FIELDS_FILE_NAME,
     ENVIRONMENTAL_FIELDS_HEADER,
     MISCELLANEOUS_FIELDS_FILE_NAME,
     MISCELLANEOUS_FIELDS_HEADER,
@@ -32,31 +35,32 @@
     PARTICLE_COUNT_FIELDS_FILE_NAME,
     PARTICLE_COUNT_FIELDS_HEADER,
     THINGSPEAK_FIELDS_FILE_NAME,
     THINGSPEAK_FIELDS_HEADER,
 )
 from os import makedirs
 from os.path import exists
-import argparse
 
 
 class PurpleAirCSVDataLogger(PurpleAirDataLogger):
     """
     The logger class. For now we will insert data into a CSV file.
     """
 
-    def __init__(self, PurpleAirAPIReadKey, path_to_save_csv_files_in):
+    def __init__(
+        self, PurpleAirAPIReadKey, PurpleAirAPIWriteKey, path_to_save_csv_files_in
+    ):
         """
         :param str PurpleAirAPIReadKey: A valid PurpleAirAPI Read key
         :param object path_to_save_csv_files_in: A string directory path
                                                  to save files in.
         """
 
         # Inherit everything from the parent base class: PurpleAirDataLogger
-        super().__init__(PurpleAirAPIReadKey)
+        super().__init__(PurpleAirAPIReadKey, PurpleAirAPIWriteKey)
 
         # save off the store path internally for later access
         self._path_to_save_csv_files_in = path_to_save_csv_files_in
 
         # Init some class vars
         self._did_we_write_the_header_bool = False
         self._data_error_counter = 0
@@ -482,61 +486,37 @@
         self._close_and_flush_csv_file(pm2_5_pseudo_average_fields_file_stream)
         self._close_and_flush_csv_file(pm10_0_fields_file_stream)
         self._close_and_flush_csv_file(particle_count_fields_file_stream)
         self._close_and_flush_csv_file(thingspeak_fields_file_stream)
 
 
 if __name__ == "__main__":
-    parser = argparse.ArgumentParser(
-        description="Collect data from PurpleAir sensors and store it in CSV files!"
+    parser = generate_common_arg_parser(
+        "Collect data from PurpleAir sensors and store it in CSV files!"
     )
+
     parser.add_argument(
         "-save_file_path",
         required=True,
         dest="save_file_path",
         type=str,
         help="""The path to save CSV files in.""",
     )
-    parser.add_argument(
-        "-paa_read_key",
-        required=True,
-        dest="paa_read_key",
-        type=str,
-        help="""The PurpleAirAPI Read key""",
-    )
-    parser.add_argument(
-        "-paa_single_sensor_request_json_file",
-        required=False,
-        default=None,
-        dest="paa_single_sensor_request_json_file",
-        type=str,
-        help="""The
-                        path to a json file containing the parameters to send a single
-                        sensor request.""",
-    )
-    parser.add_argument(
-        "-paa_multiple_sensor_request_json_file",
-        required=False,
-        default=None,
-        dest="paa_multiple_sensor_request_json_file",
-        type=str,
-        help="""The
-                        path to a json file containing the parameters to send a multiple
-                        sensor request.""",
-    )
 
     args = parser.parse_args()
 
     # Place holders that are used later down
     the_json_file = None
     file_obj = None
 
     # Second make an instance our our data logger
     the_paa_csv_data_logger = PurpleAirCSVDataLogger(
-        args.paa_read_key, args.save_file_path
+        args.paa_read_key, args.paa_write_key, args.save_file_path
     )
 
-    # Third choose what run method to execute depending on paa_multiple_sensor_request_json_file/paa_single_sensor_request_json_file
+    # Third choose what run method to execute depending on
+    # paa_multiple_sensor_request_json_file/paa_single_sensor_request_json_file/paa_group_sensor_request_json_file
     the_paa_csv_data_logger.validate_parameters_and_run(
         args.paa_multiple_sensor_request_json_file,
         args.paa_single_sensor_request_json_file,
+        args.paa_group_sensor_request_json_file,
     )
```

### Comparing `purpleair_data_logger-1.2.0a2/purpleair_data_logger/PurpleAirCSVDataLoggerConstants.py` & `purpleair_data_logger-1.2.1a1/purpleair_data_logger/PurpleAirCSVDataLoggerConstants.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env python3
 
 """
-    Copyright 2022 carlkid1499, All rights reserved.
+    Copyright 2022 carlkidcrypto, All rights reserved.
     A file containing CSVDataLogger constants.
 """
 
 #: Standard file name for -
 STATION_INFORMATION_AND_STATUS_FIELDS_FILE_NAME = (
     """station_information_and_status_fields.csv"""
 )
```

### Comparing `purpleair_data_logger-1.2.0a2/purpleair_data_logger/PurpleAirPSQLDataLogger.py` & `purpleair_data_logger-1.2.1a1/purpleair_data_logger/PurpleAirPSQLDataLogger.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 #!/usr/bin/env python3
 
 """
-    Copyright 2022 carlkid1499, All rights reserved.
+    Copyright 2023 carlkidcrypto, All rights reserved.
     A python class designed to use the PurpleAirAPI for requesting sensor(s) data.
     Data will be inserted into a PSQL database.
 
     For best practice from PurpleAir:
     "The data from individual sensors will update no less than every 30 seconds.
     As a courtesy, we ask that you limit the number of requests to no more than
     once every 1 to 10 minutes, assuming you are only using the API to obtain data
     from sensors. If retrieving data from multiple sensors at once, please send a
     single request rather than individual requests in succession."
 """
 
-from purpleair_data_logger.PurpleAirDataLogger import PurpleAirDataLogger
+from purpleair_data_logger.PurpleAirDataLogger import (
+    PurpleAirDataLogger,
+    generate_common_arg_parser,
+)
 from purpleair_data_logger.PurpleAirPSQLQueryStatements import (
     PSQL_INSERT_STATEMENT_ENVIRONMENTAL_FIELDS,
     PSQL_INSERT_STATEMENT_MISCELLANEOUS_FIELDS,
     PSQL_INSERT_STATEMENT_PARTICLE_COUNT_FIELDS,
     PSQL_INSERT_STATEMENT_PM10_0_FIELDS,
     PSQL_INSERT_STATEMENT_PM1_0_FIELDS,
     PSQL_INSERT_STATEMENT_PM2_5_FIELDS,
@@ -36,33 +39,32 @@
     PSQL_DROP_ALL_TABLES,
     PSQL_GET_LIST_OF_ACTIVE_COMPRESSION_POLICIES,
     PSQL_CREATE_MATERIALIZED_VIEW_SENSOR_INDEX_AND_NAME_1HOUR_AGGREGATE,
     PSQL_CREATE_CONTINUOUS_AGGREGATE_POLICY_ON_SENSOR_INDEX_AND_NAME_1HOUR_AGGREGATE,
     PSQL_CREATE_DATA_RETENTION_POLICY_ON_SENSOR_INDEX_AND_NAME_1HOUR_AGGREGATE,
 )
 import pg8000
-import argparse
 from datetime import datetime, timezone
 import sys
 
 
 class PurpleAirPSQLDataLogger(PurpleAirDataLogger):
     """
     The logger class. For now we will ingest data into a TimeScaleDB PostgreSQL
     database. Then we will use Grafana to visualize said data.
     """
 
-    def __init__(self, PurpleAirAPIReadKey, psql_db_conn):
+    def __init__(self, PurpleAirAPIReadKey, PurpleAirAPIWriteKey, psql_db_conn):
         """
         :param str PurpleAirAPIReadKey: A valid PurpleAirAPI Read key
         :param object psql_db_conn: A valid PG8000 database connection
         """
 
         # Inherit everything from the parent base class: PurpleAirDataLogger
-        super().__init__(PurpleAirAPIReadKey)
+        super().__init__(PurpleAirAPIReadKey, PurpleAirAPIWriteKey)
 
         # Make our psql database connection
         self._db_conn = psql_db_conn
 
         # A list of all acceptable table names
         self._acceptable_table_names_string_list = [
             "station_information_and_status_fields",
@@ -84,14 +86,46 @@
 
         # Create compression policies
         self._configure_data_compression_policies()
 
         # Create continuous aggregates and materialized views
         self._configure_continuous_aggregates()
 
+        # Create some prepared statements
+        self._db_prepared_statements = {}
+        self._db_prepared_statements[
+            "station_information_and_status_fields"
+        ] = self._db_conn.prepare(
+            PSQL_INSERT_STATEMENT_STATION_INFORMATION_AND_STATUS_FIELDS
+        )
+        self._db_prepared_statements["environmental_fields"] = self._db_conn.prepare(
+            PSQL_INSERT_STATEMENT_ENVIRONMENTAL_FIELDS
+        )
+        self._db_prepared_statements["miscellaneous_fields"] = self._db_conn.prepare(
+            PSQL_INSERT_STATEMENT_MISCELLANEOUS_FIELDS
+        )
+        self._db_prepared_statements["pm1_0_fields"] = self._db_conn.prepare(
+            PSQL_INSERT_STATEMENT_PM1_0_FIELDS
+        )
+        self._db_prepared_statements["pm2_5_fields"] = self._db_conn.prepare(
+            PSQL_INSERT_STATEMENT_PM2_5_FIELDS
+        )
+        self._db_prepared_statements[
+            "pm2_5_pseudo_average_fields"
+        ] = self._db_conn.prepare(PSQL_INSERT_STATEMENT_PM2_5_PSEUDO_AVERAGE_FIELDS)
+        self._db_prepared_statements["pm10_0_fields"] = self._db_conn.prepare(
+            PSQL_INSERT_STATEMENT_PM10_0_FIELDS
+        )
+        self._db_prepared_statements["particle_count_fields"] = self._db_conn.prepare(
+            PSQL_INSERT_STATEMENT_PARTICLE_COUNT_FIELDS
+        )
+        self._db_prepared_statements["thingspeak_fields"] = self._db_conn.prepare(
+            PSQL_INSERT_STATEMENT_THINGSPEAK_FIELDS
+        )
+
         # Commit to the db
         self._db_conn.commit()
 
     @property
     def get_acceptable_table_names_string_list(self):
         """
         A getter method that will simply return the contents of
@@ -195,16 +229,15 @@
                                              for insertion. If a sensor doesn't support
                                              a certain field make sure it is NULL and part
                                              of the dictionary. This method does no type
                                              or error checking. That is upto the caller.
         """
 
         # Run the queries
-        self._db_conn.run(
-            PSQL_INSERT_STATEMENT_STATION_INFORMATION_AND_STATUS_FIELDS,
+        self._db_prepared_statements["station_information_and_status_fields"].run(
             data_time_stamp=self._convert_unix_epoch_timestamp_to_psql_timestamp(
                 single_sensor_data_dict["data_time_stamp"]
             ),
             sensor_index=single_sensor_data_dict["sensor_index"],
             name=single_sensor_data_dict["name"],
             icon=single_sensor_data_dict["icon"],
             model=single_sensor_data_dict["model"],
@@ -236,16 +269,15 @@
             channel_flags_manual=single_sensor_data_dict["channel_flags_manual"],
             channel_flags_auto=single_sensor_data_dict["channel_flags_auto"],
             confidence=single_sensor_data_dict["confidence"],
             confidence_manual=single_sensor_data_dict["confidence_manual"],
             confidence_auto=single_sensor_data_dict["confidence_auto"],
         )
 
-        self._db_conn.run(
-            PSQL_INSERT_STATEMENT_ENVIRONMENTAL_FIELDS,
+        self._db_prepared_statements["environmental_fields"].run(
             data_time_stamp=self._convert_unix_epoch_timestamp_to_psql_timestamp(
                 single_sensor_data_dict["data_time_stamp"]
             ),
             sensor_index=single_sensor_data_dict["sensor_index"],
             humidity=single_sensor_data_dict["humidity"],
             humidity_a=single_sensor_data_dict["humidity_a"],
             humidity_b=single_sensor_data_dict["humidity_b"],
@@ -253,29 +285,27 @@
             temperature_a=single_sensor_data_dict["temperature_a"],
             temperature_b=single_sensor_data_dict["temperature_b"],
             pressure=single_sensor_data_dict["pressure"],
             pressure_a=single_sensor_data_dict["pressure_a"],
             pressure_b=single_sensor_data_dict["pressure_b"],
         )
 
-        self._db_conn.run(
-            PSQL_INSERT_STATEMENT_MISCELLANEOUS_FIELDS,
+        self._db_prepared_statements["miscellaneous_fields"].run(
             data_time_stamp=self._convert_unix_epoch_timestamp_to_psql_timestamp(
                 single_sensor_data_dict["data_time_stamp"]
             ),
             sensor_index=single_sensor_data_dict["sensor_index"],
             voc=single_sensor_data_dict["voc"],
             voc_a=single_sensor_data_dict["voc_a"],
             voc_b=single_sensor_data_dict["voc_b"],
             ozone1=single_sensor_data_dict["ozone1"],
             analog_input=single_sensor_data_dict["analog_input"],
         )
 
-        self._db_conn.run(
-            PSQL_INSERT_STATEMENT_PM1_0_FIELDS,
+        self._db_prepared_statements["pm1_0_fields"].run(
             data_time_stamp=self._convert_unix_epoch_timestamp_to_psql_timestamp(
                 single_sensor_data_dict["data_time_stamp"]
             ),
             sensor_index=single_sensor_data_dict["sensor_index"],
             pm1_0=single_sensor_data_dict["pm1.0"],
             pm1_0_a=single_sensor_data_dict["pm1.0_a"],
             pm1_0_b=single_sensor_data_dict["pm1.0_b"],
@@ -283,16 +313,15 @@
             pm1_0_atm_a=single_sensor_data_dict["pm1.0_atm_a"],
             pm1_0_atm_b=single_sensor_data_dict["pm1.0_atm_b"],
             pm1_0_cf_1=single_sensor_data_dict["pm1.0_cf_1"],
             pm1_0_cf_1_a=single_sensor_data_dict["pm1.0_cf_1_a"],
             pm1_0_cf_1_b=single_sensor_data_dict["pm1.0_cf_1_b"],
         )
 
-        self._db_conn.run(
-            PSQL_INSERT_STATEMENT_PM2_5_FIELDS,
+        self._db_prepared_statements["pm2_5_fields"].run(
             data_time_stamp=self._convert_unix_epoch_timestamp_to_psql_timestamp(
                 single_sensor_data_dict["data_time_stamp"]
             ),
             sensor_index=single_sensor_data_dict["sensor_index"],
             pm2_5_alt=single_sensor_data_dict["pm2.5_alt"],
             pm2_5_alt_a=single_sensor_data_dict["pm2.5_alt_a"],
             pm2_5_alt_b=single_sensor_data_dict["pm2.5_alt_b"],
@@ -303,16 +332,15 @@
             pm2_5_atm_a=single_sensor_data_dict["pm2.5_atm_a"],
             pm2_5_atm_b=single_sensor_data_dict["pm2.5_atm_b"],
             pm2_5_cf_1=single_sensor_data_dict["pm2.5_cf_1"],
             pm2_5_cf_1_a=single_sensor_data_dict["pm2.5_cf_1_a"],
             pm2_5_cf_1_b=single_sensor_data_dict["pm2.5_cf_1_b"],
         )
 
-        self._db_conn.run(
-            PSQL_INSERT_STATEMENT_PM2_5_PSEUDO_AVERAGE_FIELDS,
+        self._db_prepared_statements["pm2_5_pseudo_average_fields"].run(
             data_time_stamp=self._convert_unix_epoch_timestamp_to_psql_timestamp(
                 single_sensor_data_dict["data_time_stamp"]
             ),
             sensor_index=single_sensor_data_dict["sensor_index"],
             pm2_5_10minute=single_sensor_data_dict["pm2.5_10minute"],
             pm2_5_10minute_a=single_sensor_data_dict["pm2.5_10minute_a"],
             pm2_5_10minute_b=single_sensor_data_dict["pm2.5_10minute_b"],
@@ -329,16 +357,15 @@
             pm2_5_24hour_a=single_sensor_data_dict["pm2.5_24hour_a"],
             pm2_5_24hour_b=single_sensor_data_dict["pm2.5_24hour_b"],
             pm2_5_1week=single_sensor_data_dict["pm2.5_1week"],
             pm2_5_1week_a=single_sensor_data_dict["pm2.5_1week_a"],
             pm2_5_1week_b=single_sensor_data_dict["pm2.5_1week_b"],
         )
 
-        self._db_conn.run(
-            PSQL_INSERT_STATEMENT_PM10_0_FIELDS,
+        self._db_prepared_statements["pm10_0_fields"].run(
             data_time_stamp=self._convert_unix_epoch_timestamp_to_psql_timestamp(
                 single_sensor_data_dict["data_time_stamp"]
             ),
             sensor_index=single_sensor_data_dict["sensor_index"],
             pm10_0=single_sensor_data_dict["pm10.0"],
             pm10_0_a=single_sensor_data_dict["pm10.0_a"],
             pm10_0_b=single_sensor_data_dict["pm10.0_b"],
@@ -346,16 +373,15 @@
             pm10_0_atm_a=single_sensor_data_dict["pm10.0_atm_a"],
             pm10_0_atm_b=single_sensor_data_dict["pm10.0_atm_b"],
             pm10_0_cf_1=single_sensor_data_dict["pm10.0_cf_1"],
             pm10_0_cf_1_a=single_sensor_data_dict["pm10.0_cf_1_a"],
             pm10_0_cf_1_b=single_sensor_data_dict["pm10.0_cf_1_b"],
         )
 
-        self._db_conn.run(
-            PSQL_INSERT_STATEMENT_PARTICLE_COUNT_FIELDS,
+        self._db_prepared_statements["particle_count_fields"].run(
             data_time_stamp=self._convert_unix_epoch_timestamp_to_psql_timestamp(
                 single_sensor_data_dict["data_time_stamp"]
             ),
             sensor_index=single_sensor_data_dict["sensor_index"],
             um_count_0_3=single_sensor_data_dict["0.3_um_count"],
             um_count_a_0_3=single_sensor_data_dict["0.3_um_count_a"],
             um_count_b_0_3=single_sensor_data_dict["0.3_um_count_b"],
@@ -372,16 +398,15 @@
             um_count_a_5_0=single_sensor_data_dict["5.0_um_count_a"],
             um_count_b_5_0=single_sensor_data_dict["5.0_um_count_b"],
             um_count_10_0=single_sensor_data_dict["10.0_um_count"],
             um_count_a_10_0=single_sensor_data_dict["10.0_um_count_a"],
             um_count_b_10_0=single_sensor_data_dict["10.0_um_count_b"],
         )
 
-        self._db_conn.run(
-            PSQL_INSERT_STATEMENT_THINGSPEAK_FIELDS,
+        self._db_prepared_statements["thingspeak_fields"].run(
             data_time_stamp=self._convert_unix_epoch_timestamp_to_psql_timestamp(
                 single_sensor_data_dict["data_time_stamp"]
             ),
             sensor_index=single_sensor_data_dict["sensor_index"],
             primary_id_a=single_sensor_data_dict["primary_id_a"],
             primary_key_a=single_sensor_data_dict["primary_key_a"],
             secondary_id_a=single_sensor_data_dict["secondary_id_a"],
@@ -391,19 +416,23 @@
             secondary_id_b=single_sensor_data_dict["secondary_id_b"],
             secondary_key_b=single_sensor_data_dict["secondary_key_b"],
         )
 
         # Commit to the db
         self._db_conn.commit()
 
+        # Delete some stuff
+        del single_sensor_data_dict
+
 
 if __name__ == "__main__":
-    parser = argparse.ArgumentParser(
-        description="Collect data from PurpleAir sensors and insert into a database!"
+    parser = generate_common_arg_parser(
+        "Collect data from PurpleAir sensors and insert into a database!"
     )
+
     parser.add_argument(
         "-db_drop_all_tables",
         action="store_true",
         required=False,
         dest="db_drop_all_tables",
         help="""Set this flag if you wish to drop all
                         tables before loading in new data. Useful if a database change has happened.
@@ -440,41 +469,14 @@
         "-db_pwd",
         required=False,
         default=None,
         dest="db_pwd",
         type=str,
         help="""The PSQL database password""",
     )
-    parser.add_argument(
-        "-paa_read_key",
-        required=True,
-        dest="paa_read_key",
-        type=str,
-        help="""The PurpleAirAPI Read key""",
-    )
-    parser.add_argument(
-        "-paa_single_sensor_request_json_file",
-        required=False,
-        default=None,
-        dest="paa_single_sensor_request_json_file",
-        type=str,
-        help="""The
-                        path to a json file containing the parameters to send a single
-                        sensor request.""",
-    )
-    parser.add_argument(
-        "-paa_multiple_sensor_request_json_file",
-        required=False,
-        default=None,
-        dest="paa_multiple_sensor_request_json_file",
-        type=str,
-        help="""The
-                        path to a json file containing the parameters to send a multiple
-                        sensor request.""",
-    )
 
     args = parser.parse_args()
 
     # Place holders that are used later down
     the_json_file = None
     file_obj = None
 
@@ -502,15 +504,17 @@
             the_psql_db_conn.commit()
             sys.exit(
                 """All database tables have been dropped. Please rerun with a db_usr who only has insert rights provided..."""
             )
 
     # Third make an instance our our data logger
     the_paa_psql_data_logger = PurpleAirPSQLDataLogger(
-        args.paa_read_key, the_psql_db_conn
+        args.paa_read_key, args.paa_write_key, the_psql_db_conn
     )
 
-    # Fourth choose what run method to execute depending on paa_multiple_sensor_request_json_file/paa_single_sensor_request_json_file
+    # Fourth choose what run method to execute depending on
+    # paa_multiple_sensor_request_json_file/paa_single_sensor_request_json_file/paa_group_sensor_request_json_file
     the_paa_psql_data_logger.validate_parameters_and_run(
         args.paa_multiple_sensor_request_json_file,
         args.paa_single_sensor_request_json_file,
+        args.paa_group_sensor_request_json_file,
     )
```

### Comparing `purpleair_data_logger-1.2.0a2/purpleair_data_logger/PurpleAirPSQLQueryStatements.py` & `purpleair_data_logger-1.2.1a1/purpleair_data_logger/PurpleAirPSQLQueryStatements.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env python3
 
 """
-    Copyright 2022 carlkid1499, All rights reserved.
+    Copyright 2022 carlkidcrypto, All rights reserved.
     A file containing PSQL statements defined as constants.
     Generate the PSQL query strings. For simplicity our table names will match
     what the PurpleAir documentation says. We will do the same for table column names.
 """
 
 #: PSQL statement for station_information_and_status_fields table
 CREATE_STATION_INFORMATION_AND_STATUS_FIELDS_TABLE = """
```

### Comparing `purpleair_data_logger-1.2.0a2/purpleair_data_logger/PurpleAirSQLiteDataLogger.py` & `purpleair_data_logger-1.2.1a1/purpleair_data_logger/PurpleAirSQLiteDataLogger.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 #!/usr/bin/env python3
 
 """
-    Copyright 2022 carlkid1499, All rights reserved.
+    Copyright 2023 carlkidcrypto, All rights reserved.
     A python class designed to use the PurpleAirAPI for requesting sensor(s) data.
     Data will be inserted into a SQLite3 database file.
     
     For best practice from PurpleAir:
     "The data from individual sensors will update no less than every 30 seconds.
     As a courtesy, we ask that you limit the number of requests to no more than
     once every 1 to 10 minutes, assuming you are only using the API to obtain data
     from sensors. If retrieving data from multiple sensors at once, please send a
     single request rather than individual requests in succession."
 """
 
-from purpleair_data_logger.PurpleAirDataLogger import PurpleAirDataLogger
+from purpleair_data_logger.PurpleAirDataLogger import (
+    PurpleAirDataLogger,
+    generate_common_arg_parser,
+)
 from purpleair_data_logger.PurpleAirSQLiteQueryStatements import (
     SQLITE_INSERT_STATEMENT_ENVIRONMENTAL_FIELDS,
     SQLITE_INSERT_STATEMENT_MISCELLANEOUS_FIELDS,
     SQLITE_INSERT_STATEMENT_PARTICLE_COUNT_FIELDS,
     SQLITE_INSERT_STATEMENT_PM10_0_FIELDS,
     SQLITE_INSERT_STATEMENT_PM1_0_FIELDS,
     SQLITE_INSERT_STATEMENT_PM2_5_FIELDS,
@@ -31,30 +34,32 @@
     CREATE_PM2_5_PSEUDO_AVERAGE_FIELDS,
     CREATE_ENVIRONMENTAL_FIELDS_TABLE,
     CREATE_MISCELLANEOUS_FIELDS,
     CREATE_STATION_INFORMATION_AND_STATUS_FIELDS_TABLE,
     CREATE_THINGSPEAK_FIELDS,
     SQLITE_DROP_ALL_TABLES,
 )
-import argparse
+
 import sqlite3
 
 
 class PurpleAirSQLiteDataLogger(PurpleAirDataLogger):
     """
     The logger class. For now we will insert data into a SQLite3 database file.
     """
 
-    def __init__(self, PurpleAirAPIReadKey, sqlite_data_base_name):
+    def __init__(
+        self, PurpleAirAPIReadKey, PurpleAirAPIWriteKey, sqlite_data_base_name
+    ):
         """
         :param str PurpleAirAPIReadKey: A valid PurpleAirAPI Read key
         """
 
         # Inherit everything from the parent base class: PurpleAirDataLogger
-        super().__init__(PurpleAirAPIReadKey)
+        super().__init__(PurpleAirAPIReadKey, PurpleAirAPIWriteKey)
 
         self._db_conn = sqlite3.connect(sqlite_data_base_name)
 
         # Make our PSQL Tables
         self._create_sqlite_db_tables()
 
     def _create_sqlite_db_tables(self):
@@ -277,62 +282,38 @@
         )
 
         # Commit to the db
         self._db_conn.commit()
 
 
 if __name__ == "__main__":
-    parser = argparse.ArgumentParser(
-        description="Collect data from PurpleAir sensors and store it a SQLite3 database file!"
+    parser = generate_common_arg_parser(
+        "Collect data from PurpleAir sensors and store it a SQLite3 database file!"
     )
+
     parser.add_argument(
         "-db_name",
         required=True,
         dest="db_name",
         type=str,
         help="""The path and name for the SQLite3 database
                         file! i.e database_name.db""",
     )
-    parser.add_argument(
-        "-paa_read_key",
-        required=True,
-        dest="paa_read_key",
-        type=str,
-        help="""The PurpleAirAPI Read key""",
-    )
-    parser.add_argument(
-        "-paa_single_sensor_request_json_file",
-        required=False,
-        default=None,
-        dest="paa_single_sensor_request_json_file",
-        type=str,
-        help="""The
-                        path to a json file containing the parameters to send a single
-                        sensor request.""",
-    )
-    parser.add_argument(
-        "-paa_multiple_sensor_request_json_file",
-        required=False,
-        default=None,
-        dest="paa_multiple_sensor_request_json_file",
-        type=str,
-        help="""The
-                        path to a json file containing the parameters to send a multiple
-                        sensor request.""",
-    )
 
     args = parser.parse_args()
 
     # Place holders that are used later down
     the_json_file = None
     file_obj = None
 
     # Second make an instance our our data logger
     the_paa_sqlite_data_logger = PurpleAirSQLiteDataLogger(
-        args.paa_read_key, args.db_name
+        args.paa_read_key, args.paa_write_key, args.db_name
     )
 
-    # Third choose what run method to execute depending on paa_multiple_sensor_request_json_file/paa_single_sensor_request_json_file
+    # Third choose what run method to execute depending on
+    # paa_multiple_sensor_request_json_file/paa_single_sensor_request_json_file/paa_group_sensor_request_json_file
     the_paa_sqlite_data_logger.validate_parameters_and_run(
         args.paa_multiple_sensor_request_json_file,
         args.paa_single_sensor_request_json_file,
+        args.paa_group_sensor_request_json_file,
     )
```

### Comparing `purpleair_data_logger-1.2.0a2/purpleair_data_logger/PurpleAirSQLiteQueryStatements.py` & `purpleair_data_logger-1.2.1a1/purpleair_data_logger/PurpleAirSQLiteQueryStatements.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env python3
 
 """
-    Copyright 2022 carlkid1499, All rights reserved.
+    Copyright 2022 carlkidcrypto, All rights reserved.
     A file containing SQLITE statements defined as constants.
     Generate the SQLITE query strings. For simplicity our table names will match
     what the PurpleAir documentation says. We will do the same for table column names.
 """
 
 #: SQLITE statement for station_information_and_status_fields table
 CREATE_STATION_INFORMATION_AND_STATUS_FIELDS_TABLE = """
```

### Comparing `purpleair_data_logger-1.2.0a2/purpleair_data_logger.egg-info/PKG-INFO` & `purpleair_data_logger-1.2.1a1/purpleair_data_logger.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,75 +1,93 @@
 Metadata-Version: 2.1
 Name: purpleair-data-logger
-Version: 1.2.0a2
-Home-page: https://github.com/carlkid1499/purpleair_data_logger
+Version: 1.2.1a1
+Home-page: https://github.com/carlkidcrypto/purpleair_data_logger
 Author: Carlos Santos
-Author-email: 27721404+carlkid1499@users.noreply.github.com
+Author-email: dose.lucky.sake@cloak.id
 License: MIT
 Keywords: purpleair_data_logger,purple air,purple air data logger,PurpleAirPSQLDataLogger,PurpleAirCSVDataLogger,purple air api,PurpleAirSQLiteDataLogger
 Platform: Windows 32/64
 Platform: Linux 32/64
 Platform: MacOS 32/64
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# purple_air_data_logger
+# Purple Air Data Logger(s) (PADLs)
 
 A set of data logger(s) that will query purple air sensor(s) for data. That data will then be ingested into a TimeScaleDB PostGreSQL database, CSV files, or a SQLite3 database. To use these tools a PurpleAPI key is required. You can get API keys by sending an email to `contact@purpleair.com` with a first and last name to assign them to.
 
-| [![Behave Tests](https://github.com/carlkid1499/purpleair_data_logger/actions/workflows/behave_tests.yml/badge.svg?branch=main)](https://github.com/carlkid1499/purpleair_data_logger/actions/workflows/behave_tests.yml) | [![PyPI Distributions](https://github.com/carlkid1499/purpleair_data_logger/actions/workflows/build_and_publish_to_pypi.yml/badge.svg?branch=main)](https://github.com/carlkid1499/purpleair_data_logger/actions/workflows/build_and_publish_to_pypi.yml) | [![TestPyPI Distributions](https://github.com/carlkid1499/purpleair_data_logger/actions/workflows/build_and_publish_to_test_pypi.yml/badge.svg?branch=main)](https://github.com/carlkid1499/purpleair_data_logger/actions/workflows/build_and_publish_to_test_pypi.yml) |
-| --------------- | --------------- | --------------- |
+| [![Behave Tests](https://github.com/carlkidcrypto/purpleair_data_logger/actions/workflows/behave_tests.yml/badge.svg?branch=main)](https://github.com/carlkidcrypto/purpleair_data_logger/actions/workflows/behave_tests.yml) | [![PyPI Distributions](https://github.com/carlkidcrypto/purpleair_data_logger/actions/workflows/build_and_publish_to_pypi.yml/badge.svg?branch=main)](https://github.com/carlkidcrypto/purpleair_data_logger/actions/workflows/build_and_publish_to_pypi.yml) | [![TestPyPI Distributions](https://github.com/carlkidcrypto/purpleair_data_logger/actions/workflows/build_and_publish_to_test_pypi.yml/badge.svg?branch=main)](https://github.com/carlkidcrypto/purpleair_data_logger/actions/workflows/build_and_publish_to_test_pypi.yml) | [![Black](https://github.com/carlkidcrypto/purpleair_data_logger/actions/workflows/black.yml/badge.svg)](https://github.com/carlkidcrypto/purpleair_data_logger/actions/workflows/black.yml) |
+| --------------- | --------------- | --------------- | --------------- |
 
 ## How to Support This Project
 
-<a href="https://www.buymeacoffee.com/carlkid1499" target="_blank"><img src="https://cdn.buymeacoffee.com/buttons/default-orange.png" alt="Buy Me A Coffee" height="41" width="174"></a>
+<a href="https://www.buymeacoffee.com/carlkidcrypto" target="_blank"><img src="https://cdn.buymeacoffee.com/buttons/default-orange.png" alt="Buy Me A Coffee" height="41" width="174"></a>
 
 ## Installation
 
 You can install the PurpleAir Data Logger via pip.
 
 ```bash
 python3 -m pip install purpleair_data_logger
 ```
 
 You can install PurpleAir Data Logger by cloning down this repo.
 
 ```bash
-git clone https://github.com/carlkid1499/purpleair_data_logger.git
+git clone https://github.com/carlkidcrypto/purpleair_data_logger.git
 cd purpleair_data_logger
 python3 setup.py install 
 ```
 
 ## Usage PurpleAirPSQLDataLogger.py
 
 ```bash
-usage: PurpleAirPSQLDataLogger.py [-h] [-db_drop_all_tables] -db_usr DB_USR [-db_host DB_HOST] -db DB
-                                  [-db_port DB_PORT] [-db_pwd DB_PWD] -paa_read_key PAA_READ_KEY
+usage: PurpleAirPSQLDataLogger.py [-h] -paa_read_key PAA_READ_KEY -paa_write_key PAA_WRITE_KEY
                                   [-paa_single_sensor_request_json_file PAA_SINGLE_SENSOR_REQUEST_JSON_FILE]
                                   [-paa_multiple_sensor_request_json_file PAA_MULTIPLE_SENSOR_REQUEST_JSON_FILE]
+                                  [-paa_group_sensor_request_json_file PAA_GROUP_SENSOR_REQUEST_JSON_FILE]
+                                  [-db_drop_all_tables] -db_usr DB_USR [-db_host DB_HOST] -db DB [-db_port DB_PORT]
+                                  [-db_pwd DB_PWD]
 
 Collect data from PurpleAir sensors and insert into a database!
 
-optional arguments:
+options:
   -h, --help            show this help message and exit
+  -paa_read_key PAA_READ_KEY
+                        The PurpleAirAPI Read key
+  -paa_write_key PAA_WRITE_KEY
+                        The PurpleAirAPI write key
+  -paa_single_sensor_request_json_file PAA_SINGLE_SENSOR_REQUEST_JSON_FILE
+                        The path to a json file containing the parameters to send a single sensor request.
+  -paa_multiple_sensor_request_json_file PAA_MULTIPLE_SENSOR_REQUEST_JSON_FILE
+                        The path to a json file containing the parameters to send a multiple sensor request.
+  -paa_group_sensor_request_json_file PAA_GROUP_SENSOR_REQUEST_JSON_FILE
+                        The path to a json file containing the parameters to send a group sensor request.
   -db_drop_all_tables   Set this flag if you wish to drop all tables before loading in new data. Useful if a database
                         change has happened. Note: Make sure to provide a db_usr with DROP rights. WARNING: ALL
                         COLLECTED DATA WILL BE LOST!
   -db_usr DB_USR        The PSQL database user
   -db_host DB_HOST      The PSQL database host
   -db DB                The PSQL database name
   -db_port DB_PORT      The PSQL database port number
   -db_pwd DB_PWD        The PSQL database password
-  -paa_read_key PAA_READ_KEY
-                        The PurpleAirAPI Read key
-  -paa_single_sensor_request_json_file PAA_SINGLE_SENSOR_REQUEST_JSON_FILE
-                        The path to a json file containing the parameters to send a single sensor request.
-  -paa_multiple_sensor_request_json_file PAA_MULTIPLE_SENSOR_REQUEST_JSON_FILE
-                        The path to a json file containing the parameters to send a multiple sensor request.
+```
+
+Using it with single sensor requests...
+
+```bash
+python3 -m  purpleair_data_logger.PurpleAirPSQLDataLogger -db_usr USER -db_host localhost -db DB_NAME -db_port 5432 -db_pwd PASSWORD -paa_read_key 12345678-1234-1234-1234-123456789123 -paa_write_key 12345678-1234-1234-1234-123456789123 -paa_single_sensor_request_json_file PATH_TO_YOUR_FILE
+```
+
+Using it with multiple sensor requests...
+
+```bash
+python3 -m  purpleair_data_logger.PurpleAirPSQLDataLogger -db_usr USER -db_host localhost -db DB_NAME -db_port 5432 -db_pwd PASSWORD -paa_read_key 12345678-1234-1234-1234-123456789123 -paa_write_key 12345678-1234-1234-1234-123456789123 -paa_multiple_sensor_request_json_file PATH_TO_YOUR_FILE
 ```
 
 ### High Level Design
 
 ![PAA_Data_Logger_Software_Stack.drawio.png](/diagrams/PAA_Data_Logger_Software_Stack.drawio.png)
 
 ### Getting Started
@@ -79,153 +97,234 @@
 3. Install and configure TimescaleDB. <https://docs.timescale.com/install/latest/self-hosted/>
 4. Install and configure Grafana. <https://grafana.com/docs/grafana/latest/setup-grafana/installation/>
 5. Import into your local Grafana instance the dashboard file found [here](./grafana_dashboards/PurpleAirAPI%20(PAA)%20Data%20Logger%20Grafana%20Dashboard-1660355898051.json)
 
 ## Usage PurpleAirCSVDataLogger.py
 
 ```bash
-usage: PurpleAirCSVDataLogger.py [-h] -save_file_path SAVE_FILE_PATH -paa_read_key PAA_READ_KEY
+usage: PurpleAirCSVDataLogger.py [-h] -paa_read_key PAA_READ_KEY -paa_write_key PAA_WRITE_KEY
                                  [-paa_single_sensor_request_json_file PAA_SINGLE_SENSOR_REQUEST_JSON_FILE]
                                  [-paa_multiple_sensor_request_json_file PAA_MULTIPLE_SENSOR_REQUEST_JSON_FILE]
+                                 [-paa_group_sensor_request_json_file PAA_GROUP_SENSOR_REQUEST_JSON_FILE]
+                                 -save_file_path SAVE_FILE_PATH
 
 Collect data from PurpleAir sensors and store it in CSV files!
 
-optional arguments:
+options:
   -h, --help            show this help message and exit
-  -save_file_path SAVE_FILE_PATH
-                        The path to save CSV files in.
   -paa_read_key PAA_READ_KEY
                         The PurpleAirAPI Read key
+  -paa_write_key PAA_WRITE_KEY
+                        The PurpleAirAPI write key
   -paa_single_sensor_request_json_file PAA_SINGLE_SENSOR_REQUEST_JSON_FILE
                         The path to a json file containing the parameters to send a single sensor request.
   -paa_multiple_sensor_request_json_file PAA_MULTIPLE_SENSOR_REQUEST_JSON_FILE
                         The path to a json file containing the parameters to send a multiple sensor request.
+  -paa_group_sensor_request_json_file PAA_GROUP_SENSOR_REQUEST_JSON_FILE
+                        The path to a json file containing the parameters to send a group sensor request.
+  -save_file_path SAVE_FILE_PATH
+                        The path to save CSV files in.
+```
+
+Using it with single sensor requests...
+
+```bash
+python3 -m  purpleair_data_logger.PurpleAirCSVDataLogger -save_file_path SAVE_FILE_PATH -paa_read_key 12345678-1234-1234-1234-123456789123 -paa_write_key 12345678-1234-1234-1234-123456789123 -paa_single_sensor_request_json_file PATH_TO_YOUR_FILE
+```
+
+Using it with multiple sensor requests...
+
+```bash
+python3 -m  purpleair_data_logger.PurpleAirCSVDataLogger -save_file_path SAVE_FILE_PATH -paa_read_key 12345678-1234-1234-1234-123456789123 -paa_write_key 12345678-1234-1234-1234-123456789123 -paa_multiple_sensor_request_json_file PATH_TO_YOUR_FILE
 ```
 
 ## Usage PurpleAirSQLiteDataLogger.py
 
 ```bash
-usage: PurpleAirSQLiteDataLogger.py [-h] -db_name DB_NAME -paa_read_key PAA_READ_KEY
+usage: PurpleAirSQLiteDataLogger.py [-h] -paa_read_key PAA_READ_KEY -paa_write_key PAA_WRITE_KEY
                                     [-paa_single_sensor_request_json_file PAA_SINGLE_SENSOR_REQUEST_JSON_FILE]
                                     [-paa_multiple_sensor_request_json_file PAA_MULTIPLE_SENSOR_REQUEST_JSON_FILE]
+                                    [-paa_group_sensor_request_json_file PAA_GROUP_SENSOR_REQUEST_JSON_FILE] -db_name
+                                    DB_NAME
 
 Collect data from PurpleAir sensors and store it a SQLite3 database file!
 
-optional arguments:
+options:
   -h, --help            show this help message and exit
-  -db_name DB_NAME      The path and name for the SQLite3 database file! i.e database_name.db
   -paa_read_key PAA_READ_KEY
                         The PurpleAirAPI Read key
+  -paa_write_key PAA_WRITE_KEY
+                        The PurpleAirAPI write key
   -paa_single_sensor_request_json_file PAA_SINGLE_SENSOR_REQUEST_JSON_FILE
                         The path to a json file containing the parameters to send a single sensor request.
   -paa_multiple_sensor_request_json_file PAA_MULTIPLE_SENSOR_REQUEST_JSON_FILE
                         The path to a json file containing the parameters to send a multiple sensor request.
+  -paa_group_sensor_request_json_file PAA_GROUP_SENSOR_REQUEST_JSON_FILE
+                        The path to a json file containing the parameters to send a group sensor request.
+  -db_name DB_NAME      The path and name for the SQLite3 database file! i.e database_name.db
+```
+
+Using it with single sensor requests...
+
+```bash
+python3 -m  purpleair_data_logger.PurpleAirSQLiteDataLogger -db_name DB_NAME -paa_read_key 12345678-1234-1234-1234-123456789123 -paa_write_key 12345678-1234-1234-1234-123456789123 -paa_single_sensor_request_json_file PATH_TO_YOUR_FILE
+```
+
+Using it with multiple sensor requests...
+
+```bash
+python3 -m  purpleair_data_logger.PurpleAirSQLiteDataLogger -db_name DB_NAME -paa_read_key 12345678-1234-1234-1234-123456789123 -paa_write_key 12345678-1234-1234-1234-123456789123 -paa_multiple_sensor_request_json_file PATH_TO_YOUR_FILE
 ```
 
 ## Sample JSON Configuration File(s)
 
 The following sample json configuration files can be used with any of the data loggers.
 
-### PAA_SINGLE_SENSOR_REQUEST_JSON_FILE Example
+### PAA Single Sensor Request Example
 
 Out of the parameters listed below only "sensor_index" is required. The others are all optional according to PurpleAirAPI (PAA) documentation. If a field is not being used, mark it 'null' without the single quotes.
 
 ```json
 {
     "sensor_index": 53,
     "read_key": null,
     "fields": null
 }
 ```
 
+Or see this [file](./sample_json_config_files/sample_single_sensor_request_json_file.json) for another example.
+
 > Note: Refer to the PurpleAirAPI (PAA) documentation for more information. <https://api.purpleair.com/#api-sensors-get-sensor-data>
 
-### PAA_MULTIPLE_SENSOR_REQUEST_JSON_FILE Example
+### PAA Multiple Sensor Request Example
 
 Out of the parameters listed below only "fields" is required. The others are all optional according to PurpleAirAPI (PAA) documentation. If a field is not being used, mark it 'null' without the single quotes.
 
 ```json
 {
-    "fields": "A string comma delimited list of fields to retrieve",
+    "fields": "A string comma delimited string of fields to retrieve. i.e fields,name,etc",
     "location_type": null,
     "read_keys": null,
     "show_only": null,
     "modified_since": null,
     "max_age": null,
     "nwlng" : null,
     "nwlat": null,
     "selng": null,
     "selat": null
 }
 ```
 
+Or see this [file](./sample_json_config_files/sample_multiple_sensor_request_json_file.json) for another example.
+
 > Note: Refer to the PurpleAirAPI (PAA) documentation for more information. <https://api.purpleair.com/#api-sensors-get-sensors-data>
 
-> Taken From the PurpleAirAPI documentation:
+The below snippet is taken From the PurpleAirAPI (PAA) documentation:
+
+```plain text
+  Field Type Description
+  fields String
+  The 'Fields' parameter specifies which 'sensor data fields' to include in the response. It is a comma separated list with one or more of the following:
+
+  Station information and status fields:
+  name, icon, model, hardware, location_type, private, latitude, longitude, altitude, position_rating, led_brightness, firmware_version, firmware_upgrade, rssi, uptime, pa_latency, memory, last_seen, last_modified, date_created, channel_state, channel_flags, channel_flags_manual, channel_flags_auto, confidence, confidence_manual, confidence_auto
 
-    Field Type Description
-    fields String 
-    The 'Fields' parameter specifies which 'sensor data fields' to include in the response. It is a comma separated list with one or more of the following:
+  Environmental fields:
+  humidity, humidity_a, humidity_b, temperature, temperature_a, temperature_b, pressure, pressure_a, pressure_b
 
-    Station information and status fields:
-    name, icon, model, hardware, location_type, private, latitude, longitude, altitude, position_rating, led_brightness, firmware_version, firmware_upgrade, rssi, uptime, pa_latency, memory, last_seen, last_modified, date_created, channel_state, channel_flags, channel_flags_manual, channel_flags_auto, confidence, confidence_manual, confidence_auto
+  Miscellaneous fields:
+  voc, voc_a, voc_b, ozone1, analog_input
 
-    Environmental fields:
-    humidity, humidity_a, humidity_b, temperature, temperature_a, temperature_b, pressure, pressure_a, pressure_b
+  PM1.0 fields:
+  pm1.0, pm1.0_a, pm1.0_b, pm1.0_atm, pm1.0_atm_a, pm1.0_atm_b, pm1.0_cf_1, pm1.0_cf_1_a, pm1.0_cf_1_b
 
-    Miscellaneous fields:
-    voc, voc_a, voc_b, ozone1, analog_input
+  PM2.5 fields:
+  pm2.5_alt, pm2.5_alt_a, pm2.5_alt_b, pm2.5, pm2.5_a, pm2.5_b, pm2.5_atm, pm2.5_atm_a, pm2.5_atm_b, pm2.5_cf_1, pm2.5_cf_1_a, pm2.5_cf_1_b
 
-    PM1.0 fields:
-    pm1.0, pm1.0_a, pm1.0_b, pm1.0_atm, pm1.0_atm_a, pm1.0_atm_b, pm1.0_cf_1, pm1.0_cf_1_a, pm1.0_cf_1_b
+  PM2.5 pseudo (simple running) average fields:
+  pm2.5_10minute, pm2.5_10minute_a, pm2.5_10minute_b, pm2.5_30minute, pm2.5_30minute_a, pm2.5_30minute_b, pm2.5_60minute, pm2.5_60minute_a, pm2.5_60minute_b, pm2.5_6hour, pm2.5_6hour_a, pm2.5_6hour_b, pm2.5_24hour, pm2.5_24hour_a, pm2.5_24hour_b, pm2.5_1week, pm2.5_1week_a, pm2.5_1week_b
 
-    PM2.5 fields:
-    pm2.5_alt, pm2.5_alt_a, pm2.5_alt_b, pm2.5, pm2.5_a, pm2.5_b, pm2.5_atm, pm2.5_atm_a, pm2.5_atm_b, pm2.5_cf_1, pm2.5_cf_1_a, pm2.5_cf_1_b
+  PM10.0 fields:
+  pm10.0, pm10.0_a, pm10.0_b, pm10.0_atm, pm10.0_atm_a, pm10.0_atm_b, pm10.0_cf_1, pm10.0_cf_1_a, pm10.0_cf_1_b
 
-    PM2.5 pseudo (simple running) average fields:
-    pm2.5_10minute, pm2.5_10minute_a, pm2.5_10minute_b, pm2.5_30minute, pm2.5_30minute_a, pm2.5_30minute_b, pm2.5_60minute, pm2.5_60minute_a, pm2.5_60minute_b, pm2.5_6hour, pm2.5_6hour_a, pm2.5_6hour_b, pm2.5_24hour, pm2.5_24hour_a, pm2.5_24hour_b, pm2.5_1week, pm2.5_1week_a, pm2.5_1week_b
+  Visibility fields:
+  scattering_coefficient, scattering_coefficient_a, scattering_coefficient_b, deciviews, deciviews_a, deciviews_b, visual_range, visual_range_a, visual_range_b
 
-    PM10.0 fields:
-    pm10.0, pm10.0_a, pm10.0_b, pm10.0_atm, pm10.0_atm_a, pm10.0_atm_b, pm10.0_cf_1, pm10.0_cf_1_a, pm10.0_cf_1_b
+  Particle count fields:
+  0.3_um_count, 0.3_um_count_a, 0.3_um_count_b, 0.5_um_count, 0.5_um_count_a, 0.5_um_count_b, 1.0_um_count, 1.0_um_count_a, 1.0_um_count_b, 2.5_um_count, 2.5_um_count_a, 2.5_um_count_b, 5.0_um_count, 5.0_um_count_a, 5.0_um_count_b, 10.0_um_count 10.0_um_count_a, 10.0_um_count_b
 
-    Visibility fields:
-    scattering_coefficient, scattering_coefficient_a, scattering_coefficient_b, deciviews, deciviews_a, deciviews_b, visual_range, visual_range_a, visual_range_b
+  ThingSpeak fields, used to retrieve data from api.thingspeak.com:
+  primary_id_a, primary_key_a, secondary_id_a, secondary_key_a, primary_id_b, primary_key_b, secondary_id_b, secondary_key_b
 
-    Particle count fields:
-    0.3_um_count, 0.3_um_count_a, 0.3_um_count_b, 0.5_um_count, 0.5_um_count_a, 0.5_um_count_b, 1.0_um_count, 1.0_um_count_a, 1.0_um_count_b, 2.5_um_count, 2.5_um_count_a, 2.5_um_count_b, 5.0_um_count, 5.0_um_count_a, 5.0_um_count_b, 10.0_um_count 10.0_um_count_a, 10.0_um_count_b
+  For field descriptions, please see the 'sensor data fields'. section.
 
-    ThingSpeak fields, used to retrieve data from api.thingspeak.com:
-    primary_id_a, primary_key_a, secondary_id_a, secondary_key_a, primary_id_b, primary_key_b, secondary_id_b, secondary_key_b
+  location_type optional Number
+  The location_type of the sensors.
+  Possible values are: 0 = Outside or 1 = Inside.
 
-    For field descriptions, please see the 'sensor data fields'. section.
+  read_keys optional String
+  A read_key is required for private devices. It is separate to the api_key and each sensor has its own read_key. Submit multiple keys by separating them with a comma (,) character for example: key-one,key-two,key-three.
 
-    location_type optional Number 
-    The location_type of the sensors.
-    Possible values are: 0 = Outside or 1 = Inside.
+  show_only optional String
+  A comma (,) separated list of sensor_index values. When provided, the results are limited only to the sensors included in this list.
 
-    read_keys optional String 
-    A read_key is required for private devices. It is separate to the api_key and each sensor has its own read_key. Submit multiple keys by separating them with a comma (,) character for example: key-one,key-two,key-three.
+  modified_since optional long
+  The modified_since parameter causes only sensors modified after the provided time stamp to be included in the results. Using the time_stamp value from a previous call (recommended) will limit results to those with new values since the last request. Using a value of 0 will match sensors modified at any time.
 
-    show_only optional String 
-    A comma (,) separated list of sensor_index values. When provided, the results are limited only to the sensors included in this list.
+  max_age optional Integer
+  Filter results to only include sensors modified or updated within the last number of seconds. Using a value of 0 will match sensors of any age.
 
-    modified_since optional long 
-    The modified_since parameter causes only sensors modified after the provided time stamp to be included in the results. Using the time_stamp value from a previous call (recommended) will limit results to those with new values since the last request. Using a value of 0 will match sensors modified at any time.
+  Default value: 604800
 
-    max_age optional Integer 
-    Filter results to only include sensors modified or updated within the last number of seconds. Using a value of 0 will match sensors of any age.
+  nwlng optional Number
+  A north west longitude for the bounding box.
 
-    Default value: 604800
+  Use a bounding box to limit the sensors returned to a specific geographic area. The bounding box is defined by two points, a north west latitude/longitude and a south east latitude/longitude.
+
+  nwlat optional Number
+  A north west latitude for the bounding box.
+
+  selng optional Number
+  A south east longitude for the bounding box.
+
+  selat optional Number
+  A south east latitude for the bounding box.
+```
 
-    nwlng optional Number 
-    A north west longitude for the bounding box.
+### PAA Group Sensor Request Example
 
-    Use a bounding box to limit the sensors returned to a specific geographic area. The bounding box is defined by two points, a north west latitude/longitude and a south east latitude/longitude.
+Out of the parameters below `sensor_group_name`, `add_sensors_to_group`, and `sensor_index_list` are custom settings not
+defined in the official PAA documentation. These three setting help drive the `group` request feature.
 
-    nwlat optional Number 
-    A north west latitude for the bounding box.
+`sensor_group_name` - This will be the name assigned to your group. If it doesn't exist already, it will be created.
+Otherwise, the first group matching the name will be used.
 
-    selng optional Number 
-    A south east longitude for the bounding box.
+`add_sensors_to_group` - If true, adds the sensors in the `sensor_index_list`. If false, `sensor_index_list` is ignored.
+
+`sensor_index_list` -  A list of sensor indexes that will be added to your group if they don't already exist.
+
+The rest of the settings are official PAA settings. They are the same as the [### PAA Multiple Sensor Request Example](#paa-multiple-sensor-request-example). Refer above for details.
+
+```json
+{
+    "sensor_group_name": "A Name Goes Here",
+    "add_sensors_to_group": true,
+    "sensor_index_list": [
+        77,
+        81,
+        95079,
+        167897
+    ],
+    "fields": "A string comma delimited string of fields to retrieve. i.e fields,name,etc",
+    "location_type": null,
+    "read_keys": null,
+    "show_only": null,
+    "modified_since": null,
+    "max_age": null,
+    "nwlng" : null,
+    "nwlat": null,
+    "selng": null,
+    "selat": null
+}
+```
 
-    selat optional Number 
-    A south east latitude for the bounding box.
+Or see this [file](./sample_json_config_files/sample_group_sensor_request_json_file.json) for another example.
```

#### html2text {}

```diff
@@ -1,130 +1,176 @@
-Metadata-Version: 2.1 Name: purpleair-data-logger Version: 1.2.0a2 Home-page:
-https://github.com/carlkid1499/purpleair_data_logger Author: Carlos Santos
-Author-email: 27721404+carlkid1499@users.noreply.github.com License: MIT
-Keywords: purpleair_data_logger,purple air,purple air data
+Metadata-Version: 2.1 Name: purpleair-data-logger Version: 1.2.1a1 Home-page:
+https://github.com/carlkidcrypto/purpleair_data_logger Author: Carlos Santos
+Author-email: dose.lucky.sake@cloak.id License: MIT Keywords:
+purpleair_data_logger,purple air,purple air data
 logger,PurpleAirPSQLDataLogger,PurpleAirCSVDataLogger,purple air
 api,PurpleAirSQLiteDataLogger Platform: Windows 32/64 Platform: Linux 32/64
 Platform: MacOS 32/64 Requires-Python: >=3.8 Description-Content-Type: text/
-markdown License-File: LICENSE # purple_air_data_logger A set of data logger(s)
-that will query purple air sensor(s) for data. That data will then be ingested
-into a TimeScaleDB PostGreSQL database, CSV files, or a SQLite3 database. To
-use these tools a PurpleAPI key is required. You can get API keys by sending an
-email to `contact@purpleair.com` with a first and last name to assign them to.
-| [![Behave Tests](https://github.com/carlkid1499/purpleair_data_logger/
-actions/workflows/behave_tests.yml/badge.svg?branch=main)](https://github.com/
-carlkid1499/purpleair_data_logger/actions/workflows/behave_tests.yml) | [![PyPI
-Distributions](https://github.com/carlkid1499/purpleair_data_logger/actions/
-workflows/build_and_publish_to_pypi.yml/badge.svg?branch=main)](https://
-github.com/carlkid1499/purpleair_data_logger/actions/workflows/
+markdown License-File: LICENSE # Purple Air Data Logger(s) (PADLs) A set of
+data logger(s) that will query purple air sensor(s) for data. That data will
+then be ingested into a TimeScaleDB PostGreSQL database, CSV files, or a
+SQLite3 database. To use these tools a PurpleAPI key is required. You can get
+API keys by sending an email to `contact@purpleair.com` with a first and last
+name to assign them to. | [![Behave Tests](https://github.com/carlkidcrypto/
+purpleair_data_logger/actions/workflows/behave_tests.yml/
+badge.svg?branch=main)](https://github.com/carlkidcrypto/purpleair_data_logger/
+actions/workflows/behave_tests.yml) | [![PyPI Distributions](https://
+github.com/carlkidcrypto/purpleair_data_logger/actions/workflows/
+build_and_publish_to_pypi.yml/badge.svg?branch=main)](https://github.com/
+carlkidcrypto/purpleair_data_logger/actions/workflows/
 build_and_publish_to_pypi.yml) | [![TestPyPI Distributions](https://github.com/
-carlkid1499/purpleair_data_logger/actions/workflows/
+carlkidcrypto/purpleair_data_logger/actions/workflows/
 build_and_publish_to_test_pypi.yml/badge.svg?branch=main)](https://github.com/
-carlkid1499/purpleair_data_logger/actions/workflows/
-build_and_publish_to_test_pypi.yml) | | --------------- | --------------- | ---
------------- | ## How to Support This Project [Buy_Me_A_Coffee] ## Installation
-You can install the PurpleAir Data Logger via pip. ```bash python3 -m pip
-install purpleair_data_logger ``` You can install PurpleAir Data Logger by
-cloning down this repo. ```bash git clone https://github.com/carlkid1499/
+carlkidcrypto/purpleair_data_logger/actions/workflows/
+build_and_publish_to_test_pypi.yml) | [![Black](https://github.com/
+carlkidcrypto/purpleair_data_logger/actions/workflows/black.yml/badge.svg)]
+(https://github.com/carlkidcrypto/purpleair_data_logger/actions/workflows/
+black.yml) | | --------------- | --------------- | --------------- | ----------
+----- | ## How to Support This Project [Buy_Me_A_Coffee] ## Installation You
+can install the PurpleAir Data Logger via pip. ```bash python3 -m pip install
+purpleair_data_logger ``` You can install PurpleAir Data Logger by cloning down
+this repo. ```bash git clone https://github.com/carlkidcrypto/
 purpleair_data_logger.git cd purpleair_data_logger python3 setup.py install ```
 ## Usage PurpleAirPSQLDataLogger.py ```bash usage: PurpleAirPSQLDataLogger.py
-[-h] [-db_drop_all_tables] -db_usr DB_USR [-db_host DB_HOST] -db DB [-db_port
-DB_PORT] [-db_pwd DB_PWD] -paa_read_key PAA_READ_KEY [-
+[-h] -paa_read_key PAA_READ_KEY -paa_write_key PAA_WRITE_KEY [-
 paa_single_sensor_request_json_file PAA_SINGLE_SENSOR_REQUEST_JSON_FILE] [-
-paa_multiple_sensor_request_json_file PAA_MULTIPLE_SENSOR_REQUEST_JSON_FILE]
-Collect data from PurpleAir sensors and insert into a database! optional
-arguments: -h, --help show this help message and exit -db_drop_all_tables Set
-this flag if you wish to drop all tables before loading in new data. Useful if
-a database change has happened. Note: Make sure to provide a db_usr with DROP
-rights. WARNING: ALL COLLECTED DATA WILL BE LOST! -db_usr DB_USR The PSQL
-database user -db_host DB_HOST The PSQL database host -db DB The PSQL database
-name -db_port DB_PORT The PSQL database port number -db_pwd DB_PWD The PSQL
-database password -paa_read_key PAA_READ_KEY The PurpleAirAPI Read key -
-paa_single_sensor_request_json_file PAA_SINGLE_SENSOR_REQUEST_JSON_FILE The
-path to a json file containing the parameters to send a single sensor request.
--paa_multiple_sensor_request_json_file PAA_MULTIPLE_SENSOR_REQUEST_JSON_FILE
-The path to a json file containing the parameters to send a multiple sensor
-request. ``` ### High Level Design ![PAA_Data_Logger_Software_Stack.drawio.png]
-(/diagrams/PAA_Data_Logger_Software_Stack.drawio.png) ### Getting Started 1.
-Grab and install Postgresql for your platform.
+paa_multiple_sensor_request_json_file PAA_MULTIPLE_SENSOR_REQUEST_JSON_FILE] [-
+paa_group_sensor_request_json_file PAA_GROUP_SENSOR_REQUEST_JSON_FILE] [-
+db_drop_all_tables] -db_usr DB_USR [-db_host DB_HOST] -db DB [-db_port DB_PORT]
+[-db_pwd DB_PWD] Collect data from PurpleAir sensors and insert into a
+database! options: -h, --help show this help message and exit -paa_read_key
+PAA_READ_KEY The PurpleAirAPI Read key -paa_write_key PAA_WRITE_KEY The
+PurpleAirAPI write key -paa_single_sensor_request_json_file
+PAA_SINGLE_SENSOR_REQUEST_JSON_FILE The path to a json file containing the
+parameters to send a single sensor request. -
+paa_multiple_sensor_request_json_file PAA_MULTIPLE_SENSOR_REQUEST_JSON_FILE The
+path to a json file containing the parameters to send a multiple sensor
+request. -paa_group_sensor_request_json_file PAA_GROUP_SENSOR_REQUEST_JSON_FILE
+The path to a json file containing the parameters to send a group sensor
+request. -db_drop_all_tables Set this flag if you wish to drop all tables
+before loading in new data. Useful if a database change has happened. Note:
+Make sure to provide a db_usr with DROP rights. WARNING: ALL COLLECTED DATA
+WILL BE LOST! -db_usr DB_USR The PSQL database user -db_host DB_HOST The PSQL
+database host -db DB The PSQL database name -db_port DB_PORT The PSQL database
+port number -db_pwd DB_PWD The PSQL database password ``` Using it with single
+sensor requests... ```bash python3 -
+m purpleair_data_logger.PurpleAirPSQLDataLogger -db_usr USER -db_host localhost
+-db DB_NAME -db_port 5432 -db_pwd PASSWORD -paa_read_key 12345678-1234-1234-
+1234-123456789123 -paa_write_key 12345678-1234-1234-1234-123456789123 -
+paa_single_sensor_request_json_file PATH_TO_YOUR_FILE ``` Using it with
+multiple sensor requests... ```bash python3 -
+m purpleair_data_logger.PurpleAirPSQLDataLogger -db_usr USER -db_host localhost
+-db DB_NAME -db_port 5432 -db_pwd PASSWORD -paa_read_key 12345678-1234-1234-
+1234-123456789123 -paa_write_key 12345678-1234-1234-1234-123456789123 -
+paa_multiple_sensor_request_json_file PATH_TO_YOUR_FILE ``` ### High Level
+Design ![PAA_Data_Logger_Software_Stack.drawio.png](/diagrams/
+PAA_Data_Logger_Software_Stack.drawio.png) ### Getting Started 1. Grab and
+install Postgresql for your platform.
 www.postgresql.org/download/> 2. Create two database users. One for Grafana
 with select only privileges. The other for the data logger with only insert/
 create privileges.
 medium.com/coding-blocks/creating-user-database-and-adding-access-on-
 postgresql-8bfcd2f4a91e>,
 www.techonthenet.com/postgresql/grant_revoke.php> 3. Install and configure
 TimescaleDB.
 docs.timescale.com/install/latest/self-hosted/> 4. Install and configure
 Grafana.
 grafana.com/docs/grafana/latest/setup-grafana/installation/> 5. Import into
 your local Grafana instance the dashboard file found [here](./
 grafana_dashboards/PurpleAirAPI%20(PAA)%20Data%20Logger%20Grafana%20Dashboard-
 1660355898051.json) ## Usage PurpleAirCSVDataLogger.py ```bash usage:
-PurpleAirCSVDataLogger.py [-h] -save_file_path SAVE_FILE_PATH -paa_read_key
-PAA_READ_KEY [-paa_single_sensor_request_json_file
+PurpleAirCSVDataLogger.py [-h] -paa_read_key PAA_READ_KEY -paa_write_key
+PAA_WRITE_KEY [-paa_single_sensor_request_json_file
 PAA_SINGLE_SENSOR_REQUEST_JSON_FILE] [-paa_multiple_sensor_request_json_file
-PAA_MULTIPLE_SENSOR_REQUEST_JSON_FILE] Collect data from PurpleAir sensors and
-store it in CSV files! optional arguments: -h, --help show this help message
-and exit -save_file_path SAVE_FILE_PATH The path to save CSV files in. -
-paa_read_key PAA_READ_KEY The PurpleAirAPI Read key -
+PAA_MULTIPLE_SENSOR_REQUEST_JSON_FILE] [-paa_group_sensor_request_json_file
+PAA_GROUP_SENSOR_REQUEST_JSON_FILE] -save_file_path SAVE_FILE_PATH Collect data
+from PurpleAir sensors and store it in CSV files! options: -h, --help show this
+help message and exit -paa_read_key PAA_READ_KEY The PurpleAirAPI Read key -
+paa_write_key PAA_WRITE_KEY The PurpleAirAPI write key -
 paa_single_sensor_request_json_file PAA_SINGLE_SENSOR_REQUEST_JSON_FILE The
 path to a json file containing the parameters to send a single sensor request.
 -paa_multiple_sensor_request_json_file PAA_MULTIPLE_SENSOR_REQUEST_JSON_FILE
 The path to a json file containing the parameters to send a multiple sensor
-request. ``` ## Usage PurpleAirSQLiteDataLogger.py ```bash usage:
-PurpleAirSQLiteDataLogger.py [-h] -db_name DB_NAME -paa_read_key PAA_READ_KEY
-[-paa_single_sensor_request_json_file PAA_SINGLE_SENSOR_REQUEST_JSON_FILE] [-
-paa_multiple_sensor_request_json_file PAA_MULTIPLE_SENSOR_REQUEST_JSON_FILE]
-Collect data from PurpleAir sensors and store it a SQLite3 database file!
-optional arguments: -h, --help show this help message and exit -db_name DB_NAME
-The path and name for the SQLite3 database file! i.e database_name.db -
-paa_read_key PAA_READ_KEY The PurpleAirAPI Read key -
+request. -paa_group_sensor_request_json_file PAA_GROUP_SENSOR_REQUEST_JSON_FILE
+The path to a json file containing the parameters to send a group sensor
+request. -save_file_path SAVE_FILE_PATH The path to save CSV files in. ```
+Using it with single sensor requests... ```bash python3 -
+m purpleair_data_logger.PurpleAirCSVDataLogger -save_file_path SAVE_FILE_PATH -
+paa_read_key 12345678-1234-1234-1234-123456789123 -paa_write_key 12345678-1234-
+1234-1234-123456789123 -paa_single_sensor_request_json_file PATH_TO_YOUR_FILE
+``` Using it with multiple sensor requests... ```bash python3 -
+m purpleair_data_logger.PurpleAirCSVDataLogger -save_file_path SAVE_FILE_PATH -
+paa_read_key 12345678-1234-1234-1234-123456789123 -paa_write_key 12345678-1234-
+1234-1234-123456789123 -paa_multiple_sensor_request_json_file PATH_TO_YOUR_FILE
+``` ## Usage PurpleAirSQLiteDataLogger.py ```bash usage:
+PurpleAirSQLiteDataLogger.py [-h] -paa_read_key PAA_READ_KEY -paa_write_key
+PAA_WRITE_KEY [-paa_single_sensor_request_json_file
+PAA_SINGLE_SENSOR_REQUEST_JSON_FILE] [-paa_multiple_sensor_request_json_file
+PAA_MULTIPLE_SENSOR_REQUEST_JSON_FILE] [-paa_group_sensor_request_json_file
+PAA_GROUP_SENSOR_REQUEST_JSON_FILE] -db_name DB_NAME Collect data from
+PurpleAir sensors and store it a SQLite3 database file! options: -h, --help
+show this help message and exit -paa_read_key PAA_READ_KEY The PurpleAirAPI
+Read key -paa_write_key PAA_WRITE_KEY The PurpleAirAPI write key -
 paa_single_sensor_request_json_file PAA_SINGLE_SENSOR_REQUEST_JSON_FILE The
 path to a json file containing the parameters to send a single sensor request.
 -paa_multiple_sensor_request_json_file PAA_MULTIPLE_SENSOR_REQUEST_JSON_FILE
 The path to a json file containing the parameters to send a multiple sensor
-request. ``` ## Sample JSON Configuration File(s) The following sample json
-configuration files can be used with any of the data loggers. ###
-PAA_SINGLE_SENSOR_REQUEST_JSON_FILE Example Out of the parameters listed below
-only "sensor_index" is required. The others are all optional according to
-PurpleAirAPI (PAA) documentation. If a field is not being used, mark it 'null'
-without the single quotes. ```json { "sensor_index": 53, "read_key": null,
-"fields": null } ``` > Note: Refer to the PurpleAirAPI (PAA) documentation for
-more information.
-api.purpleair.com/#api-sensors-get-sensor-data> ###
-PAA_MULTIPLE_SENSOR_REQUEST_JSON_FILE Example Out of the parameters listed
-below only "fields" is required. The others are all optional according to
-PurpleAirAPI (PAA) documentation. If a field is not being used, mark it 'null'
-without the single quotes. ```json { "fields": "A string comma delimited list
-of fields to retrieve", "location_type": null, "read_keys": null, "show_only":
-null, "modified_since": null, "max_age": null, "nwlng" : null, "nwlat": null,
-"selng": null, "selat": null } ``` > Note: Refer to the PurpleAirAPI (PAA)
-documentation for more information.
-api.purpleair.com/#api-sensors-get-sensors-data> > Taken From the PurpleAirAPI
-documentation: Field Type Description fields String The 'Fields' parameter
-specifies which 'sensor data fields' to include in the response. It is a comma
-separated list with one or more of the following: Station information and
-status fields: name, icon, model, hardware, location_type, private, latitude,
-longitude, altitude, position_rating, led_brightness, firmware_version,
-firmware_upgrade, rssi, uptime, pa_latency, memory, last_seen, last_modified,
-date_created, channel_state, channel_flags, channel_flags_manual,
-channel_flags_auto, confidence, confidence_manual, confidence_auto
-Environmental fields: humidity, humidity_a, humidity_b, temperature,
-temperature_a, temperature_b, pressure, pressure_a, pressure_b Miscellaneous
-fields: voc, voc_a, voc_b, ozone1, analog_input PM1.0 fields: pm1.0, pm1.0_a,
-pm1.0_b, pm1.0_atm, pm1.0_atm_a, pm1.0_atm_b, pm1.0_cf_1, pm1.0_cf_1_a,
-pm1.0_cf_1_b PM2.5 fields: pm2.5_alt, pm2.5_alt_a, pm2.5_alt_b, pm2.5, pm2.5_a,
-pm2.5_b, pm2.5_atm, pm2.5_atm_a, pm2.5_atm_b, pm2.5_cf_1, pm2.5_cf_1_a,
-pm2.5_cf_1_b PM2.5 pseudo (simple running) average fields: pm2.5_10minute,
-pm2.5_10minute_a, pm2.5_10minute_b, pm2.5_30minute, pm2.5_30minute_a,
-pm2.5_30minute_b, pm2.5_60minute, pm2.5_60minute_a, pm2.5_60minute_b,
-pm2.5_6hour, pm2.5_6hour_a, pm2.5_6hour_b, pm2.5_24hour, pm2.5_24hour_a,
-pm2.5_24hour_b, pm2.5_1week, pm2.5_1week_a, pm2.5_1week_b PM10.0 fields:
-pm10.0, pm10.0_a, pm10.0_b, pm10.0_atm, pm10.0_atm_a, pm10.0_atm_b,
-pm10.0_cf_1, pm10.0_cf_1_a, pm10.0_cf_1_b Visibility fields:
+request. -paa_group_sensor_request_json_file PAA_GROUP_SENSOR_REQUEST_JSON_FILE
+The path to a json file containing the parameters to send a group sensor
+request. -db_name DB_NAME The path and name for the SQLite3 database file! i.e
+database_name.db ``` Using it with single sensor requests... ```bash python3 -
+m purpleair_data_logger.PurpleAirSQLiteDataLogger -db_name DB_NAME -
+paa_read_key 12345678-1234-1234-1234-123456789123 -paa_write_key 12345678-1234-
+1234-1234-123456789123 -paa_single_sensor_request_json_file PATH_TO_YOUR_FILE
+``` Using it with multiple sensor requests... ```bash python3 -
+m purpleair_data_logger.PurpleAirSQLiteDataLogger -db_name DB_NAME -
+paa_read_key 12345678-1234-1234-1234-123456789123 -paa_write_key 12345678-1234-
+1234-1234-123456789123 -paa_multiple_sensor_request_json_file PATH_TO_YOUR_FILE
+``` ## Sample JSON Configuration File(s) The following sample json
+configuration files can be used with any of the data loggers. ### PAA Single
+Sensor Request Example Out of the parameters listed below only "sensor_index"
+is required. The others are all optional according to PurpleAirAPI (PAA)
+documentation. If a field is not being used, mark it 'null' without the single
+quotes. ```json { "sensor_index": 53, "read_key": null, "fields": null } ``` Or
+see this [file](./sample_json_config_files/
+sample_single_sensor_request_json_file.json) for another example. > Note: Refer
+to the PurpleAirAPI (PAA) documentation for more information.
+api.purpleair.com/#api-sensors-get-sensor-data> ### PAA Multiple Sensor Request
+Example Out of the parameters listed below only "fields" is required. The
+others are all optional according to PurpleAirAPI (PAA) documentation. If a
+field is not being used, mark it 'null' without the single quotes. ```json
+{ "fields": "A string comma delimited string of fields to retrieve. i.e
+fields,name,etc", "location_type": null, "read_keys": null, "show_only": null,
+"modified_since": null, "max_age": null, "nwlng" : null, "nwlat": null,
+"selng": null, "selat": null } ``` Or see this [file](./
+sample_json_config_files/sample_multiple_sensor_request_json_file.json) for
+another example. > Note: Refer to the PurpleAirAPI (PAA) documentation for more
+information.
+api.purpleair.com/#api-sensors-get-sensors-data> The below snippet is taken
+From the PurpleAirAPI (PAA) documentation: ```plain text Field Type Description
+fields String The 'Fields' parameter specifies which 'sensor data fields' to
+include in the response. It is a comma separated list with one or more of the
+following: Station information and status fields: name, icon, model, hardware,
+location_type, private, latitude, longitude, altitude, position_rating,
+led_brightness, firmware_version, firmware_upgrade, rssi, uptime, pa_latency,
+memory, last_seen, last_modified, date_created, channel_state, channel_flags,
+channel_flags_manual, channel_flags_auto, confidence, confidence_manual,
+confidence_auto Environmental fields: humidity, humidity_a, humidity_b,
+temperature, temperature_a, temperature_b, pressure, pressure_a, pressure_b
+Miscellaneous fields: voc, voc_a, voc_b, ozone1, analog_input PM1.0 fields:
+pm1.0, pm1.0_a, pm1.0_b, pm1.0_atm, pm1.0_atm_a, pm1.0_atm_b, pm1.0_cf_1,
+pm1.0_cf_1_a, pm1.0_cf_1_b PM2.5 fields: pm2.5_alt, pm2.5_alt_a, pm2.5_alt_b,
+pm2.5, pm2.5_a, pm2.5_b, pm2.5_atm, pm2.5_atm_a, pm2.5_atm_b, pm2.5_cf_1,
+pm2.5_cf_1_a, pm2.5_cf_1_b PM2.5 pseudo (simple running) average fields:
+pm2.5_10minute, pm2.5_10minute_a, pm2.5_10minute_b, pm2.5_30minute,
+pm2.5_30minute_a, pm2.5_30minute_b, pm2.5_60minute, pm2.5_60minute_a,
+pm2.5_60minute_b, pm2.5_6hour, pm2.5_6hour_a, pm2.5_6hour_b, pm2.5_24hour,
+pm2.5_24hour_a, pm2.5_24hour_b, pm2.5_1week, pm2.5_1week_a, pm2.5_1week_b
+PM10.0 fields: pm10.0, pm10.0_a, pm10.0_b, pm10.0_atm, pm10.0_atm_a,
+pm10.0_atm_b, pm10.0_cf_1, pm10.0_cf_1_a, pm10.0_cf_1_b Visibility fields:
 scattering_coefficient, scattering_coefficient_a, scattering_coefficient_b,
 deciviews, deciviews_a, deciviews_b, visual_range, visual_range_a,
 visual_range_b Particle count fields: 0.3_um_count, 0.3_um_count_a,
 0.3_um_count_b, 0.5_um_count, 0.5_um_count_a, 0.5_um_count_b, 1.0_um_count,
 1.0_um_count_a, 1.0_um_count_b, 2.5_um_count, 2.5_um_count_a, 2.5_um_count_b,
 5.0_um_count, 5.0_um_count_a, 5.0_um_count_b, 10.0_um_count 10.0_um_count_a,
 10.0_um_count_b ThingSpeak fields, used to retrieve data from
@@ -146,8 +192,26 @@
 updated within the last number of seconds. Using a value of 0 will match
 sensors of any age. Default value: 604800 nwlng optional Number A north west
 longitude for the bounding box. Use a bounding box to limit the sensors
 returned to a specific geographic area. The bounding box is defined by two
 points, a north west latitude/longitude and a south east latitude/longitude.
 nwlat optional Number A north west latitude for the bounding box. selng
 optional Number A south east longitude for the bounding box. selat optional
-Number A south east latitude for the bounding box.
+Number A south east latitude for the bounding box. ``` ### PAA Group Sensor
+Request Example Out of the parameters below `sensor_group_name`,
+`add_sensors_to_group`, and `sensor_index_list` are custom settings not defined
+in the official PAA documentation. These three setting help drive the `group`
+request feature. `sensor_group_name` - This will be the name assigned to your
+group. If it doesn't exist already, it will be created. Otherwise, the first
+group matching the name will be used. `add_sensors_to_group` - If true, adds
+the sensors in the `sensor_index_list`. If false, `sensor_index_list` is
+ignored. `sensor_index_list` - A list of sensor indexes that will be added to
+your group if they don't already exist. The rest of the settings are official
+PAA settings. They are the same as the [### PAA Multiple Sensor Request
+Example](#paa-multiple-sensor-request-example). Refer above for details.
+```json { "sensor_group_name": "A Name Goes Here", "add_sensors_to_group":
+true, "sensor_index_list": [ 77, 81, 95079, 167897 ], "fields": "A string comma
+delimited string of fields to retrieve. i.e fields,name,etc", "location_type":
+null, "read_keys": null, "show_only": null, "modified_since": null, "max_age":
+null, "nwlng" : null, "nwlat": null, "selng": null, "selat": null } ``` Or see
+this [file](./sample_json_config_files/
+sample_group_sensor_request_json_file.json) for another example.
```

### Comparing `purpleair_data_logger-1.2.0a2/purpleair_data_logger.egg-info/SOURCES.txt` & `purpleair_data_logger-1.2.1a1/purpleair_data_logger.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `purpleair_data_logger-1.2.0a2/setup.py` & `purpleair_data_logger-1.2.1a1/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -8,27 +8,27 @@
         os.path.join(os.path.dirname(__file__), filename), encoding="utf-8"
     ) as file:
         return file.read()
 
 
 setup(
     name="purpleair_data_logger",
-    version="1.2.0a2",
+    version="1.2.1a1",
     license="MIT",
     author="Carlos Santos",
-    author_email="27721404+carlkid1499@users.noreply.github.com",
+    author_email="dose.lucky.sake@cloak.id",
     long_description=read_file("README.md"),
     long_description_content_type="text/markdown",
     packages=["purpleair_data_logger"],
-    url="https://github.com/carlkid1499/purpleair_data_logger",
+    url="https://github.com/carlkidcrypto/purpleair_data_logger",
     keywords=[
         "purpleair_data_logger",
         "purple air",
         "purple air data logger",
         "PurpleAirPSQLDataLogger",
         "PurpleAirCSVDataLogger",
         "purple air api",
         "PurpleAirSQLiteDataLogger",
     ],
-    install_requires=["pg8000", "requests", "purpleair_api==1.0.0a2"],
+    install_requires=["pg8000==1.29.5", "requests", "purpleair_api==1.0.2a1"],
     platforms=["Windows 32/64", "Linux 32/64", "MacOS 32/64"],
 )
```

