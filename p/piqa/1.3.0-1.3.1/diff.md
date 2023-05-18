# Comparing `tmp/piqa-1.3.0.tar.gz` & `tmp/piqa-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "piqa-1.3.0.tar", last modified: Mon Apr 10 18:36:30 2023, max compression
+gzip compressed data, was "piqa-1.3.1.tar", last modified: Thu May 18 13:01:15 2023, max compression
```

## Comparing `piqa-1.3.0.tar` & `piqa-1.3.1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxr-x   0 francois  (1001) francois  (1001)        0 2023-04-10 18:36:30.581264 piqa-1.3.0/
--rw-rw-r--   0 francois  (1001) francois  (1001)     1072 2023-03-26 10:06:00.000000 piqa-1.3.0/LICENSE
--rw-rw-r--   0 francois  (1001) francois  (1001)     5815 2023-04-10 18:36:30.581264 piqa-1.3.0/PKG-INFO
--rw-rw-r--   0 francois  (1001) francois  (1001)     4994 2023-04-10 18:33:28.000000 piqa-1.3.0/README.md
-drwxrwxr-x   0 francois  (1001) francois  (1001)        0 2023-04-10 18:36:30.577264 piqa-1.3.0/piqa/
--rw-rw-r--   0 francois  (1001) francois  (1001)      320 2023-04-10 18:33:28.000000 piqa-1.3.0/piqa/__init__.py
--rw-rw-r--   0 francois  (1001) francois  (1001)     5241 2023-04-10 18:33:28.000000 piqa-1.3.0/piqa/fid.py
--rw-rw-r--   0 francois  (1001) francois  (1001)     9181 2023-04-10 18:33:28.000000 piqa-1.3.0/piqa/fsim.py
--rw-rw-r--   0 francois  (1001) francois  (1001)     9119 2023-04-10 18:33:28.000000 piqa-1.3.0/piqa/gmsd.py
--rw-rw-r--   0 francois  (1001) francois  (1001)     5170 2023-04-10 18:33:28.000000 piqa-1.3.0/piqa/haarpsi.py
--rw-rw-r--   0 francois  (1001) francois  (1001)     4990 2023-04-10 18:33:28.000000 piqa-1.3.0/piqa/lpips.py
--rw-rw-r--   0 francois  (1001) francois  (1001)     5547 2023-04-10 18:33:28.000000 piqa-1.3.0/piqa/mdsi.py
--rw-rw-r--   0 francois  (1001) francois  (1001)     2995 2023-04-10 18:33:28.000000 piqa-1.3.0/piqa/psnr.py
--rw-rw-r--   0 francois  (1001) francois  (1001)     9782 2023-04-10 18:33:28.000000 piqa-1.3.0/piqa/ssim.py
--rw-rw-r--   0 francois  (1001) francois  (1001)     2438 2023-04-10 18:33:28.000000 piqa-1.3.0/piqa/tv.py
-drwxrwxr-x   0 francois  (1001) francois  (1001)        0 2023-04-10 18:36:30.581264 piqa-1.3.0/piqa/utils/
--rw-rw-r--   0 francois  (1001) francois  (1001)     3024 2023-04-10 18:33:28.000000 piqa-1.3.0/piqa/utils/__init__.py
--rw-rw-r--   0 francois  (1001) francois  (1001)     3856 2023-04-10 18:33:28.000000 piqa-1.3.0/piqa/utils/color.py
--rw-rw-r--   0 francois  (1001) francois  (1001)    11466 2023-04-10 18:33:28.000000 piqa-1.3.0/piqa/utils/functional.py
--rw-rw-r--   0 francois  (1001) francois  (1001)     7714 2023-04-10 18:33:28.000000 piqa-1.3.0/piqa/vsi.py
-drwxrwxr-x   0 francois  (1001) francois  (1001)        0 2023-04-10 18:36:30.581264 piqa-1.3.0/piqa.egg-info/
--rw-rw-r--   0 francois  (1001) francois  (1001)     5815 2023-04-10 18:36:30.000000 piqa-1.3.0/piqa.egg-info/PKG-INFO
--rw-rw-r--   0 francois  (1001) francois  (1001)      390 2023-04-10 18:36:30.000000 piqa-1.3.0/piqa.egg-info/SOURCES.txt
--rw-rw-r--   0 francois  (1001) francois  (1001)        1 2023-04-10 18:36:30.000000 piqa-1.3.0/piqa.egg-info/dependency_links.txt
--rw-rw-r--   0 francois  (1001) francois  (1001)       34 2023-04-10 18:36:30.000000 piqa-1.3.0/piqa.egg-info/requires.txt
--rw-rw-r--   0 francois  (1001) francois  (1001)        5 2023-04-10 18:36:30.000000 piqa-1.3.0/piqa.egg-info/top_level.txt
--rw-rw-r--   0 francois  (1001) francois  (1001)      899 2023-04-10 18:36:30.581264 piqa-1.3.0/setup.cfg
--rw-rw-r--   0 francois  (1001) francois  (1001)       61 2023-04-10 18:33:28.000000 piqa-1.3.0/setup.py
+drwxrwxr-x   0 francois  (1001) francois  (1001)        0 2023-05-18 13:01:15.831610 piqa-1.3.1/
+-rw-rw-r--   0 francois  (1001) francois  (1001)     1072 2023-03-26 10:06:00.000000 piqa-1.3.1/LICENSE
+-rw-rw-r--   0 francois  (1001) francois  (1001)     5693 2023-05-18 13:01:15.831610 piqa-1.3.1/PKG-INFO
+-rw-rw-r--   0 francois  (1001) francois  (1001)     4994 2023-04-10 18:33:28.000000 piqa-1.3.1/README.md
+drwxrwxr-x   0 francois  (1001) francois  (1001)        0 2023-05-18 13:01:15.831610 piqa-1.3.1/piqa/
+-rw-rw-r--   0 francois  (1001) francois  (1001)      320 2023-05-18 13:00:26.000000 piqa-1.3.1/piqa/__init__.py
+-rw-rw-r--   0 francois  (1001) francois  (1001)     5913 2023-05-18 12:50:27.000000 piqa-1.3.1/piqa/fid.py
+-rw-rw-r--   0 francois  (1001) francois  (1001)     9181 2023-04-10 18:33:28.000000 piqa-1.3.1/piqa/fsim.py
+-rw-rw-r--   0 francois  (1001) francois  (1001)     9119 2023-04-10 18:33:28.000000 piqa-1.3.1/piqa/gmsd.py
+-rw-rw-r--   0 francois  (1001) francois  (1001)     5170 2023-04-10 18:33:28.000000 piqa-1.3.1/piqa/haarpsi.py
+-rw-rw-r--   0 francois  (1001) francois  (1001)     4990 2023-04-10 18:33:28.000000 piqa-1.3.1/piqa/lpips.py
+-rw-rw-r--   0 francois  (1001) francois  (1001)     5547 2023-04-10 18:33:28.000000 piqa-1.3.1/piqa/mdsi.py
+-rw-rw-r--   0 francois  (1001) francois  (1001)     2995 2023-04-10 18:33:28.000000 piqa-1.3.1/piqa/psnr.py
+-rw-rw-r--   0 francois  (1001) francois  (1001)     9782 2023-04-10 18:33:28.000000 piqa-1.3.1/piqa/ssim.py
+-rw-rw-r--   0 francois  (1001) francois  (1001)     2438 2023-04-10 18:33:28.000000 piqa-1.3.1/piqa/tv.py
+drwxrwxr-x   0 francois  (1001) francois  (1001)        0 2023-05-18 13:01:15.831610 piqa-1.3.1/piqa/utils/
+-rw-rw-r--   0 francois  (1001) francois  (1001)     3024 2023-04-10 18:33:28.000000 piqa-1.3.1/piqa/utils/__init__.py
+-rw-rw-r--   0 francois  (1001) francois  (1001)     3856 2023-04-10 18:33:28.000000 piqa-1.3.1/piqa/utils/color.py
+-rw-rw-r--   0 francois  (1001) francois  (1001)    11466 2023-04-10 18:33:28.000000 piqa-1.3.1/piqa/utils/functional.py
+-rw-rw-r--   0 francois  (1001) francois  (1001)     7714 2023-04-10 18:33:28.000000 piqa-1.3.1/piqa/vsi.py
+drwxrwxr-x   0 francois  (1001) francois  (1001)        0 2023-05-18 13:01:15.831610 piqa-1.3.1/piqa.egg-info/
+-rw-rw-r--   0 francois  (1001) francois  (1001)     5693 2023-05-18 13:01:15.000000 piqa-1.3.1/piqa.egg-info/PKG-INFO
+-rw-rw-r--   0 francois  (1001) francois  (1001)      390 2023-05-18 13:01:15.000000 piqa-1.3.1/piqa.egg-info/SOURCES.txt
+-rw-rw-r--   0 francois  (1001) francois  (1001)        1 2023-05-18 13:01:15.000000 piqa-1.3.1/piqa.egg-info/dependency_links.txt
+-rw-rw-r--   0 francois  (1001) francois  (1001)       34 2023-05-18 13:01:15.000000 piqa-1.3.1/piqa.egg-info/requires.txt
+-rw-rw-r--   0 francois  (1001) francois  (1001)        5 2023-05-18 13:01:15.000000 piqa-1.3.1/piqa.egg-info/top_level.txt
+-rw-rw-r--   0 francois  (1001) francois  (1001)      792 2023-05-18 13:01:15.831610 piqa-1.3.1/setup.cfg
+-rw-rw-r--   0 francois  (1001) francois  (1001)       72 2023-04-12 12:10:12.000000 piqa-1.3.1/setup.py
```

### Comparing `piqa-1.3.0/LICENSE` & `piqa-1.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `piqa-1.3.0/PKG-INFO` & `piqa-1.3.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,22 +1,19 @@
 Metadata-Version: 2.1
 Name: piqa
-Version: 1.3.0
+Version: 1.3.1
 Summary: PyTorch Image Quality Assessment
-Home-page: https://github.com/francois-rozet/piqa
 Author: François Rozet
 Author-email: francois.rozet@outlook.com
-License: MIT License
 Project-URL: Documentation, https://piqa.readthedocs.io
 Project-URL: Source, https://github.com/francois-rozet/piqa
 Project-URL: Tracker, https://github.com/francois-rozet/piqa/issues
 Keywords: torch,vision,image,quality,metrics
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
-Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `piqa-1.3.0/README.md` & `piqa-1.3.1/README.md`

 * *Files identical despite different names*

### Comparing `piqa-1.3.0/piqa/fid.py` & `piqa-1.3.1/piqa/fid.py`

 * *Files 12% similar despite different names*

```diff
@@ -21,24 +21,49 @@
 from typing import *
 
 from .utils import assert_type
 from .utils.color import ImageNetNorm
 
 
 @torch.jit.script_if_tracing
