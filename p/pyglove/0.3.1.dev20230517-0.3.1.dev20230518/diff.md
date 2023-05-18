# Comparing `tmp/pyglove-0.3.1.dev20230517.tar.gz` & `tmp/pyglove-0.3.1.dev20230518.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyglove-0.3.1.dev20230517.tar", last modified: Wed May 17 08:06:29 2023, max compression
+gzip compressed data, was "pyglove-0.3.1.dev20230518.tar", last modified: Thu May 18 08:06:25 2023, max compression
```

## Comparing `pyglove-0.3.1.dev20230517.tar` & `pyglove-0.3.1.dev20230518.tar`

### file list

```diff
@@ -1,188 +1,188 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 08:06:29.212597 pyglove-0.3.1.dev20230517/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-17 08:06:11.000000 pyglove-0.3.1.dev20230517/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6624 2023-05-17 08:06:29.212597 pyglove-0.3.1.dev20230517/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5532 2023-05-17 08:06:26.000000 pyglove-0.3.1.dev20230517/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 08:06:29.196597 pyglove-0.3.1.dev20230517/pyglove/
--rw-r--r--   0 runner    (1001) docker     (123)     1352 2023-05-17 08:06:11.000000 pyglove-0.3.1.dev20230517/pyglove/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 08:06:29.196597 pyglove-0.3.1.dev20230517/pyglove/core/
--rw-r--r--   0 runner    (1001) docker     (123)     7917 2023-05-17 08:06:11.000000 pyglove-0.3.1.dev20230517/pyglove/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 08:06:29.196597 pyglove-0.3.1.dev20230517/pyglove/core/detouring/
--rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-05-17 08:06:11.000000 pyglove-0.3.1.dev20230517/pyglove/core/detouring/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13312 2023-05-17 08:06:11.000000 pyglove-0.3.1.dev20230517/pyglove/core/detouring/class_detour.py
--rw-r--r--   0 runner    (1001) docker     (123)     5507 2023-05-17 08:06:11.000000 pyglove-0.3.1.dev20230517/pyglove/core/detouring/class_detour_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 08:06:29.196597 pyglove-0.3.1.dev20230517/pyglove/core/geno/
--rw-r--r--   0 runner    (1001) docker     (123)     4767 2023-05-17 08:06:11.000000 pyglove-0.3.1.dev20230517/pyglove/core/geno/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    64370 2023-05-17 08:06:11.000000 pyglove-0.3.1.dev20230517/pyglove/core/geno/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    38561 2023-05-17 08:06:11.000000 pyglove-0.3.1.dev20230517/pyglove/core/geno/base_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    28154 2023-05-17 08:06:11.000000 pyglove-0.3.1.dev20230517/pyglove/core/geno/categorical.py
--rw-r--r--   0 runner    (1001) docker     (123)    18444 2023-05-17 08:06:11.000000 pyglove-0.3.1.dev20230517/pyglove/core/geno/categorical_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     7194 2023-05-17 08:06:11.000000 pyglove-0.3.1.dev20230517/pyglove/core/geno/custom.py
--rw-r--r--   0 runner    (1001) docker     (123)     5938 2023-05-17 08:06:11.000000 pyglove-0.3.1.dev20230517/pyglove/core/geno/custom_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5205 2023-05-17 08:06:11.000000 pyglove-0.3.1.dev20230517/pyglove/core/geno/deduping.py
--rw-r--r--   0 runner    (1001) docker     (123)     4583 2023-05-17 08:06:11.000000 pyglove-0.3.1.dev20230517/pyglove/core/geno/deduping_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     8959 2023-05-17 08:06:11.000000 pyglove-0.3.1.dev20230517/pyglove/core/geno/dna_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4731 2023-05-17 08:06:11.000000 pyglove-0.3.1.dev20230517/pyglove/core/geno/dna_generator_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     8330 2023-05-17 08:06:11.000000 pyglove-0.3.1.dev20230517/pyglove/core/geno/numerical.py
--rw-r--r--   0 runner    (1001) docker     (123)     5796 2023-05-17 08:06:11.000000 pyglove-0.3.1.dev20230517/pyglove/core/geno/numerical_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2619 2023-05-17 08:06:11.000000 pyglove-0.3.1.dev20230517/pyglove/core/geno/random.py
--rw-r--r--   0 runner    (1001) docker     (123)     4941 2023-05-17 08:06:11.000000 pyglove-0.3.1.dev20230517/pyglove/core/geno/random_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     9296 2023-05-17 08:06:11.000000 pyglove-0.3.1.dev20230517/pyglove/core/geno/space.py
--rw-r--r--   0 runner    (1001) docker     (123)    16554 2023-05-17 08:06:11.000000 pyglove-0.3.1.dev20230517/pyglove/core/geno/space_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-05-17 08:06:11.000000 pyglove-0.3.1.dev20230517/pyglove/core/geno/sweeping.py
--rw-r--r--   0 runner    (1001) docker     (123)     2709 2023-05-17 08:06:11.000000 pyglove-0.3.1.dev20230517/pyglove/core/geno/sweeping_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 08:06:29.200597 pyglove-0.3.1.dev20230517/pyglove/core/hyper/
--rw-r--r--   0 runner    (1001) docker     (123)     5020 2023-05-17 08:06:11.000000 pyglove-0.3.1.dev20230517/pyglove/core/hyper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7106 2023-05-17 08:06:11.000000 pyglove-0.3.1.dev20230517/pyglove/core/hyper/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    23216 2023-05-17 08:06:11.000000 pyglove-0.3.1.dev20230517/pyglove/core/hyper/categorical.py
--rw-r--r--   0 runner    (1001) docker     (123)    13533 2023-05-17 08:06:11.000000 pyglove-0.3.1.dev20230517/pyglove/core/hyper/categorical_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5750 2023-05-17 08:06:11.000000 pyglove-0.3.1.dev20230517/pyglove/core/hyper/custom.py
--rw-r--r--   0 runner    (1001) docker     (123)     3556 2023-05-17 08:06:11.000000 pyglove-0.3.1.dev20230517/pyglove/core/hyper/custom_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     6130 2023-05-17 08:06:11.000000 pyglove-0.3.1.dev20230517/pyglove/core/hyper/derived.py
--rw-r--r--   0 runner    (1001) docker     (123)     4283 2023-05-17 08:06:11.000000 pyglove-0.3.1.dev20230517/pyglove/core/hyper/derived_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    22812 2023-05-17 08:06:11.000000 pyglove-0.3.1.dev20230517/pyglove/core/hyper/dynamic_evaluation.py
--rw-r--r--   0 runner    (1001) docker     (123)    17149 2023-05-17 08:06:11.000000 pyglove-0.3.1.dev20230517/pyglove/core/hyper/dynamic_evaluation_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    10161 2023-05-17 08:06:11.000000 pyglove-0.3.1.dev20230517/pyglove/core/hyper/evolvable.py
--rw-r--r--   0 runner    (1001) docker     (123)     7505 2023-05-17 08:06:11.000000 pyglove-0.3.1.dev20230517/pyglove/core/hyper/evolvable_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     6921 2023-05-17 08:06:11.000000 pyglove-0.3.1.dev20230517/pyglove/core/hyper/iter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3906 2023-05-17 08:06:11.000000 pyglove-0.3.1.dev20230517/pyglove/core/hyper/iter_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     8206 2023-05-17 08:06:11.000000 pyglove-0.3.1.dev20230517/pyglove/core/hyper/numerical.py
--rw-r--r--   0 runner    (1001) docker     (123)     4259 2023-05-17 08:06:11.000000 pyglove-0.3.1.dev20230517/pyglove/core/hyper/numerical_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    22325 2023-05-17 08:06:11.000000 pyglove-0.3.1.dev20230517/pyglove/core/hyper/object_template.py
--rw-r--r--   0 runner    (1001) docker     (123)     9105 2023-05-17 08:06:11.000000 pyglove-0.3.1.dev20230517/pyglove/core/hyper/object_template_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2456 2023-05-17 08:06:11.000000 pyglove-0.3.1.dev20230517/pyglove/core/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     1956 2023-05-17 08:06:11.000000 pyglove-0.3.1.dev20230517/pyglove/core/logging_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 08:06:29.200597 pyglove-0.3.1.dev20230517/pyglove/core/object_utils/
--rw-r--r--   0 runner    (1001) docker     (123)     6821 2023-05-17 08:06:11.000000 pyglove-0.3.1.dev20230517/pyglove/core/object_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-05-17 08:06:11.000000 pyglove-0.3.1.dev20230517/pyglove/core/object_utils/codegen.py
--rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-05-17 08:06:11.000000 pyglove-0.3.1.dev20230517/pyglove/core/object_utils/codegen_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    14075 2023-05-17 08:06:11.000000 pyglove-0.3.1.dev20230517/pyglove/core/object_utils/common_traits.py
--rw-r--r--   0 runner    (1001) docker     (123)     3255 2023-05-17 08:06:11.000000 pyglove-0.3.1.dev20230517/pyglove/core/object_utils/common_traits_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4303 2023-05-17 08:06:11.000000 pyglove-0.3.1.dev20230517/pyglove/core/object_utils/docstr_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3165 2023-05-17 08:06:11.000000 pyglove-0.3.1.dev20230517/pyglove/core/object_utils/docstr_utils_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     6852 2023-05-17 08:06:11.000000 pyglove-0.3.1.dev20230517/pyglove/core/object_utils/formatting.py
--rw-r--r--   0 runner    (1001) docker     (123)     5901 2023-05-17 08:06:11.000000 pyglove-0.3.1.dev20230517/pyglove/core/object_utils/formatting_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    19754 2023-05-17 08:06:11.000000 pyglove-0.3.1.dev20230517/pyglove/core/object_utils/hierarchical.py
--rw-r--r--   0 runner    (1001) docker     (123)    21150 2023-05-17 08:06:11.000000 pyglove-0.3.1.dev20230517/pyglove/core/object_utils/hierarchical_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-05-17 08:06:11.000000 pyglove-0.3.1.dev20230517/pyglove/core/object_utils/missing.py
--rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-05-17 08:06:11.000000 pyglove-0.3.1.dev20230517/pyglove/core/object_utils/missing_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1614 2023-05-17 08:06:11.000000 pyglove-0.3.1.dev20230517/pyglove/core/object_utils/thread_local.py
--rw-r--r--   0 runner    (1001) docker     (123)     2531 2023-05-17 08:06:11.000000 pyglove-0.3.1.dev20230517/pyglove/core/object_utils/thread_local_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    18016 2023-05-17 08:06:11.000000 pyglove-0.3.1.dev20230517/pyglove/core/object_utils/value_location.py
--rw-r--r--   0 runner    (1001) docker     (123)    13083 2023-05-17 08:06:11.000000 pyglove-0.3.1.dev20230517/pyglove/core/object_utils/value_location_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 08:06:29.200597 pyglove-0.3.1.dev20230517/pyglove/core/patching/
--rw-r--r--   0 runner    (1001) docker     (123)     2059 2023-05-17 08:06:11.000000 pyglove-0.3.1.dev20230517/pyglove/core/patching/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3377 2023-05-17 08:06:11.000000 pyglove-0.3.1.dev20230517/pyglove/core/patching/object_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     3973 2023-05-17 08:06:11.000000 pyglove-0.3.1.dev20230517/pyglove/core/patching/object_factory_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     7872 2023-05-17 08:06:11.000000 pyglove-0.3.1.dev20230517/pyglove/core/patching/pattern_based.py
--rw-r--r--   0 runner    (1001) docker     (123)     2771 2023-05-17 08:06:11.000000 pyglove-0.3.1.dev20230517/pyglove/core/patching/pattern_based_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    16675 2023-05-17 08:06:11.000000 pyglove-0.3.1.dev20230517/pyglove/core/patching/rule_based.py
--rw-r--r--   0 runner    (1001) docker     (123)    17894 2023-05-17 08:06:11.000000 pyglove-0.3.1.dev20230517/pyglove/core/patching/rule_based_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 08:06:29.204597 pyglove-0.3.1.dev20230517/pyglove/core/symbolic/
--rw-r--r--   0 runner    (1001) docker     (123)     5396 2023-05-17 08:06:11.000000 pyglove-0.3.1.dev20230517/pyglove/core/symbolic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    69750 2023-05-17 08:06:11.000000 pyglove-0.3.1.dev20230517/pyglove/core/symbolic/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2776 2023-05-17 08:06:11.000000 pyglove-0.3.1.dev20230517/pyglove/core/symbolic/base_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     6234 2023-05-17 08:06:11.000000 pyglove-0.3.1.dev20230517/pyglove/core/symbolic/boilerplate.py
--rw-r--r--   0 runner    (1001) docker     (123)     4614 2023-05-17 08:06:11.000000 pyglove-0.3.1.dev20230517/pyglove/core/symbolic/boilerplate_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    22322 2023-05-17 08:06:11.000000 pyglove-0.3.1.dev20230517/pyglove/core/symbolic/class_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)    21508 2023-05-17 08:06:11.000000 pyglove-0.3.1.dev20230517/pyglove/core/symbolic/class_wrapper_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    32373 2023-05-17 08:06:11.000000 pyglove-0.3.1.dev20230517/pyglove/core/symbolic/dict.py
--rw-r--r--   0 runner    (1001) docker     (123)    57913 2023-05-17 08:06:11.000000 pyglove-0.3.1.dev20230517/pyglove/core/symbolic/dict_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    10690 2023-05-17 08:06:11.000000 pyglove-0.3.1.dev20230517/pyglove/core/symbolic/diff.py
--rw-r--r--   0 runner    (1001) docker     (123)     9762 2023-05-17 08:06:11.000000 pyglove-0.3.1.dev20230517/pyglove/core/symbolic/diff_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    11911 2023-05-17 08:06:11.000000 pyglove-0.3.1.dev20230517/pyglove/core/symbolic/flags.py
--rw-r--r--   0 runner    (1001) docker     (123)     5483 2023-05-17 08:06:11.000000 pyglove-0.3.1.dev20230517/pyglove/core/symbolic/flags_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    25881 2023-05-17 08:06:11.000000 pyglove-0.3.1.dev20230517/pyglove/core/symbolic/functor.py
--rw-r--r--   0 runner    (1001) docker     (123)    29009 2023-05-17 08:06:11.000000 pyglove-0.3.1.dev20230517/pyglove/core/symbolic/functor_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    27197 2023-05-17 08:06:11.000000 pyglove-0.3.1.dev20230517/pyglove/core/symbolic/list.py
--rw-r--r--   0 runner    (1001) docker     (123)    51901 2023-05-17 08:06:11.000000 pyglove-0.3.1.dev20230517/pyglove/core/symbolic/list_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    29637 2023-05-17 08:06:11.000000 pyglove-0.3.1.dev20230517/pyglove/core/symbolic/object.py
--rw-r--r--   0 runner    (1001) docker     (123)    74286 2023-05-17 08:06:11.000000 pyglove-0.3.1.dev20230517/pyglove/core/symbolic/object_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5139 2023-05-17 08:06:11.000000 pyglove-0.3.1.dev20230517/pyglove/core/symbolic/origin.py
--rw-r--r--   0 runner    (1001) docker     (123)     2393 2023-05-17 08:06:11.000000 pyglove-0.3.1.dev20230517/pyglove/core/symbolic/origin_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3244 2023-05-17 08:06:11.000000 pyglove-0.3.1.dev20230517/pyglove/core/symbolic/pure_symbolic.py
--rw-r--r--   0 runner    (1001) docker     (123)     9525 2023-05-17 08:06:11.000000 pyglove-0.3.1.dev20230517/pyglove/core/symbolic/schema_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1911 2023-05-17 08:06:11.000000 pyglove-0.3.1.dev20230517/pyglove/core/symbolic/schema_utils_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     6582 2023-05-17 08:06:11.000000 pyglove-0.3.1.dev20230517/pyglove/core/symbolic/symbolize.py
--rw-r--r--   0 runner    (1001) docker     (123)     6165 2023-05-17 08:06:11.000000 pyglove-0.3.1.dev20230517/pyglove/core/symbolic/symbolize_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 08:06:29.204597 pyglove-0.3.1.dev20230517/pyglove/core/tuning/
--rw-r--r--   0 runner    (1001) docker     (123)     2229 2023-05-17 08:06:11.000000 pyglove-0.3.1.dev20230517/pyglove/core/tuning/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5597 2023-05-17 08:06:11.000000 pyglove-0.3.1.dev20230517/pyglove/core/tuning/backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     1999 2023-05-17 08:06:11.000000 pyglove-0.3.1.dev20230517/pyglove/core/tuning/backend_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2102 2023-05-17 08:06:11.000000 pyglove-0.3.1.dev20230517/pyglove/core/tuning/early_stopping.py
--rw-r--r--   0 runner    (1001) docker     (123)    13832 2023-05-17 08:06:11.000000 pyglove-0.3.1.dev20230517/pyglove/core/tuning/local_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)    17756 2023-05-17 08:06:11.000000 pyglove-0.3.1.dev20230517/pyglove/core/tuning/protocols.py
--rw-r--r--   0 runner    (1001) docker     (123)     1883 2023-05-17 08:06:11.000000 pyglove-0.3.1.dev20230517/pyglove/core/tuning/protocols_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    12975 2023-05-17 08:06:11.000000 pyglove-0.3.1.dev20230517/pyglove/core/tuning/sample.py
--rw-r--r--   0 runner    (1001) docker     (123)    17552 2023-05-17 08:06:11.000000 pyglove-0.3.1.dev20230517/pyglove/core/tuning/sample_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 08:06:29.208597 pyglove-0.3.1.dev20230517/pyglove/core/typing/
--rw-r--r--   0 runner    (1001) docker     (123)    12960 2023-05-17 08:06:11.000000 pyglove-0.3.1.dev20230517/pyglove/core/typing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1626 2023-05-17 08:06:11.000000 pyglove-0.3.1.dev20230517/pyglove/core/typing/callable_ext.py
--rw-r--r--   0 runner    (1001) docker     (123)     2117 2023-05-17 08:06:11.000000 pyglove-0.3.1.dev20230517/pyglove/core/typing/callable_ext_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    10171 2023-05-17 08:06:11.000000 pyglove-0.3.1.dev20230517/pyglove/core/typing/callable_signature.py
--rw-r--r--   0 runner    (1001) docker     (123)     7844 2023-05-17 08:06:11.000000 pyglove-0.3.1.dev20230517/pyglove/core/typing/callable_signature_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    48578 2023-05-17 08:06:11.000000 pyglove-0.3.1.dev20230517/pyglove/core/typing/class_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)    25549 2023-05-17 08:06:11.000000 pyglove-0.3.1.dev20230517/pyglove/core/typing/class_schema_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    10139 2023-05-17 08:06:11.000000 pyglove-0.3.1.dev20230517/pyglove/core/typing/class_schema_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    10049 2023-05-17 08:06:11.000000 pyglove-0.3.1.dev20230517/pyglove/core/typing/class_schema_utils_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2218 2023-05-17 08:06:11.000000 pyglove-0.3.1.dev20230517/pyglove/core/typing/custom_typing.py
--rw-r--r--   0 runner    (1001) docker     (123)     8193 2023-05-17 08:06:11.000000 pyglove-0.3.1.dev20230517/pyglove/core/typing/key_specs.py
--rw-r--r--   0 runner    (1001) docker     (123)     5536 2023-05-17 08:06:11.000000 pyglove-0.3.1.dev20230517/pyglove/core/typing/key_specs_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2069 2023-05-17 08:06:11.000000 pyglove-0.3.1.dev20230517/pyglove/core/typing/pytype_support.py
--rw-r--r--   0 runner    (1001) docker     (123)     5104 2023-05-17 08:06:11.000000 pyglove-0.3.1.dev20230517/pyglove/core/typing/type_conversion.py
--rw-r--r--   0 runner    (1001) docker     (123)     4631 2023-05-17 08:06:11.000000 pyglove-0.3.1.dev20230517/pyglove/core/typing/type_conversion_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2784 2023-05-17 08:06:11.000000 pyglove-0.3.1.dev20230517/pyglove/core/typing/typed_missing.py
--rw-r--r--   0 runner    (1001) docker     (123)     2381 2023-05-17 08:06:11.000000 pyglove-0.3.1.dev20230517/pyglove/core/typing/typed_missing_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    82873 2023-05-17 08:06:11.000000 pyglove-0.3.1.dev20230517/pyglove/core/typing/value_specs.py
--rw-r--r--   0 runner    (1001) docker     (123)   110021 2023-05-17 08:06:11.000000 pyglove-0.3.1.dev20230517/pyglove/core/typing/value_specs_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 08:06:29.208597 pyglove-0.3.1.dev20230517/pyglove/ext/
--rw-r--r--   0 runner    (1001) docker     (123)      755 2023-05-17 08:06:11.000000 pyglove-0.3.1.dev20230517/pyglove/ext/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 08:06:29.208597 pyglove-0.3.1.dev20230517/pyglove/ext/early_stopping/
--rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-05-17 08:06:11.000000 pyglove-0.3.1.dev20230517/pyglove/ext/early_stopping/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2358 2023-05-17 08:06:11.000000 pyglove-0.3.1.dev20230517/pyglove/ext/early_stopping/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2796 2023-05-17 08:06:11.000000 pyglove-0.3.1.dev20230517/pyglove/ext/early_stopping/base_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    10117 2023-05-17 08:06:11.000000 pyglove-0.3.1.dev20230517/pyglove/ext/early_stopping/step_wise.py
--rw-r--r--   0 runner    (1001) docker     (123)     9032 2023-05-17 08:06:11.000000 pyglove-0.3.1.dev20230517/pyglove/ext/early_stopping/step_wise_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 08:06:29.208597 pyglove-0.3.1.dev20230517/pyglove/ext/evolution/
--rw-r--r--   0 runner    (1001) docker     (123)     3214 2023-05-17 08:06:11.000000 pyglove-0.3.1.dev20230517/pyglove/ext/evolution/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    50090 2023-05-17 08:06:11.000000 pyglove-0.3.1.dev20230517/pyglove/ext/evolution/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    29936 2023-05-17 08:06:11.000000 pyglove-0.3.1.dev20230517/pyglove/ext/evolution/base_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1688 2023-05-17 08:06:11.000000 pyglove-0.3.1.dev20230517/pyglove/ext/evolution/hill_climb.py
--rw-r--r--   0 runner    (1001) docker     (123)     3110 2023-05-17 08:06:11.000000 pyglove-0.3.1.dev20230517/pyglove/ext/evolution/hill_climb_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     9757 2023-05-17 08:06:11.000000 pyglove-0.3.1.dev20230517/pyglove/ext/evolution/mutators.py
--rw-r--r--   0 runner    (1001) docker     (123)    17424 2023-05-17 08:06:11.000000 pyglove-0.3.1.dev20230517/pyglove/ext/evolution/mutators_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     8162 2023-05-17 08:06:11.000000 pyglove-0.3.1.dev20230517/pyglove/ext/evolution/neat.py
--rw-r--r--   0 runner    (1001) docker     (123)     4474 2023-05-17 08:06:11.000000 pyglove-0.3.1.dev20230517/pyglove/ext/evolution/neat_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     6427 2023-05-17 08:06:11.000000 pyglove-0.3.1.dev20230517/pyglove/ext/evolution/nsga2.py
--rw-r--r--   0 runner    (1001) docker     (123)     8430 2023-05-17 08:06:11.000000 pyglove-0.3.1.dev20230517/pyglove/ext/evolution/nsga2_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    40354 2023-05-17 08:06:11.000000 pyglove-0.3.1.dev20230517/pyglove/ext/evolution/recombinators.py
--rw-r--r--   0 runner    (1001) docker     (123)    19290 2023-05-17 08:06:11.000000 pyglove-0.3.1.dev20230517/pyglove/ext/evolution/recombinators_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1954 2023-05-17 08:06:11.000000 pyglove-0.3.1.dev20230517/pyglove/ext/evolution/regularized_evolution.py
--rw-r--r--   0 runner    (1001) docker     (123)     3472 2023-05-17 08:06:11.000000 pyglove-0.3.1.dev20230517/pyglove/ext/evolution/regularized_evolution_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    12102 2023-05-17 08:06:11.000000 pyglove-0.3.1.dev20230517/pyglove/ext/evolution/selectors.py
--rw-r--r--   0 runner    (1001) docker     (123)     7714 2023-05-17 08:06:11.000000 pyglove-0.3.1.dev20230517/pyglove/ext/evolution/selectors_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4761 2023-05-17 08:06:11.000000 pyglove-0.3.1.dev20230517/pyglove/ext/evolution/where.py
--rw-r--r--   0 runner    (1001) docker     (123)     1931 2023-05-17 08:06:11.000000 pyglove-0.3.1.dev20230517/pyglove/ext/evolution/where_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 08:06:29.208597 pyglove-0.3.1.dev20230517/pyglove/ext/mutfun/
--rw-r--r--   0 runner    (1001) docker     (123)     4959 2023-05-17 08:06:11.000000 pyglove-0.3.1.dev20230517/pyglove/ext/mutfun/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16703 2023-05-17 08:06:11.000000 pyglove-0.3.1.dev20230517/pyglove/ext/mutfun/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    21312 2023-05-17 08:06:11.000000 pyglove-0.3.1.dev20230517/pyglove/ext/mutfun/base_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5667 2023-05-17 08:06:11.000000 pyglove-0.3.1.dev20230517/pyglove/ext/mutfun/basic_ops.py
--rw-r--r--   0 runner    (1001) docker     (123)    11244 2023-05-17 08:06:11.000000 pyglove-0.3.1.dev20230517/pyglove/ext/mutfun/basic_ops_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 08:06:29.212597 pyglove-0.3.1.dev20230517/pyglove/ext/scalars/
--rw-r--r--   0 runner    (1001) docker     (123)     2749 2023-05-17 08:06:11.000000 pyglove-0.3.1.dev20230517/pyglove/ext/scalars/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7102 2023-05-17 08:06:11.000000 pyglove-0.3.1.dev20230517/pyglove/ext/scalars/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3095 2023-05-17 08:06:11.000000 pyglove-0.3.1.dev20230517/pyglove/ext/scalars/base_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3188 2023-05-17 08:06:11.000000 pyglove-0.3.1.dev20230517/pyglove/ext/scalars/maths.py
--rw-r--r--   0 runner    (1001) docker     (123)     3923 2023-05-17 08:06:11.000000 pyglove-0.3.1.dev20230517/pyglove/ext/scalars/maths_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4198 2023-05-17 08:06:11.000000 pyglove-0.3.1.dev20230517/pyglove/ext/scalars/randoms.py
--rw-r--r--   0 runner    (1001) docker     (123)     2000 2023-05-17 08:06:11.000000 pyglove-0.3.1.dev20230517/pyglove/ext/scalars/randoms_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3789 2023-05-17 08:06:11.000000 pyglove-0.3.1.dev20230517/pyglove/ext/scalars/step_wise.py
--rw-r--r--   0 runner    (1001) docker     (123)     2540 2023-05-17 08:06:11.000000 pyglove-0.3.1.dev20230517/pyglove/ext/scalars/step_wise_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 08:06:29.196597 pyglove-0.3.1.dev20230517/pyglove.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6624 2023-05-17 08:06:29.000000 pyglove-0.3.1.dev20230517/pyglove.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6007 2023-05-17 08:06:29.000000 pyglove-0.3.1.dev20230517/pyglove.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 08:06:29.000000 pyglove-0.3.1.dev20230517/pyglove.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-17 08:06:29.000000 pyglove-0.3.1.dev20230517/pyglove.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-17 08:06:29.000000 pyglove-0.3.1.dev20230517/pyglove.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-17 08:06:29.212597 pyglove-0.3.1.dev20230517/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3574 2023-05-17 08:06:11.000000 pyglove-0.3.1.dev20230517/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 08:06:25.044342 pyglove-0.3.1.dev20230518/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-18 08:06:08.000000 pyglove-0.3.1.dev20230518/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6624 2023-05-18 08:06:25.044342 pyglove-0.3.1.dev20230518/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5532 2023-05-18 08:06:22.000000 pyglove-0.3.1.dev20230518/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 08:06:25.008340 pyglove-0.3.1.dev20230518/pyglove/
+-rw-r--r--   0 runner    (1001) docker     (123)     1352 2023-05-18 08:06:08.000000 pyglove-0.3.1.dev20230518/pyglove/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 08:06:25.012341 pyglove-0.3.1.dev20230518/pyglove/core/
+-rw-r--r--   0 runner    (1001) docker     (123)     7917 2023-05-18 08:06:08.000000 pyglove-0.3.1.dev20230518/pyglove/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 08:06:25.012341 pyglove-0.3.1.dev20230518/pyglove/core/detouring/
+-rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-05-18 08:06:08.000000 pyglove-0.3.1.dev20230518/pyglove/core/detouring/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13312 2023-05-18 08:06:08.000000 pyglove-0.3.1.dev20230518/pyglove/core/detouring/class_detour.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5507 2023-05-18 08:06:08.000000 pyglove-0.3.1.dev20230518/pyglove/core/detouring/class_detour_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 08:06:25.016341 pyglove-0.3.1.dev20230518/pyglove/core/geno/
+-rw-r--r--   0 runner    (1001) docker     (123)     4767 2023-05-18 08:06:08.000000 pyglove-0.3.1.dev20230518/pyglove/core/geno/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    64370 2023-05-18 08:06:08.000000 pyglove-0.3.1.dev20230518/pyglove/core/geno/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38561 2023-05-18 08:06:08.000000 pyglove-0.3.1.dev20230518/pyglove/core/geno/base_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28154 2023-05-18 08:06:08.000000 pyglove-0.3.1.dev20230518/pyglove/core/geno/categorical.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18444 2023-05-18 08:06:08.000000 pyglove-0.3.1.dev20230518/pyglove/core/geno/categorical_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7194 2023-05-18 08:06:08.000000 pyglove-0.3.1.dev20230518/pyglove/core/geno/custom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5938 2023-05-18 08:06:08.000000 pyglove-0.3.1.dev20230518/pyglove/core/geno/custom_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5205 2023-05-18 08:06:08.000000 pyglove-0.3.1.dev20230518/pyglove/core/geno/deduping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4583 2023-05-18 08:06:08.000000 pyglove-0.3.1.dev20230518/pyglove/core/geno/deduping_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8959 2023-05-18 08:06:08.000000 pyglove-0.3.1.dev20230518/pyglove/core/geno/dna_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4731 2023-05-18 08:06:08.000000 pyglove-0.3.1.dev20230518/pyglove/core/geno/dna_generator_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8330 2023-05-18 08:06:08.000000 pyglove-0.3.1.dev20230518/pyglove/core/geno/numerical.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5796 2023-05-18 08:06:08.000000 pyglove-0.3.1.dev20230518/pyglove/core/geno/numerical_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2619 2023-05-18 08:06:08.000000 pyglove-0.3.1.dev20230518/pyglove/core/geno/random.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4941 2023-05-18 08:06:08.000000 pyglove-0.3.1.dev20230518/pyglove/core/geno/random_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9296 2023-05-18 08:06:08.000000 pyglove-0.3.1.dev20230518/pyglove/core/geno/space.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16554 2023-05-18 08:06:08.000000 pyglove-0.3.1.dev20230518/pyglove/core/geno/space_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-05-18 08:06:08.000000 pyglove-0.3.1.dev20230518/pyglove/core/geno/sweeping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2709 2023-05-18 08:06:08.000000 pyglove-0.3.1.dev20230518/pyglove/core/geno/sweeping_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 08:06:25.020341 pyglove-0.3.1.dev20230518/pyglove/core/hyper/
+-rw-r--r--   0 runner    (1001) docker     (123)     5020 2023-05-18 08:06:08.000000 pyglove-0.3.1.dev20230518/pyglove/core/hyper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7106 2023-05-18 08:06:08.000000 pyglove-0.3.1.dev20230518/pyglove/core/hyper/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23216 2023-05-18 08:06:08.000000 pyglove-0.3.1.dev20230518/pyglove/core/hyper/categorical.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13533 2023-05-18 08:06:08.000000 pyglove-0.3.1.dev20230518/pyglove/core/hyper/categorical_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5750 2023-05-18 08:06:08.000000 pyglove-0.3.1.dev20230518/pyglove/core/hyper/custom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3556 2023-05-18 08:06:08.000000 pyglove-0.3.1.dev20230518/pyglove/core/hyper/custom_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6130 2023-05-18 08:06:08.000000 pyglove-0.3.1.dev20230518/pyglove/core/hyper/derived.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4283 2023-05-18 08:06:08.000000 pyglove-0.3.1.dev20230518/pyglove/core/hyper/derived_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22812 2023-05-18 08:06:08.000000 pyglove-0.3.1.dev20230518/pyglove/core/hyper/dynamic_evaluation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17149 2023-05-18 08:06:08.000000 pyglove-0.3.1.dev20230518/pyglove/core/hyper/dynamic_evaluation_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10161 2023-05-18 08:06:08.000000 pyglove-0.3.1.dev20230518/pyglove/core/hyper/evolvable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7505 2023-05-18 08:06:08.000000 pyglove-0.3.1.dev20230518/pyglove/core/hyper/evolvable_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6921 2023-05-18 08:06:08.000000 pyglove-0.3.1.dev20230518/pyglove/core/hyper/iter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3906 2023-05-18 08:06:08.000000 pyglove-0.3.1.dev20230518/pyglove/core/hyper/iter_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8206 2023-05-18 08:06:08.000000 pyglove-0.3.1.dev20230518/pyglove/core/hyper/numerical.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4259 2023-05-18 08:06:08.000000 pyglove-0.3.1.dev20230518/pyglove/core/hyper/numerical_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22325 2023-05-18 08:06:08.000000 pyglove-0.3.1.dev20230518/pyglove/core/hyper/object_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9105 2023-05-18 08:06:08.000000 pyglove-0.3.1.dev20230518/pyglove/core/hyper/object_template_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2456 2023-05-18 08:06:08.000000 pyglove-0.3.1.dev20230518/pyglove/core/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1956 2023-05-18 08:06:08.000000 pyglove-0.3.1.dev20230518/pyglove/core/logging_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 08:06:25.024341 pyglove-0.3.1.dev20230518/pyglove/core/object_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     6821 2023-05-18 08:06:08.000000 pyglove-0.3.1.dev20230518/pyglove/core/object_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-05-18 08:06:08.000000 pyglove-0.3.1.dev20230518/pyglove/core/object_utils/codegen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-05-18 08:06:08.000000 pyglove-0.3.1.dev20230518/pyglove/core/object_utils/codegen_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14075 2023-05-18 08:06:08.000000 pyglove-0.3.1.dev20230518/pyglove/core/object_utils/common_traits.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3255 2023-05-18 08:06:08.000000 pyglove-0.3.1.dev20230518/pyglove/core/object_utils/common_traits_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4303 2023-05-18 08:06:08.000000 pyglove-0.3.1.dev20230518/pyglove/core/object_utils/docstr_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3165 2023-05-18 08:06:08.000000 pyglove-0.3.1.dev20230518/pyglove/core/object_utils/docstr_utils_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6852 2023-05-18 08:06:08.000000 pyglove-0.3.1.dev20230518/pyglove/core/object_utils/formatting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5901 2023-05-18 08:06:08.000000 pyglove-0.3.1.dev20230518/pyglove/core/object_utils/formatting_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19754 2023-05-18 08:06:08.000000 pyglove-0.3.1.dev20230518/pyglove/core/object_utils/hierarchical.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21150 2023-05-18 08:06:08.000000 pyglove-0.3.1.dev20230518/pyglove/core/object_utils/hierarchical_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-05-18 08:06:08.000000 pyglove-0.3.1.dev20230518/pyglove/core/object_utils/missing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-05-18 08:06:08.000000 pyglove-0.3.1.dev20230518/pyglove/core/object_utils/missing_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1614 2023-05-18 08:06:08.000000 pyglove-0.3.1.dev20230518/pyglove/core/object_utils/thread_local.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2531 2023-05-18 08:06:08.000000 pyglove-0.3.1.dev20230518/pyglove/core/object_utils/thread_local_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18016 2023-05-18 08:06:08.000000 pyglove-0.3.1.dev20230518/pyglove/core/object_utils/value_location.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13083 2023-05-18 08:06:08.000000 pyglove-0.3.1.dev20230518/pyglove/core/object_utils/value_location_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 08:06:25.024341 pyglove-0.3.1.dev20230518/pyglove/core/patching/
+-rw-r--r--   0 runner    (1001) docker     (123)     2059 2023-05-18 08:06:08.000000 pyglove-0.3.1.dev20230518/pyglove/core/patching/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3377 2023-05-18 08:06:08.000000 pyglove-0.3.1.dev20230518/pyglove/core/patching/object_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3973 2023-05-18 08:06:08.000000 pyglove-0.3.1.dev20230518/pyglove/core/patching/object_factory_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7872 2023-05-18 08:06:08.000000 pyglove-0.3.1.dev20230518/pyglove/core/patching/pattern_based.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2771 2023-05-18 08:06:08.000000 pyglove-0.3.1.dev20230518/pyglove/core/patching/pattern_based_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16675 2023-05-18 08:06:08.000000 pyglove-0.3.1.dev20230518/pyglove/core/patching/rule_based.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17894 2023-05-18 08:06:08.000000 pyglove-0.3.1.dev20230518/pyglove/core/patching/rule_based_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 08:06:25.032342 pyglove-0.3.1.dev20230518/pyglove/core/symbolic/
+-rw-r--r--   0 runner    (1001) docker     (123)     5396 2023-05-18 08:06:08.000000 pyglove-0.3.1.dev20230518/pyglove/core/symbolic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    69750 2023-05-18 08:06:08.000000 pyglove-0.3.1.dev20230518/pyglove/core/symbolic/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2776 2023-05-18 08:06:08.000000 pyglove-0.3.1.dev20230518/pyglove/core/symbolic/base_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6234 2023-05-18 08:06:08.000000 pyglove-0.3.1.dev20230518/pyglove/core/symbolic/boilerplate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4614 2023-05-18 08:06:08.000000 pyglove-0.3.1.dev20230518/pyglove/core/symbolic/boilerplate_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22322 2023-05-18 08:06:08.000000 pyglove-0.3.1.dev20230518/pyglove/core/symbolic/class_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21508 2023-05-18 08:06:08.000000 pyglove-0.3.1.dev20230518/pyglove/core/symbolic/class_wrapper_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32373 2023-05-18 08:06:08.000000 pyglove-0.3.1.dev20230518/pyglove/core/symbolic/dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57913 2023-05-18 08:06:08.000000 pyglove-0.3.1.dev20230518/pyglove/core/symbolic/dict_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10690 2023-05-18 08:06:08.000000 pyglove-0.3.1.dev20230518/pyglove/core/symbolic/diff.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9762 2023-05-18 08:06:08.000000 pyglove-0.3.1.dev20230518/pyglove/core/symbolic/diff_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11911 2023-05-18 08:06:08.000000 pyglove-0.3.1.dev20230518/pyglove/core/symbolic/flags.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5483 2023-05-18 08:06:08.000000 pyglove-0.3.1.dev20230518/pyglove/core/symbolic/flags_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25881 2023-05-18 08:06:08.000000 pyglove-0.3.1.dev20230518/pyglove/core/symbolic/functor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29009 2023-05-18 08:06:08.000000 pyglove-0.3.1.dev20230518/pyglove/core/symbolic/functor_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27197 2023-05-18 08:06:08.000000 pyglove-0.3.1.dev20230518/pyglove/core/symbolic/list.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51901 2023-05-18 08:06:08.000000 pyglove-0.3.1.dev20230518/pyglove/core/symbolic/list_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30587 2023-05-18 08:06:08.000000 pyglove-0.3.1.dev20230518/pyglove/core/symbolic/object.py
+-rw-r--r--   0 runner    (1001) docker     (123)    74703 2023-05-18 08:06:08.000000 pyglove-0.3.1.dev20230518/pyglove/core/symbolic/object_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5139 2023-05-18 08:06:08.000000 pyglove-0.3.1.dev20230518/pyglove/core/symbolic/origin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2393 2023-05-18 08:06:08.000000 pyglove-0.3.1.dev20230518/pyglove/core/symbolic/origin_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3244 2023-05-18 08:06:08.000000 pyglove-0.3.1.dev20230518/pyglove/core/symbolic/pure_symbolic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9424 2023-05-18 08:06:08.000000 pyglove-0.3.1.dev20230518/pyglove/core/symbolic/schema_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1911 2023-05-18 08:06:08.000000 pyglove-0.3.1.dev20230518/pyglove/core/symbolic/schema_utils_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6582 2023-05-18 08:06:08.000000 pyglove-0.3.1.dev20230518/pyglove/core/symbolic/symbolize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6165 2023-05-18 08:06:08.000000 pyglove-0.3.1.dev20230518/pyglove/core/symbolic/symbolize_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 08:06:25.032342 pyglove-0.3.1.dev20230518/pyglove/core/tuning/
+-rw-r--r--   0 runner    (1001) docker     (123)     2229 2023-05-18 08:06:08.000000 pyglove-0.3.1.dev20230518/pyglove/core/tuning/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5597 2023-05-18 08:06:08.000000 pyglove-0.3.1.dev20230518/pyglove/core/tuning/backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1999 2023-05-18 08:06:08.000000 pyglove-0.3.1.dev20230518/pyglove/core/tuning/backend_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2102 2023-05-18 08:06:08.000000 pyglove-0.3.1.dev20230518/pyglove/core/tuning/early_stopping.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13832 2023-05-18 08:06:08.000000 pyglove-0.3.1.dev20230518/pyglove/core/tuning/local_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17756 2023-05-18 08:06:08.000000 pyglove-0.3.1.dev20230518/pyglove/core/tuning/protocols.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1883 2023-05-18 08:06:08.000000 pyglove-0.3.1.dev20230518/pyglove/core/tuning/protocols_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12975 2023-05-18 08:06:08.000000 pyglove-0.3.1.dev20230518/pyglove/core/tuning/sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17552 2023-05-18 08:06:08.000000 pyglove-0.3.1.dev20230518/pyglove/core/tuning/sample_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 08:06:25.036342 pyglove-0.3.1.dev20230518/pyglove/core/typing/
+-rw-r--r--   0 runner    (1001) docker     (123)    12960 2023-05-18 08:06:08.000000 pyglove-0.3.1.dev20230518/pyglove/core/typing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1626 2023-05-18 08:06:08.000000 pyglove-0.3.1.dev20230518/pyglove/core/typing/callable_ext.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2117 2023-05-18 08:06:08.000000 pyglove-0.3.1.dev20230518/pyglove/core/typing/callable_ext_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10171 2023-05-18 08:06:08.000000 pyglove-0.3.1.dev20230518/pyglove/core/typing/callable_signature.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7844 2023-05-18 08:06:08.000000 pyglove-0.3.1.dev20230518/pyglove/core/typing/callable_signature_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48578 2023-05-18 08:06:08.000000 pyglove-0.3.1.dev20230518/pyglove/core/typing/class_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25549 2023-05-18 08:06:08.000000 pyglove-0.3.1.dev20230518/pyglove/core/typing/class_schema_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10139 2023-05-18 08:06:08.000000 pyglove-0.3.1.dev20230518/pyglove/core/typing/class_schema_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10049 2023-05-18 08:06:08.000000 pyglove-0.3.1.dev20230518/pyglove/core/typing/class_schema_utils_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2218 2023-05-18 08:06:08.000000 pyglove-0.3.1.dev20230518/pyglove/core/typing/custom_typing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8193 2023-05-18 08:06:08.000000 pyglove-0.3.1.dev20230518/pyglove/core/typing/key_specs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5536 2023-05-18 08:06:08.000000 pyglove-0.3.1.dev20230518/pyglove/core/typing/key_specs_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2069 2023-05-18 08:06:08.000000 pyglove-0.3.1.dev20230518/pyglove/core/typing/pytype_support.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5104 2023-05-18 08:06:08.000000 pyglove-0.3.1.dev20230518/pyglove/core/typing/type_conversion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4631 2023-05-18 08:06:08.000000 pyglove-0.3.1.dev20230518/pyglove/core/typing/type_conversion_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2784 2023-05-18 08:06:08.000000 pyglove-0.3.1.dev20230518/pyglove/core/typing/typed_missing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2381 2023-05-18 08:06:08.000000 pyglove-0.3.1.dev20230518/pyglove/core/typing/typed_missing_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    82873 2023-05-18 08:06:08.000000 pyglove-0.3.1.dev20230518/pyglove/core/typing/value_specs.py
+-rw-r--r--   0 runner    (1001) docker     (123)   110021 2023-05-18 08:06:08.000000 pyglove-0.3.1.dev20230518/pyglove/core/typing/value_specs_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 08:06:25.036342 pyglove-0.3.1.dev20230518/pyglove/ext/
+-rw-r--r--   0 runner    (1001) docker     (123)      755 2023-05-18 08:06:08.000000 pyglove-0.3.1.dev20230518/pyglove/ext/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 08:06:25.036342 pyglove-0.3.1.dev20230518/pyglove/ext/early_stopping/
+-rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-05-18 08:06:08.000000 pyglove-0.3.1.dev20230518/pyglove/ext/early_stopping/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2358 2023-05-18 08:06:08.000000 pyglove-0.3.1.dev20230518/pyglove/ext/early_stopping/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2796 2023-05-18 08:06:08.000000 pyglove-0.3.1.dev20230518/pyglove/ext/early_stopping/base_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10117 2023-05-18 08:06:08.000000 pyglove-0.3.1.dev20230518/pyglove/ext/early_stopping/step_wise.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9032 2023-05-18 08:06:08.000000 pyglove-0.3.1.dev20230518/pyglove/ext/early_stopping/step_wise_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 08:06:25.044342 pyglove-0.3.1.dev20230518/pyglove/ext/evolution/
+-rw-r--r--   0 runner    (1001) docker     (123)     3214 2023-05-18 08:06:08.000000 pyglove-0.3.1.dev20230518/pyglove/ext/evolution/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50090 2023-05-18 08:06:08.000000 pyglove-0.3.1.dev20230518/pyglove/ext/evolution/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29936 2023-05-18 08:06:08.000000 pyglove-0.3.1.dev20230518/pyglove/ext/evolution/base_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1688 2023-05-18 08:06:08.000000 pyglove-0.3.1.dev20230518/pyglove/ext/evolution/hill_climb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3110 2023-05-18 08:06:08.000000 pyglove-0.3.1.dev20230518/pyglove/ext/evolution/hill_climb_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9757 2023-05-18 08:06:08.000000 pyglove-0.3.1.dev20230518/pyglove/ext/evolution/mutators.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17424 2023-05-18 08:06:08.000000 pyglove-0.3.1.dev20230518/pyglove/ext/evolution/mutators_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8162 2023-05-18 08:06:08.000000 pyglove-0.3.1.dev20230518/pyglove/ext/evolution/neat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4474 2023-05-18 08:06:08.000000 pyglove-0.3.1.dev20230518/pyglove/ext/evolution/neat_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6427 2023-05-18 08:06:08.000000 pyglove-0.3.1.dev20230518/pyglove/ext/evolution/nsga2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8430 2023-05-18 08:06:08.000000 pyglove-0.3.1.dev20230518/pyglove/ext/evolution/nsga2_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40354 2023-05-18 08:06:08.000000 pyglove-0.3.1.dev20230518/pyglove/ext/evolution/recombinators.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19290 2023-05-18 08:06:08.000000 pyglove-0.3.1.dev20230518/pyglove/ext/evolution/recombinators_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1954 2023-05-18 08:06:08.000000 pyglove-0.3.1.dev20230518/pyglove/ext/evolution/regularized_evolution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3472 2023-05-18 08:06:08.000000 pyglove-0.3.1.dev20230518/pyglove/ext/evolution/regularized_evolution_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12102 2023-05-18 08:06:08.000000 pyglove-0.3.1.dev20230518/pyglove/ext/evolution/selectors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7714 2023-05-18 08:06:08.000000 pyglove-0.3.1.dev20230518/pyglove/ext/evolution/selectors_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4761 2023-05-18 08:06:08.000000 pyglove-0.3.1.dev20230518/pyglove/ext/evolution/where.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1931 2023-05-18 08:06:08.000000 pyglove-0.3.1.dev20230518/pyglove/ext/evolution/where_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 08:06:25.044342 pyglove-0.3.1.dev20230518/pyglove/ext/mutfun/
+-rw-r--r--   0 runner    (1001) docker     (123)     4959 2023-05-18 08:06:08.000000 pyglove-0.3.1.dev20230518/pyglove/ext/mutfun/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16703 2023-05-18 08:06:08.000000 pyglove-0.3.1.dev20230518/pyglove/ext/mutfun/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21312 2023-05-18 08:06:08.000000 pyglove-0.3.1.dev20230518/pyglove/ext/mutfun/base_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5667 2023-05-18 08:06:08.000000 pyglove-0.3.1.dev20230518/pyglove/ext/mutfun/basic_ops.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11244 2023-05-18 08:06:08.000000 pyglove-0.3.1.dev20230518/pyglove/ext/mutfun/basic_ops_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 08:06:25.044342 pyglove-0.3.1.dev20230518/pyglove/ext/scalars/
+-rw-r--r--   0 runner    (1001) docker     (123)     2749 2023-05-18 08:06:08.000000 pyglove-0.3.1.dev20230518/pyglove/ext/scalars/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7102 2023-05-18 08:06:08.000000 pyglove-0.3.1.dev20230518/pyglove/ext/scalars/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3095 2023-05-18 08:06:08.000000 pyglove-0.3.1.dev20230518/pyglove/ext/scalars/base_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3188 2023-05-18 08:06:08.000000 pyglove-0.3.1.dev20230518/pyglove/ext/scalars/maths.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3923 2023-05-18 08:06:08.000000 pyglove-0.3.1.dev20230518/pyglove/ext/scalars/maths_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4198 2023-05-18 08:06:08.000000 pyglove-0.3.1.dev20230518/pyglove/ext/scalars/randoms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2000 2023-05-18 08:06:08.000000 pyglove-0.3.1.dev20230518/pyglove/ext/scalars/randoms_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3789 2023-05-18 08:06:08.000000 pyglove-0.3.1.dev20230518/pyglove/ext/scalars/step_wise.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2540 2023-05-18 08:06:08.000000 pyglove-0.3.1.dev20230518/pyglove/ext/scalars/step_wise_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 08:06:25.012341 pyglove-0.3.1.dev20230518/pyglove.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6624 2023-05-18 08:06:24.000000 pyglove-0.3.1.dev20230518/pyglove.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6007 2023-05-18 08:06:24.000000 pyglove-0.3.1.dev20230518/pyglove.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 08:06:24.000000 pyglove-0.3.1.dev20230518/pyglove.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-18 08:06:24.000000 pyglove-0.3.1.dev20230518/pyglove.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-18 08:06:24.000000 pyglove-0.3.1.dev20230518/pyglove.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-18 08:06:25.044342 pyglove-0.3.1.dev20230518/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3574 2023-05-18 08:06:08.000000 pyglove-0.3.1.dev20230518/setup.py
```

### Comparing `pyglove-0.3.1.dev20230517/LICENSE` & `pyglove-0.3.1.dev20230518/LICENSE`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230517/PKG-INFO` & `pyglove-0.3.1.dev20230518/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyglove
-Version: 0.3.1.dev20230517
+Version: 0.3.1.dev20230518
 Summary: PyGlove: A library for manipulating Python objects.
 Home-page: https://github.com/google/pyglove
 Author: PyGlove Authors
 Author-email: pyglove-authors@google.com
 License: Apache License 2.0
 Keywords: ai machine learning automl mutable symbolic framework meta-programming
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `pyglove-0.3.1.dev20230517/README.md` & `pyglove-0.3.1.dev20230518/README.md`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230517/pyglove/__init__.py` & `pyglove-0.3.1.dev20230518/pyglove/__init__.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230517/pyglove/core/__init__.py` & `pyglove-0.3.1.dev20230518/pyglove/core/__init__.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230517/pyglove/core/detouring/__init__.py` & `pyglove-0.3.1.dev20230518/pyglove/core/detouring/__init__.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230517/pyglove/core/detouring/class_detour.py` & `pyglove-0.3.1.dev20230518/pyglove/core/detouring/class_detour.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230517/pyglove/core/detouring/class_detour_test.py` & `pyglove-0.3.1.dev20230518/pyglove/core/detouring/class_detour_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230517/pyglove/core/geno/__init__.py` & `pyglove-0.3.1.dev20230518/pyglove/core/geno/__init__.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230517/pyglove/core/geno/base.py` & `pyglove-0.3.1.dev20230518/pyglove/core/geno/base.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230517/pyglove/core/geno/base_test.py` & `pyglove-0.3.1.dev20230518/pyglove/core/geno/base_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230517/pyglove/core/geno/categorical.py` & `pyglove-0.3.1.dev20230518/pyglove/core/geno/categorical.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230517/pyglove/core/geno/categorical_test.py` & `pyglove-0.3.1.dev20230518/pyglove/core/geno/categorical_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230517/pyglove/core/geno/custom.py` & `pyglove-0.3.1.dev20230518/pyglove/core/geno/custom.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230517/pyglove/core/geno/custom_test.py` & `pyglove-0.3.1.dev20230518/pyglove/core/geno/custom_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230517/pyglove/core/geno/deduping.py` & `pyglove-0.3.1.dev20230518/pyglove/core/geno/deduping.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230517/pyglove/core/geno/deduping_test.py` & `pyglove-0.3.1.dev20230518/pyglove/core/geno/deduping_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230517/pyglove/core/geno/dna_generator.py` & `pyglove-0.3.1.dev20230518/pyglove/core/geno/dna_generator.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230517/pyglove/core/geno/dna_generator_test.py` & `pyglove-0.3.1.dev20230518/pyglove/core/geno/dna_generator_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230517/pyglove/core/geno/numerical.py` & `pyglove-0.3.1.dev20230518/pyglove/core/geno/numerical.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230517/pyglove/core/geno/numerical_test.py` & `pyglove-0.3.1.dev20230518/pyglove/core/geno/numerical_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230517/pyglove/core/geno/random.py` & `pyglove-0.3.1.dev20230518/pyglove/core/geno/random.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230517/pyglove/core/geno/random_test.py` & `pyglove-0.3.1.dev20230518/pyglove/core/geno/random_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230517/pyglove/core/geno/space.py` & `pyglove-0.3.1.dev20230518/pyglove/core/geno/space.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230517/pyglove/core/geno/space_test.py` & `pyglove-0.3.1.dev20230518/pyglove/core/geno/space_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230517/pyglove/core/geno/sweeping.py` & `pyglove-0.3.1.dev20230518/pyglove/core/geno/sweeping.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230517/pyglove/core/geno/sweeping_test.py` & `pyglove-0.3.1.dev20230518/pyglove/core/geno/sweeping_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230517/pyglove/core/hyper/__init__.py` & `pyglove-0.3.1.dev20230518/pyglove/core/hyper/__init__.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230517/pyglove/core/hyper/base.py` & `pyglove-0.3.1.dev20230518/pyglove/core/hyper/base.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230517/pyglove/core/hyper/categorical.py` & `pyglove-0.3.1.dev20230518/pyglove/core/hyper/categorical.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230517/pyglove/core/hyper/categorical_test.py` & `pyglove-0.3.1.dev20230518/pyglove/core/hyper/categorical_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230517/pyglove/core/hyper/custom.py` & `pyglove-0.3.1.dev20230518/pyglove/core/hyper/custom.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230517/pyglove/core/hyper/custom_test.py` & `pyglove-0.3.1.dev20230518/pyglove/core/hyper/custom_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230517/pyglove/core/hyper/derived.py` & `pyglove-0.3.1.dev20230518/pyglove/core/hyper/derived.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230517/pyglove/core/hyper/derived_test.py` & `pyglove-0.3.1.dev20230518/pyglove/core/hyper/derived_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230517/pyglove/core/hyper/dynamic_evaluation.py` & `pyglove-0.3.1.dev20230518/pyglove/core/hyper/dynamic_evaluation.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230517/pyglove/core/hyper/dynamic_evaluation_test.py` & `pyglove-0.3.1.dev20230518/pyglove/core/hyper/dynamic_evaluation_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230517/pyglove/core/hyper/evolvable.py` & `pyglove-0.3.1.dev20230518/pyglove/core/hyper/evolvable.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230517/pyglove/core/hyper/evolvable_test.py` & `pyglove-0.3.1.dev20230518/pyglove/core/hyper/evolvable_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230517/pyglove/core/hyper/iter.py` & `pyglove-0.3.1.dev20230518/pyglove/core/hyper/iter.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230517/pyglove/core/hyper/iter_test.py` & `pyglove-0.3.1.dev20230518/pyglove/core/hyper/iter_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230517/pyglove/core/hyper/numerical.py` & `pyglove-0.3.1.dev20230518/pyglove/core/hyper/numerical.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230517/pyglove/core/hyper/numerical_test.py` & `pyglove-0.3.1.dev20230518/pyglove/core/hyper/numerical_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230517/pyglove/core/hyper/object_template.py` & `pyglove-0.3.1.dev20230518/pyglove/core/hyper/object_template.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230517/pyglove/core/hyper/object_template_test.py` & `pyglove-0.3.1.dev20230518/pyglove/core/hyper/object_template_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230517/pyglove/core/logging.py` & `pyglove-0.3.1.dev20230518/pyglove/core/logging.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230517/pyglove/core/logging_test.py` & `pyglove-0.3.1.dev20230518/pyglove/core/logging_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230517/pyglove/core/object_utils/__init__.py` & `pyglove-0.3.1.dev20230518/pyglove/core/object_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230517/pyglove/core/object_utils/codegen.py` & `pyglove-0.3.1.dev20230518/pyglove/core/object_utils/codegen.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230517/pyglove/core/object_utils/codegen_test.py` & `pyglove-0.3.1.dev20230518/pyglove/core/object_utils/codegen_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230517/pyglove/core/object_utils/common_traits.py` & `pyglove-0.3.1.dev20230518/pyglove/core/object_utils/common_traits.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230517/pyglove/core/object_utils/common_traits_test.py` & `pyglove-0.3.1.dev20230518/pyglove/core/object_utils/common_traits_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230517/pyglove/core/object_utils/docstr_utils.py` & `pyglove-0.3.1.dev20230518/pyglove/core/object_utils/docstr_utils.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230517/pyglove/core/object_utils/docstr_utils_test.py` & `pyglove-0.3.1.dev20230518/pyglove/core/object_utils/docstr_utils_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230517/pyglove/core/object_utils/formatting.py` & `pyglove-0.3.1.dev20230518/pyglove/core/object_utils/formatting.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230517/pyglove/core/object_utils/formatting_test.py` & `pyglove-0.3.1.dev20230518/pyglove/core/object_utils/formatting_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230517/pyglove/core/object_utils/hierarchical.py` & `pyglove-0.3.1.dev20230518/pyglove/core/object_utils/hierarchical.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230517/pyglove/core/object_utils/hierarchical_test.py` & `pyglove-0.3.1.dev20230518/pyglove/core/object_utils/hierarchical_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230517/pyglove/core/object_utils/missing.py` & `pyglove-0.3.1.dev20230518/pyglove/core/object_utils/missing.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230517/pyglove/core/object_utils/missing_test.py` & `pyglove-0.3.1.dev20230518/pyglove/core/object_utils/missing_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230517/pyglove/core/object_utils/thread_local.py` & `pyglove-0.3.1.dev20230518/pyglove/core/object_utils/thread_local.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230517/pyglove/core/object_utils/thread_local_test.py` & `pyglove-0.3.1.dev20230518/pyglove/core/object_utils/thread_local_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230517/pyglove/core/object_utils/value_location.py` & `pyglove-0.3.1.dev20230518/pyglove/core/object_utils/value_location.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230517/pyglove/core/object_utils/value_location_test.py` & `pyglove-0.3.1.dev20230518/pyglove/core/object_utils/value_location_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230517/pyglove/core/patching/__init__.py` & `pyglove-0.3.1.dev20230518/pyglove/core/patching/__init__.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230517/pyglove/core/patching/object_factory.py` & `pyglove-0.3.1.dev20230518/pyglove/core/patching/object_factory.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230517/pyglove/core/patching/object_factory_test.py` & `pyglove-0.3.1.dev20230518/pyglove/core/patching/object_factory_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230517/pyglove/core/patching/pattern_based.py` & `pyglove-0.3.1.dev20230518/pyglove/core/patching/pattern_based.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230517/pyglove/core/patching/pattern_based_test.py` & `pyglove-0.3.1.dev20230518/pyglove/core/patching/pattern_based_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230517/pyglove/core/patching/rule_based.py` & `pyglove-0.3.1.dev20230518/pyglove/core/patching/rule_based.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230517/pyglove/core/patching/rule_based_test.py` & `pyglove-0.3.1.dev20230518/pyglove/core/patching/rule_based_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230517/pyglove/core/symbolic/__init__.py` & `pyglove-0.3.1.dev20230518/pyglove/core/symbolic/__init__.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230517/pyglove/core/symbolic/base.py` & `pyglove-0.3.1.dev20230518/pyglove/core/symbolic/base.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230517/pyglove/core/symbolic/base_test.py` & `pyglove-0.3.1.dev20230518/pyglove/core/symbolic/base_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230517/pyglove/core/symbolic/boilerplate.py` & `pyglove-0.3.1.dev20230518/pyglove/core/symbolic/boilerplate.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230517/pyglove/core/symbolic/boilerplate_test.py` & `pyglove-0.3.1.dev20230518/pyglove/core/symbolic/boilerplate_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230517/pyglove/core/symbolic/class_wrapper.py` & `pyglove-0.3.1.dev20230518/pyglove/core/symbolic/class_wrapper.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230517/pyglove/core/symbolic/class_wrapper_test.py` & `pyglove-0.3.1.dev20230518/pyglove/core/symbolic/class_wrapper_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230517/pyglove/core/symbolic/dict.py` & `pyglove-0.3.1.dev20230518/pyglove/core/symbolic/dict.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230517/pyglove/core/symbolic/dict_test.py` & `pyglove-0.3.1.dev20230518/pyglove/core/symbolic/dict_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230517/pyglove/core/symbolic/diff.py` & `pyglove-0.3.1.dev20230518/pyglove/core/symbolic/diff.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230517/pyglove/core/symbolic/diff_test.py` & `pyglove-0.3.1.dev20230518/pyglove/core/symbolic/diff_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230517/pyglove/core/symbolic/flags.py` & `pyglove-0.3.1.dev20230518/pyglove/core/symbolic/flags.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230517/pyglove/core/symbolic/flags_test.py` & `pyglove-0.3.1.dev20230518/pyglove/core/symbolic/flags_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230517/pyglove/core/symbolic/functor.py` & `pyglove-0.3.1.dev20230518/pyglove/core/symbolic/functor.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230517/pyglove/core/symbolic/functor_test.py` & `pyglove-0.3.1.dev20230518/pyglove/core/symbolic/functor_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230517/pyglove/core/symbolic/list.py` & `pyglove-0.3.1.dev20230518/pyglove/core/symbolic/list.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230517/pyglove/core/symbolic/list_test.py` & `pyglove-0.3.1.dev20230518/pyglove/core/symbolic/list_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230517/pyglove/core/symbolic/object.py` & `pyglove-0.3.1.dev20230518/pyglove/core/symbolic/object.py`

 * *Files 3% similar despite different names*

