# Comparing `tmp/ape-solidity-0.6.3.tar.gz` & `tmp/ape-solidity-0.6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ape-solidity-0.6.3.tar", last modified: Thu Apr 13 22:00:18 2023, max compression
+gzip compressed data, was "ape-solidity-0.6.4.tar", last modified: Thu May 18 15:22:34 2023, max compression
```

## Comparing `ape-solidity-0.6.3.tar` & `ape-solidity-0.6.4.tar`

### file list

```diff
@@ -1,111 +1,123 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 22:00:18.297256 ape-solidity-0.6.3/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 22:00:18.289256 ape-solidity-0.6.3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 22:00:18.289256 ape-solidity-0.6.3/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      703 2023-04-13 21:59:31.000000 ape-solidity-0.6.3/.github/ISSUE_TEMPLATE/bug.md
--rw-r--r--   0 runner    (1001) docker     (123)      668 2023-04-13 21:59:31.000000 ape-solidity-0.6.3/.github/ISSUE_TEMPLATE/feature.md
--rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-04-13 21:59:31.000000 ape-solidity-0.6.3/.github/ISSUE_TEMPLATE/work-item.md
--rw-r--r--   0 runner    (1001) docker     (123)      474 2023-04-13 21:59:31.000000 ape-solidity-0.6.3/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (123)      651 2023-04-13 21:59:31.000000 ape-solidity-0.6.3/.github/release-drafter.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 22:00:18.289256 ape-solidity-0.6.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      618 2023-04-13 21:59:31.000000 ape-solidity-0.6.3/.github/workflows/codeql.yml
--rw-r--r--   0 runner    (1001) docker     (123)      368 2023-04-13 21:59:31.000000 ape-solidity-0.6.3/.github/workflows/draft.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      551 2023-04-13 21:59:31.000000 ape-solidity-0.6.3/.github/workflows/prtitle.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      620 2023-04-13 21:59:31.000000 ape-solidity-0.6.3/.github/workflows/publish.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      709 2023-04-13 21:59:31.000000 ape-solidity-0.6.3/.github/workflows/stale-prs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2506 2023-04-13 21:59:31.000000 ape-solidity-0.6.3/.github/workflows/test.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1757 2023-04-13 21:59:31.000000 ape-solidity-0.6.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-13 21:59:31.000000 ape-solidity-0.6.3/.mdformat.toml
--rw-r--r--   0 runner    (1001) docker     (123)      805 2023-04-13 21:59:31.000000 ape-solidity-0.6.3/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2175 2023-04-13 21:59:31.000000 ape-solidity-0.6.3/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)    11342 2023-04-13 21:59:31.000000 ape-solidity-0.6.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4874 2023-04-13 22:00:18.297256 ape-solidity-0.6.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3002 2023-04-13 21:59:31.000000 ape-solidity-0.6.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 22:00:18.289256 ape-solidity-0.6.3/ape_solidity/
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-04-13 21:59:31.000000 ape-solidity-0.6.3/ape_solidity/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6285 2023-04-13 21:59:31.000000 ape-solidity-0.6.3/ape_solidity/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    28796 2023-04-13 21:59:31.000000 ape-solidity-0.6.3/ape_solidity/compiler.py
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-04-13 21:59:31.000000 ape-solidity-0.6.3/ape_solidity/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 21:59:31.000000 ape-solidity-0.6.3/ape_solidity/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-13 22:00:18.000000 ape-solidity-0.6.3/ape_solidity/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 22:00:18.293256 ape-solidity-0.6.3/ape_solidity.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4874 2023-04-13 22:00:18.000000 ape-solidity-0.6.3/ape_solidity.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3145 2023-04-13 22:00:18.000000 ape-solidity-0.6.3/ape_solidity.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 22:00:18.000000 ape-solidity-0.6.3/ape_solidity.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 22:00:18.000000 ape-solidity-0.6.3/ape_solidity.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      813 2023-04-13 22:00:18.000000 ape-solidity-0.6.3/ape_solidity.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-13 22:00:18.000000 ape-solidity-0.6.3/ape_solidity.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      975 2023-04-13 21:59:31.000000 ape-solidity-0.6.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-04-13 22:00:18.297256 ape-solidity-0.6.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3353 2023-04-13 21:59:31.000000 ape-solidity-0.6.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 22:00:18.293256 ape-solidity-0.6.3/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 22:00:18.293256 ape-solidity-0.6.3/tests/BrownieProject/
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-04-13 21:59:31.000000 ape-solidity-0.6.3/tests/BrownieProject/brownie-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 22:00:18.293256 ape-solidity-0.6.3/tests/BrownieProject/contracts/
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-04-13 21:59:31.000000 ape-solidity-0.6.3/tests/BrownieProject/contracts/BrownieContract.sol
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 22:00:18.293256 ape-solidity-0.6.3/tests/BrownieStyleDependency/
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-13 21:59:31.000000 ape-solidity-0.6.3/tests/BrownieStyleDependency/ape-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 22:00:18.293256 ape-solidity-0.6.3/tests/BrownieStyleDependency/contracts/
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-04-13 21:59:31.000000 ape-solidity-0.6.3/tests/BrownieStyleDependency/contracts/BrownieStyleDependency.sol
--rw-r--r--   0 runner    (1001) docker     (123)      251 2023-04-13 21:59:31.000000 ape-solidity-0.6.3/tests/BrownieStyleDependency/contracts/FailingContract.sol
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 22:00:18.293256 ape-solidity-0.6.3/tests/Dependency/
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-04-13 21:59:31.000000 ape-solidity-0.6.3/tests/Dependency/ape-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 22:00:18.293256 ape-solidity-0.6.3/tests/Dependency/contracts/
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-04-13 21:59:31.000000 ape-solidity-0.6.3/tests/Dependency/contracts/Dependency.sol
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-04-13 21:59:31.000000 ape-solidity-0.6.3/tests/Dependency/contracts/OlderDependency.sol
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 22:00:18.293256 ape-solidity-0.6.3/tests/Dependency/contracts/subfolder/
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-04-13 21:59:31.000000 ape-solidity-0.6.3/tests/Dependency/contracts/subfolder/InDependencySubfolder.sol
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 22:00:18.293256 ape-solidity-0.6.3/tests/Dependency/contracts/subfolder_with_imports/
--rw-r--r--   0 runner    (1001) docker     (123)      256 2023-04-13 21:59:31.000000 ape-solidity-0.6.3/tests/Dependency/contracts/subfolder_with_imports/InDependencySubfolderWithImports.sol
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 22:00:18.293256 ape-solidity-0.6.3/tests/DependencyOfDependency/
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-04-13 21:59:31.000000 ape-solidity-0.6.3/tests/DependencyOfDependency/ape-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 22:00:18.293256 ape-solidity-0.6.3/tests/DependencyOfDependency/contracts/
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-04-13 21:59:31.000000 ape-solidity-0.6.3/tests/DependencyOfDependency/contracts/DependencyOfDependency.sol
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 22:00:18.293256 ape-solidity-0.6.3/tests/ProjectWithinProject/
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-04-13 21:59:31.000000 ape-solidity-0.6.3/tests/ProjectWithinProject/ape-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 22:00:18.293256 ape-solidity-0.6.3/tests/ProjectWithinProject/contracts/
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-04-13 21:59:31.000000 ape-solidity-0.6.3/tests/ProjectWithinProject/contracts/Contract.sol
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 22:00:18.293256 ape-solidity-0.6.3/tests/VersionSpecifiedInConfig/
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-13 21:59:31.000000 ape-solidity-0.6.3/tests/VersionSpecifiedInConfig/ape-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 22:00:18.293256 ape-solidity-0.6.3/tests/VersionSpecifiedInConfig/contracts/
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-04-13 21:59:31.000000 ape-solidity-0.6.3/tests/VersionSpecifiedInConfig/contracts/VersionSpecifiedInConfig.sol
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 21:59:31.000000 ape-solidity-0.6.3/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-04-13 21:59:31.000000 ape-solidity-0.6.3/tests/ape-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3172 2023-04-13 21:59:31.000000 ape-solidity-0.6.3/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 22:00:18.297256 ape-solidity-0.6.3/tests/contracts/
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-04-13 21:59:31.000000 ape-solidity-0.6.3/tests/contracts/CircularImport1.sol
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-04-13 21:59:31.000000 ape-solidity-0.6.3/tests/contracts/CircularImport2.sol
--rw-r--r--   0 runner    (1001) docker     (123)      423 2023-04-13 21:59:31.000000 ape-solidity-0.6.3/tests/contracts/CompilesOnce.sol
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-04-13 21:59:31.000000 ape-solidity-0.6.3/tests/contracts/DifferentNameThanFile.sol
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 22:00:18.297256 ape-solidity-0.6.3/tests/contracts/DirectoryWithExtension.sol/
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-04-13 21:59:31.000000 ape-solidity-0.6.3/tests/contracts/DirectoryWithExtension.sol/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-04-13 21:59:31.000000 ape-solidity-0.6.3/tests/contracts/ExperimentalABIEncoderV2.sol
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-04-13 21:59:31.000000 ape-solidity-0.6.3/tests/contracts/HasError.sol
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-04-13 21:59:31.000000 ape-solidity-0.6.3/tests/contracts/ImportOlderDependency.sol
--rw-r--r--   0 runner    (1001) docker     (123)      391 2023-04-13 21:59:31.000000 ape-solidity-0.6.3/tests/contracts/ImportSourceWithEqualSignVersion.sol
--rw-r--r--   0 runner    (1001) docker     (123)      384 2023-04-13 21:59:31.000000 ape-solidity-0.6.3/tests/contracts/ImportSourceWithNoPrefixVersion.sol
--rw-r--r--   0 runner    (1001) docker     (123)      423 2023-04-13 21:59:31.000000 ape-solidity-0.6.3/tests/contracts/ImportingLessConstrainedVersion.sol
--rw-r--r--   0 runner    (1001) docker     (123)      682 2023-04-13 21:59:31.000000 ape-solidity-0.6.3/tests/contracts/Imports.sol
--rw-r--r--   0 runner    (1001) docker     (123)      305 2023-04-13 21:59:31.000000 ape-solidity-0.6.3/tests/contracts/IndirectlyImportingMoreConstrainedVersion.sol
--rw-r--r--   0 runner    (1001) docker     (123)      431 2023-04-13 21:59:31.000000 ape-solidity-0.6.3/tests/contracts/IndirectlyImportingMoreConstrainedVersionCompanion.sol
--rw-r--r--   0 runner    (1001) docker     (123)      474 2023-04-13 21:59:31.000000 ape-solidity-0.6.3/tests/contracts/IndirectlyImportingMoreConstrainedVersionCompanionImport.sol
--rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-04-13 21:59:31.000000 ape-solidity-0.6.3/tests/contracts/LibraryFun.sol
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-04-13 21:59:31.000000 ape-solidity-0.6.3/tests/contracts/MissingPragma.sol
--rw-r--r--   0 runner    (1001) docker     (123)      212 2023-04-13 21:59:31.000000 ape-solidity-0.6.3/tests/contracts/MultipleDefinitions.sol
--rw-r--r--   0 runner    (1001) docker     (123)      484 2023-04-13 21:59:31.000000 ape-solidity-0.6.3/tests/contracts/NumerousDefinitions.sol
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-13 21:59:31.000000 ape-solidity-0.6.3/tests/contracts/OlderVersion.sol
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-13 21:59:31.000000 ape-solidity-0.6.3/tests/contracts/RandomVyperFile.vy
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-04-13 21:59:31.000000 ape-solidity-0.6.3/tests/contracts/RangedVersion.sol
--rw-r--r--   0 runner    (1001) docker     (123)      480 2023-04-13 21:59:31.000000 ape-solidity-0.6.3/tests/contracts/SpacesInPragma.sol
--rw-r--r--   0 runner    (1001) docker     (123)      197 2023-04-13 21:59:31.000000 ape-solidity-0.6.3/tests/contracts/SpecificVersionNoPrefix.sol
--rw-r--r--   0 runner    (1001) docker     (123)      395 2023-04-13 21:59:31.000000 ape-solidity-0.6.3/tests/contracts/SpecificVersionNoPrefix2.sol
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-04-13 21:59:31.000000 ape-solidity-0.6.3/tests/contracts/SpecificVersionRange.sol
--rw-r--r--   0 runner    (1001) docker     (123)      203 2023-04-13 21:59:31.000000 ape-solidity-0.6.3/tests/contracts/SpecificVersionWithEqualSign.sol
--rw-r--r--   0 runner    (1001) docker     (123)      220 2023-04-13 21:59:31.000000 ape-solidity-0.6.3/tests/contracts/UseYearn.sol
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-13 21:59:31.000000 ape-solidity-0.6.3/tests/contracts/VagueVersion.sol
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 22:00:18.297256 ape-solidity-0.6.3/tests/contracts/subfolder/
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-04-13 21:59:31.000000 ape-solidity-0.6.3/tests/contracts/subfolder/Relativecontract.sol
--rw-r--r--   0 runner    (1001) docker     (123)      223 2023-04-13 21:59:31.000000 ape-solidity-0.6.3/tests/contracts/subfolder/UsingDependencyWithinSubFolder.sol
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 22:00:18.297256 ape-solidity-0.6.3/tests/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)      647 2023-04-13 21:59:31.000000 ape-solidity-0.6.3/tests/scripts/clean.py
--rw-r--r--   0 runner    (1001) docker     (123)    16112 2023-04-13 21:59:31.000000 ape-solidity-0.6.3/tests/test_compiler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-04-13 21:59:31.000000 ape-solidity-0.6.3/tests/test_integration.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:22:34.615694 ape-solidity-0.6.4/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:22:34.603694 ape-solidity-0.6.4/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:22:34.607694 ape-solidity-0.6.4/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      703 2023-05-18 15:21:33.000000 ape-solidity-0.6.4/.github/ISSUE_TEMPLATE/bug.md
+-rw-r--r--   0 runner    (1001) docker     (123)      668 2023-05-18 15:21:33.000000 ape-solidity-0.6.4/.github/ISSUE_TEMPLATE/feature.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-05-18 15:21:33.000000 ape-solidity-0.6.4/.github/ISSUE_TEMPLATE/work-item.md
+-rw-r--r--   0 runner    (1001) docker     (123)      474 2023-05-18 15:21:33.000000 ape-solidity-0.6.4/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      651 2023-05-18 15:21:33.000000 ape-solidity-0.6.4/.github/release-drafter.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:22:34.607694 ape-solidity-0.6.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      618 2023-05-18 15:21:33.000000 ape-solidity-0.6.4/.github/workflows/codeql.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      368 2023-05-18 15:21:33.000000 ape-solidity-0.6.4/.github/workflows/draft.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      551 2023-05-18 15:21:33.000000 ape-solidity-0.6.4/.github/workflows/prtitle.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      620 2023-05-18 15:21:33.000000 ape-solidity-0.6.4/.github/workflows/publish.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      709 2023-05-18 15:21:33.000000 ape-solidity-0.6.4/.github/workflows/stale-prs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2506 2023-05-18 15:21:33.000000 ape-solidity-0.6.4/.github/workflows/test.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1757 2023-05-18 15:21:33.000000 ape-solidity-0.6.4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-18 15:21:33.000000 ape-solidity-0.6.4/.mdformat.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      805 2023-05-18 15:21:33.000000 ape-solidity-0.6.4/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2175 2023-05-18 15:21:33.000000 ape-solidity-0.6.4/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11342 2023-05-18 15:21:33.000000 ape-solidity-0.6.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4874 2023-05-18 15:22:34.615694 ape-solidity-0.6.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3002 2023-05-18 15:21:33.000000 ape-solidity-0.6.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:22:34.607694 ape-solidity-0.6.4/ape_solidity/
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-05-18 15:21:33.000000 ape-solidity-0.6.4/ape_solidity/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6464 2023-05-18 15:21:33.000000 ape-solidity-0.6.4/ape_solidity/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29021 2023-05-18 15:21:33.000000 ape-solidity-0.6.4/ape_solidity/compiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-05-18 15:21:33.000000 ape-solidity-0.6.4/ape_solidity/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 15:21:33.000000 ape-solidity-0.6.4/ape_solidity/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-18 15:22:34.000000 ape-solidity-0.6.4/ape_solidity/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:22:34.607694 ape-solidity-0.6.4/ape_solidity.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4874 2023-05-18 15:22:34.000000 ape-solidity-0.6.4/ape_solidity.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3354 2023-05-18 15:22:34.000000 ape-solidity-0.6.4/ape_solidity.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 15:22:34.000000 ape-solidity-0.6.4/ape_solidity.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 15:22:34.000000 ape-solidity-0.6.4/ape_solidity.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-05-18 15:22:34.000000 ape-solidity-0.6.4/ape_solidity.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-18 15:22:34.000000 ape-solidity-0.6.4/ape_solidity.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      975 2023-05-18 15:21:33.000000 ape-solidity-0.6.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-05-18 15:22:34.615694 ape-solidity-0.6.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3353 2023-05-18 15:21:33.000000 ape-solidity-0.6.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:22:34.607694 ape-solidity-0.6.4/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:22:34.607694 ape-solidity-0.6.4/tests/BrownieProject/
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-05-18 15:21:33.000000 ape-solidity-0.6.4/tests/BrownieProject/brownie-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:22:34.607694 ape-solidity-0.6.4/tests/BrownieProject/contracts/
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-05-18 15:21:33.000000 ape-solidity-0.6.4/tests/BrownieProject/contracts/BrownieContract.sol
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:22:34.607694 ape-solidity-0.6.4/tests/BrownieStyleDependency/
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-18 15:21:33.000000 ape-solidity-0.6.4/tests/BrownieStyleDependency/ape-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:22:34.607694 ape-solidity-0.6.4/tests/BrownieStyleDependency/contracts/
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-05-18 15:21:33.000000 ape-solidity-0.6.4/tests/BrownieStyleDependency/contracts/BrownieStyleDependency.sol
+-rw-r--r--   0 runner    (1001) docker     (123)      251 2023-05-18 15:21:33.000000 ape-solidity-0.6.4/tests/BrownieStyleDependency/contracts/FailingContract.sol
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:22:34.607694 ape-solidity-0.6.4/tests/Dependency/
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-05-18 15:21:33.000000 ape-solidity-0.6.4/tests/Dependency/ape-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:22:34.607694 ape-solidity-0.6.4/tests/Dependency/contracts/
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-05-18 15:21:33.000000 ape-solidity-0.6.4/tests/Dependency/contracts/Dependency.sol
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-05-18 15:21:33.000000 ape-solidity-0.6.4/tests/Dependency/contracts/OlderDependency.sol
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:22:34.607694 ape-solidity-0.6.4/tests/Dependency/contracts/subfolder/
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-05-18 15:21:33.000000 ape-solidity-0.6.4/tests/Dependency/contracts/subfolder/InDependencySubfolder.sol
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:22:34.607694 ape-solidity-0.6.4/tests/Dependency/contracts/subfolder_with_imports/
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-05-18 15:21:33.000000 ape-solidity-0.6.4/tests/Dependency/contracts/subfolder_with_imports/InDependencySubfolderWithImports.sol
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:22:34.607694 ape-solidity-0.6.4/tests/DependencyOfDependency/
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-05-18 15:21:33.000000 ape-solidity-0.6.4/tests/DependencyOfDependency/ape-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:22:34.607694 ape-solidity-0.6.4/tests/DependencyOfDependency/contracts/
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-05-18 15:21:33.000000 ape-solidity-0.6.4/tests/DependencyOfDependency/contracts/DependencyOfDependency.sol
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:22:34.607694 ape-solidity-0.6.4/tests/ProjectWithinProject/
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-05-18 15:21:33.000000 ape-solidity-0.6.4/tests/ProjectWithinProject/ape-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:22:34.607694 ape-solidity-0.6.4/tests/ProjectWithinProject/contracts/
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-05-18 15:21:33.000000 ape-solidity-0.6.4/tests/ProjectWithinProject/contracts/Contract.sol
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:22:34.607694 ape-solidity-0.6.4/tests/VersionSpecifiedInConfig/
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-18 15:21:33.000000 ape-solidity-0.6.4/tests/VersionSpecifiedInConfig/ape-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:22:34.607694 ape-solidity-0.6.4/tests/VersionSpecifiedInConfig/contracts/
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-05-18 15:21:33.000000 ape-solidity-0.6.4/tests/VersionSpecifiedInConfig/contracts/VersionSpecifiedInConfig.sol
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 15:21:33.000000 ape-solidity-0.6.4/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-05-18 15:21:33.000000 ape-solidity-0.6.4/tests/ape-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3462 2023-05-18 15:21:33.000000 ape-solidity-0.6.4/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:22:34.611694 ape-solidity-0.6.4/tests/contracts/
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-05-18 15:21:33.000000 ape-solidity-0.6.4/tests/contracts/CircularImport1.sol
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-05-18 15:21:33.000000 ape-solidity-0.6.4/tests/contracts/CircularImport2.sol
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-05-18 15:21:33.000000 ape-solidity-0.6.4/tests/contracts/CompilesOnce.sol
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-05-18 15:21:33.000000 ape-solidity-0.6.4/tests/contracts/DifferentNameThanFile.sol
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:22:34.611694 ape-solidity-0.6.4/tests/contracts/DirectoryWithExtension.sol/
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-05-18 15:21:33.000000 ape-solidity-0.6.4/tests/contracts/DirectoryWithExtension.sol/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-05-18 15:21:33.000000 ape-solidity-0.6.4/tests/contracts/ExperimentalABIEncoderV2.sol
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-05-18 15:21:33.000000 ape-solidity-0.6.4/tests/contracts/HasError.sol
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-05-18 15:21:33.000000 ape-solidity-0.6.4/tests/contracts/ImportOlderDependency.sol
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-05-18 15:21:33.000000 ape-solidity-0.6.4/tests/contracts/ImportSourceWithEqualSignVersion.sol
+-rw-r--r--   0 runner    (1001) docker     (123)      384 2023-05-18 15:21:33.000000 ape-solidity-0.6.4/tests/contracts/ImportSourceWithNoPrefixVersion.sol
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-05-18 15:21:33.000000 ape-solidity-0.6.4/tests/contracts/ImportingLessConstrainedVersion.sol
+-rw-r--r--   0 runner    (1001) docker     (123)      682 2023-05-18 15:21:33.000000 ape-solidity-0.6.4/tests/contracts/Imports.sol
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-05-18 15:21:33.000000 ape-solidity-0.6.4/tests/contracts/IndirectlyImportingMoreConstrainedVersion.sol
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2023-05-18 15:21:33.000000 ape-solidity-0.6.4/tests/contracts/IndirectlyImportingMoreConstrainedVersionCompanion.sol
+-rw-r--r--   0 runner    (1001) docker     (123)      474 2023-05-18 15:21:33.000000 ape-solidity-0.6.4/tests/contracts/IndirectlyImportingMoreConstrainedVersionCompanionImport.sol
+-rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-05-18 15:21:33.000000 ape-solidity-0.6.4/tests/contracts/LibraryFun.sol
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-05-18 15:21:33.000000 ape-solidity-0.6.4/tests/contracts/MissingPragma.sol
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-05-18 15:21:33.000000 ape-solidity-0.6.4/tests/contracts/MultipleDefinitions.sol
+-rw-r--r--   0 runner    (1001) docker     (123)      484 2023-05-18 15:21:33.000000 ape-solidity-0.6.4/tests/contracts/NumerousDefinitions.sol
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-18 15:21:33.000000 ape-solidity-0.6.4/tests/contracts/OlderVersion.sol
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-05-18 15:21:33.000000 ape-solidity-0.6.4/tests/contracts/RandomVyperFile.vy
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-05-18 15:21:33.000000 ape-solidity-0.6.4/tests/contracts/RangedVersion.sol
+-rw-r--r--   0 runner    (1001) docker     (123)      480 2023-05-18 15:21:33.000000 ape-solidity-0.6.4/tests/contracts/SpacesInPragma.sol
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-05-18 15:21:33.000000 ape-solidity-0.6.4/tests/contracts/SpecificVersionNoPrefix.sol
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-05-18 15:21:33.000000 ape-solidity-0.6.4/tests/contracts/SpecificVersionNoPrefix2.sol
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-05-18 15:21:33.000000 ape-solidity-0.6.4/tests/contracts/SpecificVersionRange.sol
+-rw-r--r--   0 runner    (1001) docker     (123)      203 2023-05-18 15:21:33.000000 ape-solidity-0.6.4/tests/contracts/SpecificVersionWithEqualSign.sol
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-05-18 15:21:33.000000 ape-solidity-0.6.4/tests/contracts/UseYearn.sol
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-05-18 15:21:33.000000 ape-solidity-0.6.4/tests/contracts/VagueVersion.sol
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:22:34.611694 ape-solidity-0.6.4/tests/contracts/subfolder/
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-05-18 15:21:33.000000 ape-solidity-0.6.4/tests/contracts/subfolder/Relativecontract.sol
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-05-18 15:21:33.000000 ape-solidity-0.6.4/tests/contracts/subfolder/UsingDependencyWithinSubFolder.sol
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:22:34.603694 ape-solidity-0.6.4/tests/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:22:34.603694 ape-solidity-0.6.4/tests/data/packages/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:22:34.603694 ape-solidity-0.6.4/tests/data/packages/OpenZeppelin/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:22:34.611694 ape-solidity-0.6.4/tests/data/packages/OpenZeppelin/v4.5.0/
+-rw-r--r--   0 runner    (1001) docker     (123)   698486 2023-05-18 15:21:33.000000 ape-solidity-0.6.4/tests/data/packages/OpenZeppelin/v4.5.0/OpenZeppelin.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:22:34.611694 ape-solidity-0.6.4/tests/data/packages/OpenZeppelin/v4.7.1/
+-rw-r--r--   0 runner    (1001) docker     (123)   879002 2023-05-18 15:21:33.000000 ape-solidity-0.6.4/tests/data/packages/OpenZeppelin/v4.7.1/OpenZeppelin.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:22:34.603694 ape-solidity-0.6.4/tests/data/packages/vault/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:22:34.615694 ape-solidity-0.6.4/tests/data/packages/vault/master/
+-rw-r--r--   0 runner    (1001) docker     (123)   167518 2023-05-18 15:21:33.000000 ape-solidity-0.6.4/tests/data/packages/vault/master/vault_main.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:22:34.615694 ape-solidity-0.6.4/tests/data/packages/vault/v0.4.5/
+-rw-r--r--   0 runner    (1001) docker     (123)   167551 2023-05-18 15:21:33.000000 ape-solidity-0.6.4/tests/data/packages/vault/v0.4.5/vault.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:22:34.615694 ape-solidity-0.6.4/tests/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)      647 2023-05-18 15:21:33.000000 ape-solidity-0.6.4/tests/scripts/clean.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16243 2023-05-18 15:21:33.000000 ape-solidity-0.6.4/tests/test_compiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-05-18 15:21:33.000000 ape-solidity-0.6.4/tests/test_integration.py
```

### Comparing `ape-solidity-0.6.3/.github/ISSUE_TEMPLATE/bug.md` & `ape-solidity-0.6.4/.github/ISSUE_TEMPLATE/bug.md`

 * *Files identical despite different names*

### Comparing `ape-solidity-0.6.3/.github/ISSUE_TEMPLATE/feature.md` & `ape-solidity-0.6.4/.github/ISSUE_TEMPLATE/feature.md`

 * *Files identical despite different names*

### Comparing `ape-solidity-0.6.3/.github/ISSUE_TEMPLATE/work-item.md` & `ape-solidity-0.6.4/.github/ISSUE_TEMPLATE/work-item.md`

 * *Files identical despite different names*

### Comparing `ape-solidity-0.6.3/.github/release-drafter.yml` & `ape-solidity-0.6.4/.github/release-drafter.yml`

 * *Files identical despite different names*

### Comparing `ape-solidity-0.6.3/.github/workflows/codeql.yml` & `ape-solidity-0.6.4/.github/workflows/codeql.yml`

 * *Files identical despite different names*

### Comparing `ape-solidity-0.6.3/.github/workflows/prtitle.yaml` & `ape-solidity-0.6.4/.github/workflows/prtitle.yaml`

 * *Files identical despite different names*

### Comparing `ape-solidity-0.6.3/.github/workflows/publish.yaml` & `ape-solidity-0.6.4/.github/workflows/publish.yaml`

 * *Files identical despite different names*

### Comparing `ape-solidity-0.6.3/.github/workflows/stale-prs.yml` & `ape-solidity-0.6.4/.github/workflows/stale-prs.yml`

 * *Files identical despite different names*

### Comparing `ape-solidity-0.6.3/.github/workflows/test.yaml` & `ape-solidity-0.6.4/.github/workflows/test.yaml`

 * *Files identical despite different names*

### Comparing `ape-solidity-0.6.3/.gitignore` & `ape-solidity-0.6.4/.gitignore`

 * *Files identical despite different names*

### Comparing `ape-solidity-0.6.3/.pre-commit-config.yaml` & `ape-solidity-0.6.4/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `ape-solidity-0.6.3/CONTRIBUTING.md` & `ape-solidity-0.6.4/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `ape-solidity-0.6.3/LICENSE` & `ape-solidity-0.6.4/LICENSE`

 * *Files identical despite different names*

### Comparing `ape-solidity-0.6.3/PKG-INFO` & `ape-solidity-0.6.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ape-solidity
-Version: 0.6.3
+Version: 0.6.4
 Summary: Plugin for Ape Ethereum Framework for compiling Solidity contracts
 Home-page: https://github.com/ApeWorX/ape-solidity
 Author: ApeWorX Ltd.
 Author-email: admin@apeworx.io
 License: Apache-2.0
 Description: # Quick Start
