# Comparing `tmp/indiek-gui-0.0.3.tar.gz` & `tmp/indiek-gui-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/adrian_admin/prog/indiek/indiek-gui/dist/.tmp-4b78jphm/indiek-gui-0.0.3.tar", last modified: Tue May  9 22:20:56 2023, max compression
+gzip compressed data, was "/home/adrian_admin/prog/indiek/indiek-gui/dist/.tmp-2dm50h__/indiek-gui-0.0.4.tar", last modified: Thu May 18 00:42:24 2023, max compression
```

## Comparing `indiek-gui-0.0.3.tar` & `indiek-gui-0.0.4.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxrwxr-x   0 adrian_admin  (1001) adrian_admin  (1001)        0 2023-05-09 22:20:56.993971 indiek-gui-0.0.3/
--rw-rw-r--   0 adrian_admin  (1001) adrian_admin  (1001)    34523 2023-05-05 01:24:51.000000 indiek-gui-0.0.3/LICENSE
--rw-rw-r--   0 adrian_admin  (1001) adrian_admin  (1001)     1003 2023-05-09 22:20:56.993971 indiek-gui-0.0.3/PKG-INFO
--rw-rw-r--   0 adrian_admin  (1001) adrian_admin  (1001)      555 2023-05-06 19:18:51.000000 indiek-gui-0.0.3/README.rst
-drwxrwxr-x   0 adrian_admin  (1001) adrian_admin  (1001)        0 2023-05-09 22:20:56.981971 indiek-gui-0.0.3/indiek/
-drwxrwxr-x   0 adrian_admin  (1001) adrian_admin  (1001)        0 2023-05-09 22:20:56.993971 indiek-gui-0.0.3/indiek/gui/
--rw-rw-r--   0 adrian_admin  (1001) adrian_admin  (1001)       34 2023-05-07 21:17:10.000000 indiek-gui-0.0.3/indiek/gui/__init__.py
--rw-rw-r--   0 adrian_admin  (1001) adrian_admin  (1001)    18645 2023-05-09 22:04:25.000000 indiek-gui-0.0.3/indiek/gui/app.py
--rw-rw-r--   0 adrian_admin  (1001) adrian_admin  (1001)     1452 2023-05-07 22:15:22.000000 indiek-gui-0.0.3/indiek/gui/items.py
-drwxrwxr-x   0 adrian_admin  (1001) adrian_admin  (1001)        0 2023-05-09 22:20:56.993971 indiek-gui-0.0.3/indiek_gui.egg-info/
--rw-rw-r--   0 adrian_admin  (1001) adrian_admin  (1001)     1003 2023-05-09 22:20:56.000000 indiek-gui-0.0.3/indiek_gui.egg-info/PKG-INFO
--rw-rw-r--   0 adrian_admin  (1001) adrian_admin  (1001)      304 2023-05-09 22:20:56.000000 indiek-gui-0.0.3/indiek_gui.egg-info/SOURCES.txt
--rw-rw-r--   0 adrian_admin  (1001) adrian_admin  (1001)        1 2023-05-09 22:20:56.000000 indiek-gui-0.0.3/indiek_gui.egg-info/dependency_links.txt
--rw-rw-r--   0 adrian_admin  (1001) adrian_admin  (1001)       47 2023-05-09 22:20:56.000000 indiek-gui-0.0.3/indiek_gui.egg-info/entry_points.txt
--rw-rw-r--   0 adrian_admin  (1001) adrian_admin  (1001)       56 2023-05-09 22:20:56.000000 indiek-gui-0.0.3/indiek_gui.egg-info/requires.txt
--rw-rw-r--   0 adrian_admin  (1001) adrian_admin  (1001)        7 2023-05-09 22:20:56.000000 indiek-gui-0.0.3/indiek_gui.egg-info/top_level.txt
--rw-rw-r--   0 adrian_admin  (1001) adrian_admin  (1001)      147 2023-05-09 22:20:56.993971 indiek-gui-0.0.3/setup.cfg
--rw-rw-r--   0 adrian_admin  (1001) adrian_admin  (1001)      920 2023-05-09 22:20:47.000000 indiek-gui-0.0.3/setup.py
+drwxrwxr-x   0 adrian_admin  (1001) adrian_admin  (1001)        0 2023-05-18 00:42:24.230288 indiek-gui-0.0.4/
+-rw-rw-r--   0 adrian_admin  (1001) adrian_admin  (1001)    34523 2023-05-05 01:24:51.000000 indiek-gui-0.0.4/LICENSE
+-rw-rw-r--   0 adrian_admin  (1001) adrian_admin  (1001)     1003 2023-05-18 00:42:24.230288 indiek-gui-0.0.4/PKG-INFO
+-rw-rw-r--   0 adrian_admin  (1001) adrian_admin  (1001)      555 2023-05-06 19:18:51.000000 indiek-gui-0.0.4/README.rst
+drwxrwxr-x   0 adrian_admin  (1001) adrian_admin  (1001)        0 2023-05-18 00:42:24.206288 indiek-gui-0.0.4/indiek/
+drwxrwxr-x   0 adrian_admin  (1001) adrian_admin  (1001)        0 2023-05-18 00:42:24.230288 indiek-gui-0.0.4/indiek/gui/
+-rw-rw-r--   0 adrian_admin  (1001) adrian_admin  (1001)       34 2023-05-09 22:32:51.000000 indiek-gui-0.0.4/indiek/gui/__init__.py
+-rw-rw-r--   0 adrian_admin  (1001) adrian_admin  (1001)    22894 2023-05-18 00:36:44.000000 indiek-gui-0.0.4/indiek/gui/app.py
+-rw-rw-r--   0 adrian_admin  (1001) adrian_admin  (1001)     2745 2023-05-13 12:07:45.000000 indiek-gui-0.0.4/indiek/gui/items.py
+-rw-rw-r--   0 adrian_admin  (1001) adrian_admin  (1001)     3932 2023-05-14 16:42:30.000000 indiek-gui-0.0.4/indiek/gui/styles.py
+drwxrwxr-x   0 adrian_admin  (1001) adrian_admin  (1001)        0 2023-05-18 00:42:24.230288 indiek-gui-0.0.4/indiek_gui.egg-info/
+-rw-rw-r--   0 adrian_admin  (1001) adrian_admin  (1001)     1003 2023-05-18 00:42:24.000000 indiek-gui-0.0.4/indiek_gui.egg-info/PKG-INFO
+-rw-rw-r--   0 adrian_admin  (1001) adrian_admin  (1001)      325 2023-05-18 00:42:24.000000 indiek-gui-0.0.4/indiek_gui.egg-info/SOURCES.txt
+-rw-rw-r--   0 adrian_admin  (1001) adrian_admin  (1001)        1 2023-05-18 00:42:24.000000 indiek-gui-0.0.4/indiek_gui.egg-info/dependency_links.txt
+-rw-rw-r--   0 adrian_admin  (1001) adrian_admin  (1001)       47 2023-05-18 00:42:24.000000 indiek-gui-0.0.4/indiek_gui.egg-info/entry_points.txt
+-rw-rw-r--   0 adrian_admin  (1001) adrian_admin  (1001)       56 2023-05-18 00:42:24.000000 indiek-gui-0.0.4/indiek_gui.egg-info/requires.txt
+-rw-rw-r--   0 adrian_admin  (1001) adrian_admin  (1001)        7 2023-05-18 00:42:24.000000 indiek-gui-0.0.4/indiek_gui.egg-info/top_level.txt
+-rw-rw-r--   0 adrian_admin  (1001) adrian_admin  (1001)      147 2023-05-18 00:42:24.230288 indiek-gui-0.0.4/setup.cfg
+-rw-rw-r--   0 adrian_admin  (1001) adrian_admin  (1001)      920 2023-05-09 22:33:03.000000 indiek-gui-0.0.4/setup.py
```

### Comparing `indiek-gui-0.0.3/LICENSE` & `indiek-gui-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `indiek-gui-0.0.3/PKG-INFO` & `indiek-gui-0.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: indiek-gui
-Version: 0.0.3
+Version: 0.0.4
 Summary: Tkinter GUI for IndieK
 Home-page: https://pypi.org/project/indiek-gui/
 Author: Adrian Ernesto Radillo
 Author-email: adrian.radillo@gmail.com
 License: GNU Affero General Public License v3.0
 Project-URL: GitHub, https://github.com/indiek/indiek-gui
 Project-URL: Documentation, https://indiekgui.readthedocs.io/en/latest/
```

