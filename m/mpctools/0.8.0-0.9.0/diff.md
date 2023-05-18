# Comparing `tmp/mpctools-0.8.0.tar.gz` & `tmp/mpctools-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/mpctools-0.8.0.tar", last modified: Mon Oct 24 14:25:17 2022, max compression
+gzip compressed data, was "dist/mpctools-0.9.0.tar", last modified: Wed Nov 16 13:04:18 2022, max compression
```

## Comparing `mpctools-0.8.0.tar` & `mpctools-0.9.0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxr-x   0 s1238640  (1000) s1238640  (1000)        0 2022-10-24 14:25:17.000000 mpctools-0.8.0/
--rw-r--r--   0 s1238640  (1000) s1238640  (1000)    35147 2018-09-20 17:03:59.000000 mpctools-0.8.0/LICENSE
--rw-rw-r--   0 s1238640  (1000) s1238640  (1000)     3298 2022-10-24 14:25:17.000000 mpctools-0.8.0/PKG-INFO
--rw-rw-r--   0 s1238640  (1000) s1238640  (1000)     2516 2021-07-08 09:58:35.000000 mpctools-0.8.0/README.md
-drwxrwxr-x   0 s1238640  (1000) s1238640  (1000)        0 2022-10-24 14:25:17.000000 mpctools-0.8.0/mpctools/
--rw-rw-r--   0 s1238640  (1000) s1238640  (1000)      711 2022-10-24 14:22:46.000000 mpctools-0.8.0/mpctools/__init__.py
-drwxrwxr-x   0 s1238640  (1000) s1238640  (1000)        0 2022-10-24 14:25:17.000000 mpctools-0.8.0/mpctools/extensions/
--rw-rw-r--   0 s1238640  (1000) s1238640  (1000)      689 2020-04-28 09:33:14.000000 mpctools-0.8.0/mpctools/extensions/__init__.py
--rw-rw-r--   0 s1238640  (1000) s1238640  (1000)    56107 2022-08-26 08:02:36.000000 mpctools-0.8.0/mpctools/extensions/cvext.py
--rw-rw-r--   0 s1238640  (1000) s1238640  (1000)    18131 2022-10-24 12:54:35.000000 mpctools-0.8.0/mpctools/extensions/mplext.py
--rw-rw-r--   0 s1238640  (1000) s1238640  (1000)    30987 2022-03-22 08:57:24.000000 mpctools-0.8.0/mpctools/extensions/npext.py
--rw-rw-r--   0 s1238640  (1000) s1238640  (1000)     5041 2021-03-05 16:41:45.000000 mpctools-0.8.0/mpctools/extensions/pdext.py
--rw-rw-r--   0 s1238640  (1000) s1238640  (1000)    15570 2022-10-24 07:49:48.000000 mpctools-0.8.0/mpctools/extensions/skext.py
--rw-rw-r--   0 s1238640  (1000) s1238640  (1000)    14790 2022-10-06 15:28:18.000000 mpctools-0.8.0/mpctools/extensions/utils.py
-drwxrwxr-x   0 s1238640  (1000) s1238640  (1000)        0 2022-10-24 14:25:17.000000 mpctools-0.8.0/mpctools/parallel/
--rw-rw-r--   0 s1238640  (1000) s1238640  (1000)      813 2020-04-28 09:33:25.000000 mpctools-0.8.0/mpctools/parallel/__init__.py
--rw-rw-r--   0 s1238640  (1000) s1238640  (1000)     4823 2020-08-17 15:36:04.000000 mpctools-0.8.0/mpctools/parallel/progress_bar.py
--rw-rw-r--   0 s1238640  (1000) s1238640  (1000)    12122 2020-04-27 19:02:33.000000 mpctools-0.8.0/mpctools/parallel/worker_handler.py
-drwxrwxr-x   0 s1238640  (1000) s1238640  (1000)        0 2022-10-24 14:25:17.000000 mpctools-0.8.0/mpctools.egg-info/
--rw-r--r--   0 s1238640  (1000) s1238640  (1000)     3298 2022-10-24 14:25:17.000000 mpctools-0.8.0/mpctools.egg-info/PKG-INFO
--rw-r--r--   0 s1238640  (1000) s1238640  (1000)      523 2022-10-24 14:25:17.000000 mpctools-0.8.0/mpctools.egg-info/SOURCES.txt
--rw-r--r--   0 s1238640  (1000) s1238640  (1000)        1 2022-10-24 14:25:17.000000 mpctools-0.8.0/mpctools.egg-info/dependency_links.txt
--rw-r--r--   0 s1238640  (1000) s1238640  (1000)      109 2022-10-24 14:25:17.000000 mpctools-0.8.0/mpctools.egg-info/requires.txt
--rw-r--r--   0 s1238640  (1000) s1238640  (1000)        9 2022-10-24 14:25:17.000000 mpctools-0.8.0/mpctools.egg-info/top_level.txt
--rw-rw-r--   0 s1238640  (1000) s1238640  (1000)       79 2022-10-24 14:25:17.000000 mpctools-0.8.0/setup.cfg
--rw-rw-r--   0 s1238640  (1000) s1238640  (1000)     1543 2022-10-24 14:22:46.000000 mpctools-0.8.0/setup.py
+drwxrwxr-x   0 s1238640  (1000) s1238640  (1000)        0 2022-11-16 13:04:18.000000 mpctools-0.9.0/
+-rw-r--r--   0 s1238640  (1000) s1238640  (1000)    35147 2018-09-20 17:03:59.000000 mpctools-0.9.0/LICENSE
+-rw-rw-r--   0 s1238640  (1000) s1238640  (1000)     3298 2022-11-16 13:04:18.000000 mpctools-0.9.0/PKG-INFO
+-rw-rw-r--   0 s1238640  (1000) s1238640  (1000)     2516 2021-07-08 09:58:35.000000 mpctools-0.9.0/README.md
+drwxrwxr-x   0 s1238640  (1000) s1238640  (1000)        0 2022-11-16 13:04:18.000000 mpctools-0.9.0/mpctools/
+-rw-rw-r--   0 s1238640  (1000) s1238640  (1000)      711 2022-11-16 13:00:39.000000 mpctools-0.9.0/mpctools/__init__.py
+drwxrwxr-x   0 s1238640  (1000) s1238640  (1000)        0 2022-11-16 13:04:18.000000 mpctools-0.9.0/mpctools/extensions/
+-rw-rw-r--   0 s1238640  (1000) s1238640  (1000)      689 2020-04-28 09:33:14.000000 mpctools-0.9.0/mpctools/extensions/__init__.py
+-rw-rw-r--   0 s1238640  (1000) s1238640  (1000)    56107 2022-08-26 08:02:36.000000 mpctools-0.9.0/mpctools/extensions/cvext.py
+-rw-rw-r--   0 s1238640  (1000) s1238640  (1000)    18148 2022-10-25 11:53:35.000000 mpctools-0.9.0/mpctools/extensions/mplext.py
+-rw-rw-r--   0 s1238640  (1000) s1238640  (1000)    30923 2022-10-28 17:36:36.000000 mpctools-0.9.0/mpctools/extensions/npext.py
+-rw-rw-r--   0 s1238640  (1000) s1238640  (1000)     5041 2021-03-05 16:41:45.000000 mpctools-0.9.0/mpctools/extensions/pdext.py
+-rw-rw-r--   0 s1238640  (1000) s1238640  (1000)    19072 2022-11-09 10:00:12.000000 mpctools-0.9.0/mpctools/extensions/skext.py
+-rw-rw-r--   0 s1238640  (1000) s1238640  (1000)    14790 2022-10-06 15:28:18.000000 mpctools-0.9.0/mpctools/extensions/utils.py
+drwxrwxr-x   0 s1238640  (1000) s1238640  (1000)        0 2022-11-16 13:04:18.000000 mpctools-0.9.0/mpctools/parallel/
+-rw-rw-r--   0 s1238640  (1000) s1238640  (1000)      813 2020-04-28 09:33:25.000000 mpctools-0.9.0/mpctools/parallel/__init__.py
+-rw-rw-r--   0 s1238640  (1000) s1238640  (1000)     4823 2020-08-17 15:36:04.000000 mpctools-0.9.0/mpctools/parallel/progress_bar.py
+-rw-rw-r--   0 s1238640  (1000) s1238640  (1000)    12122 2020-04-27 19:02:33.000000 mpctools-0.9.0/mpctools/parallel/worker_handler.py
+drwxrwxr-x   0 s1238640  (1000) s1238640  (1000)        0 2022-11-16 13:04:18.000000 mpctools-0.9.0/mpctools.egg-info/
+-rw-rw-r--   0 s1238640  (1000) s1238640  (1000)     3298 2022-11-16 13:04:18.000000 mpctools-0.9.0/mpctools.egg-info/PKG-INFO
+-rw-rw-r--   0 s1238640  (1000) s1238640  (1000)      523 2022-11-16 13:04:18.000000 mpctools-0.9.0/mpctools.egg-info/SOURCES.txt
+-rw-rw-r--   0 s1238640  (1000) s1238640  (1000)        1 2022-11-16 13:04:18.000000 mpctools-0.9.0/mpctools.egg-info/dependency_links.txt
+-rw-rw-r--   0 s1238640  (1000) s1238640  (1000)      115 2022-11-16 13:04:18.000000 mpctools-0.9.0/mpctools.egg-info/requires.txt
+-rw-rw-r--   0 s1238640  (1000) s1238640  (1000)        9 2022-11-16 13:04:18.000000 mpctools-0.9.0/mpctools.egg-info/top_level.txt
+-rw-rw-r--   0 s1238640  (1000) s1238640  (1000)       79 2022-11-16 13:04:18.000000 mpctools-0.9.0/setup.cfg
+-rw-rw-r--   0 s1238640  (1000) s1238640  (1000)     1560 2022-11-16 13:01:03.000000 mpctools-0.9.0/setup.py
```

### Comparing `mpctools-0.8.0/LICENSE` & `mpctools-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mpctools-0.8.0/PKG-INFO` & `mpctools-0.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: mpctools
-Version: 0.8.0
+Version: 0.9.0
 Summary: A set of tools and utilities for extending common libraries and providing parallel capabilities.
 Home-page: https://github.com/michael-camilleri/mpctools
 Author: Michael P. J. Camilleri
 Author-email: michael.p.camilleri@ed.ac.uk
 License: GNU GPL