```

### Comparing `ape-solidity-0.6.3/README.md` & `ape-solidity-0.6.4/README.md`

 * *Files identical despite different names*

### Comparing `ape-solidity-0.6.3/ape_solidity/_utils.py` & `ape-solidity-0.6.4/ape_solidity/_utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -34,21 +34,23 @@
 
         return value
 
     @property
     def _parts(self) -> List[str]:
         return self.entry.split("=")
 
+    # path normalization needed in case delimiter in remapping key/value
+    # and system path delimiter are different (Windows as an example)
     @property
     def key(self) -> str:
-        return self._parts[0]
+        return os.path.normpath(self._parts[0])
 
     @property
     def name(self) -> str:
-        suffix_str = self._parts[1]
+        suffix_str = os.path.normpath(self._parts[1])
         return suffix_str.split(os.path.sep)[0]
 
     @property
     def package_id(self) -> Path:
         suffix = Path(self._parts[1])
         data_folder_cache = self.packages_cache / suffix
```

### Comparing `ape-solidity-0.6.3/ape_solidity/compiler.py` & `ape-solidity-0.6.4/ape_solidity/compiler.py`

 * *Files 1% similar despite different names*

```diff
@@ -222,21 +222,27 @@
 
             dependency_name = str(dependency_package_name)
             if str(self.config_manager.packages_folder) in uri_str:
                 # Using a local dependency
                 version = "local"
             else:
                 # Check for GitHub-style dependency
