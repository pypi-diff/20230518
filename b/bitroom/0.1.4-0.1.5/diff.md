# Comparing `tmp/bitroom-0.1.4.tar.gz` & `tmp/bitroom-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bitroom-0.1.4.tar", last modified: Sun May  7 11:38:00 2023, max compression
+gzip compressed data, was "bitroom-0.1.5.tar", last modified: Thu May 18 01:52:32 2023, max compression
```

## Comparing `bitroom-0.1.4.tar` & `bitroom-0.1.5.tar`

### file list

```diff
@@ -1,12 +1,14 @@
--rw-r--r--   0        0        0     1063 2023-05-07 11:37:45.595288 bitroom-0.1.4/LICENSE
--rw-r--r--   0        0        0     4160 2023-05-07 11:37:45.595288 bitroom-0.1.4/README.md
--rw-r--r--   0        0        0     1408 2023-05-07 11:38:00.619281 bitroom-0.1.4/pyproject.toml
--rw-r--r--   0        0        0      100 2023-05-07 11:37:45.595288 bitroom-0.1.4/src/bitroom/__init__.py
--rw-r--r--   0        0        0       28 2023-05-07 11:37:45.595288 bitroom-0.1.4/src/bitroom/__main__.py
--rw-r--r--   0        0        0       43 2023-05-07 11:37:45.595288 bitroom-0.1.4/src/bitroom/auth/__init__.py
--rw-r--r--   0        0        0     2452 2023-05-07 11:37:45.595288 bitroom-0.1.4/src/bitroom/auth/auth.py
--rw-r--r--   0        0        0    18654 2023-05-07 11:37:45.595288 bitroom-0.1.4/src/bitroom/auth/encrypt_js.py
--rw-r--r--   0        0        0     2540 2023-05-07 11:37:45.595288 bitroom-0.1.4/src/bitroom/cli.py
--rw-r--r--   0        0        0     1642 2023-05-07 11:37:45.595288 bitroom-0.1.4/src/bitroom/config.py
--rw-r--r--   0        0        0    10664 2023-05-07 11:37:45.595288 bitroom-0.1.4/src/bitroom/room.py
--rw-r--r--   0        0        0     5263 1970-01-01 00:00:00.000000 bitroom-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1063 2023-05-18 01:52:14.750468 bitroom-0.1.5/LICENSE
+-rw-r--r--   0        0        0     5102 2023-05-18 01:52:14.750468 bitroom-0.1.5/README.md
+-rw-r--r--   0        0        0     1552 2023-05-18 01:52:32.042362 bitroom-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0      100 2023-05-18 01:52:14.750468 bitroom-0.1.5/src/bitroom/__init__.py
+-rw-r--r--   0        0        0       28 2023-05-18 01:52:14.750468 bitroom-0.1.5/src/bitroom/__main__.py
+-rw-r--r--   0        0        0       43 2023-05-18 01:52:14.750468 bitroom-0.1.5/src/bitroom/auth/__init__.py
+-rw-r--r--   0        0        0     2452 2023-05-18 01:52:14.750468 bitroom-0.1.5/src/bitroom/auth/auth.py
+-rw-r--r--   0        0        0    18654 2023-05-18 01:52:14.750468 bitroom-0.1.5/src/bitroom/auth/encrypt_js.py
+-rw-r--r--   0        0        0     2540 2023-05-18 01:52:14.750468 bitroom-0.1.5/src/bitroom/cli.py
+-rw-r--r--   0        0        0     1642 2023-05-18 01:52:14.750468 bitroom-0.1.5/src/bitroom/config.py
+-rw-r--r--   0        0        0    12970 2023-05-18 01:52:14.750468 bitroom-0.1.5/src/bitroom/room.py
+-rw-r--r--   0        0        0      348 2023-05-18 01:52:14.750468 bitroom-0.1.5/src/bitroom/tui.css
+-rw-r--r--   0        0        0     6259 2023-05-18 01:52:14.750468 bitroom-0.1.5/src/bitroom/tui.py
+-rw-r--r--   0        0        0     6353 1970-01-01 00:00:00.000000 bitroom-0.1.5/PKG-INFO
```

### Comparing `bitroom-0.1.4/LICENSE` & `bitroom-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `bitroom-0.1.4/README.md` & `bitroom-0.1.5/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -16,42 +16,60 @@
 
   例如，你可能会问：“明天下午还有没有房间？没有的话，后天下午也行。就几个人，也不需要投影。”
 
   而很少专门针对某一房间问。
 
 bitroom 目前已解决登录、包装 API 等底层问题，可供后来者调用。
 
+## 🧪 例子
+
+### 🤖编程 API
+
+这是主要支持的接口。
+
 ```python
 from datetime import date
 from httpx import AsyncClient
 from bitroom import auth, RoomAPI
 
 async with AsyncClient() as client:
     await auth(client, username, password)  # 登录“统一身份认证”
