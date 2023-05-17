# Comparing `tmp/flask-ligand-0.7.8.tar.gz` & `tmp/flask-ligand-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flask-ligand-0.7.8.tar", last modified: Tue Apr 25 22:48:38 2023, max compression
+gzip compressed data, was "flask-ligand-0.8.0.tar", last modified: Wed May 17 23:51:40 2023, max compression
```

## Comparing `flask-ligand-0.7.8.tar` & `flask-ligand-0.8.0.tar`

### file list

```diff
@@ -1,122 +1,122 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 22:48:38.359114 flask-ligand-0.7.8/
--rw-r--r--   0 root         (0) root         (0)       14 2023-04-25 22:48:33.000000 flask-ligand-0.7.8/.flaskenv
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 22:48:38.343114 flask-ligand-0.7.8/.github/
--rw-r--r--   0 root         (0) root         (0)      528 2023-04-25 22:48:33.000000 flask-ligand-0.7.8/.github/dependabot.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 22:48:38.343114 flask-ligand-0.7.8/.github/workflows/
--rw-r--r--   0 root         (0) root         (0)      625 2023-04-25 22:48:33.000000 flask-ligand-0.7.8/.github/workflows/bump_and_publish_release.yml
--rw-r--r--   0 root         (0) root         (0)      797 2023-04-25 22:48:33.000000 flask-ligand-0.7.8/.github/workflows/coverage.yml
--rw-r--r--   0 root         (0) root         (0)      622 2023-04-25 22:48:33.000000 flask-ligand-0.7.8/.github/workflows/pull_request.yml
--rw-r--r--   0 root         (0) root         (0)     1096 2023-04-25 22:48:33.000000 flask-ligand-0.7.8/.pre-commit-config.yaml
--rw-r--r--   0 root         (0) root         (0)      371 2023-04-25 22:48:33.000000 flask-ligand-0.7.8/.readthedocs.yaml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 22:48:38.347113 flask-ligand-0.7.8/.run/
--rw-r--r--   0 root         (0) root         (0)     1296 2023-04-25 22:48:33.000000 flask-ligand-0.7.8/.run/Flask - Debug.run.xml
--rw-r--r--   0 root         (0) root         (0)     1265 2023-04-25 22:48:33.000000 flask-ligand-0.7.8/.run/Flask.run.xml
--rw-r--r--   0 root         (0) root         (0)      459 2023-04-25 22:48:33.000000 flask-ligand-0.7.8/.run/Integration Test Environment.run.xml
--rw-r--r--   0 root         (0) root         (0)     1473 2023-04-25 22:48:33.000000 flask-ligand-0.7.8/.run/Integration.run.xml
--rw-r--r--   0 root         (0) root         (0)      808 2023-04-25 22:48:33.000000 flask-ligand-0.7.8/.run/Unit (tox).run.xml
--rw-r--r--   0 root         (0) root         (0)      856 2023-04-25 22:48:33.000000 flask-ligand-0.7.8/.run/Unit (tox-fast).run.xml
--rw-r--r--   0 root         (0) root         (0)     1055 2023-04-25 22:48:33.000000 flask-ligand-0.7.8/.run/Unit - Database.run.xml
--rw-r--r--   0 root         (0) root         (0)     1045 2023-04-25 22:48:33.000000 flask-ligand-0.7.8/.run/Unit - JWT.run.xml
--rw-r--r--   0 root         (0) root         (0)     1047 2023-04-25 22:48:33.000000 flask-ligand-0.7.8/.run/Unit - OpenAPI.run.xml
--rw-r--r--   0 root         (0) root         (0)     1506 2023-04-25 22:48:33.000000 flask-ligand-0.7.8/.run/Unit - Settings.run.xml
--rw-r--r--   0 root         (0) root         (0)     1459 2023-04-25 22:48:33.000000 flask-ligand-0.7.8/.run/Unit.run.xml
--rw-r--r--   0 root         (0) root         (0)      369 2023-04-25 22:48:33.000000 flask-ligand-0.7.8/.run/develop-venv.run.xml
--rw-r--r--   0 root         (0) root         (0)      389 2023-04-25 22:48:33.000000 flask-ligand-0.7.8/.run/gen-admin-access-token.run.xml
--rw-r--r--   0 root         (0) root         (0)      361 2023-04-25 22:48:33.000000 flask-ligand-0.7.8/.run/gen-docs.run.xml
--rw-r--r--   0 root         (0) root         (0)      353 2023-04-25 22:48:33.000000 flask-ligand-0.7.8/.run/lint.run.xml
--rw-r--r--   0 root         (0) root         (0)      361 2023-04-25 22:48:33.000000 flask-ligand-0.7.8/.run/setup-db.run.xml
--rw-r--r--   0 root         (0) root         (0)      361 2023-04-25 22:48:33.000000 flask-ligand-0.7.8/.run/test-all.run.xml
--rw-r--r--   0 root         (0) root         (0)       36 2023-04-25 22:48:33.000000 flask-ligand-0.7.8/AUTHORS
--rw-r--r--   0 root         (0) root         (0)    16569 2023-04-25 22:48:34.000000 flask-ligand-0.7.8/CHANGELOG.md
--rw-r--r--   0 root         (0) root         (0)     3615 2023-04-25 22:48:33.000000 flask-ligand-0.7.8/CONTRIBUTING.rst
--rw-r--r--   0 root         (0) root         (0)    34523 2023-04-25 22:48:33.000000 flask-ligand-0.7.8/LICENSE
--rw-r--r--   0 root         (0) root         (0)     8962 2023-04-25 22:48:33.000000 flask-ligand-0.7.8/Makefile
--rw-r--r--   0 root         (0) root         (0)     5001 2023-04-25 22:48:38.359114 flask-ligand-0.7.8/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3683 2023-04-25 22:48:33.000000 flask-ligand-0.7.8/README.rst
--rw-r--r--   0 root         (0) root         (0)      939 2023-04-25 22:48:33.000000 flask-ligand-0.7.8/app.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 22:48:38.339113 flask-ligand-0.7.8/docker/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 22:48:38.347113 flask-ligand-0.7.8/docker/env_files/
--rw-r--r--   0 root         (0) root         (0)      806 2023-04-25 22:48:33.000000 flask-ligand-0.7.8/docker/env_files/integration.env
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 22:48:38.347113 flask-ligand-0.7.8/docker/kc-data/
--rw-r--r--   0 root         (0) root         (0)    78994 2023-04-25 22:48:33.000000 flask-ligand-0.7.8/docker/kc-data/flask-ligand-realm.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 22:48:38.347113 flask-ligand-0.7.8/docker/postgres-data/
--rw-r--r--   0 root         (0) root         (0)      589 2023-04-25 22:48:33.000000 flask-ligand-0.7.8/docker/postgres-data/create-multiple-postgresql-databases.sh
--rw-r--r--   0 root         (0) root         (0)      799 2023-04-25 22:48:33.000000 flask-ligand-0.7.8/docker-compose.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 22:48:38.351114 flask-ligand-0.7.8/docs/
--rw-r--r--   0 root         (0) root         (0)      632 2023-04-25 22:48:33.000000 flask-ligand-0.7.8/docs/Makefile
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 22:48:38.351114 flask-ligand-0.7.8/docs/_static/
--rw-r--r--   0 root         (0) root         (0)     7352 2023-04-25 22:48:33.000000 flask-ligand-0.7.8/docs/_static/small_logo.jpg
--rw-r--r--   0 root         (0) root         (0)     2704 2023-04-25 22:48:33.000000 flask-ligand-0.7.8/docs/api_reference.rst
--rw-r--r--   0 root         (0) root         (0)     6093 2023-04-25 22:48:33.000000 flask-ligand-0.7.8/docs/auth0.rst
--rw-r--r--   0 root         (0) root         (0)       41 2023-04-25 22:48:33.000000 flask-ligand-0.7.8/docs/authors.rst
--rw-r--r--   0 root         (0) root         (0)       79 2023-04-25 22:48:33.000000 flask-ligand-0.7.8/docs/changelog.rst
--rw-r--r--   0 root         (0) root         (0)     6080 2023-04-25 22:48:33.000000 flask-ligand-0.7.8/docs/conf.py
--rw-r--r--   0 root         (0) root         (0)      163 2023-04-25 22:48:33.000000 flask-ligand-0.7.8/docs/configuration.rst
--rw-r--r--   0 root         (0) root         (0)     2571 2023-04-25 22:48:33.000000 flask-ligand-0.7.8/docs/database_configuration.rst
--rw-r--r--   0 root         (0) root         (0)     3885 2023-04-25 22:48:33.000000 flask-ligand-0.7.8/docs/developer_guide.rst
--rw-r--r--   0 root         (0) root         (0)      207 2023-04-25 22:48:33.000000 flask-ligand-0.7.8/docs/development.rst
--rw-r--r--   0 root         (0) root         (0)    12374 2023-04-25 22:48:33.000000 flask-ligand-0.7.8/docs/flask_environments.rst
--rw-r--r--   0 root         (0) root         (0)     2411 2023-04-25 22:48:33.000000 flask-ligand-0.7.8/docs/index.rst
--rw-r--r--   0 root         (0) root         (0)     1139 2023-04-25 22:48:33.000000 flask-ligand-0.7.8/docs/integration_testing.rst
--rw-r--r--   0 root         (0) root         (0)       48 2023-04-25 22:48:33.000000 flask-ligand-0.7.8/docs/license.rst
--rw-r--r--   0 root         (0) root         (0)      765 2023-04-25 22:48:33.000000 flask-ligand-0.7.8/docs/make.bat
--rw-r--r--   0 root         (0) root         (0)     1304 2023-04-25 22:48:33.000000 flask-ligand-0.7.8/docs/oidc_configuration.rst
--rw-r--r--   0 root         (0) root         (0)     2546 2023-04-25 22:48:33.000000 flask-ligand-0.7.8/docs/openapi.rst
--rw-r--r--   0 root         (0) root         (0)    25967 2023-04-25 22:48:33.000000 flask-ligand-0.7.8/docs/quickstart.rst
--rw-r--r--   0 root         (0) root         (0)     1637 2023-04-25 22:48:33.000000 flask-ligand-0.7.8/docs/release_process.rst
--rw-r--r--   0 root         (0) root         (0)      130 2023-04-25 22:48:33.000000 flask-ligand-0.7.8/docs/requirements.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 22:48:38.351114 flask-ligand-0.7.8/flask_ligand/
--rw-r--r--   0 root         (0) root         (0)     3715 2023-04-25 22:48:34.000000 flask-ligand-0.7.8/flask_ligand/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1762 2023-04-25 22:48:33.000000 flask-ligand-0.7.8/flask_ligand/cli.py
--rw-r--r--   0 root         (0) root         (0)     5441 2023-04-25 22:48:33.000000 flask-ligand-0.7.8/flask_ligand/controllers.py
--rw-r--r--   0 root         (0) root         (0)    12650 2023-04-25 22:48:33.000000 flask-ligand-0.7.8/flask_ligand/default_settings.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 22:48:38.351114 flask-ligand-0.7.8/flask_ligand/extensions/
--rw-r--r--   0 root         (0) root         (0)     1514 2023-04-25 22:48:33.000000 flask-ligand-0.7.8/flask_ligand/extensions/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6979 2023-04-25 22:48:33.000000 flask-ligand-0.7.8/flask_ligand/extensions/api.py
--rw-r--r--   0 root         (0) root         (0)     2008 2023-04-25 22:48:33.000000 flask-ligand-0.7.8/flask_ligand/extensions/database.py
--rw-r--r--   0 root         (0) root         (0)     5210 2023-04-25 22:48:33.000000 flask-ligand-0.7.8/flask_ligand/extensions/jwt.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-25 22:48:33.000000 flask-ligand-0.7.8/flask_ligand/py.typed
--rw-r--r--   0 root         (0) root         (0)     1116 2023-04-25 22:48:33.000000 flask-ligand-0.7.8/flask_ligand/schemas.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 22:48:38.355114 flask-ligand-0.7.8/flask_ligand/views/
--rw-r--r--   0 root         (0) root         (0)     1552 2023-04-25 22:48:33.000000 flask-ligand-0.7.8/flask_ligand/views/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 22:48:38.355114 flask-ligand-0.7.8/flask_ligand/views/common/
--rw-r--r--   0 root         (0) root         (0)       44 2023-04-25 22:48:33.000000 flask-ligand-0.7.8/flask_ligand/views/common/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1048 2023-04-25 22:48:33.000000 flask-ligand-0.7.8/flask_ligand/views/common/openapi_doc.py
--rw-r--r--   0 root         (0) root         (0)     3029 2023-04-25 22:48:33.000000 flask-ligand-0.7.8/flask_ligand/views/openapi.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 22:48:38.351114 flask-ligand-0.7.8/flask_ligand.egg-info/
--rw-r--r--   0 root         (0) root         (0)     5001 2023-04-25 22:48:38.000000 flask-ligand-0.7.8/flask_ligand.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2670 2023-04-25 22:48:38.000000 flask-ligand-0.7.8/flask_ligand.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-25 22:48:38.000000 flask-ligand-0.7.8/flask_ligand.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-25 22:48:38.000000 flask-ligand-0.7.8/flask_ligand.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       46 2023-04-25 22:48:38.000000 flask-ligand-0.7.8/flask_ligand.egg-info/pbr.json
--rw-r--r--   0 root         (0) root         (0)      276 2023-04-25 22:48:38.000000 flask-ligand-0.7.8/flask_ligand.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       13 2023-04-25 22:48:38.000000 flask-ligand-0.7.8/flask_ligand.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1112 2023-04-25 22:48:33.000000 flask-ligand-0.7.8/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)      514 2023-04-25 22:48:33.000000 flask-ligand-0.7.8/requirements-dev.txt
--rw-r--r--   0 root         (0) root         (0)      329 2023-04-25 22:48:33.000000 flask-ligand-0.7.8/requirements.txt
--rw-r--r--   0 root         (0) root         (0)     1437 2023-04-25 22:48:38.359114 flask-ligand-0.7.8/setup.cfg
--rwxr-xr-x   0 root         (0) root         (0)      737 2023-04-25 22:48:33.000000 flask-ligand-0.7.8/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 22:48:38.355114 flask-ligand-0.7.8/tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-25 22:48:33.000000 flask-ligand-0.7.8/tests/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 22:48:38.355114 flask-ligand-0.7.8/tests/integration/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-25 22:48:33.000000 flask-ligand-0.7.8/tests/integration/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8190 2023-04-25 22:48:33.000000 flask-ligand-0.7.8/tests/integration/conftest.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 22:48:38.355114 flask-ligand-0.7.8/tests/integration/migrations/
--rw-r--r--   0 root         (0) root         (0)       41 2023-04-25 22:48:33.000000 flask-ligand-0.7.8/tests/integration/migrations/README
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-25 22:48:33.000000 flask-ligand-0.7.8/tests/integration/migrations/__init__.py
--rw-r--r--   0 root         (0) root         (0)      855 2023-04-25 22:48:33.000000 flask-ligand-0.7.8/tests/integration/migrations/alembic.ini
--rw-r--r--   0 root         (0) root         (0)     2736 2023-04-25 22:48:33.000000 flask-ligand-0.7.8/tests/integration/migrations/env.py
--rw-r--r--   0 root         (0) root         (0)      494 2023-04-25 22:48:33.000000 flask-ligand-0.7.8/tests/integration/migrations/script.py.mako
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 22:48:38.355114 flask-ligand-0.7.8/tests/integration/migrations/versions/
--rw-r--r--   0 root         (0) root         (0)      691 2023-04-25 22:48:33.000000 flask-ligand-0.7.8/tests/integration/migrations/versions/47f10265b5d7_.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-25 22:48:33.000000 flask-ligand-0.7.8/tests/integration/migrations/versions/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1457 2023-04-25 22:48:33.000000 flask-ligand-0.7.8/tests/integration/test_basic.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 22:48:38.359114 flask-ligand-0.7.8/tests/unit/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-25 22:48:33.000000 flask-ligand-0.7.8/tests/unit/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2864 2023-04-25 22:48:33.000000 flask-ligand-0.7.8/tests/unit/conftest.py
--rw-r--r--   0 root         (0) root         (0)     2666 2023-04-25 22:48:33.000000 flask-ligand-0.7.8/tests/unit/test_api_extension.py
--rw-r--r--   0 root         (0) root         (0)    10329 2023-04-25 22:48:33.000000 flask-ligand-0.7.8/tests/unit/test_database_extension.py
--rw-r--r--   0 root         (0) root         (0)     6791 2023-04-25 22:48:33.000000 flask-ligand-0.7.8/tests/unit/test_jwt_extension.py
--rw-r--r--   0 root         (0) root         (0)    10519 2023-04-25 22:48:33.000000 flask-ligand-0.7.8/tests/unit/test_openapi_api.py
--rw-r--r--   0 root         (0) root         (0)    21947 2023-04-25 22:48:33.000000 flask-ligand-0.7.8/tests/unit/test_settings.py
--rw-r--r--   0 root         (0) root         (0)      369 2023-04-25 22:48:33.000000 flask-ligand-0.7.8/tox.ini
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 23:51:39.997346 flask-ligand-0.8.0/
+-rw-r--r--   0 root         (0) root         (0)       14 2023-05-17 23:51:36.000000 flask-ligand-0.8.0/.flaskenv
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 23:51:39.989346 flask-ligand-0.8.0/.github/
+-rw-r--r--   0 root         (0) root         (0)      528 2023-05-17 23:51:36.000000 flask-ligand-0.8.0/.github/dependabot.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 23:51:39.989346 flask-ligand-0.8.0/.github/workflows/
+-rw-r--r--   0 root         (0) root         (0)      625 2023-05-17 23:51:36.000000 flask-ligand-0.8.0/.github/workflows/bump_and_publish_release.yml
+-rw-r--r--   0 root         (0) root         (0)      797 2023-05-17 23:51:36.000000 flask-ligand-0.8.0/.github/workflows/coverage.yml
+-rw-r--r--   0 root         (0) root         (0)      622 2023-05-17 23:51:36.000000 flask-ligand-0.8.0/.github/workflows/pull_request.yml
+-rw-r--r--   0 root         (0) root         (0)     1060 2023-05-17 23:51:36.000000 flask-ligand-0.8.0/.pre-commit-config.yaml
+-rw-r--r--   0 root         (0) root         (0)      371 2023-05-17 23:51:36.000000 flask-ligand-0.8.0/.readthedocs.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 23:51:39.989346 flask-ligand-0.8.0/.run/
+-rw-r--r--   0 root         (0) root         (0)     1296 2023-05-17 23:51:36.000000 flask-ligand-0.8.0/.run/Flask - Debug.run.xml
+-rw-r--r--   0 root         (0) root         (0)     1265 2023-05-17 23:51:36.000000 flask-ligand-0.8.0/.run/Flask.run.xml
+-rw-r--r--   0 root         (0) root         (0)      459 2023-05-17 23:51:36.000000 flask-ligand-0.8.0/.run/Integration Test Environment.run.xml
+-rw-r--r--   0 root         (0) root         (0)     1473 2023-05-17 23:51:36.000000 flask-ligand-0.8.0/.run/Integration.run.xml
+-rw-r--r--   0 root         (0) root         (0)      808 2023-05-17 23:51:36.000000 flask-ligand-0.8.0/.run/Unit (tox).run.xml
+-rw-r--r--   0 root         (0) root         (0)      856 2023-05-17 23:51:36.000000 flask-ligand-0.8.0/.run/Unit (tox-fast).run.xml
+-rw-r--r--   0 root         (0) root         (0)     1055 2023-05-17 23:51:36.000000 flask-ligand-0.8.0/.run/Unit - Database.run.xml
+-rw-r--r--   0 root         (0) root         (0)     1045 2023-05-17 23:51:36.000000 flask-ligand-0.8.0/.run/Unit - JWT.run.xml
+-rw-r--r--   0 root         (0) root         (0)     1047 2023-05-17 23:51:36.000000 flask-ligand-0.8.0/.run/Unit - OpenAPI.run.xml
+-rw-r--r--   0 root         (0) root         (0)     1506 2023-05-17 23:51:36.000000 flask-ligand-0.8.0/.run/Unit - Settings.run.xml
+-rw-r--r--   0 root         (0) root         (0)     1459 2023-05-17 23:51:36.000000 flask-ligand-0.8.0/.run/Unit.run.xml
+-rw-r--r--   0 root         (0) root         (0)      369 2023-05-17 23:51:36.000000 flask-ligand-0.8.0/.run/develop-venv.run.xml
+-rw-r--r--   0 root         (0) root         (0)      389 2023-05-17 23:51:36.000000 flask-ligand-0.8.0/.run/gen-admin-access-token.run.xml
+-rw-r--r--   0 root         (0) root         (0)      361 2023-05-17 23:51:36.000000 flask-ligand-0.8.0/.run/gen-docs.run.xml
+-rw-r--r--   0 root         (0) root         (0)      353 2023-05-17 23:51:36.000000 flask-ligand-0.8.0/.run/lint.run.xml
+-rw-r--r--   0 root         (0) root         (0)      361 2023-05-17 23:51:36.000000 flask-ligand-0.8.0/.run/setup-db.run.xml
+-rw-r--r--   0 root         (0) root         (0)      361 2023-05-17 23:51:36.000000 flask-ligand-0.8.0/.run/test-all.run.xml
+-rw-r--r--   0 root         (0) root         (0)       36 2023-05-17 23:51:36.000000 flask-ligand-0.8.0/AUTHORS
+-rw-r--r--   0 root         (0) root         (0)    16888 2023-05-17 23:51:36.000000 flask-ligand-0.8.0/CHANGELOG.md
+-rw-r--r--   0 root         (0) root         (0)     3615 2023-05-17 23:51:36.000000 flask-ligand-0.8.0/CONTRIBUTING.rst
+-rw-r--r--   0 root         (0) root         (0)    34523 2023-05-17 23:51:36.000000 flask-ligand-0.8.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     8962 2023-05-17 23:51:36.000000 flask-ligand-0.8.0/Makefile
+-rw-r--r--   0 root         (0) root         (0)     5001 2023-05-17 23:51:39.997346 flask-ligand-0.8.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3683 2023-05-17 23:51:36.000000 flask-ligand-0.8.0/README.rst
+-rw-r--r--   0 root         (0) root         (0)      939 2023-05-17 23:51:36.000000 flask-ligand-0.8.0/app.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 23:51:39.985346 flask-ligand-0.8.0/docker/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 23:51:39.989346 flask-ligand-0.8.0/docker/env_files/
+-rw-r--r--   0 root         (0) root         (0)      806 2023-05-17 23:51:36.000000 flask-ligand-0.8.0/docker/env_files/integration.env
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 23:51:39.993347 flask-ligand-0.8.0/docker/kc-data/
+-rw-r--r--   0 root         (0) root         (0)    78994 2023-05-17 23:51:36.000000 flask-ligand-0.8.0/docker/kc-data/flask-ligand-realm.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 23:51:39.993347 flask-ligand-0.8.0/docker/postgres-data/
+-rw-r--r--   0 root         (0) root         (0)      589 2023-05-17 23:51:36.000000 flask-ligand-0.8.0/docker/postgres-data/create-multiple-postgresql-databases.sh
+-rw-r--r--   0 root         (0) root         (0)      799 2023-05-17 23:51:36.000000 flask-ligand-0.8.0/docker-compose.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 23:51:39.993347 flask-ligand-0.8.0/docs/
+-rw-r--r--   0 root         (0) root         (0)      632 2023-05-17 23:51:36.000000 flask-ligand-0.8.0/docs/Makefile
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 23:51:39.993347 flask-ligand-0.8.0/docs/_static/
+-rw-r--r--   0 root         (0) root         (0)     7352 2023-05-17 23:51:36.000000 flask-ligand-0.8.0/docs/_static/small_logo.jpg
+-rw-r--r--   0 root         (0) root         (0)     2704 2023-05-17 23:51:36.000000 flask-ligand-0.8.0/docs/api_reference.rst
+-rw-r--r--   0 root         (0) root         (0)     6093 2023-05-17 23:51:36.000000 flask-ligand-0.8.0/docs/auth0.rst
+-rw-r--r--   0 root         (0) root         (0)       41 2023-05-17 23:51:36.000000 flask-ligand-0.8.0/docs/authors.rst
+-rw-r--r--   0 root         (0) root         (0)       79 2023-05-17 23:51:36.000000 flask-ligand-0.8.0/docs/changelog.rst
+-rw-r--r--   0 root         (0) root         (0)     6080 2023-05-17 23:51:36.000000 flask-ligand-0.8.0/docs/conf.py
+-rw-r--r--   0 root         (0) root         (0)      163 2023-05-17 23:51:36.000000 flask-ligand-0.8.0/docs/configuration.rst
+-rw-r--r--   0 root         (0) root         (0)     2571 2023-05-17 23:51:36.000000 flask-ligand-0.8.0/docs/database_configuration.rst
+-rw-r--r--   0 root         (0) root         (0)     3885 2023-05-17 23:51:36.000000 flask-ligand-0.8.0/docs/developer_guide.rst
+-rw-r--r--   0 root         (0) root         (0)      207 2023-05-17 23:51:36.000000 flask-ligand-0.8.0/docs/development.rst
+-rw-r--r--   0 root         (0) root         (0)    12374 2023-05-17 23:51:36.000000 flask-ligand-0.8.0/docs/flask_environments.rst
+-rw-r--r--   0 root         (0) root         (0)     2411 2023-05-17 23:51:36.000000 flask-ligand-0.8.0/docs/index.rst
+-rw-r--r--   0 root         (0) root         (0)     1139 2023-05-17 23:51:36.000000 flask-ligand-0.8.0/docs/integration_testing.rst
+-rw-r--r--   0 root         (0) root         (0)       48 2023-05-17 23:51:36.000000 flask-ligand-0.8.0/docs/license.rst
+-rw-r--r--   0 root         (0) root         (0)      765 2023-05-17 23:51:36.000000 flask-ligand-0.8.0/docs/make.bat
+-rw-r--r--   0 root         (0) root         (0)     1304 2023-05-17 23:51:36.000000 flask-ligand-0.8.0/docs/oidc_configuration.rst
+-rw-r--r--   0 root         (0) root         (0)     2546 2023-05-17 23:51:36.000000 flask-ligand-0.8.0/docs/openapi.rst
+-rw-r--r--   0 root         (0) root         (0)    25967 2023-05-17 23:51:36.000000 flask-ligand-0.8.0/docs/quickstart.rst
+-rw-r--r--   0 root         (0) root         (0)     1637 2023-05-17 23:51:36.000000 flask-ligand-0.8.0/docs/release_process.rst
+-rw-r--r--   0 root         (0) root         (0)      130 2023-05-17 23:51:36.000000 flask-ligand-0.8.0/docs/requirements.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 23:51:39.993347 flask-ligand-0.8.0/flask_ligand/
+-rw-r--r--   0 root         (0) root         (0)     3715 2023-05-17 23:51:36.000000 flask-ligand-0.8.0/flask_ligand/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1762 2023-05-17 23:51:36.000000 flask-ligand-0.8.0/flask_ligand/cli.py
+-rw-r--r--   0 root         (0) root         (0)     5441 2023-05-17 23:51:36.000000 flask-ligand-0.8.0/flask_ligand/controllers.py
+-rw-r--r--   0 root         (0) root         (0)    12650 2023-05-17 23:51:36.000000 flask-ligand-0.8.0/flask_ligand/default_settings.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 23:51:39.993347 flask-ligand-0.8.0/flask_ligand/extensions/
+-rw-r--r--   0 root         (0) root         (0)     1514 2023-05-17 23:51:36.000000 flask-ligand-0.8.0/flask_ligand/extensions/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6979 2023-05-17 23:51:36.000000 flask-ligand-0.8.0/flask_ligand/extensions/api.py
+-rw-r--r--   0 root         (0) root         (0)     2008 2023-05-17 23:51:36.000000 flask-ligand-0.8.0/flask_ligand/extensions/database.py
+-rw-r--r--   0 root         (0) root         (0)     5210 2023-05-17 23:51:36.000000 flask-ligand-0.8.0/flask_ligand/extensions/jwt.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-17 23:51:36.000000 flask-ligand-0.8.0/flask_ligand/py.typed
+-rw-r--r--   0 root         (0) root         (0)     1116 2023-05-17 23:51:36.000000 flask-ligand-0.8.0/flask_ligand/schemas.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 23:51:39.997346 flask-ligand-0.8.0/flask_ligand/views/
+-rw-r--r--   0 root         (0) root         (0)     1552 2023-05-17 23:51:36.000000 flask-ligand-0.8.0/flask_ligand/views/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 23:51:39.997346 flask-ligand-0.8.0/flask_ligand/views/common/
+-rw-r--r--   0 root         (0) root         (0)       44 2023-05-17 23:51:36.000000 flask-ligand-0.8.0/flask_ligand/views/common/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1048 2023-05-17 23:51:36.000000 flask-ligand-0.8.0/flask_ligand/views/common/openapi_doc.py
+-rw-r--r--   0 root         (0) root         (0)     3029 2023-05-17 23:51:36.000000 flask-ligand-0.8.0/flask_ligand/views/openapi.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 23:51:39.993347 flask-ligand-0.8.0/flask_ligand.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5001 2023-05-17 23:51:39.000000 flask-ligand-0.8.0/flask_ligand.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2670 2023-05-17 23:51:39.000000 flask-ligand-0.8.0/flask_ligand.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-17 23:51:39.000000 flask-ligand-0.8.0/flask_ligand.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-17 23:51:39.000000 flask-ligand-0.8.0/flask_ligand.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       46 2023-05-17 23:51:39.000000 flask-ligand-0.8.0/flask_ligand.egg-info/pbr.json
+-rw-r--r--   0 root         (0) root         (0)      276 2023-05-17 23:51:39.000000 flask-ligand-0.8.0/flask_ligand.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2023-05-17 23:51:39.000000 flask-ligand-0.8.0/flask_ligand.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1112 2023-05-17 23:51:36.000000 flask-ligand-0.8.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)      492 2023-05-17 23:51:36.000000 flask-ligand-0.8.0/requirements-dev.txt
+-rw-r--r--   0 root         (0) root         (0)      329 2023-05-17 23:51:36.000000 flask-ligand-0.8.0/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)     1437 2023-05-17 23:51:39.997346 flask-ligand-0.8.0/setup.cfg
+-rwxr-xr-x   0 root         (0) root         (0)      737 2023-05-17 23:51:36.000000 flask-ligand-0.8.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 23:51:39.997346 flask-ligand-0.8.0/tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-17 23:51:36.000000 flask-ligand-0.8.0/tests/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 23:51:39.997346 flask-ligand-0.8.0/tests/integration/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-17 23:51:36.000000 flask-ligand-0.8.0/tests/integration/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8190 2023-05-17 23:51:36.000000 flask-ligand-0.8.0/tests/integration/conftest.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 23:51:39.997346 flask-ligand-0.8.0/tests/integration/migrations/
+-rw-r--r--   0 root         (0) root         (0)       41 2023-05-17 23:51:36.000000 flask-ligand-0.8.0/tests/integration/migrations/README
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-17 23:51:36.000000 flask-ligand-0.8.0/tests/integration/migrations/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      855 2023-05-17 23:51:36.000000 flask-ligand-0.8.0/tests/integration/migrations/alembic.ini
+-rw-r--r--   0 root         (0) root         (0)     2736 2023-05-17 23:51:36.000000 flask-ligand-0.8.0/tests/integration/migrations/env.py
+-rw-r--r--   0 root         (0) root         (0)      494 2023-05-17 23:51:36.000000 flask-ligand-0.8.0/tests/integration/migrations/script.py.mako
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 23:51:39.997346 flask-ligand-0.8.0/tests/integration/migrations/versions/
+-rw-r--r--   0 root         (0) root         (0)      691 2023-05-17 23:51:36.000000 flask-ligand-0.8.0/tests/integration/migrations/versions/47f10265b5d7_.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-17 23:51:36.000000 flask-ligand-0.8.0/tests/integration/migrations/versions/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1457 2023-05-17 23:51:36.000000 flask-ligand-0.8.0/tests/integration/test_basic.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 23:51:39.997346 flask-ligand-0.8.0/tests/unit/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-17 23:51:36.000000 flask-ligand-0.8.0/tests/unit/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2864 2023-05-17 23:51:36.000000 flask-ligand-0.8.0/tests/unit/conftest.py
+-rw-r--r--   0 root         (0) root         (0)     2666 2023-05-17 23:51:36.000000 flask-ligand-0.8.0/tests/unit/test_api_extension.py
+-rw-r--r--   0 root         (0) root         (0)    10329 2023-05-17 23:51:36.000000 flask-ligand-0.8.0/tests/unit/test_database_extension.py
+-rw-r--r--   0 root         (0) root         (0)     6791 2023-05-17 23:51:36.000000 flask-ligand-0.8.0/tests/unit/test_jwt_extension.py
+-rw-r--r--   0 root         (0) root         (0)    10519 2023-05-17 23:51:36.000000 flask-ligand-0.8.0/tests/unit/test_openapi_api.py
+-rw-r--r--   0 root         (0) root         (0)    21947 2023-05-17 23:51:36.000000 flask-ligand-0.8.0/tests/unit/test_settings.py
+-rw-r--r--   0 root         (0) root         (0)      369 2023-05-17 23:51:36.000000 flask-ligand-0.8.0/tox.ini
```

### Comparing `flask-ligand-0.7.8/.github/dependabot.yml` & `flask-ligand-0.8.0/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `flask-ligand-0.7.8/.github/workflows/bump_and_publish_release.yml` & `flask-ligand-0.8.0/.github/workflows/bump_and_publish_release.yml`

 * *Files identical despite different names*

