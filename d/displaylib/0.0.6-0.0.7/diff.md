# Comparing `tmp/displaylib-0.0.6.tar.gz` & `tmp/displaylib-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "displaylib-0.0.6.tar", last modified: Mon Feb 27 08:09:42 2023, max compression
+gzip compressed data, was "displaylib-0.0.7.tar", last modified: Thu May 18 19:46:40 2023, max compression
```

## Comparing `displaylib-0.0.6.tar` & `displaylib-0.0.7.tar`

### file list

```diff
@@ -1,41 +1,53 @@
-drwxrwxrwx   0        0        0        0 2023-02-27 08:09:42.825991 displaylib-0.0.6/
--rw-rw-rw-   0        0        0      156 2023-02-27 08:09:42.823163 displaylib-0.0.6/PKG-INFO
--rw-rw-rw-   0        0        0     1646 2023-02-24 16:11:54.000000 displaylib-0.0.6/README.md
-drwxrwxrwx   0        0        0        0 2023-02-27 08:09:42.662502 displaylib-0.0.6/displaylib/
--rw-rw-rw-   0        0        0      985 2023-02-22 21:35:25.000000 displaylib-0.0.6/displaylib/__init__.py
-drwxrwxrwx   0        0        0        0 2023-02-27 08:09:42.763245 displaylib-0.0.6/displaylib/ascii/
--rw-rw-rw-   0        0        0     1184 2023-02-24 16:30:03.000000 displaylib-0.0.6/displaylib/ascii/__init__.py
--rw-rw-rw-   0        0        0     6725 2023-02-25 15:51:16.000000 displaylib-0.0.6/displaylib/ascii/animation.py
--rw-rw-rw-   0        0        0     1240 2023-02-22 21:58:40.000000 displaylib-0.0.6/displaylib/ascii/camera.py
--rw-rw-rw-   0        0        0     3139 2023-02-03 17:24:34.000000 displaylib-0.0.6/displaylib/ascii/client.py
--rw-rw-rw-   0        0        0      697 2023-02-13 15:24:16.000000 displaylib-0.0.6/displaylib/ascii/clock.py
--rw-rw-rw-   0        0        0     3205 2023-02-22 21:45:45.000000 displaylib-0.0.6/displaylib/ascii/engine.py
--rw-rw-rw-   0        0        0      498 2023-02-17 12:30:13.000000 displaylib-0.0.6/displaylib/ascii/grapheme.py
--rw-rw-rw-   0        0        0     1302 2023-02-23 10:30:00.000000 displaylib-0.0.6/displaylib/ascii/image.py
--rw-rw-rw-   0        0        0      761 2023-02-20 14:22:57.000000 displaylib-0.0.6/displaylib/ascii/node.py
-drwxrwxrwx   0        0        0        0 2023-02-27 08:09:42.768562 displaylib-0.0.6/displaylib/ascii/prefab/
--rw-rw-rw-   0        0        0      900 2023-02-23 10:31:13.000000 displaylib-0.0.6/displaylib/ascii/prefab/label.py
--rw-rw-rw-   0        0        0      733 2023-02-20 14:50:05.000000 displaylib-0.0.6/displaylib/ascii/screen.py
--rw-rw-rw-   0        0        0     4146 2023-02-22 21:40:22.000000 displaylib-0.0.6/displaylib/ascii/surface.py
--rw-rw-rw-   0        0        0      195 2023-02-08 12:14:43.000000 displaylib-0.0.6/displaylib/ascii/types.py
--rw-rw-rw-   0        0        0     2413 2023-02-22 15:46:06.000000 displaylib-0.0.6/displaylib/math.py
--rw-rw-rw-   0        0        0     4528 2023-02-03 17:24:34.000000 displaylib-0.0.6/displaylib/overload.py
-drwxrwxrwx   0        0        0        0 2023-02-27 08:09:42.798705 displaylib-0.0.6/displaylib/pygame/
--rw-rw-rw-   0        0        0      816 2023-02-20 15:01:44.000000 displaylib-0.0.6/displaylib/pygame/__init__.py
--rw-rw-rw-   0        0        0       75 2023-02-03 17:24:34.000000 displaylib-0.0.6/displaylib/pygame/constants.py
--rw-rw-rw-   0        0        0     3232 2023-02-03 17:24:34.000000 displaylib-0.0.6/displaylib/pygame/engine.py
--rw-rw-rw-   0        0        0      514 2023-02-17 12:47:42.000000 displaylib-0.0.6/displaylib/pygame/node.py
--rw-rw-rw-   0        0        0      124 2023-02-03 17:24:34.000000 displaylib-0.0.6/displaylib/pygame/types.py
-drwxrwxrwx   0        0        0        0 2023-02-27 08:09:42.817652 displaylib-0.0.6/displaylib/template/
--rw-rw-rw-   0        0        0      342 2023-02-17 12:50:41.000000 displaylib-0.0.6/displaylib/template/__init__.py
--rw-rw-rw-   0        0        0      197 2023-02-03 17:24:34.000000 displaylib-0.0.6/displaylib/template/client.py
--rw-rw-rw-   0        0        0      945 2023-02-11 20:27:38.000000 displaylib-0.0.6/displaylib/template/engine.py
--rw-rw-rw-   0        0        0     2745 2023-02-20 14:26:38.000000 displaylib-0.0.6/displaylib/template/node.py
--rw-rw-rw-   0        0        0       86 2023-02-11 20:27:04.000000 displaylib-0.0.6/displaylib/template/types.py
-drwxrwxrwx   0        0        0        0 2023-02-27 08:09:42.703230 displaylib-0.0.6/displaylib.egg-info/
--rw-rw-rw-   0        0        0      156 2023-02-27 08:09:42.000000 displaylib-0.0.6/displaylib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      870 2023-02-27 08:09:42.000000 displaylib-0.0.6/displaylib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-02-27 08:09:42.000000 displaylib-0.0.6/displaylib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2023-02-27 08:09:42.000000 displaylib-0.0.6/displaylib.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-02-27 08:09:42.827304 displaylib-0.0.6/setup.cfg
--rw-rw-rw-   0        0        0      411 2023-02-24 16:12:06.000000 displaylib-0.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-18 19:46:40.381550 displaylib-0.0.7/
+-rw-rw-rw-   0        0        0     4250 2023-05-18 19:46:40.379019 displaylib-0.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0     3918 2023-04-02 12:06:36.000000 displaylib-0.0.7/README.md
+drwxrwxrwx   0        0        0        0 2023-05-18 19:46:40.148480 displaylib-0.0.7/displaylib/
+-rw-rw-rw-   0        0        0     1571 2023-03-31 06:33:19.000000 displaylib-0.0.7/displaylib/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-18 19:46:40.252791 displaylib-0.0.7/displaylib/ascii/
+-rw-rw-rw-   0        0        0     1475 2023-03-31 06:47:32.000000 displaylib-0.0.7/displaylib/ascii/__init__.py
+-rw-rw-rw-   0        0        0     8303 2023-04-16 15:46:56.000000 displaylib-0.0.7/displaylib/ascii/animation.py
+-rw-rw-rw-   0        0        0     2011 2023-04-02 10:48:57.000000 displaylib-0.0.7/displaylib/ascii/camera.py
+-rw-rw-rw-   0        0        0     1404 2023-05-16 17:27:07.000000 displaylib-0.0.7/displaylib/ascii/clock.py
+-rw-rw-rw-   0        0        0     5374 2023-05-16 17:40:47.000000 displaylib-0.0.7/displaylib/ascii/engine.py
+-rw-rw-rw-   0        0        0     4317 2023-03-29 14:58:57.000000 displaylib-0.0.7/displaylib/ascii/grapheme.py
+drwxrwxrwx   0        0        0        0 2023-05-18 19:46:40.274126 displaylib-0.0.7/displaylib/ascii/networking/
+-rw-rw-rw-   0        0        0      609 2023-04-01 18:47:05.000000 displaylib-0.0.7/displaylib/ascii/networking/__init__.py
+-rw-rw-rw-   0        0        0      229 2023-03-30 07:33:53.000000 displaylib-0.0.7/displaylib/ascii/networking/broadcast_server.py
+-rw-rw-rw-   0        0        0      193 2023-03-30 07:33:42.000000 displaylib-0.0.7/displaylib/ascii/networking/client.py
+-rw-rw-rw-   0        0        0      202 2023-03-30 07:33:50.000000 displaylib-0.0.7/displaylib/ascii/networking/server.py
+-rw-rw-rw-   0        0        0      944 2023-03-31 07:28:26.000000 displaylib-0.0.7/displaylib/ascii/node.py
+drwxrwxrwx   0        0        0        0 2023-05-18 19:46:40.294735 displaylib-0.0.7/displaylib/ascii/prefab/
+-rw-rw-rw-   0        0        0     2115 2023-04-02 19:16:16.000000 displaylib-0.0.7/displaylib/ascii/prefab/image.py
+-rw-rw-rw-   0        0        0     1117 2023-04-02 19:16:59.000000 displaylib-0.0.7/displaylib/ascii/prefab/label.py
+-rw-rw-rw-   0        0        0     2554 2023-04-02 10:34:54.000000 displaylib-0.0.7/displaylib/ascii/prefab/line.py
+-rw-rw-rw-   0        0        0      586 2023-03-31 07:32:05.000000 displaylib-0.0.7/displaylib/ascii/prefab/sprite.py
+-rw-rw-rw-   0        0        0      739 2023-03-31 07:16:26.000000 displaylib-0.0.7/displaylib/ascii/screen.py
+-rw-rw-rw-   0        0        0     9377 2023-03-27 07:32:53.000000 displaylib-0.0.7/displaylib/ascii/surface.py
+-rw-rw-rw-   0        0        0     1123 2023-04-02 10:32:30.000000 displaylib-0.0.7/displaylib/ascii/texture.py
+-rw-rw-rw-   0        0        0     8893 2023-05-16 17:50:41.000000 displaylib-0.0.7/displaylib/math.py
+drwxrwxrwx   0        0        0        0 2023-05-18 19:46:40.313772 displaylib-0.0.7/displaylib/pygame/
+-rw-rw-rw-   0        0        0      932 2023-04-02 11:10:18.000000 displaylib-0.0.7/displaylib/pygame/__init__.py
+-rw-rw-rw-   0        0        0      127 2023-04-02 19:07:04.000000 displaylib-0.0.7/displaylib/pygame/constants.py
+-rw-rw-rw-   0        0        0     5044 2023-05-16 17:41:15.000000 displaylib-0.0.7/displaylib/pygame/engine.py
+drwxrwxrwx   0        0        0        0 2023-05-18 19:46:40.318770 displaylib-0.0.7/displaylib/pygame/networking/
+-rw-rw-rw-   0        0        0      442 2023-04-02 09:47:01.000000 displaylib-0.0.7/displaylib/pygame/networking/__init__.py
+-rw-rw-rw-   0        0        0     1055 2023-04-02 11:36:07.000000 displaylib-0.0.7/displaylib/pygame/node.py
+drwxrwxrwx   0        0        0        0 2023-05-18 19:46:40.331850 displaylib-0.0.7/displaylib/template/
+-rw-rw-rw-   0        0        0      483 2023-03-31 06:32:36.000000 displaylib-0.0.7/displaylib/template/__init__.py
+-rw-rw-rw-   0        0        0     3085 2023-05-16 17:41:28.000000 displaylib-0.0.7/displaylib/template/engine.py
+drwxrwxrwx   0        0        0        0 2023-05-18 19:46:40.376135 displaylib-0.0.7/displaylib/template/networking/
+-rw-rw-rw-   0        0        0      491 2023-04-01 18:43:15.000000 displaylib-0.0.7/displaylib/template/networking/__init__.py
+-rw-rw-rw-   0        0        0     2786 2023-05-18 11:24:11.000000 displaylib-0.0.7/displaylib/template/networking/broadcast_server.py
+-rw-rw-rw-   0        0        0      400 2023-04-01 18:45:47.000000 displaylib-0.0.7/displaylib/template/networking/class_register.py
+-rw-rw-rw-   0        0        0     6673 2023-05-18 11:23:00.000000 displaylib-0.0.7/displaylib/template/networking/client.py
+-rw-rw-rw-   0        0        0     3425 2023-04-01 18:54:10.000000 displaylib-0.0.7/displaylib/template/networking/deserialize.py
+-rw-rw-rw-   0        0        0     2168 2023-04-01 18:16:21.000000 displaylib-0.0.7/displaylib/template/networking/serialize.py
+-rw-rw-rw-   0        0        0     4655 2023-05-18 11:27:57.000000 displaylib-0.0.7/displaylib/template/networking/server.py
+-rw-rw-rw-   0        0        0     6535 2023-05-16 17:52:59.000000 displaylib-0.0.7/displaylib/template/node.py
+drwxrwxrwx   0        0        0        0 2023-05-18 19:46:40.199135 displaylib-0.0.7/displaylib.egg-info/
+-rw-rw-rw-   0        0        0     4250 2023-05-18 19:46:39.000000 displaylib-0.0.7/displaylib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1329 2023-05-18 19:46:39.000000 displaylib-0.0.7/displaylib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-18 19:46:39.000000 displaylib-0.0.7/displaylib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2023-05-18 19:46:39.000000 displaylib-0.0.7/displaylib.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-18 19:46:40.381550 displaylib-0.0.7/setup.cfg
+-rw-rw-rw-   0        0        0      862 2023-05-18 19:46:33.000000 displaylib-0.0.7/setup.py
```

### Comparing `displaylib-0.0.6/displaylib/ascii/animation.py` & `displaylib-0.0.7/displaylib/ascii/animation.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,73 +1,105 @@
+from __future__ import annotations
+
 import os
