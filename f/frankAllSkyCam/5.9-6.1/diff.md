# Comparing `tmp/frankAllSkyCam-5.9.tar.gz` & `tmp/frankAllSkyCam-6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "frankAllSkyCam-5.9.tar", last modified: Sun May  7 07:59:05 2023, max compression
+gzip compressed data, was "frankAllSkyCam-6.1.tar", last modified: Thu May 18 17:58:59 2023, max compression
```

## Comparing `frankAllSkyCam-5.9.tar` & `frankAllSkyCam-6.1.tar`

### file list

```diff
@@ -1,20 +1,21 @@
-drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2023-05-07 07:59:05.198250 frankAllSkyCam-5.9/
--rw-r--r--   0 pi        (1000) pi        (1000)      899 2023-05-07 07:59:05.198250 frankAllSkyCam-5.9/PKG-INFO
-drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2023-05-07 07:59:05.198250 frankAllSkyCam-5.9/frankAllSkyCam/
--rwxrwxrw-   0 pi        (1000) pi        (1000)       71 2023-05-07 07:54:34.672446 frankAllSkyCam-5.9/frankAllSkyCam/__init__.py
--rwxrwxrw-   0 pi        (1000) pi        (1000)     3315 2023-05-06 17:05:56.950266 frankAllSkyCam-5.9/frankAllSkyCam/__main__.py
--rwxrwxrw-   0 pi        (1000) pi        (1000)      860 2023-05-06 07:38:43.382734 frankAllSkyCam-5.9/frankAllSkyCam/allskycamdelete.py
--rwxrw-rw-   0 pi        (1000) pi        (1000)     3109 2023-05-06 17:19:03.927275 frankAllSkyCam-5.9/frankAllSkyCam/config.py
--rwxrw-rw-   0 pi        (1000) pi        (1000)     3413 2023-05-06 06:51:58.022772 frankAllSkyCam-5.9/frankAllSkyCam/crontab.py
--rwxrw-rw-   0 pi        (1000) pi        (1000)     1484 2023-05-06 19:44:03.235757 frankAllSkyCam-5.9/frankAllSkyCam/drawtext.py
--rwxrwxrw-   0 pi        (1000) pi        (1000)     3492 2023-05-06 10:16:56.461921 frankAllSkyCam-5.9/frankAllSkyCam/fileManager.py
--rwxrwxrw-   0 pi        (1000) pi        (1000)    17973 2023-05-06 07:53:00.118852 frankAllSkyCam-5.9/frankAllSkyCam/imageHeader.py
--rwxrw-rw-   0 pi        (1000) pi        (1000)      503 2023-04-30 21:24:45.893867 frankAllSkyCam-5.9/frankAllSkyCam/index.py
--rwxrwxrw-   0 pi        (1000) pi        (1000)     2952 2023-05-06 07:38:13.134641 frankAllSkyCam-5.9/frankAllSkyCam/startrail.py
--rwxrw-rw-   0 pi        (1000) pi        (1000)     6939 2023-04-30 21:24:46.401862 frankAllSkyCam-5.9/frankAllSkyCam/suncalc2.py
--rwxrw-rw-   0 pi        (1000) pi        (1000)      941 2023-04-30 21:24:46.401862 frankAllSkyCam-5.9/frankAllSkyCam/test_sqm.py
--rwxrw-rw-   0 pi        (1000) pi        (1000)     2271 2023-05-06 06:49:45.473215 frankAllSkyCam-5.9/frankAllSkyCam/test_suncalc.py
--rwxrwxrw-   0 pi        (1000) pi        (1000)     4312 2023-05-07 07:53:56.040788 frankAllSkyCam-5.9/frankAllSkyCam/timelapse.py
--rwxrwxrw-   0 pi        (1000) pi        (1000)     1397 2023-05-06 07:37:43.869298 frankAllSkyCam-5.9/frankAllSkyCam/watchDog.py
--rwxrw-rw-   0 pi        (1000) pi        (1000)       65 2023-04-26 18:08:27.179909 frankAllSkyCam-5.9/setup.cfg
--rwxrwxrw-   0 pi        (1000) pi        (1000)     1824 2023-05-07 07:55:28.139972 frankAllSkyCam-5.9/setup.py
+drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2023-05-18 17:58:59.773238 frankAllSkyCam-6.1/
+-rw-r--r--   0 pi        (1000) pi        (1000)      899 2023-05-18 17:58:59.773238 frankAllSkyCam-6.1/PKG-INFO
+drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2023-05-18 17:58:59.773238 frankAllSkyCam-6.1/frankAllSkyCam/
+-rwxrwxrw-   0 pi        (1000) pi        (1000)       71 2023-05-18 17:57:30.758010 frankAllSkyCam-6.1/frankAllSkyCam/__init__.py
+-rwxrwxrw-   0 pi        (1000) pi        (1000)     3332 2023-05-14 09:27:21.198243 frankAllSkyCam-6.1/frankAllSkyCam/__main__.py
+-rwxrwxrw-   0 pi        (1000) pi        (1000)      860 2023-05-06 17:26:30.883699 frankAllSkyCam-6.1/frankAllSkyCam/allskycamdelete.py
+-rwxrw-rw-   0 pi        (1000) pi        (1000)     3109 2023-05-06 17:26:30.883699 frankAllSkyCam-6.1/frankAllSkyCam/config.py
+-rwxrw-rw-   0 pi        (1000) pi        (1000)     3413 2023-05-06 17:26:30.883699 frankAllSkyCam-6.1/frankAllSkyCam/crontab.py
+-rwxrw-rw-   0 pi        (1000) pi        (1000)     1564 2023-05-16 19:32:33.936871 frankAllSkyCam-6.1/frankAllSkyCam/drawtext.py
+-rwxrwxrw-   0 pi        (1000) pi        (1000)     3492 2023-05-06 17:26:30.883699 frankAllSkyCam-6.1/frankAllSkyCam/fileManager.py
+-rwxrwxrw-   0 pi        (1000) pi        (1000)    17648 2023-05-16 19:33:50.855978 frankAllSkyCam-6.1/frankAllSkyCam/imageHeader.py
+-rwxrw-rw-   0 pi        (1000) pi        (1000)      503 2023-05-06 17:26:30.883699 frankAllSkyCam-6.1/frankAllSkyCam/index.py
+-rwxrw-rw-   0 pi        (1000) pi        (1000)    15593 2023-05-17 17:00:21.302391 frankAllSkyCam-6.1/frankAllSkyCam/sqmreader.py
+-rwxrwxrw-   0 pi        (1000) pi        (1000)     2952 2023-05-06 17:26:30.883699 frankAllSkyCam-6.1/frankAllSkyCam/startrail.py
+-rwxrw-rw-   0 pi        (1000) pi        (1000)     6939 2023-05-06 17:26:30.887699 frankAllSkyCam-6.1/frankAllSkyCam/suncalc2.py
+-rwxrw-rw-   0 pi        (1000) pi        (1000)      941 2023-05-06 17:26:30.887699 frankAllSkyCam-6.1/frankAllSkyCam/test_sqm.py
+-rwxrw-rw-   0 pi        (1000) pi        (1000)     2271 2023-05-06 17:26:30.887699 frankAllSkyCam-6.1/frankAllSkyCam/test_suncalc.py
+-rwxrwxrw-   0 pi        (1000) pi        (1000)     4312 2023-05-07 07:16:59.842911 frankAllSkyCam-6.1/frankAllSkyCam/timelapse.py
+-rwxrwxrw-   0 pi        (1000) pi        (1000)     1397 2023-05-06 17:26:30.887699 frankAllSkyCam-6.1/frankAllSkyCam/watchDog.py
+-rwxrw-rw-   0 pi        (1000) pi        (1000)       65 2023-04-26 18:08:27.179909 frankAllSkyCam-6.1/setup.cfg
+-rwxrwxrw-   0 pi        (1000) pi        (1000)     1824 2023-05-18 17:56:59.106286 frankAllSkyCam-6.1/setup.py
```

### Comparing `frankAllSkyCam-5.9/PKG-INFO` & `frankAllSkyCam-6.1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 1.1
 Name: frankAllSkyCam
