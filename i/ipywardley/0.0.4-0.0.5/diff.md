# Comparing `tmp/ipywardley-0.0.4.tar.gz` & `tmp/ipywardley-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ipywardley-0.0.4.tar", last modified: Thu Jul 22 18:29:02 2021, max compression
+gzip compressed data, was "ipywardley-0.0.5.tar", last modified: Thu May 18 15:05:26 2023, max compression
```

## Comparing `ipywardley-0.0.4.tar` & `ipywardley-0.0.5.tar`

### file list

```diff
@@ -1,11 +1,10 @@
--rw-r--r--   0        0        0     1799 2021-07-22 18:15:06.109716 ipywardley-0.0.4/.gitignore
--rw-r--r--   0        0        0    35149 2021-07-22 18:15:06.110589 ipywardley-0.0.4/LICENSE
--rw-r--r--   0        0        0     2738 2021-07-22 18:22:51.111644 ipywardley-0.0.4/README.md
--rw-r--r--   0        0        0   241725 2021-07-22 18:15:06.114333 ipywardley-0.0.4/doc/example.png
--rw-r--r--   0        0        0      194 2021-07-22 18:28:40.149578 ipywardley-0.0.4/ipywardley/__init__.py
--rw-r--r--   0        0        0     9876 2021-07-22 18:22:06.539543 ipywardley-0.0.4/ipywardley/wardley.py
--rw-r--r--   0        0        0      466 2021-07-22 18:27:20.870919 ipywardley-0.0.4/pyproject.toml
--rw-r--r--   0        0        0  1313519 2021-07-22 18:26:30.753583 ipywardley-0.0.4/test/wardley-maps.ipynb
--rw-r--r--   0        0        0      772 2021-07-22 18:15:06.124882 ipywardley-0.0.4/test/wardley-test.owm
--rw-r--r--   0        0        0      663 1970-01-01 00:00:00.000000 ipywardley-0.0.4/setup.py
--rw-r--r--   0        0        0      221 1970-01-01 00:00:00.000000 ipywardley-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0     1810 2023-05-18 15:04:58.849881 ipywardley-0.0.5/.gitignore
+-rw-r--r--   0        0        0    35149 2023-04-11 11:12:17.266035 ipywardley-0.0.5/LICENSE
+-rw-r--r--   0        0        0     2738 2023-04-11 11:12:17.266191 ipywardley-0.0.5/README.md
+-rw-r--r--   0        0        0   241725 2023-04-11 11:12:17.268171 ipywardley-0.0.5/doc/example.png
+-rw-r--r--   0        0        0      194 2023-05-18 15:04:15.582056 ipywardley-0.0.5/ipywardley/__init__.py
+-rw-r--r--   0        0        0     9917 2023-05-18 15:01:40.028249 ipywardley-0.0.5/ipywardley/wardley.py
+-rw-r--r--   0        0        0      466 2023-05-18 15:02:47.122315 ipywardley-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0  1313519 2023-04-11 11:12:17.274398 ipywardley-0.0.5/test/wardley-maps.ipynb
+-rw-r--r--   0        0        0      772 2023-04-11 11:12:17.274563 ipywardley-0.0.5/test/wardley-test.owm
+-rw-r--r--   0        0        0     3178 1970-01-01 00:00:00.000000 ipywardley-0.0.5/PKG-INFO
```

### Comparing `ipywardley-0.0.4/.gitignore` & `ipywardley-0.0.5/.gitignore`

 * *Files 4% similar despite different names*

```diff
@@ -123,7 +123,11 @@
 # mypy
 .mypy_cache/
 .dmypy.json
 dmypy.json
 
 # Pyre type checker
 .pyre/
+
+# vim
+*~
+
```

### Comparing `ipywardley-0.0.4/LICENSE` & `ipywardley-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `ipywardley-0.0.4/README.md` & `ipywardley-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `ipywardley-0.0.4/doc/example.png` & `ipywardley-0.0.5/doc/example.png`

 * *Files identical despite different names*

### Comparing `ipywardley-0.0.4/ipywardley/wardley.py` & `ipywardley-0.0.5/ipywardley/wardley.py`

 * *Files 1% similar despite different names*

```diff
@@ -227,15 +227,15 @@
 
         plt.yticks([0.0,0.925], ['Invisible', 'Visible'], rotation=90, verticalalignment='bottom')
         plt.ylabel('Visibility', fontweight='bold')
         plt.xticks([0.0, 0.25,0.5, 0.75], ['Genesis', 'Custom-Built', 'Product\n(+rental)', 'Commodity\n(+utility)'], ha='left')
         plt.xlabel('Evolution', fontweight='bold')
 
         plt.tick_params(axis='x', direction='in', top=True, bottom=True, grid_linewidth=1)
-        plt.grid(b=True, axis='x', linestyle='--')
+        plt.grid(visibilty=True, axis='x', linestyle='--') # Updated as 'b' now depreciated
         plt.tick_params(axis='y', length=0)
 
         # Show warnings if problems were found:
         for message in wm.warnings:
             self.show_warning(message)
         if len(wm.evolutions) > 0:
             self.show_warning("Displaying evolutions is not implemented yet!")
```

### Comparing `ipywardley-0.0.4/test/wardley-maps.ipynb` & `ipywardley-0.0.5/test/wardley-maps.ipynb`

 * *Files identical despite different names*

### Comparing `ipywardley-0.0.4/test/wardley-test.owm` & `ipywardley-0.0.5/test/wardley-test.owm`

 * *Files identical despite different names*

