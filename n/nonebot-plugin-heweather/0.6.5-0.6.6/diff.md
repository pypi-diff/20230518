# Comparing `tmp/nonebot_plugin_heweather-0.6.5.tar.gz` & `tmp/nonebot_plugin_heweather-0.6.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_heweather-0.6.5.tar", max compression
+gzip compressed data, was "nonebot_plugin_heweather-0.6.6.tar", max compression
```

## Comparing `nonebot_plugin_heweather-0.6.5.tar` & `nonebot_plugin_heweather-0.6.6.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     1062 2023-05-12 04:24:13.645384 nonebot_plugin_heweather-0.6.5/LICENSE
--rw-r--r--   0        0        0     1455 2023-05-12 04:24:13.645384 nonebot_plugin_heweather-0.6.5/README.md
--rw-r--r--   0        0        0     1846 2023-05-12 04:24:13.645384 nonebot_plugin_heweather-0.6.5/nonebot_plugin_heweather/__init__.py
--rw-r--r--   0        0        0      223 2023-05-12 04:24:13.645384 nonebot_plugin_heweather-0.6.5/nonebot_plugin_heweather/config.py
--rw-r--r--   0        0        0     1094 2023-05-12 04:24:13.645384 nonebot_plugin_heweather-0.6.5/nonebot_plugin_heweather/model.py
--rw-r--r--   0        0        0     1785 2023-05-12 04:24:13.645384 nonebot_plugin_heweather-0.6.5/nonebot_plugin_heweather/render_pic.py
--rwxr-xr-x   0        0        0    69948 2023-05-12 04:24:13.645384 nonebot_plugin_heweather-0.6.5/nonebot_plugin_heweather/templates/css/fonts/qweather-icons.ttf
--rwxr-xr-x   0        0        0    27920 2023-05-12 04:24:13.645384 nonebot_plugin_heweather-0.6.5/nonebot_plugin_heweather/templates/css/fonts/qweather-icons.woff
--rwxr-xr-x   0        0        0    19688 2023-05-12 04:24:13.645384 nonebot_plugin_heweather-0.6.5/nonebot_plugin_heweather/templates/css/fonts/qweather-icons.woff2
--rwxr-xr-x   0        0        0    20240 2023-05-12 04:24:13.645384 nonebot_plugin_heweather-0.6.5/nonebot_plugin_heweather/templates/css/qweather-icons.css
--rwxr-xr-x   0        0        0     9784 2023-05-12 04:24:13.645384 nonebot_plugin_heweather-0.6.5/nonebot_plugin_heweather/templates/css/qweather-icons.json
--rw-r--r--   0        0        0     2850 2023-05-12 04:24:13.645384 nonebot_plugin_heweather-0.6.5/nonebot_plugin_heweather/templates/css/weather.css
--rw-r--r--   0        0        0     5219 2023-05-12 04:24:13.645384 nonebot_plugin_heweather-0.6.5/nonebot_plugin_heweather/templates/weather.html
--rw-r--r--   0        0        0     4915 2023-05-12 04:24:13.645384 nonebot_plugin_heweather-0.6.5/nonebot_plugin_heweather/weather_data.py
--rw-r--r--   0        0        0      839 2023-05-12 04:24:13.645384 nonebot_plugin_heweather-0.6.5/pyproject.toml
--rw-r--r--   0        0        0     2234 1970-01-01 00:00:00.000000 nonebot_plugin_heweather-0.6.5/PKG-INFO
+-rw-r--r--   0        0        0     1062 2023-05-18 13:53:48.324067 nonebot_plugin_heweather-0.6.6/LICENSE
+-rw-r--r--   0        0        0     1455 2023-05-18 13:53:48.324067 nonebot_plugin_heweather-0.6.6/README.md
+-rw-r--r--   0        0        0     1812 2023-05-18 13:53:48.324067 nonebot_plugin_heweather-0.6.6/nonebot_plugin_heweather/__init__.py
+-rw-r--r--   0        0        0      223 2023-05-18 13:53:48.324067 nonebot_plugin_heweather-0.6.6/nonebot_plugin_heweather/config.py
+-rw-r--r--   0        0        0     1104 2023-05-18 13:53:48.324067 nonebot_plugin_heweather-0.6.6/nonebot_plugin_heweather/model.py
+-rw-r--r--   0        0        0     1785 2023-05-18 13:53:48.324067 nonebot_plugin_heweather-0.6.6/nonebot_plugin_heweather/render_pic.py
+-rwxr-xr-x   0        0        0    69948 2023-05-18 13:53:48.328068 nonebot_plugin_heweather-0.6.6/nonebot_plugin_heweather/templates/css/fonts/qweather-icons.ttf
+-rwxr-xr-x   0        0        0    27920 2023-05-18 13:53:48.328068 nonebot_plugin_heweather-0.6.6/nonebot_plugin_heweather/templates/css/fonts/qweather-icons.woff
+-rwxr-xr-x   0        0        0    19688 2023-05-18 13:53:48.328068 nonebot_plugin_heweather-0.6.6/nonebot_plugin_heweather/templates/css/fonts/qweather-icons.woff2
+-rwxr-xr-x   0        0        0    20240 2023-05-18 13:53:48.328068 nonebot_plugin_heweather-0.6.6/nonebot_plugin_heweather/templates/css/qweather-icons.css
+-rwxr-xr-x   0        0        0     9784 2023-05-18 13:53:48.328068 nonebot_plugin_heweather-0.6.6/nonebot_plugin_heweather/templates/css/qweather-icons.json
+-rw-r--r--   0        0        0     2850 2023-05-18 13:53:48.328068 nonebot_plugin_heweather-0.6.6/nonebot_plugin_heweather/templates/css/weather.css
+-rw-r--r--   0        0        0     5219 2023-05-18 13:53:48.328068 nonebot_plugin_heweather-0.6.6/nonebot_plugin_heweather/templates/weather.html
+-rw-r--r--   0        0        0     4960 2023-05-18 13:53:48.328068 nonebot_plugin_heweather-0.6.6/nonebot_plugin_heweather/weather_data.py
+-rw-r--r--   0        0        0      839 2023-05-18 13:53:48.328068 nonebot_plugin_heweather-0.6.6/pyproject.toml
+-rw-r--r--   0        0        0     2234 1970-01-01 00:00:00.000000 nonebot_plugin_heweather-0.6.6/PKG-INFO
```

### Comparing `nonebot_plugin_heweather-0.6.5/LICENSE` & `nonebot_plugin_heweather-0.6.6/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_heweather-0.6.5/README.md` & `nonebot_plugin_heweather-0.6.6/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_heweather-0.6.5/nonebot_plugin_heweather/__init__.py` & `nonebot_plugin_heweather-0.6.6/nonebot_plugin_heweather/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -27,23 +27,22 @@
 
 weather = on_keyword({"天气"}, priority=1)
 
 
 @weather.handle()
 async def _(matcher: Matcher, event: MessageEvent):
     city = ""
