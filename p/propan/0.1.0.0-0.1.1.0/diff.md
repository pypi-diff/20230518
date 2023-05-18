# Comparing `tmp/propan-0.1.0.0.tar.gz` & `tmp/propan-0.1.1.0.tar.gz`

## Comparing `propan-0.1.0.0.tar` & `propan-0.1.1.0.tar`

### file list

```diff
@@ -1,95 +1,117 @@
--rw-r--r--   0        0        0     2870 2020-02-02 00:00:00.000000 propan-0.1.0.0/CONTRIBUTING.md
--rw-r--r--   0        0        0     1456 2020-02-02 00:00:00.000000 propan-0.1.0.0/SECURITY.md
--rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 propan-0.1.0.0/.github/workflows/documentation.yml
--rw-r--r--   0        0        0      956 2020-02-02 00:00:00.000000 propan-0.1.0.0/.github/workflows/publish_coverage.yml
--rw-r--r--   0        0        0     1222 2020-02-02 00:00:00.000000 propan-0.1.0.0/.github/workflows/publish_pypi.yml
--rw-r--r--   0        0        0     2517 2020-02-02 00:00:00.000000 propan-0.1.0.0/.github/workflows/tests.yml
--rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 propan-0.1.0.0/examples/1_basic_usage.py
--rw-r--r--   0        0        0      457 2020-02-02 00:00:00.000000 propan-0.1.0.0/examples/2_specific_exchange.py
--rw-r--r--   0        0        0      645 2020-02-02 00:00:00.000000 propan-0.1.0.0/examples/3_lifespan_events.py
--rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 propan-0.1.0.0/examples/4_cli_attributes_promotion.py
--rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 propan-0.1.0.0/examples/5_publishing.py
--rw-r--r--   0        0        0      932 2020-02-02 00:00:00.000000 propan-0.1.0.0/examples/6_arguments_casting.py
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 propan-0.1.0.0/examples/7_handler_errors_processing.py
--rw-r--r--   0        0        0      405 2020-02-02 00:00:00.000000 propan-0.1.0.0/examples/8_rpc_over_mq.py
--rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 propan-0.1.0.0/examples/9_noblocking_callbacks.py
--rw-r--r--   0        0        0      992 2020-02-02 00:00:00.000000 propan-0.1.0.0/examples/dependencies/1_dependency_injection.py
--rw-r--r--   0        0        0      576 2020-02-02 00:00:00.000000 propan-0.1.0.0/examples/dependencies/2_dependency_declaration.py
--rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 propan-0.1.0.0/examples/dependencies/3_dependency_aliases.py
--rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 propan-0.1.0.0/examples/dependencies/4_dependency_deep_aliases.py
--rw-r--r--   0        0        0      555 2020-02-02 00:00:00.000000 propan-0.1.0.0/examples/dependencies/5_dependency_nesting.py
--rw-r--r--   0        0        0      815 2020-02-02 00:00:00.000000 propan-0.1.0.0/examples/dependencies/6_dependecy_calling.py
--rw-r--r--   0        0        0      678 2020-02-02 00:00:00.000000 propan-0.1.0.0/examples/dependencies/7_annotated.py
--rw-r--r--   0        0        0      656 2020-02-02 00:00:00.000000 propan-0.1.0.0/examples/http_frameworks_integrations/aiohttp.py
--rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 propan-0.1.0.0/examples/http_frameworks_integrations/blacksheep.py
--rw-r--r--   0        0        0      936 2020-02-02 00:00:00.000000 propan-0.1.0.0/examples/http_frameworks_integrations/falcon.py
--rw-r--r--   0        0        0      532 2020-02-02 00:00:00.000000 propan-0.1.0.0/examples/http_frameworks_integrations/fastapi.py
--rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 propan-0.1.0.0/examples/http_frameworks_integrations/native_fastapi.py
--rw-r--r--   0        0        0      520 2020-02-02 00:00:00.000000 propan-0.1.0.0/examples/http_frameworks_integrations/quart.py
--rw-r--r--   0        0        0      601 2020-02-02 00:00:00.000000 propan-0.1.0.0/examples/http_frameworks_integrations/sanic.py
--rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 propan-0.1.0.0/examples/http_frameworks_integrations/tornado.py
--rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 propan-0.1.0.0/examples/rabbit/direct.py
--rw-r--r--   0        0        0     1034 2020-02-02 00:00:00.000000 propan-0.1.0.0/examples/rabbit/fanout.py
--rw-r--r--   0        0        0     1618 2020-02-02 00:00:00.000000 propan-0.1.0.0/examples/rabbit/header.py
--rw-r--r--   0        0        0     1171 2020-02-02 00:00:00.000000 propan-0.1.0.0/examples/rabbit/topic.py
--rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 propan-0.1.0.0/propan/__about__.py
--rw-r--r--   0        0        0      886 2020-02-02 00:00:00.000000 propan-0.1.0.0/propan/__init__.py
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 propan-0.1.0.0/propan/__main__.py
--rw-r--r--   0        0        0     1243 2020-02-02 00:00:00.000000 propan-0.1.0.0/propan/annotations.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 propan-0.1.0.0/propan/py.typed
--rw-r--r--   0        0        0      841 2020-02-02 00:00:00.000000 propan-0.1.0.0/propan/types.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 propan-0.1.0.0/propan/brokers/__init__.py
--rw-r--r--   0        0        0     2913 2020-02-02 00:00:00.000000 propan-0.1.0.0/propan/brokers/push_back_watcher.py
--rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 propan-0.1.0.0/propan/brokers/model/__init__.py
--rw-r--r--   0        0        0     6476 2020-02-02 00:00:00.000000 propan-0.1.0.0/propan/brokers/model/broker_usecase.py
--rw-r--r--   0        0        0     1610 2020-02-02 00:00:00.000000 propan-0.1.0.0/propan/brokers/model/schemas.py
--rw-r--r--   0        0        0     1764 2020-02-02 00:00:00.000000 propan-0.1.0.0/propan/brokers/model/utils.py
--rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 propan-0.1.0.0/propan/brokers/nats/__init__.py
--rw-r--r--   0        0        0     4412 2020-02-02 00:00:00.000000 propan-0.1.0.0/propan/brokers/nats/nats_broker.py
--rw-r--r--   0        0        0     5349 2020-02-02 00:00:00.000000 propan-0.1.0.0/propan/brokers/nats/nats_broker.pyi
--rw-r--r--   0        0        0     1681 2020-02-02 00:00:00.000000 propan-0.1.0.0/propan/brokers/nats/nats_js_broker.py
--rw-r--r--   0        0        0      533 2020-02-02 00:00:00.000000 propan-0.1.0.0/propan/brokers/nats/schemas.py
--rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 propan-0.1.0.0/propan/brokers/rabbit/__init__.py
--rw-r--r--   0        0        0    11224 2020-02-02 00:00:00.000000 propan-0.1.0.0/propan/brokers/rabbit/rabbit_broker.py
--rw-r--r--   0        0        0     7300 2020-02-02 00:00:00.000000 propan-0.1.0.0/propan/brokers/rabbit/rabbit_broker.pyi
--rw-r--r--   0        0        0     1427 2020-02-02 00:00:00.000000 propan-0.1.0.0/propan/brokers/rabbit/schemas.py
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 propan-0.1.0.0/propan/cli/__init__.py
--rw-r--r--   0        0        0     3746 2020-02-02 00:00:00.000000 propan-0.1.0.0/propan/cli/app.py
--rw-r--r--   0        0        0     4010 2020-02-02 00:00:00.000000 propan-0.1.0.0/propan/cli/main.py
--rw-r--r--   0        0        0     5928 2020-02-02 00:00:00.000000 propan-0.1.0.0/propan/cli/startproject.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 propan-0.1.0.0/propan/cli/supervisors/__init__.py
--rw-r--r--   0        0        0     1926 2020-02-02 00:00:00.000000 propan-0.1.0.0/propan/cli/supervisors/basereload.py
--rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 propan-0.1.0.0/propan/cli/supervisors/multiprocess.py
--rw-r--r--   0        0        0     1176 2020-02-02 00:00:00.000000 propan-0.1.0.0/propan/cli/supervisors/utils.py
--rw-r--r--   0        0        0     1825 2020-02-02 00:00:00.000000 propan-0.1.0.0/propan/cli/supervisors/watchfiles.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 propan-0.1.0.0/propan/cli/utils/__init__.py
--rw-r--r--   0        0        0      838 2020-02-02 00:00:00.000000 propan-0.1.0.0/propan/cli/utils/imports.py
--rw-r--r--   0        0        0     1111 2020-02-02 00:00:00.000000 propan-0.1.0.0/propan/cli/utils/logs.py
--rw-r--r--   0        0        0     1241 2020-02-02 00:00:00.000000 propan-0.1.0.0/propan/cli/utils/parser.py
--rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 propan-0.1.0.0/propan/fastapi/__init__.py
--rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 propan-0.1.0.0/propan/fastapi/core/__init__.py
--rw-r--r--   0        0        0     3295 2020-02-02 00:00:00.000000 propan-0.1.0.0/propan/fastapi/core/route.py
--rw-r--r--   0        0        0     4062 2020-02-02 00:00:00.000000 propan-0.1.0.0/propan/fastapi/core/router.py
--rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 propan-0.1.0.0/propan/fastapi/rabbit/__init__.py
--rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 propan-0.1.0.0/propan/fastapi/rabbit/rabbit_router.py
--rw-r--r--   0        0        0     2922 2020-02-02 00:00:00.000000 propan-0.1.0.0/propan/fastapi/rabbit/rabbit_router.pyi
--rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 propan-0.1.0.0/propan/log/__init__.py
--rw-r--r--   0        0        0     2924 2020-02-02 00:00:00.000000 propan-0.1.0.0/propan/log/formatter.py
--rw-r--r--   0        0        0     1535 2020-02-02 00:00:00.000000 propan-0.1.0.0/propan/log/logging.py
--rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 propan-0.1.0.0/propan/test/__init__.py
--rw-r--r--   0        0        0     4302 2020-02-02 00:00:00.000000 propan-0.1.0.0/propan/test/rabbit.py
--rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 propan-0.1.0.0/propan/utils/__init__.py
--rw-r--r--   0        0        0      317 2020-02-02 00:00:00.000000 propan-0.1.0.0/propan/utils/classes.py
--rw-r--r--   0        0        0      522 2020-02-02 00:00:00.000000 propan-0.1.0.0/propan/utils/functions.py
--rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 propan-0.1.0.0/propan/utils/context/__init__.py
--rw-r--r--   0        0        0     1827 2020-02-02 00:00:00.000000 propan-0.1.0.0/propan/utils/context/main.py
--rw-r--r--   0        0        0      913 2020-02-02 00:00:00.000000 propan-0.1.0.0/propan/utils/context/types.py
--rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 propan-0.1.0.0/scripts/lint.sh
--rwxr-xr-x   0        0        0       37 2020-02-02 00:00:00.000000 propan-0.1.0.0/scripts/publish.sh
--rwxr-xr-x   0        0        0       88 2020-02-02 00:00:00.000000 propan-0.1.0.0/scripts/test-cov.sh
--rwxr-xr-x   0        0        0       27 2020-02-02 00:00:00.000000 propan-0.1.0.0/scripts/test.sh
--rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 propan-0.1.0.0/.gitignore
--rw-r--r--   0        0        0     1082 2020-02-02 00:00:00.000000 propan-0.1.0.0/LICENSE
--rw-r--r--   0        0        0    11210 2020-02-02 00:00:00.000000 propan-0.1.0.0/README.md
--rw-r--r--   0        0        0     5310 2020-02-02 00:00:00.000000 propan-0.1.0.0/pyproject.toml
--rw-r--r--   0        0        0    14481 2020-02-02 00:00:00.000000 propan-0.1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     2870 2020-02-02 00:00:00.000000 propan-0.1.1.0/CONTRIBUTING.md
+-rw-r--r--   0        0        0     1456 2020-02-02 00:00:00.000000 propan-0.1.1.0/SECURITY.md
+-rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 propan-0.1.1.0/.github/workflows/documentation.yml
+-rw-r--r--   0        0        0      956 2020-02-02 00:00:00.000000 propan-0.1.1.0/.github/workflows/publish_coverage.yml
+-rw-r--r--   0        0        0     1222 2020-02-02 00:00:00.000000 propan-0.1.1.0/.github/workflows/publish_pypi.yml
+-rw-r--r--   0        0        0     2595 2020-02-02 00:00:00.000000 propan-0.1.1.0/.github/workflows/tests.yml
+-rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 propan-0.1.1.0/examples/1_basic_usage.py
+-rw-r--r--   0        0        0      457 2020-02-02 00:00:00.000000 propan-0.1.1.0/examples/2_specific_exchange.py
+-rw-r--r--   0        0        0      645 2020-02-02 00:00:00.000000 propan-0.1.1.0/examples/3_lifespan_events.py
+-rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 propan-0.1.1.0/examples/4_cli_attributes_promotion.py
+-rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 propan-0.1.1.0/examples/5_publishing.py
+-rw-r--r--   0        0        0      932 2020-02-02 00:00:00.000000 propan-0.1.1.0/examples/6_arguments_casting.py
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 propan-0.1.1.0/examples/7_handler_errors_processing.py
+-rw-r--r--   0        0        0      405 2020-02-02 00:00:00.000000 propan-0.1.1.0/examples/8_rpc_over_mq.py
+-rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 propan-0.1.1.0/examples/9_noblocking_callbacks.py
+-rw-r--r--   0        0        0      992 2020-02-02 00:00:00.000000 propan-0.1.1.0/examples/dependencies/1_dependency_injection.py
+-rw-r--r--   0        0        0      576 2020-02-02 00:00:00.000000 propan-0.1.1.0/examples/dependencies/2_dependency_declaration.py
+-rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 propan-0.1.1.0/examples/dependencies/3_dependency_aliases.py
+-rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 propan-0.1.1.0/examples/dependencies/4_dependency_deep_aliases.py
+-rw-r--r--   0        0        0      555 2020-02-02 00:00:00.000000 propan-0.1.1.0/examples/dependencies/5_dependency_nesting.py
+-rw-r--r--   0        0        0      815 2020-02-02 00:00:00.000000 propan-0.1.1.0/examples/dependencies/6_dependecy_calling.py
+-rw-r--r--   0        0        0      678 2020-02-02 00:00:00.000000 propan-0.1.1.0/examples/dependencies/7_annotated.py
+-rw-r--r--   0        0        0      656 2020-02-02 00:00:00.000000 propan-0.1.1.0/examples/http_frameworks_integrations/aiohttp.py
+-rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 propan-0.1.1.0/examples/http_frameworks_integrations/blacksheep.py
+-rw-r--r--   0        0        0      936 2020-02-02 00:00:00.000000 propan-0.1.1.0/examples/http_frameworks_integrations/falcon.py
+-rw-r--r--   0        0        0      532 2020-02-02 00:00:00.000000 propan-0.1.1.0/examples/http_frameworks_integrations/fastapi.py
+-rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 propan-0.1.1.0/examples/http_frameworks_integrations/native_fastapi.py
+-rw-r--r--   0        0        0      520 2020-02-02 00:00:00.000000 propan-0.1.1.0/examples/http_frameworks_integrations/quart.py
+-rw-r--r--   0        0        0      601 2020-02-02 00:00:00.000000 propan-0.1.1.0/examples/http_frameworks_integrations/sanic.py
+-rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 propan-0.1.1.0/examples/http_frameworks_integrations/tornado.py
+-rw-r--r--   0        0        0     1031 2020-02-02 00:00:00.000000 propan-0.1.1.0/examples/rabbit/direct.py
+-rw-r--r--   0        0        0     1011 2020-02-02 00:00:00.000000 propan-0.1.1.0/examples/rabbit/fanout.py
+-rw-r--r--   0        0        0     1595 2020-02-02 00:00:00.000000 propan-0.1.1.0/examples/rabbit/header.py
+-rw-r--r--   0        0        0     1148 2020-02-02 00:00:00.000000 propan-0.1.1.0/examples/rabbit/topic.py
+-rw-r--r--   0        0        0      518 2020-02-02 00:00:00.000000 propan-0.1.1.0/examples/redis/direct.py
+-rw-r--r--   0        0        0      592 2020-02-02 00:00:00.000000 propan-0.1.1.0/examples/redis/pattern.py
+-rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 propan-0.1.1.0/propan/__about__.py
+-rw-r--r--   0        0        0     1090 2020-02-02 00:00:00.000000 propan-0.1.1.0/propan/__init__.py
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 propan-0.1.1.0/propan/__main__.py
+-rw-r--r--   0        0        0     1485 2020-02-02 00:00:00.000000 propan-0.1.1.0/propan/annotations.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 propan-0.1.1.0/propan/py.typed
+-rw-r--r--   0        0        0      866 2020-02-02 00:00:00.000000 propan-0.1.1.0/propan/types.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 propan-0.1.1.0/propan/brokers/__init__.py
+-rw-r--r--   0        0        0     2913 2020-02-02 00:00:00.000000 propan-0.1.1.0/propan/brokers/push_back_watcher.py
+-rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 propan-0.1.1.0/propan/brokers/model/__init__.py
+-rw-r--r--   0        0        0     6586 2020-02-02 00:00:00.000000 propan-0.1.1.0/propan/brokers/model/broker_usecase.py
+-rw-r--r--   0        0        0     1795 2020-02-02 00:00:00.000000 propan-0.1.1.0/propan/brokers/model/schemas.py
+-rw-r--r--   0        0        0     1764 2020-02-02 00:00:00.000000 propan-0.1.1.0/propan/brokers/model/utils.py
+-rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 propan-0.1.1.0/propan/brokers/nats/__init__.py
+-rw-r--r--   0        0        0     4539 2020-02-02 00:00:00.000000 propan-0.1.1.0/propan/brokers/nats/nats_broker.py
+-rw-r--r--   0        0        0     5349 2020-02-02 00:00:00.000000 propan-0.1.1.0/propan/brokers/nats/nats_broker.pyi
+-rw-r--r--   0        0        0     1681 2020-02-02 00:00:00.000000 propan-0.1.1.0/propan/brokers/nats/nats_js_broker.py
+-rw-r--r--   0        0        0      524 2020-02-02 00:00:00.000000 propan-0.1.1.0/propan/brokers/nats/schemas.py
+-rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 propan-0.1.1.0/propan/brokers/rabbit/__init__.py
+-rw-r--r--   0        0        0    11019 2020-02-02 00:00:00.000000 propan-0.1.1.0/propan/brokers/rabbit/rabbit_broker.py
+-rw-r--r--   0        0        0     7300 2020-02-02 00:00:00.000000 propan-0.1.1.0/propan/brokers/rabbit/rabbit_broker.pyi
+-rw-r--r--   0        0        0     1401 2020-02-02 00:00:00.000000 propan-0.1.1.0/propan/brokers/rabbit/schemas.py
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 propan-0.1.1.0/propan/brokers/redis/__init__.py
+-rw-r--r--   0        0        0     7807 2020-02-02 00:00:00.000000 propan-0.1.1.0/propan/brokers/redis/redis_broker.py
+-rw-r--r--   0        0        0     3975 2020-02-02 00:00:00.000000 propan-0.1.1.0/propan/brokers/redis/redis_broker.pyi
+-rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 propan-0.1.1.0/propan/brokers/redis/schemas.py
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 propan-0.1.1.0/propan/cli/__init__.py
+-rw-r--r--   0        0        0     4350 2020-02-02 00:00:00.000000 propan-0.1.1.0/propan/cli/app.py
+-rw-r--r--   0        0        0     3817 2020-02-02 00:00:00.000000 propan-0.1.1.0/propan/cli/main.py
+-rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 propan-0.1.1.0/propan/cli/startproject/__init__.py
+-rw-r--r--   0        0        0      338 2020-02-02 00:00:00.000000 propan-0.1.1.0/propan/cli/startproject/app.py
+-rw-r--r--   0        0        0     3696 2020-02-02 00:00:00.000000 propan-0.1.1.0/propan/cli/startproject/core.py
+-rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 propan-0.1.1.0/propan/cli/startproject/utils.py
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 propan-0.1.1.0/propan/cli/startproject/async_app/__init__.py
+-rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 propan-0.1.1.0/propan/cli/startproject/async_app/app.py
+-rw-r--r--   0        0        0     1228 2020-02-02 00:00:00.000000 propan-0.1.1.0/propan/cli/startproject/async_app/core.py
+-rw-r--r--   0        0        0     2065 2020-02-02 00:00:00.000000 propan-0.1.1.0/propan/cli/startproject/async_app/nats.py
+-rw-r--r--   0        0        0     2560 2020-02-02 00:00:00.000000 propan-0.1.1.0/propan/cli/startproject/async_app/rabbit.py
+-rw-r--r--   0        0        0     2245 2020-02-02 00:00:00.000000 propan-0.1.1.0/propan/cli/startproject/async_app/redis.py
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 propan-0.1.1.0/propan/cli/startproject/sync_app/__init__.py
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 propan-0.1.1.0/propan/cli/startproject/sync_app/app.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 propan-0.1.1.0/propan/cli/supervisors/__init__.py
+-rw-r--r--   0        0        0     1926 2020-02-02 00:00:00.000000 propan-0.1.1.0/propan/cli/supervisors/basereload.py
+-rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 propan-0.1.1.0/propan/cli/supervisors/multiprocess.py
+-rw-r--r--   0        0        0     1176 2020-02-02 00:00:00.000000 propan-0.1.1.0/propan/cli/supervisors/utils.py
+-rw-r--r--   0        0        0     1825 2020-02-02 00:00:00.000000 propan-0.1.1.0/propan/cli/supervisors/watchfiles.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 propan-0.1.1.0/propan/cli/utils/__init__.py
+-rw-r--r--   0        0        0      838 2020-02-02 00:00:00.000000 propan-0.1.1.0/propan/cli/utils/imports.py
+-rw-r--r--   0        0        0     1111 2020-02-02 00:00:00.000000 propan-0.1.1.0/propan/cli/utils/logs.py
+-rw-r--r--   0        0        0     1241 2020-02-02 00:00:00.000000 propan-0.1.1.0/propan/cli/utils/parser.py
+-rw-r--r--   0        0        0      269 2020-02-02 00:00:00.000000 propan-0.1.1.0/propan/fastapi/__init__.py
+-rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 propan-0.1.1.0/propan/fastapi/core/__init__.py
+-rw-r--r--   0        0        0     3299 2020-02-02 00:00:00.000000 propan-0.1.1.0/propan/fastapi/core/route.py
+-rw-r--r--   0        0        0     4062 2020-02-02 00:00:00.000000 propan-0.1.1.0/propan/fastapi/core/router.py
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 propan-0.1.1.0/propan/fastapi/rabbit/__init__.py
+-rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 propan-0.1.1.0/propan/fastapi/rabbit/router.py
+-rw-r--r--   0        0        0     2922 2020-02-02 00:00:00.000000 propan-0.1.1.0/propan/fastapi/rabbit/router.pyi
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 propan-0.1.1.0/propan/fastapi/redis/__init__.py
+-rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 propan-0.1.1.0/propan/fastapi/redis/router.py
+-rw-r--r--   0        0        0     3284 2020-02-02 00:00:00.000000 propan-0.1.1.0/propan/fastapi/redis/router.pyi
+-rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 propan-0.1.1.0/propan/log/__init__.py
+-rw-r--r--   0        0        0     2924 2020-02-02 00:00:00.000000 propan-0.1.1.0/propan/log/formatter.py
+-rw-r--r--   0        0        0     1535 2020-02-02 00:00:00.000000 propan-0.1.1.0/propan/log/logging.py
+-rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 propan-0.1.1.0/propan/test/__init__.py
+-rw-r--r--   0        0        0     3806 2020-02-02 00:00:00.000000 propan-0.1.1.0/propan/test/rabbit.py
+-rw-r--r--   0        0        0     2242 2020-02-02 00:00:00.000000 propan-0.1.1.0/propan/test/redis.py
+-rw-r--r--   0        0        0      605 2020-02-02 00:00:00.000000 propan-0.1.1.0/propan/test/utils.py
+-rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 propan-0.1.1.0/propan/utils/__init__.py
+-rw-r--r--   0        0        0      317 2020-02-02 00:00:00.000000 propan-0.1.1.0/propan/utils/classes.py
+-rw-r--r--   0        0        0      522 2020-02-02 00:00:00.000000 propan-0.1.1.0/propan/utils/functions.py
+-rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 propan-0.1.1.0/propan/utils/context/__init__.py
+-rw-r--r--   0        0        0     1856 2020-02-02 00:00:00.000000 propan-0.1.1.0/propan/utils/context/main.py
+-rw-r--r--   0        0        0      913 2020-02-02 00:00:00.000000 propan-0.1.1.0/propan/utils/context/types.py
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 propan-0.1.1.0/scripts/lint.sh
+-rwxr-xr-x   0        0        0       37 2020-02-02 00:00:00.000000 propan-0.1.1.0/scripts/publish.sh
+-rwxr-xr-x   0        0        0       88 2020-02-02 00:00:00.000000 propan-0.1.1.0/scripts/test-cov.sh
+-rwxr-xr-x   0        0        0       27 2020-02-02 00:00:00.000000 propan-0.1.1.0/scripts/test.sh
+-rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 propan-0.1.1.0/.gitignore
+-rw-r--r--   0        0        0     1082 2020-02-02 00:00:00.000000 propan-0.1.1.0/LICENSE
+-rw-r--r--   0        0        0    12114 2020-02-02 00:00:00.000000 propan-0.1.1.0/README.md
+-rw-r--r--   0        0        0     5411 2020-02-02 00:00:00.000000 propan-0.1.1.0/pyproject.toml
+-rw-r--r--   0        0        0    15563 2020-02-02 00:00:00.000000 propan-0.1.1.0/PKG-INFO
```

### Comparing `propan-0.1.0.0/CONTRIBUTING.md` & `propan-0.1.1.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `propan-0.1.0.0/SECURITY.md` & `propan-0.1.1.0/SECURITY.md`

 * *Files identical despite different names*

### Comparing `propan-0.1.0.0/.github/workflows/publish_coverage.yml` & `propan-0.1.1.0/.github/workflows/publish_coverage.yml`

 * *Files identical despite different names*

### Comparing `propan-0.1.0.0/.github/workflows/publish_pypi.yml` & `propan-0.1.1.0/.github/workflows/publish_pypi.yml`

 * *Files identical despite different names*

### Comparing `propan-0.1.0.0/.github/workflows/tests.yml` & `propan-0.1.1.0/.github/workflows/tests.yml`

 * *Files 5% similar despite different names*

```diff
@@ -16,14 +16,19 @@
       fail-fast: false
     
     services:
       rabbitmq:
         image: rabbitmq
         ports:
           - 5672:5672
+      
+      redis:
+        image: redis
+        ports:
+          - 6379:6379
 
     steps:
       - uses: actions/checkout@v3
       - name: Set up Python
         uses: actions/setup-python@v4
         with:
           python-version: ${{ matrix.python-version }}
```

