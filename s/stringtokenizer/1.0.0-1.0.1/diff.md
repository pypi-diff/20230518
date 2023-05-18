# Comparing `tmp/stringtokenizer-1.0.0.tar.gz` & `tmp/stringtokenizer-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stringtokenizer-1.0.0.tar", last modified: Wed May 17 18:46:02 2023, max compression
+gzip compressed data, was "stringtokenizer-1.0.1.tar", last modified: Thu May 18 08:50:53 2023, max compression
```

## Comparing `stringtokenizer-1.0.0.tar` & `stringtokenizer-1.0.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0 tanmay    (1000) tanmay    (1000)        0 2023-05-17 18:46:02.403893 stringtokenizer-1.0.0/
--rwxrwxrwx   0 tanmay    (1000) tanmay    (1000)      222 2023-05-17 18:46:02.402791 stringtokenizer-1.0.0/PKG-INFO
--rwxrwxrwx   0 tanmay    (1000) tanmay    (1000)       38 2023-05-17 18:46:02.404087 stringtokenizer-1.0.0/setup.cfg
--rwxrwxrwx   0 tanmay    (1000) tanmay    (1000)      233 2023-05-17 18:45:18.000000 stringtokenizer-1.0.0/setup.py
-drwxrwxrwx   0 tanmay    (1000) tanmay    (1000)        0 2023-05-17 18:46:02.390602 stringtokenizer-1.0.0/stringtokenizer/
--rwxrwxrwx   0 tanmay    (1000) tanmay    (1000)       46 2023-05-17 18:44:19.000000 stringtokenizer-1.0.0/stringtokenizer/__init__.py
--rwxrwxrwx   0 tanmay    (1000) tanmay    (1000)     1460 2023-05-17 15:04:39.000000 stringtokenizer-1.0.0/stringtokenizer/stringtokenizer.py
-drwxrwxrwx   0 tanmay    (1000) tanmay    (1000)        0 2023-05-17 18:46:02.400151 stringtokenizer-1.0.0/stringtokenizer.egg-info/
--rwxrwxrwx   0 tanmay    (1000) tanmay    (1000)      222 2023-05-17 18:46:02.000000 stringtokenizer-1.0.0/stringtokenizer.egg-info/PKG-INFO
--rwxrwxrwx   0 tanmay    (1000) tanmay    (1000)      227 2023-05-17 18:46:02.000000 stringtokenizer-1.0.0/stringtokenizer.egg-info/SOURCES.txt
--rwxrwxrwx   0 tanmay    (1000) tanmay    (1000)        1 2023-05-17 18:46:02.000000 stringtokenizer-1.0.0/stringtokenizer.egg-info/dependency_links.txt
--rwxrwxrwx   0 tanmay    (1000) tanmay    (1000)       16 2023-05-17 18:46:02.000000 stringtokenizer-1.0.0/stringtokenizer.egg-info/top_level.txt
+drwxrwxrwx   0 tanmay    (1000) tanmay    (1000)        0 2023-05-18 08:50:53.282170 stringtokenizer-1.0.1/
+-rwxrwxrwx   0 tanmay    (1000) tanmay    (1000)      222 2023-05-18 08:50:53.281880 stringtokenizer-1.0.1/PKG-INFO
+-rwxrwxrwx   0 tanmay    (1000) tanmay    (1000)       38 2023-05-18 08:50:53.282266 stringtokenizer-1.0.1/setup.cfg
+-rwxrwxrwx   0 tanmay    (1000) tanmay    (1000)      233 2023-05-18 08:50:42.000000 stringtokenizer-1.0.1/setup.py
+drwxrwxrwx   0 tanmay    (1000) tanmay    (1000)        0 2023-05-18 08:50:53.279195 stringtokenizer-1.0.1/stringtokenizer/
+-rwxrwxrwx   0 tanmay    (1000) tanmay    (1000)       46 2023-05-17 18:44:19.000000 stringtokenizer-1.0.1/stringtokenizer/__init__.py
+-rwxrwxrwx   0 tanmay    (1000) tanmay    (1000)     1463 2023-05-18 08:46:38.000000 stringtokenizer-1.0.1/stringtokenizer/stringtokenizer.py
+drwxrwxrwx   0 tanmay    (1000) tanmay    (1000)        0 2023-05-18 08:50:53.281293 stringtokenizer-1.0.1/stringtokenizer.egg-info/
+-rwxrwxrwx   0 tanmay    (1000) tanmay    (1000)      222 2023-05-18 08:50:53.000000 stringtokenizer-1.0.1/stringtokenizer.egg-info/PKG-INFO
+-rwxrwxrwx   0 tanmay    (1000) tanmay    (1000)      227 2023-05-18 08:50:53.000000 stringtokenizer-1.0.1/stringtokenizer.egg-info/SOURCES.txt
+-rwxrwxrwx   0 tanmay    (1000) tanmay    (1000)        1 2023-05-18 08:50:53.000000 stringtokenizer-1.0.1/stringtokenizer.egg-info/dependency_links.txt
+-rwxrwxrwx   0 tanmay    (1000) tanmay    (1000)       16 2023-05-18 08:50:53.000000 stringtokenizer-1.0.1/stringtokenizer.egg-info/top_level.txt
```

### Comparing `stringtokenizer-1.0.0/stringtokenizer/stringtokenizer.py` & `stringtokenizer-1.0.1/stringtokenizer/stringtokenizer.py`

 * *Files 0% similar despite different names*

```diff
@@ -34,13 +34,13 @@
     def hasMoreTokens(self):
         return len(self.__tokens)>0
     def countTokens(self):
         c=0
         temp=list(self.__tokens)
         try:
             while self.hasMoreTokens():
-                s.nextToken()
+                self.nextToken()
                 c+=1
         except Exception:
             pass
         self.__tokens=temp
         return c
```

