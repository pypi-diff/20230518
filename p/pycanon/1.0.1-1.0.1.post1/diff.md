# Comparing `tmp/pycanon-1.0.1.tar.gz` & `tmp/pycanon-1.0.1.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycanon-1.0.1.tar", last modified: Wed May 17 14:10:43 2023, max compression
+gzip compressed data, was "pycanon-1.0.1.post1.tar", last modified: Thu May 18 15:06:18 2023, max compression
```

## Comparing `pycanon-1.0.1.tar` & `pycanon-1.0.1.post1.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxrwxr-x   0 judith    (1000) judith    (1000)        0 2023-05-17 14:10:43.209757 pycanon-1.0.1/
--rw-rw-r--   0 judith    (1000) judith    (1000)    11355 2023-05-12 12:04:19.000000 pycanon-1.0.1/LICENSE
--rw-rw-r--   0 judith    (1000) judith    (1000)       25 2023-05-12 12:04:19.000000 pycanon-1.0.1/MANIFEST.in
--rw-rw-r--   0 judith    (1000) judith    (1000)     6828 2023-05-17 14:10:43.209757 pycanon-1.0.1/PKG-INFO
--rw-rw-r--   0 judith    (1000) judith    (1000)     5773 2023-05-12 12:04:19.000000 pycanon-1.0.1/README.rst
-drwxrwxr-x   0 judith    (1000) judith    (1000)        0 2023-05-17 14:10:43.209757 pycanon-1.0.1/pycanon/
--rw-rw-r--   0 judith    (1000) judith    (1000)      741 2023-05-15 06:37:16.000000 pycanon-1.0.1/pycanon/__init__.py
-drwxrwxr-x   0 judith    (1000) judith    (1000)        0 2023-05-17 14:10:43.209757 pycanon-1.0.1/pycanon/anonymity/
--rw-rw-r--   0 judith    (1000) judith    (1000)     1501 2023-05-12 12:04:19.000000 pycanon-1.0.1/pycanon/anonymity/__init__.py
--rw-rw-r--   0 judith    (1000) judith    (1000)     4143 2023-05-12 12:04:19.000000 pycanon-1.0.1/pycanon/anonymity/_beta_likeness.py
--rw-rw-r--   0 judith    (1000) judith    (1000)     2430 2023-05-12 12:04:19.000000 pycanon-1.0.1/pycanon/anonymity/_delta_disclosure.py
--rw-rw-r--   0 judith    (1000) judith    (1000)     3788 2023-05-12 12:04:19.000000 pycanon-1.0.1/pycanon/anonymity/_k_anonymity.py
--rw-rw-r--   0 judith    (1000) judith    (1000)     9319 2023-05-12 12:04:19.000000 pycanon-1.0.1/pycanon/anonymity/_l_diversity.py
--rw-rw-r--   0 judith    (1000) judith    (1000)     3135 2023-05-12 12:04:19.000000 pycanon-1.0.1/pycanon/anonymity/_t_closeness.py
-drwxrwxr-x   0 judith    (1000) judith    (1000)        0 2023-05-17 14:10:43.209757 pycanon-1.0.1/pycanon/anonymity/utils/
--rw-rw-r--   0 judith    (1000) judith    (1000)      762 2023-05-12 12:04:19.000000 pycanon-1.0.1/pycanon/anonymity/utils/__init__.py
--rw-rw-r--   0 judith    (1000) judith    (1000)     6889 2023-05-12 12:04:19.000000 pycanon-1.0.1/pycanon/anonymity/utils/aux_anonymity.py
--rw-rw-r--   0 judith    (1000) judith    (1000)     4023 2023-05-12 12:04:19.000000 pycanon-1.0.1/pycanon/anonymity/utils/aux_functions.py
--rw-rw-r--   0 judith    (1000) judith    (1000)    11958 2023-05-12 12:04:19.000000 pycanon-1.0.1/pycanon/cli.py
-drwxrwxr-x   0 judith    (1000) judith    (1000)        0 2023-05-17 14:10:43.209757 pycanon-1.0.1/pycanon/report/
--rw-rw-r--   0 judith    (1000) judith    (1000)     2634 2023-05-15 06:36:57.000000 pycanon-1.0.1/pycanon/report/__init__.py
--rw-rw-r--   0 judith    (1000) judith    (1000)     2547 2023-05-12 12:04:19.000000 pycanon-1.0.1/pycanon/report/base.py
--rw-rw-r--   0 judith    (1000) judith    (1000)     2772 2023-05-12 12:04:19.000000 pycanon-1.0.1/pycanon/report/json.py
--rw-rw-r--   0 judith    (1000) judith    (1000)     5324 2023-05-12 12:04:19.000000 pycanon-1.0.1/pycanon/report/pdf.py
--rw-rw-r--   0 judith    (1000) judith    (1000)     8350 2023-05-12 12:04:19.000000 pycanon-1.0.1/pycanon/report/pdf_utility_report.py
-drwxrwxr-x   0 judith    (1000) judith    (1000)        0 2023-05-17 14:10:43.209757 pycanon-1.0.1/pycanon.egg-info/
--rw-rw-r--   0 judith    (1000) judith    (1000)     6828 2023-05-17 14:10:43.000000 pycanon-1.0.1/pycanon.egg-info/PKG-INFO
--rw-rw-r--   0 judith    (1000) judith    (1000)      790 2023-05-17 14:10:43.000000 pycanon-1.0.1/pycanon.egg-info/SOURCES.txt
--rw-rw-r--   0 judith    (1000) judith    (1000)        1 2023-05-17 14:10:43.000000 pycanon-1.0.1/pycanon.egg-info/dependency_links.txt
--rw-rw-r--   0 judith    (1000) judith    (1000)       44 2023-05-17 14:10:43.000000 pycanon-1.0.1/pycanon.egg-info/entry_points.txt
--rw-rw-r--   0 judith    (1000) judith    (1000)       82 2023-05-17 14:10:43.000000 pycanon-1.0.1/pycanon.egg-info/requires.txt
--rw-rw-r--   0 judith    (1000) judith    (1000)        8 2023-05-17 14:10:43.000000 pycanon-1.0.1/pycanon.egg-info/top_level.txt
--rw-rw-r--   0 judith    (1000) judith    (1000)       85 2023-05-15 06:36:57.000000 pycanon-1.0.1/requirements.txt
--rw-rw-r--   0 judith    (1000) judith    (1000)     1258 2023-05-17 14:10:43.209757 pycanon-1.0.1/setup.cfg
--rw-rw-r--   0 judith    (1000) judith    (1000)      216 2023-05-12 12:04:19.000000 pycanon-1.0.1/setup.py
-drwxrwxr-x   0 judith    (1000) judith    (1000)        0 2023-05-17 14:10:43.209757 pycanon-1.0.1/tests/
--rw-rw-r--   0 judith    (1000) judith    (1000)     1514 2023-05-12 12:04:19.000000 pycanon-1.0.1/tests/test_metrics.py
--rw-rw-r--   0 judith    (1000) judith    (1000)     2760 2023-05-12 12:04:19.000000 pycanon-1.0.1/tests/test_reports.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 15:06:18.431130 pycanon-1.0.1.post1/
+-rw-rw-rw-   0 root         (0) root         (0)    11355 2022-06-28 08:26:43.000000 pycanon-1.0.1.post1/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)       25 2022-08-12 22:06:36.000000 pycanon-1.0.1.post1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     7845 2023-05-18 15:06:18.431130 pycanon-1.0.1.post1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     6764 2023-05-18 11:53:16.000000 pycanon-1.0.1.post1/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 15:06:18.423130 pycanon-1.0.1.post1/pycanon/
+-rw-rw-rw-   0 root         (0) root         (0)      747 2023-05-18 14:26:08.000000 pycanon-1.0.1.post1/pycanon/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 15:06:18.427130 pycanon-1.0.1.post1/pycanon/anonymity/
+-rw-rw-rw-   0 root         (0) root         (0)     1501 2023-03-15 13:21:48.000000 pycanon-1.0.1.post1/pycanon/anonymity/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4143 2023-03-15 13:21:48.000000 pycanon-1.0.1.post1/pycanon/anonymity/_beta_likeness.py
+-rw-rw-rw-   0 root         (0) root         (0)     2430 2023-03-15 13:21:48.000000 pycanon-1.0.1.post1/pycanon/anonymity/_delta_disclosure.py
+-rw-rw-rw-   0 root         (0) root         (0)     3788 2023-03-24 11:50:39.000000 pycanon-1.0.1.post1/pycanon/anonymity/_k_anonymity.py
+-rw-rw-rw-   0 root         (0) root         (0)     9319 2023-03-24 11:50:39.000000 pycanon-1.0.1.post1/pycanon/anonymity/_l_diversity.py
+-rw-rw-rw-   0 root         (0) root         (0)     3135 2023-03-15 13:21:48.000000 pycanon-1.0.1.post1/pycanon/anonymity/_t_closeness.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 15:06:18.427130 pycanon-1.0.1.post1/pycanon/anonymity/utils/
+-rw-rw-rw-   0 root         (0) root         (0)      762 2023-03-24 11:50:39.000000 pycanon-1.0.1.post1/pycanon/anonymity/utils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6889 2023-03-24 11:50:39.000000 pycanon-1.0.1.post1/pycanon/anonymity/utils/aux_anonymity.py
+-rw-rw-rw-   0 root         (0) root         (0)     4023 2023-03-24 11:50:39.000000 pycanon-1.0.1.post1/pycanon/anonymity/utils/aux_functions.py
+-rw-rw-rw-   0 root         (0) root         (0)    11958 2023-03-24 11:50:39.000000 pycanon-1.0.1.post1/pycanon/cli.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 15:06:18.431130 pycanon-1.0.1.post1/pycanon/report/
+-rw-rw-rw-   0 root         (0) root         (0)     2799 2023-05-18 09:47:00.000000 pycanon-1.0.1.post1/pycanon/report/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2496 2023-05-18 07:13:24.000000 pycanon-1.0.1.post1/pycanon/report/base.py
+-rw-rw-rw-   0 root         (0) root         (0)     2772 2023-04-03 08:29:37.000000 pycanon-1.0.1.post1/pycanon/report/json.py
+-rw-rw-rw-   0 root         (0) root         (0)     5324 2023-03-31 12:51:46.000000 pycanon-1.0.1.post1/pycanon/report/pdf.py
+-rw-rw-rw-   0 root         (0) root         (0)     8350 2023-04-03 09:44:48.000000 pycanon-1.0.1.post1/pycanon/report/pdf_utility_report.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 15:06:18.423130 pycanon-1.0.1.post1/pycanon.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     7845 2023-05-18 15:06:18.000000 pycanon-1.0.1.post1/pycanon.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      790 2023-05-18 15:06:18.000000 pycanon-1.0.1.post1/pycanon.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-18 15:06:18.000000 pycanon-1.0.1.post1/pycanon.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       44 2023-05-18 15:06:18.000000 pycanon-1.0.1.post1/pycanon.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       89 2023-05-18 15:06:18.000000 pycanon-1.0.1.post1/pycanon.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-05-18 15:06:18.000000 pycanon-1.0.1.post1/pycanon.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)       60 2023-05-18 09:47:00.000000 pycanon-1.0.1.post1/requirements.txt
+-rw-rw-rw-   0 root         (0) root         (0)     1316 2023-05-18 15:06:18.431130 pycanon-1.0.1.post1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      216 2023-04-03 08:29:37.000000 pycanon-1.0.1.post1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 15:06:18.431130 pycanon-1.0.1.post1/tests/
+-rw-rw-rw-   0 root         (0) root         (0)     1514 2023-04-03 08:29:37.000000 pycanon-1.0.1.post1/tests/test_metrics.py
+-rw-rw-rw-   0 root         (0) root         (0)     2760 2023-04-03 08:29:37.000000 pycanon-1.0.1.post1/tests/test_reports.py
```

### Comparing `pycanon-1.0.1/LICENSE` & `pycanon-1.0.1.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `pycanon-1.0.1/PKG-INFO` & `pycanon-1.0.1.post1/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycanon
-Version: 1.0.1
+Version: 1.0.1.post1
 Summary: pyCANON, A Python library to check the level of anonymity of a dataset
 Home-page: https://gitlab.ifca.es/privacy-security/pycanon
 Author: Judith Sáinz-Pardo Díaz, Álvaro López García (IFCA (CSIC-UC))
 Author-email: sainzpardo@ifca.unican.es, aloga@ifca.unican.es
 License: Apache License 2.0
 Keywords: data,privacy,anonymity
 Classifier: Development Status :: 5 - Production/Stable
@@ -16,14 +16,15 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: Topic :: Security
+Provides-Extra: PDF
 License-File: LICENSE
 
 pyCANON
 =======
 
 |License| |Documentation Status| |Pipeline Status|
 
@@ -46,14 +47,22 @@
 Then run the following command to install the library and all its
 requirements:
 
 ::
 
    pip install pycanon
 
+
+If you also want to install the functionality that allows to generate PDF files
+for the reports, install as follows
+::
+
+   pip install pycanon[PDF]
+
+
 Documentation
 -------------
 
 The pyCANON documentation is hosted on `Read the
 Docs <https://pycanon.readthedocs.io/>`__.
 
 Getting started
