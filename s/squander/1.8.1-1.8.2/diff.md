# Comparing `tmp/squander-1.8.1.tar.gz` & `tmp/squander-1.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "squander-1.8.1.tar", last modified: Mon May 15 09:26:12 2023, max compression
+gzip compressed data, was "squander-1.8.2.tar", last modified: Thu May 18 07:29:19 2023, max compression
```

## Comparing `squander-1.8.1.tar` & `squander-1.8.2.tar`

### file list

```diff
@@ -1,192 +1,195 @@
-drwxrwxr-x   0 rakytap   (1000) rakytap   (1000)        0 2023-05-15 09:26:12.136824 squander-1.8.1/
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)    14939 2023-05-15 09:25:56.000000 squander-1.8.1/CMakeLists.txt
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)    35149 2023-05-15 09:25:56.000000 squander-1.8.1/LICENSE
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)      121 2023-05-15 09:25:56.000000 squander-1.8.1/MANIFEST.in
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)    14953 2023-05-15 09:26:12.136824 squander-1.8.1/PKG-INFO
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)    14413 2023-05-15 09:25:56.000000 squander-1.8.1/README.md
-drwxrwxr-x   0 rakytap   (1000) rakytap   (1000)        0 2023-05-15 09:26:12.116824 squander-1.8.1/cmake/
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     4306 2023-05-15 09:25:56.000000 squander-1.8.1/cmake/check_AVX.cmake
-drwxrwxr-x   0 rakytap   (1000) rakytap   (1000)        0 2023-05-15 09:26:12.120824 squander-1.8.1/common/
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     6776 2023-05-15 09:25:56.000000 squander-1.8.1/common/Adam.cpp
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     8316 2023-05-15 09:25:56.000000 squander-1.8.1/common/common.cpp
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     5293 2023-05-15 09:25:56.000000 squander-1.8.1/common/common_DFE.cpp
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     5524 2023-05-15 09:25:56.000000 squander-1.8.1/common/config_element.cpp
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)    14292 2023-05-15 09:25:56.000000 squander-1.8.1/common/dot.cpp
-drwxrwxr-x   0 rakytap   (1000) rakytap   (1000)        0 2023-05-15 09:26:12.120824 squander-1.8.1/common/include/
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     3441 2023-05-15 09:25:56.000000 squander-1.8.1/common/include/Adam.h
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)      216 2023-05-15 09:25:56.000000 squander-1.8.1/common/include/Config.h.in
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     2109 2023-05-15 09:25:56.000000 squander-1.8.1/common/include/QGDTypes.h
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     5293 2023-05-15 09:25:56.000000 squander-1.8.1/common/include/common.h
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     3026 2023-05-15 09:25:56.000000 squander-1.8.1/common/include/common_DFE.h
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     3423 2023-05-15 09:25:56.000000 squander-1.8.1/common/include/config_element.h
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     7626 2023-05-15 09:25:56.000000 squander-1.8.1/common/include/dot.h
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     9130 2023-05-15 09:25:56.000000 squander-1.8.1/common/include/lbfgs.h
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     2443 2023-05-15 09:25:56.000000 squander-1.8.1/common/include/logging.h
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     3812 2023-05-15 09:25:56.000000 squander-1.8.1/common/include/matrix.h
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)    13485 2023-05-15 09:25:56.000000 squander-1.8.1/common/include/matrix_base.h
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     3746 2023-05-15 09:25:56.000000 squander-1.8.1/common/include/matrix_real.h
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     1393 2023-05-15 09:25:56.000000 squander-1.8.1/common/include/mpi_base.h
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     1468 2023-05-15 09:25:56.000000 squander-1.8.1/common/include/numpy_interface.h
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     9251 2023-05-15 09:25:56.000000 squander-1.8.1/common/include/tolmin.h
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)   156010 2023-05-15 09:25:56.000000 squander-1.8.1/common/lbfgs.cpp
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     2515 2023-05-15 09:25:56.000000 squander-1.8.1/common/logging.cpp
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     5065 2023-05-15 09:25:56.000000 squander-1.8.1/common/matrix.cpp
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     4491 2023-05-15 09:25:56.000000 squander-1.8.1/common/matrix_real.cpp
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     1095 2023-05-15 09:25:56.000000 squander-1.8.1/common/mpi_base.cpp
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     4808 2023-05-15 09:25:56.000000 squander-1.8.1/common/numpy_interface.cpp
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)    58244 2023-05-15 09:25:56.000000 squander-1.8.1/common/tolmin.cpp
-drwxrwxr-x   0 rakytap   (1000) rakytap   (1000)        0 2023-05-15 09:26:12.120824 squander-1.8.1/decomposition/
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)    57706 2023-05-15 09:25:56.000000 squander-1.8.1/decomposition/Decomposition_Base.cpp
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)    37081 2023-05-15 09:25:56.000000 squander-1.8.1/decomposition/N_Qubit_Decomposition.cpp
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)   100052 2023-05-15 09:25:56.000000 squander-1.8.1/decomposition/N_Qubit_Decomposition_Base.cpp
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)    16714 2023-05-15 09:25:56.000000 squander-1.8.1/decomposition/N_Qubit_Decomposition_Cost_Function.cpp
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)    77317 2023-05-15 09:25:56.000000 squander-1.8.1/decomposition/N_Qubit_Decomposition_adaptive.cpp
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)    12741 2023-05-15 09:25:56.000000 squander-1.8.1/decomposition/N_Qubit_Decomposition_custom.cpp
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)    23502 2023-05-15 09:25:56.000000 squander-1.8.1/decomposition/Sub_Matrix_Decomposition.cpp
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     8536 2023-05-15 09:25:56.000000 squander-1.8.1/decomposition/Sub_Matrix_Decomposition_Cost_Function.cpp
-drwxrwxr-x   0 rakytap   (1000) rakytap   (1000)        0 2023-05-15 09:26:12.124824 squander-1.8.1/decomposition/include/
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)    16035 2023-05-15 09:25:56.000000 squander-1.8.1/decomposition/include/Decomposition_Base.h
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     7166 2023-05-15 09:25:56.000000 squander-1.8.1/decomposition/include/N_Qubit_Decomposition.h
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)    15865 2023-05-15 09:25:56.000000 squander-1.8.1/decomposition/include/N_Qubit_Decomposition_Base.h
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     5077 2023-05-15 09:25:56.000000 squander-1.8.1/decomposition/include/N_Qubit_Decomposition_Cost_Function.h
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     8301 2023-05-15 09:25:56.000000 squander-1.8.1/decomposition/include/N_Qubit_Decomposition_adaptive.h
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     3393 2023-05-15 09:25:56.000000 squander-1.8.1/decomposition/include/N_Qubit_Decomposition_custom.h
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     6922 2023-05-15 09:25:56.000000 squander-1.8.1/decomposition/include/Sub_Matrix_Decomposition.h
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     3723 2023-05-15 09:25:56.000000 squander-1.8.1/decomposition/include/Sub_Matrix_Decomposition_Cost_Function.h
-drwxrwxr-x   0 rakytap   (1000) rakytap   (1000)        0 2023-05-15 09:26:12.124824 squander-1.8.1/gates/
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     5728 2023-05-15 09:25:56.000000 squander-1.8.1/gates/Adaptive.cpp
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     4900 2023-05-15 09:25:56.000000 squander-1.8.1/gates/CH.cpp
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     4937 2023-05-15 09:25:56.000000 squander-1.8.1/gates/CNOT.cpp
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     5839 2023-05-15 09:25:56.000000 squander-1.8.1/gates/CRY.cpp
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     4841 2023-05-15 09:25:56.000000 squander-1.8.1/gates/CZ.cpp
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     7781 2023-05-15 09:25:56.000000 squander-1.8.1/gates/Composite.cpp
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)    11545 2023-05-15 09:25:56.000000 squander-1.8.1/gates/Gate.cpp
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)   120998 2023-05-15 09:25:56.000000 squander-1.8.1/gates/Gates_block.cpp
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     8547 2023-05-15 09:25:56.000000 squander-1.8.1/gates/ON.cpp
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     6819 2023-05-15 09:25:56.000000 squander-1.8.1/gates/RX.cpp
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     6815 2023-05-15 09:25:56.000000 squander-1.8.1/gates/RY.cpp
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     7110 2023-05-15 09:25:56.000000 squander-1.8.1/gates/RZ.cpp
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     8697 2023-05-15 09:25:56.000000 squander-1.8.1/gates/SX.cpp
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     9587 2023-05-15 09:25:56.000000 squander-1.8.1/gates/SYC.cpp
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)    15472 2023-05-15 09:25:56.000000 squander-1.8.1/gates/U3.cpp
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     8769 2023-05-15 09:25:56.000000 squander-1.8.1/gates/UN.cpp
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     7950 2023-05-15 09:25:56.000000 squander-1.8.1/gates/X.cpp
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     5671 2023-05-15 09:25:56.000000 squander-1.8.1/gates/Y.cpp
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     5672 2023-05-15 09:25:56.000000 squander-1.8.1/gates/Z.cpp
-drwxrwxr-x   0 rakytap   (1000) rakytap   (1000)        0 2023-05-15 09:26:12.128824 squander-1.8.1/gates/include/
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     3395 2023-05-15 09:25:56.000000 squander-1.8.1/gates/include/Adaptive.h
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     2428 2023-05-15 09:25:56.000000 squander-1.8.1/gates/include/CH.h
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     2504 2023-05-15 09:25:56.000000 squander-1.8.1/gates/include/CNOT.h
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     3113 2023-05-15 09:25:56.000000 squander-1.8.1/gates/include/CRY.h
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     2427 2023-05-15 09:25:56.000000 squander-1.8.1/gates/include/CZ.h
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     3594 2023-05-15 09:25:56.000000 squander-1.8.1/gates/include/Composite.h
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     5097 2023-05-15 09:25:56.000000 squander-1.8.1/gates/include/Gate.h
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)    15824 2023-05-15 09:25:56.000000 squander-1.8.1/gates/include/Gates_block.h
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     3412 2023-05-15 09:25:56.000000 squander-1.8.1/gates/include/ON.h
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     2812 2023-05-15 09:25:56.000000 squander-1.8.1/gates/include/RX.h
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     3088 2023-05-15 09:25:56.000000 squander-1.8.1/gates/include/RY.h
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     2808 2023-05-15 09:25:56.000000 squander-1.8.1/gates/include/RZ.h
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     2783 2023-05-15 09:25:56.000000 squander-1.8.1/gates/include/SX.h
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     2428 2023-05-15 09:25:56.000000 squander-1.8.1/gates/include/SYC.h
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     6017 2023-05-15 09:25:56.000000 squander-1.8.1/gates/include/U3.h
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     3412 2023-05-15 09:25:56.000000 squander-1.8.1/gates/include/UN.h
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     2774 2023-05-15 09:25:56.000000 squander-1.8.1/gates/include/X.h
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     2772 2023-05-15 09:25:56.000000 squander-1.8.1/gates/include/Y.h
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     2772 2023-05-15 09:25:56.000000 squander-1.8.1/gates/include/Z.h
-drwxrwxr-x   0 rakytap   (1000) rakytap   (1000)        0 2023-05-15 09:26:12.128824 squander-1.8.1/gates/kernels/
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)    23561 2023-05-15 09:25:56.000000 squander-1.8.1/gates/kernels/apply_kernel_to_input_AVX.cpp
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)    32382 2023-05-15 09:25:56.000000 squander-1.8.1/gates/kernels/apply_kernel_to_state_vector_input.cpp
-drwxrwxr-x   0 rakytap   (1000) rakytap   (1000)        0 2023-05-15 09:26:12.128824 squander-1.8.1/gates/kernels/include/
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     1786 2023-05-15 09:25:56.000000 squander-1.8.1/gates/kernels/include/apply_kernel_to_input_AVX.h
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     2099 2023-05-15 09:25:56.000000 squander-1.8.1/gates/kernels/include/apply_kernel_to_state_vector_input.h
-drwxrwxr-x   0 rakytap   (1000) rakytap   (1000)        0 2023-05-15 09:26:12.128824 squander-1.8.1/nn/
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)    18464 2023-05-15 09:25:56.000000 squander-1.8.1/nn/NN.cpp
-drwxrwxr-x   0 rakytap   (1000) rakytap   (1000)        0 2023-05-15 09:26:12.128824 squander-1.8.1/nn/include/
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     5274 2023-05-15 09:25:56.000000 squander-1.8.1/nn/include/NN.h
-drwxrwxr-x   0 rakytap   (1000) rakytap   (1000)        0 2023-05-15 09:26:12.128824 squander-1.8.1/optimization_engines/
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     9698 2023-05-15 09:25:56.000000 squander-1.8.1/optimization_engines/RL_experience.cpp
-drwxrwxr-x   0 rakytap   (1000) rakytap   (1000)        0 2023-05-15 09:26:12.128824 squander-1.8.1/optimization_engines/include/
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     3549 2023-05-15 09:25:56.000000 squander-1.8.1/optimization_engines/include/RL_experience.h
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)      123 2023-05-15 09:25:56.000000 squander-1.8.1/pyproject.toml
-drwxrwxr-x   0 rakytap   (1000) rakytap   (1000)        0 2023-05-15 09:26:12.128824 squander-1.8.1/qgd_python/
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)       27 2023-05-15 09:25:56.000000 squander-1.8.1/qgd_python/__init__.py
-drwxrwxr-x   0 rakytap   (1000) rakytap   (1000)        0 2023-05-15 09:26:12.128824 squander-1.8.1/qgd_python/decomposition/
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     4386 2023-05-15 09:25:56.000000 squander-1.8.1/qgd_python/decomposition/CMakeLists.txt
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)       27 2023-05-15 09:25:56.000000 squander-1.8.1/qgd_python/decomposition/__init__.py
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     7661 2023-05-15 09:25:56.000000 squander-1.8.1/qgd_python/decomposition/qgd_N_Qubit_Decomposition.py
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)    36730 2023-05-15 09:25:56.000000 squander-1.8.1/qgd_python/decomposition/qgd_N_Qubit_Decomposition_Wrapper.cpp
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)    24494 2023-05-15 09:25:56.000000 squander-1.8.1/qgd_python/decomposition/qgd_N_Qubit_Decomposition_adaptive.py
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)    80626 2023-05-15 09:25:56.000000 squander-1.8.1/qgd_python/decomposition/qgd_N_Qubit_Decomposition_adaptive_Wrapper.cpp
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)    14278 2023-05-15 09:25:56.000000 squander-1.8.1/qgd_python/decomposition/qgd_N_Qubit_Decomposition_custom.py
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)    41007 2023-05-15 09:25:56.000000 squander-1.8.1/qgd_python/decomposition/qgd_N_Qubit_Decomposition_custom_Wrapper.cpp
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     3367 2023-05-15 09:25:56.000000 squander-1.8.1/qgd_python/decomposition/qgd_N_Qubit_State_Preparation_adaptive.py
-drwxrwxr-x   0 rakytap   (1000) rakytap   (1000)        0 2023-05-15 09:26:12.132824 squander-1.8.1/qgd_python/decomposition/test/
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)        0 2023-05-15 09:25:56.000000 squander-1.8.1/qgd_python/decomposition/test/__init__.py
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)    11024 2023-05-15 09:25:56.000000 squander-1.8.1/qgd_python/decomposition/test/test_Compression.py
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     1927 2023-05-15 09:25:56.000000 squander-1.8.1/qgd_python/decomposition/test/test_Global_Phase.py
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     7037 2023-05-15 09:25:56.000000 squander-1.8.1/qgd_python/decomposition/test/test_IBM.py
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     1777 2023-05-15 09:25:56.000000 squander-1.8.1/qgd_python/decomposition/test/test_Project_Name.py
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     5616 2023-05-15 09:25:56.000000 squander-1.8.1/qgd_python/decomposition/test/test_QX2.py
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     4399 2023-05-15 09:25:56.000000 squander-1.8.1/qgd_python/decomposition/test/test_State_Preparation.py
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     1656 2023-05-15 09:25:56.000000 squander-1.8.1/qgd_python/decomposition/test/test_Unitary.py
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     4672 2023-05-15 09:25:56.000000 squander-1.8.1/qgd_python/decomposition/test/test_decomposition.py
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     7190 2023-05-15 09:25:56.000000 squander-1.8.1/qgd_python/decomposition/test/test_fmo.py
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     7018 2023-05-15 09:25:56.000000 squander-1.8.1/qgd_python/decomposition/test/test_heavy_hex.py
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     5222 2023-05-15 09:25:56.000000 squander-1.8.1/qgd_python/decomposition/test/test_optmization_problem_combined.py
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     4905 2023-05-15 09:25:56.000000 squander-1.8.1/qgd_python/decomposition/test/test_parametric_circuit.py
-drwxrwxr-x   0 rakytap   (1000) rakytap   (1000)        0 2023-05-15 09:26:12.132824 squander-1.8.1/qgd_python/gates/
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)    13547 2023-05-15 09:25:56.000000 squander-1.8.1/qgd_python/gates/CMakeLists.txt
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)        0 2023-05-15 09:25:56.000000 squander-1.8.1/qgd_python/gates/__init__.py
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     8219 2023-05-15 09:25:56.000000 squander-1.8.1/qgd_python/gates/qgd_CH.cpp
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     8160 2023-05-15 09:25:56.000000 squander-1.8.1/qgd_python/gates/qgd_CNOT.cpp
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     8033 2023-05-15 09:25:56.000000 squander-1.8.1/qgd_python/gates/qgd_CZ.cpp
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)    28536 2023-05-15 09:25:56.000000 squander-1.8.1/qgd_python/gates/qgd_Gates_Block.cpp
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     8529 2023-05-15 09:25:56.000000 squander-1.8.1/qgd_python/gates/qgd_RX.cpp
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     8528 2023-05-15 09:25:56.000000 squander-1.8.1/qgd_python/gates/qgd_RY.cpp
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     8527 2023-05-15 09:25:56.000000 squander-1.8.1/qgd_python/gates/qgd_RZ.cpp
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     7771 2023-05-15 09:25:56.000000 squander-1.8.1/qgd_python/gates/qgd_SX.cpp
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     7801 2023-05-15 09:25:56.000000 squander-1.8.1/qgd_python/gates/qgd_SYC.cpp
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     9054 2023-05-15 09:25:56.000000 squander-1.8.1/qgd_python/gates/qgd_U3.cpp
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     7489 2023-05-15 09:25:56.000000 squander-1.8.1/qgd_python/gates/qgd_X.cpp
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     8367 2023-05-15 09:25:56.000000 squander-1.8.1/qgd_python/gates/qgd_Y.cpp
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     8367 2023-05-15 09:25:56.000000 squander-1.8.1/qgd_python/gates/qgd_Z.cpp
-drwxrwxr-x   0 rakytap   (1000) rakytap   (1000)        0 2023-05-15 09:26:12.136824 squander-1.8.1/qgd_python/gates/test/
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)        0 2023-05-15 09:25:56.000000 squander-1.8.1/qgd_python/gates/test/__init__.py
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     3364 2023-05-15 09:25:56.000000 squander-1.8.1/qgd_python/gates/test/test_CH.py
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     3409 2023-05-15 09:25:56.000000 squander-1.8.1/qgd_python/gates/test/test_CNOT.py
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     3444 2023-05-15 09:25:56.000000 squander-1.8.1/qgd_python/gates/test/test_CZ.py
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     3466 2023-05-15 09:25:56.000000 squander-1.8.1/qgd_python/gates/test/test_RX.py
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     3348 2023-05-15 09:25:56.000000 squander-1.8.1/qgd_python/gates/test/test_RY.py
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     3919 2023-05-15 09:25:56.000000 squander-1.8.1/qgd_python/gates/test/test_RZ.py
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     3278 2023-05-15 09:25:56.000000 squander-1.8.1/qgd_python/gates/test/test_SX.py
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     3676 2023-05-15 09:25:56.000000 squander-1.8.1/qgd_python/gates/test/test_U3.py
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     3182 2023-05-15 09:25:56.000000 squander-1.8.1/qgd_python/gates/test/test_X.py
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     3179 2023-05-15 09:25:56.000000 squander-1.8.1/qgd_python/gates/test/test_Y.py
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     3232 2023-05-15 09:25:56.000000 squander-1.8.1/qgd_python/gates/test/test_Z.py
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     6878 2023-05-15 09:25:56.000000 squander-1.8.1/qgd_python/gates/test/test_gates.py
-drwxrwxr-x   0 rakytap   (1000) rakytap   (1000)        0 2023-05-15 09:26:12.136824 squander-1.8.1/qgd_python/nn/
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     1304 2023-05-15 09:25:56.000000 squander-1.8.1/qgd_python/nn/CMakeLists.txt
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)       27 2023-05-15 09:25:56.000000 squander-1.8.1/qgd_python/nn/__init__.py
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     2387 2023-05-15 09:25:56.000000 squander-1.8.1/qgd_python/nn/qgd_nn.py
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     9635 2023-05-15 09:25:56.000000 squander-1.8.1/qgd_python/nn/qgd_nn_Wrapper.cpp
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     1573 2023-05-15 09:25:56.000000 squander-1.8.1/qgd_python/utils.py
-drwxrwxr-x   0 rakytap   (1000) rakytap   (1000)        0 2023-05-15 09:26:12.136824 squander-1.8.1/random_unitary/
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     6628 2023-05-15 09:25:56.000000 squander-1.8.1/random_unitary/Random_Orthogonal.cpp
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)    11039 2023-05-15 09:25:56.000000 squander-1.8.1/random_unitary/Random_Unitary.cpp
-drwxrwxr-x   0 rakytap   (1000) rakytap   (1000)        0 2023-05-15 09:26:12.136824 squander-1.8.1/random_unitary/include/
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     1927 2023-05-15 09:25:56.000000 squander-1.8.1/random_unitary/include/Random_Orthogonal.h
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     4476 2023-05-15 09:25:56.000000 squander-1.8.1/random_unitary/include/Random_Unitary.h
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)       38 2023-05-15 09:26:12.136824 squander-1.8.1/setup.cfg
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     1850 2023-05-15 09:25:56.000000 squander-1.8.1/setup.py
-drwxrwxr-x   0 rakytap   (1000) rakytap   (1000)        0 2023-05-15 09:26:12.136824 squander-1.8.1/squander/
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     1442 2023-05-15 09:25:56.000000 squander-1.8.1/squander/__init__.py
-drwxrwxr-x   0 rakytap   (1000) rakytap   (1000)        0 2023-05-15 09:26:12.136824 squander-1.8.1/squander.egg-info/
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)    14953 2023-05-15 09:26:11.000000 squander-1.8.1/squander.egg-info/PKG-INFO
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     5133 2023-05-15 09:26:12.000000 squander-1.8.1/squander.egg-info/SOURCES.txt
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)        1 2023-05-15 09:26:11.000000 squander-1.8.1/squander.egg-info/dependency_links.txt
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)       50 2023-05-15 09:26:11.000000 squander-1.8.1/squander.egg-info/requires.txt
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)       20 2023-05-15 09:26:11.000000 squander-1.8.1/squander.egg-info/top_level.txt
-drwxrwxr-x   0 rakytap   (1000) rakytap   (1000)        0 2023-05-15 09:26:12.136824 squander-1.8.1/test_standalone/
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     1996 2023-05-15 09:25:56.000000 squander-1.8.1/test_standalone/CMakeLists.txt
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     6325 2023-05-15 09:25:56.000000 squander-1.8.1/test_standalone/custom_gate_structure_test.cpp
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     4837 2023-05-15 09:25:56.000000 squander-1.8.1/test_standalone/decomposition_test.cpp
+drwxrwxr-x   0 rakytap   (1002) rakytap   (1002)        0 2023-05-18 07:29:19.908699 squander-1.8.2/
+drwxrwxr-x   0 rakytap   (1002) rakytap   (1002)        0 2023-05-18 07:29:19.880699 squander-1.8.2/.pytest_cache/
+-rw-rw-r--   0 rakytap   (1002) rakytap   (1002)      302 2023-05-18 07:01:34.000000 squander-1.8.2/.pytest_cache/README.md
+-rw-rw-r--   0 rakytap   (1002) rakytap   (1002)    14939 2023-05-18 07:00:48.000000 squander-1.8.2/CMakeLists.txt
+-rw-rw-r--   0 rakytap   (1002) rakytap   (1002)    35149 2023-05-18 07:00:49.000000 squander-1.8.2/LICENSE
+-rw-rw-r--   0 rakytap   (1002) rakytap   (1002)      121 2023-05-18 07:00:49.000000 squander-1.8.2/MANIFEST.in
+-rw-rw-r--   0 rakytap   (1002) rakytap   (1002)    15001 2023-05-18 07:29:19.908699 squander-1.8.2/PKG-INFO
+-rw-rw-r--   0 rakytap   (1002) rakytap   (1002)    14413 2023-05-18 07:00:49.000000 squander-1.8.2/README.md
+drwxrwxr-x   0 rakytap   (1002) rakytap   (1002)        0 2023-05-18 07:29:19.880699 squander-1.8.2/cmake/
+-rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     4306 2023-05-18 07:00:49.000000 squander-1.8.2/cmake/check_AVX.cmake
+drwxrwxr-x   0 rakytap   (1002) rakytap   (1002)        0 2023-05-18 07:29:19.884699 squander-1.8.2/common/
+-rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     6776 2023-05-18 07:00:49.000000 squander-1.8.2/common/Adam.cpp
+-rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     8316 2023-05-18 07:00:49.000000 squander-1.8.2/common/common.cpp
+-rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     5293 2023-05-18 07:00:49.000000 squander-1.8.2/common/common_DFE.cpp
+-rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     5524 2023-05-18 07:00:49.000000 squander-1.8.2/common/config_element.cpp
+-rw-rw-r--   0 rakytap   (1002) rakytap   (1002)    14292 2023-05-18 07:00:49.000000 squander-1.8.2/common/dot.cpp
+drwxrwxr-x   0 rakytap   (1002) rakytap   (1002)        0 2023-05-18 07:29:19.884699 squander-1.8.2/common/include/
+-rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     3441 2023-05-18 07:00:49.000000 squander-1.8.2/common/include/Adam.h
+-rw-rw-r--   0 rakytap   (1002) rakytap   (1002)      166 2023-05-18 07:01:12.000000 squander-1.8.2/common/include/Config.h
+-rw-rw-r--   0 rakytap   (1002) rakytap   (1002)      216 2023-05-18 07:00:49.000000 squander-1.8.2/common/include/Config.h.in
+-rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     2109 2023-05-18 07:00:49.000000 squander-1.8.2/common/include/QGDTypes.h
+-rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     5293 2023-05-18 07:00:49.000000 squander-1.8.2/common/include/common.h
+-rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     3026 2023-05-18 07:00:49.000000 squander-1.8.2/common/include/common_DFE.h
+-rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     3423 2023-05-18 07:00:49.000000 squander-1.8.2/common/include/config_element.h
+-rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     7626 2023-05-18 07:00:49.000000 squander-1.8.2/common/include/dot.h
+-rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     9130 2023-05-18 07:00:49.000000 squander-1.8.2/common/include/lbfgs.h
+-rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     2443 2023-05-18 07:00:49.000000 squander-1.8.2/common/include/logging.h
+-rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     3812 2023-05-18 07:00:49.000000 squander-1.8.2/common/include/matrix.h
+-rw-rw-r--   0 rakytap   (1002) rakytap   (1002)    13485 2023-05-18 07:00:49.000000 squander-1.8.2/common/include/matrix_base.h
+-rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     3746 2023-05-18 07:00:49.000000 squander-1.8.2/common/include/matrix_real.h
+-rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     1393 2023-05-18 07:00:49.000000 squander-1.8.2/common/include/mpi_base.h
+-rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     1468 2023-05-18 07:00:49.000000 squander-1.8.2/common/include/numpy_interface.h
+-rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     9251 2023-05-18 07:00:49.000000 squander-1.8.2/common/include/tolmin.h
+-rw-rw-r--   0 rakytap   (1002) rakytap   (1002)   156010 2023-05-18 07:00:49.000000 squander-1.8.2/common/lbfgs.cpp
+-rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     2515 2023-05-18 07:00:49.000000 squander-1.8.2/common/logging.cpp
+-rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     5065 2023-05-18 07:00:49.000000 squander-1.8.2/common/matrix.cpp
+-rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     4491 2023-05-18 07:00:49.000000 squander-1.8.2/common/matrix_real.cpp
+-rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     1095 2023-05-18 07:00:49.000000 squander-1.8.2/common/mpi_base.cpp
+-rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     4808 2023-05-18 07:00:49.000000 squander-1.8.2/common/numpy_interface.cpp
+-rw-rw-r--   0 rakytap   (1002) rakytap   (1002)    58244 2023-05-18 07:00:49.000000 squander-1.8.2/common/tolmin.cpp
+drwxrwxr-x   0 rakytap   (1002) rakytap   (1002)        0 2023-05-18 07:29:19.888699 squander-1.8.2/decomposition/
+-rw-rw-r--   0 rakytap   (1002) rakytap   (1002)    57706 2023-05-18 07:00:49.000000 squander-1.8.2/decomposition/Decomposition_Base.cpp
+-rw-rw-r--   0 rakytap   (1002) rakytap   (1002)    37081 2023-05-18 07:00:49.000000 squander-1.8.2/decomposition/N_Qubit_Decomposition.cpp
+-rw-rw-r--   0 rakytap   (1002) rakytap   (1002)   100513 2023-05-18 07:00:49.000000 squander-1.8.2/decomposition/N_Qubit_Decomposition_Base.cpp
+-rw-rw-r--   0 rakytap   (1002) rakytap   (1002)    16714 2023-05-18 07:00:49.000000 squander-1.8.2/decomposition/N_Qubit_Decomposition_Cost_Function.cpp
+-rw-rw-r--   0 rakytap   (1002) rakytap   (1002)    77317 2023-05-18 07:00:49.000000 squander-1.8.2/decomposition/N_Qubit_Decomposition_adaptive.cpp
+-rw-rw-r--   0 rakytap   (1002) rakytap   (1002)    12741 2023-05-18 07:00:49.000000 squander-1.8.2/decomposition/N_Qubit_Decomposition_custom.cpp
+-rw-rw-r--   0 rakytap   (1002) rakytap   (1002)    23502 2023-05-18 07:00:49.000000 squander-1.8.2/decomposition/Sub_Matrix_Decomposition.cpp
+-rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     8536 2023-05-18 07:00:49.000000 squander-1.8.2/decomposition/Sub_Matrix_Decomposition_Cost_Function.cpp
+drwxrwxr-x   0 rakytap   (1002) rakytap   (1002)        0 2023-05-18 07:29:19.888699 squander-1.8.2/decomposition/include/
+-rw-rw-r--   0 rakytap   (1002) rakytap   (1002)    16035 2023-05-18 07:00:49.000000 squander-1.8.2/decomposition/include/Decomposition_Base.h
+-rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     7166 2023-05-18 07:00:49.000000 squander-1.8.2/decomposition/include/N_Qubit_Decomposition.h
+-rw-rw-r--   0 rakytap   (1002) rakytap   (1002)    15865 2023-05-18 07:00:49.000000 squander-1.8.2/decomposition/include/N_Qubit_Decomposition_Base.h
+-rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     5077 2023-05-18 07:00:49.000000 squander-1.8.2/decomposition/include/N_Qubit_Decomposition_Cost_Function.h
+-rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     8301 2023-05-18 07:00:49.000000 squander-1.8.2/decomposition/include/N_Qubit_Decomposition_adaptive.h
+-rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     3393 2023-05-18 07:00:49.000000 squander-1.8.2/decomposition/include/N_Qubit_Decomposition_custom.h
+-rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     6922 2023-05-18 07:00:49.000000 squander-1.8.2/decomposition/include/Sub_Matrix_Decomposition.h
+-rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     3723 2023-05-18 07:00:49.000000 squander-1.8.2/decomposition/include/Sub_Matrix_Decomposition_Cost_Function.h
+drwxrwxr-x   0 rakytap   (1002) rakytap   (1002)        0 2023-05-18 07:29:19.892699 squander-1.8.2/gates/
+-rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     5728 2023-05-18 07:00:49.000000 squander-1.8.2/gates/Adaptive.cpp
+-rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     4900 2023-05-18 07:00:49.000000 squander-1.8.2/gates/CH.cpp
+-rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     4937 2023-05-18 07:00:49.000000 squander-1.8.2/gates/CNOT.cpp
+-rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     5839 2023-05-18 07:00:49.000000 squander-1.8.2/gates/CRY.cpp
+-rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     4841 2023-05-18 07:00:49.000000 squander-1.8.2/gates/CZ.cpp
+-rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     7781 2023-05-18 07:00:49.000000 squander-1.8.2/gates/Composite.cpp
+-rw-rw-r--   0 rakytap   (1002) rakytap   (1002)    11545 2023-05-18 07:00:49.000000 squander-1.8.2/gates/Gate.cpp
+-rw-rw-r--   0 rakytap   (1002) rakytap   (1002)   120998 2023-05-18 07:00:49.000000 squander-1.8.2/gates/Gates_block.cpp
+-rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     8547 2023-05-18 07:00:49.000000 squander-1.8.2/gates/ON.cpp
+-rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     6819 2023-05-18 07:00:49.000000 squander-1.8.2/gates/RX.cpp
+-rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     6815 2023-05-18 07:00:49.000000 squander-1.8.2/gates/RY.cpp
+-rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     7110 2023-05-18 07:00:49.000000 squander-1.8.2/gates/RZ.cpp
+-rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     8697 2023-05-18 07:00:49.000000 squander-1.8.2/gates/SX.cpp
+-rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     9587 2023-05-18 07:00:49.000000 squander-1.8.2/gates/SYC.cpp
+-rw-rw-r--   0 rakytap   (1002) rakytap   (1002)    15472 2023-05-18 07:00:49.000000 squander-1.8.2/gates/U3.cpp
+-rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     8769 2023-05-18 07:00:49.000000 squander-1.8.2/gates/UN.cpp
+-rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     7950 2023-05-18 07:00:49.000000 squander-1.8.2/gates/X.cpp
+-rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     5671 2023-05-18 07:00:49.000000 squander-1.8.2/gates/Y.cpp
+-rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     5672 2023-05-18 07:00:49.000000 squander-1.8.2/gates/Z.cpp
+drwxrwxr-x   0 rakytap   (1002) rakytap   (1002)        0 2023-05-18 07:29:19.896699 squander-1.8.2/gates/include/
+-rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     3395 2023-05-18 07:00:49.000000 squander-1.8.2/gates/include/Adaptive.h
+-rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     2428 2023-05-18 07:00:49.000000 squander-1.8.2/gates/include/CH.h
+-rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     2504 2023-05-18 07:00:49.000000 squander-1.8.2/gates/include/CNOT.h
+-rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     3113 2023-05-18 07:00:49.000000 squander-1.8.2/gates/include/CRY.h
+-rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     2427 2023-05-18 07:00:49.000000 squander-1.8.2/gates/include/CZ.h
+-rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     3594 2023-05-18 07:00:49.000000 squander-1.8.2/gates/include/Composite.h
+-rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     5097 2023-05-18 07:00:49.000000 squander-1.8.2/gates/include/Gate.h
+-rw-rw-r--   0 rakytap   (1002) rakytap   (1002)    15824 2023-05-18 07:00:49.000000 squander-1.8.2/gates/include/Gates_block.h
+-rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     3412 2023-05-18 07:00:49.000000 squander-1.8.2/gates/include/ON.h
+-rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     2812 2023-05-18 07:00:49.000000 squander-1.8.2/gates/include/RX.h
+-rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     3088 2023-05-18 07:00:49.000000 squander-1.8.2/gates/include/RY.h
+-rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     2808 2023-05-18 07:00:49.000000 squander-1.8.2/gates/include/RZ.h
+-rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     2783 2023-05-18 07:00:49.000000 squander-1.8.2/gates/include/SX.h
+-rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     2428 2023-05-18 07:00:49.000000 squander-1.8.2/gates/include/SYC.h
+-rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     6017 2023-05-18 07:00:49.000000 squander-1.8.2/gates/include/U3.h
+-rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     3412 2023-05-18 07:00:49.000000 squander-1.8.2/gates/include/UN.h
+-rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     2774 2023-05-18 07:00:49.000000 squander-1.8.2/gates/include/X.h
+-rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     2772 2023-05-18 07:00:49.000000 squander-1.8.2/gates/include/Y.h
+-rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     2772 2023-05-18 07:00:49.000000 squander-1.8.2/gates/include/Z.h
+drwxrwxr-x   0 rakytap   (1002) rakytap   (1002)        0 2023-05-18 07:29:19.896699 squander-1.8.2/gates/kernels/
+-rw-rw-r--   0 rakytap   (1002) rakytap   (1002)    23561 2023-05-18 07:00:49.000000 squander-1.8.2/gates/kernels/apply_kernel_to_input_AVX.cpp
+-rw-rw-r--   0 rakytap   (1002) rakytap   (1002)    32382 2023-05-18 07:00:49.000000 squander-1.8.2/gates/kernels/apply_kernel_to_state_vector_input.cpp
+drwxrwxr-x   0 rakytap   (1002) rakytap   (1002)        0 2023-05-18 07:29:19.896699 squander-1.8.2/gates/kernels/include/
+-rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     1786 2023-05-18 07:00:49.000000 squander-1.8.2/gates/kernels/include/apply_kernel_to_input_AVX.h
+-rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     2099 2023-05-18 07:00:49.000000 squander-1.8.2/gates/kernels/include/apply_kernel_to_state_vector_input.h
+drwxrwxr-x   0 rakytap   (1002) rakytap   (1002)        0 2023-05-18 07:29:19.896699 squander-1.8.2/nn/
+-rw-rw-r--   0 rakytap   (1002) rakytap   (1002)    18464 2023-05-18 07:00:49.000000 squander-1.8.2/nn/NN.cpp
+drwxrwxr-x   0 rakytap   (1002) rakytap   (1002)        0 2023-05-18 07:29:19.896699 squander-1.8.2/nn/include/
+-rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     5274 2023-05-18 07:00:49.000000 squander-1.8.2/nn/include/NN.h
+drwxrwxr-x   0 rakytap   (1002) rakytap   (1002)        0 2023-05-18 07:29:19.896699 squander-1.8.2/optimization_engines/
+-rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     9698 2023-05-18 07:00:49.000000 squander-1.8.2/optimization_engines/RL_experience.cpp
+drwxrwxr-x   0 rakytap   (1002) rakytap   (1002)        0 2023-05-18 07:29:19.896699 squander-1.8.2/optimization_engines/include/
+-rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     3549 2023-05-18 07:00:49.000000 squander-1.8.2/optimization_engines/include/RL_experience.h
+-rw-rw-r--   0 rakytap   (1002) rakytap   (1002)      123 2023-05-18 07:00:49.000000 squander-1.8.2/pyproject.toml
+drwxrwxr-x   0 rakytap   (1002) rakytap   (1002)        0 2023-05-18 07:29:19.900699 squander-1.8.2/qgd_python/
+-rw-rw-r--   0 rakytap   (1002) rakytap   (1002)       27 2023-05-18 07:00:49.000000 squander-1.8.2/qgd_python/__init__.py
+drwxrwxr-x   0 rakytap   (1002) rakytap   (1002)        0 2023-05-18 07:29:19.900699 squander-1.8.2/qgd_python/decomposition/
+-rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     4386 2023-05-18 07:00:49.000000 squander-1.8.2/qgd_python/decomposition/CMakeLists.txt
+-rw-rw-r--   0 rakytap   (1002) rakytap   (1002)       27 2023-05-18 07:00:49.000000 squander-1.8.2/qgd_python/decomposition/__init__.py
+-rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     7661 2023-05-18 07:00:49.000000 squander-1.8.2/qgd_python/decomposition/qgd_N_Qubit_Decomposition.py
+-rw-rw-r--   0 rakytap   (1002) rakytap   (1002)    36730 2023-05-18 07:00:49.000000 squander-1.8.2/qgd_python/decomposition/qgd_N_Qubit_Decomposition_Wrapper.cpp
+-rw-rw-r--   0 rakytap   (1002) rakytap   (1002)    25000 2023-05-18 07:01:03.000000 squander-1.8.2/qgd_python/decomposition/qgd_N_Qubit_Decomposition_adaptive.py
+-rw-rw-r--   0 rakytap   (1002) rakytap   (1002)    82645 2023-05-18 07:01:03.000000 squander-1.8.2/qgd_python/decomposition/qgd_N_Qubit_Decomposition_adaptive_Wrapper.cpp
+-rw-rw-r--   0 rakytap   (1002) rakytap   (1002)    14278 2023-05-18 07:00:49.000000 squander-1.8.2/qgd_python/decomposition/qgd_N_Qubit_Decomposition_custom.py
+-rw-rw-r--   0 rakytap   (1002) rakytap   (1002)    41007 2023-05-18 07:00:49.000000 squander-1.8.2/qgd_python/decomposition/qgd_N_Qubit_Decomposition_custom_Wrapper.cpp
+-rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     3367 2023-05-18 07:00:49.000000 squander-1.8.2/qgd_python/decomposition/qgd_N_Qubit_State_Preparation_adaptive.py
+drwxrwxr-x   0 rakytap   (1002) rakytap   (1002)        0 2023-05-18 07:29:19.900699 squander-1.8.2/qgd_python/decomposition/test/
+-rw-rw-r--   0 rakytap   (1002) rakytap   (1002)        0 2023-05-18 07:00:49.000000 squander-1.8.2/qgd_python/decomposition/test/__init__.py
+-rw-rw-r--   0 rakytap   (1002) rakytap   (1002)    11024 2023-05-18 07:00:49.000000 squander-1.8.2/qgd_python/decomposition/test/test_Compression.py
+-rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     1927 2023-05-18 07:00:49.000000 squander-1.8.2/qgd_python/decomposition/test/test_Global_Phase.py
+-rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     7037 2023-05-18 07:00:49.000000 squander-1.8.2/qgd_python/decomposition/test/test_IBM.py
+-rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     1777 2023-05-18 07:00:49.000000 squander-1.8.2/qgd_python/decomposition/test/test_Project_Name.py
+-rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     5616 2023-05-18 07:00:49.000000 squander-1.8.2/qgd_python/decomposition/test/test_QX2.py
+-rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     4399 2023-05-18 07:24:24.000000 squander-1.8.2/qgd_python/decomposition/test/test_State_Preparation.py
+-rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     1656 2023-05-18 07:00:49.000000 squander-1.8.2/qgd_python/decomposition/test/test_Unitary.py
+-rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     4672 2023-05-18 07:00:49.000000 squander-1.8.2/qgd_python/decomposition/test/test_decomposition.py
+-rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     7190 2023-05-18 07:00:49.000000 squander-1.8.2/qgd_python/decomposition/test/test_fmo.py
+-rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     7018 2023-05-18 07:00:49.000000 squander-1.8.2/qgd_python/decomposition/test/test_heavy_hex.py
+-rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     5222 2023-05-18 07:00:49.000000 squander-1.8.2/qgd_python/decomposition/test/test_optmization_problem_combined.py
+-rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     4905 2023-05-18 07:00:49.000000 squander-1.8.2/qgd_python/decomposition/test/test_parametric_circuit.py
+drwxrwxr-x   0 rakytap   (1002) rakytap   (1002)        0 2023-05-18 07:29:19.904699 squander-1.8.2/qgd_python/gates/
+-rw-rw-r--   0 rakytap   (1002) rakytap   (1002)    13547 2023-05-18 07:00:49.000000 squander-1.8.2/qgd_python/gates/CMakeLists.txt
+-rw-rw-r--   0 rakytap   (1002) rakytap   (1002)        0 2023-05-18 07:00:49.000000 squander-1.8.2/qgd_python/gates/__init__.py
+-rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     8219 2023-05-18 07:00:49.000000 squander-1.8.2/qgd_python/gates/qgd_CH.cpp
+-rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     8160 2023-05-18 07:00:49.000000 squander-1.8.2/qgd_python/gates/qgd_CNOT.cpp
+-rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     8033 2023-05-18 07:00:49.000000 squander-1.8.2/qgd_python/gates/qgd_CZ.cpp
+-rw-rw-r--   0 rakytap   (1002) rakytap   (1002)    28536 2023-05-18 07:00:49.000000 squander-1.8.2/qgd_python/gates/qgd_Gates_Block.cpp
+-rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     8529 2023-05-18 07:00:49.000000 squander-1.8.2/qgd_python/gates/qgd_RX.cpp
+-rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     8528 2023-05-18 07:00:49.000000 squander-1.8.2/qgd_python/gates/qgd_RY.cpp
+-rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     8527 2023-05-18 07:00:49.000000 squander-1.8.2/qgd_python/gates/qgd_RZ.cpp
+-rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     7771 2023-05-18 07:00:49.000000 squander-1.8.2/qgd_python/gates/qgd_SX.cpp
+-rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     7801 2023-05-18 07:00:49.000000 squander-1.8.2/qgd_python/gates/qgd_SYC.cpp
+-rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     9054 2023-05-18 07:00:49.000000 squander-1.8.2/qgd_python/gates/qgd_U3.cpp
+-rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     7489 2023-05-18 07:00:49.000000 squander-1.8.2/qgd_python/gates/qgd_X.cpp
+-rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     8367 2023-05-18 07:00:49.000000 squander-1.8.2/qgd_python/gates/qgd_Y.cpp
+-rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     8367 2023-05-18 07:00:49.000000 squander-1.8.2/qgd_python/gates/qgd_Z.cpp
+drwxrwxr-x   0 rakytap   (1002) rakytap   (1002)        0 2023-05-18 07:29:19.908699 squander-1.8.2/qgd_python/gates/test/
+-rw-rw-r--   0 rakytap   (1002) rakytap   (1002)        0 2023-05-18 07:00:49.000000 squander-1.8.2/qgd_python/gates/test/__init__.py
+-rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     3364 2023-05-18 07:00:49.000000 squander-1.8.2/qgd_python/gates/test/test_CH.py
+-rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     3409 2023-05-18 07:00:49.000000 squander-1.8.2/qgd_python/gates/test/test_CNOT.py
+-rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     3444 2023-05-18 07:00:49.000000 squander-1.8.2/qgd_python/gates/test/test_CZ.py
+-rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     3466 2023-05-18 07:00:49.000000 squander-1.8.2/qgd_python/gates/test/test_RX.py
+-rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     3348 2023-05-18 07:00:49.000000 squander-1.8.2/qgd_python/gates/test/test_RY.py
+-rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     3919 2023-05-18 07:00:49.000000 squander-1.8.2/qgd_python/gates/test/test_RZ.py
+-rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     3278 2023-05-18 07:00:49.000000 squander-1.8.2/qgd_python/gates/test/test_SX.py
+-rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     3676 2023-05-18 07:00:49.000000 squander-1.8.2/qgd_python/gates/test/test_U3.py
+-rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     3182 2023-05-18 07:00:49.000000 squander-1.8.2/qgd_python/gates/test/test_X.py
+-rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     3179 2023-05-18 07:00:49.000000 squander-1.8.2/qgd_python/gates/test/test_Y.py
+-rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     3232 2023-05-18 07:00:49.000000 squander-1.8.2/qgd_python/gates/test/test_Z.py
+-rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     6878 2023-05-18 07:00:49.000000 squander-1.8.2/qgd_python/gates/test/test_gates.py
+drwxrwxr-x   0 rakytap   (1002) rakytap   (1002)        0 2023-05-18 07:29:19.908699 squander-1.8.2/qgd_python/nn/
+-rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     1304 2023-05-18 07:00:49.000000 squander-1.8.2/qgd_python/nn/CMakeLists.txt
+-rw-rw-r--   0 rakytap   (1002) rakytap   (1002)       27 2023-05-18 07:00:49.000000 squander-1.8.2/qgd_python/nn/__init__.py
+-rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     2387 2023-05-18 07:00:49.000000 squander-1.8.2/qgd_python/nn/qgd_nn.py
+-rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     9635 2023-05-18 07:00:49.000000 squander-1.8.2/qgd_python/nn/qgd_nn_Wrapper.cpp
+-rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     1573 2023-05-18 07:00:49.000000 squander-1.8.2/qgd_python/utils.py
+drwxrwxr-x   0 rakytap   (1002) rakytap   (1002)        0 2023-05-18 07:29:19.908699 squander-1.8.2/random_unitary/
+-rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     6628 2023-05-18 07:00:49.000000 squander-1.8.2/random_unitary/Random_Orthogonal.cpp
+-rw-rw-r--   0 rakytap   (1002) rakytap   (1002)    11039 2023-05-18 07:00:49.000000 squander-1.8.2/random_unitary/Random_Unitary.cpp
+drwxrwxr-x   0 rakytap   (1002) rakytap   (1002)        0 2023-05-18 07:29:19.908699 squander-1.8.2/random_unitary/include/
+-rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     1927 2023-05-18 07:00:49.000000 squander-1.8.2/random_unitary/include/Random_Orthogonal.h
+-rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     4476 2023-05-18 07:00:49.000000 squander-1.8.2/random_unitary/include/Random_Unitary.h
+-rw-rw-r--   0 rakytap   (1002) rakytap   (1002)       38 2023-05-18 07:29:19.908699 squander-1.8.2/setup.cfg
+-rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     1898 2023-05-18 07:28:49.000000 squander-1.8.2/setup.py
+drwxrwxr-x   0 rakytap   (1002) rakytap   (1002)        0 2023-05-18 07:29:19.908699 squander-1.8.2/squander/
+-rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     1442 2023-05-18 07:00:49.000000 squander-1.8.2/squander/__init__.py
+drwxrwxr-x   0 rakytap   (1002) rakytap   (1002)        0 2023-05-18 07:29:19.908699 squander-1.8.2/squander.egg-info/
+-rw-rw-r--   0 rakytap   (1002) rakytap   (1002)    15001 2023-05-18 07:29:19.000000 squander-1.8.2/squander.egg-info/PKG-INFO
+-rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     5181 2023-05-18 07:29:19.000000 squander-1.8.2/squander.egg-info/SOURCES.txt
+-rw-rw-r--   0 rakytap   (1002) rakytap   (1002)        1 2023-05-18 07:29:19.000000 squander-1.8.2/squander.egg-info/dependency_links.txt
+-rw-rw-r--   0 rakytap   (1002) rakytap   (1002)       50 2023-05-18 07:29:19.000000 squander-1.8.2/squander.egg-info/requires.txt
+-rw-rw-r--   0 rakytap   (1002) rakytap   (1002)       20 2023-05-18 07:29:19.000000 squander-1.8.2/squander.egg-info/top_level.txt
+drwxrwxr-x   0 rakytap   (1002) rakytap   (1002)        0 2023-05-18 07:29:19.908699 squander-1.8.2/test_standalone/
+-rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     1996 2023-05-18 07:00:49.000000 squander-1.8.2/test_standalone/CMakeLists.txt
+-rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     6325 2023-05-18 07:00:49.000000 squander-1.8.2/test_standalone/custom_gate_structure_test.cpp
+-rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     4837 2023-05-18 07:00:49.000000 squander-1.8.2/test_standalone/decomposition_test.cpp
```

### Comparing `squander-1.8.1/CMakeLists.txt` & `squander-1.8.2/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `squander-1.8.1/LICENSE` & `squander-1.8.2/LICENSE`

 * *Files identical despite different names*