+def sqrtm(sigma: Tensor) -> Tensor:
+    r"""Returns the square root of a positive semi-definite matrix.
+
+    .. math:: \sqrt{\Sigma} = Q \sqrt{\Lambda} Q^T
+
+    where :math:`Q \Lambda Q^T` is the eigendecomposition of :math:`\Sigma`.
+
+    Args:
+        sigma: A positive semi-definite matrix, :math:`(*, D, D)`.
+
+    Example:
+        >>> V = torch.randn(4, 4, dtype=torch.double)
+        >>> A = V @ V.T
+        >>> B = sqrtm(A @ A)
+        >>> torch.allclose(A, B)
+        True
+    """
+
+    L, Q = torch.linalg.eigh(sigma)
+    L = L.relu().sqrt()
+
+    return Q @ (L[..., None] * Q.mT)
+
+
+@torch.jit.script_if_tracing
 def frechet_distance(
     mu_x: Tensor,
     sigma_x: Tensor,
     mu_y: Tensor,
     sigma_y: Tensor,
 ) -> Tensor:
     r"""Returns the Fréchet distance between two multivariate Gaussian distributions.
 
     .. math:: d^2 = \left\| \mu_x - \mu_y \right\|_2^2 +
-        \operatorname{tr} \left( \Sigma_x + \Sigma_y - 2 \sqrt{\Sigma_x \Sigma_y} \right)
+        \operatorname{tr} \left( \Sigma_x + \Sigma_y - 2 \sqrt{\Sigma_y^{\frac{1}{2}} \Sigma_x \Sigma_y^{\frac{1}{2}}} \right)
 
     Wikipedia:
         https://wikipedia.org/wiki/Frechet_distance
 
     Args:
         mu_x: The mean :math:`\mu_x` of the first distribution, :math:`(*, D)`.
         sigma_x: The covariance :math:`\Sigma_x` of the first distribution, :math:`(*, D, D)`.
@@ -50,17 +75,19 @@
         >>> sigma_x = torch.eye(3)
         >>> mu_y = 2 * mu_x + 1
         >>> sigma_y = 2 * sigma_x + 1
         >>> frechet_distance(mu_x, sigma_x, mu_y, sigma_y)
         tensor(15.8710)
     """
 
