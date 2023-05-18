# Comparing `tmp/sphinx_reredirects-0.1.1.tar.gz` & `tmp/sphinx_reredirects-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sphinx_reredirects-0.1.1.tar", last modified: Thu Jun  9 10:23:18 2022, max compression
+gzip compressed data, was "sphinx_reredirects-0.1.2.tar", last modified: Thu May 18 07:52:14 2023, max compression
```

## Comparing `sphinx_reredirects-0.1.1.tar` & `sphinx_reredirects-0.1.2.tar`

### file list

```diff
@@ -1,15 +1,19 @@
-drwxr-xr-x   0 libor      (501) staff       (20)        0 2022-06-09 10:23:18.099221 sphinx_reredirects-0.1.1/
--rw-r--r--   0 libor      (501) staff       (20)     1508 2021-04-22 09:16:28.000000 sphinx_reredirects-0.1.1/LICENSE
--rw-r--r--   0 libor      (501) staff       (20)     2633 2022-06-09 10:23:18.099085 sphinx_reredirects-0.1.1/PKG-INFO
--rw-r--r--   0 libor      (501) staff       (20)     1755 2022-06-09 10:19:26.000000 sphinx_reredirects-0.1.1/README.rst
--rw-r--r--   0 libor      (501) staff       (20)       80 2022-06-09 10:08:47.000000 sphinx_reredirects-0.1.1/pyproject.toml
--rw-r--r--   0 libor      (501) staff       (20)       38 2022-06-09 10:23:18.099263 sphinx_reredirects-0.1.1/setup.cfg
--rw-r--r--   0 libor      (501) staff       (20)     1110 2022-06-09 10:15:22.000000 sphinx_reredirects-0.1.1/setup.py
-drwxr-xr-x   0 libor      (501) staff       (20)        0 2022-06-09 10:23:18.098399 sphinx_reredirects-0.1.1/sphinx_reredirects/
--rw-r--r--   0 libor      (501) staff       (20)     4889 2022-06-09 08:46:18.000000 sphinx_reredirects-0.1.1/sphinx_reredirects/__init__.py
-drwxr-xr-x   0 libor      (501) staff       (20)        0 2022-06-09 10:23:18.098918 sphinx_reredirects-0.1.1/sphinx_reredirects.egg-info/
--rw-r--r--   0 libor      (501) staff       (20)     2633 2022-06-09 10:23:17.000000 sphinx_reredirects-0.1.1/sphinx_reredirects.egg-info/PKG-INFO
--rw-r--r--   0 libor      (501) staff       (20)      282 2022-06-09 10:23:18.000000 sphinx_reredirects-0.1.1/sphinx_reredirects.egg-info/SOURCES.txt
--rw-r--r--   0 libor      (501) staff       (20)        1 2022-06-09 10:23:17.000000 sphinx_reredirects-0.1.1/sphinx_reredirects.egg-info/dependency_links.txt
--rw-r--r--   0 libor      (501) staff       (20)        7 2022-06-09 10:23:18.000000 sphinx_reredirects-0.1.1/sphinx_reredirects.egg-info/requires.txt
--rw-r--r--   0 libor      (501) staff       (20)       19 2022-06-09 10:23:18.000000 sphinx_reredirects-0.1.1/sphinx_reredirects.egg-info/top_level.txt
+drwxr-xr-x   0 liborjelinek   (501) staff       (20)        0 2023-05-18 07:52:14.700889 sphinx_reredirects-0.1.2/
+-rw-r--r--   0 liborjelinek   (501) staff       (20)     1508 2023-05-18 07:08:01.000000 sphinx_reredirects-0.1.2/LICENSE
+-rw-r--r--   0 liborjelinek   (501) staff       (20)     2620 2023-05-18 07:52:14.700748 sphinx_reredirects-0.1.2/PKG-INFO
+-rw-r--r--   0 liborjelinek   (501) staff       (20)     1743 2023-05-18 07:38:25.000000 sphinx_reredirects-0.1.2/README.rst
+-rw-r--r--   0 liborjelinek   (501) staff       (20)       80 2023-05-18 07:08:01.000000 sphinx_reredirects-0.1.2/pyproject.toml
+-rw-r--r--   0 liborjelinek   (501) staff       (20)       38 2023-05-18 07:52:14.700930 sphinx_reredirects-0.1.2/setup.cfg
+-rw-r--r--   0 liborjelinek   (501) staff       (20)     1110 2023-05-18 07:33:10.000000 sphinx_reredirects-0.1.2/setup.py
+drwxr-xr-x   0 liborjelinek   (501) staff       (20)        0 2023-05-18 07:52:14.698729 sphinx_reredirects-0.1.2/sphinx_reredirects/
+-rw-r--r--   0 liborjelinek   (501) staff       (20)     5897 2023-05-18 07:08:01.000000 sphinx_reredirects-0.1.2/sphinx_reredirects/__init__.py
+drwxr-xr-x   0 liborjelinek   (501) staff       (20)        0 2023-05-18 07:52:14.699693 sphinx_reredirects-0.1.2/sphinx_reredirects.egg-info/
+-rw-r--r--   0 liborjelinek   (501) staff       (20)     2620 2023-05-18 07:52:14.000000 sphinx_reredirects-0.1.2/sphinx_reredirects.egg-info/PKG-INFO
+-rw-r--r--   0 liborjelinek   (501) staff       (20)      355 2023-05-18 07:52:14.000000 sphinx_reredirects-0.1.2/sphinx_reredirects.egg-info/SOURCES.txt
+-rw-r--r--   0 liborjelinek   (501) staff       (20)        1 2023-05-18 07:52:14.000000 sphinx_reredirects-0.1.2/sphinx_reredirects.egg-info/dependency_links.txt
+-rw-r--r--   0 liborjelinek   (501) staff       (20)        7 2023-05-18 07:52:14.000000 sphinx_reredirects-0.1.2/sphinx_reredirects.egg-info/requires.txt
+-rw-r--r--   0 liborjelinek   (501) staff       (20)       19 2023-05-18 07:52:14.000000 sphinx_reredirects-0.1.2/sphinx_reredirects.egg-info/top_level.txt
+drwxr-xr-x   0 liborjelinek   (501) staff       (20)        0 2023-05-18 07:52:14.700399 sphinx_reredirects-0.1.2/tests/
+-rw-r--r--   0 liborjelinek   (501) staff       (20)     4565 2023-05-18 07:08:01.000000 sphinx_reredirects-0.1.2/tests/test_end2end.py
+-rw-r--r--   0 liborjelinek   (501) staff       (20)     1348 2023-05-18 07:08:01.000000 sphinx_reredirects-0.1.2/tests/test_placeholders.py
+-rw-r--r--   0 liborjelinek   (501) staff       (20)      598 2023-05-18 07:08:01.000000 sphinx_reredirects-0.1.2/tests/test_wildcards.py
```

### Comparing `sphinx_reredirects-0.1.1/LICENSE` & `sphinx_reredirects-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `sphinx_reredirects-0.1.1/PKG-INFO` & `sphinx_reredirects-0.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sphinx_reredirects
-Version: 0.1.1
+Version: 0.1.2
 Summary: Handles redirects for moved pages in Sphinx documentation projects
 Home-page: https://gitlab.com/documatt/sphinx-reredirects
 Author: Matt from Documatt
 Author-email: matt@documatt.com
 License: BSD3
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
@@ -34,26 +34,26 @@
 
 .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
    :target: https://github.com/psf/black
 
 .. image:: https://img.shields.io/pypi/v/sphinx-reredirects
    :target: https://pypi.org/project/sphinx-reredirects/
 
-sphinx-reredirects is the extension for `Sphinx documentation <https://https://www.sphinx-doc.org/>`_ projects that handles redirects for moved pages. It generates HTML pages with meta refresh redirects to the new page location to prevent 404 errors if you rename or move your documents.
+sphinx-reredirects is the extension for `Sphinx documentation <https://www.sphinx-doc.org/>`_ projects that handles redirects for moved pages. It generates HTML pages with meta refresh redirects to the new page location to prevent 404 errors if you rename or move your documents.
 
 * docs: https://documatt.gitlab.io/sphinx-reredirects
 * code: https://gitlab.com/documatt/sphinx-reredirects where issues and contributions are welcome
 
 Good URLs are never changing URLs. But if you must, sphinx-reredirects helps you manage redirects with ease and from the single place in project's ``conf.py``.  For example, if you rename document ``start`` to ``intro``, and tell it to sphinx-reredirects, it will generate HTML page ``start.html`` with ``<meta http-equiv="refresh" content="0; url=intro.html">``. The extension supports wildcards and moving to different domain too.
 
 *****
 About
 *****
 