-Version: 5.9
+Version: 6.1
 Summary: AllSkyCamera with Raspberry Pi and Pi HQ Camera 
 Home-page: https://github.com/sferlix/frankAllSkyCam
 Author: Francesco Sferlazza
 Author-email: sferlazza@gmail.com
 License: MIT
-Download-URL: https://github.com/sferlix/frankAllSkyCam/archive/refs/tags/5.9.tar.gz
+Download-URL: https://github.com/sferlix/frankAllSkyCam/archive/refs/tags/6.1.tar.gz
 Description: UNKNOWN
 Keywords: AllSkyCamera,Astronomy,AllSky
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `frankAllSkyCam-5.9/frankAllSkyCam/__main__.py` & `frankAllSkyCam-6.1/frankAllSkyCam/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -71,16 +71,17 @@
        comando +=" --shutter " + str(int(esposiz)) + " "
        comando += additional_params
     else:
        comando += " --metering average "
 
     try:
        # ensure no libcamera is operating
-       killcmd = "ps -ef|grep libcamera-still| grep -v color|awk '{print $2}'|xargs kill -9 1> /dev/null 2>&1"
+       killcmd = "ps -ef|grep libcamera | grep -v color|awk '{print $2}'|xargs kill -9 1> /dev/null 2>&1"
        os.system(killcmd)
+       print(killcmd)
 
        print(comando)
        os.system(comando)
 
        print("Image captured")
        # print watermark
        drawtext.printWatermark(s, nomefile, font_size, font_color)
```