-                version_match = re.match(r".*/releases/tag/(v?[\d|.]+)", str(uri_str))
-                if version_match:
-                    version = version_match.groups()[0]
-                    if not version.startswith("v"):
-                        version = f"v{version}"
-                else:
-                    raise CompilerError(f"Unable to discern dependency type '{uri_str}'.")
+                match_checks = (r".*/releases/tag/(v?[\d|.]+)", r".*/tree/(v?[\w|.|\d]+)")
+                version = None
+                for check in match_checks:
+                    version_match = re.match(check, str(uri_str))
+                    if version_match:
+                        version = version_match.groups()[0]
+                        if not version.startswith("v") and version[0].isnumeric():
+                            version = f"v{version}"
+
+                        break
+
+            if version is None:
+                raise CompilerError(f"Unable to discern dependency type '{uri_str}'.")
 
             # Find matching package
             for package in packages_dir.iterdir():
                 if package.name.replace("_", "-").lower() == dependency_name:
                     dependency_name = str(package.name)
                     break
```

### Comparing `ape-solidity-0.6.3/ape_solidity.egg-info/PKG-INFO` & `ape-solidity-0.6.4/ape_solidity.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ape-solidity
-Version: 0.6.3
+Version: 0.6.4
 Summary: Plugin for Ape Ethereum Framework for compiling Solidity contracts
 Home-page: https://github.com/ApeWorX/ape-solidity
 Author: ApeWorX Ltd.
 Author-email: admin@apeworx.io
 License: Apache-2.0
 Description: # Quick Start
