# Comparing `tmp/pydetex-1.0.1.tar.gz` & `tmp/pydetex-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydetex-1.0.1.tar", last modified: Sun May  7 20:52:57 2023, max compression
+gzip compressed data, was "pydetex-1.0.2.tar", last modified: Thu May 18 18:39:53 2023, max compression
```

## Comparing `pydetex-1.0.1.tar` & `pydetex-1.0.2.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxrwxrwx   0        0        0        0 2023-05-07 20:52:54.820000 pydetex-1.0.1/
--rw-rw-rw-   0        0        0     1073 2021-10-03 21:53:42.000000 pydetex-1.0.1/LICENSE
--rw-rw-rw-   0        0        0      406 2021-11-01 21:25:22.000000 pydetex-1.0.1/MANIFEST.in
--rw-rw-rw-   0        0        0     5567 2023-05-07 20:52:58.000000 pydetex-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     4370 2023-03-08 22:09:00.000000 pydetex-1.0.1/README.rst
-drwxrwxrwx   0        0        0        0 2023-05-07 20:52:54.880000 pydetex-1.0.1/pydetex/
--rw-rw-rw-   0        0        0      721 2022-02-03 13:19:14.000000 pydetex-1.0.1/pydetex/__init__.py
--rw-rw-rw-   0        0        0     1314 2021-11-14 20:58:54.000000 pydetex-1.0.1/pydetex/_fonts.py
--rw-rw-rw-   0        0        0    25324 2023-05-07 18:03:40.000000 pydetex-1.0.1/pydetex/_gui_settings.py
--rw-rw-rw-   0        0        0    45460 2023-02-15 12:36:58.000000 pydetex-1.0.1/pydetex/_gui_utils.py
--rw-rw-rw-   0        0        0    23466 2023-05-07 20:24:00.000000 pydetex-1.0.1/pydetex/_symbols.py
--rw-rw-rw-   0        0        0     9705 2023-02-15 12:36:20.000000 pydetex-1.0.1/pydetex/_utils_lang.py
--rw-rw-rw-   0        0        0    23887 2023-02-15 12:36:20.000000 pydetex-1.0.1/pydetex/_utils_tex.py
--rw-rw-rw-   0        0        0    30942 2022-05-13 22:07:20.000000 pydetex-1.0.1/pydetex/gui.py
--rw-rw-rw-   0        0        0    45728 2023-05-07 20:39:50.000000 pydetex-1.0.1/pydetex/parsers.py
--rw-rw-rw-   0        0        0     3887 2023-05-07 20:26:56.000000 pydetex-1.0.1/pydetex/pipelines.py
-drwxrwxrwx   0        0        0        0 2023-05-07 20:52:54.990000 pydetex-1.0.1/pydetex/res/
--rw-rw-rw-   0        0        0     4286 2021-10-13 18:08:22.000000 pydetex-1.0.1/pydetex/res/cog.ico
--rw-rw-rw-   0        0        0     4286 2021-10-18 04:07:18.000000 pydetex-1.0.1/pydetex/res/dictionary.ico
--rw-rw-rw-   0        0        0    13224 2021-09-14 16:31:46.000000 pydetex-1.0.1/pydetex/res/icon.gif
--rw-rw-rw-   0        0        0     4286 2021-10-13 18:08:22.000000 pydetex-1.0.1/pydetex/res/icon.ico
--rw-rw-rw-   0        0        0      554 2021-11-14 20:58:54.000000 pydetex-1.0.1/pydetex/res/placeholder_en.tex
--rw-rw-rw-   0        0        0      605 2021-11-14 20:58:54.000000 pydetex-1.0.1/pydetex/res/placeholder_es.tex
--rw-rw-rw-   0        0        0   184280 2021-10-16 20:19:00.000000 pydetex-1.0.1/pydetex/res/stopwords.json
--rw-rw-rw-   0        0        0      227 2020-02-26 08:23:30.000000 pydetex-1.0.1/pydetex/res/u_subscripts.txt
--rw-rw-rw-   0        0        0      416 2020-02-26 08:23:30.000000 pydetex-1.0.1/pydetex/res/u_superscripts.txt
--rw-rw-rw-   0        0        0     4861 2020-02-26 08:23:30.000000 pydetex-1.0.1/pydetex/res/u_symbols.txt
--rw-rw-rw-   0        0        0      427 2020-02-26 08:23:30.000000 pydetex-1.0.1/pydetex/res/u_textbb.txt
--rw-rw-rw-   0        0        0      900 2020-02-26 08:23:30.000000 pydetex-1.0.1/pydetex/res/u_textbf.txt
--rw-rw-rw-   0        0        0      364 2020-02-26 08:23:30.000000 pydetex-1.0.1/pydetex/res/u_textcal.txt
--rw-rw-rw-   0        0        0      359 2020-02-26 08:23:30.000000 pydetex-1.0.1/pydetex/res/u_textfrak.txt
--rw-rw-rw-   0        0        0      829 2020-02-26 08:23:30.000000 pydetex-1.0.1/pydetex/res/u_textit.txt
--rw-rw-rw-   0        0        0      434 2020-02-26 08:23:30.000000 pydetex-1.0.1/pydetex/res/u_textmono.txt
--rw-rw-rw-   0        0        0     8362 2023-05-07 20:35:20.000000 pydetex-1.0.1/pydetex/utils.py
--rw-rw-rw-   0        0        0      789 2023-05-07 20:13:54.000000 pydetex-1.0.1/pydetex/version.py
-drwxrwxrwx   0        0        0        0 2023-05-07 20:52:54.930000 pydetex-1.0.1/pydetex.egg-info/
--rw-rw-rw-   0        0        0     5567 2023-05-07 20:52:54.000000 pydetex-1.0.1/pydetex.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      870 2023-05-07 20:52:56.000000 pydetex-1.0.1/pydetex.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-07 20:52:56.000000 pydetex-1.0.1/pydetex.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      284 2023-05-07 20:52:56.000000 pydetex-1.0.1/pydetex.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-05-07 20:52:56.000000 pydetex-1.0.1/pydetex.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      173 2023-05-01 22:26:04.000000 pydetex-1.0.1/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-05-07 20:52:58.000000 pydetex-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1872 2023-04-13 16:52:48.000000 pydetex-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-18 18:39:52.880000 pydetex-1.0.2/
+-rw-rw-rw-   0        0        0     1073 2021-10-03 21:53:42.000000 pydetex-1.0.2/LICENSE
+-rw-rw-rw-   0        0        0      406 2021-11-01 21:25:22.000000 pydetex-1.0.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     5567 2023-05-18 18:39:54.000000 pydetex-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     4370 2023-03-08 22:09:00.000000 pydetex-1.0.2/README.rst
+drwxrwxrwx   0        0        0        0 2023-05-18 18:39:52.890000 pydetex-1.0.2/pydetex/
+-rw-rw-rw-   0        0        0      721 2022-02-03 13:19:14.000000 pydetex-1.0.2/pydetex/__init__.py
+-rw-rw-rw-   0        0        0     1382 2023-05-18 16:56:00.000000 pydetex-1.0.2/pydetex/_fonts.py
+-rw-rw-rw-   0        0        0    25324 2023-05-07 18:03:40.000000 pydetex-1.0.2/pydetex/_gui_settings.py
+-rw-rw-rw-   0        0        0    45460 2023-02-15 12:36:58.000000 pydetex-1.0.2/pydetex/_gui_utils.py
+-rw-rw-rw-   0        0        0    23466 2023-05-07 20:24:00.000000 pydetex-1.0.2/pydetex/_symbols.py
+-rw-rw-rw-   0        0        0     9705 2023-02-15 12:36:20.000000 pydetex-1.0.2/pydetex/_utils_lang.py
+-rw-rw-rw-   0        0        0    23887 2023-02-15 12:36:20.000000 pydetex-1.0.2/pydetex/_utils_tex.py
+-rw-rw-rw-   0        0        0    31212 2023-05-18 16:53:30.000000 pydetex-1.0.2/pydetex/gui.py
+-rw-rw-rw-   0        0        0    46327 2023-05-18 17:05:18.000000 pydetex-1.0.2/pydetex/parsers.py
+-rw-rw-rw-   0        0        0     3887 2023-05-07 20:26:56.000000 pydetex-1.0.2/pydetex/pipelines.py
+drwxrwxrwx   0        0        0        0 2023-05-18 18:39:52.900000 pydetex-1.0.2/pydetex/res/
+-rw-rw-rw-   0        0        0     4286 2021-10-13 18:08:24.000000 pydetex-1.0.2/pydetex/res/cog.ico
+-rw-rw-rw-   0        0        0     4286 2021-10-18 04:07:20.000000 pydetex-1.0.2/pydetex/res/dictionary.ico
+-rw-rw-rw-   0        0        0    13224 2021-09-14 16:31:46.000000 pydetex-1.0.2/pydetex/res/icon.gif
+-rw-rw-rw-   0        0        0     4286 2021-10-13 18:08:24.000000 pydetex-1.0.2/pydetex/res/icon.ico
+-rw-rw-rw-   0        0        0      554 2021-11-14 20:58:54.000000 pydetex-1.0.2/pydetex/res/placeholder_en.tex
+-rw-rw-rw-   0        0        0      605 2021-11-14 20:58:54.000000 pydetex-1.0.2/pydetex/res/placeholder_es.tex
+-rw-rw-rw-   0        0        0   184280 2021-10-16 20:19:00.000000 pydetex-1.0.2/pydetex/res/stopwords.json
+-rw-rw-rw-   0        0        0      227 2020-02-26 08:23:30.000000 pydetex-1.0.2/pydetex/res/u_subscripts.txt
+-rw-rw-rw-   0        0        0      416 2020-02-26 08:23:30.000000 pydetex-1.0.2/pydetex/res/u_superscripts.txt
+-rw-rw-rw-   0        0        0     4861 2020-02-26 08:23:30.000000 pydetex-1.0.2/pydetex/res/u_symbols.txt
+-rw-rw-rw-   0        0        0      427 2020-02-26 08:23:30.000000 pydetex-1.0.2/pydetex/res/u_textbb.txt
+-rw-rw-rw-   0        0        0      900 2020-02-26 08:23:30.000000 pydetex-1.0.2/pydetex/res/u_textbf.txt
+-rw-rw-rw-   0        0        0      364 2020-02-26 08:23:30.000000 pydetex-1.0.2/pydetex/res/u_textcal.txt
+-rw-rw-rw-   0        0        0      359 2020-02-26 08:23:30.000000 pydetex-1.0.2/pydetex/res/u_textfrak.txt
+-rw-rw-rw-   0        0        0      829 2020-02-26 08:23:30.000000 pydetex-1.0.2/pydetex/res/u_textit.txt
+-rw-rw-rw-   0        0        0      434 2020-02-26 08:23:30.000000 pydetex-1.0.2/pydetex/res/u_textmono.txt
+-rw-rw-rw-   0        0        0     8362 2023-05-07 20:35:20.000000 pydetex-1.0.2/pydetex/utils.py
+-rw-rw-rw-   0        0        0      789 2023-05-18 16:57:32.000000 pydetex-1.0.2/pydetex/version.py
+drwxrwxrwx   0        0        0        0 2023-05-18 18:39:52.900000 pydetex-1.0.2/pydetex.egg-info/
+-rw-rw-rw-   0        0        0     5567 2023-05-18 18:39:54.000000 pydetex-1.0.2/pydetex.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      870 2023-05-18 18:39:54.000000 pydetex-1.0.2/pydetex.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-18 18:39:54.000000 pydetex-1.0.2/pydetex.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      284 2023-05-18 18:39:54.000000 pydetex-1.0.2/pydetex.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-05-18 18:39:54.000000 pydetex-1.0.2/pydetex.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      173 2023-05-01 22:26:04.000000 pydetex-1.0.2/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-05-18 18:39:54.000000 pydetex-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1872 2023-04-13 16:52:48.000000 pydetex-1.0.2/setup.py
```

### Comparing `pydetex-1.0.1/LICENSE` & `pydetex-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pydetex-1.0.1/PKG-INFO` & `pydetex-1.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydetex
-Version: 1.0.1
+Version: 1.0.2
 Summary: An application that transforms LaTeX code to plain text
 Home-page: https://pydetex.readthedocs.io
 Author: Pablo Pizarro R.
 Author-email: pablo@ppizarror.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/ppizarror/PyDetex/issues
 Project-URL: Documentation, https://pydetex.readthedocs.io
