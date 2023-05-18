# Comparing `tmp/aemcmc-nightly-0.0.8.dev20230516.tar.gz` & `tmp/aemcmc-nightly-0.0.8.dev20230517.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aemcmc-nightly-0.0.8.dev20230516.tar", last modified: Tue May 16 00:59:07 2023, max compression
+gzip compressed data, was "aemcmc-nightly-0.0.8.dev20230517.tar", last modified: Wed May 17 01:00:33 2023, max compression
```

## Comparing `aemcmc-nightly-0.0.8.dev20230516.tar` & `aemcmc-nightly-0.0.8.dev20230517.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 00:59:07.489030 aemcmc-nightly-0.0.8.dev20230516/
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-05-16 00:58:52.000000 aemcmc-nightly-0.0.8.dev20230516/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-16 00:58:52.000000 aemcmc-nightly-0.0.8.dev20230516/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      980 2023-05-16 00:59:07.489030 aemcmc-nightly-0.0.8.dev20230516/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7042 2023-05-16 00:58:52.000000 aemcmc-nightly-0.0.8.dev20230516/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 00:59:07.489030 aemcmc-nightly-0.0.8.dev20230516/aemcmc/
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-05-16 00:58:52.000000 aemcmc-nightly-0.0.8.dev20230516/aemcmc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-05-16 00:59:07.489030 aemcmc-nightly-0.0.8.dev20230516/aemcmc/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     4304 2023-05-16 00:58:52.000000 aemcmc-nightly-0.0.8.dev20230516/aemcmc/basic.py
--rw-r--r--   0 runner    (1001) docker     (123)     8277 2023-05-16 00:58:52.000000 aemcmc-nightly-0.0.8.dev20230516/aemcmc/conjugates.py
--rw-r--r--   0 runner    (1001) docker     (123)     5496 2023-05-16 00:58:52.000000 aemcmc-nightly-0.0.8.dev20230516/aemcmc/dists.py
--rw-r--r--   0 runner    (1001) docker     (123)     4439 2023-05-16 00:58:52.000000 aemcmc-nightly-0.0.8.dev20230516/aemcmc/ffbs.py
--rw-r--r--   0 runner    (1001) docker     (123)    24238 2023-05-16 00:58:52.000000 aemcmc-nightly-0.0.8.dev20230516/aemcmc/gibbs.py
--rw-r--r--   0 runner    (1001) docker     (123)     7289 2023-05-16 00:58:52.000000 aemcmc-nightly-0.0.8.dev20230516/aemcmc/nuts.py
--rw-r--r--   0 runner    (1001) docker     (123)    13350 2023-05-16 00:58:52.000000 aemcmc-nightly-0.0.8.dev20230516/aemcmc/rewriting.py
--rw-r--r--   0 runner    (1001) docker     (123)      748 2023-05-16 00:58:52.000000 aemcmc-nightly-0.0.8.dev20230516/aemcmc/sample.py
--rw-r--r--   0 runner    (1001) docker     (123)     3427 2023-05-16 00:58:52.000000 aemcmc-nightly-0.0.8.dev20230516/aemcmc/transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)     1748 2023-05-16 00:58:52.000000 aemcmc-nightly-0.0.8.dev20230516/aemcmc/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     4668 2023-05-16 00:58:52.000000 aemcmc-nightly-0.0.8.dev20230516/aemcmc/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 00:59:07.485030 aemcmc-nightly-0.0.8.dev20230516/aemcmc_nightly.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      980 2023-05-16 00:59:07.000000 aemcmc-nightly-0.0.8.dev20230516/aemcmc_nightly.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      728 2023-05-16 00:59:07.000000 aemcmc-nightly-0.0.8.dev20230516/aemcmc_nightly.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 00:59:07.000000 aemcmc-nightly-0.0.8.dev20230516/aemcmc_nightly.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 00:59:07.000000 aemcmc-nightly-0.0.8.dev20230516/aemcmc_nightly.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-05-16 00:59:07.000000 aemcmc-nightly-0.0.8.dev20230516/aemcmc_nightly.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-16 00:59:07.000000 aemcmc-nightly-0.0.8.dev20230516/aemcmc_nightly.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-05-16 00:59:07.489030 aemcmc-nightly-0.0.8.dev20230516/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2126 2023-05-16 00:58:52.000000 aemcmc-nightly-0.0.8.dev20230516/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 00:59:07.489030 aemcmc-nightly-0.0.8.dev20230516/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     6907 2023-05-16 00:58:52.000000 aemcmc-nightly-0.0.8.dev20230516/tests/test_basic.py
--rw-r--r--   0 runner    (1001) docker     (123)     4878 2023-05-16 00:58:52.000000 aemcmc-nightly-0.0.8.dev20230516/tests/test_conjugates.py
--rw-r--r--   0 runner    (1001) docker     (123)     3725 2023-05-16 00:58:52.000000 aemcmc-nightly-0.0.8.dev20230516/tests/test_dists.py
--rw-r--r--   0 runner    (1001) docker     (123)     2653 2023-05-16 00:58:52.000000 aemcmc-nightly-0.0.8.dev20230516/tests/test_ffbs.py
--rw-r--r--   0 runner    (1001) docker     (123)    11323 2023-05-16 00:58:52.000000 aemcmc-nightly-0.0.8.dev20230516/tests/test_gibbs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-16 00:58:52.000000 aemcmc-nightly-0.0.8.dev20230516/tests/test_nuts.py
--rw-r--r--   0 runner    (1001) docker     (123)     4050 2023-05-16 00:58:52.000000 aemcmc-nightly-0.0.8.dev20230516/tests/test_rewriting.py
--rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-05-16 00:58:52.000000 aemcmc-nightly-0.0.8.dev20230516/tests/test_sample.py
--rw-r--r--   0 runner    (1001) docker     (123)     2723 2023-05-16 00:58:52.000000 aemcmc-nightly-0.0.8.dev20230516/tests/test_transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-05-16 00:58:52.000000 aemcmc-nightly-0.0.8.dev20230516/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    80044 2023-05-16 00:58:52.000000 aemcmc-nightly-0.0.8.dev20230516/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 01:00:33.423239 aemcmc-nightly-0.0.8.dev20230517/
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-05-17 01:00:22.000000 aemcmc-nightly-0.0.8.dev20230517/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-17 01:00:22.000000 aemcmc-nightly-0.0.8.dev20230517/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      980 2023-05-17 01:00:33.423239 aemcmc-nightly-0.0.8.dev20230517/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7042 2023-05-17 01:00:22.000000 aemcmc-nightly-0.0.8.dev20230517/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 01:00:33.423239 aemcmc-nightly-0.0.8.dev20230517/aemcmc/
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-05-17 01:00:22.000000 aemcmc-nightly-0.0.8.dev20230517/aemcmc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-05-17 01:00:33.423239 aemcmc-nightly-0.0.8.dev20230517/aemcmc/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4304 2023-05-17 01:00:22.000000 aemcmc-nightly-0.0.8.dev20230517/aemcmc/basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7268 2023-05-17 01:00:22.000000 aemcmc-nightly-0.0.8.dev20230517/aemcmc/conjugates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5496 2023-05-17 01:00:22.000000 aemcmc-nightly-0.0.8.dev20230517/aemcmc/dists.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4439 2023-05-17 01:00:22.000000 aemcmc-nightly-0.0.8.dev20230517/aemcmc/ffbs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24238 2023-05-17 01:00:22.000000 aemcmc-nightly-0.0.8.dev20230517/aemcmc/gibbs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7289 2023-05-17 01:00:22.000000 aemcmc-nightly-0.0.8.dev20230517/aemcmc/nuts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13350 2023-05-17 01:00:22.000000 aemcmc-nightly-0.0.8.dev20230517/aemcmc/rewriting.py
+-rw-r--r--   0 runner    (1001) docker     (123)      748 2023-05-17 01:00:22.000000 aemcmc-nightly-0.0.8.dev20230517/aemcmc/sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3427 2023-05-17 01:00:22.000000 aemcmc-nightly-0.0.8.dev20230517/aemcmc/transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1748 2023-05-17 01:00:22.000000 aemcmc-nightly-0.0.8.dev20230517/aemcmc/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4668 2023-05-17 01:00:22.000000 aemcmc-nightly-0.0.8.dev20230517/aemcmc/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 01:00:33.423239 aemcmc-nightly-0.0.8.dev20230517/aemcmc_nightly.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      980 2023-05-17 01:00:33.000000 aemcmc-nightly-0.0.8.dev20230517/aemcmc_nightly.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      728 2023-05-17 01:00:33.000000 aemcmc-nightly-0.0.8.dev20230517/aemcmc_nightly.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 01:00:33.000000 aemcmc-nightly-0.0.8.dev20230517/aemcmc_nightly.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 01:00:33.000000 aemcmc-nightly-0.0.8.dev20230517/aemcmc_nightly.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-05-17 01:00:33.000000 aemcmc-nightly-0.0.8.dev20230517/aemcmc_nightly.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-17 01:00:33.000000 aemcmc-nightly-0.0.8.dev20230517/aemcmc_nightly.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1463 2023-05-17 01:00:33.423239 aemcmc-nightly-0.0.8.dev20230517/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2126 2023-05-17 01:00:22.000000 aemcmc-nightly-0.0.8.dev20230517/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 01:00:33.423239 aemcmc-nightly-0.0.8.dev20230517/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     7415 2023-05-17 01:00:22.000000 aemcmc-nightly-0.0.8.dev20230517/tests/test_basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4665 2023-05-17 01:00:22.000000 aemcmc-nightly-0.0.8.dev20230517/tests/test_conjugates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3725 2023-05-17 01:00:22.000000 aemcmc-nightly-0.0.8.dev20230517/tests/test_dists.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2842 2023-05-17 01:00:22.000000 aemcmc-nightly-0.0.8.dev20230517/tests/test_ffbs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11323 2023-05-17 01:00:22.000000 aemcmc-nightly-0.0.8.dev20230517/tests/test_gibbs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-17 01:00:22.000000 aemcmc-nightly-0.0.8.dev20230517/tests/test_nuts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4050 2023-05-17 01:00:22.000000 aemcmc-nightly-0.0.8.dev20230517/tests/test_rewriting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-05-17 01:00:22.000000 aemcmc-nightly-0.0.8.dev20230517/tests/test_sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2723 2023-05-17 01:00:22.000000 aemcmc-nightly-0.0.8.dev20230517/tests/test_transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-05-17 01:00:22.000000 aemcmc-nightly-0.0.8.dev20230517/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    80044 2023-05-17 01:00:22.000000 aemcmc-nightly-0.0.8.dev20230517/versioneer.py
```

### Comparing `aemcmc-nightly-0.0.8.dev20230516/LICENSE` & `aemcmc-nightly-0.0.8.dev20230517/LICENSE`

 * *Files identical despite different names*

### Comparing `aemcmc-nightly-0.0.8.dev20230516/PKG-INFO` & `aemcmc-nightly-0.0.8.dev20230517/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aemcmc-nightly
-Version: 0.0.8.dev20230516
+Version: 0.0.8.dev20230517
 Summary: Miscellaneous MCMC samplers written in Aesara
 Home-page: http://github.com/aesara-devs/aemcmc
 Author: aesara-devs
 Author-email: aesara.devs@gmail.com
 Keywords: math,probability,numerical,symbolic,MCMC
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
```

### Comparing `aemcmc-nightly-0.0.8.dev20230516/README.md` & `aemcmc-nightly-0.0.8.dev20230517/README.md`

 * *Files identical despite different names*

### Comparing `aemcmc-nightly-0.0.8.dev20230516/aemcmc/basic.py` & `aemcmc-nightly-0.0.8.dev20230517/aemcmc/basic.py`

 * *Files identical despite different names*

### Comparing `aemcmc-nightly-0.0.8.dev20230516/aemcmc/conjugates.py` & `aemcmc-nightly-0.0.8.dev20230517/aemcmc/conjugates.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,37 +1,42 @@
+from functools import partial
+from typing import TYPE_CHECKING
+
 import aesara.tensor as at
