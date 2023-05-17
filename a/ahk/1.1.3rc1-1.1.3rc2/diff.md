# Comparing `tmp/ahk-1.1.3rc1.tar.gz` & `tmp/ahk-1.1.3rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ahk-1.1.3rc1.tar", last modified: Wed May 17 00:35:27 2023, max compression
+gzip compressed data, was "ahk-1.1.3rc2.tar", last modified: Wed May 17 19:28:58 2023, max compression
```

## Comparing `ahk-1.1.3rc1.tar` & `ahk-1.1.3rc2.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 00:35:27.772985 ahk-1.1.3rc1/
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-05-17 00:35:11.000000 ahk-1.1.3rc1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    18814 2023-05-17 00:35:27.776985 ahk-1.1.3rc1/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 00:35:27.768985 ahk-1.1.3rc1/ahk/
--rw-r--r--   0 runner    (1001) docker     (123)      956 2023-05-17 00:35:11.000000 ahk-1.1.3rc1/ahk/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 00:35:27.772985 ahk-1.1.3rc1/ahk/_async/
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-05-17 00:35:11.000000 ahk-1.1.3rc1/ahk/_async/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   179999 2023-05-17 00:35:11.000000 ahk-1.1.3rc1/ahk/_async/engine.py
--rw-r--r--   0 runner    (1001) docker     (123)    43479 2023-05-17 00:35:11.000000 ahk-1.1.3rc1/ahk/_async/transport.py
--rw-r--r--   0 runner    (1001) docker     (123)    29128 2023-05-17 00:35:11.000000 ahk-1.1.3rc1/ahk/_async/window.py
--rw-r--r--   0 runner    (1001) docker     (123)    83686 2023-05-17 00:35:11.000000 ahk-1.1.3rc1/ahk/_constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    13992 2023-05-17 00:35:11.000000 ahk-1.1.3rc1/ahk/_hotkey.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 00:35:27.772985 ahk-1.1.3rc1/ahk/_sync/
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-05-17 00:35:11.000000 ahk-1.1.3rc1/ahk/_sync/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   174245 2023-05-17 00:35:11.000000 ahk-1.1.3rc1/ahk/_sync/engine.py
--rw-r--r--   0 runner    (1001) docker     (123)    39283 2023-05-17 00:35:11.000000 ahk-1.1.3rc1/ahk/_sync/transport.py
--rw-r--r--   0 runner    (1001) docker     (123)    26344 2023-05-17 00:35:11.000000 ahk-1.1.3rc1/ahk/_sync/window.py
--rw-r--r--   0 runner    (1001) docker     (123)      650 2023-05-17 00:35:11.000000 ahk-1.1.3rc1/ahk/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3496 2023-05-17 00:35:11.000000 ahk-1.1.3rc1/ahk/directives.py
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-05-17 00:35:11.000000 ahk-1.1.3rc1/ahk/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     7506 2023-05-17 00:35:11.000000 ahk-1.1.3rc1/ahk/keys.py
--rw-r--r--   0 runner    (1001) docker     (123)    11435 2023-05-17 00:35:11.000000 ahk-1.1.3rc1/ahk/message.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 00:35:11.000000 ahk-1.1.3rc1/ahk/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 00:35:27.772985 ahk-1.1.3rc1/ahk/templates/
--rw-r--r--   0 runner    (1001) docker     (123)    79035 2023-05-17 00:35:11.000000 ahk-1.1.3rc1/ahk/templates/daemon.ahk
--rw-r--r--   0 runner    (1001) docker     (123)     4508 2023-05-17 00:35:11.000000 ahk-1.1.3rc1/ahk/templates/hotkeys.ahk
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 00:35:27.772985 ahk-1.1.3rc1/ahk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    18814 2023-05-17 00:35:27.000000 ahk-1.1.3rc1/ahk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      574 2023-05-17 00:35:27.000000 ahk-1.1.3rc1/ahk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 00:35:27.000000 ahk-1.1.3rc1/ahk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-05-17 00:35:27.000000 ahk-1.1.3rc1/ahk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-17 00:35:27.000000 ahk-1.1.3rc1/ahk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      875 2023-05-17 00:35:11.000000 ahk-1.1.3rc1/buildunasync.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 00:35:27.772985 ahk-1.1.3rc1/docs/
--rw-r--r--   0 runner    (1001) docker     (123)    17928 2023-05-17 00:35:11.000000 ahk-1.1.3rc1/docs/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-05-17 00:35:11.000000 ahk-1.1.3rc1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1199 2023-05-17 00:35:27.776985 ahk-1.1.3rc1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-17 00:35:11.000000 ahk-1.1.3rc1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 19:28:58.251110 ahk-1.1.3rc2/
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-05-17 19:28:43.000000 ahk-1.1.3rc2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    18814 2023-05-17 19:28:58.251110 ahk-1.1.3rc2/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 19:28:58.247110 ahk-1.1.3rc2/ahk/
+-rw-r--r--   0 runner    (1001) docker     (123)      956 2023-05-17 19:28:43.000000 ahk-1.1.3rc2/ahk/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 19:28:58.247110 ahk-1.1.3rc2/ahk/_async/
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-05-17 19:28:43.000000 ahk-1.1.3rc2/ahk/_async/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   179999 2023-05-17 19:28:43.000000 ahk-1.1.3rc2/ahk/_async/engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43479 2023-05-17 19:28:43.000000 ahk-1.1.3rc2/ahk/_async/transport.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29128 2023-05-17 19:28:43.000000 ahk-1.1.3rc2/ahk/_async/window.py
+-rw-r--r--   0 runner    (1001) docker     (123)    83686 2023-05-17 19:28:43.000000 ahk-1.1.3rc2/ahk/_constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14354 2023-05-17 19:28:43.000000 ahk-1.1.3rc2/ahk/_hotkey.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 19:28:58.247110 ahk-1.1.3rc2/ahk/_sync/
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-05-17 19:28:43.000000 ahk-1.1.3rc2/ahk/_sync/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   174245 2023-05-17 19:28:43.000000 ahk-1.1.3rc2/ahk/_sync/engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39283 2023-05-17 19:28:43.000000 ahk-1.1.3rc2/ahk/_sync/transport.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26344 2023-05-17 19:28:43.000000 ahk-1.1.3rc2/ahk/_sync/window.py
+-rw-r--r--   0 runner    (1001) docker     (123)      650 2023-05-17 19:28:43.000000 ahk-1.1.3rc2/ahk/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3496 2023-05-17 19:28:43.000000 ahk-1.1.3rc2/ahk/directives.py
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-05-17 19:28:43.000000 ahk-1.1.3rc2/ahk/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7506 2023-05-17 19:28:43.000000 ahk-1.1.3rc2/ahk/keys.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11435 2023-05-17 19:28:43.000000 ahk-1.1.3rc2/ahk/message.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 19:28:43.000000 ahk-1.1.3rc2/ahk/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 19:28:58.247110 ahk-1.1.3rc2/ahk/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)    79035 2023-05-17 19:28:43.000000 ahk-1.1.3rc2/ahk/templates/daemon.ahk
+-rw-r--r--   0 runner    (1001) docker     (123)     4508 2023-05-17 19:28:43.000000 ahk-1.1.3rc2/ahk/templates/hotkeys.ahk
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 19:28:58.247110 ahk-1.1.3rc2/ahk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    18814 2023-05-17 19:28:58.000000 ahk-1.1.3rc2/ahk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      574 2023-05-17 19:28:58.000000 ahk-1.1.3rc2/ahk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 19:28:58.000000 ahk-1.1.3rc2/ahk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-05-17 19:28:58.000000 ahk-1.1.3rc2/ahk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-17 19:28:58.000000 ahk-1.1.3rc2/ahk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      875 2023-05-17 19:28:43.000000 ahk-1.1.3rc2/buildunasync.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 19:28:58.251110 ahk-1.1.3rc2/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)    17928 2023-05-17 19:28:43.000000 ahk-1.1.3rc2/docs/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-05-17 19:28:43.000000 ahk-1.1.3rc2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1199 2023-05-17 19:28:58.251110 ahk-1.1.3rc2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-17 19:28:43.000000 ahk-1.1.3rc2/setup.py
```

### Comparing `ahk-1.1.3rc1/PKG-INFO` & `ahk-1.1.3rc2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ahk
-Version: 1.1.3rc1
+Version: 1.1.3rc2
 Summary: A Python wrapper for AHK
 Home-page: https://github.com/spyoungtech/ahk
 Author: Spencer Young
 Author-email: spencer.young@spyoung.com
 Keywords: ahk,autohotkey,windows,mouse,keyboard,automation,pyautogui
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Desktop Environment
```

### Comparing `ahk-1.1.3rc1/ahk/__init__.py` & `ahk-1.1.3rc2/ahk/__init__.py`

 * *Files identical despite different names*

### Comparing `ahk-1.1.3rc1/ahk/_async/engine.py` & `ahk-1.1.3rc2/ahk/_async/engine.py`

 * *Files identical despite different names*

### Comparing `ahk-1.1.3rc1/ahk/_async/transport.py` & `ahk-1.1.3rc2/ahk/_async/transport.py`

 * *Files identical despite different names*

### Comparing `ahk-1.1.3rc1/ahk/_async/window.py` & `ahk-1.1.3rc2/ahk/_async/window.py`

 * *Files identical despite different names*

### Comparing `ahk-1.1.3rc1/ahk/_constants.py` & `ahk-1.1.3rc2/ahk/_constants.py`

 * *Files identical despite different names*

### Comparing `ahk-1.1.3rc1/ahk/_hotkey.py` & `ahk-1.1.3rc2/ahk/_hotkey.py`

 * *Files 4% similar despite different names*

```diff
@@ -120,17 +120,25 @@
     def __init__(self, executable_path: str, default_ex_handler: Optional[Callable[[str, Exception], Any]] = None):
         super().__init__(executable_path=executable_path, default_ex_handler=default_ex_handler)
         self._callback_threads: List[threading.Thread] = []
         self._proc: Optional[subprocess.Popen[bytes]] = None
         self._callback_queue: Queue[Union[str, Type[STOP]]] = Queue()
         self._listener_thread: Optional[threading.Thread] = None
         self._dispatcher_thread: Optional[threading.Thread] = None
