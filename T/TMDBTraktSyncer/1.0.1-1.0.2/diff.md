# Comparing `tmp/TMDBTraktSyncer-1.0.1.tar.gz` & `tmp/TMDBTraktSyncer-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TMDBTraktSyncer-1.0.1.tar", last modified: Thu May 18 02:29:57 2023, max compression
+gzip compressed data, was "TMDBTraktSyncer-1.0.2.tar", last modified: Thu May 18 21:10:30 2023, max compression
```

## Comparing `TMDBTraktSyncer-1.0.1.tar` & `TMDBTraktSyncer-1.0.2.tar`

### file list

```diff
@@ -1,20 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-05-18 02:29:57.382074 TMDBTraktSyncer-1.0.1/
--rw-rw-rw-   0        0        0     1079 2023-04-26 18:19:27.000000 TMDBTraktSyncer-1.0.1/LICENSE
--rw-rw-rw-   0        0        0     5905 2023-05-18 02:29:57.382074 TMDBTraktSyncer-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     5282 2023-05-18 02:27:35.000000 TMDBTraktSyncer-1.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-05-18 02:29:57.350601 TMDBTraktSyncer-1.0.1/TMDBTraktSyncer/
--rw-rw-rw-   0        0        0     6373 2023-05-18 02:25:14.000000 TMDBTraktSyncer-1.0.1/TMDBTraktSyncer/TMDBTraktSyncer.py
--rw-rw-rw-   0        0        0        0 2023-04-29 22:05:24.000000 TMDBTraktSyncer-1.0.1/TMDBTraktSyncer/__init__.py
--rw-rw-rw-   0        0        0     1805 2023-05-18 02:25:14.000000 TMDBTraktSyncer-1.0.1/TMDBTraktSyncer/authTrakt.py
--rw-rw-rw-   0        0        0     2997 2023-05-18 02:25:14.000000 TMDBTraktSyncer-1.0.1/TMDBTraktSyncer/tmdbRatings.py
--rw-rw-rw-   0        0        0     2181 2023-05-18 02:25:14.000000 TMDBTraktSyncer-1.0.1/TMDBTraktSyncer/traktRatings.py
--rw-rw-rw-   0        0        0     1822 2023-05-18 02:26:48.000000 TMDBTraktSyncer-1.0.1/TMDBTraktSyncer/verifyCredentials.py
-drwxrwxrwx   0        0        0        0 2023-05-18 02:29:57.380072 TMDBTraktSyncer-1.0.1/TMDBTraktSyncer.egg-info/
--rw-rw-rw-   0        0        0     5905 2023-05-18 02:29:57.000000 TMDBTraktSyncer-1.0.1/TMDBTraktSyncer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      454 2023-05-18 02:29:57.000000 TMDBTraktSyncer-1.0.1/TMDBTraktSyncer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-18 02:29:57.000000 TMDBTraktSyncer-1.0.1/TMDBTraktSyncer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       73 2023-05-18 02:29:57.000000 TMDBTraktSyncer-1.0.1/TMDBTraktSyncer.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        9 2023-05-18 02:29:57.000000 TMDBTraktSyncer-1.0.1/TMDBTraktSyncer.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-05-18 02:29:57.000000 TMDBTraktSyncer-1.0.1/TMDBTraktSyncer.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-18 02:29:57.383074 TMDBTraktSyncer-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1261 2023-05-18 02:28:20.000000 TMDBTraktSyncer-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-18 21:10:30.810891 TMDBTraktSyncer-1.0.2/
+-rw-rw-rw-   0        0        0     1079 2023-04-26 18:19:27.000000 TMDBTraktSyncer-1.0.2/LICENSE
+-rw-rw-rw-   0        0        0     6444 2023-05-18 21:10:30.809886 TMDBTraktSyncer-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     5795 2023-05-18 21:09:58.000000 TMDBTraktSyncer-1.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-05-18 21:10:30.779877 TMDBTraktSyncer-1.0.2/TMDBTraktSyncer/
+-rw-rw-rw-   0        0        0     7096 2023-05-18 21:08:07.000000 TMDBTraktSyncer-1.0.2/TMDBTraktSyncer/TMDBTraktSyncer.py
+-rw-rw-rw-   0        0        0        0 2023-04-29 22:05:24.000000 TMDBTraktSyncer-1.0.2/TMDBTraktSyncer/__init__.py
+-rw-rw-rw-   0        0        0     1805 2023-05-18 21:06:55.000000 TMDBTraktSyncer-1.0.2/TMDBTraktSyncer/authTrakt.py
+-rw-rw-rw-   0        0        0      464 2023-05-18 21:07:12.000000 TMDBTraktSyncer-1.0.2/TMDBTraktSyncer/errorHandling.py
+-rw-rw-rw-   0        0        0     2997 2023-05-18 21:06:57.000000 TMDBTraktSyncer-1.0.2/TMDBTraktSyncer/tmdbRatings.py
+-rw-rw-rw-   0        0        0     2181 2023-05-18 21:06:45.000000 TMDBTraktSyncer-1.0.2/TMDBTraktSyncer/traktRatings.py
+-rw-rw-rw-   0        0        0     1822 2023-05-18 21:06:52.000000 TMDBTraktSyncer-1.0.2/TMDBTraktSyncer/verifyCredentials.py
+drwxrwxrwx   0        0        0        0 2023-05-18 21:10:30.807886 TMDBTraktSyncer-1.0.2/TMDBTraktSyncer.egg-info/
+-rw-rw-rw-   0        0        0     6444 2023-05-18 21:10:30.000000 TMDBTraktSyncer-1.0.2/TMDBTraktSyncer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      487 2023-05-18 21:10:30.000000 TMDBTraktSyncer-1.0.2/TMDBTraktSyncer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-18 21:10:30.000000 TMDBTraktSyncer-1.0.2/TMDBTraktSyncer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       73 2023-05-18 21:10:30.000000 TMDBTraktSyncer-1.0.2/TMDBTraktSyncer.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        9 2023-05-18 21:10:30.000000 TMDBTraktSyncer-1.0.2/TMDBTraktSyncer.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-05-18 21:10:30.000000 TMDBTraktSyncer-1.0.2/TMDBTraktSyncer.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-18 21:10:30.810891 TMDBTraktSyncer-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1261 2023-05-18 21:09:01.000000 TMDBTraktSyncer-1.0.2/setup.py
```

### Comparing `TMDBTraktSyncer-1.0.1/LICENSE` & `TMDBTraktSyncer-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `TMDBTraktSyncer-1.0.1/PKG-INFO` & `TMDBTraktSyncer-1.0.2/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,70 +1,96 @@
 Metadata-Version: 2.1
 Name: TMDBTraktSyncer
-Version: 1.0.1
+Version: 1.0.2
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
-This python script will sync user ratings for Movies and TV Shows and episodes both ways between [Trakt](https://trakt.tv/dashboard) and [TMDB](https://www.themoviedb.org/). Ratings already set will not be overwritten. This script should work on an OS where python is supported (Windows, Linux, Mac, ChromeOS, etc). If you're looking to sync your ratings between Trakt, Plex, IMDB, and TMDB then these are my recommended projects: [PlexTraktSync](https://github.com/Taxel/PlexTraktSync), [IMDb-Trakt-Syncer](https://github.com/RileyXX/IMDb-Trakt-Syncer) & [TMDB-Trakt-Syncer](https://github.com/RileyXX/TMDB-Trakt-Syncer).
-## Install Instructions:
-1. Install [Python](https://www.python.org/downloads/). 
-2. Run `python -m pip install TMDBTraktSyncer` in command line.
-3. Login to [Trakt](https://trakt.tv/oauth/applications) and create a new API application. We will name it `TMDbTraktSyncer`. In the Redirect uri field enter `urn:ietf:wg:oauth:2.0:oob` then Save. 
-4. Login to [TMDB](https://www.themoviedb.org/settings/api/) and create a new API application. Choose developer, accept the terms and start filling out the application form. For type of use `Personal`. For application name we will call it `TMDB-Trakt-Sync`. For application url enter `localhost`. For application summary enter `Use TMDB api and Trakt api to sync user ratings between platforms. https://github.com/RileyXX/TMDB-Trakt-Syncer`. Fill in the rest of the fields with whatever you want and submit. Your api keys will be instantly generated.
-5. Run the script by calling `TMDBTraktSyncer` in command line. 
-6. Follow the prompts on first run. It will ask you to fill in your Trakt client id and client secret from step 3. It will also ask you to fill in your tmdb_v4_token from step 4. Please note that these details are saved insecurely as credentials.txt in the same folder as the script.
-7. Done, setup complete. The script will continue to run and sync your ratings. This may take some time, you can follow its progress in the command line.
-
-## Run:
-`TMDBTraktSyncer` in command line.
-
-## Update:
-`python -m pip install TMDBTraktSyncer --upgrade` in command line.
-
-## Uninstall:
-`python -m pip uninstall TMDBTraktSyncer` in command line.
-
-## Install specific version:
-`python -m pip install TMDBTraktSyncer==VERSION_NUMBER` in command line. Replace `VERSION_NUMBER` with your [desired version](https://github.com/RileyXX/TMDb-Trakt-Syncer/releases).
-
-## Alternative manual no pip install method:
-1. Install [Python](https://www.python.org/downloads/).
-2. Download the latest .zip from the [releases page](https://github.com/RileyXX/TMDB-Trakt-Syncer/releases) and extract it to the file directory of your choice.
-3. Login to [Trakt](https://trakt.tv/oauth/applications) and create a new API application. We will name it `TMDBTraktSyncer`. In the Redirect uri field enter `urn:ietf:wg:oauth:2.0:oob` then Save. 
-4. Login to [TMDB](https://www.themoviedb.org/settings/api/) and create a new API application. Choose developer, accept the terms and start filling out the application form. For type of use `Personal`. For application name we will call it `TMDB-Trakt-Sync`. For application url enter `localhost`. For application summary enter `Use TMDB api and Trakt api to sync user ratings between platforms. https://github.com/RileyXX/TMDB-Trakt-Syncer`. Fill in the rest of the fields with whatever you want and submit. Your api keys will be instantly generated.
-5. Run `TMDBTraktSyncer.py` OR open terminal and navigate to folder where `TMDBTraktSyncer.py` is located. Run `TMDBTraktSyncer.py` in terminal. 
-6. Follow the prompts on first run. It will ask you to fill in your Trakt client id and client secret from step 3. It will also ask you to fill in your tmdb_v4_token from step 4. Please note that these details are saved insecurely as credentials.txt in the same folder as the script. 
-7. Done. The script will continue to run and sync your ratings. This may take some time, you can follow its progress in the command line.
-
-## Troubleshooting, known issues, workarounds & future outlook:
-* Add support for review/comment sync https://github.com/RileyXX/TMDB-Trakt-Syncer/issues/1
-* If any of your details change, passwords, logins, api keys etc, just delete credentials.txt and that will reset the script. It will prompt you to enter your new details on next run.
+
+This Python script syncs user ratings for Movies, TV Shows, and Episodes both ways between [Trakt](https://trakt.tv/) and [TMDB](https://www.themoviedb.org/). Ratings already set will not be overwritten. The script is compatible on any operating system that supports Python v3.6 or later, including Windows, Linux, Mac, and ChromeOS. If you're interested in syncing ratings between Trakt, Plex, IMDB, and TMDB, I recommend the following projects: [PlexTraktSync](https://github.com/Taxel/PlexTraktSync), [IMDB-Trakt-Syncer](https://github.com/RileyXX/IMDB-Trakt-Syncer), and [TMDB-Trakt-Syncer](https://github.com/RileyXX/TMDB-Trakt-Syncer).
+
+## Installation Instructions:
+1. Install [Python](https://www.python.org/downloads/) (v3.6 or later).
+2. Install the script by running `python -m pip install TMDBTraktSyncer` in command line.
+3. Login to [Trakt](https://trakt.tv/oauth/applications) and create a new API application named `TMDbTraktSyncer`. In the "Redirect uri" field, enter `urn:ietf:wg:oauth:2.0:oob`, then save the application.
+4. Login to [TMDB](https://www.themoviedb.org/settings/api/) and create a new API application. Choose "Developer" and accept the terms. Fill out the application form as follows: 
+   - Type of use: `Personal`
+   - Application name: `TMDB-Trakt-Sync`
+   - Application URL: `localhost`
+   - Application summary: `Use TMDB API and Trakt API to sync user ratings between platforms. https://github.com/RileyXX/TMDB-Trakt-Syncer`
+   - Fill in the rest of the fields as desired and submit the form. Your API keys will be generated instantly.
+5. Run the script by running `TMDBTraktSyncer` in the command line.
+6. Follow the prompts during the first run. You will need to enter your Trakt client ID and client secret from step 3, as well as your `tmdb_v4_token` from step 4. Please note that these details are saved insecurely as `credentials.txt` in the same folder as the script.
+7. Setup is complete. The script will continue running and syncing your ratings. You can monitor its progress in the command line.
+
+## Installing the Script:
+```
+python -m pip install TMDBTraktSyncer
+```
+_Run in your operating system's native command line._
+## Running the Script:
+```
+TMDBTraktSyncer
+```
+_Run in your operating system's native command line._
+## Updating the Script:
+```
+python -m pip install TMDBTraktSyncer --upgrade
+```
+_Run in your operating system's native command line._
+## Uninstalling the Script:
+```
+python -m pip uninstall TMDBTraktSyncer
+```
+_Run in your operating system's native command line._
+
+## Installing a Specific Version:
+```
+python -m pip install TMDBTraktSyncer==VERSION_NUMBER
+```
+_Replace `VERSION_NUMBER` with your [desired version](https://github.com/RileyXX/TMDB-Trakt-Syncer/releases) (e.g. 1.0.1) and run in your operating system's native command line._
+
+## Alternative Manual Installation Method (without pip install):
+1. Install [Python](https://www.python.org/downloads/) (v3.6 or later).
+2. Download the latest .zip from the [releases page](https://github.com/RileyXX/TMDB-Trakt-Syncer/releases) and extract it to the desired directory.
+3. Login to [Trakt](https://trakt.tv/oauth/applications) and create a new API application named `TMDBTraktSyncer`. In the "Redirect uri" field, enter `urn:ietf:wg:oauth:2.0:oob`, then save the application.
+4. Login to [TMDB](https://www.themoviedb.org/settings/api/) and create a new API application. Choose "Developer" and accept the terms. Fill out the application form as follows: 
+   - Type of use: `Personal`
+   - Application name: `TMDB-Trakt-Sync`
+   - Application URL: `localhost`
+   - Application summary: `Use TMDB API and Trakt API to sync user ratings between platforms. https://github.com/RileyXX/TMDB-Trakt-Syncer`
+   - Fill in the rest of the fields as desired and submit the form. Your API keys will be generated instantly.
+5. Run `TMDBTraktSyncer.py` or open the terminal and navigate to the folder where `TMDBTraktSyncer.py` is located, then run `TMDBTraktSyncer.py` in the terminal.
+6. Follow the prompts during the first run. You will need to enter your Trakt client ID and client secret from step 3, as well as your `tmdb_v4_token` from step 4. Please note that these details are saved insecurely as `credentials.txt` in the same folder as the script.
+7. Setup is complete. The script will continue running and syncing your ratings. You can monitor its progress in the command line.
+
+## Troubleshooting, Known Issues, Workarounds & Future Outlook:
+* Add support for review/comment sync [Issue #1](https://github.com/RileyXX/TMDB-Trakt-Syncer/issues/1)
+* If any of your details change (passwords, logins, API keys, etc.), simply open `credentials.txt`, modify your details, save it and then run the script again. Alternatively, delete `credentials.txt` to reset the script and it will prompt you to enter your new details on the next run.
 
 ## Screenshot:
 ![Demo](https://i.imgur.com/5LI04O2.png)
 
+## Sponsorships, Donations, and Custom Projects:
+If you find my scripts helpful, you can become a [sponsor](https://github.com/sponsors/RileyXX) and support my projects! If you need help with a project, open an issue, and I'll do my best to assist you. For other inquiries and custom projects, you can contact me on [Twitter](https://twitter.com/RileyxBell).
 
-## Sponsorships, Donations and Custom Projects:
-Like my scripts? Become a [sponsor](https://github.com/sponsors/RileyXX) and support my projects! See below for other donation options. Need help with a project? Open an issue and I will try my best to help! For other inquiries and custom projects contact me on [Twitter](https://twitter.com/RileyxBell).
-
-#### More donation options:
+#### More Donation Options:
 - Cashapp: `$rileyxx`
 - Venmo: `@rileyxx`
 - Bitcoin: `bc1qrjevwqv49z8y77len3azqfghxrjmrjvhy5zqau`
 - Amazon Wishlist: [Link ↗](https://www.amazon.com/hz/wishlist/ls/WURF5NWZ843U)
 
-## Also posted on:
+## Also Posted on:
 * [PyPi](https://pypi.org/project/TMDBTraktSyncer/)
 * [Reddit](https://www.reddit.com/r/trakt/comments/13jlu4r/tmdb_trakt_rating_syncer_tool_2_way_sync/)
 
 <br>
 
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
```

### Comparing `TMDBTraktSyncer-1.0.1/README.md` & `TMDBTraktSyncer-1.0.2/TMDBTraktSyncer.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,56 +1,96 @@
-# TMDB-Trakt-Syncer
-This python script will sync user ratings for Movies and TV Shows and episodes both ways between [Trakt](https://trakt.tv/dashboard) and [TMDB](https://www.themoviedb.org/). Ratings already set will not be overwritten. This script should work on an OS where python is supported (Windows, Linux, Mac, ChromeOS, etc). If you're looking to sync your ratings between Trakt, Plex, IMDB, and TMDB then these are my recommended projects: [PlexTraktSync](https://github.com/Taxel/PlexTraktSync), [IMDb-Trakt-Syncer](https://github.com/RileyXX/IMDb-Trakt-Syncer) & [TMDB-Trakt-Syncer](https://github.com/RileyXX/TMDB-Trakt-Syncer).
-## Install Instructions:
-1. Install [Python](https://www.python.org/downloads/). 
-2. Run `python -m pip install TMDBTraktSyncer` in command line.
-3. Login to [Trakt](https://trakt.tv/oauth/applications) and create a new API application. We will name it `TMDbTraktSyncer`. In the Redirect uri field enter `urn:ietf:wg:oauth:2.0:oob` then Save. 
-4. Login to [TMDB](https://www.themoviedb.org/settings/api/) and create a new API application. Choose developer, accept the terms and start filling out the application form. For type of use `Personal`. For application name we will call it `TMDB-Trakt-Sync`. For application url enter `localhost`. For application summary enter `Use TMDB api and Trakt api to sync user ratings between platforms. https://github.com/RileyXX/TMDB-Trakt-Syncer`. Fill in the rest of the fields with whatever you want and submit. Your api keys will be instantly generated.
-5. Run the script by calling `TMDBTraktSyncer` in command line. 
-6. Follow the prompts on first run. It will ask you to fill in your Trakt client id and client secret from step 3. It will also ask you to fill in your tmdb_v4_token from step 4. Please note that these details are saved insecurely as credentials.txt in the same folder as the script.
-7. Done, setup complete. The script will continue to run and sync your ratings. This may take some time, you can follow its progress in the command line.
-
-## Run:
-`TMDBTraktSyncer` in command line.
-
-## Update:
-`python -m pip install TMDBTraktSyncer --upgrade` in command line.
-
-## Uninstall:
-`python -m pip uninstall TMDBTraktSyncer` in command line.
-
-## Install specific version:
-`python -m pip install TMDBTraktSyncer==VERSION_NUMBER` in command line. Replace `VERSION_NUMBER` with your [desired version](https://github.com/RileyXX/TMDb-Trakt-Syncer/releases).
-
-## Alternative manual no pip install method:
-1. Install [Python](https://www.python.org/downloads/).
-2. Download the latest .zip from the [releases page](https://github.com/RileyXX/TMDB-Trakt-Syncer/releases) and extract it to the file directory of your choice.
-3. Login to [Trakt](https://trakt.tv/oauth/applications) and create a new API application. We will name it `TMDBTraktSyncer`. In the Redirect uri field enter `urn:ietf:wg:oauth:2.0:oob` then Save. 
-4. Login to [TMDB](https://www.themoviedb.org/settings/api/) and create a new API application. Choose developer, accept the terms and start filling out the application form. For type of use `Personal`. For application name we will call it `TMDB-Trakt-Sync`. For application url enter `localhost`. For application summary enter `Use TMDB api and Trakt api to sync user ratings between platforms. https://github.com/RileyXX/TMDB-Trakt-Syncer`. Fill in the rest of the fields with whatever you want and submit. Your api keys will be instantly generated.
-5. Run `TMDBTraktSyncer.py` OR open terminal and navigate to folder where `TMDBTraktSyncer.py` is located. Run `TMDBTraktSyncer.py` in terminal. 
-6. Follow the prompts on first run. It will ask you to fill in your Trakt client id and client secret from step 3. It will also ask you to fill in your tmdb_v4_token from step 4. Please note that these details are saved insecurely as credentials.txt in the same folder as the script. 
-7. Done. The script will continue to run and sync your ratings. This may take some time, you can follow its progress in the command line.
-
-## Troubleshooting, known issues, workarounds & future outlook:
-* Add support for review/comment sync https://github.com/RileyXX/TMDB-Trakt-Syncer/issues/1
-* If any of your details change, passwords, logins, api keys etc, just delete credentials.txt and that will reset the script. It will prompt you to enter your new details on next run.
-
-## Screenshot:
-![Demo](https://i.imgur.com/5LI04O2.png)
-
-
-## Sponsorships, Donations and Custom Projects:
-Like my scripts? Become a [sponsor](https://github.com/sponsors/RileyXX) and support my projects! See below for other donation options. Need help with a project? Open an issue and I will try my best to help! For other inquiries and custom projects contact me on [Twitter](https://twitter.com/RileyxBell).
-
-#### More donation options:
-- Cashapp: `$rileyxx`
-- Venmo: `@rileyxx`
-- Bitcoin: `bc1qrjevwqv49z8y77len3azqfghxrjmrjvhy5zqau`
-- Amazon Wishlist: [Link ↗](https://www.amazon.com/hz/wishlist/ls/WURF5NWZ843U)
-
-## Also posted on:
-* [PyPi](https://pypi.org/project/TMDBTraktSyncer/)
-* [Reddit](https://www.reddit.com/r/trakt/comments/13jlu4r/tmdb_trakt_rating_syncer_tool_2_way_sync/)
-
-<br>
-
-[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
+Metadata-Version: 2.1
+Name: TMDBTraktSyncer
+Version: 1.0.2
+Summary: This python script will sync user ratings for Movies and TV Shows both ways between Trakt and TMDB.
+Home-page: https://github.com/RileyXX/TMDB-Trakt-Syncer
+Keywords: python,video,trakt,tmdb,ratings,sync,movies,tv shows
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: End Users/Desktop
+Classifier: Programming Language :: Python :: 3
+Classifier: Operating System :: OS Independent
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+
+# TMDB-Trakt-Syncer
+
+This Python script syncs user ratings for Movies, TV Shows, and Episodes both ways between [Trakt](https://trakt.tv/) and [TMDB](https://www.themoviedb.org/). Ratings already set will not be overwritten. The script is compatible on any operating system that supports Python v3.6 or later, including Windows, Linux, Mac, and ChromeOS. If you're interested in syncing ratings between Trakt, Plex, IMDB, and TMDB, I recommend the following projects: [PlexTraktSync](https://github.com/Taxel/PlexTraktSync), [IMDB-Trakt-Syncer](https://github.com/RileyXX/IMDB-Trakt-Syncer), and [TMDB-Trakt-Syncer](https://github.com/RileyXX/TMDB-Trakt-Syncer).
+
+## Installation Instructions:
+1. Install [Python](https://www.python.org/downloads/) (v3.6 or later).
+2. Install the script by running `python -m pip install TMDBTraktSyncer` in command line.
+3. Login to [Trakt](https://trakt.tv/oauth/applications) and create a new API application named `TMDbTraktSyncer`. In the "Redirect uri" field, enter `urn:ietf:wg:oauth:2.0:oob`, then save the application.
+4. Login to [TMDB](https://www.themoviedb.org/settings/api/) and create a new API application. Choose "Developer" and accept the terms. Fill out the application form as follows: 
+   - Type of use: `Personal`
+   - Application name: `TMDB-Trakt-Sync`
+   - Application URL: `localhost`
+   - Application summary: `Use TMDB API and Trakt API to sync user ratings between platforms. https://github.com/RileyXX/TMDB-Trakt-Syncer`
+   - Fill in the rest of the fields as desired and submit the form. Your API keys will be generated instantly.
+5. Run the script by running `TMDBTraktSyncer` in the command line.
+6. Follow the prompts during the first run. You will need to enter your Trakt client ID and client secret from step 3, as well as your `tmdb_v4_token` from step 4. Please note that these details are saved insecurely as `credentials.txt` in the same folder as the script.
+7. Setup is complete. The script will continue running and syncing your ratings. You can monitor its progress in the command line.
+
+## Installing the Script:
+```
+python -m pip install TMDBTraktSyncer
+```
+_Run in your operating system's native command line._
+## Running the Script:
+```
+TMDBTraktSyncer
+```
+_Run in your operating system's native command line._
+## Updating the Script:
+```
+python -m pip install TMDBTraktSyncer --upgrade
+```
+_Run in your operating system's native command line._
+## Uninstalling the Script:
+```
+python -m pip uninstall TMDBTraktSyncer
+```
+_Run in your operating system's native command line._
+
+## Installing a Specific Version:
+```
+python -m pip install TMDBTraktSyncer==VERSION_NUMBER
+```
+_Replace `VERSION_NUMBER` with your [desired version](https://github.com/RileyXX/TMDB-Trakt-Syncer/releases) (e.g. 1.0.1) and run in your operating system's native command line._
+
+## Alternative Manual Installation Method (without pip install):
+1. Install [Python](https://www.python.org/downloads/) (v3.6 or later).
+2. Download the latest .zip from the [releases page](https://github.com/RileyXX/TMDB-Trakt-Syncer/releases) and extract it to the desired directory.
+3. Login to [Trakt](https://trakt.tv/oauth/applications) and create a new API application named `TMDBTraktSyncer`. In the "Redirect uri" field, enter `urn:ietf:wg:oauth:2.0:oob`, then save the application.
+4. Login to [TMDB](https://www.themoviedb.org/settings/api/) and create a new API application. Choose "Developer" and accept the terms. Fill out the application form as follows: 
+   - Type of use: `Personal`
+   - Application name: `TMDB-Trakt-Sync`
+   - Application URL: `localhost`
+   - Application summary: `Use TMDB API and Trakt API to sync user ratings between platforms. https://github.com/RileyXX/TMDB-Trakt-Syncer`
+   - Fill in the rest of the fields as desired and submit the form. Your API keys will be generated instantly.
+5. Run `TMDBTraktSyncer.py` or open the terminal and navigate to the folder where `TMDBTraktSyncer.py` is located, then run `TMDBTraktSyncer.py` in the terminal.
+6. Follow the prompts during the first run. You will need to enter your Trakt client ID and client secret from step 3, as well as your `tmdb_v4_token` from step 4. Please note that these details are saved insecurely as `credentials.txt` in the same folder as the script.
+7. Setup is complete. The script will continue running and syncing your ratings. You can monitor its progress in the command line.
+
+## Troubleshooting, Known Issues, Workarounds & Future Outlook:
+* Add support for review/comment sync [Issue #1](https://github.com/RileyXX/TMDB-Trakt-Syncer/issues/1)
+* If any of your details change (passwords, logins, API keys, etc.), simply open `credentials.txt`, modify your details, save it and then run the script again. Alternatively, delete `credentials.txt` to reset the script and it will prompt you to enter your new details on the next run.
+
+## Screenshot:
+![Demo](https://i.imgur.com/5LI04O2.png)
+
+## Sponsorships, Donations, and Custom Projects:
+If you find my scripts helpful, you can become a [sponsor](https://github.com/sponsors/RileyXX) and support my projects! If you need help with a project, open an issue, and I'll do my best to assist you. For other inquiries and custom projects, you can contact me on [Twitter](https://twitter.com/RileyxBell).
+
+#### More Donation Options:
+- Cashapp: `$rileyxx`
+- Venmo: `@rileyxx`
+- Bitcoin: `bc1qrjevwqv49z8y77len3azqfghxrjmrjvhy5zqau`
+- Amazon Wishlist: [Link ↗](https://www.amazon.com/hz/wishlist/ls/WURF5NWZ843U)
+
+## Also Posted on:
+* [PyPi](https://pypi.org/project/TMDBTraktSyncer/)
+* [Reddit](https://www.reddit.com/r/trakt/comments/13jlu4r/tmdb_trakt_rating_syncer_tool_2_way_sync/)
+
+<br>
+
+[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
```

### Comparing `TMDBTraktSyncer-1.0.1/TMDBTraktSyncer/TMDBTraktSyncer.py` & `TMDBTraktSyncer-1.0.2/TMDBTraktSyncer/TMDBTraktSyncer.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,153 +1,160 @@
 import json
 import requests
 import time
 try:
     from TMDBTraktSyncer import verifyCredentials
     from TMDBTraktSyncer import traktRatings
     from TMDBTraktSyncer import tmdbRatings
+    from TMDBTraktSyncer import errorHandling
 except:
     import verifyCredentials
     import traktRatings
     import tmdbRatings
+    import errorHandling
 
 
 def main():
+    try:
 
-    #Get credentials
-    trakt_client_id = verifyCredentials.trakt_client_id
-    trakt_client_secret = verifyCredentials.trakt_client_secret
-    trakt_access_token = verifyCredentials.trakt_access_token
-    tmdb_v4_token = verifyCredentials.tmdb_v4_token
-        
-    trakt_ratings = traktRatings.getTraktRatings(trakt_client_id, trakt_access_token)
-    tmdb_ratings = tmdbRatings.getTMDBRatings(tmdb_v4_token)
-
-    #Get trakt and tmdb ratings and filter out trakt ratings with missing tmdb id
-    trakt_ratings = [rating for rating in trakt_ratings if rating['ID'] is not None]
-    tmdb_ratings = [rating for rating in tmdb_ratings if rating['ID'] is not None]
-    #Filter out ratings already set
-    tmdb_ratings_to_set = [rating for rating in trakt_ratings if rating['ID'] not in [tmdb_rating['ID'] for tmdb_rating in tmdb_ratings]]
-    trakt_ratings_to_set = [rating for rating in tmdb_ratings if rating['ID'] not in [trakt_rating['ID'] for trakt_rating in trakt_ratings]]
-
-    if tmdb_ratings_to_set:
-        print('Setting TMDB Ratings')
-        
-        # Count the total number of items to rate
-        num_items = len(tmdb_ratings_to_set)
-        item_count = 0
-        
-        # Set TMDB Rating
-        for item in tmdb_ratings_to_set:
-            item_count += 1
+        #Get credentials
+        trakt_client_id = verifyCredentials.trakt_client_id
+        trakt_client_secret = verifyCredentials.trakt_client_secret
+        trakt_access_token = verifyCredentials.trakt_access_token
+        tmdb_v4_token = verifyCredentials.tmdb_v4_token
+            
+        trakt_ratings = traktRatings.getTraktRatings(trakt_client_id, trakt_access_token)
+        tmdb_ratings = tmdbRatings.getTMDBRatings(tmdb_v4_token)
+
+        #Get trakt and tmdb ratings and filter out trakt ratings with missing tmdb id
+        trakt_ratings = [rating for rating in trak_tratings if rating['ID'] is not None]
+        tmdb_ratings = [rating for rating in tmdb_ratings if rating['ID'] is not None]
+        #Filter out ratings already set
+        tmdb_ratings_to_set = [rating for rating in trakt_ratings if rating['ID'] not in [tmdb_rating['ID'] for tmdb_rating in tmdb_ratings]]
+        trakt_ratings_to_set = [rating for rating in tmdb_ratings if rating['ID'] not in [trakt_rating['ID'] for trakt_rating in trakt_ratings]]
+
+        if tmdb_ratings_to_set:
+            print('Setting TMDB Ratings')
+            
+            # Count the total number of items to rate
+            num_items = len(tmdb_ratings_to_set)
+            item_count = 0
+            
+            # Set TMDB Rating
+            for item in tmdb_ratings_to_set:
+                item_count += 1
+
+                headers = {
+                    'accept': 'application/json',
+                    'Content-Type': 'application/json;charset=utf-8',
+                    'Authorization': f'Bearer {tmdb_v4_token}'
+                }
+                if item['Type'] == 'movie':
+                    payload = {
+                        'value': item['Rating']
+                    }
+                    url = f"https://api.themoviedb.org/3/movie/{item['ID']}/rating"
+                    print(f"Rating movie ({item_count} of {num_items}): {item['Title']} ({item['Year']}): {item['Rating']}/10 on TMDB")
+
+                elif item['Type'] == 'show':
+                    payload = {
+                        'value': item['Rating']
+                    }
+                    url = f"https://api.themoviedb.org/3/tv/{item['ID']}/rating"
+                    print(f"Rating TV show ({item_count} of {num_items}): {item['Title']} ({item['Year']}): {item['Rating']}/10 on TMDB")
+
+                elif item['Type'] == 'episode':
+                    payload = {
+                        'value': item['Rating']
+                    }
+                    url = f"https://api.themoviedb.org/3/tv/{item['ShowID']}/season/{item['Season']}/episode/{item['Episode']}/rating"
+                    print(f"Rating episode ({item_count} of {num_items}): {item['Title']} ({item['Year']}) [S{item['Season']:02d}E{item['Episode']:02d}]: {item['Rating']}/10 on TMDB")
 
-            headers = {
-                'accept': 'application/json',
-                'Content-Type': 'application/json;charset=utf-8',
-                'Authorization': f'Bearer {tmdb_v4_token}'
-            }
-            if item['Type'] == 'movie':
-                payload = {
-                    'value': item['Rating']
-                }
-                url = f"https://api.themoviedb.org/3/movie/{item['ID']}/rating"
-                print(f"Rating movie ({item_count} of {num_items}): {item['Title']} ({item['Year']}): {item['Rating']}/10 on TMDB")
-
-            elif item['Type'] == 'show':
-                payload = {
-                    'value': item['Rating']
-                }
-                url = f"https://api.themoviedb.org/3/tv/{item['ID']}/rating"
-                print(f"Rating TV show ({item_count} of {num_items}): {item['Title']} ({item['Year']}): {item['Rating']}/10 on TMDB")
-
-            elif item['Type'] == 'episode':
-                payload = {
-                    'value': item['Rating']
-                }
-                url = f"https://api.themoviedb.org/3/tv/{item['ShowID']}/season/{item['Season']}/episode/{item['Episode']}/rating"
-                print(f"Rating episode ({item_count} of {num_items}): {item['Title']} ({item['Year']}) [S{item['Season']:02d}E{item['Episode']:02d}]: {item['Rating']}/10 on TMDB")
-
-            response = requests.post(url, headers=headers, json=payload)
-
-            while response.status_code == 429:
-                print("Rate limit exceeded. Waiting for 1 second...")
-                time.sleep(1)
                 response = requests.post(url, headers=headers, json=payload)
-            if response.status_code != 201:
-                print(f"Error rating {item}: {response.content}")
 
-        print('Setting TMDB Ratings Complete')
-    else:
-        print('No TMDB Ratings To Set')
-
-    if trakt_ratings_to_set:
-        print('Setting Trakt Ratings')
-
-        # Set the API endpoints
-        oauth_url = "https://api.trakt.tv/oauth/token"
-        rate_url = "https://api.trakt.tv/sync/ratings"
-
-        # Set the headers
-        headers = {
-            "Content-Type": "application/json",
-            "trakt-api-version": "2",
-            "trakt-api-key": trakt_client_id,
-            "Authorization": f"Bearer {trakt_access_token}"
-        }
-        
-        # Count the total number of items to rate
-        num_items = len(trakt_ratings_to_set)
-        item_count = 0
-                
-        # Loop through your data table and rate each item on Trakt
-        for item in trakt_ratings_to_set:
-            item_count += 1
-            if item["Type"] == "show":
-                # This is a TV show
-                data = {
-                    "shows": [{
-                        "ids": {
-                            "tmdb": item["ID"]
-                        },
-                        "rating": item["Rating"]
-                    }]
-                }
-                print(f"Rating TV show ({item_count} of {num_items}): {item['Title']} ({item['Year']}): {item['Rating']}/10 on Trakt")
-            elif item["Type"] == "movie":
-                # This is a movie
-                data = {
-                    "movies": [{
-                        "ids": {
-                            "tmdb": item["ID"]
-                        },
-                        "rating": item["Rating"]
-                    }]
-                }
-                print(f"Rating movie ({item_count} of {num_items}): {item['Title']} ({item['Year']}): {item['Rating']}/10 on Trakt")
-            elif item["Type"] == "episode":
-                # This is an episode
-                data = {
-                    "episodes": [{
-                        "ids": {
-                            "tmdb": item["ID"]
-                        },
-                        "rating": item["Rating"]
-                    }]
-                }
-                print(f"Rating episode ({item_count} of {num_items}): {item['Title']} ({item['Year']}) [S{item['Season']:02d}E{item['Episode']:02d}]: {item['Rating']}/10 on Trakt")
+                while response.status_code == 429:
+                    print("Rate limit exceeded. Waiting for 1 second...")
+                    time.sleep(1)
+                    response = requests.post(url, headers=headers, json=payload)
+                if response.status_code != 201:
+                    print(f"Error rating {item}: {response.content}")
+
+            print('Setting TMDB Ratings Complete')
+        else:
+            print('No TMDB Ratings To Set')
+
+        if trakt_ratings_to_set:
+            print('Setting Trakt Ratings')
+
+            # Set the API endpoints
+            oauth_url = "https://api.trakt.tv/oauth/token"
+            rate_url = "https://api.trakt.tv/sync/ratings"
 
-            # Make the API call to rate the item
-            response = requests.post(rate_url, headers=headers, json=data)
-            time.sleep(1)
-            while response.status_code == 429:
-                print("Rate limit exceeded. Waiting for 1 second...")
-                time.sleep(1)
-                response = requests.post(rate_url, headers=headers, json=data)
-            if response.status_code != 201:
-                print(f"Error rating {item}: {response.content}")
+            # Set the headers
+            headers = {
+                "Content-Type": "application/json",
+                "trakt-api-version": "2",
+                "trakt-api-key": trakt_client_id,
+                "Authorization": f"Bearer {trakt_access_token}"
+            }
+            
+            # Count the total number of items to rate
+            num_items = len(trakt_ratings_to_set)
+            item_count = 0
+                    
+            # Loop through your data table and rate each item on Trakt
+            for item in trakt_ratings_to_set:
+                item_count += 1
+                if item["Type"] == "show":
+                    # This is a TV show
+                    data = {
+                        "shows": [{
+                            "ids": {
+                                "tmdb": item["ID"]
+                            },
+                            "rating": item["Rating"]
+                        }]
+                    }
+                    print(f"Rating TV show ({item_count} of {num_items}): {item['Title']} ({item['Year']}): {item['Rating']}/10 on Trakt")
+                elif item["Type"] == "movie":
+                    # This is a movie
+                    data = {
+                        "movies": [{
+                            "ids": {
+                                "tmdb": item["ID"]
+                            },
+                            "rating": item["Rating"]
+                        }]
+                    }
+                    print(f"Rating movie ({item_count} of {num_items}): {item['Title']} ({item['Year']}): {item['Rating']}/10 on Trakt")
+                elif item["Type"] == "episode":
+                    # This is an episode
+                    data = {
+                        "episodes": [{
+                            "ids": {
+                                "tmdb": item["ID"]
+                            },
+                            "rating": item["Rating"]
+                        }]
+                    }
+                    print(f"Rating episode ({item_count} of {num_items}): {item['Title']} ({item['Year']}) [S{item['Season']:02d}E{item['Episode']:02d}]: {item['Rating']}/10 on Trakt")
 
-        print('Setting Trakt Ratings Complete')
-    else:
-        print('No Trakt Ratings To Set')
+                # Make the API call to rate the item
+                response = requests.post(rate_url, headers=headers, json=data)
+                time.sleep(1)
+                while response.status_code == 429:
+                    print("Rate limit exceeded. Waiting for 1 second...")
+                    time.sleep(1)
+                    response = requests.post(rate_url, headers=headers, json=data)
+                if response.status_code != 201:
+                    print(f"Error rating {item}: {response.content}")
+
+            print('Setting Trakt Ratings Complete')
+        else:
+            print('No Trakt Ratings To Set')
+
+    except Exception as e:
+        error_message = "An error occurred while running the script."
+        errorHandling.report_error(error_message)
 
 if __name__ == '__main__':
     main()
```

### Comparing `TMDBTraktSyncer-1.0.1/TMDBTraktSyncer/authTrakt.py` & `TMDBTraktSyncer-1.0.2/TMDBTraktSyncer/authTrakt.py`

 * *Files identical despite different names*

### Comparing `TMDBTraktSyncer-1.0.1/TMDBTraktSyncer/tmdbRatings.py` & `TMDBTraktSyncer-1.0.2/TMDBTraktSyncer/tmdbRatings.py`

 * *Files identical despite different names*

### Comparing `TMDBTraktSyncer-1.0.1/TMDBTraktSyncer/traktRatings.py` & `TMDBTraktSyncer-1.0.2/TMDBTraktSyncer/traktRatings.py`

 * *Files identical despite different names*

### Comparing `TMDBTraktSyncer-1.0.1/TMDBTraktSyncer/verifyCredentials.py` & `TMDBTraktSyncer-1.0.2/TMDBTraktSyncer/verifyCredentials.py`

 * *Files identical despite different names*

### Comparing `TMDBTraktSyncer-1.0.1/TMDBTraktSyncer.egg-info/PKG-INFO` & `TMDBTraktSyncer-1.0.2/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,70 +1,82 @@
-Metadata-Version: 2.1
-Name: TMDBTraktSyncer
-Version: 1.0.1
-Summary: This python script will sync user ratings for Movies and TV Shows both ways between Trakt and TMDB.
-Home-page: https://github.com/RileyXX/TMDB-Trakt-Syncer
-Keywords: python,video,trakt,tmdb,ratings,sync,movies,tv shows
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: End Users/Desktop
-Classifier: Programming Language :: Python :: 3
-Classifier: Operating System :: OS Independent
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-
-# TMDB-Trakt-Syncer
-This python script will sync user ratings for Movies and TV Shows and episodes both ways between [Trakt](https://trakt.tv/dashboard) and [TMDB](https://www.themoviedb.org/). Ratings already set will not be overwritten. This script should work on an OS where python is supported (Windows, Linux, Mac, ChromeOS, etc). If you're looking to sync your ratings between Trakt, Plex, IMDB, and TMDB then these are my recommended projects: [PlexTraktSync](https://github.com/Taxel/PlexTraktSync), [IMDb-Trakt-Syncer](https://github.com/RileyXX/IMDb-Trakt-Syncer) & [TMDB-Trakt-Syncer](https://github.com/RileyXX/TMDB-Trakt-Syncer).
-## Install Instructions:
-1. Install [Python](https://www.python.org/downloads/). 
-2. Run `python -m pip install TMDBTraktSyncer` in command line.
-3. Login to [Trakt](https://trakt.tv/oauth/applications) and create a new API application. We will name it `TMDbTraktSyncer`. In the Redirect uri field enter `urn:ietf:wg:oauth:2.0:oob` then Save. 
-4. Login to [TMDB](https://www.themoviedb.org/settings/api/) and create a new API application. Choose developer, accept the terms and start filling out the application form. For type of use `Personal`. For application name we will call it `TMDB-Trakt-Sync`. For application url enter `localhost`. For application summary enter `Use TMDB api and Trakt api to sync user ratings between platforms. https://github.com/RileyXX/TMDB-Trakt-Syncer`. Fill in the rest of the fields with whatever you want and submit. Your api keys will be instantly generated.
-5. Run the script by calling `TMDBTraktSyncer` in command line. 
-6. Follow the prompts on first run. It will ask you to fill in your Trakt client id and client secret from step 3. It will also ask you to fill in your tmdb_v4_token from step 4. Please note that these details are saved insecurely as credentials.txt in the same folder as the script.
-7. Done, setup complete. The script will continue to run and sync your ratings. This may take some time, you can follow its progress in the command line.
-
-## Run:
-`TMDBTraktSyncer` in command line.
-
-## Update:
-`python -m pip install TMDBTraktSyncer --upgrade` in command line.
-
-## Uninstall:
-`python -m pip uninstall TMDBTraktSyncer` in command line.
-
-## Install specific version:
-`python -m pip install TMDBTraktSyncer==VERSION_NUMBER` in command line. Replace `VERSION_NUMBER` with your [desired version](https://github.com/RileyXX/TMDb-Trakt-Syncer/releases).
-
-## Alternative manual no pip install method:
-1. Install [Python](https://www.python.org/downloads/).
-2. Download the latest .zip from the [releases page](https://github.com/RileyXX/TMDB-Trakt-Syncer/releases) and extract it to the file directory of your choice.
-3. Login to [Trakt](https://trakt.tv/oauth/applications) and create a new API application. We will name it `TMDBTraktSyncer`. In the Redirect uri field enter `urn:ietf:wg:oauth:2.0:oob` then Save. 
-4. Login to [TMDB](https://www.themoviedb.org/settings/api/) and create a new API application. Choose developer, accept the terms and start filling out the application form. For type of use `Personal`. For application name we will call it `TMDB-Trakt-Sync`. For application url enter `localhost`. For application summary enter `Use TMDB api and Trakt api to sync user ratings between platforms. https://github.com/RileyXX/TMDB-Trakt-Syncer`. Fill in the rest of the fields with whatever you want and submit. Your api keys will be instantly generated.
-5. Run `TMDBTraktSyncer.py` OR open terminal and navigate to folder where `TMDBTraktSyncer.py` is located. Run `TMDBTraktSyncer.py` in terminal. 
-6. Follow the prompts on first run. It will ask you to fill in your Trakt client id and client secret from step 3. It will also ask you to fill in your tmdb_v4_token from step 4. Please note that these details are saved insecurely as credentials.txt in the same folder as the script. 
-7. Done. The script will continue to run and sync your ratings. This may take some time, you can follow its progress in the command line.
-
-## Troubleshooting, known issues, workarounds & future outlook:
-* Add support for review/comment sync https://github.com/RileyXX/TMDB-Trakt-Syncer/issues/1
-* If any of your details change, passwords, logins, api keys etc, just delete credentials.txt and that will reset the script. It will prompt you to enter your new details on next run.
-
-## Screenshot:
-![Demo](https://i.imgur.com/5LI04O2.png)
-
-
-## Sponsorships, Donations and Custom Projects:
-Like my scripts? Become a [sponsor](https://github.com/sponsors/RileyXX) and support my projects! See below for other donation options. Need help with a project? Open an issue and I will try my best to help! For other inquiries and custom projects contact me on [Twitter](https://twitter.com/RileyxBell).
-
-#### More donation options:
-- Cashapp: `$rileyxx`
-- Venmo: `@rileyxx`
-- Bitcoin: `bc1qrjevwqv49z8y77len3azqfghxrjmrjvhy5zqau`
-- Amazon Wishlist: [Link ↗](https://www.amazon.com/hz/wishlist/ls/WURF5NWZ843U)
-
-## Also posted on:
-* [PyPi](https://pypi.org/project/TMDBTraktSyncer/)
-* [Reddit](https://www.reddit.com/r/trakt/comments/13jlu4r/tmdb_trakt_rating_syncer_tool_2_way_sync/)
-
-<br>
-
-[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
+# TMDB-Trakt-Syncer
+
+This Python script syncs user ratings for Movies, TV Shows, and Episodes both ways between [Trakt](https://trakt.tv/) and [TMDB](https://www.themoviedb.org/). Ratings already set will not be overwritten. The script is compatible on any operating system that supports Python v3.6 or later, including Windows, Linux, Mac, and ChromeOS. If you're interested in syncing ratings between Trakt, Plex, IMDB, and TMDB, I recommend the following projects: [PlexTraktSync](https://github.com/Taxel/PlexTraktSync), [IMDB-Trakt-Syncer](https://github.com/RileyXX/IMDB-Trakt-Syncer), and [TMDB-Trakt-Syncer](https://github.com/RileyXX/TMDB-Trakt-Syncer).
+
+## Installation Instructions:
+1. Install [Python](https://www.python.org/downloads/) (v3.6 or later).
+2. Install the script by running `python -m pip install TMDBTraktSyncer` in command line.
+3. Login to [Trakt](https://trakt.tv/oauth/applications) and create a new API application named `TMDbTraktSyncer`. In the "Redirect uri" field, enter `urn:ietf:wg:oauth:2.0:oob`, then save the application.
+4. Login to [TMDB](https://www.themoviedb.org/settings/api/) and create a new API application. Choose "Developer" and accept the terms. Fill out the application form as follows: 
+   - Type of use: `Personal`
+   - Application name: `TMDB-Trakt-Sync`
+   - Application URL: `localhost`
+   - Application summary: `Use TMDB API and Trakt API to sync user ratings between platforms. https://github.com/RileyXX/TMDB-Trakt-Syncer`
+   - Fill in the rest of the fields as desired and submit the form. Your API keys will be generated instantly.
+5. Run the script by running `TMDBTraktSyncer` in the command line.
+6. Follow the prompts during the first run. You will need to enter your Trakt client ID and client secret from step 3, as well as your `tmdb_v4_token` from step 4. Please note that these details are saved insecurely as `credentials.txt` in the same folder as the script.
+7. Setup is complete. The script will continue running and syncing your ratings. You can monitor its progress in the command line.
+
+## Installing the Script:
+```
+python -m pip install TMDBTraktSyncer
+```
+_Run in your operating system's native command line._
+## Running the Script:
+```
+TMDBTraktSyncer
+```
+_Run in your operating system's native command line._
+## Updating the Script:
+```
+python -m pip install TMDBTraktSyncer --upgrade
+```
+_Run in your operating system's native command line._
+## Uninstalling the Script:
+```
+python -m pip uninstall TMDBTraktSyncer
+```
+_Run in your operating system's native command line._
+
+## Installing a Specific Version:
+```
+python -m pip install TMDBTraktSyncer==VERSION_NUMBER
+```
+_Replace `VERSION_NUMBER` with your [desired version](https://github.com/RileyXX/TMDB-Trakt-Syncer/releases) (e.g. 1.0.1) and run in your operating system's native command line._
+
+## Alternative Manual Installation Method (without pip install):
+1. Install [Python](https://www.python.org/downloads/) (v3.6 or later).
+2. Download the latest .zip from the [releases page](https://github.com/RileyXX/TMDB-Trakt-Syncer/releases) and extract it to the desired directory.
+3. Login to [Trakt](https://trakt.tv/oauth/applications) and create a new API application named `TMDBTraktSyncer`. In the "Redirect uri" field, enter `urn:ietf:wg:oauth:2.0:oob`, then save the application.
+4. Login to [TMDB](https://www.themoviedb.org/settings/api/) and create a new API application. Choose "Developer" and accept the terms. Fill out the application form as follows: 
+   - Type of use: `Personal`
+   - Application name: `TMDB-Trakt-Sync`
+   - Application URL: `localhost`
+   - Application summary: `Use TMDB API and Trakt API to sync user ratings between platforms. https://github.com/RileyXX/TMDB-Trakt-Syncer`
+   - Fill in the rest of the fields as desired and submit the form. Your API keys will be generated instantly.
+5. Run `TMDBTraktSyncer.py` or open the terminal and navigate to the folder where `TMDBTraktSyncer.py` is located, then run `TMDBTraktSyncer.py` in the terminal.
+6. Follow the prompts during the first run. You will need to enter your Trakt client ID and client secret from step 3, as well as your `tmdb_v4_token` from step 4. Please note that these details are saved insecurely as `credentials.txt` in the same folder as the script.
+7. Setup is complete. The script will continue running and syncing your ratings. You can monitor its progress in the command line.
+
+## Troubleshooting, Known Issues, Workarounds & Future Outlook:
+* Add support for review/comment sync [Issue #1](https://github.com/RileyXX/TMDB-Trakt-Syncer/issues/1)
+* If any of your details change (passwords, logins, API keys, etc.), simply open `credentials.txt`, modify your details, save it and then run the script again. Alternatively, delete `credentials.txt` to reset the script and it will prompt you to enter your new details on the next run.
+
+## Screenshot:
+![Demo](https://i.imgur.com/5LI04O2.png)
+
+## Sponsorships, Donations, and Custom Projects:
+If you find my scripts helpful, you can become a [sponsor](https://github.com/sponsors/RileyXX) and support my projects! If you need help with a project, open an issue, and I'll do my best to assist you. For other inquiries and custom projects, you can contact me on [Twitter](https://twitter.com/RileyxBell).
+
+#### More Donation Options:
+- Cashapp: `$rileyxx`
+- Venmo: `@rileyxx`
+- Bitcoin: `bc1qrjevwqv49z8y77len3azqfghxrjmrjvhy5zqau`
+- Amazon Wishlist: [Link ↗](https://www.amazon.com/hz/wishlist/ls/WURF5NWZ843U)
+
+## Also Posted on:
+* [PyPi](https://pypi.org/project/TMDBTraktSyncer/)
+* [Reddit](https://www.reddit.com/r/trakt/comments/13jlu4r/tmdb_trakt_rating_syncer_tool_2_way_sync/)
+
+<br>
+
+[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
```

### Comparing `TMDBTraktSyncer-1.0.1/setup.py` & `TMDBTraktSyncer-1.0.2/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 #To upload package: twine upload dist/*
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '1.0.1'
+VERSION = '1.0.2'
 DESCRIPTION = 'This python script will sync user ratings for Movies and TV Shows both ways between Trakt and TMDB.'
 
 # Setting up
 setup(
     name="TMDBTraktSyncer",
     version=VERSION,
     description=DESCRIPTION,
```

