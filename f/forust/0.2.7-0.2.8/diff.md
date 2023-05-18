# Comparing `tmp/forust-0.2.7.tar.gz` & `tmp/forust-0.2.8.tar.gz`

## Comparing `forust-0.2.7.tar` & `forust-0.2.8.tar`

### file list

```diff
@@ -1,44 +1,44 @@
--rw-r--r--   0        0        0      745 1970-01-01 00:00:00.000000 forust-0.2.7/local_dependencies/forust-ml/Cargo.toml
--rw-r--r--   0      501       20     5608 2023-05-15 13:45:36.000000 forust-0.2.7/local_dependencies/forust-ml/.github/workflows/CI.yml
--rw-r--r--   0      501       20      262 2023-05-15 13:45:36.000000 forust-0.2.7/local_dependencies/forust-ml/.gitignore
--rw-r--r--   0      501       20      320 2023-05-15 13:45:36.000000 forust-0.2.7/local_dependencies/forust-ml/.pre-commit-config.yaml
--rw-r--r--   0      501       20     3242 2023-05-15 13:45:36.000000 forust-0.2.7/local_dependencies/forust-ml/CONTRIBUTING.md
--rw-r--r--   0      501       20    11341 2023-05-15 13:45:36.000000 forust-0.2.7/local_dependencies/forust-ml/LICENSE
--rw-r--r--   0      501       20    15307 2023-05-15 13:45:36.000000 forust-0.2.7/local_dependencies/forust-ml/README.md
--rw-r--r--   0      501       20     4228 2023-05-15 13:45:36.000000 forust-0.2.7/local_dependencies/forust-ml/benches/forust_benchmarks.rs
--rw-r--r--   0      501       20   449752 2023-05-15 13:50:45.000000 forust-0.2.7/local_dependencies/forust-ml/dist/forust-0.2.7-cp311-cp311-macosx_10_7_x86_64.whl
--rw-r--r--   0      501       20   763229 2023-05-15 13:49:15.000000 forust-0.2.7/local_dependencies/forust-ml/dist/forust-0.2.7.tar.gz
--rw-r--r--   0      501       20    16121 2023-05-15 13:45:36.000000 forust-0.2.7/local_dependencies/forust-ml/resources/pdp_plot_age.png
--rw-r--r--   0      501       20    10758 2023-05-15 13:45:36.000000 forust-0.2.7/local_dependencies/forust-ml/resources/pdp_plot_age_mono.png
--rw-r--r--   0      501       20    57018 2023-05-15 13:45:36.000000 forust-0.2.7/local_dependencies/forust-ml/resources/titanic.csv
--rw-r--r--   0      501       20   655700 2023-05-15 13:45:36.000000 forust-0.2.7/local_dependencies/forust-ml/resources/tree-image-crop.png
--rw-r--r--   0      501       20     2556 2023-05-15 13:45:36.000000 forust-0.2.7/local_dependencies/forust-ml/rs-example.md
--rw-r--r--   0      501       20     1179 2023-05-15 13:45:36.000000 forust-0.2.7/local_dependencies/forust-ml/scripts/make_resources.py
--rw-r--r--   0      501       20       53 2023-05-15 13:45:36.000000 forust-0.2.7/local_dependencies/forust-ml/scripts/run-python-tests.ps1
--rw-r--r--   0      501       20       53 2023-05-15 13:45:36.000000 forust-0.2.7/local_dependencies/forust-ml/scripts/run-python-tests.sh
--rw-r--r--   0      501       20     5610 2023-05-15 13:45:36.000000 forust-0.2.7/local_dependencies/forust-ml/src/binning.rs
--rw-r--r--   0      501       20      248 2023-05-15 13:45:36.000000 forust-0.2.7/local_dependencies/forust-ml/src/constraints.rs
--rw-r--r--   0      501       20     9944 2023-05-15 13:45:36.000000 forust-0.2.7/local_dependencies/forust-ml/src/data.rs
--rw-r--r--   0      501       20      562 2023-05-15 13:45:36.000000 forust-0.2.7/local_dependencies/forust-ml/src/errors.rs
--rw-r--r--   0      501       20    35446 2023-05-15 13:45:36.000000 forust-0.2.7/local_dependencies/forust-ml/src/gradientbooster.rs
--rw-r--r--   0      501       20     9357 2023-05-15 13:45:36.000000 forust-0.2.7/local_dependencies/forust-ml/src/histogram.rs
--rw-r--r--   0      501       20      355 2023-05-15 13:45:36.000000 forust-0.2.7/local_dependencies/forust-ml/src/lib.rs
--rw-r--r--   0      501       20     8847 2023-05-15 13:45:36.000000 forust-0.2.7/local_dependencies/forust-ml/src/metric.rs
--rw-r--r--   0      501       20     6060 2023-05-15 13:45:36.000000 forust-0.2.7/local_dependencies/forust-ml/src/node.rs
--rw-r--r--   0      501       20     4868 2023-05-15 13:45:36.000000 forust-0.2.7/local_dependencies/forust-ml/src/objective.rs
--rw-r--r--   0      501       20     4018 2023-05-15 13:45:36.000000 forust-0.2.7/local_dependencies/forust-ml/src/partial_dependence.rs
--rw-r--r--   0      501       20     2276 2023-05-15 13:45:36.000000 forust-0.2.7/local_dependencies/forust-ml/src/sampler.rs
--rw-r--r--   0      501       20    34685 2023-05-15 13:45:36.000000 forust-0.2.7/local_dependencies/forust-ml/src/splitter.rs
--rw-r--r--   0      501       20    21677 2023-05-15 13:45:36.000000 forust-0.2.7/local_dependencies/forust-ml/src/tree.rs
--rw-r--r--   0      501       20    29701 2023-05-15 13:45:36.000000 forust-0.2.7/local_dependencies/forust-ml/src/utils.rs
--rw-r--r--   0        0        0      391 1970-01-01 00:00:00.000000 forust-0.2.7/Cargo.toml
--rw-r--r--   0      501       20      685 2023-05-15 13:45:36.000000 forust-0.2.7/.gitignore
--rw-r--r--   0      501       20    15307 2023-05-15 13:46:19.000000 forust-0.2.7/README.md
--rw-r--r--   0      501       20    26798 2023-05-15 13:45:36.000000 forust-0.2.7/forust/__init__.py
--rw-r--r--   0      501       20      785 2023-05-15 13:45:36.000000 forust-0.2.7/pyproject.toml
--rw-r--r--   0      501       20     7353 2023-05-15 13:45:36.000000 forust-0.2.7/scratch.py
--rw-r--r--   0      501       20    12675 2023-05-15 13:45:36.000000 forust-0.2.7/src/lib.rs
--rw-r--r--   0      501       20    14397 2023-05-15 13:45:36.000000 forust-0.2.7/tests/test_booster.py
--rw-r--r--   0      501       20    11341 2023-05-15 13:46:19.000000 forust-0.2.7/LICENSE
--rw-r--r--   0      501       20    15307 2023-05-15 13:46:19.000000 forust-0.2.7/README.md
--rw-r--r--   0        0        0    16091 1970-01-01 00:00:00.000000 forust-0.2.7/PKG-INFO
+-rw-r--r--   0        0        0      745 1970-01-01 00:00:00.000000 forust-0.2.8/local_dependencies/forust-ml/Cargo.toml
+-rw-r--r--   0      501       20     5608 2023-05-18 18:47:19.000000 forust-0.2.8/local_dependencies/forust-ml/.github/workflows/CI.yml
+-rw-r--r--   0      501       20      268 2023-05-18 18:47:19.000000 forust-0.2.8/local_dependencies/forust-ml/.gitignore
+-rw-r--r--   0      501       20      320 2023-05-18 18:47:19.000000 forust-0.2.8/local_dependencies/forust-ml/.pre-commit-config.yaml
+-rw-r--r--   0      501       20     3242 2023-05-18 18:47:19.000000 forust-0.2.8/local_dependencies/forust-ml/CONTRIBUTING.md
+-rw-r--r--   0      501       20    11341 2023-05-18 18:47:19.000000 forust-0.2.8/local_dependencies/forust-ml/LICENSE
+-rw-r--r--   0      501       20    15541 2023-05-18 18:47:19.000000 forust-0.2.8/local_dependencies/forust-ml/README.md
+-rw-r--r--   0      501       20     4228 2023-05-18 18:47:19.000000 forust-0.2.8/local_dependencies/forust-ml/benches/forust_benchmarks.rs
+-rw-r--r--   0      501       20   452243 2023-05-18 18:52:22.000000 forust-0.2.8/local_dependencies/forust-ml/dist/forust-0.2.8-cp39-cp39-macosx_10_7_x86_64.whl
+-rw-r--r--   0      501       20   764121 2023-05-18 18:51:20.000000 forust-0.2.8/local_dependencies/forust-ml/dist/forust-0.2.8.tar.gz
+-rw-r--r--   0      501       20    16121 2023-05-18 18:47:19.000000 forust-0.2.8/local_dependencies/forust-ml/resources/pdp_plot_age.png
+-rw-r--r--   0      501       20    10758 2023-05-18 18:47:19.000000 forust-0.2.8/local_dependencies/forust-ml/resources/pdp_plot_age_mono.png
+-rw-r--r--   0      501       20    57018 2023-05-18 18:47:19.000000 forust-0.2.8/local_dependencies/forust-ml/resources/titanic.csv
+-rw-r--r--   0      501       20   655700 2023-05-18 18:47:19.000000 forust-0.2.8/local_dependencies/forust-ml/resources/tree-image-crop.png
+-rw-r--r--   0      501       20     2556 2023-05-18 18:47:19.000000 forust-0.2.8/local_dependencies/forust-ml/rs-example.md
+-rw-r--r--   0      501       20     1179 2023-05-18 18:47:19.000000 forust-0.2.8/local_dependencies/forust-ml/scripts/make_resources.py
+-rw-r--r--   0      501       20       53 2023-05-18 18:47:19.000000 forust-0.2.8/local_dependencies/forust-ml/scripts/run-python-tests.ps1
+-rw-r--r--   0      501       20       53 2023-05-18 18:47:19.000000 forust-0.2.8/local_dependencies/forust-ml/scripts/run-python-tests.sh
+-rw-r--r--   0      501       20     5610 2023-05-18 18:47:19.000000 forust-0.2.8/local_dependencies/forust-ml/src/binning.rs
+-rw-r--r--   0      501       20      248 2023-05-18 18:47:19.000000 forust-0.2.8/local_dependencies/forust-ml/src/constraints.rs
+-rw-r--r--   0      501       20     9944 2023-05-18 18:47:19.000000 forust-0.2.8/local_dependencies/forust-ml/src/data.rs
+-rw-r--r--   0      501       20      562 2023-05-18 18:47:19.000000 forust-0.2.8/local_dependencies/forust-ml/src/errors.rs
+-rw-r--r--   0      501       20    36231 2023-05-18 18:47:19.000000 forust-0.2.8/local_dependencies/forust-ml/src/gradientbooster.rs
+-rw-r--r--   0      501       20     9357 2023-05-18 18:47:19.000000 forust-0.2.8/local_dependencies/forust-ml/src/histogram.rs
+-rw-r--r--   0      501       20      355 2023-05-18 18:47:19.000000 forust-0.2.8/local_dependencies/forust-ml/src/lib.rs
+-rw-r--r--   0      501       20     8847 2023-05-18 18:47:19.000000 forust-0.2.8/local_dependencies/forust-ml/src/metric.rs
+-rw-r--r--   0      501       20     6060 2023-05-18 18:47:19.000000 forust-0.2.8/local_dependencies/forust-ml/src/node.rs
+-rw-r--r--   0      501       20     4868 2023-05-18 18:47:19.000000 forust-0.2.8/local_dependencies/forust-ml/src/objective.rs
+-rw-r--r--   0      501       20     4018 2023-05-18 18:47:19.000000 forust-0.2.8/local_dependencies/forust-ml/src/partial_dependence.rs
+-rw-r--r--   0      501       20     3458 2023-05-18 18:47:19.000000 forust-0.2.8/local_dependencies/forust-ml/src/sampler.rs
+-rw-r--r--   0      501       20    34995 2023-05-18 18:47:19.000000 forust-0.2.8/local_dependencies/forust-ml/src/splitter.rs
+-rw-r--r--   0      501       20    21713 2023-05-18 18:47:19.000000 forust-0.2.8/local_dependencies/forust-ml/src/tree.rs
+-rw-r--r--   0      501       20    29703 2023-05-18 18:47:19.000000 forust-0.2.8/local_dependencies/forust-ml/src/utils.rs
+-rw-r--r--   0        0        0      391 1970-01-01 00:00:00.000000 forust-0.2.8/Cargo.toml
+-rw-r--r--   0      501       20      685 2023-05-18 18:47:19.000000 forust-0.2.8/.gitignore
+-rw-r--r--   0      501       20    15541 2023-05-18 18:48:09.000000 forust-0.2.8/README.md
+-rw-r--r--   0      501       20    27199 2023-05-18 18:47:19.000000 forust-0.2.8/forust/__init__.py
+-rw-r--r--   0      501       20      785 2023-05-18 18:47:19.000000 forust-0.2.8/pyproject.toml
+-rw-r--r--   0      501       20     7353 2023-05-18 18:47:19.000000 forust-0.2.8/scratch.py
+-rw-r--r--   0      501       20    12899 2023-05-18 18:47:19.000000 forust-0.2.8/src/lib.rs
+-rw-r--r--   0      501       20    14838 2023-05-18 18:47:19.000000 forust-0.2.8/tests/test_booster.py
+-rw-r--r--   0      501       20    11341 2023-05-18 18:48:09.000000 forust-0.2.8/LICENSE
+-rw-r--r--   0      501       20    15541 2023-05-18 18:48:09.000000 forust-0.2.8/README.md
+-rw-r--r--   0        0        0    16325 1970-01-01 00:00:00.000000 forust-0.2.8/PKG-INFO
```