### Comparing `propan-0.1.0.0/examples/3_lifespan_events.py` & `propan-0.1.1.0/examples/3_lifespan_events.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.0.0/examples/4_cli_attributes_promotion.py` & `propan-0.1.1.0/examples/4_cli_attributes_promotion.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.0.0/examples/5_publishing.py` & `propan-0.1.1.0/examples/5_publishing.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.0.0/examples/6_arguments_casting.py` & `propan-0.1.1.0/examples/6_arguments_casting.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.0.0/examples/7_handler_errors_processing.py` & `propan-0.1.1.0/examples/7_handler_errors_processing.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.0.0/examples/dependencies/1_dependency_injection.py` & `propan-0.1.1.0/examples/dependencies/1_dependency_injection.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.0.0/examples/dependencies/2_dependency_declaration.py` & `propan-0.1.1.0/examples/dependencies/2_dependency_declaration.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.0.0/examples/dependencies/4_dependency_deep_aliases.py` & `propan-0.1.1.0/examples/dependencies/4_dependency_deep_aliases.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.0.0/examples/dependencies/5_dependency_nesting.py` & `propan-0.1.1.0/examples/dependencies/5_dependency_nesting.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.0.0/examples/dependencies/6_dependecy_calling.py` & `propan-0.1.1.0/examples/dependencies/6_dependecy_calling.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.0.0/examples/dependencies/7_annotated.py` & `propan-0.1.1.0/examples/dependencies/7_annotated.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.0.0/examples/http_frameworks_integrations/aiohttp.py` & `propan-0.1.1.0/examples/http_frameworks_integrations/aiohttp.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.0.0/examples/http_frameworks_integrations/blacksheep.py` & `propan-0.1.1.0/examples/http_frameworks_integrations/blacksheep.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.0.0/examples/http_frameworks_integrations/falcon.py` & `propan-0.1.1.0/examples/http_frameworks_integrations/falcon.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.0.0/examples/http_frameworks_integrations/fastapi.py` & `propan-0.1.1.0/examples/http_frameworks_integrations/fastapi.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.0.0/examples/http_frameworks_integrations/quart.py` & `propan-0.1.1.0/examples/http_frameworks_integrations/quart.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.0.0/examples/http_frameworks_integrations/sanic.py` & `propan-0.1.1.0/examples/http_frameworks_integrations/sanic.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.0.0/examples/http_frameworks_integrations/tornado.py` & `propan-0.1.1.0/examples/http_frameworks_integrations/tornado.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.0.0/examples/rabbit/direct.py` & `propan-0.1.1.0/examples/rabbit/direct.py`

 * *Files 8% similar despite different names*

```diff
@@ -21,15 +21,13 @@
 
 
 @broker.handle(queue_2, direct_exchange)
 async def base_handler3(logger: Logger):
     logger.info("base_handler3")
 
 
-@app.on_startup
+@app.after_startup
 async def send_messages():
-    await broker.start()
-
     await broker.publish(queue=queue_1, exchange=direct_exchange)
     await broker.publish(queue=queue_1, exchange=direct_exchange)
     await broker.publish(queue=queue_1, exchange=direct_exchange)
     await broker.publish(queue=queue_2, exchange=direct_exchange)
```

### Comparing `propan-0.1.0.0/examples/rabbit/fanout.py` & `propan-0.1.1.0/examples/rabbit/fanout.py`

 * *Files 8% similar despite different names*

```diff
@@ -21,15 +21,13 @@
 
 
 @broker.handle(queue_2, fanout_exchange)
 async def base_handler3(logger: Logger):
     logger.info("base_handler3")
 
 
-@app.on_startup
+@app.after_startup
 async def send_messages():
-    await broker.start()
-
     await broker.publish(exchange=fanout_exchange)
     await broker.publish(exchange=fanout_exchange)
     await broker.publish(exchange=fanout_exchange)
     await broker.publish(exchange=fanout_exchange)
```

### Comparing `propan-0.1.0.0/examples/rabbit/header.py` & `propan-0.1.1.0/examples/rabbit/header.py`

 * *Files 6% similar despite different names*

```diff
@@ -38,17 +38,15 @@
 
 
 @broker.handle(queue_3, header_exchange)
 async def base_handler4(logger: Logger):
     logger.info("base_handler4")
 
 
-@app.on_startup
+@app.after_startup
 async def send_messages():
-    await broker.start()
-
     await broker.publish(exchange=header_exchange, headers={"key": 1})
     await broker.publish(exchange=header_exchange, headers={"key": 1})
     await broker.publish(exchange=header_exchange, headers={"key": 1})
     await broker.publish(exchange=header_exchange, headers={"key": 2})
     await broker.publish(exchange=header_exchange, headers={"key2": 2})
     await broker.publish(exchange=header_exchange, headers={"key": 2, "key2": 2})
```

### Comparing `propan-0.1.0.0/examples/rabbit/topic.py` & `propan-0.1.1.0/examples/rabbit/topic.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,13 @@
 
 
 @broker.handle(queue_2, topic_exchange)
 async def base_handler3(logger: Logger):
     logger.info("base_handler3")
 
 
-@app.on_startup
+@app.after_startup
 async def send_messages():
-    await broker.start()
-
     await broker.publish(routing_key="logs.info", exchange=topic_exchange)
     await broker.publish(routing_key="logs.info", exchange=topic_exchange)
     await broker.publish(routing_key="logs.info", exchange=topic_exchange)
     await broker.publish(routing_key="logs.debug", exchange=topic_exchange)
```

### Comparing `propan-0.1.0.0/propan/__init__.py` & `propan-0.1.1.0/propan/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,19 +9,26 @@
     RabbitBroker = None  # type: ignore
 
 try:
     from propan.brokers.nats import NatsBroker
 except Exception:
     NatsBroker = None  # type: ignore
 
-assert any((RabbitBroker, NatsBroker)), (
+try:
+    from propan.brokers.redis import RedisBroker
+except Exception as e:
+    print(e)
+    RedisBroker = None  # type: ignore
+
+assert any((RabbitBroker, NatsBroker, RedisBroker)), (
     "You should specify using broker!\n"
     "Install it using one of the following commands:\n"
     'pip install "propan[async-rabbit]"\n'
     'pip install "propan[async-nats]"\n'
+    'pip install "propan[async-redis]"\n'
 )
 
 
 __all__ = (  # noqa: F405
     # app
     "PropanApp",
     # log
@@ -34,8 +41,9 @@
     "context",
     "Context",
     "ContextRepo" "Alias",
     "Depends",
     # brokers
     "NatsBroker",
     "RabbitBroker",
+    "RedisBroker",
 )
```

### Comparing `propan-0.1.0.0/propan/annotations.py` & `propan-0.1.1.0/propan/annotations.py`

 * *Files 16% similar despite different names*

```diff
@@ -27,18 +27,27 @@
     from propan.brokers.nats import NatsBroker as NB
 
     NatsBroker = Annotated[NB, ContextField("broker")]
     NatsMessage = Annotated[Msg, ContextField("message")]
 except Exception:
     NatsBroker = NatsMessage = None  # type: ignore
 
+try:
+    from propan.brokers.redis import RedisBroker as RedB
+
+    RedisBroker = Annotated[RedB, ContextField("broker")]
+except Exception:
+    RedisBroker = None  # type: ignore
+
 assert any(
     (
         all((RabbitBroker, RabbitMessage)),
         all((NatsBroker, NatsMessage)),
+        RedisBroker,
     )
 ), (
     "You should specify using broker!\n"
     "Install it using one of the following commands:\n"
     'pip install "propan[async-rabbit]"\n'
     'pip install "propan[async-nats]"\n'
+    'pip install "propan[async-redis]"\n'
 )
```

### Comparing `propan-0.1.0.0/propan/types.py` & `propan-0.1.1.0/propan/types.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Any, Awaitable, Callable, Coroutine, Dict, Union
+from typing import Any, Awaitable, Callable, Coroutine, Dict, Sequence, Union
 
 from pydantic import BaseModel
 from typing_extensions import TypeAlias
 
 AsyncFunc: TypeAlias = Callable[..., Awaitable[Any]]
 
 AnyDict: TypeAlias = Dict[str, Any]
@@ -11,14 +11,14 @@
 
 DecoratedCallable: TypeAlias = AnyCallable
 DecoratedCallableNone: TypeAlias = NoneCallable
 DecoratedAsync: TypeAlias = AsyncFunc
 
 Wrapper: TypeAlias = Callable[[AnyCallable], DecoratedCallable]
 AsyncWrapper: TypeAlias = Callable[[AnyCallable], DecoratedAsync]
-DecodedMessage: TypeAlias = Union[str, AnyDict, bytes]
+DecodedMessage: TypeAlias = Union[AnyDict, Sequence[Any], str, bytes]
 SendableMessage: TypeAlias = Union[DecodedMessage, BaseModel, None]
 
 HandlerWrapper: TypeAlias = Callable[
     [Callable[..., Coroutine[Any, Any, SendableMessage]]],
     Callable[..., SendableMessage],
 ]
```

### Comparing `propan-0.1.0.0/propan/brokers/push_back_watcher.py` & `propan-0.1.1.0/propan/brokers/push_back_watcher.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.0.0/propan/brokers/model/broker_usecase.py` & `propan-0.1.1.0/propan/brokers/model/broker_usecase.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,17 +16,17 @@
     set_message_context,
     suppress_decor,
 )
 from propan.brokers.push_back_watcher import BaseWatcher
 from propan.log import access_logger
 from propan.types import (
     AnyCallable,
+    AnyDict,
     DecodedMessage,
     DecoratedAsync,
-    DecoratedCallable,
     HandlerWrapper,
     SendableMessage,
     Wrapper,
 )
 from propan.utils import apply_types, context
 from propan.utils.functions import to_async
 
@@ -35,23 +35,23 @@
 
 
 class BrokerUsecase(ABC):
     logger: Optional[logging.Logger]
     log_level: int
     handlers: List[Any]
     _connection: Any
-    _fmt: str
+    _fmt: Optional[str]
 
     def __init__(
         self,
         *args: Any,
         apply_types: bool = True,
         logger: Optional[logging.Logger] = access_logger,
         log_level: int = logging.INFO,
-        log_fmt: str = "%(asctime)s %(levelname)s - %(message)s",
+        log_fmt: Optional[str] = "%(asctime)s %(levelname)s - %(message)s",
         **kwargs: Any,
     ) -> None:
         self.logger = logger
         self.log_level = log_level
         self._fmt = log_fmt
 
         self._connection = None
@@ -130,19 +130,20 @@
 
     @staticmethod
     def _encode_message(msg: SendableMessage) -> Tuple[bytes, Optional[ContentType]]:
         return SendableModel.to_send(msg)
 
     @property
     def fmt(self) -> str:  # pragma: no cover
-        return self._fmt
+        return self._fmt or ""
 
     async def start(self) -> None:
         if self.logger is not None:
             change_logger_handlers(self.logger, self.fmt)
+
         await self.connect()
 
     async def __aenter__(self: Cls) -> Cls:
         await self.connect()
         return self
 
     async def __aexit__(self, *args: Any, **kwargs: Any) -> None:
@@ -155,19 +156,19 @@
         **broker_args: Any,
     ) -> DecoratedAsync:
         f = to_async(func)
 
         if self._is_apply_types is True:
             f = apply_types(f)
 
+        f = self._wrap_decode_message(f)
+
         if self.logger is not None:
             f = self._log_execution(**broker_args)(f)
 
-        f = self._wrap_decode_message(f)
-
         f = self._process_message(f, get_watcher(self.logger, retry))
 
         f = self._wrap_parse_message(f)
 
         f = set_message_context(f)
 
         f = suppress_decor(f)
@@ -192,26 +193,26 @@
 
         return wrapper
 
     def _log_execution(
         self,
         **broker_args: Any,
     ) -> Wrapper:
-        def decor(func: AnyCallable) -> DecoratedCallable:
+        def decor(
+            func: Callable[[PropanMessage], Awaitable[T]]
+        ) -> Callable[[PropanMessage], Awaitable[T]]:
             @wraps(func)
-            async def wrapper(*args: Any, **kwargs: Any) -> Any:
-                message = context.get("message")
-
+            async def wrapper(message: PropanMessage) -> T:
                 log_context = self._get_log_context(message=message, **broker_args)
 
                 with context.scope("log_context", log_context):
                     self._log("Received")
 
                     try:
-                        r = await func(*args, **kwargs)
+                        r = await func(message)
                     except Exception as e:
                         self._log(repr(e), logging.ERROR)
                         raise e
                     else:
                         self._log("Processed")
                         return r
 
@@ -219,10 +220,13 @@
 
         return decor
 
     def _log(
         self,
         message: str,
         log_level: Optional[int] = None,
+        extra: Optional[AnyDict] = None,
     ) -> None:
         if self.logger is not None:
-            self.logger.log(level=(log_level or self.log_level), msg=message)
+            self.logger.log(
+                level=(log_level or self.log_level), msg=message, extra=extra
+            )
```

### Comparing `propan-0.1.0.0/propan/brokers/model/schemas.py` & `propan-0.1.1.0/propan/brokers/model/schemas.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,35 +1,38 @@
 import json
+from dataclasses import dataclass
 from enum import Enum
-from typing import Any, Optional, Tuple
+from typing import Any, Dict, Optional, Sequence, Tuple, Union
 from uuid import uuid4
 
-from pydantic import BaseModel, Field
-from pydantic.dataclasses import dataclass
-from typing_extensions import TypeAlias
+from pydantic import BaseModel, Field, Json
+from pydantic.dataclasses import dataclass as pydantic_dataclass
+from typing_extensions import TypeAlias, assert_never
 
-from propan.types import AnyDict, DecodedMessage, SendableMessage
+from propan.types import AnyDict, DecodedMessage, DecoratedCallable, SendableMessage
 
 ContentType: TypeAlias = str
 
 
+@dataclass
+class BaseHandler:
+    callback: DecoratedCallable
+
+
 class ContentTypes(str, Enum):
     text = "text/plain"
     json = "application/json"
 
 
 class NameRequired(BaseModel):
     name: Optional[str] = Field(...)
 
     def __init__(self, name: str, **kwargs: Any):
         super().__init__(name=name, **kwargs)
 
-    def __eq__(self, other: object) -> bool:
-        return isinstance(other, NameRequired) and self.name == other.name
-
 
 class Queue(NameRequired):
     name: Optional[str] = Field(...)
 
     def __init__(self, name: str, **kwargs: Any):
         super().__init__(name=name, **kwargs)
 
@@ -43,23 +46,27 @@
             return b"", None
 
         if isinstance(msg, bytes):
             return msg, None
 
         m = cls(message=msg).message  # type: ignore
 
-        if isinstance(m, dict):
-            return json.dumps(m).encode(), ContentTypes.json.value
-
         if isinstance(m, str):
             return m.encode(), ContentTypes.text.value
 
-        return m, None
+        if isinstance(m, (Dict, Sequence)):
+            return json.dumps(m).encode(), ContentTypes.json.value
 
+        assert_never()  # pragma: no cover
 
-@dataclass
+
+class RawDecoced(BaseModel):
+    message: Union[Json[Any], str]
+
+
+@pydantic_dataclass
 class PropanMessage:
     body: bytes
     raw_message: Any
-    content_type: str
+    content_type: Optional[str] = None
     headers: AnyDict = Field(default_factory=dict)
     message_id: str = Field(default_factory=lambda: str(uuid4()))
```

### Comparing `propan-0.1.0.0/propan/brokers/model/utils.py` & `propan-0.1.1.0/propan/brokers/model/utils.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.0.0/propan/brokers/nats/nats_broker.py` & `propan-0.1.1.0/propan/brokers/nats/nats_broker.py`

 * *Files 7% similar despite different names*

```diff
@@ -25,15 +25,22 @@
         super().__init__(*args, log_fmt=log_fmt, **kwargs)
 
         self._connection = None
 
         self.__max_queue_len = 0
         self.__max_subject_len = 4
 
