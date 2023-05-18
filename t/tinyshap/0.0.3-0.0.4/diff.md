# Comparing `tmp/tinyshap-0.0.3.tar.gz` & `tmp/tinyshap-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\Users\user\Documents\tinyshap\dist\.tmp-jo1bxdz_\tinyshap-0.0.3.tar", last modified: Sat Apr 29 17:29:45 2023, max compression
+gzip compressed data, was "tinyshap-0.0.4.tar", last modified: Thu May 18 16:34:29 2023, max compression
```

## Comparing `tinyshap-0.0.3.tar` & `tinyshap-0.0.4.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-04-29 17:29:45.984774 tinyshap-0.0.3/
--rw-rw-rw-   0        0        0     1089 2023-04-29 16:41:09.000000 tinyshap-0.0.3/LICENCE
--rw-rw-rw-   0        0        0     1995 2023-04-29 17:29:45.983767 tinyshap-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     1094 2023-04-29 17:08:30.000000 tinyshap-0.0.3/README.md
--rw-rw-rw-   0        0        0     1166 2023-04-29 17:29:05.000000 tinyshap-0.0.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-29 17:29:45.985769 tinyshap-0.0.3/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-29 17:29:45.980770 tinyshap-0.0.3/tinyshap.egg-info/
--rw-rw-rw-   0        0        0     1995 2023-04-29 17:29:45.000000 tinyshap-0.0.3/tinyshap.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      191 2023-04-29 17:29:45.000000 tinyshap-0.0.3/tinyshap.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-29 17:29:45.000000 tinyshap-0.0.3/tinyshap.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       34 2023-04-29 17:29:45.000000 tinyshap-0.0.3/tinyshap.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-04-29 17:29:45.000000 tinyshap-0.0.3/tinyshap.egg-info/top_level.txt
+drwxrwxrwx   0 tsitsimis  (1000) tsitsimis  (1000)        0 2023-05-18 16:34:29.147343 tinyshap-0.0.4/
+-rwxrwxrwx   0 tsitsimis  (1000) tsitsimis  (1000)     1089 2023-04-29 16:41:09.000000 tinyshap-0.0.4/LICENCE
+-rwxrwxrwx   0 tsitsimis  (1000) tsitsimis  (1000)     1791 2023-05-18 16:34:29.131340 tinyshap-0.0.4/PKG-INFO
+-rwxrwxrwx   0 tsitsimis  (1000) tsitsimis  (1000)      946 2023-05-18 16:22:52.000000 tinyshap-0.0.4/README.md
+-rwxrwxrwx   0 tsitsimis  (1000) tsitsimis  (1000)     1166 2023-05-18 16:31:44.000000 tinyshap-0.0.4/pyproject.toml
+-rwxrwxrwx   0 tsitsimis  (1000) tsitsimis  (1000)       38 2023-05-18 16:34:29.150351 tinyshap-0.0.4/setup.cfg
+drwxrwxrwx   0 tsitsimis  (1000) tsitsimis  (1000)        0 2023-05-18 16:34:29.056341 tinyshap-0.0.4/tinyshap.egg-info/
+-rwxrwxrwx   0 tsitsimis  (1000) tsitsimis  (1000)     1791 2023-05-18 16:34:28.000000 tinyshap-0.0.4/tinyshap.egg-info/PKG-INFO
+-rwxrwxrwx   0 tsitsimis  (1000) tsitsimis  (1000)      191 2023-05-18 16:34:28.000000 tinyshap-0.0.4/tinyshap.egg-info/SOURCES.txt
+-rwxrwxrwx   0 tsitsimis  (1000) tsitsimis  (1000)        1 2023-05-18 16:34:28.000000 tinyshap-0.0.4/tinyshap.egg-info/dependency_links.txt
+-rwxrwxrwx   0 tsitsimis  (1000) tsitsimis  (1000)       34 2023-05-18 16:34:28.000000 tinyshap-0.0.4/tinyshap.egg-info/requires.txt
+-rwxrwxrwx   0 tsitsimis  (1000) tsitsimis  (1000)        9 2023-05-18 16:34:28.000000 tinyshap-0.0.4/tinyshap.egg-info/top_level.txt
```

### Comparing `tinyshap-0.0.3/LICENCE` & `tinyshap-0.0.4/LICENCE`

 * *Files identical despite different names*

### Comparing `tinyshap-0.0.3/PKG-INFO` & `tinyshap-0.0.4/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,56 +1,54 @@
-Metadata-Version: 2.1
-Name: tinyshap
-Version: 0.0.3
-Summary: Minimal implementation of approximate Kernel SHAP algorithm
-Author-email: Theodore Tsitsimis <th.tsitsimis@gmail.com>
-Project-URL: Homepage, https://github.com/tsitsimis/tinyshap
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENCE
-
-# tinyshap
-![](./assets/demo-dependency-plot.png)
-
-A minimal implementation of the SHAP algorithm using the KernelSHAP method. In less then 100 lines of code, this repo serves as an educational resource to understand how SHAP works without all the complexities of a production-level package.
-
-Note: For reliable and more flexible estimation of SHAP values the user should use [shap](https://github.com/slundberg/shap) or a similar package.
-
-## Installation
-```bash
-pip install tinyshap
-```
-
-## Example usage
-```python
-from tinyshap import SHAPExplainer
-
-# Train model
-model = GradientBoostingRegressor()
-model.fit(X_train, y_train)
-
-# Explain predictions
-explainer = SHAPExplainer(model.predict, X=X_train.mean().to_frame().T)
-contributions = explainer.shap_values(X)
-```
-
-See complete [notebook](./notebooks/demo.ipynb)
-
-## Resources
-* [A Unified Approach to Interpreting Model Predictions (arXiv)](https://arxiv.org/abs/1705.07874)
-* [Interpretable Machine Learning](https://christophm.github.io/interpretable-ml-book/shap.html#kernelshap)
-
-
-## Licence
-MIT
- 
+Metadata-Version: 2.1
+Name: tinyshap
+Version: 0.0.4
+Summary: Minimal implementation of approximate Kernel SHAP algorithm
+Author-email: Theodore Tsitsimis <th.tsitsimis@gmail.com>
+Project-URL: Homepage, https://github.com/tsitsimis/tinyshap
+Classifier: Development Status :: 3 - Alpha
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENCE
+
+# tinyshap
+![](./assets/demo-dependency-plot.png)
+
+A minimal implementation of the SHAP algorithm using the KernelSHAP method. In less then 100 lines of code, this repo serves as an educational resource to understand how SHAP works without all the complexities of a production-level package.
+
+## Installation
+```bash
+pip install tinyshap
+```
+
+## Example usage
+```python
+from tinyshap import SHAPExplainer
+
+# Train model
+model = GradientBoostingRegressor()
+model.fit(X_train, y_train)
+
+# Explain predictions
+explainer = SHAPExplainer(model.predict, X=X_train.mean().to_frame().T)
+contributions = explainer.shap_values(X)
+```
+
+See complete [notebook](./notebooks/demo.ipynb)
+
+## Resources
+* [A Unified Approach to Interpreting Model Predictions (arXiv)](https://arxiv.org/abs/1705.07874)
+* [Interpretable Machine Learning](https://christophm.github.io/interpretable-ml-book/shap.html#kernelshap)
+
+
+## Licence
+MIT
+
```

### Comparing `tinyshap-0.0.3/README.md` & `tinyshap-0.0.4/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 # tinyshap
 ![](./assets/demo-dependency-plot.png)
 
 A minimal implementation of the SHAP algorithm using the KernelSHAP method. In less then 100 lines of code, this repo serves as an educational resource to understand how SHAP works without all the complexities of a production-level package.
 
-Note: For reliable and more flexible estimation of SHAP values the user should use [shap](https://github.com/slundberg/shap) or a similar package.
-
 ## Installation
 ```bash
 pip install tinyshap
 ```
 
 ## Example usage
 ```python
@@ -28,8 +26,8 @@
 ## Resources
 * [A Unified Approach to Interpreting Model Predictions (arXiv)](https://arxiv.org/abs/1705.07874)
 * [Interpretable Machine Learning](https://christophm.github.io/interpretable-ml-book/shap.html#kernelshap)
 
 
 ## Licence
 MIT
- 
+
```

### Comparing `tinyshap-0.0.3/pyproject.toml` & `tinyshap-0.0.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = 'tinyshap'
-version = '0.0.3'
+version = '0.0.4'
 description = 'Minimal implementation of approximate Kernel SHAP algorithm'
 readme = 'README.md'
 authors = [
   { name = 'Theodore Tsitsimis', email='th.tsitsimis@gmail.com' },
 ]
 license = {file = 'LICENSE'}
 requires-python = '>=3.8'
 dependencies = [
-  "pandas>=2.0.0",
-  "scikit-learn>=1.2.2",
+  "pandas>=1.4.0",
+  "scikit-learn>=1.1.1",
 ]
 classifiers = [
     'Development Status :: 3 - Alpha',
     'Intended Audience :: Developers',
     'License :: OSI Approved :: MIT License',
     'Operating System :: OS Independent',
     'Programming Language :: Python',
```

### Comparing `tinyshap-0.0.3/tinyshap.egg-info/PKG-INFO` & `tinyshap-0.0.4/tinyshap.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,56 +1,54 @@
-Metadata-Version: 2.1
-Name: tinyshap
-Version: 0.0.3
-Summary: Minimal implementation of approximate Kernel SHAP algorithm
-Author-email: Theodore Tsitsimis <th.tsitsimis@gmail.com>
-Project-URL: Homepage, https://github.com/tsitsimis/tinyshap
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENCE
-
-# tinyshap
-![](./assets/demo-dependency-plot.png)
-
-A minimal implementation of the SHAP algorithm using the KernelSHAP method. In less then 100 lines of code, this repo serves as an educational resource to understand how SHAP works without all the complexities of a production-level package.
-
-Note: For reliable and more flexible estimation of SHAP values the user should use [shap](https://github.com/slundberg/shap) or a similar package.
-
-## Installation
-```bash
-pip install tinyshap
-```
-
-## Example usage
-```python
-from tinyshap import SHAPExplainer
-
-# Train model
-model = GradientBoostingRegressor()
-model.fit(X_train, y_train)
-
-# Explain predictions
-explainer = SHAPExplainer(model.predict, X=X_train.mean().to_frame().T)
-contributions = explainer.shap_values(X)
-```
-
-See complete [notebook](./notebooks/demo.ipynb)
-
-## Resources
-* [A Unified Approach to Interpreting Model Predictions (arXiv)](https://arxiv.org/abs/1705.07874)
-* [Interpretable Machine Learning](https://christophm.github.io/interpretable-ml-book/shap.html#kernelshap)
-
-
-## Licence
-MIT
- 
+Metadata-Version: 2.1
+Name: tinyshap
+Version: 0.0.4
+Summary: Minimal implementation of approximate Kernel SHAP algorithm
+Author-email: Theodore Tsitsimis <th.tsitsimis@gmail.com>
+Project-URL: Homepage, https://github.com/tsitsimis/tinyshap
+Classifier: Development Status :: 3 - Alpha
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENCE
+
+# tinyshap
+![](./assets/demo-dependency-plot.png)
+
+A minimal implementation of the SHAP algorithm using the KernelSHAP method. In less then 100 lines of code, this repo serves as an educational resource to understand how SHAP works without all the complexities of a production-level package.
+
+## Installation
+```bash
+pip install tinyshap
+```
+
+## Example usage
+```python
+from tinyshap import SHAPExplainer
+
+# Train model
+model = GradientBoostingRegressor()
+model.fit(X_train, y_train)
+
+# Explain predictions
+explainer = SHAPExplainer(model.predict, X=X_train.mean().to_frame().T)
+contributions = explainer.shap_values(X)
+```
+
+See complete [notebook](./notebooks/demo.ipynb)
+
+## Resources
+* [A Unified Approach to Interpreting Model Predictions (arXiv)](https://arxiv.org/abs/1705.07874)
+* [Interpretable Machine Learning](https://christophm.github.io/interpretable-ml-book/shap.html#kernelshap)
+
+
+## Licence
+MIT
+
```