### Comparing `indiek-gui-0.0.3/README.rst` & `indiek-gui-0.0.4/README.rst`

 * *Files identical despite different names*

### Comparing `indiek-gui-0.0.3/indiek/gui/app.py` & `indiek-gui-0.0.4/indiek/gui/app.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,20 +1,37 @@
 # -*- coding: utf-8 -*-
-from typing import Optional, Mapping
+"""
+Mind refresher:
+
+What variable is shown in the Text widgets from the Edit notebook tab?
+    -> self.view_var
+"""
+# TODO: set minimum width on labels or their containing columns
+from typing import Optional, Mapping, Tuple, Iterator
 from tkinter import *
+from tkinter import filedialog
 from tkinter import ttk
 from functools import partial
+from indiek.mockdb.persistence import persist, load_from_file
 from indiek.core.search import list_all_items, filter_str
 from indiek.gui.items import core_to_gui_item, Item as GUIItem, Definition, Theorem, Proof
+from indiek.gui.styles import IndiekTheme, DEFAULT_FONT
 from indiek.core.items import (Definition as CoreDefinition, 
                                Theorem as CoreTheorem, 
                                Proof as CoreProof)
 from . import __version__
 
 
+PairOfInt = Tuple[int, int]
+
+
+DEFAULT_PERSISTENCE_DIR = '/home/adrian_admin/prog/indiek/indiek-gui/.data/'
+"""Path where DB gets persisted and loaded from."""
+
+
 ITEM_TYPES = [Definition, Theorem, Proof]
 """List of item types."""
 
 
 FILTER_NAMES = ['Definitions', 'Theorems', 'Proofs']
 """Strings used in filter radio buttons for each Item type."""
 
