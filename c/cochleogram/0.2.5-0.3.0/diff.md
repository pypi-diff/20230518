# Comparing `tmp/cochleogram-0.2.5.tar.gz` & `tmp/cochleogram-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cochleogram-0.2.5.tar", last modified: Wed May 17 00:08:06 2023, max compression
+gzip compressed data, was "cochleogram-0.3.0.tar", last modified: Wed May 17 22:04:44 2023, max compression
```

## Comparing `cochleogram-0.2.5.tar` & `cochleogram-0.3.0.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 00:08:06.342863 cochleogram-0.2.5/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 00:08:06.338863 cochleogram-0.2.5/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 00:08:06.338863 cochleogram-0.2.5/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-05-17 00:07:56.000000 cochleogram-0.2.5/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3146 2023-05-17 00:07:56.000000 cochleogram-0.2.5/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     6629 2023-05-17 00:08:06.342863 cochleogram-0.2.5/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 00:08:06.338863 cochleogram-0.2.5/cochleogram/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 00:07:56.000000 cochleogram-0.2.5/cochleogram/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21110 2023-05-17 00:07:56.000000 cochleogram-0.2.5/cochleogram/gui.enaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 00:08:06.342863 cochleogram-0.2.5/cochleogram/icons/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 00:07:56.000000 cochleogram-0.2.5/cochleogram/icons/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-05-17 00:07:56.000000 cochleogram-0.2.5/cochleogram/icons/cells.png
--rw-r--r--   0 runner    (1001) docker     (123)     1913 2023-05-17 00:07:56.000000 cochleogram-0.2.5/cochleogram/icons/exclude.png
--rw-r--r--   0 runner    (1001) docker     (123)     5707 2023-05-17 00:07:56.000000 cochleogram-0.2.5/cochleogram/icons/main-icon.png
--rw-r--r--   0 runner    (1001) docker     (123)     2808 2023-05-17 00:07:56.000000 cochleogram-0.2.5/cochleogram/icons/make_icons.py
--rw-r--r--   0 runner    (1001) docker     (123)     3175 2023-05-17 00:07:56.000000 cochleogram-0.2.5/cochleogram/icons/spiral.png
--rw-r--r--   0 runner    (1001) docker     (123)      678 2023-05-17 00:07:56.000000 cochleogram-0.2.5/cochleogram/icons/tile.png
--rw-r--r--   0 runner    (1001) docker     (123)    23257 2023-05-17 00:07:56.000000 cochleogram-0.2.5/cochleogram/instructions.html
--rw-r--r--   0 runner    (1001) docker     (123)     2618 2023-05-17 00:07:56.000000 cochleogram-0.2.5/cochleogram/main.py
--rw-r--r--   0 runner    (1001) docker     (123)    21136 2023-05-17 00:07:56.000000 cochleogram-0.2.5/cochleogram/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2595 2023-05-17 00:07:56.000000 cochleogram-0.2.5/cochleogram/plot.py
--rw-r--r--   0 runner    (1001) docker     (123)    26608 2023-05-17 00:07:56.000000 cochleogram-0.2.5/cochleogram/presenter.py
--rw-r--r--   0 runner    (1001) docker     (123)     5547 2023-05-17 00:07:56.000000 cochleogram-0.2.5/cochleogram/readers.py
--rw-r--r--   0 runner    (1001) docker     (123)    14237 2023-05-17 00:07:56.000000 cochleogram-0.2.5/cochleogram/util.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-17 00:08:06.000000 cochleogram-0.2.5/cochleogram/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 00:08:06.338863 cochleogram-0.2.5/cochleogram.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6629 2023-05-17 00:08:06.000000 cochleogram-0.2.5/cochleogram.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      738 2023-05-17 00:08:06.000000 cochleogram-0.2.5/cochleogram.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 00:08:06.000000 cochleogram-0.2.5/cochleogram.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-05-17 00:08:06.000000 cochleogram-0.2.5/cochleogram.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-05-17 00:08:06.000000 cochleogram-0.2.5/cochleogram.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-17 00:08:06.000000 cochleogram-0.2.5/cochleogram.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-05-17 00:07:56.000000 cochleogram-0.2.5/development.rst
--rw-r--r--   0 runner    (1001) docker     (123)      950 2023-05-17 00:07:56.000000 cochleogram-0.2.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     6302 2023-05-17 00:07:56.000000 cochleogram-0.2.5/readme.rst
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-17 00:08:06.342863 cochleogram-0.2.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:04:44.484983 cochleogram-0.3.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:04:44.480983 cochleogram-0.3.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:04:44.480983 cochleogram-0.3.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-05-17 22:04:31.000000 cochleogram-0.3.0/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3146 2023-05-17 22:04:31.000000 cochleogram-0.3.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     6629 2023-05-17 22:04:44.484983 cochleogram-0.3.0/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:04:44.480983 cochleogram-0.3.0/cochleogram/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 22:04:31.000000 cochleogram-0.3.0/cochleogram/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23363 2023-05-17 22:04:31.000000 cochleogram-0.3.0/cochleogram/gui.enaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:04:44.484983 cochleogram-0.3.0/cochleogram/icons/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 22:04:31.000000 cochleogram-0.3.0/cochleogram/icons/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-05-17 22:04:31.000000 cochleogram-0.3.0/cochleogram/icons/cells.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1913 2023-05-17 22:04:31.000000 cochleogram-0.3.0/cochleogram/icons/exclude.png
+-rw-r--r--   0 runner    (1001) docker     (123)     5707 2023-05-17 22:04:31.000000 cochleogram-0.3.0/cochleogram/icons/main-icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2808 2023-05-17 22:04:31.000000 cochleogram-0.3.0/cochleogram/icons/make_icons.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3175 2023-05-17 22:04:31.000000 cochleogram-0.3.0/cochleogram/icons/spiral.png
+-rw-r--r--   0 runner    (1001) docker     (123)      678 2023-05-17 22:04:31.000000 cochleogram-0.3.0/cochleogram/icons/tile.png
+-rw-r--r--   0 runner    (1001) docker     (123)    23257 2023-05-17 22:04:31.000000 cochleogram-0.3.0/cochleogram/instructions.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2598 2023-05-17 22:04:31.000000 cochleogram-0.3.0/cochleogram/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23013 2023-05-17 22:04:31.000000 cochleogram-0.3.0/cochleogram/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2903 2023-05-17 22:04:31.000000 cochleogram-0.3.0/cochleogram/plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27793 2023-05-17 22:04:31.000000 cochleogram-0.3.0/cochleogram/presenter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5727 2023-05-17 22:04:31.000000 cochleogram-0.3.0/cochleogram/readers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14237 2023-05-17 22:04:31.000000 cochleogram-0.3.0/cochleogram/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-17 22:04:44.000000 cochleogram-0.3.0/cochleogram/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:04:44.484983 cochleogram-0.3.0/cochleogram.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6629 2023-05-17 22:04:44.000000 cochleogram-0.3.0/cochleogram.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      738 2023-05-17 22:04:44.000000 cochleogram-0.3.0/cochleogram.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 22:04:44.000000 cochleogram-0.3.0/cochleogram.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-05-17 22:04:44.000000 cochleogram-0.3.0/cochleogram.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-05-17 22:04:44.000000 cochleogram-0.3.0/cochleogram.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-17 22:04:44.000000 cochleogram-0.3.0/cochleogram.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-05-17 22:04:31.000000 cochleogram-0.3.0/development.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      950 2023-05-17 22:04:31.000000 cochleogram-0.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     6302 2023-05-17 22:04:31.000000 cochleogram-0.3.0/readme.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-17 22:04:44.484983 cochleogram-0.3.0/setup.cfg
```

### Comparing `cochleogram-0.2.5/.github/workflows/publish-to-pypi.yml` & `cochleogram-0.3.0/.github/workflows/publish-to-pypi.yml`

 * *Files identical despite different names*

### Comparing `cochleogram-0.2.5/.gitignore` & `cochleogram-0.3.0/.gitignore`

 * *Files identical despite different names*

### Comparing `cochleogram-0.2.5/PKG-INFO` & `cochleogram-0.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cochleogram
-Version: 0.2.5
+Version: 0.3.0
 Summary: Module for creating cochleograms from confocal images
 Author-email: Brad Buran <buran@ohsu.edu>
 Maintainer-email: Brad Buran <buran@ohsu.edu>
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 Provides-Extra: czi
 Provides-Extra: lif