### Comparing `forust-0.2.7/local_dependencies/forust-ml/Cargo.toml` & `forust-0.2.8/local_dependencies/forust-ml/Cargo.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "forust-ml"
-version = "0.2.7"
+version = "0.2.8"
 edition = "2021"
 authors = ["James Inlow <james.d.inlow@gmail.com>"]
 homepage = "https://github.com/jinlow/forust"
 description = "A lightweight gradient boosting implementation in Rust."
 license-file = "LICENSE"
 readme = "README.md"
 repository = "https://github.com/jinlow/forust"
```

### Comparing `forust-0.2.7/local_dependencies/forust-ml/.github/workflows/CI.yml` & `forust-0.2.8/local_dependencies/forust-ml/.github/workflows/CI.yml`

 * *Files identical despite different names*

### Comparing `forust-0.2.7/local_dependencies/forust-ml/CONTRIBUTING.md` & `forust-0.2.8/local_dependencies/forust-ml/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `forust-0.2.7/local_dependencies/forust-ml/LICENSE` & `forust-0.2.8/local_dependencies/forust-ml/LICENSE`

 * *Files identical despite different names*

### Comparing `forust-0.2.7/local_dependencies/forust-ml/README.md` & `forust-0.2.8/local_dependencies/forust-ml/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 The package can be installed directly from [pypi](https://pypi.org/project/forust/).
 ```shell
 pip install forust
 ```
 
 To use in a rust project add the following to your Cargo.toml file.
 ```toml
-forust-ml = "0.2.7"
+forust-ml = "0.2.8"
 ```
 
 ## Usage
 The `GradientBooster` class is currently the only public facing class in the package, and can be used to train gradient boosted decision tree ensembles with multiple objective functions.
 
 It can be initialized with the following arguments.
 
@@ -60,14 +60,16 @@
     will be used. Defaults to 256.
  - `parallel` ***(bool, optional)***: Should multiple cores be used when training and predicting
     with this model? Defaults to `True`.
  - `allow_missing_splits` ***(bool, optional)***: Allow for splits to be made such that all missing values go down one branch, and all non-missing values go down the other, if this results in the greatest reduction of loss. If this is false, splits will only be made on non missing values. If `create_missing_branch` is set to `True` having this parameter be set to `True` will result in the missing branch further split, if this parameter is `False` then in that case the missing branch will always be a terminal node. Defaults to `True`.
  - `monotone_constraints` ***(dict[Any, int], optional)***: Constraints that are used to enforce a specific relationship between the training features and the target variable. A dictionary should be provided where the keys are the feature index value if the model will be fit on a numpy array, or a feature name if it will be fit on a pandas Dataframe. The values of the dictionary should be an integer value of -1, 1, or 0 to specify the relationship that should be estimated between the respective feature and the target variable. Use a value of -1 to enforce a negative relationship, 1 a positive relationship, and 0 will enforce no specific relationship at all. Features not included in the mapping will not have any constraint applied. If `None` is passed no constraints will be enforced on any variable.  Defaults to `None`.
  - `subsample` ***(float, optional)***: Percent of records to randomly sample at each iteration when
       training a tree. Defaults to 1.0, meaning all data is used for training.
