# Comparing `tmp/itkwasm_dicom-2.0.1.tar.gz` & `tmp/itkwasm_dicom-2.0.2.tar.gz`

## Comparing `itkwasm_dicom-2.0.1.tar` & `itkwasm_dicom-2.0.2.tar`

### file list

```diff
@@ -1,21 +1,116 @@
--rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 itkwasm_dicom-2.0.1/docs/Makefile
--rw-r--r--   0        0        0     1545 2020-02-02 00:00:00.000000 itkwasm_dicom-2.0.1/docs/conf.py
--rw-r--r--   0        0        0      377 2020-02-02 00:00:00.000000 itkwasm_dicom-2.0.1/docs/index.md
--rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 itkwasm_dicom-2.0.1/docs/make.bat
--rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 itkwasm_dicom-2.0.1/docs/requirements.txt
--rw-r--r--   0        0        0    13605 2020-02-02 00:00:00.000000 itkwasm_dicom-2.0.1/docs/_static/favicon.png
--rw-r--r--   0        0        0     2949 2020-02-02 00:00:00.000000 itkwasm_dicom-2.0.1/docs/_static/logo.svg
--rw-r--r--   0        0        0      717 2020-02-02 00:00:00.000000 itkwasm_dicom-2.0.1/itkwasm_dicom/__init__.py
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 itkwasm_dicom-2.0.1/itkwasm_dicom/_version.py
--rw-r--r--   0        0        0     1582 2020-02-02 00:00:00.000000 itkwasm_dicom-2.0.1/itkwasm_dicom/apply_presentation_state_to_image.py
--rw-r--r--   0        0        0     1606 2020-02-02 00:00:00.000000 itkwasm_dicom-2.0.1/itkwasm_dicom/apply_presentation_state_to_image_async.py
--rw-r--r--   0        0        0     2995 2020-02-02 00:00:00.000000 itkwasm_dicom-2.0.1/itkwasm_dicom/read_dicom_encapsulated_pdf.py
--rw-r--r--   0        0        0     3019 2020-02-02 00:00:00.000000 itkwasm_dicom-2.0.1/itkwasm_dicom/read_dicom_encapsulated_pdf_async.py
--rw-r--r--   0        0        0     7840 2020-02-02 00:00:00.000000 itkwasm_dicom-2.0.1/itkwasm_dicom/structured_report_to_html.py
--rw-r--r--   0        0        0     7864 2020-02-02 00:00:00.000000 itkwasm_dicom-2.0.1/itkwasm_dicom/structured_report_to_html_async.py
--rw-r--r--   0        0        0     3441 2020-02-02 00:00:00.000000 itkwasm_dicom-2.0.1/itkwasm_dicom/structured_report_to_text.py
--rw-r--r--   0        0        0     3465 2020-02-02 00:00:00.000000 itkwasm_dicom-2.0.1/itkwasm_dicom/structured_report_to_text_async.py
--rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 itkwasm_dicom-2.0.1/.gitignore
--rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 itkwasm_dicom-2.0.1/README.md
--rw-r--r--   0        0        0     1322 2020-02-02 00:00:00.000000 itkwasm_dicom-2.0.1/pyproject.toml
--rw-r--r--   0        0        0     1314 2020-02-02 00:00:00.000000 itkwasm_dicom-2.0.1/PKG-INFO
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 itkwasm_dicom-2.0.2/docs/Makefile
+-rw-r--r--   0        0        0     1545 2020-02-02 00:00:00.000000 itkwasm_dicom-2.0.2/docs/conf.py
+-rw-r--r--   0        0        0      669 2020-02-02 00:00:00.000000 itkwasm_dicom-2.0.2/docs/index.md
+-rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 itkwasm_dicom-2.0.2/docs/make.bat
+-rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 itkwasm_dicom-2.0.2/docs/requirements.txt
+-rw-r--r--   0        0        0  3933370 2020-02-02 00:00:00.000000 itkwasm_dicom-2.0.2/docs/_build/doctrees/environment.pickle
+-rw-r--r--   0        0        0     6056 2020-02-02 00:00:00.000000 itkwasm_dicom-2.0.2/docs/_build/doctrees/index.doctree
+-rw-r--r--   0        0        0     4105 2020-02-02 00:00:00.000000 itkwasm_dicom-2.0.2/docs/_build/doctrees/apidocs/index.doctree
+-rw-r--r--   0        0        0    21964 2020-02-02 00:00:00.000000 itkwasm_dicom-2.0.2/docs/_build/doctrees/apidocs/itkwasm_dicom/itkwasm_dicom.apply_presentation_state_to_image.doctree
+-rw-r--r--   0        0        0    22552 2020-02-02 00:00:00.000000 itkwasm_dicom-2.0.2/docs/_build/doctrees/apidocs/itkwasm_dicom/itkwasm_dicom.apply_presentation_state_to_image_async.doctree
+-rw-r--r--   0        0        0     4816 2020-02-02 00:00:00.000000 itkwasm_dicom-2.0.2/docs/_build/doctrees/apidocs/itkwasm_dicom/itkwasm_dicom.doctree
+-rw-r--r--   0        0        0    39083 2020-02-02 00:00:00.000000 itkwasm_dicom-2.0.2/docs/_build/doctrees/apidocs/itkwasm_dicom/itkwasm_dicom.read_dicom_encapsulated_pdf.doctree
+-rw-r--r--   0        0        0    39671 2020-02-02 00:00:00.000000 itkwasm_dicom-2.0.2/docs/_build/doctrees/apidocs/itkwasm_dicom/itkwasm_dicom.read_dicom_encapsulated_pdf_async.doctree
+-rw-r--r--   0        0        0    88726 2020-02-02 00:00:00.000000 itkwasm_dicom-2.0.2/docs/_build/doctrees/apidocs/itkwasm_dicom/itkwasm_dicom.structured_report_to_html.doctree
+-rw-r--r--   0        0        0    89314 2020-02-02 00:00:00.000000 itkwasm_dicom-2.0.2/docs/_build/doctrees/apidocs/itkwasm_dicom/itkwasm_dicom.structured_report_to_html_async.doctree
+-rw-r--r--   0        0        0    43009 2020-02-02 00:00:00.000000 itkwasm_dicom-2.0.2/docs/_build/doctrees/apidocs/itkwasm_dicom/itkwasm_dicom.structured_report_to_text.doctree
+-rw-r--r--   0        0        0    43597 2020-02-02 00:00:00.000000 itkwasm_dicom-2.0.2/docs/_build/doctrees/apidocs/itkwasm_dicom/itkwasm_dicom.structured_report_to_text_async.doctree
+-rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 itkwasm_dicom-2.0.2/docs/_build/html/.buildinfo
+-rw-r--r--   0        0        0    20877 2020-02-02 00:00:00.000000 itkwasm_dicom-2.0.2/docs/_build/html/genindex.html
+-rw-r--r--   0        0        0    17261 2020-02-02 00:00:00.000000 itkwasm_dicom-2.0.2/docs/_build/html/index.html
+-rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 itkwasm_dicom-2.0.2/docs/_build/html/objects.inv
+-rw-r--r--   0        0        0    16167 2020-02-02 00:00:00.000000 itkwasm_dicom-2.0.2/docs/_build/html/py-modindex.html
+-rw-r--r--   0        0        0    13305 2020-02-02 00:00:00.000000 itkwasm_dicom-2.0.2/docs/_build/html/search.html
+-rw-r--r--   0        0        0    16093 2020-02-02 00:00:00.000000 itkwasm_dicom-2.0.2/docs/_build/html/searchindex.js
+-rw-r--r--   0        0        0    52007 2020-02-02 00:00:00.000000 itkwasm_dicom-2.0.2/docs/_build/html/_images/social_previews/summary_apidocs_index_ee5d9aa3.png
+-rw-r--r--   0        0        0    63872 2020-02-02 00:00:00.000000 itkwasm_dicom-2.0.2/docs/_build/html/_images/social_previews/summary_apidocs_itkwasm_dicom_itkwasm_dicom.apply_presentation_state_to_image_4431682b.png
+-rw-r--r--   0        0        0    63454 2020-02-02 00:00:00.000000 itkwasm_dicom-2.0.2/docs/_build/html/_images/social_previews/summary_apidocs_itkwasm_dicom_itkwasm_dicom.apply_presentation_state_to_image_async_1402aa16.png
+-rw-r--r--   0        0        0    55897 2020-02-02 00:00:00.000000 itkwasm_dicom-2.0.2/docs/_build/html/_images/social_previews/summary_apidocs_itkwasm_dicom_itkwasm_dicom.read_dicom_encapsulated_pdf_async_82f44fbc.png
+-rw-r--r--   0        0        0    55126 2020-02-02 00:00:00.000000 itkwasm_dicom-2.0.2/docs/_build/html/_images/social_previews/summary_apidocs_itkwasm_dicom_itkwasm_dicom.read_dicom_encapsulated_pdf_e800ec07.png
+-rw-r--r--   0        0        0    52778 2020-02-02 00:00:00.000000 itkwasm_dicom-2.0.2/docs/_build/html/_images/social_previews/summary_apidocs_itkwasm_dicom_itkwasm_dicom.structured_report_to_html_5b1cdb8c.png
+-rw-r--r--   0        0        0    54308 2020-02-02 00:00:00.000000 itkwasm_dicom-2.0.2/docs/_build/html/_images/social_previews/summary_apidocs_itkwasm_dicom_itkwasm_dicom.structured_report_to_html_async_61cce5d9.png
+-rw-r--r--   0        0        0    54271 2020-02-02 00:00:00.000000 itkwasm_dicom-2.0.2/docs/_build/html/_images/social_previews/summary_apidocs_itkwasm_dicom_itkwasm_dicom.structured_report_to_html_async_c27ed679.png
+-rw-r--r--   0        0        0    56851 2020-02-02 00:00:00.000000 itkwasm_dicom-2.0.2/docs/_build/html/_images/social_previews/summary_apidocs_itkwasm_dicom_itkwasm_dicom.structured_report_to_text_196f5c98.png
+-rw-r--r--   0        0        0    58761 2020-02-02 00:00:00.000000 itkwasm_dicom-2.0.2/docs/_build/html/_images/social_previews/summary_apidocs_itkwasm_dicom_itkwasm_dicom.structured_report_to_text_async_ca1b02de.png
+-rw-r--r--   0        0        0    53721 2020-02-02 00:00:00.000000 itkwasm_dicom-2.0.2/docs/_build/html/_images/social_previews/summary_apidocs_itkwasm_dicom_itkwasm_dicom_cc35cb55.png
+-rw-r--r--   0        0        0    51482 2020-02-02 00:00:00.000000 itkwasm_dicom-2.0.2/docs/_build/html/_images/social_previews/summary_index_8d664e8d.png
+-rw-r--r--   0        0        0    39331 2020-02-02 00:00:00.000000 itkwasm_dicom-2.0.2/docs/_build/html/_images/social_previews/summary_index_e7f4a603.png
+-rw-r--r--   0        0        0      669 2020-02-02 00:00:00.000000 itkwasm_dicom-2.0.2/docs/_build/html/_sources/index.md.txt
+-rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 itkwasm_dicom-2.0.2/docs/_build/html/_sources/apidocs/index.rst.txt
+-rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 itkwasm_dicom-2.0.2/docs/_build/html/_sources/apidocs/itkwasm_dicom/itkwasm_dicom.apply_presentation_state_to_image.md.txt
+-rw-r--r--   0        0        0     1149 2020-02-02 00:00:00.000000 itkwasm_dicom-2.0.2/docs/_build/html/_sources/apidocs/itkwasm_dicom/itkwasm_dicom.apply_presentation_state_to_image_async.md.txt
+-rw-r--r--   0        0        0      541 2020-02-02 00:00:00.000000 itkwasm_dicom-2.0.2/docs/_build/html/_sources/apidocs/itkwasm_dicom/itkwasm_dicom.md.txt
+-rw-r--r--   0        0        0     1270 2020-02-02 00:00:00.000000 itkwasm_dicom-2.0.2/docs/_build/html/_sources/apidocs/itkwasm_dicom/itkwasm_dicom.read_dicom_encapsulated_pdf.md.txt
+-rw-r--r--   0        0        0     1356 2020-02-02 00:00:00.000000 itkwasm_dicom-2.0.2/docs/_build/html/_sources/apidocs/itkwasm_dicom/itkwasm_dicom.read_dicom_encapsulated_pdf_async.md.txt
+-rw-r--r--   0        0        0     2083 2020-02-02 00:00:00.000000 itkwasm_dicom-2.0.2/docs/_build/html/_sources/apidocs/itkwasm_dicom/itkwasm_dicom.structured_report_to_html.md.txt
+-rw-r--r--   0        0        0     2169 2020-02-02 00:00:00.000000 itkwasm_dicom-2.0.2/docs/_build/html/_sources/apidocs/itkwasm_dicom/itkwasm_dicom.structured_report_to_html_async.md.txt
+-rw-r--r--   0        0        0     1359 2020-02-02 00:00:00.000000 itkwasm_dicom-2.0.2/docs/_build/html/_sources/apidocs/itkwasm_dicom/itkwasm_dicom.structured_report_to_text.md.txt
+-rw-r--r--   0        0        0     1445 2020-02-02 00:00:00.000000 itkwasm_dicom-2.0.2/docs/_build/html/_sources/apidocs/itkwasm_dicom/itkwasm_dicom.structured_report_to_text_async.md.txt
+-rw-r--r--   0        0        0    48417 2020-02-02 00:00:00.000000 itkwasm_dicom-2.0.2/docs/_build/html/_sphinx_design_static/design-style.1e8bd061cd6da7fc9cf755528e8ffc24.min.css
+-rw-r--r--   0        0        0      770 2020-02-02 00:00:00.000000 itkwasm_dicom-2.0.2/docs/_build/html/_sphinx_design_static/design-tabs.js
+-rw-r--r--   0        0        0    14813 2020-02-02 00:00:00.000000 itkwasm_dicom-2.0.2/docs/_build/html/_static/basic.css
+-rw-r--r--   0        0        0      313 2020-02-02 00:00:00.000000 itkwasm_dicom-2.0.2/docs/_build/html/_static/check-solid.svg
+-rw-r--r--   0        0        0     9031 2020-02-02 00:00:00.000000 itkwasm_dicom-2.0.2/docs/_build/html/_static/clipboard.min.js
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 itkwasm_dicom-2.0.2/docs/_build/html/_static/copy-button.svg
+-rw-r--r--   0        0        0     2060 2020-02-02 00:00:00.000000 itkwasm_dicom-2.0.2/docs/_build/html/_static/copybutton.css
+-rw-r--r--   0        0        0     8467 2020-02-02 00:00:00.000000 itkwasm_dicom-2.0.2/docs/_build/html/_static/copybutton.js
+-rw-r--r--   0        0        0     2698 2020-02-02 00:00:00.000000 itkwasm_dicom-2.0.2/docs/_build/html/_static/copybutton_funcs.js
+-rw-r--r--   0        0        0     1266 2020-02-02 00:00:00.000000 itkwasm_dicom-2.0.2/docs/_build/html/_static/debug.css
+-rw-r--r--   0        0        0    48417 2020-02-02 00:00:00.000000 itkwasm_dicom-2.0.2/docs/_build/html/_static/design-style.1e8bd061cd6da7fc9cf755528e8ffc24.min.css
+-rw-r--r--   0        0        0      770 2020-02-02 00:00:00.000000 itkwasm_dicom-2.0.2/docs/_build/html/_static/design-tabs.js
+-rw-r--r--   0        0        0     4472 2020-02-02 00:00:00.000000 itkwasm_dicom-2.0.2/docs/_build/html/_static/doctools.js
+-rw-r--r--   0        0        0      415 2020-02-02 00:00:00.000000 itkwasm_dicom-2.0.2/docs/_build/html/_static/documentation_options.js
+-rw-r--r--   0        0        0    13605 2020-02-02 00:00:00.000000 itkwasm_dicom-2.0.2/docs/_build/html/_static/favicon.png
+-rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 itkwasm_dicom-2.0.2/docs/_build/html/_static/file.png
+-rw-r--r--   0        0        0     4758 2020-02-02 00:00:00.000000 itkwasm_dicom-2.0.2/docs/_build/html/_static/language_data.js
+-rw-r--r--   0        0        0     2949 2020-02-02 00:00:00.000000 itkwasm_dicom-2.0.2/docs/_build/html/_static/logo.svg
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 itkwasm_dicom-2.0.2/docs/_build/html/_static/minus.png
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 itkwasm_dicom-2.0.2/docs/_build/html/_static/plus.png
+-rw-r--r--   0        0        0    21072 2020-02-02 00:00:00.000000 itkwasm_dicom-2.0.2/docs/_build/html/_static/pygments.css
+-rw-r--r--   0        0        0    18215 2020-02-02 00:00:00.000000 itkwasm_dicom-2.0.2/docs/_build/html/_static/searchtools.js
+-rw-r--r--   0        0        0     6034 2020-02-02 00:00:00.000000 itkwasm_dicom-2.0.2/docs/_build/html/_static/skeleton.css
+-rw-r--r--   0        0        0     4712 2020-02-02 00:00:00.000000 itkwasm_dicom-2.0.2/docs/_build/html/_static/sphinx_highlight.js
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 itkwasm_dicom-2.0.2/docs/_build/html/_static/scripts/furo-extensions.js
+-rw-r--r--   0        0        0     5265 2020-02-02 00:00:00.000000 itkwasm_dicom-2.0.2/docs/_build/html/_static/scripts/furo.js
+-rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 itkwasm_dicom-2.0.2/docs/_build/html/_static/scripts/furo.js.LICENSE.txt
+-rw-r--r--   0        0        0    28242 2020-02-02 00:00:00.000000 itkwasm_dicom-2.0.2/docs/_build/html/_static/scripts/furo.js.map
+-rw-r--r--   0        0        0     5529 2020-02-02 00:00:00.000000 itkwasm_dicom-2.0.2/docs/_build/html/_static/styles/furo-extensions.css
+-rw-r--r--   0        0        0     7809 2020-02-02 00:00:00.000000 itkwasm_dicom-2.0.2/docs/_build/html/_static/styles/furo-extensions.css.map
+-rw-r--r--   0        0        0    48697 2020-02-02 00:00:00.000000 itkwasm_dicom-2.0.2/docs/_build/html/_static/styles/furo.css
+-rw-r--r--   0        0        0    73615 2020-02-02 00:00:00.000000 itkwasm_dicom-2.0.2/docs/_build/html/_static/styles/furo.css.map
+-rw-r--r--   0        0        0    18952 2020-02-02 00:00:00.000000 itkwasm_dicom-2.0.2/docs/_build/html/apidocs/index.html
+-rw-r--r--   0        0        0    24619 2020-02-02 00:00:00.000000 itkwasm_dicom-2.0.2/docs/_build/html/apidocs/itkwasm_dicom/itkwasm_dicom.apply_presentation_state_to_image.html
+-rw-r--r--   0        0        0    24902 2020-02-02 00:00:00.000000 itkwasm_dicom-2.0.2/docs/_build/html/apidocs/itkwasm_dicom/itkwasm_dicom.apply_presentation_state_to_image_async.html
+-rw-r--r--   0        0        0    19103 2020-02-02 00:00:00.000000 itkwasm_dicom-2.0.2/docs/_build/html/apidocs/itkwasm_dicom/itkwasm_dicom.html
+-rw-r--r--   0        0        0    31295 2020-02-02 00:00:00.000000 itkwasm_dicom-2.0.2/docs/_build/html/apidocs/itkwasm_dicom/itkwasm_dicom.read_dicom_encapsulated_pdf.html
+-rw-r--r--   0        0        0    31624 2020-02-02 00:00:00.000000 itkwasm_dicom-2.0.2/docs/_build/html/apidocs/itkwasm_dicom/itkwasm_dicom.read_dicom_encapsulated_pdf_async.html
+-rw-r--r--   0        0        0    50342 2020-02-02 00:00:00.000000 itkwasm_dicom-2.0.2/docs/_build/html/apidocs/itkwasm_dicom/itkwasm_dicom.structured_report_to_html.html
+-rw-r--r--   0        0        0    50767 2020-02-02 00:00:00.000000 itkwasm_dicom-2.0.2/docs/_build/html/apidocs/itkwasm_dicom/itkwasm_dicom.structured_report_to_html_async.html
+-rw-r--r--   0        0        0    32800 2020-02-02 00:00:00.000000 itkwasm_dicom-2.0.2/docs/_build/html/apidocs/itkwasm_dicom/itkwasm_dicom.structured_report_to_text.html
+-rw-r--r--   0        0        0    32386 2020-02-02 00:00:00.000000 itkwasm_dicom-2.0.2/docs/_build/html/apidocs/itkwasm_dicom/itkwasm_dicom.structured_report_to_text_async.html
+-rw-r--r--   0        0        0    13605 2020-02-02 00:00:00.000000 itkwasm_dicom-2.0.2/docs/_static/favicon.png
+-rw-r--r--   0        0        0     2949 2020-02-02 00:00:00.000000 itkwasm_dicom-2.0.2/docs/_static/logo.svg
+-rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 itkwasm_dicom-2.0.2/docs/apidocs/index.rst
+-rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 itkwasm_dicom-2.0.2/docs/apidocs/itkwasm_dicom/itkwasm_dicom.apply_presentation_state_to_image.md
+-rw-r--r--   0        0        0     1149 2020-02-02 00:00:00.000000 itkwasm_dicom-2.0.2/docs/apidocs/itkwasm_dicom/itkwasm_dicom.apply_presentation_state_to_image_async.md
+-rw-r--r--   0        0        0      541 2020-02-02 00:00:00.000000 itkwasm_dicom-2.0.2/docs/apidocs/itkwasm_dicom/itkwasm_dicom.md
+-rw-r--r--   0        0        0     1270 2020-02-02 00:00:00.000000 itkwasm_dicom-2.0.2/docs/apidocs/itkwasm_dicom/itkwasm_dicom.read_dicom_encapsulated_pdf.md
+-rw-r--r--   0        0        0     1356 2020-02-02 00:00:00.000000 itkwasm_dicom-2.0.2/docs/apidocs/itkwasm_dicom/itkwasm_dicom.read_dicom_encapsulated_pdf_async.md
+-rw-r--r--   0        0        0     2083 2020-02-02 00:00:00.000000 itkwasm_dicom-2.0.2/docs/apidocs/itkwasm_dicom/itkwasm_dicom.structured_report_to_html.md
+-rw-r--r--   0        0        0     2169 2020-02-02 00:00:00.000000 itkwasm_dicom-2.0.2/docs/apidocs/itkwasm_dicom/itkwasm_dicom.structured_report_to_html_async.md
+-rw-r--r--   0        0        0     1359 2020-02-02 00:00:00.000000 itkwasm_dicom-2.0.2/docs/apidocs/itkwasm_dicom/itkwasm_dicom.structured_report_to_text.md
+-rw-r--r--   0        0        0     1445 2020-02-02 00:00:00.000000 itkwasm_dicom-2.0.2/docs/apidocs/itkwasm_dicom/itkwasm_dicom.structured_report_to_text_async.md
+-rw-r--r--   0        0        0      717 2020-02-02 00:00:00.000000 itkwasm_dicom-2.0.2/itkwasm_dicom/__init__.py
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 itkwasm_dicom-2.0.2/itkwasm_dicom/_version.py
+-rw-r--r--   0        0        0     1582 2020-02-02 00:00:00.000000 itkwasm_dicom-2.0.2/itkwasm_dicom/apply_presentation_state_to_image.py
+-rw-r--r--   0        0        0     1606 2020-02-02 00:00:00.000000 itkwasm_dicom-2.0.2/itkwasm_dicom/apply_presentation_state_to_image_async.py
+-rw-r--r--   0        0        0     2995 2020-02-02 00:00:00.000000 itkwasm_dicom-2.0.2/itkwasm_dicom/read_dicom_encapsulated_pdf.py
+-rw-r--r--   0        0        0     3019 2020-02-02 00:00:00.000000 itkwasm_dicom-2.0.2/itkwasm_dicom/read_dicom_encapsulated_pdf_async.py
+-rw-r--r--   0        0        0     7840 2020-02-02 00:00:00.000000 itkwasm_dicom-2.0.2/itkwasm_dicom/structured_report_to_html.py
+-rw-r--r--   0        0        0     7864 2020-02-02 00:00:00.000000 itkwasm_dicom-2.0.2/itkwasm_dicom/structured_report_to_html_async.py
+-rw-r--r--   0        0        0     3441 2020-02-02 00:00:00.000000 itkwasm_dicom-2.0.2/itkwasm_dicom/structured_report_to_text.py
+-rw-r--r--   0        0        0     3465 2020-02-02 00:00:00.000000 itkwasm_dicom-2.0.2/itkwasm_dicom/structured_report_to_text_async.py
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 itkwasm_dicom-2.0.2/.gitignore
+-rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 itkwasm_dicom-2.0.2/README.md
+-rw-r--r--   0        0        0     1531 2020-02-02 00:00:00.000000 itkwasm_dicom-2.0.2/pyproject.toml
+-rw-r--r--   0        0        0     1537 2020-02-02 00:00:00.000000 itkwasm_dicom-2.0.2/PKG-INFO
```

