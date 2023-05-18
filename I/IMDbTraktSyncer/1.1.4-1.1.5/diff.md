# Comparing `tmp/IMDbTraktSyncer-1.1.4.tar.gz` & `tmp/IMDbTraktSyncer-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "IMDbTraktSyncer-1.1.4.tar", last modified: Tue May 16 01:36:43 2023, max compression
+gzip compressed data, was "IMDbTraktSyncer-1.1.5.tar", last modified: Thu May 18 02:42:15 2023, max compression
```

## Comparing `IMDbTraktSyncer-1.1.4.tar` & `IMDbTraktSyncer-1.1.5.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-05-16 01:36:43.516004 IMDbTraktSyncer-1.1.4/
-drwxrwxrwx   0        0        0        0 2023-05-16 01:36:43.483057 IMDbTraktSyncer-1.1.4/IMDbTraktSyncer/
--rw-rw-rw-   0        0        0    10838 2023-05-16 01:11:24.000000 IMDbTraktSyncer-1.1.4/IMDbTraktSyncer/IMDbTraktSyncer.py
--rw-rw-rw-   0        0        0        0 2023-04-29 22:05:24.000000 IMDbTraktSyncer-1.1.4/IMDbTraktSyncer/__init__.py
--rw-rw-rw-   0        0        0     1805 2023-05-15 09:11:52.000000 IMDbTraktSyncer-1.1.4/IMDbTraktSyncer/authTrakt.py
--rw-rw-rw-   0        0        0     4079 2023-05-15 09:11:52.000000 IMDbTraktSyncer-1.1.4/IMDbTraktSyncer/checkChromedriver.py
--rw-rw-rw-   0        0        0     2256 2023-05-16 00:33:22.000000 IMDbTraktSyncer-1.1.4/IMDbTraktSyncer/imdbRatings.py
--rw-rw-rw-   0        0        0     1876 2023-05-16 01:32:19.000000 IMDbTraktSyncer-1.1.4/IMDbTraktSyncer/traktRatings.py
--rw-rw-rw-   0        0        0     2516 2023-05-15 09:11:52.000000 IMDbTraktSyncer-1.1.4/IMDbTraktSyncer/verifyCredentials.py
-drwxrwxrwx   0        0        0        0 2023-05-16 01:36:43.513507 IMDbTraktSyncer-1.1.4/IMDbTraktSyncer.egg-info/
--rw-rw-rw-   0        0        0     6624 2023-05-16 01:36:43.000000 IMDbTraktSyncer-1.1.4/IMDbTraktSyncer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      491 2023-05-16 01:36:43.000000 IMDbTraktSyncer-1.1.4/IMDbTraktSyncer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-16 01:36:43.000000 IMDbTraktSyncer-1.1.4/IMDbTraktSyncer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       73 2023-05-16 01:36:43.000000 IMDbTraktSyncer-1.1.4/IMDbTraktSyncer.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       29 2023-05-16 01:36:43.000000 IMDbTraktSyncer-1.1.4/IMDbTraktSyncer.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-05-16 01:36:43.000000 IMDbTraktSyncer-1.1.4/IMDbTraktSyncer.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1079 2023-04-26 18:19:27.000000 IMDbTraktSyncer-1.1.4/LICENSE
--rw-rw-rw-   0        0        0     6624 2023-05-16 01:36:43.515005 IMDbTraktSyncer-1.1.4/PKG-INFO
--rw-rw-rw-   0        0        0     6004 2023-05-15 08:56:12.000000 IMDbTraktSyncer-1.1.4/README.md
--rw-rw-rw-   0        0        0       42 2023-05-16 01:36:43.516004 IMDbTraktSyncer-1.1.4/setup.cfg
--rw-rw-rw-   0        0        0     1287 2023-05-16 01:36:21.000000 IMDbTraktSyncer-1.1.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-18 02:42:15.321045 IMDbTraktSyncer-1.1.5/
+drwxrwxrwx   0        0        0        0 2023-05-18 02:42:15.288047 IMDbTraktSyncer-1.1.5/IMDbTraktSyncer/
+-rw-rw-rw-   0        0        0    10819 2023-05-18 02:39:31.000000 IMDbTraktSyncer-1.1.5/IMDbTraktSyncer/IMDbTraktSyncer.py
+-rw-rw-rw-   0        0        0        0 2023-05-16 21:29:26.000000 IMDbTraktSyncer-1.1.5/IMDbTraktSyncer/__init__.py
+-rw-rw-rw-   0        0        0     1794 2023-05-18 02:38:03.000000 IMDbTraktSyncer-1.1.5/IMDbTraktSyncer/authTrakt.py
+-rw-rw-rw-   0        0        0     4079 2023-05-16 21:29:26.000000 IMDbTraktSyncer-1.1.5/IMDbTraktSyncer/checkChromedriver.py
+-rw-rw-rw-   0        0        0     2256 2023-05-16 21:29:26.000000 IMDbTraktSyncer-1.1.5/IMDbTraktSyncer/imdbRatings.py
+-rw-rw-rw-   0        0        0     1846 2023-05-18 02:40:46.000000 IMDbTraktSyncer-1.1.5/IMDbTraktSyncer/traktRatings.py
+-rw-rw-rw-   0        0        0     2524 2023-05-18 02:41:11.000000 IMDbTraktSyncer-1.1.5/IMDbTraktSyncer/verifyCredentials.py
+drwxrwxrwx   0        0        0        0 2023-05-18 02:42:15.318045 IMDbTraktSyncer-1.1.5/IMDbTraktSyncer.egg-info/
+-rw-rw-rw-   0        0        0     7090 2023-05-18 02:42:15.000000 IMDbTraktSyncer-1.1.5/IMDbTraktSyncer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      491 2023-05-18 02:42:15.000000 IMDbTraktSyncer-1.1.5/IMDbTraktSyncer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-18 02:42:15.000000 IMDbTraktSyncer-1.1.5/IMDbTraktSyncer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       73 2023-05-18 02:42:15.000000 IMDbTraktSyncer-1.1.5/IMDbTraktSyncer.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       29 2023-05-18 02:42:15.000000 IMDbTraktSyncer-1.1.5/IMDbTraktSyncer.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-05-18 02:42:15.000000 IMDbTraktSyncer-1.1.5/IMDbTraktSyncer.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1079 2023-05-16 21:29:26.000000 IMDbTraktSyncer-1.1.5/LICENSE
+-rw-rw-rw-   0        0        0     7090 2023-05-18 02:42:15.320045 IMDbTraktSyncer-1.1.5/PKG-INFO
+-rw-rw-rw-   0        0        0     6467 2023-05-16 21:29:26.000000 IMDbTraktSyncer-1.1.5/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-18 02:42:15.321045 IMDbTraktSyncer-1.1.5/setup.cfg
+-rw-rw-rw-   0        0        0     1287 2023-05-18 02:41:48.000000 IMDbTraktSyncer-1.1.5/setup.py
```

### Comparing `IMDbTraktSyncer-1.1.4/IMDbTraktSyncer/IMDbTraktSyncer.py` & `IMDbTraktSyncer-1.1.5/IMDbTraktSyncer/IMDbTraktSyncer.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 import os
 import json
