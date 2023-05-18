# Comparing `tmp/iloscar_win-0.1.4.tar.gz` & `tmp/iloscar_win-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iloscar_win-0.1.4.tar", last modified: Thu May 18 17:20:35 2023, max compression
+gzip compressed data, was "iloscar_win-0.1.5.tar", last modified: Thu May 18 17:24:57 2023, max compression
```

## Comparing `iloscar_win-0.1.4.tar` & `iloscar_win-0.1.5.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-05-18 17:20:35.100375 iloscar_win-0.1.4/
--rw-rw-rw-   0        0        0    18548 2023-05-18 17:20:35.097381 iloscar_win-0.1.4/PKG-INFO
--rw-rw-rw-   0        0        0    17783 2023-05-18 16:23:09.000000 iloscar_win-0.1.4/README.md
-drwxrwxrwx   0        0        0        0 2023-05-18 17:20:35.035607 iloscar_win-0.1.4/iloscar_win/
--rw-rw-rw-   0        0        0      350 2023-05-18 17:19:34.000000 iloscar_win-0.1.4/iloscar_win/__init__.py
--rw-rw-rw-   0        0        0     1951 2023-05-18 17:00:12.000000 iloscar_win-0.1.4/iloscar_win/app.py
--rw-rw-rw-   0        0        0   106422 2023-05-18 16:23:10.000000 iloscar_win-0.1.4/iloscar_win/iLOSCAR_backend.py
-drwxrwxrwx   0        0        0        0 2023-05-18 17:20:35.091884 iloscar_win-0.1.4/iloscar_win/pages/
--rw-rw-rw-   0        0        0     5797 2023-05-18 17:01:06.000000 iloscar_win-0.1.4/iloscar_win/pages/Function.py
--rw-rw-rw-   0        0        0    26245 2023-05-18 17:00:56.000000 iloscar_win-0.1.4/iloscar_win/pages/forward.py
--rw-rw-rw-   0        0        0      887 2023-05-18 17:01:55.000000 iloscar_win-0.1.4/iloscar_win/pages/home.py
--rw-rw-rw-   0        0        0    46215 2023-05-18 17:01:22.000000 iloscar_win-0.1.4/iloscar_win/pages/inverse.py
--rw-rw-rw-   0        0        0     1357 2023-05-18 16:23:10.000000 iloscar_win-0.1.4/iloscar_win/style.py
-drwxrwxrwx   0        0        0        0 2023-05-18 17:20:35.080547 iloscar_win-0.1.4/iloscar_win.egg-info/
--rw-rw-rw-   0        0        0    18548 2023-05-18 17:20:34.000000 iloscar_win-0.1.4/iloscar_win.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      401 2023-05-18 17:20:34.000000 iloscar_win-0.1.4/iloscar_win.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-18 17:20:34.000000 iloscar_win-0.1.4/iloscar_win.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      131 2023-05-18 17:20:34.000000 iloscar_win-0.1.4/iloscar_win.egg-info/requires.txt
--rw-rw-rw-   0        0        0       30 2023-05-18 17:20:34.000000 iloscar_win-0.1.4/iloscar_win.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-18 17:20:35.100375 iloscar_win-0.1.4/setup.cfg
--rw-rw-rw-   0        0        0     1509 2023-05-18 17:19:47.000000 iloscar_win-0.1.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-18 17:24:57.646412 iloscar_win-0.1.5/
+-rw-rw-rw-   0        0        0    18548 2023-05-18 17:24:57.643057 iloscar_win-0.1.5/PKG-INFO
+-rw-rw-rw-   0        0        0    17783 2023-05-18 16:23:09.000000 iloscar_win-0.1.5/README.md
+drwxrwxrwx   0        0        0        0 2023-05-18 17:24:57.567992 iloscar_win-0.1.5/iloscar_win/
+-rw-rw-rw-   0        0        0      354 2023-05-18 17:23:33.000000 iloscar_win-0.1.5/iloscar_win/__init__.py
+-rw-rw-rw-   0        0        0     1955 2023-05-18 17:22:58.000000 iloscar_win-0.1.5/iloscar_win/app.py
+-rw-rw-rw-   0        0        0   106434 2023-05-18 17:23:19.000000 iloscar_win-0.1.5/iloscar_win/iLOSCAR_backend.py
+drwxrwxrwx   0        0        0        0 2023-05-18 17:24:57.634912 iloscar_win-0.1.5/iloscar_win/pages/
+-rw-rw-rw-   0        0        0     5801 2023-05-18 17:23:48.000000 iloscar_win-0.1.5/iloscar_win/pages/Function.py
+-rw-rw-rw-   0        0        0    26253 2023-05-18 17:23:44.000000 iloscar_win-0.1.5/iloscar_win/pages/forward.py
+-rw-rw-rw-   0        0        0      891 2023-05-18 17:23:53.000000 iloscar_win-0.1.5/iloscar_win/pages/home.py
+-rw-rw-rw-   0        0        0    46223 2023-05-18 17:24:04.000000 iloscar_win-0.1.5/iloscar_win/pages/inverse.py
+-rw-rw-rw-   0        0        0     1357 2023-05-18 16:23:10.000000 iloscar_win-0.1.5/iloscar_win/style.py
+drwxrwxrwx   0        0        0        0 2023-05-18 17:24:57.620919 iloscar_win-0.1.5/iloscar_win.egg-info/
+-rw-rw-rw-   0        0        0    18548 2023-05-18 17:24:57.000000 iloscar_win-0.1.5/iloscar_win.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      401 2023-05-18 17:24:57.000000 iloscar_win-0.1.5/iloscar_win.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-18 17:24:57.000000 iloscar_win-0.1.5/iloscar_win.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      131 2023-05-18 17:24:57.000000 iloscar_win-0.1.5/iloscar_win.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       30 2023-05-18 17:24:57.000000 iloscar_win-0.1.5/iloscar_win.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-18 17:24:57.647411 iloscar_win-0.1.5/setup.cfg
+-rw-rw-rw-   0        0        0     1509 2023-05-18 17:24:16.000000 iloscar_win-0.1.5/setup.py
```

### Comparing `iloscar_win-0.1.4/PKG-INFO` & `iloscar_win-0.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iloscar_win
-Version: 0.1.4
+Version: 0.1.5
 Summary: iLOSCAR_win
 Home-page: https://github.com/Shihan150/iloscar
 Author: Shihan Li
 Author-email: <shihan@tamu.edu>
 License: MIT
 Keywords: python,carbon cycle,model,paleoclimate,global warming,LOSCAR
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `iloscar_win-0.1.4/README.md` & `iloscar_win-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `iloscar_win-0.1.4/iloscar_win/app.py` & `iloscar_win-0.1.5/iloscar_win/app.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import dash
 from dash import html, dcc, DiskcacheManager, CeleryManager
 from dash_extensions.enrich import Output, DashProxy, Input, MultiplexerTransform
 import dash_bootstrap_components as dbc
