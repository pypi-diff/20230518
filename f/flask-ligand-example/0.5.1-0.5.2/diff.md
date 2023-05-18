# Comparing `tmp/flask-ligand-example-0.5.1.tar.gz` & `tmp/flask-ligand-example-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flask-ligand-example-0.5.1.tar", last modified: Fri Feb 10 21:47:00 2023, max compression
+gzip compressed data, was "flask-ligand-example-0.5.2.tar", last modified: Thu May 18 20:39:48 2023, max compression
```

## Comparing `flask-ligand-example-0.5.1.tar` & `flask-ligand-example-0.5.2.tar`

### file list

```diff
@@ -1,79 +1,79 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-10 21:47:00.364457 flask-ligand-example-0.5.1/
--rw-r--r--   0 root         (0) root         (0)       14 2023-02-10 21:46:56.000000 flask-ligand-example-0.5.1/.flaskenv
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-10 21:47:00.360457 flask-ligand-example-0.5.1/.github/
--rw-r--r--   0 root         (0) root         (0)      528 2023-02-10 21:46:56.000000 flask-ligand-example-0.5.1/.github/dependabot.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-10 21:47:00.360457 flask-ligand-example-0.5.1/.github/workflows/
--rw-r--r--   0 root         (0) root         (0)      625 2023-02-10 21:46:56.000000 flask-ligand-example-0.5.1/.github/workflows/bump_and_publish_release.yml
--rw-r--r--   0 root         (0) root         (0)      797 2023-02-10 21:46:56.000000 flask-ligand-example-0.5.1/.github/workflows/coverage.yml
--rw-r--r--   0 root         (0) root         (0)      622 2023-02-10 21:46:56.000000 flask-ligand-example-0.5.1/.github/workflows/pull_request.yml
--rw-r--r--   0 root         (0) root         (0)      983 2023-02-10 21:46:56.000000 flask-ligand-example-0.5.1/.pre-commit-config.yaml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-10 21:47:00.360457 flask-ligand-example-0.5.1/.run/
--rw-r--r--   0 root         (0) root         (0)     1338 2023-02-10 21:46:56.000000 flask-ligand-example-0.5.1/.run/Flask - Debug.run.xml
--rw-r--r--   0 root         (0) root         (0)     1307 2023-02-10 21:46:56.000000 flask-ligand-example-0.5.1/.run/Flask.run.xml
--rw-r--r--   0 root         (0) root         (0)      459 2023-02-10 21:46:56.000000 flask-ligand-example-0.5.1/.run/Integration Test Environment.run.xml
--rw-r--r--   0 root         (0) root         (0)     1493 2023-02-10 21:46:56.000000 flask-ligand-example-0.5.1/.run/Integration.run.xml
--rw-r--r--   0 root         (0) root         (0)     1267 2023-02-10 21:46:56.000000 flask-ligand-example-0.5.1/.run/Unit (tox).run.xml
--rw-r--r--   0 root         (0) root         (0)     1315 2023-02-10 21:46:56.000000 flask-ligand-example-0.5.1/.run/Unit (tox-fast).run.xml
--rw-r--r--   0 root         (0) root         (0)     1479 2023-02-10 21:46:56.000000 flask-ligand-example-0.5.1/.run/Unit.run.xml
--rw-r--r--   0 root         (0) root         (0)      369 2023-02-10 21:46:56.000000 flask-ligand-example-0.5.1/.run/develop-venv.run.xml
--rw-r--r--   0 root         (0) root         (0)      389 2023-02-10 21:46:56.000000 flask-ligand-example-0.5.1/.run/gen-admin-access-token.run.xml
--rw-r--r--   0 root         (0) root         (0)      361 2023-02-10 21:46:56.000000 flask-ligand-example-0.5.1/.run/setup-db.run.xml
--rw-r--r--   0 root         (0) root         (0)      361 2023-02-10 21:46:56.000000 flask-ligand-example-0.5.1/.run/test-all.run.xml
--rw-r--r--   0 root         (0) root         (0)       36 2023-02-10 21:46:56.000000 flask-ligand-example-0.5.1/AUTHORS
--rw-r--r--   0 root         (0) root         (0)     7392 2023-02-10 21:46:56.000000 flask-ligand-example-0.5.1/CHANGELOG.md
--rw-r--r--   0 root         (0) root         (0)     3603 2023-02-10 21:46:56.000000 flask-ligand-example-0.5.1/CONTRIBUTING.rst
--rw-r--r--   0 root         (0) root         (0)    34523 2023-02-10 21:46:56.000000 flask-ligand-example-0.5.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     8836 2023-02-10 21:46:56.000000 flask-ligand-example-0.5.1/Makefile
--rw-r--r--   0 root         (0) root         (0)     6216 2023-02-10 21:47:00.364457 flask-ligand-example-0.5.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4923 2023-02-10 21:46:56.000000 flask-ligand-example-0.5.1/README.rst
--rw-r--r--   0 root         (0) root         (0)      936 2023-02-10 21:46:56.000000 flask-ligand-example-0.5.1/app.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-10 21:47:00.356457 flask-ligand-example-0.5.1/docker/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-10 21:47:00.360457 flask-ligand-example-0.5.1/docker/env_files/
--rw-r--r--   0 root         (0) root         (0)      843 2023-02-10 21:46:56.000000 flask-ligand-example-0.5.1/docker/env_files/integration.env
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-10 21:47:00.360457 flask-ligand-example-0.5.1/docker/kc-data/
--rw-r--r--   0 root         (0) root         (0)    78994 2023-02-10 21:46:56.000000 flask-ligand-example-0.5.1/docker/kc-data/flask-ligand-realm.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-10 21:47:00.360457 flask-ligand-example-0.5.1/docker/postgres-data/
--rw-r--r--   0 root         (0) root         (0)      589 2023-02-10 21:46:56.000000 flask-ligand-example-0.5.1/docker/postgres-data/create-multiple-postgresql-databases.sh
--rw-r--r--   0 root         (0) root         (0)     1086 2023-02-10 21:46:56.000000 flask-ligand-example-0.5.1/docker-compose.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-10 21:47:00.360457 flask-ligand-example-0.5.1/flask_ligand_example/
--rw-r--r--   0 root         (0) root         (0)     2630 2023-02-10 21:46:56.000000 flask-ligand-example-0.5.1/flask_ligand_example/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1461 2023-02-10 21:46:56.000000 flask-ligand-example-0.5.1/flask_ligand_example/models.py
--rw-r--r--   0 root         (0) root         (0)     1831 2023-02-10 21:46:56.000000 flask-ligand-example-0.5.1/flask_ligand_example/schemas.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-10 21:47:00.364457 flask-ligand-example-0.5.1/flask_ligand_example/views/
--rw-r--r--   0 root         (0) root         (0)     1556 2023-02-10 21:46:56.000000 flask-ligand-example-0.5.1/flask_ligand_example/views/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4414 2023-02-10 21:46:56.000000 flask-ligand-example-0.5.1/flask_ligand_example/views/pet.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-10 21:47:00.364457 flask-ligand-example-0.5.1/flask_ligand_example.egg-info/
--rw-r--r--   0 root         (0) root         (0)     6216 2023-02-10 21:47:00.000000 flask-ligand-example-0.5.1/flask_ligand_example.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1634 2023-02-10 21:47:00.000000 flask-ligand-example-0.5.1/flask_ligand_example.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-02-10 21:47:00.000000 flask-ligand-example-0.5.1/flask_ligand_example.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-02-10 21:47:00.000000 flask-ligand-example-0.5.1/flask_ligand_example.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       46 2023-02-10 21:47:00.000000 flask-ligand-example-0.5.1/flask_ligand_example.egg-info/pbr.json
--rw-r--r--   0 root         (0) root         (0)       18 2023-02-10 21:47:00.000000 flask-ligand-example-0.5.1/flask_ligand_example.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       21 2023-02-10 21:47:00.000000 flask-ligand-example-0.5.1/flask_ligand_example.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-10 21:47:00.364457 flask-ligand-example-0.5.1/migrations/
--rw-r--r--   0 root         (0) root         (0)       41 2023-02-10 21:46:56.000000 flask-ligand-example-0.5.1/migrations/README
--rw-r--r--   0 root         (0) root         (0)      991 2023-02-10 21:46:56.000000 flask-ligand-example-0.5.1/migrations/alembic.ini
--rw-r--r--   0 root         (0) root         (0)     2751 2023-02-10 21:46:56.000000 flask-ligand-example-0.5.1/migrations/env.py
--rw-r--r--   0 root         (0) root         (0)      533 2023-02-10 21:46:56.000000 flask-ligand-example-0.5.1/migrations/script.py.mako
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-10 21:47:00.364457 flask-ligand-example-0.5.1/migrations/versions/
--rw-r--r--   0 root         (0) root         (0)     1010 2023-02-10 21:46:56.000000 flask-ligand-example-0.5.1/migrations/versions/8017390d7666_initial_migration.py
--rw-r--r--   0 root         (0) root         (0)      997 2023-02-10 21:46:56.000000 flask-ligand-example-0.5.1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)      467 2023-02-10 21:46:56.000000 flask-ligand-example-0.5.1/requirements-dev.txt
--rw-r--r--   0 root         (0) root         (0)       18 2023-02-10 21:46:56.000000 flask-ligand-example-0.5.1/requirements.txt
--rw-r--r--   0 root         (0) root         (0)     1373 2023-02-10 21:47:00.364457 flask-ligand-example-0.5.1/setup.cfg
--rwxr-xr-x   0 root         (0) root         (0)      737 2023-02-10 21:46:56.000000 flask-ligand-example-0.5.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-10 21:47:00.364457 flask-ligand-example-0.5.1/tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-02-10 21:46:56.000000 flask-ligand-example-0.5.1/tests/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-10 21:47:00.364457 flask-ligand-example-0.5.1/tests/common/
--rw-r--r--   0 root         (0) root         (0)        0 2023-02-10 21:46:56.000000 flask-ligand-example-0.5.1/tests/common/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1967 2023-02-10 21:46:56.000000 flask-ligand-example-0.5.1/tests/common/fixtures.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-10 21:47:00.364457 flask-ligand-example-0.5.1/tests/integration/
--rw-r--r--   0 root         (0) root         (0)        0 2023-02-10 21:46:56.000000 flask-ligand-example-0.5.1/tests/integration/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6493 2023-02-10 21:46:56.000000 flask-ligand-example-0.5.1/tests/integration/conftest.py
--rw-r--r--   0 root         (0) root         (0)     7974 2023-02-10 21:46:56.000000 flask-ligand-example-0.5.1/tests/integration/test_basic.py
--rw-r--r--   0 root         (0) root         (0)     1768 2023-02-10 21:46:56.000000 flask-ligand-example-0.5.1/tests/integration/test_cli.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-10 21:47:00.364457 flask-ligand-example-0.5.1/tests/unit/
--rw-r--r--   0 root         (0) root         (0)        0 2023-02-10 21:46:56.000000 flask-ligand-example-0.5.1/tests/unit/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3995 2023-02-10 21:46:56.000000 flask-ligand-example-0.5.1/tests/unit/conftest.py
--rw-r--r--   0 root         (0) root         (0)    22586 2023-02-10 21:46:56.000000 flask-ligand-example-0.5.1/tests/unit/test_basic.py
--rw-r--r--   0 root         (0) root         (0)      369 2023-02-10 21:46:56.000000 flask-ligand-example-0.5.1/tox.ini
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 20:39:48.025022 flask-ligand-example-0.5.2/
+-rw-r--r--   0 root         (0) root         (0)       14 2023-05-18 20:39:43.000000 flask-ligand-example-0.5.2/.flaskenv
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 20:39:48.013022 flask-ligand-example-0.5.2/.github/
+-rw-r--r--   0 root         (0) root         (0)      528 2023-05-18 20:39:43.000000 flask-ligand-example-0.5.2/.github/dependabot.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 20:39:48.013022 flask-ligand-example-0.5.2/.github/workflows/
+-rw-r--r--   0 root         (0) root         (0)      625 2023-05-18 20:39:43.000000 flask-ligand-example-0.5.2/.github/workflows/bump_and_publish_release.yml
+-rw-r--r--   0 root         (0) root         (0)      797 2023-05-18 20:39:43.000000 flask-ligand-example-0.5.2/.github/workflows/coverage.yml
+-rw-r--r--   0 root         (0) root         (0)      622 2023-05-18 20:39:43.000000 flask-ligand-example-0.5.2/.github/workflows/pull_request.yml
+-rw-r--r--   0 root         (0) root         (0)     1014 2023-05-18 20:39:43.000000 flask-ligand-example-0.5.2/.pre-commit-config.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 20:39:48.017022 flask-ligand-example-0.5.2/.run/
+-rw-r--r--   0 root         (0) root         (0)     1338 2023-05-18 20:39:43.000000 flask-ligand-example-0.5.2/.run/Flask - Debug.run.xml
+-rw-r--r--   0 root         (0) root         (0)     1307 2023-05-18 20:39:43.000000 flask-ligand-example-0.5.2/.run/Flask.run.xml
+-rw-r--r--   0 root         (0) root         (0)      459 2023-05-18 20:39:43.000000 flask-ligand-example-0.5.2/.run/Integration Test Environment.run.xml
+-rw-r--r--   0 root         (0) root         (0)     1493 2023-05-18 20:39:43.000000 flask-ligand-example-0.5.2/.run/Integration.run.xml
+-rw-r--r--   0 root         (0) root         (0)     1267 2023-05-18 20:39:43.000000 flask-ligand-example-0.5.2/.run/Unit (tox).run.xml
+-rw-r--r--   0 root         (0) root         (0)     1315 2023-05-18 20:39:43.000000 flask-ligand-example-0.5.2/.run/Unit (tox-fast).run.xml
+-rw-r--r--   0 root         (0) root         (0)     1479 2023-05-18 20:39:43.000000 flask-ligand-example-0.5.2/.run/Unit.run.xml
+-rw-r--r--   0 root         (0) root         (0)      369 2023-05-18 20:39:43.000000 flask-ligand-example-0.5.2/.run/develop-venv.run.xml
+-rw-r--r--   0 root         (0) root         (0)      389 2023-05-18 20:39:43.000000 flask-ligand-example-0.5.2/.run/gen-admin-access-token.run.xml
+-rw-r--r--   0 root         (0) root         (0)      361 2023-05-18 20:39:43.000000 flask-ligand-example-0.5.2/.run/setup-db.run.xml
+-rw-r--r--   0 root         (0) root         (0)      361 2023-05-18 20:39:43.000000 flask-ligand-example-0.5.2/.run/test-all.run.xml
+-rw-r--r--   0 root         (0) root         (0)       36 2023-05-18 20:39:43.000000 flask-ligand-example-0.5.2/AUTHORS
+-rw-r--r--   0 root         (0) root         (0)    12574 2023-05-18 20:39:44.000000 flask-ligand-example-0.5.2/CHANGELOG.md
+-rw-r--r--   0 root         (0) root         (0)     3603 2023-05-18 20:39:43.000000 flask-ligand-example-0.5.2/CONTRIBUTING.rst
+-rw-r--r--   0 root         (0) root         (0)    34523 2023-05-18 20:39:43.000000 flask-ligand-example-0.5.2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     8836 2023-05-18 20:39:43.000000 flask-ligand-example-0.5.2/Makefile
+-rw-r--r--   0 root         (0) root         (0)     6216 2023-05-18 20:39:48.025022 flask-ligand-example-0.5.2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4923 2023-05-18 20:39:43.000000 flask-ligand-example-0.5.2/README.rst
+-rw-r--r--   0 root         (0) root         (0)      936 2023-05-18 20:39:43.000000 flask-ligand-example-0.5.2/app.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 20:39:48.009022 flask-ligand-example-0.5.2/docker/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 20:39:48.017022 flask-ligand-example-0.5.2/docker/env_files/
+-rw-r--r--   0 root         (0) root         (0)      843 2023-05-18 20:39:43.000000 flask-ligand-example-0.5.2/docker/env_files/integration.env
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 20:39:48.017022 flask-ligand-example-0.5.2/docker/kc-data/
+-rw-r--r--   0 root         (0) root         (0)    78994 2023-05-18 20:39:43.000000 flask-ligand-example-0.5.2/docker/kc-data/flask-ligand-realm.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 20:39:48.017022 flask-ligand-example-0.5.2/docker/postgres-data/
+-rw-r--r--   0 root         (0) root         (0)      589 2023-05-18 20:39:43.000000 flask-ligand-example-0.5.2/docker/postgres-data/create-multiple-postgresql-databases.sh
+-rw-r--r--   0 root         (0) root         (0)     1086 2023-05-18 20:39:43.000000 flask-ligand-example-0.5.2/docker-compose.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 20:39:48.017022 flask-ligand-example-0.5.2/flask_ligand_example/
+-rw-r--r--   0 root         (0) root         (0)     2630 2023-05-18 20:39:44.000000 flask-ligand-example-0.5.2/flask_ligand_example/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1461 2023-05-18 20:39:43.000000 flask-ligand-example-0.5.2/flask_ligand_example/models.py
+-rw-r--r--   0 root         (0) root         (0)     1831 2023-05-18 20:39:43.000000 flask-ligand-example-0.5.2/flask_ligand_example/schemas.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 20:39:48.021022 flask-ligand-example-0.5.2/flask_ligand_example/views/
+-rw-r--r--   0 root         (0) root         (0)     1556 2023-05-18 20:39:43.000000 flask-ligand-example-0.5.2/flask_ligand_example/views/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4414 2023-05-18 20:39:43.000000 flask-ligand-example-0.5.2/flask_ligand_example/views/pet.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 20:39:48.021022 flask-ligand-example-0.5.2/flask_ligand_example.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     6216 2023-05-18 20:39:47.000000 flask-ligand-example-0.5.2/flask_ligand_example.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1634 2023-05-18 20:39:48.000000 flask-ligand-example-0.5.2/flask_ligand_example.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-18 20:39:47.000000 flask-ligand-example-0.5.2/flask_ligand_example.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-18 20:39:47.000000 flask-ligand-example-0.5.2/flask_ligand_example.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       46 2023-05-18 20:39:47.000000 flask-ligand-example-0.5.2/flask_ligand_example.egg-info/pbr.json
+-rw-r--r--   0 root         (0) root         (0)       20 2023-05-18 20:39:47.000000 flask-ligand-example-0.5.2/flask_ligand_example.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       21 2023-05-18 20:39:47.000000 flask-ligand-example-0.5.2/flask_ligand_example.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 20:39:48.021022 flask-ligand-example-0.5.2/migrations/
+-rw-r--r--   0 root         (0) root         (0)       41 2023-05-18 20:39:43.000000 flask-ligand-example-0.5.2/migrations/README
+-rw-r--r--   0 root         (0) root         (0)      991 2023-05-18 20:39:43.000000 flask-ligand-example-0.5.2/migrations/alembic.ini
+-rw-r--r--   0 root         (0) root         (0)     2751 2023-05-18 20:39:43.000000 flask-ligand-example-0.5.2/migrations/env.py
+-rw-r--r--   0 root         (0) root         (0)      533 2023-05-18 20:39:43.000000 flask-ligand-example-0.5.2/migrations/script.py.mako
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 20:39:48.021022 flask-ligand-example-0.5.2/migrations/versions/
+-rw-r--r--   0 root         (0) root         (0)     1010 2023-05-18 20:39:43.000000 flask-ligand-example-0.5.2/migrations/versions/8017390d7666_initial_migration.py
+-rw-r--r--   0 root         (0) root         (0)      997 2023-05-18 20:39:43.000000 flask-ligand-example-0.5.2/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)      465 2023-05-18 20:39:43.000000 flask-ligand-example-0.5.2/requirements-dev.txt
+-rw-r--r--   0 root         (0) root         (0)       20 2023-05-18 20:39:43.000000 flask-ligand-example-0.5.2/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)     1373 2023-05-18 20:39:48.029022 flask-ligand-example-0.5.2/setup.cfg
+-rwxr-xr-x   0 root         (0) root         (0)      737 2023-05-18 20:39:43.000000 flask-ligand-example-0.5.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 20:39:48.021022 flask-ligand-example-0.5.2/tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 20:39:43.000000 flask-ligand-example-0.5.2/tests/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 20:39:48.025022 flask-ligand-example-0.5.2/tests/common/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 20:39:43.000000 flask-ligand-example-0.5.2/tests/common/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1967 2023-05-18 20:39:43.000000 flask-ligand-example-0.5.2/tests/common/fixtures.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 20:39:48.025022 flask-ligand-example-0.5.2/tests/integration/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 20:39:43.000000 flask-ligand-example-0.5.2/tests/integration/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6493 2023-05-18 20:39:43.000000 flask-ligand-example-0.5.2/tests/integration/conftest.py
+-rw-r--r--   0 root         (0) root         (0)     7974 2023-05-18 20:39:43.000000 flask-ligand-example-0.5.2/tests/integration/test_basic.py
+-rw-r--r--   0 root         (0) root         (0)     1768 2023-05-18 20:39:43.000000 flask-ligand-example-0.5.2/tests/integration/test_cli.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 20:39:48.025022 flask-ligand-example-0.5.2/tests/unit/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 20:39:43.000000 flask-ligand-example-0.5.2/tests/unit/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3995 2023-05-18 20:39:43.000000 flask-ligand-example-0.5.2/tests/unit/conftest.py
+-rw-r--r--   0 root         (0) root         (0)    22586 2023-05-18 20:39:43.000000 flask-ligand-example-0.5.2/tests/unit/test_basic.py
+-rw-r--r--   0 root         (0) root         (0)      369 2023-05-18 20:39:43.000000 flask-ligand-example-0.5.2/tox.ini
```

### Comparing `flask-ligand-example-0.5.1/.github/dependabot.yml` & `flask-ligand-example-0.5.2/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `flask-ligand-example-0.5.1/.github/workflows/bump_and_publish_release.yml` & `flask-ligand-example-0.5.2/.github/workflows/bump_and_publish_release.yml`

 * *Files identical despite different names*

