# Comparing `tmp/digital-experiments-1.1.4.tar.gz` & `tmp/digital-experiments-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "digital-experiments-1.1.4.tar", last modified: Wed May 17 16:02:17 2023, max compression
+gzip compressed data, was "digital-experiments-1.2.0.tar", last modified: Thu May 18 20:03:03 2023, max compression
```

## Comparing `digital-experiments-1.1.4.tar` & `digital-experiments-1.2.0.tar`

### file list

```diff
@@ -1,44 +1,48 @@
-drwxr-xr-x   0 john       (504) staff       (20)        0 2023-05-17 16:02:17.805327 digital-experiments-1.1.4/
--rw-r--r--   0 john       (504) staff       (20)     1051 2022-11-18 07:34:19.000000 digital-experiments-1.1.4/LICENSE
--rw-r--r--   0 john       (504) staff       (20)     2642 2023-05-17 16:02:17.805166 digital-experiments-1.1.4/PKG-INFO
--rw-r--r--   0 john       (504) staff       (20)     1008 2023-03-29 15:42:00.000000 digital-experiments-1.1.4/README.md
--rw-r--r--   0 john       (504) staff       (20)     1321 2023-05-17 16:01:49.000000 digital-experiments-1.1.4/pyproject.toml
--rw-r--r--   0 john       (504) staff       (20)       38 2023-05-17 16:02:17.805375 digital-experiments-1.1.4/setup.cfg
-drwxr-xr-x   0 john       (504) staff       (20)        0 2023-05-17 16:02:17.799152 digital-experiments-1.1.4/src/
-drwxr-xr-x   0 john       (504) staff       (20)        0 2023-05-17 16:02:17.801814 digital-experiments-1.1.4/src/digital_experiments/
--rw-r--r--   0 john       (504) staff       (20)      138 2023-05-17 16:01:49.000000 digital-experiments-1.1.4/src/digital_experiments/__init__.py
--rw-r--r--   0 john       (504) staff       (20)     6877 2023-05-17 15:48:49.000000 digital-experiments-1.1.4/src/digital_experiments/backends.py
--rw-r--r--   0 john       (504) staff       (20)     2649 2023-05-17 16:01:39.000000 digital-experiments-1.1.4/src/digital_experiments/control_center.py
--rw-r--r--   0 john       (504) staff       (20)     4377 2023-05-17 15:50:20.000000 digital-experiments-1.1.4/src/digital_experiments/experiment.py
--rw-r--r--   0 john       (504) staff       (20)      402 2023-03-29 15:42:00.000000 digital-experiments-1.1.4/src/digital_experiments/inspection.py
--rw-r--r--   0 john       (504) staff       (20)     4450 2023-04-04 08:33:50.000000 digital-experiments-1.1.4/src/digital_experiments/minimize.py
--rw-r--r--   0 john       (504) staff       (20)      637 2023-03-29 15:42:00.000000 digital-experiments-1.1.4/src/digital_experiments/observation.py
--rw-r--r--   0 john       (504) staff       (20)      735 2023-05-10 08:20:22.000000 digital-experiments-1.1.4/src/digital_experiments/pretty.py
--rw-r--r--   0 john       (504) staff       (20)     2581 2023-05-09 14:17:13.000000 digital-experiments-1.1.4/src/digital_experiments/querying.py
-drwxr-xr-x   0 john       (504) staff       (20)        0 2023-05-17 16:02:17.803114 digital-experiments-1.1.4/src/digital_experiments/search/
--rw-r--r--   0 john       (504) staff       (20)     2897 2023-03-29 15:42:00.000000 digital-experiments-1.1.4/src/digital_experiments/search/skopt_suggest.py
--rw-r--r--   0 john       (504) staff       (20)     5381 2023-03-29 15:42:00.000000 digital-experiments-1.1.4/src/digital_experiments/search/space.py
--rw-r--r--   0 john       (504) staff       (20)     4218 2023-04-03 14:30:06.000000 digital-experiments-1.1.4/src/digital_experiments/search/suggest.py
--rw-r--r--   0 john       (504) staff       (20)     1682 2023-05-17 15:42:42.000000 digital-experiments-1.1.4/src/digital_experiments/timing.py
--rw-r--r--   0 john       (504) staff       (20)     5211 2023-05-17 15:42:42.000000 digital-experiments-1.1.4/src/digital_experiments/util.py
--rw-r--r--   0 john       (504) staff       (20)     3464 2023-03-29 15:42:00.000000 digital-experiments-1.1.4/src/digital_experiments/version_control.py
-drwxr-xr-x   0 john       (504) staff       (20)        0 2023-05-17 16:02:17.802676 digital-experiments-1.1.4/src/digital_experiments.egg-info/
--rw-r--r--   0 john       (504) staff       (20)     2642 2023-05-17 16:02:17.000000 digital-experiments-1.1.4/src/digital_experiments.egg-info/PKG-INFO
--rw-r--r--   0 john       (504) staff       (20)     1147 2023-05-17 16:02:17.000000 digital-experiments-1.1.4/src/digital_experiments.egg-info/SOURCES.txt
--rw-r--r--   0 john       (504) staff       (20)        1 2023-05-17 16:02:17.000000 digital-experiments-1.1.4/src/digital_experiments.egg-info/dependency_links.txt
--rw-r--r--   0 john       (504) staff       (20)      160 2023-05-17 16:02:17.000000 digital-experiments-1.1.4/src/digital_experiments.egg-info/requires.txt
--rw-r--r--   0 john       (504) staff       (20)       20 2023-05-17 16:02:17.000000 digital-experiments-1.1.4/src/digital_experiments.egg-info/top_level.txt
-drwxr-xr-x   0 john       (504) staff       (20)        0 2023-05-17 16:02:17.804949 digital-experiments-1.1.4/tests/
--rw-r--r--   0 john       (504) staff       (20)     2083 2023-05-17 11:01:07.000000 digital-experiments-1.1.4/tests/test_backends.py
--rw-r--r--   0 john       (504) staff       (20)      844 2023-05-17 15:42:42.000000 digital-experiments-1.1.4/tests/test_control_center.py
--rw-r--r--   0 john       (504) staff       (20)     2099 2023-05-17 11:01:07.000000 digital-experiments-1.1.4/tests/test_experiment.py
--rw-r--r--   0 john       (504) staff       (20)      391 2023-05-17 11:01:07.000000 digital-experiments-1.1.4/tests/test_inspection.py
--rw-r--r--   0 john       (504) staff       (20)      632 2023-03-29 15:42:00.000000 digital-experiments-1.1.4/tests/test_minimize.py
--rw-r--r--   0 john       (504) staff       (20)      309 2023-05-17 11:01:07.000000 digital-experiments-1.1.4/tests/test_observation.py
--rw-r--r--   0 john       (504) staff       (20)      613 2023-05-10 08:20:22.000000 digital-experiments-1.1.4/tests/test_pretty.py
--rw-r--r--   0 john       (504) staff       (20)     1580 2023-05-09 14:17:13.000000 digital-experiments-1.1.4/tests/test_querying.py
--rw-r--r--   0 john       (504) staff       (20)     1596 2023-03-29 15:42:00.000000 digital-experiments-1.1.4/tests/test_space.py
--rw-r--r--   0 john       (504) staff       (20)     2188 2023-04-04 09:25:29.000000 digital-experiments-1.1.4/tests/test_suggest.py
--rw-r--r--   0 john       (504) staff       (20)      682 2023-05-17 15:42:42.000000 digital-experiments-1.1.4/tests/test_timing.py
--rw-r--r--   0 john       (504) staff       (20)     2820 2023-05-17 15:42:42.000000 digital-experiments-1.1.4/tests/test_util.py
--rw-r--r--   0 john       (504) staff       (20)     2397 2023-05-17 11:01:07.000000 digital-experiments-1.1.4/tests/test_version_control.py
+drwxr-xr-x   0 john       (504) staff       (20)        0 2023-05-18 20:03:03.985927 digital-experiments-1.2.0/
+-rw-r--r--   0 john       (504) staff       (20)     1051 2022-11-18 07:34:19.000000 digital-experiments-1.2.0/LICENSE
+-rw-r--r--   0 john       (504) staff       (20)     2642 2023-05-18 20:03:03.985789 digital-experiments-1.2.0/PKG-INFO
+-rw-r--r--   0 john       (504) staff       (20)     1008 2023-03-29 15:42:00.000000 digital-experiments-1.2.0/README.md
+-rw-r--r--   0 john       (504) staff       (20)     1321 2023-05-18 20:02:54.000000 digital-experiments-1.2.0/pyproject.toml
+-rw-r--r--   0 john       (504) staff       (20)       38 2023-05-18 20:03:03.985974 digital-experiments-1.2.0/setup.cfg
+drwxr-xr-x   0 john       (504) staff       (20)        0 2023-05-18 20:03:03.979175 digital-experiments-1.2.0/src/
+drwxr-xr-x   0 john       (504) staff       (20)        0 2023-05-18 20:03:03.981459 digital-experiments-1.2.0/src/digital_experiments/
+-rw-r--r--   0 john       (504) staff       (20)      138 2023-05-18 20:02:54.000000 digital-experiments-1.2.0/src/digital_experiments/__init__.py
+-rw-r--r--   0 john       (504) staff       (20)     1758 2023-05-18 14:04:48.000000 digital-experiments-1.2.0/src/digital_experiments/automate.py
+-rw-r--r--   0 john       (504) staff       (20)     6877 2023-05-17 15:48:49.000000 digital-experiments-1.2.0/src/digital_experiments/backends.py
+-rw-r--r--   0 john       (504) staff       (20)     2649 2023-05-17 16:01:39.000000 digital-experiments-1.2.0/src/digital_experiments/control_center.py
+-rw-r--r--   0 john       (504) staff       (20)     2924 2023-05-18 19:58:54.000000 digital-experiments-1.2.0/src/digital_experiments/data.py
+-rw-r--r--   0 john       (504) staff       (20)     4377 2023-05-17 15:50:20.000000 digital-experiments-1.2.0/src/digital_experiments/experiment.py
+-rw-r--r--   0 john       (504) staff       (20)      402 2023-03-29 15:42:00.000000 digital-experiments-1.2.0/src/digital_experiments/inspection.py
+-rw-r--r--   0 john       (504) staff       (20)      637 2023-03-29 15:42:00.000000 digital-experiments-1.2.0/src/digital_experiments/observation.py
+-rw-r--r--   0 john       (504) staff       (20)      735 2023-05-10 08:20:22.000000 digital-experiments-1.2.0/src/digital_experiments/pretty.py
+-rw-r--r--   0 john       (504) staff       (20)     2581 2023-05-09 14:17:13.000000 digital-experiments-1.2.0/src/digital_experiments/querying.py
+drwxr-xr-x   0 john       (504) staff       (20)        0 2023-05-18 20:03:03.983045 digital-experiments-1.2.0/src/digital_experiments/search/
+-rw-r--r--   0 john       (504) staff       (20)     3354 2023-05-18 14:04:45.000000 digital-experiments-1.2.0/src/digital_experiments/search/distributions.py
+-rw-r--r--   0 john       (504) staff       (20)     2896 2023-05-18 14:04:45.000000 digital-experiments-1.2.0/src/digital_experiments/search/skopt_suggest.py
+-rw-r--r--   0 john       (504) staff       (20)     2245 2023-05-18 14:04:45.000000 digital-experiments-1.2.0/src/digital_experiments/search/space.py
+-rw-r--r--   0 john       (504) staff       (20)     5756 2023-05-18 14:04:45.000000 digital-experiments-1.2.0/src/digital_experiments/search/suggest.py
+-rw-r--r--   0 john       (504) staff       (20)     1682 2023-05-17 15:42:42.000000 digital-experiments-1.2.0/src/digital_experiments/timing.py
+-rw-r--r--   0 john       (504) staff       (20)     5440 2023-05-18 14:04:45.000000 digital-experiments-1.2.0/src/digital_experiments/util.py
+-rw-r--r--   0 john       (504) staff       (20)     3464 2023-03-29 15:42:00.000000 digital-experiments-1.2.0/src/digital_experiments/version_control.py
+drwxr-xr-x   0 john       (504) staff       (20)        0 2023-05-18 20:03:03.982466 digital-experiments-1.2.0/src/digital_experiments.egg-info/
+-rw-r--r--   0 john       (504) staff       (20)     2642 2023-05-18 20:03:03.000000 digital-experiments-1.2.0/src/digital_experiments.egg-info/PKG-INFO
+-rw-r--r--   0 john       (504) staff       (20)     1274 2023-05-18 20:03:03.000000 digital-experiments-1.2.0/src/digital_experiments.egg-info/SOURCES.txt
+-rw-r--r--   0 john       (504) staff       (20)        1 2023-05-18 20:03:03.000000 digital-experiments-1.2.0/src/digital_experiments.egg-info/dependency_links.txt
+-rw-r--r--   0 john       (504) staff       (20)      160 2023-05-18 20:03:03.000000 digital-experiments-1.2.0/src/digital_experiments.egg-info/requires.txt
+-rw-r--r--   0 john       (504) staff       (20)       20 2023-05-18 20:03:03.000000 digital-experiments-1.2.0/src/digital_experiments.egg-info/top_level.txt
+drwxr-xr-x   0 john       (504) staff       (20)        0 2023-05-18 20:03:03.985612 digital-experiments-1.2.0/tests/
+-rw-r--r--   0 john       (504) staff       (20)      482 2023-05-18 14:04:45.000000 digital-experiments-1.2.0/tests/test_automate.py
+-rw-r--r--   0 john       (504) staff       (20)     2135 2023-05-18 14:04:45.000000 digital-experiments-1.2.0/tests/test_backends.py
+-rw-r--r--   0 john       (504) staff       (20)     1122 2023-05-18 14:04:45.000000 digital-experiments-1.2.0/tests/test_control_center.py
+-rw-r--r--   0 john       (504) staff       (20)     1784 2023-05-18 20:02:10.000000 digital-experiments-1.2.0/tests/test_data.py
+-rw-r--r--   0 john       (504) staff       (20)     1395 2023-05-18 14:04:45.000000 digital-experiments-1.2.0/tests/test_distributions.py
+-rw-r--r--   0 john       (504) staff       (20)     2099 2023-05-17 11:01:07.000000 digital-experiments-1.2.0/tests/test_experiment.py
+-rw-r--r--   0 john       (504) staff       (20)      391 2023-05-17 11:01:07.000000 digital-experiments-1.2.0/tests/test_inspection.py
+-rw-r--r--   0 john       (504) staff       (20)      309 2023-05-17 11:01:07.000000 digital-experiments-1.2.0/tests/test_observation.py
+-rw-r--r--   0 john       (504) staff       (20)      613 2023-05-10 08:20:22.000000 digital-experiments-1.2.0/tests/test_pretty.py
+-rw-r--r--   0 john       (504) staff       (20)     1912 2023-05-18 14:04:45.000000 digital-experiments-1.2.0/tests/test_querying.py
+-rw-r--r--   0 john       (504) staff       (20)      712 2023-05-18 14:04:45.000000 digital-experiments-1.2.0/tests/test_space.py
+-rw-r--r--   0 john       (504) staff       (20)     3179 2023-05-18 14:04:45.000000 digital-experiments-1.2.0/tests/test_suggest.py
+-rw-r--r--   0 john       (504) staff       (20)      682 2023-05-17 15:42:42.000000 digital-experiments-1.2.0/tests/test_timing.py
+-rw-r--r--   0 john       (504) staff       (20)     2820 2023-05-17 15:42:42.000000 digital-experiments-1.2.0/tests/test_util.py
+-rw-r--r--   0 john       (504) staff       (20)     2830 2023-05-18 14:04:45.000000 digital-experiments-1.2.0/tests/test_version_control.py
```

### Comparing `digital-experiments-1.1.4/LICENSE` & `digital-experiments-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `digital-experiments-1.1.4/PKG-INFO` & `digital-experiments-1.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: digital-experiments
-Version: 1.1.4
+Version: 1.2.0
 Summary: Keep track of digital experiments.
 Author-email: John Gardner <gardner.john97@gmail.com>
 License: Copyright 2022 John Gardner
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
```

