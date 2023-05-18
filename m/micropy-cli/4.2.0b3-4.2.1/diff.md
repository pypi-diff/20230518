# Comparing `tmp/micropy_cli-4.2.0b3.tar.gz` & `tmp/micropy_cli-4.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "micropy_cli-4.2.0b3.tar", max compression
+gzip compressed data, was "micropy_cli-4.2.1.tar", max compression
```

## Comparing `micropy_cli-4.2.0b3.tar` & `micropy_cli-4.2.1.tar`

### file list

```diff
@@ -1,124 +1,124 @@
--rw-r--r--   0        0        0    45021 2023-04-17 20:07:39.160921 micropy_cli-4.2.0b3/CHANGELOG.md
--rw-r--r--   0        0        0     1068 2023-04-17 20:07:39.160921 micropy_cli-4.2.0b3/LICENSE
--rw-r--r--   0        0        0     9356 2023-04-17 20:07:39.160921 micropy_cli-4.2.0b3/README.md
--rw-r--r--   0        0        0      503 2023-04-17 20:07:39.160921 micropy_cli-4.2.0b3/micropy/__init__.py
--rw-r--r--   0        0        0      128 2023-04-17 20:07:39.160921 micropy_cli-4.2.0b3/micropy/__main__.py
--rw-r--r--   0        0        0       41 2023-04-17 20:07:39.160921 micropy_cli-4.2.0b3/micropy/app/__init__.py
--rw-r--r--   0        0        0     9530 2023-04-17 20:07:39.160921 micropy_cli-4.2.0b3/micropy/app/main.py
--rw-r--r--   0        0        0     8531 2023-04-17 20:07:39.160921 micropy_cli-4.2.0b3/micropy/app/stubs.py
--rw-r--r--   0        0        0      225 2023-04-17 20:07:39.160921 micropy_cli-4.2.0b3/micropy/config/__init__.py
--rw-r--r--   0        0        0     5626 2023-04-17 20:07:39.160921 micropy_cli-4.2.0b3/micropy/config/config.py
--rw-r--r--   0        0        0      623 2023-04-17 20:07:39.160921 micropy_cli-4.2.0b3/micropy/config/config_dict.py
--rw-r--r--   0        0        0     1804 2023-04-17 20:07:39.160921 micropy_cli-4.2.0b3/micropy/config/config_json.py
--rw-r--r--   0        0        0     1595 2023-04-17 20:07:39.160921 micropy_cli-4.2.0b3/micropy/config/config_source.py
--rw-r--r--   0        0        0      622 2023-04-17 20:07:39.160921 micropy_cli-4.2.0b3/micropy/data/__init__.py
--rw-r--r--   0        0        0     1849 2023-04-17 20:07:39.160921 micropy_cli-4.2.0b3/micropy/data/schemas/firmware.json
--rw-r--r--   0        0        0     1812 2023-04-17 20:07:39.164921 micropy_cli-4.2.0b3/micropy/data/schemas/stubs.json
--rw-r--r--   0        0        0      409 2023-04-17 20:07:39.164921 micropy_cli-4.2.0b3/micropy/data/sources.json
--rw-r--r--   0        0        0     2190 2023-04-17 20:07:39.164921 micropy_cli-4.2.0b3/micropy/exceptions.py
--rw-r--r--   0        0        0     8894 2023-04-17 20:07:39.164921 micropy_cli-4.2.0b3/micropy/logger.py
--rw-r--r--   0        0        0     2902 2023-04-17 20:07:39.164921 micropy_cli-4.2.0b3/micropy/main.py
--rw-r--r--   0        0        0     1418 2023-04-17 20:07:39.164921 micropy_cli-4.2.0b3/micropy/packages/__init__.py
--rw-r--r--   0        0        0     2987 2023-04-17 20:07:39.164921 micropy_cli-4.2.0b3/micropy/packages/package.py
--rw-r--r--   0        0        0     2045 2023-04-17 20:07:39.164921 micropy_cli-4.2.0b3/micropy/packages/source.py
--rw-r--r--   0        0        0     4752 2023-04-17 20:07:39.164921 micropy_cli-4.2.0b3/micropy/packages/source_package.py
--rw-r--r--   0        0        0      789 2023-04-17 20:07:39.164921 micropy_cli-4.2.0b3/micropy/packages/source_path.py
--rw-r--r--   0        0        0      133 2023-04-17 20:07:39.164921 micropy_cli-4.2.0b3/micropy/project/__init__.py
--rw-r--r--   0        0        0     2080 2023-04-17 20:07:39.164921 micropy_cli-4.2.0b3/micropy/project/checks.py
--rw-r--r--   0        0        0      339 2023-04-17 20:07:39.164921 micropy_cli-4.2.0b3/micropy/project/modules/__init__.py
--rw-r--r--   0        0        0     8354 2023-04-17 20:07:39.164921 micropy_cli-4.2.0b3/micropy/project/modules/modules.py
--rw-r--r--   0        0        0     7912 2023-04-17 20:07:39.164921 micropy_cli-4.2.0b3/micropy/project/modules/packages.py
--rw-r--r--   0        0        0     4529 2023-04-17 20:07:39.164921 micropy_cli-4.2.0b3/micropy/project/modules/stubs.py
--rw-r--r--   0        0        0     2454 2023-04-17 20:07:39.164921 micropy_cli-4.2.0b3/micropy/project/modules/templates.py
--rw-r--r--   0        0        0     4659 2023-04-17 20:07:39.164921 micropy_cli-4.2.0b3/micropy/project/project.py
--rw-r--r--   0        0        0     2185 2023-04-17 20:07:39.164921 micropy_cli-4.2.0b3/micropy/project/template/.gitignore
--rw-r--r--   0        0        0     1323 2023-04-17 20:07:39.164921 micropy_cli-4.2.0b3/micropy/project/template/.pylintrc
--rw-r--r--   0        0        0      488 2023-04-17 20:07:39.164921 micropy_cli-4.2.0b3/micropy/project/template/.vscode/extensions.json
--rw-r--r--   0        0        0      538 2023-04-17 20:07:39.164921 micropy_cli-4.2.0b3/micropy/project/template/.vscode/settings.json
--rw-r--r--   0        0        0      431 2023-04-17 20:07:39.164921 micropy_cli-4.2.0b3/micropy/project/template/pymakr.conf
--rw-r--r--   0        0        0       30 2023-04-17 20:07:39.164921 micropy_cli-4.2.0b3/micropy/project/template/src/boot.py
--rw-r--r--   0        0        0       10 2023-04-17 20:07:39.164921 micropy_cli-4.2.0b3/micropy/project/template/src/main.py
--rw-r--r--   0        0        0    10788 2023-04-17 20:07:39.164921 micropy_cli-4.2.0b3/micropy/project/template.py
--rw-r--r--   0        0        0        0 2023-04-17 20:07:39.164921 micropy_cli-4.2.0b3/micropy/py.typed
--rw-r--r--   0        0        0      612 2023-04-17 20:07:39.164921 micropy_cli-4.2.0b3/micropy/pyd/__init__.py
--rw-r--r--   0        0        0     3771 2023-04-17 20:07:39.164921 micropy_cli-4.2.0b3/micropy/pyd/abc.py
--rw-r--r--   0        0        0     6794 2023-04-17 20:07:39.164921 micropy_cli-4.2.0b3/micropy/pyd/backend_rshell.py
--rw-r--r--   0        0        0    12055 2023-04-17 20:07:39.164921 micropy_cli-4.2.0b3/micropy/pyd/backend_upydevice.py
--rw-r--r--   0        0        0     2497 2023-04-17 20:07:39.164921 micropy_cli-4.2.0b3/micropy/pyd/consumers.py
--rw-r--r--   0        0        0     3096 2023-04-17 20:07:39.164921 micropy_cli-4.2.0b3/micropy/pyd/pydevice.py
--rw-r--r--   0        0        0      776 2023-04-17 20:07:39.164921 micropy_cli-4.2.0b3/micropy/stubs/__init__.py
--rw-r--r--   0        0        0     1227 2023-04-17 20:07:39.164921 micropy_cli-4.2.0b3/micropy/stubs/manifest.py
--rw-r--r--   0        0        0      384 2023-04-17 20:07:39.164921 micropy_cli-4.2.0b3/micropy/stubs/package.py
--rw-r--r--   0        0        0     4916 2023-04-17 20:07:39.164921 micropy_cli-4.2.0b3/micropy/stubs/repo.py
--rw-r--r--   0        0        0     1410 2023-04-17 20:07:39.164921 micropy_cli-4.2.0b3/micropy/stubs/repo_package.py
--rw-r--r--   0        0        0      269 2023-04-17 20:07:39.164921 micropy_cli-4.2.0b3/micropy/stubs/repositories/__init__.py
--rw-r--r--   0        0        0     1049 2023-04-17 20:07:39.164921 micropy_cli-4.2.0b3/micropy/stubs/repositories/micropy.py
--rw-r--r--   0        0        0     1354 2023-04-17 20:07:39.164921 micropy_cli-4.2.0b3/micropy/stubs/repositories/micropython.py
--rw-r--r--   0        0        0      462 2023-04-17 20:07:39.164921 micropy_cli-4.2.0b3/micropy/stubs/repository_info.py
--rw-r--r--   0        0        0     4965 2023-04-17 20:07:39.164921 micropy_cli-4.2.0b3/micropy/stubs/source.py
--rw-r--r--   0        0        0    18379 2023-04-17 20:07:39.164921 micropy_cli-4.2.0b3/micropy/stubs/stubs.py
--rw-r--r--   0        0        0      584 2023-04-17 20:07:39.164921 micropy_cli-4.2.0b3/micropy/utils/__init__.py
--rw-r--r--   0        0        0      302 2023-04-17 20:07:39.164921 micropy_cli-4.2.0b3/micropy/utils/_compat.py
--rw-r--r--   0        0        0      382 2023-04-17 20:07:39.164921 micropy_cli-4.2.0b3/micropy/utils/decorators.py
--rw-r--r--   0        0        0    10917 2023-04-17 20:07:39.164921 micropy_cli-4.2.0b3/micropy/utils/helpers.py
--rw-r--r--   0        0        0     3635 2023-04-17 20:07:39.164921 micropy_cli-4.2.0b3/micropy/utils/stub.py
--rw-r--r--   0        0        0      389 2023-04-17 20:07:39.164921 micropy_cli-4.2.0b3/micropy/utils/types.py
--rw-r--r--   0        0        0     1054 2023-04-17 20:07:39.164921 micropy_cli-4.2.0b3/micropy/utils/validate.py
--rw-r--r--   0        0        0     5846 2023-04-17 20:07:39.164921 micropy_cli-4.2.0b3/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-17 20:07:39.164921 micropy_cli-4.2.0b3/tests/__init__.py
--rw-r--r--   0        0        0     1840 2023-04-17 20:07:39.164921 micropy_cli-4.2.0b3/tests/app/conftest.py
--rw-r--r--   0        0        0     8443 2023-04-17 20:07:39.164921 micropy_cli-4.2.0b3/tests/app/test_main.py
--rw-r--r--   0        0        0     6161 2023-04-17 20:07:39.164921 micropy_cli-4.2.0b3/tests/app/test_stubs.py
--rw-r--r--   0        0        0    10049 2023-04-17 20:07:39.164921 micropy_cli-4.2.0b3/tests/conftest.py
--rw-r--r--   0        0        0    45229 2023-04-17 20:07:39.164921 micropy_cli-4.2.0b3/tests/data/archive_test_stub.tar.gz
--rw-r--r--   0        0        0      882 2023-04-17 20:07:39.164921 micropy_cli-4.2.0b3/tests/data/esp32_test_stub/frozen/ntptime.py
--rw-r--r--   0        0        0      231 2023-04-17 20:07:39.164921 micropy_cli-4.2.0b3/tests/data/esp32_test_stub/frozen/ntptime.pyi
--rw-r--r--   0        0        0      553 2023-04-17 20:07:39.164921 micropy_cli-4.2.0b3/tests/data/esp32_test_stub/info.json
--rw-r--r--   0        0        0      347 2023-04-17 20:07:39.164921 micropy_cli-4.2.0b3/tests/data/esp32_test_stub/stubs/machine.py
--rw-r--r--   0        0        0     3346 2023-04-17 20:07:39.164921 micropy_cli-4.2.0b3/tests/data/esp32_test_stub/stubs/modules.json
--rw-r--r--   0        0        0      157 2023-04-17 20:07:39.164921 micropy_cli-4.2.0b3/tests/data/esp8266_invalid_stub/info.json
--rw-r--r--   0        0        0      882 2023-04-17 20:07:39.168921 micropy_cli-4.2.0b3/tests/data/esp8266_test_stub/frozen/ntptime.py
--rw-r--r--   0        0        0      231 2023-04-17 20:07:39.168921 micropy_cli-4.2.0b3/tests/data/esp8266_test_stub/frozen/ntptime.pyi
--rw-r--r--   0        0        0      570 2023-04-17 20:07:39.168921 micropy_cli-4.2.0b3/tests/data/esp8266_test_stub/info.json
--rw-r--r--   0        0        0      347 2023-04-17 20:07:39.168921 micropy_cli-4.2.0b3/tests/data/esp8266_test_stub/stubs/machine.py
--rw-r--r--   0        0        0     3346 2023-04-17 20:07:39.168921 micropy_cli-4.2.0b3/tests/data/esp8266_test_stub/stubs/modules.json
--rw-r--r--   0        0        0     2219 2023-04-17 20:07:39.168921 micropy_cli-4.2.0b3/tests/data/fware_test_stub/frozen/utarfile.py
--rw-r--r--   0        0        0     1276 2023-04-17 20:07:39.168921 micropy_cli-4.2.0b3/tests/data/fware_test_stub/frozen/utarfile.pyi
--rw-r--r--   0        0        0     1868 2023-04-17 20:07:39.168921 micropy_cli-4.2.0b3/tests/data/fware_test_stub/frozen/utokenize.py
--rw-r--r--   0        0        0      313 2023-04-17 20:07:39.168921 micropy_cli-4.2.0b3/tests/data/fware_test_stub/frozen/utokenize.pyi
--rw-r--r--   0        0        0     1331 2023-04-17 20:07:39.168921 micropy_cli-4.2.0b3/tests/data/fware_test_stub/info.json
--rw-r--r--   0        0        0      483 2023-04-17 20:07:39.168921 micropy_cli-4.2.0b3/tests/data/project_test/.pylintrc
--rw-r--r--   0        0        0     1900 2023-04-17 20:07:39.168921 micropy_cli-4.2.0b3/tests/data/project_test/.vscode/settings.json
--rw-r--r--   0        0        0      334 2023-04-17 20:07:39.168921 micropy_cli-4.2.0b3/tests/data/project_test/micropy.json
--rw-r--r--   0        0        0      500 2023-04-17 20:07:39.168921 micropy_cli-4.2.0b3/tests/data/stubber_test_stub/micropython.py
--rw-r--r--   0        0        0      401 2023-04-17 20:07:39.168921 micropy_cli-4.2.0b3/tests/data/stubber_test_stub/modules.json
--rw-r--r--   0        0        0      560 2023-04-17 20:07:39.168921 micropy_cli-4.2.0b3/tests/data/test_repo.json
--rw-r--r--   0        0        0      846 2023-04-17 20:07:39.168921 micropy_cli-4.2.0b3/tests/data/test_source.xml
--rw-r--r--   0        0        0       94 2023-04-17 20:07:39.168921 micropy_cli-4.2.0b3/tests/data/test_sources.json
--rw-r--r--   0        0        0      474 2023-04-17 20:07:39.168921 micropy_cli-4.2.0b3/tests/test_checks.py
--rw-r--r--   0        0        0     3457 2023-04-17 20:07:39.168921 micropy_cli-4.2.0b3/tests/test_config.py
--rw-r--r--   0        0        0     5119 2023-04-17 20:07:39.168921 micropy_cli-4.2.0b3/tests/test_highlevel.py
--rw-r--r--   0        0        0     1399 2023-04-17 20:07:39.168921 micropy_cli-4.2.0b3/tests/test_main.py
--rw-r--r--   0        0        0     4760 2023-04-17 20:07:39.168921 micropy_cli-4.2.0b3/tests/test_packages.py
--rw-r--r--   0        0        0    10080 2023-04-17 20:07:39.168921 micropy_cli-4.2.0b3/tests/test_project.py
--rw-r--r--   0        0        0    17567 2023-04-17 20:07:39.168921 micropy_cli-4.2.0b3/tests/test_pyd.py
--rw-r--r--   0        0        0     1574 2023-04-17 20:07:39.168921 micropy_cli-4.2.0b3/tests/test_stub_source.py
--rw-r--r--   0        0        0      157 2023-04-17 20:07:39.168921 micropy_cli-4.2.0b3/tests/test_stubs/bad_test_stub/modules.json
--rw-r--r--   0        0        0      882 2023-04-17 20:07:39.168921 micropy_cli-4.2.0b3/tests/test_stubs/esp32_test_stub/frozen/ntptime.py
--rw-r--r--   0        0        0      231 2023-04-17 20:07:39.168921 micropy_cli-4.2.0b3/tests/test_stubs/esp32_test_stub/frozen/ntptime.pyi
--rw-r--r--   0        0        0      553 2023-04-17 20:07:39.168921 micropy_cli-4.2.0b3/tests/test_stubs/esp32_test_stub/info.json
--rw-r--r--   0        0        0      347 2023-04-17 20:07:39.168921 micropy_cli-4.2.0b3/tests/test_stubs/esp32_test_stub/stubs/machine.py
--rw-r--r--   0        0        0     3346 2023-04-17 20:07:39.168921 micropy_cli-4.2.0b3/tests/test_stubs/esp32_test_stub/stubs/modules.json
--rw-r--r--   0        0        0      882 2023-04-17 20:07:39.168921 micropy_cli-4.2.0b3/tests/test_stubs/esp8266_test_stub/frozen/ntptime.py
--rw-r--r--   0        0        0      231 2023-04-17 20:07:39.168921 micropy_cli-4.2.0b3/tests/test_stubs/esp8266_test_stub/frozen/ntptime.pyi
--rw-r--r--   0        0        0      570 2023-04-17 20:07:39.168921 micropy_cli-4.2.0b3/tests/test_stubs/esp8266_test_stub/info.json
--rw-r--r--   0        0        0      347 2023-04-17 20:07:39.168921 micropy_cli-4.2.0b3/tests/test_stubs/esp8266_test_stub/stubs/machine.py
--rw-r--r--   0        0        0     3346 2023-04-17 20:07:39.168921 micropy_cli-4.2.0b3/tests/test_stubs/esp8266_test_stub/stubs/modules.json
--rw-r--r--   0        0        0     8511 2023-04-17 20:07:39.168921 micropy_cli-4.2.0b3/tests/test_stubs.py
--rw-r--r--   0        0        0     2447 2023-04-17 20:07:39.168921 micropy_cli-4.2.0b3/tests/test_stubs_repo.py
--rw-r--r--   0        0        0     4534 2023-04-17 20:07:39.168921 micropy_cli-4.2.0b3/tests/test_template.py
--rw-r--r--   0        0        0      157 2023-04-17 20:07:39.168921 micropy_cli-4.2.0b3/tests/test_utils/fail.json
--rw-r--r--   0        0        0      395 2023-04-17 20:07:39.168921 micropy_cli-4.2.0b3/tests/test_utils/pass.json
--rw-r--r--   0        0        0     1088 2023-04-17 20:07:39.168921 micropy_cli-4.2.0b3/tests/test_utils/schema.json
--rw-r--r--   0        0        0    10261 2023-04-17 20:07:39.168921 micropy_cli-4.2.0b3/tests/test_utils.py
--rw-r--r--   0        0        0    11800 1970-01-01 00:00:00.000000 micropy_cli-4.2.0b3/PKG-INFO
+-rw-r--r--   0        0        0    47296 2023-05-18 07:38:18.931266 micropy_cli-4.2.1/CHANGELOG.md
+-rw-r--r--   0        0        0     1068 2023-05-18 07:38:18.931266 micropy_cli-4.2.1/LICENSE
+-rw-r--r--   0        0        0     9356 2023-05-18 07:38:18.931266 micropy_cli-4.2.1/README.md
+-rw-r--r--   0        0        0      503 2023-05-18 07:38:18.931266 micropy_cli-4.2.1/micropy/__init__.py
+-rw-r--r--   0        0        0      128 2023-05-18 07:38:18.931266 micropy_cli-4.2.1/micropy/__main__.py
+-rw-r--r--   0        0        0       41 2023-05-18 07:38:18.931266 micropy_cli-4.2.1/micropy/app/__init__.py
+-rw-r--r--   0        0        0     9530 2023-05-18 07:38:18.931266 micropy_cli-4.2.1/micropy/app/main.py
+-rw-r--r--   0        0        0     9695 2023-05-18 07:38:18.931266 micropy_cli-4.2.1/micropy/app/stubs.py
+-rw-r--r--   0        0        0      225 2023-05-18 07:38:18.931266 micropy_cli-4.2.1/micropy/config/__init__.py
+-rw-r--r--   0        0        0     5626 2023-05-18 07:38:18.931266 micropy_cli-4.2.1/micropy/config/config.py
+-rw-r--r--   0        0        0      623 2023-05-18 07:38:18.931266 micropy_cli-4.2.1/micropy/config/config_dict.py
+-rw-r--r--   0        0        0     1804 2023-05-18 07:38:18.931266 micropy_cli-4.2.1/micropy/config/config_json.py
+-rw-r--r--   0        0        0     1595 2023-05-18 07:38:18.931266 micropy_cli-4.2.1/micropy/config/config_source.py
+-rw-r--r--   0        0        0      622 2023-05-18 07:38:18.931266 micropy_cli-4.2.1/micropy/data/__init__.py
+-rw-r--r--   0        0        0     1849 2023-05-18 07:38:18.931266 micropy_cli-4.2.1/micropy/data/schemas/firmware.json
+-rw-r--r--   0        0        0     1812 2023-05-18 07:38:18.931266 micropy_cli-4.2.1/micropy/data/schemas/stubs.json
+-rw-r--r--   0        0        0      409 2023-05-18 07:38:18.931266 micropy_cli-4.2.1/micropy/data/sources.json
+-rw-r--r--   0        0        0     2190 2023-05-18 07:38:18.931266 micropy_cli-4.2.1/micropy/exceptions.py
+-rw-r--r--   0        0        0     8894 2023-05-18 07:38:18.931266 micropy_cli-4.2.1/micropy/logger.py
+-rw-r--r--   0        0        0     2902 2023-05-18 07:38:18.931266 micropy_cli-4.2.1/micropy/main.py
+-rw-r--r--   0        0        0     1418 2023-05-18 07:38:18.931266 micropy_cli-4.2.1/micropy/packages/__init__.py
+-rw-r--r--   0        0        0     2987 2023-05-18 07:38:18.931266 micropy_cli-4.2.1/micropy/packages/package.py
+-rw-r--r--   0        0        0     2045 2023-05-18 07:38:18.931266 micropy_cli-4.2.1/micropy/packages/source.py
+-rw-r--r--   0        0        0     4752 2023-05-18 07:38:18.931266 micropy_cli-4.2.1/micropy/packages/source_package.py
+-rw-r--r--   0        0        0      789 2023-05-18 07:38:18.931266 micropy_cli-4.2.1/micropy/packages/source_path.py
+-rw-r--r--   0        0        0      133 2023-05-18 07:38:18.931266 micropy_cli-4.2.1/micropy/project/__init__.py
+-rw-r--r--   0        0        0     2080 2023-05-18 07:38:18.931266 micropy_cli-4.2.1/micropy/project/checks.py
+-rw-r--r--   0        0        0      339 2023-05-18 07:38:18.931266 micropy_cli-4.2.1/micropy/project/modules/__init__.py
+-rw-r--r--   0        0        0     8354 2023-05-18 07:38:18.931266 micropy_cli-4.2.1/micropy/project/modules/modules.py
+-rw-r--r--   0        0        0     7912 2023-05-18 07:38:18.931266 micropy_cli-4.2.1/micropy/project/modules/packages.py
+-rw-r--r--   0        0        0     4529 2023-05-18 07:38:18.931266 micropy_cli-4.2.1/micropy/project/modules/stubs.py
+-rw-r--r--   0        0        0     2454 2023-05-18 07:38:18.931266 micropy_cli-4.2.1/micropy/project/modules/templates.py
+-rw-r--r--   0        0        0     4659 2023-05-18 07:38:18.931266 micropy_cli-4.2.1/micropy/project/project.py
+-rw-r--r--   0        0        0     2185 2023-05-18 07:38:18.931266 micropy_cli-4.2.1/micropy/project/template/.gitignore
+-rw-r--r--   0        0        0     1330 2023-05-18 07:38:18.931266 micropy_cli-4.2.1/micropy/project/template/.pylintrc
+-rw-r--r--   0        0        0      488 2023-05-18 07:38:18.931266 micropy_cli-4.2.1/micropy/project/template/.vscode/extensions.json
+-rw-r--r--   0        0        0      803 2023-05-18 07:38:18.931266 micropy_cli-4.2.1/micropy/project/template/.vscode/settings.json
+-rw-r--r--   0        0        0      431 2023-05-18 07:38:18.931266 micropy_cli-4.2.1/micropy/project/template/pymakr.conf
+-rw-r--r--   0        0        0       30 2023-05-18 07:38:18.931266 micropy_cli-4.2.1/micropy/project/template/src/boot.py
+-rw-r--r--   0        0        0       10 2023-05-18 07:38:18.931266 micropy_cli-4.2.1/micropy/project/template/src/main.py
+-rw-r--r--   0        0        0    10869 2023-05-18 07:38:18.931266 micropy_cli-4.2.1/micropy/project/template.py
+-rw-r--r--   0        0        0        0 2023-05-18 07:38:18.931266 micropy_cli-4.2.1/micropy/py.typed
+-rw-r--r--   0        0        0      612 2023-05-18 07:38:18.931266 micropy_cli-4.2.1/micropy/pyd/__init__.py
+-rw-r--r--   0        0        0     3771 2023-05-18 07:38:18.931266 micropy_cli-4.2.1/micropy/pyd/abc.py
+-rw-r--r--   0        0        0     6794 2023-05-18 07:38:18.931266 micropy_cli-4.2.1/micropy/pyd/backend_rshell.py
+-rw-r--r--   0        0        0    12055 2023-05-18 07:38:18.931266 micropy_cli-4.2.1/micropy/pyd/backend_upydevice.py
+-rw-r--r--   0        0        0     2497 2023-05-18 07:38:18.931266 micropy_cli-4.2.1/micropy/pyd/consumers.py
+-rw-r--r--   0        0        0     3096 2023-05-18 07:38:18.931266 micropy_cli-4.2.1/micropy/pyd/pydevice.py
+-rw-r--r--   0        0        0      776 2023-05-18 07:38:18.931266 micropy_cli-4.2.1/micropy/stubs/__init__.py
+-rw-r--r--   0        0        0     1227 2023-05-18 07:38:18.931266 micropy_cli-4.2.1/micropy/stubs/manifest.py
+-rw-r--r--   0        0        0      384 2023-05-18 07:38:18.931266 micropy_cli-4.2.1/micropy/stubs/package.py
+-rw-r--r--   0        0        0     4916 2023-05-18 07:38:18.931266 micropy_cli-4.2.1/micropy/stubs/repo.py
+-rw-r--r--   0        0        0     1410 2023-05-18 07:38:18.931266 micropy_cli-4.2.1/micropy/stubs/repo_package.py
+-rw-r--r--   0        0        0      269 2023-05-18 07:38:18.931266 micropy_cli-4.2.1/micropy/stubs/repositories/__init__.py
+-rw-r--r--   0        0        0     1049 2023-05-18 07:38:18.935267 micropy_cli-4.2.1/micropy/stubs/repositories/micropy.py
+-rw-r--r--   0        0        0     1354 2023-05-18 07:38:18.935267 micropy_cli-4.2.1/micropy/stubs/repositories/micropython.py
+-rw-r--r--   0        0        0      462 2023-05-18 07:38:18.935267 micropy_cli-4.2.1/micropy/stubs/repository_info.py
+-rw-r--r--   0        0        0     4965 2023-05-18 07:38:18.935267 micropy_cli-4.2.1/micropy/stubs/source.py
+-rw-r--r--   0        0        0    18672 2023-05-18 07:38:18.935267 micropy_cli-4.2.1/micropy/stubs/stubs.py
+-rw-r--r--   0        0        0      584 2023-05-18 07:38:18.935267 micropy_cli-4.2.1/micropy/utils/__init__.py
+-rw-r--r--   0        0        0      302 2023-05-18 07:38:18.935267 micropy_cli-4.2.1/micropy/utils/_compat.py
+-rw-r--r--   0        0        0      382 2023-05-18 07:38:18.935267 micropy_cli-4.2.1/micropy/utils/decorators.py
+-rw-r--r--   0        0        0    10917 2023-05-18 07:38:18.935267 micropy_cli-4.2.1/micropy/utils/helpers.py
+-rw-r--r--   0        0        0     3635 2023-05-18 07:38:18.935267 micropy_cli-4.2.1/micropy/utils/stub.py
+-rw-r--r--   0        0        0      389 2023-05-18 07:38:18.935267 micropy_cli-4.2.1/micropy/utils/types.py
+-rw-r--r--   0        0        0     1054 2023-05-18 07:38:18.935267 micropy_cli-4.2.1/micropy/utils/validate.py
+-rw-r--r--   0        0        0     5833 2023-05-18 07:38:18.935267 micropy_cli-4.2.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-18 07:38:18.935267 micropy_cli-4.2.1/tests/__init__.py
+-rw-r--r--   0        0        0     1840 2023-05-18 07:38:18.935267 micropy_cli-4.2.1/tests/app/conftest.py
+-rw-r--r--   0        0        0     8443 2023-05-18 07:38:18.935267 micropy_cli-4.2.1/tests/app/test_main.py
+-rw-r--r--   0        0        0     6161 2023-05-18 07:38:18.935267 micropy_cli-4.2.1/tests/app/test_stubs.py
+-rw-r--r--   0        0        0    10049 2023-05-18 07:38:18.935267 micropy_cli-4.2.1/tests/conftest.py
+-rw-r--r--   0        0        0    45229 2023-05-18 07:38:18.935267 micropy_cli-4.2.1/tests/data/archive_test_stub.tar.gz
+-rw-r--r--   0        0        0      882 2023-05-18 07:38:18.935267 micropy_cli-4.2.1/tests/data/esp32_test_stub/frozen/ntptime.py
+-rw-r--r--   0        0        0      231 2023-05-18 07:38:18.935267 micropy_cli-4.2.1/tests/data/esp32_test_stub/frozen/ntptime.pyi
+-rw-r--r--   0        0        0      553 2023-05-18 07:38:18.935267 micropy_cli-4.2.1/tests/data/esp32_test_stub/info.json
+-rw-r--r--   0        0        0      347 2023-05-18 07:38:18.935267 micropy_cli-4.2.1/tests/data/esp32_test_stub/stubs/machine.py
+-rw-r--r--   0        0        0     3346 2023-05-18 07:38:18.935267 micropy_cli-4.2.1/tests/data/esp32_test_stub/stubs/modules.json
+-rw-r--r--   0        0        0      157 2023-05-18 07:38:18.935267 micropy_cli-4.2.1/tests/data/esp8266_invalid_stub/info.json
+-rw-r--r--   0        0        0      882 2023-05-18 07:38:18.935267 micropy_cli-4.2.1/tests/data/esp8266_test_stub/frozen/ntptime.py
+-rw-r--r--   0        0        0      231 2023-05-18 07:38:18.935267 micropy_cli-4.2.1/tests/data/esp8266_test_stub/frozen/ntptime.pyi
+-rw-r--r--   0        0        0      570 2023-05-18 07:38:18.935267 micropy_cli-4.2.1/tests/data/esp8266_test_stub/info.json
+-rw-r--r--   0        0        0      347 2023-05-18 07:38:18.935267 micropy_cli-4.2.1/tests/data/esp8266_test_stub/stubs/machine.py
+-rw-r--r--   0        0        0     3346 2023-05-18 07:38:18.935267 micropy_cli-4.2.1/tests/data/esp8266_test_stub/stubs/modules.json
+-rw-r--r--   0        0        0     2219 2023-05-18 07:38:18.935267 micropy_cli-4.2.1/tests/data/fware_test_stub/frozen/utarfile.py
+-rw-r--r--   0        0        0     1276 2023-05-18 07:38:18.935267 micropy_cli-4.2.1/tests/data/fware_test_stub/frozen/utarfile.pyi
+-rw-r--r--   0        0        0     1868 2023-05-18 07:38:18.935267 micropy_cli-4.2.1/tests/data/fware_test_stub/frozen/utokenize.py
+-rw-r--r--   0        0        0      313 2023-05-18 07:38:18.935267 micropy_cli-4.2.1/tests/data/fware_test_stub/frozen/utokenize.pyi
+-rw-r--r--   0        0        0     1331 2023-05-18 07:38:18.935267 micropy_cli-4.2.1/tests/data/fware_test_stub/info.json
+-rw-r--r--   0        0        0      483 2023-05-18 07:38:18.935267 micropy_cli-4.2.1/tests/data/project_test/.pylintrc
+-rw-r--r--   0        0        0     1900 2023-05-18 07:38:18.935267 micropy_cli-4.2.1/tests/data/project_test/.vscode/settings.json
+-rw-r--r--   0        0        0      334 2023-05-18 07:38:18.935267 micropy_cli-4.2.1/tests/data/project_test/micropy.json
+-rw-r--r--   0        0        0      500 2023-05-18 07:38:18.935267 micropy_cli-4.2.1/tests/data/stubber_test_stub/micropython.py
+-rw-r--r--   0        0        0      401 2023-05-18 07:38:18.935267 micropy_cli-4.2.1/tests/data/stubber_test_stub/modules.json
+-rw-r--r--   0        0        0      560 2023-05-18 07:38:18.935267 micropy_cli-4.2.1/tests/data/test_repo.json
+-rw-r--r--   0        0        0      846 2023-05-18 07:38:18.935267 micropy_cli-4.2.1/tests/data/test_source.xml
+-rw-r--r--   0        0        0       94 2023-05-18 07:38:18.935267 micropy_cli-4.2.1/tests/data/test_sources.json
+-rw-r--r--   0        0        0      474 2023-05-18 07:38:18.935267 micropy_cli-4.2.1/tests/test_checks.py
+-rw-r--r--   0        0        0     3457 2023-05-18 07:38:18.935267 micropy_cli-4.2.1/tests/test_config.py
+-rw-r--r--   0        0        0     5119 2023-05-18 07:38:18.935267 micropy_cli-4.2.1/tests/test_highlevel.py
+-rw-r--r--   0        0        0     1399 2023-05-18 07:38:18.935267 micropy_cli-4.2.1/tests/test_main.py
+-rw-r--r--   0        0        0     4760 2023-05-18 07:38:18.935267 micropy_cli-4.2.1/tests/test_packages.py
+-rw-r--r--   0        0        0    10080 2023-05-18 07:38:18.935267 micropy_cli-4.2.1/tests/test_project.py
+-rw-r--r--   0        0        0    17567 2023-05-18 07:38:18.935267 micropy_cli-4.2.1/tests/test_pyd.py
+-rw-r--r--   0        0        0     1574 2023-05-18 07:38:18.935267 micropy_cli-4.2.1/tests/test_stub_source.py
+-rw-r--r--   0        0        0      157 2023-05-18 07:38:18.935267 micropy_cli-4.2.1/tests/test_stubs/bad_test_stub/modules.json
+-rw-r--r--   0        0        0      882 2023-05-18 07:38:18.935267 micropy_cli-4.2.1/tests/test_stubs/esp32_test_stub/frozen/ntptime.py
+-rw-r--r--   0        0        0      231 2023-05-18 07:38:18.935267 micropy_cli-4.2.1/tests/test_stubs/esp32_test_stub/frozen/ntptime.pyi
+-rw-r--r--   0        0        0      553 2023-05-18 07:38:18.935267 micropy_cli-4.2.1/tests/test_stubs/esp32_test_stub/info.json
+-rw-r--r--   0        0        0      347 2023-05-18 07:38:18.935267 micropy_cli-4.2.1/tests/test_stubs/esp32_test_stub/stubs/machine.py
+-rw-r--r--   0        0        0     3346 2023-05-18 07:38:18.935267 micropy_cli-4.2.1/tests/test_stubs/esp32_test_stub/stubs/modules.json
+-rw-r--r--   0        0        0      882 2023-05-18 07:38:18.935267 micropy_cli-4.2.1/tests/test_stubs/esp8266_test_stub/frozen/ntptime.py
+-rw-r--r--   0        0        0      231 2023-05-18 07:38:18.935267 micropy_cli-4.2.1/tests/test_stubs/esp8266_test_stub/frozen/ntptime.pyi
+-rw-r--r--   0        0        0      570 2023-05-18 07:38:18.935267 micropy_cli-4.2.1/tests/test_stubs/esp8266_test_stub/info.json
+-rw-r--r--   0        0        0      347 2023-05-18 07:38:18.935267 micropy_cli-4.2.1/tests/test_stubs/esp8266_test_stub/stubs/machine.py
+-rw-r--r--   0        0        0     3346 2023-05-18 07:38:18.935267 micropy_cli-4.2.1/tests/test_stubs/esp8266_test_stub/stubs/modules.json
+-rw-r--r--   0        0        0     8511 2023-05-18 07:38:18.935267 micropy_cli-4.2.1/tests/test_stubs.py
+-rw-r--r--   0        0        0     2447 2023-05-18 07:38:18.935267 micropy_cli-4.2.1/tests/test_stubs_repo.py
+-rw-r--r--   0        0        0     4534 2023-05-18 07:38:18.935267 micropy_cli-4.2.1/tests/test_template.py
+-rw-r--r--   0        0        0      157 2023-05-18 07:38:18.939267 micropy_cli-4.2.1/tests/test_utils/fail.json
+-rw-r--r--   0        0        0      395 2023-05-18 07:38:18.939267 micropy_cli-4.2.1/tests/test_utils/pass.json
+-rw-r--r--   0        0        0     1088 2023-05-18 07:38:18.939267 micropy_cli-4.2.1/tests/test_utils/schema.json
+-rw-r--r--   0        0        0    10261 2023-05-18 07:38:18.935267 micropy_cli-4.2.1/tests/test_utils.py
+-rw-r--r--   0        0        0    11792 1970-01-01 00:00:00.000000 micropy_cli-4.2.1/PKG-INFO
```

### Comparing `micropy_cli-4.2.0b3/CHANGELOG.md` & `micropy_cli-4.2.1/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,42 @@
 <a name="v4.0.0"></a>
 