```

### Comparing `pydetex-1.0.1/README.rst` & `pydetex-1.0.2/README.rst`

 * *Files identical despite different names*

### Comparing `pydetex-1.0.1/pydetex/__init__.py` & `pydetex-1.0.2/pydetex/__init__.py`

 * *Files identical despite different names*

### Comparing `pydetex-1.0.1/pydetex/_fonts.py` & `pydetex-1.0.2/pydetex/_fonts.py`

 * *Files 13% similar despite different names*

```diff
@@ -33,21 +33,23 @@
     'bold': {weight: bold},
     'bold_italic': {weight: bold, slant: italic},
     'bullet': None,
     'equation_char': {weight: bold, fg: '#19b70a'},
     'equation_inside': {slant: italic, fg: '#ffa450'},
     'error': {fg: '#ff6b68'},
     'h1': {size: 2, weight: bold, spacing3: 1},
+    'highlight': {bg: '#fff200'},
     'italic': {slant: italic},
     'link': {weight: bold, fg: '#ff02a6'},
     'normal': {},
     'repeated_tag': {slant: italic, fg: '#ff002b'},
     'repeated_word': {weight: bold},
-    'tex_command': {fg: '#09accb'},
+    'strike': {overstrike: True},
     'tex_argument': {fg: '#999999'},