### Comparing `squander-1.8.1/PKG-INFO` & `squander-1.8.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: squander
-Version: 1.8.1
-Summary: The C++ binding for the SQUANDER package
+Version: 1.8.2
+Summary: Package to decompose unitaries into a quantum circuit and for quantum state preparation.
 Home-page: https://github.com/rakytap/sequential-quantum-gate-decomposer
 Maintainer: Peter Rakyta
 Maintainer-email: peter.rakyta@ttk.elte.hu
 License: GNU General Public License v3.0
 Keywords: test,cmake,extension
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
```

#### html2text {}

```diff
@@ -1,103 +1,103 @@
-Metadata-Version: 2.1 Name: squander Version: 1.8.1 Summary: The C++ binding
-for the SQUANDER package Home-page: https://github.com/rakytap/sequential-
-quantum-gate-decomposer Maintainer: Peter Rakyta Maintainer-email:
-peter.rakyta@ttk.elte.hu License: GNU General Public License v3.0 Keywords:
-test,cmake,extension Classifier: Intended Audience :: Developers Classifier:
-Natural Language :: English Classifier: Programming Language :: C Classifier:
-Programming Language :: C++ Description-Content-Type: text/markdown License-
-File: LICENSE [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.4508680.svg)]
-(https://doi.org/10.5281/zenodo.4508680) [trackgit-views] # Sequential Quantum
-Gate Decomposer (SQUANDER) The Sequential Quantum Gate Decomposer (SQUANDER)
-package provides a novel solution to decompose any n-qubit unitaries into a
-sequence of one-qubit rotations and two-qubit controlled gates (such as
-controlled NOT or controlled phase gate). SQUANDER utilizes two novel gate
-synthesis techniques reported in Refereces [1] and [2]. (i) To synthesize
-general unitaries SQUANDER applies periodic layers of two-qubit and parametric
-one-qubit gates to an n-qubit unitary such that the resulting unitary is 1-
-qubit decoupled, i.e., is a tensor product of an (n-1)-qubit and a 1-qubit
-unitary. Continuing the decoupling procedure sequentially one arrives at the
-end to a full decomposition of the original unitary into 1- and 2-qubit gates.
-SQUANDER provides lower CNOT counts for generic n-qubit unitaries (up to n=6)
-than the previously provided lower bounds. (ii) An adaptive circuit compression
-is used to optimize quantum circuit by the application of parametric two-qubit
-gates in the synthesis process. The utilization of these parametric two-qubit
-gates in the circuit design allows one to transform the discrete combinatorial
-problem of circuit synthesis into an optimization problem over continuous
-variables. The circuit is then compressed by a sequential removal of two-qubit
-gates from the design, while the remaining building blocks are continuously
-adapted to the reduced gate structure by iterated learning cycles. The SQUANDER
-library is written in C/C++ providing a Python interface via [C++ extensions]
-(https://docs.python.org/3/library/ctypes.html). The present package is
-supplied with Python building script and CMake tools to ease its deployment.
-The SQUANDER package can be built with both Intel and GNU compilers, and can be
-link against various CBLAS libraries installed on the system. (So far the CLBAS
-libraries of the GNU Scientific Library, OpenBLAS and the Intel MKL packages
-were tested.) In the following we briefly summarize the steps to build, install
-and use the SQUANDER package. The project was supported by grant OTKA PD123927
-and by the Ministry of Innovation and Technology and the National Research,
-Development and Innovation Office within the Quantum Information National
-Laboratory of Hungary. Find the documantation of the SQUANDER package at
-[CodeDocs[xyz]](https://codedocs.xyz/rakytap/sequential-quantum-gate-
-decomposer/) ### Contact Us Have a question about the SQUANDER package? Don't
-hesitate to contact us at the following e-mails: * ZoltÃ¡n ZimborÃ¡s
-(researcher): zimboras.zoltan@wigner.hu * Peter Rakyta (developer):
-peter.rakyta@ttk.elte.hu ### Dependencies The dependencies necessary to compile
-and build the SQUANDER package are the followings: * [CMake](https://cmake.org/
-) (>=3.10.2) * C++/C [Intel](https://software.intel.com/content/www/us/en/
-develop/tools/compilers/c-compilers.html) (>=14.0.1) or [GNU](https://
-gcc.gnu.org/) (>=v4.8.1) compiler * [TBB](https://github.com/oneapi-src/oneTBB)
-library (shipped with tbb-devel Python package) * [Intel MKL](https://
-software.intel.com/content/www/us/en/develop/tools/math-kernel-library.html)
-(optional) * [OpenBlas](https://www.openblas.net/) (optional, recommended) *
-[LAPACKE](https://www.netlib.org/lapack/lapacke.html) * [Doxygen](https://
-www.doxygen.nl/index.html) (optional) The Python interface of SQUANDER was
-developed and tested with Python 3.6-3.9. The SQUANDER Python interface needs
-the following packages to be installed on the system: * [Qiskit](https://
-qiskit.org/documentation/install.html) * [Numpy](https://numpy.org/install/) *
-[scipy](https://www.scipy.org/install.html) * [scikit-build](https://scikit-
-build.readthedocs.io/en/latest/) * [tbb-devel](https://pypi.org/project/tbb-
-devel/) (containing the TBB Library) ### Install SQUANDER from Python Package
-Index (PyPI) Since version 1.7.1 the SQUANDER package is accessible at Python
-Package Index (PyPI). The package can be installed on linux systems following
-the steps outlined below: $ pip install numpy swig tbb-devel wheel scikit-build
-ninja qiskit $ pip install squander ### Download the SQUANDER package The
-developer version of the Quantum Gate Decomposer package can be downloaded from
-github repository [https://github.com/rakytap/quantum-gate-decomposer/tree/
-master](https://github.com/rakytap/quantum-gate-decomposer/tree/master). After
-the package is downloaded into the directory **path/to/SQUANDER/package**
-(which would be the path to the source code of the SQUANDER package), one can
-proceed to the compilation steps described in the next section. ### How to
-build the SQUANDER package The SQUANDER package is equipped with a Python build
-script and CMake tools to ease the compilation and the deployment of the
-package. The SQUANDER package is parallelized via Threading Building Block
-(TBB) libraries. If TBB is not present in the system, it can be easily
-installed via python package [tbb-devel](https://pypi.org/project/tbb-devel/).
-Alternatively the TBB libraries can be installed via apt or yum utility (sudo
-apt install libtbb-dev) or it can be downloaded from [https://github.com/
-oneapi-src/oneTBB](https://github.com/oneapi-src/oneTBB) and built from source.
-In this case one should supply the necessary environment variables pointing to
-the header and library files of the TBB package. For newer Intel compilers the
-TBB package is part of the Intel compiler package, similarly to the MKL
-package. If the TBB library is located at non-standrad path or the SQUANDER
-package is compiled with GNU compiler, then setting the $ export
-TBB_LIB_DIR=path/to/TBB/lib(64) $ export TBB_INC_DIR=path/to/TBB/include
-environment variables are sufficient for successful compilation. When the TBB
-library is installed via a python package, setting the environment variables
-above is not necessary. The SQUANDER package with C++ Python extensions can be
-compiled via the Python script **setup.py** located in the root directory of
-the SQUANDER package. The script automatically finds out the CBLAS library
-working behind the numpy package and uses it in further linking. The
-**setup.py** script also build the C++ library of the SQUANDER package by
-making the appropriate CMake calls. ### Developer build We recommend to install
-the SQUANDER package in the Anaconda environment. In order to install the
-necessary requirements, follow the steps below: Creating new python
-environment: $ conda create -n qgd Activate the new anaconda environment $
-conda activate qgd Install dependencies: $ conda install numpy scipy pip pytest
-scikit-build tbb-devel $ pip install qiskit matplotlib After the basic
+Metadata-Version: 2.1 Name: squander Version: 1.8.2 Summary: Package to
+decompose unitaries into a quantum circuit and for quantum state preparation.
+Home-page: https://github.com/rakytap/sequential-quantum-gate-decomposer
+Maintainer: Peter Rakyta Maintainer-email: peter.rakyta@ttk.elte.hu License:
+GNU General Public License v3.0 Keywords: test,cmake,extension Classifier:
+Intended Audience :: Developers Classifier: Natural Language :: English
+Classifier: Programming Language :: C Classifier: Programming Language :: C++
+Description-Content-Type: text/markdown License-File: LICENSE [![DOI](https://
+zenodo.org/badge/DOI/10.5281/zenodo.4508680.svg)](https://doi.org/10.5281/
+zenodo.4508680) [trackgit-views] # Sequential Quantum Gate Decomposer
+(SQUANDER) The Sequential Quantum Gate Decomposer (SQUANDER) package provides a
+novel solution to decompose any n-qubit unitaries into a sequence of one-qubit
+rotations and two-qubit controlled gates (such as controlled NOT or controlled
+phase gate). SQUANDER utilizes two novel gate synthesis techniques reported in
+Refereces [1] and [2]. (i) To synthesize general unitaries SQUANDER applies
+periodic layers of two-qubit and parametric one-qubit gates to an n-qubit
+unitary such that the resulting unitary is 1-qubit decoupled, i.e., is a tensor
+product of an (n-1)-qubit and a 1-qubit unitary. Continuing the decoupling
+procedure sequentially one arrives at the end to a full decomposition of the
+original unitary into 1- and 2-qubit gates. SQUANDER provides lower CNOT counts
+for generic n-qubit unitaries (up to n=6) than the previously provided lower
+bounds. (ii) An adaptive circuit compression is used to optimize quantum
+circuit by the application of parametric two-qubit gates in the synthesis
+process. The utilization of these parametric two-qubit gates in the circuit
+design allows one to transform the discrete combinatorial problem of circuit
+synthesis into an optimization problem over continuous variables. The circuit
+is then compressed by a sequential removal of two-qubit gates from the design,
+while the remaining building blocks are continuously adapted to the reduced
+gate structure by iterated learning cycles. The SQUANDER library is written in
+C/C++ providing a Python interface via [C++ extensions](https://
+docs.python.org/3/library/ctypes.html). The present package is supplied with
+Python building script and CMake tools to ease its deployment. The SQUANDER
+package can be built with both Intel and GNU compilers, and can be link against
+various CBLAS libraries installed on the system. (So far the CLBAS libraries of
+the GNU Scientific Library, OpenBLAS and the Intel MKL packages were tested.)
+In the following we briefly summarize the steps to build, install and use the
+SQUANDER package. The project was supported by grant OTKA PD123927 and by the
+Ministry of Innovation and Technology and the National Research, Development
+and Innovation Office within the Quantum Information National Laboratory of
+Hungary. Find the documantation of the SQUANDER package at [CodeDocs[xyz]]
+(https://codedocs.xyz/rakytap/sequential-quantum-gate-decomposer/) ### Contact
+Us Have a question about the SQUANDER package? Don't hesitate to contact us at
+the following e-mails: * ZoltÃ¡n ZimborÃ¡s (researcher):
+zimboras.zoltan@wigner.hu * Peter Rakyta (developer): peter.rakyta@ttk.elte.hu
+### Dependencies The dependencies necessary to compile and build the SQUANDER
+package are the followings: * [CMake](https://cmake.org/) (>=3.10.2) * C++/C
+[Intel](https://software.intel.com/content/www/us/en/develop/tools/compilers/c-
+compilers.html) (>=14.0.1) or [GNU](https://gcc.gnu.org/) (>=v4.8.1) compiler *
+[TBB](https://github.com/oneapi-src/oneTBB) library (shipped with tbb-devel
+Python package) * [Intel MKL](https://software.intel.com/content/www/us/en/
+develop/tools/math-kernel-library.html) (optional) * [OpenBlas](https://
+www.openblas.net/) (optional, recommended) * [LAPACKE](https://www.netlib.org/
+lapack/lapacke.html) * [Doxygen](https://www.doxygen.nl/index.html) (optional)
+The Python interface of SQUANDER was developed and tested with Python 3.6-3.9.
+The SQUANDER Python interface needs the following packages to be installed on
+the system: * [Qiskit](https://qiskit.org/documentation/install.html) * [Numpy]
+(https://numpy.org/install/) * [scipy](https://www.scipy.org/install.html) *
+[scikit-build](https://scikit-build.readthedocs.io/en/latest/) * [tbb-devel]
+(https://pypi.org/project/tbb-devel/) (containing the TBB Library) ### Install
+SQUANDER from Python Package Index (PyPI) Since version 1.7.1 the SQUANDER
+package is accessible at Python Package Index (PyPI). The package can be
+installed on linux systems following the steps outlined below: $ pip install
+numpy swig tbb-devel wheel scikit-build ninja qiskit $ pip install squander ###
+Download the SQUANDER package The developer version of the Quantum Gate
+Decomposer package can be downloaded from github repository [https://
+github.com/rakytap/quantum-gate-decomposer/tree/master](https://github.com/
+rakytap/quantum-gate-decomposer/tree/master). After the package is downloaded
+into the directory **path/to/SQUANDER/package** (which would be the path to the
+source code of the SQUANDER package), one can proceed to the compilation steps
+described in the next section. ### How to build the SQUANDER package The
+SQUANDER package is equipped with a Python build script and CMake tools to ease
+the compilation and the deployment of the package. The SQUANDER package is
+parallelized via Threading Building Block (TBB) libraries. If TBB is not
+present in the system, it can be easily installed via python package [tbb-
+devel](https://pypi.org/project/tbb-devel/). Alternatively the TBB libraries
+can be installed via apt or yum utility (sudo apt install libtbb-dev) or it can
+be downloaded from [https://github.com/oneapi-src/oneTBB](https://github.com/
+oneapi-src/oneTBB) and built from source. In this case one should supply the
+necessary environment variables pointing to the header and library files of the
+TBB package. For newer Intel compilers the TBB package is part of the Intel
+compiler package, similarly to the MKL package. If the TBB library is located
+at non-standrad path or the SQUANDER package is compiled with GNU compiler,
+then setting the $ export TBB_LIB_DIR=path/to/TBB/lib(64) $ export
+TBB_INC_DIR=path/to/TBB/include environment variables are sufficient for
+successful compilation. When the TBB library is installed via a python package,
+setting the environment variables above is not necessary. The SQUANDER package
+with C++ Python extensions can be compiled via the Python script **setup.py**
+located in the root directory of the SQUANDER package. The script automatically
+finds out the CBLAS library working behind the numpy package and uses it in
+further linking. The **setup.py** script also build the C++ library of the
+SQUANDER package by making the appropriate CMake calls. ### Developer build We
+recommend to install the SQUANDER package in the Anaconda environment. In order
+to install the necessary requirements, follow the steps below: Creating new
+python environment: $ conda create -n qgd Activate the new anaconda environment
+$ conda activate qgd Install dependencies: $ conda install numpy scipy pip
+pytest scikit-build tbb-devel $ pip install qiskit matplotlib After the basic
 environment variables are set and the dependencies are installed, the
 compilation of the package can be started by the Python command: $ python3
 setup.py build_ext The command above starts the compilation of the SQUANDER C++
 library and builds the necessary C++ Python interface extensions of the
 SQUANDER package in place. After a successful build, one can register the
 SQUANDER package in the Python distribution in developer (i.e. editable) mode
 by command: $ python -m pip install -e . ### Binary distribution After the
```

### Comparing `squander-1.8.1/README.md` & `squander-1.8.2/README.md`

 * *Files identical despite different names*

### Comparing `squander-1.8.1/cmake/check_AVX.cmake` & `squander-1.8.2/cmake/check_AVX.cmake`

 * *Files identical despite different names*

### Comparing `squander-1.8.1/common/Adam.cpp` & `squander-1.8.2/common/Adam.cpp`

 * *Files identical despite different names*

### Comparing `squander-1.8.1/common/common.cpp` & `squander-1.8.2/common/common.cpp`

 * *Files identical despite different names*

### Comparing `squander-1.8.1/common/common_DFE.cpp` & `squander-1.8.2/common/common_DFE.cpp`

 * *Files identical despite different names*

### Comparing `squander-1.8.1/common/config_element.cpp` & `squander-1.8.2/common/config_element.cpp`

 * *Files identical despite different names*

### Comparing `squander-1.8.1/common/dot.cpp` & `squander-1.8.2/common/dot.cpp`

 * *Files identical despite different names*

### Comparing `squander-1.8.1/common/include/Adam.h` & `squander-1.8.2/common/include/Adam.h`

 * *Files identical despite different names*

### Comparing `squander-1.8.1/common/include/QGDTypes.h` & `squander-1.8.2/common/include/QGDTypes.h`

 * *Files identical despite different names*

### Comparing `squander-1.8.1/common/include/common.h` & `squander-1.8.2/common/include/common.h`

 * *Files identical despite different names*

### Comparing `squander-1.8.1/common/include/common_DFE.h` & `squander-1.8.2/common/include/common_DFE.h`

 * *Files identical despite different names*

### Comparing `squander-1.8.1/common/include/config_element.h` & `squander-1.8.2/common/include/config_element.h`

 * *Files identical despite different names*

### Comparing `squander-1.8.1/common/include/dot.h` & `squander-1.8.2/common/include/dot.h`

 * *Files identical despite different names*

### Comparing `squander-1.8.1/common/include/lbfgs.h` & `squander-1.8.2/common/include/lbfgs.h`

 * *Files identical despite different names*

### Comparing `squander-1.8.1/common/include/logging.h` & `squander-1.8.2/common/include/logging.h`

 * *Files identical despite different names*

### Comparing `squander-1.8.1/common/include/matrix.h` & `squander-1.8.2/common/include/matrix.h`

 * *Files identical despite different names*

### Comparing `squander-1.8.1/common/include/matrix_base.h` & `squander-1.8.2/common/include/matrix_base.h`

 * *Files identical despite different names*

### Comparing `squander-1.8.1/common/include/matrix_real.h` & `squander-1.8.2/common/include/matrix_real.h`

 * *Files identical despite different names*

### Comparing `squander-1.8.1/common/include/mpi_base.h` & `squander-1.8.2/common/include/mpi_base.h`

 * *Files identical despite different names*

### Comparing `squander-1.8.1/common/include/numpy_interface.h` & `squander-1.8.2/common/include/numpy_interface.h`

 * *Files identical despite different names*

### Comparing `squander-1.8.1/common/include/tolmin.h` & `squander-1.8.2/common/include/tolmin.h`

 * *Files identical despite different names*

### Comparing `squander-1.8.1/common/lbfgs.cpp` & `squander-1.8.2/common/lbfgs.cpp`

 * *Files identical despite different names*

### Comparing `squander-1.8.1/common/logging.cpp` & `squander-1.8.2/common/logging.cpp`

 * *Files identical despite different names*

### Comparing `squander-1.8.1/common/matrix.cpp` & `squander-1.8.2/common/matrix.cpp`

 * *Files identical despite different names*

### Comparing `squander-1.8.1/common/matrix_real.cpp` & `squander-1.8.2/common/matrix_real.cpp`

 * *Files identical despite different names*

### Comparing `squander-1.8.1/common/mpi_base.cpp` & `squander-1.8.2/common/mpi_base.cpp`

 * *Files identical despite different names*

### Comparing `squander-1.8.1/common/numpy_interface.cpp` & `squander-1.8.2/common/numpy_interface.cpp`

 * *Files identical despite different names*

### Comparing `squander-1.8.1/common/tolmin.cpp` & `squander-1.8.2/common/tolmin.cpp`

 * *Files identical despite different names*

### Comparing `squander-1.8.1/decomposition/Decomposition_Base.cpp` & `squander-1.8.2/decomposition/Decomposition_Base.cpp`

 * *Files identical despite different names*

### Comparing `squander-1.8.1/decomposition/N_Qubit_Decomposition.cpp` & `squander-1.8.2/decomposition/N_Qubit_Decomposition.cpp`

 * *Files identical despite different names*

### Comparing `squander-1.8.1/decomposition/N_Qubit_Decomposition_Base.cpp` & `squander-1.8.2/decomposition/N_Qubit_Decomposition_Base.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -817,36 +817,36 @@
 
 
         std::stringstream sstream;
         sstream << "max_inner_iterations: " << max_inner_iterations_loc << std::endl;
         sstream << "agent_lifetime_loc: " << agent_lifetime_loc << std::endl;
         print(sstream, 2); 
 
-
-
-        
-        
-        /// mutual exclusion to set the most successful agent
-        tbb::spin_mutex agent_mutex;
-        
-        double agent_exploration_rate = 0.2;
         double agent_randomization_rate = 0.2;
         
         int agent_num;
         if ( config.count("agent_num") > 0 ) { 
              long long value;                   
              config["agent_num"].get_property( value );  
              agent_num = (int) value;
         }
         else {
             agent_num = 64;
         }
+
+
+        double agent_exploration_rate = 0.2;
+        if ( config.count("agent_exploration_rate") > 0 ) {
+             config["agent_exploration_rate"].get_property( agent_exploration_rate );
+        }
         
         sstream.str("");
         sstream << "AGENTS: number of agents " << agent_num << std::endl;
+        sstream << "AGENTS: exploration_rate " << agent_exploration_rate << std::endl;
+        sstream << "AGENTS: lifetime " << agent_lifetime_loc << std::endl;
         print(sstream, 2);    
     
         
         bool terminate_optimization = false;
         
         // vector stroing the lates values of current minimums to identify convergence
         Matrix_real current_minimum_vec(1, 20); 
@@ -1002,15 +1002,15 @@
             // calculate batched cost function                         
             f0_shifted_pi_agents = optimization_problem_batched( solution_guess_mtx_agents );             
                 
                                                      
             // CPU time                                      
             t0_CPU = tbb::tick_count::now();                                  
             
-            
+         
             // determine the parameters of the cosine function and determine the parameter shift at the minimum
             for ( int agent_idx=0; agent_idx<agent_num; agent_idx++ ) {
 
                 double current_minimum_agent = current_minimum_agents[agent_idx];         
                 double f0_shifted_pi         = f0_shifted_pi_agents[agent_idx];
                 double f0_shifted_pi2        = f0_shifted_pi2_agents[agent_idx];                                                  
             
@@ -1025,23 +1025,25 @@
 
                 double parameter_shift = phi0 > 0 ? M_PI-phi0 : -phi0-M_PI;
 		
 		
                 //update  the parameter vector
                 Matrix_real& solution_guess_mtx_agent                    = solution_guess_mtx_agents[ agent_idx ];                             
                 solution_guess_mtx_agent[param_idx_agents[ agent_idx ]] = parameter_value_save_agents[ agent_idx ] + parameter_shift; 
+
                 
             }
                
             // CPU time                                                     
             CPU_time += (tbb::tick_count::now() - t0_CPU).seconds();
             
             
             // determine the current minimum  at the shifted parameters        
             current_minimum_agents = optimization_problem_batched( solution_guess_mtx_agents ); 
+
   
             // CPU time                                        
             t0_CPU = tbb::tick_count::now();        
 
 
             // generate random numbers to manage the behavior of the agents
             Matrix_real random_numbers(   agent_num, 2 );
@@ -1059,15 +1061,15 @@
 
 #ifdef __MPI__    
             }    
             MPI_Bcast( random_numbers.get_data(), 2*agent_num, MPI_DOUBLE, 0, MPI_COMM_WORLD);
 #endif   
 
 
-
+/*
             // build up probability distribution to use to chose between the agents
             Matrix_real agent_probs(  current_minimum_agents.size(), 1 );
 
             // create probability distribution in each 1000-th iteration
             if ( iter_idx % agent_lifetime_loc == 0 ) {
                 double prob_sum = 0.0;
                 double current_minimum_agents_min = DBL_MAX;
@@ -1086,15 +1088,15 @@
 
                 for( int agent_idx=0; agent_idx<agent_num; agent_idx++ ) {
                     agent_probs[agent_idx] = agent_probs[agent_idx]/prob_sum;
                 }
 
 
             }
-
+*/
             
             // govern the behavior of the agents
             for ( int agent_idx=0; agent_idx<agent_num; agent_idx++ ) {
                 double& current_minimum_agent = current_minimum_agents[ agent_idx ];
                    
            
                 
@@ -1133,21 +1135,24 @@
                         // less successful agent migh choose to keep their current state, or choose the state of more successful agents
                         
 #ifdef __MPI__        
                         if ( current_rank == 0 ) {
 #endif
                                                 
                             double random_num = random_numbers[ agent_idx*random_numbers.stride ]; 
-                                         
+
                             if ( random_num < agent_exploration_rate && agent_idx != most_successfull_agent) {
                                 // choose the state of the most succesfull agent
                             
                                 std::stringstream sstream;
                                 sstream << "agent " << agent_idx << ": adopts the state of the most succesful agent. " << most_successfull_agent << std::endl;
                                 print(sstream, 5);  
+                                
+                                current_minimum_agents[ agent_idx ] = current_minimum_agents[ most_successfull_agent ];
+                                memcpy( solution_guess_mtx_agent.get_data(), solution_guess_mtx_agents[ most_successfull_agent ].get_data(), solution_guess_mtx_agent.size()*sizeof(double) );
 
                             
                                 random_num = random_numbers[ agent_idx*random_numbers.stride + 1 ];
                             
                                 if ( random_num < agent_randomization_rate ) {
                                     randomize_parameters( optimized_parameters_mtx, solution_guess_mtx_agent, radius  );                              
                                 }     
@@ -1755,18 +1760,18 @@
 
 
         // do the optimization loops
         for (long long idx=0; idx<iteration_loops_max; idx++) {
 	    
 
 
-            Problem p(num_of_parameters, 0, 2*M_PI, optimization_problem, optimization_problem_grad, optimization_problem_combined, (void*)this);
+            Problem p(num_of_parameters, -1e100, 1e100, optimization_problem, optimization_problem_grad, optimization_problem_combined, (void*)this);
 
             double f; 
-            if (num_of_parameters > 250) {
+            if (num_of_parameters > 3168) {
                 Lbfgs lbfgs(&p);
                 f = lbfgs.Solve(solution_guess);
             } else {
                 Tolmin tolmin(&p);
                 f = tolmin.Solve(solution_guess, false, max_inner_iterations);
             }
 
@@ -1877,15 +1882,15 @@
         print(sstream, 2); 
 
         // do the optimization loops
         double f = DBL_MAX;
         for (long long iter_idx=0; iter_idx<iteration_loops_max; iter_idx++) {
 
             
-                Problem p(num_of_parameters, 0, 2*M_PI, optimization_problem, optimization_problem_grad, optimization_problem_combined, (void*)this);
+                Problem p(num_of_parameters, -1e100, 1e100, optimization_problem, optimization_problem_grad, optimization_problem_combined, (void*)this);
                 Tolmin tolmin(&p);
 
                 f = tolmin.Solve(solution_guess, false, max_inner_iterations);             
                 
                 if (sub_iter_idx == 1 ) {
                      current_minimum_hold = f;    
                 }
@@ -2360,21 +2365,21 @@
 
     //double f0_DFE = *f0;
 
     //Matrix_real grad_components_DFE_mtx(1, parameter_num_loc);
     for (int idx=0; idx<parameter_num_loc; idx++) {
 
         if ( cost_fnc == FROBENIUS_NORM ) {
-            gsl_vector_set(grad, idx, -trace_DFE_mtx[3*(idx+1)]/Umtx_loc.cols);
+            grad[idx] = -trace_DFE_mtx[3*(idx+1)]/Umtx_loc.cols;
         }
         else if ( cost_fnc == FROBENIUS_NORM_CORRECTION1 ) {
-            gsl_vector_set(grad, idx, -(trace_DFE_mtx[3*(idx+1)] + std::sqrt(prev_cost_fnv_val)*trace_DFE_mtx[3*(idx+1)+1]*correction1_scale)/Umtx_loc.cols);
+            grad[idx] = -(trace_DFE_mtx[3*(idx+1)] + std::sqrt(prev_cost_fnv_val)*trace_DFE_mtx[3*(idx+1)+1]*correction1_scale)/Umtx_loc.cols;
         }
         else if ( cost_fnc == FROBENIUS_NORM_CORRECTION2 ) {
-            gsl_vector_set(grad, idx, -(trace_DFE_mtx[3*(idx+1)] + std::sqrt(prev_cost_fnv_val)*(trace_DFE_mtx[3*(idx+1)+1]*correction1_scale + trace_DFE_mtx[3*(idx+1)+2]*correction2_scale))/Umtx_loc.cols );
+            grad[idx] = -(trace_DFE_mtx[3*(idx+1)] + std::sqrt(prev_cost_fnv_val)*(trace_DFE_mtx[3*(idx+1)+1]*correction1_scale + trace_DFE_mtx[3*(idx+1)+2]*correction2_scale))/Umtx_loc.cols;
         }
         else {
             std::string err("N_Qubit_Decomposition_Base::optimization_problem_combined: Cost function variant not implmented.");
             throw err;
         }
 
         //grad_components_DFE_mtx[idx] = gsl_vector_get( grad, idx );
```

### Comparing `squander-1.8.1/decomposition/N_Qubit_Decomposition_Cost_Function.cpp` & `squander-1.8.2/decomposition/N_Qubit_Decomposition_Cost_Function.cpp`

 * *Files identical despite different names*

### Comparing `squander-1.8.1/decomposition/N_Qubit_Decomposition_adaptive.cpp` & `squander-1.8.2/decomposition/N_Qubit_Decomposition_adaptive.cpp`

 * *Files identical despite different names*

### Comparing `squander-1.8.1/decomposition/N_Qubit_Decomposition_custom.cpp` & `squander-1.8.2/decomposition/N_Qubit_Decomposition_custom.cpp`

 * *Files identical despite different names*

### Comparing `squander-1.8.1/decomposition/Sub_Matrix_Decomposition.cpp` & `squander-1.8.2/decomposition/Sub_Matrix_Decomposition.cpp`

 * *Files identical despite different names*

### Comparing `squander-1.8.1/decomposition/Sub_Matrix_Decomposition_Cost_Function.cpp` & `squander-1.8.2/decomposition/Sub_Matrix_Decomposition_Cost_Function.cpp`

 * *Files identical despite different names*

### Comparing `squander-1.8.1/decomposition/include/Decomposition_Base.h` & `squander-1.8.2/decomposition/include/Decomposition_Base.h`

 * *Files identical despite different names*

### Comparing `squander-1.8.1/decomposition/include/N_Qubit_Decomposition.h` & `squander-1.8.2/decomposition/include/N_Qubit_Decomposition.h`

 * *Files identical despite different names*

### Comparing `squander-1.8.1/decomposition/include/N_Qubit_Decomposition_Base.h` & `squander-1.8.2/decomposition/include/N_Qubit_Decomposition_Base.h`

 * *Files identical despite different names*

### Comparing `squander-1.8.1/decomposition/include/N_Qubit_Decomposition_Cost_Function.h` & `squander-1.8.2/decomposition/include/N_Qubit_Decomposition_Cost_Function.h`

 * *Files identical despite different names*

### Comparing `squander-1.8.1/decomposition/include/N_Qubit_Decomposition_adaptive.h` & `squander-1.8.2/decomposition/include/N_Qubit_Decomposition_adaptive.h`

 * *Files identical despite different names*

### Comparing `squander-1.8.1/decomposition/include/N_Qubit_Decomposition_custom.h` & `squander-1.8.2/decomposition/include/N_Qubit_Decomposition_custom.h`

 * *Files identical despite different names*

### Comparing `squander-1.8.1/decomposition/include/Sub_Matrix_Decomposition.h` & `squander-1.8.2/decomposition/include/Sub_Matrix_Decomposition.h`

 * *Files identical despite different names*

### Comparing `squander-1.8.1/decomposition/include/Sub_Matrix_Decomposition_Cost_Function.h` & `squander-1.8.2/decomposition/include/Sub_Matrix_Decomposition_Cost_Function.h`

 * *Files identical despite different names*

### Comparing `squander-1.8.1/gates/Adaptive.cpp` & `squander-1.8.2/gates/Adaptive.cpp`

 * *Files identical despite different names*

### Comparing `squander-1.8.1/gates/CH.cpp` & `squander-1.8.2/gates/CH.cpp`

 * *Files identical despite different names*

### Comparing `squander-1.8.1/gates/CNOT.cpp` & `squander-1.8.2/gates/CNOT.cpp`

 * *Files identical despite different names*

### Comparing `squander-1.8.1/gates/CRY.cpp` & `squander-1.8.2/gates/CRY.cpp`

 * *Files identical despite different names*

### Comparing `squander-1.8.1/gates/CZ.cpp` & `squander-1.8.2/gates/CZ.cpp`

 * *Files identical despite different names*

### Comparing `squander-1.8.1/gates/Composite.cpp` & `squander-1.8.2/gates/Composite.cpp`

 * *Files identical despite different names*

### Comparing `squander-1.8.1/gates/Gate.cpp` & `squander-1.8.2/gates/Gate.cpp`

 * *Files identical despite different names*

### Comparing `squander-1.8.1/gates/Gates_block.cpp` & `squander-1.8.2/gates/Gates_block.cpp`

 * *Files identical despite different names*

### Comparing `squander-1.8.1/gates/ON.cpp` & `squander-1.8.2/gates/ON.cpp`

 * *Files identical despite different names*

### Comparing `squander-1.8.1/gates/RX.cpp` & `squander-1.8.2/gates/RX.cpp`

 * *Files identical despite different names*

### Comparing `squander-1.8.1/gates/RY.cpp` & `squander-1.8.2/gates/RY.cpp`

 * *Files identical despite different names*

### Comparing `squander-1.8.1/gates/RZ.cpp` & `squander-1.8.2/gates/RZ.cpp`

 * *Files identical despite different names*

### Comparing `squander-1.8.1/gates/SX.cpp` & `squander-1.8.2/gates/SX.cpp`

 * *Files identical despite different names*

### Comparing `squander-1.8.1/gates/SYC.cpp` & `squander-1.8.2/gates/SYC.cpp`

 * *Files identical despite different names*

### Comparing `squander-1.8.1/gates/U3.cpp` & `squander-1.8.2/gates/U3.cpp`

 * *Files identical despite different names*

### Comparing `squander-1.8.1/gates/UN.cpp` & `squander-1.8.2/gates/UN.cpp`

 * *Files identical despite different names*

### Comparing `squander-1.8.1/gates/X.cpp` & `squander-1.8.2/gates/X.cpp`

 * *Files identical despite different names*

### Comparing `squander-1.8.1/gates/Y.cpp` & `squander-1.8.2/gates/Y.cpp`

 * *Files identical despite different names*

### Comparing `squander-1.8.1/gates/Z.cpp` & `squander-1.8.2/gates/Z.cpp`

 * *Files identical despite different names*

### Comparing `squander-1.8.1/gates/include/Adaptive.h` & `squander-1.8.2/gates/include/Adaptive.h`

 * *Files identical despite different names*

### Comparing `squander-1.8.1/gates/include/CH.h` & `squander-1.8.2/gates/include/CH.h`

 * *Files identical despite different names*

### Comparing `squander-1.8.1/gates/include/CNOT.h` & `squander-1.8.2/gates/include/CNOT.h`

 * *Files identical despite different names*

### Comparing `squander-1.8.1/gates/include/CRY.h` & `squander-1.8.2/gates/include/CRY.h`

 * *Files identical despite different names*

### Comparing `squander-1.8.1/gates/include/CZ.h` & `squander-1.8.2/gates/include/CZ.h`

 * *Files identical despite different names*

### Comparing `squander-1.8.1/gates/include/Composite.h` & `squander-1.8.2/gates/include/Composite.h`

 * *Files identical despite different names*

### Comparing `squander-1.8.1/gates/include/Gate.h` & `squander-1.8.2/gates/include/Gate.h`

 * *Files identical despite different names*

### Comparing `squander-1.8.1/gates/include/Gates_block.h` & `squander-1.8.2/gates/include/Gates_block.h`

 * *Files identical despite different names*

### Comparing `squander-1.8.1/gates/include/ON.h` & `squander-1.8.2/gates/include/ON.h`

 * *Files identical despite different names*

### Comparing `squander-1.8.1/gates/include/RX.h` & `squander-1.8.2/gates/include/RX.h`

 * *Files identical despite different names*

### Comparing `squander-1.8.1/gates/include/RY.h` & `squander-1.8.2/gates/include/RY.h`

 * *Files identical despite different names*

### Comparing `squander-1.8.1/gates/include/RZ.h` & `squander-1.8.2/gates/include/RZ.h`

 * *Files identical despite different names*

### Comparing `squander-1.8.1/gates/include/SX.h` & `squander-1.8.2/gates/include/SX.h`

 * *Files identical despite different names*

### Comparing `squander-1.8.1/gates/include/SYC.h` & `squander-1.8.2/gates/include/SYC.h`

 * *Files identical despite different names*

### Comparing `squander-1.8.1/gates/include/U3.h` & `squander-1.8.2/gates/include/U3.h`

 * *Files identical despite different names*

### Comparing `squander-1.8.1/gates/include/UN.h` & `squander-1.8.2/gates/include/UN.h`

 * *Files identical despite different names*

### Comparing `squander-1.8.1/gates/include/X.h` & `squander-1.8.2/gates/include/X.h`

 * *Files identical despite different names*

### Comparing `squander-1.8.1/gates/include/Y.h` & `squander-1.8.2/gates/include/Y.h`

 * *Files identical despite different names*

### Comparing `squander-1.8.1/gates/include/Z.h` & `squander-1.8.2/gates/include/Z.h`

 * *Files identical despite different names*

### Comparing `squander-1.8.1/gates/kernels/apply_kernel_to_input_AVX.cpp` & `squander-1.8.2/gates/kernels/apply_kernel_to_input_AVX.cpp`

 * *Files identical despite different names*

### Comparing `squander-1.8.1/gates/kernels/apply_kernel_to_state_vector_input.cpp` & `squander-1.8.2/gates/kernels/apply_kernel_to_state_vector_input.cpp`

 * *Files identical despite different names*

### Comparing `squander-1.8.1/gates/kernels/include/apply_kernel_to_input_AVX.h` & `squander-1.8.2/gates/kernels/include/apply_kernel_to_input_AVX.h`

 * *Files identical despite different names*

### Comparing `squander-1.8.1/gates/kernels/include/apply_kernel_to_state_vector_input.h` & `squander-1.8.2/gates/kernels/include/apply_kernel_to_state_vector_input.h`

 * *Files identical despite different names*

### Comparing `squander-1.8.1/nn/NN.cpp` & `squander-1.8.2/nn/NN.cpp`

 * *Files identical despite different names*

### Comparing `squander-1.8.1/nn/include/NN.h` & `squander-1.8.2/nn/include/NN.h`

 * *Files identical despite different names*

### Comparing `squander-1.8.1/optimization_engines/RL_experience.cpp` & `squander-1.8.2/optimization_engines/RL_experience.cpp`

 * *Files identical despite different names*

### Comparing `squander-1.8.1/optimization_engines/include/RL_experience.h` & `squander-1.8.2/optimization_engines/include/RL_experience.h`

 * *Files identical despite different names*

### Comparing `squander-1.8.1/qgd_python/decomposition/CMakeLists.txt` & `squander-1.8.2/qgd_python/decomposition/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `squander-1.8.1/qgd_python/decomposition/qgd_N_Qubit_Decomposition.py` & `squander-1.8.2/qgd_python/decomposition/qgd_N_Qubit_Decomposition.py`

 * *Files identical despite different names*

### Comparing `squander-1.8.1/qgd_python/decomposition/qgd_N_Qubit_Decomposition_Wrapper.cpp` & `squander-1.8.2/qgd_python/decomposition/qgd_N_Qubit_Decomposition_Wrapper.cpp`

 * *Files identical despite different names*

### Comparing `squander-1.8.1/qgd_python/decomposition/qgd_N_Qubit_Decomposition_adaptive.py` & `squander-1.8.2/qgd_python/decomposition/qgd_N_Qubit_Decomposition_adaptive.py`

 * *Files 2% similar despite different names*

```diff
@@ -580,14 +580,31 @@
         cost_function = super(qgd_N_Qubit_Decomposition_adaptive, self).Optimization_Problem(parameters)  
 
 
         return cost_function
 
 
 ## 
+# @brief Call to evaluate the gradient components.
+# @param parameters A float64 numpy array
+    def Optimization_Problem_Grad( self, parameters=None ):
+
+        if parameters is None:
+            print( "Optimization_Problem: array of input parameters is None")
+            return None
+
+        # evaluate the cost function and gradients
+        grad = super(qgd_N_Qubit_Decomposition_adaptive, self).Optimization_Problem_Grad(parameters)  
+
+        grad = grad.reshape( (-1,))
+
+        return grad
+
+
+## 
 # @brief Call to evaluate the cost function and the gradient components.
 # @param parameters A float64 numpy array
     def Optimization_Problem_Combined( self, parameters=None ):
 
         if parameters is None:
             print( "Optimization_Problem_Combined: array of input parameters is None")
             return None
```

### Comparing `squander-1.8.1/qgd_python/decomposition/qgd_N_Qubit_Decomposition_adaptive_Wrapper.cpp` & `squander-1.8.2/qgd_python/decomposition/qgd_N_Qubit_Decomposition_adaptive_Wrapper.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -1503,15 +1503,75 @@
     Py_DECREF(parameters_arg);
 
 
     return Py_BuildValue("d", f0);
 }
 
 
+/**
+@brief Wrapper function to evaluate the cost function an dthe gradient components.
+@return Unitarty numpy matrix
+*/
+static PyObject *
+qgd_N_Qubit_Decomposition_adaptive_Wrapper_Optimization_Problem_Grad( qgd_N_Qubit_Decomposition_adaptive_Wrapper *self, PyObject *args)
+{
+
+
+    PyObject* parameters_arg = NULL;
+
+
+    // parsing input arguments
+    if (!PyArg_ParseTuple(args, "|O", &parameters_arg )) {
+
+        std::string err( "Unsuccessful argument parsing not ");
+        PyErr_SetString(PyExc_Exception, err.c_str());
+        return NULL;      
+
+    } 
+
+    // establish memory contiguous arrays for C calculations
+    if ( PyArray_IS_C_CONTIGUOUS(parameters_arg) && PyArray_TYPE(parameters_arg) == NPY_FLOAT64 ){
+        Py_INCREF(parameters_arg);
+    }
+    else if (PyArray_TYPE(parameters_arg) == NPY_FLOAT64 ) {
+        parameters_arg = PyArray_FROM_OTF(parameters_arg, NPY_FLOAT64, NPY_ARRAY_IN_ARRAY);
+    }
+    else {
+        std::string err( "Parameters should be should be real (given in float64 format)");
+        PyErr_SetString(PyExc_Exception, err.c_str());
+        return NULL;
+    }
+
 
+    Matrix_real parameters_mtx = numpy2matrix_real( parameters_arg );
+    Matrix_real grad_mtx(parameters_mtx.size(), 1);
+
+    try {
+        self->decomp->optimization_problem_grad(parameters_mtx, &self->decomp, grad_mtx );
+    }
+    catch (std::string err ) {
+        PyErr_SetString(PyExc_Exception, err.c_str());
+        return NULL;
+    }
+    catch (...) {
+        std::string err( "Invalid pointer to decomposition class");
+        PyErr_SetString(PyExc_Exception, err.c_str());
+        return NULL;
+    }
+
+    // convert to numpy array
+    grad_mtx.set_owner(false);
+    PyObject *grad_py = matrix_real_to_numpy( grad_mtx );
+
+    Py_DECREF(parameters_arg);
+
+
+    Py_DECREF(grad_py);
+    return grad_py;
+}
 
 /**
 @brief Wrapper function to evaluate the cost function an dthe gradient components.
 @return Unitarty numpy matrix
 */
 static PyObject *
 qgd_N_Qubit_Decomposition_adaptive_Wrapper_Optimization_Problem_Combined( qgd_N_Qubit_Decomposition_adaptive_Wrapper *self, PyObject *args)
@@ -2348,14 +2408,17 @@
     },
     {"Optimization_Problem", (PyCFunction) qgd_N_Qubit_Decomposition_adaptive_Wrapper_Optimization_Problem, METH_VARARGS,
      "Wrapper function to evaluate the cost function."
     },
     {"Optimization_Problem_Combined_Unitary", (PyCFunction) qgd_N_Qubit_Decomposition_adaptive_Wrapper_Optimization_Problem_Combined_Unitary, METH_VARARGS,
      "Wrapper function to evaluate the unitary function and the gradient components."
     },	
+    {"Optimization_Problem_Grad", (PyCFunction) qgd_N_Qubit_Decomposition_adaptive_Wrapper_Optimization_Problem_Grad, METH_VARARGS,
+     "Wrapper function to evaluate the gradient components."
+    },
     {"Optimization_Problem_Combined", (PyCFunction) qgd_N_Qubit_Decomposition_adaptive_Wrapper_Optimization_Problem_Combined, METH_VARARGS,
      "Wrapper function to evaluate the cost function and the gradient components."
     },
     {"Optimization_Problem_Batch", (PyCFunction) qgd_N_Qubit_Decomposition_adaptive_Wrapper_Optimization_Problem_Batch, METH_VARARGS,
      "Wrapper function to evaluate the cost function of batch."
     },
     {"Upload_Umtx_to_DFE", (PyCFunction) qgd_N_Qubit_Decomposition_adaptive_Wrapper_Upload_Umtx_to_DFE, METH_NOARGS,
```

### Comparing `squander-1.8.1/qgd_python/decomposition/qgd_N_Qubit_Decomposition_custom.py` & `squander-1.8.2/qgd_python/decomposition/qgd_N_Qubit_Decomposition_custom.py`

 * *Files identical despite different names*

### Comparing `squander-1.8.1/qgd_python/decomposition/qgd_N_Qubit_Decomposition_custom_Wrapper.cpp` & `squander-1.8.2/qgd_python/decomposition/qgd_N_Qubit_Decomposition_custom_Wrapper.cpp`

 * *Files identical despite different names*

### Comparing `squander-1.8.1/qgd_python/decomposition/qgd_N_Qubit_State_Preparation_adaptive.py` & `squander-1.8.2/qgd_python/decomposition/qgd_N_Qubit_State_Preparation_adaptive.py`

 * *Files identical despite different names*

### Comparing `squander-1.8.1/qgd_python/decomposition/test/test_Compression.py` & `squander-1.8.2/qgd_python/decomposition/test/test_Compression.py`

 * *Files identical despite different names*

### Comparing `squander-1.8.1/qgd_python/decomposition/test/test_Global_Phase.py` & `squander-1.8.2/qgd_python/decomposition/test/test_Global_Phase.py`

 * *Files identical despite different names*

### Comparing `squander-1.8.1/qgd_python/decomposition/test/test_IBM.py` & `squander-1.8.2/qgd_python/decomposition/test/test_IBM.py`

 * *Files identical despite different names*

### Comparing `squander-1.8.1/qgd_python/decomposition/test/test_Project_Name.py` & `squander-1.8.2/qgd_python/decomposition/test/test_Project_Name.py`

 * *Files identical despite different names*

### Comparing `squander-1.8.1/qgd_python/decomposition/test/test_QX2.py` & `squander-1.8.2/qgd_python/decomposition/test/test_QX2.py`

 * *Files identical despite different names*

### Comparing `squander-1.8.1/qgd_python/decomposition/test/test_State_Preparation.py` & `squander-1.8.2/qgd_python/decomposition/test/test_State_Preparation.py`

 * *Files identical despite different names*

### Comparing `squander-1.8.1/qgd_python/decomposition/test/test_Unitary.py` & `squander-1.8.2/qgd_python/decomposition/test/test_Unitary.py`

 * *Files identical despite different names*

### Comparing `squander-1.8.1/qgd_python/decomposition/test/test_decomposition.py` & `squander-1.8.2/qgd_python/decomposition/test/test_decomposition.py`

 * *Files identical despite different names*

### Comparing `squander-1.8.1/qgd_python/decomposition/test/test_fmo.py` & `squander-1.8.2/qgd_python/decomposition/test/test_fmo.py`

 * *Files identical despite different names*

### Comparing `squander-1.8.1/qgd_python/decomposition/test/test_heavy_hex.py` & `squander-1.8.2/qgd_python/decomposition/test/test_heavy_hex.py`

 * *Files identical despite different names*

### Comparing `squander-1.8.1/qgd_python/decomposition/test/test_optmization_problem_combined.py` & `squander-1.8.2/qgd_python/decomposition/test/test_optmization_problem_combined.py`

 * *Files identical despite different names*

### Comparing `squander-1.8.1/qgd_python/decomposition/test/test_parametric_circuit.py` & `squander-1.8.2/qgd_python/decomposition/test/test_parametric_circuit.py`

 * *Files identical despite different names*

### Comparing `squander-1.8.1/qgd_python/gates/CMakeLists.txt` & `squander-1.8.2/qgd_python/gates/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `squander-1.8.1/qgd_python/gates/qgd_CH.cpp` & `squander-1.8.2/qgd_python/gates/qgd_CH.cpp`

 * *Files identical despite different names*

### Comparing `squander-1.8.1/qgd_python/gates/qgd_CNOT.cpp` & `squander-1.8.2/qgd_python/gates/qgd_CNOT.cpp`

 * *Files identical despite different names*

### Comparing `squander-1.8.1/qgd_python/gates/qgd_CZ.cpp` & `squander-1.8.2/qgd_python/gates/qgd_CZ.cpp`

 * *Files identical despite different names*

### Comparing `squander-1.8.1/qgd_python/gates/qgd_Gates_Block.cpp` & `squander-1.8.2/qgd_python/gates/qgd_Gates_Block.cpp`

 * *Files identical despite different names*

### Comparing `squander-1.8.1/qgd_python/gates/qgd_RX.cpp` & `squander-1.8.2/qgd_python/gates/qgd_RX.cpp`

 * *Files identical despite different names*

### Comparing `squander-1.8.1/qgd_python/gates/qgd_RY.cpp` & `squander-1.8.2/qgd_python/gates/qgd_RY.cpp`

 * *Files identical despite different names*

### Comparing `squander-1.8.1/qgd_python/gates/qgd_RZ.cpp` & `squander-1.8.2/qgd_python/gates/qgd_RZ.cpp`

 * *Files identical despite different names*

### Comparing `squander-1.8.1/qgd_python/gates/qgd_SX.cpp` & `squander-1.8.2/qgd_python/gates/qgd_SX.cpp`

 * *Files identical despite different names*

### Comparing `squander-1.8.1/qgd_python/gates/qgd_SYC.cpp` & `squander-1.8.2/qgd_python/gates/qgd_SYC.cpp`

 * *Files identical despite different names*

### Comparing `squander-1.8.1/qgd_python/gates/qgd_U3.cpp` & `squander-1.8.2/qgd_python/gates/qgd_U3.cpp`

 * *Files identical despite different names*

### Comparing `squander-1.8.1/qgd_python/gates/qgd_X.cpp` & `squander-1.8.2/qgd_python/gates/qgd_X.cpp`

 * *Files identical despite different names*

### Comparing `squander-1.8.1/qgd_python/gates/qgd_Y.cpp` & `squander-1.8.2/qgd_python/gates/qgd_Y.cpp`

 * *Files identical despite different names*

### Comparing `squander-1.8.1/qgd_python/gates/qgd_Z.cpp` & `squander-1.8.2/qgd_python/gates/qgd_Z.cpp`

 * *Files identical despite different names*

### Comparing `squander-1.8.1/qgd_python/gates/test/test_CH.py` & `squander-1.8.2/qgd_python/gates/test/test_CH.py`

 * *Files identical despite different names*

### Comparing `squander-1.8.1/qgd_python/gates/test/test_CNOT.py` & `squander-1.8.2/qgd_python/gates/test/test_CNOT.py`

 * *Files identical despite different names*

### Comparing `squander-1.8.1/qgd_python/gates/test/test_CZ.py` & `squander-1.8.2/qgd_python/gates/test/test_CZ.py`

 * *Files identical despite different names*

### Comparing `squander-1.8.1/qgd_python/gates/test/test_RX.py` & `squander-1.8.2/qgd_python/gates/test/test_RX.py`

 * *Files identical despite different names*

### Comparing `squander-1.8.1/qgd_python/gates/test/test_RY.py` & `squander-1.8.2/qgd_python/gates/test/test_RY.py`

 * *Files identical despite different names*

### Comparing `squander-1.8.1/qgd_python/gates/test/test_RZ.py` & `squander-1.8.2/qgd_python/gates/test/test_RZ.py`

 * *Files identical despite different names*

### Comparing `squander-1.8.1/qgd_python/gates/test/test_SX.py` & `squander-1.8.2/qgd_python/gates/test/test_SX.py`

 * *Files identical despite different names*

### Comparing `squander-1.8.1/qgd_python/gates/test/test_U3.py` & `squander-1.8.2/qgd_python/gates/test/test_U3.py`

 * *Files identical despite different names*

### Comparing `squander-1.8.1/qgd_python/gates/test/test_X.py` & `squander-1.8.2/qgd_python/gates/test/test_X.py`

 * *Files identical despite different names*

### Comparing `squander-1.8.1/qgd_python/gates/test/test_Y.py` & `squander-1.8.2/qgd_python/gates/test/test_Y.py`

 * *Files identical despite different names*

### Comparing `squander-1.8.1/qgd_python/gates/test/test_Z.py` & `squander-1.8.2/qgd_python/gates/test/test_Z.py`

 * *Files identical despite different names*

### Comparing `squander-1.8.1/qgd_python/gates/test/test_gates.py` & `squander-1.8.2/qgd_python/gates/test/test_gates.py`

 * *Files identical despite different names*

### Comparing `squander-1.8.1/qgd_python/nn/CMakeLists.txt` & `squander-1.8.2/qgd_python/nn/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `squander-1.8.1/qgd_python/nn/qgd_nn.py` & `squander-1.8.2/qgd_python/nn/qgd_nn.py`

 * *Files identical despite different names*

### Comparing `squander-1.8.1/qgd_python/nn/qgd_nn_Wrapper.cpp` & `squander-1.8.2/qgd_python/nn/qgd_nn_Wrapper.cpp`

 * *Files identical despite different names*

### Comparing `squander-1.8.1/qgd_python/utils.py` & `squander-1.8.2/qgd_python/utils.py`

 * *Files identical despite different names*

### Comparing `squander-1.8.1/random_unitary/Random_Orthogonal.cpp` & `squander-1.8.2/random_unitary/Random_Orthogonal.cpp`

 * *Files identical despite different names*

### Comparing `squander-1.8.1/random_unitary/Random_Unitary.cpp` & `squander-1.8.2/random_unitary/Random_Unitary.cpp`

 * *Files identical despite different names*

### Comparing `squander-1.8.1/random_unitary/include/Random_Orthogonal.h` & `squander-1.8.2/random_unitary/include/Random_Orthogonal.h`

 * *Files identical despite different names*

### Comparing `squander-1.8.1/random_unitary/include/Random_Unitary.h` & `squander-1.8.2/random_unitary/include/Random_Unitary.h`

 * *Files identical despite different names*

### Comparing `squander-1.8.1/setup.py` & `squander-1.8.2/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -30,28 +30,28 @@
 setup(
     name="squander",
     packages=find_packages(
         exclude=(
             "test_standalone", "test_standalone.*",
         )
     ),
-    version='1.8.1',
+    version='1.8.2',
     url="https://github.com/rakytap/sequential-quantum-gate-decomposer", 
     maintainer="Peter Rakyta",
     maintainer_email="peter.rakyta@ttk.elte.hu",
     include_package_data=True,
     install_requires=[
         "setuptools>=40.8.0",
         "wheel",
         "scikit-build",          
         "ninja",
         "scipy",
     ],
     tests_require=["pytest"],
-    description='The C++ binding for the SQUANDER package',
+    description='Package to decompose unitaries into a quantum circuit and for quantum state preparation.',
     long_description=open("./README.md", 'r').read(),
     long_description_content_type="text/markdown",
     keywords="test, cmake, extension",
     classifiers=[
         "Intended Audience :: Developers",
         "Natural Language :: English",
         "Programming Language :: C",
```

### Comparing `squander-1.8.1/squander/__init__.py` & `squander-1.8.2/squander/__init__.py`

 * *Files identical despite different names*

### Comparing `squander-1.8.1/squander.egg-info/PKG-INFO` & `squander-1.8.2/squander.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: squander
-Version: 1.8.1
-Summary: The C++ binding for the SQUANDER package
+Version: 1.8.2
+Summary: Package to decompose unitaries into a quantum circuit and for quantum state preparation.
 Home-page: https://github.com/rakytap/sequential-quantum-gate-decomposer
 Maintainer: Peter Rakyta
 Maintainer-email: peter.rakyta@ttk.elte.hu
 License: GNU General Public License v3.0
 Keywords: test,cmake,extension
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
```

#### html2text {}

```diff
@@ -1,103 +1,103 @@
-Metadata-Version: 2.1 Name: squander Version: 1.8.1 Summary: The C++ binding
-for the SQUANDER package Home-page: https://github.com/rakytap/sequential-
-quantum-gate-decomposer Maintainer: Peter Rakyta Maintainer-email:
-peter.rakyta@ttk.elte.hu License: GNU General Public License v3.0 Keywords:
-test,cmake,extension Classifier: Intended Audience :: Developers Classifier:
-Natural Language :: English Classifier: Programming Language :: C Classifier:
-Programming Language :: C++ Description-Content-Type: text/markdown License-
-File: LICENSE [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.4508680.svg)]
-(https://doi.org/10.5281/zenodo.4508680) [trackgit-views] # Sequential Quantum
-Gate Decomposer (SQUANDER) The Sequential Quantum Gate Decomposer (SQUANDER)
-package provides a novel solution to decompose any n-qubit unitaries into a
-sequence of one-qubit rotations and two-qubit controlled gates (such as
-controlled NOT or controlled phase gate). SQUANDER utilizes two novel gate
-synthesis techniques reported in Refereces [1] and [2]. (i) To synthesize
-general unitaries SQUANDER applies periodic layers of two-qubit and parametric
-one-qubit gates to an n-qubit unitary such that the resulting unitary is 1-
-qubit decoupled, i.e., is a tensor product of an (n-1)-qubit and a 1-qubit
-unitary. Continuing the decoupling procedure sequentially one arrives at the
-end to a full decomposition of the original unitary into 1- and 2-qubit gates.
-SQUANDER provides lower CNOT counts for generic n-qubit unitaries (up to n=6)
-than the previously provided lower bounds. (ii) An adaptive circuit compression
-is used to optimize quantum circuit by the application of parametric two-qubit
-gates in the synthesis process. The utilization of these parametric two-qubit
-gates in the circuit design allows one to transform the discrete combinatorial
-problem of circuit synthesis into an optimization problem over continuous
-variables. The circuit is then compressed by a sequential removal of two-qubit
-gates from the design, while the remaining building blocks are continuously
-adapted to the reduced gate structure by iterated learning cycles. The SQUANDER
-library is written in C/C++ providing a Python interface via [C++ extensions]
-(https://docs.python.org/3/library/ctypes.html). The present package is
-supplied with Python building script and CMake tools to ease its deployment.
-The SQUANDER package can be built with both Intel and GNU compilers, and can be
-link against various CBLAS libraries installed on the system. (So far the CLBAS
-libraries of the GNU Scientific Library, OpenBLAS and the Intel MKL packages
-were tested.) In the following we briefly summarize the steps to build, install
-and use the SQUANDER package. The project was supported by grant OTKA PD123927
-and by the Ministry of Innovation and Technology and the National Research,
-Development and Innovation Office within the Quantum Information National
-Laboratory of Hungary. Find the documantation of the SQUANDER package at
-[CodeDocs[xyz]](https://codedocs.xyz/rakytap/sequential-quantum-gate-
-decomposer/) ### Contact Us Have a question about the SQUANDER package? Don't
-hesitate to contact us at the following e-mails: * ZoltÃ¡n ZimborÃ¡s
-(researcher): zimboras.zoltan@wigner.hu * Peter Rakyta (developer):
-peter.rakyta@ttk.elte.hu ### Dependencies The dependencies necessary to compile
-and build the SQUANDER package are the followings: * [CMake](https://cmake.org/
-) (>=3.10.2) * C++/C [Intel](https://software.intel.com/content/www/us/en/
-develop/tools/compilers/c-compilers.html) (>=14.0.1) or [GNU](https://
-gcc.gnu.org/) (>=v4.8.1) compiler * [TBB](https://github.com/oneapi-src/oneTBB)
-library (shipped with tbb-devel Python package) * [Intel MKL](https://
-software.intel.com/content/www/us/en/develop/tools/math-kernel-library.html)
-(optional) * [OpenBlas](https://www.openblas.net/) (optional, recommended) *
-[LAPACKE](https://www.netlib.org/lapack/lapacke.html) * [Doxygen](https://
-www.doxygen.nl/index.html) (optional) The Python interface of SQUANDER was
-developed and tested with Python 3.6-3.9. The SQUANDER Python interface needs
-the following packages to be installed on the system: * [Qiskit](https://
-qiskit.org/documentation/install.html) * [Numpy](https://numpy.org/install/) *
-[scipy](https://www.scipy.org/install.html) * [scikit-build](https://scikit-
-build.readthedocs.io/en/latest/) * [tbb-devel](https://pypi.org/project/tbb-
-devel/) (containing the TBB Library) ### Install SQUANDER from Python Package
-Index (PyPI) Since version 1.7.1 the SQUANDER package is accessible at Python
-Package Index (PyPI). The package can be installed on linux systems following
-the steps outlined below: $ pip install numpy swig tbb-devel wheel scikit-build
-ninja qiskit $ pip install squander ### Download the SQUANDER package The
-developer version of the Quantum Gate Decomposer package can be downloaded from
-github repository [https://github.com/rakytap/quantum-gate-decomposer/tree/
-master](https://github.com/rakytap/quantum-gate-decomposer/tree/master). After
-the package is downloaded into the directory **path/to/SQUANDER/package**
-(which would be the path to the source code of the SQUANDER package), one can
-proceed to the compilation steps described in the next section. ### How to
-build the SQUANDER package The SQUANDER package is equipped with a Python build
-script and CMake tools to ease the compilation and the deployment of the
-package. The SQUANDER package is parallelized via Threading Building Block
-(TBB) libraries. If TBB is not present in the system, it can be easily
-installed via python package [tbb-devel](https://pypi.org/project/tbb-devel/).
-Alternatively the TBB libraries can be installed via apt or yum utility (sudo
-apt install libtbb-dev) or it can be downloaded from [https://github.com/
-oneapi-src/oneTBB](https://github.com/oneapi-src/oneTBB) and built from source.
-In this case one should supply the necessary environment variables pointing to
-the header and library files of the TBB package. For newer Intel compilers the
-TBB package is part of the Intel compiler package, similarly to the MKL
-package. If the TBB library is located at non-standrad path or the SQUANDER
-package is compiled with GNU compiler, then setting the $ export
-TBB_LIB_DIR=path/to/TBB/lib(64) $ export TBB_INC_DIR=path/to/TBB/include
-environment variables are sufficient for successful compilation. When the TBB
-library is installed via a python package, setting the environment variables
-above is not necessary. The SQUANDER package with C++ Python extensions can be
-compiled via the Python script **setup.py** located in the root directory of
-the SQUANDER package. The script automatically finds out the CBLAS library
-working behind the numpy package and uses it in further linking. The
-**setup.py** script also build the C++ library of the SQUANDER package by
-making the appropriate CMake calls. ### Developer build We recommend to install
-the SQUANDER package in the Anaconda environment. In order to install the
-necessary requirements, follow the steps below: Creating new python
-environment: $ conda create -n qgd Activate the new anaconda environment $
-conda activate qgd Install dependencies: $ conda install numpy scipy pip pytest
-scikit-build tbb-devel $ pip install qiskit matplotlib After the basic
+Metadata-Version: 2.1 Name: squander Version: 1.8.2 Summary: Package to
+decompose unitaries into a quantum circuit and for quantum state preparation.
+Home-page: https://github.com/rakytap/sequential-quantum-gate-decomposer
+Maintainer: Peter Rakyta Maintainer-email: peter.rakyta@ttk.elte.hu License:
+GNU General Public License v3.0 Keywords: test,cmake,extension Classifier:
+Intended Audience :: Developers Classifier: Natural Language :: English
+Classifier: Programming Language :: C Classifier: Programming Language :: C++
+Description-Content-Type: text/markdown License-File: LICENSE [![DOI](https://
+zenodo.org/badge/DOI/10.5281/zenodo.4508680.svg)](https://doi.org/10.5281/
+zenodo.4508680) [trackgit-views] # Sequential Quantum Gate Decomposer
+(SQUANDER) The Sequential Quantum Gate Decomposer (SQUANDER) package provides a
+novel solution to decompose any n-qubit unitaries into a sequence of one-qubit
+rotations and two-qubit controlled gates (such as controlled NOT or controlled
+phase gate). SQUANDER utilizes two novel gate synthesis techniques reported in
+Refereces [1] and [2]. (i) To synthesize general unitaries SQUANDER applies
+periodic layers of two-qubit and parametric one-qubit gates to an n-qubit
+unitary such that the resulting unitary is 1-qubit decoupled, i.e., is a tensor
+product of an (n-1)-qubit and a 1-qubit unitary. Continuing the decoupling
+procedure sequentially one arrives at the end to a full decomposition of the
+original unitary into 1- and 2-qubit gates. SQUANDER provides lower CNOT counts
+for generic n-qubit unitaries (up to n=6) than the previously provided lower
+bounds. (ii) An adaptive circuit compression is used to optimize quantum
+circuit by the application of parametric two-qubit gates in the synthesis
+process. The utilization of these parametric two-qubit gates in the circuit
+design allows one to transform the discrete combinatorial problem of circuit
+synthesis into an optimization problem over continuous variables. The circuit
+is then compressed by a sequential removal of two-qubit gates from the design,
+while the remaining building blocks are continuously adapted to the reduced
+gate structure by iterated learning cycles. The SQUANDER library is written in
+C/C++ providing a Python interface via [C++ extensions](https://
+docs.python.org/3/library/ctypes.html). The present package is supplied with
+Python building script and CMake tools to ease its deployment. The SQUANDER
+package can be built with both Intel and GNU compilers, and can be link against
+various CBLAS libraries installed on the system. (So far the CLBAS libraries of
+the GNU Scientific Library, OpenBLAS and the Intel MKL packages were tested.)
+In the following we briefly summarize the steps to build, install and use the
+SQUANDER package. The project was supported by grant OTKA PD123927 and by the
+Ministry of Innovation and Technology and the National Research, Development
+and Innovation Office within the Quantum Information National Laboratory of
+Hungary. Find the documantation of the SQUANDER package at [CodeDocs[xyz]]
+(https://codedocs.xyz/rakytap/sequential-quantum-gate-decomposer/) ### Contact
+Us Have a question about the SQUANDER package? Don't hesitate to contact us at
+the following e-mails: * ZoltÃ¡n ZimborÃ¡s (researcher):
+zimboras.zoltan@wigner.hu * Peter Rakyta (developer): peter.rakyta@ttk.elte.hu
+### Dependencies The dependencies necessary to compile and build the SQUANDER
+package are the followings: * [CMake](https://cmake.org/) (>=3.10.2) * C++/C
+[Intel](https://software.intel.com/content/www/us/en/develop/tools/compilers/c-
+compilers.html) (>=14.0.1) or [GNU](https://gcc.gnu.org/) (>=v4.8.1) compiler *
+[TBB](https://github.com/oneapi-src/oneTBB) library (shipped with tbb-devel
+Python package) * [Intel MKL](https://software.intel.com/content/www/us/en/
+develop/tools/math-kernel-library.html) (optional) * [OpenBlas](https://
+www.openblas.net/) (optional, recommended) * [LAPACKE](https://www.netlib.org/
+lapack/lapacke.html) * [Doxygen](https://www.doxygen.nl/index.html) (optional)
+The Python interface of SQUANDER was developed and tested with Python 3.6-3.9.
+The SQUANDER Python interface needs the following packages to be installed on
+the system: * [Qiskit](https://qiskit.org/documentation/install.html) * [Numpy]
+(https://numpy.org/install/) * [scipy](https://www.scipy.org/install.html) *
+[scikit-build](https://scikit-build.readthedocs.io/en/latest/) * [tbb-devel]
+(https://pypi.org/project/tbb-devel/) (containing the TBB Library) ### Install
+SQUANDER from Python Package Index (PyPI) Since version 1.7.1 the SQUANDER
+package is accessible at Python Package Index (PyPI). The package can be
+installed on linux systems following the steps outlined below: $ pip install
+numpy swig tbb-devel wheel scikit-build ninja qiskit $ pip install squander ###
+Download the SQUANDER package The developer version of the Quantum Gate
+Decomposer package can be downloaded from github repository [https://
+github.com/rakytap/quantum-gate-decomposer/tree/master](https://github.com/
+rakytap/quantum-gate-decomposer/tree/master). After the package is downloaded
+into the directory **path/to/SQUANDER/package** (which would be the path to the
+source code of the SQUANDER package), one can proceed to the compilation steps
+described in the next section. ### How to build the SQUANDER package The
+SQUANDER package is equipped with a Python build script and CMake tools to ease
+the compilation and the deployment of the package. The SQUANDER package is
+parallelized via Threading Building Block (TBB) libraries. If TBB is not
+present in the system, it can be easily installed via python package [tbb-
+devel](https://pypi.org/project/tbb-devel/). Alternatively the TBB libraries
+can be installed via apt or yum utility (sudo apt install libtbb-dev) or it can
+be downloaded from [https://github.com/oneapi-src/oneTBB](https://github.com/
+oneapi-src/oneTBB) and built from source. In this case one should supply the
+necessary environment variables pointing to the header and library files of the
+TBB package. For newer Intel compilers the TBB package is part of the Intel
+compiler package, similarly to the MKL package. If the TBB library is located
+at non-standrad path or the SQUANDER package is compiled with GNU compiler,
+then setting the $ export TBB_LIB_DIR=path/to/TBB/lib(64) $ export
+TBB_INC_DIR=path/to/TBB/include environment variables are sufficient for
+successful compilation. When the TBB library is installed via a python package,
+setting the environment variables above is not necessary. The SQUANDER package
+with C++ Python extensions can be compiled via the Python script **setup.py**
+located in the root directory of the SQUANDER package. The script automatically
+finds out the CBLAS library working behind the numpy package and uses it in
+further linking. The **setup.py** script also build the C++ library of the
+SQUANDER package by making the appropriate CMake calls. ### Developer build We
+recommend to install the SQUANDER package in the Anaconda environment. In order
+to install the necessary requirements, follow the steps below: Creating new
+python environment: $ conda create -n qgd Activate the new anaconda environment
+$ conda activate qgd Install dependencies: $ conda install numpy scipy pip
+pytest scikit-build tbb-devel $ pip install qiskit matplotlib After the basic
 environment variables are set and the dependencies are installed, the
 compilation of the package can be started by the Python command: $ python3
 setup.py build_ext The command above starts the compilation of the SQUANDER C++
 library and builds the necessary C++ Python interface extensions of the
 SQUANDER package in place. After a successful build, one can register the
 SQUANDER package in the Python distribution in developer (i.e. editable) mode
 by command: $ python -m pip install -e . ### Binary distribution After the
```

### Comparing `squander-1.8.1/squander.egg-info/SOURCES.txt` & `squander-1.8.2/squander.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,27 +1,29 @@
 CMakeLists.txt
 LICENSE
 MANIFEST.in
 README.md
 pyproject.toml
 setup.py
+.pytest_cache/README.md
 cmake/check_AVX.cmake
 common/Adam.cpp
 common/common.cpp
 common/common_DFE.cpp
 common/config_element.cpp
 common/dot.cpp
 common/lbfgs.cpp
 common/logging.cpp
 common/matrix.cpp
 common/matrix_real.cpp
 common/mpi_base.cpp
 common/numpy_interface.cpp
 common/tolmin.cpp
 common/include/Adam.h
+common/include/Config.h
 common/include/Config.h.in
 common/include/QGDTypes.h
 common/include/common.h
 common/include/common_DFE.h
 common/include/config_element.h
 common/include/dot.h
 common/include/lbfgs.h
```

### Comparing `squander-1.8.1/test_standalone/CMakeLists.txt` & `squander-1.8.2/test_standalone/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `squander-1.8.1/test_standalone/custom_gate_structure_test.cpp` & `squander-1.8.2/test_standalone/custom_gate_structure_test.cpp`

 * *Files identical despite different names*

### Comparing `squander-1.8.1/test_standalone/decomposition_test.cpp` & `squander-1.8.2/test_standalone/decomposition_test.cpp`

 * *Files identical despite different names*

