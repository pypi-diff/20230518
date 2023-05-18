# Comparing `tmp/rapt_ble-0.1.0.tar.gz` & `tmp/rapt_ble-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rapt_ble-0.1.0.tar", max compression
+gzip compressed data, was "rapt_ble-0.1.1.tar", max compression
```

## Comparing `rapt_ble-0.1.0.tar` & `rapt_ble-0.1.1.tar`

### file list

```diff
@@ -1,8 +1,7 @@
--rw-r--r--   0        0        0     1070 2023-02-10 20:24:55.290634 rapt_ble-0.1.0/LICENSE
--rw-r--r--   0        0        0     3468 2023-02-10 20:24:55.290634 rapt_ble-0.1.0/README.md
--rw-r--r--   0        0        0     2283 2023-02-10 20:24:56.402640 rapt_ble-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      348 2023-02-10 20:24:56.346640 rapt_ble-0.1.0/src/rapt_ble/__init__.py
--rw-r--r--   0        0        0     4731 2023-02-10 20:24:55.290634 rapt_ble-0.1.0/src/rapt_ble/parser.py
--rw-r--r--   0        0        0        0 2023-02-10 20:24:55.290634 rapt_ble-0.1.0/src/rapt_ble/py.typed
--rw-r--r--   0        0        0     4364 1970-01-01 00:00:00.000000 rapt_ble-0.1.0/setup.py
--rw-r--r--   0        0        0     4707 1970-01-01 00:00:00.000000 rapt_ble-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-05-18 16:44:30.063591 rapt_ble-0.1.1/LICENSE
+-rw-r--r--   0        0        0     3468 2023-05-18 16:44:30.063591 rapt_ble-0.1.1/README.md
+-rw-r--r--   0        0        0     2283 2023-05-18 16:44:30.851588 rapt_ble-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      348 2023-05-18 16:44:30.815588 rapt_ble-0.1.1/src/rapt_ble/__init__.py
+-rw-r--r--   0        0        0     5427 2023-05-18 16:44:30.067591 rapt_ble-0.1.1/src/rapt_ble/parser.py
+-rw-r--r--   0        0        0        0 2023-05-18 16:44:30.067591 rapt_ble-0.1.1/src/rapt_ble/py.typed
+-rw-r--r--   0        0        0     4707 1970-01-01 00:00:00.000000 rapt_ble-0.1.1/PKG-INFO
```

### Comparing `rapt_ble-0.1.0/LICENSE` & `rapt_ble-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `rapt_ble-0.1.0/README.md` & `rapt_ble-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `rapt_ble-0.1.0/pyproject.toml` & `rapt_ble-0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "rapt-ble"
-version = "0.1.0"
+version = "0.1.1"
 description = "Parser for the RAPT Pill hydrometer BLE packets."
 authors = ["Jan Čermák <sairon@sairon.cz>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/sairon/rapt-ble"
 documentation = "https://rapt-ble.readthedocs.io"
 classifiers = [
```

### Comparing `rapt_ble-0.1.0/src/rapt_ble/parser.py` & `rapt_ble-0.1.1/src/rapt_ble/parser.py`

 * *Files 6% similar despite different names*

```diff
@@ -22,45 +22,64 @@
     def _process_metrics(self, data: bytes) -> None:
         """
         Process advertisement with metrics.
 
         This is what the advertisement data payload looks like in C,
         endianness is big endian:
 
+        Version 1 (with MAC, no gravity velocity):
+
         typedef struct __attribute__((packed)) {
             char prefix[4];        // RAPT
             uint8_t version;       // always 0x01
             uint8_t mac[6];
             uint16_t temperature;  // x / 128 - 273.15
             float gravity;         // / 1000
             int16_t x;             // x / 16
             int16_t y;             // x / 16
             int16_t z;             // x / 16
             int16_t battery;       // x / 256
-        } RAPTPillMetrics;
+        } RAPTPillMetricsV1;
+
+        Version 2 (no MAC, with gravity velocity):
+
+        typedef struct __attribute__((packed)) {
+            char prefix[4];        // RAPT
+            uint8_t version;       // always 0x02
+            bool gravity_velocity_valid;
+            float gravity_velocity;
+            uint16_t temperature;  // x / 128 - 273.15
+            float gravity;         // / 1000
+            int16_t x;             // x / 16
+            int16_t y;             // x / 16
+            int16_t z;             // x / 16
+            int16_t battery;       // x / 256
+        } RAPTPillMetricsV2;
         """
         if len(data) != 23:
             raise ValueError("Metrics data must have length 23")
 
         # get "raw" data, drop second part of the prefix ("PT"), start with the version
         metrics_raw = RAPTPillMetrics._make(unpack(">B6sHfhhhh", data[2:]))
 
         # convert to actual metrics
         metrics = RAPTPillMetrics(
             version=metrics_raw.version,
-            mac=hexlify(metrics_raw.mac).decode("ascii"),
+            mac=hexlify(metrics_raw.mac).decode("ascii")
+            if metrics_raw.version == 1
+            else "",
             temperature=round(metrics_raw.temperature / 128 - 273.15, 2),
             gravity=round(metrics_raw.gravity / 1000, 4),
             x=metrics_raw.x / 16,
             y=metrics_raw.y / 16,
             z=metrics_raw.z / 16,
             battery=round(metrics_raw.battery / 256),
         )
 
-        if metrics.version != 1:
+        if metrics.version <= 2:
             _LOGGER.warning(
                 "Unexpected RAPT payload version %d, measurements may be incorrect!",
                 metrics.version,
             )
 
         _LOGGER.debug("Parsed RAPT Pill data: %s", metrics)
```

### Comparing `rapt_ble-0.1.0/setup.py` & `rapt_ble-0.1.1/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,37 +1,89 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: rapt-ble
+Version: 0.1.1
+Summary: Parser for the RAPT Pill hydrometer BLE packets.
+Home-page: https://github.com/sairon/rapt-ble
+License: MIT
+Author: Jan Čermák
+Author-email: sairon@sairon.cz
+Requires-Python: >=3.9,<4.0
+Classifier: Development Status :: 2 - Pre-Alpha
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Natural Language :: English
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Software Development :: Libraries
+Requires-Dist: bluetooth-data-tools (>=0.3.1)
+Requires-Dist: bluetooth-sensor-state-data (>=1.6.1)
+Requires-Dist: home-assistant-bluetooth (>=1.9.2)
+Requires-Dist: sensor-state-data (>=2.13.0)
+Project-URL: Bug Tracker, https://github.com/sairon/rapt-ble/issues
+Project-URL: Changelog, https://github.com/sairon/rapt-ble/blob/main/CHANGELOG.md
+Project-URL: Documentation, https://rapt-ble.readthedocs.io
+Project-URL: Repository, https://github.com/sairon/rapt-ble
+Description-Content-Type: text/markdown
+
+# RAPT BLE
+
+<p align="center">
+  <a href="https://github.com/sairon/rapt-ble/actions/workflows/ci.yml?query=branch%3Amain">
+    <img src="https://img.shields.io/github/actions/workflow/status/sairon/rapt-ble/ci.yml?branch=main&label=CI&logo=github&style=flat-square" alt="CI Status" >
+  </a>
+  <a href="https://rapt-ble.readthedocs.io">
+    <img src="https://img.shields.io/readthedocs/rapt-ble.svg?logo=read-the-docs&logoColor=fff&style=flat-square" alt="Documentation Status">
+  </a>
+  <a href="https://codecov.io/gh/sairon/rapt-ble">
+    <img src="https://img.shields.io/codecov/c/github/sairon/rapt-ble.svg?logo=codecov&logoColor=fff&style=flat-square" alt="Test coverage percentage">
+  </a>
+</p>
+<p align="center">
+  <a href="https://python-poetry.org/">
+    <img src="https://img.shields.io/badge/packaging-poetry-299bd7?style=flat-square&logo=data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAA4AAAASCAYAAABrXO8xAAAACXBIWXMAAAsTAAALEwEAmpwYAAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAJJSURBVHgBfZLPa1NBEMe/s7tNXoxW1KJQKaUHkXhQvHgW6UHQQ09CBS/6V3hKc/AP8CqCrUcpmop3Cx48eDB4yEECjVQrlZb80CRN8t6OM/teagVxYZi38+Yz853dJbzoMV3MM8cJUcLMSUKIE8AzQ2PieZzFxEJOHMOgMQQ+dUgSAckNXhapU/NMhDSWLs1B24A8sO1xrN4NECkcAC9ASkiIJc6k5TRiUDPhnyMMdhKc+Zx19l6SgyeW76BEONY9exVQMzKExGKwwPsCzza7KGSSWRWEQhyEaDXp6ZHEr416ygbiKYOd7TEWvvcQIeusHYMJGhTwF9y7sGnSwaWyFAiyoxzqW0PM/RjghPxF2pWReAowTEXnDh0xgcLs8l2YQmOrj3N7ByiqEoH0cARs4u78WgAVkoEDIDoOi3AkcLOHU60RIg5wC4ZuTC7FaHKQm8Hq1fQuSOBvX/sodmNJSB5geaF5CPIkUeecdMxieoRO5jz9bheL6/tXjrwCyX/UYBUcjCaWHljx1xiX6z9xEjkYAzbGVnB8pvLmyXm9ep+W8CmsSHQQY77Zx1zboxAV0w7ybMhQmfqdmmw3nEp1I0Z+FGO6M8LZdoyZnuzzBdjISicKRnpxzI9fPb+0oYXsNdyi+d3h9bm9MWYHFtPeIZfLwzmFDKy1ai3p+PDls1Llz4yyFpferxjnyjJDSEy9CaCx5m2cJPerq6Xm34eTrZt3PqxYO1XOwDYZrFlH1fWnpU38Y9HRze3lj0vOujZcXKuuXm3jP+s3KbZVra7y2EAAAAAASUVORK5CYII=" alt="Poetry">
+  </a>
+  <a href="https://github.com/ambv/black">
+    <img src="https://img.shields.io/badge/code%20style-black-000000.svg?style=flat-square" alt="black">
+  </a>
+  <a href="https://github.com/pre-commit/pre-commit">
+    <img src="https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white&style=flat-square" alt="pre-commit">
+  </a>
+</p>
+<p align="center">
+  <a href="https://pypi.org/project/rapt-ble/">
+    <img src="https://img.shields.io/pypi/v/rapt-ble.svg?logo=python&logoColor=fff&style=flat-square" alt="PyPI Version">
+  </a>
+  <img src="https://img.shields.io/pypi/pyversions/rapt-ble.svg?style=flat-square&logo=python&amp;logoColor=fff" alt="Supported Python versions">
+  <img src="https://img.shields.io/pypi/l/rapt-ble.svg?style=flat-square" alt="License">
+</p>
+
+Parser for the RAPT Pill hydrometer BLE packets.
+
+## Installation
+
+Install this via pip (or your favourite package manager):
+
+`pip install rapt-ble`
+
+## Contributors ✨
+
+Thanks goes to these wonderful people ([emoji key](https://allcontributors.org/docs/en/emoji-key)):
+
+<!-- prettier-ignore-start -->
+<!-- ALL-CONTRIBUTORS-LIST:START - Do not remove or modify this section -->
+<!-- markdownlint-disable -->
+<!-- markdownlint-enable -->
+<!-- ALL-CONTRIBUTORS-LIST:END -->
+<!-- prettier-ignore-end -->
+
+This project follows the [all-contributors](https://github.com/all-contributors/all-contributors) specification. Contributions of any kind welcome!
+
+## Credits
+
+This package was created with
+[Copier](https://copier.readthedocs.io/) and the
+[browniebroke/pypackage-template](https://github.com/browniebroke/pypackage-template)
+project template.
 
-package_dir = \
-{'': 'src'}
-
-packages = \
-['rapt_ble']
-
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['bluetooth-data-tools>=0.3.1',
- 'bluetooth-sensor-state-data>=1.6.1',
- 'home-assistant-bluetooth>=1.9.2',
- 'sensor-state-data>=2.13.0']
-
-setup_kwargs = {
-    'name': 'rapt-ble',
-    'version': '0.1.0',
-    'description': 'Parser for the RAPT Pill hydrometer BLE packets.',
-    'long_description': '# RAPT BLE\n\n<p align="center">\n  <a href="https://github.com/sairon/rapt-ble/actions/workflows/ci.yml?query=branch%3Amain">\n    <img src="https://img.shields.io/github/actions/workflow/status/sairon/rapt-ble/ci.yml?branch=main&label=CI&logo=github&style=flat-square" alt="CI Status" >\n  </a>\n  <a href="https://rapt-ble.readthedocs.io">\n    <img src="https://img.shields.io/readthedocs/rapt-ble.svg?logo=read-the-docs&logoColor=fff&style=flat-square" alt="Documentation Status">\n  </a>\n  <a href="https://codecov.io/gh/sairon/rapt-ble">\n    <img src="https://img.shields.io/codecov/c/github/sairon/rapt-ble.svg?logo=codecov&logoColor=fff&style=flat-square" alt="Test coverage percentage">\n  </a>\n</p>\n<p align="center">\n  <a href="https://python-poetry.org/">\n    <img src="https://img.shields.io/badge/packaging-poetry-299bd7?style=flat-square&logo=data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAA4AAAASCAYAAABrXO8xAAAACXBIWXMAAAsTAAALEwEAmpwYAAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAJJSURBVHgBfZLPa1NBEMe/s7tNXoxW1KJQKaUHkXhQvHgW6UHQQ09CBS/6V3hKc/AP8CqCrUcpmop3Cx48eDB4yEECjVQrlZb80CRN8t6OM/teagVxYZi38+Yz853dJbzoMV3MM8cJUcLMSUKIE8AzQ2PieZzFxEJOHMOgMQQ+dUgSAckNXhapU/NMhDSWLs1B24A8sO1xrN4NECkcAC9ASkiIJc6k5TRiUDPhnyMMdhKc+Zx19l6SgyeW76BEONY9exVQMzKExGKwwPsCzza7KGSSWRWEQhyEaDXp6ZHEr416ygbiKYOd7TEWvvcQIeusHYMJGhTwF9y7sGnSwaWyFAiyoxzqW0PM/RjghPxF2pWReAowTEXnDh0xgcLs8l2YQmOrj3N7ByiqEoH0cARs4u78WgAVkoEDIDoOi3AkcLOHU60RIg5wC4ZuTC7FaHKQm8Hq1fQuSOBvX/sodmNJSB5geaF5CPIkUeecdMxieoRO5jz9bheL6/tXjrwCyX/UYBUcjCaWHljx1xiX6z9xEjkYAzbGVnB8pvLmyXm9ep+W8CmsSHQQY77Zx1zboxAV0w7ybMhQmfqdmmw3nEp1I0Z+FGO6M8LZdoyZnuzzBdjISicKRnpxzI9fPb+0oYXsNdyi+d3h9bm9MWYHFtPeIZfLwzmFDKy1ai3p+PDls1Llz4yyFpferxjnyjJDSEy9CaCx5m2cJPerq6Xm34eTrZt3PqxYO1XOwDYZrFlH1fWnpU38Y9HRze3lj0vOujZcXKuuXm3jP+s3KbZVra7y2EAAAAAASUVORK5CYII=" alt="Poetry">\n  </a>\n  <a href="https://github.com/ambv/black">\n    <img src="https://img.shields.io/badge/code%20style-black-000000.svg?style=flat-square" alt="black">\n  </a>\n  <a href="https://github.com/pre-commit/pre-commit">\n    <img src="https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white&style=flat-square" alt="pre-commit">\n  </a>\n</p>\n<p align="center">\n  <a href="https://pypi.org/project/rapt-ble/">\n    <img src="https://img.shields.io/pypi/v/rapt-ble.svg?logo=python&logoColor=fff&style=flat-square" alt="PyPI Version">\n  </a>\n  <img src="https://img.shields.io/pypi/pyversions/rapt-ble.svg?style=flat-square&logo=python&amp;logoColor=fff" alt="Supported Python versions">\n  <img src="https://img.shields.io/pypi/l/rapt-ble.svg?style=flat-square" alt="License">\n</p>\n\nParser for the RAPT Pill hydrometer BLE packets.\n\n## Installation\n\nInstall this via pip (or your favourite package manager):\n\n`pip install rapt-ble`\n\n## Contributors ✨\n\nThanks goes to these wonderful people ([emoji key](https://allcontributors.org/docs/en/emoji-key)):\n\n<!-- prettier-ignore-start -->\n<!-- ALL-CONTRIBUTORS-LIST:START - Do not remove or modify this section -->\n<!-- markdownlint-disable -->\n<!-- markdownlint-enable -->\n<!-- ALL-CONTRIBUTORS-LIST:END -->\n<!-- prettier-ignore-end -->\n\nThis project follows the [all-contributors](https://github.com/all-contributors/all-contributors) specification. Contributions of any kind welcome!\n\n## Credits\n\nThis package was created with\n[Copier](https://copier.readthedocs.io/) and the\n[browniebroke/pypackage-template](https://github.com/browniebroke/pypackage-template)\nproject template.\n',
-    'author': 'Jan Čermák',
-    'author_email': 'sairon@sairon.cz',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://github.com/sairon/rapt-ble',
-    'package_dir': package_dir,
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.9,<4.0',
-}
-
-
-setup(**setup_kwargs)
```

#### html2text {}

```diff
@@ -1,26 +1,29 @@
-# -*- coding: utf-8 -*- from setuptools import setup package_dir = \ {'':
-'src'} packages = \ ['rapt_ble'] package_data = \ {'': ['*']} install_requires
-= \ ['bluetooth-data-tools>=0.3.1', 'bluetooth-sensor-state-data>=1.6.1',
-'home-assistant-bluetooth>=1.9.2', 'sensor-state-data>=2.13.0'] setup_kwargs =
-{ 'name': 'rapt-ble', 'version': '0.1.0', 'description': 'Parser for the RAPT
-Pill hydrometer BLE packets.', 'long_description': '# RAPT BLE\n\n
-     \n \n_[CI_Status]\n\n \n_[Documentation_Status]\n\n \n_[Test_coverage
-                                percentage]\n\n
-\n
-             \n \n_[Poetry]\n\n \n_[black]\n\n \n_[pre-commit]\n\n
-\n
-      \n \n_[PyPI_Version]\n\n [Supported Python versions]\n [License]\n
-\n\nParser for the RAPT Pill hydrometer BLE packets.\n\n##
-Installation\n\nInstall this via pip (or your favourite package manager):
-\n\n`pip install rapt-ble`\n\n## Contributors â¨\n\nThanks goes to these
-wonderful people ([emoji key](https://allcontributors.org/docs/en/emoji-key)):
-\n\n\n\n\n\n\n\n\nThis project follows the [all-contributors](https://
-github.com/all-contributors/all-contributors) specification. Contributions of
-any kind welcome!\n\n## Credits\n\nThis package was created with\n[Copier]
-(https://copier.readthedocs.io/) and the\n[browniebroke/pypackage-template]
-(https://github.com/browniebroke/pypackage-template)\nproject template.\n',
-'author': 'Jan ÄermÃ¡k', 'author_email': 'sairon@sairon.cz', 'maintainer':
-'None', 'maintainer_email': 'None', 'url': 'https://github.com/sairon/rapt-
-ble', 'package_dir': package_dir, 'packages': packages, 'package_data':
-package_data, 'install_requires': install_requires, 'python_requires':
-'>=3.9,<4.0', } setup(**setup_kwargs)
+Metadata-Version: 2.1 Name: rapt-ble Version: 0.1.1 Summary: Parser for the
+RAPT Pill hydrometer BLE packets. Home-page: https://github.com/sairon/rapt-ble
+License: MIT Author: Jan ÄermÃ¡k Author-email: sairon@sairon.cz Requires-
+Python: >=3.9,<4.0 Classifier: Development Status :: 2 - Pre-Alpha Classifier:
+Intended Audience :: Developers Classifier: License :: OSI Approved :: MIT
+License Classifier: Natural Language :: English Classifier: Operating System ::
+OS Independent Classifier: Programming Language :: Python :: 3 Classifier:
+Programming Language :: Python :: 3.9 Classifier: Programming Language ::
+Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
+Topic :: Software Development :: Libraries Requires-Dist: bluetooth-data-tools
+(>=0.3.1) Requires-Dist: bluetooth-sensor-state-data (>=1.6.1) Requires-Dist:
+home-assistant-bluetooth (>=1.9.2) Requires-Dist: sensor-state-data (>=2.13.0)
+Project-URL: Bug Tracker, https://github.com/sairon/rapt-ble/issues Project-
+URL: Changelog, https://github.com/sairon/rapt-ble/blob/main/CHANGELOG.md
+Project-URL: Documentation, https://rapt-ble.readthedocs.io Project-URL:
+Repository, https://github.com/sairon/rapt-ble Description-Content-Type: text/
+markdown # RAPT BLE
+         [CI_Status] [Documentation_Status] [Test_coverage_percentage]
+                         [Poetry] [black] [pre-commit]
+             [PyPI_Version] [Supported Python versions] [License]
+Parser for the RAPT Pill hydrometer BLE packets. ## Installation Install this
+via pip (or your favourite package manager): `pip install rapt-ble` ##
+Contributors â¨ Thanks goes to these wonderful people ([emoji key](https://
+allcontributors.org/docs/en/emoji-key)):       This project follows the [all-
+contributors](https://github.com/all-contributors/all-contributors)
+specification. Contributions of any kind welcome! ## Credits This package was
+created with [Copier](https://copier.readthedocs.io/) and the [browniebroke/
+pypackage-template](https://github.com/browniebroke/pypackage-template) project
+template.
```