```

### Comparing `cochleogram-0.2.5/cochleogram/gui.enaml` & `cochleogram-0.3.0/cochleogram/gui.enaml`

 * *Files 14% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 import logging
 log = logging.getLogger(__name__)
 
 from importlib import resources
+from pathlib import Path
 
 from enaml.application import deferred_call
 from enaml.core.api import Conditional, Looper
 from enaml.icon import Icon, IconImage
 from enaml.image import Image
 from enaml.layout.api import align, hbox, InsertTab, RemoveItem, spacer, TabLayout, vbox
 from enaml.stdlib.fields import FloatField
 from enaml.stdlib.message_box import critical, information, question
 from enaml.qt.QtCore import Qt
 from enaml.widgets.api import (Action, ButtonGroup, CheckBox, Container,
-                               DockArea, DockItem, Feature, FileDialogEx, Form,
-                               HGroup, Html, Label, MainWindow, Menu, MenuBar,
-                               MPLCanvas, ObjectCombo, ProgressBar, PushButton,
-                               Slider, Window)
+                               DockArea, DockItem, DualSlider, Feature,
+                               FileDialogEx, Form, HGroup, Html, Label,
+                               MainWindow, Menu, MenuBar, MPLCanvas,
+                               ObjectCombo, ProgressBar, PushButton, Slider,
+                               VGroup, Window)
 
 from cochleogram import plot, util
 from cochleogram.model import Cochlea
 from cochleogram.presenter import Presenter
 from cochleogram import readers
 
 
@@ -44,40 +46,51 @@
         q = 'There are unsaved changes. Your current analysis will be lost. Are you sure?'
         button = question(None, 'Confirm action', q)
         if button is None or button.text == 'No':
             return
 
     path = FileDialogEx.get_existing_directory(window, current_path=window.current_path)
     if path:
-        load_processed_dataset(path, window, readers.ProcessedReader)
+        load_dataset(path, window, readers.ProcessedReader)
 
 
 def open_20x_lif_file(window):
     # Check for unsaved changes
     if any(p.unsaved_changes for p in window.presenters):
         q = 'There are unsaved changes. Your current analysis will be lost. Are you sure?'
         button = question(None, 'Confirm action', q)
         if button is None or button.text == 'No':
             return
 
     path = FileDialogEx.get_open_file_name(window, current_path=window.current_path)
     if path:
-        load_processed_dataset(path, window, readers.LIFReader)
+        load_dataset(path, window, readers.LIFReader)
 
 
-def load_processed_dataset(path, window, reader_class):
-    workspace = window.find('dock_area')
+def load_dataset(path, window, reader_class=None):
+    path = Path(path)
+    if reader_class is None:
+        if path.is_dir():
+            reader_class = readers.ProcessedReader
+        elif path.suffix.lower() == '.lif':
+            reader_class = readers.LIFReader
+        else:
+            raise ValueError(f'Unrecognized format for {path}')
+
+    # First, make sure we can load the cochlea
+    reader = reader_class(path)
+    window.cochlea = reader.load_cochlea()
+
     # Remove existing cochlea
+    workspace = window.find('dock_area')
     for p in window.presenters:
         remove_dock_item(workspace, p)
 
-    reader = reader_class(path)
     # Now, load new cochlea
     window.current_path = path
-    window.cochlea = reader.load_cochlea()
     window.reader = reader
     window.presenters = [Presenter(p, reader) for p in window.cochlea.pieces]
     target = 'help'
     for p in window.presenters:
         try:
             p.load_state()
         except IOError:
@@ -150,47 +163,71 @@
     initialized ::
         bind_focus(container.children, canvas.set_focus)
         deferred_call(canvas.set_focus)
 
     Container: container:
         constraints = [
             vbox(
-                hbox(display_label, display_channel, display_as_label,
+                channel_config,
+                hbox(display_label, display_as_label,
                      display_mode, z_slice_number_label, z_slice,
                      display_apply, highlight_selected),
                 hbox(tool_label, mode_buttons, spacer, load_analysis, save_analysis),
                 hbox(action_label, action_clear_spiral, action_clear_cells,
                      action_simplify_exclusions, action_merge_ohc_exclusions,
                      spacer, spacing=0),
                 action_guess_cells,
                 action_copy_exclusion,
                 canvas,
             ),
-            align('v_center', display_label, display_channel, display_as_label,
+            align('v_center', display_label, display_as_label,
                   display_mode, z_slice_number_label, z_slice, display_apply,
                   highlight_selected),
             align('v_center', tool_label, mode_buttons),
             align('v_center', action_label, action_clear_spiral,
                   action_clear_cells, action_simplify_exclusions,
                   action_merge_ohc_exclusions),
             align('left', display_label, tool_label, action_label),
-            align('left', display_channel, mode_buttons, action_clear_spiral,
+            align('left', mode_buttons, action_clear_spiral,
                   action_guess_cells, action_copy_exclusion),
             guess_width.width == 50,
             guess_spacing.width == 50,
         ]
 
         Label: display_label:
             text = 'Display'
 
-        ObjectCombo: display_channel:
-            items = ['All'] + presenter.piece.channel_names
-            selected << 'All' if presenter.current_artist is None else presenter.current_artist.display_channel
-            selected ::
-                presenter.set_display_channel(selected, display_apply.checked)
+        Container: channel_config:
+            layout_constraints => ():
+                widgets = self.visible_widgets()
+                cb = widgets[::2]
+                slider = widgets[1::2]
+                constraints = [vbox(*[hbox(c, s) for c, s in zip(cb, slider)])]
+                constraints.append(align('left', *slider))
+                constraints.append(align('left', *cb))
+                return constraints
+
+            Looper:
+                iterable << presenter.current_artist.channel_config.items() \
+                    if presenter.current_artist is not None else {}
+
+                CheckBox:
+                    text = loop_item[0]
+                    checked << loop_item[1].visible
+                    checked ::
+                        presenter.set_channel_visible(loop_item[0], checked, display_apply.checked)
+                DualSlider:
+                    minimum = 0
+                    maximum = 100
+                    low_value << int(loop_item[1].min_value * 100)
+                    high_value << int(loop_item[1].max_value * 100)
+                    low_value ::
+                        presenter.set_channel_min_value(loop_item[0], low_value / 100, display_apply.checked)
+                    high_value ::
+                        presenter.set_channel_max_value(loop_item[0], high_value / 100, display_apply.checked)
 
         Label: display_as_label:
             text = 'as'
 
         ObjectCombo: display_mode:
             items = ['projection', 'slice']
             selected << 'projection' if presenter.current_artist is None else presenter.current_artist.display_mode
@@ -213,15 +250,14 @@
         PushButton: display_apply:
             text = 'Apply to all tiles'
             checkable = True
             checked = True
             clicked ::
                 if checked:
                     presenter.set_display_mode(display_mode.selected, True)
-                    presenter.set_display_channel(display_channel.selected, True)
 
         PushButton: highlight_selected:
             text = 'Highlight selected'
             checkable = True
             checked := presenter.highlight_selected
 
         ButtonGroup: mode_group:
@@ -450,18 +486,18 @@
             clicked ::
                 try:
                     fig = plot.plot_composite(cochlea,
                                               include_freq_map=include_freq_map.checked,
                                               channels=channels)
                     fig.suptitle(reader.get_name())
                     reader.save_figure(fig, 'frequency_map')
-                    information(self, 'Composite', 'Composite has been generated.')
+                    information(self, 'Plotting', 'Composite has been generated.')
                 except Exception as e:
                     log.exception(e)
-                    critical(self, 'Composite', str(e))
+                    critical(self, 'Plotting', str(e))
 
 
 enamldef CochleagramWindow(MainWindow): window:
 
     initial_size = (900, 900)
     title = 'Cochelogram'
     icon = load_icon('main-icon')
@@ -473,20 +509,28 @@
 
     MenuBar:
         Menu:
             title = '&File'
             Action:
                 text = 'Open processed dataset'
                 triggered ::
-                    open_processed_dataset(window)
+                    try:
+                        open_processed_dataset(window)
+                    except IOError as e:
+                        log.exception(e)
+                        critical(window, 'Load', str(e))
 
             Action:
                 text = 'Open 20x LIF file'
                 triggered ::
-                    open_20x_lif_file(window)
+                    try:
+                        open_20x_lif_file(window)
+                    except IOError as e:
+                        log.exception(e)
+                        critical(window, 'Load', str(e))
 
             Action:
                 separator = True
 
             Action:
                 text = 'Process 20x LIF file\tCtrl+P'
                 triggered ::
@@ -523,14 +567,28 @@
             Action:
                 text = 'Generate composite (frequency map)\tCtrl+F'
                 enabled << cochlea is not None
                 triggered ::
                     window = CompositeWindow(cochlea=cochlea, reader=reader)
                     window.show()
 
+            Action:
+                text = 'Generate slide map'
+                enabled << cochlea is not None
+                triggered ::
+                    try:
+                        fig = plot.plot_slide_layout(cochlea)
+                        fig.suptitle(reader.get_name())
+                        reader.save_figure(fig, 'slide_map')
+                        information(window, 'Plotting', 'Slide map has been generated.')
+                    except Exception as e:
+                        log.exception(e)
+                        critical(window, 'Plotting', str(e))
+
+
     initialized ::
         for presenter in presenters:
             deferred_call(add_dock_item, workspace, presenter)
 
     closing ::
         if any(p.unsaved_changes for p in presenters):
             button = question(window, 'Question', 'There are unsaved changes. Are you sure you want to exit?')
```

