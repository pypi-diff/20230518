# Comparing `tmp/deezer_downloader-2.0.3.tar.gz` & `tmp/deezer_downloader-2.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deezer_downloader-2.0.3.tar", max compression
+gzip compressed data, was "deezer_downloader-2.0.4.tar", max compression
```

## Comparing `deezer_downloader-2.0.3.tar` & `deezer_downloader-2.0.4.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0     1063 2023-04-09 20:20:53.021110 deezer_downloader-2.0.3/LICENSE
--rw-r--r--   0        0        0     7712 2023-04-09 20:58:29.658538 deezer_downloader-2.0.3/README.md
--rw-r--r--   0        0        0     1272 2023-04-09 20:57:18.943593 deezer_downloader-2.0.3/deezer_downloader/cli/deezer-downloader.ini.template
--rw-r--r--   0        0        0     1738 2023-04-09 20:56:59.983157 deezer_downloader-2.0.3/deezer_downloader/cli/runner.py
--rw-r--r--   0        0        0     1170 2023-04-09 20:20:53.021110 deezer_downloader-2.0.3/deezer_downloader/configuration.py
--rw-r--r--   0        0        0    20706 2023-04-09 20:20:53.021110 deezer_downloader-2.0.3/deezer_downloader/deezer.py
--rw-r--r--   0        0        0     4855 2023-04-09 20:20:53.021110 deezer_downloader-2.0.3/deezer_downloader/spotify.py
--rw-r--r--   0        0        0     3382 2023-04-09 20:20:53.021110 deezer_downloader-2.0.3/deezer_downloader/threadpool_queue.py
--rw-r--r--   0        0        0    10129 2023-04-09 20:20:53.021110 deezer_downloader-2.0.3/deezer_downloader/web/app.py
--rw-r--r--   0        0        0    10617 2023-04-09 20:20:53.021110 deezer_downloader-2.0.3/deezer_downloader/web/music_backend.py
--rw-r--r--   0        0        0   623500 2023-04-09 20:20:53.024443 deezer_downloader-2.0.3/deezer_downloader/web/static/css/bootstrap-4.1.3-dist.zip
--rw-r--r--   0        0        0    70682 2023-04-09 20:20:53.024443 deezer_downloader-2.0.3/deezer_downloader/web/static/css/bootstrap.bundle.min.js
--rw-r--r--   0        0        0   155758 2023-04-09 20:20:53.024443 deezer_downloader-2.0.3/deezer_downloader/web/static/css/bootstrap.min.css
--rw-r--r--   0        0        0    31000 2023-04-09 20:20:53.024443 deezer_downloader-2.0.3/deezer_downloader/web/static/css/font-awesome.min.css
--rw-r--r--   0        0        0     1515 2023-04-09 20:20:53.024443 deezer_downloader-2.0.3/deezer_downloader/web/static/css/jquery.jgrowl.min.css
--rw-r--r--   0        0        0      327 2023-04-09 20:20:53.024443 deezer_downloader-2.0.3/deezer_downloader/web/static/favicon.ico
--rw-r--r--   0        0        0    77160 2023-04-09 20:20:53.024443 deezer_downloader-2.0.3/deezer_downloader/web/static/fonts/fontawesome-webfont.woff2
--rw-r--r--   0        0        0    58072 2023-04-09 20:20:53.024443 deezer_downloader-2.0.3/deezer_downloader/web/static/js/bootstrap.min.js
--rw-r--r--   0        0        0    11064 2023-04-09 20:20:53.027777 deezer_downloader-2.0.3/deezer_downloader/web/static/js/custom.js
--rw-r--r--   0        0        0     5476 2023-04-09 20:20:53.027777 deezer_downloader-2.0.3/deezer_downloader/web/static/js/jquery.jgrowl.min.js
--rw-r--r--   0        0        0    89795 2023-04-09 20:20:53.027777 deezer_downloader-2.0.3/deezer_downloader/web/static/js/jquery.min.js
--rw-r--r--   0        0        0    21004 2023-04-09 20:20:53.027777 deezer_downloader-2.0.3/deezer_downloader/web/static/js/popper.min.js
--rw-r--r--   0        0        0      194 2023-04-09 20:20:53.027777 deezer_downloader-2.0.3/deezer_downloader/web/templates/autoindex.html
--rw-r--r--   0        0        0     8735 2023-04-10 10:27:40.860066 deezer_downloader-2.0.3/deezer_downloader/web/templates/index.html
--rw-r--r--   0        0        0     1856 2023-04-09 20:20:53.027777 deezer_downloader-2.0.3/deezer_downloader/youtubedl.py
--rw-r--r--   0        0        0      943 2023-04-10 10:28:46.714332 deezer_downloader-2.0.3/pyproject.toml
--rw-r--r--   0        0        0     8734 1970-01-01 00:00:00.000000 deezer_downloader-2.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1063 2023-04-09 20:20:53.021110 deezer_downloader-2.0.4/LICENSE
+-rw-r--r--   0        0        0     7743 2023-04-29 16:28:37.070565 deezer_downloader-2.0.4/README.md
+-rw-r--r--   0        0        0     1422 2023-04-10 17:50:53.352272 deezer_downloader-2.0.4/deezer_downloader/cli/deezer-downloader.ini.template
+-rw-r--r--   0        0        0     1738 2023-04-09 20:56:59.983157 deezer_downloader-2.0.4/deezer_downloader/cli/runner.py
+-rw-r--r--   0        0        0     1497 2023-05-01 07:47:26.683606 deezer_downloader-2.0.4/deezer_downloader/configuration.py
+-rw-r--r--   0        0        0    20834 2023-04-10 17:48:00.685645 deezer_downloader-2.0.4/deezer_downloader/deezer.py
+-rw-r--r--   0        0        0     5031 2023-04-29 16:38:19.755822 deezer_downloader-2.0.4/deezer_downloader/spotify.py
+-rw-r--r--   0        0        0     3382 2023-04-09 20:20:53.021110 deezer_downloader-2.0.4/deezer_downloader/threadpool_queue.py
+-rw-r--r--   0        0        0    10201 2023-04-10 17:34:44.980270 deezer_downloader-2.0.4/deezer_downloader/web/app.py
+-rw-r--r--   0        0        0    11048 2023-04-29 16:16:41.814433 deezer_downloader-2.0.4/deezer_downloader/web/music_backend.py
+-rw-r--r--   0        0        0   623500 2023-04-09 20:20:53.024443 deezer_downloader-2.0.4/deezer_downloader/web/static/css/bootstrap-4.1.3-dist.zip
+-rw-r--r--   0        0        0    70682 2023-04-09 20:20:53.024443 deezer_downloader-2.0.4/deezer_downloader/web/static/css/bootstrap.bundle.min.js
+-rw-r--r--   0        0        0   155758 2023-04-09 20:20:53.024443 deezer_downloader-2.0.4/deezer_downloader/web/static/css/bootstrap.min.css
+-rw-r--r--   0        0        0    31000 2023-04-09 20:20:53.024443 deezer_downloader-2.0.4/deezer_downloader/web/static/css/font-awesome.min.css
+-rw-r--r--   0        0        0     1515 2023-04-09 20:20:53.024443 deezer_downloader-2.0.4/deezer_downloader/web/static/css/jquery.jgrowl.min.css
+-rw-r--r--   0        0        0      327 2023-04-09 20:20:53.024443 deezer_downloader-2.0.4/deezer_downloader/web/static/favicon.ico
+-rw-r--r--   0        0        0    77160 2023-04-09 20:20:53.024443 deezer_downloader-2.0.4/deezer_downloader/web/static/fonts/fontawesome-webfont.woff2
+-rw-r--r--   0        0        0    58072 2023-04-09 20:20:53.024443 deezer_downloader-2.0.4/deezer_downloader/web/static/js/bootstrap.min.js
+-rw-r--r--   0        0        0    11064 2023-04-09 20:20:53.027777 deezer_downloader-2.0.4/deezer_downloader/web/static/js/custom.js
+-rw-r--r--   0        0        0     5476 2023-04-09 20:20:53.027777 deezer_downloader-2.0.4/deezer_downloader/web/static/js/jquery.jgrowl.min.js
+-rw-r--r--   0        0        0    89795 2023-04-09 20:20:53.027777 deezer_downloader-2.0.4/deezer_downloader/web/static/js/jquery.min.js
+-rw-r--r--   0        0        0    21004 2023-04-09 20:20:53.027777 deezer_downloader-2.0.4/deezer_downloader/web/static/js/popper.min.js
+-rw-r--r--   0        0        0      194 2023-04-09 20:20:53.027777 deezer_downloader-2.0.4/deezer_downloader/web/templates/autoindex.html
+-rw-r--r--   0        0        0     8735 2023-04-10 10:27:40.860066 deezer_downloader-2.0.4/deezer_downloader/web/templates/index.html
+-rw-r--r--   0        0        0     2309 2023-04-29 15:45:57.946045 deezer_downloader-2.0.4/deezer_downloader/youtubedl.py
+-rw-r--r--   0        0        0      977 2023-05-18 15:34:22.576711 deezer_downloader-2.0.4/pyproject.toml
+-rw-r--r--   0        0        0     8676 1970-01-01 00:00:00.000000 deezer_downloader-2.0.4/PKG-INFO
```

### Comparing `deezer_downloader-2.0.3/LICENSE` & `deezer_downloader-2.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `deezer_downloader-2.0.3/README.md` & `deezer_downloader-2.0.4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 - download Spotify playlists (by parsing the Spotify website and download the songs from Deezer)
 - download as zip file (including m3u8 playlist file)
 - 320 kbit/s mp3s with ID3-Tags and album cover (UPDATE: right now only 128bkit/s mp3 works, see #66)
 - download songs via yt-dlp
 - KISS (keep it simple and stupid) front end
 - MPD integration (use it on a Raspberry Pi!)
 - simple REST api
+- proxy support (https/socks5)
 
 
 ### How to use it
 
 There is a settings file template called `settings.ini.example`. You can specify the download directory with  `download_dir`. Pressing the download button only downloads the song/album/playlist. If you set `use_mpd=True` in the `settings.ini` the backend will connect to mpd (localhost:6600) and update the music database. Pressing the play button will download the music. If `use_mpd=True`  is set the mpd database will be updated and the song/album/playlist will be added to the playlist. In `settings.ini` `music_dir` should be the music root location of mpd. The `download_dir` must be a subdirectory of `music_dir`. 
 
 As Deezer sometimes requires a captcha to login the auto login features was removed. Instead you have to manually insert a valid Deezer cookie to the `settings.ini`. The relevant cookie is the `arl` cookie.
```

