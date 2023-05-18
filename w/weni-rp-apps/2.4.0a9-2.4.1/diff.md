# Comparing `tmp/weni_rp_apps-2.4.0a9.tar.gz` & `tmp/weni_rp_apps-2.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "weni_rp_apps-2.4.0a9.tar", max compression
+gzip compressed data, was "weni_rp_apps-2.4.1.tar", max compression
```

## Comparing `weni_rp_apps-2.4.0a9.tar` & `weni_rp_apps-2.4.1.tar`

### file list

```diff
@@ -1,173 +1,173 @@
--rw-r--r--   0        0        0      646 2023-04-24 21:08:56.024578 weni_rp_apps-2.4.0a9/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-24 21:08:35.135002 weni_rp_apps-2.4.0a9/weni/activities/__init__.py
--rw-r--r--   0        0        0      231 2023-04-24 21:08:35.135002 weni_rp_apps-2.4.0a9/weni/activities/apps.py
--rw-r--r--   0        0        0        0 2023-04-24 21:08:35.135002 weni_rp_apps-2.4.0a9/weni/activities/migrations/__init__.py
--rw-r--r--   0        0        0     1960 2023-04-24 21:08:35.135002 weni_rp_apps-2.4.0a9/weni/activities/signals.py
--rw-r--r--   0        0        0      366 2023-04-24 21:08:35.135002 weni_rp_apps-2.4.0a9/weni/activities/tasks.py
--rw-r--r--   0        0        0      325 2023-04-24 21:08:35.135002 weni_rp_apps-2.4.0a9/weni/analytics_api/README.md
--rw-r--r--   0        0        0       66 2023-04-24 21:08:35.135002 weni_rp_apps-2.4.0a9/weni/analytics_api/__init__.py
--rw-r--r--   0        0        0      264 2023-04-24 21:08:35.135002 weni_rp_apps-2.4.0a9/weni/analytics_api/apps.py
--rw-r--r--   0        0        0    13526 2023-04-24 21:08:35.135002 weni_rp_apps-2.4.0a9/weni/analytics_api/tests.py
--rw-r--r--   0        0        0      475 2023-04-24 21:08:35.135002 weni_rp_apps-2.4.0a9/weni/analytics_api/urls.py
--rw-r--r--   0        0        0     8909 2023-04-24 21:08:35.135002 weni_rp_apps-2.4.0a9/weni/analytics_api/views.py
--rw-r--r--   0        0        0       49 2023-04-24 21:08:35.135002 weni_rp_apps-2.4.0a9/weni/auth/__init__.py
--rw-r--r--   0        0        0      285 2023-04-24 21:08:35.135002 weni_rp_apps-2.4.0a9/weni/auth/apps.py
--rw-r--r--   0        0        0     1401 2023-04-24 21:08:35.135002 weni_rp_apps-2.4.0a9/weni/auth/backends.py
--rw-r--r--   0        0        0      430 2023-04-24 21:08:35.135002 weni_rp_apps-2.4.0a9/weni/auth/decorators.py
--rw-r--r--   0        0        0      733 2023-04-24 21:08:35.135002 weni_rp_apps-2.4.0a9/weni/auth/urls.py
--rw-r--r--   0        0        0     2645 2023-04-24 21:08:35.135002 weni_rp_apps-2.4.0a9/weni/auth/views.py
--rw-r--r--   0        0        0      309 2023-04-24 21:08:35.135002 weni_rp_apps-2.4.0a9/weni/channel_stats/README.md
--rw-r--r--   0        0        0       66 2023-04-24 21:08:35.135002 weni_rp_apps-2.4.0a9/weni/channel_stats/__init__.py
--rw-r--r--   0        0        0      264 2023-04-24 21:08:35.135002 weni_rp_apps-2.4.0a9/weni/channel_stats/apps.py
--rw-r--r--   0        0        0     6157 2023-04-24 21:08:35.135002 weni_rp_apps-2.4.0a9/weni/channel_stats/serializers.py
--rw-r--r--   0        0        0      317 2023-04-24 21:08:35.135002 weni_rp_apps-2.4.0a9/weni/channel_stats/urls.py
--rw-r--r--   0        0        0     3575 2023-04-24 21:08:35.135002 weni_rp_apps-2.4.0a9/weni/channel_stats/views.py
--rw-r--r--   0        0        0        0 2023-04-24 21:08:35.135002 weni_rp_apps-2.4.0a9/weni/grpc/billing/__init__.py
--rw-r--r--   0        0        0      102 2023-04-24 21:08:35.135002 weni_rp_apps-2.4.0a9/weni/grpc/billing/apps.py
--rw-r--r--   0        0        0     3508 2023-04-24 21:08:35.135002 weni_rp_apps-2.4.0a9/weni/grpc/billing/queries.py
--rw-r--r--   0        0        0     3194 2023-04-24 21:08:35.135002 weni_rp_apps-2.4.0a9/weni/grpc/billing/serializers.py
--rw-r--r--   0        0        0     2072 2023-04-24 21:08:35.135002 weni_rp_apps-2.4.0a9/weni/grpc/billing/services.py
--rw-r--r--   0        0        0    11471 2023-04-24 21:08:35.135002 weni_rp_apps-2.4.0a9/weni/grpc/billing/tests.py
--rw-r--r--   0        0        0      231 2023-04-24 21:08:35.135002 weni_rp_apps-2.4.0a9/weni/grpc/billing/urls.py
--rw-r--r--   0        0        0       64 2023-04-24 21:08:35.135002 weni_rp_apps-2.4.0a9/weni/grpc/channel/__init__.py
--rw-r--r--   0        0        0      103 2023-04-24 21:08:35.135002 weni_rp_apps-2.4.0a9/weni/grpc/channel/apps.py
--rw-r--r--   0        0        0      352 2023-04-24 21:08:35.135002 weni_rp_apps-2.4.0a9/weni/grpc/channel/fields.py
--rw-r--r--   0        0        0     4110 2023-04-24 21:08:35.135002 weni_rp_apps-2.4.0a9/weni/grpc/channel/serializers.py
--rw-r--r--   0        0        0     4023 2023-04-24 21:08:35.135002 weni_rp_apps-2.4.0a9/weni/grpc/channel/services.py
--rw-r--r--   0        0        0     7747 2023-04-24 21:08:35.135002 weni_rp_apps-2.4.0a9/weni/grpc/channel/tests.py
--rw-r--r--   0        0        0      341 2023-04-24 21:08:35.135002 weni_rp_apps-2.4.0a9/weni/grpc/channel/urls.py
--rw-r--r--   0        0        0       70 2023-04-24 21:08:35.135002 weni_rp_apps-2.4.0a9/weni/grpc/classifier/__init__.py
--rw-r--r--   0        0        0      109 2023-04-24 21:08:35.135002 weni_rp_apps-2.4.0a9/weni/grpc/classifier/apps.py
--rw-r--r--   0        0        0     1262 2023-04-24 21:08:35.135002 weni_rp_apps-2.4.0a9/weni/grpc/classifier/serializers.py
--rw-r--r--   0        0        0     1175 2023-04-24 21:08:35.135002 weni_rp_apps-2.4.0a9/weni/grpc/classifier/services.py
--rw-r--r--   0        0        0     6460 2023-04-24 21:08:35.135002 weni_rp_apps-2.4.0a9/weni/grpc/classifier/tests.py
--rw-r--r--   0        0        0      249 2023-04-24 21:08:35.135002 weni_rp_apps-2.4.0a9/weni/grpc/classifier/urls.py
--rw-r--r--   0        0        0       61 2023-04-24 21:08:35.135002 weni_rp_apps-2.4.0a9/weni/grpc/core/__init__.py
--rw-r--r--   0        0        0      100 2023-04-24 21:08:35.135002 weni_rp_apps-2.4.0a9/weni/grpc/core/apps.py
--rw-r--r--   0        0        0        0 2023-04-24 21:08:35.135002 weni_rp_apps-2.4.0a9/weni/grpc/core/management/__init__.py
--rw-r--r--   0        0        0        0 2023-04-24 21:08:35.135002 weni_rp_apps-2.4.0a9/weni/grpc/core/management/commands/__init__.py
--rw-r--r--   0        0        0     1573 2023-04-24 21:08:35.135002 weni_rp_apps-2.4.0a9/weni/grpc/core/management/commands/grpc.py
--rw-r--r--   0        0        0     1213 2023-04-24 21:08:35.135002 weni_rp_apps-2.4.0a9/weni/grpc/core/serializers.py
--rw-r--r--   0        0        0      965 2023-04-24 21:08:35.135002 weni_rp_apps-2.4.0a9/weni/grpc/core/services.py
--rw-r--r--   0        0        0        0 2023-04-24 21:08:35.135002 weni_rp_apps-2.4.0a9/weni/grpc/core/tests.py
--rw-r--r--   0        0        0      700 2023-04-24 21:08:35.135002 weni_rp_apps-2.4.0a9/weni/grpc/core/urls.py
--rw-r--r--   0        0        0       58 2023-04-24 21:08:35.135002 weni_rp_apps-2.4.0a9/weni/grpc/flow/__init__.py
--rw-r--r--   0        0        0       97 2023-04-24 21:08:35.135002 weni_rp_apps-2.4.0a9/weni/grpc/flow/apps.py
--rw-r--r--   0        0        0      307 2023-04-24 21:08:35.135002 weni_rp_apps-2.4.0a9/weni/grpc/flow/serializers.py
--rw-r--r--   0        0        0      658 2023-04-24 21:08:35.135002 weni_rp_apps-2.4.0a9/weni/grpc/flow/services.py
--rw-r--r--   0        0        0     2766 2023-04-24 21:08:35.135002 weni_rp_apps-2.4.0a9/weni/grpc/flow/tests.py
--rw-r--r--   0        0        0      213 2023-04-24 21:08:35.135002 weni_rp_apps-2.4.0a9/weni/grpc/flow/urls.py
--rw-r--r--   0        0        0       56 2023-04-24 21:08:35.135002 weni_rp_apps-2.4.0a9/weni/grpc/org/__init__.py
--rw-r--r--   0        0        0       95 2023-04-24 21:08:35.135002 weni_rp_apps-2.4.0a9/weni/grpc/org/apps.py
--rw-r--r--   0        0        0     2770 2023-04-24 21:08:35.139002 weni_rp_apps-2.4.0a9/weni/grpc/org/serializers.py
--rw-r--r--   0        0        0     3957 2023-04-24 21:08:35.139002 weni_rp_apps-2.4.0a9/weni/grpc/org/services.py
--rw-r--r--   0        0        0     9824 2023-04-24 21:08:35.139002 weni_rp_apps-2.4.0a9/weni/grpc/org/tests.py
--rw-r--r--   0        0        0      207 2023-04-24 21:08:35.139002 weni_rp_apps-2.4.0a9/weni/grpc/org/urls.py
--rw-r--r--   0        0        0       68 2023-04-24 21:08:35.139002 weni_rp_apps-2.4.0a9/weni/grpc/statistic/__init__.py
--rw-r--r--   0        0        0      107 2023-04-24 21:08:35.139002 weni_rp_apps-2.4.0a9/weni/grpc/statistic/apps.py
--rw-r--r--   0        0        0      672 2023-04-24 21:08:35.139002 weni_rp_apps-2.4.0a9/weni/grpc/statistic/services.py
--rw-r--r--   0        0        0     3134 2023-04-24 21:08:35.139002 weni_rp_apps-2.4.0a9/weni/grpc/statistic/tests.py
--rw-r--r--   0        0        0      252 2023-04-24 21:08:35.139002 weni_rp_apps-2.4.0a9/weni/grpc/statistic/urls.py
--rw-r--r--   0        0        0       58 2023-04-24 21:08:35.139002 weni_rp_apps-2.4.0a9/weni/grpc/user/__init__.py
--rw-r--r--   0        0        0       97 2023-04-24 21:08:35.139002 weni_rp_apps-2.4.0a9/weni/grpc/user/apps.py
--rw-r--r--   0        0        0      843 2023-04-24 21:08:35.139002 weni_rp_apps-2.4.0a9/weni/grpc/user/serializers.py
--rw-r--r--   0        0        0     3906 2023-04-24 21:08:35.139002 weni_rp_apps-2.4.0a9/weni/grpc/user/services.py
--rw-r--r--   0        0        0    10078 2023-04-24 21:08:35.139002 weni_rp_apps-2.4.0a9/weni/grpc/user/tests.py
--rw-r--r--   0        0        0      347 2023-04-24 21:08:35.139002 weni_rp_apps-2.4.0a9/weni/grpc/user/urls.py
--rw-r--r--   0        0        0        0 2023-04-24 21:08:35.139002 weni_rp_apps-2.4.0a9/weni/internal/__init__.py
--rw-r--r--   0        0        0      328 2023-04-24 21:08:35.139002 weni_rp_apps-2.4.0a9/weni/internal/apps.py
--rw-r--r--   0        0        0      300 2023-04-24 21:08:35.139002 weni_rp_apps-2.4.0a9/weni/internal/authenticators.py
--rw-r--r--   0        0        0     1374 2023-04-24 21:08:35.139002 weni_rp_apps-2.4.0a9/weni/internal/backends.py
--rw-r--r--   0        0        0     5562 2023-04-24 21:08:35.139002 weni_rp_apps-2.4.0a9/weni/internal/channel/serializers.py
--rw-r--r--   0        0        0    16222 2023-04-24 21:08:35.139002 weni_rp_apps-2.4.0a9/weni/internal/channel/tests.py
--rw-r--r--   0        0        0      427 2023-04-24 21:08:35.139002 weni_rp_apps-2.4.0a9/weni/internal/channel/urls.py
--rw-r--r--   0        0        0     7181 2023-04-24 21:08:35.139002 weni_rp_apps-2.4.0a9/weni/internal/channel/views.py
--rw-r--r--   0        0        0     1433 2023-04-24 21:08:35.139002 weni_rp_apps-2.4.0a9/weni/internal/classifier/serializers.py
--rw-r--r--   0        0        0     8525 2023-04-24 21:08:35.139002 weni_rp_apps-2.4.0a9/weni/internal/classifier/tests.py
--rw-r--r--   0        0        0      351 2023-04-24 21:08:35.139002 weni_rp_apps-2.4.0a9/weni/internal/classifier/urls.py
--rw-r--r--   0        0        0     3169 2023-04-24 21:08:35.139002 weni_rp_apps-2.4.0a9/weni/internal/classifier/views.py
--rw-r--r--   0        0        0      107 2023-04-24 21:08:35.139002 weni_rp_apps-2.4.0a9/weni/internal/clients/__init__.py
--rw-r--r--   0        0        0      696 2023-04-24 21:08:35.139002 weni_rp_apps-2.4.0a9/weni/internal/clients/authenticators.py
--rw-r--r--   0        0        0      486 2023-04-24 21:08:35.139002 weni_rp_apps-2.4.0a9/weni/internal/clients/base.py
--rw-r--r--   0        0        0      580 2023-04-24 21:08:35.139002 weni_rp_apps-2.4.0a9/weni/internal/clients/connect.py
--rw-r--r--   0        0        0        0 2023-04-24 21:08:35.139002 weni_rp_apps-2.4.0a9/weni/internal/externals/__init__.py
--rw-r--r--   0        0        0     1308 2023-04-24 21:08:35.139002 weni_rp_apps-2.4.0a9/weni/internal/externals/serializers.py
--rw-r--r--   0        0        0      294 2023-04-24 21:08:35.139002 weni_rp_apps-2.4.0a9/weni/internal/externals/urls.py
--rw-r--r--   0        0        0     1501 2023-04-24 21:08:35.139002 weni_rp_apps-2.4.0a9/weni/internal/externals/views.py
--rw-r--r--   0        0        0        0 2023-04-24 21:08:35.139002 weni_rp_apps-2.4.0a9/weni/internal/flows/__init__.py
--rw-r--r--   0        0        0     1278 2023-04-24 21:08:35.139002 weni_rp_apps-2.4.0a9/weni/internal/flows/serializers.py
--rw-r--r--   0        0        0     4283 2023-04-24 21:08:35.139002 weni_rp_apps-2.4.0a9/weni/internal/flows/tests.py
--rw-r--r--   0        0        0      308 2023-04-24 21:08:35.139002 weni_rp_apps-2.4.0a9/weni/internal/flows/urls.py
--rw-r--r--   0        0        0      974 2023-04-24 21:08:35.139002 weni_rp_apps-2.4.0a9/weni/internal/flows/views.py
--rw-r--r--   0        0        0        0 2023-04-24 21:08:35.139002 weni_rp_apps-2.4.0a9/weni/internal/globals/__init__.py
--rw-r--r--   0        0        0     2286 2023-04-24 21:08:35.139002 weni_rp_apps-2.4.0a9/weni/internal/globals/serializers.py
--rw-r--r--   0        0        0        0 2023-04-24 21:08:35.139002 weni_rp_apps-2.4.0a9/weni/internal/globals/tests/__init__.py
--rw-r--r--   0        0        0     2183 2023-04-24 21:08:35.139002 weni_rp_apps-2.4.0a9/weni/internal/globals/tests/test_serializers.py
--rw-r--r--   0        0        0      220 2023-04-24 21:08:35.139002 weni_rp_apps-2.4.0a9/weni/internal/globals/urls.py
--rw-r--r--   0        0        0     1485 2023-04-24 21:08:35.139002 weni_rp_apps-2.4.0a9/weni/internal/globals/views.py
--rw-r--r--   0        0        0      868 2023-04-24 21:08:35.139002 weni_rp_apps-2.4.0a9/weni/internal/migrations/0001_initial.py
--rw-r--r--   0        0        0     1032 2023-04-24 21:08:35.139002 weni_rp_apps-2.4.0a9/weni/internal/migrations/0002_project.py
--rw-r--r--   0        0        0        0 2023-04-24 21:08:35.139002 weni_rp_apps-2.4.0a9/weni/internal/migrations/__init__.py
--rw-r--r--   0        0        0      813 2023-04-24 21:08:35.139002 weni_rp_apps-2.4.0a9/weni/internal/models.py
--rw-r--r--   0        0        0        0 2023-04-24 21:08:35.139002 weni_rp_apps-2.4.0a9/weni/internal/orgs/__init__.py
--rw-r--r--   0        0        0     3815 2023-04-24 21:08:35.139002 weni_rp_apps-2.4.0a9/weni/internal/orgs/serializers.py
--rw-r--r--   0        0        0    14533 2023-04-24 21:08:35.139002 weni_rp_apps-2.4.0a9/weni/internal/orgs/tests.py
--rw-r--r--   0        0        0      300 2023-04-24 21:08:35.139002 weni_rp_apps-2.4.0a9/weni/internal/orgs/urls.py
--rw-r--r--   0        0        0     4579 2023-04-24 21:08:35.139002 weni_rp_apps-2.4.0a9/weni/internal/orgs/views.py
--rw-r--r--   0        0        0      246 2023-04-24 21:08:35.139002 weni_rp_apps-2.4.0a9/weni/internal/permissions.py
--rw-r--r--   0        0        0     1993 2023-04-24 21:08:35.139002 weni_rp_apps-2.4.0a9/weni/internal/statistic/tests.py
--rw-r--r--   0        0        0      205 2023-04-24 21:08:35.139002 weni_rp_apps-2.4.0a9/weni/internal/statistic/urls.py
--rw-r--r--   0        0        0      831 2023-04-24 21:08:35.139002 weni_rp_apps-2.4.0a9/weni/internal/statistic/views.py
--rw-r--r--   0        0        0        0 2023-04-24 21:08:35.139002 weni_rp_apps-2.4.0a9/weni/internal/tests/__init__.py
--rw-r--r--   0        0        0     1249 2023-04-24 21:08:35.139002 weni_rp_apps-2.4.0a9/weni/internal/tests/test_models.py
--rw-r--r--   0        0        0        0 2023-04-24 21:08:35.139002 weni_rp_apps-2.4.0a9/weni/internal/tickets/__init__.py
--rw-r--r--   0        0        0     1152 2023-04-24 21:08:35.139002 weni_rp_apps-2.4.0a9/weni/internal/tickets/serializers.py
--rw-r--r--   0        0        0        0 2023-04-24 21:08:35.139002 weni_rp_apps-2.4.0a9/weni/internal/tickets/tests/__init__.py
--rw-r--r--   0        0        0     3398 2023-04-24 21:08:35.139002 weni_rp_apps-2.4.0a9/weni/internal/tickets/tests/test_views.py
--rw-r--r--   0        0        0      443 2023-04-24 21:08:35.139002 weni_rp_apps-2.4.0a9/weni/internal/tickets/urls.py
--rw-r--r--   0        0        0     1858 2023-04-24 21:08:35.139002 weni_rp_apps-2.4.0a9/weni/internal/tickets/views.py
--rw-r--r--   0        0        0     1315 2023-04-24 21:08:35.139002 weni_rp_apps-2.4.0a9/weni/internal/urls.py
--rw-r--r--   0        0        0        0 2023-04-24 21:08:35.139002 weni_rp_apps-2.4.0a9/weni/internal/users/__init__.py
--rw-r--r--   0        0        0      845 2023-04-24 21:08:35.139002 weni_rp_apps-2.4.0a9/weni/internal/users/serializers.py
--rw-r--r--   0        0        0    11864 2023-04-24 21:08:35.139002 weni_rp_apps-2.4.0a9/weni/internal/users/tests.py
--rw-r--r--   0        0        0      711 2023-04-24 21:08:35.139002 weni_rp_apps-2.4.0a9/weni/internal/users/urls.py
--rw-r--r--   0        0        0     6022 2023-04-24 21:08:35.139002 weni_rp_apps-2.4.0a9/weni/internal/users/views.py
--rw-r--r--   0        0        0      555 2023-04-24 21:08:35.139002 weni_rp_apps-2.4.0a9/weni/internal/views.py
--rw-r--r--   0        0        0       55 2023-04-24 21:08:35.139002 weni_rp_apps-2.4.0a9/weni/orgs_api/__init__.py
--rw-r--r--   0        0        0      253 2023-04-24 21:08:35.139002 weni_rp_apps-2.4.0a9/weni/orgs_api/apps.py
--rw-r--r--   0        0        0      906 2023-04-24 21:08:35.139002 weni_rp_apps-2.4.0a9/weni/orgs_api/serializers.py
--rw-r--r--   0        0        0     4030 2023-04-24 21:08:35.139002 weni_rp_apps-2.4.0a9/weni/orgs_api/tests.py
--rw-r--r--   0        0        0      178 2023-04-24 21:08:35.139002 weni_rp_apps-2.4.0a9/weni/orgs_api/urls.py
--rw-r--r--   0        0        0     1444 2023-04-24 21:08:35.139002 weni_rp_apps-2.4.0a9/weni/orgs_api/views.py
--rw-r--r--   0        0        0       45 2023-04-24 21:08:35.139002 weni_rp_apps-2.4.0a9/weni/s3/__init__.py
--rw-r--r--   0        0        0      243 2023-04-24 21:08:35.139002 weni_rp_apps-2.4.0a9/weni/s3/apps.py
--rw-r--r--   0        0        0      250 2023-04-24 21:08:35.139002 weni_rp_apps-2.4.0a9/weni/s3/urls.py
--rw-r--r--   0        0        0      550 2023-04-24 21:08:35.139002 weni_rp_apps-2.4.0a9/weni/s3/views.py
--rw-r--r--   0        0        0       79 2023-04-24 21:08:35.139002 weni_rp_apps-2.4.0a9/weni/serializers/__init__.py
--rw-r--r--   0        0        0      725 2023-04-24 21:08:35.139002 weni_rp_apps-2.4.0a9/weni/serializers/fields.py
--rw-r--r--   0        0        0      281 2023-04-24 21:08:35.139002 weni_rp_apps-2.4.0a9/weni/success_orgs/apps.py
--rw-r--r--   0        0        0     2403 2023-04-24 21:08:35.139002 weni_rp_apps-2.4.0a9/weni/success_orgs/business.py
--rw-r--r--   0        0        0      563 2023-04-24 21:08:35.139002 weni_rp_apps-2.4.0a9/weni/success_orgs/serializers.py
--rw-r--r--   0        0        0        0 2023-04-24 21:08:35.139002 weni_rp_apps-2.4.0a9/weni/success_orgs/tests/__init__.py
--rw-r--r--   0        0        0     2980 2023-04-24 21:08:35.139002 weni_rp_apps-2.4.0a9/weni/success_orgs/tests/test_business.py
--rw-r--r--   0        0        0      494 2023-04-24 21:08:35.139002 weni_rp_apps-2.4.0a9/weni/success_orgs/urls.py
--rw-r--r--   0        0        0     2774 2023-04-24 21:08:35.139002 weni_rp_apps-2.4.0a9/weni/success_orgs/views.py
--rw-r--r--   0        0        0      318 2023-04-24 21:08:35.139002 weni_rp_apps-2.4.0a9/weni/template_message/README.md
--rw-r--r--   0        0        0       72 2023-04-24 21:08:35.139002 weni_rp_apps-2.4.0a9/weni/template_message/__init__.py
--rw-r--r--   0        0        0      294 2023-04-24 21:08:35.139002 weni_rp_apps-2.4.0a9/weni/template_message/apps.py
--rw-r--r--   0        0        0     2041 2023-04-24 21:08:35.139002 weni_rp_apps-2.4.0a9/weni/template_message/serializers.py
--rw-r--r--   0        0        0     5295 2023-04-24 21:08:35.143002 weni_rp_apps-2.4.0a9/weni/template_message/tests.py
--rw-r--r--   0        0        0      344 2023-04-24 21:08:35.143002 weni_rp_apps-2.4.0a9/weni/template_message/urls.py
--rw-r--r--   0        0        0     1651 2023-04-24 21:08:35.143002 weni_rp_apps-2.4.0a9/weni/template_message/views.py
--rw-r--r--   0        0        0        0 2023-04-24 21:08:35.143002 weni_rp_apps-2.4.0a9/weni/templates/__init__.py
--rw-r--r--   0        0        0      559 2023-04-24 21:08:35.143002 weni_rp_apps-2.4.0a9/weni/templates/context_processors.py
--rw-r--r--   0        0        0      315 2023-04-24 21:08:35.143002 weni_rp_apps-2.4.0a9/weni/ticketer_queues/README.md
--rw-r--r--   0        0        0       70 2023-04-24 21:08:35.143002 weni_rp_apps-2.4.0a9/weni/ticketer_queues/__init__.py
--rw-r--r--   0        0        0      291 2023-04-24 21:08:35.143002 weni_rp_apps-2.4.0a9/weni/ticketer_queues/apps.py
--rw-r--r--   0        0        0      242 2023-04-24 21:08:35.143002 weni_rp_apps-2.4.0a9/weni/ticketer_queues/serializers.py
--rw-r--r--   0        0        0     1584 2023-04-24 21:08:35.143002 weni_rp_apps-2.4.0a9/weni/ticketer_queues/tests.py
--rw-r--r--   0        0        0      378 2023-04-24 21:08:35.143002 weni_rp_apps-2.4.0a9/weni/ticketer_queues/urls.py
--rw-r--r--   0        0        0      849 2023-04-24 21:08:35.143002 weni_rp_apps-2.4.0a9/weni/ticketer_queues/views.py
--rw-r--r--   0        0        0        0 2023-04-24 21:08:35.143002 weni_rp_apps-2.4.0a9/weni/utils/__init__.py
--rw-r--r--   0        0        0     1091 2023-04-24 21:08:35.143002 weni_rp_apps-2.4.0a9/weni/utils/app_config.py
--rw-r--r--   0        0        0     1003 1970-01-01 00:00:00.000000 weni_rp_apps-2.4.0a9/PKG-INFO
+-rw-r--r--   0        0        0      644 2023-05-18 01:34:12.924247 weni_rp_apps-2.4.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-18 01:33:52.639371 weni_rp_apps-2.4.1/weni/activities/__init__.py
+-rw-r--r--   0        0        0      231 2023-05-18 01:33:52.639371 weni_rp_apps-2.4.1/weni/activities/apps.py
+-rw-r--r--   0        0        0        0 2023-05-18 01:33:52.639371 weni_rp_apps-2.4.1/weni/activities/migrations/__init__.py
+-rw-r--r--   0        0        0     1960 2023-05-18 01:33:52.639371 weni_rp_apps-2.4.1/weni/activities/signals.py
+-rw-r--r--   0        0        0      366 2023-05-18 01:33:52.639371 weni_rp_apps-2.4.1/weni/activities/tasks.py
+-rw-r--r--   0        0        0      325 2023-05-18 01:33:52.639371 weni_rp_apps-2.4.1/weni/analytics_api/README.md
+-rw-r--r--   0        0        0       66 2023-05-18 01:33:52.639371 weni_rp_apps-2.4.1/weni/analytics_api/__init__.py
+-rw-r--r--   0        0        0      264 2023-05-18 01:33:52.639371 weni_rp_apps-2.4.1/weni/analytics_api/apps.py
+-rw-r--r--   0        0        0    13526 2023-05-18 01:33:52.639371 weni_rp_apps-2.4.1/weni/analytics_api/tests.py
+-rw-r--r--   0        0        0      475 2023-05-18 01:33:52.639371 weni_rp_apps-2.4.1/weni/analytics_api/urls.py
+-rw-r--r--   0        0        0     8909 2023-05-18 01:33:52.639371 weni_rp_apps-2.4.1/weni/analytics_api/views.py
+-rw-r--r--   0        0        0       49 2023-05-18 01:33:52.639371 weni_rp_apps-2.4.1/weni/auth/__init__.py
+-rw-r--r--   0        0        0      285 2023-05-18 01:33:52.639371 weni_rp_apps-2.4.1/weni/auth/apps.py
+-rw-r--r--   0        0        0     1321 2023-05-18 01:33:52.639371 weni_rp_apps-2.4.1/weni/auth/backends.py
+-rw-r--r--   0        0        0      430 2023-05-18 01:33:52.639371 weni_rp_apps-2.4.1/weni/auth/decorators.py
+-rw-r--r--   0        0        0      733 2023-05-18 01:33:52.639371 weni_rp_apps-2.4.1/weni/auth/urls.py
+-rw-r--r--   0        0        0     2645 2023-05-18 01:33:52.639371 weni_rp_apps-2.4.1/weni/auth/views.py
+-rw-r--r--   0        0        0      309 2023-05-18 01:33:52.639371 weni_rp_apps-2.4.1/weni/channel_stats/README.md
+-rw-r--r--   0        0        0       66 2023-05-18 01:33:52.639371 weni_rp_apps-2.4.1/weni/channel_stats/__init__.py
+-rw-r--r--   0        0        0      264 2023-05-18 01:33:52.639371 weni_rp_apps-2.4.1/weni/channel_stats/apps.py
+-rw-r--r--   0        0        0     6157 2023-05-18 01:33:52.639371 weni_rp_apps-2.4.1/weni/channel_stats/serializers.py
+-rw-r--r--   0        0        0      317 2023-05-18 01:33:52.639371 weni_rp_apps-2.4.1/weni/channel_stats/urls.py
+-rw-r--r--   0        0        0     3575 2023-05-18 01:33:52.639371 weni_rp_apps-2.4.1/weni/channel_stats/views.py
+-rw-r--r--   0        0        0        0 2023-05-18 01:33:52.639371 weni_rp_apps-2.4.1/weni/grpc/billing/__init__.py
+-rw-r--r--   0        0        0      102 2023-05-18 01:33:52.639371 weni_rp_apps-2.4.1/weni/grpc/billing/apps.py
+-rw-r--r--   0        0        0     3508 2023-05-18 01:33:52.639371 weni_rp_apps-2.4.1/weni/grpc/billing/queries.py
+-rw-r--r--   0        0        0     3194 2023-05-18 01:33:52.639371 weni_rp_apps-2.4.1/weni/grpc/billing/serializers.py
+-rw-r--r--   0        0        0     2072 2023-05-18 01:33:52.639371 weni_rp_apps-2.4.1/weni/grpc/billing/services.py
+-rw-r--r--   0        0        0    11471 2023-05-18 01:33:52.639371 weni_rp_apps-2.4.1/weni/grpc/billing/tests.py
+-rw-r--r--   0        0        0      231 2023-05-18 01:33:52.639371 weni_rp_apps-2.4.1/weni/grpc/billing/urls.py
+-rw-r--r--   0        0        0       64 2023-05-18 01:33:52.639371 weni_rp_apps-2.4.1/weni/grpc/channel/__init__.py
+-rw-r--r--   0        0        0      103 2023-05-18 01:33:52.639371 weni_rp_apps-2.4.1/weni/grpc/channel/apps.py
+-rw-r--r--   0        0        0      352 2023-05-18 01:33:52.639371 weni_rp_apps-2.4.1/weni/grpc/channel/fields.py
+-rw-r--r--   0        0        0     4110 2023-05-18 01:33:52.639371 weni_rp_apps-2.4.1/weni/grpc/channel/serializers.py
+-rw-r--r--   0        0        0     4023 2023-05-18 01:33:52.639371 weni_rp_apps-2.4.1/weni/grpc/channel/services.py
+-rw-r--r--   0        0        0     7747 2023-05-18 01:33:52.639371 weni_rp_apps-2.4.1/weni/grpc/channel/tests.py
+-rw-r--r--   0        0        0      341 2023-05-18 01:33:52.639371 weni_rp_apps-2.4.1/weni/grpc/channel/urls.py
+-rw-r--r--   0        0        0       70 2023-05-18 01:33:52.639371 weni_rp_apps-2.4.1/weni/grpc/classifier/__init__.py
+-rw-r--r--   0        0        0      109 2023-05-18 01:33:52.639371 weni_rp_apps-2.4.1/weni/grpc/classifier/apps.py
+-rw-r--r--   0        0        0     1262 2023-05-18 01:33:52.639371 weni_rp_apps-2.4.1/weni/grpc/classifier/serializers.py
+-rw-r--r--   0        0        0     1175 2023-05-18 01:33:52.639371 weni_rp_apps-2.4.1/weni/grpc/classifier/services.py
+-rw-r--r--   0        0        0     6460 2023-05-18 01:33:52.639371 weni_rp_apps-2.4.1/weni/grpc/classifier/tests.py
+-rw-r--r--   0        0        0      249 2023-05-18 01:33:52.639371 weni_rp_apps-2.4.1/weni/grpc/classifier/urls.py
+-rw-r--r--   0        0        0       61 2023-05-18 01:33:52.639371 weni_rp_apps-2.4.1/weni/grpc/core/__init__.py
+-rw-r--r--   0        0        0      100 2023-05-18 01:33:52.639371 weni_rp_apps-2.4.1/weni/grpc/core/apps.py
+-rw-r--r--   0        0        0        0 2023-05-18 01:33:52.639371 weni_rp_apps-2.4.1/weni/grpc/core/management/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-18 01:33:52.639371 weni_rp_apps-2.4.1/weni/grpc/core/management/commands/__init__.py
+-rw-r--r--   0        0        0     1573 2023-05-18 01:33:52.639371 weni_rp_apps-2.4.1/weni/grpc/core/management/commands/grpc.py
+-rw-r--r--   0        0        0     1213 2023-05-18 01:33:52.639371 weni_rp_apps-2.4.1/weni/grpc/core/serializers.py
+-rw-r--r--   0        0        0      965 2023-05-18 01:33:52.639371 weni_rp_apps-2.4.1/weni/grpc/core/services.py
+-rw-r--r--   0        0        0        0 2023-05-18 01:33:52.639371 weni_rp_apps-2.4.1/weni/grpc/core/tests.py
+-rw-r--r--   0        0        0      700 2023-05-18 01:33:52.639371 weni_rp_apps-2.4.1/weni/grpc/core/urls.py
+-rw-r--r--   0        0        0       58 2023-05-18 01:33:52.639371 weni_rp_apps-2.4.1/weni/grpc/flow/__init__.py
+-rw-r--r--   0        0        0       97 2023-05-18 01:33:52.639371 weni_rp_apps-2.4.1/weni/grpc/flow/apps.py
+-rw-r--r--   0        0        0      307 2023-05-18 01:33:52.639371 weni_rp_apps-2.4.1/weni/grpc/flow/serializers.py
+-rw-r--r--   0        0        0      658 2023-05-18 01:33:52.639371 weni_rp_apps-2.4.1/weni/grpc/flow/services.py
+-rw-r--r--   0        0        0     2766 2023-05-18 01:33:52.639371 weni_rp_apps-2.4.1/weni/grpc/flow/tests.py
+-rw-r--r--   0        0        0      213 2023-05-18 01:33:52.639371 weni_rp_apps-2.4.1/weni/grpc/flow/urls.py
+-rw-r--r--   0        0        0       56 2023-05-18 01:33:52.639371 weni_rp_apps-2.4.1/weni/grpc/org/__init__.py
+-rw-r--r--   0        0        0       95 2023-05-18 01:33:52.639371 weni_rp_apps-2.4.1/weni/grpc/org/apps.py
+-rw-r--r--   0        0        0     2770 2023-05-18 01:33:52.639371 weni_rp_apps-2.4.1/weni/grpc/org/serializers.py
+-rw-r--r--   0        0        0     3957 2023-05-18 01:33:52.639371 weni_rp_apps-2.4.1/weni/grpc/org/services.py
+-rw-r--r--   0        0        0     9824 2023-05-18 01:33:52.639371 weni_rp_apps-2.4.1/weni/grpc/org/tests.py
+-rw-r--r--   0        0        0      207 2023-05-18 01:33:52.639371 weni_rp_apps-2.4.1/weni/grpc/org/urls.py
+-rw-r--r--   0        0        0       68 2023-05-18 01:33:52.639371 weni_rp_apps-2.4.1/weni/grpc/statistic/__init__.py
+-rw-r--r--   0        0        0      107 2023-05-18 01:33:52.639371 weni_rp_apps-2.4.1/weni/grpc/statistic/apps.py
+-rw-r--r--   0        0        0      672 2023-05-18 01:33:52.639371 weni_rp_apps-2.4.1/weni/grpc/statistic/services.py
+-rw-r--r--   0        0        0     3134 2023-05-18 01:33:52.643371 weni_rp_apps-2.4.1/weni/grpc/statistic/tests.py
+-rw-r--r--   0        0        0      252 2023-05-18 01:33:52.643371 weni_rp_apps-2.4.1/weni/grpc/statistic/urls.py
+-rw-r--r--   0        0        0       58 2023-05-18 01:33:52.643371 weni_rp_apps-2.4.1/weni/grpc/user/__init__.py
+-rw-r--r--   0        0        0       97 2023-05-18 01:33:52.643371 weni_rp_apps-2.4.1/weni/grpc/user/apps.py
+-rw-r--r--   0        0        0      843 2023-05-18 01:33:52.643371 weni_rp_apps-2.4.1/weni/grpc/user/serializers.py
+-rw-r--r--   0        0        0     3906 2023-05-18 01:33:52.643371 weni_rp_apps-2.4.1/weni/grpc/user/services.py
+-rw-r--r--   0        0        0    10078 2023-05-18 01:33:52.643371 weni_rp_apps-2.4.1/weni/grpc/user/tests.py
+-rw-r--r--   0        0        0      347 2023-05-18 01:33:52.643371 weni_rp_apps-2.4.1/weni/grpc/user/urls.py
+-rw-r--r--   0        0        0        0 2023-05-18 01:33:52.643371 weni_rp_apps-2.4.1/weni/internal/__init__.py
+-rw-r--r--   0        0        0      328 2023-05-18 01:33:52.643371 weni_rp_apps-2.4.1/weni/internal/apps.py
+-rw-r--r--   0        0        0      300 2023-05-18 01:33:52.643371 weni_rp_apps-2.4.1/weni/internal/authenticators.py
+-rw-r--r--   0        0        0     1374 2023-05-18 01:33:52.643371 weni_rp_apps-2.4.1/weni/internal/backends.py
+-rw-r--r--   0        0        0     5562 2023-05-18 01:33:52.643371 weni_rp_apps-2.4.1/weni/internal/channel/serializers.py
+-rw-r--r--   0        0        0    16222 2023-05-18 01:33:52.643371 weni_rp_apps-2.4.1/weni/internal/channel/tests.py
+-rw-r--r--   0        0        0      427 2023-05-18 01:33:52.643371 weni_rp_apps-2.4.1/weni/internal/channel/urls.py
+-rw-r--r--   0        0        0     7611 2023-05-18 01:33:52.643371 weni_rp_apps-2.4.1/weni/internal/channel/views.py
+-rw-r--r--   0        0        0     1433 2023-05-18 01:33:52.643371 weni_rp_apps-2.4.1/weni/internal/classifier/serializers.py
+-rw-r--r--   0        0        0     8525 2023-05-18 01:33:52.643371 weni_rp_apps-2.4.1/weni/internal/classifier/tests.py
+-rw-r--r--   0        0        0      351 2023-05-18 01:33:52.643371 weni_rp_apps-2.4.1/weni/internal/classifier/urls.py
+-rw-r--r--   0        0        0     3169 2023-05-18 01:33:52.643371 weni_rp_apps-2.4.1/weni/internal/classifier/views.py
+-rw-r--r--   0        0        0      107 2023-05-18 01:33:52.643371 weni_rp_apps-2.4.1/weni/internal/clients/__init__.py
+-rw-r--r--   0        0        0      696 2023-05-18 01:33:52.643371 weni_rp_apps-2.4.1/weni/internal/clients/authenticators.py
+-rw-r--r--   0        0        0      486 2023-05-18 01:33:52.643371 weni_rp_apps-2.4.1/weni/internal/clients/base.py
+-rw-r--r--   0        0        0      580 2023-05-18 01:33:52.643371 weni_rp_apps-2.4.1/weni/internal/clients/connect.py
+-rw-r--r--   0        0        0        0 2023-05-18 01:33:52.643371 weni_rp_apps-2.4.1/weni/internal/externals/__init__.py
+-rw-r--r--   0        0        0     1308 2023-05-18 01:33:52.643371 weni_rp_apps-2.4.1/weni/internal/externals/serializers.py
+-rw-r--r--   0        0        0      294 2023-05-18 01:33:52.643371 weni_rp_apps-2.4.1/weni/internal/externals/urls.py
+-rw-r--r--   0        0        0     1501 2023-05-18 01:33:52.643371 weni_rp_apps-2.4.1/weni/internal/externals/views.py
+-rw-r--r--   0        0        0        0 2023-05-18 01:33:52.643371 weni_rp_apps-2.4.1/weni/internal/flows/__init__.py
+-rw-r--r--   0        0        0     1278 2023-05-18 01:33:52.643371 weni_rp_apps-2.4.1/weni/internal/flows/serializers.py
+-rw-r--r--   0        0        0     4283 2023-05-18 01:33:52.643371 weni_rp_apps-2.4.1/weni/internal/flows/tests.py
+-rw-r--r--   0        0        0      308 2023-05-18 01:33:52.643371 weni_rp_apps-2.4.1/weni/internal/flows/urls.py
+-rw-r--r--   0        0        0      974 2023-05-18 01:33:52.643371 weni_rp_apps-2.4.1/weni/internal/flows/views.py
+-rw-r--r--   0        0        0        0 2023-05-18 01:33:52.643371 weni_rp_apps-2.4.1/weni/internal/globals/__init__.py
+-rw-r--r--   0        0        0     2286 2023-05-18 01:33:52.643371 weni_rp_apps-2.4.1/weni/internal/globals/serializers.py
+-rw-r--r--   0        0        0        0 2023-05-18 01:33:52.643371 weni_rp_apps-2.4.1/weni/internal/globals/tests/__init__.py
+-rw-r--r--   0        0        0     2183 2023-05-18 01:33:52.643371 weni_rp_apps-2.4.1/weni/internal/globals/tests/test_serializers.py
+-rw-r--r--   0        0        0      220 2023-05-18 01:33:52.643371 weni_rp_apps-2.4.1/weni/internal/globals/urls.py
+-rw-r--r--   0        0        0     1485 2023-05-18 01:33:52.643371 weni_rp_apps-2.4.1/weni/internal/globals/views.py
+-rw-r--r--   0        0        0      868 2023-05-18 01:33:52.643371 weni_rp_apps-2.4.1/weni/internal/migrations/0001_initial.py
+-rw-r--r--   0        0        0     1032 2023-05-18 01:33:52.643371 weni_rp_apps-2.4.1/weni/internal/migrations/0002_project.py
+-rw-r--r--   0        0        0        0 2023-05-18 01:33:52.643371 weni_rp_apps-2.4.1/weni/internal/migrations/__init__.py
+-rw-r--r--   0        0        0      963 2023-05-18 01:33:52.643371 weni_rp_apps-2.4.1/weni/internal/models.py
+-rw-r--r--   0        0        0        0 2023-05-18 01:33:52.643371 weni_rp_apps-2.4.1/weni/internal/orgs/__init__.py
+-rw-r--r--   0        0        0     3816 2023-05-18 01:33:52.643371 weni_rp_apps-2.4.1/weni/internal/orgs/serializers.py
+-rw-r--r--   0        0        0    14533 2023-05-18 01:33:52.643371 weni_rp_apps-2.4.1/weni/internal/orgs/tests.py
+-rw-r--r--   0        0        0      300 2023-05-18 01:33:52.643371 weni_rp_apps-2.4.1/weni/internal/orgs/urls.py
+-rw-r--r--   0        0        0     4579 2023-05-18 01:33:52.643371 weni_rp_apps-2.4.1/weni/internal/orgs/views.py
+-rw-r--r--   0        0        0      246 2023-05-18 01:33:52.643371 weni_rp_apps-2.4.1/weni/internal/permissions.py
+-rw-r--r--   0        0        0     1993 2023-05-18 01:33:52.643371 weni_rp_apps-2.4.1/weni/internal/statistic/tests.py
+-rw-r--r--   0        0        0      205 2023-05-18 01:33:52.643371 weni_rp_apps-2.4.1/weni/internal/statistic/urls.py
+-rw-r--r--   0        0        0      928 2023-05-18 01:33:52.643371 weni_rp_apps-2.4.1/weni/internal/statistic/views.py
+-rw-r--r--   0        0        0        0 2023-05-18 01:33:52.643371 weni_rp_apps-2.4.1/weni/internal/tests/__init__.py
+-rw-r--r--   0        0        0     1249 2023-05-18 01:33:52.643371 weni_rp_apps-2.4.1/weni/internal/tests/test_models.py
+-rw-r--r--   0        0        0        0 2023-05-18 01:33:52.643371 weni_rp_apps-2.4.1/weni/internal/tickets/__init__.py
+-rw-r--r--   0        0        0     1152 2023-05-18 01:33:52.643371 weni_rp_apps-2.4.1/weni/internal/tickets/serializers.py
+-rw-r--r--   0        0        0        0 2023-05-18 01:33:52.643371 weni_rp_apps-2.4.1/weni/internal/tickets/tests/__init__.py
+-rw-r--r--   0        0        0     3398 2023-05-18 01:33:52.643371 weni_rp_apps-2.4.1/weni/internal/tickets/tests/test_views.py
+-rw-r--r--   0        0        0      443 2023-05-18 01:33:52.643371 weni_rp_apps-2.4.1/weni/internal/tickets/urls.py
+-rw-r--r--   0        0        0     1861 2023-05-18 01:33:52.643371 weni_rp_apps-2.4.1/weni/internal/tickets/views.py
+-rw-r--r--   0        0        0     1315 2023-05-18 01:33:52.643371 weni_rp_apps-2.4.1/weni/internal/urls.py
+-rw-r--r--   0        0        0        0 2023-05-18 01:33:52.643371 weni_rp_apps-2.4.1/weni/internal/users/__init__.py
+-rw-r--r--   0        0        0      845 2023-05-18 01:33:52.643371 weni_rp_apps-2.4.1/weni/internal/users/serializers.py
+-rw-r--r--   0        0        0    11864 2023-05-18 01:33:52.643371 weni_rp_apps-2.4.1/weni/internal/users/tests.py
+-rw-r--r--   0        0        0      711 2023-05-18 01:33:52.643371 weni_rp_apps-2.4.1/weni/internal/users/urls.py
+-rw-r--r--   0        0        0     5758 2023-05-18 01:33:52.643371 weni_rp_apps-2.4.1/weni/internal/users/views.py
+-rw-r--r--   0        0        0      555 2023-05-18 01:33:52.643371 weni_rp_apps-2.4.1/weni/internal/views.py
+-rw-r--r--   0        0        0       55 2023-05-18 01:33:52.643371 weni_rp_apps-2.4.1/weni/orgs_api/__init__.py
+-rw-r--r--   0        0        0      253 2023-05-18 01:33:52.643371 weni_rp_apps-2.4.1/weni/orgs_api/apps.py
+-rw-r--r--   0        0        0      906 2023-05-18 01:33:52.643371 weni_rp_apps-2.4.1/weni/orgs_api/serializers.py
+-rw-r--r--   0        0        0     4030 2023-05-18 01:33:52.643371 weni_rp_apps-2.4.1/weni/orgs_api/tests.py
+-rw-r--r--   0        0        0      178 2023-05-18 01:33:52.643371 weni_rp_apps-2.4.1/weni/orgs_api/urls.py
+-rw-r--r--   0        0        0     1444 2023-05-18 01:33:52.643371 weni_rp_apps-2.4.1/weni/orgs_api/views.py
+-rw-r--r--   0        0        0       45 2023-05-18 01:33:52.643371 weni_rp_apps-2.4.1/weni/s3/__init__.py
+-rw-r--r--   0        0        0      243 2023-05-18 01:33:52.643371 weni_rp_apps-2.4.1/weni/s3/apps.py
+-rw-r--r--   0        0        0      250 2023-05-18 01:33:52.643371 weni_rp_apps-2.4.1/weni/s3/urls.py
+-rw-r--r--   0        0        0      550 2023-05-18 01:33:52.643371 weni_rp_apps-2.4.1/weni/s3/views.py
+-rw-r--r--   0        0        0       79 2023-05-18 01:33:52.643371 weni_rp_apps-2.4.1/weni/serializers/__init__.py
+-rw-r--r--   0        0        0      725 2023-05-18 01:33:52.643371 weni_rp_apps-2.4.1/weni/serializers/fields.py
+-rw-r--r--   0        0        0      281 2023-05-18 01:33:52.643371 weni_rp_apps-2.4.1/weni/success_orgs/apps.py
+-rw-r--r--   0        0        0     2403 2023-05-18 01:33:52.643371 weni_rp_apps-2.4.1/weni/success_orgs/business.py
+-rw-r--r--   0        0        0      563 2023-05-18 01:33:52.643371 weni_rp_apps-2.4.1/weni/success_orgs/serializers.py
+-rw-r--r--   0        0        0        0 2023-05-18 01:33:52.647371 weni_rp_apps-2.4.1/weni/success_orgs/tests/__init__.py
+-rw-r--r--   0        0        0     2980 2023-05-18 01:33:52.647371 weni_rp_apps-2.4.1/weni/success_orgs/tests/test_business.py
+-rw-r--r--   0        0        0      494 2023-05-18 01:33:52.647371 weni_rp_apps-2.4.1/weni/success_orgs/urls.py
+-rw-r--r--   0        0        0     2774 2023-05-18 01:33:52.647371 weni_rp_apps-2.4.1/weni/success_orgs/views.py
+-rw-r--r--   0        0        0      318 2023-05-18 01:33:52.647371 weni_rp_apps-2.4.1/weni/template_message/README.md
+-rw-r--r--   0        0        0       72 2023-05-18 01:33:52.647371 weni_rp_apps-2.4.1/weni/template_message/__init__.py
+-rw-r--r--   0        0        0      294 2023-05-18 01:33:52.647371 weni_rp_apps-2.4.1/weni/template_message/apps.py
+-rw-r--r--   0        0        0     2041 2023-05-18 01:33:52.647371 weni_rp_apps-2.4.1/weni/template_message/serializers.py
+-rw-r--r--   0        0        0     5295 2023-05-18 01:33:52.647371 weni_rp_apps-2.4.1/weni/template_message/tests.py
+-rw-r--r--   0        0        0      344 2023-05-18 01:33:52.647371 weni_rp_apps-2.4.1/weni/template_message/urls.py
+-rw-r--r--   0        0        0     1651 2023-05-18 01:33:52.647371 weni_rp_apps-2.4.1/weni/template_message/views.py
+-rw-r--r--   0        0        0        0 2023-05-18 01:33:52.647371 weni_rp_apps-2.4.1/weni/templates/__init__.py
+-rw-r--r--   0        0        0      559 2023-05-18 01:33:52.647371 weni_rp_apps-2.4.1/weni/templates/context_processors.py
+-rw-r--r--   0        0        0      315 2023-05-18 01:33:52.647371 weni_rp_apps-2.4.1/weni/ticketer_queues/README.md
+-rw-r--r--   0        0        0       70 2023-05-18 01:33:52.647371 weni_rp_apps-2.4.1/weni/ticketer_queues/__init__.py
+-rw-r--r--   0        0        0      291 2023-05-18 01:33:52.647371 weni_rp_apps-2.4.1/weni/ticketer_queues/apps.py
+-rw-r--r--   0        0        0      242 2023-05-18 01:33:52.647371 weni_rp_apps-2.4.1/weni/ticketer_queues/serializers.py
+-rw-r--r--   0        0        0     1584 2023-05-18 01:33:52.647371 weni_rp_apps-2.4.1/weni/ticketer_queues/tests.py
+-rw-r--r--   0        0        0      378 2023-05-18 01:33:52.647371 weni_rp_apps-2.4.1/weni/ticketer_queues/urls.py
+-rw-r--r--   0        0        0      849 2023-05-18 01:33:52.647371 weni_rp_apps-2.4.1/weni/ticketer_queues/views.py
+-rw-r--r--   0        0        0        0 2023-05-18 01:33:52.647371 weni_rp_apps-2.4.1/weni/utils/__init__.py
+-rw-r--r--   0        0        0     1091 2023-05-18 01:33:52.647371 weni_rp_apps-2.4.1/weni/utils/app_config.py
+-rw-r--r--   0        0        0     1001 1970-01-01 00:00:00.000000 weni_rp_apps-2.4.1/PKG-INFO
```

### Comparing `weni_rp_apps-2.4.0a9/pyproject.toml` & `weni_rp_apps-2.4.1/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "weni-rp-apps"
-version = "2.4.0a9"
+version = "2.4.1"
 description = "Weni apps for Rapidpro Platform"
 authors = ["jcbalmeida"]
 license = "AGPL-3.0"
 packages = [
     { include = "weni" }
 ]
