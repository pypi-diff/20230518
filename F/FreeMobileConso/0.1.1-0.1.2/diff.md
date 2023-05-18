# Comparing `tmp/FreeMobileConso-0.1.1.tar.gz` & `tmp/FreeMobileConso-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FreeMobileConso-0.1.1.tar", last modified: Tue May 16 17:16:37 2023, max compression
+gzip compressed data, was "FreeMobileConso-0.1.2.tar", last modified: Thu May 18 13:37:58 2023, max compression
```

## Comparing `FreeMobileConso-0.1.1.tar` & `FreeMobileConso-0.1.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 corentin   (501) staff       (20)        0 2023-05-16 17:16:37.510061 FreeMobileConso-0.1.1/
-drwxr-xr-x   0 corentin   (501) staff       (20)        0 2023-05-16 17:16:37.508925 FreeMobileConso-0.1.1/FreeMobileConso/
--rw-r--r--   0 corentin   (501) staff       (20)     1396 2023-05-16 17:15:54.000000 FreeMobileConso-0.1.1/FreeMobileConso/__init__.py
--rw-r--r--   0 corentin   (501) staff       (20)     6173 2023-05-14 12:36:03.000000 FreeMobileConso-0.1.1/FreeMobileConso/client.py
--rw-r--r--   0 corentin   (501) staff       (20)     2033 2023-05-14 12:15:38.000000 FreeMobileConso-0.1.1/FreeMobileConso/dataClassification.py
-drwxr-xr-x   0 corentin   (501) staff       (20)        0 2023-05-16 17:16:37.509780 FreeMobileConso-0.1.1/FreeMobileConso.egg-info/
--rw-r--r--   0 corentin   (501) staff       (20)     6054 2023-05-16 17:16:37.000000 FreeMobileConso-0.1.1/FreeMobileConso.egg-info/PKG-INFO
--rw-r--r--   0 corentin   (501) staff       (20)      312 2023-05-16 17:16:37.000000 FreeMobileConso-0.1.1/FreeMobileConso.egg-info/SOURCES.txt
--rw-r--r--   0 corentin   (501) staff       (20)        1 2023-05-16 17:16:37.000000 FreeMobileConso-0.1.1/FreeMobileConso.egg-info/dependency_links.txt
--rw-r--r--   0 corentin   (501) staff       (20)       13 2023-05-16 17:16:37.000000 FreeMobileConso-0.1.1/FreeMobileConso.egg-info/requires.txt
--rw-r--r--   0 corentin   (501) staff       (20)       16 2023-05-16 17:16:37.000000 FreeMobileConso-0.1.1/FreeMobileConso.egg-info/top_level.txt
--rwxrwxrwx   0 corentin   (501) staff       (20)     1068 2022-08-01 16:04:58.000000 FreeMobileConso-0.1.1/LICENSE
--rw-r--r--   0 corentin   (501) staff       (20)     6054 2023-05-16 17:16:37.509935 FreeMobileConso-0.1.1/PKG-INFO
--rwxrwxrwx   0 corentin   (501) staff       (20)     5569 2023-05-16 17:15:01.000000 FreeMobileConso-0.1.1/README.md
--rw-r--r--   0 corentin   (501) staff       (20)       38 2023-05-16 17:16:37.510096 FreeMobileConso-0.1.1/setup.cfg
--rw-r--r--   0 corentin   (501) staff       (20)      864 2023-05-16 17:15:49.000000 FreeMobileConso-0.1.1/setup.py
+drwxr-xr-x   0 corentin   (501) staff       (20)        0 2023-05-18 13:37:58.484073 FreeMobileConso-0.1.2/
+drwxr-xr-x   0 corentin   (501) staff       (20)        0 2023-05-18 13:37:58.482871 FreeMobileConso-0.1.2/FreeMobileConso/
+-rw-r--r--   0 corentin   (501) staff       (20)     1396 2023-05-18 13:37:26.000000 FreeMobileConso-0.1.2/FreeMobileConso/__init__.py
+-rw-r--r--   0 corentin   (501) staff       (20)     7680 2023-05-18 13:37:05.000000 FreeMobileConso-0.1.2/FreeMobileConso/client.py
+-rw-r--r--   0 corentin   (501) staff       (20)     3617 2023-05-18 13:34:01.000000 FreeMobileConso-0.1.2/FreeMobileConso/dataClassification.py
+drwxr-xr-x   0 corentin   (501) staff       (20)        0 2023-05-18 13:37:58.483721 FreeMobileConso-0.1.2/FreeMobileConso.egg-info/
+-rw-r--r--   0 corentin   (501) staff       (20)     6054 2023-05-18 13:37:58.000000 FreeMobileConso-0.1.2/FreeMobileConso.egg-info/PKG-INFO
+-rw-r--r--   0 corentin   (501) staff       (20)      312 2023-05-18 13:37:58.000000 FreeMobileConso-0.1.2/FreeMobileConso.egg-info/SOURCES.txt
+-rw-r--r--   0 corentin   (501) staff       (20)        1 2023-05-18 13:37:58.000000 FreeMobileConso-0.1.2/FreeMobileConso.egg-info/dependency_links.txt
+-rw-r--r--   0 corentin   (501) staff       (20)       13 2023-05-18 13:37:58.000000 FreeMobileConso-0.1.2/FreeMobileConso.egg-info/requires.txt
+-rw-r--r--   0 corentin   (501) staff       (20)       16 2023-05-18 13:37:58.000000 FreeMobileConso-0.1.2/FreeMobileConso.egg-info/top_level.txt
+-rwxrwxrwx   0 corentin   (501) staff       (20)     1068 2022-08-01 16:04:58.000000 FreeMobileConso-0.1.2/LICENSE
+-rw-r--r--   0 corentin   (501) staff       (20)     6054 2023-05-18 13:37:58.483935 FreeMobileConso-0.1.2/PKG-INFO
+-rwxrwxrwx   0 corentin   (501) staff       (20)     5569 2023-05-16 17:15:01.000000 FreeMobileConso-0.1.2/README.md
+-rw-r--r--   0 corentin   (501) staff       (20)       38 2023-05-18 13:37:58.484120 FreeMobileConso-0.1.2/setup.cfg
+-rw-r--r--   0 corentin   (501) staff       (20)      864 2023-05-18 13:37:31.000000 FreeMobileConso-0.1.2/setup.py
```

### Comparing `FreeMobileConso-0.1.1/FreeMobileConso/__init__.py` & `FreeMobileConso-0.1.2/FreeMobileConso/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,12 +20,12 @@
 """
 
 
 __title__ = "FreeMobileConso"
 __author__ = "CorentinMre"
 __license__ = "MIT"
 __copyright__ = "Copyright (c) CorentinMre"
-__version__ = "0.1.1"
+__version__ = "0.1.2"
 
 
 from .dataClassification import *
 from .client import *
```

### Comparing `FreeMobileConso-0.1.1/FreeMobileConso/client.py` & `FreeMobileConso-0.1.2/FreeMobileConso/client.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,75 +1,101 @@
 
 import requests
 from bs4 import BeautifulSoup
 
 from . import dataClassification
 
 class Client:
+    """
+    Class to get information about your Free Mobile account
+    
+    Parameters
+    ----------
+    identifiant : str
+        Your Free Mobile identifiant
+    password : str
+        Your Free Mobile password
+
+    Functions
+    ---------
+    getConsoDict()
+        Return a dict with all information about your Free Mobile account
+    consomation()
+        Return a object with all information about your Free Mobile account
+        
+    """
     
     def __init__(self, identifiant, password):
+        # Set the identifiant and password
         self.identifiant = identifiant
         self.password = password
-        
+        # Set the payload
         self.payload = {
             "login-ident": self.identifiant,
             "login-pwd": self.password,
             "bt-login": "1"
         }
-        
+        # Set the session
         self.session = requests.Session()
-
+        # Set the headers of the session
         self.session.headers.update({
             "User-Agent": "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36"
         })
-        
+        # Set the url of the login page
         self.urlLogin = "https://mobile.free.fr/account/"
-        
+        # Information to grab
         listOfInternetInforamtion = ["conso", "consoMax", "remaining", "excludingPackage", "carbonFootprint"]
         listOfAppelInforamtion = ["conso", "consoMax", "callToMyCountry", "callToInternational", "excludingPackage"]
         listOfSMSInforamtion = ["conso", "consoMax", "maxNbSMS", "nbSMS", "excludingPackage"]
         listOfMMSInforamtion = ["conso", "consoMax", "maxNbMMS", "nbMMS", "excludingPackage"]
-
+        # Set the dict of all information
         self.dictOfAllInformation = {
             "internet": listOfInternetInforamtion,
             "call": listOfAppelInforamtion,
             "SMS": listOfSMSInforamtion,
             "MMS": listOfMMSInforamtion
         }
                     
     
 
-    def getConsoDict(self) -> dict: 
-        
+    def getConsoDict(self) -> dict:
+        """
+        getConsoDict()
+        ---------------
+        Return a dict with all information about your Free Mobile account
+        """
+        # Send the request
         req = self.session.post(self.urlLogin, data=self.payload)
-        
+        # Get the soup
         soup = BeautifulSoup(req.content, "html.parser")
-        
+        # Get the user information
         userInfo = soup.find("div", {"class": "current-user__infos"})
-
+        # Get the name of the account, try to get the name of the account, if it doesn't work, raise an exception "Identifiant or password is incorrect"
         try:
             nameAcount = userInfo.find("div", {"class": "identite_bis"}).text.strip()
         except:
             raise Exception("Identifiant or password is incorrect")
 
-
+        # Get name, identifiant, ligne and date
         nameAcount = userInfo.find("div", {"class": "identite_bis"}).text.strip()
         identifiant = userInfo.findAll("div", {"class": "smaller"})[0].text.strip()
         ligne = userInfo.findAll("div", {"class": "smaller"})[1].text.strip()
         date = soup.find("div", {"class": "details"}).find("div", {"class": "sub-title"}).text.strip()
         
         
         result= {}
-        
+        # Get the information about the internet, call, SMS and MMS in roaming and local
         for _ in range(2):
             
+            # Get the div where the information is
             place = soup.find("div", {"class": "conso-local"}) if _ == 0 else soup.find("div", {"class": "conso-roaming"})
-        
+            # Prepare the dict
             result[place["class"][1].split("-")[1]] = {}
             
+            # Get the information about the internet, call, SMS and MMS
             for key, value in self.dictOfAllInformation.items():
                 
                 if key == "internet": itteration = 0
                 elif key == "call": itteration = 1
                 elif key == "SMS": itteration = 2
                 elif key == "MMS": itteration = 3
                 
@@ -100,14 +126,15 @@
                 else:
                     result[place["class"][1].split("-")[1]][key][value[3]] = thirdInformation[0].text.strip().split(" / ")[0].replace("*","")
                     result[place["class"][1].split("-")[1]][key][value[4]] = lastSMSMMSInformation
                 
                 if key == "internet" and place["class"][1].split("-")[1] == "local":
                     result[place["class"][1].split("-")[1]][key][value[4]] = lastInternetAppelInformation[2].text.strip().split(": ")[1].replace("*","")
             
+        # Initialize the totalExcludingPackage
         result["totalExcludingPackage"] = 0
         for key, value in result.items():
             if key == "local" or key == "roaming":
                 for key2, value2 in value.items():
                     for key3, value3 in value2.items():
                         if key3 == "excludingPackage":
                             result["totalExcludingPackage"] += float(value3.replace("€", ""))
@@ -116,10 +143,16 @@
         result["nameAcount"] = nameAcount
         result["identifier"] = identifiant.split(" : ")[1]
         result["number"] = ligne.split(" : ")[1].replace(" ", "")
         result["date"] = date
         
         return result
     
-    def consommation(self) -> dict:
+    def consommation(self) -> object:
+        """
+        consommation()
+        --------------
+        Return a object with all information about your Free Mobile account
+        """
+        # Return the object
         return dataClassification.Classification(self.getConsoDict())
```

### Comparing `FreeMobileConso-0.1.1/FreeMobileConso.egg-info/PKG-INFO` & `FreeMobileConso-0.1.2/FreeMobileConso.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FreeMobileConso
-Version: 0.1.1
+Version: 0.1.2
 Summary: A python API for get your consommation of your Free mobile account
 Home-page: https://github.com/CorentinMre/FreeMobileConso
 Author: CorentinMre
 Author-email: corentin.marie@isen-ouest.yncrea.fr
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `FreeMobileConso-0.1.1/LICENSE` & `FreeMobileConso-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `FreeMobileConso-0.1.1/PKG-INFO` & `FreeMobileConso-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FreeMobileConso
-Version: 0.1.1
+Version: 0.1.2
 Summary: A python API for get your consommation of your Free mobile account
 Home-page: https://github.com/CorentinMre/FreeMobileConso
 Author: CorentinMre
 Author-email: corentin.marie@isen-ouest.yncrea.fr
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `FreeMobileConso-0.1.1/README.md` & `FreeMobileConso-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `FreeMobileConso-0.1.1/setup.py` & `FreeMobileConso-0.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='FreeMobileConso',
-    version='0.1.1',    
+    version='0.1.2',    
     description='A python API for get your consommation of your Free mobile account',
     long_description_content_type = "text/markdown",
     long_description=long_description,
     url='https://github.com/CorentinMre/FreeMobileConso',
     author='CorentinMre',
     author_email='corentin.marie@isen-ouest.yncrea.fr',
     license='MIT',
```

