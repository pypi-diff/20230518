# Comparing `tmp/knockoff-4.3.2.tar.gz` & `tmp/knockoff-4.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "knockoff-4.3.2.tar", max compression
+gzip compressed data, was "knockoff-4.4.0.tar", max compression
```

## Comparing `knockoff-4.3.2.tar` & `knockoff-4.4.0.tar`

### file list

```diff
@@ -1,65 +1,63 @@
--rw-r--r--   0        0        0    10329 2022-08-03 21:49:30.454897 knockoff-4.3.2/LICENSE.md
--rw-r--r--   0        0        0     4429 2022-08-03 21:49:30.458897 knockoff-4.3.2/README.md
--rw-r--r--   0        0        0      281 2022-08-03 21:49:30.458897 knockoff-4.3.2/knockoff/__init__.py
--rw-r--r--   0        0        0     5049 2022-08-03 21:49:30.458897 knockoff-4.3.2/knockoff/cli.py
--rw-r--r--   0        0        0     2514 2022-08-03 21:49:30.458897 knockoff-4.3.2/knockoff/cli_v2.py
--rw-r--r--   0        0        0      193 2022-08-03 21:49:30.458897 knockoff-4.3.2/knockoff/command/__init__.py
--rw-r--r--   0        0        0     4847 2022-08-03 21:49:30.458897 knockoff-4.3.2/knockoff/command/run.py
--rw-r--r--   0        0        0      349 2022-08-03 21:49:30.458897 knockoff-4.3.2/knockoff/command/version.py
--rw-r--r--   0        0        0     1217 2022-08-03 21:49:30.458897 knockoff-4.3.2/knockoff/exceptions.py
--rw-r--r--   0        0        0      193 2022-08-03 21:49:30.458897 knockoff-4.3.2/knockoff/factory/__init__.py
--rw-r--r--   0        0        0     7958 2022-08-03 21:49:30.458897 knockoff-4.3.2/knockoff/factory/assembly.py
--rw-r--r--   0        0        0      979 2022-08-03 21:49:30.458897 knockoff-4.3.2/knockoff/factory/component.py
--rw-r--r--   0        0        0     1946 2022-08-03 21:49:30.458897 knockoff-4.3.2/knockoff/factory/counterfeit.py
--rw-r--r--   0        0        0     1862 2022-08-03 21:49:30.458897 knockoff-4.3.2/knockoff/factory/node.py
--rw-r--r--   0        0        0     2166 2022-08-03 21:49:30.458897 knockoff-4.3.2/knockoff/factory/part.py
--rw-r--r--   0        0        0     5642 2022-08-03 21:49:30.458897 knockoff-4.3.2/knockoff/factory/prototype.py
--rw-r--r--   0        0        0      676 2022-08-03 21:49:30.458897 knockoff-4.3.2/knockoff/factory/sink.py
--rw-r--r--   0        0        0     1762 2022-08-03 21:49:30.458897 knockoff-4.3.2/knockoff/factory/source.py
--rw-r--r--   0        0        0      488 2022-08-03 21:49:30.458897 knockoff-4.3.2/knockoff/factory/table.py
--rw-r--r--   0        0        0     1643 2022-08-03 21:49:30.458897 knockoff-4.3.2/knockoff/io.py
--rw-r--r--   0        0        0     2073 2022-08-03 21:49:30.458897 knockoff-4.3.2/knockoff/knockoff.py
--rw-r--r--   0        0        0     3760 2022-08-03 21:49:30.458897 knockoff-4.3.2/knockoff/orm.py
--rw-r--r--   0        0        0      193 2022-08-03 21:49:30.458897 knockoff-4.3.2/knockoff/sdk/__init__.py
--rw-r--r--   0        0        0     1608 2022-08-03 21:49:30.458897 knockoff-4.3.2/knockoff/sdk/blueprint.py
--rw-r--r--   0        0        0     1270 2022-08-03 21:49:30.458897 knockoff-4.3.2/knockoff/sdk/constraints.py
--rw-r--r--   0        0        0      193 2022-08-03 21:49:30.458897 knockoff-4.3.2/knockoff/sdk/container/__init__.py
--rw-r--r--   0        0        0      986 2022-08-03 21:49:30.458897 knockoff-4.3.2/knockoff/sdk/container/default.py
--rw-r--r--   0        0        0     1404 2022-08-03 21:49:30.458897 knockoff-4.3.2/knockoff/sdk/dag.py
--rw-r--r--   0        0        0     8053 2022-08-03 21:49:30.458897 knockoff-4.3.2/knockoff/sdk/db.py
--rw-r--r--   0        0        0      193 2022-08-03 21:49:30.458897 knockoff-4.3.2/knockoff/sdk/factory/__init__.py
--rw-r--r--   0        0        0     6099 2022-08-03 21:49:30.458897 knockoff-4.3.2/knockoff/sdk/factory/collections.py
--rw-r--r--   0        0        0     2013 2022-08-03 21:49:30.458897 knockoff-4.3.2/knockoff/sdk/factory/column.py
--rw-r--r--   0        0        0      193 2022-08-03 21:49:30.458897 knockoff-4.3.2/knockoff/sdk/factory/next_strategy/__init__.py
--rw-r--r--   0        0        0      561 2022-08-03 21:49:30.458897 knockoff-4.3.2/knockoff/sdk/factory/next_strategy/df.py
--rw-r--r--   0        0        0      389 2022-08-03 21:49:30.458897 knockoff-4.3.2/knockoff/sdk/factory/next_strategy/table.py
--rw-r--r--   0        0        0    13901 2022-08-03 21:49:30.458897 knockoff-4.3.2/knockoff/sdk/table.py
--rw-r--r--   0        0        0      193 2022-08-03 21:49:30.458897 knockoff-4.3.2/knockoff/tempdb/__init__.py
--rw-r--r--   0        0        0     1060 2022-08-03 21:49:30.458897 knockoff-4.3.2/knockoff/tempdb/container.py
--rw-r--r--   0        0        0     2374 2022-08-03 21:49:30.458897 knockoff-4.3.2/knockoff/tempdb/db.py
--rw-r--r--   0        0        0      557 2022-08-03 21:49:30.458897 knockoff-4.3.2/knockoff/tempdb/initialize_tables.py
--rw-r--r--   0        0        0      786 2022-08-03 21:49:30.458897 knockoff-4.3.2/knockoff/tempdb/setup_teardown.py
--rw-r--r--   0        0        0      675 2022-08-03 21:49:30.458897 knockoff-4.3.2/knockoff/testing_postgresql.py
--rw-r--r--   0        0        0      193 2022-08-03 21:49:30.458897 knockoff-4.3.2/knockoff/utilities/__init__.py
--rw-r--r--   0        0        0      193 2022-08-03 21:49:30.458897 knockoff-4.3.2/knockoff/utilities/date/__init__.py
--rw-r--r--   0        0        0     6914 2022-08-03 21:49:30.458897 knockoff-4.3.2/knockoff/utilities/date/interval.py
--rw-r--r--   0        0        0      872 2022-08-03 21:49:30.458897 knockoff-4.3.2/knockoff/utilities/environ.py
--rw-r--r--   0        0        0      777 2022-08-03 21:49:30.458897 knockoff-4.3.2/knockoff/utilities/functools.py
--rw-r--r--   0        0        0      666 2022-08-03 21:49:30.458897 knockoff-4.3.2/knockoff/utilities/importlib_utils.py
--rw-r--r--   0        0        0     1080 2022-08-03 21:49:30.458897 knockoff-4.3.2/knockoff/utilities/io.py
--rw-r--r--   0        0        0     1374 2022-08-03 21:49:30.458897 knockoff-4.3.2/knockoff/utilities/ioc.py
--rw-r--r--   0        0        0     1916 2022-08-03 21:49:30.458897 knockoff-4.3.2/knockoff/utilities/mixin.py
--rw-r--r--   0        0        0      193 2022-08-03 21:49:30.458897 knockoff-4.3.2/knockoff/utilities/orm/__init__.py
--rw-r--r--   0        0        0     6540 2022-08-03 21:49:30.458897 knockoff-4.3.2/knockoff/utilities/orm/sql.py
--rw-r--r--   0        0        0      666 2022-08-03 21:49:30.458897 knockoff-4.3.2/knockoff/utilities/orm/sqlalchemy_conn.py
--rw-r--r--   0        0        0      830 2022-08-03 21:49:30.458897 knockoff-4.3.2/knockoff/utilities/period.py
--rw-r--r--   0        0        0     1236 2022-08-03 21:49:30.458897 knockoff-4.3.2/knockoff/utilities/regex.py
--rw-r--r--   0        0        0      194 2022-08-03 21:49:30.458897 knockoff-4.3.2/knockoff/utilities/testing/__init__.py
--rw-r--r--   0        0        0     1369 2022-08-03 21:49:30.458897 knockoff-4.3.2/knockoff/utilities/testing/base.py
--rw-r--r--   0        0        0     1166 2022-08-03 21:49:30.458897 knockoff-4.3.2/knockoff/utilities/testing/mysql.py
--rw-r--r--   0        0        0     1436 2022-08-03 21:49:30.458897 knockoff-4.3.2/knockoff/utilities/testing/postgresql.py
--rw-r--r--   0        0        0      193 2022-08-03 21:49:30.458897 knockoff-4.3.2/knockoff/writer/__init__.py
--rw-r--r--   0        0        0     1638 2022-08-03 21:49:30.458897 knockoff-4.3.2/knockoff/writer/pandas.py
--rw-r--r--   0        0        0     3435 2022-08-03 21:49:30.458897 knockoff-4.3.2/pyproject.toml
--rw-r--r--   0        0        0     9451 2022-08-03 21:49:38.550904 knockoff-4.3.2/setup.py
--rw-r--r--   0        0        0     5880 2022-08-03 21:49:38.551536 knockoff-4.3.2/PKG-INFO
+-rw-r--r--   0        0        0    10329 2023-05-18 16:28:09.524580 knockoff-4.4.0/LICENSE.md
+-rw-r--r--   0        0        0     4429 2023-05-18 16:28:09.524580 knockoff-4.4.0/README.md
+-rw-r--r--   0        0        0      266 2023-05-18 16:28:09.524580 knockoff-4.4.0/knockoff/__init__.py
+-rw-r--r--   0        0        0     5101 2023-05-18 16:28:09.524580 knockoff-4.4.0/knockoff/cli.py
+-rw-r--r--   0        0        0     2522 2023-05-18 16:28:09.524580 knockoff-4.4.0/knockoff/cli_v2.py
+-rw-r--r--   0        0        0      193 2023-05-18 16:28:09.524580 knockoff-4.4.0/knockoff/command/__init__.py
+-rw-r--r--   0        0        0     4847 2023-05-18 16:28:09.524580 knockoff-4.4.0/knockoff/command/run.py
+-rw-r--r--   0        0        0      349 2023-05-18 16:28:09.524580 knockoff-4.4.0/knockoff/command/version.py
+-rw-r--r--   0        0        0     1217 2023-05-18 16:28:09.524580 knockoff-4.4.0/knockoff/exceptions.py
+-rw-r--r--   0        0        0      193 2023-05-18 16:28:09.524580 knockoff-4.4.0/knockoff/factory/__init__.py
+-rw-r--r--   0        0        0     7958 2023-05-18 16:28:09.524580 knockoff-4.4.0/knockoff/factory/assembly.py
+-rw-r--r--   0        0        0      979 2023-05-18 16:28:09.524580 knockoff-4.4.0/knockoff/factory/component.py
+-rw-r--r--   0        0        0     1946 2023-05-18 16:28:09.524580 knockoff-4.4.0/knockoff/factory/counterfeit.py
+-rw-r--r--   0        0        0     1862 2023-05-18 16:28:09.524580 knockoff-4.4.0/knockoff/factory/node.py
+-rw-r--r--   0        0        0     2166 2023-05-18 16:28:09.524580 knockoff-4.4.0/knockoff/factory/part.py
+-rw-r--r--   0        0        0     5642 2023-05-18 16:28:09.524580 knockoff-4.4.0/knockoff/factory/prototype.py
+-rw-r--r--   0        0        0      676 2023-05-18 16:28:09.524580 knockoff-4.4.0/knockoff/factory/sink.py
+-rw-r--r--   0        0        0     1762 2023-05-18 16:28:09.524580 knockoff-4.4.0/knockoff/factory/source.py
+-rw-r--r--   0        0        0      488 2023-05-18 16:28:09.524580 knockoff-4.4.0/knockoff/factory/table.py
+-rw-r--r--   0        0        0     1584 2023-05-18 16:28:09.524580 knockoff-4.4.0/knockoff/io.py
+-rw-r--r--   0        0        0     2104 2023-05-18 16:28:09.524580 knockoff-4.4.0/knockoff/knockoff.py
+-rw-r--r--   0        0        0     3713 2023-05-18 16:28:09.524580 knockoff-4.4.0/knockoff/orm.py
+-rw-r--r--   0        0        0      193 2023-05-18 16:28:09.524580 knockoff-4.4.0/knockoff/sdk/__init__.py
+-rw-r--r--   0        0        0     1608 2023-05-18 16:28:09.524580 knockoff-4.4.0/knockoff/sdk/blueprint.py
+-rw-r--r--   0        0        0     1270 2023-05-18 16:28:09.524580 knockoff-4.4.0/knockoff/sdk/constraints.py
+-rw-r--r--   0        0        0      193 2023-05-18 16:28:09.524580 knockoff-4.4.0/knockoff/sdk/container/__init__.py
+-rw-r--r--   0        0        0      986 2023-05-18 16:28:09.524580 knockoff-4.4.0/knockoff/sdk/container/default.py
+-rw-r--r--   0        0        0     1404 2023-05-18 16:28:09.524580 knockoff-4.4.0/knockoff/sdk/dag.py
+-rw-r--r--   0        0        0     8115 2023-05-18 16:28:09.524580 knockoff-4.4.0/knockoff/sdk/db.py
+-rw-r--r--   0        0        0      193 2023-05-18 16:28:09.524580 knockoff-4.4.0/knockoff/sdk/factory/__init__.py
+-rw-r--r--   0        0        0     6140 2023-05-18 16:28:09.524580 knockoff-4.4.0/knockoff/sdk/factory/collections.py
+-rw-r--r--   0        0        0     2013 2023-05-18 16:28:09.524580 knockoff-4.4.0/knockoff/sdk/factory/column.py
+-rw-r--r--   0        0        0      193 2023-05-18 16:28:09.524580 knockoff-4.4.0/knockoff/sdk/factory/next_strategy/__init__.py
+-rw-r--r--   0        0        0      561 2023-05-18 16:28:09.524580 knockoff-4.4.0/knockoff/sdk/factory/next_strategy/df.py
+-rw-r--r--   0        0        0      423 2023-05-18 16:28:09.524580 knockoff-4.4.0/knockoff/sdk/factory/next_strategy/table.py
+-rw-r--r--   0        0        0    13925 2023-05-18 16:28:09.524580 knockoff-4.4.0/knockoff/sdk/table.py
+-rw-r--r--   0        0        0      193 2023-05-18 16:28:09.524580 knockoff-4.4.0/knockoff/tempdb/__init__.py
+-rw-r--r--   0        0        0     1060 2023-05-18 16:28:09.524580 knockoff-4.4.0/knockoff/tempdb/container.py
+-rw-r--r--   0        0        0     2389 2023-05-18 16:28:09.524580 knockoff-4.4.0/knockoff/tempdb/db.py
+-rw-r--r--   0        0        0      557 2023-05-18 16:28:09.524580 knockoff-4.4.0/knockoff/tempdb/initialize_tables.py
+-rw-r--r--   0        0        0      786 2023-05-18 16:28:09.524580 knockoff-4.4.0/knockoff/tempdb/setup_teardown.py
+-rw-r--r--   0        0        0      193 2023-05-18 16:28:09.524580 knockoff-4.4.0/knockoff/utilities/__init__.py
+-rw-r--r--   0        0        0      193 2023-05-18 16:28:09.524580 knockoff-4.4.0/knockoff/utilities/date/__init__.py
+-rw-r--r--   0        0        0     6914 2023-05-18 16:28:09.524580 knockoff-4.4.0/knockoff/utilities/date/interval.py
+-rw-r--r--   0        0        0      872 2023-05-18 16:28:09.524580 knockoff-4.4.0/knockoff/utilities/environ.py
+-rw-r--r--   0        0        0      552 2023-05-18 16:28:09.524580 knockoff-4.4.0/knockoff/utilities/functools.py
+-rw-r--r--   0        0        0      666 2023-05-18 16:28:09.524580 knockoff-4.4.0/knockoff/utilities/importlib_utils.py
+-rw-r--r--   0        0        0     1068 2023-05-18 16:28:09.524580 knockoff-4.4.0/knockoff/utilities/io.py
+-rw-r--r--   0        0        0     1374 2023-05-18 16:28:09.524580 knockoff-4.4.0/knockoff/utilities/ioc.py
+-rw-r--r--   0        0        0     1848 2023-05-18 16:28:09.524580 knockoff-4.4.0/knockoff/utilities/mixin.py
+-rw-r--r--   0        0        0      193 2023-05-18 16:28:09.524580 knockoff-4.4.0/knockoff/utilities/orm/__init__.py
+-rw-r--r--   0        0        0     6525 2023-05-18 16:28:09.524580 knockoff-4.4.0/knockoff/utilities/orm/sql.py
+-rw-r--r--   0        0        0      665 2023-05-18 16:28:09.524580 knockoff-4.4.0/knockoff/utilities/orm/sqlalchemy_conn.py
+-rw-r--r--   0        0        0      848 2023-05-18 16:28:09.524580 knockoff-4.4.0/knockoff/utilities/period.py
+-rw-r--r--   0        0        0     1199 2023-05-18 16:28:09.524580 knockoff-4.4.0/knockoff/utilities/regex.py
+-rw-r--r--   0        0        0      194 2023-05-18 16:28:09.524580 knockoff-4.4.0/knockoff/utilities/testing/__init__.py
+-rw-r--r--   0        0        0     1395 2023-05-18 16:28:09.524580 knockoff-4.4.0/knockoff/utilities/testing/base.py
+-rw-r--r--   0        0        0     1228 2023-05-18 16:28:09.524580 knockoff-4.4.0/knockoff/utilities/testing/mysql.py
+-rw-r--r--   0        0        0     1648 2023-05-18 16:28:09.524580 knockoff-4.4.0/knockoff/utilities/testing/postgresql.py
+-rw-r--r--   0        0        0      193 2023-05-18 16:28:09.524580 knockoff-4.4.0/knockoff/writer/__init__.py
+-rw-r--r--   0        0        0     1638 2023-05-18 16:28:09.524580 knockoff-4.4.0/knockoff/writer/pandas.py
+-rw-r--r--   0        0        0     3533 2023-05-18 16:28:09.528580 knockoff-4.4.0/pyproject.toml
+-rw-r--r--   0        0        0     5865 1970-01-01 00:00:00.000000 knockoff-4.4.0/PKG-INFO
```

### Comparing `knockoff-4.3.2/LICENSE.md` & `knockoff-4.4.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `knockoff-4.3.2/README.md` & `knockoff-4.4.0/README.md`

 * *Files identical despite different names*

