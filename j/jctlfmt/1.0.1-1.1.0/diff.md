# Comparing `tmp/jctlfmt-1.0.1.tar.gz` & `tmp/jctlfmt-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jctlfmt-1.0.1.tar", last modified: Tue Apr 11 21:31:10 2023, max compression
+gzip compressed data, was "jctlfmt-1.1.0.tar", last modified: Thu May 18 11:14:53 2023, max compression
```

## Comparing `jctlfmt-1.0.1.tar` & `jctlfmt-1.1.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 21:31:10.219041 jctlfmt-1.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-04-11 21:30:53.000000 jctlfmt-1.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-04-11 21:31:10.219041 jctlfmt-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2098 2023-04-11 21:30:53.000000 jctlfmt-1.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 21:31:10.219041 jctlfmt-1.0.1/jctlfmt/
--rw-r--r--   0 runner    (1001) docker     (123)     4887 2023-04-11 21:30:53.000000 jctlfmt-1.0.1/jctlfmt/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 21:31:10.219041 jctlfmt-1.0.1/jctlfmt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-04-11 21:31:10.000000 jctlfmt-1.0.1/jctlfmt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-04-11 21:31:10.000000 jctlfmt-1.0.1/jctlfmt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 21:31:10.000000 jctlfmt-1.0.1/jctlfmt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-11 21:31:10.000000 jctlfmt-1.0.1/jctlfmt.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-04-11 21:31:10.219041 jctlfmt-1.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-04-11 21:30:53.000000 jctlfmt-1.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 11:14:53.270508 jctlfmt-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-05-18 11:14:37.000000 jctlfmt-1.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-05-18 11:14:53.270508 jctlfmt-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2616 2023-05-18 11:14:37.000000 jctlfmt-1.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 11:14:53.270508 jctlfmt-1.1.0/jctlfmt/
+-rw-r--r--   0 runner    (1001) docker     (123)     5003 2023-05-18 11:14:37.000000 jctlfmt-1.1.0/jctlfmt/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 11:14:53.270508 jctlfmt-1.1.0/jctlfmt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-05-18 11:14:53.000000 jctlfmt-1.1.0/jctlfmt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-05-18 11:14:53.000000 jctlfmt-1.1.0/jctlfmt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 11:14:53.000000 jctlfmt-1.1.0/jctlfmt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-18 11:14:53.000000 jctlfmt-1.1.0/jctlfmt.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-05-18 11:14:53.270508 jctlfmt-1.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-05-18 11:14:37.000000 jctlfmt-1.1.0/setup.py
```

### Comparing `jctlfmt-1.0.1/LICENSE` & `jctlfmt-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `jctlfmt-1.0.1/PKG-INFO` & `jctlfmt-1.1.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jctlfmt
-Version: 1.0.1
+Version: 1.1.0
 Summary: Python Journalctl parsing and formatting library
 Home-page: https://github.com/dmotte/jctlfmt
 Author: dmotte
 License: MIT
 Keywords: fmt journal parsing log text formatting systemd format logs msg message journald messages filtering journalctl systemd-journald jctl
 Classifier: Intended Audience :: System Administrators
 Classifier: Environment :: Console
```

### Comparing `jctlfmt-1.0.1/README.md` & `jctlfmt-1.1.0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -17,29 +17,38 @@
 ## Usage
 
 You can use the `jctlfmt.Entry` class in your code to **parse** _Journalctl_ messages from **JSON format** and then you can create **your own formatter class** by extending `jctlfmt.BaseFormatter` to filter and print the entries in the format you like.
 
 I have put a full usage example in the [`example`](example) folder of this repo. To try it you can use the following commands:
 
 ```bash
-sudo journalctl -ojson --output-fields _SOURCE_REALTIME_TIMESTAMP,__REALTIME_TIMESTAMP,_HOSTNAME,_SYSTEMD_UNIT,SYSLOG_IDENTIFIER,_PID,PRIORITY,MESSAGE -S '1 day ago' > example/step01-json.txt
+ssh myuser@myserver.example.com "sudo journalctl -ojson --output-fields _SOURCE_REALTIME_TIMESTAMP,__REALTIME_TIMESTAMP,_HOSTNAME,_SYSTEMD_UNIT,SYSLOG_IDENTIFIER,_PID,PRIORITY,MESSAGE -S '1 day ago'" > example/step01-json.txt
 python3 example/dedup.py < example/step01-json.txt > example/step02-dedup.txt
 python3 example/fmt.py < example/step02-dedup.txt > example/step03-fmt.txt
 ```
 
 As you can see I have two custom scripts: [`dedup.py`](example/dedup.py), which removes duplicate lines based on custom rules, and [`fmt.py`](example/fmt.py) which does the actual filtering and formatting.
 
 In alternative, you can also use [`fmt.py`](example/fmt.py) to explore _Journalctl_ logs on the go:
 
 ```bash
 sudo journalctl -ojson -ussh -S '1 day ago' | python3 example/fmt.py -fs | less
 ```
 
 As you can see, this time I invoked the script with `-fs` to disable filtering and sensitive mode. See `jctlfmt.BaseFormatter` for details.
 
+You can customize [`fmt.py`](example/fmt.py) as you want and then use it in your setup. If you make modifications to the script and you want to test if the output is consistent, you can generate the output for all the possible invocations and then use `sha256sum` to check. The following commands may help:
+
+```bash
+for i in '' -f -fs -s; do
+    python3 example/fmt.py $i < example/step02-dedup.txt > "example/step03-arg$i.txt"
+done
+sha256sum example/step03-arg*.txt | sha256sum
+```
+
 ## Development
 
 If you want to contribute to this project, you can install the package in **editable** mode:
 
 ```bash
 pip3 install -e . --user
 ```
```

### Comparing `jctlfmt-1.0.1/jctlfmt/__init__.py` & `jctlfmt-1.1.0/jctlfmt/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,15 +49,18 @@
 
         self.pid: str = raw.get('_PID', '')
         'Process ID'
 
         self.prio = int(raw.get('PRIORITY', -1))
         'Priority of the message (as int)'
 
-        self.msg: str = raw['MESSAGE']
+        self.msg: str = (
+            bytes(raw['MESSAGE']).decode() if isinstance(raw['MESSAGE'], list)
+            else raw['MESSAGE']
+        ).strip()
         'Message text'
 
     @property
     def str_ui(self):
         '''
         Returns `(unit) ident` omitting the empty parts
         '''
```

### Comparing `jctlfmt-1.0.1/jctlfmt.egg-info/PKG-INFO` & `jctlfmt-1.1.0/jctlfmt.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jctlfmt
-Version: 1.0.1
+Version: 1.1.0
 Summary: Python Journalctl parsing and formatting library
 Home-page: https://github.com/dmotte/jctlfmt
 Author: dmotte
 License: MIT
 Keywords: fmt journal parsing log text formatting systemd format logs msg message journald messages filtering journalctl systemd-journald jctl
 Classifier: Intended Audience :: System Administrators
 Classifier: Environment :: Console
```

### Comparing `jctlfmt-1.0.1/setup.cfg` & `jctlfmt-1.1.0/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 	Natural Language :: English
 	License :: OSI Approved :: MIT License
 	Programming Language :: Python
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3 :: Only
 	Programming Language :: Python :: 3.9
 	Topic :: Utilities
-version = 1.0.1
+version = 1.1.0
 
 [options]
 install_requires = 
 python_requires = >=3.9.1
 packages = jctlfmt
 
 [egg_info]
```

