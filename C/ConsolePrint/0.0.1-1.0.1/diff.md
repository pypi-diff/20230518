# Comparing `tmp/consoleprint-0.0.1.tar.gz` & `tmp/consoleprint-1.0.1.tar.gz`

## Comparing `consoleprint-0.0.1.tar` & `consoleprint-1.0.1.tar`

### file list

```diff
@@ -1,9 +1,10 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 consoleprint-0.0.1/src/ConsolePrint/__init__.py
--rw-r--r--   0        0        0      989 2020-02-02 00:00:00.000000 consoleprint-0.0.1/src/ConsolePrint/console2file.py
--rw-r--r--   0        0        0     1490 2020-02-02 00:00:00.000000 consoleprint-0.0.1/src/ConsolePrint/loading.py
--rw-r--r--   0        0        0     3027 2020-02-02 00:00:00.000000 consoleprint-0.0.1/src/ConsolePrint/printing.py
--rw-r--r--   0        0        0      578 2020-02-02 00:00:00.000000 consoleprint-0.0.1/tests/tests.py
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 consoleprint-0.0.1/LICENSE
--rw-r--r--   0        0        0      642 2020-02-02 00:00:00.000000 consoleprint-0.0.1/README.md
--rw-r--r--   0        0        0      620 2020-02-02 00:00:00.000000 consoleprint-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     1172 2020-02-02 00:00:00.000000 consoleprint-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 consoleprint-1.0.1/src/ConsolePrint/__init__.py
+-rw-r--r--   0        0        0     4990 2020-02-02 00:00:00.000000 consoleprint-1.0.1/src/ConsolePrint/animate.py
+-rw-r--r--   0        0        0     1163 2020-02-02 00:00:00.000000 consoleprint-1.0.1/src/ConsolePrint/console2file.py
+-rw-r--r--   0        0        0     1512 2020-02-02 00:00:00.000000 consoleprint-1.0.1/src/ConsolePrint/loading.py
+-rw-r--r--   0        0        0     1123 2020-02-02 00:00:00.000000 consoleprint-1.0.1/tests/tests.py
+-rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 consoleprint-1.0.1/.gitignore
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 consoleprint-1.0.1/LICENSE
+-rw-r--r--   0        0        0     2052 2020-02-02 00:00:00.000000 consoleprint-1.0.1/README.md
+-rw-r--r--   0        0        0      620 2020-02-02 00:00:00.000000 consoleprint-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     2591 2020-02-02 00:00:00.000000 consoleprint-1.0.1/PKG-INFO
```

### Comparing `consoleprint-0.0.1/src/ConsolePrint/loading.py` & `consoleprint-1.0.1/src/ConsolePrint/loading.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,54 +1,56 @@
 import time
 
-def countdown(t):
+def countdown(t, confirm=True):
     '''Enter countdown time in seconds'''
     # t = int(input('Enter time in secs: '))
     while t:
         mins, secs = divmod(t, 60)
         timer = '{:02d}:{:02d}'.format(mins, secs)
         print(timer, end="\r")        
         time.sleep(1)
         t -= 1
-    if __name__ == '__main__':
+    if confirm:
         print('Timer completed!')
 
-def loading1(t):
+def loading1(t, confirm=True):
     x = t
     percent = 0
     for _ in range(t):        
         percent += 100 / x
         y = round(percent, 1) / 100
         print(f" Loading... [{'|||' * _}{'   ' * (x - _ - 1)}]", '{:4.0%}'.format(y), end="\r")
         time.sleep(0.2)
-        t -= 1
-    time.sleep(0.5)
-    if __name__ == '__main__':
-        print('\nLoading Complete!')
+        t -= 1    
+    if confirm:
+        print('\n Loading complete!')
 
-def loading2(t, text='Loading...'):
+def loading2(t, text='Loading...', confirm=False):
     "Takes two arguments, time and text to display such as 'loading...'"
     load = ['-', '\\', '|', '/', ] * t
     for _ in load:
         print(f"  {_}  {text}", end='\r')
         time.sleep(0.5)
-    if __name__ == '__main__':
-        print('\nLoading Complete!')
+    if confirm:
+        print('\nLoading complete!   ')
     
 def loading3(t):
     the_bar = "     ======     "
     nums = ([*range(len(the_bar)-5)] + [*range(len(the_bar) - 7, 0, -1)]) * t
     for a in nums:
         print(f' [{the_bar[a:a + 6]}]', end='\r')
         time.sleep(0.2) 
     if __name__ == '__main__':
         print('\nLoading Complete!')
 
 
 if __name__ == '__main__':
     countdown(5)
+    print()
     loading1(20)  
-    loading2(10, 'thinking...')
-    loading3(10)
+    print()
+    loading2(5, 'thinking...')
+    print()
+    loading3(5)
```

### Comparing `consoleprint-0.0.1/LICENSE` & `consoleprint-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `consoleprint-0.0.1/pyproject.toml` & `consoleprint-1.0.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "ConsolePrint"
-version = "0.0.1"
+version = "1.0.1"
 authors = [
   { name="Udemezue Iloabachie", email="udemezue@gmail.com" },
 ]
 description = "A package to animate print output to console"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

