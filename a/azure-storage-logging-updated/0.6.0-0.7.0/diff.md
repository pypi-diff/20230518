# Comparing `tmp/azure-storage-logging_updated-0.6.0.tar.gz` & `tmp/azure-storage-logging_updated-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "azure-storage-logging_updated-0.6.0.tar", last modified: Tue Jul  5 10:49:50 2022, max compression
+gzip compressed data, was "azure-storage-logging_updated-0.7.0.tar", last modified: Thu May 18 12:28:23 2023, max compression
```

## Comparing `azure-storage-logging_updated-0.6.0.tar` & `azure-storage-logging_updated-0.7.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 abianrodriguez   (501) staff       (20)        0 2022-07-05 10:49:50.869690 azure-storage-logging_updated-0.6.0/
--rw-r--r--   0 abianrodriguez   (501) staff       (20)    11358 2022-06-28 16:13:38.000000 azure-storage-logging_updated-0.6.0/LICENSE
--rw-r--r--   0 abianrodriguez   (501) staff       (20)      100 2022-06-28 16:13:38.000000 azure-storage-logging_updated-0.6.0/MANIFEST.in
--rw-r--r--   0 abianrodriguez   (501) staff       (20)    12149 2022-07-05 10:49:50.868995 azure-storage-logging_updated-0.6.0/PKG-INFO
--rw-r--r--   0 abianrodriguez   (501) staff       (20)     9530 2022-07-05 10:49:43.000000 azure-storage-logging_updated-0.6.0/README.rst
-drwxr-xr-x   0 abianrodriguez   (501) staff       (20)        0 2022-07-05 10:49:50.866922 azure-storage-logging_updated-0.6.0/azure_storage_logging/
--rw-r--r--   0 abianrodriguez   (501) staff       (20)        0 2022-06-28 16:13:38.000000 azure-storage-logging_updated-0.6.0/azure_storage_logging/__init__.py
--rw-r--r--   0 abianrodriguez   (501) staff       (20)     8048 2022-07-05 10:29:16.000000 azure-storage-logging_updated-0.6.0/azure_storage_logging/handlers.py
-drwxr-xr-x   0 abianrodriguez   (501) staff       (20)        0 2022-07-05 10:49:50.868625 azure-storage-logging_updated-0.6.0/azure_storage_logging_updated.egg-info/
--rw-r--r--   0 abianrodriguez   (501) staff       (20)    12149 2022-07-05 10:49:50.000000 azure-storage-logging_updated-0.6.0/azure_storage_logging_updated.egg-info/PKG-INFO
--rw-r--r--   0 abianrodriguez   (501) staff       (20)      371 2022-07-05 10:49:50.000000 azure-storage-logging_updated-0.6.0/azure_storage_logging_updated.egg-info/SOURCES.txt
--rw-r--r--   0 abianrodriguez   (501) staff       (20)        1 2022-07-05 10:49:50.000000 azure-storage-logging_updated-0.6.0/azure_storage_logging_updated.egg-info/dependency_links.txt
--rw-r--r--   0 abianrodriguez   (501) staff       (20)       26 2022-07-05 10:49:50.000000 azure-storage-logging_updated-0.6.0/azure_storage_logging_updated.egg-info/requires.txt
--rw-r--r--   0 abianrodriguez   (501) staff       (20)       22 2022-07-05 10:49:50.000000 azure-storage-logging_updated-0.6.0/azure_storage_logging_updated.egg-info/top_level.txt
--rw-r--r--   0 abianrodriguez   (501) staff       (20)       38 2022-07-05 10:49:50.869753 azure-storage-logging_updated-0.6.0/setup.cfg
--rw-r--r--   0 abianrodriguez   (501) staff       (20)     1090 2022-07-05 10:46:56.000000 azure-storage-logging_updated-0.6.0/setup.py
+drwxr-xr-x   0 abianrodriguez   (501) staff       (20)        0 2023-05-18 12:28:23.211650 azure-storage-logging_updated-0.7.0/
+-rw-r--r--   0 abianrodriguez   (501) staff       (20)    11358 2022-06-28 16:13:38.000000 azure-storage-logging_updated-0.7.0/LICENSE
+-rw-r--r--   0 abianrodriguez   (501) staff       (20)      100 2022-06-28 16:13:38.000000 azure-storage-logging_updated-0.7.0/MANIFEST.in
+-rw-r--r--   0 abianrodriguez   (501) staff       (20)    10223 2023-05-18 12:28:23.211060 azure-storage-logging_updated-0.7.0/PKG-INFO
+-rw-r--r--   0 abianrodriguez   (501) staff       (20)     9388 2022-07-05 11:27:45.000000 azure-storage-logging_updated-0.7.0/README.rst
+drwxr-xr-x   0 abianrodriguez   (501) staff       (20)        0 2023-05-18 12:28:23.208205 azure-storage-logging_updated-0.7.0/azure_storage_logging/
+-rw-r--r--   0 abianrodriguez   (501) staff       (20)        0 2022-06-28 16:13:38.000000 azure-storage-logging_updated-0.7.0/azure_storage_logging/__init__.py
+-rw-r--r--   0 abianrodriguez   (501) staff       (20)     8048 2022-07-05 11:03:27.000000 azure-storage-logging_updated-0.7.0/azure_storage_logging/handlers.py
+drwxr-xr-x   0 abianrodriguez   (501) staff       (20)        0 2023-05-18 12:28:23.210679 azure-storage-logging_updated-0.7.0/azure_storage_logging_updated.egg-info/
+-rw-r--r--   0 abianrodriguez   (501) staff       (20)    10223 2023-05-18 12:28:23.000000 azure-storage-logging_updated-0.7.0/azure_storage_logging_updated.egg-info/PKG-INFO
+-rw-r--r--   0 abianrodriguez   (501) staff       (20)      371 2023-05-18 12:28:23.000000 azure-storage-logging_updated-0.7.0/azure_storage_logging_updated.egg-info/SOURCES.txt
+-rw-r--r--   0 abianrodriguez   (501) staff       (20)        1 2023-05-18 12:28:23.000000 azure-storage-logging_updated-0.7.0/azure_storage_logging_updated.egg-info/dependency_links.txt
+-rw-r--r--   0 abianrodriguez   (501) staff       (20)       26 2023-05-18 12:28:23.000000 azure-storage-logging_updated-0.7.0/azure_storage_logging_updated.egg-info/requires.txt
+-rw-r--r--   0 abianrodriguez   (501) staff       (20)       22 2023-05-18 12:28:23.000000 azure-storage-logging_updated-0.7.0/azure_storage_logging_updated.egg-info/top_level.txt
+-rw-r--r--   0 abianrodriguez   (501) staff       (20)       38 2023-05-18 12:28:23.211696 azure-storage-logging_updated-0.7.0/setup.cfg
+-rw-r--r--   0 abianrodriguez   (501) staff       (20)     1090 2023-05-18 11:56:34.000000 azure-storage-logging_updated-0.7.0/setup.py
```

### Comparing `azure-storage-logging_updated-0.6.0/LICENSE` & `azure-storage-logging_updated-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `azure-storage-logging_updated-0.6.0/PKG-INFO` & `azure-storage-logging_updated-0.7.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,243 +1,241 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: azure-storage-logging_updated
-Version: 0.6.0
+Version: 0.7.0
 Summary: Logging handlers to send logs to Microsoft Azure Storage
 Home-page: https://github.com/AbianG/azure-storage-logging_updated
 Author: Abian Rodriguez
 Author-email: abiangrodriguez@protonmail.com
 License: Apache License 2.0
-Description: azure-storage-logging_updated
-        =================================
-        
-        .. image:: http://img.shields.io/pypi/v/azure-storage-logging.svg?style=flat
-            :target: https://pypi.python.org/pypi/azure-storage-logging
-        
-        .. image:: http://img.shields.io/pypi/l/azure-storage-logging.svg?style=flat
-            :target: http://www.apache.org/licenses/LICENSE-2.0.html
-        
-        *azure-storage-logging_table* is a fork from *azure-storage-logging* out of the author's necesity to send output from the standard Python logging APIs to Microsoft Azure Storage Tables.
-        Due to the original module by Michiya Takahashi being outdated, it modifies it to restore functionality to the TableStorageHandler for logging. 
-        In the future, more functionalities may be restored. But on this current version only the TableStorageHandler is usable.
-        
-        Dependencies
-        ------------
-        
-        * azure-data-tables 12.4.0
-        
-        Installation
-        ------------
-        
-        Install the package via pip: ::
-        
-            pip install azure-storage-logging_table
-        
-        Usage
-        -----
-        
-        The module **azure_storage_logging.handlers** in the package contains
-        the following logging handler classes. Each of them uses a different
-        type of Microsoft Azure Storage to send its output to. They all are subclasses
-        of the standard Python logging handler classes, so you can make use of them
-        in the standard ways of Python logging configuration.
-        
-        In addition to
-        `the standard formats for logging <http://docs.python.org/2.7/library/logging.html#logrecord-attributes>`_,
-        the special format ``%(hostname)s`` is also available in your message formatter
-        for the handlers. The format is introduced for ease of identifying the source
-        of log messages which come from many computers and go to the same storage.
-        
-        TableStorageHandler
-        ~~~~~~~~~~~~~~~~~~~
-        The **TableStorageHandler** class is a subclass of **logging.Handler** class,
-        and it sends log messages to Azure table storage and store them
-        as entities in the specified table.
-        
-        The handler puts a formatted log message from applications in the *message*
-        property of a table entity along with some system-defined properties
-        (*PartitionKey*, *RowKey*, and *Timestamp*) like this:
-        
-        +--------------+-----------+----------------+-------------+
-        | PartitionKey | RowKey    | Timestamp      | message     |
-        +==============+===========+================+=============+
-        | XXXXX        | XXXXXXXXX | YYYY-MM-DD ... | log message |
-        +--------------+-----------+----------------+-------------+
-        | XXXXX        | XXXXXXXXX | YYYY-MM-DD ... | log message |
-        +--------------+-----------+----------------+-------------+
-        | XXXXX        | XXXXXXXXX | YYYY-MM-DD ... | log message |
-        +--------------+-----------+----------------+-------------+
-        
-        * *class* azure_storage_logging.handlers.TableStorageHandler(*account_name=None, account_key=None, protocol='https', table='logs', batch_size=0, extra_properties=None, partition_key_formatter=None, row_key_formatter=None, is_emulated=False*)
-        
-            Returns a new instance of the **TableStorageHandler** class.
-            The instance is initialized with the name and the key of your
-            Azure Storage account and some optional parameters.
-        
-            The *table* specifies the name of the table that stores log messages.
-            A new table will be created if it doesn't exist. The table name must
-            conform to the naming convention for Azure Storage table, see
-            `the naming convention for tables <http://msdn.microsoft.com/library/azure/dd179338.aspx>`_
-            for more details.
-        
-            The *protocol* specifies the protocol to transfer data between
-            Azure Storage and your application, ``http`` and ``https``
-            are supported.
-        
-            You can specify the *batch_size* in an integer if you want to use
-            batch transaction when creating new log entities. If the *batch_size*
-            is greater than 1, all new log entities will be transferred to the
-            table at a time when the number of new log messages reaches the
-            *batch_size*. Otherwise, a new log entity will be transferred to
-            the table every time a logging is performed. The *batch_size* must be
-            up to 100 (maximum number of entities in a batch transaction for
-            Azure Storage table).
-        
-            The *extra_properties* accepts a sequence of
-            `the formats for logging <http://docs.python.org/2.7/library/logging.html#logrecord-attributes>`_.
-            The handler-specific one ``%(hostname)s`` is also acceptable.
-            The handler assigns an entity property for every format specified in
-            *extra_properties*. Here is an example of using extra properties:
-        
-            ::
-        
-                import logging
-                from azure_storage_logging.handlers import TableStorageHandler
-        
-                # configure the handler and add it to the logger
-                logger = logging.getLogger('example')
-                handler = TableStorageHandler(conn_str='myConnectionString', table='myTableName',
-                                              extra_properties=('%(hostname)s',
-                                                                '%(levelname)s'))
-                logger.addHandler(handler)
-        
-                # output log messages
-                logger.info('info message')
-                logger.warning('warning message')
-                logger.error('error message')
-        
-            And it will create the log entities, that have the extra properties
-            in addition to the regular property *message*, into the table like this:
-        
-            +--------------+-----------+----------------+----------+-----------+---------------+
-            | PartitionKey | RowKey    | Timestamp      | hostname | levelname | message       |
-            +==============+===========+================+==========+===========+===============+
-            | XXXXX        | XXXXXXXXX | YYYY-MM-DD ... | myhost   | INFO      | info message  |
-            +--------------+-----------+----------------+----------+-----------+---------------+
-            | XXXXX        | XXXXXXXXX | YYYY-MM-DD ... | myhost   | WARNING   | warn message  |
-            +--------------+-----------+----------------+----------+-----------+---------------+
-            | XXXXX        | XXXXXXXXX | YYYY-MM-DD ... | myhost   | ERROR     | error message |
-            +--------------+-----------+----------------+----------+-----------+---------------+
-        
-            You can specify an instance of your custom **logging.Formatters**
-            for the *partition_key_formatter* or the *row_key_formatter*
-            if you want to implement your own keys for the table.
-            The default formatters will be used for partition keys and row keys
-            if no custom formatter for them is given to the handler.
-            The default values for partition keys are provided by the format
-            ``%(asctime)s`` and the date format ``%Y%m%d%H%M`` (provides a unique
-            value per minute). The default values for row keys are provided by the
-            format ``%(asctime)s%(msecs)03d-%(hostname)s-%(process)d-%(rowno)02d``
-            and the date format ``%Y%m%d%H%M%S``.
-        
-            Note that the format ``%(rowno)d`` is a handler-specific one only
-            available for row keys. It would be formatted to a sequential and
-            unique number in a batch that starts from 0. The format is introduced
-            to avoid collision of row keys generated in a batch, and it would
-            always be formatted to 0 if you don't use batch transaction for logging
-            to the table.
-        
-        * setPartitionKeyFormatter(*fmt*)
-        
-            Sets the handler's formatter for partition keys to *fmt*.
-        
-        * setRowKeyFormatter(*fmt*)
-        
-            Sets the handler's formatter for row keys to *fmt*.
-        
-        Example
-        -------
-        
-        Here is an example of the configurations and the logging that uses
-        three different types of storage from the logger:
-        
-        ::
-        
-            LOGGING = {
-                'version': 1,
-                'formatters': {
-                    'simple': {
-                        'format': '%(asctime)s %(message)s',
-                    },
-                    'verbose': {
-                        'format': '%(asctime)s %(levelname)s %(hostname)s %(process)d %(message)s',
-                    },
-                    # this is the same as the default, so you can skip configuring it
-                    'partition_key': {
-                        'format': '%(asctime)s',
-                        'datefmt': '%Y%m%d%H%M',
-                    },
-                    # this is the same as the default, so you can skip configuring it
-                    'row_key': {
-                        'format': '%(asctime)s%(msecs)03d-%(hostname)s-%(process)d-%(rowno)02d',
-                        'datefmt': '%Y%m%d%H%M%S',
-                    },
-                },
-                'handlers': {
-                    'table': {
-                        'conn_str': DefaultEndpointsProtocol=https;AccountName=test;AccountKey=akey==;EndpointSuffix=core.windows.net'
-                        'protocol': 'https',
-                        'table': 'logs',
-                        'level': 'INFO',
-                        'class': 'azure_storage_logging.handlers.TableStorageHandler',
-                        'formatter': 'simple',
-                        'extra_properties': ['%(hostname)s', '%(levelname)s'],
-                        'partition_key_formatter': 'cfg://formatters.partition_key',
-                        'row_key_formatter': 'cfg://formatters.row_key',
-                    },
-                },
-                'loggers': {
-                    'example': {
-                        'handlers': ['table'],
-                        'level': 'DEBUG',
-                    },
-                }
-            }
-        
-            import logging
-            from logging.config import dictConfig
-        
-            dictConfig(LOGGING)
-            logger = logging.getLogger('example')
-            logger.debug('debug message')
-            logger.info('info message')
-            logger.warning('warning message')
-            logger.error('error message')
-            logger.critical('critical message')
-        
-        Notice
-        ------
-        
-        * Set *is_emulated* to ``True`` at initialization of the logging handlers
-          if you want to use this package with Azure storage emulator.
-        
-        License
-        -------
-        
-        Apache License 2.0
-        
-        Credits
-        -------
-        
-        -  `Abian Rodriguez <http://github.com/AbianG>`__
-        -  `Michiya Takahashi <http://github.com/michiya/>`__
 Keywords: azure logging
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Topic :: System :: Logging
+License-File: LICENSE
+
+azure-storage-logging_updated
+=================================
+
+.. image:: http://img.shields.io/pypi/l/azure-storage-logging.svg?style=flat
+    :target: http://www.apache.org/licenses/LICENSE-2.0.html
+
+*azure-storage-logging_table* is a fork from *azure-storage-logging* out of the author's necesity to send output from the standard Python logging APIs to Microsoft Azure Storage Tables.
+Due to the original module by Michiya Takahashi being outdated, it modifies it to restore functionality to the TableStorageHandler for logging. 
+In the future, more functionalities may be restored. But on this current version only the TableStorageHandler is usable.
+
+Dependencies
+------------
+
+* azure-data-tables 12.4.0
+
+Installation
+------------
+
+Install the package via pip: ::
+
+    pip install azure-storage-logging_table
+
+Usage
+-----
+
+The module **azure_storage_logging.handlers** in the package contains
+the following logging handler classes. Each of them uses a different
+type of Microsoft Azure Storage to send its output to. They all are subclasses
+of the standard Python logging handler classes, so you can make use of them
+in the standard ways of Python logging configuration.
+
+In addition to
+`the standard formats for logging <http://docs.python.org/2.7/library/logging.html#logrecord-attributes>`_,
+the special format ``%(hostname)s`` is also available in your message formatter
+for the handlers. The format is introduced for ease of identifying the source
+of log messages which come from many computers and go to the same storage.
+
+TableStorageHandler
+~~~~~~~~~~~~~~~~~~~
+The **TableStorageHandler** class is a subclass of **logging.Handler** class,
+and it sends log messages to Azure table storage and store them
+as entities in the specified table.
+
+The handler puts a formatted log message from applications in the *message*
+property of a table entity along with some system-defined properties
+(*PartitionKey*, *RowKey*, and *Timestamp*) like this:
+
++--------------+-----------+----------------+-------------+
+| PartitionKey | RowKey    | Timestamp      | message     |
++==============+===========+================+=============+
+| XXXXX        | XXXXXXXXX | YYYY-MM-DD ... | log message |
++--------------+-----------+----------------+-------------+
+| XXXXX        | XXXXXXXXX | YYYY-MM-DD ... | log message |
++--------------+-----------+----------------+-------------+
+| XXXXX        | XXXXXXXXX | YYYY-MM-DD ... | log message |
++--------------+-----------+----------------+-------------+
+
+* *class* azure_storage_logging.handlers.TableStorageHandler(*account_name=None, account_key=None, protocol='https', table='logs', batch_size=0, extra_properties=None, partition_key_formatter=None, row_key_formatter=None, is_emulated=False*)
+
+    Returns a new instance of the **TableStorageHandler** class.
+    The instance is initialized with the name and the key of your
+    Azure Storage account and some optional parameters.
+
+    The *table* specifies the name of the table that stores log messages.
+    A new table will be created if it doesn't exist. The table name must
+    conform to the naming convention for Azure Storage table, see
+    `the naming convention for tables <http://msdn.microsoft.com/library/azure/dd179338.aspx>`_
+    for more details.
+
+    The *protocol* specifies the protocol to transfer data between
+    Azure Storage and your application, ``http`` and ``https``
+    are supported.
+
+    You can specify the *batch_size* in an integer if you want to use
+    batch transaction when creating new log entities. If the *batch_size*
+    is greater than 1, all new log entities will be transferred to the
+    table at a time when the number of new log messages reaches the
+    *batch_size*. Otherwise, a new log entity will be transferred to
+    the table every time a logging is performed. The *batch_size* must be
+    up to 100 (maximum number of entities in a batch transaction for
+    Azure Storage table).
+
+    The *extra_properties* accepts a sequence of
+    `the formats for logging <http://docs.python.org/2.7/library/logging.html#logrecord-attributes>`_.
+    The handler-specific one ``%(hostname)s`` is also acceptable.
+    The handler assigns an entity property for every format specified in
+    *extra_properties*. Here is an example of using extra properties:
+
+    ::
+
+        import logging
+        from azure_storage_logging.handlers import TableStorageHandler
+
+        # configure the handler and add it to the logger
+        logger = logging.getLogger('example')
+        handler = TableStorageHandler(conn_str='myConnectionString', table='myTableName',
+                                      extra_properties=('%(hostname)s',
+                                                        '%(levelname)s'))
+        logger.addHandler(handler)
+
+        # output log messages
+        logger.info('info message')
+        logger.warning('warning message')
+        logger.error('error message')
+
+    And it will create the log entities, that have the extra properties
+    in addition to the regular property *message*, into the table like this:
+
+    +--------------+-----------+----------------+----------+-----------+---------------+
+    | PartitionKey | RowKey    | Timestamp      | hostname | levelname | message       |
+    +==============+===========+================+==========+===========+===============+
+    | XXXXX        | XXXXXXXXX | YYYY-MM-DD ... | myhost   | INFO      | info message  |
+    +--------------+-----------+----------------+----------+-----------+---------------+
+    | XXXXX        | XXXXXXXXX | YYYY-MM-DD ... | myhost   | WARNING   | warn message  |
+    +--------------+-----------+----------------+----------+-----------+---------------+
+    | XXXXX        | XXXXXXXXX | YYYY-MM-DD ... | myhost   | ERROR     | error message |
+    +--------------+-----------+----------------+----------+-----------+---------------+
+
+    You can specify an instance of your custom **logging.Formatters**
+    for the *partition_key_formatter* or the *row_key_formatter*
+    if you want to implement your own keys for the table.
+    The default formatters will be used for partition keys and row keys
+    if no custom formatter for them is given to the handler.
+    The default values for partition keys are provided by the format
+    ``%(asctime)s`` and the date format ``%Y%m%d%H%M`` (provides a unique
+    value per minute). The default values for row keys are provided by the
+    format ``%(asctime)s%(msecs)03d-%(hostname)s-%(process)d-%(rowno)02d``
+    and the date format ``%Y%m%d%H%M%S``.
+
+    Note that the format ``%(rowno)d`` is a handler-specific one only
+    available for row keys. It would be formatted to a sequential and
+    unique number in a batch that starts from 0. The format is introduced
+    to avoid collision of row keys generated in a batch, and it would
+    always be formatted to 0 if you don't use batch transaction for logging
+    to the table.
+
+* setPartitionKeyFormatter(*fmt*)
+
+    Sets the handler's formatter for partition keys to *fmt*.
+
+* setRowKeyFormatter(*fmt*)
+
+    Sets the handler's formatter for row keys to *fmt*.
+
+Example
+-------
+
+Here is an example of the configurations and the logging that uses
+three different types of storage from the logger:
+
+::
+
+    LOGGING = {
+        'version': 1,
+        'formatters': {
+            'simple': {
+                'format': '%(asctime)s %(message)s',
+            },
+            'verbose': {
+                'format': '%(asctime)s %(levelname)s %(hostname)s %(process)d %(message)s',
+            },
+            # this is the same as the default, so you can skip configuring it
+            'partition_key': {
+                'format': '%(asctime)s',
+                'datefmt': '%Y%m%d%H%M',
+            },
+            # this is the same as the default, so you can skip configuring it
+            'row_key': {
+                'format': '%(asctime)s%(msecs)03d-%(hostname)s-%(process)d-%(rowno)02d',
+                'datefmt': '%Y%m%d%H%M%S',
+            },
+        },
+        'handlers': {
+            'table': {
+                'conn_str': DefaultEndpointsProtocol=https;AccountName=test;AccountKey=akey==;EndpointSuffix=core.windows.net'
+                'protocol': 'https',
+                'table': 'logs',
+                'level': 'INFO',
+                'class': 'azure_storage_logging.handlers.TableStorageHandler',
+                'formatter': 'simple',
+                'extra_properties': ['%(hostname)s', '%(levelname)s'],
+                'partition_key_formatter': 'cfg://formatters.partition_key',
+                'row_key_formatter': 'cfg://formatters.row_key',
+            },
+        },
+        'loggers': {
+            'example': {
+                'handlers': ['table'],
+                'level': 'DEBUG',
+            },
+        }
+    }
+
+    import logging
+    from logging.config import dictConfig
+
+    dictConfig(LOGGING)
+    logger = logging.getLogger('example')
+    logger.debug('debug message')
+    logger.info('info message')
+    logger.warning('warning message')
+    logger.error('error message')
+    logger.critical('critical message')
+
+Notice
+------
+
+* Set *is_emulated* to ``True`` at initialization of the logging handlers
+  if you want to use this package with Azure storage emulator.
+
+License
+-------
+
+Apache License 2.0
+
+Credits
+-------
+
+-  `Abian Rodriguez <http://github.com/AbianG>`__
+-  `Michiya Takahashi <http://github.com/michiya/>`__
```

### Comparing `azure-storage-logging_updated-0.6.0/README.rst` & `azure-storage-logging_updated-0.7.0/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,10 @@
 azure-storage-logging_updated
 =================================
 