-from aesara.graph.rewriting.basic import in2out, node_rewriter
+from aesara.graph.rewriting.basic import in2out
 from aesara.graph.rewriting.db import LocalGroupDB
 from aesara.graph.rewriting.unify import eval_if_etuple
 from aesara.tensor.random.basic import BinomialRV, NegBinomialRV, PoissonRV
 from etuples import etuple, etuplize
 from kanren import eq, lall, run
 from unification import var
 
-from aemcmc.rewriting import sampler_finder_db
+from aemcmc.rewriting import sampler_finder, sampler_finder_db
+
+if TYPE_CHECKING:
+    from aesara.tensor.random.utils import RandomStream
 
 
-def gamma_poisson_conjugateo(observed_val, observed_rv_expr, posterior_expr):
-    r"""Produce a goal that represents the application of Bayes theorem
-    for a beta prior with a binomial observation model.
+def gamma_poisson_conjugateo(srng: "RandomStream", observed_rv_expr, posterior_expr):
+    r"""Relation for the conjugate posterior of a gamma prior with a Poisson observation model.
 
     .. math::
 
         \frac{
             Y \sim \operatorname{Poisson}\left(\lambda\right), \quad
             \lambda \sim \operatorname{Gamma}\left(\alpha, \beta\right)
         }{
             \left(\lambda|Y=y\right) \sim \operatorname{Gamma}\left(\alpha+y, \beta+1\right)
         }
 
 
     Parameters
     ----------
