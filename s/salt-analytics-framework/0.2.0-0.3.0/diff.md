# Comparing `tmp/salt-analytics-framework-0.2.0.tar.gz` & `tmp/salt-analytics-framework-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Tue May 16 17:23:19 2023, max compression
+gzip compressed data, last modified: Wed May 17 22:24:55 2023, max compression
```

## Comparing `salt-analytics-framework-0.2.0.tar` & `salt-analytics-framework-0.3.0.tar`

### file list

```diff
@@ -1,154 +1,154 @@
--rw-r--r--   0 root         (0) root         (0)       20 2023-05-16 17:23:19.000000 salt-analytics-framework-0.2.0/.bandit
--rw-r--r--   0 root         (0) root         (0)      684 2023-05-16 17:23:19.000000 salt-analytics-framework-0.2.0/.coveragerc
--rw-r--r--   0 root         (0) root         (0)        5 2023-05-16 17:23:19.000000 salt-analytics-framework-0.2.0/.dockerignore
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 17:23:19.000000 salt-analytics-framework-0.2.0/.github/
--rw-r--r--   0 root         (0) root         (0)      229 2023-05-16 17:23:19.000000 salt-analytics-framework-0.2.0/.github/actionlint.yaml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 17:23:19.000000 salt-analytics-framework-0.2.0/.github/actions/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 17:23:19.000000 salt-analytics-framework-0.2.0/.github/actions/setup-actionlint/
--rw-r--r--   0 root         (0) root         (0)      892 2023-05-16 17:23:19.000000 salt-analytics-framework-0.2.0/.github/actions/setup-actionlint/action.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 17:23:19.000000 salt-analytics-framework-0.2.0/.github/workflows/
--rw-r--r--   0 root         (0) root         (0)    10391 2023-05-16 17:23:19.000000 salt-analytics-framework-0.2.0/.github/workflows/ci.yml
--rw-r--r--   0 root         (0) root         (0)     1983 2023-05-16 17:23:19.000000 salt-analytics-framework-0.2.0/.gitignore
--rw-r--r--   0 root         (0) root         (0)     3571 2023-05-16 17:23:19.000000 salt-analytics-framework-0.2.0/.pre-commit-config.yaml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 17:23:19.000000 salt-analytics-framework-0.2.0/.pre-commit-hooks/
--rw-r--r--   0 root         (0) root         (0)     4609 2023-05-16 17:23:19.000000 salt-analytics-framework-0.2.0/.pre-commit-hooks/check-changelog-entries.py
--rw-r--r--   0 root         (0) root         (0)     2227 2023-05-16 17:23:19.000000 salt-analytics-framework-0.2.0/.pre-commit-hooks/check-cli-examples.py
--rw-r--r--   0 root         (0) root         (0)     3549 2023-05-16 17:23:19.000000 salt-analytics-framework-0.2.0/.pre-commit-hooks/copyright-headers.py
--rw-r--r--   0 root         (0) root         (0)     2092 2023-05-16 17:23:19.000000 salt-analytics-framework-0.2.0/.pre-commit-hooks/make-autodocs.py
--rw-r--r--   0 root         (0) root         (0)      579 2023-05-16 17:23:19.000000 salt-analytics-framework-0.2.0/.pre-commit-hooks/sort-pylint-spelling-words.py
--rw-r--r--   0 root         (0) root         (0)      650 2023-05-16 17:23:19.000000 salt-analytics-framework-0.2.0/.pylint-spelling-words
--rw-r--r--   0 root         (0) root         (0)     1823 2023-05-16 17:23:19.000000 salt-analytics-framework-0.2.0/CHANGELOG.rst
--rw-r--r--   0 root         (0) root         (0)     5256 2023-05-16 17:23:19.000000 salt-analytics-framework-0.2.0/CODE_OF_CONDUCT.md
--rw-r--r--   0 root         (0) root         (0)     2487 2023-05-16 17:23:19.000000 salt-analytics-framework-0.2.0/CONTRIBUTING.md
--rw-r--r--   0 root         (0) root         (0)     9283 2023-05-16 17:23:19.000000 salt-analytics-framework-0.2.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)      549 2023-05-16 17:23:19.000000 salt-analytics-framework-0.2.0/NOTICE
--rw-r--r--   0 root         (0) root         (0)     3046 2023-05-16 17:23:19.000000 salt-analytics-framework-0.2.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1861 2023-05-16 17:23:19.000000 salt-analytics-framework-0.2.0/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 17:23:19.000000 salt-analytics-framework-0.2.0/changelog/
--rw-r--r--   0 root         (0) root         (0)     1450 2023-05-16 17:23:19.000000 salt-analytics-framework-0.2.0/changelog/_template.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 17:23:19.000000 salt-analytics-framework-0.2.0/docs/
--rw-r--r--   0 root         (0) root         (0)      634 2023-05-16 17:23:19.000000 salt-analytics-framework-0.2.0/docs/Makefile
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 17:23:19.000000 salt-analytics-framework-0.2.0/docs/_static/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-16 17:23:19.000000 salt-analytics-framework-0.2.0/docs/_static/.gitkeep
--rw-r--r--   0 root         (0) root         (0)      164 2023-05-16 17:23:19.000000 salt-analytics-framework-0.2.0/docs/all.rst
--rw-r--r--   0 root         (0) root         (0)       30 2023-05-16 17:23:19.000000 salt-analytics-framework-0.2.0/docs/changelog.rst
--rw-r--r--   0 root         (0) root         (0)     6553 2023-05-16 17:23:19.000000 salt-analytics-framework-0.2.0/docs/conf.py
--rw-r--r--   0 root         (0) root         (0)      200 2023-05-16 17:23:19.000000 salt-analytics-framework-0.2.0/docs/contents.rst
--rw-r--r--   0 root         (0) root         (0)      720 2023-05-16 17:23:19.000000 salt-analytics-framework-0.2.0/docs/index.rst
--rw-r--r--   0 root         (0) root         (0)      760 2023-05-16 17:23:19.000000 salt-analytics-framework-0.2.0/docs/make.bat
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 17:23:19.000000 salt-analytics-framework-0.2.0/docs/ref/
--rw-r--r--   0 root         (0) root         (0)       46 2023-05-16 17:23:19.000000 salt-analytics-framework-0.2.0/docs/ref/modules.rst
--rw-r--r--   0 root         (0) root         (0)      720 2023-05-16 17:23:19.000000 salt-analytics-framework-0.2.0/docs/ref/saf.collect.rst
--rw-r--r--   0 root         (0) root         (0)      557 2023-05-16 17:23:19.000000 salt-analytics-framework-0.2.0/docs/ref/saf.forward.rst
--rw-r--r--   0 root         (0) root         (0)      603 2023-05-16 17:23:19.000000 salt-analytics-framework-0.2.0/docs/ref/saf.process.rst
--rw-r--r--   0 root         (0) root         (0)      861 2023-05-16 17:23:19.000000 salt-analytics-framework-0.2.0/docs/ref/saf.rst
--rw-r--r--   0 root         (0) root         (0)      346 2023-05-16 17:23:19.000000 salt-analytics-framework-0.2.0/docs/ref/saf.saltext.engines.rst
--rw-r--r--   0 root         (0) root         (0)      202 2023-05-16 17:23:19.000000 salt-analytics-framework-0.2.0/docs/ref/saf.saltext.rst
--rw-r--r--   0 root         (0) root         (0)      408 2023-05-16 17:23:19.000000 salt-analytics-framework-0.2.0/docs/ref/saf.utils.rst
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-16 17:23:19.000000 salt-analytics-framework-0.2.0/docs/sitevars.rst
--rw-r--r--   0 root         (0) root         (0)    20016 2023-05-16 17:23:19.000000 salt-analytics-framework-0.2.0/noxfile.py
--rw-r--r--   0 root         (0) root         (0)     4837 2023-05-16 17:23:19.000000 salt-analytics-framework-0.2.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)      428 2023-05-16 17:23:19.000000 salt-analytics-framework-0.2.0/pytest.ini
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 17:23:19.000000 salt-analytics-framework-0.2.0/requirements/
--rw-r--r--   0 root         (0) root         (0)      113 2023-05-16 17:23:19.000000 salt-analytics-framework-0.2.0/requirements/base.txt
--rw-r--r--   0 root         (0) root         (0)       19 2023-05-16 17:23:19.000000 salt-analytics-framework-0.2.0/requirements/build.txt
--rw-r--r--   0 root         (0) root         (0)       21 2023-05-16 17:23:19.000000 salt-analytics-framework-0.2.0/requirements/changelog.txt
--rw-r--r--   0 root         (0) root         (0)      188 2023-05-16 17:23:19.000000 salt-analytics-framework-0.2.0/requirements/dev.txt
--rw-r--r--   0 root         (0) root         (0)       17 2023-05-16 17:23:19.000000 salt-analytics-framework-0.2.0/requirements/docs-auto.txt
--rw-r--r--   0 root         (0) root         (0)      148 2023-05-16 17:23:19.000000 salt-analytics-framework-0.2.0/requirements/docs.txt
--rw-r--r--   0 root         (0) root         (0)       74 2023-05-16 17:23:19.000000 salt-analytics-framework-0.2.0/requirements/tests.txt
--rw-r--r--   0 root         (0) root         (0)       31 2023-05-16 17:23:19.000000 salt-analytics-framework-0.2.0/requirements/tools.txt
--rw-r--r--   0 root         (0) root         (0)     3170 2023-05-16 17:23:19.000000 salt-analytics-framework-0.2.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      198 2023-05-16 17:23:19.000000 salt-analytics-framework-0.2.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 17:23:19.000000 salt-analytics-framework-0.2.0/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 17:23:19.000000 salt-analytics-framework-0.2.0/src/saf/
--rw-r--r--   0 root         (0) root         (0)      914 2023-05-16 17:23:19.000000 salt-analytics-framework-0.2.0/src/saf/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 17:23:19.000000 salt-analytics-framework-0.2.0/src/saf/collect/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-16 17:23:19.000000 salt-analytics-framework-0.2.0/src/saf/collect/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2618 2023-05-16 17:23:19.000000 salt-analytics-framework-0.2.0/src/saf/collect/beacons.py
--rw-r--r--   0 root         (0) root         (0)     1857 2023-05-16 17:23:19.000000 salt-analytics-framework-0.2.0/src/saf/collect/file.py
--rw-r--r--   0 root         (0) root         (0)     1126 2023-05-16 17:23:19.000000 salt-analytics-framework-0.2.0/src/saf/collect/noop.py
--rw-r--r--   0 root         (0) root         (0)     1472 2023-05-16 17:23:19.000000 salt-analytics-framework-0.2.0/src/saf/collect/salt_exec.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 17:23:19.000000 salt-analytics-framework-0.2.0/src/saf/forward/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-16 17:23:19.000000 salt-analytics-framework-0.2.0/src/saf/forward/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1560 2023-05-16 17:23:19.000000 salt-analytics-framework-0.2.0/src/saf/forward/disk.py
--rw-r--r--   0 root         (0) root         (0)      797 2023-05-16 17:23:19.000000 salt-analytics-framework-0.2.0/src/saf/forward/noop.py
--rw-r--r--   0 root         (0) root         (0)     1825 2023-05-16 17:23:19.000000 salt-analytics-framework-0.2.0/src/saf/forward/test.py
--rw-r--r--   0 root         (0) root         (0)     3085 2023-05-16 17:23:19.000000 salt-analytics-framework-0.2.0/src/saf/manager.py
--rw-r--r--   0 root         (0) root         (0)    10262 2023-05-16 17:23:19.000000 salt-analytics-framework-0.2.0/src/saf/models.py
--rw-r--r--   0 root         (0) root         (0)     6800 2023-05-16 17:23:19.000000 salt-analytics-framework-0.2.0/src/saf/pipeline.py
--rw-r--r--   0 root         (0) root         (0)     2791 2023-05-16 17:23:19.000000 salt-analytics-framework-0.2.0/src/saf/plugins.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 17:23:19.000000 salt-analytics-framework-0.2.0/src/saf/process/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-16 17:23:19.000000 salt-analytics-framework-0.2.0/src/saf/process/__init__.py
--rw-r--r--   0 root         (0) root         (0)      872 2023-05-16 17:23:19.000000 salt-analytics-framework-0.2.0/src/saf/process/noop.py
--rw-r--r--   0 root         (0) root         (0)     3194 2023-05-16 17:23:19.000000 salt-analytics-framework-0.2.0/src/saf/process/regex_mask.py
--rw-r--r--   0 root         (0) root         (0)      594 2023-05-16 17:23:19.000000 salt-analytics-framework-0.2.0/src/saf/process/regex_mask.pyi
--rw-r--r--   0 root         (0) root         (0)     4489 2023-05-16 17:23:19.000000 salt-analytics-framework-0.2.0/src/saf/process/shannon_mask.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-16 17:23:19.000000 salt-analytics-framework-0.2.0/src/saf/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 17:23:19.000000 salt-analytics-framework-0.2.0/src/saf/saltext/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-16 17:23:19.000000 salt-analytics-framework-0.2.0/src/saf/saltext/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 17:23:19.000000 salt-analytics-framework-0.2.0/src/saf/saltext/engines/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-16 17:23:19.000000 salt-analytics-framework-0.2.0/src/saf/saltext/engines/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2116 2023-05-16 17:23:19.000000 salt-analytics-framework-0.2.0/src/saf/saltext/engines/analytics.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 17:23:19.000000 salt-analytics-framework-0.2.0/src/saf/utils/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-16 17:23:19.000000 salt-analytics-framework-0.2.0/src/saf/utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)      362 2023-05-16 17:23:19.000000 salt-analytics-framework-0.2.0/src/saf/utils/dt.py
--rw-r--r--   0 root         (0) root         (0)     5542 2023-05-16 17:23:19.000000 salt-analytics-framework-0.2.0/src/saf/utils/eventbus.py
--rw-r--r--   0 root         (0) root         (0)       42 2023-05-16 17:23:19.000000 salt-analytics-framework-0.2.0/src/saf/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 17:23:19.000000 salt-analytics-framework-0.2.0/src/salt_analytics_framework.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3046 2023-05-16 17:23:19.000000 salt-analytics-framework-0.2.0/src/salt_analytics_framework.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3417 2023-05-16 17:23:19.000000 salt-analytics-framework-0.2.0/src/salt_analytics_framework.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-16 17:23:19.000000 salt-analytics-framework-0.2.0/src/salt_analytics_framework.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      382 2023-05-16 17:23:19.000000 salt-analytics-framework-0.2.0/src/salt_analytics_framework.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-16 17:23:19.000000 salt-analytics-framework-0.2.0/src/salt_analytics_framework.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      586 2023-05-16 17:23:19.000000 salt-analytics-framework-0.2.0/src/salt_analytics_framework.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        4 2023-05-16 17:23:19.000000 salt-analytics-framework-0.2.0/src/salt_analytics_framework.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 17:23:19.000000 salt-analytics-framework-0.2.0/tests/
--rw-r--r--   0 root         (0) root         (0)      738 2023-05-16 17:23:19.000000 salt-analytics-framework-0.2.0/tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1497 2023-05-16 17:23:19.000000 salt-analytics-framework-0.2.0/tests/conftest.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 17:23:19.000000 salt-analytics-framework-0.2.0/tests/functional/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-16 17:23:19.000000 salt-analytics-framework-0.2.0/tests/functional/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1207 2023-05-16 17:23:19.000000 salt-analytics-framework-0.2.0/tests/functional/conftest.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 17:23:19.000000 salt-analytics-framework-0.2.0/tests/functional/forwarders/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-16 17:23:19.000000 salt-analytics-framework-0.2.0/tests/functional/forwarders/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2303 2023-05-16 17:23:19.000000 salt-analytics-framework-0.2.0/tests/functional/forwarders/test_concurrency.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 17:23:19.000000 salt-analytics-framework-0.2.0/tests/functional/manager/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-16 17:23:19.000000 salt-analytics-framework-0.2.0/tests/functional/manager/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1763 2023-05-16 17:23:19.000000 salt-analytics-framework-0.2.0/tests/functional/manager/conftest.py
--rw-r--r--   0 root         (0) root         (0)     1063 2023-05-16 17:23:19.000000 salt-analytics-framework-0.2.0/tests/functional/manager/test_disabled_pipeline.py
--rw-r--r--   0 root         (0) root         (0)     1211 2023-05-16 17:23:19.000000 salt-analytics-framework-0.2.0/tests/functional/manager/test_enabled_pipeline.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 17:23:19.000000 salt-analytics-framework-0.2.0/tests/integration/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-16 17:23:19.000000 salt-analytics-framework-0.2.0/tests/integration/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 17:23:19.000000 salt-analytics-framework-0.2.0/tests/integration/collectors/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-16 17:23:19.000000 salt-analytics-framework-0.2.0/tests/integration/collectors/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 17:23:19.000000 salt-analytics-framework-0.2.0/tests/integration/collectors/beacons/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-16 17:23:19.000000 salt-analytics-framework-0.2.0/tests/integration/collectors/beacons/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1967 2023-05-16 17:23:19.000000 salt-analytics-framework-0.2.0/tests/integration/collectors/beacons/test_memusage.py
--rw-r--r--   0 root         (0) root         (0)     2119 2023-05-16 17:23:19.000000 salt-analytics-framework-0.2.0/tests/integration/collectors/beacons/test_multiple.py
--rw-r--r--   0 root         (0) root         (0)     1982 2023-05-16 17:23:19.000000 salt-analytics-framework-0.2.0/tests/integration/collectors/beacons/test_status.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 17:23:19.000000 salt-analytics-framework-0.2.0/tests/integration/collectors/salt_exec/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-16 17:23:19.000000 salt-analytics-framework-0.2.0/tests/integration/collectors/salt_exec/__init__.py
--rw-r--r--   0 root         (0) root         (0)      775 2023-05-16 17:23:19.000000 salt-analytics-framework-0.2.0/tests/integration/collectors/salt_exec/conftest.py
--rw-r--r--   0 root         (0) root         (0)     1734 2023-05-16 17:23:19.000000 salt-analytics-framework-0.2.0/tests/integration/collectors/salt_exec/test_arg.py
--rw-r--r--   0 root         (0) root         (0)     1563 2023-05-16 17:23:19.000000 salt-analytics-framework-0.2.0/tests/integration/collectors/salt_exec/test_collatz.py
--rw-r--r--   0 root         (0) root         (0)     1556 2023-05-16 17:23:19.000000 salt-analytics-framework-0.2.0/tests/integration/collectors/salt_exec/test_config_get.py
--rw-r--r--   0 root         (0) root         (0)     1399 2023-05-16 17:23:19.000000 salt-analytics-framework-0.2.0/tests/integration/conftest.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 17:23:19.000000 salt-analytics-framework-0.2.0/tests/integration/engines/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-16 17:23:19.000000 salt-analytics-framework-0.2.0/tests/integration/engines/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1517 2023-05-16 17:23:19.000000 salt-analytics-framework-0.2.0/tests/integration/engines/test_engine.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 17:23:19.000000 salt-analytics-framework-0.2.0/tests/unit/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-16 17:23:19.000000 salt-analytics-framework-0.2.0/tests/unit/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 17:23:19.000000 salt-analytics-framework-0.2.0/tests/unit/process/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-16 17:23:19.000000 salt-analytics-framework-0.2.0/tests/unit/process/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3803 2023-05-16 17:23:19.000000 salt-analytics-framework-0.2.0/tests/unit/process/test_regex_mask.py
--rw-r--r--   0 root         (0) root         (0)     5436 2023-05-16 17:23:19.000000 salt-analytics-framework-0.2.0/tests/unit/process/test_shannon_mask.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 17:23:19.000000 salt-analytics-framework-0.2.0/tests/unit/salt/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-16 17:23:19.000000 salt-analytics-framework-0.2.0/tests/unit/salt/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 17:23:19.000000 salt-analytics-framework-0.2.0/tests/unit/salt/engines/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-16 17:23:19.000000 salt-analytics-framework-0.2.0/tests/unit/salt/engines/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 17:23:19.000000 salt-analytics-framework-0.2.0/tools/
--rw-r--r--   0 root         (0) root         (0)       89 2023-05-16 17:23:19.000000 salt-analytics-framework-0.2.0/tools/.ruff.toml
--rw-r--r--   0 root         (0) root         (0)      334 2023-05-16 17:23:19.000000 salt-analytics-framework-0.2.0/tools/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5495 2023-05-16 17:23:19.000000 salt-analytics-framework-0.2.0/tools/ci.py
--rw-r--r--   0 root         (0) root         (0)     1383 2023-05-16 17:23:19.000000 salt-analytics-framework-0.2.0/tools/pre_commit.py
--rw-r--r--   0 root         (0) root         (0)     1382 2023-05-16 17:23:19.000000 salt-analytics-framework-0.2.0/tools/pre_commit.py~
+-rw-r--r--   0 root         (0) root         (0)       20 2023-05-17 22:24:55.000000 salt-analytics-framework-0.3.0/.bandit
+-rw-r--r--   0 root         (0) root         (0)      684 2023-05-17 22:24:55.000000 salt-analytics-framework-0.3.0/.coveragerc
+-rw-r--r--   0 root         (0) root         (0)        5 2023-05-17 22:24:55.000000 salt-analytics-framework-0.3.0/.dockerignore
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 22:24:55.000000 salt-analytics-framework-0.3.0/.github/
+-rw-r--r--   0 root         (0) root         (0)      229 2023-05-17 22:24:55.000000 salt-analytics-framework-0.3.0/.github/actionlint.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 22:24:55.000000 salt-analytics-framework-0.3.0/.github/actions/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 22:24:55.000000 salt-analytics-framework-0.3.0/.github/actions/setup-actionlint/
+-rw-r--r--   0 root         (0) root         (0)      892 2023-05-17 22:24:55.000000 salt-analytics-framework-0.3.0/.github/actions/setup-actionlint/action.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 22:24:55.000000 salt-analytics-framework-0.3.0/.github/workflows/
+-rw-r--r--   0 root         (0) root         (0)    10391 2023-05-17 22:24:55.000000 salt-analytics-framework-0.3.0/.github/workflows/ci.yml
+-rw-r--r--   0 root         (0) root         (0)     1983 2023-05-17 22:24:55.000000 salt-analytics-framework-0.3.0/.gitignore
+-rw-r--r--   0 root         (0) root         (0)     3571 2023-05-17 22:24:55.000000 salt-analytics-framework-0.3.0/.pre-commit-config.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 22:24:55.000000 salt-analytics-framework-0.3.0/.pre-commit-hooks/
+-rw-r--r--   0 root         (0) root         (0)     4609 2023-05-17 22:24:55.000000 salt-analytics-framework-0.3.0/.pre-commit-hooks/check-changelog-entries.py
+-rw-r--r--   0 root         (0) root         (0)     2227 2023-05-17 22:24:55.000000 salt-analytics-framework-0.3.0/.pre-commit-hooks/check-cli-examples.py
+-rw-r--r--   0 root         (0) root         (0)     3549 2023-05-17 22:24:55.000000 salt-analytics-framework-0.3.0/.pre-commit-hooks/copyright-headers.py
+-rw-r--r--   0 root         (0) root         (0)     2092 2023-05-17 22:24:55.000000 salt-analytics-framework-0.3.0/.pre-commit-hooks/make-autodocs.py
+-rw-r--r--   0 root         (0) root         (0)      579 2023-05-17 22:24:55.000000 salt-analytics-framework-0.3.0/.pre-commit-hooks/sort-pylint-spelling-words.py
+-rw-r--r--   0 root         (0) root         (0)      650 2023-05-17 22:24:55.000000 salt-analytics-framework-0.3.0/.pylint-spelling-words
+-rw-r--r--   0 root         (0) root         (0)     2025 2023-05-17 22:24:55.000000 salt-analytics-framework-0.3.0/CHANGELOG.rst
+-rw-r--r--   0 root         (0) root         (0)     5256 2023-05-17 22:24:55.000000 salt-analytics-framework-0.3.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0 root         (0) root         (0)     2487 2023-05-17 22:24:55.000000 salt-analytics-framework-0.3.0/CONTRIBUTING.md
+-rw-r--r--   0 root         (0) root         (0)     9283 2023-05-17 22:24:55.000000 salt-analytics-framework-0.3.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      549 2023-05-17 22:24:55.000000 salt-analytics-framework-0.3.0/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     3046 2023-05-17 22:24:55.000000 salt-analytics-framework-0.3.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1861 2023-05-17 22:24:55.000000 salt-analytics-framework-0.3.0/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 22:24:55.000000 salt-analytics-framework-0.3.0/changelog/
+-rw-r--r--   0 root         (0) root         (0)     1450 2023-05-17 22:24:55.000000 salt-analytics-framework-0.3.0/changelog/_template.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 22:24:55.000000 salt-analytics-framework-0.3.0/docs/
+-rw-r--r--   0 root         (0) root         (0)      634 2023-05-17 22:24:55.000000 salt-analytics-framework-0.3.0/docs/Makefile
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 22:24:55.000000 salt-analytics-framework-0.3.0/docs/_static/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-17 22:24:55.000000 salt-analytics-framework-0.3.0/docs/_static/.gitkeep
+-rw-r--r--   0 root         (0) root         (0)      164 2023-05-17 22:24:55.000000 salt-analytics-framework-0.3.0/docs/all.rst
+-rw-r--r--   0 root         (0) root         (0)       30 2023-05-17 22:24:55.000000 salt-analytics-framework-0.3.0/docs/changelog.rst
+-rw-r--r--   0 root         (0) root         (0)     6553 2023-05-17 22:24:55.000000 salt-analytics-framework-0.3.0/docs/conf.py
+-rw-r--r--   0 root         (0) root         (0)      200 2023-05-17 22:24:55.000000 salt-analytics-framework-0.3.0/docs/contents.rst
+-rw-r--r--   0 root         (0) root         (0)      720 2023-05-17 22:24:55.000000 salt-analytics-framework-0.3.0/docs/index.rst
+-rw-r--r--   0 root         (0) root         (0)      760 2023-05-17 22:24:55.000000 salt-analytics-framework-0.3.0/docs/make.bat
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 22:24:55.000000 salt-analytics-framework-0.3.0/docs/ref/
+-rw-r--r--   0 root         (0) root         (0)       46 2023-05-17 22:24:55.000000 salt-analytics-framework-0.3.0/docs/ref/modules.rst
+-rw-r--r--   0 root         (0) root         (0)      720 2023-05-17 22:24:55.000000 salt-analytics-framework-0.3.0/docs/ref/saf.collect.rst
+-rw-r--r--   0 root         (0) root         (0)      557 2023-05-17 22:24:55.000000 salt-analytics-framework-0.3.0/docs/ref/saf.forward.rst
+-rw-r--r--   0 root         (0) root         (0)      603 2023-05-17 22:24:55.000000 salt-analytics-framework-0.3.0/docs/ref/saf.process.rst
+-rw-r--r--   0 root         (0) root         (0)      861 2023-05-17 22:24:55.000000 salt-analytics-framework-0.3.0/docs/ref/saf.rst
+-rw-r--r--   0 root         (0) root         (0)      346 2023-05-17 22:24:55.000000 salt-analytics-framework-0.3.0/docs/ref/saf.saltext.engines.rst
+-rw-r--r--   0 root         (0) root         (0)      202 2023-05-17 22:24:55.000000 salt-analytics-framework-0.3.0/docs/ref/saf.saltext.rst
+-rw-r--r--   0 root         (0) root         (0)      408 2023-05-17 22:24:55.000000 salt-analytics-framework-0.3.0/docs/ref/saf.utils.rst
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-17 22:24:55.000000 salt-analytics-framework-0.3.0/docs/sitevars.rst
+-rw-r--r--   0 root         (0) root         (0)    20016 2023-05-17 22:24:55.000000 salt-analytics-framework-0.3.0/noxfile.py
+-rw-r--r--   0 root         (0) root         (0)     4837 2023-05-17 22:24:55.000000 salt-analytics-framework-0.3.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)      428 2023-05-17 22:24:55.000000 salt-analytics-framework-0.3.0/pytest.ini
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 22:24:55.000000 salt-analytics-framework-0.3.0/requirements/
+-rw-r--r--   0 root         (0) root         (0)      113 2023-05-17 22:24:55.000000 salt-analytics-framework-0.3.0/requirements/base.txt
+-rw-r--r--   0 root         (0) root         (0)       19 2023-05-17 22:24:55.000000 salt-analytics-framework-0.3.0/requirements/build.txt
+-rw-r--r--   0 root         (0) root         (0)       21 2023-05-17 22:24:55.000000 salt-analytics-framework-0.3.0/requirements/changelog.txt
+-rw-r--r--   0 root         (0) root         (0)      188 2023-05-17 22:24:55.000000 salt-analytics-framework-0.3.0/requirements/dev.txt
+-rw-r--r--   0 root         (0) root         (0)       17 2023-05-17 22:24:55.000000 salt-analytics-framework-0.3.0/requirements/docs-auto.txt
+-rw-r--r--   0 root         (0) root         (0)      148 2023-05-17 22:24:55.000000 salt-analytics-framework-0.3.0/requirements/docs.txt
+-rw-r--r--   0 root         (0) root         (0)       74 2023-05-17 22:24:55.000000 salt-analytics-framework-0.3.0/requirements/tests.txt
+-rw-r--r--   0 root         (0) root         (0)       31 2023-05-17 22:24:55.000000 salt-analytics-framework-0.3.0/requirements/tools.txt
+-rw-r--r--   0 root         (0) root         (0)     3170 2023-05-17 22:24:55.000000 salt-analytics-framework-0.3.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      198 2023-05-17 22:24:55.000000 salt-analytics-framework-0.3.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 22:24:55.000000 salt-analytics-framework-0.3.0/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 22:24:55.000000 salt-analytics-framework-0.3.0/src/saf/
+-rw-r--r--   0 root         (0) root         (0)      914 2023-05-17 22:24:55.000000 salt-analytics-framework-0.3.0/src/saf/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 22:24:55.000000 salt-analytics-framework-0.3.0/src/saf/collect/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-17 22:24:55.000000 salt-analytics-framework-0.3.0/src/saf/collect/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2618 2023-05-17 22:24:55.000000 salt-analytics-framework-0.3.0/src/saf/collect/beacons.py
+-rw-r--r--   0 root         (0) root         (0)     2190 2023-05-17 22:24:55.000000 salt-analytics-framework-0.3.0/src/saf/collect/file.py
+-rw-r--r--   0 root         (0) root         (0)     1126 2023-05-17 22:24:55.000000 salt-analytics-framework-0.3.0/src/saf/collect/noop.py
+-rw-r--r--   0 root         (0) root         (0)     1472 2023-05-17 22:24:55.000000 salt-analytics-framework-0.3.0/src/saf/collect/salt_exec.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 22:24:55.000000 salt-analytics-framework-0.3.0/src/saf/forward/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-17 22:24:55.000000 salt-analytics-framework-0.3.0/src/saf/forward/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1560 2023-05-17 22:24:55.000000 salt-analytics-framework-0.3.0/src/saf/forward/disk.py
+-rw-r--r--   0 root         (0) root         (0)      797 2023-05-17 22:24:55.000000 salt-analytics-framework-0.3.0/src/saf/forward/noop.py
+-rw-r--r--   0 root         (0) root         (0)     1825 2023-05-17 22:24:55.000000 salt-analytics-framework-0.3.0/src/saf/forward/test.py
+-rw-r--r--   0 root         (0) root         (0)     3085 2023-05-17 22:24:55.000000 salt-analytics-framework-0.3.0/src/saf/manager.py
+-rw-r--r--   0 root         (0) root         (0)    10262 2023-05-17 22:24:55.000000 salt-analytics-framework-0.3.0/src/saf/models.py
+-rw-r--r--   0 root         (0) root         (0)     6800 2023-05-17 22:24:55.000000 salt-analytics-framework-0.3.0/src/saf/pipeline.py
+-rw-r--r--   0 root         (0) root         (0)     2791 2023-05-17 22:24:55.000000 salt-analytics-framework-0.3.0/src/saf/plugins.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 22:24:55.000000 salt-analytics-framework-0.3.0/src/saf/process/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-17 22:24:55.000000 salt-analytics-framework-0.3.0/src/saf/process/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      872 2023-05-17 22:24:55.000000 salt-analytics-framework-0.3.0/src/saf/process/noop.py
+-rw-r--r--   0 root         (0) root         (0)     3194 2023-05-17 22:24:55.000000 salt-analytics-framework-0.3.0/src/saf/process/regex_mask.py
+-rw-r--r--   0 root         (0) root         (0)      594 2023-05-17 22:24:55.000000 salt-analytics-framework-0.3.0/src/saf/process/regex_mask.pyi
+-rw-r--r--   0 root         (0) root         (0)     4489 2023-05-17 22:24:55.000000 salt-analytics-framework-0.3.0/src/saf/process/shannon_mask.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-17 22:24:55.000000 salt-analytics-framework-0.3.0/src/saf/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 22:24:55.000000 salt-analytics-framework-0.3.0/src/saf/saltext/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-17 22:24:55.000000 salt-analytics-framework-0.3.0/src/saf/saltext/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 22:24:55.000000 salt-analytics-framework-0.3.0/src/saf/saltext/engines/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-17 22:24:55.000000 salt-analytics-framework-0.3.0/src/saf/saltext/engines/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2116 2023-05-17 22:24:55.000000 salt-analytics-framework-0.3.0/src/saf/saltext/engines/analytics.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 22:24:55.000000 salt-analytics-framework-0.3.0/src/saf/utils/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-17 22:24:55.000000 salt-analytics-framework-0.3.0/src/saf/utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      362 2023-05-17 22:24:55.000000 salt-analytics-framework-0.3.0/src/saf/utils/dt.py
+-rw-r--r--   0 root         (0) root         (0)     5542 2023-05-17 22:24:55.000000 salt-analytics-framework-0.3.0/src/saf/utils/eventbus.py
+-rw-r--r--   0 root         (0) root         (0)       42 2023-05-17 22:24:55.000000 salt-analytics-framework-0.3.0/src/saf/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 22:24:55.000000 salt-analytics-framework-0.3.0/src/salt_analytics_framework.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3046 2023-05-17 22:24:55.000000 salt-analytics-framework-0.3.0/src/salt_analytics_framework.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3417 2023-05-17 22:24:55.000000 salt-analytics-framework-0.3.0/src/salt_analytics_framework.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-17 22:24:55.000000 salt-analytics-framework-0.3.0/src/salt_analytics_framework.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      382 2023-05-17 22:24:55.000000 salt-analytics-framework-0.3.0/src/salt_analytics_framework.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-17 22:24:55.000000 salt-analytics-framework-0.3.0/src/salt_analytics_framework.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      586 2023-05-17 22:24:55.000000 salt-analytics-framework-0.3.0/src/salt_analytics_framework.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        4 2023-05-17 22:24:55.000000 salt-analytics-framework-0.3.0/src/salt_analytics_framework.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 22:24:55.000000 salt-analytics-framework-0.3.0/tests/
+-rw-r--r--   0 root         (0) root         (0)      738 2023-05-17 22:24:55.000000 salt-analytics-framework-0.3.0/tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1497 2023-05-17 22:24:55.000000 salt-analytics-framework-0.3.0/tests/conftest.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 22:24:55.000000 salt-analytics-framework-0.3.0/tests/functional/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-17 22:24:55.000000 salt-analytics-framework-0.3.0/tests/functional/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1207 2023-05-17 22:24:55.000000 salt-analytics-framework-0.3.0/tests/functional/conftest.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 22:24:55.000000 salt-analytics-framework-0.3.0/tests/functional/forwarders/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-17 22:24:55.000000 salt-analytics-framework-0.3.0/tests/functional/forwarders/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2303 2023-05-17 22:24:55.000000 salt-analytics-framework-0.3.0/tests/functional/forwarders/test_concurrency.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 22:24:55.000000 salt-analytics-framework-0.3.0/tests/functional/manager/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-17 22:24:55.000000 salt-analytics-framework-0.3.0/tests/functional/manager/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1763 2023-05-17 22:24:55.000000 salt-analytics-framework-0.3.0/tests/functional/manager/conftest.py
+-rw-r--r--   0 root         (0) root         (0)     1063 2023-05-17 22:24:55.000000 salt-analytics-framework-0.3.0/tests/functional/manager/test_disabled_pipeline.py
+-rw-r--r--   0 root         (0) root         (0)     1211 2023-05-17 22:24:55.000000 salt-analytics-framework-0.3.0/tests/functional/manager/test_enabled_pipeline.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 22:24:55.000000 salt-analytics-framework-0.3.0/tests/integration/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-17 22:24:55.000000 salt-analytics-framework-0.3.0/tests/integration/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 22:24:55.000000 salt-analytics-framework-0.3.0/tests/integration/collectors/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-17 22:24:55.000000 salt-analytics-framework-0.3.0/tests/integration/collectors/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 22:24:55.000000 salt-analytics-framework-0.3.0/tests/integration/collectors/beacons/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-17 22:24:55.000000 salt-analytics-framework-0.3.0/tests/integration/collectors/beacons/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1967 2023-05-17 22:24:55.000000 salt-analytics-framework-0.3.0/tests/integration/collectors/beacons/test_memusage.py
+-rw-r--r--   0 root         (0) root         (0)     2119 2023-05-17 22:24:55.000000 salt-analytics-framework-0.3.0/tests/integration/collectors/beacons/test_multiple.py
+-rw-r--r--   0 root         (0) root         (0)     1982 2023-05-17 22:24:55.000000 salt-analytics-framework-0.3.0/tests/integration/collectors/beacons/test_status.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 22:24:55.000000 salt-analytics-framework-0.3.0/tests/integration/collectors/salt_exec/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-17 22:24:55.000000 salt-analytics-framework-0.3.0/tests/integration/collectors/salt_exec/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      775 2023-05-17 22:24:55.000000 salt-analytics-framework-0.3.0/tests/integration/collectors/salt_exec/conftest.py
+-rw-r--r--   0 root         (0) root         (0)     1734 2023-05-17 22:24:55.000000 salt-analytics-framework-0.3.0/tests/integration/collectors/salt_exec/test_arg.py
+-rw-r--r--   0 root         (0) root         (0)     1563 2023-05-17 22:24:55.000000 salt-analytics-framework-0.3.0/tests/integration/collectors/salt_exec/test_collatz.py
+-rw-r--r--   0 root         (0) root         (0)     1556 2023-05-17 22:24:55.000000 salt-analytics-framework-0.3.0/tests/integration/collectors/salt_exec/test_config_get.py
+-rw-r--r--   0 root         (0) root         (0)     1399 2023-05-17 22:24:55.000000 salt-analytics-framework-0.3.0/tests/integration/conftest.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 22:24:55.000000 salt-analytics-framework-0.3.0/tests/integration/engines/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-17 22:24:55.000000 salt-analytics-framework-0.3.0/tests/integration/engines/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1517 2023-05-17 22:24:55.000000 salt-analytics-framework-0.3.0/tests/integration/engines/test_engine.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 22:24:55.000000 salt-analytics-framework-0.3.0/tests/unit/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-17 22:24:55.000000 salt-analytics-framework-0.3.0/tests/unit/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 22:24:55.000000 salt-analytics-framework-0.3.0/tests/unit/process/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-17 22:24:55.000000 salt-analytics-framework-0.3.0/tests/unit/process/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3803 2023-05-17 22:24:55.000000 salt-analytics-framework-0.3.0/tests/unit/process/test_regex_mask.py
+-rw-r--r--   0 root         (0) root         (0)     5436 2023-05-17 22:24:55.000000 salt-analytics-framework-0.3.0/tests/unit/process/test_shannon_mask.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 22:24:55.000000 salt-analytics-framework-0.3.0/tests/unit/salt/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-17 22:24:55.000000 salt-analytics-framework-0.3.0/tests/unit/salt/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 22:24:55.000000 salt-analytics-framework-0.3.0/tests/unit/salt/engines/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-17 22:24:55.000000 salt-analytics-framework-0.3.0/tests/unit/salt/engines/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 22:24:55.000000 salt-analytics-framework-0.3.0/tools/
+-rw-r--r--   0 root         (0) root         (0)       89 2023-05-17 22:24:55.000000 salt-analytics-framework-0.3.0/tools/.ruff.toml
+-rw-r--r--   0 root         (0) root         (0)      334 2023-05-17 22:24:55.000000 salt-analytics-framework-0.3.0/tools/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5495 2023-05-17 22:24:55.000000 salt-analytics-framework-0.3.0/tools/ci.py
+-rw-r--r--   0 root         (0) root         (0)     1383 2023-05-17 22:24:55.000000 salt-analytics-framework-0.3.0/tools/pre_commit.py
+-rw-r--r--   0 root         (0) root         (0)     1382 2023-05-17 22:24:55.000000 salt-analytics-framework-0.3.0/tools/pre_commit.py~
```

### Comparing `salt-analytics-framework-0.2.0/.coveragerc` & `salt-analytics-framework-0.3.0/.coveragerc`

 * *Files identical despite different names*

### Comparing `salt-analytics-framework-0.2.0/.github/actions/setup-actionlint/action.yml` & `salt-analytics-framework-0.3.0/.github/actions/setup-actionlint/action.yml`

 * *Files identical despite different names*

### Comparing `salt-analytics-framework-0.2.0/.github/workflows/ci.yml` & `salt-analytics-framework-0.3.0/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `salt-analytics-framework-0.2.0/.gitignore` & `salt-analytics-framework-0.3.0/.gitignore`

 * *Files identical despite different names*