-from typing_extensions import Self
+from typing import TYPE_CHECKING, Generator
+
 from ..template import Node
 from . import grapheme
-from .types import ModeFlags, ASCIISurface
+from .texture import Texture
+
+if TYPE_CHECKING:
+    from .node import ASCIINode2D
+    from .surface import ASCIISurface
 
 
 __all__ = [
     "Frame",
     "Animation",
     "EmptyAnimation",
     "AnimationPlayer"
 ]
 
 
 class Frame:
-    __slots__ = ("content")
+    """`Frame` used to create animations
 
-    def __init__(self, fpath: str, flip: bool = False) -> None:
-        self.content = []
+    Loaded from files
+    """
+    __slots__ = ("texture")
+
+    def __init__(self, fpath: str, fliph: bool = False, flipv: bool = False) -> None:
+        self.texture = []
         f = open(fpath)
-        if flip:
-            for line in f.readlines():
-                self.content.append(list(grapheme.flip(line.rstrip("\n"))))
-        else:
-            for line in f.readlines():
-                self.content.append(list(line.rstrip("\n")))
+        for line in f.readlines():
+            self.texture.append(list(line.rstrip("\n")))
+        if fliph:
+            self.texture = grapheme.mapfliph(self.texture)
+        if flipv:
+            self.texture = grapheme.mapfliph(self.texture)
         f.close()
 
 
 class Animation:
+    """`Animation` containing frames
+
+    Frames are loaded from files
+    """
     __slots__ = ("frames")
 
-    def __init__(self, path: str, reverse: bool = False, flip: bool = False) -> None:
-        fnames = os.listdir(path)
+    def __init__(self, path: str, reverse: bool = False, fliph: bool = False, flipv: bool = False) -> None:
+        fnames = os.listdir(os.path.join(os.getcwd(), path))
         step = 1 if not reverse else -1
-        self.frames = [Frame(os.path.join(path, fname), flip=flip) for fname in fnames][::step]
+        self.frames = [Frame(os.path.join(os.getcwd(), path, fname), fliph=fliph, flipv=flipv) for fname in fnames][::step]
 
 
 class EmptyAnimation(Animation):
+    """Empty `Animation`, more like a placeholder
+    """
     __slots__ = ("frames")
 
     def __init__(self) -> None:
         self.frames = []
 
 
 class AnimationPlayer(Node): # TODO: add buffered animations on load
-    FIXED = 0 # TODO: implement FIXED and DELTATIME mode
-    # DELTATIME = 1
-
-    def __init__(self, parent: Self | None = None, fps: float = 16, mode: ModeFlags = FIXED, **animations) -> None:
+    """`AnimationPlayer` to be attached to a node, so it can control animations
+    """
+    FIXED = 0
+    DELTATIME = 1 # TODO: DELTATIME mode
+    mode_default = FIXED
+
+    def __init__(self, parent: Texture | None = None, fps: float = 16, mode: int = mode_default, **animations) -> None:
+        if not isinstance(parent, Texture) or parent == None:
+            raise TypeError(f"parent in AnimationPlayer cannot be '{type(parent)}' (requires Texture in MRO)")
         super().__init__(parent, force_sort=False)
         self.fps: float = fps
