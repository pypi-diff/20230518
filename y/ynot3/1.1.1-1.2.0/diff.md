# Comparing `tmp/ynot3-1.1.1.tar.gz` & `tmp/ynot3-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ynot3-1.1.1.tar", max compression
+gzip compressed data, was "ynot3-1.2.0.tar", max compression
```

## Comparing `ynot3-1.1.1.tar` & `ynot3-1.2.0.tar`

### file list

```diff
@@ -1,7 +1,9 @@
--rw-r--r--   0        0        0     1192 2023-05-18 15:17:33.031978 ynot3-1.1.1/README.md
--rw-r--r--   0        0        0      519 2023-05-18 16:31:23.142507 ynot3-1.1.1/pyproject.toml
--rwxr-xr-x   0        0        0      314 2023-05-18 14:15:19.883304 ynot3-1.1.1/ynot3/__init__.py
--rw-r--r--   0        0        0       65 2023-05-18 14:15:19.882304 ynot3-1.1.1/ynot3/colors.py
--rw-r--r--   0        0        0    11032 2023-05-18 15:40:18.417223 ynot3-1.1.1/ynot3/gui.py
--rw-r--r--   0        0        0     8908 2023-05-18 16:30:03.309520 ynot3-1.1.1/ynot3/shapes.py
--rw-r--r--   0        0        0     1811 1970-01-01 00:00:00.000000 ynot3-1.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1350 2023-05-18 19:29:49.320047 ynot3-1.2.0/README.md
+-rw-r--r--   0        0        0      519 2023-05-18 20:16:58.078068 ynot3-1.2.0/pyproject.toml
+-rwxr-xr-x   0        0        0      314 2023-05-18 14:15:19.883304 ynot3-1.2.0/ynot3/__init__.py
+-rw-r--r--   0        0        0     1825 2023-05-18 19:22:49.567659 ynot3-1.2.0/ynot3/buttons.py
+-rw-r--r--   0        0        0       98 2023-05-18 16:40:19.175539 ynot3-1.2.0/ynot3/colors.py
+-rw-r--r--   0        0        0     6285 2023-05-18 20:13:22.260232 ynot3-1.2.0/ynot3/gui.py
+-rw-r--r--   0        0        0    10535 2023-05-18 20:04:39.656987 ynot3-1.2.0/ynot3/shapes.py
+-rw-r--r--   0        0        0     4702 2023-05-18 20:07:56.321133 ynot3-1.2.0/ynot3/widgets.py
+-rw-r--r--   0        0        0     1969 1970-01-01 00:00:00.000000 ynot3-1.2.0/PKG-INFO
```

### Comparing `ynot3-1.1.1/pyproject.toml` & `ynot3-1.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ynot3"
-version = "1.1.1"
+version = "1.2.0"
 description = "An image annotator for Xorg & Wayland using pygame"
 authors = ["fdev31 <fdev31@gmail.com>"]
 license = "GPL"
 readme = "README.md"
 homepage = 'https://github.com/fdev31/ynot3'
 
 [tool.poetry.scripts]
```

### Comparing `ynot3-1.1.1/ynot3/gui.py` & `ynot3-1.2.0/ynot3/shapes.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,353 +1,322 @@
-import os
-import io
+import math
 import pygame
-import itertools
-import subprocess
 
-from .colors import BLACK, WHITE, GREY
-from . import shapes
+from .colors import BLACK, WHITE
 
-STATUS_HEIGHT = 40
-DEFAULT_COLOR = (255, 255, 25)
-# Nice orange
-SELECTED_COLOR = (245, 130, 48)
+WIDGET_SCALE = 1
+SUPERSAMPLE = 4
 
