# Comparing `tmp/pyhf-0.7.1.tar.gz` & `tmp/pyhf-0.7.2.tar.gz`

## Comparing `pyhf-0.7.1.tar` & `pyhf-0.7.2.tar`

### file list

```diff
@@ -1,88 +1,88 @@
--rw-r--r--   0        0        0     2526 2020-02-02 00:00:00.000000 pyhf-0.7.1/CITATION.cff
--rw-r--r--   0        0        0     1164 2020-02-02 00:00:00.000000 pyhf-0.7.1/src/pyhf/__init__.py
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 pyhf-0.7.1/src/pyhf/_version.py
--rw-r--r--   0        0        0     4036 2020-02-02 00:00:00.000000 pyhf-0.7.1/src/pyhf/compat.py
--rw-r--r--   0        0        0     9892 2020-02-02 00:00:00.000000 pyhf-0.7.1/src/pyhf/constraints.py
--rw-r--r--   0        0        0     4751 2020-02-02 00:00:00.000000 pyhf-0.7.1/src/pyhf/events.py
--rw-r--r--   0        0        0     2992 2020-02-02 00:00:00.000000 pyhf-0.7.1/src/pyhf/mixins.py
--rw-r--r--   0        0        0    11335 2020-02-02 00:00:00.000000 pyhf-0.7.1/src/pyhf/patchset.py
--rw-r--r--   0        0        0    32155 2020-02-02 00:00:00.000000 pyhf-0.7.1/src/pyhf/pdf.py
--rw-r--r--   0        0        0     9529 2020-02-02 00:00:00.000000 pyhf-0.7.1/src/pyhf/probability.py
--rw-r--r--   0        0        0    17487 2020-02-02 00:00:00.000000 pyhf-0.7.1/src/pyhf/readxml.py
--rw-r--r--   0        0        0     5684 2020-02-02 00:00:00.000000 pyhf-0.7.1/src/pyhf/simplemodels.py
--rw-r--r--   0        0        0     2893 2020-02-02 00:00:00.000000 pyhf-0.7.1/src/pyhf/typing.py
--rw-r--r--   0        0        0     4425 2020-02-02 00:00:00.000000 pyhf-0.7.1/src/pyhf/utils.py
--rw-r--r--   0        0        0    34829 2020-02-02 00:00:00.000000 pyhf-0.7.1/src/pyhf/workspace.py
--rw-r--r--   0        0        0    10923 2020-02-02 00:00:00.000000 pyhf-0.7.1/src/pyhf/writexml.py
--rw-r--r--   0        0        0      387 2020-02-02 00:00:00.000000 pyhf-0.7.1/src/pyhf/cli/__init__.py
--rw-r--r--   0        0        0     1299 2020-02-02 00:00:00.000000 pyhf-0.7.1/src/pyhf/cli/cli.py
--rw-r--r--   0        0        0      981 2020-02-02 00:00:00.000000 pyhf-0.7.1/src/pyhf/cli/complete.py
--rw-r--r--   0        0        0     7049 2020-02-02 00:00:00.000000 pyhf-0.7.1/src/pyhf/cli/infer.py
--rw-r--r--   0        0        0     4461 2020-02-02 00:00:00.000000 pyhf-0.7.1/src/pyhf/cli/patchset.py
--rw-r--r--   0        0        0     3815 2020-02-02 00:00:00.000000 pyhf-0.7.1/src/pyhf/cli/rootio.py
--rw-r--r--   0        0        0    12719 2020-02-02 00:00:00.000000 pyhf-0.7.1/src/pyhf/cli/spec.py
--rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 pyhf-0.7.1/src/pyhf/contrib/__init__.py
--rw-r--r--   0        0        0     2051 2020-02-02 00:00:00.000000 pyhf-0.7.1/src/pyhf/contrib/cli.py
--rw-r--r--   0        0        0     6313 2020-02-02 00:00:00.000000 pyhf-0.7.1/src/pyhf/contrib/utils.py
--rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 pyhf-0.7.1/src/pyhf/contrib/viz/__init__.py
--rw-r--r--   0        0        0    13476 2020-02-02 00:00:00.000000 pyhf-0.7.1/src/pyhf/contrib/viz/brazil.py
--rw-r--r--   0        0        0      699 2020-02-02 00:00:00.000000 pyhf-0.7.1/src/pyhf/data/citation.bib
--rw-r--r--   0        0        0     5483 2020-02-02 00:00:00.000000 pyhf-0.7.1/src/pyhf/exceptions/__init__.py
--rw-r--r--   0        0        0     8939 2020-02-02 00:00:00.000000 pyhf-0.7.1/src/pyhf/infer/__init__.py
--rw-r--r--   0        0        0    38704 2020-02-02 00:00:00.000000 pyhf-0.7.1/src/pyhf/infer/calculators.py
--rw-r--r--   0        0        0     8281 2020-02-02 00:00:00.000000 pyhf-0.7.1/src/pyhf/infer/mle.py
--rw-r--r--   0        0        0    20903 2020-02-02 00:00:00.000000 pyhf-0.7.1/src/pyhf/infer/test_statistics.py
--rw-r--r--   0        0        0     3336 2020-02-02 00:00:00.000000 pyhf-0.7.1/src/pyhf/infer/utils.py
--rw-r--r--   0        0        0      822 2020-02-02 00:00:00.000000 pyhf-0.7.1/src/pyhf/infer/intervals/__init__.py
--rw-r--r--   0        0        0     9724 2020-02-02 00:00:00.000000 pyhf-0.7.1/src/pyhf/infer/intervals/upper_limits.py
--rw-r--r--   0        0        0     1644 2020-02-02 00:00:00.000000 pyhf-0.7.1/src/pyhf/interpolators/__init__.py
--rw-r--r--   0        0        0     3822 2020-02-02 00:00:00.000000 pyhf-0.7.1/src/pyhf/interpolators/code0.py
--rw-r--r--   0        0        0     4473 2020-02-02 00:00:00.000000 pyhf-0.7.1/src/pyhf/interpolators/code1.py
--rw-r--r--   0        0        0     5324 2020-02-02 00:00:00.000000 pyhf-0.7.1/src/pyhf/interpolators/code2.py
--rw-r--r--   0        0        0    15982 2020-02-02 00:00:00.000000 pyhf-0.7.1/src/pyhf/interpolators/code4.py
--rw-r--r--   0        0        0     4929 2020-02-02 00:00:00.000000 pyhf-0.7.1/src/pyhf/interpolators/code4p.py
--rw-r--r--   0        0        0     1451 2020-02-02 00:00:00.000000 pyhf-0.7.1/src/pyhf/modifiers/__init__.py
--rw-r--r--   0        0        0     6369 2020-02-02 00:00:00.000000 pyhf-0.7.1/src/pyhf/modifiers/histosys.py
--rw-r--r--   0        0        0     3351 2020-02-02 00:00:00.000000 pyhf-0.7.1/src/pyhf/modifiers/lumi.py
--rw-r--r--   0        0        0     3616 2020-02-02 00:00:00.000000 pyhf-0.7.1/src/pyhf/modifiers/normfactor.py
--rw-r--r--   0        0        0     4736 2020-02-02 00:00:00.000000 pyhf-0.7.1/src/pyhf/modifiers/normsys.py
--rw-r--r--   0        0        0     7719 2020-02-02 00:00:00.000000 pyhf-0.7.1/src/pyhf/modifiers/shapefactor.py
--rw-r--r--   0        0        0     7746 2020-02-02 00:00:00.000000 pyhf-0.7.1/src/pyhf/modifiers/shapesys.py
--rw-r--r--   0        0        0     8780 2020-02-02 00:00:00.000000 pyhf-0.7.1/src/pyhf/modifiers/staterror.py
--rw-r--r--   0        0        0     1493 2020-02-02 00:00:00.000000 pyhf-0.7.1/src/pyhf/optimize/__init__.py
--rw-r--r--   0        0        0     5557 2020-02-02 00:00:00.000000 pyhf-0.7.1/src/pyhf/optimize/common.py
--rw-r--r--   0        0        0     7629 2020-02-02 00:00:00.000000 pyhf-0.7.1/src/pyhf/optimize/mixins.py
--rw-r--r--   0        0        0     2493 2020-02-02 00:00:00.000000 pyhf-0.7.1/src/pyhf/optimize/opt_jax.py
--rw-r--r--   0        0        0     5338 2020-02-02 00:00:00.000000 pyhf-0.7.1/src/pyhf/optimize/opt_minuit.py
--rw-r--r--   0        0        0     1051 2020-02-02 00:00:00.000000 pyhf-0.7.1/src/pyhf/optimize/opt_numpy.py
--rw-r--r--   0        0        0     1353 2020-02-02 00:00:00.000000 pyhf-0.7.1/src/pyhf/optimize/opt_pytorch.py
--rw-r--r--   0        0        0     3434 2020-02-02 00:00:00.000000 pyhf-0.7.1/src/pyhf/optimize/opt_scipy.py
--rw-r--r--   0        0        0     1583 2020-02-02 00:00:00.000000 pyhf-0.7.1/src/pyhf/optimize/opt_tflow.py
--rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 pyhf-0.7.1/src/pyhf/parameters/__init__.py
--rw-r--r--   0        0        0     2855 2020-02-02 00:00:00.000000 pyhf-0.7.1/src/pyhf/parameters/paramsets.py
--rw-r--r--   0        0        0     3163 2020-02-02 00:00:00.000000 pyhf-0.7.1/src/pyhf/parameters/paramview.py
--rw-r--r--   0        0        0     2820 2020-02-02 00:00:00.000000 pyhf-0.7.1/src/pyhf/parameters/utils.py
--rw-r--r--   0        0        0     2858 2020-02-02 00:00:00.000000 pyhf-0.7.1/src/pyhf/schema/__init__.py
--rw-r--r--   0        0        0     2030 2020-02-02 00:00:00.000000 pyhf-0.7.1/src/pyhf/schema/loader.py
--rw-r--r--   0        0        0     3198 2020-02-02 00:00:00.000000 pyhf-0.7.1/src/pyhf/schema/validator.py
--rw-r--r--   0        0        0      418 2020-02-02 00:00:00.000000 pyhf-0.7.1/src/pyhf/schema/variables.py
--rw-r--r--   0        0        0     6521 2020-02-02 00:00:00.000000 pyhf-0.7.1/src/pyhf/schemas/HistFactorySchema.dtd
--rw-r--r--   0        0        0    13069 2020-02-02 00:00:00.000000 pyhf-0.7.1/src/pyhf/schemas/1.0.0/defs.json
--rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 pyhf-0.7.1/src/pyhf/schemas/1.0.0/jsonpatch.json
--rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 pyhf-0.7.1/src/pyhf/schemas/1.0.0/measurement.json
--rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 pyhf-0.7.1/src/pyhf/schemas/1.0.0/model.json
--rw-r--r--   0        0        0      178 2020-02-02 00:00:00.000000 pyhf-0.7.1/src/pyhf/schemas/1.0.0/patchset.json
--rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 pyhf-0.7.1/src/pyhf/schemas/1.0.0/workspace.json
--rw-r--r--   0        0        0     3026 2020-02-02 00:00:00.000000 pyhf-0.7.1/src/pyhf/tensor/__init__.py
--rw-r--r--   0        0        0     3367 2020-02-02 00:00:00.000000 pyhf-0.7.1/src/pyhf/tensor/common.py
--rw-r--r--   0        0        0    20814 2020-02-02 00:00:00.000000 pyhf-0.7.1/src/pyhf/tensor/jax_backend.py
--rw-r--r--   0        0        0     7196 2020-02-02 00:00:00.000000 pyhf-0.7.1/src/pyhf/tensor/manager.py
--rw-r--r--   0        0        0    22865 2020-02-02 00:00:00.000000 pyhf-0.7.1/src/pyhf/tensor/numpy_backend.py
--rw-r--r--   0        0        0    21273 2020-02-02 00:00:00.000000 pyhf-0.7.1/src/pyhf/tensor/pytorch_backend.py
--rw-r--r--   0        0        0    25582 2020-02-02 00:00:00.000000 pyhf-0.7.1/src/pyhf/tensor/tensorflow_backend.py
--rw-r--r--   0        0        0      409 2020-02-02 00:00:00.000000 pyhf-0.7.1/.gitignore
--rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 pyhf-0.7.1/AUTHORS
--rw-r--r--   0        0        0    10760 2020-02-02 00:00:00.000000 pyhf-0.7.1/LICENSE
--rw-r--r--   0        0        0    13916 2020-02-02 00:00:00.000000 pyhf-0.7.1/README.rst
--rw-r--r--   0        0        0     8489 2020-02-02 00:00:00.000000 pyhf-0.7.1/pyproject.toml
--rw-r--r--   0        0        0    18519 2020-02-02 00:00:00.000000 pyhf-0.7.1/PKG-INFO
+-rw-r--r--   0        0        0     2526 2020-02-02 00:00:00.000000 pyhf-0.7.2/CITATION.cff
+-rw-r--r--   0        0        0     1164 2020-02-02 00:00:00.000000 pyhf-0.7.2/src/pyhf/__init__.py
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 pyhf-0.7.2/src/pyhf/_version.py
+-rw-r--r--   0        0        0     4036 2020-02-02 00:00:00.000000 pyhf-0.7.2/src/pyhf/compat.py
+-rw-r--r--   0        0        0     9892 2020-02-02 00:00:00.000000 pyhf-0.7.2/src/pyhf/constraints.py
+-rw-r--r--   0        0        0     4751 2020-02-02 00:00:00.000000 pyhf-0.7.2/src/pyhf/events.py
+-rw-r--r--   0        0        0     2992 2020-02-02 00:00:00.000000 pyhf-0.7.2/src/pyhf/mixins.py
+-rw-r--r--   0        0        0    11335 2020-02-02 00:00:00.000000 pyhf-0.7.2/src/pyhf/patchset.py
+-rw-r--r--   0        0        0    32407 2020-02-02 00:00:00.000000 pyhf-0.7.2/src/pyhf/pdf.py
+-rw-r--r--   0        0        0     9529 2020-02-02 00:00:00.000000 pyhf-0.7.2/src/pyhf/probability.py
+-rw-r--r--   0        0        0    17487 2020-02-02 00:00:00.000000 pyhf-0.7.2/src/pyhf/readxml.py
+-rw-r--r--   0        0        0     5684 2020-02-02 00:00:00.000000 pyhf-0.7.2/src/pyhf/simplemodels.py
+-rw-r--r--   0        0        0     2893 2020-02-02 00:00:00.000000 pyhf-0.7.2/src/pyhf/typing.py
+-rw-r--r--   0        0        0     4425 2020-02-02 00:00:00.000000 pyhf-0.7.2/src/pyhf/utils.py
+-rw-r--r--   0        0        0    34829 2020-02-02 00:00:00.000000 pyhf-0.7.2/src/pyhf/workspace.py
+-rw-r--r--   0        0        0    10923 2020-02-02 00:00:00.000000 pyhf-0.7.2/src/pyhf/writexml.py
+-rw-r--r--   0        0        0      387 2020-02-02 00:00:00.000000 pyhf-0.7.2/src/pyhf/cli/__init__.py
+-rw-r--r--   0        0        0     1299 2020-02-02 00:00:00.000000 pyhf-0.7.2/src/pyhf/cli/cli.py
+-rw-r--r--   0        0        0      983 2020-02-02 00:00:00.000000 pyhf-0.7.2/src/pyhf/cli/complete.py
+-rw-r--r--   0        0        0     7049 2020-02-02 00:00:00.000000 pyhf-0.7.2/src/pyhf/cli/infer.py
+-rw-r--r--   0        0        0     4461 2020-02-02 00:00:00.000000 pyhf-0.7.2/src/pyhf/cli/patchset.py
+-rw-r--r--   0        0        0     3819 2020-02-02 00:00:00.000000 pyhf-0.7.2/src/pyhf/cli/rootio.py
+-rw-r--r--   0        0        0    12719 2020-02-02 00:00:00.000000 pyhf-0.7.2/src/pyhf/cli/spec.py
+-rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 pyhf-0.7.2/src/pyhf/contrib/__init__.py
+-rw-r--r--   0        0        0     2055 2020-02-02 00:00:00.000000 pyhf-0.7.2/src/pyhf/contrib/cli.py
+-rw-r--r--   0        0        0     6315 2020-02-02 00:00:00.000000 pyhf-0.7.2/src/pyhf/contrib/utils.py
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 pyhf-0.7.2/src/pyhf/contrib/viz/__init__.py
+-rw-r--r--   0        0        0    13476 2020-02-02 00:00:00.000000 pyhf-0.7.2/src/pyhf/contrib/viz/brazil.py
+-rw-r--r--   0        0        0      699 2020-02-02 00:00:00.000000 pyhf-0.7.2/src/pyhf/data/citation.bib
+-rw-r--r--   0        0        0     5483 2020-02-02 00:00:00.000000 pyhf-0.7.2/src/pyhf/exceptions/__init__.py
+-rw-r--r--   0        0        0     8939 2020-02-02 00:00:00.000000 pyhf-0.7.2/src/pyhf/infer/__init__.py
+-rw-r--r--   0        0        0    38704 2020-02-02 00:00:00.000000 pyhf-0.7.2/src/pyhf/infer/calculators.py
+-rw-r--r--   0        0        0     8281 2020-02-02 00:00:00.000000 pyhf-0.7.2/src/pyhf/infer/mle.py
+-rw-r--r--   0        0        0    20903 2020-02-02 00:00:00.000000 pyhf-0.7.2/src/pyhf/infer/test_statistics.py
+-rw-r--r--   0        0        0     3336 2020-02-02 00:00:00.000000 pyhf-0.7.2/src/pyhf/infer/utils.py
+-rw-r--r--   0        0        0      822 2020-02-02 00:00:00.000000 pyhf-0.7.2/src/pyhf/infer/intervals/__init__.py
+-rw-r--r--   0        0        0     9724 2020-02-02 00:00:00.000000 pyhf-0.7.2/src/pyhf/infer/intervals/upper_limits.py
+-rw-r--r--   0        0        0     1644 2020-02-02 00:00:00.000000 pyhf-0.7.2/src/pyhf/interpolators/__init__.py
+-rw-r--r--   0        0        0     3822 2020-02-02 00:00:00.000000 pyhf-0.7.2/src/pyhf/interpolators/code0.py
+-rw-r--r--   0        0        0     4473 2020-02-02 00:00:00.000000 pyhf-0.7.2/src/pyhf/interpolators/code1.py
+-rw-r--r--   0        0        0     5324 2020-02-02 00:00:00.000000 pyhf-0.7.2/src/pyhf/interpolators/code2.py
+-rw-r--r--   0        0        0    15982 2020-02-02 00:00:00.000000 pyhf-0.7.2/src/pyhf/interpolators/code4.py
+-rw-r--r--   0        0        0     4929 2020-02-02 00:00:00.000000 pyhf-0.7.2/src/pyhf/interpolators/code4p.py
+-rw-r--r--   0        0        0     1451 2020-02-02 00:00:00.000000 pyhf-0.7.2/src/pyhf/modifiers/__init__.py
+-rw-r--r--   0        0        0     6369 2020-02-02 00:00:00.000000 pyhf-0.7.2/src/pyhf/modifiers/histosys.py
+-rw-r--r--   0        0        0     3351 2020-02-02 00:00:00.000000 pyhf-0.7.2/src/pyhf/modifiers/lumi.py
+-rw-r--r--   0        0        0     3616 2020-02-02 00:00:00.000000 pyhf-0.7.2/src/pyhf/modifiers/normfactor.py
+-rw-r--r--   0        0        0     4736 2020-02-02 00:00:00.000000 pyhf-0.7.2/src/pyhf/modifiers/normsys.py
+-rw-r--r--   0        0        0     7719 2020-02-02 00:00:00.000000 pyhf-0.7.2/src/pyhf/modifiers/shapefactor.py
+-rw-r--r--   0        0        0     7746 2020-02-02 00:00:00.000000 pyhf-0.7.2/src/pyhf/modifiers/shapesys.py
+-rw-r--r--   0        0        0     8780 2020-02-02 00:00:00.000000 pyhf-0.7.2/src/pyhf/modifiers/staterror.py
+-rw-r--r--   0        0        0     1493 2020-02-02 00:00:00.000000 pyhf-0.7.2/src/pyhf/optimize/__init__.py
+-rw-r--r--   0        0        0     5557 2020-02-02 00:00:00.000000 pyhf-0.7.2/src/pyhf/optimize/common.py
+-rw-r--r--   0        0        0     7629 2020-02-02 00:00:00.000000 pyhf-0.7.2/src/pyhf/optimize/mixins.py
+-rw-r--r--   0        0        0     2493 2020-02-02 00:00:00.000000 pyhf-0.7.2/src/pyhf/optimize/opt_jax.py
+-rw-r--r--   0        0        0     5338 2020-02-02 00:00:00.000000 pyhf-0.7.2/src/pyhf/optimize/opt_minuit.py
+-rw-r--r--   0        0        0     1051 2020-02-02 00:00:00.000000 pyhf-0.7.2/src/pyhf/optimize/opt_numpy.py
+-rw-r--r--   0        0        0     1353 2020-02-02 00:00:00.000000 pyhf-0.7.2/src/pyhf/optimize/opt_pytorch.py
+-rw-r--r--   0        0        0     3434 2020-02-02 00:00:00.000000 pyhf-0.7.2/src/pyhf/optimize/opt_scipy.py
+-rw-r--r--   0        0        0     1583 2020-02-02 00:00:00.000000 pyhf-0.7.2/src/pyhf/optimize/opt_tflow.py
+-rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 pyhf-0.7.2/src/pyhf/parameters/__init__.py
+-rw-r--r--   0        0        0     2855 2020-02-02 00:00:00.000000 pyhf-0.7.2/src/pyhf/parameters/paramsets.py
+-rw-r--r--   0        0        0     3163 2020-02-02 00:00:00.000000 pyhf-0.7.2/src/pyhf/parameters/paramview.py
+-rw-r--r--   0        0        0     2820 2020-02-02 00:00:00.000000 pyhf-0.7.2/src/pyhf/parameters/utils.py
+-rw-r--r--   0        0        0     2858 2020-02-02 00:00:00.000000 pyhf-0.7.2/src/pyhf/schema/__init__.py
+-rw-r--r--   0        0        0     2030 2020-02-02 00:00:00.000000 pyhf-0.7.2/src/pyhf/schema/loader.py
+-rw-r--r--   0        0        0     3198 2020-02-02 00:00:00.000000 pyhf-0.7.2/src/pyhf/schema/validator.py
+-rw-r--r--   0        0        0      418 2020-02-02 00:00:00.000000 pyhf-0.7.2/src/pyhf/schema/variables.py
+-rw-r--r--   0        0        0     6521 2020-02-02 00:00:00.000000 pyhf-0.7.2/src/pyhf/schemas/HistFactorySchema.dtd
+-rw-r--r--   0        0        0    13069 2020-02-02 00:00:00.000000 pyhf-0.7.2/src/pyhf/schemas/1.0.0/defs.json
+-rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 pyhf-0.7.2/src/pyhf/schemas/1.0.0/jsonpatch.json
+-rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 pyhf-0.7.2/src/pyhf/schemas/1.0.0/measurement.json
+-rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 pyhf-0.7.2/src/pyhf/schemas/1.0.0/model.json
+-rw-r--r--   0        0        0      178 2020-02-02 00:00:00.000000 pyhf-0.7.2/src/pyhf/schemas/1.0.0/patchset.json
+-rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 pyhf-0.7.2/src/pyhf/schemas/1.0.0/workspace.json
+-rw-r--r--   0        0        0     3026 2020-02-02 00:00:00.000000 pyhf-0.7.2/src/pyhf/tensor/__init__.py
+-rw-r--r--   0        0        0     3367 2020-02-02 00:00:00.000000 pyhf-0.7.2/src/pyhf/tensor/common.py
+-rw-r--r--   0        0        0    20814 2020-02-02 00:00:00.000000 pyhf-0.7.2/src/pyhf/tensor/jax_backend.py
+-rw-r--r--   0        0        0     7196 2020-02-02 00:00:00.000000 pyhf-0.7.2/src/pyhf/tensor/manager.py
+-rw-r--r--   0        0        0    22991 2020-02-02 00:00:00.000000 pyhf-0.7.2/src/pyhf/tensor/numpy_backend.py
+-rw-r--r--   0        0        0    21273 2020-02-02 00:00:00.000000 pyhf-0.7.2/src/pyhf/tensor/pytorch_backend.py
+-rw-r--r--   0        0        0    25582 2020-02-02 00:00:00.000000 pyhf-0.7.2/src/pyhf/tensor/tensorflow_backend.py
+-rw-r--r--   0        0        0      409 2020-02-02 00:00:00.000000 pyhf-0.7.2/.gitignore
+-rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 pyhf-0.7.2/AUTHORS
+-rw-r--r--   0        0        0    10760 2020-02-02 00:00:00.000000 pyhf-0.7.2/LICENSE
+-rw-r--r--   0        0        0    14286 2020-02-02 00:00:00.000000 pyhf-0.7.2/README.rst
+-rw-r--r--   0        0        0     8580 2020-02-02 00:00:00.000000 pyhf-0.7.2/pyproject.toml
+-rw-r--r--   0        0        0    19020 2020-02-02 00:00:00.000000 pyhf-0.7.2/PKG-INFO
```