### Comparing `salt-analytics-framework-0.2.0/.pre-commit-config.yaml` & `salt-analytics-framework-0.3.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `salt-analytics-framework-0.2.0/.pre-commit-hooks/check-changelog-entries.py` & `salt-analytics-framework-0.3.0/.pre-commit-hooks/check-changelog-entries.py`

 * *Files identical despite different names*

### Comparing `salt-analytics-framework-0.2.0/.pre-commit-hooks/check-cli-examples.py` & `salt-analytics-framework-0.3.0/.pre-commit-hooks/check-cli-examples.py`

 * *Files identical despite different names*

### Comparing `salt-analytics-framework-0.2.0/.pre-commit-hooks/copyright-headers.py` & `salt-analytics-framework-0.3.0/.pre-commit-hooks/copyright-headers.py`

 * *Files identical despite different names*

### Comparing `salt-analytics-framework-0.2.0/.pre-commit-hooks/make-autodocs.py` & `salt-analytics-framework-0.3.0/.pre-commit-hooks/make-autodocs.py`

 * *Files identical despite different names*

### Comparing `salt-analytics-framework-0.2.0/.pre-commit-hooks/sort-pylint-spelling-words.py` & `salt-analytics-framework-0.3.0/.pre-commit-hooks/sort-pylint-spelling-words.py`

 * *Files identical despite different names*

