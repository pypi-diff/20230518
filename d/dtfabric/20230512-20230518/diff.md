# Comparing `tmp/dtfabric-20230512.tar.gz` & `tmp/dtfabric-20230518.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dtfabric-20230512.tar", last modified: Fri May 12 04:07:16 2023, max compression
+gzip compressed data, was "dtfabric-20230518.tar", last modified: Thu May 18 16:25:30 2023, max compression
```

## Comparing `dtfabric-20230512.tar` & `dtfabric-20230518.tar`

### file list

```diff
@@ -1,132 +1,133 @@
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-12 04:07:16.685438 dtfabric-20230512/
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-12 04:07:16.332437 dtfabric-20230512/.github/
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-12 04:07:16.384437 dtfabric-20230512/.github/workflows/
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     2541 2023-05-08 04:44:50.000000 dtfabric-20230512/.github/workflows/test_docker.yml
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1378 2023-05-08 04:44:50.000000 dtfabric-20230512/.github/workflows/test_docs.yml
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     4107 2023-05-08 04:44:50.000000 dtfabric-20230512/.github/workflows/test_tox.yml
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    21911 2023-05-08 04:44:50.000000 dtfabric-20230512/.pylintrc
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      149 2022-07-10 04:44:41.000000 dtfabric-20230512/.yamllint.yaml
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       92 2022-01-24 07:36:34.000000 dtfabric-20230512/ACKNOWLEDGEMENTS
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      265 2018-07-03 18:38:13.000000 dtfabric-20230512/AUTHORS
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    11358 2016-09-25 06:41:25.000000 dtfabric-20230512/LICENSE
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      592 2021-08-22 05:30:09.000000 dtfabric-20230512/MANIFEST.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      583 2023-05-12 04:07:16.685438 dtfabric-20230512/PKG-INFO
--rw-r-----   0 lordyesta  (1000) lordyesta  (1000)      195 2020-06-21 05:38:03.000000 dtfabric-20230512/README
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1230 2023-05-08 04:44:50.000000 dtfabric-20230512/appveyor.yml
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-12 04:07:16.332437 dtfabric-20230512/config/
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-12 04:07:16.384437 dtfabric-20230512/config/appveyor/
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      839 2023-05-08 04:44:50.000000 dtfabric-20230512/config/appveyor/install.ps1
--rwxrwxr-x   0 lordyesta  (1000) lordyesta  (1000)      125 2023-05-08 04:44:50.000000 dtfabric-20230512/config/appveyor/install.sh
--rwxrwxr-x   0 lordyesta  (1000) lordyesta  (1000)      620 2023-05-08 04:44:50.000000 dtfabric-20230512/config/appveyor/runtests.sh
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-12 04:07:16.437437 dtfabric-20230512/config/dpkg/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      140 2023-05-12 03:57:04.000000 dtfabric-20230512/config/dpkg/changelog
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       38 2017-05-26 07:25:10.000000 dtfabric-20230512/config/dpkg/clean
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)        2 2023-05-08 04:44:51.000000 dtfabric-20230512/config/dpkg/compat
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      786 2023-05-08 04:44:51.000000 dtfabric-20230512/config/dpkg/control
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      884 2017-04-14 13:14:48.000000 dtfabric-20230512/config/dpkg/copyright
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       20 2017-04-14 13:31:35.000000 dtfabric-20230512/config/dpkg/dtfabric-data.dirs
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       26 2017-04-14 13:32:40.000000 dtfabric-20230512/config/dpkg/dtfabric-data.install
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      144 2017-05-26 07:25:20.000000 dtfabric-20230512/config/dpkg/python-dtfabric.install
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      144 2017-05-26 07:25:27.000000 dtfabric-20230512/config/dpkg/python3-dtfabric.install
--rwxrwxr-x   0 lordyesta  (1000) lordyesta  (1000)      122 2023-05-08 04:44:51.000000 dtfabric-20230512/config/dpkg/rules
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-12 04:07:16.437437 dtfabric-20230512/config/dpkg/source/
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       12 2017-04-14 13:14:48.000000 dtfabric-20230512/config/dpkg/source/format
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-12 04:07:16.438437 dtfabric-20230512/config/pylint/
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      362 2020-06-21 09:14:13.000000 dtfabric-20230512/config/pylint/spelling-private-dict
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      151 2020-01-19 18:45:05.000000 dtfabric-20230512/dependencies.ini
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-12 04:07:16.454437 dtfabric-20230512/docs/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5061 2023-05-08 04:44:51.000000 dtfabric-20230512/docs/conf.py
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      566 2021-07-30 06:46:25.000000 dtfabric-20230512/docs/index.rst
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      105 2023-05-08 04:45:00.000000 dtfabric-20230512/docs/requirements.txt
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-12 04:07:16.454437 dtfabric-20230512/docs/sources/
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    15554 2022-07-10 05:53:49.000000 dtfabric-20230512/docs/sources/Format-specification.md
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-12 04:07:16.455437 dtfabric-20230512/docs/sources/api/
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1097 2022-02-19 13:55:33.000000 dtfabric-20230512/docs/sources/api/dtfabric.rst
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      869 2021-07-30 06:46:25.000000 dtfabric-20230512/docs/sources/api/dtfabric.runtime.rst
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       61 2021-07-30 06:37:51.000000 dtfabric-20230512/docs/sources/api/modules.rst
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-12 04:07:16.455437 dtfabric-20230512/docs/sources/user/
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1633 2021-12-28 03:59:54.000000 dtfabric-20230512/docs/sources/user/Installation-instructions.md
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      288 2021-07-30 06:37:51.000000 dtfabric-20230512/docs/sources/user/index.rst
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-12 04:07:16.457437 dtfabric-20230512/dtfabric/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       74 2023-05-12 03:57:04.000000 dtfabric-20230512/dtfabric/__init__.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    31346 2022-09-25 13:56:37.000000 dtfabric-20230512/dtfabric/data_types.py
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      710 2022-09-18 09:38:10.000000 dtfabric-20230512/dtfabric/decorators.py
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1502 2021-07-30 10:44:15.000000 dtfabric-20230512/dtfabric/definitions.py
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1016 2021-07-30 06:46:25.000000 dtfabric-20230512/dtfabric/errors.py
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    53227 2023-05-12 03:56:53.000000 dtfabric-20230512/dtfabric/reader.py
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     3192 2022-09-18 09:35:13.000000 dtfabric-20230512/dtfabric/registry.py
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-12 04:07:16.461437 dtfabric-20230512/dtfabric/runtime/
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       24 2018-03-18 06:58:01.000000 dtfabric-20230512/dtfabric/runtime/__init__.py
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     2523 2022-09-18 09:36:04.000000 dtfabric-20230512/dtfabric/runtime/byte_operations.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    71655 2022-09-25 14:31:31.000000 dtfabric-20230512/dtfabric/runtime/data_maps.py
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1157 2022-01-27 14:27:48.000000 dtfabric-20230512/dtfabric/runtime/fabric.py
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     6233 2022-09-18 09:46:53.000000 dtfabric-20230512/dtfabric/runtime/runtime.py
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-12 04:07:16.459437 dtfabric-20230512/dtfabric.egg-info/
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      583 2023-05-12 04:07:14.000000 dtfabric-20230512/dtfabric.egg-info/PKG-INFO
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     2835 2023-05-12 04:07:16.000000 dtfabric-20230512/dtfabric.egg-info/SOURCES.txt
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)        1 2023-05-12 04:07:14.000000 dtfabric-20230512/dtfabric.egg-info/dependency_links.txt
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       24 2023-05-12 04:07:14.000000 dtfabric-20230512/dtfabric.egg-info/requires.txt
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)        9 2023-05-12 04:07:14.000000 dtfabric-20230512/dtfabric.egg-info/top_level.txt
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      395 2019-02-03 12:58:57.000000 dtfabric-20230512/dtfabric.ini
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       28 2023-05-08 04:44:50.000000 dtfabric-20230512/requirements.txt
--rwxrwxr-x   0 lordyesta  (1000) lordyesta  (1000)      777 2022-09-18 09:32:38.000000 dtfabric-20230512/run_tests.py
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-12 04:07:16.461437 dtfabric-20230512/scripts/
--rwxrwxr-x   0 lordyesta  (1000) lordyesta  (1000)     3218 2022-09-18 08:56:58.000000 dtfabric-20230512/scripts/validate-definitions.py
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      302 2023-05-12 04:07:16.686437 dtfabric-20230512/setup.cfg
--rwxrwxr-x   0 lordyesta  (1000) lordyesta  (1000)     6782 2023-05-08 04:44:50.000000 dtfabric-20230512/setup.py
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-12 04:07:16.486437 dtfabric-20230512/test_data/
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1426 2017-05-01 13:58:49.000000 dtfabric-20230512/test_data/Notepad.lnk
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       99 2022-07-10 05:55:10.000000 dtfabric-20230512/test_data/boolean.yaml
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      101 2022-07-10 05:55:12.000000 dtfabric-20230512/test_data/character.yaml
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      284 2022-07-10 05:55:13.000000 dtfabric-20230512/test_data/constant.yaml
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-12 04:07:16.487437 dtfabric-20230512/test_data/definitions/
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      524 2022-07-10 05:54:56.000000 dtfabric-20230512/test_data/definitions/booleans.yaml
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      453 2022-07-10 05:54:58.000000 dtfabric-20230512/test_data/definitions/characters.yaml
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      405 2022-07-10 05:55:00.000000 dtfabric-20230512/test_data/definitions/floating-points.yaml
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1364 2022-07-10 05:55:01.000000 dtfabric-20230512/test_data/definitions/integers.yaml
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      812 2022-07-10 05:55:15.000000 dtfabric-20230512/test_data/enumeration.yaml
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      218 2022-07-10 05:55:16.000000 dtfabric-20230512/test_data/floating-point.yaml
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      555 2022-07-10 05:55:18.000000 dtfabric-20230512/test_data/format.yaml
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      399 2022-07-10 05:55:19.000000 dtfabric-20230512/test_data/integer.yaml
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       83 2022-07-10 05:55:23.000000 dtfabric-20230512/test_data/padding.yaml
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      457 2022-07-10 05:55:28.000000 dtfabric-20230512/test_data/sequence.yaml
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      572 2022-07-10 05:55:25.000000 dtfabric-20230512/test_data/sequence_with_context.yaml
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      433 2022-07-10 05:55:26.000000 dtfabric-20230512/test_data/sequence_with_structure.yaml
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      657 2022-07-10 05:55:29.000000 dtfabric-20230512/test_data/stream.yaml
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      707 2022-07-10 05:55:32.000000 dtfabric-20230512/test_data/string.yaml
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      818 2022-07-10 05:55:30.000000 dtfabric-20230512/test_data/string_array.yaml
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1059 2022-07-10 05:55:50.000000 dtfabric-20230512/test_data/structure.yaml
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     3131 2022-07-10 05:55:34.000000 dtfabric-20230512/test_data/structure_family.yaml
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1576 2022-07-10 05:55:35.000000 dtfabric-20230512/test_data/structure_group.yaml
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      651 2022-07-10 05:55:36.000000 dtfabric-20230512/test_data/structure_with_condition.yaml
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      496 2022-07-10 05:55:38.000000 dtfabric-20230512/test_data/structure_with_context.yaml
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      712 2022-07-10 05:57:13.000000 dtfabric-20230512/test_data/structure_with_padding.yaml
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      322 2022-07-10 05:55:41.000000 dtfabric-20230512/test_data/structure_with_section.yaml
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      468 2022-07-10 05:55:43.000000 dtfabric-20230512/test_data/structure_with_sequence.yaml
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      466 2022-07-10 05:55:44.000000 dtfabric-20230512/test_data/structure_with_stream.yaml
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      446 2022-07-10 05:55:45.000000 dtfabric-20230512/test_data/structure_with_string.yaml
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      370 2022-07-10 05:55:47.000000 dtfabric-20230512/test_data/structure_with_union.yaml
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      700 2022-07-10 05:55:49.000000 dtfabric-20230512/test_data/structure_with_values.yaml
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      383 2022-07-10 05:55:53.000000 dtfabric-20230512/test_data/union.yaml
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      380 2022-07-10 05:55:51.000000 dtfabric-20230512/test_data/union_with_condition.yaml
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      200 2022-07-10 05:55:54.000000 dtfabric-20230512/test_data/uuid.yaml
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      107 2022-12-18 07:46:44.000000 dtfabric-20230512/test_dependencies.ini
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       14 2023-05-08 04:44:50.000000 dtfabric-20230512/test_requirements.txt
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-12 04:07:16.618437 dtfabric-20230512/tests/
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       24 2018-03-18 06:58:01.000000 dtfabric-20230512/tests/__init__.py
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    19685 2022-02-13 10:09:16.000000 dtfabric-20230512/tests/data_types.py
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    62062 2022-07-10 05:53:49.000000 dtfabric-20230512/tests/reader.py
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     3002 2021-07-30 06:46:25.000000 dtfabric-20230512/tests/registry.py
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-12 04:07:16.683438 dtfabric-20230512/tests/runtime/
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       24 2018-03-18 06:58:01.000000 dtfabric-20230512/tests/runtime/__init__.py
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1645 2021-07-30 09:04:50.000000 dtfabric-20230512/tests/runtime/byte_operations.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    83501 2022-09-25 13:56:56.000000 dtfabric-20230512/tests/runtime/data_maps.py
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      662 2021-07-30 06:46:25.000000 dtfabric-20230512/tests/runtime/fabric.py
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     2494 2021-07-30 06:46:25.000000 dtfabric-20230512/tests/runtime/runtime.py
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     2272 2022-09-18 09:32:59.000000 dtfabric-20230512/tests/test_lib.py
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1252 2023-05-08 04:44:51.000000 dtfabric-20230512/tox.ini
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-12 04:07:16.684438 dtfabric-20230512/utils/
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       70 2018-03-18 06:58:04.000000 dtfabric-20230512/utils/__init__.py
--rwxrwxr-x   0 lordyesta  (1000) lordyesta  (1000)      422 2023-05-08 04:44:50.000000 dtfabric-20230512/utils/check_dependencies.py
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    11583 2023-05-08 04:44:51.000000 dtfabric-20230512/utils/dependencies.py
--rwxrwxr-x   0 lordyesta  (1000) lordyesta  (1000)      616 2021-12-28 04:01:20.000000 dtfabric-20230512/utils/update_release.sh
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-18 16:25:30.548572 dtfabric-20230518/
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-18 16:25:30.209572 dtfabric-20230518/.github/
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-18 16:25:30.310572 dtfabric-20230518/.github/workflows/
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     2541 2023-05-12 04:16:07.000000 dtfabric-20230518/.github/workflows/test_docker.yml
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1378 2023-05-12 04:16:07.000000 dtfabric-20230518/.github/workflows/test_docs.yml
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     4107 2023-05-12 04:16:07.000000 dtfabric-20230518/.github/workflows/test_tox.yml
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    22994 2023-05-12 04:16:07.000000 dtfabric-20230518/.pylintrc
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      149 2022-07-10 04:44:41.000000 dtfabric-20230518/.yamllint.yaml
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       92 2022-01-24 07:36:34.000000 dtfabric-20230518/ACKNOWLEDGEMENTS
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      265 2018-07-03 18:38:13.000000 dtfabric-20230518/AUTHORS
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    11358 2016-09-25 06:41:25.000000 dtfabric-20230518/LICENSE
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      592 2021-08-22 05:30:09.000000 dtfabric-20230518/MANIFEST.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      583 2023-05-18 16:25:30.548572 dtfabric-20230518/PKG-INFO
+-rw-r-----   0 lordyesta  (1000) lordyesta  (1000)      195 2020-06-21 05:38:03.000000 dtfabric-20230518/README
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1230 2023-05-12 04:16:07.000000 dtfabric-20230518/appveyor.yml
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-18 16:25:30.210572 dtfabric-20230518/config/
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-18 16:25:30.312572 dtfabric-20230518/config/appveyor/
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      839 2023-05-12 04:16:07.000000 dtfabric-20230518/config/appveyor/install.ps1
+-rwxrwxr-x   0 lordyesta  (1000) lordyesta  (1000)      125 2023-05-12 04:16:07.000000 dtfabric-20230518/config/appveyor/install.sh
+-rwxrwxr-x   0 lordyesta  (1000) lordyesta  (1000)      620 2023-05-12 04:16:07.000000 dtfabric-20230518/config/appveyor/runtests.sh
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-18 16:25:30.364572 dtfabric-20230518/config/dpkg/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      140 2023-05-18 11:05:37.000000 dtfabric-20230518/config/dpkg/changelog
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       38 2017-05-26 07:25:10.000000 dtfabric-20230518/config/dpkg/clean
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)        2 2023-05-12 04:16:07.000000 dtfabric-20230518/config/dpkg/compat
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      786 2023-05-12 04:16:07.000000 dtfabric-20230518/config/dpkg/control
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      884 2017-04-14 13:14:48.000000 dtfabric-20230518/config/dpkg/copyright
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       20 2017-04-14 13:31:35.000000 dtfabric-20230518/config/dpkg/dtfabric-data.dirs
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       26 2017-04-14 13:32:40.000000 dtfabric-20230518/config/dpkg/dtfabric-data.install
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      144 2017-05-26 07:25:20.000000 dtfabric-20230518/config/dpkg/python-dtfabric.install
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      144 2017-05-26 07:25:27.000000 dtfabric-20230518/config/dpkg/python3-dtfabric.install
+-rwxrwxr-x   0 lordyesta  (1000) lordyesta  (1000)      122 2023-05-12 04:16:07.000000 dtfabric-20230518/config/dpkg/rules
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-18 16:25:30.378572 dtfabric-20230518/config/dpkg/source/
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       12 2017-04-14 13:14:48.000000 dtfabric-20230518/config/dpkg/source/format
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-18 16:25:30.379572 dtfabric-20230518/config/pylint/
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      362 2020-06-21 09:14:13.000000 dtfabric-20230518/config/pylint/spelling-private-dict
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      151 2020-01-19 18:45:05.000000 dtfabric-20230518/dependencies.ini
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-18 16:25:30.397572 dtfabric-20230518/docs/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5061 2023-05-12 04:16:07.000000 dtfabric-20230518/docs/conf.py
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      566 2021-07-30 06:46:25.000000 dtfabric-20230518/docs/index.rst
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      105 2023-05-12 04:16:16.000000 dtfabric-20230518/docs/requirements.txt
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-18 16:25:30.408572 dtfabric-20230518/docs/sources/
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    15554 2022-07-10 05:53:49.000000 dtfabric-20230518/docs/sources/Format-specification.md
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-18 16:25:30.447572 dtfabric-20230518/docs/sources/api/
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1097 2022-02-19 13:55:33.000000 dtfabric-20230518/docs/sources/api/dtfabric.rst
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      869 2021-07-30 06:46:25.000000 dtfabric-20230518/docs/sources/api/dtfabric.runtime.rst
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       61 2021-07-30 06:37:51.000000 dtfabric-20230518/docs/sources/api/modules.rst
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-18 16:25:30.454572 dtfabric-20230518/docs/sources/user/
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1633 2021-12-28 03:59:54.000000 dtfabric-20230518/docs/sources/user/Installation-instructions.md
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      288 2021-07-30 06:37:51.000000 dtfabric-20230518/docs/sources/user/index.rst
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-18 16:25:30.473572 dtfabric-20230518/dtfabric/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       74 2023-05-18 11:04:17.000000 dtfabric-20230518/dtfabric/__init__.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    31346 2023-05-14 14:27:49.000000 dtfabric-20230518/dtfabric/data_types.py
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      710 2022-09-18 09:38:10.000000 dtfabric-20230518/dtfabric/decorators.py
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1502 2021-07-30 10:44:15.000000 dtfabric-20230518/dtfabric/definitions.py
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1016 2021-07-30 06:46:25.000000 dtfabric-20230518/dtfabric/errors.py
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    52825 2023-05-18 03:12:53.000000 dtfabric-20230518/dtfabric/reader.py
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     3192 2022-09-18 09:35:13.000000 dtfabric-20230518/dtfabric/registry.py
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-18 16:25:30.512572 dtfabric-20230518/dtfabric/runtime/
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       24 2018-03-18 06:58:01.000000 dtfabric-20230518/dtfabric/runtime/__init__.py
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     2523 2022-09-18 09:36:04.000000 dtfabric-20230518/dtfabric/runtime/byte_operations.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    76230 2023-05-18 16:17:58.000000 dtfabric-20230518/dtfabric/runtime/data_maps.py
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1157 2022-01-27 14:27:48.000000 dtfabric-20230518/dtfabric/runtime/fabric.py
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     6233 2022-09-18 09:46:53.000000 dtfabric-20230518/dtfabric/runtime/runtime.py
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-18 16:25:30.483572 dtfabric-20230518/dtfabric.egg-info/
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      583 2023-05-18 16:25:28.000000 dtfabric-20230518/dtfabric.egg-info/PKG-INFO
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     2877 2023-05-18 16:25:29.000000 dtfabric-20230518/dtfabric.egg-info/SOURCES.txt
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)        1 2023-05-18 16:25:28.000000 dtfabric-20230518/dtfabric.egg-info/dependency_links.txt
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       24 2023-05-18 16:25:28.000000 dtfabric-20230518/dtfabric.egg-info/requires.txt
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)        9 2023-05-18 16:25:28.000000 dtfabric-20230518/dtfabric.egg-info/top_level.txt
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      395 2019-02-03 12:58:57.000000 dtfabric-20230518/dtfabric.ini
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       28 2023-05-12 04:16:07.000000 dtfabric-20230518/requirements.txt
+-rwxrwxr-x   0 lordyesta  (1000) lordyesta  (1000)      777 2022-09-18 09:32:38.000000 dtfabric-20230518/run_tests.py
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-18 16:25:30.534572 dtfabric-20230518/scripts/
+-rwxrwxr-x   0 lordyesta  (1000) lordyesta  (1000)     3218 2022-09-18 08:56:58.000000 dtfabric-20230518/scripts/validate-definitions.py
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      302 2023-05-18 16:25:30.549572 dtfabric-20230518/setup.cfg
+-rwxrwxr-x   0 lordyesta  (1000) lordyesta  (1000)     6782 2023-05-12 04:16:07.000000 dtfabric-20230518/setup.py
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-18 16:25:30.543572 dtfabric-20230518/test_data/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12288 2023-05-18 15:47:17.000000 dtfabric-20230518/test_data/.structure_with_string.yaml.swp
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1426 2017-05-01 13:58:49.000000 dtfabric-20230518/test_data/Notepad.lnk
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       99 2022-07-10 05:55:10.000000 dtfabric-20230518/test_data/boolean.yaml
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      101 2022-07-10 05:55:12.000000 dtfabric-20230518/test_data/character.yaml
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      284 2022-07-10 05:55:13.000000 dtfabric-20230518/test_data/constant.yaml
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-18 16:25:30.544572 dtfabric-20230518/test_data/definitions/
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      524 2022-07-10 05:54:56.000000 dtfabric-20230518/test_data/definitions/booleans.yaml
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      453 2022-07-10 05:54:58.000000 dtfabric-20230518/test_data/definitions/characters.yaml
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      405 2022-07-10 05:55:00.000000 dtfabric-20230518/test_data/definitions/floating-points.yaml
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1364 2022-07-10 05:55:01.000000 dtfabric-20230518/test_data/definitions/integers.yaml
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      812 2022-07-10 05:55:15.000000 dtfabric-20230518/test_data/enumeration.yaml
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      218 2022-07-10 05:55:16.000000 dtfabric-20230518/test_data/floating-point.yaml
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      555 2022-07-10 05:55:18.000000 dtfabric-20230518/test_data/format.yaml
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      399 2022-07-10 05:55:19.000000 dtfabric-20230518/test_data/integer.yaml
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       83 2022-07-10 05:55:23.000000 dtfabric-20230518/test_data/padding.yaml
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      457 2022-07-10 05:55:28.000000 dtfabric-20230518/test_data/sequence.yaml
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      572 2022-07-10 05:55:25.000000 dtfabric-20230518/test_data/sequence_with_context.yaml
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      433 2023-05-18 05:56:24.000000 dtfabric-20230518/test_data/sequence_with_structure.yaml
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      657 2022-07-10 05:55:29.000000 dtfabric-20230518/test_data/stream.yaml
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      707 2022-07-10 05:55:32.000000 dtfabric-20230518/test_data/string.yaml
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      818 2022-07-10 05:55:30.000000 dtfabric-20230518/test_data/string_array.yaml
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1059 2022-07-10 05:55:50.000000 dtfabric-20230518/test_data/structure.yaml
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     3131 2022-07-10 05:55:34.000000 dtfabric-20230518/test_data/structure_family.yaml
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1576 2022-07-10 05:55:35.000000 dtfabric-20230518/test_data/structure_group.yaml
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      651 2022-07-10 05:55:36.000000 dtfabric-20230518/test_data/structure_with_condition.yaml
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      496 2022-07-10 05:55:38.000000 dtfabric-20230518/test_data/structure_with_context.yaml
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      712 2022-07-10 05:57:13.000000 dtfabric-20230518/test_data/structure_with_padding.yaml
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      322 2022-07-10 05:55:41.000000 dtfabric-20230518/test_data/structure_with_section.yaml
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      468 2022-07-10 05:55:43.000000 dtfabric-20230518/test_data/structure_with_sequence.yaml
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      466 2022-07-10 05:55:44.000000 dtfabric-20230518/test_data/structure_with_stream.yaml
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      446 2022-07-10 05:55:45.000000 dtfabric-20230518/test_data/structure_with_string.yaml
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      370 2022-07-10 05:55:47.000000 dtfabric-20230518/test_data/structure_with_union.yaml
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      700 2022-07-10 05:55:49.000000 dtfabric-20230518/test_data/structure_with_values.yaml
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      383 2022-07-10 05:55:53.000000 dtfabric-20230518/test_data/union.yaml
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      380 2022-07-10 05:55:51.000000 dtfabric-20230518/test_data/union_with_condition.yaml
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      200 2022-07-10 05:55:54.000000 dtfabric-20230518/test_data/uuid.yaml
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      107 2022-12-18 07:46:44.000000 dtfabric-20230518/test_dependencies.ini
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       14 2023-05-12 04:16:07.000000 dtfabric-20230518/test_requirements.txt
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-18 16:25:30.545572 dtfabric-20230518/tests/
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       24 2018-03-18 06:58:01.000000 dtfabric-20230518/tests/__init__.py
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    19685 2022-02-13 10:09:16.000000 dtfabric-20230518/tests/data_types.py
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    62234 2023-05-18 03:22:07.000000 dtfabric-20230518/tests/reader.py
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     3002 2021-07-30 06:46:25.000000 dtfabric-20230518/tests/registry.py
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-18 16:25:30.547572 dtfabric-20230518/tests/runtime/
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       24 2018-03-18 06:58:01.000000 dtfabric-20230518/tests/runtime/__init__.py
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1645 2021-07-30 09:04:50.000000 dtfabric-20230518/tests/runtime/byte_operations.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    84696 2023-05-18 15:50:47.000000 dtfabric-20230518/tests/runtime/data_maps.py
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      662 2021-07-30 06:46:25.000000 dtfabric-20230518/tests/runtime/fabric.py
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     2494 2021-07-30 06:46:25.000000 dtfabric-20230518/tests/runtime/runtime.py
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     2272 2022-09-18 09:32:59.000000 dtfabric-20230518/tests/test_lib.py
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1252 2023-05-12 04:16:07.000000 dtfabric-20230518/tox.ini
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-18 16:25:30.548572 dtfabric-20230518/utils/
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       70 2018-03-18 06:58:04.000000 dtfabric-20230518/utils/__init__.py
+-rwxrwxr-x   0 lordyesta  (1000) lordyesta  (1000)      422 2023-05-12 04:16:07.000000 dtfabric-20230518/utils/check_dependencies.py
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    11583 2023-05-12 04:16:07.000000 dtfabric-20230518/utils/dependencies.py
+-rwxrwxr-x   0 lordyesta  (1000) lordyesta  (1000)      616 2021-12-28 04:01:20.000000 dtfabric-20230518/utils/update_release.sh
```

### Comparing `dtfabric-20230512/.github/workflows/test_docker.yml` & `dtfabric-20230518/.github/workflows/test_docker.yml`

 * *Files identical despite different names*

### Comparing `dtfabric-20230512/.github/workflows/test_docs.yml` & `dtfabric-20230518/.github/workflows/test_docs.yml`

 * *Files identical despite different names*

### Comparing `dtfabric-20230512/.github/workflows/test_tox.yml` & `dtfabric-20230518/.github/workflows/test_tox.yml`

 * *Files identical despite different names*

### Comparing `dtfabric-20230512/.pylintrc` & `dtfabric-20230518/.pylintrc`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,22 @@
-# Pylint 2.14.x configuration file
+# Pylint 2.17.x configuration file
 #
 # This file is generated by l2tdevtools update-dependencies.py, any dependency
 # related changes should be made in dependencies.ini.
 [MAIN]
 
 # Analyse import fallback blocks. This can be used to support both Python 2 and
 # 3 compatible code, which means that the block might have code that exists
 # only in one or another interpreter, leading to false positives when analysed.
 analyse-fallback-blocks=no
 
+# Clear in-memory caches upon conclusion of linting. Useful if running pylint
+# in a server-like mode.
+clear-cache-post-run=no
+
 # Load and enable all available extensions. Use --list-extensions to see a list
 # all available extensions.
 #enable-all-extensions=
 
 # In error mode, messages with a category besides ERROR or FATAL are
 # suppressed, and no reports are done by default. Error mode is compatible with
 # disabling specific errors.
@@ -34,31 +38,33 @@
 extension-pkg-whitelist=
 
 # Return non-zero exit code if any of these messages/categories are detected,
 # even if score is above --fail-under value. Syntax same as enable. Messages
 # specified are enabled, while categories only check already-enabled messages.
 fail-on=
 
-# Specify a score threshold to be exceeded before program exits with error.
+# Specify a score threshold under which the program will exit with error.
 fail-under=10
 
 # Interpret the stdin as a python script, whose filename needs to be passed as
 # the module_or_package argument.
 #from-stdin=
 
 # Files or directories to be skipped. They should be base names, not paths.
 ignore=CVS
 
-# Add files or directories matching the regex patterns to the ignore-list. The
-# regex matches against paths and can be in Posix or Windows format.
+# Add files or directories matching the regular expressions patterns to the
+# ignore-list. The regex matches against paths and can be in Posix or Windows
+# format. Because '\\' represents the directory delimiter on Windows systems,
+# it can't be used as an escape character.
 ignore-paths=
 
-# Files or directories matching the regex patterns are skipped. The regex
-# matches against base names, not paths. The default value ignores Emacs file
-# locks
+# Files or directories matching the regular expression patterns are skipped.
+# The regex matches against base names, not paths. The default value ignores
+# Emacs file locks
 ignore-patterns=^\.#
 
 # List of module names for which member attributes should not be checked
 # (useful for modules/projects where namespaces are manipulated during runtime
 # and thus existing member attributes cannot be deduced by static analysis). It
 # supports qualified module names, as well as Unix pattern matching.
 ignored-modules=
@@ -89,249 +95,32 @@
 # the version used to run pylint.
 py-version=3.11
 
 # Discover python modules and packages in the file system subtree.
 # recursive=no
 recursive=yes
 
+# Add paths to the list of the source roots. Supports globbing patterns. The
+# source root is an absolute path or a path relative to the current working
+# directory used to determine a package namespace for modules located under the
+# source root.
+source-roots=
+
 # When enabled, pylint would attempt to guess common misconfiguration and emit
 # user-friendly hints instead of false-positive error messages.
 suggestion-mode=yes
 
 # Allow loading of arbitrary C extensions. Extensions are imported into the
 # active Python interpreter and may run arbitrary code.
 unsafe-load-any-extension=no
 
 # In verbose mode, extra non-checker-related info will be displayed.
 #verbose=
 
 
-[REPORTS]
-
-# Python expression which should return a score less than or equal to 10. You
-# have access to the variables 'fatal', 'error', 'warning', 'refactor',
-# 'convention', and 'info' which contain the number of messages in each
-# category, as well as 'statement' which is the total number of statements
-# analyzed. This score is used by the global evaluation report (RP0004).
-evaluation=max(0, 0 if fatal else 10.0 - ((float(5 * error + warning + refactor + convention) / statement) * 10))
-
-# Template used to display messages. This is a python new-style format string
-# used to format the message information. See doc for all details.
-msg-template=
-
-# Set the output format. Available formats are text, parseable, colorized, json
-# and msvs (visual studio). You can also give a reporter class, e.g.
-# mypackage.mymodule.MyReporterClass.
-#output-format=
-
-# Tells whether to display a full report or only the messages.
-reports=no
-
-# Activate the evaluation score.
-# score=yes
-score=no
-
-
-[MESSAGES CONTROL]
-
-# Only show warnings with the listed confidence levels. Leave empty to show
-# all. Valid levels: HIGH, CONTROL_FLOW, INFERENCE, INFERENCE_FAILURE,
-# UNDEFINED.
-confidence=HIGH,
-           CONTROL_FLOW,
-           INFERENCE,
-           INFERENCE_FAILURE,
-           UNDEFINED
-
-# Disable the message, report, category or checker with the given id(s). You
-# can either give multiple identifiers separated by comma (,) or put this
-# option multiple times (only on the command line, not in the configuration
-# file where it should appear only once). You can also use "--disable=all" to
-# disable everything first and then re-enable specific checks. For example, if
-# you want to run only the similarities checker, you can use "--disable=all
-# --enable=similarities". If you want to run only the classes checker, but have
-# no Warning level messages displayed, use "--disable=all --enable=classes
-# --disable=W".
-disable=assignment-from-none,
-        bad-inline-option,
-        consider-using-f-string,
-        deprecated-pragma,
-        duplicate-code,
-        file-ignored,
-        fixme,
-        locally-disabled,
-        logging-format-interpolation,
-        logging-fstring-interpolation,
-        missing-param-doc,
-        raise-missing-from,
-        raw-checker-failed,
-        super-with-arguments,
-        suppressed-message,
-        too-few-public-methods,
-        too-many-ancestors,
-        too-many-boolean-expressions,
-        too-many-branches,
-        too-many-instance-attributes,
-        too-many-lines,
-        too-many-locals,
-        too-many-nested-blocks,
-        too-many-public-methods,
-        too-many-return-statements,
-        too-many-statements,
-        unsubscriptable-object,
-        useless-object-inheritance,
-        useless-suppression
-
-# Enable the message, report, category or checker with the given id(s). You can
-# either give multiple identifier separated by comma (,) or put this option
-# multiple time (only on the command line, not in the configuration file where
-# it should appear only once). See also the "--disable" option for examples.
-enable=c-extension-no-member
-
-
-[VARIABLES]
-
-# List of additional names supposed to be defined in builtins. Remember that
-# you should avoid defining new builtins when possible.
-additional-builtins=
-
-# Tells whether unused global variables should be treated as a violation.
-allow-global-unused-variables=yes
-
-# List of names allowed to shadow builtins
-allowed-redefined-builtins=
-
-# List of strings which can identify a callback function by name. A callback
-# name must start or end with one of those strings.
-callbacks=cb_,
-          _cb
-
-# A regular expression matching the name of dummy variables (i.e. expected to
-# not be used).
-dummy-variables-rgx=_+$|(_[a-zA-Z0-9_]*[a-zA-Z0-9]+?$)|dummy|^ignored_|^unused_
-
-# Argument names that match this expression will be ignored. Default to name
-# with leading underscore.
-ignored-argument-names=_.*|^ignored_|^unused_
-
-# Tells whether we should check for unused import in __init__ files.
-init-import=no
-
-# List of qualified module names which can have objects that can redefine
-# builtins.
-redefining-builtins-modules=six.moves,past.builtins,future.builtins,builtins,io
-
-
-[TYPECHECK]
-
-# List of decorators that produce context managers, such as
-# contextlib.contextmanager. Add to this list to register other decorators that
-# produce valid context managers.
-contextmanager-decorators=contextlib.contextmanager
-
-# List of members which are set dynamically and missed by pylint inference
-# system, and so shouldn't trigger E1101 when accessed. Python regular
-# expressions are accepted.
-generated-members=
-
-# Tells whether to warn about missing members when the owner of the attribute
-# is inferred to be None.
-ignore-none=yes
-
-# This flag controls whether pylint should warn about no-member and similar
-# checks whenever an opaque object is returned when inferring. The inference
-# can return multiple potential results while evaluating a Python object, but
-# some branches might not be evaluated, which results in partial inference. In
-# that case, it might be useful to still emit no-member and other checks for
-# the rest of the inferred objects.
-ignore-on-opaque-inference=yes
-
-# List of symbolic message names to ignore for Mixin members.
-ignored-checks-for-mixins=no-member,
-                          not-async-context-manager,
-                          not-context-manager,
-                          attribute-defined-outside-init
-
-# List of class names for which member attributes should not be checked (useful
-# for classes with dynamically set attributes). This supports the use of
-# qualified names.
-ignored-classes=optparse.Values,thread._local,_thread._local,argparse.Namespace
-
-# Show a hint with possible names when a member name was not found. The aspect
-# of finding the hint is based on edit distance.
-missing-member-hint=yes
-
-# The minimum edit distance a name should have in order to be considered a
-# similar match for a missing member name.
-missing-member-hint-distance=1
-
-# The total number of similar names that should be taken in consideration when
-# showing a hint for a missing member.
-missing-member-max-choices=1
-
-# Regex pattern to define which classes are considered mixins.
-mixin-class-rgx=.*[Mm]ixin
-
-# List of decorators that change the signature of a decorated function.
-signature-mutators=
-
-
-[LOGGING]
-
-# The type of string formatting that logging methods do. `old` means using %
-# formatting, `new` is for `{}` formatting.
-logging-format-style=old
-
-# Logging modules to check that the string format arguments are in logging
-# function parameter format.
-logging-modules=logging
-
-
-[DESIGN]
-
-# List of regular expressions of class ancestor names to ignore when counting
-# public methods (see R0903)
-exclude-too-few-public-methods=
-
-# List of qualified class names to ignore when counting class parents (see
-# R0901)
-ignored-parents=
-
-# Maximum number of arguments for function / method.
-# max-args=5
-max-args=10
-
-# Maximum number of attributes for a class (see R0902).
-max-attributes=7
-
-# Maximum number of boolean expressions in an if statement (see R0916).
-max-bool-expr=5
-
-# Maximum number of branch for function / method body.
-max-branches=12
-
-# Maximum number of locals for function / method body.
-max-locals=15
-
-# Maximum number of parents for a class (see R0901).
-max-parents=7
-
-# Maximum number of public methods for a class (see R0904).
-max-public-methods=20
-
-# Maximum number of return / yield for function / method body.
-max-returns=6
-
-# Maximum number of statements in function / method body.
-max-statements=50
-
-# Minimum number of public methods for a class (see R0903).
-min-public-methods=2
-
-
 [BASIC]
 
 # Naming style matching correct argument names.
 argument-naming-style=snake_case
 
 # Regular expression matching correct argument names. Overrides argument-
 # naming-style. If left empty, argument names will be checked with the set
@@ -456,70 +245,102 @@
 no-docstring-rgx=^_
 
 # List of decorators that produce properties, such as abc.abstractproperty. Add
 # to this list to register other decorators that produce valid properties.
 # These decorators are taken in consideration only for invalid-name.
 property-classes=abc.abstractproperty
 
+# Regular expression matching correct type alias names. If left empty, type
+# alias names will be checked with the set naming style.
+#typealias-rgx=
+
 # Regular expression matching correct type variable names. If left empty, type
 # variable names will be checked with the set naming style.
 #typevar-rgx=
 
 # Naming style matching correct variable names.
 variable-naming-style=snake_case
 
 # Regular expression matching correct variable names. Overrides variable-
 # naming-style. If left empty, variable names will be checked with the set
 # naming style.
 #variable-rgx=
 variable-rgx=(([a-z][a-z0-9_]*)|(_[a-z0-9_]*))$
 
 
-[EXCEPTIONS]
-
-# Exceptions that will emit a warning when caught.
-overgeneral-exceptions=BaseException,
-                       Exception
-
-
 [CLASSES]
 
 # Warn about protected attribute access inside special methods
 check-protected-access-in-special-methods=no
 
 # List of method names used to declare (i.e. assign) instance attributes.
 defining-attr-methods=__init__,
                       __new__,
                       setUp,
+                      asyncSetUp,
                       __post_init__
 
 # List of member names, which should be excluded from the protected access
 # warning.
-exclude-protected=_asdict,
-                  _fields,
-                  _replace,
-                  _source,
-                  _make
+exclude-protected=_asdict,_fields,_replace,_source,_make,os._exit
 
 # List of valid names for the first argument in a class method.
 valid-classmethod-first-arg=cls
 
 # List of valid names for the first argument in a metaclass class method.
+# valid-metaclass-classmethod-first-arg=mcs
 valid-metaclass-classmethod-first-arg=cls
 
 
-[MISCELLANEOUS]
+[DESIGN]
 
-# List of note tags to take in consideration, separated by a comma.
-notes=FIXME,
-      XXX,
-      TODO
+# List of regular expressions of class ancestor names to ignore when counting
+# public methods (see R0903)
+exclude-too-few-public-methods=
 
-# Regular expression of note tags to take in consideration.
-notes-rgx=
+# List of qualified class names to ignore when counting class parents (see
+# R0901)
+ignored-parents=
+
+# Maximum number of arguments for function / method.
+# max-args=5
+max-args=10
+
+# Maximum number of attributes for a class (see R0902).
+max-attributes=7
+
+# Maximum number of boolean expressions in an if statement (see R0916).
+max-bool-expr=5
+
+# Maximum number of branch for function / method body.
+max-branches=12
+
+# Maximum number of locals for function / method body.
+max-locals=15
+
+# Maximum number of parents for a class (see R0901).
+max-parents=7
+
+# Maximum number of public methods for a class (see R0904).
+max-public-methods=20
+
+# Maximum number of return / yield for function / method body.
+max-returns=6
+
+# Maximum number of statements in function / method body.
+max-statements=50
+
+# Minimum number of public methods for a class (see R0903).
+min-public-methods=2
+
+
+[EXCEPTIONS]
+
+# Exceptions that will emit a warning when caught.
+overgeneral-exceptions=builtins.BaseException,builtins.Exception
 
 
 [FORMAT]
 
 # Expected format of line ending, e.g. empty (any line ending), LF or CRLF.
 expected-line-ending-format=
 
@@ -546,14 +367,196 @@
 single-line-class-stmt=no
 
 # Allow the body of an if to be on the same line as the test if there is no
 # else.
 single-line-if-stmt=no
 
 
+[IMPORTS]
+
+# List of modules that can be imported at any level, not just the top level
+# one.
+allow-any-import-level=
+
+# Allow explicit reexports by alias from a package __init__.
+allow-reexport-from-package=no
+
+# Allow wildcard imports from modules that define __all__.
+allow-wildcard-with-all=no
+
+# Deprecated modules which should not be used, separated by a comma.
+deprecated-modules=
+
+# Output a graph (.gv or any supported image format) of external dependencies
+# to the given file (report RP0402 must not be disabled).
+ext-import-graph=
+
+# Output a graph (.gv or any supported image format) of all (i.e. internal and
+# external) dependencies to the given file (report RP0402 must not be
+# disabled).
+import-graph=
+
+# Output a graph (.gv or any supported image format) of internal dependencies
+# to the given file (report RP0402 must not be disabled).
+int-import-graph=
+
+# Force import order to recognize a module as part of the standard
+# compatibility libraries.
+known-standard-library=
+
+# Force import order to recognize a module as part of a third party library.
+known-third-party=enchant
+
+# Couples of modules and preferred modules, separated by a comma.
+preferred-modules=
+
+
+[LOGGING]
+
+# The type of string formatting that logging methods do. `old` means using %
+# formatting, `new` is for `{}` formatting.
+logging-format-style=old
+
+# Logging modules to check that the string format arguments are in logging
+# function parameter format.
+logging-modules=logging
+
+
+[MESSAGES CONTROL]
+
+# Only show warnings with the listed confidence levels. Leave empty to show
+# all. Valid levels: HIGH, CONTROL_FLOW, INFERENCE, INFERENCE_FAILURE,
+# UNDEFINED.
+confidence=HIGH,
+           CONTROL_FLOW,
+           INFERENCE,
+           INFERENCE_FAILURE,
+           UNDEFINED
+
+# Disable the message, report, category or checker with the given id(s). You
+# can either give multiple identifiers separated by comma (,) or put this
+# option multiple times (only on the command line, not in the configuration
+# file where it should appear only once). You can also use "--disable=all" to
+# disable everything first and then re-enable specific checks. For example, if
+# you want to run only the similarities checker, you can use "--disable=all
+# --enable=similarities". If you want to run only the classes checker, but have
+# no Warning level messages displayed, use "--disable=all --enable=classes
+# --disable=W".
+disable=assignment-from-none,
+        bad-inline-option,
+        consider-using-f-string,
+        deprecated-pragma,
+        duplicate-code,
+        file-ignored,
+        fixme,
+        locally-disabled,
+        logging-format-interpolation,
+        logging-fstring-interpolation,
+        missing-param-doc,
+        raise-missing-from,
+        raw-checker-failed,
+        super-with-arguments,
+        suppressed-message,
+        too-few-public-methods,
+        too-many-ancestors,
+        too-many-boolean-expressions,
+        too-many-branches,
+        too-many-instance-attributes,
+        too-many-lines,
+        too-many-locals,
+        too-many-nested-blocks,
+        too-many-public-methods,
+        too-many-return-statements,
+        too-many-statements,
+        unsubscriptable-object,
+        useless-object-inheritance,
+        useless-suppression,
+        use-symbolic-message-instead
+
+# Enable the message, report, category or checker with the given id(s). You can
+# either give multiple identifier separated by comma (,) or put this option
+# multiple time (only on the command line, not in the configuration file where
+# it should appear only once). See also the "--disable" option for examples.
+enable=c-extension-no-member
+
+
+[METHOD_ARGS]
+
+# List of qualified names (i.e., library.method) which require a timeout
+# parameter e.g. 'requests.api.get,requests.api.post'
+timeout-methods=requests.api.delete,requests.api.get,requests.api.head,requests.api.options,requests.api.patch,requests.api.post,requests.api.put,requests.api.request
+
+
+[MISCELLANEOUS]
+
+# List of note tags to take in consideration, separated by a comma.
+notes=FIXME,
+      XXX,
+      TODO
+
+# Regular expression of note tags to take in consideration.
+notes-rgx=
+
+
+[REFACTORING]
+
+# Maximum number of nested blocks for function / method body
+max-nested-blocks=5
+
+# Complete name of functions that never returns. When checking for
+# inconsistent-return-statements if a never returning function is called then
+# it will be considered as an explicit return statement and no message will be
+# printed.
+never-returning-functions=sys.exit,argparse.parse_error
+
+
+[REPORTS]
+
+# Python expression which should return a score less than or equal to 10. You
+# have access to the variables 'fatal', 'error', 'warning', 'refactor',
+# 'convention', and 'info' which contain the number of messages in each
+# category, as well as 'statement' which is the total number of statements
+# analyzed. This score is used by the global evaluation report (RP0004).
+evaluation=max(0, 0 if fatal else 10.0 - ((float(5 * error + warning + refactor + convention) / statement) * 10))
+
+# Template used to display messages. This is a python new-style format string
+# used to format the message information. See doc for all details.
+msg-template=
+
+# Set the output format. Available formats are text, parseable, colorized, json
+# and msvs (visual studio). You can also give a reporter class, e.g.
+# mypackage.mymodule.MyReporterClass.
+#output-format=
+
+# Tells whether to display a full report or only the messages.
+reports=no
+
+# Activate the evaluation score.
+# score=yes
+score=no
+
+
+[SIMILARITIES]
+
+# Comments are removed from the similarity computation
+ignore-comments=yes
+
+# Docstrings are removed from the similarity computation
+ignore-docstrings=yes
+
+# Imports are removed from the similarity computation
+ignore-imports=yes
+
+# Signatures are removed from the similarity computation
+ignore-signatures=yes
+
+# Minimum lines number of a similarity.
+min-similarity-lines=4
+
+
 [SPELLING]
 
 # Limits count of emitted suggestions for spelling mistakes.
 max-spelling-suggestions=4
 
 # Spelling dictionary name. Available dictionaries: en_AG (hunspell), en_AU
 # (hunspell), en_BS (hunspell), en_BW (hunspell), en_BZ (hunspell), en_CA
@@ -575,82 +578,102 @@
 spelling-private-dict-file=
 
 # Tells whether to store unknown words to the private dictionary (see the
 # --spelling-private-dict-file option) instead of raising a message.
 spelling-store-unknown-words=no
 
 
-[SIMILARITIES]
-
-# Comments are removed from the similarity computation
-ignore-comments=yes
-
-# Docstrings are removed from the similarity computation
-ignore-docstrings=yes
-
-# Imports are removed from the similarity computation
-ignore-imports=yes
-
-# Signatures are removed from the similarity computation
-ignore-signatures=yes
-
-# Minimum lines number of a similarity.
-min-similarity-lines=4
-
-
 [STRING]
 
 # This flag controls whether inconsistent-quotes generates a warning when the
 # character used as a quote delimiter is used inconsistently within a module.
 check-quote-consistency=no
 
 # This flag controls whether the implicit-str-concat should generate a warning
 # on implicit string concatenation in sequences defined over several lines.
 check-str-concat-over-line-jumps=no
 
 
-[IMPORTS]
+[TYPECHECK]
 
-# List of modules that can be imported at any level, not just the top level
-# one.
-allow-any-import-level=
+# List of decorators that produce context managers, such as
+# contextlib.contextmanager. Add to this list to register other decorators that
+# produce valid context managers.
+contextmanager-decorators=contextlib.contextmanager
 
-# Allow wildcard imports from modules that define __all__.
-allow-wildcard-with-all=no
+# List of members which are set dynamically and missed by pylint inference
+# system, and so shouldn't trigger E1101 when accessed. Python regular
+# expressions are accepted.
+generated-members=
 
-# Deprecated modules which should not be used, separated by a comma.
-deprecated-modules=
+# Tells whether to warn about missing members when the owner of the attribute
+# is inferred to be None.
+ignore-none=yes
 
-# Output a graph (.gv or any supported image format) of external dependencies
-# to the given file (report RP0402 must not be disabled).
-ext-import-graph=
+# This flag controls whether pylint should warn about no-member and similar
+# checks whenever an opaque object is returned when inferring. The inference
+# can return multiple potential results while evaluating a Python object, but
+# some branches might not be evaluated, which results in partial inference. In
+# that case, it might be useful to still emit no-member and other checks for
+# the rest of the inferred objects.
+ignore-on-opaque-inference=yes
 
-# Output a graph (.gv or any supported image format) of all (i.e. internal and
-# external) dependencies to the given file (report RP0402 must not be
-# disabled).
-import-graph=
+# List of symbolic message names to ignore for Mixin members.
+ignored-checks-for-mixins=no-member,
+                          not-async-context-manager,
+                          not-context-manager,
+                          attribute-defined-outside-init
 
-# Output a graph (.gv or any supported image format) of internal dependencies
-# to the given file (report RP0402 must not be disabled).
-int-import-graph=
+# List of class names for which member attributes should not be checked (useful
+# for classes with dynamically set attributes). This supports the use of
+# qualified names.
+ignored-classes=optparse.Values,thread._local,_thread._local,argparse.Namespace
 
-# Force import order to recognize a module as part of the standard
-# compatibility libraries.
-known-standard-library=
+# Show a hint with possible names when a member name was not found. The aspect
+# of finding the hint is based on edit distance.
+missing-member-hint=yes
 
-# Force import order to recognize a module as part of a third party library.
-known-third-party=enchant
+# The minimum edit distance a name should have in order to be considered a
+# similar match for a missing member name.
+missing-member-hint-distance=1
 
-# Couples of modules and preferred modules, separated by a comma.
-preferred-modules=
+# The total number of similar names that should be taken in consideration when
+# showing a hint for a missing member.
+missing-member-max-choices=1
 
+# Regex pattern to define which classes are considered mixins.
+mixin-class-rgx=.*[Mm]ixin
 
-[REFACTORING]
+# List of decorators that change the signature of a decorated function.
+signature-mutators=
 
-# Maximum number of nested blocks for function / method body
-max-nested-blocks=5
 
-# Complete name of functions that never returns. When checking for
-# inconsistent-return-statements if a never returning function is called then
-# it will be considered as an explicit return statement and no message will be
-# printed.
-never-returning-functions=sys.exit,argparse.parse_error
+[VARIABLES]
+
+# List of additional names supposed to be defined in builtins. Remember that
+# you should avoid defining new builtins when possible.
+additional-builtins=
+
+# Tells whether unused global variables should be treated as a violation.
+allow-global-unused-variables=yes
+
+# List of names allowed to shadow builtins
+allowed-redefined-builtins=
+
+# List of strings which can identify a callback function by name. A callback
+# name must start or end with one of those strings.
+callbacks=cb_,
+          _cb
+
+# A regular expression matching the name of dummy variables (i.e. expected to
+# not be used).
+dummy-variables-rgx=_+$|(_[a-zA-Z0-9_]*[a-zA-Z0-9]+?$)|dummy|^ignored_|^unused_
+
+# Argument names that match this expression will be ignored.
+ignored-argument-names=_.*|^ignored_|^unused_
+
+# Tells whether we should check for unused import in __init__ files.
+init-import=no
+
+# List of qualified module names which can have objects that can redefine
+# builtins.
+redefining-builtins-modules=six.moves,past.builtins,future.builtins,builtins,io
```

