# Comparing `tmp/n4s-2.4.2.tar.gz` & `tmp/n4s-2.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "n4s-2.4.2.tar", last modified: Mon Mar  6 06:15:34 2023, max compression
+gzip compressed data, was "n4s-2.4.3.tar", last modified: Wed May 17 21:56:01 2023, max compression
```

## Comparing `n4s-2.4.2.tar` & `n4s-2.4.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 afshari    (501) staff       (20)        0 2023-03-06 06:15:34.984207 n4s-2.4.2/
--rw-r--r--   0 afshari    (501) staff       (20)     1067 2022-06-27 07:38:29.000000 n4s-2.4.2/LICENSE
--rw-r--r--   0 afshari    (501) staff       (20)     2149 2023-03-06 06:15:34.984098 n4s-2.4.2/PKG-INFO
--rw-r--r--   0 afshari    (501) staff       (20)     1707 2022-07-19 04:58:48.000000 n4s-2.4.2/README.md
-drwxr-xr-x   0 afshari    (501) staff       (20)        0 2023-03-06 06:15:34.983320 n4s-2.4.2/n4s/
--rw-r--r--   0 afshari    (501) staff       (20)       77 2022-06-28 05:44:13.000000 n4s-2.4.2/n4s/__init__.py
--rw-r--r--   0 afshari    (501) staff       (20)    51944 2023-03-06 06:14:41.000000 n4s-2.4.2/n4s/fs.py
--rw-r--r--   0 afshari    (501) staff       (20)    11804 2022-12-16 17:27:26.000000 n4s-2.4.2/n4s/strgs.py
--rw-r--r--   0 afshari    (501) staff       (20)     6341 2022-07-06 03:16:12.000000 n4s-2.4.2/n4s/term.py
--rw-r--r--   0 afshari    (501) staff       (20)    27854 2023-02-28 19:12:28.000000 n4s-2.4.2/n4s/web.py
-drwxr-xr-x   0 afshari    (501) staff       (20)        0 2023-03-06 06:15:34.983945 n4s-2.4.2/n4s.egg-info/
--rw-r--r--   0 afshari    (501) staff       (20)     2149 2023-03-06 06:15:34.000000 n4s-2.4.2/n4s.egg-info/PKG-INFO
--rw-r--r--   0 afshari    (501) staff       (20)      196 2023-03-06 06:15:34.000000 n4s-2.4.2/n4s.egg-info/SOURCES.txt
--rw-r--r--   0 afshari    (501) staff       (20)        1 2023-03-06 06:15:34.000000 n4s-2.4.2/n4s.egg-info/dependency_links.txt
--rw-r--r--   0 afshari    (501) staff       (20)        4 2023-03-06 06:15:34.000000 n4s-2.4.2/n4s.egg-info/top_level.txt
--rw-r--r--   0 afshari    (501) staff       (20)       38 2023-03-06 06:15:34.984242 n4s-2.4.2/setup.cfg
--rw-r--r--   0 afshari    (501) staff       (20)      849 2023-03-06 06:10:36.000000 n4s-2.4.2/setup.py
+drwxr-xr-x   0 afshari    (501) staff       (20)        0 2023-05-17 21:56:01.380954 n4s-2.4.3/
+-rw-r--r--   0 afshari    (501) staff       (20)     1067 2023-05-17 21:55:49.000000 n4s-2.4.3/LICENSE
+-rw-r--r--   0 afshari    (501) staff       (20)     2149 2023-05-17 21:56:01.380840 n4s-2.4.3/PKG-INFO
+-rw-r--r--   0 afshari    (501) staff       (20)     1707 2023-05-17 21:55:49.000000 n4s-2.4.3/README.md
+drwxr-xr-x   0 afshari    (501) staff       (20)        0 2023-05-17 21:56:01.380281 n4s-2.4.3/n4s/
+-rw-r--r--   0 afshari    (501) staff       (20)       77 2023-05-17 21:55:49.000000 n4s-2.4.3/n4s/__init__.py
+-rw-r--r--   0 afshari    (501) staff       (20)    51944 2023-05-17 21:55:49.000000 n4s-2.4.3/n4s/fs.py
+-rw-r--r--   0 afshari    (501) staff       (20)    11804 2023-05-17 21:55:49.000000 n4s-2.4.3/n4s/strgs.py
+-rw-r--r--   0 afshari    (501) staff       (20)     6341 2023-05-17 21:55:49.000000 n4s-2.4.3/n4s/term.py
+-rw-r--r--   0 afshari    (501) staff       (20)    27662 2023-05-17 21:55:49.000000 n4s-2.4.3/n4s/web.py
+drwxr-xr-x   0 afshari    (501) staff       (20)        0 2023-05-17 21:56:01.380685 n4s-2.4.3/n4s.egg-info/
+-rw-r--r--   0 afshari    (501) staff       (20)     2149 2023-05-17 21:56:01.000000 n4s-2.4.3/n4s.egg-info/PKG-INFO
+-rw-r--r--   0 afshari    (501) staff       (20)      196 2023-05-17 21:56:01.000000 n4s-2.4.3/n4s.egg-info/SOURCES.txt
+-rw-r--r--   0 afshari    (501) staff       (20)        1 2023-05-17 21:56:01.000000 n4s-2.4.3/n4s.egg-info/dependency_links.txt
+-rw-r--r--   0 afshari    (501) staff       (20)        4 2023-05-17 21:56:01.000000 n4s-2.4.3/n4s.egg-info/top_level.txt
+-rw-r--r--   0 afshari    (501) staff       (20)       38 2023-05-17 21:56:01.380989 n4s-2.4.3/setup.cfg
+-rw-r--r--   0 afshari    (501) staff       (20)      849 2023-05-17 21:55:49.000000 n4s-2.4.3/setup.py
```

### Comparing `n4s-2.4.2/LICENSE` & `n4s-2.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `n4s-2.4.2/PKG-INFO` & `n4s-2.4.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: n4s
-Version: 2.4.2
+Version: 2.4.3
 Summary: Collection of useful methods by Need4Swede
 Home-page: https://github.com/n4s/n4s
 Author: Mike Afshari
 Author-email: theneed4swede@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: n4s Version: 2.4.2 Summary: Collection of useful
+Metadata-Version: 2.1 Name: n4s Version: 2.4.3 Summary: Collection of useful
 methods by Need4Swede Home-page: https://github.com/n4s/n4s Author: Mike
 Afshari Author-email: theneed4swede@gmail.com License: MIT Classifier:
 Programming Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT
 License Classifier: Operating System :: OS Independent Requires-Python: >=3.6
 Description-Content-Type: text/markdown License-File: LICENSE
     [logo.png] **When you feel the need...for an awesome Python package!**
     ______________________________________________________________________
```