-    observed_val
-        The observed value.
+    srng
+        The `RandomStream` used to generate the posterior variates.
     observed_rv_expr
         An expression that represents the observed variable.
     posterior_exp
         An expression that represents the posterior distribution of the latent
         variable.
 
     """
@@ -42,80 +47,67 @@
     z_type_idx_lv = var()
     z_et = etuple(
         etuplize(at.random.gamma), z_rng_lv, z_size_lv, z_type_idx_lv, alpha_lv, beta_lv
     )
     Y_et = etuple(etuplize(at.random.poisson), var(), var(), var(), z_et)
 
     # Posterior distribution for p
-    new_alpha_et = etuple(etuplize(at.add), alpha_lv, observed_val)
+    new_alpha_et = etuple(etuplize(at.add), alpha_lv, observed_rv_expr)
     new_beta_et = etuple(etuplize(at.add), beta_lv, 1)
     z_posterior_et = etuple(
-        etuplize(at.random.gamma),
+        partial(srng.gen, at.random.gamma),
         new_alpha_et,
         new_beta_et,
-        rng=z_rng_lv,
         size=z_size_lv,
         dtype=z_type_idx_lv,
     )
 
     return lall(
         eq(observed_rv_expr, Y_et),
         eq(posterior_expr, z_posterior_et),
     )
 
 
-@node_rewriter([PoissonRV])
-def local_gamma_poisson_posterior(fgraph, node):
-    sampler_mappings = getattr(fgraph, "sampler_mappings", None)
-
+@sampler_finder([PoissonRV])
+def local_gamma_poisson_posterior(fgraph, node, srng):
     rv_var = node.outputs[1]
-    key = ("local_gamma_poisson_posterior", rv_var)
-
-    if sampler_mappings is None or key in sampler_mappings.rvs_seen:
-        return None  # pragma: no cover
 
     q = var()
 
     rv_et = etuplize(rv_var)
 
-    res = run(None, q, gamma_poisson_conjugateo(rv_var, rv_et, q))
+    res = run(None, q, partial(gamma_poisson_conjugateo, srng)(rv_et, q))
     res = next(res, None)
 
     if res is None:
         return None  # pragma: no cover
 
     gamma_rv = rv_et[-1].evaled_obj
     gamma_posterior = eval_if_etuple(res)
 
-    sampler_mappings.rvs_to_samplers.setdefault(gamma_rv, []).append(
-        ("local_gamma_poisson_posterior", gamma_posterior, None)
-    )
-    sampler_mappings.rvs_seen.add(key)
-
-    return rv_var.owner.outputs
+    return [(gamma_rv, gamma_posterior, None)]
 
 
-def beta_binomial_conjugateo(observed_val, observed_rv_expr, posterior_expr):
-    r"""Produce a goal that represents the application of Bayes theorem
-    for a beta prior with a binomial observation model.
+def beta_binomial_conjugateo(srng: "RandomStream", observed_rv_expr, posterior_expr):
+    r"""Relation for the conjugate posterior of a beta prior with a binomial observation model.
 
     .. math::
 
         \frac{
             Y \sim \operatorname{Binom}\left(N, p\right), \quad
             p \sim \operatorname{Beta}\left(\alpha, \beta\right)
         }{
             \left(p|Y=y\right) \sim \operatorname{Beta}\left(\alpha+y, \beta+N-y\right)
         }
 
 
     Parameters
     ----------
-    observed_val
-        The observed value.
+    srng
+        The `RandomStream` used to generate the posterior variates.
     observed_rv_expr
         An expression that represents the observed variable.
     posterior_exp
         An expression that represents the posterior distribution of the latent
         variable.
 
     """
