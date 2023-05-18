# Comparing `tmp/brown_clustering-0.1.4.tar.gz` & `tmp/brown_clustering-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/BrownClustering/BrownClustering/dist/tmp0ue0iz95/brown_clustering-0.1.4.tar", last modified: Tue Nov 30 15:18:42 2021, max compression
+gzip compressed data, was "/home/runner/work/BrownClustering/BrownClustering/dist/.tmp-6nfmdbfh/brown_clustering-0.1.6.tar", last modified: Thu May 18 11:58:16 2023, max compression
```

## Comparing `brown_clustering-0.1.4.tar` & `brown_clustering-0.1.6.tar`

### file list

```diff
@@ -1,18 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-11-30 15:18:42.000000 brown_clustering-0.1.4/
--rw-r--r--   0 runner    (1001) docker     (116)      839 2021-11-30 15:18:30.000000 brown_clustering-0.1.4/setup.py
--rw-r--r--   0 runner    (1001) docker     (116)     4209 2021-11-30 15:18:42.000000 brown_clustering-0.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     1208 2021-11-30 15:18:30.000000 brown_clustering-0.1.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (116)      316 2021-11-30 15:18:42.000000 brown_clustering-0.1.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-11-30 15:18:42.000000 brown_clustering-0.1.4/brown_clustering/
--rw-r--r--   0 runner    (1001) docker     (116)      155 2021-11-30 15:18:30.000000 brown_clustering-0.1.4/brown_clustering/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     2836 2021-11-30 15:18:30.000000 brown_clustering-0.1.4/brown_clustering/data.py
--rw-r--r--   0 runner    (1001) docker     (116)      365 2021-11-30 15:18:30.000000 brown_clustering-0.1.4/brown_clustering/defaultvaluedict.py
--rw-r--r--   0 runner    (1001) docker     (116)     6764 2021-11-30 15:18:30.000000 brown_clustering-0.1.4/brown_clustering/helper.py
--rw-r--r--   0 runner    (1001) docker     (116)     2135 2021-11-30 15:18:30.000000 brown_clustering-0.1.4/brown_clustering/core.py
--rw-r--r--   0 runner    (1001) docker     (116)     3899 2021-11-30 15:18:30.000000 brown_clustering-0.1.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-11-30 15:18:42.000000 brown_clustering-0.1.4/brown_clustering.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)     4209 2021-11-30 15:18:42.000000 brown_clustering-0.1.4/brown_clustering.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)      105 2021-11-30 15:18:42.000000 brown_clustering-0.1.4/brown_clustering.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)      378 2021-11-30 15:18:42.000000 brown_clustering-0.1.4/brown_clustering.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2021-11-30 15:18:42.000000 brown_clustering-0.1.4/brown_clustering.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)       17 2021-11-30 15:18:42.000000 brown_clustering-0.1.4/brown_clustering.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 11:58:16.000000 brown_clustering-0.1.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-05-18 11:58:06.000000 brown_clustering-0.1.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4232 2023-05-18 11:58:16.000000 brown_clustering-0.1.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3899 2023-05-18 11:58:06.000000 brown_clustering-0.1.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 11:58:16.000000 brown_clustering-0.1.6/brown_clustering/
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-05-18 11:58:06.000000 brown_clustering-0.1.6/brown_clustering/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2149 2023-05-18 11:58:06.000000 brown_clustering-0.1.6/brown_clustering/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2747 2023-05-18 11:58:06.000000 brown_clustering-0.1.6/brown_clustering/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      365 2023-05-18 11:58:06.000000 brown_clustering-0.1.6/brown_clustering/defaultvaluedict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6514 2023-05-18 11:58:06.000000 brown_clustering-0.1.6/brown_clustering/helper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 11:58:16.000000 brown_clustering-0.1.6/brown_clustering.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4232 2023-05-18 11:58:16.000000 brown_clustering-0.1.6/brown_clustering.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      403 2023-05-18 11:58:16.000000 brown_clustering-0.1.6/brown_clustering.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 11:58:16.000000 brown_clustering-0.1.6/brown_clustering.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-18 11:58:16.000000 brown_clustering-0.1.6/brown_clustering.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-18 11:58:16.000000 brown_clustering-0.1.6/brown_clustering.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-05-18 11:58:16.000000 brown_clustering-0.1.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      896 2023-05-18 11:58:06.000000 brown_clustering-0.1.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 11:58:16.000000 brown_clustering-0.1.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     5552 2023-05-18 11:58:06.000000 brown_clustering-0.1.6/tests/test_clustering.py
```

### Comparing `brown_clustering-0.1.4/setup.py` & `brown_clustering-0.1.6/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,26 +2,27 @@
 
 from setuptools import find_packages, setup
 
 base_path = Path(__file__).parent
 long_description = (base_path / "README.md").read_text()
 
 setup(
-    name='brown_clustering',
+    name="brown_clustering",
     packages=find_packages(include=("brown_clustering",)),
-    version='0.1.4',
-    description='Fast Brown Clustering',
+    version="0.1.6",
+    description="Fast Brown Clustering",
     long_description=long_description,
-    long_description_content_type='text/markdown',
-    author='bfuchs',
+    long_description_content_type="text/markdown",
+    author="bfuchs",
     author_email="benedikt.fuchs.staw@hotmail.com",
     license="MIT",
-    python_requires=">=3.6",
+    python_requires=">=3.7",
+    url="https://github.com/helpmefindaname/BrownClustering",
     install_requires=[
-        "numpy<1.21",
+        "numpy",
         "numba",
         "tqdm",
     ],
     extras_require={
         "dev": [
             "pytest",
             "pytest-mypy",
```

### Comparing `brown_clustering-0.1.4/PKG-INFO` & `brown_clustering-0.1.6/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,37 +1,23 @@
-Metadata-Version: 2.1
-Name: brown_clustering
-Version: 0.1.4
-Summary: Fast Brown Clustering
-Home-page: UNKNOWN
-Author: bfuchs
-Author-email: benedikt.fuchs.staw@hotmail.com
-License: MIT
-Platform: UNKNOWN
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-Provides-Extra: dev
-License-File: LICENSE
-
 # Brown Clustering
 
 [![PyPI version](https://badge.fury.io/py/brown-clustering.svg)](https://badge.fury.io/py/brown-clustering)
 [![GitHub Issues](https://img.shields.io/github/issues/helpmefindaname/BrownClustering.svg)](https://github.com/helpmefindaname/BrownClustering/issues)
 [![License: MIT](https://img.shields.io/badge/License-MIT-brightgreen.svg)](https://opensource.org/licenses/MIT)
 Easy to use and fast Brown Clustering in python.
 
 ---
 
 
 ## Quick Start
 
 ### Requirements and Installation
 
-The project is based on Python 3.6+, because method signatures and type hints are beautiful.
-If you do not have Python 3.6, install it first. [Here is how for Ubuntu 16.04](https://vsupalov.com/developing-with-python3-6-on-ubuntu-16-04/).
+The project is based on Python 3.7+, because method signatures and type hints are beautiful.
+If you do not have Python 3.7, install it first. [Here is how for Ubuntu 16.04](https://vsupalov.com/developing-with-python3-6-on-ubuntu-16-04/).
 Then, in your favorite virtual environment, simply do:
 
 ```
 pip install brown-clustering
 ```
 
 
@@ -110,9 +96,7 @@
 | [brown-cluster](https://github.com/percyliang/brown-cluster)  | C++  | clone & make & run  | n.a.  |
 | [This](https://github.com/helpmefindaname/BrownClustering)  | python  | pipy install & import  | 00:06:51  |
 
 if you know any missing libraries, please create an issue or a pull request.
 
 
 
-
-
```

### Comparing `brown_clustering-0.1.4/LICENSE` & `brown_clustering-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `brown_clustering-0.1.4/brown_clustering/data.py` & `brown_clustering-0.1.6/brown_clustering/data.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,20 +4,20 @@
 from brown_clustering.defaultvaluedict import DefaultValueDict
 
 Corpus = Sequence[Sequence[str]]
 
 
 class BigramCorpus:
     def __init__(
-            self,
-            corpus: Corpus,
-            alpha: float = 1,
-            start_symbol: str = '<s>',
-            end_symbol: str = '</s>',
-            min_count: int = 0
+        self,
+        corpus: Corpus,
+        alpha: float = 1,
+        start_symbol: str = "<s>",
+        end_symbol: str = "</s>",
+        min_count: int = 0,
     ):
         self.vocabulary: Dict[str, int] = DefaultValueDict(0)
 
         self.gather_vocab(corpus, min_count)
 
         word_count = len(self.vocabulary) + 2
         self.alpha = alpha
@@ -27,54 +27,49 @@
         self.gather_statistics(corpus, start_symbol, end_symbol)
 
     def gather_vocab(self, corpus: Corpus, min_count: int):
         for sentence in corpus:
             for word in sentence:
                 self.vocabulary[word] += 1
 
-        self.vocabulary = dict(filter(
-            lambda x: x[1] >= min_count,
-            self.vocabulary.items()
-        ))
+        self.vocabulary = dict(
+            filter(lambda x: x[1] >= min_count, self.vocabulary.items())
+        )
 
     def gather_statistics(
-            self,
-            corpus: Corpus,
-            start_symbol: str = '<s>',
-            end_symbol: str = '</s>',
+        self,
+        corpus: Corpus,
+        start_symbol: str = "<s>",
+        end_symbol: str = "</s>",
     ):
         for sentence in corpus:
-            act_sentence = [start_symbol] + [
-                w for w in sentence if w in self.vocabulary
-            ] + [end_symbol]
+            act_sentence = (
+                [start_symbol]
+                + [w for w in sentence if w in self.vocabulary]
+                + [end_symbol]
+            )
 
             for word in act_sentence:
                 self.unigrams[word] += 1
 
             grams = two_grams(act_sentence)
             for w1, w2 in grams:
                 self.n += 1
                 self.bigrams[(w1, w2)] += 1
 
     def bigram_propa(
-            self,
-            cluster1: Sequence[str],
-            cluster2: Sequence[str]
+        self, cluster1: Sequence[str], cluster2: Sequence[str]
     ) -> float:
-        return sum(
-            self.bigrams[(w1, w2)]
-            for w1 in cluster1
-            for w2 in cluster2
-        ) / self.n
+        return (
+            sum(self.bigrams[(w1, w2)] for w1 in cluster1 for w2 in cluster2)
+            / self.n
+        )
 
     def unigram_propa(self, cluster: Sequence[str]) -> float:
-        return sum(
-            self.unigrams[w]
-            for w in cluster
-        ) / self.n
+        return sum(self.unigrams[w] for w in cluster) / self.n
 
     def ranks(self) -> List[Tuple[str, int]]:
         return sorted(self.vocabulary.items(), key=lambda x: (-x[1], x[0]))
 
     def print_stats(self):
         extended_vocab = len(self.vocabulary) + 2
         alpha_bonus = self.alpha * extended_vocab * extended_vocab
```

### Comparing `brown_clustering-0.1.4/brown_clustering/helper.py` & `brown_clustering-0.1.6/brown_clustering/helper.py`

 * *Files 2% similar despite different names*

```diff
@@ -148,40 +148,30 @@
 
     for i in prange(n):
         if not mask[i]:
             continue
         for j in prange(n):
             if not mask[j]:
                 continue
-            l2[i, j] -= (
-                    + q2[i, x]
-                    + q2[j, x]
-                    + q2[x, i]
-                    + q2[x, j]
-            )
+            l2[i, j] -= +q2[i, x] + q2[j, x] + q2[x, i] + q2[x, j]
 
 
 @jit(nopython=True, parallel=True)
 def _reduce_delta(used, l2, p1, p2, q2, x):
     _q_l_n(used, l2, p1, p2, x)
     _q_r_n(used, l2, p1, p2, x)
 
     n = l2.shape[0]
     for i in prange(n):
         if not used[i]:
             continue
         for j in prange(n):
             if not used[j]:
                 continue
-            l2[i, j] += (
-                    + q2[i, x]
-                    + q2[j, x]
-                    + q2[x, i]
-                    + q2[x, j]
-            )
+            l2[i, j] += +q2[i, x] + q2[j, x] + q2[x, i] + q2[x, j]
 
 
 @jit(nopython=True, parallel=True)
 def _update_heuristic(used, l2, p1, p2, q2, x):
     _q_l(used, p1, p2, q2, x)
     _q_r(used, p1, p2, q2, x)
 
@@ -214,33 +204,29 @@
         self.l2 = np.zeros((max_words, max_words), dtype=float)
         self.used = np.zeros(max_words, dtype=bool)
         self.max_words = max_words
         self.corpus = corpus
 
     def copy_clusters(self) -> List[List[str]]:
         return [
-            c
-            for c, used in zip(deepcopy(self.clusters), self.used)
-            if used
+            c for c, used in zip(deepcopy(self.clusters), self.used) if used
         ]
 
     def append_cluster(self, words: List[str]):
         new_i = self.used.argmin()
         self.clusters[new_i] = words
 
         self.p1[new_i] = self.corpus.unigram_propa(words)
 
         for i in range(self.max_words):
             self.p2[new_i, i] = self.corpus.bigram_propa(
-                words,
-                self.clusters[i]
+                words, self.clusters[i]
             )
             self.p2[i, new_i] = self.corpus.bigram_propa(
-                self.clusters[i],
-                words
+                self.clusters[i], words
             )
         self.p2[new_i, new_i] = self.corpus.bigram_propa(words, words)
         self.used[new_i] = True
         _update_heuristic(self.used, self.l2, self.p1, self.p2, self.q2, new_i)
 
         self.m += 1
```

### Comparing `brown_clustering-0.1.4/brown_clustering/core.py` & `brown_clustering-0.1.6/brown_clustering/core.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import heapq
 from collections import defaultdict, deque
-from typing import Deque, Dict, List, Sequence, Tuple
+from typing import Deque, Dict, List, Sequence, Tuple, cast
 
 import numpy as np
 from tqdm import tqdm
 
 from brown_clustering.data import BigramCorpus
 from brown_clustering.helper import ClusteringHelper
 
@@ -14,33 +14,32 @@
         self.m = m
         self.corpus = corpus
         self.vocabulary = corpus.vocabulary
         self.helper = ClusteringHelper(corpus, self.m + 1)
         self._codes: Dict[str, Deque[str]] = defaultdict(lambda: deque())
 
     def codes(self) -> Dict[str, str]:
-        return {
-            key: ''.join(value)
-            for key, value in self._codes.items()
-        }
+        return {key: "".join(value) for key, value in self._codes.items()}
 
     def merge_best(self) -> Tuple[int, int]:
         benefit = self.helper.l2
-        i, j = np.unravel_index(benefit.argmax(), benefit.shape)
+        i, j = cast(
+            Tuple[int, int], np.unravel_index(benefit.argmax(), benefit.shape)
+        )
 
         for word in self.helper.clusters[i]:
             self._codes[word].appendleft("0")
 
         for word in self.helper.clusters[j]:
             self._codes[word].appendleft("1")
         self.helper.merge_clusters(i, j)
         return i, j
 
     def _code_similarity(
-            self, code1: Sequence[str], code2: Sequence[str]
+        self, code1: Sequence[str], code2: Sequence[str]
     ) -> int:
         count = 0
         for w1, w2 in zip(code1, code2):
             if w1 == w2:
                 count += 1
             else:
                 return count
@@ -52,15 +51,15 @@
             return []
         code = tmp[word]
         del tmp[word]
 
         best = heapq.nlargest(
             iterable=tmp.items(),
             n=cap,
-            key=lambda it: self._code_similarity(code, it[1])
+            key=lambda it: self._code_similarity(code, it[1]),
         )
         return best
 
     def train(self) -> List[List[str]]:
         words = self.corpus.ranks()
 
         for w, count in tqdm(words):
```

### Comparing `brown_clustering-0.1.4/README.md` & `brown_clustering-0.1.6/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,23 +1,36 @@
+Metadata-Version: 2.1
+Name: brown_clustering
+Version: 0.1.6
+Summary: Fast Brown Clustering
+Home-page: https://github.com/helpmefindaname/BrownClustering
+Author: bfuchs
+Author-email: benedikt.fuchs.staw@hotmail.com
+License: MIT
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+Provides-Extra: dev
+License-File: LICENSE
+
 # Brown Clustering
 
 [![PyPI version](https://badge.fury.io/py/brown-clustering.svg)](https://badge.fury.io/py/brown-clustering)
 [![GitHub Issues](https://img.shields.io/github/issues/helpmefindaname/BrownClustering.svg)](https://github.com/helpmefindaname/BrownClustering/issues)
 [![License: MIT](https://img.shields.io/badge/License-MIT-brightgreen.svg)](https://opensource.org/licenses/MIT)
 Easy to use and fast Brown Clustering in python.
 
 ---
 
 
 ## Quick Start
 
 ### Requirements and Installation
 
-The project is based on Python 3.6+, because method signatures and type hints are beautiful.
-If you do not have Python 3.6, install it first. [Here is how for Ubuntu 16.04](https://vsupalov.com/developing-with-python3-6-on-ubuntu-16-04/).
+The project is based on Python 3.7+, because method signatures and type hints are beautiful.
+If you do not have Python 3.7, install it first. [Here is how for Ubuntu 16.04](https://vsupalov.com/developing-with-python3-6-on-ubuntu-16-04/).
 Then, in your favorite virtual environment, simply do:
 
 ```
 pip install brown-clustering
 ```
```

### Comparing `brown_clustering-0.1.4/brown_clustering.egg-info/PKG-INFO` & `brown_clustering-0.1.6/brown_clustering.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: brown-clustering
-Version: 0.1.4
+Version: 0.1.6
 Summary: Fast Brown Clustering
-Home-page: UNKNOWN
+Home-page: https://github.com/helpmefindaname/BrownClustering
 Author: bfuchs
 Author-email: benedikt.fuchs.staw@hotmail.com
 License: MIT
-Platform: UNKNOWN
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 # Brown Clustering
 
 [![PyPI version](https://badge.fury.io/py/brown-clustering.svg)](https://badge.fury.io/py/brown-clustering)
@@ -22,16 +21,16 @@
 ---
 
 
 ## Quick Start
 
 ### Requirements and Installation
 
-The project is based on Python 3.6+, because method signatures and type hints are beautiful.
-If you do not have Python 3.6, install it first. [Here is how for Ubuntu 16.04](https://vsupalov.com/developing-with-python3-6-on-ubuntu-16-04/).
+The project is based on Python 3.7+, because method signatures and type hints are beautiful.
+If you do not have Python 3.7, install it first. [Here is how for Ubuntu 16.04](https://vsupalov.com/developing-with-python3-6-on-ubuntu-16-04/).
 Then, in your favorite virtual environment, simply do:
 
 ```
 pip install brown-clustering
 ```
 
 
@@ -110,9 +109,7 @@
 | [brown-cluster](https://github.com/percyliang/brown-cluster)  | C++  | clone & make & run  | n.a.  |
 | [This](https://github.com/helpmefindaname/BrownClustering)  | python  | pipy install & import  | 00:06:51  |
 
 if you know any missing libraries, please create an issue or a pull request.
 
 
 
-
-
```