### Comparing `frankAllSkyCam-5.9/frankAllSkyCam/allskycamdelete.py` & `frankAllSkyCam-6.1/frankAllSkyCam/allskycamdelete.py`

 * *Files identical despite different names*

### Comparing `frankAllSkyCam-5.9/frankAllSkyCam/config.py` & `frankAllSkyCam-6.1/frankAllSkyCam/config.py`

 * *Files identical despite different names*

### Comparing `frankAllSkyCam-5.9/frankAllSkyCam/crontab.py` & `frankAllSkyCam-6.1/frankAllSkyCam/crontab.py`

 * *Files identical despite different names*

### Comparing `frankAllSkyCam-5.9/frankAllSkyCam/drawtext.py` & `frankAllSkyCam-6.1/frankAllSkyCam/drawtext.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,37 +20,40 @@
     esposiz   = s[13]
     sqm       = s[14]
 
     photo = Image.open(nomefile)
     drawing = ImageDraw.Draw(photo)
     font = ImageFont.truetype("DejaVuSerif.ttf", font_size)
     if len(fc)==0:
-       fc=[255,255,255]
-	   
+       fc=[255,0,0]
+
+    if sqm > 16:
+       fc=[247,13,26]
+
     colore = (fc[0], fc[1],fc[2])
 
     pos=(5, 0)
     stringa = data + "\n" + ora
     if esposiz>0:
-       stringa = stringa + "\nExp(s) = " + str(int(esposiz/1000000))
+       esposiz = round(esposiz / 1000000,3)
+       stringa = stringa + "\nExp(s) = " + str(esposiz)
 
     drawing.text(pos, stringa, fill=colore, font=font)
 
     pos=(300, 0)
     stringa = inte
     drawing.text(pos, stringa, fill=colore, font=font)
 
-    pos=(630,0)
+    pos=(670,0)
     stringa = "Sunrise " + srise + "\nSunset " + sset 
     drawing.text(pos, stringa, fill=colore, font=font)
 
     pos=(5, 535)
-    stringa = "Night Start "+ NS +"\nNight End "+ NE + "\nSQM " + sqm
+    stringa = "Night Start "+ NS +"\nNight End "+ NE + "\nSQM: " + str(round(sqm,2))
     drawing.text(pos, stringa, fill=colore, font=font)
 
     pos=(630,535)
     stringa = "Moonrise " + moon_rise + "\nMoonset " + moon_set + "\n" + str(fract) + "% | " + phase
     drawing.text(pos, stringa, fill=colore, font=font)
 
