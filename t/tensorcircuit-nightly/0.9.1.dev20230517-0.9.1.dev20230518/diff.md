# Comparing `tmp/tensorcircuit-nightly-0.9.1.dev20230517.tar.gz` & `tmp/tensorcircuit-nightly-0.9.1.dev20230518.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tensorcircuit-nightly-0.9.1.dev20230517.tar", last modified: Wed May 17 12:39:48 2023, max compression
+gzip compressed data, was "tensorcircuit-nightly-0.9.1.dev20230518.tar", last modified: Thu May 18 12:41:11 2023, max compression
```

## Comparing `tensorcircuit-nightly-0.9.1.dev20230517.tar` & `tensorcircuit-nightly-0.9.1.dev20230518.tar`

### file list

```diff
@@ -1,137 +1,137 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-17 12:39:48.601394 tensorcircuit-nightly-0.9.1.dev20230517/
--rw-r--r--   0 runner    (1001) docker     (122)    24936 2023-05-17 12:16:27.000000 tensorcircuit-nightly-0.9.1.dev20230517/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (122)     1023 2023-05-17 12:16:27.000000 tensorcircuit-nightly-0.9.1.dev20230517/HISTORY.md
--rw-r--r--   0 runner    (1001) docker     (122)    11358 2023-05-17 12:16:27.000000 tensorcircuit-nightly-0.9.1.dev20230517/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)      132 2023-05-17 12:16:27.000000 tensorcircuit-nightly-0.9.1.dev20230517/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)    21081 2023-05-17 12:39:48.601394 tensorcircuit-nightly-0.9.1.dev20230517/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)    18675 2023-05-17 12:16:27.000000 tensorcircuit-nightly-0.9.1.dev20230517/README.md
--rw-r--r--   0 runner    (1001) docker     (122)     6097 2023-05-17 12:16:27.000000 tensorcircuit-nightly-0.9.1.dev20230517/README_cn.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-17 12:39:48.585394 tensorcircuit-nightly-0.9.1.dev20230517/docs/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-17 12:39:48.589394 tensorcircuit-nightly-0.9.1.dev20230517/docs/source/
--rw-r--r--   0 runner    (1001) docker     (122)     6332 2023-05-17 12:16:27.000000 tensorcircuit-nightly-0.9.1.dev20230517/docs/source/advance.rst
--rw-r--r--   0 runner    (1001) docker     (122)     6308 2023-05-17 12:16:27.000000 tensorcircuit-nightly-0.9.1.dev20230517/docs/source/cnconf.py
--rw-r--r--   0 runner    (1001) docker     (122)     6440 2023-05-17 12:16:27.000000 tensorcircuit-nightly-0.9.1.dev20230517/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (122)     8192 2023-05-17 12:16:27.000000 tensorcircuit-nightly-0.9.1.dev20230517/docs/source/contribution.rst
--rw-r--r--   0 runner    (1001) docker     (122)    10971 2023-05-17 12:16:27.000000 tensorcircuit-nightly-0.9.1.dev20230517/docs/source/faq.rst
--rw-r--r--   0 runner    (1001) docker     (122)     3677 2023-05-17 12:16:27.000000 tensorcircuit-nightly-0.9.1.dev20230517/docs/source/generate_rst.py
--rw-r--r--   0 runner    (1001) docker     (122)     3326 2023-05-17 12:16:27.000000 tensorcircuit-nightly-0.9.1.dev20230517/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (122)    10071 2023-05-17 12:16:27.000000 tensorcircuit-nightly-0.9.1.dev20230517/docs/source/infras.rst
--rw-r--r--   0 runner    (1001) docker     (122)      680 2023-05-17 12:16:27.000000 tensorcircuit-nightly-0.9.1.dev20230517/docs/source/modules.rst
--rw-r--r--   0 runner    (1001) docker     (122)     4334 2023-05-17 12:16:27.000000 tensorcircuit-nightly-0.9.1.dev20230517/docs/source/modules.rst.backup
--rw-r--r--   0 runner    (1001) docker     (122)    27533 2023-05-17 12:16:27.000000 tensorcircuit-nightly-0.9.1.dev20230517/docs/source/quickstart.rst
--rw-r--r--   0 runner    (1001) docker     (122)     8223 2023-05-17 12:16:27.000000 tensorcircuit-nightly-0.9.1.dev20230517/docs/source/sharpbits.rst
--rw-r--r--   0 runner    (1001) docker     (122)      226 2023-05-17 12:16:27.000000 tensorcircuit-nightly-0.9.1.dev20230517/docs/source/textbooktoc.rst
--rw-r--r--   0 runner    (1001) docker     (122)      674 2023-05-17 12:16:27.000000 tensorcircuit-nightly-0.9.1.dev20230517/docs/source/tutorial.rst
--rw-r--r--   0 runner    (1001) docker     (122)      669 2023-05-17 12:16:27.000000 tensorcircuit-nightly-0.9.1.dev20230517/docs/source/tutorial_cn.rst
--rw-r--r--   0 runner    (1001) docker     (122)      509 2023-05-17 12:16:27.000000 tensorcircuit-nightly-0.9.1.dev20230517/docs/source/whitepapertoc.rst
--rw-r--r--   0 runner    (1001) docker     (122)      531 2023-05-17 12:16:27.000000 tensorcircuit-nightly-0.9.1.dev20230517/docs/source/whitepapertoc_cn.rst
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-17 12:39:48.601394 tensorcircuit-nightly-0.9.1.dev20230517/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1059 2023-05-17 12:39:42.000000 tensorcircuit-nightly-0.9.1.dev20230517/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-17 12:39:48.593394 tensorcircuit-nightly-0.9.1.dev20230517/tensorcircuit/
--rw-r--r--   0 runner    (1001) docker     (122)     1460 2023-05-17 12:39:42.000000 tensorcircuit-nightly-0.9.1.dev20230517/tensorcircuit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2901 2023-05-17 12:16:27.000000 tensorcircuit-nightly-0.9.1.dev20230517/tensorcircuit/about.py
--rw-r--r--   0 runner    (1001) docker     (122)    41617 2023-05-17 12:16:27.000000 tensorcircuit-nightly-0.9.1.dev20230517/tensorcircuit/abstractcircuit.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-17 12:39:48.593394 tensorcircuit-nightly-0.9.1.dev20230517/tensorcircuit/applications/
--rw-r--r--   0 runner    (1001) docker     (122)      234 2023-05-17 12:16:27.000000 tensorcircuit-nightly-0.9.1.dev20230517/tensorcircuit/applications/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    34460 2023-05-17 12:16:27.000000 tensorcircuit-nightly-0.9.1.dev20230517/tensorcircuit/applications/dqas.py
--rw-r--r--   0 runner    (1001) docker     (122)    15348 2023-05-17 12:16:27.000000 tensorcircuit-nightly-0.9.1.dev20230517/tensorcircuit/applications/graphdata.py
--rw-r--r--   0 runner    (1001) docker     (122)    18124 2023-05-17 12:16:27.000000 tensorcircuit-nightly-0.9.1.dev20230517/tensorcircuit/applications/layers.py
--rw-r--r--   0 runner    (1001) docker     (122)    14032 2023-05-17 12:16:27.000000 tensorcircuit-nightly-0.9.1.dev20230517/tensorcircuit/applications/utils.py
--rw-r--r--   0 runner    (1001) docker     (122)    36391 2023-05-17 12:16:27.000000 tensorcircuit-nightly-0.9.1.dev20230517/tensorcircuit/applications/vags.py
--rw-r--r--   0 runner    (1001) docker     (122)    15117 2023-05-17 12:16:27.000000 tensorcircuit-nightly-0.9.1.dev20230517/tensorcircuit/applications/van.py
--rw-r--r--   0 runner    (1001) docker     (122)    23416 2023-05-17 12:16:27.000000 tensorcircuit-nightly-0.9.1.dev20230517/tensorcircuit/applications/vqes.py
--rw-r--r--   0 runner    (1001) docker     (122)     8235 2023-05-17 12:16:27.000000 tensorcircuit-nightly-0.9.1.dev20230517/tensorcircuit/asciiart.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-17 12:39:48.593394 tensorcircuit-nightly-0.9.1.dev20230517/tensorcircuit/backends/
--rw-r--r--   0 runner    (1001) docker     (122)       80 2023-05-17 12:16:27.000000 tensorcircuit-nightly-0.9.1.dev20230517/tensorcircuit/backends/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    57621 2023-05-17 12:16:27.000000 tensorcircuit-nightly-0.9.1.dev20230517/tensorcircuit/backends/abstract_backend.py
--rw-r--r--   0 runner    (1001) docker     (122)     1713 2023-05-17 12:16:27.000000 tensorcircuit-nightly-0.9.1.dev20230517/tensorcircuit/backends/backend_factory.py
--rw-r--r--   0 runner    (1001) docker     (122)    14928 2023-05-17 12:16:27.000000 tensorcircuit-nightly-0.9.1.dev20230517/tensorcircuit/backends/cupy_backend.py
--rw-r--r--   0 runner    (1001) docker     (122)    24925 2023-05-17 12:16:27.000000 tensorcircuit-nightly-0.9.1.dev20230517/tensorcircuit/backends/jax_backend.py
--rw-r--r--   0 runner    (1001) docker     (122)     4024 2023-05-17 12:16:27.000000 tensorcircuit-nightly-0.9.1.dev20230517/tensorcircuit/backends/jax_ops.py
--rw-r--r--   0 runner    (1001) docker     (122)    13813 2023-05-17 12:16:27.000000 tensorcircuit-nightly-0.9.1.dev20230517/tensorcircuit/backends/numpy_backend.py
--rw-r--r--   0 runner    (1001) docker     (122)    24148 2023-05-17 12:16:27.000000 tensorcircuit-nightly-0.9.1.dev20230517/tensorcircuit/backends/pytorch_backend.py
--rw-r--r--   0 runner    (1001) docker     (122)     3825 2023-05-17 12:16:27.000000 tensorcircuit-nightly-0.9.1.dev20230517/tensorcircuit/backends/pytorch_ops.py
--rw-r--r--   0 runner    (1001) docker     (122)    31112 2023-05-17 12:16:27.000000 tensorcircuit-nightly-0.9.1.dev20230517/tensorcircuit/backends/tensorflow_backend.py
--rw-r--r--   0 runner    (1001) docker     (122)     3377 2023-05-17 12:16:27.000000 tensorcircuit-nightly-0.9.1.dev20230517/tensorcircuit/backends/tf_ops.py
--rw-r--r--   0 runner    (1001) docker     (122)    34020 2023-05-17 12:16:27.000000 tensorcircuit-nightly-0.9.1.dev20230517/tensorcircuit/basecircuit.py
--rw-r--r--   0 runner    (1001) docker     (122)    28637 2023-05-17 12:16:27.000000 tensorcircuit-nightly-0.9.1.dev20230517/tensorcircuit/channels.py
--rw-r--r--   0 runner    (1001) docker     (122)    36220 2023-05-17 12:16:27.000000 tensorcircuit-nightly-0.9.1.dev20230517/tensorcircuit/circuit.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-17 12:39:48.593394 tensorcircuit-nightly-0.9.1.dev20230517/tensorcircuit/cloud/
--rw-r--r--   0 runner    (1001) docker     (122)       67 2023-05-17 12:16:27.000000 tensorcircuit-nightly-0.9.1.dev20230517/tensorcircuit/cloud/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    14582 2023-05-17 12:16:27.000000 tensorcircuit-nightly-0.9.1.dev20230517/tensorcircuit/cloud/abstraction.py
--rw-r--r--   0 runner    (1001) docker     (122)    17866 2023-05-17 12:16:27.000000 tensorcircuit-nightly-0.9.1.dev20230517/tensorcircuit/cloud/apis.py
--rw-r--r--   0 runner    (1001) docker     (122)       60 2023-05-17 12:16:27.000000 tensorcircuit-nightly-0.9.1.dev20230517/tensorcircuit/cloud/config.py
--rw-r--r--   0 runner    (1001) docker     (122)     2252 2023-05-17 12:16:27.000000 tensorcircuit-nightly-0.9.1.dev20230517/tensorcircuit/cloud/local.py
--rw-r--r--   0 runner    (1001) docker     (122)     2238 2023-05-17 12:16:27.000000 tensorcircuit-nightly-0.9.1.dev20230517/tensorcircuit/cloud/quafu_provider.py
--rw-r--r--   0 runner    (1001) docker     (122)    14222 2023-05-17 12:16:27.000000 tensorcircuit-nightly-0.9.1.dev20230517/tensorcircuit/cloud/tencent.py
--rw-r--r--   0 runner    (1001) docker     (122)     3622 2023-05-17 12:16:27.000000 tensorcircuit-nightly-0.9.1.dev20230517/tensorcircuit/cloud/utils.py
--rw-r--r--   0 runner    (1001) docker     (122)    10737 2023-05-17 12:16:27.000000 tensorcircuit-nightly-0.9.1.dev20230517/tensorcircuit/cloud/wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-17 12:39:48.597394 tensorcircuit-nightly-0.9.1.dev20230517/tensorcircuit/compiler/
--rw-r--r--   0 runner    (1001) docker     (122)      241 2023-05-17 12:16:27.000000 tensorcircuit-nightly-0.9.1.dev20230517/tensorcircuit/compiler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3258 2023-05-17 12:16:27.000000 tensorcircuit-nightly-0.9.1.dev20230517/tensorcircuit/compiler/composed_compiler.py
--rw-r--r--   0 runner    (1001) docker     (122)     6032 2023-05-17 12:16:27.000000 tensorcircuit-nightly-0.9.1.dev20230517/tensorcircuit/compiler/qiskit_compiler.py
--rw-r--r--   0 runner    (1001) docker     (122)     9595 2023-05-17 12:16:27.000000 tensorcircuit-nightly-0.9.1.dev20230517/tensorcircuit/compiler/simple_compiler.py
--rw-r--r--   0 runner    (1001) docker     (122)    29573 2023-05-17 12:16:27.000000 tensorcircuit-nightly-0.9.1.dev20230517/tensorcircuit/cons.py
--rw-r--r--   0 runner    (1001) docker     (122)    13806 2023-05-17 12:16:27.000000 tensorcircuit-nightly-0.9.1.dev20230517/tensorcircuit/densitymatrix.py
--rw-r--r--   0 runner    (1001) docker     (122)    15210 2023-05-17 12:16:27.000000 tensorcircuit-nightly-0.9.1.dev20230517/tensorcircuit/experimental.py
--rw-r--r--   0 runner    (1001) docker     (122)    29016 2023-05-17 12:16:27.000000 tensorcircuit-nightly-0.9.1.dev20230517/tensorcircuit/gates.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-17 12:39:48.597394 tensorcircuit-nightly-0.9.1.dev20230517/tensorcircuit/interfaces/
--rw-r--r--   0 runner    (1001) docker     (122)      545 2023-05-17 12:16:27.000000 tensorcircuit-nightly-0.9.1.dev20230517/tensorcircuit/interfaces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1439 2023-05-17 12:16:27.000000 tensorcircuit-nightly-0.9.1.dev20230517/tensorcircuit/interfaces/numpy.py
--rw-r--r--   0 runner    (1001) docker     (122)     3402 2023-05-17 12:16:27.000000 tensorcircuit-nightly-0.9.1.dev20230517/tensorcircuit/interfaces/scipy.py
--rw-r--r--   0 runner    (1001) docker     (122)     3355 2023-05-17 12:16:27.000000 tensorcircuit-nightly-0.9.1.dev20230517/tensorcircuit/interfaces/tensorflow.py
--rw-r--r--   0 runner    (1001) docker     (122)    10364 2023-05-17 12:16:27.000000 tensorcircuit-nightly-0.9.1.dev20230517/tensorcircuit/interfaces/tensortrans.py
--rw-r--r--   0 runner    (1001) docker     (122)     5117 2023-05-17 12:16:27.000000 tensorcircuit-nightly-0.9.1.dev20230517/tensorcircuit/interfaces/torch.py
--rw-r--r--   0 runner    (1001) docker     (122)    10126 2023-05-17 12:16:27.000000 tensorcircuit-nightly-0.9.1.dev20230517/tensorcircuit/keras.py
--rw-r--r--   0 runner    (1001) docker     (122)    15270 2023-05-17 12:16:27.000000 tensorcircuit-nightly-0.9.1.dev20230517/tensorcircuit/mps_base.py
--rw-r--r--   0 runner    (1001) docker     (122)    34350 2023-05-17 12:16:27.000000 tensorcircuit-nightly-0.9.1.dev20230517/tensorcircuit/mpscircuit.py
--rw-r--r--   0 runner    (1001) docker     (122)    11861 2023-05-17 12:16:27.000000 tensorcircuit-nightly-0.9.1.dev20230517/tensorcircuit/noisemodel.py
--rw-r--r--   0 runner    (1001) docker     (122)    82850 2023-05-17 12:16:27.000000 tensorcircuit-nightly-0.9.1.dev20230517/tensorcircuit/quantum.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-17 12:39:48.597394 tensorcircuit-nightly-0.9.1.dev20230517/tensorcircuit/results/
--rw-r--r--   0 runner    (1001) docker     (122)       89 2023-05-17 12:16:27.000000 tensorcircuit-nightly-0.9.1.dev20230517/tensorcircuit/results/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3435 2023-05-17 12:16:27.000000 tensorcircuit-nightly-0.9.1.dev20230517/tensorcircuit/results/counts.py
--rw-r--r--   0 runner    (1001) docker     (122)    31362 2023-05-17 12:16:27.000000 tensorcircuit-nightly-0.9.1.dev20230517/tensorcircuit/results/readout_mitigation.py
--rw-r--r--   0 runner    (1001) docker     (122)     9413 2023-05-17 12:16:27.000000 tensorcircuit-nightly-0.9.1.dev20230517/tensorcircuit/simplify.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-17 12:39:48.597394 tensorcircuit-nightly-0.9.1.dev20230517/tensorcircuit/templates/
--rw-r--r--   0 runner    (1001) docker     (122)      111 2023-05-17 12:16:27.000000 tensorcircuit-nightly-0.9.1.dev20230517/tensorcircuit/templates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6158 2023-05-17 12:16:27.000000 tensorcircuit-nightly-0.9.1.dev20230517/tensorcircuit/templates/blocks.py
--rw-r--r--   0 runner    (1001) docker     (122)     1061 2023-05-17 12:16:27.000000 tensorcircuit-nightly-0.9.1.dev20230517/tensorcircuit/templates/chems.py
--rw-r--r--   0 runner    (1001) docker     (122)     1933 2023-05-17 12:16:27.000000 tensorcircuit-nightly-0.9.1.dev20230517/tensorcircuit/templates/dataset.py
--rw-r--r--   0 runner    (1001) docker     (122)     5811 2023-05-17 12:16:27.000000 tensorcircuit-nightly-0.9.1.dev20230517/tensorcircuit/templates/ensemble.py
--rw-r--r--   0 runner    (1001) docker     (122)     3934 2023-05-17 12:16:27.000000 tensorcircuit-nightly-0.9.1.dev20230517/tensorcircuit/templates/graphs.py
--rw-r--r--   0 runner    (1001) docker     (122)    10942 2023-05-17 12:16:27.000000 tensorcircuit-nightly-0.9.1.dev20230517/tensorcircuit/templates/measurements.py
--rw-r--r--   0 runner    (1001) docker     (122)     4621 2023-05-17 12:16:27.000000 tensorcircuit-nightly-0.9.1.dev20230517/tensorcircuit/torchnn.py
--rw-r--r--   0 runner    (1001) docker     (122)    27335 2023-05-17 12:16:27.000000 tensorcircuit-nightly-0.9.1.dev20230517/tensorcircuit/translation.py
--rw-r--r--   0 runner    (1001) docker     (122)     7060 2023-05-17 12:16:27.000000 tensorcircuit-nightly-0.9.1.dev20230517/tensorcircuit/utils.py
--rw-r--r--   0 runner    (1001) docker     (122)    12195 2023-05-17 12:16:27.000000 tensorcircuit-nightly-0.9.1.dev20230517/tensorcircuit/vis.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-17 12:39:48.597394 tensorcircuit-nightly-0.9.1.dev20230517/tensorcircuit_nightly.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)    21081 2023-05-17 12:39:48.000000 tensorcircuit-nightly-0.9.1.dev20230517/tensorcircuit_nightly.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     3561 2023-05-17 12:39:48.000000 tensorcircuit-nightly-0.9.1.dev20230517/tensorcircuit_nightly.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-17 12:39:48.000000 tensorcircuit-nightly-0.9.1.dev20230517/tensorcircuit_nightly.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      110 2023-05-17 12:39:48.000000 tensorcircuit-nightly-0.9.1.dev20230517/tensorcircuit_nightly.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       20 2023-05-17 12:39:48.000000 tensorcircuit-nightly-0.9.1.dev20230517/tensorcircuit_nightly.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-17 12:39:48.601394 tensorcircuit-nightly-0.9.1.dev20230517/tests/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-17 12:16:27.000000 tensorcircuit-nightly-0.9.1.dev20230517/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1457 2023-05-17 12:16:27.000000 tensorcircuit-nightly-0.9.1.dev20230517/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (122)    33394 2023-05-17 12:16:27.000000 tensorcircuit-nightly-0.9.1.dev20230517/tests/test_backends.py
--rw-r--r--   0 runner    (1001) docker     (122)     3805 2023-05-17 12:16:27.000000 tensorcircuit-nightly-0.9.1.dev20230517/tests/test_calibrating.py
--rw-r--r--   0 runner    (1001) docker     (122)    11237 2023-05-17 12:16:27.000000 tensorcircuit-nightly-0.9.1.dev20230517/tests/test_channels.py
--rw-r--r--   0 runner    (1001) docker     (122)    47017 2023-05-17 12:16:27.000000 tensorcircuit-nightly-0.9.1.dev20230517/tests/test_circuit.py
--rw-r--r--   0 runner    (1001) docker     (122)     5445 2023-05-17 12:16:27.000000 tensorcircuit-nightly-0.9.1.dev20230517/tests/test_cloud.py
--rw-r--r--   0 runner    (1001) docker     (122)     3419 2023-05-17 12:16:27.000000 tensorcircuit-nightly-0.9.1.dev20230517/tests/test_compiler.py
--rw-r--r--   0 runner    (1001) docker     (122)    17232 2023-05-17 12:16:27.000000 tensorcircuit-nightly-0.9.1.dev20230517/tests/test_dmcircuit.py
--rw-r--r--   0 runner    (1001) docker     (122)     1974 2023-05-17 12:16:27.000000 tensorcircuit-nightly-0.9.1.dev20230517/tests/test_ensemble.py
--rw-r--r--   0 runner    (1001) docker     (122)     4593 2023-05-17 12:16:27.000000 tensorcircuit-nightly-0.9.1.dev20230517/tests/test_gates.py
--rw-r--r--   0 runner    (1001) docker     (122)    13220 2023-05-17 12:16:27.000000 tensorcircuit-nightly-0.9.1.dev20230517/tests/test_interfaces.py
--rw-r--r--   0 runner    (1001) docker     (122)     4656 2023-05-17 12:16:27.000000 tensorcircuit-nightly-0.9.1.dev20230517/tests/test_keras.py
--rw-r--r--   0 runner    (1001) docker     (122)     6639 2023-05-17 12:16:27.000000 tensorcircuit-nightly-0.9.1.dev20230517/tests/test_miscs.py
--rw-r--r--   0 runner    (1001) docker     (122)    10552 2023-05-17 12:16:27.000000 tensorcircuit-nightly-0.9.1.dev20230517/tests/test_mpscircuit.py
--rw-r--r--   0 runner    (1001) docker     (122)     5637 2023-05-17 12:16:27.000000 tensorcircuit-nightly-0.9.1.dev20230517/tests/test_noisemodel.py
--rw-r--r--   0 runner    (1001) docker     (122)      753 2023-05-17 12:16:27.000000 tensorcircuit-nightly-0.9.1.dev20230517/tests/test_qaoa.py
--rw-r--r--   0 runner    (1001) docker     (122)    16823 2023-05-17 12:16:27.000000 tensorcircuit-nightly-0.9.1.dev20230517/tests/test_quantum.py
--rw-r--r--   0 runner    (1001) docker     (122)     1245 2023-05-17 12:16:27.000000 tensorcircuit-nightly-0.9.1.dev20230517/tests/test_quantum_attr.py
--rw-r--r--   0 runner    (1001) docker     (122)    11050 2023-05-17 12:16:27.000000 tensorcircuit-nightly-0.9.1.dev20230517/tests/test_results.py
--rw-r--r--   0 runner    (1001) docker     (122)     1175 2023-05-17 12:16:27.000000 tensorcircuit-nightly-0.9.1.dev20230517/tests/test_simplify.py
--rw-r--r--   0 runner    (1001) docker     (122)     5962 2023-05-17 12:16:27.000000 tensorcircuit-nightly-0.9.1.dev20230517/tests/test_templates.py
--rw-r--r--   0 runner    (1001) docker     (122)     2823 2023-05-17 12:16:27.000000 tensorcircuit-nightly-0.9.1.dev20230517/tests/test_torchnn.py
--rw-r--r--   0 runner    (1001) docker     (122)     3163 2023-05-17 12:16:27.000000 tensorcircuit-nightly-0.9.1.dev20230517/tests/test_van.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-18 12:41:11.041173 tensorcircuit-nightly-0.9.1.dev20230518/
+-rw-r--r--   0 runner    (1001) docker     (122)    25020 2023-05-18 12:16:18.000000 tensorcircuit-nightly-0.9.1.dev20230518/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (122)     1023 2023-05-18 12:16:18.000000 tensorcircuit-nightly-0.9.1.dev20230518/HISTORY.md
+-rw-r--r--   0 runner    (1001) docker     (122)    11358 2023-05-18 12:16:18.000000 tensorcircuit-nightly-0.9.1.dev20230518/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)      132 2023-05-18 12:16:18.000000 tensorcircuit-nightly-0.9.1.dev20230518/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)    21081 2023-05-18 12:41:11.041173 tensorcircuit-nightly-0.9.1.dev20230518/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)    18675 2023-05-18 12:16:18.000000 tensorcircuit-nightly-0.9.1.dev20230518/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)     6097 2023-05-18 12:16:18.000000 tensorcircuit-nightly-0.9.1.dev20230518/README_cn.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-18 12:41:11.021173 tensorcircuit-nightly-0.9.1.dev20230518/docs/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-18 12:41:11.025173 tensorcircuit-nightly-0.9.1.dev20230518/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (122)     6332 2023-05-18 12:16:18.000000 tensorcircuit-nightly-0.9.1.dev20230518/docs/source/advance.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     6308 2023-05-18 12:16:18.000000 tensorcircuit-nightly-0.9.1.dev20230518/docs/source/cnconf.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6440 2023-05-18 12:16:18.000000 tensorcircuit-nightly-0.9.1.dev20230518/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8192 2023-05-18 12:16:18.000000 tensorcircuit-nightly-0.9.1.dev20230518/docs/source/contribution.rst
+-rw-r--r--   0 runner    (1001) docker     (122)    10971 2023-05-18 12:16:18.000000 tensorcircuit-nightly-0.9.1.dev20230518/docs/source/faq.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     3677 2023-05-18 12:16:18.000000 tensorcircuit-nightly-0.9.1.dev20230518/docs/source/generate_rst.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3326 2023-05-18 12:16:18.000000 tensorcircuit-nightly-0.9.1.dev20230518/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (122)    10071 2023-05-18 12:16:18.000000 tensorcircuit-nightly-0.9.1.dev20230518/docs/source/infras.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      680 2023-05-18 12:16:18.000000 tensorcircuit-nightly-0.9.1.dev20230518/docs/source/modules.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     4334 2023-05-18 12:16:18.000000 tensorcircuit-nightly-0.9.1.dev20230518/docs/source/modules.rst.backup
+-rw-r--r--   0 runner    (1001) docker     (122)    27533 2023-05-18 12:16:18.000000 tensorcircuit-nightly-0.9.1.dev20230518/docs/source/quickstart.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     8223 2023-05-18 12:16:18.000000 tensorcircuit-nightly-0.9.1.dev20230518/docs/source/sharpbits.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      226 2023-05-18 12:16:18.000000 tensorcircuit-nightly-0.9.1.dev20230518/docs/source/textbooktoc.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      674 2023-05-18 12:16:18.000000 tensorcircuit-nightly-0.9.1.dev20230518/docs/source/tutorial.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      669 2023-05-18 12:16:18.000000 tensorcircuit-nightly-0.9.1.dev20230518/docs/source/tutorial_cn.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      509 2023-05-18 12:16:18.000000 tensorcircuit-nightly-0.9.1.dev20230518/docs/source/whitepapertoc.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      531 2023-05-18 12:16:18.000000 tensorcircuit-nightly-0.9.1.dev20230518/docs/source/whitepapertoc_cn.rst
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-18 12:41:11.041173 tensorcircuit-nightly-0.9.1.dev20230518/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1059 2023-05-18 12:41:04.000000 tensorcircuit-nightly-0.9.1.dev20230518/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-18 12:41:11.029173 tensorcircuit-nightly-0.9.1.dev20230518/tensorcircuit/
+-rw-r--r--   0 runner    (1001) docker     (122)     1460 2023-05-18 12:41:04.000000 tensorcircuit-nightly-0.9.1.dev20230518/tensorcircuit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2901 2023-05-18 12:16:18.000000 tensorcircuit-nightly-0.9.1.dev20230518/tensorcircuit/about.py
+-rw-r--r--   0 runner    (1001) docker     (122)    42135 2023-05-18 12:16:18.000000 tensorcircuit-nightly-0.9.1.dev20230518/tensorcircuit/abstractcircuit.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-18 12:41:11.029173 tensorcircuit-nightly-0.9.1.dev20230518/tensorcircuit/applications/
+-rw-r--r--   0 runner    (1001) docker     (122)      234 2023-05-18 12:16:18.000000 tensorcircuit-nightly-0.9.1.dev20230518/tensorcircuit/applications/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    34460 2023-05-18 12:16:18.000000 tensorcircuit-nightly-0.9.1.dev20230518/tensorcircuit/applications/dqas.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15348 2023-05-18 12:16:18.000000 tensorcircuit-nightly-0.9.1.dev20230518/tensorcircuit/applications/graphdata.py
+-rw-r--r--   0 runner    (1001) docker     (122)    18124 2023-05-18 12:16:18.000000 tensorcircuit-nightly-0.9.1.dev20230518/tensorcircuit/applications/layers.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14032 2023-05-18 12:16:18.000000 tensorcircuit-nightly-0.9.1.dev20230518/tensorcircuit/applications/utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)    36391 2023-05-18 12:16:18.000000 tensorcircuit-nightly-0.9.1.dev20230518/tensorcircuit/applications/vags.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15117 2023-05-18 12:16:18.000000 tensorcircuit-nightly-0.9.1.dev20230518/tensorcircuit/applications/van.py
+-rw-r--r--   0 runner    (1001) docker     (122)    23416 2023-05-18 12:16:18.000000 tensorcircuit-nightly-0.9.1.dev20230518/tensorcircuit/applications/vqes.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8235 2023-05-18 12:16:18.000000 tensorcircuit-nightly-0.9.1.dev20230518/tensorcircuit/asciiart.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-18 12:41:11.033173 tensorcircuit-nightly-0.9.1.dev20230518/tensorcircuit/backends/
+-rw-r--r--   0 runner    (1001) docker     (122)       80 2023-05-18 12:16:18.000000 tensorcircuit-nightly-0.9.1.dev20230518/tensorcircuit/backends/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    57621 2023-05-18 12:16:18.000000 tensorcircuit-nightly-0.9.1.dev20230518/tensorcircuit/backends/abstract_backend.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1713 2023-05-18 12:16:18.000000 tensorcircuit-nightly-0.9.1.dev20230518/tensorcircuit/backends/backend_factory.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14928 2023-05-18 12:16:18.000000 tensorcircuit-nightly-0.9.1.dev20230518/tensorcircuit/backends/cupy_backend.py
+-rw-r--r--   0 runner    (1001) docker     (122)    24925 2023-05-18 12:16:18.000000 tensorcircuit-nightly-0.9.1.dev20230518/tensorcircuit/backends/jax_backend.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4024 2023-05-18 12:16:18.000000 tensorcircuit-nightly-0.9.1.dev20230518/tensorcircuit/backends/jax_ops.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13813 2023-05-18 12:16:18.000000 tensorcircuit-nightly-0.9.1.dev20230518/tensorcircuit/backends/numpy_backend.py
+-rw-r--r--   0 runner    (1001) docker     (122)    24148 2023-05-18 12:16:18.000000 tensorcircuit-nightly-0.9.1.dev20230518/tensorcircuit/backends/pytorch_backend.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3825 2023-05-18 12:16:18.000000 tensorcircuit-nightly-0.9.1.dev20230518/tensorcircuit/backends/pytorch_ops.py
+-rw-r--r--   0 runner    (1001) docker     (122)    31112 2023-05-18 12:16:18.000000 tensorcircuit-nightly-0.9.1.dev20230518/tensorcircuit/backends/tensorflow_backend.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3377 2023-05-18 12:16:18.000000 tensorcircuit-nightly-0.9.1.dev20230518/tensorcircuit/backends/tf_ops.py
+-rw-r--r--   0 runner    (1001) docker     (122)    34020 2023-05-18 12:16:18.000000 tensorcircuit-nightly-0.9.1.dev20230518/tensorcircuit/basecircuit.py
+-rw-r--r--   0 runner    (1001) docker     (122)    28637 2023-05-18 12:16:18.000000 tensorcircuit-nightly-0.9.1.dev20230518/tensorcircuit/channels.py
+-rw-r--r--   0 runner    (1001) docker     (122)    36220 2023-05-18 12:16:18.000000 tensorcircuit-nightly-0.9.1.dev20230518/tensorcircuit/circuit.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-18 12:41:11.033173 tensorcircuit-nightly-0.9.1.dev20230518/tensorcircuit/cloud/
+-rw-r--r--   0 runner    (1001) docker     (122)       67 2023-05-18 12:16:18.000000 tensorcircuit-nightly-0.9.1.dev20230518/tensorcircuit/cloud/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14582 2023-05-18 12:16:18.000000 tensorcircuit-nightly-0.9.1.dev20230518/tensorcircuit/cloud/abstraction.py
+-rw-r--r--   0 runner    (1001) docker     (122)    17866 2023-05-18 12:16:18.000000 tensorcircuit-nightly-0.9.1.dev20230518/tensorcircuit/cloud/apis.py
+-rw-r--r--   0 runner    (1001) docker     (122)       60 2023-05-18 12:16:18.000000 tensorcircuit-nightly-0.9.1.dev20230518/tensorcircuit/cloud/config.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2252 2023-05-18 12:16:18.000000 tensorcircuit-nightly-0.9.1.dev20230518/tensorcircuit/cloud/local.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2238 2023-05-18 12:16:18.000000 tensorcircuit-nightly-0.9.1.dev20230518/tensorcircuit/cloud/quafu_provider.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14222 2023-05-18 12:16:18.000000 tensorcircuit-nightly-0.9.1.dev20230518/tensorcircuit/cloud/tencent.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3622 2023-05-18 12:16:18.000000 tensorcircuit-nightly-0.9.1.dev20230518/tensorcircuit/cloud/utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10737 2023-05-18 12:16:18.000000 tensorcircuit-nightly-0.9.1.dev20230518/tensorcircuit/cloud/wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-18 12:41:11.033173 tensorcircuit-nightly-0.9.1.dev20230518/tensorcircuit/compiler/
+-rw-r--r--   0 runner    (1001) docker     (122)      241 2023-05-18 12:16:18.000000 tensorcircuit-nightly-0.9.1.dev20230518/tensorcircuit/compiler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3258 2023-05-18 12:16:18.000000 tensorcircuit-nightly-0.9.1.dev20230518/tensorcircuit/compiler/composed_compiler.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6032 2023-05-18 12:16:18.000000 tensorcircuit-nightly-0.9.1.dev20230518/tensorcircuit/compiler/qiskit_compiler.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9595 2023-05-18 12:16:18.000000 tensorcircuit-nightly-0.9.1.dev20230518/tensorcircuit/compiler/simple_compiler.py
+-rw-r--r--   0 runner    (1001) docker     (122)    29573 2023-05-18 12:16:18.000000 tensorcircuit-nightly-0.9.1.dev20230518/tensorcircuit/cons.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13806 2023-05-18 12:16:18.000000 tensorcircuit-nightly-0.9.1.dev20230518/tensorcircuit/densitymatrix.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15210 2023-05-18 12:16:18.000000 tensorcircuit-nightly-0.9.1.dev20230518/tensorcircuit/experimental.py
+-rw-r--r--   0 runner    (1001) docker     (122)    29016 2023-05-18 12:16:18.000000 tensorcircuit-nightly-0.9.1.dev20230518/tensorcircuit/gates.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-18 12:41:11.033173 tensorcircuit-nightly-0.9.1.dev20230518/tensorcircuit/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (122)      545 2023-05-18 12:16:18.000000 tensorcircuit-nightly-0.9.1.dev20230518/tensorcircuit/interfaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1439 2023-05-18 12:16:18.000000 tensorcircuit-nightly-0.9.1.dev20230518/tensorcircuit/interfaces/numpy.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3402 2023-05-18 12:16:18.000000 tensorcircuit-nightly-0.9.1.dev20230518/tensorcircuit/interfaces/scipy.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3355 2023-05-18 12:16:18.000000 tensorcircuit-nightly-0.9.1.dev20230518/tensorcircuit/interfaces/tensorflow.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10364 2023-05-18 12:16:18.000000 tensorcircuit-nightly-0.9.1.dev20230518/tensorcircuit/interfaces/tensortrans.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5117 2023-05-18 12:16:18.000000 tensorcircuit-nightly-0.9.1.dev20230518/tensorcircuit/interfaces/torch.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10126 2023-05-18 12:16:18.000000 tensorcircuit-nightly-0.9.1.dev20230518/tensorcircuit/keras.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15270 2023-05-18 12:16:18.000000 tensorcircuit-nightly-0.9.1.dev20230518/tensorcircuit/mps_base.py
+-rw-r--r--   0 runner    (1001) docker     (122)    34350 2023-05-18 12:16:18.000000 tensorcircuit-nightly-0.9.1.dev20230518/tensorcircuit/mpscircuit.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11861 2023-05-18 12:16:18.000000 tensorcircuit-nightly-0.9.1.dev20230518/tensorcircuit/noisemodel.py
+-rw-r--r--   0 runner    (1001) docker     (122)    82850 2023-05-18 12:16:18.000000 tensorcircuit-nightly-0.9.1.dev20230518/tensorcircuit/quantum.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-18 12:41:11.033173 tensorcircuit-nightly-0.9.1.dev20230518/tensorcircuit/results/
+-rw-r--r--   0 runner    (1001) docker     (122)       89 2023-05-18 12:16:18.000000 tensorcircuit-nightly-0.9.1.dev20230518/tensorcircuit/results/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3435 2023-05-18 12:16:18.000000 tensorcircuit-nightly-0.9.1.dev20230518/tensorcircuit/results/counts.py
+-rw-r--r--   0 runner    (1001) docker     (122)    31362 2023-05-18 12:16:18.000000 tensorcircuit-nightly-0.9.1.dev20230518/tensorcircuit/results/readout_mitigation.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9413 2023-05-18 12:16:18.000000 tensorcircuit-nightly-0.9.1.dev20230518/tensorcircuit/simplify.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-18 12:41:11.037173 tensorcircuit-nightly-0.9.1.dev20230518/tensorcircuit/templates/
+-rw-r--r--   0 runner    (1001) docker     (122)      111 2023-05-18 12:16:18.000000 tensorcircuit-nightly-0.9.1.dev20230518/tensorcircuit/templates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6158 2023-05-18 12:16:18.000000 tensorcircuit-nightly-0.9.1.dev20230518/tensorcircuit/templates/blocks.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1061 2023-05-18 12:16:18.000000 tensorcircuit-nightly-0.9.1.dev20230518/tensorcircuit/templates/chems.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1933 2023-05-18 12:16:18.000000 tensorcircuit-nightly-0.9.1.dev20230518/tensorcircuit/templates/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5811 2023-05-18 12:16:18.000000 tensorcircuit-nightly-0.9.1.dev20230518/tensorcircuit/templates/ensemble.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3934 2023-05-18 12:16:18.000000 tensorcircuit-nightly-0.9.1.dev20230518/tensorcircuit/templates/graphs.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10942 2023-05-18 12:16:18.000000 tensorcircuit-nightly-0.9.1.dev20230518/tensorcircuit/templates/measurements.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4621 2023-05-18 12:16:18.000000 tensorcircuit-nightly-0.9.1.dev20230518/tensorcircuit/torchnn.py
+-rw-r--r--   0 runner    (1001) docker     (122)    27335 2023-05-18 12:16:18.000000 tensorcircuit-nightly-0.9.1.dev20230518/tensorcircuit/translation.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7060 2023-05-18 12:16:18.000000 tensorcircuit-nightly-0.9.1.dev20230518/tensorcircuit/utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12195 2023-05-18 12:16:18.000000 tensorcircuit-nightly-0.9.1.dev20230518/tensorcircuit/vis.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-18 12:41:11.037173 tensorcircuit-nightly-0.9.1.dev20230518/tensorcircuit_nightly.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)    21081 2023-05-18 12:41:10.000000 tensorcircuit-nightly-0.9.1.dev20230518/tensorcircuit_nightly.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     3561 2023-05-18 12:41:10.000000 tensorcircuit-nightly-0.9.1.dev20230518/tensorcircuit_nightly.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-18 12:41:10.000000 tensorcircuit-nightly-0.9.1.dev20230518/tensorcircuit_nightly.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      110 2023-05-18 12:41:10.000000 tensorcircuit-nightly-0.9.1.dev20230518/tensorcircuit_nightly.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       20 2023-05-18 12:41:10.000000 tensorcircuit-nightly-0.9.1.dev20230518/tensorcircuit_nightly.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-18 12:41:11.041173 tensorcircuit-nightly-0.9.1.dev20230518/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-18 12:16:18.000000 tensorcircuit-nightly-0.9.1.dev20230518/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1457 2023-05-18 12:16:18.000000 tensorcircuit-nightly-0.9.1.dev20230518/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (122)    33735 2023-05-18 12:16:18.000000 tensorcircuit-nightly-0.9.1.dev20230518/tests/test_backends.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3805 2023-05-18 12:16:18.000000 tensorcircuit-nightly-0.9.1.dev20230518/tests/test_calibrating.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11237 2023-05-18 12:16:18.000000 tensorcircuit-nightly-0.9.1.dev20230518/tests/test_channels.py
+-rw-r--r--   0 runner    (1001) docker     (122)    47235 2023-05-18 12:16:18.000000 tensorcircuit-nightly-0.9.1.dev20230518/tests/test_circuit.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5445 2023-05-18 12:16:18.000000 tensorcircuit-nightly-0.9.1.dev20230518/tests/test_cloud.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3419 2023-05-18 12:16:18.000000 tensorcircuit-nightly-0.9.1.dev20230518/tests/test_compiler.py
+-rw-r--r--   0 runner    (1001) docker     (122)    17232 2023-05-18 12:16:18.000000 tensorcircuit-nightly-0.9.1.dev20230518/tests/test_dmcircuit.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1974 2023-05-18 12:16:18.000000 tensorcircuit-nightly-0.9.1.dev20230518/tests/test_ensemble.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4593 2023-05-18 12:16:18.000000 tensorcircuit-nightly-0.9.1.dev20230518/tests/test_gates.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13220 2023-05-18 12:16:18.000000 tensorcircuit-nightly-0.9.1.dev20230518/tests/test_interfaces.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4656 2023-05-18 12:16:18.000000 tensorcircuit-nightly-0.9.1.dev20230518/tests/test_keras.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6639 2023-05-18 12:16:18.000000 tensorcircuit-nightly-0.9.1.dev20230518/tests/test_miscs.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10552 2023-05-18 12:16:18.000000 tensorcircuit-nightly-0.9.1.dev20230518/tests/test_mpscircuit.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5637 2023-05-18 12:16:18.000000 tensorcircuit-nightly-0.9.1.dev20230518/tests/test_noisemodel.py
+-rw-r--r--   0 runner    (1001) docker     (122)      753 2023-05-18 12:16:18.000000 tensorcircuit-nightly-0.9.1.dev20230518/tests/test_qaoa.py
+-rw-r--r--   0 runner    (1001) docker     (122)    16823 2023-05-18 12:16:18.000000 tensorcircuit-nightly-0.9.1.dev20230518/tests/test_quantum.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1245 2023-05-18 12:16:18.000000 tensorcircuit-nightly-0.9.1.dev20230518/tests/test_quantum_attr.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11050 2023-05-18 12:16:18.000000 tensorcircuit-nightly-0.9.1.dev20230518/tests/test_results.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1175 2023-05-18 12:16:18.000000 tensorcircuit-nightly-0.9.1.dev20230518/tests/test_simplify.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5962 2023-05-18 12:16:18.000000 tensorcircuit-nightly-0.9.1.dev20230518/tests/test_templates.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2823 2023-05-18 12:16:18.000000 tensorcircuit-nightly-0.9.1.dev20230518/tests/test_torchnn.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3163 2023-05-18 12:16:18.000000 tensorcircuit-nightly-0.9.1.dev20230518/tests/test_van.py
```

### Comparing `tensorcircuit-nightly-0.9.1.dev20230517/CHANGELOG.md` & `tensorcircuit-nightly-0.9.1.dev20230518/CHANGELOG.md`

 * *Files 0% similar despite different names*

```diff
@@ -2,14 +2,16 @@
 
 ## Unreleased
 
 ### Added
 
 - `c.measure_instruction(*qubits)` now supports multiple ints specified at the same time
 