```

### Comparing `ape-solidity-0.6.3/ape_solidity.egg-info/SOURCES.txt` & `ape-solidity-0.6.4/ape_solidity.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -78,8 +78,12 @@
 tests/contracts/SpecificVersionRange.sol
 tests/contracts/SpecificVersionWithEqualSign.sol
 tests/contracts/UseYearn.sol
 tests/contracts/VagueVersion.sol
 tests/contracts/DirectoryWithExtension.sol/README.md
 tests/contracts/subfolder/Relativecontract.sol
 tests/contracts/subfolder/UsingDependencyWithinSubFolder.sol
+tests/data/packages/OpenZeppelin/v4.5.0/OpenZeppelin.json
+tests/data/packages/OpenZeppelin/v4.7.1/OpenZeppelin.json
+tests/data/packages/vault/master/vault_main.json
+tests/data/packages/vault/v0.4.5/vault.json
 tests/scripts/clean.py
```

### Comparing `ape-solidity-0.6.3/ape_solidity.egg-info/requires.txt` & `ape-solidity-0.6.4/ape_solidity.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `ape-solidity-0.6.3/pyproject.toml` & `ape-solidity-0.6.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ape-solidity-0.6.3/setup.py` & `ape-solidity-0.6.4/setup.py`

 * *Files identical despite different names*