-    async def _connect(self, *args: Any, **kwargs: Any) -> Client:
+    async def _connect(
+        self,
+        *args: Any,
+        url: Optional[str] = None,
+        **kwargs: Any,
+    ) -> Client:
+        if url is not None:
+            kwargs["servers"] = kwargs.pop("servers", []) + [url]
         return await nats.connect(*args, **kwargs)
 
     def handle(
         self,
         subject: str,
         queue: str = "",
         **original_kwargs,
@@ -67,31 +74,30 @@
 
     async def start(self) -> None:
         await super().start()
 
         for handler in self.handlers:
             func = handler.callback
 
-            if self.logger:
-                self._get_log_context(None, handler.subject, handler.queue)
-                self.logger.info(f"`{func.__name__}` waiting for messages")
+            c = self._get_log_context(None, handler.subject, handler.queue)
+            self._log(f"`{func.__name__}` waiting for messages", extra=c)
 
             sub = await self._connection.subscribe(handler.subject, cb=func)
             handler.subscription = sub
 
     async def publish(
         self,
         message: SendableMessage,
         subject: str,
         **publish_args: Any,
     ) -> None:
         if self._connection is None:
             raise ValueError("NatsConnection not started yet")
 
-        msg, content_type = super()._encode_message(message)
+        msg, content_type = self._encode_message(message)
 
         return await self._connection.publish(
             subject,
             msg,
             headers={
                 **publish_args.pop("headers", {}),
                 "content-type": content_type,
```

### Comparing `propan-0.1.0.0/propan/brokers/nats/nats_broker.pyi` & `propan-0.1.1.0/propan/brokers/nats/nats_broker.pyi`

 * *Files identical despite different names*

### Comparing `propan-0.1.0.0/propan/brokers/nats/nats_js_broker.py` & `propan-0.1.1.0/propan/brokers/nats/nats_js_broker.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.0.0/propan/brokers/rabbit/rabbit_broker.py` & `propan-0.1.1.0/propan/brokers/rabbit/rabbit_broker.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,21 @@
 import asyncio
-import logging
 from functools import wraps
 from typing import Any, Callable, Dict, List, Optional, Tuple, Type, TypeVar, Union
 from uuid import uuid4
 
 import aio_pika
 import aiormq
 from aio_pika.abc import DeliveryMode
 
 from propan.brokers.model import BrokerUsecase
 from propan.brokers.model.schemas import PropanMessage
 from propan.brokers.push_back_watcher import BaseWatcher, WatcherContext
 from propan.brokers.rabbit.schemas import Handler, RabbitExchange, RabbitQueue
 from propan.types import AnyDict, DecoratedCallable, SendableMessage, Wrapper
-from propan.utils.context import context as global_context
 
 TimeoutType = Optional[Union[int, float]]
 PikaSendableMessage = Union[aio_pika.message.Message, SendableMessage]
 T = TypeVar("T")
 
 
 class RabbitBroker(BrokerUsecase):
@@ -63,15 +61,15 @@
         )
 
         if self._channel is None:  # pragma: no branch
             max_consumers = self._max_consumers
             self._channel = await connection.channel()
 
             if max_consumers:
-                self._log(f"Set max consumers to {max_consumers}", logging.INFO)
+                self._log(f"Set max consumers to {max_consumers}")
                 await self._channel.set_qos(prefetch_count=int(self._max_consumers))
 
         return connection
 
     def handle(
         self,
         queue: Union[str, RabbitQueue],
@@ -100,18 +98,16 @@
         await super().start()
 
         for handler in self.handlers:
             queue = await self._init_handler(handler)
 
             func = handler.callback
 
-            if self.logger is not None:
-                context = self._get_log_context(None, handler.queue, handler.exchange)
-                global_context.set_local("log_context", context)
-                self.logger.info(f"`{func.__name__}` waiting for messages")
+            c = self._get_log_context(None, handler.queue, handler.exchange)
+            self._log(f"`{func.__name__}` waiting for messages", extra=c)
 
             await queue.consume(func)
 
     async def publish(
         self,
         message: PikaSendableMessage = "",
         queue: Union[RabbitQueue, str] = "",
```

### Comparing `propan-0.1.0.0/propan/brokers/rabbit/rabbit_broker.pyi` & `propan-0.1.1.0/propan/brokers/rabbit/rabbit_broker.pyi`

 * *Files identical despite different names*

### Comparing `propan-0.1.0.0/propan/brokers/rabbit/schemas.py` & `propan-0.1.1.0/propan/brokers/rabbit/schemas.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
+from dataclasses import dataclass
 from typing import Any, Dict, Optional
 
 from aio_pika.abc import ExchangeType, TimeoutType
-from pydantic import BaseModel, Field
+from pydantic import Field
 
-from propan.brokers.model.schemas import NameRequired, Queue
-from propan.types import DecoratedCallable
+from propan.brokers.model.schemas import BaseHandler, NameRequired, Queue
 
 __all__ = (
     "RabbitQueue",
     "RabbitExchange",
     "Handler",
     "ExchangeType",
 )
@@ -43,11 +43,11 @@
     robust: bool = True
 
     bind_to: Optional["RabbitExchange"] = Field(None, exclude=True)
     bind_arguments: Optional[Dict[str, Any]] = Field(None, exclude=True)
     routing_key: str = Field("", exclude=True)
 
 
-class Handler(BaseModel):
-    callback: DecoratedCallable
+@dataclass
+class Handler(BaseHandler):
     queue: RabbitQueue
     exchange: Optional[RabbitExchange] = None
```

### Comparing `propan-0.1.0.0/propan/cli/app.py` & `propan-0.1.1.0/propan/cli/app.py`

 * *Files 19% similar despite different names*

```diff
@@ -5,30 +5,32 @@
 from anyio import create_memory_object_stream, create_task_group
 from anyio.streams.memory import MemoryObjectReceiveStream, MemoryObjectSendStream
 from typing_extensions import Protocol
 
 from propan.cli.supervisors.utils import set_exit
 from propan.cli.utils.parser import SettingField
 from propan.log import logger
-from propan.types import AnyCallable, AsyncFunc, DecoratedCallableNone
+from propan.types import AnyCallable, AsyncFunc
 from propan.utils import apply_types, context
 from propan.utils.functions import to_async
 
 
 class Runnable(Protocol):
     async def start(self) -> None:
         ...
 
     async def close(self) -> None:
         ...
 
 
 class PropanApp:
     _on_startup_calling: List[AsyncFunc]
+    _after_startup_calling: List[AsyncFunc]
     _on_shutdown_calling: List[AsyncFunc]
+    _after_shutdown_calling: List[AsyncFunc]
 
     _stop_stream: Optional[MemoryObjectSendStream[bool]]
     _receive_stream: Optional[MemoryObjectReceiveStream[bool]]
 
     def __init__(
         self,
         broker: Optional[Runnable] = None,
@@ -36,31 +38,35 @@
     ):
         self.broker = broker
         self.logger = logger
         self.context = context
         context.set_global("app", self)
 
         self._on_startup_calling = []
+        self._after_startup_calling = []
         self._on_shutdown_calling = []
+        self._after_shutdown_calling = []
         self._stop_stream = None
         self._receive_stream = None
         self._command_line_options: Dict[str, SettingField] = {}
 
     def set_broker(self, broker: Runnable) -> None:
         self.broker = broker
 
-    def on_startup(self, func: AnyCallable) -> DecoratedCallableNone:
-        f: AsyncFunc = apply_types(to_async(func))
-        self._on_startup_calling.append(f)
-        return func
-
-    def on_shutdown(self, func: AnyCallable) -> DecoratedCallableNone:
-        f: AsyncFunc = apply_types(to_async(func))
-        self._on_shutdown_calling.append(f)
-        return func
+    def on_startup(self, func: AnyCallable) -> AnyCallable:
+        return _set_async_hook(self._on_startup_calling, func)
+
+    def on_shutdown(self, func: AnyCallable) -> AnyCallable:
+        return _set_async_hook(self._on_shutdown_calling, func)
+
+    def after_startup(self, func: AnyCallable) -> AnyCallable:
+        return _set_async_hook(self._after_startup_calling, func)
+
+    def after_shutdown(self, func: AnyCallable) -> AnyCallable:
+        return _set_async_hook(self._after_shutdown_calling, func)
 
     async def run(self, log_level: int = logging.INFO) -> None:
         self._init_async_cycle()
         async with create_task_group() as tg:
             set_exit(lambda *_: tg.start_soon(self.__exit, True))
             tg.start_soon(self._stop, log_level)
             tg.start_soon(self._start, log_level)
@@ -89,20 +95,32 @@
     async def _startup(self) -> None:
         for func in self._on_startup_calling:
             await func(**self._command_line_options)
 
         if self.broker is not None:
             await self.broker.start()
 
+        for func in self._after_startup_calling:
+            await func()
+
     async def _shutdown(self) -> None:
+        for func in self._on_shutdown_calling:
+            await func()
+
         if (
             self.broker is not None
             and getattr(self.broker, "_connection", False) is not False
         ):
             await self.broker.close()
 
-        for func in self._on_shutdown_calling:
+        for func in self._after_shutdown_calling:
             await func()
 
     async def __exit(self, flag: bool) -> None:
         if self._stop_stream is not None:  # pragma: no branch
             await self._stop_stream.send(flag)
+
+
+def _set_async_hook(hooks: List[AsyncFunc], func: AnyCallable) -> AnyCallable:
+    f: AsyncFunc = apply_types(to_async(func))
+    hooks.append(f)
+    return func
```

### Comparing `propan-0.1.0.0/propan/cli/main.py` & `propan-0.1.1.0/propan/cli/main.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,20 +4,24 @@
 from pathlib import Path
 from typing import Dict, Optional
 
 import typer
 
 from propan.__about__ import __version__
 from propan.cli.app import PropanApp
+from propan.cli.startproject import create_app
 from propan.cli.utils.imports import get_app_path, import_object
 from propan.cli.utils.logs import LogLevels, get_log_level, set_log_level
 from propan.cli.utils.parser import SettingField, parse_cli_args
 from propan.log import logger
 
-cli = typer.Typer()
+cli = typer.Typer(pretty_exceptions_short=True)
+cli.add_typer(
+    create_app, name="create", help="Create a new Propan project at [APPNAME] directory"
+)
 
 
 def version_callback(version: bool) -> None:
     if version is True:
         import platform
 
         typer.echo(
@@ -33,34 +37,26 @@
         raise typer.Exit()
 
 
 @cli.callback()
 def main(
     version: Optional[bool] = typer.Option(
         False,
+        "-v",
         "--version",
         callback=version_callback,
         is_eager=True,
         help="Show current platform, python and propan version",
     )
 ) -> None:
     """
     Generate, run and manage Propan apps to greater development experience
     """
 
 
-@cli.command()
-def create(appname: str) -> None:
-    """Create a new Propan project at [APPNAME] directory"""
-    from propan.cli.startproject import create
-
-    project = create(Path.cwd() / appname, __version__)
-    typer.echo(f"Create Propan project template at: {project}")
-
-
 @cli.command(
     context_settings={"allow_extra_args": True, "ignore_unknown_options": True}
 )
 def run(
     ctx: typer.Context,
     app: str = typer.Argument(
         ..., help="[python_module:PropanApp] - path to your application"
@@ -123,18 +119,15 @@
 
     else:
         set_log_level(log_level, propan_app)
 
         propan_app._command_line_options = extra_options
 
         if sys.platform not in ("win32", "cygwin", "cli"):
-            import uvloop
-
-            if sys.version_info >= (3, 11):
-                with asyncio.Runner(loop_factory=uvloop.new_event_loop) as runner:
-                    runner.run(propan_app.run(log_level=app_level))
-                    return
-
+            try:
+                import uvloop
+            except Exception:
+                logger.warning("You have no installed `uvloop`")
             else:
                 uvloop.install()
 
         asyncio.run(propan_app.run(log_level=app_level))
```

### Comparing `propan-0.1.0.0/propan/cli/supervisors/basereload.py` & `propan-0.1.1.0/propan/cli/supervisors/basereload.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.0.0/propan/cli/supervisors/multiprocess.py` & `propan-0.1.1.0/propan/cli/supervisors/multiprocess.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.0.0/propan/cli/supervisors/utils.py` & `propan-0.1.1.0/propan/cli/supervisors/utils.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.0.0/propan/cli/supervisors/watchfiles.py` & `propan-0.1.1.0/propan/cli/supervisors/watchfiles.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.0.0/propan/cli/utils/imports.py` & `propan-0.1.1.0/propan/cli/utils/imports.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.0.0/propan/cli/utils/logs.py` & `propan-0.1.1.0/propan/cli/utils/logs.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.0.0/propan/cli/utils/parser.py` & `propan-0.1.1.0/propan/cli/utils/parser.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.0.0/propan/fastapi/core/route.py` & `propan-0.1.1.0/propan/fastapi/core/route.py`

 * *Files 2% similar despite different names*

```diff
@@ -96,15 +96,15 @@
             body=request._body,
             dependant=dependant,
             dependency_overrides_provider=dependency_overrides_provider,
         )
 
         values, errors, _, _2, _3 = solved_result
         if errors:
-            raise ValidationError(errors, create_model("MQRoute"))
+            raise ValidationError(errors, create_model("PropanRoute"))
 
         return await run_endpoint_function(
             dependant=dependant,
             values=values,
             is_coroutine=asyncio.iscoroutinefunction(dependant.call),
         )
```

### Comparing `propan-0.1.0.0/propan/fastapi/core/router.py` & `propan-0.1.1.0/propan/fastapi/core/router.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.0.0/propan/fastapi/rabbit/rabbit_router.pyi` & `propan-0.1.1.0/propan/fastapi/rabbit/router.pyi`

 * *Files identical despite different names*

### Comparing `propan-0.1.0.0/propan/log/formatter.py` & `propan-0.1.1.0/propan/log/formatter.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.0.0/propan/log/logging.py` & `propan-0.1.1.0/propan/log/logging.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.0.0/propan/test/rabbit.py` & `propan-0.1.1.0/propan/test/rabbit.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-import asyncio
 import sys
 from contextlib import asynccontextmanager
 from types import MethodType
 from typing import Any, Optional, Union
 
 from propan.types import AnyDict
 
@@ -20,52 +19,33 @@
 from propan.brokers.rabbit import (
     ExchangeType,
     RabbitBroker,
     RabbitExchange,
     RabbitQueue,
 )
 from propan.brokers.rabbit.rabbit_broker import (  # type: ignore
-    Handler,
     PikaSendableMessage,
     TimeoutType,
     _validate_exchange,
     _validate_queue,
 )
+from propan.test.utils import call_handler
 
 __all__ = (
     "build_message",
     "TestRabbitBroker",
 )
 
 
 class PatchedMessage(IncomingMessage):
     @asynccontextmanager
     async def process(self):  # type: ignore
         yield
 
 
-async def call_handler(
-    handler: Handler,
-    message: IncomingMessage,
-    callback: bool = False,
-    callback_timeout: Optional[float] = 30.0,
-    raise_timeout: bool = False,
-) -> Any:
-    r = handler.callback(message)
-    try:
-        result = await asyncio.wait_for(r, timeout=callback_timeout)
-    except asyncio.TimeoutError as e:
-        if raise_timeout is True:  # pragma: no branch
-            raise e
-        result = None
-
-    if callback is True:  # pragma: no branch
-        return result
-
-
 def build_message(
     message: PikaSendableMessage = "",
     queue: Union[RabbitQueue, str] = "",
     exchange: Union[RabbitExchange, str, None] = None,
     *,
     routing_key: str = "",
     **message_kwargs: AnyDict,
```

### Comparing `propan-0.1.0.0/propan/utils/functions.py` & `propan-0.1.1.0/propan/utils/functions.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.0.0/propan/utils/context/main.py` & `propan-0.1.1.0/propan/utils/context/main.py`

 * *Files 8% similar despite different names*

```diff
@@ -45,14 +45,15 @@
 
     def __getattr__(self, __name: str) -> Any:
         return self.get(__name)
 
     @property
     def context(self) -> Dict[str, Any]:
         return {
+            "context": self,
             **{i: j.get() for i, j in self._scope_context.items()},
             **self._global_context,
         }
 
     @contextmanager
     def scope(self, key: str, value: Any) -> Iterator[None]:
         token = self.set_local(key, value)
```

### Comparing `propan-0.1.0.0/propan/utils/context/types.py` & `propan-0.1.1.0/propan/utils/context/types.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.0.0/LICENSE` & `propan-0.1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `propan-0.1.0.0/README.md` & `propan-0.1.1.0/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -95,607 +95,664 @@
 000005e0: 2020 3c2f 613e 0a3c 2f70 3e0a 0a23 2050    </a>.</p>..# P
 000005f0: 726f 7061 6e0a 0a2a 2a50 726f 7061 6e2a  ropan..**Propan*
 00000600: 2a20 2d20 6a75 7374 202a 7e7e 616e 2061  * - just *~~an a
 00000610: 6e6f 7468 6572 206f 6e65 2048 5454 507e  nother one HTTP~
 00000620: 7e2a 2061 202a 2a64 6563 6c61 7261 7469  ~* a **declarati
 00000630: 7665 2050 7974 686f 6e20 4d51 2066 7261  ve Python MQ fra
 00000640: 6d65 776f 726b 2a2a 2e20 4974 2773 2066  mework**. It's f
-00000650: 6f6c 6c6f 7769 6e67 2062 7920 5b2a 6661  ollowing by [*fa
-00000660: 7374 6170 692a 5d28 6874 7470 733a 2f2f  stapi*](https://
-00000670: 6661 7374 6170 692e 7469 616e 676f 6c6f  fastapi.tiangolo
-00000680: 2e63 6f6d 2f72 752f 292c 0a73 696d 706c  .com/ru/),.simpl
-00000690: 6966 7920 4d65 7373 6167 6520 4272 6f6b  ify Message Brok
-000006a0: 6572 7320 6172 6f75 6e64 2063 6f64 6520  ers around code 
-000006b0: 7772 6974 696e 6720 616e 6420 7072 6f76  writing and prov
-000006c0: 6964 6573 2061 2068 656c 7066 756c 2064  ides a helpful d
-000006d0: 6576 656c 6f70 6d65 6e74 2074 6f6f 6c6b  evelopment toolk
-000006e0: 6974 2c20 7768 6963 6820 6578 6973 7465  it, which existe
-000006f0: 6420 6f6e 6c79 2069 6e20 4854 5450 2d66  d only in HTTP-f
-00000700: 7261 6d65 776f 726b 7320 776f 726c 6420  rameworks world 
-00000710: 756e 7469 6c20 6e6f 772e 0a0a 4974 2773  until now...It's
-00000720: 2064 6573 6967 6e65 6420 746f 2063 7265   designed to cre
-00000730: 6174 6520 7265 6163 7469 7665 206d 6963  ate reactive mic
-00000740: 726f 7365 7276 6963 6573 2061 726f 756e  roservices aroun
-00000750: 6420 3c61 2068 7265 663d 2268 7474 7073  d <a href="https
-00000760: 3a2f 2f6d 6963 726f 7365 7276 6963 6573  ://microservices
-00000770: 2e69 6f2f 7061 7474 6572 6e73 2f63 6f6d  .io/patterns/com
-00000780: 6d75 6e69 6361 7469 6f6e 2d73 7479 6c65  munication-style
-00000790: 2f6d 6573 7361 6769 6e67 2e68 746d 6c22  /messaging.html"
-000007a0: 2074 6172 6765 743d 225f 626c 616e 6b22   target="_blank"
-000007b0: 3e4d 6573 7361 6769 6e67 2041 7263 6869  >Messaging Archi
-000007c0: 7465 6374 7572 653c 2f61 3e2e 0a0a 4974  tecture</a>...It
-000007d0: 2069 7320 6120 6d6f 6465 726e 2c20 6869   is a modern, hi
-000007e0: 6768 2d6c 6576 656c 2066 7261 6d65 776f  gh-level framewo
-000007f0: 726b 206f 6e20 746f 7020 6f66 2070 6f70  rk on top of pop
-00000800: 756c 6172 2073 7065 6369 6669 6320 5079  ular specific Py
-00000810: 7468 6f6e 2062 726f 6b65 7273 206c 6962  thon brokers lib
-00000820: 7261 7269 6573 2c20 6261 7365 6420 6f6e  raries, based on
-00000830: 205b 2a70 7964 616e 7469 632a 5d28 6874   [*pydantic*](ht
-00000840: 7470 733a 2f2f 646f 6373 2e70 7964 616e  tps://docs.pydan
-00000850: 7469 632e 6465 762f 2920 616e 6420 5b2a  tic.dev/) and [*
-00000860: 6661 7374 6170 692a 5d28 6874 7470 733a  fastapi*](https:
-00000870: 2f2f 6661 7374 6170 692e 7469 616e 676f  //fastapi.tiango
-00000880: 6c6f 2e63 6f6d 2f72 752f 292c 205b 2a70  lo.com/ru/), [*p
-00000890: 7974 6573 742a 5d28 6874 7470 733a 2f2f  ytest*](https://
-000008a0: 646f 6373 2e70 7974 6573 742e 6f72 672f  docs.pytest.org/
-000008b0: 656e 2f37 2e33 2e78 2f29 2063 6f6e 6365  en/7.3.x/) conce
-000008c0: 7074 732e 0a0a 2d2d 2d0a 0a2a 2a44 6f63  pts...---..**Doc
-000008d0: 756d 656e 7461 7469 6f6e 2a2a 3a20 3c61  umentation**: <a
-000008e0: 2068 7265 663d 2268 7474 7073 3a2f 2f6c   href="https://l
-000008f0: 616e 6365 746e 696b 2e67 6974 6875 622e  ancetnik.github.
-00000900: 696f 2f50 726f 7061 6e2f 2220 7461 7267  io/Propan/" targ
-00000910: 6574 3d22 5f62 6c61 6e6b 223e 6874 7470  et="_blank">http
-00000920: 733a 2f2f 6c61 6e63 6574 6e69 6b2e 6769  s://lancetnik.gi
-00000930: 7468 7562 2e69 6f2f 5072 6f70 616e 2f3c  thub.io/Propan/<
-00000940: 2f61 3e0a 0a2d 2d2d 0a0a 2323 2320 5468  /a>..---..### Th
-00000950: 6520 6b65 7920 6665 6174 7572 6573 2061  e key features a
-00000960: 7265 0a0a 2a20 2a2a 4561 7379 2a2a 3a20  re..* **Easy**: 
-00000970: 4465 7369 676e 6564 2074 6f20 6265 2065  Designed to be e
-00000980: 6173 7920 746f 2075 7365 2061 6e64 206c  asy to use and l
-00000990: 6561 726e 2e0a 2a20 2a2a 496e 7475 6974  earn..* **Intuit
-000009a0: 6976 652a 2a3a 2047 7265 6174 2065 6469  ive**: Great edi
-000009b0: 746f 7220 7375 7070 6f72 742e 2041 7574  tor support. Aut
-000009c0: 6f63 6f6d 706c 6574 696f 6e20 6576 6572  ocompletion ever
-000009d0: 7977 6865 7265 2e0a 2a20 5b2a 2a44 6570  ywhere..* [**Dep
-000009e0: 656e 6465 6e63 6965 7320 6d61 6e61 6765  endencies manage
-000009f0: 6d65 6e74 2a2a 5d28 2364 6570 656e 6465  ment**](#depende
-00000a00: 6e63 6965 7329 3a20 4d69 6e69 6d69 7a65  ncies): Minimize
-00000a10: 2063 6f64 6520 6475 706c 6963 6174 696f   code duplicatio
-00000a20: 6e2e 204d 756c 7469 706c 6520 6665 6174  n. Multiple feat
-00000a30: 7572 6573 2066 726f 6d20 6561 6368 2061  ures from each a
-00000a40: 7267 756d 656e 7420 616e 6420 7061 7261  rgument and para
-00000a50: 6d65 7465 7220 6465 636c 6172 6174 696f  meter declaratio
-00000a60: 6e2e 0a2a 205b 2a2a 496e 7465 6772 6174  n..* [**Integrat
-00000a70: 696f 6e73 2a2a 5d28 2368 7474 702d 6672  ions**](#http-fr
-00000a80: 616d 6577 6f72 6b73 2d69 6e74 6567 7261  ameworks-integra
-00000a90: 7469 6f6e 7329 3a20 2a2a 5072 6f70 616e  tions): **Propan
-00000aa0: 2a2a 2069 7320 7265 6164 7920 746f 2075  ** is ready to u
-00000ab0: 7365 2069 6e20 7061 6972 2077 6974 6820  se in pair with 
-00000ac0: 5b61 6e79 2048 5454 5020 6672 616d 6577  [any HTTP framew
-00000ad0: 6f72 6b5d 2868 7474 7073 3a2f 2f6c 616e  ork](https://lan
-00000ae0: 6365 746e 696b 2e67 6974 6875 622e 696f  cetnik.github.io
-00000af0: 2f50 726f 7061 6e2f 355f 696e 7465 6772  /Propan/5_integr
-00000b00: 6174 696f 6e73 2f31 5f69 6e74 6567 7261  ations/1_integra
-00000b10: 7469 6f6e 732d 696e 6465 782f 2920 796f  tions-index/) yo
-00000b20: 7520 7761 6e74 0a2a 202a 2a4d 5120 696e  u want.* **MQ in
-00000b30: 6465 7065 6e64 656e 742a 2a3a 2053 696e  dependent**: Sin
-00000b40: 676c 6520 696e 7465 7266 6163 6520 746f  gle interface to
-00000b50: 2070 6f70 756c 6172 204d 513a 0a20 202a   popular MQ:.  *
-00000b60: 202a 2a4e 4154 532a 2a20 2862 6173 6564   **NATS** (based
-00000b70: 206f 6e20 5b6e 6174 732d 7079 5d28 6874   on [nats-py](ht
-00000b80: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-00000b90: 2f6e 6174 732d 696f 2f6e 6174 732e 7079  /nats-io/nats.py
-00000ba0: 2929 200a 2020 2a20 2a2a 5261 6262 6974  )) .  * **Rabbit
-00000bb0: 4d51 2a2a 2028 6261 7365 6420 6f6e 205b  MQ** (based on [
-00000bc0: 6169 6f2d 7069 6b61 5d28 6874 7470 733a  aio-pika](https:
-00000bd0: 2f2f 6169 6f2d 7069 6b61 2e72 6561 6474  //aio-pika.readt
-00000be0: 6865 646f 6373 2e69 6f2f 656e 2f6c 6174  hedocs.io/en/lat
-00000bf0: 6573 742f 2929 0a2a 205b 2a2a 5250 432a  est/)).* [**RPC*
-00000c00: 2a5d 2868 7474 7073 3a2f 2f6c 616e 6365  *](https://lance
-00000c10: 746e 696b 2e67 6974 6875 622e 696f 2f50  tnik.github.io/P
-00000c20: 726f 7061 6e2f 325f 6765 7474 696e 675f  ropan/2_getting_
-00000c30: 7374 6172 7465 642f 345f 6272 6f6b 6572  started/4_broker
-00000c40: 2f35 5f72 7063 2f29 3a20 5468 6520 6672  /5_rpc/): The fr
-00000c50: 616d 6577 6f72 6b20 7375 7070 6f72 7473  amework supports
-00000c60: 2052 5043 2072 6571 7565 7374 7320 6f76   RPC requests ov
-00000c70: 6572 204d 512c 2077 6869 6368 2077 696c  er MQ, which wil
-00000c80: 6c20 616c 6c6f 7720 7065 7266 6f72 6d69  l allow performi
-00000c90: 6e67 206c 6f6e 6720 6f70 6572 6174 696f  ng long operatio
-00000ca0: 6e73 206f 6e20 7265 6d6f 7465 2073 6572  ns on remote ser
-00000cb0: 7669 6365 7320 6173 796e 6368 726f 6e6f  vices asynchrono
-00000cc0: 7573 6c79 2e0a 2a20 5b2a 2a47 7265 6174  usly..* [**Great
-00000cd0: 6520 746f 2064 6576 656c 6f70 2a2a 5d28  e to develop**](
-00000ce0: 2363 6c69 2d70 6f77 6572 293a 2043 4c49  #cli-power): CLI
-00000cf0: 2074 6f6f 6c20 7072 6f76 6964 6573 2067   tool provides g
-00000d00: 7265 6174 2064 6576 656c 6f70 6d65 6e74  reat development
-00000d10: 2065 7870 6572 6965 6e63 653a 0a20 202a   experience:.  *
-00000d20: 2066 7261 6d65 776f 726b 2d69 6e64 6570   framework-indep
-00000d30: 656e 6465 6e74 2077 6179 2074 6f20 7275  endent way to ru
-00000d40: 6c65 2061 7070 6c69 6361 7469 6f6e 2065  le application e
-00000d50: 6e76 6972 6f6e 6d65 6e74 0a20 202a 2061  nvironment.  * a
-00000d60: 7070 6c69 6361 7469 6f6e 2063 6f64 6520  pplication code 
-00000d70: 686f 7420 7265 6c6f 6164 696e 670a 2a20  hot reloading.* 
-00000d80: 5b2a 2a54 6573 7461 6269 6c69 7479 2a2a  [**Testability**
-00000d90: 5d28 6874 7470 733a 2f2f 6c61 6e63 6574  ](https://lancet
-00000da0: 6e69 6b2e 6769 7468 7562 2e69 6f2f 5072  nik.github.io/Pr
-00000db0: 6f70 616e 2f32 5f67 6574 7469 6e67 5f73  opan/2_getting_s
-00000dc0: 7461 7274 6564 2f37 5f74 6573 7469 6e67  tarted/7_testing
-00000dd0: 293a 202a 2a50 726f 7061 6e2a 2a20 616c  ): **Propan** al
-00000de0: 6c6f 7773 2079 6f75 2074 6f20 7465 7374  lows you to test
-00000df0: 2079 6f75 7220 6170 7020 7769 7468 6f75   your app withou
-00000e00: 7420 6578 7465 726e 616c 2064 6570 656e  t external depen
-00000e10: 6465 6e63 6965 733a 2079 6f75 2073 686f  dencies: you sho
-00000e20: 756c 646e 2774 2073 7569 7420 7570 2061  uldn't suit up a
-00000e30: 204d 6573 7361 6765 2042 726f 6b65 722c   Message Broker,
-00000e40: 2075 7365 2061 2076 6972 7475 616c 206f   use a virtual o
-00000e50: 6e65 210a 0a23 2323 2053 7570 706f 7274  ne!..### Support
-00000e60: 6564 204d 5120 6272 6f6b 6572 730a 7c20  ed MQ brokers.| 
-00000e70: 2020 2020 2020 2020 2020 2020 207c 2061               | a
-00000e80: 7379 6e63 2020 2020 2020 2020 2020 2020  sync            
-00000e90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000ea0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000eb0: 2020 2020 2020 207c 2073 796e 6320 2020         | sync   
-00000ec0: 2020 2020 2020 2020 2020 2020 2020 7c0a                |.
-00000ed0: 7c2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d7c  |--------------|
-00000ee0: 3a2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  :---------------
-00000ef0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00000f00: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00000f10: 2d2d 2d2d 2d2d 2d2d 3a7c 3a2d 2d2d 2d2d  --------:|:-----
-00000f20: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d3a  ---------------:
-00000f30: 7c0a 7c20 2a2a 5261 6262 6974 4d51 2a2a  |.| **RabbitMQ**
-00000f40: 207c 203a 6865 6176 795f 6368 6563 6b5f   | :heavy_check_
-00000f50: 6d61 726b 3a20 2a2a 7374 6162 6c65 2a2a  mark: **stable**
-00000f60: 203a 6865 6176 795f 6368 6563 6b5f 6d61   :heavy_check_ma
-00000f70: 726b 3a20 2020 2020 2020 207c 203a 6d61  rk:        | :ma
-00000f80: 673a 2070 6c61 6e6e 696e 6720 3a6d 6167  g: planning :mag
-00000f90: 3a20 7c0a 7c20 2a2a 4e61 7473 2a2a 2020  : |.| **Nats**  
-00000fa0: 2020 207c 203a 7761 726e 696e 673a 202a     | :warning: *
-00000fb0: 2a62 6574 612a 2a20 3a77 6172 6e69 6e67  *beta** :warning
-00000fc0: 3a20 2020 2020 2020 2020 2020 2020 2020  :               
-00000fd0: 2020 2020 2020 2020 2020 2020 207c 203a               | :
-00000fe0: 6d61 673a 2070 6c61 6e6e 696e 6720 3a6d  mag: planning :m
-00000ff0: 6167 3a20 7c0a 7c20 2a2a 4e61 7473 4a53  ag: |.| **NatsJS
-00001000: 2a2a 2020 207c 203a 6861 6d6d 6572 5f61  **   | :hammer_a
-00001010: 6e64 5f77 7265 6e63 683a 202a 2a69 6e20  nd_wrench: **in 
-00001020: 7072 6f67 7265 7373 2a2a 203a 6861 6d6d  progress** :hamm
-00001030: 6572 5f61 6e64 5f77 7265 6e63 683a 207c  er_and_wrench: |
-00001040: 203a 6d61 673a 2070 6c61 6e6e 696e 6720   :mag: planning 
-00001050: 3a6d 6167 3a20 7c0a 7c20 2a2a 4d51 5454  :mag: |.| **MQTT
-00001060: 2a2a 2020 2020 207c 203a 6d61 673a 2070  **     | :mag: p
-00001070: 6c61 6e6e 696e 6720 3a6d 6167 3a20 2020  lanning :mag:   
-00001080: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001090: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000010a0: 207c 203a 6d61 673a 2070 6c61 6e6e 696e   | :mag: plannin
-000010b0: 6720 3a6d 6167 3a20 7c0a 7c20 2a2a 5245  g :mag: |.| **RE
-000010c0: 4449 532a 2a20 2020 207c 203a 6d61 673a  DIS**    | :mag:
-000010d0: 2070 6c61 6e6e 696e 6720 3a6d 6167 3a20   planning :mag: 
-000010e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000010f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001100: 2020 207c 203a 6d61 673a 2070 6c61 6e6e     | :mag: plann
-00001110: 696e 6720 3a6d 6167 3a20 7c0a 7c20 2a2a  ing :mag: |.| **
-00001120: 4b61 666b 612a 2a20 2020 207c 203a 6d61  Kafka**    | :ma
-00001130: 673a 2070 6c61 6e6e 696e 6720 3a6d 6167  g: planning :mag
-00001140: 3a20 2020 2020 2020 2020 2020 2020 2020  :               
-00001150: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001160: 2020 2020 207c 203a 6d61 673a 2070 6c61       | :mag: pla
-00001170: 6e6e 696e 6720 3a6d 6167 3a20 7c0a 7c20  nning :mag: |.| 
-00001180: 2a2a 5351 532a 2a20 2020 2020 207c 203a  **SQS**      | :
-00001190: 6d61 673a 2070 6c61 6e6e 696e 6720 3a6d  mag: planning :m
-000011a0: 6167 3a20 2020 2020 2020 2020 2020 2020  ag:             
-000011b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000011c0: 2020 2020 2020 207c 203a 6d61 673a 2070         | :mag: p
-000011d0: 6c61 6e6e 696e 6720 3a6d 6167 3a20 7c0a  lanning :mag: |.
-000011e0: 0a0a 2323 2320 436f 6d6d 756e 6974 790a  ..### Community.
-000011f0: 0a49 6620 796f 7520 6172 6520 696e 7465  .If you are inte
-00001200: 7265 7374 6564 2069 6e20 7468 6973 2070  rested in this p
-00001210: 726f 6a65 6374 2c20 706c 6561 7365 2067  roject, please g
-00001220: 6976 6520 6d65 2066 6565 6462 6163 6b20  ive me feedback 
-00001230: 6279 2073 7461 7220 6f72 2f61 6e64 2077  by star or/and w
-00001240: 6174 6368 2072 6570 6f73 6974 6f72 792e  atch repository.
-00001250: 0a0a 4966 2079 6f75 2068 6176 6520 616e  ..If you have an
-00001260: 7920 7175 6573 7469 6f6e 7320 6f72 2069  y questions or i
-00001270: 6465 6173 2061 626f 7574 2066 6561 7475  deas about featu
-00001280: 7265 7320 746f 2069 6d70 6c65 6d65 6e74  res to implement
-00001290: 2c20 7765 6c63 6f6d 6520 746f 205b 6469  , welcome to [di
-000012a0: 7363 7573 7369 6f6e 735d 2868 7474 7073  scussions](https
-000012b0: 3a2f 2f67 6974 6875 622e 636f 6d2f 4c61  ://github.com/La
-000012c0: 6e63 6574 6e69 6b2f 5072 6f70 616e 2f64  ncetnik/Propan/d
-000012d0: 6973 6375 7373 696f 6e73 2920 6f72 2070  iscussions) or p
-000012e0: 7562 6c69 6320 5b74 656c 6567 7261 6d20  ublic [telegram 
-000012f0: 6772 6f75 705d 2868 7474 7073 3a2f 2f74  group](https://t
-00001300: 2e6d 652f 7072 6f70 616e 5f70 7974 686f  .me/propan_pytho
-00001310: 6e29 2e0a 0a2d 2d2d 0a0a 2323 2044 6563  n)...---..## Dec
-00001320: 6c61 7261 7469 7665 3f0a 0a57 6974 6820  larative?..With 
-00001330: 6465 636c 6172 6174 6976 6520 746f 6f6c  declarative tool
-00001340: 7320 796f 7520 7368 6f75 6c64 2064 6566  s you should def
-00001350: 696e 6520 2a2a 7768 6174 2079 6f75 206e  ine **what you n
-00001360: 6565 6420 746f 2067 6574 2a2a 2e20 5769  eed to get**. Wi
-00001370: 7468 2074 7261 6469 7469 6f6e 616c 2069  th traditional i
-00001380: 6d70 6572 6174 6976 6520 746f 6f6c 7320  mperative tools 
-00001390: 796f 7520 7368 6f75 6c64 2077 7269 7465  you should write
-000013a0: 202a 2a77 6861 7420 796f 7520 6e65 6564   **what you need
-000013b0: 2074 6f20 646f 2a2a 2e0a 0a54 616b 6520   to do**...Take 
-000013c0: 6120 6c6f 6f6b 2061 7420 636c 6173 7369  a look at classi
-000013d0: 6320 696d 7065 7261 7469 7665 2074 6f6f  c imperative too
-000013e0: 6c73 2c20 7375 6368 2061 7320 5b61 696f  ls, such as [aio
-000013f0: 2d70 696b 615d 2868 7474 7073 3a2f 2f61  -pika](https://a
-00001400: 696f 2d70 696b 612e 7265 6164 7468 6564  io-pika.readthed
-00001410: 6f63 732e 696f 2f65 6e2f 6c61 7465 7374  ocs.io/en/latest
-00001420: 2f29 2c20 5b70 696b 615d 2868 7474 7073  /), [pika](https
-00001430: 3a2f 2f70 696b 612e 7265 6164 7468 6564  ://pika.readthed
-00001440: 6f63 732e 696f 2f65 6e2f 7374 6162 6c65  ocs.io/en/stable
-00001450: 2f29 2c20 5b6e 6174 732d 7079 5d28 6874  /), [nats-py](ht
-00001460: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-00001470: 2f6e 6174 732d 696f 2f6e 6174 732e 7079  /nats-io/nats.py
-00001480: 292c 2065 7463 2e0a 0a54 6869 7320 6973  ), etc...This is
-00001490: 2074 6865 202a 2a51 7569 636b 7374 6172   the **Quickstar
-000014a0: 742a 2a20 7769 7468 2074 6865 202a 6169  t** with the *ai
-000014b0: 6f2d 7069 6b61 2a3a 0a0a 6060 6070 7974  o-pika*:..```pyt
-000014c0: 686f 6e0a 696d 706f 7274 2061 7379 6e63  hon.import async
-000014d0: 696f 0a69 6d70 6f72 7420 6169 6f5f 7069  io.import aio_pi
-000014e0: 6b61 0a0a 6173 796e 6320 6465 6620 6d61  ka..async def ma
-000014f0: 696e 2829 3a0a 2020 2020 636f 6e6e 6563  in():.    connec
-00001500: 7469 6f6e 203d 2061 7761 6974 2061 696f  tion = await aio
-00001510: 5f70 696b 612e 636f 6e6e 6563 745f 726f  _pika.connect_ro
-00001520: 6275 7374 280a 2020 2020 2020 2020 2261  bust(.        "a
-00001530: 6d71 703a 2f2f 6775 6573 743a 6775 6573  mqp://guest:gues
-00001540: 7440 3132 372e 302e 302e 312f 220a 2020  t@127.0.0.1/".  
-00001550: 2020 290a 0a20 2020 2071 7565 7565 5f6e    )..    queue_n
-00001560: 616d 6520 3d20 2274 6573 745f 7175 6575  ame = "test_queu
-00001570: 6522 0a0a 2020 2020 6173 796e 6320 7769  e"..    async wi
-00001580: 7468 2063 6f6e 6e65 6374 696f 6e3a 0a20  th connection:. 
-00001590: 2020 2020 2020 2063 6861 6e6e 656c 203d         channel =
-000015a0: 2061 7761 6974 2063 6f6e 6e65 6374 696f   await connectio
-000015b0: 6e2e 6368 616e 6e65 6c28 290a 0a20 2020  n.channel()..   
-000015c0: 2020 2020 2071 7565 7565 203d 2061 7761       queue = awa
-000015d0: 6974 2063 6861 6e6e 656c 2e64 6563 6c61  it channel.decla
-000015e0: 7265 5f71 7565 7565 2871 7565 7565 5f6e  re_queue(queue_n
-000015f0: 616d 6529 0a0a 2020 2020 2020 2020 6173  ame)..        as
-00001600: 796e 6320 7769 7468 2071 7565 7565 2e69  ync with queue.i
-00001610: 7465 7261 746f 7228 2920 6173 2071 7565  terator() as que
-00001620: 7565 5f69 7465 723a 0a20 2020 2020 2020  ue_iter:.       
-00001630: 2020 2020 2061 7379 6e63 2066 6f72 206d       async for m
-00001640: 6573 7361 6765 2069 6e20 7175 6575 655f  essage in queue_
-00001650: 6974 6572 3a0a 2020 2020 2020 2020 2020  iter:.          
-00001660: 2020 2020 2020 6173 796e 6320 7769 7468        async with
-00001670: 206d 6573 7361 6765 2e70 726f 6365 7373   message.process
-00001680: 2829 3a0a 2020 2020 2020 2020 2020 2020  ():.            
-00001690: 2020 2020 2020 2020 7072 696e 7428 6d65          print(me
-000016a0: 7373 6167 652e 626f 6479 290a 0a61 7379  ssage.body)..asy
-000016b0: 6e63 696f 2e72 756e 286d 6169 6e28 2929  ncio.run(main())
-000016c0: 0a60 6060 0a0a 2a2a 6169 6f2d 7069 6b61  .```..**aio-pika
-000016d0: 2a2a 2069 7320 6120 7265 616c 6c79 2067  ** is a really g
-000016e0: 7265 6174 2074 6f6f 6c20 7769 7468 2061  reat tool with a
-000016f0: 2072 6561 6c6c 7920 6561 7379 206c 6561   really easy lea
-00001700: 726e 696e 6720 6375 7276 652e 2042 7574  rning curve. But
-00001710: 2069 7427 7320 7374 696c 6c20 696d 7065   it's still impe
-00001720: 7261 7469 7665 2e20 596f 7520 6e65 6564  rative. You need
-00001730: 2074 6f20 2a63 6f6e 6e65 6374 2a2c 2064   to *connect*, d
-00001740: 6563 6c61 7265 202a 6368 616e 6e65 6c2a  eclare *channel*
-00001750: 2c20 2a71 7565 7565 732a 2c20 2a65 7863  , *queues*, *exc
-00001760: 6861 6e67 6573 2a20 6279 2079 6f75 7273  hanges* by yours
-00001770: 656c 662e 2041 6c73 6f2c 2079 6f75 206e  elf. Also, you n
-00001780: 6565 6420 746f 206d 616e 6167 6520 2a63  eed to manage *c
-00001790: 6f6e 6e65 6374 696f 6e2a 2c20 2a6d 6573  onnection*, *mes
-000017a0: 7361 6765 2a2c 202a 7175 6575 652a 2063  sage*, *queue* c
-000017b0: 6f6e 7465 7874 2074 6f20 6176 6f69 6420  ontext to avoid 
-000017c0: 616e 7920 7472 6f75 626c 6573 2e0a 0a49  any troubles...I
-000017d0: 7420 6973 206e 6f74 2061 2062 6164 2077  t is not a bad w
-000017e0: 6179 2c20 6275 7420 6974 2063 616e 2062  ay, but it can b
-000017f0: 6520 6561 7379 2e0a 0a60 6060 7079 7468  e easy...```pyth
-00001800: 6f6e 0a66 726f 6d20 7072 6f70 616e 2069  on.from propan i
-00001810: 6d70 6f72 7420 5072 6f70 616e 4170 702c  mport PropanApp,
-00001820: 2052 6162 6269 7442 726f 6b65 720a 0a62   RabbitBroker..b
-00001830: 726f 6b65 7220 3d20 5261 6262 6974 4272  roker = RabbitBr
-00001840: 6f6b 6572 2822 616d 7170 3a2f 2f67 7565  oker("amqp://gue
-00001850: 7374 3a67 7565 7374 406c 6f63 616c 686f  st:guest@localho
-00001860: 7374 3a35 3637 322f 2229 0a0a 6170 7020  st:5672/")..app 
-00001870: 3d20 5072 6f70 616e 4170 7028 6272 6f6b  = PropanApp(brok
-00001880: 6572 290a 0a40 6272 6f6b 6572 2e68 616e  er)..@broker.han
-00001890: 646c 6528 2274 6573 745f 7175 6575 6522  dle("test_queue"
-000018a0: 290a 6173 796e 6320 6465 6620 6261 7365  ).async def base
-000018b0: 5f68 616e 646c 6572 2862 6f64 7929 3a0a  _handler(body):.
-000018c0: 2020 2020 7072 696e 7428 626f 6479 290a      print(body).
-000018d0: 6060 600a 0a54 6869 7320 6973 2074 6865  ```..This is the
-000018e0: 202a 2a50 726f 7061 6e2a 2a20 6465 636c   **Propan** decl
-000018f0: 6172 6174 6976 6520 7761 7920 746f 2077  arative way to w
-00001900: 7269 7465 2074 6865 2073 616d 6520 636f  rite the same co
-00001910: 6465 2e20 5468 6174 2069 7320 736f 206d  de. That is so m
-00001920: 7563 6820 6561 7369 6572 2c20 6973 6e27  uch easier, isn'
-00001930: 7420 6974 3f0a 0a2d 2d2d 0a0a 2323 2051  t it?..---..## Q
-00001940: 7569 636b 7374 6172 740a 0a49 6e73 7461  uickstart..Insta
-00001950: 6c6c 2075 7369 6e67 2060 7069 7060 3a0a  ll using `pip`:.
-00001960: 0a60 6060 7368 656c 6c0a 2420 7069 7020  .```shell.$ pip 
-00001970: 696e 7374 616c 6c20 2270 726f 7061 6e5b  install "propan[
-00001980: 6173 796e 632d 7261 6262 6974 5d22 0a23  async-rabbit]".#
-00001990: 206f 720a 2420 7069 7020 696e 7374 616c   or.$ pip instal
-000019a0: 6c20 2270 726f 7061 6e5b 6173 796e 632d  l "propan[async-
-000019b0: 6e61 7473 5d22 0a60 6060 0a0a 2323 2320  nats]".```..### 
-000019c0: 4261 7369 6320 7573 6167 650a 0a43 7265  Basic usage..Cre
-000019d0: 6174 6520 616e 2061 7070 6c69 6361 7469  ate an applicati
-000019e0: 6f6e 2077 6974 6820 7468 6520 666f 6c6c  on with the foll
-000019f0: 6f77 696e 6720 636f 6465 2061 7420 6073  owing code at `s
-00001a00: 6572 7665 2e70 7960 3a0a 0a60 6060 7079  erve.py`:..```py
-00001a10: 7468 6f6e 0a66 726f 6d20 7072 6f70 616e  thon.from propan
-00001a20: 2069 6d70 6f72 7420 5072 6f70 616e 4170   import PropanAp
-00001a30: 700a 6672 6f6d 2070 726f 7061 6e20 696d  p.from propan im
-00001a40: 706f 7274 2052 6162 6269 7442 726f 6b65  port RabbitBroke
-00001a50: 720a 2320 6672 6f6d 2070 726f 7061 6e20  r.# from propan 
-00001a60: 696d 706f 7274 204e 6174 7342 726f 6b65  import NatsBroke
-00001a70: 720a 0a62 726f 6b65 7220 3d20 5261 6262  r..broker = Rabb
-00001a80: 6974 4272 6f6b 6572 2822 616d 7170 3a2f  itBroker("amqp:/
-00001a90: 2f67 7565 7374 3a67 7565 7374 406c 6f63  /guest:guest@loc
-00001aa0: 616c 686f 7374 3a35 3637 322f 2229 0a23  alhost:5672/").#
-00001ab0: 2062 726f 6b65 7220 3d20 4e61 7473 4272   broker = NatsBr
-00001ac0: 6f6b 6572 2822 6e61 7473 3a2f 2f6c 6f63  oker("nats://loc
-00001ad0: 616c 686f 7374 3a34 3232 3222 290a 0a61  alhost:4222")..a
-00001ae0: 7070 203d 2050 726f 7061 6e41 7070 2862  pp = PropanApp(b
-00001af0: 726f 6b65 7229 0a0a 4062 726f 6b65 722e  roker)..@broker.
-00001b00: 6861 6e64 6c65 2822 7465 7374 2229 0a61  handle("test").a
-00001b10: 7379 6e63 2064 6566 2062 6173 655f 6861  sync def base_ha
-00001b20: 6e64 6c65 7228 626f 6479 293a 0a20 2020  ndler(body):.   
-00001b30: 2027 2727 4861 6e64 6c65 2061 6c6c 2064   '''Handle all d
-00001b40: 6566 6175 6c74 2065 7863 6861 6e67 6520  efault exchange 
-00001b50: 6d65 7373 6167 6573 2077 6974 6820 6074  messages with `t
-00001b60: 6573 7460 2072 6f75 7469 6e67 206b 6579  est` routing key
-00001b70: 2727 270a 2020 2020 7072 696e 7428 626f  '''.    print(bo
-00001b80: 6479 290a 6060 600a 0a41 6e64 206a 7573  dy).```..And jus
-00001b90: 7420 7275 6e20 6974 3a0a 0a60 6060 7368  t run it:..```sh
-00001ba0: 656c 6c0a 2420 7072 6f70 616e 2072 756e  ell.$ propan run
-00001bb0: 2073 6572 7665 3a61 7070 0a60 6060 0a0a   serve:app.```..
-00001bc0: 2d2d 2d0a 0a23 2320 5479 7065 2063 6173  ---..## Type cas
-00001bd0: 7469 6e67 0a0a 5072 6f70 616e 2075 7365  ting..Propan use
-00001be0: 7320 6070 7964 616e 7469 6360 2074 6f20  s `pydantic` to 
-00001bf0: 6361 7374 2069 6e63 6f6d 696e 6720 6675  cast incoming fu
-00001c00: 6e63 7469 6f6e 2061 7267 756d 656e 7473  nction arguments
-00001c10: 2074 6f20 7479 7065 7320 6163 636f 7264   to types accord
-00001c20: 696e 6720 746f 2074 6865 6972 2061 6e6e  ing to their ann
-00001c30: 6f74 6174 696f 6e2e 0a0a 6060 6070 7974  otation...```pyt
-00001c40: 686f 6e0a 6672 6f6d 2070 7964 616e 7469  hon.from pydanti
-00001c50: 6320 696d 706f 7274 2042 6173 654d 6f64  c import BaseMod
-00001c60: 656c 0a66 726f 6d20 7072 6f70 616e 2069  el.from propan i
-00001c70: 6d70 6f72 7420 5072 6f70 616e 4170 702c  mport PropanApp,
-00001c80: 2043 6f6e 7465 7874 2c20 5261 6262 6974   Context, Rabbit
-00001c90: 4272 6f6b 6572 0a0a 6272 6f6b 6572 203d  Broker..broker =
-00001ca0: 2052 6162 6269 7442 726f 6b65 7228 2261   RabbitBroker("a
-00001cb0: 6d71 703a 2f2f 6775 6573 743a 6775 6573  mqp://guest:gues
-00001cc0: 7440 6c6f 6361 6c68 6f73 743a 3536 3732  t@localhost:5672
-00001cd0: 2f22 290a 6170 7020 3d20 5072 6f70 616e  /").app = Propan
-00001ce0: 4170 7028 6272 6f6b 6572 290a 0a63 6c61  App(broker)..cla
-00001cf0: 7373 2053 696d 706c 654d 6573 7361 6765  ss SimpleMessage
-00001d00: 2842 6173 654d 6f64 656c 293a 0a20 2020  (BaseModel):.   
-00001d10: 206b 6579 3a20 696e 740a 0a40 6272 6f6b   key: int..@brok
-00001d20: 6572 2e68 616e 646c 6528 2274 6573 7432  er.handle("test2
-00001d30: 2229 0a61 7379 6e63 2064 6566 2073 6563  ").async def sec
-00001d40: 6f6e 645f 6861 6e64 6c65 7228 626f 6479  ond_handler(body
-00001d50: 3a20 5369 6d70 6c65 4d65 7373 6167 6529  : SimpleMessage)
-00001d60: 3a0a 2020 2020 6173 7365 7274 2069 7369  :.    assert isi
-00001d70: 6e73 7461 6e63 6528 626f 6479 2e6b 6579  nstance(body.key
-00001d80: 2c20 696e 7429 0a0a 6060 600a 0a2d 2d2d  , int)..```..---
-00001d90: 0a0a 2323 2044 6570 656e 6465 6e63 6965  ..## Dependencie
-00001da0: 730a 0a2a 2a50 726f 7061 6e2a 2a20 6120  s..**Propan** a 
-00001db0: 6861 7320 6465 7065 6e64 656e 6369 6573  has dependencies
-00001dc0: 206d 616e 6167 656d 656e 7420 706f 6c69   management poli
-00001dd0: 6379 2063 6c6f 7365 2074 6f20 6070 7974  cy close to `pyt
-00001de0: 6573 7420 6669 7874 7572 6573 602e 0a59  est fixtures`..Y
-00001df0: 6f75 2063 616e 2073 7065 6369 6679 2069  ou can specify i
-00001e00: 6e20 6675 6e63 7469 6f6e 7320 6172 6775  n functions argu
-00001e10: 6d65 6e74 7320 7768 6963 6820 6465 7065  ments which depe
-00001e20: 6e64 656e 6369 6573 0a79 6f75 2077 6f75  ndencies.you wou
-00001e30: 6c64 2074 6f20 7573 652e 2046 7261 6d65  ld to use. Frame
-00001e40: 776f 726b 2070 6173 7365 7320 7468 656d  work passes them
-00001e50: 2066 726f 6d20 7468 6520 676c 6f62 616c   from the global
-00001e60: 2043 6f6e 7465 7874 206f 626a 6563 742e   Context object.
-00001e70: 0a0a 416c 7265 6164 7920 6578 6973 7465  ..Already existe
-00001e80: 6420 636f 6e74 6578 7420 6669 656c 6473  d context fields
-00001e90: 2061 7265 3a20 2a61 7070 2a2c 202a 6272   are: *app*, *br
-00001ea0: 6f6b 6572 2a2c 202a 636f 6e74 6578 742a  oker*, *context*
-00001eb0: 2028 6974 7365 6c66 292c 202a 6c6f 6767   (itself), *logg
-00001ec0: 6572 2a20 616e 6420 2a6d 6573 7361 6765  er* and *message
-00001ed0: 2a2e 0a49 6620 796f 7520 6361 6c6c 206e  *..If you call n
-00001ee0: 6f74 2065 7869 7374 696e 6720 6669 656c  ot existing fiel
-00001ef0: 642c 2072 6169 7365 7320 2a70 7964 616e  d, raises *pydan
-00001f00: 7469 632e 5661 6c69 6461 7469 6f6e 4572  tic.ValidationEr
-00001f10: 726f 722a 2076 616c 7565 2e0a 0a42 7574  ror* value...But
-00001f20: 2079 6f75 2063 616e 2073 7065 6369 6679   you can specify
-00001f30: 2079 6f75 7220 6f77 6e20 6465 7065 6e64   your own depend
-00001f40: 656e 6369 6573 2c20 6361 6c6c 2064 6570  encies, call dep
-00001f50: 656e 6465 6e63 6965 7320 6675 6e63 7469  endencies functi
-00001f60: 6f6e 7320 286c 696b 6520 6046 6173 7461  ons (like `Fasta
-00001f70: 7069 2044 6570 656e 6473 6029 0a61 6e64  pi Depends`).and
-00001f80: 205b 6d6f 7265 5d28 6874 7470 733a 2f2f   [more](https://
-00001f90: 6769 7468 7562 2e63 6f6d 2f4c 616e 6365  github.com/Lance
-00001fa0: 746e 696b 2f50 726f 7061 6e2f 7472 6565  tnik/Propan/tree
-00001fb0: 2f6d 6169 6e2f 6578 616d 706c 6573 2f64  /main/examples/d
-00001fc0: 6570 656e 6465 6e63 6965 7329 2e0a 0a60  ependencies)...`
-00001fd0: 6060 7079 7468 6f6e 0a69 6d70 6f72 7420  ``python.import 
-00001fe0: 6169 6f5f 7069 6b61 0a66 726f 6d20 7072  aio_pika.from pr
-00001ff0: 6f70 616e 2069 6d70 6f72 7420 5072 6f70  opan import Prop
-00002000: 616e 4170 702c 2052 6162 6269 7442 726f  anApp, RabbitBro
-00002010: 6b65 722c 2043 6f6e 7465 7874 2c20 4465  ker, Context, De
-00002020: 7065 6e64 730a 0a72 6162 6269 745f 6272  pends..rabbit_br
-00002030: 6f6b 6572 203d 2052 6162 6269 7442 726f  oker = RabbitBro
-00002040: 6b65 7228 2261 6d71 703a 2f2f 6775 6573  ker("amqp://gues
-00002050: 743a 6775 6573 7440 6c6f 6361 6c68 6f73  t:guest@localhos
-00002060: 743a 3536 3732 2f22 290a 0a61 7070 203d  t:5672/")..app =
-00002070: 2050 726f 7061 6e41 7070 2872 6162 6269   PropanApp(rabbi
-00002080: 745f 6272 6f6b 6572 290a 0a61 7379 6e63  t_broker)..async
-00002090: 2064 6566 2064 6570 656e 6465 6e63 7928   def dependency(
-000020a0: 626f 6479 3a20 6469 6374 2920 2d3e 2062  body: dict) -> b
-000020b0: 6f6f 6c3a 0a20 2020 2072 6574 7572 6e20  ool:.    return 
-000020c0: 5472 7565 0a0a 4072 6162 6269 745f 6272  True..@rabbit_br
-000020d0: 6f6b 6572 2e68 616e 646c 6528 2274 6573  oker.handle("tes
-000020e0: 7422 290a 6173 796e 6320 6465 6620 6261  t").async def ba
-000020f0: 7365 5f68 616e 646c 6572 2862 6f64 793a  se_handler(body:
-00002100: 2064 6963 742c 0a20 2020 2020 2020 2020   dict,.         
-00002110: 2020 2020 2020 2020 2020 2020 2020 6465                de
-00002120: 703a 2062 6f6f 6c20 3d20 4465 7065 6e64  p: bool = Depend
-00002130: 7328 6465 7065 6e64 656e 6379 292c 0a20  s(dependency),. 
-00002140: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002150: 2020 2020 2020 6272 6f6b 6572 3a20 5261        broker: Ra
-00002160: 6262 6974 4272 6f6b 6572 203d 2043 6f6e  bbitBroker = Con
-00002170: 7465 7874 2829 293a 0a20 2020 2061 7373  text()):.    ass
-00002180: 6572 7420 6465 7020 6973 2054 7275 650a  ert dep is True.
-00002190: 2020 2020 6173 7365 7274 2062 726f 6b65      assert broke
-000021a0: 7220 6973 2072 6162 6269 745f 6272 6f6b  r is rabbit_brok
-000021b0: 6572 0a60 6060 0a0a 2d2d 2d0a 0a23 2320  er.```..---..## 
-000021c0: 434c 4920 706f 7765 720a 0a2a 2a50 726f  CLI power..**Pro
-000021d0: 7061 6e2a 2a20 6861 7320 6974 7320 6f77  pan** has its ow
-000021e0: 6e20 434c 4920 746f 6f6c 2074 6861 7420  n CLI tool that 
-000021f0: 7072 6f76 6964 6564 2074 6865 2066 6f6c  provided the fol
-00002200: 6c6f 7769 6e67 2066 6561 7475 7265 733a  lowing features:
-00002210: 0a0a 2a20 7072 6f6a 6563 7420 6765 6e65  ..* project gene
-00002220: 7261 7469 6f6e 0a2a 206d 756c 7469 7072  ration.* multipr
-00002230: 6f63 6573 7369 6e67 2077 6f72 6b65 7273  ocessing workers
-00002240: 0a2a 2070 726f 6a65 6374 2068 6f74 2072  .* project hot r
-00002250: 656c 6f61 6469 6e67 0a2a 2063 7573 746f  eloading.* custo
-00002260: 6d20 636f 6d6d 616e 6420 6c69 6e65 2061  m command line a
-00002270: 7267 756d 656e 7473 2070 6173 7369 6e67  rguments passing
-00002280: 0a0a 2323 2320 436f 6e74 6578 7420 7061  ..### Context pa
-00002290: 7373 696e 670a 0a46 6f72 2065 7861 6d70  ssing..For examp
-000022a0: 6c65 3a20 7061 7373 2079 6f75 7220 6375  le: pass your cu
-000022b0: 7272 656e 7420 2a2e 656e 762a 2070 726f  rrent *.env* pro
-000022c0: 6a65 6374 2073 6574 7469 6e67 2074 6f20  ject setting to 
-000022d0: 636f 6e74 6578 740a 0a60 6060 6261 7368  context..```bash
-000022e0: 0a70 726f 7061 6e20 7275 6e20 7365 7276  .propan run serv
-000022f0: 653a 6170 7020 2d2d 656e 763d 2e65 6e76  e:app --env=.env
-00002300: 2e64 6576 0a60 6060 0a0a 6060 6070 7974  .dev.```..```pyt
-00002310: 686f 6e0a 6672 6f6d 2070 726f 7061 6e20  hon.from propan 
-00002320: 696d 706f 7274 2050 726f 7061 6e41 7070  import PropanApp
-00002330: 2c20 5261 6262 6974 4272 6f6b 6572 0a66  , RabbitBroker.f
-00002340: 726f 6d20 7072 6f70 616e 2e61 6e6e 6f74  rom propan.annot
-00002350: 6174 696f 6e73 2069 6d70 6f72 7420 436f  ations import Co
-00002360: 6e74 6578 7452 6570 6f0a 6672 6f6d 2070  ntextRepo.from p
-00002370: 7964 616e 7469 6320 696d 706f 7274 2042  ydantic import B
-00002380: 6173 6553 6574 7469 6e67 730a 0a62 726f  aseSettings..bro
-00002390: 6b65 7220 3d20 5261 6262 6974 4272 6f6b  ker = RabbitBrok
-000023a0: 6572 2822 616d 7170 3a2f 2f67 7565 7374  er("amqp://guest
-000023b0: 3a67 7565 7374 406c 6f63 616c 686f 7374  :guest@localhost
-000023c0: 3a35 3637 322f 2229 0a0a 6170 7020 3d20  :5672/")..app = 
-000023d0: 5072 6f70 616e 4170 7028 6272 6f6b 6572  PropanApp(broker
-000023e0: 290a 0a63 6c61 7373 2053 6574 7469 6e67  )..class Setting
-000023f0: 7328 4261 7365 5365 7474 696e 6773 293a  s(BaseSettings):
-00002400: 0a20 2020 202e 2e2e 0a0a 4061 7070 2e6f  .    .....@app.o
-00002410: 6e5f 7374 6172 7475 700a 6173 796e 6320  n_startup.async 
-00002420: 6465 6620 7365 7475 7028 656e 763a 2073  def setup(env: s
-00002430: 7472 2c20 636f 6e74 6578 743a 2043 6f6e  tr, context: Con
-00002440: 7465 7874 5265 706f 293a 0a20 2020 2073  textRepo):.    s
-00002450: 6574 7469 6e67 7320 3d20 5365 7474 696e  ettings = Settin
-00002460: 6773 285f 656e 765f 6669 6c65 3d65 6e76  gs(_env_file=env
-00002470: 290a 2020 2020 636f 6e74 6578 742e 7365  ).    context.se
-00002480: 745f 676c 6f62 616c 2822 7365 7474 696e  t_global("settin
-00002490: 6773 222c 2073 6574 7469 6e67 7329 0a60  gs", settings).`
-000024a0: 6060 0a0a 2323 2320 5072 6f6a 6563 7420  ``..### Project 
-000024b0: 7465 6d70 6c61 7465 0a0a 416c 736f 2c20  template..Also, 
-000024c0: 2a2a 5072 6f70 616e 2043 4c49 2a2a 2069  **Propan CLI** i
-000024d0: 7320 6162 6c65 2074 6f20 6765 6e65 7261  s able to genera
-000024e0: 7465 2061 2070 726f 6475 6374 696f 6e2d  te a production-
-000024f0: 7265 6164 7920 6170 706c 6963 6174 696f  ready applicatio
-00002500: 6e20 7465 6d70 6c61 7465 3a0a 0a60 6060  n template:..```
-00002510: 6261 7368 0a70 726f 7061 6e20 6372 6561  bash.propan crea
-00002520: 7465 205b 7072 6f6a 6563 746e 616d 655d  te [projectname]
-00002530: 0a60 6060 0a0a 2a4e 6f74 6963 653a 2070  .```..*Notice: p
-00002540: 726f 6a65 6374 2074 656d 706c 6174 6520  roject template 
-00002550: 7265 7175 6972 652a 2060 7079 6461 6e74  require* `pydant
-00002560: 6963 5b64 6f74 656e 765d 6020 2a69 6e73  ic[dotenv]` *ins
-00002570: 7461 6c6c 6174 696f 6e2e 2a0a 0a52 756e  tallation.*..Run
-00002580: 2074 6865 2063 7265 6174 6564 2070 726f   the created pro
-00002590: 6a65 6374 3a0a 0a60 6060 6261 7368 0a23  ject:..```bash.#
-000025a0: 2052 756e 2072 6162 6269 6d71 2066 6972   Run rabbimq fir
-000025b0: 7374 0a64 6f63 6b65 7220 636f 6d70 6f73  st.docker compos
-000025c0: 6520 2d2d 6669 6c65 205b 7072 6f6a 6563  e --file [projec
-000025d0: 746e 616d 655d 2f64 6f63 6b65 722d 636f  tname]/docker-co
-000025e0: 6d70 6f73 652e 7961 6d6c 2075 7020 2d64  mpose.yaml up -d
-000025f0: 0a0a 2320 5275 6e20 7072 6f6a 6563 740a  ..# Run project.
-00002600: 7072 6f70 616e 2072 756e 205b 7072 6f6a  propan run [proj
-00002610: 6563 746e 616d 655d 2e61 7070 2e73 6572  ectname].app.ser
-00002620: 7665 3a61 7070 202d 2d65 6e76 3d2e 656e  ve:app --env=.en
-00002630: 7620 2d2d 7265 6c6f 6164 0a60 6060 0a0a  v --reload.```..
-00002640: 4e6f 7720 796f 7520 6361 6e20 656e 6a6f  Now you can enjo
-00002650: 7920 6120 6e65 7720 6465 7665 6c6f 706d  y a new developm
-00002660: 656e 7420 6578 7065 7269 656e 6365 210a  ent experience!.
-00002670: 0a2d 2d2d 0a0a 2323 2048 5454 5020 4672  .---..## HTTP Fr
-00002680: 616d 6577 6f72 6b73 2069 6e74 6567 7261  ameworks integra
-00002690: 7469 6f6e 730a 0a23 2323 2041 6e79 2046  tions..### Any F
-000026a0: 7261 6d65 776f 726b 0a0a 596f 7520 6361  ramework..You ca
-000026b0: 6e20 7573 6520 2a2a 5072 6f70 616e 2a2a  n use **Propan**
-000026c0: 2060 4d51 4272 6f6b 6572 7360 2077 6974   `MQBrokers` wit
-000026d0: 686f 7574 2060 5072 6f70 616e 4170 7060  hout `PropanApp`
-000026e0: 2e0a 4a75 7374 202a 7374 6172 742a 2061  ..Just *start* a
-000026f0: 6e64 202a 7374 6f70 2a20 7468 656d 2061  nd *stop* them a
-00002700: 6363 6f72 6469 6e67 2074 6f20 796f 7572  ccording to your
-00002710: 2061 7070 6c69 6361 7469 6f6e 206c 6966   application lif
-00002720: 6573 7061 6e2e 0a0a 6060 6070 7974 686f  espan...```pytho
-00002730: 6e0a 6672 6f6d 2070 726f 7061 6e20 696d  n.from propan im
-00002740: 706f 7274 204e 6174 7342 726f 6b65 720a  port NatsBroker.
-00002750: 6672 6f6d 2073 616e 6963 2069 6d70 6f72  from sanic impor
-00002760: 7420 5361 6e69 630a 0a61 7070 203d 2053  t Sanic..app = S
-00002770: 616e 6963 2822 4d79 4865 6c6c 6f57 6f72  anic("MyHelloWor
-00002780: 6c64 4170 7022 290a 6272 6f6b 6572 203d  ldApp").broker =
-00002790: 204e 6174 7342 726f 6b65 7228 226e 6174   NatsBroker("nat
-000027a0: 733a 2f2f 6c6f 6361 6c68 6f73 743a 3432  s://localhost:42
-000027b0: 3232 2229 0a0a 4062 726f 6b65 722e 6861  22")..@broker.ha
-000027c0: 6e64 6c65 2822 7465 7374 2229 0a61 7379  ndle("test").asy
-000027d0: 6e63 2064 6566 2062 6173 655f 6861 6e64  nc def base_hand
-000027e0: 6c65 7228 626f 6479 293a 0a20 2020 2070  ler(body):.    p
-000027f0: 7269 6e74 2862 6f64 7929 0a0a 4061 7070  rint(body)..@app
-00002800: 2e61 6674 6572 5f73 6572 7665 725f 7374  .after_server_st
-00002810: 6172 740a 6173 796e 6320 6465 6620 7374  art.async def st
-00002820: 6172 745f 6272 6f6b 6572 2861 7070 2c20  art_broker(app, 
-00002830: 6c6f 6f70 293a 0a20 2020 2061 7761 6974  loop):.    await
-00002840: 2062 726f 6b65 722e 7374 6172 7428 290a   broker.start().
-00002850: 0a40 6170 702e 6166 7465 725f 7365 7276  .@app.after_serv
-00002860: 6572 5f73 746f 700a 6173 796e 6320 6465  er_stop.async de
-00002870: 6620 7374 6f70 5f62 726f 6b65 7228 6170  f stop_broker(ap
-00002880: 702c 206c 6f6f 7029 3a0a 2020 2020 6177  p, loop):.    aw
-00002890: 6169 7420 6272 6f6b 6572 2e63 6c6f 7365  ait broker.close
-000028a0: 2829 0a60 6060 0a0a 2323 2320 4661 7374  ().```..### Fast
-000028b0: 4150 4920 506c 7567 696e 0a0a 416c 736f  API Plugin..Also
-000028c0: 2c20 2a2a 5072 6f70 616e 2a2a 2063 616e  , **Propan** can
-000028d0: 2062 6520 7573 6564 2061 7320 7061 7274   be used as part
-000028e0: 206f 6620 2a2a 4661 7374 4150 492a 2a2e   of **FastAPI**.
-000028f0: 0a0a 4a75 7374 2069 6d70 6f72 7420 6120  ..Just import a 
-00002900: 2a2a 5072 6f70 616e 526f 7574 6572 2a2a  **PropanRouter**
-00002910: 2079 6f75 206e 6565 6420 616e 6420 6465   you need and de
-00002920: 636c 6172 6520 7468 6520 6d65 7373 6167  clare the messag
-00002930: 6520 6861 6e64 6c65 720a 7573 696e 6720  e handler.using 
-00002940: 7468 6520 6040 6576 656e 7460 2064 6563  the `@event` dec
-00002950: 6f72 6174 6f72 2e20 5468 6973 2064 6563  orator. This dec
-00002960: 6f72 6174 6f72 2069 7320 7369 6d69 6c61  orator is simila
-00002970: 7220 746f 2074 6865 2064 6563 6f72 6174  r to the decorat
-00002980: 6f72 2060 4068 616e 646c 6560 2066 6f72  or `@handle` for
-00002990: 2074 6865 2063 6f72 7265 7370 6f6e 6469   the correspondi
-000029a0: 6e67 2062 726f 6b65 7273 2e0a 0a60 6060  ng brokers...```
-000029b0: 7079 7468 6f6e 0a66 726f 6d20 6661 7374  python.from fast
-000029c0: 6170 6920 696d 706f 7274 2044 6570 656e  api import Depen
-000029d0: 6473 2c20 4661 7374 4150 490a 6672 6f6d  ds, FastAPI.from
-000029e0: 2070 7964 616e 7469 6320 696d 706f 7274   pydantic import
-000029f0: 2042 6173 654d 6f64 656c 0a66 726f 6d20   BaseModel.from 
-00002a00: 7072 6f70 616e 2e66 6173 7461 7069 2069  propan.fastapi i
-00002a10: 6d70 6f72 7420 5261 6262 6974 526f 7574  mport RabbitRout
-00002a20: 6572 0a0a 6170 7020 3d20 4661 7374 4150  er..app = FastAP
-00002a30: 4928 290a 0a72 6f75 7465 7220 3d20 5261  I()..router = Ra
-00002a40: 6262 6974 526f 7574 6572 2822 616d 7170  bbitRouter("amqp
-00002a50: 3a2f 2f67 7565 7374 3a67 7565 7374 406c  ://guest:guest@l
-00002a60: 6f63 616c 686f 7374 3a35 3637 3222 290a  ocalhost:5672").
-00002a70: 0a63 6c61 7373 2049 6e63 6f6d 696e 6728  .class Incoming(
-00002a80: 4261 7365 4d6f 6465 6c29 3a0a 2020 2020  BaseModel):.    
-00002a90: 6d3a 2064 6963 740a 0a64 6566 2063 616c  m: dict..def cal
-00002aa0: 6c28 293a 0a20 2020 2072 6574 7572 6e20  l():.    return 
-00002ab0: 5472 7565 0a0a 4072 6f75 7465 722e 6576  True..@router.ev
-00002ac0: 656e 7428 2274 6573 7422 290a 6173 796e  ent("test").asyn
-00002ad0: 6320 6465 6620 6865 6c6c 6f28 6d3a 2049  c def hello(m: I
-00002ae0: 6e63 6f6d 696e 672c 2064 203d 2044 6570  ncoming, d = Dep
-00002af0: 656e 6473 2863 616c 6c29 2920 2d3e 2064  ends(call)) -> d
-00002b00: 6963 743a 0a20 2020 2072 6574 7572 6e20  ict:.    return 
-00002b10: 7b20 2272 6573 706f 6e73 6522 3a20 2248  { "response": "H
-00002b20: 656c 6c6f 2c20 5072 6f70 616e 2122 207d  ello, Propan!" }
-00002b30: 0a0a 6170 702e 696e 636c 7564 655f 726f  ..app.include_ro
-00002b40: 7574 6572 2872 6f75 7465 7229 0a60 6060  uter(router).```
-00002b50: 0a0a 2323 2045 7861 6d70 6c65 730a 0a54  ..## Examples..T
-00002b60: 6f20 7365 6520 6d6f 7265 2066 7261 6d65  o see more frame
-00002b70: 776f 726b 2075 7361 6765 7320 676f 2074  work usages go t
-00002b80: 6f20 5b2a 2a65 7861 6d70 6c65 732f 2a2a  o [**examples/**
-00002b90: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
-00002ba0: 2e63 6f6d 2f4c 616e 6365 746e 696b 2f50  .com/Lancetnik/P
-00002bb0: 726f 7061 6e2f 7472 6565 2f6d 6169 6e2f  ropan/tree/main/
-00002bc0: 6578 616d 706c 6573 290a                 examples).
+00000650: 6f6c 6c6f 7769 6e67 2062 7920 3c61 2068  ollowing by <a h
+00000660: 7265 663d 2268 7474 7073 3a2f 2f66 6173  ref="https://fas
+00000670: 7461 7069 2e74 6961 6e67 6f6c 6f2e 636f  tapi.tiangolo.co
+00000680: 6d2f 7275 2f22 2074 6172 6765 743d 225f  m/ru/" target="_
+00000690: 626c 616e 6b22 3e2a 6661 7374 6170 692a  blank">*fastapi*
+000006a0: 3c2f 613e 2c20 7369 6d70 6c69 6679 204d  </a>, simplify M
+000006b0: 6573 7361 6765 2042 726f 6b65 7273 2061  essage Brokers a
+000006c0: 726f 756e 6420 636f 6465 2077 7269 7469  round code writi
+000006d0: 6e67 2061 6e64 2070 726f 7669 6465 7320  ng and provides 
+000006e0: 6120 6865 6c70 6675 6c20 6465 7665 6c6f  a helpful develo
+000006f0: 706d 656e 7420 746f 6f6c 6b69 742c 2077  pment toolkit, w
+00000700: 6869 6368 2065 7869 7374 6564 206f 6e6c  hich existed onl
+00000710: 7920 696e 2048 5454 502d 6672 616d 6577  y in HTTP-framew
+00000720: 6f72 6b73 2077 6f72 6c64 2075 6e74 696c  orks world until
+00000730: 206e 6f77 2e0a 0a49 7427 7320 6465 7369   now...It's desi
+00000740: 676e 6564 2074 6f20 6372 6561 7465 2072  gned to create r
+00000750: 6561 6374 6976 6520 6d69 6372 6f73 6572  eactive microser
+00000760: 7669 6365 7320 6172 6f75 6e64 203c 6120  vices around <a 
+00000770: 6872 6566 3d22 6874 7470 733a 2f2f 6d69  href="https://mi
+00000780: 6372 6f73 6572 7669 6365 732e 696f 2f70  croservices.io/p
+00000790: 6174 7465 726e 732f 636f 6d6d 756e 6963  atterns/communic
+000007a0: 6174 696f 6e2d 7374 796c 652f 6d65 7373  ation-style/mess
+000007b0: 6167 696e 672e 6874 6d6c 2220 7461 7267  aging.html" targ
+000007c0: 6574 3d22 5f62 6c61 6e6b 223e 4d65 7373  et="_blank">Mess
+000007d0: 6167 696e 6720 4172 6368 6974 6563 7475  aging Architectu
+000007e0: 7265 3c2f 613e 2e0a 0a49 7420 6973 2061  re</a>...It is a
+000007f0: 206d 6f64 6572 6e2c 2068 6967 682d 6c65   modern, high-le
+00000800: 7665 6c20 6672 616d 6577 6f72 6b20 6f6e  vel framework on
+00000810: 2074 6f70 206f 6620 706f 7075 6c61 7220   top of popular 
+00000820: 7370 6563 6966 6963 2050 7974 686f 6e20  specific Python 
+00000830: 6272 6f6b 6572 7320 6c69 6272 6172 6965  brokers librarie
+00000840: 732c 2062 6173 6564 206f 6e20 3c61 2068  s, based on <a h
+00000850: 7265 663d 2268 7474 7073 3a2f 2f64 6f63  ref="https://doc
+00000860: 732e 7079 6461 6e74 6963 2e64 6576 2f22  s.pydantic.dev/"
+00000870: 2074 6172 6765 743d 225f 626c 616e 6b22   target="_blank"
+00000880: 3e2a 7079 6461 6e74 6963 2a3c 2f61 3e20  >*pydantic*</a> 
+00000890: 616e 6420 3c61 2068 7265 663d 2268 7474  and <a href="htt
+000008a0: 7073 3a2f 2f66 6173 7461 7069 2e74 6961  ps://fastapi.tia
+000008b0: 6e67 6f6c 6f2e 636f 6d2f 7275 2f22 2074  ngolo.com/ru/" t
+000008c0: 6172 6765 743d 225f 626c 616e 6b22 3e2a  arget="_blank">*
+000008d0: 6661 7374 6170 692a 3c2f 613e 2c20 3c61  fastapi*</a>, <a
+000008e0: 2068 7265 663d 2268 7474 7073 3a2f 2f64   href="https://d
+000008f0: 6f63 732e 7079 7465 7374 2e6f 7267 2f65  ocs.pytest.org/e
+00000900: 6e2f 372e 332e 782f 2220 7461 7267 6574  n/7.3.x/" target
+00000910: 3d22 5f62 6c61 6e6b 223e 2a70 7974 6573  ="_blank">*pytes
+00000920: 742a 3c2f 613e 2063 6f6e 6365 7074 732e  t*</a> concepts.
+00000930: 0a0a 2d2d 2d0a 0a2a 2a44 6f63 756d 656e  ..---..**Documen
+00000940: 7461 7469 6f6e 2a2a 3a20 3c61 2068 7265  tation**: <a hre
+00000950: 663d 2268 7474 7073 3a2f 2f6c 616e 6365  f="https://lance
+00000960: 746e 696b 2e67 6974 6875 622e 696f 2f50  tnik.github.io/P
+00000970: 726f 7061 6e2f 2220 7461 7267 6574 3d22  ropan/" target="
+00000980: 5f62 6c61 6e6b 223e 6874 7470 733a 2f2f  _blank">https://
+00000990: 6c61 6e63 6574 6e69 6b2e 6769 7468 7562  lancetnik.github
+000009a0: 2e69 6f2f 5072 6f70 616e 2f3c 2f61 3e0a  .io/Propan/</a>.
+000009b0: 0a2d 2d2d 0a0a 2323 2320 5468 6520 6b65  .---..### The ke
+000009c0: 7920 6665 6174 7572 6573 2061 7265 0a0a  y features are..
+000009d0: 2a20 2a2a 5369 6d70 6c65 2a2a 3a20 4465  * **Simple**: De
+000009e0: 7369 676e 6564 2074 6f20 6265 2065 6173  signed to be eas
+000009f0: 7920 746f 2075 7365 2061 6e64 206c 6561  y to use and lea
+00000a00: 726e 2e0a 2a20 2a2a 496e 7475 6974 6976  rn..* **Intuitiv
+00000a10: 652a 2a3a 2047 7265 6174 2065 6469 746f  e**: Great edito
+00000a20: 7220 7375 7070 6f72 742e 2041 7574 6f63  r support. Autoc
+00000a30: 6f6d 706c 6574 696f 6e20 6576 6572 7977  ompletion everyw
+00000a40: 6865 7265 2e0a 2a20 5b2a 2a44 6570 656e  here..* [**Depen
+00000a50: 6465 6e63 6965 7320 6d61 6e61 6765 6d65  dencies manageme
+00000a60: 6e74 2a2a 5d28 2364 6570 656e 6465 6e63  nt**](#dependenc
+00000a70: 6965 7329 3a20 4d69 6e69 6d69 7a61 7469  ies): Minimizati
+00000a80: 6f6e 206f 6620 636f 6465 2064 7570 6c69  on of code dupli
+00000a90: 6361 7469 6f6e 2e20 4163 6365 7373 2074  cation. Access t
+00000aa0: 6f20 6465 7065 6e64 656e 6369 6573 2061  o dependencies a
+00000ab0: 7420 616e 7920 6c65 7665 6c20 6f66 2074  t any level of t
+00000ac0: 6865 2063 616c 6c20 7374 6163 6b2e 0a2a  he call stack..*
+00000ad0: 205b 2a2a 496e 7465 6772 6174 696f 6e73   [**Integrations
+00000ae0: 2a2a 5d28 2368 7474 702d 6672 616d 6577  **](#http-framew
+00000af0: 6f72 6b73 2d69 6e74 6567 7261 7469 6f6e  orks-integration
+00000b00: 7329 3a20 2a2a 5072 6f70 616e 2a2a 2069  s): **Propan** i
+00000b10: 7320 6675 6c6c 7920 636f 6d70 6174 6962  s fully compatib
+00000b20: 6c65 2077 6974 6820 3c61 2068 7265 663d  le with <a href=
+00000b30: 2268 7474 7073 3a2f 2f6c 616e 6365 746e  "https://lancetn
+00000b40: 696b 2e67 6974 6875 622e 696f 2f50 726f  ik.github.io/Pro
+00000b50: 7061 6e2f 696e 7465 6772 6174 696f 6e73  pan/integrations
+00000b60: 2f31 5f69 6e74 6567 7261 7469 6f6e 732d  /1_integrations-
+00000b70: 696e 6465 782f 2220 7461 7267 6574 3d22  index/" target="
+00000b80: 5f62 6c61 6e6b 223e 616e 7920 4854 5450  _blank">any HTTP
+00000b90: 2066 7261 6d65 776f 726b 3c2f 613e 2079   framework</a> y
+00000ba0: 6f75 2077 616e 740a 2a20 2a2a 4d51 2069  ou want.* **MQ i
+00000bb0: 6e64 6570 656e 6465 6e74 2a2a 3a20 5369  ndependent**: Si
+00000bc0: 6e67 6c65 2069 6e74 6572 6661 6365 2074  ngle interface t
+00000bd0: 6f20 706f 7075 6c61 7220 4d51 3a0a 2020  o popular MQ:.  
+00000be0: 2a20 2a2a 5265 6469 732a 2a20 2862 6173  * **Redis** (bas
+00000bf0: 6564 206f 6e20 3c61 2068 7265 663d 2268  ed on <a href="h
+00000c00: 7474 7073 3a2f 2f72 6564 6973 2e72 6561  ttps://redis.rea
+00000c10: 6474 6865 646f 6373 2e69 6f2f 656e 2f73  dthedocs.io/en/s
+00000c20: 7461 626c 652f 696e 6465 782e 6874 6d6c  table/index.html
+00000c30: 2220 7461 7267 6574 3d22 5f62 6c61 6e6b  " target="_blank
+00000c40: 223e 7265 6469 732d 7079 3c2f 613e 290a  ">redis-py</a>).
+00000c50: 2020 2a20 2a2a 5261 6262 6974 4d51 2a2a    * **RabbitMQ**
+00000c60: 2028 6261 7365 6420 6f6e 203c 6120 6872   (based on <a hr
+00000c70: 6566 3d22 6874 7470 733a 2f2f 6169 6f2d  ef="https://aio-
+00000c80: 7069 6b61 2e72 6561 6474 6865 646f 6373  pika.readthedocs
+00000c90: 2e69 6f2f 656e 2f6c 6174 6573 742f 2220  .io/en/latest/" 
+00000ca0: 7461 7267 6574 3d22 5f62 6c61 6e6b 223e  target="_blank">
+00000cb0: 6169 6f2d 7069 6b61 3c2f 613e 290a 2020  aio-pika</a>).  
+00000cc0: 2a20 2a2a 4e41 5453 2a2a 2028 6261 7365  * **NATS** (base
+00000cd0: 6420 6f6e 203c 6120 6872 6566 3d22 6874  d on <a href="ht
+00000ce0: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+00000cf0: 2f6e 6174 732d 696f 2f6e 6174 732e 7079  /nats-io/nats.py
+00000d00: 2220 7461 7267 6574 3d22 5f62 6c61 6e6b  " target="_blank
+00000d10: 223e 6e61 7473 2d70 793c 2f61 3e29 0a2a  ">nats-py</a>).*
+00000d20: 203c 6120 6872 6566 3d22 6874 7470 733a   <a href="https:
+00000d30: 2f2f 6c61 6e63 6574 6e69 6b2e 6769 7468  //lancetnik.gith
+00000d40: 7562 2e69 6f2f 5072 6f70 616e 2f67 6574  ub.io/Propan/get
+00000d50: 7469 6e67 5f73 7461 7274 6564 2f34 5f62  ting_started/4_b
+00000d60: 726f 6b65 722f 355f 7270 632f 2220 7461  roker/5_rpc/" ta
+00000d70: 7267 6574 3d22 5f62 6c61 6e6b 223e 2a2a  rget="_blank">**
+00000d80: 5250 432a 2a3c 2f61 3e3a 2054 6865 2066  RPC**</a>: The f
+00000d90: 7261 6d65 776f 726b 2073 7570 706f 7274  ramework support
+00000da0: 7320 5250 4320 7265 7175 6573 7473 206f  s RPC requests o
+00000db0: 7665 7220 4d51 2c20 7768 6963 6820 7769  ver MQ, which wi
+00000dc0: 6c6c 2061 6c6c 6f77 2070 6572 666f 726d  ll allow perform
+00000dd0: 696e 6720 6c6f 6e67 206f 7065 7261 7469  ing long operati
+00000de0: 6f6e 7320 6f6e 2072 656d 6f74 6520 7365  ons on remote se
+00000df0: 7276 6963 6573 2061 7379 6e63 6872 6f6e  rvices asynchron
+00000e00: 6f75 736c 792e 0a2a 205b 2a2a 4772 6561  ously..* [**Grea
+00000e10: 7465 2074 6f20 6465 7665 6c6f 702a 2a5d  te to develop**]
+00000e20: 2823 636c 692d 706f 7765 7229 3a20 434c  (#cli-power): CL
+00000e30: 4920 746f 6f6c 2070 726f 7669 6465 7320  I tool provides 
+00000e40: 6772 6561 7420 6465 7665 6c6f 706d 656e  great developmen
+00000e50: 7420 6578 7065 7269 656e 6365 3a0a 2020  t experience:.  
+00000e60: 2a20 6672 616d 6577 6f72 6b2d 696e 6465  * framework-inde
+00000e70: 7065 6e64 656e 7420 7761 7920 746f 206d  pendent way to m
+00000e80: 616e 6167 6520 7468 6520 7072 6f6a 6563  anage the projec
+00000e90: 7420 656e 7669 726f 6e6d 656e 740a 2020  t environment.  
+00000ea0: 2a20 6170 706c 6963 6174 696f 6e20 636f  * application co
+00000eb0: 6465 202a 686f 7420 7265 6c6f 6164 2a0a  de *hot reload*.
+00000ec0: 2020 2a20 726f 6275 7374 2061 7070 6c69    * robust appli
+00000ed0: 6361 7469 6f6e 2074 656d 706c 6174 6573  cation templates
+00000ee0: 0a2a 203c 6120 6872 6566 3d22 6874 7470  .* <a href="http
+00000ef0: 733a 2f2f 6c61 6e63 6574 6e69 6b2e 6769  s://lancetnik.gi
+00000f00: 7468 7562 2e69 6f2f 5072 6f70 616e 2f67  thub.io/Propan/g
+00000f10: 6574 7469 6e67 5f73 7461 7274 6564 2f37  etting_started/7
+00000f20: 5f74 6573 7469 6e67 2220 7461 7267 6574  _testing" target
+00000f30: 3d22 5f62 6c61 6e6b 223e 2a2a 5465 7374  ="_blank">**Test
+00000f40: 6162 696c 6974 792a 2a3c 2f61 3e3a 202a  ability**</a>: *
+00000f50: 2a50 726f 7061 6e2a 2a20 616c 6c6f 7773  *Propan** allows
+00000f60: 2079 6f75 2074 6f20 7465 7374 2079 6f75   you to test you
+00000f70: 7220 6170 7020 7769 7468 6f75 7420 6578  r app without ex
+00000f80: 7465 726e 616c 2064 6570 656e 6465 6e63  ternal dependenc
+00000f90: 6965 733a 2079 6f75 2064 6f20 6e6f 7420  ies: you do not 
+00000fa0: 6861 7665 2074 6f20 7365 7420 7570 2061  have to set up a
+00000fb0: 204d 6573 7361 6765 2042 726f 6b65 722c   Message Broker,
+00000fc0: 2079 6f75 2063 616e 2075 7365 2061 2076   you can use a v
+00000fd0: 6972 7475 616c 206f 6e65 210a 0a23 2323  irtual one!..###
+00000fe0: 2053 7570 706f 7274 6564 204d 5120 6272   Supported MQ br
+00000ff0: 6f6b 6572 730a 0a7c 2020 2020 2020 2020  okers..|        
+00001000: 2020 2020 2020 2020 2020 207c 2061 7379             | asy
+00001010: 6e63 2020 2020 2020 2020 2020 2020 2020  nc              
+00001020: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001030: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001040: 2020 2020 207c 2073 796e 6320 2020 2020       | sync     
+00001050: 2020 2020 2020 2020 2020 2020 7c0a 7c2d              |.|-
+00001060: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00001070: 2d2d 7c3a 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  --|:------------
+00001080: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00001090: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000010a0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d3a 7c3a 2d2d  -----------:|:--
+000010b0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000010c0: 2d2d 3a7c 0a7c 202a 2a52 6162 6269 744d  --:|.| **RabbitM
+000010d0: 512a 2a20 2020 2020 207c 203a 6865 6176  Q**      | :heav
+000010e0: 795f 6368 6563 6b5f 6d61 726b 3a20 2a2a  y_check_mark: **
+000010f0: 7374 6162 6c65 2a2a 203a 6865 6176 795f  stable** :heavy_
+00001100: 6368 6563 6b5f 6d61 726b 3a20 2020 2020  check_mark:     
+00001110: 2020 207c 203a 6d61 673a 2070 6c61 6e6e     | :mag: plann
+00001120: 696e 6720 3a6d 6167 3a20 7c0a 7c20 2a2a  ing :mag: |.| **
+00001130: 5265 6469 732a 2a20 2020 2020 2020 2020  Redis**         
+00001140: 7c20 3a68 6561 7679 5f63 6865 636b 5f6d  | :heavy_check_m
+00001150: 6172 6b3a 202a 2a73 7461 626c 652a 2a20  ark: **stable** 
+00001160: 3a68 6561 7679 5f63 6865 636b 5f6d 6172  :heavy_check_mar
+00001170: 6b3a 2020 2020 2020 2020 7c20 3a6d 6167  k:        | :mag
+00001180: 3a20 706c 616e 6e69 6e67 203a 6d61 673a  : planning :mag:
+00001190: 207c 0a7c 202a 2a4e 6174 732a 2a20 2020   |.| **Nats**   
+000011a0: 2020 2020 2020 207c 203a 7761 726e 696e         | :warnin
+000011b0: 673a 202a 2a62 6574 612a 2a20 3a77 6172  g: **beta** :war
+000011c0: 6e69 6e67 3a20 2020 2020 2020 2020 2020  ning:           
+000011d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000011e0: 207c 203a 6d61 673a 2070 6c61 6e6e 696e   | :mag: plannin
+000011f0: 6720 3a6d 6167 3a20 7c0a 7c20 2a2a 4e61  g :mag: |.| **Na
+00001200: 7473 4a53 2a2a 2020 2020 2020 2020 7c20  tsJS**        | 
+00001210: 3a68 616d 6d65 725f 616e 645f 7772 656e  :hammer_and_wren
+00001220: 6368 3a20 2a2a 696e 2070 726f 6772 6573  ch: **in progres
+00001230: 732a 2a20 3a68 616d 6d65 725f 616e 645f  s** :hammer_and_
+00001240: 7772 656e 6368 3a20 7c20 3a6d 6167 3a20  wrench: | :mag: 
+00001250: 706c 616e 6e69 6e67 203a 6d61 673a 207c  planning :mag: |
+00001260: 0a7c 202a 2a4d 5154 542a 2a20 2020 2020  .| **MQTT**     
+00001270: 2020 2020 207c 203a 6d61 673a 2070 6c61       | :mag: pla
+00001280: 6e6e 696e 6720 3a6d 6167 3a20 2020 2020  nning :mag:     
+00001290: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000012a0: 2020 2020 2020 2020 2020 2020 2020 207c                 |
+000012b0: 203a 6d61 673a 2070 6c61 6e6e 696e 6720   :mag: planning 
+000012c0: 3a6d 6167 3a20 7c0a 7c20 2a2a 4b61 666b  :mag: |.| **Kafk
+000012d0: 612a 2a20 2020 2020 2020 2020 7c20 3a6d  a**         | :m
+000012e0: 6167 3a20 706c 616e 6e69 6e67 203a 6d61  ag: planning :ma
+000012f0: 673a 2020 2020 2020 2020 2020 2020 2020  g:              
+00001300: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001310: 2020 2020 2020 7c20 3a6d 6167 3a20 706c        | :mag: pl
+00001320: 616e 6e69 6e67 203a 6d61 673a 207c 0a7c  anning :mag: |.|
+00001330: 202a 2a52 6564 6973 2053 7472 6561 6d73   **Redis Streams
+00001340: 2a2a 207c 203a 6d61 673a 2070 6c61 6e6e  ** | :mag: plann
+00001350: 696e 6720 3a6d 6167 3a20 2020 2020 2020  ing :mag:       
+00001360: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001370: 2020 2020 2020 2020 2020 2020 207c 203a               | :
+00001380: 6d61 673a 2070 6c61 6e6e 696e 6720 3a6d  mag: planning :m
+00001390: 6167 3a20 7c0a 7c20 2a2a 5075 6c73 6172  ag: |.| **Pulsar
+000013a0: 2a2a 2020 2020 2020 2020 7c20 3a6d 6167  **        | :mag
+000013b0: 3a20 706c 616e 6e69 6e67 203a 6d61 673a  : planning :mag:
+000013c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000013d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000013e0: 2020 2020 7c20 3a6d 6167 3a20 706c 616e      | :mag: plan
+000013f0: 6e69 6e67 203a 6d61 673a 207c 0a7c 202a  ning :mag: |.| *
+00001400: 2a53 5153 2a2a 2020 2020 2020 2020 2020  *SQS**          
+00001410: 207c 203a 6d61 673a 2070 6c61 6e6e 696e   | :mag: plannin
+00001420: 6720 3a6d 6167 3a20 2020 2020 2020 2020  g :mag:         
+00001430: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001440: 2020 2020 2020 2020 2020 207c 203a 6d61             | :ma
+00001450: 673a 2070 6c61 6e6e 696e 6720 3a6d 6167  g: planning :mag
+00001460: 3a20 7c0a 0a23 2323 2043 6f6d 6d75 6e69  : |..### Communi
+00001470: 7479 0a0a 4966 2079 6f75 2061 7265 2069  ty..If you are i
+00001480: 6e74 6572 6573 7465 6420 696e 2074 6869  nterested in thi
+00001490: 7320 7072 6f6a 6563 742c 2070 6c65 6173  s project, pleas
+000014a0: 6520 6769 7665 206d 6520 6665 6564 6261  e give me feedba
+000014b0: 636b 2062 7920 7374 6172 206f 722f 616e  ck by star or/an
+000014c0: 6420 7761 7463 6820 7265 706f 7369 746f  d watch reposito
+000014d0: 7279 2e0a 0a49 6620 796f 7520 6861 7665  ry...If you have
+000014e0: 2061 6e79 2071 7565 7374 696f 6e73 206f   any questions o
+000014f0: 7220 6964 6561 7320 6162 6f75 7420 6665  r ideas about fe
+00001500: 6174 7572 6573 2074 6f20 696d 706c 656d  atures to implem
+00001510: 656e 742c 2077 656c 636f 6d65 2074 6f20  ent, welcome to 
+00001520: 5b64 6973 6375 7373 696f 6e73 5d28 6874  [discussions](ht
+00001530: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+00001540: 2f4c 616e 6365 746e 696b 2f50 726f 7061  /Lancetnik/Propa
+00001550: 6e2f 6469 7363 7573 7369 6f6e 7329 206f  n/discussions) o
+00001560: 7220 7075 626c 6963 205b 7465 6c65 6772  r public [telegr
+00001570: 616d 2067 726f 7570 5d28 6874 7470 733a  am group](https:
+00001580: 2f2f 742e 6d65 2f70 726f 7061 6e5f 7079  //t.me/propan_py
+00001590: 7468 6f6e 292e 0a0a 2d2d 2d0a 0a23 2320  thon)...---..## 
+000015a0: 4465 636c 6172 6174 6976 653f 0a0a 5769  Declarative?..Wi
+000015b0: 7468 2064 6563 6c61 7261 7469 7665 2074  th declarative t
+000015c0: 6f6f 6c73 2079 6f75 2063 616e 2064 6566  ools you can def
+000015d0: 696e 6520 2a2a 7768 6174 2079 6f75 206e  ine **what you n
+000015e0: 6565 6420 746f 2067 6574 2a2a 2e20 5769  eed to get**. Wi
+000015f0: 7468 2074 7261 6469 7469 6f6e 616c 2069  th traditional i
+00001600: 6d70 6572 6174 6976 6520 746f 6f6c 7320  mperative tools 
+00001610: 796f 7520 6d75 7374 2077 7269 7465 202a  you must write *
+00001620: 2a77 6861 7420 796f 7520 6e65 6564 2074  *what you need t
+00001630: 6f20 646f 2a2a 2e0a 0a54 616b 6520 6120  o do**...Take a 
+00001640: 6c6f 6f6b 2061 7420 636c 6173 7369 6320  look at classic 
+00001650: 696d 7065 7261 7469 7665 2074 6f6f 6c73  imperative tools
+00001660: 2c20 7375 6368 2061 7320 3c61 2068 7265  , such as <a hre
+00001670: 663d 2268 7474 7073 3a2f 2f61 696f 2d70  f="https://aio-p
+00001680: 696b 612e 7265 6164 7468 6564 6f63 732e  ika.readthedocs.
+00001690: 696f 2f65 6e2f 6c61 7465 7374 2f22 2074  io/en/latest/" t
+000016a0: 6172 6765 743d 225f 626c 616e 6b22 3e61  arget="_blank">a
+000016b0: 696f 2d70 696b 613c 2f61 3e2c 203c 6120  io-pika</a>, <a 
+000016c0: 6872 6566 3d22 6874 7470 733a 2f2f 7069  href="https://pi
+000016d0: 6b61 2e72 6561 6474 6865 646f 6373 2e69  ka.readthedocs.i
+000016e0: 6f2f 656e 2f73 7461 626c 652f 2220 7461  o/en/stable/" ta
+000016f0: 7267 6574 3d22 5f62 6c61 6e6b 223e 7069  rget="_blank">pi
+00001700: 6b61 3c2f 613e 2c20 3c61 2068 7265 663d  ka</a>, <a href=
+00001710: 2268 7474 7073 3a2f 2f72 6564 6973 2e72  "https://redis.r
+00001720: 6561 6474 6865 646f 6373 2e69 6f2f 656e  eadthedocs.io/en
+00001730: 2f73 7461 626c 652f 696e 6465 782e 6874  /stable/index.ht
+00001740: 6d6c 2220 7461 7267 6574 3d22 5f62 6c61  ml" target="_bla
+00001750: 6e6b 223e 7265 6469 732d 7079 3c2f 613e  nk">redis-py</a>
+00001760: 2c20 3c61 2068 7265 663d 2268 7474 7073  , <a href="https
+00001770: 3a2f 2f67 6974 6875 622e 636f 6d2f 6e61  ://github.com/na
+00001780: 7473 2d69 6f2f 6e61 7473 2e70 7922 2074  ts-io/nats.py" t
+00001790: 6172 6765 743d 225f 626c 616e 6b22 3e6e  arget="_blank">n
+000017a0: 6174 732d 7079 3c2f 613e 2c20 6574 632e  ats-py</a>, etc.
+000017b0: 0a0a 5468 6973 2069 7320 7468 6520 2a2a  ..This is the **
+000017c0: 5175 6963 6b73 7461 7274 2a2a 2077 6974  Quickstart** wit
+000017d0: 6820 7468 6520 2a61 696f 2d70 696b 612a  h the *aio-pika*
+000017e0: 3a0a 0a60 6060 7079 7468 6f6e 0a69 6d70  :..```python.imp
+000017f0: 6f72 7420 6173 796e 6369 6f0a 696d 706f  ort asyncio.impo
+00001800: 7274 2061 696f 5f70 696b 610a 0a61 7379  rt aio_pika..asy
+00001810: 6e63 2064 6566 206d 6169 6e28 293a 0a20  nc def main():. 
+00001820: 2020 2063 6f6e 6e65 6374 696f 6e20 3d20     connection = 
+00001830: 6177 6169 7420 6169 6f5f 7069 6b61 2e63  await aio_pika.c
+00001840: 6f6e 6e65 6374 5f72 6f62 7573 7428 0a20  onnect_robust(. 
+00001850: 2020 2020 2020 2022 616d 7170 3a2f 2f67         "amqp://g
+00001860: 7565 7374 3a67 7565 7374 4031 3237 2e30  uest:guest@127.0
+00001870: 2e30 2e31 2f22 0a20 2020 2029 0a0a 2020  .0.1/".    )..  
+00001880: 2020 7175 6575 655f 6e61 6d65 203d 2022    queue_name = "
+00001890: 7465 7374 5f71 7565 7565 220a 0a20 2020  test_queue"..   
+000018a0: 2061 7379 6e63 2077 6974 6820 636f 6e6e   async with conn
+000018b0: 6563 7469 6f6e 3a0a 2020 2020 2020 2020  ection:.        
+000018c0: 6368 616e 6e65 6c20 3d20 6177 6169 7420  channel = await 
+000018d0: 636f 6e6e 6563 7469 6f6e 2e63 6861 6e6e  connection.chann
+000018e0: 656c 2829 0a0a 2020 2020 2020 2020 7175  el()..        qu
+000018f0: 6575 6520 3d20 6177 6169 7420 6368 616e  eue = await chan
+00001900: 6e65 6c2e 6465 636c 6172 655f 7175 6575  nel.declare_queu
+00001910: 6528 7175 6575 655f 6e61 6d65 290a 0a20  e(queue_name).. 
+00001920: 2020 2020 2020 2061 7379 6e63 2077 6974         async wit
+00001930: 6820 7175 6575 652e 6974 6572 6174 6f72  h queue.iterator
+00001940: 2829 2061 7320 7175 6575 655f 6974 6572  () as queue_iter
+00001950: 3a0a 2020 2020 2020 2020 2020 2020 6173  :.            as
+00001960: 796e 6320 666f 7220 6d65 7373 6167 6520  ync for message 
+00001970: 696e 2071 7565 7565 5f69 7465 723a 0a20  in queue_iter:. 
+00001980: 2020 2020 2020 2020 2020 2020 2020 2061                 a
+00001990: 7379 6e63 2077 6974 6820 6d65 7373 6167  sync with messag
+000019a0: 652e 7072 6f63 6573 7328 293a 0a20 2020  e.process():.   
+000019b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000019c0: 2070 7269 6e74 286d 6573 7361 6765 2e62   print(message.b
+000019d0: 6f64 7929 0a0a 6173 796e 6369 6f2e 7275  ody)..asyncio.ru
+000019e0: 6e28 6d61 696e 2829 290a 6060 600a 0a2a  n(main()).```..*
+000019f0: 2a61 696f 2d70 696b 612a 2a20 6973 2061  *aio-pika** is a
+00001a00: 2067 7265 6174 2074 6f6f 6c20 7769 7468   great tool with
+00001a10: 2061 2072 6561 6c6c 7920 6561 7379 206c   a really easy l
+00001a20: 6561 726e 696e 6720 6375 7276 652e 2042  earning curve. B
+00001a30: 7574 2069 7427 7320 7374 696c 6c20 696d  ut it's still im
+00001a40: 7065 7261 7469 7665 2e20 596f 7520 6e65  perative. You ne
+00001a50: 6564 2074 6f20 2a63 6f6e 6e65 6374 2a2c  ed to *connect*,
+00001a60: 2064 6563 6c61 7265 202a 6368 616e 6e65   declare *channe
+00001a70: 6c2a 2c20 2a71 7565 7565 732a 2c20 2a65  l*, *queues*, *e
+00001a80: 7863 6861 6e67 6573 2a20 6279 2079 6f75  xchanges* by you
+00001a90: 7273 656c 662e 2041 6c73 6f2c 2079 6f75  rself. Also, you
+00001aa0: 206e 6565 6420 746f 206d 616e 6167 6520   need to manage 
+00001ab0: 2a63 6f6e 6e65 6374 696f 6e2a 2c20 2a6d  *connection*, *m
+00001ac0: 6573 7361 6765 2a2c 202a 7175 6575 652a  essage*, *queue*
+00001ad0: 2063 6f6e 7465 7874 2074 6f20 6176 6f69   context to avoi
+00001ae0: 6420 616e 7920 7472 6f75 626c 6573 2e0a  d any troubles..
+00001af0: 0a49 7420 6973 206e 6f74 2061 2062 6164  .It is not a bad
+00001b00: 2077 6179 2c20 6275 7420 6974 2063 616e   way, but it can
+00001b10: 2062 6520 6d75 6368 2065 6173 6965 722e   be much easier.
+00001b20: 0a0a 6060 6070 7974 686f 6e0a 6672 6f6d  ..```python.from
+00001b30: 2070 726f 7061 6e20 696d 706f 7274 2050   propan import P
+00001b40: 726f 7061 6e41 7070 2c20 5261 6262 6974  ropanApp, Rabbit
+00001b50: 4272 6f6b 6572 0a0a 6272 6f6b 6572 203d  Broker..broker =
+00001b60: 2052 6162 6269 7442 726f 6b65 7228 2261   RabbitBroker("a
+00001b70: 6d71 703a 2f2f 6775 6573 743a 6775 6573  mqp://guest:gues
+00001b80: 7440 6c6f 6361 6c68 6f73 743a 3536 3732  t@localhost:5672
+00001b90: 2f22 290a 0a61 7070 203d 2050 726f 7061  /")..app = Propa
+00001ba0: 6e41 7070 2862 726f 6b65 7229 0a0a 4062  nApp(broker)..@b
+00001bb0: 726f 6b65 722e 6861 6e64 6c65 2822 7465  roker.handle("te
+00001bc0: 7374 5f71 7565 7565 2229 0a61 7379 6e63  st_queue").async
+00001bd0: 2064 6566 2062 6173 655f 6861 6e64 6c65   def base_handle
+00001be0: 7228 626f 6479 293a 0a20 2020 2070 7269  r(body):.    pri
+00001bf0: 6e74 2862 6f64 7929 0a60 6060 0a0a 5468  nt(body).```..Th
+00001c00: 6973 2069 7320 7468 6520 2a2a 5072 6f70  is is the **Prop
+00001c10: 616e 2a2a 2064 6563 6c61 7261 7469 7665  an** declarative
+00001c20: 2077 6179 2074 6f20 7772 6974 6520 7468   way to write th
+00001c30: 6520 7361 6d65 2063 6f64 652e 2054 6861  e same code. Tha
+00001c40: 7420 6973 2073 6f20 6d75 6368 2065 6173  t is so much eas
+00001c50: 6965 722c 2069 736e 2774 2069 743f 0a0a  ier, isn't it?..
+00001c60: 2d2d 2d0a 0a23 2320 5175 6963 6b73 7461  ---..## Quicksta
+00001c70: 7274 0a0a 496e 7374 616c 6c20 7573 696e  rt..Install usin
+00001c80: 6720 6070 6970 603a 0a0a 6060 6073 6865  g `pip`:..```she
+00001c90: 6c6c 0a24 2070 6970 2069 6e73 7461 6c6c  ll.$ pip install
+00001ca0: 2022 7072 6f70 616e 5b61 7379 6e63 2d72   "propan[async-r
+00001cb0: 6162 6269 745d 220a 2320 6f72 0a24 2070  abbit]".# or.$ p
+00001cc0: 6970 2069 6e73 7461 6c6c 2022 7072 6f70  ip install "prop
+00001cd0: 616e 5b61 7379 6e63 2d6e 6174 735d 220a  an[async-nats]".
+00001ce0: 6060 600a 0a23 2323 2042 6173 6963 2075  ```..### Basic u
+00001cf0: 7361 6765 0a0a 4372 6561 7465 2061 6e20  sage..Create an 
+00001d00: 6170 706c 6963 6174 696f 6e20 7769 7468  application with
+00001d10: 2074 6865 2066 6f6c 6c6f 7769 6e67 2063   the following c
+00001d20: 6f64 6520 6174 2060 7365 7276 652e 7079  ode at `serve.py
+00001d30: 603a 0a0a 6060 6070 7974 686f 6e0a 6672  `:..```python.fr
+00001d40: 6f6d 2070 726f 7061 6e20 696d 706f 7274  om propan import
+00001d50: 2050 726f 7061 6e41 7070 0a66 726f 6d20   PropanApp.from 
+00001d60: 7072 6f70 616e 2069 6d70 6f72 7420 5261  propan import Ra
+00001d70: 6262 6974 4272 6f6b 6572 0a23 2066 726f  bbitBroker.# fro
+00001d80: 6d20 7072 6f70 616e 2069 6d70 6f72 7420  m propan import 
+00001d90: 5265 6469 7342 726f 6b65 720a 2320 6672  RedisBroker.# fr
+00001da0: 6f6d 2070 726f 7061 6e20 696d 706f 7274  om propan import
+00001db0: 204e 6174 7342 726f 6b65 720a 0a62 726f   NatsBroker..bro
+00001dc0: 6b65 7220 3d20 5261 6262 6974 4272 6f6b  ker = RabbitBrok
+00001dd0: 6572 2822 616d 7170 3a2f 2f67 7565 7374  er("amqp://guest
+00001de0: 3a67 7565 7374 406c 6f63 616c 686f 7374  :guest@localhost
+00001df0: 3a35 3637 322f 2229 0a23 2062 726f 6b65  :5672/").# broke
+00001e00: 7220 3d20 4e61 7473 4272 6f6b 6572 2822  r = NatsBroker("
+00001e10: 6e61 7473 3a2f 2f6c 6f63 616c 686f 7374  nats://localhost
+00001e20: 3a34 3232 3222 290a 2320 6272 6f6b 6572  :4222").# broker
+00001e30: 203d 2052 6564 6973 4272 6f6b 6572 2822   = RedisBroker("
+00001e40: 7265 6469 733a 2f2f 6c6f 6361 6c68 6f73  redis://localhos
+00001e50: 743a 3633 3739 2229 0a0a 6170 7020 3d20  t:6379")..app = 
+00001e60: 5072 6f70 616e 4170 7028 6272 6f6b 6572  PropanApp(broker
+00001e70: 290a 0a40 6272 6f6b 6572 2e68 616e 646c  )..@broker.handl
+00001e80: 6528 2274 6573 7422 290a 6173 796e 6320  e("test").async 
+00001e90: 6465 6620 6261 7365 5f68 616e 646c 6572  def base_handler
+00001ea0: 2862 6f64 7929 3a0a 2020 2020 2727 2748  (body):.    '''H
+00001eb0: 616e 646c 6520 616c 6c20 6465 6661 756c  andle all defaul
+00001ec0: 7420 6578 6368 616e 6765 206d 6573 7361  t exchange messa
+00001ed0: 6765 7320 7769 7468 2060 7465 7374 6020  ges with `test` 
+00001ee0: 726f 7574 696e 6720 6b65 7927 2727 0a20  routing key'''. 
+00001ef0: 2020 2070 7269 6e74 2862 6f64 7929 0a60     print(body).`
+00001f00: 6060 0a0a 416e 6420 6a75 7374 2072 756e  ``..And just run
+00001f10: 2069 743a 0a0a 6060 6073 6865 6c6c 0a24   it:..```shell.$
+00001f20: 2070 726f 7061 6e20 7275 6e20 7365 7276   propan run serv
+00001f30: 653a 6170 700a 6060 600a 0a2d 2d2d 0a0a  e:app.```..---..
+00001f40: 2323 2054 7970 6520 6361 7374 696e 670a  ## Type casting.
+00001f50: 0a50 726f 7061 6e20 7573 6573 2060 7079  .Propan uses `py
+00001f60: 6461 6e74 6963 6020 746f 2063 6173 7420  dantic` to cast 
+00001f70: 696e 636f 6d69 6e67 2066 756e 6374 696f  incoming functio
+00001f80: 6e20 6172 6775 6d65 6e74 7320 746f 2074  n arguments to t
+00001f90: 7970 6573 2061 6363 6f72 6469 6e67 2074  ypes according t
+00001fa0: 6f20 7468 6569 7220 616e 6e6f 7461 7469  o their annotati
+00001fb0: 6f6e 2e0a 0a60 6060 7079 7468 6f6e 0a66  on...```python.f
+00001fc0: 726f 6d20 7079 6461 6e74 6963 2069 6d70  rom pydantic imp
+00001fd0: 6f72 7420 4261 7365 4d6f 6465 6c0a 6672  ort BaseModel.fr
+00001fe0: 6f6d 2070 726f 7061 6e20 696d 706f 7274  om propan import
+00001ff0: 2050 726f 7061 6e41 7070 2c20 436f 6e74   PropanApp, Cont
+00002000: 6578 742c 2052 6162 6269 7442 726f 6b65  ext, RabbitBroke
+00002010: 720a 0a62 726f 6b65 7220 3d20 5261 6262  r..broker = Rabb
+00002020: 6974 4272 6f6b 6572 2822 616d 7170 3a2f  itBroker("amqp:/
+00002030: 2f67 7565 7374 3a67 7565 7374 406c 6f63  /guest:guest@loc
+00002040: 616c 686f 7374 3a35 3637 322f 2229 0a61  alhost:5672/").a
+00002050: 7070 203d 2050 726f 7061 6e41 7070 2862  pp = PropanApp(b
+00002060: 726f 6b65 7229 0a0a 636c 6173 7320 5369  roker)..class Si
+00002070: 6d70 6c65 4d65 7373 6167 6528 4261 7365  mpleMessage(Base
+00002080: 4d6f 6465 6c29 3a0a 2020 2020 6b65 793a  Model):.    key:
+00002090: 2069 6e74 0a0a 4062 726f 6b65 722e 6861   int..@broker.ha
+000020a0: 6e64 6c65 2822 7465 7374 3222 290a 6173  ndle("test2").as
+000020b0: 796e 6320 6465 6620 7365 636f 6e64 5f68  ync def second_h
+000020c0: 616e 646c 6572 2862 6f64 793a 2053 696d  andler(body: Sim
+000020d0: 706c 654d 6573 7361 6765 293a 0a20 2020  pleMessage):.   
+000020e0: 2061 7373 6572 7420 6973 696e 7374 616e   assert isinstan
+000020f0: 6365 2862 6f64 792e 6b65 792c 2069 6e74  ce(body.key, int
+00002100: 290a 0a60 6060 0a0a 2d2d 2d0a 0a23 2320  )..```..---..## 
+00002110: 4465 7065 6e64 656e 6369 6573 0a0a 2a2a  Dependencies..**
+00002120: 5072 6f70 616e 2a2a 2061 2068 6173 2064  Propan** a has d
+00002130: 6570 656e 6465 6e63 6965 7320 6d61 6e61  ependencies mana
+00002140: 6765 6d65 6e74 2070 6f6c 6963 7920 636c  gement policy cl
+00002150: 6f73 6520 746f 2060 7079 7465 7374 2066  ose to `pytest f
+00002160: 6978 7475 7265 7360 2e0a 596f 7520 6361  ixtures`..You ca
+00002170: 6e20 7370 6563 6966 7920 696e 2066 756e  n specify in fun
+00002180: 6374 696f 6e73 2061 7267 756d 656e 7473  ctions arguments
+00002190: 2077 6869 6368 2064 6570 656e 6465 6e63   which dependenc
+000021a0: 6965 730a 796f 7520 776f 756c 6420 746f  ies.you would to
+000021b0: 2075 7365 2e20 4672 616d 6577 6f72 6b20   use. Framework 
+000021c0: 7061 7373 6573 2074 6865 6d20 6672 6f6d  passes them from
+000021d0: 2074 6865 2067 6c6f 6261 6c20 436f 6e74   the global Cont
+000021e0: 6578 7420 6f62 6a65 6374 2e0a 0a41 6c72  ext object...Alr
+000021f0: 6561 6479 2065 7869 7374 6564 2063 6f6e  eady existed con
+00002200: 7465 7874 2066 6965 6c64 7320 6172 653a  text fields are:
+00002210: 202a 6170 702a 2c20 2a62 726f 6b65 722a   *app*, *broker*
+00002220: 2c20 2a63 6f6e 7465 7874 2a20 2869 7473  , *context* (its
+00002230: 656c 6629 2c20 2a6c 6f67 6765 722a 2061  elf), *logger* a
+00002240: 6e64 202a 6d65 7373 6167 652a 2e0a 4966  nd *message*..If
+00002250: 2079 6f75 2063 616c 6c20 6e6f 7420 6578   you call not ex
+00002260: 6973 7469 6e67 2066 6965 6c64 2c20 7261  isting field, ra
+00002270: 6973 6573 202a 7079 6461 6e74 6963 2e56  ises *pydantic.V
+00002280: 616c 6964 6174 696f 6e45 7272 6f72 2a20  alidationError* 
+00002290: 7661 6c75 652e 0a0a 4275 7420 796f 7520  value...But you 
+000022a0: 6361 6e20 7370 6563 6966 7920 796f 7572  can specify your
+000022b0: 206f 776e 2064 6570 656e 6465 6e63 6965   own dependencie
+000022c0: 732c 2063 616c 6c20 6465 7065 6e64 656e  s, call dependen
+000022d0: 6369 6573 2066 756e 6374 696f 6e73 2028  cies functions (
+000022e0: 6c69 6b65 2060 4661 7374 6170 6920 4465  like `Fastapi De
+000022f0: 7065 6e64 7360 290a 616e 6420 5b6d 6f72  pends`).and [mor
+00002300: 655d 2868 7474 7073 3a2f 2f67 6974 6875  e](https://githu
+00002310: 622e 636f 6d2f 4c61 6e63 6574 6e69 6b2f  b.com/Lancetnik/
+00002320: 5072 6f70 616e 2f74 7265 652f 6d61 696e  Propan/tree/main
+00002330: 2f65 7861 6d70 6c65 732f 6465 7065 6e64  /examples/depend
+00002340: 656e 6369 6573 292e 0a0a 6060 6070 7974  encies)...```pyt
+00002350: 686f 6e0a 696d 706f 7274 2061 696f 5f70  hon.import aio_p
+00002360: 696b 610a 6672 6f6d 2070 726f 7061 6e20  ika.from propan 
+00002370: 696d 706f 7274 2050 726f 7061 6e41 7070  import PropanApp
+00002380: 2c20 5261 6262 6974 4272 6f6b 6572 2c20  , RabbitBroker, 
+00002390: 436f 6e74 6578 742c 2044 6570 656e 6473  Context, Depends
+000023a0: 0a0a 7261 6262 6974 5f62 726f 6b65 7220  ..rabbit_broker 
+000023b0: 3d20 5261 6262 6974 4272 6f6b 6572 2822  = RabbitBroker("
+000023c0: 616d 7170 3a2f 2f67 7565 7374 3a67 7565  amqp://guest:gue
+000023d0: 7374 406c 6f63 616c 686f 7374 3a35 3637  st@localhost:567
+000023e0: 322f 2229 0a0a 6170 7020 3d20 5072 6f70  2/")..app = Prop
+000023f0: 616e 4170 7028 7261 6262 6974 5f62 726f  anApp(rabbit_bro
+00002400: 6b65 7229 0a0a 6173 796e 6320 6465 6620  ker)..async def 
+00002410: 6465 7065 6e64 656e 6379 2862 6f64 793a  dependency(body:
+00002420: 2064 6963 7429 202d 3e20 626f 6f6c 3a0a   dict) -> bool:.
+00002430: 2020 2020 7265 7475 726e 2054 7275 650a      return True.
+00002440: 0a40 7261 6262 6974 5f62 726f 6b65 722e  .@rabbit_broker.
+00002450: 6861 6e64 6c65 2822 7465 7374 2229 0a61  handle("test").a
+00002460: 7379 6e63 2064 6566 2062 6173 655f 6861  sync def base_ha
+00002470: 6e64 6c65 7228 626f 6479 3a20 6469 6374  ndler(body: dict
+00002480: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00002490: 2020 2020 2020 2020 2064 6570 3a20 626f           dep: bo
+000024a0: 6f6c 203d 2044 6570 656e 6473 2864 6570  ol = Depends(dep
+000024b0: 656e 6465 6e63 7929 2c0a 2020 2020 2020  endency),.      
+000024c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000024d0: 2062 726f 6b65 723a 2052 6162 6269 7442   broker: RabbitB
+000024e0: 726f 6b65 7220 3d20 436f 6e74 6578 7428  roker = Context(
+000024f0: 2929 3a0a 2020 2020 6173 7365 7274 2064  )):.    assert d
+00002500: 6570 2069 7320 5472 7565 0a20 2020 2061  ep is True.    a
+00002510: 7373 6572 7420 6272 6f6b 6572 2069 7320  ssert broker is 
+00002520: 7261 6262 6974 5f62 726f 6b65 720a 6060  rabbit_broker.``
+00002530: 600a 0a2d 2d2d 0a0a 2323 2043 4c49 2070  `..---..## CLI p
+00002540: 6f77 6572 0a0a 2a2a 5072 6f70 616e 2a2a  ower..**Propan**
+00002550: 2068 6173 2069 7473 206f 776e 2043 4c49   has its own CLI
+00002560: 2074 6f6f 6c20 7468 6174 2070 726f 7669   tool that provi
+00002570: 6465 6420 7468 6520 666f 6c6c 6f77 696e  ded the followin
+00002580: 6720 6665 6174 7572 6573 3a0a 0a2a 2070  g features:..* p
+00002590: 726f 6a65 6374 2067 656e 6572 6174 696f  roject generatio
+000025a0: 6e0a 2a20 6d75 6c74 6970 726f 6365 7373  n.* multiprocess
+000025b0: 696e 6720 776f 726b 6572 730a 2a20 7072  ing workers.* pr
+000025c0: 6f6a 6563 7420 686f 7420 7265 6c6f 6164  oject hot reload
+000025d0: 696e 670a 2a20 6375 7374 6f6d 2063 6f6d  ing.* custom com
+000025e0: 6d61 6e64 206c 696e 6520 6172 6775 6d65  mand line argume
+000025f0: 6e74 7320 7061 7373 696e 670a 0a23 2323  nts passing..###
+00002600: 2043 6f6e 7465 7874 2070 6173 7369 6e67   Context passing
+00002610: 0a0a 466f 7220 6578 616d 706c 653a 2070  ..For example: p
+00002620: 6173 7320 796f 7572 2063 7572 7265 6e74  ass your current
+00002630: 202a 2e65 6e76 2a20 7072 6f6a 6563 7420   *.env* project 
+00002640: 7365 7474 696e 6720 746f 2063 6f6e 7465  setting to conte
+00002650: 7874 0a0a 6060 6062 6173 680a 7072 6f70  xt..```bash.prop
+00002660: 616e 2072 756e 2073 6572 7665 3a61 7070  an run serve:app
+00002670: 202d 2d65 6e76 3d2e 656e 762e 6465 760a   --env=.env.dev.
+00002680: 6060 600a 0a60 6060 7079 7468 6f6e 0a66  ```..```python.f
+00002690: 726f 6d20 7072 6f70 616e 2069 6d70 6f72  rom propan impor
+000026a0: 7420 5072 6f70 616e 4170 702c 2052 6162  t PropanApp, Rab
+000026b0: 6269 7442 726f 6b65 720a 6672 6f6d 2070  bitBroker.from p
+000026c0: 726f 7061 6e2e 616e 6e6f 7461 7469 6f6e  ropan.annotation
+000026d0: 7320 696d 706f 7274 2043 6f6e 7465 7874  s import Context
+000026e0: 5265 706f 0a66 726f 6d20 7079 6461 6e74  Repo.from pydant
+000026f0: 6963 2069 6d70 6f72 7420 4261 7365 5365  ic import BaseSe
+00002700: 7474 696e 6773 0a0a 6272 6f6b 6572 203d  ttings..broker =
+00002710: 2052 6162 6269 7442 726f 6b65 7228 2261   RabbitBroker("a
+00002720: 6d71 703a 2f2f 6775 6573 743a 6775 6573  mqp://guest:gues
+00002730: 7440 6c6f 6361 6c68 6f73 743a 3536 3732  t@localhost:5672
+00002740: 2f22 290a 0a61 7070 203d 2050 726f 7061  /")..app = Propa
+00002750: 6e41 7070 2862 726f 6b65 7229 0a0a 636c  nApp(broker)..cl
+00002760: 6173 7320 5365 7474 696e 6773 2842 6173  ass Settings(Bas
+00002770: 6553 6574 7469 6e67 7329 3a0a 2020 2020  eSettings):.    
+00002780: 2e2e 2e0a 0a40 6170 702e 6f6e 5f73 7461  .....@app.on_sta
+00002790: 7274 7570 0a61 7379 6e63 2064 6566 2073  rtup.async def s
+000027a0: 6574 7570 2865 6e76 3a20 7374 722c 2063  etup(env: str, c
+000027b0: 6f6e 7465 7874 3a20 436f 6e74 6578 7452  ontext: ContextR
+000027c0: 6570 6f29 3a0a 2020 2020 7365 7474 696e  epo):.    settin
+000027d0: 6773 203d 2053 6574 7469 6e67 7328 5f65  gs = Settings(_e
+000027e0: 6e76 5f66 696c 653d 656e 7629 0a20 2020  nv_file=env).   
+000027f0: 2063 6f6e 7465 7874 2e73 6574 5f67 6c6f   context.set_glo
+00002800: 6261 6c28 2273 6574 7469 6e67 7322 2c20  bal("settings", 
+00002810: 7365 7474 696e 6773 290a 6060 600a 0a23  settings).```..#
+00002820: 2323 2050 726f 6a65 6374 2074 656d 706c  ## Project templ
+00002830: 6174 650a 0a41 6c73 6f2c 202a 2a50 726f  ate..Also, **Pro
+00002840: 7061 6e20 434c 492a 2a20 6973 2061 626c  pan CLI** is abl
+00002850: 6520 746f 2067 656e 6572 6174 6520 6120  e to generate a 
+00002860: 7072 6f64 7563 7469 6f6e 2d72 6561 6479  production-ready
+00002870: 2061 7070 6c69 6361 7469 6f6e 2074 656d   application tem
+00002880: 706c 6174 653a 0a0a 6060 6062 6173 680a  plate:..```bash.
+00002890: 7072 6f70 616e 2063 7265 6174 6520 6173  propan create as
+000028a0: 796e 6320 7261 6262 6974 205b 7072 6f6a  ync rabbit [proj
+000028b0: 6563 746e 616d 655d 0a60 6060 0a0a 2a4e  ectname].```..*N
+000028c0: 6f74 6963 653a 2070 726f 6a65 6374 2074  otice: project t
+000028d0: 656d 706c 6174 6520 7265 7175 6972 652a  emplate require*
+000028e0: 2060 7079 6461 6e74 6963 5b64 6f74 656e   `pydantic[doten
+000028f0: 765d 6020 2a69 6e73 7461 6c6c 6174 696f  v]` *installatio
+00002900: 6e2e 2a0a 0a52 756e 2074 6865 2063 7265  n.*..Run the cre
+00002910: 6174 6564 2070 726f 6a65 6374 3a0a 0a60  ated project:..`
+00002920: 6060 6261 7368 0a23 2052 756e 2072 6162  ``bash.# Run rab
+00002930: 6269 6d71 2066 6972 7374 0a64 6f63 6b65  bimq first.docke
+00002940: 7220 636f 6d70 6f73 6520 2d2d 6669 6c65  r compose --file
+00002950: 205b 7072 6f6a 6563 746e 616d 655d 2f64   [projectname]/d
+00002960: 6f63 6b65 722d 636f 6d70 6f73 652e 7961  ocker-compose.ya
+00002970: 6d6c 2075 7020 2d64 0a0a 2320 5275 6e20  ml up -d..# Run 
+00002980: 7072 6f6a 6563 740a 7072 6f70 616e 2072  project.propan r
+00002990: 756e 205b 7072 6f6a 6563 746e 616d 655d  un [projectname]
+000029a0: 2e61 7070 2e73 6572 7665 3a61 7070 202d  .app.serve:app -
+000029b0: 2d65 6e76 3d2e 656e 7620 2d2d 7265 6c6f  -env=.env --relo
+000029c0: 6164 0a60 6060 0a0a 4e6f 7720 796f 7520  ad.```..Now you 
+000029d0: 6361 6e20 656e 6a6f 7920 6120 6e65 7720  can enjoy a new 
+000029e0: 6465 7665 6c6f 706d 656e 7420 6578 7065  development expe
+000029f0: 7269 656e 6365 210a 0a2d 2d2d 0a0a 2323  rience!..---..##
+00002a00: 2048 5454 5020 4672 616d 6577 6f72 6b73   HTTP Frameworks
+00002a10: 2069 6e74 6567 7261 7469 6f6e 730a 0a23   integrations..#
+00002a20: 2323 2041 6e79 2046 7261 6d65 776f 726b  ## Any Framework
+00002a30: 0a0a 596f 7520 6361 6e20 7573 6520 2a2a  ..You can use **
+00002a40: 5072 6f70 616e 2a2a 2060 4d51 4272 6f6b  Propan** `MQBrok
+00002a50: 6572 7360 2077 6974 686f 7574 2060 5072  ers` without `Pr
+00002a60: 6f70 616e 4170 7060 2e0a 4a75 7374 202a  opanApp`..Just *
+00002a70: 7374 6172 742a 2061 6e64 202a 7374 6f70  start* and *stop
+00002a80: 2a20 7468 656d 2061 6363 6f72 6469 6e67  * them according
+00002a90: 2074 6f20 796f 7572 2061 7070 6c69 6361   to your applica
+00002aa0: 7469 6f6e 206c 6966 6573 7061 6e2e 0a0a  tion lifespan...
+00002ab0: 6060 6070 7974 686f 6e0a 6672 6f6d 2070  ```python.from p
+00002ac0: 726f 7061 6e20 696d 706f 7274 204e 6174  ropan import Nat
+00002ad0: 7342 726f 6b65 720a 6672 6f6d 2073 616e  sBroker.from san
+00002ae0: 6963 2069 6d70 6f72 7420 5361 6e69 630a  ic import Sanic.
+00002af0: 0a61 7070 203d 2053 616e 6963 2822 4d79  .app = Sanic("My
+00002b00: 4865 6c6c 6f57 6f72 6c64 4170 7022 290a  HelloWorldApp").
+00002b10: 6272 6f6b 6572 203d 204e 6174 7342 726f  broker = NatsBro
+00002b20: 6b65 7228 226e 6174 733a 2f2f 6c6f 6361  ker("nats://loca
+00002b30: 6c68 6f73 743a 3432 3232 2229 0a0a 4062  lhost:4222")..@b
+00002b40: 726f 6b65 722e 6861 6e64 6c65 2822 7465  roker.handle("te
+00002b50: 7374 2229 0a61 7379 6e63 2064 6566 2062  st").async def b
+00002b60: 6173 655f 6861 6e64 6c65 7228 626f 6479  ase_handler(body
+00002b70: 293a 0a20 2020 2070 7269 6e74 2862 6f64  ):.    print(bod
+00002b80: 7929 0a0a 4061 7070 2e61 6674 6572 5f73  y)..@app.after_s
+00002b90: 6572 7665 725f 7374 6172 740a 6173 796e  erver_start.asyn
+00002ba0: 6320 6465 6620 7374 6172 745f 6272 6f6b  c def start_brok
+00002bb0: 6572 2861 7070 2c20 6c6f 6f70 293a 0a20  er(app, loop):. 
+00002bc0: 2020 2061 7761 6974 2062 726f 6b65 722e     await broker.
+00002bd0: 7374 6172 7428 290a 0a40 6170 702e 6166  start()..@app.af
+00002be0: 7465 725f 7365 7276 6572 5f73 746f 700a  ter_server_stop.
+00002bf0: 6173 796e 6320 6465 6620 7374 6f70 5f62  async def stop_b
+00002c00: 726f 6b65 7228 6170 702c 206c 6f6f 7029  roker(app, loop)
+00002c10: 3a0a 2020 2020 6177 6169 7420 6272 6f6b  :.    await brok
+00002c20: 6572 2e63 6c6f 7365 2829 0a60 6060 0a0a  er.close().```..
+00002c30: 2323 2320 4661 7374 4150 4920 506c 7567  ### FastAPI Plug
+00002c40: 696e 0a0a 416c 736f 2c20 2a2a 5072 6f70  in..Also, **Prop
+00002c50: 616e 2a2a 2063 616e 2062 6520 7573 6564  an** can be used
+00002c60: 2061 7320 7061 7274 206f 6620 2a2a 4661   as part of **Fa
+00002c70: 7374 4150 492a 2a2e 0a0a 4a75 7374 2069  stAPI**...Just i
+00002c80: 6d70 6f72 7420 6120 2a2a 5072 6f70 616e  mport a **Propan
+00002c90: 526f 7574 6572 2a2a 2079 6f75 206e 6565  Router** you nee
+00002ca0: 6420 616e 6420 6465 636c 6172 6520 7468  d and declare th
+00002cb0: 6520 6d65 7373 6167 6520 6861 6e64 6c65  e message handle
+00002cc0: 720a 7573 696e 6720 7468 6520 6040 6576  r.using the `@ev
+00002cd0: 656e 7460 2064 6563 6f72 6174 6f72 2e20  ent` decorator. 
+00002ce0: 5468 6973 2064 6563 6f72 6174 6f72 2069  This decorator i
+00002cf0: 7320 7369 6d69 6c61 7220 746f 2074 6865  s similar to the
+00002d00: 2064 6563 6f72 6174 6f72 2060 4068 616e   decorator `@han
+00002d10: 646c 6560 2066 6f72 2074 6865 2063 6f72  dle` for the cor
+00002d20: 7265 7370 6f6e 6469 6e67 2062 726f 6b65  responding broke
+00002d30: 7273 2e0a 0a60 6060 7079 7468 6f6e 0a66  rs...```python.f
+00002d40: 726f 6d20 6661 7374 6170 6920 696d 706f  rom fastapi impo
+00002d50: 7274 2044 6570 656e 6473 2c20 4661 7374  rt Depends, Fast
+00002d60: 4150 490a 6672 6f6d 2070 7964 616e 7469  API.from pydanti
+00002d70: 6320 696d 706f 7274 2042 6173 654d 6f64  c import BaseMod
+00002d80: 656c 0a66 726f 6d20 7072 6f70 616e 2e66  el.from propan.f
+00002d90: 6173 7461 7069 2069 6d70 6f72 7420 5261  astapi import Ra
+00002da0: 6262 6974 526f 7574 6572 0a0a 6170 7020  bbitRouter..app 
+00002db0: 3d20 4661 7374 4150 4928 290a 0a72 6f75  = FastAPI()..rou
+00002dc0: 7465 7220 3d20 5261 6262 6974 526f 7574  ter = RabbitRout
+00002dd0: 6572 2822 616d 7170 3a2f 2f67 7565 7374  er("amqp://guest
+00002de0: 3a67 7565 7374 406c 6f63 616c 686f 7374  :guest@localhost
+00002df0: 3a35 3637 3222 290a 0a63 6c61 7373 2049  :5672")..class I
+00002e00: 6e63 6f6d 696e 6728 4261 7365 4d6f 6465  ncoming(BaseMode
+00002e10: 6c29 3a0a 2020 2020 6d3a 2064 6963 740a  l):.    m: dict.
+00002e20: 0a64 6566 2063 616c 6c28 293a 0a20 2020  .def call():.   
+00002e30: 2072 6574 7572 6e20 5472 7565 0a0a 4072   return True..@r
+00002e40: 6f75 7465 722e 6576 656e 7428 2274 6573  outer.event("tes
+00002e50: 7422 290a 6173 796e 6320 6465 6620 6865  t").async def he
+00002e60: 6c6c 6f28 6d3a 2049 6e63 6f6d 696e 672c  llo(m: Incoming,
+00002e70: 2064 203d 2044 6570 656e 6473 2863 616c   d = Depends(cal
+00002e80: 6c29 2920 2d3e 2064 6963 743a 0a20 2020  l)) -> dict:.   
+00002e90: 2072 6574 7572 6e20 7b20 2272 6573 706f   return { "respo
+00002ea0: 6e73 6522 3a20 2248 656c 6c6f 2c20 5072  nse": "Hello, Pr
+00002eb0: 6f70 616e 2122 207d 0a0a 6170 702e 696e  opan!" }..app.in
+00002ec0: 636c 7564 655f 726f 7574 6572 2872 6f75  clude_router(rou
+00002ed0: 7465 7229 0a60 6060 0a0a 2323 2045 7861  ter).```..## Exa
+00002ee0: 6d70 6c65 730a 0a54 6f20 7365 6520 6d6f  mples..To see mo
+00002ef0: 7265 2066 7261 6d65 776f 726b 2075 7361  re framework usa
+00002f00: 6765 7320 676f 2074 6f20 5b2a 2a65 7861  ges go to [**exa
+00002f10: 6d70 6c65 732f 2a2a 5d28 6874 7470 733a  mples/**](https:
+00002f20: 2f2f 6769 7468 7562 2e63 6f6d 2f4c 616e  //github.com/Lan
+00002f30: 6365 746e 696b 2f50 726f 7061 6e2f 7472  cetnik/Propan/tr
+00002f40: 6565 2f6d 6169 6e2f 6578 616d 706c 6573  ee/main/examples
+00002f50: 290a                                     ).
```

### Comparing `propan-0.1.0.0/pyproject.toml` & `propan-0.1.1.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -67,17 +67,22 @@
     "aio-pika>=9",
 ]
 
 async-nats = [
     "nats-py>=2"
 ]
 
+async-redis = [
+    "redis>=4.2.0rc1"
+]
+
 test = [
     "propan[async-rabbit]",
     "propan[async-nats]",
+    "propan[async-redis]",
 
     "coverage[toml]>=7.2",
     "pytest>=7",
     "pytest-asyncio>=0.21",
     "pytest-xdist[psutil]",
 
     "fastapi",
@@ -94,14 +99,16 @@
     "typer[all]",
 ]
 
 dev = [
     "propan[test]",
     "propan[doc]",
 
+    "types-redis",
+
     "mypy==1.1.1",
     "black==23.3.0",
     "isort>=5",
     "ruff==0.0.261",
     "typer[all]",
 ]
 
@@ -200,14 +207,15 @@
 testpaths = [
     "tests",
 ]
 markers = [
     "slow",
     "rabbit",
     "nats",
+    "redis",
     "all",
 ]
 
 [tool.coverage.run]
 parallel = true
 branch = true
 concurrency = [
```

### Comparing `propan-0.1.0.0/PKG-INFO` & `propan-0.1.1.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: propan
-Version: 0.1.0.0
+Version: 0.1.1.0
 Summary: Propan framework: the simplest way to work with a messaging queues
 Project-URL: Homepage, https://lancetnik.github.io/Propan/
 Project-URL: Documentation, https://lancetnik.github.io/Propan/
 Project-URL: Tracker, https://github.com/Lancetnik/Propan/issues
 Project-URL: Source, https://github.com/Lancetnik/Propan
 Author-email: Pastukhov Nikita <diementros@yandex.ru>
 License-Expression: MIT
@@ -40,34 +40,38 @@
 Requires-Dist: typer
 Requires-Dist: uvloop!=0.15.0,!=0.15.1,>=0.14.0; sys_platform != 'win32' and (sys_platform != 'cygwin' and platform_python_implementation != 'PyPy')
 Requires-Dist: watchfiles
 Provides-Extra: async-nats
 Requires-Dist: nats-py>=2; extra == 'async-nats'
 Provides-Extra: async-rabbit
 Requires-Dist: aio-pika>=9; extra == 'async-rabbit'
+Provides-Extra: async-redis
+Requires-Dist: redis>=4.2.0rc1; extra == 'async-redis'
 Provides-Extra: dev
 Requires-Dist: black==23.3.0; extra == 'dev'
 Requires-Dist: isort>=5; extra == 'dev'
 Requires-Dist: mypy==1.1.1; extra == 'dev'
 Requires-Dist: propan[doc]; extra == 'dev'
 Requires-Dist: propan[test]; extra == 'dev'
 Requires-Dist: ruff==0.0.261; extra == 'dev'
 Requires-Dist: typer[all]; extra == 'dev'
+Requires-Dist: types-redis; extra == 'dev'
 Provides-Extra: doc
 Requires-Dist: mdx-include<2.0.0,>=1.4.1; extra == 'doc'
 Requires-Dist: mkdocs-markdownextradata-plugin<0.3.0,>=0.1.7; extra == 'doc'
 Requires-Dist: mkdocs-material<9.0.0,>=8.1.4; extra == 'doc'
 Requires-Dist: mkdocs-static-i18n; extra == 'doc'
 Requires-Dist: typer[all]; extra == 'doc'
 Provides-Extra: test
 Requires-Dist: asyncmock; python_version < '3.8' and extra == 'test'
 Requires-Dist: coverage[toml]>=7.2; extra == 'test'
 Requires-Dist: fastapi; extra == 'test'
 Requires-Dist: propan[async-nats]; extra == 'test'
 Requires-Dist: propan[async-rabbit]; extra == 'test'
+Requires-Dist: propan[async-redis]; extra == 'test'
 Requires-Dist: pytest-asyncio>=0.21; extra == 'test'
 Requires-Dist: pytest-xdist[psutil]; extra == 'test'
 Requires-Dist: pytest>=7; extra == 'test'
 Description-Content-Type: text/markdown
 
 <p align="center">
     <a href="https://lancetnik.github.io/Propan/" target="_blank">
@@ -95,67 +99,70 @@
     <a href="https://github.com/Lancetnik/Propan/blob/main/LICENSE" target="_blank">
         <img alt="GitHub" src="https://img.shields.io/github/license/Lancetnik/Propan?color=%23007ec6">
     </a>
 </p>
 
 # Propan
 
-**Propan** - just *~~an another one HTTP~~* a **declarative Python MQ framework**. It's following by [*fastapi*](https://fastapi.tiangolo.com/ru/),
-simplify Message Brokers around code writing and provides a helpful development toolkit, which existed only in HTTP-frameworks world until now.
+**Propan** - just *~~an another one HTTP~~* a **declarative Python MQ framework**. It's following by <a href="https://fastapi.tiangolo.com/ru/" target="_blank">*fastapi*</a>, simplify Message Brokers around code writing and provides a helpful development toolkit, which existed only in HTTP-frameworks world until now.
 
 It's designed to create reactive microservices around <a href="https://microservices.io/patterns/communication-style/messaging.html" target="_blank">Messaging Architecture</a>.
 
-It is a modern, high-level framework on top of popular specific Python brokers libraries, based on [*pydantic*](https://docs.pydantic.dev/) and [*fastapi*](https://fastapi.tiangolo.com/ru/), [*pytest*](https://docs.pytest.org/en/7.3.x/) concepts.
+It is a modern, high-level framework on top of popular specific Python brokers libraries, based on <a href="https://docs.pydantic.dev/" target="_blank">*pydantic*</a> and <a href="https://fastapi.tiangolo.com/ru/" target="_blank">*fastapi*</a>, <a href="https://docs.pytest.org/en/7.3.x/" target="_blank">*pytest*</a> concepts.
 
 ---
 
 **Documentation**: <a href="https://lancetnik.github.io/Propan/" target="_blank">https://lancetnik.github.io/Propan/</a>
 
 ---
 
 ### The key features are
 
-* **Easy**: Designed to be easy to use and learn.
+* **Simple**: Designed to be easy to use and learn.
 * **Intuitive**: Great editor support. Autocompletion everywhere.
-* [**Dependencies management**](#dependencies): Minimize code duplication. Multiple features from each argument and parameter declaration.
-* [**Integrations**](#http-frameworks-integrations): **Propan** is ready to use in pair with [any HTTP framework](https://lancetnik.github.io/Propan/5_integrations/1_integrations-index/) you want
+* [**Dependencies management**](#dependencies): Minimization of code duplication. Access to dependencies at any level of the call stack.
+* [**Integrations**](#http-frameworks-integrations): **Propan** is fully compatible with <a href="https://lancetnik.github.io/Propan/integrations/1_integrations-index/" target="_blank">any HTTP framework</a> you want
 * **MQ independent**: Single interface to popular MQ:
-  * **NATS** (based on [nats-py](https://github.com/nats-io/nats.py)) 
-  * **RabbitMQ** (based on [aio-pika](https://aio-pika.readthedocs.io/en/latest/))
-* [**RPC**](https://lancetnik.github.io/Propan/2_getting_started/4_broker/5_rpc/): The framework supports RPC requests over MQ, which will allow performing long operations on remote services asynchronously.
+  * **Redis** (based on <a href="https://redis.readthedocs.io/en/stable/index.html" target="_blank">redis-py</a>)
+  * **RabbitMQ** (based on <a href="https://aio-pika.readthedocs.io/en/latest/" target="_blank">aio-pika</a>)
+  * **NATS** (based on <a href="https://github.com/nats-io/nats.py" target="_blank">nats-py</a>)
+* <a href="https://lancetnik.github.io/Propan/getting_started/4_broker/5_rpc/" target="_blank">**RPC**</a>: The framework supports RPC requests over MQ, which will allow performing long operations on remote services asynchronously.
 * [**Greate to develop**](#cli-power): CLI tool provides great development experience:
-  * framework-independent way to rule application environment
-  * application code hot reloading
-* [**Testability**](https://lancetnik.github.io/Propan/2_getting_started/7_testing): **Propan** allows you to test your app without external dependencies: you shouldn't suit up a Message Broker, use a virtual one!
+  * framework-independent way to manage the project environment
+  * application code *hot reload*
+  * robust application templates
+* <a href="https://lancetnik.github.io/Propan/getting_started/7_testing" target="_blank">**Testability**</a>: **Propan** allows you to test your app without external dependencies: you do not have to set up a Message Broker, you can use a virtual one!
 
 ### Supported MQ brokers
-|              | async                                                   | sync                 |
-|--------------|:-------------------------------------------------------:|:--------------------:|
-| **RabbitMQ** | :heavy_check_mark: **stable** :heavy_check_mark:        | :mag: planning :mag: |
-| **Nats**     | :warning: **beta** :warning:                            | :mag: planning :mag: |
-| **NatsJS**   | :hammer_and_wrench: **in progress** :hammer_and_wrench: | :mag: planning :mag: |
-| **MQTT**     | :mag: planning :mag:                                    | :mag: planning :mag: |
-| **REDIS**    | :mag: planning :mag:                                    | :mag: planning :mag: |
-| **Kafka**    | :mag: planning :mag:                                    | :mag: planning :mag: |
-| **SQS**      | :mag: planning :mag:                                    | :mag: planning :mag: |
 
+|                   | async                                                   | sync                 |
+|-------------------|:-------------------------------------------------------:|:--------------------:|
+| **RabbitMQ**      | :heavy_check_mark: **stable** :heavy_check_mark:        | :mag: planning :mag: |
+| **Redis**         | :heavy_check_mark: **stable** :heavy_check_mark:        | :mag: planning :mag: |
+| **Nats**          | :warning: **beta** :warning:                            | :mag: planning :mag: |
+| **NatsJS**        | :hammer_and_wrench: **in progress** :hammer_and_wrench: | :mag: planning :mag: |
+| **MQTT**          | :mag: planning :mag:                                    | :mag: planning :mag: |
+| **Kafka**         | :mag: planning :mag:                                    | :mag: planning :mag: |
+| **Redis Streams** | :mag: planning :mag:                                    | :mag: planning :mag: |
+| **Pulsar**        | :mag: planning :mag:                                    | :mag: planning :mag: |
+| **SQS**           | :mag: planning :mag:                                    | :mag: planning :mag: |
 
 ### Community
 
 If you are interested in this project, please give me feedback by star or/and watch repository.
 
 If you have any questions or ideas about features to implement, welcome to [discussions](https://github.com/Lancetnik/Propan/discussions) or public [telegram group](https://t.me/propan_python).
 
 ---
 
 ## Declarative?
 
-With declarative tools you should define **what you need to get**. With traditional imperative tools you should write **what you need to do**.
+With declarative tools you can define **what you need to get**. With traditional imperative tools you must write **what you need to do**.
 
-Take a look at classic imperative tools, such as [aio-pika](https://aio-pika.readthedocs.io/en/latest/), [pika](https://pika.readthedocs.io/en/stable/), [nats-py](https://github.com/nats-io/nats.py), etc.
+Take a look at classic imperative tools, such as <a href="https://aio-pika.readthedocs.io/en/latest/" target="_blank">aio-pika</a>, <a href="https://pika.readthedocs.io/en/stable/" target="_blank">pika</a>, <a href="https://redis.readthedocs.io/en/stable/index.html" target="_blank">redis-py</a>, <a href="https://github.com/nats-io/nats.py" target="_blank">nats-py</a>, etc.
 
 This is the **Quickstart** with the *aio-pika*:
 
 ```python
 import asyncio
 import aio_pika
 
@@ -175,17 +182,17 @@
             async for message in queue_iter:
                 async with message.process():
                     print(message.body)
 
 asyncio.run(main())
 ```
 
-**aio-pika** is a really great tool with a really easy learning curve. But it's still imperative. You need to *connect*, declare *channel*, *queues*, *exchanges* by yourself. Also, you need to manage *connection*, *message*, *queue* context to avoid any troubles.
+**aio-pika** is a great tool with a really easy learning curve. But it's still imperative. You need to *connect*, declare *channel*, *queues*, *exchanges* by yourself. Also, you need to manage *connection*, *message*, *queue* context to avoid any troubles.
 
-It is not a bad way, but it can be easy.
+It is not a bad way, but it can be much easier.
 
 ```python
 from propan import PropanApp, RabbitBroker
 
 broker = RabbitBroker("amqp://guest:guest@localhost:5672/")
 
 app = PropanApp(broker)
@@ -212,18 +219,20 @@
 ### Basic usage
 
 Create an application with the following code at `serve.py`:
 
 ```python
 from propan import PropanApp
 from propan import RabbitBroker
+# from propan import RedisBroker
 # from propan import NatsBroker
 
 broker = RabbitBroker("amqp://guest:guest@localhost:5672/")
 # broker = NatsBroker("nats://localhost:4222")
+# broker = RedisBroker("redis://localhost:6379")
 
 app = PropanApp(broker)
 
 @broker.handle("test")
 async def base_handler(body):
     '''Handle all default exchange messages with `test` routing key'''
     print(body)
@@ -328,15 +337,15 @@
 ```
 
 ### Project template
 
 Also, **Propan CLI** is able to generate a production-ready application template:
 
 ```bash
-propan create [projectname]
+propan create async rabbit [projectname]
 ```
 
 *Notice: project template require* `pydantic[dotenv]` *installation.*
 
 Run the created project:
 
 ```bash
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: propan Version: 0.1.0.0 Summary: Propan framework:
+Metadata-Version: 2.1 Name: propan Version: 0.1.1.0 Summary: Propan framework:
 the simplest way to work with a messaging queues Project-URL: Homepage, https:/
 /lancetnik.github.io/Propan/ Project-URL: Documentation, https://
 lancetnik.github.io/Propan/ Project-URL: Tracker, https://github.com/Lancetnik/
 Propan/issues Project-URL: Source, https://github.com/Lancetnik/Propan Author-
 email: Pastukhov Nikita
 yandex.ru> License-Expression: MIT License-File: LICENSE Keywords:
 framework,message brokers,rabbitmq Classifier: Development Status :: 5 -
@@ -23,143 +23,142 @@
 :: Application Frameworks Classifier: Topic :: Software Development ::
 Libraries :: Python Modules Classifier: Typing :: Typed Requires-Python: >=3.7
 Requires-Dist: fast-depends>=1.1.3 Requires-Dist: typer Requires-Dist:
 uvloop!=0.15.0,!=0.15.1,>=0.14.0; sys_platform != 'win32' and (sys_platform !=
 'cygwin' and platform_python_implementation != 'PyPy') Requires-Dist:
 watchfiles Provides-Extra: async-nats Requires-Dist: nats-py>=2; extra ==
 'async-nats' Provides-Extra: async-rabbit Requires-Dist: aio-pika>=9; extra ==
-'async-rabbit' Provides-Extra: dev Requires-Dist: black==23.3.0; extra == 'dev'
-Requires-Dist: isort>=5; extra == 'dev' Requires-Dist: mypy==1.1.1; extra ==
-'dev' Requires-Dist: propan[doc]; extra == 'dev' Requires-Dist: propan[test];
-extra == 'dev' Requires-Dist: ruff==0.0.261; extra == 'dev' Requires-Dist:
-typer[all]; extra == 'dev' Provides-Extra: doc Requires-Dist: mdx-
-include<2.0.0,>=1.4.1; extra == 'doc' Requires-Dist: mkdocs-markdownextradata-
-plugin<0.3.0,>=0.1.7; extra == 'doc' Requires-Dist: mkdocs-
-material<9.0.0,>=8.1.4; extra == 'doc' Requires-Dist: mkdocs-static-i18n; extra
-== 'doc' Requires-Dist: typer[all]; extra == 'doc' Provides-Extra: test
-Requires-Dist: asyncmock; python_version < '3.8' and extra == 'test' Requires-
-Dist: coverage[toml]>=7.2; extra == 'test' Requires-Dist: fastapi; extra ==
-'test' Requires-Dist: propan[async-nats]; extra == 'test' Requires-Dist: propan
-[async-rabbit]; extra == 'test' Requires-Dist: pytest-asyncio>=0.21; extra ==
+'async-rabbit' Provides-Extra: async-redis Requires-Dist: redis>=4.2.0rc1;
+extra == 'async-redis' Provides-Extra: dev Requires-Dist: black==23.3.0; extra
+== 'dev' Requires-Dist: isort>=5; extra == 'dev' Requires-Dist: mypy==1.1.1;
+extra == 'dev' Requires-Dist: propan[doc]; extra == 'dev' Requires-Dist: propan
+[test]; extra == 'dev' Requires-Dist: ruff==0.0.261; extra == 'dev' Requires-
+Dist: typer[all]; extra == 'dev' Requires-Dist: types-redis; extra == 'dev'
+Provides-Extra: doc Requires-Dist: mdx-include<2.0.0,>=1.4.1; extra == 'doc'
+Requires-Dist: mkdocs-markdownextradata-plugin<0.3.0,>=0.1.7; extra == 'doc'
+Requires-Dist: mkdocs-material<9.0.0,>=8.1.4; extra == 'doc' Requires-Dist:
+mkdocs-static-i18n; extra == 'doc' Requires-Dist: typer[all]; extra == 'doc'
+Provides-Extra: test Requires-Dist: asyncmock; python_version < '3.8' and extra
+== 'test' Requires-Dist: coverage[toml]>=7.2; extra == 'test' Requires-Dist:
+fastapi; extra == 'test' Requires-Dist: propan[async-nats]; extra == 'test'
+Requires-Dist: propan[async-rabbit]; extra == 'test' Requires-Dist: propan
+[async-redis]; extra == 'test' Requires-Dist: pytest-asyncio>=0.21; extra ==
 'test' Requires-Dist: pytest-xdist[psutil]; extra == 'test' Requires-Dist:
 pytest>=7; extra == 'test' Description-Content-Type: text/markdown
                                  [Propan_logo]
           [Tests_coverage] [Coverage] [Package_version] [downloads]
                      [Supported_Python_versions] [GitHub]
 # Propan **Propan** - just *~~an another one HTTP~~* a **declarative Python MQ
-framework**. It's following by [*fastapi*](https://fastapi.tiangolo.com/ru/),
-simplify Message Brokers around code writing and provides a helpful development
-toolkit, which existed only in HTTP-frameworks world until now. It's designed
-to create reactive microservices around Messaging_Architecture. It is a modern,
-high-level framework on top of popular specific Python brokers libraries, based
-on [*pydantic*](https://docs.pydantic.dev/) and [*fastapi*](https://
-fastapi.tiangolo.com/ru/), [*pytest*](https://docs.pytest.org/en/7.3.x/
-) concepts. --- **Documentation**: https://lancetnik.github.io/Propan/ --- ###
-The key features are * **Easy**: Designed to be easy to use and learn. *
-**Intuitive**: Great editor support. Autocompletion everywhere. *
-[**Dependencies management**](#dependencies): Minimize code duplication.
-Multiple features from each argument and parameter declaration. *
-[**Integrations**](#http-frameworks-integrations): **Propan** is ready to use
-in pair with [any HTTP framework](https://lancetnik.github.io/Propan/
-5_integrations/1_integrations-index/) you want * **MQ independent**: Single
-interface to popular MQ: * **NATS** (based on [nats-py](https://github.com/
-nats-io/nats.py)) * **RabbitMQ** (based on [aio-pika](https://aio-
-pika.readthedocs.io/en/latest/)) * [**RPC**](https://lancetnik.github.io/
-Propan/2_getting_started/4_broker/5_rpc/): The framework supports RPC requests
-over MQ, which will allow performing long operations on remote services
-asynchronously. * [**Greate to develop**](#cli-power): CLI tool provides great
-development experience: * framework-independent way to rule application
-environment * application code hot reloading * [**Testability**](https://
-lancetnik.github.io/Propan/2_getting_started/7_testing): **Propan** allows you
-to test your app without external dependencies: you shouldn't suit up a Message
-Broker, use a virtual one! ### Supported MQ brokers | | async | sync | |-------
--------|:-------------------------------------------------------:|:------------
---------:| | **RabbitMQ** | :heavy_check_mark: **stable** :heavy_check_mark: |
-:mag: planning :mag: | | **Nats** | :warning: **beta** :warning: | :mag:
-planning :mag: | | **NatsJS** | :hammer_and_wrench: **in progress** :
-hammer_and_wrench: | :mag: planning :mag: | | **MQTT** | :mag: planning :mag: |
-:mag: planning :mag: | | **REDIS** | :mag: planning :mag: | :mag: planning :
-mag: | | **Kafka** | :mag: planning :mag: | :mag: planning :mag: | | **SQS** |
-:mag: planning :mag: | :mag: planning :mag: | ### Community If you are
-interested in this project, please give me feedback by star or/and watch
-repository. If you have any questions or ideas about features to implement,
-welcome to [discussions](https://github.com/Lancetnik/Propan/discussions) or
-public [telegram group](https://t.me/propan_python). --- ## Declarative? With
-declarative tools you should define **what you need to get**. With traditional
-imperative tools you should write **what you need to do**. Take a look at
-classic imperative tools, such as [aio-pika](https://aio-pika.readthedocs.io/
-en/latest/), [pika](https://pika.readthedocs.io/en/stable/), [nats-py](https://
-github.com/nats-io/nats.py), etc. This is the **Quickstart** with the *aio-
+framework**. It's following by *fastapi*, simplify Message Brokers around code
+writing and provides a helpful development toolkit, which existed only in HTTP-
+frameworks world until now. It's designed to create reactive microservices
+around Messaging_Architecture. It is a modern, high-level framework on top of
+popular specific Python brokers libraries, based on *pydantic* and *fastapi*,
+*pytest* concepts. --- **Documentation**: https://lancetnik.github.io/Propan/ -
+-- ### The key features are * **Simple**: Designed to be easy to use and learn.
+* **Intuitive**: Great editor support. Autocompletion everywhere. *
+[**Dependencies management**](#dependencies): Minimization of code duplication.
+Access to dependencies at any level of the call stack. * [**Integrations**]
+(#http-frameworks-integrations): **Propan** is fully compatible with any_HTTP
+framework you want * **MQ independent**: Single interface to popular MQ: *
+**Redis** (based on redis-py) * **RabbitMQ** (based on aio-pika) * **NATS**
+(based on nats-py) * **RPC**: The framework supports RPC requests over MQ,
+which will allow performing long operations on remote services asynchronously.
+* [**Greate to develop**](#cli-power): CLI tool provides great development
+experience: * framework-independent way to manage the project environment *
+application code *hot reload* * robust application templates * **Testability**:
+**Propan** allows you to test your app without external dependencies: you do
+not have to set up a Message Broker, you can use a virtual one! ### Supported
+MQ brokers | | async | sync | |-------------------|:---------------------------
+----------------------------:|:--------------------:| | **RabbitMQ** | :
+heavy_check_mark: **stable** :heavy_check_mark: | :mag: planning :mag: | |
+**Redis** | :heavy_check_mark: **stable** :heavy_check_mark: | :mag: planning :
+mag: | | **Nats** | :warning: **beta** :warning: | :mag: planning :mag: | |
+**NatsJS** | :hammer_and_wrench: **in progress** :hammer_and_wrench: | :mag:
+planning :mag: | | **MQTT** | :mag: planning :mag: | :mag: planning :mag: | |
+**Kafka** | :mag: planning :mag: | :mag: planning :mag: | | **Redis Streams** |
+:mag: planning :mag: | :mag: planning :mag: | | **Pulsar** | :mag: planning :
+mag: | :mag: planning :mag: | | **SQS** | :mag: planning :mag: | :mag: planning
+:mag: | ### Community If you are interested in this project, please give me
+feedback by star or/and watch repository. If you have any questions or ideas
+about features to implement, welcome to [discussions](https://github.com/
+Lancetnik/Propan/discussions) or public [telegram group](https://t.me/
+propan_python). --- ## Declarative? With declarative tools you can define
+**what you need to get**. With traditional imperative tools you must write
+**what you need to do**. Take a look at classic imperative tools, such as aio-
+pika, pika, redis-py, nats-py, etc. This is the **Quickstart** with the *aio-
 pika*: ```python import asyncio import aio_pika async def main(): connection =
 await aio_pika.connect_robust( "amqp://guest:guest@127.0.0.1/" ) queue_name =
 "test_queue" async with connection: channel = await connection.channel() queue
 = await channel.declare_queue(queue_name) async with queue.iterator() as
 queue_iter: async for message in queue_iter: async with message.process():
-print(message.body) asyncio.run(main()) ``` **aio-pika** is a really great tool
-with a really easy learning curve. But it's still imperative. You need to
-*connect*, declare *channel*, *queues*, *exchanges* by yourself. Also, you need
-to manage *connection*, *message*, *queue* context to avoid any troubles. It is
-not a bad way, but it can be easy. ```python from propan import PropanApp,
+print(message.body) asyncio.run(main()) ``` **aio-pika** is a great tool with a
+really easy learning curve. But it's still imperative. You need to *connect*,
+declare *channel*, *queues*, *exchanges* by yourself. Also, you need to manage
+*connection*, *message*, *queue* context to avoid any troubles. It is not a bad
+way, but it can be much easier. ```python from propan import PropanApp,
 RabbitBroker broker = RabbitBroker("amqp://guest:guest@localhost:5672/") app =
 PropanApp(broker) @broker.handle("test_queue") async def base_handler(body):
 print(body) ``` This is the **Propan** declarative way to write the same code.
 That is so much easier, isn't it? --- ## Quickstart Install using `pip`:
 ```shell $ pip install "propan[async-rabbit]" # or $ pip install "propan[async-
 nats]" ``` ### Basic usage Create an application with the following code at
 `serve.py`: ```python from propan import PropanApp from propan import
-RabbitBroker # from propan import NatsBroker broker = RabbitBroker("amqp://
-guest:guest@localhost:5672/") # broker = NatsBroker("nats://localhost:4222")
-app = PropanApp(broker) @broker.handle("test") async def base_handler(body):
-'''Handle all default exchange messages with `test` routing key''' print(body)
-``` And just run it: ```shell $ propan run serve:app ``` --- ## Type casting
-Propan uses `pydantic` to cast incoming function arguments to types according
-to their annotation. ```python from pydantic import BaseModel from propan
-import PropanApp, Context, RabbitBroker broker = RabbitBroker("amqp://guest:
-guest@localhost:5672/") app = PropanApp(broker) class SimpleMessage(BaseModel):
-key: int @broker.handle("test2") async def second_handler(body: SimpleMessage):
-assert isinstance(body.key, int) ``` --- ## Dependencies **Propan** a has
-dependencies management policy close to `pytest fixtures`. You can specify in
-functions arguments which dependencies you would to use. Framework passes them
-from the global Context object. Already existed context fields are: *app*,
-*broker*, *context* (itself), *logger* and *message*. If you call not existing
-field, raises *pydantic.ValidationError* value. But you can specify your own
-dependencies, call dependencies functions (like `Fastapi Depends`) and [more]
-(https://github.com/Lancetnik/Propan/tree/main/examples/dependencies).
-```python import aio_pika from propan import PropanApp, RabbitBroker, Context,
-Depends rabbit_broker = RabbitBroker("amqp://guest:guest@localhost:5672/") app
-= PropanApp(rabbit_broker) async def dependency(body: dict) -> bool: return
-True @rabbit_broker.handle("test") async def base_handler(body: dict, dep: bool
-= Depends(dependency), broker: RabbitBroker = Context()): assert dep is True
-assert broker is rabbit_broker ``` --- ## CLI power **Propan** has its own CLI
-tool that provided the following features: * project generation *
-multiprocessing workers * project hot reloading * custom command line arguments
-passing ### Context passing For example: pass your current *.env* project
-setting to context ```bash propan run serve:app --env=.env.dev ``` ```python
-from propan import PropanApp, RabbitBroker from propan.annotations import
-ContextRepo from pydantic import BaseSettings broker = RabbitBroker("amqp://
-guest:guest@localhost:5672/") app = PropanApp(broker) class Settings
-(BaseSettings): ... @app.on_startup async def setup(env: str, context:
-ContextRepo): settings = Settings(_env_file=env) context.set_global("settings",
-settings) ``` ### Project template Also, **Propan CLI** is able to generate a
-production-ready application template: ```bash propan create [projectname] ```
-*Notice: project template require* `pydantic[dotenv]` *installation.* Run the
-created project: ```bash # Run rabbimq first docker compose --file
-[projectname]/docker-compose.yaml up -d # Run project propan run
-[projectname].app.serve:app --env=.env --reload ``` Now you can enjoy a new
-development experience! --- ## HTTP Frameworks integrations ### Any Framework
-You can use **Propan** `MQBrokers` without `PropanApp`. Just *start* and *stop*
-them according to your application lifespan. ```python from propan import
-NatsBroker from sanic import Sanic app = Sanic("MyHelloWorldApp") broker =
-NatsBroker("nats://localhost:4222") @broker.handle("test") async def
-base_handler(body): print(body) @app.after_server_start async def start_broker
-(app, loop): await broker.start() @app.after_server_stop async def stop_broker
-(app, loop): await broker.close() ``` ### FastAPI Plugin Also, **Propan** can
-be used as part of **FastAPI**. Just import a **PropanRouter** you need and
-declare the message handler using the `@event` decorator. This decorator is
-similar to the decorator `@handle` for the corresponding brokers. ```python
-from fastapi import Depends, FastAPI from pydantic import BaseModel from
-propan.fastapi import RabbitRouter app = FastAPI() router = RabbitRouter("amqp:
-//guest:guest@localhost:5672") class Incoming(BaseModel): m: dict def call():
-return True @router.event("test") async def hello(m: Incoming, d = Depends
-(call)) -> dict: return { "response": "Hello, Propan!" } app.include_router
-(router) ``` ## Examples To see more framework usages go to [**examples/**]
-(https://github.com/Lancetnik/Propan/tree/main/examples)
+RabbitBroker # from propan import RedisBroker # from propan import NatsBroker
+broker = RabbitBroker("amqp://guest:guest@localhost:5672/") # broker =
+NatsBroker("nats://localhost:4222") # broker = RedisBroker("redis://localhost:
+6379") app = PropanApp(broker) @broker.handle("test") async def base_handler
+(body): '''Handle all default exchange messages with `test` routing key'''
+print(body) ``` And just run it: ```shell $ propan run serve:app ``` --- ##
+Type casting Propan uses `pydantic` to cast incoming function arguments to
+types according to their annotation. ```python from pydantic import BaseModel
+from propan import PropanApp, Context, RabbitBroker broker = RabbitBroker
+("amqp://guest:guest@localhost:5672/") app = PropanApp(broker) class
+SimpleMessage(BaseModel): key: int @broker.handle("test2") async def
+second_handler(body: SimpleMessage): assert isinstance(body.key, int) ``` --
+- ## Dependencies **Propan** a has dependencies management policy close to
+`pytest fixtures`. You can specify in functions arguments which dependencies
+you would to use. Framework passes them from the global Context object. Already
+existed context fields are: *app*, *broker*, *context* (itself), *logger* and
+*message*. If you call not existing field, raises *pydantic.ValidationError*
+value. But you can specify your own dependencies, call dependencies functions
+(like `Fastapi Depends`) and [more](https://github.com/Lancetnik/Propan/tree/
+main/examples/dependencies). ```python import aio_pika from propan import
+PropanApp, RabbitBroker, Context, Depends rabbit_broker = RabbitBroker("amqp://
+guest:guest@localhost:5672/") app = PropanApp(rabbit_broker) async def
+dependency(body: dict) -> bool: return True @rabbit_broker.handle("test") async
+def base_handler(body: dict, dep: bool = Depends(dependency), broker:
+RabbitBroker = Context()): assert dep is True assert broker is rabbit_broker
+``` --- ## CLI power **Propan** has its own CLI tool that provided the
+following features: * project generation * multiprocessing workers * project
+hot reloading * custom command line arguments passing ### Context passing For
+example: pass your current *.env* project setting to context ```bash propan run
+serve:app --env=.env.dev ``` ```python from propan import PropanApp,
+RabbitBroker from propan.annotations import ContextRepo from pydantic import
+BaseSettings broker = RabbitBroker("amqp://guest:guest@localhost:5672/") app =
+PropanApp(broker) class Settings(BaseSettings): ... @app.on_startup async def
+setup(env: str, context: ContextRepo): settings = Settings(_env_file=env)
+context.set_global("settings", settings) ``` ### Project template Also,
+**Propan CLI** is able to generate a production-ready application template:
+```bash propan create async rabbit [projectname] ``` *Notice: project template
+require* `pydantic[dotenv]` *installation.* Run the created project: ```bash #
+Run rabbimq first docker compose --file [projectname]/docker-compose.yaml up -
+d # Run project propan run [projectname].app.serve:app --env=.env --reload ```
+Now you can enjoy a new development experience! --- ## HTTP Frameworks
+integrations ### Any Framework You can use **Propan** `MQBrokers` without
+`PropanApp`. Just *start* and *stop* them according to your application
+lifespan. ```python from propan import NatsBroker from sanic import Sanic app =
+Sanic("MyHelloWorldApp") broker = NatsBroker("nats://localhost:4222")
+@broker.handle("test") async def base_handler(body): print(body)
+@app.after_server_start async def start_broker(app, loop): await broker.start()
+@app.after_server_stop async def stop_broker(app, loop): await broker.close()
+``` ### FastAPI Plugin Also, **Propan** can be used as part of **FastAPI**.
+Just import a **PropanRouter** you need and declare the message handler using
+the `@event` decorator. This decorator is similar to the decorator `@handle`
+for the corresponding brokers. ```python from fastapi import Depends, FastAPI
+from pydantic import BaseModel from propan.fastapi import RabbitRouter app =
+FastAPI() router = RabbitRouter("amqp://guest:guest@localhost:5672") class
+Incoming(BaseModel): m: dict def call(): return True @router.event("test")
+async def hello(m: Incoming, d = Depends(call)) -> dict: return { "response":
+"Hello, Propan!" } app.include_router(router) ``` ## Examples To see more
+framework usages go to [**examples/**](https://github.com/Lancetnik/Propan/
+tree/main/examples)
```