-Download-URL: https://github.com/michael-camilleri/mpctools/archive/v_0800.tar.gz
+Download-URL: https://github.com/michael-camilleri/mpctools/archive/v_0900.tar.gz
 Keywords: extensions,parallel,utilities
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Classifier: Programming Language :: Python :: 3 :: Only
```

### Comparing `mpctools-0.8.0/README.md` & `mpctools-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `mpctools-0.8.0/mpctools/__init__.py` & `mpctools-0.9.0/mpctools/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 You should have received a copy of the GNU General Public License along with this program. If not,
 see http://www.gnu.org/licenses/.
 
 Author: Michael P. J. Camilleri
 """
 
 __author__ = "Michael P. J. Camilleri"
-__version__ = "0.8.0"
+__version__ = "0.9.0"
```

### Comparing `mpctools-0.8.0/mpctools/extensions/__init__.py` & `mpctools-0.9.0/mpctools/extensions/__init__.py`

 * *Files identical despite different names*

### Comparing `mpctools-0.8.0/mpctools/extensions/cvext.py` & `mpctools-0.9.0/mpctools/extensions/cvext.py`

 * *Files identical despite different names*

### Comparing `mpctools-0.8.0/mpctools/extensions/mplext.py` & `mpctools-0.9.0/mpctools/extensions/mplext.py`

 * *Files 1% similar despite different names*

