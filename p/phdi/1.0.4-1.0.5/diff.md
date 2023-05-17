# Comparing `tmp/phdi-1.0.4.tar.gz` & `tmp/phdi-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "phdi-1.0.4.tar", max compression
+gzip compressed data, was "phdi-1.0.5.tar", max compression
```

## Comparing `phdi-1.0.4.tar` & `phdi-1.0.5.tar`

### file list

```diff
@@ -1,68 +1,68 @@
--rw-r--r--   0        0        0     7048 2023-05-17 20:18:00.188969 phdi-1.0.4/LICENSE.md
--rw-r--r--   0        0        0    11787 2023-05-17 20:18:00.188969 phdi-1.0.4/README.md
--rw-r--r--   0        0        0       27 2023-05-17 20:18:00.696973 phdi-1.0.4/phdi/__init__.py
--rw-r--r--   0        0        0      223 2023-05-17 20:18:00.696973 phdi-1.0.4/phdi/cloud/README.md
--rw-r--r--   0        0        0        0 2023-05-17 20:18:00.696973 phdi-1.0.4/phdi/cloud/__init__.py
--rw-r--r--   0        0        0     9436 2023-05-17 20:18:00.696973 phdi-1.0.4/phdi/cloud/azure.py
--rw-r--r--   0        0        0     2516 2023-05-17 20:18:00.696973 phdi-1.0.4/phdi/cloud/core.py
--rw-r--r--   0        0        0     6055 2023-05-17 20:18:00.696973 phdi-1.0.4/phdi/cloud/gcp.py
--rw-r--r--   0        0        0      163 2023-05-17 20:18:00.696973 phdi-1.0.4/phdi/containers/README.md
--rw-r--r--   0        0        0        0 2023-05-17 20:18:00.696973 phdi-1.0.4/phdi/containers/__init__.py
--rw-r--r--   0        0        0     2776 2023-05-17 20:18:00.696973 phdi-1.0.4/phdi/containers/base_service.py
--rw-r--r--   0        0        0        0 2023-05-17 20:18:00.696973 phdi-1.0.4/phdi/fhir/__init__.py
--rw-r--r--   0        0        0      292 2023-05-17 20:18:00.696973 phdi-1.0.4/phdi/fhir/cloud/README.md
--rw-r--r--   0        0        0      119 2023-05-17 20:18:00.696973 phdi-1.0.4/phdi/fhir/cloud/__init__.py
--rw-r--r--   0        0        0     2111 2023-05-17 20:18:00.696973 phdi-1.0.4/phdi/fhir/cloud/azure.py
--rw-r--r--   0        0        0      311 2023-05-17 20:18:00.696973 phdi-1.0.4/phdi/fhir/conversion/README.md
--rw-r--r--   0        0        0       89 2023-05-17 20:18:00.696973 phdi-1.0.4/phdi/fhir/conversion/__init__.py
--rw-r--r--   0        0        0     8026 2023-05-17 20:18:00.696973 phdi-1.0.4/phdi/fhir/conversion/convert.py
--rw-r--r--   0        0        0      808 2023-05-17 20:18:00.696973 phdi-1.0.4/phdi/fhir/geospatial/README.md
--rw-r--r--   0        0        0      294 2023-05-17 20:18:00.696973 phdi-1.0.4/phdi/fhir/geospatial/__init__.py
--rw-r--r--   0        0        0     3494 2023-05-17 20:18:00.696973 phdi-1.0.4/phdi/fhir/geospatial/census.py
--rw-r--r--   0        0        0     4521 2023-05-17 20:18:00.696973 phdi-1.0.4/phdi/fhir/geospatial/core.py
--rw-r--r--   0        0        0     3587 2023-05-17 20:18:00.696973 phdi-1.0.4/phdi/fhir/geospatial/smarty.py
--rw-r--r--   0        0        0      890 2023-05-17 20:18:00.696973 phdi-1.0.4/phdi/fhir/harmonization/README.md
--rw-r--r--   0        0        0      335 2023-05-17 20:18:00.696973 phdi-1.0.4/phdi/fhir/harmonization/__init__.py
--rw-r--r--   0        0        0    11809 2023-05-17 20:18:00.696973 phdi-1.0.4/phdi/fhir/harmonization/standardization.py
--rw-r--r--   0        0        0      179 2023-05-17 20:18:00.696973 phdi-1.0.4/phdi/fhir/linkage/__init__.py
--rw-r--r--   0        0        0     3591 2023-05-17 20:18:00.696973 phdi-1.0.4/phdi/fhir/linkage/link.py
--rw-r--r--   0        0        0      412 2023-05-17 20:18:00.700973 phdi-1.0.4/phdi/fhir/tabulation/README.md
--rw-r--r--   0        0        0      367 2023-05-17 20:18:00.700973 phdi-1.0.4/phdi/fhir/tabulation/__init__.py
--rw-r--r--   0        0        0    27459 2023-05-17 20:18:00.700973 phdi-1.0.4/phdi/fhir/tabulation/tables.py
--rw-r--r--   0        0        0      397 2023-05-17 20:18:00.700973 phdi-1.0.4/phdi/fhir/transport/README.md
--rw-r--r--   0        0        0      327 2023-05-17 20:18:00.700973 phdi-1.0.4/phdi/fhir/transport/__init__.py
--rw-r--r--   0        0        0     7383 2023-05-17 20:18:00.700973 phdi-1.0.4/phdi/fhir/transport/export.py
--rw-r--r--   0        0        0     6822 2023-05-17 20:18:00.700973 phdi-1.0.4/phdi/fhir/transport/http.py
--rw-r--r--   0        0        0     7005 2023-05-17 20:18:00.700973 phdi-1.0.4/phdi/fhir/utils.py
--rw-r--r--   0        0        0      881 2023-05-17 20:18:00.700973 phdi-1.0.4/phdi/geospatial/README.md
--rw-r--r--   0        0        0      291 2023-05-17 20:18:00.700973 phdi-1.0.4/phdi/geospatial/__init__.py
--rw-r--r--   0        0        0     9294 2023-05-17 20:18:00.700973 phdi-1.0.4/phdi/geospatial/census.py
--rw-r--r--   0        0        0     2697 2023-05-17 20:18:00.700973 phdi-1.0.4/phdi/geospatial/core.py
--rw-r--r--   0        0        0     5911 2023-05-17 20:18:00.700973 phdi-1.0.4/phdi/geospatial/smarty.py
--rw-r--r--   0        0        0     1027 2023-05-17 20:18:00.700973 phdi-1.0.4/phdi/harmonization/README.md
--rw-r--r--   0        0        0      869 2023-05-17 20:18:00.700973 phdi-1.0.4/phdi/harmonization/__init__.py
--rw-r--r--   0        0        0    28162 2023-05-17 20:18:00.700973 phdi-1.0.4/phdi/harmonization/double_metaphone.py
--rw-r--r--   0        0        0    10909 2023-05-17 20:18:00.700973 phdi-1.0.4/phdi/harmonization/hl7.py
--rw-r--r--   0        0        0    36359 2023-05-17 20:18:00.700973 phdi-1.0.4/phdi/harmonization/phdi_nicknames.csv
--rw-r--r--   0        0        0    11999 2023-05-17 20:18:00.700973 phdi-1.0.4/phdi/harmonization/standardization.py
--rw-r--r--   0        0        0     1952 2023-05-17 20:18:00.700973 phdi-1.0.4/phdi/harmonization/utils.py
--rw-r--r--   0        0        0      255 2023-05-17 20:18:00.700973 phdi-1.0.4/phdi/linkage/README.md
--rw-r--r--   0        0        0     1869 2023-05-17 20:18:00.700973 phdi-1.0.4/phdi/linkage/__init__.py
--rw-r--r--   0        0        0     1948 2023-05-17 20:18:00.700973 phdi-1.0.4/phdi/linkage/algorithms.py
--rw-r--r--   0        0        0     2288 2023-05-17 20:18:00.700973 phdi-1.0.4/phdi/linkage/core.py
--rw-r--r--   0        0        0    57120 2023-05-17 20:18:00.700973 phdi-1.0.4/phdi/linkage/link.py
--rw-r--r--   0        0        0    11316 2023-05-17 20:18:00.700973 phdi-1.0.4/phdi/linkage/postgres.py
--rw-r--r--   0        0        0     2667 2023-05-17 20:18:00.700973 phdi-1.0.4/phdi/linkage/seed.py
--rw-r--r--   0        0        0      399 2023-05-17 20:18:00.700973 phdi-1.0.4/phdi/linkage/tables.ddl
--rw-r--r--   0        0        0      225 2023-05-17 20:18:00.700973 phdi-1.0.4/phdi/tabulation/README.md
--rw-r--r--   0        0        0      134 2023-05-17 20:18:00.700973 phdi-1.0.4/phdi/tabulation/__init__.py
--rw-r--r--   0        0        0    11839 2023-05-17 20:18:00.700973 phdi-1.0.4/phdi/tabulation/tables.py
--rw-r--r--   0        0        0     2046 2023-05-17 20:18:00.700973 phdi-1.0.4/phdi/tabulation/validation_schema.json
--rw-r--r--   0        0        0      225 2023-05-17 20:18:00.700973 phdi-1.0.4/phdi/transport/README.md
--rw-r--r--   0        0        0       81 2023-05-17 20:18:00.700973 phdi-1.0.4/phdi/transport/__init__.py
--rw-r--r--   0        0        0     2334 2023-05-17 20:18:00.700973 phdi-1.0.4/phdi/transport/http.py
--rw-r--r--   0        0        0     1244 2023-05-17 20:18:00.700973 phdi-1.0.4/phdi/validation/__init__.py
--rw-r--r--   0        0        0     6260 2023-05-17 20:18:00.700973 phdi-1.0.4/phdi/validation/validation.py
--rw-r--r--   0        0        0    17870 2023-05-17 20:18:00.700973 phdi-1.0.4/phdi/validation/xml_utils.py
--rw-r--r--   0        0        0     1820 2023-05-17 20:18:00.708974 phdi-1.0.4/pyproject.toml
--rw-r--r--   0        0        0    13589 1970-01-01 00:00:00.000000 phdi-1.0.4/PKG-INFO
+-rw-r--r--   0        0        0     7048 2023-05-17 21:57:42.655238 phdi-1.0.5/LICENSE.md
+-rw-r--r--   0        0        0    11787 2023-05-17 21:57:42.655238 phdi-1.0.5/README.md
+-rw-r--r--   0        0        0       27 2023-05-17 21:57:43.087275 phdi-1.0.5/phdi/__init__.py
+-rw-r--r--   0        0        0      223 2023-05-17 21:57:43.087275 phdi-1.0.5/phdi/cloud/README.md
+-rw-r--r--   0        0        0        0 2023-05-17 21:57:43.087275 phdi-1.0.5/phdi/cloud/__init__.py
+-rw-r--r--   0        0        0     9436 2023-05-17 21:57:43.087275 phdi-1.0.5/phdi/cloud/azure.py
+-rw-r--r--   0        0        0     2516 2023-05-17 21:57:43.087275 phdi-1.0.5/phdi/cloud/core.py
+-rw-r--r--   0        0        0     6055 2023-05-17 21:57:43.087275 phdi-1.0.5/phdi/cloud/gcp.py
+-rw-r--r--   0        0        0      163 2023-05-17 21:57:43.087275 phdi-1.0.5/phdi/containers/README.md
+-rw-r--r--   0        0        0        0 2023-05-17 21:57:43.087275 phdi-1.0.5/phdi/containers/__init__.py
+-rw-r--r--   0        0        0     2776 2023-05-17 21:57:43.087275 phdi-1.0.5/phdi/containers/base_service.py
+-rw-r--r--   0        0        0        0 2023-05-17 21:57:43.087275 phdi-1.0.5/phdi/fhir/__init__.py
+-rw-r--r--   0        0        0      292 2023-05-17 21:57:43.087275 phdi-1.0.5/phdi/fhir/cloud/README.md
+-rw-r--r--   0        0        0      119 2023-05-17 21:57:43.087275 phdi-1.0.5/phdi/fhir/cloud/__init__.py
+-rw-r--r--   0        0        0     2111 2023-05-17 21:57:43.087275 phdi-1.0.5/phdi/fhir/cloud/azure.py
+-rw-r--r--   0        0        0      311 2023-05-17 21:57:43.087275 phdi-1.0.5/phdi/fhir/conversion/README.md
+-rw-r--r--   0        0        0       89 2023-05-17 21:57:43.087275 phdi-1.0.5/phdi/fhir/conversion/__init__.py
+-rw-r--r--   0        0        0     8026 2023-05-17 21:57:43.087275 phdi-1.0.5/phdi/fhir/conversion/convert.py
+-rw-r--r--   0        0        0      808 2023-05-17 21:57:43.087275 phdi-1.0.5/phdi/fhir/geospatial/README.md
+-rw-r--r--   0        0        0      294 2023-05-17 21:57:43.087275 phdi-1.0.5/phdi/fhir/geospatial/__init__.py
+-rw-r--r--   0        0        0     3494 2023-05-17 21:57:43.087275 phdi-1.0.5/phdi/fhir/geospatial/census.py
+-rw-r--r--   0        0        0     4521 2023-05-17 21:57:43.087275 phdi-1.0.5/phdi/fhir/geospatial/core.py
+-rw-r--r--   0        0        0     3587 2023-05-17 21:57:43.087275 phdi-1.0.5/phdi/fhir/geospatial/smarty.py
+-rw-r--r--   0        0        0      890 2023-05-17 21:57:43.087275 phdi-1.0.5/phdi/fhir/harmonization/README.md
+-rw-r--r--   0        0        0      335 2023-05-17 21:57:43.087275 phdi-1.0.5/phdi/fhir/harmonization/__init__.py
+-rw-r--r--   0        0        0    11809 2023-05-17 21:57:43.087275 phdi-1.0.5/phdi/fhir/harmonization/standardization.py
+-rw-r--r--   0        0        0      179 2023-05-17 21:57:43.087275 phdi-1.0.5/phdi/fhir/linkage/__init__.py
+-rw-r--r--   0        0        0     3591 2023-05-17 21:57:43.087275 phdi-1.0.5/phdi/fhir/linkage/link.py
+-rw-r--r--   0        0        0      412 2023-05-17 21:57:43.087275 phdi-1.0.5/phdi/fhir/tabulation/README.md
+-rw-r--r--   0        0        0      367 2023-05-17 21:57:43.087275 phdi-1.0.5/phdi/fhir/tabulation/__init__.py
+-rw-r--r--   0        0        0    27459 2023-05-17 21:57:43.087275 phdi-1.0.5/phdi/fhir/tabulation/tables.py
+-rw-r--r--   0        0        0      397 2023-05-17 21:57:43.087275 phdi-1.0.5/phdi/fhir/transport/README.md
+-rw-r--r--   0        0        0      327 2023-05-17 21:57:43.087275 phdi-1.0.5/phdi/fhir/transport/__init__.py
+-rw-r--r--   0        0        0     7383 2023-05-17 21:57:43.087275 phdi-1.0.5/phdi/fhir/transport/export.py
+-rw-r--r--   0        0        0     6822 2023-05-17 21:57:43.087275 phdi-1.0.5/phdi/fhir/transport/http.py
+-rw-r--r--   0        0        0     7005 2023-05-17 21:57:43.087275 phdi-1.0.5/phdi/fhir/utils.py
+-rw-r--r--   0        0        0      881 2023-05-17 21:57:43.087275 phdi-1.0.5/phdi/geospatial/README.md
+-rw-r--r--   0        0        0      291 2023-05-17 21:57:43.087275 phdi-1.0.5/phdi/geospatial/__init__.py
+-rw-r--r--   0        0        0     9294 2023-05-17 21:57:43.087275 phdi-1.0.5/phdi/geospatial/census.py
+-rw-r--r--   0        0        0     2697 2023-05-17 21:57:43.087275 phdi-1.0.5/phdi/geospatial/core.py
+-rw-r--r--   0        0        0     5911 2023-05-17 21:57:43.087275 phdi-1.0.5/phdi/geospatial/smarty.py
+-rw-r--r--   0        0        0     1027 2023-05-17 21:57:43.087275 phdi-1.0.5/phdi/harmonization/README.md
+-rw-r--r--   0        0        0      869 2023-05-17 21:57:43.087275 phdi-1.0.5/phdi/harmonization/__init__.py
+-rw-r--r--   0        0        0    28162 2023-05-17 21:57:43.087275 phdi-1.0.5/phdi/harmonization/double_metaphone.py
+-rw-r--r--   0        0        0    10909 2023-05-17 21:57:43.087275 phdi-1.0.5/phdi/harmonization/hl7.py
+-rw-r--r--   0        0        0    36359 2023-05-17 21:57:43.087275 phdi-1.0.5/phdi/harmonization/phdi_nicknames.csv
+-rw-r--r--   0        0        0    11999 2023-05-17 21:57:43.087275 phdi-1.0.5/phdi/harmonization/standardization.py
+-rw-r--r--   0        0        0     1952 2023-05-17 21:57:43.087275 phdi-1.0.5/phdi/harmonization/utils.py
+-rw-r--r--   0        0        0      255 2023-05-17 21:57:43.087275 phdi-1.0.5/phdi/linkage/README.md
+-rw-r--r--   0        0        0     1869 2023-05-17 21:57:43.087275 phdi-1.0.5/phdi/linkage/__init__.py
+-rw-r--r--   0        0        0     1948 2023-05-17 21:57:43.087275 phdi-1.0.5/phdi/linkage/algorithms.py
+-rw-r--r--   0        0        0     2288 2023-05-17 21:57:43.087275 phdi-1.0.5/phdi/linkage/core.py
+-rw-r--r--   0        0        0    57120 2023-05-17 21:57:43.087275 phdi-1.0.5/phdi/linkage/link.py
+-rw-r--r--   0        0        0    11316 2023-05-17 21:57:43.091275 phdi-1.0.5/phdi/linkage/postgres.py
+-rw-r--r--   0        0        0     2667 2023-05-17 21:57:43.091275 phdi-1.0.5/phdi/linkage/seed.py
+-rw-r--r--   0        0        0      399 2023-05-17 21:57:43.091275 phdi-1.0.5/phdi/linkage/tables.ddl
+-rw-r--r--   0        0        0      225 2023-05-17 21:57:43.091275 phdi-1.0.5/phdi/tabulation/README.md
+-rw-r--r--   0        0        0      134 2023-05-17 21:57:43.091275 phdi-1.0.5/phdi/tabulation/__init__.py
+-rw-r--r--   0        0        0    11839 2023-05-17 21:57:43.091275 phdi-1.0.5/phdi/tabulation/tables.py
+-rw-r--r--   0        0        0     2046 2023-05-17 21:57:43.091275 phdi-1.0.5/phdi/tabulation/validation_schema.json
+-rw-r--r--   0        0        0      225 2023-05-17 21:57:43.091275 phdi-1.0.5/phdi/transport/README.md
+-rw-r--r--   0        0        0       81 2023-05-17 21:57:43.091275 phdi-1.0.5/phdi/transport/__init__.py
+-rw-r--r--   0        0        0     2334 2023-05-17 21:57:43.091275 phdi-1.0.5/phdi/transport/http.py
+-rw-r--r--   0        0        0     1244 2023-05-17 21:57:43.091275 phdi-1.0.5/phdi/validation/__init__.py
+-rw-r--r--   0        0        0     6260 2023-05-17 21:57:43.091275 phdi-1.0.5/phdi/validation/validation.py
+-rw-r--r--   0        0        0    17870 2023-05-17 21:57:43.091275 phdi-1.0.5/phdi/validation/xml_utils.py
+-rw-r--r--   0        0        0     1820 2023-05-17 21:57:43.095276 phdi-1.0.5/pyproject.toml
+-rw-r--r--   0        0        0    13589 1970-01-01 00:00:00.000000 phdi-1.0.5/PKG-INFO
```

### Comparing `phdi-1.0.4/LICENSE.md` & `phdi-1.0.5/LICENSE.md`

 * *Files identical despite different names*

### Comparing `phdi-1.0.4/README.md` & `phdi-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `phdi-1.0.4/phdi/cloud/azure.py` & `phdi-1.0.5/phdi/cloud/azure.py`

 * *Files identical despite different names*

