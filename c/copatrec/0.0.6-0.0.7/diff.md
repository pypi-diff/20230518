# Comparing `tmp/copatrec-0.0.6.tar.gz` & `tmp/copatrec-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "copatrec-0.0.6.tar", last modified: Wed Dec 21 13:22:37 2022, max compression
+gzip compressed data, was "copatrec-0.0.7.tar", last modified: Thu May 18 12:29:54 2023, max compression
```

## Comparing `copatrec-0.0.6.tar` & `copatrec-0.0.7.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxrwx   0        0        0        0 2022-12-21 13:22:37.704784 copatrec-0.0.6/
--rw-rw-rw-   0        0        0    20849 2021-11-08 14:54:14.000000 copatrec-0.0.6/LICENSE
--rw-rw-rw-   0        0        0     2066 2022-12-21 13:22:37.704784 copatrec-0.0.6/PKG-INFO
--rw-rw-rw-   0        0        0     1531 2022-12-21 13:21:31.000000 copatrec-0.0.6/README.md
--rw-rw-rw-   0        0        0      108 2021-09-08 11:27:10.000000 copatrec-0.0.6/pyproject.toml
--rw-rw-rw-   0        0        0       42 2022-12-21 13:22:37.705908 copatrec-0.0.6/setup.cfg
--rw-rw-rw-   0        0        0     1448 2022-12-21 13:18:24.000000 copatrec-0.0.6/setup.py
-drwxrwxrwx   0        0        0        0 2022-12-21 13:22:37.685498 copatrec-0.0.6/src/
-drwxrwxrwx   0        0        0        0 2022-12-21 13:22:37.693824 copatrec-0.0.6/src/copatrec/
--rw-rw-rw-   0        0        0      375 2022-06-27 09:47:10.000000 copatrec-0.0.6/src/copatrec/__init__.py
-drwxrwxrwx   0        0        0        0 2022-12-21 13:22:37.700786 copatrec-0.0.6/src/copatrec/constants/
--rw-rw-rw-   0        0        0      275 2022-06-27 09:38:02.000000 copatrec-0.0.6/src/copatrec/constants/__init__.py
--rw-rw-rw-   0        0        0     3708 2022-10-26 09:16:23.000000 copatrec-0.0.6/src/copatrec/constants/constants.py
--rw-rw-rw-   0        0        0    78615 2022-11-10 12:32:19.000000 copatrec-0.0.6/src/copatrec/copatrec.py
-drwxrwxrwx   0        0        0        0 2022-12-21 13:22:37.701784 copatrec-0.0.6/src/copatrec/math/
--rw-rw-rw-   0        0        0      275 2022-06-27 09:37:47.000000 copatrec-0.0.6/src/copatrec/math/__init__.py
--rw-rw-rw-   0        0        0     6783 2022-08-10 07:34:03.000000 copatrec-0.0.6/src/copatrec/math/patterns.py
-drwxrwxrwx   0        0        0        0 2022-12-21 13:22:37.703784 copatrec-0.0.6/src/copatrec/result/
--rw-rw-rw-   0        0        0      275 2022-06-27 09:37:30.000000 copatrec-0.0.6/src/copatrec/result/__init__.py
--rw-rw-rw-   0        0        0    27306 2022-12-13 10:44:17.000000 copatrec-0.0.6/src/copatrec/result/result.py
-drwxrwxrwx   0        0        0        0 2022-12-21 13:22:37.698784 copatrec-0.0.6/src/copatrec.egg-info/
--rw-rw-rw-   0        0        0     2066 2022-12-21 13:22:37.000000 copatrec-0.0.6/src/copatrec.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      463 2022-12-21 13:22:37.000000 copatrec-0.0.6/src/copatrec.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-12-21 13:22:37.000000 copatrec-0.0.6/src/copatrec.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       38 2022-12-21 13:22:37.000000 copatrec-0.0.6/src/copatrec.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2022-12-21 13:22:37.000000 copatrec-0.0.6/src/copatrec.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-18 12:29:54.627231 copatrec-0.0.7/
+-rw-rw-rw-   0        0        0    20849 2021-11-08 14:54:14.000000 copatrec-0.0.7/LICENSE
+-rw-rw-rw-   0        0        0     2071 2023-05-18 12:29:54.625227 copatrec-0.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0     1536 2023-05-03 09:14:17.000000 copatrec-0.0.7/README.md
+-rw-rw-rw-   0        0        0      108 2021-09-08 11:27:10.000000 copatrec-0.0.7/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-18 12:29:54.627231 copatrec-0.0.7/setup.cfg
+-rw-rw-rw-   0        0        0     1453 2023-05-18 11:50:20.000000 copatrec-0.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-18 12:29:54.603089 copatrec-0.0.7/src/
+drwxrwxrwx   0        0        0        0 2023-05-18 12:29:54.611827 copatrec-0.0.7/src/copatrec/
+-rw-rw-rw-   0        0        0      375 2023-05-18 11:44:27.000000 copatrec-0.0.7/src/copatrec/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-18 12:29:54.618500 copatrec-0.0.7/src/copatrec/constants/
+-rw-rw-rw-   0        0        0      275 2022-06-27 09:38:02.000000 copatrec-0.0.7/src/copatrec/constants/__init__.py
+-rw-rw-rw-   0        0        0     3708 2022-10-26 09:16:23.000000 copatrec-0.0.7/src/copatrec/constants/constants.py
+-rw-rw-rw-   0        0        0    78857 2023-05-18 11:44:00.000000 copatrec-0.0.7/src/copatrec/copatrec.py
+drwxrwxrwx   0        0        0        0 2023-05-18 12:29:54.620523 copatrec-0.0.7/src/copatrec/math/
+-rw-rw-rw-   0        0        0      275 2022-06-27 09:37:47.000000 copatrec-0.0.7/src/copatrec/math/__init__.py
+-rw-rw-rw-   0        0        0     6783 2022-08-10 07:34:03.000000 copatrec-0.0.7/src/copatrec/math/patterns.py
+drwxrwxrwx   0        0        0        0 2023-05-18 12:29:54.624230 copatrec-0.0.7/src/copatrec/result/
+-rw-rw-rw-   0        0        0      275 2022-06-27 09:37:30.000000 copatrec-0.0.7/src/copatrec/result/__init__.py
+-rw-rw-rw-   0        0        0    26752 2023-05-18 11:45:35.000000 copatrec-0.0.7/src/copatrec/result/result.py
+drwxrwxrwx   0        0        0        0 2023-05-18 12:29:54.616680 copatrec-0.0.7/src/copatrec.egg-info/
+-rw-rw-rw-   0        0        0     2071 2023-05-18 12:29:54.000000 copatrec-0.0.7/src/copatrec.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      463 2023-05-18 12:29:54.000000 copatrec-0.0.7/src/copatrec.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-18 12:29:54.000000 copatrec-0.0.7/src/copatrec.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       43 2023-05-18 12:29:54.000000 copatrec-0.0.7/src/copatrec.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-05-18 12:29:54.000000 copatrec-0.0.7/src/copatrec.egg-info/top_level.txt
```

### Comparing `copatrec-0.0.6/LICENSE` & `copatrec-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `copatrec-0.0.6/PKG-INFO` & `copatrec-0.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: copatrec
-Version: 0.0.6
+Version: 0.0.7
 Summary: Correlation pattern recognizer (Copatrec), a package to find nonlinear patterns (regressions) using Machine Learning.
 Author: Siamak Khatami
 Author-email: <siamak.khatami@ntnu.no>
 Classifier: Programming Language :: Python :: 3.6
 Classifier: License :: Free for non-commercial use
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
@@ -36,15 +36,15 @@
 If the package is installed from GitHub, then it would be suggested
 to install the following packages (dependencies) in your system using `pip` or any other 
 preferred approaches. 
 - matplotlib
 - NumPy
 - pandas
 - scipy
-- sklearn
+- scikit-learn
 
 ## Web application (On progress)
 www.copatrec.org
 
 # Examples
 
 The "examples" folder can be found under the GitHub repo. Its direct URL is:
```