### Comparing `ape-solidity-0.6.3/tests/ape-config.yaml` & `ape-solidity-0.6.4/tests/ape-config.yaml`

 * *Files 11% similar despite different names*

```diff
@@ -13,23 +13,29 @@
     local: ./BrownieStyleDependency
 
   # Ensure we can build a realistic-brownie project with dependencies.
   - name: vault
     github: yearn/yearn-vaults
     version: 0.4.5
 
+  # Ensure dependencies using GitHub references work.
+  - name: vault
+    github: yearn/yearn-vaults
+    ref: master
+
 solidity:
   import_remapping:
     - "@remapping/contracts=TestDependency"
     - "@remapping_2=TestDependency"
     - "@remapping_2_brownie=BrownieDependency"
 
     # Remapping for showing we can import a contract type from a brownie-style dependency
     # (provided the _single_ contract type compiles in the project).
     - "@styleofbrownie=BrownieStyleDependency"
 
     # Ensure yearn-vaults works as a remapping
     - "@vault=vault/v0.4.5"
+    - "@vaultmain=vault/master"
 
 
   # Using evm_version compatible with older and newer solidity versions.
   evm_version: constantinople
```

### Comparing `ape-solidity-0.6.3/tests/conftest.py` & `ape-solidity-0.6.4/tests/conftest.py`

 * *Files 13% similar despite different names*

