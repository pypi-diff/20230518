# Comparing `tmp/CADET-Process-0.7.1.tar.gz` & `tmp/CADET-Process-0.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CADET-Process-0.7.1.tar", last modified: Sun May 14 12:49:46 2023, max compression
+gzip compressed data, was "CADET-Process-0.7.2.tar", last modified: Thu May 18 07:36:37 2023, max compression
```

## Comparing `CADET-Process-0.7.1.tar` & `CADET-Process-0.7.2.tar`

### file list

```diff
@@ -1,135 +1,135 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 12:49:46.163083 CADET-Process-0.7.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 12:49:46.143083 CADET-Process-0.7.1/CADETProcess/
--rw-r--r--   0 runner    (1001) docker     (123)      421 2023-05-14 12:49:35.000000 CADET-Process-0.7.1/CADETProcess/CADETProcessError.py
--rw-r--r--   0 runner    (1001) docker     (123)      960 2023-05-14 12:49:35.000000 CADET-Process-0.7.1/CADETProcess/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 12:49:46.143083 CADET-Process-0.7.1/CADETProcess/comparison/
--rw-r--r--   0 runner    (1001) docker     (123)      656 2023-05-14 12:49:35.000000 CADET-Process-0.7.1/CADETProcess/comparison/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11685 2023-05-14 12:49:35.000000 CADET-Process-0.7.1/CADETProcess/comparison/comparator.py
--rw-r--r--   0 runner    (1001) docker     (123)    29078 2023-05-14 12:49:35.000000 CADET-Process-0.7.1/CADETProcess/comparison/difference.py
--rw-r--r--   0 runner    (1001) docker     (123)     3064 2023-05-14 12:49:35.000000 CADET-Process-0.7.1/CADETProcess/comparison/peaks.py
--rw-r--r--   0 runner    (1001) docker     (123)     6833 2023-05-14 12:49:35.000000 CADET-Process-0.7.1/CADETProcess/comparison/shape.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 12:49:46.143083 CADET-Process-0.7.1/CADETProcess/dataStructure/
--rw-r--r--   0 runner    (1001) docker     (123)      966 2023-05-14 12:49:35.000000 CADET-Process-0.7.1/CADETProcess/dataStructure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      736 2023-05-14 12:49:35.000000 CADET-Process-0.7.1/CADETProcess/dataStructure/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     2981 2023-05-14 12:49:35.000000 CADET-Process-0.7.1/CADETProcess/dataStructure/dataStructure.py
--rw-r--r--   0 runner    (1001) docker     (123)     5053 2023-05-14 12:49:35.000000 CADET-Process-0.7.1/CADETProcess/dataStructure/diskcache.py
--rw-r--r--   0 runner    (1001) docker     (123)      397 2023-05-14 12:49:35.000000 CADET-Process-0.7.1/CADETProcess/dataStructure/encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     2252 2023-05-14 12:49:35.000000 CADET-Process-0.7.1/CADETProcess/dataStructure/nested_dict.py
--rw-r--r--   0 runner    (1001) docker     (123)    16173 2023-05-14 12:49:35.000000 CADET-Process-0.7.1/CADETProcess/dataStructure/parameter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3761 2023-05-14 12:49:35.000000 CADET-Process-0.7.1/CADETProcess/dataStructure/parameter_group.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 12:49:46.147083 CADET-Process-0.7.1/CADETProcess/dynamicEvents/
--rw-r--r--   0 runner    (1001) docker     (123)      611 2023-05-14 12:49:35.000000 CADET-Process-0.7.1/CADETProcess/dynamicEvents/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    29487 2023-05-14 12:49:35.000000 CADET-Process-0.7.1/CADETProcess/dynamicEvents/event.py
--rw-r--r--   0 runner    (1001) docker     (123)    16545 2023-05-14 12:49:35.000000 CADET-Process-0.7.1/CADETProcess/dynamicEvents/section.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 12:49:46.147083 CADET-Process-0.7.1/CADETProcess/equilibria/
--rw-r--r--   0 runner    (1001) docker     (123)      838 2023-05-14 12:49:35.000000 CADET-Process-0.7.1/CADETProcess/equilibria/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11299 2023-05-14 12:49:35.000000 CADET-Process-0.7.1/CADETProcess/equilibria/buffer_capacity.py
--rw-r--r--   0 runner    (1001) docker     (123)     3721 2023-05-14 12:49:35.000000 CADET-Process-0.7.1/CADETProcess/equilibria/initial_conditions.py
--rw-r--r--   0 runner    (1001) docker     (123)     5195 2023-05-14 12:49:35.000000 CADET-Process-0.7.1/CADETProcess/equilibria/ptc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4151 2023-05-14 12:49:35.000000 CADET-Process-0.7.1/CADETProcess/equilibria/reaction_equilibria.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 12:49:46.147083 CADET-Process-0.7.1/CADETProcess/fractionation/
--rw-r--r--   0 runner    (1001) docker     (123)      466 2023-05-14 12:49:35.000000 CADET-Process-0.7.1/CADETProcess/fractionation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10687 2023-05-14 12:49:35.000000 CADET-Process-0.7.1/CADETProcess/fractionation/fractionationOptimizer.py
--rw-r--r--   0 runner    (1001) docker     (123)    19812 2023-05-14 12:49:35.000000 CADET-Process-0.7.1/CADETProcess/fractionation/fractionator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4924 2023-05-14 12:49:35.000000 CADET-Process-0.7.1/CADETProcess/fractionation/fractions.py
--rw-r--r--   0 runner    (1001) docker     (123)     5067 2023-05-14 12:49:35.000000 CADET-Process-0.7.1/CADETProcess/log.py
--rw-r--r--   0 runner    (1001) docker     (123)      494 2023-05-14 12:49:35.000000 CADET-Process-0.7.1/CADETProcess/metric.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 12:49:46.147083 CADET-Process-0.7.1/CADETProcess/modelBuilder/
--rw-r--r--   0 runner    (1001) docker     (123)      731 2023-05-14 12:49:35.000000 CADET-Process-0.7.1/CADETProcess/modelBuilder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15005 2023-05-14 12:49:35.000000 CADET-Process-0.7.1/CADETProcess/modelBuilder/carouselBuilder.py
--rw-r--r--   0 runner    (1001) docker     (123)    10546 2023-05-14 12:49:35.000000 CADET-Process-0.7.1/CADETProcess/modelBuilder/compartmentBuilder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 12:49:46.151083 CADET-Process-0.7.1/CADETProcess/optimization/
--rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-05-14 12:49:35.000000 CADET-Process-0.7.1/CADETProcess/optimization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4722 2023-05-14 12:49:35.000000 CADET-Process-0.7.1/CADETProcess/optimization/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)    10318 2023-05-14 12:49:35.000000 CADET-Process-0.7.1/CADETProcess/optimization/individual.py
--rw-r--r--   0 runner    (1001) docker     (123)    98472 2023-05-14 12:49:35.000000 CADET-Process-0.7.1/CADETProcess/optimization/optimizationProblem.py
--rw-r--r--   0 runner    (1001) docker     (123)    16546 2023-05-14 12:49:35.000000 CADET-Process-0.7.1/CADETProcess/optimization/optimizer.py
--rw-r--r--   0 runner    (1001) docker     (123)    26654 2023-05-14 12:49:35.000000 CADET-Process-0.7.1/CADETProcess/optimization/population.py
--rw-r--r--   0 runner    (1001) docker     (123)     8975 2023-05-14 12:49:35.000000 CADET-Process-0.7.1/CADETProcess/optimization/pymooAdapter.py
--rw-r--r--   0 runner    (1001) docker     (123)    27585 2023-05-14 12:49:35.000000 CADET-Process-0.7.1/CADETProcess/optimization/results.py
--rw-r--r--   0 runner    (1001) docker     (123)    12119 2023-05-14 12:49:35.000000 CADET-Process-0.7.1/CADETProcess/optimization/scipyAdapter.py
--rw-r--r--   0 runner    (1001) docker     (123)    10918 2023-05-14 12:49:35.000000 CADET-Process-0.7.1/CADETProcess/performance.py
--rw-r--r--   0 runner    (1001) docker     (123)     8423 2023-05-14 12:49:35.000000 CADET-Process-0.7.1/CADETProcess/plotting.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 12:49:46.151083 CADET-Process-0.7.1/CADETProcess/processModel/
--rw-r--r--   0 runner    (1001) docker     (123)     1946 2023-05-14 12:49:35.000000 CADET-Process-0.7.1/CADETProcess/processModel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    40569 2023-05-14 12:49:35.000000 CADET-Process-0.7.1/CADETProcess/processModel/binding.py
--rw-r--r--   0 runner    (1001) docker     (123)    10470 2023-05-14 12:49:35.000000 CADET-Process-0.7.1/CADETProcess/processModel/componentSystem.py
--rw-r--r--   0 runner    (1001) docker     (123)    22819 2023-05-14 12:49:35.000000 CADET-Process-0.7.1/CADETProcess/processModel/discretization.py
--rw-r--r--   0 runner    (1001) docker     (123)    31628 2023-05-14 12:49:35.000000 CADET-Process-0.7.1/CADETProcess/processModel/flowSheet.py
--rw-r--r--   0 runner    (1001) docker     (123)    25369 2023-05-14 12:49:35.000000 CADET-Process-0.7.1/CADETProcess/processModel/process.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    26945 2023-05-14 12:49:35.000000 CADET-Process-0.7.1/CADETProcess/processModel/reaction.py
--rw-r--r--   0 runner    (1001) docker     (123)     9452 2023-05-14 12:49:35.000000 CADET-Process-0.7.1/CADETProcess/processModel/solutionRecorder.py
--rw-r--r--   0 runner    (1001) docker     (123)    34406 2023-05-14 12:49:35.000000 CADET-Process-0.7.1/CADETProcess/processModel/unitOperation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2928 2023-05-14 12:49:35.000000 CADET-Process-0.7.1/CADETProcess/reference.py
--rw-r--r--   0 runner    (1001) docker     (123)     3780 2023-05-14 12:49:35.000000 CADET-Process-0.7.1/CADETProcess/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     8061 2023-05-14 12:49:35.000000 CADET-Process-0.7.1/CADETProcess/simulationResults.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 12:49:46.155083 CADET-Process-0.7.1/CADETProcess/simulator/
--rw-r--r--   0 runner    (1001) docker     (123)      976 2023-05-14 12:49:35.000000 CADET-Process-0.7.1/CADETProcess/simulator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    54643 2023-05-14 12:49:35.000000 CADET-Process-0.7.1/CADETProcess/simulator/cadetAdapter.py
--rw-r--r--   0 runner    (1001) docker     (123)    11112 2023-05-14 12:49:35.000000 CADET-Process-0.7.1/CADETProcess/simulator/simulator.py
--rw-r--r--   0 runner    (1001) docker     (123)     8797 2023-05-14 12:49:35.000000 CADET-Process-0.7.1/CADETProcess/smoothing.py
--rw-r--r--   0 runner    (1001) docker     (123)     2422 2023-05-14 12:49:35.000000 CADET-Process-0.7.1/CADETProcess/smoothing2.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    48809 2023-05-14 12:49:35.000000 CADET-Process-0.7.1/CADETProcess/solution.py
--rw-r--r--   0 runner    (1001) docker     (123)     4168 2023-05-14 12:49:35.000000 CADET-Process-0.7.1/CADETProcess/stationarity.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 12:49:46.155083 CADET-Process-0.7.1/CADETProcess/tools/
--rw-r--r--   0 runner    (1001) docker     (123)      378 2023-05-14 12:49:35.000000 CADET-Process-0.7.1/CADETProcess/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7301 2023-05-14 12:49:35.000000 CADET-Process-0.7.1/CADETProcess/tools/yamamoto.py
--rw-r--r--   0 runner    (1001) docker     (123)    14861 2023-05-14 12:49:35.000000 CADET-Process-0.7.1/CADETProcess/transform.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 12:49:46.155083 CADET-Process-0.7.1/CADET_Process.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4735 2023-05-14 12:49:46.000000 CADET-Process-0.7.1/CADET_Process.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3991 2023-05-14 12:49:46.000000 CADET-Process-0.7.1/CADET_Process.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-14 12:49:46.000000 CADET-Process-0.7.1/CADET_Process.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      372 2023-05-14 12:49:46.000000 CADET-Process-0.7.1/CADET_Process.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-14 12:49:46.000000 CADET-Process-0.7.1/CADET_Process.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-14 12:49:35.000000 CADET-Process-0.7.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4735 2023-05-14 12:49:46.163083 CADET-Process-0.7.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4061 2023-05-14 12:49:35.000000 CADET-Process-0.7.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 12:49:46.155083 CADET-Process-0.7.1/examples/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 12:49:35.000000 CADET-Process-0.7.1/examples/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 12:49:46.155083 CADET-Process-0.7.1/examples/batch_elution/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 12:49:35.000000 CADET-Process-0.7.1/examples/batch_elution/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2926 2023-05-14 12:49:35.000000 CADET-Process-0.7.1/examples/batch_elution/optimization_multi.py
--rw-r--r--   0 runner    (1001) docker     (123)     2545 2023-05-14 12:49:35.000000 CADET-Process-0.7.1/examples/batch_elution/optimization_single.py
--rw-r--r--   0 runner    (1001) docker     (123)     6109 2023-05-14 12:49:35.000000 CADET-Process-0.7.1/examples/batch_elution/process.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 12:49:46.155083 CADET-Process-0.7.1/examples/characterize_chromatographic_system/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 12:49:35.000000 CADET-Process-0.7.1/examples/characterize_chromatographic_system/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      351 2023-05-14 12:49:35.000000 CADET-Process-0.7.1/examples/characterize_chromatographic_system/binding_model_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     6514 2023-05-14 12:49:35.000000 CADET-Process-0.7.1/examples/characterize_chromatographic_system/column_transport_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     4495 2023-05-14 12:49:35.000000 CADET-Process-0.7.1/examples/characterize_chromatographic_system/particle_porosity.py
--rw-r--r--   0 runner    (1001) docker     (123)      448 2023-05-14 12:49:35.000000 CADET-Process-0.7.1/examples/characterize_chromatographic_system/system_periphery.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 12:49:46.155083 CADET-Process-0.7.1/examples/load_wash_elute/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 12:49:35.000000 CADET-Process-0.7.1/examples/load_wash_elute/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3487 2023-05-14 12:49:35.000000 CADET-Process-0.7.1/examples/load_wash_elute/lwe_concentration.py
--rw-r--r--   0 runner    (1001) docker     (123)     4247 2023-05-14 12:49:35.000000 CADET-Process-0.7.1/examples/load_wash_elute/lwe_flow_rate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 12:49:46.159083 CADET-Process-0.7.1/examples/recycling/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 12:49:35.000000 CADET-Process-0.7.1/examples/recycling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5772 2023-05-14 12:49:35.000000 CADET-Process-0.7.1/examples/recycling/clr_process.py
--rw-r--r--   0 runner    (1001) docker     (123)     6013 2023-05-14 12:49:35.000000 CADET-Process-0.7.1/examples/recycling/mrssr_process.py
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-14 12:49:35.000000 CADET-Process-0.7.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-05-14 12:49:46.163083 CADET-Process-0.7.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-05-14 12:49:35.000000 CADET-Process-0.7.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 12:49:46.163083 CADET-Process-0.7.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 12:49:35.000000 CADET-Process-0.7.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2292 2023-05-14 12:49:35.000000 CADET-Process-0.7.1/tests/test_binding.py
--rw-r--r--   0 runner    (1001) docker     (123)     8104 2023-05-14 12:49:35.000000 CADET-Process-0.7.1/tests/test_buffer_capacity.py
--rw-r--r--   0 runner    (1001) docker     (123)     3448 2023-05-14 12:49:35.000000 CADET-Process-0.7.1/tests/test_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)    20739 2023-05-14 12:49:35.000000 CADET-Process-0.7.1/tests/test_carousel.py
--rw-r--r--   0 runner    (1001) docker     (123)     6898 2023-05-14 12:49:35.000000 CADET-Process-0.7.1/tests/test_compartment.py
--rw-r--r--   0 runner    (1001) docker     (123)     3868 2023-05-14 12:49:35.000000 CADET-Process-0.7.1/tests/test_components.py
--rw-r--r--   0 runner    (1001) docker     (123)    12176 2023-05-14 12:49:35.000000 CADET-Process-0.7.1/tests/test_difference.py
--rw-r--r--   0 runner    (1001) docker     (123)     7228 2023-05-14 12:49:35.000000 CADET-Process-0.7.1/tests/test_equilibrium.py
--rw-r--r--   0 runner    (1001) docker     (123)     5600 2023-05-14 12:49:35.000000 CADET-Process-0.7.1/tests/test_events.py
--rw-r--r--   0 runner    (1001) docker     (123)    18558 2023-05-14 12:49:35.000000 CADET-Process-0.7.1/tests/test_flow_sheet.py
--rw-r--r--   0 runner    (1001) docker     (123)     4326 2023-05-14 12:49:35.000000 CADET-Process-0.7.1/tests/test_fractions.py
--rw-r--r--   0 runner    (1001) docker     (123)     5894 2023-05-14 12:49:35.000000 CADET-Process-0.7.1/tests/test_individual.py
--rw-r--r--   0 runner    (1001) docker     (123)     5326 2023-05-14 12:49:35.000000 CADET-Process-0.7.1/tests/test_optimization_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)    20252 2023-05-14 12:49:35.000000 CADET-Process-0.7.1/tests/test_optimization_problem.py
--rw-r--r--   0 runner    (1001) docker     (123)     2477 2023-05-14 12:49:35.000000 CADET-Process-0.7.1/tests/test_optimization_results.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5624 2023-05-14 12:49:35.000000 CADET-Process-0.7.1/tests/test_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     7710 2023-05-14 12:49:35.000000 CADET-Process-0.7.1/tests/test_population.py
--rw-r--r--   0 runner    (1001) docker     (123)      466 2023-05-14 12:49:35.000000 CADET-Process-0.7.1/tests/test_process.py
--rw-r--r--   0 runner    (1001) docker     (123)     9786 2023-05-14 12:49:35.000000 CADET-Process-0.7.1/tests/test_reaction.py
--rw-r--r--   0 runner    (1001) docker     (123)     8429 2023-05-14 12:49:35.000000 CADET-Process-0.7.1/tests/test_sections.py
--rw-r--r--   0 runner    (1001) docker     (123)    19066 2023-05-14 12:49:35.000000 CADET-Process-0.7.1/tests/test_solution.py
--rw-r--r--   0 runner    (1001) docker     (123)     4004 2023-05-14 12:49:35.000000 CADET-Process-0.7.1/tests/test_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     6695 2023-05-14 12:49:35.000000 CADET-Process-0.7.1/tests/test_unit_operation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 07:36:37.806254 CADET-Process-0.7.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 07:36:37.790253 CADET-Process-0.7.2/CADETProcess/
+-rw-r--r--   0 runner    (1001) docker     (123)      421 2023-05-18 07:36:25.000000 CADET-Process-0.7.2/CADETProcess/CADETProcessError.py
+-rw-r--r--   0 runner    (1001) docker     (123)      960 2023-05-18 07:36:25.000000 CADET-Process-0.7.2/CADETProcess/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 07:36:37.790253 CADET-Process-0.7.2/CADETProcess/comparison/
+-rw-r--r--   0 runner    (1001) docker     (123)      656 2023-05-18 07:36:25.000000 CADET-Process-0.7.2/CADETProcess/comparison/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11685 2023-05-18 07:36:25.000000 CADET-Process-0.7.2/CADETProcess/comparison/comparator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29078 2023-05-18 07:36:25.000000 CADET-Process-0.7.2/CADETProcess/comparison/difference.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3064 2023-05-18 07:36:25.000000 CADET-Process-0.7.2/CADETProcess/comparison/peaks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6833 2023-05-18 07:36:25.000000 CADET-Process-0.7.2/CADETProcess/comparison/shape.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 07:36:37.790253 CADET-Process-0.7.2/CADETProcess/dataStructure/
+-rw-r--r--   0 runner    (1001) docker     (123)      966 2023-05-18 07:36:25.000000 CADET-Process-0.7.2/CADETProcess/dataStructure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      736 2023-05-18 07:36:25.000000 CADET-Process-0.7.2/CADETProcess/dataStructure/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2981 2023-05-18 07:36:25.000000 CADET-Process-0.7.2/CADETProcess/dataStructure/dataStructure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5053 2023-05-18 07:36:25.000000 CADET-Process-0.7.2/CADETProcess/dataStructure/diskcache.py
+-rw-r--r--   0 runner    (1001) docker     (123)      397 2023-05-18 07:36:25.000000 CADET-Process-0.7.2/CADETProcess/dataStructure/encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2252 2023-05-18 07:36:25.000000 CADET-Process-0.7.2/CADETProcess/dataStructure/nested_dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16173 2023-05-18 07:36:25.000000 CADET-Process-0.7.2/CADETProcess/dataStructure/parameter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3761 2023-05-18 07:36:25.000000 CADET-Process-0.7.2/CADETProcess/dataStructure/parameter_group.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 07:36:37.790253 CADET-Process-0.7.2/CADETProcess/dynamicEvents/
+-rw-r--r--   0 runner    (1001) docker     (123)      611 2023-05-18 07:36:25.000000 CADET-Process-0.7.2/CADETProcess/dynamicEvents/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29487 2023-05-18 07:36:25.000000 CADET-Process-0.7.2/CADETProcess/dynamicEvents/event.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16545 2023-05-18 07:36:25.000000 CADET-Process-0.7.2/CADETProcess/dynamicEvents/section.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 07:36:37.794253 CADET-Process-0.7.2/CADETProcess/equilibria/
+-rw-r--r--   0 runner    (1001) docker     (123)      838 2023-05-18 07:36:25.000000 CADET-Process-0.7.2/CADETProcess/equilibria/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11299 2023-05-18 07:36:25.000000 CADET-Process-0.7.2/CADETProcess/equilibria/buffer_capacity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3721 2023-05-18 07:36:25.000000 CADET-Process-0.7.2/CADETProcess/equilibria/initial_conditions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5195 2023-05-18 07:36:25.000000 CADET-Process-0.7.2/CADETProcess/equilibria/ptc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4151 2023-05-18 07:36:25.000000 CADET-Process-0.7.2/CADETProcess/equilibria/reaction_equilibria.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 07:36:37.794253 CADET-Process-0.7.2/CADETProcess/fractionation/
+-rw-r--r--   0 runner    (1001) docker     (123)      466 2023-05-18 07:36:25.000000 CADET-Process-0.7.2/CADETProcess/fractionation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10687 2023-05-18 07:36:25.000000 CADET-Process-0.7.2/CADETProcess/fractionation/fractionationOptimizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19812 2023-05-18 07:36:25.000000 CADET-Process-0.7.2/CADETProcess/fractionation/fractionator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4924 2023-05-18 07:36:25.000000 CADET-Process-0.7.2/CADETProcess/fractionation/fractions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5067 2023-05-18 07:36:25.000000 CADET-Process-0.7.2/CADETProcess/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)      494 2023-05-18 07:36:25.000000 CADET-Process-0.7.2/CADETProcess/metric.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 07:36:37.794253 CADET-Process-0.7.2/CADETProcess/modelBuilder/
+-rw-r--r--   0 runner    (1001) docker     (123)      731 2023-05-18 07:36:25.000000 CADET-Process-0.7.2/CADETProcess/modelBuilder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15005 2023-05-18 07:36:25.000000 CADET-Process-0.7.2/CADETProcess/modelBuilder/carouselBuilder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10546 2023-05-18 07:36:25.000000 CADET-Process-0.7.2/CADETProcess/modelBuilder/compartmentBuilder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 07:36:37.794253 CADET-Process-0.7.2/CADETProcess/optimization/
+-rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-05-18 07:36:25.000000 CADET-Process-0.7.2/CADETProcess/optimization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4722 2023-05-18 07:36:25.000000 CADET-Process-0.7.2/CADETProcess/optimization/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10318 2023-05-18 07:36:25.000000 CADET-Process-0.7.2/CADETProcess/optimization/individual.py
+-rw-r--r--   0 runner    (1001) docker     (123)    98472 2023-05-18 07:36:25.000000 CADET-Process-0.7.2/CADETProcess/optimization/optimizationProblem.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16828 2023-05-18 07:36:25.000000 CADET-Process-0.7.2/CADETProcess/optimization/optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26654 2023-05-18 07:36:25.000000 CADET-Process-0.7.2/CADETProcess/optimization/population.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8959 2023-05-18 07:36:25.000000 CADET-Process-0.7.2/CADETProcess/optimization/pymooAdapter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27585 2023-05-18 07:36:25.000000 CADET-Process-0.7.2/CADETProcess/optimization/results.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12128 2023-05-18 07:36:25.000000 CADET-Process-0.7.2/CADETProcess/optimization/scipyAdapter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10918 2023-05-18 07:36:25.000000 CADET-Process-0.7.2/CADETProcess/performance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8423 2023-05-18 07:36:25.000000 CADET-Process-0.7.2/CADETProcess/plotting.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 07:36:37.798254 CADET-Process-0.7.2/CADETProcess/processModel/
+-rw-r--r--   0 runner    (1001) docker     (123)     1946 2023-05-18 07:36:25.000000 CADET-Process-0.7.2/CADETProcess/processModel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40569 2023-05-18 07:36:25.000000 CADET-Process-0.7.2/CADETProcess/processModel/binding.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10470 2023-05-18 07:36:25.000000 CADET-Process-0.7.2/CADETProcess/processModel/componentSystem.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22819 2023-05-18 07:36:25.000000 CADET-Process-0.7.2/CADETProcess/processModel/discretization.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31628 2023-05-18 07:36:25.000000 CADET-Process-0.7.2/CADETProcess/processModel/flowSheet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25369 2023-05-18 07:36:25.000000 CADET-Process-0.7.2/CADETProcess/processModel/process.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    26945 2023-05-18 07:36:25.000000 CADET-Process-0.7.2/CADETProcess/processModel/reaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9452 2023-05-18 07:36:25.000000 CADET-Process-0.7.2/CADETProcess/processModel/solutionRecorder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34406 2023-05-18 07:36:25.000000 CADET-Process-0.7.2/CADETProcess/processModel/unitOperation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2928 2023-05-18 07:36:25.000000 CADET-Process-0.7.2/CADETProcess/reference.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3780 2023-05-18 07:36:25.000000 CADET-Process-0.7.2/CADETProcess/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8061 2023-05-18 07:36:25.000000 CADET-Process-0.7.2/CADETProcess/simulationResults.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 07:36:37.798254 CADET-Process-0.7.2/CADETProcess/simulator/
+-rw-r--r--   0 runner    (1001) docker     (123)      976 2023-05-18 07:36:25.000000 CADET-Process-0.7.2/CADETProcess/simulator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    54643 2023-05-18 07:36:25.000000 CADET-Process-0.7.2/CADETProcess/simulator/cadetAdapter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11112 2023-05-18 07:36:25.000000 CADET-Process-0.7.2/CADETProcess/simulator/simulator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8797 2023-05-18 07:36:25.000000 CADET-Process-0.7.2/CADETProcess/smoothing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2422 2023-05-18 07:36:25.000000 CADET-Process-0.7.2/CADETProcess/smoothing2.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    48809 2023-05-18 07:36:25.000000 CADET-Process-0.7.2/CADETProcess/solution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4168 2023-05-18 07:36:25.000000 CADET-Process-0.7.2/CADETProcess/stationarity.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 07:36:37.798254 CADET-Process-0.7.2/CADETProcess/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)      378 2023-05-18 07:36:25.000000 CADET-Process-0.7.2/CADETProcess/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7301 2023-05-18 07:36:25.000000 CADET-Process-0.7.2/CADETProcess/tools/yamamoto.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14861 2023-05-18 07:36:25.000000 CADET-Process-0.7.2/CADETProcess/transform.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 07:36:37.798254 CADET-Process-0.7.2/CADET_Process.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4735 2023-05-18 07:36:37.000000 CADET-Process-0.7.2/CADET_Process.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3991 2023-05-18 07:36:37.000000 CADET-Process-0.7.2/CADET_Process.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 07:36:37.000000 CADET-Process-0.7.2/CADET_Process.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-05-18 07:36:37.000000 CADET-Process-0.7.2/CADET_Process.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-18 07:36:37.000000 CADET-Process-0.7.2/CADET_Process.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-18 07:36:25.000000 CADET-Process-0.7.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4735 2023-05-18 07:36:37.806254 CADET-Process-0.7.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4061 2023-05-18 07:36:25.000000 CADET-Process-0.7.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 07:36:37.798254 CADET-Process-0.7.2/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 07:36:25.000000 CADET-Process-0.7.2/examples/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 07:36:37.798254 CADET-Process-0.7.2/examples/batch_elution/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 07:36:25.000000 CADET-Process-0.7.2/examples/batch_elution/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2926 2023-05-18 07:36:25.000000 CADET-Process-0.7.2/examples/batch_elution/optimization_multi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2545 2023-05-18 07:36:25.000000 CADET-Process-0.7.2/examples/batch_elution/optimization_single.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6109 2023-05-18 07:36:25.000000 CADET-Process-0.7.2/examples/batch_elution/process.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 07:36:37.802254 CADET-Process-0.7.2/examples/characterize_chromatographic_system/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 07:36:25.000000 CADET-Process-0.7.2/examples/characterize_chromatographic_system/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      351 2023-05-18 07:36:25.000000 CADET-Process-0.7.2/examples/characterize_chromatographic_system/binding_model_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6514 2023-05-18 07:36:25.000000 CADET-Process-0.7.2/examples/characterize_chromatographic_system/column_transport_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4495 2023-05-18 07:36:25.000000 CADET-Process-0.7.2/examples/characterize_chromatographic_system/particle_porosity.py
+-rw-r--r--   0 runner    (1001) docker     (123)      448 2023-05-18 07:36:25.000000 CADET-Process-0.7.2/examples/characterize_chromatographic_system/system_periphery.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 07:36:37.802254 CADET-Process-0.7.2/examples/load_wash_elute/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 07:36:25.000000 CADET-Process-0.7.2/examples/load_wash_elute/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3487 2023-05-18 07:36:25.000000 CADET-Process-0.7.2/examples/load_wash_elute/lwe_concentration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4247 2023-05-18 07:36:25.000000 CADET-Process-0.7.2/examples/load_wash_elute/lwe_flow_rate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 07:36:37.802254 CADET-Process-0.7.2/examples/recycling/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 07:36:25.000000 CADET-Process-0.7.2/examples/recycling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5772 2023-05-18 07:36:25.000000 CADET-Process-0.7.2/examples/recycling/clr_process.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6013 2023-05-18 07:36:25.000000 CADET-Process-0.7.2/examples/recycling/mrssr_process.py
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-18 07:36:25.000000 CADET-Process-0.7.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-05-18 07:36:37.806254 CADET-Process-0.7.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-05-18 07:36:25.000000 CADET-Process-0.7.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 07:36:37.806254 CADET-Process-0.7.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 07:36:25.000000 CADET-Process-0.7.2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2292 2023-05-18 07:36:25.000000 CADET-Process-0.7.2/tests/test_binding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8104 2023-05-18 07:36:25.000000 CADET-Process-0.7.2/tests/test_buffer_capacity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3448 2023-05-18 07:36:25.000000 CADET-Process-0.7.2/tests/test_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20739 2023-05-18 07:36:25.000000 CADET-Process-0.7.2/tests/test_carousel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6898 2023-05-18 07:36:25.000000 CADET-Process-0.7.2/tests/test_compartment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3868 2023-05-18 07:36:25.000000 CADET-Process-0.7.2/tests/test_components.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12176 2023-05-18 07:36:25.000000 CADET-Process-0.7.2/tests/test_difference.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7228 2023-05-18 07:36:25.000000 CADET-Process-0.7.2/tests/test_equilibrium.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5600 2023-05-18 07:36:25.000000 CADET-Process-0.7.2/tests/test_events.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18558 2023-05-18 07:36:25.000000 CADET-Process-0.7.2/tests/test_flow_sheet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4326 2023-05-18 07:36:25.000000 CADET-Process-0.7.2/tests/test_fractions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5894 2023-05-18 07:36:25.000000 CADET-Process-0.7.2/tests/test_individual.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5326 2023-05-18 07:36:25.000000 CADET-Process-0.7.2/tests/test_optimization_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20252 2023-05-18 07:36:25.000000 CADET-Process-0.7.2/tests/test_optimization_problem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2477 2023-05-18 07:36:25.000000 CADET-Process-0.7.2/tests/test_optimization_results.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5624 2023-05-18 07:36:25.000000 CADET-Process-0.7.2/tests/test_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7710 2023-05-18 07:36:25.000000 CADET-Process-0.7.2/tests/test_population.py
+-rw-r--r--   0 runner    (1001) docker     (123)      466 2023-05-18 07:36:25.000000 CADET-Process-0.7.2/tests/test_process.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9786 2023-05-18 07:36:25.000000 CADET-Process-0.7.2/tests/test_reaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8429 2023-05-18 07:36:25.000000 CADET-Process-0.7.2/tests/test_sections.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19066 2023-05-18 07:36:25.000000 CADET-Process-0.7.2/tests/test_solution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4004 2023-05-18 07:36:25.000000 CADET-Process-0.7.2/tests/test_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6695 2023-05-18 07:36:25.000000 CADET-Process-0.7.2/tests/test_unit_operation.py
```

### Comparing `CADET-Process-0.7.1/CADETProcess/__init__.py` & `CADET-Process-0.7.2/CADETProcess/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 advanced chromatographic systems. It serves as an inteface for CADET, but also
 for other solvers.
 
 See https://cadet-process.readthedocs.io for complete documentation.
 """
 # Version information
 name = 'CADET-Process'
-__version__ = '0.7.1'
+__version__ = '0.7.2'
 
 # Imports
 from .CADETProcessError import *
 
 from . import log
 
 from .settings import Settings
```

### Comparing `CADET-Process-0.7.1/CADETProcess/comparison/__init__.py` & `CADET-Process-0.7.2/CADETProcess/comparison/__init__.py`

 * *Files identical despite different names*

### Comparing `CADET-Process-0.7.1/CADETProcess/comparison/comparator.py` & `CADET-Process-0.7.2/CADETProcess/comparison/comparator.py`

 * *Files identical despite different names*

### Comparing `CADET-Process-0.7.1/CADETProcess/comparison/difference.py` & `CADET-Process-0.7.2/CADETProcess/comparison/difference.py`

 * *Files identical despite different names*

### Comparing `CADET-Process-0.7.1/CADETProcess/comparison/peaks.py` & `CADET-Process-0.7.2/CADETProcess/comparison/peaks.py`

 * *Files identical despite different names*

### Comparing `CADET-Process-0.7.1/CADETProcess/comparison/shape.py` & `CADET-Process-0.7.2/CADETProcess/comparison/shape.py`

 * *Files identical despite different names*

### Comparing `CADET-Process-0.7.1/CADETProcess/dataStructure/__init__.py` & `CADET-Process-0.7.2/CADETProcess/dataStructure/__init__.py`

 * *Files identical despite different names*

### Comparing `CADET-Process-0.7.1/CADETProcess/dataStructure/cache.py` & `CADET-Process-0.7.2/CADETProcess/dataStructure/cache.py`

 * *Files identical despite different names*

### Comparing `CADET-Process-0.7.1/CADETProcess/dataStructure/dataStructure.py` & `CADET-Process-0.7.2/CADETProcess/dataStructure/dataStructure.py`

 * *Files identical despite different names*

### Comparing `CADET-Process-0.7.1/CADETProcess/dataStructure/diskcache.py` & `CADET-Process-0.7.2/CADETProcess/dataStructure/diskcache.py`

 * *Files identical despite different names*

### Comparing `CADET-Process-0.7.1/CADETProcess/dataStructure/nested_dict.py` & `CADET-Process-0.7.2/CADETProcess/dataStructure/nested_dict.py`

 * *Files identical despite different names*

### Comparing `CADET-Process-0.7.1/CADETProcess/dataStructure/parameter.py` & `CADET-Process-0.7.2/CADETProcess/dataStructure/parameter.py`

 * *Files identical despite different names*

### Comparing `CADET-Process-0.7.1/CADETProcess/dataStructure/parameter_group.py` & `CADET-Process-0.7.2/CADETProcess/dataStructure/parameter_group.py`

 * *Files identical despite different names*

### Comparing `CADET-Process-0.7.1/CADETProcess/dynamicEvents/__init__.py` & `CADET-Process-0.7.2/CADETProcess/dynamicEvents/__init__.py`

 * *Files identical despite different names*

### Comparing `CADET-Process-0.7.1/CADETProcess/dynamicEvents/event.py` & `CADET-Process-0.7.2/CADETProcess/dynamicEvents/event.py`

 * *Files identical despite different names*

### Comparing `CADET-Process-0.7.1/CADETProcess/dynamicEvents/section.py` & `CADET-Process-0.7.2/CADETProcess/dynamicEvents/section.py`

 * *Files identical despite different names*

### Comparing `CADET-Process-0.7.1/CADETProcess/equilibria/__init__.py` & `CADET-Process-0.7.2/CADETProcess/equilibria/__init__.py`

 * *Files identical despite different names*

### Comparing `CADET-Process-0.7.1/CADETProcess/equilibria/buffer_capacity.py` & `CADET-Process-0.7.2/CADETProcess/equilibria/buffer_capacity.py`

 * *Files identical despite different names*

### Comparing `CADET-Process-0.7.1/CADETProcess/equilibria/initial_conditions.py` & `CADET-Process-0.7.2/CADETProcess/equilibria/initial_conditions.py`

 * *Files identical despite different names*

### Comparing `CADET-Process-0.7.1/CADETProcess/equilibria/ptc.py` & `CADET-Process-0.7.2/CADETProcess/equilibria/ptc.py`

 * *Files identical despite different names*

### Comparing `CADET-Process-0.7.1/CADETProcess/equilibria/reaction_equilibria.py` & `CADET-Process-0.7.2/CADETProcess/equilibria/reaction_equilibria.py`

 * *Files identical despite different names*

### Comparing `CADET-Process-0.7.1/CADETProcess/fractionation/fractionationOptimizer.py` & `CADET-Process-0.7.2/CADETProcess/fractionation/fractionationOptimizer.py`

 * *Files identical despite different names*

### Comparing `CADET-Process-0.7.1/CADETProcess/fractionation/fractionator.py` & `CADET-Process-0.7.2/CADETProcess/fractionation/fractionator.py`

 * *Files identical despite different names*

### Comparing `CADET-Process-0.7.1/CADETProcess/fractionation/fractions.py` & `CADET-Process-0.7.2/CADETProcess/fractionation/fractions.py`

 * *Files identical despite different names*

### Comparing `CADET-Process-0.7.1/CADETProcess/log.py` & `CADET-Process-0.7.2/CADETProcess/log.py`

 * *Files identical despite different names*

### Comparing `CADET-Process-0.7.1/CADETProcess/modelBuilder/__init__.py` & `CADET-Process-0.7.2/CADETProcess/modelBuilder/__init__.py`

 * *Files identical despite different names*

### Comparing `CADET-Process-0.7.1/CADETProcess/modelBuilder/carouselBuilder.py` & `CADET-Process-0.7.2/CADETProcess/modelBuilder/carouselBuilder.py`

 * *Files identical despite different names*

### Comparing `CADET-Process-0.7.1/CADETProcess/modelBuilder/compartmentBuilder.py` & `CADET-Process-0.7.2/CADETProcess/modelBuilder/compartmentBuilder.py`

 * *Files identical despite different names*

### Comparing `CADET-Process-0.7.1/CADETProcess/optimization/__init__.py` & `CADET-Process-0.7.2/CADETProcess/optimization/__init__.py`

 * *Files identical despite different names*

### Comparing `CADET-Process-0.7.1/CADETProcess/optimization/cache.py` & `CADET-Process-0.7.2/CADETProcess/optimization/cache.py`

 * *Files identical despite different names*

### Comparing `CADET-Process-0.7.1/CADETProcess/optimization/individual.py` & `CADET-Process-0.7.2/CADETProcess/optimization/individual.py`

 * *Files identical despite different names*

### Comparing `CADET-Process-0.7.1/CADETProcess/optimization/optimizationProblem.py` & `CADET-Process-0.7.2/CADETProcess/optimization/optimizationProblem.py`

 * *Files identical despite different names*

### Comparing `CADET-Process-0.7.1/CADETProcess/optimization/optimizer.py` & `CADET-Process-0.7.2/CADETProcess/optimization/optimizer.py`

 * *Files 2% similar despite different names*

```diff
@@ -64,15 +64,15 @@
     supports_nonlinear_constraints = False
 
     progress_frequency = RangedInteger(lb=1, default=1)
     n_cores = UnsignedInteger(default=1)
     cv_tol = UnsignedFloat(default=1e-6)
     similarity_tol = UnsignedFloat()
 
-    _options = ['progress_frequency', 'n_cores', 'cv_tol', 'similarity_tol']
+    _general_options = ['progress_frequency', 'n_cores', 'cv_tol', 'similarity_tol']
 
     def optimize(
             self,
             optimization_problem,
             x0=None,
             save_results=True,
             results_directory=None,
@@ -466,11 +466,22 @@
             if self.optimization_problem.n_meta_scores > 0:
                 message += f', m: {ind.m}'
             self.logger.info(message)
 
     @property
     def options(self):
         """dict: Optimizer options."""
-        return {opt: getattr(self, opt) for opt in self._options}
+        return {
+            opt: getattr(self, opt)
+            for opt in (self._general_options + self._specific_options)
+        }
+
+    @property
+    def specific_options(self):
+        """dict: Optimizer spcific options."""
+        return {
+            opt: getattr(self, opt)
+            for opt in (self._specific_options)
+        }
 
     def __str__(self):
         return self.__class__.__name__
```

### Comparing `CADET-Process-0.7.1/CADETProcess/optimization/population.py` & `CADET-Process-0.7.2/CADETProcess/optimization/population.py`

 * *Files identical despite different names*

### Comparing `CADET-Process-0.7.1/CADETProcess/optimization/pymooAdapter.py` & `CADET-Process-0.7.2/CADETProcess/optimization/pymooAdapter.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,15 +30,15 @@
     pop_size = UnsignedInteger()
     xtol = UnsignedFloat(default=1e-8)
     cvtol = UnsignedFloat(default=1e-6)
     cv_tol = cvtol
     ftol = UnsignedFloat(default=0.0025)
     n_max_gen = UnsignedInteger()
     n_max_evals = UnsignedInteger(default=100000)
-    _options = OptimizerBase._options + [
+    _specific_options = [
         'seed', 'pop_size', 'xtol', 'cvtol', 'ftol', 'n_max_gen', 'n_max_evals',
     ]
 
     def run(self, optimization_problem, x0=None):
         """Solve optimization problem using functional pymoo implementation.
 
         Parameters