@@ -110,14 +119,18 @@
 |                           |                             |            | Distance" is used.                                  |
 +---------------------------+-----------------------------+------------+-----------------------------------------------------+
 | δ-disclosure privacy      | ``delta_disclosure``        | *δ*: float |                                                     |
 +---------------------------+-----------------------------+------------+-----------------------------------------------------+
 
 More information can be found in this `paper <https://www.nature.com/articles/s41597-022-01894-2>`__.
 
+In addition, a report can be obtained including information on the equivalence claases and the 
+usefulness of the data. In particular, for the latter the following three classically used metrics
+are implemented (as defined in the `documentation <https://pycanon.readthedocs.io/>`__): 
+*average equivalence class size*, *classification metric* and *discernability metric*.
 
 Citation
 -----------
 If you are using pyCANON you can cite it as follows:: 
 
    @article{sainzpardo2022pycanon,
       title={A Python library to check the level of anonymity of a dataset},
@@ -125,13 +138,23 @@
       journal={Scientific Data},
       volume={9},
       number={1},
       pages={785},
       year={2022},
       publisher={Nature Publishing Group UK London}}
 
+
+Acknowledgments
+-----------------
+
+The authors would like to thank the funding through the European Union - NextGenerationEU 
+(Regulation EU 2020/2094), through CSIC’s Global Health Platform (PTI+ Salud Global) and 
+the support from the project AI4EOSC “Artificial Intelligence for the European Open Science 
+Cloud” that has received funding from the European Union’s Horizon Europe research and 
+innovation programme under grant agreement number 101058593.
+
 .. |License| image:: https://img.shields.io/badge/License-Apache_2.0-blue.svg
    :target: https://gitlab.ifca.es/sainzj/check-anonymity/-/blob/main/LICENSE
 .. |Documentation Status| image:: https://readthedocs.org/projects/pycanon/badge/?version=latest
    :target: https://pycanon.readthedocs.io/en/latest/?badge=latest
 .. |Pipeline Status| image:: https://gitlab.ifca.es/privacy-security/pycanon/badges/main/pipeline.svg
    :target: https://gitlab.ifca.es/privacy-security/pycanon/-/pipelines
