# Comparing `tmp/rilacs-1.0.0.tar.gz` & `tmp/rilacs-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rilacs-1.0.0.tar", last modified: Wed Jan 12 06:21:23 2022, max compression
+gzip compressed data, was "rilacs-1.0.3.tar", last modified: Thu May 18 06:19:35 2023, max compression
```

## Comparing `rilacs-1.0.0.tar` & `rilacs-1.0.3.tar`

### file list

```diff
@@ -1,22 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-12 06:21:23.787828 rilacs-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (121)     1561 2022-01-12 06:21:17.000000 rilacs-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      279 2022-01-12 06:21:23.787828 rilacs-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2534 2022-01-12 06:21:17.000000 rilacs-1.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (121)      217 2022-01-12 06:21:17.000000 rilacs-1.0.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-12 06:21:23.783828 rilacs-1.0.0/rilacs/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-12 06:21:17.000000 rilacs-1.0.0/rilacs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2266 2022-01-12 06:21:17.000000 rilacs-1.0.0/rilacs/confseqs.py
--rw-r--r--   0 runner    (1001) docker     (121)     7361 2022-01-12 06:21:17.000000 rilacs-1.0.0/rilacs/incremental_audit.py
--rw-r--r--   0 runner    (1001) docker     (121)     4419 2022-01-12 06:21:17.000000 rilacs-1.0.0/rilacs/martingales.py
--rw-r--r--   0 runner    (1001) docker     (121)     4620 2022-01-12 06:21:17.000000 rilacs-1.0.0/rilacs/misc.py
--rw-r--r--   0 runner    (1001) docker     (121)     2415 2022-01-12 06:21:17.000000 rilacs-1.0.0/rilacs/plotting.py
--rw-r--r--   0 runner    (1001) docker     (121)      877 2022-01-12 06:21:17.000000 rilacs-1.0.0/rilacs/strategies.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-12 06:21:23.787828 rilacs-1.0.0/rilacs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      279 2022-01-12 06:21:23.000000 rilacs-1.0.0/rilacs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      362 2022-01-12 06:21:23.000000 rilacs-1.0.0/rilacs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-01-12 06:21:23.000000 rilacs-1.0.0/rilacs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-01-12 06:21:23.000000 rilacs-1.0.0/rilacs.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       20 2022-01-12 06:21:23.000000 rilacs-1.0.0/rilacs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        7 2022-01-12 06:21:23.000000 rilacs-1.0.0/rilacs.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-01-12 06:21:23.787828 rilacs-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      414 2022-01-12 06:21:17.000000 rilacs-1.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 06:19:35.873435 rilacs-1.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1561 2023-05-18 06:19:24.000000 rilacs-1.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2844 2023-05-18 06:19:35.873435 rilacs-1.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2552 2023-05-18 06:19:24.000000 rilacs-1.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-05-18 06:19:24.000000 rilacs-1.0.3/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 06:19:35.869435 rilacs-1.0.3/rilacs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 06:19:24.000000 rilacs-1.0.3/rilacs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2266 2023-05-18 06:19:24.000000 rilacs-1.0.3/rilacs/confseqs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7357 2023-05-18 06:19:24.000000 rilacs-1.0.3/rilacs/incremental_audit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4419 2023-05-18 06:19:24.000000 rilacs-1.0.3/rilacs/martingales.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4620 2023-05-18 06:19:24.000000 rilacs-1.0.3/rilacs/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2415 2023-05-18 06:19:24.000000 rilacs-1.0.3/rilacs/plotting.py
+-rw-r--r--   0 runner    (1001) docker     (123)      877 2023-05-18 06:19:24.000000 rilacs-1.0.3/rilacs/strategies.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 06:19:35.869435 rilacs-1.0.3/rilacs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2844 2023-05-18 06:19:35.000000 rilacs-1.0.3/rilacs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      464 2023-05-18 06:19:35.000000 rilacs-1.0.3/rilacs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 06:19:35.000000 rilacs-1.0.3/rilacs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 06:19:35.000000 rilacs-1.0.3/rilacs.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-18 06:19:35.000000 rilacs-1.0.3/rilacs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-18 06:19:35.000000 rilacs-1.0.3/rilacs.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-18 06:19:35.873435 rilacs-1.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-05-18 06:19:24.000000 rilacs-1.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 06:19:35.873435 rilacs-1.0.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1236 2023-05-18 06:19:24.000000 rilacs-1.0.3/tests/test_incremental_audit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2501 2023-05-18 06:19:24.000000 rilacs-1.0.3/tests/test_martingales.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2542 2023-05-18 06:19:24.000000 rilacs-1.0.3/tests/test_misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      910 2023-05-18 06:19:24.000000 rilacs-1.0.3/tests/test_strategies.py
```

### Comparing `rilacs-1.0.0/LICENSE` & `rilacs-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `rilacs-1.0.0/README.md` & `rilacs-1.0.3/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,30 +1,20 @@
 # RiLACS
 
-This package implements the martingales and confidence sequences from ["RiLACS: Risk-limiting audits via confidence sequences"](https://ian.waudbysmith.com/audit.pdf) and contains code for reproducing all of the plots therein.
-
+This package implements the martingales and confidence sequences from ["RiLACS: Risk-limiting audits via confidence sequences"](https://arxiv.org/pdf/2107.11323.pdf) and contains code for reproducing all of the plots therein.
 
 ## Installation
 
-### Dependencies
-
-First, you'll need to install the [boost C++ libraries](https://www.boost.org/). This can typically be done via your OS package manager but the package name can differ slightly across them. Here are some common ones:
-
-- MacOS+Homebrew: `boost`
-- MacOS+MacPorts: `boost`
-- Arch: `boost`
-- Debian/Ubuntu: `libboost-all-dev`
-- Fedora: `boost-devel`
-
-### Install from github via pip
+We currently support Python 3.7--3.10 on macOS (Intel/x86_64 and Apple Silicon) and Linux (x86_64).
 
 ```zsh
