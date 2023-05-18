# Comparing `tmp/mentpy-0.1.0a4.tar.gz` & `tmp/mentpy-0.1.0a5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mentpy-0.1.0a4.tar", last modified: Fri Apr 28 10:01:58 2023, max compression
+gzip compressed data, was "mentpy-0.1.0a5.tar", last modified: Thu May 18 06:26:13 2023, max compression
```

## Comparing `mentpy-0.1.0a4.tar` & `mentpy-0.1.0a5.tar`

### file list

```diff
@@ -1,64 +1,64 @@
-drwxr-xr-x   0 luismantilla   (501) staff       (20)        0 2023-04-28 10:01:58.053017 mentpy-0.1.0a4/
--rw-r--r--   0 luismantilla   (501) staff       (20)    35149 2023-03-17 11:11:29.000000 mentpy-0.1.0a4/LICENSE
--rw-r--r--   0 luismantilla   (501) staff       (20)     3373 2023-04-28 10:01:58.052776 mentpy-0.1.0a4/PKG-INFO
--rw-r--r--   0 luismantilla   (501) staff       (20)     3093 2023-04-08 10:02:59.000000 mentpy-0.1.0a4/README.md
-drwxr-xr-x   0 luismantilla   (501) staff       (20)        0 2023-04-28 10:01:58.035236 mentpy-0.1.0a4/mentpy/
--rw-r--r--   0 luismantilla   (501) staff       (20)      283 2023-04-16 02:10:35.000000 mentpy-0.1.0a4/mentpy/__init__.py
-drwxr-xr-x   0 luismantilla   (501) staff       (20)        0 2023-04-28 10:01:58.037449 mentpy-0.1.0a4/mentpy/gradients/
--rw-r--r--   0 luismantilla   (501) staff       (20)       33 2023-03-17 21:21:26.000000 mentpy-0.1.0a4/mentpy/gradients/__init__.py
--rw-r--r--   0 luismantilla   (501) staff       (20)     2014 2023-04-25 08:57:09.000000 mentpy-0.1.0a4/mentpy/gradients/finite_difference.py
-drwxr-xr-x   0 luismantilla   (501) staff       (20)        0 2023-04-28 10:01:58.038659 mentpy-0.1.0a4/mentpy/mbqc/
--rw-r--r--   0 luismantilla   (501) staff       (20)      343 2023-04-16 02:07:08.000000 mentpy-0.1.0a4/mentpy/mbqc/__init__.py
--rw-r--r--   0 luismantilla   (501) staff       (20)    16348 2023-04-16 05:41:03.000000 mentpy-0.1.0a4/mentpy/mbqc/flow.py
--rw-r--r--   0 luismantilla   (501) staff       (20)    25586 2023-04-28 04:28:02.000000 mentpy-0.1.0a4/mentpy/mbqc/mbqcircuit.py
-drwxr-xr-x   0 luismantilla   (501) staff       (20)        0 2023-04-28 10:01:58.039278 mentpy-0.1.0a4/mentpy/mbqc/states/
--rw-r--r--   0 luismantilla   (501) staff       (20)      149 2023-04-16 02:07:17.000000 mentpy-0.1.0a4/mentpy/mbqc/states/__init__.py
--rw-r--r--   0 luismantilla   (501) staff       (20)      163 2023-04-15 11:17:22.000000 mentpy-0.1.0a4/mentpy/mbqc/states/aklt.py
--rw-r--r--   0 luismantilla   (501) staff       (20)      195 2023-04-15 11:17:22.000000 mentpy-0.1.0a4/mentpy/mbqc/states/cluster.py
--rw-r--r--   0 luismantilla   (501) staff       (20)     2976 2023-04-16 05:41:03.000000 mentpy-0.1.0a4/mentpy/mbqc/states/graphstate.py
--rw-r--r--   0 luismantilla   (501) staff       (20)     7358 2023-04-25 08:57:09.000000 mentpy-0.1.0a4/mentpy/mbqc/templates.py
-drwxr-xr-x   0 luismantilla   (501) staff       (20)        0 2023-04-28 10:01:58.039866 mentpy-0.1.0a4/mentpy/noise/
--rw-r--r--   0 luismantilla   (501) staff       (20)       34 2023-03-17 21:21:26.000000 mentpy-0.1.0a4/mentpy/noise/__init__.py
--rw-r--r--   0 luismantilla   (501) staff       (20)      173 2023-03-17 21:21:26.000000 mentpy-0.1.0a4/mentpy/noise/base_noise.py
-drwxr-xr-x   0 luismantilla   (501) staff       (20)        0 2023-04-28 10:01:58.041726 mentpy-0.1.0a4/mentpy/operators/
--rw-r--r--   0 luismantilla   (501) staff       (20)      236 2023-04-21 07:24:47.000000 mentpy-0.1.0a4/mentpy/operators/__init__.py
--rw-r--r--   0 luismantilla   (501) staff       (20)     2822 2023-04-21 09:50:33.000000 mentpy-0.1.0a4/mentpy/operators/controlled_ment.py
--rw-r--r--   0 luismantilla   (501) staff       (20)     1567 2023-04-16 01:27:43.000000 mentpy-0.1.0a4/mentpy/operators/gates.py
--rw-r--r--   0 luismantilla   (501) staff       (20)     7820 2023-04-21 10:14:40.000000 mentpy-0.1.0a4/mentpy/operators/ment.py
--rw-r--r--   0 luismantilla   (501) staff       (20)     5392 2023-04-28 08:07:49.000000 mentpy-0.1.0a4/mentpy/operators/pauliop.py
-drwxr-xr-x   0 luismantilla   (501) staff       (20)        0 2023-04-28 10:01:58.045479 mentpy-0.1.0a4/mentpy/optimizers/
--rw-r--r--   0 luismantilla   (501) staff       (20)      245 2023-04-25 08:17:14.000000 mentpy-0.1.0a4/mentpy/optimizers/__init__.py
--rw-r--r--   0 luismantilla   (501) staff       (20)     3054 2023-03-22 20:56:41.000000 mentpy-0.1.0a4/mentpy/optimizers/adam.py
--rw-r--r--   0 luismantilla   (501) staff       (20)      632 2023-03-17 21:21:26.000000 mentpy-0.1.0a4/mentpy/optimizers/base_optimizer.py
--rw-r--r--   0 luismantilla   (501) staff       (20)      379 2023-03-17 21:21:26.000000 mentpy-0.1.0a4/mentpy/optimizers/bp_tools.py
--rw-r--r--   0 luismantilla   (501) staff       (20)     3101 2023-04-25 09:08:43.000000 mentpy-0.1.0a4/mentpy/optimizers/rcd.py
--rw-r--r--   0 luismantilla   (501) staff       (20)     2637 2023-04-15 23:00:30.000000 mentpy-0.1.0a4/mentpy/optimizers/sgd.py
-drwxr-xr-x   0 luismantilla   (501) staff       (20)        0 2023-04-28 10:01:58.047979 mentpy-0.1.0a4/mentpy/simulators/
--rw-r--r--   0 luismantilla   (501) staff       (20)      281 2023-04-16 02:18:15.000000 mentpy-0.1.0a4/mentpy/simulators/__init__.py
--rw-r--r--   0 luismantilla   (501) staff       (20)     2143 2023-04-18 08:22:14.000000 mentpy-0.1.0a4/mentpy/simulators/base_simulator.py
--rw-r--r--   0 luismantilla   (501) staff       (20)     1156 2023-04-18 08:22:14.000000 mentpy-0.1.0a4/mentpy/simulators/cirq_simulator.py
--rw-r--r--   0 luismantilla   (501) staff       (20)    13039 2023-04-25 08:57:09.000000 mentpy-0.1.0a4/mentpy/simulators/np_simulator_dm.py
--rw-r--r--   0 luismantilla   (501) staff       (20)    14384 2023-04-25 08:57:09.000000 mentpy-0.1.0a4/mentpy/simulators/np_simulator_sv.py
--rw-r--r--   0 luismantilla   (501) staff       (20)     2688 2023-04-28 03:47:29.000000 mentpy-0.1.0a4/mentpy/simulators/pattern_simulator.py
--rw-r--r--   0 luismantilla   (501) staff       (20)     5853 2023-04-25 08:57:09.000000 mentpy-0.1.0a4/mentpy/simulators/pennylane_simulator.py
--rw-r--r--   0 luismantilla   (501) staff       (20)     1254 2023-04-25 08:57:09.000000 mentpy-0.1.0a4/mentpy/simulators/qiskit_simulators.py
-drwxr-xr-x   0 luismantilla   (501) staff       (20)        0 2023-04-28 10:01:58.048967 mentpy-0.1.0a4/mentpy/utils/
--rw-r--r--   0 luismantilla   (501) staff       (20)      140 2023-04-16 02:10:19.000000 mentpy-0.1.0a4/mentpy/utils/__init__.py
--rw-r--r--   0 luismantilla   (501) staff       (20)     6673 2023-04-25 08:57:09.000000 mentpy-0.1.0a4/mentpy/utils/expressivity.py
--rw-r--r--   0 luismantilla   (501) staff       (20)     3183 2023-04-16 01:51:56.000000 mentpy-0.1.0a4/mentpy/utils/flow_space.py
--rw-r--r--   0 luismantilla   (501) staff       (20)     4466 2023-04-16 01:44:39.000000 mentpy-0.1.0a4/mentpy/utils/generate_data.py
--rw-r--r--   0 luismantilla   (501) staff       (20)    10395 2023-03-17 21:21:26.000000 mentpy-0.1.0a4/mentpy/utils/lc_equivalence.py
--rw-r--r--   0 luismantilla   (501) staff       (20)     5172 2023-04-28 08:24:36.000000 mentpy-0.1.0a4/mentpy/utils/lie_algebra.py
-drwxr-xr-x   0 luismantilla   (501) staff       (20)        0 2023-04-28 10:01:58.036184 mentpy-0.1.0a4/mentpy.egg-info/
--rw-r--r--   0 luismantilla   (501) staff       (20)     3373 2023-04-28 10:01:57.000000 mentpy-0.1.0a4/mentpy.egg-info/PKG-INFO
--rw-r--r--   0 luismantilla   (501) staff       (20)     1409 2023-04-28 10:01:58.000000 mentpy-0.1.0a4/mentpy.egg-info/SOURCES.txt
--rw-r--r--   0 luismantilla   (501) staff       (20)        1 2023-04-28 10:01:57.000000 mentpy-0.1.0a4/mentpy.egg-info/dependency_links.txt
--rw-r--r--   0 luismantilla   (501) staff       (20)       49 2023-04-28 10:01:57.000000 mentpy-0.1.0a4/mentpy.egg-info/requires.txt
--rw-r--r--   0 luismantilla   (501) staff       (20)        7 2023-04-28 10:01:57.000000 mentpy-0.1.0a4/mentpy.egg-info/top_level.txt
--rw-r--r--   0 luismantilla   (501) staff       (20)       38 2023-04-28 10:01:58.053091 mentpy-0.1.0a4/setup.cfg
--rw-r--r--   0 luismantilla   (501) staff       (20)      553 2023-04-28 10:00:53.000000 mentpy-0.1.0a4/setup.py
-drwxr-xr-x   0 luismantilla   (501) staff       (20)        0 2023-04-28 10:01:58.051991 mentpy-0.1.0a4/tests/
--rw-r--r--   0 luismantilla   (501) staff       (20)       58 2023-04-16 01:51:49.000000 mentpy-0.1.0a4/tests/test_flow.py
--rw-r--r--   0 luismantilla   (501) staff       (20)       64 2023-04-16 01:52:08.000000 mentpy-0.1.0a4/tests/test_graph_state.py
--rw-r--r--   0 luismantilla   (501) staff       (20)      579 2023-04-16 01:52:23.000000 mentpy-0.1.0a4/tests/test_mbqc_templates.py
--rw-r--r--   0 luismantilla   (501) staff       (20)      997 2023-04-28 03:46:02.000000 mentpy-0.1.0a4/tests/test_simulators.py
+drwxr-xr-x   0 luismantilla   (501) staff       (20)        0 2023-05-18 06:26:13.495349 mentpy-0.1.0a5/
+-rw-r--r--   0 luismantilla   (501) staff       (20)    35149 2023-03-17 11:11:29.000000 mentpy-0.1.0a5/LICENSE
+-rw-r--r--   0 luismantilla   (501) staff       (20)     3336 2023-05-18 06:26:13.495146 mentpy-0.1.0a5/PKG-INFO
+-rw-r--r--   0 luismantilla   (501) staff       (20)     3056 2023-05-08 04:08:41.000000 mentpy-0.1.0a5/README.md
+drwxr-xr-x   0 luismantilla   (501) staff       (20)        0 2023-05-18 06:26:13.475785 mentpy-0.1.0a5/mentpy/
+-rw-r--r--   0 luismantilla   (501) staff       (20)      283 2023-04-16 02:10:35.000000 mentpy-0.1.0a5/mentpy/__init__.py
+drwxr-xr-x   0 luismantilla   (501) staff       (20)        0 2023-05-18 06:26:13.477204 mentpy-0.1.0a5/mentpy/gradients/
+-rw-r--r--   0 luismantilla   (501) staff       (20)       33 2023-03-17 21:21:26.000000 mentpy-0.1.0a5/mentpy/gradients/__init__.py
+-rw-r--r--   0 luismantilla   (501) staff       (20)     2014 2023-04-25 08:57:09.000000 mentpy-0.1.0a5/mentpy/gradients/finite_difference.py
+drwxr-xr-x   0 luismantilla   (501) staff       (20)        0 2023-05-18 06:26:13.478932 mentpy-0.1.0a5/mentpy/mbqc/
+-rw-r--r--   0 luismantilla   (501) staff       (20)      343 2023-04-16 02:07:08.000000 mentpy-0.1.0a5/mentpy/mbqc/__init__.py
+-rw-r--r--   0 luismantilla   (501) staff       (20)    17441 2023-05-16 19:16:57.000000 mentpy-0.1.0a5/mentpy/mbqc/flow.py
+-rw-r--r--   0 luismantilla   (501) staff       (20)    30925 2023-05-17 16:21:24.000000 mentpy-0.1.0a5/mentpy/mbqc/mbqcircuit.py
+drwxr-xr-x   0 luismantilla   (501) staff       (20)        0 2023-05-18 06:26:13.480419 mentpy-0.1.0a5/mentpy/mbqc/states/
+-rw-r--r--   0 luismantilla   (501) staff       (20)      149 2023-05-06 07:23:30.000000 mentpy-0.1.0a5/mentpy/mbqc/states/__init__.py
+-rw-r--r--   0 luismantilla   (501) staff       (20)      197 2023-05-06 07:23:09.000000 mentpy-0.1.0a5/mentpy/mbqc/states/aklt.py
+-rw-r--r--   0 luismantilla   (501) staff       (20)      229 2023-05-06 07:23:14.000000 mentpy-0.1.0a5/mentpy/mbqc/states/cluster.py
+-rw-r--r--   0 luismantilla   (501) staff       (20)     2976 2023-04-16 05:41:03.000000 mentpy-0.1.0a5/mentpy/mbqc/states/graphstate.py
+-rw-r--r--   0 luismantilla   (501) staff       (20)     7594 2023-05-18 06:03:44.000000 mentpy-0.1.0a5/mentpy/mbqc/templates.py
+drwxr-xr-x   0 luismantilla   (501) staff       (20)        0 2023-05-18 06:26:13.481028 mentpy-0.1.0a5/mentpy/noise/
+-rw-r--r--   0 luismantilla   (501) staff       (20)       34 2023-03-17 21:21:26.000000 mentpy-0.1.0a5/mentpy/noise/__init__.py
+-rw-r--r--   0 luismantilla   (501) staff       (20)      173 2023-03-17 21:21:26.000000 mentpy-0.1.0a5/mentpy/noise/base_noise.py
+drwxr-xr-x   0 luismantilla   (501) staff       (20)        0 2023-05-18 06:26:13.482583 mentpy-0.1.0a5/mentpy/operators/
+-rw-r--r--   0 luismantilla   (501) staff       (20)      285 2023-05-10 00:16:14.000000 mentpy-0.1.0a5/mentpy/operators/__init__.py
+-rw-r--r--   0 luismantilla   (501) staff       (20)     3164 2023-05-10 00:16:14.000000 mentpy-0.1.0a5/mentpy/operators/controlled_ment.py
+-rw-r--r--   0 luismantilla   (501) staff       (20)     1599 2023-05-07 19:04:31.000000 mentpy-0.1.0a5/mentpy/operators/gates.py
+-rw-r--r--   0 luismantilla   (501) staff       (20)     8139 2023-05-16 20:00:06.000000 mentpy-0.1.0a5/mentpy/operators/ment.py
+-rw-r--r--   0 luismantilla   (501) staff       (20)     5502 2023-05-18 06:12:52.000000 mentpy-0.1.0a5/mentpy/operators/pauliop.py
+drwxr-xr-x   0 luismantilla   (501) staff       (20)        0 2023-05-18 06:26:13.484243 mentpy-0.1.0a5/mentpy/optimizers/
+-rw-r--r--   0 luismantilla   (501) staff       (20)      245 2023-04-25 08:17:14.000000 mentpy-0.1.0a5/mentpy/optimizers/__init__.py
+-rw-r--r--   0 luismantilla   (501) staff       (20)     3054 2023-03-22 20:56:41.000000 mentpy-0.1.0a5/mentpy/optimizers/adam.py
+-rw-r--r--   0 luismantilla   (501) staff       (20)      632 2023-03-17 21:21:26.000000 mentpy-0.1.0a5/mentpy/optimizers/base_optimizer.py
+-rw-r--r--   0 luismantilla   (501) staff       (20)      379 2023-03-17 21:21:26.000000 mentpy-0.1.0a5/mentpy/optimizers/bp_tools.py
+-rw-r--r--   0 luismantilla   (501) staff       (20)     3101 2023-04-25 09:08:43.000000 mentpy-0.1.0a5/mentpy/optimizers/rcd.py
+-rw-r--r--   0 luismantilla   (501) staff       (20)     2637 2023-04-15 23:00:30.000000 mentpy-0.1.0a5/mentpy/optimizers/sgd.py
+drwxr-xr-x   0 luismantilla   (501) staff       (20)        0 2023-05-18 06:26:13.487662 mentpy-0.1.0a5/mentpy/simulators/
+-rw-r--r--   0 luismantilla   (501) staff       (20)      281 2023-04-16 02:18:15.000000 mentpy-0.1.0a5/mentpy/simulators/__init__.py
+-rw-r--r--   0 luismantilla   (501) staff       (20)     2441 2023-05-07 19:04:31.000000 mentpy-0.1.0a5/mentpy/simulators/base_simulator.py
+-rw-r--r--   0 luismantilla   (501) staff       (20)     1156 2023-04-18 08:22:14.000000 mentpy-0.1.0a5/mentpy/simulators/cirq_simulator.py
+-rw-r--r--   0 luismantilla   (501) staff       (20)    15302 2023-05-10 23:53:23.000000 mentpy-0.1.0a5/mentpy/simulators/np_simulator_dm.py
+-rw-r--r--   0 luismantilla   (501) staff       (20)    15668 2023-05-10 00:49:41.000000 mentpy-0.1.0a5/mentpy/simulators/np_simulator_sv.py
+-rw-r--r--   0 luismantilla   (501) staff       (20)     2680 2023-05-07 19:04:31.000000 mentpy-0.1.0a5/mentpy/simulators/pattern_simulator.py
+-rw-r--r--   0 luismantilla   (501) staff       (20)     5576 2023-05-16 19:33:50.000000 mentpy-0.1.0a5/mentpy/simulators/pennylane_simulator.py
+-rw-r--r--   0 luismantilla   (501) staff       (20)     1254 2023-04-25 08:57:09.000000 mentpy-0.1.0a5/mentpy/simulators/qiskit_simulators.py
+drwxr-xr-x   0 luismantilla   (501) staff       (20)        0 2023-05-18 06:26:13.491265 mentpy-0.1.0a5/mentpy/utils/
+-rw-r--r--   0 luismantilla   (501) staff       (20)      140 2023-04-16 02:10:19.000000 mentpy-0.1.0a5/mentpy/utils/__init__.py
+-rw-r--r--   0 luismantilla   (501) staff       (20)     6673 2023-04-25 08:57:09.000000 mentpy-0.1.0a5/mentpy/utils/expressivity.py
+-rw-r--r--   0 luismantilla   (501) staff       (20)     3183 2023-04-16 01:51:56.000000 mentpy-0.1.0a5/mentpy/utils/flow_space.py
+-rw-r--r--   0 luismantilla   (501) staff       (20)     4466 2023-04-16 01:44:39.000000 mentpy-0.1.0a5/mentpy/utils/generate_data.py
+-rw-r--r--   0 luismantilla   (501) staff       (20)    10395 2023-05-06 07:13:49.000000 mentpy-0.1.0a5/mentpy/utils/lc_equivalence.py
+-rw-r--r--   0 luismantilla   (501) staff       (20)     6584 2023-05-18 06:20:35.000000 mentpy-0.1.0a5/mentpy/utils/lie_algebra.py
+drwxr-xr-x   0 luismantilla   (501) staff       (20)        0 2023-05-18 06:26:13.476710 mentpy-0.1.0a5/mentpy.egg-info/
+-rw-r--r--   0 luismantilla   (501) staff       (20)     3336 2023-05-18 06:26:13.000000 mentpy-0.1.0a5/mentpy.egg-info/PKG-INFO
+-rw-r--r--   0 luismantilla   (501) staff       (20)     1409 2023-05-18 06:26:13.000000 mentpy-0.1.0a5/mentpy.egg-info/SOURCES.txt
+-rw-r--r--   0 luismantilla   (501) staff       (20)        1 2023-05-18 06:26:13.000000 mentpy-0.1.0a5/mentpy.egg-info/dependency_links.txt
+-rw-r--r--   0 luismantilla   (501) staff       (20)       49 2023-05-18 06:26:13.000000 mentpy-0.1.0a5/mentpy.egg-info/requires.txt
+-rw-r--r--   0 luismantilla   (501) staff       (20)        7 2023-05-18 06:26:13.000000 mentpy-0.1.0a5/mentpy.egg-info/top_level.txt
+-rw-r--r--   0 luismantilla   (501) staff       (20)       38 2023-05-18 06:26:13.495412 mentpy-0.1.0a5/setup.cfg
+-rw-r--r--   0 luismantilla   (501) staff       (20)      553 2023-05-18 06:18:20.000000 mentpy-0.1.0a5/setup.py
+drwxr-xr-x   0 luismantilla   (501) staff       (20)        0 2023-05-18 06:26:13.494600 mentpy-0.1.0a5/tests/
+-rw-r--r--   0 luismantilla   (501) staff       (20)       58 2023-04-16 01:51:49.000000 mentpy-0.1.0a5/tests/test_flow.py
+-rw-r--r--   0 luismantilla   (501) staff       (20)       64 2023-04-16 01:52:08.000000 mentpy-0.1.0a5/tests/test_graph_state.py
+-rw-r--r--   0 luismantilla   (501) staff       (20)      579 2023-04-16 01:52:23.000000 mentpy-0.1.0a5/tests/test_mbqc_templates.py
+-rw-r--r--   0 luismantilla   (501) staff       (20)     2110 2023-05-18 06:15:48.000000 mentpy-0.1.0a5/tests/test_simulators.py
```

### Comparing `mentpy-0.1.0a4/LICENSE` & `mentpy-0.1.0a5/LICENSE`

 * *Files identical despite different names*

### Comparing `mentpy-0.1.0a4/PKG-INFO` & `mentpy-0.1.0a5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,17 @@
 Metadata-Version: 2.1
 Name: mentpy
