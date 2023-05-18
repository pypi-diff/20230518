# Comparing `tmp/ape-vyper-0.6.5.tar.gz` & `tmp/ape-vyper-0.6.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ape-vyper-0.6.5.tar", last modified: Mon May  1 16:01:52 2023, max compression
+gzip compressed data, was "ape-vyper-0.6.6.tar", last modified: Thu May 18 19:07:42 2023, max compression
```

## Comparing `ape-vyper-0.6.5.tar` & `ape-vyper-0.6.6.tar`

### file list

```diff
@@ -1,61 +1,64 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 16:01:52.048531 ape-vyper-0.6.5/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 16:01:52.044531 ape-vyper-0.6.5/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 16:01:52.044531 ape-vyper-0.6.5/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      703 2023-05-01 16:00:37.000000 ape-vyper-0.6.5/.github/ISSUE_TEMPLATE/bug.md
--rw-r--r--   0 runner    (1001) docker     (123)      668 2023-05-01 16:00:37.000000 ape-vyper-0.6.5/.github/ISSUE_TEMPLATE/feature.md
--rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-05-01 16:00:37.000000 ape-vyper-0.6.5/.github/ISSUE_TEMPLATE/work-item.md
--rw-r--r--   0 runner    (1001) docker     (123)      474 2023-05-01 16:00:37.000000 ape-vyper-0.6.5/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (123)      651 2023-05-01 16:00:37.000000 ape-vyper-0.6.5/.github/release-drafter.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 16:01:52.044531 ape-vyper-0.6.5/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      686 2023-05-01 16:00:37.000000 ape-vyper-0.6.5/.github/workflows/commitlint.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-05-01 16:00:37.000000 ape-vyper-0.6.5/.github/workflows/draft.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      616 2023-05-01 16:00:37.000000 ape-vyper-0.6.5/.github/workflows/prtitle.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      623 2023-05-01 16:00:37.000000 ape-vyper-0.6.5/.github/workflows/publish.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2628 2023-05-01 16:00:37.000000 ape-vyper-0.6.5/.github/workflows/test.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1719 2023-05-01 16:00:37.000000 ape-vyper-0.6.5/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-01 16:00:37.000000 ape-vyper-0.6.5/.mdformat.toml
--rw-r--r--   0 runner    (1001) docker     (123)      796 2023-05-01 16:00:37.000000 ape-vyper-0.6.5/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-05-01 16:00:37.000000 ape-vyper-0.6.5/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)    11342 2023-05-01 16:00:37.000000 ape-vyper-0.6.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2782 2023-05-01 16:01:52.048531 ape-vyper-0.6.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1873 2023-05-01 16:00:37.000000 ape-vyper-0.6.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 16:01:52.044531 ape-vyper-0.6.5/ape_vyper/
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-05-01 16:00:37.000000 ape-vyper-0.6.5/ape_vyper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20791 2023-05-01 16:00:37.000000 ape-vyper-0.6.5/ape_vyper/compiler.py
--rw-r--r--   0 runner    (1001) docker     (123)     3818 2023-05-01 16:00:37.000000 ape-vyper-0.6.5/ape_vyper/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-01 16:01:51.000000 ape-vyper-0.6.5/ape_vyper/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 16:01:52.048531 ape-vyper-0.6.5/ape_vyper.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2782 2023-05-01 16:01:51.000000 ape-vyper-0.6.5/ape_vyper.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-05-01 16:01:52.000000 ape-vyper-0.6.5/ape_vyper.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 16:01:51.000000 ape-vyper-0.6.5/ape_vyper.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 16:01:51.000000 ape-vyper-0.6.5/ape_vyper.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      598 2023-05-01 16:01:51.000000 ape-vyper-0.6.5/ape_vyper.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-01 16:01:51.000000 ape-vyper-0.6.5/ape_vyper.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      943 2023-05-01 16:00:37.000000 ape-vyper-0.6.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-05-01 16:01:52.048531 ape-vyper-0.6.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3021 2023-05-01 16:00:37.000000 ape-vyper-0.6.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 16:01:52.048531 ape-vyper-0.6.5/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 16:01:52.044531 ape-vyper-0.6.5/tests/ExampleDependency/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 16:01:52.048531 ape-vyper-0.6.5/tests/ExampleDependency/contracts/
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-01 16:00:37.000000 ape-vyper-0.6.5/tests/ExampleDependency/contracts/Dependency.vy
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 16:00:37.000000 ape-vyper-0.6.5/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      420 2023-05-01 16:00:37.000000 ape-vyper-0.6.5/tests/ape-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2287 2023-05-01 16:00:37.000000 ape-vyper-0.6.5/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 16:01:52.044531 ape-vyper-0.6.5/tests/contracts/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 16:01:52.048531 ape-vyper-0.6.5/tests/contracts/failing_contracts/
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-05-01 16:00:37.000000 ape-vyper-0.6.5/tests/contracts/failing_contracts/contract_undeclared_variable.vy
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-01 16:00:37.000000 ape-vyper-0.6.5/tests/contracts/failing_contracts/contract_unknown_pragma.vy
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 16:01:52.048531 ape-vyper-0.6.5/tests/contracts/passing_contracts/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 16:01:52.048531 ape-vyper-0.6.5/tests/contracts/passing_contracts/DirectoryWithExtension.vy/
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-05-01 16:00:37.000000 ape-vyper-0.6.5/tests/contracts/passing_contracts/DirectoryWithExtension.vy/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     3088 2023-05-01 16:00:37.000000 ape-vyper-0.6.5/tests/contracts/passing_contracts/contract.vy
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-01 16:00:37.000000 ape-vyper-0.6.5/tests/contracts/passing_contracts/contract_no_pragma.vy
--rw-r--r--   0 runner    (1001) docker     (123)      345 2023-05-01 16:00:37.000000 ape-vyper-0.6.5/tests/contracts/passing_contracts/contract_with_dev_messages.vy
--rw-r--r--   0 runner    (1001) docker     (123)     5231 2023-05-01 16:00:37.000000 ape-vyper-0.6.5/tests/contracts/passing_contracts/erc20.vy
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 16:01:52.048531 ape-vyper-0.6.5/tests/contracts/passing_contracts/interfaces/
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-01 16:00:37.000000 ape-vyper-0.6.5/tests/contracts/passing_contracts/interfaces/IFace.vy
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-01 16:00:37.000000 ape-vyper-0.6.5/tests/contracts/passing_contracts/interfaces/IFace2.vy
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-01 16:00:37.000000 ape-vyper-0.6.5/tests/contracts/passing_contracts/older_version.vy
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-05-01 16:00:37.000000 ape-vyper-0.6.5/tests/contracts/passing_contracts/use_iface.vy
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-05-01 16:00:37.000000 ape-vyper-0.6.5/tests/contracts/passing_contracts/use_iface2.vy
--rw-r--r--   0 runner    (1001) docker     (123)    10383 2023-05-01 16:00:37.000000 ape-vyper-0.6.5/tests/test_compiler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 19:07:42.059631 ape-vyper-0.6.6/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 19:07:42.055631 ape-vyper-0.6.6/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 19:07:42.055631 ape-vyper-0.6.6/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      703 2023-05-18 19:06:44.000000 ape-vyper-0.6.6/.github/ISSUE_TEMPLATE/bug.md
+-rw-r--r--   0 runner    (1001) docker     (123)      668 2023-05-18 19:06:44.000000 ape-vyper-0.6.6/.github/ISSUE_TEMPLATE/feature.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-05-18 19:06:44.000000 ape-vyper-0.6.6/.github/ISSUE_TEMPLATE/work-item.md
+-rw-r--r--   0 runner    (1001) docker     (123)      474 2023-05-18 19:06:44.000000 ape-vyper-0.6.6/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      651 2023-05-18 19:06:44.000000 ape-vyper-0.6.6/.github/release-drafter.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 19:07:42.059631 ape-vyper-0.6.6/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      686 2023-05-18 19:06:44.000000 ape-vyper-0.6.6/.github/workflows/commitlint.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-05-18 19:06:44.000000 ape-vyper-0.6.6/.github/workflows/draft.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      616 2023-05-18 19:06:44.000000 ape-vyper-0.6.6/.github/workflows/prtitle.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-05-18 19:06:44.000000 ape-vyper-0.6.6/.github/workflows/publish.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3402 2023-05-18 19:06:44.000000 ape-vyper-0.6.6/.github/workflows/test.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1719 2023-05-18 19:06:44.000000 ape-vyper-0.6.6/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-18 19:06:44.000000 ape-vyper-0.6.6/.mdformat.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      796 2023-05-18 19:06:44.000000 ape-vyper-0.6.6/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-05-18 19:06:44.000000 ape-vyper-0.6.6/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11342 2023-05-18 19:06:44.000000 ape-vyper-0.6.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2782 2023-05-18 19:07:42.059631 ape-vyper-0.6.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1873 2023-05-18 19:06:44.000000 ape-vyper-0.6.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 19:07:42.059631 ape-vyper-0.6.6/ape_vyper/
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-05-18 19:06:44.000000 ape-vyper-0.6.6/ape_vyper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27393 2023-05-18 19:06:44.000000 ape-vyper-0.6.6/ape_vyper/compiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3818 2023-05-18 19:06:44.000000 ape-vyper-0.6.6/ape_vyper/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-18 19:07:41.000000 ape-vyper-0.6.6/ape_vyper/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 19:07:42.059631 ape-vyper-0.6.6/ape_vyper.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2782 2023-05-18 19:07:41.000000 ape-vyper-0.6.6/ape_vyper.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1666 2023-05-18 19:07:42.000000 ape-vyper-0.6.6/ape_vyper.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 19:07:41.000000 ape-vyper-0.6.6/ape_vyper.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 19:07:41.000000 ape-vyper-0.6.6/ape_vyper.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      591 2023-05-18 19:07:41.000000 ape-vyper-0.6.6/ape_vyper.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-18 19:07:41.000000 ape-vyper-0.6.6/ape_vyper.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      943 2023-05-18 19:06:44.000000 ape-vyper-0.6.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-05-18 19:07:42.059631 ape-vyper-0.6.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3045 2023-05-18 19:06:44.000000 ape-vyper-0.6.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 19:07:42.059631 ape-vyper-0.6.6/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 19:07:42.055631 ape-vyper-0.6.6/tests/ExampleDependency/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 19:07:42.059631 ape-vyper-0.6.6/tests/ExampleDependency/contracts/
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-18 19:06:44.000000 ape-vyper-0.6.6/tests/ExampleDependency/contracts/Dependency.vy
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 19:06:44.000000 ape-vyper-0.6.6/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      420 2023-05-18 19:06:44.000000 ape-vyper-0.6.6/tests/ape-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2936 2023-05-18 19:06:44.000000 ape-vyper-0.6.6/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 19:07:42.055631 ape-vyper-0.6.6/tests/contracts/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 19:07:42.059631 ape-vyper-0.6.6/tests/contracts/failing_contracts/
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-05-18 19:06:44.000000 ape-vyper-0.6.6/tests/contracts/failing_contracts/contract_undeclared_variable.vy
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-18 19:06:44.000000 ape-vyper-0.6.6/tests/contracts/failing_contracts/contract_unknown_pragma.vy
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 19:07:42.059631 ape-vyper-0.6.6/tests/contracts/passing_contracts/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 19:07:42.059631 ape-vyper-0.6.6/tests/contracts/passing_contracts/DirectoryWithExtension.vy/
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-05-18 19:06:44.000000 ape-vyper-0.6.6/tests/contracts/passing_contracts/DirectoryWithExtension.vy/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3088 2023-05-18 19:06:44.000000 ape-vyper-0.6.6/tests/contracts/passing_contracts/contract.vy
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-18 19:06:44.000000 ape-vyper-0.6.6/tests/contracts/passing_contracts/contract_no_pragma.vy
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-05-18 19:06:44.000000 ape-vyper-0.6.6/tests/contracts/passing_contracts/contract_with_dev_messages.vy
+-rw-r--r--   0 runner    (1001) docker     (123)     5231 2023-05-18 19:06:44.000000 ape-vyper-0.6.6/tests/contracts/passing_contracts/erc20.vy
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 19:07:42.059631 ape-vyper-0.6.6/tests/contracts/passing_contracts/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-18 19:06:44.000000 ape-vyper-0.6.6/tests/contracts/passing_contracts/interfaces/IFace.vy
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-18 19:06:44.000000 ape-vyper-0.6.6/tests/contracts/passing_contracts/interfaces/IFace2.vy
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-05-18 19:06:44.000000 ape-vyper-0.6.6/tests/contracts/passing_contracts/interfaces/IRegistry.vy
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-18 19:06:44.000000 ape-vyper-0.6.6/tests/contracts/passing_contracts/older_version.vy
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-05-18 19:06:44.000000 ape-vyper-0.6.6/tests/contracts/passing_contracts/registry.vy
+-rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-05-18 19:06:44.000000 ape-vyper-0.6.6/tests/contracts/passing_contracts/traceback_contract.vy
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-05-18 19:06:44.000000 ape-vyper-0.6.6/tests/contracts/passing_contracts/use_iface.vy
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-05-18 19:06:44.000000 ape-vyper-0.6.6/tests/contracts/passing_contracts/use_iface2.vy
+-rw-r--r--   0 runner    (1001) docker     (123)    12196 2023-05-18 19:06:44.000000 ape-vyper-0.6.6/tests/test_compiler.py
```

### Comparing `ape-vyper-0.6.5/.github/ISSUE_TEMPLATE/bug.md` & `ape-vyper-0.6.6/.github/ISSUE_TEMPLATE/bug.md`

 * *Files identical despite different names*

### Comparing `ape-vyper-0.6.5/.github/ISSUE_TEMPLATE/feature.md` & `ape-vyper-0.6.6/.github/ISSUE_TEMPLATE/feature.md`

 * *Files identical despite different names*

### Comparing `ape-vyper-0.6.5/.github/ISSUE_TEMPLATE/work-item.md` & `ape-vyper-0.6.6/.github/ISSUE_TEMPLATE/work-item.md`

 * *Files identical despite different names*

### Comparing `ape-vyper-0.6.5/.github/release-drafter.yml` & `ape-vyper-0.6.6/.github/release-drafter.yml`

 * *Files identical despite different names*

### Comparing `ape-vyper-0.6.5/.github/workflows/commitlint.yaml` & `ape-vyper-0.6.6/.github/workflows/commitlint.yaml`

 * *Files identical despite different names*

### Comparing `ape-vyper-0.6.5/.github/workflows/prtitle.yaml` & `ape-vyper-0.6.6/.github/workflows/prtitle.yaml`

 * *Files identical despite different names*

### Comparing `ape-vyper-0.6.5/.github/workflows/publish.yaml` & `ape-vyper-0.6.6/.github/workflows/publish.yaml`

 * *Files identical despite different names*

### Comparing `ape-vyper-0.6.5/.github/workflows/test.yaml` & `ape-vyper-0.6.6/.github/workflows/test.yaml`

 * *Files 26% similar despite different names*

```diff
@@ -64,22 +64,48 @@
         runs-on: ${{ matrix.os }}
 
         strategy:
             matrix:
                 os: [ubuntu-latest, macos-latest]   # eventually add `windows-latest`
                 python-version: [3.8, 3.9, "3.10"]
 