### Comparing `cochleogram-0.2.5/cochleogram/icons/cells.png` & `cochleogram-0.3.0/cochleogram/icons/cells.png`

 * *Files identical despite different names*

### Comparing `cochleogram-0.2.5/cochleogram/icons/exclude.png` & `cochleogram-0.3.0/cochleogram/icons/exclude.png`

 * *Files identical despite different names*

### Comparing `cochleogram-0.2.5/cochleogram/icons/main-icon.png` & `cochleogram-0.3.0/cochleogram/icons/main-icon.png`

 * *Files identical despite different names*

### Comparing `cochleogram-0.2.5/cochleogram/icons/make_icons.py` & `cochleogram-0.3.0/cochleogram/icons/make_icons.py`

 * *Files identical despite different names*

### Comparing `cochleogram-0.2.5/cochleogram/icons/spiral.png` & `cochleogram-0.3.0/cochleogram/icons/spiral.png`

 * *Files identical despite different names*

### Comparing `cochleogram-0.2.5/cochleogram/icons/tile.png` & `cochleogram-0.3.0/cochleogram/icons/tile.png`

 * *Files identical despite different names*

### Comparing `cochleogram-0.2.5/cochleogram/instructions.html` & `cochleogram-0.3.0/cochleogram/instructions.html`

 * *Files identical despite different names*

