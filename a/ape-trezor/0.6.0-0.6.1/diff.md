# Comparing `tmp/ape-trezor-0.6.0.tar.gz` & `tmp/ape-trezor-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ape-trezor-0.6.0.tar", last modified: Tue Jan 31 22:29:03 2023, max compression
+gzip compressed data, was "ape-trezor-0.6.1.tar", last modified: Thu May 18 17:43:35 2023, max compression
```

## Comparing `ape-trezor-0.6.0.tar` & `ape-trezor-0.6.1.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 22:29:03.198204 ape-trezor-0.6.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 22:29:03.194204 ape-trezor-0.6.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 22:29:03.194204 ape-trezor-0.6.0/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      703 2023-01-31 22:28:08.000000 ape-trezor-0.6.0/.github/ISSUE_TEMPLATE/bug.md
--rw-r--r--   0 runner    (1001) docker     (123)      668 2023-01-31 22:28:08.000000 ape-trezor-0.6.0/.github/ISSUE_TEMPLATE/feature.md
--rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-01-31 22:28:08.000000 ape-trezor-0.6.0/.github/ISSUE_TEMPLATE/work-item.md
--rw-r--r--   0 runner    (1001) docker     (123)      474 2023-01-31 22:28:08.000000 ape-trezor-0.6.0/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (123)      651 2023-01-31 22:28:08.000000 ape-trezor-0.6.0/.github/release-drafter.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 22:29:03.198204 ape-trezor-0.6.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      618 2023-01-31 22:28:08.000000 ape-trezor-0.6.0/.github/workflows/codeql.yml
--rw-r--r--   0 runner    (1001) docker     (123)      621 2023-01-31 22:28:08.000000 ape-trezor-0.6.0/.github/workflows/commit.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      368 2023-01-31 22:28:08.000000 ape-trezor-0.6.0/.github/workflows/draft.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      551 2023-01-31 22:28:08.000000 ape-trezor-0.6.0/.github/workflows/prtitle.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      620 2023-01-31 22:28:08.000000 ape-trezor-0.6.0/.github/workflows/publish.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      709 2023-01-31 22:28:08.000000 ape-trezor-0.6.0/.github/workflows/stale-prs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2479 2023-01-31 22:28:08.000000 ape-trezor-0.6.0/.github/workflows/test.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1719 2023-01-31 22:28:08.000000 ape-trezor-0.6.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-01-31 22:28:08.000000 ape-trezor-0.6.0/.mdformat.toml
--rw-r--r--   0 runner    (1001) docker     (123)      803 2023-01-31 22:28:08.000000 ape-trezor-0.6.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1662 2023-01-31 22:28:08.000000 ape-trezor-0.6.0/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)    11342 2023-01-31 22:28:08.000000 ape-trezor-0.6.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4398 2023-01-31 22:29:03.198204 ape-trezor-0.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2662 2023-01-31 22:28:08.000000 ape-trezor-0.6.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 22:29:03.198204 ape-trezor-0.6.0/ape_trezor/
--rw-r--r--   0 runner    (1001) docker     (123)      280 2023-01-31 22:28:08.000000 ape-trezor-0.6.0/ape_trezor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5195 2023-01-31 22:28:08.000000 ape-trezor-0.6.0/ape_trezor/_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     4707 2023-01-31 22:28:08.000000 ape-trezor-0.6.0/ape_trezor/accounts.py
--rw-r--r--   0 runner    (1001) docker     (123)     3232 2023-01-31 22:28:08.000000 ape-trezor-0.6.0/ape_trezor/choices.py
--rw-r--r--   0 runner    (1001) docker     (123)     6033 2023-01-31 22:28:08.000000 ape-trezor-0.6.0/ape_trezor/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-01-31 22:28:08.000000 ape-trezor-0.6.0/ape_trezor/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-01-31 22:28:08.000000 ape-trezor-0.6.0/ape_trezor/hdpath.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-31 22:28:08.000000 ape-trezor-0.6.0/ape_trezor/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-01-31 22:28:08.000000 ape-trezor-0.6.0/ape_trezor/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-01-31 22:29:03.000000 ape-trezor-0.6.0/ape_trezor/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 22:29:03.198204 ape-trezor-0.6.0/ape_trezor.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4398 2023-01-31 22:29:03.000000 ape-trezor-0.6.0/ape_trezor.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-01-31 22:29:03.000000 ape-trezor-0.6.0/ape_trezor.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-31 22:29:03.000000 ape-trezor-0.6.0/ape_trezor.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-01-31 22:29:03.000000 ape-trezor-0.6.0/ape_trezor.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-31 22:29:03.000000 ape-trezor-0.6.0/ape_trezor.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      827 2023-01-31 22:29:03.000000 ape-trezor-0.6.0/ape_trezor.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-01-31 22:29:03.000000 ape-trezor-0.6.0/ape_trezor.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      945 2023-01-31 22:28:08.000000 ape-trezor-0.6.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-01-31 22:29:03.198204 ape-trezor-0.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3567 2023-01-31 22:28:08.000000 ape-trezor-0.6.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 22:29:03.198204 ape-trezor-0.6.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-31 22:28:08.000000 ape-trezor-0.6.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3213 2023-01-31 22:28:08.000000 ape-trezor-0.6.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     3436 2023-01-31 22:28:08.000000 ape-trezor-0.6.0/tests/test_accounts.py
--rw-r--r--   0 runner    (1001) docker     (123)      787 2023-01-31 22:28:08.000000 ape-trezor-0.6.0/tests/test_choices.py
--rw-r--r--   0 runner    (1001) docker     (123)     3681 2023-01-31 22:28:08.000000 ape-trezor-0.6.0/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     6670 2023-01-31 22:28:08.000000 ape-trezor-0.6.0/tests/test_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 22:29:03.198204 ape-trezor-0.6.0/tests/trezor/
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-01-31 22:28:08.000000 ape-trezor-0.6.0/tests/trezor/vitalik.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 17:43:35.548694 ape-trezor-0.6.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 17:43:35.544694 ape-trezor-0.6.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 17:43:35.544694 ape-trezor-0.6.1/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      703 2023-05-18 17:42:33.000000 ape-trezor-0.6.1/.github/ISSUE_TEMPLATE/bug.md
+-rw-r--r--   0 runner    (1001) docker     (123)      668 2023-05-18 17:42:33.000000 ape-trezor-0.6.1/.github/ISSUE_TEMPLATE/feature.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-05-18 17:42:33.000000 ape-trezor-0.6.1/.github/ISSUE_TEMPLATE/work-item.md
+-rw-r--r--   0 runner    (1001) docker     (123)      474 2023-05-18 17:42:33.000000 ape-trezor-0.6.1/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      651 2023-05-18 17:42:33.000000 ape-trezor-0.6.1/.github/release-drafter.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 17:43:35.544694 ape-trezor-0.6.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      618 2023-05-18 17:42:33.000000 ape-trezor-0.6.1/.github/workflows/codeql.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      624 2023-05-18 17:42:33.000000 ape-trezor-0.6.1/.github/workflows/commit.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      368 2023-05-18 17:42:33.000000 ape-trezor-0.6.1/.github/workflows/draft.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      554 2023-05-18 17:42:33.000000 ape-trezor-0.6.1/.github/workflows/prtitle.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-05-18 17:42:33.000000 ape-trezor-0.6.1/.github/workflows/publish.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      709 2023-05-18 17:42:33.000000 ape-trezor-0.6.1/.github/workflows/stale-prs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2488 2023-05-18 17:42:33.000000 ape-trezor-0.6.1/.github/workflows/test.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1719 2023-05-18 17:42:33.000000 ape-trezor-0.6.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-18 17:42:33.000000 ape-trezor-0.6.1/.mdformat.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      802 2023-05-18 17:42:33.000000 ape-trezor-0.6.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1653 2023-05-18 17:42:33.000000 ape-trezor-0.6.1/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11342 2023-05-18 17:42:33.000000 ape-trezor-0.6.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3573 2023-05-18 17:43:35.548694 ape-trezor-0.6.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2662 2023-05-18 17:42:33.000000 ape-trezor-0.6.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 17:43:35.548694 ape-trezor-0.6.1/ape_trezor/
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-05-18 17:42:33.000000 ape-trezor-0.6.1/ape_trezor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5193 2023-05-18 17:42:33.000000 ape-trezor-0.6.1/ape_trezor/_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4707 2023-05-18 17:42:33.000000 ape-trezor-0.6.1/ape_trezor/accounts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3232 2023-05-18 17:42:33.000000 ape-trezor-0.6.1/ape_trezor/choices.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6033 2023-05-18 17:42:33.000000 ape-trezor-0.6.1/ape_trezor/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-05-18 17:42:33.000000 ape-trezor-0.6.1/ape_trezor/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-05-18 17:42:33.000000 ape-trezor-0.6.1/ape_trezor/hdpath.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 17:42:33.000000 ape-trezor-0.6.1/ape_trezor/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-18 17:42:33.000000 ape-trezor-0.6.1/ape_trezor/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-18 17:43:35.000000 ape-trezor-0.6.1/ape_trezor/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 17:43:35.548694 ape-trezor-0.6.1/ape_trezor.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3573 2023-05-18 17:43:35.000000 ape-trezor-0.6.1/ape_trezor.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-05-18 17:43:35.000000 ape-trezor-0.6.1/ape_trezor.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 17:43:35.000000 ape-trezor-0.6.1/ape_trezor.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-18 17:43:35.000000 ape-trezor-0.6.1/ape_trezor.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 17:43:35.000000 ape-trezor-0.6.1/ape_trezor.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      825 2023-05-18 17:43:35.000000 ape-trezor-0.6.1/ape_trezor.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-18 17:43:35.000000 ape-trezor-0.6.1/ape_trezor.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      945 2023-05-18 17:42:33.000000 ape-trezor-0.6.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-05-18 17:43:35.548694 ape-trezor-0.6.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3566 2023-05-18 17:42:33.000000 ape-trezor-0.6.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 17:43:35.548694 ape-trezor-0.6.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 17:42:33.000000 ape-trezor-0.6.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3213 2023-05-18 17:42:33.000000 ape-trezor-0.6.1/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3436 2023-05-18 17:42:33.000000 ape-trezor-0.6.1/tests/test_accounts.py
+-rw-r--r--   0 runner    (1001) docker     (123)      787 2023-05-18 17:42:33.000000 ape-trezor-0.6.1/tests/test_choices.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3681 2023-05-18 17:42:33.000000 ape-trezor-0.6.1/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6670 2023-05-18 17:42:33.000000 ape-trezor-0.6.1/tests/test_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 17:43:35.548694 ape-trezor-0.6.1/tests/trezor/
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-18 17:42:33.000000 ape-trezor-0.6.1/tests/trezor/vitalik.json
```

### Comparing `ape-trezor-0.6.0/.github/ISSUE_TEMPLATE/bug.md` & `ape-trezor-0.6.1/.github/ISSUE_TEMPLATE/bug.md`

 * *Files identical despite different names*

### Comparing `ape-trezor-0.6.0/.github/ISSUE_TEMPLATE/feature.md` & `ape-trezor-0.6.1/.github/ISSUE_TEMPLATE/feature.md`

 * *Files identical despite different names*

### Comparing `ape-trezor-0.6.0/.github/ISSUE_TEMPLATE/work-item.md` & `ape-trezor-0.6.1/.github/ISSUE_TEMPLATE/work-item.md`

 * *Files identical despite different names*

### Comparing `ape-trezor-0.6.0/.github/release-drafter.yml` & `ape-trezor-0.6.1/.github/release-drafter.yml`

 * *Files identical despite different names*

### Comparing `ape-trezor-0.6.0/.github/workflows/codeql.yml` & `ape-trezor-0.6.1/.github/workflows/codeql.yml`

 * *Files identical despite different names*

### Comparing `ape-trezor-0.6.0/.github/workflows/commit.yaml` & `ape-trezor-0.6.1/.github/workflows/commit.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -12,14 +12,14 @@
         - uses: actions/checkout@v3
           with:
               fetch-depth: 0
 
         - name: Setup Python
           uses: actions/setup-python@v4
           with:
-              python-version: 3.8
+              python-version: "3.10"
 
         - name: Install Dependencies
           run: pip install commitizen
 
         - name: Check commit history
           run: cz check --rev-range $(git rev-list --all --reverse | head -1)..HEAD
```

### Comparing `ape-trezor-0.6.0/.github/workflows/prtitle.yaml` & `ape-trezor-0.6.1/.github/workflows/prtitle.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
         steps:
         - uses: actions/checkout@v3
 
         - name: Setup Python
           uses: actions/setup-python@v4
           with:
-              python-version: 3.8
+              python-version: "3.10"
 
         - name: Install Dependencies
           run: pip install commitizen
 
         - name: Check PR Title
           env:
               TITLE: ${{ github.event.pull_request.title }}
```

### Comparing `ape-trezor-0.6.0/.github/workflows/publish.yaml` & `ape-trezor-0.6.1/.github/workflows/publish.yaml`

 * *Files 21% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
     steps:
     - uses: actions/checkout@v3
 
     - name: Set up Python
       uses: actions/setup-python@v4
       with:
-        python-version: 3.8
+        python-version: "3.10"
 
     - name: Install dependencies
       run: |
         python -m pip install --upgrade pip
         pip install -e .[release]
         
     - name: Build
```

### Comparing `ape-trezor-0.6.0/.github/workflows/stale-prs.yml` & `ape-trezor-0.6.1/.github/workflows/stale-prs.yml`

 * *Files identical despite different names*