### Comparing `dtfabric-20230512/LICENSE` & `dtfabric-20230518/LICENSE`

 * *Files identical despite different names*

### Comparing `dtfabric-20230512/MANIFEST.in` & `dtfabric-20230518/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `dtfabric-20230512/PKG-INFO` & `dtfabric-20230518/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dtfabric
-Version: 20230512
+Version: 20230518
 Summary: Data type fabric (dtfabric)
 Home-page: https://github.com/libyal/dtfabric
 Maintainer: Joachim Metz
 Maintainer-email: joachim.metz@gmail.com
 License: Apache License, Version 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
```

### Comparing `dtfabric-20230512/appveyor.yml` & `dtfabric-20230518/appveyor.yml`

 * *Files identical despite different names*

### Comparing `dtfabric-20230512/config/appveyor/install.ps1` & `dtfabric-20230518/config/appveyor/install.ps1`

 * *Files identical despite different names*

### Comparing `dtfabric-20230512/config/appveyor/runtests.sh` & `dtfabric-20230518/config/appveyor/runtests.sh`

 * *Files identical despite different names*

### Comparing `dtfabric-20230512/config/dpkg/control` & `dtfabric-20230518/config/dpkg/control`

 * *Files identical despite different names*

### Comparing `dtfabric-20230512/config/dpkg/copyright` & `dtfabric-20230518/config/dpkg/copyright`

 * *Files identical despite different names*

### Comparing `dtfabric-20230512/docs/conf.py` & `dtfabric-20230518/docs/conf.py`

 * *Files identical despite different names*

### Comparing `dtfabric-20230512/docs/index.rst` & `dtfabric-20230518/docs/index.rst`

 * *Files identical despite different names*

### Comparing `dtfabric-20230512/docs/sources/Format-specification.md` & `dtfabric-20230518/docs/sources/Format-specification.md`

 * *Files identical despite different names*

### Comparing `dtfabric-20230512/docs/sources/api/dtfabric.rst` & `dtfabric-20230518/docs/sources/api/dtfabric.rst`

 * *Files identical despite different names*

### Comparing `dtfabric-20230512/docs/sources/api/dtfabric.runtime.rst` & `dtfabric-20230518/docs/sources/api/dtfabric.runtime.rst`

 * *Files identical despite different names*

### Comparing `dtfabric-20230512/docs/sources/user/Installation-instructions.md` & `dtfabric-20230518/docs/sources/user/Installation-instructions.md`

 * *Files identical despite different names*

### Comparing `dtfabric-20230512/dtfabric/data_types.py` & `dtfabric-20230518/dtfabric/data_types.py`

 * *Files identical despite different names*

### Comparing `dtfabric-20230512/dtfabric/decorators.py` & `dtfabric-20230518/dtfabric/decorators.py`

 * *Files identical despite different names*

### Comparing `dtfabric-20230512/dtfabric/definitions.py` & `dtfabric-20230518/dtfabric/definitions.py`

 * *Files identical despite different names*

### Comparing `dtfabric-20230512/dtfabric/errors.py` & `dtfabric-20230518/dtfabric/errors.py`

 * *Files identical despite different names*

### Comparing `dtfabric-20230512/dtfabric/reader.py` & `dtfabric-20230518/dtfabric/reader.py`

 * *Files 0% similar despite different names*

```diff
@@ -397,22 +397,14 @@
 
     element_data_type_definition = definitions_registry.GetDefinitionByName(
         element_data_type)
     if not element_data_type_definition:
       raise errors.DefinitionReaderError(definition_name, (
           f'undefined element data type: {element_data_type:s}'))
 
