# Comparing `tmp/prev_gen-2.0.2-py3-none-any.whl.zip` & `tmp/prev_gen-2.0.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 71013 bytes, number of entries: 8
+Zip file size: 71040 bytes, number of entries: 8
 -rw-rw-rw-  2.0 fat      102 b- defN 23-May-10 10:44 prev_gen/__init__.py
 -rw-rw-rw-  2.0 fat     1340 b- defN 23-Feb-11 16:01 prev_gen/example.txt
--rw-rw-rw-  2.0 fat    46822 b- defN 23-May-10 15:41 prev_gen/main.py
+-rw-rw-rw-  2.0 fat    46894 b- defN 23-May-10 15:48 prev_gen/main.py
 -rw-rw-rw-  2.0 fat   125452 b- defN 22-Sep-22 05:27 prev_gen/nunito.ttf
--rw-rw-rw-  2.0 fat     2471 b- defN 23-May-10 15:43 prev_gen-2.0.2.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-May-10 15:43 prev_gen-2.0.2.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        9 b- defN 23-May-10 15:43 prev_gen-2.0.2.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      606 b- defN 23-May-10 15:43 prev_gen-2.0.2.dist-info/RECORD
-8 files, 176894 bytes uncompressed, 69969 bytes compressed:  60.4%
+-rw-rw-rw-  2.0 fat     2508 b- defN 23-May-18 14:42 prev_gen-2.0.4.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-May-18 14:42 prev_gen-2.0.4.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        9 b- defN 23-May-18 14:42 prev_gen-2.0.4.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      606 b- defN 23-May-18 14:42 prev_gen-2.0.4.dist-info/RECORD
+8 files, 177003 bytes uncompressed, 69996 bytes compressed:  60.5%
```

## zipnote {}

```diff
@@ -6,20 +6,20 @@
 
 Filename: prev_gen/main.py
 Comment: 
 
 Filename: prev_gen/nunito.ttf
 Comment: 
 
-Filename: prev_gen-2.0.2.dist-info/METADATA
+Filename: prev_gen-2.0.4.dist-info/METADATA
 Comment: 
 
-Filename: prev_gen-2.0.2.dist-info/WHEEL
+Filename: prev_gen-2.0.4.dist-info/WHEEL
 Comment: 
 
-Filename: prev_gen-2.0.2.dist-info/top_level.txt
+Filename: prev_gen-2.0.4.dist-info/top_level.txt
 Comment: 
 
-Filename: prev_gen-2.0.2.dist-info/RECORD
+Filename: prev_gen-2.0.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## prev_gen/main.py

```diff
@@ -1026,17 +1026,18 @@
             (drawsvg.Drawing) the created image
         """
         t = Table(palette)
         s = t.settings
         draw = svg.Drawing(*t.size, origin=(0, 0), id_prefix='prevgen')
         font_name = s.font_name or 'Nunito'
         font_opts = s.font_opts or {'wght': 700}
-        draw.append_css('text{font-family:' + font_name + ',Calibri,sans-serif;}')
         if 'wght' in font_opts:
-            draw.append_css('text{font-weight:'+str(font_opts['wght'])+';}')
+            draw.append_css('text{font-family:' + font_name + ',Calibri,sans-serif;font-weight:' + str(font_opts['wght']) + ';}')
+        else:
+            draw.append_css('text{font-family:' + font_name + ',Calibri,sans-serif;}')
         # embed google font in svg for correct previews
         try:
             draw.embed_google_font(font_name, **font_opts)
         except urllib.error.HTTPError:
             print(f'\033[31;1mError: \'{font_name}\' with opts \'{font_opts}\' is not available in Google Fonts')
             exit(1)
         for i in t:
```

## Comparing `prev_gen-2.0.2.dist-info/METADATA` & `prev_gen-2.0.4.dist-info/METADATA`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: prev-gen
-Version: 2.0.2
+Version: 2.0.4
 Summary: Create a palette preview image by using a simple config file
 Home-page: https://github.com/Aonodensetsu/prev_gen
 Author: Remigiusz Dończyk
-Author-email: aonodensetsu@aonodensetsu.me
+Author-email: donczyk.remigiusz@gmail.com
 License: GPL-3.0
 Keywords: palette,preview,generator,image
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.10
@@ -19,15 +19,15 @@
 Description-Content-Type: text/markdown
 Requires-Dist: pillow
 Requires-Dist: drawsvg (~=2.0)
 
 ## Create a palette preview image by using a simple config file
 
 ![size](https://img.shields.io/github/repo-size/aonodensetsu/prev_gen?label=size) ![files](https://img.shields.io/github/directory-file-count/aonodensetsu/prev_gen) ![lines](https://img.shields.io/tokei/lines/github/aonodensetsu/prev_gen)   
-![py dep](https://img.shields.io/pypi/pyversions/prev-gen) [![version](https://img.shields.io/pypi/v/prev-gen)](https://pypi.org/project/prev-gen/2.0.2/)  
+![py dep](https://img.shields.io/pypi/pyversions/prev-gen) [![version](https://img.shields.io/pypi/v/prev-gen)](https://pypi.org/project/prev-gen/2.0.4/)  
 ![license](https://img.shields.io/pypi/l/prev-gen) [![downloads](https://img.shields.io/badge/releases-here-green?logo=pypi)](https://pypi.org/project/prev-gen/#history)  
 [![downloads](https://img.shields.io/badge/wiki-here-pink)](https://github.com/Aonodensetsu/prev_gen/blob/main/WIKI.md) [![downloads](https://img.shields.io/badge/changelog-here-pink)](https://github.com/Aonodensetsu/prev_gen/blob/main/CHANGELOG.md)  
 
 # Usage:
 1. `pip install prev_gen`
 2. Open up [the wiki](https://github.com/Aonodensetsu/prev_gen/blob/main/WIKI.md) to see how everything works
 3. Create a file based on instructions (or just edit [the example](https://github.com/Aonodensetsu/prev_gen/blob/main/example.py))
@@ -35,9 +35,9 @@
    # palette = [...]
    from prev_gen import Preview
    Preview(palette)
    ```
 
 # Example:
 Inspired by the great [Gruvbox](https://github.com/morhetz/gruvbox) theme, where even the preview is impressive  
-And so, below is the Gruvbox palette preview recreated with this app  
-[![example](https://raw.githubusercontent.com/Aonodensetsu/prev_gen/main/gruvbox.svg)](https://github.com/Aonodensetsu/prev_gen/blob/main/gruvbox.svg)
+And so, below is the Gruvbox palette preview recreated with this app (click for selectable text)  
+[![example](https://raw.githubusercontent.com/Aonodensetsu/prev_gen/main/gruvbox.svg)](https://raw.githubusercontent.com/Aonodensetsu/prev_gen/main/gruvbox.svg)
```

