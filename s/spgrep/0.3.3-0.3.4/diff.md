# Comparing `tmp/spgrep-0.3.3.tar.gz` & `tmp/spgrep-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spgrep-0.3.3.tar", last modified: Wed Jan 11 07:03:08 2023, max compression
+gzip compressed data, was "spgrep-0.3.4.tar", last modified: Wed May 17 22:09:22 2023, max compression
```

## Comparing `spgrep-0.3.3.tar` & `spgrep-0.3.4.tar`

### file list

```diff
@@ -1,101 +1,101 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 07:03:08.295253 spgrep-0.3.3/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 07:03:08.287253 spgrep-0.3.3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 07:03:08.287253 spgrep-0.3.3/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      487 2023-01-11 07:03:01.000000 spgrep-0.3.3/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (123)      631 2023-01-11 07:03:01.000000 spgrep-0.3.3/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0 runner    (1001) docker     (123)      206 2023-01-11 07:03:01.000000 spgrep-0.3.3/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 07:03:08.287253 spgrep-0.3.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2051 2023-01-11 07:03:01.000000 spgrep-0.3.3/.github/workflows/deploy.yml
--rw-r--r--   0 runner    (1001) docker     (123)      846 2023-01-11 07:03:01.000000 spgrep-0.3.3/.github/workflows/draft-pdf.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2021 2023-01-11 07:03:01.000000 spgrep-0.3.3/.github/workflows/testing.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1927 2023-01-11 07:03:01.000000 spgrep-0.3.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-01-11 07:03:01.000000 spgrep-0.3.3/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-01-11 07:03:01.000000 spgrep-0.3.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4751 2023-01-11 07:03:08.295253 spgrep-0.3.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3858 2023-01-11 07:03:01.000000 spgrep-0.3.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 07:03:08.287253 spgrep-0.3.3/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 07:03:08.287253 spgrep-0.3.3/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-11 07:03:01.000000 spgrep-0.3.3/docs/_static/.gitkeep
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 07:03:08.287253 spgrep-0.3.3/docs/api/
--rw-r--r--   0 runner    (1001) docker     (123)      339 2023-01-11 07:03:01.000000 spgrep-0.3.3/docs/api/api.md
--rw-r--r--   0 runner    (1001) docker     (123)     3855 2023-01-11 07:03:01.000000 spgrep-0.3.3/docs/api/api_core.md
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-01-11 07:03:01.000000 spgrep-0.3.3/docs/api/api_corep.md
--rw-r--r--   0 runner    (1001) docker     (123)      687 2023-01-11 07:03:01.000000 spgrep-0.3.3/docs/api/api_group.md
--rw-r--r--   0 runner    (1001) docker     (123)      621 2023-01-11 07:03:01.000000 spgrep-0.3.3/docs/api/api_irreps.md
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-01-11 07:03:01.000000 spgrep-0.3.3/docs/api/api_pointgroup.md
--rw-r--r--   0 runner    (1001) docker     (123)      865 2023-01-11 07:03:01.000000 spgrep-0.3.3/docs/api/api_representation.md
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-01-11 07:03:01.000000 spgrep-0.3.3/docs/api/api_spinor.md
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-01-11 07:03:01.000000 spgrep-0.3.3/docs/api/api_tensor.md
--rw-r--r--   0 runner    (1001) docker     (123)      199 2023-01-11 07:03:01.000000 spgrep-0.3.3/docs/api/api_transformation.md
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-01-11 07:03:01.000000 spgrep-0.3.3/docs/api/api_utils.md
--rw-r--r--   0 runner    (1001) docker     (123)     1932 2023-01-11 07:03:01.000000 spgrep-0.3.3/docs/changelog.md
--rw-r--r--   0 runner    (1001) docker     (123)     3213 2023-01-11 07:03:01.000000 spgrep-0.3.3/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 07:03:08.287253 spgrep-0.3.3/docs/development/
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-01-11 07:03:01.000000 spgrep-0.3.3/docs/development/development.md
--rw-r--r--   0 runner    (1001) docker     (123)     3566 2023-01-11 07:03:01.000000 spgrep-0.3.3/docs/development/memo.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 07:03:08.291253 spgrep-0.3.3/docs/examples/
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-01-11 07:03:01.000000 spgrep-0.3.3/docs/examples/examples.md
--rw-r--r--   0 runner    (1001) docker     (123)    20920 2023-01-11 07:03:01.000000 spgrep-0.3.3/docs/examples/lattice_vibration.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     3368 2023-01-11 07:03:01.000000 spgrep-0.3.3/docs/examples/phonopy_mp-2998.yaml.xz
--rw-r--r--   0 runner    (1001) docker     (123)     5525 2023-01-11 07:03:01.000000 spgrep-0.3.3/docs/examples/spin_representation.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    36342 2023-01-11 07:03:01.000000 spgrep-0.3.3/docs/examples/symmetry_adapted_tensor.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 07:03:08.291253 spgrep-0.3.3/docs/formulation/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 07:03:08.291253 spgrep-0.3.3/docs/formulation/algorithm/
--rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-01-11 07:03:01.000000 spgrep-0.3.3/docs/formulation/algorithm/algorithm.md
--rw-r--r--   0 runner    (1001) docker     (123)     2960 2023-01-11 07:03:01.000000 spgrep-0.3.3/docs/formulation/algorithm/intertwiner.md
--rw-r--r--   0 runner    (1001) docker     (123)     4288 2023-01-11 07:03:01.000000 spgrep-0.3.3/docs/formulation/algorithm/irreps_from_chain.md
--rw-r--r--   0 runner    (1001) docker     (123)     5869 2023-01-11 07:03:01.000000 spgrep-0.3.3/docs/formulation/algorithm/irreps_from_regular.md
--rw-r--r--   0 runner    (1001) docker     (123)      872 2023-01-11 07:03:01.000000 spgrep-0.3.3/docs/formulation/algorithm/point_group_chain.mmd
--rw-r--r--   0 runner    (1001) docker     (123)    42997 2023-01-11 07:03:01.000000 spgrep-0.3.3/docs/formulation/algorithm/point_group_chain.mmd.svg
--rw-r--r--   0 runner    (1001) docker     (123)      505 2023-01-11 07:03:01.000000 spgrep-0.3.3/docs/formulation/formulation.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 07:03:08.291253 spgrep-0.3.3/docs/formulation/irreps/
--rw-r--r--   0 runner    (1001) docker     (123)     6712 2023-01-11 07:03:01.000000 spgrep-0.3.3/docs/formulation/irreps/corep.md
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-01-11 07:03:01.000000 spgrep-0.3.3/docs/formulation/irreps/irreps.md
--rw-r--r--   0 runner    (1001) docker     (123)     9358 2023-01-11 07:03:01.000000 spgrep-0.3.3/docs/formulation/irreps/reality.md
--rw-r--r--   0 runner    (1001) docker     (123)     8879 2023-01-11 07:03:01.000000 spgrep-0.3.3/docs/formulation/irreps/spacegroup_irreps.md
--rw-r--r--   0 runner    (1001) docker     (123)     8812 2023-01-11 07:03:01.000000 spgrep-0.3.3/docs/formulation/irreps/spinor.md
--rw-r--r--   0 runner    (1001) docker     (123)     3480 2023-01-11 07:03:01.000000 spgrep-0.3.3/docs/formulation/projection.md
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-01-11 07:03:01.000000 spgrep-0.3.3/docs/genindex.rst
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-01-11 07:03:01.000000 spgrep-0.3.3/docs/index.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 07:03:08.291253 spgrep-0.3.3/docs/paper/
--rw-r--r--   0 runner    (1001) docker     (123)    11275 2023-01-11 07:03:01.000000 spgrep-0.3.3/docs/paper/paper.bib
--rw-r--r--   0 runner    (1001) docker     (123)     5687 2023-01-11 07:03:01.000000 spgrep-0.3.3/docs/paper/paper.md
--rw-r--r--   0 runner    (1001) docker     (123)     8775 2023-01-11 07:03:01.000000 spgrep-0.3.3/docs/references.bib
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 07:03:08.291253 spgrep-0.3.3/examples/
--rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-01-11 07:03:01.000000 spgrep-0.3.3/examples/basic.py
--rw-r--r--   0 runner    (1001) docker     (123)     3665 2023-01-11 07:03:01.000000 spgrep-0.3.3/examples/lattice_vibration.py
--rw-r--r--   0 runner    (1001) docker     (123)      529 2023-01-11 07:03:01.000000 spgrep-0.3.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-01-11 07:03:08.295253 spgrep-0.3.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2646 2023-01-11 07:03:01.000000 spgrep-0.3.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 07:03:08.283253 spgrep-0.3.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 07:03:08.295253 spgrep-0.3.3/src/spgrep/
--rw-r--r--   0 runner    (1001) docker     (123)      623 2023-01-11 07:03:01.000000 spgrep-0.3.3/src/spgrep/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    29458 2023-01-11 07:03:01.000000 spgrep-0.3.3/src/spgrep/core.py
--rw-r--r--   0 runner    (1001) docker     (123)    12905 2023-01-11 07:03:01.000000 spgrep-0.3.3/src/spgrep/corep.py
--rw-r--r--   0 runner    (1001) docker     (123)     8269 2023-01-11 07:03:01.000000 spgrep-0.3.3/src/spgrep/group.py
--rw-r--r--   0 runner    (1001) docker     (123)    24816 2023-01-11 07:03:01.000000 spgrep-0.3.3/src/spgrep/irreps.py
--rw-r--r--   0 runner    (1001) docker     (123)    25846 2023-01-11 07:03:01.000000 spgrep-0.3.3/src/spgrep/pointgroup.py
--rw-r--r--   0 runner    (1001) docker     (123)    11626 2023-01-11 07:03:01.000000 spgrep-0.3.3/src/spgrep/representation.py
--rw-r--r--   0 runner    (1001) docker     (123)     8027 2023-01-11 07:03:01.000000 spgrep-0.3.3/src/spgrep/spinor.py
--rw-r--r--   0 runner    (1001) docker     (123)     4149 2023-01-11 07:03:01.000000 spgrep-0.3.3/src/spgrep/tensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     6650 2023-01-11 07:03:01.000000 spgrep-0.3.3/src/spgrep/transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     5615 2023-01-11 07:03:01.000000 spgrep-0.3.3/src/spgrep/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 07:03:08.295253 spgrep-0.3.3/src/spgrep.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4751 2023-01-11 07:03:08.000000 spgrep-0.3.3/src/spgrep.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2185 2023-01-11 07:03:08.000000 spgrep-0.3.3/src/spgrep.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-11 07:03:08.000000 spgrep-0.3.3/src/spgrep.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-11 07:03:08.000000 spgrep-0.3.3/src/spgrep.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-01-11 07:03:08.000000 spgrep-0.3.3/src/spgrep.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-01-11 07:03:08.000000 spgrep-0.3.3/src/spgrep.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 07:03:08.295253 spgrep-0.3.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     4562 2023-01-11 07:03:01.000000 spgrep-0.3.3/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2957 2023-01-11 07:03:01.000000 spgrep-0.3.3/tests/test_corep.py
--rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-01-11 07:03:01.000000 spgrep-0.3.3/tests/test_group.py
--rw-r--r--   0 runner    (1001) docker     (123)     9228 2023-01-11 07:03:01.000000 spgrep-0.3.3/tests/test_irreps.py
--rw-r--r--   0 runner    (1001) docker     (123)     3484 2023-01-11 07:03:01.000000 spgrep-0.3.3/tests/test_pir.py
--rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-01-11 07:03:01.000000 spgrep-0.3.3/tests/test_pointgroup.py
--rw-r--r--   0 runner    (1001) docker     (123)     1864 2023-01-11 07:03:01.000000 spgrep-0.3.3/tests/test_representation.py
--rw-r--r--   0 runner    (1001) docker     (123)     5274 2023-01-11 07:03:01.000000 spgrep-0.3.3/tests/test_spinor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3302 2023-01-11 07:03:01.000000 spgrep-0.3.3/tests/test_tensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1362 2023-01-11 07:03:01.000000 spgrep-0.3.3/tests/test_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     2245 2023-01-11 07:03:01.000000 spgrep-0.3.3/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:09:22.205858 spgrep-0.3.4/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:09:22.185858 spgrep-0.3.4/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:09:22.185858 spgrep-0.3.4/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-05-17 22:09:14.000000 spgrep-0.3.4/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (123)      631 2023-05-17 22:09:14.000000 spgrep-0.3.4/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (123)      206 2023-05-17 22:09:14.000000 spgrep-0.3.4/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:09:22.185858 spgrep-0.3.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2051 2023-05-17 22:09:14.000000 spgrep-0.3.4/.github/workflows/deploy.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      846 2023-05-17 22:09:14.000000 spgrep-0.3.4/.github/workflows/draft-pdf.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2021 2023-05-17 22:09:14.000000 spgrep-0.3.4/.github/workflows/testing.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1927 2023-05-17 22:09:14.000000 spgrep-0.3.4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1320 2023-05-17 22:09:14.000000 spgrep-0.3.4/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-05-17 22:09:14.000000 spgrep-0.3.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4763 2023-05-17 22:09:22.205858 spgrep-0.3.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3870 2023-05-17 22:09:14.000000 spgrep-0.3.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:09:22.185858 spgrep-0.3.4/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:09:22.189858 spgrep-0.3.4/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 22:09:14.000000 spgrep-0.3.4/docs/_static/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:09:22.189858 spgrep-0.3.4/docs/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      339 2023-05-17 22:09:14.000000 spgrep-0.3.4/docs/api/api.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3855 2023-05-17 22:09:14.000000 spgrep-0.3.4/docs/api/api_core.md
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-05-17 22:09:14.000000 spgrep-0.3.4/docs/api/api_corep.md
+-rw-r--r--   0 runner    (1001) docker     (123)      687 2023-05-17 22:09:14.000000 spgrep-0.3.4/docs/api/api_group.md
+-rw-r--r--   0 runner    (1001) docker     (123)      621 2023-05-17 22:09:14.000000 spgrep-0.3.4/docs/api/api_irreps.md
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-17 22:09:14.000000 spgrep-0.3.4/docs/api/api_pointgroup.md
+-rw-r--r--   0 runner    (1001) docker     (123)      865 2023-05-17 22:09:14.000000 spgrep-0.3.4/docs/api/api_representation.md
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-05-17 22:09:14.000000 spgrep-0.3.4/docs/api/api_spinor.md
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-05-17 22:09:14.000000 spgrep-0.3.4/docs/api/api_tensor.md
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-05-17 22:09:14.000000 spgrep-0.3.4/docs/api/api_transformation.md
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-05-17 22:09:14.000000 spgrep-0.3.4/docs/api/api_utils.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2223 2023-05-17 22:09:14.000000 spgrep-0.3.4/docs/changelog.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3213 2023-05-17 22:09:14.000000 spgrep-0.3.4/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:09:22.189858 spgrep-0.3.4/docs/development/
+-rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-05-17 22:09:14.000000 spgrep-0.3.4/docs/development/development.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3566 2023-05-17 22:09:14.000000 spgrep-0.3.4/docs/development/memo.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:09:22.189858 spgrep-0.3.4/docs/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-05-17 22:09:14.000000 spgrep-0.3.4/docs/examples/examples.md
+-rw-r--r--   0 runner    (1001) docker     (123)    24882 2023-05-17 22:09:14.000000 spgrep-0.3.4/docs/examples/lattice_vibration.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     5525 2023-05-17 22:09:14.000000 spgrep-0.3.4/docs/examples/spin_representation.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    36342 2023-05-17 22:09:14.000000 spgrep-0.3.4/docs/examples/symmetry_adapted_tensor.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:09:22.189858 spgrep-0.3.4/docs/formulation/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:09:22.189858 spgrep-0.3.4/docs/formulation/algorithm/
+-rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-05-17 22:09:14.000000 spgrep-0.3.4/docs/formulation/algorithm/algorithm.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2960 2023-05-17 22:09:14.000000 spgrep-0.3.4/docs/formulation/algorithm/intertwiner.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4288 2023-05-17 22:09:14.000000 spgrep-0.3.4/docs/formulation/algorithm/irreps_from_chain.md
+-rw-r--r--   0 runner    (1001) docker     (123)     5869 2023-05-17 22:09:14.000000 spgrep-0.3.4/docs/formulation/algorithm/irreps_from_regular.md
+-rw-r--r--   0 runner    (1001) docker     (123)      872 2023-05-17 22:09:14.000000 spgrep-0.3.4/docs/formulation/algorithm/point_group_chain.mmd
+-rw-r--r--   0 runner    (1001) docker     (123)    42997 2023-05-17 22:09:14.000000 spgrep-0.3.4/docs/formulation/algorithm/point_group_chain.mmd.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      505 2023-05-17 22:09:14.000000 spgrep-0.3.4/docs/formulation/formulation.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:09:22.193858 spgrep-0.3.4/docs/formulation/irreps/
+-rw-r--r--   0 runner    (1001) docker     (123)     6712 2023-05-17 22:09:14.000000 spgrep-0.3.4/docs/formulation/irreps/corep.md
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-05-17 22:09:14.000000 spgrep-0.3.4/docs/formulation/irreps/irreps.md
+-rw-r--r--   0 runner    (1001) docker     (123)     9358 2023-05-17 22:09:14.000000 spgrep-0.3.4/docs/formulation/irreps/reality.md
+-rw-r--r--   0 runner    (1001) docker     (123)     8879 2023-05-17 22:09:14.000000 spgrep-0.3.4/docs/formulation/irreps/spacegroup_irreps.md
+-rw-r--r--   0 runner    (1001) docker     (123)     8812 2023-05-17 22:09:14.000000 spgrep-0.3.4/docs/formulation/irreps/spinor.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3480 2023-05-17 22:09:14.000000 spgrep-0.3.4/docs/formulation/projection.md
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-17 22:09:14.000000 spgrep-0.3.4/docs/genindex.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-05-17 22:09:14.000000 spgrep-0.3.4/docs/index.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:09:22.193858 spgrep-0.3.4/docs/paper/
+-rw-r--r--   0 runner    (1001) docker     (123)    11271 2023-05-17 22:09:14.000000 spgrep-0.3.4/docs/paper/paper.bib
+-rw-r--r--   0 runner    (1001) docker     (123)     5687 2023-05-17 22:09:14.000000 spgrep-0.3.4/docs/paper/paper.md
+-rw-r--r--   0 runner    (1001) docker     (123)     8775 2023-05-17 22:09:14.000000 spgrep-0.3.4/docs/references.bib
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:09:22.193858 spgrep-0.3.4/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-05-17 22:09:14.000000 spgrep-0.3.4/examples/basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3738 2023-05-17 22:09:14.000000 spgrep-0.3.4/examples/lattice_vibration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3368 2023-05-17 22:09:14.000000 spgrep-0.3.4/examples/phonopy_mp-2998.yaml.xz
+-rw-r--r--   0 runner    (1001) docker     (123)      529 2023-05-17 22:09:14.000000 spgrep-0.3.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-05-17 22:09:22.205858 spgrep-0.3.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2951 2023-05-17 22:09:14.000000 spgrep-0.3.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:09:22.181857 spgrep-0.3.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:09:22.197858 spgrep-0.3.4/src/spgrep/
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-05-17 22:09:14.000000 spgrep-0.3.4/src/spgrep/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29560 2023-05-17 22:09:14.000000 spgrep-0.3.4/src/spgrep/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12905 2023-05-17 22:09:14.000000 spgrep-0.3.4/src/spgrep/corep.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8269 2023-05-17 22:09:14.000000 spgrep-0.3.4/src/spgrep/group.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24816 2023-05-17 22:09:14.000000 spgrep-0.3.4/src/spgrep/irreps.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30625 2023-05-17 22:09:14.000000 spgrep-0.3.4/src/spgrep/pointgroup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11626 2023-05-17 22:09:14.000000 spgrep-0.3.4/src/spgrep/representation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8027 2023-05-17 22:09:14.000000 spgrep-0.3.4/src/spgrep/spinor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4149 2023-05-17 22:09:14.000000 spgrep-0.3.4/src/spgrep/tensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6650 2023-05-17 22:09:14.000000 spgrep-0.3.4/src/spgrep/transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5615 2023-05-17 22:09:14.000000 spgrep-0.3.4/src/spgrep/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:09:22.201858 spgrep-0.3.4/src/spgrep.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4763 2023-05-17 22:09:22.000000 spgrep-0.3.4/src/spgrep.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2180 2023-05-17 22:09:22.000000 spgrep-0.3.4/src/spgrep.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 22:09:22.000000 spgrep-0.3.4/src/spgrep.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 22:09:22.000000 spgrep-0.3.4/src/spgrep.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-05-17 22:09:22.000000 spgrep-0.3.4/src/spgrep.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-17 22:09:22.000000 spgrep-0.3.4/src/spgrep.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:09:22.205858 spgrep-0.3.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     4562 2023-05-17 22:09:14.000000 spgrep-0.3.4/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2957 2023-05-17 22:09:14.000000 spgrep-0.3.4/tests/test_corep.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-05-17 22:09:14.000000 spgrep-0.3.4/tests/test_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9228 2023-05-17 22:09:14.000000 spgrep-0.3.4/tests/test_irreps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3484 2023-05-17 22:09:14.000000 spgrep-0.3.4/tests/test_pir.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-05-17 22:09:14.000000 spgrep-0.3.4/tests/test_pointgroup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1864 2023-05-17 22:09:14.000000 spgrep-0.3.4/tests/test_representation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5274 2023-05-17 22:09:14.000000 spgrep-0.3.4/tests/test_spinor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3302 2023-05-17 22:09:14.000000 spgrep-0.3.4/tests/test_tensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1362 2023-05-17 22:09:14.000000 spgrep-0.3.4/tests/test_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2245 2023-05-17 22:09:14.000000 spgrep-0.3.4/tests/test_utils.py
```

### Comparing `spgrep-0.3.3/.github/ISSUE_TEMPLATE/feature_request.md` & `spgrep-0.3.4/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `spgrep-0.3.3/.github/workflows/deploy.yml` & `spgrep-0.3.4/.github/workflows/deploy.yml`

 * *Files identical despite different names*