```diff
@@ -193,27 +193,27 @@
         else:
             ax.set_yticks(np.arange(0.5, len(y_labels) + 0.5))
         ax.set_yticklabels(
             y_labels, rotation=y_rot, verticalalignment="center" if abs(y_rot - 45) > 25 else "bottom", fontsize=fs
         )
 
 
-def autolabel_bar(bars, labels=None, fs=12, ax=None):
+def autolabel_bar(bars, labels=None, fs=12, prec=3, ax=None):
     """
     Add a Text-Label to the top of each bar in a bar-chart.
 
     :param bars:  Rectangles returned by plot.bar()
     :param labels: Alternative labels to override with
     :param fs: Fontsize for text
     :param ax:     Axes on which to plot.
     """
     ax = utils.default(ax, plt.gca())
     for i, b in enumerate(bars):
         ax.annotate(
-            f'{b.get_height()}' if labels is None else labels[i],
+            f'{b.get_height():.{prec}f}' if labels is None else labels[i],
             xy=(b.get_x() + b.get_width() / 2, b.get_height()),
             xytext=(0, 5),
             textcoords="offset points",
             ha='center', va='bottom',
             fontsize=fs,
         )
```

### Comparing `mpctools-0.8.0/mpctools/extensions/npext.py` & `mpctools-0.9.0/mpctools/extensions/npext.py`

 * *Files 1% similar despite different names*

