# Comparing `tmp/nonebot-desktop-tk-1.0.5.tar.gz` & `tmp/nonebot-desktop-tk-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot-desktop-tk-1.0.5.tar", last modified: Sun Apr 30 16:38:49 2023, max compression
+gzip compressed data, was "nonebot-desktop-tk-1.0.6.tar", last modified: Thu May 18 14:29:31 2023, max compression
```

## Comparing `nonebot-desktop-tk-1.0.5.tar` & `nonebot-desktop-tk-1.0.6.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 16:38:49.972807 nonebot-desktop-tk-1.0.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-04-30 16:38:33.000000 nonebot-desktop-tk-1.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-04-30 16:38:49.972807 nonebot-desktop-tk-1.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-30 16:38:33.000000 nonebot-desktop-tk-1.0.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      553 2023-04-30 16:38:33.000000 nonebot-desktop-tk-1.0.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-30 16:38:49.972807 nonebot-desktop-tk-1.0.5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 16:38:49.968807 nonebot-desktop-tk-1.0.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 16:38:49.968807 nonebot-desktop-tk-1.0.5/src/nonebot_desktop_tk/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-30 16:38:33.000000 nonebot-desktop-tk-1.0.5/src/nonebot_desktop_tk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-04-30 16:38:33.000000 nonebot-desktop-tk-1.0.5/src/nonebot_desktop_tk/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    51807 2023-04-30 16:38:33.000000 nonebot-desktop-tk-1.0.5/src/nonebot_desktop_tk/gui.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 16:38:49.972807 nonebot-desktop-tk-1.0.5/src/nonebot_desktop_tk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-04-30 16:38:49.000000 nonebot-desktop-tk-1.0.5/src/nonebot_desktop_tk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      361 2023-04-30 16:38:49.000000 nonebot-desktop-tk-1.0.5/src/nonebot_desktop_tk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-30 16:38:49.000000 nonebot-desktop-tk-1.0.5/src/nonebot_desktop_tk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-30 16:38:49.000000 nonebot-desktop-tk-1.0.5/src/nonebot_desktop_tk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-30 16:38:49.000000 nonebot-desktop-tk-1.0.5/src/nonebot_desktop_tk.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 14:29:31.588411 nonebot-desktop-tk-1.0.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-18 14:29:20.000000 nonebot-desktop-tk-1.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-05-18 14:29:31.588411 nonebot-desktop-tk-1.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-05-18 14:29:20.000000 nonebot-desktop-tk-1.0.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      553 2023-05-18 14:29:20.000000 nonebot-desktop-tk-1.0.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-18 14:29:31.588411 nonebot-desktop-tk-1.0.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 14:29:31.588411 nonebot-desktop-tk-1.0.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 14:29:31.588411 nonebot-desktop-tk-1.0.6/src/nonebot_desktop_tk/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 14:29:20.000000 nonebot-desktop-tk-1.0.6/src/nonebot_desktop_tk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-18 14:29:20.000000 nonebot-desktop-tk-1.0.6/src/nonebot_desktop_tk/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51821 2023-05-18 14:29:20.000000 nonebot-desktop-tk-1.0.6/src/nonebot_desktop_tk/gui.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 14:29:31.588411 nonebot-desktop-tk-1.0.6/src/nonebot_desktop_tk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-05-18 14:29:31.000000 nonebot-desktop-tk-1.0.6/src/nonebot_desktop_tk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      361 2023-05-18 14:29:31.000000 nonebot-desktop-tk-1.0.6/src/nonebot_desktop_tk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 14:29:31.000000 nonebot-desktop-tk-1.0.6/src/nonebot_desktop_tk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-18 14:29:31.000000 nonebot-desktop-tk-1.0.6/src/nonebot_desktop_tk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-18 14:29:31.000000 nonebot-desktop-tk-1.0.6/src/nonebot_desktop_tk.egg-info/top_level.txt
```

### Comparing `nonebot-desktop-tk-1.0.5/LICENSE` & `nonebot-desktop-tk-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot-desktop-tk-1.0.5/PKG-INFO` & `nonebot-desktop-tk-1.0.6/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-desktop-tk
-Version: 1.0.5
+Version: 1.0.6
 Summary: NoneBot2 GUI manager written with tkinter.
 Author-email: HivertMoZara <worldmozara@163.com>
 License: MIT
 Project-URL: Homepage, https://github.com/nonedesktop/nonebot-desktop-tk
 Project-URL: Repository, https://github.com/nonedesktop/nonebot-desktop-tk
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `nonebot-desktop-tk-1.0.5/README.md` & `nonebot-desktop-tk-1.0.6/README.md`

 * *Files identical despite different names*

### Comparing `nonebot-desktop-tk-1.0.5/pyproject.toml` & `nonebot-desktop-tk-1.0.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "nonebot-desktop-tk"
-version = "1.0.5"
+version = "1.0.6"
 description = "NoneBot2 GUI manager written with tkinter."
 authors = [
     {name = "HivertMoZara", email = "worldmozara@163.com"},
 ]
 license = {text = "MIT"}
 dependencies = ["tkreform>=0.3.6", "nonebot-desktop-wing>=0.2.8"]
 requires-python = ">=3.8"
```

### Comparing `nonebot-desktop-tk-1.0.5/src/nonebot_desktop_tk/gui.py` & `nonebot-desktop-tk-1.0.6/src/nonebot_desktop_tk/gui.py`

 * *Files 1% similar despite different names*

```diff
@@ -671,21 +671,21 @@
         self.win[0][0].base["value"] = self.allenvs
         self.envf_updator()
 
     def new_option(self) -> None:
         k, v = StringVar(value="参数名"), StringVar(value="值")
         self.curopts.append((k, v))
         _row = self.win[1].add_widget(tk.Frame)
-        _row.grid(column=0, sticky="w")
+        _row.pack(fill="x", expand=True)
         _key = _row.add_widget(tk.Entry, textvariable=k, font=mono10)
         _lbl = _row.add_widget(tk.Label, text=" = ", font=mono10)
-        _val = _row.add_widget(tk.Entry, textvariable=v, font=mono10, width=40)
+        _val = _row.add_widget(tk.Entry, textvariable=v, font=mono10)
         _key.pack(side="left")
         _lbl.pack(side="left")
-        _val.pack(side="left")
+        _val.pack(fill="x", expand=True, side="left")
 
     def save_env(self):
         try:
             with open(self.context.cwd_path / self.target_name, "w") as f:
                 f.writelines(f"{k}={v}\n" for k, v in ((_k.get(), _v.get()) for _k, _v in self.curopts) if k and v)
         except Exception as e:
             messagebox.showerror("错误", f"{e}", master=self.win.base)
```

### Comparing `nonebot-desktop-tk-1.0.5/src/nonebot_desktop_tk.egg-info/PKG-INFO` & `nonebot-desktop-tk-1.0.6/src/nonebot_desktop_tk.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-desktop-tk
-Version: 1.0.5
+Version: 1.0.6
 Summary: NoneBot2 GUI manager written with tkinter.
 Author-email: HivertMoZara <worldmozara@163.com>
 License: MIT
 Project-URL: Homepage, https://github.com/nonedesktop/nonebot-desktop-tk
 Project-URL: Repository, https://github.com/nonedesktop/nonebot-desktop-tk
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