### Comparing `n4s-2.4.2/README.md` & `n4s-2.4.3/README.md`

 * *Files identical despite different names*

### Comparing `n4s-2.4.2/n4s/fs.py` & `n4s-2.4.3/n4s/fs.py`

 * *Files identical despite different names*

### Comparing `n4s-2.4.2/n4s/strgs.py` & `n4s-2.4.3/n4s/strgs.py`

 * *Files identical despite different names*

### Comparing `n4s-2.4.2/n4s/term.py` & `n4s-2.4.3/n4s/term.py`

 * *Files identical despite different names*

### Comparing `n4s-2.4.2/n4s/web.py` & `n4s-2.4.3/n4s/web.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import os, sys, shutil, re, base64, warnings, webbrowser, requests, math
 import http.client as httplib
 from n4s import fs, strgs
 from bs4 import BeautifulSoup
 from pathlib import Path
 ##### Dismiss the 'XML' warning
-warnings.filterwarnings("ignore", 
+warnings.filterwarnings("ignore",
 category=UserWarning, module='bs4')
 #############################
 
 
 ## WEB BROWSWER
 def browser(Action: str, Browser: str, URL: str='', debug: bool=False):
   '''
@@ -48,55 +48,56 @@
         ## RETURN TAB URL
         if debug:
           print(active_tab)
         return active_tab
 
     ## ADD PROTOCOL
     if not "http://" or not "https://" in URL:
-      URL = URL.split('/')[-1]
-      URL = f"https://{URL}"
-    
+      if "file://" not in URL:
+        URL = URL.split('/')[-1]
+        URL = f"https://{URL}"
+
     ## OPEN WEB ADDRESS IN BROWSER
     if Action.lower() == 'open':
 
       ## OPEN URL IN CHROME
       if Browser.lower() == 'google chrome':
         web_browser.open_location(URL)
         return
-      
+
       ## OPEN URL IN SAFARI
       if Browser.lower() == 'safari':
         web_browser.make(new=k.document,with_properties={k.URL:URL})
         return
 
   ## WINDOWS
   else:
     ## PRINT ERROR
     if debug:
       print('\n\nn4s.web.browser()\nOnly macOS is supported at this time!\n')
     return
 
 ## BUILD WEB TEMPLATES
 def build_html(Design: str='default', onefile: bool=False, Directory: Path=fs.root('desktop'), debug: bool=False):
-        
+
   ## DIRECTORIES
   index_dir = f"{Directory}/index"
   assets_dir = f"{index_dir}/assets"
   css_dir = f"{assets_dir}/css"
   js_dir = f"{assets_dir}/js"
 
   ## FILES
   html_file = f"{index_dir}/index.html"
   css_file = f"{css_dir}/style.css"
   js_file = f"{js_dir}/script.js"
-  
+
   Design = Design.lower()
   ###### TEMPLATES #############
   ## DEFAULT                   #
-  if Design == 'default':      
+  if Design == 'default':
     ## HTML - DEFAULT TEMPALTE
     html_string = '''
 <!DOCTYPE html>
 <html xmlns="http://www.w3.org/1999/xhtml" xml:lang="en" lang="en">
     <head>
         <meta http-equiv="Content-Type" content="text/html; charset=utf-8" />
         <title>Document</title>
@@ -466,61 +467,61 @@
 '''
 
     ## JS - DEFAULT TEMPLATE
     js_string = '''
 console.log(`%cCreated using n4s, by: \nhttps://www.mafshari.work`, 'color:lightgreen;');
 '''
   ## IFRAME                    #
-  elif Design == 'iframe':    
+  elif Design == 'iframe':
     ## HTML - IFRAME
     html_string = '''
 <!DOCTYPE html>
 <html lang="en">
 <head>
     <meta charset="UTF-8">
     <meta http-equiv="X-UA-Compatible" content="IE=edge">
     <meta name="viewport" content="width=device-width, initial-scale=1.0">
     <link rel="stylesheet" type="text/css" href="assets/css/style.css"/>
     <title>Document</title>
 </head>
 <body>
-    <iframe src="https://www.mafshari.work/websites/simplicity" frameborder="0" 
-    marginheight="0" 
-    marginwidth="0" 
-    width="100%" 
-    height="100%" 
+    <iframe src="https://www.mafshari.work/websites/simplicity" frameborder="0"
+    marginheight="0"
+    marginwidth="0"
+    width="100%"
+    height="100%"
     scrolling="auto"></iframe>
 </body>
 </html>
 '''
-          
+
     ## CSS - IFRAME
     css_string = '''
-html 
+html
 {
  overflow: auto;
 }
- 
-html, body, div, iframe 
+
+html, body, div, iframe
 {
- margin: 0px; 
- padding: 0px; 
- height: 100%; 
+ margin: 0px;
+ padding: 0px;
+ height: 100%;
  border: none;
 }
-iframe 
+iframe
 {
- display: block; 
- width: 100%; 
- border: none; 
- overflow-y: auto; 
+ display: block;
+ width: 100%;
+ border: none;
+ overflow-y: auto;
  overflow-x: hidden;
 }
 '''
-          
+
     ## JS - IFRAME
     js_string = '''
 console.log(`%cCreated using n4s, by: \nhttps://www.mafshari.work`, 'color:lightgreen;');
 '''
   ## APPLE - PODCAST REPORT    #
   elif Design == 'applepodcastreport' or Design == 'apr':
     print('\nDownloading Apple Podcast Report...')
@@ -535,61 +536,61 @@
     <meta charset="UTF-8">
     <meta http-equiv="X-UA-Compatible" content="IE=edge">
     <meta name="viewport" content="width=device-width, initial-scale=1.0">
     <link rel="stylesheet" type="text/css" href="assets/css/style.css"/>
     <title>N4S - Barcode Generator</title>
 </head>
 <body>
-    <iframe src="https://barcode-maker.netlify.app/generator/" frameborder="0" 
-    marginheight="0" 
-    marginwidth="0" 
-    width="100%" 
-    height="100%" 
+    <iframe src="https://barcode-maker.netlify.app/generator/" frameborder="0"
+    marginheight="0"
+    marginwidth="0"
+    width="100%"
+    height="100%"
     scrolling="auto"></iframe>
 </body>
 </html>
 '''
-          
+
           ## CSS - IFRAME
           css_string = '''
-html 
+html
 {
  overflow: auto;
 }
- 
-html, body, div, iframe 
+
+html, body, div, iframe
 {
- margin: 0px; 
- padding: 0px; 
- height: 100%; 
+ margin: 0px;
+ padding: 0px;
+ height: 100%;
  border: none;
 }
-iframe 
+iframe
 {
- display: block; 
- width: 100%; 
- border: none; 
- overflow-y: auto; 
+ display: block;
+ width: 100%;
+ border: none;
+ overflow-y: auto;
  overflow-x: hidden;
 }
 '''
-          
+
           ## JS - IFRAME
           js_string = '''
 console.log(`%cCreated using n4s, by: \nhttps://www.mafshari.work`, 'color:lightgreen;');
 '''
   ## BARCODE GENERATOR - DOWNLOAD
   elif Design == 'barcodegenerator-dl' or Design == 'barcode-dl':
     print('\nDownloading Barcode Generator...')
     url = "https://drive.google.com/uc?export=download&id=1QQqCM0OdD1GhuIKv7lsxVa7ItBsj3VE8"
     r = requests.get(url, allow_redirects=True)
     open(f"{Directory}/barcode_generator.zip", 'wb').write(r.content)
     return print(f'Done: {Directory}/barcode_generator.zip')
   ## CLEAN GUIDE TEMPLATE      #
-  elif Design == 'guide-clean-noscroll':      
+  elif Design == 'guide-clean-noscroll':
     print('\nDownloading Guide - Clean w/ No Scroll...')
     url = "https://drive.google.com/uc?export=download&id=1gKpq1a1Ddfo5CRGA5jmh6vzUXmIPaIbf"
     r = requests.get(url, allow_redirects=True)
     open(f"{Directory}/guide_clean_noscroll.zip", 'wb').write(r.content)
     return print(f'Done: {Directory}/guide_clean_noscroll.zip')
   ##############################
 
@@ -601,19 +602,19 @@
       css_file,
       js_file
   ], True)
 
   ## OUTPUT HTML FILE
   with open(html_file, 'w') as htmlFile:
     htmlFile.write(html_string)
