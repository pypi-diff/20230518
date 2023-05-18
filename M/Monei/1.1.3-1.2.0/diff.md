# Comparing `tmp/Monei-1.1.3.tar.gz` & `tmp/Monei-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Monei-1.1.3.tar", last modified: Wed May  3 11:03:24 2023, max compression
+gzip compressed data, was "Monei-1.2.0.tar", last modified: Thu May 18 16:43:58 2023, max compression
```

## Comparing `Monei-1.1.3.tar` & `Monei-1.2.0.tar`

### file list

```diff
@@ -1,190 +1,192 @@
-drwxr-xr-x   0 dmitriy    (501) staff       (20)        0 2023-05-03 11:03:24.024366 Monei-1.1.3/
-drwxr-xr-x   0 dmitriy    (501) staff       (20)        0 2023-05-03 11:03:23.891525 Monei-1.1.3/Monei/
--rw-r--r--   0 dmitriy    (501) staff       (20)     5448 2023-05-03 11:00:52.000000 Monei-1.1.3/Monei/__init__.py
-drwxr-xr-x   0 dmitriy    (501) staff       (20)        0 2023-05-03 11:03:23.895505 Monei-1.1.3/Monei/api/
--rw-r--r--   0 dmitriy    (501) staff       (20)      252 2023-05-03 11:00:52.000000 Monei-1.1.3/Monei/api/__init__.py
--rw-r--r--   0 dmitriy    (501) staff       (20)     7947 2023-05-03 11:00:52.000000 Monei-1.1.3/Monei/api/apple_pay_domain_api.py
--rw-r--r--   0 dmitriy    (501) staff       (20)    53999 2023-05-03 11:00:52.000000 Monei-1.1.3/Monei/api/payments_api.py
--rw-r--r--   0 dmitriy    (501) staff       (20)    40366 2023-05-03 11:00:52.000000 Monei-1.1.3/Monei/api/subscriptions_api.py
--rw-r--r--   0 dmitriy    (501) staff       (20)    27088 2023-05-03 11:00:52.000000 Monei-1.1.3/Monei/api_client.py
-drwxr-xr-x   0 dmitriy    (501) staff       (20)        0 2023-05-03 11:03:23.895974 Monei-1.1.3/Monei/apis/
--rw-r--r--   0 dmitriy    (501) staff       (20)      599 2022-07-13 14:41:18.000000 Monei-1.1.3/Monei/apis/__init__.py
--rw-r--r--   0 dmitriy    (501) staff       (20)    14466 2023-05-03 11:00:52.000000 Monei-1.1.3/Monei/configuration.py
--rw-r--r--   0 dmitriy    (501) staff       (20)     4678 2023-05-03 11:00:52.000000 Monei-1.1.3/Monei/exceptions.py
-drwxr-xr-x   0 dmitriy    (501) staff       (20)        0 2023-05-03 11:03:23.936601 Monei-1.1.3/Monei/model/
--rw-r--r--   0 dmitriy    (501) staff       (20)      339 2022-07-13 14:41:18.000000 Monei-1.1.3/Monei/model/__init__.py
--rw-r--r--   0 dmitriy    (501) staff       (20)    16834 2022-07-13 14:41:17.000000 Monei-1.1.3/Monei/model/activate_subscription_request.py
--rw-r--r--   0 dmitriy    (501) staff       (20)    13836 2022-07-13 14:41:17.000000 Monei-1.1.3/Monei/model/address.py
--rw-r--r--   0 dmitriy    (501) staff       (20)    12681 2022-07-13 14:41:17.000000 Monei-1.1.3/Monei/model/cancel_payment_request.py
--rw-r--r--   0 dmitriy    (501) staff       (20)    12577 2022-07-13 14:41:17.000000 Monei-1.1.3/Monei/model/cancel_subscription_request.py
--rw-r--r--   0 dmitriy    (501) staff       (20)    12780 2022-07-13 14:41:17.000000 Monei-1.1.3/Monei/model/capture_payment_request.py
--rw-r--r--   0 dmitriy    (501) staff       (20)    13897 2022-07-13 14:41:17.000000 Monei-1.1.3/Monei/model/card.py
--rw-r--r--   0 dmitriy    (501) staff       (20)    15438 2022-07-13 14:41:17.000000 Monei-1.1.3/Monei/model/confirm_payment_request.py
--rw-r--r--   0 dmitriy    (501) staff       (20)    12743 2022-07-13 14:41:17.000000 Monei-1.1.3/Monei/model/confirm_payment_request_payment_method.py
--rw-r--r--   0 dmitriy    (501) staff       (20)    12843 2022-07-13 14:41:17.000000 Monei-1.1.3/Monei/model/confirm_payment_request_payment_method_card.py
--rw-r--r--   0 dmitriy    (501) staff       (20)    23645 2022-07-13 14:41:17.000000 Monei-1.1.3/Monei/model/create_payment_request.py
--rw-r--r--   0 dmitriy    (501) staff       (20)    17318 2022-07-13 14:41:17.000000 Monei-1.1.3/Monei/model/create_subscription_request.py
--rw-r--r--   0 dmitriy    (501) staff       (20)    12357 2022-07-13 14:41:17.000000 Monei-1.1.3/Monei/model/domain_register200_response.py
--rw-r--r--   0 dmitriy    (501) staff       (20)    12532 2022-07-13 14:41:17.000000 Monei-1.1.3/Monei/model/error.py
--rw-r--r--   0 dmitriy    (501) staff       (20)    12983 2022-07-13 14:41:17.000000 Monei-1.1.3/Monei/model/pause_subscription_request.py
--rw-r--r--   0 dmitriy    (501) staff       (20)    24177 2022-07-13 14:41:17.000000 Monei-1.1.3/Monei/model/payment.py
--rw-r--r--   0 dmitriy    (501) staff       (20)    13516 2022-07-13 14:41:17.000000 Monei-1.1.3/Monei/model/payment_billing_details.py
--rw-r--r--   0 dmitriy    (501) staff       (20)    13224 2022-07-13 14:41:17.000000 Monei-1.1.3/Monei/model/payment_cancellation_reason.py
--rw-r--r--   0 dmitriy    (501) staff       (20)    12897 2022-07-13 14:41:17.000000 Monei-1.1.3/Monei/model/payment_customer.py
--rw-r--r--   0 dmitriy    (501) staff       (20)    13238 2022-07-13 14:41:17.000000 Monei-1.1.3/Monei/model/payment_last_refund_reason.py
--rw-r--r--   0 dmitriy    (501) staff       (20)    13322 2022-07-13 14:41:17.000000 Monei-1.1.3/Monei/model/payment_message_channel.py
--rw-r--r--   0 dmitriy    (501) staff       (20)    13501 2022-07-13 14:41:17.000000 Monei-1.1.3/Monei/model/payment_message_language.py
--rw-r--r--   0 dmitriy    (501) staff       (20)    15115 2022-07-13 14:41:17.000000 Monei-1.1.3/Monei/model/payment_next_action.py
--rw-r--r--   0 dmitriy    (501) staff       (20)    14350 2022-07-13 14:41:17.000000 Monei-1.1.3/Monei/model/payment_payment_method.py
--rw-r--r--   0 dmitriy    (501) staff       (20)    12466 2022-07-13 14:41:17.000000 Monei-1.1.3/Monei/model/payment_payment_method_bizum.py
--rw-r--r--   0 dmitriy    (501) staff       (20)    18413 2022-07-13 14:41:17.000000 Monei-1.1.3/Monei/model/payment_payment_method_card.py
--rw-r--r--   0 dmitriy    (501) staff       (20)    12412 2022-07-13 14:41:17.000000 Monei-1.1.3/Monei/model/payment_payment_method_cofidis.py
--rw-r--r--   0 dmitriy    (501) staff       (20)    12473 2022-07-13 14:41:17.000000 Monei-1.1.3/Monei/model/payment_payment_method_input.py
--rw-r--r--   0 dmitriy    (501) staff       (20)    12409 2022-07-13 14:41:17.000000 Monei-1.1.3/Monei/model/payment_payment_method_paypal.py
--rw-r--r--   0 dmitriy    (501) staff       (20)    13795 2022-07-13 14:41:17.000000 Monei-1.1.3/Monei/model/payment_payment_methods.py
--rw-r--r--   0 dmitriy    (501) staff       (20)    13206 2022-07-13 14:41:17.000000 Monei-1.1.3/Monei/model/payment_refund_reason.py
--rw-r--r--   0 dmitriy    (501) staff       (20)    13122 2022-07-13 14:41:17.000000 Monei-1.1.3/Monei/model/payment_sequence.py
--rw-r--r--   0 dmitriy    (501) staff       (20)    13203 2022-07-13 14:41:17.000000 Monei-1.1.3/Monei/model/payment_sequence_recurring.py
--rw-r--r--   0 dmitriy    (501) staff       (20)    17927 2022-07-13 14:41:17.000000 Monei-1.1.3/Monei/model/payment_session_details.py
--rw-r--r--   0 dmitriy    (501) staff       (20)    13579 2022-07-13 14:41:17.000000 Monei-1.1.3/Monei/model/payment_shipping_details.py
--rw-r--r--   0 dmitriy    (501) staff       (20)    12720 2022-07-13 14:41:17.000000 Monei-1.1.3/Monei/model/payment_shop.py
--rw-r--r--   0 dmitriy    (501) staff       (20)    13516 2022-07-13 14:41:17.000000 Monei-1.1.3/Monei/model/payment_status.py
--rw-r--r--   0 dmitriy    (501) staff       (20)    18518 2022-07-13 14:41:17.000000 Monei-1.1.3/Monei/model/payment_trace_details.py
--rw-r--r--   0 dmitriy    (501) staff       (20)    13645 2022-07-13 14:41:17.000000 Monei-1.1.3/Monei/model/payment_transaction_type.py
--rw-r--r--   0 dmitriy    (501) staff       (20)    16328 2022-07-13 14:41:17.000000 Monei-1.1.3/Monei/model/recurring_payment_request.py
--rw-r--r--   0 dmitriy    (501) staff       (20)    13130 2022-07-13 14:41:17.000000 Monei-1.1.3/Monei/model/refund_payment_request.py
--rw-r--r--   0 dmitriy    (501) staff       (20)    12531 2022-07-13 14:41:17.000000 Monei-1.1.3/Monei/model/register_domain_request.py
--rw-r--r--   0 dmitriy    (501) staff       (20)    13760 2022-07-13 14:41:17.000000 Monei-1.1.3/Monei/model/send_payment_link_request.py
--rw-r--r--   0 dmitriy    (501) staff       (20)    13791 2022-07-13 14:41:18.000000 Monei-1.1.3/Monei/model/send_payment_receipt_request.py
--rw-r--r--   0 dmitriy    (501) staff       (20)    23663 2022-07-13 14:41:18.000000 Monei-1.1.3/Monei/model/subscription.py
--rw-r--r--   0 dmitriy    (501) staff       (20)    13035 2022-07-13 14:41:18.000000 Monei-1.1.3/Monei/model/subscription_interval.py
--rw-r--r--   0 dmitriy    (501) staff       (20)    13388 2022-07-13 14:41:18.000000 Monei-1.1.3/Monei/model/subscription_last_payment.py
--rw-r--r--   0 dmitriy    (501) staff       (20)    13038 2022-07-13 14:41:18.000000 Monei-1.1.3/Monei/model/subscription_payment_method.py
--rw-r--r--   0 dmitriy    (501) staff       (20)    14681 2022-07-13 14:41:18.000000 Monei-1.1.3/Monei/model/subscription_payment_method_card.py
--rw-r--r--   0 dmitriy    (501) staff       (20)    13377 2022-07-13 14:41:18.000000 Monei-1.1.3/Monei/model/subscription_status.py
--rw-r--r--   0 dmitriy    (501) staff       (20)    17444 2022-07-13 14:41:18.000000 Monei-1.1.3/Monei/model/update_subscription_request.py
--rw-r--r--   0 dmitriy    (501) staff       (20)    83493 2022-07-13 14:41:18.000000 Monei-1.1.3/Monei/model_utils.py
-drwxr-xr-x   0 dmitriy    (501) staff       (20)        0 2023-05-03 11:03:23.977504 Monei-1.1.3/Monei/models/
--rw-r--r--   0 dmitriy    (501) staff       (20)     4839 2023-05-03 11:00:52.000000 Monei-1.1.3/Monei/models/__init__.py
--rw-r--r--   0 dmitriy    (501) staff       (20)    12145 2023-05-03 11:00:52.000000 Monei-1.1.3/Monei/models/activate_subscription_request.py
--rw-r--r--   0 dmitriy    (501) staff       (20)     7873 2023-05-03 11:00:52.000000 Monei-1.1.3/Monei/models/address.py
--rw-r--r--   0 dmitriy    (501) staff       (20)     4569 2023-05-03 11:00:52.000000 Monei-1.1.3/Monei/models/cancel_payment_request.py
--rw-r--r--   0 dmitriy    (501) staff       (20)     4764 2023-05-03 11:00:52.000000 Monei-1.1.3/Monei/models/cancel_subscription_request.py
--rw-r--r--   0 dmitriy    (501) staff       (20)     4566 2023-05-03 11:00:52.000000 Monei-1.1.3/Monei/models/capture_payment_request.py
--rw-r--r--   0 dmitriy    (501) staff       (20)     8279 2022-09-30 14:39:33.000000 Monei-1.1.3/Monei/models/card.py
--rw-r--r--   0 dmitriy    (501) staff       (20)     9680 2023-05-03 11:00:52.000000 Monei-1.1.3/Monei/models/confirm_payment_request.py
--rw-r--r--   0 dmitriy    (501) staff       (20)     4421 2023-05-03 11:00:52.000000 Monei-1.1.3/Monei/models/confirm_payment_request_payment_method.py
--rw-r--r--   0 dmitriy    (501) staff       (20)     5745 2023-05-03 11:00:52.000000 Monei-1.1.3/Monei/models/confirm_payment_request_payment_method_card.py
--rw-r--r--   0 dmitriy    (501) staff       (20)    27753 2023-05-03 11:00:52.000000 Monei-1.1.3/Monei/models/create_payment_request.py
--rw-r--r--   0 dmitriy    (501) staff       (20)    15595 2023-05-03 11:00:52.000000 Monei-1.1.3/Monei/models/create_subscription_request.py
--rw-r--r--   0 dmitriy    (501) staff       (20)     4850 2023-05-03 11:00:52.000000 Monei-1.1.3/Monei/models/error.py
--rw-r--r--   0 dmitriy    (501) staff       (20)     4192 2021-11-29 17:31:25.000000 Monei-1.1.3/Monei/models/inline_object.py
--rw-r--r--   0 dmitriy    (501) staff       (20)     4243 2023-05-03 11:00:52.000000 Monei-1.1.3/Monei/models/inline_response200.py
--rw-r--r--   0 dmitriy    (501) staff       (20)     5879 2023-05-03 11:00:52.000000 Monei-1.1.3/Monei/models/pause_subscription_request.py
--rw-r--r--   0 dmitriy    (501) staff       (20)    29033 2023-05-03 11:00:52.000000 Monei-1.1.3/Monei/models/payment.py
--rw-r--r--   0 dmitriy    (501) staff       (20)     7286 2023-05-03 11:00:52.000000 Monei-1.1.3/Monei/models/payment_billing_details.py
--rw-r--r--   0 dmitriy    (501) staff       (20)     3854 2023-05-03 11:00:52.000000 Monei-1.1.3/Monei/models/payment_cancellation_reason.py
--rw-r--r--   0 dmitriy    (501) staff       (20)     5730 2023-05-03 11:00:52.000000 Monei-1.1.3/Monei/models/payment_customer.py
--rw-r--r--   0 dmitriy    (501) staff       (20)     3846 2023-05-03 11:00:52.000000 Monei-1.1.3/Monei/models/payment_last_refund_reason.py
--rw-r--r--   0 dmitriy    (501) staff       (20)     3763 2023-05-03 11:00:52.000000 Monei-1.1.3/Monei/models/payment_message_channel.py
--rw-r--r--   0 dmitriy    (501) staff       (20)     3809 2023-05-03 11:00:52.000000 Monei-1.1.3/Monei/models/payment_message_language.py
--rw-r--r--   0 dmitriy    (501) staff       (20)     8577 2023-05-03 11:00:52.000000 Monei-1.1.3/Monei/models/payment_next_action.py
--rw-r--r--   0 dmitriy    (501) staff       (20)     7562 2023-05-03 11:00:52.000000 Monei-1.1.3/Monei/models/payment_payment_method.py
--rw-r--r--   0 dmitriy    (501) staff       (20)     4533 2023-05-03 11:00:52.000000 Monei-1.1.3/Monei/models/payment_payment_method_bizum.py
--rw-r--r--   0 dmitriy    (501) staff       (20)     4573 2023-05-03 11:00:52.000000 Monei-1.1.3/Monei/models/payment_payment_method_bizum_input.py
--rw-r--r--   0 dmitriy    (501) staff       (20)    17466 2023-05-03 11:00:52.000000 Monei-1.1.3/Monei/models/payment_payment_method_card.py
--rw-r--r--   0 dmitriy    (501) staff       (20)     8979 2023-05-03 11:00:52.000000 Monei-1.1.3/Monei/models/payment_payment_method_card_input.py
--rw-r--r--   0 dmitriy    (501) staff       (20)     4429 2023-05-03 11:00:52.000000 Monei-1.1.3/Monei/models/payment_payment_method_cofidis.py
--rw-r--r--   0 dmitriy    (501) staff       (20)     5052 2023-05-03 11:00:52.000000 Monei-1.1.3/Monei/models/payment_payment_method_input.py
--rw-r--r--   0 dmitriy    (501) staff       (20)     4421 2023-05-03 11:00:52.000000 Monei-1.1.3/Monei/models/payment_payment_method_paypal.py
--rw-r--r--   0 dmitriy    (501) staff       (20)     3830 2023-05-03 11:00:52.000000 Monei-1.1.3/Monei/models/payment_refund_reason.py
--rw-r--r--   0 dmitriy    (501) staff       (20)     5406 2023-05-03 11:00:52.000000 Monei-1.1.3/Monei/models/payment_sequence.py
--rw-r--r--   0 dmitriy    (501) staff       (20)     5474 2023-05-03 11:00:52.000000 Monei-1.1.3/Monei/models/payment_sequence_recurring.py
--rw-r--r--   0 dmitriy    (501) staff       (20)    19496 2023-05-03 11:00:52.000000 Monei-1.1.3/Monei/models/payment_session_details.py
--rw-r--r--   0 dmitriy    (501) staff       (20)     7370 2023-05-03 11:00:52.000000 Monei-1.1.3/Monei/models/payment_shipping_details.py
--rw-r--r--   0 dmitriy    (501) staff       (20)     5079 2023-05-03 11:00:52.000000 Monei-1.1.3/Monei/models/payment_shop.py
--rw-r--r--   0 dmitriy    (501) staff       (20)     3962 2023-05-03 11:00:52.000000 Monei-1.1.3/Monei/models/payment_status.py
--rw-r--r--   0 dmitriy    (501) staff       (20)    21022 2023-05-03 11:00:52.000000 Monei-1.1.3/Monei/models/payment_trace_details.py
--rw-r--r--   0 dmitriy    (501) staff       (20)     3761 2023-05-03 11:00:52.000000 Monei-1.1.3/Monei/models/payment_transaction_type.py
--rw-r--r--   0 dmitriy    (501) staff       (20)    11648 2023-05-03 11:00:52.000000 Monei-1.1.3/Monei/models/recurring_payment_request.py
--rw-r--r--   0 dmitriy    (501) staff       (20)     5284 2023-05-03 11:00:52.000000 Monei-1.1.3/Monei/models/refund_payment_request.py
--rw-r--r--   0 dmitriy    (501) staff       (20)     4642 2023-05-03 11:00:52.000000 Monei-1.1.3/Monei/models/register_domain_request.py
--rw-r--r--   0 dmitriy    (501) staff       (20)     7114 2023-05-03 11:00:52.000000 Monei-1.1.3/Monei/models/send_payment_link_request.py
--rw-r--r--   0 dmitriy    (501) staff       (20)     7196 2023-05-03 11:00:52.000000 Monei-1.1.3/Monei/models/send_payment_receipt_request.py
--rw-r--r--   0 dmitriy    (501) staff       (20)    30170 2023-05-03 11:00:52.000000 Monei-1.1.3/Monei/models/subscription.py
--rw-r--r--   0 dmitriy    (501) staff       (20)     3771 2023-05-03 11:00:52.000000 Monei-1.1.3/Monei/models/subscription_interval.py
--rw-r--r--   0 dmitriy    (501) staff       (20)     6825 2023-05-03 11:00:52.000000 Monei-1.1.3/Monei/models/subscription_last_payment.py
--rw-r--r--   0 dmitriy    (501) staff       (20)     5409 2023-05-03 11:00:52.000000 Monei-1.1.3/Monei/models/subscription_payment_method.py
--rw-r--r--   0 dmitriy    (501) staff       (20)    10674 2023-05-03 11:00:52.000000 Monei-1.1.3/Monei/models/subscription_payment_method_card.py
--rw-r--r--   0 dmitriy    (501) staff       (20)     3901 2023-05-03 11:00:52.000000 Monei-1.1.3/Monei/models/subscription_status.py
--rw-r--r--   0 dmitriy    (501) staff       (20)    16548 2023-05-03 11:00:52.000000 Monei-1.1.3/Monei/models/update_subscription_request.py
--rw-r--r--   0 dmitriy    (501) staff       (20)     1732 2023-03-15 16:02:53.000000 Monei-1.1.3/Monei/monei_client.py
--rw-r--r--   0 dmitriy    (501) staff       (20)    13201 2023-05-03 11:00:52.000000 Monei-1.1.3/Monei/rest.py
-drwxr-xr-x   0 dmitriy    (501) staff       (20)        0 2023-05-03 11:03:23.893527 Monei-1.1.3/Monei.egg-info/
--rw-r--r--   0 dmitriy    (501) staff       (20)      755 2023-05-03 11:03:23.000000 Monei-1.1.3/Monei.egg-info/PKG-INFO
--rw-r--r--   0 dmitriy    (501) staff       (20)     6598 2023-05-03 11:03:23.000000 Monei-1.1.3/Monei.egg-info/SOURCES.txt
--rw-r--r--   0 dmitriy    (501) staff       (20)        1 2023-05-03 11:03:23.000000 Monei-1.1.3/Monei.egg-info/dependency_links.txt
--rw-r--r--   0 dmitriy    (501) staff       (20)       48 2023-05-03 11:03:23.000000 Monei-1.1.3/Monei.egg-info/requires.txt
--rw-r--r--   0 dmitriy    (501) staff       (20)        6 2023-05-03 11:03:23.000000 Monei-1.1.3/Monei.egg-info/top_level.txt
--rw-r--r--   0 dmitriy    (501) staff       (20)      755 2023-05-03 11:03:24.024504 Monei-1.1.3/PKG-INFO
--rw-r--r--   0 dmitriy    (501) staff       (20)     2379 2022-02-04 13:50:42.000000 Monei-1.1.3/README.md
--rw-r--r--   0 dmitriy    (501) staff       (20)      128 2023-05-03 11:03:24.025036 Monei-1.1.3/setup.cfg
--rw-r--r--   0 dmitriy    (501) staff       (20)     1304 2021-11-29 17:24:51.000000 Monei-1.1.3/setup.py
-drwxr-xr-x   0 dmitriy    (501) staff       (20)        0 2023-05-03 11:03:24.023928 Monei-1.1.3/test/
--rw-r--r--   0 dmitriy    (501) staff       (20)     2539 2021-11-16 18:37:45.000000 Monei-1.1.3/test/test_activate_subscription_request.py
--rw-r--r--   0 dmitriy    (501) staff       (20)     1699 2021-06-21 18:57:48.000000 Monei-1.1.3/test/test_address.py
--rw-r--r--   0 dmitriy    (501) staff       (20)     1509 2021-11-16 18:37:46.000000 Monei-1.1.3/test/test_apple_pay_domain_api.py
--rw-r--r--   0 dmitriy    (501) staff       (20)     1690 2021-06-21 18:57:48.000000 Monei-1.1.3/test/test_cancel_payment_request.py
--rw-r--r--   0 dmitriy    (501) staff       (20)     2167 2021-11-16 18:37:45.000000 Monei-1.1.3/test/test_cancel_subscription_request.py
--rw-r--r--   0 dmitriy    (501) staff       (20)     1680 2021-06-21 18:57:48.000000 Monei-1.1.3/test/test_capture_payment_request.py
--rw-r--r--   0 dmitriy    (501) staff       (20)     1583 2021-06-21 18:57:48.000000 Monei-1.1.3/test/test_card.py
--rw-r--r--   0 dmitriy    (501) staff       (20)     3205 2021-06-21 18:57:48.000000 Monei-1.1.3/test/test_confirm_payment_request.py
--rw-r--r--   0 dmitriy    (501) staff       (20)     2370 2021-06-21 18:57:48.000000 Monei-1.1.3/test/test_confirm_payment_request_payment_method.py
--rw-r--r--   0 dmitriy    (501) staff       (20)     2283 2021-06-21 18:57:48.000000 Monei-1.1.3/test/test_confirm_payment_request_payment_method_card.py
--rw-r--r--   0 dmitriy    (501) staff       (20)     5396 2021-06-21 18:57:48.000000 Monei-1.1.3/test/test_create_payment_request.py
--rw-r--r--   0 dmitriy    (501) staff       (20)     4226 2021-11-16 18:37:45.000000 Monei-1.1.3/test/test_create_subscription_request.py
--rw-r--r--   0 dmitriy    (501) staff       (20)     1734 2022-07-13 14:41:17.000000 Monei-1.1.3/test/test_domain_register200_response.py
--rw-r--r--   0 dmitriy    (501) staff       (20)     1559 2021-06-21 18:57:48.000000 Monei-1.1.3/test/test_error.py
--rw-r--r--   0 dmitriy    (501) staff       (20)     2021 2021-11-16 18:37:45.000000 Monei-1.1.3/test/test_inline_object.py
--rw-r--r--   0 dmitriy    (501) staff       (20)     2063 2021-11-16 18:37:45.000000 Monei-1.1.3/test/test_inline_response200.py
--rw-r--r--   0 dmitriy    (501) staff       (20)     2198 2021-11-16 18:37:45.000000 Monei-1.1.3/test/test_pause_subscription_request.py
--rw-r--r--   0 dmitriy    (501) staff       (20)     6369 2021-07-07 16:22:19.000000 Monei-1.1.3/test/test_payment.py
--rw-r--r--   0 dmitriy    (501) staff       (20)     2100 2021-06-21 18:57:48.000000 Monei-1.1.3/test/test_payment_billing_details.py
--rw-r--r--   0 dmitriy    (501) staff       (20)     1694 2021-06-21 18:57:48.000000 Monei-1.1.3/test/test_payment_cancellation_reason.py
--rw-r--r--   0 dmitriy    (501) staff       (20)     1697 2021-06-21 18:57:48.000000 Monei-1.1.3/test/test_payment_customer.py
--rw-r--r--   0 dmitriy    (501) staff       (20)     1674 2021-06-21 18:57:48.000000 Monei-1.1.3/test/test_payment_last_refund_reason.py
--rw-r--r--   0 dmitriy    (501) staff       (20)     2314 2022-07-12 17:04:01.000000 Monei-1.1.3/test/test_payment_message_channel.py
--rw-r--r--   0 dmitriy    (501) staff       (20)     2325 2022-07-12 17:04:01.000000 Monei-1.1.3/test/test_payment_message_language.py
--rw-r--r--   0 dmitriy    (501) staff       (20)     1779 2021-07-07 16:22:19.000000 Monei-1.1.3/test/test_payment_next_action.py
--rw-r--r--   0 dmitriy    (501) staff       (20)     2322 2021-06-21 18:57:48.000000 Monei-1.1.3/test/test_payment_payment_method.py
--rw-r--r--   0 dmitriy    (501) staff       (20)     1731 2021-06-21 18:57:48.000000 Monei-1.1.3/test/test_payment_payment_method_bizum.py
--rw-r--r--   0 dmitriy    (501) staff       (20)     2452 2023-02-02 16:12:19.000000 Monei-1.1.3/test/test_payment_payment_method_bizum_input.py
--rw-r--r--   0 dmitriy    (501) staff       (20)     1908 2021-06-21 18:57:48.000000 Monei-1.1.3/test/test_payment_payment_method_card.py
--rw-r--r--   0 dmitriy    (501) staff       (20)     2635 2023-02-02 16:12:20.000000 Monei-1.1.3/test/test_payment_payment_method_card_input.py
--rw-r--r--   0 dmitriy    (501) staff       (20)     2177 2021-11-16 18:37:45.000000 Monei-1.1.3/test/test_payment_payment_method_cofidis.py
--rw-r--r--   0 dmitriy    (501) staff       (20)     1897 2021-06-21 18:57:48.000000 Monei-1.1.3/test/test_payment_payment_method_input.py
--rw-r--r--   0 dmitriy    (501) staff       (20)     1738 2021-06-21 18:57:48.000000 Monei-1.1.3/test/test_payment_payment_method_paypal.py
--rw-r--r--   0 dmitriy    (501) staff       (20)     1706 2022-07-13 14:41:17.000000 Monei-1.1.3/test/test_payment_payment_methods.py
--rw-r--r--   0 dmitriy    (501) staff       (20)     1628 2021-06-21 18:57:48.000000 Monei-1.1.3/test/test_payment_refund_reason.py
--rw-r--r--   0 dmitriy    (501) staff       (20)     1874 2021-06-21 18:57:48.000000 Monei-1.1.3/test/test_payment_sequence.py
--rw-r--r--   0 dmitriy    (501) staff       (20)     1785 2021-06-21 18:57:48.000000 Monei-1.1.3/test/test_payment_sequence_recurring.py
--rw-r--r--   0 dmitriy    (501) staff       (20)     2159 2021-06-21 18:57:48.000000 Monei-1.1.3/test/test_payment_session_details.py
--rw-r--r--   0 dmitriy    (501) staff       (20)     2111 2021-06-21 18:57:48.000000 Monei-1.1.3/test/test_payment_shipping_details.py
--rw-r--r--   0 dmitriy    (501) staff       (20)     1606 2021-06-21 18:57:48.000000 Monei-1.1.3/test/test_payment_shop.py
--rw-r--r--   0 dmitriy    (501) staff       (20)     1560 2021-06-21 18:57:48.000000 Monei-1.1.3/test/test_payment_status.py
--rw-r--r--   0 dmitriy    (501) staff       (20)     2219 2021-06-21 18:57:48.000000 Monei-1.1.3/test/test_payment_trace_details.py
--rw-r--r--   0 dmitriy    (501) staff       (20)     1661 2021-06-21 18:57:48.000000 Monei-1.1.3/test/test_payment_transaction_type.py
--rw-r--r--   0 dmitriy    (501) staff       (20)     1787 2021-06-21 18:57:48.000000 Monei-1.1.3/test/test_payments_api.py
--rw-r--r--   0 dmitriy    (501) staff       (20)     3401 2021-06-21 18:57:48.000000 Monei-1.1.3/test/test_recurring_payment_request.py
--rw-r--r--   0 dmitriy    (501) staff       (20)     1716 2021-06-21 18:57:48.000000 Monei-1.1.3/test/test_refund_payment_request.py
--rw-r--r--   0 dmitriy    (501) staff       (20)     2184 2021-11-29 17:46:51.000000 Monei-1.1.3/test/test_register_domain_request.py
--rw-r--r--   0 dmitriy    (501) staff       (20)     2198 2022-03-28 15:38:14.000000 Monei-1.1.3/test/test_send_payment_link_request.py
--rw-r--r--   0 dmitriy    (501) staff       (20)     2231 2022-03-28 15:38:14.000000 Monei-1.1.3/test/test_send_payment_receipt_request.py
--rw-r--r--   0 dmitriy    (501) staff       (20)     6061 2021-11-16 18:37:45.000000 Monei-1.1.3/test/test_subscription.py
--rw-r--r--   0 dmitriy    (501) staff       (20)     2065 2021-11-16 18:37:45.000000 Monei-1.1.3/test/test_subscription_interval.py
--rw-r--r--   0 dmitriy    (501) staff       (20)     2268 2021-11-16 18:37:45.000000 Monei-1.1.3/test/test_subscription_last_payment.py
--rw-r--r--   0 dmitriy    (501) staff       (20)     2543 2021-11-16 18:37:45.000000 Monei-1.1.3/test/test_subscription_payment_method.py
--rw-r--r--   0 dmitriy    (501) staff       (20)     2433 2021-11-16 18:37:45.000000 Monei-1.1.3/test/test_subscription_payment_method_card.py
--rw-r--r--   0 dmitriy    (501) staff       (20)     2043 2021-11-16 18:37:45.000000 Monei-1.1.3/test/test_subscription_status.py
--rw-r--r--   0 dmitriy    (501) staff       (20)     2268 2021-11-16 18:37:46.000000 Monei-1.1.3/test/test_subscriptions_api.py
--rw-r--r--   0 dmitriy    (501) staff       (20)     3994 2021-11-16 18:37:45.000000 Monei-1.1.3/test/test_update_subscription_request.py
+drwxr-xr-x   0 dmitriy    (501) staff       (20)        0 2023-05-18 16:43:58.241963 Monei-1.2.0/
+drwxr-xr-x   0 dmitriy    (501) staff       (20)        0 2023-05-18 16:43:58.151007 Monei-1.2.0/Monei/
+-rw-r--r--   0 dmitriy    (501) staff       (20)     5502 2023-05-18 16:43:52.000000 Monei-1.2.0/Monei/__init__.py
+drwxr-xr-x   0 dmitriy    (501) staff       (20)        0 2023-05-18 16:43:58.154871 Monei-1.2.0/Monei/api/
+-rw-r--r--   0 dmitriy    (501) staff       (20)      252 2023-05-18 16:43:52.000000 Monei-1.2.0/Monei/api/__init__.py
+-rw-r--r--   0 dmitriy    (501) staff       (20)     7936 2023-05-18 16:43:52.000000 Monei-1.2.0/Monei/api/apple_pay_domain_api.py
+-rw-r--r--   0 dmitriy    (501) staff       (20)    60407 2023-05-18 16:43:52.000000 Monei-1.2.0/Monei/api/payments_api.py
+-rw-r--r--   0 dmitriy    (501) staff       (20)    40355 2023-05-18 16:43:52.000000 Monei-1.2.0/Monei/api/subscriptions_api.py
+-rw-r--r--   0 dmitriy    (501) staff       (20)    27077 2023-05-18 16:43:52.000000 Monei-1.2.0/Monei/api_client.py
+drwxr-xr-x   0 dmitriy    (501) staff       (20)        0 2023-05-18 16:43:58.155311 Monei-1.2.0/Monei/apis/
+-rw-r--r--   0 dmitriy    (501) staff       (20)      599 2022-07-13 14:41:18.000000 Monei-1.2.0/Monei/apis/__init__.py
+-rw-r--r--   0 dmitriy    (501) staff       (20)    14455 2023-05-18 16:43:52.000000 Monei-1.2.0/Monei/configuration.py
+-rw-r--r--   0 dmitriy    (501) staff       (20)     4667 2023-05-18 16:43:52.000000 Monei-1.2.0/Monei/exceptions.py
+drwxr-xr-x   0 dmitriy    (501) staff       (20)        0 2023-05-18 16:43:58.187672 Monei-1.2.0/Monei/model/
+-rw-r--r--   0 dmitriy    (501) staff       (20)      339 2022-07-13 14:41:18.000000 Monei-1.2.0/Monei/model/__init__.py
+-rw-r--r--   0 dmitriy    (501) staff       (20)    16834 2022-07-13 14:41:17.000000 Monei-1.2.0/Monei/model/activate_subscription_request.py
+-rw-r--r--   0 dmitriy    (501) staff       (20)    13836 2022-07-13 14:41:17.000000 Monei-1.2.0/Monei/model/address.py
+-rw-r--r--   0 dmitriy    (501) staff       (20)    12681 2022-07-13 14:41:17.000000 Monei-1.2.0/Monei/model/cancel_payment_request.py
+-rw-r--r--   0 dmitriy    (501) staff       (20)    12577 2022-07-13 14:41:17.000000 Monei-1.2.0/Monei/model/cancel_subscription_request.py
+-rw-r--r--   0 dmitriy    (501) staff       (20)    12780 2022-07-13 14:41:17.000000 Monei-1.2.0/Monei/model/capture_payment_request.py
+-rw-r--r--   0 dmitriy    (501) staff       (20)    13897 2022-07-13 14:41:17.000000 Monei-1.2.0/Monei/model/card.py
+-rw-r--r--   0 dmitriy    (501) staff       (20)    15438 2022-07-13 14:41:17.000000 Monei-1.2.0/Monei/model/confirm_payment_request.py
+-rw-r--r--   0 dmitriy    (501) staff       (20)    12743 2022-07-13 14:41:17.000000 Monei-1.2.0/Monei/model/confirm_payment_request_payment_method.py
+-rw-r--r--   0 dmitriy    (501) staff       (20)    12843 2022-07-13 14:41:17.000000 Monei-1.2.0/Monei/model/confirm_payment_request_payment_method_card.py
+-rw-r--r--   0 dmitriy    (501) staff       (20)    23645 2022-07-13 14:41:17.000000 Monei-1.2.0/Monei/model/create_payment_request.py
+-rw-r--r--   0 dmitriy    (501) staff       (20)    17318 2022-07-13 14:41:17.000000 Monei-1.2.0/Monei/model/create_subscription_request.py
+-rw-r--r--   0 dmitriy    (501) staff       (20)    12357 2022-07-13 14:41:17.000000 Monei-1.2.0/Monei/model/domain_register200_response.py
+-rw-r--r--   0 dmitriy    (501) staff       (20)    12532 2022-07-13 14:41:17.000000 Monei-1.2.0/Monei/model/error.py
+-rw-r--r--   0 dmitriy    (501) staff       (20)    12983 2022-07-13 14:41:17.000000 Monei-1.2.0/Monei/model/pause_subscription_request.py
+-rw-r--r--   0 dmitriy    (501) staff       (20)    24177 2022-07-13 14:41:17.000000 Monei-1.2.0/Monei/model/payment.py
+-rw-r--r--   0 dmitriy    (501) staff       (20)    13516 2022-07-13 14:41:17.000000 Monei-1.2.0/Monei/model/payment_billing_details.py
+-rw-r--r--   0 dmitriy    (501) staff       (20)    13224 2022-07-13 14:41:17.000000 Monei-1.2.0/Monei/model/payment_cancellation_reason.py
+-rw-r--r--   0 dmitriy    (501) staff       (20)    12897 2022-07-13 14:41:17.000000 Monei-1.2.0/Monei/model/payment_customer.py
+-rw-r--r--   0 dmitriy    (501) staff       (20)    13238 2022-07-13 14:41:17.000000 Monei-1.2.0/Monei/model/payment_last_refund_reason.py
+-rw-r--r--   0 dmitriy    (501) staff       (20)    13322 2022-07-13 14:41:17.000000 Monei-1.2.0/Monei/model/payment_message_channel.py
+-rw-r--r--   0 dmitriy    (501) staff       (20)    13501 2022-07-13 14:41:17.000000 Monei-1.2.0/Monei/model/payment_message_language.py
+-rw-r--r--   0 dmitriy    (501) staff       (20)    15115 2022-07-13 14:41:17.000000 Monei-1.2.0/Monei/model/payment_next_action.py
+-rw-r--r--   0 dmitriy    (501) staff       (20)    14350 2022-07-13 14:41:17.000000 Monei-1.2.0/Monei/model/payment_payment_method.py
+-rw-r--r--   0 dmitriy    (501) staff       (20)    12466 2022-07-13 14:41:17.000000 Monei-1.2.0/Monei/model/payment_payment_method_bizum.py
+-rw-r--r--   0 dmitriy    (501) staff       (20)    18413 2022-07-13 14:41:17.000000 Monei-1.2.0/Monei/model/payment_payment_method_card.py
+-rw-r--r--   0 dmitriy    (501) staff       (20)    12412 2022-07-13 14:41:17.000000 Monei-1.2.0/Monei/model/payment_payment_method_cofidis.py
+-rw-r--r--   0 dmitriy    (501) staff       (20)    12473 2022-07-13 14:41:17.000000 Monei-1.2.0/Monei/model/payment_payment_method_input.py
+-rw-r--r--   0 dmitriy    (501) staff       (20)    12409 2022-07-13 14:41:17.000000 Monei-1.2.0/Monei/model/payment_payment_method_paypal.py
+-rw-r--r--   0 dmitriy    (501) staff       (20)    13795 2022-07-13 14:41:17.000000 Monei-1.2.0/Monei/model/payment_payment_methods.py
+-rw-r--r--   0 dmitriy    (501) staff       (20)    13206 2022-07-13 14:41:17.000000 Monei-1.2.0/Monei/model/payment_refund_reason.py
+-rw-r--r--   0 dmitriy    (501) staff       (20)    13122 2022-07-13 14:41:17.000000 Monei-1.2.0/Monei/model/payment_sequence.py
+-rw-r--r--   0 dmitriy    (501) staff       (20)    13203 2022-07-13 14:41:17.000000 Monei-1.2.0/Monei/model/payment_sequence_recurring.py
+-rw-r--r--   0 dmitriy    (501) staff       (20)    17927 2022-07-13 14:41:17.000000 Monei-1.2.0/Monei/model/payment_session_details.py
+-rw-r--r--   0 dmitriy    (501) staff       (20)    13579 2022-07-13 14:41:17.000000 Monei-1.2.0/Monei/model/payment_shipping_details.py
+-rw-r--r--   0 dmitriy    (501) staff       (20)    12720 2022-07-13 14:41:17.000000 Monei-1.2.0/Monei/model/payment_shop.py
+-rw-r--r--   0 dmitriy    (501) staff       (20)    13516 2022-07-13 14:41:17.000000 Monei-1.2.0/Monei/model/payment_status.py
+-rw-r--r--   0 dmitriy    (501) staff       (20)    18518 2022-07-13 14:41:17.000000 Monei-1.2.0/Monei/model/payment_trace_details.py
+-rw-r--r--   0 dmitriy    (501) staff       (20)    13645 2022-07-13 14:41:17.000000 Monei-1.2.0/Monei/model/payment_transaction_type.py
+-rw-r--r--   0 dmitriy    (501) staff       (20)    16328 2022-07-13 14:41:17.000000 Monei-1.2.0/Monei/model/recurring_payment_request.py
+-rw-r--r--   0 dmitriy    (501) staff       (20)    13130 2022-07-13 14:41:17.000000 Monei-1.2.0/Monei/model/refund_payment_request.py
+-rw-r--r--   0 dmitriy    (501) staff       (20)    12531 2022-07-13 14:41:17.000000 Monei-1.2.0/Monei/model/register_domain_request.py
+-rw-r--r--   0 dmitriy    (501) staff       (20)    13760 2022-07-13 14:41:17.000000 Monei-1.2.0/Monei/model/send_payment_link_request.py
+-rw-r--r--   0 dmitriy    (501) staff       (20)    13791 2022-07-13 14:41:18.000000 Monei-1.2.0/Monei/model/send_payment_receipt_request.py
+-rw-r--r--   0 dmitriy    (501) staff       (20)    23663 2022-07-13 14:41:18.000000 Monei-1.2.0/Monei/model/subscription.py
+-rw-r--r--   0 dmitriy    (501) staff       (20)    13035 2022-07-13 14:41:18.000000 Monei-1.2.0/Monei/model/subscription_interval.py
+-rw-r--r--   0 dmitriy    (501) staff       (20)    13388 2022-07-13 14:41:18.000000 Monei-1.2.0/Monei/model/subscription_last_payment.py
+-rw-r--r--   0 dmitriy    (501) staff       (20)    13038 2022-07-13 14:41:18.000000 Monei-1.2.0/Monei/model/subscription_payment_method.py
+-rw-r--r--   0 dmitriy    (501) staff       (20)    14681 2022-07-13 14:41:18.000000 Monei-1.2.0/Monei/model/subscription_payment_method_card.py
+-rw-r--r--   0 dmitriy    (501) staff       (20)    13377 2022-07-13 14:41:18.000000 Monei-1.2.0/Monei/model/subscription_status.py
+-rw-r--r--   0 dmitriy    (501) staff       (20)    17444 2022-07-13 14:41:18.000000 Monei-1.2.0/Monei/model/update_subscription_request.py
+-rw-r--r--   0 dmitriy    (501) staff       (20)    83493 2022-07-13 14:41:18.000000 Monei-1.2.0/Monei/model_utils.py
+drwxr-xr-x   0 dmitriy    (501) staff       (20)        0 2023-05-18 16:43:58.207947 Monei-1.2.0/Monei/models/
+-rw-r--r--   0 dmitriy    (501) staff       (20)     4893 2023-05-18 16:43:52.000000 Monei-1.2.0/Monei/models/__init__.py
+-rw-r--r--   0 dmitriy    (501) staff       (20)    12134 2023-05-18 16:43:52.000000 Monei-1.2.0/Monei/models/activate_subscription_request.py
+-rw-r--r--   0 dmitriy    (501) staff       (20)     7862 2023-05-18 16:43:52.000000 Monei-1.2.0/Monei/models/address.py
+-rw-r--r--   0 dmitriy    (501) staff       (20)     4558 2023-05-18 16:43:52.000000 Monei-1.2.0/Monei/models/cancel_payment_request.py
+-rw-r--r--   0 dmitriy    (501) staff       (20)     4753 2023-05-18 16:43:52.000000 Monei-1.2.0/Monei/models/cancel_subscription_request.py
+-rw-r--r--   0 dmitriy    (501) staff       (20)     4555 2023-05-18 16:43:52.000000 Monei-1.2.0/Monei/models/capture_payment_request.py
+-rw-r--r--   0 dmitriy    (501) staff       (20)     8279 2022-09-30 14:39:33.000000 Monei-1.2.0/Monei/models/card.py
+-rw-r--r--   0 dmitriy    (501) staff       (20)     9669 2023-05-18 16:43:52.000000 Monei-1.2.0/Monei/models/confirm_payment_request.py
+-rw-r--r--   0 dmitriy    (501) staff       (20)     4410 2023-05-18 16:43:52.000000 Monei-1.2.0/Monei/models/confirm_payment_request_payment_method.py
+-rw-r--r--   0 dmitriy    (501) staff       (20)     5734 2023-05-18 16:43:52.000000 Monei-1.2.0/Monei/models/confirm_payment_request_payment_method_card.py
+-rw-r--r--   0 dmitriy    (501) staff       (20)    27742 2023-05-18 16:43:52.000000 Monei-1.2.0/Monei/models/create_payment_request.py
+-rw-r--r--   0 dmitriy    (501) staff       (20)    15584 2023-05-18 16:43:52.000000 Monei-1.2.0/Monei/models/create_subscription_request.py
+-rw-r--r--   0 dmitriy    (501) staff       (20)     4839 2023-05-18 16:43:52.000000 Monei-1.2.0/Monei/models/error.py
+-rw-r--r--   0 dmitriy    (501) staff       (20)     4192 2021-11-29 17:31:25.000000 Monei-1.2.0/Monei/models/inline_object.py
+-rw-r--r--   0 dmitriy    (501) staff       (20)     4232 2023-05-18 16:43:52.000000 Monei-1.2.0/Monei/models/inline_response200.py
+-rw-r--r--   0 dmitriy    (501) staff       (20)     5868 2023-05-18 16:43:52.000000 Monei-1.2.0/Monei/models/pause_subscription_request.py
+-rw-r--r--   0 dmitriy    (501) staff       (20)    29022 2023-05-18 16:43:52.000000 Monei-1.2.0/Monei/models/payment.py
+-rw-r--r--   0 dmitriy    (501) staff       (20)     7275 2023-05-18 16:43:52.000000 Monei-1.2.0/Monei/models/payment_billing_details.py
+-rw-r--r--   0 dmitriy    (501) staff       (20)     3843 2023-05-18 16:43:52.000000 Monei-1.2.0/Monei/models/payment_cancellation_reason.py
+-rw-r--r--   0 dmitriy    (501) staff       (20)     5719 2023-05-18 16:43:52.000000 Monei-1.2.0/Monei/models/payment_customer.py
+-rw-r--r--   0 dmitriy    (501) staff       (20)     3835 2023-05-18 16:43:52.000000 Monei-1.2.0/Monei/models/payment_last_refund_reason.py
+-rw-r--r--   0 dmitriy    (501) staff       (20)     3752 2023-05-18 16:43:52.000000 Monei-1.2.0/Monei/models/payment_message_channel.py
+-rw-r--r--   0 dmitriy    (501) staff       (20)     3798 2023-05-18 16:43:52.000000 Monei-1.2.0/Monei/models/payment_message_language.py
+-rw-r--r--   0 dmitriy    (501) staff       (20)     8566 2023-05-18 16:43:52.000000 Monei-1.2.0/Monei/models/payment_next_action.py
+-rw-r--r--   0 dmitriy    (501) staff       (20)     7551 2023-05-18 16:43:52.000000 Monei-1.2.0/Monei/models/payment_payment_method.py
+-rw-r--r--   0 dmitriy    (501) staff       (20)     4522 2023-05-18 16:43:52.000000 Monei-1.2.0/Monei/models/payment_payment_method_bizum.py
+-rw-r--r--   0 dmitriy    (501) staff       (20)     4562 2023-05-18 16:43:52.000000 Monei-1.2.0/Monei/models/payment_payment_method_bizum_input.py
+-rw-r--r--   0 dmitriy    (501) staff       (20)    17455 2023-05-18 16:43:52.000000 Monei-1.2.0/Monei/models/payment_payment_method_card.py
+-rw-r--r--   0 dmitriy    (501) staff       (20)     8968 2023-05-18 16:43:52.000000 Monei-1.2.0/Monei/models/payment_payment_method_card_input.py
+-rw-r--r--   0 dmitriy    (501) staff       (20)     4418 2023-05-18 16:43:52.000000 Monei-1.2.0/Monei/models/payment_payment_method_cofidis.py
+-rw-r--r--   0 dmitriy    (501) staff       (20)     5041 2023-05-18 16:43:52.000000 Monei-1.2.0/Monei/models/payment_payment_method_input.py
+-rw-r--r--   0 dmitriy    (501) staff       (20)     4410 2023-05-18 16:43:52.000000 Monei-1.2.0/Monei/models/payment_payment_method_paypal.py
+-rw-r--r--   0 dmitriy    (501) staff       (20)     3819 2023-05-18 16:43:52.000000 Monei-1.2.0/Monei/models/payment_refund_reason.py
+-rw-r--r--   0 dmitriy    (501) staff       (20)     5395 2023-05-18 16:43:52.000000 Monei-1.2.0/Monei/models/payment_sequence.py
+-rw-r--r--   0 dmitriy    (501) staff       (20)     5463 2023-05-18 16:43:52.000000 Monei-1.2.0/Monei/models/payment_sequence_recurring.py
+-rw-r--r--   0 dmitriy    (501) staff       (20)    19485 2023-05-18 16:43:52.000000 Monei-1.2.0/Monei/models/payment_session_details.py
+-rw-r--r--   0 dmitriy    (501) staff       (20)     7359 2023-05-18 16:43:52.000000 Monei-1.2.0/Monei/models/payment_shipping_details.py
+-rw-r--r--   0 dmitriy    (501) staff       (20)     5068 2023-05-18 16:43:52.000000 Monei-1.2.0/Monei/models/payment_shop.py
+-rw-r--r--   0 dmitriy    (501) staff       (20)     3951 2023-05-18 16:43:52.000000 Monei-1.2.0/Monei/models/payment_status.py
+-rw-r--r--   0 dmitriy    (501) staff       (20)    21011 2023-05-18 16:43:52.000000 Monei-1.2.0/Monei/models/payment_trace_details.py
+-rw-r--r--   0 dmitriy    (501) staff       (20)     3750 2023-05-18 16:43:52.000000 Monei-1.2.0/Monei/models/payment_transaction_type.py
+-rw-r--r--   0 dmitriy    (501) staff       (20)    11637 2023-05-18 16:43:52.000000 Monei-1.2.0/Monei/models/recurring_payment_request.py
+-rw-r--r--   0 dmitriy    (501) staff       (20)     5273 2023-05-18 16:43:52.000000 Monei-1.2.0/Monei/models/refund_payment_request.py
+-rw-r--r--   0 dmitriy    (501) staff       (20)     4631 2023-05-18 16:43:52.000000 Monei-1.2.0/Monei/models/register_domain_request.py
+-rw-r--r--   0 dmitriy    (501) staff       (20)     7103 2023-05-18 16:43:52.000000 Monei-1.2.0/Monei/models/send_payment_link_request.py
+-rw-r--r--   0 dmitriy    (501) staff       (20)     7185 2023-05-18 16:43:52.000000 Monei-1.2.0/Monei/models/send_payment_receipt_request.py
+-rw-r--r--   0 dmitriy    (501) staff       (20)     5462 2023-05-18 16:43:52.000000 Monei-1.2.0/Monei/models/send_payment_request.py
+-rw-r--r--   0 dmitriy    (501) staff       (20)    30159 2023-05-18 16:43:52.000000 Monei-1.2.0/Monei/models/subscription.py
+-rw-r--r--   0 dmitriy    (501) staff       (20)     3760 2023-05-18 16:43:52.000000 Monei-1.2.0/Monei/models/subscription_interval.py
+-rw-r--r--   0 dmitriy    (501) staff       (20)     6814 2023-05-18 16:43:52.000000 Monei-1.2.0/Monei/models/subscription_last_payment.py
+-rw-r--r--   0 dmitriy    (501) staff       (20)     5398 2023-05-18 16:43:52.000000 Monei-1.2.0/Monei/models/subscription_payment_method.py
+-rw-r--r--   0 dmitriy    (501) staff       (20)    10663 2023-05-18 16:43:52.000000 Monei-1.2.0/Monei/models/subscription_payment_method_card.py
+-rw-r--r--   0 dmitriy    (501) staff       (20)     3890 2023-05-18 16:43:52.000000 Monei-1.2.0/Monei/models/subscription_status.py
+-rw-r--r--   0 dmitriy    (501) staff       (20)    16537 2023-05-18 16:43:52.000000 Monei-1.2.0/Monei/models/update_subscription_request.py
+-rw-r--r--   0 dmitriy    (501) staff       (20)     1732 2023-03-15 16:02:53.000000 Monei-1.2.0/Monei/monei_client.py
+-rw-r--r--   0 dmitriy    (501) staff       (20)    13190 2023-05-18 16:43:52.000000 Monei-1.2.0/Monei/rest.py
+drwxr-xr-x   0 dmitriy    (501) staff       (20)        0 2023-05-18 16:43:58.153129 Monei-1.2.0/Monei.egg-info/
+-rw-r--r--   0 dmitriy    (501) staff       (20)      755 2023-05-18 16:43:58.000000 Monei-1.2.0/Monei.egg-info/PKG-INFO
+-rw-r--r--   0 dmitriy    (501) staff       (20)     6669 2023-05-18 16:43:58.000000 Monei-1.2.0/Monei.egg-info/SOURCES.txt
+-rw-r--r--   0 dmitriy    (501) staff       (20)        1 2023-05-18 16:43:58.000000 Monei-1.2.0/Monei.egg-info/dependency_links.txt
+-rw-r--r--   0 dmitriy    (501) staff       (20)       48 2023-05-18 16:43:58.000000 Monei-1.2.0/Monei.egg-info/requires.txt
+-rw-r--r--   0 dmitriy    (501) staff       (20)        6 2023-05-18 16:43:58.000000 Monei-1.2.0/Monei.egg-info/top_level.txt
+-rw-r--r--   0 dmitriy    (501) staff       (20)      755 2023-05-18 16:43:58.242077 Monei-1.2.0/PKG-INFO
+-rw-r--r--   0 dmitriy    (501) staff       (20)     2379 2022-02-04 13:50:42.000000 Monei-1.2.0/README.md
+-rw-r--r--   0 dmitriy    (501) staff       (20)      128 2023-05-18 16:43:58.242486 Monei-1.2.0/setup.cfg
+-rw-r--r--   0 dmitriy    (501) staff       (20)     1304 2021-11-29 17:24:51.000000 Monei-1.2.0/setup.py
+drwxr-xr-x   0 dmitriy    (501) staff       (20)        0 2023-05-18 16:43:58.241637 Monei-1.2.0/test/
+-rw-r--r--   0 dmitriy    (501) staff       (20)     2539 2021-11-16 18:37:45.000000 Monei-1.2.0/test/test_activate_subscription_request.py
+-rw-r--r--   0 dmitriy    (501) staff       (20)     1699 2021-06-21 18:57:48.000000 Monei-1.2.0/test/test_address.py
+-rw-r--r--   0 dmitriy    (501) staff       (20)     1509 2021-11-16 18:37:46.000000 Monei-1.2.0/test/test_apple_pay_domain_api.py
+-rw-r--r--   0 dmitriy    (501) staff       (20)     1690 2021-06-21 18:57:48.000000 Monei-1.2.0/test/test_cancel_payment_request.py
+-rw-r--r--   0 dmitriy    (501) staff       (20)     2167 2021-11-16 18:37:45.000000 Monei-1.2.0/test/test_cancel_subscription_request.py
+-rw-r--r--   0 dmitriy    (501) staff       (20)     1680 2021-06-21 18:57:48.000000 Monei-1.2.0/test/test_capture_payment_request.py
+-rw-r--r--   0 dmitriy    (501) staff       (20)     1583 2021-06-21 18:57:48.000000 Monei-1.2.0/test/test_card.py
+-rw-r--r--   0 dmitriy    (501) staff       (20)     3205 2021-06-21 18:57:48.000000 Monei-1.2.0/test/test_confirm_payment_request.py
+-rw-r--r--   0 dmitriy    (501) staff       (20)     2370 2021-06-21 18:57:48.000000 Monei-1.2.0/test/test_confirm_payment_request_payment_method.py
+-rw-r--r--   0 dmitriy    (501) staff       (20)     2283 2021-06-21 18:57:48.000000 Monei-1.2.0/test/test_confirm_payment_request_payment_method_card.py
+-rw-r--r--   0 dmitriy    (501) staff       (20)     5396 2021-06-21 18:57:48.000000 Monei-1.2.0/test/test_create_payment_request.py
+-rw-r--r--   0 dmitriy    (501) staff       (20)     4226 2021-11-16 18:37:45.000000 Monei-1.2.0/test/test_create_subscription_request.py
+-rw-r--r--   0 dmitriy    (501) staff       (20)     1734 2022-07-13 14:41:17.000000 Monei-1.2.0/test/test_domain_register200_response.py
+-rw-r--r--   0 dmitriy    (501) staff       (20)     1559 2021-06-21 18:57:48.000000 Monei-1.2.0/test/test_error.py
+-rw-r--r--   0 dmitriy    (501) staff       (20)     2021 2021-11-16 18:37:45.000000 Monei-1.2.0/test/test_inline_object.py
+-rw-r--r--   0 dmitriy    (501) staff       (20)     2063 2021-11-16 18:37:45.000000 Monei-1.2.0/test/test_inline_response200.py
+-rw-r--r--   0 dmitriy    (501) staff       (20)     2198 2021-11-16 18:37:45.000000 Monei-1.2.0/test/test_pause_subscription_request.py
+-rw-r--r--   0 dmitriy    (501) staff       (20)     6369 2021-07-07 16:22:19.000000 Monei-1.2.0/test/test_payment.py
+-rw-r--r--   0 dmitriy    (501) staff       (20)     2100 2021-06-21 18:57:48.000000 Monei-1.2.0/test/test_payment_billing_details.py
+-rw-r--r--   0 dmitriy    (501) staff       (20)     1694 2021-06-21 18:57:48.000000 Monei-1.2.0/test/test_payment_cancellation_reason.py
+-rw-r--r--   0 dmitriy    (501) staff       (20)     1697 2021-06-21 18:57:48.000000 Monei-1.2.0/test/test_payment_customer.py
+-rw-r--r--   0 dmitriy    (501) staff       (20)     1674 2021-06-21 18:57:48.000000 Monei-1.2.0/test/test_payment_last_refund_reason.py
+-rw-r--r--   0 dmitriy    (501) staff       (20)     2314 2022-07-12 17:04:01.000000 Monei-1.2.0/test/test_payment_message_channel.py
+-rw-r--r--   0 dmitriy    (501) staff       (20)     2325 2022-07-12 17:04:01.000000 Monei-1.2.0/test/test_payment_message_language.py
+-rw-r--r--   0 dmitriy    (501) staff       (20)     1779 2021-07-07 16:22:19.000000 Monei-1.2.0/test/test_payment_next_action.py
+-rw-r--r--   0 dmitriy    (501) staff       (20)     2322 2021-06-21 18:57:48.000000 Monei-1.2.0/test/test_payment_payment_method.py
+-rw-r--r--   0 dmitriy    (501) staff       (20)     1731 2021-06-21 18:57:48.000000 Monei-1.2.0/test/test_payment_payment_method_bizum.py
+-rw-r--r--   0 dmitriy    (501) staff       (20)     2452 2023-02-02 16:12:19.000000 Monei-1.2.0/test/test_payment_payment_method_bizum_input.py
+-rw-r--r--   0 dmitriy    (501) staff       (20)     1908 2021-06-21 18:57:48.000000 Monei-1.2.0/test/test_payment_payment_method_card.py
+-rw-r--r--   0 dmitriy    (501) staff       (20)     2635 2023-02-02 16:12:20.000000 Monei-1.2.0/test/test_payment_payment_method_card_input.py
+-rw-r--r--   0 dmitriy    (501) staff       (20)     2177 2021-11-16 18:37:45.000000 Monei-1.2.0/test/test_payment_payment_method_cofidis.py
+-rw-r--r--   0 dmitriy    (501) staff       (20)     1897 2021-06-21 18:57:48.000000 Monei-1.2.0/test/test_payment_payment_method_input.py
+-rw-r--r--   0 dmitriy    (501) staff       (20)     1738 2021-06-21 18:57:48.000000 Monei-1.2.0/test/test_payment_payment_method_paypal.py
+-rw-r--r--   0 dmitriy    (501) staff       (20)     1706 2022-07-13 14:41:17.000000 Monei-1.2.0/test/test_payment_payment_methods.py
+-rw-r--r--   0 dmitriy    (501) staff       (20)     1628 2021-06-21 18:57:48.000000 Monei-1.2.0/test/test_payment_refund_reason.py
+-rw-r--r--   0 dmitriy    (501) staff       (20)     1874 2021-06-21 18:57:48.000000 Monei-1.2.0/test/test_payment_sequence.py
+-rw-r--r--   0 dmitriy    (501) staff       (20)     1785 2021-06-21 18:57:48.000000 Monei-1.2.0/test/test_payment_sequence_recurring.py
+-rw-r--r--   0 dmitriy    (501) staff       (20)     2159 2021-06-21 18:57:48.000000 Monei-1.2.0/test/test_payment_session_details.py
+-rw-r--r--   0 dmitriy    (501) staff       (20)     2111 2021-06-21 18:57:48.000000 Monei-1.2.0/test/test_payment_shipping_details.py
+-rw-r--r--   0 dmitriy    (501) staff       (20)     1606 2021-06-21 18:57:48.000000 Monei-1.2.0/test/test_payment_shop.py
+-rw-r--r--   0 dmitriy    (501) staff       (20)     1560 2021-06-21 18:57:48.000000 Monei-1.2.0/test/test_payment_status.py
+-rw-r--r--   0 dmitriy    (501) staff       (20)     2219 2021-06-21 18:57:48.000000 Monei-1.2.0/test/test_payment_trace_details.py
+-rw-r--r--   0 dmitriy    (501) staff       (20)     1661 2021-06-21 18:57:48.000000 Monei-1.2.0/test/test_payment_transaction_type.py
+-rw-r--r--   0 dmitriy    (501) staff       (20)     1787 2021-06-21 18:57:48.000000 Monei-1.2.0/test/test_payments_api.py
+-rw-r--r--   0 dmitriy    (501) staff       (20)     3401 2021-06-21 18:57:48.000000 Monei-1.2.0/test/test_recurring_payment_request.py
+-rw-r--r--   0 dmitriy    (501) staff       (20)     1716 2021-06-21 18:57:48.000000 Monei-1.2.0/test/test_refund_payment_request.py
+-rw-r--r--   0 dmitriy    (501) staff       (20)     2184 2021-11-29 17:46:51.000000 Monei-1.2.0/test/test_register_domain_request.py
+-rw-r--r--   0 dmitriy    (501) staff       (20)     2198 2022-03-28 15:38:14.000000 Monei-1.2.0/test/test_send_payment_link_request.py
+-rw-r--r--   0 dmitriy    (501) staff       (20)     2231 2022-03-28 15:38:14.000000 Monei-1.2.0/test/test_send_payment_receipt_request.py
+-rw-r--r--   0 dmitriy    (501) staff       (20)     2350 2023-05-18 16:23:08.000000 Monei-1.2.0/test/test_send_payment_request.py
+-rw-r--r--   0 dmitriy    (501) staff       (20)     6061 2021-11-16 18:37:45.000000 Monei-1.2.0/test/test_subscription.py
+-rw-r--r--   0 dmitriy    (501) staff       (20)     2065 2021-11-16 18:37:45.000000 Monei-1.2.0/test/test_subscription_interval.py
+-rw-r--r--   0 dmitriy    (501) staff       (20)     2268 2021-11-16 18:37:45.000000 Monei-1.2.0/test/test_subscription_last_payment.py
+-rw-r--r--   0 dmitriy    (501) staff       (20)     2543 2021-11-16 18:37:45.000000 Monei-1.2.0/test/test_subscription_payment_method.py
+-rw-r--r--   0 dmitriy    (501) staff       (20)     2433 2021-11-16 18:37:45.000000 Monei-1.2.0/test/test_subscription_payment_method_card.py
+-rw-r--r--   0 dmitriy    (501) staff       (20)     2043 2021-11-16 18:37:45.000000 Monei-1.2.0/test/test_subscription_status.py
+-rw-r--r--   0 dmitriy    (501) staff       (20)     2268 2021-11-16 18:37:46.000000 Monei-1.2.0/test/test_subscriptions_api.py
+-rw-r--r--   0 dmitriy    (501) staff       (20)     3994 2021-11-16 18:37:45.000000 Monei-1.2.0/test/test_update_subscription_request.py
```

### Comparing `Monei-1.1.3/Monei/__init__.py` & `Monei-1.2.0/Monei/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 # coding: utf-8
 
 # flake8: noqa
 
 """
     MONEI API v1
 
-    <p>The MONEI API is organized around <a href=\"https://en.wikipedia.org/wiki/Representational_State_Transfer\">REST</a>. Our API has predictable resource-oriented URLs, accepts JSON-encoded request bodies, returns JSON-encoded responses, and uses standard HTTP response codes, authentication, and verbs.</p> <h4 id=\"base-url\">Base URL:</h4> <p><a href=\"https://api.monei.com/v1\">https://api.monei.com/v1</a></p> <h4 id=\"client-libraries\">Client libraries:</h4> <ul> <li><a href=\"https://github.com/MONEI/monei-php-sdk\">PHP SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-python-sdk\">Python SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-node-sdk\">Node.js SDK</a></li> <li><a href=\"https://postman.monei.com/\">Postman Collection</a></li> </ul> <h4 id=\"important\">Important:</h4> <p><strong>If you are not using our official SDKs, you need to provide a valid <code>User-Agent</code> header in each request, otherwise your requests will be rejected.</strong></p>   # noqa: E501
+    <p>The MONEI API is organized around <a href=\"https://en.wikipedia.org/wiki/Representational_State_Transfer\">REST</a>. Our API has predictable resource-oriented URLs, accepts JSON-encoded request bodies, returns JSON-encoded responses, and uses standard HTTP response codes, authentication, and verbs.</p> <h4 id=\"base-url\">Base URL:</h4> <p><a href=\"https://api.monei.com/v1\">https://api.monei.com/v1</a></p> <h4 id=\"client-libraries\">Client libraries:</h4> <ul> <li><a href=\"https://github.com/MONEI/monei-php-sdk\">PHP SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-python-sdk\">Python SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-node-sdk\">Node.js SDK</a></li> <li><a href=\"https://postman.monei.com/\">Postman</a></li> </ul> <h4 id=\"important\">Important:</h4> <p><strong>If you are not using our official SDKs, you need to provide a valid <code>User-Agent</code> header in each request, otherwise your requests will be rejected.</strong></p>   # noqa: E501
 
-    The version of the OpenAPI document: 1.3.3
+    The version of the OpenAPI document: 1.4.0
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
-__version__ = "1.1.3"
+__version__ = "1.2.0"
 
 # import apis into sdk package
 from Monei.api.apple_pay_domain_api import ApplePayDomainApi
 from Monei.api.payments_api import PaymentsApi
 from Monei.api.subscriptions_api import SubscriptionsApi
 
 # import ApiClient
@@ -69,14 +69,15 @@
 from Monei.models.payment_trace_details import PaymentTraceDetails
 from Monei.models.payment_transaction_type import PaymentTransactionType
 from Monei.models.recurring_payment_request import RecurringPaymentRequest
 from Monei.models.refund_payment_request import RefundPaymentRequest
 from Monei.models.register_domain_request import RegisterDomainRequest
 from Monei.models.send_payment_link_request import SendPaymentLinkRequest
 from Monei.models.send_payment_receipt_request import SendPaymentReceiptRequest
+from Monei.models.send_payment_request import SendPaymentRequest
 from Monei.models.subscription import Subscription
 from Monei.models.subscription_interval import SubscriptionInterval
 from Monei.models.subscription_last_payment import SubscriptionLastPayment
 from Monei.models.subscription_payment_method import SubscriptionPaymentMethod
 from Monei.models.subscription_payment_method_card import SubscriptionPaymentMethodCard
 from Monei.models.subscription_status import SubscriptionStatus
 from Monei.models.update_subscription_request import UpdateSubscriptionRequest
```

#### html2text {}

```diff
@@ -4,21 +4,21 @@
 responses, and uses standard HTTP response codes, authentication, and verbs.
 *** Base URL: ***
 https://api.monei.com/v1
 *** Client libraries: ***
     * PHP_SDK
     * Python_SDK
     * Node.js_SDK
-    * Postman_Collection
+    * Postman
 *** Important: ***
 If you are not using our official SDKs, you need to provide a valid User-Agent
 header in each request, otherwise your requests will be rejected.
-# noqa: E501 The version of the OpenAPI document: 1.3.3 Generated by: https://
+# noqa: E501 The version of the OpenAPI document: 1.4.0 Generated by: https://
 openapi-generator.tech """ from __future__ import absolute_import __version__ =
