# Comparing `tmp/siru-0.4.tar.gz` & `tmp/siru-0.5.tar.gz`

## Comparing `siru-0.4.tar` & `siru-0.5.tar`

### file list

```diff
@@ -1,33 +1,32 @@
--rw-r--r--   0        0        0      424 2020-02-02 00:00:00.000000 siru-0.4/.clang-format
--rw-r--r--   0        0        0      668 2020-02-02 00:00:00.000000 siru-0.4/.pre-commit-config.yaml
--rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 siru-0.4/.github/workflows/pre-commit.yml
--rw-r--r--   0        0        0      746 2020-02-02 00:00:00.000000 siru-0.4/.vscode/settings.json
--rw-r--r--   0        0        0    10870 2020-02-02 00:00:00.000000 siru-0.4/doc/protocolo.md
--rw-r--r--   0        0        0     1695 2020-02-02 00:00:00.000000 siru-0.4/src/siru/__about__.py
--rw-r--r--   0        0        0     1674 2020-02-02 00:00:00.000000 siru-0.4/src/siru/__init__.py
--rw-r--r--   0        0        0     3780 2020-02-02 00:00:00.000000 siru-0.4/src/siru/ate.py
--rw-r--r--   0        0        0     3893 2020-02-02 00:00:00.000000 siru-0.4/src/siru/dut.py
--rw-r--r--   0        0        0     4810 2020-02-02 00:00:00.000000 siru-0.4/src/siru/gpio.py
--rwxr-xr-x   0        0        0     6202 2020-02-02 00:00:00.000000 siru-0.4/src/siru/preat.py
--rw-r--r--   0        0        0     2117 2020-02-02 00:00:00.000000 siru-0.4/src/siru/prueba.py
--rw-r--r--   0        0        0     8784 2020-02-02 00:00:00.000000 siru-0.4/src/siru/tasks.py
--rw-r--r--   0        0        0     1719 2020-02-02 00:00:00.000000 siru-0.4/src/siru/remote/__init__.py
--rw-r--r--   0        0        0     1674 2020-02-02 00:00:00.000000 siru-0.4/tests/__init__.py
--rw-r--r--   0        0        0     4061 2020-02-02 00:00:00.000000 siru-0.4/tests/test_ate.py
--rw-r--r--   0        0        0     3376 2020-02-02 00:00:00.000000 siru-0.4/tests/test_dut.py
--rw-r--r--   0        0        0     9068 2020-02-02 00:00:00.000000 siru-0.4/tests/test_gpio.py
--rw-r--r--   0        0        0     8464 2020-02-02 00:00:00.000000 siru-0.4/tests/test_preat.py
--rw-r--r--   0        0        0     8258 2020-02-02 00:00:00.000000 siru-0.4/tests/test_tasks.py
--rw-r--r--   0        0        0     2098 2020-02-02 00:00:00.000000 siru-0.4/tests/utils.py
--rw-r--r--   0        0        0      589 2020-02-02 00:00:00.000000 siru-0.4/tests/data/ate_test.yaml
--rw-r--r--   0        0        0      605 2020-02-02 00:00:00.000000 siru-0.4/tests/data/dut_test.yaml
--rw-r--r--   0        0        0      774 2020-02-02 00:00:00.000000 siru-0.4/tests/data/tasks_test.yaml
--rw-r--r--   0        0        0     2863 2020-02-02 00:00:00.000000 siru-0.4/tests/ruwaq/expected/inc/config.h
--rw-r--r--   0        0        0     3469 2020-02-02 00:00:00.000000 siru-0.4/tests/ruwaq/expected/src/config.c
--rw-r--r--   0        0        0     2908 2020-02-02 00:00:00.000000 siru-0.4/tests/ruwaq/template/inc/config.h
--rw-r--r--   0        0        0     3166 2020-02-02 00:00:00.000000 siru-0.4/tests/ruwaq/template/src/config.c
--rw-r--r--   0        0        0     4676 2020-02-02 00:00:00.000000 siru-0.4/.gitignore
--rw-r--r--   0        0        0     1305 2020-02-02 00:00:00.000000 siru-0.4/LICENSE.txt
--rw-r--r--   0        0        0      562 2020-02-02 00:00:00.000000 siru-0.4/README.md
--rw-r--r--   0        0        0     1900 2020-02-02 00:00:00.000000 siru-0.4/pyproject.toml
--rw-r--r--   0        0        0     1716 2020-02-02 00:00:00.000000 siru-0.4/PKG-INFO
+-rw-r--r--   0        0        0      424 2020-02-02 00:00:00.000000 siru-0.5/.clang-format
+-rw-r--r--   0        0        0      668 2020-02-02 00:00:00.000000 siru-0.5/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     3605 2020-02-02 00:00:00.000000 siru-0.5/prueba.py
+-rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 siru-0.5/.github/workflows/pre-commit.yml
+-rw-r--r--   0        0        0      746 2020-02-02 00:00:00.000000 siru-0.5/.vscode/settings.json
+-rw-r--r--   0        0        0    10870 2020-02-02 00:00:00.000000 siru-0.5/doc/protocolo.md
+-rw-r--r--   0        0        0     1695 2020-02-02 00:00:00.000000 siru-0.5/src/siru/__about__.py
+-rw-r--r--   0        0        0     1674 2020-02-02 00:00:00.000000 siru-0.5/src/siru/__init__.py
+-rw-r--r--   0        0        0     3780 2020-02-02 00:00:00.000000 siru-0.5/src/siru/ate.py
+-rw-r--r--   0        0        0     3893 2020-02-02 00:00:00.000000 siru-0.5/src/siru/dut.py
+-rw-r--r--   0        0        0     4810 2020-02-02 00:00:00.000000 siru-0.5/src/siru/gpio.py
+-rwxr-xr-x   0        0        0     6528 2020-02-02 00:00:00.000000 siru-0.5/src/siru/preat.py
+-rw-r--r--   0        0        0     8784 2020-02-02 00:00:00.000000 siru-0.5/src/siru/tasks.py
+-rw-r--r--   0        0        0     1674 2020-02-02 00:00:00.000000 siru-0.5/tests/__init__.py
+-rw-r--r--   0        0        0     4061 2020-02-02 00:00:00.000000 siru-0.5/tests/test_ate.py
+-rw-r--r--   0        0        0     3376 2020-02-02 00:00:00.000000 siru-0.5/tests/test_dut.py
+-rw-r--r--   0        0        0     9068 2020-02-02 00:00:00.000000 siru-0.5/tests/test_gpio.py
+-rw-r--r--   0        0        0     8464 2020-02-02 00:00:00.000000 siru-0.5/tests/test_preat.py
+-rw-r--r--   0        0        0     8258 2020-02-02 00:00:00.000000 siru-0.5/tests/test_tasks.py
+-rw-r--r--   0        0        0     2098 2020-02-02 00:00:00.000000 siru-0.5/tests/utils.py
+-rw-r--r--   0        0        0      589 2020-02-02 00:00:00.000000 siru-0.5/tests/data/ate_test.yaml
+-rw-r--r--   0        0        0      605 2020-02-02 00:00:00.000000 siru-0.5/tests/data/dut_test.yaml
+-rw-r--r--   0        0        0      774 2020-02-02 00:00:00.000000 siru-0.5/tests/data/tasks_test.yaml
+-rw-r--r--   0        0        0     2863 2020-02-02 00:00:00.000000 siru-0.5/tests/ruwaq/expected/inc/config.h
+-rw-r--r--   0        0        0     3469 2020-02-02 00:00:00.000000 siru-0.5/tests/ruwaq/expected/src/config.c
+-rw-r--r--   0        0        0     2908 2020-02-02 00:00:00.000000 siru-0.5/tests/ruwaq/template/inc/config.h
+-rw-r--r--   0        0        0     3166 2020-02-02 00:00:00.000000 siru-0.5/tests/ruwaq/template/src/config.c
+-rw-r--r--   0        0        0     4676 2020-02-02 00:00:00.000000 siru-0.5/.gitignore
+-rw-r--r--   0        0        0     1305 2020-02-02 00:00:00.000000 siru-0.5/LICENSE.txt
+-rw-r--r--   0        0        0     1215 2020-02-02 00:00:00.000000 siru-0.5/README.md
+-rw-r--r--   0        0        0     1988 2020-02-02 00:00:00.000000 siru-0.5/pyproject.toml
+-rw-r--r--   0        0        0     2369 2020-02-02 00:00:00.000000 siru-0.5/PKG-INFO
```