```

### Comparing `weni_rp_apps-2.4.0a9/weni/activities/signals.py` & `weni_rp_apps-2.4.1/weni/activities/signals.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.4.0a9/weni/analytics_api/tests.py` & `weni_rp_apps-2.4.1/weni/analytics_api/tests.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.4.0a9/weni/analytics_api/views.py` & `weni_rp_apps-2.4.1/weni/analytics_api/views.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.4.0a9/weni/auth/backends.py` & `weni_rp_apps-2.4.1/weni/auth/backends.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,10 @@
 import logging
 
-import pytz
-from django.conf import settings
-
 from mozilla_django_oidc.auth import OIDCAuthenticationBackend
-from temba.orgs.models import Org
 
 LOGGER = logging.getLogger("weni_django_oidc")
 
 
 class WeniOIDCAuthenticationBackend(OIDCAuthenticationBackend):
     def verify_claims(self, claims):
         # validação de permissão
```

### Comparing `weni_rp_apps-2.4.0a9/weni/auth/urls.py` & `weni_rp_apps-2.4.1/weni/auth/urls.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.4.0a9/weni/auth/views.py` & `weni_rp_apps-2.4.1/weni/auth/views.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.4.0a9/weni/channel_stats/serializers.py` & `weni_rp_apps-2.4.1/weni/channel_stats/serializers.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.4.0a9/weni/channel_stats/views.py` & `weni_rp_apps-2.4.1/weni/channel_stats/views.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.4.0a9/weni/grpc/billing/queries.py` & `weni_rp_apps-2.4.1/weni/grpc/billing/queries.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.4.0a9/weni/grpc/billing/serializers.py` & `weni_rp_apps-2.4.1/weni/grpc/billing/serializers.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.4.0a9/weni/grpc/billing/services.py` & `weni_rp_apps-2.4.1/weni/grpc/billing/services.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.4.0a9/weni/grpc/billing/tests.py` & `weni_rp_apps-2.4.1/weni/grpc/billing/tests.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.4.0a9/weni/grpc/channel/serializers.py` & `weni_rp_apps-2.4.1/weni/grpc/channel/serializers.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.4.0a9/weni/grpc/channel/services.py` & `weni_rp_apps-2.4.1/weni/grpc/channel/services.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.4.0a9/weni/grpc/channel/tests.py` & `weni_rp_apps-2.4.1/weni/grpc/channel/tests.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.4.0a9/weni/grpc/classifier/serializers.py` & `weni_rp_apps-2.4.1/weni/grpc/classifier/serializers.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.4.0a9/weni/grpc/classifier/services.py` & `weni_rp_apps-2.4.1/weni/grpc/classifier/services.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.4.0a9/weni/grpc/classifier/tests.py` & `weni_rp_apps-2.4.1/weni/grpc/classifier/tests.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.4.0a9/weni/grpc/core/management/commands/grpc.py` & `weni_rp_apps-2.4.1/weni/grpc/core/management/commands/grpc.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.4.0a9/weni/grpc/core/serializers.py` & `weni_rp_apps-2.4.1/weni/grpc/core/serializers.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.4.0a9/weni/grpc/core/services.py` & `weni_rp_apps-2.4.1/weni/grpc/core/services.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.4.0a9/weni/grpc/core/urls.py` & `weni_rp_apps-2.4.1/weni/grpc/core/urls.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.4.0a9/weni/grpc/flow/services.py` & `weni_rp_apps-2.4.1/weni/grpc/flow/services.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.4.0a9/weni/grpc/flow/tests.py` & `weni_rp_apps-2.4.1/weni/grpc/flow/tests.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.4.0a9/weni/grpc/org/serializers.py` & `weni_rp_apps-2.4.1/weni/grpc/org/serializers.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.4.0a9/weni/grpc/org/services.py` & `weni_rp_apps-2.4.1/weni/grpc/org/services.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.4.0a9/weni/grpc/org/tests.py` & `weni_rp_apps-2.4.1/weni/grpc/org/tests.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.4.0a9/weni/grpc/statistic/services.py` & `weni_rp_apps-2.4.1/weni/grpc/statistic/services.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.4.0a9/weni/grpc/statistic/tests.py` & `weni_rp_apps-2.4.1/weni/grpc/statistic/tests.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.4.0a9/weni/grpc/user/serializers.py` & `weni_rp_apps-2.4.1/weni/grpc/user/serializers.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.4.0a9/weni/grpc/user/services.py` & `weni_rp_apps-2.4.1/weni/grpc/user/services.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.4.0a9/weni/grpc/user/tests.py` & `weni_rp_apps-2.4.1/weni/grpc/user/tests.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.4.0a9/weni/internal/backends.py` & `weni_rp_apps-2.4.1/weni/internal/backends.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.4.0a9/weni/internal/channel/serializers.py` & `weni_rp_apps-2.4.1/weni/internal/channel/serializers.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.4.0a9/weni/internal/channel/tests.py` & `weni_rp_apps-2.4.1/weni/internal/channel/tests.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.4.0a9/weni/internal/channel/views.py` & `weni_rp_apps-2.4.1/weni/internal/channel/views.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,23 +4,26 @@
 from django.shortcuts import get_object_or_404
 from django.http import JsonResponse
 
 from rest_framework.response import Response
 from rest_framework.decorators import action
 from rest_framework import viewsets
 from rest_framework import status
