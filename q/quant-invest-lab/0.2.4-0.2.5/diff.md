# Comparing `tmp/quant_invest_lab-0.2.4.tar.gz` & `tmp/quant_invest_lab-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quant_invest_lab-0.2.4.tar", max compression
+gzip compressed data, was "quant_invest_lab-0.2.5.tar", max compression
```

## Comparing `quant_invest_lab-0.2.4.tar` & `quant_invest_lab-0.2.5.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     4427 2023-05-15 20:43:54.661278 quant_invest_lab-0.2.4/README.md
--rw-r--r--   0        0        0      978 2023-05-15 20:43:54.661278 quant_invest_lab-0.2.4/pyproject.toml
--rw-r--r--   0        0        0    32590 2023-05-15 20:43:54.661278 quant_invest_lab-0.2.4/quant_invest_lab/backtest.py
--rw-r--r--   0        0        0    17110 2023-05-15 20:43:54.661278 quant_invest_lab-0.2.4/quant_invest_lab/data_provider.py
--rw-r--r--   0        0        0    26301 2023-05-15 20:43:54.661278 quant_invest_lab-0.2.4/quant_invest_lab/indicators.py
--rw-r--r--   0        0        0     9477 2023-05-15 20:43:54.661278 quant_invest_lab-0.2.4/quant_invest_lab/metrics.py
--rw-r--r--   0        0        0     7659 2023-05-15 20:43:54.661278 quant_invest_lab-0.2.4/quant_invest_lab/optimization.py
--rw-r--r--   0        0        0    20461 2023-05-15 20:43:54.661278 quant_invest_lab-0.2.4/quant_invest_lab/portfolio.py
--rw-r--r--   0        0        0     3577 2023-05-15 20:43:54.661278 quant_invest_lab-0.2.4/quant_invest_lab/screener.py
--rw-r--r--   0        0        0     8477 2023-05-15 20:43:54.661278 quant_invest_lab-0.2.4/quant_invest_lab/simulation.py
--rw-r--r--   0        0        0     1107 2023-05-15 20:43:54.661278 quant_invest_lab-0.2.4/quant_invest_lab/utils.py
--rw-r--r--   0        0        0     5745 1970-01-01 00:00:00.000000 quant_invest_lab-0.2.4/PKG-INFO
+-rw-r--r--   0        0        0     5026 2023-05-18 12:53:57.987333 quant_invest_lab-0.2.5/README.md
+-rw-r--r--   0        0        0      978 2023-05-18 12:53:57.991333 quant_invest_lab-0.2.5/pyproject.toml
+-rw-r--r--   0        0        0    32590 2023-05-18 12:53:57.991333 quant_invest_lab-0.2.5/quant_invest_lab/backtest.py
+-rw-r--r--   0        0        0    17110 2023-05-18 12:53:57.991333 quant_invest_lab-0.2.5/quant_invest_lab/data_provider.py
+-rw-r--r--   0        0        0    26301 2023-05-18 12:53:57.991333 quant_invest_lab-0.2.5/quant_invest_lab/indicators.py
+-rw-r--r--   0        0        0     9477 2023-05-18 12:53:57.991333 quant_invest_lab-0.2.5/quant_invest_lab/metrics.py
+-rw-r--r--   0        0        0     7659 2023-05-18 12:53:57.991333 quant_invest_lab-0.2.5/quant_invest_lab/optimization.py
+-rw-r--r--   0        0        0    20461 2023-05-18 12:53:57.991333 quant_invest_lab-0.2.5/quant_invest_lab/portfolio.py
+-rw-r--r--   0        0        0     3577 2023-05-18 12:53:57.991333 quant_invest_lab-0.2.5/quant_invest_lab/screener.py
+-rw-r--r--   0        0        0     8477 2023-05-18 12:53:57.991333 quant_invest_lab-0.2.5/quant_invest_lab/simulation.py
+-rw-r--r--   0        0        0     1107 2023-05-18 12:53:57.991333 quant_invest_lab-0.2.5/quant_invest_lab/utils.py
+-rw-r--r--   0        0        0     6344 1970-01-01 00:00:00.000000 quant_invest_lab-0.2.5/PKG-INFO
```

### Comparing `quant_invest_lab-0.2.4/README.md` & `quant_invest_lab-0.2.5/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,13 +1,18 @@
 # Quant Invest Lab
 <p align="left">
 <a href="https://pypi.org/project/quant-invest-lab/"><img alt="PyPI" src="https://img.shields.io/pypi/v/quant-invest-lab"></a>
 <a><img alt="commit update" src="https://img.shields.io/github/last-commit/BaptisteZloch/Quant-Invest-Lab"></a>
 <a href="https://github.com/psf/black"><img alt="Code style: black" src="https://img.shields.io/badge/code%20style-black-000000.svg"></a>
