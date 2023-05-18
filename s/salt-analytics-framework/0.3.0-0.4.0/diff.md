# Comparing `tmp/salt-analytics-framework-0.3.0.tar.gz` & `tmp/salt-analytics-framework-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Wed May 17 22:24:55 2023, max compression
+gzip compressed data, last modified: Thu May 18 16:29:43 2023, max compression
```

## Comparing `salt-analytics-framework-0.3.0.tar` & `salt-analytics-framework-0.4.0.tar`

### file list

```diff
@@ -1,154 +1,154 @@
--rw-r--r--   0 root         (0) root         (0)       20 2023-05-17 22:24:55.000000 salt-analytics-framework-0.3.0/.bandit
--rw-r--r--   0 root         (0) root         (0)      684 2023-05-17 22:24:55.000000 salt-analytics-framework-0.3.0/.coveragerc
--rw-r--r--   0 root         (0) root         (0)        5 2023-05-17 22:24:55.000000 salt-analytics-framework-0.3.0/.dockerignore
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 22:24:55.000000 salt-analytics-framework-0.3.0/.github/
--rw-r--r--   0 root         (0) root         (0)      229 2023-05-17 22:24:55.000000 salt-analytics-framework-0.3.0/.github/actionlint.yaml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 22:24:55.000000 salt-analytics-framework-0.3.0/.github/actions/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 22:24:55.000000 salt-analytics-framework-0.3.0/.github/actions/setup-actionlint/
--rw-r--r--   0 root         (0) root         (0)      892 2023-05-17 22:24:55.000000 salt-analytics-framework-0.3.0/.github/actions/setup-actionlint/action.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 22:24:55.000000 salt-analytics-framework-0.3.0/.github/workflows/
--rw-r--r--   0 root         (0) root         (0)    10391 2023-05-17 22:24:55.000000 salt-analytics-framework-0.3.0/.github/workflows/ci.yml
--rw-r--r--   0 root         (0) root         (0)     1983 2023-05-17 22:24:55.000000 salt-analytics-framework-0.3.0/.gitignore
--rw-r--r--   0 root         (0) root         (0)     3571 2023-05-17 22:24:55.000000 salt-analytics-framework-0.3.0/.pre-commit-config.yaml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 22:24:55.000000 salt-analytics-framework-0.3.0/.pre-commit-hooks/
--rw-r--r--   0 root         (0) root         (0)     4609 2023-05-17 22:24:55.000000 salt-analytics-framework-0.3.0/.pre-commit-hooks/check-changelog-entries.py
--rw-r--r--   0 root         (0) root         (0)     2227 2023-05-17 22:24:55.000000 salt-analytics-framework-0.3.0/.pre-commit-hooks/check-cli-examples.py
--rw-r--r--   0 root         (0) root         (0)     3549 2023-05-17 22:24:55.000000 salt-analytics-framework-0.3.0/.pre-commit-hooks/copyright-headers.py
--rw-r--r--   0 root         (0) root         (0)     2092 2023-05-17 22:24:55.000000 salt-analytics-framework-0.3.0/.pre-commit-hooks/make-autodocs.py
--rw-r--r--   0 root         (0) root         (0)      579 2023-05-17 22:24:55.000000 salt-analytics-framework-0.3.0/.pre-commit-hooks/sort-pylint-spelling-words.py
--rw-r--r--   0 root         (0) root         (0)      650 2023-05-17 22:24:55.000000 salt-analytics-framework-0.3.0/.pylint-spelling-words
--rw-r--r--   0 root         (0) root         (0)     2025 2023-05-17 22:24:55.000000 salt-analytics-framework-0.3.0/CHANGELOG.rst
--rw-r--r--   0 root         (0) root         (0)     5256 2023-05-17 22:24:55.000000 salt-analytics-framework-0.3.0/CODE_OF_CONDUCT.md
--rw-r--r--   0 root         (0) root         (0)     2487 2023-05-17 22:24:55.000000 salt-analytics-framework-0.3.0/CONTRIBUTING.md
--rw-r--r--   0 root         (0) root         (0)     9283 2023-05-17 22:24:55.000000 salt-analytics-framework-0.3.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)      549 2023-05-17 22:24:55.000000 salt-analytics-framework-0.3.0/NOTICE
--rw-r--r--   0 root         (0) root         (0)     3046 2023-05-17 22:24:55.000000 salt-analytics-framework-0.3.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1861 2023-05-17 22:24:55.000000 salt-analytics-framework-0.3.0/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 22:24:55.000000 salt-analytics-framework-0.3.0/changelog/
--rw-r--r--   0 root         (0) root         (0)     1450 2023-05-17 22:24:55.000000 salt-analytics-framework-0.3.0/changelog/_template.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 22:24:55.000000 salt-analytics-framework-0.3.0/docs/
--rw-r--r--   0 root         (0) root         (0)      634 2023-05-17 22:24:55.000000 salt-analytics-framework-0.3.0/docs/Makefile
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 22:24:55.000000 salt-analytics-framework-0.3.0/docs/_static/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-17 22:24:55.000000 salt-analytics-framework-0.3.0/docs/_static/.gitkeep
--rw-r--r--   0 root         (0) root         (0)      164 2023-05-17 22:24:55.000000 salt-analytics-framework-0.3.0/docs/all.rst
--rw-r--r--   0 root         (0) root         (0)       30 2023-05-17 22:24:55.000000 salt-analytics-framework-0.3.0/docs/changelog.rst
--rw-r--r--   0 root         (0) root         (0)     6553 2023-05-17 22:24:55.000000 salt-analytics-framework-0.3.0/docs/conf.py
--rw-r--r--   0 root         (0) root         (0)      200 2023-05-17 22:24:55.000000 salt-analytics-framework-0.3.0/docs/contents.rst
--rw-r--r--   0 root         (0) root         (0)      720 2023-05-17 22:24:55.000000 salt-analytics-framework-0.3.0/docs/index.rst
--rw-r--r--   0 root         (0) root         (0)      760 2023-05-17 22:24:55.000000 salt-analytics-framework-0.3.0/docs/make.bat
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 22:24:55.000000 salt-analytics-framework-0.3.0/docs/ref/
--rw-r--r--   0 root         (0) root         (0)       46 2023-05-17 22:24:55.000000 salt-analytics-framework-0.3.0/docs/ref/modules.rst
--rw-r--r--   0 root         (0) root         (0)      720 2023-05-17 22:24:55.000000 salt-analytics-framework-0.3.0/docs/ref/saf.collect.rst
--rw-r--r--   0 root         (0) root         (0)      557 2023-05-17 22:24:55.000000 salt-analytics-framework-0.3.0/docs/ref/saf.forward.rst
--rw-r--r--   0 root         (0) root         (0)      603 2023-05-17 22:24:55.000000 salt-analytics-framework-0.3.0/docs/ref/saf.process.rst
--rw-r--r--   0 root         (0) root         (0)      861 2023-05-17 22:24:55.000000 salt-analytics-framework-0.3.0/docs/ref/saf.rst
--rw-r--r--   0 root         (0) root         (0)      346 2023-05-17 22:24:55.000000 salt-analytics-framework-0.3.0/docs/ref/saf.saltext.engines.rst
--rw-r--r--   0 root         (0) root         (0)      202 2023-05-17 22:24:55.000000 salt-analytics-framework-0.3.0/docs/ref/saf.saltext.rst
--rw-r--r--   0 root         (0) root         (0)      408 2023-05-17 22:24:55.000000 salt-analytics-framework-0.3.0/docs/ref/saf.utils.rst
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-17 22:24:55.000000 salt-analytics-framework-0.3.0/docs/sitevars.rst
--rw-r--r--   0 root         (0) root         (0)    20016 2023-05-17 22:24:55.000000 salt-analytics-framework-0.3.0/noxfile.py
--rw-r--r--   0 root         (0) root         (0)     4837 2023-05-17 22:24:55.000000 salt-analytics-framework-0.3.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)      428 2023-05-17 22:24:55.000000 salt-analytics-framework-0.3.0/pytest.ini
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 22:24:55.000000 salt-analytics-framework-0.3.0/requirements/
--rw-r--r--   0 root         (0) root         (0)      113 2023-05-17 22:24:55.000000 salt-analytics-framework-0.3.0/requirements/base.txt
--rw-r--r--   0 root         (0) root         (0)       19 2023-05-17 22:24:55.000000 salt-analytics-framework-0.3.0/requirements/build.txt
--rw-r--r--   0 root         (0) root         (0)       21 2023-05-17 22:24:55.000000 salt-analytics-framework-0.3.0/requirements/changelog.txt
--rw-r--r--   0 root         (0) root         (0)      188 2023-05-17 22:24:55.000000 salt-analytics-framework-0.3.0/requirements/dev.txt
--rw-r--r--   0 root         (0) root         (0)       17 2023-05-17 22:24:55.000000 salt-analytics-framework-0.3.0/requirements/docs-auto.txt
--rw-r--r--   0 root         (0) root         (0)      148 2023-05-17 22:24:55.000000 salt-analytics-framework-0.3.0/requirements/docs.txt
--rw-r--r--   0 root         (0) root         (0)       74 2023-05-17 22:24:55.000000 salt-analytics-framework-0.3.0/requirements/tests.txt
--rw-r--r--   0 root         (0) root         (0)       31 2023-05-17 22:24:55.000000 salt-analytics-framework-0.3.0/requirements/tools.txt
--rw-r--r--   0 root         (0) root         (0)     3170 2023-05-17 22:24:55.000000 salt-analytics-framework-0.3.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      198 2023-05-17 22:24:55.000000 salt-analytics-framework-0.3.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 22:24:55.000000 salt-analytics-framework-0.3.0/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 22:24:55.000000 salt-analytics-framework-0.3.0/src/saf/
--rw-r--r--   0 root         (0) root         (0)      914 2023-05-17 22:24:55.000000 salt-analytics-framework-0.3.0/src/saf/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 22:24:55.000000 salt-analytics-framework-0.3.0/src/saf/collect/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-17 22:24:55.000000 salt-analytics-framework-0.3.0/src/saf/collect/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2618 2023-05-17 22:24:55.000000 salt-analytics-framework-0.3.0/src/saf/collect/beacons.py
--rw-r--r--   0 root         (0) root         (0)     2190 2023-05-17 22:24:55.000000 salt-analytics-framework-0.3.0/src/saf/collect/file.py
--rw-r--r--   0 root         (0) root         (0)     1126 2023-05-17 22:24:55.000000 salt-analytics-framework-0.3.0/src/saf/collect/noop.py
--rw-r--r--   0 root         (0) root         (0)     1472 2023-05-17 22:24:55.000000 salt-analytics-framework-0.3.0/src/saf/collect/salt_exec.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 22:24:55.000000 salt-analytics-framework-0.3.0/src/saf/forward/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-17 22:24:55.000000 salt-analytics-framework-0.3.0/src/saf/forward/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1560 2023-05-17 22:24:55.000000 salt-analytics-framework-0.3.0/src/saf/forward/disk.py
--rw-r--r--   0 root         (0) root         (0)      797 2023-05-17 22:24:55.000000 salt-analytics-framework-0.3.0/src/saf/forward/noop.py
--rw-r--r--   0 root         (0) root         (0)     1825 2023-05-17 22:24:55.000000 salt-analytics-framework-0.3.0/src/saf/forward/test.py
--rw-r--r--   0 root         (0) root         (0)     3085 2023-05-17 22:24:55.000000 salt-analytics-framework-0.3.0/src/saf/manager.py
--rw-r--r--   0 root         (0) root         (0)    10262 2023-05-17 22:24:55.000000 salt-analytics-framework-0.3.0/src/saf/models.py
--rw-r--r--   0 root         (0) root         (0)     6800 2023-05-17 22:24:55.000000 salt-analytics-framework-0.3.0/src/saf/pipeline.py
--rw-r--r--   0 root         (0) root         (0)     2791 2023-05-17 22:24:55.000000 salt-analytics-framework-0.3.0/src/saf/plugins.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 22:24:55.000000 salt-analytics-framework-0.3.0/src/saf/process/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-17 22:24:55.000000 salt-analytics-framework-0.3.0/src/saf/process/__init__.py
--rw-r--r--   0 root         (0) root         (0)      872 2023-05-17 22:24:55.000000 salt-analytics-framework-0.3.0/src/saf/process/noop.py
--rw-r--r--   0 root         (0) root         (0)     3194 2023-05-17 22:24:55.000000 salt-analytics-framework-0.3.0/src/saf/process/regex_mask.py
--rw-r--r--   0 root         (0) root         (0)      594 2023-05-17 22:24:55.000000 salt-analytics-framework-0.3.0/src/saf/process/regex_mask.pyi
--rw-r--r--   0 root         (0) root         (0)     4489 2023-05-17 22:24:55.000000 salt-analytics-framework-0.3.0/src/saf/process/shannon_mask.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-17 22:24:55.000000 salt-analytics-framework-0.3.0/src/saf/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 22:24:55.000000 salt-analytics-framework-0.3.0/src/saf/saltext/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-17 22:24:55.000000 salt-analytics-framework-0.3.0/src/saf/saltext/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 22:24:55.000000 salt-analytics-framework-0.3.0/src/saf/saltext/engines/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-17 22:24:55.000000 salt-analytics-framework-0.3.0/src/saf/saltext/engines/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2116 2023-05-17 22:24:55.000000 salt-analytics-framework-0.3.0/src/saf/saltext/engines/analytics.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 22:24:55.000000 salt-analytics-framework-0.3.0/src/saf/utils/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-17 22:24:55.000000 salt-analytics-framework-0.3.0/src/saf/utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)      362 2023-05-17 22:24:55.000000 salt-analytics-framework-0.3.0/src/saf/utils/dt.py
--rw-r--r--   0 root         (0) root         (0)     5542 2023-05-17 22:24:55.000000 salt-analytics-framework-0.3.0/src/saf/utils/eventbus.py
--rw-r--r--   0 root         (0) root         (0)       42 2023-05-17 22:24:55.000000 salt-analytics-framework-0.3.0/src/saf/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 22:24:55.000000 salt-analytics-framework-0.3.0/src/salt_analytics_framework.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3046 2023-05-17 22:24:55.000000 salt-analytics-framework-0.3.0/src/salt_analytics_framework.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3417 2023-05-17 22:24:55.000000 salt-analytics-framework-0.3.0/src/salt_analytics_framework.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-17 22:24:55.000000 salt-analytics-framework-0.3.0/src/salt_analytics_framework.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      382 2023-05-17 22:24:55.000000 salt-analytics-framework-0.3.0/src/salt_analytics_framework.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-17 22:24:55.000000 salt-analytics-framework-0.3.0/src/salt_analytics_framework.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      586 2023-05-17 22:24:55.000000 salt-analytics-framework-0.3.0/src/salt_analytics_framework.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        4 2023-05-17 22:24:55.000000 salt-analytics-framework-0.3.0/src/salt_analytics_framework.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 22:24:55.000000 salt-analytics-framework-0.3.0/tests/
--rw-r--r--   0 root         (0) root         (0)      738 2023-05-17 22:24:55.000000 salt-analytics-framework-0.3.0/tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1497 2023-05-17 22:24:55.000000 salt-analytics-framework-0.3.0/tests/conftest.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 22:24:55.000000 salt-analytics-framework-0.3.0/tests/functional/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-17 22:24:55.000000 salt-analytics-framework-0.3.0/tests/functional/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1207 2023-05-17 22:24:55.000000 salt-analytics-framework-0.3.0/tests/functional/conftest.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 22:24:55.000000 salt-analytics-framework-0.3.0/tests/functional/forwarders/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-17 22:24:55.000000 salt-analytics-framework-0.3.0/tests/functional/forwarders/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2303 2023-05-17 22:24:55.000000 salt-analytics-framework-0.3.0/tests/functional/forwarders/test_concurrency.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 22:24:55.000000 salt-analytics-framework-0.3.0/tests/functional/manager/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-17 22:24:55.000000 salt-analytics-framework-0.3.0/tests/functional/manager/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1763 2023-05-17 22:24:55.000000 salt-analytics-framework-0.3.0/tests/functional/manager/conftest.py
--rw-r--r--   0 root         (0) root         (0)     1063 2023-05-17 22:24:55.000000 salt-analytics-framework-0.3.0/tests/functional/manager/test_disabled_pipeline.py
--rw-r--r--   0 root         (0) root         (0)     1211 2023-05-17 22:24:55.000000 salt-analytics-framework-0.3.0/tests/functional/manager/test_enabled_pipeline.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 22:24:55.000000 salt-analytics-framework-0.3.0/tests/integration/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-17 22:24:55.000000 salt-analytics-framework-0.3.0/tests/integration/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 22:24:55.000000 salt-analytics-framework-0.3.0/tests/integration/collectors/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-17 22:24:55.000000 salt-analytics-framework-0.3.0/tests/integration/collectors/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 22:24:55.000000 salt-analytics-framework-0.3.0/tests/integration/collectors/beacons/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-17 22:24:55.000000 salt-analytics-framework-0.3.0/tests/integration/collectors/beacons/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1967 2023-05-17 22:24:55.000000 salt-analytics-framework-0.3.0/tests/integration/collectors/beacons/test_memusage.py
--rw-r--r--   0 root         (0) root         (0)     2119 2023-05-17 22:24:55.000000 salt-analytics-framework-0.3.0/tests/integration/collectors/beacons/test_multiple.py
--rw-r--r--   0 root         (0) root         (0)     1982 2023-05-17 22:24:55.000000 salt-analytics-framework-0.3.0/tests/integration/collectors/beacons/test_status.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 22:24:55.000000 salt-analytics-framework-0.3.0/tests/integration/collectors/salt_exec/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-17 22:24:55.000000 salt-analytics-framework-0.3.0/tests/integration/collectors/salt_exec/__init__.py
--rw-r--r--   0 root         (0) root         (0)      775 2023-05-17 22:24:55.000000 salt-analytics-framework-0.3.0/tests/integration/collectors/salt_exec/conftest.py
--rw-r--r--   0 root         (0) root         (0)     1734 2023-05-17 22:24:55.000000 salt-analytics-framework-0.3.0/tests/integration/collectors/salt_exec/test_arg.py
--rw-r--r--   0 root         (0) root         (0)     1563 2023-05-17 22:24:55.000000 salt-analytics-framework-0.3.0/tests/integration/collectors/salt_exec/test_collatz.py
--rw-r--r--   0 root         (0) root         (0)     1556 2023-05-17 22:24:55.000000 salt-analytics-framework-0.3.0/tests/integration/collectors/salt_exec/test_config_get.py
--rw-r--r--   0 root         (0) root         (0)     1399 2023-05-17 22:24:55.000000 salt-analytics-framework-0.3.0/tests/integration/conftest.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 22:24:55.000000 salt-analytics-framework-0.3.0/tests/integration/engines/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-17 22:24:55.000000 salt-analytics-framework-0.3.0/tests/integration/engines/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1517 2023-05-17 22:24:55.000000 salt-analytics-framework-0.3.0/tests/integration/engines/test_engine.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 22:24:55.000000 salt-analytics-framework-0.3.0/tests/unit/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-17 22:24:55.000000 salt-analytics-framework-0.3.0/tests/unit/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 22:24:55.000000 salt-analytics-framework-0.3.0/tests/unit/process/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-17 22:24:55.000000 salt-analytics-framework-0.3.0/tests/unit/process/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3803 2023-05-17 22:24:55.000000 salt-analytics-framework-0.3.0/tests/unit/process/test_regex_mask.py
--rw-r--r--   0 root         (0) root         (0)     5436 2023-05-17 22:24:55.000000 salt-analytics-framework-0.3.0/tests/unit/process/test_shannon_mask.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 22:24:55.000000 salt-analytics-framework-0.3.0/tests/unit/salt/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-17 22:24:55.000000 salt-analytics-framework-0.3.0/tests/unit/salt/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 22:24:55.000000 salt-analytics-framework-0.3.0/tests/unit/salt/engines/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-17 22:24:55.000000 salt-analytics-framework-0.3.0/tests/unit/salt/engines/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 22:24:55.000000 salt-analytics-framework-0.3.0/tools/
--rw-r--r--   0 root         (0) root         (0)       89 2023-05-17 22:24:55.000000 salt-analytics-framework-0.3.0/tools/.ruff.toml
--rw-r--r--   0 root         (0) root         (0)      334 2023-05-17 22:24:55.000000 salt-analytics-framework-0.3.0/tools/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5495 2023-05-17 22:24:55.000000 salt-analytics-framework-0.3.0/tools/ci.py
--rw-r--r--   0 root         (0) root         (0)     1383 2023-05-17 22:24:55.000000 salt-analytics-framework-0.3.0/tools/pre_commit.py
--rw-r--r--   0 root         (0) root         (0)     1382 2023-05-17 22:24:55.000000 salt-analytics-framework-0.3.0/tools/pre_commit.py~
+-rw-r--r--   0 root         (0) root         (0)       20 2023-05-18 16:29:43.000000 salt-analytics-framework-0.4.0/.bandit
+-rw-r--r--   0 root         (0) root         (0)      684 2023-05-18 16:29:43.000000 salt-analytics-framework-0.4.0/.coveragerc
+-rw-r--r--   0 root         (0) root         (0)        5 2023-05-18 16:29:43.000000 salt-analytics-framework-0.4.0/.dockerignore
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 16:29:43.000000 salt-analytics-framework-0.4.0/.github/
+-rw-r--r--   0 root         (0) root         (0)      229 2023-05-18 16:29:43.000000 salt-analytics-framework-0.4.0/.github/actionlint.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 16:29:43.000000 salt-analytics-framework-0.4.0/.github/actions/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 16:29:43.000000 salt-analytics-framework-0.4.0/.github/actions/setup-actionlint/
+-rw-r--r--   0 root         (0) root         (0)      892 2023-05-18 16:29:43.000000 salt-analytics-framework-0.4.0/.github/actions/setup-actionlint/action.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 16:29:43.000000 salt-analytics-framework-0.4.0/.github/workflows/
+-rw-r--r--   0 root         (0) root         (0)    10391 2023-05-18 16:29:43.000000 salt-analytics-framework-0.4.0/.github/workflows/ci.yml
+-rw-r--r--   0 root         (0) root         (0)     1983 2023-05-18 16:29:43.000000 salt-analytics-framework-0.4.0/.gitignore
+-rw-r--r--   0 root         (0) root         (0)     3674 2023-05-18 16:29:43.000000 salt-analytics-framework-0.4.0/.pre-commit-config.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 16:29:43.000000 salt-analytics-framework-0.4.0/.pre-commit-hooks/
+-rw-r--r--   0 root         (0) root         (0)     4609 2023-05-18 16:29:43.000000 salt-analytics-framework-0.4.0/.pre-commit-hooks/check-changelog-entries.py
+-rw-r--r--   0 root         (0) root         (0)     2227 2023-05-18 16:29:43.000000 salt-analytics-framework-0.4.0/.pre-commit-hooks/check-cli-examples.py
+-rw-r--r--   0 root         (0) root         (0)     3549 2023-05-18 16:29:43.000000 salt-analytics-framework-0.4.0/.pre-commit-hooks/copyright-headers.py
+-rw-r--r--   0 root         (0) root         (0)     2092 2023-05-18 16:29:43.000000 salt-analytics-framework-0.4.0/.pre-commit-hooks/make-autodocs.py
+-rw-r--r--   0 root         (0) root         (0)      579 2023-05-18 16:29:43.000000 salt-analytics-framework-0.4.0/.pre-commit-hooks/sort-pylint-spelling-words.py
+-rw-r--r--   0 root         (0) root         (0)      650 2023-05-18 16:29:43.000000 salt-analytics-framework-0.4.0/.pylint-spelling-words
+-rw-r--r--   0 root         (0) root         (0)     2665 2023-05-18 16:29:43.000000 salt-analytics-framework-0.4.0/CHANGELOG.rst
+-rw-r--r--   0 root         (0) root         (0)     5256 2023-05-18 16:29:43.000000 salt-analytics-framework-0.4.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0 root         (0) root         (0)     2487 2023-05-18 16:29:43.000000 salt-analytics-framework-0.4.0/CONTRIBUTING.md
+-rw-r--r--   0 root         (0) root         (0)     9283 2023-05-18 16:29:43.000000 salt-analytics-framework-0.4.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      549 2023-05-18 16:29:43.000000 salt-analytics-framework-0.4.0/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     3046 2023-05-18 16:29:43.000000 salt-analytics-framework-0.4.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1861 2023-05-18 16:29:43.000000 salt-analytics-framework-0.4.0/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 16:29:43.000000 salt-analytics-framework-0.4.0/changelog/
+-rw-r--r--   0 root         (0) root         (0)     1450 2023-05-18 16:29:43.000000 salt-analytics-framework-0.4.0/changelog/_template.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 16:29:43.000000 salt-analytics-framework-0.4.0/docs/
+-rw-r--r--   0 root         (0) root         (0)      634 2023-05-18 16:29:43.000000 salt-analytics-framework-0.4.0/docs/Makefile
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 16:29:43.000000 salt-analytics-framework-0.4.0/docs/_static/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 16:29:43.000000 salt-analytics-framework-0.4.0/docs/_static/.gitkeep
+-rw-r--r--   0 root         (0) root         (0)      164 2023-05-18 16:29:43.000000 salt-analytics-framework-0.4.0/docs/all.rst
+-rw-r--r--   0 root         (0) root         (0)       30 2023-05-18 16:29:43.000000 salt-analytics-framework-0.4.0/docs/changelog.rst
+-rw-r--r--   0 root         (0) root         (0)     6553 2023-05-18 16:29:43.000000 salt-analytics-framework-0.4.0/docs/conf.py
+-rw-r--r--   0 root         (0) root         (0)      200 2023-05-18 16:29:43.000000 salt-analytics-framework-0.4.0/docs/contents.rst
+-rw-r--r--   0 root         (0) root         (0)      720 2023-05-18 16:29:43.000000 salt-analytics-framework-0.4.0/docs/index.rst
+-rw-r--r--   0 root         (0) root         (0)      760 2023-05-18 16:29:43.000000 salt-analytics-framework-0.4.0/docs/make.bat
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 16:29:43.000000 salt-analytics-framework-0.4.0/docs/ref/
+-rw-r--r--   0 root         (0) root         (0)       46 2023-05-18 16:29:43.000000 salt-analytics-framework-0.4.0/docs/ref/modules.rst
+-rw-r--r--   0 root         (0) root         (0)      720 2023-05-18 16:29:43.000000 salt-analytics-framework-0.4.0/docs/ref/saf.collect.rst
+-rw-r--r--   0 root         (0) root         (0)      557 2023-05-18 16:29:43.000000 salt-analytics-framework-0.4.0/docs/ref/saf.forward.rst
+-rw-r--r--   0 root         (0) root         (0)      603 2023-05-18 16:29:43.000000 salt-analytics-framework-0.4.0/docs/ref/saf.process.rst
+-rw-r--r--   0 root         (0) root         (0)      861 2023-05-18 16:29:43.000000 salt-analytics-framework-0.4.0/docs/ref/saf.rst
+-rw-r--r--   0 root         (0) root         (0)      346 2023-05-18 16:29:43.000000 salt-analytics-framework-0.4.0/docs/ref/saf.saltext.engines.rst
+-rw-r--r--   0 root         (0) root         (0)      202 2023-05-18 16:29:43.000000 salt-analytics-framework-0.4.0/docs/ref/saf.saltext.rst
+-rw-r--r--   0 root         (0) root         (0)      408 2023-05-18 16:29:43.000000 salt-analytics-framework-0.4.0/docs/ref/saf.utils.rst
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 16:29:43.000000 salt-analytics-framework-0.4.0/docs/sitevars.rst
+-rw-r--r--   0 root         (0) root         (0)    20016 2023-05-18 16:29:43.000000 salt-analytics-framework-0.4.0/noxfile.py
+-rw-r--r--   0 root         (0) root         (0)     4837 2023-05-18 16:29:43.000000 salt-analytics-framework-0.4.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)      428 2023-05-18 16:29:43.000000 salt-analytics-framework-0.4.0/pytest.ini
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 16:29:43.000000 salt-analytics-framework-0.4.0/requirements/
+-rw-r--r--   0 root         (0) root         (0)      176 2023-05-18 16:29:43.000000 salt-analytics-framework-0.4.0/requirements/base.txt
+-rw-r--r--   0 root         (0) root         (0)       19 2023-05-18 16:29:43.000000 salt-analytics-framework-0.4.0/requirements/build.txt
+-rw-r--r--   0 root         (0) root         (0)       21 2023-05-18 16:29:43.000000 salt-analytics-framework-0.4.0/requirements/changelog.txt
+-rw-r--r--   0 root         (0) root         (0)      188 2023-05-18 16:29:43.000000 salt-analytics-framework-0.4.0/requirements/dev.txt
+-rw-r--r--   0 root         (0) root         (0)       17 2023-05-18 16:29:43.000000 salt-analytics-framework-0.4.0/requirements/docs-auto.txt
+-rw-r--r--   0 root         (0) root         (0)      148 2023-05-18 16:29:43.000000 salt-analytics-framework-0.4.0/requirements/docs.txt
+-rw-r--r--   0 root         (0) root         (0)       74 2023-05-18 16:29:43.000000 salt-analytics-framework-0.4.0/requirements/tests.txt
+-rw-r--r--   0 root         (0) root         (0)       31 2023-05-18 16:29:43.000000 salt-analytics-framework-0.4.0/requirements/tools.txt
+-rw-r--r--   0 root         (0) root         (0)     3170 2023-05-18 16:29:43.000000 salt-analytics-framework-0.4.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      198 2023-05-18 16:29:43.000000 salt-analytics-framework-0.4.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 16:29:43.000000 salt-analytics-framework-0.4.0/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 16:29:43.000000 salt-analytics-framework-0.4.0/src/saf/
+-rw-r--r--   0 root         (0) root         (0)      914 2023-05-18 16:29:43.000000 salt-analytics-framework-0.4.0/src/saf/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 16:29:43.000000 salt-analytics-framework-0.4.0/src/saf/collect/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 16:29:43.000000 salt-analytics-framework-0.4.0/src/saf/collect/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2618 2023-05-18 16:29:43.000000 salt-analytics-framework-0.4.0/src/saf/collect/beacons.py
+-rw-r--r--   0 root         (0) root         (0)     3082 2023-05-18 16:29:43.000000 salt-analytics-framework-0.4.0/src/saf/collect/file.py
+-rw-r--r--   0 root         (0) root         (0)     1127 2023-05-18 16:29:43.000000 salt-analytics-framework-0.4.0/src/saf/collect/noop.py
+-rw-r--r--   0 root         (0) root         (0)     1473 2023-05-18 16:29:43.000000 salt-analytics-framework-0.4.0/src/saf/collect/salt_exec.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 16:29:43.000000 salt-analytics-framework-0.4.0/src/saf/forward/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 16:29:43.000000 salt-analytics-framework-0.4.0/src/saf/forward/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1691 2023-05-18 16:29:43.000000 salt-analytics-framework-0.4.0/src/saf/forward/disk.py
+-rw-r--r--   0 root         (0) root         (0)      798 2023-05-18 16:29:43.000000 salt-analytics-framework-0.4.0/src/saf/forward/noop.py
+-rw-r--r--   0 root         (0) root         (0)     1825 2023-05-18 16:29:43.000000 salt-analytics-framework-0.4.0/src/saf/forward/test.py
+-rw-r--r--   0 root         (0) root         (0)     3085 2023-05-18 16:29:43.000000 salt-analytics-framework-0.4.0/src/saf/manager.py
+-rw-r--r--   0 root         (0) root         (0)    10262 2023-05-18 16:29:43.000000 salt-analytics-framework-0.4.0/src/saf/models.py
+-rw-r--r--   0 root         (0) root         (0)     6800 2023-05-18 16:29:43.000000 salt-analytics-framework-0.4.0/src/saf/pipeline.py
+-rw-r--r--   0 root         (0) root         (0)     2791 2023-05-18 16:29:43.000000 salt-analytics-framework-0.4.0/src/saf/plugins.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 16:29:43.000000 salt-analytics-framework-0.4.0/src/saf/process/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 16:29:43.000000 salt-analytics-framework-0.4.0/src/saf/process/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      873 2023-05-18 16:29:43.000000 salt-analytics-framework-0.4.0/src/saf/process/noop.py
+-rw-r--r--   0 root         (0) root         (0)     3195 2023-05-18 16:29:43.000000 salt-analytics-framework-0.4.0/src/saf/process/regex_mask.py
+-rw-r--r--   0 root         (0) root         (0)      594 2023-05-18 16:29:43.000000 salt-analytics-framework-0.4.0/src/saf/process/regex_mask.pyi
+-rw-r--r--   0 root         (0) root         (0)     4490 2023-05-18 16:29:43.000000 salt-analytics-framework-0.4.0/src/saf/process/shannon_mask.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 16:29:43.000000 salt-analytics-framework-0.4.0/src/saf/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 16:29:43.000000 salt-analytics-framework-0.4.0/src/saf/saltext/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 16:29:43.000000 salt-analytics-framework-0.4.0/src/saf/saltext/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 16:29:43.000000 salt-analytics-framework-0.4.0/src/saf/saltext/engines/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 16:29:43.000000 salt-analytics-framework-0.4.0/src/saf/saltext/engines/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2165 2023-05-18 16:29:43.000000 salt-analytics-framework-0.4.0/src/saf/saltext/engines/analytics.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 16:29:43.000000 salt-analytics-framework-0.4.0/src/saf/utils/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 16:29:43.000000 salt-analytics-framework-0.4.0/src/saf/utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      362 2023-05-18 16:29:43.000000 salt-analytics-framework-0.4.0/src/saf/utils/dt.py
+-rw-r--r--   0 root         (0) root         (0)     5542 2023-05-18 16:29:43.000000 salt-analytics-framework-0.4.0/src/saf/utils/eventbus.py
+-rw-r--r--   0 root         (0) root         (0)       42 2023-05-18 16:29:43.000000 salt-analytics-framework-0.4.0/src/saf/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 16:29:43.000000 salt-analytics-framework-0.4.0/src/salt_analytics_framework.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3046 2023-05-18 16:29:43.000000 salt-analytics-framework-0.4.0/src/salt_analytics_framework.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3417 2023-05-18 16:29:43.000000 salt-analytics-framework-0.4.0/src/salt_analytics_framework.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-18 16:29:43.000000 salt-analytics-framework-0.4.0/src/salt_analytics_framework.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      382 2023-05-18 16:29:43.000000 salt-analytics-framework-0.4.0/src/salt_analytics_framework.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-18 16:29:43.000000 salt-analytics-framework-0.4.0/src/salt_analytics_framework.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      652 2023-05-18 16:29:43.000000 salt-analytics-framework-0.4.0/src/salt_analytics_framework.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        4 2023-05-18 16:29:43.000000 salt-analytics-framework-0.4.0/src/salt_analytics_framework.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 16:29:43.000000 salt-analytics-framework-0.4.0/tests/
+-rw-r--r--   0 root         (0) root         (0)      738 2023-05-18 16:29:43.000000 salt-analytics-framework-0.4.0/tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1497 2023-05-18 16:29:43.000000 salt-analytics-framework-0.4.0/tests/conftest.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 16:29:43.000000 salt-analytics-framework-0.4.0/tests/functional/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 16:29:43.000000 salt-analytics-framework-0.4.0/tests/functional/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1207 2023-05-18 16:29:43.000000 salt-analytics-framework-0.4.0/tests/functional/conftest.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 16:29:43.000000 salt-analytics-framework-0.4.0/tests/functional/forwarders/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 16:29:43.000000 salt-analytics-framework-0.4.0/tests/functional/forwarders/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2303 2023-05-18 16:29:43.000000 salt-analytics-framework-0.4.0/tests/functional/forwarders/test_concurrency.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 16:29:43.000000 salt-analytics-framework-0.4.0/tests/functional/manager/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 16:29:43.000000 salt-analytics-framework-0.4.0/tests/functional/manager/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1763 2023-05-18 16:29:43.000000 salt-analytics-framework-0.4.0/tests/functional/manager/conftest.py
+-rw-r--r--   0 root         (0) root         (0)     1063 2023-05-18 16:29:43.000000 salt-analytics-framework-0.4.0/tests/functional/manager/test_disabled_pipeline.py
+-rw-r--r--   0 root         (0) root         (0)     1211 2023-05-18 16:29:43.000000 salt-analytics-framework-0.4.0/tests/functional/manager/test_enabled_pipeline.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 16:29:43.000000 salt-analytics-framework-0.4.0/tests/integration/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 16:29:43.000000 salt-analytics-framework-0.4.0/tests/integration/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 16:29:43.000000 salt-analytics-framework-0.4.0/tests/integration/collectors/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 16:29:43.000000 salt-analytics-framework-0.4.0/tests/integration/collectors/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 16:29:43.000000 salt-analytics-framework-0.4.0/tests/integration/collectors/beacons/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 16:29:43.000000 salt-analytics-framework-0.4.0/tests/integration/collectors/beacons/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1967 2023-05-18 16:29:43.000000 salt-analytics-framework-0.4.0/tests/integration/collectors/beacons/test_memusage.py
+-rw-r--r--   0 root         (0) root         (0)     2119 2023-05-18 16:29:43.000000 salt-analytics-framework-0.4.0/tests/integration/collectors/beacons/test_multiple.py
+-rw-r--r--   0 root         (0) root         (0)     1982 2023-05-18 16:29:43.000000 salt-analytics-framework-0.4.0/tests/integration/collectors/beacons/test_status.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 16:29:43.000000 salt-analytics-framework-0.4.0/tests/integration/collectors/salt_exec/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 16:29:43.000000 salt-analytics-framework-0.4.0/tests/integration/collectors/salt_exec/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      775 2023-05-18 16:29:43.000000 salt-analytics-framework-0.4.0/tests/integration/collectors/salt_exec/conftest.py
+-rw-r--r--   0 root         (0) root         (0)     1734 2023-05-18 16:29:43.000000 salt-analytics-framework-0.4.0/tests/integration/collectors/salt_exec/test_arg.py
+-rw-r--r--   0 root         (0) root         (0)     1563 2023-05-18 16:29:43.000000 salt-analytics-framework-0.4.0/tests/integration/collectors/salt_exec/test_collatz.py
+-rw-r--r--   0 root         (0) root         (0)     1556 2023-05-18 16:29:43.000000 salt-analytics-framework-0.4.0/tests/integration/collectors/salt_exec/test_config_get.py
+-rw-r--r--   0 root         (0) root         (0)     1399 2023-05-18 16:29:43.000000 salt-analytics-framework-0.4.0/tests/integration/conftest.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 16:29:43.000000 salt-analytics-framework-0.4.0/tests/integration/engines/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 16:29:43.000000 salt-analytics-framework-0.4.0/tests/integration/engines/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1517 2023-05-18 16:29:43.000000 salt-analytics-framework-0.4.0/tests/integration/engines/test_engine.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 16:29:43.000000 salt-analytics-framework-0.4.0/tests/unit/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 16:29:43.000000 salt-analytics-framework-0.4.0/tests/unit/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 16:29:43.000000 salt-analytics-framework-0.4.0/tests/unit/process/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 16:29:43.000000 salt-analytics-framework-0.4.0/tests/unit/process/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3803 2023-05-18 16:29:43.000000 salt-analytics-framework-0.4.0/tests/unit/process/test_regex_mask.py
+-rw-r--r--   0 root         (0) root         (0)     5436 2023-05-18 16:29:43.000000 salt-analytics-framework-0.4.0/tests/unit/process/test_shannon_mask.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 16:29:43.000000 salt-analytics-framework-0.4.0/tests/unit/salt/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 16:29:43.000000 salt-analytics-framework-0.4.0/tests/unit/salt/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 16:29:43.000000 salt-analytics-framework-0.4.0/tests/unit/salt/engines/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 16:29:43.000000 salt-analytics-framework-0.4.0/tests/unit/salt/engines/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 16:29:43.000000 salt-analytics-framework-0.4.0/tools/
+-rw-r--r--   0 root         (0) root         (0)       89 2023-05-18 16:29:43.000000 salt-analytics-framework-0.4.0/tools/.ruff.toml
+-rw-r--r--   0 root         (0) root         (0)      334 2023-05-18 16:29:43.000000 salt-analytics-framework-0.4.0/tools/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5495 2023-05-18 16:29:43.000000 salt-analytics-framework-0.4.0/tools/ci.py
+-rw-r--r--   0 root         (0) root         (0)     1383 2023-05-18 16:29:43.000000 salt-analytics-framework-0.4.0/tools/pre_commit.py
+-rw-r--r--   0 root         (0) root         (0)     1382 2023-05-18 16:29:43.000000 salt-analytics-framework-0.4.0/tools/pre_commit.py~
```

### Comparing `salt-analytics-framework-0.3.0/.coveragerc` & `salt-analytics-framework-0.4.0/.coveragerc`

 * *Files identical despite different names*

### Comparing `salt-analytics-framework-0.3.0/.github/actions/setup-actionlint/action.yml` & `salt-analytics-framework-0.4.0/.github/actions/setup-actionlint/action.yml`

 * *Files identical despite different names*

### Comparing `salt-analytics-framework-0.3.0/.github/workflows/ci.yml` & `salt-analytics-framework-0.4.0/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `salt-analytics-framework-0.3.0/.gitignore` & `salt-analytics-framework-0.4.0/.gitignore`

 * *Files identical despite different names*