### Comparing `siru-0.4/.pre-commit-config.yaml` & `siru-0.5/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `siru-0.4/.vscode/settings.json` & `siru-0.5/.vscode/settings.json`

 * *Files identical despite different names*

### Comparing `siru-0.4/doc/protocolo.md` & `siru-0.5/doc/protocolo.md`

 * *Files identical despite different names*

### Comparing `siru-0.4/src/siru/__about__.py` & `siru-0.5/src/siru/__about__.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,8 +23,8 @@
 # OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN
 # CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
 #
 # SPDX-License-Identifier: MIT
 # SPDX-FileCopyrightText: 2023, Esteban Volentini <evolentini@herrera.unt.edu.ar>
 ##################################################################################################
 
-__version__ = "0.4"
+__version__ = "0.5"
```

### Comparing `siru-0.4/src/siru/__init__.py` & `siru-0.5/src/siru/__init__.py`

 * *Files identical despite different names*

### Comparing `siru-0.4/src/siru/ate.py` & `siru-0.5/src/siru/ate.py`

 * *Files identical despite different names*

### Comparing `siru-0.4/src/siru/dut.py` & `siru-0.5/src/siru/dut.py`

 * *Files identical despite different names*

### Comparing `siru-0.4/src/siru/gpio.py` & `siru-0.5/src/siru/gpio.py`

 * *Files identical despite different names*

### Comparing `siru-0.4/src/siru/preat.py` & `siru-0.5/src/siru/preat.py`

 * *Files 4% similar despite different names*

```diff
@@ -28,14 +28,15 @@
 ##################################################################################################
 
 from typing import List
 from enum import Enum
 from crc import Calculator, Configuration
 from struct import pack
 from serial import Serial
