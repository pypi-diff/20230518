# Comparing `tmp/sfr-pyrca-0.0.1.tar.gz` & `tmp/sfr-pyrca-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sfr-pyrca-0.0.1.tar", last modified: Thu Apr 27 06:55:33 2023, max compression
+gzip compressed data, was "sfr-pyrca-1.0.0.tar", last modified: Thu May 18 06:29:27 2023, max compression
```

## Comparing `sfr-pyrca-0.0.1.tar` & `sfr-pyrca-1.0.0.tar`

### file list

```diff
@@ -1,218 +1,219 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 06:55:33.774021 sfr-pyrca-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-04-27 06:55:22.000000 sfr-pyrca-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    13687 2023-04-27 06:55:33.774021 sfr-pyrca-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13297 2023-04-27 06:55:22.000000 sfr-pyrca-0.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 06:55:33.746021 sfr-pyrca-0.0.1/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     3377 2023-04-27 06:55:22.000000 sfr-pyrca-0.0.1/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 06:55:33.746021 sfr-pyrca-0.0.1/pyrca/
--rw-r--r--   0 runner    (1001) docker     (123)      452 2023-04-27 06:55:22.000000 sfr-pyrca-0.0.1/pyrca/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 06:55:33.750021 sfr-pyrca-0.0.1/pyrca/analyzers/
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-04-27 06:55:22.000000 sfr-pyrca-0.0.1/pyrca/analyzers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-04-27 06:55:22.000000 sfr-pyrca-0.0.1/pyrca/analyzers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    19350 2023-04-27 06:55:22.000000 sfr-pyrca-0.0.1/pyrca/analyzers/bayesian.py
--rw-r--r--   0 runner    (1001) docker     (123)     3758 2023-04-27 06:55:22.000000 sfr-pyrca-0.0.1/pyrca/analyzers/epsilon_diagnosis.py
--rw-r--r--   0 runner    (1001) docker     (123)     6335 2023-04-27 06:55:22.000000 sfr-pyrca-0.0.1/pyrca/analyzers/ht.py
--rw-r--r--   0 runner    (1001) docker     (123)     9957 2023-04-27 06:55:22.000000 sfr-pyrca-0.0.1/pyrca/analyzers/random_walk.py
--rw-r--r--   0 runner    (1001) docker     (123)     2288 2023-04-27 06:55:22.000000 sfr-pyrca-0.0.1/pyrca/analyzers/rcd.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 06:55:33.742021 sfr-pyrca-0.0.1/pyrca/applications/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 06:55:33.750021 sfr-pyrca-0.0.1/pyrca/applications/example/
--rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-04-27 06:55:22.000000 sfr-pyrca-0.0.1/pyrca/applications/example/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    10317 2023-04-27 06:55:22.000000 sfr-pyrca-0.0.1/pyrca/applications/example/rca.py
--rw-r--r--   0 runner    (1001) docker     (123)     4340 2023-04-27 06:55:22.000000 sfr-pyrca-0.0.1/pyrca/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 06:55:33.750021 sfr-pyrca-0.0.1/pyrca/graphs/
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-04-27 06:55:22.000000 sfr-pyrca-0.0.1/pyrca/graphs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 06:55:33.750021 sfr-pyrca-0.0.1/pyrca/graphs/causal/
--rw-r--r--   0 runner    (1001) docker     (123)      455 2023-04-27 06:55:22.000000 sfr-pyrca-0.0.1/pyrca/graphs/causal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11232 2023-04-27 06:55:22.000000 sfr-pyrca-0.0.1/pyrca/graphs/causal/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3786 2023-04-27 06:55:22.000000 sfr-pyrca-0.0.1/pyrca/graphs/causal/fges.py
--rw-r--r--   0 runner    (1001) docker     (123)     3231 2023-04-27 06:55:22.000000 sfr-pyrca-0.0.1/pyrca/graphs/causal/ges.py
--rw-r--r--   0 runner    (1001) docker     (123)     2924 2023-04-27 06:55:22.000000 sfr-pyrca-0.0.1/pyrca/graphs/causal/lingam.py
--rw-r--r--   0 runner    (1001) docker     (123)     2762 2023-04-27 06:55:22.000000 sfr-pyrca-0.0.1/pyrca/graphs/causal/pc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 06:55:33.750021 sfr-pyrca-0.0.1/pyrca/outliers/
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-04-27 06:55:22.000000 sfr-pyrca-0.0.1/pyrca/outliers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5500 2023-04-27 06:55:22.000000 sfr-pyrca-0.0.1/pyrca/outliers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     8130 2023-04-27 06:55:22.000000 sfr-pyrca-0.0.1/pyrca/outliers/stats.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 06:55:33.750021 sfr-pyrca-0.0.1/pyrca/simulation/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 06:55:22.000000 sfr-pyrca-0.0.1/pyrca/simulation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13951 2023-04-27 06:55:22.000000 sfr-pyrca-0.0.1/pyrca/simulation/data_gen.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 06:55:33.750021 sfr-pyrca-0.0.1/pyrca/thirdparty/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 06:55:22.000000 sfr-pyrca-0.0.1/pyrca/thirdparty/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 06:55:33.742021 sfr-pyrca-0.0.1/pyrca/thirdparty/causallearn/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 06:55:33.754021 sfr-pyrca-0.0.1/pyrca/thirdparty/causallearn/graph/
--rw-r--r--   0 runner    (1001) docker     (123)     1660 2023-04-27 06:55:22.000000 sfr-pyrca-0.0.1/pyrca/thirdparty/causallearn/graph/AdjacencyConfusion.py
--rw-r--r--   0 runner    (1001) docker     (123)     3704 2023-04-27 06:55:22.000000 sfr-pyrca-0.0.1/pyrca/thirdparty/causallearn/graph/ArrowConfusion.py
--rw-r--r--   0 runner    (1001) docker     (123)    25550 2023-04-27 06:55:22.000000 sfr-pyrca-0.0.1/pyrca/thirdparty/causallearn/graph/Dag.py
--rw-r--r--   0 runner    (1001) docker     (123)     8532 2023-04-27 06:55:22.000000 sfr-pyrca-0.0.1/pyrca/thirdparty/causallearn/graph/Edge.py
--rw-r--r--   0 runner    (1001) docker     (123)     2657 2023-04-27 06:55:22.000000 sfr-pyrca-0.0.1/pyrca/thirdparty/causallearn/graph/Edges.py
--rw-r--r--   0 runner    (1001) docker     (123)      537 2023-04-27 06:55:22.000000 sfr-pyrca-0.0.1/pyrca/thirdparty/causallearn/graph/Endpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)    37979 2023-04-27 06:55:22.000000 sfr-pyrca-0.0.1/pyrca/thirdparty/causallearn/graph/GeneralGraph.py
--rw-r--r--   0 runner    (1001) docker     (123)    18680 2023-04-27 06:55:22.000000 sfr-pyrca-0.0.1/pyrca/thirdparty/causallearn/graph/Graph.py
--rw-r--r--   0 runner    (1001) docker     (123)     8872 2023-04-27 06:55:22.000000 sfr-pyrca-0.0.1/pyrca/thirdparty/causallearn/graph/GraphClass.py
--rw-r--r--   0 runner    (1001) docker     (123)     2754 2023-04-27 06:55:22.000000 sfr-pyrca-0.0.1/pyrca/thirdparty/causallearn/graph/GraphNode.py
--rw-r--r--   0 runner    (1001) docker     (123)     2056 2023-04-27 06:55:22.000000 sfr-pyrca-0.0.1/pyrca/thirdparty/causallearn/graph/Node.py
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-04-27 06:55:22.000000 sfr-pyrca-0.0.1/pyrca/thirdparty/causallearn/graph/NodeType.py
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-04-27 06:55:22.000000 sfr-pyrca-0.0.1/pyrca/thirdparty/causallearn/graph/NodeVariableType.py
--rw-r--r--   0 runner    (1001) docker     (123)     2068 2023-04-27 06:55:22.000000 sfr-pyrca-0.0.1/pyrca/thirdparty/causallearn/graph/SHD.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 06:55:33.754021 sfr-pyrca-0.0.1/pyrca/thirdparty/causallearn/score/
--rw-r--r--   0 runner    (1001) docker     (123)    30361 2023-04-27 06:55:22.000000 sfr-pyrca-0.0.1/pyrca/thirdparty/causallearn/score/LocalScoreFunction.py
--rw-r--r--   0 runner    (1001) docker     (123)     1551 2023-04-27 06:55:22.000000 sfr-pyrca-0.0.1/pyrca/thirdparty/causallearn/score/LocalScoreFunctionClass.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 06:55:33.742021 sfr-pyrca-0.0.1/pyrca/thirdparty/causallearn/search/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 06:55:33.754021 sfr-pyrca-0.0.1/pyrca/thirdparty/causallearn/search/ConstraintBased/
--rw-r--r--   0 runner    (1001) docker     (123)    20748 2023-04-27 06:55:22.000000 sfr-pyrca-0.0.1/pyrca/thirdparty/causallearn/search/ConstraintBased/PC.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 06:55:33.754021 sfr-pyrca-0.0.1/pyrca/thirdparty/causallearn/search/ScoreBased/
--rw-r--r--   0 runner    (1001) docker     (123)    15122 2023-04-27 06:55:22.000000 sfr-pyrca-0.0.1/pyrca/thirdparty/causallearn/search/ScoreBased/GES.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 06:55:33.754021 sfr-pyrca-0.0.1/pyrca/thirdparty/causallearn/utils/
--rw-r--r--   0 runner    (1001) docker     (123)    13321 2023-04-27 06:55:22.000000 sfr-pyrca-0.0.1/pyrca/thirdparty/causallearn/utils/BackgroundKnowledge.py
--rw-r--r--   0 runner    (1001) docker     (123)     4891 2023-04-27 06:55:22.000000 sfr-pyrca-0.0.1/pyrca/thirdparty/causallearn/utils/DAG2CPDAG.py
--rw-r--r--   0 runner    (1001) docker     (123)    17718 2023-04-27 06:55:22.000000 sfr-pyrca-0.0.1/pyrca/thirdparty/causallearn/utils/GESUtils.py
--rw-r--r--   0 runner    (1001) docker     (123)    16983 2023-04-27 06:55:22.000000 sfr-pyrca-0.0.1/pyrca/thirdparty/causallearn/utils/GraphUtils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 06:55:33.758021 sfr-pyrca-0.0.1/pyrca/thirdparty/causallearn/utils/PCUtils/
--rw-r--r--   0 runner    (1001) docker     (123)     1956 2023-04-27 06:55:22.000000 sfr-pyrca-0.0.1/pyrca/thirdparty/causallearn/utils/PCUtils/BackgroundKnowledgeOrientUtils.py
--rw-r--r--   0 runner    (1001) docker     (123)    28855 2023-04-27 06:55:22.000000 sfr-pyrca-0.0.1/pyrca/thirdparty/causallearn/utils/PCUtils/Helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     9196 2023-04-27 06:55:22.000000 sfr-pyrca-0.0.1/pyrca/thirdparty/causallearn/utils/PCUtils/Meek.py
--rw-r--r--   0 runner    (1001) docker     (123)     5702 2023-04-27 06:55:22.000000 sfr-pyrca-0.0.1/pyrca/thirdparty/causallearn/utils/PCUtils/SkeletonDiscovery.py
--rw-r--r--   0 runner    (1001) docker     (123)    18852 2023-04-27 06:55:22.000000 sfr-pyrca-0.0.1/pyrca/thirdparty/causallearn/utils/PCUtils/UCSepset.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 06:55:22.000000 sfr-pyrca-0.0.1/pyrca/thirdparty/causallearn/utils/PCUtils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2586 2023-04-27 06:55:22.000000 sfr-pyrca-0.0.1/pyrca/thirdparty/causallearn/utils/PDAG2DAG.py
--rw-r--r--   0 runner    (1001) docker     (123)    28846 2023-04-27 06:55:22.000000 sfr-pyrca-0.0.1/pyrca/thirdparty/causallearn/utils/ScoreUtils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1947 2023-04-27 06:55:22.000000 sfr-pyrca-0.0.1/pyrca/thirdparty/causallearn/utils/TXT2GeneralGraph.py
--rw-r--r--   0 runner    (1001) docker     (123)    23583 2023-04-27 06:55:22.000000 sfr-pyrca-0.0.1/pyrca/thirdparty/causallearn/utils/cit.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 06:55:33.758021 sfr-pyrca-0.0.1/pyrca/thirdparty/pgmpy/
--rwxr-xr-x   0 runner    (1001) docker     (123)      116 2023-04-27 06:55:22.000000 sfr-pyrca-0.0.1/pyrca/thirdparty/pgmpy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 06:55:33.758021 sfr-pyrca-0.0.1/pyrca/thirdparty/pgmpy/base/
--rwxr-xr-x   0 runner    (1001) docker     (123)    40652 2023-04-27 06:55:22.000000 sfr-pyrca-0.0.1/pyrca/thirdparty/pgmpy/base/DAG.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     9236 2023-04-27 06:55:22.000000 sfr-pyrca-0.0.1/pyrca/thirdparty/pgmpy/base/UndirectedGraph.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      118 2023-04-27 06:55:22.000000 sfr-pyrca-0.0.1/pyrca/thirdparty/pgmpy/base/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 06:55:33.758021 sfr-pyrca-0.0.1/pyrca/thirdparty/pgmpy/estimators/
--rwxr-xr-x   0 runner    (1001) docker     (123)     9735 2023-04-27 06:55:22.000000 sfr-pyrca-0.0.1/pyrca/thirdparty/pgmpy/estimators/BayesianEstimator.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7542 2023-04-27 06:55:22.000000 sfr-pyrca-0.0.1/pyrca/thirdparty/pgmpy/estimators/MLE.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      302 2023-04-27 06:55:22.000000 sfr-pyrca-0.0.1/pyrca/thirdparty/pgmpy/estimators/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    12198 2023-04-27 06:55:22.000000 sfr-pyrca-0.0.1/pyrca/thirdparty/pgmpy/estimators/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 06:55:33.758021 sfr-pyrca-0.0.1/pyrca/thirdparty/pgmpy/extern/
--rwxr-xr-x   0 runner    (1001) docker     (123)       55 2023-04-27 06:55:22.000000 sfr-pyrca-0.0.1/pyrca/thirdparty/pgmpy/extern/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    30221 2023-04-27 06:55:22.000000 sfr-pyrca-0.0.1/pyrca/thirdparty/pgmpy/extern/tabulate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 06:55:33.758021 sfr-pyrca-0.0.1/pyrca/thirdparty/pgmpy/factors/
--rwxr-xr-x   0 runner    (1001) docker     (123)    15811 2023-04-27 06:55:22.000000 sfr-pyrca-0.0.1/pyrca/thirdparty/pgmpy/factors/FactorSet.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      242 2023-04-27 06:55:22.000000 sfr-pyrca-0.0.1/pyrca/thirdparty/pgmpy/factors/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3131 2023-04-27 06:55:22.000000 sfr-pyrca-0.0.1/pyrca/thirdparty/pgmpy/factors/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 06:55:33.758021 sfr-pyrca-0.0.1/pyrca/thirdparty/pgmpy/factors/continuous/
--rwxr-xr-x   0 runner    (1001) docker     (123)    13912 2023-04-27 06:55:22.000000 sfr-pyrca-0.0.1/pyrca/thirdparty/pgmpy/factors/continuous/ContinuousFactor.py
--rwxr-xr-x   0 runner    (1001) docker     (123)       86 2023-04-27 06:55:22.000000 sfr-pyrca-0.0.1/pyrca/thirdparty/pgmpy/factors/continuous/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 06:55:33.762021 sfr-pyrca-0.0.1/pyrca/thirdparty/pgmpy/factors/discrete/
--rwxr-xr-x   0 runner    (1001) docker     (123)    22540 2023-04-27 06:55:22.000000 sfr-pyrca-0.0.1/pyrca/thirdparty/pgmpy/factors/discrete/CPD.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    35423 2023-04-27 06:55:22.000000 sfr-pyrca-0.0.1/pyrca/thirdparty/pgmpy/factors/discrete/DiscreteFactor.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    15809 2023-04-27 06:55:22.000000 sfr-pyrca-0.0.1/pyrca/thirdparty/pgmpy/factors/discrete/JointProbabilityDistribution.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      202 2023-04-27 06:55:22.000000 sfr-pyrca-0.0.1/pyrca/thirdparty/pgmpy/factors/discrete/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 06:55:33.762021 sfr-pyrca-0.0.1/pyrca/thirdparty/pgmpy/factors/distributions/
--rwxr-xr-x   0 runner    (1001) docker     (123)    18453 2023-04-27 06:55:22.000000 sfr-pyrca-0.0.1/pyrca/thirdparty/pgmpy/factors/distributions/CustomDistribution.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    19793 2023-04-27 06:55:22.000000 sfr-pyrca-0.0.1/pyrca/thirdparty/pgmpy/factors/distributions/GaussianDistribution.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      220 2023-04-27 06:55:22.000000 sfr-pyrca-0.0.1/pyrca/thirdparty/pgmpy/factors/distributions/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      841 2023-04-27 06:55:22.000000 sfr-pyrca-0.0.1/pyrca/thirdparty/pgmpy/factors/distributions/base.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      830 2023-04-27 06:55:22.000000 sfr-pyrca-0.0.1/pyrca/thirdparty/pgmpy/global_vars.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 06:55:33.762021 sfr-pyrca-0.0.1/pyrca/thirdparty/pgmpy/independencies/
--rwxr-xr-x   0 runner    (1001) docker     (123)    16265 2023-04-27 06:55:22.000000 sfr-pyrca-0.0.1/pyrca/thirdparty/pgmpy/independencies/Independencies.py
--rwxr-xr-x   0 runner    (1001) docker     (123)        1 2023-04-27 06:55:22.000000 sfr-pyrca-0.0.1/pyrca/thirdparty/pgmpy/independencies/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 06:55:33.762021 sfr-pyrca-0.0.1/pyrca/thirdparty/pgmpy/inference/
--rwxr-xr-x   0 runner    (1001) docker     (123)     5986 2023-04-27 06:55:22.000000 sfr-pyrca-0.0.1/pyrca/thirdparty/pgmpy/inference/EliminationOrder.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    44473 2023-04-27 06:55:22.000000 sfr-pyrca-0.0.1/pyrca/thirdparty/pgmpy/inference/ExactInference.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      135 2023-04-27 06:55:22.000000 sfr-pyrca-0.0.1/pyrca/thirdparty/pgmpy/inference/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     8926 2023-04-27 06:55:22.000000 sfr-pyrca-0.0.1/pyrca/thirdparty/pgmpy/inference/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 06:55:33.762021 sfr-pyrca-0.0.1/pyrca/thirdparty/pgmpy/models/
--rwxr-xr-x   0 runner    (1001) docker     (123)    35116 2023-04-27 06:55:22.000000 sfr-pyrca-0.0.1/pyrca/thirdparty/pgmpy/models/BayesianModel.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    12668 2023-04-27 06:55:22.000000 sfr-pyrca-0.0.1/pyrca/thirdparty/pgmpy/models/ClusterGraph.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    25489 2023-04-27 06:55:22.000000 sfr-pyrca-0.0.1/pyrca/thirdparty/pgmpy/models/DynamicBayesianNetwork.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    17153 2023-04-27 06:55:22.000000 sfr-pyrca-0.0.1/pyrca/thirdparty/pgmpy/models/FactorGraph.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4302 2023-04-27 06:55:22.000000 sfr-pyrca-0.0.1/pyrca/thirdparty/pgmpy/models/JunctionTree.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    29581 2023-04-27 06:55:22.000000 sfr-pyrca-0.0.1/pyrca/thirdparty/pgmpy/models/MarkovModel.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      250 2023-04-27 06:55:22.000000 sfr-pyrca-0.0.1/pyrca/thirdparty/pgmpy/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 06:55:33.766021 sfr-pyrca-0.0.1/pyrca/thirdparty/pgmpy/readwrite/
--rwxr-xr-x   0 runner    (1001) docker     (123)    22279 2023-04-27 06:55:22.000000 sfr-pyrca-0.0.1/pyrca/thirdparty/pgmpy/readwrite/BIF.py
--rwxr-xr-x   0 runner    (1001) docker     (123)       87 2023-04-27 06:55:22.000000 sfr-pyrca-0.0.1/pyrca/thirdparty/pgmpy/readwrite/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 06:55:33.766021 sfr-pyrca-0.0.1/pyrca/thirdparty/pgmpy/utils/
--rwxr-xr-x   0 runner    (1001) docker     (123)       77 2023-04-27 06:55:22.000000 sfr-pyrca-0.0.1/pyrca/thirdparty/pgmpy/utils/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      301 2023-04-27 06:55:22.000000 sfr-pyrca-0.0.1/pyrca/thirdparty/pgmpy/utils/decorators.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3675 2023-04-27 06:55:22.000000 sfr-pyrca-0.0.1/pyrca/thirdparty/pgmpy/utils/state_name.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 06:55:33.766021 sfr-pyrca-0.0.1/pyrca/thirdparty/pycausal/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 06:55:22.000000 sfr-pyrca-0.0.1/pyrca/thirdparty/pycausal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2413 2023-04-27 06:55:22.000000 sfr-pyrca-0.0.1/pyrca/thirdparty/pycausal/prior.py
--rw-r--r--   0 runner    (1001) docker     (123)    10528 2023-04-27 06:55:22.000000 sfr-pyrca-0.0.1/pyrca/thirdparty/pycausal/pycausal.py
--rw-r--r--   0 runner    (1001) docker     (123)    20120 2023-04-27 06:55:22.000000 sfr-pyrca-0.0.1/pyrca/thirdparty/pycausal/search.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 06:55:33.766021 sfr-pyrca-0.0.1/pyrca/thirdparty/rcd/
--rw-r--r--   0 runner    (1001) docker     (123)     6701 2023-04-27 06:55:22.000000 sfr-pyrca-0.0.1/pyrca/thirdparty/rcd/rcd.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 06:55:33.766021 sfr-pyrca-0.0.1/pyrca/thirdparty/rcd/utils/
--rw-r--r--   0 runner    (1001) docker     (123)    10362 2023-04-27 06:55:22.000000 sfr-pyrca-0.0.1/pyrca/thirdparty/rcd/utils/GraphClass.py
--rw-r--r--   0 runner    (1001) docker     (123)     8081 2023-04-27 06:55:22.000000 sfr-pyrca-0.0.1/pyrca/thirdparty/rcd/utils/SkeletonDiscovery.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 06:55:33.766021 sfr-pyrca-0.0.1/pyrca/tools/
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-04-27 06:55:22.000000 sfr-pyrca-0.0.1/pyrca/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      327 2023-04-27 06:55:22.000000 sfr-pyrca-0.0.1/pyrca/tools/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      349 2023-04-27 06:55:22.000000 sfr-pyrca-0.0.1/pyrca/tools/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 06:55:33.766021 sfr-pyrca-0.0.1/pyrca/tools/dashboard/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 06:55:33.770022 sfr-pyrca-0.0.1/pyrca/tools/dashboard/assets/
--rwxr-xr-x   0 runner    (1001) docker     (123)    83784 2023-04-27 06:55:22.000000 sfr-pyrca-0.0.1/pyrca/tools/dashboard/assets/Acumin-BdPro.otf
--rw-r--r--   0 runner    (1001) docker     (123)    12207 2023-04-27 06:55:22.000000 sfr-pyrca-0.0.1/pyrca/tools/dashboard/assets/base.css
--rw-r--r--   0 runner    (1001) docker     (123)     5354 2023-04-27 06:55:22.000000 sfr-pyrca-0.0.1/pyrca/tools/dashboard/assets/logo.png
--rw-r--r--   0 runner    (1001) docker     (123)     6085 2023-04-27 06:55:22.000000 sfr-pyrca-0.0.1/pyrca/tools/dashboard/assets/modal.css
--rw-r--r--   0 runner    (1001) docker     (123)     2684 2023-04-27 06:55:22.000000 sfr-pyrca-0.0.1/pyrca/tools/dashboard/assets/rca.css
--rw-r--r--   0 runner    (1001) docker     (123)      292 2023-04-27 06:55:22.000000 sfr-pyrca-0.0.1/pyrca/tools/dashboard/assets/resizing.js
--rw-r--r--   0 runner    (1001) docker     (123)      981 2023-04-27 06:55:22.000000 sfr-pyrca-0.0.1/pyrca/tools/dashboard/assets/styles.css
--rw-r--r--   0 runner    (1001) docker     (123)      714 2023-04-27 06:55:22.000000 sfr-pyrca-0.0.1/pyrca/tools/dashboard/assets/upload.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 06:55:33.770022 sfr-pyrca-0.0.1/pyrca/tools/dashboard/callbacks/
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-04-27 06:55:22.000000 sfr-pyrca-0.0.1/pyrca/tools/dashboard/callbacks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14449 2023-04-27 06:55:22.000000 sfr-pyrca-0.0.1/pyrca/tools/dashboard/callbacks/causal.py
--rw-r--r--   0 runner    (1001) docker     (123)     5386 2023-04-27 06:55:22.000000 sfr-pyrca-0.0.1/pyrca/tools/dashboard/callbacks/data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1593 2023-04-27 06:55:22.000000 sfr-pyrca-0.0.1/pyrca/tools/dashboard/dashboard.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 06:55:33.770022 sfr-pyrca-0.0.1/pyrca/tools/dashboard/models/
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-04-27 06:55:22.000000 sfr-pyrca-0.0.1/pyrca/tools/dashboard/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8523 2023-04-27 06:55:22.000000 sfr-pyrca-0.0.1/pyrca/tools/dashboard/models/causal.py
--rw-r--r--   0 runner    (1001) docker     (123)     2576 2023-04-27 06:55:22.000000 sfr-pyrca-0.0.1/pyrca/tools/dashboard/models/data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 06:55:33.770022 sfr-pyrca-0.0.1/pyrca/tools/dashboard/pages/
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-04-27 06:55:22.000000 sfr-pyrca-0.0.1/pyrca/tools/dashboard/pages/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14014 2023-04-27 06:55:22.000000 sfr-pyrca-0.0.1/pyrca/tools/dashboard/pages/causal.py
--rw-r--r--   0 runner    (1001) docker     (123)     7029 2023-04-27 06:55:22.000000 sfr-pyrca-0.0.1/pyrca/tools/dashboard/pages/data.py
--rw-r--r--   0 runner    (1001) docker     (123)     3102 2023-04-27 06:55:22.000000 sfr-pyrca-0.0.1/pyrca/tools/dashboard/pages/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      295 2023-04-27 06:55:22.000000 sfr-pyrca-0.0.1/pyrca/tools/dashboard/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 06:55:33.770022 sfr-pyrca-0.0.1/pyrca/tools/dashboard/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-04-27 06:55:22.000000 sfr-pyrca-0.0.1/pyrca/tools/dashboard/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2750 2023-04-27 06:55:22.000000 sfr-pyrca-0.0.1/pyrca/tools/dashboard/utils/file_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1441 2023-04-27 06:55:22.000000 sfr-pyrca-0.0.1/pyrca/tools/dashboard/utils/layout.py
--rw-r--r--   0 runner    (1001) docker     (123)      625 2023-04-27 06:55:22.000000 sfr-pyrca-0.0.1/pyrca/tools/dashboard/utils/log.py
--rw-r--r--   0 runner    (1001) docker     (123)     2774 2023-04-27 06:55:22.000000 sfr-pyrca-0.0.1/pyrca/tools/dashboard/utils/plot.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 06:55:33.770022 sfr-pyrca-0.0.1/pyrca/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-04-27 06:55:22.000000 sfr-pyrca-0.0.1/pyrca/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3529 2023-04-27 06:55:22.000000 sfr-pyrca-0.0.1/pyrca/utils/domain.py
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-04-27 06:55:22.000000 sfr-pyrca-0.0.1/pyrca/utils/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-04-27 06:55:22.000000 sfr-pyrca-0.0.1/pyrca/utils/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2751 2023-04-27 06:55:22.000000 sfr-pyrca-0.0.1/pyrca/utils/plot.py
--rw-r--r--   0 runner    (1001) docker     (123)     3950 2023-04-27 06:55:22.000000 sfr-pyrca-0.0.1/pyrca/utils/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-27 06:55:33.774021 sfr-pyrca-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1429 2023-04-27 06:55:22.000000 sfr-pyrca-0.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 06:55:33.774021 sfr-pyrca-0.0.1/sfr_pyrca.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13687 2023-04-27 06:55:33.000000 sfr-pyrca-0.0.1/sfr_pyrca.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6442 2023-04-27 06:55:33.000000 sfr-pyrca-0.0.1/sfr_pyrca.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 06:55:33.000000 sfr-pyrca-0.0.1/sfr_pyrca.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 06:55:33.000000 sfr-pyrca-0.0.1/sfr_pyrca.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      329 2023-04-27 06:55:33.000000 sfr-pyrca-0.0.1/sfr_pyrca.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-27 06:55:33.000000 sfr-pyrca-0.0.1/sfr_pyrca.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 06:55:33.746021 sfr-pyrca-0.0.1/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 06:55:33.774021 sfr-pyrca-0.0.1/tests/analyzers/
--rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-04-27 06:55:22.000000 sfr-pyrca-0.0.1/tests/analyzers/test_bayesian.py
--rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-04-27 06:55:22.000000 sfr-pyrca-0.0.1/tests/analyzers/test_epsilon_diagnosis.py
--rw-r--r--   0 runner    (1001) docker     (123)     1520 2023-04-27 06:55:22.000000 sfr-pyrca-0.0.1/tests/analyzers/test_ht.py
--rw-r--r--   0 runner    (1001) docker     (123)      950 2023-04-27 06:55:22.000000 sfr-pyrca-0.0.1/tests/analyzers/test_random_walk.py
--rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-04-27 06:55:22.000000 sfr-pyrca-0.0.1/tests/analyzers/test_rcd.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 06:55:33.746021 sfr-pyrca-0.0.1/tests/applications/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 06:55:33.774021 sfr-pyrca-0.0.1/tests/applications/example/
--rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-04-27 06:55:22.000000 sfr-pyrca-0.0.1/tests/applications/example/run_rca.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 06:55:33.774021 sfr-pyrca-0.0.1/tests/graphs/
--rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-04-27 06:55:22.000000 sfr-pyrca-0.0.1/tests/graphs/test_domain.py
--rw-r--r--   0 runner    (1001) docker     (123)     1221 2023-04-27 06:55:22.000000 sfr-pyrca-0.0.1/tests/graphs/test_fges.py
--rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-04-27 06:55:22.000000 sfr-pyrca-0.0.1/tests/graphs/test_ges.py
--rw-r--r--   0 runner    (1001) docker     (123)     1653 2023-04-27 06:55:22.000000 sfr-pyrca-0.0.1/tests/graphs/test_lingam.py
--rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-04-27 06:55:22.000000 sfr-pyrca-0.0.1/tests/graphs/test_pc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 06:55:33.774021 sfr-pyrca-0.0.1/tests/outliers/
--rw-r--r--   0 runner    (1001) docker     (123)     1928 2023-04-27 06:55:22.000000 sfr-pyrca-0.0.1/tests/outliers/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2737 2023-04-27 06:55:22.000000 sfr-pyrca-0.0.1/tests/outliers/test_stats.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 06:55:33.774021 sfr-pyrca-0.0.1/tests/simulation/
--rw-r--r--   0 runner    (1001) docker     (123)     1917 2023-04-27 06:55:22.000000 sfr-pyrca-0.0.1/tests/simulation/test_simulation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 06:55:33.774021 sfr-pyrca-0.0.1/tests/tools/
--rw-r--r--   0 runner    (1001) docker     (123)     1639 2023-04-27 06:55:22.000000 sfr-pyrca-0.0.1/tests/tools/test_causal.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 06:29:27.212315 sfr-pyrca-1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-05-18 06:29:13.000000 sfr-pyrca-1.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    14160 2023-05-18 06:29:27.212315 sfr-pyrca-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13770 2023-05-18 06:29:13.000000 sfr-pyrca-1.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 06:29:27.188313 sfr-pyrca-1.0.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     3377 2023-05-18 06:29:13.000000 sfr-pyrca-1.0.0/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 06:29:27.188313 sfr-pyrca-1.0.0/pyrca/
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-05-18 06:29:13.000000 sfr-pyrca-1.0.0/pyrca/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 06:29:27.192313 sfr-pyrca-1.0.0/pyrca/analyzers/
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-05-18 06:29:13.000000 sfr-pyrca-1.0.0/pyrca/analyzers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-05-18 06:29:13.000000 sfr-pyrca-1.0.0/pyrca/analyzers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19350 2023-05-18 06:29:13.000000 sfr-pyrca-1.0.0/pyrca/analyzers/bayesian.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3834 2023-05-18 06:29:13.000000 sfr-pyrca-1.0.0/pyrca/analyzers/epsilon_diagnosis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6415 2023-05-18 06:29:13.000000 sfr-pyrca-1.0.0/pyrca/analyzers/ht.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9957 2023-05-18 06:29:13.000000 sfr-pyrca-1.0.0/pyrca/analyzers/random_walk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2368 2023-05-18 06:29:13.000000 sfr-pyrca-1.0.0/pyrca/analyzers/rcd.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 06:29:27.184312 sfr-pyrca-1.0.0/pyrca/applications/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 06:29:27.192313 sfr-pyrca-1.0.0/pyrca/applications/example/
+-rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-05-18 06:29:13.000000 sfr-pyrca-1.0.0/pyrca/applications/example/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11586 2023-05-18 06:29:13.000000 sfr-pyrca-1.0.0/pyrca/applications/example/rca.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4340 2023-05-18 06:29:13.000000 sfr-pyrca-1.0.0/pyrca/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 06:29:27.192313 sfr-pyrca-1.0.0/pyrca/graphs/
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-05-18 06:29:13.000000 sfr-pyrca-1.0.0/pyrca/graphs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 06:29:27.192313 sfr-pyrca-1.0.0/pyrca/graphs/causal/
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-05-18 06:29:13.000000 sfr-pyrca-1.0.0/pyrca/graphs/causal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11525 2023-05-18 06:29:13.000000 sfr-pyrca-1.0.0/pyrca/graphs/causal/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3786 2023-05-18 06:29:13.000000 sfr-pyrca-1.0.0/pyrca/graphs/causal/fges.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3231 2023-05-18 06:29:13.000000 sfr-pyrca-1.0.0/pyrca/graphs/causal/ges.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2924 2023-05-18 06:29:13.000000 sfr-pyrca-1.0.0/pyrca/graphs/causal/lingam.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2762 2023-05-18 06:29:13.000000 sfr-pyrca-1.0.0/pyrca/graphs/causal/pc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 06:29:27.192313 sfr-pyrca-1.0.0/pyrca/outliers/
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-05-18 06:29:13.000000 sfr-pyrca-1.0.0/pyrca/outliers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5500 2023-05-18 06:29:13.000000 sfr-pyrca-1.0.0/pyrca/outliers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8130 2023-05-18 06:29:13.000000 sfr-pyrca-1.0.0/pyrca/outliers/stats.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 06:29:27.192313 sfr-pyrca-1.0.0/pyrca/simulation/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 06:29:13.000000 sfr-pyrca-1.0.0/pyrca/simulation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13983 2023-05-18 06:29:13.000000 sfr-pyrca-1.0.0/pyrca/simulation/data_gen.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 06:29:27.192313 sfr-pyrca-1.0.0/pyrca/thirdparty/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 06:29:13.000000 sfr-pyrca-1.0.0/pyrca/thirdparty/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 06:29:27.184312 sfr-pyrca-1.0.0/pyrca/thirdparty/causallearn/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 06:29:27.196313 sfr-pyrca-1.0.0/pyrca/thirdparty/causallearn/graph/
+-rw-r--r--   0 runner    (1001) docker     (123)     1660 2023-05-18 06:29:13.000000 sfr-pyrca-1.0.0/pyrca/thirdparty/causallearn/graph/AdjacencyConfusion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3704 2023-05-18 06:29:13.000000 sfr-pyrca-1.0.0/pyrca/thirdparty/causallearn/graph/ArrowConfusion.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25550 2023-05-18 06:29:13.000000 sfr-pyrca-1.0.0/pyrca/thirdparty/causallearn/graph/Dag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8532 2023-05-18 06:29:13.000000 sfr-pyrca-1.0.0/pyrca/thirdparty/causallearn/graph/Edge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2657 2023-05-18 06:29:13.000000 sfr-pyrca-1.0.0/pyrca/thirdparty/causallearn/graph/Edges.py
+-rw-r--r--   0 runner    (1001) docker     (123)      537 2023-05-18 06:29:13.000000 sfr-pyrca-1.0.0/pyrca/thirdparty/causallearn/graph/Endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37979 2023-05-18 06:29:13.000000 sfr-pyrca-1.0.0/pyrca/thirdparty/causallearn/graph/GeneralGraph.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18680 2023-05-18 06:29:13.000000 sfr-pyrca-1.0.0/pyrca/thirdparty/causallearn/graph/Graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8872 2023-05-18 06:29:13.000000 sfr-pyrca-1.0.0/pyrca/thirdparty/causallearn/graph/GraphClass.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2754 2023-05-18 06:29:13.000000 sfr-pyrca-1.0.0/pyrca/thirdparty/causallearn/graph/GraphNode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2056 2023-05-18 06:29:13.000000 sfr-pyrca-1.0.0/pyrca/thirdparty/causallearn/graph/Node.py
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-05-18 06:29:13.000000 sfr-pyrca-1.0.0/pyrca/thirdparty/causallearn/graph/NodeType.py
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-05-18 06:29:13.000000 sfr-pyrca-1.0.0/pyrca/thirdparty/causallearn/graph/NodeVariableType.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2068 2023-05-18 06:29:13.000000 sfr-pyrca-1.0.0/pyrca/thirdparty/causallearn/graph/SHD.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 06:29:27.196313 sfr-pyrca-1.0.0/pyrca/thirdparty/causallearn/score/
+-rw-r--r--   0 runner    (1001) docker     (123)    30361 2023-05-18 06:29:13.000000 sfr-pyrca-1.0.0/pyrca/thirdparty/causallearn/score/LocalScoreFunction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1551 2023-05-18 06:29:13.000000 sfr-pyrca-1.0.0/pyrca/thirdparty/causallearn/score/LocalScoreFunctionClass.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 06:29:27.184312 sfr-pyrca-1.0.0/pyrca/thirdparty/causallearn/search/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 06:29:27.196313 sfr-pyrca-1.0.0/pyrca/thirdparty/causallearn/search/ConstraintBased/
+-rw-r--r--   0 runner    (1001) docker     (123)    20748 2023-05-18 06:29:13.000000 sfr-pyrca-1.0.0/pyrca/thirdparty/causallearn/search/ConstraintBased/PC.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 06:29:27.196313 sfr-pyrca-1.0.0/pyrca/thirdparty/causallearn/search/ScoreBased/
+-rw-r--r--   0 runner    (1001) docker     (123)    15122 2023-05-18 06:29:13.000000 sfr-pyrca-1.0.0/pyrca/thirdparty/causallearn/search/ScoreBased/GES.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 06:29:27.196313 sfr-pyrca-1.0.0/pyrca/thirdparty/causallearn/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)    13321 2023-05-18 06:29:13.000000 sfr-pyrca-1.0.0/pyrca/thirdparty/causallearn/utils/BackgroundKnowledge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4891 2023-05-18 06:29:13.000000 sfr-pyrca-1.0.0/pyrca/thirdparty/causallearn/utils/DAG2CPDAG.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17718 2023-05-18 06:29:13.000000 sfr-pyrca-1.0.0/pyrca/thirdparty/causallearn/utils/GESUtils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16983 2023-05-18 06:29:13.000000 sfr-pyrca-1.0.0/pyrca/thirdparty/causallearn/utils/GraphUtils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 06:29:27.196313 sfr-pyrca-1.0.0/pyrca/thirdparty/causallearn/utils/PCUtils/
+-rw-r--r--   0 runner    (1001) docker     (123)     1956 2023-05-18 06:29:13.000000 sfr-pyrca-1.0.0/pyrca/thirdparty/causallearn/utils/PCUtils/BackgroundKnowledgeOrientUtils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28855 2023-05-18 06:29:13.000000 sfr-pyrca-1.0.0/pyrca/thirdparty/causallearn/utils/PCUtils/Helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9196 2023-05-18 06:29:13.000000 sfr-pyrca-1.0.0/pyrca/thirdparty/causallearn/utils/PCUtils/Meek.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5702 2023-05-18 06:29:13.000000 sfr-pyrca-1.0.0/pyrca/thirdparty/causallearn/utils/PCUtils/SkeletonDiscovery.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18852 2023-05-18 06:29:13.000000 sfr-pyrca-1.0.0/pyrca/thirdparty/causallearn/utils/PCUtils/UCSepset.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 06:29:13.000000 sfr-pyrca-1.0.0/pyrca/thirdparty/causallearn/utils/PCUtils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2586 2023-05-18 06:29:13.000000 sfr-pyrca-1.0.0/pyrca/thirdparty/causallearn/utils/PDAG2DAG.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28846 2023-05-18 06:29:13.000000 sfr-pyrca-1.0.0/pyrca/thirdparty/causallearn/utils/ScoreUtils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1947 2023-05-18 06:29:13.000000 sfr-pyrca-1.0.0/pyrca/thirdparty/causallearn/utils/TXT2GeneralGraph.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23583 2023-05-18 06:29:13.000000 sfr-pyrca-1.0.0/pyrca/thirdparty/causallearn/utils/cit.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 06:29:27.196313 sfr-pyrca-1.0.0/pyrca/thirdparty/pgmpy/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      116 2023-05-18 06:29:13.000000 sfr-pyrca-1.0.0/pyrca/thirdparty/pgmpy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 06:29:27.196313 sfr-pyrca-1.0.0/pyrca/thirdparty/pgmpy/base/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    40652 2023-05-18 06:29:13.000000 sfr-pyrca-1.0.0/pyrca/thirdparty/pgmpy/base/DAG.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9236 2023-05-18 06:29:13.000000 sfr-pyrca-1.0.0/pyrca/thirdparty/pgmpy/base/UndirectedGraph.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      118 2023-05-18 06:29:13.000000 sfr-pyrca-1.0.0/pyrca/thirdparty/pgmpy/base/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 06:29:27.200314 sfr-pyrca-1.0.0/pyrca/thirdparty/pgmpy/estimators/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9735 2023-05-18 06:29:13.000000 sfr-pyrca-1.0.0/pyrca/thirdparty/pgmpy/estimators/BayesianEstimator.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7542 2023-05-18 06:29:13.000000 sfr-pyrca-1.0.0/pyrca/thirdparty/pgmpy/estimators/MLE.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      302 2023-05-18 06:29:13.000000 sfr-pyrca-1.0.0/pyrca/thirdparty/pgmpy/estimators/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    12198 2023-05-18 06:29:13.000000 sfr-pyrca-1.0.0/pyrca/thirdparty/pgmpy/estimators/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 06:29:27.200314 sfr-pyrca-1.0.0/pyrca/thirdparty/pgmpy/extern/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       55 2023-05-18 06:29:13.000000 sfr-pyrca-1.0.0/pyrca/thirdparty/pgmpy/extern/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    30221 2023-05-18 06:29:13.000000 sfr-pyrca-1.0.0/pyrca/thirdparty/pgmpy/extern/tabulate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 06:29:27.200314 sfr-pyrca-1.0.0/pyrca/thirdparty/pgmpy/factors/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    15811 2023-05-18 06:29:13.000000 sfr-pyrca-1.0.0/pyrca/thirdparty/pgmpy/factors/FactorSet.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      242 2023-05-18 06:29:13.000000 sfr-pyrca-1.0.0/pyrca/thirdparty/pgmpy/factors/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3131 2023-05-18 06:29:13.000000 sfr-pyrca-1.0.0/pyrca/thirdparty/pgmpy/factors/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 06:29:27.200314 sfr-pyrca-1.0.0/pyrca/thirdparty/pgmpy/factors/continuous/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    13912 2023-05-18 06:29:13.000000 sfr-pyrca-1.0.0/pyrca/thirdparty/pgmpy/factors/continuous/ContinuousFactor.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)       86 2023-05-18 06:29:13.000000 sfr-pyrca-1.0.0/pyrca/thirdparty/pgmpy/factors/continuous/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 06:29:27.200314 sfr-pyrca-1.0.0/pyrca/thirdparty/pgmpy/factors/discrete/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    22540 2023-05-18 06:29:13.000000 sfr-pyrca-1.0.0/pyrca/thirdparty/pgmpy/factors/discrete/CPD.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    35423 2023-05-18 06:29:13.000000 sfr-pyrca-1.0.0/pyrca/thirdparty/pgmpy/factors/discrete/DiscreteFactor.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    15809 2023-05-18 06:29:13.000000 sfr-pyrca-1.0.0/pyrca/thirdparty/pgmpy/factors/discrete/JointProbabilityDistribution.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      202 2023-05-18 06:29:13.000000 sfr-pyrca-1.0.0/pyrca/thirdparty/pgmpy/factors/discrete/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 06:29:27.200314 sfr-pyrca-1.0.0/pyrca/thirdparty/pgmpy/factors/distributions/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    18453 2023-05-18 06:29:13.000000 sfr-pyrca-1.0.0/pyrca/thirdparty/pgmpy/factors/distributions/CustomDistribution.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    19793 2023-05-18 06:29:13.000000 sfr-pyrca-1.0.0/pyrca/thirdparty/pgmpy/factors/distributions/GaussianDistribution.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      220 2023-05-18 06:29:13.000000 sfr-pyrca-1.0.0/pyrca/thirdparty/pgmpy/factors/distributions/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      841 2023-05-18 06:29:13.000000 sfr-pyrca-1.0.0/pyrca/thirdparty/pgmpy/factors/distributions/base.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      830 2023-05-18 06:29:13.000000 sfr-pyrca-1.0.0/pyrca/thirdparty/pgmpy/global_vars.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 06:29:27.200314 sfr-pyrca-1.0.0/pyrca/thirdparty/pgmpy/independencies/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    16265 2023-05-18 06:29:13.000000 sfr-pyrca-1.0.0/pyrca/thirdparty/pgmpy/independencies/Independencies.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)        1 2023-05-18 06:29:13.000000 sfr-pyrca-1.0.0/pyrca/thirdparty/pgmpy/independencies/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 06:29:27.200314 sfr-pyrca-1.0.0/pyrca/thirdparty/pgmpy/inference/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5986 2023-05-18 06:29:13.000000 sfr-pyrca-1.0.0/pyrca/thirdparty/pgmpy/inference/EliminationOrder.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    44473 2023-05-18 06:29:13.000000 sfr-pyrca-1.0.0/pyrca/thirdparty/pgmpy/inference/ExactInference.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      135 2023-05-18 06:29:13.000000 sfr-pyrca-1.0.0/pyrca/thirdparty/pgmpy/inference/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8926 2023-05-18 06:29:13.000000 sfr-pyrca-1.0.0/pyrca/thirdparty/pgmpy/inference/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 06:29:27.204314 sfr-pyrca-1.0.0/pyrca/thirdparty/pgmpy/models/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    35116 2023-05-18 06:29:13.000000 sfr-pyrca-1.0.0/pyrca/thirdparty/pgmpy/models/BayesianModel.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    12668 2023-05-18 06:29:13.000000 sfr-pyrca-1.0.0/pyrca/thirdparty/pgmpy/models/ClusterGraph.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    25489 2023-05-18 06:29:13.000000 sfr-pyrca-1.0.0/pyrca/thirdparty/pgmpy/models/DynamicBayesianNetwork.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    17153 2023-05-18 06:29:13.000000 sfr-pyrca-1.0.0/pyrca/thirdparty/pgmpy/models/FactorGraph.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4302 2023-05-18 06:29:13.000000 sfr-pyrca-1.0.0/pyrca/thirdparty/pgmpy/models/JunctionTree.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    29581 2023-05-18 06:29:13.000000 sfr-pyrca-1.0.0/pyrca/thirdparty/pgmpy/models/MarkovModel.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      250 2023-05-18 06:29:13.000000 sfr-pyrca-1.0.0/pyrca/thirdparty/pgmpy/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 06:29:27.204314 sfr-pyrca-1.0.0/pyrca/thirdparty/pgmpy/readwrite/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    22279 2023-05-18 06:29:13.000000 sfr-pyrca-1.0.0/pyrca/thirdparty/pgmpy/readwrite/BIF.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)       87 2023-05-18 06:29:13.000000 sfr-pyrca-1.0.0/pyrca/thirdparty/pgmpy/readwrite/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 06:29:27.204314 sfr-pyrca-1.0.0/pyrca/thirdparty/pgmpy/utils/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       77 2023-05-18 06:29:13.000000 sfr-pyrca-1.0.0/pyrca/thirdparty/pgmpy/utils/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      301 2023-05-18 06:29:13.000000 sfr-pyrca-1.0.0/pyrca/thirdparty/pgmpy/utils/decorators.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3675 2023-05-18 06:29:13.000000 sfr-pyrca-1.0.0/pyrca/thirdparty/pgmpy/utils/state_name.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 06:29:27.204314 sfr-pyrca-1.0.0/pyrca/thirdparty/pycausal/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 06:29:13.000000 sfr-pyrca-1.0.0/pyrca/thirdparty/pycausal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2413 2023-05-18 06:29:13.000000 sfr-pyrca-1.0.0/pyrca/thirdparty/pycausal/prior.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10528 2023-05-18 06:29:13.000000 sfr-pyrca-1.0.0/pyrca/thirdparty/pycausal/pycausal.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20120 2023-05-18 06:29:13.000000 sfr-pyrca-1.0.0/pyrca/thirdparty/pycausal/search.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 06:29:27.204314 sfr-pyrca-1.0.0/pyrca/thirdparty/rcd/
+-rw-r--r--   0 runner    (1001) docker     (123)     6701 2023-05-18 06:29:13.000000 sfr-pyrca-1.0.0/pyrca/thirdparty/rcd/rcd.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 06:29:27.204314 sfr-pyrca-1.0.0/pyrca/thirdparty/rcd/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)    10362 2023-05-18 06:29:13.000000 sfr-pyrca-1.0.0/pyrca/thirdparty/rcd/utils/GraphClass.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8081 2023-05-18 06:29:13.000000 sfr-pyrca-1.0.0/pyrca/thirdparty/rcd/utils/SkeletonDiscovery.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 06:29:27.204314 sfr-pyrca-1.0.0/pyrca/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-05-18 06:29:13.000000 sfr-pyrca-1.0.0/pyrca/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      327 2023-05-18 06:29:13.000000 sfr-pyrca-1.0.0/pyrca/tools/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-05-18 06:29:13.000000 sfr-pyrca-1.0.0/pyrca/tools/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 06:29:27.204314 sfr-pyrca-1.0.0/pyrca/tools/dashboard/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 06:29:27.208314 sfr-pyrca-1.0.0/pyrca/tools/dashboard/assets/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    83784 2023-05-18 06:29:13.000000 sfr-pyrca-1.0.0/pyrca/tools/dashboard/assets/Acumin-BdPro.otf
+-rw-r--r--   0 runner    (1001) docker     (123)    12207 2023-05-18 06:29:13.000000 sfr-pyrca-1.0.0/pyrca/tools/dashboard/assets/base.css
+-rw-r--r--   0 runner    (1001) docker     (123)     5354 2023-05-18 06:29:13.000000 sfr-pyrca-1.0.0/pyrca/tools/dashboard/assets/logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)     6085 2023-05-18 06:29:13.000000 sfr-pyrca-1.0.0/pyrca/tools/dashboard/assets/modal.css
+-rw-r--r--   0 runner    (1001) docker     (123)     2684 2023-05-18 06:29:13.000000 sfr-pyrca-1.0.0/pyrca/tools/dashboard/assets/rca.css
+-rw-r--r--   0 runner    (1001) docker     (123)      292 2023-05-18 06:29:13.000000 sfr-pyrca-1.0.0/pyrca/tools/dashboard/assets/resizing.js
+-rw-r--r--   0 runner    (1001) docker     (123)      981 2023-05-18 06:29:13.000000 sfr-pyrca-1.0.0/pyrca/tools/dashboard/assets/styles.css
+-rw-r--r--   0 runner    (1001) docker     (123)      714 2023-05-18 06:29:13.000000 sfr-pyrca-1.0.0/pyrca/tools/dashboard/assets/upload.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 06:29:27.208314 sfr-pyrca-1.0.0/pyrca/tools/dashboard/callbacks/
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-05-18 06:29:13.000000 sfr-pyrca-1.0.0/pyrca/tools/dashboard/callbacks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14520 2023-05-18 06:29:13.000000 sfr-pyrca-1.0.0/pyrca/tools/dashboard/callbacks/causal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5386 2023-05-18 06:29:13.000000 sfr-pyrca-1.0.0/pyrca/tools/dashboard/callbacks/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1593 2023-05-18 06:29:13.000000 sfr-pyrca-1.0.0/pyrca/tools/dashboard/dashboard.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 06:29:27.208314 sfr-pyrca-1.0.0/pyrca/tools/dashboard/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-05-18 06:29:13.000000 sfr-pyrca-1.0.0/pyrca/tools/dashboard/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8752 2023-05-18 06:29:13.000000 sfr-pyrca-1.0.0/pyrca/tools/dashboard/models/causal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2576 2023-05-18 06:29:13.000000 sfr-pyrca-1.0.0/pyrca/tools/dashboard/models/data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 06:29:27.208314 sfr-pyrca-1.0.0/pyrca/tools/dashboard/pages/
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-05-18 06:29:13.000000 sfr-pyrca-1.0.0/pyrca/tools/dashboard/pages/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14014 2023-05-18 06:29:13.000000 sfr-pyrca-1.0.0/pyrca/tools/dashboard/pages/causal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7029 2023-05-18 06:29:13.000000 sfr-pyrca-1.0.0/pyrca/tools/dashboard/pages/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3102 2023-05-18 06:29:13.000000 sfr-pyrca-1.0.0/pyrca/tools/dashboard/pages/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-05-18 06:29:13.000000 sfr-pyrca-1.0.0/pyrca/tools/dashboard/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 06:29:27.208314 sfr-pyrca-1.0.0/pyrca/tools/dashboard/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-05-18 06:29:13.000000 sfr-pyrca-1.0.0/pyrca/tools/dashboard/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2750 2023-05-18 06:29:13.000000 sfr-pyrca-1.0.0/pyrca/tools/dashboard/utils/file_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1441 2023-05-18 06:29:13.000000 sfr-pyrca-1.0.0/pyrca/tools/dashboard/utils/layout.py
+-rw-r--r--   0 runner    (1001) docker     (123)      625 2023-05-18 06:29:13.000000 sfr-pyrca-1.0.0/pyrca/tools/dashboard/utils/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2774 2023-05-18 06:29:13.000000 sfr-pyrca-1.0.0/pyrca/tools/dashboard/utils/plot.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 06:29:27.208314 sfr-pyrca-1.0.0/pyrca/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-05-18 06:29:13.000000 sfr-pyrca-1.0.0/pyrca/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4141 2023-05-18 06:29:13.000000 sfr-pyrca-1.0.0/pyrca/utils/domain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2473 2023-05-18 06:29:13.000000 sfr-pyrca-1.0.0/pyrca/utils/evaluation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-05-18 06:29:13.000000 sfr-pyrca-1.0.0/pyrca/utils/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-05-18 06:29:13.000000 sfr-pyrca-1.0.0/pyrca/utils/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2751 2023-05-18 06:29:13.000000 sfr-pyrca-1.0.0/pyrca/utils/plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3950 2023-05-18 06:29:13.000000 sfr-pyrca-1.0.0/pyrca/utils/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-18 06:29:27.212315 sfr-pyrca-1.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1429 2023-05-18 06:29:13.000000 sfr-pyrca-1.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 06:29:27.212315 sfr-pyrca-1.0.0/sfr_pyrca.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14160 2023-05-18 06:29:27.000000 sfr-pyrca-1.0.0/sfr_pyrca.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6468 2023-05-18 06:29:27.000000 sfr-pyrca-1.0.0/sfr_pyrca.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 06:29:27.000000 sfr-pyrca-1.0.0/sfr_pyrca.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 06:29:26.000000 sfr-pyrca-1.0.0/sfr_pyrca.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      329 2023-05-18 06:29:27.000000 sfr-pyrca-1.0.0/sfr_pyrca.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-18 06:29:27.000000 sfr-pyrca-1.0.0/sfr_pyrca.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 06:29:27.188313 sfr-pyrca-1.0.0/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 06:29:27.212315 sfr-pyrca-1.0.0/tests/analyzers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-05-18 06:29:13.000000 sfr-pyrca-1.0.0/tests/analyzers/test_bayesian.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-05-18 06:29:13.000000 sfr-pyrca-1.0.0/tests/analyzers/test_epsilon_diagnosis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1520 2023-05-18 06:29:13.000000 sfr-pyrca-1.0.0/tests/analyzers/test_ht.py
+-rw-r--r--   0 runner    (1001) docker     (123)      950 2023-05-18 06:29:13.000000 sfr-pyrca-1.0.0/tests/analyzers/test_random_walk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-05-18 06:29:13.000000 sfr-pyrca-1.0.0/tests/analyzers/test_rcd.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 06:29:27.188313 sfr-pyrca-1.0.0/tests/applications/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 06:29:27.212315 sfr-pyrca-1.0.0/tests/applications/example/
+-rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-05-18 06:29:13.000000 sfr-pyrca-1.0.0/tests/applications/example/run_rca.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 06:29:27.212315 sfr-pyrca-1.0.0/tests/graphs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-05-18 06:29:14.000000 sfr-pyrca-1.0.0/tests/graphs/test_domain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1221 2023-05-18 06:29:14.000000 sfr-pyrca-1.0.0/tests/graphs/test_fges.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-05-18 06:29:14.000000 sfr-pyrca-1.0.0/tests/graphs/test_ges.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1653 2023-05-18 06:29:14.000000 sfr-pyrca-1.0.0/tests/graphs/test_lingam.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-05-18 06:29:14.000000 sfr-pyrca-1.0.0/tests/graphs/test_pc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 06:29:27.212315 sfr-pyrca-1.0.0/tests/outliers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1928 2023-05-18 06:29:14.000000 sfr-pyrca-1.0.0/tests/outliers/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2737 2023-05-18 06:29:14.000000 sfr-pyrca-1.0.0/tests/outliers/test_stats.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 06:29:27.212315 sfr-pyrca-1.0.0/tests/simulation/
+-rw-r--r--   0 runner    (1001) docker     (123)     1917 2023-05-18 06:29:14.000000 sfr-pyrca-1.0.0/tests/simulation/test_simulation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 06:29:27.212315 sfr-pyrca-1.0.0/tests/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)     1639 2023-05-18 06:29:14.000000 sfr-pyrca-1.0.0/tests/tools/test_causal.py
```

### Comparing `sfr-pyrca-0.0.1/LICENSE` & `sfr-pyrca-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sfr-pyrca-0.0.1/PKG-INFO` & `sfr-pyrca-1.0.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sfr-pyrca
-Version: 0.0.1
+Version: 1.0.0
 Summary: PyRCA: A Python library for Root Cause Analysis
 Home-page: https://github.com/salesforce/PyRCA
 Author: Salesforce Research Warden AIOps
 License: 3-Clause BSD
 Keywords: AIOps RCA root cause analysis
 Requires-Python: >=3.7,<4
 Description-Content-Type: text/markdown