-
     api = await RoomAPI.build(client)
+
+    # 获取“可预约”的时空区间
     bookings = await api.fetch_bookings(date.today())
     print(bookings[0])
 
+    # 预约
     await api.book(
         bookings[0],
         tel="13806491023",
         applicant="Boltzmann",
         description="Boltzmann 常数是气体的内能与温度的一种比例系数。",
         remark="一般记作 k_B 或 k。",
     )
+
+    # 获取“已预约”的时空区间
+    orders = await api.fetch_orders(bookings[0].room_id, date.today())
+    print(orders[0])
 ```
 
-当然也提供了基础的命令行接口。可结合 [fzf](https://github.com/junegunn/fzf/)，搜索日期、时间、房间。
+### ⌨️命令行 CLI
+
+也提供了基础的命令行接口，支持查询，不支持预约。
+
+可结合 [fzf](https://github.com/junegunn/fzf/)，搜索日期、时间、房间。（详见 [wiki](https://github.com/YDX-2147483647/bitroom/wiki#-fzf-%E4%BD%BF%E7%94%A8%E7%A4%BA%E4%BE%8B)）
 
 ```shell
-bitroom show | fzf
+$ bitroom show | fzf
 ```
 
-## 🧪 例子
+![](https://user-images.githubusercontent.com/73375426/236676121-0bb3f80a-4ef0-4b06-bb03-d41a6f42fe38.png)
+
+详细帮助如下。
 
 （要先`pipx install bitroom`）
 
 ```shell
 $ bitroom --help
 Usage: python -m bitroom [OPTIONS] COMMAND [ARGS]...
 
@@ -96,16 +114,30 @@
 <Booking [甘棠社区-102春·事定（Multi-function Room）] 2023-05-05 21:00–22:00>
 <Booking [甘棠社区-102春·事定（Multi-function Room）] 2023-05-06 13:20–14:05>
 <Booking [甘棠社区-102春·事定（Multi-function Room）] 2023-05-06 14:10–14:55>
 <Booking [甘棠社区-102春·事定（Multi-function Room）] 2023-05-07 15:10–15:55>
 ……
 ```
 
+### 🎨图形终端 TUI
+
+目前还在早期测试阶段，仅仅能用而已。支持查询、搜索、预约。
+
+```shell
+$ pipx install bitroom[tui]
+```
+
+![RoomApp](https://github.com/YDX-2147483647/bitroom/assets/73375426/3ad4e0fd-dfb5-43ad-a07d-70b70b6242fa)
+
+![BookSceen](https://github.com/YDX-2147483647/bitroom/assets/73375426/18a824ce-f963-4f30-b0cb-b26a0f1583b2)
+
 ## ⚙️ 配置
 
+（仅用于 CLI、TUI）
+
 编辑`config.toml`，写入学号、密码，用于登录“统一身份认证”。
 
 ```toml
 # 仅作示例，非真实信息
 username = "1120771210"
 password = "cyberpunk"
 ```
```

### Comparing `bitroom-0.1.4/pyproject.toml` & `bitroom-0.1.5/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 [project]
 name = "bitroom"
-version = "0.1.4"
+version = "0.1.5"
 description = "BIT 场地预约查询接口（bitroom）"
 authors = [
     { name = "Y.D.X.", email = "73375426+YDX-2147483647@users.noreply.github.com" },
 ]
 dependencies = [
     "PyExecJS>=1.5.1",
     "httpx>=0.24.0",
     "click>=8.1.3",
     "platformdirs>=3.5.0",
     "tomli>=2.0.1; python_version < \"3.11\"",
+    "more-itertools>=9.1.0",
 ]
 requires-python = ">=3.10"
 readme = "README.md"
 classifiers = [
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3 :: Only",
     "Programming Language :: Python :: 3.10",
@@ -35,14 +36,20 @@
 Homepage = "https://github.com/YDX-2147483647/bitroom"
 Repository = "https://github.com/YDX-2147483647/bitroom"
 "Bug Tracker" = "https://github.com/YDX-2147483647/bitroom/issues"
 
 [project.scripts]
 bitroom = "bitroom.cli:cli"
 
+[project.optional-dependencies]
+tui = [
+    "rich>=13.3.5",
+    "textual>=0.23.0",
+]
+
 [build-system]
 requires = [
     "pdm-backend",
 ]
 build-backend = "pdm.backend"
 
 [tool.ruff]
@@ -53,11 +60,13 @@
     "I",
     "N",
 ]
 line-length = 88
 ignore-init-module-imports = true
 
 [tool.pdm.dev-dependencies]