-"1.1.3" # import apis into sdk package from Monei.api.apple_pay_domain_api
+"1.2.0" # import apis into sdk package from Monei.api.apple_pay_domain_api
 import ApplePayDomainApi from Monei.api.payments_api import PaymentsApi from
 Monei.api.subscriptions_api import SubscriptionsApi # import ApiClient from
 Monei.api_client import ApiClient from Monei.configuration import Configuration
 from Monei.exceptions import OpenApiException from Monei.exceptions import
 ApiTypeError from Monei.exceptions import ApiValueError from Monei.exceptions
 import ApiKeyError from Monei.exceptions import ApiException # import models
 into sdk package from Monei.models.activate_subscription_request import
@@ -61,16 +61,17 @@
 import PaymentStatus from Monei.models.payment_trace_details import
 PaymentTraceDetails from Monei.models.payment_transaction_type import
 PaymentTransactionType from Monei.models.recurring_payment_request import
 RecurringPaymentRequest from Monei.models.refund_payment_request import
 RefundPaymentRequest from Monei.models.register_domain_request import
 RegisterDomainRequest from Monei.models.send_payment_link_request import
 SendPaymentLinkRequest from Monei.models.send_payment_receipt_request import
-SendPaymentReceiptRequest from Monei.models.subscription import Subscription
-from Monei.models.subscription_interval import SubscriptionInterval from
+SendPaymentReceiptRequest from Monei.models.send_payment_request import
+SendPaymentRequest from Monei.models.subscription import Subscription from
+Monei.models.subscription_interval import SubscriptionInterval from
 Monei.models.subscription_last_payment import SubscriptionLastPayment from
 Monei.models.subscription_payment_method import SubscriptionPaymentMethod from
 Monei.models.subscription_payment_method_card import
 SubscriptionPaymentMethodCard from Monei.models.subscription_status import
 SubscriptionStatus from Monei.models.update_subscription_request import
 UpdateSubscriptionRequest # import custom MoneiClient from Monei.monei_client
 import MoneiClient
