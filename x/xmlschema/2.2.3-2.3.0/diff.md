# Comparing `tmp/xmlschema-2.2.3.tar.gz` & `tmp/xmlschema-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xmlschema-2.2.3.tar", last modified: Fri Apr 14 13:52:42 2023, max compression
+gzip compressed data, was "xmlschema-2.3.0.tar", last modified: Thu May 18 20:19:54 2023, max compression
```

## Comparing `xmlschema-2.2.3.tar` & `xmlschema-2.3.0.tar`

### file list

```diff
@@ -1,490 +1,493 @@
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-04-14 13:52:42.466140 xmlschema-2.2.3/
--rw-r--r--   0 brunato   (1000) brunato   (1000)      235 2023-03-05 21:16:57.000000 xmlschema-2.2.3/.coveragerc
--rw-r--r--   0 brunato   (1000) brunato   (1000)    24835 2023-04-14 13:49:05.000000 xmlschema-2.2.3/CHANGELOG.rst
--rw-r--r--   0 brunato   (1000) brunato   (1000)     1131 2022-09-26 10:47:27.000000 xmlschema-2.2.3/LICENSE
--rw-r--r--   0 brunato   (1000) brunato   (1000)      330 2023-03-05 20:30:24.000000 xmlschema-2.2.3/MANIFEST.in
--rw-r--r--   0 brunato   (1000) brunato   (1000)     7377 2023-04-14 13:52:42.466140 xmlschema-2.2.3/PKG-INFO
--rw-r--r--   0 brunato   (1000) brunato   (1000)     6045 2022-08-26 15:33:28.000000 xmlschema-2.2.3/README.rst
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-04-14 13:52:42.390139 xmlschema-2.2.3/doc/
--rw-r--r--   0 brunato   (1000) brunato   (1000)      606 2018-09-23 09:23:56.000000 xmlschema-2.2.3/doc/Makefile
--rw-r--r--   0 brunato   (1000) brunato   (1000)    11613 2022-10-01 13:42:01.000000 xmlschema-2.2.3/doc/api.rst
--rw-rw-r--   0 brunato   (1000) brunato   (1000)    11273 2021-08-02 14:12:17.000000 xmlschema-2.2.3/doc/components.rst
--rw-r--r--   0 brunato   (1000) brunato   (1000)     5474 2023-04-14 13:49:05.000000 xmlschema-2.2.3/doc/conf.py
--rw-rw-r--   0 brunato   (1000) brunato   (1000)     5499 2022-06-24 14:13:22.000000 xmlschema-2.2.3/doc/converters.rst
--rw-rw-r--   0 brunato   (1000) brunato   (1000)     4841 2022-06-24 14:13:22.000000 xmlschema-2.2.3/doc/extras.rst
--rw-rw-r--   0 brunato   (1000) brunato   (1000)     7488 2022-06-24 14:13:22.000000 xmlschema-2.2.3/doc/features.rst
--rw-r--r--   0 brunato   (1000) brunato   (1000)      214 2021-02-05 09:05:33.000000 xmlschema-2.2.3/doc/index.rst
--rw-r--r--   0 brunato   (1000) brunato   (1000)      468 2020-05-28 20:30:12.000000 xmlschema-2.2.3/doc/intro.rst
--rw-r--r--   0 brunato   (1000) brunato   (1000)     5921 2021-04-11 20:19:21.000000 xmlschema-2.2.3/doc/testing.rst
--rw-r--r--   0 brunato   (1000) brunato   (1000)    27730 2022-10-01 13:42:01.000000 xmlschema-2.2.3/doc/usage.rst
--rw-rw-r--   0 brunato   (1000) brunato   (1000)       31 2022-03-07 13:26:41.000000 xmlschema-2.2.3/mypy.ini
--rw-r--r--   0 brunato   (1000) brunato   (1000)      214 2023-02-06 06:20:42.000000 xmlschema-2.2.3/requirements-dev.txt
--rw-r--r--   0 brunato   (1000) brunato   (1000)       38 2023-04-14 13:52:42.466140 xmlschema-2.2.3/setup.cfg
--rwxr-xr-x   0 brunato   (1000) brunato   (1000)     2764 2023-04-14 13:49:05.000000 xmlschema-2.2.3/setup.py
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-04-14 13:52:42.394140 xmlschema-2.2.3/tests/
--rw-r--r--   0 brunato   (1000) brunato   (1000)        0 2020-12-03 21:49:59.000000 xmlschema-2.2.3/tests/__init__.py
--rwxrwxr-x   0 brunato   (1000) brunato   (1000)     4934 2022-07-18 14:19:15.000000 xmlschema-2.2.3/tests/check_memory.py
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-04-14 13:52:42.377139 xmlschema-2.2.3/tests/templates/
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-04-14 13:52:42.395140 xmlschema-2.2.3/tests/templates/demo/
--rw-r--r--   0 brunato   (1000) brunato   (1000)       39 2021-02-05 09:05:33.000000 xmlschema-2.2.3/tests/templates/demo/demo_type_filter_test.jinja
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-04-14 13:52:42.396139 xmlschema-2.2.3/tests/templates/filters/
--rw-r--r--   0 brunato   (1000) brunato   (1000)       34 2021-02-05 09:05:33.000000 xmlschema-2.2.3/tests/templates/filters/name_filter_test.jinja
--rw-r--r--   0 brunato   (1000) brunato   (1000)       39 2021-02-05 09:05:33.000000 xmlschema-2.2.3/tests/templates/filters/namespace_filter_test.jinja
--rw-r--r--   0 brunato   (1000) brunato   (1000)       42 2021-02-05 09:05:33.000000 xmlschema-2.2.3/tests/templates/filters/python_type_filter_test.jinja
--rw-r--r--   0 brunato   (1000) brunato   (1000)       35 2021-02-05 09:05:33.000000 xmlschema-2.2.3/tests/templates/filters/qname_filter_test.jinja
--rw-r--r--   0 brunato   (1000) brunato   (1000)       87 2021-02-05 09:05:33.000000 xmlschema-2.2.3/tests/templates/filters/sort_types_filter_test.jinja
--rw-r--r--   0 brunato   (1000) brunato   (1000)       39 2021-04-03 19:09:14.000000 xmlschema-2.2.3/tests/templates/filters/type_name_filter_test.jinja
--rw-r--r--   0 brunato   (1000) brunato   (1000)       40 2021-02-05 09:05:33.000000 xmlschema-2.2.3/tests/templates/filters/type_qname_filter_test.jinja
--rw-r--r--   0 brunato   (1000) brunato   (1000)       37 2021-04-05 21:38:16.000000 xmlschema-2.2.3/tests/templates/filters/unknown_filter_test.jinja
--rw-r--r--   0 brunato   (1000) brunato   (1000)       42 2021-02-05 09:05:33.000000 xmlschema-2.2.3/tests/templates/filters/wrong-template.jinja
--rw-rw-r--   0 brunato   (1000) brunato   (1000)     3484 2022-07-18 14:19:15.000000 xmlschema-2.2.3/tests/test_all.py
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-04-14 13:52:42.396139 xmlschema-2.2.3/tests/test_cases/
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-04-14 13:52:42.377139 xmlschema-2.2.3/tests/test_cases/examples/
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-04-14 13:52:42.399140 xmlschema-2.2.3/tests/test_cases/examples/collection/
--rw-r--r--   0 brunato   (1000) brunato   (1000)      925 2020-05-28 20:30:12.000000 xmlschema-2.2.3/tests/test_cases/examples/collection/collection-1_error.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      884 2022-08-26 15:33:28.000000 xmlschema-2.2.3/tests/test_cases/examples/collection/collection-default.xml
--rw-rw-r--   0 brunato   (1000) brunato   (1000)      798 2023-04-14 13:51:59.000000 xmlschema-2.2.3/tests/test_cases/examples/collection/collection.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)      923 2020-05-28 20:30:12.000000 xmlschema-2.2.3/tests/test_cases/examples/collection/collection.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)     1599 2020-01-23 20:05:17.000000 xmlschema-2.2.3/tests/test_cases/examples/collection/collection.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      941 2020-01-23 20:05:17.000000 xmlschema-2.2.3/tests/test_cases/examples/collection/collection2.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)     1736 2020-01-23 20:05:17.000000 xmlschema-2.2.3/tests/test_cases/examples/collection/collection2.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      960 2020-01-23 20:05:17.000000 xmlschema-2.2.3/tests/test_cases/examples/collection/collection3.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)     1938 2020-01-23 20:05:17.000000 xmlschema-2.2.3/tests/test_cases/examples/collection/collection3.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)     1082 2020-01-23 20:05:17.000000 xmlschema-2.2.3/tests/test_cases/examples/collection/collection3bis.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)     1979 2020-01-23 20:05:17.000000 xmlschema-2.2.3/tests/test_cases/examples/collection/collection3bis.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)     1364 2020-01-23 20:05:17.000000 xmlschema-2.2.3/tests/test_cases/examples/collection/collection4.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)     1743 2020-11-08 22:15:33.000000 xmlschema-2.2.3/tests/test_cases/examples/collection/collection4.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)     1658 2022-08-26 15:33:28.000000 xmlschema-2.2.3/tests/test_cases/examples/collection/collection5.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-04-14 13:52:42.399140 xmlschema-2.2.3/tests/test_cases/examples/stockquote/
--rw-r--r--   0 brunato   (1000) brunato   (1000)     1039 2020-11-08 22:15:33.000000 xmlschema-2.2.3/tests/test_cases/examples/stockquote/stockquote.wsdl
--rw-r--r--   0 brunato   (1000) brunato   (1000)      664 2020-11-08 22:15:33.000000 xmlschema-2.2.3/tests/test_cases/examples/stockquote/stockquote.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)     1230 2020-11-08 22:15:33.000000 xmlschema-2.2.3/tests/test_cases/examples/stockquote/stockquoteservice.wsdl
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-04-14 13:52:42.402140 xmlschema-2.2.3/tests/test_cases/examples/vehicles/
--rw-r--r--   0 brunato   (1000) brunato   (1000)      471 2020-01-23 20:05:17.000000 xmlschema-2.2.3/tests/test_cases/examples/vehicles/bikes.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      469 2020-01-23 20:05:17.000000 xmlschema-2.2.3/tests/test_cases/examples/vehicles/cars.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      595 2022-10-01 13:42:01.000000 xmlschema-2.2.3/tests/test_cases/examples/vehicles/invalid.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      361 2020-01-23 20:05:17.000000 xmlschema-2.2.3/tests/test_cases/examples/vehicles/types.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      386 2020-05-02 09:28:30.000000 xmlschema-2.2.3/tests/test_cases/examples/vehicles/vehicles-1_error.json
--rw-r--r--   0 brunato   (1000) brunato   (1000)      468 2020-01-23 20:05:17.000000 xmlschema-2.2.3/tests/test_cases/examples/vehicles/vehicles-1_error.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      475 2020-01-23 20:05:17.000000 xmlschema-2.2.3/tests/test_cases/examples/vehicles/vehicles-2_errors.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      386 2020-05-02 09:28:33.000000 xmlschema-2.2.3/tests/test_cases/examples/vehicles/vehicles-3_errors.json
--rw-r--r--   0 brunato   (1000) brunato   (1000)      491 2020-01-23 20:05:17.000000 xmlschema-2.2.3/tests/test_cases/examples/vehicles/vehicles-3_errors.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      557 2020-01-23 20:05:17.000000 xmlschema-2.2.3/tests/test_cases/examples/vehicles/vehicles-max.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)     1666 2020-11-15 16:10:20.000000 xmlschema-2.2.3/tests/test_cases/examples/vehicles/vehicles-schemas.xsd.zip
--rw-r--r--   0 brunato   (1000) brunato   (1000)      497 2020-01-23 20:05:17.000000 xmlschema-2.2.3/tests/test_cases/examples/vehicles/vehicles.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      543 2020-01-23 20:05:17.000000 xmlschema-2.2.3/tests/test_cases/examples/vehicles/vehicles.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      346 2020-05-02 09:28:32.000000 xmlschema-2.2.3/tests/test_cases/examples/vehicles/vehicles2.json
--rw-r--r--   0 brunato   (1000) brunato   (1000)      432 2020-01-23 20:05:17.000000 xmlschema-2.2.3/tests/test_cases/examples/vehicles/vehicles2.xml
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-04-14 13:52:42.379140 xmlschema-2.2.3/tests/test_cases/features/
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-04-14 13:52:42.402140 xmlschema-2.2.3/tests/test_cases/features/attributes/
--rw-r--r--   0 brunato   (1000) brunato   (1000)      688 2020-01-23 20:05:17.000000 xmlschema-2.2.3/tests/test_cases/features/attributes/default_attributes-missing_group.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      910 2020-01-23 20:05:17.000000 xmlschema-2.2.3/tests/test_cases/features/attributes/default_attributes.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-04-14 13:52:42.403140 xmlschema-2.2.3/tests/test_cases/features/builtins/
--rw-r--r--   0 brunato   (1000) brunato   (1000)      584 2020-01-23 20:05:17.000000 xmlschema-2.2.3/tests/test_cases/features/builtins/builtins.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      601 2020-01-23 20:05:17.000000 xmlschema-2.2.3/tests/test_cases/features/builtins/builtins.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-04-14 13:52:42.404140 xmlschema-2.2.3/tests/test_cases/features/decoder/
--rw-rw-r--   0 brunato   (1000) brunato   (1000)      781 2022-05-20 20:00:14.000000 xmlschema-2.2.3/tests/test_cases/features/decoder/data.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      725 2020-01-23 20:05:17.000000 xmlschema-2.2.3/tests/test_cases/features/decoder/data2.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      608 2021-04-01 09:07:37.000000 xmlschema-2.2.3/tests/test_cases/features/decoder/data3.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      480 2021-04-05 21:38:16.000000 xmlschema-2.2.3/tests/test_cases/features/decoder/data4-mixed.xml
--rw-rw-r--   0 brunato   (1000) brunato   (1000)      691 2021-12-08 19:41:39.000000 xmlschema-2.2.3/tests/test_cases/features/decoder/long-sequence-1.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      727 2021-04-05 21:38:16.000000 xmlschema-2.2.3/tests/test_cases/features/decoder/mixed-content.xsd
--rw-rw-r--   0 brunato   (1000) brunato   (1000)     5913 2022-05-20 20:00:14.000000 xmlschema-2.2.3/tests/test_cases/features/decoder/simple-types.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-04-14 13:52:42.405140 xmlschema-2.2.3/tests/test_cases/features/derivations/
--rw-r--r--   0 brunato   (1000) brunato   (1000)     1956 2020-01-23 20:05:17.000000 xmlschema-2.2.3/tests/test_cases/features/derivations/complex-extensions.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      662 2020-01-23 20:05:17.000000 xmlschema-2.2.3/tests/test_cases/features/derivations/complex-with-simple-content-restriction.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      599 2020-09-13 19:12:09.000000 xmlschema-2.2.3/tests/test_cases/features/derivations/invalid_enumeration_restriction.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)     2051 2020-08-14 19:07:25.000000 xmlschema-2.2.3/tests/test_cases/features/derivations/invalid_restrictions1.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)     1718 2020-01-23 20:05:17.000000 xmlschema-2.2.3/tests/test_cases/features/derivations/invalid_restrictions2.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      322 2020-01-23 20:05:17.000000 xmlschema-2.2.3/tests/test_cases/features/derivations/list_types.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      675 2020-01-23 20:05:17.000000 xmlschema-2.2.3/tests/test_cases/features/derivations/list_types.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-04-14 13:52:42.406140 xmlschema-2.2.3/tests/test_cases/features/elements/
--rw-r--r--   0 brunato   (1000) brunato   (1000)      154 2020-01-23 20:05:17.000000 xmlschema-2.2.3/tests/test_cases/features/elements/test_alternatives-1.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)     1487 2020-01-23 20:05:17.000000 xmlschema-2.2.3/tests/test_cases/features/elements/type_alternatives-no-ns.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)     1543 2020-01-23 20:05:17.000000 xmlschema-2.2.3/tests/test_cases/features/elements/type_alternatives.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-04-14 13:52:42.409140 xmlschema-2.2.3/tests/test_cases/features/models/
--rw-r--r--   0 brunato   (1000) brunato   (1000)     5143 2020-01-23 20:05:17.000000 xmlschema-2.2.3/tests/test_cases/features/models/billion_laughs_model.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      301 2020-01-23 20:05:17.000000 xmlschema-2.2.3/tests/test_cases/features/models/circular_model.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      215 2020-01-23 20:05:17.000000 xmlschema-2.2.3/tests/test_cases/features/models/illegal-attributes.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      647 2020-01-23 20:05:17.000000 xmlschema-2.2.3/tests/test_cases/features/models/illegal-declarations.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      523 2020-01-23 20:05:17.000000 xmlschema-2.2.3/tests/test_cases/features/models/illegal-occurs.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)     1192 2020-01-23 20:05:17.000000 xmlschema-2.2.3/tests/test_cases/features/models/invalid_models1.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)     1541 2020-01-23 20:05:17.000000 xmlschema-2.2.3/tests/test_cases/features/models/invalid_models2.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      306 2020-01-23 20:05:17.000000 xmlschema-2.2.3/tests/test_cases/features/models/model1.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)     4794 2020-04-28 13:28:56.000000 xmlschema-2.2.3/tests/test_cases/features/models/models.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      205 2020-01-23 20:05:17.000000 xmlschema-2.2.3/tests/test_cases/features/models/other-ns.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      760 2020-01-23 20:05:17.000000 xmlschema-2.2.3/tests/test_cases/features/models/recursive-groups.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)     1062 2020-04-28 13:28:56.000000 xmlschema-2.2.3/tests/test_cases/features/models/valid_model1.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-04-14 13:52:42.414140 xmlschema-2.2.3/tests/test_cases/features/namespaces/
--rw-r--r--   0 brunato   (1000) brunato   (1000)      151 2020-01-23 20:05:17.000000 xmlschema-2.2.3/tests/test_cases/features/namespaces/chameleon1.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      205 2020-01-23 20:05:17.000000 xmlschema-2.2.3/tests/test_cases/features/namespaces/chameleon2.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      272 2020-01-23 20:05:17.000000 xmlschema-2.2.3/tests/test_cases/features/namespaces/chameleon3.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      435 2020-01-23 20:05:17.000000 xmlschema-2.2.3/tests/test_cases/features/namespaces/default_ns_invalid.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      481 2020-01-23 20:05:17.000000 xmlschema-2.2.3/tests/test_cases/features/namespaces/default_ns_valid1.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      375 2020-01-23 20:05:17.000000 xmlschema-2.2.3/tests/test_cases/features/namespaces/default_ns_valid2.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      566 2020-01-23 20:05:17.000000 xmlschema-2.2.3/tests/test_cases/features/namespaces/import-case1.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      566 2020-01-23 20:05:17.000000 xmlschema-2.2.3/tests/test_cases/features/namespaces/import-case2.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      436 2020-01-23 20:05:17.000000 xmlschema-2.2.3/tests/test_cases/features/namespaces/import-case3.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      241 2020-01-23 20:05:17.000000 xmlschema-2.2.3/tests/test_cases/features/namespaces/import-case4-1.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      316 2020-01-23 20:05:17.000000 xmlschema-2.2.3/tests/test_cases/features/namespaces/import-case4-2.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      720 2020-01-23 20:05:17.000000 xmlschema-2.2.3/tests/test_cases/features/namespaces/import-case4a.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      720 2020-01-23 20:05:17.000000 xmlschema-2.2.3/tests/test_cases/features/namespaces/import-case4b.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      365 2022-09-08 10:16:11.000000 xmlschema-2.2.3/tests/test_cases/features/namespaces/import-case5a.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      377 2022-09-08 10:16:11.000000 xmlschema-2.2.3/tests/test_cases/features/namespaces/import-case5b.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      379 2022-09-08 10:16:11.000000 xmlschema-2.2.3/tests/test_cases/features/namespaces/import-case5c.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      504 2020-01-23 20:05:17.000000 xmlschema-2.2.3/tests/test_cases/features/namespaces/include-case1.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      435 2020-01-23 20:05:17.000000 xmlschema-2.2.3/tests/test_cases/features/namespaces/include-case1bis.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      590 2020-01-23 20:05:17.000000 xmlschema-2.2.3/tests/test_cases/features/namespaces/include-case2.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      541 2020-01-23 20:05:17.000000 xmlschema-2.2.3/tests/test_cases/features/namespaces/include-case2bis.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      516 2020-01-23 20:05:17.000000 xmlschema-2.2.3/tests/test_cases/features/namespaces/include-case3.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      490 2020-01-23 20:05:17.000000 xmlschema-2.2.3/tests/test_cases/features/namespaces/include-case4.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      520 2020-01-23 20:05:17.000000 xmlschema-2.2.3/tests/test_cases/features/namespaces/include-case5.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      499 2020-01-23 20:05:17.000000 xmlschema-2.2.3/tests/test_cases/features/namespaces/include-case6.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      261 2020-01-23 20:05:17.000000 xmlschema-2.2.3/tests/test_cases/features/namespaces/included3-valid.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      257 2020-01-23 20:05:17.000000 xmlschema-2.2.3/tests/test_cases/features/namespaces/included4-invalid.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      269 2020-01-23 20:05:17.000000 xmlschema-2.2.3/tests/test_cases/features/namespaces/included5-valid.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      211 2020-01-23 20:05:17.000000 xmlschema-2.2.3/tests/test_cases/features/namespaces/included6-invalid.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-04-14 13:52:42.414140 xmlschema-2.2.3/tests/test_cases/features/patterns/
--rw-r--r--   0 brunato   (1000) brunato   (1000)      833 2020-01-23 20:05:17.000000 xmlschema-2.2.3/tests/test_cases/features/patterns/patterns.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)     3276 2020-04-07 21:42:10.000000 xmlschema-2.2.3/tests/test_cases/features/patterns/patterns.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-04-14 13:52:42.415140 xmlschema-2.2.3/tests/test_cases/features/wsdl/
--rw-r--r--   0 brunato   (1000) brunato   (1000)     2091 2020-11-08 22:15:33.000000 xmlschema-2.2.3/tests/test_cases/features/wsdl/wsdl11_example3.wsdl
--rw-r--r--   0 brunato   (1000) brunato   (1000)     1954 2020-11-08 22:15:33.000000 xmlschema-2.2.3/tests/test_cases/features/wsdl/wsdl11_example3_valid.wsdl
--rw-r--r--   0 brunato   (1000) brunato   (1000)     2132 2020-11-08 22:15:33.000000 xmlschema-2.2.3/tests/test_cases/features/wsdl/wsdl11_example4.wsdl
--rw-r--r--   0 brunato   (1000) brunato   (1000)     1962 2020-11-08 22:15:33.000000 xmlschema-2.2.3/tests/test_cases/features/wsdl/wsdl11_example4_valid.wsdl
--rw-r--r--   0 brunato   (1000) brunato   (1000)     2996 2020-11-08 22:15:33.000000 xmlschema-2.2.3/tests/test_cases/features/wsdl/wsdl11_example5.wsdl
--rw-r--r--   0 brunato   (1000) brunato   (1000)     3163 2020-11-08 22:15:33.000000 xmlschema-2.2.3/tests/test_cases/features/wsdl/wsdl11_example5_valid.wsdl
--rw-r--r--   0 brunato   (1000) brunato   (1000)     3414 2020-11-08 22:15:33.000000 xmlschema-2.2.3/tests/test_cases/features/wsdl/wsdl11_example5_with_fault.wsdl
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-04-14 13:52:42.383139 xmlschema-2.2.3/tests/test_cases/issues/
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-04-14 13:52:42.416140 xmlschema-2.2.3/tests/test_cases/issues/issue_008/
--rw-r--r--   0 brunato   (1000) brunato   (1000)      252 2020-01-23 20:05:17.000000 xmlschema-2.2.3/tests/test_cases/issues/issue_008/issue_008.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      533 2020-01-23 20:05:17.000000 xmlschema-2.2.3/tests/test_cases/issues/issue_008/issue_008.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-04-14 13:52:42.416140 xmlschema-2.2.3/tests/test_cases/issues/issue_009/
--rw-r--r--   0 brunato   (1000) brunato   (1000)      303 2020-01-23 20:05:17.000000 xmlschema-2.2.3/tests/test_cases/issues/issue_009/issue_009.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-04-14 13:52:42.417140 xmlschema-2.2.3/tests/test_cases/issues/issue_013/
--rw-r--r--   0 brunato   (1000) brunato   (1000)      186 2020-01-23 20:05:17.000000 xmlschema-2.2.3/tests/test_cases/issues/issue_013/issue_013-1.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      731 2020-01-23 20:05:17.000000 xmlschema-2.2.3/tests/test_cases/issues/issue_013/issue_013-1.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      235 2020-01-23 20:05:17.000000 xmlschema-2.2.3/tests/test_cases/issues/issue_013/issue_013-2.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      184 2020-01-23 20:05:17.000000 xmlschema-2.2.3/tests/test_cases/issues/issue_013/issue_013.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      801 2020-01-23 20:05:17.000000 xmlschema-2.2.3/tests/test_cases/issues/issue_013/issue_013.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-04-14 13:52:42.417140 xmlschema-2.2.3/tests/test_cases/issues/issue_014/
--rw-r--r--   0 brunato   (1000) brunato   (1000)      556 2020-01-23 20:05:17.000000 xmlschema-2.2.3/tests/test_cases/issues/issue_014/issue014.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-04-14 13:52:42.418140 xmlschema-2.2.3/tests/test_cases/issues/issue_018/
--rw-r--r--   0 brunato   (1000) brunato   (1000)      193 2020-01-23 20:05:17.000000 xmlschema-2.2.3/tests/test_cases/issues/issue_018/issue_018-1.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)     1449 2020-01-23 20:05:17.000000 xmlschema-2.2.3/tests/test_cases/issues/issue_018/issue_018.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-04-14 13:52:42.419140 xmlschema-2.2.3/tests/test_cases/issues/issue_022/
--rw-r--r--   0 brunato   (1000) brunato   (1000)     1048 2020-01-23 20:05:17.000000 xmlschema-2.2.3/tests/test_cases/issues/issue_022/README.md
--rw-r--r--   0 brunato   (1000) brunato   (1000)      130 2020-01-23 20:05:17.000000 xmlschema-2.2.3/tests/test_cases/issues/issue_022/xml_string_1.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      208 2020-01-23 20:05:17.000000 xmlschema-2.2.3/tests/test_cases/issues/issue_022/xml_string_2.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      666 2020-01-23 20:05:17.000000 xmlschema-2.2.3/tests/test_cases/issues/issue_022/xsd_string.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-04-14 13:52:42.420140 xmlschema-2.2.3/tests/test_cases/issues/issue_026/
--rw-r--r--   0 brunato   (1000) brunato   (1000)      229 2020-01-23 20:05:17.000000 xmlschema-2.2.3/tests/test_cases/issues/issue_026/issue_026-1.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      224 2020-01-23 20:05:17.000000 xmlschema-2.2.3/tests/test_cases/issues/issue_026/issue_026-2.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      213 2020-01-23 20:05:17.000000 xmlschema-2.2.3/tests/test_cases/issues/issue_026/issue_026-3.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      664 2020-01-23 20:05:17.000000 xmlschema-2.2.3/tests/test_cases/issues/issue_026/issue_026.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-04-14 13:52:42.420140 xmlschema-2.2.3/tests/test_cases/issues/issue_028/
--rw-r--r--   0 brunato   (1000) brunato   (1000)      203 2020-01-23 20:05:17.000000 xmlschema-2.2.3/tests/test_cases/issues/issue_028/issue_028-1.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      181 2020-01-23 20:05:17.000000 xmlschema-2.2.3/tests/test_cases/issues/issue_028/issue_028-2.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      353 2020-01-23 20:05:17.000000 xmlschema-2.2.3/tests/test_cases/issues/issue_028/issue_028.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-04-14 13:52:42.421140 xmlschema-2.2.3/tests/test_cases/issues/issue_029/
--rw-r--r--   0 brunato   (1000) brunato   (1000)      203 2020-01-23 20:05:17.000000 xmlschema-2.2.3/tests/test_cases/issues/issue_029/issue_029-1.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      159 2020-01-23 20:05:17.000000 xmlschema-2.2.3/tests/test_cases/issues/issue_029/issue_029-2.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      181 2020-01-23 20:05:17.000000 xmlschema-2.2.3/tests/test_cases/issues/issue_029/issue_029-3.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      363 2020-01-23 20:05:17.000000 xmlschema-2.2.3/tests/test_cases/issues/issue_029/issue_029.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-04-14 13:52:42.421140 xmlschema-2.2.3/tests/test_cases/issues/issue_035/
--rw-r--r--   0 brunato   (1000) brunato   (1000)      869 2020-01-23 20:05:17.000000 xmlschema-2.2.3/tests/test_cases/issues/issue_035/dates.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)     1081 2020-01-23 20:05:17.000000 xmlschema-2.2.3/tests/test_cases/issues/issue_035/dates.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-04-14 13:52:42.422140 xmlschema-2.2.3/tests/test_cases/issues/issue_041/
--rw-r--r--   0 brunato   (1000) brunato   (1000)      247 2020-01-23 20:05:17.000000 xmlschema-2.2.3/tests/test_cases/issues/issue_041/issue_041.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      708 2020-01-23 20:05:17.000000 xmlschema-2.2.3/tests/test_cases/issues/issue_041/issue_041.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-04-14 13:52:42.422140 xmlschema-2.2.3/tests/test_cases/issues/issue_045/
--rw-r--r--   0 brunato   (1000) brunato   (1000)      275 2020-01-23 20:05:17.000000 xmlschema-2.2.3/tests/test_cases/issues/issue_045/issue_045.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-04-14 13:52:42.423140 xmlschema-2.2.3/tests/test_cases/issues/issue_046/
--rw-r--r--   0 brunato   (1000) brunato   (1000)      354 2020-01-23 20:05:17.000000 xmlschema-2.2.3/tests/test_cases/issues/issue_046/issue_046.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      419 2020-01-23 20:05:17.000000 xmlschema-2.2.3/tests/test_cases/issues/issue_046/issue_046.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-04-14 13:52:42.423140 xmlschema-2.2.3/tests/test_cases/issues/issue_051/
--rw-r--r--   0 brunato   (1000) brunato   (1000)      331 2020-01-23 20:05:17.000000 xmlschema-2.2.3/tests/test_cases/issues/issue_051/issue_051.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      824 2020-01-23 20:05:17.000000 xmlschema-2.2.3/tests/test_cases/issues/issue_051/issue_051.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-04-14 13:52:42.424140 xmlschema-2.2.3/tests/test_cases/issues/issue_073/
--rw-r--r--   0 brunato   (1000) brunato   (1000)      327 2020-01-23 20:05:17.000000 xmlschema-2.2.3/tests/test_cases/issues/issue_073/issue_073-1.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      362 2020-01-23 20:05:17.000000 xmlschema-2.2.3/tests/test_cases/issues/issue_073/issue_073-2.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      685 2020-01-23 20:05:17.000000 xmlschema-2.2.3/tests/test_cases/issues/issue_073/issue_073.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-04-14 13:52:42.424140 xmlschema-2.2.3/tests/test_cases/issues/issue_086/
--rw-r--r--   0 brunato   (1000) brunato   (1000)      403 2020-01-23 20:05:17.000000 xmlschema-2.2.3/tests/test_cases/issues/issue_086/issue_086-1.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      403 2020-01-23 20:05:17.000000 xmlschema-2.2.3/tests/test_cases/issues/issue_086/issue_086-2.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)     1328 2020-01-23 20:05:17.000000 xmlschema-2.2.3/tests/test_cases/issues/issue_086/issue_086.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-04-14 13:52:42.424140 xmlschema-2.2.3/tests/test_cases/issues/issue_105/
--rw-r--r--   0 brunato   (1000) brunato   (1000)      515 2020-01-23 20:05:17.000000 xmlschema-2.2.3/tests/test_cases/issues/issue_105/issue_105.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-04-14 13:52:42.425140 xmlschema-2.2.3/tests/test_cases/issues/issue_111/
--rw-r--r--   0 brunato   (1000) brunato   (1000)      698 2020-01-23 20:05:17.000000 xmlschema-2.2.3/tests/test_cases/issues/issue_111/issue_111.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      590 2020-01-23 20:05:17.000000 xmlschema-2.2.3/tests/test_cases/issues/issue_111/issue_111_skeleton.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-04-14 13:52:42.425140 xmlschema-2.2.3/tests/test_cases/issues/issue_115/
--rw-r--r--   0 brunato   (1000) brunato   (1000)      620 2020-01-23 20:05:17.000000 xmlschema-2.2.3/tests/test_cases/issues/issue_115/Rotation.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-04-14 13:52:42.426140 xmlschema-2.2.3/tests/test_cases/issues/issue_171/
--rw-r--r--   0 brunato   (1000) brunato   (1000)      535 2020-03-23 16:13:26.000000 xmlschema-2.2.3/tests/test_cases/issues/issue_171/issue_171.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      580 2020-03-23 16:13:26.000000 xmlschema-2.2.3/tests/test_cases/issues/issue_171/issue_171b.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      504 2020-08-14 19:07:25.000000 xmlschema-2.2.3/tests/test_cases/issues/issue_171/issue_171c.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-04-14 13:52:42.426140 xmlschema-2.2.3/tests/test_cases/issues/issue_187/
--rw-r--r--   0 brunato   (1000) brunato   (1000)      666 2020-09-25 15:20:24.000000 xmlschema-2.2.3/tests/test_cases/issues/issue_187/issue_187_1.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      804 2020-09-25 15:20:24.000000 xmlschema-2.2.3/tests/test_cases/issues/issue_187/issue_187_2.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-04-14 13:52:42.427140 xmlschema-2.2.3/tests/test_cases/issues/issue_190/
--rw-r--r--   0 brunato   (1000) brunato   (1000)      109 2020-05-28 20:30:12.000000 xmlschema-2.2.3/tests/test_cases/issues/issue_190/issue_190.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      785 2020-05-28 20:30:12.000000 xmlschema-2.2.3/tests/test_cases/issues/issue_190/issue_190.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-04-14 13:52:42.427140 xmlschema-2.2.3/tests/test_cases/issues/issue_200/
--rw-r--r--   0 brunato   (1000) brunato   (1000)      310 2020-08-14 19:07:25.000000 xmlschema-2.2.3/tests/test_cases/issues/issue_200/issue_200.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      752 2020-08-14 19:07:25.000000 xmlschema-2.2.3/tests/test_cases/issues/issue_200/issue_200.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-04-14 13:52:42.428140 xmlschema-2.2.3/tests/test_cases/issues/issue_203/
--rw-r--r--   0 brunato   (1000) brunato   (1000)      196 2020-09-19 06:08:01.000000 xmlschema-2.2.3/tests/test_cases/issues/issue_203/issue_203.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      960 2020-09-19 06:08:01.000000 xmlschema-2.2.3/tests/test_cases/issues/issue_203/issue_203.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      964 2020-09-19 06:08:01.000000 xmlschema-2.2.3/tests/test_cases/issues/issue_203/issue_203alt.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-04-14 13:52:42.429140 xmlschema-2.2.3/tests/test_cases/issues/issue_204/
--rw-r--r--   0 brunato   (1000) brunato   (1000)      524 2020-09-25 15:20:24.000000 xmlschema-2.2.3/tests/test_cases/issues/issue_204/issue_204.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      172 2020-09-25 15:20:24.000000 xmlschema-2.2.3/tests/test_cases/issues/issue_204/issue_204_1.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      186 2020-09-25 15:20:24.000000 xmlschema-2.2.3/tests/test_cases/issues/issue_204/issue_204_2.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      222 2020-09-25 15:20:24.000000 xmlschema-2.2.3/tests/test_cases/issues/issue_204/issue_204_3.xml
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-04-14 13:52:42.429140 xmlschema-2.2.3/tests/test_cases/issues/issue_208/
--rw-r--r--   0 brunato   (1000) brunato   (1000)      306 2020-11-08 22:15:33.000000 xmlschema-2.2.3/tests/test_cases/issues/issue_208/issue_208.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)     1532 2020-11-08 22:15:33.000000 xmlschema-2.2.3/tests/test_cases/issues/issue_208/issue_208.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-04-14 13:52:42.429140 xmlschema-2.2.3/tests/test_cases/issues/issue_222/
--rw-r--r--   0 brunato   (1000) brunato   (1000)       66 2021-01-24 21:47:47.000000 xmlschema-2.2.3/tests/test_cases/issues/issue_222/issue_222.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      569 2021-01-24 21:47:47.000000 xmlschema-2.2.3/tests/test_cases/issues/issue_222/issue_222.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-04-14 13:52:42.430140 xmlschema-2.2.3/tests/test_cases/issues/issue_223/
--rw-r--r--   0 brunato   (1000) brunato   (1000)       46 2021-01-24 21:47:47.000000 xmlschema-2.2.3/tests/test_cases/issues/issue_223/issue_223.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      392 2021-03-30 11:13:45.000000 xmlschema-2.2.3/tests/test_cases/issues/issue_223/issue_223.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-04-14 13:52:42.381139 xmlschema-2.2.3/tests/test_cases/issues/issue_237/
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-04-14 13:52:42.430140 xmlschema-2.2.3/tests/test_cases/issues/issue_237/dir1/
--rw-r--r--   0 brunato   (1000) brunato   (1000)      191 2021-04-05 21:38:16.000000 xmlschema-2.2.3/tests/test_cases/issues/issue_237/dir1/issue_237.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)     1249 2021-04-05 21:38:16.000000 xmlschema-2.2.3/tests/test_cases/issues/issue_237/dir1/stockquoteservice.wsdl
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-04-14 13:52:42.431140 xmlschema-2.2.3/tests/test_cases/issues/issue_237/dir2/
--rw-r--r--   0 brunato   (1000) brunato   (1000)      141 2021-04-05 21:38:16.000000 xmlschema-2.2.3/tests/test_cases/issues/issue_237/dir2/issue_237a.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      314 2021-04-05 21:38:16.000000 xmlschema-2.2.3/tests/test_cases/issues/issue_237/dir2/issue_237b.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)     1041 2021-04-05 21:38:16.000000 xmlschema-2.2.3/tests/test_cases/issues/issue_237/dir2/stockquote.wsdl
--rw-r--r--   0 brunato   (1000) brunato   (1000)      664 2021-04-05 21:38:16.000000 xmlschema-2.2.3/tests/test_cases/issues/issue_237/dir2/stockquote.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-04-14 13:52:42.431140 xmlschema-2.2.3/tests/test_cases/issues/issue_243/
--rw-r--r--   0 brunato   (1000) brunato   (1000)      283 2021-05-03 11:37:57.000000 xmlschema-2.2.3/tests/test_cases/issues/issue_243/issue_243.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)     2063 2021-05-03 11:37:57.000000 xmlschema-2.2.3/tests/test_cases/issues/issue_243/issue_243.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-04-14 13:52:42.432140 xmlschema-2.2.3/tests/test_cases/issues/issue_245/
--rw-r--r--   0 brunato   (1000) brunato   (1000)      757 2021-05-03 11:37:57.000000 xmlschema-2.2.3/tests/test_cases/issues/issue_245/issue_245-valid.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      757 2021-05-03 11:37:57.000000 xmlschema-2.2.3/tests/test_cases/issues/issue_245/issue_245.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)     4894 2021-05-03 11:37:57.000000 xmlschema-2.2.3/tests/test_cases/issues/issue_245/issue_245.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-04-14 13:52:42.432140 xmlschema-2.2.3/tests/test_cases/issues/issue_259/
--rw-rw-r--   0 brunato   (1000) brunato   (1000)     2422 2021-09-02 10:52:43.000000 xmlschema-2.2.3/tests/test_cases/issues/issue_259/issue_259-1.xsd
--rw-rw-r--   0 brunato   (1000) brunato   (1000)     1432 2021-09-02 10:52:43.000000 xmlschema-2.2.3/tests/test_cases/issues/issue_259/issue_259-2.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-04-14 13:52:42.433140 xmlschema-2.2.3/tests/test_cases/issues/issue_265/
--rw-rw-r--   0 brunato   (1000) brunato   (1000)     3471 2021-10-20 14:14:48.000000 xmlschema-2.2.3/tests/test_cases/issues/issue_265/issue_265-1.xsd
--rw-rw-r--   0 brunato   (1000) brunato   (1000)     1411 2021-10-20 14:14:48.000000 xmlschema-2.2.3/tests/test_cases/issues/issue_265/issue_265-2-invalid.xsd
--rw-rw-r--   0 brunato   (1000) brunato   (1000)      454 2021-10-20 14:14:48.000000 xmlschema-2.2.3/tests/test_cases/issues/issue_265/issue_265-2-override.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-04-14 13:52:42.434140 xmlschema-2.2.3/tests/test_cases/issues/issue_266/
--rw-rw-r--   0 brunato   (1000) brunato   (1000)      158 2021-10-20 14:14:48.000000 xmlschema-2.2.3/tests/test_cases/issues/issue_266/issue_266-1.xml
--rw-rw-r--   0 brunato   (1000) brunato   (1000)      538 2021-10-20 14:14:48.000000 xmlschema-2.2.3/tests/test_cases/issues/issue_266/issue_266-1.xsd
--rw-rw-r--   0 brunato   (1000) brunato   (1000)      158 2021-10-20 14:14:48.000000 xmlschema-2.2.3/tests/test_cases/issues/issue_266/issue_266-2.xml
--rw-rw-r--   0 brunato   (1000) brunato   (1000)      528 2021-10-20 14:14:48.000000 xmlschema-2.2.3/tests/test_cases/issues/issue_266/issue_266-2.xsd
--rw-rw-r--   0 brunato   (1000) brunato   (1000)      651 2021-11-11 15:30:24.000000 xmlschema-2.2.3/tests/test_cases/issues/issue_266/issue_266b-1.xsd
--rw-rw-r--   0 brunato   (1000) brunato   (1000)      551 2021-11-11 15:30:24.000000 xmlschema-2.2.3/tests/test_cases/issues/issue_266/issue_266b-2.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-04-14 13:52:42.434140 xmlschema-2.2.3/tests/test_cases/issues/issue_273/
--rw-rw-r--   0 brunato   (1000) brunato   (1000)      299 2021-12-08 19:41:39.000000 xmlschema-2.2.3/tests/test_cases/issues/issue_273/issue_273.xml
--rw-rw-r--   0 brunato   (1000) brunato   (1000)      517 2021-12-08 19:41:39.000000 xmlschema-2.2.3/tests/test_cases/issues/issue_273/issue_273.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-04-14 13:52:42.435140 xmlschema-2.2.3/tests/test_cases/issues/issue_276/
--rw-rw-r--   0 brunato   (1000) brunato   (1000)      122 2021-12-08 22:11:41.000000 xmlschema-2.2.3/tests/test_cases/issues/issue_276/dummy.xml
--rw-rw-r--   0 brunato   (1000) brunato   (1000)      495 2021-12-08 22:11:41.000000 xmlschema-2.2.3/tests/test_cases/issues/issue_276/schema.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-04-14 13:52:42.435140 xmlschema-2.2.3/tests/test_cases/issues/issue_298/
--rw-rw-r--   0 brunato   (1000) brunato   (1000)      114 2022-05-22 16:17:24.000000 xmlschema-2.2.3/tests/test_cases/issues/issue_298/issue_298-1.xml
--rw-rw-r--   0 brunato   (1000) brunato   (1000)      240 2022-05-22 16:17:24.000000 xmlschema-2.2.3/tests/test_cases/issues/issue_298/issue_298-2.xml
--rw-rw-r--   0 brunato   (1000) brunato   (1000)      792 2022-05-22 16:17:24.000000 xmlschema-2.2.3/tests/test_cases/issues/issue_298/issue_298.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-04-14 13:52:42.436140 xmlschema-2.2.3/tests/test_cases/issues/issue_306/
--rw-rw-r--   0 brunato   (1000) brunato   (1000)      881 2022-06-24 14:13:22.000000 xmlschema-2.2.3/tests/test_cases/issues/issue_306/issue_306-alt.xsd
--rw-rw-r--   0 brunato   (1000) brunato   (1000)      203 2022-06-24 14:13:22.000000 xmlschema-2.2.3/tests/test_cases/issues/issue_306/issue_306-invalid.xml
--rw-rw-r--   0 brunato   (1000) brunato   (1000)      182 2022-06-24 14:13:22.000000 xmlschema-2.2.3/tests/test_cases/issues/issue_306/issue_306-valid.xml
--rw-rw-r--   0 brunato   (1000) brunato   (1000)      689 2022-06-24 14:13:22.000000 xmlschema-2.2.3/tests/test_cases/issues/issue_306/issue_306.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-04-14 13:52:42.437140 xmlschema-2.2.3/tests/test_cases/issues/issue_311/
--rw-rw-r--   0 brunato   (1000) brunato   (1000)      786 2022-07-18 14:19:15.000000 xmlschema-2.2.3/tests/test_cases/issues/issue_311/correct_no_list.xml
--rw-rw-r--   0 brunato   (1000) brunato   (1000)      788 2022-07-18 14:19:15.000000 xmlschema-2.2.3/tests/test_cases/issues/issue_311/incorrect_with_list.xml
--rw-rw-r--   0 brunato   (1000) brunato   (1000)     4013 2022-07-18 14:19:15.000000 xmlschema-2.2.3/tests/test_cases/issues/issue_311/kPartModel_reduit_issue.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-04-14 13:52:42.437140 xmlschema-2.2.3/tests/test_cases/issues/issue_314/
--rw-rw-r--   0 brunato   (1000) brunato   (1000)      267 2022-07-21 09:40:50.000000 xmlschema-2.2.3/tests/test_cases/issues/issue_314/issue_314.xml
--rw-rw-r--   0 brunato   (1000) brunato   (1000)     1153 2022-07-21 09:40:50.000000 xmlschema-2.2.3/tests/test_cases/issues/issue_314/issue_314.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-04-14 13:52:42.439140 xmlschema-2.2.3/tests/test_cases/issues/issue_315/
--rw-rw-r--   0 brunato   (1000) brunato   (1000)       66 2022-07-18 14:19:15.000000 xmlschema-2.2.3/tests/test_cases/issues/issue_315/issue_315-1.xml
--rw-rw-r--   0 brunato   (1000) brunato   (1000)       63 2022-07-18 14:19:15.000000 xmlschema-2.2.3/tests/test_cases/issues/issue_315/issue_315-2.xml
--rw-rw-r--   0 brunato   (1000) brunato   (1000)       71 2022-07-18 14:19:15.000000 xmlschema-2.2.3/tests/test_cases/issues/issue_315/issue_315-3.xml
--rw-rw-r--   0 brunato   (1000) brunato   (1000)       76 2022-07-18 14:19:15.000000 xmlschema-2.2.3/tests/test_cases/issues/issue_315/issue_315-4.xml
--rw-rw-r--   0 brunato   (1000) brunato   (1000)       71 2022-07-18 14:19:15.000000 xmlschema-2.2.3/tests/test_cases/issues/issue_315/issue_315-5.xml
--rw-rw-r--   0 brunato   (1000) brunato   (1000)      604 2022-07-18 14:19:15.000000 xmlschema-2.2.3/tests/test_cases/issues/issue_315/issue_315_mixed.xsd
--rw-rw-r--   0 brunato   (1000) brunato   (1000)      456 2022-07-18 14:19:15.000000 xmlschema-2.2.3/tests/test_cases/issues/issue_315/issue_315_simple.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-04-14 13:52:42.439140 xmlschema-2.2.3/tests/test_cases/issues/issue_322/
--rw-r--r--   0 brunato   (1000) brunato   (1000)      155 2022-08-26 15:33:28.000000 xmlschema-2.2.3/tests/test_cases/issues/issue_322/issue_322.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      348 2022-08-26 15:33:28.000000 xmlschema-2.2.3/tests/test_cases/issues/issue_322/issue_322.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-04-14 13:52:42.440140 xmlschema-2.2.3/tests/test_cases/issues/issue_324/
--rw-r--r--   0 brunato   (1000) brunato   (1000)      373 2022-09-08 10:16:11.000000 xmlschema-2.2.3/tests/test_cases/issues/issue_324/issue_324-invalid.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      373 2022-09-08 10:16:11.000000 xmlschema-2.2.3/tests/test_cases/issues/issue_324/issue_324-valid.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      672 2022-08-28 05:56:41.000000 xmlschema-2.2.3/tests/test_cases/issues/issue_324/issue_324.zip
--rw-r--r--   0 brunato   (1000) brunato   (1000)      384 2022-09-08 10:16:11.000000 xmlschema-2.2.3/tests/test_cases/issues/issue_324/issue_324a.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      190 2022-09-08 10:16:11.000000 xmlschema-2.2.3/tests/test_cases/issues/issue_324/issue_324b.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-04-14 13:52:42.441140 xmlschema-2.2.3/tests/test_cases/issues/issue_334/
--rw-r--r--   0 brunato   (1000) brunato   (1000)     1814 2023-02-11 10:41:50.000000 xmlschema-2.2.3/tests/test_cases/issues/issue_334/issue_334.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)     5149 2023-02-11 10:41:50.000000 xmlschema-2.2.3/tests/test_cases/issues/issue_334/issue_334.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)     2663 2023-02-09 09:02:31.000000 xmlschema-2.2.3/tests/test_cases/issues/issue_334/issue_334.zip
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-04-14 13:52:42.442140 xmlschema-2.2.3/tests/test_cases/issues/issue_341/
--rw-r--r--   0 brunato   (1000) brunato   (1000)     2070 2023-04-14 13:49:05.000000 xmlschema-2.2.3/tests/test_cases/issues/issue_341/issue_341-ext.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      158 2023-04-14 13:49:05.000000 xmlschema-2.2.3/tests/test_cases/issues/issue_341/issue_341.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)     1781 2023-04-14 13:49:05.000000 xmlschema-2.2.3/tests/test_cases/issues/issue_341/issue_341.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-04-14 13:52:42.442140 xmlschema-2.2.3/tests/test_cases/mypy/
--rw-rw-r--   0 brunato   (1000) brunato   (1000)      911 2022-05-20 16:16:20.000000 xmlschema-2.2.3/tests/test_cases/mypy/extra_validator.py
--rwxrwxr-x   0 brunato   (1000) brunato   (1000)     1905 2021-11-11 15:30:24.000000 xmlschema-2.2.3/tests/test_cases/mypy/schema_source.py
--rwxrwxr-x   0 brunato   (1000) brunato   (1000)      646 2021-11-11 15:30:24.000000 xmlschema-2.2.3/tests/test_cases/mypy/simple_types.py
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-04-14 13:52:42.444140 xmlschema-2.2.3/tests/test_cases/resources/
--rw-r--r--   0 brunato   (1000) brunato   (1000)       13 2020-01-23 20:05:17.000000 xmlschema-2.2.3/tests/test_cases/resources/dummy file #2.txt
--rw-r--r--   0 brunato   (1000) brunato   (1000)       13 2020-01-23 20:05:17.000000 xmlschema-2.2.3/tests/test_cases/resources/dummy file.txt
--rw-r--r--   0 brunato   (1000) brunato   (1000)      171 2020-01-23 20:05:17.000000 xmlschema-2.2.3/tests/test_cases/resources/external_entity.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)       20 2020-01-23 20:05:17.000000 xmlschema-2.2.3/tests/test_cases/resources/malformed.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      308 2020-11-08 22:15:33.000000 xmlschema-2.2.3/tests/test_cases/resources/unparsed_entity.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      170 2020-01-23 20:05:17.000000 xmlschema-2.2.3/tests/test_cases/resources/unused_external_entity.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      270 2020-11-08 22:15:33.000000 xmlschema-2.2.3/tests/test_cases/resources/unused_unparsed_entity.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      129 2020-01-23 20:05:17.000000 xmlschema-2.2.3/tests/test_cases/resources/with_entity.xml
--rw-rw-r--   0 brunato   (1000) brunato   (1000)     6165 2022-07-18 14:19:15.000000 xmlschema-2.2.3/tests/test_cases/testfiles
--rw-r--r--   0 brunato   (1000) brunato   (1000)    11973 2021-03-04 20:38:45.000000 xmlschema-2.2.3/tests/test_cli.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    26576 2023-02-11 10:41:50.000000 xmlschema-2.2.3/tests/test_codegen.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    28857 2022-08-26 15:33:28.000000 xmlschema-2.2.3/tests/test_converters.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    26556 2023-02-06 08:55:27.000000 xmlschema-2.2.3/tests/test_dataobjects.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    24554 2023-02-06 06:20:42.000000 xmlschema-2.2.3/tests/test_documents.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)     3234 2021-02-05 08:47:55.000000 xmlschema-2.2.3/tests/test_files.py
--rw-rw-r--   0 brunato   (1000) brunato   (1000)    26065 2022-07-18 14:19:15.000000 xmlschema-2.2.3/tests/test_helpers.py
--rw-rw-r--   0 brunato   (1000) brunato   (1000)     5745 2021-12-08 22:11:41.000000 xmlschema-2.2.3/tests/test_memory.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)     9099 2023-02-11 10:41:50.000000 xmlschema-2.2.3/tests/test_namespaces.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)     4755 2023-03-05 21:16:57.000000 xmlschema-2.2.3/tests/test_package.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    70653 2023-02-06 06:20:42.000000 xmlschema-2.2.3/tests/test_resources.py
--rw-rw-r--   0 brunato   (1000) brunato   (1000)     1785 2021-09-02 10:52:43.000000 xmlschema-2.2.3/tests/test_schemas.py
--rw-rw-r--   0 brunato   (1000) brunato   (1000)     3600 2022-05-20 20:00:14.000000 xmlschema-2.2.3/tests/test_translations.py
--rw-rw-r--   0 brunato   (1000) brunato   (1000)     2397 2022-05-20 16:16:20.000000 xmlschema-2.2.3/tests/test_typing.py
--rw-rw-r--   0 brunato   (1000) brunato   (1000)     1806 2021-09-02 10:52:43.000000 xmlschema-2.2.3/tests/test_validation.py
--rw-rw-r--   0 brunato   (1000) brunato   (1000)    27317 2022-07-18 14:19:15.000000 xmlschema-2.2.3/tests/test_w3c_suite.py
--rw-rw-r--   0 brunato   (1000) brunato   (1000)    43436 2022-07-18 14:19:15.000000 xmlschema-2.2.3/tests/test_wsdl.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    15023 2023-02-11 10:41:50.000000 xmlschema-2.2.3/tests/test_xpath.py
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-04-14 13:52:42.445140 xmlschema-2.2.3/tests/validation/
--rw-r--r--   0 brunato   (1000) brunato   (1000)        0 2020-11-10 10:12:46.000000 xmlschema-2.2.3/tests/validation/__init__.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    66088 2023-04-14 13:49:05.000000 xmlschema-2.2.3/tests/validation/test_decoding.py
--rw-rw-r--   0 brunato   (1000) brunato   (1000)    33339 2022-07-18 14:19:15.000000 xmlschema-2.2.3/tests/validation/test_encoding.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    16337 2022-10-01 13:42:01.000000 xmlschema-2.2.3/tests/validation/test_validation.py
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-04-14 13:52:42.449140 xmlschema-2.2.3/tests/validators/
--rw-r--r--   0 brunato   (1000) brunato   (1000)        0 2020-11-10 10:12:46.000000 xmlschema-2.2.3/tests/validators/__init__.py
--rw-rw-r--   0 brunato   (1000) brunato   (1000)    25878 2022-07-18 14:19:15.000000 xmlschema-2.2.3/tests/validators/test_attributes.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    14352 2020-12-23 12:38:37.000000 xmlschema-2.2.3/tests/validators/test_builtins.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    33116 2023-03-05 20:30:24.000000 xmlschema-2.2.3/tests/validators/test_complex_types.py
--rw-rw-r--   0 brunato   (1000) brunato   (1000)     4333 2022-06-24 14:13:22.000000 xmlschema-2.2.3/tests/validators/test_elements.py
--rw-rw-r--   0 brunato   (1000) brunato   (1000)     9464 2022-07-18 14:19:15.000000 xmlschema-2.2.3/tests/validators/test_exceptions.py
--rw-rw-r--   0 brunato   (1000) brunato   (1000)    60271 2022-07-18 14:19:15.000000 xmlschema-2.2.3/tests/validators/test_facets.py
--rw-rw-r--   0 brunato   (1000) brunato   (1000)     5409 2022-03-07 13:26:41.000000 xmlschema-2.2.3/tests/validators/test_global_maps.py
--rw-rw-r--   0 brunato   (1000) brunato   (1000)    13430 2021-10-20 14:14:48.000000 xmlschema-2.2.3/tests/validators/test_groups.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    19187 2023-02-06 06:20:42.000000 xmlschema-2.2.3/tests/validators/test_identities.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    52697 2023-04-14 13:49:05.000000 xmlschema-2.2.3/tests/validators/test_models.py
--rw-rw-r--   0 brunato   (1000) brunato   (1000)     3447 2022-07-18 14:19:15.000000 xmlschema-2.2.3/tests/validators/test_notations.py
--rw-rw-r--   0 brunato   (1000) brunato   (1000)     8625 2022-07-18 14:19:15.000000 xmlschema-2.2.3/tests/validators/test_particles.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    41506 2022-10-01 13:42:01.000000 xmlschema-2.2.3/tests/validators/test_schemas.py
--rw-rw-r--   0 brunato   (1000) brunato   (1000)    10292 2022-07-18 14:19:15.000000 xmlschema-2.2.3/tests/validators/test_simple_types.py
--rw-rw-r--   0 brunato   (1000) brunato   (1000)    34302 2022-07-18 14:19:15.000000 xmlschema-2.2.3/tests/validators/test_wildcards.py
--rw-rw-r--   0 brunato   (1000) brunato   (1000)    33897 2022-07-18 14:19:15.000000 xmlschema-2.2.3/tests/validators/test_xsdbase.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)     1632 2023-04-14 13:49:05.000000 xmlschema-2.2.3/tox.ini
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-04-14 13:52:42.451140 xmlschema-2.2.3/xmlschema/
--rw-r--r--   0 brunato   (1000) brunato   (1000)     2857 2023-04-14 13:49:05.000000 xmlschema-2.2.3/xmlschema/__init__.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)     5515 2023-03-05 21:16:57.000000 xmlschema-2.2.3/xmlschema/aliases.py
--rw-rw-r--   0 brunato   (1000) brunato   (1000)    11662 2022-07-18 14:19:15.000000 xmlschema-2.2.3/xmlschema/cli.py
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-04-14 13:52:42.454140 xmlschema-2.2.3/xmlschema/converters/
--rw-rw-r--   0 brunato   (1000) brunato   (1000)      813 2022-07-18 14:19:15.000000 xmlschema-2.2.3/xmlschema/converters/__init__.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)     5977 2023-03-05 21:16:57.000000 xmlschema-2.2.3/xmlschema/converters/abdera.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)     7228 2023-03-05 21:16:57.000000 xmlschema-2.2.3/xmlschema/converters/badgerfish.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)     7587 2023-03-05 21:16:57.000000 xmlschema-2.2.3/xmlschema/converters/columnar.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    19819 2023-03-05 21:16:57.000000 xmlschema-2.2.3/xmlschema/converters/default.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)     4769 2023-03-05 21:16:57.000000 xmlschema-2.2.3/xmlschema/converters/jsonml.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)     5840 2023-03-05 21:16:57.000000 xmlschema-2.2.3/xmlschema/converters/parker.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)     5711 2023-03-05 21:16:57.000000 xmlschema-2.2.3/xmlschema/converters/unordered.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    23717 2023-03-05 21:16:57.000000 xmlschema-2.2.3/xmlschema/dataobjects.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    35488 2023-02-06 06:20:42.000000 xmlschema-2.2.3/xmlschema/documents.py
--rw-rw-r--   0 brunato   (1000) brunato   (1000)     1235 2021-10-20 14:14:48.000000 xmlschema-2.2.3/xmlschema/exceptions.py
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-04-14 13:52:42.455140 xmlschema-2.2.3/xmlschema/extras/
--rw-r--r--   0 brunato   (1000) brunato   (1000)        0 2021-02-05 09:05:33.000000 xmlschema-2.2.3/xmlschema/extras/__init__.py
--rw-rw-r--   0 brunato   (1000) brunato   (1000)    21923 2023-02-11 09:04:58.000000 xmlschema-2.2.3/xmlschema/extras/codegen.py
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-04-14 13:52:42.384139 xmlschema-2.2.3/xmlschema/extras/templates/
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-04-14 13:52:42.455140 xmlschema-2.2.3/xmlschema/extras/templates/python/
--rw-rw-r--   0 brunato   (1000) brunato   (1000)      997 2022-07-18 14:19:15.000000 xmlschema-2.2.3/xmlschema/extras/templates/python/bindings.py.jinja
--rw-r--r--   0 brunato   (1000) brunato   (1000)     1116 2021-02-11 14:32:40.000000 xmlschema-2.2.3/xmlschema/extras/templates/python/sample.py.jinja
--rw-rw-r--   0 brunato   (1000) brunato   (1000)    23802 2022-06-24 14:13:22.000000 xmlschema-2.2.3/xmlschema/extras/wsdl.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    11097 2022-08-26 15:33:28.000000 xmlschema-2.2.3/xmlschema/helpers.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)      677 2020-11-10 10:13:55.000000 xmlschema-2.2.3/xmlschema/limits.py
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-04-14 13:52:42.384139 xmlschema-2.2.3/xmlschema/locale/
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-04-14 13:52:42.384139 xmlschema-2.2.3/xmlschema/locale/en/
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-04-14 13:52:42.456140 xmlschema-2.2.3/xmlschema/locale/en/LC_MESSAGES/
--rw-rw-r--   0 brunato   (1000) brunato   (1000)    45327 2022-05-20 20:00:14.000000 xmlschema-2.2.3/xmlschema/locale/en/LC_MESSAGES/xmlschema.mo
--rw-rw-r--   0 brunato   (1000) brunato   (1000)    64464 2022-05-20 20:00:14.000000 xmlschema-2.2.3/xmlschema/locale/en/LC_MESSAGES/xmlschema.po
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-04-14 13:52:42.384139 xmlschema-2.2.3/xmlschema/locale/it/
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-04-14 13:52:42.456140 xmlschema-2.2.3/xmlschema/locale/it/LC_MESSAGES/
--rw-rw-r--   0 brunato   (1000) brunato   (1000)    47535 2022-05-20 20:00:14.000000 xmlschema-2.2.3/xmlschema/locale/it/LC_MESSAGES/xmlschema.mo
--rw-rw-r--   0 brunato   (1000) brunato   (1000)    67361 2022-05-20 20:00:14.000000 xmlschema-2.2.3/xmlschema/locale/it/LC_MESSAGES/xmlschema.po
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-04-14 13:52:42.385140 xmlschema-2.2.3/xmlschema/locale/ru/
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-04-14 13:52:42.457140 xmlschema-2.2.3/xmlschema/locale/ru/LC_MESSAGES/
--rw-rw-r--   0 brunato   (1000) brunato   (1000)    60295 2022-06-11 14:29:39.000000 xmlschema-2.2.3/xmlschema/locale/ru/LC_MESSAGES/xmlschema.mo
--rw-rw-r--   0 brunato   (1000) brunato   (1000)    79497 2022-06-11 14:29:39.000000 xmlschema-2.2.3/xmlschema/locale/ru/LC_MESSAGES/xmlschema.po
--rw-r--r--   0 brunato   (1000) brunato   (1000)     8827 2020-12-23 12:38:37.000000 xmlschema-2.2.3/xmlschema/names.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)     9907 2023-02-04 20:00:06.000000 xmlschema-2.2.3/xmlschema/namespaces.py
--rw-rw-r--   0 brunato   (1000) brunato   (1000)        0 2021-09-02 10:52:43.000000 xmlschema-2.2.3/xmlschema/py.typed
--rw-r--r--   0 brunato   (1000) brunato   (1000)    55658 2023-04-14 13:49:05.000000 xmlschema-2.2.3/xmlschema/resources.py
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-04-14 13:52:42.386139 xmlschema-2.2.3/xmlschema/schemas/
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-04-14 13:52:42.457140 xmlschema-2.2.3/xmlschema/schemas/HFP/
--rw-r--r--   0 brunato   (1000) brunato   (1000)     1534 2020-11-08 22:15:33.000000 xmlschema-2.2.3/xmlschema/schemas/HFP/XMLSchema-hasFacetAndProperty_minimal.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-04-14 13:52:42.457140 xmlschema-2.2.3/xmlschema/schemas/VC/
--rw-r--r--   0 brunato   (1000) brunato   (1000)      984 2020-11-08 22:15:33.000000 xmlschema-2.2.3/xmlschema/schemas/VC/XMLSchema-versioning.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-04-14 13:52:42.458140 xmlschema-2.2.3/xmlschema/schemas/WSDL/
--rw-r--r--   0 brunato   (1000) brunato   (1000)    19204 2020-11-08 22:15:33.000000 xmlschema-2.2.3/xmlschema/schemas/WSDL/soap-encoding.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)     6061 2020-11-08 22:15:33.000000 xmlschema-2.2.3/xmlschema/schemas/WSDL/soap-envelope.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)     6005 2020-11-08 22:15:33.000000 xmlschema-2.2.3/xmlschema/schemas/WSDL/wsdl-soap.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)    11900 2020-11-08 22:15:33.000000 xmlschema-2.2.3/xmlschema/schemas/WSDL/wsdl.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-04-14 13:52:42.458140 xmlschema-2.2.3/xmlschema/schemas/XHTML/
--rw-r--r--   0 brunato   (1000) brunato   (1000)    65477 2020-11-08 22:15:33.000000 xmlschema-2.2.3/xmlschema/schemas/XHTML/xhtml1-strict.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-04-14 13:52:42.459140 xmlschema-2.2.3/xmlschema/schemas/XLINK/
--rw-r--r--   0 brunato   (1000) brunato   (1000)     8051 2020-11-08 22:15:33.000000 xmlschema-2.2.3/xmlschema/schemas/XLINK/xlink.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-04-14 13:52:42.459140 xmlschema-2.2.3/xmlschema/schemas/XML/
--rw-r--r--   0 brunato   (1000) brunato   (1000)     1277 2020-11-08 22:15:33.000000 xmlschema-2.2.3/xmlschema/schemas/XML/xml_minimal.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-04-14 13:52:42.459140 xmlschema-2.2.3/xmlschema/schemas/XSD_1.0/
--rw-rw-r--   0 brunato   (1000) brunato   (1000)    88033 2022-05-20 16:16:20.000000 xmlschema-2.2.3/xmlschema/schemas/XSD_1.0/XMLSchema.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)    44301 2020-11-08 22:15:33.000000 xmlschema-2.2.3/xmlschema/schemas/XSD_1.0/datatypes.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-04-14 13:52:42.460140 xmlschema-2.2.3/xmlschema/schemas/XSD_1.1/
--rw-r--r--   0 brunato   (1000) brunato   (1000)    67728 2022-09-25 07:58:42.000000 xmlschema-2.2.3/xmlschema/schemas/XSD_1.1/XMLSchema.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)    17497 2020-11-08 22:15:33.000000 xmlschema-2.2.3/xmlschema/schemas/XSD_1.1/datatypes.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)     3767 2022-09-12 09:59:59.000000 xmlschema-2.2.3/xmlschema/schemas/XSD_1.1/xsd11-extra.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-04-14 13:52:42.460140 xmlschema-2.2.3/xmlschema/schemas/XSI/
--rw-r--r--   0 brunato   (1000) brunato   (1000)      385 2020-11-08 22:15:33.000000 xmlschema-2.2.3/xmlschema/schemas/XSI/XMLSchema-instance_minimal.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-04-14 13:52:42.462140 xmlschema-2.2.3/xmlschema/testing/
--rw-rw-r--   0 brunato   (1000) brunato   (1000)     2109 2022-03-07 13:26:41.000000 xmlschema-2.2.3/xmlschema/testing/__init__.py
--rw-rw-r--   0 brunato   (1000) brunato   (1000)    29735 2022-07-18 14:19:15.000000 xmlschema-2.2.3/xmlschema/testing/_builders.py
--rw-rw-r--   0 brunato   (1000) brunato   (1000)     7943 2022-07-18 14:19:15.000000 xmlschema-2.2.3/xmlschema/testing/_case_class.py
--rw-rw-r--   0 brunato   (1000) brunato   (1000)     9436 2022-03-07 13:26:41.000000 xmlschema-2.2.3/xmlschema/testing/_factory.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)     6911 2022-09-08 10:16:11.000000 xmlschema-2.2.3/xmlschema/testing/_helpers.py
--rw-rw-r--   0 brunato   (1000) brunato   (1000)     4884 2022-03-07 13:26:41.000000 xmlschema-2.2.3/xmlschema/testing/_observers.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)     2072 2023-02-11 10:41:50.000000 xmlschema-2.2.3/xmlschema/translation.py
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-04-14 13:52:42.465140 xmlschema-2.2.3/xmlschema/validators/
--rw-rw-r--   0 brunato   (1000) brunato   (1000)     3557 2021-11-11 15:30:24.000000 xmlschema-2.2.3/xmlschema/validators/__init__.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)     6619 2023-03-05 21:16:57.000000 xmlschema-2.2.3/xmlschema/validators/assertions.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    34132 2022-09-24 15:52:22.000000 xmlschema-2.2.3/xmlschema/validators/attributes.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    19881 2022-08-26 15:33:28.000000 xmlschema-2.2.3/xmlschema/validators/builtins.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    46791 2023-03-05 20:30:24.000000 xmlschema-2.2.3/xmlschema/validators/complex_types.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    64166 2023-03-28 06:38:11.000000 xmlschema-2.2.3/xmlschema/validators/elements.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    14970 2023-03-05 21:16:57.000000 xmlschema-2.2.3/xmlschema/validators/exceptions.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    31723 2023-03-05 21:16:57.000000 xmlschema-2.2.3/xmlschema/validators/facets.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    33050 2023-04-14 13:49:05.000000 xmlschema-2.2.3/xmlschema/validators/global_maps.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    61540 2023-04-14 13:49:05.000000 xmlschema-2.2.3/xmlschema/validators/groups.py
--rw-rw-r--   0 brunato   (1000) brunato   (1000)     6655 2022-05-20 16:16:20.000000 xmlschema-2.2.3/xmlschema/validators/helpers.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    18740 2023-03-05 21:16:57.000000 xmlschema-2.2.3/xmlschema/validators/identities.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    23474 2023-04-14 13:49:05.000000 xmlschema-2.2.3/xmlschema/validators/models.py
--rw-rw-r--   0 brunato   (1000) brunato   (1000)     1611 2022-05-20 20:00:15.000000 xmlschema-2.2.3/xmlschema/validators/notations.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)     6627 2022-09-08 10:16:11.000000 xmlschema-2.2.3/xmlschema/validators/particles.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)   103598 2023-02-06 06:20:42.000000 xmlschema-2.2.3/xmlschema/validators/schemas.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    61468 2023-02-06 06:20:42.000000 xmlschema-2.2.3/xmlschema/validators/simple_types.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    38290 2022-09-25 07:58:42.000000 xmlschema-2.2.3/xmlschema/validators/wildcards.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    41151 2023-03-05 21:16:57.000000 xmlschema-2.2.3/xmlschema/validators/xsdbase.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    13135 2023-02-11 10:41:50.000000 xmlschema-2.2.3/xmlschema/xpath.py
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-04-14 13:52:42.453140 xmlschema-2.2.3/xmlschema.egg-info/
--rw-rw-r--   0 brunato   (1000) brunato   (1000)     7377 2023-04-14 13:52:42.000000 xmlschema-2.2.3/xmlschema.egg-info/PKG-INFO
--rw-rw-r--   0 brunato   (1000) brunato   (1000)    16938 2023-04-14 13:52:42.000000 xmlschema-2.2.3/xmlschema.egg-info/SOURCES.txt
--rw-rw-r--   0 brunato   (1000) brunato   (1000)        1 2023-04-14 13:52:42.000000 xmlschema-2.2.3/xmlschema.egg-info/dependency_links.txt
--rw-rw-r--   0 brunato   (1000) brunato   (1000)      150 2023-04-14 13:52:42.000000 xmlschema-2.2.3/xmlschema.egg-info/entry_points.txt
--rw-rw-r--   0 brunato   (1000) brunato   (1000)      256 2023-04-14 13:52:42.000000 xmlschema-2.2.3/xmlschema.egg-info/requires.txt
--rw-rw-r--   0 brunato   (1000) brunato   (1000)       10 2023-04-14 13:52:42.000000 xmlschema-2.2.3/xmlschema.egg-info/top_level.txt
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-05-18 20:19:54.688786 xmlschema-2.3.0/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      235 2023-03-05 21:16:57.000000 xmlschema-2.3.0/.coveragerc
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    25053 2023-05-18 20:18:16.000000 xmlschema-2.3.0/CHANGELOG.rst
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     1131 2022-09-26 10:47:27.000000 xmlschema-2.3.0/LICENSE
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      330 2023-03-05 20:30:24.000000 xmlschema-2.3.0/MANIFEST.in
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     7377 2023-05-18 20:19:54.688786 xmlschema-2.3.0/PKG-INFO
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     6045 2022-08-26 15:33:28.000000 xmlschema-2.3.0/README.rst
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-05-18 20:19:54.545786 xmlschema-2.3.0/doc/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      606 2018-09-23 09:23:56.000000 xmlschema-2.3.0/doc/Makefile
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    11613 2022-10-01 13:42:01.000000 xmlschema-2.3.0/doc/api.rst
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)    11273 2021-08-02 14:12:17.000000 xmlschema-2.3.0/doc/components.rst
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     5474 2023-05-18 20:18:16.000000 xmlschema-2.3.0/doc/conf.py
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)     5499 2022-06-24 14:13:22.000000 xmlschema-2.3.0/doc/converters.rst
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)     4841 2022-06-24 14:13:22.000000 xmlschema-2.3.0/doc/extras.rst
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)     7488 2022-06-24 14:13:22.000000 xmlschema-2.3.0/doc/features.rst
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      214 2021-02-05 09:05:33.000000 xmlschema-2.3.0/doc/index.rst
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      468 2020-05-28 20:30:12.000000 xmlschema-2.3.0/doc/intro.rst
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     5921 2021-04-11 20:19:21.000000 xmlschema-2.3.0/doc/testing.rst
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    27730 2022-10-01 13:42:01.000000 xmlschema-2.3.0/doc/usage.rst
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)       31 2022-03-07 13:26:41.000000 xmlschema-2.3.0/mypy.ini
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      214 2023-05-18 20:18:16.000000 xmlschema-2.3.0/requirements-dev.txt
+-rw-r--r--   0 brunato   (1000) brunato   (1000)       38 2023-05-18 20:19:54.688786 xmlschema-2.3.0/setup.cfg
+-rwxr-xr-x   0 brunato   (1000) brunato   (1000)     2764 2023-05-18 20:18:16.000000 xmlschema-2.3.0/setup.py
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-05-18 20:19:54.552785 xmlschema-2.3.0/tests/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)        0 2020-12-03 21:49:59.000000 xmlschema-2.3.0/tests/__init__.py
+-rwxrwxr-x   0 brunato   (1000) brunato   (1000)     4934 2022-07-18 14:19:15.000000 xmlschema-2.3.0/tests/check_memory.py
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-05-18 20:19:54.529785 xmlschema-2.3.0/tests/templates/
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-05-18 20:19:54.552785 xmlschema-2.3.0/tests/templates/demo/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)       39 2021-02-05 09:05:33.000000 xmlschema-2.3.0/tests/templates/demo/demo_type_filter_test.jinja
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-05-18 20:19:54.555786 xmlschema-2.3.0/tests/templates/filters/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)       34 2021-02-05 09:05:33.000000 xmlschema-2.3.0/tests/templates/filters/name_filter_test.jinja
+-rw-r--r--   0 brunato   (1000) brunato   (1000)       39 2021-02-05 09:05:33.000000 xmlschema-2.3.0/tests/templates/filters/namespace_filter_test.jinja
+-rw-r--r--   0 brunato   (1000) brunato   (1000)       42 2021-02-05 09:05:33.000000 xmlschema-2.3.0/tests/templates/filters/python_type_filter_test.jinja
+-rw-r--r--   0 brunato   (1000) brunato   (1000)       35 2021-02-05 09:05:33.000000 xmlschema-2.3.0/tests/templates/filters/qname_filter_test.jinja
+-rw-r--r--   0 brunato   (1000) brunato   (1000)       87 2021-02-05 09:05:33.000000 xmlschema-2.3.0/tests/templates/filters/sort_types_filter_test.jinja
+-rw-r--r--   0 brunato   (1000) brunato   (1000)       39 2021-04-03 19:09:14.000000 xmlschema-2.3.0/tests/templates/filters/type_name_filter_test.jinja
+-rw-r--r--   0 brunato   (1000) brunato   (1000)       40 2021-02-05 09:05:33.000000 xmlschema-2.3.0/tests/templates/filters/type_qname_filter_test.jinja
+-rw-r--r--   0 brunato   (1000) brunato   (1000)       37 2021-04-05 21:38:16.000000 xmlschema-2.3.0/tests/templates/filters/unknown_filter_test.jinja
+-rw-r--r--   0 brunato   (1000) brunato   (1000)       42 2021-02-05 09:05:33.000000 xmlschema-2.3.0/tests/templates/filters/wrong-template.jinja
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)     3484 2022-07-18 14:19:15.000000 xmlschema-2.3.0/tests/test_all.py
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-05-18 20:19:54.555786 xmlschema-2.3.0/tests/test_cases/
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-05-18 20:19:54.529785 xmlschema-2.3.0/tests/test_cases/examples/
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-05-18 20:19:54.558786 xmlschema-2.3.0/tests/test_cases/examples/collection/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      925 2020-05-28 20:30:12.000000 xmlschema-2.3.0/tests/test_cases/examples/collection/collection-1_error.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      884 2022-08-26 15:33:28.000000 xmlschema-2.3.0/tests/test_cases/examples/collection/collection-default.xml
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)      798 2023-05-18 20:17:39.000000 xmlschema-2.3.0/tests/test_cases/examples/collection/collection.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      923 2020-05-28 20:30:12.000000 xmlschema-2.3.0/tests/test_cases/examples/collection/collection.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     1599 2020-01-23 20:05:17.000000 xmlschema-2.3.0/tests/test_cases/examples/collection/collection.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      941 2020-01-23 20:05:17.000000 xmlschema-2.3.0/tests/test_cases/examples/collection/collection2.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     1736 2020-01-23 20:05:17.000000 xmlschema-2.3.0/tests/test_cases/examples/collection/collection2.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      960 2020-01-23 20:05:17.000000 xmlschema-2.3.0/tests/test_cases/examples/collection/collection3.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     1938 2020-01-23 20:05:17.000000 xmlschema-2.3.0/tests/test_cases/examples/collection/collection3.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     1082 2020-01-23 20:05:17.000000 xmlschema-2.3.0/tests/test_cases/examples/collection/collection3bis.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     1979 2020-01-23 20:05:17.000000 xmlschema-2.3.0/tests/test_cases/examples/collection/collection3bis.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     1364 2020-01-23 20:05:17.000000 xmlschema-2.3.0/tests/test_cases/examples/collection/collection4.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     1743 2020-11-08 22:15:33.000000 xmlschema-2.3.0/tests/test_cases/examples/collection/collection4.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     1658 2022-08-26 15:33:28.000000 xmlschema-2.3.0/tests/test_cases/examples/collection/collection5.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-05-18 20:19:54.559786 xmlschema-2.3.0/tests/test_cases/examples/stockquote/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     1039 2020-11-08 22:15:33.000000 xmlschema-2.3.0/tests/test_cases/examples/stockquote/stockquote.wsdl
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      664 2020-11-08 22:15:33.000000 xmlschema-2.3.0/tests/test_cases/examples/stockquote/stockquote.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     1230 2020-11-08 22:15:33.000000 xmlschema-2.3.0/tests/test_cases/examples/stockquote/stockquoteservice.wsdl
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-05-18 20:19:54.568786 xmlschema-2.3.0/tests/test_cases/examples/vehicles/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      471 2020-01-23 20:05:17.000000 xmlschema-2.3.0/tests/test_cases/examples/vehicles/bikes.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      469 2020-01-23 20:05:17.000000 xmlschema-2.3.0/tests/test_cases/examples/vehicles/cars.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      595 2022-10-01 13:42:01.000000 xmlschema-2.3.0/tests/test_cases/examples/vehicles/invalid.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      361 2020-01-23 20:05:17.000000 xmlschema-2.3.0/tests/test_cases/examples/vehicles/types.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      386 2020-05-02 09:28:30.000000 xmlschema-2.3.0/tests/test_cases/examples/vehicles/vehicles-1_error.json
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      468 2020-01-23 20:05:17.000000 xmlschema-2.3.0/tests/test_cases/examples/vehicles/vehicles-1_error.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      475 2020-01-23 20:05:17.000000 xmlschema-2.3.0/tests/test_cases/examples/vehicles/vehicles-2_errors.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      386 2020-05-02 09:28:33.000000 xmlschema-2.3.0/tests/test_cases/examples/vehicles/vehicles-3_errors.json
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      491 2020-01-23 20:05:17.000000 xmlschema-2.3.0/tests/test_cases/examples/vehicles/vehicles-3_errors.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      557 2020-01-23 20:05:17.000000 xmlschema-2.3.0/tests/test_cases/examples/vehicles/vehicles-max.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     1666 2020-11-15 16:10:20.000000 xmlschema-2.3.0/tests/test_cases/examples/vehicles/vehicles-schemas.xsd.zip
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      497 2020-01-23 20:05:17.000000 xmlschema-2.3.0/tests/test_cases/examples/vehicles/vehicles.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      543 2020-01-23 20:05:17.000000 xmlschema-2.3.0/tests/test_cases/examples/vehicles/vehicles.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      346 2020-05-02 09:28:32.000000 xmlschema-2.3.0/tests/test_cases/examples/vehicles/vehicles2.json
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      432 2020-01-23 20:05:17.000000 xmlschema-2.3.0/tests/test_cases/examples/vehicles/vehicles2.xml
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-05-18 20:19:54.530785 xmlschema-2.3.0/tests/test_cases/features/
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-05-18 20:19:54.569786 xmlschema-2.3.0/tests/test_cases/features/attributes/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      688 2020-01-23 20:05:17.000000 xmlschema-2.3.0/tests/test_cases/features/attributes/default_attributes-missing_group.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      910 2020-01-23 20:05:17.000000 xmlschema-2.3.0/tests/test_cases/features/attributes/default_attributes.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-05-18 20:19:54.570786 xmlschema-2.3.0/tests/test_cases/features/builtins/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      584 2020-01-23 20:05:17.000000 xmlschema-2.3.0/tests/test_cases/features/builtins/builtins.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      601 2020-01-23 20:05:17.000000 xmlschema-2.3.0/tests/test_cases/features/builtins/builtins.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-05-18 20:19:54.572786 xmlschema-2.3.0/tests/test_cases/features/decoder/
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)      781 2022-05-20 20:00:14.000000 xmlschema-2.3.0/tests/test_cases/features/decoder/data.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      725 2020-01-23 20:05:17.000000 xmlschema-2.3.0/tests/test_cases/features/decoder/data2.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      608 2021-04-01 09:07:37.000000 xmlschema-2.3.0/tests/test_cases/features/decoder/data3.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      480 2021-04-05 21:38:16.000000 xmlschema-2.3.0/tests/test_cases/features/decoder/data4-mixed.xml
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)      691 2021-12-08 19:41:39.000000 xmlschema-2.3.0/tests/test_cases/features/decoder/long-sequence-1.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      727 2021-04-05 21:38:16.000000 xmlschema-2.3.0/tests/test_cases/features/decoder/mixed-content.xsd
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)     5913 2022-05-20 20:00:14.000000 xmlschema-2.3.0/tests/test_cases/features/decoder/simple-types.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-05-18 20:19:54.575786 xmlschema-2.3.0/tests/test_cases/features/derivations/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     1956 2020-01-23 20:05:17.000000 xmlschema-2.3.0/tests/test_cases/features/derivations/complex-extensions.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      662 2020-01-23 20:05:17.000000 xmlschema-2.3.0/tests/test_cases/features/derivations/complex-with-simple-content-restriction.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     3949 2023-05-18 20:18:16.000000 xmlschema-2.3.0/tests/test_cases/features/derivations/complex11-restrictions.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      599 2023-05-18 20:18:16.000000 xmlschema-2.3.0/tests/test_cases/features/derivations/invalid-enumeration-restriction.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     2051 2023-05-18 20:18:16.000000 xmlschema-2.3.0/tests/test_cases/features/derivations/invalid-restrictions1.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     1027 2023-05-18 20:18:16.000000 xmlschema-2.3.0/tests/test_cases/features/derivations/invalid-restrictions2.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      322 2020-01-23 20:05:17.000000 xmlschema-2.3.0/tests/test_cases/features/derivations/list_types.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      675 2020-01-23 20:05:17.000000 xmlschema-2.3.0/tests/test_cases/features/derivations/list_types.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-05-18 20:19:54.577786 xmlschema-2.3.0/tests/test_cases/features/elements/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      154 2020-01-23 20:05:17.000000 xmlschema-2.3.0/tests/test_cases/features/elements/test_alternatives-1.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     1487 2020-01-23 20:05:17.000000 xmlschema-2.3.0/tests/test_cases/features/elements/type_alternatives-no-ns.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     1543 2020-01-23 20:05:17.000000 xmlschema-2.3.0/tests/test_cases/features/elements/type_alternatives.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-05-18 20:19:54.583786 xmlschema-2.3.0/tests/test_cases/features/models/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     5143 2020-01-23 20:05:17.000000 xmlschema-2.3.0/tests/test_cases/features/models/billion_laughs_model.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      301 2020-01-23 20:05:17.000000 xmlschema-2.3.0/tests/test_cases/features/models/circular_model.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      215 2020-01-23 20:05:17.000000 xmlschema-2.3.0/tests/test_cases/features/models/illegal-attributes.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      647 2020-01-23 20:05:17.000000 xmlschema-2.3.0/tests/test_cases/features/models/illegal-declarations.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      523 2020-01-23 20:05:17.000000 xmlschema-2.3.0/tests/test_cases/features/models/illegal-occurs.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     1192 2020-01-23 20:05:17.000000 xmlschema-2.3.0/tests/test_cases/features/models/invalid_models1.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     1541 2020-01-23 20:05:17.000000 xmlschema-2.3.0/tests/test_cases/features/models/invalid_models2.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      306 2020-01-23 20:05:17.000000 xmlschema-2.3.0/tests/test_cases/features/models/model1.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     4794 2020-04-28 13:28:56.000000 xmlschema-2.3.0/tests/test_cases/features/models/models.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      205 2020-01-23 20:05:17.000000 xmlschema-2.3.0/tests/test_cases/features/models/other-ns.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      760 2020-01-23 20:05:17.000000 xmlschema-2.3.0/tests/test_cases/features/models/recursive-groups.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     1062 2020-04-28 13:28:56.000000 xmlschema-2.3.0/tests/test_cases/features/models/valid_model1.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-05-18 20:19:54.591786 xmlschema-2.3.0/tests/test_cases/features/namespaces/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      151 2020-01-23 20:05:17.000000 xmlschema-2.3.0/tests/test_cases/features/namespaces/chameleon1.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      205 2020-01-23 20:05:17.000000 xmlschema-2.3.0/tests/test_cases/features/namespaces/chameleon2.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      272 2020-01-23 20:05:17.000000 xmlschema-2.3.0/tests/test_cases/features/namespaces/chameleon3.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      435 2020-01-23 20:05:17.000000 xmlschema-2.3.0/tests/test_cases/features/namespaces/default_ns_invalid.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      481 2020-01-23 20:05:17.000000 xmlschema-2.3.0/tests/test_cases/features/namespaces/default_ns_valid1.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      375 2020-01-23 20:05:17.000000 xmlschema-2.3.0/tests/test_cases/features/namespaces/default_ns_valid2.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      566 2020-01-23 20:05:17.000000 xmlschema-2.3.0/tests/test_cases/features/namespaces/import-case1.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      566 2020-01-23 20:05:17.000000 xmlschema-2.3.0/tests/test_cases/features/namespaces/import-case2.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      436 2020-01-23 20:05:17.000000 xmlschema-2.3.0/tests/test_cases/features/namespaces/import-case3.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      241 2020-01-23 20:05:17.000000 xmlschema-2.3.0/tests/test_cases/features/namespaces/import-case4-1.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      316 2020-01-23 20:05:17.000000 xmlschema-2.3.0/tests/test_cases/features/namespaces/import-case4-2.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      720 2020-01-23 20:05:17.000000 xmlschema-2.3.0/tests/test_cases/features/namespaces/import-case4a.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      720 2020-01-23 20:05:17.000000 xmlschema-2.3.0/tests/test_cases/features/namespaces/import-case4b.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      365 2022-09-08 10:16:11.000000 xmlschema-2.3.0/tests/test_cases/features/namespaces/import-case5a.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      377 2022-09-08 10:16:11.000000 xmlschema-2.3.0/tests/test_cases/features/namespaces/import-case5b.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      379 2022-09-08 10:16:11.000000 xmlschema-2.3.0/tests/test_cases/features/namespaces/import-case5c.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      504 2020-01-23 20:05:17.000000 xmlschema-2.3.0/tests/test_cases/features/namespaces/include-case1.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      435 2020-01-23 20:05:17.000000 xmlschema-2.3.0/tests/test_cases/features/namespaces/include-case1bis.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      590 2020-01-23 20:05:17.000000 xmlschema-2.3.0/tests/test_cases/features/namespaces/include-case2.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      541 2020-01-23 20:05:17.000000 xmlschema-2.3.0/tests/test_cases/features/namespaces/include-case2bis.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      516 2020-01-23 20:05:17.000000 xmlschema-2.3.0/tests/test_cases/features/namespaces/include-case3.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      490 2020-01-23 20:05:17.000000 xmlschema-2.3.0/tests/test_cases/features/namespaces/include-case4.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      520 2020-01-23 20:05:17.000000 xmlschema-2.3.0/tests/test_cases/features/namespaces/include-case5.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      499 2020-01-23 20:05:17.000000 xmlschema-2.3.0/tests/test_cases/features/namespaces/include-case6.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      261 2020-01-23 20:05:17.000000 xmlschema-2.3.0/tests/test_cases/features/namespaces/included3-valid.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      257 2020-01-23 20:05:17.000000 xmlschema-2.3.0/tests/test_cases/features/namespaces/included4-invalid.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      269 2020-01-23 20:05:17.000000 xmlschema-2.3.0/tests/test_cases/features/namespaces/included5-valid.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      211 2020-01-23 20:05:17.000000 xmlschema-2.3.0/tests/test_cases/features/namespaces/included6-invalid.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-05-18 20:19:54.592786 xmlschema-2.3.0/tests/test_cases/features/patterns/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      833 2020-01-23 20:05:17.000000 xmlschema-2.3.0/tests/test_cases/features/patterns/patterns.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     3276 2020-04-07 21:42:10.000000 xmlschema-2.3.0/tests/test_cases/features/patterns/patterns.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-05-18 20:19:54.594786 xmlschema-2.3.0/tests/test_cases/features/wsdl/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     2089 2023-05-18 20:18:16.000000 xmlschema-2.3.0/tests/test_cases/features/wsdl/wsdl11_example3.wsdl
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     1477 2023-05-18 20:18:16.000000 xmlschema-2.3.0/tests/test_cases/features/wsdl/wsdl11_example3_no_types.wsdl
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      376 2023-05-18 20:18:16.000000 xmlschema-2.3.0/tests/test_cases/features/wsdl/wsdl11_example3_types.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     1954 2020-11-08 22:15:33.000000 xmlschema-2.3.0/tests/test_cases/features/wsdl/wsdl11_example3_valid.wsdl
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     2132 2020-11-08 22:15:33.000000 xmlschema-2.3.0/tests/test_cases/features/wsdl/wsdl11_example4.wsdl
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     1962 2020-11-08 22:15:33.000000 xmlschema-2.3.0/tests/test_cases/features/wsdl/wsdl11_example4_valid.wsdl
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     2996 2020-11-08 22:15:33.000000 xmlschema-2.3.0/tests/test_cases/features/wsdl/wsdl11_example5.wsdl
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     3163 2020-11-08 22:15:33.000000 xmlschema-2.3.0/tests/test_cases/features/wsdl/wsdl11_example5_valid.wsdl
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     3414 2020-11-08 22:15:33.000000 xmlschema-2.3.0/tests/test_cases/features/wsdl/wsdl11_example5_with_fault.wsdl
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-05-18 20:19:54.536785 xmlschema-2.3.0/tests/test_cases/issues/
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-05-18 20:19:54.594786 xmlschema-2.3.0/tests/test_cases/issues/issue_008/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      252 2020-01-23 20:05:17.000000 xmlschema-2.3.0/tests/test_cases/issues/issue_008/issue_008.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      533 2020-01-23 20:05:17.000000 xmlschema-2.3.0/tests/test_cases/issues/issue_008/issue_008.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-05-18 20:19:54.594786 xmlschema-2.3.0/tests/test_cases/issues/issue_009/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      303 2020-01-23 20:05:17.000000 xmlschema-2.3.0/tests/test_cases/issues/issue_009/issue_009.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-05-18 20:19:54.596786 xmlschema-2.3.0/tests/test_cases/issues/issue_013/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      186 2020-01-23 20:05:17.000000 xmlschema-2.3.0/tests/test_cases/issues/issue_013/issue_013-1.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      731 2020-01-23 20:05:17.000000 xmlschema-2.3.0/tests/test_cases/issues/issue_013/issue_013-1.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      235 2020-01-23 20:05:17.000000 xmlschema-2.3.0/tests/test_cases/issues/issue_013/issue_013-2.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      184 2020-01-23 20:05:17.000000 xmlschema-2.3.0/tests/test_cases/issues/issue_013/issue_013.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      801 2020-01-23 20:05:17.000000 xmlschema-2.3.0/tests/test_cases/issues/issue_013/issue_013.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-05-18 20:19:54.596786 xmlschema-2.3.0/tests/test_cases/issues/issue_014/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      556 2020-01-23 20:05:17.000000 xmlschema-2.3.0/tests/test_cases/issues/issue_014/issue014.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-05-18 20:19:54.597786 xmlschema-2.3.0/tests/test_cases/issues/issue_018/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      193 2020-01-23 20:05:17.000000 xmlschema-2.3.0/tests/test_cases/issues/issue_018/issue_018-1.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     1449 2020-01-23 20:05:17.000000 xmlschema-2.3.0/tests/test_cases/issues/issue_018/issue_018.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-05-18 20:19:54.600786 xmlschema-2.3.0/tests/test_cases/issues/issue_022/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     1048 2020-01-23 20:05:17.000000 xmlschema-2.3.0/tests/test_cases/issues/issue_022/README.md
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      130 2020-01-23 20:05:17.000000 xmlschema-2.3.0/tests/test_cases/issues/issue_022/xml_string_1.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      208 2020-01-23 20:05:17.000000 xmlschema-2.3.0/tests/test_cases/issues/issue_022/xml_string_2.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      666 2020-01-23 20:05:17.000000 xmlschema-2.3.0/tests/test_cases/issues/issue_022/xsd_string.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-05-18 20:19:54.601786 xmlschema-2.3.0/tests/test_cases/issues/issue_026/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      229 2020-01-23 20:05:17.000000 xmlschema-2.3.0/tests/test_cases/issues/issue_026/issue_026-1.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      224 2020-01-23 20:05:17.000000 xmlschema-2.3.0/tests/test_cases/issues/issue_026/issue_026-2.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      213 2020-01-23 20:05:17.000000 xmlschema-2.3.0/tests/test_cases/issues/issue_026/issue_026-3.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      664 2020-01-23 20:05:17.000000 xmlschema-2.3.0/tests/test_cases/issues/issue_026/issue_026.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-05-18 20:19:54.602786 xmlschema-2.3.0/tests/test_cases/issues/issue_028/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      203 2020-01-23 20:05:17.000000 xmlschema-2.3.0/tests/test_cases/issues/issue_028/issue_028-1.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      181 2020-01-23 20:05:17.000000 xmlschema-2.3.0/tests/test_cases/issues/issue_028/issue_028-2.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      353 2020-01-23 20:05:17.000000 xmlschema-2.3.0/tests/test_cases/issues/issue_028/issue_028.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-05-18 20:19:54.603786 xmlschema-2.3.0/tests/test_cases/issues/issue_029/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      203 2020-01-23 20:05:17.000000 xmlschema-2.3.0/tests/test_cases/issues/issue_029/issue_029-1.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      159 2020-01-23 20:05:17.000000 xmlschema-2.3.0/tests/test_cases/issues/issue_029/issue_029-2.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      181 2020-01-23 20:05:17.000000 xmlschema-2.3.0/tests/test_cases/issues/issue_029/issue_029-3.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      363 2020-01-23 20:05:17.000000 xmlschema-2.3.0/tests/test_cases/issues/issue_029/issue_029.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-05-18 20:19:54.604786 xmlschema-2.3.0/tests/test_cases/issues/issue_035/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      869 2020-01-23 20:05:17.000000 xmlschema-2.3.0/tests/test_cases/issues/issue_035/dates.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     1081 2020-01-23 20:05:17.000000 xmlschema-2.3.0/tests/test_cases/issues/issue_035/dates.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-05-18 20:19:54.604786 xmlschema-2.3.0/tests/test_cases/issues/issue_041/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      247 2020-01-23 20:05:17.000000 xmlschema-2.3.0/tests/test_cases/issues/issue_041/issue_041.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      708 2020-01-23 20:05:17.000000 xmlschema-2.3.0/tests/test_cases/issues/issue_041/issue_041.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-05-18 20:19:54.604786 xmlschema-2.3.0/tests/test_cases/issues/issue_045/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      275 2020-01-23 20:05:17.000000 xmlschema-2.3.0/tests/test_cases/issues/issue_045/issue_045.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-05-18 20:19:54.605786 xmlschema-2.3.0/tests/test_cases/issues/issue_046/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      354 2020-01-23 20:05:17.000000 xmlschema-2.3.0/tests/test_cases/issues/issue_046/issue_046.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      419 2020-01-23 20:05:17.000000 xmlschema-2.3.0/tests/test_cases/issues/issue_046/issue_046.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-05-18 20:19:54.605786 xmlschema-2.3.0/tests/test_cases/issues/issue_051/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      331 2020-01-23 20:05:17.000000 xmlschema-2.3.0/tests/test_cases/issues/issue_051/issue_051.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      824 2020-01-23 20:05:17.000000 xmlschema-2.3.0/tests/test_cases/issues/issue_051/issue_051.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-05-18 20:19:54.606786 xmlschema-2.3.0/tests/test_cases/issues/issue_073/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      327 2020-01-23 20:05:17.000000 xmlschema-2.3.0/tests/test_cases/issues/issue_073/issue_073-1.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      362 2020-01-23 20:05:17.000000 xmlschema-2.3.0/tests/test_cases/issues/issue_073/issue_073-2.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      685 2020-01-23 20:05:17.000000 xmlschema-2.3.0/tests/test_cases/issues/issue_073/issue_073.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-05-18 20:19:54.607786 xmlschema-2.3.0/tests/test_cases/issues/issue_086/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      403 2020-01-23 20:05:17.000000 xmlschema-2.3.0/tests/test_cases/issues/issue_086/issue_086-1.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      403 2020-01-23 20:05:17.000000 xmlschema-2.3.0/tests/test_cases/issues/issue_086/issue_086-2.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     1328 2020-01-23 20:05:17.000000 xmlschema-2.3.0/tests/test_cases/issues/issue_086/issue_086.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-05-18 20:19:54.607786 xmlschema-2.3.0/tests/test_cases/issues/issue_105/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      515 2020-01-23 20:05:17.000000 xmlschema-2.3.0/tests/test_cases/issues/issue_105/issue_105.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-05-18 20:19:54.608786 xmlschema-2.3.0/tests/test_cases/issues/issue_111/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      698 2020-01-23 20:05:17.000000 xmlschema-2.3.0/tests/test_cases/issues/issue_111/issue_111.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      590 2020-01-23 20:05:17.000000 xmlschema-2.3.0/tests/test_cases/issues/issue_111/issue_111_skeleton.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-05-18 20:19:54.609786 xmlschema-2.3.0/tests/test_cases/issues/issue_115/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      620 2020-01-23 20:05:17.000000 xmlschema-2.3.0/tests/test_cases/issues/issue_115/Rotation.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-05-18 20:19:54.610786 xmlschema-2.3.0/tests/test_cases/issues/issue_171/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      535 2020-03-23 16:13:26.000000 xmlschema-2.3.0/tests/test_cases/issues/issue_171/issue_171.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      580 2020-03-23 16:13:26.000000 xmlschema-2.3.0/tests/test_cases/issues/issue_171/issue_171b.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      504 2020-08-14 19:07:25.000000 xmlschema-2.3.0/tests/test_cases/issues/issue_171/issue_171c.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-05-18 20:19:54.611786 xmlschema-2.3.0/tests/test_cases/issues/issue_187/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      666 2020-09-25 15:20:24.000000 xmlschema-2.3.0/tests/test_cases/issues/issue_187/issue_187_1.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      804 2020-09-25 15:20:24.000000 xmlschema-2.3.0/tests/test_cases/issues/issue_187/issue_187_2.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-05-18 20:19:54.611786 xmlschema-2.3.0/tests/test_cases/issues/issue_190/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      109 2020-05-28 20:30:12.000000 xmlschema-2.3.0/tests/test_cases/issues/issue_190/issue_190.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      785 2020-05-28 20:30:12.000000 xmlschema-2.3.0/tests/test_cases/issues/issue_190/issue_190.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-05-18 20:19:54.612786 xmlschema-2.3.0/tests/test_cases/issues/issue_200/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      310 2020-08-14 19:07:25.000000 xmlschema-2.3.0/tests/test_cases/issues/issue_200/issue_200.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      752 2020-08-14 19:07:25.000000 xmlschema-2.3.0/tests/test_cases/issues/issue_200/issue_200.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-05-18 20:19:54.613786 xmlschema-2.3.0/tests/test_cases/issues/issue_203/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      196 2020-09-19 06:08:01.000000 xmlschema-2.3.0/tests/test_cases/issues/issue_203/issue_203.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      960 2020-09-19 06:08:01.000000 xmlschema-2.3.0/tests/test_cases/issues/issue_203/issue_203.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      964 2020-09-19 06:08:01.000000 xmlschema-2.3.0/tests/test_cases/issues/issue_203/issue_203alt.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-05-18 20:19:54.614786 xmlschema-2.3.0/tests/test_cases/issues/issue_204/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      524 2020-09-25 15:20:24.000000 xmlschema-2.3.0/tests/test_cases/issues/issue_204/issue_204.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      172 2020-09-25 15:20:24.000000 xmlschema-2.3.0/tests/test_cases/issues/issue_204/issue_204_1.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      186 2020-09-25 15:20:24.000000 xmlschema-2.3.0/tests/test_cases/issues/issue_204/issue_204_2.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      222 2020-09-25 15:20:24.000000 xmlschema-2.3.0/tests/test_cases/issues/issue_204/issue_204_3.xml
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-05-18 20:19:54.615786 xmlschema-2.3.0/tests/test_cases/issues/issue_208/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      306 2020-11-08 22:15:33.000000 xmlschema-2.3.0/tests/test_cases/issues/issue_208/issue_208.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     1532 2020-11-08 22:15:33.000000 xmlschema-2.3.0/tests/test_cases/issues/issue_208/issue_208.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-05-18 20:19:54.615786 xmlschema-2.3.0/tests/test_cases/issues/issue_222/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)       66 2021-01-24 21:47:47.000000 xmlschema-2.3.0/tests/test_cases/issues/issue_222/issue_222.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      569 2021-01-24 21:47:47.000000 xmlschema-2.3.0/tests/test_cases/issues/issue_222/issue_222.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-05-18 20:19:54.616786 xmlschema-2.3.0/tests/test_cases/issues/issue_223/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)       46 2021-01-24 21:47:47.000000 xmlschema-2.3.0/tests/test_cases/issues/issue_223/issue_223.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      392 2021-03-30 11:13:45.000000 xmlschema-2.3.0/tests/test_cases/issues/issue_223/issue_223.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-05-18 20:19:54.534786 xmlschema-2.3.0/tests/test_cases/issues/issue_237/
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-05-18 20:19:54.617786 xmlschema-2.3.0/tests/test_cases/issues/issue_237/dir1/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      191 2021-04-05 21:38:16.000000 xmlschema-2.3.0/tests/test_cases/issues/issue_237/dir1/issue_237.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     1249 2021-04-05 21:38:16.000000 xmlschema-2.3.0/tests/test_cases/issues/issue_237/dir1/stockquoteservice.wsdl
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-05-18 20:19:54.620786 xmlschema-2.3.0/tests/test_cases/issues/issue_237/dir2/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      141 2021-04-05 21:38:16.000000 xmlschema-2.3.0/tests/test_cases/issues/issue_237/dir2/issue_237a.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      314 2021-04-05 21:38:16.000000 xmlschema-2.3.0/tests/test_cases/issues/issue_237/dir2/issue_237b.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     1041 2021-04-05 21:38:16.000000 xmlschema-2.3.0/tests/test_cases/issues/issue_237/dir2/stockquote.wsdl
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      664 2021-04-05 21:38:16.000000 xmlschema-2.3.0/tests/test_cases/issues/issue_237/dir2/stockquote.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-05-18 20:19:54.620786 xmlschema-2.3.0/tests/test_cases/issues/issue_243/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      283 2021-05-03 11:37:57.000000 xmlschema-2.3.0/tests/test_cases/issues/issue_243/issue_243.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     2063 2021-05-03 11:37:57.000000 xmlschema-2.3.0/tests/test_cases/issues/issue_243/issue_243.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-05-18 20:19:54.621786 xmlschema-2.3.0/tests/test_cases/issues/issue_245/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      757 2021-05-03 11:37:57.000000 xmlschema-2.3.0/tests/test_cases/issues/issue_245/issue_245-valid.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      757 2021-05-03 11:37:57.000000 xmlschema-2.3.0/tests/test_cases/issues/issue_245/issue_245.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     4894 2021-05-03 11:37:57.000000 xmlschema-2.3.0/tests/test_cases/issues/issue_245/issue_245.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-05-18 20:19:54.621786 xmlschema-2.3.0/tests/test_cases/issues/issue_259/
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)     2422 2021-09-02 10:52:43.000000 xmlschema-2.3.0/tests/test_cases/issues/issue_259/issue_259-1.xsd
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)     1432 2021-09-02 10:52:43.000000 xmlschema-2.3.0/tests/test_cases/issues/issue_259/issue_259-2.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-05-18 20:19:54.622786 xmlschema-2.3.0/tests/test_cases/issues/issue_265/
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)     3471 2021-10-20 14:14:48.000000 xmlschema-2.3.0/tests/test_cases/issues/issue_265/issue_265-1.xsd
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)     1411 2021-10-20 14:14:48.000000 xmlschema-2.3.0/tests/test_cases/issues/issue_265/issue_265-2-invalid.xsd
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)      454 2021-10-20 14:14:48.000000 xmlschema-2.3.0/tests/test_cases/issues/issue_265/issue_265-2-override.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-05-18 20:19:54.623786 xmlschema-2.3.0/tests/test_cases/issues/issue_266/
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)      158 2021-10-20 14:14:48.000000 xmlschema-2.3.0/tests/test_cases/issues/issue_266/issue_266-1.xml
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)      538 2021-10-20 14:14:48.000000 xmlschema-2.3.0/tests/test_cases/issues/issue_266/issue_266-1.xsd
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)      158 2021-10-20 14:14:48.000000 xmlschema-2.3.0/tests/test_cases/issues/issue_266/issue_266-2.xml
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)      528 2021-10-20 14:14:48.000000 xmlschema-2.3.0/tests/test_cases/issues/issue_266/issue_266-2.xsd
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)      651 2021-11-11 15:30:24.000000 xmlschema-2.3.0/tests/test_cases/issues/issue_266/issue_266b-1.xsd
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)      551 2021-11-11 15:30:24.000000 xmlschema-2.3.0/tests/test_cases/issues/issue_266/issue_266b-2.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-05-18 20:19:54.624786 xmlschema-2.3.0/tests/test_cases/issues/issue_273/
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)      299 2021-12-08 19:41:39.000000 xmlschema-2.3.0/tests/test_cases/issues/issue_273/issue_273.xml
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)      517 2021-12-08 19:41:39.000000 xmlschema-2.3.0/tests/test_cases/issues/issue_273/issue_273.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-05-18 20:19:54.624786 xmlschema-2.3.0/tests/test_cases/issues/issue_276/
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)      122 2021-12-08 22:11:41.000000 xmlschema-2.3.0/tests/test_cases/issues/issue_276/dummy.xml
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)      495 2021-12-08 22:11:41.000000 xmlschema-2.3.0/tests/test_cases/issues/issue_276/schema.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-05-18 20:19:54.625786 xmlschema-2.3.0/tests/test_cases/issues/issue_298/
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)      114 2022-05-22 16:17:24.000000 xmlschema-2.3.0/tests/test_cases/issues/issue_298/issue_298-1.xml
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)      240 2022-05-22 16:17:24.000000 xmlschema-2.3.0/tests/test_cases/issues/issue_298/issue_298-2.xml
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)      792 2022-05-22 16:17:24.000000 xmlschema-2.3.0/tests/test_cases/issues/issue_298/issue_298.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-05-18 20:19:54.626786 xmlschema-2.3.0/tests/test_cases/issues/issue_306/
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)      881 2022-06-24 14:13:22.000000 xmlschema-2.3.0/tests/test_cases/issues/issue_306/issue_306-alt.xsd
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)      203 2022-06-24 14:13:22.000000 xmlschema-2.3.0/tests/test_cases/issues/issue_306/issue_306-invalid.xml
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)      182 2022-06-24 14:13:22.000000 xmlschema-2.3.0/tests/test_cases/issues/issue_306/issue_306-valid.xml
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)      689 2022-06-24 14:13:22.000000 xmlschema-2.3.0/tests/test_cases/issues/issue_306/issue_306.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-05-18 20:19:54.627786 xmlschema-2.3.0/tests/test_cases/issues/issue_311/
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)      786 2022-07-18 14:19:15.000000 xmlschema-2.3.0/tests/test_cases/issues/issue_311/correct_no_list.xml
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)      788 2022-07-18 14:19:15.000000 xmlschema-2.3.0/tests/test_cases/issues/issue_311/incorrect_with_list.xml
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)     4013 2022-07-18 14:19:15.000000 xmlschema-2.3.0/tests/test_cases/issues/issue_311/kPartModel_reduit_issue.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-05-18 20:19:54.627786 xmlschema-2.3.0/tests/test_cases/issues/issue_314/
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)      267 2022-07-21 09:40:50.000000 xmlschema-2.3.0/tests/test_cases/issues/issue_314/issue_314.xml
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)     1153 2022-07-21 09:40:50.000000 xmlschema-2.3.0/tests/test_cases/issues/issue_314/issue_314.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-05-18 20:19:54.629786 xmlschema-2.3.0/tests/test_cases/issues/issue_315/
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)       66 2022-07-18 14:19:15.000000 xmlschema-2.3.0/tests/test_cases/issues/issue_315/issue_315-1.xml
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)       63 2022-07-18 14:19:15.000000 xmlschema-2.3.0/tests/test_cases/issues/issue_315/issue_315-2.xml
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)       71 2022-07-18 14:19:15.000000 xmlschema-2.3.0/tests/test_cases/issues/issue_315/issue_315-3.xml
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)       76 2022-07-18 14:19:15.000000 xmlschema-2.3.0/tests/test_cases/issues/issue_315/issue_315-4.xml
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)       71 2022-07-18 14:19:15.000000 xmlschema-2.3.0/tests/test_cases/issues/issue_315/issue_315-5.xml
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)      604 2022-07-18 14:19:15.000000 xmlschema-2.3.0/tests/test_cases/issues/issue_315/issue_315_mixed.xsd
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)      456 2022-07-18 14:19:15.000000 xmlschema-2.3.0/tests/test_cases/issues/issue_315/issue_315_simple.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-05-18 20:19:54.631786 xmlschema-2.3.0/tests/test_cases/issues/issue_322/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      155 2022-08-26 15:33:28.000000 xmlschema-2.3.0/tests/test_cases/issues/issue_322/issue_322.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      348 2022-08-26 15:33:28.000000 xmlschema-2.3.0/tests/test_cases/issues/issue_322/issue_322.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-05-18 20:19:54.633786 xmlschema-2.3.0/tests/test_cases/issues/issue_324/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      373 2022-09-08 10:16:11.000000 xmlschema-2.3.0/tests/test_cases/issues/issue_324/issue_324-invalid.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      373 2022-09-08 10:16:11.000000 xmlschema-2.3.0/tests/test_cases/issues/issue_324/issue_324-valid.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      672 2022-08-28 05:56:41.000000 xmlschema-2.3.0/tests/test_cases/issues/issue_324/issue_324.zip
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      384 2022-09-08 10:16:11.000000 xmlschema-2.3.0/tests/test_cases/issues/issue_324/issue_324a.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      190 2022-09-08 10:16:11.000000 xmlschema-2.3.0/tests/test_cases/issues/issue_324/issue_324b.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-05-18 20:19:54.634786 xmlschema-2.3.0/tests/test_cases/issues/issue_334/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     1814 2023-02-11 10:41:50.000000 xmlschema-2.3.0/tests/test_cases/issues/issue_334/issue_334.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     5149 2023-02-11 10:41:50.000000 xmlschema-2.3.0/tests/test_cases/issues/issue_334/issue_334.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     2663 2023-02-09 09:02:31.000000 xmlschema-2.3.0/tests/test_cases/issues/issue_334/issue_334.zip
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-05-18 20:19:54.635786 xmlschema-2.3.0/tests/test_cases/issues/issue_341/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     2070 2023-04-14 13:49:05.000000 xmlschema-2.3.0/tests/test_cases/issues/issue_341/issue_341-ext.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      158 2023-04-14 13:49:05.000000 xmlschema-2.3.0/tests/test_cases/issues/issue_341/issue_341.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     1781 2023-04-14 13:49:05.000000 xmlschema-2.3.0/tests/test_cases/issues/issue_341/issue_341.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-05-18 20:19:54.636786 xmlschema-2.3.0/tests/test_cases/mypy/
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)      911 2022-05-20 16:16:20.000000 xmlschema-2.3.0/tests/test_cases/mypy/extra_validator.py
+-rwxrwxr-x   0 brunato   (1000) brunato   (1000)     1905 2023-05-05 12:33:46.000000 xmlschema-2.3.0/tests/test_cases/mypy/schema_source.py
+-rwxrwxr-x   0 brunato   (1000) brunato   (1000)      646 2021-11-11 15:30:24.000000 xmlschema-2.3.0/tests/test_cases/mypy/simple_types.py
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-05-18 20:19:54.637786 xmlschema-2.3.0/tests/test_cases/resources/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)       13 2020-01-23 20:05:17.000000 xmlschema-2.3.0/tests/test_cases/resources/dummy file #2.txt
+-rw-r--r--   0 brunato   (1000) brunato   (1000)       13 2020-01-23 20:05:17.000000 xmlschema-2.3.0/tests/test_cases/resources/dummy file.txt
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      171 2020-01-23 20:05:17.000000 xmlschema-2.3.0/tests/test_cases/resources/external_entity.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)       20 2020-01-23 20:05:17.000000 xmlschema-2.3.0/tests/test_cases/resources/malformed.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      308 2020-11-08 22:15:33.000000 xmlschema-2.3.0/tests/test_cases/resources/unparsed_entity.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      170 2020-01-23 20:05:17.000000 xmlschema-2.3.0/tests/test_cases/resources/unused_external_entity.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      270 2020-11-08 22:15:33.000000 xmlschema-2.3.0/tests/test_cases/resources/unused_unparsed_entity.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      129 2020-01-23 20:05:17.000000 xmlschema-2.3.0/tests/test_cases/resources/with_entity.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     6429 2023-05-18 20:18:16.000000 xmlschema-2.3.0/tests/test_cases/testfiles
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    11973 2021-03-04 20:38:45.000000 xmlschema-2.3.0/tests/test_cli.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    26576 2023-02-11 10:41:50.000000 xmlschema-2.3.0/tests/test_codegen.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    28857 2022-08-26 15:33:28.000000 xmlschema-2.3.0/tests/test_converters.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    26556 2023-02-06 08:55:27.000000 xmlschema-2.3.0/tests/test_dataobjects.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    24554 2023-02-06 06:20:42.000000 xmlschema-2.3.0/tests/test_documents.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     3234 2021-02-05 08:47:55.000000 xmlschema-2.3.0/tests/test_files.py
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)    26065 2022-07-18 14:19:15.000000 xmlschema-2.3.0/tests/test_helpers.py
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)     5745 2021-12-08 22:11:41.000000 xmlschema-2.3.0/tests/test_memory.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     9099 2023-02-11 10:41:50.000000 xmlschema-2.3.0/tests/test_namespaces.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     4755 2023-03-05 21:16:57.000000 xmlschema-2.3.0/tests/test_package.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    70653 2023-02-06 06:20:42.000000 xmlschema-2.3.0/tests/test_resources.py
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)     1785 2021-09-02 10:52:43.000000 xmlschema-2.3.0/tests/test_schemas.py
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)     3600 2022-05-20 20:00:14.000000 xmlschema-2.3.0/tests/test_translations.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     2022 2023-05-18 20:18:16.000000 xmlschema-2.3.0/tests/test_typing.py
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)     1806 2021-09-02 10:52:43.000000 xmlschema-2.3.0/tests/test_validation.py
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)    27317 2022-07-18 14:19:15.000000 xmlschema-2.3.0/tests/test_w3c_suite.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    44084 2023-05-18 20:18:16.000000 xmlschema-2.3.0/tests/test_wsdl.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    15023 2023-02-11 10:41:50.000000 xmlschema-2.3.0/tests/test_xpath.py
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-05-18 20:19:54.639786 xmlschema-2.3.0/tests/validation/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)        0 2020-11-10 10:12:46.000000 xmlschema-2.3.0/tests/validation/__init__.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    66088 2023-04-14 13:49:05.000000 xmlschema-2.3.0/tests/validation/test_decoding.py
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)    33339 2022-07-18 14:19:15.000000 xmlschema-2.3.0/tests/validation/test_encoding.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    16337 2022-10-01 13:42:01.000000 xmlschema-2.3.0/tests/validation/test_validation.py
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-05-18 20:19:54.647786 xmlschema-2.3.0/tests/validators/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)        0 2020-11-10 10:12:46.000000 xmlschema-2.3.0/tests/validators/__init__.py
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)    25878 2022-07-18 14:19:15.000000 xmlschema-2.3.0/tests/validators/test_attributes.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    14352 2020-12-23 12:38:37.000000 xmlschema-2.3.0/tests/validators/test_builtins.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    33116 2023-03-05 20:30:24.000000 xmlschema-2.3.0/tests/validators/test_complex_types.py
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)     4333 2022-06-24 14:13:22.000000 xmlschema-2.3.0/tests/validators/test_elements.py
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)     9464 2022-07-18 14:19:15.000000 xmlschema-2.3.0/tests/validators/test_exceptions.py
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)    60271 2022-07-18 14:19:15.000000 xmlschema-2.3.0/tests/validators/test_facets.py
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)     5409 2022-03-07 13:26:41.000000 xmlschema-2.3.0/tests/validators/test_global_maps.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    13500 2023-05-18 20:18:16.000000 xmlschema-2.3.0/tests/validators/test_groups.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    19187 2023-02-06 06:20:42.000000 xmlschema-2.3.0/tests/validators/test_identities.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    52697 2023-04-14 13:49:05.000000 xmlschema-2.3.0/tests/validators/test_models.py
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)     3447 2022-07-18 14:19:15.000000 xmlschema-2.3.0/tests/validators/test_notations.py
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)     8625 2022-07-18 14:19:15.000000 xmlschema-2.3.0/tests/validators/test_particles.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    41506 2022-10-01 13:42:01.000000 xmlschema-2.3.0/tests/validators/test_schemas.py
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)    10292 2022-07-18 14:19:15.000000 xmlschema-2.3.0/tests/validators/test_simple_types.py
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)    34302 2022-07-18 14:19:15.000000 xmlschema-2.3.0/tests/validators/test_wildcards.py
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)    33897 2022-07-18 14:19:15.000000 xmlschema-2.3.0/tests/validators/test_xsdbase.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     1569 2023-05-18 20:18:16.000000 xmlschema-2.3.0/tox.ini
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-05-18 20:19:54.656786 xmlschema-2.3.0/xmlschema/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     2857 2023-05-18 20:18:16.000000 xmlschema-2.3.0/xmlschema/__init__.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     5515 2023-03-05 21:16:57.000000 xmlschema-2.3.0/xmlschema/aliases.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    11669 2023-05-18 20:18:16.000000 xmlschema-2.3.0/xmlschema/cli.py
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-05-18 20:19:54.661786 xmlschema-2.3.0/xmlschema/converters/
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)      813 2022-07-18 14:19:15.000000 xmlschema-2.3.0/xmlschema/converters/__init__.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     5977 2023-03-05 21:16:57.000000 xmlschema-2.3.0/xmlschema/converters/abdera.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     7228 2023-03-05 21:16:57.000000 xmlschema-2.3.0/xmlschema/converters/badgerfish.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     7587 2023-03-05 21:16:57.000000 xmlschema-2.3.0/xmlschema/converters/columnar.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    19819 2023-03-05 21:16:57.000000 xmlschema-2.3.0/xmlschema/converters/default.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     4769 2023-03-05 21:16:57.000000 xmlschema-2.3.0/xmlschema/converters/jsonml.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     5840 2023-03-05 21:16:57.000000 xmlschema-2.3.0/xmlschema/converters/parker.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     5711 2023-03-05 21:16:57.000000 xmlschema-2.3.0/xmlschema/converters/unordered.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    23717 2023-03-05 21:16:57.000000 xmlschema-2.3.0/xmlschema/dataobjects.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    35712 2023-05-18 20:18:16.000000 xmlschema-2.3.0/xmlschema/documents.py
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)     1235 2021-10-20 14:14:48.000000 xmlschema-2.3.0/xmlschema/exceptions.py
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-05-18 20:19:54.662786 xmlschema-2.3.0/xmlschema/extras/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)        0 2021-02-05 09:05:33.000000 xmlschema-2.3.0/xmlschema/extras/__init__.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    21930 2023-05-18 20:18:16.000000 xmlschema-2.3.0/xmlschema/extras/codegen.py
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-05-18 20:19:54.538786 xmlschema-2.3.0/xmlschema/extras/templates/
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-05-18 20:19:54.663786 xmlschema-2.3.0/xmlschema/extras/templates/python/
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)      997 2022-07-18 14:19:15.000000 xmlschema-2.3.0/xmlschema/extras/templates/python/bindings.py.jinja
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     1116 2021-02-11 14:32:40.000000 xmlschema-2.3.0/xmlschema/extras/templates/python/sample.py.jinja
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    24454 2023-05-18 20:18:16.000000 xmlschema-2.3.0/xmlschema/extras/wsdl.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    11097 2022-08-26 15:33:28.000000 xmlschema-2.3.0/xmlschema/helpers.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      677 2020-11-10 10:13:55.000000 xmlschema-2.3.0/xmlschema/limits.py
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-05-18 20:19:54.538786 xmlschema-2.3.0/xmlschema/locale/
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-05-18 20:19:54.538786 xmlschema-2.3.0/xmlschema/locale/en/
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-05-18 20:19:54.665786 xmlschema-2.3.0/xmlschema/locale/en/LC_MESSAGES/
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)    45327 2022-05-20 20:00:14.000000 xmlschema-2.3.0/xmlschema/locale/en/LC_MESSAGES/xmlschema.mo
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)    64464 2022-05-20 20:00:14.000000 xmlschema-2.3.0/xmlschema/locale/en/LC_MESSAGES/xmlschema.po
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-05-18 20:19:54.538786 xmlschema-2.3.0/xmlschema/locale/it/
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-05-18 20:19:54.667786 xmlschema-2.3.0/xmlschema/locale/it/LC_MESSAGES/
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)    47535 2022-05-20 20:00:14.000000 xmlschema-2.3.0/xmlschema/locale/it/LC_MESSAGES/xmlschema.mo
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)    67361 2022-05-20 20:00:14.000000 xmlschema-2.3.0/xmlschema/locale/it/LC_MESSAGES/xmlschema.po
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-05-18 20:19:54.538786 xmlschema-2.3.0/xmlschema/locale/ru/
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-05-18 20:19:54.667786 xmlschema-2.3.0/xmlschema/locale/ru/LC_MESSAGES/
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)    60295 2022-06-11 14:29:39.000000 xmlschema-2.3.0/xmlschema/locale/ru/LC_MESSAGES/xmlschema.mo
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)    79497 2022-06-11 14:29:39.000000 xmlschema-2.3.0/xmlschema/locale/ru/LC_MESSAGES/xmlschema.po
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     8827 2020-12-23 12:38:37.000000 xmlschema-2.3.0/xmlschema/names.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     9907 2023-02-04 20:00:06.000000 xmlschema-2.3.0/xmlschema/namespaces.py
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)        0 2021-09-02 10:52:43.000000 xmlschema-2.3.0/xmlschema/py.typed
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    55658 2023-04-14 13:49:05.000000 xmlschema-2.3.0/xmlschema/resources.py
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-05-18 20:19:54.539785 xmlschema-2.3.0/xmlschema/schemas/
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-05-18 20:19:54.668786 xmlschema-2.3.0/xmlschema/schemas/HFP/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     1534 2020-11-08 22:15:33.000000 xmlschema-2.3.0/xmlschema/schemas/HFP/XMLSchema-hasFacetAndProperty_minimal.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-05-18 20:19:54.668786 xmlschema-2.3.0/xmlschema/schemas/VC/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      984 2020-11-08 22:15:33.000000 xmlschema-2.3.0/xmlschema/schemas/VC/XMLSchema-versioning.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-05-18 20:19:54.669786 xmlschema-2.3.0/xmlschema/schemas/WSDL/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    19204 2020-11-08 22:15:33.000000 xmlschema-2.3.0/xmlschema/schemas/WSDL/soap-encoding.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     6061 2020-11-08 22:15:33.000000 xmlschema-2.3.0/xmlschema/schemas/WSDL/soap-envelope.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     6005 2020-11-08 22:15:33.000000 xmlschema-2.3.0/xmlschema/schemas/WSDL/wsdl-soap.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    11900 2020-11-08 22:15:33.000000 xmlschema-2.3.0/xmlschema/schemas/WSDL/wsdl.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-05-18 20:19:54.669786 xmlschema-2.3.0/xmlschema/schemas/XHTML/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    65477 2020-11-08 22:15:33.000000 xmlschema-2.3.0/xmlschema/schemas/XHTML/xhtml1-strict.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-05-18 20:19:54.670786 xmlschema-2.3.0/xmlschema/schemas/XLINK/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     8051 2020-11-08 22:15:33.000000 xmlschema-2.3.0/xmlschema/schemas/XLINK/xlink.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-05-18 20:19:54.670786 xmlschema-2.3.0/xmlschema/schemas/XML/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     1277 2020-11-08 22:15:33.000000 xmlschema-2.3.0/xmlschema/schemas/XML/xml_minimal.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-05-18 20:19:54.671786 xmlschema-2.3.0/xmlschema/schemas/XSD_1.0/
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)    88033 2022-05-20 16:16:20.000000 xmlschema-2.3.0/xmlschema/schemas/XSD_1.0/XMLSchema.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    44301 2020-11-08 22:15:33.000000 xmlschema-2.3.0/xmlschema/schemas/XSD_1.0/datatypes.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-05-18 20:19:54.672786 xmlschema-2.3.0/xmlschema/schemas/XSD_1.1/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    67728 2022-09-25 07:58:42.000000 xmlschema-2.3.0/xmlschema/schemas/XSD_1.1/XMLSchema.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    17497 2020-11-08 22:15:33.000000 xmlschema-2.3.0/xmlschema/schemas/XSD_1.1/datatypes.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     3767 2022-09-12 09:59:59.000000 xmlschema-2.3.0/xmlschema/schemas/XSD_1.1/xsd11-extra.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-05-18 20:19:54.672786 xmlschema-2.3.0/xmlschema/schemas/XSI/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      385 2020-11-08 22:15:33.000000 xmlschema-2.3.0/xmlschema/schemas/XSI/XMLSchema-instance_minimal.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-05-18 20:19:54.675786 xmlschema-2.3.0/xmlschema/testing/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     2116 2023-05-18 20:18:16.000000 xmlschema-2.3.0/xmlschema/testing/__init__.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    29742 2023-05-18 20:18:16.000000 xmlschema-2.3.0/xmlschema/testing/_builders.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     7950 2023-05-18 20:18:16.000000 xmlschema-2.3.0/xmlschema/testing/_case_class.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     9443 2023-05-18 20:18:16.000000 xmlschema-2.3.0/xmlschema/testing/_factory.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     6911 2022-09-08 10:16:11.000000 xmlschema-2.3.0/xmlschema/testing/_helpers.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     4891 2023-05-18 20:18:16.000000 xmlschema-2.3.0/xmlschema/testing/_observers.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     2072 2023-02-11 10:41:50.000000 xmlschema-2.3.0/xmlschema/translation.py
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-05-18 20:19:54.687786 xmlschema-2.3.0/xmlschema/validators/
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)     3557 2021-11-11 15:30:24.000000 xmlschema-2.3.0/xmlschema/validators/__init__.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     6619 2023-05-07 06:35:13.000000 xmlschema-2.3.0/xmlschema/validators/assertions.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    34132 2022-09-24 15:52:22.000000 xmlschema-2.3.0/xmlschema/validators/attributes.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    19881 2022-08-26 15:33:28.000000 xmlschema-2.3.0/xmlschema/validators/builtins.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    46791 2023-05-07 06:33:55.000000 xmlschema-2.3.0/xmlschema/validators/complex_types.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    64166 2023-03-28 06:38:11.000000 xmlschema-2.3.0/xmlschema/validators/elements.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    14970 2023-03-05 21:16:57.000000 xmlschema-2.3.0/xmlschema/validators/exceptions.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    31723 2023-03-05 21:16:57.000000 xmlschema-2.3.0/xmlschema/validators/facets.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    33050 2023-05-05 13:39:50.000000 xmlschema-2.3.0/xmlschema/validators/global_maps.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    63595 2023-05-18 20:18:16.000000 xmlschema-2.3.0/xmlschema/validators/groups.py
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)     6655 2022-05-20 16:16:20.000000 xmlschema-2.3.0/xmlschema/validators/helpers.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    18740 2023-03-05 21:16:57.000000 xmlschema-2.3.0/xmlschema/validators/identities.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    23474 2023-04-14 13:49:05.000000 xmlschema-2.3.0/xmlschema/validators/models.py
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)     1611 2022-05-20 20:00:15.000000 xmlschema-2.3.0/xmlschema/validators/notations.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     6684 2023-05-18 20:18:16.000000 xmlschema-2.3.0/xmlschema/validators/particles.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)   103598 2023-05-07 06:48:48.000000 xmlschema-2.3.0/xmlschema/validators/schemas.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    61468 2023-05-08 10:45:15.000000 xmlschema-2.3.0/xmlschema/validators/simple_types.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    38290 2022-09-25 07:58:42.000000 xmlschema-2.3.0/xmlschema/validators/wildcards.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    41151 2023-03-05 21:16:57.000000 xmlschema-2.3.0/xmlschema/validators/xsdbase.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    13135 2023-02-11 10:41:50.000000 xmlschema-2.3.0/xmlschema/xpath.py
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-05-18 20:19:54.657786 xmlschema-2.3.0/xmlschema.egg-info/
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)     7377 2023-05-18 20:19:54.000000 xmlschema-2.3.0/xmlschema.egg-info/PKG-INFO
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)    17121 2023-05-18 20:19:54.000000 xmlschema-2.3.0/xmlschema.egg-info/SOURCES.txt
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)        1 2023-05-18 20:19:54.000000 xmlschema-2.3.0/xmlschema.egg-info/dependency_links.txt
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)      150 2023-05-18 20:19:54.000000 xmlschema-2.3.0/xmlschema.egg-info/entry_points.txt
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)      256 2023-05-18 20:19:54.000000 xmlschema-2.3.0/xmlschema.egg-info/requires.txt
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)       10 2023-05-18 20:19:54.000000 xmlschema-2.3.0/xmlschema.egg-info/top_level.txt
```

### Comparing `xmlschema-2.2.3/CHANGELOG.rst` & `xmlschema-2.3.0/CHANGELOG.rst`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,16 @@
 *********
 CHANGELOG
 *********
 
+`v2.3.0`_ (2023-05-18)
+======================
+* Improve sequence/all restriction checks for XSD 1.1
+* Add *schema* argument to `Wsdl11Document`
+
 `v2.2.3`_ (2023-04-14)
 ======================
 * Add support for Python 3.12
 * Detach content iteration methods from ModelVisitor
 
 `v2.2.2`_ (2023-03-05)
 ======================
@@ -612,7 +617,8 @@
 .. _v2.0.4: https://github.com/brunato/xmlschema/compare/v2.0.3...v2.0.4
 .. _v2.1.0: https://github.com/brunato/xmlschema/compare/v2.0.4...v2.1.0
 .. _v2.1.1: https://github.com/brunato/xmlschema/compare/v2.1.0...v2.1.1
 .. _v2.2.0: https://github.com/brunato/xmlschema/compare/v2.1.1...v2.2.0
 .. _v2.2.1: https://github.com/brunato/xmlschema/compare/v2.2.0...v2.2.1
 .. _v2.2.2: https://github.com/brunato/xmlschema/compare/v2.2.1...v2.2.2
 .. _v2.2.3: https://github.com/brunato/xmlschema/compare/v2.2.2...v2.2.3
+.. _v2.3.0: https://github.com/brunato/xmlschema/compare/v2.2.3...v2.3.0
```