### Comparing `cochleogram-0.2.5/cochleogram/main.py` & `cochleogram-0.3.0/cochleogram/main.py`

 * *Files 5% similar despite different names*

```diff
@@ -59,27 +59,27 @@
     import enaml
     from enaml.qt.qt_application import QtApplication
     logging.basicConfig(level='INFO')
 
     from cochleogram.presenter import Presenter
 
     with enaml.imports():
-        from cochleogram.gui import CochleagramWindow, load_processed_dataset
+        from cochleogram.gui import CochleagramWindow, load_dataset
 
     parser = argparse.ArgumentParser("Cochleogram helper")
     parser.add_argument("path", nargs='?')
     args = parser.parse_args()
 
     app = QtApplication()
     config = get_config()
 
     current_path = config['DEFAULT']['current_path']
     view = CochleagramWindow(current_path=current_path)
     if args.path is not None:
-        deferred_call(load_processed_dataset, args.path, view)
+        deferred_call(load_dataset, args.path, view)
     view.show()
     app.start()
     app.stop()
     config['DEFAULT']['current_path'] = str(Path(view.current_path).absolute())
     write_config(config)
```

### Comparing `cochleogram-0.2.5/cochleogram/model.py` & `cochleogram-0.3.0/cochleogram/model.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import logging
 log = logging.getLogger(__name__)
 