-  
+
   ## OUTPUT CSS FILE
   with open(css_file, 'w') as cssFile:
     cssFile.write(css_string)
-  
+
   ## OUTPUT JAVASCRIPT FILE
   with open(js_file, 'w') as jsFile:
     jsFile.write(js_string)
 
   ## MERGE THE FILES INTO ONE
   if onefile:
     merge_html(html_file, css_file, js_file, True, False)
@@ -660,19 +661,19 @@
       build_html()
     return
 
   ## OUTPUT HTML FILE
   if not fs.path_exists(html_file) and not HTML == '':
     with open(html_file, 'w+') as htmlFile:
         htmlFile.write(HTML)
-  
+
   ## OUTPUT CSS FILE
   with open(css_file, 'w+') as cssFile:
       cssFile.write(CSS)
-  
+
   ## OUTPUT JAVASCRIPT FILE
   with open(js_file, 'w+') as jsFile:
       jsFile.write(JS)
 
   ## MERGE HTML, CSS AND JS FILES
   if onefile:
     merge_html(html_file, css_file, js_file, True)
@@ -681,15 +682,15 @@
 def download(URL: str, Filename: str='', Save_Directory: Path=fs.root('downloads'), Detect_Format: bool=True, debug: bool=False):
   '''
   URL: (str) to file or (list) of strings to files
   Filename: Save As... (leave blank to inherit original filename)
   Save_Directory: Save To... (default = User/Downloads)
   debug: Print downloads to console
   '''
