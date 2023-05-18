# Comparing `tmp/iloscar-win-0.1.0.tar.gz` & `tmp/iloscar-win-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iloscar-win-0.1.0.tar", last modified: Thu May 18 16:50:09 2023, max compression
+gzip compressed data, was "iloscar-win-0.1.1.tar", last modified: Thu May 18 17:02:15 2023, max compression
```

## Comparing `iloscar-win-0.1.0.tar` & `iloscar-win-0.1.1.tar`

### file list

```diff
@@ -1,20 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-05-18 16:50:09.715310 iloscar-win-0.1.0/
--rw-rw-rw-   0        0        0    18548 2023-05-18 16:50:09.713060 iloscar-win-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0    17783 2023-05-18 16:23:09.000000 iloscar-win-0.1.0/README.md
-drwxrwxrwx   0        0        0        0 2023-05-18 16:50:09.646652 iloscar-win-0.1.0/iloscar/
--rw-rw-rw-   0        0        0        0 2023-05-18 16:23:09.000000 iloscar-win-0.1.0/iloscar/__init__.py
--rw-rw-rw-   0        0        0     1752 2023-05-18 16:23:09.000000 iloscar-win-0.1.0/iloscar/app.py
--rw-rw-rw-   0        0        0   106422 2023-05-18 16:23:10.000000 iloscar-win-0.1.0/iloscar/iLOSCAR_backend.py
-drwxrwxrwx   0        0        0        0 2023-05-18 16:50:09.668769 iloscar-win-0.1.0/iloscar/pages/
--rw-rw-rw-   0        0        0     5789 2023-05-18 16:23:10.000000 iloscar-win-0.1.0/iloscar/pages/Function.py
--rw-rw-rw-   0        0        0    26229 2023-05-18 16:23:10.000000 iloscar-win-0.1.0/iloscar/pages/forward.py
--rw-rw-rw-   0        0        0      879 2023-05-18 16:23:10.000000 iloscar-win-0.1.0/iloscar/pages/home.py
--rw-rw-rw-   0        0        0    46199 2023-05-18 16:23:10.000000 iloscar-win-0.1.0/iloscar/pages/inverse.py
-drwxrwxrwx   0        0        0        0 2023-05-18 16:50:09.708939 iloscar-win-0.1.0/iloscar_win.egg-info/
--rw-rw-rw-   0        0        0    18548 2023-05-18 16:50:09.000000 iloscar-win-0.1.0/iloscar_win.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      352 2023-05-18 16:50:09.000000 iloscar-win-0.1.0/iloscar_win.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-18 16:50:09.000000 iloscar-win-0.1.0/iloscar_win.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      131 2023-05-18 16:50:09.000000 iloscar-win-0.1.0/iloscar_win.egg-info/requires.txt
--rw-rw-rw-   0        0        0       22 2023-05-18 16:50:09.000000 iloscar-win-0.1.0/iloscar_win.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-18 16:50:09.716476 iloscar-win-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0     1501 2023-05-18 16:48:47.000000 iloscar-win-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-18 17:02:15.407099 iloscar-win-0.1.1/
+-rw-rw-rw-   0        0        0    18548 2023-05-18 17:02:15.404554 iloscar-win-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0    17783 2023-05-18 16:23:09.000000 iloscar-win-0.1.1/README.md
+drwxrwxrwx   0        0        0        0 2023-05-18 17:02:15.346659 iloscar-win-0.1.1/iloscar/
+-rw-rw-rw-   0        0        0      349 2023-05-18 16:58:34.000000 iloscar-win-0.1.1/iloscar/__init__.py
+-rw-rw-rw-   0        0        0     1951 2023-05-18 17:00:12.000000 iloscar-win-0.1.1/iloscar/app.py
+-rw-rw-rw-   0        0        0   106422 2023-05-18 16:23:10.000000 iloscar-win-0.1.1/iloscar/iLOSCAR_backend.py
+drwxrwxrwx   0        0        0        0 2023-05-18 17:02:15.354953 iloscar-win-0.1.1/iloscar/pages/
+-rw-rw-rw-   0        0        0     5797 2023-05-18 17:01:06.000000 iloscar-win-0.1.1/iloscar/pages/Function.py
+-rw-rw-rw-   0        0        0    26245 2023-05-18 17:00:56.000000 iloscar-win-0.1.1/iloscar/pages/forward.py
+-rw-rw-rw-   0        0        0      887 2023-05-18 17:01:55.000000 iloscar-win-0.1.1/iloscar/pages/home.py
+-rw-rw-rw-   0        0        0    46215 2023-05-18 17:01:22.000000 iloscar-win-0.1.1/iloscar/pages/inverse.py
+-rw-rw-rw-   0        0        0     1357 2023-05-18 16:23:10.000000 iloscar-win-0.1.1/iloscar/style.py
+drwxrwxrwx   0        0        0        0 2023-05-18 17:02:15.399333 iloscar-win-0.1.1/iloscar_win.egg-info/
+-rw-rw-rw-   0        0        0    18548 2023-05-18 17:02:15.000000 iloscar-win-0.1.1/iloscar_win.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      369 2023-05-18 17:02:15.000000 iloscar-win-0.1.1/iloscar_win.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-18 17:02:15.000000 iloscar-win-0.1.1/iloscar_win.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      131 2023-05-18 17:02:15.000000 iloscar-win-0.1.1/iloscar_win.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       22 2023-05-18 17:02:15.000000 iloscar-win-0.1.1/iloscar_win.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-18 17:02:15.407099 iloscar-win-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0     1501 2023-05-18 17:01:51.000000 iloscar-win-0.1.1/setup.py
```

### Comparing `iloscar-win-0.1.0/PKG-INFO` & `iloscar-win-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iloscar-win
-Version: 0.1.0
+Version: 0.1.1
 Summary: iLOSCAR-win
 Home-page: https://github.com/Shihan150/iloscar
 Author: Shihan Li
 Author-email: <shihan@tamu.edu>
 License: MIT
 Keywords: python,carbon cycle,model,paleoclimate,global warming,LOSCAR
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `iloscar-win-0.1.0/README.md` & `iloscar-win-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `iloscar-win-0.1.0/iloscar/app.py` & `iloscar-win-0.1.1/iloscar/app.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,67 +1,69 @@
 import dash
 from dash import html, dcc, DiskcacheManager, CeleryManager
 from dash_extensions.enrich import Output, DashProxy, Input, MultiplexerTransform
 import dash_bootstrap_components as dbc