-Version: 0.1.0a4
+Version: 0.1.0a5
 Summary: A Python library for simulating MBQC circuits
 Home-page: https://github.com/BestQuark/mentpy
 Author: Luis Mantilla
 Author-email: luismantilla99@outlook.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-:warning: **This library is under development.**
-
 <p align="center">
   <img src="./docs/_static/logo.png" alt="MentPy: A Measurement-Based Quantum computing simulator." width="70%">
 </p>
 
 <div align=center>
   <a href="https://pypi.org/project/mentpy"><img src="https://img.shields.io/pypi/v/mentpy"></a>
   <!-- <a href="https://pypi.org/project/mentpy"><img src="https://img.shields.io/pypi/pyversions/mentpy"></a> -->
@@ -28,16 +26,15 @@
   <a href="https://github.com/bestquark/mentpy/actions/workflows/lint.yaml"><img src="https://github.com/bestquark/mentpy/actions/workflows/lint.yaml/badge.svg"></a>
   <a href="https://github.com/bestquark/mentpy/actions/workflows/build.yaml"><img src="https://github.com/bestquark/mentpy/actions/workflows/build.yaml/badge.svg"></a>
   <a href="https://github.com/bestquark/mentpy/actions/workflows/test.yaml"><img src="https://github.com/bestquark/mentpy/actions/workflows/test.yaml/badge.svg"></a>
   <a href="https://codecov.io/gh/bestquark/mentpy"><img src="https://codecov.io/gh/bestquark/mentpy/branch/master/graph/badge.svg?token=3FJML79ZUK"></a> -->
 </div>
 
 The `MentPy` library is an open-source software for simulations of 
-measurement-based quantum computing circuits. Currently, this package is under 
-development and is not ready for public use.
+measurement-based quantum computing circuits. Currently, this package is in its alpha version and many features are still in development.
 
 ## Installation
 
 The `MentPy` library can be installed using `pip` with
 
 ```bash
 pip install mentpy
```

