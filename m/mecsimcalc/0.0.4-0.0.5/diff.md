# Comparing `tmp/mecsimcalc-0.0.4.tar.gz` & `tmp/mecsimcalc-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mecsimcalc-0.0.4.tar", last modified: Fri May 12 09:18:30 2023, max compression
+gzip compressed data, was "mecsimcalc-0.0.5.tar", last modified: Thu May 18 07:57:43 2023, max compression
```

## Comparing `mecsimcalc-0.0.4.tar` & `mecsimcalc-0.0.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 09:18:30.227098 mecsimcalc-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-05-12 09:18:19.000000 mecsimcalc-0.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    19264 2023-05-12 09:18:30.227098 mecsimcalc-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    18500 2023-05-12 09:18:19.000000 mecsimcalc-0.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 09:18:30.227098 mecsimcalc-0.0.4/mecsimcalc/
--rw-r--r--   0 runner    (1001) docker     (123)      491 2023-05-12 09:18:19.000000 mecsimcalc-0.0.4/mecsimcalc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2848 2023-05-12 09:18:19.000000 mecsimcalc-0.0.4/mecsimcalc/input_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     8012 2023-05-12 09:18:19.000000 mecsimcalc-0.0.4/mecsimcalc/output_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 09:18:30.227098 mecsimcalc-0.0.4/mecsimcalc.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    19264 2023-05-12 09:18:30.000000 mecsimcalc-0.0.4/mecsimcalc.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-05-12 09:18:30.000000 mecsimcalc-0.0.4/mecsimcalc.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 09:18:30.000000 mecsimcalc-0.0.4/mecsimcalc.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-12 09:18:30.000000 mecsimcalc-0.0.4/mecsimcalc.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-12 09:18:30.000000 mecsimcalc-0.0.4/mecsimcalc.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-12 09:18:30.227098 mecsimcalc-0.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-05-12 09:18:19.000000 mecsimcalc-0.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 07:57:43.875123 mecsimcalc-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-05-18 07:57:29.000000 mecsimcalc-0.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    19093 2023-05-18 07:57:43.875123 mecsimcalc-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    18329 2023-05-18 07:57:29.000000 mecsimcalc-0.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 07:57:43.875123 mecsimcalc-0.0.5/mecsimcalc/
+-rw-r--r--   0 runner    (1001) docker     (123)      491 2023-05-18 07:57:29.000000 mecsimcalc-0.0.5/mecsimcalc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2848 2023-05-18 07:57:29.000000 mecsimcalc-0.0.5/mecsimcalc/input_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7923 2023-05-18 07:57:29.000000 mecsimcalc-0.0.5/mecsimcalc/output_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 07:57:43.875123 mecsimcalc-0.0.5/mecsimcalc.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    19093 2023-05-18 07:57:43.000000 mecsimcalc-0.0.5/mecsimcalc.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-05-18 07:57:43.000000 mecsimcalc-0.0.5/mecsimcalc.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 07:57:43.000000 mecsimcalc-0.0.5/mecsimcalc.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-18 07:57:43.000000 mecsimcalc-0.0.5/mecsimcalc.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-18 07:57:43.000000 mecsimcalc-0.0.5/mecsimcalc.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-18 07:57:43.875123 mecsimcalc-0.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-05-18 07:57:29.000000 mecsimcalc-0.0.5/setup.py
```

### Comparing `mecsimcalc-0.0.4/LICENSE` & `mecsimcalc-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `mecsimcalc-0.0.4/PKG-INFO` & `mecsimcalc-0.0.5/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,46 +1,19 @@
-Metadata-Version: 2.1
-Name: mecsimcalc
-Version: 0.0.4
-Summary: Useful functions for MecSimCalc.com
-Author: MecSimCalc
-Author-email: <info@mecsimcalc.com>
-Keywords: python,MecSimCalc,Calculator,Simple
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Developers
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
-Classifier: Operating System :: Unix
-Classifier: Operating System :: MacOS :: MacOS X
-Classifier: Operating System :: Microsoft :: Windows
-Description-Content-Type: text/markdown
-Provides-Extra: dev
-License-File: LICENSE
-
-
----
-sidebar_label: "mecsimcalc Library"
-sidebar_position: 4
----
-
-# Mecsimcalc 0.0.4 documentation
+# Mecsimcalc 0.0.5 documentation
 
 This library is designed to provide a set of functions for handling and converting various types of data, such as base64 encoded data, Pandas DataFrames, and Pillow images.
 
 - [GitHub Repository](https://github.com/MecSimCalc/MecSimCalc-utils)
 - [PyPi Page](https://pypi.org/project/mecsimcalc/)
 
 ## General
 
-<div style={{ display: 'flex', justifyContent: 'space-between', alignItems: 'center' }}>
-  <h3 style={{ margin: 5, padding: 0 }}>decode_file_data</h3>
-  <a href="https://github.com/MecSimCalc/MecSimCalc-utils/blob/main/mecsimcalc/input_utils.py#LL8C1-L30C1" style={{ fontSize: 'larger', marginBottom: '2em', margin: 5, padding: 0 }}><strong>[Source]</strong></a>
+<div style="display: flex; justify-content: space-between; align-items: center;">
+  <h3 style="margin: 5px; padding: 0;">decode_file_data</h3>
+  <a href="https://github.com/MecSimCalc/MecSimCalc-utils/blob/main/mecsimcalc/input_utils.py#LL8C1-L30C1" style="font-size: larger; margin-bottom: 2em; margin: 5px; padding: 0;"><strong>[Source]</strong></a>
 </div>
 
 ```python
 def decode_file_data(encoded_data, metadata = False)
 ```
 
 #### Description:
@@ -68,64 +41,68 @@
 >>> file, metadata = decode_file_data(inputFile, metadata = True)
 >>> print(metadata)
 data:image/jpeg;base64,
 >>> type(file)
 <class '_io.BytesIO'>
 ```
 