-from style import *
+from iloscar.style import *
 import diskcache
 
 cache = diskcache.Cache('./cache')
 
-external_stylesheets = [dbc.themes.SPACELAB]
-# [
-#     {
-#         "href": (
-#             "https://fonts.googleapis.com/css2?"
-#             "family=Lato:wght@400;700&display=swap"
-#         ),
-#         "rel": "stylesheet",
-#     },]
-# [dbc.themes.SPACELAB]
-app = DashProxy(__name__, use_pages=True, external_stylesheets=external_stylesheets,
-    background_callback_manager = DiskcacheManager(cache),
-    transforms=[MultiplexerTransform()]
+def iloscar_run():
+    external_stylesheets = [dbc.themes.SPACELAB]
+    # [
+    #     {
+    #         "href": (
+    #             "https://fonts.googleapis.com/css2?"
+    #             "family=Lato:wght@400;700&display=swap"
+    #         ),
+    #         "rel": "stylesheet",
+    #     },]
+    # [dbc.themes.SPACELAB]
+    app = DashProxy(__name__, use_pages=True, external_stylesheets=external_stylesheets,
+        background_callback_manager = DiskcacheManager(cache),
+        transforms=[MultiplexerTransform()]
+        )
+    sidebar = dbc.Nav(
+                [
+                    dbc.NavLink(
+                        [
+                            html.Div(page["name"], className="ms-2"),
+                        ],
+                        href=page["path"],
+                        active="exact",
+                    )
+                    for page in dash.page_registry.values()
+                ],
+                vertical=True,
+                pills=True,
+                className="bg-light",
+                style = {'fontSize': 20}
     )
-sidebar = dbc.Nav(
+
+
+    app.layout = dbc.Container([
+        dbc.Row([
+            dbc.Col(html.Div("Welcom to iLOSCAR",
+                             style={'fontSize':50, 'textAlign':'center'}))
+        ]),
+
+        html.Hr(),
+
+        dbc.Row(
             [
-                dbc.NavLink(
+                dbc.Col(
                     [
-                        html.Div(page["name"], className="ms-2"),
-                    ],
-                    href=page["path"],
-                    active="exact",
-                )
-                for page in dash.page_registry.values()
-            ],
-            vertical=True,
-            pills=True,
-            className="bg-light",
-            style = {'fontSize': 20}
-)
-
-
-app.layout = dbc.Container([
-    dbc.Row([
-        dbc.Col(html.Div("Welcom to iLOSCAR",
-                         style={'fontSize':50, 'textAlign':'center'}))
-    ]),
-
-    html.Hr(),
-
-    dbc.Row(
-        [
-            dbc.Col(
-                [
-                    sidebar
-                ], xs=4, sm=4, md=2, lg=2, xl=2, xxl=2),
+                        sidebar
+                    ], xs=4, sm=4, md=2, lg=2, xl=2, xxl=2),
+
+                dbc.Col(
+                    [
+                        dash.page_container
+                    ], xs=8, sm=8, md=10, lg=10, xl=10, xxl=10)
+            ]
+        )
+    ], fluid=True)
+
 
-            dbc.Col(
-                [
-                    dash.page_container
-                ], xs=8, sm=8, md=10, lg=10, xl=10, xxl=10)
-        ]
-    )
-], fluid=True)
 
 
-if __name__ == "__main__":
-    app.run(debug=True, port = '7777')
+    app.run(debug=False, port = '7777')
```

### Comparing `iloscar-win-0.1.0/iloscar/iLOSCAR_backend.py` & `iloscar-win-0.1.1/iloscar/iLOSCAR_backend.py`

 * *Files identical despite different names*

### Comparing `iloscar-win-0.1.0/iloscar/pages/Function.py` & `iloscar-win-0.1.1/iloscar/pages/Function.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 
 import dash
 from dash import Dash, dcc, html, Input, Output, callback, State
 import dash_bootstrap_components as dbc
 from dash.exceptions import PreventUpdate
 