```

### Comparing `pycanon-1.0.1/README.rst` & `pycanon-1.0.1.post1/README.rst`

 * *Files 13% similar despite different names*

```diff
@@ -22,14 +22,22 @@
 Then run the following command to install the library and all its
 requirements:
 
 ::
 
    pip install pycanon
 
+
+If you also want to install the functionality that allows to generate PDF files
+for the reports, install as follows
+::
+
+   pip install pycanon[PDF]
+
+
 Documentation
 -------------
 
 The pyCANON documentation is hosted on `Read the
 Docs <https://pycanon.readthedocs.io/>`__.
 
 Getting started
@@ -86,14 +94,18 @@
 |                           |                             |            | Distance" is used.                                  |
 +---------------------------+-----------------------------+------------+-----------------------------------------------------+
 | δ-disclosure privacy      | ``delta_disclosure``        | *δ*: float |                                                     |
 +---------------------------+-----------------------------+------------+-----------------------------------------------------+
 
 More information can be found in this `paper <https://www.nature.com/articles/s41597-022-01894-2>`__.
 
+In addition, a report can be obtained including information on the equivalence claases and the 
+usefulness of the data. In particular, for the latter the following three classically used metrics
+are implemented (as defined in the `documentation <https://pycanon.readthedocs.io/>`__): 
+*average equivalence class size*, *classification metric* and *discernability metric*.
 
 Citation
 -----------
 If you are using pyCANON you can cite it as follows:: 
 
    @article{sainzpardo2022pycanon,
       title={A Python library to check the level of anonymity of a dataset},
@@ -101,13 +113,23 @@
       journal={Scientific Data},
       volume={9},
       number={1},
       pages={785},
       year={2022},
       publisher={Nature Publishing Group UK London}}
 
