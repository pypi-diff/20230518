# Comparing `tmp/tkinter_bounce_game-0.2.0.tar.gz` & `tmp/tkinter_bounce_game-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tkinter_bounce_game-0.2.0.tar", max compression
+gzip compressed data, was "tkinter_bounce_game-0.2.1.tar", max compression
```

## Comparing `tkinter_bounce_game-0.2.0.tar` & `tkinter_bounce_game-0.2.1.tar`

### file list

```diff
@@ -1,10 +1,9 @@
--rw-r--r--   0        0        0     1063 2023-02-23 14:43:29.892258 tkinter_bounce_game-0.2.0/LICENSE
--rw-r--r--   0        0        0      442 2023-02-23 14:58:22.385775 tkinter_bounce_game-0.2.0/README.md
--rw-r--r--   0        0        0     1194 2023-02-23 23:53:47.108843 tkinter_bounce_game-0.2.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-02-23 12:01:10.109377 tkinter_bounce_game-0.2.0/tkinter_bounce_game/__init__.py
--rw-r--r--   0        0        0      414 2023-02-23 23:46:31.930769 tkinter_bounce_game-0.2.0/tkinter_bounce_game/__main__.py
--rw-r--r--   0        0        0     1944 2023-02-23 15:46:13.045892 tkinter_bounce_game-0.2.0/tkinter_bounce_game/context.py
--rw-r--r--   0        0        0        0 2023-02-23 12:01:18.469328 tkinter_bounce_game-0.2.0/tkinter_bounce_game/py.typed
--rw-r--r--   0        0        0     3974 2023-02-23 23:52:05.837321 tkinter_bounce_game-0.2.0/tkinter_bounce_game/sprite.py
--rw-r--r--   0        0        0     1066 1970-01-01 00:00:00.000000 tkinter_bounce_game-0.2.0/setup.py
--rw-r--r--   0        0        0     1413 1970-01-01 00:00:00.000000 tkinter_bounce_game-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1063 2023-05-16 07:40:12.906092 tkinter_bounce_game-0.2.1/LICENSE
+-rw-r--r--   0        0        0      442 2023-05-16 07:40:12.906092 tkinter_bounce_game-0.2.1/README.md
+-rw-r--r--   0        0        0     1150 2023-05-18 08:59:49.578576 tkinter_bounce_game-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-16 07:40:12.910092 tkinter_bounce_game-0.2.1/tkinter_bounce_game/__init__.py
+-rw-r--r--   0        0        0      414 2023-05-16 07:40:12.910092 tkinter_bounce_game-0.2.1/tkinter_bounce_game/__main__.py
+-rw-r--r--   0        0        0     1944 2023-05-16 07:40:12.910092 tkinter_bounce_game-0.2.1/tkinter_bounce_game/context.py
+-rw-r--r--   0        0        0        0 2023-05-16 07:40:12.910092 tkinter_bounce_game-0.2.1/tkinter_bounce_game/py.typed
+-rw-r--r--   0        0        0     3920 2023-05-16 07:40:12.910092 tkinter_bounce_game-0.2.1/tkinter_bounce_game/sprite.py
+-rw-r--r--   0        0        0     1362 1970-01-01 00:00:00.000000 tkinter_bounce_game-0.2.1/PKG-INFO
```

### Comparing `tkinter_bounce_game-0.2.0/LICENSE` & `tkinter_bounce_game-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `tkinter_bounce_game-0.2.0/pyproject.toml` & `tkinter_bounce_game-0.2.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,37 +1,36 @@
 [tool.poetry]
 name = "tkinter-bounce-game"
-version = "0.2.0"
+version = "0.2.1"
 description = "Simple bounce game with Python and tkinter"
-authors = ["4513ECHO <4513echo@gmail.com>"]
+authors = ["4513ECHO <mail@4513echo.dev>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/4513ECHO/tkinter-bounce-game"
 packages = [{include = "tkinter_bounce_game"}]
 classifiers = [
   "License :: OSI Approved :: MIT License",
   "Programming Language :: Python",
   "Programming Language :: Python :: 3",
   "Programming Language :: Python :: 3 :: Only",
-  "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: Implementation :: CPython",
   "Topic :: Games/Entertainment",
   "Typing :: Typed",
 ]
 
 [tool.poetry.dependencies]
 python = "^3.10"
 
 [tool.poetry.group.dev.dependencies]
-black = "^23.1.0"
+black = "^23.3.0"
 isort = "^5.12.0"
-mypy = "^1.0.1"
-flake8 = "^5.0.4"
-flake8-pyproject = "^1.2.2"
+mypy = "^1.3.0"
+flake8 = "^6.0.0"
+flake8-pyproject = "^1.2.3"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.black]
 line-length = 88
```