-.. image:: http://img.shields.io/pypi/v/azure-storage-logging.svg?style=flat
-    :target: https://pypi.python.org/pypi/azure-storage-logging
-
 .. image:: http://img.shields.io/pypi/l/azure-storage-logging.svg?style=flat
     :target: http://www.apache.org/licenses/LICENSE-2.0.html
 
 *azure-storage-logging_table* is a fork from *azure-storage-logging* out of the author's necesity to send output from the standard Python logging APIs to Microsoft Azure Storage Tables.
 Due to the original module by Michiya Takahashi being outdated, it modifies it to restore functionality to the TableStorageHandler for logging. 
 In the future, more functionalities may be restored. But on this current version only the TableStorageHandler is usable.
```

### Comparing `azure-storage-logging_updated-0.6.0/azure_storage_logging/handlers.py` & `azure-storage-logging_updated-0.7.0/azure_storage_logging/handlers.py`

 * *Files identical despite different names*

### Comparing `azure-storage-logging_updated-0.6.0/azure_storage_logging_updated.egg-info/PKG-INFO` & `azure-storage-logging_updated-0.7.0/azure_storage_logging_updated.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,243 +1,241 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: azure-storage-logging-updated
-Version: 0.6.0
+Version: 0.7.0
 Summary: Logging handlers to send logs to Microsoft Azure Storage
 Home-page: https://github.com/AbianG/azure-storage-logging_updated
 Author: Abian Rodriguez
 Author-email: abiangrodriguez@protonmail.com
 License: Apache License 2.0