-    if args := search(r".*?(.*)天气(.*).*?", event.get_plaintext()):  # type: ignore
+    if args := event.get_plaintext().split("天气"):
         city = args[0].strip() or args[1].strip()
         if not city:
             await weather.finish("地点是...空气吗?? >_<")
 
         # 判断指令前后是否都有内容，如果是则结束，否则跳过。
         if (args[0].strip() == "") == (args[1].strip() == ""):
             await weather.finish()
-
     w_data = Weather(city_name=city, api_key=api_key, api_type=api_type)
     try:
         await w_data.load_data()
     except CityNotFoundError:
         matcher.block = False
         await weather.finish()
```

### Comparing `nonebot_plugin_heweather-0.6.5/nonebot_plugin_heweather/model.py` & `nonebot_plugin_heweather-0.6.6/nonebot_plugin_heweather/model.py`

 * *Files 8% similar despite different names*

```diff
@@ -59,8 +59,8 @@
     type: str
     pubTime: str
     text: str
 
 
 class WarningApi(BaseModel, extra=Extra.allow):
     code: str
-    warning: List[Warning]
+    warning: Optional[List[Warning]]
```

### Comparing `nonebot_plugin_heweather-0.6.5/nonebot_plugin_heweather/render_pic.py` & `nonebot_plugin_heweather-0.6.6/nonebot_plugin_heweather/render_pic.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_heweather-0.6.5/nonebot_plugin_heweather/templates/css/fonts/qweather-icons.ttf` & `nonebot_plugin_heweather-0.6.6/nonebot_plugin_heweather/templates/css/fonts/qweather-icons.ttf`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_heweather-0.6.5/nonebot_plugin_heweather/templates/css/fonts/qweather-icons.woff` & `nonebot_plugin_heweather-0.6.6/nonebot_plugin_heweather/templates/css/fonts/qweather-icons.woff`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_heweather-0.6.5/nonebot_plugin_heweather/templates/css/fonts/qweather-icons.woff2` & `nonebot_plugin_heweather-0.6.6/nonebot_plugin_heweather/templates/css/fonts/qweather-icons.woff2`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_heweather-0.6.5/nonebot_plugin_heweather/templates/css/qweather-icons.css` & `nonebot_plugin_heweather-0.6.6/nonebot_plugin_heweather/templates/css/qweather-icons.css`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_heweather-0.6.5/nonebot_plugin_heweather/templates/css/qweather-icons.json` & `nonebot_plugin_heweather-0.6.6/nonebot_plugin_heweather/templates/css/qweather-icons.json`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_heweather-0.6.5/nonebot_plugin_heweather/templates/css/weather.css` & `nonebot_plugin_heweather-0.6.6/nonebot_plugin_heweather/templates/css/weather.css`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_heweather-0.6.5/nonebot_plugin_heweather/templates/weather.html` & `nonebot_plugin_heweather-0.6.6/nonebot_plugin_heweather/templates/weather.html`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_heweather-0.6.5/nonebot_plugin_heweather/weather_data.py` & `nonebot_plugin_heweather-0.6.6/nonebot_plugin_heweather/weather_data.py`

 * *Files 2% similar despite different names*

```diff
@@ -134,8 +134,8 @@
     @property
     async def _warning(self) -> WarningApi:
         res = await self._get_data(
             url=self.url_weather_warning,
             params={"location": self.city_id, "key": self.apikey},
         )
         self._check_response(res)
-        return WarningApi(**res.json())
+        return None if res.json().get("code") == "204" else WarningApi(**res.json())
```

### Comparing `nonebot_plugin_heweather-0.6.5/pyproject.toml` & `nonebot_plugin_heweather-0.6.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nonebot-plugin-heweather"
-version = "0.6.5"
+version = "0.6.6"
 description = "Get Heweather information and convert to pictures"
 authors = ["kexue <x@kexue.io>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.8,<4.0.0"
```

### Comparing `nonebot_plugin_heweather-0.6.5/PKG-INFO` & `nonebot_plugin_heweather-0.6.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-heweather
-Version: 0.6.5
+Version: 0.6.6
 Summary: Get Heweather information and convert to pictures
 License: MIT
 Author: kexue
 Author-email: x@kexue.io
 Requires-Python: >=3.8,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