### Comparing `xmlschema-2.2.3/LICENSE` & `xmlschema-2.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.3/PKG-INFO` & `xmlschema-2.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xmlschema
-Version: 2.2.3
+Version: 2.3.0
 Summary: An XML Schema validator and decoder
 Home-page: https://github.com/sissaschool/xmlschema
 Author: Davide Brunato
 Author-email: brunato@sissa.it
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `xmlschema-2.2.3/README.rst` & `xmlschema-2.3.0/README.rst`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.3/doc/Makefile` & `xmlschema-2.3.0/doc/Makefile`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.3/doc/api.rst` & `xmlschema-2.3.0/doc/api.rst`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.3/doc/components.rst` & `xmlschema-2.3.0/doc/components.rst`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.3/doc/conf.py` & `xmlschema-2.3.0/doc/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -75,17 +75,17 @@
 author = 'Davide Brunato'
 
 # The version info for the project you're documenting, acts as replacement for
 # |version| and |release|, also used in various other places throughout the
 # built documents.
 #
 # The short X.Y version.
-version = '2.2'
+version = '2.3'
 # The full version, including alpha/beta/rc tags.
-release = '2.2.3'
+release = '2.3.0'
 
 # The language for content autogenerated by Sphinx. Refer to documentation
 # for a list of supported languages.
 #
 # This is also used if you do content translation via gettext catalogs.
 # Usually you set "language" from the command line for these cases.
 # language = None
```