```

### Comparing `Monei-1.1.3/Monei/api/apple_pay_domain_api.py` & `Monei-1.2.0/Monei/api/apple_pay_domain_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     MONEI API v1
 
-    <p>The MONEI API is organized around <a href=\"https://en.wikipedia.org/wiki/Representational_State_Transfer\">REST</a>. Our API has predictable resource-oriented URLs, accepts JSON-encoded request bodies, returns JSON-encoded responses, and uses standard HTTP response codes, authentication, and verbs.</p> <h4 id=\"base-url\">Base URL:</h4> <p><a href=\"https://api.monei.com/v1\">https://api.monei.com/v1</a></p> <h4 id=\"client-libraries\">Client libraries:</h4> <ul> <li><a href=\"https://github.com/MONEI/monei-php-sdk\">PHP SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-python-sdk\">Python SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-node-sdk\">Node.js SDK</a></li> <li><a href=\"https://postman.monei.com/\">Postman Collection</a></li> </ul> <h4 id=\"important\">Important:</h4> <p><strong>If you are not using our official SDKs, you need to provide a valid <code>User-Agent</code> header in each request, otherwise your requests will be rejected.</strong></p>   # noqa: E501
+    <p>The MONEI API is organized around <a href=\"https://en.wikipedia.org/wiki/Representational_State_Transfer\">REST</a>. Our API has predictable resource-oriented URLs, accepts JSON-encoded request bodies, returns JSON-encoded responses, and uses standard HTTP response codes, authentication, and verbs.</p> <h4 id=\"base-url\">Base URL:</h4> <p><a href=\"https://api.monei.com/v1\">https://api.monei.com/v1</a></p> <h4 id=\"client-libraries\">Client libraries:</h4> <ul> <li><a href=\"https://github.com/MONEI/monei-php-sdk\">PHP SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-python-sdk\">Python SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-node-sdk\">Node.js SDK</a></li> <li><a href=\"https://postman.monei.com/\">Postman</a></li> </ul> <h4 id=\"important\">Important:</h4> <p><strong>If you are not using our official SDKs, you need to provide a valid <code>User-Agent</code> header in each request, otherwise your requests will be rejected.</strong></p>   # noqa: E501
 
-    The version of the OpenAPI document: 1.3.3
+    The version of the OpenAPI document: 1.4.0
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import re  # noqa: F401
```

### Comparing `Monei-1.1.3/Monei/api/payments_api.py` & `Monei-1.2.0/Monei/api/payments_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     MONEI API v1
 
-    <p>The MONEI API is organized around <a href=\"https://en.wikipedia.org/wiki/Representational_State_Transfer\">REST</a>. Our API has predictable resource-oriented URLs, accepts JSON-encoded request bodies, returns JSON-encoded responses, and uses standard HTTP response codes, authentication, and verbs.</p> <h4 id=\"base-url\">Base URL:</h4> <p><a href=\"https://api.monei.com/v1\">https://api.monei.com/v1</a></p> <h4 id=\"client-libraries\">Client libraries:</h4> <ul> <li><a href=\"https://github.com/MONEI/monei-php-sdk\">PHP SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-python-sdk\">Python SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-node-sdk\">Node.js SDK</a></li> <li><a href=\"https://postman.monei.com/\">Postman Collection</a></li> </ul> <h4 id=\"important\">Important:</h4> <p><strong>If you are not using our official SDKs, you need to provide a valid <code>User-Agent</code> header in each request, otherwise your requests will be rejected.</strong></p>   # noqa: E501
+    <p>The MONEI API is organized around <a href=\"https://en.wikipedia.org/wiki/Representational_State_Transfer\">REST</a>. Our API has predictable resource-oriented URLs, accepts JSON-encoded request bodies, returns JSON-encoded responses, and uses standard HTTP response codes, authentication, and verbs.</p> <h4 id=\"base-url\">Base URL:</h4> <p><a href=\"https://api.monei.com/v1\">https://api.monei.com/v1</a></p> <h4 id=\"client-libraries\">Client libraries:</h4> <ul> <li><a href=\"https://github.com/MONEI/monei-php-sdk\">PHP SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-python-sdk\">Python SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-node-sdk\">Node.js SDK</a></li> <li><a href=\"https://postman.monei.com/\">Postman</a></li> </ul> <h4 id=\"important\">Important:</h4> <p><strong>If you are not using our official SDKs, you need to provide a valid <code>User-Agent</code> header in each request, otherwise your requests will be rejected.</strong></p>   # noqa: E501
 
-    The version of the OpenAPI document: 1.3.3
+    The version of the OpenAPI document: 1.4.0
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import re  # noqa: F401
@@ -1118,13 +1118,140 @@
             path_params,
             query_params,
             header_params,
             body=body_params,
             post_params=form_params,
             files=local_var_files,
             response_type='Payment',  # noqa: E501
+            auth_settings=auth_settings,
+            async_req=local_var_params.get('async_req'),
+            _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
+            _preload_content=local_var_params.get('_preload_content', True),
+            _request_timeout=local_var_params.get('_request_timeout'),
+            collection_formats=collection_formats)
+
+    def send_request(self, id, send_payment_request, **kwargs):  # noqa: E501
+        """Send Payment Request  # noqa: E501
+
+        Sends a payment request directly to the customer's phone. If Bizum payment method is available and the phone number is registered in Bizum, the customer will get a push notification to confirm the payment directly in the banking app, otherwise, he will receive a link to pay via WhatsApp.   # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.send_request(id, send_payment_request, async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool: execute request asynchronously
+        :param str id: The payment ID (required)
+        :param SendPaymentRequest send_payment_request: (required)
+        :param _preload_content: if False, the urllib3.HTTPResponse object will
+                                 be returned without reading/decoding response
+                                 data. Default is True.
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :return: Payment
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+        kwargs['_return_http_data_only'] = True
+        return self.send_request_with_http_info(id, send_payment_request, **kwargs)  # noqa: E501
+
+    def send_request_with_http_info(self, id, send_payment_request, **kwargs):  # noqa: E501
+        """Send Payment Request  # noqa: E501
+
+        Sends a payment request directly to the customer's phone. If Bizum payment method is available and the phone number is registered in Bizum, the customer will get a push notification to confirm the payment directly in the banking app, otherwise, he will receive a link to pay via WhatsApp.   # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.send_request_with_http_info(id, send_payment_request, async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool: execute request asynchronously
+        :param str id: The payment ID (required)
+        :param SendPaymentRequest send_payment_request: (required)
+        :param _return_http_data_only: response data without head status code
+                                       and headers
+        :param _preload_content: if False, the urllib3.HTTPResponse object will
+                                 be returned without reading/decoding response
+                                 data. Default is True.
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :return: tuple(Payment, status_code(int), headers(HTTPHeaderDict))
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+
+        local_var_params = locals()
+
+        all_params = [
+            'id',
+            'send_payment_request'
+        ]
+        all_params.extend(
+            [
+                'async_req',
+                '_return_http_data_only',
+                '_preload_content',
+                '_request_timeout'
+            ]
+        )
+
+        for key, val in six.iteritems(local_var_params['kwargs']):
+            if key not in all_params:
+                raise ApiTypeError(
+                    "Got an unexpected keyword argument '%s'"
+                    " to method send_request" % key
+                )
+            local_var_params[key] = val
+        del local_var_params['kwargs']
+        # verify the required parameter 'id' is set
+        if self.api_client.client_side_validation and ('id' not in local_var_params or  # noqa: E501
+                                                        local_var_params['id'] is None):  # noqa: E501
+            raise ApiValueError("Missing the required parameter `id` when calling `send_request`")  # noqa: E501
+        # verify the required parameter 'send_payment_request' is set
+        if self.api_client.client_side_validation and ('send_payment_request' not in local_var_params or  # noqa: E501
+                                                        local_var_params['send_payment_request'] is None):  # noqa: E501
+            raise ApiValueError("Missing the required parameter `send_payment_request` when calling `send_request`")  # noqa: E501
+
+        collection_formats = {}
+
+        path_params = {}
+        if 'id' in local_var_params:
+            path_params['id'] = local_var_params['id']  # noqa: E501
+
+        query_params = []
+
+        header_params = {}
+
+        form_params = []
+        local_var_files = {}
+
+        body_params = None
+        if 'send_payment_request' in local_var_params:
+            body_params = local_var_params['send_payment_request']
+        # HTTP header `Accept`
+        header_params['Accept'] = self.api_client.select_header_accept(
+            ['application/json'])  # noqa: E501
+
+        # HTTP header `Content-Type`
+        header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
+            ['application/json'])  # noqa: E501
+
+        # Authentication setting
+        auth_settings = ['APIKey']  # noqa: E501
+
+        return self.api_client.call_api(
+            '/payments/{id}/rtp', 'POST',
+            path_params,
+            query_params,
+            header_params,
+            body=body_params,
+            post_params=form_params,
+            files=local_var_files,
+            response_type='Payment',  # noqa: E501
             auth_settings=auth_settings,
             async_req=local_var_params.get('async_req'),
             _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=local_var_params.get('_preload_content', True),
             _request_timeout=local_var_params.get('_request_timeout'),
             collection_formats=collection_formats)
```

### Comparing `Monei-1.1.3/Monei/api/subscriptions_api.py` & `Monei-1.2.0/Monei/api/subscriptions_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     MONEI API v1
 
-    <p>The MONEI API is organized around <a href=\"https://en.wikipedia.org/wiki/Representational_State_Transfer\">REST</a>. Our API has predictable resource-oriented URLs, accepts JSON-encoded request bodies, returns JSON-encoded responses, and uses standard HTTP response codes, authentication, and verbs.</p> <h4 id=\"base-url\">Base URL:</h4> <p><a href=\"https://api.monei.com/v1\">https://api.monei.com/v1</a></p> <h4 id=\"client-libraries\">Client libraries:</h4> <ul> <li><a href=\"https://github.com/MONEI/monei-php-sdk\">PHP SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-python-sdk\">Python SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-node-sdk\">Node.js SDK</a></li> <li><a href=\"https://postman.monei.com/\">Postman Collection</a></li> </ul> <h4 id=\"important\">Important:</h4> <p><strong>If you are not using our official SDKs, you need to provide a valid <code>User-Agent</code> header in each request, otherwise your requests will be rejected.</strong></p>   # noqa: E501
+    <p>The MONEI API is organized around <a href=\"https://en.wikipedia.org/wiki/Representational_State_Transfer\">REST</a>. Our API has predictable resource-oriented URLs, accepts JSON-encoded request bodies, returns JSON-encoded responses, and uses standard HTTP response codes, authentication, and verbs.</p> <h4 id=\"base-url\">Base URL:</h4> <p><a href=\"https://api.monei.com/v1\">https://api.monei.com/v1</a></p> <h4 id=\"client-libraries\">Client libraries:</h4> <ul> <li><a href=\"https://github.com/MONEI/monei-php-sdk\">PHP SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-python-sdk\">Python SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-node-sdk\">Node.js SDK</a></li> <li><a href=\"https://postman.monei.com/\">Postman</a></li> </ul> <h4 id=\"important\">Important:</h4> <p><strong>If you are not using our official SDKs, you need to provide a valid <code>User-Agent</code> header in each request, otherwise your requests will be rejected.</strong></p>   # noqa: E501
 
-    The version of the OpenAPI document: 1.3.3
+    The version of the OpenAPI document: 1.4.0
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import re  # noqa: F401
```

### Comparing `Monei-1.1.3/Monei/api_client.py` & `Monei-1.2.0/Monei/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # coding: utf-8
 """
     MONEI API v1
 
-    <p>The MONEI API is organized around <a href=\"https://en.wikipedia.org/wiki/Representational_State_Transfer\">REST</a>. Our API has predictable resource-oriented URLs, accepts JSON-encoded request bodies, returns JSON-encoded responses, and uses standard HTTP response codes, authentication, and verbs.</p> <h4 id=\"base-url\">Base URL:</h4> <p><a href=\"https://api.monei.com/v1\">https://api.monei.com/v1</a></p> <h4 id=\"client-libraries\">Client libraries:</h4> <ul> <li><a href=\"https://github.com/MONEI/monei-php-sdk\">PHP SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-python-sdk\">Python SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-node-sdk\">Node.js SDK</a></li> <li><a href=\"https://postman.monei.com/\">Postman Collection</a></li> </ul> <h4 id=\"important\">Important:</h4> <p><strong>If you are not using our official SDKs, you need to provide a valid <code>User-Agent</code> header in each request, otherwise your requests will be rejected.</strong></p>   # noqa: E501
+    <p>The MONEI API is organized around <a href=\"https://en.wikipedia.org/wiki/Representational_State_Transfer\">REST</a>. Our API has predictable resource-oriented URLs, accepts JSON-encoded request bodies, returns JSON-encoded responses, and uses standard HTTP response codes, authentication, and verbs.</p> <h4 id=\"base-url\">Base URL:</h4> <p><a href=\"https://api.monei.com/v1\">https://api.monei.com/v1</a></p> <h4 id=\"client-libraries\">Client libraries:</h4> <ul> <li><a href=\"https://github.com/MONEI/monei-php-sdk\">PHP SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-python-sdk\">Python SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-node-sdk\">Node.js SDK</a></li> <li><a href=\"https://postman.monei.com/\">Postman</a></li> </ul> <h4 id=\"important\">Important:</h4> <p><strong>If you are not using our official SDKs, you need to provide a valid <code>User-Agent</code> header in each request, otherwise your requests will be rejected.</strong></p>   # noqa: E501
 
-    The version of the OpenAPI document: 1.3.3
+    The version of the OpenAPI document: 1.4.0
     Generated by: https://openapi-generator.tech
 """
 
 from __future__ import absolute_import
 
 import atexit
 import datetime
@@ -74,15 +74,15 @@
 
         self.rest_client = rest.RESTClientObject(configuration)
         self.default_headers = {}
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = 'OpenAPI-Generator/1.1.3/python'
+        self.user_agent = 'OpenAPI-Generator/1.2.0/python'
         self.client_side_validation = configuration.client_side_validation
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         self.close()
```

### Comparing `Monei-1.1.3/Monei/apis/__init__.py` & `Monei-1.2.0/Monei/apis/__init__.py`

 * *Files identical despite different names*

### Comparing `Monei-1.1.3/Monei/configuration.py` & `Monei-1.2.0/Monei/configuration.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     MONEI API v1
 