```diff
@@ -8,16 +8,18 @@
 import ape
 import pytest
 import solcx  # type: ignore
 
 from ape_solidity.compiler import Extension
 
 # NOTE: Ensure that we don't use local paths for these
-ape.config.DATA_FOLDER = Path(mkdtemp()).resolve()
-ape.config.PROJECT_FOLDER = Path(mkdtemp()).resolve()
+DATA_FOLDER = Path(mkdtemp()).resolve()
+PROJECT_FOLDER = Path(mkdtemp()).resolve()
+ape.config.DATA_FOLDER = DATA_FOLDER
+ape.config.PROJECT_FOLDER = PROJECT_FOLDER
 
 
 @contextmanager
 def _tmp_solcx_path(monkeypatch):
     solcx_install_path = mkdtemp()
 
     monkeypatch.setenv(
@@ -58,23 +60,31 @@
     """
     Creates a new, temporary installation path for solcx for a given test.
     """
     with _tmp_solcx_path(monkeypatch) as path:
         yield path
 
 
+@pytest.fixture(autouse=True)
+def data_folder():
+    base_path = Path(__file__).parent / "data"
+    copy_tree(base_path.as_posix(), DATA_FOLDER.as_posix())
+    return DATA_FOLDER
+
+
 @pytest.fixture
 def config():
     return ape.config
 
 
 @pytest.fixture(autouse=True)
-def project(config):
+def project(data_folder, config):
+    _ = data_folder  # Ensure happens first.
     project_source_dir = Path(__file__).parent
-    project_dest_dir = config.PROJECT_FOLDER / project_source_dir.name
+    project_dest_dir = PROJECT_FOLDER / project_source_dir.name
 
     # Delete build / .cache that may exist pre-copy
     project_path = Path(__file__).parent
     for path in (
         project_path,
         project_path / "BrownieProject",
         project_path / "BrownieStyleDependency",
```

