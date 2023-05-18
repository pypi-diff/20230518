# Comparing `tmp/ipv64-0.5.0.tar.gz` & `tmp/ipv64-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ipv64-0.5.0.tar", last modified: Mon May 15 17:44:24 2023, max compression
+gzip compressed data, was "ipv64-0.5.1.tar", last modified: Thu May 18 10:24:21 2023, max compression
```

## Comparing `ipv64-0.5.0.tar` & `ipv64-0.5.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-05-15 17:44:24.966660 ipv64-0.5.0/
--rw-rw-rw-   0        0        0     1084 2023-05-14 15:54:56.000000 ipv64-0.5.0/LICENSE
--rw-rw-rw-   0        0        0     1861 2023-05-15 17:44:24.966660 ipv64-0.5.0/PKG-INFO
--rw-rw-rw-   0        0        0     1525 2023-05-15 17:38:02.000000 ipv64-0.5.0/README.md
--rw-rw-rw-   0        0        0      111 2023-05-15 17:44:24.967691 ipv64-0.5.0/setup.cfg
--rw-rw-rw-   0        0        0      713 2023-05-15 17:44:21.000000 ipv64-0.5.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-15 17:44:24.960067 ipv64-0.5.0/src/
-drwxrwxrwx   0        0        0        0 2023-05-15 17:44:24.965660 ipv64-0.5.0/src/ipv64.egg-info/
--rw-rw-rw-   0        0        0     1861 2023-05-15 17:44:24.000000 ipv64-0.5.0/src/ipv64.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      213 2023-05-15 17:44:24.000000 ipv64-0.5.0/src/ipv64.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-15 17:44:24.000000 ipv64-0.5.0/src/ipv64.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       33 2023-05-15 17:44:24.000000 ipv64-0.5.0/src/ipv64.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-05-15 17:44:24.000000 ipv64-0.5.0/src/ipv64.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     6185 2023-05-15 17:40:44.000000 ipv64-0.5.0/src/ipv64.py
+drwxrwxrwx   0        0        0        0 2023-05-18 10:24:21.434577 ipv64-0.5.1/
+-rw-rw-rw-   0        0        0     1084 2023-05-14 15:54:56.000000 ipv64-0.5.1/LICENSE
+-rw-rw-rw-   0        0        0     1802 2023-05-18 10:24:21.434577 ipv64-0.5.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1525 2023-05-15 17:38:02.000000 ipv64-0.5.1/README.md
+-rw-rw-rw-   0        0        0      111 2023-05-18 10:24:21.436554 ipv64-0.5.1/setup.cfg
+-rw-rw-rw-   0        0        0      654 2023-05-18 10:23:34.000000 ipv64-0.5.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-18 10:24:21.403076 ipv64-0.5.1/src/
+drwxrwxrwx   0        0        0        0 2023-05-18 10:24:21.434577 ipv64-0.5.1/src/ipv64.egg-info/
+-rw-rw-rw-   0        0        0     1802 2023-05-18 10:24:21.000000 ipv64-0.5.1/src/ipv64.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      213 2023-05-18 10:24:21.000000 ipv64-0.5.1/src/ipv64.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-18 10:24:21.000000 ipv64-0.5.1/src/ipv64.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       33 2023-05-18 10:24:21.000000 ipv64-0.5.1/src/ipv64.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-05-18 10:24:21.000000 ipv64-0.5.1/src/ipv64.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     7054 2023-05-18 10:23:18.000000 ipv64-0.5.1/src/ipv64.py
```

### Comparing `ipv64-0.5.0/LICENSE` & `ipv64-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ipv64-0.5.0/PKG-INFO` & `ipv64-0.5.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: ipv64
-Version: 0.5.0
-Summary: Updater for ipv64.net - ATTENTION THIS VERSION IS NOT COMPATIBLE WITH THE 0.4.2!
+Version: 0.5.1
+Summary: Updater for ipv64.net
 Home-page: https://github.com/syncip/ipv64
 Author: R60
 Author-email: pypi.nmvk0@getrekt.win
 Keywords: ipv64,dyndns,updater
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `ipv64-0.5.0/README.md` & `ipv64-0.5.1/README.md`

 * *Files identical despite different names*

### Comparing `ipv64-0.5.0/setup.py` & `ipv64-0.5.1/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 from pathlib import Path
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
   name = 'ipv64',
-  version = '0.5.0',
-  description = 'Updater for ipv64.net - ATTENTION THIS VERSION IS NOT COMPATIBLE WITH THE 0.4.2!',
+  version = '0.5.1',
+  description = 'Updater for ipv64.net',
   author = 'R60',
   author_email = 'pypi.nmvk0@getrekt.win',
   url = 'https://github.com/syncip/ipv64',
   py_modules=["ipv64"],
   package_dir={'': 'src'},
   keywords = ['ipv64', 'dyndns', 'updater'],
   long_description=long_description,