+    sigma_y_12 = sqrtm(sigma_y)
+
     a = (mu_x - mu_y).square().sum(dim=-1)
     b = sigma_x.trace() + sigma_y.trace()
-    c = torch.linalg.eigvals(sigma_x @ sigma_y).sqrt().real.sum(dim=-1)
+    c = sqrtm(sigma_y_12 @ sigma_x @ sigma_y_12).trace()
 
     return a + b - 2 * c
 
 
 class InceptionV3(nn.Sequential):
     r"""Pretrained Inception-v3 network.
```

### Comparing `piqa-1.3.0/piqa/fsim.py` & `piqa-1.3.1/piqa/fsim.py`

 * *Files identical despite different names*

### Comparing `piqa-1.3.0/piqa/gmsd.py` & `piqa-1.3.1/piqa/gmsd.py`

 * *Files identical despite different names*

### Comparing `piqa-1.3.0/piqa/haarpsi.py` & `piqa-1.3.1/piqa/haarpsi.py`

 * *Files identical despite different names*

### Comparing `piqa-1.3.0/piqa/lpips.py` & `piqa-1.3.1/piqa/lpips.py`

 * *Files identical despite different names*

### Comparing `piqa-1.3.0/piqa/mdsi.py` & `piqa-1.3.1/piqa/mdsi.py`

 * *Files identical despite different names*

### Comparing `piqa-1.3.0/piqa/psnr.py` & `piqa-1.3.1/piqa/psnr.py`

 * *Files identical despite different names*

### Comparing `piqa-1.3.0/piqa/ssim.py` & `piqa-1.3.1/piqa/ssim.py`

 * *Files identical despite different names*

### Comparing `piqa-1.3.0/piqa/tv.py` & `piqa-1.3.1/piqa/tv.py`

 * *Files identical despite different names*

### Comparing `piqa-1.3.0/piqa/utils/__init__.py` & `piqa-1.3.1/piqa/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `piqa-1.3.0/piqa/utils/color.py` & `piqa-1.3.1/piqa/utils/color.py`

 * *Files identical despite different names*

### Comparing `piqa-1.3.0/piqa/utils/functional.py` & `piqa-1.3.1/piqa/utils/functional.py`

 * *Files identical despite different names*

### Comparing `piqa-1.3.0/piqa/vsi.py` & `piqa-1.3.1/piqa/vsi.py`

 * *Files identical despite different names*

### Comparing `piqa-1.3.0/piqa.egg-info/PKG-INFO` & `piqa-1.3.1/piqa.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,22 +1,19 @@
 Metadata-Version: 2.1
 Name: piqa
-Version: 1.3.0
+Version: 1.3.1
 Summary: PyTorch Image Quality Assessment
-Home-page: https://github.com/francois-rozet/piqa
 Author: François Rozet
 Author-email: francois.rozet@outlook.com
-License: MIT License
 Project-URL: Documentation, https://piqa.readthedocs.io
 Project-URL: Source, https://github.com/francois-rozet/piqa
 Project-URL: Tracker, https://github.com/francois-rozet/piqa/issues
 Keywords: torch,vision,image,quality,metrics
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
-Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `piqa-1.3.0/setup.cfg` & `piqa-1.3.1/setup.cfg`

 * *Files 24% similar despite different names*

```diff
@@ -8,24 +8,21 @@
 	torch
 	vision
 	image
 	quality
 	metrics
 author = François Rozet
 author_email = francois.rozet@outlook.com
-license = MIT License
-url = https://github.com/francois-rozet/piqa
 project_urls = 
 	Documentation = https://piqa.readthedocs.io
 	Source = https://github.com/francois-rozet/piqa
 	Tracker = https://github.com/francois-rozet/piqa/issues
 classifiers = 
 	Intended Audience :: Developers
 	Intended Audience :: Science/Research
-	License :: OSI Approved :: MIT License
 	Natural Language :: English
 	Operating System :: OS Independent
 	Programming Language :: Python :: 3
 
 [options]
 packages = find:
 python_requires = >=3.8
```