### Comparing `itkwasm_dicom-2.0.1/docs/Makefile` & `itkwasm_dicom-2.0.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `itkwasm_dicom-2.0.1/docs/conf.py` & `itkwasm_dicom-2.0.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `itkwasm_dicom-2.0.1/docs/make.bat` & `itkwasm_dicom-2.0.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `itkwasm_dicom-2.0.1/docs/_static/favicon.png` & `itkwasm_dicom-2.0.2/docs/_build/html/_static/favicon.png`

 * *Files identical despite different names*

### Comparing `itkwasm_dicom-2.0.1/docs/_static/logo.svg` & `itkwasm_dicom-2.0.2/docs/_build/html/_static/logo.svg`

 * *Files identical despite different names*

### Comparing `itkwasm_dicom-2.0.1/itkwasm_dicom/__init__.py` & `itkwasm_dicom-2.0.2/itkwasm_dicom/__init__.py`

 * *Files identical despite different names*

### Comparing `itkwasm_dicom-2.0.1/itkwasm_dicom/apply_presentation_state_to_image.py` & `itkwasm_dicom-2.0.2/itkwasm_dicom/apply_presentation_state_to_image.py`

 * *Files identical despite different names*

### Comparing `itkwasm_dicom-2.0.1/itkwasm_dicom/apply_presentation_state_to_image_async.py` & `itkwasm_dicom-2.0.2/itkwasm_dicom/apply_presentation_state_to_image_async.py`

 * *Files identical despite different names*