```diff
@@ -173,16 +173,17 @@
             base_schema_list=base_schema_list,
             allow_nonconst_keys=True,
             metadata={}))
     setattr(cls, '__schema__', cls_schema)
     setattr(cls, '__sym_fields', pg_typing.Dict(cls_schema))
     setattr(cls, '__serialization_key__', cls.type_name)
     cls_schema.metadata['init_arg_list'] = schema_utils.auto_init_arg_list(cls)
-    cls._update_init_signature_based_on_schema()
-    cls._generate_sym_attributes_if_enabled()
+
+    # Trigger schema update event.
+    cls._on_schema_update()
 
   @classmethod
   def _infer_fields_from_annotations(cls) -> List[pg_typing.Field]:
     """Infers symbolic fields from class annotations."""
     if not cls.infer_symbolic_fields_from_annotations:
       return []
 
@@ -203,14 +204,28 @@
       attr_value = getattr(cls, attr_name, pg_typing.MISSING_VALUE)
       if attr_value != pg_typing.MISSING_VALUE:
         field.value.set_default(attr_value)
       fields.append(field)
     return fields
 
   @classmethod
+  def _on_schema_update(cls):
+    """Triggers when the schema for the class has been updated."""
+    # Update the default value for each field after schema is updated. This is
+    # because that users may change a field's default value via class attribute.
+    cls._update_default_values_from_class_attributes()
+
+    # Update the signature of __init__.
+    cls._update_init_signature_based_on_schema()
+
+    # Expose symbolic attributes as object attributes when being asked.
+    if cls.allow_symbolic_attribute:
+      cls._generate_sym_attributes()
+
+  @classmethod
   def _update_init_signature_based_on_schema(cls):
     """Updates the signature of `__init__` if needed."""
     if (cls.__init__ is not Object.__init__
         and not hasattr(cls.__init__, '__sym_generated_init__')):
       # We only generate `__init__` from pg.Object subclass which does not
       # override the `__init__` method.
       # Functor and ClassWrapper override their `__init__` methods, therefore
@@ -230,32 +245,42 @@
       # be delegated to `Object.__init__` eventually. Therefore, directly
       # calling `Object.__init__` is equivalent to calling `super().__init__`.
       Object.__init__(self, *args, **kwargs)
     setattr(_init, '__sym_generated_init__', True)
     setattr(cls, '__init__', _init)
 
   @classmethod
-  def _generate_sym_attributes_if_enabled(cls):
+  def _update_default_values_from_class_attributes(cls):
+    for field in cls.schema.fields.values():
+      if isinstance(field.key, pg_typing.ConstStrKey):
+        attr_name = field.key.text
+        attr_value = getattr(cls, attr_name, pg_typing.MISSING_VALUE)
+        if (attr_value != pg_typing.MISSING_VALUE
+            and not isinstance(attr_value, property)
+            and not inspect.isfunction(attr_value)):
+          field.value.set_default(attr_value)
+
+  @classmethod
+  def _generate_sym_attributes(cls):
     """Generates symbolic attributes based on schema if they are enabled."""
     def _create_sym_attribute(attr_name, field):
       return property(object_utils.make_function(
           attr_name,
           ['self'],
           [f'return self._sym_attributes[\'{attr_name}\']'],
           return_type=field.value.annotation))
 
-    if cls.allow_symbolic_attribute:
-      for key, field in cls.schema.fields.items():
-        if isinstance(key, pg_typing.ConstStrKey):
-          attr_name = str(key)
-          attr_value = getattr(cls, attr_name, pg_typing.MISSING_VALUE)
-          if (attr_value == pg_typing.MISSING_VALUE
-              or (not inspect.isfunction(attr_value)
-                  and not isinstance(attr_value, property))):
-            setattr(cls, attr_name, _create_sym_attribute(attr_name, field))
+    for key, field in cls.schema.fields.items():
+      if isinstance(key, pg_typing.ConstStrKey):
+        attr_name = str(key)
+        attr_value = getattr(cls, attr_name, pg_typing.MISSING_VALUE)
+        if (attr_value == pg_typing.MISSING_VALUE
+            or (not inspect.isfunction(attr_value)
+                and not isinstance(attr_value, property))):
+          setattr(cls, attr_name, _create_sym_attribute(attr_name, field))
 
   @classmethod
   def partial(cls, *args, **kwargs) -> 'Object':
     """Class method that creates a partial object of current class."""
     return cls(*args, allow_partial=True, **kwargs)
 
   @classmethod
```