+ - `top_rate` ***(float, optional)***: Used only in goss. The retain ratio of large gradient data. Defaults to 0.1.
+ - `other_rate` ***(float, optional)***: Used only in goss. the retain ratio of small gradient data. Defaults to 0.2.
  - `seed` ***(integer, optional)***: Integer value used to seed any randomness used in the
       algorithm. Defaults to 0.
  - `missing` ***(float, optional)***: Value to consider missing, when training and predicting with the booster. Defaults to `np.nan`.
  - `create_missing_branch` ***(bool, optional)***: An experimental parameter, that if `True`, will create a separate branch for missing, creating a ternary tree, the missing node will be given the same weight value as the parent node. If this parameter is `False`, missing will be sent down either the left or right branch, creating a binary tree. Defaults to `False`.
  - `sample_method` ***(str | None, optional)***: Optional string value to use to determine the method to use to sample the data while training. If this is None, no sample method will be used. If the `subsample` parameter is less than 1 and no sample_method is provided this `sample_method` will be automatically set to "random". Valid options are "goss" and "random". Defaults to `None`.
  - `evaluation_metric` ***(str | None, optional)***: Optional string value used to define an evaluation metric that will be calculated at each iteration if a `evaluation_dataset` is provided at fit time. The metric can be one of "AUC", "LogLoss", "RootMeanSquaredLogError", or "RootMeanSquaredError". If no `evaluation_metric` is passed, but an `evaluation_dataset` is passed, then "LogLoss", will be used with the "LogLoss" objective function, and "RootMeanSquaredLogError" will be used with "SquaredLoss".
  - `early_stopping_rounds` ***(int | None, optional)***: If this is specified, and an `evaluation_dataset` is passed during fit, then an improvement in the `evaluation_metric` must be seen after at least this many iterations of training, otherwise training will be cut short.
```

#### html2text {}

```diff
@@ -13,15 +13,15 @@
 understand the XGBoost algorithm, additionally to have a fun project to work on
 in rust, and because I wanted to be able to experiment with adding new features
 to the algorithm in a smaller simpler codebase. All of the rust code for the
 package can be found in the [src](src/) directory, while all of the python
 wrapper code is in the [py-forust](py-forust/) directory. ## Installation The
 package can be installed directly from [pypi](https://pypi.org/project/forust/
 ). ```shell pip install forust ``` To use in a rust project add the following
-to your Cargo.toml file. ```toml forust-ml = "0.2.7" ``` ## Usage The
+to your Cargo.toml file. ```toml forust-ml = "0.2.8" ``` ## Usage The
 `GradientBooster` class is currently the only public facing class in the
 package, and can be used to train gradient boosted decision tree ensembles with
 multiple objective functions. It can be initialized with the following
 arguments. - `objective_type` ***(str, optional)***: The name of objective
 function used to optimize. Valid options include "LogLoss" to use logistic loss
 as the objective function (binary classification), or "SquaredLoss" to use
 Squared Error as the objective function (continuous regression). Defaults to
@@ -62,14 +62,17 @@
 estimated between the respective feature and the target variable. Use a value
 of -1 to enforce a negative relationship, 1 a positive relationship, and 0 will
 enforce no specific relationship at all. Features not included in the mapping
 will not have any constraint applied. If `None` is passed no constraints will
 be enforced on any variable. Defaults to `None`. - `subsample` ***(float,
 optional)***: Percent of records to randomly sample at each iteration when
 training a tree. Defaults to 1.0, meaning all data is used for training. -
+`top_rate` ***(float, optional)***: Used only in goss. The retain ratio of
+large gradient data. Defaults to 0.1. - `other_rate` ***(float, optional)***:
+Used only in goss. the retain ratio of small gradient data. Defaults to 0.2. -
 `seed` ***(integer, optional)***: Integer value used to seed any randomness
 used in the algorithm. Defaults to 0. - `missing` ***(float, optional)***:
 Value to consider missing, when training and predicting with the booster.
 Defaults to `np.nan`. - `create_missing_branch` ***(bool, optional)***: An
 experimental parameter, that if `True`, will create a separate branch for
 missing, creating a ternary tree, the missing node will be given the same
 weight value as the parent node. If this parameter is `False`, missing will be
```

### Comparing `forust-0.2.7/local_dependencies/forust-ml/benches/forust_benchmarks.rs` & `forust-0.2.8/local_dependencies/forust-ml/benches/forust_benchmarks.rs`

 * *Files identical despite different names*

### Comparing `forust-0.2.7/local_dependencies/forust-ml/resources/pdp_plot_age.png` & `forust-0.2.8/local_dependencies/forust-ml/resources/pdp_plot_age.png`

 * *Files identical despite different names*

### Comparing `forust-0.2.7/local_dependencies/forust-ml/resources/pdp_plot_age_mono.png` & `forust-0.2.8/local_dependencies/forust-ml/resources/pdp_plot_age_mono.png`

 * *Files identical despite different names*

### Comparing `forust-0.2.7/local_dependencies/forust-ml/resources/titanic.csv` & `forust-0.2.8/local_dependencies/forust-ml/resources/titanic.csv`

 * *Files identical despite different names*

### Comparing `forust-0.2.7/local_dependencies/forust-ml/resources/tree-image-crop.png` & `forust-0.2.8/local_dependencies/forust-ml/resources/tree-image-crop.png`

 * *Files identical despite different names*

### Comparing `forust-0.2.7/local_dependencies/forust-ml/rs-example.md` & `forust-0.2.8/local_dependencies/forust-ml/rs-example.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 ## A Complete Rust Example
 
 To run this example, add the following code to your `Cargo.toml` file.
 ```toml
 [dependencies]
-forust-ml = "0.2.7"
+forust-ml = "0.2.8"
 polars = "0.24"
 reqwest = { version = "0.11", features = ["blocking"] }
 ```
 
 The following is a runable example using `polars` for data processing. The actual data manipulation can be performed with any tool, the only vital part, is the data be in column major format.
 ```rust
 use forust_ml::{GradientBooster, Matrix};
```

### Comparing `forust-0.2.7/local_dependencies/forust-ml/scripts/make_resources.py` & `forust-0.2.8/local_dependencies/forust-ml/scripts/make_resources.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-import pandas as pd
 import numpy as np
+import pandas as pd
 import seaborn as sns
 
 if __name__ == "__main__":
     df = sns.load_dataset("titanic")
     X = df.select_dtypes("number").drop(columns=["survived"]).astype(float)
     y = df["survived"].astype(float)
