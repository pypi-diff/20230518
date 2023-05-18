# Comparing `tmp/celery-redbeat-2.0.0.tar.gz` & `tmp/celery-redbeat-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/celery-redbeat-2.0.0.tar", last modified: Mon Oct 26 01:34:51 2020, max compression
+gzip compressed data, was "dist/celery-redbeat-2.1.0.tar", last modified: Thu May 18 00:47:09 2023, max compression
```

## Comparing `celery-redbeat-2.0.0.tar` & `celery-redbeat-2.1.0.tar`

### file list

```diff
@@ -1,21 +1,28 @@
-drwxr-xr-x   0 marcs      (501) staff       (20)        0 2020-10-26 01:34:51.891150 celery-redbeat-2.0.0/
--rw-r--r--   0 marcs      (501) staff       (20)     1899 2020-10-25 13:08:09.000000 celery-redbeat-2.0.0/CHANGES.txt
--rw-r--r--   0 marcs      (501) staff       (20)    11358 2019-03-06 01:10:25.000000 celery-redbeat-2.0.0/LICENSE
--rw-r--r--   0 marcs      (501) staff       (20)       78 2019-03-06 01:10:25.000000 celery-redbeat-2.0.0/MANIFEST.in
--rw-r--r--   0 marcs      (501) staff       (20)     3829 2020-10-26 01:34:51.891353 celery-redbeat-2.0.0/PKG-INFO
--rw-r--r--   0 marcs      (501) staff       (20)     2245 2020-10-15 00:37:16.000000 celery-redbeat-2.0.0/README.rst
-drwxr-xr-x   0 marcs      (501) staff       (20)        0 2020-10-26 01:34:51.888746 celery-redbeat-2.0.0/celery_redbeat.egg-info/
--rw-r--r--   0 marcs      (501) staff       (20)     3829 2020-10-26 01:34:51.000000 celery-redbeat-2.0.0/celery_redbeat.egg-info/PKG-INFO
--rw-r--r--   0 marcs      (501) staff       (20)      362 2020-10-26 01:34:51.000000 celery-redbeat-2.0.0/celery_redbeat.egg-info/SOURCES.txt
--rw-r--r--   0 marcs      (501) staff       (20)        1 2020-10-26 01:34:51.000000 celery-redbeat-2.0.0/celery_redbeat.egg-info/dependency_links.txt
--rw-r--r--   0 marcs      (501) staff       (20)       48 2020-10-26 01:34:51.000000 celery-redbeat-2.0.0/celery_redbeat.egg-info/requires.txt
--rw-r--r--   0 marcs      (501) staff       (20)        8 2020-10-26 01:34:51.000000 celery-redbeat-2.0.0/celery_redbeat.egg-info/top_level.txt
--rw-r--r--   0 marcs      (501) staff       (20)      477 2020-10-01 22:56:33.000000 celery-redbeat-2.0.0/exampleconf.py
--rw-r--r--   0 marcs      (501) staff       (20)       90 2020-10-01 22:56:33.000000 celery-redbeat-2.0.0/pyproject.toml
-drwxr-xr-x   0 marcs      (501) staff       (20)        0 2020-10-26 01:34:51.890797 celery-redbeat-2.0.0/redbeat/
--rw-r--r--   0 marcs      (501) staff       (20)      112 2019-03-06 01:10:25.000000 celery-redbeat-2.0.0/redbeat/__init__.py
--rw-r--r--   0 marcs      (501) staff       (20)     4669 2020-10-01 22:56:33.000000 celery-redbeat-2.0.0/redbeat/decoder.py
--rw-r--r--   0 marcs      (501) staff       (20)    17640 2020-10-25 13:08:59.000000 celery-redbeat-2.0.0/redbeat/schedulers.py
--rw-r--r--   0 marcs      (501) staff       (20)     3622 2020-10-01 22:56:33.000000 celery-redbeat-2.0.0/redbeat/schedules.py
--rw-r--r--   0 marcs      (501) staff       (20)      172 2020-10-26 01:34:51.892140 celery-redbeat-2.0.0/setup.cfg
--rw-r--r--   0 marcs      (501) staff       (20)     1252 2020-10-25 13:08:23.000000 celery-redbeat-2.0.0/setup.py
+drwxr-xr-x   0 marcs      (501) staff       (20)        0 2023-05-18 00:47:09.420850 celery-redbeat-2.1.0/
+-rw-r--r--   0 marcs      (501) staff       (20)     2384 2023-05-18 00:47:07.000000 celery-redbeat-2.1.0/CHANGES.txt
+-rw-r--r--   0 marcs      (501) staff       (20)    11358 2019-03-06 01:10:25.000000 celery-redbeat-2.1.0/LICENSE
+-rw-r--r--   0 marcs      (501) staff       (20)       78 2019-03-06 01:10:25.000000 celery-redbeat-2.1.0/MANIFEST.in
+-rw-r--r--   0 marcs      (501) staff       (20)     3395 2023-05-18 00:47:09.421111 celery-redbeat-2.1.0/PKG-INFO
+-rw-r--r--   0 marcs      (501) staff       (20)     2424 2023-04-29 15:07:05.000000 celery-redbeat-2.1.0/README.rst
+drwxr-xr-x   0 marcs      (501) staff       (20)        0 2023-05-18 00:47:09.407755 celery-redbeat-2.1.0/celery_redbeat.egg-info/
+-rw-r--r--   0 marcs      (501) staff       (20)     3395 2023-05-18 00:47:09.000000 celery-redbeat-2.1.0/celery_redbeat.egg-info/PKG-INFO
+-rw-r--r--   0 marcs      (501) staff       (20)      490 2023-05-18 00:47:09.000000 celery-redbeat-2.1.0/celery_redbeat.egg-info/SOURCES.txt
+-rw-r--r--   0 marcs      (501) staff       (20)        1 2023-05-18 00:47:09.000000 celery-redbeat-2.1.0/celery_redbeat.egg-info/dependency_links.txt
+-rw-r--r--   0 marcs      (501) staff       (20)       48 2023-05-18 00:47:09.000000 celery-redbeat-2.1.0/celery_redbeat.egg-info/requires.txt
+-rw-r--r--   0 marcs      (501) staff       (20)        8 2023-05-18 00:47:09.000000 celery-redbeat-2.1.0/celery_redbeat.egg-info/top_level.txt
+-rw-r--r--   0 marcs      (501) staff       (20)      477 2023-04-29 15:06:44.000000 celery-redbeat-2.1.0/exampleconf.py
+-rw-r--r--   0 marcs      (501) staff       (20)      120 2023-05-18 00:23:38.000000 celery-redbeat-2.1.0/pyproject.toml
+drwxr-xr-x   0 marcs      (501) staff       (20)        0 2023-05-18 00:47:09.412590 celery-redbeat-2.1.0/redbeat/
+-rw-r--r--   0 marcs      (501) staff       (20)       72 2023-04-29 15:06:44.000000 celery-redbeat-2.1.0/redbeat/__init__.py
+-rw-r--r--   0 marcs      (501) staff       (20)     4598 2023-04-29 15:06:44.000000 celery-redbeat-2.1.0/redbeat/decoder.py
+-rw-r--r--   0 marcs      (501) staff       (20)    18020 2023-05-03 19:24:54.000000 celery-redbeat-2.1.0/redbeat/schedulers.py
+-rw-r--r--   0 marcs      (501) staff       (20)     3593 2023-04-29 15:06:44.000000 celery-redbeat-2.1.0/redbeat/schedules.py
+-rw-r--r--   0 marcs      (501) staff       (20)      172 2023-05-18 00:47:09.422385 celery-redbeat-2.1.0/setup.cfg
+-rw-r--r--   0 marcs      (501) staff       (20)     1256 2023-05-17 23:41:44.000000 celery-redbeat-2.1.0/setup.py
+drwxr-xr-x   0 marcs      (501) staff       (20)        0 2023-05-18 00:47:09.419923 celery-redbeat-2.1.0/tests/
+-rw-r--r--   0 marcs      (501) staff       (20)     1490 2023-04-29 15:06:44.000000 celery-redbeat-2.1.0/tests/test_config.py
+-rw-r--r--   0 marcs      (501) staff       (20)     4399 2023-04-29 15:06:44.000000 celery-redbeat-2.1.0/tests/test_entry.py
+-rw-r--r--   0 marcs      (501) staff       (20)     7629 2023-04-29 15:06:44.000000 celery-redbeat-2.1.0/tests/test_json.py
+-rw-r--r--   0 marcs      (501) staff       (20)    13799 2023-04-29 15:08:53.000000 celery-redbeat-2.1.0/tests/test_scheduler.py
+-rw-r--r--   0 marcs      (501) staff       (20)     3589 2023-04-29 15:06:44.000000 celery-redbeat-2.1.0/tests/test_schedules.py
+-rw-r--r--   0 marcs      (501) staff       (20)      543 2023-04-29 15:06:44.000000 celery-redbeat-2.1.0/tests/test_utils.py
```

### Comparing `celery-redbeat-2.0.0/CHANGES.txt` & `celery-redbeat-2.1.0/CHANGES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,21 @@
+2.1.0 ()
+---------------------
+ - BREAKING, drop for support for EOL Python < 3.8
+ - log message cleanup, thanks @joekohlsdorf
+ - ensure lock is owned before releasing, fixing #223, thanks @michaelbukachi
+ - fix #238, #208, failure to aquire lock on startup leads to multiple task executions, thanks @Junzki, @nicklyra, @nigel-gott
+ - Add options support for RedBeatSchedulerEntry, thanks @anton-petrov
+
 2.0.0 (2020-10-25)
 ---------------------
   - BREAKING CHANGES, test with your stack before deploying
     - Drop support for celery<4.2
     - Drop support for pyredis<3