### Comparing `pyhf-0.7.1/CITATION.cff` & `pyhf-0.7.2/CITATION.cff`

 * *Files 6% similar despite different names*

```diff
@@ -10,19 +10,19 @@
   given-names: "Matthew"
   orcid: "https://orcid.org/0000-0003-4124-7862"
   affiliation: "University of Wisconsin-Madison"
 - family-names: "Stark"
   given-names: "Giordon"
   orcid: "https://orcid.org/0000-0001-6616-3433"
   affiliation: "SCIPP, University of California, Santa Cruz"
-title: "pyhf: v0.7.1"
-version: 0.7.1
+title: "pyhf: v0.7.2"
+version: 0.7.2
 doi: 10.5281/zenodo.1169739
-repository-code: "https://github.com/scikit-hep/pyhf/releases/tag/v0.7.1"
-url: "https://pyhf.readthedocs.io/en/v0.7.1/"
+repository-code: "https://github.com/scikit-hep/pyhf/releases/tag/v0.7.2"
+url: "https://pyhf.readthedocs.io/en/v0.7.2/"
 keywords:
   - python
   - physics
   - statistics
   - fitting
   - scipy
   - numpy
```

### Comparing `pyhf-0.7.1/src/pyhf/__init__.py` & `pyhf-0.7.2/src/pyhf/__init__.py`

 * *Files identical despite different names*