### Comparing `deezer_downloader-2.0.3/deezer_downloader/cli/deezer-downloader.ini.template` & `deezer_downloader-2.0.4/deezer_downloader/cli/deezer-downloader.ini.template`

 * *Files 17% similar despite different names*

```diff
@@ -29,14 +29,21 @@
 
 ; if used behind a proxy, specify base url prefix
 ; url_prefix = /deezer
 url_prefix = 
 api_root = %(url_prefix)s
 static_root = %(url_prefix)s/static
 
+[proxy]
+; server:
+;   - https://user:pass@host:port
+;   - socks5://127.0.0.1:9050
+;   - socks5h://127.0.0.1:9050 (DNS goes also over proxy)
+server =
+
 [threadpool]
 ; number of workers in thread pool, this specifies the maximum number of parallel downloads
 workers = 4
 
 [deezer]
 ; valid arl cookie value
 ; login manually using your web browser and take the arl ookie
```

### Comparing `deezer_downloader-2.0.3/deezer_downloader/cli/runner.py` & `deezer_downloader-2.0.4/deezer_downloader/cli/runner.py`

 * *Files identical despite different names*

### Comparing `deezer_downloader-2.0.3/deezer_downloader/deezer.py` & `deezer_downloader-2.0.4/deezer_downloader/deezer.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 TYPE_PLAYLIST = "playlist"
 TYPE_ALBUM_TRACK = "album_track" # used for listing songs of an album
 # END TYPES
 
 session = None
 
 