@@ -23,16 +40,38 @@
     'Definitions': CoreDefinition, 
     'Theorems': CoreTheorem, 
     'Proofs': CoreProof
 }
 assert set(NAME_TO_ITEM_TYPE.keys()) == set(FILTER_NAMES)
 
 
+CANVAS_OPTIONS = {
+    'search_results': dict(
+        background='blue',
+    ),
+}
+
 WRAP_1 = 380
-ENTRY_DEFAULT_LENGTH = 54
+
+ONE_LINE_HEIGHT = 1  # in units of lines
+
+
+def grid_init(
+        frame, 
+        *,
+        subcols: Iterator[PairOfInt] = ((0, 1),), 
+        subrows: Iterator[PairOfInt] = ((0, 1),),
+        init_row_col: PairOfInt = (0,0),
+        sticky: str = 'news',
+        ) -> None:
+    frame.grid(row=init_row_col[0], column=init_row_col[1], sticky=sticky)
+    for colix, colw in subcols:
+        frame.grid_columnconfigure(colix, weight=colw)
+    for rowix, roww in subrows:
+        frame.grid_rowconfigure(rowix, weight=roww)
 
 
 class Orchestrator:
     item_result_height = 40
     """Height of Label in results to be displayed."""
 
     view_id = 0
@@ -41,15 +80,14 @@
     edit_id = 1
     """ID of edit tab in Notebook."""
 
     filters = []
     filter_callbacks = {}
     """Callbacks for filter."""
 
-    filter_buttons = {}
     filter_vars = {}
 
     view_callbacks = {}
     """Callbacks for View pane."""
 
     text = {}
     """Text widgets for Editing arranged as Dict."""
@@ -57,211 +95,265 @@
     _default_str = 'No Item Selected'
     
     search_results_list = []
     """List of GUIItems to be displayed as search results."""
 
     ikid_to_result_slot = {}
     
-    def __init__(self, root, max_results: int = 100):
+    def __init__(
+            self, 
+            root, 
+            max_results: int = 100, 
+            indiek_theme: type = IndiekTheme,
+            debug: bool = False
+            ):
+        self.debug = debug
+        self.theme = indiek_theme(debug=self.debug)
         self.search_var = StringVar()
 
-        self.view_var = GUIItem(
-                name_var=StringVar(value=self._default_str),
-                content_var=StringVar(value=self._default_str),
-                name=self._default_str, 
-                content=self._default_str
-                )
-        """Current GUIItem for View/Edit panel."""
+        self.view_var = self._initialize_view_var()
 
         self.max_results = max_results
 
         self.root = root
+
+        self.create_main_menu()
+
         self.mainframe = ttk.Panedwindow(self.root, orient=HORIZONTAL)
         self.mainframe.grid(column=0, row=0, sticky='news')
         self.mainframe.columnconfigure(0, weight=1)
         self.mainframe.columnconfigure(1, weight=2)
         self.mainframe.rowconfigure(0, weight=1)
 
         self._initialize_right_panel()
         self._initialize_left_panel()
 
         self.mainframe.add(self.left_panel, weight=1)
         self.mainframe.add(self.right_panel, weight=2)
 
     def initialize_item_view(self, frame, gui_item: GUIItem):
         local_frame = ttk.Frame(frame)
-        local_frame.grid(row=0, column=0, sticky='news')
-        local_frame.grid_rowconfigure(0, weight=1)
-        local_frame.grid_rowconfigure(1, weight=1)
-        local_frame.grid_columnconfigure(0, weight=1)
-        local_frame.grid_columnconfigure(1, weight=1)
+        grid_init(
+            local_frame,
+            subcols=[(0, 0), (1, 1)],
+            subrows=[(0, 0), (1, 0), (2, 1)]
+            )
         
-        item_name_descr = ttk.Label(local_frame, text='name')
-        item_name_descr.grid(row=0, column=0, sticky='e')
+        self.item_type = ttk.Label(
+            local_frame, 
+            text=gui_item.__class__.__name__,
+            style=self.theme.generic_label.ik_name
+            )
+        if self.debug:
+            self.item_type['text'] += ' ikid:' + str(gui_item._ikid)
+        self.item_type.grid(row=0, column=0, sticky='news')
+        gen_label = partial(ttk.Label, local_frame, style=self.theme.generic_label.ik_name)
+        item_name_descr = gen_label(text='name')
+        item_name_descr.grid(row=1, column=0, sticky='new')
 
-        item_name = ttk.Label(local_frame, textvariable=gui_item.name_var)
-        item_name.grid(row=0, column=1, sticky='w')
+        item_name = gen_label(textvariable=gui_item.name_var)
+        item_name.grid(row=1, column=1, sticky='new')
         self.item_view_name_label = item_name
 