### Comparing `spgrep-0.3.3/.github/workflows/draft-pdf.yml` & `spgrep-0.3.4/.github/workflows/draft-pdf.yml`

 * *Files identical despite different names*

### Comparing `spgrep-0.3.3/.github/workflows/testing.yml` & `spgrep-0.3.4/.github/workflows/testing.yml`

 * *Files identical despite different names*

### Comparing `spgrep-0.3.3/.gitignore` & `spgrep-0.3.4/.gitignore`

 * *Files identical despite different names*

### Comparing `spgrep-0.3.3/.pre-commit-config.yaml` & `spgrep-0.3.4/.pre-commit-config.yaml`

 * *Files 19% similar despite different names*

```diff
@@ -8,52 +8,52 @@
       - id: check-added-large-files
       - id: check-yaml
       - id: check-json
       - id: debug-statements
       - id: end-of-file-fixer
   # formatter
   - repo: https://github.com/psf/black
-    rev: 22.12.0
+    rev: 23.3.0
     hooks:
     - id: black
   # linter
   - repo: https://github.com/PyCQA/flake8
     rev: 6.0.0
     hooks:
     - id: flake8
       exclude: ^docs/
   # type annotation
   - repo: https://github.com/pre-commit/mirrors-mypy
-    rev: v0.991
+    rev: v1.3.0
     hooks:
     - id: mypy
       exclude: ^docs/
   # isort
   - repo: https://github.com/pycqa/isort
-    rev: 5.11.4
+    rev: 5.12.0
     hooks:
       - id: isort
         name: isort (python)
         args: ["--profile", "black"]
       - id: isort
         name: isort (cython)
         types: [cython]
       - id: isort
         name: isort (pyi)
         types: [pyi]
   # Upgrade syntax
   - repo: https://github.com/asottile/pyupgrade
-    rev: v3.3.1
+    rev: v3.4.0
     hooks:
       - id: pyupgrade
   # Docstring
   - repo: https://github.com/pycqa/pydocstyle
-    rev: 6.2.3
+    rev: 6.3.0
     hooks:
     - id: pydocstyle
       additional_dependencies: ["toml"]
       files: ^src/spgrep/
   # Notebook
   - repo: https://github.com/nbQA-dev/nbQA
-    rev: 1.6.1
+    rev: 1.7.0
     hooks:
       - id: nbqa-black
```