+        env:
+          GETH_VERSION: 1.11.5
+
         steps:
         - uses: actions/checkout@v3
 
         - name: Setup Python
           uses: actions/setup-python@v4
           with:
               python-version: ${{ matrix.python-version }}
 
+        - name: Setup Go
+          uses: actions/setup-go@v4
+          with:
+            go-version: '^1.20.1'
+
+        - name: Cache Geth
+          id: cache-geth
+          uses: actions/cache@v3
+          with:
+            path: $HOME/.local/bin
+            key: ${{ runner.os }}-geth-${{ env.GETH_VERSION }}
+
+        - name: Install Geth
+          if: steps.cache-geth.outputs.cache-hit != 'true'
+          run: |
+            mkdir -p $HOME/.local/bin
+            wget -O geth.tar.gz "https://github.com/ethereum/go-ethereum/archive/v$GETH_VERSION.tar.gz"
+            tar -zxvf geth.tar.gz
+            cd go-ethereum-$GETH_VERSION
+            make geth
+            cp ./build/bin/geth /usr/local/bin
+            geth version
+
         - name: Install Dependencies
           run: |
             python -m pip install --upgrade pip
             pip install .[test]
 
         - name: Run Tests
           run: pytest -m "not fuzzing" -n 0 -s --cov
```

### Comparing `ape-vyper-0.6.5/.gitignore` & `ape-vyper-0.6.6/.gitignore`

 * *Files identical despite different names*

### Comparing `ape-vyper-0.6.5/.pre-commit-config.yaml` & `ape-vyper-0.6.6/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `ape-vyper-0.6.5/CONTRIBUTING.md` & `ape-vyper-0.6.6/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `ape-vyper-0.6.5/LICENSE` & `ape-vyper-0.6.6/LICENSE`

 * *Files identical despite different names*

### Comparing `ape-vyper-0.6.5/PKG-INFO` & `ape-vyper-0.6.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ape-vyper
-Version: 0.6.5
+Version: 0.6.6
 Summary: Plugin for Ape Ethereum Framework for compiling Vyper contracts
 Home-page: https://github.com/ApeWorX/ape-vyper
 Author: ApeWorX Ltd.
 Author-email: admin@apeworx.io
 License: Apache-2.0
 Keywords: ethereum
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `ape-vyper-0.6.5/README.md` & `ape-vyper-0.6.6/README.md`

 * *Files identical despite different names*