-        item_content_descr = ttk.Label(local_frame, text='content')
-        item_content_descr.grid(row=1, column=0, sticky='e')
+        item_content_descr = gen_label(text='content')
+        item_content_descr.grid(row=2, column=0, sticky='new')
         
-        item_content = ttk.Label(local_frame, textvariable=gui_item.content_var)
-        item_content.grid(row=1, column=1, sticky='w')
+        item_content = gen_label(textvariable=gui_item.content_var)
+        item_content.grid(row=2, column=1, sticky='new')
         self.item_view_content_label = item_content
 
     def _initialize_right_panel(self):
-        right_panel_style = ttk.Style()
-        right_panel_style.configure(
-            'Rightpanel.TLabelframe',
-            background='green',
-            padding=10,
-            width=1000,
-            height=650
-        )
         self.right_panel = ttk.PanedWindow(self.mainframe, orient=VERTICAL)
 
         self.view_panel = ttk.Labelframe(
             self.right_panel,
-            relief="ridge",
-            style='Rightpanel.TLabelframe',
+            style=self.theme.right_panel.ik_name,
             text='View/Edit'
         )
-        self.view_panel.grid(row=0, column=0, sticky='news')
-        self.view_panel.grid_columnconfigure(0, weight=1)
-        self.view_panel.grid_rowconfigure(0, weight=1)
+        grid_init(self.view_panel)
 
-        self._populate_view_notebook()
+        self._initialize_view_notebook()
 
         self.project_panel = ttk.Labelframe(
             self.right_panel,
-            relief="ridge",
-            style='Rightpanel.TLabelframe',
+            style=self.theme.right_panel.ik_name,
             text='Project'
         )
 
         self.right_panel.add(self.view_panel, weight=1)
         self.right_panel.add(self.project_panel, weight=1)
 
-    def _populate_view_notebook(self):
-        self.view_nb = ttk.Notebook(self.view_panel, width=800)
+    def _initialize_view_notebook(self):
+        self.view_nb = ttk.Notebook(self.view_panel)
         self.view_nb.grid(row=0, column=0, sticky='news')
 
         # View tab
         view = ttk.Frame(self.view_nb)
-        view.grid(row=0, column=0, sticky='news')
-        view.grid_rowconfigure(0, weight=1)
-        view.grid_columnconfigure(0, weight=1)
-
-        item_frame = ttk.Frame(view, borderwidth=1, relief='groove')
-        item_frame.grid(row=0, column=0, sticky='news')
-        item_frame.grid_columnconfigure(0, weight=1)
-        item_frame.grid_columnconfigure(1, weight=0)
-        item_frame.grid_rowconfigure(0, weight=1)
+        grid_init(view)
+
+        item_frame = ttk.Frame(view, style=self.theme.item_view.ik_name)
+        grid_init(item_frame, subcols=[(0, 1), (1, 0)])
 
         self.initialize_item_view(
             item_frame,
             gui_item=self.view_var, 
             )
         # TODO: add scrollbar?
 
         btn_frame = ttk.Frame(view)
-        btn_frame.grid(row=0, column=1, sticky='news')
-        btn_frame.grid_columnconfigure(0, weight=1)
+        grid_init(
+            btn_frame,
+            init_row_col=(0, 1),
+            subrows=[(i, 0) for i in range(5)]
+        )
 
+        # BUTTONS WHILE ON VIEW MODE
         self.new_item_buttons = {}
         for row_ix, item_type in enumerate(ITEM_TYPES):
-            btn_frame.grid_rowconfigure(row_ix, weight=0)
+            # btn_frame.grid_rowconfigure(row_ix, weight=0)
             self.new_item_buttons[item_type] = ttk.Button(
                 btn_frame,
                 text=f'New {item_type.__name__}',
                 command=partial(self.switch_to_edit_new, item_type),
                 state='normal'
             )
-            self.new_item_buttons[item_type].grid(row=row_ix, column=0, sticky=(N,))
+            self.new_item_buttons[item_type].grid(row=row_ix, column=0, sticky=(N, W, E))
 
         self.edit_button = ttk.Button(
             btn_frame,
             text='Edit',
             command=self.switch_to_edit,
+            state='disabled',
+            style=self.theme.button.ik_name
+        )
+        self.edit_button.grid(row=row_ix + 1, column=0, sticky=(N, W, E))
+        self.delete_button = ttk.Button(
+            btn_frame,
+            text='Delete',
+            command=self.delete,
             state='disabled'
         )
-        self.edit_button.grid(row=row_ix + 1, column=0, sticky=(N,))
+        self.delete_button.grid(row=row_ix + 2, column=0, sticky=(N, W, E))
 
         # Edit tab
         edit = ttk.Frame(self.view_nb)
