# Comparing `tmp/protopunica-0.14.8rc2.tar.gz` & `tmp/protopunica-0.14.8rc3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "protopunica-0.14.8rc2.tar", last modified: Thu May 18 11:38:58 2023, max compression
+gzip compressed data, was "protopunica-0.14.8rc3.tar", last modified: Thu May 18 12:31:07 2023, max compression
```

## Comparing `protopunica-0.14.8rc2.tar` & `protopunica-0.14.8rc3.tar`

### file list

```diff
@@ -1,137 +1,137 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 11:38:58.737022 protopunica-0.14.8rc2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 11:38:58.689020 protopunica-0.14.8rc2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 11:38:58.693021 protopunica-0.14.8rc2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1641 2023-05-18 11:38:48.000000 protopunica-0.14.8rc2/.github/workflows/deploy.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3078 2023-05-18 11:38:48.000000 protopunica-0.14.8rc2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-05-18 11:38:48.000000 protopunica-0.14.8rc2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-05-18 11:38:48.000000 protopunica-0.14.8rc2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2772 2023-05-18 11:38:48.000000 protopunica-0.14.8rc2/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-05-18 11:38:58.737022 protopunica-0.14.8rc2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-05-18 11:38:48.000000 protopunica-0.14.8rc2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-05-18 11:38:48.000000 protopunica-0.14.8rc2/dev-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 11:38:58.693021 protopunica-0.14.8rc2/examples/
--rw-r--r--   0 runner    (1001) docker     (123)    37818 2023-05-18 11:38:48.000000 protopunica-0.14.8rc2/examples/bayes_classifier_hmm_cheating_coin_toss.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    31444 2023-05-18 11:38:48.000000 protopunica-0.14.8rc2/examples/bayesnet_asia.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    46387 2023-05-18 11:38:48.000000 protopunica-0.14.8rc2/examples/bayesnet_huge_monty_hall.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    24325 2023-05-18 11:38:48.000000 protopunica-0.14.8rc2/examples/bayesnet_monty_hall_classic.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    18197 2023-05-18 11:38:48.000000 protopunica-0.14.8rc2/examples/bayesnet_monty_hall_train.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     5408 2023-05-18 11:38:48.000000 protopunica-0.14.8rc2/examples/distributions_conditionalupdate.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     6059 2023-05-18 11:38:48.000000 protopunica-0.14.8rc2/examples/distributions_test_table.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    11767 2023-05-18 11:38:48.000000 protopunica-0.14.8rc2/examples/hmm_example.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    14688 2023-05-18 11:38:48.000000 protopunica-0.14.8rc2/examples/hmm_infinite.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     6593 2023-05-18 11:38:48.000000 protopunica-0.14.8rc2/examples/hmm_rainy_sunny.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    32620 2023-05-18 11:38:48.000000 protopunica-0.14.8rc2/examples/hmm_tied_states.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    31867 2023-05-18 11:38:48.000000 protopunica-0.14.8rc2/examples/naivebayes_hmm_cheating_coin_toss.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     5100 2023-05-18 11:38:48.000000 protopunica-0.14.8rc2/examples/naivebayes_multivariate_male_female.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    20167 2023-05-18 11:38:48.000000 protopunica-0.14.8rc2/examples/naivebayes_simple_male_female.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 11:38:58.713021 protopunica-0.14.8rc2/protopunica/
--rw-r--r--   0 runner    (1001) docker     (123)   390213 2023-05-18 11:38:48.000000 protopunica-0.14.8rc2/protopunica/BayesClassifier.c
--rw-r--r--   0 runner    (1001) docker     (123)     8861 2023-05-18 11:38:48.000000 protopunica-0.14.8rc2/protopunica/BayesClassifier.pyx
--rw-r--r--   0 runner    (1001) docker     (123)  3324023 2023-05-18 11:38:48.000000 protopunica-0.14.8rc2/protopunica/BayesianNetwork.c
--rw-r--r--   0 runner    (1001) docker     (123)    93841 2023-05-18 11:38:48.000000 protopunica-0.14.8rc2/protopunica/BayesianNetwork.pyx
--rw-r--r--   0 runner    (1001) docker     (123)   559989 2023-05-18 11:38:48.000000 protopunica-0.14.8rc2/protopunica/FactorGraph.c
--rw-r--r--   0 runner    (1001) docker     (123)    13550 2023-05-18 11:38:48.000000 protopunica-0.14.8rc2/protopunica/FactorGraph.pyx
--rw-r--r--   0 runner    (1001) docker     (123)   356354 2023-05-18 11:38:48.000000 protopunica-0.14.8rc2/protopunica/MarkovChain.c
--rw-r--r--   0 runner    (1001) docker     (123)     8976 2023-05-18 11:38:48.000000 protopunica-0.14.8rc2/protopunica/MarkovChain.pyx
--rw-r--r--   0 runner    (1001) docker     (123)  1473880 2023-05-18 11:38:48.000000 protopunica-0.14.8rc2/protopunica/MarkovNetwork.c
--rw-r--r--   0 runner    (1001) docker     (123)    27431 2023-05-18 11:38:48.000000 protopunica-0.14.8rc2/protopunica/MarkovNetwork.pyx
--rw-r--r--   0 runner    (1001) docker     (123)   382641 2023-05-18 11:38:48.000000 protopunica-0.14.8rc2/protopunica/NaiveBayes.c
--rw-r--r--   0 runner    (1001) docker     (123)     8010 2023-05-18 11:38:48.000000 protopunica-0.14.8rc2/protopunica/NaiveBayes.pyx
--rw-r--r--   0 runner    (1001) docker     (123)     2022 2023-05-18 11:38:48.000000 protopunica-0.14.8rc2/protopunica/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)  1175408 2023-05-18 11:38:48.000000 protopunica-0.14.8rc2/protopunica/base.c
--rw-r--r--   0 runner    (1001) docker     (123)      680 2023-05-18 11:38:48.000000 protopunica-0.14.8rc2/protopunica/base.pxd
--rw-r--r--   0 runner    (1001) docker     (123)    13146 2023-05-18 11:38:48.000000 protopunica-0.14.8rc2/protopunica/base.pyx
--rw-r--r--   0 runner    (1001) docker     (123)  1541734 2023-05-18 11:38:48.000000 protopunica-0.14.8rc2/protopunica/bayes.c
--rw-r--r--   0 runner    (1001) docker     (123)      605 2023-05-18 11:38:48.000000 protopunica-0.14.8rc2/protopunica/bayes.pxd
--rw-r--r--   0 runner    (1001) docker     (123)    31650 2023-05-18 11:38:48.000000 protopunica-0.14.8rc2/protopunica/bayes.pyx
--rw-r--r--   0 runner    (1001) docker     (123)     4270 2023-05-18 11:38:48.000000 protopunica-0.14.8rc2/protopunica/callbacks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 11:38:58.737022 protopunica-0.14.8rc2/protopunica/distributions/
--rw-r--r--   0 runner    (1001) docker     (123)   909800 2023-05-18 11:38:48.000000 protopunica-0.14.8rc2/protopunica/distributions/BernoulliDistribution.c
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-05-18 11:38:48.000000 protopunica-0.14.8rc2/protopunica/distributions/BernoulliDistribution.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     2278 2023-05-18 11:38:48.000000 protopunica-0.14.8rc2/protopunica/distributions/BernoulliDistribution.pyx
--rw-r--r--   0 runner    (1001) docker     (123)   918256 2023-05-18 11:38:48.000000 protopunica-0.14.8rc2/protopunica/distributions/BetaDistribution.c
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-05-18 11:38:48.000000 protopunica-0.14.8rc2/protopunica/distributions/BetaDistribution.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     2864 2023-05-18 11:38:48.000000 protopunica-0.14.8rc2/protopunica/distributions/BetaDistribution.pyx
--rw-r--r--   0 runner    (1001) docker     (123)  1427423 2023-05-18 11:38:48.000000 protopunica-0.14.8rc2/protopunica/distributions/ConditionalProbabilityTable.c
--rw-r--r--   0 runner    (1001) docker     (123)      639 2023-05-18 11:38:48.000000 protopunica-0.14.8rc2/protopunica/distributions/ConditionalProbabilityTable.pxd
--rw-r--r--   0 runner    (1001) docker     (123)    10725 2023-05-18 11:38:48.000000 protopunica-0.14.8rc2/protopunica/distributions/ConditionalProbabilityTable.pyx
--rw-r--r--   0 runner    (1001) docker     (123)   956112 2023-05-18 11:38:48.000000 protopunica-0.14.8rc2/protopunica/distributions/DirichletDistribution.c
--rw-r--r--   0 runner    (1001) docker     (123)      373 2023-05-18 11:38:48.000000 protopunica-0.14.8rc2/protopunica/distributions/DirichletDistribution.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     2945 2023-05-18 11:38:48.000000 protopunica-0.14.8rc2/protopunica/distributions/DirichletDistribution.pyx
--rw-r--r--   0 runner    (1001) docker     (123)  1299521 2023-05-18 11:38:48.000000 protopunica-0.14.8rc2/protopunica/distributions/DiscreteDistribution.c
--rw-r--r--   0 runner    (1001) docker     (123)      486 2023-05-18 11:38:48.000000 protopunica-0.14.8rc2/protopunica/distributions/DiscreteDistribution.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     9855 2023-05-18 11:38:48.000000 protopunica-0.14.8rc2/protopunica/distributions/DiscreteDistribution.pyx
--rw-r--r--   0 runner    (1001) docker     (123)   911061 2023-05-18 11:38:48.000000 protopunica-0.14.8rc2/protopunica/distributions/ExponentialDistribution.c
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-05-18 11:38:48.000000 protopunica-0.14.8rc2/protopunica/distributions/ExponentialDistribution.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     2511 2023-05-18 11:38:48.000000 protopunica-0.14.8rc2/protopunica/distributions/ExponentialDistribution.pyx
--rw-r--r--   0 runner    (1001) docker     (123)  1013935 2023-05-18 11:38:48.000000 protopunica-0.14.8rc2/protopunica/distributions/GammaDistribution.c
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-05-18 11:38:48.000000 protopunica-0.14.8rc2/protopunica/distributions/GammaDistribution.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     7928 2023-05-18 11:38:48.000000 protopunica-0.14.8rc2/protopunica/distributions/GammaDistribution.pyx
--rw-r--r--   0 runner    (1001) docker     (123)  1103415 2023-05-18 11:38:48.000000 protopunica-0.14.8rc2/protopunica/distributions/IndependentComponentsDistribution.c
--rw-r--r--   0 runner    (1001) docker     (123)      474 2023-05-18 11:38:48.000000 protopunica-0.14.8rc2/protopunica/distributions/IndependentComponentsDistribution.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     7896 2023-05-18 11:38:48.000000 protopunica-0.14.8rc2/protopunica/distributions/IndependentComponentsDistribution.pyx
--rw-r--r--   0 runner    (1001) docker     (123)  1366877 2023-05-18 11:38:48.000000 protopunica-0.14.8rc2/protopunica/distributions/JointProbabilityTable.c
--rw-r--r--   0 runner    (1001) docker     (123)      481 2023-05-18 11:38:48.000000 protopunica-0.14.8rc2/protopunica/distributions/JointProbabilityTable.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     8034 2023-05-18 11:38:48.000000 protopunica-0.14.8rc2/protopunica/distributions/JointProbabilityTable.pyx
--rw-r--r--   0 runner    (1001) docker     (123)  1060465 2023-05-18 11:38:48.000000 protopunica-0.14.8rc2/protopunica/distributions/KernelDensities.c
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-05-18 11:38:48.000000 protopunica-0.14.8rc2/protopunica/distributions/KernelDensities.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     8057 2023-05-18 11:38:48.000000 protopunica-0.14.8rc2/protopunica/distributions/KernelDensities.pyx
--rw-r--r--   0 runner    (1001) docker     (123)   927414 2023-05-18 11:38:48.000000 protopunica-0.14.8rc2/protopunica/distributions/LogNormalDistribution.c
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-05-18 11:38:48.000000 protopunica-0.14.8rc2/protopunica/distributions/LogNormalDistribution.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     3185 2023-05-18 11:38:48.000000 protopunica-0.14.8rc2/protopunica/distributions/LogNormalDistribution.pyx
--rw-r--r--   0 runner    (1001) docker     (123)  1118071 2023-05-18 11:38:48.000000 protopunica-0.14.8rc2/protopunica/distributions/MultivariateGaussianDistribution.c
--rw-r--r--   0 runner    (1001) docker     (123)      676 2023-05-18 11:38:48.000000 protopunica-0.14.8rc2/protopunica/distributions/MultivariateGaussianDistribution.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     8814 2023-05-18 11:38:48.000000 protopunica-0.14.8rc2/protopunica/distributions/MultivariateGaussianDistribution.pyx
--rw-r--r--   0 runner    (1001) docker     (123)     5534 2023-05-18 11:38:48.000000 protopunica-0.14.8rc2/protopunica/distributions/NeuralNetworkWrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)   932572 2023-05-18 11:38:48.000000 protopunica-0.14.8rc2/protopunica/distributions/NormalDistribution.c
--rw-r--r--   0 runner    (1001) docker     (123)      279 2023-05-18 11:38:48.000000 protopunica-0.14.8rc2/protopunica/distributions/NormalDistribution.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     3134 2023-05-18 11:38:48.000000 protopunica-0.14.8rc2/protopunica/distributions/NormalDistribution.pyx
--rw-r--r--   0 runner    (1001) docker     (123)   910130 2023-05-18 11:38:48.000000 protopunica-0.14.8rc2/protopunica/distributions/PoissonDistribution.c
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-05-18 11:38:48.000000 protopunica-0.14.8rc2/protopunica/distributions/PoissonDistribution.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     2759 2023-05-18 11:38:48.000000 protopunica-0.14.8rc2/protopunica/distributions/PoissonDistribution.pyx
--rw-r--r--   0 runner    (1001) docker     (123)   928439 2023-05-18 11:38:48.000000 protopunica-0.14.8rc2/protopunica/distributions/UniformDistribution.c
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-05-18 11:38:48.000000 protopunica-0.14.8rc2/protopunica/distributions/UniformDistribution.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     2788 2023-05-18 11:38:48.000000 protopunica-0.14.8rc2/protopunica/distributions/UniformDistribution.pyx
--rw-r--r--   0 runner    (1001) docker     (123)     1215 2023-05-18 11:38:48.000000 protopunica-0.14.8rc2/protopunica/distributions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   551722 2023-05-18 11:38:48.000000 protopunica-0.14.8rc2/protopunica/distributions/distributions.c
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-05-18 11:38:48.000000 protopunica-0.14.8rc2/protopunica/distributions/distributions.pxd
--rw-r--r--   0 runner    (1001) docker     (123)    10029 2023-05-18 11:38:48.000000 protopunica-0.14.8rc2/protopunica/distributions/distributions.pyx
--rw-r--r--   0 runner    (1001) docker     (123)  1221029 2023-05-18 11:38:48.000000 protopunica-0.14.8rc2/protopunica/gmm.c
--rw-r--r--   0 runner    (1001) docker     (123)    23761 2023-05-18 11:38:48.000000 protopunica-0.14.8rc2/protopunica/gmm.pyx
--rw-r--r--   0 runner    (1001) docker     (123)  2835749 2023-05-18 11:38:48.000000 protopunica-0.14.8rc2/protopunica/hmm.c
--rw-r--r--   0 runner    (1001) docker     (123)   126627 2023-05-18 11:38:48.000000 protopunica-0.14.8rc2/protopunica/hmm.pyx
--rw-r--r--   0 runner    (1001) docker     (123)    12415 2023-05-18 11:38:48.000000 protopunica-0.14.8rc2/protopunica/io.py
--rw-r--r--   0 runner    (1001) docker     (123)  1374225 2023-05-18 11:38:48.000000 protopunica-0.14.8rc2/protopunica/kmeans.c
--rw-r--r--   0 runner    (1001) docker     (123)    24982 2023-05-18 11:38:48.000000 protopunica-0.14.8rc2/protopunica/kmeans.pyx
--rw-r--r--   0 runner    (1001) docker     (123)   704735 2023-05-18 11:38:48.000000 protopunica-0.14.8rc2/protopunica/parallel.c
--rw-r--r--   0 runner    (1001) docker     (123)    15976 2023-05-18 11:38:48.000000 protopunica-0.14.8rc2/protopunica/parallel.pyx
--rw-r--r--   0 runner    (1001) docker     (123)  1223513 2023-05-18 11:38:48.000000 protopunica-0.14.8rc2/protopunica/utils.c
--rw-r--r--   0 runner    (1001) docker     (123)      745 2023-05-18 11:38:48.000000 protopunica-0.14.8rc2/protopunica/utils.pxd
--rw-r--r--   0 runner    (1001) docker     (123)    13248 2023-05-18 11:38:48.000000 protopunica-0.14.8rc2/protopunica/utils.pyx
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 11:38:58.713021 protopunica-0.14.8rc2/protopunica.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-05-18 11:38:58.000000 protopunica-0.14.8rc2/protopunica.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4589 2023-05-18 11:38:58.000000 protopunica-0.14.8rc2/protopunica.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 11:38:58.000000 protopunica-0.14.8rc2/protopunica.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 11:38:58.000000 protopunica-0.14.8rc2/protopunica.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-05-18 11:38:58.000000 protopunica-0.14.8rc2/protopunica.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-18 11:38:58.000000 protopunica-0.14.8rc2/protopunica.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-05-18 11:38:48.000000 protopunica-0.14.8rc2/pyproject.toml
--rwxr-xr-x   0 runner    (1001) docker     (123)     1840 2023-05-18 11:38:48.000000 protopunica-0.14.8rc2/rebuildconda
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-05-18 11:38:48.000000 protopunica-0.14.8rc2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-18 11:38:58.737022 protopunica-0.14.8rc2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3075 2023-05-18 11:38:48.000000 protopunica-0.14.8rc2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 11:38:58.737022 protopunica-0.14.8rc2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 11:38:48.000000 protopunica-0.14.8rc2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23744 2023-05-18 11:38:48.000000 protopunica-0.14.8rc2/tests/test_bayes_classifier.py
--rw-r--r--   0 runner    (1001) docker     (123)    59630 2023-05-18 11:38:48.000000 protopunica-0.14.8rc2/tests/test_bayesian_network.py
--rw-r--r--   0 runner    (1001) docker     (123)    27669 2023-05-18 11:38:48.000000 protopunica-0.14.8rc2/tests/test_custom_distributions.py
--rw-r--r--   0 runner    (1001) docker     (123)    45538 2023-05-18 11:38:48.000000 protopunica-0.14.8rc2/tests/test_distributions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1608 2023-05-18 11:38:48.000000 protopunica-0.14.8rc2/tests/test_factor_graphs.py
--rw-r--r--   0 runner    (1001) docker     (123)    51403 2023-05-18 11:38:48.000000 protopunica-0.14.8rc2/tests/test_gmm.py
--rw-r--r--   0 runner    (1001) docker     (123)    81204 2023-05-18 11:38:48.000000 protopunica-0.14.8rc2/tests/test_hmm.py
--rw-r--r--   0 runner    (1001) docker     (123)    23788 2023-05-18 11:38:48.000000 protopunica-0.14.8rc2/tests/test_io.py
--rw-r--r--   0 runner    (1001) docker     (123)    13746 2023-05-18 11:38:48.000000 protopunica-0.14.8rc2/tests/test_kmeans.py
--rw-r--r--   0 runner    (1001) docker     (123)    20298 2023-05-18 11:38:48.000000 protopunica-0.14.8rc2/tests/test_markov_chain.py
--rw-r--r--   0 runner    (1001) docker     (123)    18046 2023-05-18 11:38:48.000000 protopunica-0.14.8rc2/tests/test_markov_network.py
--rw-r--r--   0 runner    (1001) docker     (123)    30069 2023-05-18 11:38:48.000000 protopunica-0.14.8rc2/tests/test_naive_bayes.py
--rw-r--r--   0 runner    (1001) docker     (123)    17863 2023-05-18 11:38:48.000000 protopunica-0.14.8rc2/tests/test_profile_hmm.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 12:31:07.536670 protopunica-0.14.8rc3/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 12:31:07.488670 protopunica-0.14.8rc3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 12:31:07.492670 protopunica-0.14.8rc3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1641 2023-05-18 12:30:58.000000 protopunica-0.14.8rc3/.github/workflows/deploy.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3078 2023-05-18 12:30:58.000000 protopunica-0.14.8rc3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-05-18 12:30:58.000000 protopunica-0.14.8rc3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-05-18 12:30:58.000000 protopunica-0.14.8rc3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2772 2023-05-18 12:30:58.000000 protopunica-0.14.8rc3/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-05-18 12:31:07.536670 protopunica-0.14.8rc3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-05-18 12:30:58.000000 protopunica-0.14.8rc3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-05-18 12:30:58.000000 protopunica-0.14.8rc3/dev-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 12:31:07.492670 protopunica-0.14.8rc3/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)    37818 2023-05-18 12:30:58.000000 protopunica-0.14.8rc3/examples/bayes_classifier_hmm_cheating_coin_toss.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    31444 2023-05-18 12:30:58.000000 protopunica-0.14.8rc3/examples/bayesnet_asia.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    46387 2023-05-18 12:30:58.000000 protopunica-0.14.8rc3/examples/bayesnet_huge_monty_hall.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    24325 2023-05-18 12:30:58.000000 protopunica-0.14.8rc3/examples/bayesnet_monty_hall_classic.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    18197 2023-05-18 12:30:58.000000 protopunica-0.14.8rc3/examples/bayesnet_monty_hall_train.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     5408 2023-05-18 12:30:58.000000 protopunica-0.14.8rc3/examples/distributions_conditionalupdate.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     6059 2023-05-18 12:30:58.000000 protopunica-0.14.8rc3/examples/distributions_test_table.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    11767 2023-05-18 12:30:58.000000 protopunica-0.14.8rc3/examples/hmm_example.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    14688 2023-05-18 12:30:58.000000 protopunica-0.14.8rc3/examples/hmm_infinite.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     6593 2023-05-18 12:30:58.000000 protopunica-0.14.8rc3/examples/hmm_rainy_sunny.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    32620 2023-05-18 12:30:58.000000 protopunica-0.14.8rc3/examples/hmm_tied_states.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    31867 2023-05-18 12:30:58.000000 protopunica-0.14.8rc3/examples/naivebayes_hmm_cheating_coin_toss.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     5100 2023-05-18 12:30:58.000000 protopunica-0.14.8rc3/examples/naivebayes_multivariate_male_female.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    20167 2023-05-18 12:30:58.000000 protopunica-0.14.8rc3/examples/naivebayes_simple_male_female.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 12:31:07.512670 protopunica-0.14.8rc3/protopunica/
+-rw-r--r--   0 runner    (1001) docker     (123)   390213 2023-05-18 12:30:58.000000 protopunica-0.14.8rc3/protopunica/BayesClassifier.c
+-rw-r--r--   0 runner    (1001) docker     (123)     8861 2023-05-18 12:30:58.000000 protopunica-0.14.8rc3/protopunica/BayesClassifier.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)  3324023 2023-05-18 12:30:58.000000 protopunica-0.14.8rc3/protopunica/BayesianNetwork.c
+-rw-r--r--   0 runner    (1001) docker     (123)    93841 2023-05-18 12:30:58.000000 protopunica-0.14.8rc3/protopunica/BayesianNetwork.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)   559989 2023-05-18 12:30:58.000000 protopunica-0.14.8rc3/protopunica/FactorGraph.c
+-rw-r--r--   0 runner    (1001) docker     (123)    13550 2023-05-18 12:30:58.000000 protopunica-0.14.8rc3/protopunica/FactorGraph.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)   356354 2023-05-18 12:30:58.000000 protopunica-0.14.8rc3/protopunica/MarkovChain.c
+-rw-r--r--   0 runner    (1001) docker     (123)     8976 2023-05-18 12:30:58.000000 protopunica-0.14.8rc3/protopunica/MarkovChain.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)  1473880 2023-05-18 12:30:58.000000 protopunica-0.14.8rc3/protopunica/MarkovNetwork.c
+-rw-r--r--   0 runner    (1001) docker     (123)    27431 2023-05-18 12:30:58.000000 protopunica-0.14.8rc3/protopunica/MarkovNetwork.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)   382641 2023-05-18 12:30:58.000000 protopunica-0.14.8rc3/protopunica/NaiveBayes.c
+-rw-r--r--   0 runner    (1001) docker     (123)     8010 2023-05-18 12:30:58.000000 protopunica-0.14.8rc3/protopunica/NaiveBayes.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)     2022 2023-05-18 12:30:58.000000 protopunica-0.14.8rc3/protopunica/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)  1175408 2023-05-18 12:30:58.000000 protopunica-0.14.8rc3/protopunica/base.c
+-rw-r--r--   0 runner    (1001) docker     (123)      680 2023-05-18 12:30:58.000000 protopunica-0.14.8rc3/protopunica/base.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)    13146 2023-05-18 12:30:58.000000 protopunica-0.14.8rc3/protopunica/base.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)  1541734 2023-05-18 12:30:58.000000 protopunica-0.14.8rc3/protopunica/bayes.c
+-rw-r--r--   0 runner    (1001) docker     (123)      605 2023-05-18 12:30:58.000000 protopunica-0.14.8rc3/protopunica/bayes.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)    31650 2023-05-18 12:30:58.000000 protopunica-0.14.8rc3/protopunica/bayes.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)     4270 2023-05-18 12:30:58.000000 protopunica-0.14.8rc3/protopunica/callbacks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 12:31:07.536670 protopunica-0.14.8rc3/protopunica/distributions/
+-rw-r--r--   0 runner    (1001) docker     (123)   909800 2023-05-18 12:30:58.000000 protopunica-0.14.8rc3/protopunica/distributions/BernoulliDistribution.c
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-05-18 12:30:58.000000 protopunica-0.14.8rc3/protopunica/distributions/BernoulliDistribution.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     2278 2023-05-18 12:30:58.000000 protopunica-0.14.8rc3/protopunica/distributions/BernoulliDistribution.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)   918256 2023-05-18 12:30:58.000000 protopunica-0.14.8rc3/protopunica/distributions/BetaDistribution.c
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-05-18 12:30:58.000000 protopunica-0.14.8rc3/protopunica/distributions/BetaDistribution.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     2864 2023-05-18 12:30:58.000000 protopunica-0.14.8rc3/protopunica/distributions/BetaDistribution.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)  1427423 2023-05-18 12:30:58.000000 protopunica-0.14.8rc3/protopunica/distributions/ConditionalProbabilityTable.c
+-rw-r--r--   0 runner    (1001) docker     (123)      639 2023-05-18 12:30:58.000000 protopunica-0.14.8rc3/protopunica/distributions/ConditionalProbabilityTable.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)    10725 2023-05-18 12:30:58.000000 protopunica-0.14.8rc3/protopunica/distributions/ConditionalProbabilityTable.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)   956112 2023-05-18 12:30:58.000000 protopunica-0.14.8rc3/protopunica/distributions/DirichletDistribution.c
+-rw-r--r--   0 runner    (1001) docker     (123)      373 2023-05-18 12:30:58.000000 protopunica-0.14.8rc3/protopunica/distributions/DirichletDistribution.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     2945 2023-05-18 12:30:58.000000 protopunica-0.14.8rc3/protopunica/distributions/DirichletDistribution.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)  1299521 2023-05-18 12:30:58.000000 protopunica-0.14.8rc3/protopunica/distributions/DiscreteDistribution.c
+-rw-r--r--   0 runner    (1001) docker     (123)      486 2023-05-18 12:30:58.000000 protopunica-0.14.8rc3/protopunica/distributions/DiscreteDistribution.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     9855 2023-05-18 12:30:58.000000 protopunica-0.14.8rc3/protopunica/distributions/DiscreteDistribution.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)   911061 2023-05-18 12:30:58.000000 protopunica-0.14.8rc3/protopunica/distributions/ExponentialDistribution.c
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-05-18 12:30:58.000000 protopunica-0.14.8rc3/protopunica/distributions/ExponentialDistribution.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     2511 2023-05-18 12:30:58.000000 protopunica-0.14.8rc3/protopunica/distributions/ExponentialDistribution.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)  1013935 2023-05-18 12:30:58.000000 protopunica-0.14.8rc3/protopunica/distributions/GammaDistribution.c
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-05-18 12:30:58.000000 protopunica-0.14.8rc3/protopunica/distributions/GammaDistribution.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     7928 2023-05-18 12:30:58.000000 protopunica-0.14.8rc3/protopunica/distributions/GammaDistribution.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)  1103415 2023-05-18 12:30:58.000000 protopunica-0.14.8rc3/protopunica/distributions/IndependentComponentsDistribution.c
+-rw-r--r--   0 runner    (1001) docker     (123)      474 2023-05-18 12:30:58.000000 protopunica-0.14.8rc3/protopunica/distributions/IndependentComponentsDistribution.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     7896 2023-05-18 12:30:58.000000 protopunica-0.14.8rc3/protopunica/distributions/IndependentComponentsDistribution.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)  1366877 2023-05-18 12:30:58.000000 protopunica-0.14.8rc3/protopunica/distributions/JointProbabilityTable.c
+-rw-r--r--   0 runner    (1001) docker     (123)      481 2023-05-18 12:30:58.000000 protopunica-0.14.8rc3/protopunica/distributions/JointProbabilityTable.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     8034 2023-05-18 12:30:58.000000 protopunica-0.14.8rc3/protopunica/distributions/JointProbabilityTable.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)  1060465 2023-05-18 12:30:58.000000 protopunica-0.14.8rc3/protopunica/distributions/KernelDensities.c
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-05-18 12:30:58.000000 protopunica-0.14.8rc3/protopunica/distributions/KernelDensities.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     8057 2023-05-18 12:30:58.000000 protopunica-0.14.8rc3/protopunica/distributions/KernelDensities.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)   927414 2023-05-18 12:30:58.000000 protopunica-0.14.8rc3/protopunica/distributions/LogNormalDistribution.c
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-05-18 12:30:58.000000 protopunica-0.14.8rc3/protopunica/distributions/LogNormalDistribution.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     3185 2023-05-18 12:30:58.000000 protopunica-0.14.8rc3/protopunica/distributions/LogNormalDistribution.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)  1118071 2023-05-18 12:30:58.000000 protopunica-0.14.8rc3/protopunica/distributions/MultivariateGaussianDistribution.c
+-rw-r--r--   0 runner    (1001) docker     (123)      676 2023-05-18 12:30:58.000000 protopunica-0.14.8rc3/protopunica/distributions/MultivariateGaussianDistribution.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     8814 2023-05-18 12:30:58.000000 protopunica-0.14.8rc3/protopunica/distributions/MultivariateGaussianDistribution.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)     5534 2023-05-18 12:30:58.000000 protopunica-0.14.8rc3/protopunica/distributions/NeuralNetworkWrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)   932572 2023-05-18 12:30:58.000000 protopunica-0.14.8rc3/protopunica/distributions/NormalDistribution.c
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-05-18 12:30:58.000000 protopunica-0.14.8rc3/protopunica/distributions/NormalDistribution.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     3134 2023-05-18 12:30:58.000000 protopunica-0.14.8rc3/protopunica/distributions/NormalDistribution.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)   910130 2023-05-18 12:30:58.000000 protopunica-0.14.8rc3/protopunica/distributions/PoissonDistribution.c
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-05-18 12:30:58.000000 protopunica-0.14.8rc3/protopunica/distributions/PoissonDistribution.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     2759 2023-05-18 12:30:58.000000 protopunica-0.14.8rc3/protopunica/distributions/PoissonDistribution.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)   928439 2023-05-18 12:30:58.000000 protopunica-0.14.8rc3/protopunica/distributions/UniformDistribution.c
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-05-18 12:30:58.000000 protopunica-0.14.8rc3/protopunica/distributions/UniformDistribution.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     2788 2023-05-18 12:30:58.000000 protopunica-0.14.8rc3/protopunica/distributions/UniformDistribution.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)     1215 2023-05-18 12:30:58.000000 protopunica-0.14.8rc3/protopunica/distributions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   551722 2023-05-18 12:30:58.000000 protopunica-0.14.8rc3/protopunica/distributions/distributions.c
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-05-18 12:30:58.000000 protopunica-0.14.8rc3/protopunica/distributions/distributions.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)    10029 2023-05-18 12:30:58.000000 protopunica-0.14.8rc3/protopunica/distributions/distributions.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)  1221029 2023-05-18 12:30:58.000000 protopunica-0.14.8rc3/protopunica/gmm.c
+-rw-r--r--   0 runner    (1001) docker     (123)    23761 2023-05-18 12:30:58.000000 protopunica-0.14.8rc3/protopunica/gmm.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)  2835749 2023-05-18 12:30:58.000000 protopunica-0.14.8rc3/protopunica/hmm.c
+-rw-r--r--   0 runner    (1001) docker     (123)   126627 2023-05-18 12:30:58.000000 protopunica-0.14.8rc3/protopunica/hmm.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)    12415 2023-05-18 12:30:58.000000 protopunica-0.14.8rc3/protopunica/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)  1374225 2023-05-18 12:30:58.000000 protopunica-0.14.8rc3/protopunica/kmeans.c
+-rw-r--r--   0 runner    (1001) docker     (123)    24982 2023-05-18 12:30:58.000000 protopunica-0.14.8rc3/protopunica/kmeans.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)   704735 2023-05-18 12:30:58.000000 protopunica-0.14.8rc3/protopunica/parallel.c
+-rw-r--r--   0 runner    (1001) docker     (123)    15976 2023-05-18 12:30:58.000000 protopunica-0.14.8rc3/protopunica/parallel.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)  1223513 2023-05-18 12:30:58.000000 protopunica-0.14.8rc3/protopunica/utils.c
+-rw-r--r--   0 runner    (1001) docker     (123)      745 2023-05-18 12:30:58.000000 protopunica-0.14.8rc3/protopunica/utils.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)    13248 2023-05-18 12:30:58.000000 protopunica-0.14.8rc3/protopunica/utils.pyx
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 12:31:07.516670 protopunica-0.14.8rc3/protopunica.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-05-18 12:31:07.000000 protopunica-0.14.8rc3/protopunica.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4589 2023-05-18 12:31:07.000000 protopunica-0.14.8rc3/protopunica.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 12:31:07.000000 protopunica-0.14.8rc3/protopunica.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 12:31:07.000000 protopunica-0.14.8rc3/protopunica.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-05-18 12:31:07.000000 protopunica-0.14.8rc3/protopunica.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-18 12:31:07.000000 protopunica-0.14.8rc3/protopunica.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-05-18 12:30:58.000000 protopunica-0.14.8rc3/pyproject.toml
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1840 2023-05-18 12:30:58.000000 protopunica-0.14.8rc3/rebuildconda
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-05-18 12:30:58.000000 protopunica-0.14.8rc3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-18 12:31:07.536670 protopunica-0.14.8rc3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3032 2023-05-18 12:30:58.000000 protopunica-0.14.8rc3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 12:31:07.536670 protopunica-0.14.8rc3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 12:30:58.000000 protopunica-0.14.8rc3/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23744 2023-05-18 12:30:58.000000 protopunica-0.14.8rc3/tests/test_bayes_classifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)    59630 2023-05-18 12:30:58.000000 protopunica-0.14.8rc3/tests/test_bayesian_network.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27669 2023-05-18 12:30:58.000000 protopunica-0.14.8rc3/tests/test_custom_distributions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45538 2023-05-18 12:30:58.000000 protopunica-0.14.8rc3/tests/test_distributions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1608 2023-05-18 12:30:58.000000 protopunica-0.14.8rc3/tests/test_factor_graphs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51403 2023-05-18 12:30:58.000000 protopunica-0.14.8rc3/tests/test_gmm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    81204 2023-05-18 12:30:58.000000 protopunica-0.14.8rc3/tests/test_hmm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23788 2023-05-18 12:30:58.000000 protopunica-0.14.8rc3/tests/test_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13746 2023-05-18 12:30:58.000000 protopunica-0.14.8rc3/tests/test_kmeans.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20298 2023-05-18 12:30:58.000000 protopunica-0.14.8rc3/tests/test_markov_chain.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18046 2023-05-18 12:30:58.000000 protopunica-0.14.8rc3/tests/test_markov_network.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30069 2023-05-18 12:30:58.000000 protopunica-0.14.8rc3/tests/test_naive_bayes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17863 2023-05-18 12:30:58.000000 protopunica-0.14.8rc3/tests/test_profile_hmm.py
```

### Comparing `protopunica-0.14.8rc2/.github/workflows/deploy.yml` & `protopunica-0.14.8rc3/.github/workflows/deploy.yml`

 * *Files identical despite different names*

### Comparing `protopunica-0.14.8rc2/.gitignore` & `protopunica-0.14.8rc3/.gitignore`

 * *Files identical despite different names*

### Comparing `protopunica-0.14.8rc2/LICENSE` & `protopunica-0.14.8rc3/LICENSE`

 * *Files identical despite different names*

### Comparing `protopunica-0.14.8rc2/Makefile` & `protopunica-0.14.8rc3/Makefile`

 * *Files identical despite different names*

### Comparing `protopunica-0.14.8rc2/examples/bayes_classifier_hmm_cheating_coin_toss.ipynb` & `protopunica-0.14.8rc3/examples/bayes_classifier_hmm_cheating_coin_toss.ipynb`

 * *Files identical despite different names*

### Comparing `protopunica-0.14.8rc2/examples/bayesnet_asia.ipynb` & `protopunica-0.14.8rc3/examples/bayesnet_asia.ipynb`

 * *Files identical despite different names*

### Comparing `protopunica-0.14.8rc2/examples/bayesnet_huge_monty_hall.ipynb` & `protopunica-0.14.8rc3/examples/bayesnet_huge_monty_hall.ipynb`

 * *Files identical despite different names*

### Comparing `protopunica-0.14.8rc2/examples/bayesnet_monty_hall_classic.ipynb` & `protopunica-0.14.8rc3/examples/bayesnet_monty_hall_classic.ipynb`

 * *Files identical despite different names*

### Comparing `protopunica-0.14.8rc2/examples/bayesnet_monty_hall_train.ipynb` & `protopunica-0.14.8rc3/examples/bayesnet_monty_hall_train.ipynb`

 * *Files identical despite different names*

### Comparing `protopunica-0.14.8rc2/examples/distributions_conditionalupdate.ipynb` & `protopunica-0.14.8rc3/examples/distributions_conditionalupdate.ipynb`

 * *Files identical despite different names*

### Comparing `protopunica-0.14.8rc2/examples/distributions_test_table.ipynb` & `protopunica-0.14.8rc3/examples/distributions_test_table.ipynb`

 * *Files identical despite different names*

### Comparing `protopunica-0.14.8rc2/examples/hmm_example.ipynb` & `protopunica-0.14.8rc3/examples/hmm_example.ipynb`

 * *Files identical despite different names*

### Comparing `protopunica-0.14.8rc2/examples/hmm_infinite.ipynb` & `protopunica-0.14.8rc3/examples/hmm_infinite.ipynb`

 * *Files identical despite different names*

### Comparing `protopunica-0.14.8rc2/examples/hmm_rainy_sunny.ipynb` & `protopunica-0.14.8rc3/examples/hmm_rainy_sunny.ipynb`

 * *Files identical despite different names*

### Comparing `protopunica-0.14.8rc2/examples/hmm_tied_states.ipynb` & `protopunica-0.14.8rc3/examples/hmm_tied_states.ipynb`

 * *Files identical despite different names*

### Comparing `protopunica-0.14.8rc2/examples/naivebayes_hmm_cheating_coin_toss.ipynb` & `protopunica-0.14.8rc3/examples/naivebayes_hmm_cheating_coin_toss.ipynb`

 * *Files identical despite different names*

### Comparing `protopunica-0.14.8rc2/examples/naivebayes_multivariate_male_female.ipynb` & `protopunica-0.14.8rc3/examples/naivebayes_multivariate_male_female.ipynb`

 * *Files identical despite different names*

### Comparing `protopunica-0.14.8rc2/examples/naivebayes_simple_male_female.ipynb` & `protopunica-0.14.8rc3/examples/naivebayes_simple_male_female.ipynb`

 * *Files identical despite different names*

### Comparing `protopunica-0.14.8rc2/protopunica/BayesClassifier.c` & `protopunica-0.14.8rc3/protopunica/BayesClassifier.c`

 * *Files identical despite different names*

### Comparing `protopunica-0.14.8rc2/protopunica/BayesClassifier.pyx` & `protopunica-0.14.8rc3/protopunica/BayesClassifier.pyx`

 * *Files identical despite different names*

### Comparing `protopunica-0.14.8rc2/protopunica/BayesianNetwork.c` & `protopunica-0.14.8rc3/protopunica/BayesianNetwork.c`

 * *Files identical despite different names*

### Comparing `protopunica-0.14.8rc2/protopunica/BayesianNetwork.pyx` & `protopunica-0.14.8rc3/protopunica/BayesianNetwork.pyx`

 * *Files identical despite different names*

### Comparing `protopunica-0.14.8rc2/protopunica/FactorGraph.c` & `protopunica-0.14.8rc3/protopunica/FactorGraph.c`

 * *Files identical despite different names*

### Comparing `protopunica-0.14.8rc2/protopunica/FactorGraph.pyx` & `protopunica-0.14.8rc3/protopunica/FactorGraph.pyx`

 * *Files identical despite different names*

### Comparing `protopunica-0.14.8rc2/protopunica/MarkovChain.c` & `protopunica-0.14.8rc3/protopunica/MarkovChain.c`

 * *Files identical despite different names*

### Comparing `protopunica-0.14.8rc2/protopunica/MarkovChain.pyx` & `protopunica-0.14.8rc3/protopunica/MarkovChain.pyx`

 * *Files identical despite different names*

### Comparing `protopunica-0.14.8rc2/protopunica/MarkovNetwork.c` & `protopunica-0.14.8rc3/protopunica/MarkovNetwork.c`

 * *Files identical despite different names*

### Comparing `protopunica-0.14.8rc2/protopunica/MarkovNetwork.pyx` & `protopunica-0.14.8rc3/protopunica/MarkovNetwork.pyx`

 * *Files identical despite different names*

### Comparing `protopunica-0.14.8rc2/protopunica/NaiveBayes.c` & `protopunica-0.14.8rc3/protopunica/NaiveBayes.c`

 * *Files identical despite different names*

### Comparing `protopunica-0.14.8rc2/protopunica/NaiveBayes.pyx` & `protopunica-0.14.8rc3/protopunica/NaiveBayes.pyx`

 * *Files identical despite different names*

### Comparing `protopunica-0.14.8rc2/protopunica/__init__.py` & `protopunica-0.14.8rc3/protopunica/__init__.py`

 * *Files identical despite different names*

### Comparing `protopunica-0.14.8rc2/protopunica/base.c` & `protopunica-0.14.8rc3/protopunica/base.c`

 * *Files identical despite different names*

### Comparing `protopunica-0.14.8rc2/protopunica/base.pxd` & `protopunica-0.14.8rc3/protopunica/base.pxd`

 * *Files identical despite different names*

### Comparing `protopunica-0.14.8rc2/protopunica/base.pyx` & `protopunica-0.14.8rc3/protopunica/base.pyx`

 * *Files identical despite different names*

### Comparing `protopunica-0.14.8rc2/protopunica/bayes.c` & `protopunica-0.14.8rc3/protopunica/bayes.c`

 * *Files identical despite different names*

### Comparing `protopunica-0.14.8rc2/protopunica/bayes.pxd` & `protopunica-0.14.8rc3/protopunica/bayes.pxd`

 * *Files identical despite different names*

### Comparing `protopunica-0.14.8rc2/protopunica/bayes.pyx` & `protopunica-0.14.8rc3/protopunica/bayes.pyx`

 * *Files identical despite different names*

### Comparing `protopunica-0.14.8rc2/protopunica/callbacks.py` & `protopunica-0.14.8rc3/protopunica/callbacks.py`

 * *Files identical despite different names*

### Comparing `protopunica-0.14.8rc2/protopunica/distributions/BernoulliDistribution.c` & `protopunica-0.14.8rc3/protopunica/distributions/BernoulliDistribution.c`

 * *Files identical despite different names*

### Comparing `protopunica-0.14.8rc2/protopunica/distributions/BernoulliDistribution.pyx` & `protopunica-0.14.8rc3/protopunica/distributions/BernoulliDistribution.pyx`

 * *Files identical despite different names*

### Comparing `protopunica-0.14.8rc2/protopunica/distributions/BetaDistribution.c` & `protopunica-0.14.8rc3/protopunica/distributions/BetaDistribution.c`

 * *Files identical despite different names*

### Comparing `protopunica-0.14.8rc2/protopunica/distributions/BetaDistribution.pyx` & `protopunica-0.14.8rc3/protopunica/distributions/BetaDistribution.pyx`

 * *Files identical despite different names*

### Comparing `protopunica-0.14.8rc2/protopunica/distributions/ConditionalProbabilityTable.c` & `protopunica-0.14.8rc3/protopunica/distributions/ConditionalProbabilityTable.c`

 * *Files identical despite different names*

### Comparing `protopunica-0.14.8rc2/protopunica/distributions/ConditionalProbabilityTable.pxd` & `protopunica-0.14.8rc3/protopunica/distributions/ConditionalProbabilityTable.pxd`

 * *Files identical despite different names*

### Comparing `protopunica-0.14.8rc2/protopunica/distributions/ConditionalProbabilityTable.pyx` & `protopunica-0.14.8rc3/protopunica/distributions/ConditionalProbabilityTable.pyx`

 * *Files identical despite different names*

### Comparing `protopunica-0.14.8rc2/protopunica/distributions/DirichletDistribution.c` & `protopunica-0.14.8rc3/protopunica/distributions/DirichletDistribution.c`

 * *Files identical despite different names*

### Comparing `protopunica-0.14.8rc2/protopunica/distributions/DirichletDistribution.pyx` & `protopunica-0.14.8rc3/protopunica/distributions/DirichletDistribution.pyx`

 * *Files identical despite different names*

### Comparing `protopunica-0.14.8rc2/protopunica/distributions/DiscreteDistribution.c` & `protopunica-0.14.8rc3/protopunica/distributions/DiscreteDistribution.c`

 * *Files identical despite different names*

### Comparing `protopunica-0.14.8rc2/protopunica/distributions/DiscreteDistribution.pyx` & `protopunica-0.14.8rc3/protopunica/distributions/DiscreteDistribution.pyx`

 * *Files identical despite different names*

### Comparing `protopunica-0.14.8rc2/protopunica/distributions/ExponentialDistribution.c` & `protopunica-0.14.8rc3/protopunica/distributions/ExponentialDistribution.c`

 * *Files identical despite different names*

### Comparing `protopunica-0.14.8rc2/protopunica/distributions/ExponentialDistribution.pyx` & `protopunica-0.14.8rc3/protopunica/distributions/ExponentialDistribution.pyx`

 * *Files identical despite different names*

### Comparing `protopunica-0.14.8rc2/protopunica/distributions/GammaDistribution.c` & `protopunica-0.14.8rc3/protopunica/distributions/GammaDistribution.c`

 * *Files identical despite different names*

### Comparing `protopunica-0.14.8rc2/protopunica/distributions/GammaDistribution.pyx` & `protopunica-0.14.8rc3/protopunica/distributions/GammaDistribution.pyx`

 * *Files identical despite different names*

### Comparing `protopunica-0.14.8rc2/protopunica/distributions/IndependentComponentsDistribution.c` & `protopunica-0.14.8rc3/protopunica/distributions/IndependentComponentsDistribution.c`

 * *Files identical despite different names*

### Comparing `protopunica-0.14.8rc2/protopunica/distributions/IndependentComponentsDistribution.pyx` & `protopunica-0.14.8rc3/protopunica/distributions/IndependentComponentsDistribution.pyx`

 * *Files identical despite different names*

### Comparing `protopunica-0.14.8rc2/protopunica/distributions/JointProbabilityTable.c` & `protopunica-0.14.8rc3/protopunica/distributions/JointProbabilityTable.c`

 * *Files identical despite different names*

### Comparing `protopunica-0.14.8rc2/protopunica/distributions/JointProbabilityTable.pyx` & `protopunica-0.14.8rc3/protopunica/distributions/JointProbabilityTable.pyx`

 * *Files identical despite different names*

### Comparing `protopunica-0.14.8rc2/protopunica/distributions/KernelDensities.c` & `protopunica-0.14.8rc3/protopunica/distributions/KernelDensities.c`

 * *Files identical despite different names*

### Comparing `protopunica-0.14.8rc2/protopunica/distributions/KernelDensities.pyx` & `protopunica-0.14.8rc3/protopunica/distributions/KernelDensities.pyx`

 * *Files identical despite different names*

### Comparing `protopunica-0.14.8rc2/protopunica/distributions/LogNormalDistribution.c` & `protopunica-0.14.8rc3/protopunica/distributions/LogNormalDistribution.c`

 * *Files identical despite different names*

### Comparing `protopunica-0.14.8rc2/protopunica/distributions/LogNormalDistribution.pyx` & `protopunica-0.14.8rc3/protopunica/distributions/LogNormalDistribution.pyx`

 * *Files identical despite different names*

### Comparing `protopunica-0.14.8rc2/protopunica/distributions/MultivariateGaussianDistribution.c` & `protopunica-0.14.8rc3/protopunica/distributions/MultivariateGaussianDistribution.c`

 * *Files identical despite different names*

### Comparing `protopunica-0.14.8rc2/protopunica/distributions/MultivariateGaussianDistribution.pxd` & `protopunica-0.14.8rc3/protopunica/distributions/MultivariateGaussianDistribution.pxd`

 * *Files identical despite different names*

### Comparing `protopunica-0.14.8rc2/protopunica/distributions/MultivariateGaussianDistribution.pyx` & `protopunica-0.14.8rc3/protopunica/distributions/MultivariateGaussianDistribution.pyx`

 * *Files identical despite different names*

### Comparing `protopunica-0.14.8rc2/protopunica/distributions/NeuralNetworkWrapper.py` & `protopunica-0.14.8rc3/protopunica/distributions/NeuralNetworkWrapper.py`

 * *Files identical despite different names*

### Comparing `protopunica-0.14.8rc2/protopunica/distributions/NormalDistribution.c` & `protopunica-0.14.8rc3/protopunica/distributions/NormalDistribution.c`

 * *Files identical despite different names*

### Comparing `protopunica-0.14.8rc2/protopunica/distributions/NormalDistribution.pyx` & `protopunica-0.14.8rc3/protopunica/distributions/NormalDistribution.pyx`

 * *Files identical despite different names*

### Comparing `protopunica-0.14.8rc2/protopunica/distributions/PoissonDistribution.c` & `protopunica-0.14.8rc3/protopunica/distributions/PoissonDistribution.c`

 * *Files identical despite different names*

### Comparing `protopunica-0.14.8rc2/protopunica/distributions/PoissonDistribution.pyx` & `protopunica-0.14.8rc3/protopunica/distributions/PoissonDistribution.pyx`

 * *Files identical despite different names*

### Comparing `protopunica-0.14.8rc2/protopunica/distributions/UniformDistribution.c` & `protopunica-0.14.8rc3/protopunica/distributions/UniformDistribution.c`

 * *Files identical despite different names*

### Comparing `protopunica-0.14.8rc2/protopunica/distributions/UniformDistribution.pyx` & `protopunica-0.14.8rc3/protopunica/distributions/UniformDistribution.pyx`

 * *Files identical despite different names*

### Comparing `protopunica-0.14.8rc2/protopunica/distributions/__init__.py` & `protopunica-0.14.8rc3/protopunica/distributions/__init__.py`

 * *Files identical despite different names*

### Comparing `protopunica-0.14.8rc2/protopunica/distributions/distributions.c` & `protopunica-0.14.8rc3/protopunica/distributions/distributions.c`

 * *Files identical despite different names*

### Comparing `protopunica-0.14.8rc2/protopunica/distributions/distributions.pyx` & `protopunica-0.14.8rc3/protopunica/distributions/distributions.pyx`

 * *Files identical despite different names*

### Comparing `protopunica-0.14.8rc2/protopunica/gmm.c` & `protopunica-0.14.8rc3/protopunica/gmm.c`

 * *Files identical despite different names*

### Comparing `protopunica-0.14.8rc2/protopunica/gmm.pyx` & `protopunica-0.14.8rc3/protopunica/gmm.pyx`

 * *Files identical despite different names*

### Comparing `protopunica-0.14.8rc2/protopunica/hmm.c` & `protopunica-0.14.8rc3/protopunica/hmm.c`

 * *Files identical despite different names*

### Comparing `protopunica-0.14.8rc2/protopunica/hmm.pyx` & `protopunica-0.14.8rc3/protopunica/hmm.pyx`

 * *Files identical despite different names*

### Comparing `protopunica-0.14.8rc2/protopunica/io.py` & `protopunica-0.14.8rc3/protopunica/io.py`

 * *Files identical despite different names*

### Comparing `protopunica-0.14.8rc2/protopunica/kmeans.c` & `protopunica-0.14.8rc3/protopunica/kmeans.c`

 * *Files identical despite different names*

### Comparing `protopunica-0.14.8rc2/protopunica/kmeans.pyx` & `protopunica-0.14.8rc3/protopunica/kmeans.pyx`

 * *Files identical despite different names*

### Comparing `protopunica-0.14.8rc2/protopunica/parallel.c` & `protopunica-0.14.8rc3/protopunica/parallel.c`

 * *Files identical despite different names*

### Comparing `protopunica-0.14.8rc2/protopunica/parallel.pyx` & `protopunica-0.14.8rc3/protopunica/parallel.pyx`

 * *Files identical despite different names*

### Comparing `protopunica-0.14.8rc2/protopunica/utils.c` & `protopunica-0.14.8rc3/protopunica/utils.c`

 * *Files identical despite different names*

### Comparing `protopunica-0.14.8rc2/protopunica/utils.pxd` & `protopunica-0.14.8rc3/protopunica/utils.pxd`

 * *Files identical despite different names*

### Comparing `protopunica-0.14.8rc2/protopunica/utils.pyx` & `protopunica-0.14.8rc3/protopunica/utils.pyx`

 * *Files identical despite different names*

### Comparing `protopunica-0.14.8rc2/protopunica.egg-info/SOURCES.txt` & `protopunica-0.14.8rc3/protopunica.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `protopunica-0.14.8rc2/rebuildconda` & `protopunica-0.14.8rc3/rebuildconda`

 * *Files identical despite different names*