```

### Comparing `ipv64-0.5.0/src/ipv64.egg-info/PKG-INFO` & `ipv64-0.5.1/src/ipv64.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: ipv64
-Version: 0.5.0
-Summary: Updater for ipv64.net - ATTENTION THIS VERSION IS NOT COMPATIBLE WITH THE 0.4.2!
+Version: 0.5.1
+Summary: Updater for ipv64.net
 Home-page: https://github.com/syncip/ipv64
 Author: R60
 Author-email: pypi.nmvk0@getrekt.win
 Keywords: ipv64,dyndns,updater
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `ipv64-0.5.0/src/ipv64.py` & `ipv64-0.5.1/src/ipv64.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,32 +1,33 @@
 import requests
 from datetime import datetime as dt
 import socket
 import logging
 import json
 import time
 import argparse
+import message
 
 # =========================================
 # version
 # =========================================
-version = "0.5.0"
+version = "0.5.1"
 
+# =========================================
 # request User-Agent
+# =========================================
 global headers, timeout
 headers = {
     'User-Agent': 'ipv64-updater/' + str(version),
 }
-timeout = 10
-
 
-# logging
-#loglevel = logging.DEBUG
-loglevel = logging.INFO
-logging.basicConfig(filename='ipv64.log', encoding='utf-8', level=loglevel, format='%(asctime)s: %(message)s')
+# =========================================
+# settings
+# =========================================
+timeout = 10
 
 # =========================================
 # get the current IP of the host
 # =========================================
 def get_ip(type):
     ipv4, ipv6 = False, False
     
@@ -38,28 +39,28 @@
     if type == "A":
         for website in websites4:
             try:
                 request4 = requests.get(website, headers=headers, timeout=timeout)
                 # if website statuscode = 200 (ok) then break the loop and take the given ip
                 if request4.status_code == 200:
                     ip = request4.text.replace(" ", "").replace("\n", "")
-                    logging.info(f"IPv4 from {website}: {ip}")
+                    logging.debug(f"IPv4 from {website}: {ip}")
                     break
             except:
                 ip = False
 
     # Get the current IPv6
     elif type == "AAAA":
         for website in websites6:
             try:
                 request6 = requests.get(website, headers=headers, timeout=timeout)
                 # if website statuscode = 200 (ok) then break the loop and take the given ip
                 if request6.status_code == 200:
                     ip = request6.text.replace(" ", "").replace("\n", "")
-                    logging.info(f"IPv6 from {website}: {ip}")
+                    logging.debug(f"IPv6 from {website}: {ip}")
                     break
             except:
                 ip = False
     else:
         logging.warning("error while machine ip lookup: exit")
         exit()
 
@@ -106,31 +107,35 @@
                     ip = False
             except:
                 ip = False
                 logging.warning(f"nslookup type {type}: error while nslookup exit")
                 exit()
             
             if ip != False:
-                logging.info(f"nslookup type {type}: {domain}: {ip}")
+                logging.debug(f"nslookup type {type}: {domain}: {ip}")
 
     return ip
 
 # =========================================
 # UPDATER
 # =========================================
 def update_ipv64(machine_ip, domain_ip, domain, apikey, type):
 
     # check if machine has a valid ip for the dns type
     if machine_ip == False:
         logging.warning(f"updater: machine has no ip: please choose other DNS type")
+        status = False
+        return status
         exit()
 
     # check if the right key is given
     if len(apikey) > 24:
         logging.warning(f"updater: wrong key, use the account update token")
+        status = False
+        return status
         exit()
 
     # check if type is A or AAAA
     if type == "A":
         ipv64_updater = f"https://ipv64.net/update.php?key={apikey}&domain={domain}&ip={machine_ip}"
     elif type == "AAAA":
         ipv64_updater = f"https://ipv64.net/update.php?key={apikey}&domain={domain}&ip6={machine_ip}"
@@ -145,44 +150,62 @@
 
         if status != 200:
             logging.warning(f"updater: statuscode error {status}")
             status = False
             exit()
 
         if status == 200:
-            logging.warning(f"updater: {status} update successfull")
+            logging.info(f"updater: {status} update successfull")
             status = True
 
+    return status
 
 # =========================================
 # ARGPARSE
 # =========================================
 
 # if no inputs are given, show help
 parser = argparse.ArgumentParser(description='Update the IP for a domain on ipv64.net')
 # ipv64 Arguments
 parser.add_argument('-d', '--domain', help='The domain to update', required=True)
 parser.add_argument('-k', '--key', help='Your ipv64 Account Update Token', required=True)
 parser.add_argument('-t', '--type', help='The Update Type [A|AAAA]', default="", required=True)
+parser.add_argument('--loglevel', help='Set the loglevel [DEBUG|INFO|WARNING|ERROR|CRITICAL]', default="CRITICAL", required=False)
+parser.add_argument('--discord', help='Your Discord Webhook for Update Messages', default=None, required=False)
+parser.add_argument('--ntfy', help='Your ntfy URL for Update Messages', default=None, required=False)
+
 
 args = parser.parse_args()
 
 
 # =========================================
 # SETTINGS
 # =========================================
 APIKEY = args.key
 DOMAINNAME = args.domain
-DNSTYPE = args.type
+DNSTYPE = args.type.upper()
+LOGLEVEL = args.loglevel.upper()
+DISCORD = args.discord
+NTFY = args.ntfy
+
+
+# =========================================
+# loglevel
+# =========================================
+if LOGLEVEL == None:
+    LOGLEVEL = "CRITICAL"
+
+logging.basicConfig(filename='ipv64.log', encoding='utf-8', level=LOGLEVEL, format='%(asctime)s: %(message)s')
 
 # =========================================
 # MAIN PART
 # =========================================
 
 # current machine ip
 machine_ip = get_ip(DNSTYPE)
 
 # current domain ip
 domain_ip = get_domain_details(DOMAINNAME, DNSTYPE)
 
 # update
-update = update_ipv64(machine_ip, domain_ip, DOMAINNAME, APIKEY, DNSTYPE)
+status = update = update_ipv64(machine_ip, domain_ip, DOMAINNAME, APIKEY, DNSTYPE)
+print(status)
```