#### html2text {}

```diff
@@ -1,24 +1,23 @@
-Metadata-Version: 2.1 Name: mentpy Version: 0.1.0a4 Summary: A Python library
+Metadata-Version: 2.1 Name: mentpy Version: 0.1.0a5 Summary: A Python library
 for simulating MBQC circuits Home-page: https://github.com/BestQuark/mentpy
 Author: Luis Mantilla Author-email: luismantilla99@outlook.com Description-
-Content-Type: text/markdown License-File: LICENSE :warning: **This library is
-under development.**
+Content-Type: text/markdown License-File: LICENSE
           [MentPy: A Measurement-Based Quantum computing simulator.]
   [https://img.shields.io/pypi/v/mentpy]  [https://img.shields.io/pypi/wheel/
     mentpy] [Documentation_Status]  [https://img.shields.io/twitter/follow/
                  mentpy?label=mentpy&style=flat&logo=twitter]
 The `MentPy` library is an open-source software for simulations of measurement-
-based quantum computing circuits. Currently, this package is under development
-and is not ready for public use. ## Installation The `MentPy` library can be
-installed using `pip` with ```bash pip install mentpy ``` or directly from the
-source code for the latest version with ```bash pip install git+https://
-github.com/BestQuark/mentpy.git ``` ## Usage To simulate a measurement pattern,
-you can use the `mp.PatternSimulator`. ```python import mentpy as mp st =
-mp.templates.grid_cluster(2,4) ps = mp.PatternSimulator(st) output = ps
-(np.random.rand(len(st.outputc))) ``` For visualization of circuits, you can
-use the `mp.draw(st)` function ![image](https://user-
+based quantum computing circuits. Currently, this package is in its alpha
+version and many features are still in development. ## Installation The
+`MentPy` library can be installed using `pip` with ```bash pip install mentpy
+``` or directly from the source code for the latest version with ```bash pip
+install git+https://github.com/BestQuark/mentpy.git ``` ## Usage To simulate a
+measurement pattern, you can use the `mp.PatternSimulator`. ```python import
+mentpy as mp st = mp.templates.grid_cluster(2,4) ps = mp.PatternSimulator(st)
+output = ps(np.random.rand(len(st.outputc))) ``` For visualization of circuits,
+you can use the `mp.draw(st)` function ![image](https://user-
 images.githubusercontent.com/52287586/230715389-bf280971-c841-437d-8772-
 bf59557b0875.png) ## Documentation The documentation for `MentPy` can be found
 here. ## Contributing We welcome contributions to `MentPy`! Please see our
 [contributing guidelines](./CONTRIBUTING.md) for more information. ## License
 `MentPy` is licensed under the [GNU General Public License v3.0](./LICENSE).
```

### Comparing `mentpy-0.1.0a4/README.md` & `mentpy-0.1.0a5/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-:warning: **This library is under development.**
-
 <p align="center">
   <img src="./docs/_static/logo.png" alt="MentPy: A Measurement-Based Quantum computing simulator." width="70%">
 </p>
 
 <div align=center>
   <a href="https://pypi.org/project/mentpy"><img src="https://img.shields.io/pypi/v/mentpy"></a>
   <!-- <a href="https://pypi.org/project/mentpy"><img src="https://img.shields.io/pypi/pyversions/mentpy"></a> -->
@@ -18,16 +16,15 @@
   <a href="https://github.com/bestquark/mentpy/actions/workflows/lint.yaml"><img src="https://github.com/bestquark/mentpy/actions/workflows/lint.yaml/badge.svg"></a>
   <a href="https://github.com/bestquark/mentpy/actions/workflows/build.yaml"><img src="https://github.com/bestquark/mentpy/actions/workflows/build.yaml/badge.svg"></a>
   <a href="https://github.com/bestquark/mentpy/actions/workflows/test.yaml"><img src="https://github.com/bestquark/mentpy/actions/workflows/test.yaml/badge.svg"></a>
   <a href="https://codecov.io/gh/bestquark/mentpy"><img src="https://codecov.io/gh/bestquark/mentpy/branch/master/graph/badge.svg?token=3FJML79ZUK"></a> -->
 </div>
 
 The `MentPy` library is an open-source software for simulations of 
-measurement-based quantum computing circuits. Currently, this package is under 
-development and is not ready for public use.
+measurement-based quantum computing circuits. Currently, this package is in its alpha version and many features are still in development.
 
 ## Installation
 
 The `MentPy` library can be installed using `pip` with
 
 ```bash
 pip install mentpy
```

#### html2text {}

```diff
@@ -1,20 +1,19 @@
-:warning: **This library is under development.**
           [MentPy: A Measurement-Based Quantum computing simulator.]
   [https://img.shields.io/pypi/v/mentpy]  [https://img.shields.io/pypi/wheel/
     mentpy] [Documentation_Status]  [https://img.shields.io/twitter/follow/
                  mentpy?label=mentpy&style=flat&logo=twitter]
 The `MentPy` library is an open-source software for simulations of measurement-
-based quantum computing circuits. Currently, this package is under development
-and is not ready for public use. ## Installation The `MentPy` library can be
-installed using `pip` with ```bash pip install mentpy ``` or directly from the
-source code for the latest version with ```bash pip install git+https://
-github.com/BestQuark/mentpy.git ``` ## Usage To simulate a measurement pattern,
-you can use the `mp.PatternSimulator`. ```python import mentpy as mp st =
-mp.templates.grid_cluster(2,4) ps = mp.PatternSimulator(st) output = ps
-(np.random.rand(len(st.outputc))) ``` For visualization of circuits, you can
-use the `mp.draw(st)` function ![image](https://user-
+based quantum computing circuits. Currently, this package is in its alpha
+version and many features are still in development. ## Installation The
+`MentPy` library can be installed using `pip` with ```bash pip install mentpy
+``` or directly from the source code for the latest version with ```bash pip
+install git+https://github.com/BestQuark/mentpy.git ``` ## Usage To simulate a
+measurement pattern, you can use the `mp.PatternSimulator`. ```python import
+mentpy as mp st = mp.templates.grid_cluster(2,4) ps = mp.PatternSimulator(st)
+output = ps(np.random.rand(len(st.outputc))) ``` For visualization of circuits,
+you can use the `mp.draw(st)` function ![image](https://user-
 images.githubusercontent.com/52287586/230715389-bf280971-c841-437d-8772-
 bf59557b0875.png) ## Documentation The documentation for `MentPy` can be found
 here. ## Contributing We welcome contributions to `MentPy`! Please see our
 [contributing guidelines](./CONTRIBUTING.md) for more information. ## License
 `MentPy` is licensed under the [GNU General Public License v3.0](./LICENSE).
```

### Comparing `mentpy-0.1.0a4/mentpy/gradients/finite_difference.py` & `mentpy-0.1.0a5/mentpy/gradients/finite_difference.py`

 * *Files identical despite different names*

### Comparing `mentpy-0.1.0a4/mentpy/mbqc/flow.py` & `mentpy-0.1.0a5/mentpy/mbqc/flow.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,14 +9,34 @@
 from typing import List
 import warnings
 
 import galois
 
 ## Not used in main MBQC module
 
+# This module should only export the flow class
+
+
+class Flow:
+    def __init__(self, graph: GraphState, input_nodes, output_nodes):
+        self.graph = graph
+        self.input_nodes = input_nodes
+        self.output_nodes = output_nodes
+        flow_function, partial_order = self.find_flow()
+        self.func = flow_function
+        self.partial_order = partial_order
+        self.depth = -1  # calculate depth
+
+    def find_flow(self):
+        # include gflow and pflow
+        return find_flow(self.graph, self.input_nodes, self.output_nodes)
+
+    def adapt_angles(self, angles, outcomes):
+        raise NotImplementedError
+
 
 def find_flow(graph: GraphState, input_nodes, output_nodes, sanity_check=True):
     r"""Finds the generalized flow of graph state if allowed.
 
     Implementation of https://arxiv.org/pdf/quant-ph/0603072.pdf.
 
     Returns
@@ -24,19 +44,19 @@
     The flow function ``flow`` and the partial order function.
 
     Group
     -----
     states
     """
     # raise deprecated warning
-    warnings.warn(
-        "The function find_flow is deprecated. Use find_cflow instead.",
-        DeprecationWarning,
-        stacklevel=2,
-    )
+    # warnings.warn(
+    #     "The function find_flow is deprecated. Use find_cflow instead.",
+    #     DeprecationWarning,
+    #     stacklevel=2,
+    # )
 
     n_input, n_output = len(input_nodes), len(output_nodes)
     inp = input_nodes
     outp = output_nodes
     if n_input != n_output:
         raise ValueError(
             f"Cannot find flow or gflow. Input ({n_input}) and output ({n_output}) nodes have different size."
@@ -242,34 +262,50 @@
             output_nodes,
             fam,
             iter,
             visited,
             next(fam.predecessors(v)),
         )
         if status:
-            fam = fam.remove_edge(next(fam.predecessors(v)), v)
-            return (fam, visited, 1)
+            try:
+                fam = fam.remove_edge(next(fam.predecessors(v)), v)
+                return (fam, visited, 1)
+            except:
+                return (fam, visited, 0)
 
     for w in graph.neighbors(v):
-        if (visited[w] < iter) and (w not in input_nodes) and (not fam.has_edge(v, w)):
-            if w not in fam.nodes():
-                (fam, visited, status) = _augmented_search(
-                    graph, input_nodes, output_nodes, fam, iter, visited, w
-                )
-                if status:
-                    fam.add_edge(v, w)
-                    return (fam, visited, 1)
-            elif visited[next(fam.predecessors(w))] < iter:
-                (fam, visited, status) = _augmented_search(
-                    graph, fam, iter, visited, next(fam.predecessors(w))
-                )
-                if status:
-                    fam.remove_edge(next(fam.predecessors(w)), w)
-                    fam.add_edge(v, w)
-                    return (fam, visited, 1)
+        try:
+            if (
+                (visited[w] < iter)
+                and (w not in input_nodes)
+                and (not fam.has_edge(v, w))
+            ):
+                if w not in fam.nodes():
+                    (fam, visited, status) = _augmented_search(
+                        graph, input_nodes, output_nodes, fam, iter, visited, w
+                    )
+                    if status:
+                        fam.add_edge(v, w)
+                        return (fam, visited, 1)
+                elif visited[next(fam.predecessors(w))] < iter:
+                    (fam, visited, status) = _augmented_search(
+                        graph,
+                        input_nodes,
+                        output_nodes,
+                        fam,
+                        iter,
+                        visited,
+                        next(fam.predecessors(w)),
+                    )
+                    if status:
+                        fam.remove_edge(next(fam.predecessors(w)), w)
+                        fam.add_edge(v, w)
+                        return (fam, visited, 1)
+        except:
+            return (fam, visited, 0)
 
     return (fam, visited, 0)
 
 
 def check_if_flow(
     graph: GraphState, input_nodes: List, output_nodes: List, flow, partial_order
 ) -> bool:
```

### Comparing `mentpy-0.1.0a4/mentpy/mbqc/mbqcircuit.py` & `mentpy-0.1.0a5/mentpy/mbqc/mbqcircuit.py`

 * *Files 18% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 import numpy as np
 import scipy as scp
 import networkx as nx
 import matplotlib.pyplot as plt
 
 from mentpy.operators import Ment, ControlMent, PauliOp
 from mentpy.mbqc.states.graphstate import GraphState
-from mentpy.mbqc.flow import find_gflow, find_cflow, find_flow, check_if_flow
+from mentpy.mbqc.flow import find_cflow, find_flow, check_if_flow
 
 __all__ = ["MBQCircuit", "draw", "merge", "hstack", "vstack"]
 
 
 class MBQCircuit:
     r"""The MBQCircuit class that deals with operations and manipulations of graph states
 
@@ -57,15 +57,14 @@
         input_nodes: List[int] = [],
         output_nodes: List[int] = [],
         measurements: Optional[dict[Ment]] = None,
         default_measurement: Optional[Ment] = Ment("XY"),
         flow: Optional[Callable] = None,
         partial_order: Optional[callable] = None,
         measurement_order: Optional[List[int]] = None,
-        gflow: Optional[Callable] = None,
         relabel_indices: bool = True,
     ) -> None:
         """Initializes a graph state"""
         # TODO: Remove measurement_order and gflow from the constructor
 
         if relabel_indices:
             N = graph.number_of_nodes()
@@ -76,19 +75,14 @@
             output_nodes = [mapping[i] for i in output_nodes]
             if flow is not None:
                 flow = lambda x: mapping[flow(inv_mapping[x])]
             if partial_order is not None:
                 partial_order = lambda x, y: partial_order(
                     inv_mapping[x], inv_mapping[y]
                 )
-            if gflow is not None:
-                gflow = lambda x: mapping[
-                    gflow(inv_mapping[x])
-                ]  # FIX THIS... gflow output is not a number
-                raise NotImplementedError
             if measurement_order is not None:
                 measurement_order = [mapping[i] for i in measurement_order]
             if measurements is not None:
                 measurements = {mapping[k]: v for k, v in measurements.items()}
 
         self._graph = graph
 
@@ -132,40 +126,44 @@
             for node in self.graph.nodes:
                 if node not in measurements:
                     measurements[node] = (
                         self._default_measurement if node in self.outputc else None
                     )
 
         self._measurements = measurements
+        self._flow, self._partial_order = None, None
         self._update_attributes()
 
         if (flow is None) or (partial_order is None):
             flow, partial_order, depth = find_cflow(graph, input_nodes, output_nodes)
+            # try:
+            #     flow, partial_order = find_flow(
+            #         graph, input_nodes, output_nodes
+            #     )  # TODO: FIX find_cflow!!!!
+            # except:
+            #     pass
+            # if flow is None:
+            #     flow, partial_order = find_cflow(graph, input_nodes, output_nodes)
+            # depth = None
 
         elif (flow is not None) and (partial_order is not None):
             check_if_flow(graph, input_nodes, output_nodes, flow, partial_order)
 
         self._flow = flow
         self._partial_order = partial_order
 
-        if gflow is None:
-            if flow is None:
-                gflow, gpartial_order, depth = find_gflow(
-                    graph, input_nodes, output_nodes
-                )
-            else:
-                gflow, gpartial_order = flow, partial_order
-
-        # TODO: check if given gflow it is definitely gflow
-
-        self.gflow = gflow
-
         if measurement_order is None and flow is not None:
             measurement_order = self.calculate_order()
 
+        # in case we measure an output node
+        quantum_output_nodes = [
+            node for node, i in self.measurements.items() if i is None
+        ]
+        self._quantum_output_nodes = quantum_output_nodes
+
         self._depth = depth
         self._measurement_order = measurement_order
 
     def __repr__(self) -> str:
         """Return the representation of the current MBQC circuit state"""
         return f"MBQCircuit with {self.graph.number_of_nodes()} qubits."
 
@@ -181,17 +179,22 @@
         r"""Set the value of the measurement of the node with index key."""
         if key not in self.graph.nodes:
             raise ValueError(f"Node {key} is not in the graph.")
         if not isinstance(value, Ment):
             raise ValueError(f"Value {value} is not a Measurement object.")
 
         self._measurements[key] = value
+
         # self._update_attributes_key(key)
         self._update_attributes()
 
+        if isinstance(value, ControlMent):
+            # recalculate measurement order
+            self._measurement_order = self.calculate_order()
+
     def __getitem__(self, key):
         r"""Return the value of the measurement of the node with index key."""
         try:
             return self._measurements[key]
         except KeyError:
             raise ValueError(f"Node {key} is not in the graph.")
 
@@ -232,14 +235,24 @@
 
     @property
     def output_nodes(self) -> List[int]:
         r"""Return the output nodes of the MBQC circuit."""
         return self._output_nodes
 
     @property
+    def quantum_output_nodes(self) -> List[int]:
+        r"""Return the output nodes of the MBQC circuit."""
+        return self._quantum_output_nodes
+
+    @property
+    def classical_output_nodes(self) -> List[int]:
+        r"""Return the output nodes of the MBQC circuit."""
+        return self._classical_output_nodes
+
+    @property
     def trainable_nodes(self) -> List[int]:
         r"""Return the trainable nodes of the MBQC circuit."""
         return self._trainable_nodes
 
     @trainable_nodes.setter
     def trainable_nodes(self, trainable_nodes: List[int]) -> None:
         r"""Set the trainable nodes of the MBQC circuit."""
@@ -296,30 +309,59 @@
         r"""Returns :math:`I^c`, the complement of input nodes."""
         return [v for v in self.graph.nodes() if v not in self.input_nodes]
 
     def _update_attributes(self) -> None:
         trainable_nodes = []
         controlled_nodes = []
         planes = {}
+        quantum_outputs = []
+        classical_outputs = []
         for nodei, menti in self._measurements.items():
             if menti is not None:
                 if isinstance(menti, ControlMent):
                     controlled_nodes.append(nodei)
 
                 if menti.angle is None:
                     trainable_nodes.append(nodei)
 
                 planes[nodei] = menti.plane
                 self._measurements[nodei] = copy.deepcopy(menti)
                 self._measurements[nodei].node_id = nodei
+                if nodei in self._output_nodes:
+                    classical_outputs.append(nodei)
             else:
                 planes[nodei] = ""
+                if nodei in self._output_nodes:
+                    quantum_outputs.append(nodei)
+
         self._trainable_nodes = trainable_nodes
         self._controlled_nodes = controlled_nodes
         self._planes = planes
+        self._quantum_output_nodes = quantum_outputs
+        self._classical_output_nodes = classical_outputs
+
+        # update measurement order
+
+        # make artificial graph for new flow with controls
+        # if len(self.controlled_nodes) > 0:
+        #     artificial_graph = self.graph
+        #     for nodei in self.controlled_nodes:
+        #         new_edges = [(nodei, v) for v in self.measurements[nodei].condition.cond_nodes]
+        #         artificial_graph.add_edges_from(new_edges)
+
+        #     flow, partial_order, depth = find_cflow(artificial_graph, self.input_nodes, self.output_nodes)
+        #     self._flow = flow
+        #     self._partial_order = partial_order
+        #     self._depth = depth
+
+        if self._partial_order is not None:
+            old_partial_order = self._partial_order
+            self._partial_order = _create_new_partial_order(
+                self.controlled_nodes, self.measurements, old_partial_order
+            )
 
     def _update_attributes_key(self, key) -> None:
         menti = self._measurements[key]
         if menti is not None:
             if menti.angle is None and key not in self._trainable_nodes:
                 self._trainable_nodes.append(key)
             elif menti.angle is not None and key in self._trainable_nodes:
@@ -331,26 +373,91 @@
             self._planes[key] = ""
             if key in self._trainable_nodes:
                 self._trainable_nodes.remove(key)
 
     def calculate_order(self):
         r"""Returns the order of the measurements"""
         n = len(self.graph)
-        mat = np.zeros((n, n))
+        mat = np.zeros((n, n), dtype=int)
+
+        # for c in self.controlled_nodes:
+        #     nodes_before = self.measurements[c].condition.cond_nodes
+        #     for node in nodes_before:
 
         for indi, i in enumerate(list(self.graph.nodes())):
             for indj, j in enumerate(list(self.graph.nodes())):
                 if self.partial_order(i, j):
                     mat[indi, indj] = 1
-
+        # print(mat)
         sum_mat = np.sum(mat, axis=1)
         order = np.argsort(sum_mat)[::-1]
+        # print("sum_mat", sum_mat)
+        # print("order", order)
 
+        sum_dict = {}
+        for i, s in enumerate(sum_mat):
+            if s not in sum_dict:
+                sum_dict[s] = []
+            sum_dict[s].append(i)
+        sorted_indices = [
+            sum_dict[key] for key in sorted(sum_dict.keys(), reverse=True)
+        ]
+        sorted_labels = [
+            [list(self.graph.nodes())[i] for i in group] for group in sorted_indices
+        ]
+        # print(sorted_labels)
+        # sort within groups can be optimized
+
+        # for group in sorted_labels:
+        #     if len(group) > 1:
+        #         for i in range(len(group)):
+        #             for j in range(i+1, len(group)):
+        #                 if not self.partial_order(group[i], group[j]):
+        #                     group[i], group[j] = group[j], group[i]
+
+        # order = []
+        # print("sorted_labels", sorted_labels)
+        # print(sorted_labels, "antes")
+        # for group in sorted_labels:
+        #     if len(group) > 1:
+        #         # arange controlled nodes
+        #         for c in self.controlled_nodes:
+        #             # check if c is in group
+        #             if c in group:
+        #                 nodes_before = self.measurements[c].condition.cond_nodes
+        #                 for node in nodes_before:
+        #                     # search if node is in group else, swap groups
+        #                     if node in group:
+        #                         indx_node = group.index(node)
+        #                         indx_c = group.index(c)
+        #                         if indx_node > indx_c:
+        #                             group.remove(c)
+        #                             group.insert(indx_node, c)
+
+        # print(sorted_labels)
+        order = [item for sublist in sorted_labels for item in sublist]
         # turn order into labels of graph
-        order = [list(self.graph.nodes())[i] for i in order]
+        # order = [
+        #     list(self.graph.nodes())[i] for i in order
+        # ]  # remove once above is done
+
+        # for c in self.controlled_nodes:
+        #     nodes_before = self.measurements[c].condition.cond_nodes
+        #     for node in nodes_before:
+        #         indx_node = order.index(node)
+        #         indx_c = order.index(c)
+        #         if indx_node > indx_c:
+        #             print("swapping", node, c)
+        #             order.remove(c)
+        #             order.insert(indx_node, c)
+
+        # remove all input nodes and put them at the start
+        for i in self.input_nodes[::-1]:
+            order.remove(i)
+            order.insert(0, i)
 
         return order
 
     def add_edge(self, u, v):
         r"""Adds an edge between nodes u and v"""
         self.graph.add_edge(u, v)
         # try resetting self with new graph, if it fails, remove the edge
@@ -546,47 +653,38 @@
     TODO: Add support for graphs without flow, but with gflow
     TODO: Improve fix when there are control nodes
 
     Group
     -----
     states
     """
-    node_colors = {}
-    for i in state.graph.nodes():
-        if i in state.output_nodes:
-            node_colors[i] = "#ADD8E6"
-        elif i in state.controlled_nodes:
-            node_colors[i] = "#A88FE8"
-        elif i in set(state.nodes()) - set(state.trainable_nodes):
-            node_colors[i] = "#CCCCCC"
-        else:
-            node_colors[i] = "#FFBD59"
 
     # options = {'node_color': '#FFBD59'}
     options = {
-        "node_color": [node_colors[node] for node in state.graph.nodes()],
+        "node_color": "white",
         "font_family": "Dejavu Sans",
         "font_weight": "medium",
         "font_size": 10,
         "edgecolors": "k",
         "node_size": 500,
         "edge_color": "grey",
+        "edge_color_control": "#CCCCCC",
         "with_labels": True,
         "label": "indices",
         "transparent": True,
         "figsize": (8, 3),
         "show_controls": True,
-        "pauliop": None
+        "pauliop": None,
     }
 
     options.update(kwargs)
 
     show_controls = options.pop("show_controls")
-
     pauliop = options.pop("pauliop")
+    edge_color_control = options.pop("edge_color_control")
 
     if pauliop is not None:
         options["label"] = "pauliop"
 
     transp = options.pop("transparent")
     fig, ax = plt.subplots(figsize=options.pop("figsize"))
 
@@ -607,14 +705,27 @@
                         is_output = True
                 fix_wires.append(tuple(wire))
 
     if isinstance(state, GraphState):
         nx.draw(state, ax=ax, **options)
 
     elif isinstance(state, MBQCircuit):
+        node_colors = {}
+        for i in state.graph.nodes():
+            if i in state.quantum_output_nodes:
+                node_colors[i] = "#ADD8E6"
+            elif i in state.controlled_nodes:
+                node_colors[i] = "#A88FE8"
+            elif i in set(state.nodes()) - set(state.trainable_nodes):
+                node_colors[i] = "#CCCCCC"
+            else:
+                node_colors[i] = "#FFBD59"
+
+        options["node_color"] = [node_colors[node] for node in state.graph.nodes()]
+
         fixed_nodes = state.input_nodes + state.output_nodes
         position_xy = {}
         for indx, p in enumerate(state.input_nodes):
             position_xy[p] = (0, -1 * indx)
 
         separation = len(state.outputc) // len(state.output_nodes)
         if fix_wires is not None:
@@ -675,23 +786,23 @@
                         labels[node] = round(state.measurements[node].angle, 3)
                     else:
                         labels[node] = r"$\theta$"
                 else:
                     labels[node] = ""
 
             options["labels"] = labels
-        
+
         elif options["label"] == "pauliop":
             if len(pauliop) != 1:
                 raise ValueError("pauliop must be a single Pauli operator")
             labels = {}
             for ind, node in enumerate(state.graph.nodes()):
                 labels[node] = pauliop.txt[ind]
             options["labels"] = labels
-            
+
         else:
             raise ValueError(
                 "label must be either 'index' or 'plane', not {}".format(
                     options["label"]
                 )
             )
 
@@ -704,15 +815,15 @@
             dashed_edges = []
             for node in state.controlled_nodes:
                 for k in state.measurements[node].condition.cond_nodes:
                     dashed_edges.append((node, k))
             nx.draw_networkx_edges(
                 state.graph,
                 pos=node_pos,
-                edge_color="#CCCCCC",
+                edge_color=edge_color_control,
                 width=1.5,
                 edgelist=dashed_edges,
                 style="dashed",
             )
 
 
 def _graph_with_flow(state):
@@ -721,7 +832,26 @@
     gflow = nx.DiGraph()
     gflow.add_nodes_from(g.nodes())
     for node in state.outputc:
         gflow.add_edge(node, state.flow(node))
     return gflow
 
 
+def _create_new_partial_order(controlled_nodes, measurements, old_partial_order):
+    def new_partial_order(i, j):
+        for c in controlled_nodes:
+            cns = measurements[c].condition.cond_nodes
+
+            ibeforecns = any([old_partial_order(i, cn) for cn in cns]) or i in cns
+            jafterc = old_partial_order(c, j) or j == c
+            # print(f"Comparing {i} and {j}")
+            # print(any([old_partial_order(i, cn) for cn in cns]), i in cns)
+            # print(old_partial_order(c, j), j == c)
+            if ibeforecns and jafterc and i != j:
+                return True
+
+            if j in cns and i == c:
+                return False
+
+        return old_partial_order(i, j)
+
+    return new_partial_order
```

