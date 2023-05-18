# Comparing `tmp/tap-mambu-3.1.5.tar.gz` & `tmp/tap-mambu-4.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tap-mambu-3.1.5.tar", last modified: Thu Oct 13 13:28:34 2022, max compression
+gzip compressed data, was "tap-mambu-4.0.0.tar", last modified: Thu Feb 23 16:00:39 2023, max compression
```

## Comparing `tap-mambu-3.1.5.tar` & `tap-mambu-4.0.0.tar`

### file list

```diff
@@ -1,155 +1,155 @@
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2022-10-13 13:28:34.546474 tap-mambu-3.1.5/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    34523 2022-08-12 17:24:47.000000 tap-mambu-3.1.5/LICENSE
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       57 2022-08-12 17:24:47.000000 tap-mambu-3.1.5/MANIFEST.in
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      332 2022-10-13 13:28:34.546474 tap-mambu-3.1.5/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    19218 2022-08-12 17:24:47.000000 tap-mambu-3.1.5/README.md
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2022-10-13 13:28:34.466473 tap-mambu-3.1.5/mambu_tests/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2022-08-12 17:24:47.000000 tap-mambu-3.1.5/mambu_tests/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      953 2022-09-27 17:20:33.000000 tap-mambu-3.1.5/mambu_tests/conftest.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      413 2022-09-27 17:20:33.000000 tap-mambu-3.1.5/mambu_tests/constants.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3873 2022-09-27 17:20:33.000000 tap-mambu-3.1.5/mambu_tests/helpers.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2022-10-13 13:28:34.470473 tap-mambu-3.1.5/mambu_tests/multithreading/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2022-08-12 17:24:47.000000 tap-mambu-3.1.5/mambu_tests/multithreading/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4418 2022-09-27 17:20:33.000000 tap-mambu-3.1.5/mambu_tests/multithreading/test_multithreaded_bookmark_daybyday_generator.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    13914 2022-09-27 17:20:33.000000 tap-mambu-3.1.5/mambu_tests/multithreading/test_multithreaded_bookmark_generator.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    16607 2022-08-12 17:24:47.000000 tap-mambu-3.1.5/mambu_tests/multithreading/test_multithreaded_offset_generator.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4660 2022-08-12 17:24:47.000000 tap-mambu-3.1.5/mambu_tests/multithreading/test_requests_pool.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2022-10-13 13:28:34.486474 tap-mambu-3.1.5/mambu_tests/tap_generators/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1541 2022-09-27 17:20:33.000000 tap-mambu-3.1.5/mambu_tests/tap_generators/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1604 2022-09-27 17:20:33.000000 tap-mambu-3.1.5/mambu_tests/tap_generators/test_activities_generator.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3245 2022-09-27 17:20:33.000000 tap-mambu-3.1.5/mambu_tests/tap_generators/test_audit_trail_generator.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      537 2022-08-12 17:24:47.000000 tap-mambu-3.1.5/mambu_tests/tap_generators/test_branches_generator.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      546 2022-08-12 17:24:47.000000 tap-mambu-3.1.5/mambu_tests/tap_generators/test_centres_generator.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      669 2022-09-27 17:20:33.000000 tap-mambu-3.1.5/mambu_tests/tap_generators/test_clients_generator.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      608 2022-08-12 17:24:47.000000 tap-mambu-3.1.5/mambu_tests/tap_generators/test_communications_generator.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      565 2022-08-12 17:24:47.000000 tap-mambu-3.1.5/mambu_tests/tap_generators/test_credit_arrangements_generator.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      338 2022-08-12 17:24:47.000000 tap-mambu-3.1.5/mambu_tests/tap_generators/test_custom_field_sets_generator.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      688 2022-09-12 19:44:32.000000 tap-mambu-3.1.5/mambu_tests/tap_generators/test_deposit_accounts_generator.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      376 2022-08-12 17:24:47.000000 tap-mambu-3.1.5/mambu_tests/tap_generators/test_deposit_cards_generator.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      403 2022-08-12 17:24:47.000000 tap-mambu-3.1.5/mambu_tests/tap_generators/test_deposit_products_generator.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      687 2022-09-27 17:20:33.000000 tap-mambu-3.1.5/mambu_tests/tap_generators/test_deposit_transactions_generator.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9335 2022-09-27 17:20:33.000000 tap-mambu-3.1.5/mambu_tests/tap_generators/test_generators.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      429 2022-08-12 17:24:47.000000 tap-mambu-3.1.5/mambu_tests/tap_generators/test_gl_accounts_generator.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1072 2022-08-12 17:24:47.000000 tap-mambu-3.1.5/mambu_tests/tap_generators/test_gl_journal_entries_generator.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      630 2022-09-27 17:20:33.000000 tap-mambu-3.1.5/mambu_tests/tap_generators/test_groups_generator.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      602 2022-08-12 17:24:47.000000 tap-mambu-3.1.5/mambu_tests/tap_generators/test_index_rate_sources_generator.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      630 2022-08-12 17:24:47.000000 tap-mambu-3.1.5/mambu_tests/tap_generators/test_installments_generator.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      676 2022-08-12 17:24:47.000000 tap-mambu-3.1.5/mambu_tests/tap_generators/test_interest_accrual_breakdown_generator.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1181 2022-09-27 17:20:33.000000 tap-mambu-3.1.5/mambu_tests/tap_generators/test_loan_accounts_generators.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      457 2022-08-12 17:24:47.000000 tap-mambu-3.1.5/mambu_tests/tap_generators/test_loan_products_generator.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      663 2022-09-27 17:20:33.000000 tap-mambu-3.1.5/mambu_tests/tap_generators/test_loan_transactions_generator.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1480 2022-08-12 17:24:47.000000 tap-mambu-3.1.5/mambu_tests/tap_generators/test_no_pagination_generators.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      374 2022-08-12 17:24:47.000000 tap-mambu-3.1.5/mambu_tests/tap_generators/test_repayments_generator.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      528 2022-08-12 17:24:47.000000 tap-mambu-3.1.5/mambu_tests/tap_generators/test_tasks_generator.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      514 2022-08-12 17:24:47.000000 tap-mambu-3.1.5/mambu_tests/tap_generators/test_users_generator.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2022-10-13 13:28:34.490474 tap-mambu-3.1.5/mambu_tests/tap_processors/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1001 2022-08-12 17:24:47.000000 tap-mambu-3.1.5/mambu_tests/tap_processors/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2669 2022-08-12 17:24:47.000000 tap-mambu-3.1.5/mambu_tests/tap_processors/test_audit_trail_processor.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      201 2022-08-12 17:24:47.000000 tap-mambu-3.1.5/mambu_tests/tap_processors/test_deposit_accounts_processor.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      311 2022-08-12 17:24:47.000000 tap-mambu-3.1.5/mambu_tests/tap_processors/test_deposit_cards_processor.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      261 2022-08-12 17:24:47.000000 tap-mambu-3.1.5/mambu_tests/tap_processors/test_loan_accounts_processor.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      269 2022-08-12 17:24:47.000000 tap-mambu-3.1.5/mambu_tests/tap_processors/test_loan_repayments_processor.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    14265 2022-10-12 18:27:12.000000 tap-mambu-3.1.5/mambu_tests/tap_processors/test_processors.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    16141 2022-09-27 17:20:33.000000 tap-mambu-3.1.5/mambu_tests/test_client.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3453 2022-08-12 17:24:47.000000 tap-mambu-3.1.5/mambu_tests/test_helpers.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7154 2022-09-27 17:20:33.000000 tap-mambu-3.1.5/mambu_tests/test_sync.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2022-10-13 13:28:34.494474 tap-mambu-3.1.5/schema_fetcher/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2022-08-12 17:24:47.000000 tap-mambu-3.1.5/schema_fetcher/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1725 2022-08-12 17:24:47.000000 tap-mambu-3.1.5/schema_fetcher/constants.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      304 2022-08-12 17:24:47.000000 tap-mambu-3.1.5/schema_fetcher/converters.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      102 2022-08-12 17:24:47.000000 tap-mambu-3.1.5/schema_fetcher/custom_exceptions.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1090 2022-08-12 17:24:47.000000 tap-mambu-3.1.5/schema_fetcher/helpers.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8223 2022-08-12 17:24:47.000000 tap-mambu-3.1.5/schema_fetcher/main.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2022-10-13 13:28:34.546474 tap-mambu-3.1.5/setup.cfg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1138 2022-10-12 20:49:55.000000 tap-mambu-3.1.5/setup.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2022-10-13 13:28:34.494474 tap-mambu-3.1.5/tap_mambu/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1533 2022-08-12 17:24:47.000000 tap-mambu-3.1.5/tap_mambu/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2022-10-13 13:28:34.506474 tap-mambu-3.1.5/tap_mambu/helpers/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4970 2022-09-27 17:20:33.000000 tap-mambu-3.1.5/tap_mambu/helpers/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7112 2022-08-12 17:24:47.000000 tap-mambu-3.1.5/tap_mambu/helpers/client.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       24 2022-08-12 17:24:47.000000 tap-mambu-3.1.5/tap_mambu/helpers/constants.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2280 2022-10-07 17:57:55.000000 tap-mambu-3.1.5/tap_mambu/helpers/datetime_utils.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      921 2022-08-12 17:24:47.000000 tap-mambu-3.1.5/tap_mambu/helpers/discover.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      119 2022-08-12 17:24:47.000000 tap-mambu-3.1.5/tap_mambu/helpers/exceptions.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4448 2022-08-12 17:24:47.000000 tap-mambu-3.1.5/tap_mambu/helpers/generator_processor_pairs.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      684 2022-08-12 17:24:47.000000 tap-mambu-3.1.5/tap_mambu/helpers/hashable_dict.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1396 2022-08-12 17:24:47.000000 tap-mambu-3.1.5/tap_mambu/helpers/metrics_plotter.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2045 2022-09-27 17:20:33.000000 tap-mambu-3.1.5/tap_mambu/helpers/multithreaded_requests.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2866 2022-08-12 17:24:47.000000 tap-mambu-3.1.5/tap_mambu/helpers/perf_metrics.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4982 2022-08-12 17:24:47.000000 tap-mambu-3.1.5/tap_mambu/helpers/schema.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2022-10-13 13:28:34.522474 tap-mambu-3.1.5/tap_mambu/helpers/schemas/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3896 2022-08-12 17:24:47.000000 tap-mambu-3.1.5/tap_mambu/helpers/schemas/activities.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1138 2022-08-12 17:24:47.000000 tap-mambu-3.1.5/tap_mambu/helpers/schemas/audit_trail.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4771 2022-08-12 17:24:47.000000 tap-mambu-3.1.5/tap_mambu/helpers/schemas/branches.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      203 2022-08-12 17:24:47.000000 tap-mambu-3.1.5/tap_mambu/helpers/schemas/cards.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3545 2022-08-12 17:24:47.000000 tap-mambu-3.1.5/tap_mambu/helpers/schemas/centres.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    10574 2022-08-12 17:24:47.000000 tap-mambu-3.1.5/tap_mambu/helpers/schemas/clients.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2622 2022-08-12 17:24:47.000000 tap-mambu-3.1.5/tap_mambu/helpers/schemas/communications.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2777 2022-08-12 17:24:47.000000 tap-mambu-3.1.5/tap_mambu/helpers/schemas/credit_arrangements.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6070 2022-08-12 17:24:47.000000 tap-mambu-3.1.5/tap_mambu/helpers/schemas/custom_field_sets.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    15149 2022-08-12 17:24:47.000000 tap-mambu-3.1.5/tap_mambu/helpers/schemas/deposit_accounts.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    22827 2022-08-12 17:24:47.000000 tap-mambu-3.1.5/tap_mambu/helpers/schemas/deposit_products.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    18592 2022-08-12 17:24:47.000000 tap-mambu-3.1.5/tap_mambu/helpers/schemas/deposit_transactions.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2257 2022-08-12 17:24:47.000000 tap-mambu-3.1.5/tap_mambu/helpers/schemas/gl_accounts.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5788 2022-08-12 17:24:47.000000 tap-mambu-3.1.5/tap_mambu/helpers/schemas/gl_journal_entries.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5899 2022-08-12 17:24:47.000000 tap-mambu-3.1.5/tap_mambu/helpers/schemas/groups.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1189 2022-08-12 17:24:47.000000 tap-mambu-3.1.5/tap_mambu/helpers/schemas/index_rate_sources.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    10033 2022-08-12 17:24:47.000000 tap-mambu-3.1.5/tap_mambu/helpers/schemas/installments.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4144 2022-08-12 17:24:47.000000 tap-mambu-3.1.5/tap_mambu/helpers/schemas/interest_accrual_breakdown.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    31788 2022-08-12 17:24:47.000000 tap-mambu-3.1.5/tap_mambu/helpers/schemas/loan_accounts.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    43883 2022-08-12 17:24:47.000000 tap-mambu-3.1.5/tap_mambu/helpers/schemas/loan_products.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5677 2022-08-12 17:24:47.000000 tap-mambu-3.1.5/tap_mambu/helpers/schemas/loan_repayments.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    13302 2022-08-12 17:24:47.000000 tap-mambu-3.1.5/tap_mambu/helpers/schemas/loan_transactions.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2081 2022-08-12 17:24:47.000000 tap-mambu-3.1.5/tap_mambu/helpers/schemas/tasks.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4776 2022-08-12 17:24:47.000000 tap-mambu-3.1.5/tap_mambu/helpers/schemas/users.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      537 2022-09-27 17:20:33.000000 tap-mambu-3.1.5/tap_mambu/helpers/transformer.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5177 2022-09-27 17:20:33.000000 tap-mambu-3.1.5/tap_mambu/sync.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2022-10-13 13:28:34.542474 tap-mambu-3.1.5/tap_mambu/tap_generators/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2022-08-12 17:24:47.000000 tap-mambu-3.1.5/tap_mambu/tap_generators/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1382 2022-09-27 17:20:33.000000 tap-mambu-3.1.5/tap_mambu/tap_generators/activities_generator.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2536 2022-09-27 17:20:33.000000 tap-mambu-3.1.5/tap_mambu/tap_generators/audit_trail_generator.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      380 2022-08-12 17:24:47.000000 tap-mambu-3.1.5/tap_mambu/tap_generators/branches_generator.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      477 2022-08-12 17:24:47.000000 tap-mambu-3.1.5/tap_mambu/tap_generators/centres_generator.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      485 2022-08-12 17:24:47.000000 tap-mambu-3.1.5/tap_mambu/tap_generators/child_generator.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1218 2022-09-27 17:20:33.000000 tap-mambu-3.1.5/tap_mambu/tap_generators/clients_generator.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1382 2022-09-27 17:20:33.000000 tap-mambu-3.1.5/tap_mambu/tap_generators/communications_generator.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      406 2022-08-12 17:24:47.000000 tap-mambu-3.1.5/tap_mambu/tap_generators/credit_arrangements_generator.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      279 2022-08-12 17:24:47.000000 tap-mambu-3.1.5/tap_mambu/tap_generators/custom_field_sets_generator.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1237 2022-09-27 17:20:33.000000 tap-mambu-3.1.5/tap_mambu/tap_generators/deposit_accounts_generator.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      478 2022-08-12 17:24:47.000000 tap-mambu-3.1.5/tap_mambu/tap_generators/deposit_cards_generator.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      337 2022-08-12 17:24:47.000000 tap-mambu-3.1.5/tap_mambu/tap_generators/deposit_products_generator.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1187 2022-09-27 17:20:33.000000 tap-mambu-3.1.5/tap_mambu/tap_generators/deposit_transactions_generator.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4266 2022-08-12 17:24:47.000000 tap-mambu-3.1.5/tap_mambu/tap_generators/generator.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      375 2022-08-12 17:24:47.000000 tap-mambu-3.1.5/tap_mambu/tap_generators/gl_accounts_generator.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1304 2022-09-27 17:20:33.000000 tap-mambu-3.1.5/tap_mambu/tap_generators/gl_journal_entries_generator.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1124 2022-09-27 17:20:33.000000 tap-mambu-3.1.5/tap_mambu/tap_generators/groups_generator.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      443 2022-08-12 17:24:47.000000 tap-mambu-3.1.5/tap_mambu/tap_generators/index_rate_sources_generator.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      991 2022-09-27 17:20:33.000000 tap-mambu-3.1.5/tap_mambu/tap_generators/installments_generator.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1272 2022-09-27 17:20:33.000000 tap-mambu-3.1.5/tap_mambu/tap_generators/interest_accrual_breakdown_generator.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1557 2022-09-27 17:20:33.000000 tap-mambu-3.1.5/tap_mambu/tap_generators/loan_accounts_generator.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      378 2022-08-12 17:24:47.000000 tap-mambu-3.1.5/tap_mambu/tap_generators/loan_products_generator.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      394 2022-08-12 17:24:47.000000 tap-mambu-3.1.5/tap_mambu/tap_generators/loan_repayments_generator.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1086 2022-09-27 17:20:33.000000 tap-mambu-3.1.5/tap_mambu/tap_generators/loan_transactions_generator.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4971 2022-09-27 17:20:33.000000 tap-mambu-3.1.5/tap_mambu/tap_generators/multithreaded_bookmark_generator.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6834 2022-09-27 17:20:33.000000 tap-mambu-3.1.5/tap_mambu/tap_generators/multithreaded_offset_generator.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      344 2022-08-12 17:24:47.000000 tap-mambu-3.1.5/tap_mambu/tap_generators/no_pagination_generator.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      521 2022-08-12 17:24:47.000000 tap-mambu-3.1.5/tap_mambu/tap_generators/tasks_generator.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      410 2022-08-12 17:24:47.000000 tap-mambu-3.1.5/tap_mambu/tap_generators/users_generator.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2022-10-13 13:28:34.546474 tap-mambu-3.1.5/tap_mambu/tap_processors/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2022-08-12 17:24:47.000000 tap-mambu-3.1.5/tap_mambu/tap_processors/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2692 2022-09-27 17:20:33.000000 tap-mambu-3.1.5/tap_mambu/tap_processors/audit_trail_processor.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      650 2022-08-12 17:24:47.000000 tap-mambu-3.1.5/tap_mambu/tap_processors/child_processor.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4774 2022-09-27 17:20:33.000000 tap-mambu-3.1.5/tap_mambu/tap_processors/deduplication_processor.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      292 2022-08-12 17:24:47.000000 tap-mambu-3.1.5/tap_mambu/tap_processors/deposit_accounts_processor.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      260 2022-08-12 17:24:47.000000 tap-mambu-3.1.5/tap_mambu/tap_processors/deposit_cards_processor.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      427 2022-08-12 17:24:47.000000 tap-mambu-3.1.5/tap_mambu/tap_processors/loan_accounts_processor.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      217 2022-08-12 17:24:47.000000 tap-mambu-3.1.5/tap_mambu/tap_processors/loan_repayments_processor.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1613 2022-09-27 17:20:33.000000 tap-mambu-3.1.5/tap_mambu/tap_processors/multithreaded_parent_processor.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5648 2022-10-12 18:27:12.000000 tap-mambu-3.1.5/tap_mambu/tap_processors/processor.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2022-10-13 13:28:34.494474 tap-mambu-3.1.5/tap_mambu.egg-info/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      332 2022-10-13 13:28:34.000000 tap-mambu-3.1.5/tap_mambu.egg-info/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6426 2022-10-13 13:28:34.000000 tap-mambu-3.1.5/tap_mambu.egg-info/SOURCES.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2022-10-13 13:28:34.000000 tap-mambu-3.1.5/tap_mambu.egg-info/dependency_links.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       45 2022-10-13 13:28:34.000000 tap-mambu-3.1.5/tap_mambu.egg-info/entry_points.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      218 2022-10-13 13:28:34.000000 tap-mambu-3.1.5/tap_mambu.egg-info/requires.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       37 2022-10-13 13:28:34.000000 tap-mambu-3.1.5/tap_mambu.egg-info/top_level.txt
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-02-23 16:00:39.318190 tap-mambu-4.0.0/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    34523 2021-06-02 17:27:03.000000 tap-mambu-4.0.0/LICENSE
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       57 2022-11-22 19:50:53.000000 tap-mambu-4.0.0/MANIFEST.in
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      396 2023-02-23 16:00:39.318190 tap-mambu-4.0.0/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    19218 2022-04-18 14:39:39.000000 tap-mambu-4.0.0/README.md
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-02-23 16:00:39.242190 tap-mambu-4.0.0/mambu_tests/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2022-11-22 19:50:53.000000 tap-mambu-4.0.0/mambu_tests/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      953 2022-11-22 19:50:53.000000 tap-mambu-4.0.0/mambu_tests/conftest.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      413 2022-11-22 19:50:53.000000 tap-mambu-4.0.0/mambu_tests/constants.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3873 2022-11-22 19:50:53.000000 tap-mambu-4.0.0/mambu_tests/helpers.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-02-23 16:00:39.246190 tap-mambu-4.0.0/mambu_tests/multithreading/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2022-11-22 19:50:53.000000 tap-mambu-4.0.0/mambu_tests/multithreading/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4418 2022-11-22 19:50:53.000000 tap-mambu-4.0.0/mambu_tests/multithreading/test_multithreaded_bookmark_daybyday_generator.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    13914 2022-11-22 19:50:53.000000 tap-mambu-4.0.0/mambu_tests/multithreading/test_multithreaded_bookmark_generator.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    16607 2022-11-22 19:50:53.000000 tap-mambu-4.0.0/mambu_tests/multithreading/test_multithreaded_offset_generator.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4660 2022-11-22 19:50:53.000000 tap-mambu-4.0.0/mambu_tests/multithreading/test_requests_pool.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-02-23 16:00:39.266190 tap-mambu-4.0.0/mambu_tests/tap_generators/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1541 2022-11-22 19:50:53.000000 tap-mambu-4.0.0/mambu_tests/tap_generators/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1604 2022-11-22 19:50:53.000000 tap-mambu-4.0.0/mambu_tests/tap_generators/test_activities_generator.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3245 2022-11-22 19:50:53.000000 tap-mambu-4.0.0/mambu_tests/tap_generators/test_audit_trail_generator.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      537 2022-11-22 19:50:53.000000 tap-mambu-4.0.0/mambu_tests/tap_generators/test_branches_generator.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      546 2022-11-22 19:50:53.000000 tap-mambu-4.0.0/mambu_tests/tap_generators/test_centres_generator.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      669 2022-11-22 19:50:53.000000 tap-mambu-4.0.0/mambu_tests/tap_generators/test_clients_generator.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      608 2022-11-22 19:50:53.000000 tap-mambu-4.0.0/mambu_tests/tap_generators/test_communications_generator.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      565 2022-11-22 19:50:53.000000 tap-mambu-4.0.0/mambu_tests/tap_generators/test_credit_arrangements_generator.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      338 2022-11-22 19:50:53.000000 tap-mambu-4.0.0/mambu_tests/tap_generators/test_custom_field_sets_generator.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      688 2022-11-22 19:50:53.000000 tap-mambu-4.0.0/mambu_tests/tap_generators/test_deposit_accounts_generator.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      376 2022-11-22 19:50:53.000000 tap-mambu-4.0.0/mambu_tests/tap_generators/test_deposit_cards_generator.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      403 2022-11-22 19:50:53.000000 tap-mambu-4.0.0/mambu_tests/tap_generators/test_deposit_products_generator.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      687 2022-11-22 19:50:53.000000 tap-mambu-4.0.0/mambu_tests/tap_generators/test_deposit_transactions_generator.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9335 2022-11-22 19:50:53.000000 tap-mambu-4.0.0/mambu_tests/tap_generators/test_generators.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      429 2022-11-22 19:50:53.000000 tap-mambu-4.0.0/mambu_tests/tap_generators/test_gl_accounts_generator.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1072 2022-11-22 19:50:53.000000 tap-mambu-4.0.0/mambu_tests/tap_generators/test_gl_journal_entries_generator.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      630 2022-11-22 19:50:53.000000 tap-mambu-4.0.0/mambu_tests/tap_generators/test_groups_generator.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      602 2022-11-22 19:50:53.000000 tap-mambu-4.0.0/mambu_tests/tap_generators/test_index_rate_sources_generator.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      630 2022-11-22 19:50:53.000000 tap-mambu-4.0.0/mambu_tests/tap_generators/test_installments_generator.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      676 2022-11-22 19:50:53.000000 tap-mambu-4.0.0/mambu_tests/tap_generators/test_interest_accrual_breakdown_generator.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1181 2022-11-22 19:50:53.000000 tap-mambu-4.0.0/mambu_tests/tap_generators/test_loan_accounts_generators.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      457 2022-11-22 19:50:53.000000 tap-mambu-4.0.0/mambu_tests/tap_generators/test_loan_products_generator.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      663 2022-11-22 19:50:53.000000 tap-mambu-4.0.0/mambu_tests/tap_generators/test_loan_transactions_generator.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1480 2022-11-22 19:50:53.000000 tap-mambu-4.0.0/mambu_tests/tap_generators/test_no_pagination_generators.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      374 2022-11-22 19:50:53.000000 tap-mambu-4.0.0/mambu_tests/tap_generators/test_repayments_generator.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      528 2022-11-22 19:50:53.000000 tap-mambu-4.0.0/mambu_tests/tap_generators/test_tasks_generator.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      514 2022-11-22 19:50:53.000000 tap-mambu-4.0.0/mambu_tests/tap_generators/test_users_generator.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-02-23 16:00:39.266190 tap-mambu-4.0.0/mambu_tests/tap_processors/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1001 2022-11-22 19:50:53.000000 tap-mambu-4.0.0/mambu_tests/tap_processors/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2669 2022-11-22 19:50:53.000000 tap-mambu-4.0.0/mambu_tests/tap_processors/test_audit_trail_processor.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      201 2022-11-22 19:50:53.000000 tap-mambu-4.0.0/mambu_tests/tap_processors/test_deposit_accounts_processor.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      311 2022-11-22 19:50:53.000000 tap-mambu-4.0.0/mambu_tests/tap_processors/test_deposit_cards_processor.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      261 2022-11-22 19:50:53.000000 tap-mambu-4.0.0/mambu_tests/tap_processors/test_loan_accounts_processor.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      269 2022-11-22 19:50:53.000000 tap-mambu-4.0.0/mambu_tests/tap_processors/test_loan_repayments_processor.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    14265 2022-11-22 19:50:53.000000 tap-mambu-4.0.0/mambu_tests/tap_processors/test_processors.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    16141 2022-11-22 19:50:53.000000 tap-mambu-4.0.0/mambu_tests/test_client.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3453 2022-11-22 19:50:53.000000 tap-mambu-4.0.0/mambu_tests/test_helpers.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7154 2022-11-22 19:50:53.000000 tap-mambu-4.0.0/mambu_tests/test_sync.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-02-23 16:00:39.270190 tap-mambu-4.0.0/schema_fetcher/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2022-11-22 19:50:53.000000 tap-mambu-4.0.0/schema_fetcher/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1725 2022-11-22 19:50:53.000000 tap-mambu-4.0.0/schema_fetcher/constants.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      304 2022-11-22 19:50:53.000000 tap-mambu-4.0.0/schema_fetcher/converters.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      102 2022-11-22 19:50:53.000000 tap-mambu-4.0.0/schema_fetcher/custom_exceptions.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1090 2022-11-22 19:50:53.000000 tap-mambu-4.0.0/schema_fetcher/helpers.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8223 2022-11-22 19:50:53.000000 tap-mambu-4.0.0/schema_fetcher/main.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2023-02-23 16:00:39.318190 tap-mambu-4.0.0/setup.cfg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1138 2023-02-23 15:59:14.000000 tap-mambu-4.0.0/setup.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-02-23 16:00:39.270190 tap-mambu-4.0.0/tap_mambu/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1533 2022-11-22 19:50:53.000000 tap-mambu-4.0.0/tap_mambu/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-02-23 16:00:39.278190 tap-mambu-4.0.0/tap_mambu/helpers/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4276 2023-02-15 21:20:39.000000 tap-mambu-4.0.0/tap_mambu/helpers/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7112 2023-02-15 20:13:29.000000 tap-mambu-4.0.0/tap_mambu/helpers/client.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       24 2022-11-22 19:50:53.000000 tap-mambu-4.0.0/tap_mambu/helpers/constants.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2280 2022-11-22 19:50:53.000000 tap-mambu-4.0.0/tap_mambu/helpers/datetime_utils.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      921 2022-11-22 19:50:53.000000 tap-mambu-4.0.0/tap_mambu/helpers/discover.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      119 2022-11-22 19:50:53.000000 tap-mambu-4.0.0/tap_mambu/helpers/exceptions.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4448 2022-11-22 19:50:53.000000 tap-mambu-4.0.0/tap_mambu/helpers/generator_processor_pairs.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      684 2022-11-22 19:50:53.000000 tap-mambu-4.0.0/tap_mambu/helpers/hashable_dict.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1396 2022-11-22 19:50:53.000000 tap-mambu-4.0.0/tap_mambu/helpers/metrics_plotter.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2045 2023-02-23 15:33:32.000000 tap-mambu-4.0.0/tap_mambu/helpers/multithreaded_requests.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2866 2022-11-22 19:50:53.000000 tap-mambu-4.0.0/tap_mambu/helpers/perf_metrics.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4982 2022-11-22 19:50:53.000000 tap-mambu-4.0.0/tap_mambu/helpers/schema.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-02-23 16:00:39.294190 tap-mambu-4.0.0/tap_mambu/helpers/schemas/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3896 2022-11-22 19:50:53.000000 tap-mambu-4.0.0/tap_mambu/helpers/schemas/activities.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1138 2022-11-22 19:50:53.000000 tap-mambu-4.0.0/tap_mambu/helpers/schemas/audit_trail.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4297 2023-02-15 21:20:39.000000 tap-mambu-4.0.0/tap_mambu/helpers/schemas/branches.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      203 2022-11-22 19:50:53.000000 tap-mambu-4.0.0/tap_mambu/helpers/schemas/cards.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3071 2023-02-15 21:20:39.000000 tap-mambu-4.0.0/tap_mambu/helpers/schemas/centres.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    10100 2023-02-15 21:20:39.000000 tap-mambu-4.0.0/tap_mambu/helpers/schemas/clients.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2148 2023-02-15 21:20:39.000000 tap-mambu-4.0.0/tap_mambu/helpers/schemas/communications.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2303 2023-02-15 21:20:39.000000 tap-mambu-4.0.0/tap_mambu/helpers/schemas/credit_arrangements.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5596 2023-02-15 21:20:39.000000 tap-mambu-4.0.0/tap_mambu/helpers/schemas/custom_field_sets.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    14675 2023-02-15 21:20:39.000000 tap-mambu-4.0.0/tap_mambu/helpers/schemas/deposit_accounts.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    22353 2023-02-15 21:20:39.000000 tap-mambu-4.0.0/tap_mambu/helpers/schemas/deposit_products.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    18118 2023-02-15 21:20:39.000000 tap-mambu-4.0.0/tap_mambu/helpers/schemas/deposit_transactions.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1783 2023-02-15 21:20:39.000000 tap-mambu-4.0.0/tap_mambu/helpers/schemas/gl_accounts.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5314 2023-02-15 21:20:39.000000 tap-mambu-4.0.0/tap_mambu/helpers/schemas/gl_journal_entries.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5425 2023-02-15 21:20:39.000000 tap-mambu-4.0.0/tap_mambu/helpers/schemas/groups.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      715 2023-02-15 21:20:39.000000 tap-mambu-4.0.0/tap_mambu/helpers/schemas/index_rate_sources.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9559 2023-02-15 21:20:39.000000 tap-mambu-4.0.0/tap_mambu/helpers/schemas/installments.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3670 2023-02-15 21:20:39.000000 tap-mambu-4.0.0/tap_mambu/helpers/schemas/interest_accrual_breakdown.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    31314 2023-02-15 21:20:39.000000 tap-mambu-4.0.0/tap_mambu/helpers/schemas/loan_accounts.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    43409 2023-02-15 21:20:39.000000 tap-mambu-4.0.0/tap_mambu/helpers/schemas/loan_products.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5677 2022-11-22 19:50:53.000000 tap-mambu-4.0.0/tap_mambu/helpers/schemas/loan_repayments.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    12828 2023-02-15 21:20:39.000000 tap-mambu-4.0.0/tap_mambu/helpers/schemas/loan_transactions.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1607 2023-02-15 21:20:39.000000 tap-mambu-4.0.0/tap_mambu/helpers/schemas/tasks.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4302 2023-02-15 21:20:39.000000 tap-mambu-4.0.0/tap_mambu/helpers/schemas/users.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      537 2022-11-22 19:50:53.000000 tap-mambu-4.0.0/tap_mambu/helpers/transformer.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5177 2022-11-22 19:50:53.000000 tap-mambu-4.0.0/tap_mambu/sync.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-02-23 16:00:39.314190 tap-mambu-4.0.0/tap_mambu/tap_generators/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2022-11-22 19:50:53.000000 tap-mambu-4.0.0/tap_mambu/tap_generators/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1382 2022-11-22 19:50:53.000000 tap-mambu-4.0.0/tap_mambu/tap_generators/activities_generator.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2536 2022-11-22 19:50:53.000000 tap-mambu-4.0.0/tap_mambu/tap_generators/audit_trail_generator.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      380 2022-11-22 19:50:53.000000 tap-mambu-4.0.0/tap_mambu/tap_generators/branches_generator.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      477 2022-11-22 19:50:53.000000 tap-mambu-4.0.0/tap_mambu/tap_generators/centres_generator.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      485 2022-11-22 19:50:53.000000 tap-mambu-4.0.0/tap_mambu/tap_generators/child_generator.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1218 2022-11-22 19:50:53.000000 tap-mambu-4.0.0/tap_mambu/tap_generators/clients_generator.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1382 2022-11-22 19:50:53.000000 tap-mambu-4.0.0/tap_mambu/tap_generators/communications_generator.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      406 2022-11-22 19:50:53.000000 tap-mambu-4.0.0/tap_mambu/tap_generators/credit_arrangements_generator.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      279 2022-11-22 19:50:53.000000 tap-mambu-4.0.0/tap_mambu/tap_generators/custom_field_sets_generator.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1237 2022-11-22 19:50:53.000000 tap-mambu-4.0.0/tap_mambu/tap_generators/deposit_accounts_generator.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      478 2022-11-22 19:50:53.000000 tap-mambu-4.0.0/tap_mambu/tap_generators/deposit_cards_generator.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      337 2022-11-22 19:50:53.000000 tap-mambu-4.0.0/tap_mambu/tap_generators/deposit_products_generator.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1187 2022-11-22 19:50:53.000000 tap-mambu-4.0.0/tap_mambu/tap_generators/deposit_transactions_generator.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4266 2023-02-15 20:34:05.000000 tap-mambu-4.0.0/tap_mambu/tap_generators/generator.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      375 2022-11-22 19:50:53.000000 tap-mambu-4.0.0/tap_mambu/tap_generators/gl_accounts_generator.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1304 2022-11-22 19:50:53.000000 tap-mambu-4.0.0/tap_mambu/tap_generators/gl_journal_entries_generator.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1124 2022-11-22 19:50:53.000000 tap-mambu-4.0.0/tap_mambu/tap_generators/groups_generator.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      443 2022-11-22 19:50:53.000000 tap-mambu-4.0.0/tap_mambu/tap_generators/index_rate_sources_generator.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      991 2022-11-22 19:50:53.000000 tap-mambu-4.0.0/tap_mambu/tap_generators/installments_generator.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1272 2022-11-22 19:50:53.000000 tap-mambu-4.0.0/tap_mambu/tap_generators/interest_accrual_breakdown_generator.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1557 2022-11-22 19:50:53.000000 tap-mambu-4.0.0/tap_mambu/tap_generators/loan_accounts_generator.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      378 2022-11-22 19:50:53.000000 tap-mambu-4.0.0/tap_mambu/tap_generators/loan_products_generator.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      394 2022-11-22 19:50:53.000000 tap-mambu-4.0.0/tap_mambu/tap_generators/loan_repayments_generator.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1086 2022-11-22 19:50:53.000000 tap-mambu-4.0.0/tap_mambu/tap_generators/loan_transactions_generator.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4971 2022-11-22 19:50:53.000000 tap-mambu-4.0.0/tap_mambu/tap_generators/multithreaded_bookmark_generator.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6834 2023-02-15 20:34:08.000000 tap-mambu-4.0.0/tap_mambu/tap_generators/multithreaded_offset_generator.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      344 2022-11-22 19:50:53.000000 tap-mambu-4.0.0/tap_mambu/tap_generators/no_pagination_generator.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      521 2022-11-22 19:50:53.000000 tap-mambu-4.0.0/tap_mambu/tap_generators/tasks_generator.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      410 2022-11-22 19:50:53.000000 tap-mambu-4.0.0/tap_mambu/tap_generators/users_generator.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-02-23 16:00:39.318190 tap-mambu-4.0.0/tap_mambu/tap_processors/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2022-11-22 19:50:53.000000 tap-mambu-4.0.0/tap_mambu/tap_processors/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2692 2022-11-22 19:50:53.000000 tap-mambu-4.0.0/tap_mambu/tap_processors/audit_trail_processor.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      650 2022-11-22 19:50:53.000000 tap-mambu-4.0.0/tap_mambu/tap_processors/child_processor.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4774 2022-11-22 19:50:53.000000 tap-mambu-4.0.0/tap_mambu/tap_processors/deduplication_processor.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      292 2022-11-22 19:50:53.000000 tap-mambu-4.0.0/tap_mambu/tap_processors/deposit_accounts_processor.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      260 2022-11-22 19:50:53.000000 tap-mambu-4.0.0/tap_mambu/tap_processors/deposit_cards_processor.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      427 2022-11-22 19:50:53.000000 tap-mambu-4.0.0/tap_mambu/tap_processors/loan_accounts_processor.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      217 2022-11-22 19:50:53.000000 tap-mambu-4.0.0/tap_mambu/tap_processors/loan_repayments_processor.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1613 2022-11-22 19:50:53.000000 tap-mambu-4.0.0/tap_mambu/tap_processors/multithreaded_parent_processor.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5648 2023-02-23 15:33:29.000000 tap-mambu-4.0.0/tap_mambu/tap_processors/processor.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-02-23 16:00:39.274190 tap-mambu-4.0.0/tap_mambu.egg-info/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      396 2023-02-23 16:00:39.000000 tap-mambu-4.0.0/tap_mambu.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6426 2023-02-23 16:00:39.000000 tap-mambu-4.0.0/tap_mambu.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-02-23 16:00:39.000000 tap-mambu-4.0.0/tap_mambu.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       70 2023-02-23 16:00:39.000000 tap-mambu-4.0.0/tap_mambu.egg-info/entry_points.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      218 2023-02-23 16:00:39.000000 tap-mambu-4.0.0/tap_mambu.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       37 2023-02-23 16:00:39.000000 tap-mambu-4.0.0/tap_mambu.egg-info/top_level.txt
```

### Comparing `tap-mambu-3.1.5/LICENSE` & `tap-mambu-4.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tap-mambu-3.1.5/README.md` & `tap-mambu-4.0.0/README.md`

 * *Files identical despite different names*

### Comparing `tap-mambu-3.1.5/mambu_tests/conftest.py` & `tap-mambu-4.0.0/mambu_tests/conftest.py`

 * *Files identical despite different names*

### Comparing `tap-mambu-3.1.5/mambu_tests/helpers.py` & `tap-mambu-4.0.0/mambu_tests/helpers.py`

 * *Files identical despite different names*

### Comparing `tap-mambu-3.1.5/mambu_tests/multithreading/test_multithreaded_bookmark_daybyday_generator.py` & `tap-mambu-4.0.0/mambu_tests/multithreading/test_multithreaded_bookmark_daybyday_generator.py`

 * *Files identical despite different names*

### Comparing `tap-mambu-3.1.5/mambu_tests/multithreading/test_multithreaded_bookmark_generator.py` & `tap-mambu-4.0.0/mambu_tests/multithreading/test_multithreaded_bookmark_generator.py`

 * *Files identical despite different names*

### Comparing `tap-mambu-3.1.5/mambu_tests/multithreading/test_multithreaded_offset_generator.py` & `tap-mambu-4.0.0/mambu_tests/multithreading/test_multithreaded_offset_generator.py`

 * *Files identical despite different names*

### Comparing `tap-mambu-3.1.5/mambu_tests/multithreading/test_requests_pool.py` & `tap-mambu-4.0.0/mambu_tests/multithreading/test_requests_pool.py`

 * *Files identical despite different names*

### Comparing `tap-mambu-3.1.5/mambu_tests/tap_generators/__init__.py` & `tap-mambu-4.0.0/mambu_tests/tap_generators/__init__.py`

 * *Files identical despite different names*

### Comparing `tap-mambu-3.1.5/mambu_tests/tap_generators/test_activities_generator.py` & `tap-mambu-4.0.0/mambu_tests/tap_generators/test_activities_generator.py`

 * *Files identical despite different names*

### Comparing `tap-mambu-3.1.5/mambu_tests/tap_generators/test_audit_trail_generator.py` & `tap-mambu-4.0.0/mambu_tests/tap_generators/test_audit_trail_generator.py`

 * *Files identical despite different names*

### Comparing `tap-mambu-3.1.5/mambu_tests/tap_generators/test_branches_generator.py` & `tap-mambu-4.0.0/mambu_tests/tap_generators/test_branches_generator.py`

 * *Files identical despite different names*

### Comparing `tap-mambu-3.1.5/mambu_tests/tap_generators/test_centres_generator.py` & `tap-mambu-4.0.0/mambu_tests/tap_generators/test_centres_generator.py`

 * *Files identical despite different names*

### Comparing `tap-mambu-3.1.5/mambu_tests/tap_generators/test_clients_generator.py` & `tap-mambu-4.0.0/mambu_tests/tap_generators/test_clients_generator.py`

 * *Files identical despite different names*

### Comparing `tap-mambu-3.1.5/mambu_tests/tap_generators/test_communications_generator.py` & `tap-mambu-4.0.0/mambu_tests/tap_generators/test_communications_generator.py`

 * *Files identical despite different names*

### Comparing `tap-mambu-3.1.5/mambu_tests/tap_generators/test_credit_arrangements_generator.py` & `tap-mambu-4.0.0/mambu_tests/tap_generators/test_credit_arrangements_generator.py`

 * *Files identical despite different names*

### Comparing `tap-mambu-3.1.5/mambu_tests/tap_generators/test_deposit_accounts_generator.py` & `tap-mambu-4.0.0/mambu_tests/tap_generators/test_deposit_accounts_generator.py`

 * *Files identical despite different names*

### Comparing `tap-mambu-3.1.5/mambu_tests/tap_generators/test_deposit_transactions_generator.py` & `tap-mambu-4.0.0/mambu_tests/tap_generators/test_deposit_transactions_generator.py`

 * *Files identical despite different names*

### Comparing `tap-mambu-3.1.5/mambu_tests/tap_generators/test_generators.py` & `tap-mambu-4.0.0/mambu_tests/tap_generators/test_generators.py`

 * *Files identical despite different names*

### Comparing `tap-mambu-3.1.5/mambu_tests/tap_generators/test_gl_journal_entries_generator.py` & `tap-mambu-4.0.0/mambu_tests/tap_generators/test_gl_journal_entries_generator.py`

 * *Files identical despite different names*

### Comparing `tap-mambu-3.1.5/mambu_tests/tap_generators/test_groups_generator.py` & `tap-mambu-4.0.0/mambu_tests/tap_generators/test_groups_generator.py`

 * *Files identical despite different names*

### Comparing `tap-mambu-3.1.5/mambu_tests/tap_generators/test_index_rate_sources_generator.py` & `tap-mambu-4.0.0/mambu_tests/tap_generators/test_index_rate_sources_generator.py`

 * *Files identical despite different names*

### Comparing `tap-mambu-3.1.5/mambu_tests/tap_generators/test_installments_generator.py` & `tap-mambu-4.0.0/mambu_tests/tap_generators/test_installments_generator.py`

 * *Files identical despite different names*

### Comparing `tap-mambu-3.1.5/mambu_tests/tap_generators/test_interest_accrual_breakdown_generator.py` & `tap-mambu-4.0.0/mambu_tests/tap_generators/test_interest_accrual_breakdown_generator.py`

 * *Files identical despite different names*

### Comparing `tap-mambu-3.1.5/mambu_tests/tap_generators/test_loan_accounts_generators.py` & `tap-mambu-4.0.0/mambu_tests/tap_generators/test_loan_accounts_generators.py`

 * *Files identical despite different names*

### Comparing `tap-mambu-3.1.5/mambu_tests/tap_generators/test_loan_transactions_generator.py` & `tap-mambu-4.0.0/mambu_tests/tap_generators/test_loan_transactions_generator.py`

 * *Files identical despite different names*

### Comparing `tap-mambu-3.1.5/mambu_tests/tap_generators/test_no_pagination_generators.py` & `tap-mambu-4.0.0/mambu_tests/tap_generators/test_no_pagination_generators.py`

 * *Files identical despite different names*

### Comparing `tap-mambu-3.1.5/mambu_tests/tap_generators/test_tasks_generator.py` & `tap-mambu-4.0.0/mambu_tests/tap_generators/test_tasks_generator.py`

 * *Files identical despite different names*

### Comparing `tap-mambu-3.1.5/mambu_tests/tap_generators/test_users_generator.py` & `tap-mambu-4.0.0/mambu_tests/tap_generators/test_users_generator.py`

 * *Files identical despite different names*

### Comparing `tap-mambu-3.1.5/mambu_tests/tap_processors/__init__.py` & `tap-mambu-4.0.0/mambu_tests/tap_processors/__init__.py`

 * *Files identical despite different names*

### Comparing `tap-mambu-3.1.5/mambu_tests/tap_processors/test_audit_trail_processor.py` & `tap-mambu-4.0.0/mambu_tests/tap_processors/test_audit_trail_processor.py`

 * *Files identical despite different names*

### Comparing `tap-mambu-3.1.5/mambu_tests/tap_processors/test_processors.py` & `tap-mambu-4.0.0/mambu_tests/tap_processors/test_processors.py`

 * *Files identical despite different names*

### Comparing `tap-mambu-3.1.5/mambu_tests/test_client.py` & `tap-mambu-4.0.0/mambu_tests/test_client.py`

 * *Files identical despite different names*

### Comparing `tap-mambu-3.1.5/mambu_tests/test_helpers.py` & `tap-mambu-4.0.0/mambu_tests/test_helpers.py`

 * *Files identical despite different names*

### Comparing `tap-mambu-3.1.5/mambu_tests/test_sync.py` & `tap-mambu-4.0.0/mambu_tests/test_sync.py`

 * *Files identical despite different names*

### Comparing `tap-mambu-3.1.5/schema_fetcher/constants.py` & `tap-mambu-4.0.0/schema_fetcher/constants.py`

 * *Files identical despite different names*

### Comparing `tap-mambu-3.1.5/schema_fetcher/helpers.py` & `tap-mambu-4.0.0/schema_fetcher/helpers.py`

 * *Files identical despite different names*

### Comparing `tap-mambu-3.1.5/schema_fetcher/main.py` & `tap-mambu-4.0.0/schema_fetcher/main.py`

 * *Files identical despite different names*

### Comparing `tap-mambu-3.1.5/setup.py` & `tap-mambu-4.0.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 
 from setuptools import setup, find_packages
 
 setup(name='tap-mambu',
-      version='3.1.5',
+      version='4.0.0',
       description='Singer.io tap for extracting data from the Mambu 2.0 API',
       author='jeff.huth@bytecode.io',
       classifiers=['Programming Language :: Python :: 3 :: Only'],
       py_modules=['tap_mambu'],
       python_requires='>=3.9',
       install_requires=[
           'backoff==1.8.0',
```

### Comparing `tap-mambu-3.1.5/tap_mambu/__init__.py` & `tap-mambu-4.0.0/tap_mambu/__init__.py`

 * *Files identical despite different names*

### Comparing `tap-mambu-3.1.5/tap_mambu/helpers/__init__.py` & `tap-mambu-4.0.0/tap_mambu/helpers/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -55,53 +55,32 @@
         elif isinstance(this_json[key], list):
             out[new_key] = convert_array(this_json[key])
         else:
             out[new_key] = this_json[key]
     return out
 
 
-def remove_custom_nodes(this_json):
-    if not isinstance(this_json, (dict, list)):
-        return this_json
-    if isinstance(this_json, list):
-        return [remove_custom_nodes(vv) for vv in this_json]
-    return {kk: remove_custom_nodes(vv) for kk, vv in this_json.items()
-            if not kk[:1] == '_'}
-
-
-def add_custom_field(key, record, custom_field_sets):
-    for cf_key, cf_value in record.items():
-        field = {
-            'field_set_id': key,
-            'id': cf_key,
-            'value': cf_value,
-        }
-        custom_field_sets.append(field)
-
-
-# Convert custom fields and sets
-# Generalize/Abstract custom fields to key/value pairs
+# Move Custom Fields objects under custom_fields key
 def convert_custom_fields(this_json):
     for record in this_json:
         cust_field_sets = []
         for key, value in record.items():
             if key.startswith('_'):
                 if isinstance(value, dict):
-                    add_custom_field(key, value, cust_field_sets)
+                    cust_field_sets.append({key: value})
                 elif isinstance(value, list):
-                    for element in value:
-                        add_custom_field(key, element, cust_field_sets)
+                    cust_field_sets.append({key: value})
         record['custom_fields'] = cust_field_sets
     return this_json
 
 
 # Run all transforms: denests _embedded, removes _embedded/_links, and
 #  convert camelCase to snake_case for fieldname keys.
 def transform_json(this_json, path):
-    new_json = remove_custom_nodes(convert_custom_fields(this_json))
+    new_json = convert_custom_fields(this_json)
     out = dict()
     out[path] = new_json
     transformed_json = convert_json(out)
     return transformed_json[path]
 
 
 # def transform_activities(this_json):
```

### Comparing `tap-mambu-3.1.5/tap_mambu/helpers/client.py` & `tap-mambu-4.0.0/tap_mambu/helpers/client.py`

 * *Files identical despite different names*

### Comparing `tap-mambu-3.1.5/tap_mambu/helpers/datetime_utils.py` & `tap-mambu-4.0.0/tap_mambu/helpers/datetime_utils.py`

 * *Files identical despite different names*

### Comparing `tap-mambu-3.1.5/tap_mambu/helpers/discover.py` & `tap-mambu-4.0.0/tap_mambu/helpers/discover.py`

 * *Files identical despite different names*

### Comparing `tap-mambu-3.1.5/tap_mambu/helpers/generator_processor_pairs.py` & `tap-mambu-4.0.0/tap_mambu/helpers/generator_processor_pairs.py`

 * *Files identical despite different names*

### Comparing `tap-mambu-3.1.5/tap_mambu/helpers/hashable_dict.py` & `tap-mambu-4.0.0/tap_mambu/helpers/hashable_dict.py`

 * *Files identical despite different names*

### Comparing `tap-mambu-3.1.5/tap_mambu/helpers/metrics_plotter.py` & `tap-mambu-4.0.0/tap_mambu/helpers/metrics_plotter.py`

 * *Files identical despite different names*

### Comparing `tap-mambu-3.1.5/tap_mambu/helpers/multithreaded_requests.py` & `tap-mambu-4.0.0/tap_mambu/helpers/multithreaded_requests.py`

 * *Files identical despite different names*

### Comparing `tap-mambu-3.1.5/tap_mambu/helpers/perf_metrics.py` & `tap-mambu-4.0.0/tap_mambu/helpers/perf_metrics.py`

 * *Files identical despite different names*

### Comparing `tap-mambu-3.1.5/tap_mambu/helpers/schema.py` & `tap-mambu-4.0.0/tap_mambu/helpers/schema.py`

 * *Files identical despite different names*

### Comparing `tap-mambu-3.1.5/tap_mambu/helpers/schemas/activities.json` & `tap-mambu-4.0.0/tap_mambu/helpers/schemas/activities.json`

 * *Files identical despite different names*

### Comparing `tap-mambu-3.1.5/tap_mambu/helpers/schemas/audit_trail.json` & `tap-mambu-4.0.0/tap_mambu/helpers/schemas/audit_trail.json`

 * *Files identical despite different names*

### Comparing `tap-mambu-3.1.5/tap_mambu/helpers/schemas/branches.json` & `tap-mambu-4.0.0/tap_mambu/helpers/schemas/branches.json`

 * *Files 3% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9930555555555557%*

 * *Differences: {"'properties'": "{'custom_fields': {replace: OrderedDict([('type', ['null', 'array']), ('items', "*

 * *                 "OrderedDict([('type', ['null', 'object']), ('additionalProperties', True), "*

 * *                 "('properties', OrderedDict())]))])}}"}*

```diff
@@ -143,45 +143,25 @@
             "format": "date-time",
             "type": [
                 "null",
                 "string"
             ]
         },
         "custom_fields": {
-            "anyOf": [
-                {
-                    "items": {
-                        "additionalProperties": false,
-                        "properties": {
-                            "field_set_id": {
-                                "type": [
-                                    "null",
-                                    "string"
-                                ]
-                            },
-                            "id": {
-                                "type": [
-                                    "null",
-                                    "string"
-                                ]
-                            },
-                            "value": {
-                                "type": [
-                                    "null",
-                                    "string"
-                                ]
-                            }
-                        },
-                        "type": "object"
-                    },
-                    "type": "array"
-                },
-                {
-                    "type": "null"
-                }
+            "items": {
+                "additionalProperties": true,
+                "properties": {},
+                "type": [
+                    "null",
+                    "object"
+                ]
+            },
+            "type": [
+                "null",
+                "array"
             ]
         },
         "email_address": {
             "type": [
                 "null",
                 "string"
             ]
```

### Comparing `tap-mambu-3.1.5/tap_mambu/helpers/schemas/centres.json` & `tap-mambu-4.0.0/tap_mambu/helpers/schemas/centres.json`

 * *Files 13% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9924242424242425%*

 * *Differences: {"'properties'": "{'custom_fields': {replace: OrderedDict([('type', ['null', 'array']), ('items', "*

 * *                 "OrderedDict([('type', ['null', 'object']), ('additionalProperties', True), "*

 * *                 "('properties', OrderedDict())]))])}}"}*

```diff
@@ -95,45 +95,25 @@
             "format": "date-time",
             "type": [
                 "null",
                 "string"
             ]
         },
         "custom_fields": {
-            "anyOf": [
-                {
-                    "items": {
-                        "additionalProperties": false,
-                        "properties": {
-                            "field_set_id": {
-                                "type": [
-                                    "null",
-                                    "string"
-                                ]
-                            },
-                            "id": {
-                                "type": [
-                                    "null",
-                                    "string"
-                                ]
-                            },
-                            "value": {
-                                "type": [
-                                    "null",
-                                    "string"
-                                ]
-                            }
-                        },
-                        "type": "object"
-                    },
-                    "type": "array"
-                },
-                {
-                    "type": "null"
-                }
+            "items": {
+                "additionalProperties": true,
+                "properties": {},
+                "type": [
+                    "null",
+                    "object"
+                ]
+            },
+            "type": [
+                "null",
+                "array"
             ]
         },
         "encoded_key": {
             "type": [
                 "null",
                 "string"
             ]
```

### Comparing `tap-mambu-3.1.5/tap_mambu/helpers/schemas/clients.json` & `tap-mambu-4.0.0/tap_mambu/helpers/schemas/clients.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9974747474747474%*

 * *Differences: {"'properties'": "{'custom_fields': {replace: OrderedDict([('type', ['null', 'array']), ('items', "*

 * *                 "OrderedDict([('type', ['null', 'object']), ('additionalProperties', True), "*

 * *                 "('properties', OrderedDict())]))])}}"}*

```diff
@@ -141,45 +141,25 @@
             "format": "date-time",
             "type": [
                 "null",
                 "string"
             ]
         },
         "custom_fields": {
-            "anyOf": [
-                {
-                    "items": {
-                        "additionalProperties": false,
-                        "properties": {
-                            "field_set_id": {
-                                "type": [
-                                    "null",
-                                    "string"
-                                ]
-                            },
-                            "id": {
-                                "type": [
-                                    "null",
-                                    "string"
-                                ]
-                            },
-                            "value": {
-                                "type": [
-                                    "null",
-                                    "string"
-                                ]
-                            }
-                        },
-                        "type": "object"
-                    },
-                    "type": "array"
-                },
-                {
-                    "type": "null"
-                }
+            "items": {
+                "additionalProperties": true,
+                "properties": {},
+                "type": [
+                    "null",
+                    "object"
+                ]
+            },
+            "type": [
+                "null",
+                "array"
             ]
         },
         "email_address": {
             "type": [
                 "null",
                 "string"
             ]
```

### Comparing `tap-mambu-3.1.5/tap_mambu/helpers/schemas/communications.json` & `tap-mambu-4.0.0/tap_mambu/helpers/schemas/communications.json`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9962121212121212%*

 * *Differences: {"'properties'": "{'custom_fields': {replace: OrderedDict([('type', ['null', 'array']), ('items', "*

 * *                 "OrderedDict([('type', ['null', 'object']), ('additionalProperties', True), "*

 * *                 "('properties', OrderedDict())]))])}}"}*

```diff
@@ -17,45 +17,25 @@
             "format": "date-time",
             "type": [
                 "null",
                 "string"
             ]
         },
         "custom_fields": {
-            "anyOf": [
-                {
-                    "items": {
-                        "additionalProperties": false,
-                        "properties": {
-                            "field_set_id": {
-                                "type": [
-                                    "null",
-                                    "string"
-                                ]
-                            },
-                            "id": {
-                                "type": [
-                                    "null",
-                                    "string"
-                                ]
-                            },
-                            "value": {
-                                "type": [
-                                    "null",
-                                    "string"
-                                ]
-                            }
-                        },
-                        "type": "object"
-                    },
-                    "type": "array"
-                },
-                {
-                    "type": "null"
-                }
+            "items": {
+                "additionalProperties": true,
+                "properties": {},
+                "type": [
+                    "null",
+                    "object"
+                ]
+            },
+            "type": [
+                "null",
+                "array"
             ]
         },
         "deposit_account_key": {
             "type": [
                 "null",
                 "string"
             ]
```

### Comparing `tap-mambu-3.1.5/tap_mambu/helpers/schemas/credit_arrangements.json` & `tap-mambu-4.0.0/tap_mambu/helpers/schemas/credit_arrangements.json`

 * *Files 9% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9956140350877193%*

 * *Differences: {"'properties'": "{'custom_fields': {replace: OrderedDict([('type', ['null', 'array']), ('items', "*

 * *                 "OrderedDict([('type', ['null', 'object']), ('additionalProperties', True), "*

 * *                 "('properties', OrderedDict())]))])}}"}*

```diff
@@ -55,45 +55,25 @@
             },
             "type": [
                 "null",
                 "object"
             ]
         },
         "custom_fields": {
-            "anyOf": [
-                {
-                    "items": {
-                        "additionalProperties": false,
-                        "properties": {
-                            "field_set_id": {
-                                "type": [
-                                    "null",
-                                    "string"
-                                ]
-                            },
-                            "id": {
-                                "type": [
-                                    "null",
-                                    "string"
-                                ]
-                            },
-                            "value": {
-                                "type": [
-                                    "null",
-                                    "string"
-                                ]
-                            }
-                        },
-                        "type": "object"
-                    },
-                    "type": "array"
-                },
-                {
-                    "type": "null"
-                }
+            "items": {
+                "additionalProperties": true,
+                "properties": {},
+                "type": [
+                    "null",
+                    "object"
+                ]
+            },
+            "type": [
+                "null",
+                "array"
             ]
         },
         "encoded_key": {
             "type": [
                 "null",
                 "string"
             ]
```

### Comparing `tap-mambu-3.1.5/tap_mambu/helpers/schemas/custom_field_sets.json` & `tap-mambu-4.0.0/tap_mambu/helpers/schemas/custom_field_sets.json`

 * *Files 3% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9944444444444445%*

 * *Differences: {"'properties'": "{'custom_fields': {replace: OrderedDict([('type', ['null', 'array']), ('items', "*

 * *                 "OrderedDict([('type', ['null', 'object']), ('additionalProperties', True), "*

 * *                 "('properties', OrderedDict())]))])}}"}*

```diff
@@ -11,45 +11,25 @@
             "format": "date-time",
             "type": [
                 "null",
                 "string"
             ]
         },
         "custom_fields": {
-            "anyOf": [
-                {
-                    "items": {
-                        "additionalProperties": false,
-                        "properties": {
-                            "field_set_id": {
-                                "type": [
-                                    "null",
-                                    "string"
-                                ]
-                            },
-                            "id": {
-                                "type": [
-                                    "null",
-                                    "string"
-                                ]
-                            },
-                            "value": {
-                                "type": [
-                                    "null",
-                                    "string"
-                                ]
-                            }
-                        },
-                        "type": "object"
-                    },
-                    "type": "array"
-                },
-                {
-                    "type": "null"
-                }
+            "items": {
+                "additionalProperties": true,
+                "properties": {},
+                "type": [
+                    "null",
+                    "object"
+                ]
+            },
+            "type": [
+                "null",
+                "array"
             ]
         },
         "dependent_field_key": {
             "type": [
                 "null",
                 "string"
             ]
```

### Comparing `tap-mambu-3.1.5/tap_mambu/helpers/schemas/deposit_accounts.json` & `tap-mambu-4.0.0/tap_mambu/helpers/schemas/deposit_accounts.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9976851851851851%*

 * *Differences: {"'properties'": "{'custom_fields': {replace: OrderedDict([('type', ['null', 'array']), ('items', "*

 * *                 "OrderedDict([('type', ['null', 'object']), ('additionalProperties', True), "*

 * *                 "('properties', OrderedDict())]))])}}"}*

```diff
@@ -203,45 +203,25 @@
         "currency_code": {
             "type": [
                 "null",
                 "string"
             ]
         },
         "custom_fields": {
-            "anyOf": [
-                {
-                    "items": {
-                        "additionalProperties": false,
-                        "properties": {
-                            "field_set_id": {
-                                "type": [
-                                    "null",
-                                    "string"
-                                ]
-                            },
-                            "id": {
-                                "type": [
-                                    "null",
-                                    "string"
-                                ]
-                            },
-                            "value": {
-                                "type": [
-                                    "null",
-                                    "string"
-                                ]
-                            }
-                        },
-                        "type": "object"
-                    },
-                    "type": "array"
-                },
-                {
-                    "type": "null"
-                }
+            "items": {
+                "additionalProperties": true,
+                "properties": {},
+                "type": [
+                    "null",
+                    "object"
+                ]
+            },
+            "type": [
+                "null",
+                "array"
             ]
         },
         "encoded_key": {
             "type": [
                 "null",
                 "string"
             ]
```

### Comparing `tap-mambu-3.1.5/tap_mambu/helpers/schemas/deposit_products.json` & `tap-mambu-4.0.0/tap_mambu/helpers/schemas/deposit_products.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9965277777777777%*

 * *Differences: {"'properties'": "{'custom_fields': {replace: OrderedDict([('type', ['null', 'array']), ('items', "*

 * *                 "OrderedDict([('type', ['null', 'object']), ('additionalProperties', True), "*

 * *                 "('properties', OrderedDict())]))])}}"}*

```diff
@@ -162,45 +162,25 @@
             },
             "type": [
                 "null",
                 "object"
             ]
         },
         "custom_fields": {
-            "anyOf": [
-                {
-                    "items": {
-                        "additionalProperties": false,
-                        "properties": {
-                            "field_set_id": {
-                                "type": [
-                                    "null",
-                                    "string"
-                                ]
-                            },
-                            "id": {
-                                "type": [
-                                    "null",
-                                    "string"
-                                ]
-                            },
-                            "value": {
-                                "type": [
-                                    "null",
-                                    "string"
-                                ]
-                            }
-                        },
-                        "type": "object"
-                    },
-                    "type": "array"
-                },
-                {
-                    "type": "null"
-                }
+            "items": {
+                "additionalProperties": true,
+                "properties": {},
+                "type": [
+                    "null",
+                    "object"
+                ]
+            },
+            "type": [
+                "null",
+                "array"
             ]
         },
         "encoded_key": {
             "type": [
                 "null",
                 "string"
             ]
```

### Comparing `tap-mambu-3.1.5/tap_mambu/helpers/schemas/deposit_transactions.json` & `tap-mambu-4.0.0/tap_mambu/helpers/schemas/deposit_transactions.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9973958333333334%*

 * *Differences: {"'properties'": "{'custom_fields': {replace: OrderedDict([('type', ['null', 'array']), ('items', "*

 * *                 "OrderedDict([('type', ['null', 'object']), ('additionalProperties', True), "*

 * *                 "('properties', OrderedDict())]))])}}"}*

```diff
@@ -246,45 +246,25 @@
         "currency_code": {
             "type": [
                 "null",
                 "string"
             ]
         },
         "custom_fields": {
-            "anyOf": [
-                {
-                    "items": {
-                        "additionalProperties": false,
-                        "properties": {
-                            "field_set_id": {
-                                "type": [
-                                    "null",
-                                    "string"
-                                ]
-                            },
-                            "id": {
-                                "type": [
-                                    "null",
-                                    "string"
-                                ]
-                            },
-                            "value": {
-                                "type": [
-                                    "null",
-                                    "string"
-                                ]
-                            }
-                        },
-                        "type": "object"
-                    },
-                    "type": "array"
-                },
-                {
-                    "type": "null"
-                }
+            "items": {
+                "additionalProperties": true,
+                "properties": {},
+                "type": [
+                    "null",
+                    "object"
+                ]
+            },
+            "type": [
+                "null",
+                "array"
             ]
         },
         "encoded_key": {
             "type": [
                 "null",
                 "string"
             ]
```

### Comparing `tap-mambu-3.1.5/tap_mambu/helpers/schemas/gl_accounts.json` & `tap-mambu-4.0.0/tap_mambu/helpers/schemas/gl_accounts.json`

 * *Files 3% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9944444444444445%*

 * *Differences: {"'properties'": "{'custom_fields': {replace: OrderedDict([('type', ['null', 'array']), ('items', "*

 * *                 "OrderedDict([('type', ['null', 'object']), ('additionalProperties', True), "*

 * *                 "('properties', OrderedDict())]))])}}"}*

```diff
@@ -39,45 +39,25 @@
             },
             "type": [
                 "null",
                 "object"
             ]
         },
         "custom_fields": {
-            "anyOf": [
-                {
-                    "items": {
-                        "additionalProperties": false,
-                        "properties": {
-                            "field_set_id": {
-                                "type": [
-                                    "null",
-                                    "string"
-                                ]
-                            },
-                            "id": {
-                                "type": [
-                                    "null",
-                                    "string"
-                                ]
-                            },
-                            "value": {
-                                "type": [
-                                    "null",
-                                    "string"
-                                ]
-                            }
-                        },
-                        "type": "object"
-                    },
-                    "type": "array"
-                },
-                {
-                    "type": "null"
-                }
+            "items": {
+                "additionalProperties": true,
+                "properties": {},
+                "type": [
+                    "null",
+                    "object"
+                ]
+            },
+            "type": [
+                "null",
+                "array"
             ]
         },
         "description": {
             "type": [
                 "null",
                 "string"
             ]
```

### Comparing `tap-mambu-3.1.5/tap_mambu/helpers/schemas/gl_journal_entries.json` & `tap-mambu-4.0.0/tap_mambu/helpers/schemas/gl_journal_entries.json`

 * *Files 7% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9950980392156863%*

 * *Differences: {"'properties'": "{'custom_fields': {replace: OrderedDict([('type', ['null', 'array']), ('items', "*

 * *                 "OrderedDict([('type', ['null', 'object']), ('additionalProperties', True), "*

 * *                 "('properties', OrderedDict())]))])}}"}*

```diff
@@ -31,45 +31,25 @@
             "format": "date-time",
             "type": [
                 "null",
                 "string"
             ]
         },
         "custom_fields": {
-            "anyOf": [
-                {
-                    "items": {
-                        "additionalProperties": false,
-                        "properties": {
-                            "field_set_id": {
-                                "type": [
-                                    "null",
-                                    "string"
-                                ]
-                            },
-                            "id": {
-                                "type": [
-                                    "null",
-                                    "string"
-                                ]
-                            },
-                            "value": {
-                                "type": [
-                                    "null",
-                                    "string"
-                                ]
-                            }
-                        },
-                        "type": "object"
-                    },
-                    "type": "array"
-                },
-                {
-                    "type": "null"
-                }
+            "items": {
+                "additionalProperties": true,
+                "properties": {},
+                "type": [
+                    "null",
+                    "object"
+                ]
+            },
+            "type": [
+                "null",
+                "array"
             ]
         },
         "encoded_key": {
             "type": [
                 "null",
                 "string"
             ]
```

### Comparing `tap-mambu-3.1.5/tap_mambu/helpers/schemas/groups.json` & `tap-mambu-4.0.0/tap_mambu/helpers/schemas/groups.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9956140350877193%*

 * *Differences: {"'properties'": "{'custom_fields': {replace: OrderedDict([('type', ['null', 'array']), ('items', "*

 * *                 "OrderedDict([('type', ['null', 'object']), ('additionalProperties', True), "*

 * *                 "('properties', OrderedDict())]))])}}"}*

```diff
@@ -107,45 +107,25 @@
             "format": "date-time",
             "type": [
                 "null",
                 "string"
             ]
         },
         "custom_fields": {
-            "anyOf": [
-                {
-                    "items": {
-                        "additionalProperties": false,
-                        "properties": {
-                            "field_set_id": {
-                                "type": [
-                                    "null",
-                                    "string"
-                                ]
-                            },
-                            "id": {
-                                "type": [
-                                    "null",
-                                    "string"
-                                ]
-                            },
-                            "value": {
-                                "type": [
-                                    "null",
-                                    "string"
-                                ]
-                            }
-                        },
-                        "type": "object"
-                    },
-                    "type": "array"
-                },
-                {
-                    "type": "null"
-                }
+            "items": {
+                "additionalProperties": true,
+                "properties": {},
+                "type": [
+                    "null",
+                    "object"
+                ]
+            },
+            "type": [
+                "null",
+                "array"
             ]
         },
         "email_address": {
             "type": [
                 "null",
                 "string"
             ]
```

### Comparing `tap-mambu-3.1.5/tap_mambu/helpers/schemas/index_rate_sources.json` & `tap-mambu-4.0.0/tap_mambu/helpers/schemas/tasks.json`

 * *Files 12% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8549382716049383%*

 * *Differences: {"'properties'": "{'id': {'type': {insert: [(1, 'integer')], delete: [1]}}, 'custom_fields': "*

 * *                 "{replace: OrderedDict([('type', ['null', 'array']), ('items', "*

 * *                 "OrderedDict([('type', ['null', 'object']), ('additionalProperties', True), "*

 * *                 "('properties', OrderedDict())]))])}, 'assigned_user_key': OrderedDict([('type', "*

 * *                 "['null', 'string'])]), 'created_by_full_name': OrderedDict([('type', ['null', "*

 * *                 "'string'])]), 'created_b […]*

```diff
@@ -1,69 +1,106 @@
 {
     "additionalProperties": false,
     "properties": {
+        "assigned_user_key": {
+            "type": [
+                "null",
+                "string"
+            ]
+        },
+        "created_by_full_name": {
+            "type": [
+                "null",
+                "string"
+            ]
+        },
+        "created_by_user_key": {
+            "type": [
+                "null",
+                "string"
+            ]
+        },
+        "creation_date": {
+            "format": "date-time",
+            "type": [
+                "null",
+                "string"
+            ]
+        },
         "custom_fields": {
-            "anyOf": [
-                {
-                    "items": {
-                        "additionalProperties": false,
-                        "properties": {
-                            "field_set_id": {
-                                "type": [
-                                    "null",
-                                    "string"
-                                ]
-                            },
-                            "id": {
-                                "type": [
-                                    "null",
-                                    "string"
-                                ]
-                            },
-                            "value": {
-                                "type": [
-                                    "null",
-                                    "string"
-                                ]
-                            }
-                        },
-                        "type": "object"
-                    },
-                    "type": "array"
-                },
-                {
-                    "type": "null"
-                }
+            "items": {
+                "additionalProperties": true,
+                "properties": {},
+                "type": [
+                    "null",
+                    "object"
+                ]
+            },
+            "type": [
+                "null",
+                "array"
+            ]
+        },
+        "description": {
+            "type": [
+                "null",
+                "string"
+            ]
+        },
+        "due_date": {
+            "format": "date",
+            "type": [
+                "null",
+                "string"
             ]
         },
         "encoded_key": {
             "type": [
                 "null",
                 "string"
             ]
         },
         "id": {
             "type": [
                 "null",
+                "integer"
+            ]
+        },
+        "last_modified_date": {
+            "format": "date-time",
+            "type": [
+                "null",
+                "string"
+            ]
+        },
+        "status": {
+            "type": [
+                "null",
+                "string"
+            ]
+        },
+        "task_link_key": {
+            "type": [
+                "null",
                 "string"
             ]
         },
-        "name": {
+        "task_link_type": {
             "type": [
                 "null",
                 "string"
             ]
         },
-        "notes": {
+        "template_key": {
             "type": [
                 "null",
                 "string"
             ]
         },
-        "type": {
+        "title": {
             "type": [
                 "null",
                 "string"
             ]
         }
     },
     "type": "object"
```

### Comparing `tap-mambu-3.1.5/tap_mambu/helpers/schemas/installments.json` & `tap-mambu-4.0.0/tap_mambu/helpers/schemas/installments.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9940476190476191%*

 * *Differences: {"'properties'": "{'custom_fields': {replace: OrderedDict([('type', ['null', 'array']), ('items', "*

 * *                 "OrderedDict([('type', ['null', 'object']), ('additionalProperties', True), "*

 * *                 "('properties', OrderedDict())]))])}}"}*

```diff
@@ -1,42 +1,22 @@
 {
     "additionalProperties": false,
     "properties": {
         "custom_fields": {
-            "anyOf": [
-                {
-                    "items": {
-                        "additionalProperties": false,
-                        "properties": {
-                            "field_set_id": {
-                                "type": [
-                                    "null",
-                                    "string"
-                                ]
-                            },
-                            "id": {
-                                "type": [
-                                    "null",
-                                    "string"
-                                ]
-                            },
-                            "value": {
-                                "type": [
-                                    "null",
-                                    "string"
-                                ]
-                            }
-                        },
-                        "type": "object"
-                    },
-                    "type": "array"
-                },
-                {
-                    "type": "null"
-                }
+            "items": {
+                "additionalProperties": true,
+                "properties": {},
+                "type": [
+                    "null",
+                    "object"
+                ]
+            },
+            "type": [
+                "null",
+                "array"
             ]
         },
         "due_date": {
             "format": "date-time",
             "type": [
                 "null",
                 "string"
```

### Comparing `tap-mambu-3.1.5/tap_mambu/helpers/schemas/interest_accrual_breakdown.json` & `tap-mambu-4.0.0/tap_mambu/helpers/schemas/interest_accrual_breakdown.json`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9958333333333332%*

 * *Differences: {"'properties'": "{'custom_fields': {replace: OrderedDict([('type', ['null', 'array']), ('items', "*

 * *                 "OrderedDict([('type', ['null', 'object']), ('additionalProperties', True), "*

 * *                 "('properties', OrderedDict())]))])}}"}*

```diff
@@ -43,45 +43,25 @@
             "format": "date-time",
             "type": [
                 "null",
                 "string"
             ]
         },
         "custom_fields": {
-            "anyOf": [
-                {
-                    "items": {
-                        "additionalProperties": false,
-                        "properties": {
-                            "field_set_id": {
-                                "type": [
-                                    "null",
-                                    "string"
-                                ]
-                            },
-                            "id": {
-                                "type": [
-                                    "null",
-                                    "string"
-                                ]
-                            },
-                            "value": {
-                                "type": [
-                                    "null",
-                                    "string"
-                                ]
-                            }
-                        },
-                        "type": "object"
-                    },
-                    "type": "array"
-                },
-                {
-                    "type": "null"
-                }
+            "items": {
+                "additionalProperties": true,
+                "properties": {},
+                "type": [
+                    "null",
+                    "object"
+                ]
+            },
+            "type": [
+                "null",
+                "array"
             ]
         },
         "entry_id": {
             "type": [
                 "null",
                 "integer"
             ]
```

### Comparing `tap-mambu-3.1.5/tap_mambu/helpers/schemas/loan_accounts.json` & `tap-mambu-4.0.0/tap_mambu/helpers/schemas/loan_accounts.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9986559139784946%*

 * *Differences: {"'properties'": "{'custom_fields': {replace: OrderedDict([('type', ['null', 'array']), ('items', "*

 * *                 "OrderedDict([('type', ['null', 'object']), ('additionalProperties', True), "*

 * *                 "('properties', OrderedDict())]))])}}"}*

```diff
@@ -376,45 +376,25 @@
             },
             "type": [
                 "null",
                 "object"
             ]
         },
         "custom_fields": {
-            "anyOf": [
-                {
-                    "items": {
-                        "additionalProperties": false,
-                        "properties": {
-                            "field_set_id": {
-                                "type": [
-                                    "null",
-                                    "string"
-                                ]
-                            },
-                            "id": {
-                                "type": [
-                                    "null",
-                                    "string"
-                                ]
-                            },
-                            "value": {
-                                "type": [
-                                    "null",
-                                    "string"
-                                ]
-                            }
-                        },
-                        "type": "object"
-                    },
-                    "type": "array"
-                },
-                {
-                    "type": "null"
-                }
+            "items": {
+                "additionalProperties": true,
+                "properties": {},
+                "type": [
+                    "null",
+                    "object"
+                ]
+            },
+            "type": [
+                "null",
+                "array"
             ]
         },
         "days_in_arrears": {
             "type": [
                 "null",
                 "integer"
             ]
```

### Comparing `tap-mambu-3.1.5/tap_mambu/helpers/schemas/loan_products.json` & `tap-mambu-4.0.0/tap_mambu/helpers/schemas/loan_products.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9974747474747474%*

 * *Differences: {"'properties'": "{'custom_fields': {replace: OrderedDict([('type', ['null', 'array']), ('items', "*

 * *                 "OrderedDict([('type', ['null', 'object']), ('additionalProperties', True), "*

 * *                 "('properties', OrderedDict())]))])}}"}*

```diff
@@ -319,45 +319,25 @@
             },
             "type": [
                 "null",
                 "object"
             ]
         },
         "custom_fields": {
-            "anyOf": [
-                {
-                    "items": {
-                        "additionalProperties": false,
-                        "properties": {
-                            "field_set_id": {
-                                "type": [
-                                    "null",
-                                    "string"
-                                ]
-                            },
-                            "id": {
-                                "type": [
-                                    "null",
-                                    "string"
-                                ]
-                            },
-                            "value": {
-                                "type": [
-                                    "null",
-                                    "string"
-                                ]
-                            }
-                        },
-                        "type": "object"
-                    },
-                    "type": "array"
-                },
-                {
-                    "type": "null"
-                }
+            "items": {
+                "additionalProperties": true,
+                "properties": {},
+                "type": [
+                    "null",
+                    "object"
+                ]
+            },
+            "type": [
+                "null",
+                "array"
             ]
         },
         "encoded_key": {
             "type": [
                 "null",
                 "string"
             ]
```

### Comparing `tap-mambu-3.1.5/tap_mambu/helpers/schemas/loan_repayments.json` & `tap-mambu-4.0.0/tap_mambu/helpers/schemas/loan_repayments.json`

 * *Files identical despite different names*

### Comparing `tap-mambu-3.1.5/tap_mambu/helpers/schemas/loan_transactions.json` & `tap-mambu-4.0.0/tap_mambu/helpers/schemas/loan_transactions.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9974747474747474%*

 * *Differences: {"'properties'": "{'custom_fields': {replace: OrderedDict([('type', ['null', 'array']), ('items', "*

 * *                 "OrderedDict([('type', ['null', 'object']), ('additionalProperties', True), "*

 * *                 "('properties', OrderedDict())]))])}}"}*

```diff
@@ -284,45 +284,25 @@
             },
             "type": [
                 "null",
                 "object"
             ]
         },
         "custom_fields": {
-            "anyOf": [
-                {
-                    "items": {
-                        "additionalProperties": false,
-                        "properties": {
-                            "field_set_id": {
-                                "type": [
-                                    "null",
-                                    "string"
-                                ]
-                            },
-                            "id": {
-                                "type": [
-                                    "null",
-                                    "string"
-                                ]
-                            },
-                            "value": {
-                                "type": [
-                                    "null",
-                                    "string"
-                                ]
-                            }
-                        },
-                        "type": "object"
-                    },
-                    "type": "array"
-                },
-                {
-                    "type": "null"
-                }
+            "items": {
+                "additionalProperties": true,
+                "properties": {},
+                "type": [
+                    "null",
+                    "object"
+                ]
+            },
+            "type": [
+                "null",
+                "array"
             ]
         },
         "custom_payment_amounts": {
             "anyOf": [
                 {
                     "items": {
                         "additionalProperties": false,
```

### Comparing `tap-mambu-3.1.5/tap_mambu/helpers/schemas/users.json` & `tap-mambu-4.0.0/tap_mambu/helpers/schemas/users.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.996031746031746%*

 * *Differences: {"'properties'": "{'custom_fields': {replace: OrderedDict([('type', ['null', 'array']), ('items', "*

 * *                 "OrderedDict([('type', ['null', 'object']), ('additionalProperties', True), "*

 * *                 "('properties', OrderedDict())]))])}}"}*

```diff
@@ -109,45 +109,25 @@
             "format": "date-time",
             "type": [
                 "null",
                 "string"
             ]
         },
         "custom_fields": {
-            "anyOf": [
-                {
-                    "items": {
-                        "additionalProperties": false,
-                        "properties": {
-                            "field_set_id": {
-                                "type": [
-                                    "null",
-                                    "string"
-                                ]
-                            },
-                            "id": {
-                                "type": [
-                                    "null",
-                                    "string"
-                                ]
-                            },
-                            "value": {
-                                "type": [
-                                    "null",
-                                    "string"
-                                ]
-                            }
-                        },
-                        "type": "object"
-                    },
-                    "type": "array"
-                },
-                {
-                    "type": "null"
-                }
+            "items": {
+                "additionalProperties": true,
+                "properties": {},
+                "type": [
+                    "null",
+                    "object"
+                ]
+            },
+            "type": [
+                "null",
+                "array"
             ]
         },
         "email": {
             "type": [
                 "null",
                 "string"
             ]
```

### Comparing `tap-mambu-3.1.5/tap_mambu/helpers/transformer.py` & `tap-mambu-4.0.0/tap_mambu/helpers/transformer.py`

 * *Files identical despite different names*

### Comparing `tap-mambu-3.1.5/tap_mambu/sync.py` & `tap-mambu-4.0.0/tap_mambu/sync.py`

 * *Files identical despite different names*

### Comparing `tap-mambu-3.1.5/tap_mambu/tap_generators/activities_generator.py` & `tap-mambu-4.0.0/tap_mambu/tap_generators/activities_generator.py`

 * *Files identical despite different names*

### Comparing `tap-mambu-3.1.5/tap_mambu/tap_generators/audit_trail_generator.py` & `tap-mambu-4.0.0/tap_mambu/tap_generators/audit_trail_generator.py`

 * *Files identical despite different names*

### Comparing `tap-mambu-3.1.5/tap_mambu/tap_generators/clients_generator.py` & `tap-mambu-4.0.0/tap_mambu/tap_generators/clients_generator.py`

 * *Files identical despite different names*

### Comparing `tap-mambu-3.1.5/tap_mambu/tap_generators/communications_generator.py` & `tap-mambu-4.0.0/tap_mambu/tap_generators/communications_generator.py`

 * *Files identical despite different names*

### Comparing `tap-mambu-3.1.5/tap_mambu/tap_generators/deposit_accounts_generator.py` & `tap-mambu-4.0.0/tap_mambu/tap_generators/deposit_accounts_generator.py`

 * *Files identical despite different names*

### Comparing `tap-mambu-3.1.5/tap_mambu/tap_generators/deposit_transactions_generator.py` & `tap-mambu-4.0.0/tap_mambu/tap_generators/deposit_transactions_generator.py`

 * *Files identical despite different names*

### Comparing `tap-mambu-3.1.5/tap_mambu/tap_generators/generator.py` & `tap-mambu-4.0.0/tap_mambu/tap_generators/generator.py`

 * *Files identical despite different names*

### Comparing `tap-mambu-3.1.5/tap_mambu/tap_generators/gl_journal_entries_generator.py` & `tap-mambu-4.0.0/tap_mambu/tap_generators/gl_journal_entries_generator.py`

 * *Files identical despite different names*

### Comparing `tap-mambu-3.1.5/tap_mambu/tap_generators/groups_generator.py` & `tap-mambu-4.0.0/tap_mambu/tap_generators/groups_generator.py`

 * *Files identical despite different names*

### Comparing `tap-mambu-3.1.5/tap_mambu/tap_generators/installments_generator.py` & `tap-mambu-4.0.0/tap_mambu/tap_generators/installments_generator.py`

 * *Files identical despite different names*

### Comparing `tap-mambu-3.1.5/tap_mambu/tap_generators/interest_accrual_breakdown_generator.py` & `tap-mambu-4.0.0/tap_mambu/tap_generators/interest_accrual_breakdown_generator.py`

 * *Files identical despite different names*

### Comparing `tap-mambu-3.1.5/tap_mambu/tap_generators/loan_accounts_generator.py` & `tap-mambu-4.0.0/tap_mambu/tap_generators/loan_accounts_generator.py`

 * *Files identical despite different names*

### Comparing `tap-mambu-3.1.5/tap_mambu/tap_generators/loan_transactions_generator.py` & `tap-mambu-4.0.0/tap_mambu/tap_generators/loan_transactions_generator.py`

 * *Files identical despite different names*

### Comparing `tap-mambu-3.1.5/tap_mambu/tap_generators/multithreaded_bookmark_generator.py` & `tap-mambu-4.0.0/tap_mambu/tap_generators/multithreaded_bookmark_generator.py`

 * *Files identical despite different names*

### Comparing `tap-mambu-3.1.5/tap_mambu/tap_generators/multithreaded_offset_generator.py` & `tap-mambu-4.0.0/tap_mambu/tap_generators/multithreaded_offset_generator.py`

 * *Files identical despite different names*

### Comparing `tap-mambu-3.1.5/tap_mambu/tap_generators/tasks_generator.py` & `tap-mambu-4.0.0/tap_mambu/tap_generators/tasks_generator.py`

 * *Files identical despite different names*

### Comparing `tap-mambu-3.1.5/tap_mambu/tap_processors/audit_trail_processor.py` & `tap-mambu-4.0.0/tap_mambu/tap_processors/audit_trail_processor.py`

 * *Files identical despite different names*

### Comparing `tap-mambu-3.1.5/tap_mambu/tap_processors/child_processor.py` & `tap-mambu-4.0.0/tap_mambu/tap_processors/child_processor.py`

 * *Files identical despite different names*

### Comparing `tap-mambu-3.1.5/tap_mambu/tap_processors/deduplication_processor.py` & `tap-mambu-4.0.0/tap_mambu/tap_processors/deduplication_processor.py`

 * *Files identical despite different names*

### Comparing `tap-mambu-3.1.5/tap_mambu/tap_processors/multithreaded_parent_processor.py` & `tap-mambu-4.0.0/tap_mambu/tap_processors/multithreaded_parent_processor.py`

 * *Files identical despite different names*

### Comparing `tap-mambu-3.1.5/tap_mambu/tap_processors/processor.py` & `tap-mambu-4.0.0/tap_mambu/tap_processors/processor.py`

 * *Files identical despite different names*

### Comparing `tap-mambu-3.1.5/tap_mambu.egg-info/SOURCES.txt` & `tap-mambu-4.0.0/tap_mambu.egg-info/SOURCES.txt`

 * *Files identical despite different names*