### Comparing `copatrec-0.0.6/README.md` & `copatrec-0.0.7/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 If the package is installed from GitHub, then it would be suggested
 to install the following packages (dependencies) in your system using `pip` or any other 
 preferred approaches. 
 - matplotlib
 - NumPy
 - pandas
 - scipy
-- sklearn
+- scikit-learn
 
 ## Web application (On progress)
 www.copatrec.org
 
 # Examples
 
 The "examples" folder can be found under the GitHub repo. Its direct URL is:
```

### Comparing `copatrec-0.0.6/setup.py` & `copatrec-0.0.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,25 +18,25 @@
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
 setuptools.setup(
     name="copatrec",
-    version="0.0.6",
+    version="0.0.7",
     author="Siamak Khatami",
     author_email="<siamak.khatami@ntnu.no>",
     description="Correlation pattern recognizer (Copatrec), a package to find "
                 "nonlinear patterns (regressions) using Machine Learning.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     install_requires=['pandas',
                       'numpy',
                       'matplotlib',
-                      'sklearn',
+                      'scikit-learn',
                       'scipy'],
     classifiers=[
         "Programming Language :: Python :: 3.6",
         "License :: Free for non-commercial use",
         "Operating System :: OS Independent",
     ],
     package_dir={"": "src"},