### Comparing `flask-ligand-example-0.5.1/.github/workflows/coverage.yml` & `flask-ligand-example-0.5.2/.github/workflows/coverage.yml`

 * *Files identical despite different names*

### Comparing `flask-ligand-example-0.5.1/.github/workflows/pull_request.yml` & `flask-ligand-example-0.5.2/.github/workflows/pull_request.yml`

 * *Files identical despite different names*

### Comparing `flask-ligand-example-0.5.1/.pre-commit-config.yaml` & `flask-ligand-example-0.5.2/.pre-commit-config.yaml`

 * *Files 9% similar despite different names*

```diff
@@ -4,33 +4,34 @@
     hooks:
     -   id: check-yaml
     -   id: check-toml
     -   id: detect-private-key
     -   id: end-of-file-fixer
     -   id: trailing-whitespace
 -   repo: https://github.com/psf/black
-    rev: 22.12.0
+    rev: 23.3.0
     hooks:
     -   id: black
 -   repo: https://github.com/PyCQA/flake8
     rev: 6.0.0
     hooks:
     -   id: flake8
 -   repo: https://github.com/pre-commit/mirrors-mypy
-    rev: v0.991
+    rev: v1.3.0
     hooks:
     -   id: mypy
         additional_dependencies:
+        -   "flask-ligand~=0.7"
         -   "types-Flask-Cors~=3.0"
         -   "types-Flask-SQLAlchemy~=2.5"
-        -   "types-mock~=4.0"
+        -   "types-mock~=5.0"
         -   "types-PyYAML~=6.0"
         -   "types-requests~=2.28"
-        -   "types-setuptools~=63.4"
+        -   "types-setuptools~=67.5"
         -   "types-smorest~=1.1"
         -   "types-SQLAlchemy~=1.4"
         -   "types-sqlalchemy-utils~=1.0"
         -   "types-urllib3<1.27"
 -   repo: https://github.com/rstcheck/rstcheck
-    rev: v6.1.1
+    rev: v6.1.2
     hooks:
     -   id: rstcheck
```