-        self.mode: ModeFlags = mode # process mode (FIXED | DELTATIME)
+        self.mode: int = mode
         self.animations: dict[str, Animation] = dict(animations)
         self.current_animation: str = ""
         self.is_playing: bool = False
-        self._current_frames: bool = None
-        self._next: Frame | None = None
-        self._has_updated: bool = False # indicates if the first frame (per animation) have been displayed
+        self._current_frames: Generator[Frame, None, None] | None = None
+        self._next: None | Frame = None
+        self._has_updated: bool = False # indicates if the first frame (per animation) has been displayed
         self._accumulated_time: float = 0.0
     
-    def __iter__(self):
+    def __iter__(self) -> AnimationPlayer:
+        """Use itself as main iterator
+
+        Returns:
+            AnimationPlayer: itself
+        """
         return self
 
     def __next__(self) -> Frame:
+        """Returns the next frame from the current frames (a generator)
+
+        Returns:
+            Frame: the next frame
+        """
         try:
             self._next = next(self._current_frames) # next of generator
             return self._next
         except StopIteration:
             self.is_playing = False
             self._current_frames = None
             self._next = None
@@ -95,21 +127,40 @@
         try:
             self._next = next(self._current_frames)
         except StopIteration:
             self.is_playing = False
             self._current_frames = None
             self._next = None
     