### Comparing `phdi-1.0.4/phdi/cloud/core.py` & `phdi-1.0.5/phdi/cloud/core.py`

 * *Files identical despite different names*

### Comparing `phdi-1.0.4/phdi/cloud/gcp.py` & `phdi-1.0.5/phdi/cloud/gcp.py`

 * *Files identical despite different names*

### Comparing `phdi-1.0.4/phdi/containers/base_service.py` & `phdi-1.0.5/phdi/containers/base_service.py`

 * *Files identical despite different names*

### Comparing `phdi-1.0.4/phdi/fhir/cloud/azure.py` & `phdi-1.0.5/phdi/fhir/cloud/azure.py`

 * *Files identical despite different names*

### Comparing `phdi-1.0.4/phdi/fhir/conversion/convert.py` & `phdi-1.0.5/phdi/fhir/conversion/convert.py`

 * *Files identical despite different names*

### Comparing `phdi-1.0.4/phdi/fhir/geospatial/README.md` & `phdi-1.0.5/phdi/fhir/geospatial/README.md`

 * *Files identical despite different names*

### Comparing `phdi-1.0.4/phdi/fhir/geospatial/census.py` & `phdi-1.0.5/phdi/fhir/geospatial/census.py`

 * *Files identical despite different names*

### Comparing `phdi-1.0.4/phdi/fhir/geospatial/core.py` & `phdi-1.0.5/phdi/fhir/geospatial/core.py`

 * *Files identical despite different names*