-from atom.api import Atom, Dict, Event, Float, Int, List, Str, Typed
+from atom.api import Atom, Bool, Dict, Event, Float, Int, List, Str, Typed
 from matplotlib import colors
 from matplotlib import transforms as T
 import numpy as np
 import pandas as pd
 
 from psiaudio.util import octave_space
 from scipy import interpolate
@@ -16,18 +16,26 @@
 from cochleogram import util
 
 
 CHANNEL_CONFIG = {
     'CtBP2': { 'display_color': 'red'},
     'MyosinVIIa': {'display_color': 'blue'},
     'PMT': {'display_color': 'white'},
-    'DAPI': {'display_color': 'green'},
+    'DAPI': {'display_color': 'white'},
 }
 
 
+class ChannelConfig(Atom):
+
+    name = Str()
+    min_value = Float(0)
+    max_value = Float(1)
+    visible = Bool(True)
+
+
 class Points(Atom):
 
     x = List()
     y = List()
     origin = Int()
     exclude = List()
 
@@ -356,38 +364,71 @@
 
     def get_image(self, channels=None, z_slice=None, axis='z',
                   norm_percentile=99):
         if z_slice is None:
             data = self.image.max(axis='xyz'.index(axis))
         else:
             data = self.image[:, :, z_slice, :]
+        x, y = data.shape[:2]
+
+        # Normalize data
+        data_max =  np.percentile(data, norm_percentile, axis=(0, 1), keepdims=True)
+        data_mask = data_max != 0
+        data = np.divide(data, data_max, where=data_mask).clip(0, 1)
 
-        if channels is None or channels == 'All':
+        if channels is None:
             channels = self.channel_names
         elif isinstance(channels, int):
             raise ValueError('Must provide name for channel')
         elif isinstance(channels, str):
             channels = [channels]
         elif len(channels) == 0:
-            raise ValueError('Cannot generate image with zero channels')
+            #raise ValueError('Cannot generate image with zero channels')
+            return np.zeros((x, y))
+
+        # Check that channels are valid and generate config
+        channel_config = {}
         for c in channels:
-            if c not in self.channel_names:
+            if isinstance(c, ChannelConfig):
+                if not c.visible:
+                    continue
+                if c.name not in self.channel_names:
+                    raise ValueError(f'Channel {c.name} does not exist')
+                channel_config[c.name] = {
+                    'min_value': c.min_value,
+                    'max_value': c.max_value,
+                    **CHANNEL_CONFIG[c.name],
+                }
+            elif isinstance(c, dict):
+                channel_config[c['name']] = {
+                    **c,
+                    **CHANNEL_CONFIG[c['name']],
+                }
+            elif c not in self.channel_names:
                 raise ValueError(f'Channel {c} does not exist')
+            else:
+                channel_config[c] = {
+                    'min_value': 0,
+                    'max_value': 1,
+                    **CHANNEL_CONFIG[c],
+                }
 
-        x, y = data.shape[:2]
         image = []
         for c, c_info in enumerate(self.info['channels']):
-            if c_info['name'] in channels:
-                color = CHANNEL_CONFIG[c_info['name']]['display_color']
-                rgb = colors.to_rgba(color)[:3]
-                image.append(data[..., c][..., np.newaxis] * rgb)
-        image = np.concatenate([i[np.newaxis] for i in image]).max(axis=0)
-        image_max =  np.percentile(image, norm_percentile, axis=(0, 1), keepdims=True)
-        image_mask = image_max != 0
-        return np.divide(image, image_max, where=image_mask).clip(0, 1)
+            if c_info['name'] in channel_config:
+                config = channel_config[c_info['name']]
+                rgb = colors.to_rgba(config['display_color'])[:3]
+
+                lb = config['min_value']
+                ub = config['max_value']
+                d = np.clip((data[..., c] - lb) / (ub - lb), 0, 1)
+                d = d[..., np.newaxis] * rgb
+                image.append(d)
+
+        return np.concatenate([i[np.newaxis] for i in image]).max(axis=0)
 
     def get_state(self):
         return {"extent": self.extent}
 
     def set_state(self, state):
         self.extent = state["extent"]
 
