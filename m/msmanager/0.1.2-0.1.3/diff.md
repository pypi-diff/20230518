# Comparing `tmp/msmanager-0.1.2.tar.gz` & `tmp/msmanager-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "msmanager-0.1.2.tar", max compression
+gzip compressed data, was "msmanager-0.1.3.tar", max compression
```

## Comparing `msmanager-0.1.2.tar` & `msmanager-0.1.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1111 2023-05-14 16:04:08.180554 msmanager-0.1.2/LICENSE
--rw-r--r--   0        0        0      267 2023-05-15 20:57:42.797028 msmanager-0.1.2/msmanager/__init__.py
--rw-r--r--   0        0        0       67 2023-05-15 21:27:48.138274 msmanager-0.1.2/msmanager/__main__.py
--rw-r--r--   0        0        0     4189 2023-05-16 17:48:34.367885 msmanager-0.1.2/msmanager/cli.py
--rw-r--r--   0        0        0     2488 2023-05-15 19:04:10.101041 msmanager-0.1.2/msmanager/config.py
--rw-r--r--   0        0        0     2793 2023-05-15 20:31:27.149266 msmanager-0.1.2/msmanager/exceptions.py
--rw-r--r--   0        0        0     3224 2023-05-16 16:35:54.115596 msmanager-0.1.2/msmanager/functions.py
--rw-r--r--   0        0        0      384 2023-05-16 16:36:36.800666 msmanager-0.1.2/msmanager/models.py
--rw-r--r--   0        0        0     2907 2023-05-15 21:23:04.177803 msmanager-0.1.2/msmanager/msm.py
--rw-r--r--   0        0        0      143 2023-05-15 19:04:10.113824 msmanager-0.1.2/msmanager/types.py
--rw-r--r--   0        0        0      533 2023-05-16 17:48:52.519457 msmanager-0.1.2/msmanager/units.py
--rw-r--r--   0        0        0      547 2023-05-16 18:10:12.484055 msmanager-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      484 2023-05-16 18:07:58.584057 msmanager-0.1.2/README.md
--rw-r--r--   0        0        0     1284 1970-01-01 00:00:00.000000 msmanager-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1111 2023-05-14 16:04:08.180554 msmanager-0.1.3/LICENSE
+-rw-r--r--   0        0        0      267 2023-05-15 20:57:42.797028 msmanager-0.1.3/msmanager/__init__.py
+-rw-r--r--   0        0        0       67 2023-05-15 21:27:48.138274 msmanager-0.1.3/msmanager/__main__.py
+-rw-r--r--   0        0        0     5968 2023-05-17 21:50:42.885439 msmanager-0.1.3/msmanager/cli.py
+-rw-r--r--   0        0        0     2488 2023-05-15 19:04:10.101041 msmanager-0.1.3/msmanager/config.py
+-rw-r--r--   0        0        0     2793 2023-05-15 20:31:27.149266 msmanager-0.1.3/msmanager/exceptions.py
+-rw-r--r--   0        0        0     3441 2023-05-17 21:45:18.685171 msmanager-0.1.3/msmanager/functions.py
+-rw-r--r--   0        0        0      384 2023-05-16 16:36:36.800666 msmanager-0.1.3/msmanager/models.py
+-rw-r--r--   0        0        0     2997 2023-05-17 21:08:14.055219 msmanager-0.1.3/msmanager/msm.py
+-rw-r--r--   0        0        0      143 2023-05-15 19:04:10.113824 msmanager-0.1.3/msmanager/types.py
+-rw-r--r--   0        0        0      533 2023-05-17 21:01:49.385592 msmanager-0.1.3/msmanager/units.py
+-rw-r--r--   0        0        0      547 2023-05-17 21:01:52.515921 msmanager-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0      565 2023-05-16 18:14:53.984547 msmanager-0.1.3/README.md
+-rw-r--r--   0        0        0     1364 1970-01-01 00:00:00.000000 msmanager-0.1.3/PKG-INFO
```

### Comparing `msmanager-0.1.2/LICENSE` & `msmanager-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `msmanager-0.1.2/msmanager/config.py` & `msmanager-0.1.3/msmanager/config.py`

 * *Files identical despite different names*

### Comparing `msmanager-0.1.2/msmanager/exceptions.py` & `msmanager-0.1.3/msmanager/exceptions.py`

 * *Files identical despite different names*

