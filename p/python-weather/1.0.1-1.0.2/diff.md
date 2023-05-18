# Comparing `tmp/python-weather-1.0.1.tar.gz` & `tmp/python-weather-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-weather-1.0.1.tar", last modified: Sat Apr 29 06:28:53 2023, max compression
+gzip compressed data, was "python-weather-1.0.2.tar", last modified: Thu May 18 11:48:31 2023, max compression
```

## Comparing `python-weather-1.0.1.tar` & `python-weather-1.0.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-04-29 06:28:53.821119 python-weather-1.0.1/
--rw-rw-rw-   0        0        0     1106 2023-04-07 14:23:45.000000 python-weather-1.0.1/LICENSE
--rw-rw-rw-   0        0        0      107 2023-04-25 12:21:36.000000 python-weather-1.0.1/MANIFEST.in
--rw-rw-rw-   0        0        0     3760 2023-04-29 06:28:53.819121 python-weather-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     2176 2023-04-29 06:26:46.000000 python-weather-1.0.1/README.md
--rw-rw-rw-   0        0        0     1437 2023-04-29 06:15:32.000000 python-weather-1.0.1/pyproject.toml
-drwxrwxrwx   0        0        0        0 2023-04-29 06:28:53.720462 python-weather-1.0.1/python_weather/
--rw-rw-rw-   0        0        0     1503 2023-04-29 06:25:45.000000 python-weather-1.0.1/python_weather/__init__.py
--rw-rw-rw-   0        0        0     5663 2023-04-29 06:25:45.000000 python-weather-1.0.1/python_weather/base.py
--rw-rw-rw-   0        0        0     5683 2023-04-29 06:25:45.000000 python-weather-1.0.1/python_weather/client.py
--rw-rw-rw-   0        0        0     1295 2023-04-29 06:25:45.000000 python-weather-1.0.1/python_weather/constants.py
--rw-rw-rw-   0        0        0    10134 2023-04-29 06:25:45.000000 python-weather-1.0.1/python_weather/enums.py
--rw-rw-rw-   0        0        0     1262 2023-04-29 06:25:45.000000 python-weather-1.0.1/python_weather/errors.py
--rw-rw-rw-   0        0        0    12805 2023-04-29 06:25:45.000000 python-weather-1.0.1/python_weather/forecast.py
-drwxrwxrwx   0        0        0        0 2023-04-29 06:28:53.815120 python-weather-1.0.1/python_weather.egg-info/
--rw-rw-rw-   0        0        0     3760 2023-04-29 06:28:52.000000 python-weather-1.0.1/python_weather.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      412 2023-04-29 06:28:53.000000 python-weather-1.0.1/python_weather.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-29 06:28:52.000000 python-weather-1.0.1/python_weather.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2023-04-29 06:28:52.000000 python-weather-1.0.1/python_weather.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-04-29 06:28:52.000000 python-weather-1.0.1/python_weather.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-29 06:28:53.821119 python-weather-1.0.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-18 11:48:31.217005 python-weather-1.0.2/
+-rw-rw-rw-   0        0        0     1106 2023-04-07 14:23:45.000000 python-weather-1.0.2/LICENSE
+-rw-rw-rw-   0        0        0      107 2023-04-25 12:21:36.000000 python-weather-1.0.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     3760 2023-05-18 11:48:31.213070 python-weather-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     2176 2023-04-29 06:26:46.000000 python-weather-1.0.2/README.md
+-rw-rw-rw-   0        0        0     1437 2023-05-18 11:41:38.000000 python-weather-1.0.2/pyproject.toml
+drwxrwxrwx   0        0        0        0 2023-05-18 11:48:31.094670 python-weather-1.0.2/python_weather/
+-rw-rw-rw-   0        0        0     1503 2023-05-18 11:41:38.000000 python-weather-1.0.2/python_weather/__init__.py
+-rw-rw-rw-   0        0        0     5663 2023-04-29 06:25:45.000000 python-weather-1.0.2/python_weather/base.py
+-rw-rw-rw-   0        0        0     5683 2023-04-29 06:25:45.000000 python-weather-1.0.2/python_weather/client.py
+-rw-rw-rw-   0        0        0     1295 2023-04-29 06:25:45.000000 python-weather-1.0.2/python_weather/constants.py
+-rw-rw-rw-   0        0        0    10130 2023-05-18 11:37:15.000000 python-weather-1.0.2/python_weather/enums.py
+-rw-rw-rw-   0        0        0     1262 2023-04-29 06:25:45.000000 python-weather-1.0.2/python_weather/errors.py
+-rw-rw-rw-   0        0        0    12867 2023-05-18 11:37:15.000000 python-weather-1.0.2/python_weather/forecast.py
+drwxrwxrwx   0        0        0        0 2023-05-18 11:48:31.191871 python-weather-1.0.2/python_weather.egg-info/
+-rw-rw-rw-   0        0        0     3760 2023-05-18 11:48:30.000000 python-weather-1.0.2/python_weather.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      412 2023-05-18 11:48:30.000000 python-weather-1.0.2/python_weather.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-18 11:48:30.000000 python-weather-1.0.2/python_weather.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2023-05-18 11:48:30.000000 python-weather-1.0.2/python_weather.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-05-18 11:48:30.000000 python-weather-1.0.2/python_weather.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-18 11:48:31.217615 python-weather-1.0.2/setup.cfg
```

### Comparing `python-weather-1.0.1/LICENSE` & `python-weather-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `python-weather-1.0.1/PKG-INFO` & `python-weather-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: python-weather
-Version: 1.0.1
+Version: 1.0.2
 Summary: A free and asynchronous weather API wrapper made in Python, for Python.
 Author: null8626
 License: MIT
 Project-URL: repository, https://github.com/null8626/python-weather
-Project-URL: download_url, https://github.com/null8626/python-weather/archive/1.0.1.tar.gz
+Project-URL: download_url, https://github.com/null8626/python-weather/archive/1.0.2.tar.gz
 Keywords: weather,forecast,weather-api,weather-forecast
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: aiohttp
 Classifier: Framework :: AsyncIO
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
```