-def init_deezer_session():
+def init_deezer_session(proxy_server):
     global session
     header = {
         'Pragma': 'no-cache',
         'Origin': 'https://www.deezer.com',
         'Accept-Encoding': 'gzip, deflate, br',
         'Accept-Language': 'en-US,en;q=0.9',
         'User-Agent': 'Mozilla/5.0 (X11; Linux x86_64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/68.0.3440.106 Safari/537.36',
@@ -39,14 +39,17 @@
         'Connection': 'keep-alive',
         'Referer': 'https://www.deezer.com/login',
         'DNT': '1',
     }
     session = requests.session()
     session.headers.update(header)
     session.cookies.update({'arl': config['deezer']['cookie_arl'], 'comeback': '1'})
+    if len(proxy_server.strip()) > 0:
+        print(f"Using proxy {proxy_server}")
+        session.proxies.update({"https": proxy_server})
 
 
 class Deezer404Exception(Exception):
     pass
 
 
 class Deezer403Exception(Exception):
@@ -525,12 +528,10 @@
         print("Login is still working.")
         return True
     else:
         print("Login is not working anymore.")
         return False
 
 
-init_deezer_session()
-
 if __name__ == '__main__':
     if len(sys.argv) > 1 and sys.argv[1] == "check-login":
         test_deezer_login()
