# Comparing `tmp/bowtie_json_schema-2023.5.2.tar.gz` & `tmp/bowtie_json_schema-2023.5.3.tar.gz`

## Comparing `bowtie_json_schema-2023.5.2.tar` & `bowtie_json_schema-2023.5.3.tar`

### file list

```diff
@@ -1,49 +1,49 @@
--rw-r--r--   0        0        0      837 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.5.2/.flake8
--rw-r--r--   0        0        0     2422 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.5.2/.pre-commit-config.yaml
--rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.5.2/.readthedocs.yml
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.5.2/io-schema.json -> bowtie/schemas/io-schema.json
--rw-r--r--   0        0        0     4933 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.5.2/noxfile.py
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.5.2/test-requirements.in
--rw-r--r--   0        0        0     1990 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.5.2/test-requirements.txt
--rw-r--r--   0        0        0      622 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.5.2/.github/SECURITY.md
--rw-r--r--   0        0        0     3981 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.5.2/.github/dependabot.yml
--rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.5.2/.github/release.yml
--rw-r--r--   0        0        0     2937 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.5.2/.github/workflows/ci.yml
--rw-r--r--   0        0        0      604 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.5.2/.github/workflows/dependabot-merge.yml
--rw-r--r--   0        0        0     2809 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.5.2/.github/workflows/images.yml
--rw-r--r--   0        0        0     2195 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.5.2/.github/workflows/report.yml
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.5.2/bowtie/__init__.py
--rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.5.2/bowtie/__main__.py
--rw-r--r--   0        0        0    30648 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.5.2/bowtie/_cli.py
--rw-r--r--   0        0        0     8501 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.5.2/bowtie/_commands.py
--rw-r--r--   0        0        0    10460 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.5.2/bowtie/_core.py
--rw-r--r--   0        0        0    13029 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.5.2/bowtie/_report.py
--rw-r--r--   0        0        0      782 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.5.2/bowtie/exceptions.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.5.2/bowtie/schemas/__init__.py
--rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.5.2/docs/Makefile
--rw-r--r--   0        0        0     1914 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.5.2/docs/cli.rst
--rw-r--r--   0        0        0     2219 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.5.2/docs/conf.py
--rw-r--r--   0        0        0     2865 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.5.2/docs/contributing.rst
--rw-r--r--   0        0        0    34138 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.5.2/docs/implementers.rst
--rw-r--r--   0        0        0     3339 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.5.2/docs/index.rst
--rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.5.2/docs/requirements.in
--rw-r--r--   0        0        0     3559 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.5.2/docs/requirements.txt
--rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.5.2/docs/spelling-wordlist.txt
--rw-r--r--   0        0        0   629179 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.5.2/docs/_static/dreamed.png
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.5.2/tests/__init__.py
--rw-r--r--   0        0        0      369 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.5.2/tests/conftest.py
--rw-r--r--   0        0        0    22418 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.5.2/tests/test_integration.py
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.5.2/tests/fauxmplementations/badsonschema/Dockerfile
--rwxr-xr-x   0        0        0     1832 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.5.2/tests/fauxmplementations/badsonschema/badsonschema
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.5.2/tests/fauxmplementations/envsonschema/Dockerfile
--rwxr-xr-x   0        0        0     4529 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.5.2/tests/fauxmplementations/envsonschema/envsonschema
--rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.5.2/tests/fauxmplementations/lintsonschema/Dockerfile
--rw-r--r--   0        0        0    12345 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.5.2/tests/fauxmplementations/lintsonschema/io-schema.json
--rwxr-xr-x   0        0        0     2890 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.5.2/tests/fauxmplementations/lintsonschema/lintsonschema
--rw-r--r--   0        0        0    28309 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.5.2/bowtie/templates/report.html.j2
--rw-r--r--   0        0        0    14287 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.5.2/bowtie/schemas/io-schema.json
--rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.5.2/.gitignore
--rw-r--r--   0        0        0     1060 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.5.2/LICENSE
--rw-r--r--   0        0        0     1777 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.5.2/README.rst
--rw-r--r--   0        0        0     3932 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.5.2/pyproject.toml
--rw-r--r--   0        0        0     3325 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.5.2/PKG-INFO
+-rw-r--r--   0        0        0      837 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.5.3/.flake8
+-rw-r--r--   0        0        0     2422 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.5.3/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.5.3/.readthedocs.yml
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.5.3/io-schema.json -> bowtie/schemas/io-schema.json
+-rw-r--r--   0        0        0     4933 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.5.3/noxfile.py
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.5.3/test-requirements.in
+-rw-r--r--   0        0        0     1990 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.5.3/test-requirements.txt
+-rw-r--r--   0        0        0      622 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.5.3/.github/SECURITY.md
+-rw-r--r--   0        0        0     3981 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.5.3/.github/dependabot.yml
+-rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.5.3/.github/release.yml
+-rw-r--r--   0        0        0     2937 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.5.3/.github/workflows/ci.yml
+-rw-r--r--   0        0        0      604 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.5.3/.github/workflows/dependabot-merge.yml
+-rw-r--r--   0        0        0     2809 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.5.3/.github/workflows/images.yml
+-rw-r--r--   0        0        0     2195 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.5.3/.github/workflows/report.yml
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.5.3/bowtie/__init__.py
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.5.3/bowtie/__main__.py
+-rw-r--r--   0        0        0    30648 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.5.3/bowtie/_cli.py
+-rw-r--r--   0        0        0     8501 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.5.3/bowtie/_commands.py
+-rw-r--r--   0        0        0    10460 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.5.3/bowtie/_core.py
+-rw-r--r--   0        0        0    13733 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.5.3/bowtie/_report.py
+-rw-r--r--   0        0        0      782 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.5.3/bowtie/exceptions.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.5.3/bowtie/schemas/__init__.py
+-rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.5.3/docs/Makefile
+-rw-r--r--   0        0        0     1914 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.5.3/docs/cli.rst
+-rw-r--r--   0        0        0     2219 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.5.3/docs/conf.py
+-rw-r--r--   0        0        0     2865 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.5.3/docs/contributing.rst
+-rw-r--r--   0        0        0    34138 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.5.3/docs/implementers.rst
+-rw-r--r--   0        0        0     3339 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.5.3/docs/index.rst
+-rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.5.3/docs/requirements.in
+-rw-r--r--   0        0        0     3559 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.5.3/docs/requirements.txt
+-rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.5.3/docs/spelling-wordlist.txt
+-rw-r--r--   0        0        0   629179 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.5.3/docs/_static/dreamed.png
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.5.3/tests/__init__.py
+-rw-r--r--   0        0        0      369 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.5.3/tests/conftest.py
+-rw-r--r--   0        0        0    22418 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.5.3/tests/test_integration.py
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.5.3/tests/fauxmplementations/badsonschema/Dockerfile
+-rwxr-xr-x   0        0        0     1832 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.5.3/tests/fauxmplementations/badsonschema/badsonschema
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.5.3/tests/fauxmplementations/envsonschema/Dockerfile
+-rwxr-xr-x   0        0        0     4529 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.5.3/tests/fauxmplementations/envsonschema/envsonschema
+-rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.5.3/tests/fauxmplementations/lintsonschema/Dockerfile
+-rw-r--r--   0        0        0    12345 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.5.3/tests/fauxmplementations/lintsonschema/io-schema.json
+-rwxr-xr-x   0        0        0     2890 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.5.3/tests/fauxmplementations/lintsonschema/lintsonschema
+-rw-r--r--   0        0        0    28309 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.5.3/bowtie/templates/report.html.j2
+-rw-r--r--   0        0        0    14287 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.5.3/bowtie/schemas/io-schema.json
+-rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.5.3/.gitignore
+-rw-r--r--   0        0        0     1060 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.5.3/LICENSE
+-rw-r--r--   0        0        0     1777 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.5.3/README.rst
+-rw-r--r--   0        0        0     3932 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.5.3/pyproject.toml
+-rw-r--r--   0        0        0     3325 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.5.3/PKG-INFO
```