```

### Comparing `forust-0.2.7/local_dependencies/forust-ml/src/binning.rs` & `forust-0.2.8/local_dependencies/forust-ml/src/binning.rs`

 * *Files identical despite different names*

### Comparing `forust-0.2.7/local_dependencies/forust-ml/src/data.rs` & `forust-0.2.8/local_dependencies/forust-ml/src/data.rs`

 * *Files identical despite different names*

### Comparing `forust-0.2.7/local_dependencies/forust-ml/src/errors.rs` & `forust-0.2.8/local_dependencies/forust-ml/src/errors.rs`

 * *Files identical despite different names*

### Comparing `forust-0.2.7/local_dependencies/forust-ml/src/gradientbooster.rs` & `forust-0.2.8/local_dependencies/forust-ml/src/gradientbooster.rs`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 use crate::constraints::ConstraintMap;
 use crate::data::{Matrix, RowMajorMatrix};
 use crate::errors::ForustError;
 use crate::metric::{is_comparison_better, metric_callables, Metric, MetricFn};
 use crate::objective::{
     gradient_hessian_callables, LogLoss, ObjectiveFunction, ObjectiveType, SquaredLoss,
 };
-use crate::sampler::{RandomSampler, SampleMethod, Sampler};
+use crate::sampler::{GossSampler, RandomSampler, SampleMethod, Sampler};
 use crate::splitter::{MissingBranchSplitter, MissingImputerSplitter, Splitter};
 use crate::tree::Tree;
 use rand::rngs::StdRng;
 use rand::SeedableRng;
 use rayon::prelude::*;
 use serde::{Deserialize, Deserializer, Serialize};
 use std::collections::HashMap;
@@ -50,14 +50,16 @@
 ///   will be used.
 /// * `allow_missing_splits` - Should the algorithm allow splits that completed seperate out missing
 /// and non-missing values, in the case where `create_missing_branch` is false. When `create_missing_branch`
 /// is true, setting this to true will result in the missin branch being further split.
 /// * `monotone_constraints` - Constraints that are used to enforce a specific relationship
 ///   between the training features and the target variable.
 /// * `subsample` - Percent of records to randomly sample at each iteration when training a tree.
+/// * `top_rate` - Used only in goss. The retain ratio of large gradient data.
+/// * `other_rate` - Used only in goss. the retain ratio of small gradient data.
 /// * `seed` - Integer value used to seed any randomness used in the algorithm.
 /// * `missing` - Value to consider missing.
 /// * `create_missing_branch` - Should missing be split out it's own separate branch?
 /// * `sample_method` - Specify the method that records should be sampled when training?
 /// * `evaluation_metric` - Define the evaluation metric to record at each iterations.
 /// * `early_stopping_rounds` - Number of rounds where the evaluation metric value must improve in
 ///    to keep training.
@@ -73,14 +75,16 @@
     pub min_leaf_weight: f32,
     pub base_score: f64,
     pub nbins: u16,
     pub parallel: bool,
     pub allow_missing_splits: bool,
     pub monotone_constraints: Option<ConstraintMap>,
     pub subsample: f32,
+    pub top_rate: f64,
+    pub other_rate: f64,
     pub seed: u64,
     #[serde(deserialize_with = "parse_missing")]
     pub missing: f64,
     pub create_missing_branch: bool,
     #[serde(default = "default_sample_method")]
     pub sample_method: SampleMethod,
     #[serde(default = "default_evaluation_metric")]
@@ -142,14 +146,16 @@
             1.,
             0.5,
             256,
             true,
             true,
             None,
             1.,
+            0.1,
+            0.2,
             0,
             f64::NAN,
             false,
             SampleMethod::None,
             None,
             None,
         )
@@ -184,14 +190,16 @@
     /// * `parallel` - Should the algorithm be run in parallel?
     /// * `allow_missing_splits` - Should the algorithm allow splits that completed seperate out missing
     /// and non-missing values, in the case where `create_missing_branch` is false. When `create_missing_branch`
     /// is true, setting this to true will result in the missin branch being further split.
     /// * `monotone_constraints` - Constraints that are used to enforce a specific relationship
     ///   between the training features and the target variable.
     /// * `subsample` - Percent of records to randomly sample at each iteration when training a tree.
+    /// * `top_rate` - Used only in goss. The retain ratio of large gradient data.
+    /// * `other_rate` - Used only in goss. the retain ratio of small gradient data.
     /// * `seed` - Integer value used to seed any randomness used in the algorithm.
     /// * `missing` - Value to consider missing.
     /// * `create_missing_branch` - Should missing be split out it's own separate branch?
     /// * `sample_method` - Specify the method that records should be sampled when training?
     /// * `evaluation_metric` - Define the evaluation metric to record at each iterations.
     /// * `early_stopping_rounds` - Number of rounds that must
     #[allow(clippy::too_many_arguments)]
@@ -206,14 +214,16 @@
         min_leaf_weight: f32,
         base_score: f64,
         nbins: u16,
         parallel: bool,
         allow_missing_splits: bool,
         monotone_constraints: Option<ConstraintMap>,
         subsample: f32,
+        top_rate: f64,
+        other_rate: f64,
         seed: u64,
         missing: f64,
         create_missing_branch: bool,
         sample_method: SampleMethod,
         evaluation_metric: Option<Metric>,
         early_stopping_rounds: Option<usize>,
     ) -> Self {
@@ -228,14 +238,16 @@
             min_leaf_weight,
             base_score,
             nbins,
             parallel,
             allow_missing_splits,
             monotone_constraints,
             subsample,
+            top_rate,
+            other_rate,
             seed,
             missing,
             create_missing_branch,
             sample_method,
             evaluation_metric,
             early_stopping_rounds,
             evaluation_history: None,
@@ -285,19 +297,29 @@
             };
             self.fit_trees(y, sample_weight, data, &splitter, evaluation_data)?;
         };
 
         Ok(())
     }
 
-    fn sample_index(&self, rng: &mut StdRng, index: &[usize]) -> (Vec<usize>, Vec<usize>) {
+    fn sample_index(
+        &self,
+        rng: &mut StdRng,
+        index: &[usize],
+        grad: &mut [f32],
+        hess: &mut [f32],
+    ) -> (Vec<usize>, Vec<usize>) {
         match self.sample_method {
             SampleMethod::None => (index.to_owned(), Vec::new()),
-            SampleMethod::Random => RandomSampler::new(self.subsample).sample(rng, index),
-            SampleMethod::Goss => todo!(),
+            SampleMethod::Random => {
+                RandomSampler::new(self.subsample).sample(rng, index, grad, hess)
+            }
+            SampleMethod::Goss => {
+                GossSampler::new(self.top_rate, self.other_rate).sample(rng, index, grad, hess)
+            }
         }
     }
 
     fn get_metric_fn(&self) -> (MetricFn, bool) {
         let metric = match &self.evaluation_metric {
             None => match self.objective_type {
                 ObjectiveType::LogLoss => LogLoss::default_metric(),
@@ -345,16 +367,18 @@
                     .collect()
             });
 
         let mut best_metric: Option<f64> = None;
 
         for i in 0..self.iterations {
             // We will eventually use the excluded index.
-            let (chosen_index, _excluded_index) = self.sample_index(&mut rng, &data.index);
+            let (chosen_index, _excluded_index) =
+                self.sample_index(&mut rng, &data.index, &mut grad, &mut hess);
             let mut tree = Tree::new();
+
             tree.fit(
                 &bdata,
                 chosen_index,
                 &binned_data.cuts,
                 &grad,
                 &hess,
                 splitter,
```

### Comparing `forust-0.2.7/local_dependencies/forust-ml/src/histogram.rs` & `forust-0.2.8/local_dependencies/forust-ml/src/histogram.rs`

 * *Files identical despite different names*

### Comparing `forust-0.2.7/local_dependencies/forust-ml/src/metric.rs` & `forust-0.2.8/local_dependencies/forust-ml/src/metric.rs`

 * *Files identical despite different names*

### Comparing `forust-0.2.7/local_dependencies/forust-ml/src/node.rs` & `forust-0.2.8/local_dependencies/forust-ml/src/node.rs`

 * *Files identical despite different names*

### Comparing `forust-0.2.7/local_dependencies/forust-ml/src/objective.rs` & `forust-0.2.8/local_dependencies/forust-ml/src/objective.rs`

 * *Files identical despite different names*

### Comparing `forust-0.2.7/local_dependencies/forust-ml/src/partial_dependence.rs` & `forust-0.2.8/local_dependencies/forust-ml/src/partial_dependence.rs`

 * *Files identical despite different names*

### Comparing `forust-0.2.7/local_dependencies/forust-ml/src/sampler.rs` & `forust-0.2.8/local_dependencies/forust-ml/src/sampler.rs`

 * *Files 23% similar despite different names*