-    element_byte_size = element_data_type_definition.GetByteSize()
-    element_type_indicator = element_data_type_definition.TYPE_INDICATOR
-    if not element_byte_size and element_type_indicator != (
-        definitions.TYPE_INDICATOR_STRING):
-      raise errors.DefinitionReaderError(definition_name, (
-          f'unsupported variable size element data type: '
-          f'{element_data_type:s}'))
-
     aliases = definition_values.get('aliases', None)
     description = definition_values.get('description', None)
     urls = definition_values.get('urls', None)
 
     definition_object = data_type_definition_class(
         definition_name, element_data_type_definition, aliases=aliases,
         data_type=element_data_type, description=description, urls=urls)
```

### Comparing `dtfabric-20230512/dtfabric/registry.py` & `dtfabric-20230518/dtfabric/registry.py`

 * *Files identical despite different names*

### Comparing `dtfabric-20230512/dtfabric/runtime/byte_operations.py` & `dtfabric-20230518/dtfabric/runtime/byte_operations.py`

 * *Files identical despite different names*

### Comparing `dtfabric-20230512/dtfabric/runtime/data_maps.py` & `dtfabric-20230518/dtfabric/runtime/data_maps.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,29 +15,27 @@
 
 
 class DataTypeMapContext(object):
   """Data type map context.
 
   Attributes:
     byte_size (int): byte size.
-    members_data_size (int): members data size.
     requested_size (int): requested size.
     state (dict[str, object]): state values per name.
     values (dict[str, object]): values per name.
   """
 
   def __init__(self, values=None):
     """Initializes a data type map context.
 
     Args:
       values (dict[str, object]): values per name.
     """
     super(DataTypeMapContext, self).__init__()
     self.byte_size = None