### Comparing `flask-ligand-example-0.5.1/.run/Flask - Debug.run.xml` & `flask-ligand-example-0.5.2/.run/Flask - Debug.run.xml`

 * *Files identical despite different names*

### Comparing `flask-ligand-example-0.5.1/.run/Flask.run.xml` & `flask-ligand-example-0.5.2/.run/Flask.run.xml`

 * *Files identical despite different names*

### Comparing `flask-ligand-example-0.5.1/.run/Integration.run.xml` & `flask-ligand-example-0.5.2/.run/Integration.run.xml`

 * *Files identical despite different names*

### Comparing `flask-ligand-example-0.5.1/.run/Unit (tox).run.xml` & `flask-ligand-example-0.5.2/.run/Unit (tox).run.xml`

 * *Files identical despite different names*

### Comparing `flask-ligand-example-0.5.1/.run/Unit (tox-fast).run.xml` & `flask-ligand-example-0.5.2/.run/Unit (tox-fast).run.xml`

 * *Files identical despite different names*

### Comparing `flask-ligand-example-0.5.1/.run/Unit.run.xml` & `flask-ligand-example-0.5.2/.run/Unit.run.xml`

 * *Files identical despite different names*

### Comparing `flask-ligand-example-0.5.1/CONTRIBUTING.rst` & `flask-ligand-example-0.5.2/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `flask-ligand-example-0.5.1/LICENSE` & `flask-ligand-example-0.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `flask-ligand-example-0.5.1/Makefile` & `flask-ligand-example-0.5.2/Makefile`

 * *Files identical despite different names*

