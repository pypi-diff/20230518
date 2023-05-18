# Comparing `tmp/fenjing-0.3.2.tar.gz` & `tmp/fenjing-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fenjing-0.3.2.tar", last modified: Thu May 18 06:14:58 2023, max compression
+gzip compressed data, was "fenjing-0.3.3.tar", last modified: Thu May 18 07:35:00 2023, max compression
```

## Comparing `fenjing-0.3.2.tar` & `fenjing-0.3.3.tar`

### file list

```diff
@@ -1,37 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 06:14:58.441087 fenjing-0.3.2/
--rw-r--r--   0 runner    (1001) docker     (123)    16725 2023-05-18 06:14:39.000000 fenjing-0.3.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-05-18 06:14:39.000000 fenjing-0.3.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6255 2023-05-18 06:14:58.441087 fenjing-0.3.2/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (123)     5817 2023-05-18 06:14:39.000000 fenjing-0.3.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-18 06:14:39.000000 fenjing-0.3.2/VERSION
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 06:14:58.437087 fenjing-0.3.2/fenjing/
--rwxr-xr-x   0 runner    (1001) docker     (123)      202 2023-05-18 06:14:39.000000 fenjing-0.3.2/fenjing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-18 06:14:39.000000 fenjing-0.3.2/fenjing/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6389 2023-05-18 06:14:39.000000 fenjing-0.3.2/fenjing/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      800 2023-05-18 06:14:39.000000 fenjing-0.3.2/fenjing/colorize.py
--rw-r--r--   0 runner    (1001) docker     (123)      838 2023-05-18 06:14:39.000000 fenjing-0.3.2/fenjing/config_payload.py
--rw-r--r--   0 runner    (1001) docker     (123)     1486 2023-05-18 06:14:39.000000 fenjing-0.3.2/fenjing/const.py
--rwxr-xr-x   0 runner    (1001) docker     (123)       37 2023-05-18 06:14:39.000000 fenjing-0.3.2/fenjing/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2670 2023-05-18 06:14:39.000000 fenjing-0.3.2/fenjing/form.py
--rw-r--r--   0 runner    (1001) docker     (123)     5450 2023-05-18 06:14:39.000000 fenjing-0.3.2/fenjing/form_cracker.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3992 2023-05-18 06:14:39.000000 fenjing-0.3.2/fenjing/full_payload_gen.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2846 2023-05-18 06:14:39.000000 fenjing-0.3.2/fenjing/int_vars.py
--rw-r--r--   0 runner    (1001) docker     (123)    27358 2023-05-18 06:14:39.000000 fenjing-0.3.2/fenjing/payload_gen.py
--rw-r--r--   0 runner    (1001) docker     (123)     1549 2023-05-18 06:14:39.000000 fenjing-0.3.2/fenjing/requester.py
--rw-r--r--   0 runner    (1001) docker     (123)     1180 2023-05-18 06:14:39.000000 fenjing-0.3.2/fenjing/scan_url.py
--rw-r--r--   0 runner    (1001) docker     (123)      941 2023-05-18 06:14:39.000000 fenjing-0.3.2/fenjing/shell_payload.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 06:14:58.441087 fenjing-0.3.2/fenjing/static/
--rw-r--r--   0 runner    (1001) docker     (123)      639 2023-05-18 06:14:39.000000 fenjing-0.3.2/fenjing/static/style.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 06:14:58.441087 fenjing-0.3.2/fenjing/templates/
--rw-r--r--   0 runner    (1001) docker     (123)     6139 2023-05-18 06:14:39.000000 fenjing-0.3.2/fenjing/templates/index.html
--rw-r--r--   0 runner    (1001) docker     (123)     3192 2023-05-18 06:14:39.000000 fenjing-0.3.2/fenjing/waf_func_gen.py
--rw-r--r--   0 runner    (1001) docker     (123)     8580 2023-05-18 06:14:39.000000 fenjing-0.3.2/fenjing/webui.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 06:14:58.441087 fenjing-0.3.2/fenjing.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6255 2023-05-18 06:14:58.000000 fenjing-0.3.2/fenjing.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      629 2023-05-18 06:14:58.000000 fenjing-0.3.2/fenjing.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 06:14:58.000000 fenjing-0.3.2/fenjing.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-18 06:14:58.000000 fenjing-0.3.2/fenjing.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-18 06:14:58.000000 fenjing-0.3.2/fenjing.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-18 06:14:39.000000 fenjing-0.3.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-18 06:14:58.441087 fenjing-0.3.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      945 2023-05-18 06:14:39.000000 fenjing-0.3.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 07:35:00.353333 fenjing-0.3.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    16725 2023-05-18 07:34:43.000000 fenjing-0.3.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-05-18 07:34:43.000000 fenjing-0.3.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6255 2023-05-18 07:35:00.349333 fenjing-0.3.3/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5817 2023-05-18 07:34:43.000000 fenjing-0.3.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-18 07:34:43.000000 fenjing-0.3.3/VERSION
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 07:35:00.349333 fenjing-0.3.3/fenjing/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      202 2023-05-18 07:34:43.000000 fenjing-0.3.3/fenjing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-18 07:34:43.000000 fenjing-0.3.3/fenjing/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6635 2023-05-18 07:34:43.000000 fenjing-0.3.3/fenjing/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      800 2023-05-18 07:34:43.000000 fenjing-0.3.3/fenjing/colorize.py
+-rw-r--r--   0 runner    (1001) docker     (123)      838 2023-05-18 07:34:43.000000 fenjing-0.3.3/fenjing/config_payload.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1486 2023-05-18 07:34:43.000000 fenjing-0.3.3/fenjing/const.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)       37 2023-05-18 07:34:43.000000 fenjing-0.3.3/fenjing/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2670 2023-05-18 07:34:43.000000 fenjing-0.3.3/fenjing/form.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5450 2023-05-18 07:34:43.000000 fenjing-0.3.3/fenjing/form_cracker.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3992 2023-05-18 07:34:43.000000 fenjing-0.3.3/fenjing/full_payload_gen.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2846 2023-05-18 07:34:43.000000 fenjing-0.3.3/fenjing/int_vars.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27358 2023-05-18 07:34:43.000000 fenjing-0.3.3/fenjing/payload_gen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1549 2023-05-18 07:34:43.000000 fenjing-0.3.3/fenjing/requester.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1180 2023-05-18 07:34:43.000000 fenjing-0.3.3/fenjing/scan_url.py
+-rw-r--r--   0 runner    (1001) docker     (123)      941 2023-05-18 07:34:43.000000 fenjing-0.3.3/fenjing/shell_payload.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 07:35:00.349333 fenjing-0.3.3/fenjing/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     8540 2023-05-18 07:34:43.000000 fenjing-0.3.3/fenjing/templates/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3192 2023-05-18 07:34:43.000000 fenjing-0.3.3/fenjing/waf_func_gen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8601 2023-05-18 07:34:43.000000 fenjing-0.3.3/fenjing/webui.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 07:35:00.349333 fenjing-0.3.3/fenjing.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6255 2023-05-18 07:35:00.000000 fenjing-0.3.3/fenjing.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-05-18 07:35:00.000000 fenjing-0.3.3/fenjing.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 07:35:00.000000 fenjing-0.3.3/fenjing.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-18 07:35:00.000000 fenjing-0.3.3/fenjing.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-18 07:35:00.000000 fenjing-0.3.3/fenjing.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-18 07:34:43.000000 fenjing-0.3.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-18 07:35:00.353333 fenjing-0.3.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      945 2023-05-18 07:34:43.000000 fenjing-0.3.3/setup.py
```

### Comparing `fenjing-0.3.2/LICENSE` & `fenjing-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `fenjing-0.3.2/PKG-INFO` & `fenjing-0.3.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fenjing
-Version: 0.3.2
+Version: 0.3.3
 Summary: A Jinja2 SSTI cracker for CTF competitions
 Home-page: https://github.com/Marven11/Fenjing
 Author: Marven11
 Author-email: marven11@example.com
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Operating System :: OS Independent
```

