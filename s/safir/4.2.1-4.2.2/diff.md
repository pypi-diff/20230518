# Comparing `tmp/safir-4.2.1.tar.gz` & `tmp/safir-4.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "safir-4.2.1.tar", last modified: Wed May 17 20:28:46 2023, max compression
+gzip compressed data, was "safir-4.2.2.tar", last modified: Wed May 17 22:55:47 2023, max compression
```

## Comparing `safir-4.2.1.tar` & `safir-4.2.2.tar`

### file list

```diff
@@ -1,148 +1,150 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 20:28:46.505092 safir-4.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-05-17 20:28:30.000000 safir-4.2.1/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 20:28:46.485092 safir-4.2.1/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-05-17 20:28:30.000000 safir-4.2.1/.github/CODE_OF_CONDUCT
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-17 20:28:30.000000 safir-4.2.1/.github/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)      206 2023-05-17 20:28:30.000000 safir-4.2.1/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 20:28:46.485092 safir-4.2.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2522 2023-05-17 20:28:30.000000 safir-4.2.1/.github/workflows/ci.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-05-17 20:28:30.000000 safir-4.2.1/.github/workflows/periodic.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1853 2023-05-17 20:28:30.000000 safir-4.2.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      637 2023-05-17 20:28:30.000000 safir-4.2.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    16874 2023-05-17 20:28:30.000000 safir-4.2.1/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     1123 2023-05-17 20:28:30.000000 safir-4.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-05-17 20:28:30.000000 safir-4.2.1/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     3936 2023-05-17 20:28:46.505092 safir-4.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1537 2023-05-17 20:28:30.000000 safir-4.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 20:28:46.485092 safir-4.2.1/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-05-17 20:28:30.000000 safir-4.2.1/docs/_rst_epilog.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1825 2023-05-17 20:28:30.000000 safir-4.2.1/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)    16874 2023-05-17 20:28:30.000000 safir-4.2.1/docs/changelog.md
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-17 20:28:30.000000 safir-4.2.1/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 20:28:46.489092 safir-4.2.1/docs/dev/
--rw-r--r--   0 runner    (1001) docker     (123)     5660 2023-05-17 20:28:30.000000 safir-4.2.1/docs/dev/development.rst
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-05-17 20:28:30.000000 safir-4.2.1/docs/dev/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3379 2023-05-17 20:28:30.000000 safir-4.2.1/docs/dev/release.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-05-17 20:28:30.000000 safir-4.2.1/docs/documenteer.toml
--rw-r--r--   0 runner    (1001) docker     (123)      627 2023-05-17 20:28:30.000000 safir-4.2.1/docs/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 20:28:46.489092 safir-4.2.1/docs/user-guide/
--rw-r--r--   0 runner    (1001) docker     (123)    11297 2023-05-17 20:28:30.000000 safir-4.2.1/docs/user-guide/arq.rst
--rw-r--r--   0 runner    (1001) docker     (123)    22394 2023-05-17 20:28:30.000000 safir-4.2.1/docs/user-guide/database.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5115 2023-05-17 20:28:30.000000 safir-4.2.1/docs/user-guide/datetime.rst
--rw-r--r--   0 runner    (1001) docker     (123)     7691 2023-05-17 20:28:30.000000 safir-4.2.1/docs/user-guide/fastapi-errors.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3490 2023-05-17 20:28:30.000000 safir-4.2.1/docs/user-guide/gafaelfawr.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5495 2023-05-17 20:28:30.000000 safir-4.2.1/docs/user-guide/gcs.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 20:28:46.493092 safir-4.2.1/docs/user-guide/github-apps/
--rw-r--r--   0 runner    (1001) docker     (123)     2112 2023-05-17 20:28:30.000000 safir-4.2.1/docs/user-guide/github-apps/api-resources.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5904 2023-05-17 20:28:30.000000 safir-4.2.1/docs/user-guide/github-apps/create-a-github-client.rst
--rw-r--r--   0 runner    (1001) docker     (123)     8659 2023-05-17 20:28:30.000000 safir-4.2.1/docs/user-guide/github-apps/handling-webhooks.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-05-17 20:28:30.000000 safir-4.2.1/docs/user-guide/github-apps/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1992 2023-05-17 20:28:30.000000 safir-4.2.1/docs/user-guide/github-apps/webhook-models.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1954 2023-05-17 20:28:30.000000 safir-4.2.1/docs/user-guide/http-client.rst
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-05-17 20:28:30.000000 safir-4.2.1/docs/user-guide/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-05-17 20:28:30.000000 safir-4.2.1/docs/user-guide/ivoa.rst
--rw-r--r--   0 runner    (1001) docker     (123)    10042 2023-05-17 20:28:30.000000 safir-4.2.1/docs/user-guide/kubernetes.rst
--rw-r--r--   0 runner    (1001) docker     (123)     7140 2023-05-17 20:28:30.000000 safir-4.2.1/docs/user-guide/logging.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5267 2023-05-17 20:28:30.000000 safir-4.2.1/docs/user-guide/pydantic-redis.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4964 2023-05-17 20:28:30.000000 safir-4.2.1/docs/user-guide/pydantic.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6084 2023-05-17 20:28:30.000000 safir-4.2.1/docs/user-guide/set-up-from-template.rst
--rw-r--r--   0 runner    (1001) docker     (123)    14653 2023-05-17 20:28:30.000000 safir-4.2.1/docs/user-guide/slack-webhook.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4032 2023-05-17 20:28:30.000000 safir-4.2.1/docs/user-guide/uvicorn.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4926 2023-05-17 20:28:30.000000 safir-4.2.1/docs/user-guide/x-forwarded.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3736 2023-05-17 20:28:30.000000 safir-4.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-17 20:28:46.505092 safir-4.2.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 20:28:46.481092 safir-4.2.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 20:28:46.493092 safir-4.2.1/src/safir/
--rw-r--r--   0 runner    (1001) docker     (123)      552 2023-05-17 20:28:30.000000 safir-4.2.1/src/safir/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15368 2023-05-17 20:28:30.000000 safir-4.2.1/src/safir/arq.py
--rw-r--r--   0 runner    (1001) docker     (123)     1601 2023-05-17 20:28:30.000000 safir-4.2.1/src/safir/asyncio.py
--rw-r--r--   0 runner    (1001) docker     (123)    11751 2023-05-17 20:28:30.000000 safir-4.2.1/src/safir/database.py
--rw-r--r--   0 runner    (1001) docker     (123)     4139 2023-05-17 20:28:30.000000 safir-4.2.1/src/safir/datetime.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 20:28:46.497092 safir-4.2.1/src/safir/dependencies/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 20:28:30.000000 safir-4.2.1/src/safir/dependencies/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2914 2023-05-17 20:28:30.000000 safir-4.2.1/src/safir/dependencies/arq.py
--rw-r--r--   0 runner    (1001) docker     (123)     3641 2023-05-17 20:28:30.000000 safir-4.2.1/src/safir/dependencies/db_session.py
--rw-r--r--   0 runner    (1001) docker     (123)      884 2023-05-17 20:28:30.000000 safir-4.2.1/src/safir/dependencies/gafaelfawr.py
--rw-r--r--   0 runner    (1001) docker     (123)     1705 2023-05-17 20:28:30.000000 safir-4.2.1/src/safir/dependencies/http_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2116 2023-05-17 20:28:30.000000 safir-4.2.1/src/safir/dependencies/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     7784 2023-05-17 20:28:30.000000 safir-4.2.1/src/safir/fastapi.py
--rw-r--r--   0 runner    (1001) docker     (123)     3384 2023-05-17 20:28:30.000000 safir-4.2.1/src/safir/gcs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 20:28:46.497092 safir-4.2.1/src/safir/github/
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-05-17 20:28:30.000000 safir-4.2.1/src/safir/github/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3921 2023-05-17 20:28:30.000000 safir-4.2.1/src/safir/github/_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    11333 2023-05-17 20:28:30.000000 safir-4.2.1/src/safir/github/models.py
--rw-r--r--   0 runner    (1001) docker     (123)    10285 2023-05-17 20:28:30.000000 safir-4.2.1/src/safir/github/webhooks.py
--rw-r--r--   0 runner    (1001) docker     (123)      927 2023-05-17 20:28:30.000000 safir-4.2.1/src/safir/kubernetes.py
--rw-r--r--   0 runner    (1001) docker     (123)    10332 2023-05-17 20:28:30.000000 safir-4.2.1/src/safir/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     4895 2023-05-17 20:28:30.000000 safir-4.2.1/src/safir/metadata.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 20:28:46.497092 safir-4.2.1/src/safir/middleware/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 20:28:30.000000 safir-4.2.1/src/safir/middleware/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-05-17 20:28:30.000000 safir-4.2.1/src/safir/middleware/ivoa.py
--rw-r--r--   0 runner    (1001) docker     (123)     6227 2023-05-17 20:28:30.000000 safir-4.2.1/src/safir/middleware/x_forwarded.py
--rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-05-17 20:28:30.000000 safir-4.2.1/src/safir/models.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 20:28:30.000000 safir-4.2.1/src/safir/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     8575 2023-05-17 20:28:30.000000 safir-4.2.1/src/safir/pydantic.py
--rw-r--r--   0 runner    (1001) docker     (123)     7470 2023-05-17 20:28:30.000000 safir-4.2.1/src/safir/redis.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 20:28:46.497092 safir-4.2.1/src/safir/slack/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 20:28:30.000000 safir-4.2.1/src/safir/slack/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15576 2023-05-17 20:28:30.000000 safir-4.2.1/src/safir/slack/blockkit.py
--rw-r--r--   0 runner    (1001) docker     (123)     7360 2023-05-17 20:28:30.000000 safir-4.2.1/src/safir/slack/webhook.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 20:28:46.501092 safir-4.2.1/src/safir/testing/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 20:28:30.000000 safir-4.2.1/src/safir/testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10106 2023-05-17 20:28:30.000000 safir-4.2.1/src/safir/testing/gcs.py
--rw-r--r--   0 runner    (1001) docker     (123)    74799 2023-05-17 20:28:30.000000 safir-4.2.1/src/safir/testing/kubernetes.py
--rw-r--r--   0 runner    (1001) docker     (123)     2492 2023-05-17 20:28:30.000000 safir-4.2.1/src/safir/testing/slack.py
--rw-r--r--   0 runner    (1001) docker     (123)     5253 2023-05-17 20:28:30.000000 safir-4.2.1/src/safir/testing/uvicorn.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 20:28:46.493092 safir-4.2.1/src/safir.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3936 2023-05-17 20:28:46.000000 safir-4.2.1/src/safir.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3403 2023-05-17 20:28:46.000000 safir-4.2.1/src/safir.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 20:28:46.000000 safir-4.2.1/src/safir.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      425 2023-05-17 20:28:46.000000 safir-4.2.1/src/safir.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-17 20:28:46.000000 safir-4.2.1/src/safir.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 20:28:46.501092 safir-4.2.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 20:28:30.000000 safir-4.2.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      308 2023-05-17 20:28:30.000000 safir-4.2.1/tests/asyncio_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-05-17 20:28:30.000000 safir-4.2.1/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     6189 2023-05-17 20:28:30.000000 safir-4.2.1/tests/database_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2207 2023-05-17 20:28:30.000000 safir-4.2.1/tests/datetime_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 20:28:46.501092 safir-4.2.1/tests/dependencies/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 20:28:30.000000 safir-4.2.1/tests/dependencies/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5497 2023-05-17 20:28:30.000000 safir-4.2.1/tests/dependencies/arq_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2497 2023-05-17 20:28:30.000000 safir-4.2.1/tests/dependencies/db_session_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2099 2023-05-17 20:28:30.000000 safir-4.2.1/tests/dependencies/gafaelfawr_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-05-17 20:28:30.000000 safir-4.2.1/tests/dependencies/http_client_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2787 2023-05-17 20:28:30.000000 safir-4.2.1/tests/dependencies/logger_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2325 2023-05-17 20:28:30.000000 safir-4.2.1/tests/fastapi_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      860 2023-05-17 20:28:30.000000 safir-4.2.1/tests/gcs_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 20:28:46.501092 safir-4.2.1/tests/github/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 20:28:30.000000 safir-4.2.1/tests/github/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 20:28:46.485092 safir-4.2.1/tests/github/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 20:28:46.505092 safir-4.2.1/tests/github/data/webhooks/
--rw-r--r--   0 runner    (1001) docker     (123)    14626 2023-05-17 20:28:30.000000 safir-4.2.1/tests/github/data/webhooks/check_run_created.json
--rw-r--r--   0 runner    (1001) docker     (123)    10772 2023-05-17 20:28:30.000000 safir-4.2.1/tests/github/data/webhooks/check_suite_completed.json
--rw-r--r--   0 runner    (1001) docker     (123)     2906 2023-05-17 20:28:30.000000 safir-4.2.1/tests/github/data/webhooks/installation.json
--rw-r--r--   0 runner    (1001) docker     (123)     3337 2023-05-17 20:28:30.000000 safir-4.2.1/tests/github/data/webhooks/installation_repositories.json
--rw-r--r--   0 runner    (1001) docker     (123)    26334 2023-05-17 20:28:30.000000 safir-4.2.1/tests/github/data/webhooks/pull_request_event.json
--rw-r--r--   0 runner    (1001) docker     (123)     7917 2023-05-17 20:28:30.000000 safir-4.2.1/tests/github/data/webhooks/push_event.json
--rw-r--r--   0 runner    (1001) docker     (123)     3355 2023-05-17 20:28:30.000000 safir-4.2.1/tests/github/webhooks_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      418 2023-05-17 20:28:30.000000 safir-4.2.1/tests/kubernetes_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     9168 2023-05-17 20:28:30.000000 safir-4.2.1/tests/logging_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1342 2023-05-17 20:28:30.000000 safir-4.2.1/tests/metadata_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 20:28:46.505092 safir-4.2.1/tests/middleware/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 20:28:30.000000 safir-4.2.1/tests/middleware/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-05-17 20:28:30.000000 safir-4.2.1/tests/middleware/ivoa_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5774 2023-05-17 20:28:30.000000 safir-4.2.1/tests/middleware/x_forwarded_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      502 2023-05-17 20:28:30.000000 safir-4.2.1/tests/models_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4210 2023-05-17 20:28:30.000000 safir-4.2.1/tests/pydantic_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5042 2023-05-17 20:28:30.000000 safir-4.2.1/tests/redis_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      183 2023-05-17 20:28:30.000000 safir-4.2.1/tests/safir_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 20:28:46.505092 safir-4.2.1/tests/slack/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 20:28:30.000000 safir-4.2.1/tests/slack/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11319 2023-05-17 20:28:30.000000 safir-4.2.1/tests/slack/blockkit_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     8041 2023-05-17 20:28:30.000000 safir-4.2.1/tests/slack/webhook_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 20:28:46.505092 safir-4.2.1/tests/testing/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 20:28:30.000000 safir-4.2.1/tests/testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      623 2023-05-17 20:28:30.000000 safir-4.2.1/tests/testing/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     3897 2023-05-17 20:28:30.000000 safir-4.2.1/tests/testing/gcs_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    10018 2023-05-17 20:28:30.000000 safir-4.2.1/tests/testing/kubernetes_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2084 2023-05-17 20:28:30.000000 safir-4.2.1/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:55:47.243249 safir-4.2.2/
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-05-17 22:55:35.000000 safir-4.2.2/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:55:47.227249 safir-4.2.2/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-05-17 22:55:35.000000 safir-4.2.2/.github/CODE_OF_CONDUCT
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-17 22:55:35.000000 safir-4.2.2/.github/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)      206 2023-05-17 22:55:35.000000 safir-4.2.2/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:55:47.227249 safir-4.2.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2522 2023-05-17 22:55:35.000000 safir-4.2.2/.github/workflows/ci.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-05-17 22:55:35.000000 safir-4.2.2/.github/workflows/periodic.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1853 2023-05-17 22:55:35.000000 safir-4.2.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      637 2023-05-17 22:55:35.000000 safir-4.2.2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    18128 2023-05-17 22:55:35.000000 safir-4.2.2/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1123 2023-05-17 22:55:35.000000 safir-4.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-05-17 22:55:35.000000 safir-4.2.2/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     3936 2023-05-17 22:55:47.243249 safir-4.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1537 2023-05-17 22:55:35.000000 safir-4.2.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:55:47.227249 safir-4.2.2/changelog.d/
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-05-17 22:55:35.000000 safir-4.2.2/changelog.d/_template.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:55:47.227249 safir-4.2.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-05-17 22:55:35.000000 safir-4.2.2/docs/_rst_epilog.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1825 2023-05-17 22:55:35.000000 safir-4.2.2/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    18128 2023-05-17 22:55:35.000000 safir-4.2.2/docs/changelog.md
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-17 22:55:35.000000 safir-4.2.2/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:55:47.231248 safir-4.2.2/docs/dev/
+-rw-r--r--   0 runner    (1001) docker     (123)     5515 2023-05-17 22:55:35.000000 safir-4.2.2/docs/dev/development.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-05-17 22:55:35.000000 safir-4.2.2/docs/dev/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4936 2023-05-17 22:55:35.000000 safir-4.2.2/docs/dev/release.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-05-17 22:55:35.000000 safir-4.2.2/docs/documenteer.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      627 2023-05-17 22:55:35.000000 safir-4.2.2/docs/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:55:47.231248 safir-4.2.2/docs/user-guide/
+-rw-r--r--   0 runner    (1001) docker     (123)    11297 2023-05-17 22:55:35.000000 safir-4.2.2/docs/user-guide/arq.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    22394 2023-05-17 22:55:35.000000 safir-4.2.2/docs/user-guide/database.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5115 2023-05-17 22:55:35.000000 safir-4.2.2/docs/user-guide/datetime.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7691 2023-05-17 22:55:35.000000 safir-4.2.2/docs/user-guide/fastapi-errors.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3490 2023-05-17 22:55:35.000000 safir-4.2.2/docs/user-guide/gafaelfawr.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5495 2023-05-17 22:55:35.000000 safir-4.2.2/docs/user-guide/gcs.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:55:47.231248 safir-4.2.2/docs/user-guide/github-apps/
+-rw-r--r--   0 runner    (1001) docker     (123)     2112 2023-05-17 22:55:35.000000 safir-4.2.2/docs/user-guide/github-apps/api-resources.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5965 2023-05-17 22:55:35.000000 safir-4.2.2/docs/user-guide/github-apps/create-a-github-client.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     8659 2023-05-17 22:55:35.000000 safir-4.2.2/docs/user-guide/github-apps/handling-webhooks.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-05-17 22:55:35.000000 safir-4.2.2/docs/user-guide/github-apps/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2010 2023-05-17 22:55:35.000000 safir-4.2.2/docs/user-guide/github-apps/webhook-models.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1954 2023-05-17 22:55:35.000000 safir-4.2.2/docs/user-guide/http-client.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-05-17 22:55:35.000000 safir-4.2.2/docs/user-guide/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-05-17 22:55:35.000000 safir-4.2.2/docs/user-guide/ivoa.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    10042 2023-05-17 22:55:35.000000 safir-4.2.2/docs/user-guide/kubernetes.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7140 2023-05-17 22:55:35.000000 safir-4.2.2/docs/user-guide/logging.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5267 2023-05-17 22:55:35.000000 safir-4.2.2/docs/user-guide/pydantic-redis.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4964 2023-05-17 22:55:35.000000 safir-4.2.2/docs/user-guide/pydantic.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6084 2023-05-17 22:55:35.000000 safir-4.2.2/docs/user-guide/set-up-from-template.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    14653 2023-05-17 22:55:35.000000 safir-4.2.2/docs/user-guide/slack-webhook.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4032 2023-05-17 22:55:35.000000 safir-4.2.2/docs/user-guide/uvicorn.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4926 2023-05-17 22:55:35.000000 safir-4.2.2/docs/user-guide/x-forwarded.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4073 2023-05-17 22:55:35.000000 safir-4.2.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-17 22:55:47.243249 safir-4.2.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:55:47.227249 safir-4.2.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:55:47.235248 safir-4.2.2/src/safir/
+-rw-r--r--   0 runner    (1001) docker     (123)      552 2023-05-17 22:55:35.000000 safir-4.2.2/src/safir/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15368 2023-05-17 22:55:35.000000 safir-4.2.2/src/safir/arq.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1601 2023-05-17 22:55:35.000000 safir-4.2.2/src/safir/asyncio.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11751 2023-05-17 22:55:35.000000 safir-4.2.2/src/safir/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4139 2023-05-17 22:55:35.000000 safir-4.2.2/src/safir/datetime.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:55:47.235248 safir-4.2.2/src/safir/dependencies/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 22:55:35.000000 safir-4.2.2/src/safir/dependencies/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2914 2023-05-17 22:55:35.000000 safir-4.2.2/src/safir/dependencies/arq.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3641 2023-05-17 22:55:35.000000 safir-4.2.2/src/safir/dependencies/db_session.py
+-rw-r--r--   0 runner    (1001) docker     (123)      884 2023-05-17 22:55:35.000000 safir-4.2.2/src/safir/dependencies/gafaelfawr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1705 2023-05-17 22:55:35.000000 safir-4.2.2/src/safir/dependencies/http_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2116 2023-05-17 22:55:35.000000 safir-4.2.2/src/safir/dependencies/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7784 2023-05-17 22:55:35.000000 safir-4.2.2/src/safir/fastapi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3384 2023-05-17 22:55:35.000000 safir-4.2.2/src/safir/gcs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:55:47.235248 safir-4.2.2/src/safir/github/
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-05-17 22:55:35.000000 safir-4.2.2/src/safir/github/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3921 2023-05-17 22:55:35.000000 safir-4.2.2/src/safir/github/_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11333 2023-05-17 22:55:35.000000 safir-4.2.2/src/safir/github/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10236 2023-05-17 22:55:35.000000 safir-4.2.2/src/safir/github/webhooks.py
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-05-17 22:55:35.000000 safir-4.2.2/src/safir/kubernetes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10301 2023-05-17 22:55:35.000000 safir-4.2.2/src/safir/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4895 2023-05-17 22:55:35.000000 safir-4.2.2/src/safir/metadata.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:55:47.235248 safir-4.2.2/src/safir/middleware/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 22:55:35.000000 safir-4.2.2/src/safir/middleware/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-05-17 22:55:35.000000 safir-4.2.2/src/safir/middleware/ivoa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6227 2023-05-17 22:55:35.000000 safir-4.2.2/src/safir/middleware/x_forwarded.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-05-17 22:55:35.000000 safir-4.2.2/src/safir/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 22:55:35.000000 safir-4.2.2/src/safir/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     8575 2023-05-17 22:55:35.000000 safir-4.2.2/src/safir/pydantic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7470 2023-05-17 22:55:35.000000 safir-4.2.2/src/safir/redis.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:55:47.235248 safir-4.2.2/src/safir/slack/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 22:55:35.000000 safir-4.2.2/src/safir/slack/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15576 2023-05-17 22:55:35.000000 safir-4.2.2/src/safir/slack/blockkit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7360 2023-05-17 22:55:35.000000 safir-4.2.2/src/safir/slack/webhook.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:55:47.235248 safir-4.2.2/src/safir/testing/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 22:55:35.000000 safir-4.2.2/src/safir/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10106 2023-05-17 22:55:35.000000 safir-4.2.2/src/safir/testing/gcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    74785 2023-05-17 22:55:35.000000 safir-4.2.2/src/safir/testing/kubernetes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2492 2023-05-17 22:55:35.000000 safir-4.2.2/src/safir/testing/slack.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5253 2023-05-17 22:55:35.000000 safir-4.2.2/src/safir/testing/uvicorn.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:55:47.235248 safir-4.2.2/src/safir.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3936 2023-05-17 22:55:47.000000 safir-4.2.2/src/safir.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3428 2023-05-17 22:55:47.000000 safir-4.2.2/src/safir.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 22:55:47.000000 safir-4.2.2/src/safir.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2023-05-17 22:55:47.000000 safir-4.2.2/src/safir.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-17 22:55:47.000000 safir-4.2.2/src/safir.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:55:47.239249 safir-4.2.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 22:55:35.000000 safir-4.2.2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-05-17 22:55:35.000000 safir-4.2.2/tests/asyncio_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-05-17 22:55:35.000000 safir-4.2.2/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6189 2023-05-17 22:55:35.000000 safir-4.2.2/tests/database_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2207 2023-05-17 22:55:35.000000 safir-4.2.2/tests/datetime_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:55:47.239249 safir-4.2.2/tests/dependencies/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 22:55:35.000000 safir-4.2.2/tests/dependencies/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5497 2023-05-17 22:55:35.000000 safir-4.2.2/tests/dependencies/arq_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2497 2023-05-17 22:55:35.000000 safir-4.2.2/tests/dependencies/db_session_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2099 2023-05-17 22:55:35.000000 safir-4.2.2/tests/dependencies/gafaelfawr_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-05-17 22:55:35.000000 safir-4.2.2/tests/dependencies/http_client_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2787 2023-05-17 22:55:35.000000 safir-4.2.2/tests/dependencies/logger_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2325 2023-05-17 22:55:35.000000 safir-4.2.2/tests/fastapi_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      860 2023-05-17 22:55:35.000000 safir-4.2.2/tests/gcs_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:55:47.239249 safir-4.2.2/tests/github/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 22:55:35.000000 safir-4.2.2/tests/github/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:55:47.227249 safir-4.2.2/tests/github/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:55:47.239249 safir-4.2.2/tests/github/data/webhooks/
+-rw-r--r--   0 runner    (1001) docker     (123)    14626 2023-05-17 22:55:35.000000 safir-4.2.2/tests/github/data/webhooks/check_run_created.json
+-rw-r--r--   0 runner    (1001) docker     (123)    10772 2023-05-17 22:55:35.000000 safir-4.2.2/tests/github/data/webhooks/check_suite_completed.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2906 2023-05-17 22:55:35.000000 safir-4.2.2/tests/github/data/webhooks/installation.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3337 2023-05-17 22:55:35.000000 safir-4.2.2/tests/github/data/webhooks/installation_repositories.json
+-rw-r--r--   0 runner    (1001) docker     (123)    26334 2023-05-17 22:55:35.000000 safir-4.2.2/tests/github/data/webhooks/pull_request_event.json
+-rw-r--r--   0 runner    (1001) docker     (123)     7917 2023-05-17 22:55:35.000000 safir-4.2.2/tests/github/data/webhooks/push_event.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3355 2023-05-17 22:55:35.000000 safir-4.2.2/tests/github/webhooks_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      418 2023-05-17 22:55:35.000000 safir-4.2.2/tests/kubernetes_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9168 2023-05-17 22:55:35.000000 safir-4.2.2/tests/logging_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1342 2023-05-17 22:55:35.000000 safir-4.2.2/tests/metadata_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:55:47.239249 safir-4.2.2/tests/middleware/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 22:55:35.000000 safir-4.2.2/tests/middleware/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-05-17 22:55:35.000000 safir-4.2.2/tests/middleware/ivoa_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5774 2023-05-17 22:55:35.000000 safir-4.2.2/tests/middleware/x_forwarded_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      502 2023-05-17 22:55:35.000000 safir-4.2.2/tests/models_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4210 2023-05-17 22:55:35.000000 safir-4.2.2/tests/pydantic_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5042 2023-05-17 22:55:35.000000 safir-4.2.2/tests/redis_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-05-17 22:55:35.000000 safir-4.2.2/tests/safir_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:55:47.239249 safir-4.2.2/tests/slack/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 22:55:35.000000 safir-4.2.2/tests/slack/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11319 2023-05-17 22:55:35.000000 safir-4.2.2/tests/slack/blockkit_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8041 2023-05-17 22:55:35.000000 safir-4.2.2/tests/slack/webhook_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:55:47.239249 safir-4.2.2/tests/testing/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 22:55:35.000000 safir-4.2.2/tests/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-05-17 22:55:35.000000 safir-4.2.2/tests/testing/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3897 2023-05-17 22:55:35.000000 safir-4.2.2/tests/testing/gcs_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10018 2023-05-17 22:55:35.000000 safir-4.2.2/tests/testing/kubernetes_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2084 2023-05-17 22:55:35.000000 safir-4.2.2/tox.ini
```

### Comparing `safir-4.2.1/.github/workflows/ci.yaml` & `safir-4.2.2/.github/workflows/ci.yaml`

 * *Files identical despite different names*

### Comparing `safir-4.2.1/.github/workflows/periodic.yaml` & `safir-4.2.2/.github/workflows/periodic.yaml`

 * *Files identical despite different names*

### Comparing `safir-4.2.1/.gitignore` & `safir-4.2.2/.gitignore`

 * *Files identical despite different names*

### Comparing `safir-4.2.1/.pre-commit-config.yaml` & `safir-4.2.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `safir-4.2.1/CHANGELOG.md` & `safir-4.2.2/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,45 @@
 # Change log
 
-<!--
-Headline template:
-X.Y.Z (YYYY-MM-DD)
--->
+All notable changes to Safir will be documented in this file.
 
-## 4.2.0 (unreleased)
+Versioning follows [semver](https://semver.org/).
+
+This project uses [scriv](https://scriv.readthedocs.io/en/stable/) to maintain the change log.
+Changes for the upcoming release can be found in [changelog.d](https://github.com/lsst-sqre/safir/tree/main/changelog.d/).
+
+<!-- scriv-insert-here -->
+
+<a id='changelog-4.2.2'></a>
+## 4.2.2 (2023-05-17)
+
+### Bug fixes
+
+- Revert the documentation change in 4.2.1 to restore cross-references, since the docs-linkcheck failure appears to be a false positive.
+
+### Other changes
+
+- Safir now uses [scriv](https://scriv.readthedocs.io/en/latest/) to maintain its change log.
+
+## 4.2.1 (2023-05-17)
+
+### Bug fixes
+
+- Fix syntax of literals in the `MockKubernetesApi` docstring.
+
+## 4.2.0 (2023-05-17)
 
 ### New features
 
+- Add create, delete, read, list (with watches), and (limited) patch support for `Ingress` objects to the mock Kubernetes API.
+- Add create, delete, read, and list (with watches) support for `Job` objects to the mock Kuberntes API, and mock the `BatchV1Api`.
+- Add delete, read, and list (with watches) support for `Service` objects to the mock Kubernetes API.
+- Add support for label selectors to `list_namespaced_pod` in the mock Kubernetes API.
 - Add `create_namespaced_persistent_volume_claim` to the mock Kubernetes API for testing.
+- Add support for deleting custom resources to the mock Kubernetes API.
 
 ### Bug fixes
 
 - `SlackWebException` now extracts the method and URL of the request from more httpx exceptions, and avoids exceptions when the request information is not present.
 
 ## 4.1.0 (2023-05-08)
```