### Comparing `ape-vyper-0.6.5/ape_vyper/compiler.py` & `ape-vyper-0.6.6/ape_vyper/compiler.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,33 +1,39 @@
 import os
 import re
 import shutil
 from pathlib import Path
-from typing import Any, Dict, List, Optional, Set, Tuple, Union, cast
+from typing import Any, Dict, Iterator, List, Optional, Set, Tuple, Union, cast
 
 import vvm  # type: ignore
 from ape.api import PluginConfig
 from ape.api.compiler import CompilerAPI
 from ape.exceptions import ContractLogicError
-from ape.types import ContractType
+from ape.types import ContractType, SourceTraceback, TraceFrame
 from ape.utils import cached_property, get_relative_path
 from eth_utils import is_0x_prefixed
-from ethpm_types import ASTNode, PackageManifest, PCMap
+from ethpm_types import ASTNode, HexBytes, PackageManifest, PCMap
+from ethpm_types.ast import ASTClassification
 from ethpm_types.contract_type import SourceMap
+from ethpm_types.source import ContractSource, Function
+from evm_trace.enums import CALL_OPCODES
 from semantic_version import NpmSpec, Version  # type: ignore
 from vvm.exceptions import VyperError  # type: ignore
 
 from ape_vyper.exceptions import (
     RUNTIME_ERROR_MAP,
     RuntimeErrorType,
     VyperCompileError,
     VyperInstallError,
 )
 
 DEV_MSG_PATTERN = re.compile(r"#\s*(dev:.+)")