### Comparing `phdi-1.0.4/phdi/fhir/geospatial/smarty.py` & `phdi-1.0.5/phdi/fhir/geospatial/smarty.py`

 * *Files identical despite different names*

### Comparing `phdi-1.0.4/phdi/fhir/harmonization/README.md` & `phdi-1.0.5/phdi/fhir/harmonization/README.md`

 * *Files identical despite different names*

### Comparing `phdi-1.0.4/phdi/fhir/harmonization/standardization.py` & `phdi-1.0.5/phdi/fhir/harmonization/standardization.py`

 * *Files identical despite different names*

### Comparing `phdi-1.0.4/phdi/fhir/linkage/link.py` & `phdi-1.0.5/phdi/fhir/linkage/link.py`

 * *Files identical despite different names*

### Comparing `phdi-1.0.4/phdi/fhir/tabulation/tables.py` & `phdi-1.0.5/phdi/fhir/tabulation/tables.py`

 * *Files identical despite different names*

### Comparing `phdi-1.0.4/phdi/fhir/transport/export.py` & `phdi-1.0.5/phdi/fhir/transport/export.py`

 * *Files identical despite different names*

### Comparing `phdi-1.0.4/phdi/fhir/transport/http.py` & `phdi-1.0.5/phdi/fhir/transport/http.py`

 * *Files identical despite different names*