### Comparing `flask-ligand-example-0.5.1/PKG-INFO` & `flask-ligand-example-0.5.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flask-ligand-example
-Version: 0.5.1
+Version: 0.5.2
 Summary: A simple example project on how to use the flask-ligand library.
 Author: Ryan Gard
 Author-email: ryan@gardiancapitol.com
 License: GNU Affero General Public License v3
 Project-URL: Changelog, https://github.com/cowofevil/flask-ligand-example/blob/main/CHANGELOG.md
 Project-URL: Source, https://github.com/cowofevil/flask-ligand-example
 Project-URL: Tracker, https://github.com/cowofevil/flask-ligand-example/issues
```

### Comparing `flask-ligand-example-0.5.1/README.rst` & `flask-ligand-example-0.5.2/README.rst`

 * *Files identical despite different names*

### Comparing `flask-ligand-example-0.5.1/app.py` & `flask-ligand-example-0.5.2/app.py`

 * *Files identical despite different names*

### Comparing `flask-ligand-example-0.5.1/docker/env_files/integration.env` & `flask-ligand-example-0.5.2/docker/env_files/integration.env`

 * *Files identical despite different names*

### Comparing `flask-ligand-example-0.5.1/docker/kc-data/flask-ligand-realm.json` & `flask-ligand-example-0.5.2/docker/kc-data/flask-ligand-realm.json`

 * *Files identical despite different names*

### Comparing `flask-ligand-example-0.5.1/docker/postgres-data/create-multiple-postgresql-databases.sh` & `flask-ligand-example-0.5.2/docker/postgres-data/create-multiple-postgresql-databases.sh`

 * *Files identical despite different names*

### Comparing `flask-ligand-example-0.5.1/docker-compose.yml` & `flask-ligand-example-0.5.2/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `flask-ligand-example-0.5.1/flask_ligand_example/__init__.py` & `flask-ligand-example-0.5.2/flask_ligand_example/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 if TYPE_CHECKING:  # pragma: no cover
     from typing import Any
 
 
 # ======================================================================================================================
 # Globals
 # ======================================================================================================================
-__version__ = "0.5.1"
+__version__ = "0.5.2"
 
 
 # ======================================================================================================================
 # Functions: Public
 # ======================================================================================================================
 def create_app(flask_env: str, api_title: str, api_version: str, openapi_client_name: str, **kwargs: Any) -> Flask:
     """
```

