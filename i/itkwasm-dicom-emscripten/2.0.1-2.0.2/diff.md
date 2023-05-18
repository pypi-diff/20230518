# Comparing `tmp/itkwasm_dicom_emscripten-2.0.1.tar.gz` & `tmp/itkwasm_dicom_emscripten-2.0.2.tar.gz`

## Comparing `itkwasm_dicom_emscripten-2.0.1.tar` & `itkwasm_dicom_emscripten-2.0.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 itkwasm_dicom_emscripten-2.0.1/itkwasm_dicom_emscripten/__init__.py
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 itkwasm_dicom_emscripten-2.0.1/itkwasm_dicom_emscripten/_version.py
--rw-r--r--   0        0        0     2511 2020-02-02 00:00:00.000000 itkwasm_dicom_emscripten-2.0.1/itkwasm_dicom_emscripten/apply_presentation_state_to_image_async.py
--rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 itkwasm_dicom_emscripten-2.0.1/itkwasm_dicom_emscripten/js_package.py
--rw-r--r--   0        0        0     4431 2020-02-02 00:00:00.000000 itkwasm_dicom_emscripten-2.0.1/itkwasm_dicom_emscripten/read_dicom_encapsulated_pdf_async.py
--rw-r--r--   0        0        0    10552 2020-02-02 00:00:00.000000 itkwasm_dicom_emscripten-2.0.1/itkwasm_dicom_emscripten/structured_report_to_html_async.py
--rw-r--r--   0        0        0     5025 2020-02-02 00:00:00.000000 itkwasm_dicom_emscripten-2.0.1/itkwasm_dicom_emscripten/structured_report_to_text_async.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 itkwasm_dicom_emscripten-2.0.1/test/__init__.py
--rw-r--r--   0        0        0     1199 2020-02-02 00:00:00.000000 itkwasm_dicom_emscripten-2.0.1/test/fixtures.py
--rw-r--r--   0        0        0     2395 2020-02-02 00:00:00.000000 itkwasm_dicom_emscripten-2.0.1/test/test_apply_presentation_state_to_image_async.py
--rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 itkwasm_dicom_emscripten-2.0.1/test/test_itkwasm_dicom.py
--rw-r--r--   0        0        0      931 2020-02-02 00:00:00.000000 itkwasm_dicom_emscripten-2.0.1/test/test_read_dicom_encapsulated_pdf_async.py
--rw-r--r--   0        0        0     3961 2020-02-02 00:00:00.000000 itkwasm_dicom_emscripten-2.0.1/test/test_structured_report_to_html_async.py
--rw-r--r--   0        0        0     1237 2020-02-02 00:00:00.000000 itkwasm_dicom_emscripten-2.0.1/test/test_structured_report_to_text_async.py
--rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 itkwasm_dicom_emscripten-2.0.1/.gitignore
--rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 itkwasm_dicom_emscripten-2.0.1/README.md
--rw-r--r--   0        0        0     1661 2020-02-02 00:00:00.000000 itkwasm_dicom_emscripten-2.0.1/pyproject.toml
--rw-r--r--   0        0        0     1442 2020-02-02 00:00:00.000000 itkwasm_dicom_emscripten-2.0.1/PKG-INFO
+-rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 itkwasm_dicom_emscripten-2.0.2/itkwasm_dicom_emscripten/__init__.py
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 itkwasm_dicom_emscripten-2.0.2/itkwasm_dicom_emscripten/_version.py
+-rw-r--r--   0        0        0     2511 2020-02-02 00:00:00.000000 itkwasm_dicom_emscripten-2.0.2/itkwasm_dicom_emscripten/apply_presentation_state_to_image_async.py
+-rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 itkwasm_dicom_emscripten-2.0.2/itkwasm_dicom_emscripten/js_package.py
+-rw-r--r--   0        0        0     4431 2020-02-02 00:00:00.000000 itkwasm_dicom_emscripten-2.0.2/itkwasm_dicom_emscripten/read_dicom_encapsulated_pdf_async.py
+-rw-r--r--   0        0        0    10552 2020-02-02 00:00:00.000000 itkwasm_dicom_emscripten-2.0.2/itkwasm_dicom_emscripten/structured_report_to_html_async.py
+-rw-r--r--   0        0        0     5025 2020-02-02 00:00:00.000000 itkwasm_dicom_emscripten-2.0.2/itkwasm_dicom_emscripten/structured_report_to_text_async.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 itkwasm_dicom_emscripten-2.0.2/test/__init__.py
+-rw-r--r--   0        0        0     1199 2020-02-02 00:00:00.000000 itkwasm_dicom_emscripten-2.0.2/test/fixtures.py
+-rw-r--r--   0        0        0     2395 2020-02-02 00:00:00.000000 itkwasm_dicom_emscripten-2.0.2/test/test_apply_presentation_state_to_image_async.py
+-rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 itkwasm_dicom_emscripten-2.0.2/test/test_itkwasm_dicom.py
+-rw-r--r--   0        0        0      931 2020-02-02 00:00:00.000000 itkwasm_dicom_emscripten-2.0.2/test/test_read_dicom_encapsulated_pdf_async.py
+-rw-r--r--   0        0        0     3961 2020-02-02 00:00:00.000000 itkwasm_dicom_emscripten-2.0.2/test/test_structured_report_to_html_async.py
+-rw-r--r--   0        0        0     1237 2020-02-02 00:00:00.000000 itkwasm_dicom_emscripten-2.0.2/test/test_structured_report_to_text_async.py
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 itkwasm_dicom_emscripten-2.0.2/.gitignore
+-rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 itkwasm_dicom_emscripten-2.0.2/README.md
+-rw-r--r--   0        0        0     1869 2020-02-02 00:00:00.000000 itkwasm_dicom_emscripten-2.0.2/pyproject.toml
+-rw-r--r--   0        0        0     1665 2020-02-02 00:00:00.000000 itkwasm_dicom_emscripten-2.0.2/PKG-INFO
```

### Comparing `itkwasm_dicom_emscripten-2.0.1/itkwasm_dicom_emscripten/apply_presentation_state_to_image_async.py` & `itkwasm_dicom_emscripten-2.0.2/itkwasm_dicom_emscripten/apply_presentation_state_to_image_async.py`

 * *Files identical despite different names*

### Comparing `itkwasm_dicom_emscripten-2.0.1/itkwasm_dicom_emscripten/read_dicom_encapsulated_pdf_async.py` & `itkwasm_dicom_emscripten-2.0.2/itkwasm_dicom_emscripten/read_dicom_encapsulated_pdf_async.py`

 * *Files identical despite different names*

### Comparing `itkwasm_dicom_emscripten-2.0.1/itkwasm_dicom_emscripten/structured_report_to_html_async.py` & `itkwasm_dicom_emscripten-2.0.2/itkwasm_dicom_emscripten/structured_report_to_html_async.py`

 * *Files identical despite different names*

### Comparing `itkwasm_dicom_emscripten-2.0.1/itkwasm_dicom_emscripten/structured_report_to_text_async.py` & `itkwasm_dicom_emscripten-2.0.2/itkwasm_dicom_emscripten/structured_report_to_text_async.py`

 * *Files identical despite different names*

### Comparing `itkwasm_dicom_emscripten-2.0.1/test/fixtures.py` & `itkwasm_dicom_emscripten-2.0.2/test/fixtures.py`

 * *Files identical despite different names*

### Comparing `itkwasm_dicom_emscripten-2.0.1/test/test_apply_presentation_state_to_image_async.py` & `itkwasm_dicom_emscripten-2.0.2/test/test_apply_presentation_state_to_image_async.py`

 * *Files identical despite different names*

### Comparing `itkwasm_dicom_emscripten-2.0.1/test/test_itkwasm_dicom.py` & `itkwasm_dicom_emscripten-2.0.2/test/test_itkwasm_dicom.py`

 * *Files identical despite different names*

### Comparing `itkwasm_dicom_emscripten-2.0.1/test/test_read_dicom_encapsulated_pdf_async.py` & `itkwasm_dicom_emscripten-2.0.2/test/test_read_dicom_encapsulated_pdf_async.py`

 * *Files identical despite different names*

### Comparing `itkwasm_dicom_emscripten-2.0.1/test/test_structured_report_to_html_async.py` & `itkwasm_dicom_emscripten-2.0.2/test/test_structured_report_to_html_async.py`

 * *Files identical despite different names*

### Comparing `itkwasm_dicom_emscripten-2.0.1/test/test_structured_report_to_text_async.py` & `itkwasm_dicom_emscripten-2.0.2/test/test_structured_report_to_text_async.py`

 * *Files identical despite different names*

### Comparing `itkwasm_dicom_emscripten-2.0.1/pyproject.toml` & `itkwasm_dicom_emscripten-2.0.2/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -40,14 +40,18 @@
 
 [tool.hatch.envs.default]
 dependencies = [
   "pytest",
   "pytest-pyodide",
 ]
 
+[project.urls]
+Home = "https://itk-wasm-dicom-python-docs.on.fleek.co"
+Source = "https://github.com/InsightSoftwareConsortium/itk-wasm"
+Issues = "https://github.com/InsightSoftwareConsortium/itk-wasm/issues"
 
 [tool.hatch.envs.default.scripts]
 test = [
   "hatch build -t wheel",
   "pytest --dist-dir=./dist --rt=chrome",
 ]
 download-pyodide = [
```