+- `c.expectation_ps()` now also supports `ps` argument directly (pauli structures)
+
 ### Fixed
 
 - `tc.results.counts.plot_histogram` now can dispatch kws to corresponding qiskit method
 
 - New implementation for `c.inverse()` to partially avoid unrecognized gate name issue
 
 - Fixed bug for `batch_expectation_ps` for jax backend
```

### Comparing `tensorcircuit-nightly-0.9.1.dev20230517/HISTORY.md` & `tensorcircuit-nightly-0.9.1.dev20230518/HISTORY.md`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230517/LICENSE` & `tensorcircuit-nightly-0.9.1.dev20230518/LICENSE`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230517/PKG-INFO` & `tensorcircuit-nightly-0.9.1.dev20230518/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tensorcircuit-nightly
-Version: 0.9.1.dev20230517
+Version: 0.9.1.dev20230518
 Summary: nightly release for tensorcircuit
 Home-page: https://github.com/refraction-ray/tensorcircuit-dev
 Author: TensorCircuit Authors
 Author-email: znfesnpbh.tc@gmail.com
 License: UNKNOWN
 Description: <p align="center">
           <a href="https://github.com/tencent-quantum-lab/tensorcircuit">
```

### Comparing `tensorcircuit-nightly-0.9.1.dev20230517/README.md` & `tensorcircuit-nightly-0.9.1.dev20230518/README.md`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230517/README_cn.md` & `tensorcircuit-nightly-0.9.1.dev20230518/README_cn.md`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230517/docs/source/advance.rst` & `tensorcircuit-nightly-0.9.1.dev20230518/docs/source/advance.rst`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230517/docs/source/cnconf.py` & `tensorcircuit-nightly-0.9.1.dev20230518/docs/source/cnconf.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230517/docs/source/conf.py` & `tensorcircuit-nightly-0.9.1.dev20230518/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230517/docs/source/contribution.rst` & `tensorcircuit-nightly-0.9.1.dev20230518/docs/source/contribution.rst`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230517/docs/source/faq.rst` & `tensorcircuit-nightly-0.9.1.dev20230518/docs/source/faq.rst`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230517/docs/source/generate_rst.py` & `tensorcircuit-nightly-0.9.1.dev20230518/docs/source/generate_rst.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230517/docs/source/index.rst` & `tensorcircuit-nightly-0.9.1.dev20230518/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230517/docs/source/infras.rst` & `tensorcircuit-nightly-0.9.1.dev20230518/docs/source/infras.rst`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230517/docs/source/modules.rst` & `tensorcircuit-nightly-0.9.1.dev20230518/docs/source/modules.rst`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230517/docs/source/modules.rst.backup` & `tensorcircuit-nightly-0.9.1.dev20230518/docs/source/modules.rst.backup`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230517/docs/source/quickstart.rst` & `tensorcircuit-nightly-0.9.1.dev20230518/docs/source/quickstart.rst`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230517/docs/source/sharpbits.rst` & `tensorcircuit-nightly-0.9.1.dev20230518/docs/source/sharpbits.rst`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230517/docs/source/tutorial.rst` & `tensorcircuit-nightly-0.9.1.dev20230518/docs/source/tutorial.rst`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230517/docs/source/tutorial_cn.rst` & `tensorcircuit-nightly-0.9.1.dev20230518/docs/source/tutorial_cn.rst`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230517/docs/source/whitepapertoc_cn.rst` & `tensorcircuit-nightly-0.9.1.dev20230518/docs/source/whitepapertoc_cn.rst`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230517/setup.py` & `tensorcircuit-nightly-0.9.1.dev20230518/setup.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230517/tensorcircuit/__init__.py` & `tensorcircuit-nightly-0.9.1.dev20230518/tensorcircuit/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "0.9.1.dev20230517"
+__version__ = "0.9.1.dev20230518"
 __author__ = "TensorCircuit Authors"
 __creator__ = "refraction-ray"
 
 from .utils import gpu_memory_share
 
 gpu_memory_share()
```

