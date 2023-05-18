# Comparing `tmp/js_code-0.0.2.tar.gz` & `tmp/js_code-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "js_code-0.0.2.tar", last modified: Thu May 18 01:00:36 2023, max compression
+gzip compressed data, was "js_code-0.1.0.tar", last modified: Thu May 18 01:42:46 2023, max compression
```

## Comparing `js_code-0.0.2.tar` & `js_code-0.1.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-05-18 01:00:36.656254 js_code-0.0.2/
--rw-rw-rw-   0        0        0     1094 2023-04-12 08:29:30.000000 js_code-0.0.2/LICENSE
--rw-rw-rw-   0        0        0      328 2023-05-18 01:00:36.656254 js_code-0.0.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-18 01:00:36.636310 js_code-0.0.2/js_code/
--rw-rw-rw-   0        0        0        0 2023-04-12 06:50:12.000000 js_code-0.0.2/js_code/__init__.py
--rw-rw-rw-   0        0        0     1032 2023-05-18 00:57:15.000000 js_code-0.0.2/js_code/js_open.py
-drwxrwxrwx   0        0        0        0 2023-05-18 01:00:36.655262 js_code-0.0.2/js_code.egg-info/
--rw-rw-rw-   0        0        0      328 2023-05-18 01:00:36.000000 js_code-0.0.2/js_code.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      209 2023-05-18 01:00:36.000000 js_code-0.0.2/js_code.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-18 01:00:36.000000 js_code-0.0.2/js_code.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-05-18 01:00:36.000000 js_code-0.0.2/js_code.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-05-18 01:00:36.000000 js_code-0.0.2/js_code.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-18 01:00:36.656254 js_code-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0      488 2023-05-18 00:57:15.000000 js_code-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-18 01:42:46.244468 js_code-0.1.0/
+-rw-rw-rw-   0        0        0     1094 2023-04-12 08:29:30.000000 js_code-0.1.0/LICENSE
+-rw-rw-rw-   0        0        0      330 2023-05-18 01:42:46.244468 js_code-0.1.0/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-18 01:42:46.227514 js_code-0.1.0/js_code/
+-rw-rw-rw-   0        0        0        0 2023-04-12 06:50:12.000000 js_code-0.1.0/js_code/__init__.py
+-rw-rw-rw-   0        0        0     1107 2023-05-18 01:33:41.000000 js_code-0.1.0/js_code/js_open.py
+drwxrwxrwx   0        0        0        0 2023-05-18 01:42:46.243474 js_code-0.1.0/js_code.egg-info/
+-rw-rw-rw-   0        0        0      330 2023-05-18 01:42:46.000000 js_code-0.1.0/js_code.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      209 2023-05-18 01:42:46.000000 js_code-0.1.0/js_code.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-18 01:42:46.000000 js_code-0.1.0/js_code.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-05-18 01:42:46.000000 js_code-0.1.0/js_code.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-05-18 01:42:46.000000 js_code-0.1.0/js_code.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-18 01:42:46.244468 js_code-0.1.0/setup.cfg
+-rw-rw-rw-   0        0        0      490 2023-05-18 01:42:19.000000 js_code-0.1.0/setup.py
```

### Comparing `js_code-0.0.2/LICENSE` & `js_code-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `js_code-0.0.2/js_code/js_open.py` & `js_code-0.1.0/js_code/js_open.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,10 +20,13 @@
             if code:
                 js_code = code + f.read()
             else:
                 js_code = f.read()
             # 加载 javascript 代码
         js = execjs.compile(js_code)
     except:
-        # 做一个适配同时兼容 javascript 代码 不用读出javascript代码文件
-        js = execjs.compile(file)
+        try:
+            # 做一个适配同时兼容 javascript 代码 不用读出javascript代码文件
+            js = execjs.compile(file)
+        except:
+            js = execjs.eval(file)
     return js
```