@@ -39,38 +39,40 @@
 5. [Tutorial](https://github.com/salesforce/PyRCA/tree/main/examples)
 6. [Example](#application-example)
 7. [Benchmarks](#benchmarks)
 8. [How to Contribute](#how-to-contribute)
 
 ## Introduction
 
-With the rapidly growing adoption of microservices architectures, multi-service applications become the standard 
-paradigm in real-world IT applications. A multi-service application usually contains hundreds of interacting 
-services, making it harder to detect service failures and identify the root causes. Root cause analysis (RCA) 
-methods usually leverage the KPI metrics, traces or logs monitored on those services to determine the root causes 
-when a system failure is detected, helping engineers and SREs in the troubleshooting process.
-
-PyRCA is a Python machine-learning library designed for root cause analysis, offering multiple state-of-the-art RCA
-algorithms and an end-to-end pipeline for building RCA solutions. Currently, PyRCA mainly focuses on metric-based RCA 
-including two types of algorithms: 1. Identifying anomalous metrics in parallel with the observed anomaly via 
-metric data analysis, e.g., ε-diagnosis, and 2. Identifying root causes based a topology/causal graph representing 
-the causal relationships between the observed metrics, e.g., Bayesian inference, Random Walk. Besides, PyRCA 
-provides a convenient tool for building causal graphs from the observed time series data and domain knowledge, 
-helping users to develop graph-based solutions quickly. PyRCA also provides a benchmark for evaluating 
-various RCA methods, which is valuable for industry and academic research.
+The adoption of microservices architectures is growing at a rapid pace, making multi-service applications 
+the standard paradigm in real-world IT applications. Typically, a multi-service application consists of 
+hundreds of interacting services, making it increasingly challenging to detect service failures and identify 
+their root causes. Root cause analysis (RCA) methods typically rely on KPI metrics, traces, or logs monitored 
+on these services to determine the root causes when a system failure is detected. Such methods can aid 
+engineers and SREs in the troubleshooting process.
+
+PyRCA is a Python machine-learning library designed to facilitate root cause analysis by offering various 
+state-of-the-art RCA algorithms and an end-to-end pipeline for building RCA solutions. At present, PyRCA 
+primarily focuses on metric-based RCA, including two types of algorithms: (1) identifying anomalous metrics 
+in parallel with the observed anomaly through metric data analysis, such as ε-diagnosis, and (2) identifying 
+root causes based on a topology/causal graph representing the causal relationships between the observed 
+metrics, such as Bayesian inference and Random Walk. PyRCA also provides a convenient tool for building 
+causal graphs from the observed time series data and domain knowledge, enabling users to develop graph-based 
+solutions quickly. Furthermore, PyRCA offers a benchmark for evaluating various RCA methods, which is 
+valuable for industry and academic research.
 
 The following list shows the supported RCA methods in our library:
-1. ε-Diagnosis
+1. [ε-Diagnosis](https://dl.acm.org/doi/10.1145/3308558.3313653)
 2. Bayesian Inference-based RCA (BI)
 3. Random Walk-based RCA (RW)
-4. Root Casue Discovery method (RCD)
-5. Hypothesis Testing-based RCA (HT)
+4. [Root Casue Discovery method (RCD)](https://openreview.net/pdf?id=weoLjoYFvXY)
+5. [Hypothesis Testing-based RCA (HT)](https://dl.acm.org/doi/10.1145/3534678.3539041)
 
 We will continue improving this library to make it more comprehensive in the future. In the future, 
-PyRCA will support trace and log based RCA methods as well.
+PyRCA will support trace and log-based RCA methods as well.
 
 ## Installation
 
 You can install ``pyrca`` from PyPI by calling ``pip install sfr-pyrca``. You may install from source by
 cloning the PyRCA repo, navigating to the root directory, and calling
 ``pip install .``, or ``pip install -e .`` to install in editable mode. You may install additional dependencies:
 
@@ -80,36 +82,38 @@
   root directory of the repo.
 
 ## Getting Started
 
 PyRCA provides a unified interface for training RCA models and finding root causes. To apply
 a certain RCA method, you only need to specify: 
 
-- **The select RCA method**: e.g., ``BayesianNetwork``, ``EpsilonDiagnosis``.
-- **The RCA configuration**: e.g., ``BayesianNetworkConfig``, ``EpsilonDiagnosisConfig``.
-- **Time series data for initialization or training**: e.g., A time series data in a 
+- **The selected RCA method**: e.g., ``BayesianNetwork``, ``EpsilonDiagnosis``.
+- **The method configuration**: e.g., ``BayesianNetworkConfig``, ``EpsilonDiagnosisConfig``.
+- **Time series data for initialization/training**: e.g., A time series data in a 
   pandas dataframe.
-- **Some detected anomalous KPI metrics**: Some RCA methods require the anomalous KPI metrics detected by
-  certain anomaly detector.
+- **Abnormal time series data in an incident window**: The RCA methods require the anomalous 
+  KPI metrics in an incident window.
 
-Let's take ``BayesianNetwork`` as an example. Suppose that ``graph_df`` is a pandas dataframe of
-the graph representing causal relationships between metrics (how to construct such causal graph
-will be discussed later), and ``df`` is a pandas dataframe containing the historical observed time series 
+Let's take ``BayesianNetwork`` as an example. Suppose that ``graph_df`` is the pandas dataframe of
+a graph representing the causal relationships between metrics (how to construct such causal graph
+will be discussed later), and ``df`` is the pandas dataframe containing the historical observed time series 
 data (e.g., the index is the timestamp and each column represents one monitored metric). To train a 
 ``BayesianNetwork``, you can simply run the following code:
 
 ```python
 from pyrca.analyzers.bayesian import BayesianNetwork
 model = BayesianNetwork(config=BayesianNetwork.config_class(graph=graph_df))
 model.train(df)
 model.save("model_folder")
 ```
 
 After the model is trained, you can use it to find root causes of an incident given a list of anomalous
-metrics detected by a certain anomaly detector, e.g.,
+metrics detected by a certain anomaly detector (you can use the stats-based detector supported in PyRCA
+or other anomaly detection methods supported by our [Merlion](https://github.com/salesforce/Merlion) library), 
+e.g.,
 
 ```python
 from pyrca.analyzers.bayesian import BayesianNetwork
 model = BayesianNetwork.load("model_folder")
 results = model.find_root_causes(["observed_anomalous_metric", ...])
 print(results.to_dict())
 ```
@@ -134,24 +138,24 @@
 where ``abnormal_data`` is the time series data collected in an incident window.
 
 As mentioned above, some RCA methods such as ``BayesianNetwork`` require causal graphs as their inputs. To construct such causal
 graphs from the observed time series data, you can utilize our tool by running ``python -m pyrca.tools``.
 This command will launch a Dash app for time series data analysis and causal discovery.
 ![alt text](https://github.com/salesforce/PyRCA/raw/main/docs/_static/dashboard.png)
 
-The dashboard allows you to try different causal discovery methods, adjust causal discovery parameters,
-add domain knowledge constraints (e.g., root/leaf nodes, forbidden/required links), and visualize
-the generated causal graphs. It makes easier for manually revising causal graphs based on domain knowledge.
-You can download the graph generated by this tool if you satisfy with it. The graph can be used by the RCA 
-methods supported in PyRCA.
-
-Instead of using this dashboard, you can also write code for building such graphs. The package 
-``pyrca.graphs.causal`` includes several popular causal discovery methods you can use. All of these methods
-support domain knowledge constraints. Suppose ``df`` is the observed time series data
-and you want to apply the PC algorithm for building causal graphs, then the following code will help:
+The dashboard enables users to experiment with different causal discovery methods, customize causal discovery 
+parameters, add domain knowledge constraints (e.g., root/leaf nodes, forbidden/required links), and visualize 
+the generated causal graphs. This feature simplifies the process of manually revising causal graphs based on 
+domain knowledge. Users can download the graph generated by this tool if they are satisfied with it. The graph 
+can then be used by the RCA methods supported in PyRCA.
+
+Alternatively, users can write code to build such graphs instead of using the dashboard. The package 
+``pyrca.graphs.causal`` includes several popular causal discovery methods that users can leverage. 
+All of these methods support domain knowledge constraints. For instance, if users wish to apply the PC 
+algorithm for building causal graphs on the observed time series data ``df``, the following code can be used:
 
 ```python
 from pyrca.graphs.causal.pc import PC
 model = PC(PC.config_class())
 graph_df = model.train(df)
 ```
 
@@ -188,15 +192,15 @@
 
 [Here](https://github.com/salesforce/PyRCA/tree/main/pyrca/applications/example) is a real-world example
 of applying ``BayesianNetwork`` to build a solution for RCA, which is adapted from our internal use cases. 
 The "config" folder includes the settings for the stats-based anomaly detector and the domain knowledge. 
 The "models" folder stores the causal graph and the trained Bayesian network. The ``RCAEngine`` class in the "rca.py" 
 file implements the methods for building causal graphs, training Bayesian networks and finding root causes 
 by utilizing the modules provided by PyRCA. You can directly use this class if the stats-based anomaly detector 
-and Bayesian inference are suitable for your RCA problems. For example, given a time series dataframe ``df``, 
+and Bayesian inference are suitable for your problems. For example, given a time series dataframe ``df``, 
 you can build and train a Bayesian network via the following code:
 
 ```python
 from pyrca.applications.example.rca import RCAEngine
 engine = RCAEngine()
 engine.build_causal_graph(
     df=df,
```

#### html2text {}

```diff
@@ -1,100 +1,106 @@
-Metadata-Version: 2.1 Name: sfr-pyrca Version: 0.0.1 Summary: PyRCA: A Python
+Metadata-Version: 2.1 Name: sfr-pyrca Version: 1.0.0 Summary: PyRCA: A Python
 library for Root Cause Analysis Home-page: https://github.com/salesforce/PyRCA
 Author: Salesforce Research Warden AIOps License: 3-Clause BSD Keywords: AIOps
 RCA root cause analysis Requires-Python: >=3.7,<4 Description-Content-Type:
 text/markdown Provides-Extra: plot Provides-Extra: all License-File: LICENSE #
 PyRCA: A Python library for Root Cause Analysis
 [https://img.shields.io/badge/Python-3.7,_3.8,_3.9-blue] [PyPI] [Documentation]
                                [Downloads] [DOI]
 ## Table of Contents 1. [Introduction](#introduction) 2. [Installation]
 (#installation) 3. [Getting Started](#getting-started) 4. [Documentation]
 (https://fuzzy-disco-r42n6p1.pages.github.io/) 5. [Tutorial](https://
 github.com/salesforce/PyRCA/tree/main/examples) 6. [Example](#application-
 example) 7. [Benchmarks](#benchmarks) 8. [How to Contribute](#how-to-
-contribute) ## Introduction With the rapidly growing adoption of microservices
-architectures, multi-service applications become the standard paradigm in real-
-world IT applications. A multi-service application usually contains hundreds of
-interacting services, making it harder to detect service failures and identify
-the root causes. Root cause analysis (RCA) methods usually leverage the KPI
-metrics, traces or logs monitored on those services to determine the root
-causes when a system failure is detected, helping engineers and SREs in the
-troubleshooting process. PyRCA is a Python machine-learning library designed
-for root cause analysis, offering multiple state-of-the-art RCA algorithms and
-an end-to-end pipeline for building RCA solutions. Currently, PyRCA mainly
-focuses on metric-based RCA including two types of algorithms: 1. Identifying
-anomalous metrics in parallel with the observed anomaly via metric data
-analysis, e.g., Îµ-diagnosis, and 2. Identifying root causes based a topology/
-causal graph representing the causal relationships between the observed
-metrics, e.g., Bayesian inference, Random Walk. Besides, PyRCA provides a
-convenient tool for building causal graphs from the observed time series data
-and domain knowledge, helping users to develop graph-based solutions quickly.
-PyRCA also provides a benchmark for evaluating various RCA methods, which is
-valuable for industry and academic research. The following list shows the
-supported RCA methods in our library: 1. Îµ-Diagnosis 2. Bayesian Inference-
-based RCA (BI) 3. Random Walk-based RCA (RW) 4. Root Casue Discovery method
-(RCD) 5. Hypothesis Testing-based RCA (HT) We will continue improving this
-library to make it more comprehensive in the future. In the future, PyRCA will
-support trace and log based RCA methods as well. ## Installation You can
-install ``pyrca`` from PyPI by calling ``pip install sfr-pyrca``. You may
-install from source by cloning the PyRCA repo, navigating to the root
-directory, and calling ``pip install .``, or ``pip install -e .`` to install in
-editable mode. You may install additional dependencies: - **For plotting &
-visualization**: Calling ``pip install sfr-pyrca[plot]``, or ``pip install .
-[plot]`` from the root directory of the repo. - **Install all the
+contribute) ## Introduction The adoption of microservices architectures is
+growing at a rapid pace, making multi-service applications the standard
+paradigm in real-world IT applications. Typically, a multi-service application
+consists of hundreds of interacting services, making it increasingly
+challenging to detect service failures and identify their root causes. Root
+cause analysis (RCA) methods typically rely on KPI metrics, traces, or logs
+monitored on these services to determine the root causes when a system failure
+is detected. Such methods can aid engineers and SREs in the troubleshooting
+process. PyRCA is a Python machine-learning library designed to facilitate root
+cause analysis by offering various state-of-the-art RCA algorithms and an end-
+to-end pipeline for building RCA solutions. At present, PyRCA primarily focuses
+on metric-based RCA, including two types of algorithms: (1) identifying
+anomalous metrics in parallel with the observed anomaly through metric data
+analysis, such as Îµ-diagnosis, and (2) identifying root causes based on a
+topology/causal graph representing the causal relationships between the
+observed metrics, such as Bayesian inference and Random Walk. PyRCA also
+provides a convenient tool for building causal graphs from the observed time
+series data and domain knowledge, enabling users to develop graph-based
+solutions quickly. Furthermore, PyRCA offers a benchmark for evaluating various
+RCA methods, which is valuable for industry and academic research. The
+following list shows the supported RCA methods in our library: 1. [Îµ-
+Diagnosis](https://dl.acm.org/doi/10.1145/3308558.3313653) 2. Bayesian
+Inference-based RCA (BI) 3. Random Walk-based RCA (RW) 4. [Root Casue Discovery
+method (RCD)](https://openreview.net/pdf?id=weoLjoYFvXY) 5. [Hypothesis
+Testing-based RCA (HT)](https://dl.acm.org/doi/10.1145/3534678.3539041) We will
+continue improving this library to make it more comprehensive in the future. In
+the future, PyRCA will support trace and log-based RCA methods as well. ##
+Installation You can install ``pyrca`` from PyPI by calling ``pip install sfr-
+pyrca``. You may install from source by cloning the PyRCA repo, navigating to
+the root directory, and calling ``pip install .``, or ``pip install -e .`` to
+install in editable mode. You may install additional dependencies: - **For
+plotting & visualization**: Calling ``pip install sfr-pyrca[plot]``, or ``pip
+install .[plot]`` from the root directory of the repo. - **Install all the
 dependencies**: Calling ``pip install sfr-pyrca[all]``, or ``pip install .
 [all]`` from the root directory of the repo. ## Getting Started PyRCA provides
 a unified interface for training RCA models and finding root causes. To apply a
-certain RCA method, you only need to specify: - **The select RCA method**:
-e.g., ``BayesianNetwork``, ``EpsilonDiagnosis``. - **The RCA configuration**:
-e.g., ``BayesianNetworkConfig``, ``EpsilonDiagnosisConfig``. - **Time series
-data for initialization or training**: e.g., A time series data in a pandas
-dataframe. - **Some detected anomalous KPI metrics**: Some RCA methods require
-the anomalous KPI metrics detected by certain anomaly detector. Let's take
-``BayesianNetwork`` as an example. Suppose that ``graph_df`` is a pandas
-dataframe of the graph representing causal relationships between metrics (how
-to construct such causal graph will be discussed later), and ``df`` is a pandas
-dataframe containing the historical observed time series data (e.g., the index
-is the timestamp and each column represents one monitored metric). To train a
-``BayesianNetwork``, you can simply run the following code: ```python from
-pyrca.analyzers.bayesian import BayesianNetwork model = BayesianNetwork
+certain RCA method, you only need to specify: - **The selected RCA method**:
+e.g., ``BayesianNetwork``, ``EpsilonDiagnosis``. - **The method
+configuration**: e.g., ``BayesianNetworkConfig``, ``EpsilonDiagnosisConfig``. -
+**Time series data for initialization/training**: e.g., A time series data in a
+pandas dataframe. - **Abnormal time series data in an incident window**: The
+RCA methods require the anomalous KPI metrics in an incident window. Let's take
+``BayesianNetwork`` as an example. Suppose that ``graph_df`` is the pandas
+dataframe of a graph representing the causal relationships between metrics (how
+to construct such causal graph will be discussed later), and ``df`` is the
+pandas dataframe containing the historical observed time series data (e.g., the
+index is the timestamp and each column represents one monitored metric). To
+train a ``BayesianNetwork``, you can simply run the following code: ```python
+from pyrca.analyzers.bayesian import BayesianNetwork model = BayesianNetwork
 (config=BayesianNetwork.config_class(graph=graph_df)) model.train(df)
 model.save("model_folder") ``` After the model is trained, you can use it to
 find root causes of an incident given a list of anomalous metrics detected by a
-certain anomaly detector, e.g., ```python from pyrca.analyzers.bayesian import
-BayesianNetwork model = BayesianNetwork.load("model_folder") results =
-model.find_root_causes(["observed_anomalous_metric", ...]) print
-(results.to_dict()) ``` For other RCA methods, you can write similar code as
-above for finding root causes. For example, if you want to try
+certain anomaly detector (you can use the stats-based detector supported in
+PyRCA or other anomaly detection methods supported by our [Merlion](https://
+github.com/salesforce/Merlion) library), e.g., ```python from
+pyrca.analyzers.bayesian import BayesianNetwork model = BayesianNetwork.load
+("model_folder") results = model.find_root_causes(["observed_anomalous_metric",
+...]) print(results.to_dict()) ``` For other RCA methods, you can write similar
+code as above for finding root causes. For example, if you want to try
 ``EpsilonDiagnosis``, you can initalize ``EpsilonDiagnosis`` as follows:
 ```python from pyrca.analyzers.epsilon_diagnosis import EpsilonDiagnosis model
 = EpsilonDiagnosis(config=EpsilonDiagnosis.config_class(alpha=0.01))
 model.train(normal_data) ``` Here ``normal_data`` is the historically observed
 time series data without anomalies. To identify root causes, you can run:
 ```python results = model.find_root_causes(abnormal_data) print(results.to_dict
 ()) ``` where ``abnormal_data`` is the time series data collected in an
 incident window. As mentioned above, some RCA methods such as
 ``BayesianNetwork`` require causal graphs as their inputs. To construct such
 causal graphs from the observed time series data, you can utilize our tool by
 running ``python -m pyrca.tools``. This command will launch a Dash app for time
 series data analysis and causal discovery. ![alt text](https://github.com/
-salesforce/PyRCA/raw/main/docs/_static/dashboard.png) The dashboard allows you
-to try different causal discovery methods, adjust causal discovery parameters,
-add domain knowledge constraints (e.g., root/leaf nodes, forbidden/required
-links), and visualize the generated causal graphs. It makes easier for manually
-revising causal graphs based on domain knowledge. You can download the graph
-generated by this tool if you satisfy with it. The graph can be used by the RCA
-methods supported in PyRCA. Instead of using this dashboard, you can also write
-code for building such graphs. The package ``pyrca.graphs.causal`` includes
-several popular causal discovery methods you can use. All of these methods
-support domain knowledge constraints. Suppose ``df`` is the observed time
-series data and you want to apply the PC algorithm for building causal graphs,
-then the following code will help: ```python from pyrca.graphs.causal.pc import
-PC model = PC(PC.config_class()) graph_df = model.train(df) ``` If you have
-some domain knowledge constraints, you may run: ```python from
+salesforce/PyRCA/raw/main/docs/_static/dashboard.png) The dashboard enables
+users to experiment with different causal discovery methods, customize causal
+discovery parameters, add domain knowledge constraints (e.g., root/leaf nodes,
+forbidden/required links), and visualize the generated causal graphs. This
+feature simplifies the process of manually revising causal graphs based on
+domain knowledge. Users can download the graph generated by this tool if they
+are satisfied with it. The graph can then be used by the RCA methods supported
+in PyRCA. Alternatively, users can write code to build such graphs instead of
+using the dashboard. The package ``pyrca.graphs.causal`` includes several
+popular causal discovery methods that users can leverage. All of these methods
+support domain knowledge constraints. For instance, if users wish to apply the
+PC algorithm for building causal graphs on the observed time series data
+``df``, the following code can be used: ```python from pyrca.graphs.causal.pc
+import PC model = PC(PC.config_class()) graph_df = model.train(df) ``` If you
+have some domain knowledge constraints, you may run: ```python from
 pyrca.graphs.causal.pc import PC model = PC(PC.config_class
 (domain_knowledge_file="file_path")) graph_df = model.train(df) ``` The domain
 knowledge file has a YAML format, e.g., ```yaml causal-graph: root-nodes: ["A",
 "B"] leaf-nodes: ["E", "F"] forbids: - ["A", "E"] requires: - ["A", "C"] ```
 This domain knowledge file states that: 1. Metrics A and B must the root nodes,
 2. Metrics E and F must be the leaf nodes, 3. There is no connection from A to
 E, and 4. There is a connection from A to C. You can write your domain
@@ -104,32 +110,31 @@
 ``BayesianNetwork`` to build a solution for RCA, which is adapted from our
 internal use cases. The "config" folder includes the settings for the stats-
 based anomaly detector and the domain knowledge. The "models" folder stores the
 causal graph and the trained Bayesian network. The ``RCAEngine`` class in the
 "rca.py" file implements the methods for building causal graphs, training
 Bayesian networks and finding root causes by utilizing the modules provided by
 PyRCA. You can directly use this class if the stats-based anomaly detector and
-Bayesian inference are suitable for your RCA problems. For example, given a
-time series dataframe ``df``, you can build and train a Bayesian network via
-the following code: ```python from pyrca.applications.example.rca import
-RCAEngine engine = RCAEngine() engine.build_causal_graph( df=df,
-run_pdag2dag=True, max_num_points=5000000, verbose=True ) bn =
-engine.train_bayesian_network(dfs=[df]) bn.print_probabilities() ``` After the
-Bayesian network is constructed, you can use it directly for finding root
-causes: ```python engine = RCAEngine() result = engine.find_root_causes_bn
-(anomalies=["conn_pool", "apt"]) pprint.pprint(result) ``` The inputs of
-``find_root_causes_bn`` is a list of the anomalous metrics detected by the
-stats-based anomaly detector. This method will estimate the probability of a
-node being a root cause and extract the paths from a potential root cause node
-to the leaf nodes. ## Benchmarks The following table summarizes the RCA
-performance of different methods on the simulated dataset. How to generate the
-simulated dataset can be found [here](https://github.com/salesforce/PyRCA/blob/
-main/examples/DataGeneration.ipynb), and how to test different RCA methods can
-be found [here](https://github.com/salesforce/PyRCA/blob/main/examples/
-Root%20Cause%20Analysis.ipynb).
+Bayesian inference are suitable for your problems. For example, given a time
+series dataframe ``df``, you can build and train a Bayesian network via the
+following code: ```python from pyrca.applications.example.rca import RCAEngine
+engine = RCAEngine() engine.build_causal_graph( df=df, run_pdag2dag=True,
+max_num_points=5000000, verbose=True ) bn = engine.train_bayesian_network(dfs=
+[df]) bn.print_probabilities() ``` After the Bayesian network is constructed,
+you can use it directly for finding root causes: ```python engine = RCAEngine()
+result = engine.find_root_causes_bn(anomalies=["conn_pool", "apt"])
+pprint.pprint(result) ``` The inputs of ``find_root_causes_bn`` is a list of
+the anomalous metrics detected by the stats-based anomaly detector. This method
+will estimate the probability of a node being a root cause and extract the
+paths from a potential root cause node to the leaf nodes. ## Benchmarks The
+following table summarizes the RCA performance of different methods on the
+simulated dataset. How to generate the simulated dataset can be found [here]
+(https://github.com/salesforce/PyRCA/blob/main/examples/DataGeneration.ipynb),
+and how to test different RCA methods can be found [here](https://github.com/
+salesforce/PyRCA/blob/main/examples/Root%20Cause%20Analysis.ipynb).
 | | Recall@1 | Recall@3 | Recall@5 | :---------------------------:|:----------
  -:|:-----------:|:-----------: | Îµ-Diagnosis | 0.06 Â± 0.02 | 0.16 Â± 0.04 |
 0.16 Â± 0.04 | | RCD | 0.28 Â± 0.05 | 0.29 Â± 0.05 | 0.30 Â± 0.05 | | Local-RCD
  | 0.44 Â± 0.05 | 0.70 Â± 0.05 | 0.70 Â± 0.05 | | Random Walk | 0.07 Â± 0.03 |
 0.20 Â± 0.04 | 0.24 Â± 0.04 | | Random Walk (PC) | 0.06 Â± 0.02 | 0.17 Â± 0.04
  | 0.21 Â± 0.04 | | Bayesian Inference | 0.15 Â± 0.04 | 0.35 Â± 0.05 | 0.43 Â±
 0.05 | | Bayesian Inference (PC) | 0.11 Â± 0.03 | 0.30 Â± 0.05 | 0.40 Â± 0.05 |
```

### Comparing `sfr-pyrca-0.0.1/README.md` & `sfr-pyrca-1.0.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -25,38 +25,40 @@
 5. [Tutorial](https://github.com/salesforce/PyRCA/tree/main/examples)
 6. [Example](#application-example)
 7. [Benchmarks](#benchmarks)
 8. [How to Contribute](#how-to-contribute)
 
 ## Introduction
 
-With the rapidly growing adoption of microservices architectures, multi-service applications become the standard 
-paradigm in real-world IT applications. A multi-service application usually contains hundreds of interacting 
-services, making it harder to detect service failures and identify the root causes. Root cause analysis (RCA) 
-methods usually leverage the KPI metrics, traces or logs monitored on those services to determine the root causes 
-when a system failure is detected, helping engineers and SREs in the troubleshooting process.
-
-PyRCA is a Python machine-learning library designed for root cause analysis, offering multiple state-of-the-art RCA
-algorithms and an end-to-end pipeline for building RCA solutions. Currently, PyRCA mainly focuses on metric-based RCA 
-including two types of algorithms: 1. Identifying anomalous metrics in parallel with the observed anomaly via 
-metric data analysis, e.g., ε-diagnosis, and 2. Identifying root causes based a topology/causal graph representing 
-the causal relationships between the observed metrics, e.g., Bayesian inference, Random Walk. Besides, PyRCA 
-provides a convenient tool for building causal graphs from the observed time series data and domain knowledge, 
-helping users to develop graph-based solutions quickly. PyRCA also provides a benchmark for evaluating 
-various RCA methods, which is valuable for industry and academic research.
+The adoption of microservices architectures is growing at a rapid pace, making multi-service applications 
+the standard paradigm in real-world IT applications. Typically, a multi-service application consists of 
+hundreds of interacting services, making it increasingly challenging to detect service failures and identify 
+their root causes. Root cause analysis (RCA) methods typically rely on KPI metrics, traces, or logs monitored 
+on these services to determine the root causes when a system failure is detected. Such methods can aid 
+engineers and SREs in the troubleshooting process.
+
+PyRCA is a Python machine-learning library designed to facilitate root cause analysis by offering various 
+state-of-the-art RCA algorithms and an end-to-end pipeline for building RCA solutions. At present, PyRCA 
+primarily focuses on metric-based RCA, including two types of algorithms: (1) identifying anomalous metrics 
+in parallel with the observed anomaly through metric data analysis, such as ε-diagnosis, and (2) identifying 
+root causes based on a topology/causal graph representing the causal relationships between the observed 
+metrics, such as Bayesian inference and Random Walk. PyRCA also provides a convenient tool for building 
+causal graphs from the observed time series data and domain knowledge, enabling users to develop graph-based 
+solutions quickly. Furthermore, PyRCA offers a benchmark for evaluating various RCA methods, which is 
+valuable for industry and academic research.
 
 The following list shows the supported RCA methods in our library:
-1. ε-Diagnosis
+1. [ε-Diagnosis](https://dl.acm.org/doi/10.1145/3308558.3313653)
 2. Bayesian Inference-based RCA (BI)
 3. Random Walk-based RCA (RW)
-4. Root Casue Discovery method (RCD)
-5. Hypothesis Testing-based RCA (HT)
+4. [Root Casue Discovery method (RCD)](https://openreview.net/pdf?id=weoLjoYFvXY)
+5. [Hypothesis Testing-based RCA (HT)](https://dl.acm.org/doi/10.1145/3534678.3539041)
 
 We will continue improving this library to make it more comprehensive in the future. In the future, 
-PyRCA will support trace and log based RCA methods as well.
+PyRCA will support trace and log-based RCA methods as well.
 
 ## Installation
 
 You can install ``pyrca`` from PyPI by calling ``pip install sfr-pyrca``. You may install from source by
 cloning the PyRCA repo, navigating to the root directory, and calling
 ``pip install .``, or ``pip install -e .`` to install in editable mode. You may install additional dependencies:
 
@@ -66,36 +68,38 @@
   root directory of the repo.
 
 ## Getting Started
 
 PyRCA provides a unified interface for training RCA models and finding root causes. To apply
 a certain RCA method, you only need to specify: 
 
-- **The select RCA method**: e.g., ``BayesianNetwork``, ``EpsilonDiagnosis``.
-- **The RCA configuration**: e.g., ``BayesianNetworkConfig``, ``EpsilonDiagnosisConfig``.
-- **Time series data for initialization or training**: e.g., A time series data in a 
+- **The selected RCA method**: e.g., ``BayesianNetwork``, ``EpsilonDiagnosis``.
+- **The method configuration**: e.g., ``BayesianNetworkConfig``, ``EpsilonDiagnosisConfig``.
+- **Time series data for initialization/training**: e.g., A time series data in a 
   pandas dataframe.
-- **Some detected anomalous KPI metrics**: Some RCA methods require the anomalous KPI metrics detected by
-  certain anomaly detector.
+- **Abnormal time series data in an incident window**: The RCA methods require the anomalous 
+  KPI metrics in an incident window.
 
-Let's take ``BayesianNetwork`` as an example. Suppose that ``graph_df`` is a pandas dataframe of
-the graph representing causal relationships between metrics (how to construct such causal graph
-will be discussed later), and ``df`` is a pandas dataframe containing the historical observed time series 
+Let's take ``BayesianNetwork`` as an example. Suppose that ``graph_df`` is the pandas dataframe of
+a graph representing the causal relationships between metrics (how to construct such causal graph
+will be discussed later), and ``df`` is the pandas dataframe containing the historical observed time series 
 data (e.g., the index is the timestamp and each column represents one monitored metric). To train a 
 ``BayesianNetwork``, you can simply run the following code:
 
 ```python
 from pyrca.analyzers.bayesian import BayesianNetwork
 model = BayesianNetwork(config=BayesianNetwork.config_class(graph=graph_df))
 model.train(df)
 model.save("model_folder")
 ```
 
 After the model is trained, you can use it to find root causes of an incident given a list of anomalous
-metrics detected by a certain anomaly detector, e.g.,
+metrics detected by a certain anomaly detector (you can use the stats-based detector supported in PyRCA
+or other anomaly detection methods supported by our [Merlion](https://github.com/salesforce/Merlion) library), 
+e.g.,
 
 ```python
 from pyrca.analyzers.bayesian import BayesianNetwork
 model = BayesianNetwork.load("model_folder")
 results = model.find_root_causes(["observed_anomalous_metric", ...])
 print(results.to_dict())
 ```
@@ -120,24 +124,24 @@
 where ``abnormal_data`` is the time series data collected in an incident window.
 
 As mentioned above, some RCA methods such as ``BayesianNetwork`` require causal graphs as their inputs. To construct such causal
 graphs from the observed time series data, you can utilize our tool by running ``python -m pyrca.tools``.
 This command will launch a Dash app for time series data analysis and causal discovery.
 ![alt text](https://github.com/salesforce/PyRCA/raw/main/docs/_static/dashboard.png)
 
-The dashboard allows you to try different causal discovery methods, adjust causal discovery parameters,
-add domain knowledge constraints (e.g., root/leaf nodes, forbidden/required links), and visualize
-the generated causal graphs. It makes easier for manually revising causal graphs based on domain knowledge.
-You can download the graph generated by this tool if you satisfy with it. The graph can be used by the RCA 
-methods supported in PyRCA.
-
-Instead of using this dashboard, you can also write code for building such graphs. The package 
-``pyrca.graphs.causal`` includes several popular causal discovery methods you can use. All of these methods
-support domain knowledge constraints. Suppose ``df`` is the observed time series data
-and you want to apply the PC algorithm for building causal graphs, then the following code will help:
+The dashboard enables users to experiment with different causal discovery methods, customize causal discovery 
+parameters, add domain knowledge constraints (e.g., root/leaf nodes, forbidden/required links), and visualize 
+the generated causal graphs. This feature simplifies the process of manually revising causal graphs based on 
+domain knowledge. Users can download the graph generated by this tool if they are satisfied with it. The graph 
+can then be used by the RCA methods supported in PyRCA.
+
+Alternatively, users can write code to build such graphs instead of using the dashboard. The package 
+``pyrca.graphs.causal`` includes several popular causal discovery methods that users can leverage. 
+All of these methods support domain knowledge constraints. For instance, if users wish to apply the PC 
+algorithm for building causal graphs on the observed time series data ``df``, the following code can be used:
 
 ```python
 from pyrca.graphs.causal.pc import PC
 model = PC(PC.config_class())
 graph_df = model.train(df)
 ```
 
@@ -174,15 +178,15 @@
 
 [Here](https://github.com/salesforce/PyRCA/tree/main/pyrca/applications/example) is a real-world example
 of applying ``BayesianNetwork`` to build a solution for RCA, which is adapted from our internal use cases. 
 The "config" folder includes the settings for the stats-based anomaly detector and the domain knowledge. 
 The "models" folder stores the causal graph and the trained Bayesian network. The ``RCAEngine`` class in the "rca.py" 
 file implements the methods for building causal graphs, training Bayesian networks and finding root causes 
 by utilizing the modules provided by PyRCA. You can directly use this class if the stats-based anomaly detector 
-and Bayesian inference are suitable for your RCA problems. For example, given a time series dataframe ``df``, 
+and Bayesian inference are suitable for your problems. For example, given a time series dataframe ``df``, 
 you can build and train a Bayesian network via the following code:
 
 ```python
 from pyrca.applications.example.rca import RCAEngine
 engine = RCAEngine()
 engine.build_causal_graph(
     df=df,
```

#### html2text {}

```diff
@@ -2,94 +2,100 @@
 [https://img.shields.io/badge/Python-3.7,_3.8,_3.9-blue] [PyPI] [Documentation]
                                [Downloads] [DOI]
 ## Table of Contents 1. [Introduction](#introduction) 2. [Installation]
 (#installation) 3. [Getting Started](#getting-started) 4. [Documentation]
 (https://fuzzy-disco-r42n6p1.pages.github.io/) 5. [Tutorial](https://
 github.com/salesforce/PyRCA/tree/main/examples) 6. [Example](#application-
 example) 7. [Benchmarks](#benchmarks) 8. [How to Contribute](#how-to-
-contribute) ## Introduction With the rapidly growing adoption of microservices
-architectures, multi-service applications become the standard paradigm in real-
-world IT applications. A multi-service application usually contains hundreds of
-interacting services, making it harder to detect service failures and identify
-the root causes. Root cause analysis (RCA) methods usually leverage the KPI
-metrics, traces or logs monitored on those services to determine the root
-causes when a system failure is detected, helping engineers and SREs in the
-troubleshooting process. PyRCA is a Python machine-learning library designed
-for root cause analysis, offering multiple state-of-the-art RCA algorithms and
-an end-to-end pipeline for building RCA solutions. Currently, PyRCA mainly
-focuses on metric-based RCA including two types of algorithms: 1. Identifying
-anomalous metrics in parallel with the observed anomaly via metric data
-analysis, e.g., Îµ-diagnosis, and 2. Identifying root causes based a topology/
-causal graph representing the causal relationships between the observed
-metrics, e.g., Bayesian inference, Random Walk. Besides, PyRCA provides a
-convenient tool for building causal graphs from the observed time series data
-and domain knowledge, helping users to develop graph-based solutions quickly.
-PyRCA also provides a benchmark for evaluating various RCA methods, which is
-valuable for industry and academic research. The following list shows the
-supported RCA methods in our library: 1. Îµ-Diagnosis 2. Bayesian Inference-
-based RCA (BI) 3. Random Walk-based RCA (RW) 4. Root Casue Discovery method
-(RCD) 5. Hypothesis Testing-based RCA (HT) We will continue improving this
-library to make it more comprehensive in the future. In the future, PyRCA will
-support trace and log based RCA methods as well. ## Installation You can
-install ``pyrca`` from PyPI by calling ``pip install sfr-pyrca``. You may
-install from source by cloning the PyRCA repo, navigating to the root
-directory, and calling ``pip install .``, or ``pip install -e .`` to install in
-editable mode. You may install additional dependencies: - **For plotting &
-visualization**: Calling ``pip install sfr-pyrca[plot]``, or ``pip install .
-[plot]`` from the root directory of the repo. - **Install all the
+contribute) ## Introduction The adoption of microservices architectures is
+growing at a rapid pace, making multi-service applications the standard
+paradigm in real-world IT applications. Typically, a multi-service application
+consists of hundreds of interacting services, making it increasingly
+challenging to detect service failures and identify their root causes. Root
+cause analysis (RCA) methods typically rely on KPI metrics, traces, or logs
+monitored on these services to determine the root causes when a system failure
+is detected. Such methods can aid engineers and SREs in the troubleshooting
+process. PyRCA is a Python machine-learning library designed to facilitate root
+cause analysis by offering various state-of-the-art RCA algorithms and an end-
+to-end pipeline for building RCA solutions. At present, PyRCA primarily focuses
+on metric-based RCA, including two types of algorithms: (1) identifying
+anomalous metrics in parallel with the observed anomaly through metric data
+analysis, such as Îµ-diagnosis, and (2) identifying root causes based on a
+topology/causal graph representing the causal relationships between the
+observed metrics, such as Bayesian inference and Random Walk. PyRCA also
+provides a convenient tool for building causal graphs from the observed time
+series data and domain knowledge, enabling users to develop graph-based
+solutions quickly. Furthermore, PyRCA offers a benchmark for evaluating various
+RCA methods, which is valuable for industry and academic research. The
+following list shows the supported RCA methods in our library: 1. [Îµ-
+Diagnosis](https://dl.acm.org/doi/10.1145/3308558.3313653) 2. Bayesian
+Inference-based RCA (BI) 3. Random Walk-based RCA (RW) 4. [Root Casue Discovery
+method (RCD)](https://openreview.net/pdf?id=weoLjoYFvXY) 5. [Hypothesis
+Testing-based RCA (HT)](https://dl.acm.org/doi/10.1145/3534678.3539041) We will
+continue improving this library to make it more comprehensive in the future. In
+the future, PyRCA will support trace and log-based RCA methods as well. ##
+Installation You can install ``pyrca`` from PyPI by calling ``pip install sfr-
+pyrca``. You may install from source by cloning the PyRCA repo, navigating to
+the root directory, and calling ``pip install .``, or ``pip install -e .`` to
+install in editable mode. You may install additional dependencies: - **For
+plotting & visualization**: Calling ``pip install sfr-pyrca[plot]``, or ``pip
+install .[plot]`` from the root directory of the repo. - **Install all the
 dependencies**: Calling ``pip install sfr-pyrca[all]``, or ``pip install .
 [all]`` from the root directory of the repo. ## Getting Started PyRCA provides
 a unified interface for training RCA models and finding root causes. To apply a
-certain RCA method, you only need to specify: - **The select RCA method**:
-e.g., ``BayesianNetwork``, ``EpsilonDiagnosis``. - **The RCA configuration**:
-e.g., ``BayesianNetworkConfig``, ``EpsilonDiagnosisConfig``. - **Time series
-data for initialization or training**: e.g., A time series data in a pandas
-dataframe. - **Some detected anomalous KPI metrics**: Some RCA methods require
-the anomalous KPI metrics detected by certain anomaly detector. Let's take
-``BayesianNetwork`` as an example. Suppose that ``graph_df`` is a pandas
-dataframe of the graph representing causal relationships between metrics (how
-to construct such causal graph will be discussed later), and ``df`` is a pandas
-dataframe containing the historical observed time series data (e.g., the index
-is the timestamp and each column represents one monitored metric). To train a
-``BayesianNetwork``, you can simply run the following code: ```python from
-pyrca.analyzers.bayesian import BayesianNetwork model = BayesianNetwork
+certain RCA method, you only need to specify: - **The selected RCA method**:
+e.g., ``BayesianNetwork``, ``EpsilonDiagnosis``. - **The method
+configuration**: e.g., ``BayesianNetworkConfig``, ``EpsilonDiagnosisConfig``. -
+**Time series data for initialization/training**: e.g., A time series data in a
+pandas dataframe. - **Abnormal time series data in an incident window**: The
+RCA methods require the anomalous KPI metrics in an incident window. Let's take
+``BayesianNetwork`` as an example. Suppose that ``graph_df`` is the pandas
+dataframe of a graph representing the causal relationships between metrics (how
+to construct such causal graph will be discussed later), and ``df`` is the
+pandas dataframe containing the historical observed time series data (e.g., the
+index is the timestamp and each column represents one monitored metric). To
+train a ``BayesianNetwork``, you can simply run the following code: ```python
+from pyrca.analyzers.bayesian import BayesianNetwork model = BayesianNetwork
 (config=BayesianNetwork.config_class(graph=graph_df)) model.train(df)
 model.save("model_folder") ``` After the model is trained, you can use it to
 find root causes of an incident given a list of anomalous metrics detected by a
-certain anomaly detector, e.g., ```python from pyrca.analyzers.bayesian import
-BayesianNetwork model = BayesianNetwork.load("model_folder") results =
-model.find_root_causes(["observed_anomalous_metric", ...]) print
-(results.to_dict()) ``` For other RCA methods, you can write similar code as
-above for finding root causes. For example, if you want to try
+certain anomaly detector (you can use the stats-based detector supported in
+PyRCA or other anomaly detection methods supported by our [Merlion](https://
+github.com/salesforce/Merlion) library), e.g., ```python from
+pyrca.analyzers.bayesian import BayesianNetwork model = BayesianNetwork.load
+("model_folder") results = model.find_root_causes(["observed_anomalous_metric",
+...]) print(results.to_dict()) ``` For other RCA methods, you can write similar
+code as above for finding root causes. For example, if you want to try
 ``EpsilonDiagnosis``, you can initalize ``EpsilonDiagnosis`` as follows:
 ```python from pyrca.analyzers.epsilon_diagnosis import EpsilonDiagnosis model
 = EpsilonDiagnosis(config=EpsilonDiagnosis.config_class(alpha=0.01))
 model.train(normal_data) ``` Here ``normal_data`` is the historically observed
 time series data without anomalies. To identify root causes, you can run:
 ```python results = model.find_root_causes(abnormal_data) print(results.to_dict
 ()) ``` where ``abnormal_data`` is the time series data collected in an
 incident window. As mentioned above, some RCA methods such as
 ``BayesianNetwork`` require causal graphs as their inputs. To construct such
 causal graphs from the observed time series data, you can utilize our tool by
 running ``python -m pyrca.tools``. This command will launch a Dash app for time
 series data analysis and causal discovery. ![alt text](https://github.com/
-salesforce/PyRCA/raw/main/docs/_static/dashboard.png) The dashboard allows you
-to try different causal discovery methods, adjust causal discovery parameters,
-add domain knowledge constraints (e.g., root/leaf nodes, forbidden/required
-links), and visualize the generated causal graphs. It makes easier for manually
-revising causal graphs based on domain knowledge. You can download the graph
-generated by this tool if you satisfy with it. The graph can be used by the RCA
-methods supported in PyRCA. Instead of using this dashboard, you can also write
-code for building such graphs. The package ``pyrca.graphs.causal`` includes
-several popular causal discovery methods you can use. All of these methods
-support domain knowledge constraints. Suppose ``df`` is the observed time
-series data and you want to apply the PC algorithm for building causal graphs,
-then the following code will help: ```python from pyrca.graphs.causal.pc import
-PC model = PC(PC.config_class()) graph_df = model.train(df) ``` If you have
-some domain knowledge constraints, you may run: ```python from
+salesforce/PyRCA/raw/main/docs/_static/dashboard.png) The dashboard enables
+users to experiment with different causal discovery methods, customize causal
+discovery parameters, add domain knowledge constraints (e.g., root/leaf nodes,
+forbidden/required links), and visualize the generated causal graphs. This
+feature simplifies the process of manually revising causal graphs based on
+domain knowledge. Users can download the graph generated by this tool if they
+are satisfied with it. The graph can then be used by the RCA methods supported
+in PyRCA. Alternatively, users can write code to build such graphs instead of
+using the dashboard. The package ``pyrca.graphs.causal`` includes several
+popular causal discovery methods that users can leverage. All of these methods
+support domain knowledge constraints. For instance, if users wish to apply the
+PC algorithm for building causal graphs on the observed time series data
+``df``, the following code can be used: ```python from pyrca.graphs.causal.pc
+import PC model = PC(PC.config_class()) graph_df = model.train(df) ``` If you
+have some domain knowledge constraints, you may run: ```python from
 pyrca.graphs.causal.pc import PC model = PC(PC.config_class
 (domain_knowledge_file="file_path")) graph_df = model.train(df) ``` The domain
 knowledge file has a YAML format, e.g., ```yaml causal-graph: root-nodes: ["A",
 "B"] leaf-nodes: ["E", "F"] forbids: - ["A", "E"] requires: - ["A", "C"] ```
 This domain knowledge file states that: 1. Metrics A and B must the root nodes,
 2. Metrics E and F must be the leaf nodes, 3. There is no connection from A to
 E, and 4. There is a connection from A to C. You can write your domain
@@ -99,32 +105,31 @@
 ``BayesianNetwork`` to build a solution for RCA, which is adapted from our
 internal use cases. The "config" folder includes the settings for the stats-
 based anomaly detector and the domain knowledge. The "models" folder stores the
 causal graph and the trained Bayesian network. The ``RCAEngine`` class in the
 "rca.py" file implements the methods for building causal graphs, training
 Bayesian networks and finding root causes by utilizing the modules provided by
 PyRCA. You can directly use this class if the stats-based anomaly detector and
-Bayesian inference are suitable for your RCA problems. For example, given a
-time series dataframe ``df``, you can build and train a Bayesian network via
-the following code: ```python from pyrca.applications.example.rca import
-RCAEngine engine = RCAEngine() engine.build_causal_graph( df=df,
-run_pdag2dag=True, max_num_points=5000000, verbose=True ) bn =
-engine.train_bayesian_network(dfs=[df]) bn.print_probabilities() ``` After the
-Bayesian network is constructed, you can use it directly for finding root
-causes: ```python engine = RCAEngine() result = engine.find_root_causes_bn
-(anomalies=["conn_pool", "apt"]) pprint.pprint(result) ``` The inputs of
-``find_root_causes_bn`` is a list of the anomalous metrics detected by the
-stats-based anomaly detector. This method will estimate the probability of a
-node being a root cause and extract the paths from a potential root cause node
-to the leaf nodes. ## Benchmarks The following table summarizes the RCA
-performance of different methods on the simulated dataset. How to generate the
-simulated dataset can be found [here](https://github.com/salesforce/PyRCA/blob/
-main/examples/DataGeneration.ipynb), and how to test different RCA methods can
-be found [here](https://github.com/salesforce/PyRCA/blob/main/examples/
-Root%20Cause%20Analysis.ipynb).
+Bayesian inference are suitable for your problems. For example, given a time
+series dataframe ``df``, you can build and train a Bayesian network via the
+following code: ```python from pyrca.applications.example.rca import RCAEngine
+engine = RCAEngine() engine.build_causal_graph( df=df, run_pdag2dag=True,
+max_num_points=5000000, verbose=True ) bn = engine.train_bayesian_network(dfs=
+[df]) bn.print_probabilities() ``` After the Bayesian network is constructed,
+you can use it directly for finding root causes: ```python engine = RCAEngine()
+result = engine.find_root_causes_bn(anomalies=["conn_pool", "apt"])
+pprint.pprint(result) ``` The inputs of ``find_root_causes_bn`` is a list of
+the anomalous metrics detected by the stats-based anomaly detector. This method
+will estimate the probability of a node being a root cause and extract the
+paths from a potential root cause node to the leaf nodes. ## Benchmarks The
+following table summarizes the RCA performance of different methods on the
+simulated dataset. How to generate the simulated dataset can be found [here]
+(https://github.com/salesforce/PyRCA/blob/main/examples/DataGeneration.ipynb),
+and how to test different RCA methods can be found [here](https://github.com/
+salesforce/PyRCA/blob/main/examples/Root%20Cause%20Analysis.ipynb).
 | | Recall@1 | Recall@3 | Recall@5 | :---------------------------:|:----------
  -:|:-----------:|:-----------: | Îµ-Diagnosis | 0.06 Â± 0.02 | 0.16 Â± 0.04 |
 0.16 Â± 0.04 | | RCD | 0.28 Â± 0.05 | 0.29 Â± 0.05 | 0.30 Â± 0.05 | | Local-RCD
  | 0.44 Â± 0.05 | 0.70 Â± 0.05 | 0.70 Â± 0.05 | | Random Walk | 0.07 Â± 0.03 |
 0.20 Â± 0.04 | 0.24 Â± 0.04 | | Random Walk (PC) | 0.06 Â± 0.02 | 0.17 Â± 0.04
  | 0.21 Â± 0.04 | | Bayesian Inference | 0.15 Â± 0.04 | 0.35 Â± 0.05 | 0.43 Â±
 0.05 | | Bayesian Inference (PC) | 0.11 Â± 0.03 | 0.30 Â± 0.05 | 0.40 Â± 0.05 |
```

### Comparing `sfr-pyrca-0.0.1/docs/conf.py` & `sfr-pyrca-1.0.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `sfr-pyrca-0.0.1/pyrca/analyzers/base.py` & `sfr-pyrca-1.0.0/pyrca/analyzers/base.py`

 * *Files identical despite different names*

### Comparing `sfr-pyrca-0.0.1/pyrca/analyzers/bayesian.py` & `sfr-pyrca-1.0.0/pyrca/analyzers/bayesian.py`

 * *Files identical despite different names*

### Comparing `sfr-pyrca-0.0.1/pyrca/analyzers/epsilon_diagnosis.py` & `sfr-pyrca-1.0.0/pyrca/analyzers/epsilon_diagnosis.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,42 +16,41 @@
 
 
 @dataclass
 class EpsilonDiagnosisConfig(BaseConfig):
     """
     The configuration class for the epsilon-diagnosis algorithm for Root Cause Analysis.
 
-    :param alpha: desired significance level (float) in (0, 1). Default: 0.05.
+    :param alpha: The desired significance level (float) in (0, 1). Default: 0.05.
     :param bootstrap_time: Bootstrap times.
     :param root_cause_top_k: The maximum number of root causes in the results.
     """
 
     alpha: float = 0.05
     bootstrap_time: int = 200
     root_cause_top_k: int = 3
 
 
 class EpsilonDiagnosis(BaseRCA):
     """
-    The epsilon-diagnosis method for Root Cause Analysis.
-
-    epsilon-Diagnosis: Unsupervised and Real-time Diagnosis of Small window Long-tail Latency in Large-scale Microservice Platforms.
+    The epsilon-diagnosis method for Root Cause Analysis. If using this method, please cite the original work:
+    `epsilon-Diagnosis: Unsupervised and Real-time Diagnosis of Small window Long-tail Latency in Large-scale Microservice Platforms`.
     """
 
     config_class = EpsilonDiagnosisConfig
 
     def __init__(self, config: EpsilonDiagnosisConfig):
         super().__init__()
         self.config = config
 
     def train(self, normal_df: pd.DataFrame, **kwargs):
         """
         Two variable correlation analysis given the training time series.
 
-        :param normal_df: Dataframe of normal data.
+        :param normal_df: A pandas dataframe of normal data.
         """
         self.normal_df = normal_df
 
         def _samples(array, times=50):
             return np.random.choice(array, (array.shape[0], times))
 
         # bootstrapping to calculate the p-value
@@ -72,15 +71,15 @@
             zip(normal_df.columns, np.apply_along_axis(np.quantile, 0, normal_correlations, q=1 - self.config.alpha))
         )
 
     def find_root_causes(self, abnormal_df: pd.DataFrame, **kwargs):
         """
         Finds the root causes given the abnormal dataset.
 
-        :param abnormal_df: DataFrame of abnormal data.
+        :param abnormal_df: A pandas dataFrame of abnormal data.
         :return: A list of the found root causes.
         """
         root_cause_nodes = []
         self.correlations = {}
         for colname in abnormal_df.columns:
             if np.var(self.normal_df[colname].values) == 0 or np.var(abnormal_df[colname].values) == 0:
                 self.correlations[colname] = 0
```

### Comparing `sfr-pyrca-0.0.1/pyrca/analyzers/ht.py` & `sfr-pyrca-1.0.0/pyrca/analyzers/ht.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,17 +33,17 @@
     graph: Union[pd.DataFrame, str]
     aggregator: str = "max"
     root_cause_top_k: int = 3
 
 
 class HT(BaseRCA):
     """
-    Regression-based Hypothesis Testing method for Root Cause Analysis
-
-    Causal Inference-Based Root Cause Analysis for Online Service Systems with Intervention Recognition.
+    Regression-based Hypothesis Testing method for Root Cause Analysis.
+    If using this explainer, please cite the original work:
+    `Causal Inference-Based Root Cause Analysis for Online Service Systems with Intervention Recognition`.
     """
 
     config_class = HTConfig
 
     def __init__(self, config: HTConfig):
         super().__init__()
         self.config = config
@@ -72,15 +72,15 @@
         else:
             raise f"Unknown aggregator {name}"
 
     def train(self, normal_df: pd.DataFrame, **kwargs):
         """
         Train regression model for each node based on its parents. Build the score functions.
 
-        :param normal_df: DataFrame of normal data.
+        :param normal_df: A pandas dataFrame of normal data.
         """
         assert self.graph is not None, "The graphs is not set."
 
         for node in list(self.graph):
             parents = list(self.graph.predecessors(node))
             normal_x = normal_df[parents].values
             normal_y = normal_df[node].values
@@ -96,17 +96,17 @@
 
     def find_root_causes(
         self, abnormal_df: pd.DataFrame, anomalous_metrics: str = None, adjustment: bool = False, **kwargs
     ):
         """
         Finds the root causes given the abnormal dataset.
 
-        :param abnormal_df: DataFrame of abnormal data.
-        :param anomalous_metrics: the name of detected anomalous metrics, it is used to print the path from root nodes.
-        :param adjustment: whether to perform descendant adjustment.
+        :param abnormal_df: A pandas dataFrame of abnormal data.
+        :param anomalous_metrics: The name of detected anomalous metrics, it is used to print the path from root nodes.
+        :param adjustment: Whether to perform descendant adjustment.
         :return: A list of the found root causes.
         """
         node_scores = {}
         for node in list(self.graph):
             parents = list(self.graph.predecessors(node))
             abnormal_x = abnormal_df[parents].values
             abnormal_y = abnormal_df[node].values
```

### Comparing `sfr-pyrca-0.0.1/pyrca/analyzers/random_walk.py` & `sfr-pyrca-1.0.0/pyrca/analyzers/random_walk.py`

 * *Files identical despite different names*

### Comparing `sfr-pyrca-0.0.1/pyrca/analyzers/rcd.py` & `sfr-pyrca-1.0.0/pyrca/analyzers/rcd.py`

 * *Files 11% similar despite different names*

```diff
@@ -19,22 +19,22 @@
 
 
 @dataclass
 class RCDConfig(BaseConfig):
     """
     The configuration class for the RCD algorithm for Root Cause Analysis
 
-    :param start_alpha: desired start significance level (float) in (0, 1) for search.
-    :param alpha_step: search step for alpha.
-    :param alpha_limit: maximum alpha for search.
-    :param localized: whether use local method.
-    :param gamma: chunk size.
-    :param bins: number of bins to discretize data.
-    :param K: top-k root causes.
-    :param f_node: name of anomaly variable.
+    :param start_alpha: The desired start significance level (float) in (0, 1) for search.
+    :param alpha_step: The search step for alpha.
+    :param alpha_limit: The maximum alpha for search.
+    :param localized: Whether use local method.
+    :param gamma: Chunk size.
+    :param bins: The number of bins to discretize data.
+    :param K: Top-k root causes.
+    :param f_node: The name of anomaly variable.
     :param verbose: True iff verbose output should be printed. Default: False.
     """
 
     start_alpha: float = 0.01
     alpha_step: float = 0.1
     alpha_limit: float = 1
     localized: bool = True
@@ -44,17 +44,16 @@
     f_node: str = "F-node"
     verbose: bool = False
     ci_test: CIT = chisq
 
 
 class RCD(BaseRCA):
     """
-    The RCD algorithm for Root Cause Analysis
-
-    Root Cause Analysis of Failures in Microservices through Causal Discovery
+    The RCD algorithm for Root Cause Analysis. If using this explainer, please cite the original work:
+    `Root Cause Analysis of Failures in Microservices through Causal Discovery`.
     """
 
     config_class = RCDConfig
 
     def __init__(self, config: RCDConfig):
         super().__init__()
         self.config = config
@@ -64,12 +63,13 @@
         model training is implemented in find_root_causes function.
         """
         pass
 
     def find_root_causes(self, normal_df: pd.DataFrame, abnormal_df: pd.DataFrame, **kwargs):
         """
         Finds the root causes given the abnormal dataset.
+
         :return: A list of the found root causes.
         """
         result, _ = rcd.run_multi_phase(normal_df, abnormal_df, self.config.to_dict())
         root_cause_nodes = [(key, None) for key in result[: self.config.k]]
         return RCAResults(root_cause_nodes=root_cause_nodes)
```

### Comparing `sfr-pyrca-0.0.1/pyrca/applications/example/dataset.py` & `sfr-pyrca-1.0.0/pyrca/applications/example/dataset.py`

 * *Files identical despite different names*

### Comparing `sfr-pyrca-0.0.1/pyrca/applications/example/rca.py` & `sfr-pyrca-1.0.0/pyrca/applications/example/rca.py`

 * *Files 5% similar despite different names*

```diff
@@ -49,23 +49,35 @@
             "bn": self._find_root_causes_bn,
             "bayesian": self._find_root_causes_bn,
             "rw": self._find_root_causes_rw,
             "random_walk": self._find_root_causes_rw,
         }
 
     def build_causal_graph(
-        self,
-        df,
-        domain_knowledge_file=None,
-        run_pdag2dag=True,
-        max_num_points=5000000,
-        method_class=None,
-        verbose=False,
-        **kwargs,
+            self,
+            df,
+            domain_knowledge_file=None,
+            run_pdag2dag=True,
+            max_num_points=5000000,
+            method_class=None,
+            verbose=False,
+            **kwargs,
     ):
+        """
+        Builds the causal graph via causal discovery methods given the observed time series data.
+
+        :param df: The input time series data in a pandas dataframe.
+        :param domain_knowledge_file: The domain knowledge file.
+        :param run_pdag2dag: Whether to run the "partial DAG to DAG" function (sometimes the output of
+            a causal discovery is a partial DAG instead of DAG).
+        :param max_num_points: The maximum number of the training timestamps.
+        :param method_class: The class of a causal discovery method, e.g., FGES, PC defined in
+            `pyrca.graphs.causal`.
+        :param verbose: Whether to print debugging messages.
+        """
         from pyrca.graphs.causal.pc import PC
 
         df = df.iloc[:max_num_points] if max_num_points is not None else df
         if verbose:
             self.logger.info(f"The shape of the training data for infer_causal_graph: {df.shape}")
         if domain_knowledge_file is None:
             domain_knowledge_file = os.path.join(
@@ -83,15 +95,29 @@
             )
         )
         adjacency_df = model.train(df)
         adjacency_df.to_pickle(os.path.join(self.model_dir, self.adjacency_df_filename))
         PC.dump_to_tetrad_json(adjacency_df, self.model_dir)
         return adjacency_df
 
-    def train_bayesian_network(self, dfs, domain_knowledge_file=None, config_file=None, verbose=False):
+    def train_bayesian_network(
+            self,
+            dfs,
+            domain_knowledge_file=None,
+            config_file=None,
+            verbose=False
+    ):
+        """
+        Trains the Bayesian network parameters given the causal graph and the time series data.
+
+        :param dfs: The time series data for training (either a pandas dataframe or a list of pandas dataframe).
+        :param domain_knowledge_file: The domain knowledge file.
+        :param config_file: The configuration file for Bayesian network.
+        :param verbose: Whether to print debugging messages.
+        """
         from pyrca.utils.domain import DomainParser
         from pyrca.analyzers.bayesian import BayesianNetwork, BayesianNetworkConfig
 
         if isinstance(dfs, pd.DataFrame):
             assert dfs.shape[0] > 10000, "The length of df is less than 10000."
             if verbose:
                 self.logger.info(f"The training data shape for the Bayesian network: {dfs.shape}")
@@ -124,19 +150,19 @@
         )
         bayesian_network.train(dfs=dfs)
         bayesian_network.add_root_causes(domain.get_root_causes())
         bayesian_network.save(self.model_dir, name=self.bn_filename)
         return bayesian_network
 
     def train_detector(
-        self,
-        df: Union[pd.DataFrame, Dict],
-        config_file: Optional[str] = None,
-        use_separate_models=True,
-        additional_config: Dict = None,
+            self,
+            df: Union[pd.DataFrame, Dict],
+            config_file: Optional[str] = None,
+            use_separate_models=True,
+            additional_config: Dict = None,
     ) -> Dict:
         """
         Trains the detector(s) given the time series data.
 
         :param df: The training dataset which can be a pandas dataframe or a dict with format
             discussed in https://pandas.pydata.org/docs/reference/api/pandas.DataFrame.from_dict.html.
         :param config_file: The configuration file path.
@@ -199,20 +225,20 @@
 
         :param anomalies: A list of anomalous metrics found by any anomaly detector.
         :return: The root cause analysis results.
         """
         return self._find_root_causes_bn(None, anomalies, **kwargs).to_list()
 
     def find_root_causes(
-        self,
-        df: Union[pd.DataFrame, Dict],
-        detector: Union[Dict, BaseDetector],
-        rca_method: Optional[str] = None,
-        known_anomalies: List = None,
-        **kwargs,
+            self,
+            df: Union[pd.DataFrame, Dict],
+            detector: Union[Dict, BaseDetector],
+            rca_method: Optional[str] = None,
+            known_anomalies: List = None,
+            **kwargs,
     ):
         """
         Finds the potential root causes given an incident window.
 
         :param df: The training dataset which can be a pandas dataframe or a dict with format
             discussed in https://pandas.pydata.org/docs/reference/api/pandas.DataFrame.from_dict.html.
         :param detector: The anomaly detector (e.g., StatsDetector). It can either be a single model
```

### Comparing `sfr-pyrca-0.0.1/pyrca/base.py` & `sfr-pyrca-1.0.0/pyrca/base.py`

 * *Files identical despite different names*

### Comparing `sfr-pyrca-0.0.1/pyrca/graphs/causal/base.py` & `sfr-pyrca-1.0.0/pyrca/graphs/causal/base.py`

 * *Files 5% similar despite different names*

```diff
@@ -51,19 +51,27 @@
         """
         Builds the causal graph given the training dataset.
 
         :param df: The training dataset.
         :return: The adjacency matrix.
         """
         df = df.iloc[: self.config.max_num_points] if self.config.max_num_points is not None else df
-        parser = DomainParser(self.config.domain_knowledge_file)
 
-        adjacency_df = self._train(
-            df=df, forbids=parser.get_forbid_links(df.columns), requires=parser.get_require_links(), **kwargs
-        )
+        if self.config.domain_knowledge_file:
+            parser = DomainParser(self.config.domain_knowledge_file)
+            adjacency_df = self._train(
+                df=df, forbids=parser.get_forbid_links(df.columns), requires=parser.get_require_links(), **kwargs
+            )
+        else:
+            if "forbids" not in kwargs:
+                kwargs["forbids"] = []
+            if "requires" not in kwargs:
+                kwargs["requires"] = []
+            adjacency_df = self._train(df=df, **kwargs)
+
         var_names = adjacency_df.columns
         if self.config.run_pdag2dag:
             dag, flag = CausalModel.pdag2dag(adjacency_df.values)
             if flag is False:
                 raise RuntimeError("Orientation of the undirected edges failed.")
             adjacency_df = pd.DataFrame({var_names[i]: dag[:, i] for i in range(len(var_names))}, index=var_names)
         return adjacency_df
```

### Comparing `sfr-pyrca-0.0.1/pyrca/graphs/causal/fges.py` & `sfr-pyrca-1.0.0/pyrca/graphs/causal/fges.py`

 * *Files identical despite different names*

### Comparing `sfr-pyrca-0.0.1/pyrca/graphs/causal/ges.py` & `sfr-pyrca-1.0.0/pyrca/graphs/causal/ges.py`

 * *Files identical despite different names*

### Comparing `sfr-pyrca-0.0.1/pyrca/graphs/causal/lingam.py` & `sfr-pyrca-1.0.0/pyrca/graphs/causal/lingam.py`

 * *Files identical despite different names*

### Comparing `sfr-pyrca-0.0.1/pyrca/graphs/causal/pc.py` & `sfr-pyrca-1.0.0/pyrca/graphs/causal/pc.py`

 * *Files identical despite different names*

### Comparing `sfr-pyrca-0.0.1/pyrca/outliers/base.py` & `sfr-pyrca-1.0.0/pyrca/outliers/base.py`

 * *Files identical despite different names*

### Comparing `sfr-pyrca-0.0.1/pyrca/outliers/stats.py` & `sfr-pyrca-1.0.0/pyrca/outliers/stats.py`

 * *Files identical despite different names*

### Comparing `sfr-pyrca-0.0.1/pyrca/simulation/data_gen.py` & `sfr-pyrca-1.0.0/pyrca/simulation/data_gen.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,19 +22,19 @@
     low, high = rng.choice(segments)
     return rng.uniform(low=low, high=high)
 
 
 @dataclass
 class DAGGenConfig:
     """
-    The configuration class of generating DAG
+    The configuration class of generating DAG.
 
-    :param num_node: Number of nodes in DAG
-    :param num_edge: Number of edges in DAG
-    :param rng: random generator
+    :param num_node: Number of nodes in DAG.
+    :param num_edge: Number of edges in DAG.
+    :param rng: A random generator.
     """
 
     num_node: int = 20
     num_edge: int = 30
     rng: np.random.Generator = None
 
     def __post_init__(self):
@@ -53,15 +53,15 @@
         self.config = config
 
     def gen(self):
         """
         Generate a directed acyclic graphs with a single end.
         The first node with index of 0 is the only end that does not have results.
 
-        :return: a matrix, where matrix[i, j] != 0 means i is the cause of j
+        :return: A matrix, where matrix[i, j] != 0 means i is the cause of j.
         """
         num_edge = min(
             max(self.config.num_edge, self.config.num_node - 1),
             int(self.config.num_node * (self.config.num_node - 1) / 2),
         )
         matrix = np.zeros((self.config.num_node, self.config.num_node))
 
@@ -80,23 +80,23 @@
                 num_edge -= 1
         return matrix
 
 
 @dataclass
 class DataGenConfig:
     """
-    The configuration class of generating RCA Data
+    The configuration class of generating RCA Data.
 
-    :param dag: The dependency graph
+    :param dag: The dependency graph.
     :param noise_type: probability distribution of each node's noise,
-        it is required to be in valid_noise type list
+        it is required to be in valid_noise type list.
     :param func_type: causal function form of each node,
-        it is required to be in valid_noise type list
-    :param num_samples: Number of samples
-    :param weight_generator: random generator for model weights
+        it is required to be in valid_noise type list.
+    :param num_samples: Number of samples.
+    :param weight_generator: random generator for model weights.
     """
 
     dag: np.ndarray
     noise_type: str = None
     func_type: str = None
     num_samples: int = 5000
     weight_generator: str = "normal"
@@ -154,15 +154,15 @@
             ), f"{self.weight_generator} is not supported. The valid value is {self._VALID_WEIGHT}"
 
 
 class DataGen:
     """
     Normal data generation.
 
-    generate data (n_samples, n_nodes) according to  DAG matrix
+    Generates data (n_samples, n_nodes) according to DAG matrix.
     """
 
     config_class = DataGenConfig
 
     def __init__(self, config: DataGenConfig):
         self.config = config
 
@@ -170,20 +170,20 @@
         r"""
         For each node
 
         .. math:: x_{i} = \sum_{x_{j} \in Pa(x_i)} A_{ij} f_i(x_j) +  \beta_i * noise_i
 
         where f_i indicates element-wise transformation, it is chosen from identity, square, sin, tanh,
         noise_i is chosen from Exponential(1), Normal(0,1), Uniform(-0.5,0.5), Laplace(0, 1)
-        Both the weights of A_{ij} and \beta_i are chosen from _uniform_weight or _normal_weight
+        Both the weights of A_{ij} and \beta_i are chosen from _uniform_weight or _normal_weight.
 
         :returns:
-            - data: (num_samples, num_node) data of each variable x_i
-            - parent_weights: (num_node, num_node) Combination weights of each variable A_{ij}
-            - noise_weights: (num_node,) noise weight for of each variable \beta_i
+            - data: (num_samples, num_node) data of each variable x_i.
+            - parent_weights: (num_node, num_node) Combination weights of each variable A_{ij}.
+            - noise_weights: (num_node,) noise weight for of each variable \beta_i.
         """
 
         num_node, _ = self.config.dag.shape
         num_samples = self.config.num_samples
         graph = self.config.dag
 
         data = np.zeros((num_samples, num_node))
@@ -208,26 +208,26 @@
 
 
 @dataclass
 class AnomalyDataGenConfig:
     """
     The configuration class of generating RCA Data.
 
-    :param parent_weights: The weights of parents of each node
-    :param noise_weights: The noise weights of each node
+    :param parent_weights: The weights of parents of each node.
+    :param noise_weights: The noise weights of each node.
     :param noise_type: probability distribution of each node's noise,
-        it is required to be in valid_noise type list
+        it is required to be in valid_noise type list.
     :param func_type: causal function form of each node,
-        it is required to be in valid_noise type list
-    :param baseline: baseline of normal data
-    :param threshold: threshold to differentiate anomaly data from stats-based anomaly detector
-    :param num_samples: Number of anomaly samples
+        it is required to be in valid_noise type list.
+    :param baseline: baseline of normal data.
+    :param threshold: threshold to differentiate anomaly data from stats-based anomaly detector.
+    :param num_samples: Number of anomaly samples.
     :param anomaly_type: 0 change the weight of noise term, 1 add a constant shift to noise term,
-        2 change the weight of parent nodes
-    :param weight_generator: random generator for model weights
+        2 change the weight of parent nodes.
+    :param weight_generator: random generator for model weights.
     """
 
     parent_weights: np.array
     noise_weights: np.array
     noise_type: str
     func_type: str
     baseline: float
@@ -261,29 +261,29 @@
             ), f"{self.weight_generator} is not supported. The valid value is {self._VALID_WEIGHT}"
 
 
 class AnomalyDataGen:
     """
     Anomaly data generation.
 
-    Generate anomaly data (n_samples, n_nodes)
+    Generates anomaly data (n_samples, n_nodes).
     """
 
     config_class = AnomalyDataGenConfig
 
     def __init__(self, config: DataGenConfig):
         self.config = config
 
     def gen(self):
         """
-        Generate anomaly data by randomly choose the root cause nodes
+        Generate anomaly data by randomly choose the root cause nodes.
 
         :returns:
-            - data: (num_samples, num_node) data of each variable x_i in anomaly phase
-            - root causes: (num_node) root causes of anomaly data
+            - data: (num_samples, num_node) data of each variable x_i in anomaly phase.
+            - root causes: (num_node) root causes of anomaly data.
         """
         assert self.config.parent_weights.shape[0] == self.config.noise_weights.shape[0]
         num_node = self.config.parent_weights.shape[0]
 
         data = np.zeros((self.config.num_samples, num_node))
 
         # # Inject a fault
```

### Comparing `sfr-pyrca-0.0.1/pyrca/thirdparty/causallearn/graph/AdjacencyConfusion.py` & `sfr-pyrca-1.0.0/pyrca/thirdparty/causallearn/graph/AdjacencyConfusion.py`

 * *Files identical despite different names*

### Comparing `sfr-pyrca-0.0.1/pyrca/thirdparty/causallearn/graph/ArrowConfusion.py` & `sfr-pyrca-1.0.0/pyrca/thirdparty/causallearn/graph/ArrowConfusion.py`

 * *Files identical despite different names*

### Comparing `sfr-pyrca-0.0.1/pyrca/thirdparty/causallearn/graph/Dag.py` & `sfr-pyrca-1.0.0/pyrca/thirdparty/causallearn/graph/Dag.py`

 * *Files identical despite different names*

### Comparing `sfr-pyrca-0.0.1/pyrca/thirdparty/causallearn/graph/Edge.py` & `sfr-pyrca-1.0.0/pyrca/thirdparty/causallearn/graph/Edge.py`

 * *Files identical despite different names*

### Comparing `sfr-pyrca-0.0.1/pyrca/thirdparty/causallearn/graph/Edges.py` & `sfr-pyrca-1.0.0/pyrca/thirdparty/causallearn/graph/Edges.py`

 * *Files identical despite different names*

### Comparing `sfr-pyrca-0.0.1/pyrca/thirdparty/causallearn/graph/Endpoint.py` & `sfr-pyrca-1.0.0/pyrca/thirdparty/causallearn/graph/Endpoint.py`

 * *Files identical despite different names*

### Comparing `sfr-pyrca-0.0.1/pyrca/thirdparty/causallearn/graph/GeneralGraph.py` & `sfr-pyrca-1.0.0/pyrca/thirdparty/causallearn/graph/GeneralGraph.py`

 * *Files identical despite different names*

### Comparing `sfr-pyrca-0.0.1/pyrca/thirdparty/causallearn/graph/Graph.py` & `sfr-pyrca-1.0.0/pyrca/thirdparty/causallearn/graph/Graph.py`

 * *Files identical despite different names*

### Comparing `sfr-pyrca-0.0.1/pyrca/thirdparty/causallearn/graph/GraphClass.py` & `sfr-pyrca-1.0.0/pyrca/thirdparty/causallearn/graph/GraphClass.py`

 * *Files identical despite different names*

### Comparing `sfr-pyrca-0.0.1/pyrca/thirdparty/causallearn/graph/GraphNode.py` & `sfr-pyrca-1.0.0/pyrca/thirdparty/causallearn/graph/GraphNode.py`

 * *Files identical despite different names*

### Comparing `sfr-pyrca-0.0.1/pyrca/thirdparty/causallearn/graph/Node.py` & `sfr-pyrca-1.0.0/pyrca/thirdparty/causallearn/graph/Node.py`

 * *Files identical despite different names*

### Comparing `sfr-pyrca-0.0.1/pyrca/thirdparty/causallearn/graph/SHD.py` & `sfr-pyrca-1.0.0/pyrca/thirdparty/causallearn/graph/SHD.py`

 * *Files identical despite different names*

### Comparing `sfr-pyrca-0.0.1/pyrca/thirdparty/causallearn/score/LocalScoreFunction.py` & `sfr-pyrca-1.0.0/pyrca/thirdparty/causallearn/score/LocalScoreFunction.py`

 * *Files identical despite different names*

### Comparing `sfr-pyrca-0.0.1/pyrca/thirdparty/causallearn/score/LocalScoreFunctionClass.py` & `sfr-pyrca-1.0.0/pyrca/thirdparty/causallearn/score/LocalScoreFunctionClass.py`

 * *Files identical despite different names*

### Comparing `sfr-pyrca-0.0.1/pyrca/thirdparty/causallearn/search/ConstraintBased/PC.py` & `sfr-pyrca-1.0.0/pyrca/thirdparty/causallearn/search/ConstraintBased/PC.py`

 * *Files identical despite different names*

### Comparing `sfr-pyrca-0.0.1/pyrca/thirdparty/causallearn/search/ScoreBased/GES.py` & `sfr-pyrca-1.0.0/pyrca/thirdparty/causallearn/search/ScoreBased/GES.py`

 * *Files identical despite different names*

### Comparing `sfr-pyrca-0.0.1/pyrca/thirdparty/causallearn/utils/BackgroundKnowledge.py` & `sfr-pyrca-1.0.0/pyrca/thirdparty/causallearn/utils/BackgroundKnowledge.py`

 * *Files identical despite different names*

### Comparing `sfr-pyrca-0.0.1/pyrca/thirdparty/causallearn/utils/DAG2CPDAG.py` & `sfr-pyrca-1.0.0/pyrca/thirdparty/causallearn/utils/DAG2CPDAG.py`

 * *Files identical despite different names*

### Comparing `sfr-pyrca-0.0.1/pyrca/thirdparty/causallearn/utils/GESUtils.py` & `sfr-pyrca-1.0.0/pyrca/thirdparty/causallearn/utils/GESUtils.py`

 * *Files identical despite different names*

### Comparing `sfr-pyrca-0.0.1/pyrca/thirdparty/causallearn/utils/GraphUtils.py` & `sfr-pyrca-1.0.0/pyrca/thirdparty/causallearn/utils/GraphUtils.py`

 * *Files identical despite different names*

### Comparing `sfr-pyrca-0.0.1/pyrca/thirdparty/causallearn/utils/PCUtils/BackgroundKnowledgeOrientUtils.py` & `sfr-pyrca-1.0.0/pyrca/thirdparty/causallearn/utils/PCUtils/BackgroundKnowledgeOrientUtils.py`

 * *Files identical despite different names*

### Comparing `sfr-pyrca-0.0.1/pyrca/thirdparty/causallearn/utils/PCUtils/Helper.py` & `sfr-pyrca-1.0.0/pyrca/thirdparty/causallearn/utils/PCUtils/Helper.py`

 * *Files identical despite different names*

### Comparing `sfr-pyrca-0.0.1/pyrca/thirdparty/causallearn/utils/PCUtils/Meek.py` & `sfr-pyrca-1.0.0/pyrca/thirdparty/causallearn/utils/PCUtils/Meek.py`

 * *Files identical despite different names*

### Comparing `sfr-pyrca-0.0.1/pyrca/thirdparty/causallearn/utils/PCUtils/SkeletonDiscovery.py` & `sfr-pyrca-1.0.0/pyrca/thirdparty/causallearn/utils/PCUtils/SkeletonDiscovery.py`

 * *Files identical despite different names*

### Comparing `sfr-pyrca-0.0.1/pyrca/thirdparty/causallearn/utils/PCUtils/UCSepset.py` & `sfr-pyrca-1.0.0/pyrca/thirdparty/causallearn/utils/PCUtils/UCSepset.py`

 * *Files identical despite different names*

### Comparing `sfr-pyrca-0.0.1/pyrca/thirdparty/causallearn/utils/PDAG2DAG.py` & `sfr-pyrca-1.0.0/pyrca/thirdparty/causallearn/utils/PDAG2DAG.py`

 * *Files identical despite different names*

### Comparing `sfr-pyrca-0.0.1/pyrca/thirdparty/causallearn/utils/ScoreUtils.py` & `sfr-pyrca-1.0.0/pyrca/thirdparty/causallearn/utils/ScoreUtils.py`

 * *Files identical despite different names*

### Comparing `sfr-pyrca-0.0.1/pyrca/thirdparty/causallearn/utils/TXT2GeneralGraph.py` & `sfr-pyrca-1.0.0/pyrca/thirdparty/causallearn/utils/TXT2GeneralGraph.py`

 * *Files identical despite different names*

### Comparing `sfr-pyrca-0.0.1/pyrca/thirdparty/causallearn/utils/cit.py` & `sfr-pyrca-1.0.0/pyrca/thirdparty/causallearn/utils/cit.py`

 * *Files identical despite different names*

### Comparing `sfr-pyrca-0.0.1/pyrca/thirdparty/pgmpy/base/DAG.py` & `sfr-pyrca-1.0.0/pyrca/thirdparty/pgmpy/base/DAG.py`

 * *Files identical despite different names*

### Comparing `sfr-pyrca-0.0.1/pyrca/thirdparty/pgmpy/base/UndirectedGraph.py` & `sfr-pyrca-1.0.0/pyrca/thirdparty/pgmpy/base/UndirectedGraph.py`

 * *Files identical despite different names*

### Comparing `sfr-pyrca-0.0.1/pyrca/thirdparty/pgmpy/estimators/BayesianEstimator.py` & `sfr-pyrca-1.0.0/pyrca/thirdparty/pgmpy/estimators/BayesianEstimator.py`

 * *Files identical despite different names*

### Comparing `sfr-pyrca-0.0.1/pyrca/thirdparty/pgmpy/estimators/MLE.py` & `sfr-pyrca-1.0.0/pyrca/thirdparty/pgmpy/estimators/MLE.py`

 * *Files identical despite different names*

### Comparing `sfr-pyrca-0.0.1/pyrca/thirdparty/pgmpy/estimators/base.py` & `sfr-pyrca-1.0.0/pyrca/thirdparty/pgmpy/estimators/base.py`

 * *Files identical despite different names*

### Comparing `sfr-pyrca-0.0.1/pyrca/thirdparty/pgmpy/extern/tabulate.py` & `sfr-pyrca-1.0.0/pyrca/thirdparty/pgmpy/extern/tabulate.py`

 * *Files identical despite different names*

### Comparing `sfr-pyrca-0.0.1/pyrca/thirdparty/pgmpy/factors/FactorSet.py` & `sfr-pyrca-1.0.0/pyrca/thirdparty/pgmpy/factors/FactorSet.py`

 * *Files identical despite different names*

### Comparing `sfr-pyrca-0.0.1/pyrca/thirdparty/pgmpy/factors/base.py` & `sfr-pyrca-1.0.0/pyrca/thirdparty/pgmpy/factors/base.py`

 * *Files identical despite different names*

### Comparing `sfr-pyrca-0.0.1/pyrca/thirdparty/pgmpy/factors/continuous/ContinuousFactor.py` & `sfr-pyrca-1.0.0/pyrca/thirdparty/pgmpy/factors/continuous/ContinuousFactor.py`

 * *Files identical despite different names*

### Comparing `sfr-pyrca-0.0.1/pyrca/thirdparty/pgmpy/factors/discrete/CPD.py` & `sfr-pyrca-1.0.0/pyrca/thirdparty/pgmpy/factors/discrete/CPD.py`

 * *Files identical despite different names*

### Comparing `sfr-pyrca-0.0.1/pyrca/thirdparty/pgmpy/factors/discrete/DiscreteFactor.py` & `sfr-pyrca-1.0.0/pyrca/thirdparty/pgmpy/factors/discrete/DiscreteFactor.py`

 * *Files identical despite different names*

### Comparing `sfr-pyrca-0.0.1/pyrca/thirdparty/pgmpy/factors/discrete/JointProbabilityDistribution.py` & `sfr-pyrca-1.0.0/pyrca/thirdparty/pgmpy/factors/discrete/JointProbabilityDistribution.py`

 * *Files identical despite different names*

### Comparing `sfr-pyrca-0.0.1/pyrca/thirdparty/pgmpy/factors/distributions/CustomDistribution.py` & `sfr-pyrca-1.0.0/pyrca/thirdparty/pgmpy/factors/distributions/CustomDistribution.py`

 * *Files identical despite different names*

### Comparing `sfr-pyrca-0.0.1/pyrca/thirdparty/pgmpy/factors/distributions/GaussianDistribution.py` & `sfr-pyrca-1.0.0/pyrca/thirdparty/pgmpy/factors/distributions/GaussianDistribution.py`

 * *Files identical despite different names*

### Comparing `sfr-pyrca-0.0.1/pyrca/thirdparty/pgmpy/factors/distributions/base.py` & `sfr-pyrca-1.0.0/pyrca/thirdparty/pgmpy/factors/distributions/base.py`

 * *Files identical despite different names*

### Comparing `sfr-pyrca-0.0.1/pyrca/thirdparty/pgmpy/global_vars.py` & `sfr-pyrca-1.0.0/pyrca/thirdparty/pgmpy/global_vars.py`

 * *Files identical despite different names*

### Comparing `sfr-pyrca-0.0.1/pyrca/thirdparty/pgmpy/independencies/Independencies.py` & `sfr-pyrca-1.0.0/pyrca/thirdparty/pgmpy/independencies/Independencies.py`

 * *Files identical despite different names*

### Comparing `sfr-pyrca-0.0.1/pyrca/thirdparty/pgmpy/inference/EliminationOrder.py` & `sfr-pyrca-1.0.0/pyrca/thirdparty/pgmpy/inference/EliminationOrder.py`

 * *Files identical despite different names*

### Comparing `sfr-pyrca-0.0.1/pyrca/thirdparty/pgmpy/inference/ExactInference.py` & `sfr-pyrca-1.0.0/pyrca/thirdparty/pgmpy/inference/ExactInference.py`

 * *Files identical despite different names*

### Comparing `sfr-pyrca-0.0.1/pyrca/thirdparty/pgmpy/inference/base.py` & `sfr-pyrca-1.0.0/pyrca/thirdparty/pgmpy/inference/base.py`

 * *Files identical despite different names*

### Comparing `sfr-pyrca-0.0.1/pyrca/thirdparty/pgmpy/models/BayesianModel.py` & `sfr-pyrca-1.0.0/pyrca/thirdparty/pgmpy/models/BayesianModel.py`

 * *Files identical despite different names*

### Comparing `sfr-pyrca-0.0.1/pyrca/thirdparty/pgmpy/models/ClusterGraph.py` & `sfr-pyrca-1.0.0/pyrca/thirdparty/pgmpy/models/ClusterGraph.py`

 * *Files identical despite different names*

### Comparing `sfr-pyrca-0.0.1/pyrca/thirdparty/pgmpy/models/DynamicBayesianNetwork.py` & `sfr-pyrca-1.0.0/pyrca/thirdparty/pgmpy/models/DynamicBayesianNetwork.py`

 * *Files identical despite different names*

### Comparing `sfr-pyrca-0.0.1/pyrca/thirdparty/pgmpy/models/FactorGraph.py` & `sfr-pyrca-1.0.0/pyrca/thirdparty/pgmpy/models/FactorGraph.py`

 * *Files identical despite different names*

### Comparing `sfr-pyrca-0.0.1/pyrca/thirdparty/pgmpy/models/JunctionTree.py` & `sfr-pyrca-1.0.0/pyrca/thirdparty/pgmpy/models/JunctionTree.py`

 * *Files identical despite different names*

### Comparing `sfr-pyrca-0.0.1/pyrca/thirdparty/pgmpy/models/MarkovModel.py` & `sfr-pyrca-1.0.0/pyrca/thirdparty/pgmpy/models/MarkovModel.py`

 * *Files identical despite different names*

### Comparing `sfr-pyrca-0.0.1/pyrca/thirdparty/pgmpy/readwrite/BIF.py` & `sfr-pyrca-1.0.0/pyrca/thirdparty/pgmpy/readwrite/BIF.py`

 * *Files identical despite different names*

### Comparing `sfr-pyrca-0.0.1/pyrca/thirdparty/pgmpy/utils/state_name.py` & `sfr-pyrca-1.0.0/pyrca/thirdparty/pgmpy/utils/state_name.py`

 * *Files identical despite different names*

### Comparing `sfr-pyrca-0.0.1/pyrca/thirdparty/pycausal/prior.py` & `sfr-pyrca-1.0.0/pyrca/thirdparty/pycausal/prior.py`

 * *Files identical despite different names*

### Comparing `sfr-pyrca-0.0.1/pyrca/thirdparty/pycausal/pycausal.py` & `sfr-pyrca-1.0.0/pyrca/thirdparty/pycausal/pycausal.py`

 * *Files identical despite different names*

### Comparing `sfr-pyrca-0.0.1/pyrca/thirdparty/pycausal/search.py` & `sfr-pyrca-1.0.0/pyrca/thirdparty/pycausal/search.py`

 * *Files identical despite different names*

### Comparing `sfr-pyrca-0.0.1/pyrca/thirdparty/rcd/rcd.py` & `sfr-pyrca-1.0.0/pyrca/thirdparty/rcd/rcd.py`

 * *Files identical despite different names*

### Comparing `sfr-pyrca-0.0.1/pyrca/thirdparty/rcd/utils/GraphClass.py` & `sfr-pyrca-1.0.0/pyrca/thirdparty/rcd/utils/GraphClass.py`

 * *Files identical despite different names*

### Comparing `sfr-pyrca-0.0.1/pyrca/thirdparty/rcd/utils/SkeletonDiscovery.py` & `sfr-pyrca-1.0.0/pyrca/thirdparty/rcd/utils/SkeletonDiscovery.py`

 * *Files identical despite different names*

### Comparing `sfr-pyrca-0.0.1/pyrca/tools/dashboard/assets/Acumin-BdPro.otf` & `sfr-pyrca-1.0.0/pyrca/tools/dashboard/assets/Acumin-BdPro.otf`

 * *Files identical despite different names*

### Comparing `sfr-pyrca-0.0.1/pyrca/tools/dashboard/assets/base.css` & `sfr-pyrca-1.0.0/pyrca/tools/dashboard/assets/base.css`

 * *Files identical despite different names*

### Comparing `sfr-pyrca-0.0.1/pyrca/tools/dashboard/assets/logo.png` & `sfr-pyrca-1.0.0/pyrca/tools/dashboard/assets/logo.png`

 * *Files identical despite different names*

### Comparing `sfr-pyrca-0.0.1/pyrca/tools/dashboard/assets/modal.css` & `sfr-pyrca-1.0.0/pyrca/tools/dashboard/assets/modal.css`

 * *Files identical despite different names*

### Comparing `sfr-pyrca-0.0.1/pyrca/tools/dashboard/assets/rca.css` & `sfr-pyrca-1.0.0/pyrca/tools/dashboard/assets/rca.css`

 * *Files identical despite different names*

### Comparing `sfr-pyrca-0.0.1/pyrca/tools/dashboard/assets/styles.css` & `sfr-pyrca-1.0.0/pyrca/tools/dashboard/assets/styles.css`

 * *Files identical despite different names*

### Comparing `sfr-pyrca-0.0.1/pyrca/tools/dashboard/assets/upload.svg` & `sfr-pyrca-1.0.0/pyrca/tools/dashboard/assets/upload.svg`

 * *Files identical despite different names*

### Comparing `sfr-pyrca-0.0.1/pyrca/tools/dashboard/callbacks/causal.py` & `sfr-pyrca-1.0.0/pyrca/tools/dashboard/callbacks/causal.py`

 * *Files 1% similar despite different names*

```diff
@@ -127,14 +127,15 @@
         State("select-causal-method", "value"),
         State("causal-param-table", "children"),
         State("causal-state", "data"),
         State("causal-data-state", "data"),
         State("cytoscape", "elements"),
         State("root-leaf-table", "children"),
         State("link-table", "children"),
+        State("select-domain", "value"),
     ],
     running=[
         (Output("causal-run-btn", "disabled"), True, False),
         (Output("causal-cancel-btn", "disabled"), False, True),
     ],
     cancel=[Input("causal-cancel-btn", "n_clicks")],
     background=True,
@@ -150,14 +151,15 @@
     algorithm,
     param_table,
     causal_state,
     data_state,
     cyto_elements,
     root_leaf_table,
     link_table,
+    domain_file,
 ):
     ctx = dash.callback_context
     modal_is_open = False
     modal_content = ""
     state = json.loads(causal_state) if causal_state is not None else {}
     data_state = json.loads(data_state) if data_state is not None else {}
 
@@ -183,15 +185,15 @@
 
                 params = causal_method.parse_parameters(
                     param_info=causal_method.get_parameter_info(algorithm),
                     params={p["Parameter"]: p["Value"] for p in param_table["props"]["data"]},
                 )
                 df = causal_method.load_data(filename)
                 constraints = _build_constraints(list(df.columns), root_leaf_table, link_table)
-                graph, graph_df, relations = causal_method.run(df, algorithm, params, constraints)
+                graph, graph_df, relations = causal_method.run(df, algorithm, params, constraints, domain_file)
 
                 output_dir = os.path.join(file_manager.model_directory, filename.split(".")[0])
                 _dump_results(output_dir, graph_df, root_leaf_table, link_table)
                 _update_states(graph, graph_df, relations)
 
             elif upload_graph_file is not None and upload_graph_content is not None:
                 filename = None
```

### Comparing `sfr-pyrca-0.0.1/pyrca/tools/dashboard/callbacks/data.py` & `sfr-pyrca-1.0.0/pyrca/tools/dashboard/callbacks/data.py`

 * *Files identical despite different names*

### Comparing `sfr-pyrca-0.0.1/pyrca/tools/dashboard/dashboard.py` & `sfr-pyrca-1.0.0/pyrca/tools/dashboard/dashboard.py`

 * *Files identical despite different names*

### Comparing `sfr-pyrca-0.0.1/pyrca/tools/dashboard/models/causal.py` & `sfr-pyrca-1.0.0/pyrca/tools/dashboard/models/causal.py`

 * *Files 2% similar despite different names*

```diff
@@ -133,18 +133,24 @@
                         relations[(i, j)] = "-->"
                     else:
                         if (j, i) not in relations:
                             relations[(i, j)] = "---"
         relations = {f"{names[i]}<split>{names[j]}": v for (i, j), v in relations.items()}
         return relations
 
-    def run(self, df, algorithm, params, constraints=None):
+    def run(self, df, algorithm, params, constraints=None, domain_file=None):
         if constraints is None:
             constraints = {}
         df = df.dropna()
+        if domain_file:
+            domain = DomainParser(os.path.join(self.folder, domain_file))
+            metrics = domain.get_metrics()
+            if metrics is not None:
+                df = df[metrics]
+
         method_class = self.get_supported_methods()[algorithm]["class"]
         config_class = self.get_supported_methods()[algorithm]["config_class"]
         method = method_class(config_class.from_dict(params))
         graph_df = method.train(
             df=df, forbids=constraints.get("forbidden", []), requires=constraints.get("required", [])
         )
         relations = self._extract_relations(graph_df)
```

### Comparing `sfr-pyrca-0.0.1/pyrca/tools/dashboard/models/data.py` & `sfr-pyrca-1.0.0/pyrca/tools/dashboard/models/data.py`

 * *Files identical despite different names*

### Comparing `sfr-pyrca-0.0.1/pyrca/tools/dashboard/pages/causal.py` & `sfr-pyrca-1.0.0/pyrca/tools/dashboard/pages/causal.py`

 * *Files identical despite different names*

### Comparing `sfr-pyrca-0.0.1/pyrca/tools/dashboard/pages/data.py` & `sfr-pyrca-1.0.0/pyrca/tools/dashboard/pages/data.py`

 * *Files identical despite different names*

### Comparing `sfr-pyrca-0.0.1/pyrca/tools/dashboard/pages/utils.py` & `sfr-pyrca-1.0.0/pyrca/tools/dashboard/pages/utils.py`

 * *Files identical despite different names*

### Comparing `sfr-pyrca-0.0.1/pyrca/tools/dashboard/utils/file_manager.py` & `sfr-pyrca-1.0.0/pyrca/tools/dashboard/utils/file_manager.py`

 * *Files identical despite different names*

### Comparing `sfr-pyrca-0.0.1/pyrca/tools/dashboard/utils/layout.py` & `sfr-pyrca-1.0.0/pyrca/tools/dashboard/utils/layout.py`

 * *Files identical despite different names*

### Comparing `sfr-pyrca-0.0.1/pyrca/tools/dashboard/utils/log.py` & `sfr-pyrca-1.0.0/pyrca/tools/dashboard/utils/log.py`

 * *Files identical despite different names*

### Comparing `sfr-pyrca-0.0.1/pyrca/tools/dashboard/utils/plot.py` & `sfr-pyrca-1.0.0/pyrca/tools/dashboard/utils/plot.py`

 * *Files identical despite different names*

### Comparing `sfr-pyrca-0.0.1/pyrca/utils/misc.py` & `sfr-pyrca-1.0.0/pyrca/utils/misc.py`

 * *Files identical despite different names*

### Comparing `sfr-pyrca-0.0.1/pyrca/utils/plot.py` & `sfr-pyrca-1.0.0/pyrca/utils/plot.py`

 * *Files identical despite different names*

### Comparing `sfr-pyrca-0.0.1/pyrca/utils/utils.py` & `sfr-pyrca-1.0.0/pyrca/utils/utils.py`

 * *Files identical despite different names*

### Comparing `sfr-pyrca-0.0.1/setup.py` & `sfr-pyrca-1.0.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 extras_require = {
     "plot": ["plotly>=4", "dash>=2.0", "dash_bootstrap_components>=1.0", "jupyter-dash>=0.4", "dash[diskcache]"]
 }
 extras_require["all"] = sum(extras_require.values(), [])
 
 setup(
     name="sfr-pyrca",
-    version="0.0.1",
+    version="1.0.0",
     author="Salesforce Research Warden AIOps",
     description="PyRCA: A Python library for Root Cause Analysis",
     long_description=open("README.md", "r", encoding="utf-8").read(),
     long_description_content_type="text/markdown",
     keywords="AIOps RCA root cause analysis",
     url="https://github.com/salesforce/PyRCA",
     license="3-Clause BSD",
```

### Comparing `sfr-pyrca-0.0.1/sfr_pyrca.egg-info/PKG-INFO` & `sfr-pyrca-1.0.0/sfr_pyrca.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sfr-pyrca
-Version: 0.0.1
+Version: 1.0.0
 Summary: PyRCA: A Python library for Root Cause Analysis
 Home-page: https://github.com/salesforce/PyRCA
 Author: Salesforce Research Warden AIOps
 License: 3-Clause BSD
 Keywords: AIOps RCA root cause analysis
 Requires-Python: >=3.7,<4
 Description-Content-Type: text/markdown
@@ -39,38 +39,40 @@
 5. [Tutorial](https://github.com/salesforce/PyRCA/tree/main/examples)
 6. [Example](#application-example)
 7. [Benchmarks](#benchmarks)
 8. [How to Contribute](#how-to-contribute)
 
 ## Introduction
 
-With the rapidly growing adoption of microservices architectures, multi-service applications become the standard 
-paradigm in real-world IT applications. A multi-service application usually contains hundreds of interacting 
-services, making it harder to detect service failures and identify the root causes. Root cause analysis (RCA) 
-methods usually leverage the KPI metrics, traces or logs monitored on those services to determine the root causes 
-when a system failure is detected, helping engineers and SREs in the troubleshooting process.
-
-PyRCA is a Python machine-learning library designed for root cause analysis, offering multiple state-of-the-art RCA
-algorithms and an end-to-end pipeline for building RCA solutions. Currently, PyRCA mainly focuses on metric-based RCA 
-including two types of algorithms: 1. Identifying anomalous metrics in parallel with the observed anomaly via 
-metric data analysis, e.g., ε-diagnosis, and 2. Identifying root causes based a topology/causal graph representing 
-the causal relationships between the observed metrics, e.g., Bayesian inference, Random Walk. Besides, PyRCA 
-provides a convenient tool for building causal graphs from the observed time series data and domain knowledge, 
-helping users to develop graph-based solutions quickly. PyRCA also provides a benchmark for evaluating 
-various RCA methods, which is valuable for industry and academic research.
+The adoption of microservices architectures is growing at a rapid pace, making multi-service applications 
+the standard paradigm in real-world IT applications. Typically, a multi-service application consists of 
+hundreds of interacting services, making it increasingly challenging to detect service failures and identify 
+their root causes. Root cause analysis (RCA) methods typically rely on KPI metrics, traces, or logs monitored 
+on these services to determine the root causes when a system failure is detected. Such methods can aid 
+engineers and SREs in the troubleshooting process.
+
+PyRCA is a Python machine-learning library designed to facilitate root cause analysis by offering various 
+state-of-the-art RCA algorithms and an end-to-end pipeline for building RCA solutions. At present, PyRCA 
+primarily focuses on metric-based RCA, including two types of algorithms: (1) identifying anomalous metrics 
+in parallel with the observed anomaly through metric data analysis, such as ε-diagnosis, and (2) identifying 
+root causes based on a topology/causal graph representing the causal relationships between the observed 
+metrics, such as Bayesian inference and Random Walk. PyRCA also provides a convenient tool for building 
+causal graphs from the observed time series data and domain knowledge, enabling users to develop graph-based 
+solutions quickly. Furthermore, PyRCA offers a benchmark for evaluating various RCA methods, which is 
+valuable for industry and academic research.
 
 The following list shows the supported RCA methods in our library:
-1. ε-Diagnosis
+1. [ε-Diagnosis](https://dl.acm.org/doi/10.1145/3308558.3313653)
 2. Bayesian Inference-based RCA (BI)
 3. Random Walk-based RCA (RW)
-4. Root Casue Discovery method (RCD)
-5. Hypothesis Testing-based RCA (HT)
+4. [Root Casue Discovery method (RCD)](https://openreview.net/pdf?id=weoLjoYFvXY)
+5. [Hypothesis Testing-based RCA (HT)](https://dl.acm.org/doi/10.1145/3534678.3539041)
 
 We will continue improving this library to make it more comprehensive in the future. In the future, 
-PyRCA will support trace and log based RCA methods as well.
+PyRCA will support trace and log-based RCA methods as well.
 
 ## Installation
 
 You can install ``pyrca`` from PyPI by calling ``pip install sfr-pyrca``. You may install from source by
 cloning the PyRCA repo, navigating to the root directory, and calling
 ``pip install .``, or ``pip install -e .`` to install in editable mode. You may install additional dependencies:
 
@@ -80,36 +82,38 @@
   root directory of the repo.
 
 ## Getting Started
 
 PyRCA provides a unified interface for training RCA models and finding root causes. To apply
 a certain RCA method, you only need to specify: 
 
-- **The select RCA method**: e.g., ``BayesianNetwork``, ``EpsilonDiagnosis``.
-- **The RCA configuration**: e.g., ``BayesianNetworkConfig``, ``EpsilonDiagnosisConfig``.
-- **Time series data for initialization or training**: e.g., A time series data in a 
+- **The selected RCA method**: e.g., ``BayesianNetwork``, ``EpsilonDiagnosis``.
+- **The method configuration**: e.g., ``BayesianNetworkConfig``, ``EpsilonDiagnosisConfig``.
+- **Time series data for initialization/training**: e.g., A time series data in a 
   pandas dataframe.
-- **Some detected anomalous KPI metrics**: Some RCA methods require the anomalous KPI metrics detected by
-  certain anomaly detector.
+- **Abnormal time series data in an incident window**: The RCA methods require the anomalous 
+  KPI metrics in an incident window.
 
-Let's take ``BayesianNetwork`` as an example. Suppose that ``graph_df`` is a pandas dataframe of
-the graph representing causal relationships between metrics (how to construct such causal graph
-will be discussed later), and ``df`` is a pandas dataframe containing the historical observed time series 
+Let's take ``BayesianNetwork`` as an example. Suppose that ``graph_df`` is the pandas dataframe of
+a graph representing the causal relationships between metrics (how to construct such causal graph
+will be discussed later), and ``df`` is the pandas dataframe containing the historical observed time series 
 data (e.g., the index is the timestamp and each column represents one monitored metric). To train a 
 ``BayesianNetwork``, you can simply run the following code:
 
 ```python
 from pyrca.analyzers.bayesian import BayesianNetwork
 model = BayesianNetwork(config=BayesianNetwork.config_class(graph=graph_df))
 model.train(df)
 model.save("model_folder")
 ```
 
 After the model is trained, you can use it to find root causes of an incident given a list of anomalous
-metrics detected by a certain anomaly detector, e.g.,
+metrics detected by a certain anomaly detector (you can use the stats-based detector supported in PyRCA
+or other anomaly detection methods supported by our [Merlion](https://github.com/salesforce/Merlion) library), 
+e.g.,
 
 ```python
 from pyrca.analyzers.bayesian import BayesianNetwork
 model = BayesianNetwork.load("model_folder")
 results = model.find_root_causes(["observed_anomalous_metric", ...])
 print(results.to_dict())
 ```
@@ -134,24 +138,24 @@
 where ``abnormal_data`` is the time series data collected in an incident window.
 
 As mentioned above, some RCA methods such as ``BayesianNetwork`` require causal graphs as their inputs. To construct such causal
 graphs from the observed time series data, you can utilize our tool by running ``python -m pyrca.tools``.
 This command will launch a Dash app for time series data analysis and causal discovery.
 ![alt text](https://github.com/salesforce/PyRCA/raw/main/docs/_static/dashboard.png)
 
-The dashboard allows you to try different causal discovery methods, adjust causal discovery parameters,
-add domain knowledge constraints (e.g., root/leaf nodes, forbidden/required links), and visualize
-the generated causal graphs. It makes easier for manually revising causal graphs based on domain knowledge.
-You can download the graph generated by this tool if you satisfy with it. The graph can be used by the RCA 
-methods supported in PyRCA.
-
-Instead of using this dashboard, you can also write code for building such graphs. The package 
-``pyrca.graphs.causal`` includes several popular causal discovery methods you can use. All of these methods
-support domain knowledge constraints. Suppose ``df`` is the observed time series data
-and you want to apply the PC algorithm for building causal graphs, then the following code will help:
+The dashboard enables users to experiment with different causal discovery methods, customize causal discovery 
+parameters, add domain knowledge constraints (e.g., root/leaf nodes, forbidden/required links), and visualize 
+the generated causal graphs. This feature simplifies the process of manually revising causal graphs based on 
+domain knowledge. Users can download the graph generated by this tool if they are satisfied with it. The graph 
+can then be used by the RCA methods supported in PyRCA.
+
+Alternatively, users can write code to build such graphs instead of using the dashboard. The package 
+``pyrca.graphs.causal`` includes several popular causal discovery methods that users can leverage. 
+All of these methods support domain knowledge constraints. For instance, if users wish to apply the PC 
+algorithm for building causal graphs on the observed time series data ``df``, the following code can be used:
 
 ```python
 from pyrca.graphs.causal.pc import PC
 model = PC(PC.config_class())
 graph_df = model.train(df)
 ```
 
@@ -188,15 +192,15 @@
 
 [Here](https://github.com/salesforce/PyRCA/tree/main/pyrca/applications/example) is a real-world example
 of applying ``BayesianNetwork`` to build a solution for RCA, which is adapted from our internal use cases. 
 The "config" folder includes the settings for the stats-based anomaly detector and the domain knowledge. 
 The "models" folder stores the causal graph and the trained Bayesian network. The ``RCAEngine`` class in the "rca.py" 
 file implements the methods for building causal graphs, training Bayesian networks and finding root causes 
 by utilizing the modules provided by PyRCA. You can directly use this class if the stats-based anomaly detector 
-and Bayesian inference are suitable for your RCA problems. For example, given a time series dataframe ``df``, 
+and Bayesian inference are suitable for your problems. For example, given a time series dataframe ``df``, 
 you can build and train a Bayesian network via the following code:
 
 ```python
 from pyrca.applications.example.rca import RCAEngine
 engine = RCAEngine()
 engine.build_causal_graph(
     df=df,
```

#### html2text {}

```diff
@@ -1,100 +1,106 @@
-Metadata-Version: 2.1 Name: sfr-pyrca Version: 0.0.1 Summary: PyRCA: A Python
+Metadata-Version: 2.1 Name: sfr-pyrca Version: 1.0.0 Summary: PyRCA: A Python
 library for Root Cause Analysis Home-page: https://github.com/salesforce/PyRCA
 Author: Salesforce Research Warden AIOps License: 3-Clause BSD Keywords: AIOps
 RCA root cause analysis Requires-Python: >=3.7,<4 Description-Content-Type:
 text/markdown Provides-Extra: plot Provides-Extra: all License-File: LICENSE #
 PyRCA: A Python library for Root Cause Analysis
 [https://img.shields.io/badge/Python-3.7,_3.8,_3.9-blue] [PyPI] [Documentation]
                                [Downloads] [DOI]
 ## Table of Contents 1. [Introduction](#introduction) 2. [Installation]
 (#installation) 3. [Getting Started](#getting-started) 4. [Documentation]
 (https://fuzzy-disco-r42n6p1.pages.github.io/) 5. [Tutorial](https://
 github.com/salesforce/PyRCA/tree/main/examples) 6. [Example](#application-
 example) 7. [Benchmarks](#benchmarks) 8. [How to Contribute](#how-to-
-contribute) ## Introduction With the rapidly growing adoption of microservices
-architectures, multi-service applications become the standard paradigm in real-
-world IT applications. A multi-service application usually contains hundreds of
-interacting services, making it harder to detect service failures and identify
-the root causes. Root cause analysis (RCA) methods usually leverage the KPI
-metrics, traces or logs monitored on those services to determine the root
-causes when a system failure is detected, helping engineers and SREs in the
-troubleshooting process. PyRCA is a Python machine-learning library designed
-for root cause analysis, offering multiple state-of-the-art RCA algorithms and
-an end-to-end pipeline for building RCA solutions. Currently, PyRCA mainly
-focuses on metric-based RCA including two types of algorithms: 1. Identifying
-anomalous metrics in parallel with the observed anomaly via metric data
-analysis, e.g., Îµ-diagnosis, and 2. Identifying root causes based a topology/
-causal graph representing the causal relationships between the observed
-metrics, e.g., Bayesian inference, Random Walk. Besides, PyRCA provides a
-convenient tool for building causal graphs from the observed time series data
-and domain knowledge, helping users to develop graph-based solutions quickly.
-PyRCA also provides a benchmark for evaluating various RCA methods, which is
-valuable for industry and academic research. The following list shows the
-supported RCA methods in our library: 1. Îµ-Diagnosis 2. Bayesian Inference-
-based RCA (BI) 3. Random Walk-based RCA (RW) 4. Root Casue Discovery method
-(RCD) 5. Hypothesis Testing-based RCA (HT) We will continue improving this
-library to make it more comprehensive in the future. In the future, PyRCA will
-support trace and log based RCA methods as well. ## Installation You can
-install ``pyrca`` from PyPI by calling ``pip install sfr-pyrca``. You may
-install from source by cloning the PyRCA repo, navigating to the root
-directory, and calling ``pip install .``, or ``pip install -e .`` to install in
-editable mode. You may install additional dependencies: - **For plotting &
-visualization**: Calling ``pip install sfr-pyrca[plot]``, or ``pip install .
-[plot]`` from the root directory of the repo. - **Install all the
+contribute) ## Introduction The adoption of microservices architectures is
+growing at a rapid pace, making multi-service applications the standard
+paradigm in real-world IT applications. Typically, a multi-service application
+consists of hundreds of interacting services, making it increasingly
+challenging to detect service failures and identify their root causes. Root
+cause analysis (RCA) methods typically rely on KPI metrics, traces, or logs
+monitored on these services to determine the root causes when a system failure
+is detected. Such methods can aid engineers and SREs in the troubleshooting
+process. PyRCA is a Python machine-learning library designed to facilitate root
+cause analysis by offering various state-of-the-art RCA algorithms and an end-
+to-end pipeline for building RCA solutions. At present, PyRCA primarily focuses
+on metric-based RCA, including two types of algorithms: (1) identifying
+anomalous metrics in parallel with the observed anomaly through metric data
+analysis, such as Îµ-diagnosis, and (2) identifying root causes based on a
+topology/causal graph representing the causal relationships between the
+observed metrics, such as Bayesian inference and Random Walk. PyRCA also
+provides a convenient tool for building causal graphs from the observed time
+series data and domain knowledge, enabling users to develop graph-based
+solutions quickly. Furthermore, PyRCA offers a benchmark for evaluating various
+RCA methods, which is valuable for industry and academic research. The
+following list shows the supported RCA methods in our library: 1. [Îµ-
+Diagnosis](https://dl.acm.org/doi/10.1145/3308558.3313653) 2. Bayesian
+Inference-based RCA (BI) 3. Random Walk-based RCA (RW) 4. [Root Casue Discovery
+method (RCD)](https://openreview.net/pdf?id=weoLjoYFvXY) 5. [Hypothesis
+Testing-based RCA (HT)](https://dl.acm.org/doi/10.1145/3534678.3539041) We will
+continue improving this library to make it more comprehensive in the future. In
+the future, PyRCA will support trace and log-based RCA methods as well. ##
+Installation You can install ``pyrca`` from PyPI by calling ``pip install sfr-
+pyrca``. You may install from source by cloning the PyRCA repo, navigating to
+the root directory, and calling ``pip install .``, or ``pip install -e .`` to
+install in editable mode. You may install additional dependencies: - **For
+plotting & visualization**: Calling ``pip install sfr-pyrca[plot]``, or ``pip
+install .[plot]`` from the root directory of the repo. - **Install all the
 dependencies**: Calling ``pip install sfr-pyrca[all]``, or ``pip install .
 [all]`` from the root directory of the repo. ## Getting Started PyRCA provides
 a unified interface for training RCA models and finding root causes. To apply a
-certain RCA method, you only need to specify: - **The select RCA method**:
-e.g., ``BayesianNetwork``, ``EpsilonDiagnosis``. - **The RCA configuration**:
-e.g., ``BayesianNetworkConfig``, ``EpsilonDiagnosisConfig``. - **Time series
-data for initialization or training**: e.g., A time series data in a pandas
-dataframe. - **Some detected anomalous KPI metrics**: Some RCA methods require
-the anomalous KPI metrics detected by certain anomaly detector. Let's take
-``BayesianNetwork`` as an example. Suppose that ``graph_df`` is a pandas
-dataframe of the graph representing causal relationships between metrics (how
-to construct such causal graph will be discussed later), and ``df`` is a pandas
-dataframe containing the historical observed time series data (e.g., the index
-is the timestamp and each column represents one monitored metric). To train a
-``BayesianNetwork``, you can simply run the following code: ```python from
-pyrca.analyzers.bayesian import BayesianNetwork model = BayesianNetwork
+certain RCA method, you only need to specify: - **The selected RCA method**:
+e.g., ``BayesianNetwork``, ``EpsilonDiagnosis``. - **The method
+configuration**: e.g., ``BayesianNetworkConfig``, ``EpsilonDiagnosisConfig``. -
+**Time series data for initialization/training**: e.g., A time series data in a
+pandas dataframe. - **Abnormal time series data in an incident window**: The
+RCA methods require the anomalous KPI metrics in an incident window. Let's take
+``BayesianNetwork`` as an example. Suppose that ``graph_df`` is the pandas
+dataframe of a graph representing the causal relationships between metrics (how
+to construct such causal graph will be discussed later), and ``df`` is the
+pandas dataframe containing the historical observed time series data (e.g., the
+index is the timestamp and each column represents one monitored metric). To
+train a ``BayesianNetwork``, you can simply run the following code: ```python
+from pyrca.analyzers.bayesian import BayesianNetwork model = BayesianNetwork
 (config=BayesianNetwork.config_class(graph=graph_df)) model.train(df)
 model.save("model_folder") ``` After the model is trained, you can use it to
 find root causes of an incident given a list of anomalous metrics detected by a
-certain anomaly detector, e.g., ```python from pyrca.analyzers.bayesian import
-BayesianNetwork model = BayesianNetwork.load("model_folder") results =
-model.find_root_causes(["observed_anomalous_metric", ...]) print
-(results.to_dict()) ``` For other RCA methods, you can write similar code as
-above for finding root causes. For example, if you want to try
+certain anomaly detector (you can use the stats-based detector supported in
+PyRCA or other anomaly detection methods supported by our [Merlion](https://
+github.com/salesforce/Merlion) library), e.g., ```python from
+pyrca.analyzers.bayesian import BayesianNetwork model = BayesianNetwork.load
+("model_folder") results = model.find_root_causes(["observed_anomalous_metric",
+...]) print(results.to_dict()) ``` For other RCA methods, you can write similar
+code as above for finding root causes. For example, if you want to try
 ``EpsilonDiagnosis``, you can initalize ``EpsilonDiagnosis`` as follows:
 ```python from pyrca.analyzers.epsilon_diagnosis import EpsilonDiagnosis model
 = EpsilonDiagnosis(config=EpsilonDiagnosis.config_class(alpha=0.01))
 model.train(normal_data) ``` Here ``normal_data`` is the historically observed
 time series data without anomalies. To identify root causes, you can run:
 ```python results = model.find_root_causes(abnormal_data) print(results.to_dict
 ()) ``` where ``abnormal_data`` is the time series data collected in an
 incident window. As mentioned above, some RCA methods such as
 ``BayesianNetwork`` require causal graphs as their inputs. To construct such
 causal graphs from the observed time series data, you can utilize our tool by
 running ``python -m pyrca.tools``. This command will launch a Dash app for time
 series data analysis and causal discovery. ![alt text](https://github.com/
-salesforce/PyRCA/raw/main/docs/_static/dashboard.png) The dashboard allows you
-to try different causal discovery methods, adjust causal discovery parameters,
-add domain knowledge constraints (e.g., root/leaf nodes, forbidden/required
-links), and visualize the generated causal graphs. It makes easier for manually
-revising causal graphs based on domain knowledge. You can download the graph
-generated by this tool if you satisfy with it. The graph can be used by the RCA
-methods supported in PyRCA. Instead of using this dashboard, you can also write
-code for building such graphs. The package ``pyrca.graphs.causal`` includes
-several popular causal discovery methods you can use. All of these methods
-support domain knowledge constraints. Suppose ``df`` is the observed time
-series data and you want to apply the PC algorithm for building causal graphs,
-then the following code will help: ```python from pyrca.graphs.causal.pc import
-PC model = PC(PC.config_class()) graph_df = model.train(df) ``` If you have
-some domain knowledge constraints, you may run: ```python from
+salesforce/PyRCA/raw/main/docs/_static/dashboard.png) The dashboard enables
+users to experiment with different causal discovery methods, customize causal
+discovery parameters, add domain knowledge constraints (e.g., root/leaf nodes,
+forbidden/required links), and visualize the generated causal graphs. This
+feature simplifies the process of manually revising causal graphs based on
+domain knowledge. Users can download the graph generated by this tool if they
+are satisfied with it. The graph can then be used by the RCA methods supported
+in PyRCA. Alternatively, users can write code to build such graphs instead of
+using the dashboard. The package ``pyrca.graphs.causal`` includes several
+popular causal discovery methods that users can leverage. All of these methods
+support domain knowledge constraints. For instance, if users wish to apply the
+PC algorithm for building causal graphs on the observed time series data
+``df``, the following code can be used: ```python from pyrca.graphs.causal.pc
+import PC model = PC(PC.config_class()) graph_df = model.train(df) ``` If you
+have some domain knowledge constraints, you may run: ```python from
 pyrca.graphs.causal.pc import PC model = PC(PC.config_class
 (domain_knowledge_file="file_path")) graph_df = model.train(df) ``` The domain
 knowledge file has a YAML format, e.g., ```yaml causal-graph: root-nodes: ["A",
 "B"] leaf-nodes: ["E", "F"] forbids: - ["A", "E"] requires: - ["A", "C"] ```
 This domain knowledge file states that: 1. Metrics A and B must the root nodes,
 2. Metrics E and F must be the leaf nodes, 3. There is no connection from A to
 E, and 4. There is a connection from A to C. You can write your domain
@@ -104,32 +110,31 @@
 ``BayesianNetwork`` to build a solution for RCA, which is adapted from our
 internal use cases. The "config" folder includes the settings for the stats-
 based anomaly detector and the domain knowledge. The "models" folder stores the
 causal graph and the trained Bayesian network. The ``RCAEngine`` class in the
 "rca.py" file implements the methods for building causal graphs, training
 Bayesian networks and finding root causes by utilizing the modules provided by
 PyRCA. You can directly use this class if the stats-based anomaly detector and
-Bayesian inference are suitable for your RCA problems. For example, given a
-time series dataframe ``df``, you can build and train a Bayesian network via
-the following code: ```python from pyrca.applications.example.rca import
-RCAEngine engine = RCAEngine() engine.build_causal_graph( df=df,
-run_pdag2dag=True, max_num_points=5000000, verbose=True ) bn =
-engine.train_bayesian_network(dfs=[df]) bn.print_probabilities() ``` After the
-Bayesian network is constructed, you can use it directly for finding root
-causes: ```python engine = RCAEngine() result = engine.find_root_causes_bn
-(anomalies=["conn_pool", "apt"]) pprint.pprint(result) ``` The inputs of
-``find_root_causes_bn`` is a list of the anomalous metrics detected by the
-stats-based anomaly detector. This method will estimate the probability of a
-node being a root cause and extract the paths from a potential root cause node
-to the leaf nodes. ## Benchmarks The following table summarizes the RCA
-performance of different methods on the simulated dataset. How to generate the
-simulated dataset can be found [here](https://github.com/salesforce/PyRCA/blob/
-main/examples/DataGeneration.ipynb), and how to test different RCA methods can
-be found [here](https://github.com/salesforce/PyRCA/blob/main/examples/
-Root%20Cause%20Analysis.ipynb).
+Bayesian inference are suitable for your problems. For example, given a time
+series dataframe ``df``, you can build and train a Bayesian network via the
+following code: ```python from pyrca.applications.example.rca import RCAEngine
+engine = RCAEngine() engine.build_causal_graph( df=df, run_pdag2dag=True,
+max_num_points=5000000, verbose=True ) bn = engine.train_bayesian_network(dfs=
+[df]) bn.print_probabilities() ``` After the Bayesian network is constructed,
+you can use it directly for finding root causes: ```python engine = RCAEngine()
+result = engine.find_root_causes_bn(anomalies=["conn_pool", "apt"])
+pprint.pprint(result) ``` The inputs of ``find_root_causes_bn`` is a list of
+the anomalous metrics detected by the stats-based anomaly detector. This method
+will estimate the probability of a node being a root cause and extract the
+paths from a potential root cause node to the leaf nodes. ## Benchmarks The
+following table summarizes the RCA performance of different methods on the
+simulated dataset. How to generate the simulated dataset can be found [here]
+(https://github.com/salesforce/PyRCA/blob/main/examples/DataGeneration.ipynb),
+and how to test different RCA methods can be found [here](https://github.com/
+salesforce/PyRCA/blob/main/examples/Root%20Cause%20Analysis.ipynb).
 | | Recall@1 | Recall@3 | Recall@5 | :---------------------------:|:----------
  -:|:-----------:|:-----------: | Îµ-Diagnosis | 0.06 Â± 0.02 | 0.16 Â± 0.04 |
 0.16 Â± 0.04 | | RCD | 0.28 Â± 0.05 | 0.29 Â± 0.05 | 0.30 Â± 0.05 | | Local-RCD
  | 0.44 Â± 0.05 | 0.70 Â± 0.05 | 0.70 Â± 0.05 | | Random Walk | 0.07 Â± 0.03 |
 0.20 Â± 0.04 | 0.24 Â± 0.04 | | Random Walk (PC) | 0.06 Â± 0.02 | 0.17 Â± 0.04
  | 0.21 Â± 0.04 | | Bayesian Inference | 0.15 Â± 0.04 | 0.35 Â± 0.05 | 0.43 Â±
 0.05 | | Bayesian Inference (PC) | 0.11 Â± 0.03 | 0.30 Â± 0.05 | 0.40 Â± 0.05 |
```

### Comparing `sfr-pyrca-0.0.1/sfr_pyrca.egg-info/SOURCES.txt` & `sfr-pyrca-1.0.0/sfr_pyrca.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -133,14 +133,15 @@
 pyrca/tools/dashboard/utils/__init__.py
 pyrca/tools/dashboard/utils/file_manager.py
 pyrca/tools/dashboard/utils/layout.py
 pyrca/tools/dashboard/utils/log.py
 pyrca/tools/dashboard/utils/plot.py
 pyrca/utils/__init__.py
 pyrca/utils/domain.py
+pyrca/utils/evaluation.py
 pyrca/utils/logger.py
 pyrca/utils/misc.py
 pyrca/utils/plot.py
 pyrca/utils/utils.py
 sfr_pyrca.egg-info/PKG-INFO
 sfr_pyrca.egg-info/SOURCES.txt
 sfr_pyrca.egg-info/dependency_links.txt
```

### Comparing `sfr-pyrca-0.0.1/tests/analyzers/test_bayesian.py` & `sfr-pyrca-1.0.0/tests/analyzers/test_bayesian.py`

 * *Files identical despite different names*

### Comparing `sfr-pyrca-0.0.1/tests/analyzers/test_epsilon_diagnosis.py` & `sfr-pyrca-1.0.0/tests/analyzers/test_epsilon_diagnosis.py`

 * *Files identical despite different names*

### Comparing `sfr-pyrca-0.0.1/tests/analyzers/test_ht.py` & `sfr-pyrca-1.0.0/tests/analyzers/test_ht.py`

 * *Files identical despite different names*

### Comparing `sfr-pyrca-0.0.1/tests/analyzers/test_random_walk.py` & `sfr-pyrca-1.0.0/tests/analyzers/test_random_walk.py`

 * *Files identical despite different names*

### Comparing `sfr-pyrca-0.0.1/tests/analyzers/test_rcd.py` & `sfr-pyrca-1.0.0/tests/analyzers/test_rcd.py`

 * *Files identical despite different names*

### Comparing `sfr-pyrca-0.0.1/tests/applications/example/run_rca.py` & `sfr-pyrca-1.0.0/tests/applications/example/run_rca.py`

 * *Files identical despite different names*

### Comparing `sfr-pyrca-0.0.1/tests/graphs/test_domain.py` & `sfr-pyrca-1.0.0/tests/graphs/test_domain.py`

 * *Files identical despite different names*

### Comparing `sfr-pyrca-0.0.1/tests/graphs/test_fges.py` & `sfr-pyrca-1.0.0/tests/graphs/test_fges.py`

 * *Files identical despite different names*

### Comparing `sfr-pyrca-0.0.1/tests/graphs/test_ges.py` & `sfr-pyrca-1.0.0/tests/graphs/test_ges.py`

 * *Files identical despite different names*

### Comparing `sfr-pyrca-0.0.1/tests/graphs/test_lingam.py` & `sfr-pyrca-1.0.0/tests/graphs/test_lingam.py`

 * *Files identical despite different names*

### Comparing `sfr-pyrca-0.0.1/tests/graphs/test_pc.py` & `sfr-pyrca-1.0.0/tests/graphs/test_pc.py`

 * *Files identical despite different names*

### Comparing `sfr-pyrca-0.0.1/tests/outliers/test_config.py` & `sfr-pyrca-1.0.0/tests/outliers/test_config.py`

 * *Files identical despite different names*

### Comparing `sfr-pyrca-0.0.1/tests/outliers/test_stats.py` & `sfr-pyrca-1.0.0/tests/outliers/test_stats.py`

 * *Files identical despite different names*

### Comparing `sfr-pyrca-0.0.1/tests/simulation/test_simulation.py` & `sfr-pyrca-1.0.0/tests/simulation/test_simulation.py`

 * *Files identical despite different names*

### Comparing `sfr-pyrca-0.0.1/tests/tools/test_causal.py` & `sfr-pyrca-1.0.0/tests/tools/test_causal.py`

 * *Files identical despite different names*