```

### Comparing `copatrec-0.0.6/src/copatrec/constants/constants.py` & `copatrec-0.0.7/src/copatrec/constants/constants.py`

 * *Files identical despite different names*

### Comparing `copatrec-0.0.6/src/copatrec/copatrec.py` & `copatrec-0.0.7/src/copatrec/copatrec.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,29 +29,33 @@
     from src.constants.constants import CST, Warns, Errs
 except ImportError:
     #  If package is installed
     from copatrec.math.patterns import _EquFuncs, _EquPatterns
     from copatrec.result.result import Result
     from copatrec.constants.constants import CST, Warns, Errs
 
+
 class Copatrec:
     def __init__(self,
                  data: pd.DataFrame,
                  dependent_var: str,
+                 independent_vars: list = [],
                  time_col: str = "",
                  category_col: str = "",
                  report: bool = True,
                  report_to_file: bool = False
                  ):
         """
         COPATREC initializer function
         :param data:
         :type: pd.DataFrame
         :param dependent_var: The column name in the dataframe which represents dependent variable.
         :type: str
+        :param independent_vars: The column names in the dataframe which represents independent variables.
+        :type: list[str]
         :param time_col:  The column name in the dataframe which represents time information.
         :type: str
         :param category_col: The column name in the dataframe which represents categories names.
         :type: str
         :param report: whether to report the process or not.
         :type: bool
         :param report_to_file: Whether to print report into a file (True) or in the Terminal(False)
@@ -78,31 +82,33 @@
                        _EquFuncs.oscillating_growth,
                        _EquFuncs.double_gaussian
                        ]
 
         self.Data = data
         self.Time_col = time_col
         self.Category_col = category_col
+        self.Independent_vars = independent_vars
 
         if not self.Category_col:  # A column name is added if there is no col
             # the default category name
             self.Category_col = CST.Cat.format(''.join(rnd.sample(string.ascii_lowercase, 5)))
             self.Data[self.Category_col] = 1  # the default value
         if not self.Time_col:  # A time name is added if there is no time col
             self.Time_col = CST.Time.format(''.join(rnd.sample(string.ascii_lowercase, 5)))  # Default time col name
             self.Data[self.Time_col] = 1  # Default value for the col
             #  for col in data[self.Category_col]:
             #       self.Data[self.Time_col].at[self.Data[self.Category_col] == col] = list(
             #       range(self.Data[self.Time_col].at[self.Data[self.Category_col] == col].shape[0]))
         self.Dependent_var = dependent_var
-        self.Independent_var = [var for var in self.Data.columns if var not in [
-            self.Time_col,
-            self.Category_col,
-            self.Dependent_var
-        ]]  # All columns excepts dependent variable, time and category columns are counted as independent variable.
+        if not self.Independent_vars:  # If there is no column specified, then loop over all remaining columns.
+            self.Independent_vars = [var for var in self.Data.columns if var not in [
+                self.Time_col,
+                self.Category_col,
+                self.Dependent_var
+            ]]  # All columns excepts dependent variable, time and category columns are counted as independent variable.
         self.__fix_data_types()  # Reformat data in the dataset.
         if report:
             args = {
                 'level': lg.INFO,
                 'format': '%(levelname)s - %(message)s',
                 'filemode': 'w'
             }
@@ -558,15 +564,15 @@
         lg.warning(Warns.W101)
         dict_intervals = {}  # dict[var] = dict[cat]
         dict_standard_values = {}  # dict[var] = dict[cat]
         dict_outliers = {}  # dict[var] = dict[cat]
         grouped_data_by_cat_col = self.Data.groupby([self.Category_col])
         # Creating grouped dataframes based on the categories presented in the Dataframe.
 
-        for var in [self.Dependent_var] + self.Independent_var:
+        for var in [self.Dependent_var] + self.Independent_vars:
             lg.info('variable {} started.'.format(var).ljust(20, '-'))
             this_var_dict_intervals = {}  # dict[cat] = tuple(lower band , upper band)
             this_var_dict_standard_values = {}  # dict[cat] = values
             this_var_dict_outliers = {}  # dict[cat] = tuple(based on lower band, based on upper band)
             for cat, cat_dt in grouped_data_by_cat_col:  # Iterating over grouped data set
                 this_cat_this_var_data = cat_dt[var]
                 this_cat_category_names = cat_dt[self.Time_col].values
@@ -608,15 +614,15 @@
                     lg.error(Errs.E207.format(var, cat, CST.ALL))  # All rows are empty
 
             dict_intervals[var] = this_var_dict_intervals
             dict_standard_values[var] = this_var_dict_standard_values
             dict_outliers[var] = this_var_dict_outliers
             lg.info('variable {} done.'.format(var).ljust(20, '-'))
         if plot_pairs:
-            for x_var in self.Independent_var:
+            for x_var in self.Independent_vars:
                 for cat, cat_dt in grouped_data_by_cat_col:
                     x_unique_values = list(set(pd.Series(dict_standard_values[x_var][cat])))
                     # in Numpy np.nan == np.nan returns false. Which means, it can't aggregate nan values.
                     # Considering that characteristic, set and list is used to get the unique values.
                     # An easy way to get unique values from the series
                     y_unique_values = list(set(pd.Series(dict_standard_values[self.Dependent_var][cat])))
                     if (not (x_unique_values == [0] or x_unique_values == [])) and \
@@ -670,15 +676,15 @@
         lg.info(Warns.P101.format(CST.Cross_Sectional, method).center(40, '*'))
         lg.warning(Warns.W101)
         dict_intervals = {}  # dict[var] = dict[time]
         dict_standard_values = {}  # dict[var] = dict[time]
         dict_outliers = {}  # dict[var] = dict[time]
         grouped_data_by_time_col = self.Data.groupby([self.Time_col])
 
-        for var in [self.Dependent_var] + self.Independent_var:
+        for var in [self.Dependent_var] + self.Independent_vars:
             lg.info('variable {} started.'.format(var).ljust(20, '-'))
             this_var_dict_intervals = {}  # dict[time]
             this_var_dict_standard_values = {}  # dict[time]
             this_var_dict_outliers = {}  # dict[time]
             for time, time_dt in grouped_data_by_time_col:  # Iterating over grouped data set
                 this_time_this_var_data = time_dt[var]
                 this_time_category_names = time_dt[self.Category_col].values
@@ -717,15 +723,15 @@
 
             dict_intervals[var] = this_var_dict_intervals
             dict_standard_values[var] = this_var_dict_standard_values
             dict_outliers[var] = this_var_dict_outliers
             lg.info('variable {} done.'.format(var).ljust(20, '-'))
         if plot_pairs:
 
-            for x_var in self.Independent_var:
+            for x_var in self.Independent_vars:
                 for time, time_dt in grouped_data_by_time_col:
                     #  this_time_category_names = time_dt[self.Category_col].values  # Can be accessed form index
                     x_unique_values = list(set(pd.Series(dict_standard_values[x_var][time])))
                     y_unique_values = list(set(pd.Series(dict_standard_values[self.Dependent_var][time])))
                     if (not (x_unique_values == [0] or x_unique_values == [])) and \
                             (not (y_unique_values == [0] or y_unique_values == [])):
                         self.__plot_intervals(CST.Cross_Sectional,
@@ -781,15 +787,15 @@
         dict_standard_values = {}
         dict_outliers = {}
 
         # Grouping data based on the categories to access better
         grouped_data_by_category_col = self.Data.groupby([self.Category_col])
         list_category_names = grouped_data_by_category_col[
             self.Dependent_var].describe().index.values  # getting all category names
-        for var in [self.Dependent_var] + self.Independent_var:
+        for var in [self.Dependent_var] + self.Independent_vars:
             lg.info('variable {} started.'.format(var).ljust(20, '-'))
             this_var_data, _ = self.__calc_mean_std(
                 grouped_data_by_category_col[var])  # mean of categories are used to establish the intervals
 
             var_unique_values = list(set(this_var_data.value_counts().index))
             # This code drops nan values as well, so it is used instead of
             # list(set(this_var_data))
@@ -819,15 +825,15 @@
             else:
                 dict_intervals[var] = (np.nan, np.nan)
                 dict_standard_values[var] = np.array([])
                 dict_outliers[var] = []
                 lg.error(Errs.E207.format(var, CST.ALL, CST.ALL))  # All rows are empty
             lg.info('variable {} done.'.format(var).ljust(20, '-'))
         if plot_pairs:
-            for x_var in self.Independent_var:
+            for x_var in self.Independent_vars:
                 x_unique_values = list(set(pd.Series(dict_standard_values[x_var])))
                 y_unique_values = list(set(pd.Series(dict_standard_values[self.Dependent_var])))
                 if (not (x_unique_values == [0] or x_unique_values == [])) and \
                         (not (y_unique_values == [0] or y_unique_values == [])):
                     self.__plot_intervals(CST.Panel,
                                           x_var,
                                           dict_standard_values[x_var],
@@ -896,15 +902,15 @@
         intervals, outliers, current_outliers = None, None, None  # Initialization, To prevent linting error
         if drop_outliers:
             # collect all intervals and outliers if drop_outliers is True
             intervals, outliers = self.time_series_outliers(method=outlier_method,
                                                             plot_pairs=False,
                                                             plot_hists=False)
 
-        for independent_var in self.Independent_var:
+        for independent_var in self.Independent_vars:
             lg.info(
                 "X: {}, Y: {}".format(
                     self.Dependent_var,
                     independent_var).center(40, "="))
             # Selecting data for the current specific independent and dependent variable
             this_independent_dt = self.Data[[self.Time_col, self.Category_col,
                                              self.Dependent_var, independent_var]]
@@ -1047,15 +1053,15 @@
         error_terms = dict()  # This holds all error terms relevant to the fitting process.
         # dict[independent variable][time][equation form]
         intervals, outliers, current_outliers = None, None, None
         if drop_outliers:
             intervals, outliers = self.cross_sectional_outliers(method=outlier_method,
                                                                 plot_pairs=False,
                                                                 plot_hists=False)
-        for independent_var in self.Independent_var:
+        for independent_var in self.Independent_vars:
             lg.info("X: {}, Y: {}".format(self.Dependent_var,
                                           independent_var).center(40, "="))
             # Selecting data for the current specific independent and dependent variable
             this_independent_dt = self.Data[[self.Time_col,
                                              self.Category_col,
                                              self.Dependent_var,
                                              independent_var]]
@@ -1188,15 +1194,15 @@
         all_forms_dict = dict()  # all_forms_dict[independent variable][equation forms]
         error_terms = dict()  # error_terms[independent variable][equation form]
         intervals, outliers, current_outliers = None, None, None
         if drop_outliers:
             intervals, outliers = self.panel_outliers(method=outlier_method,
                                                       plot_pairs=False,
                                                       plot_hists=False)
-        for independent_var in self.Independent_var:
+        for independent_var in self.Independent_vars:
             results = dict()  # Initiating the results[equation form]
             errs = dict()  # errs[equation forms]
 
             this_independent_dt = self.Data[[self.Time_col,
                                              self.Category_col,
                                              self.Dependent_var,
                                              independent_var]]
@@ -1402,10 +1408,7 @@
                         np.array(d[col].values).reshape(-1, 1)) + 1e-5
                     #  To prevent data from catch in 0 errors in fitting process, an epsilon is added.
             d = d.dropna()
             if d.empty:
                 lg.error(Errs.E203)
             return d
 
-# TODO 3: Save standardized data in the data set and retrieve from there. Just do standardization if it is not in the
-# data set.
-
```

### Comparing `copatrec-0.0.6/src/copatrec/math/patterns.py` & `copatrec-0.0.7/src/copatrec/math/patterns.py`

 * *Files identical despite different names*

### Comparing `copatrec-0.0.6/src/copatrec/result/result.py` & `copatrec-0.0.7/src/copatrec/result/result.py`

 * *Files 2% similar despite different names*

```diff
@@ -122,19 +122,14 @@
         :param outlier_method: Which method used to find outliers
         :param outliers: The dict of outliers
         :param intervals: The dict of intervals
         :param alpha: Significant level
         :param cross_section_time: The list of times related to the cross_sectional study
         :param time_series_category: The list of categories related to the time_series study
         """