### Comparing `safir-4.2.1/LICENSE` & `safir-4.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `safir-4.2.1/PKG-INFO` & `safir-4.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: safir
-Version: 4.2.1
+Version: 4.2.2
 Summary: The Rubin Observatory SQuaRE framework for FastAPI services.
 Author-email: "Association of Universities for Research in Astronomy, Inc. (AURA)" <sqre-admin@lists.lsst.org>
 License: MIT License
         
         Copyright (c) 2020 Association of Universities for Research in Astronomy, Inc. (AURA)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `safir-4.2.1/README.md` & `safir-4.2.2/README.md`

 * *Files identical despite different names*

### Comparing `safir-4.2.1/docs/_rst_epilog.rst` & `safir-4.2.2/docs/_rst_epilog.rst`

 * *Files 8% similar despite different names*

```diff
@@ -6,18 +6,20 @@
 .. _fastapi_safir_app: https://github.com/lsst/templates/tree/main/project_templates/fastapi_safir_app
 .. _Gafaelfawr: https://gafaelfawr.lsst.io/
 .. _Gidgethub: https://gidgethub.readthedocs.io/en/latest/
 .. _HTTPX: https://www.python-httpx.org/
 .. _mypy: https://www.mypy-lang.org
 .. _Phalanx: https://phalanx.lsst.io
 .. _pre-commit: https://pre-commit.com
-.. _Pydantic: https://docs.pydantic.dev/
+.. _Pydantic: https://docs.pydantic.dev/latest/
 .. _PyPI: https://pypi.org/project/safir/
 .. _pytest: https://docs.pytest.org/en/latest/
 .. _redis-py: https://redis.readthedocs.io/en/stable/
 .. _respx: https://lundberg.github.io/respx/
 .. _Roundtable: https://roundtable.lsst.io
+.. _scriv: https://scriv.readthedocs.io/en/stable/
+.. _semver: https://semver.org/
 .. _SQLAlchemy: https://www.sqlalchemy.org/
 .. _structlog: https://www.structlog.org/en/stable/
 .. _templatekit: https://templatekit.lsst.io
 .. _tox: https://tox.wiki/en/latest/
 .. _Uvicorn: https://www.uvicorn.org/
```