-from rest_framework.pagination import PageNumberPagination
 
 from weni.internal.views import InternalGenericViewSet
 from django.conf import settings
 
 from temba.channels.models import Channel
 from temba.channels.types import TYPES
 
-from .serializers import ChannelSerializer, CreateChannelSerializer, ChannelWACSerializer
+from .serializers import (
+    ChannelSerializer,
+    CreateChannelSerializer,
+    ChannelWACSerializer,
+)
 
 User = get_user_model()
 
 
 class ChannelEndpoint(viewsets.ModelViewSet, InternalGenericViewSet):
     serializer_class = ChannelSerializer
     lookup_field = "uuid"
@@ -40,21 +43,25 @@
 
     def retrieve(self, request, uuid=None):
         try:
             channel = Channel.objects.get(uuid=uuid)
         except Channel.DoesNotExist:
             return Response(status=status.HTTP_404_NOT_FOUND)
 
-        return JsonResponse(data=self.get_serializer(channel).data, status=status.HTTP_200_OK)
+        return JsonResponse(
+            data=self.get_serializer(channel).data, status=status.HTTP_200_OK
+        )
 
     def create(self, request):
         serializer = CreateChannelSerializer(data=request.data)
 
         if not serializer.is_valid():
-            return JsonResponse(data=serializer.errors, status=status.HTTP_400_BAD_REQUEST)
+            return JsonResponse(
+                data=serializer.errors, status=status.HTTP_400_BAD_REQUEST
+            )
 
         serializer.save()
 
         return JsonResponse(data=serializer.data, status=status.HTTP_200_OK)
 
     def destroy(self, request, uuid=None):
         channel = get_object_or_404(Channel, uuid=uuid)
