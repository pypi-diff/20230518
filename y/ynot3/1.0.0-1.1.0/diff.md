# Comparing `tmp/ynot3-1.0.0.tar.gz` & `tmp/ynot3-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ynot3-1.0.0.tar", max compression
+gzip compressed data, was "ynot3-1.1.0.tar", max compression
```

## Comparing `ynot3-1.0.0.tar` & `ynot3-1.1.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1030 2023-05-18 13:13:03.020756 ynot3-1.0.0/README.md
--rw-r--r--   0        0        0      519 2023-05-18 13:14:24.859776 ynot3-1.0.0/pyproject.toml
--rwxr-xr-x   0        0        0      314 2023-05-18 13:11:38.461735 ynot3-1.0.0/ynot3/__init__.py
--rw-r--r--   0        0        0       65 2023-05-18 13:11:38.458735 ynot3-1.0.0/ynot3/colors.py
--rw-r--r--   0        0        0    10389 2023-05-18 13:11:38.576735 ynot3-1.0.0/ynot3/gui.py
--rw-r--r--   0        0        0     8374 2023-05-18 13:11:38.557735 ynot3-1.0.0/ynot3/shapes.py
--rw-r--r--   0        0        0     1649 1970-01-01 00:00:00.000000 ynot3-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1192 2023-05-18 15:17:33.031978 ynot3-1.1.0/README.md
+-rw-r--r--   0        0        0      519 2023-05-18 15:20:25.869152 ynot3-1.1.0/pyproject.toml
+-rwxr-xr-x   0        0        0      314 2023-05-18 14:15:19.883304 ynot3-1.1.0/ynot3/__init__.py
+-rw-r--r--   0        0        0       65 2023-05-18 14:15:19.882304 ynot3-1.1.0/ynot3/colors.py
+-rw-r--r--   0        0        0    11031 2023-05-18 15:11:54.204595 ynot3-1.1.0/ynot3/gui.py
+-rw-r--r--   0        0        0     8858 2023-05-18 14:58:00.710692 ynot3-1.1.0/ynot3/shapes.py
+-rw-r--r--   0        0        0     1811 1970-01-01 00:00:00.000000 ynot3-1.1.0/PKG-INFO
```

### Comparing `ynot3-1.0.0/README.md` & `ynot3-1.1.0/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -3,37 +3,38 @@
 A simple image annotation program compatible with x11 and wayland.
 Targetting an efficient workflow and minimal dependencies.
 
 - can save to disk or copy to clipboard (requires `xclip` or `wl-copy`).
 - copy to clipboard on exit
 - unlimited undo
 - antialiasing
+- snapping for better alignments (override setting `SNAPPING` environment variable, defaults to 8)
 - very simple user interface
 
 Supported shapes:
 
 - enumerated bullets
 - rectangles
 - arrows
 
 ## Screenshot
 
