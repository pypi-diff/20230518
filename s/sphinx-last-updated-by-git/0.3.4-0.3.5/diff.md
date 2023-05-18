# Comparing `tmp/sphinx-last-updated-by-git-0.3.4.tar.gz` & `tmp/sphinx-last-updated-by-git-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sphinx-last-updated-by-git-0.3.4.tar", last modified: Fri Sep  2 15:46:30 2022, max compression
+gzip compressed data, was "sphinx-last-updated-by-git-0.3.5.tar", last modified: Thu May 18 12:17:11 2023, max compression
```

## Comparing `sphinx-last-updated-by-git-0.3.4.tar` & `sphinx-last-updated-by-git-0.3.5.tar`

### file list

```diff
@@ -1,17 +1,31 @@
-drwxr-xr-x   0 mg        (1000) mg        (1000)        0 2022-09-02 15:46:30.263684 sphinx-last-updated-by-git-0.3.4/
--rw-r--r--   0 mg        (1000) mg        (1000)     1286 2022-07-22 19:51:31.000000 sphinx-last-updated-by-git-0.3.4/LICENSE
--rw-r--r--   0 mg        (1000) mg        (1000)       17 2020-04-24 12:10:06.000000 sphinx-last-updated-by-git-0.3.4/MANIFEST.in
--rw-r--r--   0 mg        (1000) mg        (1000)     1676 2022-09-02 15:45:26.000000 sphinx-last-updated-by-git-0.3.4/NEWS.rst
--rw-r--r--   0 mg        (1000) mg        (1000)     6150 2022-09-02 15:46:30.263684 sphinx-last-updated-by-git-0.3.4/PKG-INFO
--rw-r--r--   0 mg        (1000) mg        (1000)     5472 2022-09-02 15:41:27.000000 sphinx-last-updated-by-git-0.3.4/README.rst
--rw-r--r--   0 mg        (1000) mg        (1000)       73 2022-09-02 15:46:30.263684 sphinx-last-updated-by-git-0.3.4/setup.cfg
--rw-r--r--   0 mg        (1000) mg        (1000)     1132 2021-02-03 14:42:50.000000 sphinx-last-updated-by-git-0.3.4/setup.py
-drwxr-xr-x   0 mg        (1000) mg        (1000)        0 2022-09-02 15:46:30.259684 sphinx-last-updated-by-git-0.3.4/src/
-drwxr-xr-x   0 mg        (1000) mg        (1000)        0 2022-09-02 15:46:30.263684 sphinx-last-updated-by-git-0.3.4/src/sphinx_last_updated_by_git.egg-info/
--rw-r--r--   0 mg        (1000) mg        (1000)     6150 2022-09-02 15:46:30.000000 sphinx-last-updated-by-git-0.3.4/src/sphinx_last_updated_by_git.egg-info/PKG-INFO
--rw-r--r--   0 mg        (1000) mg        (1000)      410 2022-09-02 15:46:30.000000 sphinx-last-updated-by-git-0.3.4/src/sphinx_last_updated_by_git.egg-info/SOURCES.txt
--rw-r--r--   0 mg        (1000) mg        (1000)        1 2022-09-02 15:46:30.000000 sphinx-last-updated-by-git-0.3.4/src/sphinx_last_updated_by_git.egg-info/dependency_links.txt
--rw-r--r--   0 mg        (1000) mg        (1000)       12 2022-09-02 15:46:30.000000 sphinx-last-updated-by-git-0.3.4/src/sphinx_last_updated_by_git.egg-info/requires.txt
--rw-r--r--   0 mg        (1000) mg        (1000)       27 2022-09-02 15:46:30.000000 sphinx-last-updated-by-git-0.3.4/src/sphinx_last_updated_by_git.egg-info/top_level.txt
--rw-r--r--   0 mg        (1000) mg        (1000)        1 2022-09-02 15:46:29.000000 sphinx-last-updated-by-git-0.3.4/src/sphinx_last_updated_by_git.egg-info/zip-safe
--rw-r--r--   0 mg        (1000) mg        (1000)    11317 2022-09-02 15:43:36.000000 sphinx-last-updated-by-git-0.3.4/src/sphinx_last_updated_by_git.py
+drwxr-xr-x   0 mg        (1000) mg        (1000)        0 2023-05-18 12:17:11.909217 sphinx-last-updated-by-git-0.3.5/
+-rw-r--r--   0 mg        (1000) mg        (1000)       40 2023-02-26 18:19:08.000000 sphinx-last-updated-by-git-0.3.5/.coveragerc
+drwxr-xr-x   0 mg        (1000) mg        (1000)        0 2023-05-18 12:17:11.897217 sphinx-last-updated-by-git-0.3.5/.github/
+drwxr-xr-x   0 mg        (1000) mg        (1000)        0 2023-05-18 12:17:11.901217 sphinx-last-updated-by-git-0.3.5/.github/workflows/
+-rw-r--r--   0 mg        (1000) mg        (1000)     1063 2023-05-18 12:05:43.000000 sphinx-last-updated-by-git-0.3.5/.github/workflows/main.yml
+-rw-r--r--   0 mg        (1000) mg        (1000)       91 2020-04-24 07:52:15.000000 sphinx-last-updated-by-git-0.3.5/.gitignore
+-rw-r--r--   0 mg        (1000) mg        (1000)      270 2020-04-24 07:52:15.000000 sphinx-last-updated-by-git-0.3.5/.gitmodules
+-rw-r--r--   0 mg        (1000) mg        (1000)     1286 2023-05-18 12:12:57.000000 sphinx-last-updated-by-git-0.3.5/LICENSE
+-rw-r--r--   0 mg        (1000) mg        (1000)       17 2020-04-24 12:10:06.000000 sphinx-last-updated-by-git-0.3.5/MANIFEST.in
+-rw-r--r--   0 mg        (1000) mg        (1000)     1744 2023-05-18 12:14:18.000000 sphinx-last-updated-by-git-0.3.5/NEWS.rst
+-rw-r--r--   0 mg        (1000) mg        (1000)     6031 2023-05-18 12:17:11.909217 sphinx-last-updated-by-git-0.3.5/PKG-INFO
+-rw-r--r--   0 mg        (1000) mg        (1000)     5353 2022-10-25 18:20:56.000000 sphinx-last-updated-by-git-0.3.5/README.rst
+-rw-r--r--   0 mg        (1000) mg        (1000)       91 2023-03-08 19:19:39.000000 sphinx-last-updated-by-git-0.3.5/pyproject.toml
+-rw-r--r--   0 mg        (1000) mg        (1000)      136 2022-07-22 19:51:31.000000 sphinx-last-updated-by-git-0.3.5/pytest.ini
+-rw-r--r--   0 mg        (1000) mg        (1000)       38 2023-05-18 12:17:11.909217 sphinx-last-updated-by-git-0.3.5/setup.cfg
+-rw-r--r--   0 mg        (1000) mg        (1000)     1200 2023-04-02 09:33:33.000000 sphinx-last-updated-by-git-0.3.5/setup.py
+drwxr-xr-x   0 mg        (1000) mg        (1000)        0 2023-05-18 12:17:11.901217 sphinx-last-updated-by-git-0.3.5/src/
+drwxr-xr-x   0 mg        (1000) mg        (1000)        0 2023-05-18 12:17:11.905217 sphinx-last-updated-by-git-0.3.5/src/sphinx_last_updated_by_git.egg-info/
+-rw-r--r--   0 mg        (1000) mg        (1000)     6031 2023-05-18 12:17:11.000000 sphinx-last-updated-by-git-0.3.5/src/sphinx_last_updated_by_git.egg-info/PKG-INFO
+-rw-r--r--   0 mg        (1000) mg        (1000)      614 2023-05-18 12:17:11.000000 sphinx-last-updated-by-git-0.3.5/src/sphinx_last_updated_by_git.egg-info/SOURCES.txt
+-rw-r--r--   0 mg        (1000) mg        (1000)        1 2023-05-18 12:17:11.000000 sphinx-last-updated-by-git-0.3.5/src/sphinx_last_updated_by_git.egg-info/dependency_links.txt
+-rw-r--r--   0 mg        (1000) mg        (1000)       12 2023-05-18 12:17:11.000000 sphinx-last-updated-by-git-0.3.5/src/sphinx_last_updated_by_git.egg-info/requires.txt
+-rw-r--r--   0 mg        (1000) mg        (1000)       27 2023-05-18 12:17:11.000000 sphinx-last-updated-by-git-0.3.5/src/sphinx_last_updated_by_git.egg-info/top_level.txt
+-rw-r--r--   0 mg        (1000) mg        (1000)        1 2022-09-02 15:46:29.000000 sphinx-last-updated-by-git-0.3.5/src/sphinx_last_updated_by_git.egg-info/zip-safe
+-rw-r--r--   0 mg        (1000) mg        (1000)    11460 2023-05-18 12:14:18.000000 sphinx-last-updated-by-git-0.3.5/src/sphinx_last_updated_by_git.py
+drwxr-xr-x   0 mg        (1000) mg        (1000)        0 2023-05-18 12:17:11.909217 sphinx-last-updated-by-git-0.3.5/tests/
+-rw-r--r--   0 mg        (1000) mg        (1000)      104 2023-04-02 09:33:51.000000 sphinx-last-updated-by-git-0.3.5/tests/requirements.txt
+-rw-r--r--   0 mg        (1000) mg        (1000)     5095 2022-09-02 13:50:39.000000 sphinx-last-updated-by-git-0.3.5/tests/test_example_repo.py
+-rw-r--r--   0 mg        (1000) mg        (1000)      518 2021-02-08 18:20:35.000000 sphinx-last-updated-by-git-0.3.5/tests/test_singlehtml.py
+-rw-r--r--   0 mg        (1000) mg        (1000)     1584 2023-03-08 19:19:39.000000 sphinx-last-updated-by-git-0.3.5/tests/test_untracked.py
+-rwxr-xr-x   0 mg        (1000) mg        (1000)      392 2021-02-03 14:42:50.000000 sphinx-last-updated-by-git-0.3.5/tests/update_submodules.py
```

### Comparing `sphinx-last-updated-by-git-0.3.4/LICENSE` & `sphinx-last-updated-by-git-0.3.5/LICENSE`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-Copyright (c) 2020-2022, Matthias Geier
+Copyright (c) 2020-2023, Matthias Geier
 
 Redistribution and use in source and binary forms, with or without
 modification, are permitted provided that the following conditions are met:
 
 1. Redistributions of source code must retain the above copyright notice, this
    list of conditions and the following disclaimer.
```