-    <p>The MONEI API is organized around <a href=\"https://en.wikipedia.org/wiki/Representational_State_Transfer\">REST</a>. Our API has predictable resource-oriented URLs, accepts JSON-encoded request bodies, returns JSON-encoded responses, and uses standard HTTP response codes, authentication, and verbs.</p> <h4 id=\"base-url\">Base URL:</h4> <p><a href=\"https://api.monei.com/v1\">https://api.monei.com/v1</a></p> <h4 id=\"client-libraries\">Client libraries:</h4> <ul> <li><a href=\"https://github.com/MONEI/monei-php-sdk\">PHP SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-python-sdk\">Python SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-node-sdk\">Node.js SDK</a></li> <li><a href=\"https://postman.monei.com/\">Postman Collection</a></li> </ul> <h4 id=\"important\">Important:</h4> <p><strong>If you are not using our official SDKs, you need to provide a valid <code>User-Agent</code> header in each request, otherwise your requests will be rejected.</strong></p>   # noqa: E501
+    <p>The MONEI API is organized around <a href=\"https://en.wikipedia.org/wiki/Representational_State_Transfer\">REST</a>. Our API has predictable resource-oriented URLs, accepts JSON-encoded request bodies, returns JSON-encoded responses, and uses standard HTTP response codes, authentication, and verbs.</p> <h4 id=\"base-url\">Base URL:</h4> <p><a href=\"https://api.monei.com/v1\">https://api.monei.com/v1</a></p> <h4 id=\"client-libraries\">Client libraries:</h4> <ul> <li><a href=\"https://github.com/MONEI/monei-php-sdk\">PHP SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-python-sdk\">Python SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-node-sdk\">Node.js SDK</a></li> <li><a href=\"https://postman.monei.com/\">Postman</a></li> </ul> <h4 id=\"important\">Important:</h4> <p><strong>If you are not using our official SDKs, you need to provide a valid <code>User-Agent</code> header in each request, otherwise your requests will be rejected.</strong></p>   # noqa: E501
 
-    The version of the OpenAPI document: 1.3.3
+    The version of the OpenAPI document: 1.4.0
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import copy
@@ -354,16 +354,16 @@
         """Gets the essential information for debugging.
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
-               "Version of the API: 1.3.3\n"\
-               "SDK Package Version: 1.1.3".\
+               "Version of the API: 1.4.0\n"\
+               "SDK Package Version: 1.2.0".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
         """
```

### Comparing `Monei-1.1.3/Monei/exceptions.py` & `Monei-1.2.0/Monei/exceptions.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     MONEI API v1
 
-    <p>The MONEI API is organized around <a href=\"https://en.wikipedia.org/wiki/Representational_State_Transfer\">REST</a>. Our API has predictable resource-oriented URLs, accepts JSON-encoded request bodies, returns JSON-encoded responses, and uses standard HTTP response codes, authentication, and verbs.</p> <h4 id=\"base-url\">Base URL:</h4> <p><a href=\"https://api.monei.com/v1\">https://api.monei.com/v1</a></p> <h4 id=\"client-libraries\">Client libraries:</h4> <ul> <li><a href=\"https://github.com/MONEI/monei-php-sdk\">PHP SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-python-sdk\">Python SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-node-sdk\">Node.js SDK</a></li> <li><a href=\"https://postman.monei.com/\">Postman Collection</a></li> </ul> <h4 id=\"important\">Important:</h4> <p><strong>If you are not using our official SDKs, you need to provide a valid <code>User-Agent</code> header in each request, otherwise your requests will be rejected.</strong></p>   # noqa: E501
+    <p>The MONEI API is organized around <a href=\"https://en.wikipedia.org/wiki/Representational_State_Transfer\">REST</a>. Our API has predictable resource-oriented URLs, accepts JSON-encoded request bodies, returns JSON-encoded responses, and uses standard HTTP response codes, authentication, and verbs.</p> <h4 id=\"base-url\">Base URL:</h4> <p><a href=\"https://api.monei.com/v1\">https://api.monei.com/v1</a></p> <h4 id=\"client-libraries\">Client libraries:</h4> <ul> <li><a href=\"https://github.com/MONEI/monei-php-sdk\">PHP SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-python-sdk\">Python SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-node-sdk\">Node.js SDK</a></li> <li><a href=\"https://postman.monei.com/\">Postman</a></li> </ul> <h4 id=\"important\">Important:</h4> <p><strong>If you are not using our official SDKs, you need to provide a valid <code>User-Agent</code> header in each request, otherwise your requests will be rejected.</strong></p>   # noqa: E501
 
-    The version of the OpenAPI document: 1.3.3
+    The version of the OpenAPI document: 1.4.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import six
```

### Comparing `Monei-1.1.3/Monei/model/activate_subscription_request.py` & `Monei-1.2.0/Monei/model/activate_subscription_request.py`

 * *Files identical despite different names*

### Comparing `Monei-1.1.3/Monei/model/address.py` & `Monei-1.2.0/Monei/model/address.py`

 * *Files identical despite different names*

### Comparing `Monei-1.1.3/Monei/model/cancel_payment_request.py` & `Monei-1.2.0/Monei/model/cancel_payment_request.py`

 * *Files identical despite different names*

### Comparing `Monei-1.1.3/Monei/model/cancel_subscription_request.py` & `Monei-1.2.0/Monei/model/cancel_subscription_request.py`

 * *Files identical despite different names*

### Comparing `Monei-1.1.3/Monei/model/capture_payment_request.py` & `Monei-1.2.0/Monei/model/capture_payment_request.py`

 * *Files identical despite different names*

### Comparing `Monei-1.1.3/Monei/model/card.py` & `Monei-1.2.0/Monei/model/card.py`

 * *Files identical despite different names*

### Comparing `Monei-1.1.3/Monei/model/confirm_payment_request.py` & `Monei-1.2.0/Monei/model/confirm_payment_request.py`

 * *Files identical despite different names*

### Comparing `Monei-1.1.3/Monei/model/confirm_payment_request_payment_method.py` & `Monei-1.2.0/Monei/model/confirm_payment_request_payment_method.py`

 * *Files identical despite different names*

### Comparing `Monei-1.1.3/Monei/model/confirm_payment_request_payment_method_card.py` & `Monei-1.2.0/Monei/model/confirm_payment_request_payment_method_card.py`

 * *Files identical despite different names*

### Comparing `Monei-1.1.3/Monei/model/create_payment_request.py` & `Monei-1.2.0/Monei/model/create_payment_request.py`

 * *Files identical despite different names*

### Comparing `Monei-1.1.3/Monei/model/create_subscription_request.py` & `Monei-1.2.0/Monei/model/create_subscription_request.py`

 * *Files identical despite different names*

### Comparing `Monei-1.1.3/Monei/model/domain_register200_response.py` & `Monei-1.2.0/Monei/model/domain_register200_response.py`

 * *Files identical despite different names*

### Comparing `Monei-1.1.3/Monei/model/error.py` & `Monei-1.2.0/Monei/model/error.py`

 * *Files identical despite different names*

### Comparing `Monei-1.1.3/Monei/model/pause_subscription_request.py` & `Monei-1.2.0/Monei/model/pause_subscription_request.py`

 * *Files identical despite different names*

### Comparing `Monei-1.1.3/Monei/model/payment.py` & `Monei-1.2.0/Monei/model/payment.py`

 * *Files identical despite different names*

### Comparing `Monei-1.1.3/Monei/model/payment_billing_details.py` & `Monei-1.2.0/Monei/model/payment_billing_details.py`

 * *Files identical despite different names*

### Comparing `Monei-1.1.3/Monei/model/payment_cancellation_reason.py` & `Monei-1.2.0/Monei/model/payment_cancellation_reason.py`

 * *Files identical despite different names*

### Comparing `Monei-1.1.3/Monei/model/payment_customer.py` & `Monei-1.2.0/Monei/model/payment_customer.py`

 * *Files identical despite different names*

### Comparing `Monei-1.1.3/Monei/model/payment_last_refund_reason.py` & `Monei-1.2.0/Monei/model/payment_last_refund_reason.py`

 * *Files identical despite different names*

### Comparing `Monei-1.1.3/Monei/model/payment_message_channel.py` & `Monei-1.2.0/Monei/model/payment_message_channel.py`

 * *Files identical despite different names*

### Comparing `Monei-1.1.3/Monei/model/payment_message_language.py` & `Monei-1.2.0/Monei/model/payment_message_language.py`

 * *Files identical despite different names*

### Comparing `Monei-1.1.3/Monei/model/payment_next_action.py` & `Monei-1.2.0/Monei/model/payment_next_action.py`

 * *Files identical despite different names*

### Comparing `Monei-1.1.3/Monei/model/payment_payment_method.py` & `Monei-1.2.0/Monei/model/payment_payment_method.py`

 * *Files identical despite different names*

### Comparing `Monei-1.1.3/Monei/model/payment_payment_method_bizum.py` & `Monei-1.2.0/Monei/model/payment_payment_method_bizum.py`

 * *Files identical despite different names*

### Comparing `Monei-1.1.3/Monei/model/payment_payment_method_card.py` & `Monei-1.2.0/Monei/model/payment_payment_method_card.py`

 * *Files identical despite different names*

### Comparing `Monei-1.1.3/Monei/model/payment_payment_method_cofidis.py` & `Monei-1.2.0/Monei/model/payment_payment_method_cofidis.py`

 * *Files identical despite different names*

### Comparing `Monei-1.1.3/Monei/model/payment_payment_method_input.py` & `Monei-1.2.0/Monei/model/payment_payment_method_input.py`

 * *Files identical despite different names*

### Comparing `Monei-1.1.3/Monei/model/payment_payment_method_paypal.py` & `Monei-1.2.0/Monei/model/payment_payment_method_paypal.py`

 * *Files identical despite different names*

### Comparing `Monei-1.1.3/Monei/model/payment_payment_methods.py` & `Monei-1.2.0/Monei/model/payment_payment_methods.py`

 * *Files identical despite different names*

### Comparing `Monei-1.1.3/Monei/model/payment_refund_reason.py` & `Monei-1.2.0/Monei/model/payment_refund_reason.py`

 * *Files identical despite different names*

### Comparing `Monei-1.1.3/Monei/model/payment_sequence.py` & `Monei-1.2.0/Monei/model/payment_sequence.py`

 * *Files identical despite different names*

### Comparing `Monei-1.1.3/Monei/model/payment_sequence_recurring.py` & `Monei-1.2.0/Monei/model/payment_sequence_recurring.py`

 * *Files identical despite different names*

### Comparing `Monei-1.1.3/Monei/model/payment_session_details.py` & `Monei-1.2.0/Monei/model/payment_session_details.py`

 * *Files identical despite different names*

### Comparing `Monei-1.1.3/Monei/model/payment_shipping_details.py` & `Monei-1.2.0/Monei/model/payment_shipping_details.py`

 * *Files identical despite different names*

### Comparing `Monei-1.1.3/Monei/model/payment_shop.py` & `Monei-1.2.0/Monei/model/payment_shop.py`

 * *Files identical despite different names*

### Comparing `Monei-1.1.3/Monei/model/payment_status.py` & `Monei-1.2.0/Monei/model/payment_status.py`

 * *Files identical despite different names*

### Comparing `Monei-1.1.3/Monei/model/payment_trace_details.py` & `Monei-1.2.0/Monei/model/payment_trace_details.py`

 * *Files identical despite different names*

### Comparing `Monei-1.1.3/Monei/model/payment_transaction_type.py` & `Monei-1.2.0/Monei/model/payment_transaction_type.py`

 * *Files identical despite different names*

### Comparing `Monei-1.1.3/Monei/model/recurring_payment_request.py` & `Monei-1.2.0/Monei/model/recurring_payment_request.py`

 * *Files identical despite different names*

### Comparing `Monei-1.1.3/Monei/model/refund_payment_request.py` & `Monei-1.2.0/Monei/model/refund_payment_request.py`

 * *Files identical despite different names*

### Comparing `Monei-1.1.3/Monei/model/register_domain_request.py` & `Monei-1.2.0/Monei/model/register_domain_request.py`

 * *Files identical despite different names*

### Comparing `Monei-1.1.3/Monei/model/send_payment_link_request.py` & `Monei-1.2.0/Monei/model/send_payment_link_request.py`

 * *Files identical despite different names*

### Comparing `Monei-1.1.3/Monei/model/send_payment_receipt_request.py` & `Monei-1.2.0/Monei/model/send_payment_receipt_request.py`

 * *Files identical despite different names*

### Comparing `Monei-1.1.3/Monei/model/subscription.py` & `Monei-1.2.0/Monei/model/subscription.py`

 * *Files identical despite different names*

### Comparing `Monei-1.1.3/Monei/model/subscription_interval.py` & `Monei-1.2.0/Monei/model/subscription_interval.py`

 * *Files identical despite different names*

### Comparing `Monei-1.1.3/Monei/model/subscription_last_payment.py` & `Monei-1.2.0/Monei/model/subscription_last_payment.py`

 * *Files identical despite different names*

### Comparing `Monei-1.1.3/Monei/model/subscription_payment_method.py` & `Monei-1.2.0/Monei/model/subscription_payment_method.py`

 * *Files identical despite different names*

### Comparing `Monei-1.1.3/Monei/model/subscription_payment_method_card.py` & `Monei-1.2.0/Monei/model/subscription_payment_method_card.py`

 * *Files identical despite different names*

### Comparing `Monei-1.1.3/Monei/model/subscription_status.py` & `Monei-1.2.0/Monei/model/subscription_status.py`

 * *Files identical despite different names*

### Comparing `Monei-1.1.3/Monei/model/update_subscription_request.py` & `Monei-1.2.0/Monei/model/update_subscription_request.py`

 * *Files identical despite different names*

### Comparing `Monei-1.1.3/Monei/model_utils.py` & `Monei-1.2.0/Monei/model_utils.py`

 * *Files identical despite different names*

### Comparing `Monei-1.1.3/Monei/models/__init__.py` & `Monei-1.2.0/Monei/models/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # coding: utf-8
 
 # flake8: noqa
 """
     MONEI API v1
 
-    <p>The MONEI API is organized around <a href=\"https://en.wikipedia.org/wiki/Representational_State_Transfer\">REST</a>. Our API has predictable resource-oriented URLs, accepts JSON-encoded request bodies, returns JSON-encoded responses, and uses standard HTTP response codes, authentication, and verbs.</p> <h4 id=\"base-url\">Base URL:</h4> <p><a href=\"https://api.monei.com/v1\">https://api.monei.com/v1</a></p> <h4 id=\"client-libraries\">Client libraries:</h4> <ul> <li><a href=\"https://github.com/MONEI/monei-php-sdk\">PHP SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-python-sdk\">Python SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-node-sdk\">Node.js SDK</a></li> <li><a href=\"https://postman.monei.com/\">Postman Collection</a></li> </ul> <h4 id=\"important\">Important:</h4> <p><strong>If you are not using our official SDKs, you need to provide a valid <code>User-Agent</code> header in each request, otherwise your requests will be rejected.</strong></p>   # noqa: E501
+    <p>The MONEI API is organized around <a href=\"https://en.wikipedia.org/wiki/Representational_State_Transfer\">REST</a>. Our API has predictable resource-oriented URLs, accepts JSON-encoded request bodies, returns JSON-encoded responses, and uses standard HTTP response codes, authentication, and verbs.</p> <h4 id=\"base-url\">Base URL:</h4> <p><a href=\"https://api.monei.com/v1\">https://api.monei.com/v1</a></p> <h4 id=\"client-libraries\">Client libraries:</h4> <ul> <li><a href=\"https://github.com/MONEI/monei-php-sdk\">PHP SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-python-sdk\">Python SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-node-sdk\">Node.js SDK</a></li> <li><a href=\"https://postman.monei.com/\">Postman</a></li> </ul> <h4 id=\"important\">Important:</h4> <p><strong>If you are not using our official SDKs, you need to provide a valid <code>User-Agent</code> header in each request, otherwise your requests will be rejected.</strong></p>   # noqa: E501
 
-    The version of the OpenAPI document: 1.3.3
+    The version of the OpenAPI document: 1.4.0
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 # import models into model package
@@ -53,14 +53,15 @@
 from Monei.models.payment_trace_details import PaymentTraceDetails
 from Monei.models.payment_transaction_type import PaymentTransactionType
 from Monei.models.recurring_payment_request import RecurringPaymentRequest
 from Monei.models.refund_payment_request import RefundPaymentRequest
 from Monei.models.register_domain_request import RegisterDomainRequest
 from Monei.models.send_payment_link_request import SendPaymentLinkRequest
 from Monei.models.send_payment_receipt_request import SendPaymentReceiptRequest
+from Monei.models.send_payment_request import SendPaymentRequest
 from Monei.models.subscription import Subscription
 from Monei.models.subscription_interval import SubscriptionInterval
 from Monei.models.subscription_last_payment import SubscriptionLastPayment
 from Monei.models.subscription_payment_method import SubscriptionPaymentMethod
 from Monei.models.subscription_payment_method_card import SubscriptionPaymentMethodCard
 from Monei.models.subscription_status import SubscriptionStatus
 from Monei.models.update_subscription_request import UpdateSubscriptionRequest
```

#### html2text {}

```diff
@@ -4,19 +4,19 @@
 responses, and uses standard HTTP response codes, authentication, and verbs.
 *** Base URL: ***
 https://api.monei.com/v1
 *** Client libraries: ***
     * PHP_SDK
     * Python_SDK
     * Node.js_SDK
-    * Postman_Collection
+    * Postman
 *** Important: ***
 If you are not using our official SDKs, you need to provide a valid User-Agent
 header in each request, otherwise your requests will be rejected.
-# noqa: E501 The version of the OpenAPI document: 1.3.3 Generated by: https://
+# noqa: E501 The version of the OpenAPI document: 1.4.0 Generated by: https://
 openapi-generator.tech """ from __future__ import absolute_import # import
 models into model package from Monei.models.activate_subscription_request
 import ActivateSubscriptionRequest from Monei.models.address import Address
 from Monei.models.cancel_payment_request import CancelPaymentRequest from
 Monei.models.cancel_subscription_request import CancelSubscriptionRequest from
 Monei.models.capture_payment_request import CapturePaymentRequest from
 Monei.models.confirm_payment_request import ConfirmPaymentRequest from
@@ -54,15 +54,16 @@
 import PaymentStatus from Monei.models.payment_trace_details import
 PaymentTraceDetails from Monei.models.payment_transaction_type import
 PaymentTransactionType from Monei.models.recurring_payment_request import
 RecurringPaymentRequest from Monei.models.refund_payment_request import
 RefundPaymentRequest from Monei.models.register_domain_request import
 RegisterDomainRequest from Monei.models.send_payment_link_request import
 SendPaymentLinkRequest from Monei.models.send_payment_receipt_request import
-SendPaymentReceiptRequest from Monei.models.subscription import Subscription
-from Monei.models.subscription_interval import SubscriptionInterval from
+SendPaymentReceiptRequest from Monei.models.send_payment_request import
+SendPaymentRequest from Monei.models.subscription import Subscription from
+Monei.models.subscription_interval import SubscriptionInterval from
 Monei.models.subscription_last_payment import SubscriptionLastPayment from
 Monei.models.subscription_payment_method import SubscriptionPaymentMethod from
 Monei.models.subscription_payment_method_card import
 SubscriptionPaymentMethodCard from Monei.models.subscription_status import
 SubscriptionStatus from Monei.models.update_subscription_request import
 UpdateSubscriptionRequest
```

### Comparing `Monei-1.1.3/Monei/models/activate_subscription_request.py` & `Monei-1.2.0/Monei/models/activate_subscription_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     MONEI API v1
 
-    <p>The MONEI API is organized around <a href=\"https://en.wikipedia.org/wiki/Representational_State_Transfer\">REST</a>. Our API has predictable resource-oriented URLs, accepts JSON-encoded request bodies, returns JSON-encoded responses, and uses standard HTTP response codes, authentication, and verbs.</p> <h4 id=\"base-url\">Base URL:</h4> <p><a href=\"https://api.monei.com/v1\">https://api.monei.com/v1</a></p> <h4 id=\"client-libraries\">Client libraries:</h4> <ul> <li><a href=\"https://github.com/MONEI/monei-php-sdk\">PHP SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-python-sdk\">Python SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-node-sdk\">Node.js SDK</a></li> <li><a href=\"https://postman.monei.com/\">Postman Collection</a></li> </ul> <h4 id=\"important\">Important:</h4> <p><strong>If you are not using our official SDKs, you need to provide a valid <code>User-Agent</code> header in each request, otherwise your requests will be rejected.</strong></p>   # noqa: E501
+    <p>The MONEI API is organized around <a href=\"https://en.wikipedia.org/wiki/Representational_State_Transfer\">REST</a>. Our API has predictable resource-oriented URLs, accepts JSON-encoded request bodies, returns JSON-encoded responses, and uses standard HTTP response codes, authentication, and verbs.</p> <h4 id=\"base-url\">Base URL:</h4> <p><a href=\"https://api.monei.com/v1\">https://api.monei.com/v1</a></p> <h4 id=\"client-libraries\">Client libraries:</h4> <ul> <li><a href=\"https://github.com/MONEI/monei-php-sdk\">PHP SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-python-sdk\">Python SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-node-sdk\">Node.js SDK</a></li> <li><a href=\"https://postman.monei.com/\">Postman</a></li> </ul> <h4 id=\"important\">Important:</h4> <p><strong>If you are not using our official SDKs, you need to provide a valid <code>User-Agent</code> header in each request, otherwise your requests will be rejected.</strong></p>   # noqa: E501
 
-    The version of the OpenAPI document: 1.3.3
+    The version of the OpenAPI document: 1.4.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `Monei-1.1.3/Monei/models/address.py` & `Monei-1.2.0/Monei/models/address.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     MONEI API v1
 
-    <p>The MONEI API is organized around <a href=\"https://en.wikipedia.org/wiki/Representational_State_Transfer\">REST</a>. Our API has predictable resource-oriented URLs, accepts JSON-encoded request bodies, returns JSON-encoded responses, and uses standard HTTP response codes, authentication, and verbs.</p> <h4 id=\"base-url\">Base URL:</h4> <p><a href=\"https://api.monei.com/v1\">https://api.monei.com/v1</a></p> <h4 id=\"client-libraries\">Client libraries:</h4> <ul> <li><a href=\"https://github.com/MONEI/monei-php-sdk\">PHP SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-python-sdk\">Python SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-node-sdk\">Node.js SDK</a></li> <li><a href=\"https://postman.monei.com/\">Postman Collection</a></li> </ul> <h4 id=\"important\">Important:</h4> <p><strong>If you are not using our official SDKs, you need to provide a valid <code>User-Agent</code> header in each request, otherwise your requests will be rejected.</strong></p>   # noqa: E501
+    <p>The MONEI API is organized around <a href=\"https://en.wikipedia.org/wiki/Representational_State_Transfer\">REST</a>. Our API has predictable resource-oriented URLs, accepts JSON-encoded request bodies, returns JSON-encoded responses, and uses standard HTTP response codes, authentication, and verbs.</p> <h4 id=\"base-url\">Base URL:</h4> <p><a href=\"https://api.monei.com/v1\">https://api.monei.com/v1</a></p> <h4 id=\"client-libraries\">Client libraries:</h4> <ul> <li><a href=\"https://github.com/MONEI/monei-php-sdk\">PHP SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-python-sdk\">Python SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-node-sdk\">Node.js SDK</a></li> <li><a href=\"https://postman.monei.com/\">Postman</a></li> </ul> <h4 id=\"important\">Important:</h4> <p><strong>If you are not using our official SDKs, you need to provide a valid <code>User-Agent</code> header in each request, otherwise your requests will be rejected.</strong></p>   # noqa: E501
 
-    The version of the OpenAPI document: 1.3.3
+    The version of the OpenAPI document: 1.4.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `Monei-1.1.3/Monei/models/cancel_payment_request.py` & `Monei-1.2.0/Monei/models/cancel_payment_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     MONEI API v1
 
-    <p>The MONEI API is organized around <a href=\"https://en.wikipedia.org/wiki/Representational_State_Transfer\">REST</a>. Our API has predictable resource-oriented URLs, accepts JSON-encoded request bodies, returns JSON-encoded responses, and uses standard HTTP response codes, authentication, and verbs.</p> <h4 id=\"base-url\">Base URL:</h4> <p><a href=\"https://api.monei.com/v1\">https://api.monei.com/v1</a></p> <h4 id=\"client-libraries\">Client libraries:</h4> <ul> <li><a href=\"https://github.com/MONEI/monei-php-sdk\">PHP SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-python-sdk\">Python SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-node-sdk\">Node.js SDK</a></li> <li><a href=\"https://postman.monei.com/\">Postman Collection</a></li> </ul> <h4 id=\"important\">Important:</h4> <p><strong>If you are not using our official SDKs, you need to provide a valid <code>User-Agent</code> header in each request, otherwise your requests will be rejected.</strong></p>   # noqa: E501
+    <p>The MONEI API is organized around <a href=\"https://en.wikipedia.org/wiki/Representational_State_Transfer\">REST</a>. Our API has predictable resource-oriented URLs, accepts JSON-encoded request bodies, returns JSON-encoded responses, and uses standard HTTP response codes, authentication, and verbs.</p> <h4 id=\"base-url\">Base URL:</h4> <p><a href=\"https://api.monei.com/v1\">https://api.monei.com/v1</a></p> <h4 id=\"client-libraries\">Client libraries:</h4> <ul> <li><a href=\"https://github.com/MONEI/monei-php-sdk\">PHP SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-python-sdk\">Python SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-node-sdk\">Node.js SDK</a></li> <li><a href=\"https://postman.monei.com/\">Postman</a></li> </ul> <h4 id=\"important\">Important:</h4> <p><strong>If you are not using our official SDKs, you need to provide a valid <code>User-Agent</code> header in each request, otherwise your requests will be rejected.</strong></p>   # noqa: E501
 
-    The version of the OpenAPI document: 1.3.3
+    The version of the OpenAPI document: 1.4.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `Monei-1.1.3/Monei/models/cancel_subscription_request.py` & `Monei-1.2.0/Monei/models/cancel_subscription_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     MONEI API v1
 
-    <p>The MONEI API is organized around <a href=\"https://en.wikipedia.org/wiki/Representational_State_Transfer\">REST</a>. Our API has predictable resource-oriented URLs, accepts JSON-encoded request bodies, returns JSON-encoded responses, and uses standard HTTP response codes, authentication, and verbs.</p> <h4 id=\"base-url\">Base URL:</h4> <p><a href=\"https://api.monei.com/v1\">https://api.monei.com/v1</a></p> <h4 id=\"client-libraries\">Client libraries:</h4> <ul> <li><a href=\"https://github.com/MONEI/monei-php-sdk\">PHP SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-python-sdk\">Python SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-node-sdk\">Node.js SDK</a></li> <li><a href=\"https://postman.monei.com/\">Postman Collection</a></li> </ul> <h4 id=\"important\">Important:</h4> <p><strong>If you are not using our official SDKs, you need to provide a valid <code>User-Agent</code> header in each request, otherwise your requests will be rejected.</strong></p>   # noqa: E501
+    <p>The MONEI API is organized around <a href=\"https://en.wikipedia.org/wiki/Representational_State_Transfer\">REST</a>. Our API has predictable resource-oriented URLs, accepts JSON-encoded request bodies, returns JSON-encoded responses, and uses standard HTTP response codes, authentication, and verbs.</p> <h4 id=\"base-url\">Base URL:</h4> <p><a href=\"https://api.monei.com/v1\">https://api.monei.com/v1</a></p> <h4 id=\"client-libraries\">Client libraries:</h4> <ul> <li><a href=\"https://github.com/MONEI/monei-php-sdk\">PHP SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-python-sdk\">Python SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-node-sdk\">Node.js SDK</a></li> <li><a href=\"https://postman.monei.com/\">Postman</a></li> </ul> <h4 id=\"important\">Important:</h4> <p><strong>If you are not using our official SDKs, you need to provide a valid <code>User-Agent</code> header in each request, otherwise your requests will be rejected.</strong></p>   # noqa: E501
 
-    The version of the OpenAPI document: 1.3.3
+    The version of the OpenAPI document: 1.4.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `Monei-1.1.3/Monei/models/capture_payment_request.py` & `Monei-1.2.0/Monei/models/capture_payment_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     MONEI API v1
 
