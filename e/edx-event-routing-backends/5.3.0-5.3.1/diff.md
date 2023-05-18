# Comparing `tmp/edx-event-routing-backends-5.3.0.tar.gz` & `tmp/edx-event-routing-backends-5.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edx-event-routing-backends-5.3.0.tar", last modified: Fri May 12 07:34:04 2023, max compression
+gzip compressed data, was "edx-event-routing-backends-5.3.1.tar", last modified: Thu May 18 05:29:42 2023, max compression
```

## Comparing `edx-event-routing-backends-5.3.0.tar` & `edx-event-routing-backends-5.3.1.tar`

### file list

```diff
@@ -1,112 +1,112 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-12 07:34:04.445394 edx-event-routing-backends-5.3.0/
--rw-r--r--   0 runner    (1001) docker     (122)     2649 2023-05-12 07:33:59.000000 edx-event-routing-backends-5.3.0/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (122)    35139 2023-05-12 07:33:59.000000 edx-event-routing-backends-5.3.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (122)      222 2023-05-12 07:33:59.000000 edx-event-routing-backends-5.3.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     7155 2023-05-12 07:34:04.445394 edx-event-routing-backends-5.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     3721 2023-05-12 07:33:59.000000 edx-event-routing-backends-5.3.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-12 07:34:04.429394 edx-event-routing-backends-5.3.0/edx_event_routing_backends.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     7155 2023-05-12 07:34:04.000000 edx-event-routing-backends-5.3.0/edx_event_routing_backends.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     4467 2023-05-12 07:34:04.000000 edx-event-routing-backends-5.3.0/edx_event_routing_backends.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-12 07:34:04.000000 edx-event-routing-backends-5.3.0/edx_event_routing_backends.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      193 2023-05-12 07:34:04.000000 edx-event-routing-backends-5.3.0/edx_event_routing_backends.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-12 07:34:04.000000 edx-event-routing-backends-5.3.0/edx_event_routing_backends.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)      135 2023-05-12 07:34:04.000000 edx-event-routing-backends-5.3.0/edx_event_routing_backends.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       23 2023-05-12 07:34:04.000000 edx-event-routing-backends-5.3.0/edx_event_routing_backends.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-12 07:34:04.429394 edx-event-routing-backends-5.3.0/event_routing_backends/
--rw-r--r--   0 runner    (1001) docker     (122)      190 2023-05-12 07:33:59.000000 edx-event-routing-backends-5.3.0/event_routing_backends/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      685 2023-05-12 07:33:59.000000 edx-event-routing-backends-5.3.0/event_routing_backends/admin.py
--rw-r--r--   0 runner    (1001) docker     (122)     1427 2023-05-12 07:33:59.000000 edx-event-routing-backends-5.3.0/event_routing_backends/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-12 07:34:04.429394 edx-event-routing-backends-5.3.0/event_routing_backends/backends/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-12 07:33:59.000000 edx-event-routing-backends-5.3.0/event_routing_backends/backends/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5833 2023-05-12 07:33:59.000000 edx-event-routing-backends-5.3.0/event_routing_backends/backends/events_router.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-12 07:34:04.433394 edx-event-routing-backends-5.3.0/event_routing_backends/backends/tests/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-12 07:33:59.000000 edx-event-routing-backends-5.3.0/event_routing_backends/backends/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    13413 2023-05-12 07:33:59.000000 edx-event-routing-backends-5.3.0/event_routing_backends/backends/tests/test_events_router.py
--rw-r--r--   0 runner    (1001) docker     (122)     7942 2023-05-12 07:33:59.000000 edx-event-routing-backends-5.3.0/event_routing_backends/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-12 07:34:04.433394 edx-event-routing-backends-5.3.0/event_routing_backends/migrations/
--rw-r--r--   0 runner    (1001) docker     (122)     1591 2023-05-12 07:33:59.000000 edx-event-routing-backends-5.3.0/event_routing_backends/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (122)      981 2023-05-12 07:33:59.000000 edx-event-routing-backends-5.3.0/event_routing_backends/migrations/0002_auto_20210503_0648.py
--rw-r--r--   0 runner    (1001) docker     (122)      484 2023-05-12 07:33:59.000000 edx-event-routing-backends-5.3.0/event_routing_backends/migrations/0003_auto_20210713_0344.py
--rw-r--r--   0 runner    (1001) docker     (122)     1938 2023-05-12 07:33:59.000000 edx-event-routing-backends-5.3.0/event_routing_backends/migrations/0004_auto_20211025_1053.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-12 07:33:59.000000 edx-event-routing-backends-5.3.0/event_routing_backends/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     9131 2023-05-12 07:33:59.000000 edx-event-routing-backends-5.3.0/event_routing_backends/models.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-12 07:34:04.433394 edx-event-routing-backends-5.3.0/event_routing_backends/processors/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-12 07:33:59.000000 edx-event-routing-backends-5.3.0/event_routing_backends/processors/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-12 07:34:04.437394 edx-event-routing-backends-5.3.0/event_routing_backends/processors/caliper/
--rw-r--r--   0 runner    (1001) docker     (122)      896 2023-05-12 07:33:59.000000 edx-event-routing-backends-5.3.0/event_routing_backends/processors/caliper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      151 2023-05-12 07:33:59.000000 edx-event-routing-backends-5.3.0/event_routing_backends/processors/caliper/constants.py
--rw-r--r--   0 runner    (1001) docker     (122)      907 2023-05-12 07:33:59.000000 edx-event-routing-backends-5.3.0/event_routing_backends/processors/caliper/envelope_processor.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-12 07:34:04.437394 edx-event-routing-backends-5.3.0/event_routing_backends/processors/caliper/event_transformers/
--rw-r--r--   0 runner    (1001) docker     (122)      598 2023-05-12 07:33:59.000000 edx-event-routing-backends-5.3.0/event_routing_backends/processors/caliper/event_transformers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2035 2023-05-12 07:33:59.000000 edx-event-routing-backends-5.3.0/event_routing_backends/processors/caliper/event_transformers/enrollment_events.py
--rw-r--r--   0 runner    (1001) docker     (122)     3213 2023-05-12 07:33:59.000000 edx-event-routing-backends-5.3.0/event_routing_backends/processors/caliper/event_transformers/navigation_events.py
--rw-r--r--   0 runner    (1001) docker     (122)     5823 2023-05-12 07:33:59.000000 edx-event-routing-backends-5.3.0/event_routing_backends/processors/caliper/event_transformers/problem_interaction_events.py
--rw-r--r--   0 runner    (1001) docker     (122)     5861 2023-05-12 07:33:59.000000 edx-event-routing-backends-5.3.0/event_routing_backends/processors/caliper/event_transformers/video_events.py
--rw-r--r--   0 runner    (1001) docker     (122)      302 2023-05-12 07:33:59.000000 edx-event-routing-backends-5.3.0/event_routing_backends/processors/caliper/registry.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-12 07:34:04.437394 edx-event-routing-backends-5.3.0/event_routing_backends/processors/caliper/tests/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-12 07:33:59.000000 edx-event-routing-backends-5.3.0/event_routing_backends/processors/caliper/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3337 2023-05-12 07:33:59.000000 edx-event-routing-backends-5.3.0/event_routing_backends/processors/caliper/tests/test_caliper.py
--rw-r--r--   0 runner    (1001) docker     (122)     1290 2023-05-12 07:33:59.000000 edx-event-routing-backends-5.3.0/event_routing_backends/processors/caliper/tests/test_envelope_processor.py
--rw-r--r--   0 runner    (1001) docker     (122)     1423 2023-05-12 07:33:59.000000 edx-event-routing-backends-5.3.0/event_routing_backends/processors/caliper/tests/test_transformers.py
--rw-r--r--   0 runner    (1001) docker     (122)     2404 2023-05-12 07:33:59.000000 edx-event-routing-backends-5.3.0/event_routing_backends/processors/caliper/transformer.py
--rw-r--r--   0 runner    (1001) docker     (122)     1615 2023-05-12 07:33:59.000000 edx-event-routing-backends-5.3.0/event_routing_backends/processors/caliper/transformer_processor.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-12 07:34:04.437394 edx-event-routing-backends-5.3.0/event_routing_backends/processors/mixins/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-12 07:33:59.000000 edx-event-routing-backends-5.3.0/event_routing_backends/processors/mixins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6871 2023-05-12 07:33:59.000000 edx-event-routing-backends-5.3.0/event_routing_backends/processors/mixins/base_transformer.py
--rw-r--r--   0 runner    (1001) docker     (122)     3018 2023-05-12 07:33:59.000000 edx-event-routing-backends-5.3.0/event_routing_backends/processors/mixins/base_transformer_processor.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-12 07:34:04.437394 edx-event-routing-backends-5.3.0/event_routing_backends/processors/tests/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-12 07:33:59.000000 edx-event-routing-backends-5.3.0/event_routing_backends/processors/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4349 2023-05-12 07:33:59.000000 edx-event-routing-backends-5.3.0/event_routing_backends/processors/tests/transformers_test_mixin.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-12 07:34:04.437394 edx-event-routing-backends-5.3.0/event_routing_backends/processors/transformer_utils/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-12 07:33:59.000000 edx-event-routing-backends-5.3.0/event_routing_backends/processors/transformer_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      165 2023-05-12 07:33:59.000000 edx-event-routing-backends-5.3.0/event_routing_backends/processors/transformer_utils/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (122)     2759 2023-05-12 07:33:59.000000 edx-event-routing-backends-5.3.0/event_routing_backends/processors/transformer_utils/registry.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-12 07:34:04.441394 edx-event-routing-backends-5.3.0/event_routing_backends/processors/transformer_utils/tests/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-12 07:33:59.000000 edx-event-routing-backends-5.3.0/event_routing_backends/processors/transformer_utils/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1059 2023-05-12 07:33:59.000000 edx-event-routing-backends-5.3.0/event_routing_backends/processors/transformer_utils/tests/test_registry.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-12 07:34:04.441394 edx-event-routing-backends-5.3.0/event_routing_backends/processors/xapi/
--rw-r--r--   0 runner    (1001) docker     (122)      874 2023-05-12 07:33:59.000000 edx-event-routing-backends-5.3.0/event_routing_backends/processors/xapi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4420 2023-05-12 07:33:59.000000 edx-event-routing-backends-5.3.0/event_routing_backends/processors/xapi/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-12 07:34:04.441394 edx-event-routing-backends-5.3.0/event_routing_backends/processors/xapi/event_transformers/
--rw-r--r--   0 runner    (1001) docker     (122)      849 2023-05-12 07:33:59.000000 edx-event-routing-backends-5.3.0/event_routing_backends/processors/xapi/event_transformers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3339 2023-05-12 07:33:59.000000 edx-event-routing-backends-5.3.0/event_routing_backends/processors/xapi/event_transformers/enrollment_events.py
--rw-r--r--   0 runner    (1001) docker     (122)     4585 2023-05-12 07:33:59.000000 edx-event-routing-backends-5.3.0/event_routing_backends/processors/xapi/event_transformers/navigation_events.py
--rw-r--r--   0 runner    (1001) docker     (122)     8634 2023-05-12 07:33:59.000000 edx-event-routing-backends-5.3.0/event_routing_backends/processors/xapi/event_transformers/problem_interaction_events.py
--rw-r--r--   0 runner    (1001) docker     (122)     9997 2023-05-12 07:33:59.000000 edx-event-routing-backends-5.3.0/event_routing_backends/processors/xapi/event_transformers/video_events.py
--rw-r--r--   0 runner    (1001) docker     (122)      293 2023-05-12 07:33:59.000000 edx-event-routing-backends-5.3.0/event_routing_backends/processors/xapi/registry.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-12 07:34:04.441394 edx-event-routing-backends-5.3.0/event_routing_backends/processors/xapi/tests/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-12 07:33:59.000000 edx-event-routing-backends-5.3.0/event_routing_backends/processors/xapi/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2857 2023-05-12 07:33:59.000000 edx-event-routing-backends-5.3.0/event_routing_backends/processors/xapi/tests/test_transformers.py
--rw-r--r--   0 runner    (1001) docker     (122)     2948 2023-05-12 07:33:59.000000 edx-event-routing-backends-5.3.0/event_routing_backends/processors/xapi/tests/test_xapi.py
--rw-r--r--   0 runner    (1001) docker     (122)     5335 2023-05-12 07:33:59.000000 edx-event-routing-backends-5.3.0/event_routing_backends/processors/xapi/transformer.py
--rw-r--r--   0 runner    (1001) docker     (122)     1610 2023-05-12 07:33:59.000000 edx-event-routing-backends-5.3.0/event_routing_backends/processors/xapi/transformer_processor.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-12 07:34:04.445394 edx-event-routing-backends-5.3.0/event_routing_backends/settings/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-12 07:33:59.000000 edx-event-routing-backends-5.3.0/event_routing_backends/settings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     8862 2023-05-12 07:33:59.000000 edx-event-routing-backends-5.3.0/event_routing_backends/settings/common.py
--rw-r--r--   0 runner    (1001) docker     (122)      296 2023-05-12 07:33:59.000000 edx-event-routing-backends-5.3.0/event_routing_backends/settings/devstack.py
--rw-r--r--   0 runner    (1001) docker     (122)     1324 2023-05-12 07:33:59.000000 edx-event-routing-backends-5.3.0/event_routing_backends/settings/production.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-12 07:34:04.425394 edx-event-routing-backends-5.3.0/event_routing_backends/static/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-12 07:34:04.425394 edx-event-routing-backends-5.3.0/event_routing_backends/static/admin/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-12 07:34:04.445394 edx-event-routing-backends-5.3.0/event_routing_backends/static/admin/js/
--rw-r--r--   0 runner    (1001) docker     (122)      812 2023-05-12 07:33:59.000000 edx-event-routing-backends-5.3.0/event_routing_backends/static/admin/js/EventRoutingBankendsConditionalFieldRenderer.js
--rw-r--r--   0 runner    (1001) docker     (122)     3185 2023-05-12 07:33:59.000000 edx-event-routing-backends-5.3.0/event_routing_backends/tasks.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-12 07:34:04.425394 edx-event-routing-backends-5.3.0/event_routing_backends/templates/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-12 07:34:04.445394 edx-event-routing-backends-5.3.0/event_routing_backends/templates/admin/
--rw-r--r--   0 runner    (1001) docker     (122)      232 2023-05-12 07:33:59.000000 edx-event-routing-backends-5.3.0/event_routing_backends/templates/admin/router_conf_change_form.html
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-12 07:34:04.445394 edx-event-routing-backends-5.3.0/event_routing_backends/tests/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-12 07:33:59.000000 edx-event-routing-backends-5.3.0/event_routing_backends/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      527 2023-05-12 07:33:59.000000 edx-event-routing-backends-5.3.0/event_routing_backends/tests/factories.py
--rw-r--r--   0 runner    (1001) docker     (122)     2556 2023-05-12 07:33:59.000000 edx-event-routing-backends-5.3.0/event_routing_backends/tests/test_helpers.py
--rw-r--r--   0 runner    (1001) docker     (122)      856 2023-05-12 07:33:59.000000 edx-event-routing-backends-5.3.0/event_routing_backends/tests/test_mixin.py
--rw-r--r--   0 runner    (1001) docker     (122)     5261 2023-05-12 07:33:59.000000 edx-event-routing-backends-5.3.0/event_routing_backends/tests/test_models.py
--rw-r--r--   0 runner    (1001) docker     (122)     2114 2023-05-12 07:33:59.000000 edx-event-routing-backends-5.3.0/event_routing_backends/tests/test_settings.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-12 07:34:04.445394 edx-event-routing-backends-5.3.0/event_routing_backends/utils/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-12 07:33:59.000000 edx-event-routing-backends-5.3.0/event_routing_backends/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      227 2023-05-12 07:33:59.000000 edx-event-routing-backends-5.3.0/event_routing_backends/utils/fields.py
--rw-r--r--   0 runner    (1001) docker     (122)     2857 2023-05-12 07:33:59.000000 edx-event-routing-backends-5.3.0/event_routing_backends/utils/http_client.py
--rw-r--r--   0 runner    (1001) docker     (122)     2976 2023-05-12 07:33:59.000000 edx-event-routing-backends-5.3.0/event_routing_backends/utils/xapi_lrs_client.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-12 07:34:04.445394 edx-event-routing-backends-5.3.0/requirements/
--rw-r--r--   0 runner    (1001) docker     (122)      282 2023-05-12 07:33:59.000000 edx-event-routing-backends-5.3.0/requirements/base.in
--rw-r--r--   0 runner    (1001) docker     (122)     1084 2023-05-12 07:33:59.000000 edx-event-routing-backends-5.3.0/requirements/constraints.txt
--rw-r--r--   0 runner    (1001) docker     (122)      179 2023-05-12 07:34:04.449395 edx-event-routing-backends-5.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     5842 2023-05-12 07:33:59.000000 edx-event-routing-backends-5.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-18 05:29:42.546476 edx-event-routing-backends-5.3.1/
+-rw-r--r--   0 runner    (1001) docker     (122)     2782 2023-05-18 05:29:37.000000 edx-event-routing-backends-5.3.1/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (122)    35139 2023-05-18 05:29:37.000000 edx-event-routing-backends-5.3.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      222 2023-05-18 05:29:37.000000 edx-event-routing-backends-5.3.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     7288 2023-05-18 05:29:42.546476 edx-event-routing-backends-5.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     3721 2023-05-18 05:29:37.000000 edx-event-routing-backends-5.3.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-18 05:29:42.534475 edx-event-routing-backends-5.3.1/edx_event_routing_backends.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     7288 2023-05-18 05:29:42.000000 edx-event-routing-backends-5.3.1/edx_event_routing_backends.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     4467 2023-05-18 05:29:42.000000 edx-event-routing-backends-5.3.1/edx_event_routing_backends.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-18 05:29:42.000000 edx-event-routing-backends-5.3.1/edx_event_routing_backends.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      193 2023-05-18 05:29:42.000000 edx-event-routing-backends-5.3.1/edx_event_routing_backends.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-18 05:29:42.000000 edx-event-routing-backends-5.3.1/edx_event_routing_backends.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)      135 2023-05-18 05:29:42.000000 edx-event-routing-backends-5.3.1/edx_event_routing_backends.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       23 2023-05-18 05:29:42.000000 edx-event-routing-backends-5.3.1/edx_event_routing_backends.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-18 05:29:42.534475 edx-event-routing-backends-5.3.1/event_routing_backends/
+-rw-r--r--   0 runner    (1001) docker     (122)      190 2023-05-18 05:29:37.000000 edx-event-routing-backends-5.3.1/event_routing_backends/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      685 2023-05-18 05:29:37.000000 edx-event-routing-backends-5.3.1/event_routing_backends/admin.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1427 2023-05-18 05:29:37.000000 edx-event-routing-backends-5.3.1/event_routing_backends/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-18 05:29:42.534475 edx-event-routing-backends-5.3.1/event_routing_backends/backends/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-18 05:29:37.000000 edx-event-routing-backends-5.3.1/event_routing_backends/backends/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5833 2023-05-18 05:29:37.000000 edx-event-routing-backends-5.3.1/event_routing_backends/backends/events_router.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-18 05:29:42.538475 edx-event-routing-backends-5.3.1/event_routing_backends/backends/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-18 05:29:37.000000 edx-event-routing-backends-5.3.1/event_routing_backends/backends/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14217 2023-05-18 05:29:37.000000 edx-event-routing-backends-5.3.1/event_routing_backends/backends/tests/test_events_router.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8399 2023-05-18 05:29:37.000000 edx-event-routing-backends-5.3.1/event_routing_backends/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-18 05:29:42.538475 edx-event-routing-backends-5.3.1/event_routing_backends/migrations/
+-rw-r--r--   0 runner    (1001) docker     (122)     1591 2023-05-18 05:29:37.000000 edx-event-routing-backends-5.3.1/event_routing_backends/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (122)      981 2023-05-18 05:29:37.000000 edx-event-routing-backends-5.3.1/event_routing_backends/migrations/0002_auto_20210503_0648.py
+-rw-r--r--   0 runner    (1001) docker     (122)      484 2023-05-18 05:29:37.000000 edx-event-routing-backends-5.3.1/event_routing_backends/migrations/0003_auto_20210713_0344.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1938 2023-05-18 05:29:37.000000 edx-event-routing-backends-5.3.1/event_routing_backends/migrations/0004_auto_20211025_1053.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-18 05:29:37.000000 edx-event-routing-backends-5.3.1/event_routing_backends/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9131 2023-05-18 05:29:37.000000 edx-event-routing-backends-5.3.1/event_routing_backends/models.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-18 05:29:42.538475 edx-event-routing-backends-5.3.1/event_routing_backends/processors/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-18 05:29:37.000000 edx-event-routing-backends-5.3.1/event_routing_backends/processors/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-18 05:29:42.538475 edx-event-routing-backends-5.3.1/event_routing_backends/processors/caliper/
+-rw-r--r--   0 runner    (1001) docker     (122)      896 2023-05-18 05:29:37.000000 edx-event-routing-backends-5.3.1/event_routing_backends/processors/caliper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      151 2023-05-18 05:29:37.000000 edx-event-routing-backends-5.3.1/event_routing_backends/processors/caliper/constants.py
+-rw-r--r--   0 runner    (1001) docker     (122)      907 2023-05-18 05:29:37.000000 edx-event-routing-backends-5.3.1/event_routing_backends/processors/caliper/envelope_processor.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-18 05:29:42.538475 edx-event-routing-backends-5.3.1/event_routing_backends/processors/caliper/event_transformers/
+-rw-r--r--   0 runner    (1001) docker     (122)      598 2023-05-18 05:29:37.000000 edx-event-routing-backends-5.3.1/event_routing_backends/processors/caliper/event_transformers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2035 2023-05-18 05:29:37.000000 edx-event-routing-backends-5.3.1/event_routing_backends/processors/caliper/event_transformers/enrollment_events.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3213 2023-05-18 05:29:37.000000 edx-event-routing-backends-5.3.1/event_routing_backends/processors/caliper/event_transformers/navigation_events.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5823 2023-05-18 05:29:37.000000 edx-event-routing-backends-5.3.1/event_routing_backends/processors/caliper/event_transformers/problem_interaction_events.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5861 2023-05-18 05:29:37.000000 edx-event-routing-backends-5.3.1/event_routing_backends/processors/caliper/event_transformers/video_events.py
+-rw-r--r--   0 runner    (1001) docker     (122)      302 2023-05-18 05:29:37.000000 edx-event-routing-backends-5.3.1/event_routing_backends/processors/caliper/registry.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-18 05:29:42.538475 edx-event-routing-backends-5.3.1/event_routing_backends/processors/caliper/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-18 05:29:37.000000 edx-event-routing-backends-5.3.1/event_routing_backends/processors/caliper/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3337 2023-05-18 05:29:37.000000 edx-event-routing-backends-5.3.1/event_routing_backends/processors/caliper/tests/test_caliper.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1290 2023-05-18 05:29:37.000000 edx-event-routing-backends-5.3.1/event_routing_backends/processors/caliper/tests/test_envelope_processor.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1423 2023-05-18 05:29:37.000000 edx-event-routing-backends-5.3.1/event_routing_backends/processors/caliper/tests/test_transformers.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2404 2023-05-18 05:29:37.000000 edx-event-routing-backends-5.3.1/event_routing_backends/processors/caliper/transformer.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1615 2023-05-18 05:29:37.000000 edx-event-routing-backends-5.3.1/event_routing_backends/processors/caliper/transformer_processor.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-18 05:29:42.538475 edx-event-routing-backends-5.3.1/event_routing_backends/processors/mixins/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-18 05:29:37.000000 edx-event-routing-backends-5.3.1/event_routing_backends/processors/mixins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6871 2023-05-18 05:29:37.000000 edx-event-routing-backends-5.3.1/event_routing_backends/processors/mixins/base_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3018 2023-05-18 05:29:37.000000 edx-event-routing-backends-5.3.1/event_routing_backends/processors/mixins/base_transformer_processor.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-18 05:29:42.538475 edx-event-routing-backends-5.3.1/event_routing_backends/processors/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-18 05:29:37.000000 edx-event-routing-backends-5.3.1/event_routing_backends/processors/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4349 2023-05-18 05:29:37.000000 edx-event-routing-backends-5.3.1/event_routing_backends/processors/tests/transformers_test_mixin.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-18 05:29:42.542476 edx-event-routing-backends-5.3.1/event_routing_backends/processors/transformer_utils/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-18 05:29:37.000000 edx-event-routing-backends-5.3.1/event_routing_backends/processors/transformer_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      165 2023-05-18 05:29:37.000000 edx-event-routing-backends-5.3.1/event_routing_backends/processors/transformer_utils/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2759 2023-05-18 05:29:37.000000 edx-event-routing-backends-5.3.1/event_routing_backends/processors/transformer_utils/registry.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-18 05:29:42.542476 edx-event-routing-backends-5.3.1/event_routing_backends/processors/transformer_utils/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-18 05:29:37.000000 edx-event-routing-backends-5.3.1/event_routing_backends/processors/transformer_utils/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1059 2023-05-18 05:29:37.000000 edx-event-routing-backends-5.3.1/event_routing_backends/processors/transformer_utils/tests/test_registry.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-18 05:29:42.542476 edx-event-routing-backends-5.3.1/event_routing_backends/processors/xapi/
+-rw-r--r--   0 runner    (1001) docker     (122)      874 2023-05-18 05:29:37.000000 edx-event-routing-backends-5.3.1/event_routing_backends/processors/xapi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4420 2023-05-18 05:29:37.000000 edx-event-routing-backends-5.3.1/event_routing_backends/processors/xapi/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-18 05:29:42.542476 edx-event-routing-backends-5.3.1/event_routing_backends/processors/xapi/event_transformers/
+-rw-r--r--   0 runner    (1001) docker     (122)      849 2023-05-18 05:29:37.000000 edx-event-routing-backends-5.3.1/event_routing_backends/processors/xapi/event_transformers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3339 2023-05-18 05:29:37.000000 edx-event-routing-backends-5.3.1/event_routing_backends/processors/xapi/event_transformers/enrollment_events.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4585 2023-05-18 05:29:37.000000 edx-event-routing-backends-5.3.1/event_routing_backends/processors/xapi/event_transformers/navigation_events.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8634 2023-05-18 05:29:37.000000 edx-event-routing-backends-5.3.1/event_routing_backends/processors/xapi/event_transformers/problem_interaction_events.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9997 2023-05-18 05:29:37.000000 edx-event-routing-backends-5.3.1/event_routing_backends/processors/xapi/event_transformers/video_events.py
+-rw-r--r--   0 runner    (1001) docker     (122)      293 2023-05-18 05:29:37.000000 edx-event-routing-backends-5.3.1/event_routing_backends/processors/xapi/registry.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-18 05:29:42.542476 edx-event-routing-backends-5.3.1/event_routing_backends/processors/xapi/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-18 05:29:37.000000 edx-event-routing-backends-5.3.1/event_routing_backends/processors/xapi/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2857 2023-05-18 05:29:37.000000 edx-event-routing-backends-5.3.1/event_routing_backends/processors/xapi/tests/test_transformers.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2948 2023-05-18 05:29:37.000000 edx-event-routing-backends-5.3.1/event_routing_backends/processors/xapi/tests/test_xapi.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5335 2023-05-18 05:29:37.000000 edx-event-routing-backends-5.3.1/event_routing_backends/processors/xapi/transformer.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1610 2023-05-18 05:29:37.000000 edx-event-routing-backends-5.3.1/event_routing_backends/processors/xapi/transformer_processor.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-18 05:29:42.542476 edx-event-routing-backends-5.3.1/event_routing_backends/settings/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-18 05:29:37.000000 edx-event-routing-backends-5.3.1/event_routing_backends/settings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8862 2023-05-18 05:29:37.000000 edx-event-routing-backends-5.3.1/event_routing_backends/settings/common.py
+-rw-r--r--   0 runner    (1001) docker     (122)      296 2023-05-18 05:29:37.000000 edx-event-routing-backends-5.3.1/event_routing_backends/settings/devstack.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1324 2023-05-18 05:29:37.000000 edx-event-routing-backends-5.3.1/event_routing_backends/settings/production.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-18 05:29:42.534475 edx-event-routing-backends-5.3.1/event_routing_backends/static/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-18 05:29:42.534475 edx-event-routing-backends-5.3.1/event_routing_backends/static/admin/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-18 05:29:42.542476 edx-event-routing-backends-5.3.1/event_routing_backends/static/admin/js/
+-rw-r--r--   0 runner    (1001) docker     (122)      812 2023-05-18 05:29:37.000000 edx-event-routing-backends-5.3.1/event_routing_backends/static/admin/js/EventRoutingBankendsConditionalFieldRenderer.js
+-rw-r--r--   0 runner    (1001) docker     (122)     3185 2023-05-18 05:29:37.000000 edx-event-routing-backends-5.3.1/event_routing_backends/tasks.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-18 05:29:42.534475 edx-event-routing-backends-5.3.1/event_routing_backends/templates/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-18 05:29:42.542476 edx-event-routing-backends-5.3.1/event_routing_backends/templates/admin/
+-rw-r--r--   0 runner    (1001) docker     (122)      232 2023-05-18 05:29:37.000000 edx-event-routing-backends-5.3.1/event_routing_backends/templates/admin/router_conf_change_form.html
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-18 05:29:42.546476 edx-event-routing-backends-5.3.1/event_routing_backends/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-18 05:29:37.000000 edx-event-routing-backends-5.3.1/event_routing_backends/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      527 2023-05-18 05:29:37.000000 edx-event-routing-backends-5.3.1/event_routing_backends/tests/factories.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2556 2023-05-18 05:29:37.000000 edx-event-routing-backends-5.3.1/event_routing_backends/tests/test_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (122)      856 2023-05-18 05:29:37.000000 edx-event-routing-backends-5.3.1/event_routing_backends/tests/test_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5261 2023-05-18 05:29:37.000000 edx-event-routing-backends-5.3.1/event_routing_backends/tests/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2114 2023-05-18 05:29:37.000000 edx-event-routing-backends-5.3.1/event_routing_backends/tests/test_settings.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-18 05:29:42.546476 edx-event-routing-backends-5.3.1/event_routing_backends/utils/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-18 05:29:37.000000 edx-event-routing-backends-5.3.1/event_routing_backends/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      227 2023-05-18 05:29:37.000000 edx-event-routing-backends-5.3.1/event_routing_backends/utils/fields.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2857 2023-05-18 05:29:37.000000 edx-event-routing-backends-5.3.1/event_routing_backends/utils/http_client.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3395 2023-05-18 05:29:37.000000 edx-event-routing-backends-5.3.1/event_routing_backends/utils/xapi_lrs_client.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-18 05:29:42.546476 edx-event-routing-backends-5.3.1/requirements/
+-rw-r--r--   0 runner    (1001) docker     (122)      282 2023-05-18 05:29:37.000000 edx-event-routing-backends-5.3.1/requirements/base.in
+-rw-r--r--   0 runner    (1001) docker     (122)     1084 2023-05-18 05:29:37.000000 edx-event-routing-backends-5.3.1/requirements/constraints.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      179 2023-05-18 05:29:42.546476 edx-event-routing-backends-5.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     5842 2023-05-18 05:29:37.000000 edx-event-routing-backends-5.3.1/setup.py
```

### Comparing `edx-event-routing-backends-5.3.0/CHANGELOG.rst` & `edx-event-routing-backends-5.3.1/CHANGELOG.rst`

 * *Files 4% similar despite different names*

```diff
@@ -10,14 +10,19 @@
    This project adheres to Semantic Versioning (https://semver.org/).
 
 .. There should always be an "Unreleased" section for changes pending release.
 
 Unreleased
 ~~~~~~~~~~
 
+[5.3.1]
+~~~~~~~
+
+* Allow External ID type to fall back to LTI on older versions of edx-platform
+  to preserve backward compatibility
 
 [5.3.0]
 ~~~~~~~
 
 * Use proper externalId types XAPI and CALIPER instead of LTI
 * Make user identifier in xAPI events configurable
 * Switch from ``edx-sphinx-theme`` to ``sphinx-book-theme`` since the former is
```

### Comparing `edx-event-routing-backends-5.3.0/LICENSE.txt` & `edx-event-routing-backends-5.3.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-5.3.0/PKG-INFO` & `edx-event-routing-backends-5.3.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edx-event-routing-backends
-Version: 5.3.0
+Version: 5.3.1
 Summary: Various backends for receiving edX LMS events.
 Home-page: https://github.com/openedx/event-routing-backends
 Author: edX
 Author-email: oscm@edx.org
 License: AGPL 3.0
 Keywords: Python edx
 Classifier: Development Status :: 3 - Alpha
@@ -120,14 +120,19 @@
    This project adheres to Semantic Versioning (https://semver.org/).
 
 .. There should always be an "Unreleased" section for changes pending release.
 
 Unreleased
 ~~~~~~~~~~
 
+[5.3.1]
+~~~~~~~
+
+* Allow External ID type to fall back to LTI on older versions of edx-platform
+  to preserve backward compatibility
 
 [5.3.0]
 ~~~~~~~
 
 * Use proper externalId types XAPI and CALIPER instead of LTI
 * Make user identifier in xAPI events configurable
 * Switch from ``edx-sphinx-theme`` to ``sphinx-book-theme`` since the former is
```

### Comparing `edx-event-routing-backends-5.3.0/README.rst` & `edx-event-routing-backends-5.3.1/README.rst`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-5.3.0/edx_event_routing_backends.egg-info/PKG-INFO` & `edx-event-routing-backends-5.3.1/edx_event_routing_backends.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edx-event-routing-backends
-Version: 5.3.0
+Version: 5.3.1
 Summary: Various backends for receiving edX LMS events.
 Home-page: https://github.com/openedx/event-routing-backends
 Author: edX
 Author-email: oscm@edx.org
 License: AGPL 3.0
 Keywords: Python edx
 Classifier: Development Status :: 3 - Alpha
@@ -120,14 +120,19 @@
    This project adheres to Semantic Versioning (https://semver.org/).
 
 .. There should always be an "Unreleased" section for changes pending release.
 
 Unreleased
 ~~~~~~~~~~
 
+[5.3.1]
+~~~~~~~
+
+* Allow External ID type to fall back to LTI on older versions of edx-platform
+  to preserve backward compatibility
 
 [5.3.0]
 ~~~~~~~
 
 * Use proper externalId types XAPI and CALIPER instead of LTI
 * Make user identifier in xAPI events configurable
 * Switch from ``edx-sphinx-theme`` to ``sphinx-book-theme`` since the former is
```

### Comparing `edx-event-routing-backends-5.3.0/edx_event_routing_backends.egg-info/SOURCES.txt` & `edx-event-routing-backends-5.3.1/edx_event_routing_backends.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-5.3.0/event_routing_backends/admin.py` & `edx-event-routing-backends-5.3.1/event_routing_backends/admin.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-5.3.0/event_routing_backends/apps.py` & `edx-event-routing-backends-5.3.1/event_routing_backends/apps.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-5.3.0/event_routing_backends/backends/events_router.py` & `edx-event-routing-backends-5.3.1/event_routing_backends/backends/events_router.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-5.3.0/event_routing_backends/backends/tests/test_events_router.py` & `edx-event-routing-backends-5.3.1/event_routing_backends/backends/tests/test_events_router.py`

 * *Files 2% similar despite different names*

```diff
@@ -373,14 +373,34 @@
                         'auth_scheme': 'bearer',
                         'auth_key': 'key',
                     }
         client = LrsClient(**host_configurations)
         with self.assertRaises(EventNotDispatched):
             client.send(event_name='test', statement_data={})
 
+    @patch('event_routing_backends.utils.xapi_lrs_client.logger')
+    def test_duplicate_xapi_event_id(self, mocked_logger):
+        """
+        Test that when we receive a 409 response when inserting an XAPI statement
+        we do not raise an exception, but do log it.
+        """
+        mock_duplicate_return = MagicMock()
+        mock_duplicate_return.success = False
+        mock_duplicate_return.response.status = 409
+
+        client = LrsClient({})
+        client.lrs_client = MagicMock()
+        client.lrs_client.save_statement.return_value = mock_duplicate_return
+
+        client.send(event_name='test', statement_data={})
+        self.assertIn(
+            call('Event test received a 409 error indicating the event id already exists.'),
+            mocked_logger.info.mock_calls
+        )
+
     def test_unsuccessful_routing_of_event_http(self):
         host_configurations = {
                         'url': 'http://test4.com',
                         'auth_scheme': 'bearer',
                         'auth_key': 'key',
                     }
         client = HttpClient(**host_configurations)
```

### Comparing `edx-event-routing-backends-5.3.0/event_routing_backends/helpers.py` & `edx-event-routing-backends-5.3.1/event_routing_backends/helpers.py`

 * *Files 14% similar despite different names*

```diff
@@ -59,15 +59,25 @@
     user = get_user(username_or_id)
     if not user:
         logger.info('User with username "%s" does not exist. '
                     'Cannot generate anonymous ID', username_or_id)
 
         anonymous_id = str(uuid.uuid4())
     else:
-        type_name = getattr(ExternalIdType, external_type)
+        # Older versions of edx-platform do not have the XAPI or
+        # Caliper ExternalIdTypes, so we fall back to LTI here.
+        # Eventually this will be a problem when those instances
+        # upgrade and their actor id's all change, unless we
+        # eventually add a setting to force LTI here instead of the
+        # usual type.
+        try:
+            type_name = getattr(ExternalIdType, external_type)
+        except AttributeError:  # pragma: no cover
+            type_name = ExternalIdType.LTI
+
         external_id, _ = ExternalId.add_new_user_id(user, type_name)
         if not external_id:
             raise ValueError("External ID type: %s does not exist" % type_name)
 
         anonymous_id = str(external_id.external_user_id)
 
     return anonymous_id
```

### Comparing `edx-event-routing-backends-5.3.0/event_routing_backends/migrations/0001_initial.py` & `edx-event-routing-backends-5.3.1/event_routing_backends/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-5.3.0/event_routing_backends/migrations/0002_auto_20210503_0648.py` & `edx-event-routing-backends-5.3.1/event_routing_backends/migrations/0002_auto_20210503_0648.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-5.3.0/event_routing_backends/migrations/0004_auto_20211025_1053.py` & `edx-event-routing-backends-5.3.1/event_routing_backends/migrations/0004_auto_20211025_1053.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-5.3.0/event_routing_backends/models.py` & `edx-event-routing-backends-5.3.1/event_routing_backends/models.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-5.3.0/event_routing_backends/processors/caliper/__init__.py` & `edx-event-routing-backends-5.3.1/event_routing_backends/processors/caliper/__init__.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-5.3.0/event_routing_backends/processors/caliper/envelope_processor.py` & `edx-event-routing-backends-5.3.1/event_routing_backends/processors/caliper/envelope_processor.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-5.3.0/event_routing_backends/processors/caliper/event_transformers/__init__.py` & `edx-event-routing-backends-5.3.1/event_routing_backends/processors/caliper/event_transformers/__init__.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-5.3.0/event_routing_backends/processors/caliper/event_transformers/enrollment_events.py` & `edx-event-routing-backends-5.3.1/event_routing_backends/processors/caliper/event_transformers/enrollment_events.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-5.3.0/event_routing_backends/processors/caliper/event_transformers/navigation_events.py` & `edx-event-routing-backends-5.3.1/event_routing_backends/processors/caliper/event_transformers/navigation_events.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-5.3.0/event_routing_backends/processors/caliper/event_transformers/problem_interaction_events.py` & `edx-event-routing-backends-5.3.1/event_routing_backends/processors/caliper/event_transformers/problem_interaction_events.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-5.3.0/event_routing_backends/processors/caliper/event_transformers/video_events.py` & `edx-event-routing-backends-5.3.1/event_routing_backends/processors/caliper/event_transformers/video_events.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-5.3.0/event_routing_backends/processors/caliper/tests/test_caliper.py` & `edx-event-routing-backends-5.3.1/event_routing_backends/processors/caliper/tests/test_caliper.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-5.3.0/event_routing_backends/processors/caliper/tests/test_envelope_processor.py` & `edx-event-routing-backends-5.3.1/event_routing_backends/processors/caliper/tests/test_envelope_processor.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-5.3.0/event_routing_backends/processors/caliper/tests/test_transformers.py` & `edx-event-routing-backends-5.3.1/event_routing_backends/processors/caliper/tests/test_transformers.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-5.3.0/event_routing_backends/processors/caliper/transformer.py` & `edx-event-routing-backends-5.3.1/event_routing_backends/processors/caliper/transformer.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-5.3.0/event_routing_backends/processors/caliper/transformer_processor.py` & `edx-event-routing-backends-5.3.1/event_routing_backends/processors/caliper/transformer_processor.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-5.3.0/event_routing_backends/processors/mixins/base_transformer.py` & `edx-event-routing-backends-5.3.1/event_routing_backends/processors/mixins/base_transformer.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-5.3.0/event_routing_backends/processors/mixins/base_transformer_processor.py` & `edx-event-routing-backends-5.3.1/event_routing_backends/processors/mixins/base_transformer_processor.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-5.3.0/event_routing_backends/processors/tests/transformers_test_mixin.py` & `edx-event-routing-backends-5.3.1/event_routing_backends/processors/tests/transformers_test_mixin.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-5.3.0/event_routing_backends/processors/transformer_utils/registry.py` & `edx-event-routing-backends-5.3.1/event_routing_backends/processors/transformer_utils/registry.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-5.3.0/event_routing_backends/processors/transformer_utils/tests/test_registry.py` & `edx-event-routing-backends-5.3.1/event_routing_backends/processors/transformer_utils/tests/test_registry.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-5.3.0/event_routing_backends/processors/xapi/__init__.py` & `edx-event-routing-backends-5.3.1/event_routing_backends/processors/xapi/__init__.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-5.3.0/event_routing_backends/processors/xapi/constants.py` & `edx-event-routing-backends-5.3.1/event_routing_backends/processors/xapi/constants.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-5.3.0/event_routing_backends/processors/xapi/event_transformers/__init__.py` & `edx-event-routing-backends-5.3.1/event_routing_backends/processors/xapi/event_transformers/__init__.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-5.3.0/event_routing_backends/processors/xapi/event_transformers/enrollment_events.py` & `edx-event-routing-backends-5.3.1/event_routing_backends/processors/xapi/event_transformers/enrollment_events.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-5.3.0/event_routing_backends/processors/xapi/event_transformers/navigation_events.py` & `edx-event-routing-backends-5.3.1/event_routing_backends/processors/xapi/event_transformers/navigation_events.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-5.3.0/event_routing_backends/processors/xapi/event_transformers/problem_interaction_events.py` & `edx-event-routing-backends-5.3.1/event_routing_backends/processors/xapi/event_transformers/problem_interaction_events.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-5.3.0/event_routing_backends/processors/xapi/event_transformers/video_events.py` & `edx-event-routing-backends-5.3.1/event_routing_backends/processors/xapi/event_transformers/video_events.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-5.3.0/event_routing_backends/processors/xapi/tests/test_transformers.py` & `edx-event-routing-backends-5.3.1/event_routing_backends/processors/xapi/tests/test_transformers.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-5.3.0/event_routing_backends/processors/xapi/tests/test_xapi.py` & `edx-event-routing-backends-5.3.1/event_routing_backends/processors/xapi/tests/test_xapi.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-5.3.0/event_routing_backends/processors/xapi/transformer.py` & `edx-event-routing-backends-5.3.1/event_routing_backends/processors/xapi/transformer.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-5.3.0/event_routing_backends/processors/xapi/transformer_processor.py` & `edx-event-routing-backends-5.3.1/event_routing_backends/processors/xapi/transformer_processor.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-5.3.0/event_routing_backends/settings/common.py` & `edx-event-routing-backends-5.3.1/event_routing_backends/settings/common.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-5.3.0/event_routing_backends/settings/production.py` & `edx-event-routing-backends-5.3.1/event_routing_backends/settings/production.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-5.3.0/event_routing_backends/static/admin/js/EventRoutingBankendsConditionalFieldRenderer.js` & `edx-event-routing-backends-5.3.1/event_routing_backends/static/admin/js/EventRoutingBankendsConditionalFieldRenderer.js`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-5.3.0/event_routing_backends/tasks.py` & `edx-event-routing-backends-5.3.1/event_routing_backends/tasks.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-5.3.0/event_routing_backends/tests/factories.py` & `edx-event-routing-backends-5.3.1/event_routing_backends/tests/factories.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-5.3.0/event_routing_backends/tests/test_helpers.py` & `edx-event-routing-backends-5.3.1/event_routing_backends/tests/test_helpers.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-5.3.0/event_routing_backends/tests/test_mixin.py` & `edx-event-routing-backends-5.3.1/event_routing_backends/tests/test_mixin.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-5.3.0/event_routing_backends/tests/test_models.py` & `edx-event-routing-backends-5.3.1/event_routing_backends/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-5.3.0/event_routing_backends/tests/test_settings.py` & `edx-event-routing-backends-5.3.1/event_routing_backends/tests/test_settings.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-5.3.0/event_routing_backends/utils/http_client.py` & `edx-event-routing-backends-5.3.1/event_routing_backends/utils/http_client.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-5.3.0/event_routing_backends/utils/xapi_lrs_client.py` & `edx-event-routing-backends-5.3.1/event_routing_backends/utils/xapi_lrs_client.py`

 * *Files 11% similar despite different names*

```diff
@@ -71,11 +71,17 @@
         Returns:
             requests.Response object
         """
         logger.debug('Sending xAPI statement of edx event "{}" to {}'.format(event_name, self.URL))
 
         response = self.lrs_client.save_statement(statement_data)
         if not response.success:
-            logger.warning('{} request failed for sending xAPI statement of edx event "{}" to {}. '
-                           'Response code: {}. Response: {}'.format(response.request.method, event_name, self.URL,
-                                                                    response.response.code, response.data))
-            raise EventNotDispatched
+            # Tincan doesn't gracefully handle the response code we get from an LRS
+            # when the event id already exists, causing many retries that will never
+            # succeed, so we can eat this here.
+            if response.response.status == 409:
+                logger.info('Event {} received a 409 error indicating the event id already exists.'.format(event_name))
+            else:
+                logger.warning('{} request failed for sending xAPI statement of edx event "{}" to {}. '
+                               'Response code: {}. Response: {}'.format(response.request.method, event_name, self.URL,
+                                                                        response.response.code, response.data))
+                raise EventNotDispatched
```

### Comparing `edx-event-routing-backends-5.3.0/requirements/constraints.txt` & `edx-event-routing-backends-5.3.1/requirements/constraints.txt`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-5.3.0/setup.py` & `edx-event-routing-backends-5.3.1/setup.py`

 * *Files identical despite different names*