### Comparing `ape-trezor-0.6.0/.github/workflows/test.yaml` & `ape-trezor-0.6.1/.github/workflows/test.yaml`

 * *Files 3% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
         steps:
         - uses: actions/checkout@v3
 
         - name: Setup Python
           uses: actions/setup-python@v4
           with:
-              python-version: 3.8
+              python-version: "3.10"
 
         - name: Install Dependencies
           run: |
             python -m pip install --upgrade pip
             pip install .[lint]
 
         - name: Run Black
@@ -43,15 +43,15 @@
 
         steps:
         - uses: actions/checkout@v3
 
         - name: Setup Python
           uses: actions/setup-python@v4
           with:
-              python-version: 3.8
+              python-version: "3.10"
 
         - name: Install Dependencies
           run: |
             python -m pip install --upgrade pip
             pip install .[lint,test]
 
         - name: Run MyPy
@@ -90,14 +90,14 @@
 #
 #        steps:
 #        - uses: actions/checkout@v3
 #
 #        - name: Setup Python
 #          uses: actions/setup-python@v4
 #          with:
-#              python-version: 3.8
+#              python-version: "3.10"
 #
 #        - name: Install Dependencies
 #          run: pip install .[test]
 #
 #        - name: Run Tests
 #          run: pytest -m "fuzzing" --no-cov -s