### Comparing `tensorcircuit-nightly-0.9.1.dev20230517/tensorcircuit/about.py` & `tensorcircuit-nightly-0.9.1.dev20230518/tensorcircuit/about.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230517/tensorcircuit/abstractcircuit.py` & `tensorcircuit-nightly-0.9.1.dev20230518/tensorcircuit/abstractcircuit.py`

 * *Files 2% similar despite different names*

```diff
@@ -1156,14 +1156,15 @@
         raise NotImplementedError
 
     def expectation_ps(
         self,
         x: Optional[Sequence[int]] = None,
         y: Optional[Sequence[int]] = None,
         z: Optional[Sequence[int]] = None,
+        ps: Optional[Sequence[int]] = None,
         reuse: bool = True,
         noise_conf: Optional[Any] = None,
         nmc: int = 1000,
         status: Optional[Tensor] = None,
         **kws: Any,
     ) -> Tensor:
         """
@@ -1194,27 +1195,39 @@
 
         :param x: sites to apply X gate, defaults to None
         :type x: Optional[Sequence[int]], optional
         :param y: sites to apply Y gate, defaults to None
         :type y: Optional[Sequence[int]], optional
         :param z: sites to apply Z gate, defaults to None
         :type z: Optional[Sequence[int]], optional
+        :param ps: or one can apply a ps structures instead of ``x``, ``y``, ``z``,
+            e.g. [0, 1, 3, 0, 2, 2] for X_1Z_2Y_4Y_5
+            defaults to None, ``ps`` can overwrite ``x``, ``y`` and ``z``
+        :type ps: Optional[Sequence[int]], optional
         :param reuse: whether to cache and reuse the wavefunction, defaults to True
         :type reuse: bool, optional
         :param noise_conf: Noise Configuration, defaults to None
         :type noise_conf: Optional[NoiseConf], optional
         :param nmc: repetition time for Monte Carlo sampling for noisfy calculation, defaults to 1000
         :type nmc: int, optional
         :param status: external randomness given by tensor uniformly from [0, 1], defaults to None,
             used for noisfy circuit sampling
         :type status: Optional[Tensor], optional
         :return: Expectation value
         :rtype: Tensor
         """
         obs = []
+        if ps is not None:
+            from .quantum import ps2xyz
+
+            d = ps2xyz(ps)  # type: ignore
+            x = d.get("x", None)
+            y = d.get("y", None)
+            z = d.get("z", None)
+
         if x is not None:
             for i in x:
                 obs.append([gates.x(), [i]])  # type: ignore
         if y is not None:
             for i in y:
                 obs.append([gates.y(), [i]])  # type: ignore
         if z is not None:
```