+    'tex_command': {fg: '#09accb'},
     'underlined': {underline: True, spacing3: 1}
 }
 
 # Configure the tags
 FONT_TAGS: Dict[str, str] = {}
 TAGS_FONT: Dict[str, str] = {}
 for k in FONT_PROPERTIES.keys():
```

### Comparing `pydetex-1.0.1/pydetex/_gui_settings.py` & `pydetex-1.0.2/pydetex/_gui_settings.py`

 * *Files identical despite different names*

### Comparing `pydetex-1.0.1/pydetex/_gui_utils.py` & `pydetex-1.0.2/pydetex/_gui_utils.py`

 * *Files identical despite different names*

### Comparing `pydetex-1.0.1/pydetex/_symbols.py` & `pydetex-1.0.2/pydetex/_symbols.py`

 * *Files identical despite different names*

### Comparing `pydetex-1.0.1/pydetex/_utils_lang.py` & `pydetex-1.0.2/pydetex/_utils_lang.py`

 * *Files identical despite different names*

### Comparing `pydetex-1.0.1/pydetex/_utils_tex.py` & `pydetex-1.0.2/pydetex/_utils_tex.py`

 * *Files identical despite different names*

### Comparing `pydetex-1.0.1/pydetex/gui.py` & `pydetex-1.0.2/pydetex/gui.py`

 * *Files 1% similar despite different names*

```diff
@@ -515,19 +515,22 @@
             self._copy_clip_button['state'] = tk.NORMAL
 
         # Font format
         font_format = self._cfg.get(self._cfg.CFG_OUTPUT_FONT_FORMAT)
         par.FONT_FORMAT_SETTINGS['bold'] = FONT_TAGS['bold'] if font_format else ''
         par.FONT_FORMAT_SETTINGS['cite'] = FONT_TAGS['link'] if font_format else ''
         par.FONT_FORMAT_SETTINGS['equation'] = FONT_TAGS['equation_inside'] if font_format else ''
