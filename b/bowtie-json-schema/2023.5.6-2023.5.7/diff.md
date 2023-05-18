# Comparing `tmp/bowtie_json_schema-2023.5.6.tar.gz` & `tmp/bowtie_json_schema-2023.5.7.tar.gz`

## Comparing `bowtie_json_schema-2023.5.6.tar` & `bowtie_json_schema-2023.5.7.tar`

### file list

```diff
@@ -1,49 +1,49 @@
--rw-r--r--   0        0        0      837 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.5.6/.flake8
--rw-r--r--   0        0        0     2422 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.5.6/.pre-commit-config.yaml
--rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.5.6/.readthedocs.yml
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.5.6/io-schema.json -> bowtie/schemas/io-schema.json
--rw-r--r--   0        0        0     4933 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.5.6/noxfile.py
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.5.6/test-requirements.in
--rw-r--r--   0        0        0     1990 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.5.6/test-requirements.txt
--rw-r--r--   0        0        0      622 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.5.6/.github/SECURITY.md
--rw-r--r--   0        0        0     3981 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.5.6/.github/dependabot.yml
--rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.5.6/.github/release.yml
--rw-r--r--   0        0        0     2937 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.5.6/.github/workflows/ci.yml
--rw-r--r--   0        0        0      604 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.5.6/.github/workflows/dependabot-merge.yml
--rw-r--r--   0        0        0     2810 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.5.6/.github/workflows/images.yml
--rw-r--r--   0        0        0     2195 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.5.6/.github/workflows/report.yml
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.5.6/bowtie/__init__.py
--rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.5.6/bowtie/__main__.py
--rw-r--r--   0        0        0    30648 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.5.6/bowtie/_cli.py
--rw-r--r--   0        0        0     8501 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.5.6/bowtie/_commands.py
--rw-r--r--   0        0        0    10460 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.5.6/bowtie/_core.py
--rw-r--r--   0        0        0    13733 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.5.6/bowtie/_report.py
--rw-r--r--   0        0        0      782 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.5.6/bowtie/exceptions.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.5.6/bowtie/schemas/__init__.py
--rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.5.6/docs/Makefile
--rw-r--r--   0        0        0     1914 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.5.6/docs/cli.rst
--rw-r--r--   0        0        0     2219 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.5.6/docs/conf.py
--rw-r--r--   0        0        0     2865 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.5.6/docs/contributing.rst
--rw-r--r--   0        0        0    34138 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.5.6/docs/implementers.rst
--rw-r--r--   0        0        0     3339 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.5.6/docs/index.rst
--rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.5.6/docs/requirements.in
--rw-r--r--   0        0        0     3559 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.5.6/docs/requirements.txt
--rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.5.6/docs/spelling-wordlist.txt
--rw-r--r--   0        0        0   629179 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.5.6/docs/_static/dreamed.png
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.5.6/tests/__init__.py
--rw-r--r--   0        0        0      369 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.5.6/tests/conftest.py
--rw-r--r--   0        0        0    22418 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.5.6/tests/test_integration.py
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.5.6/tests/fauxmplementations/badsonschema/Dockerfile
--rwxr-xr-x   0        0        0     1832 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.5.6/tests/fauxmplementations/badsonschema/badsonschema
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.5.6/tests/fauxmplementations/envsonschema/Dockerfile
--rwxr-xr-x   0        0        0     4529 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.5.6/tests/fauxmplementations/envsonschema/envsonschema
--rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.5.6/tests/fauxmplementations/lintsonschema/Dockerfile
--rw-r--r--   0        0        0    12345 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.5.6/tests/fauxmplementations/lintsonschema/io-schema.json
--rwxr-xr-x   0        0        0     2890 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.5.6/tests/fauxmplementations/lintsonschema/lintsonschema
--rw-r--r--   0        0        0    28309 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.5.6/bowtie/templates/report.html.j2
--rw-r--r--   0        0        0    14287 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.5.6/bowtie/schemas/io-schema.json
--rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.5.6/.gitignore
--rw-r--r--   0        0        0     1060 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.5.6/LICENSE
--rw-r--r--   0        0        0     1777 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.5.6/README.rst
--rw-r--r--   0        0        0     3908 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.5.6/pyproject.toml
--rw-r--r--   0        0        0     3325 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.5.6/PKG-INFO
+-rw-r--r--   0        0        0      837 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.5.7/.flake8
+-rw-r--r--   0        0        0     2422 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.5.7/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.5.7/.readthedocs.yml
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.5.7/io-schema.json -> bowtie/schemas/io-schema.json
+-rw-r--r--   0        0        0     4933 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.5.7/noxfile.py
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.5.7/test-requirements.in
+-rw-r--r--   0        0        0     1990 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.5.7/test-requirements.txt
+-rw-r--r--   0        0        0      622 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.5.7/.github/SECURITY.md
+-rw-r--r--   0        0        0     3981 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.5.7/.github/dependabot.yml
+-rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.5.7/.github/release.yml
+-rw-r--r--   0        0        0     2937 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.5.7/.github/workflows/ci.yml
+-rw-r--r--   0        0        0      604 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.5.7/.github/workflows/dependabot-merge.yml
+-rw-r--r--   0        0        0     2809 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.5.7/.github/workflows/images.yml
+-rw-r--r--   0        0        0     2195 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.5.7/.github/workflows/report.yml
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.5.7/bowtie/__init__.py
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.5.7/bowtie/__main__.py
+-rw-r--r--   0        0        0    30648 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.5.7/bowtie/_cli.py
+-rw-r--r--   0        0        0     8501 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.5.7/bowtie/_commands.py
+-rw-r--r--   0        0        0    10460 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.5.7/bowtie/_core.py
+-rw-r--r--   0        0        0    13733 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.5.7/bowtie/_report.py
+-rw-r--r--   0        0        0      782 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.5.7/bowtie/exceptions.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.5.7/bowtie/schemas/__init__.py
+-rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.5.7/docs/Makefile
+-rw-r--r--   0        0        0     1914 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.5.7/docs/cli.rst
+-rw-r--r--   0        0        0     2219 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.5.7/docs/conf.py
+-rw-r--r--   0        0        0     2865 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.5.7/docs/contributing.rst
+-rw-r--r--   0        0        0    34138 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.5.7/docs/implementers.rst
+-rw-r--r--   0        0        0     3339 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.5.7/docs/index.rst
+-rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.5.7/docs/requirements.in
+-rw-r--r--   0        0        0     3559 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.5.7/docs/requirements.txt
+-rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.5.7/docs/spelling-wordlist.txt
+-rw-r--r--   0        0        0   629179 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.5.7/docs/_static/dreamed.png
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.5.7/tests/__init__.py
+-rw-r--r--   0        0        0      369 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.5.7/tests/conftest.py
+-rw-r--r--   0        0        0    22418 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.5.7/tests/test_integration.py
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.5.7/tests/fauxmplementations/badsonschema/Dockerfile
+-rwxr-xr-x   0        0        0     1832 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.5.7/tests/fauxmplementations/badsonschema/badsonschema
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.5.7/tests/fauxmplementations/envsonschema/Dockerfile
+-rwxr-xr-x   0        0        0     4529 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.5.7/tests/fauxmplementations/envsonschema/envsonschema
+-rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.5.7/tests/fauxmplementations/lintsonschema/Dockerfile
+-rw-r--r--   0        0        0    12345 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.5.7/tests/fauxmplementations/lintsonschema/io-schema.json
+-rwxr-xr-x   0        0        0     2890 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.5.7/tests/fauxmplementations/lintsonschema/lintsonschema
+-rw-r--r--   0        0        0    28309 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.5.7/bowtie/templates/report.html.j2
+-rw-r--r--   0        0        0    14287 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.5.7/bowtie/schemas/io-schema.json
+-rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.5.7/.gitignore
+-rw-r--r--   0        0        0     1060 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.5.7/LICENSE
+-rw-r--r--   0        0        0     1777 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.5.7/README.rst
+-rw-r--r--   0        0        0     3908 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.5.7/pyproject.toml
+-rw-r--r--   0        0        0     3325 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.5.7/PKG-INFO
```