### Comparing `tensorcircuit-nightly-0.9.1.dev20230517/tensorcircuit/applications/dqas.py` & `tensorcircuit-nightly-0.9.1.dev20230518/tensorcircuit/applications/dqas.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230517/tensorcircuit/applications/graphdata.py` & `tensorcircuit-nightly-0.9.1.dev20230518/tensorcircuit/applications/graphdata.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230517/tensorcircuit/applications/layers.py` & `tensorcircuit-nightly-0.9.1.dev20230518/tensorcircuit/applications/layers.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230517/tensorcircuit/applications/utils.py` & `tensorcircuit-nightly-0.9.1.dev20230518/tensorcircuit/applications/utils.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230517/tensorcircuit/applications/vags.py` & `tensorcircuit-nightly-0.9.1.dev20230518/tensorcircuit/applications/vags.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230517/tensorcircuit/applications/van.py` & `tensorcircuit-nightly-0.9.1.dev20230518/tensorcircuit/applications/van.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230517/tensorcircuit/applications/vqes.py` & `tensorcircuit-nightly-0.9.1.dev20230518/tensorcircuit/applications/vqes.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230517/tensorcircuit/asciiart.py` & `tensorcircuit-nightly-0.9.1.dev20230518/tensorcircuit/asciiart.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230517/tensorcircuit/backends/abstract_backend.py` & `tensorcircuit-nightly-0.9.1.dev20230518/tensorcircuit/backends/abstract_backend.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230517/tensorcircuit/backends/backend_factory.py` & `tensorcircuit-nightly-0.9.1.dev20230518/tensorcircuit/backends/backend_factory.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230517/tensorcircuit/backends/cupy_backend.py` & `tensorcircuit-nightly-0.9.1.dev20230518/tensorcircuit/backends/cupy_backend.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230517/tensorcircuit/backends/jax_backend.py` & `tensorcircuit-nightly-0.9.1.dev20230518/tensorcircuit/backends/jax_backend.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230517/tensorcircuit/backends/jax_ops.py` & `tensorcircuit-nightly-0.9.1.dev20230518/tensorcircuit/backends/jax_ops.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230517/tensorcircuit/backends/numpy_backend.py` & `tensorcircuit-nightly-0.9.1.dev20230518/tensorcircuit/backends/numpy_backend.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230517/tensorcircuit/backends/pytorch_backend.py` & `tensorcircuit-nightly-0.9.1.dev20230518/tensorcircuit/backends/pytorch_backend.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230517/tensorcircuit/backends/pytorch_ops.py` & `tensorcircuit-nightly-0.9.1.dev20230518/tensorcircuit/backends/pytorch_ops.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230517/tensorcircuit/backends/tensorflow_backend.py` & `tensorcircuit-nightly-0.9.1.dev20230518/tensorcircuit/backends/tensorflow_backend.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230517/tensorcircuit/backends/tf_ops.py` & `tensorcircuit-nightly-0.9.1.dev20230518/tensorcircuit/backends/tf_ops.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230517/tensorcircuit/basecircuit.py` & `tensorcircuit-nightly-0.9.1.dev20230518/tensorcircuit/basecircuit.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230517/tensorcircuit/channels.py` & `tensorcircuit-nightly-0.9.1.dev20230518/tensorcircuit/channels.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230517/tensorcircuit/circuit.py` & `tensorcircuit-nightly-0.9.1.dev20230518/tensorcircuit/circuit.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230517/tensorcircuit/cloud/abstraction.py` & `tensorcircuit-nightly-0.9.1.dev20230518/tensorcircuit/cloud/abstraction.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230517/tensorcircuit/cloud/apis.py` & `tensorcircuit-nightly-0.9.1.dev20230518/tensorcircuit/cloud/apis.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230517/tensorcircuit/cloud/local.py` & `tensorcircuit-nightly-0.9.1.dev20230518/tensorcircuit/cloud/local.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230517/tensorcircuit/cloud/quafu_provider.py` & `tensorcircuit-nightly-0.9.1.dev20230518/tensorcircuit/cloud/quafu_provider.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230517/tensorcircuit/cloud/tencent.py` & `tensorcircuit-nightly-0.9.1.dev20230518/tensorcircuit/cloud/tencent.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230517/tensorcircuit/cloud/utils.py` & `tensorcircuit-nightly-0.9.1.dev20230518/tensorcircuit/cloud/utils.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230517/tensorcircuit/cloud/wrapper.py` & `tensorcircuit-nightly-0.9.1.dev20230518/tensorcircuit/cloud/wrapper.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230517/tensorcircuit/compiler/composed_compiler.py` & `tensorcircuit-nightly-0.9.1.dev20230518/tensorcircuit/compiler/composed_compiler.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230517/tensorcircuit/compiler/qiskit_compiler.py` & `tensorcircuit-nightly-0.9.1.dev20230518/tensorcircuit/compiler/qiskit_compiler.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230517/tensorcircuit/compiler/simple_compiler.py` & `tensorcircuit-nightly-0.9.1.dev20230518/tensorcircuit/compiler/simple_compiler.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230517/tensorcircuit/cons.py` & `tensorcircuit-nightly-0.9.1.dev20230518/tensorcircuit/cons.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230517/tensorcircuit/densitymatrix.py` & `tensorcircuit-nightly-0.9.1.dev20230518/tensorcircuit/densitymatrix.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230517/tensorcircuit/experimental.py` & `tensorcircuit-nightly-0.9.1.dev20230518/tensorcircuit/experimental.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230517/tensorcircuit/gates.py` & `tensorcircuit-nightly-0.9.1.dev20230518/tensorcircuit/gates.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230517/tensorcircuit/interfaces/__init__.py` & `tensorcircuit-nightly-0.9.1.dev20230518/tensorcircuit/interfaces/__init__.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230517/tensorcircuit/interfaces/numpy.py` & `tensorcircuit-nightly-0.9.1.dev20230518/tensorcircuit/interfaces/numpy.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230517/tensorcircuit/interfaces/scipy.py` & `tensorcircuit-nightly-0.9.1.dev20230518/tensorcircuit/interfaces/scipy.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230517/tensorcircuit/interfaces/tensorflow.py` & `tensorcircuit-nightly-0.9.1.dev20230518/tensorcircuit/interfaces/tensorflow.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230517/tensorcircuit/interfaces/tensortrans.py` & `tensorcircuit-nightly-0.9.1.dev20230518/tensorcircuit/interfaces/tensortrans.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230517/tensorcircuit/interfaces/torch.py` & `tensorcircuit-nightly-0.9.1.dev20230518/tensorcircuit/interfaces/torch.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230517/tensorcircuit/keras.py` & `tensorcircuit-nightly-0.9.1.dev20230518/tensorcircuit/keras.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230517/tensorcircuit/mps_base.py` & `tensorcircuit-nightly-0.9.1.dev20230518/tensorcircuit/mps_base.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230517/tensorcircuit/mpscircuit.py` & `tensorcircuit-nightly-0.9.1.dev20230518/tensorcircuit/mpscircuit.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230517/tensorcircuit/noisemodel.py` & `tensorcircuit-nightly-0.9.1.dev20230518/tensorcircuit/noisemodel.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230517/tensorcircuit/quantum.py` & `tensorcircuit-nightly-0.9.1.dev20230518/tensorcircuit/quantum.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230517/tensorcircuit/results/counts.py` & `tensorcircuit-nightly-0.9.1.dev20230518/tensorcircuit/results/counts.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230517/tensorcircuit/results/readout_mitigation.py` & `tensorcircuit-nightly-0.9.1.dev20230518/tensorcircuit/results/readout_mitigation.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230517/tensorcircuit/simplify.py` & `tensorcircuit-nightly-0.9.1.dev20230518/tensorcircuit/simplify.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230517/tensorcircuit/templates/blocks.py` & `tensorcircuit-nightly-0.9.1.dev20230518/tensorcircuit/templates/blocks.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230517/tensorcircuit/templates/chems.py` & `tensorcircuit-nightly-0.9.1.dev20230518/tensorcircuit/templates/chems.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230517/tensorcircuit/templates/dataset.py` & `tensorcircuit-nightly-0.9.1.dev20230518/tensorcircuit/templates/dataset.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230517/tensorcircuit/templates/ensemble.py` & `tensorcircuit-nightly-0.9.1.dev20230518/tensorcircuit/templates/ensemble.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230517/tensorcircuit/templates/graphs.py` & `tensorcircuit-nightly-0.9.1.dev20230518/tensorcircuit/templates/graphs.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230517/tensorcircuit/templates/measurements.py` & `tensorcircuit-nightly-0.9.1.dev20230518/tensorcircuit/templates/measurements.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230517/tensorcircuit/torchnn.py` & `tensorcircuit-nightly-0.9.1.dev20230518/tensorcircuit/torchnn.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230517/tensorcircuit/translation.py` & `tensorcircuit-nightly-0.9.1.dev20230518/tensorcircuit/translation.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230517/tensorcircuit/utils.py` & `tensorcircuit-nightly-0.9.1.dev20230518/tensorcircuit/utils.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230517/tensorcircuit/vis.py` & `tensorcircuit-nightly-0.9.1.dev20230518/tensorcircuit/vis.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230517/tensorcircuit_nightly.egg-info/PKG-INFO` & `tensorcircuit-nightly-0.9.1.dev20230518/tensorcircuit_nightly.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tensorcircuit-nightly
-Version: 0.9.1.dev20230517
+Version: 0.9.1.dev20230518
 Summary: nightly release for tensorcircuit
 Home-page: https://github.com/refraction-ray/tensorcircuit-dev
 Author: TensorCircuit Authors
 Author-email: znfesnpbh.tc@gmail.com
 License: UNKNOWN
 Description: <p align="center">
           <a href="https://github.com/tencent-quantum-lab/tensorcircuit">
