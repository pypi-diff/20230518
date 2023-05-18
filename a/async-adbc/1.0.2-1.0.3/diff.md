# Comparing `tmp/async_adbc-1.0.2.tar.gz` & `tmp/async_adbc-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "async_adbc-1.0.2.tar", max compression
+gzip compressed data, was "async_adbc-1.0.3.tar", max compression
```

## Comparing `async_adbc-1.0.2.tar` & `async_adbc-1.0.3.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0       70 2023-05-16 06:58:01.167502 async_adbc-1.0.2/async_adbc/__init__.py
--rw-r--r--   0        0        0      998 2023-05-16 06:58:27.465793 async_adbc-1.0.2/async_adbc/adbclient.py
--rw-r--r--   0        0        0     2983 2023-05-16 06:52:10.041298 async_adbc-1.0.2/async_adbc/device.py
--rw-r--r--   0        0        0      601 2023-05-16 06:51:45.869292 async_adbc-1.0.2/async_adbc/plugins/__init__.py
--rw-r--r--   0        0        0      502 2023-05-16 02:17:28.058635 async_adbc-1.0.2/async_adbc/plugins/am.py
--rw-r--r--   0        0        0     2657 2023-05-16 02:32:10.948830 async_adbc-1.0.2/async_adbc/plugins/battery.py
--rw-r--r--   0        0        0    12259 2023-05-16 06:51:45.908294 async_adbc-1.0.2/async_adbc/plugins/cpu.py
--rw-r--r--   0        0        0     1242 2023-05-16 06:51:45.797292 async_adbc-1.0.2/async_adbc/plugins/forward.py
--rw-r--r--   0        0        0     3933 2023-05-16 02:51:02.455214 async_adbc-1.0.2/async_adbc/plugins/fps.py
--rw-r--r--   0        0        0      614 2023-05-15 12:07:09.349059 async_adbc-1.0.2/async_adbc/plugins/gpu.py
--rw-r--r--   0        0        0      393 2023-05-15 12:13:38.890420 async_adbc-1.0.2/async_adbc/plugins/input.py
--rw-r--r--   0        0        0      895 2023-05-16 03:18:01.857216 async_adbc-1.0.2/async_adbc/plugins/logcat.py
--rw-r--r--   0        0        0     2209 2023-05-16 03:26:42.422860 async_adbc-1.0.2/async_adbc/plugins/mem.py
--rw-r--r--   0        0        0     5597 2023-05-16 06:51:45.819291 async_adbc-1.0.2/async_adbc/plugins/pm.py
--rw-r--r--   0        0        0      510 2023-05-15 11:29:29.910308 async_adbc-1.0.2/async_adbc/plugins/prop.py
--rw-r--r--   0        0        0     4615 2023-05-16 04:20:29.957697 async_adbc-1.0.2/async_adbc/plugins/temp.py
--rw-r--r--   0        0        0     2216 2023-05-16 06:51:45.868298 async_adbc-1.0.2/async_adbc/plugins/traffic.py
--rw-r--r--   0        0        0      807 2023-05-15 11:29:32.496380 async_adbc-1.0.2/async_adbc/plugins/utils.py
--rw-r--r--   0        0        0     4481 2023-05-16 07:19:17.701385 async_adbc-1.0.2/async_adbc/protocol.py
--rw-r--r--   0        0        0      796 2023-05-16 06:51:45.874292 async_adbc-1.0.2/async_adbc/service/__init__.py
--rw-r--r--   0        0        0    10228 2023-05-16 06:51:45.939291 async_adbc-1.0.2/async_adbc/service/host.py
--rw-r--r--   0        0        0    10086 2023-05-16 06:51:45.937291 async_adbc-1.0.2/async_adbc/service/local.py
--rw-r--r--   0        0        0     1090 2023-05-16 05:23:42.403245 async_adbc-1.0.2/LICENSE
--rw-r--r--   0        0        0      482 2023-05-16 07:19:30.857945 async_adbc-1.0.2/pyproject.toml
--rw-r--r--   0        0        0      423 2023-05-15 02:24:29.723099 async_adbc-1.0.2/README.md
--rw-r--r--   0        0        0      849 1970-01-01 00:00:00.000000 async_adbc-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0       70 2023-05-16 06:58:01.167502 async_adbc-1.0.3/async_adbc/__init__.py
+-rw-r--r--   0        0        0      998 2023-05-16 06:58:27.465793 async_adbc-1.0.3/async_adbc/adbclient.py
+-rw-r--r--   0        0        0     2983 2023-05-16 06:52:10.041298 async_adbc-1.0.3/async_adbc/device.py
+-rw-r--r--   0        0        0      601 2023-05-16 06:51:45.869292 async_adbc-1.0.3/async_adbc/plugins/__init__.py
+-rw-r--r--   0        0        0      411 2023-05-18 06:55:18.876102 async_adbc-1.0.3/async_adbc/plugins/am.py
+-rw-r--r--   0        0        0     2657 2023-05-16 02:32:10.948830 async_adbc-1.0.3/async_adbc/plugins/battery.py
+-rw-r--r--   0        0        0    11855 2023-05-18 06:56:11.752165 async_adbc-1.0.3/async_adbc/plugins/cpu.py
+-rw-r--r--   0        0        0     1242 2023-05-16 06:51:45.797292 async_adbc-1.0.3/async_adbc/plugins/forward.py
+-rw-r--r--   0        0        0     3933 2023-05-16 02:51:02.455214 async_adbc-1.0.3/async_adbc/plugins/fps.py
+-rw-r--r--   0        0        0      614 2023-05-15 12:07:09.349059 async_adbc-1.0.3/async_adbc/plugins/gpu.py
+-rw-r--r--   0        0        0      393 2023-05-15 12:13:38.890420 async_adbc-1.0.3/async_adbc/plugins/input.py
+-rw-r--r--   0        0        0      895 2023-05-16 03:18:01.857216 async_adbc-1.0.3/async_adbc/plugins/logcat.py
+-rw-r--r--   0        0        0     2209 2023-05-16 03:26:42.422860 async_adbc-1.0.3/async_adbc/plugins/mem.py
+-rw-r--r--   0        0        0     5597 2023-05-16 06:51:45.819291 async_adbc-1.0.3/async_adbc/plugins/pm.py
+-rw-r--r--   0        0        0      510 2023-05-15 11:29:29.910308 async_adbc-1.0.3/async_adbc/plugins/prop.py
+-rw-r--r--   0        0        0     4615 2023-05-16 04:20:29.957697 async_adbc-1.0.3/async_adbc/plugins/temp.py
+-rw-r--r--   0        0        0     2216 2023-05-16 06:51:45.868298 async_adbc-1.0.3/async_adbc/plugins/traffic.py
+-rw-r--r--   0        0        0      807 2023-05-15 11:29:32.496380 async_adbc-1.0.3/async_adbc/plugins/utils.py
+-rw-r--r--   0        0        0     4481 2023-05-16 07:19:17.701385 async_adbc-1.0.3/async_adbc/protocol.py
+-rw-r--r--   0        0        0      796 2023-05-16 06:51:45.874292 async_adbc-1.0.3/async_adbc/service/__init__.py
+-rw-r--r--   0        0        0    10228 2023-05-16 06:51:45.939291 async_adbc-1.0.3/async_adbc/service/host.py
+-rw-r--r--   0        0        0    10086 2023-05-16 06:51:45.937291 async_adbc-1.0.3/async_adbc/service/local.py
+-rw-r--r--   0        0        0     1090 2023-05-16 05:23:42.403245 async_adbc-1.0.3/LICENSE
+-rw-r--r--   0        0        0      482 2023-05-18 06:58:53.309785 async_adbc-1.0.3/pyproject.toml
+-rw-r--r--   0        0        0      423 2023-05-15 02:24:29.723099 async_adbc-1.0.3/README.md
+-rw-r--r--   0        0        0      849 1970-01-01 00:00:00.000000 async_adbc-1.0.3/PKG-INFO
```

### Comparing `async_adbc-1.0.2/async_adbc/adbclient.py` & `async_adbc-1.0.3/async_adbc/adbclient.py`

 * *Files identical despite different names*

### Comparing `async_adbc-1.0.2/async_adbc/device.py` & `async_adbc-1.0.3/async_adbc/device.py`

 * *Files identical despite different names*

### Comparing `async_adbc-1.0.2/async_adbc/plugins/__init__.py` & `async_adbc-1.0.3/async_adbc/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `async_adbc-1.0.2/async_adbc/plugins/battery.py` & `async_adbc-1.0.3/async_adbc/plugins/battery.py`

 * *Files identical despite different names*