### Comparing `salt-analytics-framework-0.2.0/.pylint-spelling-words` & `salt-analytics-framework-0.3.0/.pylint-spelling-words`

 * *Files identical despite different names*

### Comparing `salt-analytics-framework-0.2.0/CHANGELOG.rst` & `salt-analytics-framework-0.3.0/CHANGELOG.rst`

 * *Files 8% similar despite different names*

```diff
@@ -10,14 +10,23 @@
 **Deprecations** section of releases.
 
 .. towncrier-draft-entries::
 
 .. towncrier release notes start
 
 
+0.3.0 (2023-05-17)
+==================
+
+Improvements
+------------
+
+- `#40 <https://github.com/saltstack/pytest-skip-markers/issues/40>`_: Allow the file collector to read from multiple files at a time
+
+
 0.2.0 (2023-05-16)
 ==================
 
 Improvements
 ------------
 
 - `#31 <https://github.com/saltstack/pytest-skip-markers/issues/31>`_: Refactored the logs collector into a generic file collector
```

### Comparing `salt-analytics-framework-0.2.0/CODE_OF_CONDUCT.md` & `salt-analytics-framework-0.3.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `salt-analytics-framework-0.2.0/CONTRIBUTING.md` & `salt-analytics-framework-0.3.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `salt-analytics-framework-0.2.0/LICENSE` & `salt-analytics-framework-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `salt-analytics-framework-0.2.0/NOTICE` & `salt-analytics-framework-0.3.0/NOTICE`

 * *Files identical despite different names*