### Comparing `knockoff-4.3.2/knockoff/cli.py` & `knockoff-4.4.0/knockoff/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,20 +14,20 @@
 import logging
 
 import sqlalchemy_utils
 from sqlalchemy import create_engine
 from sqlalchemy.exc import ProgrammingError
 
 from knockoff.utilities.functools import call_with_args_kwargs
-from .utilities.orm.sql import EngineBuilder
+from knockoff.utilities.orm.sql import EngineBuilder
 
-from . import orm, __version__
-from .io import ReaderFactory
-from .knockoff import Knockoff
-from .cli_v2 import setup_logger
+from knockoff import orm, __version__
+from knockoff.io import ReaderFactory
+from knockoff.knockoff import Knockoff
+from knockoff.cli_v2 import setup_logger
 
 
 logger = logging.getLogger(__name__)
 
 
 def shlex_join(cmd):
     return " ".join(map(pipes.quote, cmd))
@@ -61,15 +61,15 @@
 
         if sqlalchemy_utils.database_exists(url):
             logger.info("{} already exists. Skipping creation."
                         .format(config["name"]))
         else:
             # the following two lines remove configuration to specific db
             url = '/'.join(parts[:-1])
-            engine = create_engine(url)
+            engine = create_engine(url, future=True)
             orm.create_database(config['name'], engine=engine)
         for user_config in config.get('users', []):
             assert_supported_db_action(db_type)
             password = os.environ[user_config['password_env']]
             try:
                 orm.create_user(user_config['user'], password,
                                 engine=engine)
