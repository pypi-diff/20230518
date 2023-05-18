# Comparing `tmp/academyAI-1.0.2.tar.gz` & `tmp/academyAI-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "academyAI-1.0.2.tar", last modified: Thu May 18 19:30:32 2023, max compression
+gzip compressed data, was "academyAI-1.0.3.tar", last modified: Thu May 18 19:40:21 2023, max compression
```

## Comparing `academyAI-1.0.2.tar` & `academyAI-1.0.3.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxrwx   0        0        0        0 2023-05-18 19:30:32.769497 academyAI-1.0.2/
--rw-rw-rw-   0        0        0       90 2023-05-18 19:30:32.769497 academyAI-1.0.2/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-05-18 19:30:32.770526 academyAI-1.0.2/setup.cfg
--rw-rw-rw-   0        0        0      190 2023-05-18 19:30:26.000000 academyAI-1.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-18 19:30:32.739592 academyAI-1.0.2/src/
-drwxrwxrwx   0        0        0        0 2023-05-18 19:30:32.767560 academyAI-1.0.2/src/academyAI.egg-info/
--rw-rw-rw-   0        0        0       90 2023-05-18 19:30:32.000000 academyAI-1.0.2/src/academyAI.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      173 2023-05-18 19:30:32.000000 academyAI-1.0.2/src/academyAI.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-18 19:30:32.000000 academyAI-1.0.2/src/academyAI.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2023-05-18 19:30:32.000000 academyAI-1.0.2/src/academyAI.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1905 2023-05-18 19:04:45.000000 academyAI-1.0.2/src/academyAI.py
+drwxrwxrwx   0        0        0        0 2023-05-18 19:40:21.128196 academyAI-1.0.3/
+-rw-rw-rw-   0        0        0       90 2023-05-18 19:40:21.127201 academyAI-1.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-05-18 19:40:21.128196 academyAI-1.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      190 2023-05-18 19:40:11.000000 academyAI-1.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-18 19:40:21.090829 academyAI-1.0.3/src/
+drwxrwxrwx   0        0        0        0 2023-05-18 19:40:21.125198 academyAI-1.0.3/src/academyAI.egg-info/
+-rw-rw-rw-   0        0        0       90 2023-05-18 19:40:20.000000 academyAI-1.0.3/src/academyAI.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      173 2023-05-18 19:40:20.000000 academyAI-1.0.3/src/academyAI.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-18 19:40:20.000000 academyAI-1.0.3/src/academyAI.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2023-05-18 19:40:20.000000 academyAI-1.0.3/src/academyAI.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1740 2023-05-18 19:37:35.000000 academyAI-1.0.3/src/academyAI.py
```

### Comparing `academyAI-1.0.2/src/academyAI.py` & `academyAI-1.0.3/src/academyAI.py`

 * *Files 10% similar despite different names*

```diff
@@ -51,11 +51,8 @@
         response_data = response.json()
         if "data" in response_data:
             image_url = response_data["data"][0]["url"]
         else:
             image_url = "Sorry, the response from the API was not in the expected format."
         return image_url
     
-test=AcademyAI("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")
-answer = test.paint_AI("A goat on a fence eating")
-import webbrowser
-webbrowser.open(answer)
+
```