### Comparing `spgrep-0.3.3/LICENSE` & `spgrep-0.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `spgrep-0.3.3/PKG-INFO` & `spgrep-0.3.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spgrep
-Version: 0.3.3
+Version: 0.3.4
 Summary: On-the-fly generator of space-group irreducible representations
 Home-page: https://github.com/spglib/spgrep
 Author: Kohei Shinohara
 Author-email: kshinohara0508@gmail.com
 License: BSD
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
@@ -94,15 +94,15 @@
 # Two two-dimensional irreps
 for irrep in irreps:
     print(get_character(irrep))
 # [2.+0.j 0.+0.j 0.+0.j 2.+0.j 0.+0.j 0.+0.j 0.+0.j 0.+0.j]
 # [2.+0.j 0.+0.j 0.+0.j -2.+0.j 0.+0.j 0.+0.j 0.+0.j 0.+0.j]
 ```
 
-See [example pages](docs/examples/examples) for more detailed use cases and [API summary](docs/api/api_core) for summary of functionalities.
+See [example pages](docs/examples/examples.md) for more detailed use cases and [API summary](docs/api/api_core.md) for summary of functionalities.
 
 ## Installation
 
 Spgrep works with Python3.8+ and can be installed via PyPI:
 ```shell
 pip install spgrep
 ```
@@ -114,20 +114,20 @@
 git clone git@github.com:spglib/spgrep.git
 cd spgrep
 pip install -e .
 ```
 
 ## Change log
 
