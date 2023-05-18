# Comparing `tmp/py21cmemu-1.0.4.tar.gz` & `tmp/py21cmemu-1.0.5.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py21cmemu-1.0.4.tar", max compression
+gzip compressed data, was "py21cmemu-1.0.5.dev0.tar", max compression
```

## Comparing `py21cmemu-1.0.4.tar` & `py21cmemu-1.0.5.dev0.tar`

### file list

```diff
@@ -1,9 +1,12 @@
--rw-r--r--   0        0        0     1073 2023-03-03 11:01:58.918549 py21cmemu-1.0.4/LICENSE
--rw-r--r--   0        0        0     2758 2023-03-09 11:12:05.965273 py21cmemu-1.0.4/README.md
--rw-r--r--   0        0        0     2388 2023-03-16 11:28:18.288929 py21cmemu-1.0.4/pyproject.toml
--rw-r--r--   0        0        0      237 2023-03-09 10:52:15.775695 py21cmemu-1.0.4/src/py21cmemu/__init__.py
--rw-r--r--   0        0        0     2928 2023-03-09 11:12:05.965273 py21cmemu-1.0.4/src/py21cmemu/config.py
--rw-r--r--   0        0        0    18735 2023-03-16 11:30:16.245761 py21cmemu-1.0.4/src/py21cmemu/emulator.py
--rw-r--r--   0        0        0    12208 2023-02-28 09:30:46.338296 py21cmemu-1.0.4/src/py21cmemu/emulator_constants.npz
--rw-r--r--   0        0        0     3132 2023-03-03 11:01:58.918549 py21cmemu-1.0.4/src/py21cmemu/get_emulator.py
--rw-r--r--   0        0        0     4225 1970-01-01 00:00:00.000000 py21cmemu-1.0.4/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-03-03 11:01:58.918549 py21cmemu-1.0.5.dev0/LICENSE
+-rw-r--r--   0        0        0     2441 2023-05-17 16:21:22.516197 py21cmemu-1.0.5.dev0/README.rst
+-rw-r--r--   0        0        0     2370 2023-05-18 10:38:20.000046 py21cmemu-1.0.5.dev0/pyproject.toml
+-rw-r--r--   0        0        0      213 2023-05-16 14:39:00.912610 py21cmemu-1.0.5.dev0/src/py21cmemu/__init__.py
+-rw-r--r--   0        0        0     2776 2023-05-09 14:54:55.861960 py21cmemu-1.0.5.dev0/src/py21cmemu/config.py
+-rw-r--r--   0        0        0     3510 2023-05-04 09:57:53.996907 py21cmemu-1.0.5.dev0/src/py21cmemu/emulator.py
+-rw-r--r--   0        0        0    14978 2023-05-04 09:52:14.387649 py21cmemu-1.0.5.dev0/src/py21cmemu/emulator_constants.npz
+-rw-r--r--   0        0        0     1199 2023-05-03 14:37:25.023190 py21cmemu-1.0.5.dev0/src/py21cmemu/get_emulator.py
+-rw-r--r--   0        0        0     5483 2023-05-05 12:51:51.765886 py21cmemu-1.0.5.dev0/src/py21cmemu/inputs.py
+-rw-r--r--   0        0        0     7254 2023-05-05 09:35:21.501068 py21cmemu-1.0.5.dev0/src/py21cmemu/outputs.py
+-rw-r--r--   0        0        0     2795 2023-05-04 13:04:49.223046 py21cmemu-1.0.5.dev0/src/py21cmemu/properties.py
+-rw-r--r--   0        0        0     3761 1970-01-01 00:00:00.000000 py21cmemu-1.0.5.dev0/PKG-INFO
```

### Comparing `py21cmemu-1.0.4/LICENSE` & `py21cmemu-1.0.5.dev0/LICENSE`

 * *Files identical despite different names*

### Comparing `py21cmemu-1.0.4/README.md` & `py21cmemu-1.0.5.dev0/README.rst`

 * *Files 24% similar despite different names*

```diff
@@ -1,76 +1,67 @@
-# 21cmEMU
+=======
+21cmEMU
+=======
 