@@ -127,86 +119,76 @@
     p_et = etuple(
         etuplize(at.random.beta), p_rng_lv, p_size_lv, p_type_idx_lv, alpha_lv, beta_lv
     )
     n_lv = var()
     Y_et = etuple(etuplize(at.random.binomial), var(), var(), var(), n_lv, p_et)
 
     # Posterior distribution for p
-    new_alpha_et = etuple(etuplize(at.add), alpha_lv, observed_val)
+    new_alpha_et = etuple(etuplize(at.add), alpha_lv, observed_rv_expr)
     new_beta_et = etuple(
-        etuplize(at.sub), etuple(etuplize(at.add), beta_lv, n_lv), observed_val
+        etuplize(at.sub), etuple(etuplize(at.add), beta_lv, n_lv), observed_rv_expr
     )
     p_posterior_et = etuple(
-        etuplize(at.random.beta),
+        partial(srng.gen, at.random.beta),
         new_alpha_et,
         new_beta_et,
-        rng=p_rng_lv,
         size=p_size_lv,
         dtype=p_type_idx_lv,
     )
 
     return lall(
         eq(observed_rv_expr, Y_et),
         eq(posterior_expr, p_posterior_et),
     )
 
 
-@node_rewriter([BinomialRV])
-def local_beta_binomial_posterior(fgraph, node):
-    sampler_mappings = getattr(fgraph, "sampler_mappings", None)
-
+@sampler_finder([BinomialRV])
+def local_beta_binomial_posterior(fgraph, node, srng):
     rv_var = node.outputs[1]
-    key = ("local_beta_binomial_posterior", rv_var)
-
-    if sampler_mappings is None or key in sampler_mappings.rvs_seen:
-        return None  # pragma: no cover
 
     q = var()
 
     rv_et = etuplize(rv_var)
 
-    res = run(None, q, beta_binomial_conjugateo(rv_var, rv_et, q))
+    res = run(None, q, partial(beta_binomial_conjugateo, srng)(rv_et, q))
     res = next(res, None)
 
     if res is None:
         return None  # pragma: no cover
 
     beta_rv = rv_et[-1].evaled_obj
     beta_posterior = eval_if_etuple(res)
 
-    sampler_mappings.rvs_to_samplers.setdefault(beta_rv, []).append(
-        ("local_beta_binomial_posterior", beta_posterior, None)
-    )
-    sampler_mappings.rvs_seen.add(key)
-
-    return rv_var.owner.outputs
+    return [(beta_rv, beta_posterior, None)]
 
 
-def beta_negative_binomial_conjugateo(observed_val, observed_rv_expr, posterior_expr):
-    r"""Produce a goal that represents the application of Bayes theorem
-    for a beta prior with a negative binomial observation model.
+def beta_negative_binomial_conjugateo(
+    srng: "RandomStream", observed_rv_expr, posterior_expr
+):
+    r"""Relation for the conjugate posterior of a beta prior with a negative binomial observation model.
 
     .. math::
 
         \frac{
             Y \sim \operatorname{NB}\left(k, p\right), \quad
             p \sim \operatorname{Beta}\left(\alpha, \beta\right)
         }{
             \left(p \mid Y=y\right) \sim \operatorname{Beta}\left(\alpha + \sum^{n}_{i=1} y_i, \beta + k n\right)
         }
-        where :math:`k` is the number of successes before experiment ended.
+
+    where :math:`k` is the number of successes before the experiment ended.
 
 
     Parameters
     ----------
-    observed_val
-        The observed value.
+    srng
+        The `RandomStream` used to generate the posterior variates.
     observed_rv_expr
         An expression that represents the observed variable.