### Comparing `bowtie_json_schema-2023.5.2/.flake8` & `bowtie_json_schema-2023.5.3/.flake8`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.5.2/.pre-commit-config.yaml` & `bowtie_json_schema-2023.5.3/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.5.2/noxfile.py` & `bowtie_json_schema-2023.5.3/noxfile.py`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.5.2/test-requirements.txt` & `bowtie_json_schema-2023.5.3/test-requirements.txt`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.5.2/.github/SECURITY.md` & `bowtie_json_schema-2023.5.3/.github/SECURITY.md`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.5.2/.github/dependabot.yml` & `bowtie_json_schema-2023.5.3/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.5.2/.github/workflows/ci.yml` & `bowtie_json_schema-2023.5.3/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.5.2/.github/workflows/dependabot-merge.yml` & `bowtie_json_schema-2023.5.3/.github/workflows/dependabot-merge.yml`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.5.2/.github/workflows/images.yml` & `bowtie_json_schema-2023.5.3/.github/workflows/images.yml`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.5.2/.github/workflows/report.yml` & `bowtie_json_schema-2023.5.3/.github/workflows/report.yml`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.5.2/bowtie/_cli.py` & `bowtie_json_schema-2023.5.3/bowtie/_cli.py`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.5.2/bowtie/_commands.py` & `bowtie_json_schema-2023.5.3/bowtie/_commands.py`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.5.2/bowtie/_core.py` & `bowtie_json_schema-2023.5.3/bowtie/_core.py`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.5.2/bowtie/_report.py` & `bowtie_json_schema-2023.5.3/bowtie/_report.py`

 * *Files 4% similar despite different names*