```

### Comparing `knockoff-4.3.2/knockoff/cli_v2.py` & `knockoff-4.4.0/knockoff/cli_v2.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 
 import os
 import argparse
 import logging
 import sys
 
-from .utilities.mixin import ResourceLocatorMixin
+from knockoff.utilities.mixin import ResourceLocatorMixin
 
 
 logger = logging.getLogger(__name__)
 
 
 class KnockoffCLI(ResourceLocatorMixin):
     entry_point_group = "knockoff.cli.command"
```

### Comparing `knockoff-4.3.2/knockoff/command/run.py` & `knockoff-4.4.0/knockoff/command/run.py`

 * *Files identical despite different names*

### Comparing `knockoff-4.3.2/knockoff/exceptions.py` & `knockoff-4.4.0/knockoff/exceptions.py`

 * *Files identical despite different names*

### Comparing `knockoff-4.3.2/knockoff/factory/assembly.py` & `knockoff-4.4.0/knockoff/factory/assembly.py`

 * *Files identical despite different names*

### Comparing `knockoff-4.3.2/knockoff/factory/component.py` & `knockoff-4.4.0/knockoff/factory/component.py`

 * *Files identical despite different names*

### Comparing `knockoff-4.3.2/knockoff/factory/counterfeit.py` & `knockoff-4.4.0/knockoff/factory/counterfeit.py`

 * *Files identical despite different names*

### Comparing `knockoff-4.3.2/knockoff/factory/node.py` & `knockoff-4.4.0/knockoff/factory/node.py`

 * *Files identical despite different names*

### Comparing `knockoff-4.3.2/knockoff/factory/part.py` & `knockoff-4.4.0/knockoff/factory/part.py`

 * *Files identical despite different names*

### Comparing `knockoff-4.3.2/knockoff/factory/prototype.py` & `knockoff-4.4.0/knockoff/factory/prototype.py`

 * *Files identical despite different names*

### Comparing `knockoff-4.3.2/knockoff/factory/sink.py` & `knockoff-4.4.0/knockoff/factory/sink.py`

 * *Files identical despite different names*

### Comparing `knockoff-4.3.2/knockoff/factory/source.py` & `knockoff-4.4.0/knockoff/factory/source.py`

 * *Files identical despite different names*

### Comparing `knockoff-4.3.2/knockoff/io.py` & `knockoff-4.4.0/knockoff/io.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,30 +1,26 @@
 # Copyright 2021-present, Nike, Inc.
 # All rights reserved.
 #
 # This source code is licensed under the Apache-2.0 license found in
 # the LICENSE file in the root directory of this source tree.
 
 