```diff
@@ -648,21 +648,17 @@
     :return:  Inverse Softmax
     """
     # Compute Log(X)
     log_x = np.log(x)
 
     # Branch on how we achieve uniqueness
     if enforce_unique is None:
-        return log_x - np.mean(
-            log_x, axis=-1, keepdims=True
-        )  # Eq. (7), substituting Eq. (8) for C.
+        return log_x - np.mean(log_x, axis=-1, keepdims=True)  # Eq7 substituting Eq8 for C
     else:
-        return log_x - np.expand_dims(
-            log_x[..., enforce_unique], -1
-        )  # Eq. (7), substituting Eq. (9) for C.
+        return log_x - np.expand_dims(log_x[..., enforce_unique], -1)  # Eq7 substituting Eq9 for C
 
 
 def conditional_entropy(emission, prior=None, base=None):
     """
     Compute the Conditional Entropy of a Joint Distribution over latent and conditioned (visible)
     variables. This only supports 2D Emissions (ie one latent variable and one visible)
```

### Comparing `mpctools-0.8.0/mpctools/extensions/pdext.py` & `mpctools-0.9.0/mpctools/extensions/pdext.py`

 * *Files identical despite different names*

### Comparing `mpctools-0.8.0/mpctools/extensions/skext.py` & `mpctools-0.9.0/mpctools/extensions/skext.py`

 * *Files 10% similar despite different names*

```diff
@@ -14,16 +14,19 @@
 """
 from scipy.cluster.hierarchy import linkage, dendrogram, fcluster
 from sklearn.calibration import CalibrationDisplay
 from sklearn import preprocessing as skpreproc
 from scipy.spatial.distance import squareform
 from mpctools.extensions import npext, utils
 from sklearn import metrics as skmetrics
+from scipy.special import softmax
 from sklearn.svm import SVC
+import torch.nn as tnn
 import numpy as np
+import torch
 
 
 class ThresholdedClassifier:
     """
     Simple wrapper which applies a threshold to a classifier.
 
     Currently, only works for Binary Classifiers
@@ -46,14 +49,18 @@
 
     def predict_proba(self, X):
         """
         Calls the underlying predict_proba() method for the classifier.
         """
         return self.__clf.predict_proba(X)
 
+    @property
+    def threshold(self):
+        return self.__thr
+
 
 class SVCProb:
     """
     Wrapper around the SVC Classifier to include a probability interpretation of the DF (as
     opposed to the CV-folds based estimation).
     This is less accurate but provides a rough estimate for ROC thresholds.
     """
@@ -250,14 +257,38 @@
     )
     idcs = [left]
     for i in right_split:
         idcs.append(right[i])
     return idcs
 
 
+def net_benefit_curve(y_true, y_score, pos_label=1, epsilon=1e-3):
+    """
+    Creates a Net-Benefit curve for various thresholds t.
+
+    It basically replicates sklearn.metrics.roc_curve
+
+    :param y_true:  Groundtruth labels
+    :param y_score: Classifier scores
+    :param pos_label: Which label to treat as positive
+    :param epsilon: replacement for 0 - threshold
+    :return:
+    """
+    # Get Statistics
+    N, pos, neg = len(y_true), (y_true == pos_label).sum(), (y_true != pos_label).sum()
+
+    # Compute Rates at different thresholds and subsequently net benefit
+    fpr, tpr, thr = skmetrics.roc_curve(y_true, y_score, pos_label=pos_label)
+    fpr, tpr, thr = np.flip(fpr)[:-1], np.flip(tpr)[:-1], np.flip(np.clip(thr, 0, 1-epsilon))[:-1]
+    nb = (tpr * pos / N) - (fpr * neg / N) * (thr / (1 - thr))
+
+    # Return
+    return nb, thr
+
+
 def mlp_complexity(mlp):
     """
     Computes the complexity (number of trainable parameters) of a MLP model
 
     :param mlp: Model to evaluate. This must have been fit (or at least seen some data)
     :return: Number of (scalars) to learn
     """
@@ -377,7 +408,91 @@
             ax=ax,
             labels=labels,
             leaf_rotation=x_rot,
             color_threshold=color,
             leaf_font_size=fs,
         )
         return self
+
+
+class LogitCalibrator(tnn.Module):
+    """
+    Implementation of Temperature scaling which conforms to sklearn framework
+    """
+    def __init__(self, classes=None, theta_init=1.0, lr=1e-4, max_iter=100):
+        """
+        Initialises the Model
+        :param theta_init: Initial value for scaling parameter
+        :param lr:  Learning rate
+        :param max_iter: Maximum number of iterations
+        """
+        # Call BaseClass
+        super(LogitCalibrator, self).__init__()
+
+        # Initialise some Parameters
+        self.theta = theta_init
+        self.__lr = lr
+        self.__max_iter = max_iter
+        self.classes_ = classes
+
+        # Torch requirements
+        self._theta = tnn.Parameter(torch.tensor([theta_init], dtype=torch.double))
+
+    def fit(self, X, y):
+        """
+        Fits the model on the training Data
+
+        :param X: The input logits
+        :param y: The output labels (one of L behaviours, 0-indexed)
+        """
+        # Update Class List
+        if self.classes_ is None:
+            self.classes_ = np.unique(y)
+        assert X.shape[1] == len(self.classes_), f'# Classes ({len(self.classes_)}) does not equal the size of the Logits ({X.shape[1]})'
+
+        # Start by transforming to tensors.
+        X, y = torch.tensor(X, dtype=torch.double), torch.tensor(y, dtype=torch.long)
+
+        # Define optimiser (and closure for it)
+        self.train()
+        optimiser = torch.optim.LBFGS(self.parameters(), lr=self.__lr, max_iter=self.__max_iter)
+        loss_func = tnn.NLLLoss()
+
+        def _optim_step():
+            optimiser.zero_grad()
+            loss = loss_func(self(X).log(), y)
+            loss.backward()
+            return loss
+
+        # Optimise Model
+        optimiser.step(_optim_step)
+
+        # Now get the parameters of interest
+        self.eval()
+        with torch.no_grad():
+            self.theta = self._theta.numpy()[0]
+
+        # Return self for chaining
+        return self
+
+    def predict_proba(self, X):
+        """
+        Predict Probabilities
+        """
+        return softmax(X / self.theta, axis=1)
+
+    def predict(self, X):
+        """
+        Predict Behaviour
+
+        Note, this is really a dummy, since the ordering does not change.
+        """
+        return np.argmax(X, axis=1)
+
+    def forward(self, x):
+        """
+        Internal function for optimisation only.
+
+        Computes a forward pass on x (a tensor of logits, of size [# Samples, # Labels])
+        """
+        return (x / self._theta).softmax(dim=1)
+
```