### Comparing `msmanager-0.1.2/msmanager/functions.py` & `msmanager-0.1.3/msmanager/functions.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-import time
 import pydustry
 import platform
 from versioner import Version
 from vbml import Pattern, Patcher
 from subprocess import getstatusoutput
 from typing import Tuple, Dict, Any, Iterable
 # * Local Imports
@@ -20,15 +19,18 @@
     for __old, __new in replaceble.items():
         string = string.replace(__old, __new)
     return string
 
 def rich_exception(exception: Exception) -> str:
     return f"[red]{exception.__class__.__name__}:[/] {' '.join(exception.args)}"
 
-# ! ...
+def endicext(string: str) -> str:
+    return string + ("[/]" * string.count("]"))
+
+# ! Server Functions
 def wait_start_server(
     server_host: str,
     port: int=6567,
     input_port: int=6859,
     per_second: float=1
 ) -> None:
     server = pydustry.Server(server_host, port, input_port)
@@ -38,14 +40,17 @@
             break
         except:
             pass
 
 def is_server_connect_correct(server_host: str, port: int, input_port: int) -> bool:
     return isinstance(server_host, str) and isinstance(port, int) and isinstance(input_port, int)
 
+def ping(host: str, port: int, timeout: int=10) -> pydustry.Status:
+    return pydustry.Server(host, port).get_status(timeout)
+
 # ! Subproccess Functions
 def runner(*args: str) -> Tuple[int, str]:
     return getstatusoutput(" ".join([*args]))
 
 def exists_screen() -> bool:
     return runner("screen", "-v")[0] == 0
```

### Comparing `msmanager-0.1.2/msmanager/msm.py` & `msmanager-0.1.3/msmanager/msm.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import os
 import screens
 from typing import Optional
 from versioner import Version
+from pydustry import Server, Status
 # * Local Imports
 from .units import CONFIG_PATH
 from .config import MSManagerConfig
 from .models import MindustryServerConfig
 from .functions import get_mindustry_server_version, checking_environment
 from .exceptions import ServerNotExistsError, ServerIsStartedError, ServerIsStoppedError
 
@@ -59,8 +60,9 @@
             if server_screen is not None:
                 server_screen.kill()
                 screens.wipe()
             else:
                 raise ServerIsStoppedError(screen_name)
         else:
             raise ServerNotExistsError(screen_name)
-    
+    
+    def ping(self, screen_name: str) -> Status: ...
```

### Comparing `msmanager-0.1.2/msmanager/units.py` & `msmanager-0.1.3/msmanager/units.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import os
 from platformdirs import user_config_dir
 
 # ! Metadata
 __name__ = "msmanager"
-__version__ = "0.1.2"
+__version__ = "0.1.3"
 __author__ = "RCR"
 __email__ = "semina054@gmail.com"
 __url__ = "https://github.com/RCR-OOP/msmanager"
 
 # ! Constants
 SUPPORT_PLATFORMS = [
     "windows-amd64", "windows-x86_64", "linux-x86_64"
```

### Comparing `msmanager-0.1.2/pyproject.toml` & `msmanager-0.1.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "msmanager"
-version = "0.1.2"
+version = "0.1.3"
 description = "Manager for managing Mindusrty servers."
 authors = ["Romanin <semina054@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "msmanager"}]
 
 [tool.poetry.dependencies]
```

### Comparing `msmanager-0.1.2/PKG-INFO` & `msmanager-0.1.3/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: msmanager
-Version: 0.1.2
+Version: 0.1.3
 Summary: Manager for managing Mindusrty servers.
 License: MIT
 Author: Romanin
 Author-email: semina054@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -25,21 +25,22 @@
 ## Description
 Manager for managing Mindusrty servers.
 ## Install
 ```shell
 python3 -m pip install --upgrade msmanager
 ```
 ## Usage
-```shell
+```
 Usage: python -m msmanager [OPTIONS] COMMAND [ARGS]...
 
 Options:
-  --not-check-environment
+  --not-check-environment  Disables checks for GNU Screen, Java and system support.
   --help                   Show this message and exit.
 
 Commands:
   add     Add a server to the config.
   list    List of servers in the config.
   remove  Remove the server from the config.
   start   Run the server.
+  stop    Stop the server.
 ```
```