-import sys
 import logging
 import glob
 
 import pandas as pd
 import s3fs
 from pyarrow import parquet as pq
+from io import StringIO
+
+from knockoff.utilities.functools import call_with_args_kwargs
+from knockoff.utilities.mixin import ResourceLocatorMixin
+from knockoff.orm import get_connection
 
-from .utilities.functools import call_with_args_kwargs
-from .utilities.mixin import ResourceLocatorMixin
-from .orm import get_connection
-
-if sys.version_info[0] < 3:
-    from StringIO import StringIO
-else:
-    from io import StringIO
 
 logger = logging.getLogger(__name__)
 
 
 class ReaderFactory(ResourceLocatorMixin, object):
     entry_point_group = "knockoff.io.readers"
```

### Comparing `knockoff-4.3.2/knockoff/knockoff.py` & `knockoff-4.4.0/knockoff/knockoff.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,18 +6,18 @@
 
 
 from faker import Faker
 from numpy import random
 
 import yaml
 
-from . import orm
-from .factory.assembly import Blueprint, Assembler
-from .factory.node import Table, FactoryPart
-from .factory.node import FactoryComponent, FactoryPrototype
+from knockoff import orm
+from knockoff.factory.assembly import Blueprint, Assembler
+from knockoff.factory.node import Table, FactoryPart
+from knockoff.factory.node import FactoryComponent, FactoryPrototype
 
 
 class Knockoff(object):
 
     def __init__(self, path_or_config, seed=None):
 
         if isinstance(path_or_config, dict):
