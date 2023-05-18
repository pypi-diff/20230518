# Comparing `tmp/cf-view-3.2.23.tar.gz` & `tmp/cf-view-3.2.24.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cf-view-3.2.23.tar", last modified: Thu May 18 10:22:37 2023, max compression
+gzip compressed data, was "cf-view-3.2.24.tar", last modified: Thu May 18 10:48:59 2023, max compression
```

## Comparing `cf-view-3.2.23.tar` & `cf-view-3.2.24.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxr-x   0 andy      (1000) andy      (1000)        0 2023-05-18 10:22:37.830099 cf-view-3.2.23/
--rw-r--r--   0 andy      (1000) andy      (1000)     1065 2021-06-09 09:47:44.000000 cf-view-3.2.23/LICENSE.txt
--rw-rw-r--   0 andy      (1000) andy      (1000)      461 2023-05-18 10:22:37.830099 cf-view-3.2.23/PKG-INFO
--rw-r--r--   0 andy      (1000) andy      (1000)      275 2021-05-19 13:18:16.000000 cf-view-3.2.23/README.txt
-drwxrwxr-x   0 andy      (1000) andy      (1000)        0 2023-05-18 10:22:37.830099 cf-view-3.2.23/cf_view.egg-info/
--rw-rw-r--   0 andy      (1000) andy      (1000)      461 2023-05-18 10:22:37.000000 cf-view-3.2.23/cf_view.egg-info/PKG-INFO
--rw-rw-r--   0 andy      (1000) andy      (1000)      192 2023-05-18 10:22:37.000000 cf-view-3.2.23/cf_view.egg-info/SOURCES.txt
--rw-rw-r--   0 andy      (1000) andy      (1000)        1 2023-05-18 10:22:37.000000 cf-view-3.2.23/cf_view.egg-info/dependency_links.txt
--rw-rw-r--   0 andy      (1000) andy      (1000)       38 2023-05-18 10:22:37.000000 cf-view-3.2.23/cf_view.egg-info/requires.txt
--rw-rw-r--   0 andy      (1000) andy      (1000)        1 2023-05-18 10:22:37.000000 cf-view-3.2.23/cf_view.egg-info/top_level.txt
--rwxr-xr-x   0 andy      (1000) andy      (1000)   366781 2023-05-18 10:21:11.000000 cf-view-3.2.23/cfview
--rw-rw-r--   0 andy      (1000) andy      (1000)       38 2023-05-18 10:22:37.830099 cf-view-3.2.23/setup.cfg
--rw-r--r--   0 andy      (1000) andy      (1000)      805 2023-05-18 10:20:54.000000 cf-view-3.2.23/setup.py
+drwxrwxr-x   0 andy      (1000) andy      (1000)        0 2023-05-18 10:48:59.061812 cf-view-3.2.24/
+-rw-r--r--   0 andy      (1000) andy      (1000)     1065 2021-06-09 09:47:44.000000 cf-view-3.2.24/LICENSE.txt
+-rw-rw-r--   0 andy      (1000) andy      (1000)      461 2023-05-18 10:48:59.061812 cf-view-3.2.24/PKG-INFO
+-rw-r--r--   0 andy      (1000) andy      (1000)      275 2021-05-19 13:18:16.000000 cf-view-3.2.24/README.txt
+drwxrwxr-x   0 andy      (1000) andy      (1000)        0 2023-05-18 10:48:59.057812 cf-view-3.2.24/cf_view.egg-info/
+-rw-rw-r--   0 andy      (1000) andy      (1000)      461 2023-05-18 10:48:58.000000 cf-view-3.2.24/cf_view.egg-info/PKG-INFO
+-rw-rw-r--   0 andy      (1000) andy      (1000)      192 2023-05-18 10:48:59.000000 cf-view-3.2.24/cf_view.egg-info/SOURCES.txt
+-rw-rw-r--   0 andy      (1000) andy      (1000)        1 2023-05-18 10:48:58.000000 cf-view-3.2.24/cf_view.egg-info/dependency_links.txt
+-rw-rw-r--   0 andy      (1000) andy      (1000)       38 2023-05-18 10:48:58.000000 cf-view-3.2.24/cf_view.egg-info/requires.txt
+-rw-rw-r--   0 andy      (1000) andy      (1000)        1 2023-05-18 10:48:58.000000 cf-view-3.2.24/cf_view.egg-info/top_level.txt
+-rwxr-xr-x   0 andy      (1000) andy      (1000)   366687 2023-05-18 10:47:23.000000 cf-view-3.2.24/cfview
+-rw-rw-r--   0 andy      (1000) andy      (1000)       38 2023-05-18 10:48:59.061812 cf-view-3.2.24/setup.cfg
+-rw-r--r--   0 andy      (1000) andy      (1000)      805 2023-05-18 10:47:51.000000 cf-view-3.2.24/setup.py
```

### Comparing `cf-view-3.2.23/LICENSE.txt` & `cf-view-3.2.24/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `cf-view-3.2.23/cfview` & `cf-view-3.2.24/cfview`

 * *Files 0% similar despite different names*