### Comparing `itkwasm_dicom-2.0.1/itkwasm_dicom/read_dicom_encapsulated_pdf.py` & `itkwasm_dicom-2.0.2/itkwasm_dicom/read_dicom_encapsulated_pdf.py`

 * *Files identical despite different names*

### Comparing `itkwasm_dicom-2.0.1/itkwasm_dicom/read_dicom_encapsulated_pdf_async.py` & `itkwasm_dicom-2.0.2/itkwasm_dicom/read_dicom_encapsulated_pdf_async.py`

 * *Files identical despite different names*

### Comparing `itkwasm_dicom-2.0.1/itkwasm_dicom/structured_report_to_html.py` & `itkwasm_dicom-2.0.2/itkwasm_dicom/structured_report_to_html.py`

 * *Files 0% similar despite different names*

```diff
@@ -80,43 +80,39 @@
 
     :param processing_details: show currently processed content item
     :type  processing_details: bool
 
     :param unknown_relationship: accept unknown/missing relationship type
     :type  unknown_relationship: bool
 
-    :param invalid_item_value: accept invalid content item value
-(e.g. violation of VR or VM definition)
+    :param invalid_item_value: accept invalid content item value (e.g. violation of VR or VM definition)
     :type  invalid_item_value: bool
 
     :param ignore_constraints: ignore relationship content constraints
     :type  ignore_constraints: bool
 
-    :param ignore_item_errors: do not abort on content item errors, just warn
-(e.g. missing value type specific attributes)
+    :param ignore_item_errors: do not abort on content item errors, just warn (e.g. missing value type specific attributes)
     :type  ignore_item_errors: bool
 
     :param skip_invalid_items: skip invalid content items (incl. sub-tree)
     :type  skip_invalid_items: bool
 
     :param disable_vr_checker: disable check for VR-conformant string values
     :type  disable_vr_checker: bool
 
     :param charset_require: require declaration of ext. charset (default)
     :type  charset_require: bool
 
     :param charset_assume: [c]harset: string, assume charset c if no extended charset declared
     :type  charset_assume: str
 
-    :param charset_check_all: check all data elements with string values
-(default: only PN, LO, LT, SH, ST, UC and UT)
+    :param charset_check_all: check all data elements with string values (default: only PN, LO, LT, SH, ST, UC and UT)
     :type  charset_check_all: bool
 
-    :param convert_to_utf8: convert all element values that are affected
-by Specific Character Set (0008,0005) to UTF-8
+    :param convert_to_utf8: convert all element values that are affected by Specific Character Set (0008,0005) to UTF-8
     :type  convert_to_utf8: bool
 
     :param url_prefix: URL: string. Append specificed URL prefix to hyperlinks of referenced composite objects in the document.
     :type  url_prefix: str
 
     :param html_32: use only HTML version 3.2 compatible features
     :type  html_32: bool
```