+
+Acknowledgments
+-----------------
+
+The authors would like to thank the funding through the European Union - NextGenerationEU 
+(Regulation EU 2020/2094), through CSIC’s Global Health Platform (PTI+ Salud Global) and 
+the support from the project AI4EOSC “Artificial Intelligence for the European Open Science 
+Cloud” that has received funding from the European Union’s Horizon Europe research and 
+innovation programme under grant agreement number 101058593.
+
 .. |License| image:: https://img.shields.io/badge/License-Apache_2.0-blue.svg
    :target: https://gitlab.ifca.es/sainzj/check-anonymity/-/blob/main/LICENSE
 .. |Documentation Status| image:: https://readthedocs.org/projects/pycanon/badge/?version=latest
    :target: https://pycanon.readthedocs.io/en/latest/?badge=latest
 .. |Pipeline Status| image:: https://gitlab.ifca.es/privacy-security/pycanon/badges/main/pipeline.svg
    :target: https://gitlab.ifca.es/privacy-security/pycanon/-/pipelines
```

### Comparing `pycanon-1.0.1/pycanon/__init__.py` & `pycanon-1.0.1.post1/pycanon/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,8 +12,8 @@
 # distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
 # WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
 # License for the specific language governing permissions and limitations
 # under the License.
 
 """pyCANON is a library to check the values of the most common data privacy models."""
 