### Comparing `sphinx-last-updated-by-git-0.3.4/NEWS.rst` & `sphinx-last-updated-by-git-0.3.5/NEWS.rst`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,12 @@
+Version 0.3.5 (2023-05-18):
+ * A few build system and test updates
+
 Version 0.3.4 (2022-09-02):
- * add ``git_exclude_patterns`` and ``git_exclude_commits`` features
+ * Add ``git_exclude_patterns`` and ``git_exclude_commits`` features
 
 Version 0.3.3 (2022-08-21):
  * Remove ``page_source_suffix`` from ``context`` if there is no source link
 
 Version 0.3.2 (2022-04-30):
  * Use ``--no-show-signature`` to avoid error when ``log.showSignature`` is on
  * Properly stop ``git log`` subprocess even on error (to avoid warnings)
```

### Comparing `sphinx-last-updated-by-git-0.3.4/PKG-INFO` & `sphinx-last-updated-by-git-0.3.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: sphinx-last-updated-by-git
-Version: 0.3.4
+Version: 0.3.5
 Summary: Get the "last updated" time for each Sphinx page from Git
 Home-page: https://github.com/mgeier/sphinx-last-updated-by-git/
 Author: Matthias Geier
 Author-email: Matthias.Geier@gmail.com
 License: BSD-2-Clause
 Keywords: Sphinx,Git
 Platform: any
 Classifier: Framework :: Sphinx
 Classifier: Framework :: Sphinx :: Extension
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Documentation :: Sphinx
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 License-File: LICENSE
 
 Get the "last updated" time for each Sphinx page from Git
 =========================================================
 
 This is a little Sphinx_ extension that does exactly that.
 It also checks for included files and other dependencies and