### Comparing `pyglove-0.3.1.dev20230517/pyglove/core/symbolic/object_test.py` & `pyglove-0.3.1.dev20230518/pyglove/core/symbolic/object_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -275,14 +275,39 @@
     self.assertEqual(d.x, 1)
     self.assertEqual(d.y, 1.0)
     self.assertEqual(d.q, 2)
     self.assertEqual(d.k, 3)
     self.assertEqual(d.e, 4)
     self.assertEqual(d.f, 5)
 
+  def test_update_of_default_values(self):
+
+    class A(Object):
+      x: int
+
+    class B(A):
+      x = 1
+    self.assertEqual(B().x, 1)
+
+    class C(B):
+      x = 2
+    self.assertEqual(C().x, 2)
+
+    @pg_members([
+        ('x', pg_typing.Int(default=3))
+    ])
+    class D(C):
+      pass
+    self.assertEqual(D().x, 3)
+
+    class F(D):
+      def x(self):
+        pass
+    self.assertEqual(F().sym_init_args.x, 3)
+
   def test_override_symbolic_attribute_with_property(self):
 
     @pg_members([
         ('x', pg_typing.Int()),
         ('y', pg_typing.Int()),
         ('z', pg_typing.Int()),
     ])
```

### Comparing `pyglove-0.3.1.dev20230517/pyglove/core/symbolic/origin.py` & `pyglove-0.3.1.dev20230518/pyglove/core/symbolic/origin.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230517/pyglove/core/symbolic/origin_test.py` & `pyglove-0.3.1.dev20230518/pyglove/core/symbolic/origin_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230517/pyglove/core/symbolic/pure_symbolic.py` & `pyglove-0.3.1.dev20230518/pyglove/core/symbolic/pure_symbolic.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230517/pyglove/core/symbolic/schema_utils.py` & `pyglove-0.3.1.dev20230518/pyglove/core/symbolic/schema_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -111,21 +111,20 @@
     init_arg_list = metadata.pop('init_arg_list', auto_init_arg_list(cls))
   validate_init_arg_list(init_arg_list, cls_schema)
   cls_schema.metadata['init_arg_list'] = init_arg_list
 
   if description is not None:
     cls_schema.set_description(description)
 