-[![PyPI](https://img.shields.io/pypi/v/py21cmemu.svg)][pypi_]
-[![Status](https://img.shields.io/pypi/status/py21cmemu.svg)][status]
-[![Python Version](https://img.shields.io/pypi/pyversions/py21cmemu)][python version]
-[![License](https://img.shields.io/pypi/l/py21cmemu)][license]
 
-[![Read the documentation at https://21cmEMU.readthedocs.io/](https://img.shields.io/readthedocs/py21cmEMU/latest.svg?label=Read%20the%20Docs)][read the docs]
-[![Tests](https://github.com/21cmFAST/21cmEMU/workflows/Tests/badge.svg)][tests]
-[![Codecov](https://codecov.io/gh/21cmFAST/21cmEMU/branch/main/graph/badge.svg)][codecov]
+|PyPI| |Status| |Python| |License| |RTD| |Tests| |Codecov| |pre-commit| |Black|
 
-[![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)][pre-commit]
-[![Black](https://img.shields.io/badge/code%20style-black-000000.svg)][black]
+.. |PyPI| image:: https://img.shields.io/pypi/v/py21cmemu.svg
+   :target: https://pypi.org/project/py21cmemu/
+.. |Status| image:: https://img.shields.io/pypi/status/py21cmemu.svg
+   :target: https://pypi.org/project/py21cmemu/
+.. |Python| image:: https://img.shields.io/pypi/pyversions/py21cmemu.svg
 
-[pypi_]: https://pypi.org/project/py21cmemu/
-[status]: https://pypi.org/project/py21cmemu/
-[python version]: https://pypi.org/project/py21cmemu
-[read the docs]: https://21cmemu.readthedocs.io/
-[tests]: https://github.com/21cmFAST/21cmEMU/actions?workflow=Tests
-[codecov]: https://app.codecov.io/gh/21cmFAST/21cmEMU
-[pre-commit]: https://github.com/pre-commit/pre-commit
-[black]: https://github.com/psf/black
+.. |License| image:: https://img.shields.io/pypi/l/py21cmemu.svg
+    :target: https://github.com/21cmfast/21cmEMU/blob/main/LICENSE
+.. |Tests| image:: https://github.com/21cmfast/21cmEMU/actions/workflows/tests.yml/badge.svg
+    :target: https://github.com/21cmfast/21cmEMU/actions/workflows/tests.yml
+.. |Codecov| image:: https://codecov.io/gh/21cmfast/21cmEMU/branch/main/graph/badge.svg?token=yUOqyTlZ3z
+    :target: https://codecov.io/gh/21cmfast/21cmEMU
+.. |Black| image:: https://img.shields.io/badge/code%20style-black-000000.svg
+    :target: https://github.com/ambv/black
+.. |pre-commit| image:: https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white
+.. |RTD| image:: https://readthedocs.org/projects/21cmemu/badge/?version=latest
+    :target: https://21cmemu.readthedocs.io/en/latest/
+    :alt: Documentation Status
 
-## Features
+An emulator of 21cmFAST summaries.
 
-- Uses Tensorflow to emulate the following summary statistics: 21-cm power spectrum, 21-cm global brightness temperature, IGM spin temperature, and neutral fraction.
-- Uses 21cmFAST to analytically calculate the UV luminosity functions and the Thomson optical depth to the CMB.
+Emulate the following summary statistics:
+    * 21-cm power spectrum
+    * 21-cm global brightness temperature
+    * IGM spin temperature
+    * Neutral fraction
+    * Thomson scattering optical depth
+    * UV luminosity functions
 
-## Requirements
 
-- Tensorflow >= 2.6
-- 21cmFAST
 
-## Installation
+Documentation
+=============
 
-You can install _py21cmEMU_ via [pip] from [PyPI]:
-```console
-$ pip install py21cmemu
-```
+See `the documentation <https://21cmemu.readthedocs.io/en/latest/>`_ for tutorials and API.
 
-Note that you need `gcc` and the `fftw3` and `gsl` packages for the `21cmFAST` installation.
+Issues
+======
 
-## Usage
+If you encounter any problems, please `file an issue <https://github.com/21cmFAST/21cmEMU/issues>`_ along with a detailed description.
 
-Please see the [Command-line Reference] for details.
-
-## Contributing
+Contributing
+============
 
 Contributions are very welcome.
-To learn more, see the [Contributor Guide].
-
-## License
-
-Distributed under the terms of the [MIT license][license],
-_21cmEMU_ is free and open source software.
-
-## Issues
-
-If you encounter any problems,
-please [file an issue] along with a detailed description.
+To learn more, see the `Contributor Guide <https://github.com/21cmFAST/21cmEMU/blob/main/CONTRIBUTING.md>`_.
 
-## Credits
+Citation
+========
 
-This project was generated from [@cjolowicz]'s [Hypermodern Python Cookiecutter] template.
+If you use ``21cmEMU`` in your research please cite: (in prep.)
 
-[@cjolowicz]: https://github.com/cjolowicz
-[pypi]: https://pypi.org/
-[hypermodern python cookiecutter]: https://github.com/cjolowicz/cookiecutter-hypermodern-python
-[file an issue]: https://github.com/21cmFAST/21cmEMU/issues
-[pip]: https://pip.pypa.io/
+License
+=======
+Distributed under the terms of the `MIT license <https://github.com/21cmFAST/21cmEMU/blob/main/LICENSE>`_, ``21cmEMU`` is free and open source software.
 
-<!-- github-only -->
 
-[license]: https://github.com/21cmFAST/21cmEMU/blob/main/LICENSE
-[contributor guide]: https://github.com/21cmFAST/21cmEMU/blob/main/CONTRIBUTING.md
-[command-line reference]: https://21cmEMU.readthedocs.io/en/latest/usage.html
+Credits
+-------
+This project was generated from `@cjolowicz <https://github.com/cjolowicz>`_'s `Hypermodern Python Cookiecutter <https://github.com/cjolowicz/cookiecutter-hypermodern-python>`_ template.
```

### Comparing `py21cmemu-1.0.4/pyproject.toml` & `py21cmemu-1.0.5.dev0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [tool.poetry]
 name = "py21cmEMU"
-version = "1.0.4"
+version = "1.0.5dev"
 description = "Emulator of 21cmFAST summaries."
 authors = ["Daniela Breitman <daniela.breitman@sns.it>"]
 license = "MIT"
-readme = "README.md"
+readme = ["README.rst"]
 homepage = "https://github.com/21cmFAST/21cmEMU"
 repository = "https://github.com/21cmFAST/21cmEMU"
 documentation = "https://21cmEMU.readthedocs.io"
 packages = [
     { include = "py21cmemu", from = "src" },
 ]
 classifiers = [
@@ -29,19 +29,19 @@
 [tool.poetry.urls]
 Changelog = "https://github.com/21cmFAST/21cmEMU/releases"
 
 [tool.poetry.dependencies]
 python = ">=3.8,<3.12"
 click = ">=8.0.1"
 numpy = "^1.22.0"
-21cmfast = "^3.2.0"
 scipy = "^1.10.1"
 tensorflow = "^2.6.0"
 appdirs = "^1.4.4"
 toml = "^0.10.2"
+GitPython = "^3.1.31"
 
 [tool.poetry.dev-dependencies]
 Pygments = ">=2.10.0"
 black = ">=21.10b0"
 coverage = {extras = ["toml"], version = ">=6.2"}
 darglint = ">=1.8.1"
 flake8 = ">=4.0.1"
@@ -70,19 +70,18 @@
 
 [tool.coverage.paths]
 source = ["src", "*/site-packages"]
 tests = ["tests", "*/tests"]
 
 [tool.coverage.run]
 branch = true
-source = ["py21cmemu", "tests"]
+source = ["py21cmemu"]
 
 [tool.coverage.report]
 show_missing = true
-fail_under = 100
 
 [tool.isort]
 profile = "black"
 force_single_line = true
 lines_after_imports = 2
 
 [tool.mypy]
```

### Comparing `py21cmemu-1.0.4/src/py21cmemu/emulator_constants.npz` & `py21cmemu-1.0.5.dev0/src/py21cmemu/emulator_constants.npz`

 * *Files 24% similar despite different names*

#### zipinfo {}

```diff
@@ -1,16 +1,22 @@
-Zip file size: 12208 bytes, number of entries: 14
+Zip file size: 14978 bytes, number of entries: 20
 ?rw-------  2.0 unx      272 b- stor 80-Jan-01 00:00 limits.npy
 ?rw-------  2.0 unx      256 b- stor 80-Jan-01 00:00 ks.npy
 ?rw-------  2.0 unx      800 b- stor 80-Jan-01 00:00 zs.npy
 ?rw-------  2.0 unx      136 b- stor 80-Jan-01 00:00 PS_mean.npy
 ?rw-------  2.0 unx      136 b- stor 80-Jan-01 00:00 PS_std.npy
 ?rw-------  2.0 unx      136 b- stor 80-Jan-01 00:00 Ts_mean.npy
 ?rw-------  2.0 unx      136 b- stor 80-Jan-01 00:00 Ts_std.npy
 ?rw-------  2.0 unx      136 b- stor 80-Jan-01 00:00 Tb_mean.npy
 ?rw-------  2.0 unx      136 b- stor 80-Jan-01 00:00 Tb_std.npy
+?rw-------  2.0 unx      136 b- stor 80-Jan-01 00:00 UVLFs_mean.npy
+?rw-------  2.0 unx      136 b- stor 80-Jan-01 00:00 UVLFs_std.npy
+?rw-------  2.0 unx      136 b- stor 80-Jan-01 00:00 tau_mean.npy
+?rw-------  2.0 unx      136 b- stor 80-Jan-01 00:00 tau_std.npy
 ?rw-------  2.0 unx     5888 b- stor 80-Jan-01 00:00 PS_err.npy
 ?rw-------  2.0 unx      800 b- stor 80-Jan-01 00:00 Tb_err.npy
 ?rw-------  2.0 unx      800 b- stor 80-Jan-01 00:00 Ts_err.npy
 ?rw-------  2.0 unx      800 b- stor 80-Jan-01 00:00 xHI_err.npy
 ?rw-------  2.0 unx      136 b- stor 80-Jan-01 00:00 tau_err.npy
-14 files, 10568 bytes uncompressed, 10568 bytes compressed:  0.0%
+?rw-------  2.0 unx     1120 b- stor 80-Jan-01 00:00 UVLFs_err.npy
+?rw-------  2.0 unx      376 b- stor 80-Jan-01 00:00 UVLFs_MUVs.npy
+20 files, 12608 bytes uncompressed, 12608 bytes compressed:  0.0%
```

#### zipnote «TEMP»/diffoscope_kpg47x5b_/tmpk9h7ukb6_.zip

```diff
@@ -21,14 +21,26 @@
 
 Filename: Tb_mean.npy
 Comment: 
 
 Filename: Tb_std.npy
 Comment: 
 
+Filename: UVLFs_mean.npy
+Comment: 
+
+Filename: UVLFs_std.npy
+Comment: 
+
+Filename: tau_mean.npy
+Comment: 
+
+Filename: tau_std.npy
+Comment: 
+
 Filename: PS_err.npy
 Comment: 
 
 Filename: Tb_err.npy
 Comment: 
 
 Filename: Ts_err.npy
@@ -36,8 +48,14 @@
 
 Filename: xHI_err.npy
 Comment: 
 
 Filename: tau_err.npy
 Comment: 
 
+Filename: UVLFs_err.npy
+Comment: 
+
+Filename: UVLFs_MUVs.npy
+Comment: 
+
 Zip file comment:
```

#### PS_err.npy

```diff
@@ -2,367 +2,367 @@
 00000010: 7227 3a20 273c 6638 272c 2027 666f 7274  r': '<f8', 'fort
 00000020: 7261 6e5f 6f72 6465 7227 3a20 4661 6c73  ran_order': Fals
 00000030: 652c 2027 7368 6170 6527 3a20 2836 302c  e, 'shape': (60,
 00000040: 2031 3229 2c20 7d20 2020 2020 2020 2020   12), }         
 00000050: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00000060: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00000070: 2020 2020 2020 2020 2020 2020 2020 200a                 .
-00000080: 6500 0000 2e39 e13f 6500 0000 4686 e03f  e....9.?e...F..?
-00000090: 6500 0000 e956 e03f 9dff ffff f9cc e03f  e....V.?.......?
-000000a0: 421e cab3 0c74 e03f ca00 0000 e692 dd3f  B....t.?.......?
-000000b0: 56e7 ea63 d7ad dc3f 70d6 97b9 ba5f dc3f  V..c...?p...._.?
-000000c0: 3aff ffff 4f15 dd3f 3aff ffff 53c1 dc3f  :...O..?:...S..?
-000000d0: ca00 0000 d261 dc3f 9dff ffff 589a e13f  .....a.?....X..?
-000000e0: 6500 0000 baa1 e23f c1b7 73d1 d6fc e13f  e......?..s....?
-000000f0: 9dff ffff 6fdd e13f 6500 0000 8036 e23f  ....o..?e....6.?
-00000100: ca00 0000 eeac de3f 3aff ffff ef82 de3f  .......?:......?
-00000110: ca00 0000 5899 dd3f 3aff ffff b52a df3f  ....X..?:....*.?
-00000120: 9dff ffff b728 e03f 3aff ffff ff6a dc3f  .....(.?:....j.?
-00000130: 6500 0000 5f86 e03f 6500 0000 0779 e63f  e..._..?e....y.?
-00000140: 9dff ffff eb57 e63f 9dff ffff efc4 e33f  .....W.?.......?
-00000150: 0d39 857b 0eb1 e33f 6500 0000 1208 e33f  .9.{...?e......?
-00000160: 9dff ffff 9dc7 e23f 6500 0000 4fa4 e13f  .......?e...O..?
-00000170: e318 187e ca7d e03f 9dff ffff e518 e03f  ...~.}.?.......?
-00000180: 6500 0000 2592 e13f 6500 0000 747d e33f  e...%..?e...t}.?
-00000190: ab8a c0ea 28b4 e43f 6500 0000 a42b e73f  ....(..?e....+.?
-000001a0: 6500 0000 fc0e e83f 9dff ffff ce60 e63f  e......?.....`.?
-000001b0: aeb5 261b 90c7 e53f 9dff ffff aa1b e63f  ..&....?.......?
-000001c0: 6500 0000 b4e1 e43f 6500 0000 2964 e33f  e......?e...)d.?
-000001d0: e1ff dcd8 6f77 e33f 9dff ffff c176 e23f  ....ow.?.....v.?
-000001e0: beb5 2755 00ca e33f 4230 400b 2775 e33f  ..'U...?B0@.'u.?
-000001f0: 2f02 aa97 4253 e33f 9eff ffff 9b95 e93f  /...BS.?.......?
-00000200: 6c1a 9b9a ccca e93f 8f7e 51ec cd29 e73f  l......?.~Q..).?
-00000210: 6500 0000 c596 e73f 9dff ffff 63a2 e73f  e......?....c..?
-00000220: d688 0acc ea5d e73f f814 2e7a 0d2c e53f  .....].?...z.,.?
-00000230: 6500 0000 ddbd e43f 9dff ffff fd0f e53f  e......?.......?
-00000240: 9dff ffff 94fb e43f 4be6 0a9a eaed e53f  .......?K......?
-00000250: 9dff ffff d7ee e53f f05a 79e1 1bad ec3f  .......?.Zy....?
-00000260: a58d 4baa c9f0 ef3f c40a eeab 3122 e93f  ..K....?....1".?
-00000270: 6600 0000 1fe0 e93f 6500 0000 86d9 e83f  f......?e......?
-00000280: 4d43 2799 6a9e e83f 6500 0000 e4ff e63f  MC'.j..?e......?
-00000290: 42cb 0c24 c4ee e43f 9dff ffff 2f5b e53f  B..$...?..../[.?
-000002a0: 9dff ffff eccb e43f 6500 0000 4f3b e63f  .......?e...O;.?
-000002b0: 9eff ffff 3028 ea3f 57bf 1cec ebec ec3f  ....0(.?W......?
-000002c0: 3300 0080 4006 f13f 9eff ffff a774 ea3f  3...@..?.....t.?
-000002d0: 9eff ffff f977 ea3f c8c5 a03d e350 e83f  .....w.?...=.P.?
-000002e0: c21b d563 8ae2 e83f 9dff ffff fc9b e63f  ...c...?.......?
-000002f0: ff43 2eea 071c e73f 9dff ffff 4c52 e53f  .C.....?....LR.?
-00000300: 0787 79b6 930e e83f 4100 15b0 40c8 e83f  ..y....?A...@..?
-00000310: 7128 532b cd95 e93f 2d45 fc29 8070 ec3f  q(S+...?-E.).p.?
-00000320: c64c 77fc 3b7b f13f 6600 0000 88bc ea3f  .Lw.;{.?f......?
-00000330: 6600 0000 6e28 e93f abb6 e5db 1746 e73f  f...n(.?.....F.?
-00000340: 9dff ffff 0ebf e83f 3adb 600a 6bda e53f  .......?:.`.k..?
-00000350: 7a92 5aad 4bce e53f 225c 0b99 1aee e43f  z.Z.K..?"\.....?
-00000360: d920 434b e2a0 e53f b688 84b1 8899 e63f  . CK...?.......?
-00000370: 4cd8 fafa 658e e73f 6600 0000 5dd2 eb3f  L...e..?f...]..?
-00000380: c67e 28a1 6fde f03f aa6e 5a60 7219 e93f  .~(.o..?.nZ`r..?
-00000390: 9eff ffff 4726 e93f 6500 0000 af0c e73f  ....G&.?e......?
-000003a0: 2d1c 4dd2 b1bf e73f 7120 b2f9 ab7b e63f  -.M....?q ...{.?
-000003b0: 6f68 68c4 8d09 e43f a5a6 1daf 36cb e33f  ohh....?....6..?
-000003c0: fdf7 0cad 7524 e53f 39b9 0164 01fe e53f  ....u$.?9..d...?
-000003d0: 9dff ffff 721c e63f 5815 6261 80ca e93f  ....r..?X.ba...?
-000003e0: 5210 1856 1ab9 f13f 5e92 c7f9 0390 e93f  R..V...?^......?
-000003f0: 1691 5d82 7c97 e63f bc15 a00d 272d e63f  ..].|..?....'-.?
-00000400: 9dff ffff bce6 e53f fe74 93cf d1ea e33f  .......?.t.....?
-00000410: b01a ada4 b915 e43f 9dff ffff d354 e33f  .......?.....T.?
-00000420: 6500 0000 8e0a e23f 72fa a31c b96f e23f  e......?r....o.?
-00000430: 9dff ffff 65f4 e33f 9dff ffff 72ac e73f  ....e..?....r..?
-00000440: cfff ffff 7591 f13f 6600 0000 7cdd e93f  ....u..?f...|..?
-00000450: e111 5534 9e6a e63f 6a32 0990 2294 e43f  ..U4.j.?j2.."..?
-00000460: fb7d 92ce ffd6 e23f 7a1d e566 7fa0 e23f  .}.....?z..f...?
-00000470: bbcf b0bc 5847 e03f ab5b f555 fb00 e13f  ....XG.?.[.U...?
-00000480: 401c fb5e b967 e13f 66d2 2add 20ce e33f  @..^.g.?f.*. ..?
-00000490: d4c5 0d36 98fc e33f 4eaf bd81 9438 e53f  ...6...?N....8.?
-000004a0: b08c 8a4f 080f f23f 20c9 7e65 9bca e93f  ...O...? .~e...?
-000004b0: 1646 b8e8 1e91 e43f ee2c ffd4 6fbf e43f  .F.....?.,..o..?
-000004c0: 1180 863e 8f4f e23f ef27 85c6 3cc8 df3f  ...>.O.?.'..<..?
-000004d0: 6500 0000 c8fe e03f 5e16 efe0 47ad df3f  e......?^...G..?
-000004e0: 0132 1d60 8444 e03f 9dff ffff a8cd e03f  .2.`.D.?.......?
-000004f0: a01a 4077 5893 e13f 30f4 4a9c 16bf e43f  ..@wX..?0.J....?
-00000500: 523d 04e6 aea3 f23f 7dfb 4b79 368f ea3f  R=.....?}.Ky6..?
-00000510: 8810 494d 3d9d e43f 9dff ffff c44a e33f  ..IM=..?.....J.?
-00000520: e6c8 2d90 74d0 e13f 9dff ffff 9054 e03f  ..-.t..?.....T.?
-00000530: d067 68ce 3bab dd3f d284 7742 bf72 dd3f  .gh.;..?..wB.r.?
-00000540: d7d4 9a25 9143 dd3f 6500 0000 9785 e03f  ...%.C.?e......?
-00000550: f5ab c949 958d e13f dca2 5575 1a25 e23f  ...I...?..Uu.%.?
-00000560: 3300 0080 d24e f33f 2dd3 cc09 94a7 ea3f  3....N.?-......?
-00000570: 0b17 3450 5af0 e33f 9dff ffff 5537 e33f  ..4PZ..?....U7.?
-00000580: 94b7 219d 7542 df3f 82fc 9a84 d864 df3f  ..!.uB.?.....d.?
-00000590: 502a 0904 55dd dc3f a511 5ecd 663d dc3f  P*..U..?..^.f=.?
-000005a0: dc28 15ca bf73 db3f 3aff ffff c903 de3f  .(...s.?:......?
-000005b0: 8469 41b9 8eb8 e03f 1737 1e19 339e e13f  .iA....?.7..3..?
-000005c0: cfff ffff d9e3 f43f 8eda 9c8b 36bf ec3f  .......?....6..?
-000005d0: 9dff ffff 9ede e33f 9f1d 6161 c844 e33f  .......?..aa.D.?
-000005e0: 319e 6e3a 0900 e03f 3aff ffff db83 dd3f  1.n:...?:......?
-000005f0: 9e49 ce2b c7a5 da3f 3aff ffff 0f53 da3f  .I.+...?:....S.?
-00000600: 4f9a 6d08 ebd9 dd3f de25 532a 48a5 de3f  O.m....?.%S*H..?
-00000610: b0f9 278e 0baf df3f dda3 d62f ab65 e13f  ..'....?.../.e.?
-00000620: 92ba 5954 ee51 f53f 8fd6 d023 faa5 ed3f  ..YT.Q.?...#...?
-00000630: bf4a 87ca 948b e43f 187b 0bf5 ec25 e33f  .J.....?.{...%.?
-00000640: 639a 6ac1 04e8 de3f 6906 a229 fce9 dc3f  c.j....?i..)...?
-00000650: 2885 68ea a238 dc3f 68ed f982 3298 d93f  (.h..8.?h...2..?
-00000660: 439d 1a9d b04a da3f 3aff ffff 2990 dd3f  C....J.?:...)..?
-00000670: 172d c1b1 6bfd dd3f e4ca ec36 8a73 e03f  .-..k..?...6.s.?
-00000680: 649a 7539 c7ea f53f 4812 406a 8f1a f03f  d.u9...?H.@j...?
-00000690: 8443 0c1b d111 e53f 108e d64d c2ef e33f  .C.....?...M...?
-000006a0: 1fa8 678f 3f44 e03f eb1a fd3e 256d dc3f  ..g.?D.?...>%m.?
-000006b0: 0e99 a188 5700 d93f 58ed 1e66 ac7a da3f  ....W..?X..f.z.?
-000006c0: fde4 54c0 14ab db3f 4ada 78b7 0b22 dd3f  ..T....?J.x..".?
-000006d0: 3aff ffff 5136 dd3f 1585 436e c98b de3f  :...Q6.?..Cn...?
-000006e0: 25a4 a554 2e34 f53f e039 f886 3e95 ef3f  %..T.4.?.9..>..?
-000006f0: 658a f830 e787 e43f 8adb 4d74 3c33 e33f  e..0...?..Mt<3.?
-00000700: a3c2 3843 fc79 de3f 5a6f 1c3a 50cb db3f  ..8C.y.?Zo.:P..?
-00000710: ae9d f8c2 82cb d83f 8c42 39ef 5278 d83f  .......?.B9.Rx.?
-00000720: 2666 d273 f59e d83f 5866 b1a6 8667 d93f  &f.s...?Xf...g.?
-00000730: 3bf6 585f 195d dc3f b6a5 7618 84c2 dc3f  ;.X_.].?..v....?
-00000740: 4fd2 d415 e14d f33f fd64 562d a6a7 f03f  O....M.?.dV-...?
-00000750: 1f79 e80e 5103 e53f 8542 9fc8 bfe9 e43f  .y..Q..?.B.....?
-00000760: 635d f836 2e0a e03f 7fe7 8847 df9b db3f  c].6...?...G...?
-00000770: 1907 1a4b 086c d83f ed1b 3807 9739 d83f  ...K.l.?..8..9.?
-00000780: a261 2a54 fb5c d93f 2438 532b 304d db3f  .a*T.\.?$8S+0M.?
-00000790: 590b c1bc aeb5 db3f 9b08 806b 7513 dd3f  Y......?...ku..?
-000007a0: d00d 1825 b97a f13f 6600 0000 8c95 ef3f  ...%.z.?f......?
-000007b0: a3f7 f026 c7ab e53f 9dff ffff 63ec e33f  ...&...?....c..?
-000007c0: fc3a a9d9 5a41 df3f b509 897a 9b3e da3f  .:..ZA.?...z.>.?
-000007d0: dc1a d9be 3626 d83f 4e28 ac95 6824 d73f  ....6&.?N(..h$.?
-000007e0: 80d3 9948 bac0 d83f 1bc9 ded6 7398 d93f  ...H...?....s..?
-000007f0: 6516 3c2a 9382 db3f c6fb e101 52a7 dc3f  e.<*...?....R..?
-00000800: ae2e fa94 7d20 f03f ae48 4a24 5494 ef3f  ....} .?.HJ$T..?
-00000810: 0f20 e7cf 6273 e53f df60 15ea be5d e43f  . ..bs.?.`...].?
-00000820: e906 6252 c22a e03f 1e7e ac5e a52e dc3f  ..bR.*.?.~.^...?
-00000830: d0e6 5136 d768 d93f cfb4 6a02 205d d83f  ..Q6.h.?..j. ].?
-00000840: 4829 5ad2 a4ee d73f f4f5 9da9 15f4 d83f  H)Z....?.......?
-00000850: 7954 b36e 6fd2 d93f 77d6 4b2f 5413 db3f  yT.no..?w.K/T..?
-00000860: 80c4 c681 1f2b ee3f 798e e4b7 c514 ec3f  .....+.?y......?
-00000870: 1d32 1a08 b2d1 e33f bcf0 4b74 d872 e33f  .2.....?..Kt.r.?
-00000880: fcb8 621d a850 de3f c56b 023e 0008 da3f  ..b..P.?.k.>...?
-00000890: a0ac 3633 f5fa d83f 42c1 9e4f 0703 d73f  ..63...?B..O...?
-000008a0: 6254 71da ac11 d73f 5da1 7107 61a2 d73f  bTq....?].q.a..?
-000008b0: 4111 cdb6 af71 d93f 64d3 58eb ef7f db3f  A....q.?d.X....?
-000008c0: 6507 af73 cba3 ed3f 98a7 7f8c 3638 ea3f  e..s...?....68.?
-000008d0: 9ac2 51eb 9a4a e33f 9218 f75d fc62 e23f  ..Q..J.?...].b.?
-000008e0: 3864 65db 7042 de3f 3516 95de 52e5 da3f  8de.pB.?5...R..?
-000008f0: e931 bb72 3de6 d73f 97e9 b396 1be9 d73f  .1.r=..?.......?
-00000900: 8aea decb 0b3c d63f 6f84 66c1 d389 d83f  .....<.?o.f....?
-00000910: da90 8b47 d143 d93f d22b 9530 d859 da3f  ...G.C.?.+.0.Y.?
-00000920: 272b 7886 35bc ed3f 6a55 199e 9d38 e83f  '+x.5..?jU...8.?
-00000930: f771 cfcf e815 e23f a5fd 9bde 627b e13f  .q.....?....b{.?
-00000940: 2a96 8add f0d2 dd3f 0ded 95e7 b759 d93f  *......?.....Y.?
-00000950: fa10 1110 d587 d83f 5f15 d130 3f82 d53f  .......?_..0?..?
-00000960: 0ab9 37ac 898b d73f 489e 7c3a 3a9b d63f  ..7....?H.|::..?
-00000970: b476 7d04 4858 d93f 17e0 ef61 de06 d93f  .v}.HX.?...a...?
-00000980: b5a3 caab 0646 ec3f 8438 b026 b020 e63f  .....F.?.8.&. .?
-00000990: 2e1e 18f9 9f76 e03f 65b3 286e 1332 e03f  .....v.?e.(n.2.?
-000009a0: 7d95 cfa4 215a dd3f 050c e0dc c9d0 d83f  }...!Z.?.......?
-000009b0: 6d5a afc5 1a96 d73f 783a 94bb d73b d63f  mZ.....?x:...;.?
-000009c0: 96aa fe98 2f10 d63f ef36 3d2d 29d0 d63f  ..../..?.6=-)..?
-000009d0: e1a6 be5e 2dfb d63f e56e 3aa3 2f29 d83f  ...^-..?.n:./).?
-000009e0: ea28 3120 dfca eb3f b4c2 238d 1ce3 e43f  .(1 ...?..#....?
-000009f0: bf75 5043 b084 de3f d925 ee49 9896 de3f  .uPC...?.%.I...?
-00000a00: ca00 0000 da23 db3f 6dc9 a1f0 152a d83f  .....#.?m....*.?
-00000a10: 71a5 0376 ce3b d63f d64c dc56 7aa9 d43f  q..v.;.?.L.Vz..?
-00000a20: 510f 44e2 35e7 d53f 6066 1418 9307 d63f  Q.D.5..?`f.....?
-00000a30: ecc2 35f6 86ad d63f 47bf 4ddd dfff d83f  ..5....?G.M....?
-00000a40: 4e28 e3f2 8a5f ec3f c668 e789 e859 e33f  N(..._.?.h...Y.?
-00000a50: af48 d147 ded3 dd3f 3880 bf7d b6db dc3f  .H.G...?8..}...?
-00000a60: 3053 2aa7 2d0e da3f 5c47 ff8a abdf d73f  0S*.-..?\G.....?
-00000a70: 7144 cdc6 e79a d53f c6b1 9557 d191 d43f  qD.....?...W...?
-00000a80: bef9 4c53 51c1 d43f 6215 383c 33dd d63f  ..LSQ..?b.8<3..?
-00000a90: ff32 3263 6759 d63f 4bdb 27a6 eb34 d73f  .22cgY.?K.'..4.?
-00000aa0: 6571 c312 723c eb3f 1e65 ed8d 5122 e33f  eq..r<.?.e..Q".?
-00000ab0: 4181 7ff7 1387 da3f ca7b 188e eaf5 db3f  A......?.{.....?
-00000ac0: 71f1 594d 1f3c d93f b90b ba9c 1afa d63f  q.YM.<.?.......?
-00000ad0: 9cd7 27fd b492 d53f f5b6 db4e dff6 d33f  ..'....?...N...?
-00000ae0: 3aea aa17 980b d53f dfe9 410a 6bce d53f  :......?..A.k..?
-00000af0: 9258 9a3c 7280 d63f b091 b60f 3bdb d63f  .X.<r..?....;..?
-00000b00: ecea c923 32d0 eb3f d2c6 f34f 46ce e13f  ...#2..?...OF..?
-00000b10: 03cf 3a6e cb85 da3f 25e8 8cad 06e7 d93f  ..:n...?%......?
-00000b20: 4d6d 19ba ef63 d83f 18b0 3de8 2e49 d53f  Mm...c.?..=..I.?
-00000b30: ecab e4e7 8961 d53f 6ad9 bf15 66ac d33f  .....a.?j...f..?
-00000b40: 39a1 9c65 f931 d43f 8f95 b66a 76a3 d43f  9..e.1.?...jv..?
-00000b50: 57f1 fe07 0b34 d53f 2f28 013e 6d7c d63f  W....4.?/(.>m|.?
-00000b60: 8140 e02d ca8b ea3f 18b8 ae98 3af5 e03f  .@.-...?....:..?
-00000b70: 2373 1c0d 0812 d93f f019 8e24 d693 db3f  #s.....?...$...?
-00000b80: 2b77 24c3 0fe2 d73f 776f ce8c 1c0d d53f  +w$....?wo.....?
-00000b90: b09a 5c1a f66c d33f ead9 ccda 3d82 d33f  ..\..l.?....=..?
-00000ba0: a7bc faa0 248f d33f 0cc9 03d1 9bcc d43f  ....$..?.......?
-00000bb0: 4b6c c640 8853 d43f a2ae d123 0148 d63f  Kl.@.S.?...#.H.?
-00000bc0: dc08 f750 b240 ea3f b5e1 db0a de0c e13f  ...P.@.?.......?
-00000bd0: 9317 6b7c 869c d93f 3b48 0483 b40e d93f  ..k|...?;H.....?
-00000be0: b950 9467 ddeb d73f 0a8e 4ca2 f49f d43f  .P.g...?..L....?
-00000bf0: a07f 7cda d28b d33f 1be2 02b3 bdca d23f  ..|....?.......?
-00000c00: 5053 94d6 4ba9 d33f eeb7 5107 62be d43f  PS..K..?..Q.b..?
-00000c10: 9cd7 e81a b315 d53f f937 1833 5f7b d53f  .......?.7.3_{.?
-00000c20: 6af6 4dae 202a e93f 53c4 977e 96e4 e03f  j.M. *.?S..~...?
-00000c30: 2901 2385 0d6a d83f 2e28 55cf 39f8 d83f  ).#..j.?.(U.9..?
-00000c40: e5a4 bd29 dfc5 d63f 245b b152 bf5a d43f  ...)...?$[.R.Z.?
-00000c50: eb8f 7c2f 7be6 d33f 159b d37a 58e5 d23f  ..|/{..?...zX..?
-00000c60: bfcf 72b1 8b91 d33f 5bc7 a47c 8e0c d43f  ..r....?[..|...?
-00000c70: d1bb 7480 ecdd d43f df06 07cd 3485 d43f  ..t....?....4..?
-00000c80: 3578 0487 ad74 e83f 9d0a 2816 8146 e03f  5x...t.?..(..F.?
-00000c90: 0c48 8979 3255 d93f 04b5 244e 9be5 d83f  .H.y2U.?..$N...?
-00000ca0: ae6c 6bef e89f d53f ce84 b372 fa82 d33f  .lk....?...r...?
-00000cb0: 6c4e d753 ec21 d33f 011a 5e14 fa64 d23f  lN.S.!.?..^..d.?
-00000cc0: a60d 16f2 a548 d33f 271c 6c9a 93b7 d43f  .....H.?'.l....?
-00000cd0: a37a 1c0c 0b5b d33f 8625 64ac 09f4 d43f  .z...[.?.%d....?
-00000ce0: b660 7617 3110 e83f 1868 de96 c7b7 df3f  .`v.1..?.h.....?
-00000cf0: 3b9b c2bc b358 d93f 0d9e 4984 3e6c d83f  ;....X.?..I.>l.?
-00000d00: 38fe b95c 9509 d63f e45a 076c 6195 d33f  8..\...?.Z.la..?
-00000d10: 63ff fabc c1c9 d23f 5759 31b1 fb7c d23f  c......?WY1..|.?
-00000d20: 07b0 eb75 90a3 d33f 01ab aa13 9243 d33f  ...u...?.....C.?
-00000d30: 98b0 59ed 598d d43f 07ce f600 fcdb d43f  ..Y.Y..?.......?
-00000d40: c0a9 09a4 642f e73f f259 102c 2ff1 df3f  ....d/.?.Y.,/..?
-00000d50: 0648 5d42 fdc4 d83f 11e2 d579 325a d73f  .H]B...?...y2Z.?
-00000d60: 4279 84e6 bac0 d53f 0061 a827 3b49 d33f  By.....?.a.';I.?
-00000d70: 0cda e97f 3573 d23f 40cc abeb 4328 d23f  ....5s.?@...C(.?
-00000d80: d073 34d6 d52a d33f 93d5 ec06 0a25 d43f  .s4..*.?.....%.?
-00000d90: 88ac 2e3a bdf0 d33f 45e4 3317 e8ed d43f  ...:...?E.3....?
-00000da0: 3d8e 859c 3dbb e53f ca51 baae 976a df3f  =...=..?.Q...j.?
-00000db0: 5a07 037e 2b22 d83f 5271 1452 23c3 d83f  Z..~+".?Rq.R#..?
-00000dc0: b65c 43b7 462e d53f af25 1cd4 4655 d43f  .\C.F..?.%..FU.?
-00000dd0: 55af 1b15 5376 d33f 629e c1e4 4acf d33f  U...Sv.?b...J..?
-00000de0: 77aa a04b 0deb d43f 2a8a 2d0d 3400 d43f  w..K...?*.-.4..?
-00000df0: 99eb 3cb6 493a d43f f6bf 9ecd c286 d43f  ..<.I:.?.......?
-00000e00: 94ab 9801 6c73 e53f 134f 7b38 e328 e03f  ....ls.?.O{8.(.?
-00000e10: aa8c d91a 90ee d73f 689b 24e5 3b1e d93f  .......?h.$.;..?
-00000e20: f5ab a293 33ae d63f 2114 db2f 4f03 d43f  ....3..?!../O..?
-00000e30: f641 a330 0b4b d43f a770 0e83 0b2b d33f  .A.0.K.?.p...+.?
-00000e40: 7ac4 dcdc ccbf d33f 089a 1cee 02fb d43f  z......?.......?
-00000e50: 63a0 310d 4a2f d53f 3323 45e1 a0ba d43f  c.1.J/.?3#E....?
-00000e60: 2035 4eda ddc1 e63f 5ce0 115c 3920 e03f   5N....?\..\9 .?
-00000e70: 4808 922e f3d7 d83f db42 bde2 8625 d93f  H......?.B...%.?
-00000e80: 2b3d 1f44 13f6 d53f 5f8d c5bd e017 d63f  +=.D...?_......?
-00000e90: 352c 2dc1 de1d d63f 1d39 ef81 d1db d43f  5,-....?.9.....?
-00000ea0: a047 f28d 9528 d63f 3069 d1ca db88 d53f  .G...(.?0i.....?
-00000eb0: 8b26 6677 4271 d73f 9a95 6e79 73a1 d63f  .&fwBq.?..nys..?
-00000ec0: d305 2e61 611a e63f 588b 1f19 b00f e03f  ...aa..?X......?
-00000ed0: 3cfb e124 e69c d93f 00f0 437c 398f d83f  <..$...?..C|9..?
-00000ee0: 1f59 0634 6bef d73f 70f8 3863 bd60 d53f  .Y.4k..?p.8c.`.?
-00000ef0: 2d76 d9ff c5a7 d63f 3b6b e983 1034 d63f  -v.....?;k...4.?
-00000f00: fe04 0eb9 4bb3 d73f 581d 1c8c e04e d93f  ....K..?X....N.?
-00000f10: 4d50 b6ab c277 d73f 1b21 0bbb 4cf4 d63f  MP...w.?.!..L..?
-00000f20: e9f4 2805 b808 e43f 559f c9a9 671e df3f  ..(....?U...g..?
-00000f30: 8682 f583 63d7 d73f a1f2 f44d e62c da3f  ....c..?...M.,.?
-00000f40: fe80 e561 8d43 d83f 02ea 7a36 7d54 d73f  ...a.C.?..z6}T.?
-00000f50: be1a e9af 2b3b d63f 451a 62d5 1e8c d53f  ....+;.?E.b....?
-00000f60: 9298 72de 8b2c da3f db15 67a1 1c10 d83f  ..r..,.?..g....?
-00000f70: 663f 8595 235c d73f a52a 6bd1 09de d63f  f?..#\.?.*k....?
-00000f80: 4967 02e5 c884 e33f edad 686b 6297 e03f  Ig.....?..hkb..?
-00000f90: 1592 8bbf 6a11 d93f 48ae 2882 4ed1 d93f  ....j..?H.(.N..?
-00000fa0: 3ecc 9f4b 56e9 d83f 4302 561d c6bf d73f  >..KV..?C.V....?
-00000fb0: 330f 6206 87d0 d63f 80f7 9475 73a8 d53f  3.b....?...us..?
-00000fc0: 4507 80f0 7753 d93f 1c11 190a 1e54 d83f  E...wS.?.....T.?
-00000fd0: 8802 b0ea fe26 d73f 2fc3 be3e ce28 d73f  .....&.?/..>.(.?
-00000fe0: 6aa1 d7fa 307e e33f 88f8 06eb 4dee df3f  j...0~.?....M..?
-00000ff0: 2fff 251a c31b d93f 6713 e28c aba3 da3f  /.%....?g......?
-00001000: 2ec3 1f53 cd79 d93f de19 3195 dcaf d83f  ...S.y.?..1....?
-00001010: c2f4 0f21 2aff d73f a7a8 d4b1 72a3 d73f  ...!*..?....r..?
-00001020: ea2c 3aa4 2c4a da3f 2200 ed1c 2c38 da3f  .,:.,J.?"...,8.?
-00001030: 21fa 1bf0 d740 d83f d39e 06bf 2c3d d83f  !....@.?....,=.?
-00001040: c7b8 1daa f731 e43f d480 3c59 f1d6 e03f  .....1.?..<Y...?
-00001050: dbe3 2dc8 cfd8 da3f 8f6f 9737 c2d8 db3f  ..-....?.o.7...?
-00001060: e11a 4b02 6bac db3f 7a63 848f 5bbe d83f  ..K.k..?zc..[..?
-00001070: 7627 1ba8 2f0d d93f cf43 bc56 86b9 d83f  v'../..?.C.V...?
-00001080: 3d25 dd57 1825 d93f d80e d9d3 9b71 da3f  =%.W.%.?.....q.?
-00001090: 903d c329 f4e4 d93f ee51 6434 f625 d93f  .=.)...?.Qd4.%.?
-000010a0: f9d2 4c82 c76d e53f 85b6 a831 e682 e13f  ..L..m.?...1...?
-000010b0: 096f c7b5 20b0 da3f 6a56 9c59 c03c de3f  .o.. ..?jV.Y.<.?
-000010c0: 9cab d058 bb42 dc3f e693 3a0c 1bc4 da3f  ...X.B.?..:....?
-000010d0: 0f28 66b9 f395 da3f 0783 218a 46d2 d93f  .(f....?..!.F..?
-000010e0: e2cb b3fd b13e dd3f e6c4 4e3c 2298 dc3f  .....>.?..N<"..?
-000010f0: a50b 85b6 3e82 dc3f 588d b8f7 4bce db3f  ....>..?X...K..?
-00001100: fc99 d563 e51b e63f b031 4db0 8169 e23f  ...c...?.1M..i.?
-00001110: f64e 0b0d 231e df3f 483a 62cc 35c0 dd3f  .N..#..?H:b.5..?
-00001120: 5977 b437 6788 dc3f 2a09 0282 d47e dc3f  Yw.7g..?*....~.?
-00001130: 8cd2 b8bb addc da3f db24 3094 579b db3f  .......?.$0.W..?
-00001140: 6b91 df79 88a2 dc3f a2d1 a06b 10b9 dc3f  k..y...?...k...?
-00001150: 12ef 7ab7 3be2 df3f bafd c10c b014 e03f  ..z.;..?.......?
-00001160: 6118 9560 02fe e63f a13a 3cfe 002c e43f  a..`...?.:<..,.?
-00001170: 1662 ad37 1e86 e13f 69fb 96ca 082d e13f  .b.7...?i....-.?
-00001180: dd78 4ff1 174e e03f c9f5 6616 45d4 dd3f  .xO..N.?..f.E..?
-00001190: 54e4 e435 3bb9 dc3f 6738 8aeb fd95 dd3f  T..5;..?g8.....?
-000011a0: 6ab7 274b 0f64 e13f 53b1 cef7 9b81 df3f  j.'K.d.?S......?
-000011b0: ff74 245b 4181 df3f 3cfc 6bea 3f35 e13f  .t$[A..?<.k.?5.?
-000011c0: 6600 0000 4a09 eb3f a839 e503 045f e63f  f...J..?.9..._.?
-000011d0: 5531 f9f4 7af3 e23f e506 a52d 89f9 e33f  U1..z..?...-...?
-000011e0: 2c20 9720 a047 e13f 47bd 26a3 665e e03f  , . .G.?G.&.f^.?
-000011f0: 918f 1d46 a4b6 e03f 4612 2f73 c19a e03f  ...F...?F./s...?
-00001200: 6a42 62df 32c7 e23f afe7 d0ef 1454 e03f  jBb.2..?.....T.?
-00001210: 770e d82d 740d e03f 410e 5c35 c87b e13f  w..-t..?A.\5.{.?
-00001220: 041e d586 241b ed3f 035c 44ac dc7e ed3f  ....$..?.\D..~.?
-00001230: 43b6 7e8b 332f e53f df6c 0b40 8405 e73f  C.~.3/.?.l.@...?
-00001240: 06a4 af68 742b e63f bf73 26ab 30ea e33f  ...ht+.?.s&.0..?
-00001250: 5175 3bbb 902e e33f af6a 549e 0cb2 e13f  Qu;....?.jT....?
-00001260: b507 15d0 4853 e63f e839 5074 03d0 e33f  ....HS.?.9Pt...?
-00001270: d360 b523 e26a e23f 9bad 3e79 0d3f e23f  .`.#.j.?..>y.?.?
-00001280: 67f6 406d 90c8 f23f b888 0839 7c1c ee3f  g.@m...?...9|..?
-00001290: 01a8 189e 4a8d ea3f 8261 291a 5b50 e93f  ....J..?.a).[P.?
-000012a0: 25a3 900e 0eff eb3f a179 d578 862c eb3f  %......?.y.x.,.?
-000012b0: f8d3 8de9 caf5 e73f c322 e217 a818 e43f  .......?.".....?
-000012c0: 7235 fa1d 0faf e53f 0f51 fbd6 80b9 e63f  r5.....?.Q.....?
-000012d0: 4c3a d7a2 d64d e63f a173 84e2 6dce e43f  L:...M.?.s..m..?
-000012e0: ce8e 8299 1334 f43f 5713 eabd bfbd f23f  .....4.?W......?
-000012f0: 3606 b3da 7cfe ea3f 08dc 2979 8166 eb3f  6...|..?..)y.f.?
-00001300: 8e27 188c 0c34 ec3f d239 37fa 07b6 e93f  .'...4.?.97....?
-00001310: 3caa 6c44 a927 e83f d43d ee6c c7c2 e73f  <.lD.'.?.=.l...?
-00001320: 0513 7641 14fe e63f 8bca 1031 9b82 e73f  ..vA...?...1...?
-00001330: 8cd3 f154 8dbe ea3f 163f 60ff bf1f f13f  ...T...?.?`....?
-00001340: cfff ff7f fd7e f73f 57bc 42cd 6dd7 f83f  .....~.?W.B.m..?
-00001350: 74bb 1065 051a f63f 24f7 677a 8a91 f23f  t..e...?$.gz...?
-00001360: 9591 0e7d 1e55 f33f c1f6 c294 eb97 f33f  ...}.U.?.......?
-00001370: 3899 dd2f 410d f03f 6251 55a3 c583 ed3f  8../A..?bQU....?
-00001380: b6f8 9772 caed ee3f ba28 70b0 ab47 ee3f  ...r...?.(p..G.?
-00001390: 3466 c0f2 bb67 f43f c592 5f82 f5ee ed3f  4f...g.?.._....?
-000013a0: c2ea 43c2 e6bf fc3f dca8 aee4 1766 f93f  ..C....?.....f.?
-000013b0: af9a 5eff a1a6 f53f 2595 6949 0cf4 f53f  ..^....?%.iI...?
-000013c0: a14c c54d 30c5 f33f 8fe3 53d7 a23e f33f  .L.M0..?..S..>.?
-000013d0: 9f8d 5bd3 601d f23f 5ae4 bf1e c457 f03f  ..[.`..?Z....W.?
-000013e0: 48d0 bbc3 0a79 f03f 935e c252 8392 f23f  H....y.?.^.R...?
-000013f0: cfff ff7f 65a1 f43f 76ec f1fa e722 f33f  ....e..?v....".?
-00001400: ae07 f8a3 c9c6 fa3f 3400 0000 c01f fb3f  .......?4......?
-00001410: 74fe d1aa 3920 f63f 5d73 6baa 7f9b f83f  t...9 .?]sk....?
-00001420: 3300 0000 a9db f63f bd77 c782 5cf7 f53f  3......?.w..\..?
-00001430: e7e0 ed7d d24f f73f cef6 c6a5 64d1 f83f  ...}.O.?....d..?
-00001440: b25a 8e6e 7117 f73f 46fe 93ca 6480 fb3f  .Z.nq..?F...d..?
-00001450: d3a8 025f 81f2 fc3f adae 09eb 67ff fa3f  ..._...?....g..?
-00001460: cfff ff7f ecd6 f63f 3300 0080 3461 f73f  .......?3...4a.?
-00001470: b863 687b 7876 f93f 6c22 cfae cecb fb3f  .ch{xv.?l".....?
-00001480: 3400 0000 172b fd3f 124f 4c26 085b fe3f  4....+.?.OL&.[.?
-00001490: f666 39f7 e7e8 f83f 5a95 fee4 3da6 f73f  .f9....?Z...=..?
-000014a0: 4218 b29e 0808 f93f 3cad ab92 423a fc3f  B......?<...B:.?
-000014b0: 48e6 32a4 4dd6 0040 27fa 9a11 dc1c 0040  H.2.M..@'......@
-000014c0: fa4e 6563 3eba f43f 3300 0080 dfae f43f  .Nec>..?3......?
-000014d0: d0ff ffff 3e3b fc3f 57c2 97d2 4fff f83f  ....>;.?W...O..?
-000014e0: 3400 0000 e08d fe3f a367 1239 5345 fd3f  4......?.g.9SE.?
-000014f0: 265d 14e3 7efa fc3f 17b4 fed9 44dc ff3f  &]..~..?....D..?
-00001500: 1ec8 54cb 1394 0240 4a3e 5989 0147 0140  ..T....@J>Y..G.@
-00001510: 65ea 272f ec6c 0340 4374 7255 0d36 fe3f  e.'/.l.@CtrU.6.?
-00001520: 18df 5c24 9d84 eb3f cfff ffff 6551 f13f  ..\$...?....eQ.?
-00001530: 9680 d72e 7693 f83f 7877 2458 b40d f83f  ....v..?xw$X...?
-00001540: d0ff ff7f 04bb fa3f 8cd5 d3b2 dc2d 0140  .......?.....-.@
-00001550: ae40 3ec7 e344 ff3f 8913 2b7c cbff 0240  .@>..D.?..+|...@
-00001560: 3702 d88f bc9d ff3f d8f9 650a 1e5e 0240  7......?..e..^.@
-00001570: 0df2 4ba7 116c 0440 2e0b 648a e0bb 0a40  ..K..l.@..d....@
-00001580: 631f 9c34 ddac ec3f 3300 0080 55d7 f13f  c..4...?3...U..?
-00001590: c7a3 46e2 5e3f f43f c19e c29c f8d4 f23f  ..F.^?.?.......?
-000015a0: cfff ffff 85d2 f53f 9844 6d0a e150 f63f  .......?.Dm..P.?
-000015b0: d0ff ffff 5260 ff3f 92d5 de34 8abb 0240  ....R`.?...4...@
-000015c0: 1a00 0000 5259 0340 fe41 5033 1963 0640  ....RY.@.AP3.c.@
-000015d0: f4a9 0e58 6a50 0540 ac6d df8c 25ec 1140  ...XjP.@.m..%..@
-000015e0: 9eff ffff d088 e93f 6600 0000 6445 ea3f  .......?f...dE.?
-000015f0: 4cd9 0dc1 a187 ee3f 6f5b 831e 75fb ef3f  L......?o[..u..?
-00001600: f7ae 0efb e5e9 f43f c41b e3a5 ecf1 f43f  .......?.......?
-00001610: 46ba 670b 5179 fd3f e8ff ffff b0db 0340  F.g.Qy.?.......@
-00001620: be10 7bb9 f3f1 0140 e8ff ff3f 2133 0640  ..{....@...?!3.@
-00001630: 0b78 2474 2d74 0540 2639 4af7 46e0 0b40  .x$t-t.@&9J.F..@
-00001640: 9eff ffff 8538 ee3f 9dff ffff bf0b e63f  .....8.?.......?
-00001650: 6600 0000 6347 e93f 4aa3 5d87 c17c e93f  f...cG.?J.]..|.?
-00001660: 9eff ffff 99a0 ea3f 9cf2 c4b2 4ed4 f33f  .......?....N..?
-00001670: 3dcd 27a1 9936 f63f 3400 0080 9d19 fe3f  =.'..6.?4......?
-00001680: 1a00 0040 5fa1 0440 4aba 0f89 59f8 0640  ...@_..@J...Y..@
-00001690: 229c 2900 894e 0840 af19 a559 d216 0d40  ".)..N.@...Y...@
-000016a0: 9dff ffff e9f7 e33f 9dff ffff 626b e33f  .......?....bk.?
-000016b0: 9dff ffff b3bb e23f 540d 5a66 24c3 ed3f  .......?T.Zf$..?
-000016c0: 3300 0080 a145 f13f c7c6 dc34 cece f13f  3....E.?...4...?
-000016d0: 3300 0000 9722 f43f cfff ff7f 7832 f63f  3....".?....x2.?
-000016e0: bcf9 2c72 2a17 0340 611a fd5c 050b 0740  ..,r*..@a..\...@
-000016f0: 7c54 4fb7 913f 1040 f2d0 d418 d2ac 1640  |TO..?.@.......@
+00000080: 6033 3333 0b1b 603f 6033 3333 67be 603f  `333..`?`333g.`?
+00000090: a0cc cccc 90d7 603f c066 6666 3646 5c3f  ......`?.fff6F\?
+000000a0: c066 6666 ceb0 593f 4099 9999 799c 5a3f  .fff..Y?@...y.Z?
+000000b0: c066 6666 ce1f 5b3f 4099 9999 c156 573f  .fff..[?@....VW?
+000000c0: 4099 9999 21ae 573f c066 6666 7e18 563f  @...!.W?.fff~.V?
+000000d0: 4099 9999 092e 5a3f 4099 9999 19f5 5f3f  @.....Z?@....._?
+000000e0: 6033 3333 0f32 633f a0cc cccc d883 623f  `333.2c?......b?
+000000f0: a0cc cccc 902a 623f 4099 9999 89ef 5e3f  .....*b?@.....^?
+00000100: c066 6666 e6db 5e3f 4099 9999 5969 5a3f  .fff..^?@...YiZ?
+00000110: 4099 9999 09df 5b3f c066 6666 6675 5b3f  @.....[?.ffffu[?
+00000120: c066 6666 0689 593f c066 6666 5665 593f  .fff..Y?.fffVeY?
+00000130: 4099 9999 992b 5d3f 6033 3333 cb3c 603f  @....+]?`333.<`?
+00000140: a0cc cccc acf9 633f a0cc cccc 8c62 643f  ......c?.....bd?
+00000150: 6033 3333 a742 653f a0cc cccc 3408 663f  `333.Be?....4.f?
+00000160: a0cc cccc 5c58 623f a0cc cccc a818 613f  ....\Xb?......a?
+00000170: 6033 3333 bf35 613f 6033 3333 1f0a 613f  `333.5a?`333..a?
+00000180: c066 6666 4e01 5d3f 6033 3333 bf56 603f  .fffN.]?`333.V`?
+00000190: a0cc cccc f49f 633f a0cc cccc f446 683f  ......c?.....Fh?
+000001a0: 00e0 ef50 146a 6d3f a0cc cccc 208d 6c3f  ...P.jm?.... .l?
+000001b0: a0cc cccc 2ce1 683f 6033 3333 0f8b 6a3f  ....,.h?`333..j?
+000001c0: 6033 3333 f376 673f a0cc cccc ec6a 643f  `333.vg?.....jd?
+000001d0: a0cc cccc 7c36 663f 6033 3333 bf33 633f  ....|6f?`333.3c?
+000001e0: 6033 3333 334c 633f 6033 3333 5767 673f  `3333Lc?`333Wgg?
+000001f0: a0cc cccc f464 673f 6033 3333 53ed 6c3f  .....dg?`333S.l?
+00000200: b099 9999 11e5 793f 5066 6666 6aad 7f3f  ......y?Pfffj..?
+00000210: e00c 9a4c d784 7d3f 5066 6666 265c 7d3f  ...L..}?Pfff&\}?
+00000220: 80d7 ce41 91ae 7c3f b099 9999 83ff 773f  ...A..|?......w?
+00000230: 8034 5c89 65e2 743f b099 9999 e511 733f  .4\.e.t?......s?
+00000240: b099 9999 53ab 713f 5066 6666 d65d 723f  ....S.q?Pfff.]r?
+00000250: 008c 648f d027 733f b099 9999 1fff 7a3f  ..d..'s?......z?
+00000260: 0028 f224 6902 8a3f 80a3 acdf 44ec 9a3f  .(.$i..?....D..?
+00000270: 804f 22c2 bfa2 9d3f 000c babd e4fb 9a3f  .O"....?.......?
+00000280: 00b8 42ca cf08 9a3f 00d0 2c09 d03f 983f  ..B....?..,..?.?
+00000290: 40f4 cb16 db16 943f 0063 247b a4a6 913f  @......?.c${...?
+000002a0: e0f0 9afc 8981 8f3f c087 b196 c4f3 8c3f  .......?.......?
+000002b0: 00a7 9718 93ac 8c3f 8082 df86 98a0 8f3f  .......?.......?
+000002c0: 00db fb54 b5b2 9c3f a08b db68 60c0 a93f  ...T...?...h`..?
+000002d0: f89c 2743 7b12 ac3f 40f8 6c1d dc7b aa3f  ..'C{..?@.l..{.?
+000002e0: b0de e176 8eba aa3f c000 de02 d13e a73f  ...v...?.....>.?
+000002f0: d061 026d 931e a43f a040 4b57 844c a23f  .a.m...?.@KW.L.?
+00000300: 80c5 c4e6 93c4 a03f c076 4eb3 60c4 9e3f  .......?.vN.`..?
+00000310: 20ce 6e2d 57ac 9e3f 00e8 305f 9eb1 9f3f   .n-W..?..0_...?
+00000320: c0a2 9410 7c15 a63f f8f1 4d89 2712 b23f  ....|..?..M.'..?
+00000330: 0073 d6a7 0c82 b53f 40af 230e b9ca b33f  .s.....?@.#....?
+00000340: e0d1 8db0 6473 b33f 682e bf78 f624 b33f  ....ds.?h..x.$.?
+00000350: 0067 d13b 2544 af3f 00c0 7971 4253 ac3f  .g.;%D.?..yqBS.?
+00000360: 80f5 0d4c 7ed6 a93f 0060 419a 11a0 a83f  ...L~..?.`A....?
+00000370: 8038 2ee3 368b aa3f 8029 3c68 f6f3 aa3f  .8..6..?.)<h...?
+00000380: 2076 a6d0 cd20 aa3f a4a0 dbcb d1ef b63f   v... .?.......?
+00000390: 402e e3a6 7e4d ba3f 0081 7b9e bf5b be3f  @...~M.?..{..[.?
+000003a0: 1842 6216 bc32 b73f 80e3 dd91 2998 b83f  .Bb..2.?....)..?
+000003b0: 00e2 b853 1af0 b43f b823 9639 c88d b33f  ...S...?.#.9...?
+000003c0: 8039 9cf9 35e8 b13f 40bc 1fb7 8ff6 b13f  .9..5..?@......?
+000003d0: c0c3 7b0e 823e b23f 2062 39f8 b4a5 b23f  ..{..>.? b9....?
+000003e0: 8008 c72c f3b7 ae3f 808a 592f 9654 b53f  ...,...?..Y/.T.?
+000003f0: 809d 0df9 0f6f be3f 0082 09dc 3aaa be3f  .....o.?....:..?
+00000400: 00bc e314 3df8 bc3f 008e 5374 d410 bd3f  ....=..?..St...?
+00000410: f091 5b93 bef3 b93f 2020 b3b3 c0f1 bb3f  ..[....?  .....?
+00000420: c0ff 8f13 c287 b83f 80c7 ea56 0fcf b63f  .......?...V...?
+00000430: c079 ac19 c932 b73f 004a 8924 1a59 b73f  .y...2.?.J.$.Y.?
+00000440: 00af 7b2b 6244 ac3f c0ae 7d01 b5ea b63f  ..{+bD.?..}....?
+00000450: 6044 696f f805 c03f 000b 5ef4 451f c33f  `Dio...?..^.E..?
+00000460: 8005 a227 c5a1 bd3f 00e4 a084 0168 c13f  ...'...?.....h.?
+00000470: 8014 e813 198b bc3f 8087 69df 1475 be3f  .......?..i..u.?
+00000480: 808d e909 0b49 bb3f 8040 d994 cb2b bb3f  .....I.?.@...+.?
+00000490: 007e c685 c3bc ba3f 0015 e3fc 6da8 bc3f  .~.....?....m..?
+000004a0: 206f f3c6 dd1c ab3f 406f f25b dcbe b53f   o.....?@o.[...?
+000004b0: e045 0a65 c11b c03f 00c0 13b3 9ef6 c23f  .E.e...?.......?
+000004c0: 80a8 13d0 2464 c03f b02b 2d23 a5fa c33f  ....$d.?.+-#...?
+000004d0: 00c1 a8a4 4ee7 be3f 403a cc97 97e1 c03f  ....N..?@:.....?
+000004e0: c05a 0872 0076 c03f 8026 c286 bb77 c03f  .Z.r.v.?.&...w.?
+000004f0: 80f0 4dd3 573c be3f 0087 8a71 2eae c13f  ..M.W<.?...q...?
+00000500: 6097 1aa1 b7bb a93f 608f de70 d790 b33f  `......?`..p...?
+00000510: 10c0 0644 9861 c13f 0072 dc29 3d87 c13f  ...D.a.?.r.)=..?
+00000520: 8049 7b83 7fca c23f a0b6 d441 94f3 c43f  .I{....?...A...?
+00000530: 4024 26a8 e120 c03f 006c cf2c 8971 c13f  @$&.. .?.l.,.q.?
+00000540: 80fb 3559 d329 c13f e0ad b9a3 bb39 c23f  ..5Y.).?.....9.?
+00000550: 003d 0d18 ee04 c23f 80dd b584 dc64 c33f  .=.....?.....d.?
+00000560: 801b f0f9 b160 a73f 2c38 cdcc d116 b43f  .....`.?,8.....?
+00000570: 40c1 feeb 7cc2 c03f 40e8 1379 f2fe c03f  @...|..?@..y...?
+00000580: 60a5 10c8 1949 c23f 8063 062a 5339 c63f  `....I.?.c.*S9.?
+00000590: 00ae 0d15 3b95 c23f 003d 7e6f 3365 c13f  ....;..?.=~o3e.?
+000005a0: 002c 7de8 92ed c23f b01a 84b9 40fe c43f  .,}....?....@..?
+000005b0: 80dc b584 8c90 c43f 0018 139b 6f23 c63f  .......?....o#.?
+000005c0: e03e 1d8f 99b9 a73f 4096 e7c1 6d62 b23f  .>.....?@...mb.?
+000005d0: 005b 2041 b11f be3f 809d 4b71 d5c5 c13f  .[ A...?..Kq...?
+000005e0: 00f1 85c9 9cfd c13f 5086 c613 f3b9 c33f  .......?P......?
+000005f0: 80f2 2900 96fb c23f c0a3 8cb8 80f4 c33f  ..)....?.......?
+00000600: 009a 7cb3 6d7f c53f 00aa c5a7 d083 c73f  ..|.m..?.......?
+00000610: 0037 6c5b b4a4 c63f 0001 8750 cd83 c83f  .7l[...?...P...?
+00000620: 90d2 7d4a 3fb3 a33f 0020 0da7 7446 b13f  ..}J?..?. ..tF.?
+00000630: 4028 29b0 e897 be3f 00c8 7bd5 ca5d c03f  @()....?..{..].?
+00000640: c0bc 395c 73a4 c13f 00d4 484b f506 c73f  ..9\s..?..HK...?
+00000650: c0cb 9717 18e4 c23f 0039 b4c8 2e5b c63f  .......?.9...[.?
+00000660: 40c2 bb5c e4c4 c53f 008e 9081 c403 c93f  @..\...?.......?
+00000670: c0e8 b985 c085 cb3f 0037 1ac0 8b1f ca3f  .......?.7.....?
+00000680: e0cd 31c5 698d a63f 0017 95d4 e92a b13f  ..1.i..?.....*.?
+00000690: c05a b56b fa7e bc3f 40f4 bf5c db6d be3f  .Z.k.~.?@..\.m.?
+000006a0: 0068 226c 18d6 c03f 0045 9db9 0738 c53f  .h"l...?.E...8.?
+000006b0: 4034 9d9d 7cf7 c43f 002f 336c dd5b c73f  @4..|..?./3l.[.?
+000006c0: 4048 8ac8 9073 c83f 0062 f7e4 6189 cd3f  @H...s.?.b..a..?
+000006d0: 004e 4a41 5718 cb3f 00c6 3368 b847 ce3f  .NJAW..?..3h.G.?
+000006e0: 00a0 6cca 0dd2 a23f 6008 008e 2575 b03f  ..l....?`...%u.?
+000006f0: cc38 a16b 280e bc3f 8066 614f fb0d bc3f  .8.k(..?.faO...?
+00000700: c0ac 50a4 6b39 c13f 00be bf41 eb72 c63f  ..P.k9.?...A.r.?
+00000710: e0aa 07cc d78d c73f 807c ed99 25b2 c83f  .......?.|..%..?
+00000720: 004a ef1b 47b0 cc3f 00d3 9ffd 08eb cf3f  .J..G..?.......?
+00000730: 0060 1a86 9ffa cf3f 80f6 1e2e 4982 d03f  .`.....?....I..?
+00000740: 6025 cade 7252 a43f 6036 0186 792a b13f  `%..rR.?`6..y*.?
+00000750: 4075 90d7 03f1 bb3f 60af 5b04 863b c03f  @u.....?`.[..;.?
+00000760: 0846 5ed6 fe9c c13f 00c8 b5a1 6291 c83f  .F^....?....b..?
+00000770: 0008 ebff 2c4e c83f 00b1 2e6e 2343 cb3f  ....,N.?...n#C.?
+00000780: 88bc e5ea 5418 d03f a028 0989 4820 d13f  ....T..?.(..H .?
+00000790: 806c b246 4d1b d13f 006e 9049 b62f d33f  .l.FM..?.n.I./.?
+000007a0: b8f8 f2a7 9692 a53f 0098 6c3c 60e9 b33f  .......?..l<`..?
+000007b0: 00fd 3218 a344 be3f 806a 300d 934e bf3f  ..2..D.?.j0..N.?
+000007c0: c0f5 b9da e292 c13f 0013 f241 5f09 c73f  .......?...A_..?
+000007d0: 0003 caa6 2c94 ca3f 0062 7ac2 1299 cd3f  ....,..?.bz....?
+000007e0: c012 9b8f 3311 d03f 80ac 6ef5 acbf d23f  ....3..?..n....?
+000007f0: c0a1 d11d bc2d d43f 00c1 3923 5230 d53f  .....-.?..9#R0.?
+00000800: c096 8fa4 80ad aa3f 80b3 7bf2 7045 b43f  .......?..{.pE.?
+00000810: 4026 fc52 7793 bf3f 2097 ab1f d7ce c03f  @&.Rw..? ......?
+00000820: 602f a2ed 541e c23f 806d 3eae ed6f ca3f  `/..T..?.m>..o.?
+00000830: 8037 328f cc2d ca3f 0030 dd24 c699 cf3f  .72..-.?.0.$...?
+00000840: 0077 1211 6416 d43f 402b 4d4a e1d0 d53f  .w..d..?@+MJ...?
+00000850: c095 b723 2448 d43f c00f 7a36 1b17 d83f  ...#$H.?..z6...?
+00000860: 00be 9448 a274 b03f 008c 50a5 e630 b93f  ...H.t.?..P..0.?
+00000870: 0023 ab5b 3df8 c03f 704e 0988 d903 c23f  .#.[=..?pN.....?
+00000880: 8069 183e d2d7 c53f 8090 1d1b 9104 c93f  .i.>...?.......?
+00000890: 0099 81ca b81a cd3f 4081 3e91 a340 d23f  .......?@.>..@.?
+000008a0: 60e0 2d90 d402 d73f 803f 0e4a 18fa d63f  `.-....?.?.J...?
+000008b0: 804a 5e9d 3b2b d73f c072 a25d 7d8c db3f  .J^.;+.?.r.]}..?
+000008c0: 2020 5f42 d1c5 b43f 00ab 0661 1a3d ba3f    _B...?...a.=.?
+000008d0: a0b7 7878 abef c33f c085 e7a5 b2e1 c33f  ..xx...?.......?
+000008e0: e082 fa96 7544 c63f 00c5 08e1 a123 cc3f  ....uD.?.....#.?
+000008f0: 8012 49f4 c274 d03f 001d e6cb 2b56 d53f  ..I..t.?....+V.?
+00000900: 80e8 d9ac 4216 d63f 4068 e89f d8ed d83f  ....B..?@h.....?
+00000910: 0012 e9b7 ef0c dc3f 000c e02d 1001 df3f  .......?...-...?
+00000920: c04b 1aa3 add3 b83f 80ff 8139 1a84 c03f  .K.....?...9...?
+00000930: 6093 dfa2 b157 c83f 40ac a92c 220a c63f  `....W.?@..,"..?
+00000940: 0025 2191 e605 c93f 801f 2922 cb61 d03f  .%!....?..)".a.?
+00000950: 0099 2a18 1559 d33f 8023 404d 25ec d53f  ..*..Y.?.#@M%..?
+00000960: 4054 e3a5 5bd4 d83f 00b2 d2a4 6491 db3f  @T..[..?....d..?
+00000970: c084 251e 6009 df3f 4096 e7c1 419b e13f  ..%.`..?@...A..?
+00000980: 6038 d6c5 d943 bd3f 4015 1bf3 e6fd c03f  `8...C.?@......?
+00000990: 00a1 a014 7d29 ca3f a02e 185c 87b6 c93f  ....}).?...\...?
+000009a0: 00af 3db3 942a cd3f 8085 251e b834 d33f  ..=..*.?..%..4.?
+000009b0: 0068 5c38 0039 d43f c05a b1bf 84ae d83f  .h\8.9.?.Z.....?
+000009c0: 0052 27a0 79d8 db3f 40ff ca4a df08 e13f  .R'.y..?@..J...?
+000009d0: e04b ab21 7d38 e13f a013 27f7 a74b e43f  .K.!}8.?..'..K.?
+000009e0: 4081 21ab dbc5 bf3f c06d dfa3 2a56 c53f  @.!....?.m..*V.?
+000009f0: 00d6 bce3 9403 d03f 4030 f5f3 2623 cf3f  .......?@0..&#.?
+00000a00: 004e 603a d5dc d03f e07f 9d9b 2022 d73f  .N`:...?.... ".?
+00000a10: c09b 5088 90bb d73f 4054 8cf3 8f10 dc3f  ..P....?@T.....?
+00000a20: 00a4 79c7 a922 e23f c055 48f9 67dc e13f  ..y..".?.UH.g..?
+00000a30: 0052 05a3 d28f e43f 003b fc35 11ce e83f  .R.....?.;.5...?
+00000a40: a01c 3f54 b67c c13f c08c 45d3 193a c73f  ..?T.|.?..E..:.?
+00000a50: 0057 cf49 b335 d23f c0dc 5ed2 a8d5 d03f  .W.I.5.?..^....?
+00000a60: 0013 f241 971a d43f c0b1 a206 d71f d93f  ...A...?.......?
+00000a70: 403b aa9a 707c db3f 0088 eb51 08b4 e13f  @;..p|.?...Q...?
+00000a80: 6063 5ddc 0e2e e23f 00c8 af72 6891 e53f  `c]....?...rh..?
+00000a90: 809f fd48 41a2 ea3f 80be 654e efcb ec3f  ...HA..?..eN...?
+00000aa0: 404f 9143 78b5 c13f 2050 e09d e8e2 ca3f  @O.Cx..? P.....?
+00000ab0: 40b0 1bb6 fdca d53f 0054 8638 d69e d33f  @......?.T.8...?
+00000ac0: d0e4 9b6d f822 d63f e063 062a 2be7 dc3f  ...m.".?.c.*+..?
+00000ad0: 00a2 01bc c517 e03f 00ea 0434 8171 e43f  .......?...4.q.?
+00000ae0: 00f5 53e3 a540 e73f c0fe 9595 4e3a ea3f  ..S..@.?....N:.?
+00000af0: 0092 ed7c ff50 ef3f d0b7 7537 076c f33f  ...|.P.?..u7.l.?
+00000b00: c019 c231 9f06 c33f 80c4 ce14 4a58 ce3f  ...1...?....JX.?
+00000b10: b8a1 629c 11f7 d63f 2060 3c83 4254 d53f  ..b....? `<.BT.?
+00000b20: 20b7 9734 06d3 d93f 4058 8b4f e172 e13f   ..4...?@X.O.r.?
+00000b30: 00f4 85c9 545d e23f 002e d49a 0613 e83f  ....T].?.......?
+00000b40: 80fd 135c 8ce9 ea3f 0058 b81e 8587 f03f  ...\...?.X.....?
+00000b50: 00b4 627f 9920 f53f c0c0 73ef e533 f53f  ..b.. .?..s..3.?
+00000b60: 008d 40bc 4e20 c23f c010 e4a0 98db d03f  ..@.N .?.......?
+00000b70: 4085 251e d820 dd3f 00cf 7f48 3f79 d83f  @.%.. .?...H?y.?
+00000b80: 6026 8a90 22d5 dd3f 80d1 18ad 13c4 e23f  `&.."..?.......?
+00000b90: a041 60e5 e018 e53f c008 c4eb 76cd ea3f  .A`....?....v..?
+00000ba0: 00ab f1d2 7d67 f03f 00ef a7c6 cbcf f23f  ....}g.?.......?
+00000bb0: c0c0 c58a 82f3 f53f 4050 6b9a 0709 fb3f  .......?@Pk....?
+00000bc0: 806e 85b0 222a c43f 4080 43a8 da5c d23f  .n.."*.?@.C..\.?
+00000bd0: 8048 ea04 94b8 dc3f 001e 8f19 6824 db3f  .H.....?....h$.?
+00000be0: 0064 af77 7fa7 e03f 00c7 bab8 2dbc e43f  .d.w...?....-..?
+00000bf0: 60b8 c7d2 1f99 e63f 6081 ad12 2040 ee3f  `......?`... @.?
+00000c00: 00da 2b65 1916 ef3f 404f 232d 154b f53f  ..+e...?@O#-.K.?
+00000c10: 00a0 b437 f80e fc3f 0020 0456 8e9c fe3f  ...7...?. .V...?
+00000c20: 8017 2653 3de4 c33f 20a3 91cf e508 d33f  ..&S=..? ......?
+00000c30: 40d4 0968 8abd e13f 8056 60c8 5a64 dd3f  @..h...?.V`.Zd.?
+00000c40: 0024 15c6 deba e13f 002c 90a0 3804 e73f  .$.....?.,..8..?
+00000c50: 200b b08f 36b0 e83f 007f d93d 396b f03f   ...6..?...=9k.?
+00000c60: 0008 3884 ae81 f33f 00e4 e995 52d8 f53f  ..8....?....R..?
+00000c70: 804c 158c aa7b fa3f e06d 6935 14d4 0040  .L...{.?.mi5...@
+00000c80: 004f b4ab 500c c63f 803d 44a3 7bc4 d33f  .O..P..?.=D.{..?
+00000c90: 80cc d1e3 1783 e03f 802c 431c bb06 df3f  .......?.,C....?
+00000ca0: 00ef 7c3f d53c e33f 80c7 7bd5 f244 e73f  ..|?.<.?..{..D.?
+00000cb0: 009d efa7 06b1 ea3f 00f4 065f 98b9 f03f  .......?..._...?
+00000cc0: 8083 7cd0 9331 f33f 0020 85eb 112c f73f  ..|..1.?. ...,.?
+00000cd0: 80a6 0a46 753f 0040 0026 3108 6cc8 0040  ...Fu?.@.&1.l..@
+00000ce0: 3078 ee3d 4057 c73f 5085 b185 ea76 d53f  0x.=@W.?P....v.?
+00000cf0: 00ff e68c a84a e33f 40c8 2423 d70f e03f  .....J.?@.$#...?
+00000d00: 00e0 675c c4ad e23f 804d 0b5e 84e9 e63f  ..g\...?.M.^...?
+00000d10: 00e2 c798 3b37 e93f 00e3 c281 3077 f13f  ....;7.?....0w.?
+00000d20: a09f 1a2f 516e f63f c081 e7de 97ff f93f  .../Qn.?.......?
+00000d30: 80c5 feb2 8bfe fe3f a02a dec8 de74 0340  .......?.*...t.@
+00000d40: 8066 4469 7f08 c93f 0083 72a2 fd2b d63f  .fDi...?..r..+.?
+00000d50: c0e4 7e87 4ac1 e23f 8a2f 1345 e30d e13f  ..~.J..?./.E...?
+00000d60: 0002 f1ba 9ef8 e33f 00ce 1951 aa8f e93f  .......?...Q...?
+00000d70: 00d0 bce3 f45c eb3f 0066 aa60 b429 f23f  .....\.?.f.`.).?
+00000d80: 80ad d348 2b8c f33f 009d 779c 629b f93f  ...H+..?..w.b..?
+00000d90: c03a e466 003e 0040 005f 984c 05d8 0140  .:.f.>.@._.L...@
+00000da0: 8079 8d5d b215 cc3f 401e 5036 9d84 d63f  .y.]...?@.P6...?
+00000db0: 0097 4c15 8c4c e33f 6081 04c5 e3a0 e13f  ..L..L.?`......?
+00000dc0: 00e4 839e cd70 e43f 8054 a4c2 e0c6 e73f  .....p.?.T.....?
+00000dd0: 90fc c1c0 af49 ec3f 0082 e2c7 b80f f33f  .....I.?.......?
+00000de0: 8019 9e5e 891b f63f 4061 a1d6 9cdd f83f  ...^...?@a.....?
+00000df0: b0d4 cf9b fa6f ff3f 20bf 0e9c e3aa 0140  .....o.? ......@
+00000e00: 40a6 26c1 9be6 cb3f 0073 11df 9593 d63f  @.&....?.s.....?
+00000e10: 8065 791e 1ce4 e23f e0c7 98bb 6673 e03f  .ey....?....fs.?
+00000e20: e00d db16 f1a1 e43f c06e d8b6 000e e93f  .......?.n.....?
+00000e30: e097 fa79 7315 ec3f 003d df4f ad00 f23f  ...ys..?.=.O...?
+00000e40: 80c0 73ef edb4 f33f a019 c572 5f73 f73f  ..s....?...r_s.?
+00000e50: 807d fb3a 2083 fc3f 00c4 f528 dc54 ff3f  .}.: ..?...(.T.?
+00000e60: 40c7 293a 623f cc3f 0049 e0d6 5dec d43f  @.):b?.?.I..]..?
+00000e70: 404d b9c2 d38f e23f 0076 2d21 4fa8 e13f  @M.....?.v-!O..?
+00000e80: 00ea 8b84 26b1 e33f 0036 92cb ff2a e53f  ....&..?.6...*.?
+00000e90: 803b 6189 f75b e83f c037 dbdc 3067 f03f  .;a..[.?.7..0g.?
+00000ea0: 800d 9c33 d2d6 f23f 40b7 7a4e 9a4a f53f  ...3...?@.zN.J.?
+00000eb0: 0068 f7e4 e106 fb3f 40a2 7a6b 9c28 0040  .h.....?@.zk.(.@
+00000ec0: 50bb 9866 c8dd cc3f 00c5 f484 1511 d53f  P..f...?.......?
+00000ed0: 0035 5eba c90a e13f c0df dbf4 c724 df3f  .5^....?.....$.?
+00000ee0: 6081 e7de eb46 e23f 0026 3108 8ca5 e53f  `....F.?.&1....?
+00000ef0: 00bf caa1 05cf e63f 003b 2cd4 3a33 ed3f  .......?.;,.:3.?
+00000f00: 4031 4278 6c0d f03f a028 9b72 3943 f33f  @1Bxl..?.(.r9C.?
+00000f10: 00df 718a 6ebd f63f 80d4 e76a 1bbc f93f  ..q.n..?...j...?
+00000f20: 003d 2cd4 02eb c83f 0047 acc5 4f05 d13f  .=,....?.G..O..?
+00000f30: 4051 31ce 5f51 dd3f 00ac 5626 1c1a dd3f  @Q1._Q.?..V&...?
+00000f40: 800d 6c95 00a6 e13f 00f8 5c6d c5c1 e13f  ..l....?..\m...?
+00000f50: 0052 17b7 7183 e43f 00a9 f6e9 24a4 e83f  .R..q..?....$..?
+00000f60: 00a5 01bc c5ce ea3f 80ff f675 d8be f03f  .......?...u...?
+00000f70: 4057 7897 2be1 f23f 00f7 e461 a15f f63f  @Wx.+..?...a._.?
+00000f80: 007d 608e 5e2b c53f 80a9 4d9c 2c2a cf3f  .}`.^+.?..M.,*.?
+00000f90: 006e ddcd 1b65 da3f 00ac 7268 d1cd d73f  .n...e.?..rh...?
+00000fa0: 00c7 e1cc 2f2b dd3f 808c 7f9f 259b df3f  ..../+.?....%..?
+00000fb0: 4084 6401 7ff9 e13f 00ff b27b f29d e53f  @.d....?...{...?
+00000fc0: a036 37a6 3399 e73f 006e 0d6c c5ef ea3f  .67.3..?.n.l...?
+00000fd0: c0e3 141d 73aa f03f 001b 868f 20e5 f23f  ....s..?.... ..?
+00000fe0: 2023 1285 0665 c33f 0018 0802 ec8b c83f   #...e.?.......?
+00000ff0: 6099 9a04 8307 d73f b035 e9b6 6a59 d63f  `......?.5..jY.?
+00001000: 005c 3bdf 8f66 db3f 4016 f6b4 1bce db3f  .\;..f.?@......?
+00001010: 004c 9d80 06f1 de3f 805b 2041 d1d4 e13f  .L.....?.[ A...?
+00001020: 402c 137e d13e e53f c01e 6d1c c1dc e83f  @,.~.>.?..m....?
+00001030: 40e9 9ac9 cf51 ec3f 004e 840d 8f90 ef3f  @....Q.?.N.....?
+00001040: 2006 f4c2 4d0f c03f 00bd 00fb 1889 c53f   ...M..?.......?
+00001050: 0054 e3a5 9bda d13f 8097 395d 26a1 d03f  .T.....?..9]&..?
+00001060: 806b 9f8e 9723 d53f 806b 82a8 bb3c d63f  .k...#.?.k...<.?
+00001070: 007f e882 4aa1 d83f 8079 978b 388a db3f  ....J..?.y..8..?
+00001080: c0a7 1dfe a233 e03f 0090 0f7a 5671 e23f  .....3.?...zVq.?
+00001090: 209e 5e29 fb8f e53f 8099 a73a 9437 e73f   .^)...?...:.7.?
+000010a0: 0034 2c46 65c7 b83f 0094 eb34 12ed bd3f  .4,Fe..?...4...?
+000010b0: 00c3 8190 4cc5 cc3f 0011 afeb 1753 cd3f  ....L..?.....S.?
+000010c0: 40b0 e1e9 35bc d13f a011 a3e7 fe91 d33f  @...5..?.......?
+000010d0: 0087 50a5 86dd d33f 00ba 6b09 c952 d83f  ..P....?..k..R.?
+000010e0: c074 caa3 87da da3f c0f4 6228 a74b e13f  .t.....?..b(.K.?
+000010f0: 00b8 5851 875b e23f 7033 15e2 5135 e43f  ..XQ.[.?p3..Q5.?
+00001100: 8029 3a92 db00 b33f c065 4e97 6972 ba3f  .):....?.eN.ir.?
+00001110: 001a a2d1 dda0 c83f 009a 9eb0 4419 c43f  .......?....D..?
+00001120: 400f 4240 ce64 cb3f c02f 478f cfc4 ca3f  @.B@.d.?./G....?
+00001130: 0000 ed47 6ade cf3f 80e9 d9ac 1a07 d33f  ...Gj..?.......?
+00001140: c0da 8afd a52e d53f 00d1 6531 811f da3f  .......?..e1...?
+00001150: 603c 8386 0e64 de3f 80cb 6779 9e62 e03f  `<...d.?..gy.b.?
+00001160: 00f7 eae3 1155 af3f 0021 6805 4684 b23f  .....U.?.!h.F..?
+00001170: 00a4 af20 4d91 c13f e0d5 7267 9650 c33f  ... M..?..rg.P.?
+00001180: 00de 3cd5 0931 c43f 0021 6c78 3aed c43f  ..<..1.?.!lx:..?
+00001190: 800d a14a bdd0 c53f 000e 897b 8cb8 cc3f  ...J...?...{...?
+000011a0: 80da c9e0 5864 d03f 8056 7380 d01b d23f  ....Xd.?.Vs....?
+000011b0: 000a a2ee 5362 d83f c094 f1ef 7306 da3f  ....Sb.?....s..?
+000011c0: c0c9 3670 6b73 a53f 806b ed7d 8af6 ad3f  ..6pks.?.k.}...?
+000011d0: 00ae 69de c1c0 b93f 0098 bb96 905b b83f  ..i....?.....[.?
+000011e0: 4023 48a5 b03c be3f 002e 39ee 1440 be3f  @#H..<.?..9..@.?
+000011f0: 00ce be2b 427a c13f c09f fd48 618e c93f  ...+Bz.?...Ha..?
+00001200: 00aa c090 f58b c93f 0056 60c8 aadd ca3f  .......?.V`....?
+00001210: 805b fe43 8a18 d03f 8027 f224 51d3 d33f  .[.C...?.'.$Q..?
+00001220: 405c 55f6 85e1 a23f 0076 c8cd 7084 a13f  @\U....?.v..p..?
+00001230: 00de c83c 4a57 b23f 0074 d712 1237 b13f  ...<JW.?.t...7.?
+00001240: 00b6 bb07 c4d5 b23f 0065 2310 6f94 b53f  .......?.e#.o..?
+00001250: c04a 77d7 a18e b83f 8002 d193 12f6 bb3f  .Jw....?.......?
+00001260: 40be 2ec3 0f99 c23f 800a f489 1c6c c53f  @......?.....l.?
+00001270: 804f 70b1 bac7 c63f 00b7 f3fd 549a cc3f  .Op....?....T..?
+00001280: c071 e0d5 4a0e 983f 6030 fc96 fb33 9c3f  .q..J..?`0...3.?
+00001290: 003b 8c49 ef31 ad3f c023 f1f2 64b2 a83f  .;.I.1.?.#..d..?
+000012a0: c098 11de b610 a93f 009b 5088 e097 af3f  .......?..P....?
+000012b0: 80d7 f50b 9616 b23f 0007 9623 7c4f b73f  .......?...#|O.?
+000012c0: 0066 2783 03e2 ba3f 0083 0d4f afb6 bf3f  .f'....?...O...?
+000012d0: 805a 9e07 f718 c23f 805e d218 7dc8 c73f  .Z.....?.^..}..?
+000012e0: 002c b98a 35f0 903f 90b0 19e0 3e1f 923f  .,..5..?....>..?
+000012f0: 00e5 5fcb 8bfd a33f 008c 9c85 7dc6 a03f  .._....?....}..?
+00001300: 00ad 1c5a a4d8 a13f d09d 9383 a2ab a53f  ...Z...?.......?
+00001310: 0034 48c1 933f a73f c003 594f fd24 b03f  .4H..?.?..YO.$.?
+00001320: 00bf 2b82 df08 b23f 0071 7ced 9956 b53f  ..+....?.q|..V.?
+00001330: 80dd 5ed2 2884 b83f 8053 aef0 0e08 c03f  ..^.(..?.S.....?
+00001340: 0068 e6c9 b546 853f 00b8 5d68 3ebf 873f  .h...F.?..]h>..?
+00001350: c041 d719 4ae5 963f 00ac c77d 6b30 983f  .A..J..?...}k0.?
+00001360: 8075 feed a21a 973f 0068 3ee7 8e37 9b3f  .u.....?.h>..7.?
+00001370: 80e6 6ed7 abcb a03f 001a ff3e 734e a73f  ..n....?...>sN.?
+00001380: 40fe 277f 5324 b03f 0074 0305 ce84 b33f  @.'.S$.?.t.....?
+00001390: 8003 caa6 ecfa b23f 00aa 0eb9 8975 b93f  .......?.....u.?
+000013a0: c0cb 176a 8f5b 7b3f 80cc b799 a98d 803f  ...j.[{?.......?
+000013b0: 8050 f9d7 62f0 8f3f 00a2 58a7 0a74 8e3f  .P..b..?..X..t.?
+000013c0: 803e 0796 4370 8e3f 00e2 ae5e 0dff 913f  .>..Cp.?...^...?
+000013d0: 0002 603c c310 9a3f 8045 9c4e 2230 9b3f  ..`<...?.E.N"0.?
+000013e0: a003 2159 30ac a33f c015 f9f5 ebaa a83f  ..!Y0..?.......?
+000013f0: 805f 7990 4e5f ae3f 8086 53e6 66f1 b33f  ._y.N_.?..S.f..?
+00001400: b099 9999 dd3c 733f 5066 6666 1473 763f  .....<s?Pfff.sv?
+00001410: 2833 3333 1ca3 853f 00c8 98bb f61d 823f  (333...?.......?
+00001420: 003d 7fda a899 833f 00ae ba0e 05a7 893f  .=.....?.......?
+00001430: 403d 7c99 3075 903f 004e bb98 c647 953f  @=|.0u.?.N...G.?
+00001440: 80f7 aa95 b9d3 9b3f c028 97c6 5729 a23f  .......?.(..W).?
+00001450: 00be a1f0 593f a83f 4087 50a5 fe57 b23f  ....Y?.?@.P..W.?
+00001460: 80dd a51e 2ba9 6b3f 4025 db0a 6313 713f  ....+.k?@%..c.q?
+00001470: 00cf 2f4a 50c5 803f 80ab d392 08ff 793f  ../JP..?......y?
+00001480: 0081 b4ff a13b 783f d022 98b4 c9d6 803f  .....;x?.".....?
+00001490: 0060 7fc8 3165 853f 0028 4696 7cf7 8d3f  .`..1e.?.(F.|..?
+000014a0: 00af ec82 010c 963f 00e6 cb0b 7056 9c3f  .......?....pV.?
+000014b0: 6069 e047 c10c a43f c0ae ec82 19ad af3f  `i.G...?.......?
+000014c0: 6033 3333 93a7 683f 807f 4754 28f7 663f  `333..h?..GT(.f?
+000014d0: 00cb 958b 1afc 743f 80fa ec80 037a 703f  ......t?.....zp?
+000014e0: 005e 0b1f 5e76 733f c0de 477f ada1 773f  .^..^vs?..G...w?
+000014f0: 5066 6666 d277 7d3f 0033 4fae 89ca 873f  Pfff.w}?.3O....?
+00001500: 0023 da8e f9ef 903f 4049 2bbe b1f8 943f  .#.....?@I+....?
+00001510: c012 f1d6 e908 a23f 6048 861c f385 a53f  .......?`H.....?
+00001520: a0cc cccc e813 663f 80ff 7167 ebbf 623f  ......f?..qg..b?
+00001530: 8021 c43a 0ac8 693f 804f 6100 5c5b 693f  .!.:..i?.Oa.\[i?
+00001540: 6033 3333 1b60 6a3f 00b2 d9ec 2399 713f  `333.`j?....#.q?
+00001550: 801e 1730 ec8d 793f 40c7 0270 95e0 813f  ...0..y?@..p...?
+00001560: 4081 f403 1106 893f 8035 04c7 151e 923f  @......?.5.....?
+00001570: 804e 965a 5f17 993f 0073 a087 5e05 a43f  .N.Z_..?.s..^..?
+00001580: c066 6666 5ec2 5b3f c066 6666 be0f 5f3f  .fff^.[?.fff.._?
+00001590: a0cc cccc c8c8 653f 00cb dcd7 b45d 693f  ......e?.....]i?
+000015a0: 00bb d6de e785 6a3f 6033 3333 5730 6d3f  ......j?`333W0m?
+000015b0: 0037 d9ab b412 723f 00f8 c43a 15de 773f  .7....r?...:..w?
+000015c0: 0071 7500 744e 833f 001f 82aa f166 8b3f  .qu.tN.?.....f.?
+000015d0: 40c1 21af e2c4 963f 805b b22a c211 a03f  @.!....?.[.*...?
+000015e0: 4099 9999 e158 5b3f 4099 9999 d150 5f3f  @....X[?@....P_?
+000015f0: a0cc cccc fca2 613f 00bd 5708 d67d 663f  ......a?..W..}f?
+00001600: 00bd 78ab 1311 633f a0cc cccc c415 683f  ..x...c?......h?
+00001610: 0006 75ca 0305 6d3f 5066 6666 d0cf 733f  ..u...m?Pfff..s?
+00001620: 8065 fcfb 5c5a 7e3f 00b4 1d53 e746 843f  .e..\Z~?...S.F.?
+00001630: 0048 e7fc d45a 8f3f 0091 a4a4 2726 973f  .H...Z.?....'&.?
+00001640: c066 6666 5ee4 503f 4099 9999 11a2 5d3f  .fff^.P?@.....]?
+00001650: 4099 9999 d96c 5c3f 6033 3333 670c 643f  @....l\?`333g.d?
+00001660: 80ec fda1 a447 5e3f 6033 3333 f36f 653f  .....G^?`333.oe?
+00001670: c0e3 e83b 69a6 673f a0cc cccc 0479 6e3f  ...;i.g?.....yn?
+00001680: 004b 5cc7 38c1 753f 0031 43e3 f938 803f  .K\.8.u?.1C..8.?
+00001690: c05b f976 cc85 893f 60da 2736 45a0 913f  .[.v...?`.'6E..?
+000016a0: 4099 9999 219f 583f 4099 9999 b904 523f  @...!.X?@.....R?
+000016b0: c0e6 244a 810f 553f 4099 9999 a1ab 5e3f  ..$J..U?@.....^?
+000016c0: c09a 971e f07c 5f3f a0cc cccc c0ff 653f  .....|_?......e?
+000016d0: 00ff 9254 961d 663f 8029 9721 099b 6c3f  ...T..f?.).!..l?
+000016e0: 80ea 6866 2767 733f 007e 7786 e43f 7b3f  ..hf'gs?.~w..?{?
+000016f0: 003d d00a 9ca1 833f c021 4ecc b7d2 8d3f  .=.....?.!N....?
```

#### Tb_err.npy

```diff
@@ -2,49 +2,49 @@
 00000010: 7227 3a20 273c 6638 272c 2027 666f 7274  r': '<f8', 'fort
 00000020: 7261 6e5f 6f72 6465 7227 3a20 4661 6c73  ran_order': Fals
 00000030: 652c 2027 7368 6170 6527 3a20 2838 342c  e, 'shape': (84,
 00000040: 292c 207d 2020 2020 2020 2020 2020 2020  ), }            
 00000050: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00000060: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00000070: 2020 2020 2020 2020 2020 2020 2020 200a                 .
-00000080: 007e 5694 b16c 4c3f 007e 5694 b16f 4b3f  .~V..lL?.~V..oK?
-00000090: 007e 5694 b11e 4d3f 00d4 336d db67 4f3f  .~V...M?..3m.gO?
-000000a0: 00c1 d435 47b3 513f 003f 2bca 5899 533f  ...5G.Q?.?+.X.S?
-000000b0: 00f2 fdda efa8 553f 0000 5ca3 bdd5 563f  ......U?..\...V?
-000000c0: 003f 2bca d8a1 573f 005d 469f 8211 573f  .?+...W?.]F...W?
-000000d0: 000e bc17 4025 563f 00a0 438a 81cc 543f  ....@%V?..C...T?
-000000e0: 0062 0024 cdb5 533f 409e 282b c780 523f  .b.$..S?@.(+..R?
-000000f0: 00d2 6945 d157 523f 00f4 5c96 b124 523f  ..iE.WR?..\..$R?
-00000100: 006d d7ec d837 523f 0098 2d76 3dec 513f  .m...7R?..-v=.Q?
-00000110: 004c d7c0 d17d 523f 003f 2bca 78c5 523f  .L...}R?.?+.x.R?
-00000120: 009f 698a 8f61 533f 00e8 6074 9f29 543f  ..i..aS?..`t.)T?
-00000130: 00f4 0310 fece 543f 00d0 c103 c330 553f  ......T?.....0U?
-00000140: 0088 1d07 da7e 553f 003f 2bca 9818 563f  .....~U?.?+...V?
-00000150: 00e4 360a dbb9 563f 00c0 fab0 775b 573f  ..6...V?....w[W?
-00000160: 007a a593 361c 583f 0041 7b27 67b1 583f  .z..6.X?.A{'g.X?
-00000170: 006c a738 850b 593f 00d8 62b4 299a 593f  .l.8..Y?..b.).Y?
-00000180: 4006 9849 0b24 5a3f 108a 7ee5 1b91 5a3f  @..I.$Z?..~...Z?
-00000190: 80a6 bdb3 64fc 5a3f 00e4 b52b ffae 5b3f  ....d.Z?...+..[?
-000001a0: 00b3 cdc7 780d 5c3f 00f2 1a41 0d00 5c3f  ....x.\?...A..\?
-000001b0: 00ac ac46 5975 5b3f 00c8 288b 39df 593f  ...FYu[?..(.9.Y?
-000001c0: 806b 3764 9b65 583f 006b 3565 8ce6 563f  .k7d.eX?.k5e..V?
-000001d0: 0008 020f b87d 553f 00ec 1309 3aa9 533f  .....}U?....:.S?
-000001e0: a005 c4e6 11de 513f 00fc 1b88 da63 503f  ......Q?.....cP?
-000001f0: 00be c0fd cbdf 4d3f 0036 61d3 8748 4b3f  ......M?.6a..HK?
-00000200: 00d6 b44e 1c0b 493f 006c 1bfd 7fa7 463f  ...N..I?.l....F?
-00000210: 00aa e196 e462 443f 0020 e5a4 dc9f 423f  .....bD?. ....B?
-00000220: 00da 109f a40a 413f 00d0 06b1 4a56 3e3f  ......A?....JV>?
-00000230: 00a8 aa01 2280 3b3f 0074 2056 23f8 393f  ....".;?.t V#.9?
-00000240: 000c 3d78 5204 393f 00f8 80d1 97c0 373f  ..=xR.9?......7?
-00000250: 006c f6db 6f06 363f 003c bf73 ca57 353f  .l..o.6?.<.s.W5?
-00000260: 0018 2f9f 10e2 343f 00f8 0840 5aa4 343f  ../...4?...@Z.4?
-00000270: 009c 4773 7f49 343f 00b8 6d61 2d11 343f  ..Gs.I4?..ma-.4?
-00000280: 0020 24f8 a9a6 333f 0084 1b3c 3045 333f  . $...3?...<0E3?
-00000290: 0008 4c28 56e1 313f 0068 6179 b45a 313f  ..L(V.1?.hay.Z1?
-000002a0: 006c fbdb e099 303f 0078 37c1 7160 303f  .l....0?.x7.q`0?
-000002b0: 0034 69c4 7f37 303f 0084 ceb6 a55a 303f  .4i..70?.....Z0?
-000002c0: 00e0 5486 bd72 303f 0058 be2a e688 313f  ..T..r0?.X.*..1?
-000002d0: 0070 97b1 e486 313f 0028 2fa8 5fb3 303f  .p....1?.(/._.0?
-000002e0: 000c 5c97 58b1 303f 0084 9762 65ac 303f  ..\.X.0?...be.0?
-000002f0: 00c0 213e e0c1 303f 00f0 b68c cb37 313f  ..!>..0?.....71?
-00000300: 002c 0528 1ec1 303f 0044 408f eab8 303f  .,.(..0?.D@...0?
-00000310: 0090 e49e 500a 313f 0084 2f42 e4ba 303f  ....P.1?../B..0?
+00000080: 0000 0000 c059 a83f 0000 0000 c091 a63f  .....Y.?.......?
+00000090: 0000 0000 c087 a83f 0000 0000 8058 aa3f  .......?.....X.?
+000000a0: 0000 0000 c079 ad3f 0000 0000 20aa b03f  .....y.?.... ..?
+000000b0: 00f9 9ffc 7d30 b23f 8099 5fcd 71f7 b23f  ....}0.?.._.q..?
+000000c0: 0054 abaf ee2a b43f 0000 0000 608a b33f  .T...*.?....`..?
+000000d0: 0000 0000 200b b33f 0069 3524 ee30 b13f  .... ..?.i5$.0.?
+000000e0: 0000 0000 c0ac b03f 0022 5f09 a411 af3f  .......?."_....?
+000000f0: 0000 0000 0051 ae3f 0082 3463 91fa ad3f  .....Q.?..4c...?
+00000100: 00b2 4ae9 59c4 ad3f 00a0 ee03 90ee ad3f  ..J.Y..?.......?
+00000110: 00d6 3906 a479 ae3f 0014 9678 8090 af3f  ..9..y.?...x...?
+00000120: 0035 24ee 5156 b03f 0060 c3d3 ab9e b03f  .5$.QV.?.`.....?
+00000130: 006c 26df ec2e b13f 0024 1907 518d b13f  .l&....?.$..Q..?
+00000140: 000a 80f1 0c15 b23f 0018 170e 846d b23f  .......?.....m.?
+00000150: 00ae 22a3 e310 b33f 00d7 868a 11ab b33f  .."....?.......?
+00000160: 000e 6c95 e04c b43f 80a9 8251 09af b43f  ..l..L.?...Q...?
+00000170: 00c1 c6f5 5f04 b53f 0098 c2f5 2852 b53f  ...._..?....(R.?
+00000180: 00b0 8a37 328c b53f 00d8 5a5f a4b7 b53f  ...72..?..Z_...?
+00000190: 003a 02b8 1924 b63f 00f0 0dbe 30bb b63f  .:...$.?....0..?
+000001a0: 0056 f146 e643 b73f 00f3 716d a8b2 b73f  .V.F.C.?..qm...?
+000001b0: 00dc 0720 357f b63f 004c 158c cacf b53f  ... 5..?.L.....?
+000001c0: 00a4 c2d8 8279 b43f 007e 6fd3 df01 b33f  .....y.?.~o....?
+000001d0: 00c8 957a f6b7 b13f 002f 698c 363d b03f  ...z...?./i.6=.?
+000001e0: 0098 512c 3787 ad3f 008a fd65 f7dc aa3f  ..Q,7..?...e...?
+000001f0: 00ac 915d 2992 a83f 0092 442f a35f a63f  ...])..?..D/._.?
+00000200: 00ca 4a93 d212 a43f 003e 7441 fd13 a23f  ..J....?.>tA...?
+00000210: 0034 677d 0a3d a03f 00ac 7b64 f385 9d3f  .4g}.=.?..{d...?
+00000220: 0014 7ea9 1f3a 9b3f 00f8 307b d94e 983f  ..~..:.?..0{.N.?
+00000230: 006c d102 f43e 963f 00a4 164a a6b1 943f  .l...>.?...J...?
+00000240: 00d0 926c 9a2f 943f 00c8 90be a4e1 933f  ...l./.?.......?
+00000250: 0050 eca1 7d65 933f 0094 f1de 0735 923f  .P..}e.?.....5.?
+00000260: 009c 5ab6 564d 913f 0004 b39d 4af0 903f  ..Z.VM.?....J..?
+00000270: 0050 c47d bf7d 913f 00d8 9c39 da4f 923f  .P.}.}.?...9.O.?
+00000280: 0010 dcdc f383 923f 0058 40a1 1ef7 913f  .......?.X@....?
+00000290: 0094 8103 5a60 913f 003c fe0b 8472 903f  ....Z`.?.<...r.?
+000002a0: 0068 ea3c 2a5d 8f3f 0090 f5d4 ea04 8f3f  .h.<*].?.......?
+000002b0: 00b8 dbf5 d2f9 8e3f 00f8 22da 8e77 8f3f  .......?.."..w.?
+000002c0: 0068 c70d bf19 8f3f 00b8 5f3e 5954 8f3f  .h.....?.._>YT.?
+000002d0: 0060 adda 3589 8f3f 0008 2e56 547b 8f3f  .`..5..?...VT{.?
+000002e0: 0004 86ac ee9d 8f3f 004c 76a5 6560 8f3f  .......?.Lv.e`.?
+000002f0: 00b8 3b6b b7a3 8f3f 0028 04ab ea36 8f3f  ..;k...?.(...6.?
+00000300: 0040 6150 a6a8 8f3f 0054 3063 0a39 8f3f  .@aP...?.T0c.9.?
+00000310: 0044 0da6 e14c 8f3f 00e4 1ed9 5c4c 8f3f  .D...L.?....\L.?
```

#### Ts_err.npy

```diff
@@ -2,49 +2,49 @@
 00000010: 7227 3a20 273c 6638 272c 2027 666f 7274  r': '<f8', 'fort
 00000020: 7261 6e5f 6f72 6465 7227 3a20 4661 6c73  ran_order': Fals
 00000030: 652c 2027 7368 6170 6527 3a20 2838 342c  e, 'shape': (84,
 00000040: 292c 207d 2020 2020 2020 2020 2020 2020  ), }            
 00000050: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00000060: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00000070: 2020 2020 2020 2020 2020 2020 2020 200a                 .
-00000080: 0046 0c8c 3e3e 753f 4033 0e68 2aff 723f  .F..>>u?@3.h*.r?
-00000090: 8063 ddab 16b8 713f c089 9043 aa53 703f  .c....q?...C.Sp?
-000000a0: c038 8e5b 0f62 6d3f 00b3 199d 76c7 6a3f  .8.[.bm?....v.j?
-000000b0: 80d5 3675 5423 683f 007a 3e5e e1c6 653f  ..6uT#h?.z>^..e?
-000000c0: 0040 a0ed a187 643f 0026 7eb7 fbd6 623f  .@....d?.&~...b?
-000000d0: 0067 efba 1ed5 613f 00d4 9655 bc27 613f  .g....a?...U.'a?
-000000e0: 0090 8021 d85c 603f 006a 06fd 1b65 5f3f  ...!.\`?.j...e_?
-000000f0: 006f 009b 616d 5f3f 0064 bb3c a027 5e3f  .o..am_?.d.<.'^?
-00000100: 0008 7113 ff6d 5d3f 00b8 e850 7983 5c3f  ..q..m]?...Py.\?
-00000110: 00b8 0057 4ed0 5b3f 00b4 7c9e f571 5b3f  ...WN.[?..|..q[?
-00000120: 0024 a483 ecc9 5a3f 0098 3295 58cf 5a3f  .$....Z?..2.X.Z?
-00000130: 0086 d913 b5b9 5a3f 00ba e4d3 21af 593f  ......Z?....!.Y?
-00000140: 0088 fd76 60df 583f 0068 4e6e ec60 583f  ...v`.X?.hNn.`X?
-00000150: 201f ea40 51eb 573f e0fc e12e 282f 573f   ..@Q.W?....(/W?
-00000160: 0040 ed40 4932 573f 007c f733 428d 563f  .@.@I2W?.|.3B.V?
-00000170: 004e 6604 89cc 553f 8065 fa53 a095 553f  .Nf...U?.e.S..U?
-00000180: 008a c5ed e46d 553f 003c 65e4 4d3f 553f  .....mU?.<e.M?U?
-00000190: 7032 a90a be6d 553f 00c9 69eb 9389 553f  p2...mU?..i...U?
-000001a0: 00bc 2e3d 9ca0 553f 0066 b5dc 52bb 553f  ...=..U?.f..R.U?
-000001b0: 00ec 85a6 4430 553f 00ad 45ec 0864 543f  ....D0U?..E..dT?
-000001c0: 0029 d0d1 9991 533f 00a8 97c5 46ea 523f  .)....S?....F.R?
-000001d0: 8075 231c 9962 523f 00b6 70aa dadd 513f  .u#..bR?..p...Q?
-000001e0: 807a 4038 8551 513f 80d6 f9fb 85d1 503f  .z@8.QQ?......P?
-000001f0: 605a 7ee1 a612 503f 00bc 1316 0cd8 4e3f  `Z~...P?......N?
-00000200: 0010 568a 17e7 4c3f 40c9 d30f 15d2 4a3f  ..V...L?@.....J?
-00000210: 803f cf6f 61b1 483f 001c 04f4 2408 473f  .?.oa.H?....$.G?
-00000220: 0094 c6ee 7055 453f 00b8 089f 87b3 433f  ....pUE?......C?
-00000230: 0024 16b4 2d90 423f 008a 6870 3ba2 413f  .$..-.B?..hp;.A?
-00000240: 007c da29 4990 403f 0064 1992 710a 3f3f  .|.)I.@?.d..q.??
-00000250: 00c0 4d78 1d59 3d3f 007c 263a 3585 3b3f  ..Mx.Y=?.|&:5.;?
-00000260: 0064 a0b8 c366 3b3f 0044 3cda 98c1 3b3f  .d...f;?.D<...;?
-00000270: 0084 e969 df75 3b3f 002c 6c5c bcd3 3b3f  ...i.u;?.,l\..;?
-00000280: 0074 9cc0 c3c4 3b3f 00f4 5928 3d6e 3b3f  .t....;?..Y(=n;?
-00000290: 0090 53f3 0af7 3a3f 00ac 8a4c d8d7 3a3f  ..S...:?...L..:?
-000002a0: 00c8 fb0f a49f 393f 00b0 8789 5e0c 3a3f  ......9?....^.:?
-000002b0: 0020 7cf7 1e32 393f 0008 b9b9 2328 393f  . |..29?....#(9?
-000002c0: 0000 7247 c999 3a3f 0008 0104 57c6 393f  ..rG..:?....W.9?
-000002d0: 0088 ad2f 867c 3a3f 0060 c1d7 0191 393f  .../.|:?.`....9?
-000002e0: 00d0 60b9 839c 393f 00d0 f6a3 962d 3a3f  ..`...9?.....-:?
-000002f0: 0078 2637 d457 3a3f 0080 6865 05e3 393f  .x&7.W:?..he..9?
-00000300: 00a8 3d1b 23c1 3a3f 00c0 3846 d362 3a3f  ..=.#.:?..8F.b:?
-00000310: 0030 4873 3ead 393f 0010 36bd 4cc0 393f  .0Hs>.9?..6.L.9?
+00000080: 00b5 f814 b08c e63f 7838 7172 5af9 e53f  .......?x8qrZ..?
+00000090: c02e 4ca6 ca62 e63f 0051 d191 fca8 e43f  ..L..b.?.Q.....?
+000000a0: 00dc e00b 1325 e33f 004c c1a8 a456 e13f  .....%.?.L...V.?
+000000b0: 40af c91a 85f1 dd3f 0000 54e3 a5a5 d93f  @......?..T....?
+000000c0: 00bc d32b a56b d63f 0046 2575 6280 d33f  ...+.k.?.F%ub..?
+000000d0: 0098 0f7a f6df d03f 006f aa43 2e4c cd3f  ...z...?.o.C.L.?
+000000e0: 004d 97c5 4413 c93f 002e dd24 8633 c53f  .M..D..?...$.3.?
+000000f0: 80f6 3b14 2531 c23f 80ab 0304 538f be3f  ..;.%1.?....S..?
+00000100: c0aa 510f 0198 b93f 008a 5b77 f3c7 b53f  ..Q....?..[w...?
+00000110: 00b8 e045 ff82 b23f 00d4 7d00 12dc af3f  ...E...?..}....?
+00000120: 00e0 4f8d 97d8 ab3f 00de 8e70 7a36 a83f  ..O....?...pz6.?
+00000130: 40ec f7c4 528b a53f 000e c479 e0c9 a23f  @...R..?...y...?
+00000140: 0050 de8e 70bd a03f 8036 7d76 9093 9e3f  .P..p..?.6}v...?
+00000150: 00ed d5c7 c328 9c3f 0066 2d05 0436 9a3f  .....(.?.f-..6.?
+00000160: 00f4 8aa7 fe94 983f 00b7 7c24 6560 973f  .......?..|$e`.?
+00000170: 00fc 8ba0 319b 963f 0044 ff04 9700 963f  ....1..?.D.....?
+00000180: 80fe d98f 44d3 953f 0078 7b10 020e 963f  ....D..?.x{....?
+00000190: 003f 9292 4ed0 963f 008a b663 2a17 983f  .?..N..?...c*..?
+000001a0: 0068 d443 348b 993f 0074 637a c20c 9b3f  .h.C4..?.tcz...?
+000001b0: 004c 766c 04c2 9c3f 00b4 2e6e 8315 9e3f  .Lvl...?...n...?
+000001c0: 0009 2ae3 1fcc 9f3f 00c9 8e8d e0dc a03f  ..*....?.......?
+000001d0: 006c 9560 f1dc a13f 0014 7a36 abde a23f  .l.`...?..z6...?
+000001e0: 005c 68ae 53f0 a33f 00c8 98bb 1611 a53f  .\h.S..?.......?
+000001f0: 00f0 b1f4 e11e a63f 001c 2922 43e6 a63f  .......?..)"C..?
+00000200: 0098 16bc 684b a73f 0050 7424 1757 a73f  ....hK.?.Pt$.W.?
+00000210: 0000 be4d 7f39 a73f 0078 711b 0dbc a63f  ...M.9.?.xq....?
+00000220: 0008 4625 f523 a63f 0040 041c 4245 a53f  ..F%.#.?.@..BE.?
+00000230: 0050 43e2 1e8c a43f 00cc 10c7 bae7 a33f  .PC....?.......?
+00000240: 0048 1075 9fe3 a33f 00a8 9a20 6ab7 a33f  .H.u...?... j..?
+00000250: 00c8 71a7 f4ed a33f 0010 cd75 9af6 a33f  ..q....?...u...?
+00000260: 00f4 3559 a3cf a33f 0024 b589 9391 a33f  ..5Y...?.$.....?
+00000270: 00cc 9e59 1252 a33f 0098 5088 801b a33f  ...Y.R.?..P....?
+00000280: 0000 fbe8 d453 a33f 00f8 065f 98c8 a33f  .....S.?..._...?
+00000290: 00f0 a353 5770 a43f 00a8 4fe4 498c a43f  ...SWp.?..O.I..?
+000002a0: 0080 e882 faa4 a43f 0040 cbf3 e0f1 a43f  .......?.@.....?
+000002b0: 0000 6edd cdc0 a53f 0048 809a 5abd a53f  ..n....?.H..Z..?
+000002c0: 00d8 9717 60e1 a53f 0038 2b30 6497 a63f  ....`..?.8+0d..?
+000002d0: 0050 cea5 b839 a73f 00f0 6bb2 46ce a63f  .P...9.?..k.F..?
+000002e0: 0000 e78c 280f a73f 00e0 ed08 a74d a83f  ....(..?.....M.?
+000002f0: 00f8 3f87 f9c0 a73f 0050 ffe7 302f a93f  ..?....?.P..0/.?
+00000300: 00f8 6470 9494 a83f 0020 8ffc c181 a83f  ..dp...?. .....?
+00000310: 00e0 0b93 a973 a93f 0060 fb74 3c02 aa3f  .....s.?.`.t<..?
```

#### xHI_err.npy

```diff
@@ -3,48 +3,48 @@
 00000020: 7261 6e5f 6f72 6465 7227 3a20 4661 6c73  ran_order': Fals
 00000030: 652c 2027 7368 6170 6527 3a20 2838 342c  e, 'shape': (84,
 00000040: 292c 207d 2020 2020 2020 2020 2020 2020  ), }            
 00000050: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00000060: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00000070: 2020 2020 2020 2020 2020 2020 2020 200a                 .
 00000080: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000090: 0000 00a0 c40a da3a 0000 1ae9 fbf7 033f  .......:.......?
-000000a0: 0040 c505 fbb8 233f 00b4 744f e8e8 313f  .@....#?..tO..1?
-000000b0: 0038 482d b919 383f 00e4 7d66 dabf 3c3f  .8H-..8?..}f..<?
-000000c0: 00d8 9a08 762a 3c3f 00d4 79f9 c273 3b3f  ....v*<?..y..s;?
-000000d0: 6060 b499 338c 393f 0058 3a8b 8363 373f  ``..3.9?.X:..c7?
-000000e0: 0040 34e2 b89c 353f 00b8 f9fc e627 353f  .@4...5?.....'5?
-000000f0: 0050 d21e 8af8 333f 0068 3f9c d122 343f  .P....3?.h?.."4?
-00000100: 00f8 3878 cb43 333f 00a0 ffdc 5fb3 323f  ..8x.C3?...._.2?
-00000110: 0030 e752 5cd3 323f 0080 2766 bd47 323f  .0.R\.2?..'f.G2?
-00000120: 0030 993b 444a 323f 0020 521d bcd2 313f  .0.;DJ2?. R...1?
-00000130: 00a8 a5b9 15bf 313f 0048 aa39 8acc 303f  ......1?.H.9..0?
-00000140: 00d0 073d 9bd5 2f3f 0010 b83c d6f2 2e3f  ...=../?...<...?
-00000150: 00b0 1f73 af31 2f3f 0090 6b54 f1b2 2e3f  ...s.1/?..kT...?
-00000160: 0080 f596 1753 2d3f 0020 0ce1 3d98 2a3f  .....S-?. ..=.*?
-00000170: 00a0 073e 0603 293f 00c0 5d9b 3214 293f  ...>..)?..].2.)?
-00000180: 0030 f9c1 54de 293f 0000 76a7 3b5d 283f  .0..T.)?..v.;](?
-00000190: 0030 7288 b8bb 263f 0070 bac0 402d 2b3f  .0r...&?.p..@-+?
-000001a0: 0090 75aa 7c79 273f 0040 214c 9b2b 2e3f  ..u.|y'?.@!L.+.?
-000001b0: 00f8 4f48 7c73 303f 00c0 63f5 fdfe 263f  ..OH|s0?..c...&?
-000001c0: 0030 221e e41a 2a3f 0030 e2e0 7738 203f  .0"...*?.0..w8 ?
-000001d0: 0090 b6cf cf13 203f 00a0 1d87 66c7 163f  ...... ?....f..?
-000001e0: 0000 9d7c 1f9f 163f 00a0 9e0b 7e7a 133f  ...|...?....~z.?
-000001f0: 00c0 f3c4 73ae 0f3f 0000 18ad 4809 0f3f  ....s..?....H..?
-00000200: 0000 ea77 6163 083f 0080 8802 c72f 063f  ...wac.?...../.?
-00000210: 0040 ff21 fdae 043f 0000 505e 1a25 023f  .@.!...?..P^.%.?
-00000220: 0000 237e 6aa1 fc3e 0080 2a29 c15c fd3e  ..#~j..>..*).\.>
-00000230: 0000 7903 ccec f73e 0000 44e9 c143 f73e  ..y....>..D..C.>
-00000240: 0080 bde4 dadb f63e 0000 dacf bd32 f63e  .......>.....2.>
-00000250: 0000 4a8c aff7 f33e 0000 4df6 cf53 ef3e  ..J....>..M..S.>
-00000260: 0000 1cab deeb d83e 0000 f8cb 82a4 d43e  .......>.......>
-00000270: 0000 40f1 0893 cf3e 0000 70b5 f322 ca3e  ..@....>..p..".>
-00000280: 0000 e0a3 0f27 c43e 0000 34fd 1271 c03e  .....'.>..4..q.>
-00000290: 0000 08ad 2c76 bb3e 0000 a85f 330a b43e  ....,v.>..._3..>
-000002a0: 0000 6017 450f b73e 0000 80c9 7cf6 ac3e  ..`.E..>....|..>
-000002b0: 0000 c8db b694 b13e 0000 605a a1a3 ae3e  .......>..`Z...>
-000002c0: 0000 2036 5838 b43e 0000 e840 20e1 b23e  .. 6X8.>...@ ..>
-000002d0: 0000 a0e1 17a8 b13e 0000 58a7 6f3e b33e  .......>..X.o>.>
-000002e0: 0000 b0cf 08db b13e 0000 6870 00a2 b03e  .......>..hp...>
-000002f0: 0000 c0dd 0f2e ad3e 0000 d8b1 ef2f b23e  .......>...../.>
-00000300: 0000 c883 995b b53e 0000 18e3 a194 b03e  .....[.>.......>
-00000310: 0000 407b ab64 ac3e 0000 0088 cca6 b23e  ..@{.d.>.......>
+00000090: 0000 0000 168f 9c3c 0020 ec80 9011 f43e  .......<. .....>
+000000a0: 0020 3031 f129 253f 0080 eac4 ca41 343f  . 01.)%?.....A4?
+000000b0: 00e4 0c6a e43a 3f3f 00de b1d8 665f 403f  ...j.:??....f_@?
+000000c0: 0038 1ec7 ea71 413f 00ba f138 9619 413f  .8...qA?...8..A?
+000000d0: 8027 a5fb 5422 403f 0090 8e72 30a8 3d3f  .'..T"@?...r0.=?
+000000e0: 0010 b68e 6081 3c3f 0014 a930 3676 3b3f  ....`.<?...06v;?
+000000f0: 00a8 47d0 4e65 3b3f 0020 424b 0d99 3f3f  ..G.Ne;?. BK..??
+00000100: 00d8 8228 a93a 3f3f 0080 9642 7b4b 3f3f  ...(.:??...B{K??
+00000110: 0038 01e1 9e9f 3f3f 0038 8cee c52f 3f3f  .8....??.8.../??
+00000120: 0058 b19d 94fe 3d3f 0078 ba98 0b16 3c3f  .X....=?.x....<?
+00000130: 00f8 bbd2 8d82 3b3f 0018 bc0a 844f 3a3f  ......;?.....O:?
+00000140: 00e8 79cb 300d 393f 0038 8474 c2c2 373f  ..y.0.9?.8.t..7?
+00000150: 0078 351e 11a0 373f 00e0 61c9 0bdf 353f  .x5...7?..a...5?
+00000160: 0070 b7da 79dc 343f 0080 901b 3428 353f  .p..y.4?....4(5?
+00000170: 00d8 30e8 295a 353f 0050 f712 7471 343f  ..0.)Z5?.P..tq4?
+00000180: 0098 068f 804f 333f 00f0 551a e7ee 333f  .....O3?..U...3?
+00000190: 0090 9ec7 cdce 353f 0060 1dc7 0f17 393f  ......5?.`....9?
+000001a0: 0050 05a3 9274 3d3f 00d0 0935 9e09 3f3f  .P...t=?...5..??
+000001b0: 0078 f4bf 5ca6 3b3f 0008 f31e 6775 373f  .x..\.;?....gu7?
+000001c0: 0060 f547 188e 343f 0070 6957 7c80 323f  .`.G..4?.piW|.2?
+000001d0: 0050 5fa7 a21e 2f3f 00b0 9954 7ee7 283f  .P_.../?...T~.(?
+000001e0: 0090 1d2c adcc 243f 00a0 499b aa9d 213f  ...,..$?..I...!?
+000001f0: 0040 dd84 31fc 1d3f 0000 552c 23ee 1a3f  .@..1..?..U,#..?
+00000200: 00a0 df9c b6c7 173f 0060 ec3a 0abe 143f  .......?.`.:...?
+00000210: 0060 856c 6aae 103f 0080 3c21 8514 0c3f  .`.lj..?..<!...?
+00000220: 0080 5bd8 89c1 083f 0000 2cb3 ad4b 043f  ..[....?..,..K.?
+00000230: 0080 9fee f22b 023f 0080 b612 15d5 ff3e  .....+.?.......>
+00000240: 0080 bc6d 4b49 fd3e 0000 b0f0 e459 f83e  ...mKI.>.....Y.>
+00000250: 0000 b673 5038 f63e 0080 74f7 ef80 f33e  ...sP8.>..t....>
+00000260: 0000 72aa 108a e53e 0000 fc65 4112 e13e  ..r....>...eA..>
+00000270: 0000 4c10 1aa6 de3e 0000 087f 75cb db3e  ..L....>....u..>
+00000280: 0000 102e 786c d83e 0000 9a7e 89b8 d63e  ....xl.>...~...>
+00000290: 0000 bed4 7422 d83e 0000 ead7 8c02 d73e  ....t".>.......>
+000002a0: 0000 d845 d1c3 d63e 0000 d066 3061 d53e  ...E...>...f0a.>
+000002b0: 0000 f2b6 2d65 d63e 0000 4c2b 74d4 d53e  ....-e.>..L+t..>
+000002c0: 0000 78f2 e971 d53e 0000 c6ef b7c7 d53e  ..x..q.>.......>
+000002d0: 0000 68f8 056a d53e 0000 2a16 64b0 d53e  ..h..j.>..*.d..>
+000002e0: 0000 ec33 c2f6 d43e 0000 1a1c 80a8 d63e  ...3...>.......>
+000002f0: 0000 4804 3e5a d63e 0000 76ec fb0b d63e  ..H.>Z.>..v....>
+00000300: 0000 f260 e6d6 d63e 0000 3a87 d75a d63e  ...`...>..:..Z.>
+00000310: 0000 9890 6a73 d53e 0000 00de 4c56 d63e  ....js.>....LV.>
```

#### tau_err.npy

```diff
@@ -2,8 +2,8 @@
 00000010: 7227 3a20 273c 6638 272c 2027 666f 7274  r': '<f8', 'fort
 00000020: 7261 6e5f 6f72 6465 7227 3a20 4661 6c73  ran_order': Fals
 00000030: 652c 2027 7368 6170 6527 3a20 2829 2c20  e, 'shape': (), 
 00000040: 7d20 2020 2020 2020 2020 2020 2020 2020  }               
 00000050: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00000060: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00000070: 2020 2020 2020 2020 2020 2020 2020 200a                 .
-00000080: c8aa 7c82 c774 d33f                      ..|..t.?
+00000080: 008c e3f9 ccb9 113f                      .......?
```