-import subprocess
 import requests
 import time
 import logging
 from selenium import webdriver
 from selenium.webdriver.chrome.service import Service
 from selenium.webdriver.common.by import By
 from selenium.common.exceptions import StaleElementReferenceException
```

### Comparing `IMDbTraktSyncer-1.1.4/IMDbTraktSyncer/authTrakt.py` & `IMDbTraktSyncer-1.1.5/IMDbTraktSyncer/authTrakt.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import requests
-import os
 
 def authenticate(client_id, client_secret):
     CLIENT_ID = client_id
     CLIENT_SECRET = client_secret
     REDIRECT_URI = 'urn:ietf:wg:oauth:2.0:oob'
 
     # Set up the authorization endpoint URL
```

### Comparing `IMDbTraktSyncer-1.1.4/IMDbTraktSyncer/checkChromedriver.py` & `IMDbTraktSyncer-1.1.5/IMDbTraktSyncer/checkChromedriver.py`

 * *Files identical despite different names*

### Comparing `IMDbTraktSyncer-1.1.4/IMDbTraktSyncer/imdbRatings.py` & `IMDbTraktSyncer-1.1.5/IMDbTraktSyncer/imdbRatings.py`

 * *Files identical despite different names*

### Comparing `IMDbTraktSyncer-1.1.4/IMDbTraktSyncer/traktRatings.py` & `IMDbTraktSyncer-1.1.5/IMDbTraktSyncer/traktRatings.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,8 @@
-import os
 import json