### Comparing `pyhf-0.7.1/src/pyhf/compat.py` & `pyhf-0.7.2/src/pyhf/compat.py`

 * *Files identical despite different names*

### Comparing `pyhf-0.7.1/src/pyhf/constraints.py` & `pyhf-0.7.2/src/pyhf/constraints.py`

 * *Files identical despite different names*

### Comparing `pyhf-0.7.1/src/pyhf/events.py` & `pyhf-0.7.2/src/pyhf/events.py`

 * *Files identical despite different names*

### Comparing `pyhf-0.7.1/src/pyhf/mixins.py` & `pyhf-0.7.2/src/pyhf/mixins.py`

 * *Files identical despite different names*

### Comparing `pyhf-0.7.1/src/pyhf/patchset.py` & `pyhf-0.7.2/src/pyhf/patchset.py`

 * *Files identical despite different names*

### Comparing `pyhf-0.7.1/src/pyhf/pdf.py` & `pyhf-0.7.2/src/pyhf/pdf.py`

 * *Files 1% similar despite different names*

```diff
@@ -460,18 +460,21 @@
             self._poi_index = None
             return
 
         if name not in self.parameters:
             raise exceptions.InvalidModel(
                 f"The parameter of interest '{name:s}' cannot be fit as it is not declared in the model specification."
             )
-        s = self.par_slice(name)
-        assert s.stop - s.start == 1
+        if self.param_set(name).n_parameters > 1:
+            # multi-parameter modifiers are not supported as POIs
+            raise exceptions.InvalidModel(
+                f"The parameter '{name:s}' contains multiple components and is not currently supported as parameter of interest."
+            )
         self._poi_name = name
-        self._poi_index = s.start
+        self._poi_index = self.par_slice(name).start
 
     def _create_and_register_paramsets(self, required_paramsets):
         next_index = 0
         for param_name, paramset in required_paramsets.items():
             log.info(
                 'adding modifier %s (%s new nuisance parameters)',
                 param_name,
```

