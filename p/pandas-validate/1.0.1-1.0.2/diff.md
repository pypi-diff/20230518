# Comparing `tmp/pandas-validate-1.0.1.tar.gz` & `tmp/pandas-validate-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pandas-validate-1.0.1.tar", last modified: Fri May 12 03:26:49 2023, max compression
+gzip compressed data, was "pandas-validate-1.0.2.tar", last modified: Thu May 18 15:25:33 2023, max compression
```

## Comparing `pandas-validate-1.0.1.tar` & `pandas-validate-1.0.2.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 trip      (1000) trip      (1000)        0 2023-05-12 03:26:49.986541 pandas-validate-1.0.1/
--rw-r--r--   0 trip      (1000) trip      (1000)     1068 2023-05-12 00:57:22.000000 pandas-validate-1.0.1/LICENSE
--rw-r--r--   0 trip      (1000) trip      (1000)     5065 2023-05-12 03:26:49.986541 pandas-validate-1.0.1/PKG-INFO
--rw-r--r--   0 trip      (1000) trip      (1000)     2987 2023-05-12 03:24:40.000000 pandas-validate-1.0.1/README.md
--rw-r--r--   0 trip      (1000) trip      (1000)     1020 2023-05-12 03:26:16.000000 pandas-validate-1.0.1/pyproject.toml
--rw-r--r--   0 trip      (1000) trip      (1000)       38 2023-05-12 03:26:49.986541 pandas-validate-1.0.1/setup.cfg
-drwxr-xr-x   0 trip      (1000) trip      (1000)        0 2023-05-12 03:26:49.986541 pandas-validate-1.0.1/src/
-drwxr-xr-x   0 trip      (1000) trip      (1000)        0 2023-05-12 03:26:49.986541 pandas-validate-1.0.1/src/pandas_validate/
--rw-r--r--   0 trip      (1000) trip      (1000)     2265 2023-05-12 02:05:51.000000 pandas-validate-1.0.1/src/pandas_validate/Schema.py
--rw-r--r--   0 trip      (1000) trip      (1000)       49 2023-05-12 03:26:21.000000 pandas-validate-1.0.1/src/pandas_validate/__init__.py
-drwxr-xr-x   0 trip      (1000) trip      (1000)        0 2023-05-12 03:26:49.986541 pandas-validate-1.0.1/src/pandas_validate/columns/
--rw-r--r--   0 trip      (1000) trip      (1000)     1593 2023-05-12 02:12:23.000000 pandas-validate-1.0.1/src/pandas_validate/columns/Column.py
--rw-r--r--   0 trip      (1000) trip      (1000)     1703 2023-05-12 01:39:15.000000 pandas-validate-1.0.1/src/pandas_validate/columns/DateTimeColumn.py
--rw-r--r--   0 trip      (1000) trip      (1000)     1742 2023-05-12 00:57:22.000000 pandas-validate-1.0.1/src/pandas_validate/columns/DecimalColumn.py
--rw-r--r--   0 trip      (1000) trip      (1000)     1527 2023-05-12 00:57:22.000000 pandas-validate-1.0.1/src/pandas_validate/columns/FloatColumn.py
--rw-r--r--   0 trip      (1000) trip      (1000)     1523 2023-05-12 00:57:22.000000 pandas-validate-1.0.1/src/pandas_validate/columns/IntColumn.py
--rw-r--r--   0 trip      (1000) trip      (1000)     1815 2023-05-12 00:57:22.000000 pandas-validate-1.0.1/src/pandas_validate/columns/TextColumn.py
--rw-r--r--   0 trip      (1000) trip      (1000)      216 2023-05-12 00:57:22.000000 pandas-validate-1.0.1/src/pandas_validate/columns/__init__.py
-drwxr-xr-x   0 trip      (1000) trip      (1000)        0 2023-05-12 03:26:49.986541 pandas-validate-1.0.1/src/pandas_validate.egg-info/
--rw-r--r--   0 trip      (1000) trip      (1000)     5065 2023-05-12 03:26:49.000000 pandas-validate-1.0.1/src/pandas_validate.egg-info/PKG-INFO
--rw-r--r--   0 trip      (1000) trip      (1000)      777 2023-05-12 03:26:49.000000 pandas-validate-1.0.1/src/pandas_validate.egg-info/SOURCES.txt
--rw-r--r--   0 trip      (1000) trip      (1000)        1 2023-05-12 03:26:49.000000 pandas-validate-1.0.1/src/pandas_validate.egg-info/dependency_links.txt
--rw-r--r--   0 trip      (1000) trip      (1000)       53 2023-05-12 03:26:49.000000 pandas-validate-1.0.1/src/pandas_validate.egg-info/requires.txt
--rw-r--r--   0 trip      (1000) trip      (1000)       16 2023-05-12 03:26:49.000000 pandas-validate-1.0.1/src/pandas_validate.egg-info/top_level.txt
-drwxr-xr-x   0 trip      (1000) trip      (1000)        0 2023-05-12 03:26:49.986541 pandas-validate-1.0.1/tests/
--rw-r--r--   0 trip      (1000) trip      (1000)     1075 2023-05-12 00:57:22.000000 pandas-validate-1.0.1/tests/test_Column.py
--rw-r--r--   0 trip      (1000) trip      (1000)     2228 2023-05-12 00:57:22.000000 pandas-validate-1.0.1/tests/test_DateTimeColumn.py
--rw-r--r--   0 trip      (1000) trip      (1000)     2087 2023-05-12 00:57:22.000000 pandas-validate-1.0.1/tests/test_DecimalColumn.py
--rw-r--r--   0 trip      (1000) trip      (1000)     1944 2023-05-12 00:57:22.000000 pandas-validate-1.0.1/tests/test_FloatColumn.py
--rw-r--r--   0 trip      (1000) trip      (1000)     1820 2023-05-12 00:57:22.000000 pandas-validate-1.0.1/tests/test_IntColumn.py
--rw-r--r--   0 trip      (1000) trip      (1000)     2166 2023-05-12 02:27:05.000000 pandas-validate-1.0.1/tests/test_Schema.py
--rw-r--r--   0 trip      (1000) trip      (1000)     2048 2023-05-12 00:57:22.000000 pandas-validate-1.0.1/tests/test_TextColumn.py
+drwxr-xr-x   0 trip      (1000) trip      (1000)        0 2023-05-18 15:25:33.449477 pandas-validate-1.0.2/
+-rw-r--r--   0 trip      (1000) trip      (1000)     1068 2023-05-12 00:57:22.000000 pandas-validate-1.0.2/LICENSE
+-rw-r--r--   0 trip      (1000) trip      (1000)     5049 2023-05-18 15:25:33.449477 pandas-validate-1.0.2/PKG-INFO
+-rw-r--r--   0 trip      (1000) trip      (1000)     2971 2023-05-18 15:24:16.000000 pandas-validate-1.0.2/README.md
+-rw-r--r--   0 trip      (1000) trip      (1000)     1020 2023-05-18 15:22:27.000000 pandas-validate-1.0.2/pyproject.toml
+-rw-r--r--   0 trip      (1000) trip      (1000)       38 2023-05-18 15:25:33.449477 pandas-validate-1.0.2/setup.cfg
+drwxr-xr-x   0 trip      (1000) trip      (1000)        0 2023-05-18 15:25:33.449477 pandas-validate-1.0.2/src/
+drwxr-xr-x   0 trip      (1000) trip      (1000)        0 2023-05-18 15:25:33.449477 pandas-validate-1.0.2/src/pandas_validate/
+-rw-r--r--   0 trip      (1000) trip      (1000)     2265 2023-05-12 02:05:51.000000 pandas-validate-1.0.2/src/pandas_validate/Schema.py
+-rw-r--r--   0 trip      (1000) trip      (1000)       49 2023-05-18 15:22:32.000000 pandas-validate-1.0.2/src/pandas_validate/__init__.py
+drwxr-xr-x   0 trip      (1000) trip      (1000)        0 2023-05-18 15:25:33.449477 pandas-validate-1.0.2/src/pandas_validate/columns/
+-rw-r--r--   0 trip      (1000) trip      (1000)     1593 2023-05-12 02:12:23.000000 pandas-validate-1.0.2/src/pandas_validate/columns/Column.py
+-rw-r--r--   0 trip      (1000) trip      (1000)     1730 2023-05-18 15:21:31.000000 pandas-validate-1.0.2/src/pandas_validate/columns/DateTimeColumn.py
+-rw-r--r--   0 trip      (1000) trip      (1000)     1742 2023-05-18 15:20:56.000000 pandas-validate-1.0.2/src/pandas_validate/columns/DecimalColumn.py
+-rw-r--r--   0 trip      (1000) trip      (1000)     1527 2023-05-18 15:20:51.000000 pandas-validate-1.0.2/src/pandas_validate/columns/FloatColumn.py
+-rw-r--r--   0 trip      (1000) trip      (1000)     1523 2023-05-18 15:20:46.000000 pandas-validate-1.0.2/src/pandas_validate/columns/IntColumn.py
+-rw-r--r--   0 trip      (1000) trip      (1000)     1880 2023-05-18 15:22:13.000000 pandas-validate-1.0.2/src/pandas_validate/columns/TextColumn.py
+-rw-r--r--   0 trip      (1000) trip      (1000)      216 2023-05-12 00:57:22.000000 pandas-validate-1.0.2/src/pandas_validate/columns/__init__.py
+drwxr-xr-x   0 trip      (1000) trip      (1000)        0 2023-05-18 15:25:33.449477 pandas-validate-1.0.2/src/pandas_validate.egg-info/
+-rw-r--r--   0 trip      (1000) trip      (1000)     5049 2023-05-18 15:25:33.000000 pandas-validate-1.0.2/src/pandas_validate.egg-info/PKG-INFO
+-rw-r--r--   0 trip      (1000) trip      (1000)      777 2023-05-18 15:25:33.000000 pandas-validate-1.0.2/src/pandas_validate.egg-info/SOURCES.txt
+-rw-r--r--   0 trip      (1000) trip      (1000)        1 2023-05-18 15:25:33.000000 pandas-validate-1.0.2/src/pandas_validate.egg-info/dependency_links.txt
+-rw-r--r--   0 trip      (1000) trip      (1000)       53 2023-05-18 15:25:33.000000 pandas-validate-1.0.2/src/pandas_validate.egg-info/requires.txt
+-rw-r--r--   0 trip      (1000) trip      (1000)       16 2023-05-18 15:25:33.000000 pandas-validate-1.0.2/src/pandas_validate.egg-info/top_level.txt
+drwxr-xr-x   0 trip      (1000) trip      (1000)        0 2023-05-18 15:25:33.449477 pandas-validate-1.0.2/tests/
+-rw-r--r--   0 trip      (1000) trip      (1000)     1075 2023-05-12 00:57:22.000000 pandas-validate-1.0.2/tests/test_Column.py
+-rw-r--r--   0 trip      (1000) trip      (1000)     2228 2023-05-12 00:57:22.000000 pandas-validate-1.0.2/tests/test_DateTimeColumn.py
+-rw-r--r--   0 trip      (1000) trip      (1000)     2087 2023-05-12 00:57:22.000000 pandas-validate-1.0.2/tests/test_DecimalColumn.py
+-rw-r--r--   0 trip      (1000) trip      (1000)     1944 2023-05-12 00:57:22.000000 pandas-validate-1.0.2/tests/test_FloatColumn.py
+-rw-r--r--   0 trip      (1000) trip      (1000)     1820 2023-05-12 00:57:22.000000 pandas-validate-1.0.2/tests/test_IntColumn.py
+-rw-r--r--   0 trip      (1000) trip      (1000)     2166 2023-05-12 02:27:05.000000 pandas-validate-1.0.2/tests/test_Schema.py
+-rw-r--r--   0 trip      (1000) trip      (1000)     2048 2023-05-12 00:57:22.000000 pandas-validate-1.0.2/tests/test_TextColumn.py
```

### Comparing `pandas-validate-1.0.1/LICENSE` & `pandas-validate-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pandas-validate-1.0.1/PKG-INFO` & `pandas-validate-1.0.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pandas-validate
-Version: 1.0.1
+Version: 1.0.2
 Summary: A python package used for validating pandas dataframes.
 Author-email: Larry Green <larrygreen@duck.com>
 License: MIT License
         
         Copyright (c) 2023 larrygreen3
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -42,16 +42,16 @@
 License-File: LICENSE
 
 # pandas_validate
 
 <!-- Badges -->
 [![PyPI Latest Release](https://img.shields.io/pypi/v/pandas-validate.svg)](https://pypi.org/project/pandas-validate/)
 [![Package Status](https://img.shields.io/pypi/status/pandas-validate.svg)](https://pypi.org/project/pandas-validate/)
-[![License](https://img.shields.io/pypi/l/pandas.svg)](https://github.com/larrygreen3/pandas-validate/blob/main/LICENSE)
-[![Coverage](https://codecov.io/github/larrygreen3/pandas-validate/coverage.svg?branch=main)](https://codecov.io/gh/larrygreen3/pandas-validate)
+[![License](https://img.shields.io/pypi/l/pandas-validate.svg)](https://github.com/larrygreen3/pandas-validate/blob/main/LICENSE)
+[![Package Status](https://img.shields.io/pypi/dm/pandas-validate.svg)](https://pypistats.org/packages/pandas-validate)
 
 > A python package used for validating pandas dataframes.
 
 
 ## ⚙️ Installation
 ```sh
 python -m pip install pandas_validate
```

### Comparing `pandas-validate-1.0.1/README.md` & `pandas-validate-1.0.2/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # pandas_validate
 
 <!-- Badges -->
 [![PyPI Latest Release](https://img.shields.io/pypi/v/pandas-validate.svg)](https://pypi.org/project/pandas-validate/)
 [![Package Status](https://img.shields.io/pypi/status/pandas-validate.svg)](https://pypi.org/project/pandas-validate/)
-[![License](https://img.shields.io/pypi/l/pandas.svg)](https://github.com/larrygreen3/pandas-validate/blob/main/LICENSE)
-[![Coverage](https://codecov.io/github/larrygreen3/pandas-validate/coverage.svg?branch=main)](https://codecov.io/gh/larrygreen3/pandas-validate)
+[![License](https://img.shields.io/pypi/l/pandas-validate.svg)](https://github.com/larrygreen3/pandas-validate/blob/main/LICENSE)
+[![Package Status](https://img.shields.io/pypi/dm/pandas-validate.svg)](https://pypistats.org/packages/pandas-validate)
 
 > A python package used for validating pandas dataframes.
 
 
 ## ⚙️ Installation
 ```sh
 python -m pip install pandas_validate
```

### Comparing `pandas-validate-1.0.1/pyproject.toml` & `pandas-validate-1.0.2/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pandas-validate"
-version = "1.0.1"
+version = "1.0.2"
 description = "A python package used for validating pandas dataframes."
 readme = "README.md"
 authors = [
   { name="Larry Green", email="larrygreen@duck.com" },
 ]
 license = { file = "LICENSE" }
 classifiers = [
```

### Comparing `pandas-validate-1.0.1/src/pandas_validate/Schema.py` & `pandas-validate-1.0.2/src/pandas_validate/Schema.py`

 * *Files identical despite different names*

### Comparing `pandas-validate-1.0.1/src/pandas_validate/columns/Column.py` & `pandas-validate-1.0.2/src/pandas_validate/columns/Column.py`

 * *Files identical despite different names*

### Comparing `pandas-validate-1.0.1/src/pandas_validate/columns/DateTimeColumn.py` & `pandas-validate-1.0.2/src/pandas_validate/columns/DateTimeColumn.py`

 * *Files 10% similar despite different names*

```diff
@@ -53,13 +53,13 @@
 			except (ValueError, OverflowError):
 				raise ValueError(f'The value of {x} is not a valid datetime')
 
 		if not isinstance(x, datetime):
 			raise ValueError(f'The value {x} is not a valid datetime.')
 		
 		if self.min_date is not None and x < self.min_date:
-			raise ValueError(f'The value {x} is too early.')
+			raise ValueError(f'The value {x} is before {self.max_date}".')
 
 		if self.max_date is not None and x > self.max_date:
-			raise ValueError(f'The value {x} is too late.')
+			raise ValueError(f'The value {x} is after {self.max_date}.')
 
 		return x
```

### Comparing `pandas-validate-1.0.1/src/pandas_validate/columns/DecimalColumn.py` & `pandas-validate-1.0.2/src/pandas_validate/columns/DecimalColumn.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,10 +52,10 @@
 		except (TypeError, InvalidOperation):
 			raise ValueError(f'Could not convert "{x}" to a decimal')
 
 		if isinstance(self.min_value, Decimal) and d < self.min_value:
 			raise ValueError(f'The value {x} < {self.min_value}')
 
 		if isinstance(self.max_value, Decimal) and d > self.max_value:
-			raise ValueError(f'The value {x} < {self.max_value}')
+			raise ValueError(f'The value {x} > {self.max_value}')
 
 		return d
```

### Comparing `pandas-validate-1.0.1/src/pandas_validate/columns/FloatColumn.py` & `pandas-validate-1.0.2/src/pandas_validate/columns/FloatColumn.py`

 * *Files 1% similar despite different names*

```diff
@@ -50,10 +50,10 @@
 		except (ValueError, TypeError):
 			raise ValueError(f'Could not convert "{x}" to a float')
 
 		if isinstance(self.min_value, float) and f < self.min_value:
 			raise ValueError(f'The value {x} < {self.min_value}')
 
 		if isinstance(self.max_value, float) and f > self.max_value:
-			raise ValueError(f'The value {x} < {self.max_value}')
+			raise ValueError(f'The value {x} > {self.max_value}')
 
 		return f
```

### Comparing `pandas-validate-1.0.1/src/pandas_validate/columns/IntColumn.py` & `pandas-validate-1.0.2/src/pandas_validate/columns/IntColumn.py`

 * *Files 0% similar despite different names*

```diff
@@ -50,10 +50,10 @@
 		except (ValueError, TypeError):
 			raise ValueError(f'Could not convert "{x}" to an integer')
 
 		if isinstance(self.min_value, int) and i < self.min_value:
 			raise ValueError(f'The value {x} < {self.min_value}')
 
 		if isinstance(self.max_value, int) and i > self.max_value:
-			raise ValueError(f'The value {x} < {self.max_value}')
+			raise ValueError(f'The value {x} > {self.max_value}')
 
 		return i
```

### Comparing `pandas-validate-1.0.1/src/pandas_validate/columns/TextColumn.py` & `pandas-validate-1.0.2/src/pandas_validate/columns/TextColumn.py`

 * *Files 9% similar despite different names*

```diff
@@ -50,16 +50,16 @@
 			The validated value, or None if the value is invalid.
 		"""
 
 		if not isinstance(x, str):
 			raise ValueError(f'The value {x} is not a string')
 
 		if self.min_length is not None and len(x) < self.min_length:
-			raise ValueError(f'The value {x} is too short')
+			raise ValueError(f'The length of {x} is shorter than {self.min_length}')
 
 		if self.max_length is not None and len(x) > self.max_length:
-			raise ValueError(f'The value {x} is too long')
+			raise ValueError(f'The length of {x} is longer than {self.max_length}')
 		
 		if self.pattern is not None and not match(self.pattern, x):
-			raise ValueError(f'The value {x} does not match the regular expression.')
+			raise ValueError(f'The value {x} does not match the regular expression {self.pattern}.')
 
 		return x
```

### Comparing `pandas-validate-1.0.1/src/pandas_validate.egg-info/PKG-INFO` & `pandas-validate-1.0.2/src/pandas_validate.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pandas-validate
-Version: 1.0.1
+Version: 1.0.2
 Summary: A python package used for validating pandas dataframes.
 Author-email: Larry Green <larrygreen@duck.com>
 License: MIT License
         
         Copyright (c) 2023 larrygreen3
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -42,16 +42,16 @@
 License-File: LICENSE
 
 # pandas_validate
 
 <!-- Badges -->
 [![PyPI Latest Release](https://img.shields.io/pypi/v/pandas-validate.svg)](https://pypi.org/project/pandas-validate/)
 [![Package Status](https://img.shields.io/pypi/status/pandas-validate.svg)](https://pypi.org/project/pandas-validate/)
-[![License](https://img.shields.io/pypi/l/pandas.svg)](https://github.com/larrygreen3/pandas-validate/blob/main/LICENSE)
-[![Coverage](https://codecov.io/github/larrygreen3/pandas-validate/coverage.svg?branch=main)](https://codecov.io/gh/larrygreen3/pandas-validate)
+[![License](https://img.shields.io/pypi/l/pandas-validate.svg)](https://github.com/larrygreen3/pandas-validate/blob/main/LICENSE)
+[![Package Status](https://img.shields.io/pypi/dm/pandas-validate.svg)](https://pypistats.org/packages/pandas-validate)
 
 > A python package used for validating pandas dataframes.
 
 
 ## ⚙️ Installation
 ```sh
 python -m pip install pandas_validate
```

### Comparing `pandas-validate-1.0.1/src/pandas_validate.egg-info/SOURCES.txt` & `pandas-validate-1.0.2/src/pandas_validate.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pandas-validate-1.0.1/tests/test_Column.py` & `pandas-validate-1.0.2/tests/test_Column.py`

 * *Files identical despite different names*

### Comparing `pandas-validate-1.0.1/tests/test_DateTimeColumn.py` & `pandas-validate-1.0.2/tests/test_DateTimeColumn.py`

 * *Files identical despite different names*

### Comparing `pandas-validate-1.0.1/tests/test_DecimalColumn.py` & `pandas-validate-1.0.2/tests/test_DecimalColumn.py`

 * *Files identical despite different names*

### Comparing `pandas-validate-1.0.1/tests/test_FloatColumn.py` & `pandas-validate-1.0.2/tests/test_FloatColumn.py`

 * *Files identical despite different names*

### Comparing `pandas-validate-1.0.1/tests/test_IntColumn.py` & `pandas-validate-1.0.2/tests/test_IntColumn.py`

 * *Files identical despite different names*

### Comparing `pandas-validate-1.0.1/tests/test_Schema.py` & `pandas-validate-1.0.2/tests/test_Schema.py`

 * *Files identical despite different names*

### Comparing `pandas-validate-1.0.1/tests/test_TextColumn.py` & `pandas-validate-1.0.2/tests/test_TextColumn.py`

 * *Files identical despite different names*

