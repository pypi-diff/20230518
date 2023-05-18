# Comparing `tmp/Better-PyUnit-Format-0.1.1.tar.gz` & `tmp/Better-PyUnit-Format-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Better-PyUnit-Format-0.1.1.tar", last modified: Sat Mar 25 01:06:48 2023, max compression
+gzip compressed data, was "Better-PyUnit-Format-0.2.0.tar", last modified: Thu May 18 21:37:45 2023, max compression
```

## Comparing `Better-PyUnit-Format-0.1.1.tar` & `Better-PyUnit-Format-0.2.0.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxr-xr-x   0 gjbell     (501) staff       (20)        0 2023-03-25 01:06:48.588871 Better-PyUnit-Format-0.1.1/
-drwxr-xr-x   0 gjbell     (501) staff       (20)        0 2023-03-25 01:06:48.588122 Better-PyUnit-Format-0.1.1/BetterPyUnitFormat/
--rw-r--r--   0 gjbell     (501) staff       (20)     3571 2023-03-25 00:10:12.000000 Better-PyUnit-Format-0.1.1/BetterPyUnitFormat/BetterPyUnitFormat.py
--rw-r--r--   0 gjbell     (501) staff       (20)       50 2023-03-25 00:55:48.000000 Better-PyUnit-Format-0.1.1/BetterPyUnitFormat/__init__.py
-drwxr-xr-x   0 gjbell     (501) staff       (20)        0 2023-03-25 01:06:48.588620 Better-PyUnit-Format-0.1.1/Better_PyUnit_Format.egg-info/
--rw-r--r--   0 gjbell     (501) staff       (20)     2561 2023-03-25 01:06:48.000000 Better-PyUnit-Format-0.1.1/Better_PyUnit_Format.egg-info/PKG-INFO
--rw-r--r--   0 gjbell     (501) staff       (20)      280 2023-03-25 01:06:48.000000 Better-PyUnit-Format-0.1.1/Better_PyUnit_Format.egg-info/SOURCES.txt
--rw-r--r--   0 gjbell     (501) staff       (20)        1 2023-03-25 01:06:48.000000 Better-PyUnit-Format-0.1.1/Better_PyUnit_Format.egg-info/dependency_links.txt
--rw-r--r--   0 gjbell     (501) staff       (20)       19 2023-03-25 01:06:48.000000 Better-PyUnit-Format-0.1.1/Better_PyUnit_Format.egg-info/top_level.txt
--rw-r--r--   0 gjbell     (501) staff       (20)     1210 2023-03-25 00:22:37.000000 Better-PyUnit-Format-0.1.1/LICENSE
--rw-r--r--   0 gjbell     (501) staff       (20)     2561 2023-03-25 01:06:48.588755 Better-PyUnit-Format-0.1.1/PKG-INFO
--rw-r--r--   0 gjbell     (501) staff       (20)     2332 2023-03-25 01:02:54.000000 Better-PyUnit-Format-0.1.1/README.md
--rw-r--r--   0 gjbell     (501) staff       (20)      277 2023-03-25 01:05:58.000000 Better-PyUnit-Format-0.1.1/pyproject.toml
--rw-r--r--   0 gjbell     (501) staff       (20)       38 2023-03-25 01:06:48.588905 Better-PyUnit-Format-0.1.1/setup.cfg
+drwxr-xr-x   0 gjbell     (501) staff       (20)        0 2023-05-18 21:37:45.416076 Better-PyUnit-Format-0.2.0/
+drwxr-xr-x   0 gjbell     (501) staff       (20)        0 2023-05-18 21:37:45.415192 Better-PyUnit-Format-0.2.0/BetterPyUnitFormat/
+-rw-r--r--   0 gjbell     (501) staff       (20)     3571 2023-05-18 21:11:51.000000 Better-PyUnit-Format-0.2.0/BetterPyUnitFormat/BetterPyUnitResult.py
+-rw-r--r--   0 gjbell     (501) staff       (20)     1390 2023-05-18 21:20:38.000000 Better-PyUnit-Format-0.2.0/BetterPyUnitFormat/BetterPyUnitTestRunner.py
+-rw-r--r--   0 gjbell     (501) staff       (20)      116 2023-05-18 21:21:09.000000 Better-PyUnit-Format-0.2.0/BetterPyUnitFormat/__init__.py
+drwxr-xr-x   0 gjbell     (501) staff       (20)        0 2023-05-18 21:37:45.415784 Better-PyUnit-Format-0.2.0/Better_PyUnit_Format.egg-info/
+-rw-r--r--   0 gjbell     (501) staff       (20)     3008 2023-05-18 21:37:45.000000 Better-PyUnit-Format-0.2.0/Better_PyUnit_Format.egg-info/PKG-INFO
+-rw-r--r--   0 gjbell     (501) staff       (20)      325 2023-05-18 21:37:45.000000 Better-PyUnit-Format-0.2.0/Better_PyUnit_Format.egg-info/SOURCES.txt
+-rw-r--r--   0 gjbell     (501) staff       (20)        1 2023-05-18 21:37:45.000000 Better-PyUnit-Format-0.2.0/Better_PyUnit_Format.egg-info/dependency_links.txt
+-rw-r--r--   0 gjbell     (501) staff       (20)       19 2023-05-18 21:37:45.000000 Better-PyUnit-Format-0.2.0/Better_PyUnit_Format.egg-info/top_level.txt
+-rw-r--r--   0 gjbell     (501) staff       (20)     1210 2023-03-25 00:22:37.000000 Better-PyUnit-Format-0.2.0/LICENSE
+-rw-r--r--   0 gjbell     (501) staff       (20)     3008 2023-05-18 21:37:45.415943 Better-PyUnit-Format-0.2.0/PKG-INFO
+-rw-r--r--   0 gjbell     (501) staff       (20)     2779 2023-05-18 21:32:43.000000 Better-PyUnit-Format-0.2.0/README.md
+-rw-r--r--   0 gjbell     (501) staff       (20)      277 2023-05-18 21:23:31.000000 Better-PyUnit-Format-0.2.0/pyproject.toml
+-rw-r--r--   0 gjbell     (501) staff       (20)       38 2023-05-18 21:37:45.416112 Better-PyUnit-Format-0.2.0/setup.cfg
```

### Comparing `Better-PyUnit-Format-0.1.1/BetterPyUnitFormat/BetterPyUnitFormat.py` & `Better-PyUnit-Format-0.2.0/BetterPyUnitFormat/BetterPyUnitResult.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import unittest
 from math import ceil
 
 