### Comparing `async_adbc-1.0.2/async_adbc/plugins/cpu.py` & `async_adbc-1.0.3/async_adbc/plugins/cpu.py`

 * *Files 4% similar despite different names*

```diff
@@ -156,17 +156,14 @@
     def total(self) -> float:
         return self.utime + self.stime
 
 
 class CPUPlugin(Plugin):
     def __init__(self, device: "Device") -> None:
         super().__init__(device)
-        self._last_cpu_stat: Optional[CPUStatMap] = {}
-        self._last_total_cpu_stat: Optional[CPUStat] = CPUStat()
-        self._last_pid_cpu_stat: Optional[ProcessCPUStat] = ProcessCPUStat()
 
     @property
     async def count(self) -> int:
         """
         获取cpu核心数
 
         因为核心数是一定的，为了避免每次都重复请求做了缓存
@@ -264,24 +261,24 @@
 
         Returns:
             CPUUsageMap: _description_
         """
         normalize_factor = await self.normalize_factor
         cpu_count = await self.count
         cpu_usage = {i: CPUUsage() for i in range(cpu_count)}
-        if not self._last_cpu_stat:
-            self._last_cpu_stat = await self.cpu_stats
-        else:
-            cpu_state = await self.cpu_stats
-            for index, state in cpu_state.items():
-                last_cpu_state = self._last_cpu_stat[index]
-                cpu_diff: CPUStat = state - last_cpu_state
-                usage = round(cpu_diff.usage, 2)
-                normalized = usage * normalize_factor
-                cpu_usage[index] = CPUUsage(usage, normalized)
+
+        last_cpu_stats = await self.cpu_stats
+        await asyncio.sleep(1)
+        cpu_stats = await self.cpu_stats
+        for index, stat in cpu_stats.items():
+            last_cpu_stat = last_cpu_stats[index]
+            cpu_diff: CPUStat = stat - last_cpu_stat
+            usage = round(cpu_diff.usage, 2)
+            normalized = usage * normalize_factor
+            cpu_usage[index] = CPUUsage(usage, normalized)
         return cpu_usage
 
     @property
     async def total_cpu_stat(self) -> CPUStat:
         """
         _summary_
 
@@ -313,22 +310,22 @@
 
         Args:
             normalized (bool, optional): 标准化占有率. Defaults to False.
 
         Returns:
             CPUUsage: CPU使用率
         """
-        if self._last_total_cpu_stat is None:
-            self._last_total_cpu_stat = await self.total_cpu_stat
-            return CPUUsage()
 
-        total_cpu_stat = await self.total_cpu_stat
-        diff = total_cpu_stat - self._last_total_cpu_stat
+        last_total_cpu_stat = await self.total_cpu_stat
 
-        self._last_total_cpu_stat = total_cpu_stat
+        # 用sleep来间隔采样
+        await asyncio.sleep(1)
+
+        total_cpu_stat = await self.total_cpu_stat
+        diff = total_cpu_stat - last_total_cpu_stat
 
         usage = round(diff.usage, 2)
         normalize_factor = await self.normalize_factor
         normalized = usage * normalize_factor
 
         return CPUUsage(usage, normalized)
 
@@ -337,40 +334,38 @@
 
         Args:
             pid (int): 进程pid
 
         Returns:
             ProcessCPUStat: 进程cpu状态
         """
-        result = await self._device.shell("cat /proc/{}/stat".format(pid))
+        result = await self._device.shell(f"cat /proc/{pid}/stat")
 
         if "No such file or directory" in result:
             return ProcessCPUStat("", 0, 0)
         else:
             items = result.split()
             return ProcessCPUStat(items[1], int(items[13]), int(items[14]))
 
     async def get_pid_cpu_usage(self, pid: int) -> CPUUsage:
-        if self._last_pid_cpu_stat is None:
-            self._last_pid_cpu_stat = await self.get_pid_cpu_stat(pid)
-            return CPUUsage()
-
+        normalize_factor = await self.normalize_factor
+        
+        last_pid_cpu_stat = await self.get_pid_cpu_stat(pid)
+        last_total_cpu_stat = await self.total_cpu_stat
+        await asyncio.sleep(1)
         pid_stat = await self.get_pid_cpu_stat(pid)
-        pid_diff = pid_stat - self._last_pid_cpu_stat
+        pid_diff = pid_stat - last_pid_cpu_stat
 
         total_cpu_stat = await self.total_cpu_stat
-        cpu_diff = total_cpu_stat - self._last_total_cpu_stat
-        self._last_total_cpu_stat = total_cpu_stat
+        cpu_diff = total_cpu_stat - last_total_cpu_stat
 
         app_cpu_usage = pid_diff.total / cpu_diff.total * 100
         app_cpu_usage = round(app_cpu_usage, 2)
 
-        normalize_factor = await self.normalize_factor
         normalized = app_cpu_usage * normalize_factor
-
         return CPUUsage(app_cpu_usage, normalized)
 
     @property
     async def cpu_name(self) -> str:
         """
         获取CPU名
```