### Comparing `salt-analytics-framework-0.3.0/.pre-commit-config.yaml` & `salt-analytics-framework-0.4.0/.pre-commit-config.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -102,8 +102,11 @@
         name: Run mypy against the code base
         files: ^(src/|tests/).*\.py$
         args: []
         additional_dependencies:
           - types-attrs
           - types-setuptools
           - pydantic
+          - types-aiofiles
+          - aiostream
+          - typing-extensions; python_version < "3.9"
   # <---- Code Formatting and Analysis -----------------------------------------------------------
```

### Comparing `salt-analytics-framework-0.3.0/.pre-commit-hooks/check-changelog-entries.py` & `salt-analytics-framework-0.4.0/.pre-commit-hooks/check-changelog-entries.py`

 * *Files identical despite different names*

### Comparing `salt-analytics-framework-0.3.0/.pre-commit-hooks/check-cli-examples.py` & `salt-analytics-framework-0.4.0/.pre-commit-hooks/check-cli-examples.py`

 * *Files identical despite different names*

### Comparing `salt-analytics-framework-0.3.0/.pre-commit-hooks/copyright-headers.py` & `salt-analytics-framework-0.4.0/.pre-commit-hooks/copyright-headers.py`

 * *Files identical despite different names*

### Comparing `salt-analytics-framework-0.3.0/.pre-commit-hooks/make-autodocs.py` & `salt-analytics-framework-0.4.0/.pre-commit-hooks/make-autodocs.py`

 * *Files identical despite different names*

### Comparing `salt-analytics-framework-0.3.0/.pre-commit-hooks/sort-pylint-spelling-words.py` & `salt-analytics-framework-0.4.0/.pre-commit-hooks/sort-pylint-spelling-words.py`

 * *Files identical despite different names*

### Comparing `salt-analytics-framework-0.3.0/.pylint-spelling-words` & `salt-analytics-framework-0.4.0/.pylint-spelling-words`

 * *Files identical despite different names*

### Comparing `salt-analytics-framework-0.3.0/CHANGELOG.rst` & `salt-analytics-framework-0.4.0/CHANGELOG.rst`

 * *Files 8% similar despite different names*

```diff
@@ -10,14 +10,34 @@
 **Deprecations** section of releases.
 
 .. towncrier-draft-entries::
 
 .. towncrier release notes start
 
 