-  
+
   ## DOWNLOAD A LIST OF FILES
   if type(URL) == list:
 
     ## ARRAY OF FILENAMES
     filenames = []
 
     ## INITIAL FILENAME
@@ -703,15 +704,15 @@
 
       ## READ FILE FORMAT
       file_format = f".{URL[link].split('.')[-1]}"
 
       ## DEBUG: PRINT DL MESSAGE
       if debug:
         print(f"\nDownloading from {URL[link]}")
-      
+
       ## DOWNLOAD FILE
       r = requests.get(URL[link], allow_redirects=True)
 
       ## IF NO FILENAME ENTERED, USE ORIGINAL FILENAME FROM WEB
       if Filename == '':
         Filename = str(URL[link]).split('/')[-1]
 
@@ -724,32 +725,32 @@
 
       ## SAVE FILE TO CHOSEN DIRECTORY
       open(f"{Save_Directory}/{Filename}", 'wb').write(r.content)
 
       ## DEBUG: PRINT COMPLETION MESSAGE
       if debug:
         print(f'Done: {Save_Directory}/{Filename}')
-  
+
   ## DOWNLOAD SINGLE FILE
   if type(URL) == str:
-    
+
     ## READ FILE FORMAT
     file_format = f".{str(URL).split('.')[-1]}"
 
     ## DEBUG: PRINT DL MESSAGE
     if debug:
       print(f'\nDownloading from [{URL}]')