```

### Comparing `tensorcircuit-nightly-0.9.1.dev20230517/tensorcircuit_nightly.egg-info/SOURCES.txt` & `tensorcircuit-nightly-0.9.1.dev20230518/tensorcircuit_nightly.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230517/tests/conftest.py` & `tensorcircuit-nightly-0.9.1.dev20230518/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230517/tests/test_backends.py` & `tensorcircuit-nightly-0.9.1.dev20230518/tests/test_backends.py`

 * *Files 1% similar despite different names*

```diff
@@ -298,14 +298,22 @@
     np.testing.assert_allclose(
         tc.backend.relu(tc.array_to_tensor(arr, dtype="float32")),
         np.maximum(arr, 0),
         atol=1e-4,
     )
 
 
+# @pytest.mark.parametrize("backend", [lf("npb"), lf("tfb"), lf("jaxb"), lf("torchb")])
+# def test_backend_array(backend):
+#     a = tc.backend.array([[0, 1], [1, 0]])
+#     assert tc.interfaces.which_backend(a).name == tc.backend.name
+#     a = tc.backend.array([[0, 1], [1, 0]], dtype=tc.rdtypestr)
+#     assert tc.dtype(a) == "float32"
+
+
 @pytest.mark.parametrize("backend", [lf("npb"), lf("tfb"), lf("jaxb"), lf("torchb")])
 def test_device_cpu_only(backend):
     a = tc.backend.ones([])
     dev_str = tc.backend.device(a)
     assert dev_str in ["cpu", "gpu:0"]
     tc.backend.device_move(a, dev_str)