```

### Comparing `knockoff-4.3.2/knockoff/orm.py` & `knockoff-4.4.0/knockoff/orm.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,47 +2,46 @@
 # All rights reserved.
 #
 # This source code is licensed under the Apache-2.0 license found in
 # the LICENSE file in the root directory of this source tree.
 
 
 import pandas as pd
+
 from sqlalchemy.pool import NullPool
 
-from .utilities.orm.sql import EngineBuilder
-from .utilities.environ import clear_env_vars
+from knockoff.utilities.orm.sql import EngineBuilder
+from knockoff.utilities.environ import clear_env_vars
 
 
 KNOCKOFF_DB_URI = 'KNOCKOFF_DB_URI'
 KNOCKOFF_DB_USER = 'KNOCKOFF_DB_USER'
 KNOCKOFF_DB_PASSWORD = 'KNOCKOFF_DB_PASSWORD'
 KNOCKOFF_DB_HOST = 'KNOCKOFF_DB_HOST'
 KNOCKOFF_DB_PORT = 'KNOCKOFF_DB_PORT'
 KNOCKOFF_DB_NAME = 'KNOCKOFF_DB_NAME'
 KNOCKOFF_DB_DIALECT = 'KNOCKOFF_DB_DIALECT'
 KNOCKOFF_DB_DRIVER = 'KNOCKOFF_DB_DRIVER'
 
 
 def execute(sql, engine=None):
     engine = engine or get_engine()
-    with engine.connect() as conn:
-        conn.execute("commit")
+    with engine.begin() as conn:
         conn.execute(sql)
 
 
 def create_database(database, engine=None):
     engine = engine or get_engine()