### Comparing `itkwasm_dicom-2.0.1/itkwasm_dicom/structured_report_to_html_async.py` & `itkwasm_dicom-2.0.2/itkwasm_dicom/structured_report_to_html_async.py`

 * *Files 1% similar despite different names*

```diff
@@ -80,43 +80,39 @@
 
     :param processing_details: show currently processed content item
     :type  processing_details: bool
 
     :param unknown_relationship: accept unknown/missing relationship type
     :type  unknown_relationship: bool
 
-    :param invalid_item_value: accept invalid content item value
-(e.g. violation of VR or VM definition)
+    :param invalid_item_value: accept invalid content item value (e.g. violation of VR or VM definition)
     :type  invalid_item_value: bool
 
     :param ignore_constraints: ignore relationship content constraints
     :type  ignore_constraints: bool
 
-    :param ignore_item_errors: do not abort on content item errors, just warn
-(e.g. missing value type specific attributes)
+    :param ignore_item_errors: do not abort on content item errors, just warn (e.g. missing value type specific attributes)
     :type  ignore_item_errors: bool
 
     :param skip_invalid_items: skip invalid content items (incl. sub-tree)
     :type  skip_invalid_items: bool
 
     :param disable_vr_checker: disable check for VR-conformant string values
     :type  disable_vr_checker: bool
 
     :param charset_require: require declaration of ext. charset (default)
     :type  charset_require: bool
 
     :param charset_assume: [c]harset: string, assume charset c if no extended charset declared
     :type  charset_assume: str
 
-    :param charset_check_all: check all data elements with string values
-(default: only PN, LO, LT, SH, ST, UC and UT)
+    :param charset_check_all: check all data elements with string values (default: only PN, LO, LT, SH, ST, UC and UT)
     :type  charset_check_all: bool
 
-    :param convert_to_utf8: convert all element values that are affected
-by Specific Character Set (0008,0005) to UTF-8
+    :param convert_to_utf8: convert all element values that are affected by Specific Character Set (0008,0005) to UTF-8
     :type  convert_to_utf8: bool
 
     :param url_prefix: URL: string. Append specificed URL prefix to hyperlinks of referenced composite objects in the document.
     :type  url_prefix: str
 
     :param html_32: use only HTML version 3.2 compatible features
     :type  html_32: bool
```

