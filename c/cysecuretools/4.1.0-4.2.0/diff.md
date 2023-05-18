# Comparing `tmp/cysecuretools-4.1.0.tar.gz` & `tmp/cysecuretools-4.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/ihos/venv/github/dist/tmp5_qxdefx/cysecuretools-4.1.0.tar", last modified: Fri Sep 16 09:50:32 2022, max compression
+gzip compressed data, was "cysecuretools-4.2.0.tar", last modified: Thu May 18 10:54:49 2023, max compression
```

## Comparing `cysecuretools-4.1.0.tar` & `cysecuretools-4.2.0.tar`

### file list

```diff
@@ -1,366 +1,406 @@
-drwxr-xr-x   0 ihos       (501) staff       (20)        0 2022-09-16 09:50:32.000000 cysecuretools-4.1.0/
--rw-r--r--   0 ihos       (501) staff       (20)      582 2022-09-16 09:05:01.000000 cysecuretools-4.1.0/LICENSE
--rw-r--r--   0 ihos       (501) staff       (20)      934 2022-09-16 09:06:31.000000 cysecuretools-4.1.0/MANIFEST.in
--rw-r--r--   0 ihos       (501) staff       (20)     8057 2022-09-16 09:50:32.000000 cysecuretools-4.1.0/PKG-INFO
--rw-r--r--   0 ihos       (501) staff       (20)     5100 2022-09-16 09:06:31.000000 cysecuretools-4.1.0/README.md
-drwxr-xr-x   0 ihos       (501) staff       (20)        0 2022-09-16 09:50:32.000000 cysecuretools-4.1.0/cysecuretools/
--rw-r--r--   0 ihos       (501) staff       (20)      631 2022-09-16 09:05:01.000000 cysecuretools-4.1.0/cysecuretools/__init__.py
--rw-r--r--   0 ihos       (501) staff       (20)      714 2022-09-16 09:05:01.000000 cysecuretools-4.1.0/cysecuretools/__main__.py
--rw-r--r--   0 ihos       (501) staff       (20)    10726 2022-09-16 09:06:31.000000 cysecuretools-4.1.0/cysecuretools/cli.py
--rw-r--r--   0 ihos       (501) staff       (20)     6064 2022-09-16 09:05:01.000000 cysecuretools-4.1.0/cysecuretools/cli_creator.py
--rw-r--r--   0 ihos       (501) staff       (20)    33805 2022-09-16 09:06:31.000000 cysecuretools-4.1.0/cysecuretools/cli_mxs40sv2.py
--rw-r--r--   0 ihos       (501) staff       (20)    27453 2022-09-16 09:05:01.000000 cysecuretools-4.1.0/cysecuretools/cli_mxs40v1.py
-drwxr-xr-x   0 ihos       (501) staff       (20)        0 2022-09-16 09:50:32.000000 cysecuretools-4.1.0/cysecuretools/core/
--rw-r--r--   0 ihos       (501) staff       (20)     1098 2022-09-16 09:05:01.000000 cysecuretools-4.1.0/cysecuretools/core/__init__.py
--rw-r--r--   0 ihos       (501) staff       (20)      784 2022-09-16 09:05:01.000000 cysecuretools-4.1.0/cysecuretools/core/bitops.py
-drwxr-xr-x   0 ihos       (501) staff       (20)        0 2022-09-16 09:50:32.000000 cysecuretools-4.1.0/cysecuretools/core/certificates/
--rw-r--r--   0 ihos       (501) staff       (20)        0 2022-09-16 09:05:01.000000 cysecuretools-4.1.0/cysecuretools/core/certificates/__init__.py
--rw-r--r--   0 ihos       (501) staff       (20)     9866 2022-09-16 09:05:01.000000 cysecuretools-4.1.0/cysecuretools/core/certificates/x509.py
--rw-r--r--   0 ihos       (501) staff       (20)     4676 2022-09-16 09:06:31.000000 cysecuretools-4.1.0/cysecuretools/core/connect_helper.py
--rw-r--r--   0 ihos       (501) staff       (20)     2230 2022-09-16 09:05:01.000000 cysecuretools-4.1.0/cysecuretools/core/cy_bootloader_map_parser.py
--rw-r--r--   0 ihos       (501) staff       (20)     1259 2022-09-16 09:05:01.000000 cysecuretools-4.1.0/cysecuretools/core/dependecy_validator.py
--rw-r--r--   0 ihos       (501) staff       (20)      935 2022-09-16 09:05:01.000000 cysecuretools-4.1.0/cysecuretools/core/entrance_exam_base.py
--rw-r--r--   0 ihos       (501) staff       (20)     1450 2022-09-16 09:05:01.000000 cysecuretools-4.1.0/cysecuretools/core/enums.py
--rw-r--r--   0 ihos       (501) staff       (20)      736 2022-09-16 09:05:01.000000 cysecuretools-4.1.0/cysecuretools/core/exceptions.py
--rw-r--r--   0 ihos       (501) staff       (20)     1384 2022-09-16 09:05:01.000000 cysecuretools-4.1.0/cysecuretools/core/json_helper.py
--rw-r--r--   0 ihos       (501) staff       (20)     1674 2022-09-16 09:05:01.000000 cysecuretools-4.1.0/cysecuretools/core/jsonpath.py
--rw-r--r--   0 ihos       (501) staff       (20)     2144 2022-09-16 09:05:01.000000 cysecuretools-4.1.0/cysecuretools/core/key_data.py
-drwxr-xr-x   0 ihos       (501) staff       (20)        0 2022-09-16 09:50:32.000000 cysecuretools-4.1.0/cysecuretools/core/key_handlers/
--rw-r--r--   0 ihos       (501) staff       (20)       67 2022-09-16 09:05:01.000000 cysecuretools-4.1.0/cysecuretools/core/key_handlers/__init__.py
--rw-r--r--   0 ihos       (501) staff       (20)     2539 2022-09-16 09:05:01.000000 cysecuretools-4.1.0/cysecuretools/core/key_handlers/ec_handler.py
--rw-r--r--   0 ihos       (501) staff       (20)     3889 2022-09-16 09:05:01.000000 cysecuretools-4.1.0/cysecuretools/core/key_handlers/rsa_handler.py
--rw-r--r--   0 ihos       (501) staff       (20)     2280 2022-09-16 09:05:01.000000 cysecuretools-4.1.0/cysecuretools/core/key_helper.py
--rw-r--r--   0 ihos       (501) staff       (20)     2237 2022-09-16 09:05:01.000000 cysecuretools-4.1.0/cysecuretools/core/logging_configurator.py
--rw-r--r--   0 ihos       (501) staff       (20)     2401 2022-09-16 09:05:01.000000 cysecuretools-4.1.0/cysecuretools/core/logging_formatter.py
--rw-r--r--   0 ihos       (501) staff       (20)      701 2022-09-16 09:05:01.000000 cysecuretools-4.1.0/cysecuretools/core/memory_area.py
--rw-r--r--   0 ihos       (501) staff       (20)     1985 2022-09-16 09:05:01.000000 cysecuretools-4.1.0/cysecuretools/core/memory_map_base.py
--rw-r--r--   0 ihos       (501) staff       (20)     2209 2022-09-16 09:05:01.000000 cysecuretools-4.1.0/cysecuretools/core/ocd_settings.py
--rw-r--r--   0 ihos       (501) staff       (20)      840 2022-09-16 09:05:01.000000 cysecuretools-4.1.0/cysecuretools/core/policy_filter_base.py
--rw-r--r--   0 ihos       (501) staff       (20)      954 2022-09-16 09:05:01.000000 cysecuretools-4.1.0/cysecuretools/core/policy_validator_base.py
--rw-r--r--   0 ihos       (501) staff       (20)      783 2022-09-16 09:05:01.000000 cysecuretools-4.1.0/cysecuretools/core/progress_bar.py
--rw-r--r--   0 ihos       (501) staff       (20)     6765 2022-09-16 09:05:01.000000 cysecuretools-4.1.0/cysecuretools/core/project.py
-drwxr-xr-x   0 ihos       (501) staff       (20)        0 2022-09-16 09:50:32.000000 cysecuretools-4.1.0/cysecuretools/core/provisioning_flows/
--rw-r--r--   0 ihos       (501) staff       (20)      134 2022-09-16 09:05:01.000000 cysecuretools-4.1.0/cysecuretools/core/provisioning_flows/__init__.py
--rw-r--r--   0 ihos       (501) staff       (20)      716 2022-09-16 09:05:01.000000 cysecuretools-4.1.0/cysecuretools/core/provisioning_flows/application.py
--rw-r--r--   0 ihos       (501) staff       (20)      894 2022-09-16 09:05:01.000000 cysecuretools-4.1.0/cysecuretools/core/provisioning_flows/flow.py
--rw-r--r--   0 ihos       (501) staff       (20)     3267 2022-09-16 09:05:01.000000 cysecuretools-4.1.0/cysecuretools/core/register_map_base.py
--rw-r--r--   0 ihos       (501) staff       (20)     1216 2022-09-16 09:05:01.000000 cysecuretools-4.1.0/cysecuretools/core/signtool_base.py
-drwxr-xr-x   0 ihos       (501) staff       (20)        0 2022-09-16 09:50:32.000000 cysecuretools-4.1.0/cysecuretools/core/strategy_context/
--rw-r--r--   0 ihos       (501) staff       (20)      107 2022-09-16 09:05:01.000000 cysecuretools-4.1.0/cysecuretools/core/strategy_context/__init__.py
--rw-r--r--   0 ihos       (501) staff       (20)     2062 2022-09-16 09:05:01.000000 cysecuretools-4.1.0/cysecuretools/core/strategy_context/cert_strategy_ctx.py
--rw-r--r--   0 ihos       (501) staff       (20)     2812 2022-09-16 09:05:01.000000 cysecuretools-4.1.0/cysecuretools/core/strategy_context/encrypted_programming_strategy_ctx.py
--rw-r--r--   0 ihos       (501) staff       (20)     1997 2022-09-16 09:05:01.000000 cysecuretools-4.1.0/cysecuretools/core/strategy_context/prov_packet_strategy_ctx.py
--rw-r--r--   0 ihos       (501) staff       (20)     2619 2022-09-16 09:05:01.000000 cysecuretools-4.1.0/cysecuretools/core/strategy_context/provisioning_strategy_ctx.py
--rw-r--r--   0 ihos       (501) staff       (20)      716 2022-09-16 09:05:01.000000 cysecuretools-4.1.0/cysecuretools/core/strops.py
--rw-r--r--   0 ihos       (501) staff       (20)     4196 2022-09-16 09:06:31.000000 cysecuretools-4.1.0/cysecuretools/core/target_builder.py
--rw-r--r--   0 ihos       (501) staff       (20)    11421 2022-09-16 09:06:31.000000 cysecuretools-4.1.0/cysecuretools/core/target_director.py
--rw-r--r--   0 ihos       (501) staff       (20)      847 2022-09-16 09:05:01.000000 cysecuretools-4.1.0/cysecuretools/core/voltage_tool.py
-drwxr-xr-x   0 ihos       (501) staff       (20)        0 2022-09-16 09:50:32.000000 cysecuretools-4.1.0/cysecuretools/data/
--rw-r--r--   0 ihos       (501) staff       (20)        0 2022-09-16 09:05:01.000000 cysecuretools-4.1.0/cysecuretools/data/__init__.py
--rw-r--r--   0 ihos       (501) staff       (20)     1544 2022-09-16 09:05:01.000000 cysecuretools-4.1.0/cysecuretools/data/cy_bootloader_map.json
-drwxr-xr-x   0 ihos       (501) staff       (20)        0 2022-09-16 09:50:32.000000 cysecuretools-4.1.0/cysecuretools/data/mxs40sv2/
--rw-r--r--   0 ihos       (501) staff       (20)     4698 2022-09-16 09:05:01.000000 cysecuretools-4.1.0/cysecuretools/data/mxs40sv2/mxs40sv2_ram_app_status_codes.py
-drwxr-xr-x   0 ihos       (501) staff       (20)        0 2022-09-16 09:50:32.000000 cysecuretools-4.1.0/cysecuretools/data/mxs40v1/
--rw-r--r--   0 ihos       (501) staff       (20)        0 2022-09-16 09:05:01.000000 cysecuretools-4.1.0/cysecuretools/data/mxs40v1/__init__.py
--rw-r--r--   0 ihos       (501) staff       (20)    13578 2022-09-16 09:05:01.000000 cysecuretools-4.1.0/cysecuretools/data/mxs40v1/mxs40v1_sfb_status_codes.py
-drwxr-xr-x   0 ihos       (501) staff       (20)        0 2022-09-16 09:50:32.000000 cysecuretools-4.1.0/cysecuretools/execute/
--rw-r--r--   0 ihos       (501) staff       (20)        0 2022-09-16 09:05:01.000000 cysecuretools-4.1.0/cysecuretools/execute/__init__.py
--rw-r--r--   0 ihos       (501) staff       (20)     3086 2022-09-16 09:05:01.000000 cysecuretools-4.1.0/cysecuretools/execute/bootloader_provider_mxs40v1.py
-drwxr-xr-x   0 ihos       (501) staff       (20)        0 2022-09-16 09:50:32.000000 cysecuretools-4.1.0/cysecuretools/execute/debug_cert/
--rw-r--r--   0 ihos       (501) staff       (20)       97 2022-09-16 09:05:01.000000 cysecuretools-4.1.0/cysecuretools/execute/debug_cert/__init__.py
--rw-r--r--   0 ihos       (501) staff       (20)     2924 2022-09-16 09:05:01.000000 cysecuretools-4.1.0/cysecuretools/execute/debug_cert/debug_cert_mxs40sv2.py
--rw-r--r--   0 ihos       (501) staff       (20)     4365 2022-09-16 09:05:01.000000 cysecuretools-4.1.0/cysecuretools/execute/debug_cert/debug_cert_parser_mxs40sv2.py
-drwxr-xr-x   0 ihos       (501) staff       (20)        0 2022-09-16 09:50:32.000000 cysecuretools-4.1.0/cysecuretools/execute/encrypted_programming/
--rw-r--r--   0 ihos       (501) staff       (20)        0 2022-09-16 09:05:01.000000 cysecuretools-4.1.0/cysecuretools/execute/encrypted_programming/__init__.py
--rw-r--r--   0 ihos       (501) staff       (20)     2459 2022-09-16 09:05:01.000000 cysecuretools-4.1.0/cysecuretools/execute/encrypted_programming/aes_cipher.py
--rw-r--r--   0 ihos       (501) staff       (20)     4024 2022-09-16 09:05:01.000000 cysecuretools-4.1.0/cysecuretools/execute/encrypted_programming/aes_header.py
--rw-r--r--   0 ihos       (501) staff       (20)     5550 2022-09-16 09:05:01.000000 cysecuretools-4.1.0/cysecuretools/execute/encrypted_programming/aes_header_strategy.py
--rw-r--r--   0 ihos       (501) staff       (20)     2857 2022-09-16 09:05:01.000000 cysecuretools-4.1.0/cysecuretools/execute/encrypted_programming/ecc_kdf.py
--rw-r--r--   0 ihos       (501) staff       (20)     3250 2022-09-16 09:05:01.000000 cysecuretools-4.1.0/cysecuretools/execute/encrypted_programming/encrypted_programming.py
-drwxr-xr-x   0 ihos       (501) staff       (20)        0 2022-09-16 09:50:32.000000 cysecuretools-4.1.0/cysecuretools/execute/entrance_exam/
--rw-r--r--   0 ihos       (501) staff       (20)        0 2022-09-16 09:05:01.000000 cysecuretools-4.1.0/cysecuretools/execute/entrance_exam/__init__.py
--rw-r--r--   0 ihos       (501) staff       (20)     8144 2022-09-16 09:05:01.000000 cysecuretools-4.1.0/cysecuretools/execute/entrance_exam/exam_cyb06xx7.py
--rw-r--r--   0 ihos       (501) staff       (20)     8287 2022-09-16 09:05:01.000000 cysecuretools-4.1.0/cysecuretools/execute/entrance_exam/exam_mxs40v1.py
--rw-r--r--   0 ihos       (501) staff       (20)     5062 2022-09-16 09:05:01.000000 cysecuretools-4.1.0/cysecuretools/execute/image_cert.py
-drwxr-xr-x   0 ihos       (501) staff       (20)        0 2022-09-16 09:50:32.000000 cysecuretools-4.1.0/cysecuretools/execute/image_signing/
--rw-r--r--   0 ihos       (501) staff       (20)        0 2022-09-16 09:05:01.000000 cysecuretools-4.1.0/cysecuretools/execute/image_signing/__init__.py
--rw-r--r--   0 ihos       (501) staff       (20)     3152 2022-09-16 09:05:01.000000 cysecuretools-4.1.0/cysecuretools/execute/image_signing/encrypt_mxv40sv2.py
--rw-r--r--   0 ihos       (501) staff       (20)     7260 2022-09-16 09:05:01.000000 cysecuretools-4.1.0/cysecuretools/execute/image_signing/image.py
--rw-r--r--   0 ihos       (501) staff       (20)     1450 2022-09-16 09:05:01.000000 cysecuretools-4.1.0/cysecuretools/execute/image_signing/image_config_parser.py
--rw-r--r--   0 ihos       (501) staff       (20)     3782 2022-09-16 09:05:01.000000 cysecuretools-4.1.0/cysecuretools/execute/image_signing/rsa_converter.py
--rw-r--r--   0 ihos       (501) staff       (20)    18774 2022-09-16 09:05:01.000000 cysecuretools-4.1.0/cysecuretools/execute/image_signing/signtool_mxs40v1.py
--rw-r--r--   0 ihos       (501) staff       (20)    17112 2022-09-16 09:06:31.000000 cysecuretools-4.1.0/cysecuretools/execute/image_signing/signtool_mxv40sv2.py
--rw-r--r--   0 ihos       (501) staff       (20)     1231 2022-09-16 09:05:01.000000 cysecuretools-4.1.0/cysecuretools/execute/image_signing/xip_encryptor.py
-drwxr-xr-x   0 ihos       (501) staff       (20)        0 2022-09-16 09:50:32.000000 cysecuretools-4.1.0/cysecuretools/execute/imgtool/
--rw-r--r--   0 ihos       (501) staff       (20)      650 2022-09-16 09:05:01.000000 cysecuretools-4.1.0/cysecuretools/execute/imgtool/__init__.py
--rw-r--r--   0 ihos       (501) staff       (20)     1613 2022-09-16 09:05:01.000000 cysecuretools-4.1.0/cysecuretools/execute/imgtool/boot_record.py
--rw-r--r--   0 ihos       (501) staff       (20)     1208 2022-09-16 09:05:01.000000 cysecuretools-4.1.0/cysecuretools/execute/imgtool/custom_encryptor.py
--rw-r--r--   0 ihos       (501) staff       (20)    25962 2022-09-16 09:05:01.000000 cysecuretools-4.1.0/cysecuretools/execute/imgtool/image.py
-drwxr-xr-x   0 ihos       (501) staff       (20)        0 2022-09-16 09:50:32.000000 cysecuretools-4.1.0/cysecuretools/execute/imgtool/keys/
--rw-r--r--   0 ihos       (501) staff       (20)     3737 2022-09-16 09:05:01.000000 cysecuretools-4.1.0/cysecuretools/execute/imgtool/keys/__init__.py
--rw-r--r--   0 ihos       (501) staff       (20)     5388 2022-09-16 09:05:01.000000 cysecuretools-4.1.0/cysecuretools/execute/imgtool/keys/ecdsa.py
--rw-r--r--   0 ihos       (501) staff       (20)     2970 2022-09-16 09:05:01.000000 cysecuretools-4.1.0/cysecuretools/execute/imgtool/keys/ecdsa_test.py
--rw-r--r--   0 ihos       (501) staff       (20)     3090 2022-09-16 09:05:01.000000 cysecuretools-4.1.0/cysecuretools/execute/imgtool/keys/ed25519.py
--rw-r--r--   0 ihos       (501) staff       (20)     3026 2022-09-16 09:05:01.000000 cysecuretools-4.1.0/cysecuretools/execute/imgtool/keys/ed25519_test.py
--rw-r--r--   0 ihos       (501) staff       (20)     1822 2022-09-16 09:05:01.000000 cysecuretools-4.1.0/cysecuretools/execute/imgtool/keys/general.py
--rw-r--r--   0 ihos       (501) staff       (20)     5422 2022-09-16 09:05:01.000000 cysecuretools-4.1.0/cysecuretools/execute/imgtool/keys/rsa.py
--rw-r--r--   0 ihos       (501) staff       (20)     3810 2022-09-16 09:05:01.000000 cysecuretools-4.1.0/cysecuretools/execute/imgtool/keys/rsa_test.py
--rw-r--r--   0 ihos       (501) staff       (20)     3169 2022-09-16 09:05:01.000000 cysecuretools-4.1.0/cysecuretools/execute/imgtool/keys/x25519.py
--rwxr-xr-x   0 ihos       (501) staff       (20)    18214 2022-09-16 09:06:31.000000 cysecuretools-4.1.0/cysecuretools/execute/imgtool/main.py
--rw-r--r--   0 ihos       (501) staff       (20)     1773 2022-09-16 09:05:01.000000 cysecuretools-4.1.0/cysecuretools/execute/imgtool/version.py
--rw-r--r--   0 ihos       (501) staff       (20)     2587 2022-09-16 09:05:01.000000 cysecuretools-4.1.0/cysecuretools/execute/jwt.py
--rw-r--r--   0 ihos       (501) staff       (20)     3924 2022-09-16 09:05:01.000000 cysecuretools-4.1.0/cysecuretools/execute/key_reader.py
--rw-r--r--   0 ihos       (501) staff       (20)     1956 2022-09-16 09:05:01.000000 cysecuretools-4.1.0/cysecuretools/execute/key_reader_mxs40v1.py
-drwxr-xr-x   0 ihos       (501) staff       (20)        0 2022-09-16 09:50:32.000000 cysecuretools-4.1.0/cysecuretools/execute/key_source/
--rw-r--r--   0 ihos       (501) staff       (20)        0 2022-09-16 09:05:01.000000 cysecuretools-4.1.0/cysecuretools/execute/key_source/__init__.py
--rw-r--r--   0 ihos       (501) staff       (20)     5174 2022-09-16 09:05:01.000000 cysecuretools-4.1.0/cysecuretools/execute/key_source/key_source_mxs40sv2.py
--rw-r--r--   0 ihos       (501) staff       (20)      825 2022-09-16 09:05:01.000000 cysecuretools-4.1.0/cysecuretools/execute/key_source/key_source_mxs40v1.py
--rw-r--r--   0 ihos       (501) staff       (20)     8023 2022-09-16 09:05:01.000000 cysecuretools-4.1.0/cysecuretools/execute/keygen.py
-drwxr-xr-x   0 ihos       (501) staff       (20)        0 2022-09-16 09:50:32.000000 cysecuretools-4.1.0/cysecuretools/execute/programmer/
--rw-r--r--   0 ihos       (501) staff       (20)      658 2022-09-16 09:05:01.000000 cysecuretools-4.1.0/cysecuretools/execute/programmer/__init__.py
--rw-r--r--   0 ihos       (501) staff       (20)     8711 2022-09-16 09:06:31.000000 cysecuretools-4.1.0/cysecuretools/execute/programmer/base.py
--rw-r--r--   0 ihos       (501) staff       (20)    12838 2022-09-16 09:06:31.000000 cysecuretools-4.1.0/cysecuretools/execute/programmer/openocd_server.py
--rw-r--r--   0 ihos       (501) staff       (20)      938 2022-09-16 09:05:01.000000 cysecuretools-4.1.0/cysecuretools/execute/programmer/openocd_target_map.json
--rw-r--r--   0 ihos       (501) staff       (20)    21778 2022-09-16 09:06:31.000000 cysecuretools-4.1.0/cysecuretools/execute/programmer/openocd_wrapper.py
--rw-r--r--   0 ihos       (501) staff       (20)     1009 2022-09-16 09:05:01.000000 cysecuretools-4.1.0/cysecuretools/execute/programmer/programmer.py
--rw-r--r--   0 ihos       (501) staff       (20)     1427 2022-09-16 09:05:01.000000 cysecuretools-4.1.0/cysecuretools/execute/programmer/pyocd_target_map.json
--rw-r--r--   0 ihos       (501) staff       (20)    16407 2022-09-16 09:06:31.000000 cysecuretools-4.1.0/cysecuretools/execute/programmer/pyocd_wrapper.py
-drwxr-xr-x   0 ihos       (501) staff       (20)        0 2022-09-16 09:50:32.000000 cysecuretools-4.1.0/cysecuretools/execute/project_init/
--rw-r--r--   0 ihos       (501) staff       (20)        0 2022-09-16 09:05:01.000000 cysecuretools-4.1.0/cysecuretools/execute/project_init/__init__.py
--rw-r--r--   0 ihos       (501) staff       (20)     7365 2022-09-16 09:05:01.000000 cysecuretools-4.1.0/cysecuretools/execute/project_init/project_init_mxs40sv2.py
--rw-r--r--   0 ihos       (501) staff       (20)     7933 2022-09-16 09:06:31.000000 cysecuretools-4.1.0/cysecuretools/execute/project_init/project_init_mxs40v1.py
-drwxr-xr-x   0 ihos       (501) staff       (20)        0 2022-09-16 09:50:32.000000 cysecuretools-4.1.0/cysecuretools/execute/provisioning/
--rw-r--r--   0 ihos       (501) staff       (20)      200 2022-09-16 09:05:01.000000 cysecuretools-4.1.0/cysecuretools/execute/provisioning/__init__.py
-drwxr-xr-x   0 ihos       (501) staff       (20)        0 2022-09-16 09:50:32.000000 cysecuretools-4.1.0/cysecuretools/execute/provisioning/flows/
--rw-r--r--   0 ihos       (501) staff       (20)      181 2022-09-16 09:05:01.000000 cysecuretools-4.1.0/cysecuretools/execute/provisioning/flows/__init__.py
--rw-r--r--   0 ihos       (501) staff       (20)     5753 2022-09-16 09:05:01.000000 cysecuretools-4.1.0/cysecuretools/execute/provisioning/flows/application_mxs40sv2.py
--rw-r--r--   0 ihos       (501) staff       (20)     3484 2022-09-16 09:05:01.000000 cysecuretools-4.1.0/cysecuretools/execute/provisioning/flows/flow_mxs40sv2.py
--rw-r--r--   0 ihos       (501) staff       (20)     8975 2022-09-16 09:06:31.000000 cysecuretools-4.1.0/cysecuretools/execute/provisioning/load_ram_app.py
--rw-r--r--   0 ihos       (501) staff       (20)     7026 2022-09-16 09:05:01.000000 cysecuretools-4.1.0/cysecuretools/execute/provisioning/provision_device_mxs40sv2.py
--rw-r--r--   0 ihos       (501) staff       (20)    19770 2022-09-16 09:06:31.000000 cysecuretools-4.1.0/cysecuretools/execute/provisioning/provision_device_mxs40v1.py
-drwxr-xr-x   0 ihos       (501) staff       (20)        0 2022-09-16 09:50:32.000000 cysecuretools-4.1.0/cysecuretools/execute/provisioning_packet/
--rw-r--r--   0 ihos       (501) staff       (20)      107 2022-09-16 09:05:01.000000 cysecuretools-4.1.0/cysecuretools/execute/provisioning_packet/__init__.py
-drwxr-xr-x   0 ihos       (501) staff       (20)        0 2022-09-16 09:50:32.000000 cysecuretools-4.1.0/cysecuretools/execute/provisioning_packet/lib/
--rw-r--r--   0 ihos       (501) staff       (20)      564 2022-09-16 09:05:01.000000 cysecuretools-4.1.0/cysecuretools/execute/provisioning_packet/lib/__init__.py
--rw-r--r--   0 ihos       (501) staff       (20)     5407 2022-09-16 09:05:01.000000 cysecuretools-4.1.0/cysecuretools/execute/provisioning_packet/lib/cyprov_crypto.py
--rw-r--r--   0 ihos       (501) staff       (20)     1581 2022-09-16 09:05:01.000000 cysecuretools-4.1.0/cysecuretools/execute/provisioning_packet/lib/cyprov_customer.py
--rw-r--r--   0 ihos       (501) staff       (20)     3514 2022-09-16 09:05:01.000000 cysecuretools-4.1.0/cysecuretools/execute/provisioning_packet/lib/cyprov_dev.py
--rw-r--r--   0 ihos       (501) staff       (20)     1731 2022-09-16 09:05:01.000000 cysecuretools-4.1.0/cysecuretools/execute/provisioning_packet/lib/cyprov_entity.py
--rw-r--r--   0 ihos       (501) staff       (20)     3428 2022-09-16 09:05:01.000000 cysecuretools-4.1.0/cysecuretools/execute/provisioning_packet/lib/cyprov_hsm.py
--rw-r--r--   0 ihos       (501) staff       (20)     3153 2022-09-16 09:05:01.000000 cysecuretools-4.1.0/cysecuretools/execute/provisioning_packet/lib/cyprov_oem.py
--rw-r--r--   0 ihos       (501) staff       (20)     3672 2022-09-16 09:05:01.000000 cysecuretools-4.1.0/cysecuretools/execute/provisioning_packet/lib/cyprov_pem.py
--rw-r--r--   0 ihos       (501) staff       (20)     1049 2022-09-16 09:05:01.000000 cysecuretools-4.1.0/cysecuretools/execute/provisioning_packet/lib/cyprov_types.py
--rw-r--r--   0 ihos       (501) staff       (20)     6759 2022-09-16 09:05:01.000000 cysecuretools-4.1.0/cysecuretools/execute/provisioning_packet/provisioning_packet_mxs40sv2.py
--rw-r--r--   0 ihos       (501) staff       (20)     8310 2022-09-16 09:05:01.000000 cysecuretools-4.1.0/cysecuretools/execute/provisioning_packet/provisioning_packet_mxs40v1.py
-drwxr-xr-x   0 ihos       (501) staff       (20)        0 2022-09-16 09:50:32.000000 cysecuretools-4.1.0/cysecuretools/execute/silicon_data_reader/
--rw-r--r--   0 ihos       (501) staff       (20)      228 2022-09-16 09:05:01.000000 cysecuretools-4.1.0/cysecuretools/execute/silicon_data_reader/__init__.py
--rw-r--r--   0 ihos       (501) staff       (20)     3893 2022-09-16 09:05:01.000000 cysecuretools-4.1.0/cysecuretools/execute/silicon_data_reader/silicon_data_reader_mxs40sv2.py
--rw-r--r--   0 ihos       (501) staff       (20)     2856 2022-09-16 09:05:01.000000 cysecuretools-4.1.0/cysecuretools/execute/silicon_data_reader/silicon_data_reader_mxs40v1.py
--rw-r--r--   0 ihos       (501) staff       (20)    19361 2022-09-16 09:06:31.000000 cysecuretools-4.1.0/cysecuretools/execute/sys_call.py
-drwxr-xr-x   0 ihos       (501) staff       (20)        0 2022-09-16 09:50:32.000000 cysecuretools-4.1.0/cysecuretools/execute/version_provider/
--rw-r--r--   0 ihos       (501) staff       (20)        0 2022-09-16 09:05:01.000000 cysecuretools-4.1.0/cysecuretools/execute/version_provider/__init__.py
--rw-r--r--   0 ihos       (501) staff       (20)     5948 2022-09-16 09:05:01.000000 cysecuretools-4.1.0/cysecuretools/execute/version_provider/version_provider_mxs40sv2.py
--rw-r--r--   0 ihos       (501) staff       (20)     6518 2022-09-16 09:05:01.000000 cysecuretools-4.1.0/cysecuretools/execute/version_provider/version_provider_mxs40v1.py
-drwxr-xr-x   0 ihos       (501) staff       (20)        0 2022-09-16 09:50:32.000000 cysecuretools-4.1.0/cysecuretools/execute/voltage_tool/
--rw-r--r--   0 ihos       (501) staff       (20)        0 2022-09-16 09:05:01.000000 cysecuretools-4.1.0/cysecuretools/execute/voltage_tool/__init__.py
--rw-r--r--   0 ihos       (501) staff       (20)     3139 2022-09-16 09:05:01.000000 cysecuretools-4.1.0/cysecuretools/execute/voltage_tool/lvd_voltage_picker.py
--rw-r--r--   0 ihos       (501) staff       (20)     1251 2022-09-16 09:05:01.000000 cysecuretools-4.1.0/cysecuretools/execute/voltage_tool/voltage_tool_mxs40v1.py
--rw-r--r--   0 ihos       (501) staff       (20)    38840 2022-09-16 09:06:31.000000 cysecuretools-4.1.0/cysecuretools/main.py
--rw-r--r--   0 ihos       (501) staff       (20)      718 2022-09-16 09:05:01.000000 cysecuretools-4.1.0/cysecuretools/pkg_globals.py
--rw-r--r--   0 ihos       (501) staff       (20)       79 2022-09-16 09:05:01.000000 cysecuretools-4.1.0/cysecuretools/settings.json
-drwxr-xr-x   0 ihos       (501) staff       (20)        0 2022-09-16 09:50:32.000000 cysecuretools-4.1.0/cysecuretools/targets/
--rw-r--r--   0 ihos       (501) staff       (20)     5178 2022-09-16 09:05:01.000000 cysecuretools-4.1.0/cysecuretools/targets/__init__.py
-drwxr-xr-x   0 ihos       (501) staff       (20)        0 2022-09-16 09:50:32.000000 cysecuretools-4.1.0/cysecuretools/targets/common/
--rw-r--r--   0 ihos       (501) staff       (20)        0 2022-09-16 09:05:01.000000 cysecuretools-4.1.0/cysecuretools/targets/common/__init__.py
-drwxr-xr-x   0 ihos       (501) staff       (20)        0 2022-09-16 09:50:32.000000 cysecuretools-4.1.0/cysecuretools/targets/common/mxs40sv2/
--rw-r--r--   0 ihos       (501) staff       (20)      160 2022-09-16 09:05:01.000000 cysecuretools-4.1.0/cysecuretools/targets/common/mxs40sv2/__init__.py
--rw-r--r--   0 ihos       (501) staff       (20)     1336 2022-09-16 09:05:01.000000 cysecuretools-4.1.0/cysecuretools/targets/common/mxs40sv2/asset.py
--rw-r--r--   0 ihos       (501) staff       (20)     1376 2022-09-16 09:05:01.000000 cysecuretools-4.1.0/cysecuretools/targets/common/mxs40sv2/asset_builder.py
--rw-r--r--   0 ihos       (501) staff       (20)     3073 2022-09-16 09:05:01.000000 cysecuretools-4.1.0/cysecuretools/targets/common/mxs40sv2/asset_enums.py
-drwxr-xr-x   0 ihos       (501) staff       (20)        0 2022-09-16 09:50:32.000000 cysecuretools-4.1.0/cysecuretools/targets/common/mxs40sv2/dependencies_validator/
--rw-r--r--   0 ihos       (501) staff       (20)     1165 2022-09-16 09:05:01.000000 cysecuretools-4.1.0/cysecuretools/targets/common/mxs40sv2/dependencies_validator/__init__.py
--rw-r--r--   0 ihos       (501) staff       (20)     1964 2022-09-16 09:05:01.000000 cysecuretools-4.1.0/cysecuretools/targets/common/mxs40sv2/dependencies_validator/access_restrictions_validator.py
--rw-r--r--   0 ihos       (501) staff       (20)     1304 2022-09-16 09:05:01.000000 cysecuretools-4.1.0/cysecuretools/targets/common/mxs40sv2/dependencies_validator/encryption_key_validator.py
--rw-r--r--   0 ihos       (501) staff       (20)     1919 2022-09-16 09:05:01.000000 cysecuretools-4.1.0/cysecuretools/targets/common/mxs40sv2/dependencies_validator/hci_mode_validator.py
--rw-r--r--   0 ihos       (501) staff       (20)     1508 2022-09-16 09:05:01.000000 cysecuretools-4.1.0/cysecuretools/targets/common/mxs40sv2/dependencies_validator/pre_build_keys_exist_validator.py
--rw-r--r--   0 ihos       (501) staff       (20)     1198 2022-09-16 09:05:01.000000 cysecuretools-4.1.0/cysecuretools/targets/common/mxs40sv2/dependencies_validator/revoke_oem_encryption_validator.py
--rw-r--r--   0 ihos       (501) staff       (20)     1151 2022-09-16 09:05:01.000000 cysecuretools-4.1.0/cysecuretools/targets/common/mxs40sv2/enums.py
--rw-r--r--   0 ihos       (501) staff       (20)     3537 2022-09-16 09:05:01.000000 cysecuretools-4.1.0/cysecuretools/targets/common/mxs40sv2/flow_parser.py
-drwxr-xr-x   0 ihos       (501) staff       (20)        0 2022-09-16 09:50:32.000000 cysecuretools-4.1.0/cysecuretools/targets/common/mxs40sv2/json/
--rw-r--r--   0 ihos       (501) staff       (20)    24916 2022-09-16 09:05:01.000000 cysecuretools-4.1.0/cysecuretools/targets/common/mxs40sv2/json/cyw20829_no_secure.json_schema
--rw-r--r--   0 ihos       (501) staff       (20)     2049 2022-09-16 09:05:01.000000 cysecuretools-4.1.0/cysecuretools/targets/common/mxs40sv2/json/cyw20829_reprovisioning_no_secure.json_schema
--rw-r--r--   0 ihos       (501) staff       (20)     6799 2022-09-16 09:05:01.000000 cysecuretools-4.1.0/cysecuretools/targets/common/mxs40sv2/json/cyw20829_reprovisioning_secure.json_schema
--rw-r--r--   0 ihos       (501) staff       (20)    25395 2022-09-16 09:05:01.000000 cysecuretools-4.1.0/cysecuretools/targets/common/mxs40sv2/json/cyw20829_secure.json_schema
--rw-r--r--   0 ihos       (501) staff       (20)    12298 2022-09-16 09:05:01.000000 cysecuretools-4.1.0/cysecuretools/targets/common/mxs40sv2/policy_parser.py
--rw-r--r--   0 ihos       (501) staff       (20)     4085 2022-09-16 09:05:01.000000 cysecuretools-4.1.0/cysecuretools/targets/common/mxs40sv2/policy_validator.py
-drwxr-xr-x   0 ihos       (501) staff       (20)        0 2022-09-16 09:50:32.000000 cysecuretools-4.1.0/cysecuretools/targets/common/p64/
--rw-r--r--   0 ihos       (501) staff       (20)        0 2022-09-16 09:05:01.000000 cysecuretools-4.1.0/cysecuretools/targets/common/p64/__init__.py
--rw-r--r--   0 ihos       (501) staff       (20)      839 2022-09-16 09:05:01.000000 cysecuretools-4.1.0/cysecuretools/targets/common/p64/enums.py
-drwxr-xr-x   0 ihos       (501) staff       (20)        0 2022-09-16 09:50:32.000000 cysecuretools-4.1.0/cysecuretools/targets/common/p64/json/
--rw-r--r--   0 ihos       (501) staff       (20)     4452 2022-09-16 09:05:01.000000 cysecuretools-4.1.0/cysecuretools/targets/common/p64/json/policy_template.json
--rw-r--r--   0 ihos       (501) staff       (20)    15796 2022-09-16 09:05:01.000000 cysecuretools-4.1.0/cysecuretools/targets/common/p64/json/schema.json_schema
--rw-r--r--   0 ihos       (501) staff       (20)     5756 2022-09-16 09:05:01.000000 cysecuretools-4.1.0/cysecuretools/targets/common/p64/policy_filter.py
--rw-r--r--   0 ihos       (501) staff       (20)    15561 2022-09-16 09:05:01.000000 cysecuretools-4.1.0/cysecuretools/targets/common/p64/policy_parser.py
--rw-r--r--   0 ihos       (501) staff       (20)    46232 2022-09-16 09:06:31.000000 cysecuretools-4.1.0/cysecuretools/targets/common/p64/policy_validator.py
-drwxr-xr-x   0 ihos       (501) staff       (20)        0 2022-09-16 09:50:32.000000 cysecuretools-4.1.0/cysecuretools/targets/common/p64/prebuilt/
--rw-r--r--   0 ihos       (501) staff       (20)      511 2022-09-16 09:05:01.000000 cysecuretools-4.1.0/cysecuretools/targets/common/p64/prebuilt/hsm_state.json
--rw-r--r--   0 ihos       (501) staff       (20)      511 2022-09-16 09:05:01.000000 cysecuretools-4.1.0/cysecuretools/targets/common/p64/prebuilt/oem_state.json
--rw-r--r--   0 ihos       (501) staff       (20)     1381 2022-09-16 09:05:01.000000 cysecuretools-4.1.0/cysecuretools/targets/common/p64/silicon_data_parser.py
-drwxr-xr-x   0 ihos       (501) staff       (20)        0 2022-09-16 09:50:32.000000 cysecuretools-4.1.0/cysecuretools/targets/common/prebuilt/
--rw-r--r--   0 ihos       (501) staff       (20)      173 2022-09-16 09:05:01.000000 cysecuretools-4.1.0/cysecuretools/targets/common/prebuilt/bootloader_pub_key.json
-drwxr-xr-x   0 ihos       (501) staff       (20)        0 2022-09-16 09:50:32.000000 cysecuretools-4.1.0/cysecuretools/targets/cyb06xx5/
--rw-r--r--   0 ihos       (501) staff       (20)       75 2022-09-16 09:05:01.000000 cysecuretools-4.1.0/cysecuretools/targets/cyb06xx5/__init__.py
-drwxr-xr-x   0 ihos       (501) staff       (20)        0 2022-09-16 09:50:32.000000 cysecuretools-4.1.0/cysecuretools/targets/cyb06xx5/keys/
--rw-r--r--   0 ihos       (501) staff       (20)      191 2022-09-16 09:06:31.000000 cysecuretools-4.1.0/cysecuretools/targets/cyb06xx5/keys/cy_pub_key.json
-drwxr-xr-x   0 ihos       (501) staff       (20)        0 2022-09-16 09:50:32.000000 cysecuretools-4.1.0/cysecuretools/targets/cyb06xx5/maps/
--rw-r--r--   0 ihos       (501) staff       (20)        0 2022-09-16 09:05:01.000000 cysecuretools-4.1.0/cysecuretools/targets/cyb06xx5/maps/__init__.py
--rw-r--r--   0 ihos       (501) staff       (20)     1402 2022-09-16 09:05:01.000000 cysecuretools-4.1.0/cysecuretools/targets/cyb06xx5/maps/memory_map.py
--rw-r--r--   0 ihos       (501) staff       (20)     2401 2022-09-16 09:05:01.000000 cysecuretools-4.1.0/cysecuretools/targets/cyb06xx5/maps/register_map.py
-drwxr-xr-x   0 ihos       (501) staff       (20)        0 2022-09-16 09:50:32.000000 cysecuretools-4.1.0/cysecuretools/targets/cyb06xx5/packets/
--rw-r--r--   0 ihos       (501) staff       (20)      371 2022-09-16 09:05:01.000000 cysecuretools-4.1.0/cysecuretools/targets/cyb06xx5/packets/control_dap_cert.json
--rw-r--r--   0 ihos       (501) staff       (20)     1051 2022-09-16 09:05:01.000000 cysecuretools-4.1.0/cysecuretools/targets/cyb06xx5/packets/cy_auth_512k_b0_sample.jwt
--rw-r--r--   0 ihos       (501) staff       (20)      151 2022-09-16 09:05:01.000000 cysecuretools-4.1.0/cysecuretools/targets/cyb06xx5/packets/ec_key_tmpl.json
--rw-r--r--   0 ihos       (501) staff       (20)     4490 2022-09-16 09:05:01.000000 cysecuretools-4.1.0/cysecuretools/targets/cyb06xx5/packets/entrance_exam.jwt
-drwxr-xr-x   0 ihos       (501) staff       (20)        0 2022-09-16 09:50:32.000000 cysecuretools-4.1.0/cysecuretools/targets/cyb06xx5/policy/
--rw-r--r--   0 ihos       (501) staff       (20)     5312 2022-09-16 09:05:01.000000 cysecuretools-4.1.0/cysecuretools/targets/cyb06xx5/policy/policy_multi_CM0_CM4.json
--rw-r--r--   0 ihos       (501) staff       (20)     5314 2022-09-16 09:05:01.000000 cysecuretools-4.1.0/cysecuretools/targets/cyb06xx5/policy/policy_multi_CM0_CM4_smif.json
--rw-r--r--   0 ihos       (501) staff       (20)     4927 2022-09-16 09:05:01.000000 cysecuretools-4.1.0/cysecuretools/targets/cyb06xx5/policy/policy_single_CM0_CM4.json
--rw-r--r--   0 ihos       (501) staff       (20)     4927 2022-09-16 09:05:01.000000 cysecuretools-4.1.0/cysecuretools/targets/cyb06xx5/policy/policy_single_CM0_CM4_smif.json
-drwxr-xr-x   0 ihos       (501) staff       (20)        0 2022-09-16 09:50:32.000000 cysecuretools-4.1.0/cysecuretools/targets/cyb06xx5/prebuilt/
-drwxr-xr-x   0 ihos       (501) staff       (20)        0 2022-09-16 09:50:32.000000 cysecuretools-4.1.0/cysecuretools/targets/cyb06xx5/prebuilt/CyBootloader_Release/
--rw-r--r--   0 ihos       (501) staff       (20)   134553 2022-09-16 09:05:01.000000 cysecuretools-4.1.0/cysecuretools/targets/cyb06xx5/prebuilt/CyBootloader_Release/CypressBootloader_CM0p.hex
--rw-r--r--   0 ihos       (501) staff       (20)      536 2022-09-16 09:05:01.000000 cysecuretools-4.1.0/cysecuretools/targets/cyb06xx5/prebuilt/CyBootloader_Release/CypressBootloader_CM0p.jwt
-drwxr-xr-x   0 ihos       (501) staff       (20)        0 2022-09-16 09:50:32.000000 cysecuretools-4.1.0/cysecuretools/targets/cyb06xx5/prebuilt/CyBootloader_WithLogs/
--rw-r--r--   0 ihos       (501) staff       (20)   148119 2022-09-16 09:05:01.000000 cysecuretools-4.1.0/cysecuretools/targets/cyb06xx5/prebuilt/CyBootloader_WithLogs/CypressBootloader_CM0p.hex
--rw-r--r--   0 ihos       (501) staff       (20)      540 2022-09-16 09:05:01.000000 cysecuretools-4.1.0/cysecuretools/targets/cyb06xx5/prebuilt/CyBootloader_WithLogs/CypressBootloader_CM0p.jwt
--rw-r--r--   0 ihos       (501) staff       (20)     4372 2022-09-16 09:06:31.000000 cysecuretools-4.1.0/cysecuretools/targets/cyb06xx5/target_builder.py
-drwxr-xr-x   0 ihos       (501) staff       (20)        0 2022-09-16 09:50:32.000000 cysecuretools-4.1.0/cysecuretools/targets/cyb06xx7/
--rw-r--r--   0 ihos       (501) staff       (20)        0 2022-09-16 09:05:01.000000 cysecuretools-4.1.0/cysecuretools/targets/cyb06xx7/__init__.py
-drwxr-xr-x   0 ihos       (501) staff       (20)        0 2022-09-16 09:50:32.000000 cysecuretools-4.1.0/cysecuretools/targets/cyb06xx7/keys/
--rw-r--r--   0 ihos       (501) staff       (20)      191 2022-09-16 09:06:31.000000 cysecuretools-4.1.0/cysecuretools/targets/cyb06xx7/keys/cy_pub_key.json
-drwxr-xr-x   0 ihos       (501) staff       (20)        0 2022-09-16 09:50:32.000000 cysecuretools-4.1.0/cysecuretools/targets/cyb06xx7/maps/
--rw-r--r--   0 ihos       (501) staff       (20)        0 2022-09-16 09:05:01.000000 cysecuretools-4.1.0/cysecuretools/targets/cyb06xx7/maps/__init__.py
--rw-r--r--   0 ihos       (501) staff       (20)     1711 2022-09-16 09:05:01.000000 cysecuretools-4.1.0/cysecuretools/targets/cyb06xx7/maps/memory_map.py
--rw-r--r--   0 ihos       (501) staff       (20)     2401 2022-09-16 09:05:01.000000 cysecuretools-4.1.0/cysecuretools/targets/cyb06xx7/maps/register_map.py
-drwxr-xr-x   0 ihos       (501) staff       (20)        0 2022-09-16 09:50:32.000000 cysecuretools-4.1.0/cysecuretools/targets/cyb06xx7/packets/
--rw-r--r--   0 ihos       (501) staff       (20)      371 2022-09-16 09:05:01.000000 cysecuretools-4.1.0/cysecuretools/targets/cyb06xx7/packets/control_dap_cert.json
--rw-r--r--   0 ihos       (501) staff       (20)     1031 2022-09-16 09:05:01.000000 cysecuretools-4.1.0/cysecuretools/targets/cyb06xx7/packets/cy_auth_1m_b0_sample.jwt
--rw-r--r--   0 ihos       (501) staff       (20)      151 2022-09-16 09:05:01.000000 cysecuretools-4.1.0/cysecuretools/targets/cyb06xx7/packets/ec_key_tmpl.json
--rw-r--r--   0 ihos       (501) staff       (20)     4490 2022-09-16 09:05:01.000000 cysecuretools-4.1.0/cysecuretools/targets/cyb06xx7/packets/entrance_exam.jwt
-drwxr-xr-x   0 ihos       (501) staff       (20)        0 2022-09-16 09:50:32.000000 cysecuretools-4.1.0/cysecuretools/targets/cyb06xx7/policy/
--rw-r--r--   0 ihos       (501) staff       (20)     5095 2022-09-16 09:05:01.000000 cysecuretools-4.1.0/cysecuretools/targets/cyb06xx7/policy/policy_multi_CM0_CM4.json
--rw-r--r--   0 ihos       (501) staff       (20)     5095 2022-09-16 09:05:01.000000 cysecuretools-4.1.0/cysecuretools/targets/cyb06xx7/policy/policy_multi_CM0_CM4_smif.json
--rw-r--r--   0 ihos       (501) staff       (20)     5740 2022-09-16 09:05:01.000000 cysecuretools-4.1.0/cysecuretools/targets/cyb06xx7/policy/policy_multi_CM0_CM4_smif_swap.json
--rw-r--r--   0 ihos       (501) staff       (20)     5739 2022-09-16 09:05:01.000000 cysecuretools-4.1.0/cysecuretools/targets/cyb06xx7/policy/policy_multi_CM0_CM4_swap.json
--rw-r--r--   0 ihos       (501) staff       (20)     4883 2022-09-16 09:05:01.000000 cysecuretools-4.1.0/cysecuretools/targets/cyb06xx7/policy/policy_single_CM0_CM4.json
--rw-r--r--   0 ihos       (501) staff       (20)     4883 2022-09-16 09:05:01.000000 cysecuretools-4.1.0/cysecuretools/targets/cyb06xx7/policy/policy_single_CM0_CM4_smif.json
--rw-r--r--   0 ihos       (501) staff       (20)     5531 2022-09-16 09:05:01.000000 cysecuretools-4.1.0/cysecuretools/targets/cyb06xx7/policy/policy_single_CM0_CM4_smif_swap.json
--rw-r--r--   0 ihos       (501) staff       (20)     5529 2022-09-16 09:05:01.000000 cysecuretools-4.1.0/cysecuretools/targets/cyb06xx7/policy/policy_single_CM0_CM4_swap.json
-drwxr-xr-x   0 ihos       (501) staff       (20)        0 2022-09-16 09:50:32.000000 cysecuretools-4.1.0/cysecuretools/targets/cyb06xx7/prebuilt/
-drwxr-xr-x   0 ihos       (501) staff       (20)        0 2022-09-16 09:50:32.000000 cysecuretools-4.1.0/cysecuretools/targets/cyb06xx7/prebuilt/CyBootloader_Release/
--rw-r--r--   0 ihos       (501) staff       (20)   138714 2022-09-16 09:05:01.000000 cysecuretools-4.1.0/cysecuretools/targets/cyb06xx7/prebuilt/CyBootloader_Release/CypressBootloader_CM0p.hex
--rw-r--r--   0 ihos       (501) staff       (20)      543 2022-09-16 09:05:01.000000 cysecuretools-4.1.0/cysecuretools/targets/cyb06xx7/prebuilt/CyBootloader_Release/CypressBootloader_CM0p.jwt
-drwxr-xr-x   0 ihos       (501) staff       (20)        0 2022-09-16 09:50:32.000000 cysecuretools-4.1.0/cysecuretools/targets/cyb06xx7/prebuilt/CyBootloader_WithLogs/
--rw-r--r--   0 ihos       (501) staff       (20)   150520 2022-09-16 09:05:01.000000 cysecuretools-4.1.0/cysecuretools/targets/cyb06xx7/prebuilt/CyBootloader_WithLogs/CypressBootloader_CM0p.hex
--rw-r--r--   0 ihos       (501) staff       (20)      542 2022-09-16 09:05:01.000000 cysecuretools-4.1.0/cysecuretools/targets/cyb06xx7/prebuilt/CyBootloader_WithLogs/CypressBootloader_CM0p.jwt
--rw-r--r--   0 ihos       (501) staff       (20)     4373 2022-09-16 09:06:31.000000 cysecuretools-4.1.0/cysecuretools/targets/cyb06xx7/target_builder.py
-drwxr-xr-x   0 ihos       (501) staff       (20)        0 2022-09-16 09:50:32.000000 cysecuretools-4.1.0/cysecuretools/targets/cyb06xxa/
--rw-r--r--   0 ihos       (501) staff       (20)       75 2022-09-16 09:05:01.000000 cysecuretools-4.1.0/cysecuretools/targets/cyb06xxa/__init__.py
-drwxr-xr-x   0 ihos       (501) staff       (20)        0 2022-09-16 09:50:32.000000 cysecuretools-4.1.0/cysecuretools/targets/cyb06xxa/keys/
--rw-r--r--   0 ihos       (501) staff       (20)      191 2022-09-16 09:06:31.000000 cysecuretools-4.1.0/cysecuretools/targets/cyb06xxa/keys/cy_pub_key.json
-drwxr-xr-x   0 ihos       (501) staff       (20)        0 2022-09-16 09:50:32.000000 cysecuretools-4.1.0/cysecuretools/targets/cyb06xxa/maps/
--rw-r--r--   0 ihos       (501) staff       (20)        0 2022-09-16 09:05:01.000000 cysecuretools-4.1.0/cysecuretools/targets/cyb06xxa/maps/__init__.py
--rw-r--r--   0 ihos       (501) staff       (20)     1402 2022-09-16 09:05:01.000000 cysecuretools-4.1.0/cysecuretools/targets/cyb06xxa/maps/memory_map.py
--rw-r--r--   0 ihos       (501) staff       (20)     2402 2022-09-16 09:05:01.000000 cysecuretools-4.1.0/cysecuretools/targets/cyb06xxa/maps/register_map.py
-drwxr-xr-x   0 ihos       (501) staff       (20)        0 2022-09-16 09:50:32.000000 cysecuretools-4.1.0/cysecuretools/targets/cyb06xxa/packets/
--rw-r--r--   0 ihos       (501) staff       (20)      371 2022-09-16 09:05:01.000000 cysecuretools-4.1.0/cysecuretools/targets/cyb06xxa/packets/control_dap_cert.json
--rw-r--r--   0 ihos       (501) staff       (20)     1051 2022-09-16 09:05:01.000000 cysecuretools-4.1.0/cysecuretools/targets/cyb06xxa/packets/cy_auth_2m_b0_sample.jwt
--rw-r--r--   0 ihos       (501) staff       (20)      151 2022-09-16 09:05:01.000000 cysecuretools-4.1.0/cysecuretools/targets/cyb06xxa/packets/ec_key_tmpl.json
--rw-r--r--   0 ihos       (501) staff       (20)     4490 2022-09-16 09:05:01.000000 cysecuretools-4.1.0/cysecuretools/targets/cyb06xxa/packets/entrance_exam.jwt
-drwxr-xr-x   0 ihos       (501) staff       (20)        0 2022-09-16 09:50:32.000000 cysecuretools-4.1.0/cysecuretools/targets/cyb06xxa/policy/
--rw-r--r--   0 ihos       (501) staff       (20)     6068 2022-09-16 09:06:31.000000 cysecuretools-4.1.0/cysecuretools/targets/cyb06xxa/policy/policy_multi_CM0_CM4_smif_swap.json
--rw-r--r--   0 ihos       (501) staff       (20)     5784 2022-09-16 09:06:31.000000 cysecuretools-4.1.0/cysecuretools/targets/cyb06xxa/policy/policy_multi_CM0_CM4_swap.json
--rw-r--r--   0 ihos       (501) staff       (20)     5621 2022-09-16 09:06:31.000000 cysecuretools-4.1.0/cysecuretools/targets/cyb06xxa/policy/policy_single_CM0_CM4_smif_swap.json
--rw-r--r--   0 ihos       (501) staff       (20)     5573 2022-09-16 09:06:31.000000 cysecuretools-4.1.0/cysecuretools/targets/cyb06xxa/policy/policy_single_CM0_CM4_swap.json
-drwxr-xr-x   0 ihos       (501) staff       (20)        0 2022-09-16 09:50:32.000000 cysecuretools-4.1.0/cysecuretools/targets/cyb06xxa/prebuilt/
-drwxr-xr-x   0 ihos       (501) staff       (20)        0 2022-09-16 09:50:32.000000 cysecuretools-4.1.0/cysecuretools/targets/cyb06xxa/prebuilt/CyBootloader_Release_swap/
--rw-r--r--   0 ihos       (501) staff       (20)   138738 2022-09-16 09:06:31.000000 cysecuretools-4.1.0/cysecuretools/targets/cyb06xxa/prebuilt/CyBootloader_Release_swap/CypressBootloader_CM0p.hex
--rw-r--r--   0 ihos       (501) staff       (20)      592 2022-09-16 09:06:31.000000 cysecuretools-4.1.0/cysecuretools/targets/cyb06xxa/prebuilt/CyBootloader_Release_swap/CypressBootloader_CM0p.jwt
-drwxr-xr-x   0 ihos       (501) staff       (20)        0 2022-09-16 09:50:32.000000 cysecuretools-4.1.0/cysecuretools/targets/cyb06xxa/prebuilt/CyBootloader_WithLogs_swap/
--rw-r--r--   0 ihos       (501) staff       (20)   155454 2022-09-16 09:06:31.000000 cysecuretools-4.1.0/cysecuretools/targets/cyb06xxa/prebuilt/CyBootloader_WithLogs_swap/CypressBootloader_CM0p.hex
--rw-r--r--   0 ihos       (501) staff       (20)      588 2022-09-16 09:06:31.000000 cysecuretools-4.1.0/cysecuretools/targets/cyb06xxa/prebuilt/CyBootloader_WithLogs_swap/CypressBootloader_CM0p.jwt
--rw-r--r--   0 ihos       (501) staff       (20)     4376 2022-09-16 09:06:31.000000 cysecuretools-4.1.0/cysecuretools/targets/cyb06xxa/target_builder.py
-drwxr-xr-x   0 ihos       (501) staff       (20)        0 2022-09-16 09:50:32.000000 cysecuretools-4.1.0/cysecuretools/targets/cys06xxa/
--rw-r--r--   0 ihos       (501) staff       (20)       75 2022-09-16 09:05:01.000000 cysecuretools-4.1.0/cysecuretools/targets/cys06xxa/__init__.py
-drwxr-xr-x   0 ihos       (501) staff       (20)        0 2022-09-16 09:50:32.000000 cysecuretools-4.1.0/cysecuretools/targets/cys06xxa/keys/
--rw-r--r--   0 ihos       (501) staff       (20)      191 2022-09-16 09:06:31.000000 cysecuretools-4.1.0/cysecuretools/targets/cys06xxa/keys/cy_pub_key.json
-drwxr-xr-x   0 ihos       (501) staff       (20)        0 2022-09-16 09:50:32.000000 cysecuretools-4.1.0/cysecuretools/targets/cys06xxa/packets/
--rw-r--r--   0 ihos       (501) staff       (20)      371 2022-09-16 09:05:01.000000 cysecuretools-4.1.0/cysecuretools/targets/cys06xxa/packets/control_dap_cert.json
--rw-r--r--   0 ihos       (501) staff       (20)     1031 2022-09-16 09:05:01.000000 cysecuretools-4.1.0/cysecuretools/targets/cys06xxa/packets/cy_auth_2m_s0_sample.jwt
--rw-r--r--   0 ihos       (501) staff       (20)      151 2022-09-16 09:05:01.000000 cysecuretools-4.1.0/cysecuretools/targets/cys06xxa/packets/ec_key_tmpl.json
--rw-r--r--   0 ihos       (501) staff       (20)     4490 2022-09-16 09:05:01.000000 cysecuretools-4.1.0/cysecuretools/targets/cys06xxa/packets/entrance_exam.jwt
-drwxr-xr-x   0 ihos       (501) staff       (20)        0 2022-09-16 09:50:32.000000 cysecuretools-4.1.0/cysecuretools/targets/cys06xxa/policy/
--rw-r--r--   0 ihos       (501) staff       (20)     6068 2022-09-16 09:06:31.000000 cysecuretools-4.1.0/cysecuretools/targets/cys06xxa/policy/policy_multi_CM0_CM4_smif_swap.json
--rw-r--r--   0 ihos       (501) staff       (20)     5784 2022-09-16 09:06:31.000000 cysecuretools-4.1.0/cysecuretools/targets/cys06xxa/policy/policy_multi_CM0_CM4_swap.json
--rw-r--r--   0 ihos       (501) staff       (20)     5621 2022-09-16 09:06:31.000000 cysecuretools-4.1.0/cysecuretools/targets/cys06xxa/policy/policy_single_CM0_CM4_smif_swap.json
--rw-r--r--   0 ihos       (501) staff       (20)     5573 2022-09-16 09:06:31.000000 cysecuretools-4.1.0/cysecuretools/targets/cys06xxa/policy/policy_single_CM0_CM4_swap.json
-drwxr-xr-x   0 ihos       (501) staff       (20)        0 2022-09-16 09:50:32.000000 cysecuretools-4.1.0/cysecuretools/targets/cys06xxa/prebuilt/
-drwxr-xr-x   0 ihos       (501) staff       (20)        0 2022-09-16 09:50:32.000000 cysecuretools-4.1.0/cysecuretools/targets/cys06xxa/prebuilt/CyBootloader_Release_swap/
--rw-r--r--   0 ihos       (501) staff       (20)   138738 2022-09-16 09:06:31.000000 cysecuretools-4.1.0/cysecuretools/targets/cys06xxa/prebuilt/CyBootloader_Release_swap/CypressBootloader_CM0p.hex
--rw-r--r--   0 ihos       (501) staff       (20)      592 2022-09-16 09:06:31.000000 cysecuretools-4.1.0/cysecuretools/targets/cys06xxa/prebuilt/CyBootloader_Release_swap/CypressBootloader_CM0p.jwt
-drwxr-xr-x   0 ihos       (501) staff       (20)        0 2022-09-16 09:50:32.000000 cysecuretools-4.1.0/cysecuretools/targets/cys06xxa/prebuilt/CyBootloader_WithLogs_swap/
--rw-r--r--   0 ihos       (501) staff       (20)   155454 2022-09-16 09:06:31.000000 cysecuretools-4.1.0/cysecuretools/targets/cys06xxa/prebuilt/CyBootloader_WithLogs_swap/CypressBootloader_CM0p.hex
--rw-r--r--   0 ihos       (501) staff       (20)      588 2022-09-16 09:06:31.000000 cysecuretools-4.1.0/cysecuretools/targets/cys06xxa/prebuilt/CyBootloader_WithLogs_swap/CypressBootloader_CM0p.jwt
--rw-r--r--   0 ihos       (501) staff       (20)     4376 2022-09-16 09:06:31.000000 cysecuretools-4.1.0/cysecuretools/targets/cys06xxa/target_builder.py
-drwxr-xr-x   0 ihos       (501) staff       (20)        0 2022-09-16 09:50:32.000000 cysecuretools-4.1.0/cysecuretools/targets/cyw20829/
--rw-r--r--   0 ihos       (501) staff       (20)       74 2022-09-16 09:05:01.000000 cysecuretools-4.1.0/cysecuretools/targets/cyw20829/__init__.py
-drwxr-xr-x   0 ihos       (501) staff       (20)        0 2022-09-16 09:50:32.000000 cysecuretools-4.1.0/cysecuretools/targets/cyw20829/flows/
--rw-r--r--   0 ihos       (501) staff       (20)        0 2022-09-16 09:05:01.000000 cysecuretools-4.1.0/cysecuretools/targets/cyw20829/flows/__init__.py
--rw-r--r--   0 ihos       (501) staff       (20)     8218 2022-09-16 09:05:01.000000 cysecuretools-4.1.0/cysecuretools/targets/cyw20829/flows/asset_map.py
--rw-r--r--   0 ihos       (501) staff       (20)     1020 2022-09-16 09:05:01.000000 cysecuretools-4.1.0/cysecuretools/targets/cyw20829/flows/load_app_data.py
--rw-r--r--   0 ihos       (501) staff       (20)      179 2022-09-16 09:05:01.000000 cysecuretools-4.1.0/cysecuretools/targets/cyw20829/flows/oem_assets.json
--rw-r--r--   0 ihos       (501) staff       (20)      858 2022-09-16 09:05:01.000000 cysecuretools-4.1.0/cysecuretools/targets/cyw20829/flows/prov_flows.json
--rw-r--r--   0 ihos       (501) staff       (20)       94 2022-09-16 09:05:01.000000 cysecuretools-4.1.0/cysecuretools/targets/cyw20829/flows/reprovisioning_assets.json
--rw-r--r--   0 ihos       (501) staff       (20)     9210 2022-09-16 09:05:01.000000 cysecuretools-4.1.0/cysecuretools/targets/cyw20829/flows/reverse_asset_map.py
-drwxr-xr-x   0 ihos       (501) staff       (20)        0 2022-09-16 09:50:32.000000 cysecuretools-4.1.0/cysecuretools/targets/cyw20829/keys/
--rw-r--r--   0 ihos       (501) staff       (20)      460 2022-09-16 09:05:01.000000 cysecuretools-4.1.0/cysecuretools/targets/cyw20829/keys/pub_hci_0.pem
--rw-r--r--   0 ihos       (501) staff       (20)      460 2022-09-16 09:05:01.000000 cysecuretools-4.1.0/cysecuretools/targets/cyw20829/keys/pub_hci_1.pem
-drwxr-xr-x   0 ihos       (501) staff       (20)        0 2022-09-16 09:50:32.000000 cysecuretools-4.1.0/cysecuretools/targets/cyw20829/maps/
--rw-r--r--   0 ihos       (501) staff       (20)        0 2022-09-16 09:05:01.000000 cysecuretools-4.1.0/cysecuretools/targets/cyw20829/maps/__init__.py
--rw-r--r--   0 ihos       (501) staff       (20)     1052 2022-09-16 09:05:01.000000 cysecuretools-4.1.0/cysecuretools/targets/cyw20829/maps/memory_map.py
--rw-r--r--   0 ihos       (501) staff       (20)     1715 2022-09-16 09:05:01.000000 cysecuretools-4.1.0/cysecuretools/targets/cyw20829/maps/register_map.py
-drwxr-xr-x   0 ihos       (501) staff       (20)        0 2022-09-16 09:50:32.000000 cysecuretools-4.1.0/cysecuretools/targets/cyw20829/packets/
-drwxr-xr-x   0 ihos       (501) staff       (20)        0 2022-09-16 09:50:32.000000 cysecuretools-4.1.0/cysecuretools/targets/cyw20829/packets/apps/
-drwxr-xr-x   0 ihos       (501) staff       (20)        0 2022-09-16 09:50:32.000000 cysecuretools-4.1.0/cysecuretools/targets/cyw20829/packets/apps/prov_oem/
--rw-r--r--   0 ihos       (501) staff       (20)      235 2022-09-16 09:05:01.000000 cysecuretools-4.1.0/cysecuretools/targets/cyw20829/packets/apps/prov_oem/config.json
--rwxr-xr-x   0 ihos       (501) staff       (20)     7812 2022-09-16 09:05:01.000000 cysecuretools-4.1.0/cysecuretools/targets/cyw20829/packets/apps/prov_oem/cyapp_prov_oem_signed_icv0.bin
--rwxr-xr-x   0 ihos       (501) staff       (20)      375 2022-09-16 09:05:01.000000 cysecuretools-4.1.0/cysecuretools/targets/cyw20829/packets/apps/prov_oem/info.txt
-drwxr-xr-x   0 ihos       (501) staff       (20)        0 2022-09-16 09:50:32.000000 cysecuretools-4.1.0/cysecuretools/targets/cyw20829/packets/apps/reprovisioning/
--rw-r--r--   0 ihos       (501) staff       (20)      241 2022-09-16 09:05:01.000000 cysecuretools-4.1.0/cysecuretools/targets/cyw20829/packets/apps/reprovisioning/config.json
--rwxr-xr-x   0 ihos       (501) staff       (20)    28836 2022-09-16 09:05:01.000000 cysecuretools-4.1.0/cysecuretools/targets/cyw20829/packets/apps/reprovisioning/cyapp_reprovisioning_signed_icv0.bin
--rwxr-xr-x   0 ihos       (501) staff       (20)      264 2022-09-16 09:05:01.000000 cysecuretools-4.1.0/cysecuretools/targets/cyw20829/packets/apps/reprovisioning/info.txt
-drwxr-xr-x   0 ihos       (501) staff       (20)        0 2022-09-16 09:50:32.000000 cysecuretools-4.1.0/cysecuretools/targets/cyw20829/packets/apps/to_rma/
--rw-r--r--   0 ihos       (501) staff       (20)      269 2022-09-16 09:05:01.000000 cysecuretools-4.1.0/cysecuretools/targets/cyw20829/packets/apps/to_rma/config.json
--rwxr-xr-x   0 ihos       (501) staff       (20)    28612 2022-09-16 09:05:01.000000 cysecuretools-4.1.0/cysecuretools/targets/cyw20829/packets/apps/to_rma/cyapp_to_rma_signed_icv0.bin
--rwxr-xr-x   0 ihos       (501) staff       (20)      289 2022-09-16 09:05:01.000000 cysecuretools-4.1.0/cysecuretools/targets/cyw20829/packets/apps/to_rma/info.txt
--rw-r--r--   0 ihos       (501) staff       (20)      624 2022-09-16 09:05:01.000000 cysecuretools-4.1.0/cysecuretools/targets/cyw20829/packets/debug_cert.json
--rw-r--r--   0 ihos       (501) staff       (20)      168 2022-09-16 09:05:01.000000 cysecuretools-4.1.0/cysecuretools/targets/cyw20829/packets/rsa_key_tmpl.json
-drwxr-xr-x   0 ihos       (501) staff       (20)        0 2022-09-16 09:50:32.000000 cysecuretools-4.1.0/cysecuretools/targets/cyw20829/policy/
--rw-r--r--   0 ihos       (501) staff       (20)     6135 2022-09-16 09:05:01.000000 cysecuretools-4.1.0/cysecuretools/targets/cyw20829/policy/policy_hci_secure.json
--rw-r--r--   0 ihos       (501) staff       (20)     6344 2022-09-16 09:05:01.000000 cysecuretools-4.1.0/cysecuretools/targets/cyw20829/policy/policy_no_secure.json
--rw-r--r--   0 ihos       (501) staff       (20)      374 2022-09-16 09:05:01.000000 cysecuretools-4.1.0/cysecuretools/targets/cyw20829/policy/policy_reprovisioning_no_secure.json
--rw-r--r--   0 ihos       (501) staff       (20)     1812 2022-09-16 09:05:01.000000 cysecuretools-4.1.0/cysecuretools/targets/cyw20829/policy/policy_reprovisioning_secure.json
--rw-r--r--   0 ihos       (501) staff       (20)     8281 2022-09-16 09:05:01.000000 cysecuretools-4.1.0/cysecuretools/targets/cyw20829/policy/policy_secure.json
--rw-r--r--   0 ihos       (501) staff       (20)     2841 2022-09-16 09:05:01.000000 cysecuretools-4.1.0/cysecuretools/targets/cyw20829/policy_generator.py
--rw-r--r--   0 ihos       (501) staff       (20)     4293 2022-09-16 09:06:31.000000 cysecuretools-4.1.0/cysecuretools/targets/cyw20829/target_builder.py
--rw-r--r--   0 ihos       (501) staff       (20)      608 2022-09-16 09:06:31.000000 cysecuretools-4.1.0/cysecuretools/version.py
-drwxr-xr-x   0 ihos       (501) staff       (20)        0 2022-09-16 09:50:32.000000 cysecuretools-4.1.0/cysecuretools.egg-info/
--rw-r--r--   0 ihos       (501) staff       (20)     8057 2022-09-16 09:50:32.000000 cysecuretools-4.1.0/cysecuretools.egg-info/PKG-INFO
--rw-r--r--   0 ihos       (501) staff       (20)    15547 2022-09-16 09:50:32.000000 cysecuretools-4.1.0/cysecuretools.egg-info/SOURCES.txt
--rw-r--r--   0 ihos       (501) staff       (20)        1 2022-09-16 09:50:32.000000 cysecuretools-4.1.0/cysecuretools.egg-info/dependency_links.txt
--rw-r--r--   0 ihos       (501) staff       (20)       63 2022-09-16 09:50:32.000000 cysecuretools-4.1.0/cysecuretools.egg-info/entry_points.txt
--rw-r--r--   0 ihos       (501) staff       (20)      170 2022-09-16 09:50:32.000000 cysecuretools-4.1.0/cysecuretools.egg-info/requires.txt
--rw-r--r--   0 ihos       (501) staff       (20)       14 2022-09-16 09:50:32.000000 cysecuretools-4.1.0/cysecuretools.egg-info/top_level.txt
--rw-r--r--   0 ihos       (501) staff       (20)      141 2022-09-16 09:06:31.000000 cysecuretools-4.1.0/pyproject.toml
--rw-r--r--   0 ihos       (501) staff       (20)       38 2022-09-16 09:50:32.000000 cysecuretools-4.1.0/setup.cfg
--rw-r--r--   0 ihos       (501) staff       (20)     2373 2022-09-16 09:05:01.000000 cysecuretools-4.1.0/setup.py
+drwxr-xr-x   0 ihos       (501) staff       (20)        0 2023-05-18 10:54:49.510923 cysecuretools-4.2.0/
+-rw-r--r--   0 ihos       (501) staff       (20)     2674 2023-05-18 10:29:21.000000 cysecuretools-4.2.0/CHANGELOG.md
+-rw-r--r--   0 ihos       (501) staff       (20)      582 2023-05-18 10:29:21.000000 cysecuretools-4.2.0/LICENSE
+-rw-r--r--   0 ihos       (501) staff       (20)      970 2023-05-18 10:29:21.000000 cysecuretools-4.2.0/MANIFEST.in
+-rw-r--r--   0 ihos       (501) staff       (20)    10995 2023-05-18 10:54:49.510355 cysecuretools-4.2.0/PKG-INFO
+-rw-r--r--   0 ihos       (501) staff       (20)     7575 2023-05-18 10:29:21.000000 cysecuretools-4.2.0/README.md
+drwxr-xr-x   0 ihos       (501) staff       (20)        0 2023-05-18 10:54:47.976153 cysecuretools-4.2.0/cysecuretools/
+-rw-r--r--   0 ihos       (501) staff       (20)      631 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/__init__.py
+-rw-r--r--   0 ihos       (501) staff       (20)      714 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/__main__.py
+-rw-r--r--   0 ihos       (501) staff       (20)    11340 2023-05-18 10:29:21.000000 cysecuretools-4.2.0/cysecuretools/cli.py
+-rw-r--r--   0 ihos       (501) staff       (20)     6113 2023-05-18 10:29:21.000000 cysecuretools-4.2.0/cysecuretools/cli_creator.py
+-rw-r--r--   0 ihos       (501) staff       (20)    32939 2023-05-18 10:29:21.000000 cysecuretools-4.2.0/cysecuretools/cli_mxs40sv2.py
+-rw-r--r--   0 ihos       (501) staff       (20)    27673 2023-05-18 10:29:21.000000 cysecuretools-4.2.0/cysecuretools/cli_mxs40v1.py
+drwxr-xr-x   0 ihos       (501) staff       (20)        0 2023-05-18 10:54:48.149679 cysecuretools-4.2.0/cysecuretools/core/
+-rw-r--r--   0 ihos       (501) staff       (20)     1098 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/core/__init__.py
+-rw-r--r--   0 ihos       (501) staff       (20)      784 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/core/bitops.py
+drwxr-xr-x   0 ihos       (501) staff       (20)        0 2023-05-18 10:54:48.157485 cysecuretools-4.2.0/cysecuretools/core/certificates/
+-rw-r--r--   0 ihos       (501) staff       (20)        0 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/core/certificates/__init__.py
+-rw-r--r--   0 ihos       (501) staff       (20)     9951 2023-05-18 10:29:21.000000 cysecuretools-4.2.0/cysecuretools/core/certificates/x509.py
+-rw-r--r--   0 ihos       (501) staff       (20)     5168 2023-05-18 10:29:21.000000 cysecuretools-4.2.0/cysecuretools/core/connect_helper.py
+-rw-r--r--   0 ihos       (501) staff       (20)     2230 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/core/cy_bootloader_map_parser.py
+-rw-r--r--   0 ihos       (501) staff       (20)     1259 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/core/dependecy_validator.py
+-rw-r--r--   0 ihos       (501) staff       (20)     1191 2023-05-18 10:29:21.000000 cysecuretools-4.2.0/cysecuretools/core/deprecated.py
+-rw-r--r--   0 ihos       (501) staff       (20)      945 2023-05-18 10:29:21.000000 cysecuretools-4.2.0/cysecuretools/core/entrance_exam_base.py
+-rw-r--r--   0 ihos       (501) staff       (20)     1450 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/core/enums.py
+-rw-r--r--   0 ihos       (501) staff       (20)      736 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/core/exceptions.py
+-rw-r--r--   0 ihos       (501) staff       (20)     1469 2023-05-18 10:29:21.000000 cysecuretools-4.2.0/cysecuretools/core/json_helper.py
+-rw-r--r--   0 ihos       (501) staff       (20)     1674 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/core/jsonpath.py
+-rw-r--r--   0 ihos       (501) staff       (20)     2144 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/core/key_data.py
+drwxr-xr-x   0 ihos       (501) staff       (20)        0 2023-05-18 10:54:48.176950 cysecuretools-4.2.0/cysecuretools/core/key_handlers/
+-rw-r--r--   0 ihos       (501) staff       (20)       67 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/core/key_handlers/__init__.py
+-rw-r--r--   0 ihos       (501) staff       (20)     2539 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/core/key_handlers/ec_handler.py
+-rw-r--r--   0 ihos       (501) staff       (20)     3889 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/core/key_handlers/rsa_handler.py
+-rw-r--r--   0 ihos       (501) staff       (20)     2280 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/core/key_helper.py
+-rw-r--r--   0 ihos       (501) staff       (20)     2434 2023-05-18 10:29:21.000000 cysecuretools-4.2.0/cysecuretools/core/logging_configurator.py
+-rw-r--r--   0 ihos       (501) staff       (20)     2401 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/core/logging_formatter.py
+-rw-r--r--   0 ihos       (501) staff       (20)      701 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/core/memory_area.py
+-rw-r--r--   0 ihos       (501) staff       (20)     2253 2023-05-18 10:29:21.000000 cysecuretools-4.2.0/cysecuretools/core/memory_map_base.py
+-rw-r--r--   0 ihos       (501) staff       (20)     3161 2023-05-18 10:29:21.000000 cysecuretools-4.2.0/cysecuretools/core/mtb_tools_discovery.py
+-rw-r--r--   0 ihos       (501) staff       (20)     2209 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/core/ocd_settings.py
+-rw-r--r--   0 ihos       (501) staff       (20)      840 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/core/policy_filter_base.py
+-rw-r--r--   0 ihos       (501) staff       (20)      954 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/core/policy_validator_base.py
+-rw-r--r--   0 ihos       (501) staff       (20)      783 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/core/progress_bar.py
+-rw-r--r--   0 ihos       (501) staff       (20)     6765 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/core/project.py
+drwxr-xr-x   0 ihos       (501) staff       (20)        0 2023-05-18 10:54:48.190496 cysecuretools-4.2.0/cysecuretools/core/provisioning_flows/
+-rw-r--r--   0 ihos       (501) staff       (20)      134 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/core/provisioning_flows/__init__.py
+-rw-r--r--   0 ihos       (501) staff       (20)      716 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/core/provisioning_flows/application.py
+-rw-r--r--   0 ihos       (501) staff       (20)      894 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/core/provisioning_flows/flow.py
+-rw-r--r--   0 ihos       (501) staff       (20)     3267 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/core/register_map_base.py
+-rw-r--r--   0 ihos       (501) staff       (20)     1216 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/core/signtool_base.py
+drwxr-xr-x   0 ihos       (501) staff       (20)        0 2023-05-18 10:54:48.216458 cysecuretools-4.2.0/cysecuretools/core/strategy_context/
+-rw-r--r--   0 ihos       (501) staff       (20)      107 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/core/strategy_context/__init__.py
+-rw-r--r--   0 ihos       (501) staff       (20)     2062 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/core/strategy_context/cert_strategy_ctx.py
+-rw-r--r--   0 ihos       (501) staff       (20)     2812 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/core/strategy_context/encrypted_programming_strategy_ctx.py
+-rw-r--r--   0 ihos       (501) staff       (20)     1997 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/core/strategy_context/prov_packet_strategy_ctx.py
+-rw-r--r--   0 ihos       (501) staff       (20)     2890 2023-05-18 10:29:21.000000 cysecuretools-4.2.0/cysecuretools/core/strategy_context/provisioning_strategy_ctx.py
+-rw-r--r--   0 ihos       (501) staff       (20)      716 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/core/strops.py
+-rw-r--r--   0 ihos       (501) staff       (20)     4306 2023-05-18 10:29:21.000000 cysecuretools-4.2.0/cysecuretools/core/target_builder.py
+-rw-r--r--   0 ihos       (501) staff       (20)    11714 2023-05-18 10:29:21.000000 cysecuretools-4.2.0/cysecuretools/core/target_director.py
+-rw-r--r--   0 ihos       (501) staff       (20)      847 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/core/voltage_tool.py
+drwxr-xr-x   0 ihos       (501) staff       (20)        0 2023-05-18 10:54:48.221202 cysecuretools-4.2.0/cysecuretools/data/
+-rw-r--r--   0 ihos       (501) staff       (20)        0 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/data/__init__.py
+-rw-r--r--   0 ihos       (501) staff       (20)     1579 2023-05-18 10:29:21.000000 cysecuretools-4.2.0/cysecuretools/data/cy_bootloader_map.json
+drwxr-xr-x   0 ihos       (501) staff       (20)        0 2023-05-18 10:54:48.228789 cysecuretools-4.2.0/cysecuretools/data/mxs40sv2/
+-rw-r--r--   0 ihos       (501) staff       (20)     4698 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/data/mxs40sv2/mxs40sv2_ram_app_status_codes.py
+drwxr-xr-x   0 ihos       (501) staff       (20)        0 2023-05-18 10:54:48.237971 cysecuretools-4.2.0/cysecuretools/data/mxs40v1/
+-rw-r--r--   0 ihos       (501) staff       (20)        0 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/data/mxs40v1/__init__.py
+-rw-r--r--   0 ihos       (501) staff       (20)    13578 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/data/mxs40v1/mxs40v1_sfb_status_codes.py
+drwxr-xr-x   0 ihos       (501) staff       (20)        0 2023-05-18 10:54:48.284675 cysecuretools-4.2.0/cysecuretools/execute/
+-rw-r--r--   0 ihos       (501) staff       (20)        0 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/execute/__init__.py
+-rw-r--r--   0 ihos       (501) staff       (20)     3086 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/execute/bootloader_provider_mxs40v1.py
+drwxr-xr-x   0 ihos       (501) staff       (20)        0 2023-05-18 10:54:48.302133 cysecuretools-4.2.0/cysecuretools/execute/debug_cert/
+-rw-r--r--   0 ihos       (501) staff       (20)       97 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/execute/debug_cert/__init__.py
+-rw-r--r--   0 ihos       (501) staff       (20)     2924 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/execute/debug_cert/debug_cert_mxs40sv2.py
+-rw-r--r--   0 ihos       (501) staff       (20)     4365 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/execute/debug_cert/debug_cert_parser_mxs40sv2.py
+drwxr-xr-x   0 ihos       (501) staff       (20)        0 2023-05-18 10:54:48.335268 cysecuretools-4.2.0/cysecuretools/execute/encrypted_programming/
+-rw-r--r--   0 ihos       (501) staff       (20)        0 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/execute/encrypted_programming/__init__.py
+-rw-r--r--   0 ihos       (501) staff       (20)     2459 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/execute/encrypted_programming/aes_cipher.py
+-rw-r--r--   0 ihos       (501) staff       (20)     4024 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/execute/encrypted_programming/aes_header.py
+-rw-r--r--   0 ihos       (501) staff       (20)     5550 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/execute/encrypted_programming/aes_header_strategy.py
+-rw-r--r--   0 ihos       (501) staff       (20)     2857 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/execute/encrypted_programming/ecc_kdf.py
+-rw-r--r--   0 ihos       (501) staff       (20)     3204 2023-05-18 10:29:21.000000 cysecuretools-4.2.0/cysecuretools/execute/encrypted_programming/encrypted_programming.py
+drwxr-xr-x   0 ihos       (501) staff       (20)        0 2023-05-18 10:54:48.348715 cysecuretools-4.2.0/cysecuretools/execute/entrance_exam/
+-rw-r--r--   0 ihos       (501) staff       (20)        0 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/execute/entrance_exam/__init__.py
+-rw-r--r--   0 ihos       (501) staff       (20)     8164 2023-05-18 10:29:21.000000 cysecuretools-4.2.0/cysecuretools/execute/entrance_exam/exam_cyb06xx7.py
+-rw-r--r--   0 ihos       (501) staff       (20)     8849 2023-05-18 10:29:21.000000 cysecuretools-4.2.0/cysecuretools/execute/entrance_exam/exam_mxs40v1.py
+-rw-r--r--   0 ihos       (501) staff       (20)     5062 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/execute/image_cert.py
+drwxr-xr-x   0 ihos       (501) staff       (20)        0 2023-05-18 10:54:48.392051 cysecuretools-4.2.0/cysecuretools/execute/image_signing/
+-rw-r--r--   0 ihos       (501) staff       (20)        0 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/execute/image_signing/__init__.py
+-rw-r--r--   0 ihos       (501) staff       (20)     3152 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/execute/image_signing/encrypt_mxv40sv2.py
+-rw-r--r--   0 ihos       (501) staff       (20)     7260 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/execute/image_signing/image.py
+-rw-r--r--   0 ihos       (501) staff       (20)     1450 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/execute/image_signing/image_config_parser.py
+-rw-r--r--   0 ihos       (501) staff       (20)     3782 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/execute/image_signing/rsa_converter.py
+-rw-r--r--   0 ihos       (501) staff       (20)    18698 2023-05-18 10:29:21.000000 cysecuretools-4.2.0/cysecuretools/execute/image_signing/signtool_mxs40v1.py
+-rw-r--r--   0 ihos       (501) staff       (20)    17625 2023-05-18 10:29:21.000000 cysecuretools-4.2.0/cysecuretools/execute/image_signing/signtool_mxv40sv2.py
+-rw-r--r--   0 ihos       (501) staff       (20)     1231 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/execute/image_signing/xip_encryptor.py
+drwxr-xr-x   0 ihos       (501) staff       (20)        0 2023-05-18 10:54:48.426820 cysecuretools-4.2.0/cysecuretools/execute/imgtool/
+-rw-r--r--   0 ihos       (501) staff       (20)      650 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/execute/imgtool/__init__.py
+-rw-r--r--   0 ihos       (501) staff       (20)     1613 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/execute/imgtool/boot_record.py
+-rw-r--r--   0 ihos       (501) staff       (20)     1208 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/execute/imgtool/custom_encryptor.py
+-rw-r--r--   0 ihos       (501) staff       (20)    25962 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/execute/imgtool/image.py
+drwxr-xr-x   0 ihos       (501) staff       (20)        0 2023-05-18 10:54:48.482580 cysecuretools-4.2.0/cysecuretools/execute/imgtool/keys/
+-rw-r--r--   0 ihos       (501) staff       (20)     3737 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/execute/imgtool/keys/__init__.py
+-rw-r--r--   0 ihos       (501) staff       (20)     5388 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/execute/imgtool/keys/ecdsa.py
+-rw-r--r--   0 ihos       (501) staff       (20)     2970 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/execute/imgtool/keys/ecdsa_test.py
+-rw-r--r--   0 ihos       (501) staff       (20)     3090 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/execute/imgtool/keys/ed25519.py
+-rw-r--r--   0 ihos       (501) staff       (20)     3026 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/execute/imgtool/keys/ed25519_test.py
+-rw-r--r--   0 ihos       (501) staff       (20)     1822 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/execute/imgtool/keys/general.py
+-rw-r--r--   0 ihos       (501) staff       (20)     5422 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/execute/imgtool/keys/rsa.py
+-rw-r--r--   0 ihos       (501) staff       (20)     3810 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/execute/imgtool/keys/rsa_test.py
+-rw-r--r--   0 ihos       (501) staff       (20)     3169 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/execute/imgtool/keys/x25519.py
+-rwxr-xr-x   0 ihos       (501) staff       (20)    18214 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/execute/imgtool/main.py
+-rw-r--r--   0 ihos       (501) staff       (20)     1773 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/execute/imgtool/version.py
+-rw-r--r--   0 ihos       (501) staff       (20)     2587 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/execute/jwt.py
+-rw-r--r--   0 ihos       (501) staff       (20)     3924 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/execute/key_reader.py
+-rw-r--r--   0 ihos       (501) staff       (20)     1956 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/execute/key_reader_mxs40v1.py
+drwxr-xr-x   0 ihos       (501) staff       (20)        0 2023-05-18 10:54:48.498247 cysecuretools-4.2.0/cysecuretools/execute/key_source/
+-rw-r--r--   0 ihos       (501) staff       (20)        0 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/execute/key_source/__init__.py
+-rw-r--r--   0 ihos       (501) staff       (20)     5174 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/execute/key_source/key_source_mxs40sv2.py
+-rw-r--r--   0 ihos       (501) staff       (20)      825 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/execute/key_source/key_source_mxs40v1.py
+-rw-r--r--   0 ihos       (501) staff       (20)     8251 2023-05-18 10:29:21.000000 cysecuretools-4.2.0/cysecuretools/execute/keygen.py
+drwxr-xr-x   0 ihos       (501) staff       (20)        0 2023-05-18 10:54:48.555964 cysecuretools-4.2.0/cysecuretools/execute/programmer/
+-rw-r--r--   0 ihos       (501) staff       (20)      658 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/execute/programmer/__init__.py
+-rw-r--r--   0 ihos       (501) staff       (20)     8209 2023-05-18 10:29:21.000000 cysecuretools-4.2.0/cysecuretools/execute/programmer/base.py
+-rw-r--r--   0 ihos       (501) staff       (20)    12720 2023-05-18 10:29:21.000000 cysecuretools-4.2.0/cysecuretools/execute/programmer/openocd_server.py
+-rw-r--r--   0 ihos       (501) staff       (20)      938 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/execute/programmer/openocd_target_map.json
+-rw-r--r--   0 ihos       (501) staff       (20)    22128 2023-05-18 10:29:21.000000 cysecuretools-4.2.0/cysecuretools/execute/programmer/openocd_wrapper.py
+-rw-r--r--   0 ihos       (501) staff       (20)     1009 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/execute/programmer/programmer.py
+-rw-r--r--   0 ihos       (501) staff       (20)     1427 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/execute/programmer/pyocd_target_map.json
+-rw-r--r--   0 ihos       (501) staff       (20)    16156 2023-05-18 10:29:21.000000 cysecuretools-4.2.0/cysecuretools/execute/programmer/pyocd_wrapper.py
+drwxr-xr-x   0 ihos       (501) staff       (20)        0 2023-05-18 10:54:48.572987 cysecuretools-4.2.0/cysecuretools/execute/project_init/
+-rw-r--r--   0 ihos       (501) staff       (20)      122 2023-05-18 10:29:21.000000 cysecuretools-4.2.0/cysecuretools/execute/project_init/__init__.py
+-rw-r--r--   0 ihos       (501) staff       (20)     7365 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/execute/project_init/project_init_mxs40sv2.py
+-rw-r--r--   0 ihos       (501) staff       (20)     7933 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/execute/project_init/project_init_mxs40v1.py
+drwxr-xr-x   0 ihos       (501) staff       (20)        0 2023-05-18 10:54:48.606679 cysecuretools-4.2.0/cysecuretools/execute/provisioning/
+-rw-r--r--   0 ihos       (501) staff       (20)      200 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/execute/provisioning/__init__.py
+drwxr-xr-x   0 ihos       (501) staff       (20)        0 2023-05-18 10:54:48.627815 cysecuretools-4.2.0/cysecuretools/execute/provisioning/flows/
+-rw-r--r--   0 ihos       (501) staff       (20)      181 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/execute/provisioning/flows/__init__.py
+-rw-r--r--   0 ihos       (501) staff       (20)     5753 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/execute/provisioning/flows/application_mxs40sv2.py
+-rw-r--r--   0 ihos       (501) staff       (20)     3484 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/execute/provisioning/flows/flow_mxs40sv2.py
+-rw-r--r--   0 ihos       (501) staff       (20)     8975 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/execute/provisioning/load_ram_app.py
+-rw-r--r--   0 ihos       (501) staff       (20)     7139 2023-05-18 10:29:21.000000 cysecuretools-4.2.0/cysecuretools/execute/provisioning/provision_device_mxs40sv2.py
+-rw-r--r--   0 ihos       (501) staff       (20)    21411 2023-05-18 10:29:21.000000 cysecuretools-4.2.0/cysecuretools/execute/provisioning/provision_device_mxs40v1.py
+drwxr-xr-x   0 ihos       (501) staff       (20)        0 2023-05-18 10:54:48.645562 cysecuretools-4.2.0/cysecuretools/execute/provisioning_packet/
+-rw-r--r--   0 ihos       (501) staff       (20)      107 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/execute/provisioning_packet/__init__.py
+drwxr-xr-x   0 ihos       (501) staff       (20)        0 2023-05-18 10:54:48.707965 cysecuretools-4.2.0/cysecuretools/execute/provisioning_packet/lib/
+-rw-r--r--   0 ihos       (501) staff       (20)      564 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/execute/provisioning_packet/lib/__init__.py
+-rw-r--r--   0 ihos       (501) staff       (20)     5407 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/execute/provisioning_packet/lib/cyprov_crypto.py
+-rw-r--r--   0 ihos       (501) staff       (20)     1581 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/execute/provisioning_packet/lib/cyprov_customer.py
+-rw-r--r--   0 ihos       (501) staff       (20)     3514 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/execute/provisioning_packet/lib/cyprov_dev.py
+-rw-r--r--   0 ihos       (501) staff       (20)     1731 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/execute/provisioning_packet/lib/cyprov_entity.py
+-rw-r--r--   0 ihos       (501) staff       (20)     3428 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/execute/provisioning_packet/lib/cyprov_hsm.py
+-rw-r--r--   0 ihos       (501) staff       (20)     3153 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/execute/provisioning_packet/lib/cyprov_oem.py
+-rw-r--r--   0 ihos       (501) staff       (20)     3672 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/execute/provisioning_packet/lib/cyprov_pem.py
+-rw-r--r--   0 ihos       (501) staff       (20)     1049 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/execute/provisioning_packet/lib/cyprov_types.py
+-rw-r--r--   0 ihos       (501) staff       (20)     6784 2023-05-18 10:29:21.000000 cysecuretools-4.2.0/cysecuretools/execute/provisioning_packet/provisioning_packet_mxs40sv2.py
+-rw-r--r--   0 ihos       (501) staff       (20)     8310 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/execute/provisioning_packet/provisioning_packet_mxs40v1.py
+drwxr-xr-x   0 ihos       (501) staff       (20)        0 2023-05-18 10:54:48.732637 cysecuretools-4.2.0/cysecuretools/execute/silicon_data_reader/
+-rw-r--r--   0 ihos       (501) staff       (20)     1218 2023-05-18 10:29:21.000000 cysecuretools-4.2.0/cysecuretools/execute/silicon_data_reader/__init__.py
+-rw-r--r--   0 ihos       (501) staff       (20)     3893 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/execute/silicon_data_reader/silicon_data_reader_mxs40sv2.py
+-rw-r--r--   0 ihos       (501) staff       (20)     2856 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/execute/silicon_data_reader/silicon_data_reader_mxs40v1.py
+-rw-r--r--   0 ihos       (501) staff       (20)    22517 2023-05-18 10:29:21.000000 cysecuretools-4.2.0/cysecuretools/execute/sys_call.py
+drwxr-xr-x   0 ihos       (501) staff       (20)        0 2023-05-18 10:54:48.749827 cysecuretools-4.2.0/cysecuretools/execute/version_provider/
+-rw-r--r--   0 ihos       (501) staff       (20)      124 2023-05-18 10:29:21.000000 cysecuretools-4.2.0/cysecuretools/execute/version_provider/__init__.py
+-rw-r--r--   0 ihos       (501) staff       (20)     5951 2023-05-18 10:29:21.000000 cysecuretools-4.2.0/cysecuretools/execute/version_provider/version_provider_mxs40sv2.py
+-rw-r--r--   0 ihos       (501) staff       (20)     8684 2023-05-18 10:29:21.000000 cysecuretools-4.2.0/cysecuretools/execute/version_provider/version_provider_mxs40v1.py
+drwxr-xr-x   0 ihos       (501) staff       (20)        0 2023-05-18 10:54:48.762015 cysecuretools-4.2.0/cysecuretools/execute/voltage_tool/
+-rw-r--r--   0 ihos       (501) staff       (20)        0 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/execute/voltage_tool/__init__.py
+-rw-r--r--   0 ihos       (501) staff       (20)     3139 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/execute/voltage_tool/lvd_voltage_picker.py
+-rw-r--r--   0 ihos       (501) staff       (20)     1251 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/execute/voltage_tool/voltage_tool_mxs40v1.py
+-rw-r--r--   0 ihos       (501) staff       (20)    40522 2023-05-18 10:29:21.000000 cysecuretools-4.2.0/cysecuretools/main.py
+-rw-r--r--   0 ihos       (501) staff       (20)      718 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/pkg_globals.py
+-rw-r--r--   0 ihos       (501) staff       (20)       79 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/settings.json
+drwxr-xr-x   0 ihos       (501) staff       (20)        0 2023-05-18 10:54:48.767948 cysecuretools-4.2.0/cysecuretools/targets/
+-rw-r--r--   0 ihos       (501) staff       (20)     5662 2023-05-18 10:29:21.000000 cysecuretools-4.2.0/cysecuretools/targets/__init__.py
+drwxr-xr-x   0 ihos       (501) staff       (20)        0 2023-05-18 10:54:48.768920 cysecuretools-4.2.0/cysecuretools/targets/common/
+-rw-r--r--   0 ihos       (501) staff       (20)        0 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/targets/common/__init__.py
+drwxr-xr-x   0 ihos       (501) staff       (20)        0 2023-05-18 10:54:48.824049 cysecuretools-4.2.0/cysecuretools/targets/common/mxs40sv2/
+-rw-r--r--   0 ihos       (501) staff       (20)      160 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/targets/common/mxs40sv2/__init__.py
+-rw-r--r--   0 ihos       (501) staff       (20)     1336 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/targets/common/mxs40sv2/asset.py
+-rw-r--r--   0 ihos       (501) staff       (20)     1376 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/targets/common/mxs40sv2/asset_builder.py
+-rw-r--r--   0 ihos       (501) staff       (20)     3073 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/targets/common/mxs40sv2/asset_enums.py
+drwxr-xr-x   0 ihos       (501) staff       (20)        0 2023-05-18 10:54:48.864425 cysecuretools-4.2.0/cysecuretools/targets/common/mxs40sv2/dependencies_validator/
+-rw-r--r--   0 ihos       (501) staff       (20)     1201 2023-05-18 10:29:21.000000 cysecuretools-4.2.0/cysecuretools/targets/common/mxs40sv2/dependencies_validator/__init__.py
+-rw-r--r--   0 ihos       (501) staff       (20)     1964 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/targets/common/mxs40sv2/dependencies_validator/access_restrictions_validator.py
+-rw-r--r--   0 ihos       (501) staff       (20)     1304 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/targets/common/mxs40sv2/dependencies_validator/encryption_key_validator.py
+-rw-r--r--   0 ihos       (501) staff       (20)     1919 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/targets/common/mxs40sv2/dependencies_validator/hci_mode_validator.py
+-rw-r--r--   0 ihos       (501) staff       (20)     3387 2023-05-18 10:29:21.000000 cysecuretools-4.2.0/cysecuretools/targets/common/mxs40sv2/dependencies_validator/nv_counter_validator.py
+-rw-r--r--   0 ihos       (501) staff       (20)     1508 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/targets/common/mxs40sv2/dependencies_validator/pre_build_keys_exist_validator.py
+-rw-r--r--   0 ihos       (501) staff       (20)     1198 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/targets/common/mxs40sv2/dependencies_validator/revoke_oem_encryption_validator.py
+-rw-r--r--   0 ihos       (501) staff       (20)     1151 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/targets/common/mxs40sv2/enums.py
+-rw-r--r--   0 ihos       (501) staff       (20)     3537 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/targets/common/mxs40sv2/flow_parser.py
+drwxr-xr-x   0 ihos       (501) staff       (20)        0 2023-05-18 10:54:48.884601 cysecuretools-4.2.0/cysecuretools/targets/common/mxs40sv2/json/
+-rw-r--r--   0 ihos       (501) staff       (20)    24916 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/targets/common/mxs40sv2/json/cyw20829_no_secure.json_schema
+-rw-r--r--   0 ihos       (501) staff       (20)     2049 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/targets/common/mxs40sv2/json/cyw20829_reprovisioning_no_secure.json_schema
+-rw-r--r--   0 ihos       (501) staff       (20)     7972 2023-05-18 10:29:21.000000 cysecuretools-4.2.0/cysecuretools/targets/common/mxs40sv2/json/cyw20829_reprovisioning_secure.json_schema
+-rw-r--r--   0 ihos       (501) staff       (20)    29537 2023-05-18 10:29:21.000000 cysecuretools-4.2.0/cysecuretools/targets/common/mxs40sv2/json/cyw20829_secure.json_schema
+-rw-r--r--   0 ihos       (501) staff       (20)     3282 2023-05-18 10:29:21.000000 cysecuretools-4.2.0/cysecuretools/targets/common/mxs40sv2/nv_counter_calc.py
+-rw-r--r--   0 ihos       (501) staff       (20)    12510 2023-05-18 10:29:21.000000 cysecuretools-4.2.0/cysecuretools/targets/common/mxs40sv2/policy_parser.py
+-rw-r--r--   0 ihos       (501) staff       (20)     4182 2023-05-18 10:29:21.000000 cysecuretools-4.2.0/cysecuretools/targets/common/mxs40sv2/policy_validator.py
+drwxr-xr-x   0 ihos       (501) staff       (20)        0 2023-05-18 10:54:48.918414 cysecuretools-4.2.0/cysecuretools/targets/common/p64/
+-rw-r--r--   0 ihos       (501) staff       (20)        0 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/targets/common/p64/__init__.py
+-rw-r--r--   0 ihos       (501) staff       (20)      839 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/targets/common/p64/enums.py
+drwxr-xr-x   0 ihos       (501) staff       (20)        0 2023-05-18 10:54:48.927355 cysecuretools-4.2.0/cysecuretools/targets/common/p64/json/
+-rw-r--r--   0 ihos       (501) staff       (20)     4452 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/targets/common/p64/json/policy_template.json
+-rw-r--r--   0 ihos       (501) staff       (20)    15796 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/targets/common/p64/json/schema.json_schema
+-rw-r--r--   0 ihos       (501) staff       (20)     5756 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/targets/common/p64/policy_filter.py
+-rw-r--r--   0 ihos       (501) staff       (20)    15561 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/targets/common/p64/policy_parser.py
+-rw-r--r--   0 ihos       (501) staff       (20)    46232 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/targets/common/p64/policy_validator.py
+drwxr-xr-x   0 ihos       (501) staff       (20)        0 2023-05-18 10:54:48.935210 cysecuretools-4.2.0/cysecuretools/targets/common/p64/prebuilt/
+-rw-r--r--   0 ihos       (501) staff       (20)      511 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/targets/common/p64/prebuilt/hsm_state.json
+-rw-r--r--   0 ihos       (501) staff       (20)      511 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/targets/common/p64/prebuilt/oem_state.json
+-rw-r--r--   0 ihos       (501) staff       (20)     1381 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/targets/common/p64/silicon_data_parser.py
+drwxr-xr-x   0 ihos       (501) staff       (20)        0 2023-05-18 10:54:48.938401 cysecuretools-4.2.0/cysecuretools/targets/common/prebuilt/
+-rw-r--r--   0 ihos       (501) staff       (20)      173 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/targets/common/prebuilt/bootloader_pub_key.json
+drwxr-xr-x   0 ihos       (501) staff       (20)        0 2023-05-18 10:54:48.951127 cysecuretools-4.2.0/cysecuretools/targets/cyb06xx5/
+-rw-r--r--   0 ihos       (501) staff       (20)       75 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/targets/cyb06xx5/__init__.py
+drwxr-xr-x   0 ihos       (501) staff       (20)        0 2023-05-18 10:54:48.954395 cysecuretools-4.2.0/cysecuretools/targets/cyb06xx5/keys/
+-rw-r--r--   0 ihos       (501) staff       (20)      191 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/targets/cyb06xx5/keys/cy_pub_key.json
+drwxr-xr-x   0 ihos       (501) staff       (20)        0 2023-05-18 10:54:48.967235 cysecuretools-4.2.0/cysecuretools/targets/cyb06xx5/maps/
+-rw-r--r--   0 ihos       (501) staff       (20)        0 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/targets/cyb06xx5/maps/__init__.py
+-rw-r--r--   0 ihos       (501) staff       (20)     1599 2023-05-18 10:29:21.000000 cysecuretools-4.2.0/cysecuretools/targets/cyb06xx5/maps/memory_map.py
+-rw-r--r--   0 ihos       (501) staff       (20)     2401 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/targets/cyb06xx5/maps/register_map.py
+drwxr-xr-x   0 ihos       (501) staff       (20)        0 2023-05-18 10:54:48.985546 cysecuretools-4.2.0/cysecuretools/targets/cyb06xx5/packets/
+-rw-r--r--   0 ihos       (501) staff       (20)      371 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/targets/cyb06xx5/packets/control_dap_cert.json
+-rw-r--r--   0 ihos       (501) staff       (20)     1051 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/targets/cyb06xx5/packets/cy_auth_512k_b0_sample.jwt
+-rw-r--r--   0 ihos       (501) staff       (20)      151 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/targets/cyb06xx5/packets/ec_key_tmpl.json
+-rw-r--r--   0 ihos       (501) staff       (20)     4490 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/targets/cyb06xx5/packets/entrance_exam.jwt
+drwxr-xr-x   0 ihos       (501) staff       (20)        0 2023-05-18 10:54:49.004017 cysecuretools-4.2.0/cysecuretools/targets/cyb06xx5/policy/
+-rw-r--r--   0 ihos       (501) staff       (20)     5312 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/targets/cyb06xx5/policy/policy_multi_CM0_CM4.json
+-rw-r--r--   0 ihos       (501) staff       (20)     5314 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/targets/cyb06xx5/policy/policy_multi_CM0_CM4_smif.json
+-rw-r--r--   0 ihos       (501) staff       (20)     4927 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/targets/cyb06xx5/policy/policy_single_CM0_CM4.json
+-rw-r--r--   0 ihos       (501) staff       (20)     4927 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/targets/cyb06xx5/policy/policy_single_CM0_CM4_smif.json
+drwxr-xr-x   0 ihos       (501) staff       (20)        0 2023-05-18 10:54:47.881461 cysecuretools-4.2.0/cysecuretools/targets/cyb06xx5/prebuilt/
+drwxr-xr-x   0 ihos       (501) staff       (20)        0 2023-05-18 10:54:49.013319 cysecuretools-4.2.0/cysecuretools/targets/cyb06xx5/prebuilt/CyBootloader_Release/
+-rw-r--r--   0 ihos       (501) staff       (20)   134553 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/targets/cyb06xx5/prebuilt/CyBootloader_Release/CypressBootloader_CM0p.hex
+-rw-r--r--   0 ihos       (501) staff       (20)      536 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/targets/cyb06xx5/prebuilt/CyBootloader_Release/CypressBootloader_CM0p.jwt
+drwxr-xr-x   0 ihos       (501) staff       (20)        0 2023-05-18 10:54:49.022255 cysecuretools-4.2.0/cysecuretools/targets/cyb06xx5/prebuilt/CyBootloader_WithLogs/
+-rw-r--r--   0 ihos       (501) staff       (20)   148119 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/targets/cyb06xx5/prebuilt/CyBootloader_WithLogs/CypressBootloader_CM0p.hex
+-rw-r--r--   0 ihos       (501) staff       (20)      540 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/targets/cyb06xx5/prebuilt/CyBootloader_WithLogs/CypressBootloader_CM0p.jwt
+-rw-r--r--   0 ihos       (501) staff       (20)     4562 2023-05-18 10:29:21.000000 cysecuretools-4.2.0/cysecuretools/targets/cyb06xx5/target_builder.py
+drwxr-xr-x   0 ihos       (501) staff       (20)        0 2023-05-18 10:54:49.029820 cysecuretools-4.2.0/cysecuretools/targets/cyb06xx7/
+-rw-r--r--   0 ihos       (501) staff       (20)        0 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/targets/cyb06xx7/__init__.py
+drwxr-xr-x   0 ihos       (501) staff       (20)        0 2023-05-18 10:54:49.033059 cysecuretools-4.2.0/cysecuretools/targets/cyb06xx7/keys/
+-rw-r--r--   0 ihos       (501) staff       (20)      191 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/targets/cyb06xx7/keys/cy_pub_key.json
+drwxr-xr-x   0 ihos       (501) staff       (20)        0 2023-05-18 10:54:49.047056 cysecuretools-4.2.0/cysecuretools/targets/cyb06xx7/maps/
+-rw-r--r--   0 ihos       (501) staff       (20)        0 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/targets/cyb06xx7/maps/__init__.py
+-rw-r--r--   0 ihos       (501) staff       (20)     2001 2023-05-18 10:29:21.000000 cysecuretools-4.2.0/cysecuretools/targets/cyb06xx7/maps/memory_map.py
+-rw-r--r--   0 ihos       (501) staff       (20)     2401 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/targets/cyb06xx7/maps/register_map.py
+drwxr-xr-x   0 ihos       (501) staff       (20)        0 2023-05-18 10:54:49.061004 cysecuretools-4.2.0/cysecuretools/targets/cyb06xx7/packets/
+-rw-r--r--   0 ihos       (501) staff       (20)      371 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/targets/cyb06xx7/packets/control_dap_cert.json
+-rw-r--r--   0 ihos       (501) staff       (20)     1031 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/targets/cyb06xx7/packets/cy_auth_1m_b0_sample.jwt
+-rw-r--r--   0 ihos       (501) staff       (20)      151 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/targets/cyb06xx7/packets/ec_key_tmpl.json
+-rw-r--r--   0 ihos       (501) staff       (20)     4490 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/targets/cyb06xx7/packets/entrance_exam.jwt
+drwxr-xr-x   0 ihos       (501) staff       (20)        0 2023-05-18 10:54:49.099640 cysecuretools-4.2.0/cysecuretools/targets/cyb06xx7/policy/
+-rw-r--r--   0 ihos       (501) staff       (20)     5095 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/targets/cyb06xx7/policy/policy_multi_CM0_CM4.json
+-rw-r--r--   0 ihos       (501) staff       (20)     5095 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/targets/cyb06xx7/policy/policy_multi_CM0_CM4_smif.json
+-rw-r--r--   0 ihos       (501) staff       (20)     5740 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/targets/cyb06xx7/policy/policy_multi_CM0_CM4_smif_swap.json
+-rw-r--r--   0 ihos       (501) staff       (20)     5739 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/targets/cyb06xx7/policy/policy_multi_CM0_CM4_swap.json
+-rw-r--r--   0 ihos       (501) staff       (20)     4883 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/targets/cyb06xx7/policy/policy_single_CM0_CM4.json
+-rw-r--r--   0 ihos       (501) staff       (20)     4883 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/targets/cyb06xx7/policy/policy_single_CM0_CM4_smif.json
+-rw-r--r--   0 ihos       (501) staff       (20)     5531 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/targets/cyb06xx7/policy/policy_single_CM0_CM4_smif_swap.json
+-rw-r--r--   0 ihos       (501) staff       (20)     5529 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/targets/cyb06xx7/policy/policy_single_CM0_CM4_swap.json
+drwxr-xr-x   0 ihos       (501) staff       (20)        0 2023-05-18 10:54:47.886198 cysecuretools-4.2.0/cysecuretools/targets/cyb06xx7/prebuilt/
+drwxr-xr-x   0 ihos       (501) staff       (20)        0 2023-05-18 10:54:49.112820 cysecuretools-4.2.0/cysecuretools/targets/cyb06xx7/prebuilt/CyBootloader_Release/
+-rw-r--r--   0 ihos       (501) staff       (20)   138714 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/targets/cyb06xx7/prebuilt/CyBootloader_Release/CypressBootloader_CM0p.hex
+-rw-r--r--   0 ihos       (501) staff       (20)      543 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/targets/cyb06xx7/prebuilt/CyBootloader_Release/CypressBootloader_CM0p.jwt
+drwxr-xr-x   0 ihos       (501) staff       (20)        0 2023-05-18 10:54:49.123089 cysecuretools-4.2.0/cysecuretools/targets/cyb06xx7/prebuilt/CyBootloader_WithLogs/
+-rw-r--r--   0 ihos       (501) staff       (20)   150520 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/targets/cyb06xx7/prebuilt/CyBootloader_WithLogs/CypressBootloader_CM0p.hex
+-rw-r--r--   0 ihos       (501) staff       (20)      542 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/targets/cyb06xx7/prebuilt/CyBootloader_WithLogs/CypressBootloader_CM0p.jwt
+-rw-r--r--   0 ihos       (501) staff       (20)     4465 2023-05-18 10:29:21.000000 cysecuretools-4.2.0/cysecuretools/targets/cyb06xx7/target_builder.py
+drwxr-xr-x   0 ihos       (501) staff       (20)        0 2023-05-18 10:54:49.135164 cysecuretools-4.2.0/cysecuretools/targets/cyb06xxa/
+-rw-r--r--   0 ihos       (501) staff       (20)       75 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/targets/cyb06xxa/__init__.py
+drwxr-xr-x   0 ihos       (501) staff       (20)        0 2023-05-18 10:54:49.137169 cysecuretools-4.2.0/cysecuretools/targets/cyb06xxa/keys/
+-rw-r--r--   0 ihos       (501) staff       (20)      191 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/targets/cyb06xxa/keys/cy_pub_key.json
+drwxr-xr-x   0 ihos       (501) staff       (20)        0 2023-05-18 10:54:49.148477 cysecuretools-4.2.0/cysecuretools/targets/cyb06xxa/maps/
+-rw-r--r--   0 ihos       (501) staff       (20)        0 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/targets/cyb06xxa/maps/__init__.py
+-rw-r--r--   0 ihos       (501) staff       (20)     1692 2023-05-18 10:29:21.000000 cysecuretools-4.2.0/cysecuretools/targets/cyb06xxa/maps/memory_map.py
+-rw-r--r--   0 ihos       (501) staff       (20)     2402 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/targets/cyb06xxa/maps/register_map.py
+drwxr-xr-x   0 ihos       (501) staff       (20)        0 2023-05-18 10:54:49.160752 cysecuretools-4.2.0/cysecuretools/targets/cyb06xxa/packets/
+-rw-r--r--   0 ihos       (501) staff       (20)      371 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/targets/cyb06xxa/packets/control_dap_cert.json
+-rw-r--r--   0 ihos       (501) staff       (20)     1051 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/targets/cyb06xxa/packets/cy_auth_2m_b0_sample.jwt
+-rw-r--r--   0 ihos       (501) staff       (20)      151 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/targets/cyb06xxa/packets/ec_key_tmpl.json
+-rw-r--r--   0 ihos       (501) staff       (20)     4490 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/targets/cyb06xxa/packets/entrance_exam.jwt
+drwxr-xr-x   0 ihos       (501) staff       (20)        0 2023-05-18 10:54:49.181908 cysecuretools-4.2.0/cysecuretools/targets/cyb06xxa/policy/
+-rw-r--r--   0 ihos       (501) staff       (20)     6068 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/targets/cyb06xxa/policy/policy_multi_CM0_CM4_smif_swap.json
+-rw-r--r--   0 ihos       (501) staff       (20)     5784 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/targets/cyb06xxa/policy/policy_multi_CM0_CM4_swap.json
+-rw-r--r--   0 ihos       (501) staff       (20)     5621 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/targets/cyb06xxa/policy/policy_single_CM0_CM4_smif_swap.json
+-rw-r--r--   0 ihos       (501) staff       (20)     5573 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/targets/cyb06xxa/policy/policy_single_CM0_CM4_swap.json
+drwxr-xr-x   0 ihos       (501) staff       (20)        0 2023-05-18 10:54:47.890798 cysecuretools-4.2.0/cysecuretools/targets/cyb06xxa/prebuilt/
+drwxr-xr-x   0 ihos       (501) staff       (20)        0 2023-05-18 10:54:49.191202 cysecuretools-4.2.0/cysecuretools/targets/cyb06xxa/prebuilt/CyBootloader_Release_swap/
+-rw-r--r--   0 ihos       (501) staff       (20)   138738 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/targets/cyb06xxa/prebuilt/CyBootloader_Release_swap/CypressBootloader_CM0p.hex
+-rw-r--r--   0 ihos       (501) staff       (20)      592 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/targets/cyb06xxa/prebuilt/CyBootloader_Release_swap/CypressBootloader_CM0p.jwt
+drwxr-xr-x   0 ihos       (501) staff       (20)        0 2023-05-18 10:54:49.201285 cysecuretools-4.2.0/cysecuretools/targets/cyb06xxa/prebuilt/CyBootloader_WithLogs_swap/
+-rw-r--r--   0 ihos       (501) staff       (20)   155454 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/targets/cyb06xxa/prebuilt/CyBootloader_WithLogs_swap/CypressBootloader_CM0p.hex
+-rw-r--r--   0 ihos       (501) staff       (20)      588 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/targets/cyb06xxa/prebuilt/CyBootloader_WithLogs_swap/CypressBootloader_CM0p.jwt
+-rw-r--r--   0 ihos       (501) staff       (20)     4468 2023-05-18 10:29:21.000000 cysecuretools-4.2.0/cysecuretools/targets/cyb06xxa/target_builder.py
+drwxr-xr-x   0 ihos       (501) staff       (20)        0 2023-05-18 10:54:49.213719 cysecuretools-4.2.0/cysecuretools/targets/cys06xxa/
+-rw-r--r--   0 ihos       (501) staff       (20)       75 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/targets/cys06xxa/__init__.py
+drwxr-xr-x   0 ihos       (501) staff       (20)        0 2023-05-18 10:54:49.216895 cysecuretools-4.2.0/cysecuretools/targets/cys06xxa/keys/
+-rw-r--r--   0 ihos       (501) staff       (20)      191 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/targets/cys06xxa/keys/cy_pub_key.json
+drwxr-xr-x   0 ihos       (501) staff       (20)        0 2023-05-18 10:54:49.232996 cysecuretools-4.2.0/cysecuretools/targets/cys06xxa/packets/
+-rw-r--r--   0 ihos       (501) staff       (20)      371 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/targets/cys06xxa/packets/control_dap_cert.json
+-rw-r--r--   0 ihos       (501) staff       (20)     1031 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/targets/cys06xxa/packets/cy_auth_2m_s0_sample.jwt
+-rw-r--r--   0 ihos       (501) staff       (20)      151 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/targets/cys06xxa/packets/ec_key_tmpl.json
+-rw-r--r--   0 ihos       (501) staff       (20)     4490 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/targets/cys06xxa/packets/entrance_exam.jwt
+drwxr-xr-x   0 ihos       (501) staff       (20)        0 2023-05-18 10:54:49.252777 cysecuretools-4.2.0/cysecuretools/targets/cys06xxa/policy/
+-rw-r--r--   0 ihos       (501) staff       (20)     6068 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/targets/cys06xxa/policy/policy_multi_CM0_CM4_smif_swap.json
+-rw-r--r--   0 ihos       (501) staff       (20)     5784 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/targets/cys06xxa/policy/policy_multi_CM0_CM4_swap.json
+-rw-r--r--   0 ihos       (501) staff       (20)     5621 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/targets/cys06xxa/policy/policy_single_CM0_CM4_smif_swap.json
+-rw-r--r--   0 ihos       (501) staff       (20)     5573 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/targets/cys06xxa/policy/policy_single_CM0_CM4_swap.json
+drwxr-xr-x   0 ihos       (501) staff       (20)        0 2023-05-18 10:54:47.894629 cysecuretools-4.2.0/cysecuretools/targets/cys06xxa/prebuilt/
+drwxr-xr-x   0 ihos       (501) staff       (20)        0 2023-05-18 10:54:49.262236 cysecuretools-4.2.0/cysecuretools/targets/cys06xxa/prebuilt/CyBootloader_Release_swap/
+-rw-r--r--   0 ihos       (501) staff       (20)   138738 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/targets/cys06xxa/prebuilt/CyBootloader_Release_swap/CypressBootloader_CM0p.hex
+-rw-r--r--   0 ihos       (501) staff       (20)      592 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/targets/cys06xxa/prebuilt/CyBootloader_Release_swap/CypressBootloader_CM0p.jwt
+drwxr-xr-x   0 ihos       (501) staff       (20)        0 2023-05-18 10:54:49.272609 cysecuretools-4.2.0/cysecuretools/targets/cys06xxa/prebuilt/CyBootloader_WithLogs_swap/
+-rw-r--r--   0 ihos       (501) staff       (20)   155454 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/targets/cys06xxa/prebuilt/CyBootloader_WithLogs_swap/CypressBootloader_CM0p.hex
+-rw-r--r--   0 ihos       (501) staff       (20)      588 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/targets/cys06xxa/prebuilt/CyBootloader_WithLogs_swap/CypressBootloader_CM0p.jwt
+-rw-r--r--   0 ihos       (501) staff       (20)     4468 2023-05-18 10:29:21.000000 cysecuretools-4.2.0/cysecuretools/targets/cys06xxa/target_builder.py
+drwxr-xr-x   0 ihos       (501) staff       (20)        0 2023-05-18 10:54:49.293330 cysecuretools-4.2.0/cysecuretools/targets/cyw20829/
+-rw-r--r--   0 ihos       (501) staff       (20)       74 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/targets/cyw20829/__init__.py
+drwxr-xr-x   0 ihos       (501) staff       (20)        0 2023-05-18 10:54:49.326872 cysecuretools-4.2.0/cysecuretools/targets/cyw20829/flows/
+-rw-r--r--   0 ihos       (501) staff       (20)        0 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/targets/cyw20829/flows/__init__.py
+-rw-r--r--   0 ihos       (501) staff       (20)     8407 2023-05-18 10:29:21.000000 cysecuretools-4.2.0/cysecuretools/targets/cyw20829/flows/asset_map.py
+-rw-r--r--   0 ihos       (501) staff       (20)     1020 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/targets/cyw20829/flows/load_app_data.py
+-rw-r--r--   0 ihos       (501) staff       (20)      179 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/targets/cyw20829/flows/oem_assets.json
+-rw-r--r--   0 ihos       (501) staff       (20)      858 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/targets/cyw20829/flows/prov_flows.json
+-rw-r--r--   0 ihos       (501) staff       (20)       94 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/targets/cyw20829/flows/reprovisioning_assets.json
+-rw-r--r--   0 ihos       (501) staff       (20)     9210 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/targets/cyw20829/flows/reverse_asset_map.py
+drwxr-xr-x   0 ihos       (501) staff       (20)        0 2023-05-18 10:54:49.334383 cysecuretools-4.2.0/cysecuretools/targets/cyw20829/keys/
+-rw-r--r--   0 ihos       (501) staff       (20)      460 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/targets/cyw20829/keys/pub_hci_0.pem
+-rw-r--r--   0 ihos       (501) staff       (20)      460 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/targets/cyw20829/keys/pub_hci_1.pem
+drwxr-xr-x   0 ihos       (501) staff       (20)        0 2023-05-18 10:54:49.345423 cysecuretools-4.2.0/cysecuretools/targets/cyw20829/maps/
+-rw-r--r--   0 ihos       (501) staff       (20)        0 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/targets/cyw20829/maps/__init__.py
+-rw-r--r--   0 ihos       (501) staff       (20)     1052 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/targets/cyw20829/maps/memory_map.py
+-rw-r--r--   0 ihos       (501) staff       (20)     1715 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/targets/cyw20829/maps/register_map.py
+drwxr-xr-x   0 ihos       (501) staff       (20)        0 2023-05-18 10:54:49.353465 cysecuretools-4.2.0/cysecuretools/targets/cyw20829/packets/
+drwxr-xr-x   0 ihos       (501) staff       (20)        0 2023-05-18 10:54:47.898919 cysecuretools-4.2.0/cysecuretools/targets/cyw20829/packets/apps/
+drwxr-xr-x   0 ihos       (501) staff       (20)        0 2023-05-18 10:54:49.368260 cysecuretools-4.2.0/cysecuretools/targets/cyw20829/packets/apps/prov_oem/
+-rw-r--r--   0 ihos       (501) staff       (20)      235 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/targets/cyw20829/packets/apps/prov_oem/config.json
+-rw-r--r--   0 ihos       (501) staff       (20)     7780 2023-05-18 10:29:21.000000 cysecuretools-4.2.0/cysecuretools/targets/cyw20829/packets/apps/prov_oem/cyapp_prov_oem_signed_icv0.bin
+-rwxr-xr-x   0 ihos       (501) staff       (20)      375 2023-05-18 10:29:21.000000 cysecuretools-4.2.0/cysecuretools/targets/cyw20829/packets/apps/prov_oem/info.txt
+drwxr-xr-x   0 ihos       (501) staff       (20)        0 2023-05-18 10:54:49.381095 cysecuretools-4.2.0/cysecuretools/targets/cyw20829/packets/apps/reprovisioning/
+-rw-r--r--   0 ihos       (501) staff       (20)      241 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/targets/cyw20829/packets/apps/reprovisioning/config.json
+-rw-r--r--   0 ihos       (501) staff       (20)    28868 2023-05-18 10:29:21.000000 cysecuretools-4.2.0/cysecuretools/targets/cyw20829/packets/apps/reprovisioning/cyapp_reprovisioning_signed_icv0.bin
+-rwxr-xr-x   0 ihos       (501) staff       (20)      264 2023-05-18 10:29:21.000000 cysecuretools-4.2.0/cysecuretools/targets/cyw20829/packets/apps/reprovisioning/info.txt
+drwxr-xr-x   0 ihos       (501) staff       (20)        0 2023-05-18 10:54:49.392899 cysecuretools-4.2.0/cysecuretools/targets/cyw20829/packets/apps/to_rma/
+-rw-r--r--   0 ihos       (501) staff       (20)      269 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/targets/cyw20829/packets/apps/to_rma/config.json
+-rw-r--r--   0 ihos       (501) staff       (20)    28676 2023-05-18 10:29:21.000000 cysecuretools-4.2.0/cysecuretools/targets/cyw20829/packets/apps/to_rma/cyapp_to_rma_signed_icv0.bin
+-rwxr-xr-x   0 ihos       (501) staff       (20)      289 2023-05-18 10:29:21.000000 cysecuretools-4.2.0/cysecuretools/targets/cyw20829/packets/apps/to_rma/info.txt
+-rw-r--r--   0 ihos       (501) staff       (20)      624 2023-05-18 10:29:21.000000 cysecuretools-4.2.0/cysecuretools/targets/cyw20829/packets/debug_cert.json
+-rw-r--r--   0 ihos       (501) staff       (20)      168 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/targets/cyw20829/packets/rsa_key_tmpl.json
+drwxr-xr-x   0 ihos       (501) staff       (20)        0 2023-05-18 10:54:49.413759 cysecuretools-4.2.0/cysecuretools/targets/cyw20829/policy/
+-rw-r--r--   0 ihos       (501) staff       (20)     6135 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/targets/cyw20829/policy/policy_hci_secure.json
+-rw-r--r--   0 ihos       (501) staff       (20)     6344 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/targets/cyw20829/policy/policy_no_secure.json
+-rw-r--r--   0 ihos       (501) staff       (20)      374 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/targets/cyw20829/policy/policy_reprovisioning_no_secure.json
+-rw-r--r--   0 ihos       (501) staff       (20)     2099 2023-05-18 10:29:21.000000 cysecuretools-4.2.0/cysecuretools/targets/cyw20829/policy/policy_reprovisioning_secure.json
+-rw-r--r--   0 ihos       (501) staff       (20)     8568 2023-05-18 10:29:21.000000 cysecuretools-4.2.0/cysecuretools/targets/cyw20829/policy/policy_secure.json
+-rw-r--r--   0 ihos       (501) staff       (20)     2841 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/targets/cyw20829/policy_generator.py
+-rw-r--r--   0 ihos       (501) staff       (20)     4481 2023-05-18 10:29:21.000000 cysecuretools-4.2.0/cysecuretools/targets/cyw20829/target_builder.py
+drwxr-xr-x   0 ihos       (501) staff       (20)        0 2023-05-18 10:54:49.426161 cysecuretools-4.2.0/cysecuretools/targets/cyw20829_a0/
+-rw-r--r--   0 ihos       (501) staff       (20)       79 2023-05-18 10:29:21.000000 cysecuretools-4.2.0/cysecuretools/targets/cyw20829_a0/__init__.py
+drwxr-xr-x   0 ihos       (501) staff       (20)        0 2023-05-18 10:54:49.435227 cysecuretools-4.2.0/cysecuretools/targets/cyw20829_a0/flows/
+-rw-r--r--   0 ihos       (501) staff       (20)      179 2023-05-18 10:29:21.000000 cysecuretools-4.2.0/cysecuretools/targets/cyw20829_a0/flows/oem_assets.json
+-rw-r--r--   0 ihos       (501) staff       (20)      858 2023-05-18 10:29:21.000000 cysecuretools-4.2.0/cysecuretools/targets/cyw20829_a0/flows/prov_flows.json
+-rw-r--r--   0 ihos       (501) staff       (20)       94 2023-05-18 10:29:21.000000 cysecuretools-4.2.0/cysecuretools/targets/cyw20829_a0/flows/reprovisioning_assets.json
+drwxr-xr-x   0 ihos       (501) staff       (20)        0 2023-05-18 10:54:49.439997 cysecuretools-4.2.0/cysecuretools/targets/cyw20829_a0/keys/
+-rw-r--r--   0 ihos       (501) staff       (20)      460 2023-05-18 10:29:21.000000 cysecuretools-4.2.0/cysecuretools/targets/cyw20829_a0/keys/pub_hci_0.pem
+-rw-r--r--   0 ihos       (501) staff       (20)      460 2023-05-18 10:29:21.000000 cysecuretools-4.2.0/cysecuretools/targets/cyw20829_a0/keys/pub_hci_1.pem
+drwxr-xr-x   0 ihos       (501) staff       (20)        0 2023-05-18 10:54:49.446155 cysecuretools-4.2.0/cysecuretools/targets/cyw20829_a0/packets/
+drwxr-xr-x   0 ihos       (501) staff       (20)        0 2023-05-18 10:54:47.902629 cysecuretools-4.2.0/cysecuretools/targets/cyw20829_a0/packets/apps/
+drwxr-xr-x   0 ihos       (501) staff       (20)        0 2023-05-18 10:54:49.456379 cysecuretools-4.2.0/cysecuretools/targets/cyw20829_a0/packets/apps/prov_oem/
+-rw-r--r--   0 ihos       (501) staff       (20)      235 2023-05-18 10:29:21.000000 cysecuretools-4.2.0/cysecuretools/targets/cyw20829_a0/packets/apps/prov_oem/config.json
+-rwxr-xr-x   0 ihos       (501) staff       (20)     7812 2023-05-18 10:29:21.000000 cysecuretools-4.2.0/cysecuretools/targets/cyw20829_a0/packets/apps/prov_oem/cyapp_prov_oem_signed_icv0.bin
+-rwxr-xr-x   0 ihos       (501) staff       (20)      375 2023-05-18 10:29:21.000000 cysecuretools-4.2.0/cysecuretools/targets/cyw20829_a0/packets/apps/prov_oem/info.txt
+drwxr-xr-x   0 ihos       (501) staff       (20)        0 2023-05-18 10:54:49.466198 cysecuretools-4.2.0/cysecuretools/targets/cyw20829_a0/packets/apps/reprovisioning/
+-rw-r--r--   0 ihos       (501) staff       (20)      241 2023-05-18 10:29:21.000000 cysecuretools-4.2.0/cysecuretools/targets/cyw20829_a0/packets/apps/reprovisioning/config.json
+-rwxr-xr-x   0 ihos       (501) staff       (20)    28836 2023-05-18 10:29:21.000000 cysecuretools-4.2.0/cysecuretools/targets/cyw20829_a0/packets/apps/reprovisioning/cyapp_reprovisioning_signed_icv0.bin
+-rwxr-xr-x   0 ihos       (501) staff       (20)      264 2023-05-18 10:29:21.000000 cysecuretools-4.2.0/cysecuretools/targets/cyw20829_a0/packets/apps/reprovisioning/info.txt
+drwxr-xr-x   0 ihos       (501) staff       (20)        0 2023-05-18 10:54:49.476534 cysecuretools-4.2.0/cysecuretools/targets/cyw20829_a0/packets/apps/to_rma/
+-rw-r--r--   0 ihos       (501) staff       (20)      269 2023-05-18 10:29:21.000000 cysecuretools-4.2.0/cysecuretools/targets/cyw20829_a0/packets/apps/to_rma/config.json
+-rwxr-xr-x   0 ihos       (501) staff       (20)    28612 2023-05-18 10:29:21.000000 cysecuretools-4.2.0/cysecuretools/targets/cyw20829_a0/packets/apps/to_rma/cyapp_to_rma_signed_icv0.bin
+-rwxr-xr-x   0 ihos       (501) staff       (20)      289 2023-05-18 10:29:21.000000 cysecuretools-4.2.0/cysecuretools/targets/cyw20829_a0/packets/apps/to_rma/info.txt
+-rw-r--r--   0 ihos       (501) staff       (20)      624 2023-05-18 10:29:21.000000 cysecuretools-4.2.0/cysecuretools/targets/cyw20829_a0/packets/debug_cert.json
+-rw-r--r--   0 ihos       (501) staff       (20)      168 2023-05-18 10:29:21.000000 cysecuretools-4.2.0/cysecuretools/targets/cyw20829_a0/packets/rsa_key_tmpl.json
+drwxr-xr-x   0 ihos       (501) staff       (20)        0 2023-05-18 10:54:49.494492 cysecuretools-4.2.0/cysecuretools/targets/cyw20829_a0/policy/
+-rw-r--r--   0 ihos       (501) staff       (20)     6135 2023-05-18 10:29:21.000000 cysecuretools-4.2.0/cysecuretools/targets/cyw20829_a0/policy/policy_hci_secure.json
+-rw-r--r--   0 ihos       (501) staff       (20)     6344 2023-05-18 10:29:21.000000 cysecuretools-4.2.0/cysecuretools/targets/cyw20829_a0/policy/policy_no_secure.json
+-rw-r--r--   0 ihos       (501) staff       (20)      374 2023-05-18 10:29:21.000000 cysecuretools-4.2.0/cysecuretools/targets/cyw20829_a0/policy/policy_reprovisioning_no_secure.json
+-rw-r--r--   0 ihos       (501) staff       (20)     1812 2023-05-18 10:29:21.000000 cysecuretools-4.2.0/cysecuretools/targets/cyw20829_a0/policy/policy_reprovisioning_secure.json
+-rw-r--r--   0 ihos       (501) staff       (20)     8281 2023-05-18 10:29:21.000000 cysecuretools-4.2.0/cysecuretools/targets/cyw20829_a0/policy/policy_secure.json
+-rw-r--r--   0 ihos       (501) staff       (20)     1185 2023-05-18 10:29:21.000000 cysecuretools-4.2.0/cysecuretools/targets/cyw20829_a0/target_builder.py
+-rw-r--r--   0 ihos       (501) staff       (20)      613 2023-05-18 10:29:21.000000 cysecuretools-4.2.0/cysecuretools/version.py
+drwxr-xr-x   0 ihos       (501) staff       (20)        0 2023-05-18 10:54:47.982369 cysecuretools-4.2.0/cysecuretools.egg-info/
+-rw-r--r--   0 ihos       (501) staff       (20)    10995 2023-05-18 10:54:47.000000 cysecuretools-4.2.0/cysecuretools.egg-info/PKG-INFO
+-rw-r--r--   0 ihos       (501) staff       (20)    17340 2023-05-18 10:54:47.000000 cysecuretools-4.2.0/cysecuretools.egg-info/SOURCES.txt
+-rw-r--r--   0 ihos       (501) staff       (20)        1 2023-05-18 10:54:47.000000 cysecuretools-4.2.0/cysecuretools.egg-info/dependency_links.txt
+-rw-r--r--   0 ihos       (501) staff       (20)       63 2023-05-18 10:54:47.000000 cysecuretools-4.2.0/cysecuretools.egg-info/entry_points.txt
+-rw-r--r--   0 ihos       (501) staff       (20)      156 2023-05-18 10:54:47.000000 cysecuretools-4.2.0/cysecuretools.egg-info/requires.txt
+-rw-r--r--   0 ihos       (501) staff       (20)       14 2023-05-18 10:54:47.000000 cysecuretools-4.2.0/cysecuretools.egg-info/top_level.txt
+drwxr-xr-x   0 ihos       (501) staff       (20)        0 2023-05-18 10:54:49.509165 cysecuretools-4.2.0/docs/
+-rw-r--r--   0 ihos       (501) staff       (20)    40778 2023-05-18 10:29:21.000000 cysecuretools-4.2.0/docs/README_CYW20829.md
+-rw-r--r--   0 ihos       (501) staff       (20)    40021 2023-05-18 10:29:21.000000 cysecuretools-4.2.0/docs/README_PSOC64.md
+-rw-r--r--   0 ihos       (501) staff       (20)      141 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/pyproject.toml
+-rw-r--r--   0 ihos       (501) staff       (20)       38 2023-05-18 10:54:49.511077 cysecuretools-4.2.0/setup.cfg
+-rw-r--r--   0 ihos       (501) staff       (20)     2441 2023-05-18 10:29:21.000000 cysecuretools-4.2.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `cysecuretools-4.1.0/LICENSE` & `cysecuretools-4.2.0/LICENSE`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-Copyright (c) 2019-2020 Cypress Semiconductor Corporation
+Copyright (c) 2019-2023 Cypress Semiconductor Corporation
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `cysecuretools-4.1.0/MANIFEST.in` & `cysecuretools-4.2.0/MANIFEST.in`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,10 @@
 include README.md
+include CHANGELOG.md
+include docs/*
 include cysecuretools/execute/programmer/pyocd_target_map.json
 include cysecuretools/execute/programmer/openocd_target_map.json
 include cysecuretools/settings.json
 recursive-include cysecuretools/targets *
 recursive-include cysecuretools/data *
 global-exclude .DS_Store
 global-exclude *policy_single_stage_CM4*.json
```

### Comparing `cysecuretools-4.1.0/cysecuretools/__init__.py` & `cysecuretools-4.2.0/cysecuretools/__init__.py`

 * *Files identical despite different names*

### Comparing `cysecuretools-4.1.0/cysecuretools/__main__.py` & `cysecuretools-4.2.0/cysecuretools/__main__.py`

 * *Files identical despite different names*

### Comparing `cysecuretools-4.1.0/cysecuretools/cli.py` & `cysecuretools-4.2.0/cysecuretools/cli.py`

 * *Files 5% similar despite different names*

```diff
@@ -40,27 +40,28 @@
                 or ('bin2hex' in sys.argv))
 
 
 @click.group(chain=True)
 @click.pass_context
 @click.option('-t', '--target', type=click.STRING, required=require_target(),
               help='Device name or family')
+@click.option('--rev', help='Device revision')
 @click.option('-p', '--policy', type=click.File(), required=False,
               help='Provisioning policy file')
 @click.option('-v', '--verbose', is_flag=True, help='Provides debug-level log')
 @click.option('-q', '--quiet', is_flag=True, help='Quiet display option')
 @click.option('--logfile-off', is_flag=True, help='Avoids logging into file')
 @click.option('--no-interactive-mode', is_flag=True, hidden=True,
               help='Skips user interactive prompts')
 @click.option('--skip-validation', is_flag=True, hidden=True,
               help='Skips policy validation')
-def main(ctx, target, policy, verbose, quiet,
+def main(ctx, target, rev, policy, verbose, quiet,
          logfile_off, no_interactive_mode, skip_validation):
     """
-    Common options (e.g. -t, -p, -v, -q) are common for all commands and must
+    Common options (e.g. -t, --rev, -p, -v, -q) are common for all commands and must
     precede them:
 
     \b
     cysecuretools -t <TARGET> -p <POLICY> <COMMAND> --<COMMAND_OPTION>
 
     \b
     For detailed help for command use:
@@ -77,33 +78,49 @@
         LoggingConfigurator.set_logger_level(logging.DEBUG)
     ctx.ensure_object(dict)
     log_file = not logfile_off
 
     if require_target():
         if 'init' in sys.argv:
             validate_init_cmd_args()
-            policy_path = default_policy(target)
+            try:
+                policy_path = default_policy(target, rev=rev)
+            except ValueError as e:
+                logger.error(e)
+                sys.exit(2)
             log_file = False
         else:
             policy_path = policy.name if policy else None
-        ctx.obj['TOOL'] = CySecureTools(target, policy_path, log_file,
-                                        no_interactive_mode,
-                                        skip_validation)
+        try:
+            ctx.obj['TOOL'] = CySecureTools(target, policy_path, log_file,
+                                            no_interactive_mode,
+                                            skip_validation, rev=rev)
+        except ValueError as e:
+            logger.error(e)
+            sys.exit(2)
     else:
         if 'version' in sys.argv:
             if '--target' in sys.argv or '-t' in sys.argv:
-                ctx.obj['TOOL'] = CySecureTools(
-                    target, policy.name if policy else None,
-                    log_file=log_file, skip_prompts=no_interactive_mode,
-                    skip_validation=skip_validation)
+                try:
+                    ctx.obj['TOOL'] = CySecureTools(
+                        target, policy.name if policy else None,
+                        log_file=log_file, skip_prompts=no_interactive_mode,
+                        skip_validation=skip_validation, rev=rev)
+                except ValueError as e:
+                    logger.error(e)
+                    sys.exit(2)
         else:
-            ctx.obj['TOOL'] = CySecureTools(
-                target, policy.name if policy else None,
-                log_file=log_file, skip_prompts=no_interactive_mode,
-                skip_validation=skip_validation)
+            try:
+                ctx.obj['TOOL'] = CySecureTools(
+                    target, policy.name if policy else None, log_file=log_file,
+                    skip_prompts=no_interactive_mode,
+                    skip_validation=skip_validation, rev=rev)
+            except ValueError as e:
+                logger.error(e)
+                sys.exit(2)
     logger.debug(sys.argv)
 
 
 @main.result_callback()
 def process_pipeline(processors, **_):
     for func in processors:
         res = func()
@@ -273,18 +290,18 @@
     stack_trace = stack_trace.rstrip('\n')
     logger.debug(stack_trace)
     filename, line, _, text = tb_info[-1]
     logger.error("An error occurred in file '%s' on line %d in statement %s",
                  filename, line, text)
 
 
-def default_policy(target_name):
+def default_policy(target_name, rev=None):
     director = TargetDirector()
     target_name = target_name.lower()
-    get_target_builder(director, target_name)
+    get_target_builder(director, target_name, rev=rev)
     target = director.get_target(None, target_name, None)
     return target.policy
 
 
 def validate_init_cmd_args():
     if '--policy' in sys.argv:
         sys.stderr.write('Error: invalid argument used with "init" '
```

### Comparing `cysecuretools-4.1.0/cysecuretools/cli_creator.py` & `cysecuretools-4.2.0/cysecuretools/cli_creator.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 import os
 import sys
 import click
 
-from cysecuretools.targets import target_map
+from cysecuretools.targets import target_data
 from cysecuretools import cli as base_cli
 
 
 class CliCreator:
     @staticmethod
     def create():
         is_help = '--help' in sys.argv[1:]
@@ -126,19 +126,20 @@
         args = sys.argv[1:]
         try:
             return [args[i + 1] for i in range(len(args)) if args[i] in opt][0]
         except IndexError:
             return None
 
     @staticmethod
-    def _get_platform(target):
+    def _get_platform(target_name):
         platform = None
-        if target is not None:
+        if target_name is not None:
             try:
-                platform = target_map[target.lower()].get('platform')
+                target = target_data(target_name.lower())
+                platform = target.get('platform')
             except KeyError:
                 platform = None
         return platform
 
     @staticmethod
     def _command_list(obj):
         if isinstance(obj, click.Group):
```

### Comparing `cysecuretools-4.1.0/cysecuretools/cli_mxs40sv2.py` & `cysecuretools-4.2.0/cysecuretools/cli_mxs40sv2.py`

 * *Files 2% similar despite different names*

```diff
@@ -118,27 +118,25 @@
 
     return process
 
 
 @main.command('version', short_help='Show BootROM version')
 @click.option('--probe-id', 'probe_id', type=click.STRING, default=None,
               help='Probe serial number')
-@click.option('--ap', hidden=True, type=click.Choice(['cm33', 'sysap']),
-              default='sysap', help='The access port used to read the data')
 @click.option('--testapps', is_flag=True, hidden=True)
 @click.option('--testapps-si', is_flag=True, hidden=True)
 @click.pass_context
-def cmd_version(ctx, probe_id, ap, testapps, testapps_si):
+def cmd_version(ctx, probe_id, testapps, testapps_si):
     @process_handler()
     def process():
         if 'TOOL' not in ctx.obj:
             return False
         validate_testapps_args(testapps, testapps_si)
         ctx.obj['TOOL'].print_version(
-            probe_id, ap, testapps=test_pkg_type(testapps, testapps_si))
+            probe_id, testapps=test_pkg_type(testapps, testapps_si))
         return True
 
     return process
 
 
 @main.command('create-provisioning-packet',
               help='Creates binary packet for device provisioning')
@@ -234,21 +232,19 @@
 
 
 @main.command('provision-device', help='Executes device provisioning')
 @click.option('--probe-id', 'probe_id', type=click.STRING, default=None,
               help='Probe serial number')
 @click.option('--existing-packet', is_flag=True,
               help='Skip provisioning packet creation and use existing')
-@click.option('--ap', hidden=True, type=click.Choice(['cm33', 'sysap']),
-              default='sysap', help='The access port used for provisioning')
 @click.option('--testapps', is_flag=True, hidden=True)
 @click.option('--testapps-si', is_flag=True, hidden=True)
 @click.pass_context
 def cmd_provision_device(
-        ctx, probe_id, existing_packet, ap, testapps, testapps_si):
+        ctx, probe_id, existing_packet, testapps, testapps_si):
     @process_handler()
     def process():
         if 'TOOL' not in ctx.obj:
             return False
         validate_testapps_args(testapps, testapps_si)
         if existing_packet:
             result = True
@@ -258,15 +254,15 @@
                 logger.error('Reprovisioning policy type specified for '
                              'the provisioning operation')
                 return False
             result = ctx.obj['TOOL'].create_provisioning_packet(
                 testapps=test_pkg_type(testapps, testapps_si))
         if result:
             result = ctx.obj['TOOL'].provision_device(
-                probe_id, ap, testapps=test_pkg_type(testapps, testapps_si))
+                probe_id, 'sysap', testapps=test_pkg_type(testapps, testapps_si))
         return result
 
     return process
 
 
 @main.command('reprovision-device', help='Executes device reprovisioning')
 @click.option('-k', '--key-id', type=click.Choice(['0', '1']),
@@ -276,21 +272,19 @@
                    'Overrides --key-id option')
 @click.option('--signature', type=click.Path(),
               help='The name of the file containing the signature')
 @click.option('--probe-id', type=click.STRING, required=False, default=None,
               help='Probe serial number')
 @click.option('--existing-packet', is_flag=True,
               help='Skip reprovisioning packet creation and use the existing')
-@click.option('--ap', hidden=True, type=click.Choice(['cm33', 'sysap']),
-              default='sysap', help='The access port used for re-provisioning')
 @click.option('--testapps', is_flag=True, hidden=True)
 @click.option('--testapps-si', is_flag=True, hidden=True)
 @click.pass_context
 def cmd_re_provision_device(ctx, key_id, key_path, signature, probe_id,
-                            existing_packet, ap, testapps, testapps_si):
+                            existing_packet, testapps, testapps_si):
     @process_handler()
     def process():
         if 'TOOL' not in ctx.obj:
             return False
 
         validate_policy_type()
         validate_args()
@@ -300,15 +294,15 @@
             result = ctx.obj['TOOL'].create_provisioning_packet(
                 key_id=None if key_path or key_id is None else int(key_id),
                 key_path=key_path, signature=signature,
                 testapps=test_pkg_type(testapps, testapps_si))
 
         if result:
             result = ctx.obj['TOOL'].re_provision_device(
-                probe_id, ap, testapps=test_pkg_type(testapps, testapps_si))
+                probe_id, testapps=test_pkg_type(testapps, testapps_si))
         return result
 
     def validate_args():
         error = None
         from .targets.common.mxs40sv2.enums import PolicyType
         policy_type = ctx.obj['TOOL'].policy_parser.get_policy_type()
 
@@ -346,27 +340,25 @@
 
 @main.command('device-info',
               help='Reads device information - silicon ID, family ID, silicon '
                    'revision',
               short_help='Reads device information - silicon ID, family ID, '
                          'silicon revision')
 @click.option('--probe-id', default=None, help='Probe serial number')
-@click.option('--ap', type=click.Choice(['cm33', 'sysap']),
-              default='sysap', help='The access port used to read the data')
 @click.pass_context
-def cmd_device_info(ctx, probe_id, ap):
+def cmd_device_info(ctx, probe_id):
     @process_handler()
     def process():
         if 'TOOL' not in ctx.obj:
             return False
         status = True
         ConnectHelper.do_not_disconnect = True
-        dev_info = ctx.obj['TOOL'].get_device_info(probe_id, ap)
+        dev_info = ctx.obj['TOOL'].get_device_info(probe_id)
         ConnectHelper.do_not_disconnect = False
-        lifecycle = ctx.obj['TOOL'].get_device_lifecycle(probe_id, ap)
+        lifecycle = ctx.obj['TOOL'].get_device_lifecycle(probe_id)
 
         logger.info('*' * 39)
         if dev_info:
             logger.info(
                 'Silicon: 0x%x, Family: 0x%0x, Rev.: 0x%0x',
                 dev_info.silicon_id, dev_info.family_id, dev_info.silicon_rev)
         else:
@@ -434,20 +426,21 @@
 @click.option('--align', type=click.Choice(['1', '2', '4', '8']), default='8',
               help='Flash alignment')
 @click.option('-v', '--version',
               help='Sets image version in the image header')
 @click.option('-d', '--dependencies', callback=get_dependencies,
               required=False, help='''Add dependence on another image, format:
               "(<image_ID>,<image_version>), ... "''')
+@click.option('--image-id', type=click.INT, help='Image ID', default=0)
 @click.pass_context
 def cmd_sign_image(ctx, image, erased_val, key_id, key_path, image_config,
                    output, signature, header_size, slot_size, encrypt, enckey,
                    app_addr, hex_addr, update_key_id, update_key_path,
-                   image_format, pad, confirm, overwrite_only, min_erase_size, align,
-                   version, dependencies):
+                   image_format, pad, confirm, overwrite_only, min_erase_size,
+                   align, version, dependencies, image_id):
     @process_handler()
     def process():
         if 'TOOL' not in ctx.obj:
             return False
         if signature:
             with open(signature, 'rb') as f:
                 s = binascii.hexlify(f.read()).decode(sys.stdout.encoding)
@@ -477,15 +470,16 @@
                 image_format=image_format,
                 pad=pad,
                 confirm=confirm,
                 overwrite_only=overwrite_only,
                 min_erase_size=min_erase_size,
                 align=align,
                 version=version,
-                dependencies=dependencies
+                dependencies=dependencies,
+                image_id=image_id
                 )
         return result is not None
 
     def validate_key_args():
         if key_id is None and key_path is None:
             sys.stderr.write("Either '--key-id' or '--key-path' option must "
                              "be specified.\n")
@@ -541,19 +535,20 @@
 @click.option('--align', type=click.Choice(['1', '2', '4', '8']), default='8',
               help='Flash alignment')
 @click.option('--update-key-id', type=click.Choice(['0', '1']),
               help='OEM private key ID used to sign the update data packet')
 @click.option('--update-key-path', type=click.Path(),
               help='The key used to sign the update data packet. Overrides '
                    'the --update-key-id option')
+@click.option('--image-id', type=click.INT, help='Image ID', default=0)
 @click.pass_context
 def cmd_extend_image(ctx, image, pubkey, erased_val, image_config, output,
                      protected_tlv, header_size, slot_size, hex_addr,
                      image_format, pad, confirm, overwrite_only, align,
-                     update_key_id, update_key_path):
+                     update_key_id, update_key_path, image_id):
     @process_handler()
     def process():
         if 'TOOL' not in ctx.obj:
             return False
         validate_args()
         result = ctx.obj['TOOL'].extend_image(
             image, pubkey=pubkey, erased_val=erased_val,
@@ -562,15 +557,15 @@
             header_size=header_size, skip_tlv_info=True,
             hex_addr=hex_addr, image_format=image_format, pad=pad,
             confirm=confirm, overwrite_only=overwrite_only,
             align=align,
             update_key_id=
             None if update_key_path or update_key_id is None else int(
                 update_key_id),
-            update_key_path=update_key_path
+            update_key_path=update_key_path, image_id=image_id
         )
         return result is not None
 
     def validate_args():
         if image_format == 'bootrom_next_app' and not pubkey:
             sys.stderr.write("Error: Missing option '--pubkey'.\n")
             sys.exit(2)
@@ -601,23 +596,21 @@
 
 
 @main.command('load-and-run-app', hidden=True,
               help='Loads and runs RAM application')
 @click.option('-c', '--config', type=click.Path(), required=True,
               help='Path to the application configuration file')
 @click.option('--probe-id', default=None, help='Probe serial number')
-@click.option('--ap', type=click.Choice(['cm33', 'sysap']),
-              default='sysap', help='The access port used to load application')
 @click.pass_context
-def cmd_load_and_run_app(ctx, config, probe_id, ap):
+def cmd_load_and_run_app(ctx, config, probe_id):
     @process_handler(None)
     def process():
         if 'TOOL' not in ctx.obj:
             return False
-        return ctx.obj['TOOL'].load_and_run_app(config, probe_id, ap)
+        return ctx.obj['TOOL'].load_and_run_app(config, probe_id)
 
     return process
 
 
 @main.command('debug-certificate',
               help='Creates debug or RMA certificate binary based on template',
               short_help='Creates debug or RMA certificate binary based on '
@@ -687,23 +680,21 @@
 
 
 @main.command('read-die-id', help='Reads die ID from device')
 @click.option('-o', '--out-file', default=None,
               help='Filename where to save die ID')
 @click.option('--probe-id', default=None,
               help='Probe serial number')
-@click.option('--ap', hidden=True, type=click.Choice(['cm33', 'sysap']),
-              default='sysap', help='The access port used to read the data')
 @click.pass_context
-def cmd_read_die_id(ctx, out_file, probe_id, ap):
+def cmd_read_die_id(ctx, out_file, probe_id):
     @process_handler()
     def process():
         if 'TOOL' not in ctx.obj:
             return False
-        data = ctx.obj['TOOL'].read_die_id(probe_id, ap)
+        data = ctx.obj['TOOL'].read_die_id(probe_id)
         if data:
             logger.info('die_id = %s', json.dumps(data, indent=4))
             if out_file:
                 with open(out_file, 'w', encoding='utf-8') as f:
                     json.dump(data, f, indent=4)
             return True
         return False
@@ -711,27 +702,25 @@
     return process
 
 
 @main.command('convert-to-rma', help='Converts device to RMA lifecycle stage')
 @click.option('-c', '--cert', type=click.Path(),
               help='Path to debug certificate')
 @click.option('--probe-id', default=None, help='Probe serial number')
-@click.option('--ap', hidden=True, type=click.Choice(['cm33', 'sysap']),
-              default='sysap', help='The access port used to read the data')
 @click.option('--testapps', is_flag=True, hidden=True)
 @click.option('--testapps-si', is_flag=True, hidden=True)
 @click.pass_context
-def cmd_convert_to_rma(ctx, cert, probe_id, ap, testapps, testapps_si):
+def cmd_convert_to_rma(ctx, cert, probe_id, testapps, testapps_si):
     @process_handler()
     def process():
         if 'TOOL' not in ctx.obj:
             return False
         validate_testapps_args(testapps, testapps_si)
-        return ctx.obj['TOOL'].convert_to_rma(
-            cert=cert, probe_id=probe_id, ap=ap,
+        return ctx.obj['TOOL'].transit_to_rma(
+            cert=cert, probe_id=probe_id,
             testapps=test_pkg_type(testapps, testapps_si))
     return process
 
 
 def validate_update_key(update_key_id, update_key_path):
     if update_key_id is None and update_key_path is None:
         sys.stderr.write(
```

### Comparing `cysecuretools-4.1.0/cysecuretools/cli_mxs40v1.py` & `cysecuretools-4.2.0/cysecuretools/cli_mxs40v1.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 from json.decoder import JSONDecodeError
 from cryptography.hazmat.primitives import serialization
 from cysecuretools.execute.image_cert import ImageCertificate
 from cysecuretools.core.enums import KeyAlgorithm
 from cysecuretools.cli import main as main, process_handler
 
 logger = logging.getLogger(__name__)
+name = 'cli_mxs40v1'
 
 
 @main.command('create-keys', help='Creates keys specified in policy file')
 @click.option('--overwrite/--no-overwrite', 'overwrite', is_flag=True,
               default=None, required=False,
               help='Indicates whether overwrite keys in the output directory '
                    'if they already exist')
@@ -55,27 +56,22 @@
 
     return process
 
 
 @main.command('version',
               help='Show CyBootloader and Secure Flash Boot version',
               short_help='Show CyBootloader and Secure Flash Boot version')
-@click.option('--probe-id', 'probe_id', type=click.STRING, default=None,
-              help='Probe serial number')
-@click.option('--ap', hidden=True, type=click.Choice(['cm0', 'cm4', 'sysap']),
-              default='sysap',
-              help='The access port used to read CyBootloader and '
-                   'Secure Flash Boot version from device')
+@click.option('--probe-id', 'probe_id', help='Probe serial number')
 @click.pass_context
-def cmd_version(ctx, probe_id, ap):
+def cmd_version(ctx, probe_id):
     @process_handler()
     def process():
         if 'TOOL' not in ctx.obj:
             return False
-        ctx.obj['TOOL'].print_version(probe_id, ap)
+        ctx.obj['TOOL'].print_version(probe_id)
         return True
 
     return process
 
 
 @main.command('image-metadata',
               help='Adds metadata to a firmware image (header and TLVs)',
@@ -266,60 +262,56 @@
 
 
 @main.command('provision-device', help='Executes device provisioning')
 @click.option('--probe-id', 'probe_id', type=click.STRING, default=None,
               help='Probe serial number')
 @click.option('--existing-packet', 'use_existing_packet', is_flag=True,
               help='Skip provisioning packet creation and use existing one')
-@click.option('--ap', hidden=True, type=click.Choice(['cm0', 'cm4', 'sysap']),
-              default='cm4', help='The access port used for provisioning')
 @click.pass_context
-def cmd_provision_device(ctx, probe_id, use_existing_packet, ap):
+def cmd_provision_device(ctx, probe_id, use_existing_packet):
     @process_handler()
     def process():
         if 'TOOL' not in ctx.obj:
             return False
         if use_existing_packet:
             result = True
         else:
             result = ctx.obj['TOOL'].create_provisioning_packet()
         if result:
-            result = ctx.obj['TOOL'].provision_device(probe_id, ap)
+            result = ctx.obj['TOOL'].provision_device(probe_id)
         return result
 
     return process
 
 
 @main.command('re-provision-device', help='Executes device re-provisioning')
 @click.option('--probe-id', type=click.STRING, required=False, default=None,
               help='Probe serial number')
 @click.option('--existing-packet', is_flag=True,
               help='Skip provisioning packet creation and use existing one')
-@click.option('--ap', hidden=True, type=click.Choice(['cm0', 'cm4', 'sysap']),
-              default='sysap', help='The access port used for re-provisioning')
 @click.option('--erase-boot', is_flag=True,
               help='Indicates whether erase BOOT slot')
 @click.option('--control-dap-cert', default=None,
               help='The certificate that provides the access to control DAP')
 @click.option('--skip-bootloader', is_flag=True, hidden=True, default=False,
               help='Skips bootloader programming')
 @click.pass_context
-def cmd_re_provision_device(ctx, probe_id, existing_packet, ap, erase_boot,
+def cmd_re_provision_device(ctx, probe_id, existing_packet, erase_boot,
                             control_dap_cert, skip_bootloader):
     @process_handler()
     def process():
         if 'TOOL' not in ctx.obj:
             return False
         if existing_packet:
             result = True
         else:
             result = ctx.obj['TOOL'].create_provisioning_packet()
         if result:
             result = ctx.obj['TOOL'].re_provision_device(
-                probe_id, ap, erase_boot=erase_boot,
+                probe_id, erase_boot=erase_boot,
                 control_dap_cert=control_dap_cert,
                 skip_bootloader=skip_bootloader)
         return result
 
     return process
 
 
@@ -416,26 +408,24 @@
 @main.command('entrance-exam',
               help='Checks device life cycle, FlashBoot firmware '
                    'and Flash state',
               short_help='Checks device life cycle, FlashBoot firmware '
                          'and Flash state')
 @click.option('--probe-id', type=click.STRING, required=False, default=None,
               help='Probe serial number')
-@click.option('--ap', hidden=True, default='cm4',
-              type=click.Choice(['cm0', 'cm4', 'sysap']),
-              help='The access port used for the entrance exam')
 @click.option('--erase-flash', hidden=True, is_flag=True,
               help='Erase flash before the command execution')
 @click.pass_context
-def cmd_entrance_exam(ctx, probe_id, ap, erase_flash):
+def cmd_entrance_exam(ctx, probe_id, erase_flash):
     @process_handler()
     def process():
         if 'TOOL' not in ctx.obj:
             return False
-        return ctx.obj['TOOL'].entrance_exam(probe_id, ap, erase_flash)
+        return ctx.obj['TOOL'].entrance_exam(probe_id=probe_id,
+                                             erase_flash=erase_flash)
 
     return process
 
 
 @main.command('encrypt-image',
               help='Creates encrypted image for encrypted programming',
               short_help='Creates encrypted image for encrypted programming')
@@ -565,69 +555,63 @@
 
 
 @main.command('read-die-id', help='Reads die ID from device')
 @click.option('-o', '--out-file', default=None,
               help='Filename where to save die ID')
 @click.option('--probe-id', default=None,
               help='Probe serial number')
-@click.option('--ap', hidden=True, type=click.Choice(['cm0', 'cm4', 'sysap']),
-              default='sysap', help='The access port used to read the data')
 @click.pass_context
-def cmd_read_die_id(ctx, out_file, probe_id, ap):
+def cmd_read_die_id(ctx, out_file, probe_id):
     @process_handler()
     def process():
         if 'TOOL' not in ctx.obj:
             return False
-        data = ctx.obj['TOOL'].read_die_id(probe_id, ap)
+        data = ctx.obj['TOOL'].read_die_id(probe_id)
         if data:
             logger.info('die_id = %s', json.dumps(data, indent=4))
             if out_file:
                 with open(out_file, 'w', encoding='utf-8') as f:
                     json.dump(data, f, indent=4)
             return True
         else:
             return False
 
     return process
 
 
 @main.command('sign-cert', help='Signs JSON certificate with the private key')
-@click.option('-j', '--json-file', type=click.File('r'), required=True,
-              help='JSON file to be signed')
+@click.option('-j', '--json-file', '--template', 'template', type=click.Path(),
+              required=True, help='Certificate template')
 @click.option('-k', '--key-id', type=click.INT, required=True,
               help='Private Key ID to sign the certificate with '
                    '(1 - DEVICE, 4 - HSM, 5 - OEM, 12 - GROUP')
-@click.option('-o', '--out-file', default=None,
+@click.option('-o', '--out-file', '--output', 'output', type=click.Path(),
               help='Filename where to save the JWT. If not specified, the '
                    'input file name with "jwt" extension will be used')
 @click.pass_context
-def cmd_sign_cert(ctx, json_file, key_id, out_file):
+def cmd_sign_cert(ctx, template, key_id, output):
     @process_handler()
     def process():
         if 'TOOL' not in ctx.obj:
             return False
-        token = ctx.obj['TOOL'].sign_json(json_file.name, key_id, out_file)
+        token = ctx.obj['TOOL'].sign_json(template, key_id, output)
         return True if token else False
 
     return process
 
 
-@main.command('device-info', hidden=True,
-              help='Gets device information')
-@click.option('--probe-id', default=None,
-              help='Probe serial number')
-@click.option('--ap', type=click.Choice(['cm0', 'cm4', 'sysap']),
-              default='sysap', help='The access port used to read the data')
+@main.command('device-info', help='Reads silicon ID, family, and revision')
+@click.option('--probe-id', default=None, help='Probe serial number')
 @click.pass_context
-def cmd_device_info(ctx, probe_id, ap):
+def cmd_device_info(ctx, probe_id):
     @process_handler()
     def process():
         if 'TOOL' not in ctx.obj:
             return
-        dev_info = ctx.obj['TOOL'].get_device_info(probe_id, ap)
+        dev_info = ctx.obj['TOOL'].get_device_info(probe_id)
         if dev_info:
             logger.info(
                 'Silicon: 0x%x, Family: 0x%0x, Rev.: 0x%0x',
                 dev_info.silicon_id, dev_info.family_id, dev_info.silicon_rev)
         return True
 
     return process
@@ -640,7 +624,42 @@
     def process():
         if 'TOOL' not in ctx.obj:
             return False
         ctx.obj['TOOL'].init()
         return True
 
     return process
+
+
+@main.command('transit-to-rma',
+              help='Transition device to RMA lifecycle stage')
+@click.option('-c', '--cert', type=click.Path(), required=True,
+              help='Path to debug certificate')
+@click.option('--probe-id', default=None, help='Probe serial number')
+@click.pass_context
+def cmd_transit_to_rma(ctx, cert, probe_id):
+    """Transits device to RMA LCS"""
+    @process_handler()
+    def process():
+        if 'TOOL' not in ctx.obj:
+            return False
+        return ctx.obj['TOOL'].transit_to_rma(probe_id=probe_id, cert=cert)
+
+    return process
+
+
+@main.command('open-rma',
+              help='Enables full access to device in RMA lifecycle stage',
+              short_help='Enables full access to device in RMA lifecycle stage')
+@click.option('-c', '--cert', type=click.Path(), required=True,
+              help='Path to debug certificate')
+@click.option('--probe-id', default=None, help='Probe serial number')
+@click.pass_context
+def cmd_open_rma(ctx, cert, probe_id):
+    """Enables full access to device in RMA LCS"""
+    @process_handler()
+    def process():
+        if 'TOOL' not in ctx.obj:
+            return False
+        return ctx.obj['TOOL'].open_rma(cert, probe_id=probe_id)
+
+    return process
```

### Comparing `cysecuretools-4.1.0/cysecuretools/core/__init__.py` & `cysecuretools-4.2.0/cysecuretools/core/__init__.py`

 * *Files identical despite different names*

### Comparing `cysecuretools-4.1.0/cysecuretools/core/bitops.py` & `cysecuretools-4.2.0/cysecuretools/core/bitops.py`

 * *Files identical despite different names*

### Comparing `cysecuretools-4.1.0/cysecuretools/core/certificates/x509.py` & `cysecuretools-4.2.0/cysecuretools/core/certificates/x509.py`

 * *Files 2% similar despite different names*

```diff
@@ -175,16 +175,18 @@
         :param target: Target object
         :param probe_id: Probe ID. Need to be used if more than one
                device is connected to the computer.
         :return: Dictionary with the certificate fields.
         """
         # Read silicon data
         if ConnectHelper.connect(tool, target, probe_id=probe_id, ap='sysap'):
+            if not target.version_provider.check_compatibility(tool):
+                ConnectHelper.disconnect(tool)
+                return None
             target.version_provider.log_version(tool)
-            target.version_provider.verify_fw_version(tool)
             data = read_silicon_data(tool, target)
             if data is None:
                 logger.error('Failed to read silicon data')
                 return None
 
             dev_pub_key = target.key_reader.read_public_key(tool, KeyId.DEVICE)
             ConnectHelper.disconnect(tool)
```

### Comparing `cysecuretools-4.1.0/cysecuretools/core/connect_helper.py` & `cysecuretools-4.2.0/cysecuretools/core/connect_helper.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """
-Copyright (c) 2021 Cypress Semiconductor Corporation
+Copyright 2021-2023 Cypress Semiconductor Corporation (an Infineon company)
+or an affiliate of Cypress Semiconductor Corporation. All rights reserved.
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
 
@@ -13,78 +14,80 @@
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 import os
 import sys
 import logging
 
+from .mtb_tools_discovery import mtb_openocd_dir
 from .target_director import Target
 from ..execute.programmer.base import ProgrammerBase
 
 logger = logging.getLogger(__name__)
 
 
 class ConnectHelper:
     """ Helper class for connection creation process """
 
     connected = False
     do_not_disconnect = False
 
     @staticmethod
     def connect(tool: ProgrammerBase, target: Target,
-                probe_id=None, ap=None, acquire=True, blocking=True,
-                suppress_errors=False, reset_and_halt=False,
-                power=None, voltage=None) -> bool:
+                probe_id=None, ap='sysap', acquire=True, blocking=True,
+                ignore_errors=False, power=None, voltage=None) -> bool:
         """ Checks for target/OCD compatibility and creates a connection """
 
         if tool.name not in target.ocds:
             logger.error("Target '%s' is not supported by the selected "
                          "on-chip debugger '%s'", target.name, tool.name)
             ConnectHelper._print_ocd_info(tool, target)
             ConnectHelper._print_example()
             raise ValueError('Incompatible target and on-chip debugger')
 
         if tool.require_path:
             if not tool.tool_path:
-                logger.error("Path to '%s' not specified", tool.name)
-                ConnectHelper._print_example()
-                raise ValueError('Invalid on-chip debugger path')
-            elif not os.path.exists(tool.tool_path):
+                tool.tool_path = ConnectHelper.discover_tool(tool.name)
+                if not tool.tool_path:
+                    logger.error("Path to '%s' not specified", tool.name)
+                    ConnectHelper._print_example()
+                    raise ValueError('Invalid on-chip debugger path')
+            if not os.path.exists(tool.tool_path):
                 logger.error(
                     "Path to '%s' not found (%s)", tool.name, tool.tool_path)
                 ConnectHelper._print_example()
                 raise ValueError('Invalid on-chip debugger path')
 
         if not ConnectHelper.connected:
+            if tool.require_path and tool.tool_path:
+                logger.info("On-Chip debugger path is '%s'", tool.tool_path)
             ConnectHelper.connected = tool.connect(
                 target.name, probe_id=probe_id, ap=ap, acquire=acquire,
-                blocking=blocking, reset_and_halt=reset_and_halt,
-                power=power, voltage=voltage)
+                blocking=blocking, power=power, voltage=voltage,
+                ignore_errors=ignore_errors)
 
         if not ConnectHelper.connected:
-            if tool.name == 'openocd' and not suppress_errors:
+            if tool.name == 'openocd' and not ignore_errors:
                 logger.error('OpenOCD server has not started')
         return ConnectHelper.connected
 
     @staticmethod
-    def power_on(tool: ProgrammerBase, target: Target,
-                 voltage):
+    def power_on(tool: ProgrammerBase, target: Target, voltage):
         if tool.name != 'openocd':
             logger.error("Incompatible command and on-chip debugger")
             return False
         logger.warning('ATTENTION! To avoid device destruction, make sure the '
                        'external power is not connected. Continue? (y/n): ')
         confirm = input()
         if confirm.lower() == 'y':
             if voltage is None:
                 voltage = 2500
                 logger.warning('Voltage is not specified. Default voltage '
                                f'level will be used ({voltage} mV).')
-            if ConnectHelper.connect(tool, target, power='on',
-                                     voltage=voltage):
+            if ConnectHelper.connect(tool, target, power='on', voltage=voltage):
                 logger.info('Power on command sent')
                 return True
         else:
             return True
         return False
 
     @staticmethod
@@ -100,14 +103,21 @@
     @staticmethod
     def disconnect(tool: ProgrammerBase):
         if ConnectHelper.connected and not ConnectHelper.do_not_disconnect:
             tool.disconnect()
             ConnectHelper.connected = False
 
     @staticmethod
+    def discover_tool(tool_name):
+        """Autodiscovery of the OCD path"""
+        if tool_name == 'openocd':
+            return mtb_openocd_dir()
+        return None
+
+    @staticmethod
     def _print_ocd_info(tool, target):
         print(f'The currently selected on-chip debugger: {tool.name}.')
         print(f"The supported on-chip debugger(s) for the '{target.name}' "
               f'target: {",".join(target.ocds)}.')
 
     @staticmethod
     def _print_example():
```

### Comparing `cysecuretools-4.1.0/cysecuretools/core/cy_bootloader_map_parser.py` & `cysecuretools-4.2.0/cysecuretools/core/cy_bootloader_map_parser.py`

 * *Files identical despite different names*

### Comparing `cysecuretools-4.1.0/cysecuretools/core/dependecy_validator.py` & `cysecuretools-4.2.0/cysecuretools/core/dependecy_validator.py`

 * *Files identical despite different names*

### Comparing `cysecuretools-4.1.0/cysecuretools/core/entrance_exam_base.py` & `cysecuretools-4.2.0/cysecuretools/core/entrance_exam_base.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 
 class EntranceExam(ABC):
     @abstractmethod
     def __init__(self, target, **kwargs):
         pass
 
     @abstractmethod
-    def execute(self, tool):
+    def execute(self, tool, **kwargs):
         pass
 
     @abstractmethod
     def read_sfb_version(self, tool):
         pass
 
     @abstractmethod
```

### Comparing `cysecuretools-4.1.0/cysecuretools/core/enums.py` & `cysecuretools-4.2.0/cysecuretools/core/enums.py`

 * *Files identical despite different names*

### Comparing `cysecuretools-4.1.0/cysecuretools/core/exceptions.py` & `cysecuretools-4.2.0/cysecuretools/core/exceptions.py`

 * *Files identical despite different names*

### Comparing `cysecuretools-4.1.0/cysecuretools/core/json_helper.py` & `cysecuretools-4.2.0/cysecuretools/core/json_helper.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """
-Copyright (c) 2020-2021 Cypress Semiconductor Corporation
+Copyright 2020-2022 Cypress Semiconductor Corporation (an Infineon company)
+or an affiliate of Cypress Semiconductor Corporation. All rights reserved.
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
 
@@ -31,12 +32,12 @@
         json.dump(data, f, indent=4)
 
 
 def replace(datadict, lookup_key, value):
     """ Sets value to all fields with the specified name """
     replaced_dict = deepcopy(datadict)
     for k, v in datadict.items():
-        if isinstance(v, (dict, list)):
+        if isinstance(v, dict):
             replaced_dict[k] = replace(datadict[k], lookup_key, value)
         if k == lookup_key:
             replaced_dict[k] = value
     return replaced_dict
```

### Comparing `cysecuretools-4.1.0/cysecuretools/core/jsonpath.py` & `cysecuretools-4.2.0/cysecuretools/core/jsonpath.py`

 * *Files identical despite different names*

### Comparing `cysecuretools-4.1.0/cysecuretools/core/key_data.py` & `cysecuretools-4.2.0/cysecuretools/core/key_data.py`

 * *Files identical despite different names*

### Comparing `cysecuretools-4.1.0/cysecuretools/core/key_handlers/ec_handler.py` & `cysecuretools-4.2.0/cysecuretools/core/key_handlers/ec_handler.py`

 * *Files identical despite different names*

### Comparing `cysecuretools-4.1.0/cysecuretools/core/key_handlers/rsa_handler.py` & `cysecuretools-4.2.0/cysecuretools/core/key_handlers/rsa_handler.py`

 * *Files identical despite different names*

### Comparing `cysecuretools-4.1.0/cysecuretools/core/key_helper.py` & `cysecuretools-4.2.0/cysecuretools/core/key_helper.py`

 * *Files identical despite different names*

### Comparing `cysecuretools-4.1.0/cysecuretools/core/logging_configurator.py` & `cysecuretools-4.2.0/cysecuretools/core/logging_configurator.py`

 * *Files 13% similar despite different names*

```diff
@@ -27,17 +27,23 @@
     The class that allows configuring the way how the data is logged
     """
 
     LOG_FORMATTER = CustomFormatter()
 
     @staticmethod
     def disable_logging():
+        """Disable all logging calls of severity 'CRITICAL' and below"""
         logging.disable(logging.CRITICAL)
 
     @staticmethod
+    def enable_logging():
+        """Restore disabled logging"""
+        logging.disable(logging.NOTSET)
+
+    @staticmethod
     def set_logger_level(level):
         """
         Sets logging level (ERROR, WARNING, INFO, DEBUG)
         """
         root_logger = logging.getLogger()
         root_logger.setLevel(level)
         for handler in root_logger.handlers:
```

### Comparing `cysecuretools-4.1.0/cysecuretools/core/logging_formatter.py` & `cysecuretools-4.2.0/cysecuretools/core/logging_formatter.py`

 * *Files identical despite different names*

### Comparing `cysecuretools-4.1.0/cysecuretools/core/memory_area.py` & `cysecuretools-4.2.0/cysecuretools/core/memory_area.py`

 * *Files identical despite different names*

### Comparing `cysecuretools-4.1.0/cysecuretools/core/memory_map_base.py` & `cysecuretools-4.2.0/cysecuretools/core/memory_map_base.py`

 * *Files 4% similar despite different names*

```diff
@@ -29,14 +29,29 @@
     @property
     @abc.abstractmethod
     def FLASH_SIZE(self):
         raise NotImplementedError
 
     @property
     @abc.abstractmethod
+    def RAM_ADDR(self):
+        """RAM address"""
+
+    @property
+    @abc.abstractmethod
+    def SRAM_ADDR(self):
+        """SRAM address"""
+
+    @property
+    @abc.abstractmethod
+    def SRAM_SIZE(self):
+        """SRAM size"""
+
+    @property
+    @abc.abstractmethod
     def PROVISION_JWT_PACKET_ADDRESS(self):
         raise NotImplementedError
 
     @property
     @abc.abstractmethod
     def PROVISION_JWT_PACKET_SIZE(self):
         raise NotImplementedError
```

### Comparing `cysecuretools-4.1.0/cysecuretools/core/ocd_settings.py` & `cysecuretools-4.2.0/cysecuretools/core/ocd_settings.py`

 * *Files identical despite different names*

### Comparing `cysecuretools-4.1.0/cysecuretools/core/policy_filter_base.py` & `cysecuretools-4.2.0/cysecuretools/core/policy_filter_base.py`

 * *Files identical despite different names*

### Comparing `cysecuretools-4.1.0/cysecuretools/core/policy_validator_base.py` & `cysecuretools-4.2.0/cysecuretools/core/policy_validator_base.py`

 * *Files identical despite different names*

### Comparing `cysecuretools-4.1.0/cysecuretools/core/progress_bar.py` & `cysecuretools-4.2.0/cysecuretools/core/progress_bar.py`

 * *Files identical despite different names*

### Comparing `cysecuretools-4.1.0/cysecuretools/core/project.py` & `cysecuretools-4.2.0/cysecuretools/core/project.py`

 * *Files identical despite different names*

### Comparing `cysecuretools-4.1.0/cysecuretools/core/provisioning_flows/application.py` & `cysecuretools-4.2.0/cysecuretools/core/provisioning_flows/application.py`

 * *Files identical despite different names*

### Comparing `cysecuretools-4.1.0/cysecuretools/core/provisioning_flows/flow.py` & `cysecuretools-4.2.0/cysecuretools/core/provisioning_flows/flow.py`

 * *Files identical despite different names*

### Comparing `cysecuretools-4.1.0/cysecuretools/core/register_map_base.py` & `cysecuretools-4.2.0/cysecuretools/core/register_map_base.py`

 * *Files identical despite different names*

### Comparing `cysecuretools-4.1.0/cysecuretools/core/signtool_base.py` & `cysecuretools-4.2.0/cysecuretools/core/signtool_base.py`

 * *Files identical despite different names*

### Comparing `cysecuretools-4.1.0/cysecuretools/core/strategy_context/cert_strategy_ctx.py` & `cysecuretools-4.2.0/cysecuretools/core/strategy_context/cert_strategy_ctx.py`

 * *Files identical despite different names*

### Comparing `cysecuretools-4.1.0/cysecuretools/core/strategy_context/encrypted_programming_strategy_ctx.py` & `cysecuretools-4.2.0/cysecuretools/core/strategy_context/encrypted_programming_strategy_ctx.py`

 * *Files identical despite different names*

### Comparing `cysecuretools-4.1.0/cysecuretools/core/strategy_context/prov_packet_strategy_ctx.py` & `cysecuretools-4.2.0/cysecuretools/core/strategy_context/prov_packet_strategy_ctx.py`

 * *Files identical despite different names*

### Comparing `cysecuretools-4.1.0/cysecuretools/core/strategy_context/provisioning_strategy_ctx.py` & `cysecuretools-4.2.0/cysecuretools/core/strategy_context/provisioning_strategy_ctx.py`

 * *Files 19% similar despite different names*

```diff
@@ -30,15 +30,19 @@
         pass
 
     @abstractmethod
     def erase_flash(self, tool, target):
         pass
 
     @abstractmethod
-    def convert_to_rma(self, tool, target, **kwargs):
+    def transit_to_rma(self, tool, target, cert, **kwargs):
+        pass
+
+    @abstractmethod
+    def open_rma(self, tool, target, cert):
         pass
 
 
 class ProvisioningContext:
     """
     The Context defines the interface of interest to clients.
     """
@@ -76,12 +80,18 @@
 
     def erase_flash(self, tool, target):
         """
         Delegates work to the Strategy object.
         """
         self._strategy.erase_flash(tool, target)
 
-    def convert_to_rma(self, tool, target, **kwargs):
+    def transit_to_rma(self, tool, target, cert, **kwargs):
+        """
+        Delegates work to the Strategy object.
+        """
+        return self._strategy.transit_to_rma(tool, target, cert, **kwargs)
+
+    def open_rma(self, tool, target, cert):
         """
         Delegates work to the Strategy object.
         """
-        return self._strategy.convert_to_rma(tool, target, **kwargs)
+        return self._strategy.open_rma(tool, target, cert)
```

### Comparing `cysecuretools-4.1.0/cysecuretools/core/strops.py` & `cysecuretools-4.2.0/cysecuretools/core/strops.py`

 * *Files identical despite different names*

### Comparing `cysecuretools-4.1.0/cysecuretools/core/target_builder.py` & `cysecuretools-4.2.0/cysecuretools/core/target_builder.py`

 * *Files 2% similar despite different names*

```diff
@@ -149,7 +149,13 @@
 
     @abstractmethod
     def get_test_packages(self):
         """
         Gets a dictionary with Python packages containing content for
         testing purpose
         """
+
+    @abstractmethod
+    def get_silicon_id(self):
+        """
+        Gets the target silicon ID
+        """
```

### Comparing `cysecuretools-4.1.0/cysecuretools/core/target_director.py` & `cysecuretools-4.2.0/cysecuretools/core/target_director.py`

 * *Files 2% similar despite different names*

```diff
@@ -129,14 +129,17 @@
         # Policy generator
         target.policy_generator = self._builder.get_policy_generator(
             policy_parser)
 
         # Python package name containing content for testing purpose
         target.test_packages = self._builder.get_test_packages()
 
+        # Target silicon ID
+        target.silicon_id = self._builder.get_silicon_id()
+
         self._instantiate_types(target)
 
         return target
 
     @staticmethod
     def _instantiate_types(target):
         """
@@ -177,14 +180,15 @@
         self._sign_tool = None
         self._key_source = None
         self._bootloader_provider = None
         self._version_provider = None
         self._debug_certificate = None
         self._policy_generator = None
         self._test_packages = None
+        self._silicon_id = None
 
     @property
     def name(self):
         return self._name
 
     @name.setter
     def name(self, name):
@@ -401,7 +405,15 @@
     @property
     def test_packages(self):
         return self._test_packages
 
     @test_packages.setter
     def test_packages(self, packages):
         self._test_packages = packages
+
+    @property
+    def silicon_id(self):
+        return self._silicon_id
+
+    @silicon_id.setter
+    def silicon_id(self, silicon_id):
+        self._silicon_id = silicon_id
```

### Comparing `cysecuretools-4.1.0/cysecuretools/core/voltage_tool.py` & `cysecuretools-4.2.0/cysecuretools/core/voltage_tool.py`

 * *Files identical despite different names*

### Comparing `cysecuretools-4.1.0/cysecuretools/data/cy_bootloader_map.json` & `cysecuretools-4.2.0/cysecuretools/data/cy_bootloader_map.json`

 * *Files 16% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9772727272727273%*

 * *Differences: {"'targets'": "{'cyb06xx5_a1': 'cyx06xxx'}"}*

```diff
@@ -30,12 +30,13 @@
         "cy8ckit-064b0s2-4343w": "cyx06xxx",
         "cy8ckit-064s0s2-4343w": "cyx06xxx",
         "cy8cproto-064b0s1-ble": "cyx06xxx",
         "cy8cproto-064b0s1-ssa": "cyx06xxx",
         "cy8cproto-064b0s3": "cyx06xxx",
         "cy8cproto-064s1-sb": "cyx06xxx",
         "cyb06xx5": "cyx06xxx",
+        "cyb06xx5_a1": "cyx06xxx",
         "cyb06xx7": "cyx06xxx",
         "cyb06xxa": "cyx06xxx",
         "cys06xxa": "cyx06xxx"
     }
 }
```

### Comparing `cysecuretools-4.1.0/cysecuretools/data/mxs40sv2/mxs40sv2_ram_app_status_codes.py` & `cysecuretools-4.2.0/cysecuretools/data/mxs40sv2/mxs40sv2_ram_app_status_codes.py`

 * *Files identical despite different names*

### Comparing `cysecuretools-4.1.0/cysecuretools/data/mxs40v1/mxs40v1_sfb_status_codes.py` & `cysecuretools-4.2.0/cysecuretools/data/mxs40v1/mxs40v1_sfb_status_codes.py`

 * *Files identical despite different names*

### Comparing `cysecuretools-4.1.0/cysecuretools/execute/bootloader_provider_mxs40v1.py` & `cysecuretools-4.2.0/cysecuretools/execute/bootloader_provider_mxs40v1.py`

 * *Files identical despite different names*

### Comparing `cysecuretools-4.1.0/cysecuretools/execute/debug_cert/debug_cert_mxs40sv2.py` & `cysecuretools-4.2.0/cysecuretools/execute/debug_cert/debug_cert_mxs40sv2.py`

 * *Files identical despite different names*

### Comparing `cysecuretools-4.1.0/cysecuretools/execute/debug_cert/debug_cert_parser_mxs40sv2.py` & `cysecuretools-4.2.0/cysecuretools/execute/debug_cert/debug_cert_parser_mxs40sv2.py`

 * *Files identical despite different names*

### Comparing `cysecuretools-4.1.0/cysecuretools/execute/encrypted_programming/aes_cipher.py` & `cysecuretools-4.2.0/cysecuretools/execute/encrypted_programming/aes_cipher.py`

 * *Files identical despite different names*

### Comparing `cysecuretools-4.1.0/cysecuretools/execute/encrypted_programming/aes_header.py` & `cysecuretools-4.2.0/cysecuretools/execute/encrypted_programming/aes_header.py`

 * *Files identical despite different names*

### Comparing `cysecuretools-4.1.0/cysecuretools/execute/encrypted_programming/aes_header_strategy.py` & `cysecuretools-4.2.0/cysecuretools/execute/encrypted_programming/aes_header_strategy.py`

 * *Files identical despite different names*

### Comparing `cysecuretools-4.1.0/cysecuretools/execute/encrypted_programming/ecc_kdf.py` & `cysecuretools-4.2.0/cysecuretools/execute/encrypted_programming/ecc_kdf.py`

 * *Files identical despite different names*

### Comparing `cysecuretools-4.1.0/cysecuretools/execute/encrypted_programming/encrypted_programming.py` & `cysecuretools-4.2.0/cysecuretools/execute/encrypted_programming/encrypted_programming.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,14 @@
 class EPMode(IntEnum):
     init = 0x00
     data = 0x01
     finish = 0x02
 
 
 def program(tool, target, encrypted_image):
-    tool.reset()
     encrypted_image_path = os.path.abspath(encrypted_image)
     logger.info("Start encrypted programming of '%s':", encrypted_image_path)
 
     # Read keys ID and AES header
     with open(encrypted_image, 'r', encoding='utf-8') as f:
         file_lines = f.readlines()
         host_key_id = int(file_lines[0].strip()[:2])
@@ -87,10 +86,9 @@
 
     # Finish programming
     logger.debug('\nFinish encrypted programming:')
     syscall_status = encrypted_programming(tool, target.register_map,
                                            EPMode.finish, None)
     if not syscall_status:
         return False
-    tool.reset(ResetType.HW)
 
     return True
```

### Comparing `cysecuretools-4.1.0/cysecuretools/execute/entrance_exam/exam_cyb06xx7.py` & `cysecuretools-4.2.0/cysecuretools/execute/entrance_exam/exam_cyb06xx7.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,20 +27,20 @@
 class EntranceExamCyb06xx7(EntranceExamMXS40v1):
     def __init__(self, target: Target, **kwargs):
         super(EntranceExamCyb06xx7, self).__init__(target, **kwargs)
         self.word_size = 4
         self.asset_hash_len = 16
         self.mem_map = target.memory_map
 
-    def execute(self, tool):
+    def execute(self, tool, **kwargs):
         """
         Checks device life-cycle, Flashboot firmware, Flash state and
         bunch of registers.
         """
-        exam_status = super(EntranceExamCyb06xx7, self).execute(tool)
+        exam_status = super(EntranceExamCyb06xx7, self).execute(tool, **kwargs)
         if exam_status == EntranceExamStatus.OK:
             if self.verify_asset_hash(tool):
                 return EntranceExamStatus.OK
             else:
                 return EntranceExamStatus.FAIL
 
     def verify_asset_hash(self, tool):
```

### Comparing `cysecuretools-4.1.0/cysecuretools/execute/entrance_exam/exam_mxs40v1.py` & `cysecuretools-4.2.0/cysecuretools/execute/entrance_exam/exam_mxs40v1.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,15 +11,18 @@
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 import os
 import logging
+
+from cysecuretools.core.connect_helper import ConnectHelper
 from cysecuretools.core.enums import EntranceExamStatus, RegionHashStatus
+from cysecuretools.core.strategy_context.provisioning_strategy_ctx import ProvisioningContext
 from cysecuretools.execute.sys_call import region_hash, read_lifecycle
 from cysecuretools.execute.programmer.base import AP
 from cysecuretools.execute.provisioning_packet.lib import Crypto
 from cysecuretools.core.target_director import Target
 from cysecuretools.core.entrance_exam_base import EntranceExam
 from cysecuretools.targets.common.p64.enums import ProtectionState
 
@@ -38,32 +41,42 @@
         self.target = target
 
     @property
     def entrance_exam_jwt(self):
         packet_dir = self.target.policy_parser.get_provisioning_packet_dir()
         return os.path.abspath(os.path.join(packet_dir, ENTRANCE_EXAM_JWT))
 
-    def execute(self, tool):
+    def execute(self, tool, **kwargs):
         """
-        Checks device life-cycle, Flashboot firmware, Flash state and
-        bunch of registers.
+        Checks device life-cycle, FlashBoot firmware, Flash state and
+        a bunch of registers.
         """
         jwt_text = Crypto.read_jwt(self.entrance_exam_jwt)
 
         logger.info('*****************************************')
         logger.info('             ENTRANCE EXAM               ')
         logger.info('*****************************************')
 
         complete = self.target.silicon_data_reader.read_complete_status(tool)
         exam_pass = not complete
         if not exam_pass:
             logger.error('Device has been previously provisioned')
 
         if exam_pass:
+            ConnectHelper.disconnect(tool)
+            ConnectHelper.connect(tool, self.target,
+                                  probe_id=tool.probe_id, ap='cm4')
             tool.examine_ap()
+
+            # Erase flash
+            context = ProvisioningContext(self.target.provisioning_strategy)
+            if kwargs.get('erase_flash'):
+                context.erase_flash(tool, self.target)
+
+            # Verify voltage
             voltage = self.target.voltage_tool.get_voltage(tool)
             v_min = self.target.voltage_tool.voltage_level * 0.9
             v_max = self.target.voltage_tool.voltage_level * 1.1
             if voltage < v_min or voltage > v_max:
                 exam_pass = False
                 logger.error(
                     'Silicon voltage is out of range. Expected voltage level '
```

### Comparing `cysecuretools-4.1.0/cysecuretools/execute/image_cert.py` & `cysecuretools-4.2.0/cysecuretools/execute/image_cert.py`

 * *Files identical despite different names*

### Comparing `cysecuretools-4.1.0/cysecuretools/execute/image_signing/encrypt_mxv40sv2.py` & `cysecuretools-4.2.0/cysecuretools/execute/image_signing/encrypt_mxv40sv2.py`

 * *Files identical despite different names*

### Comparing `cysecuretools-4.1.0/cysecuretools/execute/image_signing/image.py` & `cysecuretools-4.2.0/cysecuretools/execute/image_signing/image.py`

 * *Files identical despite different names*

### Comparing `cysecuretools-4.1.0/cysecuretools/execute/image_signing/image_config_parser.py` & `cysecuretools-4.2.0/cysecuretools/execute/image_signing/image_config_parser.py`

 * *Files identical despite different names*

### Comparing `cysecuretools-4.1.0/cysecuretools/execute/image_signing/rsa_converter.py` & `cysecuretools-4.2.0/cysecuretools/execute/image_signing/rsa_converter.py`

 * *Files identical despite different names*

### Comparing `cysecuretools-4.1.0/cysecuretools/execute/image_signing/signtool_mxs40v1.py` & `cysecuretools-4.2.0/cysecuretools/execute/image_signing/signtool_mxs40v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -337,21 +337,14 @@
         for file in self.tmp_files:
             if file is not None:
                 try:
                     os.remove(file)
                 except OSError:
                     pass
 
-    @staticmethod
-    def _get_image_id(kwargs):
-        image_id = kwargs.get('image_id')
-        if image_id is None:
-            raise KeyError("Mandatory argument 'image_id' not specified")
-        return image_id
-
     def _get_min_erase_size(self, min_erase_size, slot_address):
         if self.mem_map.FLASH_ADDRESS <= slot_address < self.mem_map.FLASH_SIZE + \
                 self.mem_map.FLASH_ADDRESS:
             return self.mem_map.MIN_INT_ERASE_SIZE
         if min_erase_size is None:
             return self.mem_map.MIN_EXT_ERASE_SIZE
         return int(str(min_erase_size), 0)
@@ -372,14 +365,19 @@
                 'internal and external Flash memory are 0x00 and 0xFF '
                 'respectively', erased_val)
         else:
             erased_val = self._default_erased_value(image_type)
         return erased_val
 
     @staticmethod
+    def _get_image_id(kwargs):
+        image_id = kwargs.get('image_id')
+        return 1 if image_id is None else image_id
+
+    @staticmethod
     def _get_image_type(kwargs):
         image_type = kwargs.get('image_type')
         return image_type.upper() if image_type is not None else None
 
     def _get_upgrade_mode(self, kwargs):
         upgrade_mode = kwargs.get('upgrade_mode', self.upgrade_mode).lower()
         self._validate_upgrade_mode(upgrade_mode)
```

### Comparing `cysecuretools-4.1.0/cysecuretools/execute/image_signing/signtool_mxv40sv2.py` & `cysecuretools-4.2.0/cysecuretools/execute/image_signing/signtool_mxv40sv2.py`

 * *Files 3% similar despite different names*

```diff
@@ -28,14 +28,15 @@
 from cysecuretools.core.key_handlers import RSAHandler
 from .image_config_parser import ImageConfigParser
 from .rsa_converter import RSAConverter
 from .encrypt_mxv40sv2 import EncryptorMXS40Sv2
 from .xip_encryptor import XipEncryptor
 from cysecuretools.targets.common.mxs40sv2.enums import PolicyType
 from cysecuretools.execute.image_signing.image import Image
+from ...targets.common.mxs40sv2.nv_counter_calc import NvCounterCalculator
 
 
 logger = logging.getLogger(__name__)
 
 
 class SignToolMXS40Sv2(SignTool):
     IMAGE_ALIGNMENT = 8
@@ -62,14 +63,15 @@
         skip_tlv_info = kwargs.get('skip_tlv_info', False)
         hex_addr = self._get_hex_addr(kwargs)
         pad = self._get_pad(kwargs)
         confirm = self._get_confirm(image_format, kwargs)
         overwrite_only = self._get_overwrite_only(image_format, kwargs)
         align = self._get_align(kwargs)
         image_version = self._get_image_version(kwargs)
+        image_id = kwargs.get('image_id', 0)
         update_key_id = kwargs.get('update_key_id')
         update_key_path = kwargs.get('update_key_path')
 
         if 'bootrom_next_app' == image_format:
             if pubkey_data is None:
                 raise ValueError('Public key not specified')
 
@@ -83,15 +85,15 @@
             protected_tlv.append((t, v))
 
         nv_counter = None
         if self.policy_parser.json:
             policy_type = self.policy_parser.get_policy_type()
             if policy_type == PolicyType.REPROVISIONING_SECURE:
                 nv_counter, update_packet = self._get_update_packet_data(
-                   update_key_id, update_key_path)
+                   update_key_id, update_key_path, image_id)
                 protected_tlv.append(update_packet)
             else:
                 if update_key_id is not None or update_key_path:
                     logger.warning(
                         "The update key is specified, but the policy is not of "
                         "the 'reprovisioning_secure' type. Update packet will "
                         "not be added to the image")
@@ -139,14 +141,15 @@
         pad = self._get_pad(kwargs)
         confirm = self._get_confirm(image_format, kwargs)
         overwrite_only = self._get_overwrite_only(image_format, kwargs)
         min_erase_size = self._get_min_erase_size(kwargs)
         align = self._get_align(kwargs)
         dependencies = self._get_dependencies(kwargs)
         image_version = self._get_image_version(kwargs)
+        image_id = self._get_image_id(kwargs)
 
         if not RSAHandler.is_private_key(key_path):
             raise ValueError(f'Signing image with public key \'{key_path}\'')
 
         self._time_warning(pad, slot_size)
 
         tlvs = self._get_config_tlvs(kwargs.get('image_config'))
@@ -198,15 +201,16 @@
         if image_format in ['bootrom_next_app', 'bootrom_ram_app']:
             pubkey_data = RSAConverter.convert_to_mbedtls(key_path)
             args['custom_tlv'].append(('0xf0', f'0x{pubkey_data}'))
 
         policy_type = self.policy_parser.get_policy_type()
         if policy_type == PolicyType.REPROVISIONING_SECURE:
             nv_counter, update_packet = self._get_update_packet_data(
-                kwargs.get('update_key_id'), kwargs.get('update_key_path'))
+                kwargs.get('update_key_id'), kwargs.get('update_key_path'),
+                image_id)
             args['security_counter'] = nv_counter
             args['custom_tlv'].append(update_packet)
 
         try:
             self._call_imgtool_sign(args)
         except Exception:
             logger.error('Signature not added')
@@ -236,24 +240,29 @@
             else:
                 logger.info(
                     'Image signed and encrypted successfully (%s)', output)
         else:
             logger.info('Image signed successfully (%s)', output)
         return output
 
-    def _get_update_packet_data(self, update_key_id, update_key_path):
+    def _get_update_packet_data(self, update_key_id, update_key_path, image_id):
         if update_key_id is None and update_key_path is None:
             raise KeyError('Either update data packet key ID or key path '
                            'must be specified')
         if update_key_path is None:
             update_key_path = self.key_source.get_key(update_key_id, 'private')
 
-        nv_counter = self.policy_parser.get_nv_counter()
+        nv_counter = NvCounterCalculator.calculate(
+            self.policy_parser.get_nv_counter(),
+            self.policy_parser.get_bits_per_cnt(),
+            image_id=image_id)
+
         reprov_data = binascii.hexlify(self._reprovisioning_packet(
-            key_id=update_key_id, key_path=update_key_path)).decode()
+            key_id=update_key_id, key_path=update_key_path,
+            image_id=image_id)).decode()
         return nv_counter, ('0x51', f'0x{reprov_data}')
 
     def _reprovisioning_packet(self, **kwargs):
         from ..provisioning_packet.provisioning_packet_mxs40sv2 import (
             ProvisioningPacketMXS40Sv2)
         packet = ProvisioningPacketMXS40Sv2(self.policy_parser)
         return packet.reprovisioning_data(self.target.key_source, **kwargs)
@@ -353,14 +362,19 @@
     def _get_confirm(image_format, kwargs):
         if image_format == 'mcuboot_user_app':
             return kwargs.get('confirm', False)
         else:
             return False
 
     @staticmethod
+    def _get_image_id(kwargs):
+        image_id = kwargs.get('image_id')
+        return 0 if image_id is None else image_id
+
+    @staticmethod
     def validate_trailer(bin_file, slot_size, min_erase_size):
         """
         Checks whether there is only trailer data in the last sector of the image.
         Only trailer should be present in the last sector of the slot, otherwise
         the image will not be validated by MCUboot.
         @param bin_file: Input file to validate
         @param min_erase_size: Minimum erase size to be used
```

### Comparing `cysecuretools-4.1.0/cysecuretools/execute/image_signing/xip_encryptor.py` & `cysecuretools-4.2.0/cysecuretools/execute/image_signing/xip_encryptor.py`

 * *Files identical despite different names*

### Comparing `cysecuretools-4.1.0/cysecuretools/execute/imgtool/__init__.py` & `cysecuretools-4.2.0/cysecuretools/execute/imgtool/__init__.py`

 * *Files identical despite different names*

### Comparing `cysecuretools-4.1.0/cysecuretools/execute/imgtool/boot_record.py` & `cysecuretools-4.2.0/cysecuretools/execute/imgtool/boot_record.py`

 * *Files identical despite different names*

### Comparing `cysecuretools-4.1.0/cysecuretools/execute/imgtool/custom_encryptor.py` & `cysecuretools-4.2.0/cysecuretools/execute/imgtool/custom_encryptor.py`

 * *Files identical despite different names*

### Comparing `cysecuretools-4.1.0/cysecuretools/execute/imgtool/image.py` & `cysecuretools-4.2.0/cysecuretools/execute/imgtool/image.py`

 * *Files identical despite different names*

### Comparing `cysecuretools-4.1.0/cysecuretools/execute/imgtool/keys/__init__.py` & `cysecuretools-4.2.0/cysecuretools/execute/imgtool/keys/__init__.py`

 * *Files identical despite different names*

### Comparing `cysecuretools-4.1.0/cysecuretools/execute/imgtool/keys/ecdsa.py` & `cysecuretools-4.2.0/cysecuretools/execute/imgtool/keys/ecdsa.py`

 * *Files identical despite different names*

### Comparing `cysecuretools-4.1.0/cysecuretools/execute/imgtool/keys/ecdsa_test.py` & `cysecuretools-4.2.0/cysecuretools/execute/imgtool/keys/ecdsa_test.py`

 * *Files identical despite different names*

### Comparing `cysecuretools-4.1.0/cysecuretools/execute/imgtool/keys/ed25519.py` & `cysecuretools-4.2.0/cysecuretools/execute/imgtool/keys/ed25519.py`

 * *Files identical despite different names*

### Comparing `cysecuretools-4.1.0/cysecuretools/execute/imgtool/keys/ed25519_test.py` & `cysecuretools-4.2.0/cysecuretools/execute/imgtool/keys/ed25519_test.py`

 * *Files identical despite different names*

### Comparing `cysecuretools-4.1.0/cysecuretools/execute/imgtool/keys/general.py` & `cysecuretools-4.2.0/cysecuretools/execute/imgtool/keys/general.py`

 * *Files identical despite different names*

### Comparing `cysecuretools-4.1.0/cysecuretools/execute/imgtool/keys/rsa.py` & `cysecuretools-4.2.0/cysecuretools/execute/imgtool/keys/rsa.py`

 * *Files identical despite different names*

### Comparing `cysecuretools-4.1.0/cysecuretools/execute/imgtool/keys/rsa_test.py` & `cysecuretools-4.2.0/cysecuretools/execute/imgtool/keys/rsa_test.py`

 * *Files identical despite different names*

### Comparing `cysecuretools-4.1.0/cysecuretools/execute/imgtool/keys/x25519.py` & `cysecuretools-4.2.0/cysecuretools/execute/imgtool/keys/x25519.py`

 * *Files identical despite different names*

### Comparing `cysecuretools-4.1.0/cysecuretools/execute/imgtool/main.py` & `cysecuretools-4.2.0/cysecuretools/execute/imgtool/main.py`

 * *Files identical despite different names*

### Comparing `cysecuretools-4.1.0/cysecuretools/execute/imgtool/version.py` & `cysecuretools-4.2.0/cysecuretools/execute/imgtool/version.py`

 * *Files identical despite different names*

### Comparing `cysecuretools-4.1.0/cysecuretools/execute/jwt.py` & `cysecuretools-4.2.0/cysecuretools/execute/jwt.py`

 * *Files identical despite different names*

### Comparing `cysecuretools-4.1.0/cysecuretools/execute/key_reader.py` & `cysecuretools-4.2.0/cysecuretools/execute/key_reader.py`

 * *Files identical despite different names*

### Comparing `cysecuretools-4.1.0/cysecuretools/execute/key_reader_mxs40v1.py` & `cysecuretools-4.2.0/cysecuretools/execute/key_reader_mxs40v1.py`

 * *Files identical despite different names*

### Comparing `cysecuretools-4.1.0/cysecuretools/execute/key_source/key_source_mxs40sv2.py` & `cysecuretools-4.2.0/cysecuretools/execute/key_source/key_source_mxs40sv2.py`

 * *Files identical despite different names*

### Comparing `cysecuretools-4.1.0/cysecuretools/execute/key_source/key_source_mxs40v1.py` & `cysecuretools-4.2.0/cysecuretools/execute/key_source/key_source_mxs40v1.py`

 * *Files identical despite different names*

### Comparing `cysecuretools-4.1.0/cysecuretools/execute/keygen.py` & `cysecuretools-4.2.0/cysecuretools/execute/keygen.py`

 * *Files 7% similar despite different names*

```diff
@@ -62,15 +62,15 @@
 
     if filename is not None:
         dirname = os.path.dirname(filename)
         if dirname:
             os.makedirs(os.path.dirname(filename), exist_ok=True)
         with open(filename, 'wb') as fp:
             fp.write(key)
-        logger.info("Created key in '%s'", filename)
+        logger.info("Created a key '%s'", os.path.abspath(filename))
     return KeyPair(key, None)
 
 
 def generate_ecdsa_key(kid=6, jwkey=None, pem_priv=None, pem_pub=None,
                        template=None):
     """Creates either private or public key using ECDSA algorithm
     :param kid: Customer key ID. Key ID to define key slot number in
@@ -84,20 +84,21 @@
     :param template: JSON file containing public key numbers
     :return: A key in JWK format
     """
     if template:
         try:
             data = read_json(template)
             pubkey = ECHandler.populate_public_key(bytes.fromhex(data['pub']))
-        except ValueError:
-            logger.error('The template contains invalid data (%s)', template)
-            return None
-        except KeyError:
-            logger.error('The template structure is invalid (%s)', template)
-            return None
+        except ValueError as e:
+            raise ValueError(
+                f'The template contains invalid data ({template})') from e
+        except KeyError as e:
+            raise KeyError(
+                f'The template structure is invalid ({template})') from e
+
         key_json = ECHandler.public_jwk(pubkey, kid)
     else:
         key_json = _ecdsa_private_key(kid=kid)
 
     _save_ec_key(key_json, jwkey, pem_priv, pem_pub)
 
     return json.dumps(key_json, indent=4)
@@ -111,26 +112,28 @@
 
 
 def _save_ec_key(key_json, jwkey, pem_priv, pem_pub):
     if jwkey:
         os.makedirs(os.path.dirname(jwkey), exist_ok=True)
         with open(jwkey, 'w', encoding='utf-8') as fp:
             fp.write(json.dumps(key_json, indent=4))
-            logger.info("Created a key in '%s'", jwkey)
+            logger.info("Created a key '%s'", os.path.abspath(jwkey))
 
         key = ECKey(key_json, ALGORITHMS.ES256)
         if pem_priv:
             os.makedirs(os.path.dirname(pem_priv), exist_ok=True)
             with open(pem_priv, 'wb') as fp:
                 fp.write(key.to_pem().strip())
+                logger.info("Created a key '%s'", os.path.abspath(pem_priv))
 
         if pem_pub:
             os.makedirs(os.path.dirname(pem_pub), exist_ok=True)
             with open(pem_pub, 'wb') as fp:
                 fp.write(key.public_key().to_pem().strip())
+                logger.info("Created a key '%s'", os.path.abspath(pem_pub))
 
 
 def create_rsa_key(priv_key, pub_key, template=None, hash_path=None):
     """
     Either creates a new RSA key in PEM format or converts RSA key
     modulus and exponent to PEM if a template is specified
     @param priv_key: A path where to save private key
@@ -140,22 +143,23 @@
     :return: Named tuple containing private and public key pair
     """
     if template:
         data = read_json(template)
         try:
             key = RSAHandler.populate_public_key(
                 data['exponent'], data['modulus'])
-        except ValueError:
-            logger.error('The template contains invalid data (%s)', template)
-            return None
-        except KeyError:
-            logger.error('The template structure is invalid (%s)', template)
-            return None
+        except ValueError as e:
+            raise ValueError(
+                f'The template contains invalid data ({template})') from e
+        except KeyError as e:
+            raise KeyError(
+                f'The template structure is invalid ({template})') from e
+
         RSAHandler.save_public_key(key, pub_key)
-        logger.info("Created public key in '%s'", pub_key)
+        logger.info("Created a key '%s'", pub_key)
         keypair = KeyPair(None, key)
     else:
         keypair = _generate_rsa_key(priv_key, pub_key)
 
     if hash_path is not None:
         create_pubkey_hash(pub_key, hash_path)
 
@@ -194,17 +198,17 @@
         format=serialization.PublicFormat.SubjectPublicKeyInfo)
 
     key_dir = os.path.dirname(priv_key_path)
     if key_dir:
         os.makedirs(key_dir, exist_ok=True)
     with open(priv_key_path, 'wb') as fp:
         fp.write(private_pem)
-        logger.info("Created private key '%s'", priv_key_path)
+        logger.info("Created a key '%s'", os.path.abspath(priv_key_path))
 
     key_dir = os.path.dirname(pub_key_path)
     if key_dir:
         os.makedirs(key_dir, exist_ok=True)
     with open(pub_key_path, 'wb') as fp:
         fp.write(public_pem)
-        logger.info("Created public key '%s'", pub_key_path)
+        logger.info("Created a key '%s'", os.path.abspath(pub_key_path))
 
     return KeyPair(private_key, public_key)
```

### Comparing `cysecuretools-4.1.0/cysecuretools/execute/programmer/__init__.py` & `cysecuretools-4.2.0/cysecuretools/execute/programmer/__init__.py`

 * *Files identical despite different names*

### Comparing `cysecuretools-4.1.0/cysecuretools/execute/programmer/base.py` & `cysecuretools-4.2.0/cysecuretools/execute/programmer/base.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """
-Copyright (c) 2019 Cypress Semiconductor Corporation
+Copyright 2019-2023 Cypress Semiconductor Corporation (an Infineon company)
+or an affiliate of Cypress Semiconductor Corporation. All rights reserved.
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
 
@@ -14,57 +15,44 @@
 limitations under the License.
 """
 from enum import Enum
 from abc import ABCMeta, abstractmethod
 
 
 class ResetType(Enum):
+    """Enumeration for reset types"""
     SW = 1
     HW = 2
 
 
 class Interface(Enum):
+    """Enumeration for communication interfaces"""
     SWD = 1
     JTAG = 2
 
 
 class AP(Enum):
+    """Enumeration for access ports"""
     SYS = 'sys'
     CM0 = 'cm0'
     CM4 = 'cm4'
     CMx = 'cmx'
     CM33 = 'cm33'
 
 
 class ProgrammerBase(metaclass=ABCMeta):
+    """Base class which is necessary to be implemented by the classes
+    providing communication with OCD
+    """
+
     def __init__(self, name, path, require_path=True):
         self.name = name
         self.tool_path = path
         self.require_path = require_path
 
-    def _start_core(self):
-        """
-        Writes infinite loop into RAM and starts core execution.
-        CM0 will not be able to execute sys calls in case it is in
-        undefined state.
-        """
-        start_core_program_address = 0x08000000
-        program_counter_address = 0x08000000
-        stack_pointer_address = 0x08001000
-        thumb_bit_address = 0x01000000
-        infinite_loop_code = 0xE7FEB662
-        self.halt()
-        # B662 - CPSIE I - Enable IRQ by clearing PRIMASK
-        # E7FE - B - Jump to address (argument is an offset)
-        self.write32(start_core_program_address, infinite_loop_code)
-        self.write_reg('pc', program_counter_address)
-        self.write_reg('sp', stack_pointer_address)
-        self.write_reg('xpsr', thumb_bit_address)
-        self.resume()
-
     @property
     def wait_for_target(self):
         """
         Gets a value indicating whether to wait for the target
         if no available devices are connected
         """
         raise NotImplementedError
@@ -74,61 +62,60 @@
         """
         Sets a value indicating whether to wait for the target
         if no available devices are connected
         """
         raise NotImplementedError
 
     @abstractmethod
-    def connect(self, target_name=None, interface=None, probe_id=None,
-                ap=None, acquire=True, blocking=True, reset_and_halt=False,
-                power=None, voltage=None):
+    def connect(self, target_name=None, interface=None, probe_id=None, ap=None,
+                acquire=True, blocking=True, power=None, voltage=None,
+                ignore_errors=False):
         """
         Connects to target.
-        :param target_name: The target name.
-        :param interface: Debug interface.
-        :param probe_id: Probe serial number.
-        :param ap: The access port used for communication.
-        :param acquire: Indicates whether to acquire device on connect
-        :param blocking: Specifies whether to wait for a probe to be
+        @param target_name: The target name.
+        @param interface: Debug interface.
+        @param probe_id: Probe serial number.
+        @param ap: The access port used for communication.
+        @param acquire: Indicates whether to acquire device on connect
+        @param blocking: Specifies whether to wait for a probe to be
                connected if there are no available probes
-        :param reset_and_halt: Indicates whether to do reset and halt
-               after connect
-        :param power: Target power
-        :param voltage: Target power voltage
-        :return: True if connected successfully, otherwise False.
+        @param power: Target power
+        @param voltage: Target power voltage
+        @param ignore_errors: Ignore errors and continue execution
+        @return: True if connected successfully, otherwise False.
         """
         raise NotImplementedError()
 
     @abstractmethod
     def disconnect(self):
         """
         Disconnects from target.
         """
         raise NotImplementedError()
 
     @abstractmethod
     def get_ap(self):
         """
         Gets access port.
-        :return: Selected AP.
+        @return: Selected AP.
         """
         raise NotImplementedError()
 
     @abstractmethod
     def set_ap(self, ap):
         """
         Sets access port.
         """
         raise NotImplementedError()
 
     @abstractmethod
     def set_frequency(self, value_khz):
         """
         Sets probe frequency.
-        :param value_khz: Frequency in kHz.
+        @param value_khz: Frequency in kHz.
         """
         raise NotImplementedError()
 
     @abstractmethod
     def halt(self):
         """
         Halts the target.
@@ -142,156 +129,156 @@
         """
         raise NotImplementedError()
 
     @abstractmethod
     def reset(self, reset_type=ResetType.SW):
         """
         Resets the target.
-        :param reset_type: The reset type.
+        @param reset_type: The reset type.
         """
         raise NotImplementedError()
 
     @abstractmethod
     def reset_and_halt(self, reset_type=ResetType.SW):
         """
         Resets the target and halts the CPU immediately after reset.
-        :param reset_type: The reset type.
+        @param reset_type: The reset type.
         """
         raise NotImplementedError()
 
     @abstractmethod
     def read8(self, address):
         """
         Reads 8-bit value from specified memory location.
-        :param address: The memory address to read.
-        :return: The read value.
+        @param address: The memory address to read.
+        @return: The read value.
         """
         raise NotImplementedError()
 
     @abstractmethod
     def read16(self, address):
         """
         Reads 16-bit value from specified memory location.
-        :param address: The memory address to read.
-        :return: The read value.
+        @param address: The memory address to read.
+        @return: The read value.
         """
         raise NotImplementedError()
 
     @abstractmethod
     def read32(self, address):
         """
         Reads 32-bit value from specified memory location.
-        :param address: The memory address to read.
-        :return: The read value.
+        @param address: The memory address to read.
+        @return: The read value.
         """
         raise NotImplementedError()
 
     @abstractmethod
     def write8(self, address, value):
         """
         Writes 8-bit value by specified memory location.
-        :param address: The memory address to write.
-        :param value: The 8-bit value to write.
+        @param address: The memory address to write.
+        @param value: The 8-bit value to write.
         """
         raise NotImplementedError()
 
     @abstractmethod
     def write16(self, address, value):
         """
         Writes 16-bit value by specified memory location.
-        :param address: The memory address to write.
-        :param value: The 16-bit value to write.
+        @param address: The memory address to write.
+        @param value: The 16-bit value to write.
         """
         raise NotImplementedError()
 
     @abstractmethod
     def write32(self, address, value):
         """
         Writes 32-bit value by specified memory location.
-        :param address: The memory address to write.
-        :param value: The 32-bit value to write.
+        @param address: The memory address to write.
+        @param value: The 32-bit value to write.
         """
         raise NotImplementedError()
 
     @abstractmethod
     def read_reg(self, reg_name):
         """
         Gets value of a core register.
-        :param reg_name: Core register name.
-        :return: The register value.
+        @param reg_name: Core register name.
+        @return: The register value.
         """
         raise NotImplementedError()
 
     @abstractmethod
     def write_reg(self, reg_name, value):
         """
         Sets value of a core register.
-        :param reg_name: Core register name.
-        :param value: The value to set.
+        @param reg_name: Core register name.
+        @param value: The value to set.
         """
         raise NotImplementedError()
 
     @abstractmethod
     def erase(self, address, size):
         """
         Erases entire device flash or specified sectors.
-        :param address: The memory location.
-        :param size: The memory size.
+        @param address: The memory location.
+        @param size: The memory size.
         """
         raise NotImplementedError()
 
     @abstractmethod
     def program(self, filename, file_format=None, address=None):
         """
         Programs a file into flash.
-        :param filename: Path to a file.
-        :param file_format: File format. Default is to use the file's extension.
-        :param address: Base address used for the address where to flash a binary.
-        :return: True if programmed successfully, otherwise False.
+        @param filename: Path to a file.
+        @param file_format: File format. Default is to use the file's extension.
+        @param address: Base address used for the address where to flash a binary.
+        @return: True if programmed successfully, otherwise False.
         """
         raise NotImplementedError()
 
     @abstractmethod
     def read(self, address, length):
         """
         Reads a block of unaligned bytes in memory
-        :param address: The memory address where start reading
-        :param length: Number of bytes to read
-        :return: Values array
+        @param address: The memory address where start reading
+        @param length: Number of bytes to read
+        @return: Values array
         """
         raise NotImplementedError()
 
     @abstractmethod
     def write(self, address, data):
         """
         Writes a block of unaligned bytes in memory
-        :param address: The memory address where start writing
-        :param data: Data block
+        @param address: The memory address where start writing
+        @param data: Data block
         """
         raise NotImplementedError()
 
     @abstractmethod
     def get_probe_list(self):
         """
         Gets list of connected probes
         """
         raise NotImplementedError()
 
     def set_skip_reset_and_halt(self, value):
         """
         Sets skip_reset_and_halt property value. This is applicable
         for pyOCD and likely should not be implemented for other tools
-        :param value: Indicates whether to skip or not
+        @param value: Indicates whether to skip or not
         """
 
     def examine_ap(self):
         """
         Examines CMx (depending on selected ap for connection) AP
         without reset. This is applicable for OpenOCD and likely should
         not be implemented for other tools
         """
 
     @abstractmethod
     def get_voltage(self):
         """Reads target voltage
-        :@return Voltage value in Volts
+        @return Voltage value in Volts
         """
```

### Comparing `cysecuretools-4.1.0/cysecuretools/execute/programmer/openocd_server.py` & `cysecuretools-4.2.0/cysecuretools/execute/programmer/openocd_server.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """
-Copyright (c) 2020-2022 Cypress Semiconductor Corporation
+Copyright 2020-2023 Cypress Semiconductor Corporation (an Infineon company)
+or an affiliate of Cypress Semiconductor Corporation. All rights reserved.
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
 
@@ -18,16 +19,14 @@
 import enum
 import platform
 import time
 import atexit
 import subprocess
 from pathlib import Path
 
-import psutil
-
 from cysecuretools.core.logging_configurator import LoggingConfigurator
 from cysecuretools.core.ocd_settings import OcdSettings
 
 
 OPENOCD_DEFAULT_PATH = os.path.join(os.path.dirname(__file__), os.pardir,
                                     os.pardir, os.pardir, 'openocd')
 
@@ -127,27 +126,28 @@
         'Windows': 'win',
         'Linux':   'linux',
         'Darwin':  'osx',
     }
 
     log_counter = 1
 
-    def __init__(self, target, target_name=None, interface=None,
-                 probe_id=None, tool_path=None, power=None, voltage=None):
+    def __init__(self, target, target_name=None, interface=None, probe_id=None,
+                 tool_path=None, power=None, voltage=None, ignore_errors=False):
         """ Set initial basic configuration params for OpenOCD """
         if interface:
             raise NotImplementedError
 
         super().__init__()
         self.inited = True
         self.server_proc = None  # TCL RPC server process
         self.openocd_cmd = ''    # command for OpenOCD configuration
         self.before_init, self.after_init = self._get_ocd_config(target)
         self.power = power
         self.voltage = voltage
+        self.ignore_errors = ignore_errors
 
         os_name = platform.system()  # current OS type
         # Set OpenOCD execution filename
         if os_name in self._supported_os_short_names.keys():
             self._os_short_name = self._supported_os_short_names[os_name]
         else:
             self.inited = False
@@ -328,42 +328,32 @@
         """From the OpenOCD output gets lines that are not in
         the previous result
         """
         previous_set = set(previous_lines)
         result = [x for x in current_lines if x not in previous_set]
         return result
 
-    @staticmethod
-    def _ocd_start_result(lines):
+    def _ocd_start_result(self, lines):
         """Analyzes OpenOCD output and returns the result of the start"""
         for line in lines:
             if 'Error' in line:
                 logger.error(line.rstrip())
-                return False
+                if not self.ignore_errors:
+                    return False
             logger.info(line.rstrip())
             if 'Listening on port' in line:
                 return True
         return False
 
     def stop(self):
-        """
-        This command stops the local OpeOCD server.
-        :return: None
-        """
+        """This command stops the local OpenOCD server"""
         if self.server_proc is not None:
-            timeout = 1  # seconds
+            timeout_sec = 1
             self.server_proc.kill()
             start_time = time.time()
             while self.server_proc.poll() is None:
-                if time.time() - start_time > timeout:
+                if time.time() - start_time > timeout_sec:
                     break
             self.server_proc = None
 
-    def _kill_all(self):
-        """ This command kill all OpeOCD processes """
-        openocd_proc_name = self.openocd_exec_file
-        for proc in psutil.process_iter():
-            if proc.name() == openocd_proc_name:
-                proc.kill()
-
     def __del__(self):
         self.stop()
```

### Comparing `cysecuretools-4.1.0/cysecuretools/execute/programmer/openocd_target_map.json` & `cysecuretools-4.2.0/cysecuretools/execute/programmer/openocd_target_map.json`

 * *Files identical despite different names*

### Comparing `cysecuretools-4.1.0/cysecuretools/execute/programmer/openocd_wrapper.py` & `cysecuretools-4.2.0/cysecuretools/execute/programmer/openocd_wrapper.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-Copyright 2022 Cypress Semiconductor Corporation (an Infineon company)
+Copyright 2022-2023 Cypress Semiconductor Corporation (an Infineon company)
 or an affiliate of Cypress Semiconductor Corporation. All rights reserved.
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
@@ -72,32 +72,30 @@
 
     @wait_for_target.setter
     def wait_for_target(self, value):
         """
         N/A for OpenOCD
         """
 
-    def connect(self, target_name=None,
-                interface=None, probe_id=None, ap='cm4', acquire=None,
-                blocking=None, reset_and_halt=False,
-                power=None, voltage=None):
+    def connect(self, target_name=None, interface=None, probe_id=None,
+                ap='sysap', acquire=None, blocking=None, power=None,
+                voltage=None, ignore_errors=False):
         """
         Connects to target using default debug interface.
-        :param power: Indicates whether to on/off the KitProg3 power
-        :param voltage: The KitProg3 voltage level
-        :param target_name: The target name.
-        :param interface: Debug interface.
-        :param probe_id: Probe serial number.
-        :param ap: The access port to be used for flash operations
-        :param acquire: Indicates whether to acquire device on connect
-        :param blocking: Specifies whether to wait for a probe to be
+        @param target_name: The target name.
+        @param interface: Debug interface.
+        @param probe_id: Probe serial number.
+        @param ap: The access port to be used for flash operations
+        @param acquire: Indicates whether to acquire device on connect
+        @param blocking: Specifies whether to wait for a probe to be
                connected if there are no available probes.
-        :param reset_and_halt: Indicates whether to do reset and halt
-               after connect
-        :return: True if connected successfully, otherwise False.
+        @param power: Indicates whether to on/off the KitProg3 power
+        @param voltage: The KitProg3 voltage level
+        @param ignore_errors: Ignore errors and continue execution
+        @return: True if connected successfully, otherwise False.
         """
         if interface:
             raise NotImplementedError
 
         if target_name:
             ocd_target_name = ''
             # Search for device in target map
@@ -105,16 +103,16 @@
                 file_content = f.read()
                 json_data = json.loads(file_content)
             for json_target in json_data:
                 if target_name.lower().strip() == json_target.lower().strip():
                     # Get target info
                     director = TargetDirector()
                     try:
-                        from cysecuretools.targets import target_map
-                        director.builder = target_map[target_name]['class']()
+                        from cysecuretools.targets import target_data
+                        director.builder = target_data(target_name)['class']()
                     except KeyError as e:
                         raise ValueError(
                             f'Unknown target "{target_name}"') from e
                     self.target = director.get_target(None, target_name, None)
                     # Get target name which is relevant to OpenOCD
                     ocd_target_name = json_data[json_target]['target']
                     self.mcu = json_data[json_target]['mcu']
@@ -137,18 +135,18 @@
         # Register the signal handlers
         # When TERMINATE or INT signal from the system will be received,
         # the OCD server will be stopped
         signal.signal(signal.SIGTERM, self._terminate_signal_received)
         signal.signal(signal.SIGINT, self._terminate_signal_received)
 
         # Configure OpenOCD server
-        self.ocd_server = OpenocdServer(self.target, ocd_target_name,
-                                        interface, probe_id,
-                                        tool_path=self.tool_path,
-                                        power=power, voltage=voltage)
+        self.ocd_server = OpenocdServer(
+            self.target, ocd_target_name, interface, probe_id,
+            tool_path=self.tool_path, power=power, voltage=voltage,
+            ignore_errors=ignore_errors)
         self.probe_id = self.ocd_server.probe_id
         # Start GDB server and check if it is started
         server_started = self.ocd_server.start(ap, acquire)
         # No need of further connection if the power command is sent
         if power:
             return server_started
         if server_started:
@@ -156,21 +154,14 @@
             if self.sock is None:
                 self.sock = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
                 self.sock.connect((self.tcp_host_address, self.tcp_host_port))
             else:
                 raise ValueError('Debug session has already initialized')
         else:
             return False
-        self.set_ap(self.connect_ap)
-        self.examine_ap()
-        if reset_and_halt:
-            self.reset_and_halt(reset_type=ResetType.HW)
-        if self.current_ap in [AP.CM0, AP.CM4]:
-            self._start_core()
-            self.set_ap(AP.SYS)
 
         return True
 
     def disconnect(self):
         """
         Closes active connection.
         """
@@ -180,15 +171,15 @@
         self.sock.close()
         self.sock = None
         self.ocd_server.stop()
 
     def set_frequency(self, value_khz):
         """
         Sets probe frequency.
-        :param value_khz: Frequency in kHz.
+        @param value_khz: Frequency in kHz.
         """
         if self.sock is None:
             raise ValueError('Debug probe is not initialized')
         self._send('adapter_khz {0}'.format(value_khz))
 
     def halt(self):
         """
@@ -207,155 +198,155 @@
             raise ValueError('Target is not initialized')
         logger.debug('resume')
         self._send('resume')
 
     def reset(self, reset_type=ResetType.SW):
         """
         Resets the target.
-        :param reset_type: The reset type.
+        @param reset_type: The reset type.
         """
         if self.sock is None:
             raise ValueError('Target is not initialized')
         logger.debug('reset')
         self._send('reset run')
 
     def reset_and_halt(self, reset_type=ResetType.SW):
         """
         Resets the target and halts the CPU immediately after reset.
-        :param reset_type: The reset type.
+        @param reset_type: The reset type.
         """
         if self.sock is None:
             raise ValueError('Target is not initialized')
         logger.debug('reset_and_halt')
         self._send('reset init')
 
     def read8(self, address):
         """
         Reads 8-bit value from specified memory location.
-        :param address: The memory address to read.
-        :return: The read value.
+        @param address: The memory address to read.
+        @return: The read value.
         """
         if self.sock is None:
             raise ValueError('Target is not initialized')
         cmd_rsp = self._send('mdb 0x{0:x}'.format(address))
         value = self._parse_and_convert_read(cmd_rsp)
         logger.debug('read8 (0x%x): 0x%x', address, value)
         return value
 
     def read16(self, address):
         """
         Reads 16-bit value from specified memory location.
-        :param address: The memory address to read.
-        :return: The read value.
+        @param address: The memory address to read.
+        @return: The read value.
         """
         if self.sock is None:
             raise ValueError('Target is not initialized')
         if (address & 0x01) == 0:
             cmd_rsp = self._send('mdh 0x{0:x}'.format(address))
             value = self._parse_and_convert_read(cmd_rsp)
             logger.debug('read16 (0x%x): 0x%x', address, value)
             return value
         else:
             raise ValueError('Address not aligned')
 
     def read32(self, address):
         """
         Reads 32-bit value from specified memory location.
-        :param address: The memory address to read.
-        :return: The read value.
+        @param address: The memory address to read.
+        @return: The read value.
         """
         if self.sock is None:
             raise ValueError('Target is not initialized')
         if (address & 0x03) == 0:
             cmd_rsp = self._send('mdw 0x{0:x}'.format(address))
             value = self._parse_and_convert_read(cmd_rsp)
             logger.debug('read32 (0x%x): 0x%x', address, value)
             return value
         else:
             raise ValueError('Address not aligned')
 
     def write8(self, address, value):
         """
         Writes 8-bit value by specified memory location.
-        :param address: The memory address to write.
-        :param value: The 8-bit value to write.
+        @param address: The memory address to write.
+        @param value: The 8-bit value to write.
         """
         if self.sock is None:
             raise ValueError('Target is not initialized.')
         logger.debug('write8 (0x%x): 0x%x', address, value)
         data = self._send('mwb 0x{0:x} 0x{1:x}'.format(address, value))
         return data
 
     def write16(self, address, value):
         """
         Writes 16-bit value by specified memory location.
-        :param address: The memory address to write.
-        :param value: The 16-bit value to write.
+        @param address: The memory address to write.
+        @param value: The 16-bit value to write.
         """
         if self.sock is None:
             raise ValueError('Target is not initialized')
         logger.debug('write16 (0x%x): 0x%x', address, value)
         data = self._send('mwh 0x{0:x} 0x{1:x}'.format(address, value))
         return data
 
     def write32(self, address, value):
         """
         Writes 32-bit value by specified memory location.
-        :param address: The memory address to write.
-        :param value: The 32-bit value to write.
+        @param address: The memory address to write.
+        @param value: The 32-bit value to write.
         """
         self._send('targets')
         if self.sock is None:
             raise ValueError('Target is not initialized')
         logger.debug('write32 (0x%x): 0x%x', address, value)
         data = self._send('mww 0x{0:x} 0x{1:x}'.format(address, value))
         return data
 
     def read_reg(self, reg_name):
         """
         Gets value of a core register.
-        :param reg_name: Core register name.
-        :return: The register value.
+        @param reg_name: Core register name.
+        @return: The register value.
         """
         reg = reg_name.lower()
         value = self._send('reg {0}'.format(reg))
         logger.debug('read_reg (%s): 0x%x', reg, value)
         return value
 
     def write_reg(self, reg_name, value):
         """
         Sets value of a core register.
-        :param reg_name: Core register name.
-        :param value: The value to set.
-        :return: The register value.
+        @param reg_name: Core register name.
+        @param value: The value to set.
+        @return: The register value.
         """
         reg = reg_name.lower()
         logger.debug('write_reg (%s): 0x%x', reg, value)
         self._send('reg {0} {1:#x}'.format(reg, value))
 
     def erase(self, address, size):
         """
         Erases entire device flash or specified sectors.
-        :param address: The memory location.
-        :param size: The memory size.
+        @param address: The memory location.
+        @param size: The memory size.
         """
         if self.sock is None:
             raise ValueError('Debug session is not initialized')
         self.halt()
         logger.debug('erase 0x%x-0x%x', address, address + size)
         self._send('flash erase_address {0} {1}'.format(address, size))
 
     def program(self, filename, file_format=None, address=None):
         """
         Programs a file into flash.
-        :param filename: Path to a file.
-        :param file_format: N/A for OpenOCD.
-        :param address: Base address used for the address where to
+        @param filename: Path to a file.
+        @param file_format: N/A for OpenOCD.
+        @param address: Base address used for the address where to
                flash a binary.
-        :return: True if programmed successfully, otherwise False.
+        @return: True if programmed successfully, otherwise False.
         """
         if self.sock is None:
             raise ValueError('Debug session is not initialized')
         # Remove Windows-style path separator
         filename = filename.replace(os.sep, '/')
         self.halt()
         if address:
@@ -364,19 +355,19 @@
         else:
             logger.debug("Programming '%s'", filename)
             self._send(f'flash write_image erase "{filename}"')
 
     def program_ram(self, filename, file_format=None, address=None):
         """
         Programs a file into flash.
-        :param filename: Path to a file.
-        :param file_format: N/A for OpenOCD.
-        :param address: Base address used for the address where to
+        @param filename: Path to a file.
+        @param file_format: N/A for OpenOCD.
+        @param address: Base address used for the address where to
                flash a binary.
-        :return: True if programmed successfully, otherwise False.
+        @return: True if programmed successfully, otherwise False.
         """
         if self.sock is None:
             raise ValueError('Debug session is not initialized')
         # Remove Windows-style path separator
         filename = filename.replace(os.sep, '/')
         self.halt()
         if address:
@@ -385,43 +376,43 @@
         else:
             logger.debug("Programming '%s'", filename)
             self._send(f'load_image "{filename}"')
 
     def _parse_read(self, cmd_response):
         """
         Parse OpenOCD output from read memory commands
-        :param cmd_response: String with response from server to the
+        @param cmd_response: String with response from server to the
                read command
-        :return: The register as integer value
+        @return: The register as integer value
         """
         for err_msg in self._error_msg_patterns:
             if err_msg in cmd_response:
                 logger.error("Unable to get data from the memory")
                 return self._CMD_FAIL
         cmd_result = cmd_response.split(':')
         value = cmd_result[1].strip()
         return value
 
     def _parse_and_convert_read(self, cmd_response):
         """
         Parse OpenOCD output from read memory commands
-        :param cmd_response: String with response from server to the
+        @param cmd_response: String with response from server to the
                read command
-        :return: The register as integer value
+        @return: The register as integer value
         """
         value = self._parse_read(cmd_response)
         value = int(value, 16)
         return value
 
     def _send(self, cmd):
         """
         Send a command to TCL RPC.
         Note: This command also check command status and if it is not SUCCESS raise ValueError exception
-        :param cmd: String with command for OpenOCD server.
-        :return: String with response on sent command to the server.
+        @param cmd: String with command for OpenOCD server.
+        @return: String with response on sent command to the server.
         """
         if self.sock is None:
             raise ValueError('Debug session is not initialized')
             # Stop OpenOCD server if termination signal was received
 
         if self.verbose:
             logger.info('send -> %s', cmd)
@@ -445,61 +436,61 @@
         if cmd_message:
             logger.debug(cmd_message)
         return cmd_message
 
     def _send_cmd(self, cmd):
         """
         Send a command string to TCL RPC.
-        :param cmd: String with command for OpenOCD server.
-        :return: String with response on sent command.
+        @param cmd: String with command for OpenOCD server.
+        @return: String with response on sent command.
         """
         data = (cmd + self._command_token).encode("utf-8")
         self.sock.send(data)
         return self._receive()
 
     def _receive(self):
         """
         Read from the stream until the token (\x1a) was received.
-        :return: String with response on sent command to the server.
+        @return: String with response on sent command to the server.
         """
         data = bytes()
         while True:
             chunk = self.sock.recv(self.sock_buffer_size)
             data += chunk
             if bytes(self._command_token, encoding="utf-8") in chunk:
                 break
         data = data.decode("utf-8").strip()
         data = data[:-1]  # strip trailing command token \x1a
         if self.verbose:
             logger.info('receive -> %s', data)
         return data
 
-    def _terminate_signal_received(self, **_):
+    def _terminate_signal_received(self, *_args):
         """
         The termination signal from the system was received
         """
         if logger is not None:
             logger.info('The termination signal from the system was received')
         if self.sock is not None:
             self.sock.close()
         self.ocd_server.stop()
         sys.exit(0)
 
     def get_ap(self):
         """
         Gets access port.
-        :return: Selected AP.
+        @return: Selected AP.
         """
         logger.debug('AP: %s', self.current_ap)
         return self.current_ap
 
     def set_ap(self, ap):
         """
         Sets access port.
-        :param ap: The AP name.
+        @param ap: The AP name.
         """
         if ap == AP.CM0:
             logger.debug('Use cm0 AP')
             self._send(f'targets {self.mcu}.cm0')
         elif ap == AP.CM4:
             logger.debug('Use cm4 AP')
             self._send(f'targets {self.mcu}.cm4')
@@ -521,29 +512,48 @@
             self._send(f'targets {self.mcu}.sysap')
         self._send('targets')
         self.current_ap = ap
 
     def read(self, address, length):
         """
         Reads a block of unaligned bytes in memory
-        :param address: The memory address where start reading
-        :param length: Number of bytes to read
-        :return: An array of byte values
-        """
-        cmd = 'read_memory 0x{0:x} 8 {1}'.format(address, length)
-        logger.debug(cmd)
-        response = self._send(cmd)
-        value = [int(i, 16) for i in response.split()]
-        return value
+        @param address: The memory address where start reading
+        @param length: Number of bytes to read
+        @return: An array of byte values
+        """
+        def read_memory(addr, size):
+            cmd = 'read_memory 0x{0:x} 8 {1}'.format(addr, size)
+            logger.debug(cmd)
+            response = self._send(cmd)
+            value = [int(i, 16) for i in response.split()]
+            return value
+
+        # The maximum length limit of the 'read_memory' command is 64K
+        # elements. For better performance, the maximum chunk size is 20K
+        data = []
+        max_size = 0x5000
+        if length > max_size:
+            read_address = address
+            while len(data) < length:
+                if len(data) + max_size > length:
+                    read_size = length - len(data)
+                else:
+                    read_size = max_size
+                data.extend(read_memory(read_address, read_size))
+                read_address += read_size
+        else:
+            data = read_memory(address, length)
+
+        return data
 
     def write(self, address, data):
         """
         Write a block of unaligned bytes in memory
-        :param address: The memory address where start writing
-        :param data: An array of byte values
+        @param address: The memory address where start writing
+        @param data: An array of byte values
         """
         if self.sock is None:
             raise ValueError('Target is not initialized.')
 
         if isinstance(data, list) and all(isinstance(i, int) for i in data):
             value = ' '.join([hex(i) for i in data])
         elif isinstance(data, (bytes, bytearray)):
@@ -580,15 +590,15 @@
         elif self.connect_ap == AP.SYS:
             ap = 'sysap'
 
         self._send(f'{self.mcu}.{ap} arp_examine')
 
     def get_voltage(self):
         """Reads target voltage
-        :@return Voltage value in Volts
+        @return Voltage value in Volts
         """
         if self.sock is None:
             raise ValueError('Target is not initialized')
 
         if self.ocd_server.probe_interface == 'kitprog3':
             logger.debug('kitprog3 get_power')
             response = self._send('kitprog3 get_power')
```

### Comparing `cysecuretools-4.1.0/cysecuretools/execute/programmer/programmer.py` & `cysecuretools-4.2.0/cysecuretools/execute/programmer/programmer.py`

 * *Files identical despite different names*

### Comparing `cysecuretools-4.1.0/cysecuretools/execute/programmer/pyocd_target_map.json` & `cysecuretools-4.2.0/cysecuretools/execute/programmer/pyocd_target_map.json`

 * *Files identical despite different names*

### Comparing `cysecuretools-4.1.0/cysecuretools/execute/programmer/pyocd_wrapper.py` & `cysecuretools-4.2.0/cysecuretools/execute/programmer/pyocd_wrapper.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-Copyright 2019-2022 Cypress Semiconductor Corporation (an Infineon company)
+Copyright 2019-2023 Cypress Semiconductor Corporation (an Infineon company)
 or an affiliate of Cypress Semiconductor Corporation. All rights reserved.
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
@@ -53,30 +53,29 @@
         """
         Sets a value indicating whether to wait for the target
         if no available devices are connected
         """
         self._wait_for_target = value
 
     def connect(self, target_name=None, interface=None, probe_id=None,
-                ap='cm4', acquire=None, blocking=True, reset_and_halt=False,
-                power=None, voltage=None):
+                ap='sysap', acquire=None, blocking=True, power=None,
+                voltage=None, ignore_errors=False):
         """
         Connects to target using default debug interface.
-        :param target_name: The target name.
-        :param interface: Debug interface.
-        :param ap: The access port used for communication (cm0 or cm4).
-        :param probe_id: Probe serial number.
-        :param acquire: Indicates whether to acquire device on connect
-        :param blocking: Specifies whether to wait for a probe to be
+        @param target_name: The target name.
+        @param interface: Debug interface.
+        @param probe_id: Probe serial number.
+        @param ap: The access port to be used for flash operations
+        @param acquire: Indicates whether to acquire device on connect
+        @param blocking: Specifies whether to wait for a probe to be
                connected if there are no available probes.
-        :param reset_and_halt: Indicates whether to do reset and halt
-               after connect
-        :param power: N/A for PyOCD
-        :param voltage: N/A for PyOCD
-        :return: True if connected successfully, otherwise False.
+        @param power: Indicates whether to on/off the KitProg3 power
+        @param voltage: The KitProg3 voltage level
+        @param ignore_errors: Ignore errors and continue execution
+        @return: True if connected successfully, otherwise False.
         """
         if interface:
             raise NotImplementedError
         else:
             if target_name:
                 logger.info('Target: %s', target_name)
                 # Search for device in target map
@@ -106,17 +105,14 @@
             self.board = self.session.board
             self.session.open()
 
             self.target = self.board.target
             self.probe = self.session.probe
             self.probe_id = self.probe.unique_id
 
-            if reset_and_halt:
-                self.reset_and_halt(reset_type=ResetType.HW)
-
             self.ap = ap
             self.set_ap(AP.SYS)
             logger.info('Probe ID: %s', self.probe.unique_id)
             return True
 
     def disconnect(self):
         """ Closes the active connection. """
@@ -170,52 +166,47 @@
                 else:
                     raise e
         logger.debug('disconnect::exit')
 
     def get_ap(self):
         """
         Gets access port.
-        :return: Selected AP.
+        @return: Selected AP.
         """
         if self.target.selected_core == self.target.cores[0]:
             ap = AP.SYS
         elif self.target.selected_core == self.target.cores[1]:
             ap = AP.CMx
         logger.debug('AP: %s', ap)
         return ap
 
     def set_ap(self, ap):
         """
         Sets access port.
-        :param ap: The AP name.
+        @param ap: The AP name.
         """
         if ap == AP.SYS:
             logger.debug('Use system AP')
-            if self.get_ap() != AP.SYS:
-                self._start_core()
             self.target.selected_core = 0
         elif ap == AP.CM0:
             logger.debug('Use cm0 AP')
             self.target.selected_core = 1
-            self._start_core()
         elif ap == AP.CM4:
             logger.debug('Use cm4 AP')
             self.target.selected_core = 1
-            self._start_core()
         elif ap == AP.CMx:
             logger.debug('Use %s AP', self.ap)
             self.target.selected_core = 1
-            self._start_core()
         else:
             raise ValueError('Invalid access port.')
 
     def set_frequency(self, value_khz):
         """
         Sets probe frequency.
-        :param value_khz: Frequency in kHz.
+        @param value_khz: Frequency in kHz.
         """
         if self.probe is None:
             raise ValueError('Debug probe is not initialized.')
         self.probe.set_clock(value_khz * 1000)
 
     def halt(self):
         """
@@ -234,184 +225,184 @@
             raise ValueError('Target is not initialized.')
         logger.debug('resume')
         self.target.resume()
 
     def reset(self, reset_type=ResetType.SW):
         """
         Resets the target.
-        :param reset_type: The reset type.
+        @param reset_type: The reset type.
         """
         if self.target is None:
             raise ValueError('Target is not initialized.')
         logger.debug('reset (%s)', reset_type)
         self.target.reset(reset_type=self._pyocd_reset_type(reset_type))
 
     def reset_and_halt(self, reset_type=ResetType.SW):
         """
         Resets the target and halts the CPU immediately after reset.
-        :param reset_type: The reset type.
+        @param reset_type: The reset type.
         """
         if self.target is None:
             raise ValueError('Target is not initialized.')
         logger.debug('reset_and_halt (%s)', reset_type)
         self.target.reset_and_halt(reset_type=self._pyocd_reset_type(
             reset_type))
 
     def read8(self, address):
         """
         Reads 8-bit value from specified memory location.
-        :param address: The memory address to read.
-        :return: The read value.
+        @param address: The memory address to read.
+        @return: The read value.
         """
         if self.target is None:
             raise ValueError('Target is not initialized.')
         data = self.target.read_memory(address, transfer_size=8)
         logger.debug('read8 (0x%x): 0x%x', address, data)
         return data
 
     def read16(self, address):
         """
         Reads 16-bit value from specified memory location.
-        :param address: The memory address to read.
-        :return: The read value.
+        @param address: The memory address to read.
+        @return: The read value.
         """
         if self.target is None:
             raise ValueError('Target is not initialized.')
         if (address & 0x01) == 0:
             data = self.target.read_memory(address, transfer_size=16)
             logger.debug('read16 (0x%x): 0x%x', address, data)
             return data
         else:
             raise ValueError('Address not aligned.')
 
     def read32(self, address):
         """
         Reads 32-bit value from specified memory location.
-        :param address: The memory address to read.
-        :return: The read value.
+        @param address: The memory address to read.
+        @return: The read value.
         """
         if self.target is None:
             raise ValueError('Target is not initialized.')
         if (address & 0x03) == 0:
             data = self.target.read_memory(address, transfer_size=32)
             logger.debug('read32 (0x%x): 0x%x', address, data)
             return data
         else:
             raise ValueError('Address not aligned.')
 
     def write8(self, address, value):
         """
         Writes 8-bit value by specified memory location.
-        :param address: The memory address to write.
-        :param value: The 8-bit value to write.
+        @param address: The memory address to write.
+        @param value: The 8-bit value to write.
         """
         if self.target is None:
             raise ValueError('Target is not initialized.')
         logger.debug('write8 (0x%x): 0x%x', address, value)
         data = self.target.write_memory(address, value, transfer_size=8)
         return data
 
     def write16(self, address, value):
         """
         Writes 16-bit value by specified memory location.
-        :param address: The memory address to write.
-        :param value: The 16-bit value to write.
+        @param address: The memory address to write.
+        @param value: The 16-bit value to write.
         """
         if self.target is None:
             raise ValueError('Target is not initialized.')
         logger.debug('write16 (0x%x): 0x%x', address, value)
         data = self.target.write_memory(address, value, transfer_size=16)
         return data
 
     def write32(self, address, value):
         """
         Writes 32-bit value by specified memory location.
-        :param address: The memory address to write.
-        :param value: The 32-bit value to write.
+        @param address: The memory address to write.
+        @param value: The 32-bit value to write.
         """
         if self.target is None:
             raise ValueError('Target is not initialized.')
         logger.debug('write32 (0x%x): 0x%x', address, value)
         data = self.target.write_memory(address, value, transfer_size=32)
         return data
 
     def read_reg(self, reg_name):
         """
         Gets value of a core register.
-        :param reg_name: Core register name.
-        :return: The register value.
+        @param reg_name: Core register name.
+        @return: The register value.
         """
         reg = reg_name.lower()
         value = self.target.read_core_register(reg)
         logger.debug('read_reg (%s): 0x%x', reg_name, value)
         return value
 
     def write_reg(self, reg_name, value):
         """
         Sets value of a core register.
-        :param reg_name: Core register name.
-        :param value: The value to set.
-        :return: The register value.
+        @param reg_name: Core register name.
+        @param value: The value to set.
+        @return: The register value.
         """
         reg = reg_name.lower()
         logger.debug('write_reg (%s): 0x%x', reg_name, value)
         self.target.write_core_register(reg, value)
 
     def erase(self, address, size):
         """
         Erases entire device flash or specified sectors.
-        :param address: The memory location.
-        :param size: The memory size.
+        @param address: The memory location.
+        @param size: The memory size.
         """
         region = self.session.target.memory_map.get_region_for_address(address)
         if not region:
             raise ValueError('Address 0x%08x is not within a memory region.' % address)
         if not region.is_flash:
             raise ValueError('Address 0x%08x is not in flash.' % address)
         eraser = FlashEraser(self.session, FlashEraser.Mode.SECTOR)
         address_range = f"{hex(address)}-{hex(address + size)}"
         logger.debug('erase %s', address_range)
         eraser.erase([address_range])
 
     def program(self, filename, file_format=None, address=None):
         """
         Programs a file into flash.
-        :param filename: Path to a file.
-        :param file_format: File format. Default is to use the file's
+        @param filename: Path to a file.
+        @param file_format: File format. Default is to use the file's
                extension.
-        :param address: Base address used for the address where to
+        @param address: Base address used for the address where to
                flash a binary.
-        :return: True if programmed successfully, otherwise False.
+        @return: True if programmed successfully, otherwise False.
         """
         if self.session is None:
             raise ValueError('Debug session is not initialized.')
         programmer = FileProgrammer(self.session, chip_erase='sector')
         logger.debug('program %s', filename)
         programmer.program(filename, base_address=address,
                            file_format=file_format)
 
     def read(self, address, length):
         """
         Reads a block of unaligned bytes in memory
-        :param address: The memory address where start reading
-        :param length: Number of bytes to read
-        :return: An array of byte values
+        @param address: The memory address where start reading
+        @param length: Number of bytes to read
+        @return: An array of byte values
         """
         if self.target is None:
             raise ValueError('Target is not initialized.')
         data = self.target.read_memory_block8(address, length)
         logger.debug('Read block (address=0x%x, length=%s): %s',
                      address, length, data)
         return data
 
     def write(self, address, data):
         """
         Writes a block of unaligned bytes in memory
-        :param address: The memory address where start writing
-        :param data: An array of byte values
+        @param address: The memory address where start writing
+        @param data: An array of byte values
         """
         if self.target is None:
             raise ValueError('Target is not initialized.')
         self.target.write_memory_block8(address, data)
         logger.debug('Write block (address=0x%x): %s', address, data)
 
     @staticmethod
@@ -420,29 +411,29 @@
         Gets list of all connected probes
         """
         return ConnectHelper.get_all_connected_probes(blocking=False)
 
     def set_skip_reset_and_halt(self, value):
         """
         Sets skip_reset_and_halt property value
-        :param value: Indicates whether to skip or not
+        @param value: Indicates whether to skip or not
         """
         for i in range(len(self.target.cores)):
             logger.debug('core #%d, skip_reset_and_halt = %s', i, value)
             self.target.cores[i].skip_reset_and_halt = value
 
     def examine_ap(self):
         """
         N/A for pyOCD
         """
 
     def _set_acquire_timeout(self, timeout):
         """
         Sets acquire_timeout property value
-        :param timeout: Timeout in seconds
+        @param timeout: Timeout in seconds
         """
         for i in range(len(self.target.cores)):
             self.target.cores[i].acquire_timeout = timeout
 
     @staticmethod
     def _pyocd_reset_type(reset_type: ResetType):
         """ Maps internal ResetType value to the pyocd ResetType value """
```

### Comparing `cysecuretools-4.1.0/cysecuretools/execute/project_init/project_init_mxs40sv2.py` & `cysecuretools-4.2.0/cysecuretools/execute/project_init/project_init_mxs40sv2.py`

 * *Files identical despite different names*

### Comparing `cysecuretools-4.1.0/cysecuretools/execute/project_init/project_init_mxs40v1.py` & `cysecuretools-4.2.0/cysecuretools/execute/project_init/project_init_mxs40v1.py`

 * *Files identical despite different names*

### Comparing `cysecuretools-4.1.0/cysecuretools/execute/provisioning/flows/application_mxs40sv2.py` & `cysecuretools-4.2.0/cysecuretools/execute/provisioning/flows/application_mxs40sv2.py`

 * *Files identical despite different names*

### Comparing `cysecuretools-4.1.0/cysecuretools/execute/provisioning/flows/flow_mxs40sv2.py` & `cysecuretools-4.2.0/cysecuretools/execute/provisioning/flows/flow_mxs40sv2.py`

 * *Files identical despite different names*

### Comparing `cysecuretools-4.1.0/cysecuretools/execute/provisioning/load_ram_app.py` & `cysecuretools-4.2.0/cysecuretools/execute/provisioning/load_ram_app.py`

 * *Files identical despite different names*

### Comparing `cysecuretools-4.1.0/cysecuretools/execute/provisioning/provision_device_mxs40sv2.py` & `cysecuretools-4.2.0/cysecuretools/execute/provisioning/provision_device_mxs40sv2.py`

 * *Files 2% similar despite different names*

```diff
@@ -102,17 +102,16 @@
                          'lifecycle stage')
 
         return status
 
     def erase_flash(self, tool, target):
         """ N/A. The target does not have flash """
 
-    def convert_to_rma(self, tool, target, **kwargs):
+    def transit_to_rma(self, tool, target, cert, **kwargs):
         """ Converts a part to the RMA LCS """
-        cert = kwargs.get('cert')
         test_pkg_type = kwargs.get('testapps')
 
         flow_parser = FlowParser(target, test_pkg_type=test_pkg_type)
         apps = flow_parser.apps_by_flow('rma')
         if not apps:
             raise ValueError('RAM applications list is empty')
 
@@ -142,14 +141,18 @@
             logger.info('       TRANSITION TO RMA PASSED          ')
             logger.info('*****************************************\n')
         elif status == ProvisioningStatus.SKIPPED:
             logger.error('The device cannot be converted to RMA due to '
                          'invalid lifecycle stage')
         return status
 
+    def open_rma(self, tool, target, cert, **kwargs):
+        """Not implemented for MXS40Sv2 platform"""
+        raise NotImplementedError
+
     @staticmethod
     def _copy_rma_cert(cert, apps, apps_dir):
         for app_name in apps:
             app = ApplicationMXS40Sv2(app_name, apps_dir)
             cert = os.path.abspath(cert)
             if os.path.isfile(cert):
                 logger.debug("Copy '%s' into '%s'", cert, app.in_params_path)
```

### Comparing `cysecuretools-4.1.0/cysecuretools/execute/provisioning/provision_device_mxs40v1.py` & `cysecuretools-4.2.0/cysecuretools/execute/provisioning/provision_device_mxs40v1.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-Copyright (c) 2018-2021 Cypress Semiconductor Corporation
+Copyright (c) 2018-2023 Cypress Semiconductor Corporation
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
 
@@ -18,17 +18,17 @@
 import logging
 from time import sleep
 import cysecuretools.execute.provisioning_packet.provisioning_packet_mxs40v1 as prov_packet
 from cysecuretools.core.connect_helper import ConnectHelper
 from cysecuretools.core.target_director import Target
 from cysecuretools.core.enums import (EntranceExamStatus, ProvisioningStatus)
 from cysecuretools.execute.provisioning_packet.lib.cyprov_pem import PemKey
-from cysecuretools.execute.sys_call \
-    import (provision_keys_and_policies, read_lifecycle, dap_control,
-            get_prov_details, FB_POLICY_JWT)
+from cysecuretools.execute.sys_call import (
+    provision_keys_and_policies, read_lifecycle, dap_control, get_prov_details,
+    transition_to_rma, open_rma, FB_POLICY_JWT)
 from cysecuretools.execute.programmer.base import AP
 from cysecuretools.execute.programmer.pyocd_wrapper import ResetType
 from cysecuretools.core.strategy_context.provisioning_strategy_ctx import \
     ProvisioningStrategy
 from cysecuretools.core.strategy_context.encrypted_programming_strategy_ctx \
     import EncryptedProgrammingContext
 from cysecuretools.execute.encrypted_programming.aes_header_strategy import \
@@ -40,32 +40,26 @@
 from cysecuretools.execute.provisioning_packet.lib import Crypto
 
 logger = logging.getLogger(__name__)
 
 
 class ProvisioningMXS40v1(ProvisioningStrategy):
 
-    def provision(self, tool,
-                  target: Target, bootloader, **kwargs) -> ProvisioningStatus:
+    def provision(self, tool, target: Target, bootloader,
+                  **kwargs) -> ProvisioningStatus:
         """
         Programs Cypress Bootloader and calls system calls for device
         provisioning.
         :param tool: Programming/debugging tool used for communication
         :param target: The target object.
         :param bootloader: Path to Cypress Bootloader program file.
         :param kwargs: Dictionary with the following fields:
-               - ap: Access port to use
                - probe_id: Probe ID to use
         :return: Provisioning status.
         """
-        if 'ap' in kwargs:
-            ap = kwargs['ap']
-        else:
-            ap = 'cm0'
-
         if 'skip_prompts' in kwargs:
             skip_prompts = kwargs['skip_prompts']
         else:
             skip_prompts = None
 
         if 'probe_id' in kwargs:
             probe_id = kwargs['probe_id']
@@ -75,64 +69,56 @@
         prov_packets = self._get_provisioning_packet(target)
         status = _provision_identity(
             tool, target, prov_packets['prov_identity'], skip_prompts)
 
         if status == ProvisioningStatus.OK:
             status = _provision_complete(tool, target,
                                          prov_packets['prov_cmd'], bootloader,
-                                         False, ap=ap, probe_id=probe_id)
+                                         False, ap='cm4', probe_id=probe_id)
 
         if status == ProvisioningStatus.OK:
             logger.info('*****************************************')
             logger.info('       PROVISIONING PASSED               ')
             logger.info('*****************************************\n')
 
         return status
 
-    def re_provision(self, tool, target: Target, bootloader, **kwargs) \
-            -> ProvisioningStatus:
+    def re_provision(self, tool, target: Target, bootloader,
+                     **kwargs) -> ProvisioningStatus:
         """
         Programs Cypress Bootloader and calls system calls for device
         provisioning.
         :param tool: Programming/debugging tool used for communication
         :param target: The target object.
         :param bootloader: Path to Cypress Bootloader program file.
         :param kwargs: Dictionary with the following fields:
                - erase_boot: Indicates whether to erase BOOT slot
                - control_dap_cert: Certificate for AP control
-               - ap: Access port to use
-               - probe_id: Probe ID to use
         :return: Provisioning status.
         """
-        # Process keyword arguments
         if 'erase_boot' in kwargs:
             erase_boot = kwargs['erase_boot']
         else:
             erase_boot = False
 
         if 'control_dap_cert' in kwargs:
             control_dap_cert = kwargs['control_dap_cert']
         else:
             control_dap_cert = None
 
-        if 'ap' in kwargs:
-            ap = kwargs['ap']
-        else:
-            ap = 'cm0'
-
         if 'probe_id' in kwargs:
             probe_id = kwargs['probe_id']
         else:
             probe_id = None
 
         prov_packets = self._get_re_provisioning_packet(target)
-        tool.reset_and_halt(ResetType.HW)
         status = _provision_complete(
             tool, target, prov_packets['prov_cmd'], bootloader, True,
-            erase_boot, control_dap_cert, ap, probe_id)
+            erase_boot=erase_boot, control_dap_cert=control_dap_cert,
+            probe_id=probe_id)
 
         if status == ProvisioningStatus.OK:
             logger.info('*****************************************')
             logger.info('       RE-PROVISIONING PASSED               ')
             logger.info('*****************************************\n')
 
         return status
@@ -141,17 +127,54 @@
         """
         Erases allowed (w/o bootloader, data only) flash area
         :param tool: Programming/debugging tool used for communication
         :param target: The target object
         """
         erase_flash(tool, target)
 
-    def convert_to_rma(self, tool, target, **kwargs):
-        """ N/A for MXS40v1 platform """
-        raise NotImplementedError
+    def transit_to_rma(self, tool, target, cert, *_):
+        """Transits a part to the RMA LCS
+        @param tool: Programming/debugging tool used for communication
+        @param target: The target object
+        @param cert: JWT packet signed by the key mentioned in the debug/RMA
+                     section of the policy, with authentication object
+                     including valid DIE_ID range
+        """
+        if cert is None:
+            raise ValueError('Certificate not specified')
+        logger.info("Apply certificate '%s'", cert)
+        with open(cert, encoding='utf-8') as f:
+            cert_data = f.read()
+        if transition_to_rma(tool, target.memory_map, target.register_map,
+                             cert_data):
+            tool.reset()
+            logger.info('*****************************************')
+            logger.info('      TRANSITION TO RMA LCS PASSED       ')
+            logger.info('*****************************************\n')
+            return ProvisioningStatus.OK
+        return ProvisioningStatus.FAIL
+
+    def open_rma(self, tool, target, cert, **kwargs):
+        """Enables full access to device in RMA lifecycle stage
+        @param tool: Programming/debugging tool used for communication
+        @param target: The target object
+        @param cert: JWT packet signed by the key mentioned in the debug/RMA
+                     section of the policy, with authentication object
+                     including valid DIE_ID range
+        """
+        logger.info("Apply certificate '%s'", cert)
+        with open(cert, encoding='utf-8') as f:
+            cert_data = f.read()
+        if open_rma(tool, target.memory_map, target.register_map, cert_data):
+            logger.info('*****************************************')
+            logger.info('          FULL ACCESS ENABLED            ')
+            logger.info('        DO NOT RESET THE DEVICE          ')
+            logger.info('*****************************************\n')
+            return ProvisioningStatus.OK
+        return ProvisioningStatus.FAIL
 
     @staticmethod
     def _get_provisioning_packet(target):
         packet_dir = target.policy_parser.get_provisioning_packet_dir()
         prov_identity = os.path.join(packet_dir, prov_packet.PROV_IDENTITY_JWT)
         prov_cmd = os.path.join(packet_dir, prov_packet.PROV_CMD_JWT)
 
@@ -191,28 +214,30 @@
 
 def erase_flash(tool, target):
     logger.info('Erase main flash:')
     addr = target.memory_map.FLASH_ADDRESS
     size = target.memory_map.FLASH_SIZE
     logger.info('erasing address 0x%x, size 0x%x ...', addr, size)
     ap = tool.get_ap()
-    tool.set_ap(AP.CMx)
+    if ap == AP.SYS:
+        tool.set_ap(AP.CMx)
     tool.halt()
     tool.erase(addr, size)
     logger.info('Erasing complete')
     tool.set_ap(ap)
     erase_smif(tool, target)
 
 
 def erase_smif(tool, target):
     smif_resources = target.policy_parser.get_smif_resources()
     if len(smif_resources) > 0:
         logger.info('Erase main smif slots:')
         ap = tool.get_ap()
-        tool.set_ap(AP.CMx)
+        if ap == AP.SYS:
+            tool.set_ap(AP.CMx)
         for (addr, size) in smif_resources:
             # Aligning start address to erase to minimal erase size of smif
             actual_addr = addr - addr % target.memory_map.MIN_EXT_ERASE_SIZE
             # Aligning size to erase to minimal erase size of smif
             if size % target.memory_map.MIN_EXT_ERASE_SIZE == 0:
                 actual_size = size
             else:
@@ -226,28 +251,30 @@
 
 
 def erase_status_partition(tool, target):
     memory_area = target.policy_parser.status_partition()
     if memory_area is not None:
         logger.info('Erase SWAP status partition memory region:')
         ap = tool.get_ap()
-        tool.set_ap(AP.CMx)
+        if ap == AP.SYS:
+            tool.set_ap(AP.CMx)
         logger.info('erasing address 0x%x, size 0x%x ...',
                     memory_area.address, memory_area.size)
         tool.erase(memory_area.address, memory_area.size)
         logger.info('Erasing complete')
         tool.set_ap(ap)
 
 
 def erase_scratch_area(tool, target):
     memory_area = target.policy_parser.scratch_area()
     if memory_area is not None:
         logger.info('Erase SCRATCH memory region:')
         ap = tool.get_ap()
-        tool.set_ap(AP.CMx)
+        if ap == AP.SYS:
+            tool.set_ap(AP.CMx)
         logger.info('erasing address 0x%x, size 0x%x ...',
                     memory_area.address, memory_area.size)
         tool.erase(memory_area.address, memory_area.size)
         logger.info('Erasing complete')
         tool.set_ap(ap)
 
 
@@ -261,26 +288,28 @@
                        enough to prevent application from starting
     """
     data = target.policy_parser.get_image_data(slot_type)
     logger.info('Erase %s slot:', slot_type)
     for addr, size in data:
         logger.info('erasing address 0x%x, size 0x%x ...', addr, size)
         ap = tool.get_ap()
-        tool.set_ap(AP.CMx)
+        if ap == AP.SYS:
+            tool.set_ap(AP.CMx)
         tool.halt()
         tool.erase(addr, size)
         logger.info('Erasing complete')
         tool.set_ap(ap)
         if first_only:
             break
 
 
 def _provision_identity(tool, target: Target,
                         prov_identity_jwt, skip_prompts) -> ProvisioningStatus:
     lifecycle = read_lifecycle(tool, target.register_map)
+    tool.examine_ap()
 
     if lifecycle == ProtectionState.secure:
         status = target.entrance_exam.execute(tool)
         if status == EntranceExamStatus.FLASH_NOT_EMPTY:
             if skip_prompts:
                 logger.error('Cannot start provisioning. '
                              'User firmware running on chip detected')
@@ -307,28 +336,26 @@
         logger.error('Unexpected ProvisionKeysAndPolicies syscall response')
         return ProvisioningStatus.FAIL
     else:
         return ProvisioningStatus.OK
 
 
 def _provision_complete(tool, target: Target, prov_cmd_jwt, bootloader,
-                        re_provision, erase_boot=False,
-                        control_dap_cert=None, ap='cm0', probe_id=None) \
-        -> ProvisioningStatus:
+                        re_provision, erase_boot=False, control_dap_cert=None,
+                        probe_id=None, ap='cm0') -> ProvisioningStatus:
+    reg_map = target.register_map
     flash_ops_allowed = True
+
     if re_provision:
-        # Check whether cm0 is open
-        cm0_open = read_cm0_permissions(tool, target.register_map)
-        if cm0_open:
+        is_cm0_open = read_cm0_permissions(tool, reg_map)
+        if is_cm0_open:
             ConnectHelper.disconnect(tool)
-            ConnectHelper.connect(tool, target, probe_id=probe_id, ap='cm0')
-            tool.reset_and_halt(ResetType.HW)
-        flash_ops_allowed = cm0_open or ap == 'cm4'
-
-    reg_map = target.register_map
+            ConnectHelper.connect(tool, target, probe_id=probe_id, ap=ap)
+            tool.examine_ap()
+        flash_ops_allowed = is_cm0_open
 
     if flash_ops_allowed:
         erase_status_partition(tool, target)
         erase_scratch_area(tool, target)
 
     # Read firmware status
     logger.info('Read FlashBoot firmware status:')
@@ -345,27 +372,26 @@
     if expected != received:
         try:
             status = sfb_status_codes[received]
             logger.info('SFB status: %s: %s', status['status'], status['desc'])
         except KeyError:
             logger.debug('Unexpected SFB status 0x%x', received)
 
-    # Open cm0 AP
+    # Open cm0 AP with a certificate
     if control_dap_cert:
         logger.info('Opening cm0 AP')
-        cm_open = dap_control(tool, reg_map, 0, 1, False, control_dap_cert)
-        logger.info('cm0 AP %s', 'open' if cm_open else 'closed')
-        if cm_open:
-            logger.info('Use cm0 AP')
+        is_cm0_open = dap_control(tool, reg_map, 0, 1, False, control_dap_cert)
+        logger.info('cm0 AP %s', 'open' if is_cm0_open else 'closed')
+        if is_cm0_open:
             ConnectHelper.disconnect(tool)
             ConnectHelper.connect(tool, target, probe_id=probe_id, ap='cm0',
                                   acquire=False)
             tool.set_skip_reset_and_halt(True)
             tool.examine_ap()
-        flash_ops_allowed = cm_open
+        flash_ops_allowed = is_cm0_open
 
     if erase_boot:
         if flash_ops_allowed:
             erase_slots(tool, target, 'BOOT')
         else:
             logger.warning('Skip erasing BOOT slot, AP cm0 is closed')
     else:
@@ -378,30 +404,36 @@
             erase_smif(tool, target)
         else:
             logger.warning('Skip erasing external memory, AP cm0 is closed')
 
     context = EncryptedProgrammingContext(AesHeaderStrategy)
 
     # Program user application
-    for encrypted, app in target.policy_parser.get_user_apps():
+    user_apps = target.policy_parser.get_user_apps()
+    if user_apps:
+        tool.reset()
+    for encrypted, app in user_apps:
         if not os.path.isabs(app):
             app = os.path.join(target.policy_parser.policy_dir, app)
         if encrypted:
             logger.info("Programming encrypted user application '%s':", app)
             result = context.program(tool, target, app)
             if not result:
                 logger.error('User application encrypted programming failed')
                 return ProvisioningStatus.FAIL
         else:
             if flash_ops_allowed:
                 current_ap = tool.get_ap()
-                tool.set_ap(AP.CMx)
+                if current_ap == AP.SYS:
+                    tool.set_ap(AP.CMx)
                 logger.info("Programming user application '%s':", app)
-                tool.reset_and_halt(reset_type=ResetType.HW)
+                tool.halt()
                 tool.program(app)
+                logger.info('Programming user application complete')
+                tool.resume()
                 tool.set_ap(current_ap)
             else:
                 logger.warning('Skip programming user application, '
                                'AP cm0 is closed')
 
     # Program bootloader
     is_custom_bootloader = target.policy_parser.is_custom_bootloader()
@@ -416,57 +448,48 @@
             return ProvisioningStatus.FAIL
     else:
         if not flash_ops_allowed:
             logger.warning('Skip programming bootloader, AP cm0 is closed')
         elif bootloader is None:
             logger.warning('Skip programming bootloader')
         else:
-            sleep(3)
             current_ap = tool.get_ap()
-            tool.set_ap(AP.CMx)
+            if current_ap == AP.SYS:
+                tool.set_ap(AP.CMx)
             logger.info("Programming bootloader '%s':", bootloader)
             tool.halt()
             tool.program(bootloader)
             logger.info('Programming bootloader complete')
+            tool.resume()
             tool.set_ap(current_ap)
 
     if control_dap_cert:
         tool.set_skip_reset_and_halt(False)
 
-    if flash_ops_allowed and re_provision:
-        ConnectHelper.disconnect(tool)
-        ConnectHelper.connect(tool, target, probe_id=probe_id, ap=ap)
-
     tool.reset(ResetType.HW)
     sleep(3)
 
     _save_device_public_key(tool, target)
 
     # Run provisioning syscall
     logger.info('Run provisioning syscall:')
     is_exam_pass, response = provision_keys_and_policies(tool, prov_cmd_jwt,
                                                          target.register_map)
+    tool.reset()
+
     if not is_exam_pass:
         return ProvisioningStatus.FAIL
 
     _save_device_response(target, response)
 
-    tool.reset()
-
     if not target.policy_parser.is_sys_ap_enabled():
-        if not target.policy_parser.is_cmx_ap_enabled(re_provision):
-            logger.info('All APs closed by policy. Final verification is '
-                        'unavailable.')
-            return ProvisioningStatus.OK
-        else:
-            tool.set_ap(AP.CMx)
-
-    logger.debug('Access through %s', tool.get_ap())
+        logger.warning('System AP closed by policy. Final verification is '
+                       'not available')
+        return ProvisioningStatus.OK
 
-    sleep(3)
     sfb_fw_status = tool.read32(reg_map.ENTRANCE_EXAM_FW_STATUS_REG)
     logger.info('FlashBoot firmware status = 0x%x', sfb_fw_status)
     is_exam_pass = sfb_fw_status == reg_map.FB_FW_STATUS_FIRMWARE_RUNNING_CM0
 
     if not is_exam_pass:
         logger.error('FlashBoot firmware status is not as expected')
 
@@ -475,33 +498,35 @@
 
 def read_cm0_permissions(tool, reg_map):
     logger.info('Checking cm0 AP permissions')
     passed, data = get_prov_details(tool, reg_map, FB_POLICY_JWT)
     if passed and len(data) > 0:
         policy = Crypto.readable_jwt(data)
         silicon_policy_parser = PolicyParser(policy['payload'])
-        cm0_open = silicon_policy_parser.is_cmx_ap_enabled(True)
-        logger.info('cm0 AP %s', 'open' if cm0_open else 'closed')
+        is_cm0_open = silicon_policy_parser.is_cmx_ap_enabled(True)
+        logger.info('cm0 AP %s', 'open' if is_cm0_open else 'closed')
     else:
         logger.error('Failed to read policy from device while getting AP '
                      'permission')
         logger.warning('Flash operations will be skipped')
-        cm0_open = False
-    return cm0_open
+        is_cm0_open = False
+    return is_cm0_open
 
 
 def _save_device_public_key(tool, target):
     try:
         jwk_path, pem_path = target.policy_parser.device_public_key_path()
         key = target.key_reader.read_public_key(tool, KeyId.DEVICE, 'jwk')
         if key:
             with open(jwk_path, 'w', encoding='utf-8') as f:
                 f.write(json.dumps(key, indent=4))
             pem = PemKey(jwk_path)
             pem.save(pem_path, private_key=False)
+    except TimeoutError:
+        raise
     except (KeyError, OSError, ValueError, TypeError) as e:
         logger.error('Failed to save device public key')
         logger.error(e)
 
 
 def _save_device_response(target, response):
     try:
```

### Comparing `cysecuretools-4.1.0/cysecuretools/execute/provisioning_packet/lib/__init__.py` & `cysecuretools-4.2.0/cysecuretools/execute/provisioning_packet/lib/__init__.py`

 * *Files identical despite different names*

### Comparing `cysecuretools-4.1.0/cysecuretools/execute/provisioning_packet/lib/cyprov_crypto.py` & `cysecuretools-4.2.0/cysecuretools/execute/provisioning_packet/lib/cyprov_crypto.py`

 * *Files identical despite different names*

### Comparing `cysecuretools-4.1.0/cysecuretools/execute/provisioning_packet/lib/cyprov_customer.py` & `cysecuretools-4.2.0/cysecuretools/execute/provisioning_packet/lib/cyprov_customer.py`

 * *Files identical despite different names*

### Comparing `cysecuretools-4.1.0/cysecuretools/execute/provisioning_packet/lib/cyprov_dev.py` & `cysecuretools-4.2.0/cysecuretools/execute/provisioning_packet/lib/cyprov_dev.py`

 * *Files identical despite different names*

### Comparing `cysecuretools-4.1.0/cysecuretools/execute/provisioning_packet/lib/cyprov_entity.py` & `cysecuretools-4.2.0/cysecuretools/execute/provisioning_packet/lib/cyprov_entity.py`

 * *Files identical despite different names*

### Comparing `cysecuretools-4.1.0/cysecuretools/execute/provisioning_packet/lib/cyprov_hsm.py` & `cysecuretools-4.2.0/cysecuretools/execute/provisioning_packet/lib/cyprov_hsm.py`

 * *Files identical despite different names*

### Comparing `cysecuretools-4.1.0/cysecuretools/execute/provisioning_packet/lib/cyprov_oem.py` & `cysecuretools-4.2.0/cysecuretools/execute/provisioning_packet/lib/cyprov_oem.py`

 * *Files identical despite different names*

### Comparing `cysecuretools-4.1.0/cysecuretools/execute/provisioning_packet/lib/cyprov_pem.py` & `cysecuretools-4.2.0/cysecuretools/execute/provisioning_packet/lib/cyprov_pem.py`

 * *Files identical despite different names*

### Comparing `cysecuretools-4.1.0/cysecuretools/execute/provisioning_packet/lib/cyprov_types.py` & `cysecuretools-4.2.0/cysecuretools/execute/provisioning_packet/lib/cyprov_types.py`

 * *Files identical despite different names*

### Comparing `cysecuretools-4.1.0/cysecuretools/execute/provisioning_packet/provisioning_packet_mxs40sv2.py` & `cysecuretools-4.2.0/cysecuretools/execute/provisioning_packet/provisioning_packet_mxs40sv2.py`

 * *Files 5% similar despite different names*

```diff
@@ -132,16 +132,17 @@
 
         if not signature:
             if not os.path.isfile(pubkey):
                 raise FileNotFoundError(
                     errno.ENOENT, os.strerror(errno.ENOENT), pubkey)
 
             assets_list = self._reprovisioning_assets()
-            asset_builder = AssetBuilder(self.policy_parser, assets_list,
-                                         pubkey=pubkey)
+            asset_builder = AssetBuilder(
+                self.policy_parser, assets_list, pubkey=pubkey,
+                image_id=kwargs.get('image_id'))
             input_data = asset_builder.get_assets()
         else:
             if not in_params_path:
                 raise ValueError('Input parameters file not specified')
             with open(in_params_path, 'rb') as f:
                 input_data = f.read()
```

### Comparing `cysecuretools-4.1.0/cysecuretools/execute/provisioning_packet/provisioning_packet_mxs40v1.py` & `cysecuretools-4.2.0/cysecuretools/execute/provisioning_packet/provisioning_packet_mxs40v1.py`

 * *Files identical despite different names*

### Comparing `cysecuretools-4.1.0/cysecuretools/execute/silicon_data_reader/silicon_data_reader_mxs40sv2.py` & `cysecuretools-4.2.0/cysecuretools/execute/silicon_data_reader/silicon_data_reader_mxs40sv2.py`

 * *Files identical despite different names*

### Comparing `cysecuretools-4.1.0/cysecuretools/execute/silicon_data_reader/silicon_data_reader_mxs40v1.py` & `cysecuretools-4.2.0/cysecuretools/execute/silicon_data_reader/silicon_data_reader_mxs40v1.py`

 * *Files identical despite different names*

### Comparing `cysecuretools-4.1.0/cysecuretools/execute/sys_call.py` & `cysecuretools-4.2.0/cysecuretools/execute/sys_call.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-Copyright 2018-2022 Cypress Semiconductor Corporation (an Infineon company)
+Copyright 2018-2023 Cypress Semiconductor Corporation (an Infineon company)
 or an affiliate of Cypress Semiconductor Corporation. All rights reserved.
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
@@ -25,14 +25,16 @@
 READ_SILICON_ID_OPCODE = 0x00
 READ_SILICON_ID_COMM = 0x01
 REGION_HASH_OPCODE = 0x31
 PROVISIONING_OPCODE = 0x33
 ENCRYPTED_PROGRAMMING_OPCODE = 0x34
 GET_PROV_DETAILS_OPCODE = 0x37
 SET_DAP_CONTROL_OPCODE = 0x3A
+TRANSITION_TO_RMA_OPCODE = 0x3B
+OPEN_RMA_OPCODE = 0x29
 
 # GetProvDetails SysCall codes
 FB_POLICY_JWT = 0x100
 FB_POLICY_IMG_CERTIFICATE = 0x300
 
 logger = logging.getLogger(__name__)
 
@@ -81,14 +83,90 @@
             logger.error('RegionHash syscall error: 0x%x', response)
             print_sfb_status(response)
             result = RegionHashStatus.FAIL
 
     return result
 
 
+def transition_to_rma(tool, mem_map, reg_map, cert):
+    """
+    Converts parts from SECURE to RMA lifecycle stage
+    @param tool: Programming/debugging tool.
+    @param mem_map: Device memory map.
+    @param reg_map: Device register map.
+    @param cert: JWT packet signed by the key mentioned in the debug/RMA
+           section of the policy, with authentication object including
+           valid DIE_ID range.
+    :return: True if the SysCall succeeds, otherwise False.
+    """
+    return _rma_syscall(tool, mem_map, reg_map, cert, 'TransitionToRMA')
+
+
+def open_rma(tool, mem_map, reg_map, cert):
+    """
+    Enables full access to device in RMA lifecycle stage.
+    @param tool: Programming/debugging tool.
+    @param mem_map: Device memory map.
+    @param reg_map: Device register map.
+    @param cert: JWT packet signed by the key mentioned in the debug/RMA
+           section of the policy, with authentication object including
+           valid DIE_ID range.
+    :return: True if the SysCall succeeds, otherwise False.
+    """
+    return _rma_syscall(tool, mem_map, reg_map, cert, 'OpenRMA')
+
+
+def _rma_syscall(tool, mem_map, reg_map, cert, syscall_name):
+    """
+    Executes RMA system call.
+    @param tool: Programming/debugging tool.
+    @param reg_map: Device register map.
+    @param cert: JWT packet signed by the key mentioned in the debug/RMA
+           section of the policy, with authentication object including
+           valid DIE_ID range.
+    @param syscall_name: SysCall name - TransitionToRMA or OpenRMA.
+    :return: True if the SysCall succeeds, otherwise False.
+    """
+    if len(cert) > mem_map.SRAM_SIZE:
+        logger.error('JWT packet size (%s) exceeds SRAM_SCRATCH2 size (%s)',
+                     len(cert), mem_map.SRAM_SIZE)
+        return False
+
+    if syscall_name == 'TransitionToRMA':
+        op_code = TRANSITION_TO_RMA_OPCODE << 24
+        sram_scratch_addr = mem_map.SRAM_ADDR
+    elif syscall_name == 'OpenRMA':
+        op_code = OPEN_RMA_OPCODE << 24
+        sram_scratch_addr = mem_map.RAM_ADDR
+    else:
+        raise ValueError(f"Invalid SysCall name '{syscall_name}'")
+    sram_scratch2_addr = sram_scratch_addr + 0x08
+
+    if not wait_acquire_ipc_struct(tool, reg_map):
+        raise TimeoutError('Acquire IPC struct timeout')
+
+    logger.debug('Start %s syscall', syscall_name)
+    tool.write32(reg_map.CYREG_IPC2_STRUCT_DATA, sram_scratch_addr)
+    tool.write32(sram_scratch_addr, op_code)
+    tool.write32(sram_scratch_addr + 0x04, sram_scratch2_addr)
+    tool.write32(sram_scratch2_addr, len(cert))
+    tool.write(sram_scratch2_addr + 0x04, [ord(char) for char in list(cert)])
+
+    ipc_struct_notify(tool, reg_map)
+    wait_release_ipc_struct(tool, reg_map)
+    response = tool.read32(sram_scratch_addr)
+
+    if (response & 0xFF000000) == 0xa0000000:
+        logger.debug('%s syscall passed', syscall_name)
+        return True
+    logger.error('%s syscall error: 0x%x', syscall_name, response)
+    print_sfb_status(response)
+    return False
+
+
 def get_prov_details(tool, reg_map, key_id):
     """
     Calls GetProvDetails syscall over IPC.
     :param tool: Programming/debugging tool.
     :param key_id: Public key ID.
     :param reg_map: Device register map.
     :return: True if syscall succeeds, otherwise False.
@@ -159,14 +237,15 @@
     Calls ProvisionKeysAndPolicies syscall over IPC.
     :param tool: Programming/debugging tool.
     :param filename: Path to provisioning JWT file.
     :param reg_map: Device register map.
     :return: Tuple with the syscall result and device response
     """
     logger.debug('Start ProvisionKeysAndPolicies syscall')
+    logger.debug("Apply JWT '%s'", filename)
     if filename:
         file_size = os.path.getsize(filename)
         if file_size > reg_map.ENTRANCE_EXAM_SRAM_SIZE:
             logger.error('JWT packet too long')
             return False
 
         logger.info('JWT packet size = %d', file_size)
@@ -360,14 +439,15 @@
         logger.debug('JWT is NOT required')
         tool.write32(reg_map.CYREG_IPC2_STRUCT_DATA, op_code)
         log_reg_value(tool, reg_map.CYREG_IPC2_STRUCT_DATA)
     else:
         logger.debug('JWT is required')
         if not filename:
             raise ValueError('JWT certificate is required but not specified')
+        logger.info("Apply certificate '%s'", filename)
 
         file_size = os.path.getsize(filename)
         if file_size > reg_map.ENTRANCE_EXAM_SRAM_SIZE:
             logger.error('JWT packet too long')
             return False
 
         logger.debug('JWT packet size: %d', file_size)
@@ -469,41 +549,41 @@
         raise TimeoutError('IPC structure release timeout')
 
     result = (ipc_acquire & (1 << 31)) != 0
     logger.debug("wait_acquire_ipc_struct result '0x%x'", result)
     return result
 
 
-def wait_release_ipc_struct(tool, reg_map, timeout=1500):
+def wait_release_ipc_struct(tool, reg_map, timeout=300):
     """
     Wait for release IPC structure.
-    :param tool: Programming/debugging tool.
-    :param reg_map: Device register map.
-    :param timeout: Timeout to release structure.
-    :return: IPC acquire status (True or False)
+    @param tool: Programming/debugging tool.
+    @param reg_map: Device register map.
+    @param timeout: Timeout to release structure.
+    @return: IPC acquire status (True or False)
     """
     logger.debug('Start wait_release_ipc_struct')
     response = 0x80000000
     count = 0
     while (response & 0x80000000) != 0 and count < timeout:
         response = tool.read32(reg_map.CYREG_IPC2_STRUCT_LOCK_STATUS)
         count += 1
         sleep(0.2)
     if count >= timeout:
         raise TimeoutError('IPC structure release timeout')
-    result = (response & (1 << 31)) != 0
+    result = response & (1 << 31)
     logger.debug("wait_release_ipc_struct result '0x%x'", result)
-    return result
+    return result != 0
 
 
 def ipc_struct_notify(tool, reg_map):
     """
     IPC_STRUCT[ipc_id].IPC_NOTIFY
-    :param tool: Programming/debugging tool.
-    :param reg_map: Device register map.
+    @param tool: Programming/debugging tool.
+    @param reg_map: Device register map.
     """
     logger.debug('ipc_struct_notify')
     tool.write32(reg_map.CYREG_IPC2_STRUCT_NOTIFY, 0x00000001)
 
 
 def print_sfb_status(status_code, severity='error'):
     """
```

### Comparing `cysecuretools-4.1.0/cysecuretools/execute/version_provider/version_provider_mxs40sv2.py` & `cysecuretools-4.2.0/cysecuretools/execute/version_provider/version_provider_mxs40sv2.py`

 * *Files 4% similar despite different names*

```diff
@@ -99,17 +99,17 @@
             logger.debug('Not able to find installation source details')
 
     def log_version(self, tool):
         """ Logs lifecycle stage of the device """
         self.log_lifecycle_stage(tool)
 
     @staticmethod
-    def verify_fw_version(_):
+    def check_compatibility(_tool, **_):
         """
-        Verifies FW version compatibility.
+        Verifies HW compatibility.
         N/A for MXS40Sv2 platform
         """
         return True
 
     def log_lifecycle_stage(self, tool):
         """
         Reads device lifecycle stage and creates a
```

### Comparing `cysecuretools-4.1.0/cysecuretools/execute/voltage_tool/lvd_voltage_picker.py` & `cysecuretools-4.2.0/cysecuretools/execute/voltage_tool/lvd_voltage_picker.py`

 * *Files identical despite different names*

### Comparing `cysecuretools-4.1.0/cysecuretools/execute/voltage_tool/voltage_tool_mxs40v1.py` & `cysecuretools-4.2.0/cysecuretools/execute/voltage_tool/voltage_tool_mxs40v1.py`

 * *Files identical despite different names*

### Comparing `cysecuretools-4.1.0/cysecuretools/main.py` & `cysecuretools-4.2.0/cysecuretools/main.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """
-Copyright (c) 2019-2021 Cypress Semiconductor Corporation
+Copyright 2019-2022 Cypress Semiconductor Corporation (an Infineon company)
+or an affiliate of Cypress Semiconductor Corporation. All rights reserved.
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
 
@@ -13,14 +14,15 @@
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 import json
 import logging
 import os
 import sys
+
 from cryptography.hazmat.primitives import serialization
 
 import cysecuretools.execute.jwt as jwt
 import cysecuretools.execute.keygen as keygen
 from cysecuretools.core.certificates.x509 import X509CertificateStrategy
 from cysecuretools.core.logging_formatter import CustomFormatter
 from cysecuretools.core.strategy_context.cert_strategy_ctx \
@@ -42,14 +44,15 @@
 from cysecuretools.execute.image_cert import ImageCertificate
 from cysecuretools.execute.key_reader import get_aes_key
 from cysecuretools.execute.programmer.programmer import ProgrammingTool
 from .targets import print_targets, get_target_builder, is_psoc64, is_mxs40sv2
 from cysecuretools.core.logging_configurator import LoggingConfigurator
 from .core.ocd_settings import OcdSettings
 from .core.connect_helper import ConnectHelper
+from .core.deprecated import deprecated
 
 # Initialize logger
 logging.root.setLevel(logging.DEBUG)
 fmt = CustomFormatter()
 console_handler = logging.StreamHandler(sys.stdout)
 console_handler.setFormatter(fmt)
 console_handler.setLevel(logging.INFO)
@@ -60,23 +63,24 @@
 class CySecureTools:
     """
     Class provides methods for creating keys, signing user
     application and device provisioning.
     """
 
     def __init__(self, target=None, policy=None, log_file=True,
-                 skip_prompts=False, skip_validation=False):
+                 skip_prompts=False, skip_validation=False, rev=None):
         """
         Creates instance of the class
-        :param target: Device manufacturing part number
-        :param policy: Provisioning policy file
-        :param log_file: Indicates whether to write log into a file
-        :param skip_prompts: Indicates whether to skip user interactive
+        @param target: Device manufacturing part number
+        @param policy: Provisioning policy file
+        @param log_file: Indicates whether to write log into a file
+        @param skip_prompts: Indicates whether to skip user interactive
                prompts
-        :param skip_validation: Indicates whether to skip policy validation
+        @param skip_validation: Indicates whether to skip policy validation
+        @param rev: Device revision
         """
         self.skip_validation = skip_validation
 
         if log_file:
             LoggingConfigurator.add_file_logging()
 
         settings = OcdSettings()
@@ -100,15 +104,17 @@
         if policy is not None:
             self.policy = os.path.abspath(policy)
         if ProjectInitializer.is_project():
             if policy is None:
                 self.policy = ProjectInitializer.get_default_policy()
             cwd = os.getcwd()
 
-        self.target = self._get_target(self.target_name, self.policy, cwd)
+        self.target = self._get_target(self.target_name, self.policy, cwd,
+                                       rev=rev)
+
         self.policy = self.target.policy
         self.policy_parser = self.target.policy_parser
         self.version_provider = self.target.version_provider
 
     def create_keys(self, overwrite=None, out=None, kid=None,
                     user_key_alg=KeyAlgorithm.EC, **kwargs):
         """
@@ -254,38 +260,36 @@
         :param image: User application file
         :param signature: Path to the binary file containing signature
         :param output: Path where to save the signed image
         :return: Path to
         """
         self.target.sign_tool.add_signature(image, signature, output)
 
-    def sign_image(self, image, image_id=1, **kwargs):
+    def sign_image(self, image, image_id=None, **kwargs):
         """
         Signs firmware image with the key specified in the policy file.
         :param image: User application file.
         :param image_id: The ID of the image in the policy file.
         :return: Signed (and encrypted if applicable) hex file path.
         """
         if not self._validate_policy(['pre_build', 'dap_disabling']):
             return None
-        result = self.target.sign_tool.sign_image(image, image_id=image_id,
-                                                  **kwargs)
-        return result
+        return self.target.sign_tool.sign_image(image, image_id=image_id,
+                                                **kwargs)
 
     def extend_image(self, image, **kwargs):
         """
         Extends firmware image with the TLVs.
         :param image: User application file.
         :return: Extended (and encrypted if applicable) file path.
         """
         if not is_mxs40sv2(self.target_name):
             raise ValueError(
                 'Method is not compatible with the selected target')
-        result = self.target.sign_tool.extend_image(image, **kwargs)
-        return result
+        return self.target.sign_tool.extend_image(image, **kwargs)
 
     def create_provisioning_packet(self, **kwargs):
         """
         Creates JWT packet for provisioning device.
         :return: True if packet created successfully, otherwise False.
         """
         if not self._validate_policy():
@@ -324,17 +328,18 @@
             bootloader = self.target.bootloader_provider.hex_path()
             if not os.path.isfile(bootloader):
                 logger.error("Cannot find bootloader file '%s'", bootloader)
                 return False
 
         if ConnectHelper.connect(self.tool, self.target, probe_id=probe_id,
                                  ap=ap):
-            self.version_provider.log_version(self.tool)
-            if not self.version_provider.verify_fw_version(self.tool):
+            if not self.version_provider.check_compatibility(self.tool):
+                ConnectHelper.disconnect(self.tool)
                 return False
+            self.version_provider.log_version(self.tool)
 
             context = ProvisioningContext(self.target.provisioning_strategy)
             status = context.provision(
                 self.tool, self.target,
                 bootloader=bootloader,
                 probe_id=self.tool.probe_id, ap=ap, skip_prompts=self.skip_prompts,
                 **kwargs)
@@ -346,17 +351,17 @@
             logger.error('Error occurred while provisioning device')
 
         return status == ProvisioningStatus.OK
 
     def re_provision_device(self, probe_id=None, ap='sysap', **kwargs):
         """
         Executes device re-provisioning
-        :param probe_id: Probe serial number.
-        :param ap: The access port used for re-provisioning
-        :return: Provisioning result. True if success, otherwise False.
+        @param probe_id: Probe serial number.
+        @param ap: The access port used for re-provisioning
+        @return: Provisioning result. True if success, otherwise False.
         """
         if not self._validate_policy():
             return False
 
         # Get bootloader program file
         bootloader = None
         if not kwargs.get('skip_bootloader', False):
@@ -368,21 +373,22 @@
                     return False
 
         context = ProvisioningContext(self.target.provisioning_strategy)
 
         if ConnectHelper.connect(self.tool, self.target, probe_id=probe_id,
                                  ap=ap):
 
-            self.version_provider.log_version(self.tool)
-            if not self.version_provider.verify_fw_version(self.tool):
+            if not self.version_provider.check_compatibility(self.tool):
+                ConnectHelper.disconnect(self.tool)
                 return False
+            self.version_provider.log_version(self.tool)
 
             status = context.re_provision(
                 self.tool, self.target,
-                bootloader=bootloader, probe_id=self.tool.probe_id, ap=ap, **kwargs)
+                bootloader=bootloader, probe_id=self.tool.probe_id, **kwargs)
             ConnectHelper.disconnect(self.tool)
         else:
             status = ProvisioningStatus.FAIL
 
         if status == ProvisioningStatus.FAIL:
             logger.error('Error occurred while reprovisioning device')
 
@@ -433,15 +439,15 @@
                 kwargs['public_key'] = default['public_key']
 
         logger.info('Start creating certificate')
         overwrite = True if self.skip_prompts else None
         return context.create_certificate(cert_name, cert_encoding,
                                           overwrite=overwrite, **kwargs)
 
-    def entrance_exam(self, probe_id=None, ap='cm4', erase_flash=False):
+    def entrance_exam(self, probe_id=None, ap='sysap', erase_flash=False):
         """
         Checks device life-cycle, Flashboot firmware and Flash state.
         :param probe_id: Probe serial number.
         :param ap: The access port used for entrance exam
         :param erase_flash: Indicates whether to erase flash before the
                entrance exam
         :return True if the device is ready for provisioning,
@@ -451,25 +457,25 @@
             raise ValueError(
                 'Method is not compatible with the selected target')
 
         if not self._validate_policy(['pre_build', 'dap_disabling']):
             return False
 
         status = False
-        if ConnectHelper.connect(self.tool, self.target, probe_id=probe_id,
-                                 ap=ap, reset_and_halt=True):
+        if ConnectHelper.connect(self.tool, self.target,
+                                 probe_id=probe_id, ap=ap):
 
-            self.version_provider.log_version(self.tool)
-            if not self.version_provider.verify_fw_version(self.tool):
+            if not self.version_provider.check_compatibility(self.tool):
+                ConnectHelper.disconnect(self.tool)
                 return False
+            self.version_provider.log_version(self.tool)
 
             context = ProvisioningContext(self.target.provisioning_strategy)
-            if erase_flash:
-                context.erase_flash(self.tool, self.target)
-            status = self.target.entrance_exam.execute(self.tool)
+            status = self.target.entrance_exam.execute(self.tool,
+                                                       erase_flash=erase_flash)
             if status == EntranceExamStatus.FLASH_NOT_EMPTY:
                 if self.skip_prompts:
                     logger.error('Entrance exam failed. '
                                  'User firmware running on chip detected')
                     return ProvisioningStatus.FAIL
                 else:
                     answer = input(
@@ -585,16 +591,19 @@
         # Get public key
         pub_key_pem = None
         logger.debug('Device key id = %d', dev_key_id)
 
         connected = ConnectHelper.connect(self.tool, self.target, ap='sysap',
                                           probe_id=probe_id, blocking=False)
         if connected:
+            if not self.version_provider.check_compatibility(
+                    self.tool, check_si_rev=False):
+                ConnectHelper.disconnect(self.tool)
+                return False
             self.version_provider.log_version(self.tool)
-            self.version_provider.verify_fw_version(self.tool)
 
             logger.info('Read device public key from device')
             pub_key_pem = self.target.key_reader.read_public_key(
                 self.tool, dev_key_id, 'pem')
             ConnectHelper.disconnect(self.tool)
 
         if not connected or not pub_key_pem:
@@ -630,18 +639,17 @@
                 'Method is not compatible with the selected target')
 
         result = False
         context = EncryptedProgrammingContext(AesHeaderStrategy)
         if ConnectHelper.connect(self.tool, self.target, probe_id=probe_id,
                                  ap='sysap'):
 
-            self.version_provider.log_version(self.tool)
-            self.version_provider.verify_fw_version(self.tool)
-
-            result = context.program(self.tool, self.target, encrypted_image)
+            if self.version_provider.check_compatibility(self.tool):
+                self.version_provider.log_version(self.tool)
+                result = context.program(self.tool, self.target, encrypted_image)
             ConnectHelper.disconnect(self.tool)
         return result
 
     def read_public_key(self, key_id, key_fmt, out_file=None, probe_id=None):
         """
         Reads public key from device and saves it to the file
         :param key_id: Key ID to read
@@ -654,16 +662,19 @@
             raise ValueError(
                 'Method is not compatible with the selected target')
 
         key = None
         if ConnectHelper.connect(self.tool, self.target, probe_id=probe_id,
                                  ap='sysap'):
 
+            if not self.version_provider.check_compatibility(
+                    self.tool, check_si_rev=False):
+                ConnectHelper.disconnect(self.tool)
+                return key
             self.version_provider.log_version(self.tool)
-            self.version_provider.verify_fw_version(self.tool)
 
             try:
                 key = self.target.key_reader.read_public_key(
                     self.tool, key_id, key_fmt)
                 if key is None:
                     logger.error('Cannot read public key (key_id=%d)', key_id)
                 elif out_file:
@@ -687,18 +698,18 @@
         :param probe_id: Probe serial number
         :param ap: The access port used to read the data
         :return: Die ID if success, otherwise None
         """
         die_id = None
         if ConnectHelper.connect(self.tool, self.target, probe_id=probe_id,
                                  ap=ap):
-            self.version_provider.log_version(self.tool)
-            self.version_provider.verify_fw_version(self.tool)
-
-            die_id = self.target.silicon_data_reader.read_die_id(self.tool)
+            if self.version_provider.check_compatibility(
+                    self.tool, check_si_rev=False):
+                self.version_provider.log_version(self.tool)
+                die_id = self.target.silicon_data_reader.read_die_id(self.tool)
             ConnectHelper.disconnect(self.tool)
         return die_id
 
     def get_device_lifecycle(self, probe_id=None, ap='sysap'):
         """
         Reads device lifecycle stage
         :param probe_id: Probe serial number
@@ -772,19 +783,20 @@
         Boot version programmed into device
         :param probe_id: Probe serial number
         :param ap: The access port used for to read CyBootloader and
                Secure Flash Boot version from device
         """
         connected = ConnectHelper.connect(self.tool, self.target, ap=ap,
                                           probe_id=probe_id, blocking=False,
-                                          suppress_errors=True)
+                                          ignore_errors=True)
         self.version_provider.print_version(**kwargs)
         if connected:
-            self.version_provider.print_fw_version(self.tool)
-            self.version_provider.verify_fw_version(self.tool)
+            if self.version_provider.check_compatibility(
+                    self.tool, check_si_rev=False):
+                self.version_provider.print_fw_version(self.tool)
             ConnectHelper.disconnect(self.tool)
 
     def init(self, **kwargs):
         """
         Initializes new project
         """
         cwd = os.getcwd()
@@ -826,46 +838,66 @@
         if not os.path.isfile(config):
             raise FileNotFoundError(f'File \'{config}\' not found')
 
         context = ProvisioningContext(self.target.provisioning_strategy)
 
         if ConnectHelper.connect(self.tool, self.target, probe_id=probe_id,
                                  ap=ap):
-            self.version_provider.log_version(self.tool)
-            if not self.version_provider.verify_fw_version(self.tool):
+            if not self.version_provider.check_compatibility(self.tool):
+                ConnectHelper.disconnect(self.tool)
                 return False
+            self.version_provider.log_version(self.tool)
             status = context.provision(self.tool, self.target,
                                        skip_prompts=self.skip_prompts,
                                        config=config)
             ConnectHelper.disconnect(self.tool)
         else:
             status = ProvisioningStatus.FAIL
 
         if status == ProvisioningStatus.FAIL:
             logger.error('An error occurred while loading the application')
 
         return status == ProvisioningStatus.OK
 
+    @deprecated("DEPRECATED! Use 'transit_to_rma()', not 'convert_to_rma()'")
     def convert_to_rma(self, probe_id=None, ap='sysap', **kwargs):
+        return self.transit_to_rma(probe_id=probe_id, ap=ap, **kwargs)
+
+    def transit_to_rma(self, probe_id=None, ap='sysap', **kwargs):
         """
-        Converts device to the RMA lifecycle stage
+        Transits device to the RMA lifecycle stage
         @param probe_id: Probe serial number
         @param ap: The access port used for communication
         @return: True if success, otherwise False
         """
-        if not is_mxs40sv2(self.target_name):
-            raise ValueError(
-                'Method is not compatible with the selected target')
+        status = ProvisioningStatus.FAIL
+        cert = kwargs.get('cert')
+        del (kwargs['cert'])
+        if ConnectHelper.connect(self.tool, self.target,
+                                 probe_id=probe_id, ap=ap):
+            self.version_provider.log_version(self.tool)
+            context = ProvisioningContext(self.target.provisioning_strategy)
+            status = context.transit_to_rma(self.tool, self.target, cert,
+                                            **kwargs)
+            ConnectHelper.disconnect(self.tool)
+        return status == ProvisioningStatus.OK
 
+    def open_rma(self, cert, probe_id=None):
+        """
+        Enables full access to device in RMA lifecycle stage
+        @param cert: Open RMA certificate
+        @param probe_id: Probe serial number
+        @param ap: The access port used for communication
+        @return: True if success, otherwise False
+        """
         status = ProvisioningStatus.FAIL
         if ConnectHelper.connect(self.tool, self.target, probe_id=probe_id,
-                                 ap=ap):
-            self.version_provider.log_version(self.tool)
+                                 ignore_errors=True):
             context = ProvisioningContext(self.target.provisioning_strategy)
-            status = context.convert_to_rma(self.tool, self.target, **kwargs)
+            status = context.open_rma(self.tool, self.target, cert)
             ConnectHelper.disconnect(self.tool)
         return status == ProvisioningStatus.OK
 
     def debug_certificate(self, template, output, key_id=0, key_path=None,
                           **kwargs):
         """
         Creates debug or RMA certificate binary from the
@@ -919,16 +951,16 @@
         self.target.policy_validator.skip_validation = self.skip_validation
         validation_state = self.target.policy_validator.validate(
             skip=skip_list,
             skip_prompts=self.skip_prompts)
         return validation_state not in [ValidationStatus.ERROR,
                                         ValidationStatus.TERMINATED]
 
-    def _get_target(self, target_name, policy, cwd):
+    def _get_target(self, target_name, policy, cwd, rev=None):
         director = TargetDirector()
-        self.target_builder = get_target_builder(director, target_name)
+        self.target_builder = get_target_builder(director, target_name, rev=rev)
         return director.get_target(policy, target_name, cwd)
 
     @staticmethod
     def device_list():
         print_targets()
         return True
```

### Comparing `cysecuretools-4.1.0/cysecuretools/pkg_globals.py` & `cysecuretools-4.2.0/cysecuretools/pkg_globals.py`

 * *Files identical despite different names*

### Comparing `cysecuretools-4.1.0/cysecuretools/targets/common/mxs40sv2/asset.py` & `cysecuretools-4.2.0/cysecuretools/targets/common/mxs40sv2/asset.py`

 * *Files identical despite different names*

### Comparing `cysecuretools-4.1.0/cysecuretools/targets/common/mxs40sv2/asset_builder.py` & `cysecuretools-4.2.0/cysecuretools/targets/common/mxs40sv2/asset_builder.py`

 * *Files identical despite different names*

### Comparing `cysecuretools-4.1.0/cysecuretools/targets/common/mxs40sv2/asset_enums.py` & `cysecuretools-4.2.0/cysecuretools/targets/common/mxs40sv2/asset_enums.py`

 * *Files identical despite different names*

### Comparing `cysecuretools-4.1.0/cysecuretools/targets/common/mxs40sv2/dependencies_validator/__init__.py` & `cysecuretools-4.2.0/cysecuretools/targets/common/mxs40sv2/dependencies_validator/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,20 +1,23 @@
 from .pre_build_keys_exist_validator import PreBuildKeysExistValidator
 from .encryption_key_validator import EncryptionAndProgramOemKey1Validator
 from .hci_mode_validator import HciModeValidator
 from .revoke_oem_encryption_validator import RevocationAndEncryptionValidator
 from .access_restrictions_validator import AccessRestrictionsValidator
+from .nv_counter_validator import NvCounterValidator
 
 validators = {
-    'pre_build': [PreBuildKeysExistValidator,
-                  HciModeValidator,
-                  EncryptionAndProgramOemKey1Validator,
-                  RevocationAndEncryptionValidator,
-                  AccessRestrictionsValidator
-                  ]
+    'pre_build': [
+        PreBuildKeysExistValidator,
+        HciModeValidator,
+        EncryptionAndProgramOemKey1Validator,
+        RevocationAndEncryptionValidator,
+        AccessRestrictionsValidator,
+        NvCounterValidator
+    ]
 }
 
 
 def validate(policy_parser, skip_list):
     """ Validates dependencies and returns list of messages """
     is_valid = True
     messages = list()
```

### Comparing `cysecuretools-4.1.0/cysecuretools/targets/common/mxs40sv2/dependencies_validator/access_restrictions_validator.py` & `cysecuretools-4.2.0/cysecuretools/targets/common/mxs40sv2/dependencies_validator/access_restrictions_validator.py`

 * *Files identical despite different names*

### Comparing `cysecuretools-4.1.0/cysecuretools/targets/common/mxs40sv2/dependencies_validator/encryption_key_validator.py` & `cysecuretools-4.2.0/cysecuretools/targets/common/mxs40sv2/dependencies_validator/encryption_key_validator.py`

 * *Files identical despite different names*

### Comparing `cysecuretools-4.1.0/cysecuretools/targets/common/mxs40sv2/dependencies_validator/hci_mode_validator.py` & `cysecuretools-4.2.0/cysecuretools/targets/common/mxs40sv2/dependencies_validator/hci_mode_validator.py`

 * *Files identical despite different names*

### Comparing `cysecuretools-4.1.0/cysecuretools/targets/common/mxs40sv2/dependencies_validator/pre_build_keys_exist_validator.py` & `cysecuretools-4.2.0/cysecuretools/targets/common/mxs40sv2/dependencies_validator/pre_build_keys_exist_validator.py`

 * *Files identical despite different names*

### Comparing `cysecuretools-4.1.0/cysecuretools/targets/common/mxs40sv2/dependencies_validator/revoke_oem_encryption_validator.py` & `cysecuretools-4.2.0/cysecuretools/targets/common/mxs40sv2/dependencies_validator/revoke_oem_encryption_validator.py`

 * *Files identical despite different names*

### Comparing `cysecuretools-4.1.0/cysecuretools/targets/common/mxs40sv2/enums.py` & `cysecuretools-4.2.0/cysecuretools/targets/common/mxs40sv2/enums.py`

 * *Files identical despite different names*

### Comparing `cysecuretools-4.1.0/cysecuretools/targets/common/mxs40sv2/flow_parser.py` & `cysecuretools-4.2.0/cysecuretools/targets/common/mxs40sv2/flow_parser.py`

 * *Files identical despite different names*

### Comparing `cysecuretools-4.1.0/cysecuretools/targets/common/mxs40sv2/json/cyw20829_no_secure.json_schema` & `cysecuretools-4.2.0/cysecuretools/targets/common/mxs40sv2/json/cyw20829_no_secure.json_schema`

 * *Files identical despite different names*

### Comparing `cysecuretools-4.1.0/cysecuretools/targets/common/mxs40sv2/json/cyw20829_reprovisioning_no_secure.json_schema` & `cysecuretools-4.2.0/cysecuretools/targets/common/mxs40sv2/json/cyw20829_reprovisioning_no_secure.json_schema`

 * *Files identical despite different names*

### Comparing `cysecuretools-4.1.0/cysecuretools/targets/common/mxs40sv2/json/cyw20829_reprovisioning_secure.json_schema` & `cysecuretools-4.2.0/cysecuretools/targets/common/mxs40sv2/json/cyw20829_reprovisioning_secure.json_schema`

 * *Files 10% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999984809027778%*

 * *Differences: {"'properties'": "{'device_policy': {'properties': {'reprovisioning': {'properties': "*

 * *                 '{\'nv_counter\': {\'description\': "Anti-rollback counter. Each item of the '*

 * *                 "'value' array defines counter for each next application. Each 'bits_per_cnt' "*

 * *                 'item defines number of bits for the next application counter (total bits number '*

 * *                 "32). IMPORTANT: 'bits_per_cnt' in the provisioning and reprovisioning policy "*

 * *                 'files MUST BE the […]*

```diff
@@ -35,21 +35,40 @@
                     "type": "object"
                 },
                 "reprovisioning": {
                     "description": "Re-provisioning assets",
                     "id": "reprovisioning",
                     "properties": {
                         "nv_counter": {
-                            "description": "Anti-rollback counter (supports up to 32 updates)",
+                            "description": "Anti-rollback counter. Each item of the 'value' array defines counter for each next application. Each 'bits_per_cnt' item defines number of bits for the next application counter (total bits number 32). IMPORTANT: 'bits_per_cnt' in the provisioning and reprovisioning policy files MUST BE the same",
                             "id": "nv_counter",
                             "properties": {
+                                "bits_per_cnt": {
+                                    "items": {
+                                        "maximum": 32,
+                                        "minimum": 0,
+                                        "type": "number"
+                                    },
+                                    "type": "array"
+                                },
                                 "value": {
-                                    "maximum": 32,
-                                    "minimum": 0,
-                                    "type": "number"
+                                    "anyOf": [
+                                        {
+                                            "maximum": 32,
+                                            "minimum": 0,
+                                            "type": "number"
+                                        },
+                                        {
+                                            "items": {
+                                                "minimum": 0,
+                                                "type": "number"
+                                            },
+                                            "type": "array"
+                                        }
+                                    ]
                                 }
                             },
                             "required": false
                         },
                         "revoke_icv_pubkey_0": {
                             "description": "Revokes ICV public key 0. The ICV public key 1 is used for service application verification (this can be done only once)",
                             "id": "revoke_icv_pubkey_0",
```

### Comparing `cysecuretools-4.1.0/cysecuretools/targets/common/mxs40sv2/json/cyw20829_secure.json_schema` & `cysecuretools-4.2.0/cysecuretools/targets/common/mxs40sv2/json/cyw20829_secure.json_schema`

 * *Files 16% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.999999240451389%*

 * *Differences: {"'properties'": "{'device_policy': {'properties': {'reprovisioning': {'properties': "*

 * *                 '{\'nv_counter\': {\'description\': "Anti-rollback counter. Each item of the '*

 * *                 "'value' array defines counter for each next application. Each 'bits_per_cnt' "*

 * *                 'item defines number of bits for the next application counter (total bits number '*

 * *                 "32). IMPORTANT: 'bits_per_cnt' in the provisioning and reprovisioning policy "*

 * *                 'files MUST BE the […]*

```diff
@@ -329,21 +329,40 @@
                     "type": "object"
                 },
                 "reprovisioning": {
                     "description": "Re-provisioning assets",
                     "id": "reprovisioning",
                     "properties": {
                         "nv_counter": {
-                            "description": "Anti-rollback counter (supports up to 32 updates)",
+                            "description": "Anti-rollback counter. Each item of the 'value' array defines counter for each next application. Each 'bits_per_cnt' item defines number of bits for the next application counter (total bits number 32). IMPORTANT: 'bits_per_cnt' in the provisioning and reprovisioning policy files MUST BE the same",
                             "id": "nv_counter",
                             "properties": {
+                                "bits_per_cnt": {
+                                    "items": {
+                                        "maximum": 32,
+                                        "minimum": 0,
+                                        "type": "number"
+                                    },
+                                    "type": "array"
+                                },
                                 "value": {
-                                    "maximum": 32,
-                                    "minimum": 0,
-                                    "type": "number"
+                                    "anyOf": [
+                                        {
+                                            "maximum": 32,
+                                            "minimum": 0,
+                                            "type": "number"
+                                        },
+                                        {
+                                            "items": {
+                                                "minimum": 0,
+                                                "type": "number"
+                                            },
+                                            "type": "array"
+                                        }
+                                    ]
                                 }
                             },
                             "required": false
                         },
                         "revoke_icv_pubkey_0": {
                             "description": "Revokes ICV public key 0. The ICV public key 1 is used for service application verification (this can be done only once)",
                             "id": "revoke_icv_pubkey_0",
```

### Comparing `cysecuretools-4.1.0/cysecuretools/targets/common/mxs40sv2/policy_parser.py` & `cysecuretools-4.2.0/cysecuretools/targets/common/mxs40sv2/policy_parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -228,14 +228,21 @@
     def get_nv_counter(self):
         try:
             value = self.json['device_policy']['reprovisioning']['nv_counter']['value']
         except KeyError:
             value = 0
         return value
 
+    def get_bits_per_cnt(self):
+        try:
+            value = self.json['device_policy']['reprovisioning']['nv_counter']['bits_per_cnt']
+        except KeyError:
+            value = [32]
+        return value
+
     def get_complete_provisioning(self):
         try:
             value = self.json['device_policy']['misc']['complete_provisioning']['value']
         except KeyError:
             value = False
         return value
```

### Comparing `cysecuretools-4.1.0/cysecuretools/targets/common/mxs40sv2/policy_validator.py` & `cysecuretools-4.2.0/cysecuretools/targets/common/mxs40sv2/policy_validator.py`

 * *Files 2% similar despite different names*

```diff
@@ -67,14 +67,16 @@
         schema = self._get_schema()
         if schema is not None:
             status = self._validate_by_schema(schema, self.policy_parser.json)
 
             if status is ValidationStatus.OK:
                 status = self._validate_dependencies(skip)
 
+        if status == ValidationStatus.ERROR:
+            logger.error('Policy validation error')
         return status
 
     @staticmethod
     def _validate_by_schema(schema, data):
         """ Validation against JSON schema """
         status = ValidationStatus.OK
         with open(schema, encoding='utf-8') as f:
```

### Comparing `cysecuretools-4.1.0/cysecuretools/targets/common/p64/enums.py` & `cysecuretools-4.2.0/cysecuretools/targets/common/p64/enums.py`

 * *Files identical despite different names*

### Comparing `cysecuretools-4.1.0/cysecuretools/targets/common/p64/json/policy_template.json` & `cysecuretools-4.2.0/cysecuretools/targets/common/p64/json/policy_template.json`

 * *Files identical despite different names*

### Comparing `cysecuretools-4.1.0/cysecuretools/targets/common/p64/json/schema.json_schema` & `cysecuretools-4.2.0/cysecuretools/targets/common/p64/json/schema.json_schema`

 * *Files identical despite different names*

### Comparing `cysecuretools-4.1.0/cysecuretools/targets/common/p64/policy_filter.py` & `cysecuretools-4.2.0/cysecuretools/targets/common/p64/policy_filter.py`

 * *Files identical despite different names*

### Comparing `cysecuretools-4.1.0/cysecuretools/targets/common/p64/policy_parser.py` & `cysecuretools-4.2.0/cysecuretools/targets/common/p64/policy_parser.py`

 * *Files identical despite different names*

### Comparing `cysecuretools-4.1.0/cysecuretools/targets/common/p64/policy_validator.py` & `cysecuretools-4.2.0/cysecuretools/targets/common/p64/policy_validator.py`

 * *Files identical despite different names*

### Comparing `cysecuretools-4.1.0/cysecuretools/targets/common/p64/silicon_data_parser.py` & `cysecuretools-4.2.0/cysecuretools/targets/common/p64/silicon_data_parser.py`

 * *Files identical despite different names*

### Comparing `cysecuretools-4.1.0/cysecuretools/targets/cyb06xx5/maps/memory_map.py` & `cysecuretools-4.2.0/cysecuretools/targets/cyb06xxa/maps/memory_map.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """
-Copyright (c) 2019-2020 Cypress Semiconductor Corporation
+Copyright 2019-2023 Cypress Semiconductor Corporation (an Infineon company)
+or an affiliate of Cypress Semiconductor Corporation. All rights reserved.
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
 
@@ -12,26 +13,38 @@
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 from cysecuretools.core import MemoryMapBaseP64
 
 
-class MemoryMap_cyb06xx5(MemoryMapBaseP64):
+class MemoryMap_cyb06xxa(MemoryMapBaseP64):
     @property
     def FLASH_ADDRESS(self):
         return 0x10000000
 
     @property
     def FLASH_SIZE(self):
-        return 0x00070000
+        return 0x001E0000
+
+    @property
+    def RAM_ADDR(self):
+        return 0x08000000
+
+    @property
+    def SRAM_ADDR(self):
+        return 0x080ec000
+
+    @property
+    def SRAM_SIZE(self):
+        return 0x00004000
 
     @property
     def PROVISION_JWT_PACKET_ADDRESS(self):
-        return 0x14003600
+        return 0x101FB600
 
     @property
     def PROVISION_JWT_PACKET_SIZE(self):
         return 0x4A00
 
     @property
     def SPE_IMAGE_ID(self):
```

### Comparing `cysecuretools-4.1.0/cysecuretools/targets/cyb06xx5/maps/register_map.py` & `cysecuretools-4.2.0/cysecuretools/targets/cyb06xx5/maps/register_map.py`

 * *Files identical despite different names*

### Comparing `cysecuretools-4.1.0/cysecuretools/targets/cyb06xx5/packets/cy_auth_512k_b0_sample.jwt` & `cysecuretools-4.2.0/cysecuretools/targets/cyb06xx5/packets/cy_auth_512k_b0_sample.jwt`

 * *Files identical despite different names*

### Comparing `cysecuretools-4.1.0/cysecuretools/targets/cyb06xx5/packets/entrance_exam.jwt` & `cysecuretools-4.2.0/cysecuretools/targets/cyb06xx5/packets/entrance_exam.jwt`

 * *Files identical despite different names*

### Comparing `cysecuretools-4.1.0/cysecuretools/targets/cyb06xx5/policy/policy_multi_CM0_CM4.json` & `cysecuretools-4.2.0/cysecuretools/targets/cyb06xx5/policy/policy_multi_CM0_CM4.json`

 * *Files identical despite different names*

### Comparing `cysecuretools-4.1.0/cysecuretools/targets/cyb06xx5/policy/policy_multi_CM0_CM4_smif.json` & `cysecuretools-4.2.0/cysecuretools/targets/cyb06xx5/policy/policy_multi_CM0_CM4_smif.json`

 * *Files identical despite different names*

### Comparing `cysecuretools-4.1.0/cysecuretools/targets/cyb06xx5/policy/policy_single_CM0_CM4.json` & `cysecuretools-4.2.0/cysecuretools/targets/cyb06xx5/policy/policy_single_CM0_CM4.json`

 * *Files identical despite different names*

### Comparing `cysecuretools-4.1.0/cysecuretools/targets/cyb06xx5/policy/policy_single_CM0_CM4_smif.json` & `cysecuretools-4.2.0/cysecuretools/targets/cyb06xx5/policy/policy_single_CM0_CM4_smif.json`

 * *Files identical despite different names*

### Comparing `cysecuretools-4.1.0/cysecuretools/targets/cyb06xx5/prebuilt/CyBootloader_Release/CypressBootloader_CM0p.hex` & `cysecuretools-4.2.0/cysecuretools/targets/cyb06xx5/prebuilt/CyBootloader_Release/CypressBootloader_CM0p.hex`

 * *Files identical despite different names*

### Comparing `cysecuretools-4.1.0/cysecuretools/targets/cyb06xx5/prebuilt/CyBootloader_Release/CypressBootloader_CM0p.jwt` & `cysecuretools-4.2.0/cysecuretools/targets/cyb06xx5/prebuilt/CyBootloader_Release/CypressBootloader_CM0p.jwt`

 * *Files identical despite different names*

### Comparing `cysecuretools-4.1.0/cysecuretools/targets/cyb06xx5/prebuilt/CyBootloader_WithLogs/CypressBootloader_CM0p.hex` & `cysecuretools-4.2.0/cysecuretools/targets/cyb06xx5/prebuilt/CyBootloader_WithLogs/CypressBootloader_CM0p.hex`

 * *Files identical despite different names*

### Comparing `cysecuretools-4.1.0/cysecuretools/targets/cyb06xx5/prebuilt/CyBootloader_WithLogs/CypressBootloader_CM0p.jwt` & `cysecuretools-4.2.0/cysecuretools/targets/cyb06xx5/prebuilt/CyBootloader_WithLogs/CypressBootloader_CM0p.jwt`

 * *Files identical despite different names*

### Comparing `cysecuretools-4.1.0/cysecuretools/targets/cyb06xx5/target_builder.py` & `cysecuretools-4.2.0/cysecuretools/targets/cyb06xxa/target_builder.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,20 +10,19 @@
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 import os
-
 from cysecuretools.core import TargetBuilder
 from cysecuretools.core.enums import KeyAlgorithm
-from cysecuretools.targets.cyb06xx5.maps.memory_map import MemoryMap_cyb06xx5
-from cysecuretools.targets.cyb06xx5.maps.register_map import \
-    RegisterMap_cyb06xx5
+from cysecuretools.targets.cyb06xxa.maps.memory_map import MemoryMap_cyb06xxa
+from cysecuretools.targets.cyb06xxa.maps.register_map import \
+    RegisterMap_cyb06xxa
 from cysecuretools.targets.common.p64.policy_filter import PolicyFilter
 from cysecuretools.targets.common.p64.policy_parser import PolicyParser
 from cysecuretools.targets.common.p64.policy_validator import PolicyValidator
 from cysecuretools.execute.provisioning import ProvisioningMXS40v1
 from cysecuretools.execute.provisioning_packet import ProvisioningPacketMXS40v1
 from cysecuretools.execute.entrance_exam.exam_mxs40v1 import \
     EntranceExamMXS40v1
@@ -34,46 +33,45 @@
 from cysecuretools.execute.silicon_data_reader import SiliconDataReaderMXS40v1
 from cysecuretools.execute.image_signing.signtool_mxs40v1 import \
     SignToolMXS40v1
 from cysecuretools.execute.key_source.key_source_mxs40v1 import (
     KeySourceMXS40v1)
 
 
-class CYB06xx5_Builder(TargetBuilder):
-    """ CYB06xx5 target builder """
+class CYB06xxA_Builder(TargetBuilder):
+    """ CYB06xxA target builder """
 
     def get_default_policy(self):
         return os.path.join(
-            self.target_dir, 'policy', 'policy_single_CM0_CM4.json')
+            self.target_dir, 'policy', 'policy_single_CM0_CM4_swap.json')
 
     def get_ocds(self):
         return ['pyocd', 'openocd']
 
     def get_ocd_config(self):
         return {
             'openocd': {
                 'before_init': '',
                 'after_init': 'targets'
             }
         }
 
     def get_memory_map(self):
-        memory_map = MemoryMap_cyb06xx5()
+        memory_map = MemoryMap_cyb06xxa()
         return memory_map
 
     def get_register_map(self):
-        register_map = RegisterMap_cyb06xx5()
+        register_map = RegisterMap_cyb06xxa()
         return register_map
 
     def get_policy_parser(self, policy):
         policy_parser = PolicyParser(policy)
         return policy_parser
 
     def get_policy_validator(self, policy_parser, memory_map):
-
         policy_validator = PolicyValidator(policy_parser, memory_map)
         return policy_validator
 
     def get_policy_filter(self, policy_parser):
         policy_filter = PolicyFilter(policy_parser)
         return policy_filter
 
@@ -104,16 +102,16 @@
     def get_sign_tool(self):
         return SignToolMXS40v1
 
     def get_key_source(self, **kwargs):
         return KeySourceMXS40v1(kwargs['policy_parser'])
 
     def get_bootloader_provider(self):
-        from cysecuretools.execute.bootloader_provider_mxs40v1 import \
-            BootloaderProviderMXS40v1
+        from cysecuretools.execute.bootloader_provider_mxs40v1 import (
+            BootloaderProviderMXS40v1)
         return BootloaderProviderMXS40v1
 
     def get_version_provider(self):
         from cysecuretools.execute.version_provider.version_provider_mxs40v1 \
             import VersionProviderMXS40v1
         return VersionProviderMXS40v1
 
@@ -124,7 +122,11 @@
     def get_policy_generator(self, policy_parser):
         """ N/A for MXS40v1 platform """
         return None
 
     def get_test_packages(self):
         """ N/A for MXS40v1 platform """
         return None
+
+    def get_silicon_id(self):
+        """Gets the target silicon ID"""
+        return None
```

### Comparing `cysecuretools-4.1.0/cysecuretools/targets/cyb06xx7/maps/memory_map.py` & `cysecuretools-4.2.0/cysecuretools/targets/cyb06xx5/maps/memory_map.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,26 +12,38 @@
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 from cysecuretools.core import MemoryMapBaseP64
 
 
-class MemoryMap_cyb06xx7(MemoryMapBaseP64):
+class MemoryMap_cyb06xx5(MemoryMapBaseP64):
     @property
     def FLASH_ADDRESS(self):
         return 0x10000000
 
     @property
     def FLASH_SIZE(self):
-        return 0x000E0000
+        return 0x00070000
+
+    @property
+    def RAM_ADDR(self):
+        return 0x08000000
+
+    @property
+    def SRAM_ADDR(self):
+        return 0x0802c000
+
+    @property
+    def SRAM_SIZE(self):
+        return 0x00004000
 
     @property
     def PROVISION_JWT_PACKET_ADDRESS(self):
-        return 0x100FB600
+        return 0x14003600
 
     @property
     def PROVISION_JWT_PACKET_SIZE(self):
         return 0x4A00
 
     @property
     def SPE_IMAGE_ID(self):
@@ -45,31 +57,14 @@
     def EXTERNAL_MEM_START(self):
         return 0x18000000
 
     @property
     def VECTOR_TABLE_ADDR_ALIGNMENT(self):
         return 0x400
 
-    # SFB addresses
-    @property
-    def TOC1_ADDRESS(self):
-        return 0x16007800
-
-    @property
-    def TOC1_SFB_ADDRESS_OFFSET(self):
-        return 0x14
-
-    @property
-    def TOC1_HASH_OBJ_OFFSET(self):
-        return 0x08
-
-    @property
-    def SYSCALL_TABLE_ADDR(self):
-        return 0x16002400
-
     @property
     def MIN_INT_ERASE_SIZE(self):
         return 0x200
 
     @property
     def MIN_EXT_ERASE_SIZE(self):
         return 0x40000
```

### Comparing `cysecuretools-4.1.0/cysecuretools/targets/cyb06xx7/maps/register_map.py` & `cysecuretools-4.2.0/cysecuretools/targets/cyb06xx7/maps/register_map.py`

 * *Files identical despite different names*

### Comparing `cysecuretools-4.1.0/cysecuretools/targets/cyb06xx7/packets/cy_auth_1m_b0_sample.jwt` & `cysecuretools-4.2.0/cysecuretools/targets/cyb06xx7/packets/cy_auth_1m_b0_sample.jwt`

 * *Files identical despite different names*

### Comparing `cysecuretools-4.1.0/cysecuretools/targets/cyb06xx7/packets/entrance_exam.jwt` & `cysecuretools-4.2.0/cysecuretools/targets/cyb06xx7/packets/entrance_exam.jwt`

 * *Files identical despite different names*

### Comparing `cysecuretools-4.1.0/cysecuretools/targets/cyb06xx7/policy/policy_multi_CM0_CM4.json` & `cysecuretools-4.2.0/cysecuretools/targets/cyb06xx7/policy/policy_multi_CM0_CM4.json`

 * *Files identical despite different names*

### Comparing `cysecuretools-4.1.0/cysecuretools/targets/cyb06xx7/policy/policy_multi_CM0_CM4_smif.json` & `cysecuretools-4.2.0/cysecuretools/targets/cyb06xx7/policy/policy_multi_CM0_CM4_smif.json`

 * *Files identical despite different names*

### Comparing `cysecuretools-4.1.0/cysecuretools/targets/cyb06xx7/policy/policy_multi_CM0_CM4_smif_swap.json` & `cysecuretools-4.2.0/cysecuretools/targets/cyb06xx7/policy/policy_multi_CM0_CM4_smif_swap.json`

 * *Files identical despite different names*

### Comparing `cysecuretools-4.1.0/cysecuretools/targets/cyb06xx7/policy/policy_multi_CM0_CM4_swap.json` & `cysecuretools-4.2.0/cysecuretools/targets/cyb06xx7/policy/policy_multi_CM0_CM4_swap.json`

 * *Files identical despite different names*

### Comparing `cysecuretools-4.1.0/cysecuretools/targets/cyb06xx7/policy/policy_single_CM0_CM4.json` & `cysecuretools-4.2.0/cysecuretools/targets/cyb06xx7/policy/policy_single_CM0_CM4.json`

 * *Files identical despite different names*

### Comparing `cysecuretools-4.1.0/cysecuretools/targets/cyb06xx7/policy/policy_single_CM0_CM4_smif.json` & `cysecuretools-4.2.0/cysecuretools/targets/cyb06xx7/policy/policy_single_CM0_CM4_smif.json`

 * *Files identical despite different names*

### Comparing `cysecuretools-4.1.0/cysecuretools/targets/cyb06xx7/policy/policy_single_CM0_CM4_smif_swap.json` & `cysecuretools-4.2.0/cysecuretools/targets/cyb06xx7/policy/policy_single_CM0_CM4_smif_swap.json`

 * *Files identical despite different names*

### Comparing `cysecuretools-4.1.0/cysecuretools/targets/cyb06xx7/policy/policy_single_CM0_CM4_swap.json` & `cysecuretools-4.2.0/cysecuretools/targets/cyb06xx7/policy/policy_single_CM0_CM4_swap.json`

 * *Files identical despite different names*

### Comparing `cysecuretools-4.1.0/cysecuretools/targets/cyb06xx7/prebuilt/CyBootloader_Release/CypressBootloader_CM0p.hex` & `cysecuretools-4.2.0/cysecuretools/targets/cyb06xx7/prebuilt/CyBootloader_Release/CypressBootloader_CM0p.hex`

 * *Files identical despite different names*

### Comparing `cysecuretools-4.1.0/cysecuretools/targets/cyb06xx7/prebuilt/CyBootloader_Release/CypressBootloader_CM0p.jwt` & `cysecuretools-4.2.0/cysecuretools/targets/cyb06xx7/prebuilt/CyBootloader_Release/CypressBootloader_CM0p.jwt`

 * *Files identical despite different names*

### Comparing `cysecuretools-4.1.0/cysecuretools/targets/cyb06xx7/prebuilt/CyBootloader_WithLogs/CypressBootloader_CM0p.hex` & `cysecuretools-4.2.0/cysecuretools/targets/cyb06xx7/prebuilt/CyBootloader_WithLogs/CypressBootloader_CM0p.hex`

 * *Files identical despite different names*

### Comparing `cysecuretools-4.1.0/cysecuretools/targets/cyb06xx7/prebuilt/CyBootloader_WithLogs/CypressBootloader_CM0p.jwt` & `cysecuretools-4.2.0/cysecuretools/targets/cyb06xx7/prebuilt/CyBootloader_WithLogs/CypressBootloader_CM0p.jwt`

 * *Files identical despite different names*

### Comparing `cysecuretools-4.1.0/cysecuretools/targets/cyb06xx7/target_builder.py` & `cysecuretools-4.2.0/cysecuretools/targets/cyb06xx7/target_builder.py`

 * *Files 2% similar despite different names*

```diff
@@ -122,7 +122,11 @@
     def get_policy_generator(self, policy_parser):
         """ N/A for MXS40v1 platform """
         return None
 
     def get_test_packages(self):
         """ N/A for MXS40v1 platform """
         return None
+
+    def get_silicon_id(self):
+        """Gets the target silicon ID"""
+        return None
```

### Comparing `cysecuretools-4.1.0/cysecuretools/targets/cyb06xxa/maps/memory_map.py` & `cysecuretools-4.2.0/cysecuretools/targets/cyw20829/maps/register_map.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,58 +1,78 @@
 """
-Copyright (c) 2019-2020 Cypress Semiconductor Corporation
+Copyright (c) 2021 Cypress Semiconductor Corporation
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
 
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
-from cysecuretools.core import MemoryMapBaseP64
+from cysecuretools.core import RegisterMapBaseCYW20829
 
 
-class MemoryMap_cyb06xxa(MemoryMapBaseP64):
+class RegisterMap_cyw20829(RegisterMapBaseCYW20829):
+
+    @property
+    def BOOTROM_VERSION(self):
+        return 0x20000004
+
+    @property
+    def BOOTROM_BUILD(self):
+        return 0x20000008
+
+    @property
+    def CPUSS_PROTECTION(self):
+        return 0x401C2004
+
+    @property
+    def BOOTROW(self):
+        return 0x40810180
+
     @property
-    def FLASH_ADDRESS(self):
-        return 0x10000000
+    def TST_DEBUG_CTL(self):
+        return 0x40200404
 
     @property
-    def FLASH_SIZE(self):
-        return 0x001E0000
+    def TST_DEBUG_STATUS(self):
+        return 0x40200408
 
     @property
-    def PROVISION_JWT_PACKET_ADDRESS(self):
-        return 0x101FB600
+    def RES_SOFT_CTL(self):
+        return 0x40200410
 
     @property
-    def PROVISION_JWT_PACKET_SIZE(self):
-        return 0x4A00
+    def EFUSE_DIE_ID_0(self):
+        return 0x40810874
 
     @property
-    def SPE_IMAGE_ID(self):
-        return 1
+    def EFUSE_DIE_ID_1(self):
+        return 0x40810878
 
     @property
-    def NSPE_IMAGE_ID(self):
-        return 16
+    def EFUSE_DIE_ID_2(self):
+        return 0x4081087C
 
     @property
-    def EXTERNAL_MEM_START(self):
-        return 0x18000000
+    def EFUSE_DEVICE_ID(self):
+        return 0x40810870
 
     @property
-    def VECTOR_TABLE_ADDR_ALIGNMENT(self):
-        return 0x400
+    def EFUSE_CTRL_ADDR(self):
+        return 0x40810000
+    #
+    # LVD registers
+    #
 
     @property
-    def MIN_INT_ERASE_SIZE(self):
-        return 0x200
+    def PWR_LVD_CTL(self):
+        return 0x40201020
 
     @property
-    def MIN_EXT_ERASE_SIZE(self):
-        return 0x40000
+    def PWR_LVD_STATUS(self):
+        return 0x40200040
```

### Comparing `cysecuretools-4.1.0/cysecuretools/targets/cyb06xxa/maps/register_map.py` & `cysecuretools-4.2.0/cysecuretools/targets/cyb06xxa/maps/register_map.py`

 * *Files identical despite different names*

### Comparing `cysecuretools-4.1.0/cysecuretools/targets/cyb06xxa/packets/cy_auth_2m_b0_sample.jwt` & `cysecuretools-4.2.0/cysecuretools/targets/cyb06xxa/packets/cy_auth_2m_b0_sample.jwt`

 * *Files identical despite different names*

### Comparing `cysecuretools-4.1.0/cysecuretools/targets/cyb06xxa/packets/entrance_exam.jwt` & `cysecuretools-4.2.0/cysecuretools/targets/cyb06xxa/packets/entrance_exam.jwt`

 * *Files identical despite different names*

### Comparing `cysecuretools-4.1.0/cysecuretools/targets/cyb06xxa/policy/policy_multi_CM0_CM4_smif_swap.json` & `cysecuretools-4.2.0/cysecuretools/targets/cyb06xxa/policy/policy_multi_CM0_CM4_smif_swap.json`

 * *Files identical despite different names*

### Comparing `cysecuretools-4.1.0/cysecuretools/targets/cyb06xxa/policy/policy_multi_CM0_CM4_swap.json` & `cysecuretools-4.2.0/cysecuretools/targets/cyb06xxa/policy/policy_multi_CM0_CM4_swap.json`

 * *Files identical despite different names*

### Comparing `cysecuretools-4.1.0/cysecuretools/targets/cyb06xxa/policy/policy_single_CM0_CM4_smif_swap.json` & `cysecuretools-4.2.0/cysecuretools/targets/cyb06xxa/policy/policy_single_CM0_CM4_smif_swap.json`

 * *Files identical despite different names*

### Comparing `cysecuretools-4.1.0/cysecuretools/targets/cyb06xxa/policy/policy_single_CM0_CM4_swap.json` & `cysecuretools-4.2.0/cysecuretools/targets/cyb06xxa/policy/policy_single_CM0_CM4_swap.json`

 * *Files identical despite different names*

### Comparing `cysecuretools-4.1.0/cysecuretools/targets/cyb06xxa/prebuilt/CyBootloader_Release_swap/CypressBootloader_CM0p.hex` & `cysecuretools-4.2.0/cysecuretools/targets/cyb06xxa/prebuilt/CyBootloader_Release_swap/CypressBootloader_CM0p.hex`

 * *Files identical despite different names*

### Comparing `cysecuretools-4.1.0/cysecuretools/targets/cyb06xxa/prebuilt/CyBootloader_Release_swap/CypressBootloader_CM0p.jwt` & `cysecuretools-4.2.0/cysecuretools/targets/cyb06xxa/prebuilt/CyBootloader_Release_swap/CypressBootloader_CM0p.jwt`

 * *Files identical despite different names*

### Comparing `cysecuretools-4.1.0/cysecuretools/targets/cyb06xxa/prebuilt/CyBootloader_WithLogs_swap/CypressBootloader_CM0p.hex` & `cysecuretools-4.2.0/cysecuretools/targets/cyb06xxa/prebuilt/CyBootloader_WithLogs_swap/CypressBootloader_CM0p.hex`

 * *Files identical despite different names*

### Comparing `cysecuretools-4.1.0/cysecuretools/targets/cyb06xxa/prebuilt/CyBootloader_WithLogs_swap/CypressBootloader_CM0p.jwt` & `cysecuretools-4.2.0/cysecuretools/targets/cyb06xxa/prebuilt/CyBootloader_WithLogs_swap/CypressBootloader_CM0p.jwt`

 * *Files identical despite different names*

### Comparing `cysecuretools-4.1.0/cysecuretools/targets/cyb06xxa/target_builder.py` & `cysecuretools-4.2.0/cysecuretools/targets/cys06xxa/target_builder.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-Copyright (c) 2019-2021 Cypress Semiconductor Corporation
+Copyright (c) 2020-2021 Cypress Semiconductor Corporation
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
 
@@ -33,16 +33,16 @@
 from cysecuretools.execute.silicon_data_reader import SiliconDataReaderMXS40v1
 from cysecuretools.execute.image_signing.signtool_mxs40v1 import \
     SignToolMXS40v1
 from cysecuretools.execute.key_source.key_source_mxs40v1 import (
     KeySourceMXS40v1)
 
 
-class CYB06xxA_Builder(TargetBuilder):
-    """ CYB06xxA target builder """
+class CYS06xxA_Builder(TargetBuilder):
+    """ CYS06xxA target builder """
 
     def get_default_policy(self):
         return os.path.join(
             self.target_dir, 'policy', 'policy_single_CM0_CM4_swap.json')
 
     def get_ocds(self):
         return ['pyocd', 'openocd']
@@ -122,7 +122,11 @@
     def get_policy_generator(self, policy_parser):
         """ N/A for MXS40v1 platform """
         return None
 
     def get_test_packages(self):
         """ N/A for MXS40v1 platform """
         return None
+
+    def get_silicon_id(self):
+        """Gets the target silicon ID"""
+        return None
```

### Comparing `cysecuretools-4.1.0/cysecuretools/targets/cys06xxa/packets/cy_auth_2m_s0_sample.jwt` & `cysecuretools-4.2.0/cysecuretools/targets/cys06xxa/packets/cy_auth_2m_s0_sample.jwt`

 * *Files identical despite different names*

### Comparing `cysecuretools-4.1.0/cysecuretools/targets/cys06xxa/packets/entrance_exam.jwt` & `cysecuretools-4.2.0/cysecuretools/targets/cys06xxa/packets/entrance_exam.jwt`

 * *Files identical despite different names*

### Comparing `cysecuretools-4.1.0/cysecuretools/targets/cys06xxa/policy/policy_multi_CM0_CM4_smif_swap.json` & `cysecuretools-4.2.0/cysecuretools/targets/cys06xxa/policy/policy_multi_CM0_CM4_smif_swap.json`

 * *Files identical despite different names*

### Comparing `cysecuretools-4.1.0/cysecuretools/targets/cys06xxa/policy/policy_multi_CM0_CM4_swap.json` & `cysecuretools-4.2.0/cysecuretools/targets/cys06xxa/policy/policy_multi_CM0_CM4_swap.json`

 * *Files identical despite different names*

### Comparing `cysecuretools-4.1.0/cysecuretools/targets/cys06xxa/policy/policy_single_CM0_CM4_smif_swap.json` & `cysecuretools-4.2.0/cysecuretools/targets/cys06xxa/policy/policy_single_CM0_CM4_smif_swap.json`

 * *Files identical despite different names*

### Comparing `cysecuretools-4.1.0/cysecuretools/targets/cys06xxa/policy/policy_single_CM0_CM4_swap.json` & `cysecuretools-4.2.0/cysecuretools/targets/cys06xxa/policy/policy_single_CM0_CM4_swap.json`

 * *Files identical despite different names*

### Comparing `cysecuretools-4.1.0/cysecuretools/targets/cys06xxa/prebuilt/CyBootloader_Release_swap/CypressBootloader_CM0p.hex` & `cysecuretools-4.2.0/cysecuretools/targets/cys06xxa/prebuilt/CyBootloader_Release_swap/CypressBootloader_CM0p.hex`

 * *Files identical despite different names*

### Comparing `cysecuretools-4.1.0/cysecuretools/targets/cys06xxa/prebuilt/CyBootloader_Release_swap/CypressBootloader_CM0p.jwt` & `cysecuretools-4.2.0/cysecuretools/targets/cys06xxa/prebuilt/CyBootloader_Release_swap/CypressBootloader_CM0p.jwt`

 * *Files identical despite different names*

### Comparing `cysecuretools-4.1.0/cysecuretools/targets/cys06xxa/prebuilt/CyBootloader_WithLogs_swap/CypressBootloader_CM0p.hex` & `cysecuretools-4.2.0/cysecuretools/targets/cys06xxa/prebuilt/CyBootloader_WithLogs_swap/CypressBootloader_CM0p.hex`

 * *Files identical despite different names*

### Comparing `cysecuretools-4.1.0/cysecuretools/targets/cys06xxa/prebuilt/CyBootloader_WithLogs_swap/CypressBootloader_CM0p.jwt` & `cysecuretools-4.2.0/cysecuretools/targets/cys06xxa/prebuilt/CyBootloader_WithLogs_swap/CypressBootloader_CM0p.jwt`

 * *Files identical despite different names*

### Comparing `cysecuretools-4.1.0/cysecuretools/targets/cys06xxa/target_builder.py` & `cysecuretools-4.2.0/cysecuretools/targets/cyb06xx5/target_builder.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 """
-Copyright (c) 2020-2021 Cypress Semiconductor Corporation
+Copyright (c) 2019-2021 Cypress Semiconductor Corporation
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
 
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 import os
+
 from cysecuretools.core import TargetBuilder
 from cysecuretools.core.enums import KeyAlgorithm
-from cysecuretools.targets.cyb06xxa.maps.memory_map import MemoryMap_cyb06xxa
-from cysecuretools.targets.cyb06xxa.maps.register_map import \
-    RegisterMap_cyb06xxa
+from cysecuretools.targets.cyb06xx5.maps.memory_map import MemoryMap_cyb06xx5
+from cysecuretools.targets.cyb06xx5.maps.register_map import \
+    RegisterMap_cyb06xx5
 from cysecuretools.targets.common.p64.policy_filter import PolicyFilter
 from cysecuretools.targets.common.p64.policy_parser import PolicyParser
 from cysecuretools.targets.common.p64.policy_validator import PolicyValidator
 from cysecuretools.execute.provisioning import ProvisioningMXS40v1
 from cysecuretools.execute.provisioning_packet import ProvisioningPacketMXS40v1
 from cysecuretools.execute.entrance_exam.exam_mxs40v1 import \
     EntranceExamMXS40v1
@@ -33,45 +34,46 @@
 from cysecuretools.execute.silicon_data_reader import SiliconDataReaderMXS40v1
 from cysecuretools.execute.image_signing.signtool_mxs40v1 import \
     SignToolMXS40v1
 from cysecuretools.execute.key_source.key_source_mxs40v1 import (
     KeySourceMXS40v1)
 
 
-class CYS06xxA_Builder(TargetBuilder):
-    """ CYS06xxA target builder """
+class CYB06xx5_Builder(TargetBuilder):
+    """ CYB06xx5 target builder """
 
     def get_default_policy(self):
         return os.path.join(
-            self.target_dir, 'policy', 'policy_single_CM0_CM4_swap.json')
+            self.target_dir, 'policy', 'policy_single_CM0_CM4.json')
 
     def get_ocds(self):
         return ['pyocd', 'openocd']
 
     def get_ocd_config(self):
         return {
             'openocd': {
                 'before_init': '',
                 'after_init': 'targets'
             }
         }
 
     def get_memory_map(self):
-        memory_map = MemoryMap_cyb06xxa()
+        memory_map = MemoryMap_cyb06xx5()
         return memory_map
 
     def get_register_map(self):
-        register_map = RegisterMap_cyb06xxa()
+        register_map = RegisterMap_cyb06xx5()
         return register_map
 
     def get_policy_parser(self, policy):
         policy_parser = PolicyParser(policy)
         return policy_parser
 
     def get_policy_validator(self, policy_parser, memory_map):
+
         policy_validator = PolicyValidator(policy_parser, memory_map)
         return policy_validator
 
     def get_policy_filter(self, policy_parser):
         policy_filter = PolicyFilter(policy_parser)
         return policy_filter
 
@@ -102,16 +104,16 @@
     def get_sign_tool(self):
         return SignToolMXS40v1
 
     def get_key_source(self, **kwargs):
         return KeySourceMXS40v1(kwargs['policy_parser'])
 
     def get_bootloader_provider(self):
-        from cysecuretools.execute.bootloader_provider_mxs40v1 import (
-            BootloaderProviderMXS40v1)
+        from cysecuretools.execute.bootloader_provider_mxs40v1 import \
+            BootloaderProviderMXS40v1
         return BootloaderProviderMXS40v1
 
     def get_version_provider(self):
         from cysecuretools.execute.version_provider.version_provider_mxs40v1 \
             import VersionProviderMXS40v1
         return VersionProviderMXS40v1
 
@@ -122,7 +124,15 @@
     def get_policy_generator(self, policy_parser):
         """ N/A for MXS40v1 platform """
         return None
 
     def get_test_packages(self):
         """ N/A for MXS40v1 platform """
         return None
+
+    def get_silicon_id(self):
+        """Gets the target silicon ID"""
+        return {
+            'id': [0xE701, 0xE70D],
+            'rev': [0x12],
+            'family': 0x105
+        }
```

### Comparing `cysecuretools-4.1.0/cysecuretools/targets/cyw20829/flows/asset_map.py` & `cysecuretools-4.2.0/cysecuretools/targets/cyw20829/flows/asset_map.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 from cysecuretools.core.key_helper import get_key_bytearray
 from cysecuretools.core.key_helper import calc_key_hash
+from ...common.mxs40sv2.nv_counter_calc import NvCounterCalculator
 
 
 def asset_map(p, **kwargs):
     """
     RAM applications asset map
     @params p: Policy parser
     @return: Initialized asset map
@@ -194,27 +195,29 @@
         },
         "nv_counter": {
             "size": 4,
             "data": [
                 {
                     "name": "ANTI_ROLLBACK",
                     "shift": 0,
-                    "value": pow(2, p.get_nv_counter()) - 1
+                    "value": NvCounterCalculator.calculate(
+                        p.get_nv_counter(), p.get_bits_per_cnt(),
+                        kwargs.get('image_id'))
                 },
             ],
         },
         "oem_key_0_hash": {
             "size": 16,
             "data": [
                 {
                     "name": "KEY_MANAGEMENT_0",
                     "shift": 0,
                     "value": calc_key_hash(p.get_pub_key_0_path()
-                                       if p.get_program_oem_key_0_hash()
-                                       else None)
+                                           if p.get_program_oem_key_0_hash()
+                                           else None)
                 },
             ],
         },
         "oem_key_1_hash": {
             "size": 16,
             "data": [
                 {
```

### Comparing `cysecuretools-4.1.0/cysecuretools/targets/cyw20829/flows/load_app_data.py` & `cysecuretools-4.2.0/cysecuretools/targets/cyw20829/flows/load_app_data.py`

 * *Files identical despite different names*

### Comparing `cysecuretools-4.1.0/cysecuretools/targets/cyw20829/flows/prov_flows.json` & `cysecuretools-4.2.0/cysecuretools/targets/cyw20829/flows/prov_flows.json`

 * *Files identical despite different names*

### Comparing `cysecuretools-4.1.0/cysecuretools/targets/cyw20829/flows/reverse_asset_map.py` & `cysecuretools-4.2.0/cysecuretools/targets/cyw20829/flows/reverse_asset_map.py`

 * *Files identical despite different names*

### Comparing `cysecuretools-4.1.0/cysecuretools/targets/cyw20829/maps/memory_map.py` & `cysecuretools-4.2.0/cysecuretools/targets/cyw20829/maps/memory_map.py`

 * *Files identical despite different names*

### Comparing `cysecuretools-4.1.0/cysecuretools/targets/cyw20829/maps/register_map.py` & `cysecuretools-4.2.0/cysecuretools/targets/cyb06xx7/maps/memory_map.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,78 +1,88 @@
 """
-Copyright (c) 2021 Cypress Semiconductor Corporation
+Copyright 2019-2023 Cypress Semiconductor Corporation (an Infineon company)
+or an affiliate of Cypress Semiconductor Corporation. All rights reserved.
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
 
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
-from cysecuretools.core import RegisterMapBaseCYW20829
+from cysecuretools.core import MemoryMapBaseP64
 
 
-class RegisterMap_cyw20829(RegisterMapBaseCYW20829):
+class MemoryMap_cyb06xx7(MemoryMapBaseP64):
+    @property
+    def FLASH_ADDRESS(self):
+        return 0x10000000
+
+    @property
+    def FLASH_SIZE(self):
+        return 0x000E0000
+
+    @property
+    def RAM_ADDR(self):
+        return 0x08000000
 
     @property
-    def BOOTROM_VERSION(self):
-        return 0x20000004
+    def SRAM_ADDR(self):
+        return 0x0802c000
 
     @property
-    def BOOTROM_BUILD(self):
-        return 0x20000008
+    def SRAM_SIZE(self):
+        return 0x00004000
 
     @property
-    def CPUSS_PROTECTION(self):
-        return 0x401C2004
+    def PROVISION_JWT_PACKET_ADDRESS(self):
+        return 0x100FB600
 
     @property
-    def BOOTROW(self):
-        return 0x40810180
+    def PROVISION_JWT_PACKET_SIZE(self):
+        return 0x4A00
 
     @property
-    def TST_DEBUG_CTL(self):
-        return 0x40200404
+    def SPE_IMAGE_ID(self):
+        return 1
 
     @property
-    def TST_DEBUG_STATUS(self):
-        return 0x40200408
+    def NSPE_IMAGE_ID(self):
+        return 16
 
     @property
-    def RES_SOFT_CTL(self):
-        return 0x40200410
+    def EXTERNAL_MEM_START(self):
+        return 0x18000000
 
     @property
-    def EFUSE_DIE_ID_0(self):
-        return 0x40810874
+    def VECTOR_TABLE_ADDR_ALIGNMENT(self):
+        return 0x400
 
+    # SFB addresses
     @property
-    def EFUSE_DIE_ID_1(self):
-        return 0x40810878
+    def TOC1_ADDRESS(self):
+        return 0x16007800
 
     @property
-    def EFUSE_DIE_ID_2(self):
-        return 0x4081087C
+    def TOC1_SFB_ADDRESS_OFFSET(self):
+        return 0x14
 
     @property
-    def EFUSE_DEVICE_ID(self):
-        return 0x40810870
+    def TOC1_HASH_OBJ_OFFSET(self):
+        return 0x08
 
     @property
-    def EFUSE_CTRL_ADDR(self):
-        return 0x40810000
-    #
-    # LVD registers
-    #
+    def SYSCALL_TABLE_ADDR(self):
+        return 0x16002400
 
     @property
-    def PWR_LVD_CTL(self):
-        return 0x40201020
+    def MIN_INT_ERASE_SIZE(self):
+        return 0x200
 
     @property
-    def PWR_LVD_STATUS(self):
-        return 0x40200040
+    def MIN_EXT_ERASE_SIZE(self):
+        return 0x40000
```

### Comparing `cysecuretools-4.1.0/cysecuretools/targets/cyw20829/packets/apps/prov_oem/cyapp_prov_oem_signed_icv0.bin` & `cysecuretools-4.2.0/cysecuretools/targets/cyw20829_a0/packets/apps/prov_oem/cyapp_prov_oem_signed_icv0.bin`

 * *Files identical despite different names*

### Comparing `cysecuretools-4.1.0/cysecuretools/targets/cyw20829/packets/apps/reprovisioning/cyapp_reprovisioning_signed_icv0.bin` & `cysecuretools-4.2.0/cysecuretools/targets/cyw20829_a0/packets/apps/reprovisioning/cyapp_reprovisioning_signed_icv0.bin`

 * *Files identical despite different names*

### Comparing `cysecuretools-4.1.0/cysecuretools/targets/cyw20829/packets/apps/to_rma/cyapp_to_rma_signed_icv0.bin` & `cysecuretools-4.2.0/cysecuretools/targets/cyw20829_a0/packets/apps/to_rma/cyapp_to_rma_signed_icv0.bin`

 * *Files identical despite different names*

### Comparing `cysecuretools-4.1.0/cysecuretools/targets/cyw20829/packets/debug_cert.json` & `cysecuretools-4.2.0/cysecuretools/targets/cyw20829_a0/packets/debug_cert.json`

 * *Files identical despite different names*

### Comparing `cysecuretools-4.1.0/cysecuretools/targets/cyw20829/policy/policy_hci_secure.json` & `cysecuretools-4.2.0/cysecuretools/targets/cyw20829/policy/policy_hci_secure.json`

 * *Files identical despite different names*

### Comparing `cysecuretools-4.1.0/cysecuretools/targets/cyw20829/policy/policy_no_secure.json` & `cysecuretools-4.2.0/cysecuretools/targets/cyw20829/policy/policy_no_secure.json`

 * *Files identical despite different names*

### Comparing `cysecuretools-4.1.0/cysecuretools/targets/cyw20829/policy/policy_reprovisioning_secure.json` & `cysecuretools-4.2.0/cysecuretools/targets/cyw20829_a0/policy/policy_reprovisioning_secure.json`

 * *Files identical despite different names*

### Comparing `cysecuretools-4.1.0/cysecuretools/targets/cyw20829/policy/policy_secure.json` & `cysecuretools-4.2.0/cysecuretools/targets/cyw20829_a0/policy/policy_secure.json`

 * *Files identical despite different names*

### Comparing `cysecuretools-4.1.0/cysecuretools/targets/cyw20829/policy_generator.py` & `cysecuretools-4.2.0/cysecuretools/targets/cyw20829/policy_generator.py`

 * *Files identical despite different names*

### Comparing `cysecuretools-4.1.0/cysecuretools/targets/cyw20829/target_builder.py` & `cysecuretools-4.2.0/cysecuretools/targets/cyw20829/target_builder.py`

 * *Files 6% similar despite different names*

```diff
@@ -116,13 +116,21 @@
 
     def get_policy_generator(self, policy_parser):
         return PolicyGenerator(policy_parser)
 
     def get_test_packages(self):
         return {
             'testapps': {
-                'package': 'testapps_cyw20829', 'flow_name': 'testapps'
+                'package': 'testapps_cyw20829_b0', 'flow_name': 'testapps'
             },
             'testapps_si': {
-                'package': 'testapps_cyw20829', 'flow_name': 'testapps_si'
+                'package': 'testapps_cyw20829_b0', 'flow_name': 'testapps_si'
             }
         }
+
+    def get_silicon_id(self):
+        """Gets the target silicon ID"""
+        return {
+            'id': [0xEB43],
+            'rev': [0x21],
+            'family': 0x110
+        }
```

### Comparing `cysecuretools-4.1.0/cysecuretools/version.py` & `cysecuretools-4.2.0/cysecuretools/version.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """
-Copyright (c) 2022 Cypress Semiconductor Corporation
+Copyright (c) 2022-2023 Cypress Semiconductor Corporation
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
 
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
-__version__ = '4.1.0'
+__version__ = '4.2.0'
```

### Comparing `cysecuretools-4.1.0/cysecuretools.egg-info/SOURCES.txt` & `cysecuretools-4.2.0/cysecuretools.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+CHANGELOG.md
 LICENSE
 MANIFEST.in
 README.md
 pyproject.toml
 setup.py
 cysecuretools/__init__.py
 cysecuretools/__main__.py
@@ -20,25 +21,27 @@
 cysecuretools.egg-info/requires.txt
 cysecuretools.egg-info/top_level.txt
 cysecuretools/core/__init__.py
 cysecuretools/core/bitops.py
 cysecuretools/core/connect_helper.py
 cysecuretools/core/cy_bootloader_map_parser.py
 cysecuretools/core/dependecy_validator.py
+cysecuretools/core/deprecated.py
 cysecuretools/core/entrance_exam_base.py
 cysecuretools/core/enums.py
 cysecuretools/core/exceptions.py
 cysecuretools/core/json_helper.py
 cysecuretools/core/jsonpath.py
 cysecuretools/core/key_data.py
 cysecuretools/core/key_helper.py
 cysecuretools/core/logging_configurator.py
 cysecuretools/core/logging_formatter.py
 cysecuretools/core/memory_area.py
 cysecuretools/core/memory_map_base.py
+cysecuretools/core/mtb_tools_discovery.py
 cysecuretools/core/ocd_settings.py
 cysecuretools/core/policy_filter_base.py
 cysecuretools/core/policy_validator_base.py
 cysecuretools/core/progress_bar.py
 cysecuretools/core/project.py
 cysecuretools/core/register_map_base.py
 cysecuretools/core/signtool_base.py
@@ -153,20 +156,22 @@
 cysecuretools/targets/common/__init__.py
 cysecuretools/targets/common/mxs40sv2/__init__.py
 cysecuretools/targets/common/mxs40sv2/asset.py
 cysecuretools/targets/common/mxs40sv2/asset_builder.py
 cysecuretools/targets/common/mxs40sv2/asset_enums.py
 cysecuretools/targets/common/mxs40sv2/enums.py
 cysecuretools/targets/common/mxs40sv2/flow_parser.py
+cysecuretools/targets/common/mxs40sv2/nv_counter_calc.py
 cysecuretools/targets/common/mxs40sv2/policy_parser.py
 cysecuretools/targets/common/mxs40sv2/policy_validator.py
 cysecuretools/targets/common/mxs40sv2/dependencies_validator/__init__.py
 cysecuretools/targets/common/mxs40sv2/dependencies_validator/access_restrictions_validator.py
 cysecuretools/targets/common/mxs40sv2/dependencies_validator/encryption_key_validator.py
 cysecuretools/targets/common/mxs40sv2/dependencies_validator/hci_mode_validator.py
+cysecuretools/targets/common/mxs40sv2/dependencies_validator/nv_counter_validator.py
 cysecuretools/targets/common/mxs40sv2/dependencies_validator/pre_build_keys_exist_validator.py
 cysecuretools/targets/common/mxs40sv2/dependencies_validator/revoke_oem_encryption_validator.py
 cysecuretools/targets/common/mxs40sv2/json/cyw20829_no_secure.json_schema
 cysecuretools/targets/common/mxs40sv2/json/cyw20829_reprovisioning_no_secure.json_schema
 cysecuretools/targets/common/mxs40sv2/json/cyw20829_reprovisioning_secure.json_schema
 cysecuretools/targets/common/mxs40sv2/json/cyw20829_secure.json_schema
 cysecuretools/targets/common/p64/__init__.py
@@ -279,8 +284,33 @@
 cysecuretools/targets/cyw20829/packets/apps/to_rma/config.json
 cysecuretools/targets/cyw20829/packets/apps/to_rma/cyapp_to_rma_signed_icv0.bin
 cysecuretools/targets/cyw20829/packets/apps/to_rma/info.txt
 cysecuretools/targets/cyw20829/policy/policy_hci_secure.json
 cysecuretools/targets/cyw20829/policy/policy_no_secure.json
 cysecuretools/targets/cyw20829/policy/policy_reprovisioning_no_secure.json
 cysecuretools/targets/cyw20829/policy/policy_reprovisioning_secure.json
-cysecuretools/targets/cyw20829/policy/policy_secure.json
+cysecuretools/targets/cyw20829/policy/policy_secure.json
+cysecuretools/targets/cyw20829_a0/__init__.py
+cysecuretools/targets/cyw20829_a0/target_builder.py
+cysecuretools/targets/cyw20829_a0/flows/oem_assets.json
+cysecuretools/targets/cyw20829_a0/flows/prov_flows.json
+cysecuretools/targets/cyw20829_a0/flows/reprovisioning_assets.json
+cysecuretools/targets/cyw20829_a0/keys/pub_hci_0.pem
+cysecuretools/targets/cyw20829_a0/keys/pub_hci_1.pem
+cysecuretools/targets/cyw20829_a0/packets/debug_cert.json
+cysecuretools/targets/cyw20829_a0/packets/rsa_key_tmpl.json
+cysecuretools/targets/cyw20829_a0/packets/apps/prov_oem/config.json
+cysecuretools/targets/cyw20829_a0/packets/apps/prov_oem/cyapp_prov_oem_signed_icv0.bin
+cysecuretools/targets/cyw20829_a0/packets/apps/prov_oem/info.txt
+cysecuretools/targets/cyw20829_a0/packets/apps/reprovisioning/config.json
+cysecuretools/targets/cyw20829_a0/packets/apps/reprovisioning/cyapp_reprovisioning_signed_icv0.bin
+cysecuretools/targets/cyw20829_a0/packets/apps/reprovisioning/info.txt
+cysecuretools/targets/cyw20829_a0/packets/apps/to_rma/config.json
+cysecuretools/targets/cyw20829_a0/packets/apps/to_rma/cyapp_to_rma_signed_icv0.bin
+cysecuretools/targets/cyw20829_a0/packets/apps/to_rma/info.txt
+cysecuretools/targets/cyw20829_a0/policy/policy_hci_secure.json
+cysecuretools/targets/cyw20829_a0/policy/policy_no_secure.json
+cysecuretools/targets/cyw20829_a0/policy/policy_reprovisioning_no_secure.json
+cysecuretools/targets/cyw20829_a0/policy/policy_reprovisioning_secure.json
+cysecuretools/targets/cyw20829_a0/policy/policy_secure.json
+docs/README_CYW20829.md
+docs/README_PSOC64.md
```

### Comparing `cysecuretools-4.1.0/setup.py` & `cysecuretools-4.2.0/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """
-Copyright (c) 2019-2022 Cypress Semiconductor Corporation
+Copyright 2019-2023 Cypress Semiconductor Corporation (an Infineon company)
+or an affiliate of Cypress Semiconductor Corporation. All rights reserved.
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
 
@@ -27,15 +28,14 @@
     exec(f.read(), version)  # pylint: disable=exec-used
 
 setup(
     name='cysecuretools',
     version=version['__version__'],
     install_requires=[
         'setuptools==59.6.0',
-        'psutil==5.9.0',
         'cryptography==36.0.1',
         'click==8.0.4',
         'intelhex==2.3.0',
         'python-jose==3.3.0',
         'jsonschema>=4.0.0,<=4.4.0',
         'pyocd==0.32.3',
         'cbor==1.0.0',
```