### Comparing `pyhf-0.7.1/src/pyhf/probability.py` & `pyhf-0.7.2/src/pyhf/probability.py`

 * *Files identical despite different names*

### Comparing `pyhf-0.7.1/src/pyhf/readxml.py` & `pyhf-0.7.2/src/pyhf/readxml.py`

 * *Files identical despite different names*

### Comparing `pyhf-0.7.1/src/pyhf/simplemodels.py` & `pyhf-0.7.2/src/pyhf/simplemodels.py`

 * *Files identical despite different names*

### Comparing `pyhf-0.7.1/src/pyhf/typing.py` & `pyhf-0.7.2/src/pyhf/typing.py`

 * *Files identical despite different names*

### Comparing `pyhf-0.7.1/src/pyhf/utils.py` & `pyhf-0.7.2/src/pyhf/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -107,15 +107,15 @@
     """
     Get the bibtex citation for pyhf
 
     Example:
 
         >>> import pyhf
         >>> pyhf.utils.citation(oneline=True)
-        '@software{pyhf,  author = {Lukas Heinrich and Matthew Feickert and Giordon Stark},  title = "{pyhf: v0.7.1}",  version = {0.7.1},  doi = {10.5281/zenodo.1169739},  url = {https://doi.org/10.5281/zenodo.1169739},  note = {https://github.com/scikit-hep/pyhf/releases/tag/v0.7.1}}@article{pyhf_joss,  doi = {10.21105/joss.02823},  url = {https://doi.org/10.21105/joss.02823},  year = {2021},  publisher = {The Open Journal},  volume = {6},  number = {58},  pages = {2823},  author = {Lukas Heinrich and Matthew Feickert and Giordon Stark and Kyle Cranmer},  title = {pyhf: pure-Python implementation of HistFactory statistical models},  journal = {Journal of Open Source Software}}'
+        '@software{pyhf,  author = {Lukas Heinrich and Matthew Feickert and Giordon Stark},  title = "{pyhf: v0.7.2}",  version = {0.7.2},  doi = {10.5281/zenodo.1169739},  url = {https://doi.org/10.5281/zenodo.1169739},  note = {https://github.com/scikit-hep/pyhf/releases/tag/v0.7.2}}@article{pyhf_joss,  doi = {10.21105/joss.02823},  url = {https://doi.org/10.21105/joss.02823},  year = {2021},  publisher = {The Open Journal},  volume = {6},  number = {58},  pages = {2823},  author = {Lukas Heinrich and Matthew Feickert and Giordon Stark and Kyle Cranmer},  title = {pyhf: pure-Python implementation of HistFactory statistical models},  journal = {Journal of Open Source Software}}'
 
     Keyword Args:
         oneline (:obj:`bool`): Whether to provide citation with new lines (default) or as a one-liner.
 
     Returns:
         citation (:obj:`str`): The citation for this software
     """