-        # TODO (Function Domain and Range Report): Is the equation validated if yes (what are domains and ranges)
-        #  if no, is it verified (for example for GDPPC you can use GDP/population and this makes sense), but for
-        #  the GDP's equation, you can't say it comes from sky, and if you are using other resources, you may report
-        #  its domain, range and error?
-        #
         self.Data = data
         self.Reg_Type = reg_type
         self.Independent_Var = independent_var
         self.Dependent_Var = dependent_var
         self.Func = func
         self.Func_name = func.__name__  # the name of function in the patterns file
         y_values = self.Data[self.Dependent_Var]
@@ -453,16 +448,14 @@
 
     def plot(self,
              show_time_label: bool = False,
              show_category_label: bool = False,
              show_outliers: bool = False,
              plot_predicted_outliers: bool = False):
         """
-        TODO: Parametrize figure size
-        TODO: New Feature: plot time_series or cross_sectional beside panel plot to show bigger and smaller scale
         This function plots the result of analysis using the result object;
         :param show_time_label: Weather to show the labels of the times on the plot
         Only works if the regression type is panel or time_series
         :param show_category_label: Weather to show the labels of the categories on the plot
         Only works if the regression type is panel or cross_sectional
         :param show_outliers: Weather to plot outliers' points or not. Color would be cyan
         :param plot_predicted_outliers: Weather to plot predicted values related to the outliers or not
```

### Comparing `copatrec-0.0.6/src/copatrec.egg-info/PKG-INFO` & `copatrec-0.0.7/src/copatrec.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: copatrec
-Version: 0.0.6
+Version: 0.0.7
 Summary: Correlation pattern recognizer (Copatrec), a package to find nonlinear patterns (regressions) using Machine Learning.
 Author: Siamak Khatami
 Author-email: <siamak.khatami@ntnu.no>
 Classifier: Programming Language :: Python :: 3.6
 Classifier: License :: Free for non-commercial use
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
@@ -36,15 +36,15 @@
 If the package is installed from GitHub, then it would be suggested
 to install the following packages (dependencies) in your system using `pip` or any other 
 preferred approaches. 
 - matplotlib
 - NumPy
 - pandas
 - scipy
-- sklearn
+- scikit-learn
 
 ## Web application (On progress)
 www.copatrec.org
 
 # Examples
 
 The "examples" folder can be found under the GitHub repo. Its direct URL is:
```