-    <p>The MONEI API is organized around <a href=\"https://en.wikipedia.org/wiki/Representational_State_Transfer\">REST</a>. Our API has predictable resource-oriented URLs, accepts JSON-encoded request bodies, returns JSON-encoded responses, and uses standard HTTP response codes, authentication, and verbs.</p> <h4 id=\"base-url\">Base URL:</h4> <p><a href=\"https://api.monei.com/v1\">https://api.monei.com/v1</a></p> <h4 id=\"client-libraries\">Client libraries:</h4> <ul> <li><a href=\"https://github.com/MONEI/monei-php-sdk\">PHP SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-python-sdk\">Python SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-node-sdk\">Node.js SDK</a></li> <li><a href=\"https://postman.monei.com/\">Postman Collection</a></li> </ul> <h4 id=\"important\">Important:</h4> <p><strong>If you are not using our official SDKs, you need to provide a valid <code>User-Agent</code> header in each request, otherwise your requests will be rejected.</strong></p>   # noqa: E501
+    <p>The MONEI API is organized around <a href=\"https://en.wikipedia.org/wiki/Representational_State_Transfer\">REST</a>. Our API has predictable resource-oriented URLs, accepts JSON-encoded request bodies, returns JSON-encoded responses, and uses standard HTTP response codes, authentication, and verbs.</p> <h4 id=\"base-url\">Base URL:</h4> <p><a href=\"https://api.monei.com/v1\">https://api.monei.com/v1</a></p> <h4 id=\"client-libraries\">Client libraries:</h4> <ul> <li><a href=\"https://github.com/MONEI/monei-php-sdk\">PHP SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-python-sdk\">Python SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-node-sdk\">Node.js SDK</a></li> <li><a href=\"https://postman.monei.com/\">Postman</a></li> </ul> <h4 id=\"important\">Important:</h4> <p><strong>If you are not using our official SDKs, you need to provide a valid <code>User-Agent</code> header in each request, otherwise your requests will be rejected.</strong></p>   # noqa: E501
 
-    The version of the OpenAPI document: 1.3.3
+    The version of the OpenAPI document: 1.4.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `Monei-1.1.3/Monei/models/card.py` & `Monei-1.2.0/Monei/models/card.py`

 * *Files identical despite different names*

### Comparing `Monei-1.1.3/Monei/models/confirm_payment_request.py` & `Monei-1.2.0/Monei/models/confirm_payment_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     MONEI API v1
 
-    <p>The MONEI API is organized around <a href=\"https://en.wikipedia.org/wiki/Representational_State_Transfer\">REST</a>. Our API has predictable resource-oriented URLs, accepts JSON-encoded request bodies, returns JSON-encoded responses, and uses standard HTTP response codes, authentication, and verbs.</p> <h4 id=\"base-url\">Base URL:</h4> <p><a href=\"https://api.monei.com/v1\">https://api.monei.com/v1</a></p> <h4 id=\"client-libraries\">Client libraries:</h4> <ul> <li><a href=\"https://github.com/MONEI/monei-php-sdk\">PHP SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-python-sdk\">Python SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-node-sdk\">Node.js SDK</a></li> <li><a href=\"https://postman.monei.com/\">Postman Collection</a></li> </ul> <h4 id=\"important\">Important:</h4> <p><strong>If you are not using our official SDKs, you need to provide a valid <code>User-Agent</code> header in each request, otherwise your requests will be rejected.</strong></p>   # noqa: E501
+    <p>The MONEI API is organized around <a href=\"https://en.wikipedia.org/wiki/Representational_State_Transfer\">REST</a>. Our API has predictable resource-oriented URLs, accepts JSON-encoded request bodies, returns JSON-encoded responses, and uses standard HTTP response codes, authentication, and verbs.</p> <h4 id=\"base-url\">Base URL:</h4> <p><a href=\"https://api.monei.com/v1\">https://api.monei.com/v1</a></p> <h4 id=\"client-libraries\">Client libraries:</h4> <ul> <li><a href=\"https://github.com/MONEI/monei-php-sdk\">PHP SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-python-sdk\">Python SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-node-sdk\">Node.js SDK</a></li> <li><a href=\"https://postman.monei.com/\">Postman</a></li> </ul> <h4 id=\"important\">Important:</h4> <p><strong>If you are not using our official SDKs, you need to provide a valid <code>User-Agent</code> header in each request, otherwise your requests will be rejected.</strong></p>   # noqa: E501
 
-    The version of the OpenAPI document: 1.3.3
+    The version of the OpenAPI document: 1.4.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `Monei-1.1.3/Monei/models/confirm_payment_request_payment_method.py` & `Monei-1.2.0/Monei/models/confirm_payment_request_payment_method.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     MONEI API v1
 
-    <p>The MONEI API is organized around <a href=\"https://en.wikipedia.org/wiki/Representational_State_Transfer\">REST</a>. Our API has predictable resource-oriented URLs, accepts JSON-encoded request bodies, returns JSON-encoded responses, and uses standard HTTP response codes, authentication, and verbs.</p> <h4 id=\"base-url\">Base URL:</h4> <p><a href=\"https://api.monei.com/v1\">https://api.monei.com/v1</a></p> <h4 id=\"client-libraries\">Client libraries:</h4> <ul> <li><a href=\"https://github.com/MONEI/monei-php-sdk\">PHP SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-python-sdk\">Python SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-node-sdk\">Node.js SDK</a></li> <li><a href=\"https://postman.monei.com/\">Postman Collection</a></li> </ul> <h4 id=\"important\">Important:</h4> <p><strong>If you are not using our official SDKs, you need to provide a valid <code>User-Agent</code> header in each request, otherwise your requests will be rejected.</strong></p>   # noqa: E501
+    <p>The MONEI API is organized around <a href=\"https://en.wikipedia.org/wiki/Representational_State_Transfer\">REST</a>. Our API has predictable resource-oriented URLs, accepts JSON-encoded request bodies, returns JSON-encoded responses, and uses standard HTTP response codes, authentication, and verbs.</p> <h4 id=\"base-url\">Base URL:</h4> <p><a href=\"https://api.monei.com/v1\">https://api.monei.com/v1</a></p> <h4 id=\"client-libraries\">Client libraries:</h4> <ul> <li><a href=\"https://github.com/MONEI/monei-php-sdk\">PHP SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-python-sdk\">Python SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-node-sdk\">Node.js SDK</a></li> <li><a href=\"https://postman.monei.com/\">Postman</a></li> </ul> <h4 id=\"important\">Important:</h4> <p><strong>If you are not using our official SDKs, you need to provide a valid <code>User-Agent</code> header in each request, otherwise your requests will be rejected.</strong></p>   # noqa: E501
 
-    The version of the OpenAPI document: 1.3.3
+    The version of the OpenAPI document: 1.4.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `Monei-1.1.3/Monei/models/confirm_payment_request_payment_method_card.py` & `Monei-1.2.0/Monei/models/confirm_payment_request_payment_method_card.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     MONEI API v1
 
-    <p>The MONEI API is organized around <a href=\"https://en.wikipedia.org/wiki/Representational_State_Transfer\">REST</a>. Our API has predictable resource-oriented URLs, accepts JSON-encoded request bodies, returns JSON-encoded responses, and uses standard HTTP response codes, authentication, and verbs.</p> <h4 id=\"base-url\">Base URL:</h4> <p><a href=\"https://api.monei.com/v1\">https://api.monei.com/v1</a></p> <h4 id=\"client-libraries\">Client libraries:</h4> <ul> <li><a href=\"https://github.com/MONEI/monei-php-sdk\">PHP SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-python-sdk\">Python SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-node-sdk\">Node.js SDK</a></li> <li><a href=\"https://postman.monei.com/\">Postman Collection</a></li> </ul> <h4 id=\"important\">Important:</h4> <p><strong>If you are not using our official SDKs, you need to provide a valid <code>User-Agent</code> header in each request, otherwise your requests will be rejected.</strong></p>   # noqa: E501
+    <p>The MONEI API is organized around <a href=\"https://en.wikipedia.org/wiki/Representational_State_Transfer\">REST</a>. Our API has predictable resource-oriented URLs, accepts JSON-encoded request bodies, returns JSON-encoded responses, and uses standard HTTP response codes, authentication, and verbs.</p> <h4 id=\"base-url\">Base URL:</h4> <p><a href=\"https://api.monei.com/v1\">https://api.monei.com/v1</a></p> <h4 id=\"client-libraries\">Client libraries:</h4> <ul> <li><a href=\"https://github.com/MONEI/monei-php-sdk\">PHP SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-python-sdk\">Python SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-node-sdk\">Node.js SDK</a></li> <li><a href=\"https://postman.monei.com/\">Postman</a></li> </ul> <h4 id=\"important\">Important:</h4> <p><strong>If you are not using our official SDKs, you need to provide a valid <code>User-Agent</code> header in each request, otherwise your requests will be rejected.</strong></p>   # noqa: E501
 
-    The version of the OpenAPI document: 1.3.3
+    The version of the OpenAPI document: 1.4.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `Monei-1.1.3/Monei/models/create_payment_request.py` & `Monei-1.2.0/Monei/models/create_payment_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     MONEI API v1
 
-    <p>The MONEI API is organized around <a href=\"https://en.wikipedia.org/wiki/Representational_State_Transfer\">REST</a>. Our API has predictable resource-oriented URLs, accepts JSON-encoded request bodies, returns JSON-encoded responses, and uses standard HTTP response codes, authentication, and verbs.</p> <h4 id=\"base-url\">Base URL:</h4> <p><a href=\"https://api.monei.com/v1\">https://api.monei.com/v1</a></p> <h4 id=\"client-libraries\">Client libraries:</h4> <ul> <li><a href=\"https://github.com/MONEI/monei-php-sdk\">PHP SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-python-sdk\">Python SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-node-sdk\">Node.js SDK</a></li> <li><a href=\"https://postman.monei.com/\">Postman Collection</a></li> </ul> <h4 id=\"important\">Important:</h4> <p><strong>If you are not using our official SDKs, you need to provide a valid <code>User-Agent</code> header in each request, otherwise your requests will be rejected.</strong></p>   # noqa: E501
+    <p>The MONEI API is organized around <a href=\"https://en.wikipedia.org/wiki/Representational_State_Transfer\">REST</a>. Our API has predictable resource-oriented URLs, accepts JSON-encoded request bodies, returns JSON-encoded responses, and uses standard HTTP response codes, authentication, and verbs.</p> <h4 id=\"base-url\">Base URL:</h4> <p><a href=\"https://api.monei.com/v1\">https://api.monei.com/v1</a></p> <h4 id=\"client-libraries\">Client libraries:</h4> <ul> <li><a href=\"https://github.com/MONEI/monei-php-sdk\">PHP SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-python-sdk\">Python SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-node-sdk\">Node.js SDK</a></li> <li><a href=\"https://postman.monei.com/\">Postman</a></li> </ul> <h4 id=\"important\">Important:</h4> <p><strong>If you are not using our official SDKs, you need to provide a valid <code>User-Agent</code> header in each request, otherwise your requests will be rejected.</strong></p>   # noqa: E501
 
-    The version of the OpenAPI document: 1.3.3
+    The version of the OpenAPI document: 1.4.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `Monei-1.1.3/Monei/models/create_subscription_request.py` & `Monei-1.2.0/Monei/models/create_subscription_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     MONEI API v1
 
-    <p>The MONEI API is organized around <a href=\"https://en.wikipedia.org/wiki/Representational_State_Transfer\">REST</a>. Our API has predictable resource-oriented URLs, accepts JSON-encoded request bodies, returns JSON-encoded responses, and uses standard HTTP response codes, authentication, and verbs.</p> <h4 id=\"base-url\">Base URL:</h4> <p><a href=\"https://api.monei.com/v1\">https://api.monei.com/v1</a></p> <h4 id=\"client-libraries\">Client libraries:</h4> <ul> <li><a href=\"https://github.com/MONEI/monei-php-sdk\">PHP SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-python-sdk\">Python SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-node-sdk\">Node.js SDK</a></li> <li><a href=\"https://postman.monei.com/\">Postman Collection</a></li> </ul> <h4 id=\"important\">Important:</h4> <p><strong>If you are not using our official SDKs, you need to provide a valid <code>User-Agent</code> header in each request, otherwise your requests will be rejected.</strong></p>   # noqa: E501
+    <p>The MONEI API is organized around <a href=\"https://en.wikipedia.org/wiki/Representational_State_Transfer\">REST</a>. Our API has predictable resource-oriented URLs, accepts JSON-encoded request bodies, returns JSON-encoded responses, and uses standard HTTP response codes, authentication, and verbs.</p> <h4 id=\"base-url\">Base URL:</h4> <p><a href=\"https://api.monei.com/v1\">https://api.monei.com/v1</a></p> <h4 id=\"client-libraries\">Client libraries:</h4> <ul> <li><a href=\"https://github.com/MONEI/monei-php-sdk\">PHP SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-python-sdk\">Python SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-node-sdk\">Node.js SDK</a></li> <li><a href=\"https://postman.monei.com/\">Postman</a></li> </ul> <h4 id=\"important\">Important:</h4> <p><strong>If you are not using our official SDKs, you need to provide a valid <code>User-Agent</code> header in each request, otherwise your requests will be rejected.</strong></p>   # noqa: E501
 
-    The version of the OpenAPI document: 1.3.3
+    The version of the OpenAPI document: 1.4.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `Monei-1.1.3/Monei/models/error.py` & `Monei-1.2.0/Monei/models/error.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     MONEI API v1
 
-    <p>The MONEI API is organized around <a href=\"https://en.wikipedia.org/wiki/Representational_State_Transfer\">REST</a>. Our API has predictable resource-oriented URLs, accepts JSON-encoded request bodies, returns JSON-encoded responses, and uses standard HTTP response codes, authentication, and verbs.</p> <h4 id=\"base-url\">Base URL:</h4> <p><a href=\"https://api.monei.com/v1\">https://api.monei.com/v1</a></p> <h4 id=\"client-libraries\">Client libraries:</h4> <ul> <li><a href=\"https://github.com/MONEI/monei-php-sdk\">PHP SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-python-sdk\">Python SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-node-sdk\">Node.js SDK</a></li> <li><a href=\"https://postman.monei.com/\">Postman Collection</a></li> </ul> <h4 id=\"important\">Important:</h4> <p><strong>If you are not using our official SDKs, you need to provide a valid <code>User-Agent</code> header in each request, otherwise your requests will be rejected.</strong></p>   # noqa: E501
+    <p>The MONEI API is organized around <a href=\"https://en.wikipedia.org/wiki/Representational_State_Transfer\">REST</a>. Our API has predictable resource-oriented URLs, accepts JSON-encoded request bodies, returns JSON-encoded responses, and uses standard HTTP response codes, authentication, and verbs.</p> <h4 id=\"base-url\">Base URL:</h4> <p><a href=\"https://api.monei.com/v1\">https://api.monei.com/v1</a></p> <h4 id=\"client-libraries\">Client libraries:</h4> <ul> <li><a href=\"https://github.com/MONEI/monei-php-sdk\">PHP SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-python-sdk\">Python SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-node-sdk\">Node.js SDK</a></li> <li><a href=\"https://postman.monei.com/\">Postman</a></li> </ul> <h4 id=\"important\">Important:</h4> <p><strong>If you are not using our official SDKs, you need to provide a valid <code>User-Agent</code> header in each request, otherwise your requests will be rejected.</strong></p>   # noqa: E501
 
-    The version of the OpenAPI document: 1.3.3
+    The version of the OpenAPI document: 1.4.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `Monei-1.1.3/Monei/models/inline_object.py` & `Monei-1.2.0/Monei/models/inline_object.py`

 * *Files identical despite different names*

### Comparing `Monei-1.1.3/Monei/models/inline_response200.py` & `Monei-1.2.0/Monei/models/inline_response200.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     MONEI API v1
 
-    <p>The MONEI API is organized around <a href=\"https://en.wikipedia.org/wiki/Representational_State_Transfer\">REST</a>. Our API has predictable resource-oriented URLs, accepts JSON-encoded request bodies, returns JSON-encoded responses, and uses standard HTTP response codes, authentication, and verbs.</p> <h4 id=\"base-url\">Base URL:</h4> <p><a href=\"https://api.monei.com/v1\">https://api.monei.com/v1</a></p> <h4 id=\"client-libraries\">Client libraries:</h4> <ul> <li><a href=\"https://github.com/MONEI/monei-php-sdk\">PHP SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-python-sdk\">Python SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-node-sdk\">Node.js SDK</a></li> <li><a href=\"https://postman.monei.com/\">Postman Collection</a></li> </ul> <h4 id=\"important\">Important:</h4> <p><strong>If you are not using our official SDKs, you need to provide a valid <code>User-Agent</code> header in each request, otherwise your requests will be rejected.</strong></p>   # noqa: E501
+    <p>The MONEI API is organized around <a href=\"https://en.wikipedia.org/wiki/Representational_State_Transfer\">REST</a>. Our API has predictable resource-oriented URLs, accepts JSON-encoded request bodies, returns JSON-encoded responses, and uses standard HTTP response codes, authentication, and verbs.</p> <h4 id=\"base-url\">Base URL:</h4> <p><a href=\"https://api.monei.com/v1\">https://api.monei.com/v1</a></p> <h4 id=\"client-libraries\">Client libraries:</h4> <ul> <li><a href=\"https://github.com/MONEI/monei-php-sdk\">PHP SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-python-sdk\">Python SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-node-sdk\">Node.js SDK</a></li> <li><a href=\"https://postman.monei.com/\">Postman</a></li> </ul> <h4 id=\"important\">Important:</h4> <p><strong>If you are not using our official SDKs, you need to provide a valid <code>User-Agent</code> header in each request, otherwise your requests will be rejected.</strong></p>   # noqa: E501
 
-    The version of the OpenAPI document: 1.3.3
+    The version of the OpenAPI document: 1.4.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `Monei-1.1.3/Monei/models/pause_subscription_request.py` & `Monei-1.2.0/Monei/models/pause_subscription_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     MONEI API v1
 
-    <p>The MONEI API is organized around <a href=\"https://en.wikipedia.org/wiki/Representational_State_Transfer\">REST</a>. Our API has predictable resource-oriented URLs, accepts JSON-encoded request bodies, returns JSON-encoded responses, and uses standard HTTP response codes, authentication, and verbs.</p> <h4 id=\"base-url\">Base URL:</h4> <p><a href=\"https://api.monei.com/v1\">https://api.monei.com/v1</a></p> <h4 id=\"client-libraries\">Client libraries:</h4> <ul> <li><a href=\"https://github.com/MONEI/monei-php-sdk\">PHP SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-python-sdk\">Python SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-node-sdk\">Node.js SDK</a></li> <li><a href=\"https://postman.monei.com/\">Postman Collection</a></li> </ul> <h4 id=\"important\">Important:</h4> <p><strong>If you are not using our official SDKs, you need to provide a valid <code>User-Agent</code> header in each request, otherwise your requests will be rejected.</strong></p>   # noqa: E501
+    <p>The MONEI API is organized around <a href=\"https://en.wikipedia.org/wiki/Representational_State_Transfer\">REST</a>. Our API has predictable resource-oriented URLs, accepts JSON-encoded request bodies, returns JSON-encoded responses, and uses standard HTTP response codes, authentication, and verbs.</p> <h4 id=\"base-url\">Base URL:</h4> <p><a href=\"https://api.monei.com/v1\">https://api.monei.com/v1</a></p> <h4 id=\"client-libraries\">Client libraries:</h4> <ul> <li><a href=\"https://github.com/MONEI/monei-php-sdk\">PHP SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-python-sdk\">Python SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-node-sdk\">Node.js SDK</a></li> <li><a href=\"https://postman.monei.com/\">Postman</a></li> </ul> <h4 id=\"important\">Important:</h4> <p><strong>If you are not using our official SDKs, you need to provide a valid <code>User-Agent</code> header in each request, otherwise your requests will be rejected.</strong></p>   # noqa: E501
 
-    The version of the OpenAPI document: 1.3.3
+    The version of the OpenAPI document: 1.4.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `Monei-1.1.3/Monei/models/payment.py` & `Monei-1.2.0/Monei/models/payment.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     MONEI API v1
 
-    <p>The MONEI API is organized around <a href=\"https://en.wikipedia.org/wiki/Representational_State_Transfer\">REST</a>. Our API has predictable resource-oriented URLs, accepts JSON-encoded request bodies, returns JSON-encoded responses, and uses standard HTTP response codes, authentication, and verbs.</p> <h4 id=\"base-url\">Base URL:</h4> <p><a href=\"https://api.monei.com/v1\">https://api.monei.com/v1</a></p> <h4 id=\"client-libraries\">Client libraries:</h4> <ul> <li><a href=\"https://github.com/MONEI/monei-php-sdk\">PHP SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-python-sdk\">Python SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-node-sdk\">Node.js SDK</a></li> <li><a href=\"https://postman.monei.com/\">Postman Collection</a></li> </ul> <h4 id=\"important\">Important:</h4> <p><strong>If you are not using our official SDKs, you need to provide a valid <code>User-Agent</code> header in each request, otherwise your requests will be rejected.</strong></p>   # noqa: E501
+    <p>The MONEI API is organized around <a href=\"https://en.wikipedia.org/wiki/Representational_State_Transfer\">REST</a>. Our API has predictable resource-oriented URLs, accepts JSON-encoded request bodies, returns JSON-encoded responses, and uses standard HTTP response codes, authentication, and verbs.</p> <h4 id=\"base-url\">Base URL:</h4> <p><a href=\"https://api.monei.com/v1\">https://api.monei.com/v1</a></p> <h4 id=\"client-libraries\">Client libraries:</h4> <ul> <li><a href=\"https://github.com/MONEI/monei-php-sdk\">PHP SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-python-sdk\">Python SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-node-sdk\">Node.js SDK</a></li> <li><a href=\"https://postman.monei.com/\">Postman</a></li> </ul> <h4 id=\"important\">Important:</h4> <p><strong>If you are not using our official SDKs, you need to provide a valid <code>User-Agent</code> header in each request, otherwise your requests will be rejected.</strong></p>   # noqa: E501
 
-    The version of the OpenAPI document: 1.3.3
+    The version of the OpenAPI document: 1.4.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `Monei-1.1.3/Monei/models/payment_billing_details.py` & `Monei-1.2.0/Monei/models/payment_billing_details.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     MONEI API v1
 
-    <p>The MONEI API is organized around <a href=\"https://en.wikipedia.org/wiki/Representational_State_Transfer\">REST</a>. Our API has predictable resource-oriented URLs, accepts JSON-encoded request bodies, returns JSON-encoded responses, and uses standard HTTP response codes, authentication, and verbs.</p> <h4 id=\"base-url\">Base URL:</h4> <p><a href=\"https://api.monei.com/v1\">https://api.monei.com/v1</a></p> <h4 id=\"client-libraries\">Client libraries:</h4> <ul> <li><a href=\"https://github.com/MONEI/monei-php-sdk\">PHP SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-python-sdk\">Python SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-node-sdk\">Node.js SDK</a></li> <li><a href=\"https://postman.monei.com/\">Postman Collection</a></li> </ul> <h4 id=\"important\">Important:</h4> <p><strong>If you are not using our official SDKs, you need to provide a valid <code>User-Agent</code> header in each request, otherwise your requests will be rejected.</strong></p>   # noqa: E501
+    <p>The MONEI API is organized around <a href=\"https://en.wikipedia.org/wiki/Representational_State_Transfer\">REST</a>. Our API has predictable resource-oriented URLs, accepts JSON-encoded request bodies, returns JSON-encoded responses, and uses standard HTTP response codes, authentication, and verbs.</p> <h4 id=\"base-url\">Base URL:</h4> <p><a href=\"https://api.monei.com/v1\">https://api.monei.com/v1</a></p> <h4 id=\"client-libraries\">Client libraries:</h4> <ul> <li><a href=\"https://github.com/MONEI/monei-php-sdk\">PHP SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-python-sdk\">Python SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-node-sdk\">Node.js SDK</a></li> <li><a href=\"https://postman.monei.com/\">Postman</a></li> </ul> <h4 id=\"important\">Important:</h4> <p><strong>If you are not using our official SDKs, you need to provide a valid <code>User-Agent</code> header in each request, otherwise your requests will be rejected.</strong></p>   # noqa: E501
 
-    The version of the OpenAPI document: 1.3.3
+    The version of the OpenAPI document: 1.4.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `Monei-1.1.3/Monei/models/payment_cancellation_reason.py` & `Monei-1.2.0/Monei/models/payment_cancellation_reason.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     MONEI API v1
 
-    <p>The MONEI API is organized around <a href=\"https://en.wikipedia.org/wiki/Representational_State_Transfer\">REST</a>. Our API has predictable resource-oriented URLs, accepts JSON-encoded request bodies, returns JSON-encoded responses, and uses standard HTTP response codes, authentication, and verbs.</p> <h4 id=\"base-url\">Base URL:</h4> <p><a href=\"https://api.monei.com/v1\">https://api.monei.com/v1</a></p> <h4 id=\"client-libraries\">Client libraries:</h4> <ul> <li><a href=\"https://github.com/MONEI/monei-php-sdk\">PHP SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-python-sdk\">Python SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-node-sdk\">Node.js SDK</a></li> <li><a href=\"https://postman.monei.com/\">Postman Collection</a></li> </ul> <h4 id=\"important\">Important:</h4> <p><strong>If you are not using our official SDKs, you need to provide a valid <code>User-Agent</code> header in each request, otherwise your requests will be rejected.</strong></p>   # noqa: E501
+    <p>The MONEI API is organized around <a href=\"https://en.wikipedia.org/wiki/Representational_State_Transfer\">REST</a>. Our API has predictable resource-oriented URLs, accepts JSON-encoded request bodies, returns JSON-encoded responses, and uses standard HTTP response codes, authentication, and verbs.</p> <h4 id=\"base-url\">Base URL:</h4> <p><a href=\"https://api.monei.com/v1\">https://api.monei.com/v1</a></p> <h4 id=\"client-libraries\">Client libraries:</h4> <ul> <li><a href=\"https://github.com/MONEI/monei-php-sdk\">PHP SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-python-sdk\">Python SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-node-sdk\">Node.js SDK</a></li> <li><a href=\"https://postman.monei.com/\">Postman</a></li> </ul> <h4 id=\"important\">Important:</h4> <p><strong>If you are not using our official SDKs, you need to provide a valid <code>User-Agent</code> header in each request, otherwise your requests will be rejected.</strong></p>   # noqa: E501
 
-    The version of the OpenAPI document: 1.3.3
+    The version of the OpenAPI document: 1.4.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `Monei-1.1.3/Monei/models/payment_customer.py` & `Monei-1.2.0/Monei/models/payment_customer.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     MONEI API v1
 
-    <p>The MONEI API is organized around <a href=\"https://en.wikipedia.org/wiki/Representational_State_Transfer\">REST</a>. Our API has predictable resource-oriented URLs, accepts JSON-encoded request bodies, returns JSON-encoded responses, and uses standard HTTP response codes, authentication, and verbs.</p> <h4 id=\"base-url\">Base URL:</h4> <p><a href=\"https://api.monei.com/v1\">https://api.monei.com/v1</a></p> <h4 id=\"client-libraries\">Client libraries:</h4> <ul> <li><a href=\"https://github.com/MONEI/monei-php-sdk\">PHP SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-python-sdk\">Python SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-node-sdk\">Node.js SDK</a></li> <li><a href=\"https://postman.monei.com/\">Postman Collection</a></li> </ul> <h4 id=\"important\">Important:</h4> <p><strong>If you are not using our official SDKs, you need to provide a valid <code>User-Agent</code> header in each request, otherwise your requests will be rejected.</strong></p>   # noqa: E501
+    <p>The MONEI API is organized around <a href=\"https://en.wikipedia.org/wiki/Representational_State_Transfer\">REST</a>. Our API has predictable resource-oriented URLs, accepts JSON-encoded request bodies, returns JSON-encoded responses, and uses standard HTTP response codes, authentication, and verbs.</p> <h4 id=\"base-url\">Base URL:</h4> <p><a href=\"https://api.monei.com/v1\">https://api.monei.com/v1</a></p> <h4 id=\"client-libraries\">Client libraries:</h4> <ul> <li><a href=\"https://github.com/MONEI/monei-php-sdk\">PHP SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-python-sdk\">Python SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-node-sdk\">Node.js SDK</a></li> <li><a href=\"https://postman.monei.com/\">Postman</a></li> </ul> <h4 id=\"important\">Important:</h4> <p><strong>If you are not using our official SDKs, you need to provide a valid <code>User-Agent</code> header in each request, otherwise your requests will be rejected.</strong></p>   # noqa: E501
 
-    The version of the OpenAPI document: 1.3.3
+    The version of the OpenAPI document: 1.4.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `Monei-1.1.3/Monei/models/payment_last_refund_reason.py` & `Monei-1.2.0/Monei/models/payment_last_refund_reason.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     MONEI API v1
 