### Comparing `tkinter_bounce_game-0.2.0/tkinter_bounce_game/context.py` & `tkinter_bounce_game-0.2.1/tkinter_bounce_game/context.py`

 * *Files identical despite different names*

### Comparing `tkinter_bounce_game-0.2.0/tkinter_bounce_game/sprite.py` & `tkinter_bounce_game-0.2.1/tkinter_bounce_game/sprite.py`

 * *Files 7% similar despite different names*

```diff
@@ -31,18 +31,17 @@
             self._y = -self._speed
         if pos[0] <= 0:
             self._x = self._speed
         if pos[2] >= self._context.canvas_width:
             self._x = -self._speed
 
     def _is_hit_paddle(self, pos: list[float]) -> bool:
+        self._paddle = self._paddle or self._context.get_sprite("paddle")
         if self._paddle is None:
-            self._paddle = self._context.get_sprite("paddle")
-            if self._paddle is None:
-                return False
+            return False
         paddle_pos = self._context.canvas.coords(self._paddle.id)
         return (
             pos[2] >= paddle_pos[0]
             and pos[0] <= paddle_pos[2]
             and paddle_pos[3] >= pos[3] >= paddle_pos[1]
         )
 
@@ -60,25 +59,23 @@
         self._x = 0
         context.canvas.bind_all("<KeyPress-Left>", self._turn)
         context.canvas.bind_all("<KeyPress-Right>", self._turn)
 
     def draw(self) -> None:
         self._context.canvas.move(self.id, self._x, 0)
         pos = self._context.canvas.coords(self.id)
-        if pos[0] <= 0:
-            self._x = 0
-        if pos[2] >= self._context.canvas_width:
+        if pos[0] <= 0 or pos[2] >= self._context.canvas_width:
             self._x = 0
 
     def _turn(self, event: Event[Misc]) -> None:
         pos = self._context.canvas.coords(self.id)
         match event.keysym:
-            case "Left" if pos[0] >= 0:
+            case "Left" if not pos[0] <= 0:
                 self._x = -self._speed
-            case "Right" if pos[2] <= self._context.canvas_width:
+            case "Right" if not pos[2] >= self._context.canvas_width:
                 self._x = self._speed
 
 
 class PointCounter:
     role = "pointcounter"
 
     def __init__(self, context: Context) -> None:
```

### Comparing `tkinter_bounce_game-0.2.0/PKG-INFO` & `tkinter_bounce_game-0.2.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 Metadata-Version: 2.1
 Name: tkinter-bounce-game
-Version: 0.2.0
+Version: 0.2.1
 Summary: Simple bounce game with Python and tkinter
 Home-page: https://github.com/4513ECHO/tkinter-bounce-game
 License: MIT
 Author: 4513ECHO
-Author-email: 4513echo@gmail.com
+Author-email: mail@4513echo.dev
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Games/Entertainment
 Classifier: Typing :: Typed
 Project-URL: Repository, https://github.com/4513ECHO/tkinter-bounce-game
 Description-Content-Type: text/markdown
 
 # tkinter-bounce-game
```