-dev = []
+dev = [
+    "textual[dev]>=0.23.0",
+]
 
 [tool.pdm.scripts]
 lint = "pre-commit run --all-files"
```

### Comparing `bitroom-0.1.4/src/bitroom/auth/auth.py` & `bitroom-0.1.5/src/bitroom/auth/auth.py`

 * *Files identical despite different names*

### Comparing `bitroom-0.1.4/src/bitroom/auth/encrypt_js.py` & `bitroom-0.1.5/src/bitroom/auth/encrypt_js.py`

 * *Files identical despite different names*

### Comparing `bitroom-0.1.4/src/bitroom/cli.py` & `bitroom-0.1.5/src/bitroom/cli.py`

 * *Files identical despite different names*

### Comparing `bitroom-0.1.4/src/bitroom/config.py` & `bitroom-0.1.5/src/bitroom/config.py`

 * *Files identical despite different names*

### Comparing `bitroom-0.1.4/src/bitroom/room.py` & `bitroom-0.1.5/src/bitroom/room.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from dataclasses import asdict, dataclass
 from itertools import chain
 from json import dumps
 from math import ceil
 from typing import TYPE_CHECKING
 
 if TYPE_CHECKING:
-    from typing import Any, Generator, Mapping
+    from typing import Generator
 
     from httpx import AsyncClient, Response
 
 API_BASE = "http://stu.bit.edu.cn"
 
 
 async def prepare_headers(client: AsyncClient) -> None:
@@ -118,14 +118,33 @@
         for k, v in raw.items():
             if k.startswith("t_") and isinstance(v, str):
                 raw[k] = datetime.datetime.fromisoformat(v)
 
         return Booking(**raw)
 
 
+@dataclass
+class Order(Booking):
+    """已预约的时空区间"""
+
+    applicant: str
+    """预约人姓名"""
+    tel: str
+    """联系电话"""
+    description: str
+    """申请陈述"""
+
+    def __str__(self) -> str:
+        return (
+            f"<Order [{self.room_name}] "
+            f"{format_datetime_range((self.t_start,self.t_end))} "
+            f"“{self.applicant}” ({self.tel}): “{self.description}”>"
+        )
+
+
 class RoomAPI:
     """场地预约 API 包装
 
     ## 例子
 
     ```
     from datetime import date
@@ -150,20 +169,17 @@
     def __init__(self, client: AsyncClient) -> None:
         """
         请使用`build`。
         """
 
         self._client = client
 
-    async def _post(
-        self, url_path: str, data: Mapping[str, Any] | None = None, **kwargs
-    ) -> Response:
+    async def _post(self, url_path: str, **kwargs) -> Response:
         return await self._client.post(
             f"{API_BASE}{url_path}",
-            data={"data": dumps(data)},
             **kwargs,
         )
 
     async def _fetch_bookings_data(
         self, date: datetime.date, page: int, *, rooms_per_page: int
     ) -> dict:
         """Get a page of data
@@ -172,25 +188,31 @@
         :param rooms_per_page: 每页房间数量
         :return: 相邻一周（周一–周日）的预约情况
         """
 
         res = await self._post(
             "/xsfw/sys/cdyyapp/modules/CdyyApplyController/getSiteInfo.do",
             data={
-                # 预约日期
-                "YYRQ": date.isoformat(),
-                "pageNumber": page + 1,
-                "pageSize": rooms_per_page,
+                "data": dumps(
+                    {
+                        # 预约日期
+                        "YYRQ": date.isoformat(),
+                        "pageNumber": page + 1,
+                        "pageSize": rooms_per_page,
+                    }
+                )
             },
             timeout=max(20, 20 * rooms_per_page),  # Yes, it's really slow…
             follow_redirects=True,
         )
         res.raise_for_status()
         json = res.json()
-        assert json["code"] == "0" and json["msg"] == "成功"
+        assert (
+            json["code"] == "0" and json["msg"] == "成功"
+        ), f"Fetching bookings data failed with {json['code']} “{json['msg']}”."
 
         return json["data"]
 
     def _parse_bookings_data(
         self, data: dict, *, dates: list[datetime.date]
     ) -> Generator[Booking, None, None]:
         """Parse a page of data to bookings