-        edit.grid(row=0, column=0, sticky='news')
-        edit.grid_rowconfigure(0, weight=1)
-        edit.grid_columnconfigure(0, weight=1)
-        edit.grid_columnconfigure(1, weight=0)
+        grid_init(edit, subcols=[(0, 1), (1, 0)])
 
-        save_button = ttk.Button(
-            edit, text='Save', command=self.switch_to_view)
-        save_button.grid(row=0, column=1)
+        item_edit_frame = ttk.Frame(edit, style=self.theme.item_view.ik_name)
+        grid_init(item_edit_frame)
 
-        self.initialize_item_edit(edit)
+        self.initialize_item_edit(item_edit_frame)
+
+        # Buttons while on EDIT mode
+        edit_btn_frame = ttk.Frame(edit)
+        grid_init(
+            edit_btn_frame, 
+            init_row_col=(0, 1), 
+            subrows=[(i, 0) for i in range(2)]
+            )
+
+        save_button = ttk.Button(
+            edit_btn_frame, text='Save', command=self.switch_to_view)
+        save_button.grid(row=0, column=1, sticky=(N, W, E))
+        
+        self.cancel_button = ttk.Button(
+            edit_btn_frame,
+            text='Cancel',
+            command=self.cancel,
+        )
+        self.cancel_button.grid(row=1, column=1, sticky=(N, W, E))
 
         self.view_nb.add(view, text='View')
         self.view_nb.add(edit, text='Edit', state='hidden')
 
+    def cancel(self):
+        self.populate_edit_pane()
+        self.switch_to_view(save=False, update_view_var=False)
+
     def initialize_item_edit(self, frame):
+        """Create frames and labels for single item edition."""
         local_frame = ttk.Frame(frame)
-        local_frame.grid(row=0, column=0, sticky='news')
-        local_frame.grid_rowconfigure(0, weight=1)
-        local_frame.grid_rowconfigure(1, weight=1)
-        local_frame.grid_columnconfigure(0, weight=1)
-        local_frame.grid_columnconfigure(1, weight=1)
+        grid_init(
+            local_frame,
+            subrows=[(0, 0), (1, 0), (2, 1)],
+            subcols=[(0, 0), (1, 1)]
+        )
         
+        self.item_type_edit = ttk.Label(
+            local_frame, 
+            text='',
+            style=self.theme.generic_label.ik_name
+            )
+        self.item_type_edit.grid(row=0, column=0, sticky='news')
+
         item_name_descr = ttk.Label(local_frame, text='name')
-        item_name_descr.grid(row=0, column=0, sticky='e')
+        item_name_descr.grid(row=1, column=0, sticky='wen')
 
-        self.text['name'] = Text(local_frame)
-        # self.text['name'].insert('1.0', gui_item.name)
-        self.text['name'].grid(row=0, column=1, sticky='w')
+        self.text['name'] = Text(
+            local_frame, 
+            height=ONE_LINE_HEIGHT, 
+            font=DEFAULT_FONT
+            )
+        self.text['name'].grid(row=1, column=1, sticky='w')
 
         item_content_descr = ttk.Label(local_frame, text='content')
-        item_content_descr.grid(row=1, column=0, sticky='e')
+        item_content_descr.grid(row=2, column=0, sticky='wen')
         
-        self.text['content'] = Text(local_frame)
-        # self.text['content'].insert('1.0', gui_item.content)
-        self.text['content'].grid(row=1, column=1, sticky='w')
+        self.text['content'] = Text(local_frame, font=DEFAULT_FONT)
+        self.text['content'].grid(row=2, column=1, sticky='nwe')
 
     def switch_to_edit(self):
         """Switch focus from item view to item edition."""
+        self.populate_edit_pane()
         self.view_nb.tab(self.edit_id, state='normal')
         self.view_nb.select(self.edit_id)
     
     def switch_to_edit_new(self, item_cls: GUIItem):
         """Switch to edit tab for new item creation."""
         new_item = item_cls(name_var=StringVar(), content_var=StringVar())
         self.populate_view_pane(new_item)
+        self.populate_edit_pane()
         self.view_nb.tab(self.edit_id, state='normal')
         self.view_nb.select(self.edit_id)
 
-    def switch_to_view(self):
-        """When focus is on Edit tab; save and switch to View tab."""
+    def delete(self):
+        self.view_var.delete()
+        self.delete_button['state'] = 'disabled'
+        self.collect_search()
+        self.populate_edit_pane()
 
-        # content attr
-        content_str = self.text['content'].get('1.0', 'end')
-        self.view_var.update_content(content_str)
-
-        # name attr
-        name_str = self.text['name'].get('1.0', 'end')
-        self.view_var.update_name(name_str)
+    def switch_to_view(self, save: bool = True, update_view_var: bool = True):
+        """When focus is on Edit tab; save and switch to View tab."""
 
