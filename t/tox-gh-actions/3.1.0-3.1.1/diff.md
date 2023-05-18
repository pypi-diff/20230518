# Comparing `tmp/tox-gh-actions-3.1.0.tar.gz` & `tmp/tox-gh-actions-3.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tox-gh-actions-3.1.0.tar", last modified: Sat Mar 11 06:22:14 2023, max compression
+gzip compressed data, was "tox-gh-actions-3.1.1.tar", last modified: Thu May 18 12:22:18 2023, max compression
```

## Comparing `tox-gh-actions-3.1.0.tar` & `tox-gh-actions-3.1.1.tar`

### file list

```diff
@@ -1,36 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-11 06:22:14.693940 tox-gh-actions-3.1.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-11 06:22:14.689940 tox-gh-actions-3.1.0/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      719 2023-03-11 06:21:50.000000 tox-gh-actions-3.1.0/.github/FUNDING.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-11 06:22:14.689940 tox-gh-actions-3.1.0/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      515 2023-03-11 06:21:50.000000 tox-gh-actions-3.1.0/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-03-11 06:21:50.000000 tox-gh-actions-3.1.0/.github/ISSUE_TEMPLATE/question.md
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-03-11 06:21:50.000000 tox-gh-actions-3.1.0/.github/PULL_REQUEST_TEMPLATE.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-11 06:22:14.693940 tox-gh-actions-3.1.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2795 2023-03-11 06:21:50.000000 tox-gh-actions-3.1.0/.github/workflows/codeql-analysis.yml
--rw-r--r--   0 runner    (1001) docker     (123)      797 2023-03-11 06:21:50.000000 tox-gh-actions-3.1.0/.github/workflows/packaging.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1864 2023-03-11 06:21:50.000000 tox-gh-actions-3.1.0/.github/workflows/tests.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3041 2023-03-11 06:21:50.000000 tox-gh-actions-3.1.0/ARCHITECTURE.md
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-03-11 06:21:50.000000 tox-gh-actions-3.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    11042 2023-03-11 06:22:14.693940 tox-gh-actions-3.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9540 2023-03-11 06:21:50.000000 tox-gh-actions-3.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-03-11 06:21:50.000000 tox-gh-actions-3.1.0/codecov.yml
--rw-r--r--   0 runner    (1001) docker     (123)      670 2023-03-11 06:21:50.000000 tox-gh-actions-3.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     2757 2023-03-11 06:22:14.697939 tox-gh-actions-3.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-11 06:21:50.000000 tox-gh-actions-3.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-11 06:22:14.689940 tox-gh-actions-3.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-11 06:22:14.693940 tox-gh-actions-3.1.0/src/tox_gh_actions/
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-03-11 06:21:50.000000 tox-gh-actions-3.1.0/src/tox_gh_actions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9053 2023-03-11 06:21:50.000000 tox-gh-actions-3.1.0/src/tox_gh_actions/plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-11 06:21:50.000000 tox-gh-actions-3.1.0/src/tox_gh_actions/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-03-11 06:22:14.000000 tox-gh-actions-3.1.0/src/tox_gh_actions/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-11 06:22:14.693940 tox-gh-actions-3.1.0/src/tox_gh_actions.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    11042 2023-03-11 06:22:14.000000 tox-gh-actions-3.1.0/src/tox_gh_actions.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      758 2023-03-11 06:22:14.000000 tox-gh-actions-3.1.0/src/tox_gh_actions.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-11 06:22:14.000000 tox-gh-actions-3.1.0/src/tox_gh_actions.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-03-11 06:22:14.000000 tox-gh-actions-3.1.0/src/tox_gh_actions.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      216 2023-03-11 06:22:14.000000 tox-gh-actions-3.1.0/src/tox_gh_actions.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-03-11 06:22:14.000000 tox-gh-actions-3.1.0/src/tox_gh_actions.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-11 06:22:14.000000 tox-gh-actions-3.1.0/src/tox_gh_actions.egg-info/zip-safe
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-11 06:22:14.693940 tox-gh-actions-3.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2505 2023-03-11 06:21:50.000000 tox-gh-actions-3.1.0/tests/test_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)     8311 2023-03-11 06:21:50.000000 tox-gh-actions-3.1.0/tests/test_plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 12:22:18.605049 tox-gh-actions-3.1.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 12:22:18.601049 tox-gh-actions-3.1.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 12:22:18.601049 tox-gh-actions-3.1.1/.github/DISCUSSION_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      611 2023-05-18 12:22:00.000000 tox-gh-actions-3.1.1/.github/DISCUSSION_TEMPLATE/q-a.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      719 2023-05-18 12:22:00.000000 tox-gh-actions-3.1.1/.github/FUNDING.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 12:22:18.601049 tox-gh-actions-3.1.1/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      515 2023-05-18 12:22:00.000000 tox-gh-actions-3.1.1/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-05-18 12:22:00.000000 tox-gh-actions-3.1.1/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-05-18 12:22:00.000000 tox-gh-actions-3.1.1/.github/PULL_REQUEST_TEMPLATE.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 12:22:18.601049 tox-gh-actions-3.1.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2795 2023-05-18 12:22:00.000000 tox-gh-actions-3.1.1/.github/workflows/codeql-analysis.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      797 2023-05-18 12:22:00.000000 tox-gh-actions-3.1.1/.github/workflows/packaging.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1864 2023-05-18 12:22:00.000000 tox-gh-actions-3.1.1/.github/workflows/tests.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3041 2023-05-18 12:22:00.000000 tox-gh-actions-3.1.1/ARCHITECTURE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-05-18 12:22:00.000000 tox-gh-actions-3.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    11042 2023-05-18 12:22:18.605049 tox-gh-actions-3.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9540 2023-05-18 12:22:00.000000 tox-gh-actions-3.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-18 12:22:00.000000 tox-gh-actions-3.1.1/codecov.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      670 2023-05-18 12:22:00.000000 tox-gh-actions-3.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     2757 2023-05-18 12:22:18.605049 tox-gh-actions-3.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-18 12:22:00.000000 tox-gh-actions-3.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 12:22:18.597049 tox-gh-actions-3.1.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 12:22:18.601049 tox-gh-actions-3.1.1/src/tox_gh_actions/
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-18 12:22:00.000000 tox-gh-actions-3.1.1/src/tox_gh_actions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9271 2023-05-18 12:22:00.000000 tox-gh-actions-3.1.1/src/tox_gh_actions/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 12:22:00.000000 tox-gh-actions-3.1.1/src/tox_gh_actions/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-18 12:22:18.000000 tox-gh-actions-3.1.1/src/tox_gh_actions/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 12:22:18.605049 tox-gh-actions-3.1.1/src/tox_gh_actions.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11042 2023-05-18 12:22:18.000000 tox-gh-actions-3.1.1/src/tox_gh_actions.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      793 2023-05-18 12:22:18.000000 tox-gh-actions-3.1.1/src/tox_gh_actions.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 12:22:18.000000 tox-gh-actions-3.1.1/src/tox_gh_actions.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-18 12:22:18.000000 tox-gh-actions-3.1.1/src/tox_gh_actions.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      216 2023-05-18 12:22:18.000000 tox-gh-actions-3.1.1/src/tox_gh_actions.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-18 12:22:18.000000 tox-gh-actions-3.1.1/src/tox_gh_actions.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 12:22:18.000000 tox-gh-actions-3.1.1/src/tox_gh_actions.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 12:22:18.605049 tox-gh-actions-3.1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2505 2023-05-18 12:22:00.000000 tox-gh-actions-3.1.1/tests/test_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8311 2023-05-18 12:22:00.000000 tox-gh-actions-3.1.1/tests/test_plugin.py
```

### Comparing `tox-gh-actions-3.1.0/.github/FUNDING.yml` & `tox-gh-actions-3.1.1/.github/FUNDING.yml`

 * *Files identical despite different names*

### Comparing `tox-gh-actions-3.1.0/.github/ISSUE_TEMPLATE/bug_report.md` & `tox-gh-actions-3.1.1/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `tox-gh-actions-3.1.0/.github/workflows/codeql-analysis.yml` & `tox-gh-actions-3.1.1/.github/workflows/codeql-analysis.yml`

 * *Files identical despite different names*