-    execute("create database {};".format(database),
+    execute(f"create database {database};",
             engine=engine)
 
 
 def create_user(user, password, engine=None):
     engine = engine or get_engine()
-    execute("create user {} with encrypted password '{}';"
-            .format(user, password),
+    execute(f"create user {user} with encrypted password '{password}';",
             engine=engine)
 
 
 DEFAULT_BUILDER = (EngineBuilder()
                    .uri(env_var=KNOCKOFF_DB_URI)
                    .host(env_var=KNOCKOFF_DB_HOST)
                    .port(env_var=KNOCKOFF_DB_PORT)
```

### Comparing `knockoff-4.3.2/knockoff/sdk/blueprint.py` & `knockoff-4.4.0/knockoff/sdk/blueprint.py`

 * *Files identical despite different names*

### Comparing `knockoff-4.3.2/knockoff/sdk/constraints.py` & `knockoff-4.4.0/knockoff/sdk/constraints.py`

 * *Files identical despite different names*

### Comparing `knockoff-4.3.2/knockoff/sdk/container/default.py` & `knockoff-4.4.0/knockoff/sdk/container/default.py`

 * *Files identical despite different names*

### Comparing `knockoff-4.3.2/knockoff/sdk/dag.py` & `knockoff-4.4.0/knockoff/sdk/dag.py`

 * *Files identical despite different names*

### Comparing `knockoff-4.3.2/knockoff/sdk/db.py` & `knockoff-4.4.0/knockoff/sdk/db.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,16 +17,16 @@
 from sqlalchemy import create_engine
 
 from faker import Faker
 from numpy import random
 
 from knockoff.utilities.io import to_sql
 from knockoff.orm import get_engine, get_child_tables
-from .constraints import KnockoffUniqueConstraint
-from .dag import DagService, Node
+from knockoff.sdk.constraints import KnockoffUniqueConstraint
+from knockoff.sdk.dag import DagService, Node
 
 logger = logging.getLogger(__name__)
 
 
 class KnockoffDatabaseService(metaclass=ABCMeta):
 
     Schema = namedtuple("Schema", ["columns", "dtype"])
@@ -63,15 +63,15 @@
             'if_exists': 'append',
             'index': False,
             'method': 'multi'
         }
         self.kwargs.update(kwargs)
 
     def has_table(self, name):
-        engine = create_engine(self.url)
+        engine = create_engine(self.url, future=True)
         with engine.connect() as conn:
             return conn.dialect.has_table(conn, name)
 
     def _resolve_table_name_postgresql(self, name, conn):
         inspector = inspect(conn)
         try:
             inspector.get_table_oid(name)
@@ -85,30 +85,30 @@
                            "table.".format(name))
             names = get_child_tables(name, engine=self.engine)
             if names:
                 return names[0]
             raise
 
     def _resolve_table_name(self, name):
-        engine = create_engine(self.url)
+        engine = create_engine(self.url, future=True)
         with engine.connect() as conn:
             dialect = conn.dialect.name
             if dialect == postgresql.dialect.name:
                 return self._resolve_table_name_postgresql(name, conn)
             # so far there are no special cases we've had to deal with
             # for other dialects like postgresql partitioned tables
             return name
 
     def reflect_table(self, name):
         if not self.has_table(name):
             raise NoSuchTableError(name)
         meta = MetaData()
-        engine = create_engine(self.url)
+        engine = create_engine(self.url, future=True)
         with engine.connect() as conn:
-            table = Table(self._resolve_table_name(name), meta, autoload=True, autoload_with=conn)
+            table = Table(self._resolve_table_name(name), meta, autoload_with=conn)
             table.name = name  # we do this in case we needed to use the resolved child table of a partition
             return table
 
     def reflect_schema(self, name):
         table = self.reflect_table(name)
         dialect = self.engine.dialect.name
         dtype = {}
@@ -124,15 +124,15 @@
                 dtype[col.name] = col.type.python_type
         return self.Schema(columns=columns, dtype=dtype)
 
     def reflect_unique_constraints(self, name):
         if not self.has_table(name):
             raise NoSuchTableError(name)
         name = self._resolve_table_name(name)
-        engine = create_engine(self.url)
+        engine = create_engine(self.url, future=True)
         with engine.connect() as conn:
             insp = inspect(conn)
             response = insp.get_pk_constraint(name)
             constraints = [KnockoffUniqueConstraint(response['constrained_columns'],
                                                     name=response['name'])]
 
             unique_constraints = insp.get_unique_constraints(name)
@@ -210,15 +210,15 @@
     def insert(self):
         # TODO: Should we use the dfs from self.build()?
         # TODO: parallelize?
         for node in self.dag_service.iter_topologically():
             table = node.table
             table.prepare(database_service=self.database_service)
             if not node.insert:
-                _ = node.table.build() # create table needed downstream
+                _ = node.table.build()  # create table needed downstream
                 continue
             dtype = {}
             for c, t in table.dtype.items():
                 if t == dict:
                     dtype[c] = JSON
             self.database_service.insert(table.name, table.df, dtype=dtype)
```

### Comparing `knockoff-4.3.2/knockoff/sdk/factory/collections.py` & `knockoff-4.4.0/knockoff/sdk/factory/collections.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,16 +2,17 @@
 # All rights reserved.
 #
 # This source code is licensed under the Apache-2.0 license found in
 # the LICENSE file in the root directory of this source tree.
 
 
 import pandas as pd
-from .next_strategy.df import sample_df
-from .next_strategy.table import sample_table
+
+from knockoff.sdk.factory.next_strategy.df import sample_df
+from knockoff.sdk.factory.next_strategy.table import sample_table
 
 
 class CollectionsFactory(object):
     """
     CollectionsFactory is a callable that
     wraps another callable function. Similar
     to the ColumnFactory, this uses the depends_on
```

### Comparing `knockoff-4.3.2/knockoff/sdk/factory/column.py` & `knockoff-4.4.0/knockoff/sdk/factory/column.py`

 * *Files identical despite different names*

### Comparing `knockoff-4.3.2/knockoff/sdk/factory/next_strategy/df.py` & `knockoff-4.4.0/knockoff/sdk/factory/next_strategy/df.py`

 * *Files identical despite different names*

### Comparing `knockoff-4.3.2/knockoff/sdk/table.py` & `knockoff-4.4.0/knockoff/sdk/table.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,16 +12,16 @@
 from sqlalchemy import Table
 
 import pandas as pd
 
 from faker import Faker
 from knockoff.exceptions import FactoryNotFound, AttemptLimitReached
 
-from .factory.column import ColumnFactory
-from .factory.collections import CollectionsFactory
+from knockoff.sdk.factory.column import ColumnFactory
+from knockoff.sdk.factory.collections import CollectionsFactory
 
 logger = logging.getLogger(__name__)
 
 KNOCKOFF_ATTEMPT_LIMIT_ENV = "KNOCKOFF_ATTEMPT_LIMIT"
 
 
 class KnockoffTable(object):
```

### Comparing `knockoff-4.3.2/knockoff/tempdb/container.py` & `knockoff-4.4.0/knockoff/tempdb/container.py`

 * *Files identical despite different names*

### Comparing `knockoff-4.3.2/knockoff/tempdb/db.py` & `knockoff-4.4.0/knockoff/tempdb/db.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # Copyright 2021-present, Nike, Inc.
 # All rights reserved.
 #
 # This source code is licensed under the Apache-2.0 license found in
 # the LICENSE file in the root directory of this source tree.
 
-from .setup_teardown import postgres_setup_teardown
+from knockoff.tempdb.setup_teardown import postgres_setup_teardown
 
 
 class TempDatabaseService(object):
     def __init__(self,
                  url,
                  setup_teardown=postgres_setup_teardown,
                  initialize_tables=None):
```

### Comparing `knockoff-4.3.2/knockoff/tempdb/initialize_tables.py` & `knockoff-4.4.0/knockoff/tempdb/initialize_tables.py`

 * *Files identical despite different names*

### Comparing `knockoff-4.3.2/knockoff/tempdb/setup_teardown.py` & `knockoff-4.4.0/knockoff/tempdb/setup_teardown.py`

 * *Files identical despite different names*

### Comparing `knockoff-4.3.2/knockoff/utilities/date/interval.py` & `knockoff-4.4.0/knockoff/utilities/date/interval.py`

 * *Files identical despite different names*

### Comparing `knockoff-4.3.2/knockoff/utilities/environ.py` & `knockoff-4.4.0/knockoff/utilities/environ.py`

 * *Files identical despite different names*

### Comparing `knockoff-4.3.2/knockoff/utilities/importlib_utils.py` & `knockoff-4.4.0/knockoff/utilities/importlib_utils.py`

 * *Files identical despite different names*

### Comparing `knockoff-4.3.2/knockoff/utilities/io.py` & `knockoff-4.4.0/knockoff/utilities/io.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,38 +4,38 @@
 from joblib import Parallel, delayed
 
 logger = logging.getLogger(__name__)
 
 
 def _to_sql(df, table, url, **kwargs):
     to_sql_kwargs = {
-        'index': False,
-        'method': 'multi',
-        'if_exists': 'append'
+        "index": False,
+        "method": "multi",
+        "if_exists": "append"
     }
     to_sql_kwargs.update(kwargs)
     engine = create_engine(url)
     with engine.connect() as conn:
         df.to_sql(table, conn, **to_sql_kwargs)
 
 
 def to_sql(df,
            table,
            url,
            parallelize=True,
            chunksize=1000,
            n_jobs=-1,
            **kwargs):
-    logger.info("Populating table: {}".format(table))
+    logger.info("Populating table: %s" % table)
     # TODO: better default for more effect parallelization?
     nrows = df.shape[0]
     if parallelize and nrows > chunksize:
         Parallel(n_jobs=n_jobs)(
             delayed(_to_sql)(
                 df[i:i+chunksize],
                 table,
                 url,
                 **kwargs
             ) for i in range(0, nrows, chunksize))
     else:
         _to_sql(df, table, url, **kwargs)
-    logger.info("Populated table: {}".format(table))
+    logger.info("Populated table: %s" % table)
```

### Comparing `knockoff-4.3.2/knockoff/utilities/ioc.py` & `knockoff-4.4.0/knockoff/utilities/ioc.py`

 * *Files identical despite different names*

### Comparing `knockoff-4.3.2/knockoff/utilities/mixin.py` & `knockoff-4.4.0/knockoff/utilities/mixin.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 # Copyright 2021-present, Nike, Inc.
 # All rights reserved.
 #
 # This source code is licensed under the Apache-2.0 license found in
 # the LICENSE file in the root directory of this source tree.
 
 
-import pkg_resources
 import logging
 
+from importlib.metadata import entry_points
+
 from knockoff.exceptions import ResourceNotFoundError
 from knockoff.exceptions import NoEntryPointGroupError
 
 logger = logging.getLogger(__name__)
 
 
 # noinspection PyAttributeOutsideInit
@@ -34,17 +35,15 @@
         if self.entry_point_group is None:
             raise NoEntryPointGroupError(f"No entry_point declared for {self}")
         if self.registered_resources:
             logger.warning("Resources already registered. "
                            "Registering again will override "
                            "existing resources")
         self.__resources = {}
-        for entry_point in (pkg_resources
-                            .iter_entry_points(self
-                                               .entry_point_group)):
+        for entry_point in entry_points(group=self.entry_point_group):
             self.__resources[entry_point.name] = entry_point.load()
 
     def get_resource(self, name):
         self.lazy_register_resources()
         try:
             return self.__resources[name]
         except KeyError:
```

### Comparing `knockoff-4.3.2/knockoff/utilities/orm/sql.py` & `knockoff-4.4.0/knockoff/utilities/orm/sql.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,36 +1,34 @@
 # Copyright 2021-present, Nike, Inc.
 # All rights reserved.
 #
 # This source code is licensed under the Apache-2.0 license found in
 # the LICENSE file in the root directory of this source tree.
 
-from sqlalchemy import create_engine
-from sqlalchemy import Table, MetaData
+from sqlalchemy import create_engine, Table, MetaData, text
 
-from ..environ import EnvironmentVariable
+from knockoff.utilities.environ import EnvironmentVariable
 
 
 def get_table(name, engine=None, meta=None):
     engine = engine or get_engine()
-    with engine.connect() as conn:
+    with engine.begin() as conn:
         meta = meta or MetaData()
         return Table(name, meta, autoload=True, autoload_with=conn)
 
 
 def execute(sql, engine=None):
     engine = engine or get_engine()
-    with engine.connect() as conn:
-        conn.execute("commit")
-        conn.execute(sql)
+    with engine.begin() as conn:
+        conn.execute(text(sql))
 
 
 def get_engine(uri=None, **kwargs):
     uri = uri or get_uri()
-    return create_engine(uri, **kwargs)
+    return create_engine(uri, future=True, **kwargs)
 
 
 def get_uri(user="postgres",
             database="",
             password="password",
             host="localhost",
             port=5432,
```

### Comparing `knockoff-4.3.2/knockoff/utilities/orm/sqlalchemy_conn.py` & `knockoff-4.4.0/knockoff/utilities/orm/sqlalchemy_conn.py`

 * *Files 14% similar despite different names*

```diff
@@ -10,15 +10,14 @@
 
 class SqlAlchemyConn(object):
     def __init__(self, engine):
         self.engine = engine
         Session = sessionmaker(bind=self.engine)
         self.session = Session()
 
-
     def __enter__(self):
         return self
 
     def __exit__(self, exception_type, exception_value, traceback):
         if exception_type:
             self.session.rollback()
         else:
```

### Comparing `knockoff-4.3.2/knockoff/utilities/period.py` & `knockoff-4.4.0/knockoff/utilities/period.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Copyright 2021-present, Nike, Inc.
 # All rights reserved.
 #
 # This source code is licensed under the Apache-2.0 license found in
 # the LICENSE file in the root directory of this source tree.
 
 
-from .date.interval import Interval
+from knockoff.utilities.date.interval import Interval
 
 
 def generate_periods_from_intervals(bop_interval, eop_interval):
     """
 
     :param bop_interval: beginning of period interval
     :param eop_interval: end of period interval
```

### Comparing `knockoff-4.3.2/knockoff/utilities/regex.py` & `knockoff-4.4.0/knockoff/utilities/regex.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,16 +3,14 @@
 #
 # This source code is licensed under the Apache-2.0 license found in
 # the LICENSE file in the root directory of this source tree.
 
 
 from abc import ABCMeta, abstractmethod
 
-from .functools import abstractproperty2to3
-
 
 class InvalidStringError(ValueError):
     """ Raised when an invalid string is encountered """
 
     def __init__(self, string, regex):
         self.string = string
         self.regex = regex
@@ -21,15 +19,16 @@
         return ('Invalid string: {}. Regex: {}'
                 .format(repr(self.string),
                         repr(self.regex)))
 
 
 class RegexParser(metaclass=ABCMeta):
 
-    @abstractproperty2to3
+    @property
+    @abstractmethod
     def compiled_regex(self):
         raise NotImplementedError  # pragma: no cover
 
     @classmethod
     @abstractmethod
     def make(cls, **kwargs):
         return  # pragma: no cover
```

### Comparing `knockoff-4.3.2/knockoff/utilities/testing/base.py` & `knockoff-4.4.0/knockoff/utilities/testing/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,23 +23,23 @@
                  url,
                  create_db,
                  drop_db,
                  db_name=None):
         self.db_name = db_name or 'test_' + str(uuid4()).replace('-', '')
         self.create_db = create_db
         self.drop_db = drop_db