```diff
@@ -28,30 +28,42 @@
     }
 }
 
 // A sampler can be used to subset the data prior to fitting a new tree.
 pub trait Sampler {
     /// Sample the data, returning a tuple, where the first item is the samples
     /// chosen for training, and the second are the samples excluded.
-    fn sample(&mut self, rng: &mut StdRng, index: &[usize]) -> (Vec<usize>, Vec<usize>);
+    fn sample(
+        &mut self,
+        rng: &mut StdRng,
+        index: &[usize],
+        grad: &mut [f32],
+        hess: &mut [f32],
+    ) -> (Vec<usize>, Vec<usize>);
 }
 
 pub struct RandomSampler {
     subsample: f32,
 }
 
 impl RandomSampler {
     #[allow(dead_code)]
     pub fn new(subsample: f32) -> Self {
         RandomSampler { subsample }
     }
 }
 
 impl Sampler for RandomSampler {
-    fn sample(&mut self, rng: &mut StdRng, index: &[usize]) -> (Vec<usize>, Vec<usize>) {
+    fn sample(
+        &mut self,
+        rng: &mut StdRng,
+        index: &[usize],
+        _grad: &mut [f32],
+        _hess: &mut [f32],
+    ) -> (Vec<usize>, Vec<usize>) {
         let subsample = self.subsample;
         let mut chosen = Vec::new();
         let mut excluded = Vec::new();
         for i in index {
             if rng.gen_range(0.0..1.0) < subsample {
                 chosen.push(*i);
             } else {
@@ -59,33 +71,59 @@
             }
         }
         (chosen, excluded)
     }
 }
 
 #[allow(dead_code)]
-pub struct GossSampler<'a> {
-    gradient: Option<&'a [f64]>,
+pub struct GossSampler {
+    a: f64, // https://lightgbm.readthedocs.io/en/latest/Parameters.html#top_rate
+    b: f64, // https://lightgbm.readthedocs.io/en/latest/Parameters.html#other_rate
 }
 
-impl<'a> Default for GossSampler<'a> {
+impl Default for GossSampler {
     fn default() -> Self {
-        Self::new()
+        GossSampler { a: 0.2, b: 0.1 }
     }
 }
 
 #[allow(dead_code)]
-impl<'a> GossSampler<'a> {
-    pub fn new() -> Self {
-        GossSampler { gradient: None }
-    }
-    pub fn add_gradient(&mut self, gradient: &'a [f64]) {
-        self.gradient = Some(gradient);
+impl GossSampler {
+    pub fn new(a: f64, b: f64) -> Self {
+        GossSampler { a, b }
     }
 }
 
-impl<'a> Sampler for GossSampler<'a> {
-    #[allow(unused_variables)]
-    fn sample(&mut self, rng: &mut StdRng, index: &[usize]) -> (Vec<usize>, Vec<usize>) {
-        todo!()
+impl Sampler for GossSampler {
+    fn sample(
+        &mut self,
+        rng: &mut StdRng,
+        index: &[usize],
+        grad: &mut [f32],
+        hess: &mut [f32],
+    ) -> (Vec<usize>, Vec<usize>) {
+        let fact = ((1. - self.a) / self.b) as f32;
+        let top_n = (self.a * index.len() as f64) as usize;
+        let rand_n = (self.b * index.len() as f64) as usize;
+
+        // sort gradient by absolute value from highest to lowest
+        let mut sorted = (0..index.len()).collect::<Vec<_>>();
+        sorted.sort_unstable_by(|&a, &b| grad[b].abs().total_cmp(&grad[a].abs()));
+
+        // select the topN largest gradients
+        let mut used_set = sorted[0..top_n].to_vec();
+
+        // sample the rest based on randN
+        let subsample = rand_n as f64 / (index.len() as f64 - top_n as f64);
+
+        // weight the sampled "small gradients" by fact and append indices to used_set
+        for i in &sorted[top_n..sorted.len()] {
+            if rng.gen_range(0.0..1.0) < subsample {
+                grad[*i] *= fact;
+                hess[*i] *= fact;
+                used_set.push(*i);
+            }
+        }
+
+        (used_set, Vec::new())
     }
 }
```

### Comparing `forust-0.2.7/local_dependencies/forust-ml/src/splitter.rs` & `forust-0.2.8/local_dependencies/forust-ml/src/splitter.rs`

 * *Files 1% similar despite different names*

```diff
@@ -36,14 +36,15 @@
 }
 
 pub trait Splitter {
     fn get_constraint(&self, feature: &usize) -> Option<&Constraint>;
     // fn get_allow_missing_splits(&self) -> bool;
     fn get_gamma(&self) -> f32;
     fn get_l2(&self) -> f32;
+    fn get_learning_rate(&self) -> f32;
 
     /// Find the best possible split, considering all feature histograms.
     /// If we wanted to add Column sampling, this is probably where
     /// we would need to do it, otherwise, it would be at the tree level.
     fn best_split(&self, node: &SplittableNode) -> Option<SplitInfo> {
         let mut best_split_info = None;
         let mut best_gain = 0.0;
@@ -97,25 +98,26 @@
 
         for (i, bin) in histogram[1..].iter().enumerate() {
             let left_gradient = cuml_grad;
             let left_hessian = cuml_hess;
             let right_gradient = node.gradient_sum - cuml_grad - missing.gradient_sum;
             let right_hessian = node.hessian_sum - cuml_hess - missing.hessian_sum;
 
-            let (mut left_node_info, mut right_node_info, missing_info) = match self.evaluate_split(
-                left_gradient,
-                left_hessian,
-                right_gradient,
-                right_hessian,
-                missing.gradient_sum,
-                missing.hessian_sum,
-                node.lower_bound,
-                node.upper_bound,
-                constraint,
-            ) {
+            let (mut left_node_info, mut right_node_info, mut missing_info) = match self
+                .evaluate_split(
+                    left_gradient,
+                    left_hessian,
+                    right_gradient,
+                    right_hessian,
+                    missing.gradient_sum,
+                    missing.hessian_sum,
+                    node.lower_bound,
+                    node.upper_bound,
+                    constraint,
+                ) {
                 None => {
                     cuml_grad += bin.gradient_sum;
                     cuml_hess += bin.hessian_sum;
                     continue;
                 }
                 Some(v) => v,
             };
@@ -154,15 +156,20 @@
                     (node.lower_bound, node.upper_bound),
                 ),
                 Some(Constraint::Negative) => ((mid, node.upper_bound), (node.lower_bound, mid)),
                 Some(Constraint::Positive) => ((node.lower_bound, mid), (mid, node.upper_bound)),
             };
             left_node_info.bounds = left_bounds;
             right_node_info.bounds = right_bounds;
-
+            // Apply shrinkage at this point...
+            left_node_info.weight *= self.get_learning_rate();
+            right_node_info.weight *= self.get_learning_rate();
+            if let MissingInfo::Branch(info) | MissingInfo::Leaf(info) = &mut missing_info {
+                info.weight *= self.get_learning_rate();
+            }
             // If split gain is NaN, one of the sides is empty, do not allow
             // this split.
             let split_gain = if split_gain.is_nan() { 0.0 } else { split_gain };
             if max_gain.is_none() || split_gain > max_gain.unwrap() {
                 max_gain = Some(split_gain);
                 split_info = Some(SplitInfo {
                     split_gain,
@@ -244,14 +251,18 @@
         self.gamma
     }
 
     fn get_l2(&self) -> f32 {
         self.l2
     }
 
+    fn get_learning_rate(&self) -> f32 {
+        self.learning_rate
+    }
+
     fn evaluate_split(
         &self,
         left_gradient: f32,
         left_hessian: f32,
         right_gradient: f32,
         right_hessian: f32,
         missing_gradient: f32,
@@ -265,20 +276,14 @@
         // and so we should continue.
         if (left_gradient == 0.0) && (left_hessian == 0.0)
             || (right_gradient == 0.0) && (right_hessian == 0.0)
         {
             return None;
         }
 
-        let left_gradient = left_gradient;
-        let left_hessian = left_hessian;
-
-        let right_gradient = right_gradient;
-        let right_hessian = right_hessian;
-
         let left_weight = constrained_weight(
             &self.l2,
             left_gradient,
             left_hessian,
             lower_bound,
             upper_bound,
             constraint,
@@ -318,15 +323,15 @@
             missing_hessian,
             missing_weight,
         );
         let missing_info = NodeInfo {
             grad: missing_gradient,
             gain: missing_gain,
             cover: missing_hessian,
-            weight: missing_weight * self.learning_rate,
+            weight: missing_weight,
             bounds: (f32::NEG_INFINITY, f32::INFINITY),
         };
         let missing_node = // Check Missing direction
         if ((missing_gradient != 0.0) || (missing_hessian != 0.0)) && self.allow_missing_splits {
             MissingInfo::Branch(
                 missing_info
             )
@@ -341,22 +346,22 @@
             return None;
         }
         Some((
             NodeInfo {
                 grad: left_gradient,
                 gain: left_gain,
                 cover: left_hessian,
-                weight: left_weight * self.learning_rate,
+                weight: left_weight,
                 bounds: (f32::NEG_INFINITY, f32::INFINITY),
             },
             NodeInfo {
                 grad: right_gradient,
                 gain: right_gain,
                 cover: right_hessian,
-                weight: right_weight * self.learning_rate,
+                weight: right_weight,
                 bounds: (f32::NEG_INFINITY, f32::INFINITY),
             },
             missing_node,
         ))
     }
 
     fn handle_split_info(
@@ -589,14 +594,30 @@
             allow_missing_splits,
             constraints_map,
         }
     }
 }
 
 impl Splitter for MissingImputerSplitter {
+    fn get_constraint(&self, feature: &usize) -> Option<&Constraint> {
+        self.constraints_map.get(feature)
+    }
+
+    fn get_gamma(&self) -> f32 {
+        self.gamma
+    }
+
+    fn get_l2(&self) -> f32 {
+        self.l2
+    }
+
+    fn get_learning_rate(&self) -> f32 {
+        self.learning_rate
+    }
+
     #[allow(clippy::too_many_arguments)]
     fn evaluate_split(
         &self,
         left_gradient: f32,
         left_hessian: f32,
         right_gradient: f32,
         right_hessian: f32,
@@ -729,22 +750,22 @@
             return None;
         }
         Some((
             NodeInfo {
                 grad: left_gradient,
                 gain: left_gain,
                 cover: left_hessian,
-                weight: left_weight * self.learning_rate,
+                weight: left_weight,
                 bounds: (f32::NEG_INFINITY, f32::INFINITY),
             },
             NodeInfo {
                 grad: right_gradient,
                 gain: right_gain,
                 cover: right_hessian,
-                weight: right_weight * self.learning_rate,
+                weight: right_weight,
                 bounds: (f32::NEG_INFINITY, f32::INFINITY),
             },
             missing_info,
         ))
     }
 
     fn handle_split_info(
@@ -839,26 +860,14 @@
             node.depth + 1,
             split_idx,
             node.stop_idx,
             split_info.right_node,
         );
         vec![left_node, right_node]
     }
-
-    fn get_constraint(&self, feature: &usize) -> Option<&Constraint> {
-        self.constraints_map.get(feature)
-    }
-
-    fn get_gamma(&self) -> f32 {
-        self.gamma
-    }
-
-    fn get_l2(&self) -> f32 {
-        self.l2
-    }
 }
 
 #[cfg(test)]
 mod tests {
     use super::*;
     use crate::binning::bin_matrix;
     use crate::data::Matrix;
```