```diff
@@ -310,38 +310,52 @@
                 case["registry"],
                 each["results"],
             )
 
     def generate_badges(self, target_dir: Path, dialect: str):
         label = _DIALECT_URI_TO_SHORTNAME[dialect]
         for impl in self.implementations:
-            if dialect not in impl["dialects"]:
+            dialect_versions = impl["dialects"]
+            if dialect not in dialect_versions:
                 continue
+            supported_drafts = ", ".join(
+                _DIALECT_URI_TO_SHORTNAME[each].removeprefix("Draft ")
+                for each in reversed(dialect_versions)
+            )
             name = impl["name"]
             lang = impl["language"]
             counts = self.counts[impl["image"]]
             total = counts.total_tests
             passed = (
                 total
                 - counts.failed_tests
                 - counts.errored_tests
                 - counts.skipped_tests
             )
             pct = (passed / total) * 100
-            impl_dir = target_dir / f"{lang}-{name}"
-            impl_dir.mkdir(parents=True, exist_ok=True)
             r, g, b = 100 - int(pct), int(pct), 0
-            badge = {
+            badge_per_draft = {
                 "schemaVersion": 1,
                 "label": label,
                 "message": "%d%% Passing" % int(pct),
                 "color": f"{r:02x}{g:02x}{b:02x}",
             }
-            badge_path = impl_dir / f"{label.replace(' ', '_')}.json"
-            badge_path.write_text(json.dumps(badge))
+            comp_dir = target_dir / f"{lang}-{name}" / "compliance"
+            comp_dir.mkdir(parents=True, exist_ok=True)
+            badge_path_per_draft = comp_dir / f"{label.replace(' ', '_')}.json"
+            badge_path_per_draft.write_text(json.dumps(badge_per_draft))
+            badge_supp_draft = {
+                "schemaVersion": 1,
+                "label": "JSON Schema Versions",
+                "message": supported_drafts,
+                "color": "lightgreen",
+            }
+            supp_dir = target_dir / f"{lang}-{name}"
+            badge_path_supp_drafts = supp_dir / "supported_versions.json"
+            badge_path_supp_drafts.write_text(json.dumps(badge_supp_draft))
 
 
 @frozen
 class RunInfo:
     started: str
     bowtie_version: str
     dialect: str
```

### Comparing `bowtie_json_schema-2023.5.2/bowtie/exceptions.py` & `bowtie_json_schema-2023.5.3/bowtie/exceptions.py`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.5.2/docs/Makefile` & `bowtie_json_schema-2023.5.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.5.2/docs/cli.rst` & `bowtie_json_schema-2023.5.3/docs/cli.rst`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.5.2/docs/conf.py` & `bowtie_json_schema-2023.5.3/docs/conf.py`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.5.2/docs/contributing.rst` & `bowtie_json_schema-2023.5.3/docs/contributing.rst`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.5.2/docs/implementers.rst` & `bowtie_json_schema-2023.5.3/docs/implementers.rst`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.5.2/docs/index.rst` & `bowtie_json_schema-2023.5.3/docs/index.rst`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.5.2/docs/requirements.txt` & `bowtie_json_schema-2023.5.3/docs/requirements.txt`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.5.2/docs/_static/dreamed.png` & `bowtie_json_schema-2023.5.3/docs/_static/dreamed.png`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.5.2/tests/test_integration.py` & `bowtie_json_schema-2023.5.3/tests/test_integration.py`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.5.2/tests/fauxmplementations/badsonschema/badsonschema` & `bowtie_json_schema-2023.5.3/tests/fauxmplementations/badsonschema/badsonschema`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.5.2/tests/fauxmplementations/envsonschema/envsonschema` & `bowtie_json_schema-2023.5.3/tests/fauxmplementations/envsonschema/envsonschema`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.5.2/tests/fauxmplementations/lintsonschema/io-schema.json` & `bowtie_json_schema-2023.5.3/tests/fauxmplementations/lintsonschema/io-schema.json`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.5.2/tests/fauxmplementations/lintsonschema/lintsonschema` & `bowtie_json_schema-2023.5.3/tests/fauxmplementations/lintsonschema/lintsonschema`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.5.2/bowtie/templates/report.html.j2` & `bowtie_json_schema-2023.5.3/bowtie/templates/report.html.j2`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.5.2/bowtie/schemas/io-schema.json` & `bowtie_json_schema-2023.5.3/bowtie/schemas/io-schema.json`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.5.2/.gitignore` & `bowtie_json_schema-2023.5.3/.gitignore`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.5.2/LICENSE` & `bowtie_json_schema-2023.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.5.2/README.rst` & `bowtie_json_schema-2023.5.3/README.rst`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.5.2/pyproject.toml` & `bowtie_json_schema-2023.5.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.5.2/PKG-INFO` & `bowtie_json_schema-2023.5.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bowtie-json-schema
-Version: 2023.5.2
+Version: 2023.5.3
 Summary: A meta-validator for the JSON Schema specification.
 Project-URL: Documentation, https://bowtie-json-schema.readthedocs.io/
 Project-URL: Homepage, https://github.com/bowtie-json-schema/bowtie
 Project-URL: Issues, https://github.com/bowtie-json-schema/bowtie/issues/
 Project-URL: Source, https://github.com/bowtie-json-schema/bowtie
 Author: Julian Berman
 Author-email: Julian+bowtie@GrayVines.com
```