### Comparing `ape-solidity-0.6.3/tests/contracts/Imports.sol` & `ape-solidity-0.6.4/tests/contracts/Imports.sol`

 * *Files identical despite different names*

### Comparing `ape-solidity-0.6.3/tests/contracts/LibraryFun.sol` & `ape-solidity-0.6.4/tests/contracts/LibraryFun.sol`

 * *Files identical despite different names*

### Comparing `ape-solidity-0.6.3/tests/scripts/clean.py` & `ape-solidity-0.6.4/tests/scripts/clean.py`

 * *Files identical despite different names*

### Comparing `ape-solidity-0.6.3/tests/test_compiler.py` & `ape-solidity-0.6.4/tests/test_compiler.py`

 * *Files 1% similar despite different names*

```diff
@@ -139,14 +139,15 @@
         "@dependency_remapping": ".cache/TestDependencyOfDependency/local",
         "@remapping_2": ".cache/TestDependency/local",
         "@remapping/contracts": ".cache/TestDependency/local",
         "@styleofbrownie": ".cache/BrownieStyleDependency/local",
         "@openzeppelin/contracts": ".cache/OpenZeppelin/v4.7.1",
         "@oz/contracts": ".cache/OpenZeppelin/v4.5.0",
         "@vault": ".cache/vault/v0.4.5",
+        "@vaultmain": ".cache/vault/master",
     }
 
     with config.using_project(project.path / "ProjectWithinProject") as proj:
         # Trigger downloading dependencies in new ProjectWithinProject
         dependencies = proj.dependencies
         assert dependencies
         # Should be different now that we have changed projects.
@@ -249,14 +250,15 @@
     ), f"Remappings found: {compiler_0812.settings['remappings']}"
 
     assert (
         "@openzeppelin/contracts=.cache/OpenZeppelin/v4.7.1"
         in compiler_latest.settings["remappings"]
     )
     assert "@vault=.cache/vault/v0.4.5" in compiler_latest.settings["remappings"]
+    assert "@vaultmain=.cache/vault/master" in compiler_latest.settings["remappings"]
     common_suffix = ".cache/TestDependency/local"
     expected_remappings = (
         "@remapping_2_brownie=.cache/BrownieDependency/local",
         "@dependency_remapping=.cache/TestDependencyOfDependency/local",
         f"@remapping_2={common_suffix}",
         f"@remapping/contracts={common_suffix}",
         "@styleofbrownie=.cache/BrownieStyleDependency/local",
```

### Comparing `ape-solidity-0.6.3/tests/test_integration.py` & `ape-solidity-0.6.4/tests/test_integration.py`

 * *Files identical despite different names*