-__version__ = "1.0.1"
+__version__ = "1.0.1.post1"
```

### Comparing `pycanon-1.0.1/pycanon/anonymity/__init__.py` & `pycanon-1.0.1.post1/pycanon/anonymity/__init__.py`

 * *Files identical despite different names*

### Comparing `pycanon-1.0.1/pycanon/anonymity/_beta_likeness.py` & `pycanon-1.0.1.post1/pycanon/anonymity/_beta_likeness.py`

 * *Files identical despite different names*

### Comparing `pycanon-1.0.1/pycanon/anonymity/_delta_disclosure.py` & `pycanon-1.0.1.post1/pycanon/anonymity/_delta_disclosure.py`

 * *Files identical despite different names*

### Comparing `pycanon-1.0.1/pycanon/anonymity/_k_anonymity.py` & `pycanon-1.0.1.post1/pycanon/anonymity/_k_anonymity.py`

 * *Files identical despite different names*

### Comparing `pycanon-1.0.1/pycanon/anonymity/_l_diversity.py` & `pycanon-1.0.1.post1/pycanon/anonymity/_l_diversity.py`

 * *Files identical despite different names*

### Comparing `pycanon-1.0.1/pycanon/anonymity/_t_closeness.py` & `pycanon-1.0.1.post1/pycanon/anonymity/_t_closeness.py`

 * *Files identical despite different names*

### Comparing `pycanon-1.0.1/pycanon/anonymity/utils/__init__.py` & `pycanon-1.0.1.post1/pycanon/anonymity/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `pycanon-1.0.1/pycanon/anonymity/utils/aux_anonymity.py` & `pycanon-1.0.1.post1/pycanon/anonymity/utils/aux_anonymity.py`

 * *Files identical despite different names*