-OUTPUT_FILENAME = os.environ.get("ANNOTATED", "/tmp/annotated.jpg")
+OUTPUT_FILENAME = "/tmp/annotated.jpg"
 
 
-class Snap:
-    level = int(os.environ.get("SNAPPING", 8))
-
-    @classmethod
-    def getSnapped(cls, coord):
-        l = cls.level
-        if not l:
-            return list(coord)
-        return [((l // 2 + coord[0]) // l) * l, ((l // 2 + coord[1]) // l) * l]
-
-
-class Icon:
-    _index = 0
-
-    def __init__(self, x, y, size):
-        self.rect = pygame.Rect(x, y, size, size)
-        self.index = Icon._index
-        Icon._index += 1
-        self.shape = None
-
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
+class Shape:
+    _name = "unknown"
+    _surface = None
+    shadow = (3 * SUPERSAMPLE, 3 * SUPERSAMPLE)
+    shadow_color = (50, 50, 50, 200)
+
+    def __init__(
+        self,
+        color: tuple[int, int, int] | list[int],
+        start: tuple[int, int] | list[int],
+        end: tuple[int, int] | list[int],
+        isDummy=False,
+    ):
+        self.color = color
+        self.start = start
+        self.end = end
+        self.isDummy = isDummy
+
+    @property
+    def inv_color(self):
+        r, g, b = self.color
+
+        # Calculate relative luminance
+        L = (0.2126 * r + 0.7152 * g + 0.0722 * b) / 255.0
+
+        # Choose white or black text color based on luminance
+        if L > 0.5:
+            return BLACK
+        else:
+            return WHITE
 
-class Button:
-    def __init__(self, gui, label="X"):
-        self.gui = gui
-        font = pygame.font.SysFont("Symbols Nerd Font", 20)
-        self.text = font.render(label, True, BLACK)
-        self.bg = GREY
+    @property
+    def rect(self):
+        return pygame.Rect(
+            self.start, (self.end[0] - self.start[0], self.end[1] - self.start[1])
+        )
 
-    def draw(self, surface, rect):
-        pygame.draw.rect(surface, self.bg, rect, border_radius=5)
-        sz = self.text.get_size()
-        pos = tuple((rect.center[0] - sz[0] // 2, rect.center[1] - sz[1] // 2))
-        surface.blit(self.text, pos)
+    def draw(self, surface: pygame.Surface):
+        raise NotImplementedError(
+            "Missing draw implementation for the {} class.".format(self._name)
+        )
 
+    def instance_removed(self):
+        pass
 
-class BigSmallBut(Button):
-    def __init__(self, gui):
-        super().__init__(gui, "󰧴")
 
-    def execute(self):
-        if shapes.WIDGET_SCALE == 1:
-            shapes.WIDGET_SCALE = 2
-            self.bg = SELECTED_COLOR
+class Arrow(Shape):
+    thickness = 5
+    arrowhead_size = 20
+    _name = "arrow"
+    _old_pos = None
+    _ssurface = None
+
+    @property
+    def fixed_size(self):
+        if self.isDummy:
+            return self.arrowhead_size
         else:
-            shapes.WIDGET_SCALE = 1
-            self.bg = GREY
+            return self.arrowhead_size * WIDGET_SCALE
 
+    def draw(self, surface):
+        start = [SUPERSAMPLE * i for i in self.start]
+        end = [SUPERSAMPLE * i for i in self.end]
+
+        if not self._surface or self._old_pos != (start, end, WIDGET_SCALE):
+            self._old_pos = (start, end, WIDGET_SCALE)
+
+            if self.isDummy:
+                # add some padding
+                end[0] -= 5
+                end[1] -= 5
+                start[0] += 10
+                start[1] += 10
+
+            # Calculate the angle of the line from start to end
+            angle = math.atan2(end[1] - start[1], end[0] - start[0])
+            if not self._ssurface:
+                supersampled_surface = pygame.Surface(
+                    tuple(SUPERSAMPLE * i for i in surface.get_size()), pygame.SRCALPHA
+                )
+                self._ssurface = supersampled_surface
+            else:
+                self._ssurface.fill(list(self.color) + [0])
 
-class SaveBut(Button):
-    def __init__(self, gui):
-        super().__init__(gui, "")
+            # Calculate the endpoint of the line from start to end
+            line_length = math.sqrt((end[1] - start[1]) ** 2 + (end[0] - start[0]) ** 2)
+            end_point = (
+                int(start[0] + line_length * math.cos(angle)),
+                int(start[1] + line_length * math.sin(angle)),
+            )
 
-    def execute(self):
-        pygame.image.save(self.gui.canvas, OUTPUT_FILENAME)
+            if self.isDummy:
+                sz = int(self.fixed_size * SUPERSAMPLE * 0.7)
+            else:
+                sz = (
+                    self.fixed_size
+                    * SUPERSAMPLE
+                    * (WIDGET_SCALE * 0.5 if WIDGET_SCALE > 1 else 1)
+                )
+            # shadow
+            if not self.isDummy:
+                pygame.draw.polygon(
+                    self._ssurface,
+                    self.shadow_color,
+                    (
+                        end_point,
+                        (
+                            (end_point[0] - sz * math.cos(angle - math.pi / 6))
+                            - self.shadow[0],
+                            (end_point[1] - sz * math.sin(angle - math.pi / 6))
+                            + self.shadow[1],
+                        ),
+                        (
+                            (end_point[0] - sz * math.cos(angle + math.pi / 6))
+                            - self.shadow[0],
+                            (end_point[1] - sz * math.sin(angle + math.pi / 6))
+                            + self.shadow[1],
+                        ),
+                    ),
+                )
+                sline_length = line_length - (sz // 2)
+                send_point = (
+                    int(start[0] - self.shadow[0] + sline_length * math.cos(angle)),
+                    int(start[1] + self.shadow[1] + sline_length * math.sin(angle)),
+                )
+                # Draw the line from start to end
+                pygame.draw.line(
+                    self._ssurface,
+                    self.shadow_color,
+                    start,
+                    send_point,
+                    self.thickness * WIDGET_SCALE * SUPERSAMPLE + 5,
+                )
+            # real shape
+            # Draw a circle t point A
+            pygame.draw.circle(
+                self._ssurface,
+                self.color,
+                start,
+                2 * (1 if self.isDummy else WIDGET_SCALE * SUPERSAMPLE),
+            )
+            # Draw the arrowhead at point B
+            pygame.draw.polygon(
+                self._ssurface,
+                self.color,
+                (
+                    (end_point[0], end_point[1]),
+                    (
+                        end_point[0] - sz * math.cos(angle - math.pi / 6),
+                        end_point[1] - sz * math.sin(angle - math.pi / 6),
+                    ),
+                    (
+                        end_point[0] - sz * math.cos(angle + math.pi / 6),
+                        end_point[1] - sz * math.sin(angle + math.pi / 6),
+                    ),
+                ),
+            )
+            line_length -= sz // 2
+            end_point = (
+                int(start[0] + line_length * math.cos(angle)),
+                int(start[1] + line_length * math.sin(angle)),
+            )
+            # Draw the line from start to end
+            pygame.draw.line(
+                self._ssurface,
+                self.color,
+                start,
+                end_point,
+                self.thickness * (2 if self.isDummy else WIDGET_SCALE * SUPERSAMPLE),
+            )
+            self._surface = pygame.transform.smoothscale(
+                self._ssurface, surface.get_size()
+            )
+        surface.blit(self._surface, (0, 0))
 
 
-class CopyBut(Button):
-    def __init__(self, gui):
-        super().__init__(gui, "")
+class Bullet(Shape):
+    _name = "bullet"
+    size = 12
+    _counter = 0
+
+    def __init__(self, *a, **k):
+        super().__init__(*a, **k)
+        if not self.isDummy:
+            Bullet._counter += 1
+        self.counter = Bullet._counter
+        self._old_scale = 0
+        self._surface = None
+
+    def instance_removed(self):
+        Bullet._counter -= 1
+
+    @property
+    def corrected_size(self):
+        return self.size * SUPERSAMPLE
+
+    def draw(self, surface):
+        if WIDGET_SCALE != self._old_scale:
+            self._font = pygame.font.SysFont(
+                "Arial",
+                48
+                * (
+                    1
+                    if self.isDummy
+                    else (WIDGET_SCALE // 2 if WIDGET_SCALE > 1 else 1)
+                ),
+                bold=True,
+            )
+            self.text = self._font.render(
+                "2" if self.isDummy else str(self.counter), True, self.inv_color
+            )
+            self._surface = None
 
-    def execute(self):
-        if os.environ.get("WAYLAND_DISPLAY"):
-            proc = subprocess.Popen(
-                ["wl-copy", "-t", "image/png"], stdin=subprocess.PIPE
+        if not self._surface:
+            border_sz = int(
+                SUPERSAMPLE * 3 * (WIDGET_SCALE * 0.5 if WIDGET_SCALE > 1 else 1)
             )
-        else:
-            proc = subprocess.Popen(
-                ["xclip", "-selection", "clipboard", "-t", "image/png"],
-                stdin=subprocess.PIPE,
-            )
-        buffer = io.BytesIO()
-        pygame.image.save(self.gui.canvas, buffer, "png")
-        proc.communicate(input=buffer.getvalue())
-
-
-class BackBut(Button):
-    def __init__(self, gui):
-        super().__init__(gui, "󰕌")
-
-    def execute(self):
-        if self.gui.objects:
-            self.gui.objects[-1].instance_removed()
-            self.gui.objects = self.gui.objects[:-1]
-
-
-class ClearBut(Button):
-    def __init__(self, gui):
-        super().__init__(gui, "󰗩")
-
-    def execute(self):
-        for obj in self.gui.objects:
-            obj.instance_removed()
-            # Clear all the shapes
-        self.gui.objects = []
-
-
-class StatusBar:
-    margin = 5
-    separation = 20
-    # List of distinctive colors
-    available_colors = [
-        (128, 0, 0),
-        (230, 25, 75),
-        (255, 255, 25),
-        (60, 180, 75),
-        (70, 240, 240),
-        (240, 50, 230),
-        (0, 130, 200),
-        (255, 255, 255),
-        (0, 0, 0),
-    ]
-    available_shapes = shapes.all_shapes
-
-    @classmethod
-    def getHeight(cls, width, buttons):
-        if cls.fitsScreen(width, buttons, 40):
-            return 40
-        return 20
-
-    @classmethod
-    def estimateWidth(cls, buttons, icon_size):
-        nb_icons = len(buttons) + len(cls.available_colors) + len(cls.available_shapes)
-        return icon_size * nb_icons + cls.margin * (nb_icons - 4) + 2 * cls.separation
-
-    @classmethod
-    def fitsScreen(cls, width, buttons, icon_size):
-        return not width < cls.estimateWidth(buttons, icon_size)
-
-    def __init__(self, screen, buttons=[]):
-        self.screen = screen
-        self.rect = pygame.Rect(0, 0, screen.get_width(), STATUS_HEIGHT)
-        self.icon_size = STATUS_HEIGHT
-        self.selected_color = DEFAULT_COLOR
-        self.selected_shape = self.available_shapes[0]
-        self.available_buttons = buttons
-
-        x_offset = self.margin
-
-        self.icons = []
-        for _ in self.available_shapes:
-            self.icons.append(Icon(x_offset, 0, self.icon_size))
-            x_offset += self.icon_size + self.margin
-
-        x_offset += self.separation
-        for _ in self.available_colors:
-            self.icons.append(Icon(x_offset, 0, self.icon_size))
-            x_offset += self.icon_size
-
-        x_offset += self.separation
-        for _ in self.available_buttons:
-            self.icons.append(Icon(x_offset, 0, self.icon_size))
-            x_offset += self.icon_size + self.margin
-
-    def icon_action(self, index):
-        nbs = len(self.available_shapes)
-        nbc = len(self.available_colors)
-        if index < nbs:
-            self.selected_shape = self.available_shapes[index]
-        elif index < nbs + nbc:
-            self.selected_color = self.available_colors[index - nbs]
-        else:
-            self.available_buttons[index - nbs - nbc].execute()
+            side = max(self.text.get_size()[0] + 10, self.corrected_size) + border_sz
 
-    def draw(self):
-        # Draw the status bar background
-        pygame.draw.rect(self.screen, GREY, self.rect)
-
-        icon_counter = itertools.count(0)
-
-        radius = 3
-
-        for shape in self.available_shapes:
-            color = SELECTED_COLOR if shape == self.selected_shape else GREY
-            idx = next(icon_counter)
-            icon = self.icons[idx]
-            pygame.draw.rect(self.screen, color, icon.rect, border_radius=radius)
-            if icon.shape is None:
-                icon.shape = shape(
-                    color=BLACK,
-                    start=icon.rect.topleft,
-                    end=icon.rect.bottomright,
-                    isDummy=True,
+            supersampled_surface = pygame.Surface(
+                (side + border_sz, side + border_sz), pygame.SRCALPHA
+            )
+            supersampled_surface.fill(list(self.inv_color) + [0])
+            corrected_rect = pygame.Rect(0, 0, side, side)
+            corrected_rect[0] += border_sz // 2
+            corrected_rect[1] += border_sz // 2
+
+            if not self.isDummy:  # draw shadow
+                pygame.draw.circle(
+                    supersampled_surface,
+                    self.shadow_color,
+                    (corrected_rect.center[0] - 4, corrected_rect.center[1] + 4),
+                    (side // 2),
                 )
-            icon.shape.draw(self.screen)
+            pygame.draw.circle(
+                supersampled_surface, self.inv_color, corrected_rect.center, (side // 2)
+            )
+            pygame.draw.circle(
+                supersampled_surface,
+                self.color,
+                corrected_rect.center,
+                (side - border_sz) // 2,
+            )
 
-        for color in self.available_colors:
-            idx = next(icon_counter)
-            icon = self.icons[idx]
-            if color == self.selected_color:
-                pygame.draw.rect(
-                    self.screen, SELECTED_COLOR, icon.rect, border_radius=radius
-                )
-            if not getattr(icon, "surface", None):
-                icon.surface = shapes.make_color_shape(
-                    color, icon.rect.width, icon.rect.height
-                )
-            self.screen.blit(icon.surface, icon.rect)
+            pos = list(corrected_rect.center)
+            text_size = self.text.get_size()
+            pos[0] -= text_size[0] // 2
+            pos[1] -= text_size[1] // 2
+            supersampled_surface.blit(self.text, pos)
+            sz = self.rect.size[0] if self.isDummy else (self.size * WIDGET_SCALE * 2)
+            self._surface = pygame.transform.smoothscale(supersampled_surface, (sz, sz))
+
+        if self.isDummy:
+            surface.blit(
+                self._surface, [i - self.rect.width // 2 for i in self.rect.center]
+            )
+        else:
+            surface.blit(
+                self._surface,
+                (
+                    self.start[0] - self.size * WIDGET_SCALE,
+                    self.start[1] - self.size * WIDGET_SCALE,
+                ),
+            )
 
-        for but in self.available_buttons:
-            idx = next(icon_counter)
-            icon = self.icons[idx]
-            but.draw(self.screen, icon.rect)
-
-    def handle_event(self, event):
-        if event.type == pygame.MOUSEBUTTONDOWN and event.button == 1:
-            for idx, shape in enumerate(self.icons):
-                # detect if shape is under cursor
-                if shape.rect.collidepoint(event.pos):
-                    self.icon_action(idx)
-                    break
-
-
-class GUI:
-    def __init__(self, background):
-        global STATUS_HEIGHT
-        self.objects: list[shapes.Shape] = []
-        self.dragging = False
-        self.canvas: None | pygame.Surface = None
-        self.but_undo = BackBut(self)
-        self.but_save = SaveBut(self)
-        self.but_clear = ClearBut(self)
-        self.but_copy = CopyBut(self)
-        buttons = [
-            self.but_undo,
-            self.but_copy,
-            self.but_save,
-            BigSmallBut(self),
-            self.but_clear,
-        ]
-        bg_rect = background.get_rect()
-        STATUS_HEIGHT = StatusBar.getHeight(bg_rect.width, buttons)
-        self.screen = pygame.display.set_mode(
-            (
-                max(bg_rect.width, StatusBar.estimateWidth(buttons, STATUS_HEIGHT)),
-                bg_rect.height + STATUS_HEIGHT,
+
+class Rectangle(Shape):
+    _name = "rectangle"
+    thickness = 3
+
+    def draw(self, surface):
+        if self.isDummy:
+            rect = self.rect.copy()
+            rect.width -= 6
+            rect.height -= 6
+            rect.x += 3
+            rect.y += 3
+            pygame.draw.rect(surface, self.color, rect, width=2)
+        else:
+            pygame.draw.rect(
+                surface,
+                list(self.color) + [50],
+                self.rect,
+            )
+            pygame.draw.rect(
+                surface,
+                self.color,
+                self.rect,
+                width=1 if self.isDummy else self.thickness * WIDGET_SCALE,
             )
-        )
 
-        self.background = background.convert_alpha()
-        self.status_bar = StatusBar(self.screen, buttons)
+    @property
+    def rect(self):
+        x = min(self.start[0], self.end[0])
+        y = min(self.start[1], self.end[1])
+        width = max(self.start[0], self.end[0]) - x
+        height = max(self.start[1], self.end[1]) - y
+        return pygame.Rect(x, y, width, height)
 
-    def handle_event(self, event):
-        if event.pos[1] < STATUS_HEIGHT:
-            return self.status_bar.handle_event(event)
-
-        if event.type == pygame.MOUSEBUTTONDOWN:
-            if event.button == 1:  # left mouse button
-                self.dragging = True
-
-                # Add a shape to the list of shapes
-                start_pos = Snap.getSnapped(event.pos)
-                start_pos[1] -= STATUS_HEIGHT
-                shape = self.status_bar.selected_shape(
-                    color=self.status_bar.selected_color,
-                    start=start_pos,
-                    end=start_pos,
-                )
-                self.objects.append(shape)
-        elif event.type == pygame.MOUSEBUTTONUP:
-            if event.button == 1:  # left mouse button
-                if self.dragging:
-                    pos = Snap.getSnapped(event.pos)
-                    pos[1] -= STATUS_HEIGHT
-                    self.objects[-1].end = pos
-                    self.dragging = False
-        elif event.type == pygame.MOUSEMOTION:
-            if self.dragging:
-                pos = list(event.pos)
-                pos[1] -= STATUS_HEIGHT
-                if self.objects:
-                    self.objects[-1].end = pos
-
-    def draw(self):
-        self.status_bar.draw()
-
-        surf = self.background.copy()
-        self.canvas = surf
-
-        for shape in self.objects:
-            shape.draw(surf)
-        self.screen.blit(surf, (0, STATUS_HEIGHT))
-
-        pygame.display.update()
-
-
-def main(image_path: str):
-    pygame.init()
-    pygame.display.set_caption("Draw Shapes")
-
-    background = pygame.image.load(image_path)
-
-    # Create the GUI
-    gui = GUI(background)
-
-    clock = pygame.time.Clock()
-    # Game loop
-    running = True
-    while running:
-        # Handle events
-        for event in pygame.event.get():
-            if event.type == pygame.QUIT:
-                running = False
-            else:
-                if event.type in (
-                    pygame.MOUSEBUTTONDOWN,
-                    pygame.MOUSEBUTTONUP,
-                    pygame.MOUSEMOTION,
-                    pygame.BUTTON_WHEELDOWN,
-                    pygame.BUTTON_WHEELUP,
-                ):
-                    gui.handle_event(event)
-                else:
-                    if event.type == pygame.KEYDOWN:
-                        if event.key == pygame.K_s:
-                            gui.but_save.execute()
-                        elif event.key == pygame.K_ESCAPE:
-                            running = False
-                        elif event.key == pygame.K_c:
-                            gui.but_clear.execute()
-                        elif event.key == pygame.K_BACKSPACE:
-                            gui.but_undo.execute()
-                        elif event.key == pygame.K_r:
-                            gui.status_bar.selected_shape = shapes.Rectangle
-                        elif event.key == pygame.K_a:
-                            gui.status_bar.selected_shape = shapes.Arrow
-                        elif event.key == pygame.K_e:
-                            gui.status_bar.selected_shape = shapes.Bullet
-
-        # Update the screen
-        gui.draw()
-        clock.tick(60)
-        pygame.display.flip()
-
-    gui.but_copy.execute()
-    # Quit pygame
-    pygame.quit()
+
+all_shapes = [Rectangle, Arrow, Bullet]
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `ynot3-1.1.1/PKG-INFO` & `ynot3-1.2.0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ynot3
-Version: 1.1.1
+Version: 1.2.0
 Summary: An image annotator for Xorg & Wayland using pygame
 Home-page: https://github.com/fdev31/ynot3
 License: GPL
 Author: fdev31
 Author-email: fdev31@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: Other/Proprietary License
@@ -30,30 +30,44 @@
 
 Supported shapes:
 
 - enumerated bullets
 - rectangles
 - arrows
 
-## Screenshot
+## Documentation / annotation example
 
 ![](https://raw.githubusercontent.com/fdev31/ynot3/main/img/annotated.png)
 
 1. Active tool
     - *(4)* rectangle
     - *(5)* arrow
     - *(6)* enumerated bullet
 2. Active color
 3. Action buttons
     - *(7)* undo (shorcut: backspace)
-    - *(8)* copy to clipboard
-    - *(9)* save to `/tmp/annotated.jpg` (override setting `ANNOTATED` environment variable)
+    - *(8)* copy to clipboard (automatic on exit)
+    - *(9)* save to `/tmp/annotated.jpg` (shortcut: "s")
+        - override setting the `ANNOTATED` environment variable
     - *(10)* toggle large mode (everything is magnified)
     - *(11)* clear changes (remove all annotations) (shortcut: "c")
 
+
+## Installation
+
+```
+pip install ynot3
+```
+
+Or, on Archlinux:
+
+```
+yay -S ynot3
+```
+
 ## Example usage
 
 ### Edit an existing image
 
 `ynote3 ~/Images/example.jpg`
 
 ### Edit a screenshot
```