### Comparing `fenjing-0.3.2/README.md` & `fenjing-0.3.3/README.md`

 * *Files identical despite different names*

### Comparing `fenjing-0.3.2/fenjing/cli.py` & `fenjing-0.3.3/fenjing/cli.py`

 * *Files 5% similar despite different names*

```diff
@@ -191,12 +191,17 @@
             else:
                 print(cmd_exec_func(exec_cmd))
             return
     logger.warning("Scan failed...")
 
 
 @main.command()
-def webui():
-    webui_main()
+@click.option("--host", "-h", default = "127.0.0.1", help="需要监听的host, 默认为127.0.0.1")
+@click.option("--port", "-p", default = 11451, help="需要监听的端口, 默认为11451")
+def webui(host, port):
+    """
+    启动webui
+    """
+    webui_main(host, port)
 
 if __name__ == '__main__':
     main()
```

### Comparing `fenjing-0.3.2/fenjing/colorize.py` & `fenjing-0.3.3/fenjing/colorize.py`

 * *Files identical despite different names*

### Comparing `fenjing-0.3.2/fenjing/config_payload.py` & `fenjing-0.3.3/fenjing/config_payload.py`

 * *Files identical despite different names*

### Comparing `fenjing-0.3.2/fenjing/const.py` & `fenjing-0.3.3/fenjing/const.py`

 * *Files identical despite different names*