+    - Drop Python 2.7 and 3.5 support, update to 3.6+ syntax, thanks @kleschenko
   - Support timezones other than UTC thanks @luoxiaohei, @sempr and @noamkush
   - Many config handling consistentcy updates
   - Use black linter and drop circle CI in favor of GitHub Actions
 
 1.0.0 (2020-05-16)
 --------------------
   - version bump of 0.13.0
```

### Comparing `celery-redbeat-2.0.0/LICENSE` & `celery-redbeat-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `celery-redbeat-2.0.0/PKG-INFO` & `celery-redbeat-2.1.0/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,99 +1,103 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: celery-redbeat
-Version: 2.0.0
+Version: 2.1.0
 Summary: A Celery Beat Scheduler using Redis for persistent storage
 Home-page: https://github.com/sibson/redbeat
 Author: Marc Sibson
 Author-email: sibson+redbeat@gmail.com
 License: Apache License, Version 2.0
-Description: RedBeat
-        =======
-        
-        .. image:: https://img.shields.io/pypi/v/celery-redbeat.svg
-           :target: https://pypi.python.org/pypi/celery-redbeat
-           :alt: PyPI
-        
-        .. image:: https://github.com/sibson/redbeat/workflows/RedBeat%20CI/badge.svg
-           :target: https://github.com/sibson/redbeat/actions
-           :alt: Actions Status
-        
-        .. image:: https://readthedocs.org/projects/redbeat/badge/?version=latest&style=flat
-           :target: https://redbeat.readthedocs.io/en/latest/
-           :alt: ReadTheDocs
-        
-        .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
-           :target: https://github.com/psf/black
-           :alt: Code style: black
-        
-        `RedBeat <https://github.com/sibson/redbeat>`_ is a
-        `Celery Beat Scheduler <http://celery.readthedocs.org/en/latest/userguide/periodic-tasks.html>`_
-        that stores the scheduled tasks and runtime metadata in `Redis <http://redis.io/>`_.
-        
-        Why RedBeat?
-        -------------
-        
-        #. Dynamic live task creation and modification, without lengthy downtime
-        #. Externally manage tasks from any language with Redis bindings
-        #. Shared data store; Beat isn't tied to a single drive or machine
-        #. Fast startup even with a large task count
-        #. Prevent accidentally running multiple Beat servers
-        
-        For more background on the genesis of RedBeat see this `blog post <https://blog.heroku.com/redbeat-celery-beat-scheduler>`_
-        
-        Getting Started
-        ---------------
-        
-        Install with pip:
-        
-        .. code-block:: console
-        
-            pip install celery-redbeat
-        
-        Configure RedBeat settings in your Celery configuration file:
-        
-        .. code-block:: python
-        
-            redbeat_redis_url = "redis://localhost:6379/1"
-        
-        Then specify the scheduler when running Celery Beat:
-        
-        .. code-block:: console
-        
-            celery beat -S redbeat.RedBeatScheduler
-        
-        RedBeat uses a distributed lock to prevent multiple instances running.
-        To disable this feature, set:
-        
-        .. code-block:: python
-        
-            redbeat_lock_key = None
-        
-        More details available on `Read the Docs <https://redbeat.readthedocs.io/en/latest/>`_
-        
-        Development
-        --------------
-        RedBeat is available on `GitHub <https://github.com/sibson/redbeat>`_
-        
-        Once you have the source you can run the tests with the following commands::
-        
-            pip install -r requirements.dev.txt
-            py.test tests
-        
-        You can also quickly fire up a sample Beat instance with::
-        
-            celery beat --config exampleconf
-        
 Keywords: python,celery,beat,redis
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Topic :: System :: Distributed Computing
 Classifier: Topic :: Software Development :: Object Brokering
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 2
-Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.4
-Classifier: Programming Language :: Python :: 3.5
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Operating System :: OS Independent
+License-File: LICENSE
+
+RedBeat
+=======
+
+.. image:: https://img.shields.io/pypi/pyversions/celery-redbeat.svg
+   :target: https://pypi.python.org/pypi/celery-redbeat
+   :alt: Python Versions
+
+.. image:: https://img.shields.io/pypi/v/celery-redbeat.svg
+   :target: https://pypi.python.org/pypi/celery-redbeat
+   :alt: PyPI Package
+
+.. image:: https://github.com/sibson/redbeat/workflows/RedBeat%20CI/badge.svg
+   :target: https://github.com/sibson/redbeat/actions
+   :alt: Actions Status
+
+.. image:: https://readthedocs.org/projects/redbeat/badge/?version=latest&style=flat
+   :target: https://redbeat.readthedocs.io/en/latest/
+   :alt: ReadTheDocs
+
+.. image:: https://img.shields.io/badge/code%20style-black-000000.svg
+   :target: https://github.com/psf/black
+   :alt: Code style: black
+
+`RedBeat <https://github.com/sibson/redbeat>`_ is a
+`Celery Beat Scheduler <http://celery.readthedocs.org/en/latest/userguide/periodic-tasks.html>`_
+that stores the scheduled tasks and runtime metadata in `Redis <http://redis.io/>`_.
+
+Why RedBeat?
+-------------
+
+#. Dynamic live task creation and modification, without lengthy downtime
+#. Externally manage tasks from any language with Redis bindings
+#. Shared data store; Beat isn't tied to a single drive or machine
+#. Fast startup even with a large task count
+#. Prevent accidentally running multiple Beat servers
+
+For more background on the genesis of RedBeat see this `blog post <https://blog.heroku.com/redbeat-celery-beat-scheduler>`_
+
+Getting Started
+---------------
+
+Install with pip:
+
+.. code-block:: console
+
+    pip install celery-redbeat
+
+Configure RedBeat settings in your Celery configuration file:
+
+.. code-block:: python
+
+    redbeat_redis_url = "redis://localhost:6379/1"
+
+Then specify the scheduler when running Celery Beat:
+
+.. code-block:: console
+
+    celery beat -S redbeat.RedBeatScheduler
+
+RedBeat uses a distributed lock to prevent multiple instances running.
+To disable this feature, set:
+
+.. code-block:: python
+
+    redbeat_lock_key = None
+
+More details available on `Read the Docs <https://redbeat.readthedocs.io/en/latest/>`_
+
+Development
+--------------
+RedBeat is available on `GitHub <https://github.com/sibson/redbeat>`_
+
+Once you have the source you can run the tests with the following commands::
+
+    pip install -r requirements-dev.txt
+    python -m unittest discover tests
+
+You can also quickly fire up a sample Beat instance with::
+
+    celery beat --config exampleconf
```

### Comparing `celery-redbeat-2.0.0/README.rst` & `celery-redbeat-2.1.0/README.rst`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,17 @@
 RedBeat
 =======
 
+.. image:: https://img.shields.io/pypi/pyversions/celery-redbeat.svg
+   :target: https://pypi.python.org/pypi/celery-redbeat
+   :alt: Python Versions
+
 .. image:: https://img.shields.io/pypi/v/celery-redbeat.svg
    :target: https://pypi.python.org/pypi/celery-redbeat
-   :alt: PyPI
+   :alt: PyPI Package
 
 .. image:: https://github.com/sibson/redbeat/workflows/RedBeat%20CI/badge.svg
    :target: https://github.com/sibson/redbeat/actions
    :alt: Actions Status
 
 .. image:: https://readthedocs.org/projects/redbeat/badge/?version=latest&style=flat
    :target: https://redbeat.readthedocs.io/en/latest/
@@ -64,13 +68,13 @@
 
 Development
 --------------
 RedBeat is available on `GitHub <https://github.com/sibson/redbeat>`_
 
 Once you have the source you can run the tests with the following commands::
 