### Comparing `pycanon-1.0.1/pycanon/anonymity/utils/aux_functions.py` & `pycanon-1.0.1.post1/pycanon/anonymity/utils/aux_functions.py`

 * *Files identical despite different names*

### Comparing `pycanon-1.0.1/pycanon/cli.py` & `pycanon-1.0.1.post1/pycanon/cli.py`

 * *Files identical despite different names*

### Comparing `pycanon-1.0.1/pycanon/report/__init__.py` & `pycanon-1.0.1.post1/pycanon/report/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -14,18 +14,27 @@
 # License for the specific language governing permissions and limitations
 # under the License.
 
 """Generate reports with all privacy model's scores."""
 
 import pandas as pd
 
-from pycanon.report.base import get_report_values
-from pycanon.report.json import get_json_report
-from pycanon.report.pdf import get_pdf_report
-from pycanon.report.pdf_utility_report import get_pdf_utility_report
+from pycanon.report.base import get_report_values  # noqa(F401)
+from pycanon.report.json import get_json_report  # noqa(F401)
+
+try:
+    from pycanon.report.pdf import get_pdf_report  # noqa(F401)
+    from pycanon.report.pdf_utility_report import get_pdf_utility_report  # noqa(F401)
+except ImportError:
+    __all_pdf__ = []
+else:
+    __all_pdf__ = [
+        "get_pdf_report",
+        "get_pdf_utility_report",
+    ]
 
 
 def print_report(
     data: pd.DataFrame, quasi_ident: list, sens_att: list, gen=True
 ) -> None:
     """Generate a report with the parameters obtained for each anonymity check.
 
@@ -69,11 +78,9 @@
           \t - delta-disclosure privacy with delta = {delta_disc}"""
     )
 
 
 __all__ = [
     "print_report",
     "get_json_report",
-    "get_pdf_report",
     "get_report_values",
-    "get_pdf_utility_report",
-]
+] + __all_pdf__
```

### Comparing `pycanon-1.0.1/pycanon/report/base.py` & `pycanon-1.0.1.post1/pycanon/report/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,15 +51,14 @@
     entropy_l = anonymity.entropy_l_diversity(data, quasi_ident, sens_att, gen)
     c_div, l_c_div = anonymity.recursive_c_l_diversity(data, quasi_ident, sens_att, gen)
     basic_beta = anonymity.basic_beta_likeness(data, quasi_ident, sens_att, gen)
     enhanced_beta = anonymity.enhanced_beta_likeness(data, quasi_ident, sens_att, gen)
     delta_disc = anonymity.delta_disclosure(data, quasi_ident, sens_att, gen)
     t_clos = anonymity.t_closeness(data, quasi_ident, sens_att, gen)
 
