# Comparing `tmp/sml-exporter-0.1.4.tar.gz` & `tmp/sml_exporter-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sml-exporter-0.1.4.tar", max compression
+gzip compressed data, was "sml_exporter-0.1.5.tar", max compression
```

## Comparing `sml-exporter-0.1.4.tar` & `sml_exporter-0.1.5.tar`

### file list

```diff
@@ -1,7 +1,6 @@
--rw-r--r--   0        0        0     1055 2020-11-02 20:49:50.216482 sml-exporter-0.1.4/LICENSE
--rw-r--r--   0        0        0     9060 2022-04-04 18:04:23.401508 sml-exporter-0.1.4/README.md
--rw-r--r--   0        0        0      903 2022-04-04 19:42:02.702846 sml-exporter-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     3028 2022-04-04 18:41:44.190040 sml-exporter-0.1.4/sml_exporter/__init__.py
--rw-r--r--   0        0        0      707 2022-04-04 18:38:50.298254 sml-exporter-0.1.4/sml_exporter/__main__.py
--rw-r--r--   0        0        0    10045 2022-04-04 19:42:54.771133 sml-exporter-0.1.4/setup.py
--rw-r--r--   0        0        0     9884 2022-04-04 19:42:54.771389 sml-exporter-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1055 2020-11-02 20:49:50.216482 sml_exporter-0.1.5/LICENSE
+-rw-r--r--   0        0        0     9060 2022-04-04 18:04:23.401508 sml_exporter-0.1.5/README.md
+-rw-r--r--   0        0        0      905 2023-05-18 09:45:04.865432 sml_exporter-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     6420 2023-05-18 09:46:20.382881 sml_exporter-0.1.5/sml_exporter/__init__.py
+-rw-r--r--   0        0        0      936 2023-05-18 09:27:51.773603 sml_exporter-0.1.5/sml_exporter/__main__.py
+-rw-r--r--   0        0        0    10081 1970-01-01 00:00:00.000000 sml_exporter-0.1.5/PKG-INFO
```

### Comparing `sml-exporter-0.1.4/LICENSE` & `sml_exporter-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `sml-exporter-0.1.4/README.md` & `sml_exporter-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `sml-exporter-0.1.4/pyproject.toml` & `sml_exporter-0.1.5/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,35 +1,35 @@
 [tool.poetry]
 name = "sml-exporter"
-version = "0.1.4"
+version = "0.1.5"
 description = "Smartmeter Message Language Prometheus Exporter"
 
 license = "MIT"
 authors = ["Martin Weinelt <hexa@darmstadt.ccc.de>"]
 
 readme = "README.md"
 
 repository = "https://github.com/mweinelt/sml-exporter"
 
 keywords = ["smartmeter", "prometheus", "exporter"]
 
 classifiers = [
     "License :: OSI Approved :: MIT License",
-    "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
-    "Programming Language :: Python :: 3.10"
+    "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
 ]
 
 [tool.poetry.scripts]
 sml-exporter = "sml_exporter.__main__:main"
 
 [tool.poetry.dependencies]
-python = "^3.7"
-pysml = "^0.0.7"
+python = "^3.8"
+pysml = "0.0.11"
 prometheus-client = "^0"
 click = "^8"
 
 [tool.poetry.dev-dependencies]
 black = "*"
 isort = "*"
 mypy = "*"