-    <p>The MONEI API is organized around <a href=\"https://en.wikipedia.org/wiki/Representational_State_Transfer\">REST</a>. Our API has predictable resource-oriented URLs, accepts JSON-encoded request bodies, returns JSON-encoded responses, and uses standard HTTP response codes, authentication, and verbs.</p> <h4 id=\"base-url\">Base URL:</h4> <p><a href=\"https://api.monei.com/v1\">https://api.monei.com/v1</a></p> <h4 id=\"client-libraries\">Client libraries:</h4> <ul> <li><a href=\"https://github.com/MONEI/monei-php-sdk\">PHP SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-python-sdk\">Python SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-node-sdk\">Node.js SDK</a></li> <li><a href=\"https://postman.monei.com/\">Postman Collection</a></li> </ul> <h4 id=\"important\">Important:</h4> <p><strong>If you are not using our official SDKs, you need to provide a valid <code>User-Agent</code> header in each request, otherwise your requests will be rejected.</strong></p>   # noqa: E501
+    <p>The MONEI API is organized around <a href=\"https://en.wikipedia.org/wiki/Representational_State_Transfer\">REST</a>. Our API has predictable resource-oriented URLs, accepts JSON-encoded request bodies, returns JSON-encoded responses, and uses standard HTTP response codes, authentication, and verbs.</p> <h4 id=\"base-url\">Base URL:</h4> <p><a href=\"https://api.monei.com/v1\">https://api.monei.com/v1</a></p> <h4 id=\"client-libraries\">Client libraries:</h4> <ul> <li><a href=\"https://github.com/MONEI/monei-php-sdk\">PHP SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-python-sdk\">Python SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-node-sdk\">Node.js SDK</a></li> <li><a href=\"https://postman.monei.com/\">Postman</a></li> </ul> <h4 id=\"important\">Important:</h4> <p><strong>If you are not using our official SDKs, you need to provide a valid <code>User-Agent</code> header in each request, otherwise your requests will be rejected.</strong></p>   # noqa: E501
 
-    The version of the OpenAPI document: 1.3.3
+    The version of the OpenAPI document: 1.4.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `Monei-1.1.3/Monei/models/payment_message_channel.py` & `Monei-1.2.0/Monei/models/payment_message_channel.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     MONEI API v1
 
-    <p>The MONEI API is organized around <a href=\"https://en.wikipedia.org/wiki/Representational_State_Transfer\">REST</a>. Our API has predictable resource-oriented URLs, accepts JSON-encoded request bodies, returns JSON-encoded responses, and uses standard HTTP response codes, authentication, and verbs.</p> <h4 id=\"base-url\">Base URL:</h4> <p><a href=\"https://api.monei.com/v1\">https://api.monei.com/v1</a></p> <h4 id=\"client-libraries\">Client libraries:</h4> <ul> <li><a href=\"https://github.com/MONEI/monei-php-sdk\">PHP SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-python-sdk\">Python SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-node-sdk\">Node.js SDK</a></li> <li><a href=\"https://postman.monei.com/\">Postman Collection</a></li> </ul> <h4 id=\"important\">Important:</h4> <p><strong>If you are not using our official SDKs, you need to provide a valid <code>User-Agent</code> header in each request, otherwise your requests will be rejected.</strong></p>   # noqa: E501
+    <p>The MONEI API is organized around <a href=\"https://en.wikipedia.org/wiki/Representational_State_Transfer\">REST</a>. Our API has predictable resource-oriented URLs, accepts JSON-encoded request bodies, returns JSON-encoded responses, and uses standard HTTP response codes, authentication, and verbs.</p> <h4 id=\"base-url\">Base URL:</h4> <p><a href=\"https://api.monei.com/v1\">https://api.monei.com/v1</a></p> <h4 id=\"client-libraries\">Client libraries:</h4> <ul> <li><a href=\"https://github.com/MONEI/monei-php-sdk\">PHP SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-python-sdk\">Python SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-node-sdk\">Node.js SDK</a></li> <li><a href=\"https://postman.monei.com/\">Postman</a></li> </ul> <h4 id=\"important\">Important:</h4> <p><strong>If you are not using our official SDKs, you need to provide a valid <code>User-Agent</code> header in each request, otherwise your requests will be rejected.</strong></p>   # noqa: E501
 
-    The version of the OpenAPI document: 1.3.3
+    The version of the OpenAPI document: 1.4.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `Monei-1.1.3/Monei/models/payment_message_language.py` & `Monei-1.2.0/Monei/models/payment_message_language.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     MONEI API v1
 
-    <p>The MONEI API is organized around <a href=\"https://en.wikipedia.org/wiki/Representational_State_Transfer\">REST</a>. Our API has predictable resource-oriented URLs, accepts JSON-encoded request bodies, returns JSON-encoded responses, and uses standard HTTP response codes, authentication, and verbs.</p> <h4 id=\"base-url\">Base URL:</h4> <p><a href=\"https://api.monei.com/v1\">https://api.monei.com/v1</a></p> <h4 id=\"client-libraries\">Client libraries:</h4> <ul> <li><a href=\"https://github.com/MONEI/monei-php-sdk\">PHP SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-python-sdk\">Python SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-node-sdk\">Node.js SDK</a></li> <li><a href=\"https://postman.monei.com/\">Postman Collection</a></li> </ul> <h4 id=\"important\">Important:</h4> <p><strong>If you are not using our official SDKs, you need to provide a valid <code>User-Agent</code> header in each request, otherwise your requests will be rejected.</strong></p>   # noqa: E501
+    <p>The MONEI API is organized around <a href=\"https://en.wikipedia.org/wiki/Representational_State_Transfer\">REST</a>. Our API has predictable resource-oriented URLs, accepts JSON-encoded request bodies, returns JSON-encoded responses, and uses standard HTTP response codes, authentication, and verbs.</p> <h4 id=\"base-url\">Base URL:</h4> <p><a href=\"https://api.monei.com/v1\">https://api.monei.com/v1</a></p> <h4 id=\"client-libraries\">Client libraries:</h4> <ul> <li><a href=\"https://github.com/MONEI/monei-php-sdk\">PHP SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-python-sdk\">Python SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-node-sdk\">Node.js SDK</a></li> <li><a href=\"https://postman.monei.com/\">Postman</a></li> </ul> <h4 id=\"important\">Important:</h4> <p><strong>If you are not using our official SDKs, you need to provide a valid <code>User-Agent</code> header in each request, otherwise your requests will be rejected.</strong></p>   # noqa: E501
 
-    The version of the OpenAPI document: 1.3.3
+    The version of the OpenAPI document: 1.4.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `Monei-1.1.3/Monei/models/payment_next_action.py` & `Monei-1.2.0/Monei/models/payment_next_action.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     MONEI API v1
 
-    <p>The MONEI API is organized around <a href=\"https://en.wikipedia.org/wiki/Representational_State_Transfer\">REST</a>. Our API has predictable resource-oriented URLs, accepts JSON-encoded request bodies, returns JSON-encoded responses, and uses standard HTTP response codes, authentication, and verbs.</p> <h4 id=\"base-url\">Base URL:</h4> <p><a href=\"https://api.monei.com/v1\">https://api.monei.com/v1</a></p> <h4 id=\"client-libraries\">Client libraries:</h4> <ul> <li><a href=\"https://github.com/MONEI/monei-php-sdk\">PHP SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-python-sdk\">Python SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-node-sdk\">Node.js SDK</a></li> <li><a href=\"https://postman.monei.com/\">Postman Collection</a></li> </ul> <h4 id=\"important\">Important:</h4> <p><strong>If you are not using our official SDKs, you need to provide a valid <code>User-Agent</code> header in each request, otherwise your requests will be rejected.</strong></p>   # noqa: E501
+    <p>The MONEI API is organized around <a href=\"https://en.wikipedia.org/wiki/Representational_State_Transfer\">REST</a>. Our API has predictable resource-oriented URLs, accepts JSON-encoded request bodies, returns JSON-encoded responses, and uses standard HTTP response codes, authentication, and verbs.</p> <h4 id=\"base-url\">Base URL:</h4> <p><a href=\"https://api.monei.com/v1\">https://api.monei.com/v1</a></p> <h4 id=\"client-libraries\">Client libraries:</h4> <ul> <li><a href=\"https://github.com/MONEI/monei-php-sdk\">PHP SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-python-sdk\">Python SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-node-sdk\">Node.js SDK</a></li> <li><a href=\"https://postman.monei.com/\">Postman</a></li> </ul> <h4 id=\"important\">Important:</h4> <p><strong>If you are not using our official SDKs, you need to provide a valid <code>User-Agent</code> header in each request, otherwise your requests will be rejected.</strong></p>   # noqa: E501
 
-    The version of the OpenAPI document: 1.3.3
+    The version of the OpenAPI document: 1.4.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `Monei-1.1.3/Monei/models/payment_payment_method.py` & `Monei-1.2.0/Monei/models/payment_payment_method.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     MONEI API v1
 
-    <p>The MONEI API is organized around <a href=\"https://en.wikipedia.org/wiki/Representational_State_Transfer\">REST</a>. Our API has predictable resource-oriented URLs, accepts JSON-encoded request bodies, returns JSON-encoded responses, and uses standard HTTP response codes, authentication, and verbs.</p> <h4 id=\"base-url\">Base URL:</h4> <p><a href=\"https://api.monei.com/v1\">https://api.monei.com/v1</a></p> <h4 id=\"client-libraries\">Client libraries:</h4> <ul> <li><a href=\"https://github.com/MONEI/monei-php-sdk\">PHP SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-python-sdk\">Python SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-node-sdk\">Node.js SDK</a></li> <li><a href=\"https://postman.monei.com/\">Postman Collection</a></li> </ul> <h4 id=\"important\">Important:</h4> <p><strong>If you are not using our official SDKs, you need to provide a valid <code>User-Agent</code> header in each request, otherwise your requests will be rejected.</strong></p>   # noqa: E501
+    <p>The MONEI API is organized around <a href=\"https://en.wikipedia.org/wiki/Representational_State_Transfer\">REST</a>. Our API has predictable resource-oriented URLs, accepts JSON-encoded request bodies, returns JSON-encoded responses, and uses standard HTTP response codes, authentication, and verbs.</p> <h4 id=\"base-url\">Base URL:</h4> <p><a href=\"https://api.monei.com/v1\">https://api.monei.com/v1</a></p> <h4 id=\"client-libraries\">Client libraries:</h4> <ul> <li><a href=\"https://github.com/MONEI/monei-php-sdk\">PHP SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-python-sdk\">Python SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-node-sdk\">Node.js SDK</a></li> <li><a href=\"https://postman.monei.com/\">Postman</a></li> </ul> <h4 id=\"important\">Important:</h4> <p><strong>If you are not using our official SDKs, you need to provide a valid <code>User-Agent</code> header in each request, otherwise your requests will be rejected.</strong></p>   # noqa: E501
 
-    The version of the OpenAPI document: 1.3.3
+    The version of the OpenAPI document: 1.4.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `Monei-1.1.3/Monei/models/payment_payment_method_bizum.py` & `Monei-1.2.0/Monei/models/payment_payment_method_bizum.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     MONEI API v1
 
-    <p>The MONEI API is organized around <a href=\"https://en.wikipedia.org/wiki/Representational_State_Transfer\">REST</a>. Our API has predictable resource-oriented URLs, accepts JSON-encoded request bodies, returns JSON-encoded responses, and uses standard HTTP response codes, authentication, and verbs.</p> <h4 id=\"base-url\">Base URL:</h4> <p><a href=\"https://api.monei.com/v1\">https://api.monei.com/v1</a></p> <h4 id=\"client-libraries\">Client libraries:</h4> <ul> <li><a href=\"https://github.com/MONEI/monei-php-sdk\">PHP SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-python-sdk\">Python SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-node-sdk\">Node.js SDK</a></li> <li><a href=\"https://postman.monei.com/\">Postman Collection</a></li> </ul> <h4 id=\"important\">Important:</h4> <p><strong>If you are not using our official SDKs, you need to provide a valid <code>User-Agent</code> header in each request, otherwise your requests will be rejected.</strong></p>   # noqa: E501
+    <p>The MONEI API is organized around <a href=\"https://en.wikipedia.org/wiki/Representational_State_Transfer\">REST</a>. Our API has predictable resource-oriented URLs, accepts JSON-encoded request bodies, returns JSON-encoded responses, and uses standard HTTP response codes, authentication, and verbs.</p> <h4 id=\"base-url\">Base URL:</h4> <p><a href=\"https://api.monei.com/v1\">https://api.monei.com/v1</a></p> <h4 id=\"client-libraries\">Client libraries:</h4> <ul> <li><a href=\"https://github.com/MONEI/monei-php-sdk\">PHP SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-python-sdk\">Python SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-node-sdk\">Node.js SDK</a></li> <li><a href=\"https://postman.monei.com/\">Postman</a></li> </ul> <h4 id=\"important\">Important:</h4> <p><strong>If you are not using our official SDKs, you need to provide a valid <code>User-Agent</code> header in each request, otherwise your requests will be rejected.</strong></p>   # noqa: E501
 
-    The version of the OpenAPI document: 1.3.3
+    The version of the OpenAPI document: 1.4.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `Monei-1.1.3/Monei/models/payment_payment_method_bizum_input.py` & `Monei-1.2.0/Monei/models/payment_payment_method_bizum_input.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     MONEI API v1
 
-    <p>The MONEI API is organized around <a href=\"https://en.wikipedia.org/wiki/Representational_State_Transfer\">REST</a>. Our API has predictable resource-oriented URLs, accepts JSON-encoded request bodies, returns JSON-encoded responses, and uses standard HTTP response codes, authentication, and verbs.</p> <h4 id=\"base-url\">Base URL:</h4> <p><a href=\"https://api.monei.com/v1\">https://api.monei.com/v1</a></p> <h4 id=\"client-libraries\">Client libraries:</h4> <ul> <li><a href=\"https://github.com/MONEI/monei-php-sdk\">PHP SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-python-sdk\">Python SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-node-sdk\">Node.js SDK</a></li> <li><a href=\"https://postman.monei.com/\">Postman Collection</a></li> </ul> <h4 id=\"important\">Important:</h4> <p><strong>If you are not using our official SDKs, you need to provide a valid <code>User-Agent</code> header in each request, otherwise your requests will be rejected.</strong></p>   # noqa: E501
+    <p>The MONEI API is organized around <a href=\"https://en.wikipedia.org/wiki/Representational_State_Transfer\">REST</a>. Our API has predictable resource-oriented URLs, accepts JSON-encoded request bodies, returns JSON-encoded responses, and uses standard HTTP response codes, authentication, and verbs.</p> <h4 id=\"base-url\">Base URL:</h4> <p><a href=\"https://api.monei.com/v1\">https://api.monei.com/v1</a></p> <h4 id=\"client-libraries\">Client libraries:</h4> <ul> <li><a href=\"https://github.com/MONEI/monei-php-sdk\">PHP SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-python-sdk\">Python SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-node-sdk\">Node.js SDK</a></li> <li><a href=\"https://postman.monei.com/\">Postman</a></li> </ul> <h4 id=\"important\">Important:</h4> <p><strong>If you are not using our official SDKs, you need to provide a valid <code>User-Agent</code> header in each request, otherwise your requests will be rejected.</strong></p>   # noqa: E501
 
-    The version of the OpenAPI document: 1.3.3
+    The version of the OpenAPI document: 1.4.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `Monei-1.1.3/Monei/models/payment_payment_method_card.py` & `Monei-1.2.0/Monei/models/payment_payment_method_card.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     MONEI API v1
 
-    <p>The MONEI API is organized around <a href=\"https://en.wikipedia.org/wiki/Representational_State_Transfer\">REST</a>. Our API has predictable resource-oriented URLs, accepts JSON-encoded request bodies, returns JSON-encoded responses, and uses standard HTTP response codes, authentication, and verbs.</p> <h4 id=\"base-url\">Base URL:</h4> <p><a href=\"https://api.monei.com/v1\">https://api.monei.com/v1</a></p> <h4 id=\"client-libraries\">Client libraries:</h4> <ul> <li><a href=\"https://github.com/MONEI/monei-php-sdk\">PHP SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-python-sdk\">Python SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-node-sdk\">Node.js SDK</a></li> <li><a href=\"https://postman.monei.com/\">Postman Collection</a></li> </ul> <h4 id=\"important\">Important:</h4> <p><strong>If you are not using our official SDKs, you need to provide a valid <code>User-Agent</code> header in each request, otherwise your requests will be rejected.</strong></p>   # noqa: E501
+    <p>The MONEI API is organized around <a href=\"https://en.wikipedia.org/wiki/Representational_State_Transfer\">REST</a>. Our API has predictable resource-oriented URLs, accepts JSON-encoded request bodies, returns JSON-encoded responses, and uses standard HTTP response codes, authentication, and verbs.</p> <h4 id=\"base-url\">Base URL:</h4> <p><a href=\"https://api.monei.com/v1\">https://api.monei.com/v1</a></p> <h4 id=\"client-libraries\">Client libraries:</h4> <ul> <li><a href=\"https://github.com/MONEI/monei-php-sdk\">PHP SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-python-sdk\">Python SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-node-sdk\">Node.js SDK</a></li> <li><a href=\"https://postman.monei.com/\">Postman</a></li> </ul> <h4 id=\"important\">Important:</h4> <p><strong>If you are not using our official SDKs, you need to provide a valid <code>User-Agent</code> header in each request, otherwise your requests will be rejected.</strong></p>   # noqa: E501
 
-    The version of the OpenAPI document: 1.3.3
+    The version of the OpenAPI document: 1.4.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `Monei-1.1.3/Monei/models/payment_payment_method_card_input.py` & `Monei-1.2.0/Monei/models/payment_payment_method_card_input.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     MONEI API v1
 
-    <p>The MONEI API is organized around <a href=\"https://en.wikipedia.org/wiki/Representational_State_Transfer\">REST</a>. Our API has predictable resource-oriented URLs, accepts JSON-encoded request bodies, returns JSON-encoded responses, and uses standard HTTP response codes, authentication, and verbs.</p> <h4 id=\"base-url\">Base URL:</h4> <p><a href=\"https://api.monei.com/v1\">https://api.monei.com/v1</a></p> <h4 id=\"client-libraries\">Client libraries:</h4> <ul> <li><a href=\"https://github.com/MONEI/monei-php-sdk\">PHP SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-python-sdk\">Python SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-node-sdk\">Node.js SDK</a></li> <li><a href=\"https://postman.monei.com/\">Postman Collection</a></li> </ul> <h4 id=\"important\">Important:</h4> <p><strong>If you are not using our official SDKs, you need to provide a valid <code>User-Agent</code> header in each request, otherwise your requests will be rejected.</strong></p>   # noqa: E501
+    <p>The MONEI API is organized around <a href=\"https://en.wikipedia.org/wiki/Representational_State_Transfer\">REST</a>. Our API has predictable resource-oriented URLs, accepts JSON-encoded request bodies, returns JSON-encoded responses, and uses standard HTTP response codes, authentication, and verbs.</p> <h4 id=\"base-url\">Base URL:</h4> <p><a href=\"https://api.monei.com/v1\">https://api.monei.com/v1</a></p> <h4 id=\"client-libraries\">Client libraries:</h4> <ul> <li><a href=\"https://github.com/MONEI/monei-php-sdk\">PHP SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-python-sdk\">Python SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-node-sdk\">Node.js SDK</a></li> <li><a href=\"https://postman.monei.com/\">Postman</a></li> </ul> <h4 id=\"important\">Important:</h4> <p><strong>If you are not using our official SDKs, you need to provide a valid <code>User-Agent</code> header in each request, otherwise your requests will be rejected.</strong></p>   # noqa: E501
 
-    The version of the OpenAPI document: 1.3.3
+    The version of the OpenAPI document: 1.4.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `Monei-1.1.3/Monei/models/payment_payment_method_cofidis.py` & `Monei-1.2.0/Monei/models/payment_payment_method_cofidis.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     MONEI API v1
 
-    <p>The MONEI API is organized around <a href=\"https://en.wikipedia.org/wiki/Representational_State_Transfer\">REST</a>. Our API has predictable resource-oriented URLs, accepts JSON-encoded request bodies, returns JSON-encoded responses, and uses standard HTTP response codes, authentication, and verbs.</p> <h4 id=\"base-url\">Base URL:</h4> <p><a href=\"https://api.monei.com/v1\">https://api.monei.com/v1</a></p> <h4 id=\"client-libraries\">Client libraries:</h4> <ul> <li><a href=\"https://github.com/MONEI/monei-php-sdk\">PHP SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-python-sdk\">Python SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-node-sdk\">Node.js SDK</a></li> <li><a href=\"https://postman.monei.com/\">Postman Collection</a></li> </ul> <h4 id=\"important\">Important:</h4> <p><strong>If you are not using our official SDKs, you need to provide a valid <code>User-Agent</code> header in each request, otherwise your requests will be rejected.</strong></p>   # noqa: E501
+    <p>The MONEI API is organized around <a href=\"https://en.wikipedia.org/wiki/Representational_State_Transfer\">REST</a>. Our API has predictable resource-oriented URLs, accepts JSON-encoded request bodies, returns JSON-encoded responses, and uses standard HTTP response codes, authentication, and verbs.</p> <h4 id=\"base-url\">Base URL:</h4> <p><a href=\"https://api.monei.com/v1\">https://api.monei.com/v1</a></p> <h4 id=\"client-libraries\">Client libraries:</h4> <ul> <li><a href=\"https://github.com/MONEI/monei-php-sdk\">PHP SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-python-sdk\">Python SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-node-sdk\">Node.js SDK</a></li> <li><a href=\"https://postman.monei.com/\">Postman</a></li> </ul> <h4 id=\"important\">Important:</h4> <p><strong>If you are not using our official SDKs, you need to provide a valid <code>User-Agent</code> header in each request, otherwise your requests will be rejected.</strong></p>   # noqa: E501
 
-    The version of the OpenAPI document: 1.3.3
+    The version of the OpenAPI document: 1.4.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `Monei-1.1.3/Monei/models/payment_payment_method_input.py` & `Monei-1.2.0/Monei/models/payment_payment_method_input.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     MONEI API v1
 
-    <p>The MONEI API is organized around <a href=\"https://en.wikipedia.org/wiki/Representational_State_Transfer\">REST</a>. Our API has predictable resource-oriented URLs, accepts JSON-encoded request bodies, returns JSON-encoded responses, and uses standard HTTP response codes, authentication, and verbs.</p> <h4 id=\"base-url\">Base URL:</h4> <p><a href=\"https://api.monei.com/v1\">https://api.monei.com/v1</a></p> <h4 id=\"client-libraries\">Client libraries:</h4> <ul> <li><a href=\"https://github.com/MONEI/monei-php-sdk\">PHP SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-python-sdk\">Python SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-node-sdk\">Node.js SDK</a></li> <li><a href=\"https://postman.monei.com/\">Postman Collection</a></li> </ul> <h4 id=\"important\">Important:</h4> <p><strong>If you are not using our official SDKs, you need to provide a valid <code>User-Agent</code> header in each request, otherwise your requests will be rejected.</strong></p>   # noqa: E501
+    <p>The MONEI API is organized around <a href=\"https://en.wikipedia.org/wiki/Representational_State_Transfer\">REST</a>. Our API has predictable resource-oriented URLs, accepts JSON-encoded request bodies, returns JSON-encoded responses, and uses standard HTTP response codes, authentication, and verbs.</p> <h4 id=\"base-url\">Base URL:</h4> <p><a href=\"https://api.monei.com/v1\">https://api.monei.com/v1</a></p> <h4 id=\"client-libraries\">Client libraries:</h4> <ul> <li><a href=\"https://github.com/MONEI/monei-php-sdk\">PHP SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-python-sdk\">Python SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-node-sdk\">Node.js SDK</a></li> <li><a href=\"https://postman.monei.com/\">Postman</a></li> </ul> <h4 id=\"important\">Important:</h4> <p><strong>If you are not using our official SDKs, you need to provide a valid <code>User-Agent</code> header in each request, otherwise your requests will be rejected.</strong></p>   # noqa: E501
 
-    The version of the OpenAPI document: 1.3.3
+    The version of the OpenAPI document: 1.4.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `Monei-1.1.3/Monei/models/payment_payment_method_paypal.py` & `Monei-1.2.0/Monei/models/payment_payment_method_paypal.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     MONEI API v1
 
-    <p>The MONEI API is organized around <a href=\"https://en.wikipedia.org/wiki/Representational_State_Transfer\">REST</a>. Our API has predictable resource-oriented URLs, accepts JSON-encoded request bodies, returns JSON-encoded responses, and uses standard HTTP response codes, authentication, and verbs.</p> <h4 id=\"base-url\">Base URL:</h4> <p><a href=\"https://api.monei.com/v1\">https://api.monei.com/v1</a></p> <h4 id=\"client-libraries\">Client libraries:</h4> <ul> <li><a href=\"https://github.com/MONEI/monei-php-sdk\">PHP SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-python-sdk\">Python SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-node-sdk\">Node.js SDK</a></li> <li><a href=\"https://postman.monei.com/\">Postman Collection</a></li> </ul> <h4 id=\"important\">Important:</h4> <p><strong>If you are not using our official SDKs, you need to provide a valid <code>User-Agent</code> header in each request, otherwise your requests will be rejected.</strong></p>   # noqa: E501
+    <p>The MONEI API is organized around <a href=\"https://en.wikipedia.org/wiki/Representational_State_Transfer\">REST</a>. Our API has predictable resource-oriented URLs, accepts JSON-encoded request bodies, returns JSON-encoded responses, and uses standard HTTP response codes, authentication, and verbs.</p> <h4 id=\"base-url\">Base URL:</h4> <p><a href=\"https://api.monei.com/v1\">https://api.monei.com/v1</a></p> <h4 id=\"client-libraries\">Client libraries:</h4> <ul> <li><a href=\"https://github.com/MONEI/monei-php-sdk\">PHP SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-python-sdk\">Python SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-node-sdk\">Node.js SDK</a></li> <li><a href=\"https://postman.monei.com/\">Postman</a></li> </ul> <h4 id=\"important\">Important:</h4> <p><strong>If you are not using our official SDKs, you need to provide a valid <code>User-Agent</code> header in each request, otherwise your requests will be rejected.</strong></p>   # noqa: E501
 
-    The version of the OpenAPI document: 1.3.3
+    The version of the OpenAPI document: 1.4.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `Monei-1.1.3/Monei/models/payment_refund_reason.py` & `Monei-1.2.0/Monei/models/payment_refund_reason.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     MONEI API v1
 
-    <p>The MONEI API is organized around <a href=\"https://en.wikipedia.org/wiki/Representational_State_Transfer\">REST</a>. Our API has predictable resource-oriented URLs, accepts JSON-encoded request bodies, returns JSON-encoded responses, and uses standard HTTP response codes, authentication, and verbs.</p> <h4 id=\"base-url\">Base URL:</h4> <p><a href=\"https://api.monei.com/v1\">https://api.monei.com/v1</a></p> <h4 id=\"client-libraries\">Client libraries:</h4> <ul> <li><a href=\"https://github.com/MONEI/monei-php-sdk\">PHP SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-python-sdk\">Python SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-node-sdk\">Node.js SDK</a></li> <li><a href=\"https://postman.monei.com/\">Postman Collection</a></li> </ul> <h4 id=\"important\">Important:</h4> <p><strong>If you are not using our official SDKs, you need to provide a valid <code>User-Agent</code> header in each request, otherwise your requests will be rejected.</strong></p>   # noqa: E501
+    <p>The MONEI API is organized around <a href=\"https://en.wikipedia.org/wiki/Representational_State_Transfer\">REST</a>. Our API has predictable resource-oriented URLs, accepts JSON-encoded request bodies, returns JSON-encoded responses, and uses standard HTTP response codes, authentication, and verbs.</p> <h4 id=\"base-url\">Base URL:</h4> <p><a href=\"https://api.monei.com/v1\">https://api.monei.com/v1</a></p> <h4 id=\"client-libraries\">Client libraries:</h4> <ul> <li><a href=\"https://github.com/MONEI/monei-php-sdk\">PHP SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-python-sdk\">Python SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-node-sdk\">Node.js SDK</a></li> <li><a href=\"https://postman.monei.com/\">Postman</a></li> </ul> <h4 id=\"important\">Important:</h4> <p><strong>If you are not using our official SDKs, you need to provide a valid <code>User-Agent</code> header in each request, otherwise your requests will be rejected.</strong></p>   # noqa: E501
 