-</p>
+<a href="https://codeclimate.com/github/BaptisteZloch/Quant-Invest-Lab"><img alt="Code Climate" src="https://codeclimate.com/github/BaptisteZloch/Quant-Invest-Lab/badges/gpa.svg"></a>
+<a href="https://github.com/BaptisteZloch/Quant-Invest-Lab/blob/master/.github/workflows/python-publish.yml"><img alt="GitHub Actions CI" src="https://github.com/BaptisteZloch/Quant-Invest-Lab/actions/workflows/python-publish.yml/badge.svg"></a>
+
+[![contributions welcome](https://img.shields.io/badge/contributions-welcome-brightgreen.svg?style=flat-square)](https://github.com/BaptisteZloch/Quant-Invest-Lab/issues)
+
+
 
 **Quant Invest Lab** is a project aimed to provide a set of basic tools for quantitative experiments. By quantitative experiment I mean trying to build you own set of investments solution. The project is still in its early stage, but I hope it will grow in the future. 
 
 Initially this project was aimed to be a set of tools for my own experiments, but I decided to make it open source. Of courses it already exists some awesome packages, more detailed, better suited for some use cases. But I hope it will be useful for someone else (learn, practice, understand and create). Feel free to use it, modify it and contribute to it. This package is basically the package I wanted to find when I started to learn quantitative finance.
 ## Main features
 - **Data**: download data from external data provider without restriction on candle stick, the main provider is kucoin for now (currently only crypto data are supported).
 - **Backtesting**: backtest your trading strategy (Long only for now but soon short and leverage) on historical data for different timeframe. Optimize you take profit, stop loss. Access full metrics of your strategy.
```

#### html2text {}

```diff
@@ -1,21 +1,23 @@
 # Quant Invest Lab
-[PyPI] [commit update] [Code_style:_black]
-**Quant Invest Lab** is a project aimed to provide a set of basic tools for
-quantitative experiments. By quantitative experiment I mean trying to build you
-own set of investments solution. The project is still in its early stage, but I
-hope it will grow in the future. Initially this project was aimed to be a set
-of tools for my own experiments, but I decided to make it open source. Of
-courses it already exists some awesome packages, more detailed, better suited
-for some use cases. But I hope it will be useful for someone else (learn,
-practice, understand and create). Feel free to use it, modify it and contribute
-to it. This package is basically the package I wanted to find when I started to
-learn quantitative finance. ## Main features - **Data**: download data from
-external data provider without restriction on candle stick, the main provider
-is kucoin for now (currently only crypto data are supported). -
+[PyPI] [commit update] [Code_style:_black] [Code_Climate] [GitHub_Actions_CI]
+[![contributions welcome](https://img.shields.io/badge/contributions-welcome-
+brightgreen.svg?style=flat-square)](https://github.com/BaptisteZloch/Quant-
+Invest-Lab/issues) **Quant Invest Lab** is a project aimed to provide a set of
+basic tools for quantitative experiments. By quantitative experiment I mean
+trying to build you own set of investments solution. The project is still in
+its early stage, but I hope it will grow in the future. Initially this project
+was aimed to be a set of tools for my own experiments, but I decided to make it
+open source. Of courses it already exists some awesome packages, more detailed,
+better suited for some use cases. But I hope it will be useful for someone else
+(learn, practice, understand and create). Feel free to use it, modify it and
+contribute to it. This package is basically the package I wanted to find when I
+started to learn quantitative finance. ## Main features - **Data**: download
+data from external data provider without restriction on candle stick, the main
+provider is kucoin for now (currently only crypto data are supported). -
 **Backtesting**: backtest your trading strategy (Long only for now but soon
 short and leverage) on historical data for different timeframe. Optimize you
 take profit, stop loss. Access full metrics of your strategy. - **Indicators**:
 a set of indicators to help you build your strategy. - **Portfolio**: a set of
 portfolio optimization tools to help you build your portfolio. -
 **Simulation**: simulate your data based on real data using statistics to get a
 better understanding of its behavior during backtesting. - **Metrics**: a set
```

### Comparing `quant_invest_lab-0.2.4/pyproject.toml` & `quant_invest_lab-0.2.5/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 [tool.poetry]
 name = "quant-invest-lab"
-version = "0.2.4"
+version = "0.2.5"
 description = "Quant Invest Lab is a python package to help you to do some quantitative experiments, while trying to learn or build quantitative investment solutions. This project was initially my own set of functionnalities but I decided to build a package for that and sharing it as open source project."
 authors = ["BaptisteZloch <bzloch@hotmail.fr>"]
 readme = "README.md"
 packages = [{include = "quant_invest_lab"}]
 
 [tool.poetry.dependencies]
 python = ">=3.8,<3.12"
-pandas = "^2.0.1"
+pandas = "^1.5.3"
 scipy = "^1.10.1"
 statsmodels = "^0.14.0"
 kucoin-python = "^1.0.11"
-numpy = "^1.24.3"
+numpy = "^1.23.5"
 ta = "^0.10.2"
 plotly = "^5.14.1"
 nbformat = "^5.8.0"
 matplotlib = "^3.7.1"
 seaborn = "^0.12.2"
 tqdm = "^4.65.0"
 beautifulsoup4 = "^4.12.2"
```

### Comparing `quant_invest_lab-0.2.4/quant_invest_lab/backtest.py` & `quant_invest_lab-0.2.5/quant_invest_lab/backtest.py`

 * *Files identical despite different names*

### Comparing `quant_invest_lab-0.2.4/quant_invest_lab/data_provider.py` & `quant_invest_lab-0.2.5/quant_invest_lab/data_provider.py`

 * *Files identical despite different names*

### Comparing `quant_invest_lab-0.2.4/quant_invest_lab/indicators.py` & `quant_invest_lab-0.2.5/quant_invest_lab/indicators.py`

 * *Files identical despite different names*

### Comparing `quant_invest_lab-0.2.4/quant_invest_lab/metrics.py` & `quant_invest_lab-0.2.5/quant_invest_lab/metrics.py`

 * *Files identical despite different names*

### Comparing `quant_invest_lab-0.2.4/quant_invest_lab/optimization.py` & `quant_invest_lab-0.2.5/quant_invest_lab/optimization.py`

 * *Files identical despite different names*

### Comparing `quant_invest_lab-0.2.4/quant_invest_lab/portfolio.py` & `quant_invest_lab-0.2.5/quant_invest_lab/portfolio.py`

 * *Files identical despite different names*

### Comparing `quant_invest_lab-0.2.4/quant_invest_lab/screener.py` & `quant_invest_lab-0.2.5/quant_invest_lab/screener.py`

 * *Files identical despite different names*

### Comparing `quant_invest_lab-0.2.4/quant_invest_lab/simulation.py` & `quant_invest_lab-0.2.5/quant_invest_lab/simulation.py`

 * *Files identical despite different names*

### Comparing `quant_invest_lab-0.2.4/quant_invest_lab/utils.py` & `quant_invest_lab-0.2.5/quant_invest_lab/utils.py`

 * *Files identical despite different names*

### Comparing `quant_invest_lab-0.2.4/PKG-INFO` & `quant_invest_lab-0.2.5/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,41 +1,46 @@
 Metadata-Version: 2.1
 Name: quant-invest-lab
-Version: 0.2.4
+Version: 0.2.5
 Summary: Quant Invest Lab is a python package to help you to do some quantitative experiments, while trying to learn or build quantitative investment solutions. This project was initially my own set of functionnalities but I decided to build a package for that and sharing it as open source project.
 Author: BaptisteZloch
 Author-email: bzloch@hotmail.fr
 Requires-Python: >=3.8,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: beautifulsoup4 (>=4.12.2,<5.0.0)
 Requires-Dist: fitter (>=1.5.2,<2.0.0)
 Requires-Dist: kucoin-python (>=1.0.11,<2.0.0)
 Requires-Dist: matplotlib (>=3.7.1,<4.0.0)
 Requires-Dist: nbformat (>=5.8.0,<6.0.0)
-Requires-Dist: numpy (>=1.24.3,<2.0.0)
-Requires-Dist: pandas (>=2.0.1,<3.0.0)
+Requires-Dist: numpy (>=1.23.5,<2.0.0)
+Requires-Dist: pandas (>=1.5.3,<2.0.0)
 Requires-Dist: plotly (>=5.14.1,<6.0.0)
 Requires-Dist: scikit-learn (>=1.2.2,<2.0.0)
 Requires-Dist: scipy (>=1.10.1,<2.0.0)
 Requires-Dist: seaborn (>=0.12.2,<0.13.0)
 Requires-Dist: statsmodels (>=0.14.0,<0.15.0)
 Requires-Dist: ta (>=0.10.2,<0.11.0)
 Requires-Dist: tqdm (>=4.65.0,<5.0.0)
 Description-Content-Type: text/markdown
 
 # Quant Invest Lab
 <p align="left">
 <a href="https://pypi.org/project/quant-invest-lab/"><img alt="PyPI" src="https://img.shields.io/pypi/v/quant-invest-lab"></a>
 <a><img alt="commit update" src="https://img.shields.io/github/last-commit/BaptisteZloch/Quant-Invest-Lab"></a>
 <a href="https://github.com/psf/black"><img alt="Code style: black" src="https://img.shields.io/badge/code%20style-black-000000.svg"></a>
-</p>
+<a href="https://codeclimate.com/github/BaptisteZloch/Quant-Invest-Lab"><img alt="Code Climate" src="https://codeclimate.com/github/BaptisteZloch/Quant-Invest-Lab/badges/gpa.svg"></a>
+<a href="https://github.com/BaptisteZloch/Quant-Invest-Lab/blob/master/.github/workflows/python-publish.yml"><img alt="GitHub Actions CI" src="https://github.com/BaptisteZloch/Quant-Invest-Lab/actions/workflows/python-publish.yml/badge.svg"></a>
+
+[![contributions welcome](https://img.shields.io/badge/contributions-welcome-brightgreen.svg?style=flat-square)](https://github.com/BaptisteZloch/Quant-Invest-Lab/issues)
+
+
 
 **Quant Invest Lab** is a project aimed to provide a set of basic tools for quantitative experiments. By quantitative experiment I mean trying to build you own set of investments solution. The project is still in its early stage, but I hope it will grow in the future. 
 
 Initially this project was aimed to be a set of tools for my own experiments, but I decided to make it open source. Of courses it already exists some awesome packages, more detailed, better suited for some use cases. But I hope it will be useful for someone else (learn, practice, understand and create). Feel free to use it, modify it and contribute to it. This package is basically the package I wanted to find when I started to learn quantitative finance.
 ## Main features
 - **Data**: download data from external data provider without restriction on candle stick, the main provider is kucoin for now (currently only crypto data are supported).
 - **Backtesting**: backtest your trading strategy (Long only for now but soon short and leverage) on historical data for different timeframe. Optimize you take profit, stop loss. Access full metrics of your strategy.
```

#### html2text {}

```diff
@@ -1,38 +1,40 @@
-Metadata-Version: 2.1 Name: quant-invest-lab Version: 0.2.4 Summary: Quant
+Metadata-Version: 2.1 Name: quant-invest-lab Version: 0.2.5 Summary: Quant
 Invest Lab is a python package to help you to do some quantitative experiments,
 while trying to learn or build quantitative investment solutions. This project
 was initially my own set of functionnalities but I decided to build a package
 for that and sharing it as open source project. Author: BaptisteZloch Author-
 email: bzloch@hotmail.fr Requires-Python: >=3.8,<3.12 Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: beautifulsoup4 (>=4.12.2,<5.0.0) Requires-Dist: fitter
 (>=1.5.2,<2.0.0) Requires-Dist: kucoin-python (>=1.0.11,<2.0.0) Requires-Dist:
 matplotlib (>=3.7.1,<4.0.0) Requires-Dist: nbformat (>=5.8.0,<6.0.0) Requires-
-Dist: numpy (>=1.24.3,<2.0.0) Requires-Dist: pandas (>=2.0.1,<3.0.0) Requires-
+Dist: numpy (>=1.23.5,<2.0.0) Requires-Dist: pandas (>=1.5.3,<2.0.0) Requires-
 Dist: plotly (>=5.14.1,<6.0.0) Requires-Dist: scikit-learn (>=1.2.2,<2.0.0)
 Requires-Dist: scipy (>=1.10.1,<2.0.0) Requires-Dist: seaborn
 (>=0.12.2,<0.13.0) Requires-Dist: statsmodels (>=0.14.0,<0.15.0) Requires-Dist:
 ta (>=0.10.2,<0.11.0) Requires-Dist: tqdm (>=4.65.0,<5.0.0) Description-
 Content-Type: text/markdown # Quant Invest Lab
-[PyPI] [commit update] [Code_style:_black]
-**Quant Invest Lab** is a project aimed to provide a set of basic tools for
-quantitative experiments. By quantitative experiment I mean trying to build you
-own set of investments solution. The project is still in its early stage, but I
-hope it will grow in the future. Initially this project was aimed to be a set
-of tools for my own experiments, but I decided to make it open source. Of
-courses it already exists some awesome packages, more detailed, better suited
-for some use cases. But I hope it will be useful for someone else (learn,
-practice, understand and create). Feel free to use it, modify it and contribute
-to it. This package is basically the package I wanted to find when I started to
-learn quantitative finance. ## Main features - **Data**: download data from
-external data provider without restriction on candle stick, the main provider
-is kucoin for now (currently only crypto data are supported). -
+[PyPI] [commit update] [Code_style:_black] [Code_Climate] [GitHub_Actions_CI]
+[![contributions welcome](https://img.shields.io/badge/contributions-welcome-
+brightgreen.svg?style=flat-square)](https://github.com/BaptisteZloch/Quant-
+Invest-Lab/issues) **Quant Invest Lab** is a project aimed to provide a set of
+basic tools for quantitative experiments. By quantitative experiment I mean
+trying to build you own set of investments solution. The project is still in
+its early stage, but I hope it will grow in the future. Initially this project
+was aimed to be a set of tools for my own experiments, but I decided to make it
+open source. Of courses it already exists some awesome packages, more detailed,
+better suited for some use cases. But I hope it will be useful for someone else
+(learn, practice, understand and create). Feel free to use it, modify it and
+contribute to it. This package is basically the package I wanted to find when I
+started to learn quantitative finance. ## Main features - **Data**: download
+data from external data provider without restriction on candle stick, the main
+provider is kucoin for now (currently only crypto data are supported). -
 **Backtesting**: backtest your trading strategy (Long only for now but soon
 short and leverage) on historical data for different timeframe. Optimize you
 take profit, stop loss. Access full metrics of your strategy. - **Indicators**:
 a set of indicators to help you build your strategy. - **Portfolio**: a set of
 portfolio optimization tools to help you build your portfolio. -
 **Simulation**: simulate your data based on real data using statistics to get a
 better understanding of its behavior during backtesting. - **Metrics**: a set
```