-Description: azure-storage-logging_updated
-        =================================
-        
-        .. image:: http://img.shields.io/pypi/v/azure-storage-logging.svg?style=flat
-            :target: https://pypi.python.org/pypi/azure-storage-logging
-        
-        .. image:: http://img.shields.io/pypi/l/azure-storage-logging.svg?style=flat
-            :target: http://www.apache.org/licenses/LICENSE-2.0.html
-        
-        *azure-storage-logging_table* is a fork from *azure-storage-logging* out of the author's necesity to send output from the standard Python logging APIs to Microsoft Azure Storage Tables.
-        Due to the original module by Michiya Takahashi being outdated, it modifies it to restore functionality to the TableStorageHandler for logging. 
-        In the future, more functionalities may be restored. But on this current version only the TableStorageHandler is usable.
-        
-        Dependencies
-        ------------
-        
-        * azure-data-tables 12.4.0
-        
-        Installation
-        ------------
-        
-        Install the package via pip: ::
-        
-            pip install azure-storage-logging_table
-        
-        Usage
-        -----
-        
-        The module **azure_storage_logging.handlers** in the package contains
-        the following logging handler classes. Each of them uses a different
-        type of Microsoft Azure Storage to send its output to. They all are subclasses
-        of the standard Python logging handler classes, so you can make use of them
-        in the standard ways of Python logging configuration.
-        
-        In addition to
-        `the standard formats for logging <http://docs.python.org/2.7/library/logging.html#logrecord-attributes>`_,
-        the special format ``%(hostname)s`` is also available in your message formatter
-        for the handlers. The format is introduced for ease of identifying the source
-        of log messages which come from many computers and go to the same storage.
-        
-        TableStorageHandler
-        ~~~~~~~~~~~~~~~~~~~
-        The **TableStorageHandler** class is a subclass of **logging.Handler** class,
-        and it sends log messages to Azure table storage and store them
-        as entities in the specified table.
-        
-        The handler puts a formatted log message from applications in the *message*
-        property of a table entity along with some system-defined properties
-        (*PartitionKey*, *RowKey*, and *Timestamp*) like this:
-        
-        +--------------+-----------+----------------+-------------+
-        | PartitionKey | RowKey    | Timestamp      | message     |
-        +==============+===========+================+=============+
-        | XXXXX        | XXXXXXXXX | YYYY-MM-DD ... | log message |
-        +--------------+-----------+----------------+-------------+
-        | XXXXX        | XXXXXXXXX | YYYY-MM-DD ... | log message |
-        +--------------+-----------+----------------+-------------+
-        | XXXXX        | XXXXXXXXX | YYYY-MM-DD ... | log message |
-        +--------------+-----------+----------------+-------------+
-        
-        * *class* azure_storage_logging.handlers.TableStorageHandler(*account_name=None, account_key=None, protocol='https', table='logs', batch_size=0, extra_properties=None, partition_key_formatter=None, row_key_formatter=None, is_emulated=False*)
-        
-            Returns a new instance of the **TableStorageHandler** class.
-            The instance is initialized with the name and the key of your
-            Azure Storage account and some optional parameters.
-        
-            The *table* specifies the name of the table that stores log messages.
-            A new table will be created if it doesn't exist. The table name must
-            conform to the naming convention for Azure Storage table, see
-            `the naming convention for tables <http://msdn.microsoft.com/library/azure/dd179338.aspx>`_
-            for more details.
-        
-            The *protocol* specifies the protocol to transfer data between
-            Azure Storage and your application, ``http`` and ``https``
-            are supported.
-        
-            You can specify the *batch_size* in an integer if you want to use
-            batch transaction when creating new log entities. If the *batch_size*
-            is greater than 1, all new log entities will be transferred to the
-            table at a time when the number of new log messages reaches the
-            *batch_size*. Otherwise, a new log entity will be transferred to
-            the table every time a logging is performed. The *batch_size* must be
-            up to 100 (maximum number of entities in a batch transaction for
-            Azure Storage table).
-        
-            The *extra_properties* accepts a sequence of
-            `the formats for logging <http://docs.python.org/2.7/library/logging.html#logrecord-attributes>`_.
-            The handler-specific one ``%(hostname)s`` is also acceptable.
-            The handler assigns an entity property for every format specified in
-            *extra_properties*. Here is an example of using extra properties:
-        
-            ::
-        
-                import logging
-                from azure_storage_logging.handlers import TableStorageHandler
-        
-                # configure the handler and add it to the logger
-                logger = logging.getLogger('example')
-                handler = TableStorageHandler(conn_str='myConnectionString', table='myTableName',
-                                              extra_properties=('%(hostname)s',
-                                                                '%(levelname)s'))
-                logger.addHandler(handler)
-        
-                # output log messages
-                logger.info('info message')
-                logger.warning('warning message')
-                logger.error('error message')
-        
-            And it will create the log entities, that have the extra properties
-            in addition to the regular property *message*, into the table like this:
-        
-            +--------------+-----------+----------------+----------+-----------+---------------+
-            | PartitionKey | RowKey    | Timestamp      | hostname | levelname | message       |
-            +==============+===========+================+==========+===========+===============+
-            | XXXXX        | XXXXXXXXX | YYYY-MM-DD ... | myhost   | INFO      | info message  |
-            +--------------+-----------+----------------+----------+-----------+---------------+
-            | XXXXX        | XXXXXXXXX | YYYY-MM-DD ... | myhost   | WARNING   | warn message  |
-            +--------------+-----------+----------------+----------+-----------+---------------+
-            | XXXXX        | XXXXXXXXX | YYYY-MM-DD ... | myhost   | ERROR     | error message |
-            +--------------+-----------+----------------+----------+-----------+---------------+
-        
-            You can specify an instance of your custom **logging.Formatters**
-            for the *partition_key_formatter* or the *row_key_formatter*
-            if you want to implement your own keys for the table.
-            The default formatters will be used for partition keys and row keys
-            if no custom formatter for them is given to the handler.
-            The default values for partition keys are provided by the format
-            ``%(asctime)s`` and the date format ``%Y%m%d%H%M`` (provides a unique
-            value per minute). The default values for row keys are provided by the
-            format ``%(asctime)s%(msecs)03d-%(hostname)s-%(process)d-%(rowno)02d``
-            and the date format ``%Y%m%d%H%M%S``.
-        
-            Note that the format ``%(rowno)d`` is a handler-specific one only
-            available for row keys. It would be formatted to a sequential and
-            unique number in a batch that starts from 0. The format is introduced
-            to avoid collision of row keys generated in a batch, and it would
-            always be formatted to 0 if you don't use batch transaction for logging
-            to the table.
-        
-        * setPartitionKeyFormatter(*fmt*)
-        
-            Sets the handler's formatter for partition keys to *fmt*.
-        
-        * setRowKeyFormatter(*fmt*)
-        
-            Sets the handler's formatter for row keys to *fmt*.
-        
-        Example
-        -------
-        
-        Here is an example of the configurations and the logging that uses
-        three different types of storage from the logger:
-        
-        ::
-        
-            LOGGING = {
-                'version': 1,
-                'formatters': {
-                    'simple': {
-                        'format': '%(asctime)s %(message)s',
-                    },
-                    'verbose': {
-                        'format': '%(asctime)s %(levelname)s %(hostname)s %(process)d %(message)s',
-                    },
-                    # this is the same as the default, so you can skip configuring it
-                    'partition_key': {
-                        'format': '%(asctime)s',
-                        'datefmt': '%Y%m%d%H%M',
-                    },
-                    # this is the same as the default, so you can skip configuring it
-                    'row_key': {
-                        'format': '%(asctime)s%(msecs)03d-%(hostname)s-%(process)d-%(rowno)02d',
-                        'datefmt': '%Y%m%d%H%M%S',
-                    },
-                },
-                'handlers': {
-                    'table': {
-                        'conn_str': DefaultEndpointsProtocol=https;AccountName=test;AccountKey=akey==;EndpointSuffix=core.windows.net'
-                        'protocol': 'https',
-                        'table': 'logs',
-                        'level': 'INFO',
-                        'class': 'azure_storage_logging.handlers.TableStorageHandler',
-                        'formatter': 'simple',
-                        'extra_properties': ['%(hostname)s', '%(levelname)s'],
-                        'partition_key_formatter': 'cfg://formatters.partition_key',
-                        'row_key_formatter': 'cfg://formatters.row_key',
-                    },
-                },
-                'loggers': {
-                    'example': {
-                        'handlers': ['table'],
-                        'level': 'DEBUG',
-                    },
-                }
-            }
-        
-            import logging
-            from logging.config import dictConfig
-        
-            dictConfig(LOGGING)
-            logger = logging.getLogger('example')
-            logger.debug('debug message')
-            logger.info('info message')
-            logger.warning('warning message')
-            logger.error('error message')
-            logger.critical('critical message')
-        
-        Notice
-        ------
-        
-        * Set *is_emulated* to ``True`` at initialization of the logging handlers
-          if you want to use this package with Azure storage emulator.
-        
-        License
-        -------
-        
-        Apache License 2.0
-        
-        Credits
-        -------
-        
-        -  `Abian Rodriguez <http://github.com/AbianG>`__
-        -  `Michiya Takahashi <http://github.com/michiya/>`__
 Keywords: azure logging
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Topic :: System :: Logging
+License-File: LICENSE
+
+azure-storage-logging_updated
+=================================
+
+.. image:: http://img.shields.io/pypi/l/azure-storage-logging.svg?style=flat
+    :target: http://www.apache.org/licenses/LICENSE-2.0.html
+
+*azure-storage-logging_table* is a fork from *azure-storage-logging* out of the author's necesity to send output from the standard Python logging APIs to Microsoft Azure Storage Tables.
+Due to the original module by Michiya Takahashi being outdated, it modifies it to restore functionality to the TableStorageHandler for logging. 
+In the future, more functionalities may be restored. But on this current version only the TableStorageHandler is usable.
+
+Dependencies
+------------
+
+* azure-data-tables 12.4.0
+
+Installation
+------------
+
+Install the package via pip: ::
+
+    pip install azure-storage-logging_table
+
+Usage
+-----
+
+The module **azure_storage_logging.handlers** in the package contains
+the following logging handler classes. Each of them uses a different
+type of Microsoft Azure Storage to send its output to. They all are subclasses
+of the standard Python logging handler classes, so you can make use of them
+in the standard ways of Python logging configuration.
+
+In addition to
+`the standard formats for logging <http://docs.python.org/2.7/library/logging.html#logrecord-attributes>`_,
+the special format ``%(hostname)s`` is also available in your message formatter
+for the handlers. The format is introduced for ease of identifying the source
+of log messages which come from many computers and go to the same storage.
+
+TableStorageHandler
+~~~~~~~~~~~~~~~~~~~
+The **TableStorageHandler** class is a subclass of **logging.Handler** class,
+and it sends log messages to Azure table storage and store them
+as entities in the specified table.
+
+The handler puts a formatted log message from applications in the *message*
+property of a table entity along with some system-defined properties
+(*PartitionKey*, *RowKey*, and *Timestamp*) like this:
+
++--------------+-----------+----------------+-------------+
+| PartitionKey | RowKey    | Timestamp      | message     |
++==============+===========+================+=============+
+| XXXXX        | XXXXXXXXX | YYYY-MM-DD ... | log message |
++--------------+-----------+----------------+-------------+
+| XXXXX        | XXXXXXXXX | YYYY-MM-DD ... | log message |
++--------------+-----------+----------------+-------------+
+| XXXXX        | XXXXXXXXX | YYYY-MM-DD ... | log message |
++--------------+-----------+----------------+-------------+
+
+* *class* azure_storage_logging.handlers.TableStorageHandler(*account_name=None, account_key=None, protocol='https', table='logs', batch_size=0, extra_properties=None, partition_key_formatter=None, row_key_formatter=None, is_emulated=False*)
+
+    Returns a new instance of the **TableStorageHandler** class.
+    The instance is initialized with the name and the key of your
+    Azure Storage account and some optional parameters.
+
+    The *table* specifies the name of the table that stores log messages.
+    A new table will be created if it doesn't exist. The table name must
+    conform to the naming convention for Azure Storage table, see
+    `the naming convention for tables <http://msdn.microsoft.com/library/azure/dd179338.aspx>`_
+    for more details.
+
+    The *protocol* specifies the protocol to transfer data between
+    Azure Storage and your application, ``http`` and ``https``
+    are supported.
+
+    You can specify the *batch_size* in an integer if you want to use
+    batch transaction when creating new log entities. If the *batch_size*
+    is greater than 1, all new log entities will be transferred to the
+    table at a time when the number of new log messages reaches the
+    *batch_size*. Otherwise, a new log entity will be transferred to
+    the table every time a logging is performed. The *batch_size* must be
+    up to 100 (maximum number of entities in a batch transaction for
+    Azure Storage table).
+
+    The *extra_properties* accepts a sequence of
+    `the formats for logging <http://docs.python.org/2.7/library/logging.html#logrecord-attributes>`_.
+    The handler-specific one ``%(hostname)s`` is also acceptable.
+    The handler assigns an entity property for every format specified in
+    *extra_properties*. Here is an example of using extra properties:
+
+    ::
+
+        import logging
+        from azure_storage_logging.handlers import TableStorageHandler
+
+        # configure the handler and add it to the logger
+        logger = logging.getLogger('example')
+        handler = TableStorageHandler(conn_str='myConnectionString', table='myTableName',
+                                      extra_properties=('%(hostname)s',
+                                                        '%(levelname)s'))
+        logger.addHandler(handler)
+
+        # output log messages
+        logger.info('info message')
+        logger.warning('warning message')
+        logger.error('error message')
+
+    And it will create the log entities, that have the extra properties
+    in addition to the regular property *message*, into the table like this:
+
+    +--------------+-----------+----------------+----------+-----------+---------------+
+    | PartitionKey | RowKey    | Timestamp      | hostname | levelname | message       |
+    +==============+===========+================+==========+===========+===============+
+    | XXXXX        | XXXXXXXXX | YYYY-MM-DD ... | myhost   | INFO      | info message  |
+    +--------------+-----------+----------------+----------+-----------+---------------+
+    | XXXXX        | XXXXXXXXX | YYYY-MM-DD ... | myhost   | WARNING   | warn message  |
+    +--------------+-----------+----------------+----------+-----------+---------------+
+    | XXXXX        | XXXXXXXXX | YYYY-MM-DD ... | myhost   | ERROR     | error message |
+    +--------------+-----------+----------------+----------+-----------+---------------+
+
+    You can specify an instance of your custom **logging.Formatters**
+    for the *partition_key_formatter* or the *row_key_formatter*
+    if you want to implement your own keys for the table.
+    The default formatters will be used for partition keys and row keys
+    if no custom formatter for them is given to the handler.
+    The default values for partition keys are provided by the format
+    ``%(asctime)s`` and the date format ``%Y%m%d%H%M`` (provides a unique
+    value per minute). The default values for row keys are provided by the
+    format ``%(asctime)s%(msecs)03d-%(hostname)s-%(process)d-%(rowno)02d``
+    and the date format ``%Y%m%d%H%M%S``.
+
+    Note that the format ``%(rowno)d`` is a handler-specific one only
+    available for row keys. It would be formatted to a sequential and
+    unique number in a batch that starts from 0. The format is introduced
+    to avoid collision of row keys generated in a batch, and it would
+    always be formatted to 0 if you don't use batch transaction for logging
+    to the table.
+
+* setPartitionKeyFormatter(*fmt*)
+
+    Sets the handler's formatter for partition keys to *fmt*.
+
+* setRowKeyFormatter(*fmt*)
+
+    Sets the handler's formatter for row keys to *fmt*.
+
+Example
+-------
+
+Here is an example of the configurations and the logging that uses
+three different types of storage from the logger:
+
+::
+
+    LOGGING = {
+        'version': 1,
+        'formatters': {
+            'simple': {
+                'format': '%(asctime)s %(message)s',
+            },
+            'verbose': {
+                'format': '%(asctime)s %(levelname)s %(hostname)s %(process)d %(message)s',
+            },
+            # this is the same as the default, so you can skip configuring it
+            'partition_key': {
+                'format': '%(asctime)s',
+                'datefmt': '%Y%m%d%H%M',
+            },
+            # this is the same as the default, so you can skip configuring it
+            'row_key': {
+                'format': '%(asctime)s%(msecs)03d-%(hostname)s-%(process)d-%(rowno)02d',
+                'datefmt': '%Y%m%d%H%M%S',
+            },
+        },
+        'handlers': {
+            'table': {
+                'conn_str': DefaultEndpointsProtocol=https;AccountName=test;AccountKey=akey==;EndpointSuffix=core.windows.net'
+                'protocol': 'https',
+                'table': 'logs',
+                'level': 'INFO',
+                'class': 'azure_storage_logging.handlers.TableStorageHandler',
+                'formatter': 'simple',
+                'extra_properties': ['%(hostname)s', '%(levelname)s'],
+                'partition_key_formatter': 'cfg://formatters.partition_key',
+                'row_key_formatter': 'cfg://formatters.row_key',
+            },
+        },
+        'loggers': {
+            'example': {
+                'handlers': ['table'],
+                'level': 'DEBUG',
+            },
+        }
+    }
+
+    import logging
+    from logging.config import dictConfig
+
+    dictConfig(LOGGING)
+    logger = logging.getLogger('example')
+    logger.debug('debug message')
+    logger.info('info message')
+    logger.warning('warning message')
+    logger.error('error message')
+    logger.critical('critical message')
+
+Notice
+------
+
+* Set *is_emulated* to ``True`` at initialization of the logging handlers
+  if you want to use this package with Azure storage emulator.
+
+License
+-------
+
+Apache License 2.0
+
+Credits
+-------
+
+-  `Abian Rodriguez <http://github.com/AbianG>`__
+-  `Michiya Takahashi <http://github.com/michiya/>`__
```

### Comparing `azure-storage-logging_updated-0.6.0/setup.py` & `azure-storage-logging_updated-0.7.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,21 +14,21 @@
     'Programming Language :: Python :: 3.4',
     'Programming Language :: Python :: 3.5',
     'Topic :: System :: Logging',
 ]
 
 setup(
     name='azure-storage-logging_updated',
-    version='0.6.0',
+    version='0.7.0',
     description='Logging handlers to send logs to Microsoft Azure Storage',
     long_description=open('README.rst').read(),
     author='Abian Rodriguez',
     author_email='abiangrodriguez@protonmail.com',
     url='https://github.com/AbianG/azure-storage-logging_updated',
     license='Apache License 2.0',
     packages=['azure_storage_logging'],
     install_requires=[
-        'azure-data-tables==12.2.0'
+        'azure-data-tables==12.4.0'
     ],
     classifiers=CLASSIFIERS,
     keywords='azure logging',
 )
```