-    # TODO(aloga): Move to a better data type here
     return (
         k_anon,
         (alpha, alpha_k),
         l_div,
         entropy_l,
         (c_div, l_c_div),
         basic_beta,
```

### Comparing `pycanon-1.0.1/pycanon/report/json.py` & `pycanon-1.0.1.post1/pycanon/report/json.py`

 * *Files identical despite different names*

### Comparing `pycanon-1.0.1/pycanon/report/pdf.py` & `pycanon-1.0.1.post1/pycanon/report/pdf.py`

 * *Files identical despite different names*

### Comparing `pycanon-1.0.1/pycanon/report/pdf_utility_report.py` & `pycanon-1.0.1.post1/pycanon/report/pdf_utility_report.py`

 * *Files identical despite different names*

### Comparing `pycanon-1.0.1/pycanon.egg-info/PKG-INFO` & `pycanon-1.0.1.post1/pycanon.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycanon
-Version: 1.0.1
+Version: 1.0.1.post1
 Summary: pyCANON, A Python library to check the level of anonymity of a dataset
 Home-page: https://gitlab.ifca.es/privacy-security/pycanon
 Author: Judith Sáinz-Pardo Díaz, Álvaro López García (IFCA (CSIC-UC))
 Author-email: sainzpardo@ifca.unican.es, aloga@ifca.unican.es
 License: Apache License 2.0
 Keywords: data,privacy,anonymity
 Classifier: Development Status :: 5 - Production/Stable
@@ -16,14 +16,15 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: Topic :: Security
+Provides-Extra: PDF
 License-File: LICENSE
 
 pyCANON
 =======
 
 |License| |Documentation Status| |Pipeline Status|
 
@@ -46,14 +47,22 @@
 Then run the following command to install the library and all its
 requirements:
 
 ::
 
    pip install pycanon
 
+
+If you also want to install the functionality that allows to generate PDF files
+for the reports, install as follows
+::
+
+   pip install pycanon[PDF]
+
+
 Documentation
 -------------
 
 The pyCANON documentation is hosted on `Read the
 Docs <https://pycanon.readthedocs.io/>`__.
 
 Getting started
@@ -110,14 +119,18 @@
 |                           |                             |            | Distance" is used.                                  |
 +---------------------------+-----------------------------+------------+-----------------------------------------------------+
 | δ-disclosure privacy      | ``delta_disclosure``        | *δ*: float |                                                     |
 +---------------------------+-----------------------------+------------+-----------------------------------------------------+
 
 More information can be found in this `paper <https://www.nature.com/articles/s41597-022-01894-2>`__.
 
+In addition, a report can be obtained including information on the equivalence claases and the 
+usefulness of the data. In particular, for the latter the following three classically used metrics
+are implemented (as defined in the `documentation <https://pycanon.readthedocs.io/>`__): 
+*average equivalence class size*, *classification metric* and *discernability metric*.
 
 Citation
 -----------
 If you are using pyCANON you can cite it as follows:: 
 
    @article{sainzpardo2022pycanon,
       title={A Python library to check the level of anonymity of a dataset},
@@ -125,13 +138,23 @@
       journal={Scientific Data},
       volume={9},
       number={1},
       pages={785},
       year={2022},
       publisher={Nature Publishing Group UK London}}
 
+
+Acknowledgments
+-----------------
+
+The authors would like to thank the funding through the European Union - NextGenerationEU 
+(Regulation EU 2020/2094), through CSIC’s Global Health Platform (PTI+ Salud Global) and 
+the support from the project AI4EOSC “Artificial Intelligence for the European Open Science 
+Cloud” that has received funding from the European Union’s Horizon Europe research and 
+innovation programme under grant agreement number 101058593.
+
 .. |License| image:: https://img.shields.io/badge/License-Apache_2.0-blue.svg
    :target: https://gitlab.ifca.es/sainzj/check-anonymity/-/blob/main/LICENSE
 .. |Documentation Status| image:: https://readthedocs.org/projects/pycanon/badge/?version=latest
    :target: https://pycanon.readthedocs.io/en/latest/?badge=latest
 .. |Pipeline Status| image:: https://gitlab.ifca.es/privacy-security/pycanon/badges/main/pipeline.svg
    :target: https://gitlab.ifca.es/privacy-security/pycanon/-/pipelines
```

### Comparing `pycanon-1.0.1/pycanon.egg-info/SOURCES.txt` & `pycanon-1.0.1.post1/pycanon.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pycanon-1.0.1/setup.cfg` & `pycanon-1.0.1.post1/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -31,14 +31,18 @@
 	pycanon.anonymity.utils
 	pycanon.report
 
 [options.entry_points]
 console_scripts = 
 	pycanon = pycanon.cli:app
 
+[options.extras_require]
+PDF = 
+	reportlab>=3.6.9,<4.0.0
+
 [build_sphinx]
 source_dir = doc/source
 build_dir = doc/build
 all_files = 1
 
 [egg_info]
 tag_build =
```

### Comparing `pycanon-1.0.1/tests/test_metrics.py` & `pycanon-1.0.1.post1/tests/test_metrics.py`

 * *Files identical despite different names*

### Comparing `pycanon-1.0.1/tests/test_reports.py` & `pycanon-1.0.1.post1/tests/test_reports.py`

 * *Files identical despite different names*