-        # save to DB
-        self.view_var.save()
+        if update_view_var:
+            # content attr
+            content_str = self.text['content'].get('1.0', 'end')
+            self.view_var.update_str_var('content_var', content_str, set_core_attr=True)
+
+            # name attr
+            name_str = self.text['name'].get('1.0', 'end')
+            self.view_var.update_str_var('name_var', name_str, set_core_attr=True)
+
+        if save:
+            # save to DB
+            ikid = self.view_var.save()
+
+            if self.debug:
+                itype = self.view_var.__class__.__name__
+                self.item_type['text'] = itype + ' ikid:' + str(ikid)
 
-        # refresh search results
-        self.collect_search()
+            # refresh search results
+            self.collect_search()
 
         # hide editor
         self.view_nb.tab(self.edit_id, state='hidden')
 
         # focus back on view
+        self.delete_button['state'] = 'normal'
+
         self.view_nb.select(self.view_id)
 
     def _initialize_filter_block(self):
         (ttk
          .Label(self.left_search_pane, text="filter")
          .grid(column=0, row=0, sticky=(N, W, E, S)))
 
@@ -288,157 +380,176 @@
                 offvalue=''
             ).grid(row=0, column=colix, sticky=(N, E, S, W))
 
     def _initialize_searchbar(self):
         ttk.Label(self.left_search_pane, text="search").grid(
             column=0, row=1, sticky='ens')
 
-        searchbar_style_name = 'Searchbar.TFrame'
-        self.searchbar_style = ttk.Style()
-        self.searchbar_style.configure(
-            searchbar_style_name,
-            background='orange',
-            foreground='black',
-            padding=5
-        )
         searchbar = ttk.Frame(
             self.left_search_pane,
-            style=searchbar_style_name,
+            style=self.theme.searchbar.ik_name,
         )
-        searchbar.grid(row=1, column=1, sticky=(E, W, N, S))
-        searchbar.grid_columnconfigure(0, weight=1)
-        searchbar.grid_rowconfigure(0, weight=1)
+        grid_init(searchbar, init_row_col=(1, 1))
 
         # inspired from: https://tkdocs.com/tutorial/widgets.html#entry (Validation section)
         search_entry = ttk.Entry(
             searchbar,
             textvariable=self.search_var,
             validate='key',
             validatecommand=(self.root.register(self.validate_search), '%P'),
-            font=('Century 9'),
-            width=ENTRY_DEFAULT_LENGTH
+            style=self.theme.generic_entry.ik_name,
+            font=DEFAULT_FONT
         )
-        search_entry.grid(row=0, column=0, sticky='news', pady=2)
+        search_entry.grid(row=0, column=0, sticky='news')  #, pady=2)
         search_entry.bind("<Return>", self.collect_search)
         search_entry.bind("<FocusOut>", self.collect_search)
         search_entry.bind("<KeyRelease>", self.collect_search)
 
     def _initialize_search_results(self):
         # --------------
         # OVERALL FRAME
         # --------------
         self.results_frame = ttk.Labelframe(
             self.left_panel,
             text='Results',
         )
-        self.results_frame.grid(row=0, column=0)
-        self.results_frame.grid_columnconfigure(0, weight=0)
-        self.results_frame.grid_columnconfigure(1, weight=1)
-        self.results_frame.grid_rowconfigure(0, weight=1)
+        grid_init(self.results_frame, subcols=[(0, 0), (1, 1)])
         self.left_panel.add(self.results_frame, weight=3)
 
         # ------------------
         # SCROLLABLE CANVAS
         # ------------------
         scroll_height = self.max_results * self.item_result_height
         scroll_width = 300
 
         scr = ttk.Scrollbar(self.results_frame, orient=VERTICAL)
         self.results_canvas = Canvas(
             self.results_frame,
             scrollregion=(0, 0, scroll_width, scroll_height),
             yscrollcommand=scr.set,
-            background='blue'
+            background=CANVAS_OPTIONS['search_results']['background']
         )
         scr['command'] = self.results_canvas.yview
         self.results_canvas.grid(column=1, row=0, sticky=(N, W, E, S))
         scr.grid(column=0, row=0, sticky=(N, S))
 
         # -------------------
         # DUMMY RESULT PANES
         # -------------------
         self.populate_search_results_canvas(self.search_results_list)
 
     def populate_search_results_canvas(self, results_list):
         # clear canvas
         result_tag = 'result_item'
         self.results_canvas.delete(result_tag)
+        # self.result_buttons = []
+        self.result_bools = []
         for result_ix, gui_item in enumerate(results_list):
-            search_result = ttk.Label(
+            mini_item_frame = ttk.Labelframe(
                 self.results_canvas,
-                textvariable=gui_item.name_var,
-                wraplength=WRAP_1,  # pixels
+                text=gui_item.__class__.__name__,
+                style=self.theme.item_snippet.ik_name
             )
+            
+            grid_init(mini_item_frame)
+
             self.view_callbacks[result_ix] = partial(
-                self.populate_view_pane, gui_item)
+                self.populate_view_pane, gui_item, source_ix=result_ix)
+            
+            result_bool = BooleanVar(value=gui_item == self.view_var)
+            search_result = ttk.Checkbutton(
+                mini_item_frame,
+                textvariable=gui_item.name_var,
+                command=self.view_callbacks[result_ix],
+                style=self.theme.item_button.ik_name,
+                variable=result_bool
+            )
+            self.result_bools.append(result_bool)
+            # self.result_buttons.append(search_result)
+            search_result.grid(row=0, column=0, sticky='news')
 