### Comparing `flask-ligand-0.7.8/.github/workflows/coverage.yml` & `flask-ligand-0.8.0/.github/workflows/coverage.yml`

 * *Files identical despite different names*

### Comparing `flask-ligand-0.7.8/.github/workflows/pull_request.yml` & `flask-ligand-0.8.0/.github/workflows/pull_request.yml`

 * *Files identical despite different names*

### Comparing `flask-ligand-0.7.8/.pre-commit-config.yaml` & `flask-ligand-0.8.0/.pre-commit-config.yaml`

 * *Files 6% similar despite different names*

```diff
@@ -12,26 +12,25 @@
     hooks:
     -   id: black
 -   repo: https://github.com/PyCQA/flake8
     rev: 6.0.0
     hooks:
     -   id: flake8
 -   repo: https://github.com/pre-commit/mirrors-mypy
-    rev: v1.2.0
+    rev: v1.3.0
     hooks:
     -   id: mypy
         additional_dependencies:
         -   "types-Flask-Cors~=3.0"
         -   "types-Flask-SQLAlchemy~=2.5"
-        -   "types-mock~=4.0"
+        -   "types-mock~=5.0"
         -   "types-PyYAML~=6.0"
         -   "types-requests~=2.28"
         -   "types-setuptools~=63.4"
         -   "types-smorest~=1.1"
-        -   "types-SQLAlchemy~=1.4"
         -   "types-sqlalchemy-utils~=1.0"
         -   "types-urllib3<1.27"
 -   repo: https://github.com/rstcheck/rstcheck
     rev: v6.1.2
     hooks:
     -   id: rstcheck
         additional_dependencies: [sphinx]
```