+        par.FONT_FORMAT_SETTINGS['hl'] = FONT_TAGS['highlight'] if font_format else ''
         par.FONT_FORMAT_SETTINGS['italic'] = FONT_TAGS['italic'] if font_format else ''
         par.FONT_FORMAT_SETTINGS['normal'] = FONT_TAGS['normal'] if font_format else ''
         par.FONT_FORMAT_SETTINGS['ref'] = FONT_TAGS['link'] if font_format else ''
+        par.FONT_FORMAT_SETTINGS['strike'] = FONT_TAGS['strike'] if font_format else ''
         par.FONT_FORMAT_SETTINGS['tex_text_tag'] = FONT_TAGS['bold'] if font_format else ''
         par.FONT_FORMAT_SETTINGS['tex_text_tag_content'] = FONT_TAGS['italic'] if font_format else ''
+        par.FONT_FORMAT_SETTINGS['underline'] = FONT_TAGS['underlined'] if font_format else ''
 
         # Process the text and get the language
         # noinspection PyBroadException
         try:
             out = self.pipeline(
                 text,
                 self._detected_lang_tag,
```

### Comparing `pydetex-1.0.1/pydetex/parsers.py` & `pydetex-1.0.2/pydetex/parsers.py`

 * *Files 1% similar despite different names*

```diff
@@ -79,19 +79,22 @@
 # Parser font format. This dict stores the font of some tex elements to be represented
 # in the GUI text editor. The values are the same of _fonts.FONT_TAGS. By default,
 # they are empty, and are updated in the PyDetexGUI._process() method
 FONT_FORMAT_SETTINGS = {
     'bold': '',
     'cite': '',
     'equation': '',
+    'hl': '',
     'italic': '',
     'normal': '',
     'ref': '',
+    'strike': '',
     'tex_text_tag': '',
-    'tex_text_tag_content': ''
+    'tex_text_tag_content': '',
+    'underline': ''
 }
 
 LANG_TT_TAGS = ut.LangTexTextTags()
 
 
 def _find_str(s: str, char: str) -> int:
     """
@@ -711,22 +714,24 @@
     # relaced is 'YOUR TAG {0}, {1}
     # All *arguments will be formatted using the tag
     commands: List[Tuple[str, List[Tuple[int, bool]], Union[str, Callable[[str, ...], str]], int, Optional[str], Optional[str], Tuple[bool, bool]]] = [
         ('ac', [(1, False)], '{0}', 1, 'normal', 'normal', (False, False)),  # Acronym
         ('acf', [(1, False)], '{0}', 1, 'normal', 'normal', (False, False)),  # Acronym
         ('acl', [(1, False)], '{0}', 1, 'normal', 'normal', (False, False)),  # Acronym
         ('acs', [(1, False)], '{0}', 1, 'normal', 'normal', (False, False)),  # Acronym
+        ('cancel', [(1, False)], '{0}', 1, 'normal', 'strike', (False, False)),
         ('caption', [(1, False)], LANG_TT_TAGS.get(lang, 'caption'), 1, None, None, (False, True)),
         ('chapter', [(1, False)], '{0}', 1, 'normal', 'bold', (True, True)),
         ('chapter*', [(1, False)], '{0}', 1, 'normal', 'bold', (True, True)),
         ('doublequotes', [(1, False)], lambda t: '"{0}"'.format(t), 1, 'normal', 'normal', (False, False)),
         ('em', [(1, False)], '{0}', 1, 'normal', 'bold', (False, False)),
         ('emph', [(1, False)], '{0}', 1, 'normal', 'italic', (False, False)),
         ('enquote', [(1, False)], lambda t: '"{0}"'.format(t), 1, 'normal', 'normal', (False, False)),
         ('frac', [(1, False), (2, False)], '{0}/{1}', 2, 'normal', 'normal', (False, False)),
+        ('hl', [(1, False)], '{0}', 1, 'normal', 'hl', (False, False)),
         ('href', [(2, False)], LANG_TT_TAGS.get(lang, 'link'), 2, None, None, (False, False)),
         ('insertimage', [(3, False)], LANG_TT_TAGS.get(lang, 'figure_caption'), 3, None, None, (False, True)),  # (Template) Informe
         ('insertimage', [(4, False)], LANG_TT_TAGS.get(lang, 'figure_caption'), 4, None, None, (False, False)),  # (Template) Informe
         ('insertimageboxed', [(4, False)], LANG_TT_TAGS.get(lang, 'figure_caption'), 4, None, None, (False, True)),  # (Template) Informe
         ('insertimageboxed', [(5, False)], LANG_TT_TAGS.get(lang, 'figure_caption'), 5, None, None, (False, True)),  # (Template) Informe
         ('institutionentry', [(1, False), (2, False), (3, False), (4, False)], '{0} ({1}-{2}). {3}', 4, 'normal', 'normal', (False, False)),  # (Template) Professional-CV
         ('institutionentryshort', [(1, False), (2, False), (3, False), (4, False)], '{0} ({1}-{2}). {3}', 4, 'normal', 'normal', (False, False)),  # (Template) Professional-CV
@@ -734,25 +739,30 @@
         ('MakeLowercase', [(1, False)], lambda t: t.lower(), 1, 'normal', 'normal', (False, False)),
         ('MakeUppercase', [(1, False)], lambda t: t.upper(), 1, 'normal', 'normal', (False, False)),
         ('otherentry', [(1, False), (2, False)], '{0} {1}', 2, 'normal', 'normal', (False, False)),  # (Template) Professional-CV
         ('paragraph', [(1, False)], '{0}', 1, 'normal', 'bold', (True, True)),
         ('quotes', [(1, False)], lambda t: '"{0}"'.format(t), 1, 'normal', 'normal', (False, False)),
         ('section', [(1, False)], '{0}', 1, 'normal', 'bold', (True, True)),
         ('section*', [(1, False)], '{0}', 1, 'normal', 'bold', (True, True)),
+        ('so', [(1, False)], '{0}', 1, 'normal', 'normal', (False, False)),
+        ('sout', [(1, False)], '{0}', 1, 'normal', 'strike', (False, False)),
+        ('st', [(1, False)], '{0}', 1, 'normal', 'strike', (False, False)),
         ('subfloat', [(1, True)], LANG_TT_TAGS.get(lang, 'sub_figure_title'), 1, None, None, (False, True)),
         ('subparagraph', [(1, False)], '{0}', 1, 'normal', 'bold', (True, True)),
         ('subsection', [(1, False)], '{0}', 1, 'normal', 'bold', (True, True)),
         ('subsection*', [(1, False)], '{0}', 1, 'normal', 'bold', (True, True)),
         ('subsubsection', [(1, False)], '{0}', 1, 'normal', 'bold', (True, True)),
         ('subsubsection*', [(1, False)], '{0}', 1, 'normal', 'bold', (True, True)),
         ('subsubsubsection', [(1, False)], '{0}', 1, 'normal', 'bold', (True, True)),
         ('subsubsubsection*', [(1, False)], '{0}', 1, 'normal', 'bold', (True, True)),
+        ('text', [(1, False)], '{0}', 1, 'normal', 'normal', (False, False)),
         ('textbf', [(1, False)], '{0}', 1, 'normal', 'bold', (False, False)),
         ('textit', [(1, False)], '{0}', 1, 'normal', 'italic', (False, False)),
         ('texttt', [(1, False)], '{0}', 1, 'normal', 'normal', (False, False)),
+        ('underline', [(1, False)], '{0}', 1, 'normal', 'underline', (False, False)),
         ('uppercase', [(1, False)], lambda t: t.upper(), 1, 'normal', 'normal', (False, False))
     ]
     new_s = ''
 
     # Get the commands
     cmd_args = ut.get_tex_commands_args(s)
     for c in cmd_args:
```

### Comparing `pydetex-1.0.1/pydetex/pipelines.py` & `pydetex-1.0.2/pydetex/pipelines.py`

 * *Files identical despite different names*

### Comparing `pydetex-1.0.1/pydetex/res/cog.ico` & `pydetex-1.0.2/pydetex/res/cog.ico`

 * *Files identical despite different names*

### Comparing `pydetex-1.0.1/pydetex/res/dictionary.ico` & `pydetex-1.0.2/pydetex/res/dictionary.ico`

 * *Files identical despite different names*

### Comparing `pydetex-1.0.1/pydetex/res/icon.gif` & `pydetex-1.0.2/pydetex/res/icon.gif`

 * *Files identical despite different names*

### Comparing `pydetex-1.0.1/pydetex/res/icon.ico` & `pydetex-1.0.2/pydetex/res/icon.ico`

 * *Files identical despite different names*

### Comparing `pydetex-1.0.1/pydetex/res/placeholder_en.tex` & `pydetex-1.0.2/pydetex/res/placeholder_en.tex`

 * *Files identical despite different names*

### Comparing `pydetex-1.0.1/pydetex/res/placeholder_es.tex` & `pydetex-1.0.2/pydetex/res/placeholder_es.tex`

 * *Files identical despite different names*

### Comparing `pydetex-1.0.1/pydetex/res/stopwords.json` & `pydetex-1.0.2/pydetex/res/stopwords.json`

 * *Files identical despite different names*

### Comparing `pydetex-1.0.1/pydetex/res/u_symbols.txt` & `pydetex-1.0.2/pydetex/res/u_symbols.txt`

 * *Files identical despite different names*

### Comparing `pydetex-1.0.1/pydetex/res/u_textbf.txt` & `pydetex-1.0.2/pydetex/res/u_textbf.txt`

 * *Files identical despite different names*

### Comparing `pydetex-1.0.1/pydetex/res/u_textit.txt` & `pydetex-1.0.2/pydetex/res/u_textit.txt`

 * *Files identical despite different names*

### Comparing `pydetex-1.0.1/pydetex/utils.py` & `pydetex-1.0.2/pydetex/utils.py`

 * *Files identical despite different names*

### Comparing `pydetex-1.0.1/pydetex/version.py` & `pydetex-1.0.2/pydetex/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,10 +28,10 @@
         return '{}.{}.{}'.format(*self)
 
     major = property(lambda self: self[0])
     minor = property(lambda self: self[1])
     patch = property(lambda self: self[2])
 
 
-vernum = Version(1, 0, 1)
+vernum = Version(1, 0, 2)
 ver = str(vernum)
 rev = ''
```

### Comparing `pydetex-1.0.1/pydetex.egg-info/PKG-INFO` & `pydetex-1.0.2/pydetex.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydetex
-Version: 1.0.1
+Version: 1.0.2
 Summary: An application that transforms LaTeX code to plain text
 Home-page: https://pydetex.readthedocs.io
 Author: Pablo Pizarro R.
 Author-email: pablo@ppizarror.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/ppizarror/PyDetex/issues
 Project-URL: Documentation, https://pydetex.readthedocs.io
```

### Comparing `pydetex-1.0.1/pydetex.egg-info/SOURCES.txt` & `pydetex-1.0.2/pydetex.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pydetex-1.0.1/setup.py` & `pydetex-1.0.2/setup.py`

 * *Files identical despite different names*