### Comparing `phdi-1.0.4/phdi/fhir/utils.py` & `phdi-1.0.5/phdi/fhir/utils.py`

 * *Files identical despite different names*

### Comparing `phdi-1.0.4/phdi/geospatial/README.md` & `phdi-1.0.5/phdi/geospatial/README.md`

 * *Files identical despite different names*

### Comparing `phdi-1.0.4/phdi/geospatial/census.py` & `phdi-1.0.5/phdi/geospatial/census.py`

 * *Files identical despite different names*

### Comparing `phdi-1.0.4/phdi/geospatial/core.py` & `phdi-1.0.5/phdi/geospatial/core.py`

 * *Files identical despite different names*

### Comparing `phdi-1.0.4/phdi/geospatial/smarty.py` & `phdi-1.0.5/phdi/geospatial/smarty.py`

 * *Files identical despite different names*

### Comparing `phdi-1.0.4/phdi/harmonization/README.md` & `phdi-1.0.5/phdi/harmonization/README.md`

 * *Files identical despite different names*

### Comparing `phdi-1.0.4/phdi/harmonization/__init__.py` & `phdi-1.0.5/phdi/harmonization/__init__.py`

 * *Files identical despite different names*

### Comparing `phdi-1.0.4/phdi/harmonization/double_metaphone.py` & `phdi-1.0.5/phdi/harmonization/double_metaphone.py`

 * *Files identical despite different names*