-![](https://github.com/fdev31/ynot3/blob/0e68c2eca32b6ba8b324b9822a188fa9fce089ec/img/annotated.jpg)
+![](https://raw.githubusercontent.com/fdev31/ynot3/main/img/annotated.png)
 
 1. Active tool
     - *(4)* rectangle
     - *(5)* arrow
     - *(6)* enumerated bullet
 2. Active color
 3. Action buttons
-    - *(7)* undo
+    - *(7)* undo (shorcut: backspace)
     - *(8)* copy to clipboard
-    - *(9)* save to `/tmp/annotated.jpg`
+    - *(9)* save to `/tmp/annotated.jpg` (override setting `ANNOTATED` environment variable)
     - *(10)* toggle large mode (everything is magnified)
-    - *(11)* clear changes (remove all annotations)
+    - *(11)* clear changes (remove all annotations) (shortcut: "c")
 
 ## Example usage
 
 ### Edit an existing image
 
 `ynote3 ~/Images/example.jpg`
```

### Comparing `ynot3-1.0.0/pyproject.toml` & `ynot3-1.1.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ynot3"
-version = "1.0.0"
+version = "1.1.0"
 description = "An image annotator for Xorg & Wayland using pygame"
 authors = ["fdev31 <fdev31@gmail.com>"]
 license = "GPL"
 readme = "README.md"
 homepage = 'https://github.com/fdev31/ynot3'
 
 [tool.poetry.scripts]
```

### Comparing `ynot3-1.0.0/ynot3/gui.py` & `ynot3-1.1.0/ynot3/gui.py`

 * *Files 9% similar despite different names*

```diff
@@ -6,17 +6,28 @@
 
 from .colors import BLACK, WHITE, GREY
 from . import shapes
 
 STATUS_HEIGHT = 40
 DEFAULT_COLOR = (255, 255, 0)
 # Nice orange
-SELECTED_COLOR = (255, 128, 0)
+SELECTED_COLOR = (245, 130, 48)
 
-OUTPUT_FILENAME = "/tmp/annotated.jpg"
+OUTPUT_FILENAME = os.environ.get("ANNOTATED", "/tmp/annotated.jpg")
+
+
+class Snap:
+    level = int(os.environ.get("SNAPPING", 8))
+
+    @classmethod
+    def getSnapped(cls, coord):
+        l = cls.level
+        if not l:
+            return list(coord)
+        return [((l // 2 + coord[0]) // l) * l, ((l // 2 + coord[1]) // l) * l]
 
 
 class Icon:
     _index = 0
 
     def __init__(self, x, y, size):
         self.rect = pygame.Rect(x, y, size, size)
@@ -101,36 +112,40 @@
 
 
 class StatusBar:
     margin = 5
     separation = 20
     # List of distinctive colors
     available_colors = [
-        (255, 0, 0),
-        (0, 255, 0),
-        (0, 0, 255),
-        (0, 255, 255),
-        (255, 255, 0),
-        (255, 0, 255),
+        (128, 0, 0),
+        (230, 25, 75),
+        (255, 255, 25),
+        (60, 180, 75),
+        (70, 240, 240),
+        (240, 50, 230),
+        (0, 130, 200),
         (255, 255, 255),
         (0, 0, 0),
     ]
     available_shapes = shapes.all_shapes
 
     @classmethod
     def getHeight(cls, width, buttons):
         if cls.fitsScreen(width, buttons, 40):
             return 40
         return 20
 
     @classmethod
+    def estimateWidth(cls, buttons, icon_size):
+        nb_icons = len(buttons) + len(cls.available_colors) + len(cls.available_shapes)
+        return icon_size * nb_icons + cls.margin * (nb_icons - 4) + 2 * cls.separation
+
+    @classmethod
     def fitsScreen(cls, width, buttons, icon_size):
-        return not width < icon_size * (
-            len(buttons) + len(cls.available_colors) + len(cls.available_shapes)
-        ) + (cls.separation * 2)
+        return not width < cls.estimateWidth(buttons, icon_size)
 
     def __init__(self, screen, buttons=[]):
         self.screen = screen
         self.rect = pygame.Rect(0, 0, screen.get_width(), STATUS_HEIGHT)
         self.icon_size = STATUS_HEIGHT
         self.selected_color = DEFAULT_COLOR
         self.selected_shape = self.available_shapes[0]
@@ -177,28 +192,30 @@
             icon = self.icons[idx]
             pygame.draw.rect(self.screen, color, icon.rect, border_radius=radius)
             if icon.shape is None:
                 icon.shape = shape(
                     color=BLACK,
                     start=icon.rect.topleft,
                     end=icon.rect.bottomright,
-                    isFake=True,
+                    isDummy=True,
                 )
             icon.shape.draw(self.screen)
 
         for color in self.available_colors:
             idx = next(icon_counter)
             icon = self.icons[idx]
             if color == self.selected_color:
                 pygame.draw.rect(
                     self.screen, SELECTED_COLOR, icon.rect, border_radius=radius
                 )
-            pygame.draw.circle(
-                self.screen, color, icon.rect.center, icon.rect.width // 2 - 2
-            )
+            if not getattr(icon, "surface", None):
+                icon.surface = shapes.make_color_shape(
+                    color, icon.rect.width, icon.rect.height
+                )
+            self.screen.blit(icon.surface, icon.rect)
 
         for but in self.available_buttons:
             idx = next(icon_counter)
             icon = self.icons[idx]
             but.draw(self.screen, icon.rect)
 
     def handle_event(self, event):
@@ -226,53 +243,55 @@
             self.but_save,
             BigSmallBut(self),
             self.but_clear,
         ]
         bg_rect = background.get_rect()
         STATUS_HEIGHT = StatusBar.getHeight(bg_rect.width, buttons)
         self.screen = pygame.display.set_mode(
-            (bg_rect.width, bg_rect.height + STATUS_HEIGHT)
+            (
+                max(bg_rect.width, StatusBar.estimateWidth(buttons, STATUS_HEIGHT)),
+                bg_rect.height + STATUS_HEIGHT,
+            )
         )
 
         self.background = background.convert_alpha()
         self.status_bar = StatusBar(self.screen, buttons)
 
     def handle_event(self, event):
         if event.pos[1] < STATUS_HEIGHT:
             return self.status_bar.handle_event(event)
 
         if event.type == pygame.MOUSEBUTTONDOWN:
             if event.button == 1:  # left mouse button
                 self.dragging = True
 
                 # Add a shape to the list of shapes
-                start_pos = list(event.pos)
+                start_pos = Snap.getSnapped(event.pos)
                 start_pos[1] -= STATUS_HEIGHT
                 shape = self.status_bar.selected_shape(
                     color=self.status_bar.selected_color,
                     start=start_pos,
                     end=start_pos,
                 )
                 self.objects.append(shape)
         elif event.type == pygame.MOUSEBUTTONUP:
             if event.button == 1:  # left mouse button
                 if self.dragging:
-                    pos = list(event.pos)
+                    pos = Snap.getSnapped(event.pos)
                     pos[1] -= STATUS_HEIGHT
                     self.objects[-1].end = pos
                     self.dragging = False
         elif event.type == pygame.MOUSEMOTION:
             if self.dragging:
                 pos = list(event.pos)
                 pos[1] -= STATUS_HEIGHT
                 if self.objects:
                     self.objects[-1].end = pos
 
     def draw(self):
-        #         print("******************************************")
         self.status_bar.draw()
 
         surf = self.background.copy()
         self.canvas = surf
 
         for shape in self.objects:
             shape.draw(surf)
```

### Comparing `ynot3-1.0.0/ynot3/shapes.py` & `ynot3-1.1.0/ynot3/shapes.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,30 +5,40 @@
 
 WIDGET_SCALE = 1
 SUPERSAMPLE = 4
 
 OUTPUT_FILENAME = "/tmp/annotated.jpg"
 
 
+def make_color_shape(color: tuple[int, int, int], width: int, height: int):
+    w = width * SUPERSAMPLE
+    h = height * SUPERSAMPLE
+    surf = pygame.Surface((w, h), pygame.SRCALPHA)
+    surf.fill(list(color) + [0])
+    pygame.draw.circle(surf, (50, 50, 50), (w / 2 - 4, h / 2 + 4), int(0.4 * w))
+    pygame.draw.circle(surf, color, (w / 2, h / 2), int(0.4 * w))
+    return pygame.transform.smoothscale(surf, (width, height))
+
+
 class Shape:
     _name = "unknown"
     _surface = None
 
     def __init__(
         self,
         color: tuple[int, int, int],
         start: tuple[int, int],
         end: tuple[int, int],
-        isFake=False,
+        isDummy=False,
     ):
         self.name = self._name
         self.color = color
         self.start = start
         self.end = end
-        self.isFake = isFake
+        self.isDummy = isDummy
 
     @property
     def inv_color(self):
         r, g, b = self.color
 
         # Calculate relative luminance
         L = (0.2126 * r + 0.7152 * g + 0.0722 * b) / 255.0
@@ -69,27 +79,27 @@
     arrowhead_size = 20
     _name = "arrow"
     _old_pos = None
     _ssurface = None
 
     @property
     def fixed_size(self):
-        if self.isFake:
+        if self.isDummy:
             return self.arrowhead_size
         else:
             return self.arrowhead_size * WIDGET_SCALE
 
     def draw(self, surface):
         start = [SUPERSAMPLE * i for i in self.start]
         end = [SUPERSAMPLE * i for i in self.end]
 
         if not self._surface or self._old_pos != (start, end, WIDGET_SCALE):
             self._old_pos = (start, end, WIDGET_SCALE)
 
-            if self.isFake:
+            if self.isDummy:
                 # add some padding
                 end[0] -= 5
                 end[1] -= 5
                 start[0] += 10
                 start[1] += 10
 
             # Calculate the angle of the line from start to end
@@ -105,28 +115,28 @@
             # Calculate the endpoint of the line from start to end
             line_length = math.sqrt((end[1] - start[1]) ** 2 + (end[0] - start[0]) ** 2)
             end_point = (
                 int(start[0] + line_length * math.cos(angle)),
                 int(start[1] + line_length * math.sin(angle)),
             )
 
-            if self.isFake:
+            if self.isDummy:
                 sz = int(self.fixed_size * SUPERSAMPLE * 0.7)
             else:
                 sz = (
                     self.fixed_size
                     * SUPERSAMPLE
                     * (WIDGET_SCALE * 0.5 if WIDGET_SCALE > 1 else 1)
                 )
             # Draw a circle t point A
             pygame.draw.circle(
                 self._ssurface,
                 self.color,
                 start,
-                2 * (1 if self.isFake else WIDGET_SCALE * SUPERSAMPLE),
+                2 * (1 if self.isDummy else WIDGET_SCALE * SUPERSAMPLE),
             )
             # Draw the arrowhead at point B
             pygame.draw.polygon(
                 self._ssurface,
                 self.color,
                 (
                     (end_point[0], end_point[1]),
@@ -147,30 +157,30 @@
             )
             # Draw the line from start to end
             pygame.draw.line(
                 self._ssurface,
                 self.color,
                 start,
                 end_point,
-                self.thickness * (2 if self.isFake else WIDGET_SCALE * SUPERSAMPLE),
+                self.thickness * (2 if self.isDummy else WIDGET_SCALE * SUPERSAMPLE),
             )
             self._surface = pygame.transform.smoothscale(
                 self._ssurface, surface.get_size()
             )
         surface.blit(self._surface, (0, 0))
 
 
 class Bullet(Shape):
     _name = "bullet"
     size = 12
     _counter = 0
 
     def __init__(self, *a, **k):
         super().__init__(*a, **k)
-        if not self.isFake:
+        if not self.isDummy:
             Bullet._counter += 1
         self.counter = Bullet._counter
         self._old_scale = 0
         self._surface = None
 
     def instance_removed(self):
         Bullet._counter -= 1
@@ -186,20 +196,22 @@
 
     def draw(self, surface):
         if WIDGET_SCALE != self._old_scale:
             self._font = pygame.font.SysFont(
                 "Arial",
                 48
                 * (
-                    1 if self.isFake else (WIDGET_SCALE // 2 if WIDGET_SCALE > 1 else 1)
+                    1
+                    if self.isDummy
+                    else (WIDGET_SCALE // 2 if WIDGET_SCALE > 1 else 1)
                 ),
                 bold=True,
             )
             self.text = self._font.render(
-                "2" if self.isFake else str(self.counter), True, self.inv_color
+                "2" if self.isDummy else str(self.counter), True, self.inv_color
             )
             self._surface = None
 
         if not self._surface:
             border_sz = int(
                 SUPERSAMPLE * 3 * (WIDGET_SCALE * 0.5 if WIDGET_SCALE > 1 else 1)
             )
@@ -224,18 +236,18 @@
             )
 
             pos = list(corrected_rect.center)
             text_size = self.text.get_size()
             pos[0] -= text_size[0] // 2
             pos[1] -= text_size[1] // 2
             supersampled_surface.blit(self.text, pos)
-            sz = self.size * 2 - 2 if self.isFake else self.size * WIDGET_SCALE * 2
+            sz = self.size * 2 - 2 if self.isDummy else self.size * WIDGET_SCALE * 2
             self._surface = pygame.transform.smoothscale(supersampled_surface, (sz, sz))
 
-        if self.isFake:
+        if self.isDummy:
             surface.blit(self._surface, [i - 1 for i in self.rect.topleft])
         else:
             surface.blit(
                 self._surface,
                 (
                     self.start[0] - self.size * WIDGET_SCALE,
                     self.start[1] - self.size * WIDGET_SCALE,
@@ -244,27 +256,27 @@
 
 
 class Rectangle(Shape):
     _name = "rectangle"
     thickness = 3
 
     def draw(self, surface):
-        if self.isFake:
+        if self.isDummy:
             rect = self.rect.copy()
             rect.width -= 3
             rect.height -= 3
             rect.x += 2
             rect.y += 2
             pygame.draw.rect(surface, self.color, rect, width=2)
         else:
             pygame.draw.rect(
                 surface,
                 self.color,
                 self.rect,
-                width=1 if self.isFake else self.thickness * WIDGET_SCALE,
+                width=1 if self.isDummy else self.thickness * WIDGET_SCALE,
             )
 
     @property
     def rect(self):
         x = min(self.start[0], self.end[0])
         y = min(self.start[1], self.end[1])
         width = max(self.start[0], self.end[0]) - x
```

### Comparing `ynot3-1.0.0/PKG-INFO` & `ynot3-1.1.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ynot3
-Version: 1.0.0
+Version: 1.1.0
 Summary: An image annotator for Xorg & Wayland using pygame
 Home-page: https://github.com/fdev31/ynot3
 License: GPL
 Author: fdev31
 Author-email: fdev31@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: Other/Proprietary License
@@ -21,37 +21,38 @@
 A simple image annotation program compatible with x11 and wayland.
 Targetting an efficient workflow and minimal dependencies.
 
 - can save to disk or copy to clipboard (requires `xclip` or `wl-copy`).
 - copy to clipboard on exit
 - unlimited undo
 - antialiasing
+- snapping for better alignments (override setting `SNAPPING` environment variable, defaults to 8)
 - very simple user interface
 
 Supported shapes:
 
 - enumerated bullets
 - rectangles
 - arrows
 
 ## Screenshot
 
-![](https://github.com/fdev31/ynot3/blob/0e68c2eca32b6ba8b324b9822a188fa9fce089ec/img/annotated.jpg)
+![](https://raw.githubusercontent.com/fdev31/ynot3/main/img/annotated.png)
 
 1. Active tool
     - *(4)* rectangle
     - *(5)* arrow
     - *(6)* enumerated bullet
 2. Active color
 3. Action buttons
-    - *(7)* undo
+    - *(7)* undo (shorcut: backspace)
     - *(8)* copy to clipboard
-    - *(9)* save to `/tmp/annotated.jpg`
+    - *(9)* save to `/tmp/annotated.jpg` (override setting `ANNOTATED` environment variable)
     - *(10)* toggle large mode (everything is magnified)
-    - *(11)* clear changes (remove all annotations)
+    - *(11)* clear changes (remove all annotations) (shortcut: "c")
 
 ## Example usage
 
 ### Edit an existing image
 
 `ynote3 ~/Images/example.jpg`
```