-    The version of the OpenAPI document: 1.3.3
+    The version of the OpenAPI document: 1.4.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `Monei-1.1.3/Monei/models/payment_sequence.py` & `Monei-1.2.0/Monei/models/payment_sequence.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     MONEI API v1
 
-    <p>The MONEI API is organized around <a href=\"https://en.wikipedia.org/wiki/Representational_State_Transfer\">REST</a>. Our API has predictable resource-oriented URLs, accepts JSON-encoded request bodies, returns JSON-encoded responses, and uses standard HTTP response codes, authentication, and verbs.</p> <h4 id=\"base-url\">Base URL:</h4> <p><a href=\"https://api.monei.com/v1\">https://api.monei.com/v1</a></p> <h4 id=\"client-libraries\">Client libraries:</h4> <ul> <li><a href=\"https://github.com/MONEI/monei-php-sdk\">PHP SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-python-sdk\">Python SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-node-sdk\">Node.js SDK</a></li> <li><a href=\"https://postman.monei.com/\">Postman Collection</a></li> </ul> <h4 id=\"important\">Important:</h4> <p><strong>If you are not using our official SDKs, you need to provide a valid <code>User-Agent</code> header in each request, otherwise your requests will be rejected.</strong></p>   # noqa: E501
+    <p>The MONEI API is organized around <a href=\"https://en.wikipedia.org/wiki/Representational_State_Transfer\">REST</a>. Our API has predictable resource-oriented URLs, accepts JSON-encoded request bodies, returns JSON-encoded responses, and uses standard HTTP response codes, authentication, and verbs.</p> <h4 id=\"base-url\">Base URL:</h4> <p><a href=\"https://api.monei.com/v1\">https://api.monei.com/v1</a></p> <h4 id=\"client-libraries\">Client libraries:</h4> <ul> <li><a href=\"https://github.com/MONEI/monei-php-sdk\">PHP SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-python-sdk\">Python SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-node-sdk\">Node.js SDK</a></li> <li><a href=\"https://postman.monei.com/\">Postman</a></li> </ul> <h4 id=\"important\">Important:</h4> <p><strong>If you are not using our official SDKs, you need to provide a valid <code>User-Agent</code> header in each request, otherwise your requests will be rejected.</strong></p>   # noqa: E501
 
-    The version of the OpenAPI document: 1.3.3
+    The version of the OpenAPI document: 1.4.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `Monei-1.1.3/Monei/models/payment_sequence_recurring.py` & `Monei-1.2.0/Monei/models/payment_sequence_recurring.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     MONEI API v1
 
-    <p>The MONEI API is organized around <a href=\"https://en.wikipedia.org/wiki/Representational_State_Transfer\">REST</a>. Our API has predictable resource-oriented URLs, accepts JSON-encoded request bodies, returns JSON-encoded responses, and uses standard HTTP response codes, authentication, and verbs.</p> <h4 id=\"base-url\">Base URL:</h4> <p><a href=\"https://api.monei.com/v1\">https://api.monei.com/v1</a></p> <h4 id=\"client-libraries\">Client libraries:</h4> <ul> <li><a href=\"https://github.com/MONEI/monei-php-sdk\">PHP SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-python-sdk\">Python SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-node-sdk\">Node.js SDK</a></li> <li><a href=\"https://postman.monei.com/\">Postman Collection</a></li> </ul> <h4 id=\"important\">Important:</h4> <p><strong>If you are not using our official SDKs, you need to provide a valid <code>User-Agent</code> header in each request, otherwise your requests will be rejected.</strong></p>   # noqa: E501
+    <p>The MONEI API is organized around <a href=\"https://en.wikipedia.org/wiki/Representational_State_Transfer\">REST</a>. Our API has predictable resource-oriented URLs, accepts JSON-encoded request bodies, returns JSON-encoded responses, and uses standard HTTP response codes, authentication, and verbs.</p> <h4 id=\"base-url\">Base URL:</h4> <p><a href=\"https://api.monei.com/v1\">https://api.monei.com/v1</a></p> <h4 id=\"client-libraries\">Client libraries:</h4> <ul> <li><a href=\"https://github.com/MONEI/monei-php-sdk\">PHP SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-python-sdk\">Python SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-node-sdk\">Node.js SDK</a></li> <li><a href=\"https://postman.monei.com/\">Postman</a></li> </ul> <h4 id=\"important\">Important:</h4> <p><strong>If you are not using our official SDKs, you need to provide a valid <code>User-Agent</code> header in each request, otherwise your requests will be rejected.</strong></p>   # noqa: E501
 
-    The version of the OpenAPI document: 1.3.3
+    The version of the OpenAPI document: 1.4.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `Monei-1.1.3/Monei/models/payment_session_details.py` & `Monei-1.2.0/Monei/models/payment_session_details.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     MONEI API v1
 
-    <p>The MONEI API is organized around <a href=\"https://en.wikipedia.org/wiki/Representational_State_Transfer\">REST</a>. Our API has predictable resource-oriented URLs, accepts JSON-encoded request bodies, returns JSON-encoded responses, and uses standard HTTP response codes, authentication, and verbs.</p> <h4 id=\"base-url\">Base URL:</h4> <p><a href=\"https://api.monei.com/v1\">https://api.monei.com/v1</a></p> <h4 id=\"client-libraries\">Client libraries:</h4> <ul> <li><a href=\"https://github.com/MONEI/monei-php-sdk\">PHP SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-python-sdk\">Python SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-node-sdk\">Node.js SDK</a></li> <li><a href=\"https://postman.monei.com/\">Postman Collection</a></li> </ul> <h4 id=\"important\">Important:</h4> <p><strong>If you are not using our official SDKs, you need to provide a valid <code>User-Agent</code> header in each request, otherwise your requests will be rejected.</strong></p>   # noqa: E501
+    <p>The MONEI API is organized around <a href=\"https://en.wikipedia.org/wiki/Representational_State_Transfer\">REST</a>. Our API has predictable resource-oriented URLs, accepts JSON-encoded request bodies, returns JSON-encoded responses, and uses standard HTTP response codes, authentication, and verbs.</p> <h4 id=\"base-url\">Base URL:</h4> <p><a href=\"https://api.monei.com/v1\">https://api.monei.com/v1</a></p> <h4 id=\"client-libraries\">Client libraries:</h4> <ul> <li><a href=\"https://github.com/MONEI/monei-php-sdk\">PHP SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-python-sdk\">Python SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-node-sdk\">Node.js SDK</a></li> <li><a href=\"https://postman.monei.com/\">Postman</a></li> </ul> <h4 id=\"important\">Important:</h4> <p><strong>If you are not using our official SDKs, you need to provide a valid <code>User-Agent</code> header in each request, otherwise your requests will be rejected.</strong></p>   # noqa: E501
 
-    The version of the OpenAPI document: 1.3.3
+    The version of the OpenAPI document: 1.4.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `Monei-1.1.3/Monei/models/payment_shipping_details.py` & `Monei-1.2.0/Monei/models/payment_shipping_details.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     MONEI API v1
 
-    <p>The MONEI API is organized around <a href=\"https://en.wikipedia.org/wiki/Representational_State_Transfer\">REST</a>. Our API has predictable resource-oriented URLs, accepts JSON-encoded request bodies, returns JSON-encoded responses, and uses standard HTTP response codes, authentication, and verbs.</p> <h4 id=\"base-url\">Base URL:</h4> <p><a href=\"https://api.monei.com/v1\">https://api.monei.com/v1</a></p> <h4 id=\"client-libraries\">Client libraries:</h4> <ul> <li><a href=\"https://github.com/MONEI/monei-php-sdk\">PHP SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-python-sdk\">Python SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-node-sdk\">Node.js SDK</a></li> <li><a href=\"https://postman.monei.com/\">Postman Collection</a></li> </ul> <h4 id=\"important\">Important:</h4> <p><strong>If you are not using our official SDKs, you need to provide a valid <code>User-Agent</code> header in each request, otherwise your requests will be rejected.</strong></p>   # noqa: E501
+    <p>The MONEI API is organized around <a href=\"https://en.wikipedia.org/wiki/Representational_State_Transfer\">REST</a>. Our API has predictable resource-oriented URLs, accepts JSON-encoded request bodies, returns JSON-encoded responses, and uses standard HTTP response codes, authentication, and verbs.</p> <h4 id=\"base-url\">Base URL:</h4> <p><a href=\"https://api.monei.com/v1\">https://api.monei.com/v1</a></p> <h4 id=\"client-libraries\">Client libraries:</h4> <ul> <li><a href=\"https://github.com/MONEI/monei-php-sdk\">PHP SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-python-sdk\">Python SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-node-sdk\">Node.js SDK</a></li> <li><a href=\"https://postman.monei.com/\">Postman</a></li> </ul> <h4 id=\"important\">Important:</h4> <p><strong>If you are not using our official SDKs, you need to provide a valid <code>User-Agent</code> header in each request, otherwise your requests will be rejected.</strong></p>   # noqa: E501
 
-    The version of the OpenAPI document: 1.3.3
+    The version of the OpenAPI document: 1.4.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `Monei-1.1.3/Monei/models/payment_shop.py` & `Monei-1.2.0/Monei/models/payment_shop.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     MONEI API v1
 
-    <p>The MONEI API is organized around <a href=\"https://en.wikipedia.org/wiki/Representational_State_Transfer\">REST</a>. Our API has predictable resource-oriented URLs, accepts JSON-encoded request bodies, returns JSON-encoded responses, and uses standard HTTP response codes, authentication, and verbs.</p> <h4 id=\"base-url\">Base URL:</h4> <p><a href=\"https://api.monei.com/v1\">https://api.monei.com/v1</a></p> <h4 id=\"client-libraries\">Client libraries:</h4> <ul> <li><a href=\"https://github.com/MONEI/monei-php-sdk\">PHP SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-python-sdk\">Python SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-node-sdk\">Node.js SDK</a></li> <li><a href=\"https://postman.monei.com/\">Postman Collection</a></li> </ul> <h4 id=\"important\">Important:</h4> <p><strong>If you are not using our official SDKs, you need to provide a valid <code>User-Agent</code> header in each request, otherwise your requests will be rejected.</strong></p>   # noqa: E501
+    <p>The MONEI API is organized around <a href=\"https://en.wikipedia.org/wiki/Representational_State_Transfer\">REST</a>. Our API has predictable resource-oriented URLs, accepts JSON-encoded request bodies, returns JSON-encoded responses, and uses standard HTTP response codes, authentication, and verbs.</p> <h4 id=\"base-url\">Base URL:</h4> <p><a href=\"https://api.monei.com/v1\">https://api.monei.com/v1</a></p> <h4 id=\"client-libraries\">Client libraries:</h4> <ul> <li><a href=\"https://github.com/MONEI/monei-php-sdk\">PHP SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-python-sdk\">Python SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-node-sdk\">Node.js SDK</a></li> <li><a href=\"https://postman.monei.com/\">Postman</a></li> </ul> <h4 id=\"important\">Important:</h4> <p><strong>If you are not using our official SDKs, you need to provide a valid <code>User-Agent</code> header in each request, otherwise your requests will be rejected.</strong></p>   # noqa: E501
 
-    The version of the OpenAPI document: 1.3.3
+    The version of the OpenAPI document: 1.4.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `Monei-1.1.3/Monei/models/payment_status.py` & `Monei-1.2.0/Monei/models/payment_status.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     MONEI API v1
 
-    <p>The MONEI API is organized around <a href=\"https://en.wikipedia.org/wiki/Representational_State_Transfer\">REST</a>. Our API has predictable resource-oriented URLs, accepts JSON-encoded request bodies, returns JSON-encoded responses, and uses standard HTTP response codes, authentication, and verbs.</p> <h4 id=\"base-url\">Base URL:</h4> <p><a href=\"https://api.monei.com/v1\">https://api.monei.com/v1</a></p> <h4 id=\"client-libraries\">Client libraries:</h4> <ul> <li><a href=\"https://github.com/MONEI/monei-php-sdk\">PHP SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-python-sdk\">Python SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-node-sdk\">Node.js SDK</a></li> <li><a href=\"https://postman.monei.com/\">Postman Collection</a></li> </ul> <h4 id=\"important\">Important:</h4> <p><strong>If you are not using our official SDKs, you need to provide a valid <code>User-Agent</code> header in each request, otherwise your requests will be rejected.</strong></p>   # noqa: E501
+    <p>The MONEI API is organized around <a href=\"https://en.wikipedia.org/wiki/Representational_State_Transfer\">REST</a>. Our API has predictable resource-oriented URLs, accepts JSON-encoded request bodies, returns JSON-encoded responses, and uses standard HTTP response codes, authentication, and verbs.</p> <h4 id=\"base-url\">Base URL:</h4> <p><a href=\"https://api.monei.com/v1\">https://api.monei.com/v1</a></p> <h4 id=\"client-libraries\">Client libraries:</h4> <ul> <li><a href=\"https://github.com/MONEI/monei-php-sdk\">PHP SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-python-sdk\">Python SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-node-sdk\">Node.js SDK</a></li> <li><a href=\"https://postman.monei.com/\">Postman</a></li> </ul> <h4 id=\"important\">Important:</h4> <p><strong>If you are not using our official SDKs, you need to provide a valid <code>User-Agent</code> header in each request, otherwise your requests will be rejected.</strong></p>   # noqa: E501
 
-    The version of the OpenAPI document: 1.3.3
+    The version of the OpenAPI document: 1.4.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `Monei-1.1.3/Monei/models/payment_trace_details.py` & `Monei-1.2.0/Monei/models/payment_trace_details.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     MONEI API v1
 
-    <p>The MONEI API is organized around <a href=\"https://en.wikipedia.org/wiki/Representational_State_Transfer\">REST</a>. Our API has predictable resource-oriented URLs, accepts JSON-encoded request bodies, returns JSON-encoded responses, and uses standard HTTP response codes, authentication, and verbs.</p> <h4 id=\"base-url\">Base URL:</h4> <p><a href=\"https://api.monei.com/v1\">https://api.monei.com/v1</a></p> <h4 id=\"client-libraries\">Client libraries:</h4> <ul> <li><a href=\"https://github.com/MONEI/monei-php-sdk\">PHP SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-python-sdk\">Python SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-node-sdk\">Node.js SDK</a></li> <li><a href=\"https://postman.monei.com/\">Postman Collection</a></li> </ul> <h4 id=\"important\">Important:</h4> <p><strong>If you are not using our official SDKs, you need to provide a valid <code>User-Agent</code> header in each request, otherwise your requests will be rejected.</strong></p>   # noqa: E501
+    <p>The MONEI API is organized around <a href=\"https://en.wikipedia.org/wiki/Representational_State_Transfer\">REST</a>. Our API has predictable resource-oriented URLs, accepts JSON-encoded request bodies, returns JSON-encoded responses, and uses standard HTTP response codes, authentication, and verbs.</p> <h4 id=\"base-url\">Base URL:</h4> <p><a href=\"https://api.monei.com/v1\">https://api.monei.com/v1</a></p> <h4 id=\"client-libraries\">Client libraries:</h4> <ul> <li><a href=\"https://github.com/MONEI/monei-php-sdk\">PHP SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-python-sdk\">Python SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-node-sdk\">Node.js SDK</a></li> <li><a href=\"https://postman.monei.com/\">Postman</a></li> </ul> <h4 id=\"important\">Important:</h4> <p><strong>If you are not using our official SDKs, you need to provide a valid <code>User-Agent</code> header in each request, otherwise your requests will be rejected.</strong></p>   # noqa: E501
 
-    The version of the OpenAPI document: 1.3.3
+    The version of the OpenAPI document: 1.4.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `Monei-1.1.3/Monei/models/payment_transaction_type.py` & `Monei-1.2.0/Monei/models/payment_transaction_type.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     MONEI API v1
 
-    <p>The MONEI API is organized around <a href=\"https://en.wikipedia.org/wiki/Representational_State_Transfer\">REST</a>. Our API has predictable resource-oriented URLs, accepts JSON-encoded request bodies, returns JSON-encoded responses, and uses standard HTTP response codes, authentication, and verbs.</p> <h4 id=\"base-url\">Base URL:</h4> <p><a href=\"https://api.monei.com/v1\">https://api.monei.com/v1</a></p> <h4 id=\"client-libraries\">Client libraries:</h4> <ul> <li><a href=\"https://github.com/MONEI/monei-php-sdk\">PHP SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-python-sdk\">Python SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-node-sdk\">Node.js SDK</a></li> <li><a href=\"https://postman.monei.com/\">Postman Collection</a></li> </ul> <h4 id=\"important\">Important:</h4> <p><strong>If you are not using our official SDKs, you need to provide a valid <code>User-Agent</code> header in each request, otherwise your requests will be rejected.</strong></p>   # noqa: E501
+    <p>The MONEI API is organized around <a href=\"https://en.wikipedia.org/wiki/Representational_State_Transfer\">REST</a>. Our API has predictable resource-oriented URLs, accepts JSON-encoded request bodies, returns JSON-encoded responses, and uses standard HTTP response codes, authentication, and verbs.</p> <h4 id=\"base-url\">Base URL:</h4> <p><a href=\"https://api.monei.com/v1\">https://api.monei.com/v1</a></p> <h4 id=\"client-libraries\">Client libraries:</h4> <ul> <li><a href=\"https://github.com/MONEI/monei-php-sdk\">PHP SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-python-sdk\">Python SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-node-sdk\">Node.js SDK</a></li> <li><a href=\"https://postman.monei.com/\">Postman</a></li> </ul> <h4 id=\"important\">Important:</h4> <p><strong>If you are not using our official SDKs, you need to provide a valid <code>User-Agent</code> header in each request, otherwise your requests will be rejected.</strong></p>   # noqa: E501
 
-    The version of the OpenAPI document: 1.3.3
+    The version of the OpenAPI document: 1.4.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `Monei-1.1.3/Monei/models/recurring_payment_request.py` & `Monei-1.2.0/Monei/models/recurring_payment_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     MONEI API v1
 
-    <p>The MONEI API is organized around <a href=\"https://en.wikipedia.org/wiki/Representational_State_Transfer\">REST</a>. Our API has predictable resource-oriented URLs, accepts JSON-encoded request bodies, returns JSON-encoded responses, and uses standard HTTP response codes, authentication, and verbs.</p> <h4 id=\"base-url\">Base URL:</h4> <p><a href=\"https://api.monei.com/v1\">https://api.monei.com/v1</a></p> <h4 id=\"client-libraries\">Client libraries:</h4> <ul> <li><a href=\"https://github.com/MONEI/monei-php-sdk\">PHP SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-python-sdk\">Python SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-node-sdk\">Node.js SDK</a></li> <li><a href=\"https://postman.monei.com/\">Postman Collection</a></li> </ul> <h4 id=\"important\">Important:</h4> <p><strong>If you are not using our official SDKs, you need to provide a valid <code>User-Agent</code> header in each request, otherwise your requests will be rejected.</strong></p>   # noqa: E501
+    <p>The MONEI API is organized around <a href=\"https://en.wikipedia.org/wiki/Representational_State_Transfer\">REST</a>. Our API has predictable resource-oriented URLs, accepts JSON-encoded request bodies, returns JSON-encoded responses, and uses standard HTTP response codes, authentication, and verbs.</p> <h4 id=\"base-url\">Base URL:</h4> <p><a href=\"https://api.monei.com/v1\">https://api.monei.com/v1</a></p> <h4 id=\"client-libraries\">Client libraries:</h4> <ul> <li><a href=\"https://github.com/MONEI/monei-php-sdk\">PHP SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-python-sdk\">Python SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-node-sdk\">Node.js SDK</a></li> <li><a href=\"https://postman.monei.com/\">Postman</a></li> </ul> <h4 id=\"important\">Important:</h4> <p><strong>If you are not using our official SDKs, you need to provide a valid <code>User-Agent</code> header in each request, otherwise your requests will be rejected.</strong></p>   # noqa: E501
 
-    The version of the OpenAPI document: 1.3.3
+    The version of the OpenAPI document: 1.4.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `Monei-1.1.3/Monei/models/refund_payment_request.py` & `Monei-1.2.0/Monei/models/refund_payment_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     MONEI API v1
 
-    <p>The MONEI API is organized around <a href=\"https://en.wikipedia.org/wiki/Representational_State_Transfer\">REST</a>. Our API has predictable resource-oriented URLs, accepts JSON-encoded request bodies, returns JSON-encoded responses, and uses standard HTTP response codes, authentication, and verbs.</p> <h4 id=\"base-url\">Base URL:</h4> <p><a href=\"https://api.monei.com/v1\">https://api.monei.com/v1</a></p> <h4 id=\"client-libraries\">Client libraries:</h4> <ul> <li><a href=\"https://github.com/MONEI/monei-php-sdk\">PHP SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-python-sdk\">Python SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-node-sdk\">Node.js SDK</a></li> <li><a href=\"https://postman.monei.com/\">Postman Collection</a></li> </ul> <h4 id=\"important\">Important:</h4> <p><strong>If you are not using our official SDKs, you need to provide a valid <code>User-Agent</code> header in each request, otherwise your requests will be rejected.</strong></p>   # noqa: E501
+    <p>The MONEI API is organized around <a href=\"https://en.wikipedia.org/wiki/Representational_State_Transfer\">REST</a>. Our API has predictable resource-oriented URLs, accepts JSON-encoded request bodies, returns JSON-encoded responses, and uses standard HTTP response codes, authentication, and verbs.</p> <h4 id=\"base-url\">Base URL:</h4> <p><a href=\"https://api.monei.com/v1\">https://api.monei.com/v1</a></p> <h4 id=\"client-libraries\">Client libraries:</h4> <ul> <li><a href=\"https://github.com/MONEI/monei-php-sdk\">PHP SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-python-sdk\">Python SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-node-sdk\">Node.js SDK</a></li> <li><a href=\"https://postman.monei.com/\">Postman</a></li> </ul> <h4 id=\"important\">Important:</h4> <p><strong>If you are not using our official SDKs, you need to provide a valid <code>User-Agent</code> header in each request, otherwise your requests will be rejected.</strong></p>   # noqa: E501
 
-    The version of the OpenAPI document: 1.3.3
+    The version of the OpenAPI document: 1.4.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `Monei-1.1.3/Monei/models/register_domain_request.py` & `Monei-1.2.0/Monei/models/register_domain_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     MONEI API v1
 
-    <p>The MONEI API is organized around <a href=\"https://en.wikipedia.org/wiki/Representational_State_Transfer\">REST</a>. Our API has predictable resource-oriented URLs, accepts JSON-encoded request bodies, returns JSON-encoded responses, and uses standard HTTP response codes, authentication, and verbs.</p> <h4 id=\"base-url\">Base URL:</h4> <p><a href=\"https://api.monei.com/v1\">https://api.monei.com/v1</a></p> <h4 id=\"client-libraries\">Client libraries:</h4> <ul> <li><a href=\"https://github.com/MONEI/monei-php-sdk\">PHP SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-python-sdk\">Python SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-node-sdk\">Node.js SDK</a></li> <li><a href=\"https://postman.monei.com/\">Postman Collection</a></li> </ul> <h4 id=\"important\">Important:</h4> <p><strong>If you are not using our official SDKs, you need to provide a valid <code>User-Agent</code> header in each request, otherwise your requests will be rejected.</strong></p>   # noqa: E501
+    <p>The MONEI API is organized around <a href=\"https://en.wikipedia.org/wiki/Representational_State_Transfer\">REST</a>. Our API has predictable resource-oriented URLs, accepts JSON-encoded request bodies, returns JSON-encoded responses, and uses standard HTTP response codes, authentication, and verbs.</p> <h4 id=\"base-url\">Base URL:</h4> <p><a href=\"https://api.monei.com/v1\">https://api.monei.com/v1</a></p> <h4 id=\"client-libraries\">Client libraries:</h4> <ul> <li><a href=\"https://github.com/MONEI/monei-php-sdk\">PHP SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-python-sdk\">Python SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-node-sdk\">Node.js SDK</a></li> <li><a href=\"https://postman.monei.com/\">Postman</a></li> </ul> <h4 id=\"important\">Important:</h4> <p><strong>If you are not using our official SDKs, you need to provide a valid <code>User-Agent</code> header in each request, otherwise your requests will be rejected.</strong></p>   # noqa: E501
 
-    The version of the OpenAPI document: 1.3.3
+    The version of the OpenAPI document: 1.4.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `Monei-1.1.3/Monei/models/send_payment_link_request.py` & `Monei-1.2.0/Monei/models/send_payment_link_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     MONEI API v1
 
-    <p>The MONEI API is organized around <a href=\"https://en.wikipedia.org/wiki/Representational_State_Transfer\">REST</a>. Our API has predictable resource-oriented URLs, accepts JSON-encoded request bodies, returns JSON-encoded responses, and uses standard HTTP response codes, authentication, and verbs.</p> <h4 id=\"base-url\">Base URL:</h4> <p><a href=\"https://api.monei.com/v1\">https://api.monei.com/v1</a></p> <h4 id=\"client-libraries\">Client libraries:</h4> <ul> <li><a href=\"https://github.com/MONEI/monei-php-sdk\">PHP SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-python-sdk\">Python SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-node-sdk\">Node.js SDK</a></li> <li><a href=\"https://postman.monei.com/\">Postman Collection</a></li> </ul> <h4 id=\"important\">Important:</h4> <p><strong>If you are not using our official SDKs, you need to provide a valid <code>User-Agent</code> header in each request, otherwise your requests will be rejected.</strong></p>   # noqa: E501
+    <p>The MONEI API is organized around <a href=\"https://en.wikipedia.org/wiki/Representational_State_Transfer\">REST</a>. Our API has predictable resource-oriented URLs, accepts JSON-encoded request bodies, returns JSON-encoded responses, and uses standard HTTP response codes, authentication, and verbs.</p> <h4 id=\"base-url\">Base URL:</h4> <p><a href=\"https://api.monei.com/v1\">https://api.monei.com/v1</a></p> <h4 id=\"client-libraries\">Client libraries:</h4> <ul> <li><a href=\"https://github.com/MONEI/monei-php-sdk\">PHP SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-python-sdk\">Python SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-node-sdk\">Node.js SDK</a></li> <li><a href=\"https://postman.monei.com/\">Postman</a></li> </ul> <h4 id=\"important\">Important:</h4> <p><strong>If you are not using our official SDKs, you need to provide a valid <code>User-Agent</code> header in each request, otherwise your requests will be rejected.</strong></p>   # noqa: E501
 
-    The version of the OpenAPI document: 1.3.3
+    The version of the OpenAPI document: 1.4.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `Monei-1.1.3/Monei/models/send_payment_receipt_request.py` & `Monei-1.2.0/Monei/models/send_payment_receipt_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     MONEI API v1
 
-    <p>The MONEI API is organized around <a href=\"https://en.wikipedia.org/wiki/Representational_State_Transfer\">REST</a>. Our API has predictable resource-oriented URLs, accepts JSON-encoded request bodies, returns JSON-encoded responses, and uses standard HTTP response codes, authentication, and verbs.</p> <h4 id=\"base-url\">Base URL:</h4> <p><a href=\"https://api.monei.com/v1\">https://api.monei.com/v1</a></p> <h4 id=\"client-libraries\">Client libraries:</h4> <ul> <li><a href=\"https://github.com/MONEI/monei-php-sdk\">PHP SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-python-sdk\">Python SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-node-sdk\">Node.js SDK</a></li> <li><a href=\"https://postman.monei.com/\">Postman Collection</a></li> </ul> <h4 id=\"important\">Important:</h4> <p><strong>If you are not using our official SDKs, you need to provide a valid <code>User-Agent</code> header in each request, otherwise your requests will be rejected.</strong></p>   # noqa: E501
+    <p>The MONEI API is organized around <a href=\"https://en.wikipedia.org/wiki/Representational_State_Transfer\">REST</a>. Our API has predictable resource-oriented URLs, accepts JSON-encoded request bodies, returns JSON-encoded responses, and uses standard HTTP response codes, authentication, and verbs.</p> <h4 id=\"base-url\">Base URL:</h4> <p><a href=\"https://api.monei.com/v1\">https://api.monei.com/v1</a></p> <h4 id=\"client-libraries\">Client libraries:</h4> <ul> <li><a href=\"https://github.com/MONEI/monei-php-sdk\">PHP SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-python-sdk\">Python SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-node-sdk\">Node.js SDK</a></li> <li><a href=\"https://postman.monei.com/\">Postman</a></li> </ul> <h4 id=\"important\">Important:</h4> <p><strong>If you are not using our official SDKs, you need to provide a valid <code>User-Agent</code> header in each request, otherwise your requests will be rejected.</strong></p>   # noqa: E501
 
-    The version of the OpenAPI document: 1.3.3
+    The version of the OpenAPI document: 1.4.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `Monei-1.1.3/Monei/models/subscription.py` & `Monei-1.2.0/Monei/models/subscription.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     MONEI API v1
 