-sphinx-reredirects started from the urge to manage redirects for all documents during moving our *Tech writer at work blog* to the new domain https://techwriter.documatt.com.
+sphinx-reredirects started from the urge to manage redirects for all documents during moving our *Tech writer at work blog* to the new domain https://documatt.com/blog/.
 
 *****
 Legal
 *****
 
 Forward Arrow icon by `Icons8 <https://icons8.com/icon/74159/forward-arrow>`_.
```

### Comparing `sphinx_reredirects-0.1.1/README.rst` & `sphinx_reredirects-0.1.2/README.rst`

 * *Files 6% similar despite different names*

```diff
@@ -10,27 +10,27 @@
 
 .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
    :target: https://github.com/psf/black
 
 .. image:: https://img.shields.io/pypi/v/sphinx-reredirects
    :target: https://pypi.org/project/sphinx-reredirects/
 
-sphinx-reredirects is the extension for `Sphinx documentation <https://https://www.sphinx-doc.org/>`_ projects that handles redirects for moved pages. It generates HTML pages with meta refresh redirects to the new page location to prevent 404 errors if you rename or move your documents.
+sphinx-reredirects is the extension for `Sphinx documentation <https://www.sphinx-doc.org/>`_ projects that handles redirects for moved pages. It generates HTML pages with meta refresh redirects to the new page location to prevent 404 errors if you rename or move your documents.
 
 * docs: https://documatt.gitlab.io/sphinx-reredirects
 * code: https://gitlab.com/documatt/sphinx-reredirects where issues and contributions are welcome
 
 Good URLs are never changing URLs. But if you must, sphinx-reredirects helps you manage redirects with ease and from the single place in project's ``conf.py``.  For example, if you rename document ``start`` to ``intro``, and tell it to sphinx-reredirects, it will generate HTML page ``start.html`` with ``<meta http-equiv="refresh" content="0; url=intro.html">``. The extension supports wildcards and moving to different domain too.
 
 *****
 About
 *****
 