-class BetterPyunitFormatResult(unittest.TestResult):
+class BetterPyUnitFormatResult(unittest.TestResult):
     class Colors:
         RED = u"\u001b[31m"
         GREEN = u"\u001b[32m"
         YELLOW = u"\u001b[33m"
         RESET = u"\u001b[0m"
 
     RUN = {
```

### Comparing `Better-PyUnit-Format-0.1.1/Better_PyUnit_Format.egg-info/PKG-INFO` & `Better-PyUnit-Format-0.2.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,45 +1,46 @@
-Metadata-Version: 2.1
-Name: Better-PyUnit-Format
-Version: 0.1.1
-Summary: A more readable text output for Python's built in unittest framework
-Requires-Python: >=3.5
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # Better PyUnit Format
 #### A more readable text output for Python's built in unittest framework
 
 
 ### Overview
 
-This package simply is an implementation of the `unittest.TestResult` class that sits on
-top of the `unittest.TextTestRunner` test runner. It is designed to provide a more understandable
-output to students that are just getting started with Python. It also has pretty colors.
+This package provides an implementation of a test runner and a test result for the Python unittest package.
+
+This package simply creates an override of the built-in TextTestRunner that removes all the formatting that
+it does by default and only runs the test suite. This means that this test runner passes all formatting
+responsibility on to the test result. 
+
+The test result that this package provides formats the output of the test in a much more readable way to make
+interpreting unit test results a bit easier for introductory students.
+
+This package is targeted towards students and education and was built with that limited use case in mind. 
+With that said, please, feel free to use this in your applications and tell me what you think!
 
 ### Using Better PyUnit Format
 
 1. Install the package via pip with `pip install Better-PyUnit-Format`
-2. Replace the test result in your `TextTestRunner` with BetterPyUnitFormat
+2. Import the `BetterPyUnitTestRunner`
 3. Run your testsuite!
 
 
 ### Example code
 
 ```python
+# run.py
 
 import unittest
-
-from BetterPyUnitFormat.BetterPyUnitFormat import BetterPyunitFormatResult
 import test
+from BetterPyUnitFormat import BetterPyUnitTestRunner
 
 if __name__ == "__main__":
     testSuite = unittest.loader.makeSuite(test.Test)
-    runner = unittest.TextTestRunner(resultclass=BetterPyunitFormatResult)
+    runner = BetterPyUnitTestRunner()
     runner.run(testSuite)
+
 ```
 
 ### Example Execution
 
 ```python
 # test.py
 
@@ -98,11 +99,12 @@
 [  FAILED  ] 
 1 tests passed.
 1 tests failed.
 1 tests errored.
 1 tests skipped.
 1 / 4
 ====================
-Ran 4 tests in 0.001s
 
-FAILED (failures=1, errors=1, skipped=1)
 ```
+
+### License
+This package is licensed under the Unlicense. Feel free to use it for any purpose commercial or non-commercial.
```

### Comparing `Better-PyUnit-Format-0.1.1/LICENSE` & `Better-PyUnit-Format-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `Better-PyUnit-Format-0.1.1/PKG-INFO` & `Better-PyUnit-Format-0.2.0/Better_PyUnit_Format.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,45 +1,54 @@
 Metadata-Version: 2.1
 Name: Better-PyUnit-Format
-Version: 0.1.1
+Version: 0.2.0
 Summary: A more readable text output for Python's built in unittest framework
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Better PyUnit Format
 #### A more readable text output for Python's built in unittest framework
 
 
 ### Overview
 
-This package simply is an implementation of the `unittest.TestResult` class that sits on
-top of the `unittest.TextTestRunner` test runner. It is designed to provide a more understandable
-output to students that are just getting started with Python. It also has pretty colors.
+This package provides an implementation of a test runner and a test result for the Python unittest package.
+
+This package simply creates an override of the built-in TextTestRunner that removes all the formatting that
+it does by default and only runs the test suite. This means that this test runner passes all formatting
+responsibility on to the test result. 
+
+The test result that this package provides formats the output of the test in a much more readable way to make
+interpreting unit test results a bit easier for introductory students.
+
+This package is targeted towards students and education and was built with that limited use case in mind. 
+With that said, please, feel free to use this in your applications and tell me what you think!
 
 ### Using Better PyUnit Format
 
 1. Install the package via pip with `pip install Better-PyUnit-Format`
-2. Replace the test result in your `TextTestRunner` with BetterPyUnitFormat
+2. Import the `BetterPyUnitTestRunner`
 3. Run your testsuite!
 
 
 ### Example code
 
 ```python
+# run.py
 
 import unittest
-
-from BetterPyUnitFormat.BetterPyUnitFormat import BetterPyunitFormatResult
 import test
+from BetterPyUnitFormat import BetterPyUnitTestRunner
 
 if __name__ == "__main__":
     testSuite = unittest.loader.makeSuite(test.Test)
-    runner = unittest.TextTestRunner(resultclass=BetterPyunitFormatResult)
+    runner = BetterPyUnitTestRunner()
     runner.run(testSuite)
+
 ```
 
 ### Example Execution
 
 ```python
 # test.py
 
@@ -98,11 +107,12 @@
 [  FAILED  ] 
 1 tests passed.
 1 tests failed.
 1 tests errored.
 1 tests skipped.
 1 / 4
 ====================
-Ran 4 tests in 0.001s
 
-FAILED (failures=1, errors=1, skipped=1)
 ```
+
+### License
+This package is licensed under the Unlicense. Feel free to use it for any purpose commercial or non-commercial.
```

### Comparing `Better-PyUnit-Format-0.1.1/README.md` & `Better-PyUnit-Format-0.2.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,37 +1,54 @@
+Metadata-Version: 2.1
+Name: Better-PyUnit-Format
+Version: 0.2.0
+Summary: A more readable text output for Python's built in unittest framework
+Requires-Python: >=3.5
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # Better PyUnit Format
 #### A more readable text output for Python's built in unittest framework
 
 
 ### Overview
 
-This package simply is an implementation of the `unittest.TestResult` class that sits on
-top of the `unittest.TextTestRunner` test runner. It is designed to provide a more understandable
-output to students that are just getting started with Python. It also has pretty colors.
+This package provides an implementation of a test runner and a test result for the Python unittest package.
+
+This package simply creates an override of the built-in TextTestRunner that removes all the formatting that
+it does by default and only runs the test suite. This means that this test runner passes all formatting
+responsibility on to the test result. 
+
+The test result that this package provides formats the output of the test in a much more readable way to make
+interpreting unit test results a bit easier for introductory students.
+
+This package is targeted towards students and education and was built with that limited use case in mind. 
+With that said, please, feel free to use this in your applications and tell me what you think!
 
 ### Using Better PyUnit Format
 
 1. Install the package via pip with `pip install Better-PyUnit-Format`
-2. Replace the test result in your `TextTestRunner` with BetterPyUnitFormat
+2. Import the `BetterPyUnitTestRunner`
 3. Run your testsuite!
 
 
 ### Example code
 
 ```python
+# run.py
 
 import unittest
-
-from BetterPyUnitFormat.BetterPyUnitFormat import BetterPyunitFormatResult
 import test
+from BetterPyUnitFormat import BetterPyUnitTestRunner
 
 if __name__ == "__main__":
     testSuite = unittest.loader.makeSuite(test.Test)
-    runner = unittest.TextTestRunner(resultclass=BetterPyunitFormatResult)
+    runner = BetterPyUnitTestRunner()
     runner.run(testSuite)
+
 ```
 
 ### Example Execution
 
 ```python
 # test.py
 
@@ -90,11 +107,12 @@
 [  FAILED  ] 
 1 tests passed.
 1 tests failed.
 1 tests errored.
 1 tests skipped.
 1 / 4
 ====================
-Ran 4 tests in 0.001s
 
-FAILED (failures=1, errors=1, skipped=1)
-```
+```
+
+### License
+This package is licensed under the Unlicense. Feel free to use it for any purpose commercial or non-commercial.
```

