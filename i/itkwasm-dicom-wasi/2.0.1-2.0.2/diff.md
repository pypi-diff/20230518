# Comparing `tmp/itkwasm_dicom_wasi-2.0.1.tar.gz` & `tmp/itkwasm_dicom_wasi-2.0.2.tar.gz`

## Comparing `itkwasm_dicom_wasi-2.0.1.tar` & `itkwasm_dicom_wasi-2.0.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0      415 2020-02-02 00:00:00.000000 itkwasm_dicom_wasi-2.0.1/itkwasm_dicom_wasi/__init__.py
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 itkwasm_dicom_wasi-2.0.1/itkwasm_dicom_wasi/_version.py
--rw-r--r--   0        0        0     2746 2020-02-02 00:00:00.000000 itkwasm_dicom_wasi-2.0.1/itkwasm_dicom_wasi/apply_presentation_state_to_image.py
--rw-r--r--   0        0        0     4209 2020-02-02 00:00:00.000000 itkwasm_dicom_wasi-2.0.1/itkwasm_dicom_wasi/read_dicom_encapsulated_pdf.py
--rw-r--r--   0        0        0    10347 2020-02-02 00:00:00.000000 itkwasm_dicom_wasi-2.0.1/itkwasm_dicom_wasi/structured_report_to_html.py
--rw-r--r--   0        0        0     4719 2020-02-02 00:00:00.000000 itkwasm_dicom_wasi-2.0.1/itkwasm_dicom_wasi/structured_report_to_text.py
--rwxr-xr-x   0        0        0  4530704 2020-02-02 00:00:00.000000 itkwasm_dicom_wasi-2.0.1/itkwasm_dicom_wasi/wasm_modules/apply-presentation-state-to-image.wasi.wasm
--rwxr-xr-x   0        0        0  1882868 2020-02-02 00:00:00.000000 itkwasm_dicom_wasi-2.0.1/itkwasm_dicom_wasi/wasm_modules/read-dicom-encapsulated-pdf.wasi.wasm
--rwxr-xr-x   0        0        0  3972262 2020-02-02 00:00:00.000000 itkwasm_dicom_wasi-2.0.1/itkwasm_dicom_wasi/wasm_modules/structured-report-to-html.wasi.wasm
--rwxr-xr-x   0        0        0  3952009 2020-02-02 00:00:00.000000 itkwasm_dicom_wasi-2.0.1/itkwasm_dicom_wasi/wasm_modules/structured-report-to-text.wasi.wasm
--rw-r--r--   0        0        0     2151 2020-02-02 00:00:00.000000 itkwasm_dicom_wasi-2.0.1/test/test_apply_presentation_state_to_image.py
--rw-r--r--   0        0        0      415 2020-02-02 00:00:00.000000 itkwasm_dicom_wasi-2.0.1/test/test_read_dicom_encapsulated_pdf.py
--rw-r--r--   0        0        0     2748 2020-02-02 00:00:00.000000 itkwasm_dicom_wasi-2.0.1/test/test_structured_report_to_html.py
--rw-r--r--   0        0        0      706 2020-02-02 00:00:00.000000 itkwasm_dicom_wasi-2.0.1/test/test_structured_report_to_text.py
--rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 itkwasm_dicom_wasi-2.0.1/.gitignore
--rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 itkwasm_dicom_wasi-2.0.1/README.md
--rw-r--r--   0        0        0     1221 2020-02-02 00:00:00.000000 itkwasm_dicom_wasi-2.0.1/pyproject.toml
--rw-r--r--   0        0        0     1429 2020-02-02 00:00:00.000000 itkwasm_dicom_wasi-2.0.1/PKG-INFO
+-rw-r--r--   0        0        0      415 2020-02-02 00:00:00.000000 itkwasm_dicom_wasi-2.0.2/itkwasm_dicom_wasi/__init__.py
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 itkwasm_dicom_wasi-2.0.2/itkwasm_dicom_wasi/_version.py
+-rw-r--r--   0        0        0     2746 2020-02-02 00:00:00.000000 itkwasm_dicom_wasi-2.0.2/itkwasm_dicom_wasi/apply_presentation_state_to_image.py
+-rw-r--r--   0        0        0     4209 2020-02-02 00:00:00.000000 itkwasm_dicom_wasi-2.0.2/itkwasm_dicom_wasi/read_dicom_encapsulated_pdf.py
+-rw-r--r--   0        0        0    10347 2020-02-02 00:00:00.000000 itkwasm_dicom_wasi-2.0.2/itkwasm_dicom_wasi/structured_report_to_html.py
+-rw-r--r--   0        0        0     4719 2020-02-02 00:00:00.000000 itkwasm_dicom_wasi-2.0.2/itkwasm_dicom_wasi/structured_report_to_text.py
+-rwxr-xr-x   0        0        0  4530704 2020-02-02 00:00:00.000000 itkwasm_dicom_wasi-2.0.2/itkwasm_dicom_wasi/wasm_modules/apply-presentation-state-to-image.wasi.wasm
+-rwxr-xr-x   0        0        0  1882868 2020-02-02 00:00:00.000000 itkwasm_dicom_wasi-2.0.2/itkwasm_dicom_wasi/wasm_modules/read-dicom-encapsulated-pdf.wasi.wasm
+-rwxr-xr-x   0        0        0  3972262 2020-02-02 00:00:00.000000 itkwasm_dicom_wasi-2.0.2/itkwasm_dicom_wasi/wasm_modules/structured-report-to-html.wasi.wasm
+-rwxr-xr-x   0        0        0  3952009 2020-02-02 00:00:00.000000 itkwasm_dicom_wasi-2.0.2/itkwasm_dicom_wasi/wasm_modules/structured-report-to-text.wasi.wasm
+-rw-r--r--   0        0        0     2151 2020-02-02 00:00:00.000000 itkwasm_dicom_wasi-2.0.2/test/test_apply_presentation_state_to_image.py
+-rw-r--r--   0        0        0      415 2020-02-02 00:00:00.000000 itkwasm_dicom_wasi-2.0.2/test/test_read_dicom_encapsulated_pdf.py
+-rw-r--r--   0        0        0     2748 2020-02-02 00:00:00.000000 itkwasm_dicom_wasi-2.0.2/test/test_structured_report_to_html.py
+-rw-r--r--   0        0        0      706 2020-02-02 00:00:00.000000 itkwasm_dicom_wasi-2.0.2/test/test_structured_report_to_text.py
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 itkwasm_dicom_wasi-2.0.2/.gitignore
+-rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 itkwasm_dicom_wasi-2.0.2/README.md
+-rw-r--r--   0        0        0     1430 2020-02-02 00:00:00.000000 itkwasm_dicom_wasi-2.0.2/pyproject.toml
+-rw-r--r--   0        0        0     1652 2020-02-02 00:00:00.000000 itkwasm_dicom_wasi-2.0.2/PKG-INFO
```

### Comparing `itkwasm_dicom_wasi-2.0.1/itkwasm_dicom_wasi/apply_presentation_state_to_image.py` & `itkwasm_dicom_wasi-2.0.2/itkwasm_dicom_wasi/apply_presentation_state_to_image.py`

 * *Files identical despite different names*

### Comparing `itkwasm_dicom_wasi-2.0.1/itkwasm_dicom_wasi/read_dicom_encapsulated_pdf.py` & `itkwasm_dicom_wasi-2.0.2/itkwasm_dicom_wasi/read_dicom_encapsulated_pdf.py`

 * *Files identical despite different names*

### Comparing `itkwasm_dicom_wasi-2.0.1/itkwasm_dicom_wasi/structured_report_to_html.py` & `itkwasm_dicom_wasi-2.0.2/itkwasm_dicom_wasi/structured_report_to_html.py`

 * *Files identical despite different names*

### Comparing `itkwasm_dicom_wasi-2.0.1/itkwasm_dicom_wasi/structured_report_to_text.py` & `itkwasm_dicom_wasi-2.0.2/itkwasm_dicom_wasi/structured_report_to_text.py`

 * *Files identical despite different names*

### Comparing `itkwasm_dicom_wasi-2.0.1/itkwasm_dicom_wasi/wasm_modules/apply-presentation-state-to-image.wasi.wasm` & `itkwasm_dicom_wasi-2.0.2/itkwasm_dicom_wasi/wasm_modules/apply-presentation-state-to-image.wasi.wasm`

 * *Files identical despite different names*

### Comparing `itkwasm_dicom_wasi-2.0.1/itkwasm_dicom_wasi/wasm_modules/read-dicom-encapsulated-pdf.wasi.wasm` & `itkwasm_dicom_wasi-2.0.2/itkwasm_dicom_wasi/wasm_modules/read-dicom-encapsulated-pdf.wasi.wasm`

 * *Files identical despite different names*

### Comparing `itkwasm_dicom_wasi-2.0.1/itkwasm_dicom_wasi/wasm_modules/structured-report-to-html.wasi.wasm` & `itkwasm_dicom_wasi-2.0.2/itkwasm_dicom_wasi/wasm_modules/structured-report-to-html.wasi.wasm`

 * *Files identical despite different names*

### Comparing `itkwasm_dicom_wasi-2.0.1/itkwasm_dicom_wasi/wasm_modules/structured-report-to-text.wasi.wasm` & `itkwasm_dicom_wasi-2.0.2/itkwasm_dicom_wasi/wasm_modules/structured-report-to-text.wasi.wasm`

 * *Files identical despite different names*

### Comparing `itkwasm_dicom_wasi-2.0.1/test/test_apply_presentation_state_to_image.py` & `itkwasm_dicom_wasi-2.0.2/test/test_apply_presentation_state_to_image.py`

 * *Files identical despite different names*

### Comparing `itkwasm_dicom_wasi-2.0.1/test/test_structured_report_to_html.py` & `itkwasm_dicom_wasi-2.0.2/test/test_structured_report_to_html.py`

 * *Files identical despite different names*

### Comparing `itkwasm_dicom_wasi-2.0.1/test/test_structured_report_to_text.py` & `itkwasm_dicom_wasi-2.0.2/test/test_structured_report_to_text.py`

 * *Files identical despite different names*

### Comparing `itkwasm_dicom_wasi-2.0.1/pyproject.toml` & `itkwasm_dicom_wasi-2.0.2/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -33,14 +33,19 @@
 requires-python = ">=3.7"
 dependencies = [
     "itkwasm >= 1.0.b104",
     "importlib_resources",
 
 ]
 