-            search_result.bind('<Button-1>', self.view_callbacks[result_ix])
+            mini_item_frame.bind('<Button-1>', self.view_callbacks[result_ix])
 
             _ = self.results_canvas.create_window(
                 0,
                 self.item_result_height * result_ix,
                 anchor='nw',
-                window=search_result,
+                window=mini_item_frame,
                 height=self.item_result_height,
-                tags=(result_tag)
+                tags=(result_tag,)
             )
 
-    def populate_view_pane(self, gui_item: GUIItem, *args):
+    def populate_view_pane(self, gui_item: GUIItem, *args, source_ix = None):
         """Populate View & Edit tabs with GUIItem data.
 
         This callback gets triggered when:
          - item from search results gets clicked upon, or,
-         - user clicks on create new Item
+         - user clicks on create new <Item>
 
         Args:
             gui_item (GUIItem): Item to use to populate data fields.
         """
         self.view_var = gui_item
+        self.item_type['text'] = self.view_var.__class__.__name__
+        if self.debug:
+            self.item_type['text'] += ' ikid:' + str(self.view_var._ikid)
+
         # TODO: think about improving below logic
         self.item_view_name_label['textvariable'] = self.view_var.name_var
         self.item_view_content_label['textvariable'] = self.view_var.content_var
 
+        # enable delete button if gui_item exists in DB
+        if gui_item.exists_in_db:
+            self.delete_button['state'] = 'normal'
+
         # enable editing
         self.edit_button['state'] = 'normal'
+        self.cancel_button['state'] = 'normal'  # acts as "reload" button
+
+        # deselect all other result buttons
+        if source_ix is not None:
+            for ix, bool_ in enumerate(self.result_bools):
+                if ix != source_ix:
+                    bool_.set(False)
+
+    def populate_edit_pane(self, gui_item: Optional[GUIItem] = None):
+        """Populate text widget with self.view_var or provided GUIItem."""
+        if gui_item is None:
+            gui_item = self.view_var
+        
+        # display which Item type is being edited
+        self.item_type_edit['text'] = gui_item.__class__.__name__
+        if self.debug:
+            self.item_type_edit['text'] += ' ikid:' + str(gui_item._ikid)
 
-        # update Text widgets for future edits
-        for attr_name in ['name', 'content']:
+        # populate Text widgets for edition
+        for attr_name in gui_item.displayable:
             self.text[attr_name].delete('1.0', 'end')
-            self.text[attr_name].insert('1.0', getattr(self.view_var, attr_name))
+            to_insert = getattr(gui_item, attr_name)
+            if to_insert:
+                self.text[attr_name].insert('1.0', to_insert)
 
     def _initialize_left_panel(self):
         """Setup left panel in main frame."""
-        # -----------------
-        # LEFT PANEL STYLE
-        # -----------------
-        left_panel_style_name = 'Leftpanel.TLabelframe'
-        left_panel_style = ttk.Style()
-        left_panel_style.configure(
-            left_panel_style_name,
-            background='yellow',
-            foreground='black',
-            padding=10
-        )
-
         # -------------------------
         # LEFT PANEL WINDOWED PANE
         # -------------------------
         self.left_panel = ttk.PanedWindow(self.mainframe, orient=VERTICAL)
 
         self.left_search_pane = ttk.Labelframe(
             self.left_panel,
             relief="ridge",
-            style=left_panel_style_name,
+            style=self.theme.left_panel.ik_name,
             text='Search'
         )
-        self.left_search_pane.grid(column=0, row=0, sticky='news')
-        self.left_search_pane.grid_rowconfigure(0, weight=0)
-        self.left_search_pane.grid_columnconfigure(0, weight=0)
-        self.left_search_pane.grid_rowconfigure(1, weight=1)
-        self.left_search_pane.grid_columnconfigure(1, weight=1)
+        grid_init(
+            self.left_search_pane,
+            subrows=[(0, 0), (1, 1)],
+            subcols=[(0, 0), (1, 1)]
+        )
 
         self.left_panel.add(self.left_search_pane, weight=0)
         self.left_panel.bind('<<filter-update>>', self.collect_search)
 
         self._initialize_filter_block()
         self._initialize_searchbar()
         self._initialize_search_results()
@@ -459,77 +570,112 @@
     def collect_search(self, *args):
         """Collect search parameters and triggers search.
 
         This callback gets called when:
         - a <<filter-update>> event happens
         - a change happens in search bar entry
         - user clicks "Save" on edit tab
+        - user loads persisted DB
 
         This method calls refresh_results method to update
         results list.
         """
         vars = {}
         vars['filters'] = self.filters
         vars['search'] = self.search_var.get()
 
         self.refresh_results(vars)
 