-<div style={{ display: 'flex', justifyContent: 'space-between', alignItems: 'center' }}>
-  <h3 style={{ margin: 5, padding: 0 }}>download_text</h3>
-  <a href="https://github.com/MecSimCalc/MecSimCalc-utils/blob/main/mecsimcalc/output_utils.py#LL182C1-L214C1" style={{ fontSize: 'larger', marginBottom: '2em', margin: 5, padding: 0 }}><strong>[Source]</strong></a>
+<div style="display: flex; justify-content: space-between; align-items: center;">
+  <h3 style="margin: 5px; padding: 0;">download_text</h3>
+  <a href="https://github.com/MecSimCalc/MecSimCalc-utils/blob/main/mecsimcalc/output_utils.py#LL182C1-L214C1" style="font-size: larger; margin-bottom: 2em; margin: 5px; padding: 0;"><strong>[Source]</strong></a>
 </div>
 
 ```python
 def download_text(
     text: str,
     filename: str = "myfile",
     extension: str = ".txt",
     download_text: str = "Download File",
 ) -> str:
 ```
 
 #### Description:
+
 Generates a downloadable text file containing the given text
 
 #### Arguments:
+
 | Argument            | Type               | Description                                                                   |
 | ------------------- | ------------------ | ----------------------------------------------------------------------------- |
 | **`text`**          | **str**            | The text to be downloaded                                                     |
 | **`filename`**      | **str** (optional) | The name of the file to be downloaded (Defaults to "myfile")                  |
 | **`extension`**     | **str** (optional) | The file extension of the file to be downloaded (Defaults to ".txt")          |
 | **`download_text`** | **str** (optional) | The text to be displayed on the download button (Defaults to "Download File") |
 
 #### Returns:
+
 | Return Type | Description                           |
 | ----------- | ------------------------------------- |
 | **`str`**   | The HTML code for the download button |
 
 #### Example:
 
 #### Python
 
 ```python
 >>> downloadLink = download_text("Hello World!")
 >>> return {"downloadLink": downloadLink}
 ```
+
 #### Jinja2
 
 ```python
 # outputs.downloadLink is the html download link generated by the function
 {{ outputs.downloadLink }}
 ```
 
 ## Tables/DataFrames
 
