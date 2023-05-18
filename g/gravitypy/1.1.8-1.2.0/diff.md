# Comparing `tmp/gravitypy-1.1.8.tar.gz` & `tmp/gravitypy-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gravitypy-1.1.8.tar", last modified: Thu May 18 20:33:23 2023, max compression
+gzip compressed data, was "gravitypy-1.2.0.tar", last modified: Thu May 18 20:38:37 2023, max compression
```

## Comparing `gravitypy-1.1.8.tar` & `gravitypy-1.2.0.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxr-x   0 wiktor    (1000) wiktor    (1000)        0 2023-05-18 20:33:23.486915 gravitypy-1.1.8/
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)     1066 2023-05-07 20:40:23.000000 gravitypy-1.1.8/LICENSE
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)       25 2023-05-07 20:40:23.000000 gravitypy-1.1.8/MANIFEST.in
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)      292 2023-05-18 20:33:23.482915 gravitypy-1.1.8/PKG-INFO
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)     1332 2023-05-11 15:01:38.000000 gravitypy-1.1.8/README.md
-drwxrwxr-x   0 wiktor    (1000) wiktor    (1000)        0 2023-05-18 20:33:23.482915 gravitypy-1.1.8/gravitypy/
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)        0 2023-05-07 20:40:23.000000 gravitypy-1.1.8/gravitypy/__init__.py
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)       70 2023-05-12 13:14:06.000000 gravitypy-1.1.8/gravitypy/__main__.py
-drwxrwxr-x   0 wiktor    (1000) wiktor    (1000)        0 2023-05-18 20:33:23.482915 gravitypy-1.1.8/gravitypy/button/
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)       27 2023-05-12 13:07:34.000000 gravitypy-1.1.8/gravitypy/button/__init__.py
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)     2384 2023-05-18 20:17:12.000000 gravitypy-1.1.8/gravitypy/button/button.py
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)        0 2023-05-18 19:07:09.000000 gravitypy-1.1.8/gravitypy/config.py
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)    13259 2023-05-18 20:32:30.000000 gravitypy-1.1.8/gravitypy/main.py
-drwxrwxr-x   0 wiktor    (1000) wiktor    (1000)        0 2023-05-18 20:33:23.482915 gravitypy-1.1.8/gravitypy/particle/
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)       31 2023-05-12 13:07:49.000000 gravitypy-1.1.8/gravitypy/particle/__init__.py
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)     5394 2023-05-18 20:27:42.000000 gravitypy-1.1.8/gravitypy/particle/particle.py
-drwxrwxr-x   0 wiktor    (1000) wiktor    (1000)        0 2023-05-18 20:33:23.482915 gravitypy-1.1.8/gravitypy/resources/
-drwxrwxr-x   0 wiktor    (1000) wiktor    (1000)        0 2023-05-18 20:33:23.482915 gravitypy-1.1.8/gravitypy/resources/fonts/
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)    15700 2023-05-07 20:40:23.000000 gravitypy-1.1.8/gravitypy/resources/fonts/minecraft_font.ttf
-drwxrwxr-x   0 wiktor    (1000) wiktor    (1000)        0 2023-05-18 20:33:23.482915 gravitypy-1.1.8/gravitypy.egg-info/
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)      292 2023-05-18 20:33:23.000000 gravitypy-1.1.8/gravitypy.egg-info/PKG-INFO
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)      500 2023-05-18 20:33:23.000000 gravitypy-1.1.8/gravitypy.egg-info/SOURCES.txt
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)        1 2023-05-18 20:33:23.000000 gravitypy-1.1.8/gravitypy.egg-info/dependency_links.txt
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)       54 2023-05-18 20:33:23.000000 gravitypy-1.1.8/gravitypy.egg-info/entry_points.txt
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)       14 2023-05-18 20:33:23.000000 gravitypy-1.1.8/gravitypy.egg-info/requires.txt
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)       10 2023-05-18 20:33:23.000000 gravitypy-1.1.8/gravitypy.egg-info/top_level.txt
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)       14 2023-05-07 20:40:23.000000 gravitypy-1.1.8/requirements.txt
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)       38 2023-05-18 20:33:23.486915 gravitypy-1.1.8/setup.cfg
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)      959 2023-05-18 20:21:53.000000 gravitypy-1.1.8/setup.py
+drwxrwxr-x   0 wiktor    (1000) wiktor    (1000)        0 2023-05-18 20:38:37.762516 gravitypy-1.2.0/
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)     1066 2023-05-07 20:40:23.000000 gravitypy-1.2.0/LICENSE
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)       25 2023-05-07 20:40:23.000000 gravitypy-1.2.0/MANIFEST.in
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)      292 2023-05-18 20:38:37.762516 gravitypy-1.2.0/PKG-INFO
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)     1332 2023-05-11 15:01:38.000000 gravitypy-1.2.0/README.md
+drwxrwxr-x   0 wiktor    (1000) wiktor    (1000)        0 2023-05-18 20:38:37.762516 gravitypy-1.2.0/gravitypy/
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)        0 2023-05-07 20:40:23.000000 gravitypy-1.2.0/gravitypy/__init__.py
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)       70 2023-05-12 13:14:06.000000 gravitypy-1.2.0/gravitypy/__main__.py
+drwxrwxr-x   0 wiktor    (1000) wiktor    (1000)        0 2023-05-18 20:38:37.762516 gravitypy-1.2.0/gravitypy/button/
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)       27 2023-05-12 13:07:34.000000 gravitypy-1.2.0/gravitypy/button/__init__.py
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)     2384 2023-05-18 20:17:12.000000 gravitypy-1.2.0/gravitypy/button/button.py
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)        0 2023-05-18 19:07:09.000000 gravitypy-1.2.0/gravitypy/config.py
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)    13252 2023-05-18 20:38:04.000000 gravitypy-1.2.0/gravitypy/main.py
+drwxrwxr-x   0 wiktor    (1000) wiktor    (1000)        0 2023-05-18 20:38:37.762516 gravitypy-1.2.0/gravitypy/particle/
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)       31 2023-05-12 13:07:49.000000 gravitypy-1.2.0/gravitypy/particle/__init__.py
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)     5394 2023-05-18 20:27:42.000000 gravitypy-1.2.0/gravitypy/particle/particle.py
+drwxrwxr-x   0 wiktor    (1000) wiktor    (1000)        0 2023-05-18 20:38:37.762516 gravitypy-1.2.0/gravitypy/resources/
+drwxrwxr-x   0 wiktor    (1000) wiktor    (1000)        0 2023-05-18 20:38:37.762516 gravitypy-1.2.0/gravitypy/resources/fonts/
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)    15700 2023-05-07 20:40:23.000000 gravitypy-1.2.0/gravitypy/resources/fonts/minecraft_font.ttf
+drwxrwxr-x   0 wiktor    (1000) wiktor    (1000)        0 2023-05-18 20:38:37.762516 gravitypy-1.2.0/gravitypy.egg-info/
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)      292 2023-05-18 20:38:37.000000 gravitypy-1.2.0/gravitypy.egg-info/PKG-INFO
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)      500 2023-05-18 20:38:37.000000 gravitypy-1.2.0/gravitypy.egg-info/SOURCES.txt
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)        1 2023-05-18 20:38:37.000000 gravitypy-1.2.0/gravitypy.egg-info/dependency_links.txt
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)       54 2023-05-18 20:38:37.000000 gravitypy-1.2.0/gravitypy.egg-info/entry_points.txt
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)       14 2023-05-18 20:38:37.000000 gravitypy-1.2.0/gravitypy.egg-info/requires.txt
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)       10 2023-05-18 20:38:37.000000 gravitypy-1.2.0/gravitypy.egg-info/top_level.txt
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)       14 2023-05-07 20:40:23.000000 gravitypy-1.2.0/requirements.txt
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)       38 2023-05-18 20:38:37.762516 gravitypy-1.2.0/setup.cfg
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)      959 2023-05-18 20:37:25.000000 gravitypy-1.2.0/setup.py
```

### Comparing `gravitypy-1.1.8/LICENSE` & `gravitypy-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `gravitypy-1.1.8/README.md` & `gravitypy-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `gravitypy-1.1.8/gravitypy/button/button.py` & `gravitypy-1.2.0/gravitypy/button/button.py`

 * *Files identical despite different names*

### Comparing `gravitypy-1.1.8/gravitypy/main.py` & `gravitypy-1.2.0/gravitypy/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -281,8 +281,7 @@
             SCREEN.blit(data['text'], data['position'])
     
 
         pygame.display.update()
         CLOCK.tick(60)
     
     pygame.quit()
-main()
```

### Comparing `gravitypy-1.1.8/gravitypy/particle/particle.py` & `gravitypy-1.2.0/gravitypy/particle/particle.py`

 * *Files identical despite different names*

### Comparing `gravitypy-1.1.8/gravitypy/resources/fonts/minecraft_font.ttf` & `gravitypy-1.2.0/gravitypy/resources/fonts/minecraft_font.ttf`

 * *Files identical despite different names*

### Comparing `gravitypy-1.1.8/setup.py` & `gravitypy-1.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 req_file = os.path.join(here, 'requirements.txt')
 with open(req_file, 'r') as f:
     REQUIREMENTS = [line.strip() for line in f.readlines()]
 LONG_DESCRIPTION = 'Pygame N-Body gravity simulation app'
 
 setup(
    name='gravitypy',
-   version='1.1.8',
+   version='1.2.0',
    description='GravityPy',
    license="MIT",
    author='WiktorK02',
    author_email='wiktor.kidon@hotmail.com',
    url="https://github.com/WiktorK02/gravityPy",
    long_description_content_type="text/markdown",
    package_data={'gravitypy': ['*']},
```