### Comparing `async_adbc-1.0.2/async_adbc/plugins/forward.py` & `async_adbc-1.0.3/async_adbc/plugins/forward.py`

 * *Files identical despite different names*

### Comparing `async_adbc-1.0.2/async_adbc/plugins/fps.py` & `async_adbc-1.0.3/async_adbc/plugins/fps.py`

 * *Files identical despite different names*

### Comparing `async_adbc-1.0.2/async_adbc/plugins/gpu.py` & `async_adbc-1.0.3/async_adbc/plugins/gpu.py`

 * *Files identical despite different names*

### Comparing `async_adbc-1.0.2/async_adbc/plugins/logcat.py` & `async_adbc-1.0.3/async_adbc/plugins/logcat.py`

 * *Files identical despite different names*

### Comparing `async_adbc-1.0.2/async_adbc/plugins/mem.py` & `async_adbc-1.0.3/async_adbc/plugins/mem.py`

 * *Files identical despite different names*

### Comparing `async_adbc-1.0.2/async_adbc/plugins/pm.py` & `async_adbc-1.0.3/async_adbc/plugins/pm.py`

 * *Files identical despite different names*

### Comparing `async_adbc-1.0.2/async_adbc/plugins/temp.py` & `async_adbc-1.0.3/async_adbc/plugins/temp.py`

 * *Files identical despite different names*