-    
+
     ## DOWNLOAD FILE
     r = requests.get(URL, allow_redirects=True)
-    
+
     ## IF NO FILENAME ENTERED, USE ORIGINAL FILENAME FROM WEB
     if Filename == '':
       Filename = str(URL).split("/")[-1]
-    
+
     ## IF FILENAME ENTERED, BUT NO EXTENSION SPECIFIED - GET EXTENSION FROM ORIGINAL FILE
     if not '.' in Filename and Detect_Format:
       Filename = f"{Filename}{file_format}"
 
     ## SAVE FILE TO CHOSEN DIRECTORY
     open(f"{Save_Directory}/{Filename}", 'wb').write(r.content)
 
@@ -757,29 +758,29 @@
     if debug:
       print(f'Done: {Save_Directory}/{Filename}')
 
 ## CALL ITUNES API
 def itunes_api(Type: str, Country: str, Term: str, Output: str='all', Print: bool=False):
   '''
   Type: movie, podcast, music, musicVideo, audiobook, shortFilm, tvShow, software, ebook, all
-  
+
   Country: The two-letter country code for the store you want to search
-  
+
   Term: The string you want to search for
-  
+
   Limit: The number of results you want the iTunes API to return
-  
+
   Output: wrapperType, kind, artistId, collectionId, trackId, artistName, collectionName, trackName, collectionCensoredName, trackCensoredName, artistViewUrl, collectionViewUrl, feedUrl, trackViewUrl, artworkUrl30, artworkUrl60, artworkUrl100, collectionPrice, trackPrice, collectionHdPrice, releaseDate, collectionExplicitness, trackExplicitness, trackCount, trackTimeMillis, country, currency, primaryGenreName, contentAdvisoryRating, artworkUrl600, genreIds, genres, all
 
   Print: Prints results to terminal
   '''