@@ -322,39 +344,83 @@
             and b.t_start.date() == bookings[0].t_start.date()
             for b in bookings
         ), f"预约必须不是同一天、同一房间，请分多次预约：{bookings}"
 
         res = await self._post(
             "/xsfw/sys/cdyyapp/modules/CdyyApplyController/saveReserveSite.do",
             data={
-                # 场地代码-显示
-                "CDDM_DISPLAY": bookings[0].room_name,
-                # 场地代码
-                "CDDM": bookings[0].room_id,
-                # 预约日期
-                "YYRQ": bookings[0].t_start.date().isoformat(),
-                # 使用时段
-                "SYSD": ",".join(
-                    format_time_range((b.t_start.time(), b.t_end.time()))
-                    for b in bookings
-                ),
-                # 申请陈述
-                "SQCS": description or "",
-                # 备注
-                "BZ": remark or "",
-                # 联系电话
-                "LXDH": tel,
-                # 申请人姓名
-                "SQRXM": applicant,
-                # 单位代码（无用）
-                "DWDM": "299792458",  # 光在真空中的速率（m/s）
-                # 申请编码（无用）
-                "SQBM": "",
-                # 审核状态（无用）
-                "SHZT": "90",
+                "data": dumps(
+                    {
+                        # 场地代码-显示
+                        "CDDM_DISPLAY": bookings[0].room_name,
+                        # 场地代码
+                        "CDDM": bookings[0].room_id,
+                        # 预约日期
+                        "YYRQ": bookings[0].t_start.date().isoformat(),
+                        # 使用时段
+                        "SYSD": ",".join(
+                            format_time_range((b.t_start.time(), b.t_end.time()))
+                            for b in bookings
+                        ),
+                        # 申请陈述
+                        "SQCS": description or "",
+                        # 备注
+                        "BZ": remark or "",
+                        # 联系电话
+                        "LXDH": tel,
+                        # 申请人姓名
+                        "SQRXM": applicant,
+                        # 单位代码（无用）
+                        "DWDM": "299792458",  # 光在真空中的速率（m/s）
+                        # 申请编码（无用）
+                        "SQBM": "",
+                        # 审核状态（无用）
+                        "SHZT": "90",
+                    }
+                )
             },
         )
 
         res.raise_for_status()
         json = res.json()
         # 似乎服务端没验证，永远成功
-        assert json["code"] == "0" and json["msg"] == "成功"
+        assert (
+            json["code"] == "0" and json["msg"] == "成功"
+        ), f"Booking failed with {json['code']} “{json['msg']}”."
+
+    async def fetch_orders(self, room_id: str, date: datetime.date) -> list[Order]:
+        """获取已预约的时空区间
+
+        :param room_id:
+        :param date: 日期
+        """
+
+        res = await self._post(
+            "/xsfw/sys/cdyyapp/modules/kyycd/cdsyqkcx.do",
+            data={
+                "CDDM": room_id,  # 场地代码
+                "YYRQ": date.isoformat(),  # 预约日期
+            },
+        )
+        res.raise_for_status()
+        json = res.json()
+        assert json["code"] == "0", f"Fetching orders failed with {json['code']}."
+
+        orders = []
+        for row in json["data" "s"]["cdsyqkcx"]["rows"]:
+            date_str, time_str = row["SYRQ"].split()  # 使用日期
+            date = datetime.date.fromisoformat(date_str)
+            t_start, t_end = parse_time_range(time_str)
+
+            orders.append(
+                Order(
+                    # todo: room name
+                    room_name="<unknown>",
+                    room_id=room_id,
+                    applicant=row["SQRXM"],  # 申请人姓名
+                    tel=row["LXDH"],  # 联系电话
+                    description=row["SQCS"],  # 申请陈述
+                    t_start=datetime.datetime.combine(date, t_start),
+                    t_end=datetime.datetime.combine(date, t_end),
+                )
+            )
+        return orders
```

### Comparing `bitroom-0.1.4/PKG-INFO` & `bitroom-0.1.5/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bitroom
-Version: 0.1.4
+Version: 0.1.5
 Summary: BIT 场地预约查询接口（bitroom）
 Author-Email: Y.D.X. <73375426+YDX-2147483647@users.noreply.github.com>
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -20,14 +20,18 @@
 Project-URL: Bug tracker, https://github.com/YDX-2147483647/bitroom/issues
 Requires-Python: >=3.10
 Requires-Dist: PyExecJS>=1.5.1
 Requires-Dist: httpx>=0.24.0
 Requires-Dist: click>=8.1.3
 Requires-Dist: platformdirs>=3.5.0
 Requires-Dist: tomli>=2.0.1; python_version < "3.11"