-    def get(self, name: str) -> Animation:
-        return self.animations[name]
+    def get(self, name: str) -> Animation | None:
+        """Returns a stored animation given its name
+
+        Args:
+            name (str): name of the animation
+
+        Returns:
+            Animation | None: animation object or None if not found
+        """
+        return self.animations.get(name, None)
     
     def add(self, name: str, animation: Animation) -> None:
+        """Adds a new animation and binds it to a name
+
+        Args:
+            name (str): name to access the animation later
+            animation (Animation): animation object to store
+        """
         self.animations[name] = animation
     
     def remove(self, name: str) -> None:
+        """Removes an animation given the name of the animation
+
+        Args:
+            name (str): name of the animation to delete
+        """
         del self.animations[name]
     
     def play(self, animation: str) -> None:
         """Plays an animation given the name of the animation
 
         Args:
             animation (str): the name of the animation to play
@@ -120,15 +171,15 @@
         try:
             self._next: Frame = next(self._current_frames)
         except StopIteration:
             self.is_playing = False
             self._current_frames = None
             self._next: Frame = None
         if self._next != None:
-            self.parent.content = self._next.content
+            self.parent.texture = self._next.texture
             self._has_updated = False
     
     def play_backwards(self, animation: str) -> None:
         """Plays an animation backwards given the name of the animation
 
         Args:
             animation (str): the name of the animation to play backwards
@@ -140,60 +191,60 @@
         try:
             self._next: Frame = next(self._current_frames)
         except StopIteration:
             self.is_playing = False
             self._current_frames = None
             self._next: Frame = None
         if self._next != None:
-            self.parent.content = self._next.content
+            self.parent.texture = self._next.texture
             self._has_updated = False
         
     def advance(self) -> bool:
         """Advances 1 frame
 
         Can be used in a `while loop`:
         >>> while self.my_animation_player.advance():
-        ...     ... # do stuff each frame
+        >>>     ... # do stuff each frame
 
         Returns:
             bool: whether it was NOT stopped
         """
         if self._current_frames == None:
             return False
         frame = self._next
         try:
             self._next = next(self._current_frames)
         except StopIteration:
             self.is_playing = False
             self._current_frames = None
             self._next = None
         if frame != None:
-            self.parent.content = frame.content
+            self.parent.texture = frame.texture
             self._has_updated = False
         return frame != None # returns true if not stopped
 
 
     def stop(self) -> None:
         """Stops the animation from playing
         """
         self.is_playing = False
 
     def _render(self, surface: ASCIISurface) -> None: # dummy method
         return
 