### Comparing `salt-analytics-framework-0.2.0/PKG-INFO` & `salt-analytics-framework-0.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: salt-analytics-framework
-Version: 0.2.0
+Version: 0.3.0
 Summary: Salt Analytics Framework
 Home-page: https://github.com/saltstack/salt-analytics-framework
 Author: Pedro Algarvio
 Author-email: palgarvio@vmware.com
 License: Apache Software License
 Project-URL: Source, https://github.com/saltstack/salt-analytics-framework
 Project-URL: Tracker, https://github.com/saltstack/salt-analytics-framework/issues
```

### Comparing `salt-analytics-framework-0.2.0/README.rst` & `salt-analytics-framework-0.3.0/README.rst`

 * *Files identical despite different names*

### Comparing `salt-analytics-framework-0.2.0/changelog/_template.rst` & `salt-analytics-framework-0.3.0/changelog/_template.rst`

 * *Files identical despite different names*

### Comparing `salt-analytics-framework-0.2.0/docs/Makefile` & `salt-analytics-framework-0.3.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `salt-analytics-framework-0.2.0/docs/conf.py` & `salt-analytics-framework-0.3.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `salt-analytics-framework-0.2.0/docs/index.rst` & `salt-analytics-framework-0.3.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `salt-analytics-framework-0.2.0/docs/make.bat` & `salt-analytics-framework-0.3.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `salt-analytics-framework-0.2.0/docs/ref/saf.collect.rst` & `salt-analytics-framework-0.3.0/docs/ref/saf.collect.rst`

 * *Files identical despite different names*

### Comparing `salt-analytics-framework-0.2.0/docs/ref/saf.forward.rst` & `salt-analytics-framework-0.3.0/docs/ref/saf.forward.rst`

 * *Files identical despite different names*

### Comparing `salt-analytics-framework-0.2.0/docs/ref/saf.process.rst` & `salt-analytics-framework-0.3.0/docs/ref/saf.process.rst`

 * *Files identical despite different names*

### Comparing `salt-analytics-framework-0.2.0/docs/ref/saf.rst` & `salt-analytics-framework-0.3.0/docs/ref/saf.rst`

 * *Files identical despite different names*

### Comparing `salt-analytics-framework-0.2.0/noxfile.py` & `salt-analytics-framework-0.3.0/noxfile.py`

 * *Files identical despite different names*

### Comparing `salt-analytics-framework-0.2.0/pyproject.toml` & `salt-analytics-framework-0.3.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `salt-analytics-framework-0.2.0/setup.cfg` & `salt-analytics-framework-0.3.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `salt-analytics-framework-0.2.0/src/saf/__init__.py` & `salt-analytics-framework-0.3.0/src/saf/__init__.py`

 * *Files identical despite different names*

### Comparing `salt-analytics-framework-0.2.0/src/saf/collect/beacons.py` & `salt-analytics-framework-0.3.0/src/saf/collect/beacons.py`

 * *Files identical despite different names*

### Comparing `salt-analytics-framework-0.2.0/src/saf/collect/file.py` & `salt-analytics-framework-0.3.0/src/saf/collect/file.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,37 +1,38 @@
 # Copyright 2021-2023 VMware, Inc.
 # SPDX-License-Identifier: Apache-2.0
 """
 A file collector plugin.
 """
 from __future__ import annotations
 