-        self._jinja_env: jinja2.Environment = jinja2.Environment(
-            loader=jinja2.PackageLoader('ahk', 'templates'), autoescape=False
-        )
+        loader: jinja2.BaseLoader
+        try:
+            loader = jinja2.PackageLoader('ahk', 'templates')
+        except ValueError:
+            # see: https://github.com/spyoungtech/ahk/issues/201
+            warnings.warn(
+                'Jinja could not find templates with PackageLoader. Falling back to BaseLoader',
+                category=UserWarning,
+            )
+            loader = jinja2.BaseLoader()
+        self._jinja_env: jinja2.Environment = jinja2.Environment(loader=loader, autoescape=False)
         self._template: jinja2.Template
         try:
             self._template = self._jinja_env.get_template('hotkeys.ahk')
         except jinja2.TemplateNotFound:
             warnings.warn('hotkey template not found, falling back to constant', category=UserWarning)
             self._template = self._jinja_env.from_string(_HOTKEY_SCRIPT)
```

### Comparing `ahk-1.1.3rc1/ahk/_sync/engine.py` & `ahk-1.1.3rc2/ahk/_sync/engine.py`

 * *Files identical despite different names*

### Comparing `ahk-1.1.3rc1/ahk/_sync/transport.py` & `ahk-1.1.3rc2/ahk/_sync/transport.py`

 * *Files identical despite different names*

### Comparing `ahk-1.1.3rc1/ahk/_sync/window.py` & `ahk-1.1.3rc2/ahk/_sync/window.py`

 * *Files identical despite different names*

### Comparing `ahk-1.1.3rc1/ahk/_utils.py` & `ahk-1.1.3rc2/ahk/_utils.py`

 * *Files identical despite different names*

### Comparing `ahk-1.1.3rc1/ahk/directives.py` & `ahk-1.1.3rc2/ahk/directives.py`

 * *Files identical despite different names*

### Comparing `ahk-1.1.3rc1/ahk/keys.py` & `ahk-1.1.3rc2/ahk/keys.py`

 * *Files identical despite different names*

### Comparing `ahk-1.1.3rc1/ahk/message.py` & `ahk-1.1.3rc2/ahk/message.py`

 * *Files identical despite different names*

### Comparing `ahk-1.1.3rc1/ahk/templates/daemon.ahk` & `ahk-1.1.3rc2/ahk/templates/daemon.ahk`

 * *Files identical despite different names*

### Comparing `ahk-1.1.3rc1/ahk/templates/hotkeys.ahk` & `ahk-1.1.3rc2/ahk/templates/hotkeys.ahk`

 * *Files identical despite different names*

### Comparing `ahk-1.1.3rc1/ahk.egg-info/PKG-INFO` & `ahk-1.1.3rc2/ahk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ahk
-Version: 1.1.3rc1
+Version: 1.1.3rc2
 Summary: A Python wrapper for AHK
 Home-page: https://github.com/spyoungtech/ahk
 Author: Spencer Young
 Author-email: spencer.young@spyoung.com
 Keywords: ahk,autohotkey,windows,mouse,keyboard,automation,pyautogui
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Desktop Environment
```

### Comparing `ahk-1.1.3rc1/ahk.egg-info/SOURCES.txt` & `ahk-1.1.3rc2/ahk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ahk-1.1.3rc1/buildunasync.py` & `ahk-1.1.3rc2/buildunasync.py`

 * *Files identical despite different names*

### Comparing `ahk-1.1.3rc1/docs/README.md` & `ahk-1.1.3rc2/docs/README.md`

 * *Files identical despite different names*

### Comparing `ahk-1.1.3rc1/setup.cfg` & `ahk-1.1.3rc2/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = ahk
-version = 1.1.3rc1
+version = 1.1.3rc2
 author_email = spencer.young@spyoung.com
 author = Spencer Young
 description = A Python wrapper for AHK
 long_description = file: docs/README.md
 long_description_content_type = text/markdown
 url = https://github.com/spyoungtech/ahk
 keywords =
```

