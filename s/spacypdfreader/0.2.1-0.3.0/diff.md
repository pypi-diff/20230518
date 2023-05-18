# Comparing `tmp/spacypdfreader-0.2.1.tar.gz` & `tmp/spacypdfreader-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spacypdfreader-0.2.1.tar", max compression
+gzip compressed data, was "spacypdfreader-0.3.0.tar", max compression
```

## Comparing `spacypdfreader-0.2.1.tar` & `spacypdfreader-0.3.0.tar`

### file list

```diff
@@ -1,13 +1,11 @@
--rw-r--r--   0        0        0     1069 2022-01-09 17:36:51.955551 spacypdfreader-0.2.1/LICENSE
--rw-r--r--   0        0        0     3959 2022-01-09 17:59:10.453401 spacypdfreader-0.2.1/README.md
--rw-r--r--   0        0        0     1061 2022-01-09 17:36:51.964008 spacypdfreader-0.2.1/pyproject.toml
--rw-r--r--   0        0        0       76 2022-01-09 17:36:51.964577 spacypdfreader-0.2.1/spacypdfreader/__init__.py
--rw-r--r--   0        0        0     1520 2022-01-09 17:36:51.964856 spacypdfreader-0.2.1/spacypdfreader/_utils.py
--rw-r--r--   0        0        0       54 2022-01-09 17:36:51.965045 spacypdfreader-0.2.1/spacypdfreader/console.py
--rw-r--r--   0        0        0        0 2022-01-09 17:36:51.965210 spacypdfreader-0.2.1/spacypdfreader/parsers/__init__.py
--rw-r--r--   0        0        0     1140 2022-01-09 17:36:51.965944 spacypdfreader-0.2.1/spacypdfreader/parsers/base.py
--rw-r--r--   0        0        0     2688 2022-01-09 17:36:51.966652 spacypdfreader-0.2.1/spacypdfreader/parsers/pdfminer.py
--rw-r--r--   0        0        0     2918 2022-01-09 17:56:18.293438 spacypdfreader-0.2.1/spacypdfreader/parsers/pytesseract.py
--rw-r--r--   0        0        0     4284 2022-01-09 17:56:18.342340 spacypdfreader-0.2.1/spacypdfreader/spacypdfreader.py
--rw-r--r--   0        0        0     5039 2022-01-09 18:03:26.493528 spacypdfreader-0.2.1/setup.py
--rw-r--r--   0        0        0     5038 2022-01-09 18:03:26.494009 spacypdfreader-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-03-07 15:38:12.234113 spacypdfreader-0.3.0/LICENSE
+-rw-r--r--   0        0        0     4126 2023-05-17 23:37:16.062077 spacypdfreader-0.3.0/README.md
+-rw-r--r--   0        0        0     1123 2023-03-07 17:00:18.559587 spacypdfreader-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0       86 2023-05-17 23:37:16.065209 spacypdfreader-0.3.0/spacypdfreader/__init__.py
+-rw-r--r--   0        0        0     1520 2023-03-07 15:38:12.236546 spacypdfreader-0.3.0/spacypdfreader/_utils.py
+-rw-r--r--   0        0        0       54 2023-03-07 15:38:12.236630 spacypdfreader-0.3.0/spacypdfreader/console.py
+-rw-r--r--   0        0        0        0 2023-03-07 15:38:12.236715 spacypdfreader-0.3.0/spacypdfreader/parsers/__init__.py
+-rw-r--r--   0        0        0     2559 2023-05-17 23:37:16.084163 spacypdfreader-0.3.0/spacypdfreader/parsers/pdfminer.py
+-rw-r--r--   0        0        0     2849 2023-05-17 23:37:16.074695 spacypdfreader-0.3.0/spacypdfreader/parsers/pytesseract.py
+-rw-r--r--   0        0        0     6570 2023-05-18 00:01:32.708496 spacypdfreader-0.3.0/spacypdfreader/spacypdfreader.py
+-rw-r--r--   0        0        0     5246 1970-01-01 00:00:00.000000 spacypdfreader-0.3.0/PKG-INFO
```

### Comparing `spacypdfreader-0.2.1/LICENSE` & `spacypdfreader-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `spacypdfreader-0.2.1/README.md` & `spacypdfreader-0.3.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,19 @@
 # spacypdfreader
 
 Easy PDF to text to *spaCy* text extraction in Python.
 
 <p>
+    <!-- PyPI version -->
     <a href="https://pypi.org/project/spacypdfreader" target="_blank">
         <img src="https://img.shields.io/pypi/v/spacypdfreader?color=%2334D058&label=pypi%20package" alt="Package version">
     </a>
+    <!-- PyPi Downloads -->
+    <img alt="PyPI - Downloads" src="https://img.shields.io/pypi/dm/spacypdfreader?label=PyPi%20downloads">
+    <!-- Pytest -->
     <a href="https://github.com/SamEdwardes/spacypdfreader/actions/workflows/pytest.yml" target="_blank">
         <img src="https://github.com/SamEdwardes/spacypdfreader/actions/workflows/pytest.yml/badge.svg" alt="pytest">
     </a>
 </p>
 
 <hr></hr>
 
@@ -51,31 +55,32 @@
 pip install 'spacypdfreader[pytesseract]'
 ```
 
 ## Usage
 
 ```python
 import spacy
+
 from spacypdfreader import pdf_reader
 
 nlp = spacy.load("en_core_web_sm")
 doc = pdf_reader("tests/data/test_pdf_01.pdf", nlp)
 
 # Get the page number of any token.
 print(doc[0]._.page_number)  # 1
-print(doc[-1]._.page_number) # 4
+print(doc[-1]._.page_number)  # 4
 
 # Get page meta data about the PDF document.
-print(doc._.pdf_file_name)   # "tests/data/test_pdf_01.pdf"
-print(doc._.page_range)      # (1, 4)
-print(doc._.first_page)      # 1
-print(doc._.last_page)       # 4
+print(doc._.pdf_file_name)  # "tests/data/test_pdf_01.pdf"
+print(doc._.page_range)  # (1, 4)
+print(doc._.first_page)  # 1
+print(doc._.last_page)  # 4
 
 # Get all of the text from a specific PDF page.
-print(doc._.page(4))         # "able to display the destination page (unless..."
+print(doc._.page(4))  # "able to display the destination page (unless..."
 ```
 
 ## What is *spaCy*?
 
 *spaCy* is a natural language processing (NLP) tool. It can be used to perform a variety of NLP tasks. For more information check out the excellent documentation at [https://spacy.io](https://spacy.io).
 
 ## Implementation Notes
@@ -87,22 +92,24 @@
 Example of a "traditional" spaCy pipeline component [negspaCy](https://spacy.io/universe/project/negspacy):
 
 ```python
 import spacy
 from negspacy.negation import Negex
 
 nlp = spacy.load("en_core_web_sm")
-nlp.add_pipe("negex", config={"ent_types":["PERSON","ORG"]})
+nlp.add_pipe("negex", config={"ent_types": ["PERSON", "ORG"]})
 doc = nlp("She does not like Steve Jobs but likes Apple products.")
 ```
 
 Example of `spaCyPDFreader` usage:
 
 ```python
 import spacy
+
 from spacypdfreader import pdf_reader
+
 nlp = spacy.load("en_core_web_sm")
 
 doc = pdf_reader("tests/data/test_pdf_01.pdf", nlp)
 ```
 
 Note that the `nlp.add_pipe` is not used by spaCyPDFreader.
```

#### html2text {}

```diff
@@ -1,9 +1,9 @@
 # spacypdfreader Easy PDF to text to *spaCy* text extraction in Python.
-[Package_version] [pytest]
+ [Package_version]  [PyPI - Downloads]  [pytest]
 ===============================================================================
 **Documentation:** [https://samedwardes.github.io/spacypdfreader/](https://
 samedwardes.github.io/spacypdfreader/) **Source code:** [https://github.com/
 SamEdwardes/spacypdfreader](https://github.com/SamEdwardes/spacypdfreader)
 **PyPi:** [https://pypi.org/project/spacypdfreader/](https://pypi.org/project/
 spacypdfreader/) **spaCy universe:** [https://spacy.io/universe/project/
 spacypdfreader](https://spacy.io/universe/project/spacypdfreader)
@@ -37,13 +37,13 @@
 Instead `pdf_reader` takes a path to a PDF file and a `spacy.Language` object
 as parameters and returns a `spacy.tokens.Doc` object. This allows users an
 easy way to extract text from PDF files while still allowing them use and
 customize all of the features spacy has to offer by allowing you to pass in the
 `spacy.Language` object. Example of a "traditional" spaCy pipeline component
 [negspaCy](https://spacy.io/universe/project/negspacy): ```python import spacy
 from negspacy.negation import Negex nlp = spacy.load("en_core_web_sm")
-nlp.add_pipe("negex", config={"ent_types":["PERSON","ORG"]}) doc = nlp("She
+nlp.add_pipe("negex", config={"ent_types": ["PERSON", "ORG"]}) doc = nlp("She
 does not like Steve Jobs but likes Apple products.") ``` Example of
 `spaCyPDFreader` usage: ```python import spacy from spacypdfreader import
 pdf_reader nlp = spacy.load("en_core_web_sm") doc = pdf_reader("tests/data/
 test_pdf_01.pdf", nlp) ``` Note that the `nlp.add_pipe` is not used by
 spaCyPDFreader.
```

### Comparing `spacypdfreader-0.2.1/pyproject.toml` & `spacypdfreader-0.3.0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,33 +1,34 @@
 [tool.poetry]
 name = "spacypdfreader"
-version = "0.2.1"
+version = "0.3.0"
 description = "A PDF to text extraction pipeline component for spaCy."
 authors = ["SamEdwardes <edwardes.s@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/SamEdwardes/spaCyPDFreader"
 keywords = ["python", "spacy", "nlp", "pdf", "pdfs"]
 
 [tool.poetry.dependencies]
-python = "^3.7"
-spacy = "^3.0.0"
+python = ">=3.8,<3.12"
+spacy = "^3.4"
 rich = "^10.15.2"
 "pdfminer.six" = "^20211012"
 pytesseract = {version = "^0.3.8", optional = true}
-Pillow = {version = "^8.4.0", optional = true}
 pdf2image = {version = "^1.16.0", optional = true}
-
-[tool.poetry.dev-dependencies]
-pytest = "^6.2.5"
-en-core-web-sm = {url = "https://github.com/explosion/spacy-models/releases/download/en_core_web_sm-3.0.0/en_core_web_sm-3.0.0-py3-none-any.whl"}
-black = "^21.12b0"
-mkdocs-material = "^8.1.3"
-mkdocstrings = "^0.16.2"
-mkdocs-include-markdown-plugin = "^3.2.3"
+numpy = "^1.24.2"
+Pillow = {version = "^9.4.0", optional = true}
 
 [tool.poetry.extras]
 pytesseract = ["pytesseract", "Pillow", "pdf2image"]
 
+[tool.poetry.group.dev.dependencies]
+pytest = "^6.2.5"
+en-core-web-sm = {url = "https://github.com/explosion/spacy-models/releases/download/en_core_web_sm-3.4.1/en_core_web_sm-3.4.1-py3-none-any.whl"}
+mkdocs-material = "^9.1.1"
+mkdocs-include-markdown-plugin = "^4.0.3"
+mkdocstrings = {extras = ["python"], version = "^0.20.0"}
+shed = "^2023.3.1"
+
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `spacypdfreader-0.2.1/spacypdfreader/_utils.py` & `spacypdfreader-0.3.0/spacypdfreader/_utils.py`

 * *Files identical despite different names*

### Comparing `spacypdfreader-0.2.1/spacypdfreader/parsers/pdfminer.py` & `spacypdfreader-0.3.0/spacypdfreader/parsers/pdfminer.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,72 +1,68 @@
 from pdfminer.high_level import extract_text
 
-from .base import BaseParser
-from typing import Any
 
-
-class PdfminerParser(BaseParser):
+def parser(pdf_path: str, page_number: int, **kwargs):
     """Convert PDFs to text using pdfminer.
 
     The pdfminer library is "pure python" library for converting PDF into text.
     pdfminer is relatively fast, but has low accuracy than other parsers such as
     [pytesseract](/parsers/#pytesseract).
 
-    Refer to [spacypdfreader.parsers.base.BaseParser][] for a list of attributes
-    and the `__init__` method.
+    Parameters:
+        pdf_path: Path to a PDF file.
+        page_number: The page number of the PDF to convert from PDF to text. Must be one
+            digit based indexing (e.g. the first page of the PDF is page 1, as
+            opposed to page 0).
+        **kwargs: `**kwargs` will be passed to
+            [`pdfminer.high_level.extract_text`](https://pdfminersix.readthedocs.io/en/latest/reference/highlevel.html#extract-text).
+
+    Returns:
+        str: The PDF page as a string.
 
     Examples:
-        `PdfminerParser` is the default PDF to text parser and will be
-        automatically used unless otherwise specificied.
+        pdfminer is the default PDF to text parser and will be automatically
+        used unless otherwise specified.
 
         >>> import spacy
         >>> from spacypdfreader import pdf_reader
         >>>
         >>> nlp = spacy.load("en_core_web_sm")
         >>> doc = pdf_reader("tests/data/test_pdf_01.pdf", nlp)
 
-        To be more explicit import `PdfminerParser` and pass it into the
+        To be more explicit import the parser and pass it into the
         `pdf_reader` function.
 
         >>> import spacy
         >>> from spacypdfreader import pdf_reader
-        >>> from spacypdfreader.parsers.pdfminer import PdfminerParser
+        >>> from spacypdfreader.parsers.pdfminer import parser
         >>>
         >>> nlp = spacy.load("en_core_web_sm")
-        >>> doc = pdf_reader("tests/data/test_pdf_01.pdf", nlp, PdfminerParser)
+        >>> doc = pdf_reader("tests/data/test_pdf_01.pdf", nlp, parser)
 
         For more fine tuning you can pass in additional parameters to pdfminer.
 
         >>> import spacy
         >>> from spacypdfreader import pdf_reader
-        >>> from spacypdfreader.parsers.pdfminer import PdfminerParser
+        >>> from spacypdfreader.parsers.pdfminer import parser
         >>>
         >>> nlp = spacy.load("en_core_web_sm")
         >>> params = {"caching": False}
-        >>> doc = pdf_reader("tests/data/test_pdf_01.pdf", nlp, PdfminerParser, **params)
+        >>> doc = pdf_reader("tests/data/test_pdf_01.pdf", nlp, parser, **params)
 
     Info:
         See the [pdfminer section](/parsers/#pdfminer) in the docs for more
         details on the implementation of pdfminer. For more details on pdfminer
-        refer to the
-        [pdfminer docs](https://pdfminersix.readthedocs.io/en/latest/).
+        refer to the [pdfminer docs](https://pdfminersix.readthedocs.io/en/latest/).
     """
+    # pdfminer uses zero indexed page numbers. Therefore need to remove 1
+    # from the page count.
+    page_number -= 1
+    text = extract_text(pdf_path, page_numbers=[page_number], **kwargs)
+    return text
+
 
-    name: str = "pdfminer"
+class PdfminerParser:
+    """This class has bee included for backwards compatibility. Do not use."""
 
-    def pdf_to_text(self, **kwargs: Any) -> str:
-        """Convert a PDF page to text using the `extract_text` function from
-        pdfminer.
-
-        Args:
-            **kwargs: Arbitrary keyword arguments. See the pdfminer docs for the
-                [extract_text](https://pdfminersix.readthedocs.io/en/latest/reference/highlevel.html#extract-text)
-                function for the available keywork arguments.
-
-        Returns:
-            A string respresentation of the PDF page.
-        """
-        # pdfminer uses zero indexed page numbers. Therefore need to remove 1
-        # from the page count.
-        self.page_number -= 1
-        text = extract_text(self.pdf_path, page_numbers=[self.page_number], **kwargs)
-        return text
+    def __init__(self):
+        return None
```

### Comparing `spacypdfreader-0.2.1/spacypdfreader/parsers/pytesseract.py` & `spacypdfreader-0.3.0/spacypdfreader/parsers/pytesseract.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,83 +1,78 @@
-import os
 import tempfile
-from typing import Any
+from pathlib import Path
 
 from pdf2image import convert_from_path
 from PIL import Image
-
 from pytesseract import image_to_string
 
-from .base import BaseParser
-
 
-class PytesseractParser(BaseParser):
-    """Convert PDFs to text using pytesseract.
+def parser(pdf_path: str, page_number: int, **kwargs):
+    """Convert a single PDF page to text using pytesseract.
 
     The pytesseract library has the highest accuracy of all the PDF to text
     parsers included in spacypdfreader. It takes a different approach than other
     parsers. It first converts the PDF to an image, then runs an OCR engine on
     the image to extract the text. pytesseract results in the best quality but
     can be very slow compared to other parsers.
 
-    Refer to [spacypdfreader.parsers.base.BaseParser][] for a list of attributes
-    and the `__init__` method.
+    Parameters:
+        pdf_path: Path to a PDF file.
+        page_number: The page number of the PDF to convert from PDF to text. Must be one
+            digit based indexing (e.g. the first page of the PDF is page 1, as
+            opposed to page 0).
+        **kwargs: `**kwargs` will be passed to
+            [`pytesseract.image_to_string`](https://github.com/madmaze/pytesseract/blob/8fe7cd1faf4abc0946cb69813d535198772dbb6c/pytesseract/pytesseract.py#L409-L426).
+
+    Returns:
+        str: The PDF page as a string.
 
     Examples:
-        To use `PytesseractParser` it must be explicitly imported and passed
+        To use pytesseract it must be explicitly imported and passed
         into the `pdf_reader` function.
 
         >>> import spacy
         >>> from spacypdfreader import pdf_reader
-        >>> from spacypdfreader.parsers.pytesseract import PytesseractParser
+        >>> from spacypdfreader.parsers.pytesseract import parser
         >>>
         >>> nlp = spacy.load("en_core_web_sm")
-        >>> doc = pdf_reader("tests/data/test_pdf_01.pdf", nlp, PytesseractParser)
+        >>> doc = pdf_reader("tests/data/test_pdf_01.pdf", nlp, parser)
 
         For more fine tuning you can pass in additional parameters to
         pytesseract.
 
         >>> import spacy
         >>> from spacypdfreader import pdf_reader
-        >>> from spacypdfreader.parsers.pytesseract import PytesseractParser
+        >>> from spacypdfreader.parsers.pytesseract import parser
         >>>
         >>> nlp = spacy.load("en_core_web_sm")
         >>> params = {"nice": 1}
-        >>> doc = pdf_reader("tests/data/test_pdf_01.pdf", nlp, PytesseractParser, **params)
+        >>> doc = pdf_reader("tests/data/test_pdf_01.pdf", nlp, parser, **params)
 
     Info:
         See the [pytesseract section](/parsers/#pytesseract) in the docs for
         more details on the implementation of pytesseract. For more details on
-        pytesseract see the
-        [pytesseract docs](https://github.com/madmaze/pytesseract).
+        pytesseract see the [pytesseract docs](https://github.com/madmaze/pytesseract).
     """
 
-    name: str = "pytesseract"
+    with tempfile.TemporaryDirectory() as tmp_dir:
+        # Convert pdf page to image.
+        file_name = convert_from_path(
+            pdf_path=pdf_path,
+            output_folder=tmp_dir,
+            paths_only=True,
+            first_page=page_number,
+            last_page=page_number + 1,
+        )[0]
+
+        # Convert images to text.
+        file_path = Path(tmp_dir, str(file_name))
+        text = str(image_to_string(Image.open(file_path), **kwargs))
+
+    return text
 
-    def pdf_to_text(self, **kwargs: Any) -> str:
-        """Convert a PDF page to text using the `image_to_string` function from
-        pytesseract.
 
-        Args:
-            **kwargs: Arbitrary keyword arguments. See the pytesseract docs for
-                the [image_to_string](https://github.com/madmaze/pytesseract)
-                function for the available keyword arguments.
-
-        Returns:
-            A string respresentation of the PDF page.
-        """
-        with tempfile.TemporaryDirectory() as tmp_dir:
-
-            # Convert pdf page to image.
-            file_name = convert_from_path(
-                self.pdf_path,
-                output_folder=tmp_dir,
-                paths_only=True,
-                first_page=self.page_number,
-                last_page=self.page_number + 1,
-            )[0]
-
-            # Convert images to text.
-            file_path = os.path.join(tmp_dir, file_name)
-            text = str(image_to_string(Image.open(file_path), **kwargs))
+class PytesseractParser:
+    """This class has bee included for backwards compatibility. Do not use."""
 
-        return text
+    def __init__(self):
+        return None
```

### Comparing `spacypdfreader-0.2.1/setup.py` & `spacypdfreader-0.3.0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,38 +1,142 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: spacypdfreader
+Version: 0.3.0
+Summary: A PDF to text extraction pipeline component for spaCy.
+Home-page: https://github.com/SamEdwardes/spaCyPDFreader
+License: MIT
+Keywords: python,spacy,nlp,pdf,pdfs
+Author: SamEdwardes
+Author-email: edwardes.s@gmail.com
+Requires-Python: >=3.8,<3.12
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Provides-Extra: pytesseract
+Requires-Dist: Pillow (>=9.4.0,<10.0.0) ; extra == "pytesseract"
+Requires-Dist: numpy (>=1.24.2,<2.0.0)
+Requires-Dist: pdf2image (>=1.16.0,<2.0.0) ; extra == "pytesseract"
+Requires-Dist: pdfminer.six (>=20211012,<20211013)
+Requires-Dist: pytesseract (>=0.3.8,<0.4.0) ; extra == "pytesseract"
+Requires-Dist: rich (>=10.15.2,<11.0.0)
+Requires-Dist: spacy (>=3.4,<4.0)
+Project-URL: Repository, https://github.com/SamEdwardes/spaCyPDFreader
+Description-Content-Type: text/markdown
 
-packages = \
-['spacypdfreader', 'spacypdfreader.parsers']
+# spacypdfreader
 
-package_data = \
-{'': ['*']}
+Easy PDF to text to *spaCy* text extraction in Python.
 
-install_requires = \
-['pdfminer.six>=20211012,<20211013',
- 'rich>=10.15.2,<11.0.0',
- 'spacy>=3.0.0,<4.0.0']
-
-extras_require = \
-{'pytesseract': ['pytesseract>=0.3.8,<0.4.0',
-                 'Pillow>=8.4.0,<9.0.0',
-                 'pdf2image>=1.16.0,<2.0.0']}
-
-setup_kwargs = {
-    'name': 'spacypdfreader',
-    'version': '0.2.1',
-    'description': 'A PDF to text extraction pipeline component for spaCy.',
-    'long_description': '# spacypdfreader\n\nEasy PDF to text to *spaCy* text extraction in Python.\n\n<p>\n    <a href="https://pypi.org/project/spacypdfreader" target="_blank">\n        <img src="https://img.shields.io/pypi/v/spacypdfreader?color=%2334D058&label=pypi%20package" alt="Package version">\n    </a>\n    <a href="https://github.com/SamEdwardes/spacypdfreader/actions/workflows/pytest.yml" target="_blank">\n        <img src="https://github.com/SamEdwardes/spacypdfreader/actions/workflows/pytest.yml/badge.svg" alt="pytest">\n    </a>\n</p>\n\n<hr></hr>\n\n**Documentation:** [https://samedwardes.github.io/spacypdfreader/](https://samedwardes.github.io/spacypdfreader/)\n\n**Source code:** [https://github.com/SamEdwardes/spacypdfreader](https://github.com/SamEdwardes/spacypdfreader)\n\n**PyPi:** [https://pypi.org/project/spacypdfreader/](https://pypi.org/project/spacypdfreader/)\n\n**spaCy universe:** [https://spacy.io/universe/project/spacypdfreader](https://spacy.io/universe/project/spacypdfreader)\n\n<hr></hr>\n\n*spacypdfreader* is a python library for extracting text from PDF documents into *spaCy* `Doc` objects. When you use *spacypdfreader* the token and doc objects from spacy are annotated with additional information about the pdf.\n\nThe key features are:\n\n- **PDF to spaCy Doc object:** Convert a PDF document directly into a *spaCy* `Doc` object.\n- **Custom spaCy attributes and methods:**\n    - `token._.page_number`\n    - `doc._.page_range`\n    - `doc._.first_page`\n    - `doc._.last_page`\n    - `doc._.pdf_file_name`\n    - `doc._.page(int)`\n- **Multiple parsers:** Select between multiple built in PDF to text parsers or bring your own PDF to text parser.\n\n## Installation\n\nInstall *spacypdfreader* using pip:\n\n```bash\npip install spacypdfreader\n```\n\nTo install with the required pytesseract dependencies:\n\n```bash\npip install \'spacypdfreader[pytesseract]\'\n```\n\n## Usage\n\n```python\nimport spacy\nfrom spacypdfreader import pdf_reader\n\nnlp = spacy.load("en_core_web_sm")\ndoc = pdf_reader("tests/data/test_pdf_01.pdf", nlp)\n\n# Get the page number of any token.\nprint(doc[0]._.page_number)  # 1\nprint(doc[-1]._.page_number) # 4\n\n# Get page meta data about the PDF document.\nprint(doc._.pdf_file_name)   # "tests/data/test_pdf_01.pdf"\nprint(doc._.page_range)      # (1, 4)\nprint(doc._.first_page)      # 1\nprint(doc._.last_page)       # 4\n\n# Get all of the text from a specific PDF page.\nprint(doc._.page(4))         # "able to display the destination page (unless..."\n```\n\n## What is *spaCy*?\n\n*spaCy* is a natural language processing (NLP) tool. It can be used to perform a variety of NLP tasks. For more information check out the excellent documentation at [https://spacy.io](https://spacy.io).\n\n## Implementation Notes\n\nspaCyPDFreader behaves a little bit different than your typical [spaCy custom component](https://spacy.io/usage/processing-pipelines#custom-components). Typically a spaCy component should receive and return a `spacy.tokens.Doc` object.\n\nspaCyPDFreader breaks this convention because the text must first be extracted from the PDF. Instead `pdf_reader` takes a path to a PDF file and a `spacy.Language` object as parameters and returns a `spacy.tokens.Doc` object. This allows users an easy way to extract text from PDF files while still allowing them use and customize all of the features spacy has to offer by allowing you to pass in the `spacy.Language` object.\n\nExample of a "traditional" spaCy pipeline component [negspaCy](https://spacy.io/universe/project/negspacy):\n\n```python\nimport spacy\nfrom negspacy.negation import Negex\n\nnlp = spacy.load("en_core_web_sm")\nnlp.add_pipe("negex", config={"ent_types":["PERSON","ORG"]})\ndoc = nlp("She does not like Steve Jobs but likes Apple products.")\n```\n\nExample of `spaCyPDFreader` usage:\n\n```python\nimport spacy\nfrom spacypdfreader import pdf_reader\nnlp = spacy.load("en_core_web_sm")\n\ndoc = pdf_reader("tests/data/test_pdf_01.pdf", nlp)\n```\n\nNote that the `nlp.add_pipe` is not used by spaCyPDFreader.',
-    'author': 'SamEdwardes',
-    'author_email': 'edwardes.s@gmail.com',
-    'maintainer': None,
-    'maintainer_email': None,
-    'url': 'https://github.com/SamEdwardes/spaCyPDFreader',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'extras_require': extras_require,
-    'python_requires': '>=3.7,<4.0',
-}
+<p>
+    <!-- PyPI version -->
+    <a href="https://pypi.org/project/spacypdfreader" target="_blank">
+        <img src="https://img.shields.io/pypi/v/spacypdfreader?color=%2334D058&label=pypi%20package" alt="Package version">
+    </a>
+    <!-- PyPi Downloads -->
+    <img alt="PyPI - Downloads" src="https://img.shields.io/pypi/dm/spacypdfreader?label=PyPi%20downloads">
+    <!-- Pytest -->
+    <a href="https://github.com/SamEdwardes/spacypdfreader/actions/workflows/pytest.yml" target="_blank">
+        <img src="https://github.com/SamEdwardes/spacypdfreader/actions/workflows/pytest.yml/badge.svg" alt="pytest">
+    </a>
+</p>
 
+<hr></hr>
 
-setup(**setup_kwargs)
+**Documentation:** [https://samedwardes.github.io/spacypdfreader/](https://samedwardes.github.io/spacypdfreader/)
+
+**Source code:** [https://github.com/SamEdwardes/spacypdfreader](https://github.com/SamEdwardes/spacypdfreader)
+
+**PyPi:** [https://pypi.org/project/spacypdfreader/](https://pypi.org/project/spacypdfreader/)
+
+**spaCy universe:** [https://spacy.io/universe/project/spacypdfreader](https://spacy.io/universe/project/spacypdfreader)
+
+<hr></hr>
+
+*spacypdfreader* is a python library for extracting text from PDF documents into *spaCy* `Doc` objects. When you use *spacypdfreader* the token and doc objects from spacy are annotated with additional information about the pdf.
+
+The key features are:
+
+- **PDF to spaCy Doc object:** Convert a PDF document directly into a *spaCy* `Doc` object.
+- **Custom spaCy attributes and methods:**
+    - `token._.page_number`
+    - `doc._.page_range`
+    - `doc._.first_page`
+    - `doc._.last_page`
+    - `doc._.pdf_file_name`
+    - `doc._.page(int)`
+- **Multiple parsers:** Select between multiple built in PDF to text parsers or bring your own PDF to text parser.
+
+## Installation
+
+Install *spacypdfreader* using pip:
+
+```bash
+pip install spacypdfreader
+```
+
+To install with the required pytesseract dependencies:
+
+```bash
+pip install 'spacypdfreader[pytesseract]'
+```
+
+## Usage
+
+```python
+import spacy
+
+from spacypdfreader import pdf_reader
+
+nlp = spacy.load("en_core_web_sm")
+doc = pdf_reader("tests/data/test_pdf_01.pdf", nlp)
+
+# Get the page number of any token.
+print(doc[0]._.page_number)  # 1
+print(doc[-1]._.page_number)  # 4
+
+# Get page meta data about the PDF document.
+print(doc._.pdf_file_name)  # "tests/data/test_pdf_01.pdf"
+print(doc._.page_range)  # (1, 4)
+print(doc._.first_page)  # 1
+print(doc._.last_page)  # 4
+
+# Get all of the text from a specific PDF page.
+print(doc._.page(4))  # "able to display the destination page (unless..."
+```
+
+## What is *spaCy*?
+
+*spaCy* is a natural language processing (NLP) tool. It can be used to perform a variety of NLP tasks. For more information check out the excellent documentation at [https://spacy.io](https://spacy.io).
+
+## Implementation Notes
+
+spaCyPDFreader behaves a little bit different than your typical [spaCy custom component](https://spacy.io/usage/processing-pipelines#custom-components). Typically a spaCy component should receive and return a `spacy.tokens.Doc` object.
+
+spaCyPDFreader breaks this convention because the text must first be extracted from the PDF. Instead `pdf_reader` takes a path to a PDF file and a `spacy.Language` object as parameters and returns a `spacy.tokens.Doc` object. This allows users an easy way to extract text from PDF files while still allowing them use and customize all of the features spacy has to offer by allowing you to pass in the `spacy.Language` object.
+
+Example of a "traditional" spaCy pipeline component [negspaCy](https://spacy.io/universe/project/negspacy):
+
+```python
+import spacy
+from negspacy.negation import Negex
+
+nlp = spacy.load("en_core_web_sm")
+nlp.add_pipe("negex", config={"ent_types": ["PERSON", "ORG"]})
+doc = nlp("She does not like Steve Jobs but likes Apple products.")
+```
+
+Example of `spaCyPDFreader` usage:
+
+```python
+import spacy
+
+from spacypdfreader import pdf_reader
+
+nlp = spacy.load("en_core_web_sm")
+
+doc = pdf_reader("tests/data/test_pdf_01.pdf", nlp)
+```
+
+Note that the `nlp.add_pipe` is not used by spaCyPDFreader.
```

#### html2text {}

```diff
@@ -1,66 +1,65 @@
-# -*- coding: utf-8 -*- from setuptools import setup packages = \
-['spacypdfreader', 'spacypdfreader.parsers'] package_data = \ {'': ['*']}
-install_requires = \ ['pdfminer.six>=20211012,<20211013',
-'rich>=10.15.2,<11.0.0', 'spacy>=3.0.0,<4.0.0'] extras_require = \
-{'pytesseract': ['pytesseract>=0.3.8,<0.4.0', 'Pillow>=8.4.0,<9.0.0',
-'pdf2image>=1.16.0,<2.0.0']} setup_kwargs = { 'name': 'spacypdfreader',
-'version': '0.2.1', 'description': 'A PDF to text extraction pipeline component
-for spaCy.', 'long_description': '# spacypdfreader\n\nEasy PDF to text to
-*spaCy* text extraction in Python.\n\n
-\n \n_[Package_version]\n\n \n_[pytest]\n\n
-\n\n
+Metadata-Version: 2.1 Name: spacypdfreader Version: 0.3.0 Summary: A PDF to
+text extraction pipeline component for spaCy. Home-page: https://github.com/
+SamEdwardes/spaCyPDFreader License: MIT Keywords: python,spacy,nlp,pdf,pdfs
+Author: SamEdwardes Author-email: edwardes.s@gmail.com Requires-Python:
+>=3.8,<3.12 Classifier: License :: OSI Approved :: MIT License Classifier:
+Programming Language :: Python :: 3 Classifier: Programming Language :: Python
+:: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
+Programming Language :: Python :: 3.10 Classifier: Programming Language ::
+Python :: 3.11 Provides-Extra: pytesseract Requires-Dist: Pillow
+(>=9.4.0,<10.0.0) ; extra == "pytesseract" Requires-Dist: numpy
+(>=1.24.2,<2.0.0) Requires-Dist: pdf2image (>=1.16.0,<2.0.0) ; extra ==
+"pytesseract" Requires-Dist: pdfminer.six (>=20211012,<20211013) Requires-Dist:
+pytesseract (>=0.3.8,<0.4.0) ; extra == "pytesseract" Requires-Dist: rich
+(>=10.15.2,<11.0.0) Requires-Dist: spacy (>=3.4,<4.0) Project-URL: Repository,
+https://github.com/SamEdwardes/spaCyPDFreader Description-Content-Type: text/
+markdown # spacypdfreader Easy PDF to text to *spaCy* text extraction in
+Python.
+ [Package_version]  [PyPI - Downloads]  [pytest]
 ===============================================================================
-\n\n**Documentation:** [https://samedwardes.github.io/spacypdfreader/](https://
-samedwardes.github.io/spacypdfreader/)\n\n**Source code:** [https://github.com/
-SamEdwardes/spacypdfreader](https://github.com/SamEdwardes/
-spacypdfreader)\n\n**PyPi:** [https://pypi.org/project/spacypdfreader/](https:/
-/pypi.org/project/spacypdfreader/)\n\n**spaCy universe:** [https://spacy.io/
-universe/project/spacypdfreader](https://spacy.io/universe/project/
-spacypdfreader)\n\n
+**Documentation:** [https://samedwardes.github.io/spacypdfreader/](https://
+samedwardes.github.io/spacypdfreader/) **Source code:** [https://github.com/
+SamEdwardes/spacypdfreader](https://github.com/SamEdwardes/spacypdfreader)
+**PyPi:** [https://pypi.org/project/spacypdfreader/](https://pypi.org/project/
+spacypdfreader/) **spaCy universe:** [https://spacy.io/universe/project/
+spacypdfreader](https://spacy.io/universe/project/spacypdfreader)
 ===============================================================================
-\n\n*spacypdfreader* is a python library for extracting text from PDF documents
+*spacypdfreader* is a python library for extracting text from PDF documents
 into *spaCy* `Doc` objects. When you use *spacypdfreader* the token and doc
-objects from spacy are annotated with additional information about the
-pdf.\n\nThe key features are:\n\n- **PDF to spaCy Doc object:** Convert a PDF
-document directly into a *spaCy* `Doc` object.\n- **Custom spaCy attributes and
-methods:**\n - `token._.page_number`\n - `doc._.page_range`\n -
-`doc._.first_page`\n - `doc._.last_page`\n - `doc._.pdf_file_name`\n -
-`doc._.page(int)`\n- **Multiple parsers:** Select between multiple built in PDF
-to text parsers or bring your own PDF to text parser.\n\n##
-Installation\n\nInstall *spacypdfreader* using pip:\n\n```bash\npip install
-spacypdfreader\n```\n\nTo install with the required pytesseract dependencies:
-\n\n```bash\npip install \'spacypdfreader[pytesseract]\'\n```\n\n##
-Usage\n\n```python\nimport spacy\nfrom spacypdfreader import pdf_reader\n\nnlp
-= spacy.load("en_core_web_sm")\ndoc = pdf_reader("tests/data/test_pdf_01.pdf",
-nlp)\n\n# Get the page number of any token.\nprint(doc[0]._.page_number) #
-1\nprint(doc[-1]._.page_number) # 4\n\n# Get page meta data about the PDF
-document.\nprint(doc._.pdf_file_name) # "tests/data/test_pdf_01.pdf"\nprint
-(doc._.page_range) # (1, 4)\nprint(doc._.first_page) # 1\nprint
-(doc._.last_page) # 4\n\n# Get all of the text from a specific PDF page.\nprint
-(doc._.page(4)) # "able to display the destination page (unless..."\n```\n\n##
-What is *spaCy*?\n\n*spaCy* is a natural language processing (NLP) tool. It can
-be used to perform a variety of NLP tasks. For more information check out the
-excellent documentation at [https://spacy.io](https://spacy.io).\n\n##
-Implementation Notes\n\nspaCyPDFreader behaves a little bit different than your
-typical [spaCy custom component](https://spacy.io/usage/processing-
-pipelines#custom-components). Typically a spaCy component should receive and
-return a `spacy.tokens.Doc` object.\n\nspaCyPDFreader breaks this convention
-because the text must first be extracted from the PDF. Instead `pdf_reader`
-takes a path to a PDF file and a `spacy.Language` object as parameters and
-returns a `spacy.tokens.Doc` object. This allows users an easy way to extract
-text from PDF files while still allowing them use and customize all of the
-features spacy has to offer by allowing you to pass in the `spacy.Language`
-object.\n\nExample of a "traditional" spaCy pipeline component [negspaCy]
-(https://spacy.io/universe/project/negspacy):\n\n```python\nimport spacy\nfrom
-negspacy.negation import Negex\n\nnlp = spacy.load
-("en_core_web_sm")\nnlp.add_pipe("negex", config={"ent_types":
-["PERSON","ORG"]})\ndoc = nlp("She does not like Steve Jobs but likes Apple
-products.")\n```\n\nExample of `spaCyPDFreader` usage:\n\n```python\nimport
-spacy\nfrom spacypdfreader import pdf_reader\nnlp = spacy.load
-("en_core_web_sm")\n\ndoc = pdf_reader("tests/data/test_pdf_01.pdf",
-nlp)\n```\n\nNote that the `nlp.add_pipe` is not used by spaCyPDFreader.',
-'author': 'SamEdwardes', 'author_email': 'edwardes.s@gmail.com', 'maintainer':
-None, 'maintainer_email': None, 'url': 'https://github.com/SamEdwardes/
-spaCyPDFreader', 'packages': packages, 'package_data': package_data,
-'install_requires': install_requires, 'extras_require': extras_require,
-'python_requires': '>=3.7,<4.0', } setup(**setup_kwargs)
+objects from spacy are annotated with additional information about the pdf. The
+key features are: - **PDF to spaCy Doc object:** Convert a PDF document
+directly into a *spaCy* `Doc` object. - **Custom spaCy attributes and methods:
+** - `token._.page_number` - `doc._.page_range` - `doc._.first_page` -
+`doc._.last_page` - `doc._.pdf_file_name` - `doc._.page(int)` - **Multiple
+parsers:** Select between multiple built in PDF to text parsers or bring your
+own PDF to text parser. ## Installation Install *spacypdfreader* using pip:
+```bash pip install spacypdfreader ``` To install with the required pytesseract
+dependencies: ```bash pip install 'spacypdfreader[pytesseract]' ``` ## Usage
+```python import spacy from spacypdfreader import pdf_reader nlp = spacy.load
+("en_core_web_sm") doc = pdf_reader("tests/data/test_pdf_01.pdf", nlp) # Get
+the page number of any token. print(doc[0]._.page_number) # 1 print(doc[-
+1]._.page_number) # 4 # Get page meta data about the PDF document. print
+(doc._.pdf_file_name) # "tests/data/test_pdf_01.pdf" print(doc._.page_range) #
+(1, 4) print(doc._.first_page) # 1 print(doc._.last_page) # 4 # Get all of the
+text from a specific PDF page. print(doc._.page(4)) # "able to display the
+destination page (unless..." ``` ## What is *spaCy*? *spaCy* is a natural
+language processing (NLP) tool. It can be used to perform a variety of NLP
+tasks. For more information check out the excellent documentation at [https://
+spacy.io](https://spacy.io). ## Implementation Notes spaCyPDFreader behaves a
+little bit different than your typical [spaCy custom component](https://
+spacy.io/usage/processing-pipelines#custom-components). Typically a spaCy
+component should receive and return a `spacy.tokens.Doc` object. spaCyPDFreader
+breaks this convention because the text must first be extracted from the PDF.
+Instead `pdf_reader` takes a path to a PDF file and a `spacy.Language` object
+as parameters and returns a `spacy.tokens.Doc` object. This allows users an
+easy way to extract text from PDF files while still allowing them use and
+customize all of the features spacy has to offer by allowing you to pass in the
+`spacy.Language` object. Example of a "traditional" spaCy pipeline component
+[negspaCy](https://spacy.io/universe/project/negspacy): ```python import spacy
+from negspacy.negation import Negex nlp = spacy.load("en_core_web_sm")
+nlp.add_pipe("negex", config={"ent_types": ["PERSON", "ORG"]}) doc = nlp("She
+does not like Steve Jobs but likes Apple products.") ``` Example of
+`spaCyPDFreader` usage: ```python import spacy from spacypdfreader import
+pdf_reader nlp = spacy.load("en_core_web_sm") doc = pdf_reader("tests/data/
+test_pdf_01.pdf", nlp) ``` Note that the `nlp.add_pipe` is not used by
+spaCyPDFreader.
```