@@ -441,15 +482,21 @@
 
     @property
     def channel_names(self):
         # We assume that each tile has the same set of channels
         return self.tiles[0].channel_names
 
     def get_image_extent(self):
-        extents = np.vstack([tile.get_image_extent() for tile in self.tiles])
+        return self._get_extent(lambda t: t.get_image_extent())
+
+    def get_rotated_extent(self):
+        return self._get_extent(lambda t: t.get_rotated_extent())
+
+    def _get_extent(self, cb):
+        extents = np.vstack([cb(tile) for tile in self.tiles])
         xmin = extents[:, 0].min()
         xmax = extents[:, 1].max()
         ymin = extents[:, 2].min()
         ymax = extents[:, 3].max()
         return [xmin, xmax, ymin, ymax]
 
     def merge_tiles(self):
@@ -551,14 +598,28 @@
     def channel_names(self):
         # We assume that each tile has the same set of channels
         names = set()
         for piece in self.pieces:
             names.update(piece.channel_names)
         return sorted(names)
 
+    def get_image_extent(self):
+        return self._get_extent(lambda p: p.get_image_extent())
+
+    def get_rotated_extent(self):
+        return self._get_extent(lambda p: p.get_rotated_extent())
+
+    def _get_extent(self, cb):
+        extents = np.vstack([cb(piece) for piece in self.pieces])
+        xmin = extents[:, 0].min()
+        xmax = extents[:, 1].max()
+        ymin = extents[:, 2].min()
+        ymax = extents[:, 3].max()
+        return [xmin, xmax, ymin, ymax]
+
     def ihc_spiral_complete(self):
         for piece in self.pieces:
             s = piece.spirals['IHC']
             x, y = s.interpolate(resolution=0.001)
             if len(x) == 0:
                 return False
         return True
```

### Comparing `cochleogram-0.2.5/cochleogram/plot.py` & `cochleogram-0.3.0/cochleogram/plot.py`

 * *Files 21% similar despite different names*

```diff
@@ -65,13 +65,26 @@
     ax.set_xticks([])
     ax.set_yticks([])
 
     figure.subplots_adjust(left=0.025, right=0.975, top=0.95, bottom=0.025)
     return figure
 
 
+def plot_slide_layout(cochlea):
+    figure, ax = plt.subplots(1, 1)
+    for piece in cochlea.pieces:
+        for tile in piece.tiles:
+            plot_tile(ax, tile)
+    e = cochlea.get_rotated_extent()
+    ax.axis(e)
+    ax.set_xticks([])
+    ax.set_yticks([])
+    ax.set_facecolor('k')
+    return figure
+
+
 def plot_tile(ax, tile):
     ax.imshow(tile.get_image().swapaxes(0, 1),
               origin='lower',
               aspect='equal',
               transform=tile.get_image_transform() + ax.transData,
               extent=tile.get_image_extent())
```

### Comparing `cochleogram-0.2.5/cochleogram/presenter.py` & `cochleogram-0.3.0/cochleogram/presenter.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 from matplotlib import patches as mpatches
 from matplotlib import path as mpath
 from matplotlib import transforms as T
 
 import numpy as np
 from scipy import interpolate
 
-from cochleogram.model import Piece, Points, Tile
+from cochleogram.model import ChannelConfig, Piece, Points, Tile
 from cochleogram.util import get_region, make_plot_path, shortest_path
 
 
 class PointPlot(Atom):
 
     #: Artist that plots the nodes the user specified
     artist = Value()
@@ -197,16 +197,18 @@
 
 class ImagePlot(Atom):
 
     alpha = Float(0.75)
     highlight = Bool(False)
     zorder = Int(10)
 
+    channel_config = Value()
+
     display_mode = Enum("projection", "slice")
-    display_channel = Str('All')
+    display_channels = List()
     extent = Tuple()
     z_slice = Int(0)
     z_slice_min = Int(0)
     z_slice_max = Int(0)
     shift = Float()
 
     tile = Typed(Tile)
@@ -220,26 +222,26 @@
     needs_redraw = Bool(False)
 
     def get_state(self):
         return {
             "alpha": self.alpha,
             "zorder": self.zorder,
             "display_mode": self.display_mode,
-            "display_channel": self.display_channel,
+            "display_channels": self.display_channels,
             "z_slice": self.z_slice,
             "z_slice_min": self.z_slice_min,
             "z_slice_max": self.z_slice_max,
             "shift": self.shift,
         }
 
     def set_state(self, state):
         self.alpha = state["alpha"]
         self.zorder = state["zorder"]
         self.display_mode = state["display_mode"]
-        self.display_channel = state["display_channel"]
+        self.display_channels = state["display_channels"]
         self.z_slice = state["z_slice"]
         self.z_slice_min = state["z_slice_min"]
         self.z_slice_max = state["z_slice_max"]
         self.shift = state["shift"]
 
     def __init__(self, axes, tile, **kwargs):
         super().__init__(**kwargs)