```

### Comparing `deezer_downloader-2.0.3/deezer_downloader/spotify.py` & `deezer_downloader-2.0.4/deezer_downloader/spotify.py`

 * *Files 5% similar despite different names*

```diff
@@ -51,52 +51,53 @@
         return {"type": parts[3], "id": parts[4]}
 
     # todo add support for other types; artists, searches, users
 
     raise SpotifyInvalidUrlException("ERROR: unable to determine Spotify URL type or type is unsupported.")
 
 
-def get_songs_from_spotify_website(playlist):
+def get_songs_from_spotify_website(playlist, proxy):
     # parses Spotify Playlist from Spotify website
     # playlist: playlist url or playlist id as string
+    # proxy: https/socks5 proxy (e. g. socks5://user:pass@127.0.0.1:1080/)
     # e.g. https://open.spotify.com/playlist/0wl9Q3oedquNlBAJ4MGZtS
     # e.g. https://open.spotify.com/embed/0wl9Q3oedquNlBAJ4MGZtS
     # e.g. 0wl9Q3oedquNlBAJ4MGZtS
     # return: list of songs (song: artist - title)
     # raises SpotifyWebsiteParserException if parsing the website goes wrong
 
     return_data = []
     url_info = parse_uri(playlist)
 
-    req = requests.get(token_url, headers=headers)
+    req = requests.get(token_url, headers=headers, proxies={"https": proxy})
     if req.status_code != 200:
         raise SpotifyWebsiteParserException(
             "ERROR: {} gave us not a 200. Instead: {}".format(token_url, req.status_code))
     token = req.json()
 
     if url_info['type'] == "playlist":
         url = playlist_base_url.format(url_info["id"])
         while True:
-            resp = get_json_from_api(url, token["accessToken"])
+            resp = get_json_from_api(url, token["accessToken"], proxy)
             for track in resp['items']:
                 return_data.append(parse_track(track["track"]))
 
             if resp['next'] is None:
                 break
             url = resp['next']
     elif url_info["type"] == "track":
-        resp = get_json_from_api(track_base_url.format(url_info["id"]), token["accessToken"])
+        resp = get_json_from_api(track_base_url.format(url_info["id"]), token["accessToken"], proxy)
         if resp is None:  # try again in case of rate limit
-            resp = get_json_from_api(track_base_url.format(url_info["id"]), token["accessToken"])
+            resp = get_json_from_api(track_base_url.format(url_info["id"]), token["accessToken"], proxy)
 
         return_data.append(parse_track(resp))
     elif url_info["type"] == "album":
-        resp = get_json_from_api(album_base_url.format(url_info["id"]), token["accessToken"])
+        resp = get_json_from_api(album_base_url.format(url_info["id"]), token["accessToken"], proxy)
         if resp is None:  # try again in case of rate limit
-            resp = get_json_from_api(album_base_url.format(url_info["id"]), token["accessToken"])
+            resp = get_json_from_api(album_base_url.format(url_info["id"]), token["accessToken"], proxy)
 
         for track in resp['items']:
             return_data.append(parse_track(track))
 
     return [track for track in return_data if track]
 
 
@@ -105,17 +106,17 @@
     song = track['name']
     full = "{} {}".format(artist, song)
     # remove everything in brackets to get better search results later on Deezer
     # e.g. (Radio  Version) or (Remastered)
     return re.sub(r'\([^)]*\)', '', full)
 
 
-def get_json_from_api(api_url, access_token):
+def get_json_from_api(api_url, access_token, proxy):
     headers.update({'Authorization': 'Bearer {}'.format(access_token)})
-    req = requests.get(api_url, headers=headers)
+    req = requests.get(api_url, headers=headers, proxies={"https": proxy})
 
     if req.status_code == 429:
         seconds = int(req.headers.get("Retry-After")) + 1
         print("INFO: rate limited! Sleeping for {} seconds".format(seconds))
         sleep(seconds)
         return None