### Comparing `digital-experiments-1.1.4/README.md` & `digital-experiments-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `digital-experiments-1.1.4/pyproject.toml` & `digital-experiments-1.2.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "digital-experiments"
-version = "1.1.4"
+version = "1.2.0"
 description = "Keep track of digital experiments."
 readme = "README.md"
 authors = [{ name = "John Gardner", email = "gardner.john97@gmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
@@ -41,15 +41,15 @@
     "pytest-cov",
 ]
 
 [project.urls]
 Homepage = "https://github.com/jla-gardner/digital-experiments"
 
 [tool.bumpver]
-current_version = "1.1.4"
+current_version = "1.2.0"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "Bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 push = false
 
 [tool.bumpver.file_patterns]
```

### Comparing `digital-experiments-1.1.4/src/digital_experiments/backends.py` & `digital-experiments-1.2.0/src/digital_experiments/backends.py`

 * *Files identical despite different names*

### Comparing `digital-experiments-1.1.4/src/digital_experiments/control_center.py` & `digital-experiments-1.2.0/src/digital_experiments/control_center.py`

 * *Files identical despite different names*

### Comparing `digital-experiments-1.1.4/src/digital_experiments/experiment.py` & `digital-experiments-1.2.0/src/digital_experiments/experiment.py`

 * *Files identical despite different names*

### Comparing `digital-experiments-1.1.4/src/digital_experiments/observation.py` & `digital-experiments-1.2.0/src/digital_experiments/observation.py`

 * *Files identical despite different names*

### Comparing `digital-experiments-1.1.4/src/digital_experiments/pretty.py` & `digital-experiments-1.2.0/src/digital_experiments/pretty.py`

 * *Files identical despite different names*

### Comparing `digital-experiments-1.1.4/src/digital_experiments/querying.py` & `digital-experiments-1.2.0/src/digital_experiments/querying.py`

 * *Files identical despite different names*

### Comparing `digital-experiments-1.1.4/src/digital_experiments/search/skopt_suggest.py` & `digital-experiments-1.2.0/src/digital_experiments/search/skopt_suggest.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,34 +1,31 @@
 from typing import Dict, List, Union
 
 import numpy as np
-from pandas import Categorical
 from skopt import Optimizer as SKOptimizer
 from skopt import space as SK
 
-from digital_experiments.search.space import (
+from digital_experiments.search.distributions import (
     Categorical,
     Distribution,
     LogUniform,
-    Space,
     Uniform,
-    to_space,
 )
-from digital_experiments.search.suggest import Point, Step, Suggester
+from digital_experiments.search.space import Point, Space, to_space
+from digital_experiments.search.suggest import Step, Suggester
 
 
 class SKSuggester(Suggester):
     def __init__(
         self,
         space: Union[Dict[str, Distribution], Space],
         previous_steps: List[Step] = None,
         n_explore_steps: int = 10,
         seed: int = 42,
     ) -> None:
-
         super().__init__(space, previous_steps)
 
         self.tells_since_suggest = len(self.previous_steps)
         self.n_explore_steps = n_explore_steps
         self.random = np.random.RandomState(seed=seed).random
 
         _skopt_dimensions = to_skopt_dims(space)
@@ -48,27 +45,25 @@
         n_points_so_far = len(self.previous_steps)
         if n_points_so_far < self.n_explore_steps:
             return self.explore_step()
         else:
             return self.exploit_step()
 
     def explore_step(self) -> Point:
-        return self.space.random_sample(n=1, generator=self.random)
+        return self.space.random_sample(random_number_generator=self.random)
 
     def exploit_step(self) -> Point:
         values = self.optimizer.ask()
         return {key: value for key, value in zip(self.space.keys(), values)}
 
     def _fit_if_necessary(self):
         if self.tells_since_suggest == 0:
             return
 
-        for i, step in enumerate(
-            self.previous_steps[-self.tells_since_suggest :]
-        ):
+        for i, step in enumerate(self.previous_steps[-self.tells_since_suggest :]):
             values = list(step.point.values())
             observation = step.observation
 
             # only fit the underlying model on the last step
             fit_model = i == self.tells_since_suggest - 1
             self.optimizer.tell(values, observation, fit=fit_model)
```

### Comparing `digital-experiments-1.1.4/src/digital_experiments/timing.py` & `digital-experiments-1.2.0/src/digital_experiments/timing.py`

 * *Files identical despite different names*

### Comparing `digital-experiments-1.1.4/src/digital_experiments/util.py` & `digital-experiments-1.2.0/src/digital_experiments/util.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import inspect
+import random
 import sys
 from contextlib import contextmanager
 from datetime import datetime
 from pathlib import Path
 from typing import Any, Dict, Union
 
 from filelock import FileLock
@@ -206,7 +207,19 @@
 
     # now we need to add all the keys from d2 that are not in d1
     for k, v in d2.items():
         if k not in d1:
             new_dict[k] = v
 
     return new_dict
+
+
+def is_iterable(obj):
+    """
+    check if an object is iterable
+    """
+    return hasattr(obj, "__iter__")
+
+
+def get_random_number():
+    """returns a random number between 0 and 1"""
+    return random.random()
```

### Comparing `digital-experiments-1.1.4/src/digital_experiments/version_control.py` & `digital-experiments-1.2.0/src/digital_experiments/version_control.py`

 * *Files identical despite different names*

### Comparing `digital-experiments-1.1.4/src/digital_experiments.egg-info/PKG-INFO` & `digital-experiments-1.2.0/src/digital_experiments.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: digital-experiments
-Version: 1.1.4
+Version: 1.2.0
 Summary: Keep track of digital experiments.
 Author-email: John Gardner <gardner.john97@gmail.com>
 License: Copyright 2022 John Gardner
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
```

### Comparing `digital-experiments-1.1.4/src/digital_experiments.egg-info/SOURCES.txt` & `digital-experiments-1.2.0/src/digital_experiments.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,35 +1,39 @@
 LICENSE
 README.md
 pyproject.toml
 src/digital_experiments/__init__.py
+src/digital_experiments/automate.py
 src/digital_experiments/backends.py
 src/digital_experiments/control_center.py
+src/digital_experiments/data.py
 src/digital_experiments/experiment.py
 src/digital_experiments/inspection.py
-src/digital_experiments/minimize.py
 src/digital_experiments/observation.py
 src/digital_experiments/pretty.py
 src/digital_experiments/querying.py
 src/digital_experiments/timing.py
 src/digital_experiments/util.py
 src/digital_experiments/version_control.py
 src/digital_experiments.egg-info/PKG-INFO
 src/digital_experiments.egg-info/SOURCES.txt
 src/digital_experiments.egg-info/dependency_links.txt
 src/digital_experiments.egg-info/requires.txt
 src/digital_experiments.egg-info/top_level.txt
+src/digital_experiments/search/distributions.py
 src/digital_experiments/search/skopt_suggest.py
 src/digital_experiments/search/space.py
 src/digital_experiments/search/suggest.py
+tests/test_automate.py
 tests/test_backends.py
 tests/test_control_center.py
+tests/test_data.py
+tests/test_distributions.py
 tests/test_experiment.py
 tests/test_inspection.py
-tests/test_minimize.py
 tests/test_observation.py
 tests/test_pretty.py
 tests/test_querying.py
 tests/test_space.py
 tests/test_suggest.py
 tests/test_timing.py
 tests/test_util.py
```

### Comparing `digital-experiments-1.1.4/tests/test_backends.py` & `digital-experiments-1.2.0/tests/test_backends.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from digital_experiments import experiment
 from digital_experiments.backends import (
     Backend,
     available_backends,
     backend_from_type,
     this_is_a_backend,
 )
+from digital_experiments.inspection import code_for
 from digital_experiments.observation import Observation
 
 
 def test_incomplete_subclassing():
     """
     A backend must implement save and all_observations
     """
```

### Comparing `digital-experiments-1.1.4/tests/test_experiment.py` & `digital-experiments-1.2.0/tests/test_experiment.py`

 * *Files identical despite different names*

### Comparing `digital-experiments-1.1.4/tests/test_pretty.py` & `digital-experiments-1.2.0/tests/test_pretty.py`

 * *Files identical despite different names*

### Comparing `digital-experiments-1.1.4/tests/test_querying.py` & `digital-experiments-1.2.0/tests/test_querying.py`

 * *Files 10% similar despite different names*

```diff
@@ -55,7 +55,16 @@
         assert len(df) == 0, "Should have no rows"
 
     add(1, 2)
     add(1, 3)
 
     df = add.to_dataframe()
     assert len(df) == 2, "Should have two rows"
+
+    df = add.to_dataframe(config={"b": 2})
+    assert len(df) == 1, "Should have one row"
+
+    df = add.to_dataframe(include_id=False)
+    assert "id" not in df.columns, "Should not have id column"
+
+    df = add.to_dataframe(include_metadata=True)
+    assert not df.filter(regex="metadata.*").empty, "Should have metadata columns"
```

### Comparing `digital-experiments-1.1.4/tests/test_space.py` & `digital-experiments-1.2.0/tests/test_distributions.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,58 +1,50 @@
-from digital_experiments.search.space import (
+from digital_experiments.search.distributions import (
     Categorical,
     LogUniform,
-    Space,
     Uniform,
+    convert_from_shorthand,
 )
 
 
 def test_uniform():
     x = Uniform(3.6, 10.7)
 
     s = x.random_sample()
-    unit_s = x.inverse_transform(s)
+    unit_s = x.transform_to_unit_range(s)
 
     assert x.contains(s), "Sampled value is not in the distribution"
     assert 0 <= unit_s <= 1, "Unit value is not in the unit range"
 
     assert x.contains(3.6), "Lower bound is not in the distribution"
     assert x.contains(10.7), "Upper bound is not in the distribution"
     assert not x.contains(3.5)
 
 
 def test_log_uniform():
     x = LogUniform(1e-3, 1e4)
 
     s = x.random_sample()
-    unit_s = x.inverse_transform(s)
+    unit_s = x.transform_to_unit_range(s)
 
     assert x.contains(s), "Sampled value is not in the distribution"
     assert 0 <= unit_s <= 1, "Unit value is not in the unit range"
 
 
 def test_categorical():
     vals = ["a", "b", "c"]
     x = Categorical(vals)
 
     s = x.random_sample()
-    unit_s = x.inverse_transform(s)
+    unit_s = x.transform_to_unit_range(s)
 
     assert s in vals, "Sampled value is not in the distribution"
     assert x.contains(s), "Sampled value is not in the distribution"
     assert 0 <= unit_s <= 1, "Unit value is not in the unit range"
 
 
-def test_space():
-    space = Space(
-        x=Uniform(3.6, 10.7),
-        y=LogUniform(1e-3, 1e4),
-        z=Categorical(["a", "b", "c"]),
-    )
-
-    s = space.random_sample()
-    unit_s = space.inverse_transform(s)
-
-    assert space.contains(s), "Sampled value is not in the distribution"
-    for k, v in s.items():
-        assert space[k].contains(v), "Sampled value is not in the distribution"
-    assert 0 <= unit_s[k] <= 1, "Unit value is not in the unit range"
+def test_from_shorthand():
+    dims = {"foo": [1, 2, 3], "bar": Uniform(0, 1)}
+    new_dims = convert_from_shorthand(dims)
+
+    assert isinstance(new_dims["foo"], Categorical)
+    assert isinstance(new_dims["bar"], Uniform)
```

### Comparing `digital-experiments-1.1.4/tests/test_timing.py` & `digital-experiments-1.2.0/tests/test_timing.py`

 * *Files identical despite different names*

### Comparing `digital-experiments-1.1.4/tests/test_util.py` & `digital-experiments-1.2.0/tests/test_util.py`

 * *Files identical despite different names*

### Comparing `digital-experiments-1.1.4/tests/test_version_control.py` & `digital-experiments-1.2.0/tests/test_version_control.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 import shutil
 from pathlib import Path
 
 from digital_experiments import experiment
+from digital_experiments.inspection import code_for
 from digital_experiments.version_control import (
     current_max_version,
     for_version,
     get_all_versions,
     get_backend_for,
+    get_or_create_backend_for,
     latest_version,
 )
 
 
 def _get_root_for(experiment):
     return experiment._backend.home.parent
 
@@ -70,7 +72,20 @@
     assert backend is not None, "Should have a backend"
 
     backend = get_backend_for(root, for_version("version-1"))
     assert backend is not None, "Should have a backend"
 
     backend = get_backend_for(root, for_version("version-2"))
     assert backend is None, "Should not have a backend"
+
+
+def test_get_or_create_backend_for(tmp_path):
+    @experiment(absolute_root=tmp_path, backend="csv")
+    def add(a, b):
+        return a + b
+
+    # get the code
+    code = code_for(add._experiment)
+    backend_str = "csv"
+
+    backend = get_or_create_backend_for(tmp_path, code, backend_str)
+    assert backend is not None, "Should have a backend"
```