@@ -65,15 +72,17 @@
         return Response(status=status.HTTP_200_OK)
 
     @action(methods=["POST"], detail=False)
     def create_wac(self, request):
         serializer = ChannelWACSerializer(data=request.data)
 
         if not serializer.is_valid():
-            return JsonResponse(data=serializer.errors, status=status.HTTP_400_BAD_REQUEST)
+            return JsonResponse(
+                data=serializer.errors, status=status.HTTP_400_BAD_REQUEST
+            )
 
         serializer.save()
 
         return JsonResponse(data=serializer.data, status=status.HTTP_200_OK)
 
 
 class AvailableChannels(viewsets.ViewSet, InternalGenericViewSet):
@@ -94,15 +103,15 @@
             "channel_types": channel_types,
         }
         return Response(payload)
 
     def retrieve(self, request, pk=None):
         channel_type = None
         fields_form = {}
-        code_type =  pk
+        code_type = pk
         current_form = None
         if code_type:
             channel_type = TYPES.get(code_type.upper(), None)
 
         if channel_type is None:
             return Response(status=status.HTTP_404_NOT_FOUND)
 
@@ -126,85 +135,109 @@
             fields_types = {}
             attibutes_type = extract_type_info(channel_type)
             if not (attibutes_type):
                 return Response(status=status.HTTP_404_NOT_FOUND)
 
             fields_types["attributes"] = attibutes_type
 