```

### Comparing `deezer_downloader-2.0.3/deezer_downloader/threadpool_queue.py` & `deezer_downloader-2.0.4/deezer_downloader/threadpool_queue.py`

 * *Files identical despite different names*

### Comparing `deezer_downloader-2.0.3/deezer_downloader/web/app.py` & `deezer_downloader-2.0.4/deezer_downloader/web/app.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,25 +5,26 @@
 import atexit
 from flask import Flask, render_template, request, jsonify, escape
 from flask_autoindex import AutoIndex
 import giphypop
 
 from deezer_downloader.configuration import config
 from deezer_downloader.web.music_backend import sched
-from deezer_downloader.deezer import deezer_search
+from deezer_downloader.deezer import deezer_search, init_deezer_session
 
 app = Flask(__name__)
 auto_index = AutoIndex(app, config["download_dirs"]["base"], add_url_rules=False)
 auto_index.add_icon_rule('music.png', ext='m3u8')
 
 giphy = giphypop.Giphy()
 
 
 def init():
     sched.run_workers(config.getint('threadpool', 'workers'))
+    init_deezer_session(config['proxy']['server'])
 
     @atexit.register
     def stop_workers():
         sched.stop_workers()
 
 
 init()
```

### Comparing `deezer_downloader-2.0.3/deezer_downloader/web/music_backend.py` & `deezer_downloader-2.0.4/deezer_downloader/web/music_backend.py`

 * *Files 2% similar despite different names*

```diff
@@ -73,15 +73,21 @@
     else:
         array_of_special_characters = ['/', ':', '"', '?']
 
     return ''.join([c for c in path if c not in array_of_special_characters])
 
 
 def download_song_and_get_absolute_filename(search_type, song, playlist_name=None):
-    song_filename = "{} - {}.{}".format(song['ART_NAME'], song['SNG_TITLE'], 'flac' if config['deezer'].getboolean('flac_quality') else 'mp3')
+    if search_type == TYPE_ALBUM:
+        song_filename = "{:02d} - {} {}.mp3".format(int(song['TRACK_NUMBER']),
+                                                    song['ART_NAME'],
+                                                    song['SNG_TITLE'])
+    else:
+        song_filename = "{} - {}.mp3".format(song['ART_NAME'],
+                                             song['SNG_TITLE'])
     song_filename = clean_filename(song_filename)
 
     if search_type == TYPE_TRACK:
         absolute_filename = os.path.join(config["download_dirs"]["songs"], song_filename)
     elif search_type == TYPE_ALBUM:
         album_name = "{} - {}".format(song['ART_NAME'], song['ALB_TITLE'])
         album_name = clean_filename(album_name)
@@ -172,15 +178,16 @@
     if create_zip:
         return [create_zip_file(songs_with_m3u8_file)]
     return make_song_paths_relative_to_mpd_root(songs_absolute_location)
 
 
 @sched.register_command()
 def download_spotify_playlist_and_queue_and_zip(playlist_name, playlist_id, add_to_playlist, create_zip):
-    songs = get_songs_from_spotify_website(playlist_id)
+    songs = get_songs_from_spotify_website(playlist_id,
+                                           config["proxy"]["server"])
     songs_absolute_location = []
     print(f"We got {len(songs)} songs from the Spotify playlist")
     for i, song_of_playlist in enumerate(songs):
         report_progress(i, len(songs))
         # song_of_playlist: string (artist - song)
         try:
             track_id = deezer_search(song_of_playlist, TYPE_TRACK)[0]['id'] #[0] can throw IndexError
@@ -196,15 +203,17 @@
     if create_zip:
         return [create_zip_file(songs_with_m3u8_file)]
     return make_song_paths_relative_to_mpd_root(songs_absolute_location)
 
 
 @sched.register_command()
 def download_youtubedl_and_queue(video_url, add_to_playlist):
-    filename_absolute = youtubedl_download(video_url, config["download_dirs"]["youtubedl"])
+    filename_absolute = youtubedl_download(video_url,
+                                           config["download_dirs"]["youtubedl"],
+                                           config["proxy"]["server"])
     update_mpd_db(filename_absolute, add_to_playlist)
     return make_song_paths_relative_to_mpd_root([filename_absolute])
 
 
 @sched.register_command()
 def download_deezer_favorites(user_id: str, add_to_playlist: bool, create_zip: bool):
     songs_absolute_location = []