+from serial.tools import list_ports
 
 
 class Result(Enum):
     NO_ERROR = 0x00
     CRC_ERROR = 0x01
     METHOD_ERROR = 0x02
     PARAMETERS_ERROR = 0x03
@@ -109,17 +110,25 @@
                 optimized=True,
             )
         return self._crc
 
     @property
     def port(self) -> Serial:
         if self._port == None:
-            self._port = Serial(port=self._url, baudrate=115200)
+            self._port = Serial(port=self.serial_url, baudrate=115200)
         return self._port
 
+    def serial_url(self) -> str:
+        location = self._url.split("//")
+        if location[0].lower() == "usb:":
+            for port in list_ports.comports():
+                if str(port.location).startswith(location[1]):
+                    return port
+        return self._url
+
     @property
     def url(self) -> Serial:
         return self._url
 
     @url.setter
     def url(self, value) -> Serial:
         self._url = value
```

### Comparing `siru-0.4/src/siru/prueba.py` & `siru-0.5/tests/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -22,27 +22,7 @@
 # NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES
 # OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN
 # CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
 #
 # SPDX-License-Identifier: MIT
 # SPDX-FileCopyrightText: 2023, Esteban Volentini <evolentini@herrera.unt.edu.ar>
 ##################################################################################################
-
-from remote import Preat
-from remote.gpio import Output, Input
-
-port = "/dev/tty.usbserial-14401"
-preat = Preat(port)
-led_r = Output(preat, 0)
-led_g = Output(preat, 1)
-led_b = Output(preat, 2)
-led_1 = Output(preat, 3)
-led_2 = Output(preat, 4)
-
-tec_1 = Input(preat, 0)
-tec_2 = Input(preat, 1)
-tec_3 = Input(preat, 2)
-tec_4 = Input(preat, 3)
-
-preat.wait(100, 5000, [tec_1.has_rising, tec_2.has_falling], led_r.set)
-# led_r.set()
-led_r.toogle()
```

### Comparing `siru-0.4/src/siru/tasks.py` & `siru-0.5/src/siru/tasks.py`

 * *Files identical despite different names*

### Comparing `siru-0.4/src/siru/remote/__init__.py` & `siru-0.5/LICENSE.txt`

 * *Files 17% similar despite different names*

```diff
@@ -1,30 +1,28 @@
-#!/usr/bin/env python3
-# -*- coding: utf-8 -*-
+MIT License
 