-    pip install -r requirements.dev.txt
-    py.test tests
+    pip install -r requirements-dev.txt
+    python -m unittest discover tests
 
 You can also quickly fire up a sample Beat instance with::
 
     celery beat --config exampleconf
```

### Comparing `celery-redbeat-2.0.0/celery_redbeat.egg-info/PKG-INFO` & `celery-redbeat-2.1.0/celery_redbeat.egg-info/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,99 +1,103 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: celery-redbeat
-Version: 2.0.0
+Version: 2.1.0
 Summary: A Celery Beat Scheduler using Redis for persistent storage
 Home-page: https://github.com/sibson/redbeat
 Author: Marc Sibson
 Author-email: sibson+redbeat@gmail.com
 License: Apache License, Version 2.0
-Description: RedBeat
-        =======
-        
-        .. image:: https://img.shields.io/pypi/v/celery-redbeat.svg
-           :target: https://pypi.python.org/pypi/celery-redbeat
-           :alt: PyPI
-        
-        .. image:: https://github.com/sibson/redbeat/workflows/RedBeat%20CI/badge.svg
-           :target: https://github.com/sibson/redbeat/actions
-           :alt: Actions Status
-        
-        .. image:: https://readthedocs.org/projects/redbeat/badge/?version=latest&style=flat
-           :target: https://redbeat.readthedocs.io/en/latest/
-           :alt: ReadTheDocs
-        
-        .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
-           :target: https://github.com/psf/black
-           :alt: Code style: black
-        
-        `RedBeat <https://github.com/sibson/redbeat>`_ is a
-        `Celery Beat Scheduler <http://celery.readthedocs.org/en/latest/userguide/periodic-tasks.html>`_
-        that stores the scheduled tasks and runtime metadata in `Redis <http://redis.io/>`_.
-        
-        Why RedBeat?
-        -------------
-        
-        #. Dynamic live task creation and modification, without lengthy downtime
-        #. Externally manage tasks from any language with Redis bindings
-        #. Shared data store; Beat isn't tied to a single drive or machine
-        #. Fast startup even with a large task count
-        #. Prevent accidentally running multiple Beat servers
-        
-        For more background on the genesis of RedBeat see this `blog post <https://blog.heroku.com/redbeat-celery-beat-scheduler>`_
-        
-        Getting Started
-        ---------------
-        
-        Install with pip:
-        
-        .. code-block:: console
-        
-            pip install celery-redbeat
-        
-        Configure RedBeat settings in your Celery configuration file:
-        
-        .. code-block:: python
-        
-            redbeat_redis_url = "redis://localhost:6379/1"
-        
-        Then specify the scheduler when running Celery Beat:
-        
-        .. code-block:: console
-        
-            celery beat -S redbeat.RedBeatScheduler
-        
-        RedBeat uses a distributed lock to prevent multiple instances running.
-        To disable this feature, set:
-        
-        .. code-block:: python
-        
-            redbeat_lock_key = None
-        
-        More details available on `Read the Docs <https://redbeat.readthedocs.io/en/latest/>`_
-        
-        Development
-        --------------
-        RedBeat is available on `GitHub <https://github.com/sibson/redbeat>`_
-        
-        Once you have the source you can run the tests with the following commands::
-        
-            pip install -r requirements.dev.txt
-            py.test tests
-        
-        You can also quickly fire up a sample Beat instance with::
-        
-            celery beat --config exampleconf
-        
 Keywords: python,celery,beat,redis
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Topic :: System :: Distributed Computing
 Classifier: Topic :: Software Development :: Object Brokering
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 2
-Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.4
-Classifier: Programming Language :: Python :: 3.5
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Operating System :: OS Independent
+License-File: LICENSE
+
+RedBeat
+=======
+
+.. image:: https://img.shields.io/pypi/pyversions/celery-redbeat.svg
+   :target: https://pypi.python.org/pypi/celery-redbeat
+   :alt: Python Versions
+
+.. image:: https://img.shields.io/pypi/v/celery-redbeat.svg
+   :target: https://pypi.python.org/pypi/celery-redbeat
+   :alt: PyPI Package
+
+.. image:: https://github.com/sibson/redbeat/workflows/RedBeat%20CI/badge.svg
+   :target: https://github.com/sibson/redbeat/actions
+   :alt: Actions Status
+
+.. image:: https://readthedocs.org/projects/redbeat/badge/?version=latest&style=flat
+   :target: https://redbeat.readthedocs.io/en/latest/
+   :alt: ReadTheDocs
+
+.. image:: https://img.shields.io/badge/code%20style-black-000000.svg
+   :target: https://github.com/psf/black
+   :alt: Code style: black
+
+`RedBeat <https://github.com/sibson/redbeat>`_ is a
+`Celery Beat Scheduler <http://celery.readthedocs.org/en/latest/userguide/periodic-tasks.html>`_
+that stores the scheduled tasks and runtime metadata in `Redis <http://redis.io/>`_.
+
+Why RedBeat?
+-------------
+
+#. Dynamic live task creation and modification, without lengthy downtime
+#. Externally manage tasks from any language with Redis bindings
+#. Shared data store; Beat isn't tied to a single drive or machine
+#. Fast startup even with a large task count
+#. Prevent accidentally running multiple Beat servers
+
+For more background on the genesis of RedBeat see this `blog post <https://blog.heroku.com/redbeat-celery-beat-scheduler>`_
+
+Getting Started
+---------------
+
+Install with pip:
+
+.. code-block:: console
+
+    pip install celery-redbeat
+
+Configure RedBeat settings in your Celery configuration file:
+
+.. code-block:: python
+
+    redbeat_redis_url = "redis://localhost:6379/1"
+
+Then specify the scheduler when running Celery Beat:
+
+.. code-block:: console
+
+    celery beat -S redbeat.RedBeatScheduler
+
+RedBeat uses a distributed lock to prevent multiple instances running.
+To disable this feature, set:
+
+.. code-block:: python
+
+    redbeat_lock_key = None
+
+More details available on `Read the Docs <https://redbeat.readthedocs.io/en/latest/>`_
+
+Development
+--------------
+RedBeat is available on `GitHub <https://github.com/sibson/redbeat>`_
+
+Once you have the source you can run the tests with the following commands::
+
+    pip install -r requirements-dev.txt
+    python -m unittest discover tests
+
+You can also quickly fire up a sample Beat instance with::
+
+    celery beat --config exampleconf
```

### Comparing `celery-redbeat-2.0.0/redbeat/decoder.py` & `celery-redbeat-2.1.0/redbeat/decoder.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,42 +1,40 @@
-# coding: utf-8
-
 import calendar
 import json
 from datetime import datetime
 