```

### Comparing `deezer_downloader-2.0.3/deezer_downloader/web/static/css/bootstrap-4.1.3-dist.zip` & `deezer_downloader-2.0.4/deezer_downloader/web/static/css/bootstrap-4.1.3-dist.zip`

 * *Files identical despite different names*

### Comparing `deezer_downloader-2.0.3/deezer_downloader/web/static/css/bootstrap.bundle.min.js` & `deezer_downloader-2.0.4/deezer_downloader/web/static/css/bootstrap.bundle.min.js`

 * *Files identical despite different names*

### Comparing `deezer_downloader-2.0.3/deezer_downloader/web/static/css/bootstrap.min.css` & `deezer_downloader-2.0.4/deezer_downloader/web/static/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `deezer_downloader-2.0.3/deezer_downloader/web/static/css/font-awesome.min.css` & `deezer_downloader-2.0.4/deezer_downloader/web/static/css/font-awesome.min.css`

 * *Files identical despite different names*

### Comparing `deezer_downloader-2.0.3/deezer_downloader/web/static/css/jquery.jgrowl.min.css` & `deezer_downloader-2.0.4/deezer_downloader/web/static/css/jquery.jgrowl.min.css`

 * *Files identical despite different names*

### Comparing `deezer_downloader-2.0.3/deezer_downloader/web/static/fonts/fontawesome-webfont.woff2` & `deezer_downloader-2.0.4/deezer_downloader/web/static/fonts/fontawesome-webfont.woff2`

 * *Files identical despite different names*

### Comparing `deezer_downloader-2.0.3/deezer_downloader/web/static/js/bootstrap.min.js` & `deezer_downloader-2.0.4/deezer_downloader/web/static/js/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `deezer_downloader-2.0.3/deezer_downloader/web/static/js/custom.js` & `deezer_downloader-2.0.4/deezer_downloader/web/static/js/custom.js`

 * *Files identical despite different names*

### Comparing `deezer_downloader-2.0.3/deezer_downloader/web/static/js/jquery.jgrowl.min.js` & `deezer_downloader-2.0.4/deezer_downloader/web/static/js/jquery.jgrowl.min.js`

 * *Files identical despite different names*

### Comparing `deezer_downloader-2.0.3/deezer_downloader/web/static/js/jquery.min.js` & `deezer_downloader-2.0.4/deezer_downloader/web/static/js/jquery.min.js`

 * *Files identical despite different names*

### Comparing `deezer_downloader-2.0.3/deezer_downloader/web/static/js/popper.min.js` & `deezer_downloader-2.0.4/deezer_downloader/web/static/js/popper.min.js`

 * *Files identical despite different names*

### Comparing `deezer_downloader-2.0.3/deezer_downloader/web/templates/index.html` & `deezer_downloader-2.0.4/deezer_downloader/web/templates/index.html`

 * *Files identical despite different names*

### Comparing `deezer_downloader-2.0.3/deezer_downloader/youtubedl.py` & `deezer_downloader-2.0.4/deezer_downloader/youtubedl.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import re
 from shlex import quote
 from subprocess import Popen, PIPE
 
 from deezer_downloader.configuration import config
-youtube_dl_cmd = config["youtubedl"]["command"] + " -x --audio-format mp3 --audio-quality 0 {video_url} -o '{destination_dir}/%(title)s.%(ext)s'"
 
 
 class YoutubeDLFailedException(Exception):
     pass
 
 
 class DownloadedFileNotFoundException(Exception):
@@ -29,23 +28,31 @@
 def get_absolute_filename(stdout, stderr):
     regex_foo = re.search(r'Destination:\s(.*mp3)', stdout)
     if not regex_foo:
         raise DownloadedFileNotFoundException("ERROR: Can not extract output file via regex. \nstderr: {}\nstdout: {}".format(stderr, stdout))
     return regex_foo.group(1)
 
 
-def youtubedl_download(url, destination_dir):
+def youtubedl_download(url, destination_dir, proxy=None):
     # url, e.g. https://www.youtube.com/watch?v=ZbZSe6N_BXs
     # destination_dir: /tmp/
+    # proxy: https/socks5 proxy (e. g. socks5://user:pass@127.0.0.1:1080/)
     # returns: absolute filename of the downloaded file
     # raises
     # YoutubeDLFailedException if youtube-dl exits with non-zero
     # DownloadedFileNotFoundException if we cannot get the converted output file from youtube-dl with a regex
 
     video_url = quote(url)