-  
+
   ## TYPES OF RETURN OPTIONS
   output_options = 'wrapperType,kind,artistId,collectionId,trackId,artistName,collectionName,trackName,collectionCensoredName,trackCensoredName,artistViewUrl,collectionViewUrl,feedUrl,trackViewUrl,artworkUrl30,artworkUrl60,artworkUrl100,collectionPrice,trackPrice,collectionHdPrice,releaseDate,collectionExplicitness,trackExplicitness,trackCount,trackTimeMillis,country,currency,primaryGenreName,contentAdvisoryRating,artworkUrl600,genreIds,genres,all'
-  
+
   ## SPLIT OPTIONS INTO LIST
   output_options = output_options.split(',')
 
   ## VERIFY A VALID NETWORK CONNECTION
   _network = network_test()
 
   ## CALL ITUNES API
@@ -789,33 +790,33 @@
         'country': Country,
         'entity': Type,
         'limit': 1
     })
 
     ## GATHER RESULTS
     data = r.json()
-  
+
   ## NO INTERNET CONNECTION
   else:
     return print("\nn4s.web.itunes_api():\n"
             "Failed to connect online. Verify your internet connection!\n")
-  
+
   ## RETURN ALL RESULTS FROM API CALL
   if Output == 'all':
 
     ## IF PRINT
     if Print:
       data = str(data)
       data = data.split(',')
       for x in range(len(data)):
         print(data[x])
-    
+
     ## RETURN
     return data
-  
+
   ## RETURN SPECIFIC RESULT FROM API CALL
   else:
 
     ## ITERATE THROUGH OUTPUT OPTIONS
     for option in output_options:
 
       ## IF PRINT
@@ -839,46 +840,46 @@
     resp = requests.request('HEAD', File)
   except Exception: ## INVALID ADDRESS / FAILED TO CONNECT
     if debug:
       print("\nn4s.web.read_filesize():\n"
             "Unable to retrieve filesize\n"
             "Error => Failed to Connect / Invalid Address\n")
     return
-  
+
   ## VERIFY CONTENT LENGTH KEY IN HEADER
   if 'Content-Length' in resp.headers:
       file_size = resp.headers['Content-Length']
   else:
       try:
           resp = requests.request('HEAD', File)
           file_size = resp.headers['Content-Length']
       except KeyError:
           if debug:
             print("\nn4s.web.read_filesize():\n"
                   "Unable to retrieve filesize\n"
                   "Error => No 'Content-Length' Key\n")
           return
-  
+
   ## CAST FILE SIZE AS INT
   file_size = int(file_size)
-  
+
   ## CONVERT FILE SIZE
   if file_size == 0:
       return "0B"
   size_name = ("B", "KB", "MB", "GB", "TB", "PB", "EB", "ZB", "YB")
   i = int(math.floor(math.log(file_size, 1024)))
   p = math.pow(1024, i)
   s = round(file_size / p, 2)
-  
+
   # RETURN FILE SIZE IN BYTES
   if Bytes:
     if Print:
       print(file_size)
     return file_size
-  
+
   ## RETURN FILE SIZE (FORMATTED)
   if Print:
     print("%s %s" % (s, size_name[i]))
   return "%s %s" % (s, size_name[i])
 
 ## MERGE HTML/CSS/JS INTO ONE HTML FILE
 def merge_html(HTML: Path, CSS: Path, JS: Path, onefile: bool=False, debug: bool=False, filename: str='index', remove_webfiles: bool=False):
@@ -921,45 +922,45 @@
                     if debug:
                         return print('\nn4s.web.merge_html():\nCSS File Not Found - Files Not Merged\n')
                     else:
                         return
 
                 # remove the tag from soup
                 tag.extract()