-from celery.schedules import schedule, crontab
-from celery.utils.time import timezone, FixedOffset
+from celery.schedules import crontab, schedule
+from celery.utils.time import FixedOffset, timezone
 from dateutil.rrule import weekday
 
 from .schedules import rrule
 
 
 def to_timestamp(dt):
-    """ convert local tz aware datetime to seconds since the epoch """
+    """convert local tz aware datetime to seconds since the epoch"""
     return calendar.timegm(dt.utctimetuple())
 
 
 def get_utcoffset_minutes(dt):
-    """ calculates timezone utc offset, returns minutes relative to utc """
+    """calculates timezone utc offset, returns minutes relative to utc"""
     utcoffset = dt.utcoffset()
 
     # Python 3: utcoffset / timedelta(minutes=1)
     return utcoffset.total_seconds() / 60 if utcoffset else 0
 
 
 def from_timestamp(seconds, tz_minutes=0):
-    """ convert seconds since the epoch to an UTC aware datetime """
+    """convert seconds since the epoch to an UTC aware datetime"""
     tz = FixedOffset(tz_minutes) if tz_minutes else timezone.utc
     return datetime.fromtimestamp(seconds, tz=tz)
 
 
 class RedBeatJSONDecoder(json.JSONDecoder):
     def __init__(self, *args, **kargs):