+0.4.0 (2023-05-18)
+==================
+
+Improvements
+------------
+
+- `#41 <https://github.com/saltstack/pytest-skip-markers/issues/41>`_: AsyncIO cooperative file reads/writes. Support glob matching on paths.
+
+
+
+Bug Fixes
+---------
+
+- `#42 <https://github.com/saltstack/pytest-skip-markers/issues/42>`_: Explicitly create a new loop and assign it to the current thread and avoid a `DeprecationWarning`
+
+- `#43 <https://github.com/saltstack/pytest-skip-markers/issues/43>`_: Fix the seek to end of file call
+
+- `#44 <https://github.com/saltstack/pytest-skip-markers/issues/44>`_: Import `TypedDict` from typing_extensions on Python < 3.9.2
+
+
 0.3.0 (2023-05-17)
 ==================
 
 Improvements
 ------------
 
 - `#40 <https://github.com/saltstack/pytest-skip-markers/issues/40>`_: Allow the file collector to read from multiple files at a time
```

### Comparing `salt-analytics-framework-0.3.0/CODE_OF_CONDUCT.md` & `salt-analytics-framework-0.4.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `salt-analytics-framework-0.3.0/CONTRIBUTING.md` & `salt-analytics-framework-0.4.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `salt-analytics-framework-0.3.0/LICENSE` & `salt-analytics-framework-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `salt-analytics-framework-0.3.0/NOTICE` & `salt-analytics-framework-0.4.0/NOTICE`

 * *Files identical despite different names*