### Comparing `xmlschema-2.2.3/doc/converters.rst` & `xmlschema-2.3.0/doc/converters.rst`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.3/doc/extras.rst` & `xmlschema-2.3.0/doc/extras.rst`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.3/doc/features.rst` & `xmlschema-2.3.0/doc/features.rst`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.3/doc/testing.rst` & `xmlschema-2.3.0/doc/testing.rst`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.3/doc/usage.rst` & `xmlschema-2.3.0/doc/usage.rst`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.3/setup.py` & `xmlschema-2.3.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -14,35 +14,35 @@
 
 with Path(__file__).parent.joinpath('README.rst').open() as readme:
     long_description = readme.read()
 
 
 setup(
     name='xmlschema',
-    version='2.2.3',
+    version='2.3.0',
     packages=find_packages(include=['xmlschema*']),
     package_data={
         'xmlschema': ['py.typed', 'locale/**/*.mo', 'locale/**/*.po', 'schemas/*/*.xsd'],
         'xmlschema.extras': ['templates/*/*.jinja'],
     },
     entry_points={
         'console_scripts': [
             'xmlschema-validate=xmlschema.cli:validate',
             'xmlschema-xml2json=xmlschema.cli:xml2json',
             'xmlschema-json2xml=xmlschema.cli:json2xml',
         ]
     },
     python_requires='>=3.7',
-    install_requires=['elementpath>=4.0.0, <5.0.0'],
+    install_requires=['elementpath>=4.1.2, <5.0.0'],
     extras_require={
-        'codegen': ['elementpath>=4.0.0, <5.0.0', 'jinja2'],
-        'dev': ['tox', 'coverage', 'lxml', 'elementpath>=4.0.0, <5.0.0',
+        'codegen': ['elementpath>=4.1.2, <5.0.0', 'jinja2'],
+        'dev': ['tox', 'coverage', 'lxml', 'elementpath>=4.1.2, <5.0.0',
                 'memory_profiler', 'Sphinx', 'sphinx_rtd_theme', 'jinja2',
                 'flake8', 'mypy', 'lxml-stubs'],
-        'docs': ['elementpath>=4.0.0, <5.0.0', 'Sphinx', 'sphinx_rtd_theme', 'jinja2']
+        'docs': ['elementpath>=4.1.2, <5.0.0', 'Sphinx', 'sphinx_rtd_theme', 'jinja2']
     },
     author='Davide Brunato',
     author_email='brunato@sissa.it',
     url='https://github.com/sissaschool/xmlschema',
     license='MIT',
     license_file='LICENSE',
     description='An XML Schema validator and decoder',
```

### Comparing `xmlschema-2.2.3/tests/check_memory.py` & `xmlschema-2.3.0/tests/check_memory.py`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.3/tests/test_all.py` & `xmlschema-2.3.0/tests/test_all.py`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.3/tests/test_cases/examples/collection/collection-1_error.xml` & `xmlschema-2.3.0/tests/test_cases/examples/collection/collection-1_error.xml`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.3/tests/test_cases/examples/collection/collection-default.xml` & `xmlschema-2.3.0/tests/test_cases/examples/collection/collection-default.xml`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.3/tests/test_cases/examples/collection/collection.py` & `xmlschema-2.3.0/tests/test_cases/examples/collection/collection.py`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.3/tests/test_cases/examples/collection/collection.xml` & `xmlschema-2.3.0/tests/test_cases/examples/collection/collection.xml`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.3/tests/test_cases/examples/collection/collection.xsd` & `xmlschema-2.3.0/tests/test_cases/examples/collection/collection.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.3/tests/test_cases/examples/collection/collection2.xml` & `xmlschema-2.3.0/tests/test_cases/examples/collection/collection2.xml`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.3/tests/test_cases/examples/collection/collection2.xsd` & `xmlschema-2.3.0/tests/test_cases/examples/collection/collection2.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.3/tests/test_cases/examples/collection/collection3.xml` & `xmlschema-2.3.0/tests/test_cases/examples/collection/collection3.xml`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.3/tests/test_cases/examples/collection/collection3.xsd` & `xmlschema-2.3.0/tests/test_cases/examples/collection/collection3.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.3/tests/test_cases/examples/collection/collection3bis.xml` & `xmlschema-2.3.0/tests/test_cases/examples/collection/collection3bis.xml`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.3/tests/test_cases/examples/collection/collection3bis.xsd` & `xmlschema-2.3.0/tests/test_cases/examples/collection/collection3bis.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.3/tests/test_cases/examples/collection/collection4.xml` & `xmlschema-2.3.0/tests/test_cases/examples/collection/collection4.xml`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.3/tests/test_cases/examples/collection/collection4.xsd` & `xmlschema-2.3.0/tests/test_cases/examples/collection/collection4.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.3/tests/test_cases/examples/collection/collection5.xsd` & `xmlschema-2.3.0/tests/test_cases/examples/collection/collection5.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.3/tests/test_cases/examples/stockquote/stockquote.wsdl` & `xmlschema-2.3.0/tests/test_cases/examples/stockquote/stockquote.wsdl`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.3/tests/test_cases/examples/stockquote/stockquote.xsd` & `xmlschema-2.3.0/tests/test_cases/examples/stockquote/stockquote.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.3/tests/test_cases/examples/stockquote/stockquoteservice.wsdl` & `xmlschema-2.3.0/tests/test_cases/examples/stockquote/stockquoteservice.wsdl`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.3/tests/test_cases/examples/vehicles/invalid.xsd` & `xmlschema-2.3.0/tests/test_cases/examples/vehicles/invalid.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.3/tests/test_cases/examples/vehicles/vehicles-max.xsd` & `xmlschema-2.3.0/tests/test_cases/examples/vehicles/vehicles-max.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.3/tests/test_cases/examples/vehicles/vehicles-schemas.xsd.zip` & `xmlschema-2.3.0/tests/test_cases/examples/vehicles/vehicles-schemas.xsd.zip`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.3/tests/test_cases/examples/vehicles/vehicles.xsd` & `xmlschema-2.3.0/tests/test_cases/examples/vehicles/vehicles.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.3/tests/test_cases/features/attributes/default_attributes-missing_group.xsd` & `xmlschema-2.3.0/tests/test_cases/features/attributes/default_attributes-missing_group.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.3/tests/test_cases/features/attributes/default_attributes.xsd` & `xmlschema-2.3.0/tests/test_cases/features/attributes/default_attributes.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.3/tests/test_cases/features/builtins/builtins.xml` & `xmlschema-2.3.0/tests/test_cases/features/builtins/builtins.xml`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.3/tests/test_cases/features/builtins/builtins.xsd` & `xmlschema-2.3.0/tests/test_cases/features/builtins/builtins.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.3/tests/test_cases/features/decoder/data.xml` & `xmlschema-2.3.0/tests/test_cases/features/decoder/data.xml`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.3/tests/test_cases/features/decoder/data2.xml` & `xmlschema-2.3.0/tests/test_cases/features/decoder/data2.xml`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.3/tests/test_cases/features/decoder/data3.xml` & `xmlschema-2.3.0/tests/test_cases/features/decoder/data3.xml`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.3/tests/test_cases/features/decoder/long-sequence-1.xsd` & `xmlschema-2.3.0/tests/test_cases/features/decoder/long-sequence-1.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.3/tests/test_cases/features/decoder/mixed-content.xsd` & `xmlschema-2.3.0/tests/test_cases/features/decoder/mixed-content.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.3/tests/test_cases/features/decoder/simple-types.xsd` & `xmlschema-2.3.0/tests/test_cases/features/decoder/simple-types.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.3/tests/test_cases/features/derivations/complex-extensions.xsd` & `xmlschema-2.3.0/tests/test_cases/features/derivations/complex-extensions.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.3/tests/test_cases/features/derivations/complex-with-simple-content-restriction.xsd` & `xmlschema-2.3.0/tests/test_cases/features/derivations/complex-with-simple-content-restriction.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.3/tests/test_cases/features/derivations/invalid_enumeration_restriction.xsd` & `xmlschema-2.3.0/tests/test_cases/features/derivations/invalid-enumeration-restriction.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.3/tests/test_cases/features/derivations/invalid_restrictions1.xsd` & `xmlschema-2.3.0/tests/test_cases/features/derivations/invalid-restrictions1.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.3/tests/test_cases/features/derivations/invalid_restrictions2.xsd` & `xmlschema-2.3.0/tests/test_cases/features/models/valid_model1.xsd`

 * *Files 20% similar despite different names*

#### Comparing `xmlschema-2.2.3/tests/test_cases/features/derivations/invalid_restrictions2.xsd` & `xmlschema-2.3.0/tests/test_cases/features/models/valid_model1.xsd`

```diff
@@ -1,39 +1,28 @@
 <?xml version="1.0" encoding="utf-8"?>
-<!-- Schema test for invalid models: UPA violation restricting a substitution group head. -->
-<xs:schema xmlns:xs="http://www.w3.org/2001/XMLSchema">
-  <xs:complexType name="baseType1">
+<!-- A valid schema model (related to issue #182). -->
+<xs:schema xmlns="ns" xmlns:xs="http://www.w3.org/2001/XMLSchema" targetNamespace="ns">
+  <xs:element name="elem1" type="xs:string"/>
+  <xs:element name="elem2" type="xs:string"/>
+  <xs:element name="elem3" type="xs:string"/>
+  <xs:element name="elem4" type="xs:string"/>
+  <xs:complexType name="type1">
     <xs:sequence>
-      <xs:element name="elem1"/>
-      <xs:element minOccurs="0" name="elem2"/>
+      <xs:element ref="elem1" maxOccurs="10"/>
       <xs:choice>
-        <xs:element name="elem3" type="xs:string"/>
-        <xs:element name="elem4" type="xs:string"/>
-      </xs:choice>
-      <xs:element minOccurs="0" name="elem5"/>
-      <xs:element minOccurs="0" name="elem6" type="xs:string"/>
-      <xs:element minOccurs="0" name="elem7"/>
-    </xs:sequence>
-  </xs:complexType>
-  <xs:complexType name="restrictedType1">
-    <xs:complexContent>
-      <xs:restriction base="baseType1">
         <xs:sequence>
-          <xs:sequence>
-            <xs:element name="elem1"/>
-            <xs:element minOccurs="0" name="elem2"/>
-            <xs:choice>
-              <xs:element name="elem3" type="xs:token"/>
-              <xs:element name="elem4" type="xs:string"/>
-            </xs:choice>
-            <xs:sequence>
-              <xs:element minOccurs="0" name="elem6" type="xs:string"/>
-            </xs:sequence>
-          </xs:sequence>
-          <xs:sequence>
-            <xs:element minOccurs="0" name="elem7"/>
-          </xs:sequence>
+          <xs:choice>
+            <xs:element ref="elem2"/>
+            <xs:element ref="elem3"/>
+          </xs:choice>
         </xs:sequence>
-      </xs:restriction>
-    </xs:complexContent>
+        <xs:sequence>
+          <xs:element ref="elem4"/>
+          <xs:choice>
+            <xs:element ref="elem2" minOccurs="0"/>
+            <xs:element ref="elem3" minOccurs="0"/>
+          </xs:choice>
+        </xs:sequence>
+      </xs:choice>
+    </xs:sequence>
   </xs:complexType>
 </xs:schema>
```

### Comparing `xmlschema-2.2.3/tests/test_cases/features/derivations/list_types.xsd` & `xmlschema-2.3.0/tests/test_cases/features/derivations/list_types.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.3/tests/test_cases/features/elements/type_alternatives-no-ns.xsd` & `xmlschema-2.3.0/tests/test_cases/features/elements/type_alternatives-no-ns.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.3/tests/test_cases/features/elements/type_alternatives.xsd` & `xmlschema-2.3.0/tests/test_cases/features/elements/type_alternatives.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.3/tests/test_cases/features/models/billion_laughs_model.xsd` & `xmlschema-2.3.0/tests/test_cases/features/models/billion_laughs_model.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.3/tests/test_cases/features/models/illegal-declarations.xsd` & `xmlschema-2.3.0/tests/test_cases/features/models/illegal-declarations.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.3/tests/test_cases/features/models/illegal-occurs.xsd` & `xmlschema-2.3.0/tests/test_cases/features/models/illegal-occurs.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.3/tests/test_cases/features/models/invalid_models1.xsd` & `xmlschema-2.3.0/tests/test_cases/features/models/invalid_models1.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.3/tests/test_cases/features/models/invalid_models2.xsd` & `xmlschema-2.3.0/tests/test_cases/features/models/invalid_models2.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.3/tests/test_cases/features/models/models.xsd` & `xmlschema-2.3.0/tests/test_cases/features/models/models.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.3/tests/test_cases/features/models/recursive-groups.xsd` & `xmlschema-2.3.0/tests/test_cases/features/models/recursive-groups.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.3/tests/test_cases/features/models/valid_model1.xsd` & `xmlschema-2.3.0/tests/test_cases/issues/issue_306/issue_306.xsd`

 * *Files 20% similar despite different names*

#### Comparing `xmlschema-2.2.3/tests/test_cases/features/models/valid_model1.xsd` & `xmlschema-2.3.0/tests/test_cases/issues/issue_306/issue_306.xsd`

```diff
@@ -1,28 +1,17 @@
 <?xml version="1.0" encoding="utf-8"?>
-<!-- A valid schema model (related to issue #182). -->
-<xs:schema xmlns="ns" xmlns:xs="http://www.w3.org/2001/XMLSchema" targetNamespace="ns">
-  <xs:element name="elem1" type="xs:string"/>
-  <xs:element name="elem2" type="xs:string"/>
-  <xs:element name="elem3" type="xs:string"/>
-  <xs:element name="elem4" type="xs:string"/>
-  <xs:complexType name="type1">
-    <xs:sequence>
-      <xs:element ref="elem1" maxOccurs="10"/>
-      <xs:choice>
-        <xs:sequence>
-          <xs:choice>
-            <xs:element ref="elem2"/>
-            <xs:element ref="elem3"/>
-          </xs:choice>
-        </xs:sequence>
-        <xs:sequence>
-          <xs:element ref="elem4"/>
-          <xs:choice>
-            <xs:element ref="elem2" minOccurs="0"/>
-            <xs:element ref="elem3" minOccurs="0"/>
-          </xs:choice>
-        </xs:sequence>
-      </xs:choice>
-    </xs:sequence>
-  </xs:complexType>
+<xs:schema xmlns:xs="http://www.w3.org/2001/XMLSchema">
+  <xs:element name="Document">
+    <xs:complexType>
+      <xs:sequence>
+        <xs:element name="shipto">
+          <xs:complexType>
+            <xs:sequence>
+              <xs:element minOccurs="0" maxOccurs="0" name="name" type="xs:string"/>
+              <xs:element minOccurs="0" maxOccurs="1" name="address" type="xs:string"/>
+            </xs:sequence>
+          </xs:complexType>
+        </xs:element>
+      </xs:sequence>
+    </xs:complexType>
+  </xs:element>
 </xs:schema>
```

### Comparing `xmlschema-2.2.3/tests/test_cases/features/namespaces/import-case1.xsd` & `xmlschema-2.3.0/tests/test_cases/features/namespaces/import-case1.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.3/tests/test_cases/features/namespaces/import-case2.xsd` & `xmlschema-2.3.0/tests/test_cases/features/namespaces/import-case2.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.3/tests/test_cases/features/namespaces/import-case4a.xsd` & `xmlschema-2.3.0/tests/test_cases/features/namespaces/import-case4a.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.3/tests/test_cases/features/namespaces/import-case4b.xsd` & `xmlschema-2.3.0/tests/test_cases/features/namespaces/import-case4b.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.3/tests/test_cases/features/namespaces/include-case2.xsd` & `xmlschema-2.3.0/tests/test_cases/features/namespaces/include-case2.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.3/tests/test_cases/features/namespaces/include-case2bis.xsd` & `xmlschema-2.3.0/tests/test_cases/features/namespaces/include-case2bis.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.3/tests/test_cases/features/namespaces/include-case3.xsd` & `xmlschema-2.3.0/tests/test_cases/features/namespaces/include-case3.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.3/tests/test_cases/features/namespaces/include-case5.xsd` & `xmlschema-2.3.0/tests/test_cases/features/namespaces/include-case5.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.3/tests/test_cases/features/patterns/patterns.xml` & `xmlschema-2.3.0/tests/test_cases/features/patterns/patterns.xml`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.3/tests/test_cases/features/patterns/patterns.xsd` & `xmlschema-2.3.0/tests/test_cases/features/patterns/patterns.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.3/tests/test_cases/features/wsdl/wsdl11_example3.wsdl` & `xmlschema-2.3.0/tests/test_cases/features/wsdl/wsdl11_example3_valid.wsdl`

 * *Files 4% similar despite different names*

#### Comparing `xmlschema-2.2.3/tests/test_cases/features/wsdl/wsdl11_example3.wsdl` & `xmlschema-2.3.0/tests/test_cases/features/wsdl/wsdl11_example3_valid.wsdl`

```diff
@@ -1,29 +1,26 @@
 <?xml version="1.0" encoding="utf-8"?>
 <!--
-Original example #3 from WSDL 1.1 definition with SOAP 1.1 bindings:
+Example #3 from WSDL 1.1 definition with SOAP 1.1 bindings:
   href: https://www.w3.org/TR/2001/NOTE-wsdl-20010315#_soap-e
-
-Thi version contains a typo in <binding> definition
 -->
 <definitions xmlns:tns="http://example.com/stockquote.wsdl" xmlns:xsd1="http://example.com/stockquote.xsd" xmlns:soap="http://schemas.xmlsoap.org/wsdl/soap/" xmlns="http://schemas.xmlsoap.org/wsdl/" name="StockQuote" targetNamespace="http://example.com/stockquote.wsdl">
   <message name="SubscribeToQuotes">
     <part name="body" element="xsd1:SubscribeToQuotes"/>
     <part name="subscribeheader" element="xsd1:SubscriptionHeader"/>
   </message>
   <portType name="StockQuotePortType">
     <operation name="SubscribeToQuotes">
       <input message="tns:SubscribeToQuotes"/>
     </operation>
   </portType>
   <binding name="StockQuoteSoap" type="tns:StockQuotePortType">
     <soap:binding style="document" transport="http://example.com/smtp"/>
     <operation name="SubscribeToQuotes">
-      <input message="tns:SubscribeToQuotes">
-        <!-- attribute 'message' not allowed -->
+      <input>
         <soap:body parts="body" use="literal"/>
         <soap:header message="tns:SubscribeToQuotes" part="subscribeheader" use="literal"/>
       </input>
     </operation>
   </binding>
   <service name="StockQuoteService">
     <port name="StockQuotePort" binding="tns:StockQuoteSoap">
```

### Comparing `xmlschema-2.2.3/tests/test_cases/features/wsdl/wsdl11_example3_valid.wsdl` & `xmlschema-2.3.0/tests/test_cases/features/wsdl/wsdl11_example3.wsdl`

 * *Files 6% similar despite different names*

#### Comparing `xmlschema-2.2.3/tests/test_cases/features/wsdl/wsdl11_example3_valid.wsdl` & `xmlschema-2.3.0/tests/test_cases/features/wsdl/wsdl11_example3.wsdl`

```diff
@@ -1,26 +1,29 @@
 <?xml version="1.0" encoding="utf-8"?>
 <!--
-Example #3 from WSDL 1.1 definition with SOAP 1.1 bindings:
+Original example #3 from WSDL 1.1 definition with SOAP 1.1 bindings:
   href: https://www.w3.org/TR/2001/NOTE-wsdl-20010315#_soap-e
+
+This case contains a typo in <binding> definition
 -->
 <definitions xmlns:tns="http://example.com/stockquote.wsdl" xmlns:xsd1="http://example.com/stockquote.xsd" xmlns:soap="http://schemas.xmlsoap.org/wsdl/soap/" xmlns="http://schemas.xmlsoap.org/wsdl/" name="StockQuote" targetNamespace="http://example.com/stockquote.wsdl">
   <message name="SubscribeToQuotes">
     <part name="body" element="xsd1:SubscribeToQuotes"/>
     <part name="subscribeheader" element="xsd1:SubscriptionHeader"/>
   </message>
   <portType name="StockQuotePortType">
     <operation name="SubscribeToQuotes">
       <input message="tns:SubscribeToQuotes"/>
     </operation>
   </portType>
   <binding name="StockQuoteSoap" type="tns:StockQuotePortType">
     <soap:binding style="document" transport="http://example.com/smtp"/>
     <operation name="SubscribeToQuotes">
-      <input>
+      <input message="tns:SubscribeToQuotes">
+        <!-- attribute 'message' not allowed -->
         <soap:body parts="body" use="literal"/>
         <soap:header message="tns:SubscribeToQuotes" part="subscribeheader" use="literal"/>
       </input>
     </operation>
   </binding>
   <service name="StockQuoteService">
     <port name="StockQuotePort" binding="tns:StockQuoteSoap">
```

### Comparing `xmlschema-2.2.3/tests/test_cases/features/wsdl/wsdl11_example4.wsdl` & `xmlschema-2.3.0/tests/test_cases/features/wsdl/wsdl11_example4.wsdl`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.3/tests/test_cases/features/wsdl/wsdl11_example4_valid.wsdl` & `xmlschema-2.3.0/tests/test_cases/features/wsdl/wsdl11_example4_valid.wsdl`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.3/tests/test_cases/features/wsdl/wsdl11_example5.wsdl` & `xmlschema-2.3.0/tests/test_cases/features/wsdl/wsdl11_example5.wsdl`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.3/tests/test_cases/features/wsdl/wsdl11_example5_valid.wsdl` & `xmlschema-2.3.0/tests/test_cases/features/wsdl/wsdl11_example5_valid.wsdl`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.3/tests/test_cases/features/wsdl/wsdl11_example5_with_fault.wsdl` & `xmlschema-2.3.0/tests/test_cases/features/wsdl/wsdl11_example5_with_fault.wsdl`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.3/tests/test_cases/issues/issue_008/issue_008.xsd` & `xmlschema-2.3.0/tests/test_cases/issues/issue_008/issue_008.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.3/tests/test_cases/issues/issue_013/issue_013-1.xsd` & `xmlschema-2.3.0/tests/test_cases/issues/issue_013/issue_013-1.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.3/tests/test_cases/issues/issue_013/issue_013.xsd` & `xmlschema-2.3.0/tests/test_cases/issues/issue_013/issue_013.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.3/tests/test_cases/issues/issue_014/issue014.xsd` & `xmlschema-2.3.0/tests/test_cases/issues/issue_014/issue014.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.3/tests/test_cases/issues/issue_018/issue_018.xsd` & `xmlschema-2.3.0/tests/test_cases/issues/issue_018/issue_018.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.3/tests/test_cases/issues/issue_022/README.md` & `xmlschema-2.3.0/tests/test_cases/issues/issue_022/README.md`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.3/tests/test_cases/issues/issue_022/xsd_string.xsd` & `xmlschema-2.3.0/tests/test_cases/issues/issue_022/xsd_string.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.3/tests/test_cases/issues/issue_026/issue_026.xsd` & `xmlschema-2.3.0/tests/test_cases/issues/issue_026/issue_026.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.3/tests/test_cases/issues/issue_035/dates.xml` & `xmlschema-2.3.0/tests/test_cases/issues/issue_035/dates.xml`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.3/tests/test_cases/issues/issue_035/dates.xsd` & `xmlschema-2.3.0/tests/test_cases/issues/issue_035/dates.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.3/tests/test_cases/issues/issue_041/issue_041.xsd` & `xmlschema-2.3.0/tests/test_cases/issues/issue_041/issue_041.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.3/tests/test_cases/issues/issue_051/issue_051.xsd` & `xmlschema-2.3.0/tests/test_cases/issues/issue_051/issue_051.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.3/tests/test_cases/issues/issue_073/issue_073.xsd` & `xmlschema-2.3.0/tests/test_cases/issues/issue_073/issue_073.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.3/tests/test_cases/issues/issue_086/issue_086.xsd` & `xmlschema-2.3.0/tests/test_cases/issues/issue_086/issue_086.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.3/tests/test_cases/issues/issue_105/issue_105.xsd` & `xmlschema-2.3.0/tests/test_cases/issues/issue_105/issue_105.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.3/tests/test_cases/issues/issue_111/issue_111.xsd` & `xmlschema-2.3.0/tests/test_cases/issues/issue_111/issue_111.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.3/tests/test_cases/issues/issue_111/issue_111_skeleton.xsd` & `xmlschema-2.3.0/tests/test_cases/issues/issue_111/issue_111_skeleton.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.3/tests/test_cases/issues/issue_115/Rotation.xsd` & `xmlschema-2.3.0/tests/test_cases/issues/issue_115/Rotation.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.3/tests/test_cases/issues/issue_171/issue_171.xsd` & `xmlschema-2.3.0/tests/test_cases/issues/issue_171/issue_171.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.3/tests/test_cases/issues/issue_171/issue_171b.xsd` & `xmlschema-2.3.0/tests/test_cases/issues/issue_171/issue_171b.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.3/tests/test_cases/issues/issue_187/issue_187_1.xsd` & `xmlschema-2.3.0/tests/test_cases/issues/issue_187/issue_187_1.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.3/tests/test_cases/issues/issue_187/issue_187_2.xsd` & `xmlschema-2.3.0/tests/test_cases/issues/issue_187/issue_187_2.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.3/tests/test_cases/issues/issue_190/issue_190.xsd` & `xmlschema-2.3.0/tests/test_cases/issues/issue_190/issue_190.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.3/tests/test_cases/issues/issue_200/issue_200.xsd` & `xmlschema-2.3.0/tests/test_cases/issues/issue_200/issue_200.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.3/tests/test_cases/issues/issue_203/issue_203.xsd` & `xmlschema-2.3.0/tests/test_cases/issues/issue_203/issue_203.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.3/tests/test_cases/issues/issue_203/issue_203alt.xsd` & `xmlschema-2.3.0/tests/test_cases/issues/issue_203/issue_203alt.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.3/tests/test_cases/issues/issue_204/issue_204.xsd` & `xmlschema-2.3.0/tests/test_cases/issues/issue_204/issue_204.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.3/tests/test_cases/issues/issue_208/issue_208.xsd` & `xmlschema-2.3.0/tests/test_cases/issues/issue_208/issue_208.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.3/tests/test_cases/issues/issue_222/issue_222.xsd` & `xmlschema-2.3.0/tests/test_cases/issues/issue_222/issue_222.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.3/tests/test_cases/issues/issue_237/dir1/stockquoteservice.wsdl` & `xmlschema-2.3.0/tests/test_cases/issues/issue_237/dir1/stockquoteservice.wsdl`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.3/tests/test_cases/issues/issue_237/dir2/stockquote.wsdl` & `xmlschema-2.3.0/tests/test_cases/issues/issue_237/dir2/stockquote.wsdl`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.3/tests/test_cases/issues/issue_237/dir2/stockquote.xsd` & `xmlschema-2.3.0/tests/test_cases/issues/issue_237/dir2/stockquote.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.3/tests/test_cases/issues/issue_243/issue_243.xsd` & `xmlschema-2.3.0/tests/test_cases/issues/issue_243/issue_243.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.3/tests/test_cases/issues/issue_245/issue_245-valid.xml` & `xmlschema-2.3.0/tests/test_cases/issues/issue_245/issue_245-valid.xml`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.3/tests/test_cases/issues/issue_245/issue_245.xml` & `xmlschema-2.3.0/tests/test_cases/issues/issue_245/issue_245.xml`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.3/tests/test_cases/issues/issue_245/issue_245.xsd` & `xmlschema-2.3.0/tests/test_cases/issues/issue_245/issue_245.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.3/tests/test_cases/issues/issue_259/issue_259-1.xsd` & `xmlschema-2.3.0/tests/test_cases/issues/issue_259/issue_259-1.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.3/tests/test_cases/issues/issue_259/issue_259-2.xsd` & `xmlschema-2.3.0/tests/test_cases/issues/issue_259/issue_259-2.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.3/tests/test_cases/issues/issue_265/issue_265-1.xsd` & `xmlschema-2.3.0/tests/test_cases/issues/issue_265/issue_265-1.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.3/tests/test_cases/issues/issue_265/issue_265-2-invalid.xsd` & `xmlschema-2.3.0/tests/test_cases/issues/issue_265/issue_265-2-invalid.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.3/tests/test_cases/issues/issue_266/issue_266-1.xsd` & `xmlschema-2.3.0/tests/test_cases/issues/issue_266/issue_266-1.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.3/tests/test_cases/issues/issue_266/issue_266-2.xsd` & `xmlschema-2.3.0/tests/test_cases/issues/issue_266/issue_266-2.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.3/tests/test_cases/issues/issue_266/issue_266b-1.xsd` & `xmlschema-2.3.0/tests/test_cases/issues/issue_266/issue_266b-1.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.3/tests/test_cases/issues/issue_266/issue_266b-2.xsd` & `xmlschema-2.3.0/tests/test_cases/issues/issue_266/issue_266b-2.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.3/tests/test_cases/issues/issue_273/issue_273.xsd` & `xmlschema-2.3.0/tests/test_cases/issues/issue_273/issue_273.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.3/tests/test_cases/issues/issue_298/issue_298.xsd` & `xmlschema-2.3.0/tests/test_cases/issues/issue_298/issue_298.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.3/tests/test_cases/issues/issue_306/issue_306-alt.xsd` & `xmlschema-2.3.0/tests/test_cases/issues/issue_306/issue_306-alt.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.3/tests/test_cases/issues/issue_306/issue_306.xsd` & `xmlschema-2.3.0/tests/test_cases/issues/issue_315/issue_315_mixed.xsd`

 * *Files 26% similar despite different names*

#### Comparing `xmlschema-2.2.3/tests/test_cases/issues/issue_306/issue_306.xsd` & `xmlschema-2.3.0/tests/test_cases/issues/issue_315/issue_315_mixed.xsd`

```diff
@@ -1,17 +1,14 @@
 <?xml version="1.0" encoding="utf-8"?>
-<xs:schema xmlns:xs="http://www.w3.org/2001/XMLSchema">
-  <xs:element name="Document">
-    <xs:complexType>
-      <xs:sequence>
-        <xs:element name="shipto">
-          <xs:complexType>
-            <xs:sequence>
-              <xs:element minOccurs="0" maxOccurs="0" name="name" type="xs:string"/>
-              <xs:element minOccurs="0" maxOccurs="1" name="address" type="xs:string"/>
-            </xs:sequence>
-          </xs:complexType>
-        </xs:element>
-      </xs:sequence>
-    </xs:complexType>
-  </xs:element>
+<xs:schema xmlns:tst="http://xmlschema.test/ns" xmlns:xs="http://www.w3.org/2001/XMLSchema" targetNamespace="http://xmlschema.test/ns">
+  <xs:element name="e1" type="tst:t1"/>
+  <xs:complexType name="t1">
+    <xs:complexContent mixed="true">
+      <xs:restriction base="xs:anyType">
+        <xs:choice minOccurs="0" maxOccurs="unbounded">
+          <xs:element name="e2" type="xs:string"/>
+        </xs:choice>
+        <xs:attribute type="xs:string" name="a1"/>
+      </xs:restriction>
+    </xs:complexContent>
+  </xs:complexType>
 </xs:schema>
```

### Comparing `xmlschema-2.2.3/tests/test_cases/issues/issue_311/correct_no_list.xml` & `xmlschema-2.3.0/tests/test_cases/issues/issue_311/correct_no_list.xml`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.3/tests/test_cases/issues/issue_311/incorrect_with_list.xml` & `xmlschema-2.3.0/tests/test_cases/issues/issue_311/incorrect_with_list.xml`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.3/tests/test_cases/issues/issue_311/kPartModel_reduit_issue.xsd` & `xmlschema-2.3.0/tests/test_cases/issues/issue_311/kPartModel_reduit_issue.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.3/tests/test_cases/issues/issue_314/issue_314.xsd` & `xmlschema-2.3.0/tests/test_cases/issues/issue_314/issue_314.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.3/tests/test_cases/issues/issue_324/issue_324.zip` & `xmlschema-2.3.0/tests/test_cases/issues/issue_324/issue_324.zip`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.3/tests/test_cases/issues/issue_334/issue_334.xml` & `xmlschema-2.3.0/tests/test_cases/issues/issue_334/issue_334.xml`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.3/tests/test_cases/issues/issue_334/issue_334.xsd` & `xmlschema-2.3.0/tests/test_cases/issues/issue_334/issue_334.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.3/tests/test_cases/issues/issue_334/issue_334.zip` & `xmlschema-2.3.0/tests/test_cases/issues/issue_334/issue_334.zip`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.3/tests/test_cases/issues/issue_341/issue_341-ext.xsd` & `xmlschema-2.3.0/tests/test_cases/issues/issue_341/issue_341-ext.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.3/tests/test_cases/issues/issue_341/issue_341.xsd` & `xmlschema-2.3.0/tests/test_cases/issues/issue_341/issue_341.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.3/tests/test_cases/mypy/extra_validator.py` & `xmlschema-2.3.0/tests/test_cases/mypy/extra_validator.py`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.3/tests/test_cases/mypy/schema_source.py` & `xmlschema-2.3.0/tests/test_cases/mypy/schema_source.py`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.3/tests/test_cases/mypy/simple_types.py` & `xmlschema-2.3.0/tests/test_cases/mypy/simple_types.py`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.3/tests/test_cases/testfiles` & `xmlschema-2.3.0/tests/test_cases/testfiles`

 * *Files 2% similar despite different names*

```diff
@@ -35,19 +35,23 @@
 
 features/decoder/simple-types.xsd
 features/decoder/data2.xml --errors=2
 features/decoder/mixed-content.xsd
 features/decoder/data4-mixed.xml
 
 features/derivations/complex-extensions.xsd --errors=1
+features/derivations/complex11-restrictions.xsd --version=1.1
 features/derivations/complex-with-simple-content-restriction.xsd
 features/derivations/list_types.xsd --errors=1
 features/derivations/list_types.xml --errors=2
-features/derivations/invalid_enumeration_restriction.xsd --errors=1
-features/derivations/invalid_restrictions1.xsd --errors=2
+features/derivations/invalid-enumeration-restriction.xsd --errors=1
+features/derivations/invalid-restrictions1.xsd --errors=2
+features/derivations/invalid-restrictions1.xsd --version=1.1 --errors=1
+features/derivations/invalid-restrictions2.xsd --errors=1
+features/derivations/invalid-restrictions2.xsd --version=1.1 --errors=1
 
 features/elements/type_alternatives.xsd --errors=3
 features/elements/type_alternatives.xsd --version=1.1
 features/elements/type_alternatives-no-ns.xsd --version=1.1
 features/elements/test_alternatives-1.xml --version=1.1
 
 features/models/billion_laughs_model.xsd
```

### Comparing `xmlschema-2.2.3/tests/test_cli.py` & `xmlschema-2.3.0/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.3/tests/test_codegen.py` & `xmlschema-2.3.0/tests/test_codegen.py`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.3/tests/test_converters.py` & `xmlschema-2.3.0/tests/test_converters.py`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.3/tests/test_dataobjects.py` & `xmlschema-2.3.0/tests/test_dataobjects.py`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.3/tests/test_documents.py` & `xmlschema-2.3.0/tests/test_documents.py`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.3/tests/test_files.py` & `xmlschema-2.3.0/tests/test_files.py`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.3/tests/test_helpers.py` & `xmlschema-2.3.0/tests/test_helpers.py`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.3/tests/test_memory.py` & `xmlschema-2.3.0/tests/test_memory.py`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.3/tests/test_namespaces.py` & `xmlschema-2.3.0/tests/test_namespaces.py`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.3/tests/test_package.py` & `xmlschema-2.3.0/tests/test_package.py`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.3/tests/test_resources.py` & `xmlschema-2.3.0/tests/test_resources.py`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.3/tests/test_schemas.py` & `xmlschema-2.3.0/tests/test_schemas.py`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.3/tests/test_translations.py` & `xmlschema-2.3.0/tests/test_translations.py`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.3/tests/test_validation.py` & `xmlschema-2.3.0/tests/test_validation.py`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.3/tests/test_w3c_suite.py` & `xmlschema-2.3.0/tests/test_w3c_suite.py`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.3/tests/test_wsdl.py` & `xmlschema-2.3.0/tests/test_wsdl.py`

 * *Files 0% similar despite different names*

```diff
@@ -254,14 +254,27 @@
         service_name = '{http://example.com/stockquote.wsdl}StockQuoteService'
         self.assertListEqual(list(wsdl_document.services), [service_name])
         self.assertEqual(list(wsdl_document.services[service_name].ports), ['StockQuotePort'])
 
         port = wsdl_document.services[service_name].ports['StockQuotePort']
         self.assertEqual(port.soap_location, 'mailto:subscribe@example.com')
 
+    def test_example3_without_types__issue_347(self):
+        no_types_file = casepath('features/wsdl/wsdl11_example3_no_types.wsdl')
+        with self.assertRaises(WsdlParseError):
+            Wsdl11Document(no_types_file)
+
+        schema_file = casepath('features/wsdl/wsdl11_example3_types.xsd')
+        wsdl_document = Wsdl11Document(no_types_file, schema=schema_file)
+
+        self.assertIn('{http://example.com/stockquote.xsd}SubscribeToQuotes',
+                      wsdl_document.schema.maps.elements)
+        self.assertIn('{http://example.com/stockquote.xsd}SubscriptionHeader',
+                      wsdl_document.schema.maps.elements)
+
     def test_example4(self):
         original_example4_file = casepath('features/wsdl/wsdl11_example4.wsdl')
         with self.assertRaises(XMLSchemaValidationError):
             Wsdl11Document(original_example4_file)
 
         example_4_file = casepath('features/wsdl/wsdl11_example4_valid.wsdl')
         wsdl_document = Wsdl11Document(example_4_file)
```

### Comparing `xmlschema-2.2.3/tests/test_xpath.py` & `xmlschema-2.3.0/tests/test_xpath.py`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.3/tests/validation/test_decoding.py` & `xmlschema-2.3.0/tests/validation/test_decoding.py`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.3/tests/validation/test_encoding.py` & `xmlschema-2.3.0/tests/validation/test_encoding.py`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.3/tests/validation/test_validation.py` & `xmlschema-2.3.0/tests/validation/test_validation.py`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.3/tests/validators/test_attributes.py` & `xmlschema-2.3.0/tests/validators/test_attributes.py`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.3/tests/validators/test_builtins.py` & `xmlschema-2.3.0/tests/validators/test_builtins.py`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.3/tests/validators/test_complex_types.py` & `xmlschema-2.3.0/tests/validators/test_complex_types.py`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.3/tests/validators/test_elements.py` & `xmlschema-2.3.0/tests/validators/test_elements.py`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.3/tests/validators/test_exceptions.py` & `xmlschema-2.3.0/tests/validators/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.3/tests/validators/test_facets.py` & `xmlschema-2.3.0/tests/validators/test_facets.py`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.3/tests/validators/test_global_maps.py` & `xmlschema-2.3.0/tests/validators/test_global_maps.py`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.3/tests/validators/test_groups.py` & `xmlschema-2.3.0/tests/validators/test_groups.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,14 +26,18 @@
             raise XMLSchemaValueError("invalid model {!r} for a group".format(model))
         self._group: List[Union[ParticleMixin, 'ModelGroup']] = []
         self.model: str = model
 
     def __repr__(self) -> str:
         return '%s(model=%r, occurs=%r)' % (self.__class__.__name__, self.model, self.occurs)
 
+    @property
+    def xsd_version(self) -> str:
+        return '1.0'
+
     append: Any
 
 
 class TestXsdGroups(unittest.TestCase):
 
     def test_model_group_init(self):
         group = ModelGroup('sequence')
```

### Comparing `xmlschema-2.2.3/tests/validators/test_identities.py` & `xmlschema-2.3.0/tests/validators/test_identities.py`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.3/tests/validators/test_models.py` & `xmlschema-2.3.0/tests/validators/test_models.py`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.3/tests/validators/test_notations.py` & `xmlschema-2.3.0/tests/validators/test_notations.py`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.3/tests/validators/test_particles.py` & `xmlschema-2.3.0/tests/validators/test_particles.py`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.3/tests/validators/test_schemas.py` & `xmlschema-2.3.0/tests/validators/test_schemas.py`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.3/tests/validators/test_simple_types.py` & `xmlschema-2.3.0/tests/validators/test_simple_types.py`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.3/tests/validators/test_wildcards.py` & `xmlschema-2.3.0/tests/validators/test_wildcards.py`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.3/tests/validators/test_xsdbase.py` & `xmlschema-2.3.0/tests/validators/test_xsdbase.py`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.3/tox.ini` & `xmlschema-2.3.0/tox.ini`

 * *Files 12% similar despite different names*

```diff
@@ -1,36 +1,31 @@
 [tox]
-envlist = py{37,38,39,310,311,312,py3}, ep{40}, docs,
+envlist = py{37,38,39,310,311,312,py3}, docs,
     flake8, mypy-py{37,38,39,310,311,312,py3}, coverage, pytest
 skip_missing_interpreters = true
 work_dir = {tox_root}/../.tox/xmlschema
 
 [testenv]
 deps =
-    elementpath>=4.0.0, <5.0.0
+    elementpath>=4.1.2, <5.0.0
     lxml
     jinja2
     py{310,311}: memory_profiler
     docs: Sphinx
     docs: sphinx_rtd_theme
     coverage: coverage
 commands =
     python -m unittest
 
 [testenv:py312]
 deps =
-    elementpath>=4.0.0, <5.0.0
+    elementpath>=4.1.2, <5.0.0
     # lxml: skip for now
     jinja2
 
-[testenv:ep40]
-deps =
-    elementpath~=4.0.0
-    lxml
-
 [testenv:docs]
 commands =
     make -C doc html SPHINXOPTS="-W -n"
     make -C doc latexpdf SPHINXOPTS="-W -n"
     make -C doc doctest SPHINXOPTS="-W -n"
     sphinx-build -W -n -T -b man doc build/sphinx/man
 allowlist_externals = make
@@ -43,25 +38,25 @@
     flake8
 commands =
     flake8 xmlschema
     flake8 tests
 
 [testenv:mypy-py37]
 deps =
-    mypy==1.2.0
-    elementpath==4.1.1
+    mypy==1.3.0
+    elementpath==4.1.2
     lxml-stubs
     jinja2
 commands =
     mypy --config-file {toxinidir}/mypy.ini xmlschema
 
 [testenv:mypy-py{38,39,310,311,312,py3}]
 deps =
-    mypy==1.2.0
-    elementpath==4.1.1
+    mypy==1.3.0
+    elementpath==4.1.2
     lxml-stubs
     jinja2
 commands =
     mypy --config-file {toxinidir}/mypy.ini xmlschema
     python tests/test_typing.py
 
 [testenv:coverage]
@@ -70,18 +65,18 @@
     coverage run -a -m unittest
     coverage report -m
 
 [testenv:pytest]
 deps =
     pytest
     pytest-randomly
-    elementpath>=4.0.0, <5.0.0
+    elementpath>=4.1.2, <5.0.0
     lxml
     jinja2
-    mypy==1.2.0
+    mypy==1.3.0
     lxml-stubs
 commands =
     pytest tests -ra
 
 [testenv:build]
 deps =
     setuptools
```

### Comparing `xmlschema-2.2.3/xmlschema/__init__.py` & `xmlschema-2.3.0/xmlschema/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     XMLSchemaModelError, XMLSchemaModelDepthError, XMLSchemaValidationError,
     XMLSchemaDecodeError, XMLSchemaEncodeError, XMLSchemaChildrenValidationError,
     XMLSchemaIncludeWarning, XMLSchemaImportWarning, XMLSchemaTypeTableWarning,
     XsdGlobals, XMLSchemaBase, XMLSchema, XMLSchema10, XMLSchema11,
     XsdComponent, XsdType, XsdElement, XsdAttribute
 )
 
-__version__ = '2.2.3'
+__version__ = '2.3.0'
 __author__ = "Davide Brunato"
 __contact__ = "brunato@sissa.it"
 __copyright__ = "Copyright 2016-2023, SISSA"
 __license__ = "MIT"
 __status__ = "Production/Stable"
 
 __all__ = [
```

### Comparing `xmlschema-2.2.3/xmlschema/aliases.py` & `xmlschema-2.3.0/xmlschema/aliases.py`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.3/xmlschema/cli.py` & `xmlschema-2.3.0/xmlschema/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # All rights reserved.
 # This file is distributed under the terms of the MIT License.
 # See the file 'LICENSE' in the root directory of the present
 # distribution, or http://opensource.org/licenses/MIT.
 #
 # @author Davide Brunato <brunato@sissa.it>
 #
-# type: ignore
+# mypy: ignore-errors
 """Command Line Interface"""
 import sys
 import os
 import argparse
 import logging
 import pathlib
 from urllib.error import URLError
```

### Comparing `xmlschema-2.2.3/xmlschema/converters/__init__.py` & `xmlschema-2.3.0/xmlschema/converters/__init__.py`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.3/xmlschema/converters/abdera.py` & `xmlschema-2.3.0/xmlschema/converters/abdera.py`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.3/xmlschema/converters/badgerfish.py` & `xmlschema-2.3.0/xmlschema/converters/badgerfish.py`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.3/xmlschema/converters/columnar.py` & `xmlschema-2.3.0/xmlschema/converters/columnar.py`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.3/xmlschema/converters/default.py` & `xmlschema-2.3.0/xmlschema/converters/default.py`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.3/xmlschema/converters/jsonml.py` & `xmlschema-2.3.0/xmlschema/converters/jsonml.py`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.3/xmlschema/converters/parker.py` & `xmlschema-2.3.0/xmlschema/converters/parker.py`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.3/xmlschema/converters/unordered.py` & `xmlschema-2.3.0/xmlschema/converters/unordered.py`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.3/xmlschema/dataobjects.py` & `xmlschema-2.3.0/xmlschema/dataobjects.py`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.3/xmlschema/documents.py` & `xmlschema-2.3.0/xmlschema/documents.py`

 * *Files 1% similar despite different names*

```diff
@@ -539,14 +539,17 @@
     :param locations: resource location hints, that can be a dictionary or a \
     sequence of couples (namespace URI, resource URL).
     :param base_url: the base URL for base :class:`xmlschema.XMLResource` initialization.
     :param allow: the security mode for base :class:`xmlschema.XMLResource` initialization.
     :param defuse: the defuse mode for base :class:`xmlschema.XMLResource` initialization.
     :param timeout: the timeout for base :class:`xmlschema.XMLResource` initialization.
     :param lazy: the lazy mode for base :class:`xmlschema.XMLResource` initialization.
+    :param use_location_hints: for default, in case a schema instance has \
+    to be built, uses also schema locations hints provided within XML data. \
+    Set this option to `False` to ignore these schema location hints.
     """
     schema: Optional[XMLSchemaBase] = None
     _fallback_schema: Optional[XMLSchemaBase] = None
     validation: str = 'skip'
     namespaces: Optional[NamespacesType] = None
     errors: Union[Tuple[()], List[XMLSchemaValidationError]] = ()
```

### Comparing `xmlschema-2.2.3/xmlschema/exceptions.py` & `xmlschema-2.3.0/xmlschema/exceptions.py`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.3/xmlschema/extras/codegen.py` & `xmlschema-2.3.0/xmlschema/extras/codegen.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # All rights reserved.
 # This file is distributed under the terms of the MIT License.
 # See the file 'LICENSE' in the root directory of the present
 # distribution, or http://opensource.org/licenses/MIT.
 #
 # @author Davide Brunato <brunato@sissa.it>
 #
-# type: ignore
+# mypy: ignore-errors
 """
 This module contains abstact base class and helper
 functions for building XSD based code generators.
 """
 import os
 import re
 import sys
```

### Comparing `xmlschema-2.2.3/xmlschema/extras/templates/python/bindings.py.jinja` & `xmlschema-2.3.0/xmlschema/extras/templates/python/bindings.py.jinja`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.3/xmlschema/extras/templates/python/sample.py.jinja` & `xmlschema-2.3.0/xmlschema/extras/templates/python/sample.py.jinja`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.3/xmlschema/extras/wsdl.py` & `xmlschema-2.3.0/xmlschema/extras/wsdl.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,25 +3,25 @@
 # All rights reserved.
 # This file is distributed under the terms of the MIT License.
 # See the file 'LICENSE' in the root directory of the present
 # distribution, or http://opensource.org/licenses/MIT.
 #
 # @author Davide Brunato <brunato@sissa.it>
 #
-# type: ignore
+# mypy: ignore-errors
 import os
 
 from ..exceptions import XMLSchemaException, XMLSchemaValueError
 from ..names import XSD_NAMESPACE, WSDL_NAMESPACE, SOAP_NAMESPACE, \
     SCHEMAS_DIR, XSD_ANY_TYPE, XSD_SCHEMA
 from ..helpers import get_qname, local_name, get_extended_qname, get_prefixed_qname
 from ..namespaces import NamespaceResourcesMap
 from ..resources import fetch_resource
 from ..documents import XmlDocument
-from ..validators import XMLSchema10
+from ..validators import XMLSchemaBase, XMLSchema10
 
 
 # WSDL 1.1 global declarations
 WSDL_IMPORT = '{%s}import' % WSDL_NAMESPACE
 WSDL_TYPES = '{%s}types' % WSDL_NAMESPACE
 WSDL_MESSAGE = '{%s}message' % WSDL_NAMESPACE
 WSDL_PORT_TYPE = '{%s}portType' % WSDL_NAMESPACE
@@ -459,14 +459,17 @@
 
 class Wsdl11Document(XmlDocument):
     """
     Class for WSDL 1.1 documents.
 
     :param source: a string containing XML data or a file path or an URL or a \
     file like object or an ElementTree or an Element.
+    :param schema: additional schema for providing XSD types and elements to the \
+    WSDL document. Can be a :class:`xmlschema.XMLSchema` instance or a file-like \
+    object or a file path or a URL of a resource or a string containing the XSD schema.
     :param cls: class to use for building the schema instance (for default \
     :class:`xmlschema.XMLSchema10` is used).
     :param validation: the XSD validation mode to use for validating the XML document, \
     that can be 'strict' (default), 'lax' or 'skip'.
     :param maps: WSDL definitions shared maps.
     :param namespaces: is an optional mapping from namespace prefix to URI.
     :param locations: resource location hints, that can be a dictionary or a \
@@ -475,25 +478,38 @@
     :param allow: the security mode for base :class:`xmlschema.XMLResource` initialization.
     :param defuse: the defuse mode for base :class:`xmlschema.XMLResource` initialization.
     :param timeout: the timeout for base :class:`xmlschema.XMLResource` initialization.
     """
     target_namespace = ''
     soap_binding = False
 
-    def __init__(self, source, cls=None, validation='strict', namespaces=None, maps=None,
-                 locations=None, base_url=None, allow='all', defuse='remote', timeout=300):
+    def __init__(self, source, schema=None, cls=None, validation='strict',
+                 namespaces=None, maps=None, locations=None, base_url=None,
+                 allow='all', defuse='remote', timeout=300):
 
-        if maps is None:
+        if maps is not None:
+            self.maps = maps
+            self.schema = maps.wsdl_document.schema
+        else:
             if cls is None:
                 cls = XMLSchema10
-            self.schema = cls(source=os.path.join(SCHEMAS_DIR, 'WSDL/wsdl.xsd'))
+
+            if isinstance(schema, XMLSchemaBase):
+                cls = schema.__class__
+                global_maps = schema.maps
+            elif schema is not None:
+                global_maps = cls(schema).maps
+            else:
+                global_maps = None
+
+            self.schema = cls(
+                source=os.path.join(SCHEMAS_DIR, 'WSDL/wsdl.xsd'),
+                global_maps=global_maps,
+            )
             self.maps = Wsdl11Maps(self)
-        else:
-            self.schema = maps.wsdl_document.schema
-            self.maps = maps
 
         if locations:
             self.locations = NamespaceResourcesMap(locations)
         else:
             self.locations = NamespaceResourcesMap()
 
         super(Wsdl11Document, self).__init__(
```

### Comparing `xmlschema-2.2.3/xmlschema/helpers.py` & `xmlschema-2.3.0/xmlschema/helpers.py`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.3/xmlschema/limits.py` & `xmlschema-2.3.0/xmlschema/limits.py`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.3/xmlschema/locale/en/LC_MESSAGES/xmlschema.mo` & `xmlschema-2.3.0/xmlschema/locale/en/LC_MESSAGES/xmlschema.mo`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.3/xmlschema/locale/en/LC_MESSAGES/xmlschema.po` & `xmlschema-2.3.0/xmlschema/locale/en/LC_MESSAGES/xmlschema.po`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.3/xmlschema/locale/it/LC_MESSAGES/xmlschema.mo` & `xmlschema-2.3.0/xmlschema/locale/it/LC_MESSAGES/xmlschema.mo`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.3/xmlschema/locale/it/LC_MESSAGES/xmlschema.po` & `xmlschema-2.3.0/xmlschema/locale/it/LC_MESSAGES/xmlschema.po`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.3/xmlschema/locale/ru/LC_MESSAGES/xmlschema.mo` & `xmlschema-2.3.0/xmlschema/locale/ru/LC_MESSAGES/xmlschema.mo`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.3/xmlschema/locale/ru/LC_MESSAGES/xmlschema.po` & `xmlschema-2.3.0/xmlschema/locale/ru/LC_MESSAGES/xmlschema.po`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.3/xmlschema/names.py` & `xmlschema-2.3.0/xmlschema/names.py`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.3/xmlschema/namespaces.py` & `xmlschema-2.3.0/xmlschema/namespaces.py`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.3/xmlschema/resources.py` & `xmlschema-2.3.0/xmlschema/resources.py`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.3/xmlschema/schemas/HFP/XMLSchema-hasFacetAndProperty_minimal.xsd` & `xmlschema-2.3.0/xmlschema/schemas/HFP/XMLSchema-hasFacetAndProperty_minimal.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.3/xmlschema/schemas/VC/XMLSchema-versioning.xsd` & `xmlschema-2.3.0/xmlschema/schemas/VC/XMLSchema-versioning.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.3/xmlschema/schemas/WSDL/soap-encoding.xsd` & `xmlschema-2.3.0/xmlschema/schemas/WSDL/soap-encoding.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.3/xmlschema/schemas/WSDL/soap-envelope.xsd` & `xmlschema-2.3.0/xmlschema/schemas/WSDL/soap-envelope.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.3/xmlschema/schemas/WSDL/wsdl-soap.xsd` & `xmlschema-2.3.0/xmlschema/schemas/WSDL/wsdl-soap.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.3/xmlschema/schemas/WSDL/wsdl.xsd` & `xmlschema-2.3.0/xmlschema/schemas/WSDL/wsdl.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.3/xmlschema/schemas/XHTML/xhtml1-strict.xsd` & `xmlschema-2.3.0/xmlschema/schemas/XHTML/xhtml1-strict.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.3/xmlschema/schemas/XLINK/xlink.xsd` & `xmlschema-2.3.0/xmlschema/schemas/XLINK/xlink.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.3/xmlschema/schemas/XML/xml_minimal.xsd` & `xmlschema-2.3.0/xmlschema/schemas/XML/xml_minimal.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.3/xmlschema/schemas/XSD_1.0/XMLSchema.xsd` & `xmlschema-2.3.0/xmlschema/schemas/XSD_1.0/XMLSchema.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.3/xmlschema/schemas/XSD_1.0/datatypes.xsd` & `xmlschema-2.3.0/xmlschema/schemas/XSD_1.0/datatypes.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.3/xmlschema/schemas/XSD_1.1/XMLSchema.xsd` & `xmlschema-2.3.0/xmlschema/schemas/XSD_1.1/XMLSchema.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.3/xmlschema/schemas/XSD_1.1/datatypes.xsd` & `xmlschema-2.3.0/xmlschema/schemas/XSD_1.1/datatypes.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.3/xmlschema/schemas/XSD_1.1/xsd11-extra.xsd` & `xmlschema-2.3.0/xmlschema/schemas/XSD_1.1/xsd11-extra.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.3/xmlschema/testing/__init__.py` & `xmlschema-2.3.0/xmlschema/testing/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # All rights reserved.
 # This file is distributed under the terms of the MIT License.
 # See the file 'LICENSE' in the root directory of the present
 # distribution, or http://opensource.org/licenses/MIT.
 #
 # @author Davide Brunato <brunato@sissa.it>
 #
-# type: ignore
+# mypy: ignore-errors
 """
 Subpackage with unittest extensions for xmlschema.
 
 Includes common classes and helpers for building test scripts for xmlschema. The main
 part is a test factory for creating test cases from lists of paths to XSD or XML files.
 The list of cases can be defined within files named "testfiles". These are text files
 that contain a list of relative paths to XSD or XML files, that are used to dinamically
```

### Comparing `xmlschema-2.2.3/xmlschema/testing/_builders.py` & `xmlschema-2.3.0/xmlschema/testing/_builders.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # All rights reserved.
 # This file is distributed under the terms of the MIT License.
 # See the file 'LICENSE' in the root directory of the present
 # distribution, or http://opensource.org/licenses/MIT.
 #
 # @author Davide Brunato <brunato@sissa.it>
 #
-# type: ignore
+# mypy: ignore-errors
 import pdb
 import os
 import ast
 import pickle
 import time
 import logging
 import importlib
```

### Comparing `xmlschema-2.2.3/xmlschema/testing/_case_class.py` & `xmlschema-2.3.0/xmlschema/testing/_case_class.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # All rights reserved.
 # This file is distributed under the terms of the MIT License.
 # See the file 'LICENSE' in the root directory of the present
 # distribution, or http://opensource.org/licenses/MIT.
 #
 # @author Davide Brunato <brunato@sissa.it>
 #
-# type: ignore
+# mypy: ignore-errors
 """
 Tests subpackage module: common definitions for unittest scripts of the 'xmlschema' package.
 """
 import unittest
 import re
 import os
 from textwrap import dedent
```

### Comparing `xmlschema-2.2.3/xmlschema/testing/_factory.py` & `xmlschema-2.3.0/xmlschema/testing/_factory.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # All rights reserved.
 # This file is distributed under the terms of the MIT License.
 # See the file 'LICENSE' in the root directory of the present
 # distribution, or http://opensource.org/licenses/MIT.
 #
 # @author Davide Brunato <brunato@sissa.it>
 #
-# type: ignore
+# mypy: ignore-errors
 """
 Test factory for creating test cases from lists of paths to XSD or XML files.
 
 The list of cases can be defined within files named "testfiles". These are text files
 that contain a list of relative paths to XSD or XML files, that are used to dinamically
 build a set of test classes. Each path is followed by a list of options that defines a
 custom setting for each test.
```

### Comparing `xmlschema-2.2.3/xmlschema/testing/_helpers.py` & `xmlschema-2.3.0/xmlschema/testing/_helpers.py`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.3/xmlschema/testing/_observers.py` & `xmlschema-2.3.0/xmlschema/testing/_observers.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # All rights reserved.
 # This file is distributed under the terms of the MIT License.
 # See the file 'LICENSE' in the root directory of the present
 # distribution, or http://opensource.org/licenses/MIT.
 #
 # @author Davide Brunato <brunato@sissa.it>
 #
-# type: ignore
+# mypy: ignore-errors
 """
 Observers for testing XMLSchema classes.
 """
 from functools import wraps
 
 from ..names import XSD_NAMESPACE, XSD_ANY_TYPE
 from ..validators import XMLSchema10, XMLSchema11, XsdGroup, \
```

### Comparing `xmlschema-2.2.3/xmlschema/translation.py` & `xmlschema-2.3.0/xmlschema/translation.py`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.3/xmlschema/validators/__init__.py` & `xmlschema-2.3.0/xmlschema/validators/__init__.py`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.3/xmlschema/validators/assertions.py` & `xmlschema-2.3.0/xmlschema/validators/assertions.py`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.3/xmlschema/validators/attributes.py` & `xmlschema-2.3.0/xmlschema/validators/attributes.py`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.3/xmlschema/validators/builtins.py` & `xmlschema-2.3.0/xmlschema/validators/builtins.py`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.3/xmlschema/validators/complex_types.py` & `xmlschema-2.3.0/xmlschema/validators/complex_types.py`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.3/xmlschema/validators/elements.py` & `xmlschema-2.3.0/xmlschema/validators/elements.py`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.3/xmlschema/validators/exceptions.py` & `xmlschema-2.3.0/xmlschema/validators/exceptions.py`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.3/xmlschema/validators/facets.py` & `xmlschema-2.3.0/xmlschema/validators/facets.py`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.3/xmlschema/validators/global_maps.py` & `xmlschema-2.3.0/xmlschema/validators/global_maps.py`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.3/xmlschema/validators/groups.py` & `xmlschema-2.3.0/xmlschema/validators/groups.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,16 +9,16 @@
 #
 """
 This module contains classes for XML Schema model groups.
 """
 import warnings
 from collections.abc import MutableMapping
 from copy import copy as _copy
-from typing import TYPE_CHECKING, overload, Any, Iterable, Iterator, List, \
-    MutableSequence, Optional, Tuple, Union
+from typing import TYPE_CHECKING, cast, overload, Any, Iterable, Iterator, \
+    List, MutableSequence, Optional, Tuple, Union
 from xml.etree import ElementTree
 
 from .. import limits
 from ..exceptions import XMLSchemaValueError
 from ..names import XSD_GROUP, XSD_SEQUENCE, XSD_ALL, XSD_CHOICE, XSD_ELEMENT, \
     XSD_ANY, XSI_TYPE, XSD_ANY_TYPE, XSD_ANNOTATION
 from ..aliases import ElementType, NamespacesType, SchemaType, IterDecodeType, \
@@ -192,57 +192,77 @@
         else:
             return True
 
     @property
     def effective_min_occurs(self) -> int:
         if not self.min_occurs or not self:
             return 0
+
+        effective_items: List[Any]
+        min_occurs: int
+        effective_items = [e for e in self.iter_model() if e.effective_max_occurs != 0]
+        if not effective_items:
+            return 0
         elif self.model == 'choice':
-            if any(not e.effective_min_occurs for e in self.iter_model()):
-                return 0
-        else:
-            if all(not e.effective_min_occurs for e in self.iter_model()):
-                return 0
-        return self.min_occurs
+            min_occurs = min(e.effective_min_occurs for e in effective_items)
+            return self.min_occurs * min_occurs
+        elif self.model == 'all':
+            min_occurs = max(e.effective_min_occurs for e in effective_items)
+            return min_occurs
+
+        not_emptiable_items = [e for e in effective_items if e.effective_min_occurs]
+        if not not_emptiable_items:
+            return 0
+        elif len(not_emptiable_items) > 1:
+            return self.min_occurs
+
+        min_occurs = not_emptiable_items[0].effective_min_occurs
+        return self.min_occurs * min_occurs
 
     @property
     def effective_max_occurs(self) -> Optional[int]:
         if self.max_occurs == 0 or not self:
             return 0
 
         effective_items: List[Any]
-        value: int
+        max_occurs: int
 
-        effective_items = [e for e in self.iter_model() if e.effective_max_occurs != 0]
+        model_items = [(e, e.effective_max_occurs) for e in self.iter_model()]
+        effective_items = [x for x in model_items if x[1] != 0]
         if not effective_items:
             return 0
         elif self.max_occurs is None:
             return None
         elif self.model == 'choice':
-            try:
-                value = max(e.effective_max_occurs for e in effective_items)
-            except TypeError:
+            if any(x[1] is None for x in effective_items):
                 return None
             else:
-                return self.max_occurs * value
+                max_occurs = max(x[1] for x in effective_items)
+                return self.max_occurs * max_occurs
 
-        not_emptiable_items = [e for e in effective_items if e.effective_min_occurs]
+        not_emptiable_items = [x for x in effective_items if x[0].effective_min_occurs]
         if not not_emptiable_items:
-            try:
-                value = max(e.effective_max_occurs for e in effective_items)
-            except TypeError:
+            if any(x[1] is None for x in effective_items):
                 return None
             else:
-                return self.max_occurs * value
+                max_occurs = max(x[1] for x in effective_items)
+                return self.max_occurs * max_occurs
 
         elif len(not_emptiable_items) > 1:
-            return self.max_occurs
-
-        value = not_emptiable_items[0].effective_max_occurs
-        return None if value is None else self.max_occurs * value
+            if self.model == 'sequence':
+                return self.max_occurs
+            elif all(x[1] is None for x in not_emptiable_items):
+                return None
+            else:
+                max_occurs = min(x[1] for x in not_emptiable_items if x[1] is not None)
+                return max_occurs
+        elif not_emptiable_items[0][1] is None:
+            return None
+        else:
+            return self.max_occurs * cast(int, not_emptiable_items[0][1])
 
     def has_occurs_restriction(
             self, other: Union[ModelParticleType, ParticleMixin, 'OccursCalculator']) -> bool:
 
         if not self:
             return True
         elif isinstance(other, XsdGroup):
@@ -1276,14 +1296,34 @@
         if other.model == 'sequence':
             return self.is_sequence_restriction(other)
         elif other.model == 'all':
             return self.is_all_restriction(other)
         else:  # other.model == 'choice':
             return self.is_choice_restriction(other)
 
+    def has_occurs_restriction(
+            self, other: Union[ModelParticleType, ParticleMixin, 'OccursCalculator']) -> bool:
+        if not isinstance(other, XsdGroup):
+            return super().has_occurs_restriction(other)
+        elif not self:
+            return True
+        elif self.effective_min_occurs < other.effective_min_occurs:
+            return False
+
+        effective_max_occurs = self.effective_max_occurs
+        if effective_max_occurs == 0:
+            return True
+        elif effective_max_occurs is None:
+            return other.effective_max_occurs is None
+
+        try:
+            return effective_max_occurs <= other.effective_max_occurs  # type: ignore[operator]
+        except TypeError:
+            return True
+
     def is_sequence_restriction(self, other: XsdGroup) -> bool:
         if not self.has_occurs_restriction(other):
             return False
 
         check_occurs = other.max_occurs != 0
 
         item_iterator = iter(self.iter_model())
@@ -1302,20 +1342,30 @@
         item_iterator = iter(self)
         item = next(item_iterator, None)
 
         for other_item in other.iter_model():
             if item is not None and item.is_restriction(other_item, check_occurs):
                 item = next(item_iterator, None)
             elif not other_item.is_emptiable():
+                break
+        else:
+            if item is None:
+                return True
+
+        # Restriction check failed again: try checking other items against self
+        other_items = other.iter_model()
+        for other_item in other_items:
+            if self.is_restriction(other_item, check_occurs):
+                return all(x.is_emptiable() for x in other_items)
+            elif not other_item.is_emptiable():
                 return False
-        return item is None
+        else:
+            return False
 
     def is_all_restriction(self, other: XsdGroup) -> bool:
-        if not self.has_occurs_restriction(other):
-            return False
         restriction_items = [x for x in self.iter_model()]
 
         base_items = [x for x in other.iter_model()]
 
         # If the base includes more wildcard, calculates and appends a
         # wildcard union for validating wildcard unions in restriction
         wildcards: List[XsdAnyElement] = []
```

### Comparing `xmlschema-2.2.3/xmlschema/validators/helpers.py` & `xmlschema-2.3.0/xmlschema/validators/helpers.py`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.3/xmlschema/validators/identities.py` & `xmlschema-2.3.0/xmlschema/validators/identities.py`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.3/xmlschema/validators/models.py` & `xmlschema-2.3.0/xmlschema/validators/models.py`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.3/xmlschema/validators/notations.py` & `xmlschema-2.3.0/xmlschema/validators/notations.py`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.3/xmlschema/validators/particles.py` & `xmlschema-2.3.0/xmlschema/validators/particles.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,25 +40,26 @@
         return self.min_occurs, self.max_occurs
 
     @property
     def effective_min_occurs(self) -> int:
         """
         A property calculated from minOccurs, that is equal to minOccurs
         for elements and may vary for content model groups, in dependance
-        of group model and structure.
+        of group model and structure. Used for checking restrictions of
+        model groups in XSD 1.1.
         """
         return self.min_occurs
 
     @property
     def effective_max_occurs(self) -> Optional[int]:
         """
         A property calculated from maxOccurs, that is equal to maxOccurs
         for elements and may vary for content model groups, in dependance
         of group model and structure. Used for checking restrictions of
-        xs:choice model groups in XSD 1.1.
+        model groups in XSD 1.1.
         """
         return self.max_occurs
 
     def is_emptiable(self) -> bool:
         """
         Tests if max_occurs == 0. A zero-length model group is considered emptiable.
         For model groups the test outcome depends also on nested particles.
```

### Comparing `xmlschema-2.2.3/xmlschema/validators/schemas.py` & `xmlschema-2.3.0/xmlschema/validators/schemas.py`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.3/xmlschema/validators/simple_types.py` & `xmlschema-2.3.0/xmlschema/validators/simple_types.py`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.3/xmlschema/validators/wildcards.py` & `xmlschema-2.3.0/xmlschema/validators/wildcards.py`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.3/xmlschema/validators/xsdbase.py` & `xmlschema-2.3.0/xmlschema/validators/xsdbase.py`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.3/xmlschema/xpath.py` & `xmlschema-2.3.0/xmlschema/xpath.py`

 * *Files identical despite different names*

### Comparing `xmlschema-2.2.3/xmlschema.egg-info/PKG-INFO` & `xmlschema-2.3.0/xmlschema.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xmlschema
-Version: 2.2.3
+Version: 2.3.0
 Summary: An XML Schema validator and decoder
 Home-page: https://github.com/sissaschool/xmlschema
 Author: Davide Brunato
 Author-email: brunato@sissa.it
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `xmlschema-2.2.3/xmlschema.egg-info/SOURCES.txt` & `xmlschema-2.3.0/xmlschema.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -91,17 +91,18 @@
 tests/test_cases/features/decoder/data3.xml
 tests/test_cases/features/decoder/data4-mixed.xml
 tests/test_cases/features/decoder/long-sequence-1.xsd
 tests/test_cases/features/decoder/mixed-content.xsd
 tests/test_cases/features/decoder/simple-types.xsd
 tests/test_cases/features/derivations/complex-extensions.xsd
 tests/test_cases/features/derivations/complex-with-simple-content-restriction.xsd
-tests/test_cases/features/derivations/invalid_enumeration_restriction.xsd
-tests/test_cases/features/derivations/invalid_restrictions1.xsd
-tests/test_cases/features/derivations/invalid_restrictions2.xsd
+tests/test_cases/features/derivations/complex11-restrictions.xsd
+tests/test_cases/features/derivations/invalid-enumeration-restriction.xsd
+tests/test_cases/features/derivations/invalid-restrictions1.xsd
+tests/test_cases/features/derivations/invalid-restrictions2.xsd
 tests/test_cases/features/derivations/list_types.xml
 tests/test_cases/features/derivations/list_types.xsd
 tests/test_cases/features/elements/test_alternatives-1.xml
 tests/test_cases/features/elements/type_alternatives-no-ns.xsd
 tests/test_cases/features/elements/type_alternatives.xsd
 tests/test_cases/features/models/billion_laughs_model.xsd
 tests/test_cases/features/models/circular_model.xsd
@@ -142,14 +143,16 @@
 tests/test_cases/features/namespaces/included3-valid.xsd
 tests/test_cases/features/namespaces/included4-invalid.xsd
 tests/test_cases/features/namespaces/included5-valid.xsd
 tests/test_cases/features/namespaces/included6-invalid.xsd
 tests/test_cases/features/patterns/patterns.xml
 tests/test_cases/features/patterns/patterns.xsd
 tests/test_cases/features/wsdl/wsdl11_example3.wsdl
+tests/test_cases/features/wsdl/wsdl11_example3_no_types.wsdl
+tests/test_cases/features/wsdl/wsdl11_example3_types.xsd
 tests/test_cases/features/wsdl/wsdl11_example3_valid.wsdl
 tests/test_cases/features/wsdl/wsdl11_example4.wsdl
 tests/test_cases/features/wsdl/wsdl11_example4_valid.wsdl
 tests/test_cases/features/wsdl/wsdl11_example5.wsdl
 tests/test_cases/features/wsdl/wsdl11_example5_valid.wsdl
 tests/test_cases/features/wsdl/wsdl11_example5_with_fault.wsdl
 tests/test_cases/issues/issue_008/issue_008.xml
```