### Comparing `mentpy-0.1.0a4/mentpy/mbqc/states/graphstate.py` & `mentpy-0.1.0a5/mentpy/mbqc/states/graphstate.py`

 * *Files identical despite different names*

### Comparing `mentpy-0.1.0a4/mentpy/mbqc/templates.py` & `mentpy-0.1.0a5/mentpy/mbqc/templates.py`

 * *Files 3% similar despite different names*

```diff
@@ -85,23 +85,25 @@
         input_nodes=[sum(n_wires[:i]) for i in range(len(n_wires))],
         output_nodes=[sum(n_wires[: i + 1]) - 1 for i in range(len(n_wires))],
         **kwargs,
     )
     return gs
 
 
-def grid_cluster(n, m, **kwargs) -> MBQCircuit:
+def grid_cluster(n, m, periodic=False, **kwargs) -> MBQCircuit:
     r"""Returns a grid cluster state of n x m qubits.
 
     Args
     ----
     n: int
         The number of rows in the cluster state.
     m: int
         The number of columns in the cluster state.
+    periodic: bool
+        If True, the returned state will be a cylinder.
 
     Returns
     -------
     The grid cluster state of n x m qubits.
 
     Examples
     --------
@@ -125,14 +127,19 @@
             [(j + sum(n_wires[:i]), j + sum(n_wires[:i]) + 1) for j in range(m - 1)]
         )
 
     # add edges between columns
     for i in range(n - 1):
         g.add_edges_from([(i * m + j, (i + 1) * m + j) for j in range(m)])
 
+    if periodic and n > 1:
+        # add edges between first and last row
+        for j in range(m):
+            g.add_edge(j, (n - 1) * m + j)
+
     gs = MBQCircuit(
         g,
         input_nodes=[sum(n_wires[:i]) for i in range(len(n_wires))],
         output_nodes=[sum(n_wires[: i + 1]) - 1 for i in range(len(n_wires))],
         **kwargs,
     )
     return gs
```

### Comparing `mentpy-0.1.0a4/mentpy/operators/controlled_ment.py` & `mentpy-0.1.0a5/mentpy/operators/controlled_ment.py`

 * *Files 14% similar despite different names*

```diff
@@ -76,13 +76,22 @@
             self.condition,
             self._true_ment.angle,
             self._true_ment.plane,
             self.angle,
             self.plane,
         )
 
-    def matrix(self, angle, *args, **kwargs):
+    def matrix(self, angle: float | None = None, *args, **kwargs):
         """Return the matrix of the controlled measurement operator."""
         if self.condition(*args, **kwargs):
-            return self._true_ment.matrix(angle)
+            return self._true_ment.matrix(angle, *args, **kwargs)
         else:
-            return super().matrix(angle)
+            return super().matrix(angle, *args, **kwargs)
+
+    def get_povm(self, angle: float | None = None, *args, **kwargs):
+        if self.condition(*args, **kwargs):
+            return self._true_ment.get_povm(angle, *args, **kwargs)
+        else:
+            return super().get_povm(angle, *args, **kwargs)
+
+
+ControlledMent = ControlMent
```

### Comparing `mentpy-0.1.0a4/mentpy/operators/gates.py` & `mentpy-0.1.0a5/mentpy/operators/gates.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import numpy as np
-import cirq
+import cirq  # TODO: remove this dependency
 
 CNOT = np.array([[1, 0, 0, 0], [0, 1, 0, 0], [0, 0, 0, 1], [0, 0, 1, 0]])
 
 SWAP = np.array([[1, 0, 0, 0], [0, 0, 1, 0], [0, 1, 0, 0], [0, 0, 0, 1]])
 
 CSGate = np.array([[1, 0, 0, 0], [0, 1, 0, 0], [0, 0, 1, 0], [0, 0, 0, 1j]])
```

### Comparing `mentpy-0.1.0a4/mentpy/operators/ment.py` & `mentpy-0.1.0a5/mentpy/operators/ment.py`

 * *Files 4% similar despite different names*

```diff
@@ -212,37 +212,41 @@
             if self.angle != angle:
                 raise ValueError(
                     f"Measurement has a fixed angle of {round(self.angle, 4)}"
                 )
         elif self.angle is not None:
             angle = self.angle
 