-    self.members_data_size = None
     self.requested_size = None
     self.state = {}
     self.values = values or {}
 
 
 class DataTypeMapSizeHint(object):
   """Data type map size hint.
@@ -59,14 +57,16 @@
     self.byte_size = byte_size
     self.is_complete = is_complete
 
 
 class DataTypeMap(object):
   """Data type map."""
 
+  _MAXIMUM_RECURSION_DEPTH = 10
+
   def __init__(self, data_type_definition):
     """Initializes a data type map.
 
     Args:
       data_type_definition (DataTypeDefinition): data type definition.
 
     Raises:
@@ -234,16 +234,14 @@
           the byte stream.
     """
 
 
 class PrimitiveDataTypeMap(StorageDataTypeMap):
   """Primitive data type map."""
 
-  # pylint: disable=arguments-differ
-
   def __init__(self, data_type_definition):
     """Initializes a primitive data type map.
 
     Args:
       data_type_definition (DataTypeDefinition): data type definition.
     """
     super(PrimitiveDataTypeMap, self).__init__(data_type_definition)
@@ -301,14 +299,15 @@
       MappingError: if the data type definition cannot be mapped on
           the byte stream.
     """
     data_type_size = self._data_type_definition.GetByteSize()
     self._CheckByteStreamSize(byte_stream, byte_offset, data_type_size)
 
     if context:
+      context.byte_size = None
       context.requested_size = data_type_size
 
     try:
       struct_tuple = self._operation.ReadFrom(byte_stream[byte_offset:])
       mapped_value = self.MapValue(*struct_tuple)
 
     except Exception as exception:
@@ -525,16 +524,14 @@
     return self._FORMAT_STRINGS_SIGNED.get(
         self._data_type_definition.size, None)
 
 
 class UUIDMap(StorageDataTypeMap):
   """UUID (or GUID) data type map."""
 
-  # pylint: disable=arguments-differ
-
   def __init__(self, data_type_definition):
     """Initializes an UUID (or GUID) data type map.
 
     Args:
       data_type_definition (DataTypeDefinition): data type definition.
     """
     super(UUIDMap, self).__init__(data_type_definition)
@@ -584,14 +581,15 @@
       MappingError: if the data type definition cannot be mapped on
           the byte stream.
     """
     data_type_size = self._data_type_definition.GetByteSize()
     self._CheckByteStreamSize(byte_stream, byte_offset, data_type_size)
 
     if context:
+      context.byte_size = None
       context.requested_size = data_type_size
 
     try:
       if self._byte_order == definitions.BYTE_ORDER_BIG_ENDIAN:
         mapped_value = uuid.UUID(
             bytes=byte_stream[byte_offset:byte_offset + 16])
       elif self._byte_order == definitions.BYTE_ORDER_LITTLE_ENDIAN:
@@ -608,16 +606,14 @@
 
     return mapped_value
 
 
 class ElementSequenceDataTypeMap(StorageDataTypeMap):
   """Element sequence data type map."""
 
-  # pylint: disable=arguments-differ
-
   def __init__(self, data_type_definition):
     """Initializes a sequence data type map.
 
     Args:
       data_type_definition (DataTypeDefinition): data type definition.
     """
     super(ElementSequenceDataTypeMap, self).__init__(data_type_definition)
@@ -646,24 +642,32 @@
     Args:
       context (Optional[DataTypeMapContext]): data type map context, used to
           determine the size hint.
 
     Returns:
       int: the elements data size or None if not available.
     """
-    elements_data_size = None
+    context_state = getattr(context, 'state', {})
+
+    elements_data_size = context_state.get('elements_data_size', None)
+    if elements_data_size:
+      return elements_data_size
 
     if self._HasElementsDataSize():
       elements_data_size = self._EvaluateElementsDataSize(context)
 
     elif self._HasNumberOfElements():
       element_byte_size = self._element_data_type_definition.GetByteSize()
       if element_byte_size is not None:
-        number_of_elements = self._EvaluateNumberOfElements(context)
-        elements_data_size = number_of_elements * element_byte_size
+        number_of_elements = context_state.get('number_of_elements', None)
+        if number_of_elements is None:
+          number_of_elements = self._EvaluateNumberOfElements(context)
+
+        if number_of_elements is not None:
+          elements_data_size = number_of_elements * element_byte_size
 
     return elements_data_size
 
   def _EvaluateElementsDataSize(self, context):
     """Evaluates elements data size.
 
     Args:
@@ -845,36 +849,62 @@
     Args:
       context (Optional[DataTypeMapContext]): data type map context, used to
           determine the size hint.
 
     Returns:
       int: hint of the number of bytes needed from the byte stream or None.
     """
+    size_hint = getattr(context, 'byte_size', None)
+    if size_hint is not None:
+      return size_hint
+
     context_state = getattr(context, 'state', {})
 
-    elements_data_size = self._data_type_definition.GetByteSize()
+    elements_data_size = context_state.get('elements_data_size', None)
     if elements_data_size:
       return elements_data_size
 