```

### Comparing `pyhf-0.7.1/src/pyhf/workspace.py` & `pyhf-0.7.2/src/pyhf/workspace.py`

 * *Files identical despite different names*

### Comparing `pyhf-0.7.1/src/pyhf/writexml.py` & `pyhf-0.7.2/src/pyhf/writexml.py`

 * *Files identical despite different names*

### Comparing `pyhf-0.7.1/src/pyhf/cli/cli.py` & `pyhf-0.7.2/src/pyhf/cli/cli.py`

 * *Files identical despite different names*

### Comparing `pyhf-0.7.1/src/pyhf/cli/infer.py` & `pyhf-0.7.2/src/pyhf/cli/infer.py`

 * *Files identical despite different names*

### Comparing `pyhf-0.7.1/src/pyhf/cli/patchset.py` & `pyhf-0.7.2/src/pyhf/cli/patchset.py`

 * *Files identical despite different names*

### Comparing `pyhf-0.7.1/src/pyhf/cli/rootio.py` & `pyhf-0.7.2/src/pyhf/cli/rootio.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,15 +46,15 @@
     try:
         import uproot
 
         assert uproot
     except ImportError:
         log.error(
             "xml2json requires uproot, please install pyhf using the "
-            "xmlio extra: python -m pip install pyhf[xmlio]",
+            "xmlio extra: python -m pip install 'pyhf[xmlio]'",
             exc_info=True,
         )
     from pyhf import readxml
 
     spec = readxml.parse(
         entrypoint_xml,
         basedir,
@@ -82,15 +82,15 @@
     try:
         import uproot
 
         assert uproot
     except ImportError:
         log.error(
             "json2xml requires uproot, please install pyhf using the "
-            "xmlio extra: python -m pip install pyhf[xmlio]",
+            "xmlio extra: python -m pip install 'pyhf[xmlio]'",
             exc_info=True,
         )
     from pyhf import writexml
 
     os.makedirs(output_dir, exist_ok=True)
     with click.open_file(workspace, "r", encoding="utf-8") as specstream:
         spec = json.load(specstream)
```

### Comparing `pyhf-0.7.1/src/pyhf/cli/spec.py` & `pyhf-0.7.2/src/pyhf/cli/spec.py`

 * *Files identical despite different names*

### Comparing `pyhf-0.7.1/src/pyhf/contrib/cli.py` & `pyhf-0.7.2/src/pyhf/contrib/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
     .. note::
 
         Requires installation of the ``contrib`` extra.
 
         .. code-block:: shell
 
-            $ python -m pip install pyhf[contrib]
+            $ python -m pip install 'pyhf[contrib]'
     """
     from pyhf.contrib import utils  # Guard CLI from missing extra # noqa: F401
 
 
 @cli.command()
 @click.argument("archive-url")
 @click.argument("output-directory")
@@ -68,10 +68,10 @@
 
         if verbose:
             file_list = [str(file) for file in list(Path(output_directory).glob("*"))]
             print("\n".join(file_list))
     except AttributeError:
         log.error(
             "\nInstallation of the contrib extra is required to use the contrib CLI API"
-            + "\nPlease install with: python -m pip install pyhf[contrib]\n",
+            + "\nPlease install with: python -m pip install 'pyhf[contrib]'\n",
             exc_info=True,
         )
```

### Comparing `pyhf-0.7.1/src/pyhf/contrib/utils.py` & `pyhf-0.7.2/src/pyhf/contrib/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -124,10 +124,10 @@
                         # from creation time
                         rmtree(output_directory)
                         _tmp_path.replace(output_directory)
 
 except ModuleNotFoundError:
     log.error(
         "\nInstallation of the contrib extra is required to use pyhf.contrib.utils.download"
-        + "\nPlease install with: python -m pip install pyhf[contrib]\n",
+        + "\nPlease install with: python -m pip install 'pyhf[contrib]'\n",
         exc_info=True,
     )
```

### Comparing `pyhf-0.7.1/src/pyhf/contrib/viz/brazil.py` & `pyhf-0.7.2/src/pyhf/contrib/viz/brazil.py`

 * *Files identical despite different names*

### Comparing `pyhf-0.7.1/src/pyhf/data/citation.bib` & `pyhf-0.7.2/src/pyhf/data/citation.bib`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 @software{pyhf,
   author = {Lukas Heinrich and Matthew Feickert and Giordon Stark},
-  title = "{pyhf: v0.7.1}",
-  version = {0.7.1},
+  title = "{pyhf: v0.7.2}",
+  version = {0.7.2},
   doi = {10.5281/zenodo.1169739},
   url = {https://doi.org/10.5281/zenodo.1169739},
-  note = {https://github.com/scikit-hep/pyhf/releases/tag/v0.7.1}
+  note = {https://github.com/scikit-hep/pyhf/releases/tag/v0.7.2}
 }
 
 @article{pyhf_joss,
   doi = {10.21105/joss.02823},
   url = {https://doi.org/10.21105/joss.02823},
   year = {2021},
   publisher = {The Open Journal},
```

### Comparing `pyhf-0.7.1/src/pyhf/exceptions/__init__.py` & `pyhf-0.7.2/src/pyhf/exceptions/__init__.py`

 * *Files identical despite different names*

### Comparing `pyhf-0.7.1/src/pyhf/infer/__init__.py` & `pyhf-0.7.2/src/pyhf/infer/__init__.py`

 * *Files identical despite different names*

### Comparing `pyhf-0.7.1/src/pyhf/infer/calculators.py` & `pyhf-0.7.2/src/pyhf/infer/calculators.py`

 * *Files identical despite different names*

### Comparing `pyhf-0.7.1/src/pyhf/infer/mle.py` & `pyhf-0.7.2/src/pyhf/infer/mle.py`

 * *Files identical despite different names*

### Comparing `pyhf-0.7.1/src/pyhf/infer/test_statistics.py` & `pyhf-0.7.2/src/pyhf/infer/test_statistics.py`

 * *Files identical despite different names*

### Comparing `pyhf-0.7.1/src/pyhf/infer/utils.py` & `pyhf-0.7.2/src/pyhf/infer/utils.py`

 * *Files identical despite different names*

### Comparing `pyhf-0.7.1/src/pyhf/infer/intervals/__init__.py` & `pyhf-0.7.2/src/pyhf/infer/intervals/__init__.py`

 * *Files identical despite different names*

### Comparing `pyhf-0.7.1/src/pyhf/infer/intervals/upper_limits.py` & `pyhf-0.7.2/src/pyhf/infer/intervals/upper_limits.py`

 * *Files identical despite different names*

### Comparing `pyhf-0.7.1/src/pyhf/interpolators/__init__.py` & `pyhf-0.7.2/src/pyhf/interpolators/__init__.py`

 * *Files identical despite different names*

### Comparing `pyhf-0.7.1/src/pyhf/interpolators/code0.py` & `pyhf-0.7.2/src/pyhf/interpolators/code0.py`

 * *Files identical despite different names*

### Comparing `pyhf-0.7.1/src/pyhf/interpolators/code1.py` & `pyhf-0.7.2/src/pyhf/interpolators/code1.py`

 * *Files identical despite different names*

### Comparing `pyhf-0.7.1/src/pyhf/interpolators/code2.py` & `pyhf-0.7.2/src/pyhf/interpolators/code2.py`

 * *Files identical despite different names*

### Comparing `pyhf-0.7.1/src/pyhf/interpolators/code4.py` & `pyhf-0.7.2/src/pyhf/interpolators/code4.py`

 * *Files identical despite different names*

### Comparing `pyhf-0.7.1/src/pyhf/interpolators/code4p.py` & `pyhf-0.7.2/src/pyhf/interpolators/code4p.py`

 * *Files identical despite different names*

### Comparing `pyhf-0.7.1/src/pyhf/modifiers/__init__.py` & `pyhf-0.7.2/src/pyhf/modifiers/__init__.py`

 * *Files identical despite different names*

### Comparing `pyhf-0.7.1/src/pyhf/modifiers/histosys.py` & `pyhf-0.7.2/src/pyhf/modifiers/histosys.py`

 * *Files identical despite different names*

### Comparing `pyhf-0.7.1/src/pyhf/modifiers/lumi.py` & `pyhf-0.7.2/src/pyhf/modifiers/lumi.py`

 * *Files identical despite different names*

### Comparing `pyhf-0.7.1/src/pyhf/modifiers/normfactor.py` & `pyhf-0.7.2/src/pyhf/modifiers/normfactor.py`

 * *Files identical despite different names*

### Comparing `pyhf-0.7.1/src/pyhf/modifiers/normsys.py` & `pyhf-0.7.2/src/pyhf/modifiers/normsys.py`

 * *Files identical despite different names*

### Comparing `pyhf-0.7.1/src/pyhf/modifiers/shapefactor.py` & `pyhf-0.7.2/src/pyhf/modifiers/shapefactor.py`

 * *Files identical despite different names*

### Comparing `pyhf-0.7.1/src/pyhf/modifiers/shapesys.py` & `pyhf-0.7.2/src/pyhf/modifiers/shapesys.py`

 * *Files identical despite different names*

### Comparing `pyhf-0.7.1/src/pyhf/modifiers/staterror.py` & `pyhf-0.7.2/src/pyhf/modifiers/staterror.py`

 * *Files identical despite different names*

### Comparing `pyhf-0.7.1/src/pyhf/optimize/__init__.py` & `pyhf-0.7.2/src/pyhf/optimize/__init__.py`

 * *Files identical despite different names*

### Comparing `pyhf-0.7.1/src/pyhf/optimize/common.py` & `pyhf-0.7.2/src/pyhf/optimize/common.py`

 * *Files identical despite different names*

### Comparing `pyhf-0.7.1/src/pyhf/optimize/mixins.py` & `pyhf-0.7.2/src/pyhf/optimize/mixins.py`

 * *Files identical despite different names*

### Comparing `pyhf-0.7.1/src/pyhf/optimize/opt_jax.py` & `pyhf-0.7.2/src/pyhf/optimize/opt_jax.py`

 * *Files identical despite different names*

### Comparing `pyhf-0.7.1/src/pyhf/optimize/opt_minuit.py` & `pyhf-0.7.2/src/pyhf/optimize/opt_minuit.py`

 * *Files identical despite different names*

### Comparing `pyhf-0.7.1/src/pyhf/optimize/opt_numpy.py` & `pyhf-0.7.2/src/pyhf/optimize/opt_numpy.py`

 * *Files identical despite different names*

### Comparing `pyhf-0.7.1/src/pyhf/optimize/opt_pytorch.py` & `pyhf-0.7.2/src/pyhf/optimize/opt_pytorch.py`

 * *Files identical despite different names*

### Comparing `pyhf-0.7.1/src/pyhf/optimize/opt_scipy.py` & `pyhf-0.7.2/src/pyhf/optimize/opt_scipy.py`

 * *Files identical despite different names*

### Comparing `pyhf-0.7.1/src/pyhf/optimize/opt_tflow.py` & `pyhf-0.7.2/src/pyhf/optimize/opt_tflow.py`

 * *Files identical despite different names*

### Comparing `pyhf-0.7.1/src/pyhf/parameters/paramsets.py` & `pyhf-0.7.2/src/pyhf/parameters/paramsets.py`

 * *Files identical despite different names*

### Comparing `pyhf-0.7.1/src/pyhf/parameters/paramview.py` & `pyhf-0.7.2/src/pyhf/parameters/paramview.py`

 * *Files identical despite different names*

### Comparing `pyhf-0.7.1/src/pyhf/parameters/utils.py` & `pyhf-0.7.2/src/pyhf/parameters/utils.py`

 * *Files identical despite different names*

### Comparing `pyhf-0.7.1/src/pyhf/schema/__init__.py` & `pyhf-0.7.2/src/pyhf/schema/__init__.py`

 * *Files identical despite different names*

### Comparing `pyhf-0.7.1/src/pyhf/schema/loader.py` & `pyhf-0.7.2/src/pyhf/schema/loader.py`

 * *Files identical despite different names*

### Comparing `pyhf-0.7.1/src/pyhf/schema/validator.py` & `pyhf-0.7.2/src/pyhf/schema/validator.py`

 * *Files identical despite different names*

### Comparing `pyhf-0.7.1/src/pyhf/schemas/HistFactorySchema.dtd` & `pyhf-0.7.2/src/pyhf/schemas/HistFactorySchema.dtd`

 * *Files identical despite different names*

### Comparing `pyhf-0.7.1/src/pyhf/schemas/1.0.0/defs.json` & `pyhf-0.7.2/src/pyhf/schemas/1.0.0/defs.json`

 * *Files identical despite different names*

### Comparing `pyhf-0.7.1/src/pyhf/tensor/__init__.py` & `pyhf-0.7.2/src/pyhf/tensor/__init__.py`

 * *Files identical despite different names*

### Comparing `pyhf-0.7.1/src/pyhf/tensor/common.py` & `pyhf-0.7.2/src/pyhf/tensor/common.py`

 * *Files identical despite different names*

### Comparing `pyhf-0.7.1/src/pyhf/tensor/jax_backend.py` & `pyhf-0.7.2/src/pyhf/tensor/jax_backend.py`

 * *Files identical despite different names*

### Comparing `pyhf-0.7.1/src/pyhf/tensor/manager.py` & `pyhf-0.7.2/src/pyhf/tensor/manager.py`

 * *Files identical despite different names*

### Comparing `pyhf-0.7.1/src/pyhf/tensor/numpy_backend.py` & `pyhf-0.7.2/src/pyhf/tensor/numpy_backend.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,21 @@
 """NumPy Tensor Library Module."""
 from __future__ import annotations
 
 import logging
-from typing import Callable, Generic, Mapping, Sequence, TypeVar, Union
+from typing import TYPE_CHECKING, Callable, Generic, Mapping, Sequence, TypeVar, Union
 
 import numpy as np
-from numpy.typing import ArrayLike, DTypeLike, NBitBase, NDArray
+
+# Needed while numpy lower bound is older than v1.21.0
+if TYPE_CHECKING:
+    from numpy.typing import ArrayLike, DTypeLike, NBitBase, NDArray
+else:
+    NBitBase = "NBitBase"
+
 from scipy import special
 from scipy.special import gammaln, xlogy
 from scipy.stats import norm, poisson
 
 from pyhf.typing import Literal, Shape
 
 T = TypeVar("T", bound=NBitBase)
```

### Comparing `pyhf-0.7.1/src/pyhf/tensor/pytorch_backend.py` & `pyhf-0.7.2/src/pyhf/tensor/pytorch_backend.py`

 * *Files identical despite different names*

### Comparing `pyhf-0.7.1/src/pyhf/tensor/tensorflow_backend.py` & `pyhf-0.7.2/src/pyhf/tensor/tensorflow_backend.py`

 * *Files identical despite different names*

### Comparing `pyhf-0.7.1/LICENSE` & `pyhf-0.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyhf-0.7.1/README.rst` & `pyhf-0.7.2/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
    :alt: pyhf logo
    :width: 320
    :align: center
 
 pure-python fitting/limit-setting/interval estimation HistFactory-style
 =======================================================================
 
-|GitHub Project| |DOI| |JOSS DOI| |Scikit-HEP| |NSF Award Number|
+|GitHub Project| |DOI| |JOSS DOI| |Scikit-HEP| |NSF Award Number| |NumFOCUS Affiliated Project|
 
 |Docs from latest| |Docs from main| |Jupyter Book tutorial| |Binder|
 
 |PyPI version| |Conda-forge version| |Supported Python versions| |Docker Hub pyhf| |Docker Hub pyhf CUDA|
 
 |Code Coverage| |CodeFactor| |pre-commit.ci Status| |Code style: black|
 
@@ -305,19 +305,19 @@
 `Zenodo <https://zenodo.org/>`__ archive and the
 `JOSS <https://joss.theoj.org/>`__ paper:
 
 .. code:: bibtex
 
    @software{pyhf,
      author = {Lukas Heinrich and Matthew Feickert and Giordon Stark},
-     title = "{pyhf: v0.7.1}",
-     version = {0.7.1},
+     title = "{pyhf: v0.7.2}",
+     version = {0.7.2},
      doi = {10.5281/zenodo.1169739},
      url = {https://doi.org/10.5281/zenodo.1169739},
-     note = {https://github.com/scikit-hep/pyhf/releases/tag/v0.7.1}
+     note = {https://github.com/scikit-hep/pyhf/releases/tag/v0.7.2}
    }
 
    @article{pyhf_joss,
      doi = {10.21105/joss.02823},
      url = {https://doi.org/10.21105/joss.02823},
      year = {2021},
      publisher = {The Open Journal},
@@ -347,40 +347,44 @@
 Acknowledgements
 ----------------
 
 Matthew Feickert has received support to work on ``pyhf`` provided by NSF
 cooperative agreement `OAC-1836650 <https://www.nsf.gov/awardsearch/showAward?AWD_ID=1836650>`__ (IRIS-HEP)
 and grant `OAC-1450377 <https://www.nsf.gov/awardsearch/showAward?AWD_ID=1450377>`__ (DIANA/HEP).
 
+``pyhf`` is a `NumFOCUS Affiliated Project <https://numfocus.org/sponsored-projects/affiliated-projects>`__.
+
 .. |GitHub Project| image:: https://img.shields.io/badge/GitHub--blue?style=social&logo=GitHub
    :target: https://github.com/scikit-hep/pyhf
 .. |DOI| image:: https://zenodo.org/badge/DOI/10.5281/zenodo.1169739.svg
    :target: https://doi.org/10.5281/zenodo.1169739
 .. |JOSS DOI| image:: https://joss.theoj.org/papers/10.21105/joss.02823/status.svg
    :target: https://doi.org/10.21105/joss.02823
 .. |Scikit-HEP| image:: https://scikit-hep.org/assets/images/Scikit--HEP-Project-blue.svg
    :target: https://scikit-hep.org/
 .. |NSF Award Number| image:: https://img.shields.io/badge/NSF-1836650-blue.svg
    :target: https://nsf.gov/awardsearch/showAward?AWD_ID=1836650
-.. |Docs from latest| image:: https://img.shields.io/badge/docs-v0.7.1-blue.svg
+.. |NumFOCUS Affiliated Project| image:: https://img.shields.io/badge/NumFOCUS-Affiliated%20Project-orange.svg?style=flat&colorA=E1523D&colorB=007D8A
+   :target: https://numfocus.org/sponsored-projects/affiliated-projects
+.. |Docs from latest| image:: https://img.shields.io/badge/docs-v0.7.2-blue.svg
    :target: https://pyhf.readthedocs.io/
 .. |Docs from main| image:: https://img.shields.io/badge/docs-main-blue.svg
    :target: https://scikit-hep.github.io/pyhf
 .. |Jupyter Book tutorial| image:: https://jupyterbook.org/_images/badge.svg
    :target: https://pyhf.github.io/pyhf-tutorial/
 .. |Binder| image:: https://mybinder.org/badge_logo.svg
    :target: https://mybinder.org/v2/gh/scikit-hep/pyhf/main?filepath=docs%2Fexamples%2Fnotebooks%2Fbinderexample%2FStatisticalAnalysis.ipynb
 
 .. |PyPI version| image:: https://badge.fury.io/py/pyhf.svg
    :target: https://badge.fury.io/py/pyhf
 .. |Conda-forge version| image:: https://img.shields.io/conda/vn/conda-forge/pyhf.svg
-   :target: https://github.com/conda-forge/pyhf-feedstock
+   :target: https://prefix.dev/channels/conda-forge/packages/pyhf
 .. |Supported Python versions| image:: https://img.shields.io/pypi/pyversions/pyhf.svg
    :target: https://pypi.org/project/pyhf/
-.. |Docker Hub pyhf| image:: https://img.shields.io/badge/pyhf-v0.7.1-blue?logo=Docker
+.. |Docker Hub pyhf| image:: https://img.shields.io/badge/pyhf-v0.7.2-blue?logo=Docker
    :target: https://hub.docker.com/r/pyhf/pyhf/tags
 .. |Docker Hub pyhf CUDA| image:: https://img.shields.io/badge/pyhf-CUDA-blue?logo=Docker
    :target: https://hub.docker.com/r/pyhf/cuda/tags
 
 .. |Code Coverage| image:: https://codecov.io/gh/scikit-hep/pyhf/graph/badge.svg?branch=main
    :target: https://codecov.io/gh/scikit-hep/pyhf?branch=main
 .. |CodeFactor| image:: https://www.codefactor.io/repository/github/scikit-hep/pyhf/badge
```

### Comparing `pyhf-0.7.1/pyproject.toml` & `pyhf-0.7.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -67,15 +67,15 @@
 "Source Code" = "https://github.com/scikit-hep/pyhf"
 
 [project.optional-dependencies]
 shellcomplete = ["click_completion"]
 tensorflow = [
     "tensorflow>=2.7.0; platform_machine != 'arm64'",  # c.f. PR #1962
     "tensorflow-macos>=2.7.0; platform_machine == 'arm64' and platform_system == 'Darwin'",  # c.f. PR #2119
-    "tensorflow-probability>=0.11.0",  # c.f. PR #1657
+    "tensorflow-probability>=0.11.0,!=0.20.0",  # c.f. PR #1657, PR #2203
 ]
 torch = ["torch>=1.10.0"]  # c.f. PR #1657
 jax = [
     "jax>=0.2.10",  # c.f. PR #1962, Issue #1501
     "jaxlib>=0.1.61,!=0.1.68",  # c.f. PR #1962, Issue #1501
 ]
 xmlio = ["uproot>=4.1.1"]  # c.f. PR #1567
@@ -110,16 +110,18 @@
     "sphinx>=5.1.1",  # c.f. https://github.com/scikit-hep/pyhf/pull/1926
     "sphinxcontrib-bibtex~=2.1",
     "sphinx-click",
     "sphinx_rtd_theme",
     "nbsphinx!=0.8.8",  # c.f. https://github.com/spatialaudio/nbsphinx/issues/620
     "ipywidgets",
     "sphinx-issues",
-    "sphinx-copybutton>=0.3.2",
-    "sphinx-togglebutton>=0.3.0",
+    "sphinx-copybutton>=0.3.2,!=0.5.1",
+    "jupyterlite-sphinx>=0.8.0",
+    "jupyterlite-pyodide-kernel>=0.0.7",
+    "jupytext>=1.14.0",
     "ipython!=8.7.0",  # c.f. https://github.com/scikit-hep/pyhf/pull/2068
 ]
 develop = [
     "pyhf[test,docs]",
     "tbump>=6.7.0",
     "pre-commit",
     "nox",
```

### Comparing `pyhf-0.7.1/PKG-INFO` & `pyhf-0.7.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyhf
-Version: 0.7.1
+Version: 0.7.2
 Summary: pure-Python HistFactory implementation with tensors and autodiff
 Project-URL: Documentation, https://pyhf.readthedocs.io/
 Project-URL: Homepage, https://github.com/scikit-hep/pyhf
 Project-URL: Issue Tracker, https://github.com/scikit-hep/pyhf/issues
 Project-URL: Release Notes, https://pyhf.readthedocs.io/en/stable/release-notes.html
 Project-URL: Releases, https://github.com/scikit-hep/pyhf/releases
 Project-URL: Source Code, https://github.com/scikit-hep/pyhf
@@ -50,33 +50,35 @@
 Requires-Dist: nox; extra == 'develop'
 Requires-Dist: pre-commit; extra == 'develop'
 Requires-Dist: pyhf[docs,test]; extra == 'develop'
 Requires-Dist: tbump>=6.7.0; extra == 'develop'
 Provides-Extra: docs
 Requires-Dist: ipython!=8.7.0; extra == 'docs'
 Requires-Dist: ipywidgets; extra == 'docs'
+Requires-Dist: jupyterlite-pyodide-kernel>=0.0.7; extra == 'docs'
+Requires-Dist: jupyterlite-sphinx>=0.8.0; extra == 'docs'
+Requires-Dist: jupytext>=1.14.0; extra == 'docs'
 Requires-Dist: nbsphinx!=0.8.8; extra == 'docs'
 Requires-Dist: pyhf[contrib,xmlio]; extra == 'docs'
 Requires-Dist: sphinx-click; extra == 'docs'
-Requires-Dist: sphinx-copybutton>=0.3.2; extra == 'docs'
+Requires-Dist: sphinx-copybutton!=0.5.1,>=0.3.2; extra == 'docs'
 Requires-Dist: sphinx-issues; extra == 'docs'
 Requires-Dist: sphinx-rtd-theme; extra == 'docs'
-Requires-Dist: sphinx-togglebutton>=0.3.0; extra == 'docs'
 Requires-Dist: sphinx>=5.1.1; extra == 'docs'
 Requires-Dist: sphinxcontrib-bibtex~=2.1; extra == 'docs'
 Provides-Extra: jax
 Requires-Dist: jax>=0.2.10; extra == 'jax'
 Requires-Dist: jaxlib!=0.1.68,>=0.1.61; extra == 'jax'
 Provides-Extra: minuit
 Requires-Dist: iminuit>=2.7.0; extra == 'minuit'
 Provides-Extra: shellcomplete
 Requires-Dist: click-completion; extra == 'shellcomplete'
 Provides-Extra: tensorflow
 Requires-Dist: tensorflow-macos>=2.7.0; platform_machine == 'arm64' and platform_system == 'Darwin' and extra == 'tensorflow'
-Requires-Dist: tensorflow-probability>=0.11.0; extra == 'tensorflow'
+Requires-Dist: tensorflow-probability!=0.20.0,>=0.11.0; extra == 'tensorflow'
 Requires-Dist: tensorflow>=2.7.0; platform_machine != 'arm64' and extra == 'tensorflow'
 Provides-Extra: test
 Requires-Dist: graphviz; extra == 'test'
 Requires-Dist: jupyter; extra == 'test'
 Requires-Dist: papermill~=2.3.4; extra == 'test'
 Requires-Dist: pydocstyle; extra == 'test'
 Requires-Dist: pyhf[all]; extra == 'test'
@@ -100,15 +102,15 @@
    :alt: pyhf logo
    :width: 320
    :align: center
 
 pure-python fitting/limit-setting/interval estimation HistFactory-style
 =======================================================================
 
-|GitHub Project| |DOI| |JOSS DOI| |Scikit-HEP| |NSF Award Number|
+|GitHub Project| |DOI| |JOSS DOI| |Scikit-HEP| |NSF Award Number| |NumFOCUS Affiliated Project|
 
 |Docs from latest| |Docs from main| |Jupyter Book tutorial| |Binder|
 
 |PyPI version| |Conda-forge version| |Supported Python versions| |Docker Hub pyhf| |Docker Hub pyhf CUDA|
 
 |Code Coverage| |CodeFactor| |pre-commit.ci Status| |Code style: black|
 
@@ -403,19 +405,19 @@
 `Zenodo <https://zenodo.org/>`__ archive and the
 `JOSS <https://joss.theoj.org/>`__ paper:
 
 .. code:: bibtex
 
    @software{pyhf,
      author = {Lukas Heinrich and Matthew Feickert and Giordon Stark},
-     title = "{pyhf: v0.7.1}",
-     version = {0.7.1},
+     title = "{pyhf: v0.7.2}",
+     version = {0.7.2},
      doi = {10.5281/zenodo.1169739},
      url = {https://doi.org/10.5281/zenodo.1169739},
-     note = {https://github.com/scikit-hep/pyhf/releases/tag/v0.7.1}
+     note = {https://github.com/scikit-hep/pyhf/releases/tag/v0.7.2}
    }
 
    @article{pyhf_joss,
      doi = {10.21105/joss.02823},
      url = {https://doi.org/10.21105/joss.02823},
      year = {2021},
      publisher = {The Open Journal},
@@ -445,40 +447,44 @@
 Acknowledgements
 ----------------
 
 Matthew Feickert has received support to work on ``pyhf`` provided by NSF
 cooperative agreement `OAC-1836650 <https://www.nsf.gov/awardsearch/showAward?AWD_ID=1836650>`__ (IRIS-HEP)
 and grant `OAC-1450377 <https://www.nsf.gov/awardsearch/showAward?AWD_ID=1450377>`__ (DIANA/HEP).
 
+``pyhf`` is a `NumFOCUS Affiliated Project <https://numfocus.org/sponsored-projects/affiliated-projects>`__.
+
 .. |GitHub Project| image:: https://img.shields.io/badge/GitHub--blue?style=social&logo=GitHub
    :target: https://github.com/scikit-hep/pyhf
 .. |DOI| image:: https://zenodo.org/badge/DOI/10.5281/zenodo.1169739.svg
    :target: https://doi.org/10.5281/zenodo.1169739
 .. |JOSS DOI| image:: https://joss.theoj.org/papers/10.21105/joss.02823/status.svg
    :target: https://doi.org/10.21105/joss.02823
 .. |Scikit-HEP| image:: https://scikit-hep.org/assets/images/Scikit--HEP-Project-blue.svg
    :target: https://scikit-hep.org/
 .. |NSF Award Number| image:: https://img.shields.io/badge/NSF-1836650-blue.svg
    :target: https://nsf.gov/awardsearch/showAward?AWD_ID=1836650
-.. |Docs from latest| image:: https://img.shields.io/badge/docs-v0.7.1-blue.svg
+.. |NumFOCUS Affiliated Project| image:: https://img.shields.io/badge/NumFOCUS-Affiliated%20Project-orange.svg?style=flat&colorA=E1523D&colorB=007D8A
+   :target: https://numfocus.org/sponsored-projects/affiliated-projects
+.. |Docs from latest| image:: https://img.shields.io/badge/docs-v0.7.2-blue.svg
    :target: https://pyhf.readthedocs.io/
 .. |Docs from main| image:: https://img.shields.io/badge/docs-main-blue.svg
    :target: https://scikit-hep.github.io/pyhf
 .. |Jupyter Book tutorial| image:: https://jupyterbook.org/_images/badge.svg
    :target: https://pyhf.github.io/pyhf-tutorial/
 .. |Binder| image:: https://mybinder.org/badge_logo.svg
    :target: https://mybinder.org/v2/gh/scikit-hep/pyhf/main?filepath=docs%2Fexamples%2Fnotebooks%2Fbinderexample%2FStatisticalAnalysis.ipynb
 
 .. |PyPI version| image:: https://badge.fury.io/py/pyhf.svg
    :target: https://badge.fury.io/py/pyhf
 .. |Conda-forge version| image:: https://img.shields.io/conda/vn/conda-forge/pyhf.svg
-   :target: https://github.com/conda-forge/pyhf-feedstock
+   :target: https://prefix.dev/channels/conda-forge/packages/pyhf
 .. |Supported Python versions| image:: https://img.shields.io/pypi/pyversions/pyhf.svg
    :target: https://pypi.org/project/pyhf/
-.. |Docker Hub pyhf| image:: https://img.shields.io/badge/pyhf-v0.7.1-blue?logo=Docker
+.. |Docker Hub pyhf| image:: https://img.shields.io/badge/pyhf-v0.7.2-blue?logo=Docker
    :target: https://hub.docker.com/r/pyhf/pyhf/tags
 .. |Docker Hub pyhf CUDA| image:: https://img.shields.io/badge/pyhf-CUDA-blue?logo=Docker
    :target: https://hub.docker.com/r/pyhf/cuda/tags
 
 .. |Code Coverage| image:: https://codecov.io/gh/scikit-hep/pyhf/graph/badge.svg?branch=main
    :target: https://codecov.io/gh/scikit-hep/pyhf?branch=main
 .. |CodeFactor| image:: https://www.codefactor.io/repository/github/scikit-hep/pyhf/badge
```