-        payload = {"attributes": fields_types.get("attributes"), "form": fields_form.get("form")}
+        payload = {
+            "attributes": fields_types.get("attributes"),
+            "form": fields_form.get("form"),
+        }
 
         return Response(payload)
 
 
 def extract_type_info(_class):
     channel = {}
     type_exclude = ["<class 'function'>"]
-    items_exclude = ["redact_response_keys", "claim_view_kwargs", "extra_links", "redact_request_keys"]
+    items_exclude = [
+        "redact_response_keys",
+        "claim_view_kwargs",
+        "extra_links",
+        "redact_request_keys",
+    ]
 
     for i in _class.__class__.__dict__.items():
         if not i[0].startswith("_"):
-            if not inspect.isclass(i[1]) and str(type(i[1])) not in (type_exclude) and i[0] not in items_exclude:
+            if (
+                not inspect.isclass(i[1])
+                and str(type(i[1])) not in (type_exclude)
+                and i[0] not in items_exclude
+            ):
                 if str(type(i[1])) == "<enum 'Category'>":
-                    channel[i[0]] = {"name": i[1].name if i[1].name else "", "value": i[1].value if i[1].value else ""}
+                    channel[i[0]] = {
+                        "name": i[1].name if i[1].name else "",
+                        "value": i[1].value if i[1].value else "",
+                    }
 
                 elif i[0] == "configuration_urls":
                     if i[1]:
                         if i[1][0]:
                             urls_list = []
                             url_dict = {}
                             for url in i[1]:
                                 if url.get("label"):
                                     url_dict["label"] = str(url.get("label"))
 
                                 if i[1][0].get("url"):
                                     url_dict["url"] = str(url.get("url"))
 
                                 if i[1][0].get("description"):