### Comparing `mpctools-0.8.0/mpctools/extensions/utils.py` & `mpctools-0.9.0/mpctools/extensions/utils.py`

 * *Files identical despite different names*

### Comparing `mpctools-0.8.0/mpctools/parallel/__init__.py` & `mpctools-0.9.0/mpctools/parallel/__init__.py`

 * *Files identical despite different names*

### Comparing `mpctools-0.8.0/mpctools/parallel/progress_bar.py` & `mpctools-0.9.0/mpctools/parallel/progress_bar.py`

 * *Files identical despite different names*

### Comparing `mpctools-0.8.0/mpctools/parallel/worker_handler.py` & `mpctools-0.9.0/mpctools/parallel/worker_handler.py`

 * *Files identical despite different names*

### Comparing `mpctools-0.8.0/mpctools.egg-info/PKG-INFO` & `mpctools-0.9.0/mpctools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: mpctools
-Version: 0.8.0
+Version: 0.9.0
 Summary: A set of tools and utilities for extending common libraries and providing parallel capabilities.
 Home-page: https://github.com/michael-camilleri/mpctools
 Author: Michael P. J. Camilleri
 Author-email: michael.p.camilleri@ed.ac.uk
 License: GNU GPL
-Download-URL: https://github.com/michael-camilleri/mpctools/archive/v_0800.tar.gz
+Download-URL: https://github.com/michael-camilleri/mpctools/archive/v_0900.tar.gz
 Keywords: extensions,parallel,utilities
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Classifier: Programming Language :: Python :: 3 :: Only
```

### Comparing `mpctools-0.8.0/mpctools.egg-info/SOURCES.txt` & `mpctools-0.9.0/mpctools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mpctools-0.8.0/setup.py` & `mpctools-0.9.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,26 +21,27 @@
         "deprecated",
         "lapsolver",
         "hotelling",
         "seaborn",
         "pandas",
         "pathos",
         "scipy",
+        "torch",
         "numpy",
         "numba",
     ],
     # Meta-Data
     author="Michael P. J. Camilleri",
     author_email="michael.p.camilleri@ed.ac.uk",
     description="A set of tools and utilities for extending common libraries and providing parallel"
                 " capabilities.",
     license="GNU GPL",
     keywords=["extensions", "parallel", "utilities"],
     url="https://github.com/michael-camilleri/mpctools",
-    download_url="https://github.com/michael-camilleri/mpctools/archive/v_0800.tar.gz",
+    download_url="https://github.com/michael-camilleri/mpctools/archive/v_0900.tar.gz",
     long_description=long_description,
     long_description_content_type="text/markdown",
     data_files=[("", ["LICENSE"])],
     include_package_data=True,
     # PyPi Data
     classifiers=[
         "Development Status :: 4 - Beta",
```