-sphinx-reredirects started from the urge to manage redirects for all documents during moving our *Tech writer at work blog* to the new domain https://techwriter.documatt.com.
+sphinx-reredirects started from the urge to manage redirects for all documents during moving our *Tech writer at work blog* to the new domain https://documatt.com/blog/.
 
 *****
 Legal
 *****
 
 Forward Arrow icon by `Icons8 <https://icons8.com/icon/74159/forward-arrow>`_.
 
-sphinx-reredirects is licensed under BSD3.
+sphinx-reredirects is licensed under BSD3.
```

### Comparing `sphinx_reredirects-0.1.1/setup.py` & `sphinx_reredirects-0.1.2/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name="sphinx_reredirects",
-    version="0.1.1",
+    version="0.1.2",
     url="https://gitlab.com/documatt/sphinx-reredirects",
     license="BSD3",
     author="Matt from Documatt",
     author_email="matt@documatt.com",
     description="Handles redirects for moved pages in Sphinx documentation " "projects",
     long_description=open("README.rst", encoding="utf-8").read(),
     long_description_content_type="text/x-rst",
```

### Comparing `sphinx_reredirects-0.1.1/sphinx_reredirects/__init__.py` & `sphinx_reredirects-0.1.2/sphinx_reredirects/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,35 +2,37 @@
 from fnmatch import fnmatch
 from pathlib import Path
 from string import Template
 from typing import Dict, Mapping, Optional, Sequence
 
 from sphinx.application import Sphinx
 from sphinx.util import logging
+from sphinx.util.osutil import SEP
 
 OPTION_REDIRECTS = "redirects"
 OPTION_REDIRECTS_DEFAULT: Dict[str, str] = {}
 
 OPTION_TEMPLATE_FILE = "redirect_html_template_file"
 OPTION_TEMPLATE_FILE_DEFAULT = None
 
 REDIRECT_FILE_DEFAULT_TEMPLATE = '<html><head><meta http-equiv="refresh" content="0; url=${to_uri}"></head></html>'  # noqa: E501
 
 logger = logging.getLogger(__name__)
 
 wildcard_pattern = re.compile(r"[\*\?\[\]]")
 
 
-def setup(app: Sphinx) -> None:
+def setup(app: Sphinx) -> Dict:
     """
     Extension setup, called by Sphinx
     """
     app.connect("html-collect-pages", init)
     app.add_config_value(OPTION_REDIRECTS, OPTION_REDIRECTS_DEFAULT, "env")
     app.add_config_value(OPTION_TEMPLATE_FILE, OPTION_TEMPLATE_FILE_DEFAULT, "env")
+    return dict(parallel_read_safe=True)
 
 
 def init(app: Sphinx) -> Optional[Sequence]:
     if not app.config[OPTION_REDIRECTS]:
         logger.debug("No redirects configured")
         return []
 
@@ -75,37 +77,60 @@
 
             for doc in expanded_docs:
                 new_target = self._apply_placeholders(doc, target)
                 to_be_redirected[doc] = new_target
 
         return to_be_redirected
 