### Comparing `phdi-1.0.4/phdi/harmonization/hl7.py` & `phdi-1.0.5/phdi/harmonization/hl7.py`

 * *Files identical despite different names*

### Comparing `phdi-1.0.4/phdi/harmonization/phdi_nicknames.csv` & `phdi-1.0.5/phdi/harmonization/phdi_nicknames.csv`

 * *Files identical despite different names*

### Comparing `phdi-1.0.4/phdi/harmonization/standardization.py` & `phdi-1.0.5/phdi/harmonization/standardization.py`

 * *Files identical despite different names*

### Comparing `phdi-1.0.4/phdi/harmonization/utils.py` & `phdi-1.0.5/phdi/harmonization/utils.py`

 * *Files identical despite different names*

### Comparing `phdi-1.0.4/phdi/linkage/__init__.py` & `phdi-1.0.5/phdi/linkage/__init__.py`

 * *Files identical despite different names*

### Comparing `phdi-1.0.4/phdi/linkage/algorithms.py` & `phdi-1.0.5/phdi/linkage/algorithms.py`

 * *Files identical despite different names*

### Comparing `phdi-1.0.4/phdi/linkage/core.py` & `phdi-1.0.5/phdi/linkage/core.py`

 * *Files identical despite different names*

### Comparing `phdi-1.0.4/phdi/linkage/link.py` & `phdi-1.0.5/phdi/linkage/link.py`

 * *Files identical despite different names*