### Comparing `async_adbc-1.0.2/async_adbc/plugins/traffic.py` & `async_adbc-1.0.3/async_adbc/plugins/traffic.py`

 * *Files identical despite different names*

### Comparing `async_adbc-1.0.2/async_adbc/plugins/utils.py` & `async_adbc-1.0.3/async_adbc/plugins/utils.py`

 * *Files identical despite different names*

### Comparing `async_adbc-1.0.2/async_adbc/protocol.py` & `async_adbc-1.0.3/async_adbc/protocol.py`

 * *Files identical despite different names*

### Comparing `async_adbc-1.0.2/async_adbc/service/__init__.py` & `async_adbc-1.0.3/async_adbc/service/__init__.py`

 * *Files identical despite different names*

### Comparing `async_adbc-1.0.2/async_adbc/service/host.py` & `async_adbc-1.0.3/async_adbc/service/host.py`

 * *Files identical despite different names*

### Comparing `async_adbc-1.0.2/async_adbc/service/local.py` & `async_adbc-1.0.3/async_adbc/service/local.py`

 * *Files identical despite different names*

### Comparing `async_adbc-1.0.2/LICENSE` & `async_adbc-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `async_adbc-1.0.2/PKG-INFO` & `async_adbc-1.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: async-adbc
-Version: 1.0.2
+Version: 1.0.3
 Summary: 
 Author: kaluluosi
 Author-email: kaluluosi@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