-from iloscar.style import *
+from iloscar_win.style import *
 import diskcache
 
 cache = diskcache.Cache('./cache')
 
 def iloscar_run():
     external_stylesheets = [dbc.themes.SPACELAB]
     # [
```

### Comparing `iloscar_win-0.1.4/iloscar_win/iLOSCAR_backend.py` & `iloscar_win-0.1.5/iloscar_win/iLOSCAR_backend.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 import pandas as pd
 import numpy as np
 from numba import jit
 import sys
 
 import dash
 from dash import html, dcc
-from style import *
+from iloscar_win.style import *
 
 import timeit
 import plotly.graph_objects as go
 
 
 from scipy import interpolate
 from scipy.optimize import root_scalar, toms748
```

### Comparing `iloscar_win-0.1.4/iloscar_win/pages/Function.py` & `iloscar_win-0.1.5/iloscar_win/pages/Function.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 
 import dash
 from dash import Dash, dcc, html, Input, Output, callback, State
 import dash_bootstrap_components as dbc
 from dash.exceptions import PreventUpdate
 
-from iloscar.style import *
+from iloscar_win.style import *
 
 
 dash.register_page(__name__, order = 4)
 
 
 def make_fig(xdata, ydata , x_axis, y_axis):
     fig = make_subplots(rows=1, cols=1)