### Comparing `forust-0.2.7/local_dependencies/forust-ml/src/tree.rs` & `forust-0.2.8/local_dependencies/forust-ml/src/tree.rs`

 * *Files 0% similar despite different names*

```diff
@@ -409,16 +409,16 @@
             .expect("Something went wrong reading the file");
         let data_vec: Vec<f64> = file.lines().map(|x| x.parse::<f64>().unwrap()).collect();
         let file = fs::read_to_string("resources/performance.csv")
             .expect("Something went wrong reading the file");
         let y: Vec<f64> = file.lines().map(|x| x.parse::<f64>().unwrap()).collect();
         let yhat = vec![0.5; y.len()];
         let w = vec![1.; y.len()];
-        let g = LogLoss::calc_grad(&y, &yhat, &w);
-        let h = LogLoss::calc_hess(&y, &yhat, &w);
+        let mut g = LogLoss::calc_grad(&y, &yhat, &w);
+        let mut h = LogLoss::calc_hess(&y, &yhat, &w);
 
         let data = Matrix::new(&data_vec, 891, 5);
         let splitter = MissingImputerSplitter {
             l2: 1.0,
             gamma: 3.0,
             min_leaf_weight: 1.0,
             learning_rate: 0.3,
@@ -426,15 +426,16 @@
             constraints_map: ConstraintMap::new(),
         };
         let mut tree = Tree::new();
 
         let b = bin_matrix(&data, &w, 300, f64::NAN).unwrap();
         let bdata = Matrix::new(&b.binned_data, data.rows, data.cols);
         let mut rng = StdRng::seed_from_u64(0);
-        let (index, excluded) = RandomSampler::new(0.5).sample(&mut rng, &data.index);
+        let (index, excluded) =
+            RandomSampler::new(0.5).sample(&mut rng, &data.index, &mut g, &mut h);
         assert!(excluded.len() > 0);
         tree.fit(
             &bdata,
             index,
             &b.cuts,
             &g,
             &h,
```

### Comparing `forust-0.2.7/local_dependencies/forust-ml/src/utils.rs` & `forust-0.2.8/local_dependencies/forust-ml/src/utils.rs`

 * *Files 0% similar despite different names*

```diff
@@ -76,22 +76,22 @@
     left_weight: f32,
     right_weight: f32,
     constraint: Option<&Constraint>,
 ) -> f32 {
     match constraint {
         None | Some(Constraint::Unconstrained) => gain,
         Some(Constraint::Negative) => {
-            if left_weight < right_weight {
+            if left_weight <= right_weight {
                 f32::NEG_INFINITY
             } else {
                 gain
             }
         }
         Some(Constraint::Positive) => {
-            if left_weight > right_weight {
+            if left_weight >= right_weight {
                 f32::NEG_INFINITY
             } else {
                 gain
             }
         }
     }
 }
```

### Comparing `forust-0.2.7/.gitignore` & `forust-0.2.8/.gitignore`

 * *Files identical despite different names*

### Comparing `forust-0.2.7/README.md` & `forust-0.2.8/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 The package can be installed directly from [pypi](https://pypi.org/project/forust/).
 ```shell
 pip install forust
 ```
 
 To use in a rust project add the following to your Cargo.toml file.
 ```toml
-forust-ml = "0.2.7"
+forust-ml = "0.2.8"
 ```
 
 ## Usage
 The `GradientBooster` class is currently the only public facing class in the package, and can be used to train gradient boosted decision tree ensembles with multiple objective functions.
 
 It can be initialized with the following arguments.
 
@@ -60,14 +60,16 @@
     will be used. Defaults to 256.
  - `parallel` ***(bool, optional)***: Should multiple cores be used when training and predicting
     with this model? Defaults to `True`.
  - `allow_missing_splits` ***(bool, optional)***: Allow for splits to be made such that all missing values go down one branch, and all non-missing values go down the other, if this results in the greatest reduction of loss. If this is false, splits will only be made on non missing values. If `create_missing_branch` is set to `True` having this parameter be set to `True` will result in the missing branch further split, if this parameter is `False` then in that case the missing branch will always be a terminal node. Defaults to `True`.
  - `monotone_constraints` ***(dict[Any, int], optional)***: Constraints that are used to enforce a specific relationship between the training features and the target variable. A dictionary should be provided where the keys are the feature index value if the model will be fit on a numpy array, or a feature name if it will be fit on a pandas Dataframe. The values of the dictionary should be an integer value of -1, 1, or 0 to specify the relationship that should be estimated between the respective feature and the target variable. Use a value of -1 to enforce a negative relationship, 1 a positive relationship, and 0 will enforce no specific relationship at all. Features not included in the mapping will not have any constraint applied. If `None` is passed no constraints will be enforced on any variable.  Defaults to `None`.
  - `subsample` ***(float, optional)***: Percent of records to randomly sample at each iteration when
       training a tree. Defaults to 1.0, meaning all data is used for training.