-                                    url_dict["description"] = str(url.get("description"))
+                                    url_dict["description"] = str(
+                                        url.get("description")
+                                    )
 
                             urls_list.append(url_dict)
                             channel[i[0]] = urls_list
 
                 elif i[0] == "configuration_blurb":
                     channel[i[0]] = str(i[1])
 
                 elif i[0] == "claim_blurb":
                     channel[i[0]] = str(i[1])
 
                 elif (i[0]) == "ivr_protocol":
-                    channel[i[0]] = {"name": i[1].name if i[1].name else "", "value": i[1].value if i[1].value else ""}
+                    channel[i[0]] = {
+                        "name": i[1].name if i[1].name else "",
+                        "value": i[1].value if i[1].value else "",
+                    }
                 else:
                     channel[i[0]] = i[1]
 
-    if (not (channel.get("code"))) or (not (len(channel)) > 0) or (not (channel.get("name"))):
+    if (
+        (not (channel.get("code")))
+        or (not (len(channel)) > 0)
+        or (not (channel.get("name")))
+    ):
         return None
 
     channel["num_fields"] = len(channel)
     return channel
 
 
 def extract_form_info(_form, name_form):
     detail = {}
     detail["name"] = name_form if name_form else None
 
     try:
-        detail['type'] = str(_form.widget.input_type)
+        detail["type"] = str(_form.widget.input_type)
     except AttributeError:
-        detail['type'] = str(_form.widget.__class__.__name__).lower()
+        detail["type"] = str(_form.widget.__class__.__name__).lower()
 
     if _form.help_text:
         detail["help_text"] = str(_form.help_text)
     else:
-        detail['help_text'] = ''
+        detail["help_text"] = ""
 
     if detail.get("type") == "select":
         detail["choices"] = _form.choices
 
     if _form.label:
         detail["label"] = str(_form.label)
     else:
-        detail['label'] = ''
+        detail["label"] = ""
 
     if not (detail.get("name")) or not (detail.get("type")):
         return None
 
-    return detail
+    return detail
```

### Comparing `weni_rp_apps-2.4.0a9/weni/internal/classifier/serializers.py` & `weni_rp_apps-2.4.1/weni/internal/classifier/serializers.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.4.0a9/weni/internal/classifier/tests.py` & `weni_rp_apps-2.4.1/weni/internal/classifier/tests.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.4.0a9/weni/internal/classifier/views.py` & `weni_rp_apps-2.4.1/weni/internal/classifier/views.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.4.0a9/weni/internal/clients/authenticators.py` & `weni_rp_apps-2.4.1/weni/internal/clients/authenticators.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.4.0a9/weni/internal/clients/connect.py` & `weni_rp_apps-2.4.1/weni/internal/clients/connect.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.4.0a9/weni/internal/externals/serializers.py` & `weni_rp_apps-2.4.1/weni/internal/externals/serializers.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.4.0a9/weni/internal/externals/views.py` & `weni_rp_apps-2.4.1/weni/internal/externals/views.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.4.0a9/weni/internal/flows/serializers.py` & `weni_rp_apps-2.4.1/weni/internal/flows/serializers.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.4.0a9/weni/internal/flows/tests.py` & `weni_rp_apps-2.4.1/weni/internal/flows/tests.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.4.0a9/weni/internal/flows/views.py` & `weni_rp_apps-2.4.1/weni/internal/flows/views.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.4.0a9/weni/internal/globals/serializers.py` & `weni_rp_apps-2.4.1/weni/internal/globals/serializers.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.4.0a9/weni/internal/globals/tests/test_serializers.py` & `weni_rp_apps-2.4.1/weni/internal/globals/tests/test_serializers.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.4.0a9/weni/internal/globals/views.py` & `weni_rp_apps-2.4.1/weni/internal/globals/views.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.4.0a9/weni/internal/migrations/0001_initial.py` & `weni_rp_apps-2.4.1/weni/internal/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.4.0a9/weni/internal/migrations/0002_project.py` & `weni_rp_apps-2.4.1/weni/internal/migrations/0002_project.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.4.0a9/weni/internal/models.py` & `weni_rp_apps-2.4.1/weni/internal/models.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,23 +3,32 @@
 from django.db import models
 
 from temba.tickets.models import Ticketer, Topic
 from temba.orgs.models import Org
 
 
 class TicketerQueue(Topic):
-    topic = models.OneToOneField(Topic, on_delete=models.CASCADE, parent_link=True, related_name="queue")
-    ticketer = models.ForeignKey(Ticketer, on_delete=models.CASCADE, related_name="queues")
+    topic = models.OneToOneField(
+        Topic, on_delete=models.CASCADE, parent_link=True, related_name="queue"
+    )
+    ticketer = models.ForeignKey(
+        Ticketer, on_delete=models.CASCADE, related_name="queues"
+    )
 
     class Meta:
         db_table = "internal_tickets_ticketerqueue"
 
     def __str__(self):
         return f"Queue[uuid={self.uuid}, name={self.name}]"
 
+    def release(self, user):
+        self.ticketer.release(user=user)
+        self.is_active = False
+        self.save()
+
 
 class Project(Org):
     project_uuid = models.UUIDField(default=uuid4, unique=True)
 
     class Meta:
         db_table = "internal_project"
```

### Comparing `weni_rp_apps-2.4.0a9/weni/internal/orgs/serializers.py` & `weni_rp_apps-2.4.1/weni/internal/orgs/serializers.py`

 * *Files 0% similar despite different names*

```diff
@@ -37,14 +37,15 @@
         return ret
 
     def create(self, validated_data):
         validated_data["plan"] = "infinity"
         validated_data["project_uuid"] = validated_data.pop("uuid")
 
         project = super().create(validated_data)
+
         project.administrators.add(validated_data.get("created_by"))
         project.initialize(sample_flows=False)
 
         return project
 
 
 class OrgSerializer(serializers.ModelSerializer):
```

### Comparing `weni_rp_apps-2.4.0a9/weni/internal/orgs/tests.py` & `weni_rp_apps-2.4.1/weni/internal/orgs/tests.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.4.0a9/weni/internal/orgs/views.py` & `weni_rp_apps-2.4.1/weni/internal/orgs/views.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.4.0a9/weni/internal/statistic/tests.py` & `weni_rp_apps-2.4.1/weni/internal/statistic/tests.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.4.0a9/weni/internal/statistic/views.py` & `weni_rp_apps-2.4.1/weni/internal/statistic/views.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 from django.shortcuts import get_object_or_404
 
 from rest_framework.response import Response
 from rest_framework.mixins import RetrieveModelMixin
 from rest_framework import status
 
 from temba.orgs.models import Org
+from temba.contacts.models import ContactGroup
 
 from weni.internal.views import InternalGenericViewSet
 
 
 class StatisticEndpoint(RetrieveModelMixin, InternalGenericViewSet):
     lookup_field = "uuid"
 
     def retrieve(self, request, uuid=None):
         org = get_object_or_404(Org, uuid=uuid)
+        group = ContactGroup.all_groups.get(org=org, group_type='A')
 
         response = {
             "active_flows": org.flows.filter(is_active=True, is_archived=False).exclude(is_system=True).count(),
             "active_classifiers": org.classifiers.filter(is_active=True).count(),
-            "active_contacts": org.contacts.filter(is_active=True).count(),
+            "active_contacts": group.get_member_count(),
         }
 
         return Response(data=response, status=status.HTTP_200_OK)
```

### Comparing `weni_rp_apps-2.4.0a9/weni/internal/tests/test_models.py` & `weni_rp_apps-2.4.1/weni/internal/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.4.0a9/weni/internal/tickets/serializers.py` & `weni_rp_apps-2.4.1/weni/internal/tickets/serializers.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.4.0a9/weni/internal/tickets/tests/test_views.py` & `weni_rp_apps-2.4.1/weni/internal/tickets/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.4.0a9/weni/internal/tickets/views.py` & `weni_rp_apps-2.4.1/weni/internal/tickets/views.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,41 +1,52 @@
 from rest_framework import mixins
 from rest_framework.generics import get_object_or_404
 
 from temba.tickets.models import Ticketer
 from weni.internal.views import InternalGenericViewSet
 from weni.internal.models import TicketerQueue
-from weni.internal.tickets.serializers import TicketerSerializer, TicketerQueueSerializer
+from weni.internal.tickets.serializers import (
+    TicketerSerializer,
+    TicketerQueueSerializer,
+)
 
 
 class TicketerViewSet(
-    mixins.CreateModelMixin, mixins.UpdateModelMixin, mixins.DestroyModelMixin, InternalGenericViewSet
+    mixins.CreateModelMixin,
+    mixins.UpdateModelMixin,
+    mixins.DestroyModelMixin,
+    InternalGenericViewSet,
 ):
     serializer_class = TicketerSerializer
     queryset = Ticketer.objects.filter(is_active=True)
     lookup_field = "uuid"
 
     def perform_destroy(self, instance):
         instance.release(self.request.user)
 
 
 class TicketerQueueViewSet(
-    mixins.CreateModelMixin, mixins.UpdateModelMixin, mixins.DestroyModelMixin, InternalGenericViewSet
+    mixins.CreateModelMixin,
+    mixins.UpdateModelMixin,
+    mixins.DestroyModelMixin,
+    InternalGenericViewSet,
 ):
     serializer_class = TicketerQueueSerializer
     queryset = TicketerQueue.objects
     lookup_field = "uuid"
 
     @property
     def _ticketer(self):
         sector_uuid = self.kwargs.get("ticketer_uuid")