-    try:
-      elements_data_size = self._CalculateElementsDataSize(context)
-    except errors.MappingError:
-      pass
-
-    if elements_data_size is None and self._HasElementsTerminator():
-      size_hints = context_state.get('size_hints', {})
-      size_hint = size_hints.get(self._data_type_definition.name, None)
-
-      elements_data_size = 0
+    if self._HasElementsDataSize():
+      elements_data_size = self._data_type_definition.GetByteSize()
+      if elements_data_size is None:
+        try:
+          elements_data_size = self._EvaluateElementsDataSize(context)
+        except errors.MappingError:
+          pass
 
-      if size_hint:
-        elements_data_size = size_hint.byte_size
+    elif self._HasElementsTerminator():
+      element_size_hint = self._element_data_type_definition.GetByteSize()
+      if element_size_hint is None:
+        subcontext = context_state.get('context', None)
+        element_size_hint = self._element_data_type_map.GetSizeHint(
+            context=subcontext)
+
+      if element_size_hint is not None:
+        elements_data_size = context_state.get('elements_data_offset', 0)
+        elements_data_size += element_size_hint
 
-      if not size_hint or not size_hint.is_complete:
-        elements_data_size += self._element_data_type_definition.GetByteSize()
+    elif self._HasNumberOfElements():
+      number_of_elements = context_state.get('number_of_elements', None)
+      if number_of_elements is None:
+        try:
+          number_of_elements = self._EvaluateNumberOfElements(context)
+        except errors.MappingError:
+          pass
+
+      if number_of_elements is not None:
+        element_byte_size = self._element_data_type_definition.GetByteSize()
+        if element_byte_size:
+          elements_data_size = number_of_elements * element_byte_size
+        else:
+          subcontext = context_state.get('context', None)
+          element_size_hint = self._element_data_type_map.GetSizeHint(
+              context=subcontext)
+          if element_size_hint is not None:
+            elements_data_size = context_state.get('elements_data_offset', 0)
+            elements_data_size += element_size_hint
 
     return elements_data_size
 
   def GetStructByteOrderString(self):
     """Retrieves the Python struct format string.
 
     Returns:
@@ -941,30 +971,35 @@
     Raises:
       FoldingError: if the data type definition cannot be folded into
           the byte stream.
     """
     # TODO: implement.
 
   def _CompositeMapByteStream(
-      self, byte_stream, byte_offset=0, context=None, **unused_kwargs):
+      self, byte_stream, byte_offset=0, context=None, recursion_depth=0,
+      **unused_kwargs):
     """Maps a sequence of composite data types on a byte stream.
 
     Args:
       byte_stream (bytes): byte stream.
       byte_offset (Optional[int]): offset into the byte stream where to start.
       context (Optional[DataTypeMapContext]): data type map context.
+      recursion_depth (Optional[int]): recursion depth.
 
     Returns:
       tuple[object, ...]: mapped values.
 
     Raises:
       ByteStreamTooSmallError: if the byte stream is too small.
       MappingError: if the data type definition cannot be mapped on
           the byte stream.
     """
+    if recursion_depth > self._MAXIMUM_RECURSION_DEPTH:
+      raise errors.MappingError('At maximum recursion depth')
+
     elements_data_size = None
     elements_terminator = None
     number_of_elements = None
 
     if self._HasElementsDataSize():
       elements_data_size = self._EvaluateElementsDataSize(context)
 
@@ -987,84 +1022,87 @@
 
     context_state = getattr(context, 'state', {})
 
     elements_data_offset = context_state.get('elements_data_offset', 0)
     element_index = context_state.get('element_index', 0)
     element_value = None
     mapped_values = context_state.get('mapped_values', [])
-    size_hints = context_state.get('size_hints', {})
     subcontext = context_state.get('context', None)
 
     if not subcontext:
       subcontext = DataTypeMapContext()
 
+    if context:
+      context.byte_size = None
+
     try:
       while byte_stream[byte_offset:]:
         if (number_of_elements is not None and
             element_index == number_of_elements):
           break
 
         if (elements_data_size is not None and
             elements_data_offset >= elements_data_size):
           break
 
         element_value = self._element_data_type_map.MapByteStream(
-            byte_stream, byte_offset=byte_offset, context=subcontext)
+            byte_stream, byte_offset=byte_offset, context=subcontext,
+            recursion_depth=recursion_depth + 1)
 
         byte_offset += subcontext.byte_size
         elements_data_offset += subcontext.byte_size
         element_index += 1
         mapped_values.append(element_value)
 
         if (elements_terminator is not None and
             element_value == elements_terminator):
           break
 
     except errors.ByteStreamTooSmallError:
       context_state['context'] = subcontext
-      context_state['elements_data_offset'] = elements_data_offset
       context_state['element_index'] = element_index
+      context_state['elements_data_offset'] = elements_data_offset
+      context_state['elements_data_size'] = elements_data_size
       context_state['mapped_values'] = mapped_values
+      context_state['number_of_elements'] = number_of_elements
 
       requested_size = byte_offset + (subcontext.requested_size or 0)
       byte_stream_size = len(byte_stream)
       raise errors.ByteStreamTooSmallError(
           f'Byte stream too small requested: {requested_size:d} available: '
           f'{byte_stream_size:d}')
 
     except Exception as exception:
       raise errors.MappingError(exception)
 
     if number_of_elements is not None and element_index != number_of_elements:
       context_state['context'] = subcontext
-      context_state['elements_data_offset'] = elements_data_offset
       context_state['element_index'] = element_index
+      context_state['elements_data_offset'] = elements_data_offset
+      context_state['elements_data_size'] = elements_data_size
       context_state['mapped_values'] = mapped_values
+      context_state['number_of_elements'] = number_of_elements
 
       error_element_index = element_index - 1
 
       raise errors.ByteStreamTooSmallError(
           f'Unable to read: {self._data_type_definition.name:s} from byte '
           f'stream at offset: {byte_offset:d} with error: missing element: '
           f'{error_element_index:d}')
 
     if (elements_terminator is not None and
         element_value != elements_terminator and (
             elements_data_size is None or
             elements_data_offset < elements_data_size)):
-      byte_stream_size = len(byte_stream)
-
-      size_hints[self._data_type_definition.name] = DataTypeMapSizeHint(
-          byte_stream_size - byte_offset)
-
       context_state['context'] = subcontext
-      context_state['elements_data_offset'] = elements_data_offset
       context_state['element_index'] = element_index
+      context_state['elements_data_offset'] = elements_data_offset
+      context_state['elements_data_size'] = elements_data_size
       context_state['mapped_values'] = mapped_values
-      context_state['size_hints'] = size_hints
+      context_state['number_of_elements'] = number_of_elements
 
       raise errors.ByteStreamTooSmallError(
           f'Unable to read: {self._data_type_definition.name:s} from byte '
           f'stream at offset: {byte_offset:d} with error: unable to find '
           f'elements terminator')
 
     if context:
@@ -1103,34 +1141,51 @@
       byte_offset (Optional[int]): offset into the byte stream where to start.
       context (Optional[DataTypeMapContext]): data type map context.
 
     Returns:
       tuple[object, ...]: mapped values.
 
     Raises:
+      ByteStreamTooSmallError: if the byte stream is too small.
       MappingError: if the data type definition cannot be mapped on
           the byte stream.
     """
+    context_state = getattr(context, 'state', {})
+
     elements_data_size = self._data_type_definition.GetByteSize()
-    self._CheckByteStreamSize(byte_stream, byte_offset, elements_data_size)
 
     if context:
+      context.byte_size = None
       context.requested_size = elements_data_size
 
     try:
+      byte_stream_size = len(byte_stream)
+
+    except Exception as exception:
+      raise errors.MappingError(exception)
+
+    if byte_stream_size - byte_offset < elements_data_size:
+      context_state['elements_data_size'] = elements_data_size
+
+      raise errors.ByteStreamTooSmallError(
+          f'Byte stream too small requested: {elements_data_size:d} '
+          f'available: {byte_stream_size:d}')
+
+    try:
       struct_tuple = self._operation.ReadFrom(byte_stream[byte_offset:])
       mapped_values = map(self._element_data_type_map.MapValue, struct_tuple)
 
     except Exception as exception:
       raise errors.MappingError(
           f'Unable to read: {self._data_type_definition.name:s} from byte '
           f'stream at offset: {byte_offset:d} with error: {exception!s}')
 
     if context:
       context.byte_size = elements_data_size
+      context.state = {}
 
     return tuple(mapped_values)
 
   def FoldByteStream(self, mapped_value, **kwargs):
     """Folds the data type into a byte stream.
 
     Args:
@@ -1188,16 +1243,14 @@
     """
     return self._map_byte_stream(byte_stream, **kwargs)
 
 
 class StreamMap(ElementSequenceDataTypeMap):
   """Stream data type map."""
 
-  # pylint: disable=arguments-differ
-
   def __init__(self, data_type_definition):
     """Initializes a stream data type map.
 
     Args:
       data_type_definition (DataTypeDefinition): data type definition.
 
     Raises:
@@ -1270,32 +1323,40 @@
     Raises:
       ByteStreamTooSmallError: if the byte stream is too small.
       MappingError: if the data type definition cannot be mapped on
           the byte stream.
     """
     context_state = getattr(context, 'state', {})
 
-    size_hints = context_state.get('size_hints', {})
-
     elements_data_size = self._CalculateElementsDataSize(context)
 
     if context:
+      context.byte_size = None
       context.requested_size = elements_data_size
 
     if elements_data_size is not None:
-      self._CheckByteStreamSize(byte_stream, byte_offset, elements_data_size)
+      try:
+        byte_stream_size = len(byte_stream)
+
+      except Exception as exception:
+        raise errors.MappingError(exception)
+
+      if byte_stream_size - byte_offset < elements_data_size:
+        context_state['elements_data_size'] = elements_data_size
+
+        raise errors.ByteStreamTooSmallError(
+            f'Byte stream too small requested: {elements_data_size:d} '
+            f'available: {byte_stream_size:d}')
 
     elif not self._HasElementsTerminator():
       raise errors.MappingError(
           'Unable to determine elements data size and missing elements '
           'terminator')
 
     else:
-      byte_stream_size = len(byte_stream)
-
       element_byte_size = self._element_data_type_definition.GetByteSize()
       elements_data_offset = byte_offset
       next_elements_data_offset = elements_data_offset + element_byte_size
 
       elements_terminator = self._data_type_definition.elements_terminator
       element_value = byte_stream[
           elements_data_offset:next_elements_data_offset]
@@ -1307,40 +1368,32 @@
           break
 
         next_elements_data_offset += element_byte_size
         element_value = byte_stream[
             elements_data_offset:next_elements_data_offset]
 
       if element_value != elements_terminator:
-        size_hints[self._data_type_definition.name] = DataTypeMapSizeHint(
-            byte_stream_size - byte_offset)
-
-        context_state['size_hints'] = size_hints
+        context_state['elements_data_offset'] = (
+            elements_data_offset - byte_offset)
 
         raise errors.ByteStreamTooSmallError(
             f'Unable to read: {self._data_type_definition.name:s} from byte '
             f'stream at offset: {byte_offset:d} with error: unable to find '
             f'elements terminator')
 
     if context:
       context.byte_size = elements_data_size
-
-      size_hints[self._data_type_definition.name] = DataTypeMapSizeHint(
-          elements_data_size, is_complete=True)
-
-      context_state['size_hints'] = size_hints
+      context.state = {}
 
     return byte_stream[byte_offset:byte_offset + elements_data_size]
 
 
 class PaddingMap(DataTypeMap):
   """Padding data type map."""
 
-  # pylint: disable=arguments-differ
-
   def _CalculatePaddingSize(self, byte_offset):
     """Calculates the padding size.
 
     Args:
       byte_offset (int): offset into the byte stream where to start.
 
     Returns:
@@ -1379,23 +1432,29 @@
       object: folded value.
 
     Raises:
       ValueError: if the data type definition cannot be folded into the value.
     """
     return value
 
-  def GetSizeHint(self, byte_offset=0, **unused_kwargs):
+  def GetSizeHint(self, byte_offset=0, context=None, **unused_kwargs):
     """Retrieves a hint about the size.
 
     Args:
       byte_offset (Optional[int]): offset into the byte stream where to start.
+      context (Optional[DataTypeMapContext]): data type map context, used to
+          determine the size hint.
 
     Returns:
       int: hint of the number of bytes needed from the byte stream or None.
     """
+    size_hint = getattr(context, 'byte_size', None)
+    if size_hint is not None:
+      return size_hint
+
     return self._CalculatePaddingSize(byte_offset)
 
   def GetStructFormatString(self):  # pylint: disable=redundant-returns-doc
     """Retrieves the Python struct format string.
 
     Returns:
       str: format string as used by Python struct or None if format string
@@ -1417,14 +1476,15 @@
 
     Raises:
       ByteStreamTooSmallError: if the byte stream is too small.
     """
     padding_size = self._CalculatePaddingSize(byte_offset)
 
     if context:
+      context.byte_size = None
       context.requested_size = padding_size
 
     byte_stream_size = len(byte_stream)
     if byte_stream_size - byte_offset < padding_size:
       raise errors.ByteStreamTooSmallError(
           f'Byte stream too small requested: {padding_size:d} available: '
           f'{byte_stream_size:d}')
@@ -1450,17 +1510,15 @@
     """
     return value
 
 
 class StringMap(StreamMap):
   """String data type map."""
 