+  cls._on_schema_update()  # pylint: disable=protected-access
+
   if add_to_registry:
     register_serialization_keys(
         cls, serialization_key, additional_keys)
 
-  cls._update_init_signature_based_on_schema()  # pylint: disable=protected-access
-  cls._generate_sym_attributes_if_enabled()  # pylint: disable=protected-access
-
 
 def validate_init_arg_list(
     init_arg_list: List[str], cls_schema: pg_typing.Schema) -> None:
   """Validate init arg list."""
   for i, arg in enumerate(init_arg_list):
     is_vararg = False
     if i == len(init_arg_list) - 1 and arg.startswith('*'):
```

### Comparing `pyglove-0.3.1.dev20230517/pyglove/core/symbolic/schema_utils_test.py` & `pyglove-0.3.1.dev20230518/pyglove/core/symbolic/schema_utils_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230517/pyglove/core/symbolic/symbolize.py` & `pyglove-0.3.1.dev20230518/pyglove/core/symbolic/symbolize.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230517/pyglove/core/symbolic/symbolize_test.py` & `pyglove-0.3.1.dev20230518/pyglove/core/symbolic/symbolize_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230517/pyglove/core/tuning/__init__.py` & `pyglove-0.3.1.dev20230518/pyglove/core/tuning/__init__.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230517/pyglove/core/tuning/backend.py` & `pyglove-0.3.1.dev20230518/pyglove/core/tuning/backend.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230517/pyglove/core/tuning/backend_test.py` & `pyglove-0.3.1.dev20230518/pyglove/core/tuning/backend_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230517/pyglove/core/tuning/early_stopping.py` & `pyglove-0.3.1.dev20230518/pyglove/core/tuning/early_stopping.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230517/pyglove/core/tuning/local_backend.py` & `pyglove-0.3.1.dev20230518/pyglove/core/tuning/local_backend.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230517/pyglove/core/tuning/protocols.py` & `pyglove-0.3.1.dev20230518/pyglove/core/tuning/protocols.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230517/pyglove/core/tuning/protocols_test.py` & `pyglove-0.3.1.dev20230518/pyglove/core/tuning/protocols_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230517/pyglove/core/tuning/sample.py` & `pyglove-0.3.1.dev20230518/pyglove/core/tuning/sample.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230517/pyglove/core/tuning/sample_test.py` & `pyglove-0.3.1.dev20230518/pyglove/core/tuning/sample_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230517/pyglove/core/typing/__init__.py` & `pyglove-0.3.1.dev20230518/pyglove/core/typing/__init__.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230517/pyglove/core/typing/callable_ext.py` & `pyglove-0.3.1.dev20230518/pyglove/core/typing/callable_ext.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230517/pyglove/core/typing/callable_ext_test.py` & `pyglove-0.3.1.dev20230518/pyglove/core/typing/callable_ext_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230517/pyglove/core/typing/callable_signature.py` & `pyglove-0.3.1.dev20230518/pyglove/core/typing/callable_signature.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230517/pyglove/core/typing/callable_signature_test.py` & `pyglove-0.3.1.dev20230518/pyglove/core/typing/callable_signature_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230517/pyglove/core/typing/class_schema.py` & `pyglove-0.3.1.dev20230518/pyglove/core/typing/class_schema.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230517/pyglove/core/typing/class_schema_test.py` & `pyglove-0.3.1.dev20230518/pyglove/core/typing/class_schema_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230517/pyglove/core/typing/class_schema_utils.py` & `pyglove-0.3.1.dev20230518/pyglove/core/typing/class_schema_utils.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230517/pyglove/core/typing/class_schema_utils_test.py` & `pyglove-0.3.1.dev20230518/pyglove/core/typing/class_schema_utils_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230517/pyglove/core/typing/custom_typing.py` & `pyglove-0.3.1.dev20230518/pyglove/core/typing/custom_typing.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230517/pyglove/core/typing/key_specs.py` & `pyglove-0.3.1.dev20230518/pyglove/core/typing/key_specs.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230517/pyglove/core/typing/key_specs_test.py` & `pyglove-0.3.1.dev20230518/pyglove/core/typing/key_specs_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230517/pyglove/core/typing/pytype_support.py` & `pyglove-0.3.1.dev20230518/pyglove/core/typing/pytype_support.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230517/pyglove/core/typing/type_conversion.py` & `pyglove-0.3.1.dev20230518/pyglove/core/typing/type_conversion.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230517/pyglove/core/typing/type_conversion_test.py` & `pyglove-0.3.1.dev20230518/pyglove/core/typing/type_conversion_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230517/pyglove/core/typing/typed_missing.py` & `pyglove-0.3.1.dev20230518/pyglove/core/typing/typed_missing.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230517/pyglove/core/typing/typed_missing_test.py` & `pyglove-0.3.1.dev20230518/pyglove/core/typing/typed_missing_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230517/pyglove/core/typing/value_specs.py` & `pyglove-0.3.1.dev20230518/pyglove/core/typing/value_specs.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230517/pyglove/core/typing/value_specs_test.py` & `pyglove-0.3.1.dev20230518/pyglove/core/typing/value_specs_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230517/pyglove/ext/__init__.py` & `pyglove-0.3.1.dev20230518/pyglove/ext/__init__.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230517/pyglove/ext/early_stopping/__init__.py` & `pyglove-0.3.1.dev20230518/pyglove/ext/early_stopping/__init__.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230517/pyglove/ext/early_stopping/base.py` & `pyglove-0.3.1.dev20230518/pyglove/ext/early_stopping/base.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230517/pyglove/ext/early_stopping/base_test.py` & `pyglove-0.3.1.dev20230518/pyglove/ext/early_stopping/base_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230517/pyglove/ext/early_stopping/step_wise.py` & `pyglove-0.3.1.dev20230518/pyglove/ext/early_stopping/step_wise.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230517/pyglove/ext/early_stopping/step_wise_test.py` & `pyglove-0.3.1.dev20230518/pyglove/ext/early_stopping/step_wise_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230517/pyglove/ext/evolution/__init__.py` & `pyglove-0.3.1.dev20230518/pyglove/ext/evolution/__init__.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230517/pyglove/ext/evolution/base.py` & `pyglove-0.3.1.dev20230518/pyglove/ext/evolution/base.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230517/pyglove/ext/evolution/base_test.py` & `pyglove-0.3.1.dev20230518/pyglove/ext/evolution/base_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230517/pyglove/ext/evolution/hill_climb.py` & `pyglove-0.3.1.dev20230518/pyglove/ext/evolution/hill_climb.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230517/pyglove/ext/evolution/hill_climb_test.py` & `pyglove-0.3.1.dev20230518/pyglove/ext/evolution/hill_climb_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230517/pyglove/ext/evolution/mutators.py` & `pyglove-0.3.1.dev20230518/pyglove/ext/evolution/mutators.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230517/pyglove/ext/evolution/mutators_test.py` & `pyglove-0.3.1.dev20230518/pyglove/ext/evolution/mutators_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230517/pyglove/ext/evolution/neat.py` & `pyglove-0.3.1.dev20230518/pyglove/ext/evolution/neat.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230517/pyglove/ext/evolution/neat_test.py` & `pyglove-0.3.1.dev20230518/pyglove/ext/evolution/neat_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230517/pyglove/ext/evolution/nsga2.py` & `pyglove-0.3.1.dev20230518/pyglove/ext/evolution/nsga2.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230517/pyglove/ext/evolution/nsga2_test.py` & `pyglove-0.3.1.dev20230518/pyglove/ext/evolution/nsga2_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230517/pyglove/ext/evolution/recombinators.py` & `pyglove-0.3.1.dev20230518/pyglove/ext/evolution/recombinators.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230517/pyglove/ext/evolution/recombinators_test.py` & `pyglove-0.3.1.dev20230518/pyglove/ext/evolution/recombinators_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230517/pyglove/ext/evolution/regularized_evolution.py` & `pyglove-0.3.1.dev20230518/pyglove/ext/evolution/regularized_evolution.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230517/pyglove/ext/evolution/regularized_evolution_test.py` & `pyglove-0.3.1.dev20230518/pyglove/ext/evolution/regularized_evolution_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230517/pyglove/ext/evolution/selectors.py` & `pyglove-0.3.1.dev20230518/pyglove/ext/evolution/selectors.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230517/pyglove/ext/evolution/selectors_test.py` & `pyglove-0.3.1.dev20230518/pyglove/ext/evolution/selectors_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230517/pyglove/ext/evolution/where.py` & `pyglove-0.3.1.dev20230518/pyglove/ext/evolution/where.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230517/pyglove/ext/evolution/where_test.py` & `pyglove-0.3.1.dev20230518/pyglove/ext/evolution/where_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230517/pyglove/ext/mutfun/__init__.py` & `pyglove-0.3.1.dev20230518/pyglove/ext/mutfun/__init__.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230517/pyglove/ext/mutfun/base.py` & `pyglove-0.3.1.dev20230518/pyglove/ext/mutfun/base.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230517/pyglove/ext/mutfun/base_test.py` & `pyglove-0.3.1.dev20230518/pyglove/ext/mutfun/base_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230517/pyglove/ext/mutfun/basic_ops.py` & `pyglove-0.3.1.dev20230518/pyglove/ext/mutfun/basic_ops.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230517/pyglove/ext/mutfun/basic_ops_test.py` & `pyglove-0.3.1.dev20230518/pyglove/ext/mutfun/basic_ops_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230517/pyglove/ext/scalars/__init__.py` & `pyglove-0.3.1.dev20230518/pyglove/ext/scalars/__init__.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230517/pyglove/ext/scalars/base.py` & `pyglove-0.3.1.dev20230518/pyglove/ext/scalars/base.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230517/pyglove/ext/scalars/base_test.py` & `pyglove-0.3.1.dev20230518/pyglove/ext/scalars/base_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230517/pyglove/ext/scalars/maths.py` & `pyglove-0.3.1.dev20230518/pyglove/ext/scalars/maths.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230517/pyglove/ext/scalars/maths_test.py` & `pyglove-0.3.1.dev20230518/pyglove/ext/scalars/maths_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230517/pyglove/ext/scalars/randoms.py` & `pyglove-0.3.1.dev20230518/pyglove/ext/scalars/randoms.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230517/pyglove/ext/scalars/randoms_test.py` & `pyglove-0.3.1.dev20230518/pyglove/ext/scalars/randoms_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230517/pyglove/ext/scalars/step_wise.py` & `pyglove-0.3.1.dev20230518/pyglove/ext/scalars/step_wise.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230517/pyglove/ext/scalars/step_wise_test.py` & `pyglove-0.3.1.dev20230518/pyglove/ext/scalars/step_wise_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230517/pyglove.egg-info/PKG-INFO` & `pyglove-0.3.1.dev20230518/pyglove.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyglove
-Version: 0.3.1.dev20230517
+Version: 0.3.1.dev20230518
 Summary: PyGlove: A library for manipulating Python objects.
 Home-page: https://github.com/google/pyglove
 Author: PyGlove Authors
 Author-email: pyglove-authors@google.com
 License: Apache License 2.0
 Keywords: ai machine learning automl mutable symbolic framework meta-programming
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `pyglove-0.3.1.dev20230517/pyglove.egg-info/SOURCES.txt` & `pyglove-0.3.1.dev20230518/pyglove.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230517/setup.py` & `pyglove-0.3.1.dev20230518/setup.py`

 * *Files identical despite different names*