+_RETURN_OPCODES = ("RETURN", "REVERT", "STOP")
+_FUNCTION_DEF = "FunctionDef"
+_FUNCTION_AST_TYPES = (_FUNCTION_DEF, "Name", "arguments")
 
 
 class VyperConfig(PluginConfig):
     evm_version: Optional[str] = None
 
     import_remapping: List[str] = []
     """
@@ -238,22 +244,30 @@
                     base_path=base_path,
                     vyper_version=vyper_version,
                     vyper_binary=vyper_binary,
                 )
             except VyperError as err:
                 raise VyperCompileError(err) from err
 
+            def classify_ast(_node: ASTNode):
+                if _node.ast_type in _FUNCTION_AST_TYPES:
+                    _node.classification = ASTClassification.FUNCTION
+
+                for child in _node.children:
+                    classify_ast(child)
+
             for source_id, output_items in result["contracts"].items():
                 content = {
                     i + 1: ln
                     for i, ln in enumerate((base_path / source_id).read_text().splitlines())
                 }
                 for name, output in output_items.items():
                     # De-compress source map to get PC POS map.
                     ast = ASTNode.parse_obj(result["sources"][source_id]["ast"])
+                    classify_ast(ast)
 
                     # Track function offsets.
                     function_offsets = []
                     for node in ast.children:
                         lineno = node.lineno
 
                         # NOTE: Constructor is handled elsewhere.
@@ -484,14 +498,154 @@
                 txn=err.txn, trace=err.trace, contract_address=err.contract_address
             )
 
         else:
             # Not a builtin compiler error; cannot enrich.
             return err
 
+    def trace_source(
+        self, contract_type: ContractType, trace: Iterator[TraceFrame], calldata: HexBytes
+    ) -> SourceTraceback:
+        source_contract_type = self.project_manager._create_contract_source(contract_type)
+        if not source_contract_type:
+            return SourceTraceback.parse_obj([])
+
+        return self._get_traceback(source_contract_type, trace, calldata)
+
+    def _get_traceback(
+        self, contract_src: ContractSource, trace: Iterator[TraceFrame], calldata: HexBytes
+    ) -> SourceTraceback:
+        traceback = SourceTraceback.parse_obj([])
+        function = None
+
+        for frame in trace:
+            if frame.op in CALL_OPCODES:
+                called_contract, sub_calldata = self._create_contract_from_call(frame)
+                if called_contract:
+                    ext = Path(called_contract.source_id).suffix
+                    if not ext.endswith(".vy"):
+                        # Not a Vyper contract!
+                        compiler = self.compiler_manager.registered_compilers[ext]
+                        try:
+                            sub_trace = compiler.trace_source(
+                                called_contract.contract_type, trace, sub_calldata
+                            )
+                            traceback.extend(sub_trace)
+                        except NotImplementedError:
+                            # Compiler not supported. Fast forward out of this call.
+                            for fr in trace:
+                                if fr.op == "RETURN":
+                                    break
+
+                    else:
+                        sub_trace = self._get_traceback(called_contract, trace, sub_calldata)
+                        traceback.extend(sub_trace)
+
+                else:
+                    # Contract not found. Fast forward out of this call.
+                    for fr in trace:
+                        if fr.op == "RETURN":
+                            break
+
+            elif frame.op in _RETURN_OPCODES:
+                if frame.op == "RETURN" and function:
+                    return_ast_result = [x for x in function.ast.children if x.ast_type == "Return"]
+                    if return_ast_result:
+                        # Ensure return statement added.
+                        # Sometimes it is missing from the PCMap otherwise.
+                        return_ast = return_ast_result[-1]
+                        location = return_ast.line_numbers
+                        start = traceback.last.end_lineno + 1
+                        traceback.last.extend(location, ws_start=start)
+
+                # Completed!
+                return traceback
+
+            if "PUSH" in frame.op and frame.pc in contract_src.pcmap:
+                # Check if next op is SSTORE to properly use AST from push op.
+                next_frame = next(trace, None)
+                if next_frame and next_frame.op == "SSTORE":
+                    push_location = tuple(contract_src.pcmap[frame.pc]["location"])  # type: ignore
+                    pcmap = PCMap.parse_obj({next_frame.pc: {"location": push_location}})
+                else:
+                    pcmap = contract_src.pcmap
+
+                if next_frame:
+                    frame = next_frame
+
+            else:
+                pcmap = contract_src.pcmap
+
+            if frame.pc not in pcmap:
+                continue
+
+            method_id = HexBytes(calldata[:4])
+            location = cast(Tuple[int, int, int, int], tuple(pcmap[frame.pc].get("location") or []))
+            dev = str(pcmap[frame.pc].get("dev", "")).replace("dev: ", "")
+            if not location and dev in [m.value for m in RuntimeErrorType]:
+                error_type = RuntimeErrorType(dev)
+                if error_type != RuntimeErrorType.NONPAYABLE_CHECK and traceback.last is not None:
+                    # If the error type is not the non-payable check,
+                    # it happened in the last method.
+                    name = traceback.last.name
+
+                elif method_id in contract_src.contract_type.methods:
+                    # For non-payable checks, they should hit here.
+                    method_checked = contract_src.contract_type.methods[method_id]
+                    name = method_checked.name
+
+                else:
+                    # Not sure if possible to get here.
+                    name = error_type.name.lower()
+
+                if (
+                    error_type == RuntimeErrorType.NONPAYABLE_CHECK
+                    and traceback.last is not None
+                    and traceback.last.closure.name == name
+                ):
+                    # Prevent weird duplicate non-payable check..
+                    # TODO: Find a better way to do this at compile time.
+                    continue
+
+                # Empty source (is builtin)
+                stmt_type = f"dev: {error_type.value}"
+                traceback.add_builtin_jump(name, stmt_type, self.name)
+                continue
+
+            elif not location:
+                # Unknown.
+                continue
+
+            function = contract_src.lookup_function(location, method_id=method_id)
+            if not function:
+                continue
+
+            if (
+                not traceback.last
+                or traceback.last.closure.name != function.name
+                or not isinstance(traceback.last.closure, Function)
+            ):
+                depth = (
+                    frame.depth + 1
+                    if traceback.last and traceback.last.depth == frame.depth
+                    else frame.depth
+                )
+                traceback.add_jump(
+                    location,
+                    function,
+                    depth,
+                    source_path=contract_src.source_path,
+                )
+            else:
+                traceback.extend_last(location)
+
+        # Never actually hits this return.
+        # See `Completed!` comment above.
+        return traceback
+
 
 def _safe_append(data: Dict, version: Union[Version, NpmSpec], paths: Union[Path, Set]):
     if isinstance(paths, Path):
         paths = {paths}
     if version in data:
         data[version] = data[version].union(paths)
     else:
```

### Comparing `ape-vyper-0.6.5/ape_vyper/exceptions.py` & `ape-vyper-0.6.6/ape_vyper/exceptions.py`

 * *Files identical despite different names*

### Comparing `ape-vyper-0.6.5/ape_vyper.egg-info/PKG-INFO` & `ape-vyper-0.6.6/ape_vyper.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ape-vyper
-Version: 0.6.5
+Version: 0.6.6
 Summary: Plugin for Ape Ethereum Framework for compiling Vyper contracts
 Home-page: https://github.com/ApeWorX/ape-vyper
 Author: ApeWorX Ltd.
 Author-email: admin@apeworx.io
 License: Apache-2.0
 Keywords: ethereum
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `ape-vyper-0.6.5/ape_vyper.egg-info/SOURCES.txt` & `ape-vyper-0.6.6/ape_vyper.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -35,12 +35,15 @@
 tests/contracts/failing_contracts/contract_undeclared_variable.vy
 tests/contracts/failing_contracts/contract_unknown_pragma.vy
 tests/contracts/passing_contracts/contract.vy
 tests/contracts/passing_contracts/contract_no_pragma.vy
 tests/contracts/passing_contracts/contract_with_dev_messages.vy
 tests/contracts/passing_contracts/erc20.vy
 tests/contracts/passing_contracts/older_version.vy
+tests/contracts/passing_contracts/registry.vy
+tests/contracts/passing_contracts/traceback_contract.vy
 tests/contracts/passing_contracts/use_iface.vy
 tests/contracts/passing_contracts/use_iface2.vy
 tests/contracts/passing_contracts/DirectoryWithExtension.vy/README.md
 tests/contracts/passing_contracts/interfaces/IFace.vy
-tests/contracts/passing_contracts/interfaces/IFace2.vy
+tests/contracts/passing_contracts/interfaces/IFace2.vy
+tests/contracts/passing_contracts/interfaces/IRegistry.vy
```

### Comparing `ape-vyper-0.6.5/ape_vyper.egg-info/requires.txt` & `ape-vyper-0.6.6/ape_vyper.egg-info/requires.txt`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-eth-ape<0.7,>=0.6.8
-ethpm-types>=0.4.4
+eth-ape<0.7,>=0.6.9
+ethpm-types
 tqdm
 vvm<0.2,>=0.1.0
 
 [dev]
 pytest>=6.0
 pytest-xdist
 pytest-cov
```

### Comparing `ape-vyper-0.6.5/pyproject.toml` & `ape-vyper-0.6.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ape-vyper-0.6.5/setup.py` & `ape-vyper-0.6.6/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -53,16 +53,16 @@
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="ApeWorX Ltd.",
     author_email="admin@apeworx.io",
     url="https://github.com/ApeWorX/ape-vyper",
     include_package_data=True,
     install_requires=[
-        "eth-ape>=0.6.8,<0.7",
-        "ethpm-types>=0.4.4",
+        "eth-ape>=0.6.9,<0.7",
+        "ethpm-types",  # Use same version as eth-ape
         "tqdm",  # Use same version as eth-ape
         "vvm>=0.1.0,<0.2",
     ],
     python_requires=">=3.8,<3.11",
     extras_require=extras_require,
     py_modules=["ape_vyper"],
     license="Apache-2.0",
```

### Comparing `ape-vyper-0.6.5/tests/conftest.py` & `ape-vyper-0.6.6/tests/conftest.py`

 * *Files 11% similar despite different names*

```diff
@@ -85,7 +85,33 @@
         shutil.rmtree(cache)
 
     copy_tree(project_source_dir.as_posix(), project_dest_dir.as_posix())
     with config.using_project(project_dest_dir) as project:
         yield project
         if project.local_project._cache_folder.is_dir():
             shutil.rmtree(project.local_project._cache_folder)
+
+
+@pytest.fixture
+def geth_provider():
+    if not ape.networks.active_provider or ape.networks.provider.name != "geth":
+        with ape.networks.ethereum.local.use_provider(
+            "geth", provider_settings={"uri": "http://127.0.0.1:5550"}
+        ) as provider:
+            yield provider
+    else:
+        yield ape.networks.provider
+
+
+@pytest.fixture
+def account():
+    return ape.accounts.test_accounts[0]
+
+
+@pytest.fixture
+def registry(geth_provider, account, project):
+    return account.deploy(project.registry)
+
+
+@pytest.fixture
+def contract(registry, account, project):
+    return account.deploy(project.traceback_contract, registry)
```

### Comparing `ape-vyper-0.6.5/tests/contracts/passing_contracts/contract.vy` & `ape-vyper-0.6.6/tests/contracts/passing_contracts/contract.vy`

 * *Files identical despite different names*

### Comparing `ape-vyper-0.6.5/tests/contracts/passing_contracts/erc20.vy` & `ape-vyper-0.6.6/tests/contracts/passing_contracts/erc20.vy`

 * *Files identical despite different names*

### Comparing `ape-vyper-0.6.5/tests/test_compiler.py` & `ape-vyper-0.6.6/tests/test_compiler.py`

 * *Files 13% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import pytest
 from ape.exceptions import ContractLogicError
 from semantic_version import Version  # type: ignore
 from vvm import compile_source  # type: ignore
 from vvm.exceptions import VyperError  # type: ignore
 
 from ape_vyper.compiler import RuntimeErrorType
-from ape_vyper.exceptions import NonPayableError, VyperCompileError, VyperInstallError
+from ape_vyper.exceptions import IntegerOverflowError, VyperCompileError, VyperInstallError
 
 BASE_CONTRACTS_PATH = Path(__file__).parent / "contracts"
 PASSING_BASE = BASE_CONTRACTS_PATH / "passing_contracts"
 FAILING_BASE = BASE_CONTRACTS_PATH / "failing_contracts"
 
 # Currently, this is the only version specified from a pragma spec
 OLDER_VERSION_FROM_PRAGMA = Version("0.2.8")
@@ -20,24 +20,14 @@
 
 
 @pytest.fixture
 def dev_revert_source():
     return PASSING_BASE / "contract_with_dev_messages.vy"
 
 
-@pytest.fixture
-def contract_logic_error():
-    err = ContractLogicError()
-
-    # Inject cached PC message so no need to have tracing provider.
-    err.__dict__["dev_message"] = f"dev: {RuntimeErrorType.NONPAYABLE_CHECK.value}"
-
-    return err
-
-
 def contract_test_cases(passing: bool) -> List[str]:
     """
     Returns test-case names for outputting nicely with pytest.
     """
     suffix = "passing_contracts" if passing else "failing_contracts"
     return [p.name for p in (BASE_CONTRACTS_PATH / suffix).glob("*.vy") if p.is_file()]
 
@@ -93,44 +83,66 @@
             continue
 
         sources = ", ".join([p.name for p in actual[version]])
         fail_message = f"Unexpected version '{version}' with sources: {sources}"
         pytest.fail(fail_message)
 
     assert len(actual[OLDER_VERSION_FROM_PRAGMA]) == 1
-    assert len(actual[VERSION_FROM_PRAGMA]) == 6
+    assert len(actual[VERSION_FROM_PRAGMA]) == 8
     assert actual[OLDER_VERSION_FROM_PRAGMA] == {project.contracts_folder / "older_version.vy"}
-    assert actual[VERSION_FROM_PRAGMA] == {
-        project.contracts_folder / "contract.vy",
-        project.contracts_folder / "contract_no_pragma.vy",
-        project.contracts_folder / "contract_with_dev_messages.vy",
-        project.contracts_folder / "use_iface.vy",
-        project.contracts_folder / "use_iface2.vy",
-        project.contracts_folder / "erc20.vy",
-    }
+
+    expected = (
+        "contract.vy",
+        "contract_no_pragma.vy",
+        "contract_with_dev_messages.vy",
+        "erc20.vy",
+        "registry.vy",
+        "traceback_contract.vy",
+        "use_iface.vy",
+        "use_iface2.vy",
+    )
+    names = [x.name for x in actual[VERSION_FROM_PRAGMA]]
+    failures = []
+    missing = []
+    for ex in expected:
+        if ex not in names:
+            missing.append(ex)
+
+    if missing:
+        failures.append(f"Missing contracts: {','.join(missing)}")
+
+    extra = []
+    for ac in actual[VERSION_FROM_PRAGMA]:
+        if ac.name not in expected:
+            extra.append(ac.name)
+
+    if extra:
+        failures.append(f"Extra contracts: {', '.join(extra)}")
+
+    assert not failures, "\n".join(failures)
 
 
 def test_compiler_data_in_manifest(project):
     _ = project.contracts
     manifest = project.extract_manifest()
     assert len(manifest.compilers) == 2, manifest.compilers
 
-    vyper_034 = [c for c in manifest.compilers if str(c.version) == str(VERSION_FROM_PRAGMA)][0]
+    vyper_037 = [c for c in manifest.compilers if str(c.version) == str(VERSION_FROM_PRAGMA)][0]
     vyper_028 = [c for c in manifest.compilers if str(c.version) == str(OLDER_VERSION_FROM_PRAGMA)][
         0
     ]
 
-    for compiler in (vyper_028, vyper_034):
+    for compiler in (vyper_028, vyper_037):
         assert compiler.name == "vyper"
 
-    assert len(vyper_034.contractTypes) == 6
+    assert len(vyper_037.contractTypes) == 8
     assert len(vyper_028.contractTypes) == 1
-    assert "contract" in vyper_034.contractTypes
+    assert "contract" in vyper_037.contractTypes
     assert "older_version" in vyper_028.contractTypes
-    for compiler in (vyper_034, vyper_028):
+    for compiler in (vyper_037, vyper_028):
         assert compiler.settings["evmVersion"] == "constantinople"
         assert compiler.settings["optimize"] is True
 
 
 def test_compile_parse_dev_messages(compiler, dev_revert_source):
     """
     Test parsing of dev messages in a contract. These follow the form of "#dev: ...".