### Comparing `flask-ligand-0.7.8/.run/Flask - Debug.run.xml` & `flask-ligand-0.8.0/.run/Flask - Debug.run.xml`

 * *Files identical despite different names*

### Comparing `flask-ligand-0.7.8/.run/Flask.run.xml` & `flask-ligand-0.8.0/.run/Flask.run.xml`

 * *Files identical despite different names*

### Comparing `flask-ligand-0.7.8/.run/Integration.run.xml` & `flask-ligand-0.8.0/.run/Integration.run.xml`

 * *Files identical despite different names*

### Comparing `flask-ligand-0.7.8/.run/Unit (tox).run.xml` & `flask-ligand-0.8.0/.run/Unit (tox).run.xml`

 * *Files identical despite different names*

### Comparing `flask-ligand-0.7.8/.run/Unit (tox-fast).run.xml` & `flask-ligand-0.8.0/.run/Unit (tox-fast).run.xml`

 * *Files identical despite different names*

### Comparing `flask-ligand-0.7.8/.run/Unit - Database.run.xml` & `flask-ligand-0.8.0/.run/Unit - Database.run.xml`

 * *Files identical despite different names*

### Comparing `flask-ligand-0.7.8/.run/Unit - JWT.run.xml` & `flask-ligand-0.8.0/.run/Unit - JWT.run.xml`

 * *Files identical despite different names*