```

### Comparing `tensorcircuit-nightly-0.9.1.dev20230517/tests/test_calibrating.py` & `tensorcircuit-nightly-0.9.1.dev20230518/tests/test_calibrating.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230517/tests/test_channels.py` & `tensorcircuit-nightly-0.9.1.dev20230518/tests/test_channels.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230517/tests/test_circuit.py` & `tensorcircuit-nightly-0.9.1.dev20230518/tests/test_circuit.py`

 * *Files 1% similar despite different names*

```diff
@@ -418,14 +418,18 @@
     r = c.expectation_ps(z=[0, 1])
     np.testing.assert_allclose(tc.backend.numpy(r), -1, atol=1e-5)
 
     c = tc.Circuit(2)
     c.H(0)
     r = c.expectation_ps(z=[1], x=[0])
     np.testing.assert_allclose(tc.backend.numpy(r), 1, atol=1e-5)
+    r1 = c.expectation_ps(ps=[1, 3])
+    np.testing.assert_allclose(tc.backend.numpy(r1), 1, atol=1e-5)
+    r1 = c.expectation_ps(z=[1, 2], ps=[1, 3])
+    np.testing.assert_allclose(tc.backend.numpy(r1), 1, atol=1e-5)
 
 
 def test_probability():
     for c_cls in [tc.Circuit, tc.DMCircuit]:
         c = c_cls(2)
         c.h(0)
         c.h(1)