-        self.engine = create_engine(url)
+        self.engine = create_engine(url, future=True)
         create_db(self.engine, self.db_name)
 
     def url(self):
         # Substitute db name in URI with generated db
         url = re.sub(
             "(?:/[A-Za-z0-9_]+)$", "/{}".format(self.db_name), str(self.engine.url)
         )
-        engine = create_engine(url, pool=NullPool)
+        engine = create_engine(url, pool=NullPool, future=True)
         url = str(engine.url)
         return url
 
     def __enter__(self):
         return self
 
     def __exit__(self, exception_type, exception_value, traceback):
```

### Comparing `knockoff-4.3.2/knockoff/writer/pandas.py` & `knockoff-4.4.0/knockoff/writer/pandas.py`

 * *Files identical despite different names*

### Comparing `knockoff-4.3.2/pyproject.toml` & `knockoff-4.4.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "knockoff"
-version = "4.3.2"
+version = "4.4.0"
 description = "Library for generating and bootstrapping mock data"
 authors = ["Gregory Yu <gregory.yu@nike.com>"]
 readme = "README.md"
 repository = "https://github.com/Nike-Inc/knockoff-factory"
 license = "Apache-2.0"
 packages = [
   { include = "knockoff" },
@@ -12,47 +12,49 @@
 maintainers = [
   "Mohamed Abdul Huq Ismail <Abdul.Ismail@nike.com>",
   "Mark Niedzielski <Mark.Niedzielski@nike.com>"
 ]
 
 
 [tool.poetry.dependencies]
-python = "^3.7 || ^3.8"
-psycopg2 = { version = ">=2.8.4" }
-Pyrseas = { version = ">=0.9.0", optional = true }
-# Issue: https://github.com/python-poetry/poetry/issues/5121#issuecomment-1191490472
-pandas = { version = "<1.4" }
-pyaml = { version = ">=19.12.0" }
-s3fs = { version = ">=0.2.2" }
-ipython = { version = ">=5.9.0" }
-faker = { version = ">=3.0.1" }
-dotty_dict = { version = ">=1.2.1" }
-networkx = { version = ">=2.2" }
-numpy = { version = ">=1.16.6" }
-pyarrow = { version = ">=0.15.1" }
-joblib = { version = ">=0.14.1" }
-sqlalchemy-utils = { version = ">=0.32.12" }
+python = "^3.10.10"
+psycopg2 = { version = "^2.9.5" }
+Pyrseas = { version = "^0.10.0", optional = true }
+# Restrict pandas to <2.0.0 until ready for v2 upgrade.
+pandas = { version = "~1.5.3" }
+PyYaml = { version = "^6.0.0" }
+s3fs = { version = "^0.4.2" }
+ipython = { version = "^8.11" }
+faker = { version = "^18.9.0" }
+dotty_dict = { version = "^1.3.1" }
+networkx = { version = "^3.1" }
+numpy = { version = "^1.23.5" }
+pyarrow = { version = "~10.0.0" }
+joblib = { version = "^1.2.0" }
+# Restrict to <2.0.0 until databricks-sql-connector and snowflake-sqlalchemy packages
+# are compatible with SQLAlchemy>=2.0.0.
+SQLAlchemy = { version = "~1.4.48" }
+sqlalchemy-utils = { version = ">=0.41.1" }
 "testing.postgresql" = { version = ">=1.3.0" }
-dependency_injector = { version = "~4.39.0" }
-PyMySQL = { version = "~1.0.2", optional = true}
+dependency_injector = { version = "^4.41.0" }
+PyMySQL = { version = "~1.0.3", optional = true}
 
 [tool.poetry.dev-dependencies]
-pytest = { version = ">=4.6.9" }
+pytest = { version = "^7.2.2" }
 more-itertools = { version = "==5.0.0" }
-mock = { version = ">=3.0.4" }
 pytest-cov = { version = "~2.12.1" }
 jupyter = { version = "~1.0.0" }
 
 [tool.poetry.extras]
 mysql = ["PyMySQL"]
 complete = ["Pyrseas", "PyMySQL"]
 
 [build-system]
-requires = ["poetry>=1.0.0"]
-build-backend = "poetry.masonry.api"
+requires = ["poetry-core>=1.5.2"]
+build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.scripts]
 knockoff = "knockoff.cli_v2:main"
 
 [tool.poetry.plugins."knockoff.cli.command"]
 "run" = "knockoff.command.run:main"
 "version" = "knockoff.command.version:main"