-  # pylint: disable=arguments-differ
-
-  def FoldByteStream(self, mapped_value, **kwargs):
+  def FoldByteStream(self, mapped_value, **kwargs):  # pylint: disable=arguments-differ
     """Folds the data type into a byte stream.
 
     Args:
       mapped_value (object): mapped value.
 
     Returns:
       bytes: byte stream.
@@ -1475,25 +1533,26 @@
     except Exception as exception:
       raise errors.FoldingError(
           f'Unable to write: {self._data_type_definition.name:s} to byte '
           f'stream with error: {exception!s}')
 
     return super(StringMap, self).FoldByteStream(byte_stream, **kwargs)
 
-  def MapByteStream(self, byte_stream, byte_offset=0, **kwargs):
+  def MapByteStream(self, byte_stream, byte_offset=0, **kwargs):  # pylint: disable=arguments-differ
     """Maps the data type on a byte stream.
 
     Args:
       byte_stream (bytes): byte stream.
       byte_offset (Optional[int]): offset into the byte stream where to start.
 
     Returns:
       str: mapped values.
 
     Raises:
+      ByteStreamTooSmallError: if the byte stream is too small.
       MappingError: if the data type definition cannot be mapped on
           the byte stream.
     """
     byte_stream = super(StringMap, self).MapByteStream(
         byte_stream, byte_offset=byte_offset, **kwargs)
 
     if self._HasElementsTerminator():
@@ -1522,16 +1581,14 @@
           f'Unable to read: {self._data_type_definition.name:s} from byte '
           f'stream at offset: {byte_offset:d} with error: {exception!s}')
 
 
 class StructureMap(StorageDataTypeMap):
   """Structure data type map."""
 
-  # pylint: disable=arguments-differ
-
   def __init__(self, data_type_definition):
     """Initializes a structure data type map.
 
     Args:
       data_type_definition (DataTypeDefinition): data type definition.
     """
     super(StructureMap, self).__init__(data_type_definition)
@@ -1638,30 +1695,35 @@
 
     if context:
       context.state = {}
 
     return b''.join(data_attributes)
 
   def _CompositeMapByteStream(
-      self, byte_stream, byte_offset=0, context=None, **unused_kwargs):
+      self, byte_stream, byte_offset=0, context=None, recursion_depth=0,
+      **unused_kwargs):
     """Maps a sequence of composite data types on a byte stream.
 
     Args:
       byte_stream (bytes): byte stream.
       byte_offset (Optional[int]): offset into the byte stream where to start.
       context (Optional[DataTypeMapContext]): data type map context.
+      recursion_depth (Optional[int]): recursion depth.
 
     Returns:
       object: mapped value.
 
     Raises:
       ByteStreamTooSmallError: if the byte stream is too small.
       MappingError: if the data type definition cannot be mapped on
           the byte stream.
     """
+    if recursion_depth > self._MAXIMUM_RECURSION_DEPTH:
+      raise errors.MappingError('At maximum recursion depth')
+
     context_state = getattr(context, 'state', {})
     context_values = getattr(context, 'values', {})
 
     attribute_index = context_state.get('attribute_index', 0)
     mapped_values = context_state.get('mapped_values', None)
     subcontext = context_state.get('context', None)
 
@@ -1669,14 +1731,17 @@
       mapped_values = self._structure_values_class()
     if not subcontext:
       subcontext_values = {type(mapped_values).__name__: mapped_values}
       # Pass externally defined values.
       subcontext_values.update(context_values)
       subcontext = DataTypeMapContext(values=subcontext_values)
 
+    if context:
+      context.byte_size = None
+
     members_data_size = 0
 
     for attribute_index in range(attribute_index, self._number_of_attributes):
       attribute_name = self._attribute_names[attribute_index]
       data_type_map = self._data_type_maps[attribute_index]
       member_definition = self._data_type_definition.members[attribute_index]
 
@@ -1698,24 +1763,23 @@
               'Condition does not result in a boolean value')
 
         if not condition_result:
           continue
 
       try:
         value = data_type_map.MapByteStream(
-            byte_stream, byte_offset=byte_offset, context=subcontext)
+            byte_stream, byte_offset=byte_offset, context=subcontext,
+            recursion_depth=recursion_depth + 1)
         setattr(mapped_values, attribute_name, value)
 
       except errors.ByteStreamTooSmallError:
         context_state['attribute_index'] = attribute_index
         context_state['context'] = subcontext
         context_state['mapped_values'] = mapped_values
-
-        if context:
-          context.members_data_size = members_data_size
+        context_state['members_data_size'] = members_data_size
 
         requested_size = byte_offset + (subcontext.requested_size or 0)
         byte_stream_size = len(byte_stream)
 
         raise errors.ByteStreamTooSmallError(
             f'Byte stream too small requested: {requested_size:d} available: '
             f'{byte_stream_size:d}')
@@ -1734,17 +1798,15 @@
       byte_offset += subcontext.byte_size
       members_data_size += subcontext.byte_size
 
     if attribute_index != (self._number_of_attributes - 1):
       context_state['attribute_index'] = attribute_index
       context_state['context'] = subcontext
       context_state['mapped_values'] = mapped_values
-
-      if context:
-        context.members_data_size = members_data_size
+      context_state['members_data_size'] = members_data_size
 
       raise errors.ByteStreamTooSmallError(
           f'Unable to read: {self._data_type_definition.name:s} from byte '
           f'stream at offset: {byte_offset:d} with error: missing attribute: '
           f'{attribute_index:d}')
 
     if context:
@@ -1843,19 +1905,39 @@
       byte_offset (Optional[int]): offset into the byte stream where to start.
       context (Optional[DataTypeMapContext]): data type map context.
 
     Returns:
       object: mapped value.
 
     Raises:
+      ByteStreamTooSmallError: if the byte stream is too small.
       MappingError: if the data type definition cannot be mapped on
           the byte stream.
     """
     members_data_size = self._data_type_definition.GetByteSize()
-    self._CheckByteStreamSize(byte_stream, byte_offset, members_data_size)
+
+    context_state = getattr(context, 'state', {})
+
+    if context:
+      context.byte_size = None
+      context.requested_size = members_data_size
+
+    try:
+      byte_stream_size = len(byte_stream)
+
+    except Exception as exception:
+      raise errors.MappingError(exception)
+
+    if byte_stream_size - byte_offset < members_data_size:
+      context_state['attribute_index'] = self._number_of_attributes
+      context_state['members_data_size'] = members_data_size
+
+      raise errors.ByteStreamTooSmallError(
+          f'Byte stream too small requested: {members_data_size:d} available: '
+          f'{byte_stream_size:d}')
 
     try:
       struct_tuple = self._operation.ReadFrom(byte_stream[byte_offset:])
       struct_values = []
       for attribute_index, value in enumerate(struct_tuple):
         data_type_map = self._data_type_maps[attribute_index]
         member_definition = self._data_type_definition.members[attribute_index]
@@ -1877,14 +1959,15 @@
     except Exception as exception:
       raise errors.MappingError(
           f'Unable to read: {self._data_type_definition.name:s} from byte '
           f'stream at offset: {byte_offset:d} with error: {exception!s}')
 
     if context:
       context.byte_size = members_data_size
+      context.state = {}
 
     return mapped_value
 
   def CreateStructureValues(self, *args, **kwargs):
     """Creates a structure values object.
 
     Returns:
@@ -1913,36 +1996,44 @@
     Args:
       context (Optional[DataTypeMapContext]): data type map context, used to
           determine the size hint.
 
     Returns:
       int: hint of the number of bytes needed from the byte stream or None.
     """
+    size_hint = getattr(context, 'byte_size', None)
+    if size_hint is not None:
+      return size_hint
+
     context_state = getattr(context, 'state', {})
 
     attribute_index = context_state.get('attribute_index', 0)
     mapped_values = context_state.get('mapped_values', None)
     subcontext = context_state.get('context', None)
 
     if not mapped_values:
       mapped_values = self._structure_values_class()
     if not subcontext:
       subcontext_values = {type(mapped_values).__name__: mapped_values}
       subcontext = DataTypeMapContext(values=subcontext_values)
 
-    size_hint = getattr(context, 'members_data_size', None) or 0
+    size_hint = context_state.get('members_data_size', 0)
     for attribute_index in range(attribute_index, self._number_of_attributes):
       data_type_map = self._data_type_maps[attribute_index]
-      data_type_size = data_type_map.GetSizeHint(
+      attribute_size_hint = data_type_map.GetSizeHint(
           byte_offset=size_hint, context=subcontext)
 
-      if data_type_size is None:
+      if attribute_size_hint is None:
         break
 
-      size_hint += data_type_size
+      size_hint += attribute_size_hint
+
+      # A new subcontext is created to prevent the current state affecting
+      # the size hint calculation of subsequent attributes.
+      subcontext = DataTypeMapContext()
 
     return size_hint
 
   def GetStructFormatString(self):
     """Retrieves the Python struct format string.
 
     Returns:
@@ -2178,54 +2269,64 @@
     This method is deprecated use GetSizeHint instead.
 
     Returns:
       int: data type size in bytes or None if size cannot be determined.
     """
     return None
 
-  def GetSizeHint(self, context=None, **kwargs):  # pylint: disable=arguments-differ
+  def GetSizeHint(self, context=None, **kwargs):
     """Retrieves a hint about the size.
 
     Args:
       context (Optional[DataTypeMapContext]): data type map context, used to
           determine the size hint.
 
     Returns:
       int: hint of the number of bytes needed from the byte stream or None.
     """
+    size_hint = getattr(context, 'byte_size', None)
+    if size_hint is not None:
+      return size_hint
+
     context_state = getattr(context, 'state', {})
 
     member_identifier = context_state.get('member_identifier', None)
+    subcontext = context_state.get('context', None)
+
+    if not subcontext:
+      subcontext = DataTypeMapContext()
 
     member_data_type_map = self._data_type_maps.get(member_identifier, None)
-    if not member_data_type_map:
-      return self._base_data_type_map.GetSizeHint(context=context, **kwargs)
+    if member_data_type_map:
+      return member_data_type_map.GetSizeHint(context=subcontext, **kwargs)
 
-    return member_data_type_map.GetSizeHint(context=context, **kwargs)
+    return self._base_data_type_map.GetSizeHint(context=subcontext, **kwargs)
 
-  def MapByteStream(self, byte_stream, context=None, **kwargs):  # pylint: disable=arguments-differ
+  def MapByteStream(self, byte_stream, context=None, **kwargs):
     """Maps the data type on a byte stream.
 
     Args:
       byte_stream (bytes): byte stream.
       context (Optional[DataTypeMapContext]): data type map context.
 
     Returns:
       object: mapped value.
 
     Raises:
+      ByteStreamTooSmallError: if the byte stream is too small.
       MappingError: if the data type definition cannot be mapped on
           the byte stream.
     """
     context_state = getattr(context, 'state', {})
 
     member_identifier = context_state.get('member_identifier', None)
     if member_identifier is None:
+      subcontext = DataTypeMapContext()
       mapped_base_value = self._base_data_type_map.MapByteStream(
-          byte_stream, context=context, **kwargs)
+          byte_stream, context=subcontext, **kwargs)
 
       member_identifier = getattr(
           mapped_base_value, self._data_type_definition.identifier, None)
       if member_identifier is None:
         raise errors.MappingError(
             f'Unable to determine value of '
             f'{self._data_type_definition.identifier:s}')
@@ -2235,16 +2336,38 @@
     member_data_type_map = self._data_type_maps.get(member_identifier, None)
     if member_data_type_map is None:
       raise errors.MappingError(
           f'Missing member data type map for '
           f'{self._data_type_definition.identifier:s}: '
           f'{member_identifier!s}')
 
-    return member_data_type_map.MapByteStream(
-        byte_stream, context=context, **kwargs)
+    subcontext = context_state.get('context', None)
+
+    if not subcontext:
+      subcontext = DataTypeMapContext()
+
+    if context:
+      context.byte_size = None
+
+    try:
+      value = member_data_type_map.MapByteStream(
+          byte_stream, context=subcontext, **kwargs)
+
+    except errors.ByteStreamTooSmallError as exception:
+      context_state['context'] = subcontext
+      raise exception
+
+    except Exception as exception:
+      raise errors.MappingError(exception)
+
+    if context:
+      context.byte_size = subcontext.byte_size
+      context.state = {}
+
+    return value
 
 
 class DataTypeMapFactory(object):
   """Factory for data type maps."""
 
   # TODO: add support for definitions.TYPE_INDICATOR_FORMAT
   # TODO: add support for definitions.TYPE_INDICATOR_STRUCTURE_FAMILY