### Comparing `tox-gh-actions-3.1.0/.github/workflows/packaging.yml` & `tox-gh-actions-3.1.1/.github/workflows/packaging.yml`

 * *Files identical despite different names*

### Comparing `tox-gh-actions-3.1.0/.github/workflows/tests.yml` & `tox-gh-actions-3.1.1/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `tox-gh-actions-3.1.0/ARCHITECTURE.md` & `tox-gh-actions-3.1.1/ARCHITECTURE.md`

 * *Files identical despite different names*

### Comparing `tox-gh-actions-3.1.0/LICENSE` & `tox-gh-actions-3.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `tox-gh-actions-3.1.0/PKG-INFO` & `tox-gh-actions-3.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tox-gh-actions
-Version: 3.1.0
+Version: 3.1.1
 Summary: Seamless integration of tox into GitHub Actions
 Home-page: https://github.com/ymyzk/tox-gh-actions
 Author: Yusuke Miyazaki
 Author-email: miyazaki.dev@gmail.com
 Maintainer: Yusuke Miyazaki
 Maintainer-email: miyazaki.dev@gmail.com
 License: MIT
```

### Comparing `tox-gh-actions-3.1.0/README.md` & `tox-gh-actions-3.1.1/README.md`

 * *Files identical despite different names*

### Comparing `tox-gh-actions-3.1.0/pyproject.toml` & `tox-gh-actions-3.1.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `tox-gh-actions-3.1.0/setup.cfg` & `tox-gh-actions-3.1.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `tox-gh-actions-3.1.0/src/tox_gh_actions/plugin.py` & `tox-gh-actions-3.1.1/src/tox_gh_actions/plugin.py`

 * *Files 2% similar despite different names*

```diff
@@ -201,20 +201,25 @@
         return False
 
     # The parallel option is not always defined (e.g., `tox run`) so we should check
     # its existence first.
     # As --parallel-live option doesn't seem to be working correctly,
     # this condition is more conservative compared to the plugin for tox 3.
     if hasattr(options, "parallel"):