-        super(RedBeatJSONDecoder, self).__init__(object_hook=self.dict_to_object, *args, **kargs)
+        super().__init__(object_hook=self.dict_to_object, *args, **kargs)
 
     def dict_to_object(self, d):
         if '__type__' not in d:
             return d
 
         objtype = d.pop('__type__')
 
@@ -139,8 +137,8 @@
         if isinstance(obj, schedule):
             return {
                 '__type__': 'interval',
                 'every': obj.run_every.total_seconds(),
                 'relative': bool(obj.relative),
             }
 
-        return super(RedBeatJSONEncoder, self).default(obj)
+        return super().default(obj)
```

### Comparing `celery-redbeat-2.0.0/redbeat/schedulers.py` & `celery-redbeat-2.1.0/redbeat/schedulers.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,37 +1,32 @@
 # Licensed under the Apache License, Version 2.0 (the 'License'); you may not
 # use this file except in compliance with the License. You may obtain a copy
 # of the License at http://www.apache.org/licenses/LICENSE-2.0
 # Copyright 2015 Marc Sibson
 
-from __future__ import absolute_import
 
 import json
-import logging
-import warnings
 import ssl
-from datetime import datetime, MINYEAR
+import warnings
+from datetime import MINYEAR, datetime
 
-from celery.beat import Scheduler, ScheduleEntry, DEFAULT_MAX_INTERVAL
-from celery.utils.log import get_logger
+import redis.exceptions
+from celery.app import app_or_default
+from celery.beat import DEFAULT_MAX_INTERVAL, ScheduleEntry, Scheduler
 from celery.signals import beat_init