-
     photo.save(nomefile)
     return
```

### Comparing `frankAllSkyCam-5.9/frankAllSkyCam/fileManager.py` & `frankAllSkyCam-6.1/frankAllSkyCam/fileManager.py`

 * *Files identical despite different names*

### Comparing `frankAllSkyCam-5.9/frankAllSkyCam/imageHeader.py` & `frankAllSkyCam-6.1/frankAllSkyCam/imageHeader.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 import datetime
 import time
 import traceback
 from datetime import datetime, timedelta
 from frankAllSkyCam import suncalc2, fileManager
+from frankAllSkyCam import sqmreader
 from pytz import timezone
 import pytz
 import sys
 import math
 import os
 from importlib import resources  # Python 3.7+
 from configparser import ConfigParser
 import socket
-
+import numpy
 
 config = ConfigParser()
 configFileName = fileManager.getConfigFileName()
 config.read(configFileName)
 appPath = os.path.expanduser("~") + "/frankAllSkyCam/"
 
 time_zone = str(config['site']['time_zone'])
@@ -33,20 +34,14 @@
 ms_duration = float(config['moon']['ms_duration'])
 mr_offset = float(config['moon']['mr_offset'])
 mr_duration = float(config['moon']['mr_duration'])
 
 dd_offset_dawn = float(config['offset']['dawn'])
 dd_offset_dusk = float(config['offset']['dusk'])
 
-SQM_LE = str(config['sqm_le']['use_sqm'])
-SQM_LE_IP = str(config['sqm_le']['ip_address'])
-SQM_LE_PORT = float(config['sqm_le']['port'])
-SQM_WRITE_LOG = str(config['sqm_le']['write_log'])
-SQM_FOLDER = appPath + str(config['system']['sqmFolder'])
-
 esp_secs = float(config['exposure']['esp_secs'])
 esp_dawn_dusk = float(config['exposure']['esp_dawn_dusk'])
 
 def getHeader(datacalcolo):
     isDebug= True          # True will stampa debug info. False, not
     logLevel = 0           # 0 = basic, 1= full
     isLinear= False        # True: linear variation of exposure; False:quadratic
@@ -72,15 +67,15 @@
        #valori[9] = nightstart
        #valori[10]= nightend
        #valori[11]= moonphase
        #valori[12] = moonangle
        #valori[13] = exposure
        #valori[14] = sqm
 
-       valori=["",0,False,"","","","","","","","","","","",""]
+       valori=["",0,False,"","","","","","","","","","",0,0]
 
        tz = timezone(timeZone)
        stampa("Orario attuale = "+str(datacalcolo), isDebug, logLevel, 0)
 
        # get sun information
        sc = suncalc2.getTimes(datacalcolo, latitude, longitude)
 
@@ -125,22 +120,21 @@
        moon_reduction = getMoonReduction(datacalcolo,isDebug, logLevel)
     
        moon_rise = moonValues[0]
        moon_set = moonValues[1]
        fr = moonValues[2]
        ph = moonValues[3]
 
-       sqm = '--.--'
-       if SQM_LE == 'y':
-          sqm = readSQM()
+       #sqm = sqmreader.readSQM()
 
        stampa("suncalc2= "+str(sc), isDebug, logLevel, 1)
        sep = " | "
        stringa = datacalcolo.strftime("%d/%m %H:%M") + sep + "NS " + NS + sep
-       stringa += "NE " + NE + sep+ "MR " + moon_rise + sep + "MS " + moon_set + sep + str(int(round(fr*100,0))) + "% | " + ph +' | SQM ' + sqm + ' |'
+       stringa += "NE " + NE + sep+ "MR " + moon_rise + sep + "MS " + moon_set + sep + str(int(round(fr*100,0))) + "% | " + ph
+       # +' | SQM ' + sqm + ' |'
 
 
        stampa(stringa, isDebug, logLevel, 0)
 
        # offset dawn e dusk 
        dawn = dawn+timedelta(minutes= + dd_offset_dawn)
        dusk = dusk+timedelta(minutes= + dd_offset_dusk)