```

### Comparing `ape-trezor-0.6.0/.gitignore` & `ape-trezor-0.6.1/.gitignore`

 * *Files identical despite different names*

### Comparing `ape-trezor-0.6.0/.pre-commit-config.yaml` & `ape-trezor-0.6.1/.pre-commit-config.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 -   repo: https://github.com/pre-commit/mirrors-isort
     rev: v5.10.1
     hooks:
       - id: isort
 
 -   repo: https://github.com/psf/black
-    rev: 22.12.0
+    rev: 23.3.0
     hooks:
       - id: black
         name: black
 
 -   repo: https://github.com/pycqa/flake8
     rev: 5.0.4
     hooks:
```

### Comparing `ape-trezor-0.6.0/CONTRIBUTING.md` & `ape-trezor-0.6.1/CONTRIBUTING.md`

 * *Files 2% similar despite different names*

```diff
@@ -42,8 +42,8 @@
 
 It's a good idea to make pull requests early on.
 A pull request represents the start of a discussion, and doesn't necessarily need to be the final, finished submission.
 
 If you are opening a work-in-progress pull request to verify that it passes CI tests, please consider
 [marking it as a draft](https://help.github.com/en/github/collaborating-with-issues-and-pull-requests/about-pull-requests#draft-pull-requests).
 
-Join the Ethereum Python [Discord](https://discord.gg/PcEJ54yX) if you have any questions.
+Join the ApeWorX [Discord](https://discord.gg/apeworx) if you have any questions.
```

### Comparing `ape-trezor-0.6.0/LICENSE` & `ape-trezor-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ape-trezor-0.6.0/README.md` & `ape-trezor-0.6.1/README.md`

 * *Files identical despite different names*

### Comparing `ape-trezor-0.6.0/ape_trezor/_cli.py` & `ape-trezor-0.6.1/ape_trezor/_cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -119,15 +119,14 @@
 
 
 @cli.command(short_help="Sign a message with your Trezor device")
 @click.argument("alias")
 @click.argument("message")
 @ape_cli_context()
 def sign_message(cli_ctx, alias, message):
-
     if alias not in accounts.aliases:
         cli_ctx.abort(f"Account with alias '{alias}' does not exist.")
 
     eip191_message = encode_defunct(text=message)
     account = accounts.load(alias)
     signature = account.sign_message(eip191_message)
     signature_bytes = signature.encode_rsv()
@@ -141,15 +140,14 @@
     click.echo("Signature: " + signature.encode_rsv().hex())
 
 
 @cli.command(short_help="Verify a message with your Trezor device")
 @click.argument("message")
 @click.argument("signature")
 def verify_message(message, signature):
-
     eip191message = encode_defunct(text=message)
 
     try:
         signer_address = Account.recover_message(eip191message, signature=signature)
     except ValueError as exc:
         message = "Message cannot be verified. Check the signature and try again."
         raise TrezorSigningError(message) from exc
```

### Comparing `ape-trezor-0.6.0/ape_trezor/accounts.py` & `ape-trezor-0.6.1/ape_trezor/accounts.py`

 * *Files identical despite different names*

### Comparing `ape-trezor-0.6.0/ape_trezor/choices.py` & `ape-trezor-0.6.1/ape_trezor/choices.py`

 * *Files identical despite different names*

### Comparing `ape-trezor-0.6.0/ape_trezor/client.py` & `ape-trezor-0.6.1/ape_trezor/client.py`

 * *Files identical despite different names*

### Comparing `ape-trezor-0.6.0/ape_trezor/exceptions.py` & `ape-trezor-0.6.1/ape_trezor/exceptions.py`

 * *Files identical despite different names*

### Comparing `ape-trezor-0.6.0/ape_trezor/hdpath.py` & `ape-trezor-0.6.1/ape_trezor/hdpath.py`

 * *Files identical despite different names*

### Comparing `ape-trezor-0.6.0/ape_trezor.egg-info/SOURCES.txt` & `ape-trezor-0.6.1/ape_trezor.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ape-trezor-0.6.0/ape_trezor.egg-info/requires.txt` & `ape-trezor-0.6.1/ape_trezor.egg-info/requires.txt`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-eth-ape<0.7,>=0.6.0
+eth-ape<0.7,>=0.6.9
 eth-account
 eth-typing>=3.1
 click
-trezor[ethereum]<0.14,>=0.13.5
+trezor[ethereum]<0.14,>=0.13.6
 
 [dev]
 pytest>=6.0
 pytest-xdist
 pytest-cov
 pytest-mock
 hypothesis<7.0,>=6.2.0
 eip712
-black>=22.12.0
+black>=23.3.0
 mypy>=0.991
 types-setuptools
 types-PyYAML
 flake8>=5.0.4
 isort>=5.10.1
 mdformat>=0.7.16
 mdformat-gfm>=0.3.5
@@ -34,15 +34,15 @@
 
 [doc]
 Sphinx<4,>=3.4.3
 sphinx_rtd_theme<1,>=0.1.9
 towncrier<20,>=19.2.0
 
 [lint]
-black>=22.12.0
+black>=23.3.0
 mypy>=0.991
 types-setuptools
 types-PyYAML
 flake8>=5.0.4
 isort>=5.10.1
 mdformat>=0.7.16
 mdformat-gfm>=0.3.5
```

### Comparing `ape-trezor-0.6.0/pyproject.toml` & `ape-trezor-0.6.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ape-trezor-0.6.0/setup.py` & `ape-trezor-0.6.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
         "pytest-xdist",  # multi-process runner
         "pytest-cov",  # Coverage analyzer plugin
         "pytest-mock",  # For creating mocks
         "hypothesis>=6.2.0,<7.0",  # Strategy-based fuzzer
         "eip712",  # Used for cleaner test cases
     ],
     "lint": [
-        "black>=22.12.0",  # auto-formatter and linter
+        "black>=23.3.0",  # auto-formatter and linter
         "mypy>=0.991",  # Static type analyzer
         "types-setuptools",  # Needed for mypy typeshed
         "types-PyYAML",  # Needed for mypy typeshed
         "flake8>=5.0.4",  # Style linter
         "isort>=5.10.1",  # Import sorting linter
         "mdformat>=0.7.16",  # Auto-formatter for markdown
         "mdformat-gfm>=0.3.5",  # Needed for formatting GitHub-flavored markdown
@@ -62,19 +62,19 @@
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="ApeWorX Ltd.",
     author_email="admin@apeworx.io",
     url="https://github.com/ApeWorX/ape-trezor",
     include_package_data=True,
     install_requires=[
-        "eth-ape>=0.6.0,<0.7",
+        "eth-ape>=0.6.9,<0.7",
         "eth-account",  # Use same version as eth-ape
         "eth-typing>=3.1",  # Influenced by eth-ape so no upper pin
         "click",  # Use same version as eth-ape
-        "trezor[ethereum]>=0.13.5,<0.14",
+        "trezor[ethereum]>=0.13.6,<0.14",
     ],
     entry_points={
         "ape_cli_subcommands": [
             "ape_trezor=ape_trezor._cli:cli",
         ],
     },
     python_requires=">=3.8,<4",
```

### Comparing `ape-trezor-0.6.0/tests/conftest.py` & `ape-trezor-0.6.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `ape-trezor-0.6.0/tests/test_accounts.py` & `ape-trezor-0.6.1/tests/test_accounts.py`

 * *Files identical despite different names*

### Comparing `ape-trezor-0.6.0/tests/test_choices.py` & `ape-trezor-0.6.1/tests/test_choices.py`

 * *Files identical despite different names*

### Comparing `ape-trezor-0.6.0/tests/test_cli.py` & `ape-trezor-0.6.1/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `ape-trezor-0.6.0/tests/test_client.py` & `ape-trezor-0.6.1/tests/test_client.py`

 * *Files identical despite different names*