### Comparing `flask-ligand-example-0.5.1/flask_ligand_example/models.py` & `flask-ligand-example-0.5.2/flask_ligand_example/models.py`

 * *Files identical despite different names*

### Comparing `flask-ligand-example-0.5.1/flask_ligand_example/schemas.py` & `flask-ligand-example-0.5.2/flask_ligand_example/schemas.py`

 * *Files identical despite different names*

### Comparing `flask-ligand-example-0.5.1/flask_ligand_example/views/__init__.py` & `flask-ligand-example-0.5.2/flask_ligand_example/views/__init__.py`

 * *Files identical despite different names*

### Comparing `flask-ligand-example-0.5.1/flask_ligand_example/views/pet.py` & `flask-ligand-example-0.5.2/flask_ligand_example/views/pet.py`

 * *Files identical despite different names*

### Comparing `flask-ligand-example-0.5.1/flask_ligand_example.egg-info/PKG-INFO` & `flask-ligand-example-0.5.2/flask_ligand_example.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flask-ligand-example
-Version: 0.5.1
+Version: 0.5.2
 Summary: A simple example project on how to use the flask-ligand library.
 Author: Ryan Gard
 Author-email: ryan@gardiancapitol.com
 License: GNU Affero General Public License v3
 Project-URL: Changelog, https://github.com/cowofevil/flask-ligand-example/blob/main/CHANGELOG.md
 Project-URL: Source, https://github.com/cowofevil/flask-ligand-example
 Project-URL: Tracker, https://github.com/cowofevil/flask-ligand-example/issues