-from style import *
+from iloscar.style import *
 
 
 dash.register_page(__name__, order = 4)
 
 
 def make_fig(xdata, ydata , x_axis, y_axis):
     fig = make_subplots(rows=1, cols=1)
```

### Comparing `iloscar-win-0.1.0/iloscar/pages/forward.py` & `iloscar-win-0.1.1/iloscar/pages/forward.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,16 +6,16 @@
 import pandas as pd
 from dash.exceptions import PreventUpdate
 
 import plotly.express as px
 import plotly.graph_objects as go
 from plotly.subplots import make_subplots
 
-from style import *
-from iLOSCAR_backend import init_start, model_run, wo_results
+from iloscar.style import *
+from iloscar.iLOSCAR_backend import init_start, model_run, wo_results
 
 dash.register_page(__name__, order = 2)
 
 df_mode = pd.DataFrame(OrderedDict([
     ('Value', [0,1,1,1,0]),
     ('Parameter', ['PALEO', 'Sediment', 'LOADFLAG', 'Ocaen temperature change', 'Save ystart']),
     ('Options', [ '1/0', '1/0', '1/0', '1/0', '1/0']),
```

### Comparing `iloscar-win-0.1.0/iloscar/pages/home.py` & `iloscar-win-0.1.1/iloscar/pages/home.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import dash
 from dash import html, dcc
-from style import *
+from iloscar.style import *
 
 dash.register_page(__name__, path='/', order = 1)
 
 link = "href='https://doi.org/10.5194/gmd-5-149-2012"
 layout = html.Div(children=[
     html.Div(style = Home_STYLE, children =[
     html.P("The LOSCAR model is designed to efficiently compute the partitioning of carbon between ocean, atmosphere, and sediments on time scales ranging from centuries to millions of years. "),
```

### Comparing `iloscar-win-0.1.0/iloscar/pages/inverse.py` & `iloscar-win-0.1.1/iloscar/pages/inverse.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,16 +7,16 @@
 import pprint
 from dash.exceptions import PreventUpdate
 
 import plotly.express as px
 import plotly.graph_objects as go
 from plotly.subplots import make_subplots
 
-from style import *
-from iLOSCAR_backend import init_start, model_run, wo_results
+from iloscar.style import *
+from iloscar.iLOSCAR_backend import init_start, model_run, wo_results
 
 dash.register_page(__name__, order = 3)
 
 # choose the target variables
 inv_opt = html.Div(
         children = [
         dbc.Row([
```

### Comparing `iloscar-win-0.1.0/iloscar_win.egg-info/PKG-INFO` & `iloscar-win-0.1.1/iloscar_win.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iloscar-win
-Version: 0.1.0
+Version: 0.1.1
 Summary: iLOSCAR-win
 Home-page: https://github.com/Shihan150/iloscar
 Author: Shihan Li
 Author-email: <shihan@tamu.edu>
 License: MIT
 Keywords: python,carbon cycle,model,paleoclimate,global warming,LOSCAR
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `iloscar-win-0.1.0/setup.py` & `iloscar-win-0.1.1/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '0.1.0'
+VERSION = '0.1.1'
 DESCRIPTION = 'iLOSCAR-win'
 LONG_DESCRIPTION = 'A web-based interactive carbon cycle model, built upon the classic LOSCAR model.'
 
 # Setting up
 setup(
     name="iloscar-win",
     version=VERSION,
```