+    def docname_out_path(self, docname: str, suffix: str) -> Sequence[str]:
+        """
+        For a Sphinx docname (the path to a source document without suffix),
+        returns path to outfile that would be created by the used builder.
+        """
+        # Return as-is, if the docname already has been passed with a suffix
+        if docname.endswith(suffix):
+            return [docname]
+
+        # Remove any trailing slashes, except for "/"" index
+        if len(docname) > 1 and docname.endswith(SEP):
+            docname = docname.rstrip(SEP)
+
+        # Figure out whether we have dirhtml builder
+        out_uri = self.app.builder.get_target_uri(docname=docname)  # type: ignore
+
+        if not out_uri.endswith(suffix):
+            # If dirhtml builder is used, need to append "index"
+            return [out_uri, "index"]
+
+        # Otherwise, convert e.g. 'source' to 'source.html'
+        return [out_uri]
+
     def create_redirects(self, to_be_redirected: Mapping[str, str]) -> None:
         """Create actual redirect file for each pair in passed mapping of \
         docnames to targets."""
-        if self.app.config.html_file_suffix is not None:
-            suffix = self.app.config.html_file_suffix
-        else:
+
+        # Corresponds to value of `html_file_suffix`, but takes into account
+        # modifications done by the builder class
+        try:
+            suffix = self.app.builder.out_suffix  # type: ignore
+        except Exception:
             suffix = ".html"
 
-        for doc, target in to_be_redirected.items():
-            redirect_file_abs = Path(self.app.outdir).joinpath(doc).with_suffix(suffix)
+        for docname, target in to_be_redirected.items():
+            out = self.docname_out_path(docname, suffix)
+            redirect_file_abs = Path(self.app.outdir).joinpath(*out).with_suffix(suffix)
+
             redirect_file_rel = redirect_file_abs.relative_to(self.app.outdir)
 
             if redirect_file_abs.exists():
                 logger.info(
-                    f"Creating redirect file '{redirect_file_rel}' "
-                    f"pointing to '{target}' that replaces "
-                    f"document '{doc}'."
+                    f"Overwriting '{redirect_file_rel}' with redirect to '{target}'."
                 )
             else:
-                logger.info(
-                    f"Creating redirect file '{redirect_file_rel}' "
-                    f"pointing to '{target}'."
-                )
+                logger.info(f"Creating redirect '{redirect_file_rel}' to '{target}'.")
 
             self._create_redirect_file(redirect_file_abs, target)
 
     @staticmethod
     def _contains_wildcard(text: str) -> bool:
         """Tells whether passed argument contains wildcard characters."""
         return bool(wildcard_pattern.search(text))
```

### Comparing `sphinx_reredirects-0.1.1/sphinx_reredirects.egg-info/PKG-INFO` & `sphinx_reredirects-0.1.2/sphinx_reredirects.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sphinx-reredirects
-Version: 0.1.1
+Version: 0.1.2
 Summary: Handles redirects for moved pages in Sphinx documentation projects
 Home-page: https://gitlab.com/documatt/sphinx-reredirects
 Author: Matt from Documatt
 Author-email: matt@documatt.com
 License: BSD3
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
@@ -34,26 +34,26 @@
 
 .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
    :target: https://github.com/psf/black
 
 .. image:: https://img.shields.io/pypi/v/sphinx-reredirects
    :target: https://pypi.org/project/sphinx-reredirects/
 
-sphinx-reredirects is the extension for `Sphinx documentation <https://https://www.sphinx-doc.org/>`_ projects that handles redirects for moved pages. It generates HTML pages with meta refresh redirects to the new page location to prevent 404 errors if you rename or move your documents.
+sphinx-reredirects is the extension for `Sphinx documentation <https://www.sphinx-doc.org/>`_ projects that handles redirects for moved pages. It generates HTML pages with meta refresh redirects to the new page location to prevent 404 errors if you rename or move your documents.
 
 * docs: https://documatt.gitlab.io/sphinx-reredirects
 * code: https://gitlab.com/documatt/sphinx-reredirects where issues and contributions are welcome
 
 Good URLs are never changing URLs. But if you must, sphinx-reredirects helps you manage redirects with ease and from the single place in project's ``conf.py``.  For example, if you rename document ``start`` to ``intro``, and tell it to sphinx-reredirects, it will generate HTML page ``start.html`` with ``<meta http-equiv="refresh" content="0; url=intro.html">``. The extension supports wildcards and moving to different domain too.
 
 *****
 About
 *****
 
-sphinx-reredirects started from the urge to manage redirects for all documents during moving our *Tech writer at work blog* to the new domain https://techwriter.documatt.com.
+sphinx-reredirects started from the urge to manage redirects for all documents during moving our *Tech writer at work blog* to the new domain https://documatt.com/blog/.
 
 *****
 Legal
 *****
 
 Forward Arrow icon by `Icons8 <https://icons8.com/icon/74159/forward-arrow>`_.
```