-import subprocess
 import requests
 
 def getTraktRatings(trakt_client_id, trakt_access_token):
     # Get Trakt Ratings
     print('Getting Trakt Ratings')
 
     headers = {
```

### Comparing `IMDbTraktSyncer-1.1.4/IMDbTraktSyncer/verifyCredentials.py` & `IMDbTraktSyncer-1.1.5/IMDbTraktSyncer/verifyCredentials.py`

 * *Files 8% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 # Load the values from the file
 with open(file_path, "r") as f:
     values = json.load(f)
 
 # Check if any of the values are "empty" and prompt the user to enter them
 for key in values.keys():
     if values[key] == "empty" and key != "trakt_access_token":
-        values[key] = input(f"Please enter a value for {key}: ")
+        values[key] = input(f"Please enter a value for {key}: ").strip()
         with open(file_path, "w") as f:
             json.dump(values, f)
 
 # Get the trakt_access_token value if it exists, or run the authTrakt.py function to get it
 trakt_access_token = None
 if "trakt_access_token" in values and values["trakt_access_token"] != "empty":
     trakt_access_token = values["trakt_access_token"]
```

### Comparing `IMDbTraktSyncer-1.1.4/IMDbTraktSyncer.egg-info/PKG-INFO` & `IMDbTraktSyncer-1.1.5/IMDbTraktSyncer.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: IMDbTraktSyncer
-Version: 1.1.4
+Version: 1.1.5
 Summary: This python script will sync user ratings for Movies and TV Shows both ways between Trakt and IMDb.
 Home-page: https://github.com/RileyXX/IMDb-Trakt-Syncer
 Keywords: python,video,trakt,imdb,ratings,sync,movies,tv shows
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 
 # IMDb-Trakt-Syncer
-This python script will sync user ratings for Movies and TV Shows both ways between Trakt and IMDb. Currently season and episode ratings are not supported. Ratings already set will not be overwritten. This script should work on an OS where python and chromedriver are supported (Windows, Linux, Mac, and ChromeOS).
+This python script will sync user ratings for Movies and TV Shows both ways between Trakt and IMDb. Ratings already set will not be overwritten. This script should work on an OS where python and chromedriver are supported (Windows, Linux, Mac, and ChromeOS). If you're looking to sync your ratings between Trakt, Plex, IMDB, and TMDB then these are my recommended projects: [PlexTraktSync](https://github.com/Taxel/PlexTraktSync), [IMDb-Trakt-Syncer](https://github.com/RileyXX/IMDb-Trakt-Syncer) & [TMDB-Trakt-Syncer](https://github.com/RileyXX/TMDB-Trakt-Syncer).
 ## Install Instructions:
 1. Install [Python](https://www.python.org/downloads/) and [Google Chrome](https://www.google.com/chrome/). _If these are already installed on your machine you can ignore this step. Please note this script does not effect Chrome in anyway it is simply required in order for chromedriver to work._
 2. Run `python -m pip install IMDbTraktSyncer` in command line.
 3. Login to [Trakt](https://trakt.tv/oauth/applications) and create a new API application. We will name it `IMDbTraktSyncer`. In the Redirect uri field enter `urn:ietf:wg:oauth:2.0:oob` then Save. 
 4. Run the script by calling `IMDbTraktSyncer` in command line. 
 5. Follow the prompts on first run. It will ask you to fill in your Trakt client id and client secret from step 3. It will also ask you to enter your IMDb username and password. Please note that these details are saved insecurely as credentials.txt in the same folder as the script. Recommended to change your password to something unique beforehand.
 6. Done, setup complete. The script will continue to run and sync your ratings. This may take some time, you can follow its progress in the command line.
@@ -27,14 +27,17 @@
 
 ## Update:
 `python -m pip install IMDbTraktSyncer --upgrade` in command line.
 
 ## Uninstall:
 `python -m pip uninstall IMDbTraktSyncer` in command line.
 
+## Install specific version:
+`python -m pip install IMDbTraktSyncer==VERSION_NUMBER` in command line. Replace `VERSION_NUMBER` with your [desired version](https://github.com/RileyXX/IMDb-Trakt-Syncer/releases).
+
 ## Alternative manual no pip install method:
 1. Install [Python](https://www.python.org/downloads/) and [Google Chrome](https://www.google.com/chrome/). _If these are already installed on your machine you can ignore this step. Please note this script does not effect Chrome in anyway it is simply required in order for chromedriver to work._
 2. Download the latest .zip from the [releases page](https://github.com/RileyXX/IMDb-Trakt-Syncer/releases) and extract it to the file directory of your choice.
 3. Login to [Trakt](https://trakt.tv/oauth/applications) and create a new API application. We will name it `IMDbTraktSyncer`. In the Redirect uri field enter `urn:ietf:wg:oauth:2.0:oob` then Save. 
 4. Run `IMDbTraktSyncer.py` OR open terminal and navigate to folder where `IMDbTraktSyncer.py` is located. Run `IMDbTraktSyncer.py` in terminal. 
 5. Follow the prompts on first run. It will ask you to fill in your Trakt client id and client secret from step 3. It will also ask you to enter your IMDb username and password. Please note that these details are saved insecurely as credentials.txt in the same folder as the script. Recommended to change your password to something unique beforehand.
 6. Done. The script will continue to run and sync your ratings. This may take some time, you can follow its progress in the command line.
```

### Comparing `IMDbTraktSyncer-1.1.4/LICENSE` & `IMDbTraktSyncer-1.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `IMDbTraktSyncer-1.1.4/PKG-INFO` & `IMDbTraktSyncer-1.1.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: IMDbTraktSyncer
-Version: 1.1.4
+Version: 1.1.5
 Summary: This python script will sync user ratings for Movies and TV Shows both ways between Trakt and IMDb.
 Home-page: https://github.com/RileyXX/IMDb-Trakt-Syncer
 Keywords: python,video,trakt,imdb,ratings,sync,movies,tv shows
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 
 # IMDb-Trakt-Syncer
-This python script will sync user ratings for Movies and TV Shows both ways between Trakt and IMDb. Currently season and episode ratings are not supported. Ratings already set will not be overwritten. This script should work on an OS where python and chromedriver are supported (Windows, Linux, Mac, and ChromeOS).
+This python script will sync user ratings for Movies and TV Shows both ways between Trakt and IMDb. Ratings already set will not be overwritten. This script should work on an OS where python and chromedriver are supported (Windows, Linux, Mac, and ChromeOS). If you're looking to sync your ratings between Trakt, Plex, IMDB, and TMDB then these are my recommended projects: [PlexTraktSync](https://github.com/Taxel/PlexTraktSync), [IMDb-Trakt-Syncer](https://github.com/RileyXX/IMDb-Trakt-Syncer) & [TMDB-Trakt-Syncer](https://github.com/RileyXX/TMDB-Trakt-Syncer).
 ## Install Instructions:
 1. Install [Python](https://www.python.org/downloads/) and [Google Chrome](https://www.google.com/chrome/). _If these are already installed on your machine you can ignore this step. Please note this script does not effect Chrome in anyway it is simply required in order for chromedriver to work._
 2. Run `python -m pip install IMDbTraktSyncer` in command line.
 3. Login to [Trakt](https://trakt.tv/oauth/applications) and create a new API application. We will name it `IMDbTraktSyncer`. In the Redirect uri field enter `urn:ietf:wg:oauth:2.0:oob` then Save. 
 4. Run the script by calling `IMDbTraktSyncer` in command line. 
 5. Follow the prompts on first run. It will ask you to fill in your Trakt client id and client secret from step 3. It will also ask you to enter your IMDb username and password. Please note that these details are saved insecurely as credentials.txt in the same folder as the script. Recommended to change your password to something unique beforehand.
 6. Done, setup complete. The script will continue to run and sync your ratings. This may take some time, you can follow its progress in the command line.
@@ -27,14 +27,17 @@
 
 ## Update:
 `python -m pip install IMDbTraktSyncer --upgrade` in command line.
 
 ## Uninstall:
 `python -m pip uninstall IMDbTraktSyncer` in command line.
 
+## Install specific version:
+`python -m pip install IMDbTraktSyncer==VERSION_NUMBER` in command line. Replace `VERSION_NUMBER` with your [desired version](https://github.com/RileyXX/IMDb-Trakt-Syncer/releases).
+
 ## Alternative manual no pip install method:
 1. Install [Python](https://www.python.org/downloads/) and [Google Chrome](https://www.google.com/chrome/). _If these are already installed on your machine you can ignore this step. Please note this script does not effect Chrome in anyway it is simply required in order for chromedriver to work._
 2. Download the latest .zip from the [releases page](https://github.com/RileyXX/IMDb-Trakt-Syncer/releases) and extract it to the file directory of your choice.
 3. Login to [Trakt](https://trakt.tv/oauth/applications) and create a new API application. We will name it `IMDbTraktSyncer`. In the Redirect uri field enter `urn:ietf:wg:oauth:2.0:oob` then Save. 
 4. Run `IMDbTraktSyncer.py` OR open terminal and navigate to folder where `IMDbTraktSyncer.py` is located. Run `IMDbTraktSyncer.py` in terminal. 
 5. Follow the prompts on first run. It will ask you to fill in your Trakt client id and client secret from step 3. It will also ask you to enter your IMDb username and password. Please note that these details are saved insecurely as credentials.txt in the same folder as the script. Recommended to change your password to something unique beforehand.
 6. Done. The script will continue to run and sync your ratings. This may take some time, you can follow its progress in the command line.
```

### Comparing `IMDbTraktSyncer-1.1.4/README.md` & `IMDbTraktSyncer-1.1.5/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # IMDb-Trakt-Syncer
-This python script will sync user ratings for Movies and TV Shows both ways between Trakt and IMDb. Currently season and episode ratings are not supported. Ratings already set will not be overwritten. This script should work on an OS where python and chromedriver are supported (Windows, Linux, Mac, and ChromeOS).
+This python script will sync user ratings for Movies and TV Shows both ways between Trakt and IMDb. Ratings already set will not be overwritten. This script should work on an OS where python and chromedriver are supported (Windows, Linux, Mac, and ChromeOS). If you're looking to sync your ratings between Trakt, Plex, IMDB, and TMDB then these are my recommended projects: [PlexTraktSync](https://github.com/Taxel/PlexTraktSync), [IMDb-Trakt-Syncer](https://github.com/RileyXX/IMDb-Trakt-Syncer) & [TMDB-Trakt-Syncer](https://github.com/RileyXX/TMDB-Trakt-Syncer).
 ## Install Instructions:
 1. Install [Python](https://www.python.org/downloads/) and [Google Chrome](https://www.google.com/chrome/). _If these are already installed on your machine you can ignore this step. Please note this script does not effect Chrome in anyway it is simply required in order for chromedriver to work._
 2. Run `python -m pip install IMDbTraktSyncer` in command line.
 3. Login to [Trakt](https://trakt.tv/oauth/applications) and create a new API application. We will name it `IMDbTraktSyncer`. In the Redirect uri field enter `urn:ietf:wg:oauth:2.0:oob` then Save. 
 4. Run the script by calling `IMDbTraktSyncer` in command line. 
 5. Follow the prompts on first run. It will ask you to fill in your Trakt client id and client secret from step 3. It will also ask you to enter your IMDb username and password. Please note that these details are saved insecurely as credentials.txt in the same folder as the script. Recommended to change your password to something unique beforehand.
 6. Done, setup complete. The script will continue to run and sync your ratings. This may take some time, you can follow its progress in the command line.
@@ -13,14 +13,17 @@
 
 ## Update:
 `python -m pip install IMDbTraktSyncer --upgrade` in command line.
 
 ## Uninstall:
 `python -m pip uninstall IMDbTraktSyncer` in command line.
 
+## Install specific version:
+`python -m pip install IMDbTraktSyncer==VERSION_NUMBER` in command line. Replace `VERSION_NUMBER` with your [desired version](https://github.com/RileyXX/IMDb-Trakt-Syncer/releases).
+
 ## Alternative manual no pip install method:
 1. Install [Python](https://www.python.org/downloads/) and [Google Chrome](https://www.google.com/chrome/). _If these are already installed on your machine you can ignore this step. Please note this script does not effect Chrome in anyway it is simply required in order for chromedriver to work._
 2. Download the latest .zip from the [releases page](https://github.com/RileyXX/IMDb-Trakt-Syncer/releases) and extract it to the file directory of your choice.
 3. Login to [Trakt](https://trakt.tv/oauth/applications) and create a new API application. We will name it `IMDbTraktSyncer`. In the Redirect uri field enter `urn:ietf:wg:oauth:2.0:oob` then Save. 
 4. Run `IMDbTraktSyncer.py` OR open terminal and navigate to folder where `IMDbTraktSyncer.py` is located. Run `IMDbTraktSyncer.py` in terminal. 
 5. Follow the prompts on first run. It will ask you to fill in your Trakt client id and client secret from step 3. It will also ask you to enter your IMDb username and password. Please note that these details are saved insecurely as credentials.txt in the same folder as the script. Recommended to change your password to something unique beforehand.
 6. Done. The script will continue to run and sync your ratings. This may take some time, you can follow its progress in the command line.
```

### Comparing `IMDbTraktSyncer-1.1.4/setup.py` & `IMDbTraktSyncer-1.1.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 #To upload package: twine upload dist/*
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '1.1.4'
+VERSION = '1.1.5'
 DESCRIPTION = 'This python script will sync user ratings for Movies and TV Shows both ways between Trakt and IMDb.'
 
 # Setting up
 setup(
     name="IMDbTraktSyncer",
     version=VERSION,
     description=DESCRIPTION,
```