### Comparing `python-weather-1.0.1/README.md` & `python-weather-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `python-weather-1.0.1/pyproject.toml` & `python-weather-1.0.2/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools"]
 
 [project]
 name = "python-weather"
-version = "1.0.1"
+version = "1.0.2"
 description = "A free and asynchronous weather API wrapper made in Python, for Python."
 readme = "README.md"
 license = { text = "MIT" }
 authors = [{ name = "null8626" }]
 keywords = ["weather", "forecast", "weather-api", "weather-forecast"]
 dependencies = ["aiohttp==3.8.4"]
 classifiers = [
@@ -34,8 +34,8 @@
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: 3.12"
 ]
 requires-python = ">=3.7"
 
 [project.urls]
 repository = "https://github.com/null8626/python-weather"
-download_url = "https://github.com/null8626/python-weather/archive/1.0.1.tar.gz"
+download_url = "https://github.com/null8626/python-weather/archive/1.0.2.tar.gz"
```

### Comparing `python-weather-1.0.1/python_weather/__init__.py` & `python-weather-1.0.2/python_weather/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -26,12 +26,12 @@
 """
 
 from .enums import Kind, Locale, Phase, Ultraviolet, WindDirection
 from .constants import METRIC, IMPERIAL
 from .client import Client
 from .errors import Error
 
-__version__ = '1.0.1'
+__version__ = '1.0.2'
 __all__ = (
   'METRIC', 'IMPERIAL', 'Client', 'Error', 'Kind', 'Locale', 'Phase',
   'Ultraviolet', 'WindDirection'
 )
```

### Comparing `python-weather-1.0.1/python_weather/base.py` & `python-weather-1.0.2/python_weather/base.py`

 * *Files identical despite different names*

### Comparing `python-weather-1.0.1/python_weather/client.py` & `python-weather-1.0.2/python_weather/client.py`

 * *Files identical despite different names*

### Comparing `python-weather-1.0.1/python_weather/constants.py` & `python-weather-1.0.2/python_weather/constants.py`

 * *Files identical despite different names*

### Comparing `python-weather-1.0.1/python_weather/enums.py` & `python-weather-1.0.2/python_weather/enums.py`

 * *Files 0% similar despite different names*

```diff
@@ -41,15 +41,15 @@
     return self.name.replace('_', ' ').title()
 
 class Ultraviolet(BasicEnum):
   """Represents a :term:`UV index`."""
   
   __slots__ = ()
   
-  LOW = auto()
+  LOW = 13
   MODERATE = auto()
   HIGH = auto()
   VERY_HIGH = auto()
   EXTREME = auto()
   
   @classmethod
   def _missing_(self, index: int):
```

### Comparing `python-weather-1.0.1/python_weather/errors.py` & `python-weather-1.0.2/python_weather/errors.py`

 * *Files identical despite different names*

### Comparing `python-weather-1.0.1/python_weather/forecast.py` & `python-weather-1.0.2/python_weather/forecast.py`

 * *Files 0% similar despite different names*

```diff
@@ -162,16 +162,18 @@
 class HourlyForecast(BaseForecast):
   """Represents a weather forecast of a specific hour."""
   
   __slots__ = ()
   
   def __init__(self, json: dict, unit: auto, locale: Locale):
     # for inheritance purposes
-    json['temp_C'] = json.pop('tempC')
-    json['temp_F'] = json.pop('tempF')
+    if 'temp_C' not in json:
+      json['temp_C'] = json.pop('tempC')
+    if 'temp_F' not in json:
+      json['temp_F'] = json.pop('tempF')
     
     super().__init__(json, unit, locale)
   
   def __repr__(self) -> str:
     """:class:`str`: The string representation of this object."""
     
     return f'<{self.__class__.__name__} time={self.time!r} temperature={self.temperature!r} description={self.description!r} kind={self.kind!r}>'
```

### Comparing `python-weather-1.0.1/python_weather.egg-info/PKG-INFO` & `python-weather-1.0.2/python_weather.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: python-weather
-Version: 1.0.1
+Version: 1.0.2
 Summary: A free and asynchronous weather API wrapper made in Python, for Python.
 Author: null8626
 License: MIT
 Project-URL: repository, https://github.com/null8626/python-weather
-Project-URL: download_url, https://github.com/null8626/python-weather/archive/1.0.1.tar.gz
+Project-URL: download_url, https://github.com/null8626/python-weather/archive/1.0.2.tar.gz
 Keywords: weather,forecast,weather-api,weather-forecast
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: aiohttp
 Classifier: Framework :: AsyncIO
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
```