+Requires-Dist: more-itertools>=9.1.0
+Requires-Dist: rich>=13.3.5; extra == "tui"
+Requires-Dist: textual>=0.23.0; extra == "tui"
+Provides-Extra: tui
 Description-Content-Type: text/markdown
 
 # 🚩🏠 bitroom (Book an Incongruent Topological Room Or be Out of Mind)
 
 [![PyPI](https://img.shields.io/pypi/v/bitroom?label=PyPI&logo=PyPI&logoColor=white)](https://pypi.org/project/bitroom/)
 [![Source GitHub](https://img.shields.io/badge/Source-GitHub-lightgray?logo=github)](https://github.com/YDX-2147483647/bitroom/)
 [![Mirror Gitee](https://img.shields.io/badge/Mirror-Gitee-red?logo=gitee)](https://gitee.com/YDX-2147483647/bitroom/)
@@ -44,42 +48,60 @@
 
   例如，你可能会问：“明天下午还有没有房间？没有的话，后天下午也行。就几个人，也不需要投影。”
 
   而很少专门针对某一房间问。
 
 bitroom 目前已解决登录、包装 API 等底层问题，可供后来者调用。
 
+## 🧪 例子
+
+### 🤖编程 API
+
+这是主要支持的接口。
+
 ```python
 from datetime import date
 from httpx import AsyncClient
 from bitroom import auth, RoomAPI
 
 async with AsyncClient() as client:
     await auth(client, username, password)  # 登录“统一身份认证”
-
     api = await RoomAPI.build(client)
+
+    # 获取“可预约”的时空区间
     bookings = await api.fetch_bookings(date.today())
     print(bookings[0])
 
+    # 预约
     await api.book(
         bookings[0],
         tel="13806491023",
         applicant="Boltzmann",
         description="Boltzmann 常数是气体的内能与温度的一种比例系数。",
         remark="一般记作 k_B 或 k。",
     )
+
+    # 获取“已预约”的时空区间
+    orders = await api.fetch_orders(bookings[0].room_id, date.today())
+    print(orders[0])
 ```
 
-当然也提供了基础的命令行接口。可结合 [fzf](https://github.com/junegunn/fzf/)，搜索日期、时间、房间。
+### ⌨️命令行 CLI
+
+也提供了基础的命令行接口，支持查询，不支持预约。
+
+可结合 [fzf](https://github.com/junegunn/fzf/)，搜索日期、时间、房间。（详见 [wiki](https://github.com/YDX-2147483647/bitroom/wiki#-fzf-%E4%BD%BF%E7%94%A8%E7%A4%BA%E4%BE%8B)）
 
 ```shell
-bitroom show | fzf
+$ bitroom show | fzf
 ```
 
-## 🧪 例子
+![](https://user-images.githubusercontent.com/73375426/236676121-0bb3f80a-4ef0-4b06-bb03-d41a6f42fe38.png)
+
+详细帮助如下。
 
 （要先`pipx install bitroom`）
 
 ```shell
 $ bitroom --help
 Usage: python -m bitroom [OPTIONS] COMMAND [ARGS]...
 
@@ -124,16 +146,30 @@
 <Booking [甘棠社区-102春·事定（Multi-function Room）] 2023-05-05 21:00–22:00>
 <Booking [甘棠社区-102春·事定（Multi-function Room）] 2023-05-06 13:20–14:05>
 <Booking [甘棠社区-102春·事定（Multi-function Room）] 2023-05-06 14:10–14:55>
 <Booking [甘棠社区-102春·事定（Multi-function Room）] 2023-05-07 15:10–15:55>
 ……
 ```
 
+### 🎨图形终端 TUI
+
+目前还在早期测试阶段，仅仅能用而已。支持查询、搜索、预约。
+
+```shell
+$ pipx install bitroom[tui]
+```
+
+![RoomApp](https://github.com/YDX-2147483647/bitroom/assets/73375426/3ad4e0fd-dfb5-43ad-a07d-70b70b6242fa)
+
+![BookSceen](https://github.com/YDX-2147483647/bitroom/assets/73375426/18a824ce-f963-4f30-b0cb-b26a0f1583b2)
+
 ## ⚙️ 配置
 
+（仅用于 CLI、TUI）
+
 编辑`config.toml`，写入学号、密码，用于登录“统一身份认证”。
 
 ```toml
 # 仅作示例，非真实信息
 username = "1120771210"
 password = "cyberpunk"
 ```
```

