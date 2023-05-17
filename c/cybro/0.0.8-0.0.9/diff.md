# Comparing `tmp/cybro-0.0.8.tar.gz` & `tmp/cybro-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cybro-0.0.8.tar", max compression
+gzip compressed data, was "cybro-0.0.9.tar", max compression
```

## Comparing `cybro-0.0.8.tar` & `cybro-0.0.9.tar`

### file list

```diff
@@ -1,9 +1,8 @@
--rw-r--r--   0        0        0     1069 2022-03-14 20:38:32.913093 cybro-0.0.8/LICENSE
--rw-r--r--   0        0        0     2144 2022-09-27 19:45:31.901776 cybro-0.0.8/README.md
--rw-r--r--   0        0        0     4185 2022-09-27 21:20:14.289456 cybro-0.0.8/pyproject.toml
--rw-r--r--   0        0        0      463 2022-08-16 20:14:31.723283 cybro-0.0.8/src/cybro/__init__.py
--rw-r--r--   0        0        0    13738 2022-09-27 21:20:14.289456 cybro-0.0.8/src/cybro/cybro.py
--rw-r--r--   0        0        0      450 2022-09-22 19:20:40.033235 cybro-0.0.8/src/cybro/exceptions.py
--rw-r--r--   0        0        0    14957 2022-09-27 19:45:31.905109 cybro-0.0.8/src/cybro/models.py
--rw-r--r--   0        0        0     3020 1970-01-01 00:00:00.000000 cybro-0.0.8/setup.py
--rw-r--r--   0        0        0     3699 1970-01-01 00:00:00.000000 cybro-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-05-17 23:43:06.628973 cybro-0.0.9/LICENSE
+-rw-r--r--   0        0        0     2144 2023-05-17 23:43:06.628973 cybro-0.0.9/README.md
+-rw-r--r--   0        0        0     4186 2023-05-17 23:43:06.628973 cybro-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0      463 2023-05-17 23:43:06.628973 cybro-0.0.9/src/cybro/__init__.py
+-rw-r--r--   0        0        0    14106 2023-05-17 23:43:06.628973 cybro-0.0.9/src/cybro/cybro.py
+-rw-r--r--   0        0        0      450 2023-05-17 23:43:06.628973 cybro-0.0.9/src/cybro/exceptions.py
+-rw-r--r--   0        0        0    14957 2023-05-17 23:43:06.628973 cybro-0.0.9/src/cybro/models.py
+-rw-r--r--   0        0        0     3551 1970-01-01 00:00:00.000000 cybro-0.0.9/PKG-INFO
```

### Comparing `cybro-0.0.8/LICENSE` & `cybro-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `cybro-0.0.8/README.md` & `cybro-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `cybro-0.0.8/pyproject.toml` & `cybro-0.0.9/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cybro"
-version = "0.0.8"
+version = "0.0.9"
 description = "Asynchronous Python client for Cybro scgi server."
 authors = ["Daniel Gangl <killer007@gmx.at>"]
 maintainers = ["Daniel Gangl <killer007@gmx.at>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/killer0071234/python-cybro"
 repository = "https://github.com/killer0071234/python-cybro"
@@ -31,43 +31,43 @@
 yarl = ">=1.7.2"
 backoff = ">=1.11.0"
 cachetools = ">=5.0.0"
 xmltodict = "^0.13.0"
 
 [tool.poetry.dev-dependencies]
 aresponses = "^2.1.6"
-black = "^22.6"
+black = "^22.10"
 blacken-docs = "^1.12.1"
-coverage = {version = "^6.2", extras = ["toml"]}
+coverage = {version = "^6.5", extras = ["toml"]}
 flake8 = "^4.0.1"
 flake8-docstrings = "^1.5.0"
 isort = "^5.10.1"
-mypy = "^0.981"
+mypy = "^0.982"
 pre-commit = "^2.17.0"
 pre-commit-hooks = "^4.1.0"
-pylint = "^2.15.3"
+pylint = "^2.16.3"
 pytest = "^7.1.3"
-pytest-asyncio = "^0.19.0"
-pytest-cov = "^3.0.0"
+pytest-asyncio = "^0.21.0"
+pytest-cov = "^4.0.0"
 yamllint = "^1.26.3"
-pyupgrade = "^2.38.2"
+pyupgrade = "^3.4.0"
 flake8-simplify = "^0.19.3"
 vulture = "^2.3"
 flake8-bandit = "^3.0.0"
-flake8-bugbear = "^22.9.23"
-flake8-builtins = "^1.5.3"
-flake8-comprehensions = "^3.8.0"
+flake8-bugbear = "^23.3.12"
+flake8-builtins = "^2.0.0"
+flake8-comprehensions = "^3.12.0"
 flake8-eradicate = "^1.4.0"
 flake8-markdown = "^0.3.0"
 darglint = "^1.8.1"
-safety = "^2.2.0"
-codespell = "^2.1.0"
+safety = "^2.3.1"
+codespell = "^2.2.2"
 bandit = "^1.7.0"
 types-cachetools = "^5.2.1"
-reorder-python-imports = "^3.8.3"
+reorder-python-imports = "^3.8.5"
 
 [tool.poetry.urls]
 "Bug Tracker" = "https://github.com/killer0071234/python-cybro/issues"
 Changelog = "https://github.com/killer0071234/python-cybro/releases"
 
 [tool.black]
 target-version = ['py37']
```

### Comparing `cybro-0.0.8/src/cybro/cybro.py` & `cybro-0.0.9/src/cybro/cybro.py`

 * *Files 2% similar despite different names*

```diff
@@ -362,14 +362,22 @@
     _vars[controller + "lc05_general_error"] = ""
     _vars[controller + "lc06_general_error"] = ""
     _vars[controller + "lc07_general_error"] = ""
     _vars[controller + "ld00_general_error"] = ""
     _vars[controller + "ld01_general_error"] = ""
     _vars[controller + "ld02_general_error"] = ""
     _vars[controller + "ld03_general_error"] = ""
+    _vars[controller + "ld00_rgb_mode"] = ""
+    _vars[controller + "ld01_rgb_mode"] = ""
+    _vars[controller + "ld02_rgb_mode"] = ""
+    _vars[controller + "ld03_rgb_mode"] = ""
+    _vars[controller + "ld00_rgb_mode_2"] = ""
+    _vars[controller + "ld01_rgb_mode_2"] = ""
+    _vars[controller + "ld02_rgb_mode_2"] = ""
+    _vars[controller + "ld03_rgb_mode_2"] = ""
     _vars[controller + "bc00_general_error"] = ""
     _vars[controller + "bc01_general_error"] = ""
     _vars[controller + "bc02_general_error"] = ""
     _vars[controller + "bc03_general_error"] = ""
     _vars[controller + "bc04_general_error"] = ""
     _vars[controller + "bc05_general_error"] = ""
     _vars[controller + "sc00_general_error"] = ""
```

### Comparing `cybro-0.0.8/src/cybro/models.py` & `cybro-0.0.9/src/cybro/models.py`

 * *Files identical despite different names*

### Comparing `cybro-0.0.8/setup.py` & `cybro-0.0.9/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,38 +1,78 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: cybro
+Version: 0.0.9
+Summary: Asynchronous Python client for Cybro scgi server.
+Home-page: https://github.com/killer0071234/python-cybro
+License: MIT
+Keywords: cybro,api,async,client
+Author: Daniel Gangl
+Author-email: killer007@gmx.at
+Maintainer: Daniel Gangl
+Maintainer-email: killer007@gmx.at
+Requires-Python: >=3.8,<4.0
+Classifier: Development Status :: 4 - Beta
+Classifier: Framework :: AsyncIO
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Natural Language :: English
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Requires-Dist: aiohttp (>=3.8.0)
+Requires-Dist: backoff (>=1.11.0)
+Requires-Dist: cachetools (>=5.0.0)
+Requires-Dist: xmltodict (>=0.13.0,<0.14.0)
+Requires-Dist: yarl (>=1.7.2)
+Project-URL: Bug Tracker, https://github.com/killer0071234/python-cybro/issues
+Project-URL: Changelog, https://github.com/killer0071234/python-cybro/releases
+Project-URL: Documentation, https://github.com/killer0071234/python-cybro
+Project-URL: Repository, https://github.com/killer0071234/python-cybro
+Description-Content-Type: text/markdown
+
+# python-cybro
+
+[![GitHub Release][releases-shield]][releases]
+[![GitHub Activity][commits-shield]][commits]
+[![License][license-shield]](LICENSE)
+
+[![pre-commit][pre-commit-shield]][pre-commit]
+[![Black][black-shield]][black]
+[![Code Coverage][codecov-shield]][codecov]
+
+[![Project Maintenance][maintenance-shield]][user_profile]
+
+## Functionality
+
+Python library to communicate with a cybro scgi server
+To use this library you need to have a running scgi server (it could be a docker container or native installed).
+Further information of the docker container can be found here: [![dockerhub][scgi-docker-shield]][scgi-docker]
+
+## Tested scgi server
+
+- Cybrotech scgi server v3.1.3
+
+## Contributions are welcome!
+
+If you want to contribute to this please read the [Contribution guidelines](https://github.com/killer0071234/python-cybro/blob/master/CONTRIBUTING.md)
+
+---
+
+[black]: https://github.com/psf/black
+[black-shield]: https://img.shields.io/badge/code%20style-black-000000.svg?style=for-the-badge
+[commits-shield]: https://img.shields.io/github/commit-activity/y/killer0071234/python-cybro.svg?style=for-the-badge
+[commits]: https://github.com/killer0071234/python-cybro/commits/main
+[codecov-shield]: https://img.shields.io/codecov/c/gh/killer0071234/python-cybro?style=for-the-badge&token=2VFGXXQ4N0
+[codecov]: https://codecov.io/gh/killer0071234/python-cybro
+[pre-commit]: https://github.com/pre-commit/pre-commit
+[pre-commit-shield]: https://img.shields.io/badge/pre--commit-enabled-brightgreen?style=for-the-badge
+[license-shield]: https://img.shields.io/github/license/killer0071234/python-cybro.svg?style=for-the-badge
+[maintenance-shield]: https://img.shields.io/badge/maintainer-@killer0071234-blue.svg?style=for-the-badge
+[releases-shield]: https://img.shields.io/github/release/killer0071234/python-cybro.svg?style=for-the-badge
+[releases]: https://github.com/killer0071234/python-cybro/releases
+[user_profile]: https://github.com/killer0071234
+[scgi-docker-shield]: https://img.shields.io/badge/dockerhub-cybroscgiserver-brightgreen.svg?style=for-the-badge
+[scgi-docker]: https://hub.docker.com/r/killer007/cybroscgiserver
 
-package_dir = \
-{'': 'src'}
-
-packages = \
-['cybro']
-
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['aiohttp>=3.8.0',
- 'backoff>=1.11.0',
- 'cachetools>=5.0.0',
- 'xmltodict>=0.13.0,<0.14.0',
- 'yarl>=1.7.2']
-
-setup_kwargs = {
-    'name': 'cybro',
-    'version': '0.0.8',
-    'description': 'Asynchronous Python client for Cybro scgi server.',
-    'long_description': '# python-cybro\n\n[![GitHub Release][releases-shield]][releases]\n[![GitHub Activity][commits-shield]][commits]\n[![License][license-shield]](LICENSE)\n\n[![pre-commit][pre-commit-shield]][pre-commit]\n[![Black][black-shield]][black]\n[![Code Coverage][codecov-shield]][codecov]\n\n[![Project Maintenance][maintenance-shield]][user_profile]\n\n## Functionality\n\nPython library to communicate with a cybro scgi server\nTo use this library you need to have a running scgi server (it could be a docker container or native installed).\nFurther information of the docker container can be found here: [![dockerhub][scgi-docker-shield]][scgi-docker]\n\n## Tested scgi server\n\n- Cybrotech scgi server v3.1.3\n\n## Contributions are welcome!\n\nIf you want to contribute to this please read the [Contribution guidelines](https://github.com/killer0071234/python-cybro/blob/master/CONTRIBUTING.md)\n\n---\n\n[black]: https://github.com/psf/black\n[black-shield]: https://img.shields.io/badge/code%20style-black-000000.svg?style=for-the-badge\n[commits-shield]: https://img.shields.io/github/commit-activity/y/killer0071234/python-cybro.svg?style=for-the-badge\n[commits]: https://github.com/killer0071234/python-cybro/commits/main\n[codecov-shield]: https://img.shields.io/codecov/c/gh/killer0071234/python-cybro?style=for-the-badge&token=2VFGXXQ4N0\n[codecov]: https://codecov.io/gh/killer0071234/python-cybro\n[pre-commit]: https://github.com/pre-commit/pre-commit\n[pre-commit-shield]: https://img.shields.io/badge/pre--commit-enabled-brightgreen?style=for-the-badge\n[license-shield]: https://img.shields.io/github/license/killer0071234/python-cybro.svg?style=for-the-badge\n[maintenance-shield]: https://img.shields.io/badge/maintainer-@killer0071234-blue.svg?style=for-the-badge\n[releases-shield]: https://img.shields.io/github/release/killer0071234/python-cybro.svg?style=for-the-badge\n[releases]: https://github.com/killer0071234/python-cybro/releases\n[user_profile]: https://github.com/killer0071234\n[scgi-docker-shield]: https://img.shields.io/badge/dockerhub-cybroscgiserver-brightgreen.svg?style=for-the-badge\n[scgi-docker]: https://hub.docker.com/r/killer007/cybroscgiserver\n',
-    'author': 'Daniel Gangl',
-    'author_email': 'killer007@gmx.at',
-    'maintainer': 'Daniel Gangl',
-    'maintainer_email': 'killer007@gmx.at',
-    'url': 'https://github.com/killer0071234/python-cybro',
-    'package_dir': package_dir,
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.8,<4.0',
-}
-
-
-setup(**setup_kwargs)
```