```

### Comparing `CADET-Process-0.7.1/CADETProcess/optimization/results.py` & `CADET-Process-0.7.2/CADETProcess/optimization/results.py`

 * *Files identical despite different names*

### Comparing `CADET-Process-0.7.1/CADETProcess/optimization/scipyAdapter.py` & `CADET-Process-0.7.2/CADETProcess/optimization/scipyAdapter.py`

 * *Files 1% similar despite different names*

```diff
@@ -84,15 +84,16 @@
             scipy_results = optimize.minimize(
                 objective_function,
                 x0=x0,
                 method=str(self),
                 tol=self.tol,
                 jac=self.jac,
                 constraints=self.get_constraint_objects(optimization_problem),
-                options=self.options,
+                bounds=self.get_bounds(optimization_problem),
+                options=self.specific_options,
                 callback=callback_function,
             )
 
         self.results.exit_flag = scipy_results.status
         self.results.exit_message = scipy_results.message
 
     def get_bounds(self, optimization_problem):
@@ -276,15 +277,16 @@
     initial_tr_radius = UnsignedFloat(default=1.0)
     initial_barrier_parameter = UnsignedFloat(default=0.1)
     initial_barrier_tolerance = UnsignedFloat(default=0.1)
     factorization_method = None
     maxiter = UnsignedInteger(default=1000)
     verbose = UnsignedInteger(default=0)
     disp = Bool(default=False)
