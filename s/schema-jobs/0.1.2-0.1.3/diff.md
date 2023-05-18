# Comparing `tmp/schema_jobs-0.1.2.tar.gz` & `tmp/schema_jobs-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "schema_jobs-0.1.2.tar", max compression
+gzip compressed data, was "schema_jobs-0.1.3.tar", max compression
```

## Comparing `schema_jobs-0.1.2.tar` & `schema_jobs-0.1.3.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0      460 2023-05-18 13:55:52.457641 schema_jobs-0.1.2/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-10 15:32:59.929513 schema_jobs-0.1.2/README.md
--rw-r--r--   0        0        0        0 2023-05-10 15:32:59.929513 schema_jobs-0.1.2/schema_jobs/__init__.py
--rw-r--r--   0        0        0        0 2023-05-16 18:07:02.358000 schema_jobs-0.1.2/schema_jobs/jobs/__init__.py
--rw-r--r--   0        0        0      192 2023-05-18 13:18:38.390862 schema_jobs-0.1.2/schema_jobs/jobs/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0        0 2023-05-16 18:07:02.358473 schema_jobs-0.1.2/schema_jobs/jobs/configuration/__init__.py
--rw-r--r--   0        0        0      184 2023-05-18 13:27:25.274846 schema_jobs-0.1.2/schema_jobs/jobs/configuration/database_configuration.py
--rw-r--r--   0        0        0      917 2023-05-16 18:03:06.305152 schema_jobs-0.1.2/schema_jobs/jobs/configuration/table_configs.py
--rw-r--r--   0        0        0        0 2023-05-16 18:07:02.358000 schema_jobs-0.1.2/schema_jobs/jobs/deploy/__init__.py
--rw-r--r--   0        0        0      600 2023-05-18 13:46:35.012146 schema_jobs-0.1.2/schema_jobs/jobs/deploy/deploy_database_tables.py
--rw-r--r--   0        0        0        0 2023-05-16 18:07:02.358000 schema_jobs-0.1.2/schema_jobs/jobs/migration/__init__.py
--rw-r--r--   0        0        0      232 2023-05-16 18:15:04.261246 schema_jobs-0.1.2/schema_jobs/jobs/migration/deploy_migration.py
--rw-r--r--   0        0        0        0 2023-05-16 18:07:02.358000 schema_jobs-0.1.2/schema_jobs/jobs/utility/__init__.py
--rw-r--r--   0        0        0      200 2023-05-18 13:18:38.408301 schema_jobs-0.1.2/schema_jobs/jobs/utility/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0        0 2023-05-16 18:07:02.358000 schema_jobs-0.1.2/schema_jobs/jobs/utility/schema/__init__.py
--rw-r--r--   0        0        0      207 2023-05-18 13:18:38.429925 schema_jobs-0.1.2/schema_jobs/jobs/utility/schema/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0      587 2023-05-18 13:18:38.438950 schema_jobs-0.1.2/schema_jobs/jobs/utility/schema/__pycache__/database.cpython-39.pyc
--rw-r--r--   0        0        0      306 2023-05-18 13:55:36.742899 schema_jobs-0.1.2/schema_jobs/jobs/utility/schema/database.py
--rw-r--r--   0        0        0       62 2023-05-16 18:12:06.405926 schema_jobs-0.1.2/schema_jobs/jobs/utility/schema/migration.py
--rw-r--r--   0        0        0     1769 2023-05-17 18:22:00.078921 schema_jobs-0.1.2/schema_jobs/jobs/utility/schema/schemas.py
--rw-r--r--   0        0        0      112 2023-05-17 18:46:35.559107 schema_jobs-0.1.2/schema_jobs/jobs/utility/schema/sql.py
--rw-r--r--   0        0        0      433 2023-05-17 18:48:28.770890 schema_jobs-0.1.2/schema_jobs/jobs/utility/schema/table.py
--rw-r--r--   0        0        0      425 1970-01-01 00:00:00.000000 schema_jobs-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0      460 2023-05-18 14:08:08.309135 schema_jobs-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-10 15:32:59.929513 schema_jobs-0.1.3/README.md
+-rw-r--r--   0        0        0        0 2023-05-10 15:32:59.929513 schema_jobs-0.1.3/schema_jobs/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-16 18:07:02.358000 schema_jobs-0.1.3/schema_jobs/jobs/__init__.py
+-rw-r--r--   0        0        0      192 2023-05-18 13:18:38.390862 schema_jobs-0.1.3/schema_jobs/jobs/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0        0 2023-05-16 18:07:02.358473 schema_jobs-0.1.3/schema_jobs/jobs/configuration/__init__.py
+-rw-r--r--   0        0        0      184 2023-05-18 13:27:25.274846 schema_jobs-0.1.3/schema_jobs/jobs/configuration/database_configuration.py
+-rw-r--r--   0        0        0      917 2023-05-16 18:03:06.305152 schema_jobs-0.1.3/schema_jobs/jobs/configuration/table_configs.py
+-rw-r--r--   0        0        0        0 2023-05-16 18:07:02.358000 schema_jobs-0.1.3/schema_jobs/jobs/deploy/__init__.py
+-rw-r--r--   0        0        0      600 2023-05-18 13:46:35.012146 schema_jobs-0.1.3/schema_jobs/jobs/deploy/deploy_database_tables.py
+-rw-r--r--   0        0        0        0 2023-05-16 18:07:02.358000 schema_jobs-0.1.3/schema_jobs/jobs/migration/__init__.py
+-rw-r--r--   0        0        0      232 2023-05-16 18:15:04.261246 schema_jobs-0.1.3/schema_jobs/jobs/migration/deploy_migration.py
+-rw-r--r--   0        0        0        0 2023-05-16 18:07:02.358000 schema_jobs-0.1.3/schema_jobs/jobs/utility/__init__.py
+-rw-r--r--   0        0        0      200 2023-05-18 13:18:38.408301 schema_jobs-0.1.3/schema_jobs/jobs/utility/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0        0 2023-05-16 18:07:02.358000 schema_jobs-0.1.3/schema_jobs/jobs/utility/schema/__init__.py
+-rw-r--r--   0        0        0      207 2023-05-18 13:18:38.429925 schema_jobs-0.1.3/schema_jobs/jobs/utility/schema/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0      587 2023-05-18 13:18:38.438950 schema_jobs-0.1.3/schema_jobs/jobs/utility/schema/__pycache__/database.cpython-39.pyc
+-rw-r--r--   0        0        0      306 2023-05-18 13:55:36.742899 schema_jobs-0.1.3/schema_jobs/jobs/utility/schema/database.py
+-rw-r--r--   0        0        0       62 2023-05-16 18:12:06.405926 schema_jobs-0.1.3/schema_jobs/jobs/utility/schema/migration.py
+-rw-r--r--   0        0        0     1769 2023-05-17 18:22:00.078921 schema_jobs-0.1.3/schema_jobs/jobs/utility/schema/schemas.py
+-rw-r--r--   0        0        0      112 2023-05-17 18:46:35.559107 schema_jobs-0.1.3/schema_jobs/jobs/utility/schema/sql.py
+-rw-r--r--   0        0        0      418 2023-05-18 14:07:50.128510 schema_jobs-0.1.3/schema_jobs/jobs/utility/schema/table.py
+-rw-r--r--   0        0        0      425 1970-01-01 00:00:00.000000 schema_jobs-0.1.3/PKG-INFO
```

### Comparing `schema_jobs-0.1.2/schema_jobs/jobs/configuration/table_configs.py` & `schema_jobs-0.1.3/schema_jobs/jobs/configuration/table_configs.py`

 * *Files identical despite different names*

### Comparing `schema_jobs-0.1.2/schema_jobs/jobs/deploy/deploy_database_tables.py` & `schema_jobs-0.1.3/schema_jobs/jobs/deploy/deploy_database_tables.py`

 * *Files identical despite different names*

### Comparing `schema_jobs-0.1.2/schema_jobs/jobs/utility/schema/__pycache__/database.cpython-39.pyc` & `schema_jobs-0.1.3/schema_jobs/jobs/utility/schema/__pycache__/database.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `schema_jobs-0.1.2/schema_jobs/jobs/utility/schema/schemas.py` & `schema_jobs-0.1.3/schema_jobs/jobs/utility/schema/schemas.py`

 * *Files identical despite different names*