-<div style={{ display: 'flex', justifyContent: 'space-between', alignItems: 'center' }}>
-  <h3 style={{ margin: 5, padding: 0 }}>file_to_dataframe</h3>
-  <a href="https://github.com/MecSimCalc/MecSimCalc-utils/blob/main/mecsimcalc/input_utils.py#LL32C1-L52C14" style={{ fontSize: 'larger', marginBottom: '2em', margin: 5, padding: 0 }}><strong>[Source]</strong></a>
+<div style="display: flex; justify-content: space-between; align-items: center;">
+  <h3 style="margin: 5px; padding: 0;">file_to_dataframe</h3>
+  <a href="https://github.com/MecSimCalc/MecSimCalc-utils/blob/main/mecsimcalc/input_utils.py#LL32C1-L52C14" style="font-size: larger; margin-bottom: 2em; margin: 5px; padding: 0;"><strong>[Source]</strong></a>
 </div>
 
 ```python
 def file_to_dataframe(file_data):
 ```
 
 #### Description:
@@ -154,19 +131,21 @@
 
 ```python
 >>> inputFile = inputs['file']
 >>> file = decode_file_data(inputFile)
 >>> df = file_to_dataframe(file)
 >>> print(df)
    A  B  C
+0  a  b  c
+1  d  e  f
 ```
 
-<div style={{ display: 'flex', justifyContent: 'space-between', alignItems: 'center' }}>
-  <h3 style={{ margin: 5, padding: 0 }}>input_to_dataframe</h3>
-  <a href="https://github.com/MecSimCalc/MecSimCalc-utils/blob/main/mecsimcalc/input_utils.py#LL55C1-L67C39" style={{ fontSize: 'larger', marginBottom: '2em', margin: 5, padding: 0 }}><strong>[Source]</strong></a>
+<div style="display: flex; justify-content: space-between; align-items: center;">
+  <h3 style="margin: 5px; padding: 0;">input_to_dataframe</h3>
+  <a href="https://github.com/MecSimCalc/MecSimCalc-utils/blob/main/mecsimcalc/input_utils.py#LL55C1-L67C39" style="font-size: larger; margin-bottom: 2em; margin: 5px; padding: 0;"><strong>[Source]</strong></a>
 </div>
 
 ```python
 def input_to_dataframe(file):
 ```
 
 #### Description:
@@ -192,17 +171,17 @@
 >>> df = input_to_dataframe(inputFile)
 >>> print(df)
    A  B  C
 0  a  b  c
 1  d  e  f
 ```
 
-<div style={{ display: 'flex', justifyContent: 'space-between', alignItems: 'center' }}>
-  <h3 style={{ margin: 5, padding: 0 }}>print_dataframe</h3>
-  <a href="https://github.com/MecSimCalc/MecSimCalc-utils/blob/main/mecsimcalc/output_utils.py#LL10C1-L67C39" style={{ fontSize: 'larger', marginBottom: '2em', margin: 5, padding: 0 }}><strong>[Source]</strong></a>
+<div style="display: flex; justify-content: space-between; align-items: center;">
+  <h3 style="margin: 5px; padding: 0;">print_dataframe</h3>
+  <a href="https://github.com/MecSimCalc/MecSimCalc-utils/blob/main/mecsimcalc/output_utils.py#LL10C1-L67C39" style="font-size: larger; margin-bottom: 2em; margin: 5px; padding: 0;"><strong>[Source]</strong></a>
 </div>
 
 ```python
 def print_dataframe(
     df,
     download = False,
     DownloadText = "Download Table",
@@ -254,83 +233,87 @@
 {{ outputs.table }}
 
 # outputs.download is the download link
 Downloading Table
 {{ outputs.download }}
 ```
 
-<div style={{ display: 'flex', justifyContent: 'space-between', alignItems: 'center' }}>
-  <h3 style={{ margin: 5, padding: 0 }}>table_to_dataframe</h3>
-  <a href="https://github.com/MecSimCalc/MecSimCalc-utils/blob/main/mecsimcalc/input_utils.py#LL89C1-L105C35" style={{ fontSize: 'larger', marginBottom: '2em', margin: 5, padding: 0 }}><strong>[Source]</strong></a>
+<div style="display: flex; justify-content: space-between; align-items: center;">
+  <h3 style="margin: 5px; padding: 0;">table_to_dataframe</h3>
+  <a href="https://github.com/MecSimCalc/MecSimCalc-utils/blob/main/mecsimcalc/input_utils.py#LL89C1-L105C35 style="font-size: larger; margin-bottom: 2em; margin: 5px; padding: 0;"><strong>[Source]</strong></a>
 </div>
 
 ```python
 def table_to_dataframe(columns: List[List[str]], column_headers: List[str]) -> pd.DataFrame:
 ```
 
 #### Description:
+
 Creates a DataFrame from given columns and headers
 
 #### Arguments:
 
 | Argument             | Type                | Description                                                                        |
 | -------------------- | ------------------- | ---------------------------------------------------------------------------------- |
 | **`columns`**        | **List[List[str]]** | List of columns to be converted into a DataFrame. Each column is a list of strings |
 | **`column_headers`** | **List[str]**       | List of column headers                                                             |
 
 #### Returns:
+
 | Return Type        | Description                                |
 | ------------------ | ------------------------------------------ |
 | **`pd.DataFrame`** | DataFrame created from columns and headers |
 
 #### Example:
 
 ```python
 >>> columns = [["a", "b", "c"], ["d", "e", "f"]]
 >>> column_headers = ["A", "B", "C"]
 >>> df = table_to_dataframe(columns, column_headers)
 >>> print(df)
    A  B  C
 0  a  b  c
 1  d  e  f
+
 ```
 
-<div style={{ display: 'flex', justifyContent: 'space-between', alignItems: 'center' }}>
-  <h3 style={{ margin: 5, padding: 0 }}>print_table</h3>
-  <a href="https://github.com/MecSimCalc/MecSimCalc-utils/blob/main/mecsimcalc/output_utils.py#LL216C1-L240C114" style={{ fontSize: 'larger', marginBottom: '2em', margin: 5, padding: 0 }}><strong>[Source]</strong></a>
+<div style="display: flex; justify-content: space-between; align-items: center;">
+  <h3 style="margin: 5px; padding: 0;">print_table</h3>
+  <a href="https://github.com/MecSimCalc/MecSimCalc-utils/blob/main/mecsimcalc/output_utils.py#LL216C1-L240C114" style="font-size: larger; margin-bottom: 2em; margin: 5px; padding: 0;"><strong>[Source]</strong></a>
 </div>
 
 ```python
-print_table(columns: List[List[str]], column_headers: List[str]):
+print_table(rows: List[List[str]], column_headers: List[str]):
 ```
 
 #### Description:
-Creates an HTML table from given columns and headers
+
+Creates an HTML table from given rows and column headers
 
 #### Arguments:
 
-| Argument             | Type                | Description                                                                    |
-| -------------------- | ------------------- | ------------------------------------------------------------------------------ |
-| **`columns`**        | **List[List[str]]** | List of columns to be converted into a table. Each column is a list of strings |
-| **`column_headers`** | **List[str]**       | List of column headers                                                         |
+| Argument             | Type                | Description                                                                 |
+| -------------------- | ------------------- | --------------------------------------------------------------------------- |
+| **`rows`**           | **List[List[str]]** | List of rows to be converted into a table. Each column is a list of strings |
+| **`column_headers`** | **List[str]**       | List of column headers                                                      |
 
 #### Returns:
 
-| Return Type | Description                                 |
-| ----------- | ------------------------------------------- |
-| **`str`**   | HTML table created from columns and headers |
+| Return Type | Description                              |
+| ----------- | ---------------------------------------- |
+| **`str`**   | HTML table created from rows and headers |
 
 #### Example:
 
 #### Python Code:
 
 ```python
->>> columns = [["a", "b", "c"], ["d", "e", "f"]]
+>>> rows = [["a", "b", "c"], ["d", "e", "f"]]
 >>> column_headers = ["A", "B", "C"]
->>> table = print_table(columns, column_headers)
+>>> table = print_table(rows, column_headers)
 >>> return {
         "table":table,
     }
 ```
 
 #### Output using Jinja2 Template:
 
@@ -338,17 +321,17 @@
 # outputs.table is the HTML table
 Displaying Table
 {{ outputs.table }}
 ```
 
 ## Images
 
-<div style={{ display: 'flex', justifyContent: 'space-between', alignItems: 'center' }}>
-  <h3 style={{ margin: 5, padding: 0 }}>input_to_PIL</h3>
-  <a href="https://github.com/MecSimCalc/MecSimCalc-utils/blob/main/mecsimcalc/input_utils.py#LL70C1-L87C1" style={{ fontSize: 'larger', marginBottom: '2em', margin: 5, padding: 0 }}><strong>[Source]</strong></a>
+<div style="display: flex; justify-content: space-between; align-items: center;">
+  <h3 style="margin: 5px; padding: 0;">input_to_PIL</h3>
+  <a href="https://github.com/MecSimCalc/MecSimCalc-utils/blob/main/mecsimcalc/input_utils.py#LL70C1-L87C1" style="font-size: larger; margin-bottom: 2em; margin: 5px; padding: 0;"><strong>[Source]</strong></a>
 </div>
 
 ```python
 def input_to_PIL(file):
 ```
 
 #### Description:
@@ -374,18 +357,17 @@
 >>> img, metadata = input_to_PIL(inputFile)
 >>> print(metadata)
 data:image/jpeg;base64,
 >>> type(file)
 <class 'PIL.JpegImagePlugin.JpegImageFile'>
 ```
 
-
-<div style={{ display: 'flex', justifyContent: 'space-between', alignItems: 'center' }}>
-  <h3 style={{ margin: 5, padding: 0 }}>print_img</h3>
-  <a href="https://github.com/MecSimCalc/MecSimCalc-utils/blob/main/mecsimcalc/output_utils.py#LL70C1-L129C1" style={{ fontSize: 'larger', marginBottom: '2em', margin: 5, padding: 0 }}><strong>[Source]</strong></a>
+<div style="display: flex; justify-content: space-between; align-items: center;">
+  <h3 style="margin: 5px; padding: 0;">print_img</h3>
+  <a href="https://github.com/MecSimCalc/MecSimCalc-utils/blob/main/mecsimcalc/output_utils.py#LL70C1-L129C1 style="font-size: larger; margin-bottom: 2em; margin: 5px; padding: 0;"><strong>[Source]</strong></a>
 </div>
 
 ```python
 def print_img(
     img,
     metadata,
     WIDTH = 200,
@@ -443,44 +425,47 @@
 {{ outputs.image }}
 
 # outputs.download is the download link
 Downloading Image
 {{ outputs.download }}
 ```
 
-<div style={{ display: 'flex', justifyContent: 'space-between', alignItems: 'center' }}>
-  <h3 style={{ margin: 5, padding: 0 }}>print_plt</h3>
-  <a href="https://github.com/MecSimCalc/MecSimCalc-utils/blob/main/mecsimcalc/output_utils.py#LL131C1-L180C1" style={{ fontSize: 'larger', marginBottom: '2em', margin: 5, padding: 0 }}><strong>[Source]</strong></a>
+<div style="display: flex; justify-content: space-between; align-items: center;">
+  <h3 style="margin: 5px; padding: 0;">print_plt</h3>
+  <a href="https://github.com/MecSimCalc/MecSimCalc-utils/blob/main/mecsimcalc/output_utils.py#LL131C1-L180C1" style="font-size: larger; margin-bottom: 2em; margin: 5px; padding: 0;"><strong>[Source]</strong></a>
 </div>
 
 ```python
 def print_plt(
     plt:,
     width = 500,
     dpi= 100,
     download= False,
     DownloadText = "Download Plot",
     DownloadFileName = "myplot",
 )
 ```
 
 #### Description:
+
 Converts a matplotlib.pyplot or matplotlib.figure into an HTML image tag and optionally provides a download link for the image
 
 #### Arguments:
+
 | Argument               | Type                | Description                                                                 |
 | ---------------------- | ------------------- | --------------------------------------------------------------------------- |
 | **`plt`**              | **plt or figure**   | Matplotlib figure                                                           |
 | **`width`**            | **int** (optional)  | Output width of the image in pixels (Defaults to 500)                       |
 | **`dpi`**              | **int** (optional)  | Output dpi of the image in pixels (Defaults to 100)                         |
 | **`download`**         | **bool** (optional) | If True, function returns a download link (Defaults to False)               |
 | **`DownloadText`**     | **str** (optional)  | The text to be displayed on the download link (Defaults to "Download Plot") |
 | **`DownloadFileName`** | **str** (optional)  | The name of the image file when downloaded (Defaults to "myplot")           |
 
 #### Returns:
+
 | Return Type           | Description                 | Condition         |
 | --------------------- | --------------------------- | ----------------- |
 | **`str`**             | HTML image                  | download is False |
 | **`Tuple[str, str]`** | (HTML image, download link) | download is True  |
 
 #### Example:
```

### Comparing `mecsimcalc-0.0.4/mecsimcalc/input_utils.py` & `mecsimcalc-0.0.5/mecsimcalc/input_utils.py`

 * *Files identical despite different names*

### Comparing `mecsimcalc-0.0.4/mecsimcalc/output_utils.py` & `mecsimcalc-0.0.5/mecsimcalc/output_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -209,32 +209,32 @@
 
     # Return the download link
     return (
         f"<a href='{encoded_data}' download='{filename}{extension}'>{download_text}</a>"
     )
 
 
-def print_table(columns: List[List[str]], column_headers: List[str]) -> str:
+def print_table(rows: List[List[str]], column_headers: List[str]) -> str:
     """
-    Creates an HTML table from given columns and column headers.
+    Creates an HTML table from given rows and column headers.
 
     Args:
-        columns (List[List[str]]): A list of columns (each column is a list of strings) (columns are the vertical data)
+        rows (List[List[str]]): A list of rows (each row is a list of strings)
         column_headers (List[str]): The header for each column
+
     Returns:
         str: HTML table
     """
 
     # Create the header row
     header_row = (
         "<tr>" + "".join(f"<th>{header}</th>" for header in column_headers) + "</tr>"
     )
 
     # Create the data rows
-    rows = len(columns[0])
     data_rows = "".join(
-        "<tr>" + "".join(f"<td>{str(column[i])}</td>" for column in columns) + "</tr>"
-        for i in range(rows)
+        "<tr>" + "".join(f"<td>{str(item)}</td>" for item in row) + "</tr>"
+        for row in rows
     )
 
     # Return the table
     return f"<table border='3' cellpadding='5' style='border-collapse:collapse;'>{header_row}{data_rows}</table>"
```

#### html2text {}

```diff
@@ -71,22 +71,21 @@
 (Defaults to "myfile") extension (str, optional): Extension of the download
 file. (Defaults to ".txt") download_text (str, optional): Text to be displayed
 as the download link (Defaults to "Download File") Returns: str: HTML text
 download link """ # Add a dot to the extension if it doesn't have one if
 extension[0] != "." and extension != "": extension = f".{extension}" # Encode
 the text newdata = base64.b64encode(text.encode()).decode() meta = "data:text/
 plain;base64," encoded_data = meta + newdata # Return the download link return
-( f"{download_text}" ) def print_table(columns: List[List[str]],
-column_headers: List[str]) -> str: """ Creates an HTML table from given columns
-and column headers. Args: columns (List[List[str]]): A list of columns (each
-column is a list of strings) (columns are the vertical data) column_headers
-(List[str]): The header for each column Returns: str: HTML table """ # Create
-the header row header_row = ( "
+( f"{download_text}" ) def print_table(rows: List[List[str]], column_headers:
+List[str]) -> str: """ Creates an HTML table from given rows and column
+headers. Args: rows (List[List[str]]): A list of rows (each row is a list of
+strings) column_headers (List[str]): The header for each column Returns: str:
+HTML table """ # Create the header row header_row = ( "
 " + "".join(f"
 {header}
 " for header in column_headers) + "
-" ) # Create the data rows rows = len(columns[0]) data_rows = "".join( "
+" ) # Create the data rows data_rows = "".join( "
 " + "".join(f"
-{str(column[i])}
-" for column in columns) + "
-" for i in range(rows) ) # Return the table return f"
+{str(item)}
+" for item in row) + "
+" for row in rows ) # Return the table return f"
 "
```

### Comparing `mecsimcalc-0.0.4/setup.py` & `mecsimcalc-0.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = "0.0.4"
+VERSION = "0.0.5"
 DESCRIPTION = "Useful functions for MecSimCalc.com"
 LONG_DESCRIPTION = "Useful functions for MecSimCalc.com"
 
 # Setting up
 setup(
     name="mecsimcalc",
     version=VERSION,
```