-    def _update(self, delta: float) -> None:
+    def _update(self, _delta: float) -> None:
         if self.is_playing and self._has_updated:
             # if self.mode == AnimationPlayer.FIXED:
             frame = next(self)
             if frame == None:
                 return
-            self.parent.content = frame.content
+            self.parent.texture = frame.texture
 
             # elif self.mode == AnimationPlayer.DELTATIME:
             #     # apply delta time
             #     self._accumulated_time += delta
             #     if self._accumulated_time >= self._fps_ratio:
             #         self._accumulated_time -= self._fps_ratio # does not clear time
             #         frame = next(self)
-            #         self.owner.content = frame.content
+            #         self.owner.texture = frame.texture
         elif not self._has_updated:
             self._has_updated = True
```

### Comparing `displaylib-0.0.6/displaylib/ascii/prefab/label.py` & `displaylib-0.0.7/displaylib/ascii/prefab/label.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,30 +1,37 @@
-from typing_extensions import Self
-from ..node import ASCIINode
+from __future__ import annotations
 
+from typing import TYPE_CHECKING
 
-class ASCIILabel(ASCIINode):
+from ..node import ASCIINode2D
+from ..texture import Texture
+
+if TYPE_CHECKING:
+    from ...template import Node
+
+
+class ASCIILabel(ASCIINode2D, Texture):
     """Prefabricated `Label` node
 
     A new line is created for each `\\n`
     """
-    def __init__(self, parent: Self | None = None, x: int = 0, y: int = 0, text: str = "", z_index: int = 0, force_sort: bool = True) -> None:
-        super().__init__(parent, x, y, z_index, force_sort)
+    def __init__(self, parent: Node | None = None, x: int = 0, y: int = 0, *, text: str = "", z_index: int = 0, force_sort: bool = True) -> None:
+        super().__init__(parent, x, y, z_index=z_index, force_sort=force_sort)
         self.text = text
     
     @property
     def text(self) -> str:
-        """Returns a string from content
+        """Returns a string from texture
 
         Returns:
             str: content as string
         """
-        return "\n".join("".join(line) for line in self.content)
+        return "\n".join("".join(line) for line in self.texture)
     
     @text.setter
     def text(self, text: str) -> None:
-        """Set content from string
+        """Set content from string. Argument `text` is run through `str` in the process
 
         Args:
             text (str): string to be converted to content
         """