@@ -177,15 +189,15 @@
     from `compile_src()` which includes the uncompressed source map data.
     """
 
     path = PASSING_BASE / "contract.vy"
     result = compiler.compile([path], base_path=PASSING_BASE)[0]
     actual = result.pcmap.__root__
     code = path.read_text()
-    compile_result = compile_source(code)["<stdin>"]
+    compile_result = compile_source(code, vyper_version="0.3.7")["<stdin>"]
     src_map = compile_result["source_map"]
     lines = code.splitlines()
 
     # Use the old-fashioned way of gathering PCMap to ensure our creative way works
     expected = {pc: {"location": ln} for pc, ln in src_map["pc_pos_map"].items()}
     missing_pcs = []
     empty_locs = []
@@ -269,10 +281,62 @@
     # Verify index out of range checks
     range_checks = _all(RuntimeErrorType.INDEX_OUT_OF_RANGE)
     range_no = line("return self.dynArray[idx]")
     assert len(range_checks) == 1
     assert range_checks[0]["location"] == [range_no, 11, range_no, 24]
 
 
-def test_enrich_error(contract_logic_error, compiler):
-    actual = compiler.enrich_error(contract_logic_error)
-    assert isinstance(actual, NonPayableError)
+def test_enrich_error(compiler, geth_provider, contract, account):
+    int_max = 2**256 - 1
+    with pytest.raises(IntegerOverflowError):
+        contract.addBalance(int_max, sender=account)
+
+
+def test_trace_source(account, geth_provider, project, contract):
+    receipt = contract.addBalance(123, sender=account)
+    actual = receipt.source_traceback
+    base_folder = project.contracts_folder
+    expected = rf"""
+Traceback (most recent call last)
+  File {base_folder}/traceback_contract.vy, in addBalance
+       27     # Comments in the middle (is a test)
+       28
+       29     for i in [1, 2, 3, 4, 5]:
+       30         if i != num:
+       31             continue
+       32
+  -->  33     return self._balance
+""".strip()
+    assert str(actual) == expected
+
+
+def test_trace_err_source(account, geth_provider, project, contract):
+    txn = contract.addBalance_f.as_transaction(123)
+    try:
+        account.call(txn)
+    except ContractLogicError:
+        pass
+
+    receipt = geth_provider.get_receipt(txn.txn_hash.hex())
+    actual = receipt.source_traceback
+    base_folder = project.contracts_folder
+    expected = rf"""
+Traceback (most recent call last)
+  File {base_folder}/traceback_contract.vy, in addBalance_f
+       44     # Run some loops.
+       45     for i in [1, 2, 3, 4, 5]:
+       46         if i == num:
+       47             break
+       48
+       49     # Fail in the middle (is test)
+       50     # Fails because was already set above.
+  -->  51     self.registry.register_f(msg.sender)
+       52
+       53     for i in [1, 2, 3, 4, 5]:
+       54         if i != num:
+       55             continue
+
+  File {base_folder}/registry.vy, in register_f
+  -->  12     assert self.addr != addr, "doubling."
+       13     self.addr = addr
+    """.strip()
+    assert str(actual) == expected
```