### Comparing `phdi-1.0.4/phdi/linkage/postgres.py` & `phdi-1.0.5/phdi/linkage/postgres.py`

 * *Files identical despite different names*

### Comparing `phdi-1.0.4/phdi/linkage/seed.py` & `phdi-1.0.5/phdi/linkage/seed.py`

 * *Files identical despite different names*

### Comparing `phdi-1.0.4/phdi/tabulation/tables.py` & `phdi-1.0.5/phdi/tabulation/tables.py`

 * *Files identical despite different names*

### Comparing `phdi-1.0.4/phdi/tabulation/validation_schema.json` & `phdi-1.0.5/phdi/tabulation/validation_schema.json`

 * *Files identical despite different names*

### Comparing `phdi-1.0.4/phdi/transport/http.py` & `phdi-1.0.5/phdi/transport/http.py`

 * *Files identical despite different names*

### Comparing `phdi-1.0.4/phdi/validation/__init__.py` & `phdi-1.0.5/phdi/validation/__init__.py`

 * *Files identical despite different names*

### Comparing `phdi-1.0.4/phdi/validation/validation.py` & `phdi-1.0.5/phdi/validation/validation.py`

 * *Files identical despite different names*

### Comparing `phdi-1.0.4/phdi/validation/xml_utils.py` & `phdi-1.0.5/phdi/validation/xml_utils.py`

 * *Files identical despite different names*