+ - `top_rate` ***(float, optional)***: Used only in goss. The retain ratio of large gradient data. Defaults to 0.1.
+ - `other_rate` ***(float, optional)***: Used only in goss. the retain ratio of small gradient data. Defaults to 0.2.
  - `seed` ***(integer, optional)***: Integer value used to seed any randomness used in the
       algorithm. Defaults to 0.
  - `missing` ***(float, optional)***: Value to consider missing, when training and predicting with the booster. Defaults to `np.nan`.
  - `create_missing_branch` ***(bool, optional)***: An experimental parameter, that if `True`, will create a separate branch for missing, creating a ternary tree, the missing node will be given the same weight value as the parent node. If this parameter is `False`, missing will be sent down either the left or right branch, creating a binary tree. Defaults to `False`.
  - `sample_method` ***(str | None, optional)***: Optional string value to use to determine the method to use to sample the data while training. If this is None, no sample method will be used. If the `subsample` parameter is less than 1 and no sample_method is provided this `sample_method` will be automatically set to "random". Valid options are "goss" and "random". Defaults to `None`.
  - `evaluation_metric` ***(str | None, optional)***: Optional string value used to define an evaluation metric that will be calculated at each iteration if a `evaluation_dataset` is provided at fit time. The metric can be one of "AUC", "LogLoss", "RootMeanSquaredLogError", or "RootMeanSquaredError". If no `evaluation_metric` is passed, but an `evaluation_dataset` is passed, then "LogLoss", will be used with the "LogLoss" objective function, and "RootMeanSquaredLogError" will be used with "SquaredLoss".
  - `early_stopping_rounds` ***(int | None, optional)***: If this is specified, and an `evaluation_dataset` is passed during fit, then an improvement in the `evaluation_metric` must be seen after at least this many iterations of training, otherwise training will be cut short.
```

#### html2text {}

```diff
@@ -13,15 +13,15 @@
 understand the XGBoost algorithm, additionally to have a fun project to work on
 in rust, and because I wanted to be able to experiment with adding new features
 to the algorithm in a smaller simpler codebase. All of the rust code for the
 package can be found in the [src](src/) directory, while all of the python
 wrapper code is in the [py-forust](py-forust/) directory. ## Installation The
 package can be installed directly from [pypi](https://pypi.org/project/forust/
 ). ```shell pip install forust ``` To use in a rust project add the following
-to your Cargo.toml file. ```toml forust-ml = "0.2.7" ``` ## Usage The
+to your Cargo.toml file. ```toml forust-ml = "0.2.8" ``` ## Usage The
 `GradientBooster` class is currently the only public facing class in the
 package, and can be used to train gradient boosted decision tree ensembles with
 multiple objective functions. It can be initialized with the following
 arguments. - `objective_type` ***(str, optional)***: The name of objective
 function used to optimize. Valid options include "LogLoss" to use logistic loss
 as the objective function (binary classification), or "SquaredLoss" to use
 Squared Error as the objective function (continuous regression). Defaults to
@@ -62,14 +62,17 @@
 estimated between the respective feature and the target variable. Use a value
 of -1 to enforce a negative relationship, 1 a positive relationship, and 0 will
 enforce no specific relationship at all. Features not included in the mapping
 will not have any constraint applied. If `None` is passed no constraints will
 be enforced on any variable. Defaults to `None`. - `subsample` ***(float,
 optional)***: Percent of records to randomly sample at each iteration when
 training a tree. Defaults to 1.0, meaning all data is used for training. -
+`top_rate` ***(float, optional)***: Used only in goss. The retain ratio of
+large gradient data. Defaults to 0.1. - `other_rate` ***(float, optional)***:
+Used only in goss. the retain ratio of small gradient data. Defaults to 0.2. -
 `seed` ***(integer, optional)***: Integer value used to seed any randomness
 used in the algorithm. Defaults to 0. - `missing` ***(float, optional)***:
 Value to consider missing, when training and predicting with the booster.
 Defaults to `np.nan`. - `create_missing_branch` ***(bool, optional)***: An
 experimental parameter, that if `True`, will create a separate branch for
 missing, creating a ternary tree, the missing node will be given the same
 weight value as the parent node. If this parameter is `False`, missing will be
```

### Comparing `forust-0.2.7/forust/__init__.py` & `forust-0.2.8/forust/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -138,14 +138,16 @@
         min_leaf_weight: float = 1.0,
         base_score: float = 0.5,
         nbins: int = 256,
         parallel: bool = True,
         allow_missing_splits: bool = True,
         monotone_constraints: Union[dict[Any, int], None] = None,
         subsample: float = 1.0,
+        top_rate: float = 0.1,
+        other_rate: float = 0.2,
         seed: int = 0,
         missing: float = np.nan,
         create_missing_branch: bool = False,
         sample_method: str | None = None,
         evaluation_metric: str | None = None,
         early_stopping_rounds: int | None = None,
     ):
@@ -193,14 +195,16 @@
                 that should be estimated between the respective feature and the target variable.
                 Use a value of -1 to enforce a negative relationship, 1 a positive relationship,
                 and 0 will enforce no specific relationship at all. Features not included in the
                 mapping will not have any constraint applied. If `None` is passed no constraints
                 will be enforced on any variable.  Defaults to `None`.
             subsample (float, optional): Percent of records to randomly sample at each iteration when
                 training a tree. Defaults to 1.0, meaning all data is used to training.
+            top_rate (float, optional): Used only in goss. The retain ratio of large gradient data.
+            other_rate (float, optional):Used only in goss. the retain ratio of small gradient data.
             seed (integer, optional): Integer value used to seed any randomness used in the
                 algorithm. Defaults to 0.
             missing (float, optional): Value to consider missing, when training and predicting
                 with the booster. Defaults to `np.nan`.
             create_missing_branch (bool, optional): An experimental parameter, that if `True`, will
                 create a separate branch for missing, creating a ternary tree, the missing node will be given the same
                 weight value as the parent node. If this parameter is `False`, missing will be sent
@@ -237,14 +241,16 @@
             min_leaf_weight=min_leaf_weight,
             base_score=base_score,
             nbins=nbins,
             parallel=parallel,
             allow_missing_splits=allow_missing_splits,
             monotone_constraints={},
             subsample=subsample,
+            top_rate=top_rate,
+            other_rate=other_rate,
             seed=seed,
             missing=missing,
             create_missing_branch=create_missing_branch,
             sample_method=sample_method,
             evaluation_metric=evaluation_metric,
             early_stopping_rounds=early_stopping_rounds,
         )
@@ -266,14 +272,16 @@
         self.allow_missing_splits = allow_missing_splits
         self.monotone_constraints = monotone_constraints_
         self.subsample = subsample
         self.seed = seed
         self.missing = missing
         self.create_missing_branch = create_missing_branch
         self.sample_method = sample_method