### Comparing `flask-ligand-0.7.8/.run/Unit - OpenAPI.run.xml` & `flask-ligand-0.8.0/.run/Unit - OpenAPI.run.xml`

 * *Files identical despite different names*

### Comparing `flask-ligand-0.7.8/.run/Unit - Settings.run.xml` & `flask-ligand-0.8.0/.run/Unit - Settings.run.xml`

 * *Files identical despite different names*

### Comparing `flask-ligand-0.7.8/.run/Unit.run.xml` & `flask-ligand-0.8.0/.run/Unit.run.xml`

 * *Files identical despite different names*

### Comparing `flask-ligand-0.7.8/CHANGELOG.md` & `flask-ligand-0.8.0/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,19 @@
 Changelog
 =========
 
 <!--next-version-placeholder-->
 
+## v0.8.0 (2023-05-17)
+### Feature
+* [FIX:sparkles:] Update mypy Deps ([`d6bce6e`](https://github.com/cowofevil/flask-ligand/commit/d6bce6ee5758fa02b15ddeb73f3b42f7fc792612))
+
+### Other
+* [FIX:robot:] Update Deps ([`4d1a1e5`](https://github.com/cowofevil/flask-ligand/commit/4d1a1e5760c8708ee2b9bf1c29a82d904d0212a0))
+
 ## v0.7.8 (2023-04-25)
 ### Fix
 * :arrow_up: Update sphinx-autodoc-typehints requirement ([`b318780`](https://github.com/cowofevil/flask-ligand/commit/b3187807256a9f8360d83e48833acd63851285a4))
 * :arrow_up: Update pipdeptree requirement from ~=2.5 to ~=2.7 ([`7b0498d`](https://github.com/cowofevil/flask-ligand/commit/7b0498d542dc604c0a1406276dc682b46bae448a))
 
 ## v0.7.7 (2023-04-25)
 ### Fix
```

### Comparing `flask-ligand-0.7.8/CONTRIBUTING.rst` & `flask-ligand-0.8.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `flask-ligand-0.7.8/LICENSE` & `flask-ligand-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `flask-ligand-0.7.8/Makefile` & `flask-ligand-0.8.0/Makefile`

 * *Files identical despite different names*

### Comparing `flask-ligand-0.7.8/PKG-INFO` & `flask-ligand-0.8.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flask-ligand
-Version: 0.7.8
+Version: 0.8.0
 Summary: A simple flask library for building microservices with RBAC JWT security, OpenAPI client and SQLAlchemy database support.
 Author: Ryan Gard
 Author-email: ryan@gardiancapitol.com
 License: GNU Affero General Public License v3
 Project-URL: Changelog, https://github.com/cowofevil/flask-ligand/blob/main/CHANGELOG.md
 Project-URL: Source, https://github.com/cowofevil/flask-ligand
 Project-URL: Tracker, https://github.com/cowofevil/flask-ligand/issues
```

### Comparing `flask-ligand-0.7.8/README.rst` & `flask-ligand-0.8.0/README.rst`

 * *Files identical despite different names*

### Comparing `flask-ligand-0.7.8/app.py` & `flask-ligand-0.8.0/app.py`

 * *Files identical despite different names*

### Comparing `flask-ligand-0.7.8/docker/env_files/integration.env` & `flask-ligand-0.8.0/docker/env_files/integration.env`

 * *Files identical despite different names*

### Comparing `flask-ligand-0.7.8/docker/kc-data/flask-ligand-realm.json` & `flask-ligand-0.8.0/docker/kc-data/flask-ligand-realm.json`

 * *Files identical despite different names*

### Comparing `flask-ligand-0.7.8/docker/postgres-data/create-multiple-postgresql-databases.sh` & `flask-ligand-0.8.0/docker/postgres-data/create-multiple-postgresql-databases.sh`

 * *Files identical despite different names*

### Comparing `flask-ligand-0.7.8/docker-compose.yml` & `flask-ligand-0.8.0/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `flask-ligand-0.7.8/docs/Makefile` & `flask-ligand-0.8.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `flask-ligand-0.7.8/docs/_static/small_logo.jpg` & `flask-ligand-0.8.0/docs/_static/small_logo.jpg`

 * *Files identical despite different names*

### Comparing `flask-ligand-0.7.8/docs/api_reference.rst` & `flask-ligand-0.8.0/docs/api_reference.rst`

 * *Files identical despite different names*

### Comparing `flask-ligand-0.7.8/docs/auth0.rst` & `flask-ligand-0.8.0/docs/auth0.rst`

 * *Files identical despite different names*

### Comparing `flask-ligand-0.7.8/docs/conf.py` & `flask-ligand-0.8.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `flask-ligand-0.7.8/docs/database_configuration.rst` & `flask-ligand-0.8.0/docs/database_configuration.rst`

 * *Files identical despite different names*

### Comparing `flask-ligand-0.7.8/docs/developer_guide.rst` & `flask-ligand-0.8.0/docs/developer_guide.rst`

 * *Files identical despite different names*

### Comparing `flask-ligand-0.7.8/docs/flask_environments.rst` & `flask-ligand-0.8.0/docs/flask_environments.rst`

 * *Files identical despite different names*

### Comparing `flask-ligand-0.7.8/docs/index.rst` & `flask-ligand-0.8.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `flask-ligand-0.7.8/docs/integration_testing.rst` & `flask-ligand-0.8.0/docs/integration_testing.rst`

 * *Files identical despite different names*

### Comparing `flask-ligand-0.7.8/docs/make.bat` & `flask-ligand-0.8.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `flask-ligand-0.7.8/docs/oidc_configuration.rst` & `flask-ligand-0.8.0/docs/oidc_configuration.rst`

 * *Files identical despite different names*

### Comparing `flask-ligand-0.7.8/docs/openapi.rst` & `flask-ligand-0.8.0/docs/openapi.rst`

 * *Files identical despite different names*

### Comparing `flask-ligand-0.7.8/docs/quickstart.rst` & `flask-ligand-0.8.0/docs/quickstart.rst`

 * *Files identical despite different names*

### Comparing `flask-ligand-0.7.8/docs/release_process.rst` & `flask-ligand-0.8.0/docs/release_process.rst`

 * *Files identical despite different names*

### Comparing `flask-ligand-0.7.8/flask_ligand/__init__.py` & `flask-ligand-0.8.0/flask_ligand/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     from typing import Any, Tuple
     from flask_ligand.extensions.api import Api
 
 
 # ======================================================================================================================
 # Globals
 # ======================================================================================================================
-__version__ = "0.7.8"
+__version__ = "0.8.0"
 
 
 # ======================================================================================================================
 # Functions: Public
 # ======================================================================================================================
 def create_app(
     flask_app_name: str,
```

### Comparing `flask-ligand-0.7.8/flask_ligand/cli.py` & `flask-ligand-0.8.0/flask_ligand/cli.py`

 * *Files identical despite different names*

### Comparing `flask-ligand-0.7.8/flask_ligand/controllers.py` & `flask-ligand-0.8.0/flask_ligand/controllers.py`

 * *Files identical despite different names*

### Comparing `flask-ligand-0.7.8/flask_ligand/default_settings.py` & `flask-ligand-0.8.0/flask_ligand/default_settings.py`

 * *Files identical despite different names*

### Comparing `flask-ligand-0.7.8/flask_ligand/extensions/__init__.py` & `flask-ligand-0.8.0/flask_ligand/extensions/__init__.py`

 * *Files identical despite different names*

### Comparing `flask-ligand-0.7.8/flask_ligand/extensions/api.py` & `flask-ligand-0.8.0/flask_ligand/extensions/api.py`

 * *Files identical despite different names*

### Comparing `flask-ligand-0.7.8/flask_ligand/extensions/database.py` & `flask-ligand-0.8.0/flask_ligand/extensions/database.py`

 * *Files identical despite different names*

### Comparing `flask-ligand-0.7.8/flask_ligand/extensions/jwt.py` & `flask-ligand-0.8.0/flask_ligand/extensions/jwt.py`

 * *Files identical despite different names*

### Comparing `flask-ligand-0.7.8/flask_ligand/schemas.py` & `flask-ligand-0.8.0/flask_ligand/schemas.py`

 * *Files identical despite different names*

### Comparing `flask-ligand-0.7.8/flask_ligand/views/__init__.py` & `flask-ligand-0.8.0/flask_ligand/views/__init__.py`

 * *Files identical despite different names*

### Comparing `flask-ligand-0.7.8/flask_ligand/views/common/openapi_doc.py` & `flask-ligand-0.8.0/flask_ligand/views/common/openapi_doc.py`

 * *Files identical despite different names*

### Comparing `flask-ligand-0.7.8/flask_ligand/views/openapi.py` & `flask-ligand-0.8.0/flask_ligand/views/openapi.py`

 * *Files identical despite different names*

### Comparing `flask-ligand-0.7.8/flask_ligand.egg-info/PKG-INFO` & `flask-ligand-0.8.0/flask_ligand.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flask-ligand
-Version: 0.7.8
+Version: 0.8.0
 Summary: A simple flask library for building microservices with RBAC JWT security, OpenAPI client and SQLAlchemy database support.
 Author: Ryan Gard
 Author-email: ryan@gardiancapitol.com
 License: GNU Affero General Public License v3
 Project-URL: Changelog, https://github.com/cowofevil/flask-ligand/blob/main/CHANGELOG.md
 Project-URL: Source, https://github.com/cowofevil/flask-ligand
 Project-URL: Tracker, https://github.com/cowofevil/flask-ligand/issues
```

### Comparing `flask-ligand-0.7.8/flask_ligand.egg-info/SOURCES.txt` & `flask-ligand-0.8.0/flask_ligand.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `flask-ligand-0.7.8/pyproject.toml` & `flask-ligand-0.8.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `flask-ligand-0.7.8/setup.cfg` & `flask-ligand-0.8.0/setup.cfg`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = flask-ligand
-version = 0.7.8
+version = 0.8.0
 summary = A simple flask library for building microservices with RBAC JWT security, OpenAPI client and SQLAlchemy database support.
 description_file = README.rst
 description_content_type = text/x-rst; charset=UTF-8
 author = Ryan Gard
 author_email = ryan@gardiancapitol.com
 keywords = flask
 license = GNU Affero General Public License v3
```

### Comparing `flask-ligand-0.7.8/setup.py` & `flask-ligand-0.8.0/setup.py`

 * *Files identical despite different names*

### Comparing `flask-ligand-0.7.8/tests/integration/conftest.py` & `flask-ligand-0.8.0/tests/integration/conftest.py`

 * *Files identical despite different names*

### Comparing `flask-ligand-0.7.8/tests/integration/migrations/alembic.ini` & `flask-ligand-0.8.0/tests/integration/migrations/alembic.ini`

 * *Files identical despite different names*

### Comparing `flask-ligand-0.7.8/tests/integration/migrations/env.py` & `flask-ligand-0.8.0/tests/integration/migrations/env.py`

 * *Files identical despite different names*

### Comparing `flask-ligand-0.7.8/tests/integration/migrations/versions/47f10265b5d7_.py` & `flask-ligand-0.8.0/tests/integration/migrations/versions/47f10265b5d7_.py`

 * *Files identical despite different names*

### Comparing `flask-ligand-0.7.8/tests/integration/test_basic.py` & `flask-ligand-0.8.0/tests/integration/test_basic.py`

 * *Files identical despite different names*

### Comparing `flask-ligand-0.7.8/tests/unit/conftest.py` & `flask-ligand-0.8.0/tests/unit/conftest.py`

 * *Files identical despite different names*

### Comparing `flask-ligand-0.7.8/tests/unit/test_api_extension.py` & `flask-ligand-0.8.0/tests/unit/test_api_extension.py`

 * *Files identical despite different names*

### Comparing `flask-ligand-0.7.8/tests/unit/test_database_extension.py` & `flask-ligand-0.8.0/tests/unit/test_database_extension.py`

 * *Files identical despite different names*

### Comparing `flask-ligand-0.7.8/tests/unit/test_jwt_extension.py` & `flask-ligand-0.8.0/tests/unit/test_jwt_extension.py`

 * *Files identical despite different names*

### Comparing `flask-ligand-0.7.8/tests/unit/test_openapi_api.py` & `flask-ligand-0.8.0/tests/unit/test_openapi_api.py`

 * *Files identical despite different names*

### Comparing `flask-ligand-0.7.8/tests/unit/test_settings.py` & `flask-ligand-0.8.0/tests/unit/test_settings.py`

 * *Files identical despite different names*