-See the [change log](docs/changelog) for recent changes.
+See the [change log](docs/changelog.md) for recent changes.
 
 ## How to contribute
 
 We welcome any contributions to improve functionalities.
 Please open [issues](https://github.com/spglib/spgrep/issues?q=is%3Aissue+is%3Aopen+sort%3Aupdated-desc) or create [pull requests](https://github.com/spglib/spgrep/pulls?q=is%3Apr+is%3Aopen+sort%3Aupdated-desc).
-See the [development page](docs/development/development) for preparing an environment.
+See the [development page](docs/development/development.md) for preparing an environment.
 
 ## License
 
 Spgrep is released under a BSD 3-clause license.
```

### Comparing `spgrep-0.3.3/README.md` & `spgrep-0.3.4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -68,15 +68,15 @@
 # Two two-dimensional irreps
 for irrep in irreps:
     print(get_character(irrep))
 # [2.+0.j 0.+0.j 0.+0.j 2.+0.j 0.+0.j 0.+0.j 0.+0.j 0.+0.j]
 # [2.+0.j 0.+0.j 0.+0.j -2.+0.j 0.+0.j 0.+0.j 0.+0.j 0.+0.j]
 ```
 
-See [example pages](docs/examples/examples) for more detailed use cases and [API summary](docs/api/api_core) for summary of functionalities.
+See [example pages](docs/examples/examples.md) for more detailed use cases and [API summary](docs/api/api_core.md) for summary of functionalities.
 
 ## Installation
 
 Spgrep works with Python3.8+ and can be installed via PyPI:
 ```shell
 pip install spgrep
 ```
@@ -88,18 +88,18 @@
 git clone git@github.com:spglib/spgrep.git
 cd spgrep
 pip install -e .
 ```
 
 ## Change log
 
-See the [change log](docs/changelog) for recent changes.
+See the [change log](docs/changelog.md) for recent changes.
 
 ## How to contribute
 
 We welcome any contributions to improve functionalities.
 Please open [issues](https://github.com/spglib/spgrep/issues?q=is%3Aissue+is%3Aopen+sort%3Aupdated-desc) or create [pull requests](https://github.com/spglib/spgrep/pulls?q=is%3Apr+is%3Aopen+sort%3Aupdated-desc).
-See the [development page](docs/development/development) for preparing an environment.
+See the [development page](docs/development/development.md) for preparing an environment.
 
 ## License
 
 Spgrep is released under a BSD 3-clause license.
```

### Comparing `spgrep-0.3.3/docs/api/api_core.md` & `spgrep-0.3.4/docs/api/api_core.md`

 * *Files identical despite different names*

### Comparing `spgrep-0.3.3/docs/api/api_group.md` & `spgrep-0.3.4/docs/api/api_group.md`

 * *Files identical despite different names*

### Comparing `spgrep-0.3.3/docs/api/api_irreps.md` & `spgrep-0.3.4/docs/api/api_irreps.md`

 * *Files identical despite different names*

### Comparing `spgrep-0.3.3/docs/api/api_representation.md` & `spgrep-0.3.4/docs/api/api_representation.md`

 * *Files identical despite different names*

### Comparing `spgrep-0.3.3/docs/changelog.md` & `spgrep-0.3.4/docs/changelog.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,15 @@
 # Change Log
 
+## v0.3.4 (18 May 2023)
+
+- Fix comments for symmetry operations in `src/spgrep/pointgroup.py`
+- Fix docutils and sphinx versions not to collapse documents [[#66]](https://github.com/spglib/spgrep/pull/66)
+- Fix data path for phonon example [[#78]](https://github.com/spglib/spgrep/pull/78)
+
 ## v0.3.3 (11 Jan. 2023)
 - Improve comparison between linear subspaces [[#53]](https://github.com/spglib/spgrep/pull/53)
     - Use Grassmann distance to measure linear subspaces: {func}`spgrep.utils.grassmann_distance`
     - Drop `spgrep.utils.contain_space`
 
 ## v0.3.2 (28 Dec. 2022)
 - Clean documents and add JOSS draft [[#50]](https://github.com/spglib/spgrep/pull/50)
```

### Comparing `spgrep-0.3.3/docs/conf.py` & `spgrep-0.3.4/docs/conf.py`

 * *Files identical despite different names*

### Comparing `spgrep-0.3.3/docs/development/development.md` & `spgrep-0.3.4/docs/development/development.md`

 * *Files 3% similar despite different names*

```diff
@@ -44,16 +44,15 @@
 python -m setuptools_scm
 
 # Update changelog here
 vim docs/changelog.md
 
 # Push with tag
 git tag <next-version>
-git push origin main
-git push origin --tags
+git push origin <next-version>
 ```
 
 ## Subpages
 
 ```{toctree}
   :maxdepth: 1
   Memo <memo>
```

### Comparing `spgrep-0.3.3/docs/development/memo.md` & `spgrep-0.3.4/docs/development/memo.md`

 * *Files identical despite different names*

### Comparing `spgrep-0.3.3/docs/examples/phonopy_mp-2998.yaml.xz` & `spgrep-0.3.4/examples/phonopy_mp-2998.yaml.xz`

 * *Files identical despite different names*

### Comparing `spgrep-0.3.3/docs/examples/spin_representation.ipynb` & `spgrep-0.3.4/docs/examples/spin_representation.ipynb`

 * *Files identical despite different names*

### Comparing `spgrep-0.3.3/docs/examples/symmetry_adapted_tensor.ipynb` & `spgrep-0.3.4/docs/examples/symmetry_adapted_tensor.ipynb`

 * *Files identical despite different names*

### Comparing `spgrep-0.3.3/docs/formulation/algorithm/algorithm.md` & `spgrep-0.3.4/docs/formulation/algorithm/algorithm.md`

 * *Files identical despite different names*

### Comparing `spgrep-0.3.3/docs/formulation/algorithm/intertwiner.md` & `spgrep-0.3.4/docs/formulation/algorithm/intertwiner.md`

 * *Files identical despite different names*

### Comparing `spgrep-0.3.3/docs/formulation/algorithm/irreps_from_chain.md` & `spgrep-0.3.4/docs/formulation/algorithm/irreps_from_chain.md`

 * *Files identical despite different names*

### Comparing `spgrep-0.3.3/docs/formulation/algorithm/irreps_from_regular.md` & `spgrep-0.3.4/docs/formulation/algorithm/irreps_from_regular.md`

 * *Files identical despite different names*

### Comparing `spgrep-0.3.3/docs/formulation/algorithm/point_group_chain.mmd` & `spgrep-0.3.4/docs/formulation/algorithm/point_group_chain.mmd`

 * *Files identical despite different names*

### Comparing `spgrep-0.3.3/docs/formulation/algorithm/point_group_chain.mmd.svg` & `spgrep-0.3.4/docs/formulation/algorithm/point_group_chain.mmd.svg`

 * *Files identical despite different names*

### Comparing `spgrep-0.3.3/docs/formulation/irreps/corep.md` & `spgrep-0.3.4/docs/formulation/irreps/corep.md`

 * *Files identical despite different names*

### Comparing `spgrep-0.3.3/docs/formulation/irreps/reality.md` & `spgrep-0.3.4/docs/formulation/irreps/reality.md`

 * *Files identical despite different names*

### Comparing `spgrep-0.3.3/docs/formulation/irreps/spacegroup_irreps.md` & `spgrep-0.3.4/docs/formulation/irreps/spacegroup_irreps.md`

 * *Files identical despite different names*

### Comparing `spgrep-0.3.3/docs/formulation/irreps/spinor.md` & `spgrep-0.3.4/docs/formulation/irreps/spinor.md`

 * *Files identical despite different names*

### Comparing `spgrep-0.3.3/docs/formulation/projection.md` & `spgrep-0.3.4/docs/formulation/projection.md`

 * *Files identical despite different names*

### Comparing `spgrep-0.3.3/docs/paper/paper.bib` & `spgrep-0.3.4/docs/paper/paper.bib`

 * *Files 1% similar despite different names*

```diff
@@ -246,15 +246,15 @@
   url = {https://doi.org/10.1524/zkri.2006.221.1.15},
   title = {Bilbao Crystallographic Server: I. Databases and crystallographic computing programs},
   author = {Aroyo, M. I. and Perez-Mato, Juan Manuel and Capillas, Cesar and Kroumova, Eli and Ivantchev, Svetoslav and Madariaga, Gotzon and Kirov, Asen and Wondratschek, Hans},
   pages = {15--27},
   volume = {221},
   number = {1},
   journal = {Zeitschrift f\"{u}r Kristallographie - Crystalline Materials},
-  doi = {doi:10.1524/zkri.2006.221.1.15},
+  doi = {10.1524/zkri.2006.221.1.15},
   year = {2006},
   lastchecked = {2022-12-19}
 }
 @article{Aroyo:xo5013,
   author = "Aroyo, M. I. and Kirov, A. and Capillas, C. and Perez-Mato, J. M. and Wondratschek, H.",
   title = "{Bilbao Crystallographic Server. II. Representations of crystallographic point groups and space groups}",
   journal = "Acta Crystallographica Section A",
```

### Comparing `spgrep-0.3.3/docs/paper/paper.md` & `spgrep-0.3.4/docs/paper/paper.md`

 * *Files identical despite different names*

### Comparing `spgrep-0.3.3/docs/references.bib` & `spgrep-0.3.4/docs/references.bib`

 * *Files identical despite different names*

### Comparing `spgrep-0.3.3/examples/basic.py` & `spgrep-0.3.4/examples/basic.py`

 * *Files identical despite different names*

### Comparing `spgrep-0.3.3/examples/lattice_vibration.py` & `spgrep-0.3.4/examples/lattice_vibration.py`

 * *Files 2% similar despite different names*

```diff
@@ -93,12 +93,13 @@
     )
     assert check_spacegroup_representation(little_rotations, little_translations, qpoint, rep)
 
     all_basis = []
     for irrep in irreps:
         all_basis.extend(project_to_irrep(rep, irrep))
 
+    # http://phonondb.mtl.kyoto-u.ac.jp/xz-files/phonopy_mp-2998.yaml.xz
     path = Path(__file__).resolve().parent / "phonopy_mp-2998.yaml.xz"
     ph = phonopy.load(path)
 
     ph.dynamical_matrix.run(qpoint)
     dynamical_matrix = ph.dynamical_matrix.dynamical_matrix
```

### Comparing `spgrep-0.3.3/pyproject.toml` & `spgrep-0.3.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `spgrep-0.3.3/setup.py` & `spgrep-0.3.4/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -19,33 +19,36 @@
     "numpy>=1.20.1",
     "spglib>=2.0.2",
 ]
 
 # What packages are optional?
 EXTRAS = {
     "dev": [
-        "pytest==7.2.0",
+        "pytest==7.3.1",
         "pytest-cov==4.0.0",
         "pre-commit",
         "black",
         "mypy",
         "flake8",
         "pyupgrade",
         "pydocstyle",
         "nbqa",
-        "phonopy==2.17.1",
+        "phonopy==2.19.0",
         # Jupyter notebook
         "notebook",
         "matplotlib",
         "seaborn",
         "ipython",
         "ipykernel",
     ],
     "docs": [
-        "sphinx",
+        # We cannot update sphinx to >6 until docutils==0.20 is released: https://github.com/mcmtroffaes/sphinxcontrib-bibtex/issues/322
+        # Another issue requires sphinx<4.3 (fixed in pydata-sphinx-theme>=0.8.0): https://github.com/pydata/pydata-sphinx-theme/pull/509
+        "docutils<=0.17",
+        "sphinx<4.3",
         "sphinx-autobuild",
         "nbsphinx",
         "sphinxcontrib-bibtex",
         "myst-parser",
         "sphinx-book-theme",
         "linkify-it-py",
     ],
```

### Comparing `spgrep-0.3.3/src/spgrep/__init__.py` & `spgrep-0.3.4/src/spgrep/__init__.py`

 * *Files identical despite different names*

### Comparing `spgrep-0.3.3/src/spgrep/core.py` & `spgrep-0.3.4/src/spgrep/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -272,31 +272,34 @@
     kpoint: NDArrayFloat | None = None,
     method: Literal["Neto", "random"] = "Neto",
     reciprocal_lattice: NDArrayFloat | None = None,
     symprec: float = 1e-5,
     rtol: float = 1e-5,
     atol: float = 1e-8,
     max_num_random_generations: int = 4,
-) -> tuple[
-    list[NDArrayComplex],
-    NDArrayComplex,
-    NDArrayComplex,
-    NDArrayInt,
-    NDArrayFloat,
-    NDArrayInt,
-] | tuple[
-    list[NDArrayComplex],
-    NDArrayComplex,
-    NDArrayComplex,
-    NDArrayBool,
-    NDArrayInt,
-    NDArrayFloat,
-    NDArrayInt,
-    NDArrayInt,
-]:
+) -> (
+    tuple[
+        list[NDArrayComplex],
+        NDArrayComplex,
+        NDArrayComplex,
+        NDArrayInt,
+        NDArrayFloat,
+        NDArrayInt,
+    ]
+    | tuple[
+        list[NDArrayComplex],
+        NDArrayComplex,
+        NDArrayComplex,
+        NDArrayBool,
+        NDArrayInt,
+        NDArrayFloat,
+        NDArrayInt,
+        NDArrayInt,
+    ]
+):
     r"""Compute all irreducible representations :math:`\mathbf{\Gamma}^{\mathbf{k}\alpha}` of space group of given structure up to unitary transformation for spinor.
 
     Each irrep :math:`\mathbf{\Gamma}^{\mathbf{k}\alpha}` satisfies
 
     .. math::
        \mathbf{\Gamma}^{\mathbf{k}\alpha}((\mathbf{S}_{i}, \mathbf{w}_{i})) \mathbf{\Gamma}^{\mathbf{k}\alpha}((\mathbf{S}_{j}, \mathbf{w}_{j}))
        = z(\mathbf{S}_{i}, \mathbf{S}_{j}) \mathbf{\Gamma}^{\mathbf{k}\alpha}((\mathbf{S}_{i}, \mathbf{w}_{i})(\mathbf{S}_{j}, \mathbf{w}_{j})).
@@ -462,17 +465,20 @@
     translations: NDArrayFloat,
     time_reversals: NDArrayInt | None = None,
     kpoint: NDArrayFloat | None = None,
     method: Literal["Neto", "random"] = "Neto",
     rtol: float = 1e-5,
     atol: float = 1e-8,
     max_num_random_generations: int = 4,
-) -> tuple[list[NDArrayComplex], NDArrayComplex, NDArrayComplex, NDArrayInt] | tuple[
-    list[NDArrayComplex], list[int], NDArrayComplex, NDArrayComplex, NDArrayBool, NDArrayInt
-]:
+) -> (
+    tuple[list[NDArrayComplex], NDArrayComplex, NDArrayComplex, NDArrayInt]
+    | tuple[
+        list[NDArrayComplex], list[int], NDArrayComplex, NDArrayComplex, NDArrayBool, NDArrayInt
+    ]
+):
     r"""Compute all irreducible representations :math:`\mathbf{\Gamma}^{\mathbf{k}\alpha}` of given space group up to unitary transformation for spinor.
 
     Each irrep :math:`\mathbf{\Gamma}^{\mathbf{k}\alpha}` satisfies
 
     .. math::
        \mathbf{\Gamma}^{\mathbf{k}\alpha}((\mathbf{S}_{i}, \mathbf{w}_{i})) \mathbf{\Gamma}^{\mathbf{k}\alpha}((\mathbf{S}_{j}, \mathbf{w}_{j}))
        = z(\mathbf{S}_{i}, \mathbf{S}_{j}) \mathbf{\Gamma}^{\mathbf{k}\alpha}((\mathbf{S}_{i}, \mathbf{w}_{i})(\mathbf{S}_{j}, \mathbf{w}_{j})).
@@ -590,17 +596,18 @@
     lattice: NDArrayFloat,
     rotations: NDArrayInt,
     time_reversals: NDArrayInt | None = None,
     method: Literal["Neto", "random"] = "Neto",
     rtol: float = 1e-5,
     atol: float = 1e-8,
     max_num_random_generations: int = 4,
-) -> tuple[list[NDArrayComplex], NDArrayComplex, NDArrayComplex] | tuple[
-    list[NDArrayComplex], list[int], NDArrayComplex, NDArrayComplex, NDArrayBool
-]:
+) -> (
+    tuple[list[NDArrayComplex], NDArrayComplex, NDArrayComplex]
+    | tuple[list[NDArrayComplex], list[int], NDArrayComplex, NDArrayComplex, NDArrayBool]
+):
     r"""Compute all irreducible representations :math:`\mathbf{D}^{\alpha}` of given crystallographic point group up to unitary transformation for spinor.
 
     Each irrep :math:`\mathbf{D}^{\alpha}` satisfies
 
     .. math::
        \mathbf{D}^{\alpha}(\mathbf{S}_{i}) \mathbf{D}^{\alpha}(\mathbf{S}_{j})
        = z(\mathbf{S}_{i}, \mathbf{S}_{j}) \mathbf{D}^{\alpha}(\mathbf{S}_{k}).
```

### Comparing `spgrep-0.3.3/src/spgrep/corep.py` & `spgrep-0.3.4/src/spgrep/corep.py`

 * *Files identical despite different names*

### Comparing `spgrep-0.3.3/src/spgrep/group.py` & `spgrep-0.3.4/src/spgrep/group.py`

 * *Files identical despite different names*

### Comparing `spgrep-0.3.3/src/spgrep/irreps.py` & `spgrep-0.3.4/src/spgrep/irreps.py`

 * *Files identical despite different names*

### Comparing `spgrep-0.3.3/src/spgrep/representation.py` & `spgrep-0.3.4/src/spgrep/representation.py`

 * *Files identical despite different names*

### Comparing `spgrep-0.3.3/src/spgrep/spinor.py` & `spgrep-0.3.4/src/spgrep/spinor.py`

 * *Files identical despite different names*

### Comparing `spgrep-0.3.3/src/spgrep/tensor.py` & `spgrep-0.3.4/src/spgrep/tensor.py`

 * *Files identical despite different names*

### Comparing `spgrep-0.3.3/src/spgrep/transform.py` & `spgrep-0.3.4/src/spgrep/transform.py`

 * *Files identical despite different names*

### Comparing `spgrep-0.3.3/src/spgrep/utils.py` & `spgrep-0.3.4/src/spgrep/utils.py`

 * *Files identical despite different names*

### Comparing `spgrep-0.3.3/src/spgrep.egg-info/PKG-INFO` & `spgrep-0.3.4/src/spgrep.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spgrep
-Version: 0.3.3
+Version: 0.3.4
 Summary: On-the-fly generator of space-group irreducible representations
 Home-page: https://github.com/spglib/spgrep
 Author: Kohei Shinohara
 Author-email: kshinohara0508@gmail.com
 License: BSD
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
@@ -94,15 +94,15 @@
 # Two two-dimensional irreps
 for irrep in irreps:
     print(get_character(irrep))
 # [2.+0.j 0.+0.j 0.+0.j 2.+0.j 0.+0.j 0.+0.j 0.+0.j 0.+0.j]
 # [2.+0.j 0.+0.j 0.+0.j -2.+0.j 0.+0.j 0.+0.j 0.+0.j 0.+0.j]
 ```
 
-See [example pages](docs/examples/examples) for more detailed use cases and [API summary](docs/api/api_core) for summary of functionalities.
+See [example pages](docs/examples/examples.md) for more detailed use cases and [API summary](docs/api/api_core.md) for summary of functionalities.
 
 ## Installation
 
 Spgrep works with Python3.8+ and can be installed via PyPI:
 ```shell
 pip install spgrep
 ```
@@ -114,20 +114,20 @@
 git clone git@github.com:spglib/spgrep.git
 cd spgrep
 pip install -e .
 ```
 
 ## Change log
 
-See the [change log](docs/changelog) for recent changes.
+See the [change log](docs/changelog.md) for recent changes.
 
 ## How to contribute
 
 We welcome any contributions to improve functionalities.
 Please open [issues](https://github.com/spglib/spgrep/issues?q=is%3Aissue+is%3Aopen+sort%3Aupdated-desc) or create [pull requests](https://github.com/spglib/spgrep/pulls?q=is%3Apr+is%3Aopen+sort%3Aupdated-desc).
-See the [development page](docs/development/development) for preparing an environment.
+See the [development page](docs/development/development.md) for preparing an environment.
 
 ## License
 
 Spgrep is released under a BSD 3-clause license.
```

### Comparing `spgrep-0.3.3/src/spgrep.egg-info/SOURCES.txt` & `spgrep-0.3.4/src/spgrep.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,14 @@
 docs/api/api_tensor.md
 docs/api/api_transformation.md
 docs/api/api_utils.md
 docs/development/development.md
 docs/development/memo.md
 docs/examples/examples.md
 docs/examples/lattice_vibration.ipynb
-docs/examples/phonopy_mp-2998.yaml.xz
 docs/examples/spin_representation.ipynb
 docs/examples/symmetry_adapted_tensor.ipynb
 docs/formulation/formulation.md
 docs/formulation/projection.md
 docs/formulation/algorithm/algorithm.md
 docs/formulation/algorithm/intertwiner.md
 docs/formulation/algorithm/irreps_from_chain.md
@@ -48,14 +47,15 @@
 docs/formulation/irreps/reality.md
 docs/formulation/irreps/spacegroup_irreps.md
 docs/formulation/irreps/spinor.md
 docs/paper/paper.bib
 docs/paper/paper.md
 examples/basic.py
 examples/lattice_vibration.py
+examples/phonopy_mp-2998.yaml.xz
 src/spgrep/__init__.py
 src/spgrep/core.py
 src/spgrep/corep.py
 src/spgrep/group.py
 src/spgrep/irreps.py
 src/spgrep/pointgroup.py
 src/spgrep/representation.py
```

### Comparing `spgrep-0.3.3/tests/conftest.py` & `spgrep-0.3.4/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `spgrep-0.3.3/tests/test_corep.py` & `spgrep-0.3.4/tests/test_corep.py`

 * *Files identical despite different names*

### Comparing `spgrep-0.3.3/tests/test_group.py` & `spgrep-0.3.4/tests/test_group.py`

 * *Files identical despite different names*

### Comparing `spgrep-0.3.3/tests/test_irreps.py` & `spgrep-0.3.4/tests/test_irreps.py`

 * *Files identical despite different names*

### Comparing `spgrep-0.3.3/tests/test_pir.py` & `spgrep-0.3.4/tests/test_pir.py`

 * *Files identical despite different names*

### Comparing `spgrep-0.3.3/tests/test_pointgroup.py` & `spgrep-0.3.4/tests/test_pointgroup.py`

 * *Files identical despite different names*

### Comparing `spgrep-0.3.3/tests/test_representation.py` & `spgrep-0.3.4/tests/test_representation.py`

 * *Files identical despite different names*

### Comparing `spgrep-0.3.3/tests/test_spinor.py` & `spgrep-0.3.4/tests/test_spinor.py`

 * *Files identical despite different names*

### Comparing `spgrep-0.3.3/tests/test_tensor.py` & `spgrep-0.3.4/tests/test_tensor.py`

 * *Files identical despite different names*

### Comparing `spgrep-0.3.3/tests/test_transform.py` & `spgrep-0.3.4/tests/test_transform.py`

 * *Files identical despite different names*

### Comparing `spgrep-0.3.3/tests/test_utils.py` & `spgrep-0.3.4/tests/test_utils.py`

 * *Files identical despite different names*