-        return get_object_or_404(Ticketer, config__sector_uuid=sector_uuid)
+        return get_object_or_404(
+            Ticketer, is_active=True, config__sector_uuid=sector_uuid
+        )
 
     def get_queryset(self):
-        return super().get_queryset().filter(ticketer=self._ticketer)
+        return super().get_queryset().filter(is_active=True, ticketer=self._ticketer)
 
     def perform_create(self, serializer):
         ticketer = self._ticketer
 
         serializer.save(
             ticketer=ticketer,
             org=ticketer.org,
@@ -47,11 +58,8 @@
         partial = kwargs.get("partial", False)
         if not partial:
             self.http_method_not_allowed(request, *args, **kwargs)
 
         return super().update(request, *args, **kwargs)
 
     def perform_destroy(self, instance):
-        ticketer = instance.ticketer
-        # Release Ticketer
-        ticketer.release(self.request.user)
-        instance.delete()
+        instance.release(self.request.user)
```

### Comparing `weni_rp_apps-2.4.0a9/weni/internal/urls.py` & `weni_rp_apps-2.4.1/weni/internal/urls.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.4.0a9/weni/internal/users/serializers.py` & `weni_rp_apps-2.4.1/weni/internal/users/serializers.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.4.0a9/weni/internal/users/tests.py` & `weni_rp_apps-2.4.1/weni/internal/users/tests.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.4.0a9/weni/internal/users/urls.py` & `weni_rp_apps-2.4.1/weni/internal/users/urls.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.4.0a9/weni/internal/users/views.py` & `weni_rp_apps-2.4.1/weni/internal/users/views.py`

 * *Files 18% similar despite different names*

```diff
@@ -8,166 +8,150 @@
 from rest_framework.decorators import action
 from rest_framework.response import Response
 from rest_framework import exceptions
 from rest_framework import mixins
 from rest_framework.exceptions import ValidationError
 
 from weni.internal.views import InternalGenericViewSet
-from weni.internal.users.serializers import (
-    UserAPITokenSerializer,
-    UserSerializer,
-    UserPermissionSerializer,
-)
+from weni.internal.users.serializers import UserAPITokenSerializer, UserSerializer, UserPermissionSerializer
 from temba.api.models import APIToken
 from temba.orgs.models import Org
 from weni.internal.models import Project
 
 
 if TYPE_CHECKING:
     from rest_framework.request import Request
 
 User = get_user_model()
 
 
 class UserViewSet(InternalGenericViewSet):
-    @action(
-        detail=False,
-        methods=["GET"],
-        url_path="api-token",
-        serializer_class=UserAPITokenSerializer,
-    )
+    @action(detail=False, methods=["GET"], url_path="api-token", serializer_class=UserAPITokenSerializer)
     def api_token(self, request: "Request", **kwargs):
         serializer = self.get_serializer(data=request.query_params)
         serializer.is_valid(raise_exception=True)
         user = serializer.validated_data.get("user")
         project = serializer.validated_data.get("project")
 
         try:
             api_token = APIToken.objects.get(user=user, org=project.org)
         except APIToken.DoesNotExist:
             raise exceptions.PermissionDenied()
 
         return Response(
-            dict(
-                user=api_token.user.email,
-                org=api_token.org.uuid,
-                api_token=api_token.key,
-            )
+            dict(user=api_token.user.email, project=project.project_uuid, api_token=api_token.key)
         )
 
 
 class UserPermissionEndpoint(InternalGenericViewSet):
     serializer_class = UserPermissionSerializer
 
     def retrieve(self, request):
         org = get_object_or_404(Org, uuid=request.query_params.get("org_uuid"))
         user = get_object_or_404(
             User,
             email=request.query_params.get("user_email"),
             is_active=request.query_params.get("is_active", True),
         )
 
-        permissions = self._get_user_permissions(project, user)
+        permissions = self._get_user_permissions(org, user)
         serializer = self.get_serializer(permissions)
 
         return Response(serializer.data)
 
     def partial_update(self, request):
         org = get_object_or_404(Org, uuid=request.data.get("org_uuid"))
         user, created = User.objects.get_or_create(
             email=request.data.get("user_email"),
             defaults={"username": request.data.get("user_email")},
             is_active=request.query_params.get("is_active", True),
         )
 
-        self._validate_permission(project, request.data.get("permission", ""))
-        self._set_user_permission(project, user, request.data.get("permission", ""))
+        self._validate_permission(org, request.data.get("permission", ""))
+        self._set_user_permission(org, user, request.data.get("permission", ""))
 
-        permissions = self._get_user_permissions(project, user)
+        permissions = self._get_user_permissions(org, user)
         serializer = self.get_serializer(permissions)
 
         return Response(serializer.data)
 
     def destroy(self, request):
         org = get_object_or_404(Org, uuid=request.data.get("org_uuid"))
         user = get_object_or_404(
             User,
             email=request.data.get("user_email"),
             is_active=request.query_params.get("is_active", True),
         )
 
-        self._validate_permission(project, request.data.get("permission", ""))
-        self._remove_user_permission(project, user, request.data.get("permission", ""))
+        self._validate_permission(org, request.data.get("permission", ""))
+        self._remove_user_permission(org, user, request.data.get("permission", ""))
 
-        permissions = self._get_user_permissions(project, user)
+        permissions = self._get_user_permissions(org, user)
         serializer = self.get_serializer(permissions)
 
         return Response(serializer.data)
 
-    def _remove_user_permission(self, project: Project, user: User, permission: str):
-        permissions = self._get_permissions(project)
+    def _remove_user_permission(self, org: Org, user: User, permission: str):
+        permissions = self._get_permissions(org)
         permissions.get(permission).remove(user)
 
-    def _set_user_permission(self, project: Project, user: User, permission: str):
-        permissions = self._get_permissions(project)
+    def _set_user_permission(self, org: Org, user: User, permission: str):
+        permissions = self._get_permissions(org)
 
-        for perm_name, project_field in permissions.items():
+        for perm_name, org_field in permissions.items():
             if not perm_name == permission:
-                project_field.remove(user)
+                org_field.remove(user)
 
         permissions.get(permission).add(user)
 
     def _validate_permission(self, org: Org, permission: str):
         permissions_keys = self._get_permissions(org).keys()
         if permission not in permissions_keys:
             raise ValidationError(detail=f"{permission} is not a valid permission!")
 
-    def _get_permissions(self, project: Project) -> dict:
+    def _get_permissions(self, org: Org) -> dict:
         return {
-            "administrator": project.administrators,
-            "viewer": project.viewers,
-            "editor": project.editors,
-            "surveyor": project.surveyors,
-            "agent": project.agents,
+            "administrator": org.administrators,
+            "viewer": org.viewers,
+            "editor": org.editors,
+            "surveyor": org.surveyors,
+            "agent": org.agents,
         }
 
-    def _get_user_permissions(self, project: Project, user: User) -> dict:
+    def _get_user_permissions(self, org: Org, user: User) -> dict:
         permissions = {}
-        project_permissions = self._get_permissions(project)
+        org_permissions = self._get_permissions(org)
 
-        for perm_name, project_field in project_permissions.items():
-            if project_field.filter(pk=user.id).exists():
+        for perm_name, org_field in org_permissions.items():
+            if org_field.filter(pk=user.id).exists():
                 permissions[perm_name] = True
 
         return permissions
 
 
 class UserEndpoint(InternalGenericViewSet, mixins.RetrieveModelMixin):
     serializer_class = UserSerializer
     queryset = User.objects.all()
     lookup_field = "uuid"
 
     def partial_update(self, request):
         instance = get_object_or_404(User, email=request.query_params.get("email"))
 
-        if request.data.get("language") not in [
-            language[0] for language in settings.LANGUAGES
-        ]:
+        if request.data.get("language") not in [language[0] for language in settings.LANGUAGES]:
             raise ValidationError("Invalid argument: language")
 
         user_settings = instance.get_settings()
         user_settings.language = request.data.get("language")
         user_settings.save()
 
         return Response(status=status.HTTP_200_OK)
 
     def retrieve(self, request):
         if not request.query_params.get("email"):
             raise ValidationError(detail="empty email")
 
         user = User.objects.get_or_create(
-            email=request.query_params.get("email"),
-            defaults={"username": request.query_params.get("email")},
+            email=request.query_params.get("email"), defaults={"username": request.query_params.get("email")}
         )
 
         serializer = self.get_serializer(user[0])
         return Response(serializer.data)
```

### Comparing `weni_rp_apps-2.4.0a9/weni/internal/views.py` & `weni_rp_apps-2.4.1/weni/internal/views.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.4.0a9/weni/orgs_api/serializers.py` & `weni_rp_apps-2.4.1/weni/orgs_api/serializers.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.4.0a9/weni/orgs_api/tests.py` & `weni_rp_apps-2.4.1/weni/orgs_api/tests.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.4.0a9/weni/orgs_api/views.py` & `weni_rp_apps-2.4.1/weni/orgs_api/views.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.4.0a9/weni/s3/views.py` & `weni_rp_apps-2.4.1/weni/s3/views.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.4.0a9/weni/serializers/fields.py` & `weni_rp_apps-2.4.1/weni/serializers/fields.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.4.0a9/weni/success_orgs/business.py` & `weni_rp_apps-2.4.1/weni/success_orgs/business.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.4.0a9/weni/success_orgs/serializers.py` & `weni_rp_apps-2.4.1/weni/success_orgs/serializers.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.4.0a9/weni/success_orgs/tests/test_business.py` & `weni_rp_apps-2.4.1/weni/success_orgs/tests/test_business.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.4.0a9/weni/success_orgs/views.py` & `weni_rp_apps-2.4.1/weni/success_orgs/views.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.4.0a9/weni/template_message/serializers.py` & `weni_rp_apps-2.4.1/weni/template_message/serializers.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.4.0a9/weni/template_message/tests.py` & `weni_rp_apps-2.4.1/weni/template_message/tests.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.4.0a9/weni/template_message/views.py` & `weni_rp_apps-2.4.1/weni/template_message/views.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.4.0a9/weni/templates/context_processors.py` & `weni_rp_apps-2.4.1/weni/templates/context_processors.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.4.0a9/weni/ticketer_queues/tests.py` & `weni_rp_apps-2.4.1/weni/ticketer_queues/tests.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.4.0a9/weni/ticketer_queues/views.py` & `weni_rp_apps-2.4.1/weni/ticketer_queues/views.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.4.0a9/weni/utils/app_config.py` & `weni_rp_apps-2.4.1/weni/utils/app_config.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.4.0a9/PKG-INFO` & `weni_rp_apps-2.4.1/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: weni-rp-apps
-Version: 2.4.0a9
+Version: 2.4.1
 Summary: Weni apps for Rapidpro Platform
 License: AGPL-3.0
 Author: jcbalmeida
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
```