### Comparing `itkwasm_dicom-2.0.1/itkwasm_dicom/structured_report_to_text.py` & `itkwasm_dicom-2.0.2/itkwasm_dicom/structured_report_to_text.py`

 * *Files identical despite different names*

### Comparing `itkwasm_dicom-2.0.1/itkwasm_dicom/structured_report_to_text_async.py` & `itkwasm_dicom-2.0.2/itkwasm_dicom/structured_report_to_text_async.py`

 * *Files identical despite different names*

### Comparing `itkwasm_dicom-2.0.1/pyproject.toml` & `itkwasm_dicom-2.0.2/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -35,14 +35,19 @@
 dependencies = [
     "itkwasm >= 1.0.b103",
     "itkwasm-dicom-wasi; sys_platform != \"emscripten\"",
     "itkwasm-dicom-emscripten; sys_platform == \"emscripten\"",
 
 ]
 
+[project.urls]
+Home = "https://itk-wasm-dicom-python-docs.on.fleek.co"
+Source = "https://github.com/InsightSoftwareConsortium/itk-wasm"
+Issues = "https://github.com/InsightSoftwareConsortium/itk-wasm/issues"
+
 [tool.hatch.version]
 path = "itkwasm_dicom/_version.py"
 
 [tool.hatch.envs.default]
 dependencies = [
   "pytest",
 ]
```

### Comparing `itkwasm_dicom-2.0.1/PKG-INFO` & `itkwasm_dicom-2.0.2/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,13 @@
 Metadata-Version: 2.1
 Name: itkwasm-dicom
-Version: 2.0.1
+Version: 2.0.2
+Project-URL: Home, https://itk-wasm-dicom-python-docs.on.fleek.co
+Project-URL: Source, https://github.com/InsightSoftwareConsortium/itk-wasm
+Project-URL: Issues, https://github.com/InsightSoftwareConsortium/itk-wasm/issues
 License-Expression: Apache-2.0
 Keywords: emscripten,itkwasm,wasi,webassembly
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: WebAssembly
 Classifier: Environment :: WebAssembly :: Emscripten
 Classifier: Environment :: WebAssembly :: WASI
 Classifier: Intended Audience :: Developers
```