@@ -210,18 +204,17 @@
        if zona == "notte":
           esposizione = int(esp_secs * 1000000 * riduzione_totale)
        elif zona == "alba" or zona == "tramonto":
           esposizione = int(esp_dawn_dusk * 1000000 * riduzione_totale)
        else:
           esposizione = 0
 
-       e=0
-
-       if SQM_LE == "y":
-          e = getSQM()
+       lett = getSQM()
+       e= lett[0]
+       sqm= lett[1]
 
        if e> 0:
           esposizione = e * 1000000
 
        stringa += str(round(esposizione/1000000,3))
        valori[0] = datacalcolo.strftime("%d/%m/%y")
        valori[1] = datacalcolo.strftime("%H:%M")
@@ -238,15 +231,15 @@
        valori[12] = str(int(round(fr*100,0)))
        valori[13] = esposizione
        valori[14] = sqm
 
        #print(valori)
 
     except Exception as e:
-       stampa("type error: " + str(e), isDebug, logLevel, 0)
+#       stampa("type error: " + str(e), isDebug, logLevel, 0)
        stampa(traceback.format_exc(), isDebug, logLevel, 0)
        valori[0] = ""
        valori[1] = 0
     return valori
 
 
 def getMoonValues(datacalcolo, isDebug, logLevel):
@@ -350,25 +343,26 @@
    smt_prima = suncalc2.getMoonTimes(datacalcolo+timedelta(days=-1), latitude, longitude)
    smt_dopo  = suncalc2.getMoonTimes(datacalcolo+timedelta(days=1), latitude, longitude)
 
    try:
       mrise= smt["rise"].astimezone(tz)
       moon_rise = str(mrise)[11:16]
    except:
-      mset="--"
-      moon_set="--"
+      mrise="--"
+      moon_rise="--"
 
 
    try:
       mset= smt["set"].astimezone(tz)
       moon_set = str(mset)[11:16]
    except:
       mset="--"
       moon_set="--"
 
+  
    if moon_rise!="--" and moon_set!="--":
       if mrise > mset and datacalcolo > mrise:
          if datacalcolo <=mset:
             # mrise del giorno prima
             mrise= "--"
             moon_rise = "--"
          elif (datacalcolo > mset and datacalcolo < mrise) or (datacalcolo >=mrise):
@@ -474,45 +468,49 @@
 def stampa(stringa, isDebug, logLevel, logActual):
     if isDebug==False:
         return
     if logLevel>=logActual:
         print("   " + stringa)
     return
 
-def readSQM():
-    sqm = '--.--'
-    try:
-        s = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
-        #print(SQM_LE_IP + ":" + str(int(SQM_LE_PORT)))
-        s.connect((SQM_LE_IP,int(SQM_LE_PORT)))
-        #print('connected')
-        s.sendall(b'rx')
-        msg = ''
-        while len(msg) < 55:
-          chunk = s.recv(55-len(msg))
-          if chunk == '':
-             print("socket connection broken")
-          msg = msg + str(chunk)
-        #print(msg)
-        sqm=msg[5:10]
-        #print(sqm)
-        s.close()
-        if SQM_WRITE_LOG=='y':
-            if int(sqm[0:2]) > 0:
-                tz = timezone(timeZone)
-                d = datetime.now(tz)
-                line = d.strftime("%d/%m/%Y %H:%M") + "," + sqm + "\n"
-                f = open(SQM_FOLDER + "/sqm.csv", "a+")
-                f.write(line)
-                f.close()
-    except:
-        print('aaa')
-    return sqm
-
 def getSQM():