+## [4.2.1](https://github.com/BradenM/micropy-cli/compare/v4.2.0...v4.2.1) (2023-05-18)
+
+
+### Bug Fixes
+
+* **deps:** Update dependency attrs to v23 ([3422a84](https://github.com/BradenM/micropy-cli/commit/3422a84f576e2db7e39331512e71e3d72ed85d55))
+* **deps:** Update dependency python-minifier to v2.9.0 ([2a7464c](https://github.com/BradenM/micropy-cli/commit/2a7464cf9be34dc4766083fab6570fe0c507e5d7))
+* **deps:** Update dependency requests to v2.29.0 ([8361e7c](https://github.com/BradenM/micropy-cli/commit/8361e7cc15b0bdcefa07048814f30c0d4bb531b3))
+* **deps:** Update dependency requests to v2.30.0 ([9e389b1](https://github.com/BradenM/micropy-cli/commit/9e389b11c171d16af26b28217993e38bbbf4fa4f))
+* **deps:** Update dependency typer to v0.8.0 ([d2bf4e6](https://github.com/BradenM/micropy-cli/commit/d2bf4e69e83da62b589658ed3210742152547db6))
+* **deps:** Update dependency typer to v0.9.0 ([f8f4105](https://github.com/BradenM/micropy-cli/commit/f8f4105e65370eb275114f1e30ce5c3361e61dd5))
+* **stubs:** Always ensure correct pyi stub root paths. ([27f87a1](https://github.com/BradenM/micropy-cli/commit/27f87a1d697e2ee5e18d178eb46c7532b3c2fe29))
+* **stubs:** Do not drop firmware name when parsing from dist metadata. ([be269ee](https://github.com/BradenM/micropy-cli/commit/be269ee5e241d9274d100c5dc1c9f28278b0d1d6))
+* **template:** Resolve pylance type-checking / import errors. ([179c29d](https://github.com/BradenM/micropy-cli/commit/179c29d68bf025c1b3436d53dd3f9168d93285cf))
+* **template:** Update pylint config to use `MAIN` and `INFERENCE` confidence level. ([f5f5c98](https://github.com/BradenM/micropy-cli/commit/f5f5c983cbeeb6730c85750ac78115d86135d44b))
+
+## [4.2.0](https://github.com/BradenM/micropy-cli/compare/v4.2.0-beta.3...v4.2.0) (2023-04-22)
+
+
+### Features
+
+* **app:** Add exclude_defaults, improve help in stubs create command. ([efa3263](https://github.com/BradenM/micropy-cli/commit/efa3263121704e56d6e4dc0aa4975228b4731184))
+
+
+### Documentation
+
+* **app:** Improve stubs create help. ([9738ac7](https://github.com/BradenM/micropy-cli/commit/9738ac71256e8375ee190f3114ef5cb7e46c3506))
+
+
+### Miscellaneous Chores
+
+* **release:** Release as 4.2.0 ([817c583](https://github.com/BradenM/micropy-cli/commit/817c583bc460e642ddad0b383d88483945ee234b))
+
 ## [4.2.0-beta.3](https://github.com/BradenM/micropy-cli/compare/v4.2.0-beta.2...v4.2.0-beta.3) (2023-04-17)
 
 
 ### Features
 
 * **app:** Expose compile, module-defaults flags, integrity in stubs create command. ([885e9d3](https://github.com/BradenM/micropy-cli/commit/885e9d369cad98345e6132315f6fb76694379339))
 * **exc:** `PyDeviceFileIntegrityError` exception. ([a2187c8](https://github.com/BradenM/micropy-cli/commit/a2187c898c9aeb641a63a9237d2469faaf929de5))
```

### Comparing `micropy_cli-4.2.0b3/LICENSE` & `micropy_cli-4.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `micropy_cli-4.2.0b3/README.md` & `micropy_cli-4.2.1/README.md`

 * *Files identical despite different names*

### Comparing `micropy_cli-4.2.0b3/micropy/app/main.py` & `micropy_cli-4.2.1/micropy/app/main.py`

 * *Files identical despite different names*

### Comparing `micropy_cli-4.2.0b3/micropy/app/stubs.py` & `micropy_cli-4.2.1/micropy/app/stubs.py`

 * *Files 6% similar despite different names*

```diff
@@ -70,44 +70,77 @@
     return ListChangeSet.from_strings(add=value, replace=replace)
 
 
 @stubs_app.command(name="create")
 def stubs_create(
     ctx: typer.Context,
     port: str = typer.Argument(..., help="Serial port used to connect to device"),
-    backend: CreateBackend = typer.Option(CreateBackend.upydevice, help="PyDevice backend."),
+    backend: CreateBackend = typer.Option(CreateBackend.upydevice, help="PyDevice backend to use."),
     variant: stub_board.CreateStubsVariant = typer.Option(
         stub_board.CreateStubsVariant.BASE,
         "-v",
         "--variant",
         help="Create Stubs variant.",
         rich_help_panel="Stubs",
     ),
     module: Optional[List[str]] = typer.Option(
-        None, "-m", "--module", help="Modules to add.", rich_help_panel="Stubs"
+        None,
+        "-m",
+        "--module",
+        help="Modules to look for and stub. This flag can be used multiple times.",
+        rich_help_panel="Stubs",
     ),
     module_defaults: bool = typer.Option(
-        True, help="Include createstubs default modules.", rich_help_panel="Stubs"
+        True, help="Include createstubs.py default modules.", rich_help_panel="Stubs"
     ),
     exclude: Optional[List[str]] = typer.Option(
-        None, "-e", "--exclude", help="Modules to exclude.", rich_help_panel="Stubs"
+        None,
+        "-e",
+        "--exclude",
+        help="Modules to exclude from stubber. This flag can be used multiple times.",
+        rich_help_panel="Stubs",
+    ),
+    exclude_defaults: bool = typer.Option(
+        True,
+        help="Include createstubs.py default module excludes. This flag can be used multiple times.",
+        rich_help_panel="Stubs",
     ),
     compile: bool = typer.Option(
         True,
         "-c",
         "--compile",
         help="Cross compile to .mpy via mpy-cross.",
         rich_help_panel="Stubs",
     ),
 ):
     """Create stubs from micropython-enabled devices.
 
     Utilize Josverl's [micropython-stubber](https://github.com/josverl/micropython-stubber/)
     to generate stubs from your own micropython-enabled device.
 
+    \n
+    **Create stubs with defaults**:\n
+     - `micropy stubs create /dev/ttyUSB0`
+
+    \n
+    **Specify additional modules**:\n
+     - `micropy stubs create -m custom_module -m other_module /dev/ttyUSB0`\n
+     - _Only given modules_: `micropy stubs create -m custom_module --no-module-defaults /dev/ttyUSB0`
+
+    \n
+    **Exclude additional modules**:\n
+     - `micropy stubs create -e custom_module -e other_module /dev/ttyUSB0`\n
+     - _Only exclude given modules_: `micropy stubs create -e custom_module --no-module-defaults /dev/ttyUSB0`
+
+    \n
+    **Create Stubs Variants**:\n
+     - **mem**: Optimized for low memory devices._\n
+     - **db**: Persist stub progress across reboots.\n
+     - **lvgl**: Additional support for LVGL devices.\n
+
     """
     mp: MicroPy = ctx.ensure_object(MicroPy)
     log = mp.log
     log.title(f"Connecting to Pyboard @ $[{port}]")
     pyb_log = Log.add_logger("Pyboard", "bright_white")
 
     def _get_desc(name: str, cfg: dict):
@@ -133,15 +166,15 @@
     if module or exclude:
         log.title("Preparing createstubs for:")
         log.info(f"Modules: {', '.join(module or [])}")
         log.info(f"Exclude: {', '.join(exclude or [])}")
     create_stubs = prepare_create_stubs(
         variant=variant,
         modules_set=create_changeset(module, replace=not module_defaults),
-        exclude_set=create_changeset(exclude),
+        exclude_set=create_changeset(exclude, replace=not exclude_defaults),
         compile=compile,
     )
     dev_path = DevicePath("createstubs.mpy") if compile else DevicePath("createstubs.py")
     log.info("Executing stubber on pyboard...")
     try:
         pyb.run_script(create_stubs, DevicePath(dev_path))
     except Exception as e:
```

### Comparing `micropy_cli-4.2.0b3/micropy/config/config.py` & `micropy_cli-4.2.1/micropy/config/config.py`

 * *Files identical despite different names*

### Comparing `micropy_cli-4.2.0b3/micropy/config/config_dict.py` & `micropy_cli-4.2.1/micropy/config/config_dict.py`

 * *Files identical despite different names*

### Comparing `micropy_cli-4.2.0b3/micropy/config/config_json.py` & `micropy_cli-4.2.1/micropy/config/config_json.py`

 * *Files identical despite different names*

### Comparing `micropy_cli-4.2.0b3/micropy/config/config_source.py` & `micropy_cli-4.2.1/micropy/config/config_source.py`

 * *Files identical despite different names*

### Comparing `micropy_cli-4.2.0b3/micropy/data/__init__.py` & `micropy_cli-4.2.1/micropy/data/__init__.py`

 * *Files identical despite different names*

### Comparing `micropy_cli-4.2.0b3/micropy/data/schemas/firmware.json` & `micropy_cli-4.2.1/micropy/data/schemas/firmware.json`

 * *Files identical despite different names*

### Comparing `micropy_cli-4.2.0b3/micropy/data/schemas/stubs.json` & `micropy_cli-4.2.1/micropy/data/schemas/stubs.json`

 * *Files identical despite different names*

### Comparing `micropy_cli-4.2.0b3/micropy/exceptions.py` & `micropy_cli-4.2.1/micropy/exceptions.py`

 * *Files identical despite different names*

### Comparing `micropy_cli-4.2.0b3/micropy/logger.py` & `micropy_cli-4.2.1/micropy/logger.py`

 * *Files identical despite different names*

### Comparing `micropy_cli-4.2.0b3/micropy/main.py` & `micropy_cli-4.2.1/micropy/main.py`

 * *Files identical despite different names*

### Comparing `micropy_cli-4.2.0b3/micropy/packages/__init__.py` & `micropy_cli-4.2.1/micropy/packages/__init__.py`

 * *Files identical despite different names*

### Comparing `micropy_cli-4.2.0b3/micropy/packages/package.py` & `micropy_cli-4.2.1/micropy/packages/package.py`

 * *Files identical despite different names*

### Comparing `micropy_cli-4.2.0b3/micropy/packages/source.py` & `micropy_cli-4.2.1/micropy/packages/source.py`

 * *Files identical despite different names*

### Comparing `micropy_cli-4.2.0b3/micropy/packages/source_package.py` & `micropy_cli-4.2.1/micropy/packages/source_package.py`

 * *Files identical despite different names*

### Comparing `micropy_cli-4.2.0b3/micropy/packages/source_path.py` & `micropy_cli-4.2.1/micropy/packages/source_path.py`

 * *Files identical despite different names*

### Comparing `micropy_cli-4.2.0b3/micropy/project/checks.py` & `micropy_cli-4.2.1/micropy/project/checks.py`

 * *Files identical despite different names*

### Comparing `micropy_cli-4.2.0b3/micropy/project/modules/modules.py` & `micropy_cli-4.2.1/micropy/project/modules/modules.py`

 * *Files identical despite different names*

### Comparing `micropy_cli-4.2.0b3/micropy/project/modules/packages.py` & `micropy_cli-4.2.1/micropy/project/modules/packages.py`

 * *Files identical despite different names*

### Comparing `micropy_cli-4.2.0b3/micropy/project/modules/stubs.py` & `micropy_cli-4.2.1/micropy/project/modules/stubs.py`

 * *Files identical despite different names*

### Comparing `micropy_cli-4.2.0b3/micropy/project/modules/templates.py` & `micropy_cli-4.2.1/micropy/project/modules/templates.py`

 * *Files identical despite different names*

### Comparing `micropy_cli-4.2.0b3/micropy/project/project.py` & `micropy_cli-4.2.1/micropy/project/project.py`

 * *Files identical despite different names*

### Comparing `micropy_cli-4.2.0b3/micropy/project/template/.gitignore` & `micropy_cli-4.2.1/micropy/project/template/.gitignore`

 * *Files identical despite different names*

### Comparing `micropy_cli-4.2.0b3/micropy/project/template/.pylintrc` & `micropy_cli-4.2.1/micropy/project/template/.pylintrc`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-[MASTER]
+[MAIN]
 # Loaded Stubs: {% for stub in stubs %} {{ stub }} {% endfor %}
 init-hook='import sys;sys.path[1:1]=["src/lib",{% for path in paths %}"{{ path|replace("\\", "/") }}", {% endfor %} ]'
 
 [MESSAGES CONTROL]
 # Only show warnings with the listed confidence levels. Leave empty to show
 # all. Valid levels: HIGH, INFERENCE, INFERENCE_FAILURE, UNDEFINED.
-confidence=
+confidence=INFERENCE
 
 # Disable the message, report, category or checker with the given id(s). You
 # can either give multiple identifiers separated by comma (,) or put this
 # option multiple times (only on the command line, not in the configuration
 # file where it should appear only once). You can also use "--disable=all" to
 # disable everything first and then reenable specific checks. For example, if
 # you want to run only the similarities checker, you can use "--disable=all
```

### Comparing `micropy_cli-4.2.0b3/micropy/project/template.py` & `micropy_cli-4.2.1/micropy/project/template.py`

 * *Files 0% similar despite different names*

```diff
@@ -188,14 +188,15 @@
             paths = list(self.iter_relative_paths(self.paths, strict=True))
         if self.local_paths:
             paths.extend(self.iter_relative_paths(self.local_paths))
         stub_paths = json.dumps([str(s) for s in paths])
         ctx = {
             "stubs": self.stubs or [],
             "paths": stub_paths,
+            "typeshed_paths": json.dumps([str(s) for s in [*paths, "typings"]]),
             "language_server": self.language_server,
         }
         return ctx
 
 
 class PylintTemplate(Template):
     """Template for Pylint settings."""
```

### Comparing `micropy_cli-4.2.0b3/micropy/pyd/__init__.py` & `micropy_cli-4.2.1/micropy/pyd/__init__.py`

 * *Files identical despite different names*

### Comparing `micropy_cli-4.2.0b3/micropy/pyd/abc.py` & `micropy_cli-4.2.1/micropy/pyd/abc.py`

 * *Files identical despite different names*

### Comparing `micropy_cli-4.2.0b3/micropy/pyd/backend_rshell.py` & `micropy_cli-4.2.1/micropy/pyd/backend_rshell.py`

 * *Files identical despite different names*

### Comparing `micropy_cli-4.2.0b3/micropy/pyd/backend_upydevice.py` & `micropy_cli-4.2.1/micropy/pyd/backend_upydevice.py`

 * *Files identical despite different names*

### Comparing `micropy_cli-4.2.0b3/micropy/pyd/consumers.py` & `micropy_cli-4.2.1/micropy/pyd/consumers.py`

 * *Files identical despite different names*

### Comparing `micropy_cli-4.2.0b3/micropy/pyd/pydevice.py` & `micropy_cli-4.2.1/micropy/pyd/pydevice.py`

 * *Files identical despite different names*

### Comparing `micropy_cli-4.2.0b3/micropy/stubs/__init__.py` & `micropy_cli-4.2.1/micropy/stubs/__init__.py`

 * *Files identical despite different names*

### Comparing `micropy_cli-4.2.0b3/micropy/stubs/manifest.py` & `micropy_cli-4.2.1/micropy/stubs/manifest.py`

 * *Files identical despite different names*

### Comparing `micropy_cli-4.2.0b3/micropy/stubs/repo.py` & `micropy_cli-4.2.1/micropy/stubs/repo.py`

 * *Files identical despite different names*

### Comparing `micropy_cli-4.2.0b3/micropy/stubs/repo_package.py` & `micropy_cli-4.2.1/micropy/stubs/repo_package.py`

 * *Files identical despite different names*

### Comparing `micropy_cli-4.2.0b3/micropy/stubs/repositories/micropy.py` & `micropy_cli-4.2.1/micropy/stubs/repositories/micropy.py`

 * *Files identical despite different names*

### Comparing `micropy_cli-4.2.0b3/micropy/stubs/repositories/micropython.py` & `micropy_cli-4.2.1/micropy/stubs/repositories/micropython.py`

 * *Files identical despite different names*

### Comparing `micropy_cli-4.2.0b3/micropy/stubs/source.py` & `micropy_cli-4.2.1/micropy/stubs/source.py`

 * *Files identical despite different names*

### Comparing `micropy_cli-4.2.0b3/micropy/stubs/stubs.py` & `micropy_cli-4.2.1/micropy/stubs/stubs.py`

 * *Files 2% similar despite different names*

```diff
@@ -382,21 +382,21 @@
         meta = next(m for m in metadatas if m.todict()["name"] == package_name)
         info_path = path / "info.json"
         name_parts = set(meta.todict()["name"].split("-"))
         name_parts.remove("stubs")
         # oh lawd, look away!!
         dev_name = min(name_parts, key=lambda s: len(s))
         name_parts.remove(dev_name)
-        name_parts.pop()
+        firm_name = name_parts.pop()
         firm = {
             "ver": meta.version or "",
             "port": dev_name,
             "arch": "",
             "sysname": dev_name,
-            "name": "",
+            "name": firm_name,
             "mpy": 0,
             "version": meta.version or "",
             "machine": "",
             "build": "",
             "nodename": dev_name,
             "platform": dev_name,
             "family": "",
@@ -458,14 +458,21 @@
     def __init__(self, path, copy_to=None, **kwargs):
         self.path = Path(path)
         ref = self.path / "info.json"
         self.info = json.load(ref.open())
         if copy_to is not None:
             self.copy_to(copy_to)
 
+    def find_root(self, path: Path) -> Path:
+        """Attempt to find appropriate stub root."""
+        pyi_files = path.rglob("*.pyi")
+        if pyi_path := next(pyi_files, None):
+            return pyi_path.parent
+        return path
+
     def copy_to(self, dest, name=None):
         """Copy stub to a directory."""
         if not name:
             dest = Path(dest) / self.path.name
         shutil.copytree(self.path, dest)
         self.path = dest.resolve()
         return self
@@ -515,17 +522,19 @@
 
     """
 
     def __init__(self, path, copy_to=None, **kwargs):
         super().__init__(path, copy_to, **kwargs)
 
         stubs_path = self.path / "stubs"
-        self.stubs = stubs_path if stubs_path.exists() else self.path
+        self.stubs = self.find_root(stubs_path if stubs_path.exists() else self.path)
+
         frozen_path = self.path / "frozen"
-        self.frozen = frozen_path if frozen_path.exists() else self.path
+        self.frozen = self.find_root(frozen_path if frozen_path.exists() else self.path)
+
         stubber = self.info.get("stubber")
         self.stub_version = stubber.get("version")
 
         self.firm_info = self.info.get("firmware")
         self.firmware = kwargs.get("firmware", None)
         self.sysname = self.firm_info.get("sysname")
         self.version = self.firm_info.get("version")
```

### Comparing `micropy_cli-4.2.0b3/micropy/utils/__init__.py` & `micropy_cli-4.2.1/micropy/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `micropy_cli-4.2.0b3/micropy/utils/helpers.py` & `micropy_cli-4.2.1/micropy/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `micropy_cli-4.2.0b3/micropy/utils/stub.py` & `micropy_cli-4.2.1/micropy/utils/stub.py`

 * *Files identical despite different names*

### Comparing `micropy_cli-4.2.0b3/micropy/utils/validate.py` & `micropy_cli-4.2.1/micropy/utils/validate.py`

 * *Files identical despite different names*

### Comparing `micropy_cli-4.2.0b3/pyproject.toml` & `micropy_cli-4.2.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "micropy-cli"
-version = "4.2.0-beta.3"
+version = "4.2.1"
 description = "Micropython Project Management Tool with VSCode support, Linting, Intellisense, Dependency Management, and more!"
 authors = ["Braden Mars <bradenmars@bradenmars.me>"]
 license = "MIT"
 packages = [{ include = "micropy" }]
 include = [
     { path = "tests", format = "sdist" },
     "README.md",
@@ -38,40 +38,40 @@
 
 [tool.poetry.dependencies]
 python = ">=3.8,<3.12"
 boltons = "==23.0.0"
 cachier = "2.0.0"
 Jinja2 = "3.1.2"
 questionary = "1.10.0"
-requests = "2.28.2"
+requests = "2.30.0"
 requirements-parser = "0.2.0"
 tqdm = "4.65.0"
 click = "8.1.3"
 colorama = { version = "==0.4.6", platform = "win32" }
 jsonschema = "=3.2.0"
 dpath = "==1.5.0"
 GitPython = "==3.1.31"
 packaging = "==21.3"
-python-minifier = "==2.8.1"
-mypy = "==1.0.1"
+python-minifier = "==2.9.0"
+mypy = "==1.2.0"
 ## rshell is broken on windows (with python >=3.10) due to pyreadline dependency.
 rshell = [
     { version = "^0.0.31", platform = "win32", python = "<3.10" },
     { version = "^0.0.31", platform = "!=win32" },
 ]
 MarkupSafe = "==2.1.2"
 upydevice = "0.3.8"
-attrs = "==22.2.0"
+attrs = "==23.1.0"
 typing-extensions = "4.5.0"
 pydantic = "1.10.7"
 distlib = "0.3.6"
 importlib-metadata = { version = "==5.2.0", python = '<3.10' }
-micropython-stubber = "==1.13.1.post1"
+micropython-stubber = "==1.13.7"
 libcst = "0.4.9"
-typer = {version = "0.7.0", extras = ["all"]}
+typer = {version = "0.9.0", extras = ["all"]}
 
 [tool.poetry.group.dev.dependencies]
 bump2version = "^0.5.11"
 pre-commit = "^3.0.2"
 mypy = { version = "^1.0", extras = ["dmypy"] }
 types-requests = "^2.27.14"
 pylint = "^2.7"
@@ -81,15 +81,15 @@
 [tool.poetry.group.lint]
 optional = true
 
 [tool.poetry.group.lint.dependencies]
 pyupgrade = "^3.3.1"
 isort = "^5.12.0"
 black = ">=22.10,<23.0"
-ruff = "^0.0.261"
+ruff = "^0.0.267"
 
 [tool.poetry.group.test]
 optional = true
 
 [tool.poetry.group.test.dependencies]
 pytest = "^7.1.1"
 pytest-cov = "^4.0"
```

### Comparing `micropy_cli-4.2.0b3/tests/app/conftest.py` & `micropy_cli-4.2.1/tests/app/conftest.py`

 * *Files identical despite different names*

### Comparing `micropy_cli-4.2.0b3/tests/app/test_main.py` & `micropy_cli-4.2.1/tests/app/test_main.py`

 * *Files identical despite different names*

### Comparing `micropy_cli-4.2.0b3/tests/app/test_stubs.py` & `micropy_cli-4.2.1/tests/app/test_stubs.py`

 * *Files identical despite different names*

### Comparing `micropy_cli-4.2.0b3/tests/conftest.py` & `micropy_cli-4.2.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `micropy_cli-4.2.0b3/tests/data/archive_test_stub.tar.gz` & `micropy_cli-4.2.1/tests/data/archive_test_stub.tar.gz`

 * *Files identical despite different names*

### Comparing `micropy_cli-4.2.0b3/tests/data/esp32_test_stub/frozen/ntptime.py` & `micropy_cli-4.2.1/tests/data/esp32_test_stub/frozen/ntptime.py`

 * *Files identical despite different names*

### Comparing `micropy_cli-4.2.0b3/tests/data/esp32_test_stub/info.json` & `micropy_cli-4.2.1/tests/data/esp32_test_stub/info.json`

 * *Files identical despite different names*

### Comparing `micropy_cli-4.2.0b3/tests/data/esp32_test_stub/stubs/modules.json` & `micropy_cli-4.2.1/tests/data/esp32_test_stub/stubs/modules.json`

 * *Files identical despite different names*

### Comparing `micropy_cli-4.2.0b3/tests/data/esp8266_test_stub/frozen/ntptime.py` & `micropy_cli-4.2.1/tests/data/esp8266_test_stub/frozen/ntptime.py`

 * *Files identical despite different names*

### Comparing `micropy_cli-4.2.0b3/tests/data/esp8266_test_stub/info.json` & `micropy_cli-4.2.1/tests/data/esp8266_test_stub/info.json`

 * *Files identical despite different names*

### Comparing `micropy_cli-4.2.0b3/tests/data/esp8266_test_stub/stubs/modules.json` & `micropy_cli-4.2.1/tests/data/esp8266_test_stub/stubs/modules.json`

 * *Files identical despite different names*

### Comparing `micropy_cli-4.2.0b3/tests/data/fware_test_stub/frozen/utarfile.py` & `micropy_cli-4.2.1/tests/data/fware_test_stub/frozen/utarfile.py`

 * *Files identical despite different names*

### Comparing `micropy_cli-4.2.0b3/tests/data/fware_test_stub/frozen/utarfile.pyi` & `micropy_cli-4.2.1/tests/data/fware_test_stub/frozen/utarfile.pyi`

 * *Files identical despite different names*

### Comparing `micropy_cli-4.2.0b3/tests/data/fware_test_stub/frozen/utokenize.py` & `micropy_cli-4.2.1/tests/data/fware_test_stub/frozen/utokenize.py`

 * *Files identical despite different names*

### Comparing `micropy_cli-4.2.0b3/tests/data/fware_test_stub/info.json` & `micropy_cli-4.2.1/tests/data/fware_test_stub/info.json`

 * *Files identical despite different names*

### Comparing `micropy_cli-4.2.0b3/tests/data/project_test/.vscode/settings.json` & `micropy_cli-4.2.1/tests/data/project_test/.vscode/settings.json`

 * *Files identical despite different names*

### Comparing `micropy_cli-4.2.0b3/tests/data/test_repo.json` & `micropy_cli-4.2.1/tests/data/test_repo.json`

 * *Files identical despite different names*

### Comparing `micropy_cli-4.2.0b3/tests/data/test_source.xml` & `micropy_cli-4.2.1/tests/data/test_source.xml`

 * *Files identical despite different names*

### Comparing `micropy_cli-4.2.0b3/tests/test_config.py` & `micropy_cli-4.2.1/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `micropy_cli-4.2.0b3/tests/test_highlevel.py` & `micropy_cli-4.2.1/tests/test_highlevel.py`

 * *Files identical despite different names*

### Comparing `micropy_cli-4.2.0b3/tests/test_main.py` & `micropy_cli-4.2.1/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `micropy_cli-4.2.0b3/tests/test_packages.py` & `micropy_cli-4.2.1/tests/test_packages.py`

 * *Files identical despite different names*

### Comparing `micropy_cli-4.2.0b3/tests/test_project.py` & `micropy_cli-4.2.1/tests/test_project.py`

 * *Files identical despite different names*

### Comparing `micropy_cli-4.2.0b3/tests/test_pyd.py` & `micropy_cli-4.2.1/tests/test_pyd.py`

 * *Files identical despite different names*

### Comparing `micropy_cli-4.2.0b3/tests/test_stub_source.py` & `micropy_cli-4.2.1/tests/test_stub_source.py`

 * *Files identical despite different names*

### Comparing `micropy_cli-4.2.0b3/tests/test_stubs/esp32_test_stub/frozen/ntptime.py` & `micropy_cli-4.2.1/tests/test_stubs/esp32_test_stub/frozen/ntptime.py`

 * *Files identical despite different names*

### Comparing `micropy_cli-4.2.0b3/tests/test_stubs/esp32_test_stub/info.json` & `micropy_cli-4.2.1/tests/test_stubs/esp32_test_stub/info.json`

 * *Files identical despite different names*

### Comparing `micropy_cli-4.2.0b3/tests/test_stubs/esp32_test_stub/stubs/modules.json` & `micropy_cli-4.2.1/tests/test_stubs/esp32_test_stub/stubs/modules.json`

 * *Files identical despite different names*

### Comparing `micropy_cli-4.2.0b3/tests/test_stubs/esp8266_test_stub/frozen/ntptime.py` & `micropy_cli-4.2.1/tests/test_stubs/esp8266_test_stub/frozen/ntptime.py`

 * *Files identical despite different names*

### Comparing `micropy_cli-4.2.0b3/tests/test_stubs/esp8266_test_stub/info.json` & `micropy_cli-4.2.1/tests/test_stubs/esp8266_test_stub/info.json`

 * *Files identical despite different names*

### Comparing `micropy_cli-4.2.0b3/tests/test_stubs/esp8266_test_stub/stubs/modules.json` & `micropy_cli-4.2.1/tests/test_stubs/esp8266_test_stub/stubs/modules.json`

 * *Files identical despite different names*

### Comparing `micropy_cli-4.2.0b3/tests/test_stubs.py` & `micropy_cli-4.2.1/tests/test_stubs.py`

 * *Files identical despite different names*

### Comparing `micropy_cli-4.2.0b3/tests/test_stubs_repo.py` & `micropy_cli-4.2.1/tests/test_stubs_repo.py`

 * *Files identical despite different names*

### Comparing `micropy_cli-4.2.0b3/tests/test_template.py` & `micropy_cli-4.2.1/tests/test_template.py`

 * *Files identical despite different names*

### Comparing `micropy_cli-4.2.0b3/tests/test_utils/schema.json` & `micropy_cli-4.2.1/tests/test_utils/schema.json`

 * *Files identical despite different names*

### Comparing `micropy_cli-4.2.0b3/tests/test_utils.py` & `micropy_cli-4.2.1/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `micropy_cli-4.2.0b3/PKG-INFO` & `micropy_cli-4.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: micropy-cli
-Version: 4.2.0b3
+Version: 4.2.1
 Summary: Micropython Project Management Tool with VSCode support, Linting, Intellisense, Dependency Management, and more!
 Home-page: https://github.com/BradenM/micropy-cli
 License: MIT
 Keywords: micropython,stubs,linting,vscode,intellisense
 Author: Braden Mars
 Author-email: bradenmars@bradenmars.me
 Requires-Python: >=3.8,<3.12
@@ -21,36 +21,36 @@
 Classifier: Programming Language :: Python :: Implementation :: MicroPython
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: Topic :: Software Development :: Code Generators
 Classifier: Topic :: Software Development :: Embedded Systems
 Requires-Dist: GitPython (==3.1.31)
 Requires-Dist: Jinja2 (==3.1.2)
 Requires-Dist: MarkupSafe (==2.1.2)
-Requires-Dist: attrs (==22.2.0)
+Requires-Dist: attrs (==23.1.0)
 Requires-Dist: boltons (==23.0.0)
 Requires-Dist: cachier (==2.0.0)
 Requires-Dist: click (==8.1.3)
 Requires-Dist: colorama (==0.4.6) ; sys_platform == "win32"
 Requires-Dist: distlib (==0.3.6)
 Requires-Dist: dpath (==1.5.0)
 Requires-Dist: importlib-metadata (==5.2.0) ; python_version < "3.10"
 Requires-Dist: jsonschema (==3.2.0)
 Requires-Dist: libcst (==0.4.9)
-Requires-Dist: micropython-stubber (==1.13.1.post1)
-Requires-Dist: mypy (==1.0.1)
+Requires-Dist: micropython-stubber (==1.13.7)
+Requires-Dist: mypy (==1.2.0)
 Requires-Dist: packaging (==21.3)
 Requires-Dist: pydantic (==1.10.7)
-Requires-Dist: python-minifier (==2.8.1)
+Requires-Dist: python-minifier (==2.9.0)
 Requires-Dist: questionary (==1.10.0)
-Requires-Dist: requests (==2.28.2)
+Requires-Dist: requests (==2.30.0)
 Requires-Dist: requirements-parser (==0.2.0)
 Requires-Dist: rshell (>=0.0.31,<0.0.32) ; python_version < "3.10" and sys_platform == "win32"
 Requires-Dist: rshell (>=0.0.31,<0.0.32) ; sys_platform != "win32"
 Requires-Dist: tqdm (==4.65.0)
-Requires-Dist: typer[all] (==0.7.0)
+Requires-Dist: typer[all] (==0.9.0)
 Requires-Dist: typing-extensions (==4.5.0)
 Requires-Dist: upydevice (==0.3.8)
 Project-URL: Documentation, https://micropy-cli.readthedocs.io
 Project-URL: Repository, https://github.com/BradenM/micropy-cli
 Description-Content-Type: text/markdown
 
 # Micropy Cli [![PyPI][pypi-img]][pypi-url] [![PyPI - Python Version][pypiv-img]][pypi-url] [![Github - Test Micropy Cli][build-img]][build-url] [![Coverage Status][cover-img]][cover-url]
```