@@ -252,14 +254,19 @@
         self.artist = axes.imshow(np.array([[0, 1], [0, 1]]), origin="lower", transform=self.transform)
         self.rectangle = mp.patches.Rectangle((0, 0), 0, 0, ec='red', fc='None', zorder=5000, transform=self.transform)
         self.rectangle.set_alpha(0)
         self.axes.add_patch(self.rectangle)
         self.z_slice_max = self.tile.image.shape[2] - 1
         self.z_slice = self.tile.image.shape[2] // 2
         self.shift = self.tile.info["voxel_size"][0] * 5
+        self.channel_config = {c: ChannelConfig(name=c) for c in tile.channel_names}
+        for config in self.channel_config.values():
+            config.observe('visible', self.request_redraw)
+            config.observe('min_value', self.request_redraw)
+            config.observe('max_value', self.request_redraw)
         tile.observe('extent', self.request_redraw)
 
     def _observe_highlight(self, event):
         if self.highlight:
             self.rectangle.set_alpha(1)
         else:
             self.rectangle.set_alpha(0)
@@ -285,40 +292,48 @@
             extent[2:4] -= step
         elif direction == "left":
             extent[0:2] -= step
         elif direction == "right":
             extent[0:2] += step
         self.tile.extent = extent.tolist()
 
-    @observe("z_slice", "display_mode", "display_channel", "alpha", "highlight")
+    @observe("z_slice", "display_mode", "alpha", "highlight")
     def request_redraw(self, event=False):
         self.needs_redraw = True
         deferred_call(self.redraw_if_needed)
 
     def redraw_if_needed(self):
         if self.needs_redraw:
             self.redraw()
             self.needs_redraw = False
 
     def redraw(self, event=None):
         z_slice = None if self.display_mode == 'projection' else self.z_slice
-        image = self.tile.get_image(channels=self.display_channel,
-                                    z_slice=z_slice).swapaxes(0, 1)
+        channels = [c for c in self.channel_config.values() if c.visible]
+        image = self.tile.get_image(channels=channels, z_slice=z_slice).swapaxes(0, 1)
         self.artist.set_data(image)
         xlb, xub, ylb, yub = extent = self.tile.get_image_extent()[:4]
         self.artist.set_extent(extent)
         self.rectangle.set_bounds(xlb, ylb, xub-xlb, yub-ylb)
-
         t = self.tile.get_image_transform()
         self.rotation_transform.set_matrix(t.get_matrix())
         self.updated = True
 
     def contains(self, x, y):
         return self.tile.contains(x, y)
 
+    def set_channel_visible(self, channel_name, visible):
+        self.channel_config[channel_name].visible = visible
+
+    def set_channel_min_value(self, channel_name, min_value):
+        self.channel_config[channel_name].min_value = min_value
+
+    def set_channel_max_value(self, channel_name, max_value):
+        self.channel_config[channel_name].max_value = max_value
+
 
 class Presenter(Atom):
 
     # Interface to help read data
     reader = Value()
 
     # Tile artists
@@ -379,15 +394,15 @@
         self.piece = piece
         self.reader = reader
         self.tile_artists = {
             t.source: ImagePlot(self.axes, t) for t in self.piece.tiles
         }
         for artist in self.tile_artists.values():
             artist.observe('updated', self.update)
-        self.current_artist_index = None
+        self.current_artist_index = 0
         for key in ('IHC', 'OHC1', 'OHC2', 'OHC3', 'Extra'):
             cells = PointPlot(self.axes, self.piece.cells[key], name=key)
             spiral = LinePlot(self.axes, self.piece.spirals[key], name=key)
             cells.observe('updated', self.update)
             spiral.observe('updated', self.update)
             self.point_artists[key, 'cells'] = cells
             self.point_artists[key, 'spiral'] = spiral
@@ -414,18 +429,15 @@
     def _default_figure(self):
         return Figure()
 
     def _default_axes(self):
         return self.figure.add_axes([0, 0, 1, 1])
 
     def _observe_current_artist_index(self, event):
-        if self.current_artist_index is None:
-            self.current_artist = None
-        else:
-            self.current_artist = list(self.tile_artists.values())[self.current_artist_index]
+        self.current_artist = list(self.tile_artists.values())[self.current_artist_index]
         self.update_highlight()
 
     @observe("highlight_selected",)
     def update_highlight(self, event=None):
         alpha = self.alpha_unselected if self.highlight_selected else 1
         for artist in self.tile_artists.values():
             artist.zorder = self.zorder_unselected
@@ -530,20 +542,19 @@
     def key_press_tile(self, event):
         if event.key in ["right", "left", "up", "down"]:
             if self.current_artist is not None:
                 self.current_artist.move_image(event.key)
         elif event.key in ["shift+right", "shift+left", "shift+up", "shift+down"]:
             if self.current_artist is not None:
                 self.current_artist.move_image(event.key.split('+')[1], 0.25)
-
         elif event.key.lower() == "n":
-            i = -1 if self.current_artist_index is None else self.current_artist_index
+            i = self.current_artist_index
             self.current_artist_index = (i + 1) % len(self.tile_artists)
         elif event.key.lower() == "p":