```

### Comparing `sml-exporter-0.1.4/setup.py` & `sml_exporter-0.1.5/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,34 +1,170 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: sml-exporter
+Version: 0.1.5
+Summary: Smartmeter Message Language Prometheus Exporter
+Home-page: https://github.com/mweinelt/sml-exporter
+License: MIT
+Keywords: smartmeter,prometheus,exporter
+Author: Martin Weinelt
+Author-email: hexa@darmstadt.ccc.de
+Requires-Python: >=3.8,<4.0
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Requires-Dist: click (>=8,<9)
+Requires-Dist: prometheus-client (>=0,<1)
+Requires-Dist: pysml (==0.0.11)
+Project-URL: Repository, https://github.com/mweinelt/sml-exporter
+Description-Content-Type: text/markdown
+
+# sml-exporter
+
+[Prometheus](https://prometheus.io/) Exporter for smart meters that communicate using the [SML language](https://de.wikipedia.org/wiki/Smart_Message_Language), which is widely available through read-only interfaces on smart power meters in Germany.
+
+Built on top of [pysml](https://github.com/mtdcr/pysml), which does most of the heavy lifting, by parsing the message stream into python objects.
+
+## Install
+
+The [package](https://pypi.org/project/sml-exporter/) can be installed from [PyPi](https://pypi.org). It provides an executable that should be installed automatically into your environment.
+
+```
+$ python3 -m pip install sml-exporter
+```
+
+Update an existing installation using
+
+```
+$ python3 -m pip install -U sml-exporter
+```
+
+## Usage
+
+The only two options available configure the serial interface where your USB to D0 (or similiar) adapter is connected at. Setting an explicit port number is useful when you have multiple power meters.
+
+```
+❯ sml-exporter --help
+Usage: sml-exporter [OPTIONS] TTY
+
+Options:
+  -p, --http-port INTEGER RANGE  HTTP Port for the Prometheus Exporter
+                                 [default: 9761]
+
+  --help                         Show this message and exit.
+```
+
+Make sure to use stable device symlinks provided by `/dev/serial/by-id/`, so you don't mixup different serial devices.
+
+```
+# ls /dev/serial/by-id/
+usb-FTDI_FT232R_USB_UART_XXXXXXXX-if00-port0
+usb-FTDI_FT232R_USB_UART_YYYYYYYY-if00-port0
+```
+
+## Metrics
+
+Metrics are identified by their [OBIS](https://de.wikipedia.org/wiki/OBIS-Kennzahlen) numbering and transformed into a the following metrics:
+
+```
+# HELP smartmeter_wirkarbeit_verbrauch_total_wh Summe Wirkarbeit Verbrauch über alle Tarife (1-0:1.8.0*255)
+# TYPE smartmeter_wirkarbeit_verbrauch_total_wh gauge
+smartmeter_wirkarbeit_verbrauch_total_wh{device="1 EMH00 XXXXXXXX",vendor="EMH"} 6.8437382e+06
+# HELP smartmeter_wirkarbeit_lieferung_total_wh Summe Wirkarbeit Lieferung über alle Tarife (1-0:2.8.0*255)
+# TYPE smartmeter_wirkarbeit_lieferung_total_wh gauge
+smartmeter_wirkarbeit_lieferung_total_wh{device="1 EMH00 XXXXXXXX",vendor="EMH"} 5.8312058e+06
+# HELP smartmeter_wirkarbeit_verbrauch_tarif1_wh Summe Wirkarbeit Verbrauch im Tarif 1 (1-0:1.8.1*255)
+# TYPE smartmeter_wirkarbeit_verbrauch_tarif1_wh gauge
+smartmeter_wirkarbeit_verbrauch_tarif1_wh{device="1 EMH00 XXXXXXXX",vendor="EMH"} 6.8437382e+06
+# HELP smartmeter_wirkarbeit_lieferung_tarif1_wh Summe Wirkarbeit Lieferung im Tarif 1 (1-0:2.8.1*255)
+# TYPE smartmeter_wirkarbeit_lieferung_tarif1_wh gauge
+smartmeter_wirkarbeit_lieferung_tarif1_wh{device="1 EMH00 XXXXXXXX",vendor="EMH"} 5.8312058e+06
+# HELP smartmeter_wirkarbeit_verbrauch_tarif2_wh Summe Wirkarbeit Verbrauch im Tarif 2 (1-0:1.8.2*255)
+# TYPE smartmeter_wirkarbeit_verbrauch_tarif2_wh gauge
+smartmeter_wirkarbeit_verbrauch_tarif2_wh{device="1 EMH00 XXXXXXXX",vendor="EMH"} 0.0
+# HELP smartmeter_wirkarbeit_lieferung_tarif2_wh Summe Wirkarbeit Lieferung im Tarif 2 (1-0:2.8.2*255)
+# TYPE smartmeter_wirkarbeit_lieferung_tarif2_wh gauge
+smartmeter_wirkarbeit_lieferung_tarif2_wh{device="1 EMH00 XXXXXXXX",vendor="EMH"} 0.0
+# HELP smartmeter_wirkleistung_w Momentane Wirkleistung (1-0:16.7.0*255)
+# TYPE smartmeter_wirkleistung_w gauge
+smartmeter_wirkleistung_w{device="1 EMH00 XXXXXXXX",vendor="EMH"} 892.4
+# HELP smartmeter_wirkarbeit_verbrauch_total_wh Summe Wirkarbeit Verbrauch über alle Tarife (1-0:1.8.0*255)
+# TYPE smartmeter_wirkarbeit_verbrauch_total_wh gauge
+smartmeter_wirkarbeit_verbrauch_total_wh{device="1 EMH00 XXXXXXXX",vendor="EMH"} 6.8437382e+06
+# HELP smartmeter_wirkarbeit_lieferung_total_wh Summe Wirkarbeit Lieferung über alle Tarife (1-0:2.8.0*255)
+# TYPE smartmeter_wirkarbeit_lieferung_total_wh gauge
+smartmeter_wirkarbeit_lieferung_total_wh{device="1 EMH00 XXXXXXXX",vendor="EMH"} 5.8312058e+06
+# HELP smartmeter_wirkarbeit_verbrauch_tarif1_wh Summe Wirkarbeit Verbrauch im Tarif 1 (1-0:1.8.1*255)
+# TYPE smartmeter_wirkarbeit_verbrauch_tarif1_wh gauge
+smartmeter_wirkarbeit_verbrauch_tarif1_wh{device="1 EMH00 XXXXXXXX",vendor="EMH"} 6.8437382e+06
+# HELP smartmeter_wirkarbeit_lieferung_tarif1_wh Summe Wirkarbeit Lieferung im Tarif 1 (1-0:2.8.1*255)
+# TYPE smartmeter_wirkarbeit_lieferung_tarif1_wh gauge
+smartmeter_wirkarbeit_lieferung_tarif1_wh{device="1 EMH00 XXXXXXXX",vendor="EMH"} 5.8312058e+06
+# HELP smartmeter_wirkarbeit_verbrauch_tarif2_wh Summe Wirkarbeit Verbrauch im Tarif 2 (1-0:1.8.2*255)
+# TYPE smartmeter_wirkarbeit_verbrauch_tarif2_wh gauge
+smartmeter_wirkarbeit_verbrauch_tarif2_wh{device="1 EMH00 XXXXXXXX",vendor="EMH"} 0.0
+# HELP smartmeter_wirkarbeit_lieferung_tarif2_wh Summe Wirkarbeit Lieferung im Tarif 2 (1-0:2.8.2*255)
+# TYPE smartmeter_wirkarbeit_lieferung_tarif2_wh gauge
+smartmeter_wirkarbeit_lieferung_tarif2_wh{device="1 EMH00 XXXXXXXX",vendor="EMH"} 0.0
+# HELP smartmeter_wirkleistung_w Momentane Wirkleistung (1-0:16.7.0*255)
+# TYPE smartmeter_wirkleistung_w gauge
+smartmeter_wirkleistung_w{device="1 EMH00 XXXXXXXX",vendor="EMH"} 892.4# HELP smartmeter_wirkarbeit_verbrauch_total_wh Summe Wirkarbeit Verbrauch über alle Tarife (1-0:1.8.0*255)
+# TYPE smartmeter_wirkarbeit_verbrauch_total_wh gauge
+smartmeter_wirkarbeit_verbrauch_total_wh{device="1 EMH00 XXXXXXXX",vendor="EMH"} 6.8437382e+06
+# HELP smartmeter_wirkarbeit_lieferung_total_wh Summe Wirkarbeit Lieferung über alle Tarife (1-0:2.8.0*255)
+# TYPE smartmeter_wirkarbeit_lieferung_total_wh gauge
+smartmeter_wirkarbeit_lieferung_total_wh{device="1 EMH00 XXXXXXXX",vendor="EMH"} 5.8312058e+06
+# HELP smartmeter_wirkarbeit_verbrauch_tarif1_wh Summe Wirkarbeit Verbrauch im Tarif 1 (1-0:1.8.1*255)
+# TYPE smartmeter_wirkarbeit_verbrauch_tarif1_wh gauge
+smartmeter_wirkarbeit_verbrauch_tarif1_wh{device="1 EMH00 XXXXXXXX",vendor="EMH"} 6.8437382e+06
+# HELP smartmeter_wirkarbeit_lieferung_tarif1_wh Summe Wirkarbeit Lieferung im Tarif 1 (1-0:2.8.1*255)
+# TYPE smartmeter_wirkarbeit_lieferung_tarif1_wh gauge
+smartmeter_wirkarbeit_lieferung_tarif1_wh{device="1 EMH00 XXXXXXXX",vendor="EMH"} 5.8312058e+06
+# HELP smartmeter_wirkarbeit_verbrauch_tarif2_wh Summe Wirkarbeit Verbrauch im Tarif 2 (1-0:1.8.2*255)
+# TYPE smartmeter_wirkarbeit_verbrauch_tarif2_wh gauge
+smartmeter_wirkarbeit_verbrauch_tarif2_wh{device="1 EMH00 XXXXXXXX",vendor="EMH"} 0.0
+# HELP smartmeter_wirkarbeit_lieferung_tarif2_wh Summe Wirkarbeit Lieferung im Tarif 2 (1-0:2.8.2*255)
+# TYPE smartmeter_wirkarbeit_lieferung_tarif2_wh gauge
+smartmeter_wirkarbeit_lieferung_tarif2_wh{device="1 EMH00 XXXXXXXX",vendor="EMH"} 0.0
+# HELP smartmeter_wirkleistung_w Momentane Wirkleistung (1-0:16.7.0*255)
+# TYPE smartmeter_wirkleistung_w gauge
+smartmeter_wirkleistung_w{device="1 EMH00 XXXXXXXX",vendor="EMH"} 892.4# HELP smartmeter_wirkarbeit_verbrauch_total_wh Summe Wirkarbeit Verbrauch über alle Tarife (1-0:1.8.0*255)
+# TYPE smartmeter_wirkarbeit_verbrauch_total_wh gauge
+smartmeter_wirkarbeit_verbrauch_total_wh{device="1 EMH00 XXXXXXXX",vendor="EMH"} 6.8437382e+06
+# HELP smartmeter_wirkarbeit_lieferung_total_wh Summe Wirkarbeit Lieferung über alle Tarife (1-0:2.8.0*255)
+# TYPE smartmeter_wirkarbeit_lieferung_total_wh gauge
+smartmeter_wirkarbeit_lieferung_total_wh{device="1 EMH00 XXXXXXXX",vendor="EMH"} 5.8312058e+06
+# HELP smartmeter_wirkarbeit_verbrauch_tarif1_wh Summe Wirkarbeit Verbrauch im Tarif 1 (1-0:1.8.1*255)
+# TYPE smartmeter_wirkarbeit_verbrauch_tarif1_wh gauge
+smartmeter_wirkarbeit_verbrauch_tarif1_wh{device="1 EMH00 XXXXXXXX",vendor="EMH"} 6.8437382e+06
+# HELP smartmeter_wirkarbeit_lieferung_tarif1_wh Summe Wirkarbeit Lieferung im Tarif 1 (1-0:2.8.1*255)
+# TYPE smartmeter_wirkarbeit_lieferung_tarif1_wh gauge
+smartmeter_wirkarbeit_lieferung_tarif1_wh{device="1 EMH00 XXXXXXXX",vendor="EMH"} 5.8312058e+06
+# HELP smartmeter_wirkarbeit_verbrauch_tarif2_wh Summe Wirkarbeit Verbrauch im Tarif 2 (1-0:1.8.2*255)
+# TYPE smartmeter_wirkarbeit_verbrauch_tarif2_wh gauge
+smartmeter_wirkarbeit_verbrauch_tarif2_wh{device="1 EMH00 XXXXXXXX",vendor="EMH"} 0.0
+# HELP smartmeter_wirkarbeit_lieferung_tarif2_wh Summe Wirkarbeit Lieferung im Tarif 2 (1-0:2.8.2*255)
+# TYPE smartmeter_wirkarbeit_lieferung_tarif2_wh gauge
+smartmeter_wirkarbeit_lieferung_tarif2_wh{device="1 EMH00 XXXXXXXX",vendor="EMH"} 0.0
+# HELP smartmeter_wirkleistung_w Momentane Wirkleistung (1-0:16.7.0*255)
+# TYPE smartmeter_wirkleistung_w gauge
+smartmeter_wirkleistung_w{device="1 EMH00 XXXXXXXX",vendor="EMH"} 892.4
+```
+
+## Caveats
+
+The exporter caches new values as they arrive, until they are overwritten by newer ones. This design was chosen as the arrival of data usually does not match up with any particular polling interval.
+In an ideal world we would migrate this exporter to reuse [pushgateway](https://github.com/prometheus/pushgateway). This did not happen because I don't have any experience using it.
+
+## License
+
+This software is provided under the [MIT license](LICENSE) and uses
+  - [pysml](https://pypi.org/project/pysml/) MIT
+  - [click](https://pypi.org/project/click/) BSD3
+  - [prometheus-client](https://pypi.org/project/prometheus-client/) ASL20
 
-packages = \
-['sml_exporter']
-
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['click>=8,<9', 'prometheus-client>=0,<1', 'pysml>=0.0.7,<0.0.8']
-
-entry_points = \
-{'console_scripts': ['sml-exporter = sml_exporter.__main__:main']}
-
-setup_kwargs = {
-    'name': 'sml-exporter',
-    'version': '0.1.4',
-    'description': 'Smartmeter Message Language Prometheus Exporter',
-    'long_description': '# sml-exporter\n\n[Prometheus](https://prometheus.io/) Exporter for smart meters that communicate using the [SML language](https://de.wikipedia.org/wiki/Smart_Message_Language), which is widely available through read-only interfaces on smart power meters in Germany.\n\nBuilt on top of [pysml](https://github.com/mtdcr/pysml), which does most of the heavy lifting, by parsing the message stream into python objects.\n\n## Install\n\nThe [package](https://pypi.org/project/sml-exporter/) can be installed from [PyPi](https://pypi.org). It provides an executable that should be installed automatically into your environment.\n\n```\n$ python3 -m pip install sml-exporter\n```\n\nUpdate an existing installation using\n\n```\n$ python3 -m pip install -U sml-exporter\n```\n\n## Usage\n\nThe only two options available configure the serial interface where your USB to D0 (or similiar) adapter is connected at. Setting an explicit port number is useful when you have multiple power meters.\n\n```\n❯ sml-exporter --help\nUsage: sml-exporter [OPTIONS] TTY\n\nOptions:\n  -p, --http-port INTEGER RANGE  HTTP Port for the Prometheus Exporter\n                                 [default: 9761]\n\n  --help                         Show this message and exit.\n```\n\nMake sure to use stable device symlinks provided by `/dev/serial/by-id/`, so you don\'t mixup different serial devices.\n\n```\n# ls /dev/serial/by-id/\nusb-FTDI_FT232R_USB_UART_XXXXXXXX-if00-port0\nusb-FTDI_FT232R_USB_UART_YYYYYYYY-if00-port0\n```\n\n## Metrics\n\nMetrics are identified by their [OBIS](https://de.wikipedia.org/wiki/OBIS-Kennzahlen) numbering and transformed into a the following metrics:\n\n```\n# HELP smartmeter_wirkarbeit_verbrauch_total_wh Summe Wirkarbeit Verbrauch über alle Tarife (1-0:1.8.0*255)\n# TYPE smartmeter_wirkarbeit_verbrauch_total_wh gauge\nsmartmeter_wirkarbeit_verbrauch_total_wh{device="1 EMH00 XXXXXXXX",vendor="EMH"} 6.8437382e+06\n# HELP smartmeter_wirkarbeit_lieferung_total_wh Summe Wirkarbeit Lieferung über alle Tarife (1-0:2.8.0*255)\n# TYPE smartmeter_wirkarbeit_lieferung_total_wh gauge\nsmartmeter_wirkarbeit_lieferung_total_wh{device="1 EMH00 XXXXXXXX",vendor="EMH"} 5.8312058e+06\n# HELP smartmeter_wirkarbeit_verbrauch_tarif1_wh Summe Wirkarbeit Verbrauch im Tarif 1 (1-0:1.8.1*255)\n# TYPE smartmeter_wirkarbeit_verbrauch_tarif1_wh gauge\nsmartmeter_wirkarbeit_verbrauch_tarif1_wh{device="1 EMH00 XXXXXXXX",vendor="EMH"} 6.8437382e+06\n# HELP smartmeter_wirkarbeit_lieferung_tarif1_wh Summe Wirkarbeit Lieferung im Tarif 1 (1-0:2.8.1*255)\n# TYPE smartmeter_wirkarbeit_lieferung_tarif1_wh gauge\nsmartmeter_wirkarbeit_lieferung_tarif1_wh{device="1 EMH00 XXXXXXXX",vendor="EMH"} 5.8312058e+06\n# HELP smartmeter_wirkarbeit_verbrauch_tarif2_wh Summe Wirkarbeit Verbrauch im Tarif 2 (1-0:1.8.2*255)\n# TYPE smartmeter_wirkarbeit_verbrauch_tarif2_wh gauge\nsmartmeter_wirkarbeit_verbrauch_tarif2_wh{device="1 EMH00 XXXXXXXX",vendor="EMH"} 0.0\n# HELP smartmeter_wirkarbeit_lieferung_tarif2_wh Summe Wirkarbeit Lieferung im Tarif 2 (1-0:2.8.2*255)\n# TYPE smartmeter_wirkarbeit_lieferung_tarif2_wh gauge\nsmartmeter_wirkarbeit_lieferung_tarif2_wh{device="1 EMH00 XXXXXXXX",vendor="EMH"} 0.0\n# HELP smartmeter_wirkleistung_w Momentane Wirkleistung (1-0:16.7.0*255)\n# TYPE smartmeter_wirkleistung_w gauge\nsmartmeter_wirkleistung_w{device="1 EMH00 XXXXXXXX",vendor="EMH"} 892.4\n# HELP smartmeter_wirkarbeit_verbrauch_total_wh Summe Wirkarbeit Verbrauch über alle Tarife (1-0:1.8.0*255)\n# TYPE smartmeter_wirkarbeit_verbrauch_total_wh gauge\nsmartmeter_wirkarbeit_verbrauch_total_wh{device="1 EMH00 XXXXXXXX",vendor="EMH"} 6.8437382e+06\n# HELP smartmeter_wirkarbeit_lieferung_total_wh Summe Wirkarbeit Lieferung über alle Tarife (1-0:2.8.0*255)\n# TYPE smartmeter_wirkarbeit_lieferung_total_wh gauge\nsmartmeter_wirkarbeit_lieferung_total_wh{device="1 EMH00 XXXXXXXX",vendor="EMH"} 5.8312058e+06\n# HELP smartmeter_wirkarbeit_verbrauch_tarif1_wh Summe Wirkarbeit Verbrauch im Tarif 1 (1-0:1.8.1*255)\n# TYPE smartmeter_wirkarbeit_verbrauch_tarif1_wh gauge\nsmartmeter_wirkarbeit_verbrauch_tarif1_wh{device="1 EMH00 XXXXXXXX",vendor="EMH"} 6.8437382e+06\n# HELP smartmeter_wirkarbeit_lieferung_tarif1_wh Summe Wirkarbeit Lieferung im Tarif 1 (1-0:2.8.1*255)\n# TYPE smartmeter_wirkarbeit_lieferung_tarif1_wh gauge\nsmartmeter_wirkarbeit_lieferung_tarif1_wh{device="1 EMH00 XXXXXXXX",vendor="EMH"} 5.8312058e+06\n# HELP smartmeter_wirkarbeit_verbrauch_tarif2_wh Summe Wirkarbeit Verbrauch im Tarif 2 (1-0:1.8.2*255)\n# TYPE smartmeter_wirkarbeit_verbrauch_tarif2_wh gauge\nsmartmeter_wirkarbeit_verbrauch_tarif2_wh{device="1 EMH00 XXXXXXXX",vendor="EMH"} 0.0\n# HELP smartmeter_wirkarbeit_lieferung_tarif2_wh Summe Wirkarbeit Lieferung im Tarif 2 (1-0:2.8.2*255)\n# TYPE smartmeter_wirkarbeit_lieferung_tarif2_wh gauge\nsmartmeter_wirkarbeit_lieferung_tarif2_wh{device="1 EMH00 XXXXXXXX",vendor="EMH"} 0.0\n# HELP smartmeter_wirkleistung_w Momentane Wirkleistung (1-0:16.7.0*255)\n# TYPE smartmeter_wirkleistung_w gauge\nsmartmeter_wirkleistung_w{device="1 EMH00 XXXXXXXX",vendor="EMH"} 892.4# HELP smartmeter_wirkarbeit_verbrauch_total_wh Summe Wirkarbeit Verbrauch über alle Tarife (1-0:1.8.0*255)\n# TYPE smartmeter_wirkarbeit_verbrauch_total_wh gauge\nsmartmeter_wirkarbeit_verbrauch_total_wh{device="1 EMH00 XXXXXXXX",vendor="EMH"} 6.8437382e+06\n# HELP smartmeter_wirkarbeit_lieferung_total_wh Summe Wirkarbeit Lieferung über alle Tarife (1-0:2.8.0*255)\n# TYPE smartmeter_wirkarbeit_lieferung_total_wh gauge\nsmartmeter_wirkarbeit_lieferung_total_wh{device="1 EMH00 XXXXXXXX",vendor="EMH"} 5.8312058e+06\n# HELP smartmeter_wirkarbeit_verbrauch_tarif1_wh Summe Wirkarbeit Verbrauch im Tarif 1 (1-0:1.8.1*255)\n# TYPE smartmeter_wirkarbeit_verbrauch_tarif1_wh gauge\nsmartmeter_wirkarbeit_verbrauch_tarif1_wh{device="1 EMH00 XXXXXXXX",vendor="EMH"} 6.8437382e+06\n# HELP smartmeter_wirkarbeit_lieferung_tarif1_wh Summe Wirkarbeit Lieferung im Tarif 1 (1-0:2.8.1*255)\n# TYPE smartmeter_wirkarbeit_lieferung_tarif1_wh gauge\nsmartmeter_wirkarbeit_lieferung_tarif1_wh{device="1 EMH00 XXXXXXXX",vendor="EMH"} 5.8312058e+06\n# HELP smartmeter_wirkarbeit_verbrauch_tarif2_wh Summe Wirkarbeit Verbrauch im Tarif 2 (1-0:1.8.2*255)\n# TYPE smartmeter_wirkarbeit_verbrauch_tarif2_wh gauge\nsmartmeter_wirkarbeit_verbrauch_tarif2_wh{device="1 EMH00 XXXXXXXX",vendor="EMH"} 0.0\n# HELP smartmeter_wirkarbeit_lieferung_tarif2_wh Summe Wirkarbeit Lieferung im Tarif 2 (1-0:2.8.2*255)\n# TYPE smartmeter_wirkarbeit_lieferung_tarif2_wh gauge\nsmartmeter_wirkarbeit_lieferung_tarif2_wh{device="1 EMH00 XXXXXXXX",vendor="EMH"} 0.0\n# HELP smartmeter_wirkleistung_w Momentane Wirkleistung (1-0:16.7.0*255)\n# TYPE smartmeter_wirkleistung_w gauge\nsmartmeter_wirkleistung_w{device="1 EMH00 XXXXXXXX",vendor="EMH"} 892.4# HELP smartmeter_wirkarbeit_verbrauch_total_wh Summe Wirkarbeit Verbrauch über alle Tarife (1-0:1.8.0*255)\n# TYPE smartmeter_wirkarbeit_verbrauch_total_wh gauge\nsmartmeter_wirkarbeit_verbrauch_total_wh{device="1 EMH00 XXXXXXXX",vendor="EMH"} 6.8437382e+06\n# HELP smartmeter_wirkarbeit_lieferung_total_wh Summe Wirkarbeit Lieferung über alle Tarife (1-0:2.8.0*255)\n# TYPE smartmeter_wirkarbeit_lieferung_total_wh gauge\nsmartmeter_wirkarbeit_lieferung_total_wh{device="1 EMH00 XXXXXXXX",vendor="EMH"} 5.8312058e+06\n# HELP smartmeter_wirkarbeit_verbrauch_tarif1_wh Summe Wirkarbeit Verbrauch im Tarif 1 (1-0:1.8.1*255)\n# TYPE smartmeter_wirkarbeit_verbrauch_tarif1_wh gauge\nsmartmeter_wirkarbeit_verbrauch_tarif1_wh{device="1 EMH00 XXXXXXXX",vendor="EMH"} 6.8437382e+06\n# HELP smartmeter_wirkarbeit_lieferung_tarif1_wh Summe Wirkarbeit Lieferung im Tarif 1 (1-0:2.8.1*255)\n# TYPE smartmeter_wirkarbeit_lieferung_tarif1_wh gauge\nsmartmeter_wirkarbeit_lieferung_tarif1_wh{device="1 EMH00 XXXXXXXX",vendor="EMH"} 5.8312058e+06\n# HELP smartmeter_wirkarbeit_verbrauch_tarif2_wh Summe Wirkarbeit Verbrauch im Tarif 2 (1-0:1.8.2*255)\n# TYPE smartmeter_wirkarbeit_verbrauch_tarif2_wh gauge\nsmartmeter_wirkarbeit_verbrauch_tarif2_wh{device="1 EMH00 XXXXXXXX",vendor="EMH"} 0.0\n# HELP smartmeter_wirkarbeit_lieferung_tarif2_wh Summe Wirkarbeit Lieferung im Tarif 2 (1-0:2.8.2*255)\n# TYPE smartmeter_wirkarbeit_lieferung_tarif2_wh gauge\nsmartmeter_wirkarbeit_lieferung_tarif2_wh{device="1 EMH00 XXXXXXXX",vendor="EMH"} 0.0\n# HELP smartmeter_wirkleistung_w Momentane Wirkleistung (1-0:16.7.0*255)\n# TYPE smartmeter_wirkleistung_w gauge\nsmartmeter_wirkleistung_w{device="1 EMH00 XXXXXXXX",vendor="EMH"} 892.4\n```\n\n## Caveats\n\nThe exporter caches new values as they arrive, until they are overwritten by newer ones. This design was chosen as the arrival of data usually does not match up with any particular polling interval.\nIn an ideal world we would migrate this exporter to reuse [pushgateway](https://github.com/prometheus/pushgateway). This did not happen because I don\'t have any experience using it.\n\n## License\n\nThis software is provided under the [MIT license](LICENSE) and uses\n  - [pysml](https://pypi.org/project/pysml/) MIT\n  - [click](https://pypi.org/project/click/) BSD3\n  - [prometheus-client](https://pypi.org/project/prometheus-client/) ASL20\n',
-    'author': 'Martin Weinelt',
-    'author_email': 'hexa@darmstadt.ccc.de',
-    'maintainer': None,
-    'maintainer_email': None,
-    'url': 'https://github.com/mweinelt/sml-exporter',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'entry_points': entry_points,
-    'python_requires': '>=3.7,<4.0',
-}
-
-
-setup(**setup_kwargs)
```