### Comparing `bowtie_json_schema-2023.5.6/.flake8` & `bowtie_json_schema-2023.5.7/.flake8`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.5.6/.pre-commit-config.yaml` & `bowtie_json_schema-2023.5.7/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.5.6/noxfile.py` & `bowtie_json_schema-2023.5.7/noxfile.py`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.5.6/test-requirements.txt` & `bowtie_json_schema-2023.5.7/test-requirements.txt`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.5.6/.github/SECURITY.md` & `bowtie_json_schema-2023.5.7/.github/SECURITY.md`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.5.6/.github/dependabot.yml` & `bowtie_json_schema-2023.5.7/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.5.6/.github/workflows/ci.yml` & `bowtie_json_schema-2023.5.7/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.5.6/.github/workflows/dependabot-merge.yml` & `bowtie_json_schema-2023.5.7/.github/workflows/dependabot-merge.yml`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.5.6/.github/workflows/images.yml` & `bowtie_json_schema-2023.5.7/.github/workflows/images.yml`

 * *Files 5% similar despite different names*

```diff
@@ -90,9 +90,9 @@
         with:
           python-version: "3.x"
         if: steps.changes.outputs.impl == 'true'
 
       - name: Smoke Test
         run: |
           python3 -m pip install bowtie-json-schema
-          bowtie smoke -i "localhost/${{ steps.build_image.outputs.image }}"
+          bowtie smoke -i "${{ steps.build_image.outputs.image-with-tag }}"
         if: steps.changes.outputs.impl == 'true' || (github.event_name == 'push' && startsWith(github.event.ref, 'refs/tags'))
```