-            i = len(self.tile_artists) + 1 if self.current_artist_index is None else self.current_artist_index
+            i = len(self.tile_artists) + 1
             self.current_artist_index = (i - 1) % len(self.tile_artists)
 
     def key_press_point_plot(self, event):
         if event.key.startswith('shift+'):
             direction = event.key.split('+')[1]
             scale = 0.025
         else:
@@ -568,16 +579,14 @@
 
     def button_release_tile(self, event):
         if event.button == MouseButton.LEFT and event.xdata is not None:
             for i, artist in enumerate(self.tile_artists.values()):
                 if artist.contains(event.xdata, event.ydata):
                     self.current_artist_index = i
                     break
-            else:
-                self.current_artist_index = None
 
     def button_press_point_plot(self, event):
         if event.button != MouseButton.RIGHT:
             return
         if self.cells == 'Extra' and self.tool != 'cells':
             # Special case. I don't want to add spiral/exclude regions to extra
             # cells data structure for now.
@@ -706,20 +715,34 @@
     def set_display_mode(self, display_mode, all_tiles=False):
         if all_tiles:
             for artist in self.tile_artists.values():
                 artist.display_mode = display_mode
         elif self.current_artist is not None:
             self.current_artist.display_mode = display_mode
 
-    def set_display_channel(self, display_channel, all_tiles=False):
+    def set_channel_visible(self, channel_name, visible, all_tiles=False):
+        if all_tiles:
+            for artist in self.tile_artists.values():
+                artist.set_channel_visible(channel_name, visible)
+        elif self.current_artist is not None:
+            self.current_artist.set_channel_visible(channel_name, visible)
+
+    def set_channel_min_value(self, channel_name, low_value, all_tiles=False):
+        if all_tiles:
+            for artist in self.tile_artists.values():
+                artist.set_channel_min_value(channel_name, low_value)
+        elif self.current_artist is not None:
+            self.current_artist.set_channel_min_value(channel_name, low_value)
+
+    def set_channel_max_value(self, channel_name, high_value, all_tiles=False):
         if all_tiles:
             for artist in self.tile_artists.values():
-                artist.display_channel = display_channel
+                artist.set_channel_max_value(channel_name, high_value)
         elif self.current_artist is not None:
-            self.current_artist.display_channel = display_channel
+            self.current_artist.set_channel_max_value(channel_name, high_value)
 
     def set_z_slice(self, z_slice, all_tiles=False):
         if all_tiles:
             for artist in self.tile_artists.values():
                 artist.z_slice = z_slice
         elif self.current_artist is not None:
             self.current_artist.z_slice = z_slice
```

### Comparing `cochleogram-0.2.5/cochleogram/readers.py` & `cochleogram-0.3.0/cochleogram/readers.py`

 * *Files 4% similar despite different names*

```diff
@@ -94,14 +94,16 @@
             t.image = np.pad(t.image, padding)
             t.extent[4:] = [z_min, z_max]
 
         return model.Piece(tiles, piece)
 
     def load_cochlea(self):
         pieces = [self.load_piece(p, sn) for p, sn in self.list_pieces().items()]
+        if len(pieces) == 0:
+            raise IOError(f'No pieces found in {self.path}')
         return model.Cochlea(pieces)
 
     def save_path(self):
         return self.path.parent / self.path.stem
 
     def state_filename(self, piece):
         return self.save_path() / f'{self.path.stem}_piece_{piece.piece}_analysis.json'
@@ -150,14 +152,16 @@
             t.image = np.pad(t.image, padding)
             t.extent[4:] = [z_min, z_max]
 
         return model.Piece(tiles, piece)
 
     def load_cochlea(self):
         pieces = [self.load_piece(p) for p in self.list_pieces()]
+        if len(pieces) == 0:
+            raise IOError(f'No pieces found in {self.path}')
         return model.Cochlea(pieces)
 
     def state_filename(self, piece):
         return self.path /  f'{self.path.stem}_piece_{piece.piece}_analysis.json'
 
     def save_path(self):
         return self.path
```

### Comparing `cochleogram-0.2.5/cochleogram/util.py` & `cochleogram-0.3.0/cochleogram/util.py`

 * *Files identical despite different names*

### Comparing `cochleogram-0.2.5/cochleogram.egg-info/PKG-INFO` & `cochleogram-0.3.0/cochleogram.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cochleogram
-Version: 0.2.5
+Version: 0.3.0
 Summary: Module for creating cochleograms from confocal images
 Author-email: Brad Buran <buran@ohsu.edu>
 Maintainer-email: Brad Buran <buran@ohsu.edu>
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 Provides-Extra: czi
 Provides-Extra: lif
```

### Comparing `cochleogram-0.2.5/cochleogram.egg-info/SOURCES.txt` & `cochleogram-0.3.0/cochleogram.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cochleogram-0.2.5/pyproject.toml` & `cochleogram-0.3.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `cochleogram-0.2.5/readme.rst` & `cochleogram-0.3.0/readme.rst`

 * *Files identical despite different names*