-##################################################################################################
-# Copyright (c) 2022-2023, Laboratorio de Microprocesadores
-# Facultad de Ciencias Exactas y Tecnología, Universidad Nacional de Tucumán
-# https://www.microprocesadores.unt.edu.ar/
-#
-# Copyright (c) 2022-2023, Esteban Volentini <evolentini@herrera.unt.edu.ar>
-#
-# Permission is hereby granted, free of charge, to any person obtaining a copy of this software and
-# associated documentation files (the "Software"), to deal in the Software without restriction,
-# including without limitation the rights to use, copy, modify, merge, publish, distribute,
-# sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is
-# furnished to do so, subject to the following conditions:
-#
-# The above copyright notice and this permission notice shall be included in all copies or substantial
-# portions of the Software.
-#
-# THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT
-# NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND
-# NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES
-# OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN
-# CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
-#
-# SPDX-License-Identifier: MIT
-# SPDX-FileCopyrightText: 2023, Esteban Volentini <evolentini@herrera.unt.edu.ar>
-##################################################################################################
+Copyright 2022, Laboratorio de Microprocesadores
+Facultad de Ciencias Exactas y Tecnología
+Universidad Nacional de Tucumán
+https://www.microprocesadores.unt.edu.ar/
 
-from .preat import Preat, Parameter, Result
+Copyright (c) 2023, Esteban Volentini <evolentini@herrera.unt.edu.ar>
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
+
+SPDX-License-Identifier: MIT
```

### Comparing `siru-0.4/tests/__init__.py` & `siru-0.5/tests/utils.py`

 * *Files 22% similar despite different names*

```diff
@@ -22,7 +22,24 @@
 # NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES
 # OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN
 # CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
 #
 # SPDX-License-Identifier: MIT
 # SPDX-FileCopyrightText: 2023, Esteban Volentini <evolentini@herrera.unt.edu.ar>
 ##################################################################################################