### Comparing `protopunica-0.14.8rc2/setup.py` & `protopunica-0.14.8rc3/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -62,37 +62,35 @@
 
 class build_ext(_build_ext):
     def finalize_options(self):
         _build_ext.finalize_options(self)
         # Prevent numpy from thinking it is still in its setup process:
         if hasattr(__builtins__, '__NUMPY_SETUP__'):
             __builtins__.__NUMPY_SETUP__ = False
-        import numpy
-        self.include_dirs.append(numpy.get_include())
+        try:
+            import numpy
+            self.include_dirs.append(numpy.get_include())
+        except ImportError:
+            pass
 
 setup(
     name='protopunica',
-    version='0.14.8rc2',
+    version='0.14.8rc3',
     author='Jacob Schreiber',
     author_email='jmschreiber91@gmail.com',
     packages=[
         'protopunica',
         'protopunica/distributions',
     ],
     url='http://pypi.python.org/pypi/protopunica/',
     license='MIT',
     description='Protopunica is pomegranate frozen at version 0.14.8.',
     long_description='Protopunica is pomegranate frozen at version 0.14.8.',
     ext_modules=extensions,
     cmdclass={'build_ext':build_ext},
-    setup_requires=[
-        "cython >= 0.22.1",
-        "numpy >= 1.20.0",
-        "scipy >= 0.17.0"
-    ],
     install_requires=[
         "numpy >= 1.20.0",
         "joblib >= 0.9.0b4",
         "networkx >= 2.4",
         "scipy >= 0.17.0",
         "pyyaml"
     ],
```

### Comparing `protopunica-0.14.8rc2/tests/test_bayes_classifier.py` & `protopunica-0.14.8rc3/tests/test_bayes_classifier.py`

 * *Files identical despite different names*

### Comparing `protopunica-0.14.8rc2/tests/test_bayesian_network.py` & `protopunica-0.14.8rc3/tests/test_bayesian_network.py`

 * *Files identical despite different names*

### Comparing `protopunica-0.14.8rc2/tests/test_custom_distributions.py` & `protopunica-0.14.8rc3/tests/test_custom_distributions.py`

 * *Files identical despite different names*

### Comparing `protopunica-0.14.8rc2/tests/test_distributions.py` & `protopunica-0.14.8rc3/tests/test_distributions.py`

 * *Files identical despite different names*

### Comparing `protopunica-0.14.8rc2/tests/test_factor_graphs.py` & `protopunica-0.14.8rc3/tests/test_factor_graphs.py`

 * *Files identical despite different names*

### Comparing `protopunica-0.14.8rc2/tests/test_gmm.py` & `protopunica-0.14.8rc3/tests/test_gmm.py`

 * *Files identical despite different names*

### Comparing `protopunica-0.14.8rc2/tests/test_hmm.py` & `protopunica-0.14.8rc3/tests/test_hmm.py`

 * *Files identical despite different names*

### Comparing `protopunica-0.14.8rc2/tests/test_io.py` & `protopunica-0.14.8rc3/tests/test_io.py`

 * *Files identical despite different names*

### Comparing `protopunica-0.14.8rc2/tests/test_kmeans.py` & `protopunica-0.14.8rc3/tests/test_kmeans.py`

 * *Files identical despite different names*

### Comparing `protopunica-0.14.8rc2/tests/test_markov_chain.py` & `protopunica-0.14.8rc3/tests/test_markov_chain.py`

 * *Files identical despite different names*

### Comparing `protopunica-0.14.8rc2/tests/test_markov_network.py` & `protopunica-0.14.8rc3/tests/test_markov_network.py`

 * *Files identical despite different names*

### Comparing `protopunica-0.14.8rc2/tests/test_naive_bayes.py` & `protopunica-0.14.8rc3/tests/test_naive_bayes.py`

 * *Files identical despite different names*

### Comparing `protopunica-0.14.8rc2/tests/test_profile_hmm.py` & `protopunica-0.14.8rc3/tests/test_profile_hmm.py`

 * *Files identical despite different names*

