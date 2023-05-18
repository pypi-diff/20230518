# Comparing `tmp/siru-0.6.tar.gz` & `tmp/siru-0.7.tar.gz`

## Comparing `siru-0.6.tar` & `siru-0.7.tar`

### file list

```diff
@@ -1,32 +1,32 @@
--rw-r--r--   0        0        0      424 2020-02-02 00:00:00.000000 siru-0.6/.clang-format
--rw-r--r--   0        0        0      668 2020-02-02 00:00:00.000000 siru-0.6/.pre-commit-config.yaml
--rw-r--r--   0        0        0     3605 2020-02-02 00:00:00.000000 siru-0.6/prueba.py
--rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 siru-0.6/.github/workflows/pre-commit.yml
--rw-r--r--   0        0        0      746 2020-02-02 00:00:00.000000 siru-0.6/.vscode/settings.json
--rw-r--r--   0        0        0    10870 2020-02-02 00:00:00.000000 siru-0.6/doc/protocolo.md
--rw-r--r--   0        0        0     1695 2020-02-02 00:00:00.000000 siru-0.6/src/siru/__about__.py
--rw-r--r--   0        0        0     1674 2020-02-02 00:00:00.000000 siru-0.6/src/siru/__init__.py
--rw-r--r--   0        0        0     3780 2020-02-02 00:00:00.000000 siru-0.6/src/siru/ate.py
--rw-r--r--   0        0        0     3893 2020-02-02 00:00:00.000000 siru-0.6/src/siru/dut.py
--rw-r--r--   0        0        0     4810 2020-02-02 00:00:00.000000 siru-0.6/src/siru/gpio.py
--rwxr-xr-x   0        0        0     6549 2020-02-02 00:00:00.000000 siru-0.6/src/siru/preat.py
--rw-r--r--   0        0        0     8784 2020-02-02 00:00:00.000000 siru-0.6/src/siru/tasks.py
--rw-r--r--   0        0        0     1674 2020-02-02 00:00:00.000000 siru-0.6/tests/__init__.py
--rw-r--r--   0        0        0     4061 2020-02-02 00:00:00.000000 siru-0.6/tests/test_ate.py
--rw-r--r--   0        0        0     3376 2020-02-02 00:00:00.000000 siru-0.6/tests/test_dut.py
--rw-r--r--   0        0        0     9068 2020-02-02 00:00:00.000000 siru-0.6/tests/test_gpio.py
--rw-r--r--   0        0        0     8464 2020-02-02 00:00:00.000000 siru-0.6/tests/test_preat.py
--rw-r--r--   0        0        0     8258 2020-02-02 00:00:00.000000 siru-0.6/tests/test_tasks.py
--rw-r--r--   0        0        0     2098 2020-02-02 00:00:00.000000 siru-0.6/tests/utils.py
--rw-r--r--   0        0        0      589 2020-02-02 00:00:00.000000 siru-0.6/tests/data/ate_test.yaml
--rw-r--r--   0        0        0      605 2020-02-02 00:00:00.000000 siru-0.6/tests/data/dut_test.yaml
--rw-r--r--   0        0        0      774 2020-02-02 00:00:00.000000 siru-0.6/tests/data/tasks_test.yaml
--rw-r--r--   0        0        0     2863 2020-02-02 00:00:00.000000 siru-0.6/tests/ruwaq/expected/inc/config.h
--rw-r--r--   0        0        0     3469 2020-02-02 00:00:00.000000 siru-0.6/tests/ruwaq/expected/src/config.c
--rw-r--r--   0        0        0     2908 2020-02-02 00:00:00.000000 siru-0.6/tests/ruwaq/template/inc/config.h
--rw-r--r--   0        0        0     3166 2020-02-02 00:00:00.000000 siru-0.6/tests/ruwaq/template/src/config.c
--rw-r--r--   0        0        0     4676 2020-02-02 00:00:00.000000 siru-0.6/.gitignore
--rw-r--r--   0        0        0     1305 2020-02-02 00:00:00.000000 siru-0.6/LICENSE.txt
--rw-r--r--   0        0        0     1215 2020-02-02 00:00:00.000000 siru-0.6/README.md
--rw-r--r--   0        0        0     1988 2020-02-02 00:00:00.000000 siru-0.6/pyproject.toml
--rw-r--r--   0        0        0     2369 2020-02-02 00:00:00.000000 siru-0.6/PKG-INFO
+-rw-r--r--   0        0        0      424 2020-02-02 00:00:00.000000 siru-0.7/.clang-format
+-rw-r--r--   0        0        0      668 2020-02-02 00:00:00.000000 siru-0.7/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     3605 2020-02-02 00:00:00.000000 siru-0.7/prueba.py
+-rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 siru-0.7/.github/workflows/pre-commit.yml
+-rw-r--r--   0        0        0      746 2020-02-02 00:00:00.000000 siru-0.7/.vscode/settings.json
+-rw-r--r--   0        0        0    10870 2020-02-02 00:00:00.000000 siru-0.7/doc/protocolo.md
+-rw-r--r--   0        0        0     1695 2020-02-02 00:00:00.000000 siru-0.7/src/siru/__about__.py
+-rw-r--r--   0        0        0     1674 2020-02-02 00:00:00.000000 siru-0.7/src/siru/__init__.py
+-rw-r--r--   0        0        0     3780 2020-02-02 00:00:00.000000 siru-0.7/src/siru/ate.py
+-rw-r--r--   0        0        0     3893 2020-02-02 00:00:00.000000 siru-0.7/src/siru/dut.py
+-rw-r--r--   0        0        0     4810 2020-02-02 00:00:00.000000 siru-0.7/src/siru/gpio.py
+-rwxr-xr-x   0        0        0     6549 2020-02-02 00:00:00.000000 siru-0.7/src/siru/preat.py
+-rw-r--r--   0        0        0     9030 2020-02-02 00:00:00.000000 siru-0.7/src/siru/tasks.py
+-rw-r--r--   0        0        0     1674 2020-02-02 00:00:00.000000 siru-0.7/tests/__init__.py
+-rw-r--r--   0        0        0     4061 2020-02-02 00:00:00.000000 siru-0.7/tests/test_ate.py
+-rw-r--r--   0        0        0     3376 2020-02-02 00:00:00.000000 siru-0.7/tests/test_dut.py
+-rw-r--r--   0        0        0     9068 2020-02-02 00:00:00.000000 siru-0.7/tests/test_gpio.py
+-rw-r--r--   0        0        0     8902 2020-02-02 00:00:00.000000 siru-0.7/tests/test_preat.py
+-rw-r--r--   0        0        0     8999 2020-02-02 00:00:00.000000 siru-0.7/tests/test_tasks.py
+-rw-r--r--   0        0        0     2098 2020-02-02 00:00:00.000000 siru-0.7/tests/utils.py
+-rw-r--r--   0        0        0      589 2020-02-02 00:00:00.000000 siru-0.7/tests/data/ate_test.yaml
+-rw-r--r--   0        0        0      605 2020-02-02 00:00:00.000000 siru-0.7/tests/data/dut_test.yaml
+-rw-r--r--   0        0        0      854 2020-02-02 00:00:00.000000 siru-0.7/tests/data/tasks_test.yaml
+-rw-r--r--   0        0        0     2863 2020-02-02 00:00:00.000000 siru-0.7/tests/ruwaq/expected/inc/config.h
+-rw-r--r--   0        0        0     3469 2020-02-02 00:00:00.000000 siru-0.7/tests/ruwaq/expected/src/config.c
+-rw-r--r--   0        0        0     2908 2020-02-02 00:00:00.000000 siru-0.7/tests/ruwaq/template/inc/config.h
+-rw-r--r--   0        0        0     3166 2020-02-02 00:00:00.000000 siru-0.7/tests/ruwaq/template/src/config.c
+-rw-r--r--   0        0        0     4676 2020-02-02 00:00:00.000000 siru-0.7/.gitignore
+-rw-r--r--   0        0        0     1305 2020-02-02 00:00:00.000000 siru-0.7/LICENSE.txt
+-rw-r--r--   0        0        0     1215 2020-02-02 00:00:00.000000 siru-0.7/README.md
+-rw-r--r--   0        0        0     1988 2020-02-02 00:00:00.000000 siru-0.7/pyproject.toml
+-rw-r--r--   0        0        0     2369 2020-02-02 00:00:00.000000 siru-0.7/PKG-INFO
```