### Comparing `salt-analytics-framework-0.3.0/PKG-INFO` & `salt-analytics-framework-0.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: salt-analytics-framework
-Version: 0.3.0
+Version: 0.4.0
 Summary: Salt Analytics Framework
 Home-page: https://github.com/saltstack/salt-analytics-framework
 Author: Pedro Algarvio
 Author-email: palgarvio@vmware.com
 License: Apache Software License
 Project-URL: Source, https://github.com/saltstack/salt-analytics-framework
 Project-URL: Tracker, https://github.com/saltstack/salt-analytics-framework/issues
```

### Comparing `salt-analytics-framework-0.3.0/README.rst` & `salt-analytics-framework-0.4.0/README.rst`

 * *Files identical despite different names*

### Comparing `salt-analytics-framework-0.3.0/changelog/_template.rst` & `salt-analytics-framework-0.4.0/changelog/_template.rst`

 * *Files identical despite different names*

### Comparing `salt-analytics-framework-0.3.0/docs/Makefile` & `salt-analytics-framework-0.4.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `salt-analytics-framework-0.3.0/docs/conf.py` & `salt-analytics-framework-0.4.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `salt-analytics-framework-0.3.0/docs/index.rst` & `salt-analytics-framework-0.4.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `salt-analytics-framework-0.3.0/docs/make.bat` & `salt-analytics-framework-0.4.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `salt-analytics-framework-0.3.0/docs/ref/saf.collect.rst` & `salt-analytics-framework-0.4.0/docs/ref/saf.collect.rst`

 * *Files identical despite different names*

### Comparing `salt-analytics-framework-0.3.0/docs/ref/saf.forward.rst` & `salt-analytics-framework-0.4.0/docs/ref/saf.forward.rst`

 * *Files identical despite different names*

### Comparing `salt-analytics-framework-0.3.0/docs/ref/saf.process.rst` & `salt-analytics-framework-0.4.0/docs/ref/saf.process.rst`

 * *Files identical despite different names*

### Comparing `salt-analytics-framework-0.3.0/docs/ref/saf.rst` & `salt-analytics-framework-0.4.0/docs/ref/saf.rst`

 * *Files identical despite different names*

### Comparing `salt-analytics-framework-0.3.0/noxfile.py` & `salt-analytics-framework-0.4.0/noxfile.py`

 * *Files identical despite different names*

### Comparing `salt-analytics-framework-0.3.0/pyproject.toml` & `salt-analytics-framework-0.4.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -98,15 +98,15 @@
   "D100",   # Missing docstring in public module
 ]
 "src/saf/models.py" = [
   "D106",   # Missing docstring in public nested class
   "SLF001", # Private member accessed"
   "ARG003", # Unused class method argument: `kwargs`
 ]