+
+import yaml
+from yamlinclude import YamlIncludeConstructor
+from pathlib import Path
+from typing import Dict
+
+DATA_DIR = Path(__file__).parent / "data"
+
+
+def load_config(filename: str) -> Dict:
+    YamlIncludeConstructor.add_to_loader_class(
+        loader_class=yaml.FullLoader, base_dir=DATA_DIR
+    )
+
+    with open(DATA_DIR / filename) as file:
+        result = yaml.load(file, Loader=yaml.FullLoader)
+    return result
```

### Comparing `siru-0.4/tests/test_ate.py` & `siru-0.5/tests/test_ate.py`

 * *Files identical despite different names*

### Comparing `siru-0.4/tests/test_dut.py` & `siru-0.5/tests/test_dut.py`

 * *Files identical despite different names*

### Comparing `siru-0.4/tests/test_gpio.py` & `siru-0.5/tests/test_gpio.py`

 * *Files identical despite different names*

### Comparing `siru-0.4/tests/test_preat.py` & `siru-0.5/tests/test_preat.py`

 * *Files identical despite different names*

### Comparing `siru-0.4/tests/test_tasks.py` & `siru-0.5/tests/test_tasks.py`

 * *Files identical despite different names*

### Comparing `siru-0.4/tests/data/ate_test.yaml` & `siru-0.5/tests/data/ate_test.yaml`

 * *Files identical despite different names*

### Comparing `siru-0.4/tests/data/dut_test.yaml` & `siru-0.5/tests/data/dut_test.yaml`

 * *Files identical despite different names*

### Comparing `siru-0.4/tests/data/tasks_test.yaml` & `siru-0.5/tests/data/tasks_test.yaml`

 * *Files identical despite different names*

### Comparing `siru-0.4/tests/ruwaq/expected/inc/config.h` & `siru-0.5/tests/ruwaq/expected/inc/config.h`

 * *Files identical despite different names*

### Comparing `siru-0.4/tests/ruwaq/expected/src/config.c` & `siru-0.5/tests/ruwaq/expected/src/config.c`

 * *Files identical despite different names*

### Comparing `siru-0.4/tests/ruwaq/template/inc/config.h` & `siru-0.5/tests/ruwaq/template/inc/config.h`

 * *Files identical despite different names*

### Comparing `siru-0.4/tests/ruwaq/template/src/config.c` & `siru-0.5/tests/ruwaq/template/src/config.c`

 * *Files identical despite different names*

### Comparing `siru-0.4/.gitignore` & `siru-0.5/.gitignore`

 * *Files identical despite different names*

### Comparing `siru-0.4/pyproject.toml` & `siru-0.5/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -43,14 +43,15 @@
 path = "src/siru/__about__.py"
 
 [tool.hatch.envs.default]
 dependencies = ["pytest", "pytest-mock", "pytest-cov", "pycrc"]
 
 [tool.hatch.envs.default.scripts]
 cov = "pytest --cov-report=term-missing --cov-config=pyproject.toml --cov=src/siru --cov=tests {args}"
+html-cov = "pytest --cov-report=html --cov-config=pyproject.toml --cov=src/siru {args}"
 no-cov = "cov --no-cov {args}"
 
 [[tool.hatch.envs.test.matrix]]
 python = ["37", "38", "39", "310", "311"]
 
 [tool.coverage.run]
 branch = true
```

### Comparing `siru-0.4/PKG-INFO` & `siru-0.5/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: siru
-Version: 0.4
+Version: 0.5
 Summary: Automated tests on hardware for embedded systems
 Project-URL: Documentation, https://github.com/labmicro/siru#readme
 Project-URL: Issues, https://github.com/labmicro/siru/issues
 Project-URL: Source, https://github.com/labmicro/siru
 Author-email: Esteban Volentini <evolentini@herrera.unt.edu.ar>
 License-Expression: MIT
 License-File: LICENSE.txt
@@ -43,11 +43,50 @@
 - [License](#license)
 
 ## Installation
 
 ```console
 pip install siru
 ```
+## Arquitectura Ruwaq
 
+@startuml
+skinparam componentStyle uml1
+
+frame "Microkernel" {
+    [Despachador] -l-> Ejecutar : usa
+    Ejecutar <.l. [Servidor PREAT] : usa
+
+    port Registrar
+    [Despachador] -r-> Registrar
+
+    [Servidor PREAT] ..> Enviar : usa
+    [Servidor PREAT] ..> Recibido : usa
+
+    Recibido <-- [Transporte]
+    Enviar <-- [Transporte]
+}
+
+Registrar <.. [GPIO]: usa
+[Despachador] --> [GPIO]
+@enduml
+
+## Arquitectura Siru
+
+@startuml
+skinparam componentStyle uml1
+
+[DUT] -right-> [ATE]
+
+[ATE] -right-> [GPIO]
+
+[ATE] ..> Ejecutar: usa
+[ATE] ..> Esperar: usa
+[GPIO] ..> Ejecutar: usa
+
+Ejecutar <-- [PREAT]
+Esperar <-- [PREAT]
+@enduml
+siru
 ## License
 
 `SIRU` is distributed under the terms of the [MIT](https://spdx.org/licenses/MIT.html) license.
```