-import asyncio
 import logging
 import os
 import pathlib  # noqa: TCH003
+from contextlib import ExitStack
+from typing import Any
 from typing import AsyncIterator
+from typing import List
 from typing import Type
 
 from saf.models import CollectConfigBase
 from saf.models import CollectedEvent
 from saf.models import PipelineRunContext
 
 log = logging.getLogger(__name__)
 
 
 class FileCollectConfig(CollectConfigBase):
     """
     Configuration schema for the file collect plugin.
     """
 
-    path: pathlib.Path
+    paths: List[pathlib.Path]
     # If true, starts at the beginning of a file, else at the end
     backfill: bool = False
-    wait: float = 5
     # If true, reads to the end of the file, else one line at a time
     multiline: bool = False
     file_mode: str = "r"
 
 
 def get_config_schema() -> Type[FileCollectConfig]:
     """
@@ -41,25 +42,31 @@
 
 
 async def collect(*, ctx: PipelineRunContext[FileCollectConfig]) -> AsyncIterator[CollectedEvent]:
     """
     Method called to collect file contents.
     """
     config = ctx.config
-    try:
-        with config.path.open(mode=config.file_mode) as rfh:
-            # If we do not need to gather older content, we put the cursor at the end of file
+
+    with ExitStack() as stack:
+        try:
+            handles = {
+                str(path): stack.enter_context(path.open(mode=config.file_mode))
+                for path in config.paths
+            }
             if not config.backfill:
-                rfh.seek(0, os.SEEK_END)
+                for handle in handles.values():
+                    handle.seek(0, os.SEEK_END)
             while True:
-                if config.multiline:
-                    contents = rfh.readlines()
-                else:
-                    contents = rfh.readline()
-                if not contents:
-                    await asyncio.sleep(config.wait)
-                else:
-                    event = CollectedEvent(data={"lines": contents})
-                    yield event
-
-    except FileNotFoundError as exc:
-        log.debug("File %s not found", exc.filename)
+                for path, rfh in handles.items():
+                    contents: Any
+                    if config.multiline:
+                        contents = rfh.readlines()
+                    else:
+                        contents = rfh.readline()
+                    if contents and isinstance(contents, str):
+                        contents = [contents]
+                    if contents is not None:
+                        for line in contents:
+                            yield CollectedEvent(data={"lines": line, "source": path})
+        except FileNotFoundError as exc:
+            log.debug("File %s not found", exc.filename)
```

### Comparing `salt-analytics-framework-0.2.0/src/saf/collect/noop.py` & `salt-analytics-framework-0.3.0/src/saf/collect/noop.py`

 * *Files identical despite different names*

### Comparing `salt-analytics-framework-0.2.0/src/saf/collect/salt_exec.py` & `salt-analytics-framework-0.3.0/src/saf/collect/salt_exec.py`

 * *Files identical despite different names*

### Comparing `salt-analytics-framework-0.2.0/src/saf/forward/disk.py` & `salt-analytics-framework-0.3.0/src/saf/forward/disk.py`

 * *Files identical despite different names*

### Comparing `salt-analytics-framework-0.2.0/src/saf/forward/noop.py` & `salt-analytics-framework-0.3.0/src/saf/forward/noop.py`

 * *Files identical despite different names*

### Comparing `salt-analytics-framework-0.2.0/src/saf/forward/test.py` & `salt-analytics-framework-0.3.0/src/saf/forward/test.py`

 * *Files identical despite different names*

### Comparing `salt-analytics-framework-0.2.0/src/saf/manager.py` & `salt-analytics-framework-0.3.0/src/saf/manager.py`

 * *Files identical despite different names*

### Comparing `salt-analytics-framework-0.2.0/src/saf/models.py` & `salt-analytics-framework-0.3.0/src/saf/models.py`

 * *Files identical despite different names*

### Comparing `salt-analytics-framework-0.2.0/src/saf/pipeline.py` & `salt-analytics-framework-0.3.0/src/saf/pipeline.py`

 * *Files identical despite different names*

### Comparing `salt-analytics-framework-0.2.0/src/saf/plugins.py` & `salt-analytics-framework-0.3.0/src/saf/plugins.py`

 * *Files identical despite different names*

### Comparing `salt-analytics-framework-0.2.0/src/saf/process/noop.py` & `salt-analytics-framework-0.3.0/src/saf/process/noop.py`

 * *Files identical despite different names*

### Comparing `salt-analytics-framework-0.2.0/src/saf/process/regex_mask.py` & `salt-analytics-framework-0.3.0/src/saf/process/regex_mask.py`

 * *Files identical despite different names*

### Comparing `salt-analytics-framework-0.2.0/src/saf/process/regex_mask.pyi` & `salt-analytics-framework-0.3.0/src/saf/process/regex_mask.pyi`

 * *Files identical despite different names*

### Comparing `salt-analytics-framework-0.2.0/src/saf/process/shannon_mask.py` & `salt-analytics-framework-0.3.0/src/saf/process/shannon_mask.py`

 * *Files identical despite different names*

### Comparing `salt-analytics-framework-0.2.0/src/saf/saltext/engines/analytics.py` & `salt-analytics-framework-0.3.0/src/saf/saltext/engines/analytics.py`

 * *Files identical despite different names*

### Comparing `salt-analytics-framework-0.2.0/src/saf/utils/eventbus.py` & `salt-analytics-framework-0.3.0/src/saf/utils/eventbus.py`

 * *Files identical despite different names*

### Comparing `salt-analytics-framework-0.2.0/src/salt_analytics_framework.egg-info/PKG-INFO` & `salt-analytics-framework-0.3.0/src/salt_analytics_framework.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: salt-analytics-framework
-Version: 0.2.0
+Version: 0.3.0
 Summary: Salt Analytics Framework
 Home-page: https://github.com/saltstack/salt-analytics-framework
 Author: Pedro Algarvio
 Author-email: palgarvio@vmware.com
 License: Apache Software License
 Project-URL: Source, https://github.com/saltstack/salt-analytics-framework
 Project-URL: Tracker, https://github.com/saltstack/salt-analytics-framework/issues
```

### Comparing `salt-analytics-framework-0.2.0/src/salt_analytics_framework.egg-info/SOURCES.txt` & `salt-analytics-framework-0.3.0/src/salt_analytics_framework.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `salt-analytics-framework-0.2.0/src/salt_analytics_framework.egg-info/requires.txt` & `salt-analytics-framework-0.3.0/src/salt_analytics_framework.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `salt-analytics-framework-0.2.0/tests/__init__.py` & `salt-analytics-framework-0.3.0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `salt-analytics-framework-0.2.0/tests/conftest.py` & `salt-analytics-framework-0.3.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `salt-analytics-framework-0.2.0/tests/functional/conftest.py` & `salt-analytics-framework-0.3.0/tests/functional/conftest.py`

 * *Files identical despite different names*

### Comparing `salt-analytics-framework-0.2.0/tests/functional/forwarders/test_concurrency.py` & `salt-analytics-framework-0.3.0/tests/functional/forwarders/test_concurrency.py`

 * *Files identical despite different names*

### Comparing `salt-analytics-framework-0.2.0/tests/functional/manager/conftest.py` & `salt-analytics-framework-0.3.0/tests/functional/manager/conftest.py`

 * *Files identical despite different names*

### Comparing `salt-analytics-framework-0.2.0/tests/functional/manager/test_disabled_pipeline.py` & `salt-analytics-framework-0.3.0/tests/functional/manager/test_disabled_pipeline.py`

 * *Files identical despite different names*

### Comparing `salt-analytics-framework-0.2.0/tests/functional/manager/test_enabled_pipeline.py` & `salt-analytics-framework-0.3.0/tests/functional/manager/test_enabled_pipeline.py`

 * *Files identical despite different names*

### Comparing `salt-analytics-framework-0.2.0/tests/integration/collectors/beacons/test_memusage.py` & `salt-analytics-framework-0.3.0/tests/integration/collectors/beacons/test_memusage.py`

 * *Files identical despite different names*

### Comparing `salt-analytics-framework-0.2.0/tests/integration/collectors/beacons/test_multiple.py` & `salt-analytics-framework-0.3.0/tests/integration/collectors/beacons/test_multiple.py`

 * *Files identical despite different names*

### Comparing `salt-analytics-framework-0.2.0/tests/integration/collectors/beacons/test_status.py` & `salt-analytics-framework-0.3.0/tests/integration/collectors/beacons/test_status.py`

 * *Files identical despite different names*

### Comparing `salt-analytics-framework-0.2.0/tests/integration/collectors/salt_exec/conftest.py` & `salt-analytics-framework-0.3.0/tests/integration/collectors/salt_exec/conftest.py`

 * *Files identical despite different names*

### Comparing `salt-analytics-framework-0.2.0/tests/integration/collectors/salt_exec/test_arg.py` & `salt-analytics-framework-0.3.0/tests/integration/collectors/salt_exec/test_arg.py`

 * *Files identical despite different names*

### Comparing `salt-analytics-framework-0.2.0/tests/integration/collectors/salt_exec/test_collatz.py` & `salt-analytics-framework-0.3.0/tests/integration/collectors/salt_exec/test_collatz.py`

 * *Files identical despite different names*

### Comparing `salt-analytics-framework-0.2.0/tests/integration/collectors/salt_exec/test_config_get.py` & `salt-analytics-framework-0.3.0/tests/integration/collectors/salt_exec/test_config_get.py`

 * *Files identical despite different names*

### Comparing `salt-analytics-framework-0.2.0/tests/integration/conftest.py` & `salt-analytics-framework-0.3.0/tests/integration/conftest.py`

 * *Files identical despite different names*

### Comparing `salt-analytics-framework-0.2.0/tests/integration/engines/test_engine.py` & `salt-analytics-framework-0.3.0/tests/integration/engines/test_engine.py`

 * *Files identical despite different names*

### Comparing `salt-analytics-framework-0.2.0/tests/unit/process/test_regex_mask.py` & `salt-analytics-framework-0.3.0/tests/unit/process/test_regex_mask.py`

 * *Files identical despite different names*

### Comparing `salt-analytics-framework-0.2.0/tests/unit/process/test_shannon_mask.py` & `salt-analytics-framework-0.3.0/tests/unit/process/test_shannon_mask.py`

 * *Files identical despite different names*

### Comparing `salt-analytics-framework-0.2.0/tools/ci.py` & `salt-analytics-framework-0.3.0/tools/ci.py`

 * *Files identical despite different names*

### Comparing `salt-analytics-framework-0.2.0/tools/pre_commit.py` & `salt-analytics-framework-0.3.0/tools/pre_commit.py`

 * *Files identical despite different names*

### Comparing `salt-analytics-framework-0.2.0/tools/pre_commit.py~` & `salt-analytics-framework-0.3.0/tools/pre_commit.py~`

 * *Files identical despite different names*

