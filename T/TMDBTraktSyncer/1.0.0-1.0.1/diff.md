# Comparing `tmp/TMDBTraktSyncer-1.0.0.tar.gz` & `tmp/TMDBTraktSyncer-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TMDBTraktSyncer-1.0.0.tar", last modified: Tue May 16 23:40:08 2023, max compression
+gzip compressed data, was "TMDBTraktSyncer-1.0.1.tar", last modified: Thu May 18 02:29:57 2023, max compression
```

## Comparing `TMDBTraktSyncer-1.0.0.tar` & `TMDBTraktSyncer-1.0.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-05-16 23:40:08.681217 TMDBTraktSyncer-1.0.0/
--rw-rw-rw-   0        0        0     1079 2023-04-26 18:19:27.000000 TMDBTraktSyncer-1.0.0/LICENSE
--rw-rw-rw-   0        0        0     5758 2023-05-16 23:40:08.680217 TMDBTraktSyncer-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     5136 2023-05-16 23:32:27.000000 TMDBTraktSyncer-1.0.0/README.md
-drwxrwxrwx   0        0        0        0 2023-05-16 23:40:08.661217 TMDBTraktSyncer-1.0.0/TMDBTraktSyncer/
--rw-rw-rw-   0        0        0     6373 2023-05-16 22:39:43.000000 TMDBTraktSyncer-1.0.0/TMDBTraktSyncer/TMDBTraktSyncer.py
--rw-rw-rw-   0        0        0        0 2023-04-29 22:05:24.000000 TMDBTraktSyncer-1.0.0/TMDBTraktSyncer/__init__.py
--rw-rw-rw-   0        0        0     1805 2023-05-15 09:11:52.000000 TMDBTraktSyncer-1.0.0/TMDBTraktSyncer/authTrakt.py
--rw-rw-rw-   0        0        0     2997 2023-05-16 22:31:56.000000 TMDBTraktSyncer-1.0.0/TMDBTraktSyncer/tmdbRatings.py
--rw-rw-rw-   0        0        0     2181 2023-05-16 22:31:26.000000 TMDBTraktSyncer-1.0.0/TMDBTraktSyncer/traktRatings.py
--rw-rw-rw-   0        0        0     1814 2023-05-16 18:56:40.000000 TMDBTraktSyncer-1.0.0/TMDBTraktSyncer/verifyCredentials.py
-drwxrwxrwx   0        0        0        0 2023-05-16 23:40:08.679217 TMDBTraktSyncer-1.0.0/TMDBTraktSyncer.egg-info/
--rw-rw-rw-   0        0        0     5758 2023-05-16 23:40:08.000000 TMDBTraktSyncer-1.0.0/TMDBTraktSyncer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      454 2023-05-16 23:40:08.000000 TMDBTraktSyncer-1.0.0/TMDBTraktSyncer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-16 23:40:08.000000 TMDBTraktSyncer-1.0.0/TMDBTraktSyncer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       73 2023-05-16 23:40:08.000000 TMDBTraktSyncer-1.0.0/TMDBTraktSyncer.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        9 2023-05-16 23:40:08.000000 TMDBTraktSyncer-1.0.0/TMDBTraktSyncer.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-05-16 23:40:08.000000 TMDBTraktSyncer-1.0.0/TMDBTraktSyncer.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-16 23:40:08.681217 TMDBTraktSyncer-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0     1261 2023-05-16 22:44:31.000000 TMDBTraktSyncer-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-18 02:29:57.382074 TMDBTraktSyncer-1.0.1/
+-rw-rw-rw-   0        0        0     1079 2023-04-26 18:19:27.000000 TMDBTraktSyncer-1.0.1/LICENSE
+-rw-rw-rw-   0        0        0     5905 2023-05-18 02:29:57.382074 TMDBTraktSyncer-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     5282 2023-05-18 02:27:35.000000 TMDBTraktSyncer-1.0.1/README.md
+drwxrwxrwx   0        0        0        0 2023-05-18 02:29:57.350601 TMDBTraktSyncer-1.0.1/TMDBTraktSyncer/
+-rw-rw-rw-   0        0        0     6373 2023-05-18 02:25:14.000000 TMDBTraktSyncer-1.0.1/TMDBTraktSyncer/TMDBTraktSyncer.py
+-rw-rw-rw-   0        0        0        0 2023-04-29 22:05:24.000000 TMDBTraktSyncer-1.0.1/TMDBTraktSyncer/__init__.py
+-rw-rw-rw-   0        0        0     1805 2023-05-18 02:25:14.000000 TMDBTraktSyncer-1.0.1/TMDBTraktSyncer/authTrakt.py
+-rw-rw-rw-   0        0        0     2997 2023-05-18 02:25:14.000000 TMDBTraktSyncer-1.0.1/TMDBTraktSyncer/tmdbRatings.py
+-rw-rw-rw-   0        0        0     2181 2023-05-18 02:25:14.000000 TMDBTraktSyncer-1.0.1/TMDBTraktSyncer/traktRatings.py
+-rw-rw-rw-   0        0        0     1822 2023-05-18 02:26:48.000000 TMDBTraktSyncer-1.0.1/TMDBTraktSyncer/verifyCredentials.py
+drwxrwxrwx   0        0        0        0 2023-05-18 02:29:57.380072 TMDBTraktSyncer-1.0.1/TMDBTraktSyncer.egg-info/
+-rw-rw-rw-   0        0        0     5905 2023-05-18 02:29:57.000000 TMDBTraktSyncer-1.0.1/TMDBTraktSyncer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      454 2023-05-18 02:29:57.000000 TMDBTraktSyncer-1.0.1/TMDBTraktSyncer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-18 02:29:57.000000 TMDBTraktSyncer-1.0.1/TMDBTraktSyncer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       73 2023-05-18 02:29:57.000000 TMDBTraktSyncer-1.0.1/TMDBTraktSyncer.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        9 2023-05-18 02:29:57.000000 TMDBTraktSyncer-1.0.1/TMDBTraktSyncer.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-05-18 02:29:57.000000 TMDBTraktSyncer-1.0.1/TMDBTraktSyncer.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-18 02:29:57.383074 TMDBTraktSyncer-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0     1261 2023-05-18 02:28:20.000000 TMDBTraktSyncer-1.0.1/setup.py
```

### Comparing `TMDBTraktSyncer-1.0.0/LICENSE` & `TMDBTraktSyncer-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `TMDBTraktSyncer-1.0.0/PKG-INFO` & `TMDBTraktSyncer-1.0.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 Metadata-Version: 2.1
 Name: TMDBTraktSyncer
-Version: 1.0.0
+Version: 1.0.1
 Summary: This python script will sync user ratings for Movies and TV Shows both ways between Trakt and TMDB.
 Home-page: https://github.com/RileyXX/TMDB-Trakt-Syncer
 Keywords: python,video,trakt,tmdb,ratings,sync,movies,tv shows
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 
 # TMDB-Trakt-Syncer
-This python script will sync user ratings for Movies and TV Shows both ways between Trakt and TMDB. Ratings already set will not be overwritten. This script should work on an OS where python is supported (Windows, Linux, Mac, ChromeOS, etc). If you're looking to sync your ratings between Trakt, Plex, IMDB, and TMDB then these are my recommended projects: [PlexTraktSync](https://github.com/Taxel/PlexTraktSync), [IMDb-Trakt-Syncer](https://github.com/RileyXX/IMDb-Trakt-Syncer) & [TMDB-Trakt-Syncer](https://github.com/RileyXX/TMDB-Trakt-Syncer).
+This python script will sync user ratings for Movies and TV Shows and episodes both ways between [Trakt](https://trakt.tv/dashboard) and [TMDB](https://www.themoviedb.org/). Ratings already set will not be overwritten. This script should work on an OS where python is supported (Windows, Linux, Mac, ChromeOS, etc). If you're looking to sync your ratings between Trakt, Plex, IMDB, and TMDB then these are my recommended projects: [PlexTraktSync](https://github.com/Taxel/PlexTraktSync), [IMDb-Trakt-Syncer](https://github.com/RileyXX/IMDb-Trakt-Syncer) & [TMDB-Trakt-Syncer](https://github.com/RileyXX/TMDB-Trakt-Syncer).
 ## Install Instructions:
 1. Install [Python](https://www.python.org/downloads/). 
-2. Run `python -m pip install TMDbTraktSyncer` in command line.
+2. Run `python -m pip install TMDBTraktSyncer` in command line.
 3. Login to [Trakt](https://trakt.tv/oauth/applications) and create a new API application. We will name it `TMDbTraktSyncer`. In the Redirect uri field enter `urn:ietf:wg:oauth:2.0:oob` then Save. 
-4. Login to [TMDB](https://www.themoviedb.org/settings/api/) and create a new API application. Choose developer, accept the terms and start filling out the application form. For type of use `Personal`. For application name we will call it `TMDB-Trakt-Sync`. For application url enter `localhost`. For application summary enter `Use TMDB api and Trakt api to sync ratings user ratings between platforms. https://github.com/RileyXX/TMDB-Trakt-Syncer`. Fill in the rest of the fields with whatever you want and submit. Your api keys will be instantly generated.
-5. Run the script by calling `TMDbTraktSyncer` in command line. 
+4. Login to [TMDB](https://www.themoviedb.org/settings/api/) and create a new API application. Choose developer, accept the terms and start filling out the application form. For type of use `Personal`. For application name we will call it `TMDB-Trakt-Sync`. For application url enter `localhost`. For application summary enter `Use TMDB api and Trakt api to sync user ratings between platforms. https://github.com/RileyXX/TMDB-Trakt-Syncer`. Fill in the rest of the fields with whatever you want and submit. Your api keys will be instantly generated.
+5. Run the script by calling `TMDBTraktSyncer` in command line. 
 6. Follow the prompts on first run. It will ask you to fill in your Trakt client id and client secret from step 3. It will also ask you to fill in your tmdb_v4_token from step 4. Please note that these details are saved insecurely as credentials.txt in the same folder as the script.
 7. Done, setup complete. The script will continue to run and sync your ratings. This may take some time, you can follow its progress in the command line.
 
 ## Run:
 `TMDBTraktSyncer` in command line.
 
 ## Update:
@@ -33,22 +33,23 @@
 `python -m pip uninstall TMDBTraktSyncer` in command line.
 
 ## Install specific version:
 `python -m pip install TMDBTraktSyncer==VERSION_NUMBER` in command line. Replace `VERSION_NUMBER` with your [desired version](https://github.com/RileyXX/TMDb-Trakt-Syncer/releases).
 
 ## Alternative manual no pip install method:
 1. Install [Python](https://www.python.org/downloads/).
-2. Download the latest .zip from the [releases page](https://github.com/RileyXX/TMDb-Trakt-Syncer/releases) and extract it to the file directory of your choice.
+2. Download the latest .zip from the [releases page](https://github.com/RileyXX/TMDB-Trakt-Syncer/releases) and extract it to the file directory of your choice.
 3. Login to [Trakt](https://trakt.tv/oauth/applications) and create a new API application. We will name it `TMDBTraktSyncer`. In the Redirect uri field enter `urn:ietf:wg:oauth:2.0:oob` then Save. 
-4. Login to [TMDB](https://www.themoviedb.org/settings/api/) and create a new API application. Choose developer, accept the terms and start filling out the application form. For type of use `Personal`. For application name we will call it `TMDB-Trakt-Sync`. For application url enter `localhost`. For application summary enter `Use TMDB api and Trakt api to sync ratings user ratings between platforms. https://github.com/RileyXX/TMDB-Trakt-Syncer`. Fill in the rest of the fields with whatever you want and submit. Your api keys will be instantly generated.
+4. Login to [TMDB](https://www.themoviedb.org/settings/api/) and create a new API application. Choose developer, accept the terms and start filling out the application form. For type of use `Personal`. For application name we will call it `TMDB-Trakt-Sync`. For application url enter `localhost`. For application summary enter `Use TMDB api and Trakt api to sync user ratings between platforms. https://github.com/RileyXX/TMDB-Trakt-Syncer`. Fill in the rest of the fields with whatever you want and submit. Your api keys will be instantly generated.
 5. Run `TMDBTraktSyncer.py` OR open terminal and navigate to folder where `TMDBTraktSyncer.py` is located. Run `TMDBTraktSyncer.py` in terminal. 
 6. Follow the prompts on first run. It will ask you to fill in your Trakt client id and client secret from step 3. It will also ask you to fill in your tmdb_v4_token from step 4. Please note that these details are saved insecurely as credentials.txt in the same folder as the script. 
 7. Done. The script will continue to run and sync your ratings. This may take some time, you can follow its progress in the command line.
 
 ## Troubleshooting, known issues, workarounds & future outlook:
+* Add support for review/comment sync https://github.com/RileyXX/TMDB-Trakt-Syncer/issues/1
 * If any of your details change, passwords, logins, api keys etc, just delete credentials.txt and that will reset the script. It will prompt you to enter your new details on next run.
 
 ## Screenshot:
 ![Demo](https://i.imgur.com/5LI04O2.png)
 
 
 ## Sponsorships, Donations and Custom Projects:
@@ -57,13 +58,13 @@
 #### More donation options:
 - Cashapp: `$rileyxx`
 - Venmo: `@rileyxx`
 - Bitcoin: `bc1qrjevwqv49z8y77len3azqfghxrjmrjvhy5zqau`
 - Amazon Wishlist: [Link ↗](https://www.amazon.com/hz/wishlist/ls/WURF5NWZ843U)
 
 ## Also posted on:
-* [PyPi](https://pypi.org/project/TMDbTraktSyncer/)
-* [Reddit](https://www.reddit.com/r/trakt/comments/132heo0/imdb_trakt_rating_syncer_tool_sync_both_ways/)
+* [PyPi](https://pypi.org/project/TMDBTraktSyncer/)
+* [Reddit](https://www.reddit.com/r/trakt/comments/13jlu4r/tmdb_trakt_rating_syncer_tool_2_way_sync/)
 
 <br>
 
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
```

### Comparing `TMDBTraktSyncer-1.0.0/README.md` & `TMDBTraktSyncer-1.0.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # TMDB-Trakt-Syncer
-This python script will sync user ratings for Movies and TV Shows both ways between Trakt and TMDB. Ratings already set will not be overwritten. This script should work on an OS where python is supported (Windows, Linux, Mac, ChromeOS, etc). If you're looking to sync your ratings between Trakt, Plex, IMDB, and TMDB then these are my recommended projects: [PlexTraktSync](https://github.com/Taxel/PlexTraktSync), [IMDb-Trakt-Syncer](https://github.com/RileyXX/IMDb-Trakt-Syncer) & [TMDB-Trakt-Syncer](https://github.com/RileyXX/TMDB-Trakt-Syncer).
+This python script will sync user ratings for Movies and TV Shows and episodes both ways between [Trakt](https://trakt.tv/dashboard) and [TMDB](https://www.themoviedb.org/). Ratings already set will not be overwritten. This script should work on an OS where python is supported (Windows, Linux, Mac, ChromeOS, etc). If you're looking to sync your ratings between Trakt, Plex, IMDB, and TMDB then these are my recommended projects: [PlexTraktSync](https://github.com/Taxel/PlexTraktSync), [IMDb-Trakt-Syncer](https://github.com/RileyXX/IMDb-Trakt-Syncer) & [TMDB-Trakt-Syncer](https://github.com/RileyXX/TMDB-Trakt-Syncer).
 ## Install Instructions:
 1. Install [Python](https://www.python.org/downloads/). 
-2. Run `python -m pip install TMDbTraktSyncer` in command line.
+2. Run `python -m pip install TMDBTraktSyncer` in command line.
 3. Login to [Trakt](https://trakt.tv/oauth/applications) and create a new API application. We will name it `TMDbTraktSyncer`. In the Redirect uri field enter `urn:ietf:wg:oauth:2.0:oob` then Save. 
-4. Login to [TMDB](https://www.themoviedb.org/settings/api/) and create a new API application. Choose developer, accept the terms and start filling out the application form. For type of use `Personal`. For application name we will call it `TMDB-Trakt-Sync`. For application url enter `localhost`. For application summary enter `Use TMDB api and Trakt api to sync ratings user ratings between platforms. https://github.com/RileyXX/TMDB-Trakt-Syncer`. Fill in the rest of the fields with whatever you want and submit. Your api keys will be instantly generated.
-5. Run the script by calling `TMDbTraktSyncer` in command line. 
+4. Login to [TMDB](https://www.themoviedb.org/settings/api/) and create a new API application. Choose developer, accept the terms and start filling out the application form. For type of use `Personal`. For application name we will call it `TMDB-Trakt-Sync`. For application url enter `localhost`. For application summary enter `Use TMDB api and Trakt api to sync user ratings between platforms. https://github.com/RileyXX/TMDB-Trakt-Syncer`. Fill in the rest of the fields with whatever you want and submit. Your api keys will be instantly generated.
+5. Run the script by calling `TMDBTraktSyncer` in command line. 
 6. Follow the prompts on first run. It will ask you to fill in your Trakt client id and client secret from step 3. It will also ask you to fill in your tmdb_v4_token from step 4. Please note that these details are saved insecurely as credentials.txt in the same folder as the script.
 7. Done, setup complete. The script will continue to run and sync your ratings. This may take some time, you can follow its progress in the command line.
 
 ## Run:
 `TMDBTraktSyncer` in command line.
 
 ## Update:
@@ -19,22 +19,23 @@
 `python -m pip uninstall TMDBTraktSyncer` in command line.
 
 ## Install specific version:
 `python -m pip install TMDBTraktSyncer==VERSION_NUMBER` in command line. Replace `VERSION_NUMBER` with your [desired version](https://github.com/RileyXX/TMDb-Trakt-Syncer/releases).
 
 ## Alternative manual no pip install method:
 1. Install [Python](https://www.python.org/downloads/).
-2. Download the latest .zip from the [releases page](https://github.com/RileyXX/TMDb-Trakt-Syncer/releases) and extract it to the file directory of your choice.
+2. Download the latest .zip from the [releases page](https://github.com/RileyXX/TMDB-Trakt-Syncer/releases) and extract it to the file directory of your choice.
 3. Login to [Trakt](https://trakt.tv/oauth/applications) and create a new API application. We will name it `TMDBTraktSyncer`. In the Redirect uri field enter `urn:ietf:wg:oauth:2.0:oob` then Save. 
-4. Login to [TMDB](https://www.themoviedb.org/settings/api/) and create a new API application. Choose developer, accept the terms and start filling out the application form. For type of use `Personal`. For application name we will call it `TMDB-Trakt-Sync`. For application url enter `localhost`. For application summary enter `Use TMDB api and Trakt api to sync ratings user ratings between platforms. https://github.com/RileyXX/TMDB-Trakt-Syncer`. Fill in the rest of the fields with whatever you want and submit. Your api keys will be instantly generated.
+4. Login to [TMDB](https://www.themoviedb.org/settings/api/) and create a new API application. Choose developer, accept the terms and start filling out the application form. For type of use `Personal`. For application name we will call it `TMDB-Trakt-Sync`. For application url enter `localhost`. For application summary enter `Use TMDB api and Trakt api to sync user ratings between platforms. https://github.com/RileyXX/TMDB-Trakt-Syncer`. Fill in the rest of the fields with whatever you want and submit. Your api keys will be instantly generated.
 5. Run `TMDBTraktSyncer.py` OR open terminal and navigate to folder where `TMDBTraktSyncer.py` is located. Run `TMDBTraktSyncer.py` in terminal. 
 6. Follow the prompts on first run. It will ask you to fill in your Trakt client id and client secret from step 3. It will also ask you to fill in your tmdb_v4_token from step 4. Please note that these details are saved insecurely as credentials.txt in the same folder as the script. 
 7. Done. The script will continue to run and sync your ratings. This may take some time, you can follow its progress in the command line.
 
 ## Troubleshooting, known issues, workarounds & future outlook:
+* Add support for review/comment sync https://github.com/RileyXX/TMDB-Trakt-Syncer/issues/1
 * If any of your details change, passwords, logins, api keys etc, just delete credentials.txt and that will reset the script. It will prompt you to enter your new details on next run.
 
 ## Screenshot:
 ![Demo](https://i.imgur.com/5LI04O2.png)
 
 
 ## Sponsorships, Donations and Custom Projects:
@@ -43,13 +44,13 @@
 #### More donation options:
 - Cashapp: `$rileyxx`
 - Venmo: `@rileyxx`
 - Bitcoin: `bc1qrjevwqv49z8y77len3azqfghxrjmrjvhy5zqau`
 - Amazon Wishlist: [Link ↗](https://www.amazon.com/hz/wishlist/ls/WURF5NWZ843U)
 
 ## Also posted on:
-* [PyPi](https://pypi.org/project/TMDbTraktSyncer/)
-* [Reddit](https://www.reddit.com/r/trakt/comments/132heo0/imdb_trakt_rating_syncer_tool_sync_both_ways/)
+* [PyPi](https://pypi.org/project/TMDBTraktSyncer/)
+* [Reddit](https://www.reddit.com/r/trakt/comments/13jlu4r/tmdb_trakt_rating_syncer_tool_2_way_sync/)
 
 <br>
 
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
```

### Comparing `TMDBTraktSyncer-1.0.0/TMDBTraktSyncer/TMDBTraktSyncer.py` & `TMDBTraktSyncer-1.0.1/TMDBTraktSyncer/TMDBTraktSyncer.py`

 * *Files identical despite different names*

### Comparing `TMDBTraktSyncer-1.0.0/TMDBTraktSyncer/authTrakt.py` & `TMDBTraktSyncer-1.0.1/TMDBTraktSyncer/authTrakt.py`

 * *Files identical despite different names*

### Comparing `TMDBTraktSyncer-1.0.0/TMDBTraktSyncer/tmdbRatings.py` & `TMDBTraktSyncer-1.0.1/TMDBTraktSyncer/tmdbRatings.py`

 * *Files identical despite different names*

### Comparing `TMDBTraktSyncer-1.0.0/TMDBTraktSyncer/traktRatings.py` & `TMDBTraktSyncer-1.0.1/TMDBTraktSyncer/traktRatings.py`

 * *Files identical despite different names*

### Comparing `TMDBTraktSyncer-1.0.0/TMDBTraktSyncer/verifyCredentials.py` & `TMDBTraktSyncer-1.0.1/TMDBTraktSyncer/verifyCredentials.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,15 @@
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

### Comparing `TMDBTraktSyncer-1.0.0/TMDBTraktSyncer.egg-info/PKG-INFO` & `TMDBTraktSyncer-1.0.1/TMDBTraktSyncer.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 Metadata-Version: 2.1
 Name: TMDBTraktSyncer
-Version: 1.0.0
+Version: 1.0.1
 Summary: This python script will sync user ratings for Movies and TV Shows both ways between Trakt and TMDB.
 Home-page: https://github.com/RileyXX/TMDB-Trakt-Syncer
 Keywords: python,video,trakt,tmdb,ratings,sync,movies,tv shows
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 
 # TMDB-Trakt-Syncer
-This python script will sync user ratings for Movies and TV Shows both ways between Trakt and TMDB. Ratings already set will not be overwritten. This script should work on an OS where python is supported (Windows, Linux, Mac, ChromeOS, etc). If you're looking to sync your ratings between Trakt, Plex, IMDB, and TMDB then these are my recommended projects: [PlexTraktSync](https://github.com/Taxel/PlexTraktSync), [IMDb-Trakt-Syncer](https://github.com/RileyXX/IMDb-Trakt-Syncer) & [TMDB-Trakt-Syncer](https://github.com/RileyXX/TMDB-Trakt-Syncer).
+This python script will sync user ratings for Movies and TV Shows and episodes both ways between [Trakt](https://trakt.tv/dashboard) and [TMDB](https://www.themoviedb.org/). Ratings already set will not be overwritten. This script should work on an OS where python is supported (Windows, Linux, Mac, ChromeOS, etc). If you're looking to sync your ratings between Trakt, Plex, IMDB, and TMDB then these are my recommended projects: [PlexTraktSync](https://github.com/Taxel/PlexTraktSync), [IMDb-Trakt-Syncer](https://github.com/RileyXX/IMDb-Trakt-Syncer) & [TMDB-Trakt-Syncer](https://github.com/RileyXX/TMDB-Trakt-Syncer).
 ## Install Instructions:
 1. Install [Python](https://www.python.org/downloads/). 
-2. Run `python -m pip install TMDbTraktSyncer` in command line.
+2. Run `python -m pip install TMDBTraktSyncer` in command line.
 3. Login to [Trakt](https://trakt.tv/oauth/applications) and create a new API application. We will name it `TMDbTraktSyncer`. In the Redirect uri field enter `urn:ietf:wg:oauth:2.0:oob` then Save. 
-4. Login to [TMDB](https://www.themoviedb.org/settings/api/) and create a new API application. Choose developer, accept the terms and start filling out the application form. For type of use `Personal`. For application name we will call it `TMDB-Trakt-Sync`. For application url enter `localhost`. For application summary enter `Use TMDB api and Trakt api to sync ratings user ratings between platforms. https://github.com/RileyXX/TMDB-Trakt-Syncer`. Fill in the rest of the fields with whatever you want and submit. Your api keys will be instantly generated.
-5. Run the script by calling `TMDbTraktSyncer` in command line. 
+4. Login to [TMDB](https://www.themoviedb.org/settings/api/) and create a new API application. Choose developer, accept the terms and start filling out the application form. For type of use `Personal`. For application name we will call it `TMDB-Trakt-Sync`. For application url enter `localhost`. For application summary enter `Use TMDB api and Trakt api to sync user ratings between platforms. https://github.com/RileyXX/TMDB-Trakt-Syncer`. Fill in the rest of the fields with whatever you want and submit. Your api keys will be instantly generated.
+5. Run the script by calling `TMDBTraktSyncer` in command line. 
 6. Follow the prompts on first run. It will ask you to fill in your Trakt client id and client secret from step 3. It will also ask you to fill in your tmdb_v4_token from step 4. Please note that these details are saved insecurely as credentials.txt in the same folder as the script.
 7. Done, setup complete. The script will continue to run and sync your ratings. This may take some time, you can follow its progress in the command line.
 
 ## Run:
 `TMDBTraktSyncer` in command line.
 
 ## Update:
@@ -33,22 +33,23 @@
 `python -m pip uninstall TMDBTraktSyncer` in command line.
 
 ## Install specific version:
 `python -m pip install TMDBTraktSyncer==VERSION_NUMBER` in command line. Replace `VERSION_NUMBER` with your [desired version](https://github.com/RileyXX/TMDb-Trakt-Syncer/releases).
 
 ## Alternative manual no pip install method:
 1. Install [Python](https://www.python.org/downloads/).
-2. Download the latest .zip from the [releases page](https://github.com/RileyXX/TMDb-Trakt-Syncer/releases) and extract it to the file directory of your choice.
+2. Download the latest .zip from the [releases page](https://github.com/RileyXX/TMDB-Trakt-Syncer/releases) and extract it to the file directory of your choice.
 3. Login to [Trakt](https://trakt.tv/oauth/applications) and create a new API application. We will name it `TMDBTraktSyncer`. In the Redirect uri field enter `urn:ietf:wg:oauth:2.0:oob` then Save. 
-4. Login to [TMDB](https://www.themoviedb.org/settings/api/) and create a new API application. Choose developer, accept the terms and start filling out the application form. For type of use `Personal`. For application name we will call it `TMDB-Trakt-Sync`. For application url enter `localhost`. For application summary enter `Use TMDB api and Trakt api to sync ratings user ratings between platforms. https://github.com/RileyXX/TMDB-Trakt-Syncer`. Fill in the rest of the fields with whatever you want and submit. Your api keys will be instantly generated.
+4. Login to [TMDB](https://www.themoviedb.org/settings/api/) and create a new API application. Choose developer, accept the terms and start filling out the application form. For type of use `Personal`. For application name we will call it `TMDB-Trakt-Sync`. For application url enter `localhost`. For application summary enter `Use TMDB api and Trakt api to sync user ratings between platforms. https://github.com/RileyXX/TMDB-Trakt-Syncer`. Fill in the rest of the fields with whatever you want and submit. Your api keys will be instantly generated.
 5. Run `TMDBTraktSyncer.py` OR open terminal and navigate to folder where `TMDBTraktSyncer.py` is located. Run `TMDBTraktSyncer.py` in terminal. 
 6. Follow the prompts on first run. It will ask you to fill in your Trakt client id and client secret from step 3. It will also ask you to fill in your tmdb_v4_token from step 4. Please note that these details are saved insecurely as credentials.txt in the same folder as the script. 
 7. Done. The script will continue to run and sync your ratings. This may take some time, you can follow its progress in the command line.
 
 ## Troubleshooting, known issues, workarounds & future outlook:
+* Add support for review/comment sync https://github.com/RileyXX/TMDB-Trakt-Syncer/issues/1
 * If any of your details change, passwords, logins, api keys etc, just delete credentials.txt and that will reset the script. It will prompt you to enter your new details on next run.
 
 ## Screenshot:
 ![Demo](https://i.imgur.com/5LI04O2.png)
 
 
 ## Sponsorships, Donations and Custom Projects:
@@ -57,13 +58,13 @@
 #### More donation options:
 - Cashapp: `$rileyxx`
 - Venmo: `@rileyxx`
 - Bitcoin: `bc1qrjevwqv49z8y77len3azqfghxrjmrjvhy5zqau`
 - Amazon Wishlist: [Link ↗](https://www.amazon.com/hz/wishlist/ls/WURF5NWZ843U)
 
 ## Also posted on:
-* [PyPi](https://pypi.org/project/TMDbTraktSyncer/)
-* [Reddit](https://www.reddit.com/r/trakt/comments/132heo0/imdb_trakt_rating_syncer_tool_sync_both_ways/)
+* [PyPi](https://pypi.org/project/TMDBTraktSyncer/)
+* [Reddit](https://www.reddit.com/r/trakt/comments/13jlu4r/tmdb_trakt_rating_syncer_tool_2_way_sync/)
 
 <br>
 
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
```

### Comparing `TMDBTraktSyncer-1.0.0/setup.py` & `TMDBTraktSyncer-1.0.1/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 #To upload package: twine upload dist/*
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '1.0.0'
+VERSION = '1.0.1'
 DESCRIPTION = 'This python script will sync user ratings for Movies and TV Shows both ways between Trakt and TMDB.'
 
 # Setting up
 setup(
     name="TMDBTraktSyncer",
     version=VERSION,
     description=DESCRIPTION,
```