### Comparing `siru-0.6/.pre-commit-config.yaml` & `siru-0.7/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `siru-0.6/prueba.py` & `siru-0.7/prueba.py`

 * *Files identical despite different names*

### Comparing `siru-0.6/.vscode/settings.json` & `siru-0.7/.vscode/settings.json`

 * *Files identical despite different names*

### Comparing `siru-0.6/doc/protocolo.md` & `siru-0.7/doc/protocolo.md`

 * *Files identical despite different names*

### Comparing `siru-0.6/src/siru/__about__.py` & `siru-0.7/src/siru/__about__.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,8 +23,8 @@
 # OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN
 # CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
 #
 # SPDX-License-Identifier: MIT
 # SPDX-FileCopyrightText: 2023, Esteban Volentini <evolentini@herrera.unt.edu.ar>
 ##################################################################################################
 
-__version__ = "0.6"
+__version__ = "0.7"
```

### Comparing `siru-0.6/src/siru/__init__.py` & `siru-0.7/src/siru/__init__.py`

 * *Files identical despite different names*

### Comparing `siru-0.6/src/siru/ate.py` & `siru-0.7/src/siru/ate.py`

 * *Files identical despite different names*

### Comparing `siru-0.6/src/siru/dut.py` & `siru-0.7/src/siru/dut.py`

 * *Files identical despite different names*

### Comparing `siru-0.6/src/siru/gpio.py` & `siru-0.7/src/siru/gpio.py`

 * *Files identical despite different names*

### Comparing `siru-0.6/src/siru/preat.py` & `siru-0.7/src/siru/preat.py`

 * *Files identical despite different names*

### Comparing `siru-0.6/src/siru/tasks.py` & `siru-0.7/src/siru/tasks.py`

 * *Files 4% similar despite different names*

```diff
@@ -75,16 +75,18 @@
         path = Path(self.project.path, Template(filename).render(job=self))
         return str(path.resolve().absolute())
 
     def relpath(self, filename: str) -> str:
         path = Path(self.project.path, Template(filename).render(job=self))
         return str(path.relative_to(self.project.path))
 