-"src/saf/collect/logs.py" = [
+"src/saf/collect/file.py" = [
   "TCH003",  # Move standard library import `pathlib` into a type-checking block
 ]
 "src/saf/forward/disk.py" = [
   "TCH003",  # Move standard library import `pathlib` into a type-checking block
 ]
 "src/saf/forward/test.py" = [
   "TCH003",  # Move standard library import `pathlib` into a type-checking block
```

### Comparing `salt-analytics-framework-0.3.0/setup.cfg` & `salt-analytics-framework-0.4.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `salt-analytics-framework-0.3.0/src/saf/__init__.py` & `salt-analytics-framework-0.4.0/src/saf/__init__.py`

 * *Files identical despite different names*

### Comparing `salt-analytics-framework-0.3.0/src/saf/collect/beacons.py` & `salt-analytics-framework-0.4.0/src/saf/collect/beacons.py`

 * *Files identical despite different names*

### Comparing `salt-analytics-framework-0.3.0/src/saf/collect/file.py` & `salt-analytics-framework-0.4.0/src/saf/forward/test.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,72 +1,70 @@
 # Copyright 2021-2023 VMware, Inc.
 # SPDX-License-Identifier: Apache-2.0
 """
-A file collector plugin.
+Test forwarder plugin.
+
+The test forward plugin exists as an implementation example and also to be able
+to test the salt-analytics-framework
+
+It doesn't really do anything to the collected event.
 """
 from __future__ import annotations
 
+import asyncio
+import json
 import logging
-import os
-import pathlib  # noqa: TCH003
-from contextlib import ExitStack
-from typing import Any
-from typing import AsyncIterator
-from typing import List
+import pathlib
+from typing import Optional
 from typing import Type
 
-from saf.models import CollectConfigBase
 from saf.models import CollectedEvent
+from saf.models import ForwardConfigBase
 from saf.models import PipelineRunContext
 
 log = logging.getLogger(__name__)
 
 
-class FileCollectConfig(CollectConfigBase):
+class TestForwardConfig(ForwardConfigBase):
     """
-    Configuration schema for the file collect plugin.
+    Test forwarder configuration.
     """
 
-    paths: List[pathlib.Path]
-    # If true, starts at the beginning of a file, else at the end
-    backfill: bool = False
-    # If true, reads to the end of the file, else one line at a time
-    multiline: bool = False
-    file_mode: str = "r"
+    sleep: float = 0.0
+    path: Optional[pathlib.Path] = None
+    message: Optional[str] = None
+    dump_event: bool = False
 
 
-def get_config_schema() -> Type[FileCollectConfig]:
+def get_config_schema() -> Type[TestForwardConfig]:
     """
-    Get the file collect plugin configuration schema.
+    Get the noop plugin configuration schema.
     """
-    return FileCollectConfig
+    return TestForwardConfig
 
 
-async def collect(*, ctx: PipelineRunContext[FileCollectConfig]) -> AsyncIterator[CollectedEvent]:
+async def forward(
+    *,
+    ctx: PipelineRunContext[TestForwardConfig],
+    event: CollectedEvent,
+) -> None:
     """
-    Method called to collect file contents.
+    Method called to forward the event.
     """
     config = ctx.config
-
-    with ExitStack() as stack:
-        try:
-            handles = {
-                str(path): stack.enter_context(path.open(mode=config.file_mode))
-                for path in config.paths
-            }
-            if not config.backfill:
-                for handle in handles.values():
-                    handle.seek(0, os.SEEK_END)
-            while True:
-                for path, rfh in handles.items():
-                    contents: Any
-                    if config.multiline:
-                        contents = rfh.readlines()
-                    else:
-                        contents = rfh.readline()
-                    if contents and isinstance(contents, str):
-                        contents = [contents]
-                    if contents is not None:
-                        for line in contents:
-                            yield CollectedEvent(data={"lines": line, "source": path})
-        except FileNotFoundError as exc:
-            log.debug("File %s not found", exc.filename)
+    log.info("Forwarding using %s: %s", config.name, event)
+    if config.sleep > 0:
+        await asyncio.sleep(config.sleep)
+    if config.path:
+        if config.message:
+            if config.dump_event:
+                dump_text = json.dumps({config.message: event.dict()})
+            else:
+                dump_text = config.message
+        elif config.dump_event:
+            dump_text = event.json()
+        else:
+            dump_text = ""
+        log.info("Writing into %s. Contents: %s", config.path, dump_text)
+        with config.path.open("a", encoding="utf-8") as wfh:
+            wfh.write(dump_text + "\n")
+    log.info("Forwarded using %s: %s", config.name, event)
```

### Comparing `salt-analytics-framework-0.3.0/src/saf/collect/noop.py` & `salt-analytics-framework-0.4.0/src/saf/collect/noop.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,10 +39,10 @@
     Method called to collect events.
     """
     config = ctx.config
     ticks = 0
     while True:
         ticks += 1
         event = CollectedEvent(data={"ticks": ticks})
-        log.info("CollectedEvent: %s", event)
+        log.debug("CollectedEvent: %s", event)
         yield event
         await asyncio.sleep(config.interval)
```

### Comparing `salt-analytics-framework-0.3.0/src/saf/collect/salt_exec.py` & `salt-analytics-framework-0.4.0/src/saf/collect/salt_exec.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,10 +48,10 @@
     # Load salt functions and pick out the desired one
     loaded_funcs = salt.loader.minion_mods(config.parent.salt_config)
     loaded_fn = loaded_funcs[config.fn]
 
     while True:
         ret = loaded_fn(*config.args, **config.kwargs)
         event = CollectedEvent(data={"ret": ret})
-        log.info("CollectedEvent: %s", event)
+        log.debug("CollectedEvent: %s", event)
         yield event
         await asyncio.sleep(config.interval)
```

### Comparing `salt-analytics-framework-0.3.0/src/saf/forward/disk.py` & `salt-analytics-framework-0.4.0/src/saf/forward/disk.py`

 * *Files 20% similar despite different names*

```diff
@@ -8,14 +8,16 @@
 from __future__ import annotations
 
 import logging
 import pathlib
 from typing import Optional
 from typing import Type
 
+import aiofiles
+
 from saf.models import CollectedEvent
 from saf.models import ForwardConfigBase
 from saf.models import PipelineRunContext
 
 log = logging.getLogger(__name__)
 
 
@@ -49,14 +51,15 @@
     if config.pretty_print:
         indent = 2
     if not config.path.exists():
         config.path.mkdir(parents=True)
     if config.filename:
         dest = config.path / config.filename
         dest.touch()
-        with dest.open("a") as wfh:
-            wrote = wfh.write(event.json(indent=indent) + "\n")
+        async with aiofiles.open(dest, "a", encoding="utf-8") as wfh:
+            wrote = await wfh.write(f"{event.json(indent=indent)}\n")
     else:
         file_count = len(list(config.path.iterdir()))
         dest = config.path / f"event-dump-{file_count + 1}.json"
-        wrote = dest.write_text(event.json(indent=indent))
+        async with aiofiles.open(dest, "w", encoding="utf-8") as wfh:
+            wrote = await wfh.write(event.json(indent=indent))
     log.debug("Wrote %s bytes to %s", wrote, dest)
```

### Comparing `salt-analytics-framework-0.3.0/src/saf/forward/noop.py` & `salt-analytics-framework-0.4.0/src/saf/forward/noop.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,8 +28,8 @@
     *,
     ctx: PipelineRunContext[ForwardConfigBase],  # noqa: ARG001
     event: CollectedEvent,
 ) -> None:
     """
     Method called to forward the event.
     """
-    log.info("Forwarding: %s", event)
+    log.debug("Forwarding: %s", event)
```

### Comparing `salt-analytics-framework-0.3.0/src/saf/forward/test.py` & `salt-analytics-framework-0.4.0/tests/integration/collectors/salt_exec/test_config_get.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,70 +1,71 @@
 # Copyright 2021-2023 VMware, Inc.
 # SPDX-License-Identifier: Apache-2.0
-"""
-Test forwarder plugin.
-
-The test forward plugin exists as an implementation example and also to be able
-to test the salt-analytics-framework
-
-It doesn't really do anything to the collected event.
-"""
+#
 from __future__ import annotations
 
-import asyncio
 import json
 import logging
 import pathlib
-from typing import Optional
-from typing import Type
+import time
+
+import pytest
 
 from saf.models import CollectedEvent
-from saf.models import ForwardConfigBase
-from saf.models import PipelineRunContext
 
 log = logging.getLogger(__name__)
 
 
-class TestForwardConfig(ForwardConfigBase):
-    """
-    Test forwarder configuration.
-    """
-
-    sleep: float = 0.0
-    path: Optional[pathlib.Path] = None
-    message: Optional[str] = None
-    dump_event: bool = False
-
-
-def get_config_schema() -> Type[TestForwardConfig]:
-    """
-    Get the noop plugin configuration schema.
-    """
-    return TestForwardConfig
-
-
-async def forward(
-    *,
-    ctx: PipelineRunContext[TestForwardConfig],
-    event: CollectedEvent,
-) -> None:
-    """
-    Method called to forward the event.
-    """
-    config = ctx.config
-    log.info("Forwarding using %s: %s", config.name, event)
-    if config.sleep > 0:
-        await asyncio.sleep(config.sleep)
-    if config.path:
-        if config.message:
-            if config.dump_event:
-                dump_text = json.dumps({config.message: event.dict()})
-            else:
-                dump_text = config.message
-        elif config.dump_event:
-            dump_text = event.json()
-        else:
-            dump_text = ""
-        log.info("Writing into %s. Contents: %s", config.path, dump_text)
-        with config.path.open("a", encoding="utf-8") as wfh:
-            wfh.write(dump_text + "\n")
-    log.info("Forwarded using %s: %s", config.name, event)
+@pytest.fixture(scope="module")
+def analytics_config_contents(analytics_events_dump_directory) -> str:
+    return """
+    collectors:
+      salt-collector:
+        plugin: salt_exec
+        interval: 1
+        fn: config.get
+        args:
+          - id
+
+
+    processors:
+      noop-processor:
+        plugin: noop
+
+
+    forwarders:
+      disk-forwarder:
+        plugin: disk
+        filename: salt_exec_config_dump
+        path: {}
+
+
+    pipelines:
+      my-pipeline:
+        collect: salt-collector
+        process: noop-processor
+        forward: disk-forwarder
+    """.format(
+        analytics_events_dump_directory
+    )
+
+
+def test_pipeline(minion, analytics_events_dump_directory: pathlib.Path):
+    """
+    Test output of config.get being dumped to disk.
+    """
+    timeout = 10
+    dumpfile = analytics_events_dump_directory / "salt_exec_config_dump"
+
+    while timeout:
+        time.sleep(1)
+        timeout -= 1
+        if dumpfile.exists() and dumpfile.read_text().strip():
+            break
+    else:
+        pytest.fail(f"Failed to find dumped events in {analytics_events_dump_directory}")
+
+    contents = [
+        CollectedEvent.parse_obj(json.loads(i)) for i in dumpfile.read_text().strip().split("\n")
+    ]
+    for event in contents:
+        assert event.data["ret"] == minion.id
```

### Comparing `salt-analytics-framework-0.3.0/src/saf/manager.py` & `salt-analytics-framework-0.4.0/src/saf/manager.py`

 * *Files identical despite different names*

### Comparing `salt-analytics-framework-0.3.0/src/saf/models.py` & `salt-analytics-framework-0.4.0/src/saf/models.py`

 * *Files identical despite different names*

### Comparing `salt-analytics-framework-0.3.0/src/saf/pipeline.py` & `salt-analytics-framework-0.4.0/src/saf/pipeline.py`

 * *Files identical despite different names*

### Comparing `salt-analytics-framework-0.3.0/src/saf/plugins.py` & `salt-analytics-framework-0.4.0/src/saf/plugins.py`

 * *Files identical despite different names*

### Comparing `salt-analytics-framework-0.3.0/src/saf/process/noop.py` & `salt-analytics-framework-0.4.0/src/saf/process/noop.py`

 * *Files 5% similar despite different names*

```diff
@@ -29,9 +29,9 @@
     *,
     ctx: PipelineRunContext[ProcessConfigBase],  # noqa: ARG001
     event: CollectedEvent,
 ) -> AsyncIterator[CollectedEvent]:
     """
     Method called to process the event.
     """
-    log.info("Processing: %s", event)
+    log.debug("Processing: %s", event)
     yield event
```

### Comparing `salt-analytics-framework-0.3.0/src/saf/process/regex_mask.py` & `salt-analytics-framework-0.4.0/src/saf/process/regex_mask.py`

 * *Files 2% similar despite different names*

```diff
@@ -99,11 +99,11 @@
     ctx: PipelineRunContext[RegexMaskProcessConfig],
     event: CollectedEvent,
 ) -> AsyncIterator[CollectedEvent]:
     """
     Method called to mask the data based on provided regex rules.
     """
     config = ctx.config
-    log.info("Processing event in regex_mask: %s", event.json())
+    log.debug("Processing event in regex_mask: %s", event.json())
     event_dict = event.dict()
     processed_event_dict = _regex_process(event_dict, config)
     yield event.parse_obj(processed_event_dict)
```

### Comparing `salt-analytics-framework-0.3.0/src/saf/process/regex_mask.pyi` & `salt-analytics-framework-0.4.0/src/saf/process/regex_mask.pyi`

 * *Files identical despite different names*

### Comparing `salt-analytics-framework-0.3.0/src/saf/process/shannon_mask.py` & `salt-analytics-framework-0.4.0/src/saf/process/shannon_mask.py`

 * *Files 2% similar despite different names*

```diff
@@ -121,11 +121,11 @@
     ctx: PipelineRunContext[ShannonMaskProcessConfig],
     event: CollectedEvent,
 ) -> AsyncIterator[CollectedEvent]:
     """
     Method called to mask the data based on normalized Shannon index values.
     """
     config = ctx.config
-    log.info("Processing event in shannon_mask: %s", event.json())
+    log.debug("Processing event in shannon_mask: %s", event.json())
     event_dict = event.dict()
     processed_event_dict = _shannon_process(event_dict, config)
     yield event.parse_obj(processed_event_dict)
```

### Comparing `salt-analytics-framework-0.3.0/src/saf/saltext/engines/analytics.py` & `salt-analytics-framework-0.4.0/src/saf/saltext/engines/analytics.py`

 * *Files 3% similar despite different names*

```diff
@@ -61,15 +61,17 @@
     return config_dict
 
 
 def start() -> None:
     """
     Start the salt analytics engine.
     """
+    loop = asyncio.new_event_loop()
+    asyncio.set_event_loop(loop)
     config = AnalyticsConfig.parse_obj(get_config_dict())
     manager = Manager(config)
     aiorun.run(
         manager.run(),
-        loop=asyncio.get_event_loop(),
+        loop=loop,
         stop_on_unhandled_errors=True,
         shutdown_callback=manager.await_stopped(),
     )
```

### Comparing `salt-analytics-framework-0.3.0/src/saf/utils/eventbus.py` & `salt-analytics-framework-0.4.0/src/saf/utils/eventbus.py`

 * *Files identical despite different names*

### Comparing `salt-analytics-framework-0.3.0/src/salt_analytics_framework.egg-info/PKG-INFO` & `salt-analytics-framework-0.4.0/src/salt_analytics_framework.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: salt-analytics-framework
-Version: 0.3.0
+Version: 0.4.0
 Summary: Salt Analytics Framework
 Home-page: https://github.com/saltstack/salt-analytics-framework
 Author: Pedro Algarvio
 Author-email: palgarvio@vmware.com
 License: Apache Software License
 Project-URL: Source, https://github.com/saltstack/salt-analytics-framework
 Project-URL: Tracker, https://github.com/saltstack/salt-analytics-framework/issues
```

### Comparing `salt-analytics-framework-0.3.0/src/salt_analytics_framework.egg-info/SOURCES.txt` & `salt-analytics-framework-0.4.0/src/salt_analytics_framework.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `salt-analytics-framework-0.3.0/tests/__init__.py` & `salt-analytics-framework-0.4.0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `salt-analytics-framework-0.3.0/tests/conftest.py` & `salt-analytics-framework-0.4.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `salt-analytics-framework-0.3.0/tests/functional/conftest.py` & `salt-analytics-framework-0.4.0/tests/functional/conftest.py`

 * *Files identical despite different names*

### Comparing `salt-analytics-framework-0.3.0/tests/functional/forwarders/test_concurrency.py` & `salt-analytics-framework-0.4.0/tests/functional/forwarders/test_concurrency.py`

 * *Files identical despite different names*

### Comparing `salt-analytics-framework-0.3.0/tests/functional/manager/conftest.py` & `salt-analytics-framework-0.4.0/tests/functional/manager/conftest.py`

 * *Files identical despite different names*

### Comparing `salt-analytics-framework-0.3.0/tests/functional/manager/test_disabled_pipeline.py` & `salt-analytics-framework-0.4.0/tests/functional/manager/test_disabled_pipeline.py`

 * *Files identical despite different names*

### Comparing `salt-analytics-framework-0.3.0/tests/functional/manager/test_enabled_pipeline.py` & `salt-analytics-framework-0.4.0/tests/functional/manager/test_enabled_pipeline.py`

 * *Files identical despite different names*

### Comparing `salt-analytics-framework-0.3.0/tests/integration/collectors/beacons/test_memusage.py` & `salt-analytics-framework-0.4.0/tests/integration/collectors/beacons/test_memusage.py`

 * *Files identical despite different names*

### Comparing `salt-analytics-framework-0.3.0/tests/integration/collectors/beacons/test_multiple.py` & `salt-analytics-framework-0.4.0/tests/integration/collectors/beacons/test_multiple.py`

 * *Files identical despite different names*

### Comparing `salt-analytics-framework-0.3.0/tests/integration/collectors/beacons/test_status.py` & `salt-analytics-framework-0.4.0/tests/integration/collectors/beacons/test_status.py`

 * *Files identical despite different names*

### Comparing `salt-analytics-framework-0.3.0/tests/integration/collectors/salt_exec/conftest.py` & `salt-analytics-framework-0.4.0/tests/integration/collectors/salt_exec/conftest.py`

 * *Files identical despite different names*

### Comparing `salt-analytics-framework-0.3.0/tests/integration/collectors/salt_exec/test_arg.py` & `salt-analytics-framework-0.4.0/tests/integration/collectors/salt_exec/test_arg.py`

 * *Files identical despite different names*

### Comparing `salt-analytics-framework-0.3.0/tests/integration/collectors/salt_exec/test_collatz.py` & `salt-analytics-framework-0.4.0/tests/integration/collectors/salt_exec/test_collatz.py`

 * *Files identical despite different names*

### Comparing `salt-analytics-framework-0.3.0/tests/integration/conftest.py` & `salt-analytics-framework-0.4.0/tests/integration/conftest.py`

 * *Files identical despite different names*

### Comparing `salt-analytics-framework-0.3.0/tests/integration/engines/test_engine.py` & `salt-analytics-framework-0.4.0/tests/integration/engines/test_engine.py`

 * *Files identical despite different names*

### Comparing `salt-analytics-framework-0.3.0/tests/unit/process/test_regex_mask.py` & `salt-analytics-framework-0.4.0/tests/unit/process/test_regex_mask.py`

 * *Files identical despite different names*

### Comparing `salt-analytics-framework-0.3.0/tests/unit/process/test_shannon_mask.py` & `salt-analytics-framework-0.4.0/tests/unit/process/test_shannon_mask.py`

 * *Files identical despite different names*

### Comparing `salt-analytics-framework-0.3.0/tools/ci.py` & `salt-analytics-framework-0.4.0/tools/ci.py`

 * *Files identical despite different names*

### Comparing `salt-analytics-framework-0.3.0/tools/pre_commit.py` & `salt-analytics-framework-0.4.0/tools/pre_commit.py`

 * *Files identical despite different names*

### Comparing `salt-analytics-framework-0.3.0/tools/pre_commit.py~` & `salt-analytics-framework-0.4.0/tools/pre_commit.py~`

 * *Files identical despite different names*