+from celery.utils.log import get_logger
 from celery.utils.time import humanize_seconds
 from kombu.utils.objects import cached_property
-from celery.app import app_or_default
 from kombu.utils.url import maybe_sanitize_url
-from tenacity import (
-    retry,
-    retry_if_exception_type,
-    stop_after_delay,
-    wait_exponential,
-)
-import redis.exceptions
 from redis.client import StrictRedis
+from tenacity import retry, retry_if_exception_type, stop_after_delay, wait_exponential
 
-from .decoder import RedBeatJSONEncoder, RedBeatJSONDecoder, to_timestamp
+from .decoder import RedBeatJSONDecoder, RedBeatJSONEncoder, to_timestamp
+
+logger = get_logger('celery.beat')
 
 # Copied from:
 # https://github.com/andymccurdy/redis-py/blob/master/redis/lock.py#L33
 # Changes:
 #     The second line from the bottom: The original Lua script intends
 #     to extend time to (lock remaining time + additional time); while
 #     the script here extend time to a expected expiration time.
@@ -52,15 +47,15 @@
         return 0
     end
     redis.call('pexpire', KEYS[1], ARGV[2])
     return 1
 """
 
 
-class RetryingConnection(object):
+class RetryingConnection:
     """A proxy for the Redis connection that delegates all the calls to
     underlying Redis connection while retrying on connection or time-out error.
     """
 
     RETRY_MAX_WAIT = 30
 
     def __init__(self, retry_period, wrapped_connection):
@@ -89,16 +84,16 @@
             return method(*args, **kwargs)
 
         return retrier
 
     @staticmethod
     def _log_retry_attempt(retry_state):
         """Log when next reconnection attempt is about to be made."""
-        logger.log(
-            logging.WARNING, "Retrying connection in %s seconds...", retry_state.next_action.sleep
+        logger.warning(
+            'beat: Retrying Redis connection in %s seconds...', retry_state.next_action.sleep
         )
 
 
 def ensure_conf(app):
     """
     Ensure for the given app the the redbeat_conf
     attribute is set to an instance of the RedBeatConfig
@@ -128,15 +123,17 @@
                 redis_options['sentinels'],
                 socket_timeout=redis_options.get('socket_timeout'),
                 password=redis_options.get('password'),
                 db=redis_options.get('db', 0),
                 decode_responses=True,
                 sentinel_kwargs=redis_options.get('sentinel_kwargs'),
             )
-            connection = sentinel.master_for(redis_options.get('service_name', 'master'))
+            connection = sentinel.master_for(
+                redis_options.get('service_name', 'master'), db=redis_options.get('db', 0)
+            )
         elif conf.redis_url.startswith('rediss'):
             ssl_options = {'ssl_cert_reqs': ssl.CERT_REQUIRED}
             if isinstance(conf.redis_use_ssl, dict):
                 ssl_options.update(conf.redis_use_ssl)
             connection = StrictRedis.from_url(conf.redis_url, decode_responses=True, **ssl_options)
         elif conf.redis_url.startswith('redis-cluster'):
             from rediscluster import RedisCluster
@@ -156,18 +153,16 @@
 
 
 ADD_ENTRY_ERROR = """\
 
 Couldn't add entry %r to redis schedule: %r. Contents: %r
 """
 
-logger = get_logger(__name__)
 
-
-class RedBeatConfig(object):
+class RedBeatConfig:
     def __init__(self, app=None):
         self.app = app_or_default(app)
         self.key_prefix = self.either_or('redbeat_key_prefix', 'redbeat:')
         self.schedule_key = self.key_prefix + ':schedule'
         self.statics_key = self.key_prefix + ':statics'
         self.lock_key = self.either_or('redbeat_lock_key', self.key_prefix + ':lock')
         self.lock_timeout = self.either_or('redbeat_lock_timeout', None)
@@ -195,18 +190,32 @@
         return self.app.conf.first(name, name.upper()) or default
 
 
 class RedBeatSchedulerEntry(ScheduleEntry):
     _meta = None
 
     def __init__(
-        self, name=None, task=None, schedule=None, args=None, kwargs=None, enabled=True, **clsargs
+        self,
+        name=None,
+        task=None,
+        schedule=None,
+        args=None,
+        kwargs=None,
+        enabled=True,
+        options=None,
+        **clsargs,
     ):