-        self.content = [list(line) for line in text.split("\n")]
+        self.texture = [list(line) for line in str(text).split("\n")]
```

### Comparing `displaylib-0.0.6/displaylib/pygame/engine.py` & `displaylib-0.0.7/displaylib/ascii/prefab/line.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,89 +1,65 @@
-import pygame
-from pygame.constants import *
-from ..template import Node, Engine
-from .constants import DEFAULT, MILLISECOND
-from .types import Event, Surface
-
-
-class PygameEngine(Engine):
-    bg_color = (255, 255, 255) # white
-
-    def __init__(self, window_name: str = "DisplayLib Window", tps: int = 60, width: int = 512, height: int = 256, icon_path: str | None = None, flags: int = DEFAULT) -> None:
-        self._window_name = window_name # TODO: add setter
-        self.tps = tps
-        self._width = width # TODO: add setter
-        self._height = height # TODO: add setter
-        self.icon_img: None | Surface = None
-        if icon_path:
-            pygame.image.load(icon_path)
-            pygame.display.set_icon(self.icon_img)
-        self.flags = flags
-        self.screen = pygame.display.set_mode(size=(width, height), flags=flags)
-        self.display = pygame.Surface(size=(width, height))
-        self._on_start()
-        
-        self.is_running = True
-        self._main_loop()
-    
-    @property
-    def height(self) -> int:
-        return self._height
-    
-    @property
-    def height(self, value: int) -> None: # TODO: queue this action
-        self._height = value
-        self.screen = pygame.display.set_mode(size=(self.width, self.height), flags=self.flags)
-    
-    @property
-    def width(self) -> int:
-        return self._width
-    
-    @property
-    def width(self, value: int) -> None: # TODO: queue this action
-        self._width = value
-        self.screen = pygame.display.set_mode(size=(self.width, self.height), flags=self.flags)
-
-    @property
-    def icon(self) -> None:
-        return self.icon_img
-    
-    @property
-    def icon(self, icon_path: str) -> None:
-        self.icon_img = pygame.image.load(icon_path)
-        pygame.display.set_icon(self.icon_img)
-
-    def _input(self, event: Event) -> None:
-        if event.type == QUIT:
-            self.is_running = False
-    
-    def _main_loop(self) -> None:
-        def sort_fn(element):
-            return element[1].z_index
-
-        clock = pygame.time.Clock()
-        delta = 1.0 / self.tps
-        # update one time at the very start
-        self.screen.fill(self.bg_color)
-        pygame.display.flip()
-
-        while self.is_running:
-            self._update(delta)
-            nodes = tuple(Node.nodes.values())
-            for event in pygame.event.get():
-                self._input(event)
-                for node in nodes:
-                    node._input(event)
-            for node in nodes:
-                node._update(delta)
-            if Node._request_sort: # only sort once per frame if needed
-                Node.nodes = {k: v for k, v in sorted(Node.nodes.items(), key=sort_fn)}
-            
-            self.display.fill(self.bg_color)
-            for node in nodes: # render nodes onto the display
-                node._render(self.display)
-            # TODO: implement camera
-            self.screen.blit(self.display, (0, 0)) # render display onto the main screen
-            
-            pygame.display.flip()
-            delta = clock.tick(self.tps) / MILLISECOND # milliseconds -> seconds
-        self._on_exit()
+from __future__ import annotations
+
+from typing import TYPE_CHECKING, ClassVar
+
+from ...math import Vec2
+from ..node import ASCIINode2D
+from ..texture import Texture
+
+if TYPE_CHECKING:
+    from ...template import Node
+
+
+class ASCIIPoint2D(ASCIINode2D, Texture):
+    """Thin wrapper around `ASCIINode2D` capable of displaying a single point
+    
+    Components:
+        `Texture`: allows the node to be displayed
+    """
+    def __init__(self, parent: Node | None = None, x: int = 0, y: int = 0, *, texture: str = "#", z_index: int = 0, force_sort: bool = True) -> None:
+        super().__init__(parent, x, y, z_index=z_index, force_sort=force_sort)
+        self.texture = [[texture]]
+
+
+class ASCIILine(ASCIINode2D):
+    """Prefabricated `Line` node
+
+    Known issue: Does not work well when changing `rotation` or `global_rotation`
+    """
+    texture_default: ClassVar[str] = "#" # only used when creating a line node
+
+    def __init__(self, parent: Node | None = None, x: int = 0, y: int = 0, *, start: Vec2 = Vec2(0, 0), end: Vec2 = Vec2(0, 0), texture: str | None = None, z_index: int = 0, force_sort: bool = True) -> None:
+        super().__init__(parent, x, y, z_index=z_index, force_sort=force_sort)
+        self.start = start
+        self.end = end
+        self.texture = texture or self.texture_default
+        self.points: list[ASCIIPoint2D] = [
+            ASCIIPoint2D(self, z_index=self.z_index, texture=self.texture).where(position=start),
+            ASCIIPoint2D(self, z_index=self.z_index, texture=self.texture).where(position=end)
+        ]
+
+    def _update(self, delta: float) -> None:
+        # -- clear points
+        for point in self.points:
+            point.queue_free()
+        self.points.clear()
+
+        if not self.visible:
+            return
+        # -- create points along the current/new line
+        diff = (self.end - self.start)
+        direction = diff.normalized()
+        length = diff.length() # length of difference
+        steps = round(length)
+        for idx in range(steps):
+            position = self.start + (direction * idx)
+            point = ASCIIPoint2D(self, x=int(position.x), y=int(position.y), texture=self.texture, z_index=self.z_index)
+            self.points.append(point)
+    
+    def queue_free(self) -> None:
+        """Queues all points for deletion before calling its super().queue_free()
+        """
+        for point in self.points:
+            point.queue_free()
+        self.points.clear()
+        super().queue_free()
```