-        if self.plane == "XY":
-            matrix = np.cos(angle) * PauliX + np.sin(angle) * PauliY
-
-        elif self.plane == "XZ":
-            matrix = np.cos(angle) * PauliX + np.sin(angle) * PauliZ
-
-        elif self.plane == "YZ":
-            matrix = np.cos(angle) * PauliY + np.sin(angle) * PauliZ
-
-        elif self.plane == "XYZ":
-            if isinstance(angle, tuple):
-                angle1, angle2 = angle
-            else:
-                raise TypeError(
-                    f"Invalid argument type. Expected tuple but got {type(angle)}"
+        match self.plane:
+            case "XY":
+                matrix = np.cos(angle) * PauliX + np.sin(angle) * PauliY
+            case "X" | "Y" | "Z":
+                matrices = {"X": PauliX, "Y": PauliY, "Z": PauliZ}
+                matrix = matrices[self.plane]
+            case "XZ":
+                matrix = np.cos(angle) * PauliX + np.sin(angle) * PauliZ
+            case "YZ":
+                matrix = np.cos(angle) * PauliY + np.sin(angle) * PauliZ
+            case "XYZ":
+                if isinstance(angle, tuple):
+                    angle1, angle2 = angle
+                else:
+                    raise TypeError(
+                        f"Invalid argument type. Expected tuple but got {type(angle)}"
+                    )
+                matrix = (
+                    np.cos(angle1) * np.cos(angle2) * PauliX
+                    + np.sin(angle1) * np.cos(angle2) * PauliY
+                    + np.sin(angle2) * PauliZ
                 )
-            matrix = (
-                np.cos(angle1) * np.cos(angle2) * PauliX
-                + np.sin(angle1) * np.cos(angle2) * PauliY
-                + np.sin(angle2) * PauliZ
-            )
-
-        elif self.plane in ["X", "Y", "Z"]:
-            matrices = {"X": PauliX, "Y": PauliY, "Z": PauliZ}
-            matrix = matrices[self.plane]
 
         return matrix
 
+    def get_povm(self, angle: Optional[float] = None, *args, **kwargs):
+        """Returns the POVM representation of the measurement."""
+        mat = self.matrix(angle, *args, **kwargs)
+        m0 = (np.eye(2) + mat) / 2
+        m1 = (np.eye(2) - mat) / 2
+        return m0, m1
+
 
 Measurement = Ment
```

### Comparing `mentpy-0.1.0a4/mentpy/operators/pauliop.py` & `mentpy-0.1.0a5/mentpy/operators/pauliop.py`

 * *Files 5% similar despite different names*

```diff
@@ -48,63 +48,62 @@
         """Initialize a PauliOp object."""
 
         if isinstance(op, np.ndarray):
             if op.shape[1] % 2 != 0:
                 raise ValueError(
                     "Tableau representation must have an even number of columns"
                 )
-            self.mat = GF(op)
+            self.matrix = GF(op)
             self.txt = self._mat_to_txt(op)
 
         elif isinstance(op, str):
             op = op.replace(" ", "")
             if op[-1] == ";":
                 op = op[:-1]
 
             op_list = op.split(";")
 
             if not all([len(op) == len(op_list[0]) for op in op_list]):
                 raise ValueError("All Pauli operators must be the same length")
 
             self.txt = op.replace(";", "\n")
-            self.mat = self._txt_to_mat(op_list)
+            self.matrix = self._txt_to_mat(op_list)
 
         elif isinstance(op, list):
             if not all([len(pauliop) == len(op[0]) for pauliop in op]):
                 raise ValueError("All Pauli operators must be the same length")
 
             self.txt = "\n".join(op)
-            self.mat = self._txt_to_mat(op)
+            self.matrix = self._txt_to_mat(op)
 
         else:
             raise ValueError(
                 "PauliOp must be initialized with a string or a numpy array"
             )
 
-        if self.mat.shape[0] == 1:
+        if self.matrix.shape[0] == 1:
             self._array = [self]
         else:
             self._array = [PauliOp(op) for op in self.txt.split("\n") if op != ""]
 
     def __repr__(self):
         return self.txt
 
     def __len__(self):
-        return self.mat.shape[0]
+        return self.matrix.shape[0]
 
     def __getitem__(self, key):
         paulis = self._array[key]
         if isinstance(key, slice):
             return PauliOp(";".join([pauli.txt for pauli in paulis]))
         return paulis
 
     def __contains__(self, item: "PauliOp"):
-        
-        for row in item.mat:
-            if not np.any((self.mat == row).all(axis=1)):
+        for row in item.matrix:
+            if not np.any((self.matrix == row).all(axis=1)):
                 return False
         return True
 
     def _mat_to_txt(self, op):
         n_qubits = op.shape[1] // 2
         txt = ""
         for i in range(op.shape[0]):
@@ -134,39 +133,40 @@
                 elif char == "Z":
                     mat[i, j + n_qubits] = 1
                 elif char == "Y":
                     mat[i, j] = 1
                     mat[i, j + n_qubits] = 1
         return GF(mat)
 
-    def commutator(self, other):
+    def commutator(self, other) -> "PauliOp":
         """Returns the commutator of two Pauli operators."""
-        return PauliOp(self.mat + other.mat)
+        new_matrix = GF(self.matrix) + GF(other.matrix)
+        return PauliOp(new_matrix)
 
     def symplectic_prod(self, other):
         """Returns the symplectic product of two Pauli operators."""
-        x1 = self.mat[:, : self.mat.shape[1] // 2]
-        x2 = other.mat[:, : other.mat.shape[1] // 2]
-        z1 = self.mat[:, self.mat.shape[1] // 2 :]
-        z2 = other.mat[:, other.mat.shape[1] // 2 :]
+        x1 = self.matrix[:, : self.matrix.shape[1] // 2]
+        x2 = other.matrix[:, : other.matrix.shape[1] // 2]
+        z1 = self.matrix[:, self.matrix.shape[1] // 2 :]
+        z2 = other.matrix[:, other.matrix.shape[1] // 2 :]
         return x1 @ z2.T + z1 @ x2.T
 
     def append(self, other):
         """Appends a Pauli operator to the end of another Pauli operator.
 
         Examples
         --------
         .. ipython:: python
 
             op1 = mp.PauliOp('XIZ;IZI')
             op2 = mp.PauliOp('XZZ')
             op1.append(op2)
             print(op1)
         """
-        new_mat = np.vstack((self.mat, other.mat))
+        new_mat = np.vstack((self.matrix, other.matrix))
         self.__init__(new_mat)
 
     def get_subset(self, indices):
         """Returns a subset of the Pauli operator.
 
         Parameters
         ----------
@@ -176,12 +176,12 @@
         Examples
         --------
         .. ipython:: python
 
             op = mp.PauliOp('XIZ;ZII;IIZ;IZI')
             print(op.get_subset([0, 2]))
         """
-        if max(indices) >= self.mat.shape[1] // 2:
+        if max(indices) >= self.matrix.shape[1] // 2:
             raise ValueError("Index out of range")
 
-        indices += [i + self.mat.shape[1] // 2 for i in indices]
-        return PauliOp(self.mat[:, indices])
+        indices += [i + self.matrix.shape[1] // 2 for i in indices]
+        return PauliOp(self.matrix[:, indices])
```

### Comparing `mentpy-0.1.0a4/mentpy/optimizers/adam.py` & `mentpy-0.1.0a5/mentpy/optimizers/adam.py`

 * *Files identical despite different names*

### Comparing `mentpy-0.1.0a4/mentpy/optimizers/base_optimizer.py` & `mentpy-0.1.0a5/mentpy/optimizers/base_optimizer.py`

 * *Files identical despite different names*

### Comparing `mentpy-0.1.0a4/mentpy/optimizers/rcd.py` & `mentpy-0.1.0a5/mentpy/optimizers/rcd.py`

 * *Files identical despite different names*

### Comparing `mentpy-0.1.0a4/mentpy/optimizers/sgd.py` & `mentpy-0.1.0a5/mentpy/optimizers/sgd.py`

 * *Files identical despite different names*

### Comparing `mentpy-0.1.0a4/mentpy/simulators/base_simulator.py` & `mentpy-0.1.0a5/mentpy/simulators/base_simulator.py`

 * *Files 6% similar despite different names*

```diff
@@ -31,14 +31,15 @@
     def __init__(
         self,
         mbqcircuit: MBQCircuit,
         input_state: np.ndarray = None,
     ) -> None:
         self._mbqcirc = mbqcircuit
         self._input_state = input_state
+        self._outcomes = {}
 
     @property
     def mbqcircuit(self) -> MBQCircuit:
         """The MBQC circuit used for the simulation."""
         return self._mbqcirc
 
     @property
@@ -47,14 +48,24 @@
         return self._input_state
 
     @input_state.setter
     def input_state(self, input_state: np.ndarray):
         """Sets the input state of the simulator."""
         self._input_state = input_state
 
+    @property
+    def outcomes(self) -> dict:
+        """The outcomes of the simulation."""
+        return self._outcomes
+
+    @outcomes.setter
+    def outcomes(self, outcomes: dict):
+        """Sets the outcomes of the simulation."""
+        self._outcomes = outcomes
+
     def __call__(self, angles: List[float], **kwargs):
         return self.run(angles, **kwargs)
 
     def __repr__(self) -> str:
         return f"{self.__class__.__name__} for {self.mbqcircuit}"
 
     @abc.abstractmethod
```

### Comparing `mentpy-0.1.0a4/mentpy/simulators/cirq_simulator.py` & `mentpy-0.1.0a5/mentpy/simulators/cirq_simulator.py`

 * *Files identical despite different names*

### Comparing `mentpy-0.1.0a4/mentpy/simulators/np_simulator_dm.py` & `mentpy-0.1.0a5/mentpy/simulators/np_simulator_dm.py`

 * *Files 10% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 q_zero = np.array([1, 0])
 qubit_plus = H @ q_zero
 
 
 class NumpySimulatorDM(BaseSimulator):
     """A density matrix simulator that uses numpy to simulate the quantum circuit."""
 
+    # TODO: CALCULATE OPTIMAL WINDOW SIZE AUTOMATICALLY
     def __init__(
         self, mbqcircuit: MBQCircuit, input_state: np.ndarray = None, **kwargs
     ) -> None:
         super().__init__(mbqcircuit, input_state)
 
         self.window_size = kwargs.pop("window_size", 1)
         self.schedule = kwargs.pop("schedule", None)
@@ -41,24 +42,29 @@
                 i for i in self.schedule if i not in mbqcircuit.measurements.values()
             ]
         elif mbqcircuit.measurement_order is not None:
             # remove output nodes from the measurement order
             self.schedule_measure = [
                 i
                 for i in mbqcircuit.measurement_order
-                if i not in mbqcircuit.output_nodes
+                if i not in mbqcircuit.quantum_output_nodes
             ]
             self.schedule = mbqcircuit.measurement_order
             if self.window_size == 1 and mbqcircuit.flow is not None:
                 self.window_size = len(mbqcircuit.input_nodes) + 1
         else:
             raise ValueError(
                 "Schedule must be provided for numpy simulator as the MBQCircuit does not have a flow."
             )
 
+        input_state = self.reorder_qubits(
+            input_state,
+            self.mbqcircuit.input_nodes,
+            self.schedule[: len(self.mbqcircuit.input_nodes)],
+        )
         self.input_state = input_state
 
         n_qubits_input = len(mbqcircuit.input_nodes)
 
         if n_qubits_input > self.window_size:
             raise ValueError(
                 f"Input state has {n_qubits_input} qubits, but window size is set to {self.window_size}."
@@ -114,16 +120,21 @@
 
         current_ment = self.mbqcircuit[
             self.schedule_measure[self.current_measurement]
         ].copy()
         self.qstate, outcome = self.measure_ment(
             current_ment, angle, 0, force0=self.force0
         )
-
+        # check if qstate has nan
+        if np.isnan(self.qstate).any():
+            raise ValueError(
+                "qstate has nan, you might want to increase the window size"
+            )
         self.current_measurement += 1
+
         self.qstate = self.partial_trace(self.qstate, [0])
 
         if self.current_measurement + self.window_size <= len(
             self.mbqcircuit.graph.nodes
         ):
             self.qstate = np.kron(self.qstate, self.pure2density(qubit_plus))
             new_qubit = self.current_simulated_nodes()[-1]
@@ -151,34 +162,45 @@
 
         for i in self.schedule_measure:
             if i in self.mbqcircuit.trainable_nodes:
                 angle = angles[self.mbqcircuit.trainable_nodes.index(i)]
             else:
                 angle = self.mbqcircuit[i].angle
 
-            plane = self.mbqcircuit[i].plane
-
             self.qstate, outcome = self.measure(angle)
             self.outcomes[i] = outcome
 
-        # check if output nodes have a measurement, if so, measure them
-        for i in self.mbqcircuit.output_nodes:
-            if isinstance(self.mbqcircuit[i], Ment):
-                self.qstate, outcome = self.measure_ment(
-                    self.mbqcircuit[i], self.mbqcircuit[i].angle, i, force0=self.force0
-                )
-                self.outcomes[i] = outcome
+        current_output_order = [
+            i for i in self.schedule if i not in self.schedule_measure
+        ]
+        if self.mbqcircuit.quantum_output_nodes != current_output_order:
+            self.qstate = self.reorder_qubits(
+                self.qstate, current_output_order, self.mbqcircuit.quantum_output_nodes
+            )
+
+        # # check if output nodes have a measurement, if so, measure them
+        # for i in self.mbqcircuit.output_nodes:
+        #     if isinstance(self.mbqcircuit[i], Ment):
+        #         self.qstate, outcome = self.measure_ment(
+        #             self.mbqcircuit[i], self.mbqcircuit[i].angle, i, force0=self.force0
+        #         )
+        #         self.outcomes[i] = outcome
 
         return self.qstate
 
     def reset(self, input_state: np.ndarray = None):
         """Resets the simulator to the initial state."""
         self.current_measurement = 0
 
         if input_state is not None:
+            input_state = self.reorder_qubits(
+                input_state,
+                self.mbqcircuit.input_nodes,
+                self.schedule[: len(self.mbqcircuit.input_nodes)],
+            )
             self.input_state = input_state
             for i in range(self.window_size - len(self.mbqcircuit.input_nodes)):
                 self.input_state = np.kron(self.input_state, qubit_plus)
 
         self.qstate = self.pure2density(self.input_state)
 
         self.qstate = self.initial_czs @ self.qstate @ np.conj(self.initial_czs).T
@@ -261,30 +283,32 @@
         """
         Measures a ment
         """
         op = ment.matrix(angle, self.outcomes)
         if op is None:
             raise ValueError(f"Ment has no matrix representation at qubit {i}")
 
-        p0 = (np.eye(2) + op) / 2
-        p1 = (np.eye(2) - op) / 2
-        p1_extended = self.arbitrary_qubit_gate(
-            p1, i, self.current_number_simulated_nodes()
-        )
+        p0, p1 = ment.get_povm(angle, self.outcomes)
         p0_extended = self.arbitrary_qubit_gate(
             p0, i, self.current_number_simulated_nodes()
         )
+        p1_extended = self.arbitrary_qubit_gate(
+            p1, i, self.current_number_simulated_nodes()
+        )
 
         prob0 = np.real(np.trace(self.qstate @ p0_extended))
         prob1 = np.real(np.trace(self.qstate @ p1_extended))
 
         if not force0:
             outcome = np.random.choice([0, 1], p=[prob0, prob1] / (prob0 + prob1))
         else:
-            outcome = 0
+            if prob0 < 1e-4:
+                outcome = 1  # important when measuring Z's -- should make pretty
+            else:
+                outcome = 0
 
         if outcome == 0:
             self.qstate = p0_extended @ self.qstate @ np.conj(p0_extended).T / prob0
         else:
             self.qstate = p1_extended @ self.qstate @ np.conj(p1_extended).T / prob1
 
         return self.qstate, outcome
@@ -350,7 +374,41 @@
 
     def pure2density(self, psi):
         """
         Input: quantum state
         Output: corresponding density matrix
         """
         return np.outer(psi, np.conj(psi).T)
+
+    def find_swaps(self, source, target):
+        assert set(source) == set(
+            target
+        ), f"Both lists must have the same elements, but source={source} and target={target}"
+
+        swaps = []
+        source = list(source)  # Make a copy to avoid modifying the original list
+
+        for i, target_element in enumerate(target):
+            if source[i] != target_element:
+                j = source.index(target_element, i + 1)
+                source[i], source[j] = source[j], source[i]  # Swap elements
+                swaps.append((i, j))
+
+        return swaps
+
+    def reorder_qubits(self, state, current_order, target_order):
+        """
+        Reorders the qubits in the given order.
+        """
+        new_state = state.copy()
+        type_state = "dm"
+        if len(new_state.shape) == 1:
+            type_state = "pure"
+
+        swaps = self.find_swaps(current_order, target_order)
+        for i, j in swaps:
+            swap_op = self.swap_ij(i, j, len(current_order))
+            if type_state == "pure":
+                new_state = swap_op @ new_state
+            else:
+                new_state = swap_op @ new_state @ np.conj(swap_op).T
+        return new_state
```

### Comparing `mentpy-0.1.0a4/mentpy/simulators/np_simulator_sv.py` & `mentpy-0.1.0a5/mentpy/simulators/np_simulator_sv.py`

 * *Files 7% similar despite different names*

```diff
@@ -59,14 +59,19 @@
             if self.window_size == 1 and mbqcircuit.flow is not None:
                 self.window_size = len(mbqcircuit.input_nodes) + 1
         else:
             raise ValueError(
                 "Schedule must be provided for numpy simulator as the MBQCircuit does not have a flow."
             )
 
+        input_state = self.reorder_qubits(
+            input_state,
+            self.mbqcircuit.input_nodes,
+            self.schedule[: len(self.mbqcircuit.input_nodes)],
+        )
         self.input_state = input_state
 
         n_qubits_input = len(mbqcircuit.input_nodes)
 
         if n_qubits_input > self.window_size:
             raise ValueError(
                 f"Input state has {n_qubits_input} qubits, but window size is set to {self.window_size}."
@@ -118,16 +123,17 @@
     def measure(self, angle: float) -> Tuple:
         if self.current_measurement >= len(self.schedule_measure):
             raise ValueError("No more measurements to be done.")
 
         current_ment = self.mbqcircuit[
             self.schedule_measure[self.current_measurement]
         ].copy()
+
         self.qstate, outcome = self.measure_ment(
-            current_ment.set_angle(angle), 0, force0=self.force0
+            current_ment, angle, 0, force0=self.force0
         )
 
         self.current_measurement += 1
         self.qstate = self.partial_trace_pure_state(self.qstate, [0])
 
         if self.current_measurement + self.window_size <= len(
             self.mbqcircuit.graph.nodes
@@ -140,15 +146,15 @@
 
             # do cz between new qubit and neighbours
             indx_new = self.current_simulated_nodes().index(new_qubit)
             for neighbour in neighbours:
                 if neighbour in self.current_simulated_nodes():
                     indxn = self.current_simulated_nodes().index(neighbour)
                     cz = self.controlled_z(indxn, indx_new, self.window_size)
-                    self.qstate = cz @ self.qstate @ np.conj(cz.T)
+                    self.qstate = cz @ self.qstate
 
         return self.qstate, outcome
 
     def run(
         self, angles: List[float], output_form="dm"
     ) -> Tuple[List[int], np.ndarray]:
         """Measures the quantum state in the given pattern.
@@ -162,53 +168,60 @@
             raise ValueError(
                 f"Number of angles ({len(angles)}) does not match number of trainable nodes ({len(self.mbqcircuit.trainable_nodes)})."
             )
 
         for i in self.schedule_measure:
             if i in self.mbqcircuit.trainable_nodes:
                 angle = angles[self.mbqcircuit.trainable_nodes.index(i)]
-                plane = self.mbqcircuit[self.mbqcircuit.trainable_nodes.index(i)].plane
             else:
-                plane = self.mbqcircuit[i].plane
-                if plane == "X":
-                    angle = 0
-                elif plane == "Y":
-                    angle = np.pi / 2
-                else:
-                    raise ValueError(
-                        f"Plane {plane} is not supported for numpy simulator."
-                    )
+                angle = self.mbqcircuit[i].angle
 
             self.qstate, outcome = self.measure(angle)
+            self.outcomes[i] = outcome
 
         # check if output nodes have a measurement, if so, measure them
         for i in self.mbqcircuit.output_nodes:
             if isinstance(self.mbqcircuit[i], Ment):
                 self.qstate, outcome = self.measure_ment(
-                    self.mbqcircuit[i], i, force0=self.force0
+                    self.mbqcircuit[i], self.mbqcircuit[i].angle, i, force0=self.force0
                 )
+                self.outcomes[i] = outcome
+
+        current_output_order = self.schedule[-len(self.mbqcircuit.output_nodes) :]
+        if self.mbqcircuit.quantum_output_nodes != current_output_order:
+            self.qstate = self.reorder_qubits(
+                self.qstate, current_output_order, self.mbqcircuit.output_nodes
+            )
+
         if output_form.lower() == "dm" or output_form.lower() == "densitymatrix":
             return np.outer(self.qstate, np.conj(self.qstate).T)
         elif output_form.lower() == "sv" or output_form.lower() == "statevector":
             return self.qstate
         else:
             raise ValueError(f"Output form {output_form} is not supported.")
 
     def reset(self, input_state: np.ndarray = None):
         """Resets the simulator to the initial state."""
         self.current_measurement = 0
 
         if input_state is not None:
+            input_state = self.reorder_qubits(
+                input_state,
+                self.mbqcircuit.input_nodes,
+                self.schedule[: len(self.mbqcircuit.input_nodes)],
+            )
             self.input_state = input_state
             for i in range(self.window_size - len(self.mbqcircuit.input_nodes)):
                 self.input_state = np.kron(self.input_state, qubit_plus)
 
         self.qstate = self.input_state
 
-        self.qstate = self.initial_czs @ self.qstate @ np.conj(self.initial_czs).T
+        self.qstate = self.initial_czs @ self.qstate
+
+        self.outcomes = {}
 
     def arbitrary_qubit_gate(self, u, i, n):
         """
         Single qubit gate u acting on qubit i
         n is the number of qubits
         """
         op = 1
@@ -252,65 +265,68 @@
                     op3, np.kron(np.array([[1], [0]]).T, np.array([[0], [1]]))
                 )
             else:
                 op2 = np.kron(op2, np.eye(2))
                 op3 = np.kron(op3, np.eye(2))
         return op1 + op2 + op3 + op4
 
-    def partial_trace_pure_state(self, psi, indices):
-        """Partial trace of a pure state over some indices. It is asumed that the indices
-        over which the trace is taken are unentangled with the rest of the rest of the system.
-        """
-        n = int(np.log2(len(psi)))
-        indices_to_keep = [x for x in range(n) if x not in indices]
-        preserved_dim = 2 ** len(indices_to_keep)
-
-        # Reshape the state vector into a tensor with shape (2, 2, ..., 2)
-        reshaped_psi = psi.reshape([2] * n)
-
-        # Move the preserved dimensions to the front and traced dimensions to the back
-        reshaped_psi = np.moveaxis(
-            reshaped_psi, indices_to_keep, range(len(indices_to_keep))
+    def partial_trace_pure_state(self, psi, indices_to_trace):
+        num_qubits = int(np.log2(psi.shape[0]))
+
+        remaining_qubits = sorted(set(range(num_qubits)) - set(indices_to_trace))
+        num_remaining_qubits = len(remaining_qubits)
+
+        # Calculate the initial shape of the tensor product
+        initial_shape = [2] * num_qubits
+
+        # Reshape the state vector into a tensor
+        tensor = psi.reshape(initial_shape)
+
+        # Transpose the tensor to move the qubits to trace to the end
+        tensor = tensor.transpose(remaining_qubits + indices_to_trace)
+
+        # Calculate the final shape after tracing
+        final_shape = [2] * num_remaining_qubits
+
+        # Perform the partial trace by summing over the traced qubits
+        traced_tensor = tensor.reshape(final_shape + [-1]).sum(
+            axis=tuple(range(-len(indices_to_trace), 0))
         )
 
-        # Select the appropriate elements from the reshaped tensor
-        index_slice = [0] * len(
-            indices
-        )  # assuming that the traced qubits are in state |0>
-        reshaped_psi = reshaped_psi[tuple(index_slice)]
+        # Reshape to a vector
+        traced_tensor = traced_tensor.reshape(-1)
 
-        # Reshape back into a vector with shape (preserved_dim,)
-        output_state = reshaped_psi.reshape((preserved_dim,))
+        # Normalize the result
+        traced_tensor /= np.linalg.norm(traced_tensor)
 
-        return output_state
+        return traced_tensor
 
-    def measure_ment(self, ment: Ment, i, force0=True):
+    def measure_ment(self, ment: Ment, angle, i, force0=False):
         """
         Measures a ment
         """
         if ment.plane not in ["X", "Y", "XY"]:
             raise ValueError(
                 f"Plane {ment.plane} is not supported for state vector numpy simulator."
             )
 
-        op = ment.matrix()
+        op = ment.matrix(angle, self.outcomes)
         if op is None:
             raise ValueError(f"Ment has no matrix representation at qubit {i}")
 
-        p0 = (np.eye(2) + op) / 2
-        p1 = (np.eye(2) - op) / 2
+        p0, p1 = ment.get_povm(angle, self.outcomes)
         p1_extended = self.arbitrary_qubit_gate(
             p1, i, self.current_number_simulated_nodes()
         )
         p0_extended = self.arbitrary_qubit_gate(
             p0, i, self.current_number_simulated_nodes()
         )
 
-        prob0 = np.abs(np.vdot(self.qstate, p0_extended @ self.qstate)) ** 2
-        prob1 = np.abs(np.vdot(self.qstate, p1_extended @ self.qstate)) ** 2
+        prob0 = np.dot(np.conj(self.qstate), p0_extended @ self.qstate)
+        prob1 = np.dot(np.conj(self.qstate), p1_extended @ self.qstate)
 
         if not force0:
             outcome = np.random.choice([0, 1], p=[prob0, prob1] / (prob0 + prob1))
         else:
             outcome = 0
 
         if outcome == 0:
@@ -376,7 +392,33 @@
                 )
             else:
                 op2 = np.kron(op2, np.eye(2))
                 op3 = np.kron(op3, np.eye(2))
                 op4 = np.kron(op4, np.eye(2))
 
         return op1 + op2 + op3 + op4
+
+    def find_swaps(self, source, target):
+        assert set(source) == set(
+            target
+        ), f"Both lists must have the same elements, but source={source} and target={target}"
+
+        swaps = []
+        source = list(source)  # Make a copy to avoid modifying the original list
+
+        for i, target_element in enumerate(target):
+            if source[i] != target_element:
+                j = source.index(target_element, i + 1)
+                source[i], source[j] = source[j], source[i]  # Swap elements
+                swaps.append((i, j))
+
+        return swaps
+
+    def reorder_qubits(self, state, current_order, target_order):
+        """
+        Reorders the qubits in the given order.
+        """
+        new_state = state.copy()
+        swaps = self.find_swaps(current_order, target_order)
+        for i, j in swaps:
+            new_state = self.swap_ij(i, j, len(current_order)) @ new_state
+        return new_state
```

### Comparing `mentpy-0.1.0a4/mentpy/simulators/pattern_simulator.py` & `mentpy-0.1.0a5/mentpy/simulators/pattern_simulator.py`

 * *Files 0% similar despite different names*

```diff
@@ -43,15 +43,15 @@
         supported_backends = {
             "pennylane": PennylaneSimulator,
             # "cirq": CirqSimulator,
             # "qiskit": QiskitSimulator,
             "numpy-dm": NumpySimulatorDM,
             "numpy-sv": NumpySimulatorSV,
         }
-        
+
         backend = backend.lower()
         if backend not in supported_backends:
             raise ValueError(
                 f"Backend {backend} not supported. Supported backends are {supported_backends.keys()}"
             )
 
         if input_state is None:
```

### Comparing `mentpy-0.1.0a4/mentpy/simulators/pennylane_simulator.py` & `mentpy-0.1.0a5/mentpy/simulators/pennylane_simulator.py`

 * *Files 6% similar despite different names*

```diff
@@ -45,38 +45,28 @@
             raise NotImplementedError(
                 "Controlled nodes are not supported with the PennyLane simulator."
             )
 
     def measure(self, angle: float, plane: str = "XY"):
         raise NotImplementedError
 
-    def run(
-        self, angles: List[float], planes: Union[List[str], str] = "XY", **kwargs
-    ) -> Tuple[List[int], np.ndarray]:
+    def run(self, angles: List[float], **kwargs) -> Tuple[List[int], np.ndarray]:
         if len(angles) != len(self.mbqcircuit.trainable_nodes):
             raise ValueError(
                 f"Number of angles ({len(angles)}) does not match number of trainable nodes ({len(self.mbqcircuit.trainable_nodes)})."
             )
 
-        # TODO: Implement this
-        if planes != "XY":
-            raise NotImplementedError
-
-        if isinstance(planes, str):
-            planes = [planes] * len(angles)
-
         # extend angles to all nodes
 
         extended_angles = []
 
         if len(self.mbqcircuit.trainable_nodes) != len(self.mbqcircuit.outputc):
             for i in self.mbqcircuit.outputc:
                 if i in self.mbqcircuit.trainable_nodes:
                     angle = angles[self.mbqcircuit.trainable_nodes.index(i)]
-                    plane = planes[self.mbqcircuit.trainable_nodes.index(i)]
                 else:
                     plane = self.mbqcircuit.planes[i]
                     if plane == "X":
                         angle = 0
                     elif plane == "Y":
                         angle = np.pi / 2
                     else:
@@ -136,31 +126,33 @@
                     qml.GeneralizedAmplitudeDamping(wires=i, *args, **kwargs)
                 else:
                     raise ValueError(f"Unrecognized circuit noise: {circuit_noise}")
 
         topord_no_output = [
             x for x in gsc.measurement_order if (x not in gsc.output_nodes)
         ]
-        for indx, p in zip(topord_no_output, param[: len(gsc.outputc)]):
-            qml.RZ(p, wires=indx)
+        for indx in topord_no_output:
+            p = param[gsc.outputc.index(indx)]
+
+            qml.RZ(-p, wires=indx)
             qml.Hadamard(wires=indx)
             m_0 = qml.measure(indx)
             qml.cond(m_0, qml.PauliX)(wires=gsc.flow(indx))
             for neigh in gr.neighbors(gsc.flow(indx)):
                 if neigh != indx and (
                     gsc.measurement_order.index(neigh)
                     > gsc.measurement_order.index(indx)
                 ):
                     qml.cond(m_0, qml.PauliZ)(wires=neigh)
 
-        if output == "expval":
-            for indx, p in zip(gsc.output_nodes, param[len(gsc.outputc) :]):
-                qml.RZ(p, wires=indx)
-            return [qml.expval(qml.PauliX(j)) for j in gsc.output_nodes]
-        elif output == "sample":
-            for indx, p in zip(gsc.output_nodes, param[len(gsc.outputc) :]):
-                qml.RZ(p, wires=indx)
-            return [qml.sample(qml.PauliX(j)) for j in gsc.output_nodes]
-        elif output == "density":
+        # if output == "expval":
+        #     for indx, p in zip(gsc.output_nodes, param[len(gsc.outputc) :]):
+        #         qml.RZ(-p, wires=indx)
+        #     return [qml.expval(qml.PauliX(j)) for j in gsc.output_nodes]
+        # elif output == "sample":
+        #     for indx, p in zip(gsc.output_nodes, param[len(gsc.outputc) :]):
+        #         qml.RZ(-p, wires=indx)
+        #     return [qml.sample(qml.PauliX(j)) for j in gsc.output_nodes]
+        if output == "density":
             return qml.density_matrix(gsc.output_nodes)
 
     return circuit
```

### Comparing `mentpy-0.1.0a4/mentpy/simulators/qiskit_simulators.py` & `mentpy-0.1.0a5/mentpy/simulators/qiskit_simulators.py`

 * *Files identical despite different names*

### Comparing `mentpy-0.1.0a4/mentpy/utils/expressivity.py` & `mentpy-0.1.0a5/mentpy/utils/expressivity.py`

 * *Files identical despite different names*

### Comparing `mentpy-0.1.0a4/mentpy/utils/flow_space.py` & `mentpy-0.1.0a5/mentpy/utils/flow_space.py`

 * *Files identical despite different names*

### Comparing `mentpy-0.1.0a4/mentpy/utils/generate_data.py` & `mentpy-0.1.0a5/mentpy/utils/generate_data.py`

 * *Files identical despite different names*

### Comparing `mentpy-0.1.0a4/mentpy/utils/lc_equivalence.py` & `mentpy-0.1.0a5/mentpy/utils/lc_equivalence.py`

 * *Files identical despite different names*

### Comparing `mentpy-0.1.0a4/mentpy/utils/lie_algebra.py` & `mentpy-0.1.0a5/mentpy/utils/lie_algebra.py`

 * *Files 22% similar despite different names*

```diff
@@ -36,18 +36,21 @@
         if row >= rows:
             break
 
     # Back-substitution
     x = np.zeros(cols, dtype=int)
     for row in range(min(rows, cols) - 1, -1, -1):
         col = np.argmax(augmented_matrix[row, :cols])
-        x[col] = augmented_matrix[row, -1] ^ np.sum(augmented_matrix[row, col + 1:cols] * x[col + 1:cols])
+        x[col] = augmented_matrix[row, -1] ^ np.sum(
+            augmented_matrix[row, col + 1 : cols] * x[col + 1 : cols]
+        )
 
     return x
 
+
 def _constrains(j: int, state: MBQCircuit, stabilizers: PauliOp):
     """Creates the A matrix for the constraints on the stabilizers"""
 
     if j not in state.outputc:
         raise ValueError("j should be in outputc")
 
     mo = state.measurement_order
@@ -57,19 +60,19 @@
 
     A = []
     b = []
     for k in mo:
         indk = mo.index(k)
         indj = mo.index(j)
         if indk <= indj:
-            A.append(stabilizers[k].mat[0, :len(mo)])
+            A.append(stabilizers[k].matrix[0, : len(mo)])
             b.append(np.zeros(1, dtype=int))
 
     for k in [mapping[i] for i in state.outputc]:
-        A.append(stabilizers[k].mat[0, len(mo) :])
+        A.append(stabilizers[k].matrix[0, len(mo) :])
         p = 0 if k != j else 1
         b.append(np.array([p]))
 
     return GF(np.vstack(A)), GF(np.vstack(b))
 
 
 def _check_solution(A, b, x):
@@ -87,28 +90,30 @@
 
     op = PauliOp("I" * len(state.measurement_order))
     for i in range(len(sol)):
         if sol[i] == 1:
             op = op.commutator(stabilizers[i])
     return op
 
+
 def calculate_complete_gens_lie_algebra(state: MBQCircuit):
     """Calculates the Pauli operators for the Lie algebra of a given state"""
     graph_stabs = state.stabilizers()
 
     lieAlgebra = None
     for i in state.outputc:
         op = _find_solution(i, state, graph_stabs)
         if lieAlgebra is None:
             lieAlgebra = op
         else:
             lieAlgebra.append(op)
-    
+
     return lieAlgebra
 
+
 def calculate_gens_lie_algebra(state: MBQCircuit):
     """Calculates the generators of the Lie algebra of a given state"""
     mapping = {
         i: j
         for i, j in zip(state.measurement_order, range(len(state.measurement_order)))
     }
     graph_stabs = state.stabilizers()
@@ -121,58 +126,100 @@
         else:
             lieAlgebra.append(op)
 
     output_ops = lieAlgebra.get_subset([mapping[i] for i in state.output_nodes])
     return remove_repeated_ops(output_ops)
 
 
-def lie_algebra_completion(generators: PauliOp, max_iter: int = 100):
+# def lie_algebra_completion_old(generators: PauliOp, max_iter: int = 1000):
+#     """Completes a given set of Pauli operators to a basis of the Lie algebra"""
+#     lieAlg = copy.deepcopy(generators)
+#     already_commutated = []
+#     iter = 0
+#     while iter < max_iter:
+#         iter += 1
+#         new_lieAlg = None
+#         for i, j in combinations(range(len(lieAlg)), 2):
+#             if (i, j) not in already_commutated:
+#                 already_commutated.append((i, j))
+#                 if lieAlg[i].symplectic_prod(lieAlg[j])[0][0] != 0:
+#                     if new_lieAlg is None:
+#                         new_lieAlg = lieAlg[i].commutator(lieAlg[j])
+#                     else:
+#                         new_lieAlg.append(lieAlg[i].commutator(lieAlg[j]))
+
+#         if new_lieAlg is None:
+#             break
+#         else:
+#             lieAlg.append(new_lieAlg)
+#             new_lieAlg = remove_repeated_ops(lieAlg)
+#             if len(new_lieAlg) == len(lieAlg):
+#                 break
+
+#         lieAlg = new_lieAlg
+
+#     if iter >= max_iter - 1:
+#         raise ValueError("Max iterations reached")
+
+#     return lieAlg
+
+
+def lie_algebra_completion(generators: PauliOp, max_iter: int = 1000):
     """Completes a given set of Pauli operators to a basis of the Lie algebra"""
     lieAlg = copy.deepcopy(generators)
-    already_commutated = []
+    already_commutated = set()
+    n = len(lieAlg)
+    queue = [(i, j) for i, j in combinations(range(n), 2)]
     iter = 0
-    while iter < max_iter:
+    while iter < max_iter and queue:
         iter += 1
-        new_lieAlg = None
-        for i, j in combinations(range(len(lieAlg)), 2):
-            if (i, j) not in already_commutated:
-                already_commutated.append((i, j))
-                if lieAlg[i].symplectic_prod(lieAlg[j])[0][0] != 0:
-                    if new_lieAlg is None:
-                        new_lieAlg = lieAlg[i].commutator(lieAlg[j])
-                    else:
-                        new_lieAlg.append(lieAlg[i].commutator(lieAlg[j]))
-
-        if new_lieAlg is None:
-            break
-        else:
-            lieAlg.append(new_lieAlg)
-            new_lieAlg = remove_repeated_ops(lieAlg)
-            if len(new_lieAlg) == len(lieAlg):
-                break
-
-        lieAlg = new_lieAlg
-        
+        i, j = queue.pop(0)
+        if (i, j) not in already_commutated:
+            already_commutated.add((i, j))
+            newOp = lieAlg[i].commutator(lieAlg[j])
+            if newOp not in lieAlg:
+                lieAlg.append(newOp)
+                queue.extend((len(lieAlg) - 1, k) for k in range(len(lieAlg) - 1))
+
+    if iter >= max_iter - 1 and queue:
+        raise ValueError("Max iterations reached")
+
+    # check IIII is in lieAlg
+    n_qubits = int(lieAlg.matrix.shape[1] // 2)
+    if PauliOp("I" * n_qubits) not in lieAlg:
+        lieAlg.append(PauliOp("I" * n_qubits))
 
     return lieAlg
 
-def calculate_lie_algebra(state: MBQCircuit, max_iter: int = 100):
+
+def calculate_lie_algebra(state: MBQCircuit, max_iter: int = 10000):
     """Calculates the Lie algebra of a given state"""
     generators = calculate_gens_lie_algebra(state)
     return lie_algebra_completion(generators, max_iter=max_iter)
 
 
 def remove_repeated_ops(ops: PauliOp):
     """Removes repeated Pauli operators from a set"""
     ops = copy.deepcopy(ops)
     unrep_ops = ops[0]
     for op in ops[1:]:
         if op not in unrep_ops:
             unrep_ops.append(op)
     return unrep_ops
 
+
 # dimension of su(n)
 def dim_su(n):
+    """Calculates the dimension of :math:`Su(n)`"""
     return int(n**2 - 1)
 
+
 def dim_so(n):
-    return int(n*(n-1)//2)
+    """Calculates the dimension of :math:`So(n)`"""
+    return int(n * (n - 1) // 2)
+
+
+def dim_sp(n):
+    """Calculates the dimension of :math:`Sp(n)`"""
+    assert n % 2 == 0, "n must be even"
+    n = n // 2
+    return int(n * (2 * n + 1))
```

### Comparing `mentpy-0.1.0a4/mentpy.egg-info/PKG-INFO` & `mentpy-0.1.0a5/mentpy.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,17 @@
 Metadata-Version: 2.1
 Name: mentpy
-Version: 0.1.0a4
+Version: 0.1.0a5
 Summary: A Python library for simulating MBQC circuits
 Home-page: https://github.com/BestQuark/mentpy
 Author: Luis Mantilla
 Author-email: luismantilla99@outlook.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-:warning: **This library is under development.**
-
 <p align="center">
   <img src="./docs/_static/logo.png" alt="MentPy: A Measurement-Based Quantum computing simulator." width="70%">
 </p>
 
 <div align=center>
   <a href="https://pypi.org/project/mentpy"><img src="https://img.shields.io/pypi/v/mentpy"></a>
   <!-- <a href="https://pypi.org/project/mentpy"><img src="https://img.shields.io/pypi/pyversions/mentpy"></a> -->
@@ -28,16 +26,15 @@
   <a href="https://github.com/bestquark/mentpy/actions/workflows/lint.yaml"><img src="https://github.com/bestquark/mentpy/actions/workflows/lint.yaml/badge.svg"></a>
   <a href="https://github.com/bestquark/mentpy/actions/workflows/build.yaml"><img src="https://github.com/bestquark/mentpy/actions/workflows/build.yaml/badge.svg"></a>
   <a href="https://github.com/bestquark/mentpy/actions/workflows/test.yaml"><img src="https://github.com/bestquark/mentpy/actions/workflows/test.yaml/badge.svg"></a>
   <a href="https://codecov.io/gh/bestquark/mentpy"><img src="https://codecov.io/gh/bestquark/mentpy/branch/master/graph/badge.svg?token=3FJML79ZUK"></a> -->
 </div>
 
 The `MentPy` library is an open-source software for simulations of 
-measurement-based quantum computing circuits. Currently, this package is under 
-development and is not ready for public use.
+measurement-based quantum computing circuits. Currently, this package is in its alpha version and many features are still in development.
 
 ## Installation
 
 The `MentPy` library can be installed using `pip` with
 
 ```bash
 pip install mentpy
```

#### html2text {}

```diff
@@ -1,24 +1,23 @@
-Metadata-Version: 2.1 Name: mentpy Version: 0.1.0a4 Summary: A Python library
+Metadata-Version: 2.1 Name: mentpy Version: 0.1.0a5 Summary: A Python library
 for simulating MBQC circuits Home-page: https://github.com/BestQuark/mentpy
 Author: Luis Mantilla Author-email: luismantilla99@outlook.com Description-
-Content-Type: text/markdown License-File: LICENSE :warning: **This library is
-under development.**
+Content-Type: text/markdown License-File: LICENSE
           [MentPy: A Measurement-Based Quantum computing simulator.]
   [https://img.shields.io/pypi/v/mentpy]  [https://img.shields.io/pypi/wheel/
     mentpy] [Documentation_Status]  [https://img.shields.io/twitter/follow/
                  mentpy?label=mentpy&style=flat&logo=twitter]
 The `MentPy` library is an open-source software for simulations of measurement-
-based quantum computing circuits. Currently, this package is under development
-and is not ready for public use. ## Installation The `MentPy` library can be
-installed using `pip` with ```bash pip install mentpy ``` or directly from the
-source code for the latest version with ```bash pip install git+https://
-github.com/BestQuark/mentpy.git ``` ## Usage To simulate a measurement pattern,
-you can use the `mp.PatternSimulator`. ```python import mentpy as mp st =
-mp.templates.grid_cluster(2,4) ps = mp.PatternSimulator(st) output = ps
-(np.random.rand(len(st.outputc))) ``` For visualization of circuits, you can
-use the `mp.draw(st)` function ![image](https://user-
+based quantum computing circuits. Currently, this package is in its alpha
+version and many features are still in development. ## Installation The
+`MentPy` library can be installed using `pip` with ```bash pip install mentpy
+``` or directly from the source code for the latest version with ```bash pip
+install git+https://github.com/BestQuark/mentpy.git ``` ## Usage To simulate a
+measurement pattern, you can use the `mp.PatternSimulator`. ```python import
+mentpy as mp st = mp.templates.grid_cluster(2,4) ps = mp.PatternSimulator(st)
+output = ps(np.random.rand(len(st.outputc))) ``` For visualization of circuits,
+you can use the `mp.draw(st)` function ![image](https://user-
 images.githubusercontent.com/52287586/230715389-bf280971-c841-437d-8772-
 bf59557b0875.png) ## Documentation The documentation for `MentPy` can be found
 here. ## Contributing We welcome contributions to `MentPy`! Please see our
 [contributing guidelines](./CONTRIBUTING.md) for more information. ## License
 `MentPy` is licensed under the [GNU General Public License v3.0](./LICENSE).
```

### Comparing `mentpy-0.1.0a4/mentpy.egg-info/SOURCES.txt` & `mentpy-0.1.0a5/mentpy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mentpy-0.1.0a4/setup.py` & `mentpy-0.1.0a5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-version = "0.1.0a4"
+version = "0.1.0a5"
 
 with open("requirements.txt") as f:
     required_packages = f.read().splitlines()
 
 setup(
     name="mentpy",
     version=version,
```

### Comparing `mentpy-0.1.0a4/tests/test_mbqc_templates.py` & `mentpy-0.1.0a5/tests/test_mbqc_templates.py`

 * *Files identical despite different names*