```

### Comparing `knockoff-4.3.2/PKG-INFO` & `knockoff-4.4.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,41 +1,39 @@
 Metadata-Version: 2.1
 Name: knockoff
-Version: 4.3.2
+Version: 4.4.0
 Summary: Library for generating and bootstrapping mock data
 Home-page: https://github.com/Nike-Inc/knockoff-factory
 License: Apache-2.0
 Author: Gregory Yu
 Author-email: gregory.yu@nike.com
 Maintainer: Mohamed Abdul Huq Ismail
 Maintainer-email: Abdul.Ismail@nike.com
-Requires-Python: >=3.7,<4.0
+Requires-Python: >=3.10.10,<4.0.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: complete
 Provides-Extra: mysql
-Requires-Dist: PyMySQL (>=1.0.2,<1.1.0); extra == "mysql" or extra == "complete"
-Requires-Dist: Pyrseas (>=0.9.0); extra == "complete"
-Requires-Dist: dependency_injector (>=4.39.0,<4.40.0)
-Requires-Dist: dotty_dict (>=1.2.1)
-Requires-Dist: faker (>=3.0.1)
-Requires-Dist: ipython (>=5.9.0)
-Requires-Dist: joblib (>=0.14.1)
-Requires-Dist: networkx (>=2.2)
-Requires-Dist: numpy (>=1.16.6)
-Requires-Dist: pandas (<1.4)
-Requires-Dist: psycopg2 (>=2.8.4)
-Requires-Dist: pyaml (>=19.12.0)
-Requires-Dist: pyarrow (>=0.15.1)
-Requires-Dist: s3fs (>=0.2.2)
-Requires-Dist: sqlalchemy-utils (>=0.32.12)
+Requires-Dist: PyMySQL (>=1.0.3,<1.1.0) ; extra == "mysql" or extra == "complete"
+Requires-Dist: PyYaml (>=6.0.0,<7.0.0)
+Requires-Dist: Pyrseas (>=0.10.0,<0.11.0) ; extra == "complete"
+Requires-Dist: SQLAlchemy (>=1.4.48,<1.5.0)
+Requires-Dist: dependency_injector (>=4.41.0,<5.0.0)
+Requires-Dist: dotty_dict (>=1.3.1,<2.0.0)
+Requires-Dist: faker (>=18.9.0,<19.0.0)
+Requires-Dist: ipython (>=8.11,<9.0)
+Requires-Dist: joblib (>=1.2.0,<2.0.0)
+Requires-Dist: networkx (>=3.1,<4.0)
+Requires-Dist: numpy (>=1.23.5,<2.0.0)
+Requires-Dist: pandas (>=1.5.3,<1.6.0)
+Requires-Dist: psycopg2 (>=2.9.5,<3.0.0)
+Requires-Dist: pyarrow (>=10.0.0,<10.1.0)
+Requires-Dist: s3fs (>=0.4.2,<0.5.0)
+Requires-Dist: sqlalchemy-utils (>=0.41.1)
 Requires-Dist: testing.postgresql (>=1.3.0)
 Project-URL: Repository, https://github.com/Nike-Inc/knockoff-factory
 Description-Content-Type: text/markdown
 
 Knockoff Factory
 ---
 [![codecov](https://codecov.io/gh/Nike-Inc/knockoff-factory/branch/master/graph/badge.svg?token=93wOmtZxIk)](https://codecov.io/gh/Nike-Inc/knockoff-factory)
```