-    <p>The MONEI API is organized around <a href=\"https://en.wikipedia.org/wiki/Representational_State_Transfer\">REST</a>. Our API has predictable resource-oriented URLs, accepts JSON-encoded request bodies, returns JSON-encoded responses, and uses standard HTTP response codes, authentication, and verbs.</p> <h4 id=\"base-url\">Base URL:</h4> <p><a href=\"https://api.monei.com/v1\">https://api.monei.com/v1</a></p> <h4 id=\"client-libraries\">Client libraries:</h4> <ul> <li><a href=\"https://github.com/MONEI/monei-php-sdk\">PHP SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-python-sdk\">Python SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-node-sdk\">Node.js SDK</a></li> <li><a href=\"https://postman.monei.com/\">Postman Collection</a></li> </ul> <h4 id=\"important\">Important:</h4> <p><strong>If you are not using our official SDKs, you need to provide a valid <code>User-Agent</code> header in each request, otherwise your requests will be rejected.</strong></p>   # noqa: E501
+    <p>The MONEI API is organized around <a href=\"https://en.wikipedia.org/wiki/Representational_State_Transfer\">REST</a>. Our API has predictable resource-oriented URLs, accepts JSON-encoded request bodies, returns JSON-encoded responses, and uses standard HTTP response codes, authentication, and verbs.</p> <h4 id=\"base-url\">Base URL:</h4> <p><a href=\"https://api.monei.com/v1\">https://api.monei.com/v1</a></p> <h4 id=\"client-libraries\">Client libraries:</h4> <ul> <li><a href=\"https://github.com/MONEI/monei-php-sdk\">PHP SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-python-sdk\">Python SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-node-sdk\">Node.js SDK</a></li> <li><a href=\"https://postman.monei.com/\">Postman</a></li> </ul> <h4 id=\"important\">Important:</h4> <p><strong>If you are not using our official SDKs, you need to provide a valid <code>User-Agent</code> header in each request, otherwise your requests will be rejected.</strong></p>   # noqa: E501
 
-    The version of the OpenAPI document: 1.3.3
+    The version of the OpenAPI document: 1.4.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `Monei-1.1.3/Monei/models/subscription_interval.py` & `Monei-1.2.0/Monei/models/subscription_interval.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     MONEI API v1
 
-    <p>The MONEI API is organized around <a href=\"https://en.wikipedia.org/wiki/Representational_State_Transfer\">REST</a>. Our API has predictable resource-oriented URLs, accepts JSON-encoded request bodies, returns JSON-encoded responses, and uses standard HTTP response codes, authentication, and verbs.</p> <h4 id=\"base-url\">Base URL:</h4> <p><a href=\"https://api.monei.com/v1\">https://api.monei.com/v1</a></p> <h4 id=\"client-libraries\">Client libraries:</h4> <ul> <li><a href=\"https://github.com/MONEI/monei-php-sdk\">PHP SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-python-sdk\">Python SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-node-sdk\">Node.js SDK</a></li> <li><a href=\"https://postman.monei.com/\">Postman Collection</a></li> </ul> <h4 id=\"important\">Important:</h4> <p><strong>If you are not using our official SDKs, you need to provide a valid <code>User-Agent</code> header in each request, otherwise your requests will be rejected.</strong></p>   # noqa: E501
+    <p>The MONEI API is organized around <a href=\"https://en.wikipedia.org/wiki/Representational_State_Transfer\">REST</a>. Our API has predictable resource-oriented URLs, accepts JSON-encoded request bodies, returns JSON-encoded responses, and uses standard HTTP response codes, authentication, and verbs.</p> <h4 id=\"base-url\">Base URL:</h4> <p><a href=\"https://api.monei.com/v1\">https://api.monei.com/v1</a></p> <h4 id=\"client-libraries\">Client libraries:</h4> <ul> <li><a href=\"https://github.com/MONEI/monei-php-sdk\">PHP SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-python-sdk\">Python SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-node-sdk\">Node.js SDK</a></li> <li><a href=\"https://postman.monei.com/\">Postman</a></li> </ul> <h4 id=\"important\">Important:</h4> <p><strong>If you are not using our official SDKs, you need to provide a valid <code>User-Agent</code> header in each request, otherwise your requests will be rejected.</strong></p>   # noqa: E501
 
-    The version of the OpenAPI document: 1.3.3
+    The version of the OpenAPI document: 1.4.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `Monei-1.1.3/Monei/models/subscription_last_payment.py` & `Monei-1.2.0/Monei/models/subscription_last_payment.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     MONEI API v1
 
-    <p>The MONEI API is organized around <a href=\"https://en.wikipedia.org/wiki/Representational_State_Transfer\">REST</a>. Our API has predictable resource-oriented URLs, accepts JSON-encoded request bodies, returns JSON-encoded responses, and uses standard HTTP response codes, authentication, and verbs.</p> <h4 id=\"base-url\">Base URL:</h4> <p><a href=\"https://api.monei.com/v1\">https://api.monei.com/v1</a></p> <h4 id=\"client-libraries\">Client libraries:</h4> <ul> <li><a href=\"https://github.com/MONEI/monei-php-sdk\">PHP SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-python-sdk\">Python SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-node-sdk\">Node.js SDK</a></li> <li><a href=\"https://postman.monei.com/\">Postman Collection</a></li> </ul> <h4 id=\"important\">Important:</h4> <p><strong>If you are not using our official SDKs, you need to provide a valid <code>User-Agent</code> header in each request, otherwise your requests will be rejected.</strong></p>   # noqa: E501
+    <p>The MONEI API is organized around <a href=\"https://en.wikipedia.org/wiki/Representational_State_Transfer\">REST</a>. Our API has predictable resource-oriented URLs, accepts JSON-encoded request bodies, returns JSON-encoded responses, and uses standard HTTP response codes, authentication, and verbs.</p> <h4 id=\"base-url\">Base URL:</h4> <p><a href=\"https://api.monei.com/v1\">https://api.monei.com/v1</a></p> <h4 id=\"client-libraries\">Client libraries:</h4> <ul> <li><a href=\"https://github.com/MONEI/monei-php-sdk\">PHP SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-python-sdk\">Python SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-node-sdk\">Node.js SDK</a></li> <li><a href=\"https://postman.monei.com/\">Postman</a></li> </ul> <h4 id=\"important\">Important:</h4> <p><strong>If you are not using our official SDKs, you need to provide a valid <code>User-Agent</code> header in each request, otherwise your requests will be rejected.</strong></p>   # noqa: E501
 
-    The version of the OpenAPI document: 1.3.3
+    The version of the OpenAPI document: 1.4.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `Monei-1.1.3/Monei/models/subscription_payment_method.py` & `Monei-1.2.0/Monei/models/subscription_payment_method.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     MONEI API v1
 
-    <p>The MONEI API is organized around <a href=\"https://en.wikipedia.org/wiki/Representational_State_Transfer\">REST</a>. Our API has predictable resource-oriented URLs, accepts JSON-encoded request bodies, returns JSON-encoded responses, and uses standard HTTP response codes, authentication, and verbs.</p> <h4 id=\"base-url\">Base URL:</h4> <p><a href=\"https://api.monei.com/v1\">https://api.monei.com/v1</a></p> <h4 id=\"client-libraries\">Client libraries:</h4> <ul> <li><a href=\"https://github.com/MONEI/monei-php-sdk\">PHP SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-python-sdk\">Python SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-node-sdk\">Node.js SDK</a></li> <li><a href=\"https://postman.monei.com/\">Postman Collection</a></li> </ul> <h4 id=\"important\">Important:</h4> <p><strong>If you are not using our official SDKs, you need to provide a valid <code>User-Agent</code> header in each request, otherwise your requests will be rejected.</strong></p>   # noqa: E501
+    <p>The MONEI API is organized around <a href=\"https://en.wikipedia.org/wiki/Representational_State_Transfer\">REST</a>. Our API has predictable resource-oriented URLs, accepts JSON-encoded request bodies, returns JSON-encoded responses, and uses standard HTTP response codes, authentication, and verbs.</p> <h4 id=\"base-url\">Base URL:</h4> <p><a href=\"https://api.monei.com/v1\">https://api.monei.com/v1</a></p> <h4 id=\"client-libraries\">Client libraries:</h4> <ul> <li><a href=\"https://github.com/MONEI/monei-php-sdk\">PHP SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-python-sdk\">Python SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-node-sdk\">Node.js SDK</a></li> <li><a href=\"https://postman.monei.com/\">Postman</a></li> </ul> <h4 id=\"important\">Important:</h4> <p><strong>If you are not using our official SDKs, you need to provide a valid <code>User-Agent</code> header in each request, otherwise your requests will be rejected.</strong></p>   # noqa: E501
 
-    The version of the OpenAPI document: 1.3.3
+    The version of the OpenAPI document: 1.4.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `Monei-1.1.3/Monei/models/subscription_payment_method_card.py` & `Monei-1.2.0/Monei/models/subscription_payment_method_card.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     MONEI API v1
 
-    <p>The MONEI API is organized around <a href=\"https://en.wikipedia.org/wiki/Representational_State_Transfer\">REST</a>. Our API has predictable resource-oriented URLs, accepts JSON-encoded request bodies, returns JSON-encoded responses, and uses standard HTTP response codes, authentication, and verbs.</p> <h4 id=\"base-url\">Base URL:</h4> <p><a href=\"https://api.monei.com/v1\">https://api.monei.com/v1</a></p> <h4 id=\"client-libraries\">Client libraries:</h4> <ul> <li><a href=\"https://github.com/MONEI/monei-php-sdk\">PHP SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-python-sdk\">Python SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-node-sdk\">Node.js SDK</a></li> <li><a href=\"https://postman.monei.com/\">Postman Collection</a></li> </ul> <h4 id=\"important\">Important:</h4> <p><strong>If you are not using our official SDKs, you need to provide a valid <code>User-Agent</code> header in each request, otherwise your requests will be rejected.</strong></p>   # noqa: E501
+    <p>The MONEI API is organized around <a href=\"https://en.wikipedia.org/wiki/Representational_State_Transfer\">REST</a>. Our API has predictable resource-oriented URLs, accepts JSON-encoded request bodies, returns JSON-encoded responses, and uses standard HTTP response codes, authentication, and verbs.</p> <h4 id=\"base-url\">Base URL:</h4> <p><a href=\"https://api.monei.com/v1\">https://api.monei.com/v1</a></p> <h4 id=\"client-libraries\">Client libraries:</h4> <ul> <li><a href=\"https://github.com/MONEI/monei-php-sdk\">PHP SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-python-sdk\">Python SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-node-sdk\">Node.js SDK</a></li> <li><a href=\"https://postman.monei.com/\">Postman</a></li> </ul> <h4 id=\"important\">Important:</h4> <p><strong>If you are not using our official SDKs, you need to provide a valid <code>User-Agent</code> header in each request, otherwise your requests will be rejected.</strong></p>   # noqa: E501
 
-    The version of the OpenAPI document: 1.3.3
+    The version of the OpenAPI document: 1.4.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `Monei-1.1.3/Monei/models/subscription_status.py` & `Monei-1.2.0/Monei/models/subscription_status.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     MONEI API v1
 
-    <p>The MONEI API is organized around <a href=\"https://en.wikipedia.org/wiki/Representational_State_Transfer\">REST</a>. Our API has predictable resource-oriented URLs, accepts JSON-encoded request bodies, returns JSON-encoded responses, and uses standard HTTP response codes, authentication, and verbs.</p> <h4 id=\"base-url\">Base URL:</h4> <p><a href=\"https://api.monei.com/v1\">https://api.monei.com/v1</a></p> <h4 id=\"client-libraries\">Client libraries:</h4> <ul> <li><a href=\"https://github.com/MONEI/monei-php-sdk\">PHP SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-python-sdk\">Python SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-node-sdk\">Node.js SDK</a></li> <li><a href=\"https://postman.monei.com/\">Postman Collection</a></li> </ul> <h4 id=\"important\">Important:</h4> <p><strong>If you are not using our official SDKs, you need to provide a valid <code>User-Agent</code> header in each request, otherwise your requests will be rejected.</strong></p>   # noqa: E501
+    <p>The MONEI API is organized around <a href=\"https://en.wikipedia.org/wiki/Representational_State_Transfer\">REST</a>. Our API has predictable resource-oriented URLs, accepts JSON-encoded request bodies, returns JSON-encoded responses, and uses standard HTTP response codes, authentication, and verbs.</p> <h4 id=\"base-url\">Base URL:</h4> <p><a href=\"https://api.monei.com/v1\">https://api.monei.com/v1</a></p> <h4 id=\"client-libraries\">Client libraries:</h4> <ul> <li><a href=\"https://github.com/MONEI/monei-php-sdk\">PHP SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-python-sdk\">Python SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-node-sdk\">Node.js SDK</a></li> <li><a href=\"https://postman.monei.com/\">Postman</a></li> </ul> <h4 id=\"important\">Important:</h4> <p><strong>If you are not using our official SDKs, you need to provide a valid <code>User-Agent</code> header in each request, otherwise your requests will be rejected.</strong></p>   # noqa: E501
 
-    The version of the OpenAPI document: 1.3.3
+    The version of the OpenAPI document: 1.4.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `Monei-1.1.3/Monei/models/update_subscription_request.py` & `Monei-1.2.0/Monei/models/update_subscription_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     MONEI API v1
 
-    <p>The MONEI API is organized around <a href=\"https://en.wikipedia.org/wiki/Representational_State_Transfer\">REST</a>. Our API has predictable resource-oriented URLs, accepts JSON-encoded request bodies, returns JSON-encoded responses, and uses standard HTTP response codes, authentication, and verbs.</p> <h4 id=\"base-url\">Base URL:</h4> <p><a href=\"https://api.monei.com/v1\">https://api.monei.com/v1</a></p> <h4 id=\"client-libraries\">Client libraries:</h4> <ul> <li><a href=\"https://github.com/MONEI/monei-php-sdk\">PHP SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-python-sdk\">Python SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-node-sdk\">Node.js SDK</a></li> <li><a href=\"https://postman.monei.com/\">Postman Collection</a></li> </ul> <h4 id=\"important\">Important:</h4> <p><strong>If you are not using our official SDKs, you need to provide a valid <code>User-Agent</code> header in each request, otherwise your requests will be rejected.</strong></p>   # noqa: E501
+    <p>The MONEI API is organized around <a href=\"https://en.wikipedia.org/wiki/Representational_State_Transfer\">REST</a>. Our API has predictable resource-oriented URLs, accepts JSON-encoded request bodies, returns JSON-encoded responses, and uses standard HTTP response codes, authentication, and verbs.</p> <h4 id=\"base-url\">Base URL:</h4> <p><a href=\"https://api.monei.com/v1\">https://api.monei.com/v1</a></p> <h4 id=\"client-libraries\">Client libraries:</h4> <ul> <li><a href=\"https://github.com/MONEI/monei-php-sdk\">PHP SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-python-sdk\">Python SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-node-sdk\">Node.js SDK</a></li> <li><a href=\"https://postman.monei.com/\">Postman</a></li> </ul> <h4 id=\"important\">Important:</h4> <p><strong>If you are not using our official SDKs, you need to provide a valid <code>User-Agent</code> header in each request, otherwise your requests will be rejected.</strong></p>   # noqa: E501
 
-    The version of the OpenAPI document: 1.3.3
+    The version of the OpenAPI document: 1.4.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `Monei-1.1.3/Monei/monei_client.py` & `Monei-1.2.0/Monei/monei_client.py`

 * *Files identical despite different names*

### Comparing `Monei-1.1.3/Monei/rest.py` & `Monei-1.2.0/Monei/rest.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     MONEI API v1
 
-    <p>The MONEI API is organized around <a href=\"https://en.wikipedia.org/wiki/Representational_State_Transfer\">REST</a>. Our API has predictable resource-oriented URLs, accepts JSON-encoded request bodies, returns JSON-encoded responses, and uses standard HTTP response codes, authentication, and verbs.</p> <h4 id=\"base-url\">Base URL:</h4> <p><a href=\"https://api.monei.com/v1\">https://api.monei.com/v1</a></p> <h4 id=\"client-libraries\">Client libraries:</h4> <ul> <li><a href=\"https://github.com/MONEI/monei-php-sdk\">PHP SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-python-sdk\">Python SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-node-sdk\">Node.js SDK</a></li> <li><a href=\"https://postman.monei.com/\">Postman Collection</a></li> </ul> <h4 id=\"important\">Important:</h4> <p><strong>If you are not using our official SDKs, you need to provide a valid <code>User-Agent</code> header in each request, otherwise your requests will be rejected.</strong></p>   # noqa: E501
+    <p>The MONEI API is organized around <a href=\"https://en.wikipedia.org/wiki/Representational_State_Transfer\">REST</a>. Our API has predictable resource-oriented URLs, accepts JSON-encoded request bodies, returns JSON-encoded responses, and uses standard HTTP response codes, authentication, and verbs.</p> <h4 id=\"base-url\">Base URL:</h4> <p><a href=\"https://api.monei.com/v1\">https://api.monei.com/v1</a></p> <h4 id=\"client-libraries\">Client libraries:</h4> <ul> <li><a href=\"https://github.com/MONEI/monei-php-sdk\">PHP SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-python-sdk\">Python SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-node-sdk\">Node.js SDK</a></li> <li><a href=\"https://postman.monei.com/\">Postman</a></li> </ul> <h4 id=\"important\">Important:</h4> <p><strong>If you are not using our official SDKs, you need to provide a valid <code>User-Agent</code> header in each request, otherwise your requests will be rejected.</strong></p>   # noqa: E501
 
-    The version of the OpenAPI document: 1.3.3
+    The version of the OpenAPI document: 1.4.0
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import io
```

### Comparing `Monei-1.1.3/Monei.egg-info/PKG-INFO` & `Monei-1.2.0/Monei.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Monei
-Version: 1.1.3
+Version: 1.2.0
 Summary: MONEI PYTHON SDK
 Home-page: https://github.com/monei/monei-python-sdk
 Author: MONEI
 Author-email: hi@monei.com
 Maintainer: MONEI
 Maintainer-email: support@monei.com
 Keywords: monei,monei pay,pay,payments,payment gateway,python,sdk,rest,api
```

### Comparing `Monei-1.1.3/Monei.egg-info/SOURCES.txt` & `Monei-1.2.0/Monei.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -111,14 +111,15 @@
 Monei/models/payment_trace_details.py
 Monei/models/payment_transaction_type.py
 Monei/models/recurring_payment_request.py
 Monei/models/refund_payment_request.py
 Monei/models/register_domain_request.py
 Monei/models/send_payment_link_request.py
 Monei/models/send_payment_receipt_request.py
+Monei/models/send_payment_request.py
 Monei/models/subscription.py
 Monei/models/subscription_interval.py
 Monei/models/subscription_last_payment.py
 Monei/models/subscription_payment_method.py
 Monei/models/subscription_payment_method_card.py
 Monei/models/subscription_status.py
 Monei/models/update_subscription_request.py
@@ -167,14 +168,15 @@
 test/test_payment_transaction_type.py
 test/test_payments_api.py
 test/test_recurring_payment_request.py
 test/test_refund_payment_request.py
 test/test_register_domain_request.py
 test/test_send_payment_link_request.py
 test/test_send_payment_receipt_request.py
+test/test_send_payment_request.py
 test/test_subscription.py
 test/test_subscription_interval.py
 test/test_subscription_last_payment.py
 test/test_subscription_payment_method.py
 test/test_subscription_payment_method_card.py
 test/test_subscription_status.py
 test/test_subscriptions_api.py
```

### Comparing `Monei-1.1.3/PKG-INFO` & `Monei-1.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Monei
-Version: 1.1.3
+Version: 1.2.0
 Summary: MONEI PYTHON SDK
 Home-page: https://github.com/monei/monei-python-sdk
 Author: MONEI
 Author-email: hi@monei.com
 Maintainer: MONEI
 Maintainer-email: support@monei.com
 Keywords: monei,monei pay,pay,payments,payment gateway,python,sdk,rest,api
```

### Comparing `Monei-1.1.3/README.md` & `Monei-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `Monei-1.1.3/setup.py` & `Monei-1.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `Monei-1.1.3/test/test_activate_subscription_request.py` & `Monei-1.2.0/test/test_activate_subscription_request.py`

 * *Files identical despite different names*

### Comparing `Monei-1.1.3/test/test_address.py` & `Monei-1.2.0/test/test_address.py`

 * *Files identical despite different names*

### Comparing `Monei-1.1.3/test/test_apple_pay_domain_api.py` & `Monei-1.2.0/test/test_apple_pay_domain_api.py`

 * *Files identical despite different names*

### Comparing `Monei-1.1.3/test/test_cancel_payment_request.py` & `Monei-1.2.0/test/test_cancel_payment_request.py`

 * *Files identical despite different names*

### Comparing `Monei-1.1.3/test/test_cancel_subscription_request.py` & `Monei-1.2.0/test/test_cancel_subscription_request.py`

 * *Files identical despite different names*

### Comparing `Monei-1.1.3/test/test_capture_payment_request.py` & `Monei-1.2.0/test/test_capture_payment_request.py`

 * *Files identical despite different names*

### Comparing `Monei-1.1.3/test/test_card.py` & `Monei-1.2.0/test/test_card.py`

 * *Files identical despite different names*

### Comparing `Monei-1.1.3/test/test_confirm_payment_request.py` & `Monei-1.2.0/test/test_confirm_payment_request.py`

 * *Files identical despite different names*

### Comparing `Monei-1.1.3/test/test_confirm_payment_request_payment_method.py` & `Monei-1.2.0/test/test_confirm_payment_request_payment_method.py`

 * *Files identical despite different names*

### Comparing `Monei-1.1.3/test/test_confirm_payment_request_payment_method_card.py` & `Monei-1.2.0/test/test_confirm_payment_request_payment_method_card.py`

 * *Files identical despite different names*

### Comparing `Monei-1.1.3/test/test_create_payment_request.py` & `Monei-1.2.0/test/test_create_payment_request.py`

 * *Files identical despite different names*

### Comparing `Monei-1.1.3/test/test_create_subscription_request.py` & `Monei-1.2.0/test/test_create_subscription_request.py`

 * *Files identical despite different names*

### Comparing `Monei-1.1.3/test/test_domain_register200_response.py` & `Monei-1.2.0/test/test_domain_register200_response.py`

 * *Files identical despite different names*

### Comparing `Monei-1.1.3/test/test_error.py` & `Monei-1.2.0/test/test_error.py`

 * *Files identical despite different names*

### Comparing `Monei-1.1.3/test/test_inline_object.py` & `Monei-1.2.0/test/test_inline_object.py`

 * *Files identical despite different names*

### Comparing `Monei-1.1.3/test/test_inline_response200.py` & `Monei-1.2.0/test/test_inline_response200.py`

 * *Files identical despite different names*

### Comparing `Monei-1.1.3/test/test_pause_subscription_request.py` & `Monei-1.2.0/test/test_pause_subscription_request.py`

 * *Files identical despite different names*

### Comparing `Monei-1.1.3/test/test_payment.py` & `Monei-1.2.0/test/test_payment.py`

 * *Files identical despite different names*

### Comparing `Monei-1.1.3/test/test_payment_billing_details.py` & `Monei-1.2.0/test/test_payment_billing_details.py`

 * *Files identical despite different names*

### Comparing `Monei-1.1.3/test/test_payment_cancellation_reason.py` & `Monei-1.2.0/test/test_payment_cancellation_reason.py`

 * *Files identical despite different names*

### Comparing `Monei-1.1.3/test/test_payment_customer.py` & `Monei-1.2.0/test/test_payment_customer.py`

 * *Files identical despite different names*

### Comparing `Monei-1.1.3/test/test_payment_last_refund_reason.py` & `Monei-1.2.0/test/test_payment_last_refund_reason.py`

 * *Files identical despite different names*

### Comparing `Monei-1.1.3/test/test_payment_message_channel.py` & `Monei-1.2.0/test/test_payment_message_channel.py`

 * *Files identical despite different names*

### Comparing `Monei-1.1.3/test/test_payment_message_language.py` & `Monei-1.2.0/test/test_payment_message_language.py`

 * *Files identical despite different names*

### Comparing `Monei-1.1.3/test/test_payment_next_action.py` & `Monei-1.2.0/test/test_payment_next_action.py`

 * *Files identical despite different names*

### Comparing `Monei-1.1.3/test/test_payment_payment_method.py` & `Monei-1.2.0/test/test_payment_payment_method.py`

 * *Files identical despite different names*

### Comparing `Monei-1.1.3/test/test_payment_payment_method_bizum.py` & `Monei-1.2.0/test/test_payment_payment_method_bizum.py`

 * *Files identical despite different names*

### Comparing `Monei-1.1.3/test/test_payment_payment_method_bizum_input.py` & `Monei-1.2.0/test/test_payment_payment_method_bizum_input.py`

 * *Files identical despite different names*

### Comparing `Monei-1.1.3/test/test_payment_payment_method_card.py` & `Monei-1.2.0/test/test_payment_payment_method_card.py`

 * *Files identical despite different names*

### Comparing `Monei-1.1.3/test/test_payment_payment_method_card_input.py` & `Monei-1.2.0/test/test_payment_payment_method_card_input.py`

 * *Files identical despite different names*

### Comparing `Monei-1.1.3/test/test_payment_payment_method_cofidis.py` & `Monei-1.2.0/test/test_payment_payment_method_cofidis.py`

 * *Files identical despite different names*

### Comparing `Monei-1.1.3/test/test_payment_payment_method_input.py` & `Monei-1.2.0/test/test_payment_payment_method_input.py`

 * *Files identical despite different names*

### Comparing `Monei-1.1.3/test/test_payment_payment_method_paypal.py` & `Monei-1.2.0/test/test_payment_payment_method_paypal.py`

 * *Files identical despite different names*

### Comparing `Monei-1.1.3/test/test_payment_payment_methods.py` & `Monei-1.2.0/test/test_payment_payment_methods.py`

 * *Files identical despite different names*

### Comparing `Monei-1.1.3/test/test_payment_refund_reason.py` & `Monei-1.2.0/test/test_payment_refund_reason.py`

 * *Files identical despite different names*

### Comparing `Monei-1.1.3/test/test_payment_sequence.py` & `Monei-1.2.0/test/test_payment_sequence.py`

 * *Files identical despite different names*

### Comparing `Monei-1.1.3/test/test_payment_sequence_recurring.py` & `Monei-1.2.0/test/test_payment_sequence_recurring.py`

 * *Files identical despite different names*

### Comparing `Monei-1.1.3/test/test_payment_session_details.py` & `Monei-1.2.0/test/test_payment_session_details.py`

 * *Files identical despite different names*

### Comparing `Monei-1.1.3/test/test_payment_shipping_details.py` & `Monei-1.2.0/test/test_payment_shipping_details.py`

 * *Files identical despite different names*

### Comparing `Monei-1.1.3/test/test_payment_shop.py` & `Monei-1.2.0/test/test_payment_shop.py`

 * *Files identical despite different names*

### Comparing `Monei-1.1.3/test/test_payment_status.py` & `Monei-1.2.0/test/test_payment_status.py`

 * *Files identical despite different names*

### Comparing `Monei-1.1.3/test/test_payment_trace_details.py` & `Monei-1.2.0/test/test_payment_trace_details.py`

 * *Files identical despite different names*

### Comparing `Monei-1.1.3/test/test_payment_transaction_type.py` & `Monei-1.2.0/test/test_payment_transaction_type.py`

 * *Files identical despite different names*

### Comparing `Monei-1.1.3/test/test_payments_api.py` & `Monei-1.2.0/test/test_payments_api.py`

 * *Files identical despite different names*

### Comparing `Monei-1.1.3/test/test_recurring_payment_request.py` & `Monei-1.2.0/test/test_recurring_payment_request.py`

 * *Files identical despite different names*

### Comparing `Monei-1.1.3/test/test_refund_payment_request.py` & `Monei-1.2.0/test/test_refund_payment_request.py`

 * *Files identical despite different names*

### Comparing `Monei-1.1.3/test/test_register_domain_request.py` & `Monei-1.2.0/test/test_register_domain_request.py`

 * *Files identical despite different names*

### Comparing `Monei-1.1.3/test/test_send_payment_link_request.py` & `Monei-1.2.0/test/test_send_payment_link_request.py`

 * *Files identical despite different names*

### Comparing `Monei-1.1.3/test/test_send_payment_receipt_request.py` & `Monei-1.2.0/test/test_send_payment_receipt_request.py`

 * *Files identical despite different names*

### Comparing `Monei-1.1.3/test/test_subscription.py` & `Monei-1.2.0/test/test_subscription.py`

 * *Files identical despite different names*

### Comparing `Monei-1.1.3/test/test_subscription_interval.py` & `Monei-1.2.0/test/test_subscription_interval.py`

 * *Files identical despite different names*

### Comparing `Monei-1.1.3/test/test_subscription_last_payment.py` & `Monei-1.2.0/test/test_subscription_last_payment.py`

 * *Files identical despite different names*

### Comparing `Monei-1.1.3/test/test_subscription_payment_method.py` & `Monei-1.2.0/test/test_subscription_payment_method.py`

 * *Files identical despite different names*

### Comparing `Monei-1.1.3/test/test_subscription_payment_method_card.py` & `Monei-1.2.0/test/test_subscription_payment_method_card.py`

 * *Files identical despite different names*

### Comparing `Monei-1.1.3/test/test_subscription_status.py` & `Monei-1.2.0/test/test_subscription_status.py`

 * *Files identical despite different names*

### Comparing `Monei-1.1.3/test/test_subscriptions_api.py` & `Monei-1.2.0/test/test_subscriptions_api.py`

 * *Files identical despite different names*

### Comparing `Monei-1.1.3/test/test_update_subscription_request.py` & `Monei-1.2.0/test/test_update_subscription_request.py`

 * *Files identical despite different names*