-        super(RedBeatSchedulerEntry, self).__init__(
-            name=name, task=task, schedule=schedule, args=args, kwargs=kwargs, **clsargs
+        super().__init__(
+            name=name,
+            task=task,
+            schedule=schedule,
+            args=args,
+            kwargs=kwargs,
+            options=options,
+            **clsargs,
         )
         self.enabled = enabled
         ensure_conf(self.app)
 
     @staticmethod
     def load_definition(key, app=None, definition=None):
         if definition is None:
@@ -274,15 +283,15 @@
 
     @property
     def key(self):
         return self.app.redbeat_conf.key_prefix + self.name
 
     @property
     def score(self):
-        """ return UTC based UNIX timestamp """
+        """return UTC based UNIX timestamp"""
         if self.due_at is None:
             # Scores < zero are ignored on each tick.
             return -1
         return to_timestamp(self.due_at)
 
     @property
     def rank(self):
@@ -312,15 +321,15 @@
     def delete(self):
         with get_redis(self.app).pipeline() as pipe:
             pipe.zrem(self.app.redbeat_conf.schedule_key, self.key)
             pipe.delete(self.key)
             pipe.execute()
 
     def _next_instance(self, last_run_at=None, only_update_last_run_at=False):
-        entry = super(RedBeatSchedulerEntry, self)._next_instance(last_run_at=last_run_at)
+        entry = super()._next_instance(last_run_at=last_run_at)
 
         if only_update_last_run_at:
             # rollback the update to total_run_count
             entry.total_run_count = self.total_run_count
 
         meta = {
             'last_run_at': entry.last_run_at,
@@ -363,31 +372,32 @@
     lock = None
 
     #: The default lock timeout in seconds.
     lock_timeout = DEFAULT_MAX_INTERVAL * 5
 
     def __init__(self, app, lock_key=None, lock_timeout=None, **kwargs):
         ensure_conf(app)  # set app.redbeat_conf
+        super(RedBeatScheduler, self).__init__(app, **kwargs)
+
         self.lock_key = lock_key or app.redbeat_conf.lock_key
         self.lock_timeout = (
             lock_timeout
             or app.redbeat_conf.lock_timeout
             or self.max_interval * 5
             or self.lock_timeout
         )
-        super(RedBeatScheduler, self).__init__(app, **kwargs)
 
     def setup_schedule(self):
         # cleanup old static schedule entries
         client = get_redis(self.app)
-        previous = set(key for key in client.smembers(self.app.redbeat_conf.statics_key))
+        previous = {key for key in client.smembers(self.app.redbeat_conf.statics_key)}
         removed = previous.difference(self.app.redbeat_conf.schedule.keys())
 
         for name in removed:
-            logger.debug("Removing old static schedule entry '%s'.", name)
+            logger.debug("beat: Removing old static schedule entry '%s'.", name)
             with client.pipeline() as pipe:
                 RedBeatSchedulerEntry(name, app=self.app).delete()
                 pipe.srem(self.app.redbeat_conf.statics_key, name)
                 pipe.execute()
 
         # setup static schedule entries
         self.install_default_entries(self.app.redbeat_conf.schedule)
@@ -403,23 +413,23 @@
             try:
                 entry = self._maybe_entry(name, entry)
             except Exception as exc:
                 logger.error(ADD_ENTRY_ERROR, name, exc, entry)
                 continue
 
             entry.save()  # store into redis
-            logger.debug("Stored entry: %s", entry)
+            logger.debug("beat: Stored entry: %s", entry)
 
     def reserve(self, entry):
         new_entry = next(entry)
         return new_entry
 
     @property
     def schedule(self):
-        logger.debug('Selecting tasks')
+        logger.debug('beat: Selecting tasks')
 
         max_due_at = to_timestamp(self.app.now())
         client = get_redis(self.app)
 
         with client.pipeline() as pipe:
             pipe.zrangebyscore(self.app.redbeat_conf.schedule_key, 0, max_due_at)
 
@@ -429,21 +439,21 @@
                 '({}'.format(max_due_at),
                 max_due_at + self.max_interval,
                 start=0,
                 num=1,
             )
             due_tasks, maybe_due = pipe.execute()
 
-        logger.debug('Loading %d tasks', len(due_tasks) + len(maybe_due))
+        logger.debug('beat: Loading %d tasks', len(due_tasks) + len(maybe_due))
         d = {}
         for key in due_tasks + maybe_due:
             try:
                 entry = self.Entry.from_key(key, app=self.app)
             except KeyError:
-                logger.warning('failed to load %s, removing', key)
+                logger.warning('beat: Failed to load %s, removing', key)
                 client.zrem(self.app.redbeat_conf.schedule_key, key)
                 continue
 
             d[entry.name] = entry
 
         return d
 
@@ -451,21 +461,21 @@
         is_due, next_time_to_run = entry.is_due()
 
         if is_due:
             logger.info('Scheduler: Sending due task %s (%s)', entry.name, entry.task)
             try:
                 result = self.apply_async(entry, **kwargs)
             except Exception as exc:
-                logger.exception('Message Error: %s', exc)
+                logger.exception('Scheduler: Message Error: %s', exc)
             else:
-                logger.debug('%s sent. id->%s', entry.task, result.id)
+                logger.debug('Scheduler: %s sent. id->%s', entry.task, result.id)
         return next_time_to_run
 
     def tick(self, min=min, **kwargs):
-        if self.lock:
+        if self.lock_key:
             logger.debug('beat: Extending lock...')
             self.lock.extend(int(self.lock_timeout))
 
         remaining_times = []
         try:
             for entry in self.schedule.values():
                 next_time_to_run = self.maybe_due(entry, **self._maybe_due_kwargs)
@@ -474,38 +484,45 @@
         except RuntimeError:
             logger.debug('beat: RuntimeError', exc_info=True)
 
         return min(remaining_times + [self.max_interval])
 
     def close(self):
         if self.lock:
-            logger.debug('beat: Releasing Lock')
-            self.lock.release()
+            logger.info('beat: Releasing lock')
+            if self.lock.owned():
+                self.lock.release()
             self.lock = None
-        super(RedBeatScheduler, self).close()
+        super().close()
 
     @property
     def info(self):
         info = ['       . redis -> {}'.format(maybe_sanitize_url(self.app.redbeat_conf.redis_url))]
         if self.lock_key:
             info.append(
                 '       . lock -> `{}` {} ({}s)'.format(
                     self.lock_key, humanize_seconds(self.lock_timeout), self.lock_timeout
                 )
             )
         return '\n'.join(info)
 
     @cached_property
     def _maybe_due_kwargs(self):
-        """ handle rename of publisher to producer """
+        """handle rename of publisher to producer"""
         return {'producer': self.producer}
 
 
 @beat_init.connect
 def acquire_distributed_beat_lock(sender=None, **kwargs):
+    """
+    Attempt to acquire lock on startup
+
+    Celery will squash any exceptions raised here. If one is raised
+    scheduler.lock will be None while scheduler.lock_key is set
+    """
     scheduler = sender.scheduler
     if not scheduler.lock_key:
         return
 
     logger.debug('beat: Acquiring lock...')
     redis_client = get_redis(scheduler.app)
 
@@ -514,9 +531,9 @@
         timeout=scheduler.lock_timeout,
         sleep=scheduler.max_interval,
     )
     # overwrite redis-py's extend script
     # which will add additional timeout instead of extend to a new timeout
     lock.lua_extend = redis_client.register_script(LUA_EXTEND_TO_SCRIPT)
     lock.acquire()