```

### Comparing `flask-ligand-example-0.5.1/flask_ligand_example.egg-info/SOURCES.txt` & `flask-ligand-example-0.5.2/flask_ligand_example.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `flask-ligand-example-0.5.1/migrations/alembic.ini` & `flask-ligand-example-0.5.2/migrations/alembic.ini`

 * *Files identical despite different names*

### Comparing `flask-ligand-example-0.5.1/migrations/env.py` & `flask-ligand-example-0.5.2/migrations/env.py`

 * *Files identical despite different names*

### Comparing `flask-ligand-example-0.5.1/migrations/script.py.mako` & `flask-ligand-example-0.5.2/migrations/script.py.mako`

 * *Files identical despite different names*

### Comparing `flask-ligand-example-0.5.1/migrations/versions/8017390d7666_initial_migration.py` & `flask-ligand-example-0.5.2/migrations/versions/8017390d7666_initial_migration.py`

 * *Files identical despite different names*

### Comparing `flask-ligand-example-0.5.1/pyproject.toml` & `flask-ligand-example-0.5.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `flask-ligand-example-0.5.1/setup.cfg` & `flask-ligand-example-0.5.2/setup.cfg`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = flask-ligand-example
-version = 0.5.1
+version = 0.5.2
 summary = A simple example project on how to use the flask-ligand library.
 description_file = README.rst
 description_content_type = text/x-rst; charset=UTF-8
 author = Ryan Gard
 author_email = ryan@gardiancapitol.com
 keywords = flask
 license = GNU Affero General Public License v3