-    posterior_exp
+    posterior_expr
         An expression that represents the posterior distribution of the latent
         variable.
 
     """
     # beta-negative_binomial observation model
     alpha_lv, beta_lv = var(), var()
     p_rng_lv = var()
@@ -216,60 +198,48 @@
         etuplize(at.random.beta), p_rng_lv, p_size_lv, p_type_idx_lv, alpha_lv, beta_lv
     )
     n_lv = var()  # success
     Y_et = etuple(
         etuplize(at.random.negative_binomial), var(), var(), var(), n_lv, p_et
     )
 
-    new_alpha_et = etuple(etuplize(at.add), alpha_lv, observed_val)
+    new_alpha_et = etuple(etuplize(at.add), alpha_lv, observed_rv_expr)
     new_beta_et = etuple(etuplize(at.add), beta_lv, n_lv)
     p_posterior_et = etuple(
-        etuplize(at.random.beta),
+        partial(srng.gen, at.random.beta),
         new_alpha_et,
         new_beta_et,
-        rng=p_rng_lv,
         size=p_size_lv,
         dtype=p_type_idx_lv,
     )
 
     return lall(
         eq(observed_rv_expr, Y_et),
         eq(posterior_expr, p_posterior_et),
     )
 
 
-@node_rewriter([NegBinomialRV])
-def local_beta_negative_binomial_posterior(fgraph, node):
-    sampler_mappings = getattr(fgraph, "sampler_mappings", None)
-
+@sampler_finder([NegBinomialRV])
+def local_beta_negative_binomial_posterior(fgraph, node, srng):
     rv_var = node.outputs[1]
-    key = ("local_beta_negative_binomial_posterior", rv_var)
-
-    if sampler_mappings is None or key in sampler_mappings.rvs_seen:
-        return None  # pragma: no cover
 
     q = var()
 
     rv_et = etuplize(rv_var)
 
-    res = run(None, q, beta_negative_binomial_conjugateo(rv_var, rv_et, q))
+    res = run(None, q, partial(beta_negative_binomial_conjugateo, srng)(rv_et, q))
     res = next(res, None)
 
     if res is None:
         return None  # pragma: no cover
 
     beta_rv = rv_et[-1].evaled_obj
     beta_posterior = eval_if_etuple(res)
 
-    sampler_mappings.rvs_to_samplers.setdefault(beta_rv, []).append(
-        ("local_beta_negative_binomial_posterior", beta_posterior, None)
-    )
-    sampler_mappings.rvs_seen.add(key)
-
-    return rv_var.owner.outputs
+    return [(beta_rv, beta_posterior, None)]
 
 
 conjugates_db = LocalGroupDB(apply_all_rewrites=True)
 conjugates_db.name = "conjugates_db"
 conjugates_db.register("beta_binomial", local_beta_binomial_posterior, "basic")
 conjugates_db.register("gamma_poisson", local_gamma_poisson_posterior, "basic")
 conjugates_db.register(
```

### Comparing `aemcmc-nightly-0.0.8.dev20230516/aemcmc/dists.py` & `aemcmc-nightly-0.0.8.dev20230517/aemcmc/dists.py`

 * *Files identical despite different names*

### Comparing `aemcmc-nightly-0.0.8.dev20230516/aemcmc/ffbs.py` & `aemcmc-nightly-0.0.8.dev20230517/aemcmc/ffbs.py`

 * *Files identical despite different names*

### Comparing `aemcmc-nightly-0.0.8.dev20230516/aemcmc/gibbs.py` & `aemcmc-nightly-0.0.8.dev20230517/aemcmc/gibbs.py`

 * *Files identical despite different names*

### Comparing `aemcmc-nightly-0.0.8.dev20230516/aemcmc/nuts.py` & `aemcmc-nightly-0.0.8.dev20230517/aemcmc/nuts.py`

 * *Files identical despite different names*

### Comparing `aemcmc-nightly-0.0.8.dev20230516/aemcmc/rewriting.py` & `aemcmc-nightly-0.0.8.dev20230517/aemcmc/rewriting.py`

 * *Files identical despite different names*

### Comparing `aemcmc-nightly-0.0.8.dev20230516/aemcmc/sample.py` & `aemcmc-nightly-0.0.8.dev20230517/aemcmc/sample.py`

 * *Files identical despite different names*

### Comparing `aemcmc-nightly-0.0.8.dev20230516/aemcmc/transforms.py` & `aemcmc-nightly-0.0.8.dev20230517/aemcmc/transforms.py`

 * *Files identical despite different names*

### Comparing `aemcmc-nightly-0.0.8.dev20230516/aemcmc/types.py` & `aemcmc-nightly-0.0.8.dev20230517/aemcmc/types.py`

 * *Files identical despite different names*

### Comparing `aemcmc-nightly-0.0.8.dev20230516/aemcmc/utils.py` & `aemcmc-nightly-0.0.8.dev20230517/aemcmc/utils.py`

 * *Files identical despite different names*

### Comparing `aemcmc-nightly-0.0.8.dev20230516/aemcmc_nightly.egg-info/PKG-INFO` & `aemcmc-nightly-0.0.8.dev20230517/aemcmc_nightly.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aemcmc-nightly
-Version: 0.0.8.dev20230516
+Version: 0.0.8.dev20230517
 Summary: Miscellaneous MCMC samplers written in Aesara
 Home-page: http://github.com/aesara-devs/aemcmc
 Author: aesara-devs
 Author-email: aesara.devs@gmail.com
 Keywords: math,probability,numerical,symbolic,MCMC
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
```

### Comparing `aemcmc-nightly-0.0.8.dev20230516/aemcmc_nightly.egg-info/SOURCES.txt` & `aemcmc-nightly-0.0.8.dev20230517/aemcmc_nightly.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aemcmc-nightly-0.0.8.dev20230516/setup.cfg` & `aemcmc-nightly-0.0.8.dev20230517/setup.cfg`

 * *Files 3% similar despite different names*

```diff
@@ -28,14 +28,15 @@
 
 [coverage:report]
 omit = 
 	aemcmc/_version.py
 	tests/*
 exclude_lines = 
 	pragma: no cover
+	if TYPE_CHECKING:
 show_missing = 1
 
 [isort]
 multi_line_output = 3
 include_trailing_comma = True
 force_grid_wrap = 0
 use_parentheses = True
```

### Comparing `aemcmc-nightly-0.0.8.dev20230516/setup.py` & `aemcmc-nightly-0.0.8.dev20230517/setup.py`

 * *Files identical despite different names*

### Comparing `aemcmc-nightly-0.0.8.dev20230516/tests/test_basic.py` & `aemcmc-nightly-0.0.8.dev20230517/tests/test_basic.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 from aemcmc.basic import construct_sampler
 from aemcmc.gibbs import (
     DispersionGibbsKernel,
     HorseshoeGibbsKernel,
     NBRegressionGibbsKernel,
 )
 from aemcmc.rewriting import SubsumingElemwise
+from tests.utils import assert_consistent_rng_updates
 
 
 def test_closed_form_posterior_beta_binomial():
     srng = RandomStream(0)
 
     alpha_tt = at.scalar("alpha")
     beta_tt = at.scalar("beta")
@@ -31,14 +32,15 @@
 
     sampler, initial_values = construct_sampler({Y_rv: y_vv}, srng)
 
     p_posterior_step = sampler.sample_steps[p_rv]
     assert len(sampler.parameters) == 0
     assert len(sampler.stages) == 1
     assert isinstance(p_posterior_step.owner.op, BetaRV)
+    assert_consistent_rng_updates(p_posterior_step)
 
 
 def test_closed_form_posterior_gamma_poisson():
     srng = RandomStream(0)
 
     alpha_tt = at.scalar("alpha")
     beta_tt = at.scalar("beta")
@@ -51,14 +53,15 @@
 
     sampler, initial_values = construct_sampler({Y_rv: y_vv}, srng)
 
     p_posterior_step = sampler.sample_steps[l_rv]
     assert len(sampler.parameters) == 0
     assert len(sampler.stages) == 1
     assert isinstance(p_posterior_step.owner.op, GammaRV)
+    assert_consistent_rng_updates(p_posterior_step)
 
 
 def test_closed_form_posterior_beta_nbinom():
     srng = RandomStream(0)
 
     alpha_tt = at.scalar("alpha")
     beta_tt = at.scalar("beta")
@@ -73,14 +76,15 @@
 
     sampler, initial_values = construct_sampler({Y_rv: y_vv}, srng)
 
     p_posterior_step = sampler.sample_steps[p_rv]
     assert len(sampler.parameters) == 0
     assert len(sampler.stages) == 1
     assert isinstance(p_posterior_step.owner.op, BetaRV)
+    assert_consistent_rng_updates(p_posterior_step)
 
 
 @pytest.mark.parametrize("size", [1, (1,), (2, 3)])
 def test_nuts_sampler_single_variable(size):
     """We make sure that the NUTS sampler compiles and updates the chains for
     different sizes of the random variable.
 