@@ -95,21 +95,19 @@
       by means of a ``requirements.txt`` file containing something like this::
 
           sphinx>=2
           sphinx_rtd_theme>=0.5
 
       See also `issue #1`_.
 
-    * Starting with Sphinx version 5.0, there has been a
-      (most likely unintentional) change in how dependencies are determined.
-      This may lead to spurious dependencies which means that some
-      "last changed" dates might be wrong.
-      This will hopefully be fixed in a future Sphinx version.
-      In the meantime, Sphinx version 4.5.0  (with docutils 0.17.1)
-      can be used.
+    * In Sphinx versions 5.0 and 5.1, there has been
+      a regression in how dependencies are determined.
+      This could lead to spurious dependencies
+      which means that some "last changed" dates were wrong.
+      This has been fixed in Sphinx version 5.2 and above.
 
       See also `issue #40`_.
 
 License
     BSD-2-Clause (same as Sphinx itself),
     for more information take a look at the ``LICENSE`` file.
```

### Comparing `sphinx-last-updated-by-git-0.3.4/README.rst` & `sphinx-last-updated-by-git-0.3.5/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -75,21 +75,19 @@
       by means of a ``requirements.txt`` file containing something like this::
 
           sphinx>=2
           sphinx_rtd_theme>=0.5
 
       See also `issue #1`_.
 