+   ex=0
+   sq=0
+   r= [ex,sq]
+
+   try:
+      sq = sqmreader.readSQM()
+   except:
+      stampa("type error: " + str(e), isDebug, logLevel, 0)
+      stampa(traceback.format_exc(), isDebug, logLevel, 0)
+      print("imageHeader.getSQM: Error while calculating SQM")
+
+
+   if sq < 10.5:
+      return r
+   elif sq >= 10.5 and sq <= 17:
+      myExp=[10.5, 11.0, 11.5, 12.5, 13.5, 14.5, 15.5, 16.5,  17]
+      mySqm=[ 0.0, 0.01, 0.025, 0.07, 0.20, 0.70, 1.10,  1.8, 2.2]
+      polyGrade = 6
+   else:
+      myExp=[17.0, 17.5, 18.0, 18.5, 19.5, 20.5, 21, 22]
+      mySqm=[2.2,  3.00, 10.0, 15.0, 30.0, 45.0, 55, 75]
+      polyGrade = 3
+
+   myModel= numpy.poly1d(numpy.polyfit(myExp, mySqm, polyGrade ))
+   ex = myModel(sq)
+
+   if ex>esp_secs:
+      ex = esp_secs
+   
+   r=[ex,sq]
+   return r
+
+
+def getSQMold():
    try:
       s = float(readSQM())
    except:
       print("SQM: Error Reading SQM. Assuming no SMQ Reader")
       s = 0
```

### Comparing `frankAllSkyCam-5.9/frankAllSkyCam/startrail.py` & `frankAllSkyCam-6.1/frankAllSkyCam/startrail.py`

 * *Files identical despite different names*

### Comparing `frankAllSkyCam-5.9/frankAllSkyCam/suncalc2.py` & `frankAllSkyCam-6.1/frankAllSkyCam/suncalc2.py`

 * *Files identical despite different names*

### Comparing `frankAllSkyCam-5.9/frankAllSkyCam/test_sqm.py` & `frankAllSkyCam-6.1/frankAllSkyCam/test_sqm.py`

 * *Files identical despite different names*

### Comparing `frankAllSkyCam-5.9/frankAllSkyCam/test_suncalc.py` & `frankAllSkyCam-6.1/frankAllSkyCam/test_suncalc.py`

 * *Files identical despite different names*

### Comparing `frankAllSkyCam-5.9/frankAllSkyCam/timelapse.py` & `frankAllSkyCam-6.1/frankAllSkyCam/timelapse.py`

 * *Files identical despite different names*

### Comparing `frankAllSkyCam-5.9/frankAllSkyCam/watchDog.py` & `frankAllSkyCam-6.1/frankAllSkyCam/watchDog.py`

 * *Files identical despite different names*

### Comparing `frankAllSkyCam-5.9/setup.py` & `frankAllSkyCam-6.1/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from distutils.core import setup
 
 setup(
   name = 'frankAllSkyCam',         # How you named your package folder (MyLib)
   packages = ['frankAllSkyCam'],   # Chose the same as "name"
-  version = '5.9',      # Start with a small number and increase it with every change you make
+  version = '6.1',      # Start with a small number and increase it with every change you make
   license='MIT',        # Chose a license from here: https://help.github.com/articles/licensing-a-repository
   description = 'AllSkyCamera with Raspberry Pi and Pi HQ Camera ',   # Give a short description about your library
   author = 'Francesco Sferlazza',                   # Type in your name
   author_email = 'sferlazza@gmail.com',      # Type in your E-Mail
   url = 'https://github.com/sferlix/frankAllSkyCam',   # Provide either the link to your github or to your website
-  download_url = 'https://github.com/sferlix/frankAllSkyCam/archive/refs/tags/5.9.tar.gz',    # I explain this later on
+  download_url = 'https://github.com/sferlix/frankAllSkyCam/archive/refs/tags/6.1.tar.gz',    # I explain this later on
   keywords = ['AllSkyCamera', 'Astronomy', 'AllSky'],   # Keywords that define your package best
   install_requires=[            # I get to this in a second
           'pytz',
           'numpy',
       ],
   classifiers=[
     'Development Status :: 4 - Beta',      # Chose either "3 - Alpha", "4 - Beta" or "5 - Production/Stable" as the current state of your package
```