-    _options = OptimizerBase._options + [
+
+    _specific_options = [
         'gtol', 'xtol', 'barrier_tol', 'finite_diff_rel_step',
         'initial_constr_penalty',
         'initial_tr_radius', 'initial_barrier_parameter',
         'initial_barrier_tolerance', 'factorization_method',
         'maxiter', 'verbose', 'disp'
     ]
 
@@ -309,28 +311,29 @@
     supports_nonlinear_constraints = True
 
     rhobeg = UnsignedFloat(default=1)
     maxiter = UnsignedInteger(default=10000)
     disp = Bool(default=False)
     catol = UnsignedFloat(default=0.0002)
     cv_tol = catol
-    _options = OptimizerBase._options + ['rhobeg', 'maxiter', 'disp', 'catol']
+
+    _specific_options = ['rhobeg', 'maxiter', 'disp', 'catol']
 
 
 class NelderMead(SciPyInterface):
     """Class from scipy for optimization with NelderMead as method for the
     solver.
     """
     maxiter = UnsignedInteger()
     maxfev = UnsignedInteger()
     initial_simplex = None
     xatol = UnsignedFloat(default=0.01)
     fatol = UnsignedFloat(default=0.01)
     adaptive = Bool(default=True)
-    _options = OptimizerBase._options + [
+    _specific_options = [
         'maxiter', 'maxfev', 'initial_simplex', 'xatol', 'fatol', 'adaptive'
     ]
 
     def __str__(self):
         return 'Nelder-Mead'
 
 
@@ -346,8 +349,8 @@
     supports_linear_constraints = True
     supports_linear_equality_constraints = True
     supports_nonlinear_constraints = True
 
     ftol = UnsignedFloat(default=1e-2)
     eps = UnsignedFloat(default=1e-6)
     disp = Bool(default=False)
-    _options = OptimizerBase._options + ['ftol', 'eps', 'disp']
+    _specific_options = ['ftol', 'eps', 'disp']
```

### Comparing `CADET-Process-0.7.1/CADETProcess/performance.py` & `CADET-Process-0.7.2/CADETProcess/performance.py`

 * *Files identical despite different names*

### Comparing `CADET-Process-0.7.1/CADETProcess/plotting.py` & `CADET-Process-0.7.2/CADETProcess/plotting.py`

 * *Files identical despite different names*

### Comparing `CADET-Process-0.7.1/CADETProcess/processModel/__init__.py` & `CADET-Process-0.7.2/CADETProcess/processModel/__init__.py`

 * *Files identical despite different names*

### Comparing `CADET-Process-0.7.1/CADETProcess/processModel/binding.py` & `CADET-Process-0.7.2/CADETProcess/processModel/binding.py`

 * *Files identical despite different names*

### Comparing `CADET-Process-0.7.1/CADETProcess/processModel/componentSystem.py` & `CADET-Process-0.7.2/CADETProcess/processModel/componentSystem.py`

 * *Files identical despite different names*

### Comparing `CADET-Process-0.7.1/CADETProcess/processModel/discretization.py` & `CADET-Process-0.7.2/CADETProcess/processModel/discretization.py`

 * *Files identical despite different names*

### Comparing `CADET-Process-0.7.1/CADETProcess/processModel/flowSheet.py` & `CADET-Process-0.7.2/CADETProcess/processModel/flowSheet.py`

 * *Files identical despite different names*

### Comparing `CADET-Process-0.7.1/CADETProcess/processModel/process.py` & `CADET-Process-0.7.2/CADETProcess/processModel/process.py`

 * *Files identical despite different names*

### Comparing `CADET-Process-0.7.1/CADETProcess/processModel/reaction.py` & `CADET-Process-0.7.2/CADETProcess/processModel/reaction.py`

 * *Files identical despite different names*

### Comparing `CADET-Process-0.7.1/CADETProcess/processModel/solutionRecorder.py` & `CADET-Process-0.7.2/CADETProcess/processModel/solutionRecorder.py`

 * *Files identical despite different names*

### Comparing `CADET-Process-0.7.1/CADETProcess/processModel/unitOperation.py` & `CADET-Process-0.7.2/CADETProcess/processModel/unitOperation.py`

 * *Files identical despite different names*

### Comparing `CADET-Process-0.7.1/CADETProcess/reference.py` & `CADET-Process-0.7.2/CADETProcess/reference.py`

 * *Files identical despite different names*

### Comparing `CADET-Process-0.7.1/CADETProcess/settings.py` & `CADET-Process-0.7.2/CADETProcess/settings.py`

 * *Files identical despite different names*

### Comparing `CADET-Process-0.7.1/CADETProcess/simulationResults.py` & `CADET-Process-0.7.2/CADETProcess/simulationResults.py`

 * *Files identical despite different names*

### Comparing `CADET-Process-0.7.1/CADETProcess/simulator/__init__.py` & `CADET-Process-0.7.2/CADETProcess/simulator/__init__.py`

 * *Files identical despite different names*

### Comparing `CADET-Process-0.7.1/CADETProcess/simulator/cadetAdapter.py` & `CADET-Process-0.7.2/CADETProcess/simulator/cadetAdapter.py`

 * *Files identical despite different names*

### Comparing `CADET-Process-0.7.1/CADETProcess/simulator/simulator.py` & `CADET-Process-0.7.2/CADETProcess/simulator/simulator.py`

 * *Files identical despite different names*

### Comparing `CADET-Process-0.7.1/CADETProcess/smoothing.py` & `CADET-Process-0.7.2/CADETProcess/smoothing.py`

 * *Files identical despite different names*

### Comparing `CADET-Process-0.7.1/CADETProcess/smoothing2.py` & `CADET-Process-0.7.2/CADETProcess/smoothing2.py`

 * *Files identical despite different names*

### Comparing `CADET-Process-0.7.1/CADETProcess/solution.py` & `CADET-Process-0.7.2/CADETProcess/solution.py`

 * *Files identical despite different names*

### Comparing `CADET-Process-0.7.1/CADETProcess/stationarity.py` & `CADET-Process-0.7.2/CADETProcess/stationarity.py`

 * *Files identical despite different names*

### Comparing `CADET-Process-0.7.1/CADETProcess/tools/yamamoto.py` & `CADET-Process-0.7.2/CADETProcess/tools/yamamoto.py`

 * *Files identical despite different names*

### Comparing `CADET-Process-0.7.1/CADETProcess/transform.py` & `CADET-Process-0.7.2/CADETProcess/transform.py`

 * *Files identical despite different names*

### Comparing `CADET-Process-0.7.1/CADET_Process.egg-info/PKG-INFO` & `CADET-Process-0.7.2/CADET_Process.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CADET-Process
-Version: 0.7.1
+Version: 0.7.2
 Summary: A Framework for Modelling and Optimizing Advanced Chromatographic Processes
 Home-page: https://github.com/fau-advanced-separations/CADET-Process
 Author: Johannes Schmölder
 Author-email: j.schmoelder@fz-juelich.de
 Project-URL: Bug Tracker, https://github.com/fau-advanced-separations/CADET-Process/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `CADET-Process-0.7.1/CADET_Process.egg-info/SOURCES.txt` & `CADET-Process-0.7.2/CADET_Process.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `CADET-Process-0.7.1/LICENSE` & `CADET-Process-0.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `CADET-Process-0.7.1/PKG-INFO` & `CADET-Process-0.7.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CADET-Process
-Version: 0.7.1
+Version: 0.7.2
 Summary: A Framework for Modelling and Optimizing Advanced Chromatographic Processes
 Home-page: https://github.com/fau-advanced-separations/CADET-Process
 Author: Johannes Schmölder
 Author-email: j.schmoelder@fz-juelich.de
 Project-URL: Bug Tracker, https://github.com/fau-advanced-separations/CADET-Process/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `CADET-Process-0.7.1/README.md` & `CADET-Process-0.7.2/README.md`

 * *Files identical despite different names*

### Comparing `CADET-Process-0.7.1/examples/batch_elution/optimization_multi.py` & `CADET-Process-0.7.2/examples/batch_elution/optimization_multi.py`

 * *Files identical despite different names*

### Comparing `CADET-Process-0.7.1/examples/batch_elution/optimization_single.py` & `CADET-Process-0.7.2/examples/batch_elution/optimization_single.py`

 * *Files identical despite different names*

### Comparing `CADET-Process-0.7.1/examples/batch_elution/process.py` & `CADET-Process-0.7.2/examples/batch_elution/process.py`

 * *Files identical despite different names*

### Comparing `CADET-Process-0.7.1/examples/characterize_chromatographic_system/column_transport_parameters.py` & `CADET-Process-0.7.2/examples/characterize_chromatographic_system/column_transport_parameters.py`

 * *Files identical despite different names*

### Comparing `CADET-Process-0.7.1/examples/characterize_chromatographic_system/particle_porosity.py` & `CADET-Process-0.7.2/examples/characterize_chromatographic_system/particle_porosity.py`

 * *Files identical despite different names*

### Comparing `CADET-Process-0.7.1/examples/load_wash_elute/lwe_concentration.py` & `CADET-Process-0.7.2/examples/load_wash_elute/lwe_concentration.py`

 * *Files identical despite different names*

### Comparing `CADET-Process-0.7.1/examples/load_wash_elute/lwe_flow_rate.py` & `CADET-Process-0.7.2/examples/load_wash_elute/lwe_flow_rate.py`

 * *Files identical despite different names*

### Comparing `CADET-Process-0.7.1/examples/recycling/clr_process.py` & `CADET-Process-0.7.2/examples/recycling/clr_process.py`

 * *Files identical despite different names*

### Comparing `CADET-Process-0.7.1/examples/recycling/mrssr_process.py` & `CADET-Process-0.7.2/examples/recycling/mrssr_process.py`

 * *Files identical despite different names*

### Comparing `CADET-Process-0.7.1/setup.cfg` & `CADET-Process-0.7.2/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = CADET-Process
-version = 0.7.1
+version = 0.7.2
 author = Johannes Schmölder
 author_email = j.schmoelder@fz-juelich.de
 description = A Framework for Modelling and Optimizing Advanced Chromatographic Processes
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/fau-advanced-separations/CADET-Process
 project_urls =
```

### Comparing `CADET-Process-0.7.1/tests/test_binding.py` & `CADET-Process-0.7.2/tests/test_binding.py`

 * *Files identical despite different names*

### Comparing `CADET-Process-0.7.1/tests/test_buffer_capacity.py` & `CADET-Process-0.7.2/tests/test_buffer_capacity.py`

 * *Files identical despite different names*

### Comparing `CADET-Process-0.7.1/tests/test_cache.py` & `CADET-Process-0.7.2/tests/test_cache.py`

 * *Files identical despite different names*

### Comparing `CADET-Process-0.7.1/tests/test_carousel.py` & `CADET-Process-0.7.2/tests/test_carousel.py`

 * *Files identical despite different names*

### Comparing `CADET-Process-0.7.1/tests/test_compartment.py` & `CADET-Process-0.7.2/tests/test_compartment.py`

 * *Files identical despite different names*

### Comparing `CADET-Process-0.7.1/tests/test_components.py` & `CADET-Process-0.7.2/tests/test_components.py`

 * *Files identical despite different names*

### Comparing `CADET-Process-0.7.1/tests/test_difference.py` & `CADET-Process-0.7.2/tests/test_difference.py`

 * *Files identical despite different names*

### Comparing `CADET-Process-0.7.1/tests/test_equilibrium.py` & `CADET-Process-0.7.2/tests/test_equilibrium.py`

 * *Files identical despite different names*

### Comparing `CADET-Process-0.7.1/tests/test_events.py` & `CADET-Process-0.7.2/tests/test_events.py`

 * *Files identical despite different names*

### Comparing `CADET-Process-0.7.1/tests/test_flow_sheet.py` & `CADET-Process-0.7.2/tests/test_flow_sheet.py`

 * *Files identical despite different names*

### Comparing `CADET-Process-0.7.1/tests/test_fractions.py` & `CADET-Process-0.7.2/tests/test_fractions.py`

 * *Files identical despite different names*

### Comparing `CADET-Process-0.7.1/tests/test_individual.py` & `CADET-Process-0.7.2/tests/test_individual.py`

 * *Files identical despite different names*

### Comparing `CADET-Process-0.7.1/tests/test_optimization_integration.py` & `CADET-Process-0.7.2/tests/test_optimization_integration.py`

 * *Files identical despite different names*

### Comparing `CADET-Process-0.7.1/tests/test_optimization_problem.py` & `CADET-Process-0.7.2/tests/test_optimization_problem.py`

 * *Files identical despite different names*

### Comparing `CADET-Process-0.7.1/tests/test_optimization_results.py` & `CADET-Process-0.7.2/tests/test_optimization_results.py`

 * *Files identical despite different names*

### Comparing `CADET-Process-0.7.1/tests/test_parameters.py` & `CADET-Process-0.7.2/tests/test_parameters.py`

 * *Files identical despite different names*

### Comparing `CADET-Process-0.7.1/tests/test_population.py` & `CADET-Process-0.7.2/tests/test_population.py`

 * *Files identical despite different names*

### Comparing `CADET-Process-0.7.1/tests/test_reaction.py` & `CADET-Process-0.7.2/tests/test_reaction.py`

 * *Files identical despite different names*

### Comparing `CADET-Process-0.7.1/tests/test_sections.py` & `CADET-Process-0.7.2/tests/test_sections.py`

 * *Files identical despite different names*

### Comparing `CADET-Process-0.7.1/tests/test_solution.py` & `CADET-Process-0.7.2/tests/test_solution.py`

 * *Files identical despite different names*

### Comparing `CADET-Process-0.7.1/tests/test_transform.py` & `CADET-Process-0.7.2/tests/test_transform.py`

 * *Files identical despite different names*

### Comparing `CADET-Process-0.7.1/tests/test_unit_operation.py` & `CADET-Process-0.7.2/tests/test_unit_operation.py`

 * *Files identical despite different names*