```

### Comparing `dtfabric-20230512/dtfabric/runtime/fabric.py` & `dtfabric-20230518/dtfabric/runtime/fabric.py`

 * *Files identical despite different names*

### Comparing `dtfabric-20230512/dtfabric/runtime/runtime.py` & `dtfabric-20230518/dtfabric/runtime/runtime.py`

 * *Files identical despite different names*

### Comparing `dtfabric-20230512/dtfabric.egg-info/PKG-INFO` & `dtfabric-20230518/dtfabric.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dtfabric
-Version: 20230512
+Version: 20230518
 Summary: Data type fabric (dtfabric)
 Home-page: https://github.com/libyal/dtfabric
 Maintainer: Joachim Metz
 Maintainer-email: joachim.metz@gmail.com
 License: Apache License, Version 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
```

### Comparing `dtfabric-20230512/dtfabric.egg-info/SOURCES.txt` & `dtfabric-20230518/dtfabric.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -56,14 +56,15 @@
 dtfabric.egg-info/top_level.txt
 dtfabric/runtime/__init__.py
 dtfabric/runtime/byte_operations.py
 dtfabric/runtime/data_maps.py
 dtfabric/runtime/fabric.py
 dtfabric/runtime/runtime.py
 scripts/validate-definitions.py
+test_data/.structure_with_string.yaml.swp
 test_data/Notepad.lnk
 test_data/boolean.yaml
 test_data/character.yaml
 test_data/constant.yaml
 test_data/enumeration.yaml
 test_data/floating-point.yaml
 test_data/format.yaml
```

### Comparing `dtfabric-20230512/run_tests.py` & `dtfabric-20230518/run_tests.py`

 * *Files identical despite different names*

### Comparing `dtfabric-20230512/scripts/validate-definitions.py` & `dtfabric-20230518/scripts/validate-definitions.py`

 * *Files identical despite different names*

### Comparing `dtfabric-20230512/setup.py` & `dtfabric-20230518/setup.py`

 * *Files identical despite different names*

### Comparing `dtfabric-20230512/test_data/Notepad.lnk` & `dtfabric-20230518/test_data/Notepad.lnk`

 * *Files identical despite different names*

### Comparing `dtfabric-20230512/test_data/definitions/booleans.yaml` & `dtfabric-20230518/test_data/definitions/booleans.yaml`

 * *Files identical despite different names*

### Comparing `dtfabric-20230512/test_data/definitions/integers.yaml` & `dtfabric-20230518/test_data/definitions/integers.yaml`

 * *Files identical despite different names*

### Comparing `dtfabric-20230512/test_data/enumeration.yaml` & `dtfabric-20230518/test_data/enumeration.yaml`

 * *Files identical despite different names*

### Comparing `dtfabric-20230512/test_data/format.yaml` & `dtfabric-20230518/test_data/format.yaml`

 * *Files identical despite different names*

### Comparing `dtfabric-20230512/test_data/sequence_with_context.yaml` & `dtfabric-20230518/test_data/sequence_with_context.yaml`

 * *Files identical despite different names*

### Comparing `dtfabric-20230512/test_data/stream.yaml` & `dtfabric-20230518/test_data/stream.yaml`

 * *Files identical despite different names*

### Comparing `dtfabric-20230512/test_data/string.yaml` & `dtfabric-20230518/test_data/string.yaml`

 * *Files identical despite different names*

### Comparing `dtfabric-20230512/test_data/string_array.yaml` & `dtfabric-20230518/test_data/string_array.yaml`

 * *Files identical despite different names*

### Comparing `dtfabric-20230512/test_data/structure.yaml` & `dtfabric-20230518/test_data/structure.yaml`

 * *Files identical despite different names*

### Comparing `dtfabric-20230512/test_data/structure_family.yaml` & `dtfabric-20230518/test_data/structure_family.yaml`

 * *Files identical despite different names*

### Comparing `dtfabric-20230512/test_data/structure_group.yaml` & `dtfabric-20230518/test_data/structure_group.yaml`

 * *Files identical despite different names*

### Comparing `dtfabric-20230512/test_data/structure_with_condition.yaml` & `dtfabric-20230518/test_data/structure_with_condition.yaml`

 * *Files identical despite different names*

### Comparing `dtfabric-20230512/test_data/structure_with_padding.yaml` & `dtfabric-20230518/test_data/structure_with_padding.yaml`

 * *Files identical despite different names*

### Comparing `dtfabric-20230512/test_data/structure_with_values.yaml` & `dtfabric-20230518/test_data/structure_with_values.yaml`

 * *Files identical despite different names*

### Comparing `dtfabric-20230512/tests/data_types.py` & `dtfabric-20230518/tests/data_types.py`

 * *Files identical despite different names*

### Comparing `dtfabric-20230512/tests/reader.py` & `dtfabric-20230518/tests/reader.py`

 * *Files 1% similar despite different names*

```diff
@@ -1085,17 +1085,21 @@
 
     definitions_registry = registry.DataTypeDefinitionsRegistry()
     definitions_reader = reader.YAMLDataTypeDefinitionsFileReader()
 
     definitions_file = self._GetTestFilePath(['sequence_with_structure.yaml'])
     self._SkipIfPathNotExists(definitions_file)
 
-    with self.assertRaises(errors.FormatError):
-      with open(definitions_file, 'rb') as file_object:
-        definitions_reader.ReadFileObject(definitions_registry, file_object)
+    with open(definitions_file, 'rb') as file_object:
+      definitions_reader.ReadFileObject(definitions_registry, file_object)
+
+    self.assertEqual(len(definitions_registry._definitions), 3)
+
+    data_type_definition = definitions_registry.GetDefinitionByName('vectors')
+    self.assertIsInstance(data_type_definition, data_types.SequenceDefinition)
 
   def testReadFileObjectStream(self):
     """Tests the ReadFileObject function of a stream data type."""
     definitions_registry = registry.DataTypeDefinitionsRegistry()
     definitions_reader = reader.YAMLDataTypeDefinitionsFileReader()
 
     definitions_file = self._GetTestFilePath(['stream.yaml'])
```

### Comparing `dtfabric-20230512/tests/registry.py` & `dtfabric-20230518/tests/registry.py`

 * *Files identical despite different names*

### Comparing `dtfabric-20230512/tests/runtime/byte_operations.py` & `dtfabric-20230518/tests/runtime/byte_operations.py`

 * *Files identical despite different names*

### Comparing `dtfabric-20230512/tests/runtime/data_maps.py` & `dtfabric-20230518/tests/runtime/data_maps.py`

 * *Files 1% similar despite different names*

```diff
@@ -66,14 +66,15 @@
         definitions_file)
     data_type_definition = definitions_registry.GetDefinitionByName('int32le')
 
     data_type_map = data_maps.DataTypeMap(data_type_definition)
 
     self.assertEqual(data_type_map.name, 'int32le')
 
+  # TODO: remove GetByteSize is deprecated.
   def testGetByteSize(self):
     """Tests the GetByteSize function."""
     definitions_file = self._GetTestFilePath(['integer.yaml'])
     definitions_registry = self._CreateDefinitionRegistryFromFile(
         definitions_file)
     data_type_definition = definitions_registry.GetDefinitionByName('int32le')
 
@@ -854,14 +855,24 @@
 
     data_type_definition = definitions_registry.GetDefinitionByName('vector4')
     data_type_map = data_maps.ElementSequenceDataTypeMap(data_type_definition)
 
     size_hint = data_type_map.GetSizeHint()
     self.assertEqual(size_hint, 16)
 
+    definitions_file = self._GetTestFilePath(['sequence_with_structure.yaml'])
+    definitions_registry = self._CreateDefinitionRegistryFromFile(
+        definitions_file)
+
+    data_type_definition = definitions_registry.GetDefinitionByName('vectors')
+    data_type_map = data_maps.ElementSequenceDataTypeMap(data_type_definition)
+
+    size_hint = data_type_map.GetSizeHint()
+    self.assertEqual(size_hint, 4)
+
   def testGetStructByteOrderString(self):
     """Tests the GetStructByteOrderString function."""
     definitions_file = self._GetTestFilePath(['sequence.yaml'])
     definitions_registry = self._CreateDefinitionRegistryFromFile(
         definitions_file)
 
     data_type_definition = definitions_registry.GetDefinitionByName('vector4')
@@ -905,14 +916,17 @@
     sequence_value = data_type_map._CompositeMapByteStream(byte_stream)
     self.assertEqual(
         sequence_value, ((1, 2, 3, 4), (5, 6, 7, 8), (9, 10, 11, 12)))
 
     with self.assertRaises(errors.MappingError):
       data_type_map._CompositeMapByteStream(None)
 
+    with self.assertRaises(errors.MappingError):
+      data_type_map._CompositeMapByteStream(byte_stream, recursion_depth=999)
+
     with self.assertRaises(errors.ByteStreamTooSmallError):
       data_type_map._CompositeMapByteStream(b'\x12\x34\x56')
 
   def testLinearFoldByteStream(self):
     """Tests the _LinearFoldByteStream function."""
     definitions_file = self._GetTestFilePath(['sequence.yaml'])
     definitions_registry = self._CreateDefinitionRegistryFromFile(
@@ -1255,14 +1269,17 @@
     byte_stream = b''.join([
         bytes(bytearray([len(text_stream), 0])), text_stream])
 
     utf16_string = data_type_map._CompositeMapByteStream(byte_stream)
     self.assertEqual(utf16_string.size, len(text_stream))
     self.assertEqual(utf16_string.text, 'dtFabric')
 
+    with self.assertRaises(errors.MappingError):
+      data_type_map._CompositeMapByteStream(byte_stream, recursion_depth=999)
+
     byte_stream = b''.join([bytes(bytearray([3, 0])), text_stream])
 
     with self.assertRaises(errors.MappingError):
       data_type_map._CompositeMapByteStream(byte_stream)
 
     definitions_file = self._GetTestFilePath(['structure_with_context.yaml'])
     definitions_registry = self._CreateDefinitionRegistryFromFile(
@@ -1999,28 +2016,40 @@
     test_definition2.values = None
 
     data_type_map._data_type_maps = None
 
     with self.assertRaises(errors.FormatError):
       data_type_map._GetMemberDataTypeMaps(data_type_definition)
 
+  # TODO: remove GetByteSize is deprecated.
   def testGetByteSize(self):
     """Tests the GetByteSize function."""
     definitions_file = self._GetTestFilePath(['structure_group.yaml'])
     definitions_registry = self._CreateDefinitionRegistryFromFile(
         definitions_file)
 
     data_type_definition = definitions_registry.GetDefinitionByName(
         'bsm_token')
     data_type_map = data_maps.StructureGroupMap(data_type_definition)
 
     byte_size = data_type_map.GetByteSize()
     self.assertIsNone(byte_size)
 
-  # TODO: add tests for GetSizeHint.
+  def testGetSizeHint(self):
+    """Tests the GetSizeHint function."""
+    definitions_file = self._GetTestFilePath(['structure_group.yaml'])
+    definitions_registry = self._CreateDefinitionRegistryFromFile(
+        definitions_file)
+
+    data_type_definition = definitions_registry.GetDefinitionByName(
+        'bsm_token')
+    data_type_map = data_maps.StructureGroupMap(data_type_definition)
+
+    size_hint = data_type_map.GetSizeHint()
+    self.assertEqual(size_hint, 1)
 
   def testMapByteStream(self):
     """Tests the MapByteStream function."""
     definitions_file = self._GetTestFilePath(['structure_group.yaml'])
     definitions_registry = self._CreateDefinitionRegistryFromFile(
         definitions_file)
```

### Comparing `dtfabric-20230512/tests/runtime/fabric.py` & `dtfabric-20230518/tests/runtime/fabric.py`

 * *Files identical despite different names*

### Comparing `dtfabric-20230512/tests/runtime/runtime.py` & `dtfabric-20230518/tests/runtime/runtime.py`

 * *Files identical despite different names*

### Comparing `dtfabric-20230512/tests/test_lib.py` & `dtfabric-20230518/tests/test_lib.py`

 * *Files identical despite different names*

### Comparing `dtfabric-20230512/tox.ini` & `dtfabric-20230518/tox.ini`

 * *Files 0% similar despite different names*

```diff
@@ -36,15 +36,15 @@
     CPPFLAGS
     LDFLAGS
 setenv =
     PYTHONPATH = {toxinidir}
 deps =
     -rrequirements.txt
     -rtest_requirements.txt
-    pylint >= 2.14.0, < 2.15.0
+    pylint >= 2.17.0, < 2.18.0
     yamllint >= 1.26.0
 commands =
     pylint --version
     yamllint -v
     # Ignore setup.py for now due to:
     # setup.py:15:0: E0001: Cannot import 'distutils.command.bdist_msi' due to
     # syntax error 'expected an indented block (<unknown>, line 347)' (syntax-error)
```

### Comparing `dtfabric-20230512/utils/dependencies.py` & `dtfabric-20230518/utils/dependencies.py`

 * *Files identical despite different names*

### Comparing `dtfabric-20230512/utils/update_release.sh` & `dtfabric-20230518/utils/update_release.sh`

 * *Files identical despite different names*