@@ -94,14 +98,15 @@
     y_vv.name = "y"
 
     sampler, initial_values = construct_sampler({Y_rv: y_vv}, srng)
     assert len(sampler.sample_steps) == 1
     assert len(sampler.stages) == 1
 
     tau_post_step = sampler.sample_steps[tau_rv]
+    assert_consistent_rng_updates(tau_post_step)
     nuts = tau_post_step.owner.op
     assert y_vv in graph_inputs([tau_post_step])
     assert len(sampler.parameters[nuts]) == 2
 
     inputs = [
         initial_values[tau_rv],
         y_vv,
@@ -133,18 +138,19 @@
     y_vv = Y_rv.clone()
     y_vv.name = "y"
 
     sampler, initial_values = construct_sampler({Y_rv: y_vv}, srng)
 
     assert len(sampler.stages) == 2
 
-    p_posterior_step = sampler.sample_steps[l_rv]
-    assert y_vv in graph_inputs([p_posterior_step])
+    l_posterior_step = sampler.sample_steps[l_rv]
+    assert_consistent_rng_updates(l_posterior_step)
+    assert y_vv in graph_inputs([l_posterior_step])
     assert len(initial_values) == 2
-    assert isinstance(p_posterior_step.owner.op, GammaRV)
+    assert isinstance(l_posterior_step.owner.op, GammaRV)
 
     assert beta_rv in sampler.sample_steps
 
 
 def test_create_gibbs():
     srng = RandomStream(0)
 
@@ -174,23 +180,27 @@
     assert len(sampler.sample_steps) == 4
     assert len(sampler.stages) == 3
     assert sampler.updates
 
     tau_post_step = sampler.sample_steps[tau_rv]
     # These are *very* rough checks of the resulting graphs
     assert isinstance(tau_post_step.owner.op, HorseshoeGibbsKernel)
+    assert_consistent_rng_updates(tau_post_step)
 
     lmbda_post_step = sampler.sample_steps[lmbda_rv]
     assert isinstance(lmbda_post_step.owner.op, HorseshoeGibbsKernel)
+    assert_consistent_rng_updates(lmbda_post_step)
 
     beta_post_step = sampler.sample_steps[beta_rv]
     assert isinstance(beta_post_step.owner.op, NBRegressionGibbsKernel)
+    assert_consistent_rng_updates(beta_post_step)
 
     h_post_step = sampler.sample_steps[h_rv]
     assert isinstance(h_post_step.owner.op, DispersionGibbsKernel)
+    assert_consistent_rng_updates(h_post_step)
 
     inputs = [X, a, b, y_vv] + [initial_values[rv] for rv in sample_vars]
     outputs = [sampler.sample_steps[rv] for rv in sample_vars]
 
     subsuming_elemwises = [
         n for n in io_toposort([], outputs) if isinstance(n.op, SubsumingElemwise)
     ]
```

### Comparing `aemcmc-nightly-0.0.8.dev20230516/tests/test_conjugates.py` & `aemcmc-nightly-0.0.8.dev20230517/tests/test_conjugates.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,40 +1,34 @@
 import aesara
 import aesara.tensor as at
 import pytest
-from aesara.graph.rewriting.unify import eval_if_etuple
 from aesara.tensor.random import RandomStream
+from etuples import etuplize
 from kanren import run
 from unification import var
 
 from aemcmc.conjugates import (
     beta_binomial_conjugateo,
     beta_negative_binomial_conjugateo,
     gamma_poisson_conjugateo,
 )
 
 
 def test_gamma_poisson_conjugate_contract():
-    """Produce the closed-form posterior for the poisson observation model with
-    a gamma prior.
-
-    """
+    """Produce the closed-form posterior for the poisson observation model with a gamma prior."""
     srng = RandomStream(0)
 
     alpha_tt = at.scalar("alpha")
     beta_tt = at.scalar("beta")
     z_rv = srng.gamma(alpha_tt, beta_tt)
-
     Y_rv = srng.poisson(z_rv)
-    y_vv = Y_rv.clone()
-    y_vv.name = "y"
 
     q_lv = var()
-    (posterior_expr,) = run(1, q_lv, gamma_poisson_conjugateo(y_vv, Y_rv, q_lv))
-    posterior = eval_if_etuple(posterior_expr)
+    (posterior_expr,) = run(1, q_lv, gamma_poisson_conjugateo(srng, Y_rv, q_lv))
+    posterior = posterior_expr.evaled_obj
 
     assert isinstance(posterior.owner.op, type(at.random.gamma))
 
 
 @pytest.mark.xfail(
     reason="Op.__call__ does not dispatch to Op.make_node for some RandomVariable and etuple evaluation returns an error"
 )
@@ -43,46 +37,42 @@
 
     srng = RandomStream(0)
 
     alpha_tt = at.scalar("alpha")
     beta_tt = at.scalar("beta")
     y_vv = at.iscalar("y")
     Y_rv = srng.gamma(alpha_tt + y_vv, beta_tt + 1)
+    Y_et = etuplize(Y_rv)
 
     e_lv = var()
-    (expanded_expr,) = run(1, e_lv, gamma_poisson_conjugateo(e_lv, y_vv, Y_rv))
-    expanded = eval_if_etuple(expanded_expr)
+    (expanded_expr,) = run(1, e_lv, gamma_poisson_conjugateo(srng, e_lv, Y_et))
+    expanded = expanded_expr.evaled_obj
 
     assert isinstance(expanded.owner.op, type(at.random.gamma))
 
 
 def test_beta_binomial_conjugate_contract():
-    """Produce the closed-form posterior for the binomial observation model with
-    a beta prior.
-
-    """
+    """Produce the closed-form posterior for the binomial observation model with a beta prior."""
     srng = RandomStream(0)
 
     alpha_tt = at.scalar("alpha")
     beta_tt = at.scalar("beta")
     p_rv = srng.beta(alpha_tt, beta_tt, name="p")
 
     n_tt = at.iscalar("n")
     Y_rv = srng.binomial(n_tt, p_rv)
-    y_vv = Y_rv.clone()
-    y_vv.tag.name = "y"
 
     q_lv = var()
-    (posterior_expr,) = run(1, q_lv, beta_binomial_conjugateo(y_vv, Y_rv, q_lv))
-    posterior = eval_if_etuple(posterior_expr)
+    (posterior_expr,) = run(1, q_lv, beta_binomial_conjugateo(srng, Y_rv, q_lv))
+    posterior = posterior_expr.evaled_obj
 
     assert isinstance(posterior.owner.op, type(at.random.beta))
 
     # Build the sampling function and check the results on limiting cases.
-    sample_fn = aesara.function((alpha_tt, beta_tt, y_vv, n_tt), posterior)
+    sample_fn = aesara.function((alpha_tt, beta_tt, Y_rv, n_tt), posterior)
     assert sample_fn(1.0, 1.0, 1000, 1000) == pytest.approx(
         1.0, abs=0.01
     )  # only successes
     assert sample_fn(1.0, 1.0, 0, 1000) == pytest.approx(0.0, abs=0.01)  # zero success
 
 
 @pytest.mark.xfail(
@@ -96,46 +86,41 @@
     alpha_tt = at.scalar("alpha")
     beta_tt = at.scalar("beta")
     y_vv = at.iscalar("y")
     n_tt = at.iscalar("n")
     Y_rv = srng.beta(alpha_tt + y_vv, beta_tt + n_tt - y_vv)
 
     e_lv = var()
-    (expanded_expr,) = run(1, e_lv, beta_binomial_conjugateo(e_lv, y_vv, Y_rv))
-    expanded = eval_if_etuple(expanded_expr)
+    (expanded_expr,) = run(1, e_lv, beta_binomial_conjugateo(srng, e_lv, Y_rv))
+    expanded = expanded_expr.evaled_obj
 
     assert isinstance(expanded.owner.op, type(at.random.beta))
 
 
 def test_beta_negative_binomial_conjugate_contract():
-    """Produce the closed-form posterior for the binomial observation model with
-    a beta prior.
-
-    """
+    """Produce the closed-form posterior for the binomial observation model with a beta prior."""
     srng = RandomStream(0)
 
     alpha_tt = at.scalar("alpha")
     beta_tt = at.scalar("beta")
     p_rv = srng.beta(alpha_tt, beta_tt, name="p")
 
     n_tt = at.iscalar("n")
     Y_rv = srng.negative_binomial(n_tt, p_rv)
-    y_vv = Y_rv.clone()
-    y_vv.tag.name = "y"
 
     q_lv = var()
     (posterior_expr,) = run(
-        1, q_lv, beta_negative_binomial_conjugateo(y_vv, Y_rv, q_lv)
+        1, q_lv, beta_negative_binomial_conjugateo(srng, Y_rv, q_lv)
     )
-    posterior = eval_if_etuple(posterior_expr)
+    posterior = posterior_expr.evaled_obj
 
     assert isinstance(posterior.owner.op, type(at.random.beta))
 
     # Build the sampling function and check the results on limiting cases.
-    sample_fn = aesara.function((alpha_tt, beta_tt, y_vv, n_tt), posterior)
+    sample_fn = aesara.function((alpha_tt, beta_tt, Y_rv, n_tt), posterior)
     assert sample_fn(1.0, 1.0, 1000, 0) == pytest.approx(
         1.0, abs=0.01
     )  # only successes
     assert sample_fn(1.0, 1.0, 0, 1000) == pytest.approx(0.0, abs=0.01)  # no success
 
 
 @pytest.mark.xfail(
@@ -149,11 +134,11 @@
     alpha_tt = at.scalar("alpha")
     beta_tt = at.scalar("beta")
     y_vv = at.iscalar("y")
     n_tt = at.iscalar("n")
     Y_rv = srng.beta(alpha_tt + y_vv, beta_tt + n_tt)
 
     e_lv = var()
-    (expanded_expr,) = run(1, e_lv, beta_negative_binomial_conjugateo(e_lv, y_vv, Y_rv))
-    expanded = eval_if_etuple(expanded_expr)
+    (expanded_expr,) = run(1, e_lv, beta_negative_binomial_conjugateo(srng, e_lv, Y_rv))
+    expanded = expanded_expr
 
     assert isinstance(expanded.owner.op, type(at.random.beta))
```

### Comparing `aemcmc-nightly-0.0.8.dev20230516/tests/test_dists.py` & `aemcmc-nightly-0.0.8.dev20230517/tests/test_dists.py`

 * *Files identical despite different names*

### Comparing `aemcmc-nightly-0.0.8.dev20230516/tests/test_ffbs.py` & `aemcmc-nightly-0.0.8.dev20230517/tests/test_ffbs.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import aesara.tensor as at
 import aesara.tensor.random as atr
 import numpy as np
 import pytest
 import scipy.stats as sp
 
 from aemcmc.ffbs import ffbs_step
+from tests.utils import assert_consistent_rng_updates
 
 
 @pytest.mark.parametrize("first_is_nonzero", [True, False])
 def test_ffbs_one_state_likelihood(first_is_nonzero):
     """Test for categorical emissions that assign non-zero likelihood to only one state."""
 
     Gammas = np.array([[[0.9, 0.1], [0.1, 0.9]]])
@@ -20,14 +21,17 @@
     if first_is_nonzero:
         log_lik = at.stack([at.broadcast_to(0.0, (N,)), at.broadcast_to(-np.inf, (N,))])
     else:
         log_lik = at.stack([at.broadcast_to(-np.inf, (N,)), at.broadcast_to(0.0, (N,))])
 
     srng = atr.RandomStream(seed=2032)
     step_at, updates = ffbs_step(gamma_0, Gammas, log_lik, srng)
+
+    assert_consistent_rng_updates(step_at)
+
     step_fn = aesara.function([], step_at, updates=updates)
     res = step_fn()
 
     if first_is_nonzero:
         assert np.all(res == 0)
     else:
         assert np.all(res == 1)
@@ -51,14 +55,17 @@
     )
 
     # TODO FIXME: This is a fairly arbitrary check
     assert np.mean(np.abs(log_lik.argmax(0) - seq)) < 1e-2
 
     srng = atr.RandomStream(seed=2032)
     step_at, updates = ffbs_step(gamma_0, Gammas, log_lik, srng)
+
+    assert_consistent_rng_updates(step_at)
+
     step_fn = aesara.function([], step_at, updates=updates)
     res = step_fn()
 
     # TODO FIXME: This is a fairly arbitrary check
     assert np.mean(np.abs(res - seq)) < 1e-2
 
 
@@ -78,11 +85,14 @@
 
     log_lik = np.tile(np.r_[np.log(0.9), np.log(0.1)], (4, 1))
     log_lik[::2] = log_lik[::2][:, ::-1]
     log_lik = log_lik.T
 
     srng = atr.RandomStream(seed=2032)
     step_at, updates = ffbs_step(gamma_0, Gammas, log_lik, srng)
+
+    assert_consistent_rng_updates(step_at)
+
     step_fn = aesara.function([], step_at, updates=updates)
     res = step_fn()
 
     assert np.array_equal(res, np.r_[1, 0, 0, 1])
```

### Comparing `aemcmc-nightly-0.0.8.dev20230516/tests/test_gibbs.py` & `aemcmc-nightly-0.0.8.dev20230517/tests/test_gibbs.py`

 * *Files identical despite different names*

### Comparing `aemcmc-nightly-0.0.8.dev20230516/tests/test_nuts.py` & `aemcmc-nightly-0.0.8.dev20230517/tests/test_nuts.py`

 * *Files identical despite different names*

### Comparing `aemcmc-nightly-0.0.8.dev20230516/tests/test_rewriting.py` & `aemcmc-nightly-0.0.8.dev20230517/tests/test_rewriting.py`

 * *Files identical despite different names*

### Comparing `aemcmc-nightly-0.0.8.dev20230516/tests/test_sample.py` & `aemcmc-nightly-0.0.8.dev20230517/tests/test_sample.py`

 * *Files identical despite different names*

### Comparing `aemcmc-nightly-0.0.8.dev20230516/tests/test_transforms.py` & `aemcmc-nightly-0.0.8.dev20230517/tests/test_transforms.py`

 * *Files identical despite different names*

### Comparing `aemcmc-nightly-0.0.8.dev20230516/tests/test_utils.py` & `aemcmc-nightly-0.0.8.dev20230517/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `aemcmc-nightly-0.0.8.dev20230516/versioneer.py` & `aemcmc-nightly-0.0.8.dev20230517/versioneer.py`

 * *Files identical despite different names*