### Comparing `phdi-1.0.4/pyproject.toml` & `phdi-1.0.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "phdi"
-version = "v1.0.4"
+version = "v1.0.5"
 description = "Public health data infrastructure Building Blocks is a library to help public health departments work with their data"
 authors = ["Kenneth Chow <kenneth@skylight.digital>", "Brandon Mader <brandon@skylight.digital>", "Spencer Kathol <spencer@skylight.digital>", "Nick Clyde <nclyde@skylight.digital", "Dan Paseltiner <dan@skylight.digital>", "Brady Fausett <brady@skylight.digital>", "Marcelle Goggins <marcelle@skylight.digital", "Nick Bristow <nick@skylight.digital>", "Bryan Britten <bryan@skylight.digital>", "Emma Stephenson <emma@skylight.digital>" , "Gordon Farrell <gordon@skylight.digital>", "Robert Mitchell <rmitchell@skylight.digital>"]
 homepage = "https://github.com/CDCgov/phdi"
 repository = "https://github.com/CDCgov/phdi"
 documentation = "https://cdcgov.github.io/phdi"
 readme = "README.md"
```

### Comparing `phdi-1.0.4/PKG-INFO` & `phdi-1.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: phdi
-Version: 1.0.4
+Version: 1.0.5
 Summary: Public health data infrastructure Building Blocks is a library to help public health departments work with their data
 Home-page: https://github.com/CDCgov/phdi
 Author: Kenneth Chow
 Author-email: kenneth@skylight.digital
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