-        if options.parallel > 0:
-            # Case for `tox p` or `tox -p <num>`
-            return False
-        elif options.parallel is None:
+        if options.parallel is None:
             # Case for `tox -p`
             return False
+        elif isinstance(options.parallel, int) and options.parallel > 0:
+            # Case for `tox p` or `tox -p <num>`
+            return False
+        logger.warning(
+            "tox-gh-actions couldn't understand the parallel option. "
+            "ignoring the given option: %s",
+            options.parallel,
+        )
 
     return True
 
 
 def is_env_specified(config: Config) -> bool:
     """Returns True when environments are explicitly given"""
     if hasattr(config.options, "env") and not config.options.env.is_default_list:
```

### Comparing `tox-gh-actions-3.1.0/src/tox_gh_actions.egg-info/PKG-INFO` & `tox-gh-actions-3.1.1/src/tox_gh_actions.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tox-gh-actions
-Version: 3.1.0
+Version: 3.1.1
 Summary: Seamless integration of tox into GitHub Actions
 Home-page: https://github.com/ymyzk/tox-gh-actions
 Author: Yusuke Miyazaki
 Author-email: miyazaki.dev@gmail.com
 Maintainer: Yusuke Miyazaki
 Maintainer-email: miyazaki.dev@gmail.com
 License: MIT
```

### Comparing `tox-gh-actions-3.1.0/src/tox_gh_actions.egg-info/SOURCES.txt` & `tox-gh-actions-3.1.1/src/tox_gh_actions.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -3,16 +3,17 @@
 README.md
 codecov.yml
 pyproject.toml
 setup.cfg
 setup.py
 .github/FUNDING.yml
 .github/PULL_REQUEST_TEMPLATE.md
+.github/DISCUSSION_TEMPLATE/q-a.yml
 .github/ISSUE_TEMPLATE/bug_report.md
-.github/ISSUE_TEMPLATE/question.md
+.github/ISSUE_TEMPLATE/config.yml
 .github/workflows/codeql-analysis.yml
 .github/workflows/packaging.yml
 .github/workflows/tests.yml
 src/tox_gh_actions/__init__.py
 src/tox_gh_actions/plugin.py
 src/tox_gh_actions/py.typed
 src/tox_gh_actions/version.py
```

### Comparing `tox-gh-actions-3.1.0/tests/test_integration.py` & `tox-gh-actions-3.1.1/tests/test_integration.py`

 * *Files identical despite different names*

### Comparing `tox-gh-actions-3.1.0/tests/test_plugin.py` & `tox-gh-actions-3.1.1/tests/test_plugin.py`

 * *Files identical despite different names*