-pip install git+ssh://git@github.com/WannabeSmith/RiLACS.git
+pip install rilacs
 ```
-_Note: we have plans to release this on pypi in the future_
+
+Installation on other platforms may still be possible, but in that case, the dependency [confseq](github.com/gostevehoward/confseq) would need to be installed manually. If you would like to see an additional platform supported, please open an [issue at confseq](https://github.com/gostevehoward/confseq/issues), not RiLACS.
 
 ## Compute a confidence sequence
 
 ```python
 import numpy as np
 from rilacs.confseqs import sqKelly
 
@@ -34,15 +24,15 @@
 # Compute the confidence sequence
 l, u = sqKelly(x, N = 1000)
 ```
 
 ## Run unit tests
 ```zsh
 # Clone the repository 
-git clone git@github.com:WannabeSmith/RiLACS.git
+git clone https://github.com/WannabeSmith/RiLACS.git
 
 # Run unit tests via pytest
 pytest RiLACS
 ```
 
 ## Reproduce the paper's plots
 
@@ -69,13 +59,23 @@
 The `canada_audit` folder contains code to produce a web application which allows for interactive auditing of Canadian ridings in the 2019 federal election.
 
 For more details, view the README in [`canada_audit`](./canada_audit)
 
 ![audit](https://ian.waudbysmith.com/audit_demo_quick.gif)
 
 ## Contributing
-If you find a bug, please do [open an issue](https://github.com/wannabesmith/RiLACS/issues) and we'll try to fix it as soon as possible.
 
-If you want to add a feature or have other suggestions, feel free to reach out [via email](mailto:ianws@cmu.edu) or simply submit a [pull request](https://github.com/WannabeSmith/RiLACS/pulls)!
+If you find a bug, please [open an issue](https://github.com/wannabesmith/RiLACS/issues) and we'll try to fix it as soon as possible.
+
+## Citing
+
+The algorithms in this codebase are based on "RiLACS: Risk-limiting audits via confidence sequences" by Ian Waudby-Smith, Philip B. Stark, and Aaditya Ramdas. The BibTeX entry is provided here.
+
+@inproceedings{waudby2021rilacs,
+  title={RiLACS: Risk Limiting Audits via Confidence Sequences},
+  author={Waudby-Smith, Ian and Stark, Philip B and Ramdas, Aaditya},
+  booktitle={International Joint Conference on Electronic Voting},
+  pages={124--139},
+  year={2021},
+  organization={Springer}
+}
 
-## Credits
-The algorithms in this codebase were derived by [Ian Waudby-Smith](https://ian.waudbysmith.com), [Philip B. Stark](https://www.stat.berkeley.edu/~stark/), and [Aaditya Ramdas](http://stat.cmu.edu/~aramdas).
```

### Comparing `rilacs-1.0.0/rilacs/confseqs.py` & `rilacs-1.0.3/rilacs/confseqs.py`

 * *Files identical despite different names*

### Comparing `rilacs-1.0.0/rilacs/incremental_audit.py` & `rilacs-1.0.3/rilacs/incremental_audit.py`

 * *Files 0% similar despite different names*

```diff
@@ -152,15 +152,15 @@
         self.mu_denominator += l * (1 + (self.t - 1) / (self.N - self.t + 1))
         self.mu = self.mu_numerator / self.mu_denominator
 
         return self.mu
 
     def _update_margin(self, ballot):
         l = self._get_lambda(self.t)
-        self.margin_numerator += l ** 2 / 8
+        self.margin_numerator += l**2 / 8
         self.margin_denominator += l * (1 + (self.t - 1) / (self.N - self.t + 1))
         self.margin = self.margin_numerator / self.margin_denominator
         return self.margin
 
     def _get_lambda(self, t):
         return np.minimum(np.sqrt(8 * np.log(1 / self.alpha) / t / np.log(t + 1)), 1)
 
@@ -197,15 +197,15 @@
         self.mu_denominator += l * (1 + (self.t - 1) / (self.N - self.t + 1))
         self.mu = self.mu_numerator / self.mu_denominator
 
         return self.mu
 
     def _update_margin(self, ballot):
         l = self._get_lambda(self.t)
-        self.margin_numerator += l ** 2 / 8
+        self.margin_numerator += l**2 / 8
         self.margin_denominator += l * (1 + (self.t - 1) / (self.N - self.t + 1))
         self.margin = self.margin_numerator / self.margin_denominator
         return self.margin
 
     def _get_lambda(self, t):
         return np.minimum(np.sqrt(8 * np.log(1 / self.alpha) / t / np.log(t + 1)), 1)
```

### Comparing `rilacs-1.0.0/rilacs/martingales.py` & `rilacs-1.0.3/rilacs/martingales.py`

 * *Files identical despite different names*

### Comparing `rilacs-1.0.0/rilacs/misc.py` & `rilacs-1.0.3/rilacs/misc.py`

 * *Files identical despite different names*

### Comparing `rilacs-1.0.0/rilacs/plotting.py` & `rilacs-1.0.3/rilacs/plotting.py`

 * *Files identical despite different names*

### Comparing `rilacs-1.0.0/rilacs/strategies.py` & `rilacs-1.0.3/rilacs/strategies.py`

 * *Files identical despite different names*