-    * Starting with Sphinx version 5.0, there has been a
-      (most likely unintentional) change in how dependencies are determined.
-      This may lead to spurious dependencies which means that some
-      "last changed" dates might be wrong.
-      This will hopefully be fixed in a future Sphinx version.
-      In the meantime, Sphinx version 4.5.0  (with docutils 0.17.1)
-      can be used.
+    * In Sphinx versions 5.0 and 5.1, there has been
+      a regression in how dependencies are determined.
+      This could lead to spurious dependencies
+      which means that some "last changed" dates were wrong.
+      This has been fixed in Sphinx version 5.2 and above.
 
       See also `issue #40`_.
 
 License
     BSD-2-Clause (same as Sphinx itself),
     for more information take a look at the ``LICENSE`` file.
```

### Comparing `sphinx-last-updated-by-git-0.3.4/setup.py` & `sphinx-last-updated-by-git-0.3.5/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,29 +1,33 @@
+from pathlib import Path
+
 from setuptools import setup
 
+
 # "import" __version__
 __version__ = 'unknown'
-for line in open('src/sphinx_last_updated_by_git.py'):
-    if line.startswith('__version__'):
-        exec(line)
-        break
+with Path('src/sphinx_last_updated_by_git.py').open() as f:
+    for line in f:
+        if line.startswith('__version__'):
+            exec(line)
+            break
 
 setup(
     name='sphinx-last-updated-by-git',
     version=__version__,
     package_dir={'': 'src'},
     py_modules=['sphinx_last_updated_by_git'],
-    python_requires='>=3.6',
+    python_requires='>=3.7',
     install_requires=[
         'sphinx>=1.8',
     ],
     author='Matthias Geier',
     author_email='Matthias.Geier@gmail.com',
     description='Get the "last updated" time for each Sphinx page from Git',
-    long_description=open('README.rst').read(),
+    long_description=Path('README.rst').read_text(),
     license='BSD-2-Clause',
     keywords='Sphinx Git'.split(),
     url='https://github.com/mgeier/sphinx-last-updated-by-git/',
     platforms='any',
     classifiers=[
         'Framework :: Sphinx',
         'Framework :: Sphinx :: Extension',
```

### Comparing `sphinx-last-updated-by-git-0.3.4/src/sphinx_last_updated_by_git.egg-info/PKG-INFO` & `sphinx-last-updated-by-git-0.3.5/src/sphinx_last_updated_by_git.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: sphinx-last-updated-by-git
-Version: 0.3.4
+Version: 0.3.5
 Summary: Get the "last updated" time for each Sphinx page from Git
 Home-page: https://github.com/mgeier/sphinx-last-updated-by-git/
 Author: Matthias Geier
 Author-email: Matthias.Geier@gmail.com
 License: BSD-2-Clause
 Keywords: Sphinx,Git
 Platform: any
 Classifier: Framework :: Sphinx
 Classifier: Framework :: Sphinx :: Extension
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Documentation :: Sphinx
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 License-File: LICENSE
 
 Get the "last updated" time for each Sphinx page from Git
 =========================================================
 
 This is a little Sphinx_ extension that does exactly that.
 It also checks for included files and other dependencies and
@@ -95,21 +95,19 @@
       by means of a ``requirements.txt`` file containing something like this::
 
           sphinx>=2
           sphinx_rtd_theme>=0.5
 
       See also `issue #1`_.
 
-    * Starting with Sphinx version 5.0, there has been a
-      (most likely unintentional) change in how dependencies are determined.
-      This may lead to spurious dependencies which means that some
-      "last changed" dates might be wrong.
-      This will hopefully be fixed in a future Sphinx version.
-      In the meantime, Sphinx version 4.5.0  (with docutils 0.17.1)
-      can be used.
+    * In Sphinx versions 5.0 and 5.1, there has been
+      a regression in how dependencies are determined.
+      This could lead to spurious dependencies
+      which means that some "last changed" dates were wrong.
+      This has been fixed in Sphinx version 5.2 and above.
 
       See also `issue #40`_.
 
 License
     BSD-2-Clause (same as Sphinx itself),
     for more information take a look at the ``LICENSE`` file.
```

### Comparing `sphinx-last-updated-by-git-0.3.4/src/sphinx_last_updated_by_git.py` & `sphinx-last-updated-by-git-0.3.5/src/sphinx_last_updated_by_git.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,18 +5,22 @@
 from pathlib import Path
 import subprocess
 
 from sphinx.locale import _
 from sphinx.util.i18n import format_date
 from sphinx.util.logging import getLogger
 from sphinx.util.matching import Matcher
-from sphinx.util import status_iterator
+try:
+    from sphinx.util.display import status_iterator
+except ImportError:
+    # For older Sphinx versions, will be removed in Sphinx 8:
+    from sphinx.util import status_iterator
 
 
-__version__ = '0.3.4'
+__version__ = '0.3.5'
 
 
 logger = getLogger(__name__)
 
 
 def update_file_dates(git_dir, exclude_commits, file_dates):
     """Ask Git for "author date" of given files in given directory.
```