+        self.top_rate = top_rate
+        self.other_rate = other_rate
         self.evaluation_metric = evaluation_metric
         self.early_stopping_rounds = early_stopping_rounds
 
     def fit(
         self,
         X: FrameLike,
         y: ArrayLike,
```

### Comparing `forust-0.2.7/pyproject.toml` & `forust-0.2.8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `forust-0.2.7/scratch.py` & `forust-0.2.8/scratch.py`

 * *Files identical despite different names*

### Comparing `forust-0.2.7/src/lib.rs` & `forust-0.2.8/src/lib.rs`

 * *Files 1% similar despite different names*

```diff
@@ -64,14 +64,16 @@
         min_leaf_weight: f32,
         base_score: f64,
         nbins: u16,
         parallel: bool,
         allow_missing_splits: bool,
         monotone_constraints: HashMap<usize, i8>,
         subsample: f32,
+        top_rate: f64,
+        other_rate: f64,
         seed: u64,
         missing: f64,
         create_missing_branch: bool,
         sample_method: Option<&str>,
         evaluation_metric: Option<&str>,
         early_stopping_rounds: Option<usize>,
     ) -> PyResult<Self> {
@@ -96,14 +98,16 @@
             min_leaf_weight,
             base_score,
             nbins,
             parallel,
             allow_missing_splits,
             Some(constraints),
             subsample,
+            top_rate,
+            other_rate,
             seed,
             missing,
             create_missing_branch,
             sample_method_,
             evaluation_metric_,
             early_stopping_rounds,
         );
@@ -306,14 +310,16 @@
             ("parallel", self.booster.parallel.to_object(py)),
             (
                 "allow_missing_splits",
                 self.booster.allow_missing_splits.to_object(py),
             ),
             ("monotone_constraints", constraints.to_object(py)),
             ("subsample", self.booster.subsample.to_object(py)),
+            ("top_rate", self.booster.top_rate.to_object(py)),
+            ("other_rate", self.booster.other_rate.to_object(py)),
             ("seed", self.booster.seed.to_object(py)),
             ("missing", self.booster.missing.to_object(py)),
             (
                 "create_missing_branch",
                 self.booster.create_missing_branch.to_object(py),
             ),
             ("sample_method", sample_method_.to_object(py)),
```

### Comparing `forust-0.2.7/tests/test_booster.py` & `forust-0.2.8/tests/test_booster.py`

 * *Files 2% similar despite different names*

```diff
@@ -539,7 +539,30 @@
     assert best_iteration < history.shape[0]
     fmod.set_prediction_iteration(4)
     new_preds = fmod.predict(X)
     assert not np.allclose(new_preds, preds)
     fmod.save_booster(mod_path)
     loaded = GradientBooster.load_booster(mod_path)
     assert np.allclose(loaded.predict(X), new_preds)
+
+
+def test_goss_sampling_method(X_y):
+    X, y = X_y
+    X = X
+    fmod = GradientBooster(
+        iterations=100,
+        learning_rate=0.3,
+        max_depth=5,
+        l2=1,
+        sample_method="goss",
+        min_leaf_weight=1,
+        gamma=1,
+        top_rate=0.2,
+        other_rate=0.3,
+        objective_type="LogLoss",
+        nbins=500,
+        parallel=True,
+        base_score=0.5,
+    )
+    fmod.fit(X, y=y)
+
+    assert True
```

### Comparing `forust-0.2.7/LICENSE` & `forust-0.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `forust-0.2.7/PKG-INFO` & `forust-0.2.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: forust
-Version: 0.2.7
+Version: 0.2.8
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Dist: numpy>=1.21
 Requires-Dist: pandas>=1.3
 Requires-Dist: maturin; extra == 'dev'
 Requires-Dist: pytest; extra == 'dev'
@@ -43,15 +43,15 @@
 The package can be installed directly from [pypi](https://pypi.org/project/forust/).
 ```shell
 pip install forust
 ```
 
 To use in a rust project add the following to your Cargo.toml file.
 ```toml
-forust-ml = "0.2.7"
+forust-ml = "0.2.8"
 ```
 
 ## Usage
 The `GradientBooster` class is currently the only public facing class in the package, and can be used to train gradient boosted decision tree ensembles with multiple objective functions.
 
 It can be initialized with the following arguments.
 
@@ -81,14 +81,16 @@
     will be used. Defaults to 256.
  - `parallel` ***(bool, optional)***: Should multiple cores be used when training and predicting
     with this model? Defaults to `True`.
  - `allow_missing_splits` ***(bool, optional)***: Allow for splits to be made such that all missing values go down one branch, and all non-missing values go down the other, if this results in the greatest reduction of loss. If this is false, splits will only be made on non missing values. If `create_missing_branch` is set to `True` having this parameter be set to `True` will result in the missing branch further split, if this parameter is `False` then in that case the missing branch will always be a terminal node. Defaults to `True`.
  - `monotone_constraints` ***(dict[Any, int], optional)***: Constraints that are used to enforce a specific relationship between the training features and the target variable. A dictionary should be provided where the keys are the feature index value if the model will be fit on a numpy array, or a feature name if it will be fit on a pandas Dataframe. The values of the dictionary should be an integer value of -1, 1, or 0 to specify the relationship that should be estimated between the respective feature and the target variable. Use a value of -1 to enforce a negative relationship, 1 a positive relationship, and 0 will enforce no specific relationship at all. Features not included in the mapping will not have any constraint applied. If `None` is passed no constraints will be enforced on any variable.  Defaults to `None`.
  - `subsample` ***(float, optional)***: Percent of records to randomly sample at each iteration when
       training a tree. Defaults to 1.0, meaning all data is used for training.
+ - `top_rate` ***(float, optional)***: Used only in goss. The retain ratio of large gradient data. Defaults to 0.1.
+ - `other_rate` ***(float, optional)***: Used only in goss. the retain ratio of small gradient data. Defaults to 0.2.
  - `seed` ***(integer, optional)***: Integer value used to seed any randomness used in the
       algorithm. Defaults to 0.
  - `missing` ***(float, optional)***: Value to consider missing, when training and predicting with the booster. Defaults to `np.nan`.
  - `create_missing_branch` ***(bool, optional)***: An experimental parameter, that if `True`, will create a separate branch for missing, creating a ternary tree, the missing node will be given the same weight value as the parent node. If this parameter is `False`, missing will be sent down either the left or right branch, creating a binary tree. Defaults to `False`.
  - `sample_method` ***(str | None, optional)***: Optional string value to use to determine the method to use to sample the data while training. If this is None, no sample method will be used. If the `subsample` parameter is less than 1 and no sample_method is provided this `sample_method` will be automatically set to "random". Valid options are "goss" and "random". Defaults to `None`.
  - `evaluation_metric` ***(str | None, optional)***: Optional string value used to define an evaluation metric that will be calculated at each iteration if a `evaluation_dataset` is provided at fit time. The metric can be one of "AUC", "LogLoss", "RootMeanSquaredLogError", or "RootMeanSquaredError". If no `evaluation_metric` is passed, but an `evaluation_dataset` is passed, then "LogLoss", will be used with the "LogLoss" objective function, and "RootMeanSquaredLogError" will be used with "SquaredLoss".
  - `early_stopping_rounds` ***(int | None, optional)***: If this is specified, and an `evaluation_dataset` is passed during fit, then an improvement in the `evaluation_metric` must be seen after at least this many iterations of training, otherwise training will be cut short.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: forust Version: 0.2.7 Classifier: Programming
+Metadata-Version: 2.1 Name: forust Version: 0.2.8 Classifier: Programming
 Language :: Rust Classifier: Programming Language :: Python :: Implementation
 :: CPython Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Dist: numpy>=1.21 Requires-Dist: pandas>=1.3 Requires-Dist: maturin;
 extra == 'dev' Requires-Dist: pytest; extra == 'dev' Requires-Dist: seaborn;
 extra == 'dev' Requires-Dist: xgboost==1.6.1; extra == 'dev' Requires-Dist:
 scikit-learn; extra == 'dev' Provides-Extra: dev License-File: LICENSE Summary:
 A lightweight gradient boosting implementation in Rust. Keywords:
@@ -24,15 +24,15 @@
 understand the XGBoost algorithm, additionally to have a fun project to work on
 in rust, and because I wanted to be able to experiment with adding new features
 to the algorithm in a smaller simpler codebase. All of the rust code for the
 package can be found in the [src](src/) directory, while all of the python
 wrapper code is in the [py-forust](py-forust/) directory. ## Installation The
 package can be installed directly from [pypi](https://pypi.org/project/forust/
 ). ```shell pip install forust ``` To use in a rust project add the following
-to your Cargo.toml file. ```toml forust-ml = "0.2.7" ``` ## Usage The
+to your Cargo.toml file. ```toml forust-ml = "0.2.8" ``` ## Usage The
 `GradientBooster` class is currently the only public facing class in the
 package, and can be used to train gradient boosted decision tree ensembles with
 multiple objective functions. It can be initialized with the following
 arguments. - `objective_type` ***(str, optional)***: The name of objective
 function used to optimize. Valid options include "LogLoss" to use logistic loss
 as the objective function (binary classification), or "SquaredLoss" to use
 Squared Error as the objective function (continuous regression). Defaults to
@@ -73,14 +73,17 @@
 estimated between the respective feature and the target variable. Use a value
 of -1 to enforce a negative relationship, 1 a positive relationship, and 0 will
 enforce no specific relationship at all. Features not included in the mapping
 will not have any constraint applied. If `None` is passed no constraints will
 be enforced on any variable. Defaults to `None`. - `subsample` ***(float,
 optional)***: Percent of records to randomly sample at each iteration when
 training a tree. Defaults to 1.0, meaning all data is used for training. -
+`top_rate` ***(float, optional)***: Used only in goss. The retain ratio of
+large gradient data. Defaults to 0.1. - `other_rate` ***(float, optional)***:
+Used only in goss. the retain ratio of small gradient data. Defaults to 0.2. -
 `seed` ***(integer, optional)***: Integer value used to seed any randomness
 used in the algorithm. Defaults to 0. - `missing` ***(float, optional)***:
 Value to consider missing, when training and predicting with the booster.
 Defaults to `np.nan`. - `create_missing_branch` ***(bool, optional)***: An
 experimental parameter, that if `True`, will create a separate branch for
 missing, creating a ternary tree, the missing node will be given the same
 weight value as the parent node. If this parameter is `False`, missing will be
```