### Comparing `fenjing-0.3.2/fenjing/form.py` & `fenjing-0.3.3/fenjing/form.py`

 * *Files identical despite different names*

### Comparing `fenjing-0.3.2/fenjing/form_cracker.py` & `fenjing-0.3.3/fenjing/form_cracker.py`

 * *Files identical despite different names*

### Comparing `fenjing-0.3.2/fenjing/full_payload_gen.py` & `fenjing-0.3.3/fenjing/full_payload_gen.py`

 * *Files identical despite different names*

### Comparing `fenjing-0.3.2/fenjing/int_vars.py` & `fenjing-0.3.3/fenjing/int_vars.py`

 * *Files identical despite different names*

### Comparing `fenjing-0.3.2/fenjing/payload_gen.py` & `fenjing-0.3.3/fenjing/payload_gen.py`

 * *Files identical despite different names*

### Comparing `fenjing-0.3.2/fenjing/requester.py` & `fenjing-0.3.3/fenjing/requester.py`

 * *Files identical despite different names*

### Comparing `fenjing-0.3.2/fenjing/scan_url.py` & `fenjing-0.3.3/fenjing/scan_url.py`

 * *Files identical despite different names*

### Comparing `fenjing-0.3.2/fenjing/shell_payload.py` & `fenjing-0.3.3/fenjing/shell_payload.py`

 * *Files identical despite different names*

### Comparing `fenjing-0.3.2/fenjing/waf_func_gen.py` & `fenjing-0.3.3/fenjing/waf_func_gen.py`

 * *Files identical despite different names*

### Comparing `fenjing-0.3.2/fenjing/webui.py` & `fenjing-0.3.3/fenjing/webui.py`

 * *Files 1% similar despite different names*

```diff
@@ -70,15 +70,15 @@
         testsuccess_msg = "payload测试成功！" if data["test_success"] else "payload测试失败。"
         will_print_msg = "其会产生回显。" if data["will_print"] else "其不会产生回显。"
         self.messages.append(
             testsuccess_msg + will_print_msg
         )
 
     def __call__(self, callback_type, data):
-        def default_handler(data): 
+        def default_handler(data):
             return logger.warning(f"{callback_type=} not found")
         return {
             CALLBACK_PREPARE_FULLPAYLOADGEN: self.callback_prepare_fullpayloadgen,
             CALLBACK_GENERATE_FULLPAYLOAD: self.callback_generate_fullpayload,
             CALLBACK_GENERATE_PAYLOAD: self.callback_generate_payload,
             CALLBACK_SUBMIT: self.callback_submit,
             CALLBACK_TEST_FORM_INPUT: self.callback_test_form_input
@@ -146,27 +146,29 @@
         self.messages.append(r.text)
 
 
 @app.route("/")
 def index():
     return render_template("index.html")
 
+
 def create_crack_task(url, method, inputs, action, interval):
     form = Form(
         action=action or urlparse(url).path,
         method=method,
         inputs=inputs.split(",")
     )
     taskid = uuid.uuid4().hex
     task = CrackTaskThread(taskid, url, form, float(interval))
     task.daemon = True
     task.start()
     tasks[taskid] = task
     return taskid
 
+
 def create_interactive_id(cmd, last_task):
     cracker, field, full_payload_gen = (
         last_task.cracker,
         last_task.result.input_field,
         last_task.result.full_payload_gen
     )
     taskid = uuid.uuid4().hex
@@ -260,13 +262,13 @@
             "taskid": task.taskid,
             "done": not task.is_alive(),
             "messages": task.messages,
             "flash_messages": task.flash_messages,
         })
 
 
-def main():
-    app.run(host="127.0.0.1", port=11451)
+def main(host="127.0.0.1", port=11451):
+    app.run(host=host, port=port)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `fenjing-0.3.2/fenjing.egg-info/PKG-INFO` & `fenjing-0.3.3/fenjing.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fenjing
-Version: 0.3.2
+Version: 0.3.3
 Summary: A Jinja2 SSTI cracker for CTF competitions
 Home-page: https://github.com/Marven11/Fenjing
 Author: Marven11
 Author-email: marven11@example.com
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Operating System :: OS Independent
```

### Comparing `fenjing-0.3.2/setup.py` & `fenjing-0.3.3/setup.py`

 * *Files identical despite different names*

