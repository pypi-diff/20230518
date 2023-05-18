# Comparing `tmp/twilio-8.2.0.tar.gz` & `tmp/twilio-8.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "twilio-8.2.0.tar", last modified: Thu May  4 09:30:45 2023, max compression
+gzip compressed data, was "twilio-8.2.1.tar", last modified: Thu May 18 08:05:51 2023, max compression
```

## Comparing `twilio-8.2.0.tar` & `twilio-8.2.1.tar`

### file list

```diff
@@ -1,851 +1,855 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.332207 twilio-8.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1387 2023-05-04 09:30:30.000000 twilio-8.2.0/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-05-04 09:30:30.000000 twilio-8.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-05-04 09:30:30.000000 twilio-8.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    11938 2023-05-04 09:30:45.332207 twilio-8.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10921 2023-05-04 09:30:30.000000 twilio-8.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-05-04 09:30:45.332207 twilio-8.2.0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     1694 2023-05-04 09:30:30.000000 twilio-8.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.152205 twilio-8.2.0/twilio/
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.156205 twilio-8.2.0/twilio/base/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8153 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/base/client_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2019 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/base/deserialize.py
--rw-r--r--   0 runner    (1001) docker     (123)     2978 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/base/domain.py
--rw-r--r--   0 runner    (1001) docker     (123)     2890 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/base/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/base/instance_context.py
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/base/instance_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/base/list_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     1417 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/base/obsolete.py
--rw-r--r--   0 runner    (1001) docker     (123)     5181 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/base/page.py
--rw-r--r--   0 runner    (1001) docker     (123)     2039 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/base/serialize.py
--rw-r--r--   0 runner    (1001) docker     (123)      280 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/base/values.py
--rw-r--r--   0 runner    (1001) docker     (123)    14614 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/base/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.156205 twilio-8.2.0/twilio/http/
--rw-r--r--   0 runner    (1001) docker     (123)     3434 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/http/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4503 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/http/async_http_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     3735 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/http/http_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2655 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/http/request.py
--rw-r--r--   0 runner    (1001) docker     (123)      518 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/http/response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4810 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/http/validation_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.156205 twilio-8.2.0/twilio/jwt/
--rw-r--r--   0 runner    (1001) docker     (123)     5085 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/jwt/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.156205 twilio-8.2.0/twilio/jwt/access_token/
--rw-r--r--   0 runner    (1001) docker     (123)     2415 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/jwt/access_token/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4902 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/jwt/access_token/grants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.156205 twilio-8.2.0/twilio/jwt/client/
--rw-r--r--   0 runner    (1001) docker     (123)     3982 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/jwt/client/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.156205 twilio-8.2.0/twilio/jwt/taskrouter/
--rw-r--r--   0 runner    (1001) docker     (123)     5726 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/jwt/taskrouter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4309 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/jwt/taskrouter/capabilities.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.160205 twilio-8.2.0/twilio/jwt/validation/
--rw-r--r--   0 runner    (1001) docker     (123)     3156 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/jwt/validation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4100 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/request_validator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.160205 twilio-8.2.0/twilio/rest/
--rw-r--r--   0 runner    (1001) docker     (123)    20879 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.160205 twilio-8.2.0/twilio/rest/accounts/
--rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/accounts/AccountsBase.py
--rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/accounts/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.160205 twilio-8.2.0/twilio/rest/accounts/v1/
--rw-r--r--   0 runner    (1001) docker     (123)     2102 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/accounts/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5547 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/accounts/v1/auth_token_promotion.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.160205 twilio-8.2.0/twilio/rest/accounts/v1/credential/
--rw-r--r--   0 runner    (1001) docker     (123)     1766 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/accounts/v1/credential/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19489 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/accounts/v1/credential/aws.py
--rw-r--r--   0 runner    (1001) docker     (123)    20007 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/accounts/v1/credential/public_key.py
--rw-r--r--   0 runner    (1001) docker     (123)     6551 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/accounts/v1/secondary_auth_token.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.160205 twilio-8.2.0/twilio/rest/api/
--rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/api/ApiBase.py
--rw-r--r--   0 runner    (1001) docker     (123)     8255 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.160205 twilio-8.2.0/twilio/rest/api/v2010/
--rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/api/v2010/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.164205 twilio-8.2.0/twilio/rest/api/v2010/account/
--rw-r--r--   0 runner    (1001) docker     (123)    36206 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/api/v2010/account/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.164205 twilio-8.2.0/twilio/rest/api/v2010/account/address/
--rw-r--r--   0 runner    (1001) docker     (123)    35858 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/api/v2010/account/address/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17044 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/api/v2010/account/address/dependent_phone_number.py
--rw-r--r--   0 runner    (1001) docker     (123)    47553 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/api/v2010/account/application.py
--rw-r--r--   0 runner    (1001) docker     (123)    17274 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/api/v2010/account/authorized_connect_app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.164205 twilio-8.2.0/twilio/rest/api/v2010/account/available_phone_number_country/
--rw-r--r--   0 runner    (1001) docker     (123)    21427 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/api/v2010/account/available_phone_number_country/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    46239 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/api/v2010/account/available_phone_number_country/local.py
--rw-r--r--   0 runner    (1001) docker     (123)    46210 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/api/v2010/account/available_phone_number_country/machine_to_machine.py
--rw-r--r--   0 runner    (1001) docker     (123)    45860 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/api/v2010/account/available_phone_number_country/mobile.py
--rw-r--r--   0 runner    (1001) docker     (123)    45930 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/api/v2010/account/available_phone_number_country/national.py
--rw-r--r--   0 runner    (1001) docker     (123)    46000 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/api/v2010/account/available_phone_number_country/shared_cost.py
--rw-r--r--   0 runner    (1001) docker     (123)    45930 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/api/v2010/account/available_phone_number_country/toll_free.py
--rw-r--r--   0 runner    (1001) docker     (123)    45790 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/api/v2010/account/available_phone_number_country/voip.py
--rw-r--r--   0 runner    (1001) docker     (123)     3186 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/api/v2010/account/balance.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.168205 twilio-8.2.0/twilio/rest/api/v2010/account/call/
--rw-r--r--   0 runner    (1001) docker     (123)    92392 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/api/v2010/account/call/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10658 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/api/v2010/account/call/event.py
--rw-r--r--   0 runner    (1001) docker     (123)    11932 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/api/v2010/account/call/feedback.py
--rw-r--r--   0 runner    (1001) docker     (123)    13986 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/api/v2010/account/call/feedback_summary.py
--rw-r--r--   0 runner    (1001) docker     (123)    28363 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/api/v2010/account/call/notification.py
--rw-r--r--   0 runner    (1001) docker     (123)    23472 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/api/v2010/account/call/payment.py
--rw-r--r--   0 runner    (1001) docker     (123)    38495 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/api/v2010/account/call/recording.py
--rw-r--r--   0 runner    (1001) docker     (123)    77226 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/api/v2010/account/call/siprec.py
--rw-r--r--   0 runner    (1001) docker     (123)    77116 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/api/v2010/account/call/stream.py
--rw-r--r--   0 runner    (1001) docker     (123)     5278 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/api/v2010/account/call/user_defined_message.py
--rw-r--r--   0 runner    (1001) docker     (123)    10898 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/api/v2010/account/call/user_defined_message_subscription.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.168205 twilio-8.2.0/twilio/rest/api/v2010/account/conference/
--rw-r--r--   0 runner    (1001) docker     (123)    41186 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/api/v2010/account/conference/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    74737 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/api/v2010/account/conference/participant.py
--rw-r--r--   0 runner    (1001) docker     (123)    32729 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/api/v2010/account/conference/recording.py
--rw-r--r--   0 runner    (1001) docker     (123)    26539 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/api/v2010/account/connect_app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.172205 twilio-8.2.0/twilio/rest/api/v2010/account/incoming_phone_number/
--rw-r--r--   0 runner    (1001) docker     (123)    73374 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/api/v2010/account/incoming_phone_number/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.172205 twilio-8.2.0/twilio/rest/api/v2010/account/incoming_phone_number/assigned_add_on/
--rw-r--r--   0 runner    (1001) docker     (123)    20750 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/api/v2010/account/incoming_phone_number/assigned_add_on/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18341 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/api/v2010/account/incoming_phone_number/assigned_add_on/assigned_add_on_extension.py
--rw-r--r--   0 runner    (1001) docker     (123)    36935 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/api/v2010/account/incoming_phone_number/local.py
--rw-r--r--   0 runner    (1001) docker     (123)    37019 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/api/v2010/account/incoming_phone_number/mobile.py
--rw-r--r--   0 runner    (1001) docker     (123)    37103 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/api/v2010/account/incoming_phone_number/toll_free.py
--rw-r--r--   0 runner    (1001) docker     (123)    17989 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/api/v2010/account/key.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.172205 twilio-8.2.0/twilio/rest/api/v2010/account/message/
--rw-r--r--   0 runner    (1001) docker     (123)    53984 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/api/v2010/account/message/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5102 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/api/v2010/account/message/feedback.py
--rw-r--r--   0 runner    (1001) docker     (123)    27246 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/api/v2010/account/message/media.py
--rw-r--r--   0 runner    (1001) docker     (123)     4785 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/api/v2010/account/new_key.py
--rw-r--r--   0 runner    (1001) docker     (123)     4813 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/api/v2010/account/new_signing_key.py
--rw-r--r--   0 runner    (1001) docker     (123)    27505 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/api/v2010/account/notification.py
--rw-r--r--   0 runner    (1001) docker     (123)    22199 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/api/v2010/account/outgoing_caller_id.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.172205 twilio-8.2.0/twilio/rest/api/v2010/account/queue/
--rw-r--r--   0 runner    (1001) docker     (123)    22428 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/api/v2010/account/queue/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19131 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/api/v2010/account/queue/member.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.172205 twilio-8.2.0/twilio/rest/api/v2010/account/recording/
--rw-r--r--   0 runner    (1001) docker     (123)    37769 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/api/v2010/account/recording/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.172205 twilio-8.2.0/twilio/rest/api/v2010/account/recording/add_on_result/
--rw-r--r--   0 runner    (1001) docker     (123)    19239 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/api/v2010/account/recording/add_on_result/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19233 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/api/v2010/account/recording/add_on_result/payload.py
--rw-r--r--   0 runner    (1001) docker     (123)    19008 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/api/v2010/account/recording/transcription.py
--rw-r--r--   0 runner    (1001) docker     (123)    26406 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/api/v2010/account/short_code.py
--rw-r--r--   0 runner    (1001) docker     (123)    17376 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/api/v2010/account/signing_key.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.172205 twilio-8.2.0/twilio/rest/api/v2010/account/sip/
--rw-r--r--   0 runner    (1001) docker     (123)     2871 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/api/v2010/account/sip/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.172205 twilio-8.2.0/twilio/rest/api/v2010/account/sip/credential_list/
--rw-r--r--   0 runner    (1001) docker     (123)    21278 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/api/v2010/account/sip/credential_list/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22757 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/api/v2010/account/sip/credential_list/credential.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.172205 twilio-8.2.0/twilio/rest/api/v2010/account/sip/domain/
--rw-r--r--   0 runner    (1001) docker     (123)    45116 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/api/v2010/account/sip/domain/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.176205 twilio-8.2.0/twilio/rest/api/v2010/account/sip/domain/auth_types/
--rw-r--r--   0 runner    (1001) docker     (123)     2758 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/api/v2010/account/sip/domain/auth_types/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.176205 twilio-8.2.0/twilio/rest/api/v2010/account/sip/domain/auth_types/auth_type_calls/
--rw-r--r--   0 runner    (1001) docker     (123)     3330 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/api/v2010/account/sip/domain/auth_types/auth_type_calls/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20440 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/api/v2010/account/sip/domain/auth_types/auth_type_calls/auth_calls_credential_list_mapping.py
--rw-r--r--   0 runner    (1001) docker     (123)    20981 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/api/v2010/account/sip/domain/auth_types/auth_type_calls/auth_calls_ip_access_control_list_mapping.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.176205 twilio-8.2.0/twilio/rest/api/v2010/account/sip/domain/auth_types/auth_type_registrations/
--rw-r--r--   0 runner    (1001) docker     (123)     2473 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/api/v2010/account/sip/domain/auth_types/auth_type_registrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21048 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/api/v2010/account/sip/domain/auth_types/auth_type_registrations/auth_registrations_credential_list_mapping.py
--rw-r--r--   0 runner    (1001) docker     (123)    19893 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/api/v2010/account/sip/domain/credential_list_mapping.py
--rw-r--r--   0 runner    (1001) docker     (123)    20164 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/api/v2010/account/sip/domain/ip_access_control_list_mapping.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.176205 twilio-8.2.0/twilio/rest/api/v2010/account/sip/ip_access_control_list/
--rw-r--r--   0 runner    (1001) docker     (123)    21808 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/api/v2010/account/sip/ip_access_control_list/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    26238 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/api/v2010/account/sip/ip_access_control_list/ip_address.py
--rw-r--r--   0 runner    (1001) docker     (123)     4823 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/api/v2010/account/token.py
--rw-r--r--   0 runner    (1001) docker     (123)    18034 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/api/v2010/account/transcription.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.176205 twilio-8.2.0/twilio/rest/api/v2010/account/usage/
--rw-r--r--   0 runner    (1001) docker     (123)     2220 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/api/v2010/account/usage/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.180205 twilio-8.2.0/twilio/rest/api/v2010/account/usage/record/
--rw-r--r--   0 runner    (1001) docker     (123)    41695 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/api/v2010/account/usage/record/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    38339 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/api/v2010/account/usage/record/all_time.py
--rw-r--r--   0 runner    (1001) docker     (123)    38247 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/api/v2010/account/usage/record/daily.py
--rw-r--r--   0 runner    (1001) docker     (123)    38431 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/api/v2010/account/usage/record/last_month.py
--rw-r--r--   0 runner    (1001) docker     (123)    38339 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/api/v2010/account/usage/record/monthly.py
--rw-r--r--   0 runner    (1001) docker     (123)    38431 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/api/v2010/account/usage/record/this_month.py
--rw-r--r--   0 runner    (1001) docker     (123)    38247 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/api/v2010/account/usage/record/today.py
--rw-r--r--   0 runner    (1001) docker     (123)    38293 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/api/v2010/account/usage/record/yearly.py
--rw-r--r--   0 runner    (1001) docker     (123)    38431 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/api/v2010/account/usage/record/yesterday.py
--rw-r--r--   0 runner    (1001) docker     (123)    49245 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/api/v2010/account/usage/trigger.py
--rw-r--r--   0 runner    (1001) docker     (123)     7397 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/api/v2010/account/validation_request.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.180205 twilio-8.2.0/twilio/rest/autopilot/
--rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/autopilot/AutopilotBase.py
--rw-r--r--   0 runner    (1001) docker     (123)      778 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/autopilot/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.180205 twilio-8.2.0/twilio/rest/autopilot/v1/
--rw-r--r--   0 runner    (1001) docker     (123)     1680 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/autopilot/v1/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.180205 twilio-8.2.0/twilio/rest/autopilot/v1/assistant/
--rw-r--r--   0 runner    (1001) docker     (123)    35087 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/autopilot/v1/assistant/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8479 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/autopilot/v1/assistant/defaults.py
--rw-r--r--   0 runner    (1001) docker     (123)     6698 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/autopilot/v1/assistant/dialogue.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.180205 twilio-8.2.0/twilio/rest/autopilot/v1/assistant/field_type/
--rw-r--r--   0 runner    (1001) docker     (123)    23752 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/autopilot/v1/assistant/field_type/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22246 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/autopilot/v1/assistant/field_type/field_value.py
--rw-r--r--   0 runner    (1001) docker     (123)    22851 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/autopilot/v1/assistant/model_build.py
--rw-r--r--   0 runner    (1001) docker     (123)    29877 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/autopilot/v1/assistant/query.py
--rw-r--r--   0 runner    (1001) docker     (123)     8288 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/autopilot/v1/assistant/style_sheet.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.180205 twilio-8.2.0/twilio/rest/autopilot/v1/assistant/task/
--rw-r--r--   0 runner    (1001) docker     (123)    28213 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/autopilot/v1/assistant/task/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20115 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/autopilot/v1/assistant/task/field.py
--rw-r--r--   0 runner    (1001) docker     (123)    27891 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/autopilot/v1/assistant/task/sample.py
--rw-r--r--   0 runner    (1001) docker     (123)     9964 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/autopilot/v1/assistant/task/task_actions.py
--rw-r--r--   0 runner    (1001) docker     (123)     7530 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/autopilot/v1/assistant/task/task_statistics.py
--rw-r--r--   0 runner    (1001) docker     (123)    24728 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/autopilot/v1/assistant/webhook.py
--rw-r--r--   0 runner    (1001) docker     (123)     5222 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/autopilot/v1/restore_assistant.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.184205 twilio-8.2.0/twilio/rest/bulkexports/
--rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/bulkexports/BulkexportsBase.py
--rw-r--r--   0 runner    (1001) docker     (123)      792 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/bulkexports/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.184205 twilio-8.2.0/twilio/rest/bulkexports/v1/
--rw-r--r--   0 runner    (1001) docker     (123)     1692 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/bulkexports/v1/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.184205 twilio-8.2.0/twilio/rest/bulkexports/v1/export/
--rw-r--r--   0 runner    (1001) docker     (123)     7083 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/bulkexports/v1/export/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14521 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/bulkexports/v1/export/day.py
--rw-r--r--   0 runner    (1001) docker     (123)    17005 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/bulkexports/v1/export/export_custom_job.py
--rw-r--r--   0 runner    (1001) docker     (123)     8224 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/bulkexports/v1/export/job.py
--rw-r--r--   0 runner    (1001) docker     (123)    10811 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/bulkexports/v1/export_configuration.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.184205 twilio-8.2.0/twilio/rest/chat/
--rw-r--r--   0 runner    (1001) docker     (123)     1700 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/chat/ChatBase.py
--rw-r--r--   0 runner    (1001) docker     (123)      970 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/chat/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.184205 twilio-8.2.0/twilio/rest/chat/v1/
--rw-r--r--   0 runner    (1001) docker     (123)     1569 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/chat/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    27856 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/chat/v1/credential.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.184205 twilio-8.2.0/twilio/rest/chat/v1/service/
--rw-r--r--   0 runner    (1001) docker     (123)    92674 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/chat/v1/service/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.184205 twilio-8.2.0/twilio/rest/chat/v1/service/channel/
--rw-r--r--   0 runner    (1001) docker     (123)    28967 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/chat/v1/service/channel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22312 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/chat/v1/service/channel/invite.py
--rw-r--r--   0 runner    (1001) docker     (123)    27709 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/chat/v1/service/channel/member.py
--rw-r--r--   0 runner    (1001) docker     (123)    26356 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/chat/v1/service/channel/message.py
--rw-r--r--   0 runner    (1001) docker     (123)    21831 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/chat/v1/service/role.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.188205 twilio-8.2.0/twilio/rest/chat/v1/service/user/
--rw-r--r--   0 runner    (1001) docker     (123)    26317 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/chat/v1/service/user/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12925 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/chat/v1/service/user/user_channel.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.188205 twilio-8.2.0/twilio/rest/chat/v2/
--rw-r--r--   0 runner    (1001) docker     (123)     1569 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/chat/v2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    27486 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/chat/v2/credential.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.188205 twilio-8.2.0/twilio/rest/chat/v2/service/
--rw-r--r--   0 runner    (1001) docker     (123)    66570 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/chat/v2/service/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22118 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/chat/v2/service/binding.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.188205 twilio-8.2.0/twilio/rest/chat/v2/service/channel/
--rw-r--r--   0 runner    (1001) docker     (123)    39123 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/chat/v2/service/channel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22292 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/chat/v2/service/channel/invite.py
--rw-r--r--   0 runner    (1001) docker     (123)    41109 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/chat/v2/service/channel/member.py
--rw-r--r--   0 runner    (1001) docker     (123)    37545 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/chat/v2/service/channel/message.py
--rw-r--r--   0 runner    (1001) docker     (123)    33770 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/chat/v2/service/channel/webhook.py
--rw-r--r--   0 runner    (1001) docker     (123)    22232 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/chat/v2/service/role.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.188205 twilio-8.2.0/twilio/rest/chat/v2/service/user/
--rw-r--r--   0 runner    (1001) docker     (123)    29035 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/chat/v2/service/user/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21909 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/chat/v2/service/user/user_binding.py
--rw-r--r--   0 runner    (1001) docker     (123)    27050 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/chat/v2/service/user/user_channel.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.188205 twilio-8.2.0/twilio/rest/chat/v3/
--rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/chat/v3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11567 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/chat/v3/channel.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.188205 twilio-8.2.0/twilio/rest/content/
--rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/content/ContentBase.py
--rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/content/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.192205 twilio-8.2.0/twilio/rest/content/v1/
--rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/content/v1/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.192205 twilio-8.2.0/twilio/rest/content/v1/content/
--rw-r--r--   0 runner    (1001) docker     (123)    16628 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/content/v1/content/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5839 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/content/v1/content/approval_fetch.py
--rw-r--r--   0 runner    (1001) docker     (123)    11924 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/content/v1/content_and_approvals.py
--rw-r--r--   0 runner    (1001) docker     (123)    12123 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/content/v1/legacy_content.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.192205 twilio-8.2.0/twilio/rest/conversations/
--rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/conversations/ConversationsBase.py
--rw-r--r--   0 runner    (1001) docker     (123)     2760 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/conversations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.192205 twilio-8.2.0/twilio/rest/conversations/v1/
--rw-r--r--   0 runner    (1001) docker     (123)     3659 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/conversations/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    36854 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/conversations/v1/address_configuration.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.192205 twilio-8.2.0/twilio/rest/conversations/v1/configuration/
--rw-r--r--   0 runner    (1001) docker     (123)    12497 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/conversations/v1/configuration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11083 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/conversations/v1/configuration/webhook.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.192205 twilio-8.2.0/twilio/rest/conversations/v1/conversation/
--rw-r--r--   0 runner    (1001) docker     (123)    37723 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/conversations/v1/conversation/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.196205 twilio-8.2.0/twilio/rest/conversations/v1/conversation/message/
--rw-r--r--   0 runner    (1001) docker     (123)    34972 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/conversations/v1/conversation/message/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18063 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/conversations/v1/conversation/message/delivery_receipt.py
--rw-r--r--   0 runner    (1001) docker     (123)    40116 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/conversations/v1/conversation/participant.py
--rw-r--r--   0 runner    (1001) docker     (123)    27236 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/conversations/v1/conversation/webhook.py
--rw-r--r--   0 runner    (1001) docker     (123)    27935 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/conversations/v1/credential.py
--rw-r--r--   0 runner    (1001) docker     (123)    18739 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/conversations/v1/participant_conversation.py
--rw-r--r--   0 runner    (1001) docker     (123)    20943 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/conversations/v1/role.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.196205 twilio-8.2.0/twilio/rest/conversations/v1/service/
--rw-r--r--   0 runner    (1001) docker     (123)    20025 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/conversations/v1/service/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22289 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/conversations/v1/service/binding.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.196205 twilio-8.2.0/twilio/rest/conversations/v1/service/configuration/
--rw-r--r--   0 runner    (1001) docker     (123)    16088 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/conversations/v1/service/configuration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24410 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/conversations/v1/service/configuration/notification.py
--rw-r--r--   0 runner    (1001) docker     (123)    13881 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/conversations/v1/service/configuration/webhook.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.196205 twilio-8.2.0/twilio/rest/conversations/v1/service/conversation/
--rw-r--r--   0 runner    (1001) docker     (123)    39574 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/conversations/v1/service/conversation/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.200205 twilio-8.2.0/twilio/rest/conversations/v1/service/conversation/message/
--rw-r--r--   0 runner    (1001) docker     (123)    36629 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/conversations/v1/service/conversation/message/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19398 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/conversations/v1/service/conversation/message/delivery_receipt.py
--rw-r--r--   0 runner    (1001) docker     (123)    41799 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/conversations/v1/service/conversation/participant.py
--rw-r--r--   0 runner    (1001) docker     (123)    28926 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/conversations/v1/service/conversation/webhook.py
--rw-r--r--   0 runner    (1001) docker     (123)    19530 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/conversations/v1/service/participant_conversation.py
--rw-r--r--   0 runner    (1001) docker     (123)    22534 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/conversations/v1/service/role.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.200205 twilio-8.2.0/twilio/rest/conversations/v1/service/user/
--rw-r--r--   0 runner    (1001) docker     (123)    29682 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/conversations/v1/service/user/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    26510 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/conversations/v1/service/user/user_conversation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.200205 twilio-8.2.0/twilio/rest/conversations/v1/user/
--rw-r--r--   0 runner    (1001) docker     (123)    28016 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/conversations/v1/user/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25215 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/conversations/v1/user/user_conversation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.200205 twilio-8.2.0/twilio/rest/events/
--rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/events/EventsBase.py
--rw-r--r--   0 runner    (1001) docker     (123)     1277 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/events/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.200205 twilio-8.2.0/twilio/rest/events/v1/
--rw-r--r--   0 runner    (1001) docker     (123)     2133 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/events/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15317 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/events/v1/event_type.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.200205 twilio-8.2.0/twilio/rest/events/v1/schema/
--rw-r--r--   0 runner    (1001) docker     (123)     6417 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/events/v1/schema/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14920 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/events/v1/schema/schema_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.204205 twilio-8.2.0/twilio/rest/events/v1/sink/
--rw-r--r--   0 runner    (1001) docker     (123)    22872 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/events/v1/sink/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2768 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/events/v1/sink/sink_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3358 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/events/v1/sink/sink_validate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.204205 twilio-8.2.0/twilio/rest/events/v1/subscription/
--rw-r--r--   0 runner    (1001) docker     (123)    22609 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/events/v1/subscription/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20282 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/events/v1/subscription/subscribed_event.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.204205 twilio-8.2.0/twilio/rest/flex_api/
--rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/flex_api/FlexApiBase.py
--rw-r--r--   0 runner    (1001) docker     (123)     6332 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/flex_api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.208206 twilio-8.2.0/twilio/rest/flex_api/v1/
--rw-r--r--   0 runner    (1001) docker     (123)     7374 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/flex_api/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23435 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/flex_api/v1/assessments.py
--rw-r--r--   0 runner    (1001) docker     (123)    19793 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/flex_api/v1/channel.py
--rw-r--r--   0 runner    (1001) docker     (123)    13488 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/flex_api/v1/configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)    46860 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/flex_api/v1/flex_flow.py
--rw-r--r--   0 runner    (1001) docker     (123)    17501 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/flex_api/v1/insights_assessments_comment.py
--rw-r--r--   0 runner    (1001) docker     (123)    12580 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/flex_api/v1/insights_conversations.py
--rw-r--r--   0 runner    (1001) docker     (123)    27126 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/flex_api/v1/insights_questionnaires.py
--rw-r--r--   0 runner    (1001) docker     (123)    20401 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/flex_api/v1/insights_questionnaires_category.py
--rw-r--r--   0 runner    (1001) docker     (123)    26054 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/flex_api/v1/insights_questionnaires_question.py
--rw-r--r--   0 runner    (1001) docker     (123)    15704 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/flex_api/v1/insights_segments.py
--rw-r--r--   0 runner    (1001) docker     (123)     5688 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/flex_api/v1/insights_session.py
--rw-r--r--   0 runner    (1001) docker     (123)     3164 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/flex_api/v1/insights_settings_answer_sets.py
--rw-r--r--   0 runner    (1001) docker     (123)     2745 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/flex_api/v1/insights_settings_comment.py
--rw-r--r--   0 runner    (1001) docker     (123)     5365 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/flex_api/v1/insights_user_roles.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.208206 twilio-8.2.0/twilio/rest/flex_api/v1/interaction/
--rw-r--r--   0 runner    (1001) docker     (123)     8562 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/flex_api/v1/interaction/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.212206 twilio-8.2.0/twilio/rest/flex_api/v1/interaction/interaction_channel/
--rw-r--r--   0 runner    (1001) docker     (123)    20915 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/flex_api/v1/interaction/interaction_channel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13861 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/flex_api/v1/interaction/interaction_channel/interaction_channel_invite.py
--rw-r--r--   0 runner    (1001) docker     (123)    19858 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/flex_api/v1/interaction/interaction_channel/interaction_channel_participant.py
--rw-r--r--   0 runner    (1001) docker     (123)    20821 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/flex_api/v1/web_channel.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.212206 twilio-8.2.0/twilio/rest/flex_api/v2/
--rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/flex_api/v2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5583 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/flex_api/v2/web_channels.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.212206 twilio-8.2.0/twilio/rest/frontline_api/
--rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/frontline_api/FrontlineApiBase.py
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/frontline_api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.212206 twilio-8.2.0/twilio/rest/frontline_api/v1/
--rw-r--r--   0 runner    (1001) docker     (123)     1277 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/frontline_api/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10822 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/frontline_api/v1/user.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.212206 twilio-8.2.0/twilio/rest/insights/
--rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/insights/InsightsBase.py
--rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/insights/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.212206 twilio-8.2.0/twilio/rest/insights/v1/
--rw-r--r--   0 runner    (1001) docker     (123)     2419 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/insights/v1/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.216206 twilio-8.2.0/twilio/rest/insights/v1/call/
--rw-r--r--   0 runner    (1001) docker     (123)     6981 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/insights/v1/call/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17445 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/insights/v1/call/annotation.py
--rw-r--r--   0 runner    (1001) docker     (123)     9363 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/insights/v1/call/call_summary.py
--rw-r--r--   0 runner    (1001) docker     (123)    12166 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/insights/v1/call/event.py
--rw-r--r--   0 runner    (1001) docker     (123)    13146 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/insights/v1/call/metric.py
--rw-r--r--   0 runner    (1001) docker     (123)    28813 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/insights/v1/call_summaries.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.216206 twilio-8.2.0/twilio/rest/insights/v1/conference/
--rw-r--r--   0 runner    (1001) docker     (123)    31370 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/insights/v1/conference/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25248 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/insights/v1/conference/conference_participant.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.216206 twilio-8.2.0/twilio/rest/insights/v1/room/
--rw-r--r--   0 runner    (1001) docker     (123)    25243 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/insights/v1/room/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17908 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/insights/v1/room/participant.py
--rw-r--r--   0 runner    (1001) docker     (123)     8063 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/insights/v1/setting.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.216206 twilio-8.2.0/twilio/rest/ip_messaging/
--rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/ip_messaging/IpMessagingBase.py
--rw-r--r--   0 runner    (1001) docker     (123)      738 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/ip_messaging/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.216206 twilio-8.2.0/twilio/rest/ip_messaging/v1/
--rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/ip_messaging/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21632 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/ip_messaging/v1/credential.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.220206 twilio-8.2.0/twilio/rest/ip_messaging/v1/service/
--rw-r--r--   0 runner    (1001) docker     (123)    62960 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/ip_messaging/v1/service/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.220206 twilio-8.2.0/twilio/rest/ip_messaging/v1/service/channel/
--rw-r--r--   0 runner    (1001) docker     (123)    24064 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/ip_messaging/v1/service/channel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18541 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/ip_messaging/v1/service/channel/invite.py
--rw-r--r--   0 runner    (1001) docker     (123)    21725 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/ip_messaging/v1/service/channel/member.py
--rw-r--r--   0 runner    (1001) docker     (123)    21818 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/ip_messaging/v1/service/channel/message.py
--rw-r--r--   0 runner    (1001) docker     (123)    18855 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/ip_messaging/v1/service/role.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.220206 twilio-8.2.0/twilio/rest/ip_messaging/v1/service/user/
--rw-r--r--   0 runner    (1001) docker     (123)    21365 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/ip_messaging/v1/service/user/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11548 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/ip_messaging/v1/service/user/user_channel.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.220206 twilio-8.2.0/twilio/rest/ip_messaging/v2/
--rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/ip_messaging/v2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21632 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/ip_messaging/v2/credential.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.220206 twilio-8.2.0/twilio/rest/ip_messaging/v2/service/
--rw-r--r--   0 runner    (1001) docker     (123)    45390 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/ip_messaging/v2/service/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17907 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/ip_messaging/v2/service/binding.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.224206 twilio-8.2.0/twilio/rest/ip_messaging/v2/service/channel/
--rw-r--r--   0 runner    (1001) docker     (123)    30568 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/ip_messaging/v2/service/channel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18541 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/ip_messaging/v2/service/channel/invite.py
--rw-r--r--   0 runner    (1001) docker     (123)    29520 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/ip_messaging/v2/service/channel/member.py
--rw-r--r--   0 runner    (1001) docker     (123)    28798 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/ip_messaging/v2/service/channel/message.py
--rw-r--r--   0 runner    (1001) docker     (123)    26175 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/ip_messaging/v2/service/channel/webhook.py
--rw-r--r--   0 runner    (1001) docker     (123)    18855 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/ip_messaging/v2/service/role.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.224206 twilio-8.2.0/twilio/rest/ip_messaging/v2/service/user/
--rw-r--r--   0 runner    (1001) docker     (123)    24051 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/ip_messaging/v2/service/user/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18192 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/ip_messaging/v2/service/user/user_binding.py
--rw-r--r--   0 runner    (1001) docker     (123)    21476 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/ip_messaging/v2/service/user/user_channel.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.224206 twilio-8.2.0/twilio/rest/lookups/
--rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/lookups/LookupsBase.py
--rw-r--r--   0 runner    (1001) docker     (123)      432 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/lookups/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.224206 twilio-8.2.0/twilio/rest/lookups/v1/
--rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/lookups/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13250 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/lookups/v1/phone_number.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.224206 twilio-8.2.0/twilio/rest/lookups/v2/
--rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/lookups/v2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20961 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/lookups/v2/phone_number.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.228206 twilio-8.2.0/twilio/rest/media/
--rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/media/MediaBase.py
--rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/media/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.228206 twilio-8.2.0/twilio/rest/media/v1/
--rw-r--r--   0 runner    (1001) docker     (123)     2030 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/media/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    26533 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/media/v1/media_processor.py
--rw-r--r--   0 runner    (1001) docker     (123)    22582 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/media/v1/media_recording.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.228206 twilio-8.2.0/twilio/rest/media/v1/player_streamer/
--rw-r--r--   0 runner    (1001) docker     (123)    25414 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/media/v1/player_streamer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9432 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/media/v1/player_streamer/playback_grant.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.228206 twilio-8.2.0/twilio/rest/messaging/
--rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/messaging/MessagingBase.py
--rw-r--r--   0 runner    (1001) docker     (123)     3308 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/messaging/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.232206 twilio-8.2.0/twilio/rest/messaging/v1/
--rw-r--r--   0 runner    (1001) docker     (123)     4427 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/messaging/v1/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.232206 twilio-8.2.0/twilio/rest/messaging/v1/brand_registration/
--rw-r--r--   0 runner    (1001) docker     (123)    24289 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/messaging/v1/brand_registration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3583 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/messaging/v1/brand_registration/brand_registration_otp.py
--rw-r--r--   0 runner    (1001) docker     (123)    19914 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/messaging/v1/brand_registration/brand_vetting.py
--rw-r--r--   0 runner    (1001) docker     (123)     5796 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/messaging/v1/deactivations.py
--rw-r--r--   0 runner    (1001) docker     (123)    10495 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/messaging/v1/domain_certs.py
--rw-r--r--   0 runner    (1001) docker     (123)    10525 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/messaging/v1/domain_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     7773 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/messaging/v1/domain_config_messaging_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     4360 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/messaging/v1/external_campaign.py
--rw-r--r--   0 runner    (1001) docker     (123)     9216 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/messaging/v1/linkshortening_messaging_service.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.232206 twilio-8.2.0/twilio/rest/messaging/v1/service/
--rw-r--r--   0 runner    (1001) docker     (123)    54653 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/messaging/v1/service/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18348 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/messaging/v1/service/alpha_sender.py
--rw-r--r--   0 runner    (1001) docker     (123)    18413 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/messaging/v1/service/phone_number.py
--rw-r--r--   0 runner    (1001) docker     (123)    18135 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/messaging/v1/service/short_code.py
--rw-r--r--   0 runner    (1001) docker     (123)    33395 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/messaging/v1/service/us_app_to_person.py
--rw-r--r--   0 runner    (1001) docker     (123)     3513 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/messaging/v1/service/us_app_to_person_usecase.py
--rw-r--r--   0 runner    (1001) docker     (123)     2322 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/messaging/v1/usecase.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.236206 twilio-8.2.0/twilio/rest/microvisor/
--rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/microvisor/MicrovisorBase.py
--rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/microvisor/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.236206 twilio-8.2.0/twilio/rest/microvisor/v1/
--rw-r--r--   0 runner    (1001) docker     (123)     2211 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/microvisor/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17838 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/microvisor/v1/account_config.py
--rw-r--r--   0 runner    (1001) docker     (123)    17723 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/microvisor/v1/account_secret.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.236206 twilio-8.2.0/twilio/rest/microvisor/v1/app/
--rw-r--r--   0 runner    (1001) docker     (123)    15664 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/microvisor/v1/app/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5534 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/microvisor/v1/app/app_manifest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.236206 twilio-8.2.0/twilio/rest/microvisor/v1/device/
--rw-r--r--   0 runner    (1001) docker     (123)    20135 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/microvisor/v1/device/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19145 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/microvisor/v1/device/device_config.py
--rw-r--r--   0 runner    (1001) docker     (123)    19030 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/microvisor/v1/device/device_secret.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.236206 twilio-8.2.0/twilio/rest/monitor/
--rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/monitor/MonitorBase.py
--rw-r--r--   0 runner    (1001) docker     (123)      658 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/monitor/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.236206 twilio-8.2.0/twilio/rest/monitor/v1/
--rw-r--r--   0 runner    (1001) docker     (123)     1517 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/monitor/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22723 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/monitor/v1/alert.py
--rw-r--r--   0 runner    (1001) docker     (123)    25437 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/monitor/v1/event.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.240206 twilio-8.2.0/twilio/rest/notify/
--rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/notify/NotifyBase.py
--rw-r--r--   0 runner    (1001) docker     (123)      700 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/notify/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.240206 twilio-8.2.0/twilio/rest/notify/v1/
--rw-r--r--   0 runner    (1001) docker     (123)     1581 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/notify/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    27961 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/notify/v1/credential.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.240206 twilio-8.2.0/twilio/rest/notify/v1/service/
--rw-r--r--   0 runner    (1001) docker     (123)    47060 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/notify/v1/service/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    30272 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/notify/v1/service/binding.py
--rw-r--r--   0 runner    (1001) docker     (123)    25490 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/notify/v1/service/notification.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.240206 twilio-8.2.0/twilio/rest/numbers/
--rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/numbers/NumbersBase.py
--rw-r--r--   0 runner    (1001) docker     (123)      491 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/numbers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.240206 twilio-8.2.0/twilio/rest/numbers/v2/
--rw-r--r--   0 runner    (1001) docker     (123)     1414 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/numbers/v2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.244206 twilio-8.2.0/twilio/rest/numbers/v2/regulatory_compliance/
--rw-r--r--   0 runner    (1001) docker     (123)     3690 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/numbers/v2/regulatory_compliance/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.244206 twilio-8.2.0/twilio/rest/numbers/v2/regulatory_compliance/bundle/
--rw-r--r--   0 runner    (1001) docker     (123)    47502 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/numbers/v2/regulatory_compliance/bundle/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13880 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/numbers/v2/regulatory_compliance/bundle/bundle_copy.py
--rw-r--r--   0 runner    (1001) docker     (123)    16186 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/numbers/v2/regulatory_compliance/bundle/evaluation.py
--rw-r--r--   0 runner    (1001) docker     (123)    17833 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/numbers/v2/regulatory_compliance/bundle/item_assignment.py
--rw-r--r--   0 runner    (1001) docker     (123)     5665 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/numbers/v2/regulatory_compliance/bundle/replace_items.py
--rw-r--r--   0 runner    (1001) docker     (123)    20500 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/numbers/v2/regulatory_compliance/end_user.py
--rw-r--r--   0 runner    (1001) docker     (123)    14140 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/numbers/v2/regulatory_compliance/end_user_type.py
--rw-r--r--   0 runner    (1001) docker     (123)    18536 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/numbers/v2/regulatory_compliance/regulation.py
--rw-r--r--   0 runner    (1001) docker     (123)    22407 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/numbers/v2/regulatory_compliance/supporting_document.py
--rw-r--r--   0 runner    (1001) docker     (123)    14788 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/numbers/v2/regulatory_compliance/supporting_document_type.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.244206 twilio-8.2.0/twilio/rest/oauth/
--rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/oauth/OauthBase.py
--rw-r--r--   0 runner    (1001) docker     (123)     1578 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/oauth/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.248206 twilio-8.2.0/twilio/rest/oauth/v1/
--rw-r--r--   0 runner    (1001) docker     (123)     2434 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/oauth/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4598 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/oauth/v1/device_code.py
--rw-r--r--   0 runner    (1001) docker     (123)     4115 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/oauth/v1/oauth.py
--rw-r--r--   0 runner    (1001) docker     (123)     7059 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/oauth/v1/openid_discovery.py
--rw-r--r--   0 runner    (1001) docker     (123)     6329 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/oauth/v1/token.py
--rw-r--r--   0 runner    (1001) docker     (123)     4714 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/oauth/v1/user_info.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.248206 twilio-8.2.0/twilio/rest/preview/
--rw-r--r--   0 runner    (1001) docker     (123)     3081 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/preview/PreviewBase.py
--rw-r--r--   0 runner    (1001) docker     (123)     3528 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/preview/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.248206 twilio-8.2.0/twilio/rest/preview/deployed_devices/
--rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/preview/deployed_devices/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.252206 twilio-8.2.0/twilio/rest/preview/deployed_devices/fleet/
--rw-r--r--   0 runner    (1001) docker     (123)    22442 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/preview/deployed_devices/fleet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24118 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/preview/deployed_devices/fleet/certificate.py
--rw-r--r--   0 runner    (1001) docker     (123)    22163 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/preview/deployed_devices/fleet/deployment.py
--rw-r--r--   0 runner    (1001) docker     (123)    26656 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/preview/deployed_devices/fleet/device.py
--rw-r--r--   0 runner    (1001) docker     (123)    22726 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/preview/deployed_devices/fleet/key.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.252206 twilio-8.2.0/twilio/rest/preview/hosted_numbers/
--rw-r--r--   0 runner    (1001) docker     (123)     1892 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/preview/hosted_numbers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.252206 twilio-8.2.0/twilio/rest/preview/hosted_numbers/authorization_document/
--rw-r--r--   0 runner    (1001) docker     (123)    32009 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/preview/hosted_numbers/authorization_document/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24829 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/preview/hosted_numbers/authorization_document/dependent_hosted_number_order.py
--rw-r--r--   0 runner    (1001) docker     (123)    48143 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/preview/hosted_numbers/hosted_number_order.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.252206 twilio-8.2.0/twilio/rest/preview/marketplace/
--rw-r--r--   0 runner    (1001) docker     (123)     1775 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/preview/marketplace/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.252206 twilio-8.2.0/twilio/rest/preview/marketplace/available_add_on/
--rw-r--r--   0 runner    (1001) docker     (123)    15067 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/preview/marketplace/available_add_on/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16163 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/preview/marketplace/available_add_on/available_add_on_extension.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.252206 twilio-8.2.0/twilio/rest/preview/marketplace/installed_add_on/
--rw-r--r--   0 runner    (1001) docker     (123)    23293 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/preview/marketplace/installed_add_on/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18542 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/preview/marketplace/installed_add_on/installed_add_on_extension.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.252206 twilio-8.2.0/twilio/rest/preview/sync/
--rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/preview/sync/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.256206 twilio-8.2.0/twilio/rest/preview/sync/service/
--rw-r--r--   0 runner    (1001) docker     (123)    22270 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/preview/sync/service/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.256206 twilio-8.2.0/twilio/rest/preview/sync/service/document/
--rw-r--r--   0 runner    (1001) docker     (123)    20547 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/preview/sync/service/document/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21455 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/preview/sync/service/document/document_permission.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.256206 twilio-8.2.0/twilio/rest/preview/sync/service/sync_list/
--rw-r--r--   0 runner    (1001) docker     (123)    18339 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/preview/sync/service/sync_list/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24174 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/preview/sync/service/sync_list/sync_list_item.py
--rw-r--r--   0 runner    (1001) docker     (123)    21397 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/preview/sync/service/sync_list/sync_list_permission.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.256206 twilio-8.2.0/twilio/rest/preview/sync/service/sync_map/
--rw-r--r--   0 runner    (1001) docker     (123)    18217 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/preview/sync/service/sync_map/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24063 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/preview/sync/service/sync_map/sync_map_item.py
--rw-r--r--   0 runner    (1001) docker     (123)    21250 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/preview/sync/service/sync_map/sync_map_permission.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.256206 twilio-8.2.0/twilio/rest/preview/understand/
--rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/preview/understand/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.260206 twilio-8.2.0/twilio/rest/preview/understand/assistant/
--rw-r--r--   0 runner    (1001) docker     (123)    35382 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/preview/understand/assistant/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8318 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/preview/understand/assistant/assistant_fallback_actions.py
--rw-r--r--   0 runner    (1001) docker     (123)     8510 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/preview/understand/assistant/assistant_initiation_actions.py
--rw-r--r--   0 runner    (1001) docker     (123)     5976 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/preview/understand/assistant/dialogue.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.260206 twilio-8.2.0/twilio/rest/preview/understand/assistant/field_type/
--rw-r--r--   0 runner    (1001) docker     (123)    22348 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/preview/understand/assistant/field_type/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20410 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/preview/understand/assistant/field_type/field_value.py
--rw-r--r--   0 runner    (1001) docker     (123)    21062 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/preview/understand/assistant/model_build.py
--rw-r--r--   0 runner    (1001) docker     (123)    26433 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/preview/understand/assistant/query.py
--rw-r--r--   0 runner    (1001) docker     (123)     7799 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/preview/understand/assistant/style_sheet.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.260206 twilio-8.2.0/twilio/rest/preview/understand/assistant/task/
--rw-r--r--   0 runner    (1001) docker     (123)    26813 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/preview/understand/assistant/task/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19110 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/preview/understand/assistant/task/field.py
--rw-r--r--   0 runner    (1001) docker     (123)    24937 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/preview/understand/assistant/task/sample.py
--rw-r--r--   0 runner    (1001) docker     (123)     8816 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/preview/understand/assistant/task/task_actions.py
--rw-r--r--   0 runner    (1001) docker     (123)     6871 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/preview/understand/assistant/task/task_statistics.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.264206 twilio-8.2.0/twilio/rest/preview/wireless/
--rw-r--r--   0 runner    (1001) docker     (123)     1849 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/preview/wireless/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18911 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/preview/wireless/command.py
--rw-r--r--   0 runner    (1001) docker     (123)    21681 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/preview/wireless/rate_plan.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.264206 twilio-8.2.0/twilio/rest/preview/wireless/sim/
--rw-r--r--   0 runner    (1001) docker     (123)    28867 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/preview/wireless/sim/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6592 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/preview/wireless/sim/usage.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.264206 twilio-8.2.0/twilio/rest/pricing/
--rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/pricing/PricingBase.py
--rw-r--r--   0 runner    (1001) docker     (123)     1569 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/pricing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.264206 twilio-8.2.0/twilio/rest/pricing/v1/
--rw-r--r--   0 runner    (1001) docker     (123)     1867 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/pricing/v1/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.264206 twilio-8.2.0/twilio/rest/pricing/v1/messaging/
--rw-r--r--   0 runner    (1001) docker     (123)     1443 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/pricing/v1/messaging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14530 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/pricing/v1/messaging/country.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.264206 twilio-8.2.0/twilio/rest/pricing/v1/phone_number/
--rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/pricing/v1/phone_number/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14123 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/pricing/v1/phone_number/country.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.264206 twilio-8.2.0/twilio/rest/pricing/v1/voice/
--rw-r--r--   0 runner    (1001) docker     (123)     1753 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/pricing/v1/voice/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14416 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/pricing/v1/voice/country.py
--rw-r--r--   0 runner    (1001) docker     (123)     5701 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/pricing/v1/voice/number.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.268206 twilio-8.2.0/twilio/rest/pricing/v2/
--rw-r--r--   0 runner    (1001) docker     (123)     1801 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/pricing/v2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14470 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/pricing/v2/country.py
--rw-r--r--   0 runner    (1001) docker     (123)     8966 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/pricing/v2/number.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.268206 twilio-8.2.0/twilio/rest/pricing/v2/voice/
--rw-r--r--   0 runner    (1001) docker     (123)     1753 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/pricing/v2/voice/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14446 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/pricing/v2/voice/country.py
--rw-r--r--   0 runner    (1001) docker     (123)     9040 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/pricing/v2/voice/number.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.268206 twilio-8.2.0/twilio/rest/proxy/
--rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/proxy/ProxyBase.py
--rw-r--r--   0 runner    (1001) docker     (123)      387 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/proxy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.268206 twilio-8.2.0/twilio/rest/proxy/v1/
--rw-r--r--   0 runner    (1001) docker     (123)     1273 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/proxy/v1/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.268206 twilio-8.2.0/twilio/rest/proxy/v1/service/
--rw-r--r--   0 runner    (1001) docker     (123)    38044 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/proxy/v1/service/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23754 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/proxy/v1/service/phone_number.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.268206 twilio-8.2.0/twilio/rest/proxy/v1/service/session/
--rw-r--r--   0 runner    (1001) docker     (123)    27767 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/proxy/v1/service/session/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21109 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/proxy/v1/service/session/interaction.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.272206 twilio-8.2.0/twilio/rest/proxy/v1/service/session/participant/
--rw-r--r--   0 runner    (1001) docker     (123)    22765 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/proxy/v1/service/session/participant/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23242 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/proxy/v1/service/session/participant/message_interaction.py
--rw-r--r--   0 runner    (1001) docker     (123)    21333 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/proxy/v1/service/short_code.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.272206 twilio-8.2.0/twilio/rest/routes/
--rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/routes/RoutesBase.py
--rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/routes/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.272206 twilio-8.2.0/twilio/rest/routes/v2/
--rw-r--r--   0 runner    (1001) docker     (123)     1876 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/routes/v2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9727 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/routes/v2/phone_number.py
--rw-r--r--   0 runner    (1001) docker     (123)     8319 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/routes/v2/sip_domain.py
--rw-r--r--   0 runner    (1001) docker     (123)     9536 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/routes/v2/trunk.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.272206 twilio-8.2.0/twilio/rest/serverless/
--rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/serverless/ServerlessBase.py
--rw-r--r--   0 runner    (1001) docker     (123)      417 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/serverless/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.272206 twilio-8.2.0/twilio/rest/serverless/v1/
--rw-r--r--   0 runner    (1001) docker     (123)     1298 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/serverless/v1/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.272206 twilio-8.2.0/twilio/rest/serverless/v1/service/
--rw-r--r--   0 runner    (1001) docker     (123)    25510 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/serverless/v1/service/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.276206 twilio-8.2.0/twilio/rest/serverless/v1/service/asset/
--rw-r--r--   0 runner    (1001) docker     (123)    20582 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/serverless/v1/service/asset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16714 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/serverless/v1/service/asset/asset_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.276206 twilio-8.2.0/twilio/rest/serverless/v1/service/build/
--rw-r--r--   0 runner    (1001) docker     (123)    20195 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/serverless/v1/service/build/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6403 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/serverless/v1/service/build/build_status.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.276206 twilio-8.2.0/twilio/rest/serverless/v1/service/environment/
--rw-r--r--   0 runner    (1001) docker     (123)    21009 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/serverless/v1/service/environment/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18049 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/serverless/v1/service/environment/deployment.py
--rw-r--r--   0 runner    (1001) docker     (123)    20926 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/serverless/v1/service/environment/log.py
--rw-r--r--   0 runner    (1001) docker     (123)    22598 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/serverless/v1/service/environment/variable.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.276206 twilio-8.2.0/twilio/rest/serverless/v1/service/function/
--rw-r--r--   0 runner    (1001) docker     (123)    20928 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/serverless/v1/service/function/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.276206 twilio-8.2.0/twilio/rest/serverless/v1/service/function/function_version/
--rw-r--r--   0 runner    (1001) docker     (123)    18093 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/serverless/v1/service/function/function_version/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7736 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/serverless/v1/service/function/function_version/function_version_content.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.280206 twilio-8.2.0/twilio/rest/studio/
--rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/studio/StudioBase.py
--rw-r--r--   0 runner    (1001) docker     (123)      694 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/studio/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.280206 twilio-8.2.0/twilio/rest/studio/v1/
--rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/studio/v1/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.280206 twilio-8.2.0/twilio/rest/studio/v1/flow/
--rw-r--r--   0 runner    (1001) docker     (123)    16404 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/studio/v1/flow/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.280206 twilio-8.2.0/twilio/rest/studio/v1/flow/engagement/
--rw-r--r--   0 runner    (1001) docker     (123)    21366 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/studio/v1/flow/engagement/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6720 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/studio/v1/flow/engagement/engagement_context.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.280206 twilio-8.2.0/twilio/rest/studio/v1/flow/engagement/step/
--rw-r--r--   0 runner    (1001) docker     (123)    17219 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/studio/v1/flow/engagement/step/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7395 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/studio/v1/flow/engagement/step/step_context.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.280206 twilio-8.2.0/twilio/rest/studio/v1/flow/execution/
--rw-r--r--   0 runner    (1001) docker     (123)    27270 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/studio/v1/flow/execution/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6877 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/studio/v1/flow/execution/execution_context.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.280206 twilio-8.2.0/twilio/rest/studio/v1/flow/execution/execution_step/
--rw-r--r--   0 runner    (1001) docker     (123)    17888 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/studio/v1/flow/execution/execution_step/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7716 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/studio/v1/flow/execution/execution_step/execution_step_context.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.284206 twilio-8.2.0/twilio/rest/studio/v2/
--rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/studio/v2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.284206 twilio-8.2.0/twilio/rest/studio/v2/flow/
--rw-r--r--   0 runner    (1001) docker     (123)    23658 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/studio/v2/flow/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.284206 twilio-8.2.0/twilio/rest/studio/v2/flow/execution/
--rw-r--r--   0 runner    (1001) docker     (123)    27154 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/studio/v2/flow/execution/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6877 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/studio/v2/flow/execution/execution_context.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.284206 twilio-8.2.0/twilio/rest/studio/v2/flow/execution/execution_step/
--rw-r--r--   0 runner    (1001) docker     (123)    17888 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/studio/v2/flow/execution/execution_step/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7716 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/studio/v2/flow/execution/execution_step/execution_step_context.py
--rw-r--r--   0 runner    (1001) docker     (123)    16059 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/studio/v2/flow/flow_revision.py
--rw-r--r--   0 runner    (1001) docker     (123)     7422 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/studio/v2/flow/flow_test_user.py
--rw-r--r--   0 runner    (1001) docker     (123)     3892 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/studio/v2/flow_validate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.284206 twilio-8.2.0/twilio/rest/supersim/
--rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/supersim/SupersimBase.py
--rw-r--r--   0 runner    (1001) docker     (123)     2908 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/supersim/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.288206 twilio-8.2.0/twilio/rest/supersim/v1/
--rw-r--r--   0 runner    (1001) docker     (123)     3800 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/supersim/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23623 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/supersim/v1/esim_profile.py
--rw-r--r--   0 runner    (1001) docker     (123)    35226 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/supersim/v1/fleet.py
--rw-r--r--   0 runner    (1001) docker     (123)    26640 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/supersim/v1/ip_command.py
--rw-r--r--   0 runner    (1001) docker     (123)    17582 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/supersim/v1/network.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.288206 twilio-8.2.0/twilio/rest/supersim/v1/network_access_profile/
--rw-r--r--   0 runner    (1001) docker     (123)    20071 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/supersim/v1/network_access_profile/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19359 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/supersim/v1/network_access_profile/network_access_profile_network.py
--rw-r--r--   0 runner    (1001) docker     (123)    14206 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/supersim/v1/settings_update.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.288206 twilio-8.2.0/twilio/rest/supersim/v1/sim/
--rw-r--r--   0 runner    (1001) docker     (123)    28732 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/supersim/v1/sim/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12030 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/supersim/v1/sim/billing_period.py
--rw-r--r--   0 runner    (1001) docker     (123)    10625 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/supersim/v1/sim/sim_ip_address.py
--rw-r--r--   0 runner    (1001) docker     (123)    23001 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/supersim/v1/sms_command.py
--rw-r--r--   0 runner    (1001) docker     (123)    26841 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/supersim/v1/usage_record.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.292207 twilio-8.2.0/twilio/rest/sync/
--rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/sync/SyncBase.py
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/sync/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.292207 twilio-8.2.0/twilio/rest/sync/v1/
--rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/sync/v1/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.292207 twilio-8.2.0/twilio/rest/sync/v1/service/
--rw-r--r--   0 runner    (1001) docker     (123)    36623 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/sync/v1/service/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.292207 twilio-8.2.0/twilio/rest/sync/v1/service/document/
--rw-r--r--   0 runner    (1001) docker     (123)    25373 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/sync/v1/service/document/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21822 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/sync/v1/service/document/document_permission.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.292207 twilio-8.2.0/twilio/rest/sync/v1/service/sync_list/
--rw-r--r--   0 runner    (1001) docker     (123)    25198 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/sync/v1/service/sync_list/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    36671 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/sync/v1/service/sync_list/sync_list_item.py
--rw-r--r--   0 runner    (1001) docker     (123)    21826 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/sync/v1/service/sync_list/sync_list_permission.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.292207 twilio-8.2.0/twilio/rest/sync/v1/service/sync_map/
--rw-r--r--   0 runner    (1001) docker     (123)    24886 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/sync/v1/service/sync_map/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    37230 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/sync/v1/service/sync_map/sync_map_item.py
--rw-r--r--   0 runner    (1001) docker     (123)    21754 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/sync/v1/service/sync_map/sync_map_permission.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.296207 twilio-8.2.0/twilio/rest/sync/v1/service/sync_stream/
--rw-r--r--   0 runner    (1001) docker     (123)    22899 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/sync/v1/service/sync_stream/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4315 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/sync/v1/service/sync_stream/stream_message.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.296207 twilio-8.2.0/twilio/rest/taskrouter/
--rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/taskrouter/TaskrouterBase.py
--rw-r--r--   0 runner    (1001) docker     (123)      431 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/taskrouter/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.296207 twilio-8.2.0/twilio/rest/taskrouter/v1/
--rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/taskrouter/v1/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.296207 twilio-8.2.0/twilio/rest/taskrouter/v1/workspace/
--rw-r--r--   0 runner    (1001) docker     (123)    44452 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/taskrouter/v1/workspace/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25986 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/taskrouter/v1/workspace/activity.py
--rw-r--r--   0 runner    (1001) docker     (123)    32776 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/taskrouter/v1/workspace/event.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.300207 twilio-8.2.0/twilio/rest/taskrouter/v1/workspace/task/
--rw-r--r--   0 runner    (1001) docker     (123)    51478 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/taskrouter/v1/workspace/task/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    79751 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/taskrouter/v1/workspace/task/reservation.py
--rw-r--r--   0 runner    (1001) docker     (123)    23470 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/taskrouter/v1/workspace/task_channel.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.300207 twilio-8.2.0/twilio/rest/taskrouter/v1/workspace/task_queue/
--rw-r--r--   0 runner    (1001) docker     (123)    39230 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/taskrouter/v1/workspace/task_queue/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18318 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/taskrouter/v1/workspace/task_queue/task_queue_cumulative_statistics.py
--rw-r--r--   0 runner    (1001) docker     (123)    10983 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/taskrouter/v1/workspace/task_queue/task_queue_real_time_statistics.py
--rw-r--r--   0 runner    (1001) docker     (123)    13380 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/taskrouter/v1/workspace/task_queue/task_queue_statistics.py
--rw-r--r--   0 runner    (1001) docker     (123)    21315 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/taskrouter/v1/workspace/task_queue/task_queues_statistics.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.304207 twilio-8.2.0/twilio/rest/taskrouter/v1/workspace/worker/
--rw-r--r--   0 runner    (1001) docker     (123)    43462 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/taskrouter/v1/workspace/worker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    77533 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/taskrouter/v1/workspace/worker/reservation.py
--rw-r--r--   0 runner    (1001) docker     (123)    22091 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/taskrouter/v1/workspace/worker/worker_channel.py
--rw-r--r--   0 runner    (1001) docker     (123)    11730 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/taskrouter/v1/workspace/worker/worker_statistics.py
--rw-r--r--   0 runner    (1001) docker     (123)    13241 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/taskrouter/v1/workspace/worker/workers_cumulative_statistics.py
--rw-r--r--   0 runner    (1001) docker     (123)     7884 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/taskrouter/v1/workspace/worker/workers_real_time_statistics.py
--rw-r--r--   0 runner    (1001) docker     (123)    13545 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/taskrouter/v1/workspace/worker/workers_statistics.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.304207 twilio-8.2.0/twilio/rest/taskrouter/v1/workspace/workflow/
--rw-r--r--   0 runner    (1001) docker     (123)    34579 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/taskrouter/v1/workspace/workflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19228 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/taskrouter/v1/workspace/workflow/workflow_cumulative_statistics.py
--rw-r--r--   0 runner    (1001) docker     (123)     9689 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/taskrouter/v1/workspace/workflow/workflow_real_time_statistics.py
--rw-r--r--   0 runner    (1001) docker     (123)    14701 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/taskrouter/v1/workspace/workflow/workflow_statistics.py
--rw-r--r--   0 runner    (1001) docker     (123)    18165 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/taskrouter/v1/workspace/workspace_cumulative_statistics.py
--rw-r--r--   0 runner    (1001) docker     (123)     9027 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/taskrouter/v1/workspace/workspace_real_time_statistics.py
--rw-r--r--   0 runner    (1001) docker     (123)    13564 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/taskrouter/v1/workspace/workspace_statistics.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.304207 twilio-8.2.0/twilio/rest/trunking/
--rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/trunking/TrunkingBase.py
--rw-r--r--   0 runner    (1001) docker     (123)      391 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/trunking/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.304207 twilio-8.2.0/twilio/rest/trunking/v1/
--rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/trunking/v1/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.304207 twilio-8.2.0/twilio/rest/trunking/v1/trunk/
--rw-r--r--   0 runner    (1001) docker     (123)    39976 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/trunking/v1/trunk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18350 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/trunking/v1/trunk/credential_list.py
--rw-r--r--   0 runner    (1001) docker     (123)    18720 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/trunking/v1/trunk/ip_access_control_list.py
--rw-r--r--   0 runner    (1001) docker     (123)    27739 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/trunking/v1/trunk/origination_url.py
--rw-r--r--   0 runner    (1001) docker     (123)    22459 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/trunking/v1/trunk/phone_number.py
--rw-r--r--   0 runner    (1001) docker     (123)     8181 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/trunking/v1/trunk/recording.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.308207 twilio-8.2.0/twilio/rest/trusthub/
--rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/trusthub/TrusthubBase.py
--rw-r--r--   0 runner    (1001) docker     (123)     2483 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/trusthub/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.308207 twilio-8.2.0/twilio/rest/trusthub/v1/
--rw-r--r--   0 runner    (1001) docker     (123)     3431 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/trusthub/v1/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.308207 twilio-8.2.0/twilio/rest/trusthub/v1/customer_profiles/
--rw-r--r--   0 runner    (1001) docker     (123)    30761 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/trusthub/v1/customer_profiles/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23437 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/trusthub/v1/customer_profiles/customer_profiles_channel_endpoint_assignment.py
--rw-r--r--   0 runner    (1001) docker     (123)    19934 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/trusthub/v1/customer_profiles/customer_profiles_entity_assignments.py
--rw-r--r--   0 runner    (1001) docker     (123)    18436 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/trusthub/v1/customer_profiles/customer_profiles_evaluations.py
--rw-r--r--   0 runner    (1001) docker     (123)    20560 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/trusthub/v1/end_user.py
--rw-r--r--   0 runner    (1001) docker     (123)    14103 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/trusthub/v1/end_user_type.py
--rw-r--r--   0 runner    (1001) docker     (123)    13542 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/trusthub/v1/policies.py
--rw-r--r--   0 runner    (1001) docker     (123)    22191 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/trusthub/v1/supporting_document.py
--rw-r--r--   0 runner    (1001) docker     (123)    14729 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/trusthub/v1/supporting_document_type.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.312207 twilio-8.2.0/twilio/rest/trusthub/v1/trust_products/
--rw-r--r--   0 runner    (1001) docker     (123)    30206 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/trusthub/v1/trust_products/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23131 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/trusthub/v1/trust_products/trust_products_channel_endpoint_assignment.py
--rw-r--r--   0 runner    (1001) docker     (123)    19505 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/trusthub/v1/trust_products/trust_products_entity_assignments.py
--rw-r--r--   0 runner    (1001) docker     (123)    18057 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/trusthub/v1/trust_products/trust_products_evaluations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.312207 twilio-8.2.0/twilio/rest/verify/
--rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/verify/VerifyBase.py
--rw-r--r--   0 runner    (1001) docker     (123)     2056 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/verify/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.312207 twilio-8.2.0/twilio/rest/verify/v2/
--rw-r--r--   0 runner    (1001) docker     (123)     2992 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/verify/v2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5695 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/verify/v2/form.py
--rw-r--r--   0 runner    (1001) docker     (123)     8036 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/verify/v2/safelist.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.316207 twilio-8.2.0/twilio/rest/verify/v2/service/
--rw-r--r--   0 runner    (1001) docker     (123)    55315 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/verify/v2/service/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10267 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/verify/v2/service/access_token.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.316207 twilio-8.2.0/twilio/rest/verify/v2/service/entity/
--rw-r--r--   0 runner    (1001) docker     (123)    20668 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/verify/v2/service/entity/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.316207 twilio-8.2.0/twilio/rest/verify/v2/service/entity/challenge/
--rw-r--r--   0 runner    (1001) docker     (123)    34458 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/verify/v2/service/entity/challenge/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6557 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/verify/v2/service/entity/challenge/notification.py
--rw-r--r--   0 runner    (1001) docker     (123)    29593 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/verify/v2/service/entity/factor.py
--rw-r--r--   0 runner    (1001) docker     (123)    16164 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/verify/v2/service/entity/new_factor.py
--rw-r--r--   0 runner    (1001) docker     (123)    23201 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/verify/v2/service/messaging_configuration.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.320207 twilio-8.2.0/twilio/rest/verify/v2/service/rate_limit/
--rw-r--r--   0 runner    (1001) docker     (123)    21507 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/verify/v2/service/rate_limit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22242 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/verify/v2/service/rate_limit/bucket.py
--rw-r--r--   0 runner    (1001) docker     (123)    21417 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/verify/v2/service/verification.py
--rw-r--r--   0 runner    (1001) docker     (123)     8363 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/verify/v2/service/verification_check.py
--rw-r--r--   0 runner    (1001) docker     (123)    25389 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/verify/v2/service/webhook.py
--rw-r--r--   0 runner    (1001) docker     (123)    11731 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/verify/v2/template.py
--rw-r--r--   0 runner    (1001) docker     (123)    29432 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/verify/v2/verification_attempt.py
--rw-r--r--   0 runner    (1001) docker     (123)    13009 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/verify/v2/verification_attempts_summary.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.320207 twilio-8.2.0/twilio/rest/video/
--rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/video/VideoBase.py
--rw-r--r--   0 runner    (1001) docker     (123)     2050 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/video/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.320207 twilio-8.2.0/twilio/rest/video/v1/
--rw-r--r--   0 runner    (1001) docker     (123)     2971 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/video/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    34977 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/video/v1/composition.py
--rw-r--r--   0 runner    (1001) docker     (123)    54707 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/video/v1/composition_hook.py
--rw-r--r--   0 runner    (1001) docker     (123)    14079 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/video/v1/composition_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)    27313 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/video/v1/recording.py
--rw-r--r--   0 runner    (1001) docker     (123)    13910 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/video/v1/recording_settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.320207 twilio-8.2.0/twilio/rest/video/v1/room/
--rw-r--r--   0 runner    (1001) docker     (123)    38074 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/video/v1/room/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.324207 twilio-8.2.0/twilio/rest/video/v1/room/participant/
--rw-r--r--   0 runner    (1001) docker     (123)    28698 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/video/v1/room/participant/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7905 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/video/v1/room/participant/anonymize.py
--rw-r--r--   0 runner    (1001) docker     (123)    16887 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/video/v1/room/participant/published_track.py
--rw-r--r--   0 runner    (1001) docker     (123)     6391 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/video/v1/room/participant/subscribe_rules.py
--rw-r--r--   0 runner    (1001) docker     (123)    17079 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/video/v1/room/participant/subscribed_track.py
--rw-r--r--   0 runner    (1001) docker     (123)     5087 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/video/v1/room/recording_rules.py
--rw-r--r--   0 runner    (1001) docker     (123)    24746 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/video/v1/room/room_recording.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.324207 twilio-8.2.0/twilio/rest/voice/
--rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/voice/VoiceBase.py
--rw-r--r--   0 runner    (1001) docker     (123)     2099 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/voice/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.324207 twilio-8.2.0/twilio/rest/voice/v1/
--rw-r--r--   0 runner    (1001) docker     (123)     3035 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/voice/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3316 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/voice/v1/archived_call.py
--rw-r--r--   0 runner    (1001) docker     (123)    37359 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/voice/v1/byoc_trunk.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.324207 twilio-8.2.0/twilio/rest/voice/v1/connection_policy/
--rw-r--r--   0 runner    (1001) docker     (123)    20484 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/voice/v1/connection_policy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    29170 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/voice/v1/connection_policy/connection_policy_target.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.328207 twilio-8.2.0/twilio/rest/voice/v1/dialing_permissions/
--rw-r--r--   0 runner    (1001) docker     (123)     2327 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/voice/v1/dialing_permissions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3837 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/voice/v1/dialing_permissions/bulk_country_update.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.328207 twilio-8.2.0/twilio/rest/voice/v1/dialing_permissions/country/
--rw-r--r--   0 runner    (1001) docker     (123)    26486 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/voice/v1/dialing_permissions/country/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11128 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/voice/v1/dialing_permissions/country/highrisk_special_prefix.py
--rw-r--r--   0 runner    (1001) docker     (123)     6995 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/voice/v1/dialing_permissions/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)    20413 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/voice/v1/ip_record.py
--rw-r--r--   0 runner    (1001) docker     (123)    19429 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/voice/v1/source_ip_mapping.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.328207 twilio-8.2.0/twilio/rest/wireless/
--rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/wireless/WirelessBase.py
--rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/wireless/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.328207 twilio-8.2.0/twilio/rest/wireless/v1/
--rw-r--r--   0 runner    (1001) docker     (123)     2135 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/wireless/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    27361 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/wireless/v1/command.py
--rw-r--r--   0 runner    (1001) docker     (123)    29604 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/wireless/v1/rate_plan.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.328207 twilio-8.2.0/twilio/rest/wireless/v1/sim/
--rw-r--r--   0 runner    (1001) docker     (123)    46125 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/wireless/v1/sim/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14307 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/wireless/v1/sim/data_session.py
--rw-r--r--   0 runner    (1001) docker     (123)    17463 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/wireless/v1/sim/usage_record.py
--rw-r--r--   0 runner    (1001) docker     (123)    16059 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/rest/wireless/v1/usage_record.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.332207 twilio-8.2.0/twilio/twiml/
--rw-r--r--   0 runner    (1001) docker     (123)     3471 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/twiml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/twiml/fax_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2935 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/twiml/messaging_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    82958 2023-05-04 09:30:30.000000 twilio-8.2.0/twilio/twiml/voice_response.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:45.152205 twilio-8.2.0/twilio.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    11938 2023-05-04 09:30:45.000000 twilio-8.2.0/twilio.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    30316 2023-05-04 09:30:45.000000 twilio-8.2.0/twilio.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 09:30:45.000000 twilio-8.2.0/twilio.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-05-04 09:30:45.000000 twilio-8.2.0/twilio.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-04 09:30:45.000000 twilio-8.2.0/twilio.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 08:05:51.036838 twilio-8.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1387 2023-05-18 08:05:37.000000 twilio-8.2.1/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-05-18 08:05:37.000000 twilio-8.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-05-18 08:05:37.000000 twilio-8.2.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    11938 2023-05-18 08:05:51.036838 twilio-8.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10921 2023-05-18 08:05:37.000000 twilio-8.2.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-05-18 08:05:51.036838 twilio-8.2.1/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1694 2023-05-18 08:05:37.000000 twilio-8.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 08:05:50.932836 twilio-8.2.1/twilio/
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 08:05:50.936836 twilio-8.2.1/twilio/base/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8153 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/base/client_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2019 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/base/deserialize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2978 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/base/domain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2890 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/base/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/base/instance_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/base/instance_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/base/list_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1417 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/base/obsolete.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5181 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/base/page.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2039 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/base/serialize.py
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/base/values.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14614 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/base/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 08:05:50.936836 twilio-8.2.1/twilio/http/
+-rw-r--r--   0 runner    (1001) docker     (123)     3434 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/http/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4503 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/http/async_http_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3735 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/http/http_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2655 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/http/request.py
+-rw-r--r--   0 runner    (1001) docker     (123)      518 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/http/response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4810 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/http/validation_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 08:05:50.936836 twilio-8.2.1/twilio/jwt/
+-rw-r--r--   0 runner    (1001) docker     (123)     5085 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/jwt/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 08:05:50.940837 twilio-8.2.1/twilio/jwt/access_token/
+-rw-r--r--   0 runner    (1001) docker     (123)     2415 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/jwt/access_token/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4902 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/jwt/access_token/grants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 08:05:50.940837 twilio-8.2.1/twilio/jwt/client/
+-rw-r--r--   0 runner    (1001) docker     (123)     3982 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/jwt/client/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 08:05:50.940837 twilio-8.2.1/twilio/jwt/taskrouter/
+-rw-r--r--   0 runner    (1001) docker     (123)     5726 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/jwt/taskrouter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4309 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/jwt/taskrouter/capabilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 08:05:50.940837 twilio-8.2.1/twilio/jwt/validation/
+-rw-r--r--   0 runner    (1001) docker     (123)     3156 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/jwt/validation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4100 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/request_validator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 08:05:50.940837 twilio-8.2.1/twilio/rest/
+-rw-r--r--   0 runner    (1001) docker     (123)    20879 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 08:05:50.940837 twilio-8.2.1/twilio/rest/accounts/
+-rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/accounts/AccountsBase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/accounts/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 08:05:50.940837 twilio-8.2.1/twilio/rest/accounts/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)     2102 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/accounts/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5547 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/accounts/v1/auth_token_promotion.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 08:05:50.940837 twilio-8.2.1/twilio/rest/accounts/v1/credential/
+-rw-r--r--   0 runner    (1001) docker     (123)     1766 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/accounts/v1/credential/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19489 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/accounts/v1/credential/aws.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20007 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/accounts/v1/credential/public_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6551 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/accounts/v1/secondary_auth_token.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 08:05:50.940837 twilio-8.2.1/twilio/rest/api/
+-rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/api/ApiBase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8255 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 08:05:50.940837 twilio-8.2.1/twilio/rest/api/v2010/
+-rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/api/v2010/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 08:05:50.944836 twilio-8.2.1/twilio/rest/api/v2010/account/
+-rw-r--r--   0 runner    (1001) docker     (123)    36206 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/api/v2010/account/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 08:05:50.944836 twilio-8.2.1/twilio/rest/api/v2010/account/address/
+-rw-r--r--   0 runner    (1001) docker     (123)    35858 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/api/v2010/account/address/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17044 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/api/v2010/account/address/dependent_phone_number.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47553 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/api/v2010/account/application.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17274 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/api/v2010/account/authorized_connect_app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 08:05:50.944836 twilio-8.2.1/twilio/rest/api/v2010/account/available_phone_number_country/
+-rw-r--r--   0 runner    (1001) docker     (123)    21427 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/api/v2010/account/available_phone_number_country/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46239 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/api/v2010/account/available_phone_number_country/local.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46210 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/api/v2010/account/available_phone_number_country/machine_to_machine.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45860 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/api/v2010/account/available_phone_number_country/mobile.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45930 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/api/v2010/account/available_phone_number_country/national.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46000 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/api/v2010/account/available_phone_number_country/shared_cost.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45930 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/api/v2010/account/available_phone_number_country/toll_free.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45790 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/api/v2010/account/available_phone_number_country/voip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3186 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/api/v2010/account/balance.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 08:05:50.948837 twilio-8.2.1/twilio/rest/api/v2010/account/call/
+-rw-r--r--   0 runner    (1001) docker     (123)    92392 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/api/v2010/account/call/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10658 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/api/v2010/account/call/event.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11932 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/api/v2010/account/call/feedback.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13986 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/api/v2010/account/call/feedback_summary.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28363 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/api/v2010/account/call/notification.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23472 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/api/v2010/account/call/payment.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38495 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/api/v2010/account/call/recording.py
+-rw-r--r--   0 runner    (1001) docker     (123)    77226 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/api/v2010/account/call/siprec.py
+-rw-r--r--   0 runner    (1001) docker     (123)    77116 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/api/v2010/account/call/stream.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5278 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/api/v2010/account/call/user_defined_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10898 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/api/v2010/account/call/user_defined_message_subscription.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 08:05:50.948837 twilio-8.2.1/twilio/rest/api/v2010/account/conference/
+-rw-r--r--   0 runner    (1001) docker     (123)    41186 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/api/v2010/account/conference/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    74737 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/api/v2010/account/conference/participant.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32729 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/api/v2010/account/conference/recording.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26539 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/api/v2010/account/connect_app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 08:05:50.948837 twilio-8.2.1/twilio/rest/api/v2010/account/incoming_phone_number/
+-rw-r--r--   0 runner    (1001) docker     (123)    73374 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/api/v2010/account/incoming_phone_number/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 08:05:50.948837 twilio-8.2.1/twilio/rest/api/v2010/account/incoming_phone_number/assigned_add_on/
+-rw-r--r--   0 runner    (1001) docker     (123)    20750 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/api/v2010/account/incoming_phone_number/assigned_add_on/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18341 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/api/v2010/account/incoming_phone_number/assigned_add_on/assigned_add_on_extension.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36935 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/api/v2010/account/incoming_phone_number/local.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37019 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/api/v2010/account/incoming_phone_number/mobile.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37103 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/api/v2010/account/incoming_phone_number/toll_free.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17989 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/api/v2010/account/key.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 08:05:50.952837 twilio-8.2.1/twilio/rest/api/v2010/account/message/
+-rw-r--r--   0 runner    (1001) docker     (123)    53984 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/api/v2010/account/message/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5102 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/api/v2010/account/message/feedback.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27246 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/api/v2010/account/message/media.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4785 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/api/v2010/account/new_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4813 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/api/v2010/account/new_signing_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27505 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/api/v2010/account/notification.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22199 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/api/v2010/account/outgoing_caller_id.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 08:05:50.952837 twilio-8.2.1/twilio/rest/api/v2010/account/queue/
+-rw-r--r--   0 runner    (1001) docker     (123)    22428 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/api/v2010/account/queue/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19131 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/api/v2010/account/queue/member.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 08:05:50.952837 twilio-8.2.1/twilio/rest/api/v2010/account/recording/
+-rw-r--r--   0 runner    (1001) docker     (123)    37769 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/api/v2010/account/recording/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 08:05:50.952837 twilio-8.2.1/twilio/rest/api/v2010/account/recording/add_on_result/
+-rw-r--r--   0 runner    (1001) docker     (123)    19239 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/api/v2010/account/recording/add_on_result/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19233 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/api/v2010/account/recording/add_on_result/payload.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19008 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/api/v2010/account/recording/transcription.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26406 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/api/v2010/account/short_code.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17376 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/api/v2010/account/signing_key.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 08:05:50.952837 twilio-8.2.1/twilio/rest/api/v2010/account/sip/
+-rw-r--r--   0 runner    (1001) docker     (123)     2871 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/api/v2010/account/sip/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 08:05:50.952837 twilio-8.2.1/twilio/rest/api/v2010/account/sip/credential_list/
+-rw-r--r--   0 runner    (1001) docker     (123)    21278 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/api/v2010/account/sip/credential_list/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22757 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/api/v2010/account/sip/credential_list/credential.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 08:05:50.952837 twilio-8.2.1/twilio/rest/api/v2010/account/sip/domain/
+-rw-r--r--   0 runner    (1001) docker     (123)    45116 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/api/v2010/account/sip/domain/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 08:05:50.952837 twilio-8.2.1/twilio/rest/api/v2010/account/sip/domain/auth_types/
+-rw-r--r--   0 runner    (1001) docker     (123)     2758 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/api/v2010/account/sip/domain/auth_types/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 08:05:50.952837 twilio-8.2.1/twilio/rest/api/v2010/account/sip/domain/auth_types/auth_type_calls/
+-rw-r--r--   0 runner    (1001) docker     (123)     3330 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/api/v2010/account/sip/domain/auth_types/auth_type_calls/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20440 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/api/v2010/account/sip/domain/auth_types/auth_type_calls/auth_calls_credential_list_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20981 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/api/v2010/account/sip/domain/auth_types/auth_type_calls/auth_calls_ip_access_control_list_mapping.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 08:05:50.956837 twilio-8.2.1/twilio/rest/api/v2010/account/sip/domain/auth_types/auth_type_registrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     2473 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/api/v2010/account/sip/domain/auth_types/auth_type_registrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21048 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/api/v2010/account/sip/domain/auth_types/auth_type_registrations/auth_registrations_credential_list_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19893 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/api/v2010/account/sip/domain/credential_list_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20164 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/api/v2010/account/sip/domain/ip_access_control_list_mapping.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 08:05:50.956837 twilio-8.2.1/twilio/rest/api/v2010/account/sip/ip_access_control_list/
+-rw-r--r--   0 runner    (1001) docker     (123)    21808 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/api/v2010/account/sip/ip_access_control_list/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26238 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/api/v2010/account/sip/ip_access_control_list/ip_address.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4823 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/api/v2010/account/token.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18034 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/api/v2010/account/transcription.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 08:05:50.956837 twilio-8.2.1/twilio/rest/api/v2010/account/usage/
+-rw-r--r--   0 runner    (1001) docker     (123)     2220 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/api/v2010/account/usage/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 08:05:50.956837 twilio-8.2.1/twilio/rest/api/v2010/account/usage/record/
+-rw-r--r--   0 runner    (1001) docker     (123)    41695 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/api/v2010/account/usage/record/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38339 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/api/v2010/account/usage/record/all_time.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38247 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/api/v2010/account/usage/record/daily.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38431 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/api/v2010/account/usage/record/last_month.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38339 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/api/v2010/account/usage/record/monthly.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38431 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/api/v2010/account/usage/record/this_month.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38247 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/api/v2010/account/usage/record/today.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38293 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/api/v2010/account/usage/record/yearly.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38431 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/api/v2010/account/usage/record/yesterday.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49245 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/api/v2010/account/usage/trigger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7397 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/api/v2010/account/validation_request.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 08:05:50.956837 twilio-8.2.1/twilio/rest/autopilot/
+-rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/autopilot/AutopilotBase.py
+-rw-r--r--   0 runner    (1001) docker     (123)      778 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/autopilot/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 08:05:50.956837 twilio-8.2.1/twilio/rest/autopilot/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1680 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/autopilot/v1/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 08:05:50.960837 twilio-8.2.1/twilio/rest/autopilot/v1/assistant/
+-rw-r--r--   0 runner    (1001) docker     (123)    35087 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/autopilot/v1/assistant/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8479 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/autopilot/v1/assistant/defaults.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6698 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/autopilot/v1/assistant/dialogue.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 08:05:50.960837 twilio-8.2.1/twilio/rest/autopilot/v1/assistant/field_type/
+-rw-r--r--   0 runner    (1001) docker     (123)    23752 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/autopilot/v1/assistant/field_type/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22246 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/autopilot/v1/assistant/field_type/field_value.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22851 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/autopilot/v1/assistant/model_build.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29877 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/autopilot/v1/assistant/query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8288 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/autopilot/v1/assistant/style_sheet.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 08:05:50.960837 twilio-8.2.1/twilio/rest/autopilot/v1/assistant/task/
+-rw-r--r--   0 runner    (1001) docker     (123)    28213 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/autopilot/v1/assistant/task/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20115 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/autopilot/v1/assistant/task/field.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27891 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/autopilot/v1/assistant/task/sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9964 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/autopilot/v1/assistant/task/task_actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7530 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/autopilot/v1/assistant/task/task_statistics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24728 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/autopilot/v1/assistant/webhook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5222 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/autopilot/v1/restore_assistant.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 08:05:50.960837 twilio-8.2.1/twilio/rest/bulkexports/
+-rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/bulkexports/BulkexportsBase.py
+-rw-r--r--   0 runner    (1001) docker     (123)      792 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/bulkexports/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 08:05:50.960837 twilio-8.2.1/twilio/rest/bulkexports/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1692 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/bulkexports/v1/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 08:05:50.960837 twilio-8.2.1/twilio/rest/bulkexports/v1/export/
+-rw-r--r--   0 runner    (1001) docker     (123)     7083 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/bulkexports/v1/export/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14521 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/bulkexports/v1/export/day.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17005 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/bulkexports/v1/export/export_custom_job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8224 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/bulkexports/v1/export/job.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10811 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/bulkexports/v1/export_configuration.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 08:05:50.960837 twilio-8.2.1/twilio/rest/chat/
+-rw-r--r--   0 runner    (1001) docker     (123)     1700 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/chat/ChatBase.py
+-rw-r--r--   0 runner    (1001) docker     (123)      970 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/chat/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 08:05:50.964837 twilio-8.2.1/twilio/rest/chat/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1569 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/chat/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27856 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/chat/v1/credential.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 08:05:50.964837 twilio-8.2.1/twilio/rest/chat/v1/service/
+-rw-r--r--   0 runner    (1001) docker     (123)    92674 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/chat/v1/service/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 08:05:50.964837 twilio-8.2.1/twilio/rest/chat/v1/service/channel/
+-rw-r--r--   0 runner    (1001) docker     (123)    28967 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/chat/v1/service/channel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22312 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/chat/v1/service/channel/invite.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27709 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/chat/v1/service/channel/member.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26356 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/chat/v1/service/channel/message.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21831 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/chat/v1/service/role.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 08:05:50.964837 twilio-8.2.1/twilio/rest/chat/v1/service/user/
+-rw-r--r--   0 runner    (1001) docker     (123)    26317 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/chat/v1/service/user/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12925 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/chat/v1/service/user/user_channel.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 08:05:50.964837 twilio-8.2.1/twilio/rest/chat/v2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1569 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/chat/v2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27486 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/chat/v2/credential.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 08:05:50.964837 twilio-8.2.1/twilio/rest/chat/v2/service/
+-rw-r--r--   0 runner    (1001) docker     (123)    66570 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/chat/v2/service/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22118 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/chat/v2/service/binding.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 08:05:50.964837 twilio-8.2.1/twilio/rest/chat/v2/service/channel/
+-rw-r--r--   0 runner    (1001) docker     (123)    39123 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/chat/v2/service/channel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22292 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/chat/v2/service/channel/invite.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41109 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/chat/v2/service/channel/member.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37545 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/chat/v2/service/channel/message.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33770 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/chat/v2/service/channel/webhook.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22232 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/chat/v2/service/role.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 08:05:50.968837 twilio-8.2.1/twilio/rest/chat/v2/service/user/
+-rw-r--r--   0 runner    (1001) docker     (123)    29035 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/chat/v2/service/user/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21909 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/chat/v2/service/user/user_binding.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27050 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/chat/v2/service/user/user_channel.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 08:05:50.968837 twilio-8.2.1/twilio/rest/chat/v3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/chat/v3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11567 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/chat/v3/channel.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 08:05:50.968837 twilio-8.2.1/twilio/rest/content/
+-rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/content/ContentBase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/content/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 08:05:50.968837 twilio-8.2.1/twilio/rest/content/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/content/v1/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 08:05:50.968837 twilio-8.2.1/twilio/rest/content/v1/content/
+-rw-r--r--   0 runner    (1001) docker     (123)    16628 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/content/v1/content/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5839 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/content/v1/content/approval_fetch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11924 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/content/v1/content_and_approvals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12123 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/content/v1/legacy_content.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 08:05:50.968837 twilio-8.2.1/twilio/rest/conversations/
+-rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/conversations/ConversationsBase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2760 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/conversations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 08:05:50.968837 twilio-8.2.1/twilio/rest/conversations/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)     3659 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/conversations/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37619 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/conversations/v1/address_configuration.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 08:05:50.968837 twilio-8.2.1/twilio/rest/conversations/v1/configuration/
+-rw-r--r--   0 runner    (1001) docker     (123)    12497 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/conversations/v1/configuration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11083 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/conversations/v1/configuration/webhook.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 08:05:50.972837 twilio-8.2.1/twilio/rest/conversations/v1/conversation/
+-rw-r--r--   0 runner    (1001) docker     (123)    42957 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/conversations/v1/conversation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 08:05:50.972837 twilio-8.2.1/twilio/rest/conversations/v1/conversation/message/
+-rw-r--r--   0 runner    (1001) docker     (123)    34972 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/conversations/v1/conversation/message/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18063 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/conversations/v1/conversation/message/delivery_receipt.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40116 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/conversations/v1/conversation/participant.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27236 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/conversations/v1/conversation/webhook.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27935 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/conversations/v1/credential.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18739 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/conversations/v1/participant_conversation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20943 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/conversations/v1/role.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 08:05:50.972837 twilio-8.2.1/twilio/rest/conversations/v1/service/
+-rw-r--r--   0 runner    (1001) docker     (123)    20025 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/conversations/v1/service/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22289 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/conversations/v1/service/binding.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 08:05:50.972837 twilio-8.2.1/twilio/rest/conversations/v1/service/configuration/
+-rw-r--r--   0 runner    (1001) docker     (123)    16088 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/conversations/v1/service/configuration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24410 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/conversations/v1/service/configuration/notification.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13881 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/conversations/v1/service/configuration/webhook.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 08:05:50.972837 twilio-8.2.1/twilio/rest/conversations/v1/service/conversation/
+-rw-r--r--   0 runner    (1001) docker     (123)    44808 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/conversations/v1/service/conversation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 08:05:50.972837 twilio-8.2.1/twilio/rest/conversations/v1/service/conversation/message/
+-rw-r--r--   0 runner    (1001) docker     (123)    36629 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/conversations/v1/service/conversation/message/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19398 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/conversations/v1/service/conversation/message/delivery_receipt.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41799 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/conversations/v1/service/conversation/participant.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28926 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/conversations/v1/service/conversation/webhook.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19530 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/conversations/v1/service/participant_conversation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22534 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/conversations/v1/service/role.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 08:05:50.972837 twilio-8.2.1/twilio/rest/conversations/v1/service/user/
+-rw-r--r--   0 runner    (1001) docker     (123)    29682 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/conversations/v1/service/user/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26510 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/conversations/v1/service/user/user_conversation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 08:05:50.972837 twilio-8.2.1/twilio/rest/conversations/v1/user/
+-rw-r--r--   0 runner    (1001) docker     (123)    28016 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/conversations/v1/user/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25215 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/conversations/v1/user/user_conversation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 08:05:50.976837 twilio-8.2.1/twilio/rest/events/
+-rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/events/EventsBase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1277 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/events/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 08:05:50.976837 twilio-8.2.1/twilio/rest/events/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)     2133 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/events/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15317 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/events/v1/event_type.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 08:05:50.976837 twilio-8.2.1/twilio/rest/events/v1/schema/
+-rw-r--r--   0 runner    (1001) docker     (123)     6417 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/events/v1/schema/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14920 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/events/v1/schema/schema_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 08:05:50.976837 twilio-8.2.1/twilio/rest/events/v1/sink/
+-rw-r--r--   0 runner    (1001) docker     (123)    22872 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/events/v1/sink/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2768 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/events/v1/sink/sink_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3358 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/events/v1/sink/sink_validate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 08:05:50.976837 twilio-8.2.1/twilio/rest/events/v1/subscription/
+-rw-r--r--   0 runner    (1001) docker     (123)    22609 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/events/v1/subscription/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20282 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/events/v1/subscription/subscribed_event.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 08:05:50.976837 twilio-8.2.1/twilio/rest/flex_api/
+-rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/flex_api/FlexApiBase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6332 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/flex_api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 08:05:50.980837 twilio-8.2.1/twilio/rest/flex_api/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)     7374 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/flex_api/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23439 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/flex_api/v1/assessments.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19793 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/flex_api/v1/channel.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13488 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/flex_api/v1/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46860 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/flex_api/v1/flex_flow.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17361 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/flex_api/v1/insights_assessments_comment.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12870 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/flex_api/v1/insights_conversations.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27954 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/flex_api/v1/insights_questionnaires.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21091 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/flex_api/v1/insights_questionnaires_category.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26772 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/flex_api/v1/insights_questionnaires_question.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15944 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/flex_api/v1/insights_segments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5688 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/flex_api/v1/insights_session.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3164 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/flex_api/v1/insights_settings_answer_sets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2745 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/flex_api/v1/insights_settings_comment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5365 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/flex_api/v1/insights_user_roles.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 08:05:50.980837 twilio-8.2.1/twilio/rest/flex_api/v1/interaction/
+-rw-r--r--   0 runner    (1001) docker     (123)     8562 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/flex_api/v1/interaction/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 08:05:50.980837 twilio-8.2.1/twilio/rest/flex_api/v1/interaction/interaction_channel/
+-rw-r--r--   0 runner    (1001) docker     (123)    20915 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/flex_api/v1/interaction/interaction_channel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13861 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/flex_api/v1/interaction/interaction_channel/interaction_channel_invite.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19858 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/flex_api/v1/interaction/interaction_channel/interaction_channel_participant.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20821 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/flex_api/v1/web_channel.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 08:05:50.980837 twilio-8.2.1/twilio/rest/flex_api/v2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/flex_api/v2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5583 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/flex_api/v2/web_channels.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 08:05:50.980837 twilio-8.2.1/twilio/rest/frontline_api/
+-rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/frontline_api/FrontlineApiBase.py
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/frontline_api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 08:05:50.980837 twilio-8.2.1/twilio/rest/frontline_api/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1277 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/frontline_api/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10822 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/frontline_api/v1/user.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 08:05:50.980837 twilio-8.2.1/twilio/rest/insights/
+-rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/insights/InsightsBase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/insights/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 08:05:50.980837 twilio-8.2.1/twilio/rest/insights/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)     2419 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/insights/v1/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 08:05:50.984837 twilio-8.2.1/twilio/rest/insights/v1/call/
+-rw-r--r--   0 runner    (1001) docker     (123)     6981 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/insights/v1/call/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17445 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/insights/v1/call/annotation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9363 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/insights/v1/call/call_summary.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12166 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/insights/v1/call/event.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13146 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/insights/v1/call/metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31969 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/insights/v1/call_summaries.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 08:05:50.984837 twilio-8.2.1/twilio/rest/insights/v1/conference/
+-rw-r--r--   0 runner    (1001) docker     (123)    31370 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/insights/v1/conference/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25248 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/insights/v1/conference/conference_participant.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 08:05:50.984837 twilio-8.2.1/twilio/rest/insights/v1/room/
+-rw-r--r--   0 runner    (1001) docker     (123)    25243 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/insights/v1/room/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17908 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/insights/v1/room/participant.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8063 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/insights/v1/setting.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 08:05:50.984837 twilio-8.2.1/twilio/rest/ip_messaging/
+-rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/ip_messaging/IpMessagingBase.py
+-rw-r--r--   0 runner    (1001) docker     (123)      738 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/ip_messaging/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 08:05:50.984837 twilio-8.2.1/twilio/rest/ip_messaging/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/ip_messaging/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21632 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/ip_messaging/v1/credential.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 08:05:50.984837 twilio-8.2.1/twilio/rest/ip_messaging/v1/service/
+-rw-r--r--   0 runner    (1001) docker     (123)    62960 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/ip_messaging/v1/service/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 08:05:50.984837 twilio-8.2.1/twilio/rest/ip_messaging/v1/service/channel/
+-rw-r--r--   0 runner    (1001) docker     (123)    24064 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/ip_messaging/v1/service/channel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18541 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/ip_messaging/v1/service/channel/invite.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21725 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/ip_messaging/v1/service/channel/member.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21818 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/ip_messaging/v1/service/channel/message.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18855 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/ip_messaging/v1/service/role.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 08:05:50.988838 twilio-8.2.1/twilio/rest/ip_messaging/v1/service/user/
+-rw-r--r--   0 runner    (1001) docker     (123)    21365 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/ip_messaging/v1/service/user/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11548 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/ip_messaging/v1/service/user/user_channel.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 08:05:50.988838 twilio-8.2.1/twilio/rest/ip_messaging/v2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/ip_messaging/v2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21632 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/ip_messaging/v2/credential.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 08:05:50.988838 twilio-8.2.1/twilio/rest/ip_messaging/v2/service/
+-rw-r--r--   0 runner    (1001) docker     (123)    45390 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/ip_messaging/v2/service/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17907 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/ip_messaging/v2/service/binding.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 08:05:50.988838 twilio-8.2.1/twilio/rest/ip_messaging/v2/service/channel/
+-rw-r--r--   0 runner    (1001) docker     (123)    30568 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/ip_messaging/v2/service/channel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18541 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/ip_messaging/v2/service/channel/invite.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29520 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/ip_messaging/v2/service/channel/member.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28798 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/ip_messaging/v2/service/channel/message.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26175 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/ip_messaging/v2/service/channel/webhook.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18855 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/ip_messaging/v2/service/role.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 08:05:50.988838 twilio-8.2.1/twilio/rest/ip_messaging/v2/service/user/
+-rw-r--r--   0 runner    (1001) docker     (123)    24051 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/ip_messaging/v2/service/user/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18192 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/ip_messaging/v2/service/user/user_binding.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21476 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/ip_messaging/v2/service/user/user_channel.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 08:05:50.988838 twilio-8.2.1/twilio/rest/lookups/
+-rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/lookups/LookupsBase.py
+-rw-r--r--   0 runner    (1001) docker     (123)      432 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/lookups/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 08:05:50.988838 twilio-8.2.1/twilio/rest/lookups/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/lookups/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13250 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/lookups/v1/phone_number.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 08:05:50.988838 twilio-8.2.1/twilio/rest/lookups/v2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/lookups/v2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20961 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/lookups/v2/phone_number.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 08:05:50.988838 twilio-8.2.1/twilio/rest/media/
+-rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/media/MediaBase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/media/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 08:05:50.988838 twilio-8.2.1/twilio/rest/media/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)     2030 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/media/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26533 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/media/v1/media_processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22582 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/media/v1/media_recording.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 08:05:50.988838 twilio-8.2.1/twilio/rest/media/v1/player_streamer/
+-rw-r--r--   0 runner    (1001) docker     (123)    25414 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/media/v1/player_streamer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9432 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/media/v1/player_streamer/playback_grant.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 08:05:50.992838 twilio-8.2.1/twilio/rest/messaging/
+-rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/messaging/MessagingBase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3308 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/messaging/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 08:05:50.992838 twilio-8.2.1/twilio/rest/messaging/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)     5200 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/messaging/v1/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 08:05:50.992838 twilio-8.2.1/twilio/rest/messaging/v1/brand_registration/
+-rw-r--r--   0 runner    (1001) docker     (123)    24289 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/messaging/v1/brand_registration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3583 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/messaging/v1/brand_registration/brand_registration_otp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19914 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/messaging/v1/brand_registration/brand_vetting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5796 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/messaging/v1/deactivations.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10495 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/messaging/v1/domain_certs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13875 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/messaging/v1/domain_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7990 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/messaging/v1/domain_config_messaging_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4360 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/messaging/v1/external_campaign.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9216 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/messaging/v1/linkshortening_messaging_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7383 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/messaging/v1/linkshortening_messaging_service_domain_association.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 08:05:50.992838 twilio-8.2.1/twilio/rest/messaging/v1/service/
+-rw-r--r--   0 runner    (1001) docker     (123)    54653 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/messaging/v1/service/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18348 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/messaging/v1/service/alpha_sender.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18413 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/messaging/v1/service/phone_number.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18135 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/messaging/v1/service/short_code.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33395 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/messaging/v1/service/us_app_to_person.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3513 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/messaging/v1/service/us_app_to_person_usecase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2322 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/messaging/v1/usecase.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 08:05:50.992838 twilio-8.2.1/twilio/rest/microvisor/
+-rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/microvisor/MicrovisorBase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/microvisor/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 08:05:50.992838 twilio-8.2.1/twilio/rest/microvisor/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)     2211 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/microvisor/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17838 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/microvisor/v1/account_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17723 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/microvisor/v1/account_secret.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 08:05:50.992838 twilio-8.2.1/twilio/rest/microvisor/v1/app/
+-rw-r--r--   0 runner    (1001) docker     (123)    15664 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/microvisor/v1/app/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5534 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/microvisor/v1/app/app_manifest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 08:05:50.992838 twilio-8.2.1/twilio/rest/microvisor/v1/device/
+-rw-r--r--   0 runner    (1001) docker     (123)    20135 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/microvisor/v1/device/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19145 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/microvisor/v1/device/device_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19030 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/microvisor/v1/device/device_secret.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 08:05:50.996838 twilio-8.2.1/twilio/rest/monitor/
+-rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/monitor/MonitorBase.py
+-rw-r--r--   0 runner    (1001) docker     (123)      658 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/monitor/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 08:05:50.996838 twilio-8.2.1/twilio/rest/monitor/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1517 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/monitor/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22723 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/monitor/v1/alert.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25437 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/monitor/v1/event.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 08:05:50.996838 twilio-8.2.1/twilio/rest/notify/
+-rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/notify/NotifyBase.py
+-rw-r--r--   0 runner    (1001) docker     (123)      700 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/notify/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 08:05:50.996838 twilio-8.2.1/twilio/rest/notify/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1581 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/notify/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27961 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/notify/v1/credential.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 08:05:50.996838 twilio-8.2.1/twilio/rest/notify/v1/service/
+-rw-r--r--   0 runner    (1001) docker     (123)    47060 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/notify/v1/service/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30272 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/notify/v1/service/binding.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25490 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/notify/v1/service/notification.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 08:05:50.996838 twilio-8.2.1/twilio/rest/numbers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/numbers/NumbersBase.py
+-rw-r--r--   0 runner    (1001) docker     (123)      491 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/numbers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 08:05:50.996838 twilio-8.2.1/twilio/rest/numbers/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1374 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/numbers/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7086 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/numbers/v1/bulk_eligibility.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 08:05:50.996838 twilio-8.2.1/twilio/rest/numbers/v2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1414 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/numbers/v2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 08:05:50.996838 twilio-8.2.1/twilio/rest/numbers/v2/regulatory_compliance/
+-rw-r--r--   0 runner    (1001) docker     (123)     3690 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/numbers/v2/regulatory_compliance/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 08:05:50.996838 twilio-8.2.1/twilio/rest/numbers/v2/regulatory_compliance/bundle/
+-rw-r--r--   0 runner    (1001) docker     (123)    47502 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/numbers/v2/regulatory_compliance/bundle/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13880 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/numbers/v2/regulatory_compliance/bundle/bundle_copy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16186 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/numbers/v2/regulatory_compliance/bundle/evaluation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17833 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/numbers/v2/regulatory_compliance/bundle/item_assignment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5665 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/numbers/v2/regulatory_compliance/bundle/replace_items.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20500 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/numbers/v2/regulatory_compliance/end_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14140 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/numbers/v2/regulatory_compliance/end_user_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18536 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/numbers/v2/regulatory_compliance/regulation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22407 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/numbers/v2/regulatory_compliance/supporting_document.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14788 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/numbers/v2/regulatory_compliance/supporting_document_type.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 08:05:51.000838 twilio-8.2.1/twilio/rest/oauth/
+-rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/oauth/OauthBase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1578 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/oauth/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 08:05:51.000838 twilio-8.2.1/twilio/rest/oauth/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)     2434 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/oauth/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4598 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/oauth/v1/device_code.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4115 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/oauth/v1/oauth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7059 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/oauth/v1/openid_discovery.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6329 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/oauth/v1/token.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4714 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/oauth/v1/user_info.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 08:05:51.000838 twilio-8.2.1/twilio/rest/preview/
+-rw-r--r--   0 runner    (1001) docker     (123)     3081 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/preview/PreviewBase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3528 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/preview/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 08:05:51.000838 twilio-8.2.1/twilio/rest/preview/deployed_devices/
+-rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/preview/deployed_devices/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 08:05:51.000838 twilio-8.2.1/twilio/rest/preview/deployed_devices/fleet/
+-rw-r--r--   0 runner    (1001) docker     (123)    22442 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/preview/deployed_devices/fleet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24118 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/preview/deployed_devices/fleet/certificate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22163 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/preview/deployed_devices/fleet/deployment.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26656 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/preview/deployed_devices/fleet/device.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22726 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/preview/deployed_devices/fleet/key.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 08:05:51.000838 twilio-8.2.1/twilio/rest/preview/hosted_numbers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1892 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/preview/hosted_numbers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 08:05:51.000838 twilio-8.2.1/twilio/rest/preview/hosted_numbers/authorization_document/
+-rw-r--r--   0 runner    (1001) docker     (123)    32009 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/preview/hosted_numbers/authorization_document/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24829 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/preview/hosted_numbers/authorization_document/dependent_hosted_number_order.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48143 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/preview/hosted_numbers/hosted_number_order.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 08:05:51.000838 twilio-8.2.1/twilio/rest/preview/marketplace/
+-rw-r--r--   0 runner    (1001) docker     (123)     1775 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/preview/marketplace/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 08:05:51.000838 twilio-8.2.1/twilio/rest/preview/marketplace/available_add_on/
+-rw-r--r--   0 runner    (1001) docker     (123)    15067 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/preview/marketplace/available_add_on/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16163 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/preview/marketplace/available_add_on/available_add_on_extension.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 08:05:51.000838 twilio-8.2.1/twilio/rest/preview/marketplace/installed_add_on/
+-rw-r--r--   0 runner    (1001) docker     (123)    23293 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/preview/marketplace/installed_add_on/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18542 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/preview/marketplace/installed_add_on/installed_add_on_extension.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 08:05:51.000838 twilio-8.2.1/twilio/rest/preview/sync/
+-rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/preview/sync/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 08:05:51.000838 twilio-8.2.1/twilio/rest/preview/sync/service/
+-rw-r--r--   0 runner    (1001) docker     (123)    22270 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/preview/sync/service/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 08:05:51.000838 twilio-8.2.1/twilio/rest/preview/sync/service/document/
+-rw-r--r--   0 runner    (1001) docker     (123)    20547 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/preview/sync/service/document/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21455 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/preview/sync/service/document/document_permission.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 08:05:51.004838 twilio-8.2.1/twilio/rest/preview/sync/service/sync_list/
+-rw-r--r--   0 runner    (1001) docker     (123)    18339 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/preview/sync/service/sync_list/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24174 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/preview/sync/service/sync_list/sync_list_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21397 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/preview/sync/service/sync_list/sync_list_permission.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 08:05:51.004838 twilio-8.2.1/twilio/rest/preview/sync/service/sync_map/
+-rw-r--r--   0 runner    (1001) docker     (123)    18217 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/preview/sync/service/sync_map/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24063 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/preview/sync/service/sync_map/sync_map_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21250 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/preview/sync/service/sync_map/sync_map_permission.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 08:05:51.004838 twilio-8.2.1/twilio/rest/preview/understand/
+-rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/preview/understand/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 08:05:51.004838 twilio-8.2.1/twilio/rest/preview/understand/assistant/
+-rw-r--r--   0 runner    (1001) docker     (123)    35382 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/preview/understand/assistant/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8318 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/preview/understand/assistant/assistant_fallback_actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8510 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/preview/understand/assistant/assistant_initiation_actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5976 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/preview/understand/assistant/dialogue.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 08:05:51.004838 twilio-8.2.1/twilio/rest/preview/understand/assistant/field_type/
+-rw-r--r--   0 runner    (1001) docker     (123)    22348 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/preview/understand/assistant/field_type/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20410 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/preview/understand/assistant/field_type/field_value.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21062 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/preview/understand/assistant/model_build.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26433 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/preview/understand/assistant/query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7799 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/preview/understand/assistant/style_sheet.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 08:05:51.004838 twilio-8.2.1/twilio/rest/preview/understand/assistant/task/
+-rw-r--r--   0 runner    (1001) docker     (123)    26813 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/preview/understand/assistant/task/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19110 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/preview/understand/assistant/task/field.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24937 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/preview/understand/assistant/task/sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8816 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/preview/understand/assistant/task/task_actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6871 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/preview/understand/assistant/task/task_statistics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 08:05:51.004838 twilio-8.2.1/twilio/rest/preview/wireless/
+-rw-r--r--   0 runner    (1001) docker     (123)     1849 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/preview/wireless/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18911 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/preview/wireless/command.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21681 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/preview/wireless/rate_plan.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 08:05:51.004838 twilio-8.2.1/twilio/rest/preview/wireless/sim/
+-rw-r--r--   0 runner    (1001) docker     (123)    28867 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/preview/wireless/sim/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6592 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/preview/wireless/sim/usage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 08:05:51.004838 twilio-8.2.1/twilio/rest/pricing/
+-rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/pricing/PricingBase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1569 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/pricing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 08:05:51.008838 twilio-8.2.1/twilio/rest/pricing/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1867 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/pricing/v1/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 08:05:51.008838 twilio-8.2.1/twilio/rest/pricing/v1/messaging/
+-rw-r--r--   0 runner    (1001) docker     (123)     1443 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/pricing/v1/messaging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14530 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/pricing/v1/messaging/country.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 08:05:51.008838 twilio-8.2.1/twilio/rest/pricing/v1/phone_number/
+-rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/pricing/v1/phone_number/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14123 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/pricing/v1/phone_number/country.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 08:05:51.008838 twilio-8.2.1/twilio/rest/pricing/v1/voice/
+-rw-r--r--   0 runner    (1001) docker     (123)     1753 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/pricing/v1/voice/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14416 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/pricing/v1/voice/country.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5701 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/pricing/v1/voice/number.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 08:05:51.008838 twilio-8.2.1/twilio/rest/pricing/v2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1801 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/pricing/v2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14470 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/pricing/v2/country.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8966 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/pricing/v2/number.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 08:05:51.008838 twilio-8.2.1/twilio/rest/pricing/v2/voice/
+-rw-r--r--   0 runner    (1001) docker     (123)     1753 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/pricing/v2/voice/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14446 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/pricing/v2/voice/country.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9040 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/pricing/v2/voice/number.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 08:05:51.008838 twilio-8.2.1/twilio/rest/proxy/
+-rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/proxy/ProxyBase.py
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/proxy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 08:05:51.008838 twilio-8.2.1/twilio/rest/proxy/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1273 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/proxy/v1/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 08:05:51.008838 twilio-8.2.1/twilio/rest/proxy/v1/service/
+-rw-r--r--   0 runner    (1001) docker     (123)    38044 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/proxy/v1/service/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23754 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/proxy/v1/service/phone_number.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 08:05:51.008838 twilio-8.2.1/twilio/rest/proxy/v1/service/session/
+-rw-r--r--   0 runner    (1001) docker     (123)    27767 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/proxy/v1/service/session/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21109 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/proxy/v1/service/session/interaction.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 08:05:51.008838 twilio-8.2.1/twilio/rest/proxy/v1/service/session/participant/
+-rw-r--r--   0 runner    (1001) docker     (123)    22765 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/proxy/v1/service/session/participant/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23242 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/proxy/v1/service/session/participant/message_interaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21333 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/proxy/v1/service/short_code.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 08:05:51.008838 twilio-8.2.1/twilio/rest/routes/
+-rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/routes/RoutesBase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/routes/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 08:05:51.008838 twilio-8.2.1/twilio/rest/routes/v2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1876 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/routes/v2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9727 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/routes/v2/phone_number.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8319 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/routes/v2/sip_domain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9536 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/routes/v2/trunk.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 08:05:51.012838 twilio-8.2.1/twilio/rest/serverless/
+-rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/serverless/ServerlessBase.py
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/serverless/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 08:05:51.012838 twilio-8.2.1/twilio/rest/serverless/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1298 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/serverless/v1/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 08:05:51.012838 twilio-8.2.1/twilio/rest/serverless/v1/service/
+-rw-r--r--   0 runner    (1001) docker     (123)    25510 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/serverless/v1/service/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 08:05:51.012838 twilio-8.2.1/twilio/rest/serverless/v1/service/asset/
+-rw-r--r--   0 runner    (1001) docker     (123)    20582 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/serverless/v1/service/asset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16714 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/serverless/v1/service/asset/asset_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 08:05:51.012838 twilio-8.2.1/twilio/rest/serverless/v1/service/build/
+-rw-r--r--   0 runner    (1001) docker     (123)    20195 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/serverless/v1/service/build/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6403 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/serverless/v1/service/build/build_status.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 08:05:51.012838 twilio-8.2.1/twilio/rest/serverless/v1/service/environment/
+-rw-r--r--   0 runner    (1001) docker     (123)    21009 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/serverless/v1/service/environment/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18049 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/serverless/v1/service/environment/deployment.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20926 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/serverless/v1/service/environment/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22598 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/serverless/v1/service/environment/variable.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 08:05:51.012838 twilio-8.2.1/twilio/rest/serverless/v1/service/function/
+-rw-r--r--   0 runner    (1001) docker     (123)    20928 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/serverless/v1/service/function/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 08:05:51.012838 twilio-8.2.1/twilio/rest/serverless/v1/service/function/function_version/
+-rw-r--r--   0 runner    (1001) docker     (123)    18093 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/serverless/v1/service/function/function_version/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7736 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/serverless/v1/service/function/function_version/function_version_content.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 08:05:51.012838 twilio-8.2.1/twilio/rest/studio/
+-rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/studio/StudioBase.py
+-rw-r--r--   0 runner    (1001) docker     (123)      694 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/studio/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 08:05:51.012838 twilio-8.2.1/twilio/rest/studio/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/studio/v1/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 08:05:51.012838 twilio-8.2.1/twilio/rest/studio/v1/flow/
+-rw-r--r--   0 runner    (1001) docker     (123)    16404 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/studio/v1/flow/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 08:05:51.012838 twilio-8.2.1/twilio/rest/studio/v1/flow/engagement/
+-rw-r--r--   0 runner    (1001) docker     (123)    21366 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/studio/v1/flow/engagement/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6720 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/studio/v1/flow/engagement/engagement_context.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 08:05:51.012838 twilio-8.2.1/twilio/rest/studio/v1/flow/engagement/step/
+-rw-r--r--   0 runner    (1001) docker     (123)    17219 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/studio/v1/flow/engagement/step/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7395 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/studio/v1/flow/engagement/step/step_context.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 08:05:51.012838 twilio-8.2.1/twilio/rest/studio/v1/flow/execution/
+-rw-r--r--   0 runner    (1001) docker     (123)    27270 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/studio/v1/flow/execution/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6877 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/studio/v1/flow/execution/execution_context.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 08:05:51.012838 twilio-8.2.1/twilio/rest/studio/v1/flow/execution/execution_step/
+-rw-r--r--   0 runner    (1001) docker     (123)    17888 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/studio/v1/flow/execution/execution_step/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7716 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/studio/v1/flow/execution/execution_step/execution_step_context.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 08:05:51.016838 twilio-8.2.1/twilio/rest/studio/v2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/studio/v2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 08:05:51.016838 twilio-8.2.1/twilio/rest/studio/v2/flow/
+-rw-r--r--   0 runner    (1001) docker     (123)    23658 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/studio/v2/flow/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 08:05:51.016838 twilio-8.2.1/twilio/rest/studio/v2/flow/execution/
+-rw-r--r--   0 runner    (1001) docker     (123)    27154 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/studio/v2/flow/execution/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6877 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/studio/v2/flow/execution/execution_context.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 08:05:51.016838 twilio-8.2.1/twilio/rest/studio/v2/flow/execution/execution_step/
+-rw-r--r--   0 runner    (1001) docker     (123)    17888 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/studio/v2/flow/execution/execution_step/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7716 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/studio/v2/flow/execution/execution_step/execution_step_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16059 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/studio/v2/flow/flow_revision.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7422 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/studio/v2/flow/flow_test_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3892 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/studio/v2/flow_validate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 08:05:51.016838 twilio-8.2.1/twilio/rest/supersim/
+-rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/supersim/SupersimBase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2908 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/supersim/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 08:05:51.016838 twilio-8.2.1/twilio/rest/supersim/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)     3800 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/supersim/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23623 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/supersim/v1/esim_profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35226 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/supersim/v1/fleet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26640 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/supersim/v1/ip_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17582 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/supersim/v1/network.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 08:05:51.016838 twilio-8.2.1/twilio/rest/supersim/v1/network_access_profile/
+-rw-r--r--   0 runner    (1001) docker     (123)    20071 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/supersim/v1/network_access_profile/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19359 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/supersim/v1/network_access_profile/network_access_profile_network.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14206 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/supersim/v1/settings_update.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 08:05:51.016838 twilio-8.2.1/twilio/rest/supersim/v1/sim/
+-rw-r--r--   0 runner    (1001) docker     (123)    28732 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/supersim/v1/sim/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12030 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/supersim/v1/sim/billing_period.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10625 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/supersim/v1/sim/sim_ip_address.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23001 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/supersim/v1/sms_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26841 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/supersim/v1/usage_record.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 08:05:51.016838 twilio-8.2.1/twilio/rest/sync/
+-rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/sync/SyncBase.py
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/sync/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 08:05:51.016838 twilio-8.2.1/twilio/rest/sync/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/sync/v1/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 08:05:51.016838 twilio-8.2.1/twilio/rest/sync/v1/service/
+-rw-r--r--   0 runner    (1001) docker     (123)    36623 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/sync/v1/service/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 08:05:51.020838 twilio-8.2.1/twilio/rest/sync/v1/service/document/
+-rw-r--r--   0 runner    (1001) docker     (123)    25373 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/sync/v1/service/document/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21822 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/sync/v1/service/document/document_permission.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 08:05:51.020838 twilio-8.2.1/twilio/rest/sync/v1/service/sync_list/
+-rw-r--r--   0 runner    (1001) docker     (123)    25198 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/sync/v1/service/sync_list/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36671 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/sync/v1/service/sync_list/sync_list_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21826 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/sync/v1/service/sync_list/sync_list_permission.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 08:05:51.020838 twilio-8.2.1/twilio/rest/sync/v1/service/sync_map/
+-rw-r--r--   0 runner    (1001) docker     (123)    24886 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/sync/v1/service/sync_map/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37230 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/sync/v1/service/sync_map/sync_map_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21754 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/sync/v1/service/sync_map/sync_map_permission.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 08:05:51.020838 twilio-8.2.1/twilio/rest/sync/v1/service/sync_stream/
+-rw-r--r--   0 runner    (1001) docker     (123)    22899 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/sync/v1/service/sync_stream/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4315 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/sync/v1/service/sync_stream/stream_message.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 08:05:51.020838 twilio-8.2.1/twilio/rest/taskrouter/
+-rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/taskrouter/TaskrouterBase.py
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/taskrouter/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 08:05:51.020838 twilio-8.2.1/twilio/rest/taskrouter/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/taskrouter/v1/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 08:05:51.020838 twilio-8.2.1/twilio/rest/taskrouter/v1/workspace/
+-rw-r--r--   0 runner    (1001) docker     (123)    44452 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/taskrouter/v1/workspace/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25986 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/taskrouter/v1/workspace/activity.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32776 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/taskrouter/v1/workspace/event.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 08:05:51.020838 twilio-8.2.1/twilio/rest/taskrouter/v1/workspace/task/
+-rw-r--r--   0 runner    (1001) docker     (123)    51478 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/taskrouter/v1/workspace/task/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    79751 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/taskrouter/v1/workspace/task/reservation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23470 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/taskrouter/v1/workspace/task_channel.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 08:05:51.020838 twilio-8.2.1/twilio/rest/taskrouter/v1/workspace/task_queue/
+-rw-r--r--   0 runner    (1001) docker     (123)    39230 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/taskrouter/v1/workspace/task_queue/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18318 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/taskrouter/v1/workspace/task_queue/task_queue_cumulative_statistics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10983 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/taskrouter/v1/workspace/task_queue/task_queue_real_time_statistics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13380 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/taskrouter/v1/workspace/task_queue/task_queue_statistics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21315 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/taskrouter/v1/workspace/task_queue/task_queues_statistics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 08:05:51.024838 twilio-8.2.1/twilio/rest/taskrouter/v1/workspace/worker/
+-rw-r--r--   0 runner    (1001) docker     (123)    43462 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/taskrouter/v1/workspace/worker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    77533 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/taskrouter/v1/workspace/worker/reservation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22091 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/taskrouter/v1/workspace/worker/worker_channel.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11730 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/taskrouter/v1/workspace/worker/worker_statistics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13241 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/taskrouter/v1/workspace/worker/workers_cumulative_statistics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7884 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/taskrouter/v1/workspace/worker/workers_real_time_statistics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13545 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/taskrouter/v1/workspace/worker/workers_statistics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 08:05:51.024838 twilio-8.2.1/twilio/rest/taskrouter/v1/workspace/workflow/
+-rw-r--r--   0 runner    (1001) docker     (123)    34579 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/taskrouter/v1/workspace/workflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19228 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/taskrouter/v1/workspace/workflow/workflow_cumulative_statistics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9689 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/taskrouter/v1/workspace/workflow/workflow_real_time_statistics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14701 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/taskrouter/v1/workspace/workflow/workflow_statistics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18165 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/taskrouter/v1/workspace/workspace_cumulative_statistics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9027 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/taskrouter/v1/workspace/workspace_real_time_statistics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13564 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/taskrouter/v1/workspace/workspace_statistics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 08:05:51.024838 twilio-8.2.1/twilio/rest/trunking/
+-rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/trunking/TrunkingBase.py
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/trunking/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 08:05:51.024838 twilio-8.2.1/twilio/rest/trunking/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/trunking/v1/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 08:05:51.024838 twilio-8.2.1/twilio/rest/trunking/v1/trunk/
+-rw-r--r--   0 runner    (1001) docker     (123)    39976 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/trunking/v1/trunk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18350 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/trunking/v1/trunk/credential_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18720 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/trunking/v1/trunk/ip_access_control_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27739 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/trunking/v1/trunk/origination_url.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22459 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/trunking/v1/trunk/phone_number.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8181 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/trunking/v1/trunk/recording.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 08:05:51.024838 twilio-8.2.1/twilio/rest/trusthub/
+-rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/trusthub/TrusthubBase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2483 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/trusthub/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 08:05:51.024838 twilio-8.2.1/twilio/rest/trusthub/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)     3431 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/trusthub/v1/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 08:05:51.028838 twilio-8.2.1/twilio/rest/trusthub/v1/customer_profiles/
+-rw-r--r--   0 runner    (1001) docker     (123)    30761 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/trusthub/v1/customer_profiles/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23437 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/trusthub/v1/customer_profiles/customer_profiles_channel_endpoint_assignment.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19934 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/trusthub/v1/customer_profiles/customer_profiles_entity_assignments.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18436 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/trusthub/v1/customer_profiles/customer_profiles_evaluations.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20560 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/trusthub/v1/end_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14103 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/trusthub/v1/end_user_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13542 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/trusthub/v1/policies.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22191 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/trusthub/v1/supporting_document.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14729 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/trusthub/v1/supporting_document_type.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 08:05:51.028838 twilio-8.2.1/twilio/rest/trusthub/v1/trust_products/
+-rw-r--r--   0 runner    (1001) docker     (123)    30206 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/trusthub/v1/trust_products/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23131 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/trusthub/v1/trust_products/trust_products_channel_endpoint_assignment.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19505 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/trusthub/v1/trust_products/trust_products_entity_assignments.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18057 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/trusthub/v1/trust_products/trust_products_evaluations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 08:05:51.028838 twilio-8.2.1/twilio/rest/verify/
+-rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/verify/VerifyBase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2056 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/verify/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 08:05:51.028838 twilio-8.2.1/twilio/rest/verify/v2/
+-rw-r--r--   0 runner    (1001) docker     (123)     2992 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/verify/v2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5695 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/verify/v2/form.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8036 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/verify/v2/safelist.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 08:05:51.028838 twilio-8.2.1/twilio/rest/verify/v2/service/
+-rw-r--r--   0 runner    (1001) docker     (123)    55315 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/verify/v2/service/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10267 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/verify/v2/service/access_token.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 08:05:51.028838 twilio-8.2.1/twilio/rest/verify/v2/service/entity/
+-rw-r--r--   0 runner    (1001) docker     (123)    20668 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/verify/v2/service/entity/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 08:05:51.028838 twilio-8.2.1/twilio/rest/verify/v2/service/entity/challenge/
+-rw-r--r--   0 runner    (1001) docker     (123)    34458 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/verify/v2/service/entity/challenge/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6557 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/verify/v2/service/entity/challenge/notification.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29593 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/verify/v2/service/entity/factor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16164 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/verify/v2/service/entity/new_factor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23201 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/verify/v2/service/messaging_configuration.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 08:05:51.032838 twilio-8.2.1/twilio/rest/verify/v2/service/rate_limit/
+-rw-r--r--   0 runner    (1001) docker     (123)    21507 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/verify/v2/service/rate_limit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22242 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/verify/v2/service/rate_limit/bucket.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21417 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/verify/v2/service/verification.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8363 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/verify/v2/service/verification_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25389 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/verify/v2/service/webhook.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11731 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/verify/v2/template.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29432 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/verify/v2/verification_attempt.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13009 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/verify/v2/verification_attempts_summary.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 08:05:51.032838 twilio-8.2.1/twilio/rest/video/
+-rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/video/VideoBase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2050 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/video/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 08:05:51.032838 twilio-8.2.1/twilio/rest/video/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)     2971 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/video/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34977 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/video/v1/composition.py
+-rw-r--r--   0 runner    (1001) docker     (123)    54707 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/video/v1/composition_hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14079 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/video/v1/composition_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27313 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/video/v1/recording.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13910 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/video/v1/recording_settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 08:05:51.032838 twilio-8.2.1/twilio/rest/video/v1/room/
+-rw-r--r--   0 runner    (1001) docker     (123)    38074 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/video/v1/room/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 08:05:51.032838 twilio-8.2.1/twilio/rest/video/v1/room/participant/
+-rw-r--r--   0 runner    (1001) docker     (123)    28698 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/video/v1/room/participant/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7905 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/video/v1/room/participant/anonymize.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16887 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/video/v1/room/participant/published_track.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6391 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/video/v1/room/participant/subscribe_rules.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17079 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/video/v1/room/participant/subscribed_track.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5087 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/video/v1/room/recording_rules.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24746 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/video/v1/room/room_recording.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 08:05:51.032838 twilio-8.2.1/twilio/rest/voice/
+-rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/voice/VoiceBase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2099 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/voice/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 08:05:51.032838 twilio-8.2.1/twilio/rest/voice/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)     3035 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/voice/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3316 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/voice/v1/archived_call.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37359 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/voice/v1/byoc_trunk.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 08:05:51.032838 twilio-8.2.1/twilio/rest/voice/v1/connection_policy/
+-rw-r--r--   0 runner    (1001) docker     (123)    20484 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/voice/v1/connection_policy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29170 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/voice/v1/connection_policy/connection_policy_target.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 08:05:51.036838 twilio-8.2.1/twilio/rest/voice/v1/dialing_permissions/
+-rw-r--r--   0 runner    (1001) docker     (123)     2327 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/voice/v1/dialing_permissions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3837 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/voice/v1/dialing_permissions/bulk_country_update.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 08:05:51.036838 twilio-8.2.1/twilio/rest/voice/v1/dialing_permissions/country/
+-rw-r--r--   0 runner    (1001) docker     (123)    26486 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/voice/v1/dialing_permissions/country/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11128 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/voice/v1/dialing_permissions/country/highrisk_special_prefix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6995 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/voice/v1/dialing_permissions/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20413 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/voice/v1/ip_record.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19429 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/voice/v1/source_ip_mapping.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 08:05:51.036838 twilio-8.2.1/twilio/rest/wireless/
+-rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/wireless/WirelessBase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/wireless/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 08:05:51.036838 twilio-8.2.1/twilio/rest/wireless/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)     2135 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/wireless/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27361 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/wireless/v1/command.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29604 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/wireless/v1/rate_plan.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 08:05:51.036838 twilio-8.2.1/twilio/rest/wireless/v1/sim/
+-rw-r--r--   0 runner    (1001) docker     (123)    46125 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/wireless/v1/sim/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14307 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/wireless/v1/sim/data_session.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17463 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/wireless/v1/sim/usage_record.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16059 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/rest/wireless/v1/usage_record.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 08:05:51.036838 twilio-8.2.1/twilio/twiml/
+-rw-r--r--   0 runner    (1001) docker     (123)     3471 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/twiml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/twiml/fax_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2935 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/twiml/messaging_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    82958 2023-05-18 08:05:37.000000 twilio-8.2.1/twilio/twiml/voice_response.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 08:05:50.936836 twilio-8.2.1/twilio.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11938 2023-05-18 08:05:50.000000 twilio-8.2.1/twilio.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    30474 2023-05-18 08:05:50.000000 twilio-8.2.1/twilio.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 08:05:50.000000 twilio-8.2.1/twilio.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-05-18 08:05:50.000000 twilio-8.2.1/twilio.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-18 08:05:50.000000 twilio-8.2.1/twilio.egg-info/top_level.txt
```

### Comparing `twilio-8.2.0/AUTHORS.md` & `twilio-8.2.1/AUTHORS.md`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/LICENSE` & `twilio-8.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/PKG-INFO` & `twilio-8.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: twilio
-Version: 8.2.0
+Version: 8.2.1
 Summary: Twilio API client and TwiML generator
 Home-page: https://github.com/twilio/twilio-python/
 Author: Twilio
 Author-email: help@twilio.com
 Keywords: twilio,twiml
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `twilio-8.2.0/README.md` & `twilio-8.2.1/README.md`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/setup.py` & `twilio-8.2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # python setup.py install
 #
 # You need to have the setuptools module installed. Try reading the setuptools
 # documentation: http://pypi.python.org/pypi/setuptools
 
 setup(
     name="twilio",
-    version="8.2.0",
+    version="8.2.1",
     description="Twilio API client and TwiML generator",
     author="Twilio",
     author_email="help@twilio.com",
     url="https://github.com/twilio/twilio-python/",
     keywords=["twilio", "twiml"],
     python_requires=">=3.7.0",
     install_requires=[
```

### Comparing `twilio-8.2.0/twilio/base/client_base.py` & `twilio-8.2.1/twilio/base/client_base.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/base/deserialize.py` & `twilio-8.2.1/twilio/base/deserialize.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/base/domain.py` & `twilio-8.2.1/twilio/base/domain.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/base/exceptions.py` & `twilio-8.2.1/twilio/base/exceptions.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/base/obsolete.py` & `twilio-8.2.1/twilio/base/obsolete.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/base/page.py` & `twilio-8.2.1/twilio/base/page.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/base/serialize.py` & `twilio-8.2.1/twilio/base/serialize.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/base/version.py` & `twilio-8.2.1/twilio/base/version.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/http/__init__.py` & `twilio-8.2.1/twilio/http/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/http/async_http_client.py` & `twilio-8.2.1/twilio/http/async_http_client.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/http/http_client.py` & `twilio-8.2.1/twilio/http/http_client.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/http/request.py` & `twilio-8.2.1/twilio/http/request.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/http/response.py` & `twilio-8.2.1/twilio/http/response.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/http/validation_client.py` & `twilio-8.2.1/twilio/http/validation_client.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/jwt/__init__.py` & `twilio-8.2.1/twilio/jwt/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/jwt/access_token/__init__.py` & `twilio-8.2.1/twilio/jwt/access_token/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/jwt/access_token/grants.py` & `twilio-8.2.1/twilio/jwt/access_token/grants.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/jwt/client/__init__.py` & `twilio-8.2.1/twilio/jwt/client/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/jwt/taskrouter/__init__.py` & `twilio-8.2.1/twilio/jwt/taskrouter/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/jwt/taskrouter/capabilities.py` & `twilio-8.2.1/twilio/jwt/taskrouter/capabilities.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/jwt/validation/__init__.py` & `twilio-8.2.1/twilio/jwt/validation/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/request_validator.py` & `twilio-8.2.1/twilio/request_validator.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/__init__.py` & `twilio-8.2.1/twilio/rest/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/accounts/AccountsBase.py` & `twilio-8.2.1/twilio/rest/accounts/AccountsBase.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/accounts/__init__.py` & `twilio-8.2.1/twilio/rest/accounts/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/accounts/v1/__init__.py` & `twilio-8.2.1/twilio/rest/accounts/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/accounts/v1/auth_token_promotion.py` & `twilio-8.2.1/twilio/rest/accounts/v1/auth_token_promotion.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/accounts/v1/credential/__init__.py` & `twilio-8.2.1/twilio/rest/accounts/v1/credential/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/accounts/v1/credential/aws.py` & `twilio-8.2.1/twilio/rest/accounts/v1/credential/aws.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/accounts/v1/credential/public_key.py` & `twilio-8.2.1/twilio/rest/accounts/v1/credential/public_key.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/accounts/v1/secondary_auth_token.py` & `twilio-8.2.1/twilio/rest/accounts/v1/secondary_auth_token.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/api/ApiBase.py` & `twilio-8.2.1/twilio/rest/api/ApiBase.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/api/__init__.py` & `twilio-8.2.1/twilio/rest/api/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/api/v2010/__init__.py` & `twilio-8.2.1/twilio/rest/api/v2010/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/api/v2010/account/__init__.py` & `twilio-8.2.1/twilio/rest/api/v2010/account/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/api/v2010/account/address/__init__.py` & `twilio-8.2.1/twilio/rest/api/v2010/account/address/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/api/v2010/account/address/dependent_phone_number.py` & `twilio-8.2.1/twilio/rest/api/v2010/account/address/dependent_phone_number.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/api/v2010/account/application.py` & `twilio-8.2.1/twilio/rest/api/v2010/account/application.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/api/v2010/account/authorized_connect_app.py` & `twilio-8.2.1/twilio/rest/api/v2010/account/authorized_connect_app.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/api/v2010/account/available_phone_number_country/__init__.py` & `twilio-8.2.1/twilio/rest/api/v2010/account/available_phone_number_country/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/api/v2010/account/available_phone_number_country/local.py` & `twilio-8.2.1/twilio/rest/api/v2010/account/available_phone_number_country/local.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/api/v2010/account/available_phone_number_country/machine_to_machine.py` & `twilio-8.2.1/twilio/rest/api/v2010/account/available_phone_number_country/machine_to_machine.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/api/v2010/account/available_phone_number_country/mobile.py` & `twilio-8.2.1/twilio/rest/api/v2010/account/available_phone_number_country/mobile.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/api/v2010/account/available_phone_number_country/national.py` & `twilio-8.2.1/twilio/rest/api/v2010/account/available_phone_number_country/national.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/api/v2010/account/available_phone_number_country/shared_cost.py` & `twilio-8.2.1/twilio/rest/api/v2010/account/available_phone_number_country/shared_cost.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/api/v2010/account/available_phone_number_country/toll_free.py` & `twilio-8.2.1/twilio/rest/api/v2010/account/available_phone_number_country/toll_free.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/api/v2010/account/available_phone_number_country/voip.py` & `twilio-8.2.1/twilio/rest/api/v2010/account/available_phone_number_country/voip.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/api/v2010/account/balance.py` & `twilio-8.2.1/twilio/rest/api/v2010/account/balance.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/api/v2010/account/call/__init__.py` & `twilio-8.2.1/twilio/rest/api/v2010/account/call/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/api/v2010/account/call/event.py` & `twilio-8.2.1/twilio/rest/api/v2010/account/call/event.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/api/v2010/account/call/feedback.py` & `twilio-8.2.1/twilio/rest/api/v2010/account/call/feedback.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/api/v2010/account/call/feedback_summary.py` & `twilio-8.2.1/twilio/rest/api/v2010/account/call/feedback_summary.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/api/v2010/account/call/notification.py` & `twilio-8.2.1/twilio/rest/api/v2010/account/call/notification.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/api/v2010/account/call/payment.py` & `twilio-8.2.1/twilio/rest/api/v2010/account/call/payment.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/api/v2010/account/call/recording.py` & `twilio-8.2.1/twilio/rest/api/v2010/account/call/recording.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/api/v2010/account/call/siprec.py` & `twilio-8.2.1/twilio/rest/api/v2010/account/call/siprec.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/api/v2010/account/call/stream.py` & `twilio-8.2.1/twilio/rest/api/v2010/account/call/stream.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/api/v2010/account/call/user_defined_message.py` & `twilio-8.2.1/twilio/rest/api/v2010/account/call/user_defined_message.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/api/v2010/account/call/user_defined_message_subscription.py` & `twilio-8.2.1/twilio/rest/api/v2010/account/call/user_defined_message_subscription.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/api/v2010/account/conference/__init__.py` & `twilio-8.2.1/twilio/rest/api/v2010/account/conference/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/api/v2010/account/conference/participant.py` & `twilio-8.2.1/twilio/rest/api/v2010/account/conference/participant.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/api/v2010/account/conference/recording.py` & `twilio-8.2.1/twilio/rest/api/v2010/account/conference/recording.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/api/v2010/account/connect_app.py` & `twilio-8.2.1/twilio/rest/api/v2010/account/connect_app.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/api/v2010/account/incoming_phone_number/__init__.py` & `twilio-8.2.1/twilio/rest/api/v2010/account/incoming_phone_number/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/api/v2010/account/incoming_phone_number/assigned_add_on/__init__.py` & `twilio-8.2.1/twilio/rest/api/v2010/account/incoming_phone_number/assigned_add_on/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/api/v2010/account/incoming_phone_number/assigned_add_on/assigned_add_on_extension.py` & `twilio-8.2.1/twilio/rest/api/v2010/account/incoming_phone_number/assigned_add_on/assigned_add_on_extension.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/api/v2010/account/incoming_phone_number/local.py` & `twilio-8.2.1/twilio/rest/api/v2010/account/incoming_phone_number/local.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/api/v2010/account/incoming_phone_number/mobile.py` & `twilio-8.2.1/twilio/rest/api/v2010/account/incoming_phone_number/mobile.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/api/v2010/account/incoming_phone_number/toll_free.py` & `twilio-8.2.1/twilio/rest/api/v2010/account/incoming_phone_number/toll_free.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/api/v2010/account/key.py` & `twilio-8.2.1/twilio/rest/api/v2010/account/key.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/api/v2010/account/message/__init__.py` & `twilio-8.2.1/twilio/rest/api/v2010/account/message/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/api/v2010/account/message/feedback.py` & `twilio-8.2.1/twilio/rest/api/v2010/account/message/feedback.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/api/v2010/account/message/media.py` & `twilio-8.2.1/twilio/rest/api/v2010/account/message/media.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/api/v2010/account/new_key.py` & `twilio-8.2.1/twilio/rest/api/v2010/account/new_key.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/api/v2010/account/new_signing_key.py` & `twilio-8.2.1/twilio/rest/api/v2010/account/new_signing_key.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/api/v2010/account/notification.py` & `twilio-8.2.1/twilio/rest/api/v2010/account/notification.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/api/v2010/account/outgoing_caller_id.py` & `twilio-8.2.1/twilio/rest/api/v2010/account/outgoing_caller_id.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/api/v2010/account/queue/__init__.py` & `twilio-8.2.1/twilio/rest/api/v2010/account/queue/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/api/v2010/account/queue/member.py` & `twilio-8.2.1/twilio/rest/api/v2010/account/queue/member.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/api/v2010/account/recording/__init__.py` & `twilio-8.2.1/twilio/rest/api/v2010/account/recording/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/api/v2010/account/recording/add_on_result/__init__.py` & `twilio-8.2.1/twilio/rest/api/v2010/account/recording/add_on_result/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/api/v2010/account/recording/add_on_result/payload.py` & `twilio-8.2.1/twilio/rest/api/v2010/account/recording/add_on_result/payload.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/api/v2010/account/recording/transcription.py` & `twilio-8.2.1/twilio/rest/api/v2010/account/recording/transcription.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/api/v2010/account/short_code.py` & `twilio-8.2.1/twilio/rest/api/v2010/account/short_code.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/api/v2010/account/signing_key.py` & `twilio-8.2.1/twilio/rest/api/v2010/account/signing_key.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/api/v2010/account/sip/__init__.py` & `twilio-8.2.1/twilio/rest/api/v2010/account/sip/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/api/v2010/account/sip/credential_list/__init__.py` & `twilio-8.2.1/twilio/rest/api/v2010/account/sip/credential_list/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/api/v2010/account/sip/credential_list/credential.py` & `twilio-8.2.1/twilio/rest/api/v2010/account/sip/credential_list/credential.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/api/v2010/account/sip/domain/__init__.py` & `twilio-8.2.1/twilio/rest/api/v2010/account/sip/domain/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/api/v2010/account/sip/domain/auth_types/__init__.py` & `twilio-8.2.1/twilio/rest/api/v2010/account/sip/domain/auth_types/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/api/v2010/account/sip/domain/auth_types/auth_type_calls/__init__.py` & `twilio-8.2.1/twilio/rest/api/v2010/account/sip/domain/auth_types/auth_type_calls/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/api/v2010/account/sip/domain/auth_types/auth_type_calls/auth_calls_credential_list_mapping.py` & `twilio-8.2.1/twilio/rest/api/v2010/account/sip/domain/auth_types/auth_type_calls/auth_calls_credential_list_mapping.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/api/v2010/account/sip/domain/auth_types/auth_type_calls/auth_calls_ip_access_control_list_mapping.py` & `twilio-8.2.1/twilio/rest/api/v2010/account/sip/domain/auth_types/auth_type_calls/auth_calls_ip_access_control_list_mapping.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/api/v2010/account/sip/domain/auth_types/auth_type_registrations/__init__.py` & `twilio-8.2.1/twilio/rest/api/v2010/account/sip/domain/auth_types/auth_type_registrations/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/api/v2010/account/sip/domain/auth_types/auth_type_registrations/auth_registrations_credential_list_mapping.py` & `twilio-8.2.1/twilio/rest/api/v2010/account/sip/domain/auth_types/auth_type_registrations/auth_registrations_credential_list_mapping.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/api/v2010/account/sip/domain/credential_list_mapping.py` & `twilio-8.2.1/twilio/rest/api/v2010/account/sip/domain/credential_list_mapping.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/api/v2010/account/sip/domain/ip_access_control_list_mapping.py` & `twilio-8.2.1/twilio/rest/api/v2010/account/sip/domain/ip_access_control_list_mapping.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/api/v2010/account/sip/ip_access_control_list/__init__.py` & `twilio-8.2.1/twilio/rest/api/v2010/account/sip/ip_access_control_list/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/api/v2010/account/sip/ip_access_control_list/ip_address.py` & `twilio-8.2.1/twilio/rest/api/v2010/account/sip/ip_access_control_list/ip_address.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/api/v2010/account/token.py` & `twilio-8.2.1/twilio/rest/api/v2010/account/token.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/api/v2010/account/transcription.py` & `twilio-8.2.1/twilio/rest/api/v2010/account/transcription.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/api/v2010/account/usage/__init__.py` & `twilio-8.2.1/twilio/rest/api/v2010/account/usage/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/api/v2010/account/usage/record/__init__.py` & `twilio-8.2.1/twilio/rest/api/v2010/account/usage/record/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/api/v2010/account/usage/record/all_time.py` & `twilio-8.2.1/twilio/rest/api/v2010/account/usage/record/all_time.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/api/v2010/account/usage/record/daily.py` & `twilio-8.2.1/twilio/rest/api/v2010/account/usage/record/daily.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/api/v2010/account/usage/record/last_month.py` & `twilio-8.2.1/twilio/rest/api/v2010/account/usage/record/last_month.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/api/v2010/account/usage/record/monthly.py` & `twilio-8.2.1/twilio/rest/api/v2010/account/usage/record/monthly.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/api/v2010/account/usage/record/this_month.py` & `twilio-8.2.1/twilio/rest/api/v2010/account/usage/record/this_month.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/api/v2010/account/usage/record/today.py` & `twilio-8.2.1/twilio/rest/api/v2010/account/usage/record/today.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/api/v2010/account/usage/record/yearly.py` & `twilio-8.2.1/twilio/rest/api/v2010/account/usage/record/yearly.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/api/v2010/account/usage/record/yesterday.py` & `twilio-8.2.1/twilio/rest/api/v2010/account/usage/record/yesterday.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/api/v2010/account/usage/trigger.py` & `twilio-8.2.1/twilio/rest/api/v2010/account/usage/trigger.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/api/v2010/account/validation_request.py` & `twilio-8.2.1/twilio/rest/api/v2010/account/validation_request.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/autopilot/AutopilotBase.py` & `twilio-8.2.1/twilio/rest/autopilot/AutopilotBase.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/autopilot/__init__.py` & `twilio-8.2.1/twilio/rest/autopilot/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/autopilot/v1/__init__.py` & `twilio-8.2.1/twilio/rest/autopilot/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/autopilot/v1/assistant/__init__.py` & `twilio-8.2.1/twilio/rest/autopilot/v1/assistant/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/autopilot/v1/assistant/defaults.py` & `twilio-8.2.1/twilio/rest/autopilot/v1/assistant/defaults.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/autopilot/v1/assistant/dialogue.py` & `twilio-8.2.1/twilio/rest/autopilot/v1/assistant/dialogue.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/autopilot/v1/assistant/field_type/__init__.py` & `twilio-8.2.1/twilio/rest/autopilot/v1/assistant/field_type/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/autopilot/v1/assistant/field_type/field_value.py` & `twilio-8.2.1/twilio/rest/autopilot/v1/assistant/field_type/field_value.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/autopilot/v1/assistant/model_build.py` & `twilio-8.2.1/twilio/rest/autopilot/v1/assistant/model_build.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/autopilot/v1/assistant/query.py` & `twilio-8.2.1/twilio/rest/autopilot/v1/assistant/query.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/autopilot/v1/assistant/style_sheet.py` & `twilio-8.2.1/twilio/rest/autopilot/v1/assistant/style_sheet.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/autopilot/v1/assistant/task/__init__.py` & `twilio-8.2.1/twilio/rest/autopilot/v1/assistant/task/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/autopilot/v1/assistant/task/field.py` & `twilio-8.2.1/twilio/rest/autopilot/v1/assistant/task/field.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/autopilot/v1/assistant/task/sample.py` & `twilio-8.2.1/twilio/rest/autopilot/v1/assistant/task/sample.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/autopilot/v1/assistant/task/task_actions.py` & `twilio-8.2.1/twilio/rest/autopilot/v1/assistant/task/task_actions.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/autopilot/v1/assistant/task/task_statistics.py` & `twilio-8.2.1/twilio/rest/autopilot/v1/assistant/task/task_statistics.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/autopilot/v1/assistant/webhook.py` & `twilio-8.2.1/twilio/rest/autopilot/v1/assistant/webhook.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/autopilot/v1/restore_assistant.py` & `twilio-8.2.1/twilio/rest/autopilot/v1/restore_assistant.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/bulkexports/BulkexportsBase.py` & `twilio-8.2.1/twilio/rest/bulkexports/BulkexportsBase.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/bulkexports/__init__.py` & `twilio-8.2.1/twilio/rest/bulkexports/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/bulkexports/v1/__init__.py` & `twilio-8.2.1/twilio/rest/bulkexports/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/bulkexports/v1/export/__init__.py` & `twilio-8.2.1/twilio/rest/bulkexports/v1/export/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/bulkexports/v1/export/day.py` & `twilio-8.2.1/twilio/rest/bulkexports/v1/export/day.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/bulkexports/v1/export/export_custom_job.py` & `twilio-8.2.1/twilio/rest/bulkexports/v1/export/export_custom_job.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/bulkexports/v1/export/job.py` & `twilio-8.2.1/twilio/rest/bulkexports/v1/export/job.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/bulkexports/v1/export_configuration.py` & `twilio-8.2.1/twilio/rest/bulkexports/v1/export_configuration.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/chat/ChatBase.py` & `twilio-8.2.1/twilio/rest/chat/ChatBase.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/chat/__init__.py` & `twilio-8.2.1/twilio/rest/chat/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/chat/v1/__init__.py` & `twilio-8.2.1/twilio/rest/chat/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/chat/v1/credential.py` & `twilio-8.2.1/twilio/rest/chat/v1/credential.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/chat/v1/service/__init__.py` & `twilio-8.2.1/twilio/rest/chat/v1/service/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/chat/v1/service/channel/__init__.py` & `twilio-8.2.1/twilio/rest/chat/v1/service/channel/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/chat/v1/service/channel/invite.py` & `twilio-8.2.1/twilio/rest/chat/v1/service/channel/invite.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/chat/v1/service/channel/member.py` & `twilio-8.2.1/twilio/rest/chat/v1/service/channel/member.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/chat/v1/service/channel/message.py` & `twilio-8.2.1/twilio/rest/chat/v1/service/channel/message.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/chat/v1/service/role.py` & `twilio-8.2.1/twilio/rest/chat/v1/service/role.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/chat/v1/service/user/__init__.py` & `twilio-8.2.1/twilio/rest/chat/v1/service/user/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/chat/v1/service/user/user_channel.py` & `twilio-8.2.1/twilio/rest/chat/v1/service/user/user_channel.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/chat/v2/__init__.py` & `twilio-8.2.1/twilio/rest/chat/v2/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/chat/v2/credential.py` & `twilio-8.2.1/twilio/rest/chat/v2/credential.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/chat/v2/service/__init__.py` & `twilio-8.2.1/twilio/rest/chat/v2/service/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/chat/v2/service/binding.py` & `twilio-8.2.1/twilio/rest/chat/v2/service/binding.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/chat/v2/service/channel/__init__.py` & `twilio-8.2.1/twilio/rest/chat/v2/service/channel/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/chat/v2/service/channel/invite.py` & `twilio-8.2.1/twilio/rest/chat/v2/service/channel/invite.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/chat/v2/service/channel/member.py` & `twilio-8.2.1/twilio/rest/chat/v2/service/channel/member.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/chat/v2/service/channel/message.py` & `twilio-8.2.1/twilio/rest/chat/v2/service/channel/message.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/chat/v2/service/channel/webhook.py` & `twilio-8.2.1/twilio/rest/chat/v2/service/channel/webhook.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/chat/v2/service/role.py` & `twilio-8.2.1/twilio/rest/chat/v2/service/role.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/chat/v2/service/user/__init__.py` & `twilio-8.2.1/twilio/rest/chat/v2/service/user/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/chat/v2/service/user/user_binding.py` & `twilio-8.2.1/twilio/rest/chat/v2/service/user/user_binding.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/chat/v2/service/user/user_channel.py` & `twilio-8.2.1/twilio/rest/chat/v2/service/user/user_channel.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/chat/v3/__init__.py` & `twilio-8.2.1/twilio/rest/chat/v3/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/chat/v3/channel.py` & `twilio-8.2.1/twilio/rest/chat/v3/channel.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/content/ContentBase.py` & `twilio-8.2.1/twilio/rest/content/ContentBase.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/content/__init__.py` & `twilio-8.2.1/twilio/rest/content/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/content/v1/__init__.py` & `twilio-8.2.1/twilio/rest/content/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/content/v1/content/__init__.py` & `twilio-8.2.1/twilio/rest/content/v1/content/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/content/v1/content/approval_fetch.py` & `twilio-8.2.1/twilio/rest/content/v1/content/approval_fetch.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/content/v1/content_and_approvals.py` & `twilio-8.2.1/twilio/rest/content/v1/content_and_approvals.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/content/v1/legacy_content.py` & `twilio-8.2.1/twilio/rest/content/v1/legacy_content.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/conversations/ConversationsBase.py` & `twilio-8.2.1/twilio/rest/conversations/ConversationsBase.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/conversations/__init__.py` & `twilio-8.2.1/twilio/rest/conversations/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/conversations/v1/__init__.py` & `twilio-8.2.1/twilio/rest/conversations/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/conversations/v1/address_configuration.py` & `twilio-8.2.1/twilio/rest/conversations/v1/address_configuration.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,14 +45,15 @@
     :ivar type: Type of Address, value can be `whatsapp` or `sms`.
     :ivar address: The unique address to be configured. The address can be a whatsapp address or phone number
     :ivar friendly_name: The human-readable name of this configuration, limited to 256 characters. Optional.
     :ivar auto_creation: Auto Creation configuration for the address.
     :ivar date_created: The date that this resource was created.
     :ivar date_updated: The date that this resource was last updated.
     :ivar url: An absolute API resource URL for this address configuration.
+    :ivar address_country: An ISO 3166-1 alpha-2n country code which the address belongs to. This is currently only applicable to short code addresses.
     """
 
     def __init__(
         self, version: Version, payload: Dict[str, Any], sid: Optional[str] = None
     ):
         super().__init__(version)
 
@@ -65,14 +66,15 @@
         self.date_created: Optional[datetime] = deserialize.iso8601_datetime(
             payload.get("date_created")
         )
         self.date_updated: Optional[datetime] = deserialize.iso8601_datetime(
             payload.get("date_updated")
         )
         self.url: Optional[str] = payload.get("url")
+        self.address_country: Optional[str] = payload.get("address_country")
 
         self._solution = {
             "sid": sid or self.sid,
         }
         self._context: Optional[AddressConfigurationContext] = None
 
     @property
@@ -471,14 +473,15 @@
         auto_creation_webhook_url: Union[str, object] = values.unset,
         auto_creation_webhook_method: Union[
             "AddressConfigurationInstance.Method", object
         ] = values.unset,
         auto_creation_webhook_filters: Union[List[str], object] = values.unset,
         auto_creation_studio_flow_sid: Union[str, object] = values.unset,
         auto_creation_studio_retry_count: Union[int, object] = values.unset,
+        address_country: Union[str, object] = values.unset,
     ) -> AddressConfigurationInstance:
         """
         Create the AddressConfigurationInstance
 
         :param type:
         :param address: The unique address to be configured. The address can be a whatsapp address or phone number
         :param friendly_name: The human-readable name of this configuration, limited to 256 characters. Optional.
@@ -486,14 +489,15 @@
         :param auto_creation_type:
         :param auto_creation_conversation_service_sid: Conversation Service for the auto-created conversation. If not set, the conversation is created in the default service.
         :param auto_creation_webhook_url: For type `webhook`, the url for the webhook request.
         :param auto_creation_webhook_method:
         :param auto_creation_webhook_filters: The list of events, firing webhook event for this Conversation. Values can be any of the following: `onMessageAdded`, `onMessageUpdated`, `onMessageRemoved`, `onConversationUpdated`, `onConversationStateUpdated`, `onConversationRemoved`, `onParticipantAdded`, `onParticipantUpdated`, `onParticipantRemoved`, `onDeliveryUpdated`
         :param auto_creation_studio_flow_sid: For type `studio`, the studio flow SID where the webhook should be sent to.
         :param auto_creation_studio_retry_count: For type `studio`, number of times to retry the webhook request
+        :param address_country: An ISO 3166-1 alpha-2n country code which the address belongs to. This is currently only applicable to short code addresses.
 
         :returns: The created AddressConfigurationInstance
         """
         data = values.of(
             {
                 "Type": type,
                 "Address": address,
@@ -504,14 +508,15 @@
                 "AutoCreation.WebhookUrl": auto_creation_webhook_url,
                 "AutoCreation.WebhookMethod": auto_creation_webhook_method,
                 "AutoCreation.WebhookFilters": serialize.map(
                     auto_creation_webhook_filters, lambda e: e
                 ),
                 "AutoCreation.StudioFlowSid": auto_creation_studio_flow_sid,
                 "AutoCreation.StudioRetryCount": auto_creation_studio_retry_count,
+                "AddressCountry": address_country,
             }
         )
 
         payload = self._version.create(
             method="POST",
             uri=self._uri,
             data=data,
@@ -532,14 +537,15 @@
         auto_creation_webhook_url: Union[str, object] = values.unset,
         auto_creation_webhook_method: Union[
             "AddressConfigurationInstance.Method", object
         ] = values.unset,
         auto_creation_webhook_filters: Union[List[str], object] = values.unset,
         auto_creation_studio_flow_sid: Union[str, object] = values.unset,
         auto_creation_studio_retry_count: Union[int, object] = values.unset,
+        address_country: Union[str, object] = values.unset,
     ) -> AddressConfigurationInstance:
         """
         Asynchronously create the AddressConfigurationInstance
 
         :param type:
         :param address: The unique address to be configured. The address can be a whatsapp address or phone number
         :param friendly_name: The human-readable name of this configuration, limited to 256 characters. Optional.
@@ -547,14 +553,15 @@
         :param auto_creation_type:
         :param auto_creation_conversation_service_sid: Conversation Service for the auto-created conversation. If not set, the conversation is created in the default service.
         :param auto_creation_webhook_url: For type `webhook`, the url for the webhook request.
         :param auto_creation_webhook_method:
         :param auto_creation_webhook_filters: The list of events, firing webhook event for this Conversation. Values can be any of the following: `onMessageAdded`, `onMessageUpdated`, `onMessageRemoved`, `onConversationUpdated`, `onConversationStateUpdated`, `onConversationRemoved`, `onParticipantAdded`, `onParticipantUpdated`, `onParticipantRemoved`, `onDeliveryUpdated`
         :param auto_creation_studio_flow_sid: For type `studio`, the studio flow SID where the webhook should be sent to.
         :param auto_creation_studio_retry_count: For type `studio`, number of times to retry the webhook request
+        :param address_country: An ISO 3166-1 alpha-2n country code which the address belongs to. This is currently only applicable to short code addresses.
 
         :returns: The created AddressConfigurationInstance
         """
         data = values.of(
             {
                 "Type": type,
                 "Address": address,
@@ -565,14 +572,15 @@
                 "AutoCreation.WebhookUrl": auto_creation_webhook_url,
                 "AutoCreation.WebhookMethod": auto_creation_webhook_method,
                 "AutoCreation.WebhookFilters": serialize.map(
                     auto_creation_webhook_filters, lambda e: e
                 ),
                 "AutoCreation.StudioFlowSid": auto_creation_studio_flow_sid,
                 "AutoCreation.StudioRetryCount": auto_creation_studio_retry_count,
+                "AddressCountry": address_country,
             }
         )
 
         payload = await self._version.create_async(
             method="POST",
             uri=self._uri,
             data=data,
```

### Comparing `twilio-8.2.0/twilio/rest/conversations/v1/configuration/__init__.py` & `twilio-8.2.1/twilio/rest/conversations/v1/configuration/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/conversations/v1/configuration/webhook.py` & `twilio-8.2.1/twilio/rest/conversations/v1/configuration/webhook.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/conversations/v1/conversation/__init__.py` & `twilio-8.2.1/twilio/rest/conversations/v1/service/conversation/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -17,17 +17,19 @@
 from typing import Any, Dict, List, Optional, Union, Iterator, AsyncIterator
 from twilio.base import deserialize, serialize, values
 from twilio.base.instance_context import InstanceContext
 from twilio.base.instance_resource import InstanceResource
 from twilio.base.list_resource import ListResource
 from twilio.base.version import Version
 from twilio.base.page import Page
-from twilio.rest.conversations.v1.conversation.message import MessageList
-from twilio.rest.conversations.v1.conversation.participant import ParticipantList
-from twilio.rest.conversations.v1.conversation.webhook import WebhookList
+from twilio.rest.conversations.v1.service.conversation.message import MessageList
+from twilio.rest.conversations.v1.service.conversation.participant import (
+    ParticipantList,
+)
+from twilio.rest.conversations.v1.service.conversation.webhook import WebhookList
 
 
 class ConversationInstance(InstanceResource):
     class State(object):
         INACTIVE = "inactive"
         ACTIVE = "active"
         CLOSED = "closed"
@@ -50,15 +52,19 @@
     :ivar timers: Timer date values representing state update for this conversation.
     :ivar url: An absolute API resource URL for this conversation.
     :ivar links: Contains absolute URLs to access the [participants](https://www.twilio.com/docs/conversations/api/conversation-participant-resource), [messages](https://www.twilio.com/docs/conversations/api/conversation-message-resource) and [webhooks](https://www.twilio.com/docs/conversations/api/conversation-scoped-webhook-resource) of this conversation.
     :ivar bindings: 
     """
 
     def __init__(
-        self, version: Version, payload: Dict[str, Any], sid: Optional[str] = None
+        self,
+        version: Version,
+        payload: Dict[str, Any],
+        chat_service_sid: str,
+        sid: Optional[str] = None,
     ):
         super().__init__(version)
 
         self.account_sid: Optional[str] = payload.get("account_sid")
         self.chat_service_sid: Optional[str] = payload.get("chat_service_sid")
         self.messaging_service_sid: Optional[str] = payload.get("messaging_service_sid")
         self.sid: Optional[str] = payload.get("sid")
@@ -74,14 +80,15 @@
         )
         self.timers: Optional[Dict[str, object]] = payload.get("timers")
         self.url: Optional[str] = payload.get("url")
         self.links: Optional[Dict[str, object]] = payload.get("links")
         self.bindings: Optional[Dict[str, object]] = payload.get("bindings")
 
         self._solution = {
+            "chat_service_sid": chat_service_sid,
             "sid": sid or self.sid,
         }
         self._context: Optional[ConversationContext] = None
 
     @property
     def _proxy(self) -> "ConversationContext":
         """
@@ -89,14 +96,15 @@
         performing various actions. All instance actions are proxied to the context
 
         :returns: ConversationContext for this ConversationInstance
         """
         if self._context is None:
             self._context = ConversationContext(
                 self._version,
+                chat_service_sid=self._solution["chat_service_sid"],
                 sid=self._solution["sid"],
             )
         return self._context
 
     def delete(
         self,
         x_twilio_webhook_enabled: Union[
@@ -265,28 +273,32 @@
         :returns: Machine friendly representation
         """
         context = " ".join("{}={}".format(k, v) for k, v in self._solution.items())
         return "<Twilio.Conversations.V1.ConversationInstance {}>".format(context)
 
 
 class ConversationContext(InstanceContext):
-    def __init__(self, version: Version, sid: str):
+    def __init__(self, version: Version, chat_service_sid: str, sid: str):
         """
         Initialize the ConversationContext
 
         :param version: Version that contains the resource
+        :param chat_service_sid: The SID of the [Conversation Service](https://www.twilio.com/docs/conversations/api/service-resource) the Conversation resource is associated with.
         :param sid: A 34 character string that uniquely identifies this resource. Can also be the `unique_name` of the Conversation.
         """
         super().__init__(version)
 
         # Path Solution
         self._solution = {
+            "chat_service_sid": chat_service_sid,
             "sid": sid,
         }
-        self._uri = "/Conversations/{sid}".format(**self._solution)
+        self._uri = "/Services/{chat_service_sid}/Conversations/{sid}".format(
+            **self._solution
+        )
 
         self._messages: Optional[MessageList] = None
         self._participants: Optional[ParticipantList] = None
         self._webhooks: Optional[WebhookList] = None
 
     def delete(
         self,
@@ -344,14 +356,15 @@
             method="GET",
             uri=self._uri,
         )
 
         return ConversationInstance(
             self._version,
             payload,
+            chat_service_sid=self._solution["chat_service_sid"],
             sid=self._solution["sid"],
         )
 
     async def fetch_async(self) -> ConversationInstance:
         """
         Asynchronous coroutine to fetch the ConversationInstance
 
@@ -363,14 +376,15 @@
             method="GET",
             uri=self._uri,
         )
 
         return ConversationInstance(
             self._version,
             payload,
+            chat_service_sid=self._solution["chat_service_sid"],
             sid=self._solution["sid"],
         )
 
     def update(
         self,
         x_twilio_webhook_enabled: Union[
             "ConversationInstance.WebhookEnabledType", object
@@ -420,15 +434,20 @@
             }
         )
 
         payload = self._version.update(
             method="POST", uri=self._uri, data=data, headers=headers
         )
 
-        return ConversationInstance(self._version, payload, sid=self._solution["sid"])
+        return ConversationInstance(
+            self._version,
+            payload,
+            chat_service_sid=self._solution["chat_service_sid"],
+            sid=self._solution["sid"],
+        )
 
     async def update_async(
         self,
         x_twilio_webhook_enabled: Union[
             "ConversationInstance.WebhookEnabledType", object
         ] = values.unset,
         friendly_name: Union[str, object] = values.unset,
@@ -476,48 +495,56 @@
             }
         )
 
         payload = await self._version.update_async(
             method="POST", uri=self._uri, data=data, headers=headers
         )
 
-        return ConversationInstance(self._version, payload, sid=self._solution["sid"])
+        return ConversationInstance(
+            self._version,
+            payload,
+            chat_service_sid=self._solution["chat_service_sid"],
+            sid=self._solution["sid"],
+        )
 
     @property
     def messages(self) -> MessageList:
         """
         Access the messages
         """
         if self._messages is None:
             self._messages = MessageList(
                 self._version,
+                self._solution["chat_service_sid"],
                 self._solution["sid"],
             )
         return self._messages
 
     @property
     def participants(self) -> ParticipantList:
         """
         Access the participants
         """
         if self._participants is None:
             self._participants = ParticipantList(
                 self._version,
+                self._solution["chat_service_sid"],
                 self._solution["sid"],
             )
         return self._participants
 
     @property
     def webhooks(self) -> WebhookList:
         """
         Access the webhooks
         """
         if self._webhooks is None:
             self._webhooks = WebhookList(
                 self._version,
+                self._solution["chat_service_sid"],
                 self._solution["sid"],
             )
         return self._webhooks
 
     def __repr__(self) -> str:
         """
         Provide a friendly representation
@@ -531,345 +558,420 @@
 class ConversationPage(Page):
     def get_instance(self, payload: Dict[str, Any]) -> ConversationInstance:
         """
         Build an instance of ConversationInstance
 
         :param payload: Payload response from the API
         """
-        return ConversationInstance(self._version, payload)
+        return ConversationInstance(
+            self._version, payload, chat_service_sid=self._solution["chat_service_sid"]
+        )
 
     def __repr__(self) -> str:
         """
         Provide a friendly representation
 
         :returns: Machine friendly representation
         """
         return "<Twilio.Conversations.V1.ConversationPage>"
 
 
 class ConversationList(ListResource):
-    def __init__(self, version: Version):
+    def __init__(self, version: Version, chat_service_sid: str):
         """
         Initialize the ConversationList
 
         :param version: Version that contains the resource
+        :param chat_service_sid: The SID of the [Conversation Service](https://www.twilio.com/docs/conversations/api/service-resource) the Conversation resource is associated with.
 
         """
         super().__init__(version)
 
-        self._uri = "/Conversations"
+        # Path Solution
+        self._solution = {
+            "chat_service_sid": chat_service_sid,
+        }
+        self._uri = "/Services/{chat_service_sid}/Conversations".format(
+            **self._solution
+        )
 
     def create(
         self,
         x_twilio_webhook_enabled: Union[
             "ConversationInstance.WebhookEnabledType", object
         ] = values.unset,
         friendly_name: Union[str, object] = values.unset,
         unique_name: Union[str, object] = values.unset,
+        attributes: Union[str, object] = values.unset,
+        messaging_service_sid: Union[str, object] = values.unset,
         date_created: Union[datetime, object] = values.unset,
         date_updated: Union[datetime, object] = values.unset,
-        messaging_service_sid: Union[str, object] = values.unset,
-        attributes: Union[str, object] = values.unset,
         state: Union["ConversationInstance.State", object] = values.unset,
         timers_inactive: Union[str, object] = values.unset,
         timers_closed: Union[str, object] = values.unset,
     ) -> ConversationInstance:
         """
         Create the ConversationInstance
 
         :param x_twilio_webhook_enabled: The X-Twilio-Webhook-Enabled HTTP request header
         :param friendly_name: The human-readable name of this conversation, limited to 256 characters. Optional.
         :param unique_name: An application-defined string that uniquely identifies the resource. It can be used to address the resource in place of the resource's `sid` in the URL.
+        :param attributes: An optional string metadata field you can use to store any data you wish. The string value must contain structurally valid JSON if specified.  **Note** that if the attributes are not set \\\"{}\\\" will be returned.
+        :param messaging_service_sid: The unique ID of the [Messaging Service](https://www.twilio.com/docs/sms/services/api) this conversation belongs to.
         :param date_created: The date that this resource was created.
         :param date_updated: The date that this resource was last updated.
-        :param messaging_service_sid: The unique ID of the [Messaging Service](https://www.twilio.com/docs/sms/services/api) this conversation belongs to.
-        :param attributes: An optional string metadata field you can use to store any data you wish. The string value must contain structurally valid JSON if specified.  **Note** that if the attributes are not set \\\"{}\\\" will be returned.
         :param state:
         :param timers_inactive: ISO8601 duration when conversation will be switched to `inactive` state. Minimum value for this timer is 1 minute.
         :param timers_closed: ISO8601 duration when conversation will be switched to `closed` state. Minimum value for this timer is 10 minutes.
 
         :returns: The created ConversationInstance
         """
         data = values.of(
             {
                 "FriendlyName": friendly_name,
                 "UniqueName": unique_name,
+                "Attributes": attributes,
+                "MessagingServiceSid": messaging_service_sid,
                 "DateCreated": serialize.iso8601_datetime(date_created),
                 "DateUpdated": serialize.iso8601_datetime(date_updated),
-                "MessagingServiceSid": messaging_service_sid,
-                "Attributes": attributes,
                 "State": state,
                 "Timers.Inactive": timers_inactive,
                 "Timers.Closed": timers_closed,
             }
         )
         headers = values.of(
             {
                 "X-Twilio-Webhook-Enabled": x_twilio_webhook_enabled,
             }
         )
         payload = self._version.create(
             method="POST", uri=self._uri, data=data, headers=headers
         )
 
-        return ConversationInstance(self._version, payload)
+        return ConversationInstance(
+            self._version, payload, chat_service_sid=self._solution["chat_service_sid"]
+        )
 
     async def create_async(
         self,
         x_twilio_webhook_enabled: Union[
             "ConversationInstance.WebhookEnabledType", object
         ] = values.unset,
         friendly_name: Union[str, object] = values.unset,
         unique_name: Union[str, object] = values.unset,
+        attributes: Union[str, object] = values.unset,
+        messaging_service_sid: Union[str, object] = values.unset,
         date_created: Union[datetime, object] = values.unset,
         date_updated: Union[datetime, object] = values.unset,
-        messaging_service_sid: Union[str, object] = values.unset,
-        attributes: Union[str, object] = values.unset,
         state: Union["ConversationInstance.State", object] = values.unset,
         timers_inactive: Union[str, object] = values.unset,
         timers_closed: Union[str, object] = values.unset,
     ) -> ConversationInstance:
         """
         Asynchronously create the ConversationInstance
 
         :param x_twilio_webhook_enabled: The X-Twilio-Webhook-Enabled HTTP request header
         :param friendly_name: The human-readable name of this conversation, limited to 256 characters. Optional.
         :param unique_name: An application-defined string that uniquely identifies the resource. It can be used to address the resource in place of the resource's `sid` in the URL.
+        :param attributes: An optional string metadata field you can use to store any data you wish. The string value must contain structurally valid JSON if specified.  **Note** that if the attributes are not set \\\"{}\\\" will be returned.
+        :param messaging_service_sid: The unique ID of the [Messaging Service](https://www.twilio.com/docs/sms/services/api) this conversation belongs to.
         :param date_created: The date that this resource was created.
         :param date_updated: The date that this resource was last updated.
-        :param messaging_service_sid: The unique ID of the [Messaging Service](https://www.twilio.com/docs/sms/services/api) this conversation belongs to.
-        :param attributes: An optional string metadata field you can use to store any data you wish. The string value must contain structurally valid JSON if specified.  **Note** that if the attributes are not set \\\"{}\\\" will be returned.
         :param state:
         :param timers_inactive: ISO8601 duration when conversation will be switched to `inactive` state. Minimum value for this timer is 1 minute.
         :param timers_closed: ISO8601 duration when conversation will be switched to `closed` state. Minimum value for this timer is 10 minutes.
 
         :returns: The created ConversationInstance
         """
         data = values.of(
             {
                 "FriendlyName": friendly_name,
                 "UniqueName": unique_name,
+                "Attributes": attributes,
+                "MessagingServiceSid": messaging_service_sid,
                 "DateCreated": serialize.iso8601_datetime(date_created),
                 "DateUpdated": serialize.iso8601_datetime(date_updated),
-                "MessagingServiceSid": messaging_service_sid,
-                "Attributes": attributes,
                 "State": state,
                 "Timers.Inactive": timers_inactive,
                 "Timers.Closed": timers_closed,
             }
         )
         headers = values.of(
             {
                 "X-Twilio-Webhook-Enabled": x_twilio_webhook_enabled,
             }
         )
         payload = await self._version.create_async(
             method="POST", uri=self._uri, data=data, headers=headers
         )
 
-        return ConversationInstance(self._version, payload)
+        return ConversationInstance(
+            self._version, payload, chat_service_sid=self._solution["chat_service_sid"]
+        )
 
     def stream(
         self,
+        start_date: Union[str, object] = values.unset,
+        end_date: Union[str, object] = values.unset,
+        state: Union["ConversationInstance.State", object] = values.unset,
         limit: Optional[int] = None,
         page_size: Optional[int] = None,
     ) -> Iterator[ConversationInstance]:
         """
         Streams ConversationInstance records from the API as a generator stream.
         This operation lazily loads records as efficiently as possible until the limit
         is reached.
         The results are returned as a generator, so this operation is memory efficient.
 
+        :param str start_date: Start date or time in ISO8601 format for filtering list of Conversations. If a date is provided, the start time of the date is used (YYYY-MM-DDT00:00:00Z). Can be combined with other filters.
+        :param str end_date: End date or time in ISO8601 format for filtering list of Conversations. If a date is provided, the end time of the date is used (YYYY-MM-DDT23:59:59Z). Can be combined with other filters.
+        :param &quot;ConversationInstance.State&quot; state: State for sorting and filtering list of Conversations. Can be `active`, `inactive` or `closed`
         :param limit: Upper limit for the number of records to return. stream()
                       guarantees to never return more than limit.  Default is no limit
         :param page_size: Number of records to fetch per request, when not set will use
                           the default value of 50 records.  If no page_size is defined
                           but a limit is defined, stream() will attempt to read the
                           limit with the most efficient page size, i.e. min(limit, 1000)
 
         :returns: Generator that will yield up to limit results
         """
         limits = self._version.read_limits(limit, page_size)
-        page = self.page(page_size=limits["page_size"])
+        page = self.page(
+            start_date=start_date,
+            end_date=end_date,
+            state=state,
+            page_size=limits["page_size"],
+        )
 
         return self._version.stream(page, limits["limit"])
 
     async def stream_async(
         self,
+        start_date: Union[str, object] = values.unset,
+        end_date: Union[str, object] = values.unset,
+        state: Union["ConversationInstance.State", object] = values.unset,
         limit: Optional[int] = None,
         page_size: Optional[int] = None,
     ) -> AsyncIterator[ConversationInstance]:
         """
         Asynchronously streams ConversationInstance records from the API as a generator stream.
         This operation lazily loads records as efficiently as possible until the limit
         is reached.
         The results are returned as a generator, so this operation is memory efficient.
 
+        :param str start_date: Start date or time in ISO8601 format for filtering list of Conversations. If a date is provided, the start time of the date is used (YYYY-MM-DDT00:00:00Z). Can be combined with other filters.
+        :param str end_date: End date or time in ISO8601 format for filtering list of Conversations. If a date is provided, the end time of the date is used (YYYY-MM-DDT23:59:59Z). Can be combined with other filters.
+        :param &quot;ConversationInstance.State&quot; state: State for sorting and filtering list of Conversations. Can be `active`, `inactive` or `closed`
         :param limit: Upper limit for the number of records to return. stream()
                       guarantees to never return more than limit.  Default is no limit
         :param page_size: Number of records to fetch per request, when not set will use
                           the default value of 50 records.  If no page_size is defined
                           but a limit is defined, stream() will attempt to read the
                           limit with the most efficient page size, i.e. min(limit, 1000)
 
         :returns: Generator that will yield up to limit results
         """
         limits = self._version.read_limits(limit, page_size)
-        page = await self.page_async(page_size=limits["page_size"])
+        page = await self.page_async(
+            start_date=start_date,
+            end_date=end_date,
+            state=state,
+            page_size=limits["page_size"],
+        )
 
         return self._version.stream_async(page, limits["limit"])
 
     def list(
         self,
+        start_date: Union[str, object] = values.unset,
+        end_date: Union[str, object] = values.unset,
+        state: Union["ConversationInstance.State", object] = values.unset,
         limit: Optional[int] = None,
         page_size: Optional[int] = None,
     ) -> List[ConversationInstance]:
         """
         Lists ConversationInstance records from the API as a list.
         Unlike stream(), this operation is eager and will load `limit` records into
         memory before returning.
 
+        :param str start_date: Start date or time in ISO8601 format for filtering list of Conversations. If a date is provided, the start time of the date is used (YYYY-MM-DDT00:00:00Z). Can be combined with other filters.
+        :param str end_date: End date or time in ISO8601 format for filtering list of Conversations. If a date is provided, the end time of the date is used (YYYY-MM-DDT23:59:59Z). Can be combined with other filters.
+        :param &quot;ConversationInstance.State&quot; state: State for sorting and filtering list of Conversations. Can be `active`, `inactive` or `closed`
         :param limit: Upper limit for the number of records to return. list() guarantees
                       never to return more than limit.  Default is no limit
         :param page_size: Number of records to fetch per request, when not set will use
                           the default value of 50 records.  If no page_size is defined
                           but a limit is defined, list() will attempt to read the limit
                           with the most efficient page size, i.e. min(limit, 1000)
 
         :returns: list that will contain up to limit results
         """
         return list(
             self.stream(
+                start_date=start_date,
+                end_date=end_date,
+                state=state,
                 limit=limit,
                 page_size=page_size,
             )
         )
 
     async def list_async(
         self,
+        start_date: Union[str, object] = values.unset,
+        end_date: Union[str, object] = values.unset,
+        state: Union["ConversationInstance.State", object] = values.unset,
         limit: Optional[int] = None,
         page_size: Optional[int] = None,
     ) -> List[ConversationInstance]:
         """
         Asynchronously lists ConversationInstance records from the API as a list.
         Unlike stream(), this operation is eager and will load `limit` records into
         memory before returning.
 
+        :param str start_date: Start date or time in ISO8601 format for filtering list of Conversations. If a date is provided, the start time of the date is used (YYYY-MM-DDT00:00:00Z). Can be combined with other filters.
+        :param str end_date: End date or time in ISO8601 format for filtering list of Conversations. If a date is provided, the end time of the date is used (YYYY-MM-DDT23:59:59Z). Can be combined with other filters.
+        :param &quot;ConversationInstance.State&quot; state: State for sorting and filtering list of Conversations. Can be `active`, `inactive` or `closed`
         :param limit: Upper limit for the number of records to return. list() guarantees
                       never to return more than limit.  Default is no limit
         :param page_size: Number of records to fetch per request, when not set will use
                           the default value of 50 records.  If no page_size is defined
                           but a limit is defined, list() will attempt to read the limit
                           with the most efficient page size, i.e. min(limit, 1000)
 
         :returns: list that will contain up to limit results
         """
         return [
             record
             async for record in await self.stream_async(
+                start_date=start_date,
+                end_date=end_date,
+                state=state,
                 limit=limit,
                 page_size=page_size,
             )
         ]
 
     def page(
         self,
+        start_date: Union[str, object] = values.unset,
+        end_date: Union[str, object] = values.unset,
+        state: Union["ConversationInstance.State", object] = values.unset,
         page_token: Union[str, object] = values.unset,
         page_number: Union[int, object] = values.unset,
         page_size: Union[int, object] = values.unset,
     ) -> ConversationPage:
         """
         Retrieve a single page of ConversationInstance records from the API.
         Request is executed immediately
 
+        :param start_date: Start date or time in ISO8601 format for filtering list of Conversations. If a date is provided, the start time of the date is used (YYYY-MM-DDT00:00:00Z). Can be combined with other filters.
+        :param end_date: End date or time in ISO8601 format for filtering list of Conversations. If a date is provided, the end time of the date is used (YYYY-MM-DDT23:59:59Z). Can be combined with other filters.
+        :param state: State for sorting and filtering list of Conversations. Can be `active`, `inactive` or `closed`
         :param page_token: PageToken provided by the API
         :param page_number: Page Number, this value is simply for client state
         :param page_size: Number of records to return, defaults to 50
 
         :returns: Page of ConversationInstance
         """
         data = values.of(
             {
+                "StartDate": start_date,
+                "EndDate": end_date,
+                "State": state,
                 "PageToken": page_token,
                 "Page": page_number,
                 "PageSize": page_size,
             }
         )
 
         response = self._version.page(method="GET", uri=self._uri, params=data)
-        return ConversationPage(self._version, response)
+        return ConversationPage(self._version, response, self._solution)
 
     async def page_async(
         self,
+        start_date: Union[str, object] = values.unset,
+        end_date: Union[str, object] = values.unset,
+        state: Union["ConversationInstance.State", object] = values.unset,
         page_token: Union[str, object] = values.unset,
         page_number: Union[int, object] = values.unset,
         page_size: Union[int, object] = values.unset,
     ) -> ConversationPage:
         """
         Asynchronously retrieve a single page of ConversationInstance records from the API.
         Request is executed immediately
 
+        :param start_date: Start date or time in ISO8601 format for filtering list of Conversations. If a date is provided, the start time of the date is used (YYYY-MM-DDT00:00:00Z). Can be combined with other filters.
+        :param end_date: End date or time in ISO8601 format for filtering list of Conversations. If a date is provided, the end time of the date is used (YYYY-MM-DDT23:59:59Z). Can be combined with other filters.
+        :param state: State for sorting and filtering list of Conversations. Can be `active`, `inactive` or `closed`
         :param page_token: PageToken provided by the API
         :param page_number: Page Number, this value is simply for client state
         :param page_size: Number of records to return, defaults to 50
 
         :returns: Page of ConversationInstance
         """
         data = values.of(
             {
+                "StartDate": start_date,
+                "EndDate": end_date,
+                "State": state,
                 "PageToken": page_token,
                 "Page": page_number,
                 "PageSize": page_size,
             }
         )
 
         response = await self._version.page_async(
             method="GET", uri=self._uri, params=data
         )
-        return ConversationPage(self._version, response)
+        return ConversationPage(self._version, response, self._solution)
 
     def get_page(self, target_url: str) -> ConversationPage:
         """
         Retrieve a specific page of ConversationInstance records from the API.
         Request is executed immediately
 
         :param target_url: API-generated URL for the requested results page
 
         :returns: Page of ConversationInstance
         """
         response = self._version.domain.twilio.request("GET", target_url)
-        return ConversationPage(self._version, response)
+        return ConversationPage(self._version, response, self._solution)
 
     async def get_page_async(self, target_url: str) -> ConversationPage:
         """
         Asynchronously retrieve a specific page of ConversationInstance records from the API.
         Request is executed immediately
 
         :param target_url: API-generated URL for the requested results page
 
         :returns: Page of ConversationInstance
         """
         response = await self._version.domain.twilio.request_async("GET", target_url)
-        return ConversationPage(self._version, response)
+        return ConversationPage(self._version, response, self._solution)
 
     def get(self, sid: str) -> ConversationContext:
         """
         Constructs a ConversationContext
 
         :param sid: A 34 character string that uniquely identifies this resource. Can also be the `unique_name` of the Conversation.
         """
-        return ConversationContext(self._version, sid=sid)
+        return ConversationContext(
+            self._version, chat_service_sid=self._solution["chat_service_sid"], sid=sid
+        )
 
     def __call__(self, sid: str) -> ConversationContext:
         """
         Constructs a ConversationContext
 
         :param sid: A 34 character string that uniquely identifies this resource. Can also be the `unique_name` of the Conversation.
         """
-        return ConversationContext(self._version, sid=sid)
+        return ConversationContext(
+            self._version, chat_service_sid=self._solution["chat_service_sid"], sid=sid
+        )
 
     def __repr__(self) -> str:
         """
         Provide a friendly representation
 
         :returns: Machine friendly representation
         """
```

### Comparing `twilio-8.2.0/twilio/rest/conversations/v1/conversation/message/__init__.py` & `twilio-8.2.1/twilio/rest/conversations/v1/conversation/message/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/conversations/v1/conversation/message/delivery_receipt.py` & `twilio-8.2.1/twilio/rest/conversations/v1/conversation/message/delivery_receipt.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/conversations/v1/conversation/participant.py` & `twilio-8.2.1/twilio/rest/conversations/v1/conversation/participant.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/conversations/v1/conversation/webhook.py` & `twilio-8.2.1/twilio/rest/conversations/v1/conversation/webhook.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/conversations/v1/credential.py` & `twilio-8.2.1/twilio/rest/conversations/v1/credential.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/conversations/v1/participant_conversation.py` & `twilio-8.2.1/twilio/rest/conversations/v1/participant_conversation.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/conversations/v1/role.py` & `twilio-8.2.1/twilio/rest/conversations/v1/role.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/conversations/v1/service/__init__.py` & `twilio-8.2.1/twilio/rest/conversations/v1/service/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/conversations/v1/service/binding.py` & `twilio-8.2.1/twilio/rest/conversations/v1/service/binding.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/conversations/v1/service/configuration/__init__.py` & `twilio-8.2.1/twilio/rest/conversations/v1/service/configuration/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/conversations/v1/service/configuration/notification.py` & `twilio-8.2.1/twilio/rest/conversations/v1/service/configuration/notification.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/conversations/v1/service/configuration/webhook.py` & `twilio-8.2.1/twilio/rest/conversations/v1/service/configuration/webhook.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/conversations/v1/service/conversation/__init__.py` & `twilio-8.2.1/twilio/rest/conversations/v1/conversation/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -17,19 +17,17 @@
 from typing import Any, Dict, List, Optional, Union, Iterator, AsyncIterator
 from twilio.base import deserialize, serialize, values
 from twilio.base.instance_context import InstanceContext
 from twilio.base.instance_resource import InstanceResource
 from twilio.base.list_resource import ListResource
 from twilio.base.version import Version
 from twilio.base.page import Page
-from twilio.rest.conversations.v1.service.conversation.message import MessageList
-from twilio.rest.conversations.v1.service.conversation.participant import (
-    ParticipantList,
-)
-from twilio.rest.conversations.v1.service.conversation.webhook import WebhookList
+from twilio.rest.conversations.v1.conversation.message import MessageList
+from twilio.rest.conversations.v1.conversation.participant import ParticipantList
+from twilio.rest.conversations.v1.conversation.webhook import WebhookList
 
 
 class ConversationInstance(InstanceResource):
     class State(object):
         INACTIVE = "inactive"
         ACTIVE = "active"
         CLOSED = "closed"
@@ -52,19 +50,15 @@
     :ivar timers: Timer date values representing state update for this conversation.
     :ivar url: An absolute API resource URL for this conversation.
     :ivar links: Contains absolute URLs to access the [participants](https://www.twilio.com/docs/conversations/api/conversation-participant-resource), [messages](https://www.twilio.com/docs/conversations/api/conversation-message-resource) and [webhooks](https://www.twilio.com/docs/conversations/api/conversation-scoped-webhook-resource) of this conversation.
     :ivar bindings: 
     """
 
     def __init__(
-        self,
-        version: Version,
-        payload: Dict[str, Any],
-        chat_service_sid: str,
-        sid: Optional[str] = None,
+        self, version: Version, payload: Dict[str, Any], sid: Optional[str] = None
     ):
         super().__init__(version)
 
         self.account_sid: Optional[str] = payload.get("account_sid")
         self.chat_service_sid: Optional[str] = payload.get("chat_service_sid")
         self.messaging_service_sid: Optional[str] = payload.get("messaging_service_sid")
         self.sid: Optional[str] = payload.get("sid")
@@ -80,15 +74,14 @@
         )
         self.timers: Optional[Dict[str, object]] = payload.get("timers")
         self.url: Optional[str] = payload.get("url")
         self.links: Optional[Dict[str, object]] = payload.get("links")
         self.bindings: Optional[Dict[str, object]] = payload.get("bindings")
 
         self._solution = {
-            "chat_service_sid": chat_service_sid,
             "sid": sid or self.sid,
         }
         self._context: Optional[ConversationContext] = None
 
     @property
     def _proxy(self) -> "ConversationContext":
         """
@@ -96,15 +89,14 @@
         performing various actions. All instance actions are proxied to the context
 
         :returns: ConversationContext for this ConversationInstance
         """
         if self._context is None:
             self._context = ConversationContext(
                 self._version,
-                chat_service_sid=self._solution["chat_service_sid"],
                 sid=self._solution["sid"],
             )
         return self._context
 
     def delete(
         self,
         x_twilio_webhook_enabled: Union[
@@ -273,32 +265,28 @@
         :returns: Machine friendly representation
         """
         context = " ".join("{}={}".format(k, v) for k, v in self._solution.items())
         return "<Twilio.Conversations.V1.ConversationInstance {}>".format(context)
 
 
 class ConversationContext(InstanceContext):
-    def __init__(self, version: Version, chat_service_sid: str, sid: str):
+    def __init__(self, version: Version, sid: str):
         """
         Initialize the ConversationContext
 
         :param version: Version that contains the resource
-        :param chat_service_sid: The SID of the [Conversation Service](https://www.twilio.com/docs/conversations/api/service-resource) the Conversation resource is associated with.
         :param sid: A 34 character string that uniquely identifies this resource. Can also be the `unique_name` of the Conversation.
         """
         super().__init__(version)
 
         # Path Solution
         self._solution = {
-            "chat_service_sid": chat_service_sid,
             "sid": sid,
         }
-        self._uri = "/Services/{chat_service_sid}/Conversations/{sid}".format(
-            **self._solution
-        )
+        self._uri = "/Conversations/{sid}".format(**self._solution)
 
         self._messages: Optional[MessageList] = None
         self._participants: Optional[ParticipantList] = None
         self._webhooks: Optional[WebhookList] = None
 
     def delete(
         self,
@@ -356,15 +344,14 @@
             method="GET",
             uri=self._uri,
         )
 
         return ConversationInstance(
             self._version,
             payload,
-            chat_service_sid=self._solution["chat_service_sid"],
             sid=self._solution["sid"],
         )
 
     async def fetch_async(self) -> ConversationInstance:
         """
         Asynchronous coroutine to fetch the ConversationInstance
 
@@ -376,15 +363,14 @@
             method="GET",
             uri=self._uri,
         )
 
         return ConversationInstance(
             self._version,
             payload,
-            chat_service_sid=self._solution["chat_service_sid"],
             sid=self._solution["sid"],
         )
 
     def update(
         self,
         x_twilio_webhook_enabled: Union[
             "ConversationInstance.WebhookEnabledType", object
@@ -434,20 +420,15 @@
             }
         )
 
         payload = self._version.update(
             method="POST", uri=self._uri, data=data, headers=headers
         )
 
-        return ConversationInstance(
-            self._version,
-            payload,
-            chat_service_sid=self._solution["chat_service_sid"],
-            sid=self._solution["sid"],
-        )
+        return ConversationInstance(self._version, payload, sid=self._solution["sid"])
 
     async def update_async(
         self,
         x_twilio_webhook_enabled: Union[
             "ConversationInstance.WebhookEnabledType", object
         ] = values.unset,
         friendly_name: Union[str, object] = values.unset,
@@ -495,56 +476,48 @@
             }
         )
 
         payload = await self._version.update_async(
             method="POST", uri=self._uri, data=data, headers=headers
         )
 
-        return ConversationInstance(
-            self._version,
-            payload,
-            chat_service_sid=self._solution["chat_service_sid"],
-            sid=self._solution["sid"],
-        )
+        return ConversationInstance(self._version, payload, sid=self._solution["sid"])
 
     @property
     def messages(self) -> MessageList:
         """
         Access the messages
         """
         if self._messages is None:
             self._messages = MessageList(
                 self._version,
-                self._solution["chat_service_sid"],
                 self._solution["sid"],
             )
         return self._messages
 
     @property
     def participants(self) -> ParticipantList:
         """
         Access the participants
         """
         if self._participants is None:
             self._participants = ParticipantList(
                 self._version,
-                self._solution["chat_service_sid"],
                 self._solution["sid"],
             )
         return self._participants
 
     @property
     def webhooks(self) -> WebhookList:
         """
         Access the webhooks
         """
         if self._webhooks is None:
             self._webhooks = WebhookList(
                 self._version,
-                self._solution["chat_service_sid"],
                 self._solution["sid"],
             )
         return self._webhooks
 
     def __repr__(self) -> str:
         """
         Provide a friendly representation
@@ -558,362 +531,403 @@
 class ConversationPage(Page):
     def get_instance(self, payload: Dict[str, Any]) -> ConversationInstance:
         """
         Build an instance of ConversationInstance
 
         :param payload: Payload response from the API
         """
-        return ConversationInstance(
-            self._version, payload, chat_service_sid=self._solution["chat_service_sid"]
-        )
+        return ConversationInstance(self._version, payload)
 
     def __repr__(self) -> str:
         """
         Provide a friendly representation
 
         :returns: Machine friendly representation
         """
         return "<Twilio.Conversations.V1.ConversationPage>"
 
 
 class ConversationList(ListResource):
-    def __init__(self, version: Version, chat_service_sid: str):
+    def __init__(self, version: Version):
         """
         Initialize the ConversationList
 
         :param version: Version that contains the resource
-        :param chat_service_sid: The SID of the [Conversation Service](https://www.twilio.com/docs/conversations/api/service-resource) the Conversation resource is associated with.
 
         """
         super().__init__(version)
 
-        # Path Solution
-        self._solution = {
-            "chat_service_sid": chat_service_sid,
-        }
-        self._uri = "/Services/{chat_service_sid}/Conversations".format(
-            **self._solution
-        )
+        self._uri = "/Conversations"
 
     def create(
         self,
         x_twilio_webhook_enabled: Union[
             "ConversationInstance.WebhookEnabledType", object
         ] = values.unset,
         friendly_name: Union[str, object] = values.unset,
         unique_name: Union[str, object] = values.unset,
-        attributes: Union[str, object] = values.unset,
-        messaging_service_sid: Union[str, object] = values.unset,
         date_created: Union[datetime, object] = values.unset,
         date_updated: Union[datetime, object] = values.unset,
+        messaging_service_sid: Union[str, object] = values.unset,
+        attributes: Union[str, object] = values.unset,
         state: Union["ConversationInstance.State", object] = values.unset,
         timers_inactive: Union[str, object] = values.unset,
         timers_closed: Union[str, object] = values.unset,
     ) -> ConversationInstance:
         """
         Create the ConversationInstance
 
         :param x_twilio_webhook_enabled: The X-Twilio-Webhook-Enabled HTTP request header
         :param friendly_name: The human-readable name of this conversation, limited to 256 characters. Optional.
         :param unique_name: An application-defined string that uniquely identifies the resource. It can be used to address the resource in place of the resource's `sid` in the URL.
-        :param attributes: An optional string metadata field you can use to store any data you wish. The string value must contain structurally valid JSON if specified.  **Note** that if the attributes are not set \\\"{}\\\" will be returned.
-        :param messaging_service_sid: The unique ID of the [Messaging Service](https://www.twilio.com/docs/sms/services/api) this conversation belongs to.
         :param date_created: The date that this resource was created.
         :param date_updated: The date that this resource was last updated.
+        :param messaging_service_sid: The unique ID of the [Messaging Service](https://www.twilio.com/docs/sms/services/api) this conversation belongs to.
+        :param attributes: An optional string metadata field you can use to store any data you wish. The string value must contain structurally valid JSON if specified.  **Note** that if the attributes are not set \\\"{}\\\" will be returned.
         :param state:
         :param timers_inactive: ISO8601 duration when conversation will be switched to `inactive` state. Minimum value for this timer is 1 minute.
         :param timers_closed: ISO8601 duration when conversation will be switched to `closed` state. Minimum value for this timer is 10 minutes.
 
         :returns: The created ConversationInstance
         """
         data = values.of(
             {
                 "FriendlyName": friendly_name,
                 "UniqueName": unique_name,
-                "Attributes": attributes,
-                "MessagingServiceSid": messaging_service_sid,
                 "DateCreated": serialize.iso8601_datetime(date_created),
                 "DateUpdated": serialize.iso8601_datetime(date_updated),
+                "MessagingServiceSid": messaging_service_sid,
+                "Attributes": attributes,
                 "State": state,
                 "Timers.Inactive": timers_inactive,
                 "Timers.Closed": timers_closed,
             }
         )
         headers = values.of(
             {
                 "X-Twilio-Webhook-Enabled": x_twilio_webhook_enabled,
             }
         )
         payload = self._version.create(
             method="POST", uri=self._uri, data=data, headers=headers
         )
 
-        return ConversationInstance(
-            self._version, payload, chat_service_sid=self._solution["chat_service_sid"]
-        )
+        return ConversationInstance(self._version, payload)
 
     async def create_async(
         self,
         x_twilio_webhook_enabled: Union[
             "ConversationInstance.WebhookEnabledType", object
         ] = values.unset,
         friendly_name: Union[str, object] = values.unset,
         unique_name: Union[str, object] = values.unset,
-        attributes: Union[str, object] = values.unset,
-        messaging_service_sid: Union[str, object] = values.unset,
         date_created: Union[datetime, object] = values.unset,
         date_updated: Union[datetime, object] = values.unset,
+        messaging_service_sid: Union[str, object] = values.unset,
+        attributes: Union[str, object] = values.unset,
         state: Union["ConversationInstance.State", object] = values.unset,
         timers_inactive: Union[str, object] = values.unset,
         timers_closed: Union[str, object] = values.unset,
     ) -> ConversationInstance:
         """
         Asynchronously create the ConversationInstance
 
         :param x_twilio_webhook_enabled: The X-Twilio-Webhook-Enabled HTTP request header
         :param friendly_name: The human-readable name of this conversation, limited to 256 characters. Optional.
         :param unique_name: An application-defined string that uniquely identifies the resource. It can be used to address the resource in place of the resource's `sid` in the URL.
-        :param attributes: An optional string metadata field you can use to store any data you wish. The string value must contain structurally valid JSON if specified.  **Note** that if the attributes are not set \\\"{}\\\" will be returned.
-        :param messaging_service_sid: The unique ID of the [Messaging Service](https://www.twilio.com/docs/sms/services/api) this conversation belongs to.
         :param date_created: The date that this resource was created.
         :param date_updated: The date that this resource was last updated.
+        :param messaging_service_sid: The unique ID of the [Messaging Service](https://www.twilio.com/docs/sms/services/api) this conversation belongs to.
+        :param attributes: An optional string metadata field you can use to store any data you wish. The string value must contain structurally valid JSON if specified.  **Note** that if the attributes are not set \\\"{}\\\" will be returned.
         :param state:
         :param timers_inactive: ISO8601 duration when conversation will be switched to `inactive` state. Minimum value for this timer is 1 minute.
         :param timers_closed: ISO8601 duration when conversation will be switched to `closed` state. Minimum value for this timer is 10 minutes.
 
         :returns: The created ConversationInstance
         """
         data = values.of(
             {
                 "FriendlyName": friendly_name,
                 "UniqueName": unique_name,
-                "Attributes": attributes,
-                "MessagingServiceSid": messaging_service_sid,
                 "DateCreated": serialize.iso8601_datetime(date_created),
                 "DateUpdated": serialize.iso8601_datetime(date_updated),
+                "MessagingServiceSid": messaging_service_sid,
+                "Attributes": attributes,
                 "State": state,
                 "Timers.Inactive": timers_inactive,
                 "Timers.Closed": timers_closed,
             }
         )
         headers = values.of(
             {
                 "X-Twilio-Webhook-Enabled": x_twilio_webhook_enabled,
             }
         )
         payload = await self._version.create_async(
             method="POST", uri=self._uri, data=data, headers=headers
         )
 
-        return ConversationInstance(
-            self._version, payload, chat_service_sid=self._solution["chat_service_sid"]
-        )
+        return ConversationInstance(self._version, payload)
 
     def stream(
         self,
+        start_date: Union[str, object] = values.unset,
+        end_date: Union[str, object] = values.unset,
+        state: Union["ConversationInstance.State", object] = values.unset,
         limit: Optional[int] = None,
         page_size: Optional[int] = None,
     ) -> Iterator[ConversationInstance]:
         """
         Streams ConversationInstance records from the API as a generator stream.
         This operation lazily loads records as efficiently as possible until the limit
         is reached.
         The results are returned as a generator, so this operation is memory efficient.
 
+        :param str start_date: Start date or time in ISO8601 format for filtering list of Conversations. If a date is provided, the start time of the date is used (YYYY-MM-DDT00:00:00Z). Can be combined with other filters.
+        :param str end_date: End date or time in ISO8601 format for filtering list of Conversations. If a date is provided, the end time of the date is used (YYYY-MM-DDT23:59:59Z). Can be combined with other filters.
+        :param &quot;ConversationInstance.State&quot; state: State for sorting and filtering list of Conversations. Can be `active`, `inactive` or `closed`
         :param limit: Upper limit for the number of records to return. stream()
                       guarantees to never return more than limit.  Default is no limit
         :param page_size: Number of records to fetch per request, when not set will use
                           the default value of 50 records.  If no page_size is defined
                           but a limit is defined, stream() will attempt to read the
                           limit with the most efficient page size, i.e. min(limit, 1000)
 
         :returns: Generator that will yield up to limit results
         """
         limits = self._version.read_limits(limit, page_size)
-        page = self.page(page_size=limits["page_size"])
+        page = self.page(
+            start_date=start_date,
+            end_date=end_date,
+            state=state,
+            page_size=limits["page_size"],
+        )
 
         return self._version.stream(page, limits["limit"])
 
     async def stream_async(
         self,
+        start_date: Union[str, object] = values.unset,
+        end_date: Union[str, object] = values.unset,
+        state: Union["ConversationInstance.State", object] = values.unset,
         limit: Optional[int] = None,
         page_size: Optional[int] = None,
     ) -> AsyncIterator[ConversationInstance]:
         """
         Asynchronously streams ConversationInstance records from the API as a generator stream.
         This operation lazily loads records as efficiently as possible until the limit
         is reached.
         The results are returned as a generator, so this operation is memory efficient.
 
+        :param str start_date: Start date or time in ISO8601 format for filtering list of Conversations. If a date is provided, the start time of the date is used (YYYY-MM-DDT00:00:00Z). Can be combined with other filters.
+        :param str end_date: End date or time in ISO8601 format for filtering list of Conversations. If a date is provided, the end time of the date is used (YYYY-MM-DDT23:59:59Z). Can be combined with other filters.
+        :param &quot;ConversationInstance.State&quot; state: State for sorting and filtering list of Conversations. Can be `active`, `inactive` or `closed`
         :param limit: Upper limit for the number of records to return. stream()
                       guarantees to never return more than limit.  Default is no limit
         :param page_size: Number of records to fetch per request, when not set will use
                           the default value of 50 records.  If no page_size is defined
                           but a limit is defined, stream() will attempt to read the
                           limit with the most efficient page size, i.e. min(limit, 1000)
 
         :returns: Generator that will yield up to limit results
         """
         limits = self._version.read_limits(limit, page_size)
-        page = await self.page_async(page_size=limits["page_size"])
+        page = await self.page_async(
+            start_date=start_date,
+            end_date=end_date,
+            state=state,
+            page_size=limits["page_size"],
+        )
 
         return self._version.stream_async(page, limits["limit"])
 
     def list(
         self,
+        start_date: Union[str, object] = values.unset,
+        end_date: Union[str, object] = values.unset,
+        state: Union["ConversationInstance.State", object] = values.unset,
         limit: Optional[int] = None,
         page_size: Optional[int] = None,
     ) -> List[ConversationInstance]:
         """
         Lists ConversationInstance records from the API as a list.
         Unlike stream(), this operation is eager and will load `limit` records into
         memory before returning.
 
+        :param str start_date: Start date or time in ISO8601 format for filtering list of Conversations. If a date is provided, the start time of the date is used (YYYY-MM-DDT00:00:00Z). Can be combined with other filters.
+        :param str end_date: End date or time in ISO8601 format for filtering list of Conversations. If a date is provided, the end time of the date is used (YYYY-MM-DDT23:59:59Z). Can be combined with other filters.
+        :param &quot;ConversationInstance.State&quot; state: State for sorting and filtering list of Conversations. Can be `active`, `inactive` or `closed`
         :param limit: Upper limit for the number of records to return. list() guarantees
                       never to return more than limit.  Default is no limit
         :param page_size: Number of records to fetch per request, when not set will use
                           the default value of 50 records.  If no page_size is defined
                           but a limit is defined, list() will attempt to read the limit
                           with the most efficient page size, i.e. min(limit, 1000)
 
         :returns: list that will contain up to limit results
         """
         return list(
             self.stream(
+                start_date=start_date,
+                end_date=end_date,
+                state=state,
                 limit=limit,
                 page_size=page_size,
             )
         )
 
     async def list_async(
         self,
+        start_date: Union[str, object] = values.unset,
+        end_date: Union[str, object] = values.unset,
+        state: Union["ConversationInstance.State", object] = values.unset,
         limit: Optional[int] = None,
         page_size: Optional[int] = None,
     ) -> List[ConversationInstance]:
         """
         Asynchronously lists ConversationInstance records from the API as a list.
         Unlike stream(), this operation is eager and will load `limit` records into
         memory before returning.
 
+        :param str start_date: Start date or time in ISO8601 format for filtering list of Conversations. If a date is provided, the start time of the date is used (YYYY-MM-DDT00:00:00Z). Can be combined with other filters.
+        :param str end_date: End date or time in ISO8601 format for filtering list of Conversations. If a date is provided, the end time of the date is used (YYYY-MM-DDT23:59:59Z). Can be combined with other filters.
+        :param &quot;ConversationInstance.State&quot; state: State for sorting and filtering list of Conversations. Can be `active`, `inactive` or `closed`
         :param limit: Upper limit for the number of records to return. list() guarantees
                       never to return more than limit.  Default is no limit
         :param page_size: Number of records to fetch per request, when not set will use
                           the default value of 50 records.  If no page_size is defined
                           but a limit is defined, list() will attempt to read the limit
                           with the most efficient page size, i.e. min(limit, 1000)
 
         :returns: list that will contain up to limit results
         """
         return [
             record
             async for record in await self.stream_async(
+                start_date=start_date,
+                end_date=end_date,
+                state=state,
                 limit=limit,
                 page_size=page_size,
             )
         ]
 
     def page(
         self,
+        start_date: Union[str, object] = values.unset,
+        end_date: Union[str, object] = values.unset,
+        state: Union["ConversationInstance.State", object] = values.unset,
         page_token: Union[str, object] = values.unset,
         page_number: Union[int, object] = values.unset,
         page_size: Union[int, object] = values.unset,
     ) -> ConversationPage:
         """
         Retrieve a single page of ConversationInstance records from the API.
         Request is executed immediately
 
+        :param start_date: Start date or time in ISO8601 format for filtering list of Conversations. If a date is provided, the start time of the date is used (YYYY-MM-DDT00:00:00Z). Can be combined with other filters.
+        :param end_date: End date or time in ISO8601 format for filtering list of Conversations. If a date is provided, the end time of the date is used (YYYY-MM-DDT23:59:59Z). Can be combined with other filters.
+        :param state: State for sorting and filtering list of Conversations. Can be `active`, `inactive` or `closed`
         :param page_token: PageToken provided by the API
         :param page_number: Page Number, this value is simply for client state
         :param page_size: Number of records to return, defaults to 50
 
         :returns: Page of ConversationInstance
         """
         data = values.of(
             {
+                "StartDate": start_date,
+                "EndDate": end_date,
+                "State": state,
                 "PageToken": page_token,
                 "Page": page_number,
                 "PageSize": page_size,
             }
         )
 
         response = self._version.page(method="GET", uri=self._uri, params=data)
-        return ConversationPage(self._version, response, self._solution)
+        return ConversationPage(self._version, response)
 
     async def page_async(
         self,
+        start_date: Union[str, object] = values.unset,
+        end_date: Union[str, object] = values.unset,
+        state: Union["ConversationInstance.State", object] = values.unset,
         page_token: Union[str, object] = values.unset,
         page_number: Union[int, object] = values.unset,
         page_size: Union[int, object] = values.unset,
     ) -> ConversationPage:
         """
         Asynchronously retrieve a single page of ConversationInstance records from the API.
         Request is executed immediately
 
+        :param start_date: Start date or time in ISO8601 format for filtering list of Conversations. If a date is provided, the start time of the date is used (YYYY-MM-DDT00:00:00Z). Can be combined with other filters.
+        :param end_date: End date or time in ISO8601 format for filtering list of Conversations. If a date is provided, the end time of the date is used (YYYY-MM-DDT23:59:59Z). Can be combined with other filters.
+        :param state: State for sorting and filtering list of Conversations. Can be `active`, `inactive` or `closed`
         :param page_token: PageToken provided by the API
         :param page_number: Page Number, this value is simply for client state
         :param page_size: Number of records to return, defaults to 50
 
         :returns: Page of ConversationInstance
         """
         data = values.of(
             {
+                "StartDate": start_date,
+                "EndDate": end_date,
+                "State": state,
                 "PageToken": page_token,
                 "Page": page_number,
                 "PageSize": page_size,
             }
         )
 
         response = await self._version.page_async(
             method="GET", uri=self._uri, params=data
         )
-        return ConversationPage(self._version, response, self._solution)
+        return ConversationPage(self._version, response)
 
     def get_page(self, target_url: str) -> ConversationPage:
         """
         Retrieve a specific page of ConversationInstance records from the API.
         Request is executed immediately
 
         :param target_url: API-generated URL for the requested results page
 
         :returns: Page of ConversationInstance
         """
         response = self._version.domain.twilio.request("GET", target_url)
-        return ConversationPage(self._version, response, self._solution)
+        return ConversationPage(self._version, response)
 
     async def get_page_async(self, target_url: str) -> ConversationPage:
         """
         Asynchronously retrieve a specific page of ConversationInstance records from the API.
         Request is executed immediately
 
         :param target_url: API-generated URL for the requested results page
 
         :returns: Page of ConversationInstance
         """
         response = await self._version.domain.twilio.request_async("GET", target_url)
-        return ConversationPage(self._version, response, self._solution)
+        return ConversationPage(self._version, response)
 
     def get(self, sid: str) -> ConversationContext:
         """
         Constructs a ConversationContext
 
         :param sid: A 34 character string that uniquely identifies this resource. Can also be the `unique_name` of the Conversation.
         """
-        return ConversationContext(
-            self._version, chat_service_sid=self._solution["chat_service_sid"], sid=sid
-        )
+        return ConversationContext(self._version, sid=sid)
 
     def __call__(self, sid: str) -> ConversationContext:
         """
         Constructs a ConversationContext
 
         :param sid: A 34 character string that uniquely identifies this resource. Can also be the `unique_name` of the Conversation.
         """
-        return ConversationContext(
-            self._version, chat_service_sid=self._solution["chat_service_sid"], sid=sid
-        )
+        return ConversationContext(self._version, sid=sid)
 
     def __repr__(self) -> str:
         """
         Provide a friendly representation
 
         :returns: Machine friendly representation
         """
```

### Comparing `twilio-8.2.0/twilio/rest/conversations/v1/service/conversation/message/__init__.py` & `twilio-8.2.1/twilio/rest/conversations/v1/service/conversation/message/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/conversations/v1/service/conversation/message/delivery_receipt.py` & `twilio-8.2.1/twilio/rest/conversations/v1/service/conversation/message/delivery_receipt.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/conversations/v1/service/conversation/participant.py` & `twilio-8.2.1/twilio/rest/conversations/v1/service/conversation/participant.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/conversations/v1/service/conversation/webhook.py` & `twilio-8.2.1/twilio/rest/conversations/v1/service/conversation/webhook.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/conversations/v1/service/participant_conversation.py` & `twilio-8.2.1/twilio/rest/conversations/v1/service/participant_conversation.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/conversations/v1/service/role.py` & `twilio-8.2.1/twilio/rest/conversations/v1/service/role.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/conversations/v1/service/user/__init__.py` & `twilio-8.2.1/twilio/rest/conversations/v1/service/user/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/conversations/v1/service/user/user_conversation.py` & `twilio-8.2.1/twilio/rest/conversations/v1/service/user/user_conversation.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/conversations/v1/user/__init__.py` & `twilio-8.2.1/twilio/rest/conversations/v1/user/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/conversations/v1/user/user_conversation.py` & `twilio-8.2.1/twilio/rest/conversations/v1/user/user_conversation.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/events/EventsBase.py` & `twilio-8.2.1/twilio/rest/events/EventsBase.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/events/__init__.py` & `twilio-8.2.1/twilio/rest/events/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/events/v1/__init__.py` & `twilio-8.2.1/twilio/rest/events/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/events/v1/event_type.py` & `twilio-8.2.1/twilio/rest/events/v1/event_type.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/events/v1/schema/__init__.py` & `twilio-8.2.1/twilio/rest/events/v1/schema/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/events/v1/schema/schema_version.py` & `twilio-8.2.1/twilio/rest/events/v1/schema/schema_version.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/events/v1/sink/__init__.py` & `twilio-8.2.1/twilio/rest/events/v1/sink/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/events/v1/sink/sink_test.py` & `twilio-8.2.1/twilio/rest/events/v1/sink/sink_test.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/events/v1/sink/sink_validate.py` & `twilio-8.2.1/twilio/rest/events/v1/sink/sink_validate.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/events/v1/subscription/__init__.py` & `twilio-8.2.1/twilio/rest/events/v1/subscription/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/events/v1/subscription/subscribed_event.py` & `twilio-8.2.1/twilio/rest/events/v1/subscription/subscribed_event.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/flex_api/FlexApiBase.py` & `twilio-8.2.1/twilio/rest/flex_api/FlexApiBase.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/flex_api/__init__.py` & `twilio-8.2.1/twilio/rest/flex_api/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/flex_api/v1/__init__.py` & `twilio-8.2.1/twilio/rest/flex_api/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/flex_api/v1/assessments.py` & `twilio-8.2.1/twilio/rest/flex_api/v1/assessments.py`

 * *Files 20% similar despite different names*

```diff
@@ -85,55 +85,55 @@
         return self._context
 
     def update(
         self,
         offset: float,
         answer_text: str,
         answer_id: str,
-        token: Union[str, object] = values.unset,
+        authorization: Union[str, object] = values.unset,
     ) -> "AssessmentsInstance":
         """
         Update the AssessmentsInstance
 
         :param offset: The offset of the conversation
         :param answer_text: The answer text selected by user
         :param answer_id: The id of the answer selected by user
-        :param token: The Token HTTP request header
+        :param authorization: The Authorization HTTP request header
 
         :returns: The updated AssessmentsInstance
         """
         return self._proxy.update(
             offset=offset,
             answer_text=answer_text,
             answer_id=answer_id,
-            token=token,
+            authorization=authorization,
         )
 
     async def update_async(
         self,
         offset: float,
         answer_text: str,
         answer_id: str,
-        token: Union[str, object] = values.unset,
+        authorization: Union[str, object] = values.unset,
     ) -> "AssessmentsInstance":
         """
         Asynchronous coroutine to update the AssessmentsInstance
 
         :param offset: The offset of the conversation
         :param answer_text: The answer text selected by user
         :param answer_id: The id of the answer selected by user
-        :param token: The Token HTTP request header
+        :param authorization: The Authorization HTTP request header
 
         :returns: The updated AssessmentsInstance
         """
         return await self._proxy.update_async(
             offset=offset,
             answer_text=answer_text,
             answer_id=answer_id,
-            token=token,
+            authorization=authorization,
         )
 
     def __repr__(self) -> str:
         """
         Provide a friendly representation
 
         :returns: Machine friendly representation
@@ -161,36 +161,36 @@
         )
 
     def update(
         self,
         offset: float,
         answer_text: str,
         answer_id: str,
-        token: Union[str, object] = values.unset,
+        authorization: Union[str, object] = values.unset,
     ) -> AssessmentsInstance:
         """
         Update the AssessmentsInstance
 
         :param offset: The offset of the conversation
         :param answer_text: The answer text selected by user
         :param answer_id: The id of the answer selected by user
-        :param token: The Token HTTP request header
+        :param authorization: The Authorization HTTP request header
 
         :returns: The updated AssessmentsInstance
         """
         data = values.of(
             {
                 "Offset": offset,
                 "AnswerText": answer_text,
                 "AnswerId": answer_id,
             }
         )
         headers = values.of(
             {
-                "Token": token,
+                "Authorization": authorization,
             }
         )
 
         payload = self._version.update(
             method="POST", uri=self._uri, data=data, headers=headers
         )
 
@@ -199,36 +199,36 @@
         )
 
     async def update_async(
         self,
         offset: float,
         answer_text: str,
         answer_id: str,
-        token: Union[str, object] = values.unset,
+        authorization: Union[str, object] = values.unset,
     ) -> AssessmentsInstance:
         """
         Asynchronous coroutine to update the AssessmentsInstance
 
         :param offset: The offset of the conversation
         :param answer_text: The answer text selected by user
         :param answer_id: The id of the answer selected by user
-        :param token: The Token HTTP request header
+        :param authorization: The Authorization HTTP request header
 
         :returns: The updated AssessmentsInstance
         """
         data = values.of(
             {
                 "Offset": offset,
                 "AnswerText": answer_text,
                 "AnswerId": answer_id,
             }
         )
         headers = values.of(
             {
-                "Token": token,
+                "Authorization": authorization,
             }
         )
 
         payload = await self._version.update_async(
             method="POST", uri=self._uri, data=data, headers=headers
         )
 
@@ -277,316 +277,308 @@
         self._uri = "/Insights/QualityManagement/Assessments"
 
     def create(
         self,
         category_sid: str,
         category_name: str,
         segment_id: str,
-        user_name: str,
-        user_email: str,
         agent_id: str,
         offset: float,
         metric_id: str,
         metric_name: str,
         answer_text: str,
         answer_id: str,
         questionnaire_sid: str,
-        token: Union[str, object] = values.unset,
+        authorization: Union[str, object] = values.unset,
     ) -> AssessmentsInstance:
         """
         Create the AssessmentsInstance
 
         :param category_sid: The SID of the category
         :param category_name: The name of the category
         :param segment_id: Segment Id of the conversation
-        :param user_name: Name of the user assessing conversation
-        :param user_email: Email of the user assessing conversation
         :param agent_id: The id of the Agent
         :param offset: The offset of the conversation.
         :param metric_id: The question SID selected for assessment
         :param metric_name: The question name of the assessment
         :param answer_text: The answer text selected by user
         :param answer_id: The id of the answer selected by user
         :param questionnaire_sid: Questionnaire SID of the associated question
-        :param token: The Token HTTP request header
+        :param authorization: The Authorization HTTP request header
 
         :returns: The created AssessmentsInstance
         """
         data = values.of(
             {
                 "CategorySid": category_sid,
                 "CategoryName": category_name,
                 "SegmentId": segment_id,
-                "UserName": user_name,
-                "UserEmail": user_email,
                 "AgentId": agent_id,
                 "Offset": offset,
                 "MetricId": metric_id,
                 "MetricName": metric_name,
                 "AnswerText": answer_text,
                 "AnswerId": answer_id,
                 "QuestionnaireSid": questionnaire_sid,
             }
         )
         headers = values.of(
             {
-                "Token": token,
+                "Authorization": authorization,
             }
         )
         payload = self._version.create(
             method="POST", uri=self._uri, data=data, headers=headers
         )
 
         return AssessmentsInstance(self._version, payload)
 
     async def create_async(
         self,
         category_sid: str,
         category_name: str,
         segment_id: str,
-        user_name: str,
-        user_email: str,
         agent_id: str,
         offset: float,
         metric_id: str,
         metric_name: str,
         answer_text: str,
         answer_id: str,
         questionnaire_sid: str,
-        token: Union[str, object] = values.unset,
+        authorization: Union[str, object] = values.unset,
     ) -> AssessmentsInstance:
         """
         Asynchronously create the AssessmentsInstance
 
         :param category_sid: The SID of the category
         :param category_name: The name of the category
         :param segment_id: Segment Id of the conversation
-        :param user_name: Name of the user assessing conversation
-        :param user_email: Email of the user assessing conversation
         :param agent_id: The id of the Agent
         :param offset: The offset of the conversation.
         :param metric_id: The question SID selected for assessment
         :param metric_name: The question name of the assessment
         :param answer_text: The answer text selected by user
         :param answer_id: The id of the answer selected by user
         :param questionnaire_sid: Questionnaire SID of the associated question
-        :param token: The Token HTTP request header
+        :param authorization: The Authorization HTTP request header
 
         :returns: The created AssessmentsInstance
         """
         data = values.of(
             {
                 "CategorySid": category_sid,
                 "CategoryName": category_name,
                 "SegmentId": segment_id,
-                "UserName": user_name,
-                "UserEmail": user_email,
                 "AgentId": agent_id,
                 "Offset": offset,
                 "MetricId": metric_id,
                 "MetricName": metric_name,
                 "AnswerText": answer_text,
                 "AnswerId": answer_id,
                 "QuestionnaireSid": questionnaire_sid,
             }
         )
         headers = values.of(
             {
-                "Token": token,
+                "Authorization": authorization,
             }
         )
         payload = await self._version.create_async(
             method="POST", uri=self._uri, data=data, headers=headers
         )
 
         return AssessmentsInstance(self._version, payload)
 
     def stream(
         self,
-        token: Union[str, object] = values.unset,
+        authorization: Union[str, object] = values.unset,
         segment_id: Union[str, object] = values.unset,
         limit: Optional[int] = None,
         page_size: Optional[int] = None,
     ) -> Iterator[AssessmentsInstance]:
         """
         Streams AssessmentsInstance records from the API as a generator stream.
         This operation lazily loads records as efficiently as possible until the limit
         is reached.
         The results are returned as a generator, so this operation is memory efficient.
 
-        :param str token: The Token HTTP request header
+        :param str authorization: The Authorization HTTP request header
         :param str segment_id: The id of the segment.
         :param limit: Upper limit for the number of records to return. stream()
                       guarantees to never return more than limit.  Default is no limit
         :param page_size: Number of records to fetch per request, when not set will use
                           the default value of 50 records.  If no page_size is defined
                           but a limit is defined, stream() will attempt to read the
                           limit with the most efficient page size, i.e. min(limit, 1000)
 
         :returns: Generator that will yield up to limit results
         """
         limits = self._version.read_limits(limit, page_size)
         page = self.page(
-            token=token, segment_id=segment_id, page_size=limits["page_size"]
+            authorization=authorization,
+            segment_id=segment_id,
+            page_size=limits["page_size"],
         )
 
         return self._version.stream(page, limits["limit"])
 
     async def stream_async(
         self,
-        token: Union[str, object] = values.unset,
+        authorization: Union[str, object] = values.unset,
         segment_id: Union[str, object] = values.unset,
         limit: Optional[int] = None,
         page_size: Optional[int] = None,
     ) -> AsyncIterator[AssessmentsInstance]:
         """
         Asynchronously streams AssessmentsInstance records from the API as a generator stream.
         This operation lazily loads records as efficiently as possible until the limit
         is reached.
         The results are returned as a generator, so this operation is memory efficient.
 
-        :param str token: The Token HTTP request header
+        :param str authorization: The Authorization HTTP request header
         :param str segment_id: The id of the segment.
         :param limit: Upper limit for the number of records to return. stream()
                       guarantees to never return more than limit.  Default is no limit
         :param page_size: Number of records to fetch per request, when not set will use
                           the default value of 50 records.  If no page_size is defined
                           but a limit is defined, stream() will attempt to read the
                           limit with the most efficient page size, i.e. min(limit, 1000)
 
         :returns: Generator that will yield up to limit results
         """
         limits = self._version.read_limits(limit, page_size)
         page = await self.page_async(
-            token=token, segment_id=segment_id, page_size=limits["page_size"]
+            authorization=authorization,
+            segment_id=segment_id,
+            page_size=limits["page_size"],
         )
 
         return self._version.stream_async(page, limits["limit"])
 
     def list(
         self,
-        token: Union[str, object] = values.unset,
+        authorization: Union[str, object] = values.unset,
         segment_id: Union[str, object] = values.unset,
         limit: Optional[int] = None,
         page_size: Optional[int] = None,
     ) -> List[AssessmentsInstance]:
         """
         Lists AssessmentsInstance records from the API as a list.
         Unlike stream(), this operation is eager and will load `limit` records into
         memory before returning.
 
-        :param str token: The Token HTTP request header
+        :param str authorization: The Authorization HTTP request header
         :param str segment_id: The id of the segment.
         :param limit: Upper limit for the number of records to return. list() guarantees
                       never to return more than limit.  Default is no limit
         :param page_size: Number of records to fetch per request, when not set will use
                           the default value of 50 records.  If no page_size is defined
                           but a limit is defined, list() will attempt to read the limit
                           with the most efficient page size, i.e. min(limit, 1000)
 
         :returns: list that will contain up to limit results
         """
         return list(
             self.stream(
-                token=token,
+                authorization=authorization,
                 segment_id=segment_id,
                 limit=limit,
                 page_size=page_size,
             )
         )
 
     async def list_async(
         self,
-        token: Union[str, object] = values.unset,
+        authorization: Union[str, object] = values.unset,
         segment_id: Union[str, object] = values.unset,
         limit: Optional[int] = None,
         page_size: Optional[int] = None,
     ) -> List[AssessmentsInstance]:
         """
         Asynchronously lists AssessmentsInstance records from the API as a list.
         Unlike stream(), this operation is eager and will load `limit` records into
         memory before returning.
 
-        :param str token: The Token HTTP request header
+        :param str authorization: The Authorization HTTP request header
         :param str segment_id: The id of the segment.
         :param limit: Upper limit for the number of records to return. list() guarantees
                       never to return more than limit.  Default is no limit
         :param page_size: Number of records to fetch per request, when not set will use
                           the default value of 50 records.  If no page_size is defined
                           but a limit is defined, list() will attempt to read the limit
                           with the most efficient page size, i.e. min(limit, 1000)
 
         :returns: list that will contain up to limit results
         """
         return [
             record
             async for record in await self.stream_async(
-                token=token,
+                authorization=authorization,
                 segment_id=segment_id,
                 limit=limit,
                 page_size=page_size,
             )
         ]
 
     def page(
         self,
-        token: Union[str, object] = values.unset,
+        authorization: Union[str, object] = values.unset,
         segment_id: Union[str, object] = values.unset,
         page_token: Union[str, object] = values.unset,
         page_number: Union[int, object] = values.unset,
         page_size: Union[int, object] = values.unset,
     ) -> AssessmentsPage:
         """
         Retrieve a single page of AssessmentsInstance records from the API.
         Request is executed immediately
 
-        :param token: The Token HTTP request header
+        :param authorization: The Authorization HTTP request header
         :param segment_id: The id of the segment.
         :param page_token: PageToken provided by the API
         :param page_number: Page Number, this value is simply for client state
         :param page_size: Number of records to return, defaults to 50
 
         :returns: Page of AssessmentsInstance
         """
         data = values.of(
             {
-                "Token": token,
+                "Authorization": authorization,
                 "SegmentId": segment_id,
                 "PageToken": page_token,
                 "Page": page_number,
                 "PageSize": page_size,
             }
         )
 
         response = self._version.page(method="GET", uri=self._uri, params=data)
         return AssessmentsPage(self._version, response)
 
     async def page_async(
         self,
-        token: Union[str, object] = values.unset,
+        authorization: Union[str, object] = values.unset,
         segment_id: Union[str, object] = values.unset,
         page_token: Union[str, object] = values.unset,
         page_number: Union[int, object] = values.unset,
         page_size: Union[int, object] = values.unset,
     ) -> AssessmentsPage:
         """
         Asynchronously retrieve a single page of AssessmentsInstance records from the API.
         Request is executed immediately
 
-        :param token: The Token HTTP request header
+        :param authorization: The Authorization HTTP request header
         :param segment_id: The id of the segment.
         :param page_token: PageToken provided by the API
         :param page_number: Page Number, this value is simply for client state
         :param page_size: Number of records to return, defaults to 50
 
         :returns: Page of AssessmentsInstance
         """
         data = values.of(
             {
-                "Token": token,
+                "Authorization": authorization,
                 "SegmentId": segment_id,
                 "PageToken": page_token,
                 "Page": page_number,
                 "PageSize": page_size,
             }
         )
```

### Comparing `twilio-8.2.0/twilio/rest/flex_api/v1/channel.py` & `twilio-8.2.1/twilio/rest/flex_api/v1/channel.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/flex_api/v1/configuration.py` & `twilio-8.2.1/twilio/rest/flex_api/v1/configuration.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/flex_api/v1/flex_flow.py` & `twilio-8.2.1/twilio/rest/flex_api/v1/flex_flow.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/flex_api/v1/insights_assessments_comment.py` & `twilio-8.2.1/twilio/rest/flex_api/v1/insights_assessments_comment.py`

 * *Files 8% similar despite different names*

```diff
@@ -99,312 +99,300 @@
 
     def create(
         self,
         category_id: str,
         category_name: str,
         comment: str,
         segment_id: str,
-        user_name: str,
-        user_email: str,
         agent_id: str,
         offset: float,
-        token: Union[str, object] = values.unset,
+        authorization: Union[str, object] = values.unset,
     ) -> InsightsAssessmentsCommentInstance:
         """
         Create the InsightsAssessmentsCommentInstance
 
         :param category_id: The ID of the category
         :param category_name: The name of the category
         :param comment: The Assessment comment.
         :param segment_id: The id of the segment.
-        :param user_name: The name of the user.
-        :param user_email: The email id of the user.
         :param agent_id: The id of the agent.
         :param offset: The offset
-        :param token: The Token HTTP request header
+        :param authorization: The Authorization HTTP request header
 
         :returns: The created InsightsAssessmentsCommentInstance
         """
         data = values.of(
             {
                 "CategoryId": category_id,
                 "CategoryName": category_name,
                 "Comment": comment,
                 "SegmentId": segment_id,
-                "UserName": user_name,
-                "UserEmail": user_email,
                 "AgentId": agent_id,
                 "Offset": offset,
             }
         )
         headers = values.of(
             {
-                "Token": token,
+                "Authorization": authorization,
             }
         )
         payload = self._version.create(
             method="POST", uri=self._uri, data=data, headers=headers
         )
 
         return InsightsAssessmentsCommentInstance(self._version, payload)
 
     async def create_async(
         self,
         category_id: str,
         category_name: str,
         comment: str,
         segment_id: str,
-        user_name: str,
-        user_email: str,
         agent_id: str,
         offset: float,
-        token: Union[str, object] = values.unset,
+        authorization: Union[str, object] = values.unset,
     ) -> InsightsAssessmentsCommentInstance:
         """
         Asynchronously create the InsightsAssessmentsCommentInstance
 
         :param category_id: The ID of the category
         :param category_name: The name of the category
         :param comment: The Assessment comment.
         :param segment_id: The id of the segment.
-        :param user_name: The name of the user.
-        :param user_email: The email id of the user.
         :param agent_id: The id of the agent.
         :param offset: The offset
-        :param token: The Token HTTP request header
+        :param authorization: The Authorization HTTP request header
 
         :returns: The created InsightsAssessmentsCommentInstance
         """
         data = values.of(
             {
                 "CategoryId": category_id,
                 "CategoryName": category_name,
                 "Comment": comment,
                 "SegmentId": segment_id,
-                "UserName": user_name,
-                "UserEmail": user_email,
                 "AgentId": agent_id,
                 "Offset": offset,
             }
         )
         headers = values.of(
             {
-                "Token": token,
+                "Authorization": authorization,
             }
         )
         payload = await self._version.create_async(
             method="POST", uri=self._uri, data=data, headers=headers
         )
 
         return InsightsAssessmentsCommentInstance(self._version, payload)
 
     def stream(
         self,
-        token: Union[str, object] = values.unset,
+        authorization: Union[str, object] = values.unset,
         segment_id: Union[str, object] = values.unset,
         agent_id: Union[str, object] = values.unset,
         limit: Optional[int] = None,
         page_size: Optional[int] = None,
     ) -> Iterator[InsightsAssessmentsCommentInstance]:
         """
         Streams InsightsAssessmentsCommentInstance records from the API as a generator stream.
         This operation lazily loads records as efficiently as possible until the limit
         is reached.
         The results are returned as a generator, so this operation is memory efficient.
 
-        :param str token: The Token HTTP request header
+        :param str authorization: The Authorization HTTP request header
         :param str segment_id: The id of the segment.
         :param str agent_id: The id of the agent.
         :param limit: Upper limit for the number of records to return. stream()
                       guarantees to never return more than limit.  Default is no limit
         :param page_size: Number of records to fetch per request, when not set will use
                           the default value of 50 records.  If no page_size is defined
                           but a limit is defined, stream() will attempt to read the
                           limit with the most efficient page size, i.e. min(limit, 1000)
 
         :returns: Generator that will yield up to limit results
         """
         limits = self._version.read_limits(limit, page_size)
         page = self.page(
-            token=token,
+            authorization=authorization,
             segment_id=segment_id,
             agent_id=agent_id,
             page_size=limits["page_size"],
         )
 
         return self._version.stream(page, limits["limit"])
 
     async def stream_async(
         self,
-        token: Union[str, object] = values.unset,
+        authorization: Union[str, object] = values.unset,
         segment_id: Union[str, object] = values.unset,
         agent_id: Union[str, object] = values.unset,
         limit: Optional[int] = None,
         page_size: Optional[int] = None,
     ) -> AsyncIterator[InsightsAssessmentsCommentInstance]:
         """
         Asynchronously streams InsightsAssessmentsCommentInstance records from the API as a generator stream.
         This operation lazily loads records as efficiently as possible until the limit
         is reached.
         The results are returned as a generator, so this operation is memory efficient.
 
-        :param str token: The Token HTTP request header
+        :param str authorization: The Authorization HTTP request header
         :param str segment_id: The id of the segment.
         :param str agent_id: The id of the agent.
         :param limit: Upper limit for the number of records to return. stream()
                       guarantees to never return more than limit.  Default is no limit
         :param page_size: Number of records to fetch per request, when not set will use
                           the default value of 50 records.  If no page_size is defined
                           but a limit is defined, stream() will attempt to read the
                           limit with the most efficient page size, i.e. min(limit, 1000)
 
         :returns: Generator that will yield up to limit results
         """
         limits = self._version.read_limits(limit, page_size)
         page = await self.page_async(
-            token=token,
+            authorization=authorization,
             segment_id=segment_id,
             agent_id=agent_id,
             page_size=limits["page_size"],
         )
 
         return self._version.stream_async(page, limits["limit"])
 
     def list(
         self,
-        token: Union[str, object] = values.unset,
+        authorization: Union[str, object] = values.unset,
         segment_id: Union[str, object] = values.unset,
         agent_id: Union[str, object] = values.unset,
         limit: Optional[int] = None,
         page_size: Optional[int] = None,
     ) -> List[InsightsAssessmentsCommentInstance]:
         """
         Lists InsightsAssessmentsCommentInstance records from the API as a list.
         Unlike stream(), this operation is eager and will load `limit` records into
         memory before returning.
 
-        :param str token: The Token HTTP request header
+        :param str authorization: The Authorization HTTP request header
         :param str segment_id: The id of the segment.
         :param str agent_id: The id of the agent.
         :param limit: Upper limit for the number of records to return. list() guarantees
                       never to return more than limit.  Default is no limit
         :param page_size: Number of records to fetch per request, when not set will use
                           the default value of 50 records.  If no page_size is defined
                           but a limit is defined, list() will attempt to read the limit
                           with the most efficient page size, i.e. min(limit, 1000)
 
         :returns: list that will contain up to limit results
         """
         return list(
             self.stream(
-                token=token,
+                authorization=authorization,
                 segment_id=segment_id,
                 agent_id=agent_id,
                 limit=limit,
                 page_size=page_size,
             )
         )
 
     async def list_async(
         self,
-        token: Union[str, object] = values.unset,
+        authorization: Union[str, object] = values.unset,
         segment_id: Union[str, object] = values.unset,
         agent_id: Union[str, object] = values.unset,
         limit: Optional[int] = None,
         page_size: Optional[int] = None,
     ) -> List[InsightsAssessmentsCommentInstance]:
         """
         Asynchronously lists InsightsAssessmentsCommentInstance records from the API as a list.
         Unlike stream(), this operation is eager and will load `limit` records into
         memory before returning.
 
-        :param str token: The Token HTTP request header
+        :param str authorization: The Authorization HTTP request header
         :param str segment_id: The id of the segment.
         :param str agent_id: The id of the agent.
         :param limit: Upper limit for the number of records to return. list() guarantees
                       never to return more than limit.  Default is no limit
         :param page_size: Number of records to fetch per request, when not set will use
                           the default value of 50 records.  If no page_size is defined
                           but a limit is defined, list() will attempt to read the limit
                           with the most efficient page size, i.e. min(limit, 1000)
 
         :returns: list that will contain up to limit results
         """
         return [
             record
             async for record in await self.stream_async(
-                token=token,
+                authorization=authorization,
                 segment_id=segment_id,
                 agent_id=agent_id,
                 limit=limit,
                 page_size=page_size,
             )
         ]
 
     def page(
         self,
-        token: Union[str, object] = values.unset,
+        authorization: Union[str, object] = values.unset,
         segment_id: Union[str, object] = values.unset,
         agent_id: Union[str, object] = values.unset,
         page_token: Union[str, object] = values.unset,
         page_number: Union[int, object] = values.unset,
         page_size: Union[int, object] = values.unset,
     ) -> InsightsAssessmentsCommentPage:
         """
         Retrieve a single page of InsightsAssessmentsCommentInstance records from the API.
         Request is executed immediately
 
-        :param token: The Token HTTP request header
+        :param authorization: The Authorization HTTP request header
         :param segment_id: The id of the segment.
         :param agent_id: The id of the agent.
         :param page_token: PageToken provided by the API
         :param page_number: Page Number, this value is simply for client state
         :param page_size: Number of records to return, defaults to 50
 
         :returns: Page of InsightsAssessmentsCommentInstance
         """
         data = values.of(
             {
-                "Token": token,
+                "Authorization": authorization,
                 "SegmentId": segment_id,
                 "AgentId": agent_id,
                 "PageToken": page_token,
                 "Page": page_number,
                 "PageSize": page_size,
             }
         )
 
         response = self._version.page(method="GET", uri=self._uri, params=data)
         return InsightsAssessmentsCommentPage(self._version, response)
 
     async def page_async(
         self,
-        token: Union[str, object] = values.unset,
+        authorization: Union[str, object] = values.unset,
         segment_id: Union[str, object] = values.unset,
         agent_id: Union[str, object] = values.unset,
         page_token: Union[str, object] = values.unset,
         page_number: Union[int, object] = values.unset,
         page_size: Union[int, object] = values.unset,
     ) -> InsightsAssessmentsCommentPage:
         """
         Asynchronously retrieve a single page of InsightsAssessmentsCommentInstance records from the API.
         Request is executed immediately
 
-        :param token: The Token HTTP request header
+        :param authorization: The Authorization HTTP request header
         :param segment_id: The id of the segment.
         :param agent_id: The id of the agent.
         :param page_token: PageToken provided by the API
         :param page_number: Page Number, this value is simply for client state
         :param page_size: Number of records to return, defaults to 50
 
         :returns: Page of InsightsAssessmentsCommentInstance
         """
         data = values.of(
             {
-                "Token": token,
+                "Authorization": authorization,
                 "SegmentId": segment_id,
                 "AgentId": agent_id,
                 "PageToken": page_token,
                 "Page": page_number,
                 "PageSize": page_size,
             }
         )
```

### Comparing `twilio-8.2.0/twilio/rest/flex_api/v1/insights_conversations.py` & `twilio-8.2.1/twilio/rest/flex_api/v1/insights_conversations.py`

 * *Files 8% similar despite different names*

```diff
@@ -79,195 +79,199 @@
         """
         super().__init__(version)
 
         self._uri = "/Insights/Conversations"
 
     def stream(
         self,
-        token: Union[str, object] = values.unset,
+        authorization: Union[str, object] = values.unset,
         segment_id: Union[str, object] = values.unset,
         limit: Optional[int] = None,
         page_size: Optional[int] = None,
     ) -> Iterator[InsightsConversationsInstance]:
         """
         Streams InsightsConversationsInstance records from the API as a generator stream.
         This operation lazily loads records as efficiently as possible until the limit
         is reached.
         The results are returned as a generator, so this operation is memory efficient.
 
-        :param str token: The Token HTTP request header
+        :param str authorization: The Authorization HTTP request header
         :param str segment_id: Unique Id of the segment for which conversation details needs to be fetched
         :param limit: Upper limit for the number of records to return. stream()
                       guarantees to never return more than limit.  Default is no limit
         :param page_size: Number of records to fetch per request, when not set will use
                           the default value of 50 records.  If no page_size is defined
                           but a limit is defined, stream() will attempt to read the
                           limit with the most efficient page size, i.e. min(limit, 1000)
 
         :returns: Generator that will yield up to limit results
         """
         limits = self._version.read_limits(limit, page_size)
         page = self.page(
-            token=token, segment_id=segment_id, page_size=limits["page_size"]
+            authorization=authorization,
+            segment_id=segment_id,
+            page_size=limits["page_size"],
         )
 
         return self._version.stream(page, limits["limit"])
 
     async def stream_async(
         self,
-        token: Union[str, object] = values.unset,
+        authorization: Union[str, object] = values.unset,
         segment_id: Union[str, object] = values.unset,
         limit: Optional[int] = None,
         page_size: Optional[int] = None,
     ) -> AsyncIterator[InsightsConversationsInstance]:
         """
         Asynchronously streams InsightsConversationsInstance records from the API as a generator stream.
         This operation lazily loads records as efficiently as possible until the limit
         is reached.
         The results are returned as a generator, so this operation is memory efficient.
 
-        :param str token: The Token HTTP request header
+        :param str authorization: The Authorization HTTP request header
         :param str segment_id: Unique Id of the segment for which conversation details needs to be fetched
         :param limit: Upper limit for the number of records to return. stream()
                       guarantees to never return more than limit.  Default is no limit
         :param page_size: Number of records to fetch per request, when not set will use
                           the default value of 50 records.  If no page_size is defined
                           but a limit is defined, stream() will attempt to read the
                           limit with the most efficient page size, i.e. min(limit, 1000)
 
         :returns: Generator that will yield up to limit results
         """
         limits = self._version.read_limits(limit, page_size)
         page = await self.page_async(
-            token=token, segment_id=segment_id, page_size=limits["page_size"]
+            authorization=authorization,
+            segment_id=segment_id,
+            page_size=limits["page_size"],
         )
 
         return self._version.stream_async(page, limits["limit"])
 
     def list(
         self,
-        token: Union[str, object] = values.unset,
+        authorization: Union[str, object] = values.unset,
         segment_id: Union[str, object] = values.unset,
         limit: Optional[int] = None,
         page_size: Optional[int] = None,
     ) -> List[InsightsConversationsInstance]:
         """
         Lists InsightsConversationsInstance records from the API as a list.
         Unlike stream(), this operation is eager and will load `limit` records into
         memory before returning.
 
-        :param str token: The Token HTTP request header
+        :param str authorization: The Authorization HTTP request header
         :param str segment_id: Unique Id of the segment for which conversation details needs to be fetched
         :param limit: Upper limit for the number of records to return. list() guarantees
                       never to return more than limit.  Default is no limit
         :param page_size: Number of records to fetch per request, when not set will use
                           the default value of 50 records.  If no page_size is defined
                           but a limit is defined, list() will attempt to read the limit
                           with the most efficient page size, i.e. min(limit, 1000)
 
         :returns: list that will contain up to limit results
         """
         return list(
             self.stream(
-                token=token,
+                authorization=authorization,
                 segment_id=segment_id,
                 limit=limit,
                 page_size=page_size,
             )
         )
 
     async def list_async(
         self,
-        token: Union[str, object] = values.unset,
+        authorization: Union[str, object] = values.unset,
         segment_id: Union[str, object] = values.unset,
         limit: Optional[int] = None,
         page_size: Optional[int] = None,
     ) -> List[InsightsConversationsInstance]:
         """
         Asynchronously lists InsightsConversationsInstance records from the API as a list.
         Unlike stream(), this operation is eager and will load `limit` records into
         memory before returning.
 
-        :param str token: The Token HTTP request header
+        :param str authorization: The Authorization HTTP request header
         :param str segment_id: Unique Id of the segment for which conversation details needs to be fetched
         :param limit: Upper limit for the number of records to return. list() guarantees
                       never to return more than limit.  Default is no limit
         :param page_size: Number of records to fetch per request, when not set will use
                           the default value of 50 records.  If no page_size is defined
                           but a limit is defined, list() will attempt to read the limit
                           with the most efficient page size, i.e. min(limit, 1000)
 
         :returns: list that will contain up to limit results
         """
         return [
             record
             async for record in await self.stream_async(
-                token=token,
+                authorization=authorization,
                 segment_id=segment_id,
                 limit=limit,
                 page_size=page_size,
             )
         ]
 
     def page(
         self,
-        token: Union[str, object] = values.unset,
+        authorization: Union[str, object] = values.unset,
         segment_id: Union[str, object] = values.unset,
         page_token: Union[str, object] = values.unset,
         page_number: Union[int, object] = values.unset,
         page_size: Union[int, object] = values.unset,
     ) -> InsightsConversationsPage:
         """
         Retrieve a single page of InsightsConversationsInstance records from the API.
         Request is executed immediately
 
-        :param token: The Token HTTP request header
+        :param authorization: The Authorization HTTP request header
         :param segment_id: Unique Id of the segment for which conversation details needs to be fetched
         :param page_token: PageToken provided by the API
         :param page_number: Page Number, this value is simply for client state
         :param page_size: Number of records to return, defaults to 50
 
         :returns: Page of InsightsConversationsInstance
         """
         data = values.of(
             {
-                "Token": token,
+                "Authorization": authorization,
                 "SegmentId": segment_id,
                 "PageToken": page_token,
                 "Page": page_number,
                 "PageSize": page_size,
             }
         )
 
         response = self._version.page(method="GET", uri=self._uri, params=data)
         return InsightsConversationsPage(self._version, response)
 
     async def page_async(
         self,
-        token: Union[str, object] = values.unset,
+        authorization: Union[str, object] = values.unset,
         segment_id: Union[str, object] = values.unset,
         page_token: Union[str, object] = values.unset,
         page_number: Union[int, object] = values.unset,
         page_size: Union[int, object] = values.unset,
     ) -> InsightsConversationsPage:
         """
         Asynchronously retrieve a single page of InsightsConversationsInstance records from the API.
         Request is executed immediately
 
-        :param token: The Token HTTP request header
+        :param authorization: The Authorization HTTP request header
         :param segment_id: Unique Id of the segment for which conversation details needs to be fetched
         :param page_token: PageToken provided by the API
         :param page_number: Page Number, this value is simply for client state
         :param page_size: Number of records to return, defaults to 50
 
         :returns: Page of InsightsConversationsInstance
         """
         data = values.of(
             {
-                "Token": token,
+                "Authorization": authorization,
                 "SegmentId": segment_id,
                 "PageToken": page_token,
                 "Page": page_number,
                 "PageSize": page_size,
             }
         )
```

### Comparing `twilio-8.2.0/twilio/rest/flex_api/v1/insights_questionnaires.py` & `twilio-8.2.1/twilio/rest/flex_api/v1/insights_questionnaires.py`

 * *Files 14% similar despite different names*

```diff
@@ -66,115 +66,117 @@
         if self._context is None:
             self._context = InsightsQuestionnairesContext(
                 self._version,
                 questionnaire_sid=self._solution["questionnaire_sid"],
             )
         return self._context
 
-    def delete(self, token: Union[str, object] = values.unset) -> bool:
+    def delete(self, authorization: Union[str, object] = values.unset) -> bool:
         """
         Deletes the InsightsQuestionnairesInstance
 
-        :param token: The Token HTTP request header
+        :param authorization: The Authorization HTTP request header
 
         :returns: True if delete succeeds, False otherwise
         """
         return self._proxy.delete(
-            token=token,
+            authorization=authorization,
         )
 
-    async def delete_async(self, token: Union[str, object] = values.unset) -> bool:
+    async def delete_async(
+        self, authorization: Union[str, object] = values.unset
+    ) -> bool:
         """
         Asynchronous coroutine that deletes the InsightsQuestionnairesInstance
 
-        :param token: The Token HTTP request header
+        :param authorization: The Authorization HTTP request header
 
         :returns: True if delete succeeds, False otherwise
         """
         return await self._proxy.delete_async(
-            token=token,
+            authorization=authorization,
         )
 
     def fetch(
-        self, token: Union[str, object] = values.unset
+        self, authorization: Union[str, object] = values.unset
     ) -> "InsightsQuestionnairesInstance":
         """
         Fetch the InsightsQuestionnairesInstance
 
-        :param token: The Token HTTP request header
+        :param authorization: The Authorization HTTP request header
 
         :returns: The fetched InsightsQuestionnairesInstance
         """
         return self._proxy.fetch(
-            token=token,
+            authorization=authorization,
         )
 
     async def fetch_async(
-        self, token: Union[str, object] = values.unset
+        self, authorization: Union[str, object] = values.unset
     ) -> "InsightsQuestionnairesInstance":
         """
         Asynchronous coroutine to fetch the InsightsQuestionnairesInstance
 
-        :param token: The Token HTTP request header
+        :param authorization: The Authorization HTTP request header
 
         :returns: The fetched InsightsQuestionnairesInstance
         """
         return await self._proxy.fetch_async(
-            token=token,
+            authorization=authorization,
         )
 
     def update(
         self,
         active: bool,
-        token: Union[str, object] = values.unset,
+        authorization: Union[str, object] = values.unset,
         name: Union[str, object] = values.unset,
         description: Union[str, object] = values.unset,
         question_sids: Union[List[str], object] = values.unset,
     ) -> "InsightsQuestionnairesInstance":
         """
         Update the InsightsQuestionnairesInstance
 
         :param active: The flag to enable or disable questionnaire
-        :param token: The Token HTTP request header
+        :param authorization: The Authorization HTTP request header
         :param name: The name of this questionnaire
         :param description: The description of this questionnaire
         :param question_sids: The list of questions sids under a questionnaire
 
         :returns: The updated InsightsQuestionnairesInstance
         """
         return self._proxy.update(
             active=active,
-            token=token,
+            authorization=authorization,
             name=name,
             description=description,
             question_sids=question_sids,
         )
 
     async def update_async(
         self,
         active: bool,
-        token: Union[str, object] = values.unset,
+        authorization: Union[str, object] = values.unset,
         name: Union[str, object] = values.unset,
         description: Union[str, object] = values.unset,
         question_sids: Union[List[str], object] = values.unset,
     ) -> "InsightsQuestionnairesInstance":
         """
         Asynchronous coroutine to update the InsightsQuestionnairesInstance
 
         :param active: The flag to enable or disable questionnaire
-        :param token: The Token HTTP request header
+        :param authorization: The Authorization HTTP request header
         :param name: The name of this questionnaire
         :param description: The description of this questionnaire
         :param question_sids: The list of questions sids under a questionnaire
 
         :returns: The updated InsightsQuestionnairesInstance
         """
         return await self._proxy.update_async(
             active=active,
-            token=token,
+            authorization=authorization,
             name=name,
             description=description,
             question_sids=question_sids,
         )
 
     def __repr__(self) -> str:
         """
@@ -202,87 +204,89 @@
         }
         self._uri = (
             "/Insights/QualityManagement/Questionnaires/{questionnaire_sid}".format(
                 **self._solution
             )
         )
 
-    def delete(self, token: Union[str, object] = values.unset) -> bool:
+    def delete(self, authorization: Union[str, object] = values.unset) -> bool:
         """
         Deletes the InsightsQuestionnairesInstance
 
-        :param token: The Token HTTP request header
+        :param authorization: The Authorization HTTP request header
 
         :returns: True if delete succeeds, False otherwise
         """
         headers = values.of(
             {
-                "Token": token,
+                "Authorization": authorization,
             }
         )
 
         return self._version.delete(method="DELETE", uri=self._uri, headers=headers)
 
-    async def delete_async(self, token: Union[str, object] = values.unset) -> bool:
+    async def delete_async(
+        self, authorization: Union[str, object] = values.unset
+    ) -> bool:
         """
         Asynchronous coroutine that deletes the InsightsQuestionnairesInstance
 
-        :param token: The Token HTTP request header
+        :param authorization: The Authorization HTTP request header
 
         :returns: True if delete succeeds, False otherwise
         """
         headers = values.of(
             {
-                "Token": token,
+                "Authorization": authorization,
             }
         )
 
         return await self._version.delete_async(
             method="DELETE", uri=self._uri, headers=headers
         )
 
     def fetch(
-        self, token: Union[str, object] = values.unset
+        self, authorization: Union[str, object] = values.unset
     ) -> InsightsQuestionnairesInstance:
         """
         Fetch the InsightsQuestionnairesInstance
 
-        :param token: The Token HTTP request header
+        :param authorization: The Authorization HTTP request header
 
         :returns: The fetched InsightsQuestionnairesInstance
         """
 
         data = values.of(
             {
-                "Token": token,
+                "Authorization": authorization,
             }
         )
 
         payload = self._version.fetch(method="GET", uri=self._uri, params=data)
 
         return InsightsQuestionnairesInstance(
             self._version,
             payload,
             questionnaire_sid=self._solution["questionnaire_sid"],
         )
 
     async def fetch_async(
-        self, token: Union[str, object] = values.unset
+        self, authorization: Union[str, object] = values.unset
     ) -> InsightsQuestionnairesInstance:
         """
         Asynchronous coroutine to fetch the InsightsQuestionnairesInstance
 
-        :param token: The Token HTTP request header
+        :param authorization: The Authorization HTTP request header
 
         :returns: The fetched InsightsQuestionnairesInstance
         """
 
         data = values.of(
             {
-                "Token": token,
+                "Authorization": authorization,
             }
         )
 
         payload = await self._version.fetch_async(
             method="GET", uri=self._uri, params=data
         )
 
@@ -291,24 +295,24 @@
             payload,
             questionnaire_sid=self._solution["questionnaire_sid"],
         )
 
     def update(
         self,
         active: bool,
-        token: Union[str, object] = values.unset,
+        authorization: Union[str, object] = values.unset,
         name: Union[str, object] = values.unset,
         description: Union[str, object] = values.unset,
         question_sids: Union[List[str], object] = values.unset,
     ) -> InsightsQuestionnairesInstance:
         """
         Update the InsightsQuestionnairesInstance
 
         :param active: The flag to enable or disable questionnaire
-        :param token: The Token HTTP request header
+        :param authorization: The Authorization HTTP request header
         :param name: The name of this questionnaire
         :param description: The description of this questionnaire
         :param question_sids: The list of questions sids under a questionnaire
 
         :returns: The updated InsightsQuestionnairesInstance
         """
         data = values.of(
@@ -317,15 +321,15 @@
                 "Name": name,
                 "Description": description,
                 "QuestionSids": serialize.map(question_sids, lambda e: e),
             }
         )
         headers = values.of(
             {
-                "Token": token,
+                "Authorization": authorization,
             }
         )
 
         payload = self._version.update(
             method="POST", uri=self._uri, data=data, headers=headers
         )
 
@@ -334,24 +338,24 @@
             payload,
             questionnaire_sid=self._solution["questionnaire_sid"],
         )
 
     async def update_async(
         self,
         active: bool,
-        token: Union[str, object] = values.unset,
+        authorization: Union[str, object] = values.unset,
         name: Union[str, object] = values.unset,
         description: Union[str, object] = values.unset,
         question_sids: Union[List[str], object] = values.unset,
     ) -> InsightsQuestionnairesInstance:
         """
         Asynchronous coroutine to update the InsightsQuestionnairesInstance
 
         :param active: The flag to enable or disable questionnaire
-        :param token: The Token HTTP request header
+        :param authorization: The Authorization HTTP request header
         :param name: The name of this questionnaire
         :param description: The description of this questionnaire
         :param question_sids: The list of questions sids under a questionnaire
 
         :returns: The updated InsightsQuestionnairesInstance
         """
         data = values.of(
@@ -360,15 +364,15 @@
                 "Name": name,
                 "Description": description,
                 "QuestionSids": serialize.map(question_sids, lambda e: e),
             }
         )
         headers = values.of(
             {
-                "Token": token,
+                "Authorization": authorization,
             }
         )
 
         payload = await self._version.update_async(
             method="POST", uri=self._uri, data=data, headers=headers
         )
 
@@ -417,24 +421,24 @@
         super().__init__(version)
 
         self._uri = "/Insights/QualityManagement/Questionnaires"
 
     def create(
         self,
         name: str,
-        token: Union[str, object] = values.unset,
+        authorization: Union[str, object] = values.unset,
         description: Union[str, object] = values.unset,
         active: Union[bool, object] = values.unset,
         question_sids: Union[List[str], object] = values.unset,
     ) -> InsightsQuestionnairesInstance:
         """
         Create the InsightsQuestionnairesInstance
 
         :param name: The name of this questionnaire
-        :param token: The Token HTTP request header
+        :param authorization: The Authorization HTTP request header
         :param description: The description of this questionnaire
         :param active: The flag to enable or disable questionnaire
         :param question_sids: The list of questions sids under a questionnaire
 
         :returns: The created InsightsQuestionnairesInstance
         """
         data = values.of(
@@ -443,36 +447,36 @@
                 "Description": description,
                 "Active": active,
                 "QuestionSids": serialize.map(question_sids, lambda e: e),
             }
         )
         headers = values.of(
             {
-                "Token": token,
+                "Authorization": authorization,
             }
         )
         payload = self._version.create(
             method="POST", uri=self._uri, data=data, headers=headers
         )
 
         return InsightsQuestionnairesInstance(self._version, payload)
 
     async def create_async(
         self,
         name: str,
-        token: Union[str, object] = values.unset,
+        authorization: Union[str, object] = values.unset,
         description: Union[str, object] = values.unset,
         active: Union[bool, object] = values.unset,
         question_sids: Union[List[str], object] = values.unset,
     ) -> InsightsQuestionnairesInstance:
         """
         Asynchronously create the InsightsQuestionnairesInstance
 
         :param name: The name of this questionnaire
-        :param token: The Token HTTP request header
+        :param authorization: The Authorization HTTP request header
         :param description: The description of this questionnaire
         :param active: The flag to enable or disable questionnaire
         :param question_sids: The list of questions sids under a questionnaire
 
         :returns: The created InsightsQuestionnairesInstance
         """
         data = values.of(
@@ -481,210 +485,210 @@
                 "Description": description,
                 "Active": active,
                 "QuestionSids": serialize.map(question_sids, lambda e: e),
             }
         )
         headers = values.of(
             {
-                "Token": token,
+                "Authorization": authorization,
             }
         )
         payload = await self._version.create_async(
             method="POST", uri=self._uri, data=data, headers=headers
         )
 
         return InsightsQuestionnairesInstance(self._version, payload)
 
     def stream(
         self,
-        token: Union[str, object] = values.unset,
+        authorization: Union[str, object] = values.unset,
         include_inactive: Union[bool, object] = values.unset,
         limit: Optional[int] = None,
         page_size: Optional[int] = None,
     ) -> Iterator[InsightsQuestionnairesInstance]:
         """
         Streams InsightsQuestionnairesInstance records from the API as a generator stream.
         This operation lazily loads records as efficiently as possible until the limit
         is reached.
         The results are returned as a generator, so this operation is memory efficient.
 
-        :param str token: The Token HTTP request header
+        :param str authorization: The Authorization HTTP request header
         :param bool include_inactive: Flag indicating whether to include inactive questionnaires or not
         :param limit: Upper limit for the number of records to return. stream()
                       guarantees to never return more than limit.  Default is no limit
         :param page_size: Number of records to fetch per request, when not set will use
                           the default value of 50 records.  If no page_size is defined
                           but a limit is defined, stream() will attempt to read the
                           limit with the most efficient page size, i.e. min(limit, 1000)
 
         :returns: Generator that will yield up to limit results
         """
         limits = self._version.read_limits(limit, page_size)
         page = self.page(
-            token=token,
+            authorization=authorization,
             include_inactive=include_inactive,
             page_size=limits["page_size"],
         )
 
         return self._version.stream(page, limits["limit"])
 
     async def stream_async(
         self,
-        token: Union[str, object] = values.unset,
+        authorization: Union[str, object] = values.unset,
         include_inactive: Union[bool, object] = values.unset,
         limit: Optional[int] = None,
         page_size: Optional[int] = None,
     ) -> AsyncIterator[InsightsQuestionnairesInstance]:
         """
         Asynchronously streams InsightsQuestionnairesInstance records from the API as a generator stream.
         This operation lazily loads records as efficiently as possible until the limit
         is reached.
         The results are returned as a generator, so this operation is memory efficient.
 
-        :param str token: The Token HTTP request header
+        :param str authorization: The Authorization HTTP request header
         :param bool include_inactive: Flag indicating whether to include inactive questionnaires or not
         :param limit: Upper limit for the number of records to return. stream()
                       guarantees to never return more than limit.  Default is no limit
         :param page_size: Number of records to fetch per request, when not set will use
                           the default value of 50 records.  If no page_size is defined
                           but a limit is defined, stream() will attempt to read the
                           limit with the most efficient page size, i.e. min(limit, 1000)
 
         :returns: Generator that will yield up to limit results
         """
         limits = self._version.read_limits(limit, page_size)
         page = await self.page_async(
-            token=token,
+            authorization=authorization,
             include_inactive=include_inactive,
             page_size=limits["page_size"],
         )
 
         return self._version.stream_async(page, limits["limit"])
 
     def list(
         self,
-        token: Union[str, object] = values.unset,
+        authorization: Union[str, object] = values.unset,
         include_inactive: Union[bool, object] = values.unset,
         limit: Optional[int] = None,
         page_size: Optional[int] = None,
     ) -> List[InsightsQuestionnairesInstance]:
         """
         Lists InsightsQuestionnairesInstance records from the API as a list.
         Unlike stream(), this operation is eager and will load `limit` records into
         memory before returning.
 
-        :param str token: The Token HTTP request header
+        :param str authorization: The Authorization HTTP request header
         :param bool include_inactive: Flag indicating whether to include inactive questionnaires or not
         :param limit: Upper limit for the number of records to return. list() guarantees
                       never to return more than limit.  Default is no limit
         :param page_size: Number of records to fetch per request, when not set will use
                           the default value of 50 records.  If no page_size is defined
                           but a limit is defined, list() will attempt to read the limit
                           with the most efficient page size, i.e. min(limit, 1000)
 
         :returns: list that will contain up to limit results
         """
         return list(
             self.stream(
-                token=token,
+                authorization=authorization,
                 include_inactive=include_inactive,
                 limit=limit,
                 page_size=page_size,
             )
         )
 
     async def list_async(
         self,
-        token: Union[str, object] = values.unset,
+        authorization: Union[str, object] = values.unset,
         include_inactive: Union[bool, object] = values.unset,
         limit: Optional[int] = None,
         page_size: Optional[int] = None,
     ) -> List[InsightsQuestionnairesInstance]:
         """
         Asynchronously lists InsightsQuestionnairesInstance records from the API as a list.
         Unlike stream(), this operation is eager and will load `limit` records into
         memory before returning.
 
-        :param str token: The Token HTTP request header
+        :param str authorization: The Authorization HTTP request header
         :param bool include_inactive: Flag indicating whether to include inactive questionnaires or not
         :param limit: Upper limit for the number of records to return. list() guarantees
                       never to return more than limit.  Default is no limit
         :param page_size: Number of records to fetch per request, when not set will use
                           the default value of 50 records.  If no page_size is defined
                           but a limit is defined, list() will attempt to read the limit
                           with the most efficient page size, i.e. min(limit, 1000)
 
         :returns: list that will contain up to limit results
         """
         return [
             record
             async for record in await self.stream_async(
-                token=token,
+                authorization=authorization,
                 include_inactive=include_inactive,
                 limit=limit,
                 page_size=page_size,
             )
         ]
 
     def page(
         self,
-        token: Union[str, object] = values.unset,
+        authorization: Union[str, object] = values.unset,
         include_inactive: Union[bool, object] = values.unset,
         page_token: Union[str, object] = values.unset,
         page_number: Union[int, object] = values.unset,
         page_size: Union[int, object] = values.unset,
     ) -> InsightsQuestionnairesPage:
         """
         Retrieve a single page of InsightsQuestionnairesInstance records from the API.
         Request is executed immediately
 
-        :param token: The Token HTTP request header
+        :param authorization: The Authorization HTTP request header
         :param include_inactive: Flag indicating whether to include inactive questionnaires or not
         :param page_token: PageToken provided by the API
         :param page_number: Page Number, this value is simply for client state
         :param page_size: Number of records to return, defaults to 50
 
         :returns: Page of InsightsQuestionnairesInstance
         """
         data = values.of(
             {
-                "Token": token,
+                "Authorization": authorization,
                 "IncludeInactive": include_inactive,
                 "PageToken": page_token,
                 "Page": page_number,
                 "PageSize": page_size,
             }
         )
 
         response = self._version.page(method="GET", uri=self._uri, params=data)
         return InsightsQuestionnairesPage(self._version, response)
 
     async def page_async(
         self,
-        token: Union[str, object] = values.unset,
+        authorization: Union[str, object] = values.unset,
         include_inactive: Union[bool, object] = values.unset,
         page_token: Union[str, object] = values.unset,
         page_number: Union[int, object] = values.unset,
         page_size: Union[int, object] = values.unset,
     ) -> InsightsQuestionnairesPage:
         """
         Asynchronously retrieve a single page of InsightsQuestionnairesInstance records from the API.
         Request is executed immediately
 
-        :param token: The Token HTTP request header
+        :param authorization: The Authorization HTTP request header
         :param include_inactive: Flag indicating whether to include inactive questionnaires or not
         :param page_token: PageToken provided by the API
         :param page_number: Page Number, this value is simply for client state
         :param page_size: Number of records to return, defaults to 50
 
         :returns: Page of InsightsQuestionnairesInstance
         """
         data = values.of(
             {
-                "Token": token,
+                "Authorization": authorization,
                 "IncludeInactive": include_inactive,
                 "PageToken": page_token,
                 "Page": page_number,
                 "PageSize": page_size,
             }
         )
```

### Comparing `twilio-8.2.0/twilio/rest/flex_api/v1/insights_questionnaires_category.py` & `twilio-8.2.1/twilio/rest/flex_api/v1/insights_questionnaires_category.py`

 * *Files 12% similar despite different names*

```diff
@@ -60,68 +60,70 @@
         if self._context is None:
             self._context = InsightsQuestionnairesCategoryContext(
                 self._version,
                 category_sid=self._solution["category_sid"],
             )
         return self._context
 
-    def delete(self, token: Union[str, object] = values.unset) -> bool:
+    def delete(self, authorization: Union[str, object] = values.unset) -> bool:
         """
         Deletes the InsightsQuestionnairesCategoryInstance
 
-        :param token: The Token HTTP request header
+        :param authorization: The Authorization HTTP request header
 
         :returns: True if delete succeeds, False otherwise
         """
         return self._proxy.delete(
-            token=token,
+            authorization=authorization,
         )
 
-    async def delete_async(self, token: Union[str, object] = values.unset) -> bool:
+    async def delete_async(
+        self, authorization: Union[str, object] = values.unset
+    ) -> bool:
         """
         Asynchronous coroutine that deletes the InsightsQuestionnairesCategoryInstance
 
-        :param token: The Token HTTP request header
+        :param authorization: The Authorization HTTP request header
 
         :returns: True if delete succeeds, False otherwise
         """
         return await self._proxy.delete_async(
-            token=token,
+            authorization=authorization,
         )
 
     def update(
-        self, name: str, token: Union[str, object] = values.unset
+        self, name: str, authorization: Union[str, object] = values.unset
     ) -> "InsightsQuestionnairesCategoryInstance":
         """
         Update the InsightsQuestionnairesCategoryInstance
 
         :param name: The name of this category.
-        :param token: The Token HTTP request header
+        :param authorization: The Authorization HTTP request header
 
         :returns: The updated InsightsQuestionnairesCategoryInstance
         """
         return self._proxy.update(
             name=name,
-            token=token,
+            authorization=authorization,
         )
 
     async def update_async(
-        self, name: str, token: Union[str, object] = values.unset
+        self, name: str, authorization: Union[str, object] = values.unset
     ) -> "InsightsQuestionnairesCategoryInstance":
         """
         Asynchronous coroutine to update the InsightsQuestionnairesCategoryInstance
 
         :param name: The name of this category.
-        :param token: The Token HTTP request header
+        :param authorization: The Authorization HTTP request header
 
         :returns: The updated InsightsQuestionnairesCategoryInstance
         """
         return await self._proxy.update_async(
             name=name,
-            token=token,
+            authorization=authorization,
         )
 
     def __repr__(self) -> str:
         """
         Provide a friendly representation
 
         :returns: Machine friendly representation
@@ -146,97 +148,99 @@
         self._solution = {
             "category_sid": category_sid,
         }
         self._uri = "/Insights/QualityManagement/Categories/{category_sid}".format(
             **self._solution
         )
 
-    def delete(self, token: Union[str, object] = values.unset) -> bool:
+    def delete(self, authorization: Union[str, object] = values.unset) -> bool:
         """
         Deletes the InsightsQuestionnairesCategoryInstance
 
-        :param token: The Token HTTP request header
+        :param authorization: The Authorization HTTP request header
 
         :returns: True if delete succeeds, False otherwise
         """
         headers = values.of(
             {
-                "Token": token,
+                "Authorization": authorization,
             }
         )
 
         return self._version.delete(method="DELETE", uri=self._uri, headers=headers)
 
-    async def delete_async(self, token: Union[str, object] = values.unset) -> bool:
+    async def delete_async(
+        self, authorization: Union[str, object] = values.unset
+    ) -> bool:
         """
         Asynchronous coroutine that deletes the InsightsQuestionnairesCategoryInstance
 
-        :param token: The Token HTTP request header
+        :param authorization: The Authorization HTTP request header
 
         :returns: True if delete succeeds, False otherwise
         """
         headers = values.of(
             {
-                "Token": token,
+                "Authorization": authorization,
             }
         )
 
         return await self._version.delete_async(
             method="DELETE", uri=self._uri, headers=headers
         )
 
     def update(
-        self, name: str, token: Union[str, object] = values.unset
+        self, name: str, authorization: Union[str, object] = values.unset
     ) -> InsightsQuestionnairesCategoryInstance:
         """
         Update the InsightsQuestionnairesCategoryInstance
 
         :param name: The name of this category.
-        :param token: The Token HTTP request header
+        :param authorization: The Authorization HTTP request header
 
         :returns: The updated InsightsQuestionnairesCategoryInstance
         """
         data = values.of(
             {
                 "Name": name,
             }
         )
         headers = values.of(
             {
-                "Token": token,
+                "Authorization": authorization,
             }
         )
 
         payload = self._version.update(
             method="POST", uri=self._uri, data=data, headers=headers
         )
 
         return InsightsQuestionnairesCategoryInstance(
             self._version, payload, category_sid=self._solution["category_sid"]
         )
 
     async def update_async(
-        self, name: str, token: Union[str, object] = values.unset
+        self, name: str, authorization: Union[str, object] = values.unset
     ) -> InsightsQuestionnairesCategoryInstance:
         """
         Asynchronous coroutine to update the InsightsQuestionnairesCategoryInstance
 
         :param name: The name of this category.
-        :param token: The Token HTTP request header
+        :param authorization: The Authorization HTTP request header
 
         :returns: The updated InsightsQuestionnairesCategoryInstance
         """
         data = values.of(
             {
                 "Name": name,
             }
         )
         headers = values.of(
             {
-                "Token": token,
+                "Authorization": authorization,
             }
         )
 
         payload = await self._version.update_async(
             method="POST", uri=self._uri, data=data, headers=headers
         )
 
@@ -285,231 +289,233 @@
 
         """
         super().__init__(version)
 
         self._uri = "/Insights/QualityManagement/Categories"
 
     def create(
-        self, name: str, token: Union[str, object] = values.unset
+        self, name: str, authorization: Union[str, object] = values.unset
     ) -> InsightsQuestionnairesCategoryInstance:
         """
         Create the InsightsQuestionnairesCategoryInstance
 
         :param name: The name of this category.
-        :param token: The Token HTTP request header
+        :param authorization: The Authorization HTTP request header
 
         :returns: The created InsightsQuestionnairesCategoryInstance
         """
         data = values.of(
             {
                 "Name": name,
             }
         )
         headers = values.of(
             {
-                "Token": token,
+                "Authorization": authorization,
             }
         )
         payload = self._version.create(
             method="POST", uri=self._uri, data=data, headers=headers
         )
 
         return InsightsQuestionnairesCategoryInstance(self._version, payload)
 
     async def create_async(
-        self, name: str, token: Union[str, object] = values.unset
+        self, name: str, authorization: Union[str, object] = values.unset
     ) -> InsightsQuestionnairesCategoryInstance:
         """
         Asynchronously create the InsightsQuestionnairesCategoryInstance
 
         :param name: The name of this category.
-        :param token: The Token HTTP request header
+        :param authorization: The Authorization HTTP request header
 
         :returns: The created InsightsQuestionnairesCategoryInstance
         """
         data = values.of(
             {
                 "Name": name,
             }
         )
         headers = values.of(
             {
-                "Token": token,
+                "Authorization": authorization,
             }
         )
         payload = await self._version.create_async(
             method="POST", uri=self._uri, data=data, headers=headers
         )
 
         return InsightsQuestionnairesCategoryInstance(self._version, payload)
 
     def stream(
         self,
-        token: Union[str, object] = values.unset,
+        authorization: Union[str, object] = values.unset,
         limit: Optional[int] = None,
         page_size: Optional[int] = None,
     ) -> Iterator[InsightsQuestionnairesCategoryInstance]:
         """
         Streams InsightsQuestionnairesCategoryInstance records from the API as a generator stream.
         This operation lazily loads records as efficiently as possible until the limit
         is reached.
         The results are returned as a generator, so this operation is memory efficient.
 
-        :param str token: The Token HTTP request header
+        :param str authorization: The Authorization HTTP request header
         :param limit: Upper limit for the number of records to return. stream()
                       guarantees to never return more than limit.  Default is no limit
         :param page_size: Number of records to fetch per request, when not set will use
                           the default value of 50 records.  If no page_size is defined
                           but a limit is defined, stream() will attempt to read the
                           limit with the most efficient page size, i.e. min(limit, 1000)
 
         :returns: Generator that will yield up to limit results
         """
         limits = self._version.read_limits(limit, page_size)
-        page = self.page(token=token, page_size=limits["page_size"])
+        page = self.page(authorization=authorization, page_size=limits["page_size"])
 
         return self._version.stream(page, limits["limit"])
 
     async def stream_async(
         self,
-        token: Union[str, object] = values.unset,
+        authorization: Union[str, object] = values.unset,
         limit: Optional[int] = None,
         page_size: Optional[int] = None,
     ) -> AsyncIterator[InsightsQuestionnairesCategoryInstance]:
         """
         Asynchronously streams InsightsQuestionnairesCategoryInstance records from the API as a generator stream.
         This operation lazily loads records as efficiently as possible until the limit
         is reached.
         The results are returned as a generator, so this operation is memory efficient.
 
-        :param str token: The Token HTTP request header
+        :param str authorization: The Authorization HTTP request header
         :param limit: Upper limit for the number of records to return. stream()
                       guarantees to never return more than limit.  Default is no limit
         :param page_size: Number of records to fetch per request, when not set will use
                           the default value of 50 records.  If no page_size is defined
                           but a limit is defined, stream() will attempt to read the
                           limit with the most efficient page size, i.e. min(limit, 1000)
 
         :returns: Generator that will yield up to limit results
         """
         limits = self._version.read_limits(limit, page_size)
-        page = await self.page_async(token=token, page_size=limits["page_size"])
+        page = await self.page_async(
+            authorization=authorization, page_size=limits["page_size"]
+        )
 
         return self._version.stream_async(page, limits["limit"])
 
     def list(
         self,
-        token: Union[str, object] = values.unset,
+        authorization: Union[str, object] = values.unset,
         limit: Optional[int] = None,
         page_size: Optional[int] = None,
     ) -> List[InsightsQuestionnairesCategoryInstance]:
         """
         Lists InsightsQuestionnairesCategoryInstance records from the API as a list.
         Unlike stream(), this operation is eager and will load `limit` records into
         memory before returning.
 
-        :param str token: The Token HTTP request header
+        :param str authorization: The Authorization HTTP request header
         :param limit: Upper limit for the number of records to return. list() guarantees
                       never to return more than limit.  Default is no limit
         :param page_size: Number of records to fetch per request, when not set will use
                           the default value of 50 records.  If no page_size is defined
                           but a limit is defined, list() will attempt to read the limit
                           with the most efficient page size, i.e. min(limit, 1000)
 
         :returns: list that will contain up to limit results
         """
         return list(
             self.stream(
-                token=token,
+                authorization=authorization,
                 limit=limit,
                 page_size=page_size,
             )
         )
 
     async def list_async(
         self,
-        token: Union[str, object] = values.unset,
+        authorization: Union[str, object] = values.unset,
         limit: Optional[int] = None,
         page_size: Optional[int] = None,
     ) -> List[InsightsQuestionnairesCategoryInstance]:
         """
         Asynchronously lists InsightsQuestionnairesCategoryInstance records from the API as a list.
         Unlike stream(), this operation is eager and will load `limit` records into
         memory before returning.
 
-        :param str token: The Token HTTP request header
+        :param str authorization: The Authorization HTTP request header
         :param limit: Upper limit for the number of records to return. list() guarantees
                       never to return more than limit.  Default is no limit
         :param page_size: Number of records to fetch per request, when not set will use
                           the default value of 50 records.  If no page_size is defined
                           but a limit is defined, list() will attempt to read the limit
                           with the most efficient page size, i.e. min(limit, 1000)
 
         :returns: list that will contain up to limit results
         """
         return [
             record
             async for record in await self.stream_async(
-                token=token,
+                authorization=authorization,
                 limit=limit,
                 page_size=page_size,
             )
         ]
 
     def page(
         self,
-        token: Union[str, object] = values.unset,
+        authorization: Union[str, object] = values.unset,
         page_token: Union[str, object] = values.unset,
         page_number: Union[int, object] = values.unset,
         page_size: Union[int, object] = values.unset,
     ) -> InsightsQuestionnairesCategoryPage:
         """
         Retrieve a single page of InsightsQuestionnairesCategoryInstance records from the API.
         Request is executed immediately
 
-        :param token: The Token HTTP request header
+        :param authorization: The Authorization HTTP request header
         :param page_token: PageToken provided by the API
         :param page_number: Page Number, this value is simply for client state
         :param page_size: Number of records to return, defaults to 50
 
         :returns: Page of InsightsQuestionnairesCategoryInstance
         """
         data = values.of(
             {
-                "Token": token,
+                "Authorization": authorization,
                 "PageToken": page_token,
                 "Page": page_number,
                 "PageSize": page_size,
             }
         )
 
         response = self._version.page(method="GET", uri=self._uri, params=data)
         return InsightsQuestionnairesCategoryPage(self._version, response)
 
     async def page_async(
         self,
-        token: Union[str, object] = values.unset,
+        authorization: Union[str, object] = values.unset,
         page_token: Union[str, object] = values.unset,
         page_number: Union[int, object] = values.unset,
         page_size: Union[int, object] = values.unset,
     ) -> InsightsQuestionnairesCategoryPage:
         """
         Asynchronously retrieve a single page of InsightsQuestionnairesCategoryInstance records from the API.
         Request is executed immediately
 
-        :param token: The Token HTTP request header
+        :param authorization: The Authorization HTTP request header
         :param page_token: PageToken provided by the API
         :param page_number: Page Number, this value is simply for client state
         :param page_size: Number of records to return, defaults to 50
 
         :returns: Page of InsightsQuestionnairesCategoryInstance
         """
         data = values.of(
             {
-                "Token": token,
+                "Authorization": authorization,
                 "PageToken": page_token,
                 "Page": page_number,
                 "PageSize": page_size,
             }
         )
 
         response = await self._version.page_async(
```

### Comparing `twilio-8.2.0/twilio/rest/flex_api/v1/insights_questionnaires_question.py` & `twilio-8.2.1/twilio/rest/flex_api/v1/insights_questionnaires_question.py`

 * *Files 16% similar despite different names*

```diff
@@ -72,92 +72,94 @@
         if self._context is None:
             self._context = InsightsQuestionnairesQuestionContext(
                 self._version,
                 question_sid=self._solution["question_sid"],
             )
         return self._context
 
-    def delete(self, token: Union[str, object] = values.unset) -> bool:
+    def delete(self, authorization: Union[str, object] = values.unset) -> bool:
         """
         Deletes the InsightsQuestionnairesQuestionInstance
 
-        :param token: The Token HTTP request header
+        :param authorization: The Authorization HTTP request header
 
         :returns: True if delete succeeds, False otherwise
         """
         return self._proxy.delete(
-            token=token,
+            authorization=authorization,
         )
 
-    async def delete_async(self, token: Union[str, object] = values.unset) -> bool:
+    async def delete_async(
+        self, authorization: Union[str, object] = values.unset
+    ) -> bool:
         """
         Asynchronous coroutine that deletes the InsightsQuestionnairesQuestionInstance
 
-        :param token: The Token HTTP request header
+        :param authorization: The Authorization HTTP request header
 
         :returns: True if delete succeeds, False otherwise
         """
         return await self._proxy.delete_async(
-            token=token,
+            authorization=authorization,
         )
 
     def update(
         self,
         allow_na: bool,
-        token: Union[str, object] = values.unset,
+        authorization: Union[str, object] = values.unset,
         category_sid: Union[str, object] = values.unset,
         question: Union[str, object] = values.unset,
         description: Union[str, object] = values.unset,
         answer_set_id: Union[str, object] = values.unset,
     ) -> "InsightsQuestionnairesQuestionInstance":
         """
         Update the InsightsQuestionnairesQuestionInstance
 
         :param allow_na: The flag to enable for disable NA for answer.
-        :param token: The Token HTTP request header
+        :param authorization: The Authorization HTTP request header
         :param category_sid: The SID of the category
         :param question: The question.
         :param description: The description for the question.
         :param answer_set_id: The answer_set for the question.
 
         :returns: The updated InsightsQuestionnairesQuestionInstance
         """
         return self._proxy.update(
             allow_na=allow_na,
-            token=token,
+            authorization=authorization,
             category_sid=category_sid,
             question=question,
             description=description,
             answer_set_id=answer_set_id,
         )
 
     async def update_async(
         self,
         allow_na: bool,
-        token: Union[str, object] = values.unset,
+        authorization: Union[str, object] = values.unset,
         category_sid: Union[str, object] = values.unset,
         question: Union[str, object] = values.unset,
         description: Union[str, object] = values.unset,
         answer_set_id: Union[str, object] = values.unset,
     ) -> "InsightsQuestionnairesQuestionInstance":
         """
         Asynchronous coroutine to update the InsightsQuestionnairesQuestionInstance
 
         :param allow_na: The flag to enable for disable NA for answer.
-        :param token: The Token HTTP request header
+        :param authorization: The Authorization HTTP request header
         :param category_sid: The SID of the category
         :param question: The question.
         :param description: The description for the question.
         :param answer_set_id: The answer_set for the question.
 
         :returns: The updated InsightsQuestionnairesQuestionInstance
         """
         return await self._proxy.update_async(
             allow_na=allow_na,
-            token=token,
+            authorization=authorization,
             category_sid=category_sid,
             question=question,
             description=description,
             answer_set_id=answer_set_id,
         )
 
     def __repr__(self) -> str:
@@ -186,62 +188,64 @@
         self._solution = {
             "question_sid": question_sid,
         }
         self._uri = "/Insights/QualityManagement/Questions/{question_sid}".format(
             **self._solution
         )
 
-    def delete(self, token: Union[str, object] = values.unset) -> bool:
+    def delete(self, authorization: Union[str, object] = values.unset) -> bool:
         """
         Deletes the InsightsQuestionnairesQuestionInstance
 
-        :param token: The Token HTTP request header
+        :param authorization: The Authorization HTTP request header
 
         :returns: True if delete succeeds, False otherwise
         """
         headers = values.of(
             {
-                "Token": token,
+                "Authorization": authorization,
             }
         )
 
         return self._version.delete(method="DELETE", uri=self._uri, headers=headers)
 
-    async def delete_async(self, token: Union[str, object] = values.unset) -> bool:
+    async def delete_async(
+        self, authorization: Union[str, object] = values.unset
+    ) -> bool:
         """
         Asynchronous coroutine that deletes the InsightsQuestionnairesQuestionInstance
 
-        :param token: The Token HTTP request header
+        :param authorization: The Authorization HTTP request header
 
         :returns: True if delete succeeds, False otherwise
         """
         headers = values.of(
             {
-                "Token": token,
+                "Authorization": authorization,
             }
         )
 
         return await self._version.delete_async(
             method="DELETE", uri=self._uri, headers=headers
         )
 
     def update(
         self,
         allow_na: bool,
-        token: Union[str, object] = values.unset,
+        authorization: Union[str, object] = values.unset,
         category_sid: Union[str, object] = values.unset,
         question: Union[str, object] = values.unset,
         description: Union[str, object] = values.unset,
         answer_set_id: Union[str, object] = values.unset,
     ) -> InsightsQuestionnairesQuestionInstance:
         """
         Update the InsightsQuestionnairesQuestionInstance
 
         :param allow_na: The flag to enable for disable NA for answer.
-        :param token: The Token HTTP request header
+        :param authorization: The Authorization HTTP request header
         :param category_sid: The SID of the category
         :param question: The question.
         :param description: The description for the question.
         :param answer_set_id: The answer_set for the question.
 
         :returns: The updated InsightsQuestionnairesQuestionInstance
         """
@@ -252,40 +256,40 @@
                 "Question": question,
                 "Description": description,
                 "AnswerSetId": answer_set_id,
             }
         )
         headers = values.of(
             {
-                "Token": token,
+                "Authorization": authorization,
             }
         )
 
         payload = self._version.update(
             method="POST", uri=self._uri, data=data, headers=headers
         )
 
         return InsightsQuestionnairesQuestionInstance(
             self._version, payload, question_sid=self._solution["question_sid"]
         )
 
     async def update_async(
         self,
         allow_na: bool,
-        token: Union[str, object] = values.unset,
+        authorization: Union[str, object] = values.unset,
         category_sid: Union[str, object] = values.unset,
         question: Union[str, object] = values.unset,
         description: Union[str, object] = values.unset,
         answer_set_id: Union[str, object] = values.unset,
     ) -> InsightsQuestionnairesQuestionInstance:
         """
         Asynchronous coroutine to update the InsightsQuestionnairesQuestionInstance
 
         :param allow_na: The flag to enable for disable NA for answer.
-        :param token: The Token HTTP request header
+        :param authorization: The Authorization HTTP request header
         :param category_sid: The SID of the category
         :param question: The question.
         :param description: The description for the question.
         :param answer_set_id: The answer_set for the question.
 
         :returns: The updated InsightsQuestionnairesQuestionInstance
         """
@@ -296,15 +300,15 @@
                 "Question": question,
                 "Description": description,
                 "AnswerSetId": answer_set_id,
             }
         )
         headers = values.of(
             {
-                "Token": token,
+                "Authorization": authorization,
             }
         )
 
         payload = await self._version.update_async(
             method="POST", uri=self._uri, data=data, headers=headers
         )
 
@@ -358,25 +362,25 @@
 
     def create(
         self,
         category_sid: str,
         question: str,
         answer_set_id: str,
         allow_na: bool,
-        token: Union[str, object] = values.unset,
+        authorization: Union[str, object] = values.unset,
         description: Union[str, object] = values.unset,
     ) -> InsightsQuestionnairesQuestionInstance:
         """
         Create the InsightsQuestionnairesQuestionInstance
 
         :param category_sid: The SID of the category
         :param question: The question.
         :param answer_set_id: The answer_set for the question.
         :param allow_na: The flag to enable for disable NA for answer.
-        :param token: The Token HTTP request header
+        :param authorization: The Authorization HTTP request header
         :param description: The description for the question.
 
         :returns: The created InsightsQuestionnairesQuestionInstance
         """
         data = values.of(
             {
                 "CategorySid": category_sid,
@@ -384,40 +388,40 @@
                 "AnswerSetId": answer_set_id,
                 "AllowNa": allow_na,
                 "Description": description,
             }
         )
         headers = values.of(
             {
-                "Token": token,
+                "Authorization": authorization,
             }
         )
         payload = self._version.create(
             method="POST", uri=self._uri, data=data, headers=headers
         )
 
         return InsightsQuestionnairesQuestionInstance(self._version, payload)
 
     async def create_async(
         self,
         category_sid: str,
         question: str,
         answer_set_id: str,
         allow_na: bool,
-        token: Union[str, object] = values.unset,
+        authorization: Union[str, object] = values.unset,
         description: Union[str, object] = values.unset,
     ) -> InsightsQuestionnairesQuestionInstance:
         """
         Asynchronously create the InsightsQuestionnairesQuestionInstance
 
         :param category_sid: The SID of the category
         :param question: The question.
         :param answer_set_id: The answer_set for the question.
         :param allow_na: The flag to enable for disable NA for answer.
-        :param token: The Token HTTP request header
+        :param authorization: The Authorization HTTP request header
         :param description: The description for the question.
 
         :returns: The created InsightsQuestionnairesQuestionInstance
         """
         data = values.of(
             {
                 "CategorySid": category_sid,
@@ -425,206 +429,210 @@
                 "AnswerSetId": answer_set_id,
                 "AllowNa": allow_na,
                 "Description": description,
             }
         )
         headers = values.of(
             {
-                "Token": token,
+                "Authorization": authorization,
             }
         )
         payload = await self._version.create_async(
             method="POST", uri=self._uri, data=data, headers=headers
         )
 
         return InsightsQuestionnairesQuestionInstance(self._version, payload)
 
     def stream(
         self,
-        token: Union[str, object] = values.unset,
+        authorization: Union[str, object] = values.unset,
         category_sid: Union[List[str], object] = values.unset,
         limit: Optional[int] = None,
         page_size: Optional[int] = None,
     ) -> Iterator[InsightsQuestionnairesQuestionInstance]:
         """
         Streams InsightsQuestionnairesQuestionInstance records from the API as a generator stream.
         This operation lazily loads records as efficiently as possible until the limit
         is reached.
         The results are returned as a generator, so this operation is memory efficient.
 
-        :param str token: The Token HTTP request header
+        :param str authorization: The Authorization HTTP request header
         :param List[str] category_sid: The list of category SIDs
         :param limit: Upper limit for the number of records to return. stream()
                       guarantees to never return more than limit.  Default is no limit
         :param page_size: Number of records to fetch per request, when not set will use
                           the default value of 50 records.  If no page_size is defined
                           but a limit is defined, stream() will attempt to read the
                           limit with the most efficient page size, i.e. min(limit, 1000)
 
         :returns: Generator that will yield up to limit results
         """
         limits = self._version.read_limits(limit, page_size)
         page = self.page(
-            token=token, category_sid=category_sid, page_size=limits["page_size"]
+            authorization=authorization,
+            category_sid=category_sid,
+            page_size=limits["page_size"],
         )
 
         return self._version.stream(page, limits["limit"])
 
     async def stream_async(
         self,
-        token: Union[str, object] = values.unset,
+        authorization: Union[str, object] = values.unset,
         category_sid: Union[List[str], object] = values.unset,
         limit: Optional[int] = None,
         page_size: Optional[int] = None,
     ) -> AsyncIterator[InsightsQuestionnairesQuestionInstance]:
         """
         Asynchronously streams InsightsQuestionnairesQuestionInstance records from the API as a generator stream.
         This operation lazily loads records as efficiently as possible until the limit
         is reached.
         The results are returned as a generator, so this operation is memory efficient.
 
-        :param str token: The Token HTTP request header
+        :param str authorization: The Authorization HTTP request header
         :param List[str] category_sid: The list of category SIDs
         :param limit: Upper limit for the number of records to return. stream()
                       guarantees to never return more than limit.  Default is no limit
         :param page_size: Number of records to fetch per request, when not set will use
                           the default value of 50 records.  If no page_size is defined
                           but a limit is defined, stream() will attempt to read the
                           limit with the most efficient page size, i.e. min(limit, 1000)
 
         :returns: Generator that will yield up to limit results
         """
         limits = self._version.read_limits(limit, page_size)
         page = await self.page_async(
-            token=token, category_sid=category_sid, page_size=limits["page_size"]
+            authorization=authorization,
+            category_sid=category_sid,
+            page_size=limits["page_size"],
         )
 
         return self._version.stream_async(page, limits["limit"])
 
     def list(
         self,
-        token: Union[str, object] = values.unset,
+        authorization: Union[str, object] = values.unset,
         category_sid: Union[List[str], object] = values.unset,
         limit: Optional[int] = None,
         page_size: Optional[int] = None,
     ) -> List[InsightsQuestionnairesQuestionInstance]:
         """
         Lists InsightsQuestionnairesQuestionInstance records from the API as a list.
         Unlike stream(), this operation is eager and will load `limit` records into
         memory before returning.
 
-        :param str token: The Token HTTP request header
+        :param str authorization: The Authorization HTTP request header
         :param List[str] category_sid: The list of category SIDs
         :param limit: Upper limit for the number of records to return. list() guarantees
                       never to return more than limit.  Default is no limit
         :param page_size: Number of records to fetch per request, when not set will use
                           the default value of 50 records.  If no page_size is defined
                           but a limit is defined, list() will attempt to read the limit
                           with the most efficient page size, i.e. min(limit, 1000)
 
         :returns: list that will contain up to limit results
         """
         return list(
             self.stream(
-                token=token,
+                authorization=authorization,
                 category_sid=category_sid,
                 limit=limit,
                 page_size=page_size,
             )
         )
 
     async def list_async(
         self,
-        token: Union[str, object] = values.unset,
+        authorization: Union[str, object] = values.unset,
         category_sid: Union[List[str], object] = values.unset,
         limit: Optional[int] = None,
         page_size: Optional[int] = None,
     ) -> List[InsightsQuestionnairesQuestionInstance]:
         """
         Asynchronously lists InsightsQuestionnairesQuestionInstance records from the API as a list.
         Unlike stream(), this operation is eager and will load `limit` records into
         memory before returning.
 
-        :param str token: The Token HTTP request header
+        :param str authorization: The Authorization HTTP request header
         :param List[str] category_sid: The list of category SIDs
         :param limit: Upper limit for the number of records to return. list() guarantees
                       never to return more than limit.  Default is no limit
         :param page_size: Number of records to fetch per request, when not set will use
                           the default value of 50 records.  If no page_size is defined
                           but a limit is defined, list() will attempt to read the limit
                           with the most efficient page size, i.e. min(limit, 1000)
 
         :returns: list that will contain up to limit results
         """
         return [
             record
             async for record in await self.stream_async(
-                token=token,
+                authorization=authorization,
                 category_sid=category_sid,
                 limit=limit,
                 page_size=page_size,
             )
         ]
 
     def page(
         self,
-        token: Union[str, object] = values.unset,
+        authorization: Union[str, object] = values.unset,
         category_sid: Union[List[str], object] = values.unset,
         page_token: Union[str, object] = values.unset,
         page_number: Union[int, object] = values.unset,
         page_size: Union[int, object] = values.unset,
     ) -> InsightsQuestionnairesQuestionPage:
         """
         Retrieve a single page of InsightsQuestionnairesQuestionInstance records from the API.
         Request is executed immediately
 
-        :param token: The Token HTTP request header
+        :param authorization: The Authorization HTTP request header
         :param category_sid: The list of category SIDs
         :param page_token: PageToken provided by the API
         :param page_number: Page Number, this value is simply for client state
         :param page_size: Number of records to return, defaults to 50
 
         :returns: Page of InsightsQuestionnairesQuestionInstance
         """
         data = values.of(
             {
-                "Token": token,
+                "Authorization": authorization,
                 "CategorySid": serialize.map(category_sid, lambda e: e),
                 "PageToken": page_token,
                 "Page": page_number,
                 "PageSize": page_size,
             }
         )
 
         response = self._version.page(method="GET", uri=self._uri, params=data)
         return InsightsQuestionnairesQuestionPage(self._version, response)
 
     async def page_async(
         self,
-        token: Union[str, object] = values.unset,
+        authorization: Union[str, object] = values.unset,
         category_sid: Union[List[str], object] = values.unset,
         page_token: Union[str, object] = values.unset,
         page_number: Union[int, object] = values.unset,
         page_size: Union[int, object] = values.unset,
     ) -> InsightsQuestionnairesQuestionPage:
         """
         Asynchronously retrieve a single page of InsightsQuestionnairesQuestionInstance records from the API.
         Request is executed immediately
 
-        :param token: The Token HTTP request header
+        :param authorization: The Authorization HTTP request header
         :param category_sid: The list of category SIDs
         :param page_token: PageToken provided by the API
         :param page_number: Page Number, this value is simply for client state
         :param page_size: Number of records to return, defaults to 50
 
         :returns: Page of InsightsQuestionnairesQuestionInstance
         """
         data = values.of(
             {
-                "Token": token,
+                "Authorization": authorization,
                 "CategorySid": serialize.map(category_sid, lambda e: e),
                 "PageToken": page_token,
                 "Page": page_number,
                 "PageSize": page_size,
             }
         )
```

### Comparing `twilio-8.2.0/twilio/rest/flex_api/v1/insights_segments.py` & `twilio-8.2.1/twilio/rest/flex_api/v1/insights_segments.py`

 * *Files 8% similar despite different names*

```diff
@@ -123,216 +123,216 @@
         """
         super().__init__(version)
 
         self._uri = "/Insights/Segments"
 
     def stream(
         self,
-        token: Union[str, object] = values.unset,
+        authorization: Union[str, object] = values.unset,
         segment_id: Union[str, object] = values.unset,
         reservation_id: Union[List[str], object] = values.unset,
         limit: Optional[int] = None,
         page_size: Optional[int] = None,
     ) -> Iterator[InsightsSegmentsInstance]:
         """
         Streams InsightsSegmentsInstance records from the API as a generator stream.
         This operation lazily loads records as efficiently as possible until the limit
         is reached.
         The results are returned as a generator, so this operation is memory efficient.
 
-        :param str token: The Token HTTP request header
+        :param str authorization: The Authorization HTTP request header
         :param str segment_id: To unique id of the segment
         :param List[str] reservation_id: The list of reservation Ids
         :param limit: Upper limit for the number of records to return. stream()
                       guarantees to never return more than limit.  Default is no limit
         :param page_size: Number of records to fetch per request, when not set will use
                           the default value of 50 records.  If no page_size is defined
                           but a limit is defined, stream() will attempt to read the
                           limit with the most efficient page size, i.e. min(limit, 1000)
 
         :returns: Generator that will yield up to limit results
         """
         limits = self._version.read_limits(limit, page_size)
         page = self.page(
-            token=token,
+            authorization=authorization,
             segment_id=segment_id,
             reservation_id=reservation_id,
             page_size=limits["page_size"],
         )
 
         return self._version.stream(page, limits["limit"])
 
     async def stream_async(
         self,
-        token: Union[str, object] = values.unset,
+        authorization: Union[str, object] = values.unset,
         segment_id: Union[str, object] = values.unset,
         reservation_id: Union[List[str], object] = values.unset,
         limit: Optional[int] = None,
         page_size: Optional[int] = None,
     ) -> AsyncIterator[InsightsSegmentsInstance]:
         """
         Asynchronously streams InsightsSegmentsInstance records from the API as a generator stream.
         This operation lazily loads records as efficiently as possible until the limit
         is reached.
         The results are returned as a generator, so this operation is memory efficient.
 
-        :param str token: The Token HTTP request header
+        :param str authorization: The Authorization HTTP request header
         :param str segment_id: To unique id of the segment
         :param List[str] reservation_id: The list of reservation Ids
         :param limit: Upper limit for the number of records to return. stream()
                       guarantees to never return more than limit.  Default is no limit
         :param page_size: Number of records to fetch per request, when not set will use
                           the default value of 50 records.  If no page_size is defined
                           but a limit is defined, stream() will attempt to read the
                           limit with the most efficient page size, i.e. min(limit, 1000)
 
         :returns: Generator that will yield up to limit results
         """
         limits = self._version.read_limits(limit, page_size)
         page = await self.page_async(
-            token=token,
+            authorization=authorization,
             segment_id=segment_id,
             reservation_id=reservation_id,
             page_size=limits["page_size"],
         )
 
         return self._version.stream_async(page, limits["limit"])
 
     def list(
         self,
-        token: Union[str, object] = values.unset,
+        authorization: Union[str, object] = values.unset,
         segment_id: Union[str, object] = values.unset,
         reservation_id: Union[List[str], object] = values.unset,
         limit: Optional[int] = None,
         page_size: Optional[int] = None,
     ) -> List[InsightsSegmentsInstance]:
         """
         Lists InsightsSegmentsInstance records from the API as a list.
         Unlike stream(), this operation is eager and will load `limit` records into
         memory before returning.
 
-        :param str token: The Token HTTP request header
+        :param str authorization: The Authorization HTTP request header
         :param str segment_id: To unique id of the segment
         :param List[str] reservation_id: The list of reservation Ids
         :param limit: Upper limit for the number of records to return. list() guarantees
                       never to return more than limit.  Default is no limit
         :param page_size: Number of records to fetch per request, when not set will use
                           the default value of 50 records.  If no page_size is defined
                           but a limit is defined, list() will attempt to read the limit
                           with the most efficient page size, i.e. min(limit, 1000)
 
         :returns: list that will contain up to limit results
         """
         return list(
             self.stream(
-                token=token,
+                authorization=authorization,
                 segment_id=segment_id,
                 reservation_id=reservation_id,
                 limit=limit,
                 page_size=page_size,
             )
         )
 
     async def list_async(
         self,
-        token: Union[str, object] = values.unset,
+        authorization: Union[str, object] = values.unset,
         segment_id: Union[str, object] = values.unset,
         reservation_id: Union[List[str], object] = values.unset,
         limit: Optional[int] = None,
         page_size: Optional[int] = None,
     ) -> List[InsightsSegmentsInstance]:
         """
         Asynchronously lists InsightsSegmentsInstance records from the API as a list.
         Unlike stream(), this operation is eager and will load `limit` records into
         memory before returning.
 
-        :param str token: The Token HTTP request header
+        :param str authorization: The Authorization HTTP request header
         :param str segment_id: To unique id of the segment
         :param List[str] reservation_id: The list of reservation Ids
         :param limit: Upper limit for the number of records to return. list() guarantees
                       never to return more than limit.  Default is no limit
         :param page_size: Number of records to fetch per request, when not set will use
                           the default value of 50 records.  If no page_size is defined
                           but a limit is defined, list() will attempt to read the limit
                           with the most efficient page size, i.e. min(limit, 1000)
 
         :returns: list that will contain up to limit results
         """
         return [
             record
             async for record in await self.stream_async(
-                token=token,
+                authorization=authorization,
                 segment_id=segment_id,
                 reservation_id=reservation_id,
                 limit=limit,
                 page_size=page_size,
             )
         ]
 
     def page(
         self,
-        token: Union[str, object] = values.unset,
+        authorization: Union[str, object] = values.unset,
         segment_id: Union[str, object] = values.unset,
         reservation_id: Union[List[str], object] = values.unset,
         page_token: Union[str, object] = values.unset,
         page_number: Union[int, object] = values.unset,
         page_size: Union[int, object] = values.unset,
     ) -> InsightsSegmentsPage:
         """
         Retrieve a single page of InsightsSegmentsInstance records from the API.
         Request is executed immediately
 
-        :param token: The Token HTTP request header
+        :param authorization: The Authorization HTTP request header
         :param segment_id: To unique id of the segment
         :param reservation_id: The list of reservation Ids
         :param page_token: PageToken provided by the API
         :param page_number: Page Number, this value is simply for client state
         :param page_size: Number of records to return, defaults to 50
 
         :returns: Page of InsightsSegmentsInstance
         """
         data = values.of(
             {
-                "Token": token,
+                "Authorization": authorization,
                 "SegmentId": segment_id,
                 "ReservationId": serialize.map(reservation_id, lambda e: e),
                 "PageToken": page_token,
                 "Page": page_number,
                 "PageSize": page_size,
             }
         )
 
         response = self._version.page(method="GET", uri=self._uri, params=data)
         return InsightsSegmentsPage(self._version, response)
 
     async def page_async(
         self,
-        token: Union[str, object] = values.unset,
+        authorization: Union[str, object] = values.unset,
         segment_id: Union[str, object] = values.unset,
         reservation_id: Union[List[str], object] = values.unset,
         page_token: Union[str, object] = values.unset,
         page_number: Union[int, object] = values.unset,
         page_size: Union[int, object] = values.unset,
     ) -> InsightsSegmentsPage:
         """
         Asynchronously retrieve a single page of InsightsSegmentsInstance records from the API.
         Request is executed immediately
 
-        :param token: The Token HTTP request header
+        :param authorization: The Authorization HTTP request header
         :param segment_id: To unique id of the segment
         :param reservation_id: The list of reservation Ids
         :param page_token: PageToken provided by the API
         :param page_number: Page Number, this value is simply for client state
         :param page_size: Number of records to return, defaults to 50
 
         :returns: Page of InsightsSegmentsInstance
         """
         data = values.of(
             {
-                "Token": token,
+                "Authorization": authorization,
                 "SegmentId": segment_id,
                 "ReservationId": serialize.map(reservation_id, lambda e: e),
                 "PageToken": page_token,
                 "Page": page_number,
                 "PageSize": page_size,
             }
         )
```

### Comparing `twilio-8.2.0/twilio/rest/flex_api/v1/insights_session.py` & `twilio-8.2.1/twilio/rest/flex_api/v1/insights_session.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/flex_api/v1/insights_settings_answer_sets.py` & `twilio-8.2.1/twilio/rest/flex_api/v1/insights_settings_answer_sets.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/flex_api/v1/insights_settings_comment.py` & `twilio-8.2.1/twilio/rest/flex_api/v1/insights_settings_comment.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/flex_api/v1/insights_user_roles.py` & `twilio-8.2.1/twilio/rest/flex_api/v1/insights_user_roles.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/flex_api/v1/interaction/__init__.py` & `twilio-8.2.1/twilio/rest/flex_api/v1/interaction/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/flex_api/v1/interaction/interaction_channel/__init__.py` & `twilio-8.2.1/twilio/rest/flex_api/v1/interaction/interaction_channel/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/flex_api/v1/interaction/interaction_channel/interaction_channel_invite.py` & `twilio-8.2.1/twilio/rest/flex_api/v1/interaction/interaction_channel/interaction_channel_invite.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/flex_api/v1/interaction/interaction_channel/interaction_channel_participant.py` & `twilio-8.2.1/twilio/rest/flex_api/v1/interaction/interaction_channel/interaction_channel_participant.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/flex_api/v1/web_channel.py` & `twilio-8.2.1/twilio/rest/flex_api/v1/web_channel.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/flex_api/v2/__init__.py` & `twilio-8.2.1/twilio/rest/flex_api/v2/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/flex_api/v2/web_channels.py` & `twilio-8.2.1/twilio/rest/flex_api/v2/web_channels.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/frontline_api/FrontlineApiBase.py` & `twilio-8.2.1/twilio/rest/frontline_api/FrontlineApiBase.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/frontline_api/v1/__init__.py` & `twilio-8.2.1/twilio/rest/frontline_api/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/frontline_api/v1/user.py` & `twilio-8.2.1/twilio/rest/frontline_api/v1/user.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/insights/InsightsBase.py` & `twilio-8.2.1/twilio/rest/insights/InsightsBase.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/insights/__init__.py` & `twilio-8.2.1/twilio/rest/insights/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/insights/v1/__init__.py` & `twilio-8.2.1/twilio/rest/insights/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/insights/v1/call/__init__.py` & `twilio-8.2.1/twilio/rest/insights/v1/call/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/insights/v1/call/annotation.py` & `twilio-8.2.1/twilio/rest/insights/v1/call/annotation.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/insights/v1/call/call_summary.py` & `twilio-8.2.1/twilio/rest/insights/v1/call/call_summary.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/insights/v1/call/event.py` & `twilio-8.2.1/twilio/rest/insights/v1/call/event.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/insights/v1/call/metric.py` & `twilio-8.2.1/twilio/rest/insights/v1/call/metric.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/insights/v1/call_summaries.py` & `twilio-8.2.1/twilio/rest/insights/v1/call_summaries.py`

 * *Files 5% similar despite different names*

```diff
@@ -189,14 +189,18 @@
         processing_state: Union[
             "CallSummariesInstance.ProcessingStateRequest", object
         ] = values.unset,
         sort_by: Union["CallSummariesInstance.SortBy", object] = values.unset,
         subaccount: Union[str, object] = values.unset,
         abnormal_session: Union[bool, object] = values.unset,
         answered_by: Union["CallSummariesInstance.AnsweredBy", object] = values.unset,
+        connectivity_issues: Union[str, object] = values.unset,
+        quality_issues: Union[str, object] = values.unset,
+        spam: Union[bool, object] = values.unset,
+        call_scores: Union[str, object] = values.unset,
         limit: Optional[int] = None,
         page_size: Optional[int] = None,
     ) -> Iterator[CallSummariesInstance]:
         """
         Streams CallSummariesInstance records from the API as a generator stream.
         This operation lazily loads records as efficiently as possible until the limit
         is reached.
@@ -217,14 +221,18 @@
         :param str call_state:
         :param str direction:
         :param &quot;CallSummariesInstance.ProcessingStateRequest&quot; processing_state:
         :param &quot;CallSummariesInstance.SortBy&quot; sort_by:
         :param str subaccount:
         :param bool abnormal_session:
         :param &quot;CallSummariesInstance.AnsweredBy&quot; answered_by:
+        :param str connectivity_issues:
+        :param str quality_issues:
+        :param bool spam:
+        :param str call_scores:
         :param limit: Upper limit for the number of records to return. stream()
                       guarantees to never return more than limit.  Default is no limit
         :param page_size: Number of records to fetch per request, when not set will use
                           the default value of 50 records.  If no page_size is defined
                           but a limit is defined, stream() will attempt to read the
                           limit with the most efficient page size, i.e. min(limit, 1000)
 
@@ -247,14 +255,18 @@
             call_state=call_state,
             direction=direction,
             processing_state=processing_state,
             sort_by=sort_by,
             subaccount=subaccount,
             abnormal_session=abnormal_session,
             answered_by=answered_by,
+            connectivity_issues=connectivity_issues,
+            quality_issues=quality_issues,
+            spam=spam,
+            call_scores=call_scores,
             page_size=limits["page_size"],
         )
 
         return self._version.stream(page, limits["limit"])
 
     async def stream_async(
         self,
@@ -275,14 +287,18 @@
         processing_state: Union[
             "CallSummariesInstance.ProcessingStateRequest", object
         ] = values.unset,
         sort_by: Union["CallSummariesInstance.SortBy", object] = values.unset,
         subaccount: Union[str, object] = values.unset,
         abnormal_session: Union[bool, object] = values.unset,
         answered_by: Union["CallSummariesInstance.AnsweredBy", object] = values.unset,
+        connectivity_issues: Union[str, object] = values.unset,
+        quality_issues: Union[str, object] = values.unset,
+        spam: Union[bool, object] = values.unset,
+        call_scores: Union[str, object] = values.unset,
         limit: Optional[int] = None,
         page_size: Optional[int] = None,
     ) -> AsyncIterator[CallSummariesInstance]:
         """
         Asynchronously streams CallSummariesInstance records from the API as a generator stream.
         This operation lazily loads records as efficiently as possible until the limit
         is reached.
@@ -303,14 +319,18 @@
         :param str call_state:
         :param str direction:
         :param &quot;CallSummariesInstance.ProcessingStateRequest&quot; processing_state:
         :param &quot;CallSummariesInstance.SortBy&quot; sort_by:
         :param str subaccount:
         :param bool abnormal_session:
         :param &quot;CallSummariesInstance.AnsweredBy&quot; answered_by:
+        :param str connectivity_issues:
+        :param str quality_issues:
+        :param bool spam:
+        :param str call_scores:
         :param limit: Upper limit for the number of records to return. stream()
                       guarantees to never return more than limit.  Default is no limit
         :param page_size: Number of records to fetch per request, when not set will use
                           the default value of 50 records.  If no page_size is defined
                           but a limit is defined, stream() will attempt to read the
                           limit with the most efficient page size, i.e. min(limit, 1000)
 
@@ -333,14 +353,18 @@
             call_state=call_state,
             direction=direction,
             processing_state=processing_state,
             sort_by=sort_by,
             subaccount=subaccount,
             abnormal_session=abnormal_session,
             answered_by=answered_by,
+            connectivity_issues=connectivity_issues,
+            quality_issues=quality_issues,
+            spam=spam,
+            call_scores=call_scores,
             page_size=limits["page_size"],
         )
 
         return self._version.stream_async(page, limits["limit"])
 
     def list(
         self,
@@ -361,14 +385,18 @@
         processing_state: Union[
             "CallSummariesInstance.ProcessingStateRequest", object
         ] = values.unset,
         sort_by: Union["CallSummariesInstance.SortBy", object] = values.unset,
         subaccount: Union[str, object] = values.unset,
         abnormal_session: Union[bool, object] = values.unset,
         answered_by: Union["CallSummariesInstance.AnsweredBy", object] = values.unset,
+        connectivity_issues: Union[str, object] = values.unset,
+        quality_issues: Union[str, object] = values.unset,
+        spam: Union[bool, object] = values.unset,
+        call_scores: Union[str, object] = values.unset,
         limit: Optional[int] = None,
         page_size: Optional[int] = None,
     ) -> List[CallSummariesInstance]:
         """
         Lists CallSummariesInstance records from the API as a list.
         Unlike stream(), this operation is eager and will load `limit` records into
         memory before returning.
@@ -388,14 +416,18 @@
         :param str call_state:
         :param str direction:
         :param &quot;CallSummariesInstance.ProcessingStateRequest&quot; processing_state:
         :param &quot;CallSummariesInstance.SortBy&quot; sort_by:
         :param str subaccount:
         :param bool abnormal_session:
         :param &quot;CallSummariesInstance.AnsweredBy&quot; answered_by:
+        :param str connectivity_issues:
+        :param str quality_issues:
+        :param bool spam:
+        :param str call_scores:
         :param limit: Upper limit for the number of records to return. list() guarantees
                       never to return more than limit.  Default is no limit
         :param page_size: Number of records to fetch per request, when not set will use
                           the default value of 50 records.  If no page_size is defined
                           but a limit is defined, list() will attempt to read the limit
                           with the most efficient page size, i.e. min(limit, 1000)
 
@@ -418,14 +450,18 @@
                 call_state=call_state,
                 direction=direction,
                 processing_state=processing_state,
                 sort_by=sort_by,
                 subaccount=subaccount,
                 abnormal_session=abnormal_session,
                 answered_by=answered_by,
+                connectivity_issues=connectivity_issues,
+                quality_issues=quality_issues,
+                spam=spam,
+                call_scores=call_scores,
                 limit=limit,
                 page_size=page_size,
             )
         )
 
     async def list_async(
         self,
@@ -446,14 +482,18 @@
         processing_state: Union[
             "CallSummariesInstance.ProcessingStateRequest", object
         ] = values.unset,
         sort_by: Union["CallSummariesInstance.SortBy", object] = values.unset,
         subaccount: Union[str, object] = values.unset,
         abnormal_session: Union[bool, object] = values.unset,
         answered_by: Union["CallSummariesInstance.AnsweredBy", object] = values.unset,
+        connectivity_issues: Union[str, object] = values.unset,
+        quality_issues: Union[str, object] = values.unset,
+        spam: Union[bool, object] = values.unset,
+        call_scores: Union[str, object] = values.unset,
         limit: Optional[int] = None,
         page_size: Optional[int] = None,
     ) -> List[CallSummariesInstance]:
         """
         Asynchronously lists CallSummariesInstance records from the API as a list.
         Unlike stream(), this operation is eager and will load `limit` records into
         memory before returning.
@@ -473,14 +513,18 @@
         :param str call_state:
         :param str direction:
         :param &quot;CallSummariesInstance.ProcessingStateRequest&quot; processing_state:
         :param &quot;CallSummariesInstance.SortBy&quot; sort_by:
         :param str subaccount:
         :param bool abnormal_session:
         :param &quot;CallSummariesInstance.AnsweredBy&quot; answered_by:
+        :param str connectivity_issues:
+        :param str quality_issues:
+        :param bool spam:
+        :param str call_scores:
         :param limit: Upper limit for the number of records to return. list() guarantees
                       never to return more than limit.  Default is no limit
         :param page_size: Number of records to fetch per request, when not set will use
                           the default value of 50 records.  If no page_size is defined
                           but a limit is defined, list() will attempt to read the limit
                           with the most efficient page size, i.e. min(limit, 1000)
 
@@ -504,14 +548,18 @@
                 call_state=call_state,
                 direction=direction,
                 processing_state=processing_state,
                 sort_by=sort_by,
                 subaccount=subaccount,
                 abnormal_session=abnormal_session,
                 answered_by=answered_by,
+                connectivity_issues=connectivity_issues,
+                quality_issues=quality_issues,
+                spam=spam,
+                call_scores=call_scores,
                 limit=limit,
                 page_size=page_size,
             )
         ]
 
     def page(
         self,
@@ -532,14 +580,18 @@
         processing_state: Union[
             "CallSummariesInstance.ProcessingStateRequest", object
         ] = values.unset,
         sort_by: Union["CallSummariesInstance.SortBy", object] = values.unset,
         subaccount: Union[str, object] = values.unset,
         abnormal_session: Union[bool, object] = values.unset,
         answered_by: Union["CallSummariesInstance.AnsweredBy", object] = values.unset,
+        connectivity_issues: Union[str, object] = values.unset,
+        quality_issues: Union[str, object] = values.unset,
+        spam: Union[bool, object] = values.unset,
+        call_scores: Union[str, object] = values.unset,
         page_token: Union[str, object] = values.unset,
         page_number: Union[int, object] = values.unset,
         page_size: Union[int, object] = values.unset,
     ) -> CallSummariesPage:
         """
         Retrieve a single page of CallSummariesInstance records from the API.
         Request is executed immediately
@@ -559,14 +611,18 @@
         :param call_state:
         :param direction:
         :param processing_state:
         :param sort_by:
         :param subaccount:
         :param abnormal_session:
         :param answered_by:
+        :param connectivity_issues:
+        :param quality_issues:
+        :param spam:
+        :param call_scores:
         :param page_token: PageToken provided by the API
         :param page_number: Page Number, this value is simply for client state
         :param page_size: Number of records to return, defaults to 50
 
         :returns: Page of CallSummariesInstance
         """
         data = values.of(
@@ -586,14 +642,18 @@
                 "CallState": call_state,
                 "Direction": direction,
                 "ProcessingState": processing_state,
                 "SortBy": sort_by,
                 "Subaccount": subaccount,
                 "AbnormalSession": abnormal_session,
                 "AnsweredBy": answered_by,
+                "ConnectivityIssues": connectivity_issues,
+                "QualityIssues": quality_issues,
+                "Spam": spam,
+                "CallScores": call_scores,
                 "PageToken": page_token,
                 "Page": page_number,
                 "PageSize": page_size,
             }
         )
 
         response = self._version.page(method="GET", uri=self._uri, params=data)
@@ -618,14 +678,18 @@
         processing_state: Union[
             "CallSummariesInstance.ProcessingStateRequest", object
         ] = values.unset,
         sort_by: Union["CallSummariesInstance.SortBy", object] = values.unset,
         subaccount: Union[str, object] = values.unset,
         abnormal_session: Union[bool, object] = values.unset,
         answered_by: Union["CallSummariesInstance.AnsweredBy", object] = values.unset,
+        connectivity_issues: Union[str, object] = values.unset,
+        quality_issues: Union[str, object] = values.unset,
+        spam: Union[bool, object] = values.unset,
+        call_scores: Union[str, object] = values.unset,
         page_token: Union[str, object] = values.unset,
         page_number: Union[int, object] = values.unset,
         page_size: Union[int, object] = values.unset,
     ) -> CallSummariesPage:
         """
         Asynchronously retrieve a single page of CallSummariesInstance records from the API.
         Request is executed immediately
@@ -645,14 +709,18 @@
         :param call_state:
         :param direction:
         :param processing_state:
         :param sort_by:
         :param subaccount:
         :param abnormal_session:
         :param answered_by:
+        :param connectivity_issues:
+        :param quality_issues:
+        :param spam:
+        :param call_scores:
         :param page_token: PageToken provided by the API
         :param page_number: Page Number, this value is simply for client state
         :param page_size: Number of records to return, defaults to 50
 
         :returns: Page of CallSummariesInstance
         """
         data = values.of(
@@ -672,14 +740,18 @@
                 "CallState": call_state,
                 "Direction": direction,
                 "ProcessingState": processing_state,
                 "SortBy": sort_by,
                 "Subaccount": subaccount,
                 "AbnormalSession": abnormal_session,
                 "AnsweredBy": answered_by,
+                "ConnectivityIssues": connectivity_issues,
+                "QualityIssues": quality_issues,
+                "Spam": spam,
+                "CallScores": call_scores,
                 "PageToken": page_token,
                 "Page": page_number,
                 "PageSize": page_size,
             }
         )
 
         response = await self._version.page_async(
```

### Comparing `twilio-8.2.0/twilio/rest/insights/v1/conference/__init__.py` & `twilio-8.2.1/twilio/rest/insights/v1/conference/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/insights/v1/conference/conference_participant.py` & `twilio-8.2.1/twilio/rest/insights/v1/conference/conference_participant.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/insights/v1/room/__init__.py` & `twilio-8.2.1/twilio/rest/insights/v1/room/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/insights/v1/room/participant.py` & `twilio-8.2.1/twilio/rest/insights/v1/room/participant.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/insights/v1/setting.py` & `twilio-8.2.1/twilio/rest/insights/v1/setting.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/ip_messaging/IpMessagingBase.py` & `twilio-8.2.1/twilio/rest/ip_messaging/IpMessagingBase.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/ip_messaging/__init__.py` & `twilio-8.2.1/twilio/rest/ip_messaging/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/ip_messaging/v1/__init__.py` & `twilio-8.2.1/twilio/rest/ip_messaging/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/ip_messaging/v1/credential.py` & `twilio-8.2.1/twilio/rest/ip_messaging/v1/credential.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/ip_messaging/v1/service/__init__.py` & `twilio-8.2.1/twilio/rest/ip_messaging/v1/service/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/ip_messaging/v1/service/channel/__init__.py` & `twilio-8.2.1/twilio/rest/ip_messaging/v1/service/channel/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/ip_messaging/v1/service/channel/invite.py` & `twilio-8.2.1/twilio/rest/ip_messaging/v1/service/channel/invite.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/ip_messaging/v1/service/channel/member.py` & `twilio-8.2.1/twilio/rest/ip_messaging/v1/service/channel/member.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/ip_messaging/v1/service/channel/message.py` & `twilio-8.2.1/twilio/rest/ip_messaging/v1/service/channel/message.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/ip_messaging/v1/service/role.py` & `twilio-8.2.1/twilio/rest/ip_messaging/v1/service/role.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/ip_messaging/v1/service/user/__init__.py` & `twilio-8.2.1/twilio/rest/ip_messaging/v1/service/user/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/ip_messaging/v1/service/user/user_channel.py` & `twilio-8.2.1/twilio/rest/ip_messaging/v1/service/user/user_channel.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/ip_messaging/v2/__init__.py` & `twilio-8.2.1/twilio/rest/ip_messaging/v2/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/ip_messaging/v2/credential.py` & `twilio-8.2.1/twilio/rest/ip_messaging/v2/credential.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/ip_messaging/v2/service/__init__.py` & `twilio-8.2.1/twilio/rest/ip_messaging/v2/service/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/ip_messaging/v2/service/binding.py` & `twilio-8.2.1/twilio/rest/ip_messaging/v2/service/binding.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/ip_messaging/v2/service/channel/__init__.py` & `twilio-8.2.1/twilio/rest/ip_messaging/v2/service/channel/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/ip_messaging/v2/service/channel/invite.py` & `twilio-8.2.1/twilio/rest/ip_messaging/v2/service/channel/invite.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/ip_messaging/v2/service/channel/member.py` & `twilio-8.2.1/twilio/rest/ip_messaging/v2/service/channel/member.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/ip_messaging/v2/service/channel/message.py` & `twilio-8.2.1/twilio/rest/ip_messaging/v2/service/channel/message.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/ip_messaging/v2/service/channel/webhook.py` & `twilio-8.2.1/twilio/rest/ip_messaging/v2/service/channel/webhook.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/ip_messaging/v2/service/role.py` & `twilio-8.2.1/twilio/rest/ip_messaging/v2/service/role.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/ip_messaging/v2/service/user/__init__.py` & `twilio-8.2.1/twilio/rest/ip_messaging/v2/service/user/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/ip_messaging/v2/service/user/user_binding.py` & `twilio-8.2.1/twilio/rest/ip_messaging/v2/service/user/user_binding.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/ip_messaging/v2/service/user/user_channel.py` & `twilio-8.2.1/twilio/rest/ip_messaging/v2/service/user/user_channel.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/lookups/LookupsBase.py` & `twilio-8.2.1/twilio/rest/lookups/LookupsBase.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/lookups/v1/__init__.py` & `twilio-8.2.1/twilio/rest/lookups/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/lookups/v1/phone_number.py` & `twilio-8.2.1/twilio/rest/lookups/v1/phone_number.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/lookups/v2/__init__.py` & `twilio-8.2.1/twilio/rest/lookups/v2/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/lookups/v2/phone_number.py` & `twilio-8.2.1/twilio/rest/lookups/v2/phone_number.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/media/MediaBase.py` & `twilio-8.2.1/twilio/rest/media/MediaBase.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/media/__init__.py` & `twilio-8.2.1/twilio/rest/media/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/media/v1/__init__.py` & `twilio-8.2.1/twilio/rest/media/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/media/v1/media_processor.py` & `twilio-8.2.1/twilio/rest/media/v1/media_processor.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/media/v1/media_recording.py` & `twilio-8.2.1/twilio/rest/media/v1/media_recording.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/media/v1/player_streamer/__init__.py` & `twilio-8.2.1/twilio/rest/media/v1/player_streamer/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/media/v1/player_streamer/playback_grant.py` & `twilio-8.2.1/twilio/rest/media/v1/player_streamer/playback_grant.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/messaging/MessagingBase.py` & `twilio-8.2.1/twilio/rest/messaging/MessagingBase.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/messaging/__init__.py` & `twilio-8.2.1/twilio/rest/messaging/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/messaging/v1/__init__.py` & `twilio-8.2.1/twilio/rest/messaging/v1/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -22,14 +22,17 @@
 from twilio.rest.messaging.v1.domain_config_messaging_service import (
     DomainConfigMessagingServiceList,
 )
 from twilio.rest.messaging.v1.external_campaign import ExternalCampaignList
 from twilio.rest.messaging.v1.linkshortening_messaging_service import (
     LinkshorteningMessagingServiceList,
 )
+from twilio.rest.messaging.v1.linkshortening_messaging_service_domain_association import (
+    LinkshorteningMessagingServiceDomainAssociationList,
+)
 from twilio.rest.messaging.v1.service import ServiceList
 from twilio.rest.messaging.v1.usecase import UsecaseList
 
 
 class V1(Version):
     def __init__(self, domain: Domain):
         """
@@ -45,14 +48,17 @@
         self._domain_config_messaging_service: Optional[
             DomainConfigMessagingServiceList
         ] = None
         self._external_campaign: Optional[ExternalCampaignList] = None
         self._linkshortening_messaging_service: Optional[
             LinkshorteningMessagingServiceList
         ] = None
+        self._linkshortening_messaging_service_domain_association: Optional[
+            LinkshorteningMessagingServiceDomainAssociationList
+        ] = None
         self._services: Optional[ServiceList] = None
         self._usecases: Optional[UsecaseList] = None
 
     @property
     def brand_registrations(self) -> BrandRegistrationList:
         if self._brand_registrations is None:
             self._brand_registrations = BrandRegistrationList(self)
@@ -95,14 +101,24 @@
         if self._linkshortening_messaging_service is None:
             self._linkshortening_messaging_service = LinkshorteningMessagingServiceList(
                 self
             )
         return self._linkshortening_messaging_service
 
     @property
+    def linkshortening_messaging_service_domain_association(
+        self,
+    ) -> LinkshorteningMessagingServiceDomainAssociationList:
+        if self._linkshortening_messaging_service_domain_association is None:
+            self._linkshortening_messaging_service_domain_association = (
+                LinkshorteningMessagingServiceDomainAssociationList(self)
+            )
+        return self._linkshortening_messaging_service_domain_association
+
+    @property
     def services(self) -> ServiceList:
         if self._services is None:
             self._services = ServiceList(self)
         return self._services
 
     @property
     def usecases(self) -> UsecaseList:
```

### Comparing `twilio-8.2.0/twilio/rest/messaging/v1/brand_registration/__init__.py` & `twilio-8.2.1/twilio/rest/messaging/v1/brand_registration/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/messaging/v1/brand_registration/brand_registration_otp.py` & `twilio-8.2.1/twilio/rest/messaging/v1/brand_registration/brand_registration_otp.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/messaging/v1/brand_registration/brand_vetting.py` & `twilio-8.2.1/twilio/rest/messaging/v1/brand_registration/brand_vetting.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/messaging/v1/deactivations.py` & `twilio-8.2.1/twilio/rest/messaging/v1/deactivations.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/messaging/v1/domain_certs.py` & `twilio-8.2.1/twilio/rest/messaging/v1/domain_certs.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/messaging/v1/domain_config.py` & `twilio-8.2.1/twilio/rest/verify/v2/service/access_token.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 r"""
     This code was generated by
    ___ _ _ _ _ _    _ ____    ____ ____ _    ____ ____ _  _ ____ ____ ____ ___ __   __
     |  | | | | |    | |  | __ |  | |__| | __ | __ |___ |\ | |___ |__/ |__|  | |  | |__/
     |  |_|_| | |___ | |__|    |__| |  | |    |__] |___ | \| |___ |  \ |  |  | |__| |  \
 
-    Twilio - Messaging
+    Twilio - Verify
     This is the public Twilio REST API.
 
     NOTE: This class is auto generated by OpenAPI Generator.
     https://openapi-generator.tech
     Do not edit the class manually.
 """
 
@@ -18,282 +18,284 @@
 from twilio.base import deserialize, values
 from twilio.base.instance_context import InstanceContext
 from twilio.base.instance_resource import InstanceResource
 from twilio.base.list_resource import ListResource
 from twilio.base.version import Version
 
 
-class DomainConfigInstance(InstanceResource):
+class AccessTokenInstance(InstanceResource):
+    class FactorTypes(object):
+        PUSH = "push"
 
     """
-    :ivar domain_sid: The unique string that we created to identify the Domain resource.
-    :ivar config_sid: The unique string that we created to identify the Domain config (prefix ZK).
-    :ivar fallback_url: Any requests we receive to this domain that do not match an existing shortened message will be redirected to the fallback url. These will likely be either expired messages, random misdirected traffic, or intentional scraping.
-    :ivar callback_url: URL to receive click events to your webhook whenever the recipients click on the shortened links.
-    :ivar date_created: Date this Domain Config was created.
-    :ivar date_updated: Date that this Domain Config was last updated.
-    :ivar url:
+    :ivar sid: A 34 character string that uniquely identifies this Access Token.
+    :ivar account_sid: The unique SID identifier of the Account.
+    :ivar service_sid: The unique SID identifier of the Verify Service.
+    :ivar entity_identity: The unique external identifier for the Entity of the Service.
+    :ivar factor_type: 
+    :ivar factor_friendly_name: A human readable description of this factor, up to 64 characters. For a push factor, this can be the device's name.
+    :ivar token: The access token generated for enrollment, this is an encrypted json web token.
+    :ivar url: The URL of this resource.
+    :ivar ttl: How long, in seconds, the access token is valid. Max: 5 minutes
+    :ivar date_created: The date that this access token was created, given in [ISO 8601](https://en.wikipedia.org/wiki/ISO_8601) format.
     """
 
     def __init__(
         self,
         version: Version,
         payload: Dict[str, Any],
-        domain_sid: Optional[str] = None,
+        service_sid: str,
+        sid: Optional[str] = None,
     ):
         super().__init__(version)
 
-        self.domain_sid: Optional[str] = payload.get("domain_sid")
-        self.config_sid: Optional[str] = payload.get("config_sid")
-        self.fallback_url: Optional[str] = payload.get("fallback_url")
-        self.callback_url: Optional[str] = payload.get("callback_url")
+        self.sid: Optional[str] = payload.get("sid")
+        self.account_sid: Optional[str] = payload.get("account_sid")
+        self.service_sid: Optional[str] = payload.get("service_sid")
+        self.entity_identity: Optional[str] = payload.get("entity_identity")
+        self.factor_type: Optional["AccessTokenInstance.FactorTypes"] = payload.get(
+            "factor_type"
+        )
+        self.factor_friendly_name: Optional[str] = payload.get("factor_friendly_name")
+        self.token: Optional[str] = payload.get("token")
+        self.url: Optional[str] = payload.get("url")
+        self.ttl: Optional[int] = deserialize.integer(payload.get("ttl"))
         self.date_created: Optional[datetime] = deserialize.iso8601_datetime(
             payload.get("date_created")
         )
-        self.date_updated: Optional[datetime] = deserialize.iso8601_datetime(
-            payload.get("date_updated")
-        )
-        self.url: Optional[str] = payload.get("url")
 
         self._solution = {
-            "domain_sid": domain_sid or self.domain_sid,
+            "service_sid": service_sid,
+            "sid": sid or self.sid,
         }
-        self._context: Optional[DomainConfigContext] = None
+        self._context: Optional[AccessTokenContext] = None
 
     @property
-    def _proxy(self) -> "DomainConfigContext":
+    def _proxy(self) -> "AccessTokenContext":
         """
         Generate an instance context for the instance, the context is capable of
         performing various actions. All instance actions are proxied to the context
 
-        :returns: DomainConfigContext for this DomainConfigInstance
+        :returns: AccessTokenContext for this AccessTokenInstance
         """
         if self._context is None:
-            self._context = DomainConfigContext(
+            self._context = AccessTokenContext(
                 self._version,
-                domain_sid=self._solution["domain_sid"],
+                service_sid=self._solution["service_sid"],
+                sid=self._solution["sid"],
             )
         return self._context
 
-    def fetch(self) -> "DomainConfigInstance":
+    def fetch(self) -> "AccessTokenInstance":
         """
-        Fetch the DomainConfigInstance
+        Fetch the AccessTokenInstance
 
 
-        :returns: The fetched DomainConfigInstance
+        :returns: The fetched AccessTokenInstance
         """
         return self._proxy.fetch()
 
-    async def fetch_async(self) -> "DomainConfigInstance":
+    async def fetch_async(self) -> "AccessTokenInstance":
         """
-        Asynchronous coroutine to fetch the DomainConfigInstance
+        Asynchronous coroutine to fetch the AccessTokenInstance
 
 
-        :returns: The fetched DomainConfigInstance
+        :returns: The fetched AccessTokenInstance
         """
         return await self._proxy.fetch_async()
 
-    def update(
-        self,
-        fallback_url: Union[str, object] = values.unset,
-        callback_url: Union[str, object] = values.unset,
-    ) -> "DomainConfigInstance":
-        """
-        Update the DomainConfigInstance
-
-        :param fallback_url: Any requests we receive to this domain that do not match an existing shortened message will be redirected to the fallback url. These will likely be either expired messages, random misdirected traffic, or intentional scraping.
-        :param callback_url: URL to receive click events to your webhook whenever the recipients click on the shortened links
-
-        :returns: The updated DomainConfigInstance
-        """
-        return self._proxy.update(
-            fallback_url=fallback_url,
-            callback_url=callback_url,
-        )
-
-    async def update_async(
-        self,
-        fallback_url: Union[str, object] = values.unset,
-        callback_url: Union[str, object] = values.unset,
-    ) -> "DomainConfigInstance":
-        """
-        Asynchronous coroutine to update the DomainConfigInstance
-
-        :param fallback_url: Any requests we receive to this domain that do not match an existing shortened message will be redirected to the fallback url. These will likely be either expired messages, random misdirected traffic, or intentional scraping.
-        :param callback_url: URL to receive click events to your webhook whenever the recipients click on the shortened links
-
-        :returns: The updated DomainConfigInstance
-        """
-        return await self._proxy.update_async(
-            fallback_url=fallback_url,
-            callback_url=callback_url,
-        )
-
     def __repr__(self) -> str:
         """
         Provide a friendly representation
 
         :returns: Machine friendly representation
         """
         context = " ".join("{}={}".format(k, v) for k, v in self._solution.items())
-        return "<Twilio.Messaging.V1.DomainConfigInstance {}>".format(context)
+        return "<Twilio.Verify.V2.AccessTokenInstance {}>".format(context)
 
 
-class DomainConfigContext(InstanceContext):
-    def __init__(self, version: Version, domain_sid: str):
+class AccessTokenContext(InstanceContext):
+    def __init__(self, version: Version, service_sid: str, sid: str):
         """
-        Initialize the DomainConfigContext
+        Initialize the AccessTokenContext
 
         :param version: Version that contains the resource
-        :param domain_sid: Unique string used to identify the domain that this config should be associated with.
+        :param service_sid: The unique SID identifier of the Service.
+        :param sid: A 34 character string that uniquely identifies this Access Token.
         """
         super().__init__(version)
 
         # Path Solution
         self._solution = {
-            "domain_sid": domain_sid,
+            "service_sid": service_sid,
+            "sid": sid,
         }
-        self._uri = "/LinkShortening/Domains/{domain_sid}/Config".format(
+        self._uri = "/Services/{service_sid}/AccessTokens/{sid}".format(
             **self._solution
         )
 
-    def fetch(self) -> DomainConfigInstance:
+    def fetch(self) -> AccessTokenInstance:
         """
-        Fetch the DomainConfigInstance
+        Fetch the AccessTokenInstance
 
 
-        :returns: The fetched DomainConfigInstance
+        :returns: The fetched AccessTokenInstance
         """
 
         payload = self._version.fetch(
             method="GET",
             uri=self._uri,
         )
 
-        return DomainConfigInstance(
+        return AccessTokenInstance(
             self._version,
             payload,
-            domain_sid=self._solution["domain_sid"],
+            service_sid=self._solution["service_sid"],
+            sid=self._solution["sid"],
         )
 
-    async def fetch_async(self) -> DomainConfigInstance:
+    async def fetch_async(self) -> AccessTokenInstance:
         """
-        Asynchronous coroutine to fetch the DomainConfigInstance
+        Asynchronous coroutine to fetch the AccessTokenInstance
 
 
-        :returns: The fetched DomainConfigInstance
+        :returns: The fetched AccessTokenInstance
         """
 
         payload = await self._version.fetch_async(
             method="GET",
             uri=self._uri,
         )
 
-        return DomainConfigInstance(
+        return AccessTokenInstance(
             self._version,
             payload,
-            domain_sid=self._solution["domain_sid"],
+            service_sid=self._solution["service_sid"],
+            sid=self._solution["sid"],
         )
 
-    def update(
-        self,
-        fallback_url: Union[str, object] = values.unset,
-        callback_url: Union[str, object] = values.unset,
-    ) -> DomainConfigInstance:
+    def __repr__(self) -> str:
+        """
+        Provide a friendly representation
+
+        :returns: Machine friendly representation
+        """
+        context = " ".join("{}={}".format(k, v) for k, v in self._solution.items())
+        return "<Twilio.Verify.V2.AccessTokenContext {}>".format(context)
+
+
+class AccessTokenList(ListResource):
+    def __init__(self, version: Version, service_sid: str):
+        """
+        Initialize the AccessTokenList
+
+        :param version: Version that contains the resource
+        :param service_sid: The unique SID identifier of the Service.
+
         """
-        Update the DomainConfigInstance
+        super().__init__(version)
 
-        :param fallback_url: Any requests we receive to this domain that do not match an existing shortened message will be redirected to the fallback url. These will likely be either expired messages, random misdirected traffic, or intentional scraping.
-        :param callback_url: URL to receive click events to your webhook whenever the recipients click on the shortened links
+        # Path Solution
+        self._solution = {
+            "service_sid": service_sid,
+        }
+        self._uri = "/Services/{service_sid}/AccessTokens".format(**self._solution)
 
-        :returns: The updated DomainConfigInstance
+    def create(
+        self,
+        identity: str,
+        factor_type: "AccessTokenInstance.FactorTypes",
+        factor_friendly_name: Union[str, object] = values.unset,
+        ttl: Union[int, object] = values.unset,
+    ) -> AccessTokenInstance:
+        """
+        Create the AccessTokenInstance
+
+        :param identity: The unique external identifier for the Entity of the Service. This identifier should be immutable, not PII, and generated by your external system, such as your user's UUID, GUID, or SID.
+        :param factor_type:
+        :param factor_friendly_name: The friendly name of the factor that is going to be created with this access token
+        :param ttl: How long, in seconds, the access token is valid. Can be an integer between 60 and 300. Default is 60.
+
+        :returns: The created AccessTokenInstance
         """
         data = values.of(
             {
-                "FallbackUrl": fallback_url,
-                "CallbackUrl": callback_url,
+                "Identity": identity,
+                "FactorType": factor_type,
+                "FactorFriendlyName": factor_friendly_name,
+                "Ttl": ttl,
             }
         )
 
-        payload = self._version.update(
+        payload = self._version.create(
             method="POST",
             uri=self._uri,
             data=data,
         )
 
-        return DomainConfigInstance(
-            self._version, payload, domain_sid=self._solution["domain_sid"]
+        return AccessTokenInstance(
+            self._version, payload, service_sid=self._solution["service_sid"]
         )
 
-    async def update_async(
+    async def create_async(
         self,
-        fallback_url: Union[str, object] = values.unset,
-        callback_url: Union[str, object] = values.unset,
-    ) -> DomainConfigInstance:
-        """
-        Asynchronous coroutine to update the DomainConfigInstance
+        identity: str,
+        factor_type: "AccessTokenInstance.FactorTypes",
+        factor_friendly_name: Union[str, object] = values.unset,
+        ttl: Union[int, object] = values.unset,
+    ) -> AccessTokenInstance:
+        """
+        Asynchronously create the AccessTokenInstance
+
+        :param identity: The unique external identifier for the Entity of the Service. This identifier should be immutable, not PII, and generated by your external system, such as your user's UUID, GUID, or SID.
+        :param factor_type:
+        :param factor_friendly_name: The friendly name of the factor that is going to be created with this access token
+        :param ttl: How long, in seconds, the access token is valid. Can be an integer between 60 and 300. Default is 60.
 
-        :param fallback_url: Any requests we receive to this domain that do not match an existing shortened message will be redirected to the fallback url. These will likely be either expired messages, random misdirected traffic, or intentional scraping.
-        :param callback_url: URL to receive click events to your webhook whenever the recipients click on the shortened links
-
-        :returns: The updated DomainConfigInstance
+        :returns: The created AccessTokenInstance
         """
         data = values.of(
             {
-                "FallbackUrl": fallback_url,
-                "CallbackUrl": callback_url,
+                "Identity": identity,
+                "FactorType": factor_type,
+                "FactorFriendlyName": factor_friendly_name,
+                "Ttl": ttl,
             }
         )
 
-        payload = await self._version.update_async(
+        payload = await self._version.create_async(
             method="POST",
             uri=self._uri,
             data=data,
         )
 
-        return DomainConfigInstance(
-            self._version, payload, domain_sid=self._solution["domain_sid"]
+        return AccessTokenInstance(
+            self._version, payload, service_sid=self._solution["service_sid"]
         )
 
-    def __repr__(self) -> str:
+    def get(self, sid: str) -> AccessTokenContext:
         """
-        Provide a friendly representation
+        Constructs a AccessTokenContext
 
-        :returns: Machine friendly representation
+        :param sid: A 34 character string that uniquely identifies this Access Token.
         """
-        context = " ".join("{}={}".format(k, v) for k, v in self._solution.items())
-        return "<Twilio.Messaging.V1.DomainConfigContext {}>".format(context)
-
-
-class DomainConfigList(ListResource):
-    def __init__(self, version: Version):
-        """
-        Initialize the DomainConfigList
-
-        :param version: Version that contains the resource
-
-        """
-        super().__init__(version)
-
-    def get(self, domain_sid: str) -> DomainConfigContext:
-        """
-        Constructs a DomainConfigContext
-
-        :param domain_sid: Unique string used to identify the domain that this config should be associated with.
-        """
-        return DomainConfigContext(self._version, domain_sid=domain_sid)
+        return AccessTokenContext(
+            self._version, service_sid=self._solution["service_sid"], sid=sid
+        )
 
-    def __call__(self, domain_sid: str) -> DomainConfigContext:
+    def __call__(self, sid: str) -> AccessTokenContext:
         """
-        Constructs a DomainConfigContext
+        Constructs a AccessTokenContext
 
-        :param domain_sid: Unique string used to identify the domain that this config should be associated with.
+        :param sid: A 34 character string that uniquely identifies this Access Token.
         """
-        return DomainConfigContext(self._version, domain_sid=domain_sid)
+        return AccessTokenContext(
+            self._version, service_sid=self._solution["service_sid"], sid=sid
+        )
 
     def __repr__(self) -> str:
         """
         Provide a friendly representation
 
         :returns: Machine friendly representation
         """
-        return "<Twilio.Messaging.V1.DomainConfigList>"
+        return "<Twilio.Verify.V2.AccessTokenList>"
```

### Comparing `twilio-8.2.0/twilio/rest/messaging/v1/domain_config_messaging_service.py` & `twilio-8.2.1/twilio/rest/messaging/v1/domain_config_messaging_service.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,14 +26,15 @@
 
     """
     :ivar domain_sid: The unique string that we created to identify the Domain resource.
     :ivar config_sid: The unique string that we created to identify the Domain config (prefix ZK).
     :ivar messaging_service_sid: The unique string that identifies the messaging service
     :ivar fallback_url: Any requests we receive to this domain that do not match an existing shortened message will be redirected to the fallback url. These will likely be either expired messages, random misdirected traffic, or intentional scraping.
     :ivar callback_url: URL to receive click events to your webhook whenever the recipients click on the shortened links.
+    :ivar continue_on_failure: Boolean field to set customer delivery preference when there is a failure in linkShortening service
     :ivar date_created: Date this Domain Config was created.
     :ivar date_updated: Date that this Domain Config was last updated.
     :ivar url:
     """
 
     def __init__(
         self,
@@ -44,14 +45,15 @@
         super().__init__(version)
 
         self.domain_sid: Optional[str] = payload.get("domain_sid")
         self.config_sid: Optional[str] = payload.get("config_sid")
         self.messaging_service_sid: Optional[str] = payload.get("messaging_service_sid")
         self.fallback_url: Optional[str] = payload.get("fallback_url")
         self.callback_url: Optional[str] = payload.get("callback_url")
+        self.continue_on_failure: Optional[bool] = payload.get("continue_on_failure")
         self.date_created: Optional[datetime] = deserialize.iso8601_datetime(
             payload.get("date_created")
         )
         self.date_updated: Optional[datetime] = deserialize.iso8601_datetime(
             payload.get("date_updated")
         )
         self.url: Optional[str] = payload.get("url")
```

### Comparing `twilio-8.2.0/twilio/rest/messaging/v1/external_campaign.py` & `twilio-8.2.1/twilio/rest/messaging/v1/external_campaign.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/messaging/v1/linkshortening_messaging_service.py` & `twilio-8.2.1/twilio/rest/messaging/v1/linkshortening_messaging_service.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/messaging/v1/service/__init__.py` & `twilio-8.2.1/twilio/rest/messaging/v1/service/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/messaging/v1/service/alpha_sender.py` & `twilio-8.2.1/twilio/rest/messaging/v1/service/alpha_sender.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/messaging/v1/service/phone_number.py` & `twilio-8.2.1/twilio/rest/messaging/v1/service/phone_number.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/messaging/v1/service/short_code.py` & `twilio-8.2.1/twilio/rest/messaging/v1/service/short_code.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/messaging/v1/service/us_app_to_person.py` & `twilio-8.2.1/twilio/rest/messaging/v1/service/us_app_to_person.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/messaging/v1/service/us_app_to_person_usecase.py` & `twilio-8.2.1/twilio/rest/messaging/v1/service/us_app_to_person_usecase.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/messaging/v1/usecase.py` & `twilio-8.2.1/twilio/rest/messaging/v1/usecase.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/microvisor/MicrovisorBase.py` & `twilio-8.2.1/twilio/rest/microvisor/MicrovisorBase.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/microvisor/__init__.py` & `twilio-8.2.1/twilio/rest/microvisor/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/microvisor/v1/__init__.py` & `twilio-8.2.1/twilio/rest/microvisor/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/microvisor/v1/account_config.py` & `twilio-8.2.1/twilio/rest/microvisor/v1/account_config.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/microvisor/v1/account_secret.py` & `twilio-8.2.1/twilio/rest/microvisor/v1/account_secret.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/microvisor/v1/app/__init__.py` & `twilio-8.2.1/twilio/rest/microvisor/v1/app/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/microvisor/v1/app/app_manifest.py` & `twilio-8.2.1/twilio/rest/microvisor/v1/app/app_manifest.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/microvisor/v1/device/__init__.py` & `twilio-8.2.1/twilio/rest/microvisor/v1/device/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/microvisor/v1/device/device_config.py` & `twilio-8.2.1/twilio/rest/microvisor/v1/device/device_config.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/microvisor/v1/device/device_secret.py` & `twilio-8.2.1/twilio/rest/microvisor/v1/device/device_secret.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/monitor/MonitorBase.py` & `twilio-8.2.1/twilio/rest/monitor/MonitorBase.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/monitor/__init__.py` & `twilio-8.2.1/twilio/rest/monitor/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/monitor/v1/__init__.py` & `twilio-8.2.1/twilio/rest/monitor/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/monitor/v1/alert.py` & `twilio-8.2.1/twilio/rest/monitor/v1/alert.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/monitor/v1/event.py` & `twilio-8.2.1/twilio/rest/monitor/v1/event.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/notify/NotifyBase.py` & `twilio-8.2.1/twilio/rest/notify/NotifyBase.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/notify/__init__.py` & `twilio-8.2.1/twilio/rest/notify/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/notify/v1/__init__.py` & `twilio-8.2.1/twilio/rest/notify/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/notify/v1/credential.py` & `twilio-8.2.1/twilio/rest/notify/v1/credential.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/notify/v1/service/__init__.py` & `twilio-8.2.1/twilio/rest/notify/v1/service/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/notify/v1/service/binding.py` & `twilio-8.2.1/twilio/rest/notify/v1/service/binding.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/notify/v1/service/notification.py` & `twilio-8.2.1/twilio/rest/notify/v1/service/notification.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/numbers/NumbersBase.py` & `twilio-8.2.1/twilio/rest/video/VideoBase.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,35 +9,35 @@
   Do not edit the class manually.
 """
 
 from typing import Optional
 
 from twilio.base.domain import Domain
 from twilio.rest import Client
-from twilio.rest.numbers.v2 import V2
+from twilio.rest.video.v1 import V1
 
 
-class NumbersBase(Domain):
+class VideoBase(Domain):
     def __init__(self, twilio: Client):
         """
-        Initialize the Numbers Domain
+        Initialize the Video Domain
 
-        :returns: Domain for Numbers
+        :returns: Domain for Video
         """
-        super().__init__(twilio, "https://numbers.twilio.com")
-        self._v2: Optional[V2] = None
+        super().__init__(twilio, "https://video.twilio.com")
+        self._v1: Optional[V1] = None
 
     @property
-    def v2(self) -> V2:
+    def v1(self) -> V1:
         """
-        :returns: Versions v2 of Numbers
+        :returns: Versions v1 of Video
         """
-        if self._v2 is None:
-            self._v2 = V2(self)
-        return self._v2
+        if self._v1 is None:
+            self._v1 = V1(self)
+        return self._v1
 
     def __repr__(self) -> str:
         """
         Provide a friendly representation
         :returns: Machine friendly representation
         """
-        return "<Twilio.Numbers>"
+        return "<Twilio.Video>"
```

### Comparing `twilio-8.2.0/twilio/rest/numbers/v2/__init__.py` & `twilio-8.2.1/twilio/rest/numbers/v2/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/numbers/v2/regulatory_compliance/__init__.py` & `twilio-8.2.1/twilio/rest/numbers/v2/regulatory_compliance/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/numbers/v2/regulatory_compliance/bundle/__init__.py` & `twilio-8.2.1/twilio/rest/numbers/v2/regulatory_compliance/bundle/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/numbers/v2/regulatory_compliance/bundle/bundle_copy.py` & `twilio-8.2.1/twilio/rest/numbers/v2/regulatory_compliance/bundle/bundle_copy.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/numbers/v2/regulatory_compliance/bundle/evaluation.py` & `twilio-8.2.1/twilio/rest/numbers/v2/regulatory_compliance/bundle/evaluation.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/numbers/v2/regulatory_compliance/bundle/item_assignment.py` & `twilio-8.2.1/twilio/rest/numbers/v2/regulatory_compliance/bundle/item_assignment.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/numbers/v2/regulatory_compliance/bundle/replace_items.py` & `twilio-8.2.1/twilio/rest/numbers/v2/regulatory_compliance/bundle/replace_items.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/numbers/v2/regulatory_compliance/end_user.py` & `twilio-8.2.1/twilio/rest/numbers/v2/regulatory_compliance/end_user.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/numbers/v2/regulatory_compliance/end_user_type.py` & `twilio-8.2.1/twilio/rest/numbers/v2/regulatory_compliance/end_user_type.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/numbers/v2/regulatory_compliance/regulation.py` & `twilio-8.2.1/twilio/rest/numbers/v2/regulatory_compliance/regulation.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/numbers/v2/regulatory_compliance/supporting_document.py` & `twilio-8.2.1/twilio/rest/numbers/v2/regulatory_compliance/supporting_document.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/numbers/v2/regulatory_compliance/supporting_document_type.py` & `twilio-8.2.1/twilio/rest/numbers/v2/regulatory_compliance/supporting_document_type.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/oauth/OauthBase.py` & `twilio-8.2.1/twilio/rest/oauth/OauthBase.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/oauth/__init__.py` & `twilio-8.2.1/twilio/rest/oauth/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/oauth/v1/__init__.py` & `twilio-8.2.1/twilio/rest/oauth/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/oauth/v1/device_code.py` & `twilio-8.2.1/twilio/rest/oauth/v1/device_code.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/oauth/v1/oauth.py` & `twilio-8.2.1/twilio/rest/oauth/v1/oauth.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/oauth/v1/openid_discovery.py` & `twilio-8.2.1/twilio/rest/oauth/v1/openid_discovery.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/oauth/v1/token.py` & `twilio-8.2.1/twilio/rest/oauth/v1/token.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/oauth/v1/user_info.py` & `twilio-8.2.1/twilio/rest/oauth/v1/user_info.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/preview/PreviewBase.py` & `twilio-8.2.1/twilio/rest/preview/PreviewBase.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/preview/__init__.py` & `twilio-8.2.1/twilio/rest/preview/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/preview/deployed_devices/__init__.py` & `twilio-8.2.1/twilio/rest/preview/deployed_devices/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/preview/deployed_devices/fleet/__init__.py` & `twilio-8.2.1/twilio/rest/preview/deployed_devices/fleet/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/preview/deployed_devices/fleet/certificate.py` & `twilio-8.2.1/twilio/rest/preview/deployed_devices/fleet/certificate.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/preview/deployed_devices/fleet/deployment.py` & `twilio-8.2.1/twilio/rest/preview/deployed_devices/fleet/deployment.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/preview/deployed_devices/fleet/device.py` & `twilio-8.2.1/twilio/rest/preview/deployed_devices/fleet/device.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/preview/deployed_devices/fleet/key.py` & `twilio-8.2.1/twilio/rest/preview/deployed_devices/fleet/key.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/preview/hosted_numbers/__init__.py` & `twilio-8.2.1/twilio/rest/preview/hosted_numbers/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/preview/hosted_numbers/authorization_document/__init__.py` & `twilio-8.2.1/twilio/rest/preview/hosted_numbers/authorization_document/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/preview/hosted_numbers/authorization_document/dependent_hosted_number_order.py` & `twilio-8.2.1/twilio/rest/preview/hosted_numbers/authorization_document/dependent_hosted_number_order.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/preview/hosted_numbers/hosted_number_order.py` & `twilio-8.2.1/twilio/rest/preview/hosted_numbers/hosted_number_order.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/preview/marketplace/__init__.py` & `twilio-8.2.1/twilio/rest/preview/marketplace/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/preview/marketplace/available_add_on/__init__.py` & `twilio-8.2.1/twilio/rest/preview/marketplace/available_add_on/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/preview/marketplace/available_add_on/available_add_on_extension.py` & `twilio-8.2.1/twilio/rest/preview/marketplace/available_add_on/available_add_on_extension.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/preview/marketplace/installed_add_on/__init__.py` & `twilio-8.2.1/twilio/rest/preview/marketplace/installed_add_on/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/preview/marketplace/installed_add_on/installed_add_on_extension.py` & `twilio-8.2.1/twilio/rest/preview/marketplace/installed_add_on/installed_add_on_extension.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/preview/sync/__init__.py` & `twilio-8.2.1/twilio/rest/preview/sync/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/preview/sync/service/__init__.py` & `twilio-8.2.1/twilio/rest/preview/sync/service/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/preview/sync/service/document/__init__.py` & `twilio-8.2.1/twilio/rest/preview/sync/service/document/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/preview/sync/service/document/document_permission.py` & `twilio-8.2.1/twilio/rest/preview/sync/service/document/document_permission.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/preview/sync/service/sync_list/__init__.py` & `twilio-8.2.1/twilio/rest/preview/sync/service/sync_list/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/preview/sync/service/sync_list/sync_list_item.py` & `twilio-8.2.1/twilio/rest/preview/sync/service/sync_list/sync_list_item.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/preview/sync/service/sync_list/sync_list_permission.py` & `twilio-8.2.1/twilio/rest/preview/sync/service/sync_list/sync_list_permission.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/preview/sync/service/sync_map/__init__.py` & `twilio-8.2.1/twilio/rest/preview/sync/service/sync_map/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/preview/sync/service/sync_map/sync_map_item.py` & `twilio-8.2.1/twilio/rest/preview/sync/service/sync_map/sync_map_item.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/preview/sync/service/sync_map/sync_map_permission.py` & `twilio-8.2.1/twilio/rest/preview/sync/service/sync_map/sync_map_permission.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/preview/understand/__init__.py` & `twilio-8.2.1/twilio/rest/preview/understand/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/preview/understand/assistant/__init__.py` & `twilio-8.2.1/twilio/rest/preview/understand/assistant/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/preview/understand/assistant/assistant_fallback_actions.py` & `twilio-8.2.1/twilio/rest/preview/understand/assistant/assistant_fallback_actions.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/preview/understand/assistant/assistant_initiation_actions.py` & `twilio-8.2.1/twilio/rest/preview/understand/assistant/assistant_initiation_actions.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/preview/understand/assistant/dialogue.py` & `twilio-8.2.1/twilio/rest/preview/understand/assistant/dialogue.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/preview/understand/assistant/field_type/__init__.py` & `twilio-8.2.1/twilio/rest/preview/understand/assistant/field_type/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/preview/understand/assistant/field_type/field_value.py` & `twilio-8.2.1/twilio/rest/preview/understand/assistant/field_type/field_value.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/preview/understand/assistant/model_build.py` & `twilio-8.2.1/twilio/rest/preview/understand/assistant/model_build.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/preview/understand/assistant/query.py` & `twilio-8.2.1/twilio/rest/preview/understand/assistant/query.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/preview/understand/assistant/style_sheet.py` & `twilio-8.2.1/twilio/rest/preview/understand/assistant/style_sheet.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/preview/understand/assistant/task/__init__.py` & `twilio-8.2.1/twilio/rest/preview/understand/assistant/task/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/preview/understand/assistant/task/field.py` & `twilio-8.2.1/twilio/rest/preview/understand/assistant/task/field.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/preview/understand/assistant/task/sample.py` & `twilio-8.2.1/twilio/rest/preview/understand/assistant/task/sample.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/preview/understand/assistant/task/task_actions.py` & `twilio-8.2.1/twilio/rest/preview/understand/assistant/task/task_actions.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/preview/understand/assistant/task/task_statistics.py` & `twilio-8.2.1/twilio/rest/preview/understand/assistant/task/task_statistics.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/preview/wireless/__init__.py` & `twilio-8.2.1/twilio/rest/preview/wireless/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/preview/wireless/command.py` & `twilio-8.2.1/twilio/rest/preview/wireless/command.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/preview/wireless/rate_plan.py` & `twilio-8.2.1/twilio/rest/preview/wireless/rate_plan.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/preview/wireless/sim/__init__.py` & `twilio-8.2.1/twilio/rest/preview/wireless/sim/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/preview/wireless/sim/usage.py` & `twilio-8.2.1/twilio/rest/preview/wireless/sim/usage.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/pricing/PricingBase.py` & `twilio-8.2.1/twilio/rest/pricing/PricingBase.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/pricing/__init__.py` & `twilio-8.2.1/twilio/rest/pricing/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/pricing/v1/__init__.py` & `twilio-8.2.1/twilio/rest/pricing/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/pricing/v1/messaging/__init__.py` & `twilio-8.2.1/twilio/rest/pricing/v1/messaging/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/pricing/v1/messaging/country.py` & `twilio-8.2.1/twilio/rest/pricing/v1/messaging/country.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/pricing/v1/phone_number/__init__.py` & `twilio-8.2.1/twilio/rest/pricing/v1/phone_number/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/pricing/v1/phone_number/country.py` & `twilio-8.2.1/twilio/rest/pricing/v1/phone_number/country.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/pricing/v1/voice/__init__.py` & `twilio-8.2.1/twilio/rest/pricing/v1/voice/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/pricing/v1/voice/country.py` & `twilio-8.2.1/twilio/rest/pricing/v1/voice/country.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/pricing/v1/voice/number.py` & `twilio-8.2.1/twilio/rest/pricing/v1/voice/number.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/pricing/v2/__init__.py` & `twilio-8.2.1/twilio/rest/pricing/v2/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/pricing/v2/country.py` & `twilio-8.2.1/twilio/rest/pricing/v2/country.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/pricing/v2/number.py` & `twilio-8.2.1/twilio/rest/pricing/v2/number.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/pricing/v2/voice/__init__.py` & `twilio-8.2.1/twilio/rest/pricing/v2/voice/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/pricing/v2/voice/country.py` & `twilio-8.2.1/twilio/rest/pricing/v2/voice/country.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/pricing/v2/voice/number.py` & `twilio-8.2.1/twilio/rest/pricing/v2/voice/number.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/proxy/ProxyBase.py` & `twilio-8.2.1/twilio/rest/proxy/ProxyBase.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/proxy/v1/__init__.py` & `twilio-8.2.1/twilio/rest/proxy/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/proxy/v1/service/__init__.py` & `twilio-8.2.1/twilio/rest/proxy/v1/service/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/proxy/v1/service/phone_number.py` & `twilio-8.2.1/twilio/rest/proxy/v1/service/phone_number.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/proxy/v1/service/session/__init__.py` & `twilio-8.2.1/twilio/rest/proxy/v1/service/session/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/proxy/v1/service/session/interaction.py` & `twilio-8.2.1/twilio/rest/proxy/v1/service/session/interaction.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/proxy/v1/service/session/participant/__init__.py` & `twilio-8.2.1/twilio/rest/proxy/v1/service/session/participant/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/proxy/v1/service/session/participant/message_interaction.py` & `twilio-8.2.1/twilio/rest/proxy/v1/service/session/participant/message_interaction.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/proxy/v1/service/short_code.py` & `twilio-8.2.1/twilio/rest/proxy/v1/service/short_code.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/routes/RoutesBase.py` & `twilio-8.2.1/twilio/rest/routes/RoutesBase.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/routes/__init__.py` & `twilio-8.2.1/twilio/rest/routes/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/routes/v2/__init__.py` & `twilio-8.2.1/twilio/rest/routes/v2/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/routes/v2/phone_number.py` & `twilio-8.2.1/twilio/rest/routes/v2/phone_number.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/routes/v2/sip_domain.py` & `twilio-8.2.1/twilio/rest/routes/v2/sip_domain.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/routes/v2/trunk.py` & `twilio-8.2.1/twilio/rest/routes/v2/trunk.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/serverless/ServerlessBase.py` & `twilio-8.2.1/twilio/rest/serverless/ServerlessBase.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/serverless/v1/__init__.py` & `twilio-8.2.1/twilio/rest/serverless/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/serverless/v1/service/__init__.py` & `twilio-8.2.1/twilio/rest/serverless/v1/service/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/serverless/v1/service/asset/__init__.py` & `twilio-8.2.1/twilio/rest/serverless/v1/service/asset/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/serverless/v1/service/asset/asset_version.py` & `twilio-8.2.1/twilio/rest/serverless/v1/service/asset/asset_version.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/serverless/v1/service/build/__init__.py` & `twilio-8.2.1/twilio/rest/serverless/v1/service/build/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/serverless/v1/service/build/build_status.py` & `twilio-8.2.1/twilio/rest/serverless/v1/service/build/build_status.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/serverless/v1/service/environment/__init__.py` & `twilio-8.2.1/twilio/rest/serverless/v1/service/environment/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/serverless/v1/service/environment/deployment.py` & `twilio-8.2.1/twilio/rest/serverless/v1/service/environment/deployment.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/serverless/v1/service/environment/log.py` & `twilio-8.2.1/twilio/rest/serverless/v1/service/environment/log.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/serverless/v1/service/environment/variable.py` & `twilio-8.2.1/twilio/rest/serverless/v1/service/environment/variable.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/serverless/v1/service/function/__init__.py` & `twilio-8.2.1/twilio/rest/serverless/v1/service/function/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/serverless/v1/service/function/function_version/__init__.py` & `twilio-8.2.1/twilio/rest/serverless/v1/service/function/function_version/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/serverless/v1/service/function/function_version/function_version_content.py` & `twilio-8.2.1/twilio/rest/serverless/v1/service/function/function_version/function_version_content.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/studio/StudioBase.py` & `twilio-8.2.1/twilio/rest/studio/StudioBase.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/studio/__init__.py` & `twilio-8.2.1/twilio/rest/studio/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/studio/v1/__init__.py` & `twilio-8.2.1/twilio/rest/studio/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/studio/v1/flow/__init__.py` & `twilio-8.2.1/twilio/rest/studio/v1/flow/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/studio/v1/flow/engagement/__init__.py` & `twilio-8.2.1/twilio/rest/studio/v1/flow/engagement/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/studio/v1/flow/engagement/engagement_context.py` & `twilio-8.2.1/twilio/rest/studio/v1/flow/engagement/engagement_context.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/studio/v1/flow/engagement/step/__init__.py` & `twilio-8.2.1/twilio/rest/studio/v1/flow/engagement/step/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/studio/v1/flow/engagement/step/step_context.py` & `twilio-8.2.1/twilio/rest/studio/v1/flow/engagement/step/step_context.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/studio/v1/flow/execution/__init__.py` & `twilio-8.2.1/twilio/rest/studio/v1/flow/execution/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/studio/v1/flow/execution/execution_context.py` & `twilio-8.2.1/twilio/rest/studio/v1/flow/execution/execution_context.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/studio/v1/flow/execution/execution_step/__init__.py` & `twilio-8.2.1/twilio/rest/studio/v1/flow/execution/execution_step/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/studio/v1/flow/execution/execution_step/execution_step_context.py` & `twilio-8.2.1/twilio/rest/studio/v1/flow/execution/execution_step/execution_step_context.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/studio/v2/__init__.py` & `twilio-8.2.1/twilio/rest/studio/v2/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/studio/v2/flow/__init__.py` & `twilio-8.2.1/twilio/rest/studio/v2/flow/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/studio/v2/flow/execution/__init__.py` & `twilio-8.2.1/twilio/rest/studio/v2/flow/execution/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/studio/v2/flow/execution/execution_context.py` & `twilio-8.2.1/twilio/rest/studio/v2/flow/execution/execution_context.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/studio/v2/flow/execution/execution_step/__init__.py` & `twilio-8.2.1/twilio/rest/studio/v2/flow/execution/execution_step/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/studio/v2/flow/execution/execution_step/execution_step_context.py` & `twilio-8.2.1/twilio/rest/studio/v2/flow/execution/execution_step/execution_step_context.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/studio/v2/flow/flow_revision.py` & `twilio-8.2.1/twilio/rest/studio/v2/flow/flow_revision.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/studio/v2/flow/flow_test_user.py` & `twilio-8.2.1/twilio/rest/studio/v2/flow/flow_test_user.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/studio/v2/flow_validate.py` & `twilio-8.2.1/twilio/rest/studio/v2/flow_validate.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/supersim/SupersimBase.py` & `twilio-8.2.1/twilio/rest/supersim/SupersimBase.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/supersim/__init__.py` & `twilio-8.2.1/twilio/rest/supersim/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/supersim/v1/__init__.py` & `twilio-8.2.1/twilio/rest/supersim/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/supersim/v1/esim_profile.py` & `twilio-8.2.1/twilio/rest/supersim/v1/esim_profile.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/supersim/v1/fleet.py` & `twilio-8.2.1/twilio/rest/supersim/v1/fleet.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/supersim/v1/ip_command.py` & `twilio-8.2.1/twilio/rest/supersim/v1/ip_command.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/supersim/v1/network.py` & `twilio-8.2.1/twilio/rest/supersim/v1/network.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/supersim/v1/network_access_profile/__init__.py` & `twilio-8.2.1/twilio/rest/supersim/v1/network_access_profile/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/supersim/v1/network_access_profile/network_access_profile_network.py` & `twilio-8.2.1/twilio/rest/supersim/v1/network_access_profile/network_access_profile_network.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/supersim/v1/settings_update.py` & `twilio-8.2.1/twilio/rest/supersim/v1/settings_update.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/supersim/v1/sim/__init__.py` & `twilio-8.2.1/twilio/rest/supersim/v1/sim/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/supersim/v1/sim/billing_period.py` & `twilio-8.2.1/twilio/rest/supersim/v1/sim/billing_period.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/supersim/v1/sim/sim_ip_address.py` & `twilio-8.2.1/twilio/rest/supersim/v1/sim/sim_ip_address.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/supersim/v1/sms_command.py` & `twilio-8.2.1/twilio/rest/supersim/v1/sms_command.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/supersim/v1/usage_record.py` & `twilio-8.2.1/twilio/rest/supersim/v1/usage_record.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/sync/SyncBase.py` & `twilio-8.2.1/twilio/rest/sync/SyncBase.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/sync/v1/__init__.py` & `twilio-8.2.1/twilio/rest/sync/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/sync/v1/service/__init__.py` & `twilio-8.2.1/twilio/rest/sync/v1/service/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/sync/v1/service/document/__init__.py` & `twilio-8.2.1/twilio/rest/sync/v1/service/document/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/sync/v1/service/document/document_permission.py` & `twilio-8.2.1/twilio/rest/sync/v1/service/document/document_permission.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/sync/v1/service/sync_list/__init__.py` & `twilio-8.2.1/twilio/rest/sync/v1/service/sync_list/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/sync/v1/service/sync_list/sync_list_item.py` & `twilio-8.2.1/twilio/rest/sync/v1/service/sync_list/sync_list_item.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/sync/v1/service/sync_list/sync_list_permission.py` & `twilio-8.2.1/twilio/rest/sync/v1/service/sync_list/sync_list_permission.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/sync/v1/service/sync_map/__init__.py` & `twilio-8.2.1/twilio/rest/sync/v1/service/sync_map/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/sync/v1/service/sync_map/sync_map_item.py` & `twilio-8.2.1/twilio/rest/sync/v1/service/sync_map/sync_map_item.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/sync/v1/service/sync_map/sync_map_permission.py` & `twilio-8.2.1/twilio/rest/sync/v1/service/sync_map/sync_map_permission.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/sync/v1/service/sync_stream/__init__.py` & `twilio-8.2.1/twilio/rest/sync/v1/service/sync_stream/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/sync/v1/service/sync_stream/stream_message.py` & `twilio-8.2.1/twilio/rest/sync/v1/service/sync_stream/stream_message.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/taskrouter/TaskrouterBase.py` & `twilio-8.2.1/twilio/rest/taskrouter/TaskrouterBase.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/taskrouter/v1/__init__.py` & `twilio-8.2.1/twilio/rest/taskrouter/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/taskrouter/v1/workspace/__init__.py` & `twilio-8.2.1/twilio/rest/taskrouter/v1/workspace/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/taskrouter/v1/workspace/activity.py` & `twilio-8.2.1/twilio/rest/taskrouter/v1/workspace/activity.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/taskrouter/v1/workspace/event.py` & `twilio-8.2.1/twilio/rest/taskrouter/v1/workspace/event.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/taskrouter/v1/workspace/task/__init__.py` & `twilio-8.2.1/twilio/rest/taskrouter/v1/workspace/task/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/taskrouter/v1/workspace/task/reservation.py` & `twilio-8.2.1/twilio/rest/taskrouter/v1/workspace/task/reservation.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/taskrouter/v1/workspace/task_channel.py` & `twilio-8.2.1/twilio/rest/taskrouter/v1/workspace/task_channel.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/taskrouter/v1/workspace/task_queue/__init__.py` & `twilio-8.2.1/twilio/rest/taskrouter/v1/workspace/task_queue/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/taskrouter/v1/workspace/task_queue/task_queue_cumulative_statistics.py` & `twilio-8.2.1/twilio/rest/taskrouter/v1/workspace/task_queue/task_queue_cumulative_statistics.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/taskrouter/v1/workspace/task_queue/task_queue_real_time_statistics.py` & `twilio-8.2.1/twilio/rest/taskrouter/v1/workspace/task_queue/task_queue_real_time_statistics.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/taskrouter/v1/workspace/task_queue/task_queue_statistics.py` & `twilio-8.2.1/twilio/rest/taskrouter/v1/workspace/task_queue/task_queue_statistics.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/taskrouter/v1/workspace/task_queue/task_queues_statistics.py` & `twilio-8.2.1/twilio/rest/taskrouter/v1/workspace/task_queue/task_queues_statistics.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/taskrouter/v1/workspace/worker/__init__.py` & `twilio-8.2.1/twilio/rest/taskrouter/v1/workspace/worker/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/taskrouter/v1/workspace/worker/reservation.py` & `twilio-8.2.1/twilio/rest/taskrouter/v1/workspace/worker/reservation.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/taskrouter/v1/workspace/worker/worker_channel.py` & `twilio-8.2.1/twilio/rest/taskrouter/v1/workspace/worker/worker_channel.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/taskrouter/v1/workspace/worker/worker_statistics.py` & `twilio-8.2.1/twilio/rest/taskrouter/v1/workspace/worker/worker_statistics.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/taskrouter/v1/workspace/worker/workers_cumulative_statistics.py` & `twilio-8.2.1/twilio/rest/taskrouter/v1/workspace/worker/workers_cumulative_statistics.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/taskrouter/v1/workspace/worker/workers_real_time_statistics.py` & `twilio-8.2.1/twilio/rest/taskrouter/v1/workspace/worker/workers_real_time_statistics.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/taskrouter/v1/workspace/worker/workers_statistics.py` & `twilio-8.2.1/twilio/rest/taskrouter/v1/workspace/worker/workers_statistics.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/taskrouter/v1/workspace/workflow/__init__.py` & `twilio-8.2.1/twilio/rest/taskrouter/v1/workspace/workflow/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/taskrouter/v1/workspace/workflow/workflow_cumulative_statistics.py` & `twilio-8.2.1/twilio/rest/taskrouter/v1/workspace/workflow/workflow_cumulative_statistics.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/taskrouter/v1/workspace/workflow/workflow_real_time_statistics.py` & `twilio-8.2.1/twilio/rest/taskrouter/v1/workspace/workflow/workflow_real_time_statistics.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/taskrouter/v1/workspace/workflow/workflow_statistics.py` & `twilio-8.2.1/twilio/rest/taskrouter/v1/workspace/workflow/workflow_statistics.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/taskrouter/v1/workspace/workspace_cumulative_statistics.py` & `twilio-8.2.1/twilio/rest/taskrouter/v1/workspace/workspace_cumulative_statistics.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/taskrouter/v1/workspace/workspace_real_time_statistics.py` & `twilio-8.2.1/twilio/rest/taskrouter/v1/workspace/workspace_real_time_statistics.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/taskrouter/v1/workspace/workspace_statistics.py` & `twilio-8.2.1/twilio/rest/taskrouter/v1/workspace/workspace_statistics.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/trunking/TrunkingBase.py` & `twilio-8.2.1/twilio/rest/trunking/TrunkingBase.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/trunking/v1/__init__.py` & `twilio-8.2.1/twilio/rest/trunking/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/trunking/v1/trunk/__init__.py` & `twilio-8.2.1/twilio/rest/trunking/v1/trunk/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/trunking/v1/trunk/credential_list.py` & `twilio-8.2.1/twilio/rest/trunking/v1/trunk/credential_list.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/trunking/v1/trunk/ip_access_control_list.py` & `twilio-8.2.1/twilio/rest/trunking/v1/trunk/ip_access_control_list.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/trunking/v1/trunk/origination_url.py` & `twilio-8.2.1/twilio/rest/trunking/v1/trunk/origination_url.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/trunking/v1/trunk/phone_number.py` & `twilio-8.2.1/twilio/rest/trunking/v1/trunk/phone_number.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/trunking/v1/trunk/recording.py` & `twilio-8.2.1/twilio/rest/trunking/v1/trunk/recording.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/trusthub/TrusthubBase.py` & `twilio-8.2.1/twilio/rest/trusthub/TrusthubBase.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/trusthub/__init__.py` & `twilio-8.2.1/twilio/rest/trusthub/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/trusthub/v1/__init__.py` & `twilio-8.2.1/twilio/rest/trusthub/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/trusthub/v1/customer_profiles/__init__.py` & `twilio-8.2.1/twilio/rest/trusthub/v1/customer_profiles/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/trusthub/v1/customer_profiles/customer_profiles_channel_endpoint_assignment.py` & `twilio-8.2.1/twilio/rest/trusthub/v1/customer_profiles/customer_profiles_channel_endpoint_assignment.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/trusthub/v1/customer_profiles/customer_profiles_entity_assignments.py` & `twilio-8.2.1/twilio/rest/trusthub/v1/customer_profiles/customer_profiles_entity_assignments.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/trusthub/v1/customer_profiles/customer_profiles_evaluations.py` & `twilio-8.2.1/twilio/rest/trusthub/v1/customer_profiles/customer_profiles_evaluations.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/trusthub/v1/end_user.py` & `twilio-8.2.1/twilio/rest/trusthub/v1/end_user.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/trusthub/v1/end_user_type.py` & `twilio-8.2.1/twilio/rest/trusthub/v1/end_user_type.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/trusthub/v1/policies.py` & `twilio-8.2.1/twilio/rest/trusthub/v1/policies.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/trusthub/v1/supporting_document.py` & `twilio-8.2.1/twilio/rest/trusthub/v1/supporting_document.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/trusthub/v1/supporting_document_type.py` & `twilio-8.2.1/twilio/rest/trusthub/v1/supporting_document_type.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/trusthub/v1/trust_products/__init__.py` & `twilio-8.2.1/twilio/rest/trusthub/v1/trust_products/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/trusthub/v1/trust_products/trust_products_channel_endpoint_assignment.py` & `twilio-8.2.1/twilio/rest/trusthub/v1/trust_products/trust_products_channel_endpoint_assignment.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/trusthub/v1/trust_products/trust_products_entity_assignments.py` & `twilio-8.2.1/twilio/rest/trusthub/v1/trust_products/trust_products_entity_assignments.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/trusthub/v1/trust_products/trust_products_evaluations.py` & `twilio-8.2.1/twilio/rest/trusthub/v1/trust_products/trust_products_evaluations.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/verify/VerifyBase.py` & `twilio-8.2.1/twilio/rest/verify/VerifyBase.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/verify/__init__.py` & `twilio-8.2.1/twilio/rest/verify/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/verify/v2/__init__.py` & `twilio-8.2.1/twilio/rest/verify/v2/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/verify/v2/form.py` & `twilio-8.2.1/twilio/rest/verify/v2/form.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/verify/v2/safelist.py` & `twilio-8.2.1/twilio/rest/verify/v2/safelist.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/verify/v2/service/__init__.py` & `twilio-8.2.1/twilio/rest/verify/v2/service/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/verify/v2/service/entity/__init__.py` & `twilio-8.2.1/twilio/rest/verify/v2/service/entity/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/verify/v2/service/entity/challenge/__init__.py` & `twilio-8.2.1/twilio/rest/verify/v2/service/entity/challenge/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/verify/v2/service/entity/challenge/notification.py` & `twilio-8.2.1/twilio/rest/verify/v2/service/entity/challenge/notification.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/verify/v2/service/entity/factor.py` & `twilio-8.2.1/twilio/rest/verify/v2/service/entity/factor.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/verify/v2/service/entity/new_factor.py` & `twilio-8.2.1/twilio/rest/verify/v2/service/entity/new_factor.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/verify/v2/service/messaging_configuration.py` & `twilio-8.2.1/twilio/rest/verify/v2/service/messaging_configuration.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/verify/v2/service/rate_limit/__init__.py` & `twilio-8.2.1/twilio/rest/verify/v2/service/rate_limit/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/verify/v2/service/rate_limit/bucket.py` & `twilio-8.2.1/twilio/rest/verify/v2/service/rate_limit/bucket.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/verify/v2/service/verification.py` & `twilio-8.2.1/twilio/rest/verify/v2/service/verification.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/verify/v2/service/verification_check.py` & `twilio-8.2.1/twilio/rest/verify/v2/service/verification_check.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/verify/v2/service/webhook.py` & `twilio-8.2.1/twilio/rest/verify/v2/service/webhook.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/verify/v2/template.py` & `twilio-8.2.1/twilio/rest/verify/v2/template.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/verify/v2/verification_attempt.py` & `twilio-8.2.1/twilio/rest/verify/v2/verification_attempt.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/verify/v2/verification_attempts_summary.py` & `twilio-8.2.1/twilio/rest/verify/v2/verification_attempts_summary.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/video/VideoBase.py` & `twilio-8.2.1/twilio/rest/voice/VoiceBase.py`

 * *Files 11% similar despite different names*

```diff
@@ -9,35 +9,35 @@
   Do not edit the class manually.
 """
 
 from typing import Optional
 
 from twilio.base.domain import Domain
 from twilio.rest import Client
-from twilio.rest.video.v1 import V1
+from twilio.rest.voice.v1 import V1
 
 
-class VideoBase(Domain):
+class VoiceBase(Domain):
     def __init__(self, twilio: Client):
         """
-        Initialize the Video Domain
+        Initialize the Voice Domain
 
-        :returns: Domain for Video
+        :returns: Domain for Voice
         """
-        super().__init__(twilio, "https://video.twilio.com")
+        super().__init__(twilio, "https://voice.twilio.com")
         self._v1: Optional[V1] = None
 
     @property
     def v1(self) -> V1:
         """
-        :returns: Versions v1 of Video
+        :returns: Versions v1 of Voice
         """
         if self._v1 is None:
             self._v1 = V1(self)
         return self._v1
 
     def __repr__(self) -> str:
         """
         Provide a friendly representation
         :returns: Machine friendly representation
         """
-        return "<Twilio.Video>"
+        return "<Twilio.Voice>"
```

### Comparing `twilio-8.2.0/twilio/rest/video/__init__.py` & `twilio-8.2.1/twilio/rest/video/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/video/v1/__init__.py` & `twilio-8.2.1/twilio/rest/video/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/video/v1/composition.py` & `twilio-8.2.1/twilio/rest/video/v1/composition.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/video/v1/composition_hook.py` & `twilio-8.2.1/twilio/rest/video/v1/composition_hook.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/video/v1/composition_settings.py` & `twilio-8.2.1/twilio/rest/video/v1/composition_settings.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/video/v1/recording.py` & `twilio-8.2.1/twilio/rest/video/v1/recording.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/video/v1/recording_settings.py` & `twilio-8.2.1/twilio/rest/video/v1/recording_settings.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/video/v1/room/__init__.py` & `twilio-8.2.1/twilio/rest/video/v1/room/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/video/v1/room/participant/__init__.py` & `twilio-8.2.1/twilio/rest/video/v1/room/participant/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/video/v1/room/participant/anonymize.py` & `twilio-8.2.1/twilio/rest/video/v1/room/participant/anonymize.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/video/v1/room/participant/published_track.py` & `twilio-8.2.1/twilio/rest/video/v1/room/participant/published_track.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/video/v1/room/participant/subscribe_rules.py` & `twilio-8.2.1/twilio/rest/video/v1/room/participant/subscribe_rules.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/video/v1/room/participant/subscribed_track.py` & `twilio-8.2.1/twilio/rest/video/v1/room/participant/subscribed_track.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/video/v1/room/recording_rules.py` & `twilio-8.2.1/twilio/rest/video/v1/room/recording_rules.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/video/v1/room/room_recording.py` & `twilio-8.2.1/twilio/rest/video/v1/room/room_recording.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/voice/VoiceBase.py` & `twilio-8.2.1/twilio/rest/numbers/NumbersBase.py`

 * *Files 9% similar despite different names*

```diff
@@ -9,35 +9,46 @@
   Do not edit the class manually.
 """
 
 from typing import Optional
 
 from twilio.base.domain import Domain
 from twilio.rest import Client
-from twilio.rest.voice.v1 import V1
+from twilio.rest.numbers.v1 import V1
+from twilio.rest.numbers.v2 import V2
 
 
-class VoiceBase(Domain):
+class NumbersBase(Domain):
     def __init__(self, twilio: Client):
         """
-        Initialize the Voice Domain
+        Initialize the Numbers Domain
 
-        :returns: Domain for Voice
+        :returns: Domain for Numbers
         """
-        super().__init__(twilio, "https://voice.twilio.com")
+        super().__init__(twilio, "https://numbers.twilio.com")
         self._v1: Optional[V1] = None
+        self._v2: Optional[V2] = None
 
     @property
     def v1(self) -> V1:
         """
-        :returns: Versions v1 of Voice
+        :returns: Versions v1 of Numbers
         """
         if self._v1 is None:
             self._v1 = V1(self)
         return self._v1
 
+    @property
+    def v2(self) -> V2:
+        """
+        :returns: Versions v2 of Numbers
+        """
+        if self._v2 is None:
+            self._v2 = V2(self)
+        return self._v2
+
     def __repr__(self) -> str:
         """
         Provide a friendly representation
         :returns: Machine friendly representation
         """
-        return "<Twilio.Voice>"
+        return "<Twilio.Numbers>"
```

### Comparing `twilio-8.2.0/twilio/rest/voice/__init__.py` & `twilio-8.2.1/twilio/rest/voice/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/voice/v1/__init__.py` & `twilio-8.2.1/twilio/rest/voice/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/voice/v1/archived_call.py` & `twilio-8.2.1/twilio/rest/voice/v1/archived_call.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/voice/v1/byoc_trunk.py` & `twilio-8.2.1/twilio/rest/voice/v1/byoc_trunk.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/voice/v1/connection_policy/__init__.py` & `twilio-8.2.1/twilio/rest/voice/v1/connection_policy/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/voice/v1/connection_policy/connection_policy_target.py` & `twilio-8.2.1/twilio/rest/voice/v1/connection_policy/connection_policy_target.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/voice/v1/dialing_permissions/__init__.py` & `twilio-8.2.1/twilio/rest/voice/v1/dialing_permissions/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/voice/v1/dialing_permissions/bulk_country_update.py` & `twilio-8.2.1/twilio/rest/voice/v1/dialing_permissions/bulk_country_update.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/voice/v1/dialing_permissions/country/__init__.py` & `twilio-8.2.1/twilio/rest/voice/v1/dialing_permissions/country/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/voice/v1/dialing_permissions/country/highrisk_special_prefix.py` & `twilio-8.2.1/twilio/rest/voice/v1/dialing_permissions/country/highrisk_special_prefix.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/voice/v1/dialing_permissions/settings.py` & `twilio-8.2.1/twilio/rest/voice/v1/dialing_permissions/settings.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/voice/v1/ip_record.py` & `twilio-8.2.1/twilio/rest/voice/v1/ip_record.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/voice/v1/source_ip_mapping.py` & `twilio-8.2.1/twilio/rest/voice/v1/source_ip_mapping.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/wireless/WirelessBase.py` & `twilio-8.2.1/twilio/rest/wireless/WirelessBase.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/wireless/__init__.py` & `twilio-8.2.1/twilio/rest/wireless/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/wireless/v1/__init__.py` & `twilio-8.2.1/twilio/rest/wireless/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/wireless/v1/command.py` & `twilio-8.2.1/twilio/rest/wireless/v1/command.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/wireless/v1/rate_plan.py` & `twilio-8.2.1/twilio/rest/wireless/v1/rate_plan.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/wireless/v1/sim/__init__.py` & `twilio-8.2.1/twilio/rest/wireless/v1/sim/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/wireless/v1/sim/data_session.py` & `twilio-8.2.1/twilio/rest/wireless/v1/sim/data_session.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/wireless/v1/sim/usage_record.py` & `twilio-8.2.1/twilio/rest/wireless/v1/sim/usage_record.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/rest/wireless/v1/usage_record.py` & `twilio-8.2.1/twilio/rest/wireless/v1/usage_record.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/twiml/__init__.py` & `twilio-8.2.1/twilio/twiml/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/twiml/fax_response.py` & `twilio-8.2.1/twilio/twiml/fax_response.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/twiml/messaging_response.py` & `twilio-8.2.1/twilio/twiml/messaging_response.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio/twiml/voice_response.py` & `twilio-8.2.1/twilio/twiml/voice_response.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.0/twilio.egg-info/PKG-INFO` & `twilio-8.2.1/twilio.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: twilio
-Version: 8.2.0
+Version: 8.2.1
 Summary: Twilio API client and TwiML generator
 Home-page: https://github.com/twilio/twilio-python/
 Author: Twilio
 Author-email: help@twilio.com
 Keywords: twilio,twiml
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `twilio-8.2.0/twilio.egg-info/SOURCES.txt` & `twilio-8.2.1/twilio.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -314,14 +314,15 @@
 twilio/rest/messaging/v1/__init__.py
 twilio/rest/messaging/v1/deactivations.py
 twilio/rest/messaging/v1/domain_certs.py
 twilio/rest/messaging/v1/domain_config.py
 twilio/rest/messaging/v1/domain_config_messaging_service.py
 twilio/rest/messaging/v1/external_campaign.py
 twilio/rest/messaging/v1/linkshortening_messaging_service.py
+twilio/rest/messaging/v1/linkshortening_messaging_service_domain_association.py
 twilio/rest/messaging/v1/usecase.py
 twilio/rest/messaging/v1/brand_registration/__init__.py
 twilio/rest/messaging/v1/brand_registration/brand_registration_otp.py
 twilio/rest/messaging/v1/brand_registration/brand_vetting.py
 twilio/rest/messaging/v1/service/__init__.py
 twilio/rest/messaging/v1/service/alpha_sender.py
 twilio/rest/messaging/v1/service/phone_number.py
@@ -348,14 +349,16 @@
 twilio/rest/notify/v1/__init__.py
 twilio/rest/notify/v1/credential.py
 twilio/rest/notify/v1/service/__init__.py
 twilio/rest/notify/v1/service/binding.py
 twilio/rest/notify/v1/service/notification.py
 twilio/rest/numbers/NumbersBase.py
 twilio/rest/numbers/__init__.py
+twilio/rest/numbers/v1/__init__.py
+twilio/rest/numbers/v1/bulk_eligibility.py
 twilio/rest/numbers/v2/__init__.py
 twilio/rest/numbers/v2/regulatory_compliance/__init__.py
 twilio/rest/numbers/v2/regulatory_compliance/end_user.py
 twilio/rest/numbers/v2/regulatory_compliance/end_user_type.py
 twilio/rest/numbers/v2/regulatory_compliance/regulation.py
 twilio/rest/numbers/v2/regulatory_compliance/supporting_document.py
 twilio/rest/numbers/v2/regulatory_compliance/supporting_document_type.py
```