+    if proxy:
+        if proxy.startswith("socks5h://"):
+            # https://github.com/yt-dlp/yt-dlp/issues/6325
+            proxy = proxy.replace("socks5h://", "socks5://")
+        youtube_dl_cmd = config["youtubedl"]["command"] + f" --proxy {proxy} -x --audio-format mp3 --audio-quality 0 {video_url} -o '{destination_dir}/%(title)s.%(ext)s'"
+    else:
+        youtube_dl_cmd = config["youtubedl"]["command"] + " -x --audio-format mp3 --audio-quality 0 {video_url} -o '{destination_dir}/%(title)s.%(ext)s'"
     cmd = youtube_dl_cmd.format(video_url=video_url, destination_dir=destination_dir)
     filename_absolute = execute(cmd)
     return filename_absolute
 
 
 if __name__ == '__main__':
     video_url = "https://www.invidio.us/watch?v=ZbZSe6N_BXs"
```

### Comparing `deezer_downloader-2.0.3/PKG-INFO` & `deezer_downloader-2.0.4/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,28 +1,26 @@
 Metadata-Version: 2.1
 Name: deezer-downloader
-Version: 2.0.3
+Version: 2.0.4
 Summary: download music from Deezer with a nice front end
 Home-page: https://github.com/kmille/deezer-downloader
 Author: kmille
 Author-email: github@androidloves.me
-Requires-Python: >=3.7,<4.0
+Requires-Python: >=3.8.1,<4.0.0
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: flask (>=2.2.2,<3.0.0)
 Requires-Dist: flask-autoindex (>=0.6.6,<0.7.0)
 Requires-Dist: giphypop (>=0.3,<0.4)
 Requires-Dist: jinja2 (>=3.1.2,<4.0.0)
 Requires-Dist: pycryptodome (>=3.16.0,<4.0.0)
 Requires-Dist: python-mpd2 (>=3.0.5,<4.0.0)
-Requires-Dist: requests (>=2.28.1,<3.0.0)
+Requires-Dist: requests[socks] (>=2.28.2,<3.0.0)
 Requires-Dist: waitress (>=2.1.2,<3.0.0)
 Requires-Dist: yt-dlp
 Project-URL: Repository, https://github.com/kmille/deezer-downloader
 Description-Content-Type: text/markdown
 
 ## Music Downloader 🎶 🎧 💃 🦄
 ![tests](https://github.com/kmille/deezer-downloader/workflows/tests/badge.svg) ![push image to dockerhub](https://github.com/kmille/deezer-downloader/workflows/push%20to%20dockerhub/badge.svg) ![docker pulls](https://img.shields.io/docker/pulls/kmille2/deezer-downloader) ![latest tag](https://img.shields.io/github/v/tag/kmille/deezer-downloader?sort=semver) ![Python 3.6](https://img.shields.io/badge/python-%3E=3.6-blue.svg) ![pypi-version](https://img.shields.io/pypi/v/deezer-downloader) ![pypi-downloads](https://img.shields.io/pypi/dm/deezer-downloader)
@@ -35,14 +33,15 @@
 - download Spotify playlists (by parsing the Spotify website and download the songs from Deezer)
 - download as zip file (including m3u8 playlist file)
 - 320 kbit/s mp3s with ID3-Tags and album cover (UPDATE: right now only 128bkit/s mp3 works, see #66)
 - download songs via yt-dlp
 - KISS (keep it simple and stupid) front end
 - MPD integration (use it on a Raspberry Pi!)
 - simple REST api
+- proxy support (https/socks5)
 
 
 ### How to use it
 
 There is a settings file template called `settings.ini.example`. You can specify the download directory with  `download_dir`. Pressing the download button only downloads the song/album/playlist. If you set `use_mpd=True` in the `settings.ini` the backend will connect to mpd (localhost:6600) and update the music database. Pressing the play button will download the music. If `use_mpd=True`  is set the mpd database will be updated and the song/album/playlist will be added to the playlist. In `settings.ini` `music_dir` should be the music root location of mpd. The `download_dir` must be a subdirectory of `music_dir`. 
 
 As Deezer sometimes requires a captcha to login the auto login features was removed. Instead you have to manually insert a valid Deezer cookie to the `settings.ini`. The relevant cookie is the `arl` cookie.
```