+[project.urls]
+Home = "https://itk-wasm-dicom-python-docs.on.fleek.co"
+Source = "https://github.com/InsightSoftwareConsortium/itk-wasm"
+Issues = "https://github.com/InsightSoftwareConsortium/itk-wasm/issues"
+
 [tool.hatch.version]
 path = "itkwasm_dicom_wasi/_version.py"
 
 [tool.hatch.envs.default]
 dependencies = [
   "pytest",
 ]
```

### Comparing `itkwasm_dicom_wasi-2.0.1/PKG-INFO` & `itkwasm_dicom_wasi-2.0.2/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,13 @@
 Metadata-Version: 2.1
 Name: itkwasm-dicom-wasi
-Version: 2.0.1
+Version: 2.0.2
+Project-URL: Home, https://itk-wasm-dicom-python-docs.on.fleek.co
+Project-URL: Source, https://github.com/InsightSoftwareConsortium/itk-wasm
+Project-URL: Issues, https://github.com/InsightSoftwareConsortium/itk-wasm/issues
 License-Expression: Apache-2.0
 Keywords: itkwasm,wasi,webassembly
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: WebAssembly
 Classifier: Environment :: WebAssembly :: Emscripten
 Classifier: Environment :: WebAssembly :: WASI
 Classifier: Intended Audience :: Developers
```