### Comparing `safir-4.2.1/docs/api.rst` & `safir-4.2.2/docs/api.rst`

 * *Files identical despite different names*

### Comparing `safir-4.2.1/docs/changelog.md` & `safir-4.2.2/docs/changelog.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,45 @@
 # Change log
 
-<!--
-Headline template:
-X.Y.Z (YYYY-MM-DD)
--->
+All notable changes to Safir will be documented in this file.
 
-## 4.2.0 (unreleased)
+Versioning follows [semver](https://semver.org/).
+
+This project uses [scriv](https://scriv.readthedocs.io/en/stable/) to maintain the change log.
+Changes for the upcoming release can be found in [changelog.d](https://github.com/lsst-sqre/safir/tree/main/changelog.d/).
+
+<!-- scriv-insert-here -->
+
+<a id='changelog-4.2.2'></a>
+## 4.2.2 (2023-05-17)
+
+### Bug fixes
+
+- Revert the documentation change in 4.2.1 to restore cross-references, since the docs-linkcheck failure appears to be a false positive.
+
+### Other changes
+
+- Safir now uses [scriv](https://scriv.readthedocs.io/en/latest/) to maintain its change log.
+
+## 4.2.1 (2023-05-17)
+
+### Bug fixes
+
+- Fix syntax of literals in the `MockKubernetesApi` docstring.
+
+## 4.2.0 (2023-05-17)
 
 ### New features
 
+- Add create, delete, read, list (with watches), and (limited) patch support for `Ingress` objects to the mock Kubernetes API.
+- Add create, delete, read, and list (with watches) support for `Job` objects to the mock Kuberntes API, and mock the `BatchV1Api`.
+- Add delete, read, and list (with watches) support for `Service` objects to the mock Kubernetes API.
+- Add support for label selectors to `list_namespaced_pod` in the mock Kubernetes API.
 - Add `create_namespaced_persistent_volume_claim` to the mock Kubernetes API for testing.
+- Add support for deleting custom resources to the mock Kubernetes API.
 
 ### Bug fixes
 
 - `SlackWebException` now extracts the method and URL of the request from more httpx exceptions, and avoids exceptions when the request information is not present.
 
 ## 4.1.0 (2023-05-08)
```

### Comparing `safir-4.2.1/docs/dev/development.rst` & `safir-4.2.2/docs/dev/development.rst`

 * *Files 14% similar despite different names*

```diff
@@ -102,44 +102,35 @@
 The build documentation is located in the :file:`docs/_build/html` directory.
 
 .. _dev-change-log:
 
 Updating the change log
 =======================
 
-Each pull request should update the change log (:file:`CHANGELOG.md`).
-Add a description of new features and fixes as list items under a section at the top of the change log, using ``unreleased`` for the date portion.
-The version number for that heading should be chosen or updated based on the semver_ rules.
+Safir uses scriv_ to maintain its change log.
 
-.. _semver: https://semver.org/
+When preparing a pull request, run :command:`scriv create`.
+This will create a change log fragment in :file:`changelog.d`.
+Edit that fragment, removing the sections that do not apply and adding entries fo this pull request.
+You can pass the ``--edit`` flag to :command:`scriv create` to open the created fragment automatically in an editor.
 
-.. code-block:: markdown
+Change log entries use the following sections:
 
-   ## X.Y.Z (unreleased)
-
-   ### Subheading (see below)
-
-   - Description of the feature or fix.
-
-All changelog entries should be divided into sections (each starting with ``###``) chosen from the following:
-
-- **Backward-incompatible changes** (also increase the major version except in unusual cases)
-- **New features** (also increase the minor version except in unusual cases)
+- **Backward-incompatible changes**
+- **New features**
 - **Bug fixes**
-- **Other changes** (which are mostly new features that are not significant enough to call attention to, such as logging formatting changes or updates to the documentation)
-
-If the exact version and release date is known (:doc:`because a release is being prepared <release>`), the section header is formatted as:
-
-.. code-block:: markdown
+- **Other changes** (for minor, patch-level changes that are not bug fixes, such as logging formatting changes or updates to the documentation)
 
-   ## X.Y.Z (YYYY-MM-DD)
+These entries will eventually be cut and pasted into the release description for the next release, so the Markdown for the change descriptions should be compatible with GitHub's Markdown conventions for the release description.
+Specifically:
 
-Each entry in the change log should be on one line without line breaks, even though this violates the normal rule of putting a newline after each sentence.
-This allows the whole change log entry to be copied and pasted into the GitHub release page when creating a release.
-Unfortunately, GitHub Markdown preserves line breaks after sentences as hard line breaks when rendering the description of a release.
+- Each bullet point should be entirely on one line, even if it contains multiple sentences.
+  This is an exception to the normal documentation convention of a newline after each sentence.
+  Unfortunately, GitHub interprets those newlines as hard line breaks, so they would result in an ugly release description.
+- Avoid using too much complex markup, such as nested bullet lists, since the formatting in the GitHub release description may not be what you expect and manually editing it is tedious.
 
 .. _style-guide:
 
 Style guide
 ===========
 
 Code
```

### Comparing `safir-4.2.1/docs/documenteer.toml` & `safir-4.2.2/docs/documenteer.toml`

 * *Files identical despite different names*

### Comparing `safir-4.2.1/docs/index.rst` & `safir-4.2.2/docs/index.rst`

 * *Files identical despite different names*

### Comparing `safir-4.2.1/docs/user-guide/arq.rst` & `safir-4.2.2/docs/user-guide/arq.rst`

 * *Files identical despite different names*

### Comparing `safir-4.2.1/docs/user-guide/database.rst` & `safir-4.2.2/docs/user-guide/database.rst`

 * *Files identical despite different names*

### Comparing `safir-4.2.1/docs/user-guide/datetime.rst` & `safir-4.2.2/docs/user-guide/datetime.rst`

 * *Files identical despite different names*

### Comparing `safir-4.2.1/docs/user-guide/fastapi-errors.rst` & `safir-4.2.2/docs/user-guide/fastapi-errors.rst`

 * *Files identical despite different names*

### Comparing `safir-4.2.1/docs/user-guide/gafaelfawr.rst` & `safir-4.2.2/docs/user-guide/gafaelfawr.rst`

 * *Files identical despite different names*

### Comparing `safir-4.2.1/docs/user-guide/gcs.rst` & `safir-4.2.2/docs/user-guide/gcs.rst`

 * *Files identical despite different names*

### Comparing `safir-4.2.1/docs/user-guide/github-apps/api-resources.rst` & `safir-4.2.2/docs/user-guide/github-apps/api-resources.rst`

 * *Files identical despite different names*

### Comparing `safir-4.2.1/docs/user-guide/github-apps/create-a-github-client.rst` & `safir-4.2.2/docs/user-guide/github-apps/create-a-github-client.rst`

 * *Files 2% similar despite different names*

```diff
@@ -6,32 +6,32 @@
 
 Gidgethub_ is the recommended library for building GitHub integrations with Safir applications.
 To create a Gidgethub client for a GitHub App, Safir provides the `safir.github.GitHubAppClientFactory` class.
 
 .. note::
 
    GitHub provides multiple way of building integrations, each with slightly different capabilities and authentication flows.
-   The `GitHubAppClientFactory` is designed to work with `GitHub Apps <https://developer.github.com/apps/building-github-apps/>`__, which are the recommended way of building integrations.
+   The `GitHubAppClientFactory` is designed to work with `GitHub Apps <https://docs.github.com/en/apps/creating-github-apps/setting-up-a-github-app>`__, which are the recommended way of building integrations.
    GitHub Apps are specifically installed into an organization or user account, and can be granted access to specific repositories.
 
    Another common way of building an integration is as an OAuth app (particularly before the introduction of GitHub Apps).
    OAuth app integrations are still useful if your app needs to access a user's GitHub account (such as to provide a GitHub login for your application).
    However, it is not generally recommended since it requires users to grant your app access to their account.
 
    A third way of building a GitHub integration is to authenticate as a user with a personal access token (usually for a bot account).
    GitHub Apps generally replace this use case for all but the simplest integrations.
    Note in particular that a GitHub App can be `authenticated on behalf of a user <https://docs.github.com/en/apps/creating-github-apps/authenticating-with-a-github-app/authenticating-with-a-github-app-on-behalf-of-a-user>`__.
 
-   For a comparison of the different ways of building integrations, see `GitHub's documentation <https://docs.github.com/en/apps/creating-github-apps/creating-github-apps/about-apps>`__.
+   For a comparison of the different ways of building integrations, see `GitHub's documentation <https://docs.github.com/en/apps/creating-github-apps/setting-up-a-github-app/about-creating-github-apps>`__.
 
 Setting up the factory
 ======================
 
 The `GitHubAppClientFactory` requires information about the GitHub App, which you will normally include in your application's configuration, and an instance of `httpx.AsyncClient`, which your application will typically create with the `~safir.dependencies.http_client.http_client_dependency` dependency (see :doc:`../http-client`).
-For information about creating a GitHub App, retrieving its App ID and generating a private key, see `GitHub's documentation <https://developer.github.com/apps/building-github-apps/creating-a-github-app/>`__.
+For information about creating a GitHub App, retrieving its App ID and generating a private key, see `GitHub's documentation <https://docs.github.com/en/apps/creating-github-apps/setting-up-a-github-app/creating-a-github-app>`__.
 
 .. code-block:: python
 
    from pydantic import BaseSettings, Field, SecretStr
 
    from safir.github import GitHubAppClientFactory
```

### Comparing `safir-4.2.1/docs/user-guide/github-apps/handling-webhooks.rst` & `safir-4.2.2/docs/user-guide/github-apps/handling-webhooks.rst`

 * *Files identical despite different names*

### Comparing `safir-4.2.1/docs/user-guide/github-apps/index.rst` & `safir-4.2.2/docs/user-guide/github-apps/index.rst`

 * *Files identical despite different names*

### Comparing `safir-4.2.1/docs/user-guide/github-apps/webhook-models.rst` & `safir-4.2.2/docs/user-guide/github-apps/webhook-models.rst`

 * *Files 6% similar despite different names*

```diff
@@ -17,25 +17,25 @@
 =============
 
 .. list-table::
    :header-rows: 1
 
    * - Event
      - Model
-   * - `check_run <https://docs.github.com/webhooks-and-events/webhooks/webhook-events-and-payloads#check_run>`__
+   * - `check_run <https://docs.github.com/en/webhooks-and-events/webhooks/webhook-events-and-payloads#check_run>`__
      - `~safir.github.webhooks.GitHubCheckRunEventModel`
-   * - `check_suite <https://docs.github.com/webhooks-and-events/webhooks/webhook-events-and-payloads#check_suite>`__
+   * - `check_suite <https://docs.github.com/en/webhooks-and-events/webhooks/webhook-events-and-payloads#check_suite>`__
      - `~safir.github.webhooks.GitHubCheckSuiteEventModel`
-   * - `installation <https://docs.github.com/webhooks-and-events/webhooks/webhook-events-and-payloads#installation>`__
+   * - `installation <https://docs.github.com/en/webhooks-and-events/webhooks/webhook-events-and-payloads#installation>`__
      - `~safir.github.webhooks.GitHubAppInstallationEventModel`
-   * - `installation_repositories <https://docs.github.com/webhooks-and-events/webhooks/webhook-events-and-payloads#installation_repositories>`__
+   * - `installation_repositories <https://docs.github.com/en/webhooks-and-events/webhooks/webhook-events-and-payloads#installation_repositories>`__
      - `~safir.github.webhooks.GitHubAppInstallationRepositoriesEventModel`
-   * - `pull_request <https://docs.github.com/webhooks-and-events/webhooks/webhook-events-and-payloads#pull_request>`__
+   * - `pull_request <https://docs.github.com/en/webhooks-and-events/webhooks/webhook-events-and-payloads#pull_request>`__
      - `~safir.github.webhooks.GitHubPullRequestEventModel`
-   * - `push <https://docs.github.com/webhooks-and-events/webhooks/webhook-events-and-payloads#push>`__
+   * - `push <https://docs.github.com/en/webhooks-and-events/webhooks/webhook-events-and-payloads#push>`__
      - `~safir.github.webhooks.GitHubPushEventModel`
 
 Related documentation
 =====================
 
 - :doc:`api-resources`
 - :doc:`handling-webhooks`
```

### Comparing `safir-4.2.1/docs/user-guide/http-client.rst` & `safir-4.2.2/docs/user-guide/http-client.rst`

 * *Files identical despite different names*

### Comparing `safir-4.2.1/docs/user-guide/ivoa.rst` & `safir-4.2.2/docs/user-guide/ivoa.rst`

 * *Files identical despite different names*

### Comparing `safir-4.2.1/docs/user-guide/kubernetes.rst` & `safir-4.2.2/docs/user-guide/kubernetes.rst`

 * *Files identical despite different names*

### Comparing `safir-4.2.1/docs/user-guide/logging.rst` & `safir-4.2.2/docs/user-guide/logging.rst`

 * *Files identical despite different names*

### Comparing `safir-4.2.1/docs/user-guide/pydantic-redis.rst` & `safir-4.2.2/docs/user-guide/pydantic-redis.rst`

 * *Files identical despite different names*

### Comparing `safir-4.2.1/docs/user-guide/pydantic.rst` & `safir-4.2.2/docs/user-guide/pydantic.rst`

 * *Files identical despite different names*

### Comparing `safir-4.2.1/docs/user-guide/set-up-from-template.rst` & `safir-4.2.2/docs/user-guide/set-up-from-template.rst`

 * *Files identical despite different names*

### Comparing `safir-4.2.1/docs/user-guide/slack-webhook.rst` & `safir-4.2.2/docs/user-guide/slack-webhook.rst`

 * *Files identical despite different names*

### Comparing `safir-4.2.1/docs/user-guide/uvicorn.rst` & `safir-4.2.2/docs/user-guide/uvicorn.rst`

 * *Files identical despite different names*

### Comparing `safir-4.2.1/docs/user-guide/x-forwarded.rst` & `safir-4.2.2/docs/user-guide/x-forwarded.rst`

 * *Files identical despite different names*

### Comparing `safir-4.2.1/pyproject.toml` & `safir-4.2.2/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -46,14 +46,15 @@
     "flake8",
     "mypy",
     "pre-commit",
     "psycopg2",
     "pytest",
     "pytest-asyncio",
     "respx",
+    "scriv",
     "sqlalchemy[mypy]",
     "types-redis",
     "uvicorn",
     # documentation
     "documenteer[guide]>=0.7.0b2",
     "autodoc_pydantic",
 ]
@@ -164,7 +165,20 @@
 warn_unused_ignores = true
 
 [tool.pydantic-mypy]
 init_forbid_extra = true
 init_typed = true
 warn_required_dynamic_aliases = true
 warn_untyped_fields = true
+
+[tool.scriv]
+categories = [
+    "Backwards-incompatible changes",
+    "New features",
+    "Bug fixes",
+    "Other changes",
+]
+entry_title_template = "{{ version }} ({{ date.strftime('%Y-%m-%d') }})"
+format = "md"
+md_header_level = "2"
+new_fragment_template = "file:changelog.d/_template.md"
+skip_fragments = "_template.md"
```

### Comparing `safir-4.2.1/src/safir/__init__.py` & `safir-4.2.2/src/safir/__init__.py`

 * *Files identical despite different names*

### Comparing `safir-4.2.1/src/safir/arq.py` & `safir-4.2.2/src/safir/arq.py`

 * *Files identical despite different names*

### Comparing `safir-4.2.1/src/safir/asyncio.py` & `safir-4.2.2/src/safir/asyncio.py`

 * *Files identical despite different names*

### Comparing `safir-4.2.1/src/safir/database.py` & `safir-4.2.2/src/safir/database.py`

 * *Files identical despite different names*

### Comparing `safir-4.2.1/src/safir/datetime.py` & `safir-4.2.2/src/safir/datetime.py`

 * *Files identical despite different names*

### Comparing `safir-4.2.1/src/safir/dependencies/arq.py` & `safir-4.2.2/src/safir/dependencies/arq.py`

 * *Files identical despite different names*

### Comparing `safir-4.2.1/src/safir/dependencies/db_session.py` & `safir-4.2.2/src/safir/dependencies/db_session.py`

 * *Files identical despite different names*

### Comparing `safir-4.2.1/src/safir/dependencies/gafaelfawr.py` & `safir-4.2.2/src/safir/dependencies/gafaelfawr.py`

 * *Files identical despite different names*

### Comparing `safir-4.2.1/src/safir/dependencies/http_client.py` & `safir-4.2.2/src/safir/dependencies/http_client.py`

 * *Files identical despite different names*

### Comparing `safir-4.2.1/src/safir/dependencies/logger.py` & `safir-4.2.2/src/safir/dependencies/logger.py`

 * *Files identical despite different names*

### Comparing `safir-4.2.1/src/safir/fastapi.py` & `safir-4.2.2/src/safir/fastapi.py`

 * *Files identical despite different names*

### Comparing `safir-4.2.1/src/safir/gcs.py` & `safir-4.2.2/src/safir/gcs.py`

 * *Files identical despite different names*

### Comparing `safir-4.2.1/src/safir/github/_client.py` & `safir-4.2.2/src/safir/github/_client.py`

 * *Files identical despite different names*

### Comparing `safir-4.2.1/src/safir/github/models.py` & `safir-4.2.2/src/safir/github/models.py`

 * *Files identical despite different names*

### Comparing `safir-4.2.1/src/safir/github/webhooks.py` & `safir-4.2.2/src/safir/github/webhooks.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,15 +38,15 @@
     id: str = Field(description="The installation ID.")
 
 
 class GitHubPushEventModel(BaseModel):
     """A Pydantic model for the ``push`` event webhook when a commit or
     tag is pushed.
 
-    https://docs.github.com/webhooks-and-events/webhooks/webhook-events-and-payloads#push
+    https://docs.github.com/en/webhooks-and-events/webhooks/webhook-events-and-payloads#push
     """
 
     repository: GitHubRepositoryModel = Field(
         description="The repository that was pushed to."
     )
 
     installation: GitHubAppInstallationModel = Field(
@@ -70,15 +70,15 @@
     )
 
 
 class GitHubAppInstallationEventRepoModel(BaseModel):
     """A pydantic model for repository objects used by
     `GitHubAppInstallationRepositoriesEventModel`.
 
-    https://docs.github.com/webhooks-and-events/webhooks/webhook-events-and-payloads#installation
+    https://docs.github.com/en/webhooks-and-events/webhooks/webhook-events-and-payloads#installation
     """
 
     name: str = Field(
         description="The name of the repository, e.g. 'times-square'."
     )
 
     full_name: str = Field(
@@ -115,15 +115,15 @@
     account.
     """
 
 
 class GitHubAppInstallationEventModel(BaseModel):
     """A Pydantic model for an ``installation`` webhook.
 
-    https://docs.github.com/en/developers/webhooks-and-events/webhooks/webhook-events-and-payloads#installation
+    https://docs.github.com/en/webhooks-and-events/webhooks/webhook-events-and-payloads#installation
     """
 
     action: GitHubAppInstallationEventAction = Field(
         description="Action performed."
     )
 
     repositories: list[GitHubAppInstallationEventRepoModel] = Field(
@@ -146,15 +146,15 @@
     #: Someone removed a repository from an installation.
     removed = "removed"
 
 
 class GitHubAppInstallationRepositoriesEventModel(BaseModel):
     """A Pydantic model for a ``installation_repositories`` webhook.
 
-    https://docs.github.com/en/developers/webhooks-and-events/webhooks/webhook-events-and-payloads#installation_repositories
+    https://docs.github.com/en/webhooks-and-events/webhooks/webhook-events-and-payloads#installation_repositories
     """
 
     action: GitHubAppInstallationRepositoriesEventAction = Field(
         description="Action performed on the installation."
     )
 
     repositories_added: list[GitHubAppInstallationEventRepoModel] = Field(
@@ -240,15 +240,15 @@
     unlocked = "unlocked"
     """Conversation on a pull request was unlocked."""
 
 
 class GitHubPullRequestEventModel(BaseModel):
     """A Pydantic model for a ``pull_request`` webhook.
 
-    https://docs.github.com/en/developers/webhooks-and-events/webhooks/webhook-events-and-payloads#pull_request
+    https://docs.github.com/en/webhooks-and-events/webhooks/webhook-events-and-payloads#pull_request
     """
 
     repository: GitHubRepositoryModel = Field(
         description="The repository that the pull request was opened against."
     )
 
     installation: GitHubAppInstallationModel = Field(
@@ -282,15 +282,15 @@
     rerequested = "rerequested"
     """Someone requested to re-run the check runs in a check suite."""
 
 
 class GitHubCheckSuiteEventModel(BaseModel):
     """A Pydantic model for the ``check_suite`` webhook payload.
 
-    https://docs.github.com/en/developers/webhooks-and-events/webhooks/webhook-events-and-payloads#check_suite
+    https://docs.github.com/en/webhooks-and-events/webhooks/webhook-events-and-payloads#check_suite
     """
 
     action: GitHubCheckSuiteEventAction = Field(
         description="The action performed.",
     )
 
     check_suite: GitHubCheckSuiteModel = Field(
@@ -325,15 +325,15 @@
     rerequested = "rerequested"
     """Someone requested to re-run a check run."""
 
 
 class GitHubCheckRunEventModel(BaseModel):
     """A Pydantic model for the ``check_run`` webhook payload.
 
-    https://docs.github.com/en/developers/webhooks-and-events/webhooks/webhook-events-and-payloads#check_run
+    https://docs.github.com/en/webhooks-and-events/webhooks/webhook-events-and-payloads#check_run
     """
 
     action: GitHubCheckRunEventAction = Field(
         description="The action that was performed.",
     )
 
     repository: GitHubRepositoryModel = Field(
```

### Comparing `safir-4.2.1/src/safir/kubernetes.py` & `safir-4.2.2/src/safir/kubernetes.py`

 * *Files identical despite different names*

### Comparing `safir-4.2.1/src/safir/logging.py` & `safir-4.2.2/src/safir/logging.py`

 * *Files 2% similar despite different names*

```diff
@@ -117,15 +117,15 @@
         or a case-insensitive string.
     add_timestamp
         Whether to add an ISO-format timestamp to each log message.
 
     Notes
     -----
     This function helps you configure a useful logging set up for your
-    application that's based on `structlog <https://www.structlog.org>`__.
+    application that's based on structlog_.
 
     First, it configures the logger for your application to log to STDOUT.
     Second, it configures the formatting of your log messages through
     structlog.
 
     In development mode, messages are key-value formatted, like this:
```

### Comparing `safir-4.2.1/src/safir/metadata.py` & `safir-4.2.2/src/safir/metadata.py`

 * *Files identical despite different names*

### Comparing `safir-4.2.1/src/safir/middleware/ivoa.py` & `safir-4.2.2/src/safir/middleware/ivoa.py`

 * *Files identical despite different names*

### Comparing `safir-4.2.1/src/safir/middleware/x_forwarded.py` & `safir-4.2.2/src/safir/middleware/x_forwarded.py`

 * *Files identical despite different names*

### Comparing `safir-4.2.1/src/safir/models.py` & `safir-4.2.2/src/safir/models.py`

 * *Files identical despite different names*

### Comparing `safir-4.2.1/src/safir/pydantic.py` & `safir-4.2.2/src/safir/pydantic.py`

 * *Files identical despite different names*

### Comparing `safir-4.2.1/src/safir/redis.py` & `safir-4.2.2/src/safir/redis.py`

 * *Files identical despite different names*

### Comparing `safir-4.2.1/src/safir/slack/blockkit.py` & `safir-4.2.2/src/safir/slack/blockkit.py`

 * *Files identical despite different names*

### Comparing `safir-4.2.1/src/safir/slack/webhook.py` & `safir-4.2.2/src/safir/slack/webhook.py`

 * *Files identical despite different names*

### Comparing `safir-4.2.1/src/safir/testing/gcs.py` & `safir-4.2.2/src/safir/testing/gcs.py`

 * *Files identical despite different names*

### Comparing `safir-4.2.1/src/safir/testing/kubernetes.py` & `safir-4.2.2/src/safir/testing/kubernetes.py`

 * *Files 0% similar despite different names*

```diff
@@ -358,17 +358,16 @@
     change the object returned by subsequent API calls. Likewise, the object
     returned by ``read_*`` calls will be the same object stored in the mock,
     and changing it will change the mock's data. (Sometimes this is the
     desired behavior, sometimes it isn't; we had to pick one and this is the
     approach we picked.)
 
     Most APIs do not support watches. The current exceptions are
-    ``list_namespaced_event``, ``list_namespaced_ingress``,
-    ``list_namespaced_job``, ``list_namespaced_pod``, and
-    ``list_namespaced_service``.
+    `list_namespaced_event`, `list_namespaced_ingress`, `list_namespaced_job`,
+    `list_namespaced_pod`, and `list_namespaced_service`.
 
     Attributes
     ----------
     initial_pod_phase
         String value to set the status of pods to when created. If this is set
         to ``Running`` (the default), a pod start event will also be
         generated when the pod is created.
```

### Comparing `safir-4.2.1/src/safir/testing/slack.py` & `safir-4.2.2/src/safir/testing/slack.py`

 * *Files identical despite different names*

### Comparing `safir-4.2.1/src/safir/testing/uvicorn.py` & `safir-4.2.2/src/safir/testing/uvicorn.py`

 * *Files identical despite different names*

### Comparing `safir-4.2.1/src/safir.egg-info/PKG-INFO` & `safir-4.2.2/src/safir.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: safir
-Version: 4.2.1
+Version: 4.2.2
 Summary: The Rubin Observatory SQuaRE framework for FastAPI services.
 Author-email: "Association of Universities for Research in Astronomy, Inc. (AURA)" <sqre-admin@lists.lsst.org>
 License: MIT License
         
         Copyright (c) 2020 Association of Universities for Research in Astronomy, Inc. (AURA)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `safir-4.2.1/src/safir.egg-info/SOURCES.txt` & `safir-4.2.2/src/safir.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 pyproject.toml
 tox.ini
 .github/CODE_OF_CONDUCT
 .github/CONTRIBUTING.md
 .github/dependabot.yml
 .github/workflows/ci.yaml
 .github/workflows/periodic.yaml
+changelog.d/_template.md
 docs/_rst_epilog.rst
 docs/api.rst
 docs/changelog.md
 docs/conf.py
 docs/documenteer.toml
 docs/index.rst
 docs/dev/development.rst
```

### Comparing `safir-4.2.1/tests/conftest.py` & `safir-4.2.2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `safir-4.2.1/tests/database_test.py` & `safir-4.2.2/tests/database_test.py`

 * *Files identical despite different names*

### Comparing `safir-4.2.1/tests/datetime_test.py` & `safir-4.2.2/tests/datetime_test.py`

 * *Files identical despite different names*

### Comparing `safir-4.2.1/tests/dependencies/arq_test.py` & `safir-4.2.2/tests/dependencies/arq_test.py`

 * *Files identical despite different names*

### Comparing `safir-4.2.1/tests/dependencies/db_session_test.py` & `safir-4.2.2/tests/dependencies/db_session_test.py`

 * *Files identical despite different names*

### Comparing `safir-4.2.1/tests/dependencies/gafaelfawr_test.py` & `safir-4.2.2/tests/dependencies/gafaelfawr_test.py`

 * *Files identical despite different names*

### Comparing `safir-4.2.1/tests/dependencies/http_client_test.py` & `safir-4.2.2/tests/dependencies/http_client_test.py`

 * *Files identical despite different names*

### Comparing `safir-4.2.1/tests/dependencies/logger_test.py` & `safir-4.2.2/tests/dependencies/logger_test.py`

 * *Files identical despite different names*

### Comparing `safir-4.2.1/tests/fastapi_test.py` & `safir-4.2.2/tests/fastapi_test.py`

 * *Files identical despite different names*

### Comparing `safir-4.2.1/tests/gcs_test.py` & `safir-4.2.2/tests/gcs_test.py`

 * *Files identical despite different names*

### Comparing `safir-4.2.1/tests/github/data/webhooks/check_run_created.json` & `safir-4.2.2/tests/github/data/webhooks/check_run_created.json`

 * *Files identical despite different names*

### Comparing `safir-4.2.1/tests/github/data/webhooks/check_suite_completed.json` & `safir-4.2.2/tests/github/data/webhooks/check_suite_completed.json`

 * *Files identical despite different names*

### Comparing `safir-4.2.1/tests/github/data/webhooks/installation.json` & `safir-4.2.2/tests/github/data/webhooks/installation.json`

 * *Files identical despite different names*

### Comparing `safir-4.2.1/tests/github/data/webhooks/installation_repositories.json` & `safir-4.2.2/tests/github/data/webhooks/installation_repositories.json`

 * *Files identical despite different names*

### Comparing `safir-4.2.1/tests/github/data/webhooks/pull_request_event.json` & `safir-4.2.2/tests/github/data/webhooks/pull_request_event.json`

 * *Files identical despite different names*

### Comparing `safir-4.2.1/tests/github/data/webhooks/push_event.json` & `safir-4.2.2/tests/github/data/webhooks/push_event.json`

 * *Files identical despite different names*

### Comparing `safir-4.2.1/tests/github/webhooks_test.py` & `safir-4.2.2/tests/github/webhooks_test.py`

 * *Files identical despite different names*

### Comparing `safir-4.2.1/tests/logging_test.py` & `safir-4.2.2/tests/logging_test.py`

 * *Files identical despite different names*

### Comparing `safir-4.2.1/tests/metadata_test.py` & `safir-4.2.2/tests/metadata_test.py`

 * *Files identical despite different names*

### Comparing `safir-4.2.1/tests/middleware/ivoa_test.py` & `safir-4.2.2/tests/middleware/ivoa_test.py`

 * *Files identical despite different names*

### Comparing `safir-4.2.1/tests/middleware/x_forwarded_test.py` & `safir-4.2.2/tests/middleware/x_forwarded_test.py`

 * *Files identical despite different names*

### Comparing `safir-4.2.1/tests/pydantic_test.py` & `safir-4.2.2/tests/pydantic_test.py`

 * *Files identical despite different names*

### Comparing `safir-4.2.1/tests/redis_test.py` & `safir-4.2.2/tests/redis_test.py`

 * *Files identical despite different names*

### Comparing `safir-4.2.1/tests/slack/blockkit_test.py` & `safir-4.2.2/tests/slack/blockkit_test.py`

 * *Files identical despite different names*

### Comparing `safir-4.2.1/tests/slack/webhook_test.py` & `safir-4.2.2/tests/slack/webhook_test.py`

 * *Files identical despite different names*

### Comparing `safir-4.2.1/tests/testing/conftest.py` & `safir-4.2.2/tests/testing/conftest.py`

 * *Files identical despite different names*

### Comparing `safir-4.2.1/tests/testing/gcs_test.py` & `safir-4.2.2/tests/testing/gcs_test.py`

 * *Files identical despite different names*

### Comparing `safir-4.2.1/tests/testing/kubernetes_test.py` & `safir-4.2.2/tests/testing/kubernetes_test.py`

 * *Files identical despite different names*

### Comparing `safir-4.2.1/tox.ini` & `safir-4.2.2/tox.ini`

 * *Files identical despite different names*