```

### Comparing `flask-ligand-example-0.5.1/setup.py` & `flask-ligand-example-0.5.2/setup.py`

 * *Files identical despite different names*

### Comparing `flask-ligand-example-0.5.1/tests/common/fixtures.py` & `flask-ligand-example-0.5.2/tests/common/fixtures.py`

 * *Files identical despite different names*

### Comparing `flask-ligand-example-0.5.1/tests/integration/conftest.py` & `flask-ligand-example-0.5.2/tests/integration/conftest.py`

 * *Files identical despite different names*

### Comparing `flask-ligand-example-0.5.1/tests/integration/test_basic.py` & `flask-ligand-example-0.5.2/tests/integration/test_basic.py`

 * *Files identical despite different names*

### Comparing `flask-ligand-example-0.5.1/tests/integration/test_cli.py` & `flask-ligand-example-0.5.2/tests/integration/test_cli.py`

 * *Files identical despite different names*

### Comparing `flask-ligand-example-0.5.1/tests/unit/conftest.py` & `flask-ligand-example-0.5.2/tests/unit/conftest.py`

 * *Files identical despite different names*

### Comparing `flask-ligand-example-0.5.1/tests/unit/test_basic.py` & `flask-ligand-example-0.5.2/tests/unit/test_basic.py`

 * *Files identical despite different names*