```

### Comparing `tensorcircuit-nightly-0.9.1.dev20230517/tests/test_cloud.py` & `tensorcircuit-nightly-0.9.1.dev20230518/tests/test_cloud.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230517/tests/test_compiler.py` & `tensorcircuit-nightly-0.9.1.dev20230518/tests/test_compiler.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230517/tests/test_dmcircuit.py` & `tensorcircuit-nightly-0.9.1.dev20230518/tests/test_dmcircuit.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230517/tests/test_ensemble.py` & `tensorcircuit-nightly-0.9.1.dev20230518/tests/test_ensemble.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230517/tests/test_gates.py` & `tensorcircuit-nightly-0.9.1.dev20230518/tests/test_gates.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230517/tests/test_interfaces.py` & `tensorcircuit-nightly-0.9.1.dev20230518/tests/test_interfaces.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230517/tests/test_keras.py` & `tensorcircuit-nightly-0.9.1.dev20230518/tests/test_keras.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230517/tests/test_miscs.py` & `tensorcircuit-nightly-0.9.1.dev20230518/tests/test_miscs.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230517/tests/test_mpscircuit.py` & `tensorcircuit-nightly-0.9.1.dev20230518/tests/test_mpscircuit.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230517/tests/test_noisemodel.py` & `tensorcircuit-nightly-0.9.1.dev20230518/tests/test_noisemodel.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230517/tests/test_qaoa.py` & `tensorcircuit-nightly-0.9.1.dev20230518/tests/test_qaoa.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230517/tests/test_quantum.py` & `tensorcircuit-nightly-0.9.1.dev20230518/tests/test_quantum.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230517/tests/test_quantum_attr.py` & `tensorcircuit-nightly-0.9.1.dev20230518/tests/test_quantum_attr.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230517/tests/test_results.py` & `tensorcircuit-nightly-0.9.1.dev20230518/tests/test_results.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230517/tests/test_simplify.py` & `tensorcircuit-nightly-0.9.1.dev20230518/tests/test_simplify.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230517/tests/test_templates.py` & `tensorcircuit-nightly-0.9.1.dev20230518/tests/test_templates.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230517/tests/test_torchnn.py` & `tensorcircuit-nightly-0.9.1.dev20230518/tests/test_torchnn.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230517/tests/test_van.py` & `tensorcircuit-nightly-0.9.1.dev20230518/tests/test_van.py`

 * *Files identical despite different names*

