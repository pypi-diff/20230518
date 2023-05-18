# Comparing `tmp/raspisump-1.6.tar.gz` & `tmp/raspisump-1.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "raspisump-1.6.tar", last modified: Tue May 16 16:42:20 2023, max compression
+gzip compressed data, was "raspisump-1.6.1.tar", last modified: Thu May 18 16:54:00 2023, max compression
```

## Comparing `raspisump-1.6.tar` & `raspisump-1.6.1.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxr-xr-x   0 al        (1000) users      (984)        0 2023-05-16 16:42:20.720138 raspisump-1.6/
--rw-r--r--   0 al        (1000) users      (984)     1073 2023-02-19 16:52:26.000000 raspisump-1.6/LICENSE
--rw-r--r--   0 al        (1000) users      (984)      278 2023-05-10 18:31:52.000000 raspisump-1.6/MANIFEST.in
--rw-r--r--   0 al        (1000) users      (984)     3940 2023-05-16 16:42:20.716805 raspisump-1.6/PKG-INFO
--rw-r--r--   0 al        (1000) users      (984)     3168 2023-05-11 10:55:58.000000 raspisump-1.6/README.md
--rw-r--r--   0 al        (1000) users      (984)       23 2023-05-16 16:38:14.000000 raspisump-1.6/VERSION
-drwxr-xr-x   0 al        (1000) users      (984)        0 2023-05-16 16:42:20.710138 raspisump-1.6/bin/
--rw-r--r--   0 al        (1000) users      (984)      362 2023-05-16 16:38:14.000000 raspisump-1.6/bin/emailtest
--rwxr-xr-x   0 al        (1000) users      (984)      866 2023-05-16 16:38:14.000000 raspisump-1.6/bin/rsump.py
--rwxr-xr-x   0 al        (1000) users      (984)      619 2023-05-16 16:38:14.000000 raspisump-1.6/bin/rsumpchart.py
--rwxr-xr-x   0 al        (1000) users      (984)      537 2023-05-16 16:38:14.000000 raspisump-1.6/bin/rsumpmonitor.py
--rwxr-xr-x   0 al        (1000) users      (984)      662 2023-05-16 16:38:14.000000 raspisump-1.6/bin/rsumpwebchart.py
-drwxr-xr-x   0 al        (1000) users      (984)        0 2023-05-16 16:42:20.710138 raspisump-1.6/conf/
-drwxr-xr-x   0 al        (1000) users      (984)        0 2023-05-16 16:42:20.713472 raspisump-1.6/conf/charts/
--rw-r--r--   0 al        (1000) users      (984)       80 2022-04-12 11:43:48.000000 raspisump-1.6/conf/charts/README.md
-drwxr-xr-x   0 al        (1000) users      (984)        0 2023-05-16 16:42:20.713472 raspisump-1.6/conf/csv/
--rw-r--r--   0 al        (1000) users      (984)       80 2022-04-12 11:43:48.000000 raspisump-1.6/conf/csv/README.md
--rw-r--r--   0 al        (1000) users      (984)     1112 2023-05-10 18:31:52.000000 raspisump-1.6/conf/lighttpd.conf
-drwxr-xr-x   0 al        (1000) users      (984)        0 2023-05-16 16:42:20.713472 raspisump-1.6/conf/logs/
--rw-r--r--   0 al        (1000) users      (984)      217 2022-04-12 11:43:48.000000 raspisump-1.6/conf/logs/README.md
--rw-r--r--   0 al        (1000) users      (984)     5687 2022-04-12 11:43:48.000000 raspisump-1.6/conf/raspisump.conf
-drwxr-xr-x   0 al        (1000) users      (984)        0 2023-05-16 16:42:20.713472 raspisump-1.6/conf/web/
-drwxr-xr-x   0 al        (1000) users      (984)        0 2023-05-16 16:42:20.713472 raspisump-1.6/conf/web/css/
--rw-r--r--   0 al        (1000) users      (984)        0 2022-04-12 11:43:48.000000 raspisump-1.6/conf/web/css/index.html
--rw-r--r--   0 al        (1000) users      (984)      614 2022-04-12 11:43:48.000000 raspisump-1.6/conf/web/css/raspi.css
--rw-r--r--   0 al        (1000) users      (984)      690 2022-04-12 11:43:48.000000 raspisump-1.6/conf/web/css/raspi.css~
-drwxr-xr-x   0 al        (1000) users      (984)        0 2023-05-16 16:42:20.713472 raspisump-1.6/conf/web/images/
--rw-r--r--   0 al        (1000) users      (984)    51981 2022-04-12 11:43:48.000000 raspisump-1.6/conf/web/images/logo.png
--rwxr-xr-x   0 al        (1000) users      (984)      906 2022-04-12 11:43:48.000000 raspisump-1.6/conf/web/index.html
-drwxr-xr-x   0 al        (1000) users      (984)        0 2023-05-16 16:42:20.713472 raspisump-1.6/cron/
--rw-r--r--   0 al        (1000) users      (984)      140 2022-04-12 11:43:48.000000 raspisump-1.6/cron/README.md
--rw-r--r--   0 al        (1000) users      (984)      258 2022-04-12 11:43:48.000000 raspisump-1.6/cron/picrontab
-drwxr-xr-x   0 al        (1000) users      (984)        0 2023-05-16 16:42:20.713472 raspisump-1.6/docs/
--rw-r--r--   0 al        (1000) users      (984)      275 2022-04-12 11:43:48.000000 raspisump-1.6/docs/README.md
--rw-r--r--   0 al        (1000) users      (984)    11066 2023-05-16 16:38:14.000000 raspisump-1.6/docs/install.md
--rw-r--r--   0 al        (1000) users      (984)   133692 2023-05-10 18:31:52.000000 raspisump-1.6/docs/install.pdf
-drwxr-xr-x   0 al        (1000) users      (984)        0 2023-05-16 16:42:20.716805 raspisump-1.6/raspisump/
--rwxr-xr-x   0 al        (1000) users      (984)        0 2022-04-12 11:43:48.000000 raspisump-1.6/raspisump/__init__.py
--rw-r--r--   0 al        (1000) users      (984)     4910 2023-05-16 16:38:14.000000 raspisump-1.6/raspisump/alerts.py
--rw-r--r--   0 al        (1000) users      (984)     1980 2023-05-16 16:38:14.000000 raspisump-1.6/raspisump/checkpid.py
--rw-r--r--   0 al        (1000) users      (984)     1962 2023-05-16 16:38:14.000000 raspisump-1.6/raspisump/emailtest.py
--rw-r--r--   0 al        (1000) users      (984)     4594 2023-05-16 16:38:14.000000 raspisump-1.6/raspisump/heartbeat.py
--rw-r--r--   0 al        (1000) users      (984)      821 2023-05-16 16:38:14.000000 raspisump-1.6/raspisump/log.py
--rw-r--r--   0 al        (1000) users      (984)     2704 2023-05-16 16:38:14.000000 raspisump-1.6/raspisump/reading.py
--rw-r--r--   0 al        (1000) users      (984)     2565 2023-05-16 16:38:14.000000 raspisump-1.6/raspisump/todaychart.py
--rw-r--r--   0 al        (1000) users      (984)     1490 2023-05-16 16:38:14.000000 raspisump-1.6/raspisump/webchart.py
-drwxr-xr-x   0 al        (1000) users      (984)        0 2023-05-16 16:42:20.716805 raspisump-1.6/raspisump.egg-info/
--rw-r--r--   0 al        (1000) users      (984)     3940 2023-05-16 16:42:20.000000 raspisump-1.6/raspisump.egg-info/PKG-INFO
--rw-r--r--   0 al        (1000) users      (984)      784 2023-05-16 16:42:20.000000 raspisump-1.6/raspisump.egg-info/SOURCES.txt
--rw-r--r--   0 al        (1000) users      (984)        1 2023-05-16 16:42:20.000000 raspisump-1.6/raspisump.egg-info/dependency_links.txt
--rw-r--r--   0 al        (1000) users      (984)       13 2023-05-16 16:42:20.000000 raspisump-1.6/raspisump.egg-info/requires.txt
--rw-r--r--   0 al        (1000) users      (984)       10 2023-05-16 16:42:20.000000 raspisump-1.6/raspisump.egg-info/top_level.txt
--rw-r--r--   0 al        (1000) users      (984)       38 2023-05-16 16:42:20.720138 raspisump-1.6/setup.cfg
--rwxr-xr-x   0 al        (1000) users      (984)     2316 2023-05-16 16:38:14.000000 raspisump-1.6/setup.py
+drwxr-xr-x   0 al        (1000) users      (984)        0 2023-05-18 16:54:00.070026 raspisump-1.6.1/
+-rw-r--r--   0 al        (1000) users      (984)     1073 2023-02-19 16:52:26.000000 raspisump-1.6.1/LICENSE
+-rw-r--r--   0 al        (1000) users      (984)      278 2023-05-10 18:31:52.000000 raspisump-1.6.1/MANIFEST.in
+-rw-r--r--   0 al        (1000) users      (984)     3942 2023-05-18 16:54:00.070026 raspisump-1.6.1/PKG-INFO
+-rw-r--r--   0 al        (1000) users      (984)     3168 2023-05-11 10:55:58.000000 raspisump-1.6.1/README.md
+-rw-r--r--   0 al        (1000) users      (984)       25 2023-05-18 16:52:54.000000 raspisump-1.6.1/VERSION
+drwxr-xr-x   0 al        (1000) users      (984)        0 2023-05-18 16:54:00.063360 raspisump-1.6.1/bin/
+-rw-r--r--   0 al        (1000) users      (984)      362 2023-05-16 16:38:14.000000 raspisump-1.6.1/bin/emailtest
+-rwxr-xr-x   0 al        (1000) users      (984)      866 2023-05-16 16:38:14.000000 raspisump-1.6.1/bin/rsump.py
+-rwxr-xr-x   0 al        (1000) users      (984)      619 2023-05-16 16:38:14.000000 raspisump-1.6.1/bin/rsumpchart.py
+-rwxr-xr-x   0 al        (1000) users      (984)      537 2023-05-16 16:38:14.000000 raspisump-1.6.1/bin/rsumpmonitor.py
+-rwxr-xr-x   0 al        (1000) users      (984)      662 2023-05-16 16:38:14.000000 raspisump-1.6.1/bin/rsumpwebchart.py
+drwxr-xr-x   0 al        (1000) users      (984)        0 2023-05-18 16:54:00.063360 raspisump-1.6.1/conf/
+drwxr-xr-x   0 al        (1000) users      (984)        0 2023-05-18 16:54:00.063360 raspisump-1.6.1/conf/charts/
+-rw-r--r--   0 al        (1000) users      (984)       80 2022-04-12 11:43:48.000000 raspisump-1.6.1/conf/charts/README.md
+drwxr-xr-x   0 al        (1000) users      (984)        0 2023-05-18 16:54:00.063360 raspisump-1.6.1/conf/csv/
+-rw-r--r--   0 al        (1000) users      (984)       80 2022-04-12 11:43:48.000000 raspisump-1.6.1/conf/csv/README.md
+-rw-r--r--   0 al        (1000) users      (984)     1112 2023-05-10 18:31:52.000000 raspisump-1.6.1/conf/lighttpd.conf
+drwxr-xr-x   0 al        (1000) users      (984)        0 2023-05-18 16:54:00.063360 raspisump-1.6.1/conf/logs/
+-rw-r--r--   0 al        (1000) users      (984)      217 2022-04-12 11:43:48.000000 raspisump-1.6.1/conf/logs/README.md
+-rw-r--r--   0 al        (1000) users      (984)     5687 2022-04-12 11:43:48.000000 raspisump-1.6.1/conf/raspisump.conf
+drwxr-xr-x   0 al        (1000) users      (984)        0 2023-05-18 16:54:00.063360 raspisump-1.6.1/conf/web/
+drwxr-xr-x   0 al        (1000) users      (984)        0 2023-05-18 16:54:00.063360 raspisump-1.6.1/conf/web/css/
+-rw-r--r--   0 al        (1000) users      (984)        0 2022-04-12 11:43:48.000000 raspisump-1.6.1/conf/web/css/index.html
+-rw-r--r--   0 al        (1000) users      (984)      614 2022-04-12 11:43:48.000000 raspisump-1.6.1/conf/web/css/raspi.css
+-rw-r--r--   0 al        (1000) users      (984)      690 2022-04-12 11:43:48.000000 raspisump-1.6.1/conf/web/css/raspi.css~
+drwxr-xr-x   0 al        (1000) users      (984)        0 2023-05-18 16:54:00.063360 raspisump-1.6.1/conf/web/images/
+-rw-r--r--   0 al        (1000) users      (984)    51981 2022-04-12 11:43:48.000000 raspisump-1.6.1/conf/web/images/logo.png
+-rwxr-xr-x   0 al        (1000) users      (984)      906 2022-04-12 11:43:48.000000 raspisump-1.6.1/conf/web/index.html
+drwxr-xr-x   0 al        (1000) users      (984)        0 2023-05-18 16:54:00.066693 raspisump-1.6.1/cron/
+-rw-r--r--   0 al        (1000) users      (984)      140 2022-04-12 11:43:48.000000 raspisump-1.6.1/cron/README.md
+-rw-r--r--   0 al        (1000) users      (984)      258 2022-04-12 11:43:48.000000 raspisump-1.6.1/cron/picrontab
+drwxr-xr-x   0 al        (1000) users      (984)        0 2023-05-18 16:54:00.066693 raspisump-1.6.1/docs/
+-rw-r--r--   0 al        (1000) users      (984)      275 2022-04-12 11:43:48.000000 raspisump-1.6.1/docs/README.md
+-rw-r--r--   0 al        (1000) users      (984)    11066 2023-05-16 16:38:14.000000 raspisump-1.6.1/docs/install.md
+-rw-r--r--   0 al        (1000) users      (984)   133692 2023-05-10 18:31:52.000000 raspisump-1.6.1/docs/install.pdf
+drwxr-xr-x   0 al        (1000) users      (984)        0 2023-05-18 16:54:00.066693 raspisump-1.6.1/raspisump/
+-rwxr-xr-x   0 al        (1000) users      (984)        0 2022-04-12 11:43:48.000000 raspisump-1.6.1/raspisump/__init__.py
+-rw-r--r--   0 al        (1000) users      (984)     4910 2023-05-16 16:38:14.000000 raspisump-1.6.1/raspisump/alerts.py
+-rw-r--r--   0 al        (1000) users      (984)     2068 2023-05-18 16:52:54.000000 raspisump-1.6.1/raspisump/checkpid.py
+-rw-r--r--   0 al        (1000) users      (984)     1962 2023-05-16 16:38:14.000000 raspisump-1.6.1/raspisump/emailtest.py
+-rw-r--r--   0 al        (1000) users      (984)     4594 2023-05-16 16:38:14.000000 raspisump-1.6.1/raspisump/heartbeat.py
+-rw-r--r--   0 al        (1000) users      (984)      821 2023-05-16 16:38:14.000000 raspisump-1.6.1/raspisump/log.py
+-rw-r--r--   0 al        (1000) users      (984)     2704 2023-05-16 16:38:14.000000 raspisump-1.6.1/raspisump/reading.py
+-rw-r--r--   0 al        (1000) users      (984)     2565 2023-05-16 16:38:14.000000 raspisump-1.6.1/raspisump/todaychart.py
+-rw-r--r--   0 al        (1000) users      (984)     1490 2023-05-16 16:38:14.000000 raspisump-1.6.1/raspisump/webchart.py
+drwxr-xr-x   0 al        (1000) users      (984)        0 2023-05-18 16:54:00.070026 raspisump-1.6.1/raspisump.egg-info/
+-rw-r--r--   0 al        (1000) users      (984)     3942 2023-05-18 16:53:59.000000 raspisump-1.6.1/raspisump.egg-info/PKG-INFO
+-rw-r--r--   0 al        (1000) users      (984)      784 2023-05-18 16:53:59.000000 raspisump-1.6.1/raspisump.egg-info/SOURCES.txt
+-rw-r--r--   0 al        (1000) users      (984)        1 2023-05-18 16:53:59.000000 raspisump-1.6.1/raspisump.egg-info/dependency_links.txt
+-rw-r--r--   0 al        (1000) users      (984)       13 2023-05-18 16:53:59.000000 raspisump-1.6.1/raspisump.egg-info/requires.txt
+-rw-r--r--   0 al        (1000) users      (984)       10 2023-05-18 16:53:59.000000 raspisump-1.6.1/raspisump.egg-info/top_level.txt
+-rw-r--r--   0 al        (1000) users      (984)       38 2023-05-18 16:54:00.070026 raspisump-1.6.1/setup.cfg
+-rwxr-xr-x   0 al        (1000) users      (984)     2318 2023-05-18 16:52:54.000000 raspisump-1.6.1/setup.py
```

### Comparing `raspisump-1.6/LICENSE` & `raspisump-1.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `raspisump-1.6/PKG-INFO` & `raspisump-1.6.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: raspisump
-Version: 1.6
+Version: 1.6.1
 Summary: A sump pit monitoring system for Raspberry Pi
 Home-page: https://www.linuxnorth.org/raspi-sump/
 Download-URL: https://github.com/alaudet/raspi-sump/releases
 Author: Al Audet
 Author-email: alaudet@linuxnorth.org
 License: MIT License
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `raspisump-1.6/README.md` & `raspisump-1.6.1/README.md`

 * *Files identical despite different names*

### Comparing `raspisump-1.6/bin/rsump.py` & `raspisump-1.6.1/bin/rsump.py`

 * *Files identical despite different names*

### Comparing `raspisump-1.6/bin/rsumpchart.py` & `raspisump-1.6.1/bin/rsumpchart.py`

 * *Files identical despite different names*

### Comparing `raspisump-1.6/bin/rsumpmonitor.py` & `raspisump-1.6.1/bin/rsumpmonitor.py`

 * *Files identical despite different names*

### Comparing `raspisump-1.6/bin/rsumpwebchart.py` & `raspisump-1.6.1/bin/rsumpwebchart.py`

 * *Files identical despite different names*

### Comparing `raspisump-1.6/conf/lighttpd.conf` & `raspisump-1.6.1/conf/lighttpd.conf`

 * *Files identical despite different names*

### Comparing `raspisump-1.6/conf/raspisump.conf` & `raspisump-1.6.1/conf/raspisump.conf`

 * *Files identical despite different names*

### Comparing `raspisump-1.6/conf/web/css/raspi.css` & `raspisump-1.6.1/conf/web/css/raspi.css`

 * *Files identical despite different names*

### Comparing `raspisump-1.6/conf/web/css/raspi.css~` & `raspisump-1.6.1/conf/web/css/raspi.css~`

 * *Files identical despite different names*

### Comparing `raspisump-1.6/conf/web/images/logo.png` & `raspisump-1.6.1/conf/web/images/logo.png`

 * *Files identical despite different names*

### Comparing `raspisump-1.6/conf/web/index.html` & `raspisump-1.6.1/conf/web/index.html`

 * *Files identical despite different names*

### Comparing `raspisump-1.6/docs/install.md` & `raspisump-1.6.1/docs/install.md`

 * *Files identical despite different names*

### Comparing `raspisump-1.6/docs/install.pdf` & `raspisump-1.6.1/docs/install.pdf`

 * *Files identical despite different names*

### Comparing `raspisump-1.6/raspisump/alerts.py` & `raspisump-1.6.1/raspisump/alerts.py`

 * *Files identical despite different names*

### Comparing `raspisump-1.6/raspisump/checkpid.py` & `raspisump-1.6.1/raspisump/checkpid.py`

 * *Files 13% similar despite different names*

```diff
@@ -33,20 +33,22 @@
     part2.stdout.close()
     part4 = subprocess.Popen(cmdp4list, stdin=part3.stdout,
                              stdout=subprocess.PIPE
                              )
     part3.stdout.close()
     number_of_processes = int(part4.communicate()[0])
     if number_of_processes == 0:
-        log.log_errors('rsump.py process stopped, restarting')
+        log.log_event('error_log',
+                      'ERROR - rsump.py process stopped, restarting')
         restart(process)
     elif number_of_processes == 1:
         exit(0)
     else:
-        log.log_errors('Multiple rsump.py processes...killing and restarting')
+        log.log_event('error_log',
+                      'ERROR - Multiple rsump.py processes...killing all and restarting')
         kill_start(process)
 
 
 def restart(process):
     '''Restart process'''
     restart_cmd = process + ' &'
     restart_now = restart_cmd.split(' ')
```

### Comparing `raspisump-1.6/raspisump/emailtest.py` & `raspisump-1.6.1/raspisump/emailtest.py`

 * *Files identical despite different names*

### Comparing `raspisump-1.6/raspisump/heartbeat.py` & `raspisump-1.6.1/raspisump/heartbeat.py`

 * *Files identical despite different names*

### Comparing `raspisump-1.6/raspisump/log.py` & `raspisump-1.6.1/raspisump/log.py`

 * *Files identical despite different names*

### Comparing `raspisump-1.6/raspisump/reading.py` & `raspisump-1.6.1/raspisump/reading.py`

 * *Files identical despite different names*

### Comparing `raspisump-1.6/raspisump/todaychart.py` & `raspisump-1.6.1/raspisump/todaychart.py`

 * *Files identical despite different names*

### Comparing `raspisump-1.6/raspisump/webchart.py` & `raspisump-1.6.1/raspisump/webchart.py`

 * *Files identical despite different names*

### Comparing `raspisump-1.6/raspisump.egg-info/PKG-INFO` & `raspisump-1.6.1/raspisump.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: raspisump
-Version: 1.6
+Version: 1.6.1
 Summary: A sump pit monitoring system for Raspberry Pi
 Home-page: https://www.linuxnorth.org/raspi-sump/
 Download-URL: https://github.com/alaudet/raspi-sump/releases
 Author: Al Audet
 Author-email: alaudet@linuxnorth.org
 License: MIT License
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `raspisump-1.6/raspisump.egg-info/SOURCES.txt` & `raspisump-1.6.1/raspisump.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `raspisump-1.6/setup.py` & `raspisump-1.6.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup
 import os
 
-version = "1.6"
+version = "1.6.1"
 
 homedir = "/home/pi/raspi-sump/"
 
 if os.path.isfile(homedir + "raspisump.conf"):
     cmd = "cp -u " + homedir + "raspisump.conf " + homedir + "raspisump.conf.save"
     os.system(cmd)
```