-
+    logger.info('beat: Acquired lock')
     scheduler.lock = lock
```

### Comparing `celery-redbeat-2.0.0/redbeat/schedules.py` & `celery-redbeat-2.1.0/redbeat/schedules.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,11 @@
-import celery
-from dateutil.rrule import (
-    rrule as dateutil_rrule,
-    YEARLY,
-    MONTHLY,
-    WEEKLY,
-    DAILY,
-    HOURLY,
-    MINUTELY,
-    SECONDLY,
-)
 from celery.schedules import BaseSchedule as schedule
+from celery.schedules import schedstate
+from dateutil.rrule import DAILY, HOURLY, MINUTELY, MONTHLY, SECONDLY, WEEKLY, YEARLY
+from dateutil.rrule import rrule as dateutil_rrule
 
 
 class rrule(schedule):
     RRULE_REPR = (
         '<rrule: freq: {0.freq}, dtstart: {0.dtstart}, interval: {0.interval}, '
         'wkst: {0.wkst}, count: {0.count}, until: {0.until}, bysetpos: {0.bysetpos}, '
         'bymonth: {0.bymonth}, bymonthday: {0.bymonthday}, byyearday: {0.byyearday}, '
@@ -45,17 +37,17 @@
         byyearday=None,
         byeaster=None,
         byweekno=None,
         byweekday=None,
         byhour=None,
         byminute=None,
         bysecond=None,
-        **kwargs
+        **kwargs,
     ):
-        super(rrule, self).__init__(**kwargs)
+        super().__init__(**kwargs)
 
         if type(freq) == str:
             freq_str = freq.upper()
             assert freq_str in rrule.FREQ_MAP
             freq = rrule.FREQ_MAP[freq_str]
 
         dtstart = self.maybe_make_aware(dtstart) if dtstart else self.maybe_make_aware(self.now())
@@ -113,15 +105,15 @@
             due = rem == 0
             if due:
                 rem_delta = self.remaining_estimate(self.now())
                 if rem_delta is not None:
                     rem = max(rem_delta.total_seconds(), 0)
                 else:
                     rem = None
-            return celery.schedules.schedstate(due, rem)
-        return celery.schedules.schedstate(False, None)
+            return schedstate(due, rem)
+        return schedstate(False, None)
 
     def __repr__(self):
         return self.RRULE_REPR.format(self)
 
     def __reduce__(self):
         return (self.__class__, (self.rrule), None)
```

### Comparing `celery-redbeat-2.0.0/setup.py` & `celery-redbeat-2.1.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,31 +2,31 @@
 
 long_description = open('README.rst').read()
 
 setup(
     name="celery-redbeat",
     description="A Celery Beat Scheduler using Redis for persistent storage",
     long_description=long_description,
-    version="2.0.0",
+    version="2.1.0",
     url="https://github.com/sibson/redbeat",
     license="Apache License, Version 2.0",
     author="Marc Sibson",
     author_email="sibson+redbeat@gmail.com",
     keywords="python celery beat redis".split(),
     packages=["redbeat"],
     classifiers=[
         'Development Status :: 5 - Production/Stable',
         'License :: OSI Approved :: Apache Software License',
         'Topic :: System :: Distributed Computing',
         'Topic :: Software Development :: Object Brokering',
         'Programming Language :: Python',
-        'Programming Language :: Python :: 2',
-        'Programming Language :: Python :: 2.7',
         'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.4',
-        'Programming Language :: Python :: 3.5',
+        'Programming Language :: Python :: 3.8',
+        'Programming Language :: Python :: 3.9',
+        'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
         'Programming Language :: Python :: Implementation :: CPython',
         'Operating System :: OS Independent',
     ],
-    install_requires=['redis>=3.2', 'celery>=4.2', 'python-dateutil', 'tenacity'],
+    install_requires=['redis>=3.2', 'celery>=5.0', 'python-dateutil', 'tenacity'],
     tests_require=['pytest'],
 )
```