```diff
@@ -1131,15 +1131,14 @@
             for i in np.arange(8):
                 if vars[i] in map_args:
                     map_com += vars[i] + "="
                 if vars[i] in map_args and vars[i] in ['proj', 'resolution']:
                     map_com += "'"
                 if vars[i] in map_args:    
                     map_com += getattr(plotvars, vars[i])
-                    print('keyword and value are ', vars[i], getattr(plotvars, vars[i]))
                 if vars[i] in map_args and vars[i] in ['proj', 'resolution']:
                     map_com += "'"                    
                 if vars[i] in map_args:                    
                     comma_count += 1
                     if comma_count < len(map_args) :
                         map_com += ", "
                         
@@ -2846,25 +2845,25 @@
         if value.text() == 'transform':
             if self.transform_window is None:
                 self.transform_window = Transform_window(self.parent)
             self.transform_window.show()
 
         if value.text() == 'about':
             html = '<body><h2>About cfview</h2>'
-            html += '<b>This is version 3.2.23</b><p>'
+            html += '<b>This is version 3.2.24</b><p>'
             html += 'cfview is a quick look data exploration tool for netCDF, Met Office PP and fields file data'
             html += '<p>'
             html += 'cfview uses:<br>'
             html += '<b>cf-python</b> - data I/O and manipulation<br>'
             html += 'https://ncas-cms.github.io/cf-python<p>'
             html += '<b>cf-plot</b> - plotting<br>'
             html += 'http://ajheaps.github.io/cf-plot<P>'
             html += '<b>PyQt5</b> - GUI toolkit<p>'
             html += 'Author: Andy Heaps andy.heaps@ncas.ac.uk<br>'
-            html += '&#169; NCAS CMS February 2023'
+            html += '&#169; NCAS CMS May 2023'
             self.about_help = Help(html)
             self.about_help.show()
 
         if value.text() == 'cfview':
             html = '<body><h2>Using cfview</h2>'
             html += 'cfview is available for the Unix and Mac platforms<p>'
             html += '<h4>Starting cfview</h4>'
```

### Comparing `cf-view-3.2.23/setup.py` & `cf-view-3.2.24/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(name = "cf-view",
     long_description = "GUI for viewing CF files",
-    version      = "3.2.23",
+    version      = "3.2.24",
     description  = "GUI for viewing CF files",
     author       = "Andy Heaps",
     maintainer   = "Andy Heaps",
     maintainer_email  = "andy.heaps@ncas.ac.uk",
     author_email = "andy.heaps@ncas.ac.uk",
     url          = "http://ajheaps.github.io/cf-view",
     download_url = "https://github.com/ajheaps/CF-View",
```