-        
+
                 # insert style element
                 new_style = soup.new_tag('style')
                 new_style.string = css_file
                 soup.html.head.append(new_style)
                 break
-        
+
         ## FIND SCRIPT TAGS : <script src="js/script.js"></script>
         for tag in soup.find_all('script', src=True):
             if tag.has_attr('src'):
                 try:
                     js_file = Path(f'{JS}').read_text(encoding="utf-8")
                 except FileNotFoundError:
                     if debug:
                         return print('\nn4s.web.merge_html():\nJS File Not Found - Files Not Merged\n')
                     else:
                         return
 
                 # remove the tag from soup
                 tag.extract()
-        
+
                 # insert script element
                 new_script = soup.new_tag('script')
                 new_script.string = js_file
                 soup.html.body.append(new_script)
-        
+
         ## FIND IMAGE TAGS : <img src="" alt="">
         for tag in soup.find_all('img', src=True):
             if tag.has_attr('src'):
                 file_content = Path(tag['src']).read_bytes()
-        
+
                 # replace filename with base64 of the content of the file
                 base64_file_content = base64.b64encode(file_content)
                 tag['src'] = "data:image/png;base64, {}".format(base64_file_content.decode('ascii'))
 
         ## CREATE WEBFILES DIR FOR PREVIOUS FILES
         fs.path_exists(f"{directory}/webfiles", True)
 
@@ -1019,29 +1020,29 @@
         except Exception:
             return False
         finally:
             network_connectivity_test.close()
 
 ## READS FILE EXTENSIONS
 def read_format(Input: str, Include_Period: bool=False, Print: bool=False, Uppercase: bool=False):
-    
+
     ## INCLUDE PERIOD IN FORMAT
     if Include_Period:
         file_format = f".{Input.split('.')[-1]}"
-    
+
     ## RETURN FORMAT WITHOUT PERIOD
     else:
         file_format = Input.split('.')[-1]
 
     ## CLEAR SPECIAL CHARACTERS
     if '?' in file_format:
         file_format = file_format.split('?')[0]
     if '/' in file_format:
         file_format = file_format.split('/')[0]
-    
+
     ## IF UPPERCASE == ENABLED
     if Uppercase:
         file_format = file_format.upper()
 
     ## PRINT FORMAT TO TERMINAL
     if Print:
         print(file_format)
```

### Comparing `n4s-2.4.2/n4s.egg-info/PKG-INFO` & `n4s-2.4.3/n4s.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: n4s
-Version: 2.4.2
+Version: 2.4.3
 Summary: Collection of useful methods by Need4Swede
 Home-page: https://github.com/n4s/n4s
 Author: Mike Afshari
 Author-email: theneed4swede@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: n4s Version: 2.4.2 Summary: Collection of useful
+Metadata-Version: 2.1 Name: n4s Version: 2.4.3 Summary: Collection of useful
 methods by Need4Swede Home-page: https://github.com/n4s/n4s Author: Mike
 Afshari Author-email: theneed4swede@gmail.com License: MIT Classifier:
 Programming Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT
 License Classifier: Operating System :: OS Independent Requires-Python: >=3.6
 Description-Content-Type: text/markdown License-File: LICENSE
     [logo.png] **When you feel the need...for an awesome Python package!**
     ______________________________________________________________________
```

### Comparing `n4s-2.4.2/setup.py` & `n4s-2.4.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     pip(['install', '--user', 'appscript==1.2.0'])
 
 pip(['install', '--user', 'beautifulsoup4==4.11.1'])
 pip(['install', '--user', 'requests==2.27.1'])
 
 setuptools.setup(
     name='n4s',
-    version='2.4.2',
+    version='2.4.3',
     author='Mike Afshari',
     author_email='theneed4swede@gmail.com',
     description='Collection of useful methods by Need4Swede',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='https://github.com/n4s/n4s',
     license='MIT',
```