```

### Comparing `iloscar_win-0.1.4/iloscar_win/pages/forward.py` & `iloscar_win-0.1.5/iloscar_win/pages/forward.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,16 +6,16 @@
 import pandas as pd
 from dash.exceptions import PreventUpdate
 
 import plotly.express as px
 import plotly.graph_objects as go
 from plotly.subplots import make_subplots
 
-from iloscar.style import *
-from iloscar.iLOSCAR_backend import init_start, model_run, wo_results
+from iloscar_win.style import *
+from iloscar_win.iLOSCAR_backend import init_start, model_run, wo_results
 
 dash.register_page(__name__, order = 2)
 
 df_mode = pd.DataFrame(OrderedDict([
     ('Value', [0,1,1,1,0]),
     ('Parameter', ['PALEO', 'Sediment', 'LOADFLAG', 'Ocaen temperature change', 'Save ystart']),
     ('Options', [ '1/0', '1/0', '1/0', '1/0', '1/0']),
```

### Comparing `iloscar_win-0.1.4/iloscar_win/pages/home.py` & `iloscar_win-0.1.5/iloscar_win/pages/home.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import dash
 from dash import html, dcc
-from iloscar.style import *
+from iloscar_win.style import *
 
 dash.register_page(__name__, path='/', order = 1)
 
 link = "href='https://doi.org/10.5194/gmd-5-149-2012"
 layout = html.Div(children=[
     html.Div(style = Home_STYLE, children =[
     html.P("The LOSCAR model is designed to efficiently compute the partitioning of carbon between ocean, atmosphere, and sediments on time scales ranging from centuries to millions of years. "),
```

### Comparing `iloscar_win-0.1.4/iloscar_win/pages/inverse.py` & `iloscar_win-0.1.5/iloscar_win/pages/inverse.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,16 +7,16 @@
 import pprint
 from dash.exceptions import PreventUpdate
 
 import plotly.express as px
 import plotly.graph_objects as go
 from plotly.subplots import make_subplots
 
-from iloscar.style import *
-from iloscar.iLOSCAR_backend import init_start, model_run, wo_results
+from iloscar_win.style import *
+from iloscar_win.iLOSCAR_backend import init_start, model_run, wo_results
 
 dash.register_page(__name__, order = 3)
 
 # choose the target variables
 inv_opt = html.Div(
         children = [
         dbc.Row([
```

### Comparing `iloscar_win-0.1.4/iloscar_win/style.py` & `iloscar_win-0.1.5/iloscar_win/style.py`

 * *Files identical despite different names*

### Comparing `iloscar_win-0.1.4/iloscar_win.egg-info/PKG-INFO` & `iloscar_win-0.1.5/iloscar_win.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iloscar-win
-Version: 0.1.4
+Version: 0.1.5
 Summary: iLOSCAR_win
 Home-page: https://github.com/Shihan150/iloscar
 Author: Shihan Li
 Author-email: <shihan@tamu.edu>
 License: MIT
 Keywords: python,carbon cycle,model,paleoclimate,global warming,LOSCAR
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `iloscar_win-0.1.4/setup.py` & `iloscar_win-0.1.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '0.1.4'
+VERSION = '0.1.5'
 DESCRIPTION = 'iLOSCAR_win'
 LONG_DESCRIPTION = 'A web-based interactive carbon cycle model, built upon the classic LOSCAR model.'
 
 # Setting up
 setup(
     name="iloscar_win",
     version=VERSION,
```