-    def render(self) -> str:
-        first_pass = Template(self.template).render(job=self)
+    def render(self, template=None) -> str:
+        if not template:
+            template = self.template
+        first_pass = Template(template).render(job=self)
         return Template(first_pass).render(job=self)
 
     def log_start_process(self, command: str):
         if self.verbose:
             process = self.__class__.__name__
             header = f"=== Inicio del proceso {process} ---" + 60 * "-"
             print(f"{header:80}\n{command}")
@@ -93,18 +95,18 @@
         if self.verbose:
             process = self.__class__.__name__
             header = f"=== Salida del proceso {process} ---" + 60 * "-"
             print(f"{header:80}\n{result[0]}")
             header = f"=== Errores del proceso {process} --" + 60 * "-"
             print(f"{header:80}\n{result[1]}")
 
-    def open_process(self):
+    def open_process(self, template=None):
         if self.on_execute:
             self.on_execute(self)
-        command = self.render()
+        command = self.render(template=template)
         self.log_start_process(command)
         return subprocess.Popen(
             command,
             cwd=self.abspath(self.project.path),
             stdout=subprocess.PIPE,
             stderr=subprocess.PIPE,
             encoding="utf-8",
@@ -133,14 +135,15 @@
     COMMAND = "openocd"
     TEMPLATE = '${job.command} -f ${job.config} -c "gdb_port ${job.port}"'
 
     def __init__(self, project: Project, environ: Dict, **kwargs) -> None:
         super().__init__(project=project, environ=environ, **kwargs)
         self.config = kwargs.get("config", "")
         self.port = int(kwargs.get("port", "3333"))
+        self.reset = kwargs.get("reset", "")
 
 
 class Debugger(Job):
     COMMAND = "gdb"
     TEMPLATE = '${job.command} -f ${job.binary} -ex "${job.execute}"'
 
     def __init__(self, project: Project, environ: Dict, **kwargs) -> None:
@@ -252,18 +255,19 @@
         commands = [
             "load",
             "monitor reset run",
         ]
         return self.debug(commands)
 
     def restart(self):
-        commands = [
-            "monitor reset run",
-        ]
-        return self.debug(commands)
+        monitor = self.monitor.open_process(template=self.monitor.reset)
+        result = monitor.communicate()
+        self.monitor.log_end_process(result)
+
+        return monitor.returncode == 0
 
     def flash(self):
         flasher = self.flasher.open_process()
         result = flasher.communicate()
         self.flasher.log_end_process(result)
 
         return flasher.returncode == 0
```

### Comparing `siru-0.6/tests/__init__.py` & `siru-0.7/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `siru-0.6/tests/test_ate.py` & `siru-0.7/tests/test_ate.py`

 * *Files identical despite different names*

### Comparing `siru-0.6/tests/test_dut.py` & `siru-0.7/tests/test_dut.py`

 * *Files identical despite different names*

### Comparing `siru-0.6/tests/test_gpio.py` & `siru-0.7/tests/test_gpio.py`

 * *Files identical despite different names*

### Comparing `siru-0.6/tests/test_preat.py` & `siru-0.7/tests/test_preat.py`

 * *Files 5% similar despite different names*

```diff
@@ -25,14 +25,16 @@
 #
 # SPDX-License-Identifier: MIT
 # SPDX-FileCopyrightText: 2023, Esteban Volentini <evolentini@herrera.unt.edu.ar>
 ##################################################################################################
 
 import pytest
 from serial import Serial
+from serial.tools import list_ports
+from serial.tools.list_ports_common import ListPortInfo
 from pytest_mock import MockerFixture
 from siru.preat import Preat, Parameter, Result
 
 EXECUTE_OUTPUT_SINGLE_PARAM = b"\x07\x01\x01\x10\x01\xb5\xa3"
 EXECUTE_ASSERT = b"\x11\x00\x54\x33\x00\x00\x00\x64\x00\x00\x13\x88\x11\x01\x00\xCD\x2C"
 EXECUTE_INPUT_SINGLE_PARAM = b"\x07\x01\x51\x10\x03\xB1\xFA"
 
@@ -67,14 +69,15 @@
 
 @pytest.fixture(autouse=True)
 def mock_serial_port_init(mocker):
     mocker.init = mocker.patch.object(Serial, "__init__", return_value=None)
     mocker.write = mocker.patch.object(Serial, "write", return_value=None)
     mocker.read = mocker.patch.object(Serial, "read")
     mocker.timeout = mocker.patch.object(Serial, "timeout")
+    mocker.port_list = mocker.patch("serial.tools.list_ports.comports")
 
 
 def test_execute_command(mocker: MockerFixture):
     mocker.read.side_effect = [ACK_NO_ERROR[:1], ACK_NO_ERROR[1:]]
 
     preat = Preat("/dev/tty.USB")
     result = preat.execute(0x010, [Parameter(Parameter.Type.UINT8, 0x01)])
@@ -229,7 +232,15 @@
     assert preat.url == "/dev/tty.USB_DEVICE"
 
     mocker.init.reset_mock()
     mocker.read.return_value = None
     result = preat.execute(0x010, [Parameter(Parameter.Type.UINT8, 0x01)])
     mocker.init.assert_called_once_with(port="/dev/tty.USB_DEVICE", baudrate=115200)
     assert result == Result.RESPONSE_TIMEOUT
+
+
+def test_use_usb_location_to_server(mocker: MockerFixture):
+    port = ListPortInfo(device="/dev/tty.USB_DEVICE")
+    port.location = "1-2.3"
+    preat = Preat(f"usb://{port.location}")
+    mocker.port_list.return_value = [port]
+    assert preat.serial_url == port.device
```

### Comparing `siru-0.6/tests/test_tasks.py` & `siru-0.7/tests/test_tasks.py`

 * *Files 4% similar despite different names*

```diff
@@ -101,14 +101,15 @@
     assert tasks.builder.clean == "clean"
     assert tasks.builder.build == "all"
     assert tasks.builder.template == "${job.command} ${job.action}"
 
     assert tasks.monitor.command == "openocd"
     assert tasks.monitor.config == ""
     assert tasks.monitor.port == 3333
+    assert tasks.monitor.reset == ""
     assert (
         tasks.monitor.template
         == '${job.command} -f ${job.config} -c "gdb_port ${job.port}"'
     )
 
     assert tasks.debugger.command == "gdb"
     assert tasks.debugger.execute == ""
@@ -141,14 +142,19 @@
     assert tasks.builder.render() == "/usr/bin/make  MUJU=/home/test/muju"
 
     assert (
         tasks.monitor.render()
         == '/usr/bin/openocd -c "gdb_port 8888" -f '
         + local_path("/home/test/project/openocd/config.file")
     )
+    assert tasks.monitor.render(
+        tasks.monitor.reset
+    ) == '/usr/bin/openocd -c "init" -c "reset run" -c "shutdown" -f ' + local_path(
+        "/home/test/project/openocd/config.file"
+    )
 
     assert (
         tasks.debugger.render()
         == "arm-none-eabi-gdb "
         + local_path("/home/test/project/build/bin/project.elf")
         + ' --ex "target extended-remote localhost:8888"'
     )
@@ -193,14 +199,31 @@
     tasks = Tasks(project={"path": "/home/test"})
     tasks.clean()
     call = mock_open.open.call_args
     assert call.args[0] == "make clean"
     assert str(call.kwargs["cwd"]) == local_path("/home/test")
 
 
+def test_monitor_reset(mock_open):
+    tasks = Tasks(
+        project={"path": "/home/test"},
+        monitor={"config": "config.cfg"},
+    )
+    tasks.write()
+    # assert mock_open.open.call_count == 2
+
+    # call = mock_open.open.call_args_list[0]
+    # assert call.args[0] == 'openocd -f config.cfg -c "gdb_port 3333"'
+    # assert str(call.kwargs["cwd"]) == local_path("/home/test")
+
+    # call = mock_open.open.call_args_list[1]
+    # assert call.args[0] == 'gdb -f project.elf -ex "target remote"'
+    # assert str(call.kwargs["cwd"]) == local_path("/home/test")
+
+
 def test_tasks_builder_debugger_write(mock_open):
     tasks = Tasks(
         project={"path": "/home/test"},
         monitor={"config": "config.cfg"},
         debugger={"execute": "target remote"},
     )
     tasks.write()
@@ -214,26 +237,26 @@
     assert call.args[0] == 'gdb -f project.elf -ex "target remote"'
     assert str(call.kwargs["cwd"]) == local_path("/home/test")
 
 
 def test_tasks_builder_debugger_restart(mock_open):
     tasks = Tasks(
         project={"path": "/home/test"},
-        monitor={"config": "config.cfg"},
-        debugger={"execute": "target remote"},
+        monitor={
+            "config": "config.cfg",
+            "reset": '${job.command} -c "init" -c "reset run" -c "shutdown" -f ${job.config}',
+        },
     )
     tasks.restart()
-    assert mock_open.open.call_count == 2
+    assert mock_open.open.call_count == 1
 
     call = mock_open.open.call_args_list[0]
-    assert call.args[0] == 'openocd -f config.cfg -c "gdb_port 3333"'
-    assert str(call.kwargs["cwd"]) == local_path("/home/test")
-
-    call = mock_open.open.call_args_list[1]
-    assert call.args[0] == 'gdb -f project.elf -ex "target remote"'
+    assert (
+        call.args[0] == 'openocd -c "init" -c "reset run" -c "shutdown" -f config.cfg'
+    )
     assert str(call.kwargs["cwd"]) == local_path("/home/test")
 
 
 def test_tasks_flasher(mock_open):
     tasks = Tasks(
         project={"path": "/home/test"},
         flasher={"config": "config.cfg"},
```

### Comparing `siru-0.6/tests/utils.py` & `siru-0.7/tests/utils.py`

 * *Files identical despite different names*

### Comparing `siru-0.6/tests/data/ate_test.yaml` & `siru-0.7/tests/data/ate_test.yaml`

 * *Files identical despite different names*

### Comparing `siru-0.6/tests/data/dut_test.yaml` & `siru-0.7/tests/data/dut_test.yaml`

 * *Files identical despite different names*

### Comparing `siru-0.6/tests/data/tasks_test.yaml` & `siru-0.7/tests/data/tasks_test.yaml`

 * *Files 12% similar despite different names*

```diff
@@ -13,14 +13,15 @@
   template: ${job.command} ${job.action} MUJU=${job.environ["MUJU"]}
 
 monitor:
   command: /usr/bin/openocd
   config: ${job.abspath("openocd/config.file")}
   port: 8888
   template: ${job.command} -c "gdb_port ${job.port}" -f ${job.config}
+  reset: ${job.command} -c "init" -c "reset run" -c "shutdown" -f ${job.config}
 
 debugger:
   command: arm-none-eabi-gdb
   execute: target extended-remote localhost:${job.monitor.port}
   template: ${job.command} ${job.abspath(job.project.binary)} --ex "${job.execute}"
 
 flasher:
```

### Comparing `siru-0.6/tests/ruwaq/expected/inc/config.h` & `siru-0.7/tests/ruwaq/expected/inc/config.h`

 * *Files identical despite different names*

### Comparing `siru-0.6/tests/ruwaq/expected/src/config.c` & `siru-0.7/tests/ruwaq/expected/src/config.c`

 * *Files identical despite different names*

### Comparing `siru-0.6/tests/ruwaq/template/inc/config.h` & `siru-0.7/tests/ruwaq/template/inc/config.h`

 * *Files identical despite different names*

### Comparing `siru-0.6/tests/ruwaq/template/src/config.c` & `siru-0.7/tests/ruwaq/template/src/config.c`

 * *Files identical despite different names*

### Comparing `siru-0.6/.gitignore` & `siru-0.7/.gitignore`

 * *Files identical despite different names*

### Comparing `siru-0.6/LICENSE.txt` & `siru-0.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `siru-0.6/README.md` & `siru-0.7/README.md`

 * *Files identical despite different names*

### Comparing `siru-0.6/pyproject.toml` & `siru-0.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `siru-0.6/PKG-INFO` & `siru-0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: siru
-Version: 0.6
+Version: 0.7
 Summary: Automated tests on hardware for embedded systems
 Project-URL: Documentation, https://github.com/labmicro/siru#readme
 Project-URL: Issues, https://github.com/labmicro/siru/issues
 Project-URL: Source, https://github.com/labmicro/siru
 Author-email: Esteban Volentini <evolentini@herrera.unt.edu.ar>
 License-Expression: MIT
 License-File: LICENSE.txt
```