+    def clear_all_search(self):
+        self.filters = []
+
+        # deselect all radio buttons
+        for var in self.filter_vars.values():
+            var.set('')
+
+        self.search_var.set('')
+
     def refresh_results(self, search_params: Optional[Mapping] = None):
         """Trigger backend search using search parameters.
 
         This method also updates results on GUI.
 
         Args:
             search_params (Optional[Mapping], optional): Search parameters. Defaults to None.
 
         Raises:
             NotImplementedError: If search_params is not None.
         """
         self.search_results_list = []
-        # TODO: current logic ignores searchbar
         # TODO: setup logging instead of print() below
 
-        # print(f"{search_params=}")
         if search_params is not None:
             item_type_filter = [NAME_TO_ITEM_TYPE[f] for f in search_params['filters']]
             search_str = search_params['search']
             if search_str:
                 item_buckets = filter_str(search_str, item_type_filter)
             else:
                 item_buckets = list_all_items(item_type_filter)
-            # print(f"   {item_buckets=}")
         else:
             item_buckets = list_all_items()
 
         # TODO: keep item types separate below
         item_list = []
         for ll in item_buckets.values():
             item_list += ll
-        # print(f"   {item_list=}")
         for result_ix, core_item in enumerate(item_list):
             gui_item = core_to_gui_item(
                 core_item,
                 name_var=StringVar(value=core_item.name),
                 content_var=StringVar(value=core_item.content),
                 )
             self.search_results_list.append(gui_item)
             self.ikid_to_result_slot[gui_item._ikid] = result_ix
-        # print(f"   {self.search_results_list=}")
         self.populate_search_results_canvas(self.search_results_list)
 
-def main():
+    def _initialize_view_var(self):
+        return GUIItem(
+                name_var=StringVar(value=self._default_str),
+                content_var=StringVar(value=self._default_str),
+                name=self._default_str, 
+                content=self._default_str
+                )
+
+    def persist_box(self):
+        filename = filedialog.asksaveasfilename(initialdir=DEFAULT_PERSISTENCE_DIR)
+        persist(filename)
+
+    def load_box(self):
+        filename = filedialog.askopenfilename(initialdir=DEFAULT_PERSISTENCE_DIR)
+        load_from_file(filename)
+        neutral_item = self._initialize_view_var()
+        self.populate_view_pane(neutral_item)
+        self.clear_all_search()
+        self.collect_search()
+
+
+    def create_main_menu(self):
+        win = self.root
+        menubar = Menu(win)
+        menu_file = Menu(menubar)
+        menu_file.add_command(label='Persist Session', command=self.persist_box)
+        menu_file.add_command(label='Load Session', command=self.load_box)
+        menubar.add_cascade(menu=menu_file, label='File')
+        win['menu'] = menubar
+        return win
+
+
+def main(debug: bool = False):
     """Launch main Tkinter event loop."""
     root = Tk()
+    root.option_add('*tearOff', FALSE)
     root.title(f"indiek-gui v{__version__}")
     root.columnconfigure(0, weight=1)
     root.rowconfigure(0, weight=1)
 
-    # for some reason width and height below have no effect
-    root.configure(width=2000, height=1000)
-
-    Orchestrator(root)
+    Orchestrator(root, debug=debug)
 
     root.mainloop()
 
 
 if __name__ == '__main__':
-    main()
+    main(True)
```

### Comparing `indiek-gui-0.0.3/indiek_gui.egg-info/PKG-INFO` & `indiek-gui-0.0.4/indiek_gui.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: indiek-gui
-Version: 0.0.3
+Version: 0.0.4
 Summary: Tkinter GUI for IndieK
 Home-page: https://pypi.org/project/indiek-gui/
 Author: Adrian Ernesto Radillo
 Author-email: adrian.radillo@gmail.com
 License: GNU Affero General Public License v3.0
 Project-URL: GitHub, https://github.com/indiek/indiek-gui
 Project-URL: Documentation, https://indiekgui.readthedocs.io/en/latest/
```

### Comparing `indiek-gui-0.0.3/setup.py` & `indiek-gui-0.0.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,23 +4,23 @@
 this_dir = abspath(dirname(__file__))
 with open(join(this_dir, 'README.rst'), encoding='utf-8') as file:
     long_description = file.read()
 
 setup(
     name='indiek-gui',
     python_requires='>=3.8',
-    version='0.0.3',
+    version='0.0.4',
     url='https://pypi.org/project/indiek-gui/',
     description='Tkinter GUI for IndieK',
     long_description=long_description,
     author='Adrian Ernesto Radillo',
     author_email='adrian.radillo@gmail.com',
     license='GNU Affero General Public License v3.0',
     packages=['indiek.gui'],
-    install_requires=['indiek-core == 0.1.3'],
+    install_requires=['indiek-core == 0.1.4'],
     extras_require={
         'dev': [
             'pytest',
             'pytest-pep8',
             'pytest-cov'
         ]
     },
```