### Comparing `bowtie_json_schema-2023.5.6/.github/workflows/report.yml` & `bowtie_json_schema-2023.5.7/.github/workflows/report.yml`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.5.6/bowtie/_cli.py` & `bowtie_json_schema-2023.5.7/bowtie/_cli.py`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.5.6/bowtie/_commands.py` & `bowtie_json_schema-2023.5.7/bowtie/_commands.py`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.5.6/bowtie/_core.py` & `bowtie_json_schema-2023.5.7/bowtie/_core.py`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.5.6/bowtie/_report.py` & `bowtie_json_schema-2023.5.7/bowtie/_report.py`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.5.6/bowtie/exceptions.py` & `bowtie_json_schema-2023.5.7/bowtie/exceptions.py`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.5.6/docs/Makefile` & `bowtie_json_schema-2023.5.7/docs/Makefile`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.5.6/docs/cli.rst` & `bowtie_json_schema-2023.5.7/docs/cli.rst`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.5.6/docs/conf.py` & `bowtie_json_schema-2023.5.7/docs/conf.py`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.5.6/docs/contributing.rst` & `bowtie_json_schema-2023.5.7/docs/contributing.rst`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.5.6/docs/implementers.rst` & `bowtie_json_schema-2023.5.7/docs/implementers.rst`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.5.6/docs/index.rst` & `bowtie_json_schema-2023.5.7/docs/index.rst`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.5.6/docs/requirements.txt` & `bowtie_json_schema-2023.5.7/docs/requirements.txt`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.5.6/docs/_static/dreamed.png` & `bowtie_json_schema-2023.5.7/docs/_static/dreamed.png`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.5.6/tests/test_integration.py` & `bowtie_json_schema-2023.5.7/tests/test_integration.py`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.5.6/tests/fauxmplementations/badsonschema/badsonschema` & `bowtie_json_schema-2023.5.7/tests/fauxmplementations/badsonschema/badsonschema`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.5.6/tests/fauxmplementations/envsonschema/envsonschema` & `bowtie_json_schema-2023.5.7/tests/fauxmplementations/envsonschema/envsonschema`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.5.6/tests/fauxmplementations/lintsonschema/io-schema.json` & `bowtie_json_schema-2023.5.7/tests/fauxmplementations/lintsonschema/io-schema.json`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.5.6/tests/fauxmplementations/lintsonschema/lintsonschema` & `bowtie_json_schema-2023.5.7/tests/fauxmplementations/lintsonschema/lintsonschema`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.5.6/bowtie/templates/report.html.j2` & `bowtie_json_schema-2023.5.7/bowtie/templates/report.html.j2`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.5.6/bowtie/schemas/io-schema.json` & `bowtie_json_schema-2023.5.7/bowtie/schemas/io-schema.json`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.5.6/.gitignore` & `bowtie_json_schema-2023.5.7/.gitignore`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.5.6/LICENSE` & `bowtie_json_schema-2023.5.7/LICENSE`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.5.6/README.rst` & `bowtie_json_schema-2023.5.7/README.rst`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.5.6/pyproject.toml` & `bowtie_json_schema-2023.5.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.5.6/PKG-INFO` & `bowtie_json_schema-2023.5.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bowtie-json-schema
-Version: 2023.5.6
+Version: 2023.5.7
 Summary: A meta-validator for the JSON Schema specification.
 Project-URL: Documentation, https://bowtie-json-schema.readthedocs.io/
 Project-URL: Homepage, https://github.com/bowtie-json-schema/bowtie
 Project-URL: Issues, https://github.com/bowtie-json-schema/bowtie/issues/
 Project-URL: Source, https://github.com/bowtie-json-schema/bowtie
 Author: Julian Berman
 Author-email: Julian+bowtie@GrayVines.com
```

