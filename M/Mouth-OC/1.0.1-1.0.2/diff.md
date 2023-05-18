# Comparing `tmp/Mouth-OC-1.0.1.tar.gz` & `tmp/Mouth-OC-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Mouth-OC-1.0.1.tar", last modified: Tue Mar 21 14:45:36 2023, max compression
+gzip compressed data, was "Mouth-OC-1.0.2.tar", last modified: Sun Mar 26 13:22:07 2023, max compression
```

## Comparing `Mouth-OC-1.0.1.tar` & `Mouth-OC-1.0.2.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxr-x   0 bast      (1002) bast      (1002)        0 2023-03-21 14:45:36.780460 Mouth-OC-1.0.1/
--rw-rw-r--   0 bast      (1002) bast      (1002)      360 2023-01-10 19:59:34.000000 Mouth-OC-1.0.1/LICENSE
-drwxrwxr-x   0 bast      (1002) bast      (1002)        0 2023-03-21 14:45:36.776460 Mouth-OC-1.0.1/Mouth_OC.egg-info/
--rw-rw-r--   0 bast      (1002) bast      (1002)      873 2023-03-21 14:45:36.000000 Mouth-OC-1.0.1/Mouth_OC.egg-info/PKG-INFO
--rw-rw-r--   0 bast      (1002) bast      (1002)      462 2023-03-21 14:45:36.000000 Mouth-OC-1.0.1/Mouth_OC.egg-info/SOURCES.txt
--rw-rw-r--   0 bast      (1002) bast      (1002)        1 2023-03-21 14:45:36.000000 Mouth-OC-1.0.1/Mouth_OC.egg-info/dependency_links.txt
--rw-rw-r--   0 bast      (1002) bast      (1002)       46 2023-03-21 14:45:36.000000 Mouth-OC-1.0.1/Mouth_OC.egg-info/entry_points.txt
--rw-rw-r--   0 bast      (1002) bast      (1002)       61 2023-03-21 14:45:36.000000 Mouth-OC-1.0.1/Mouth_OC.egg-info/requires.txt
--rw-rw-r--   0 bast      (1002) bast      (1002)        6 2023-03-21 14:45:36.000000 Mouth-OC-1.0.1/Mouth_OC.egg-info/top_level.txt
--rw-rw-r--   0 bast      (1002) bast      (1002)        1 2023-01-16 14:54:06.000000 Mouth-OC-1.0.1/Mouth_OC.egg-info/zip-safe
--rw-rw-r--   0 bast      (1002) bast      (1002)      873 2023-03-21 14:45:36.780460 Mouth-OC-1.0.1/PKG-INFO
--rw-rw-r--   0 bast      (1002) bast      (1002)      244 2023-01-10 19:59:12.000000 Mouth-OC-1.0.1/README.md
-drwxrwxr-x   0 bast      (1002) bast      (1002)        0 2023-03-21 14:45:36.776460 Mouth-OC-1.0.1/mouth/
--rw-rw-r--   0 bast      (1002) bast      (1002)    41045 2023-03-21 14:45:07.000000 Mouth-OC-1.0.1/mouth/__init__.py
--rw-rw-r--   0 bast      (1002) bast      (1002)     3716 2023-03-11 19:54:34.000000 Mouth-OC-1.0.1/mouth/__main__.py
-drwxrwxr-x   0 bast      (1002) bast      (1002)        0 2023-03-21 14:45:36.780460 Mouth-OC-1.0.1/mouth/definitions/
--rw-rw-r--   0 bast      (1002) bast      (1002)      892 2023-01-27 13:21:51.000000 Mouth-OC-1.0.1/mouth/definitions/locale.json
--rw-rw-r--   0 bast      (1002) bast      (1002)      922 2023-01-27 13:21:51.000000 Mouth-OC-1.0.1/mouth/definitions/template.json
--rw-rw-r--   0 bast      (1002) bast      (1002)     1257 2023-01-27 13:21:51.000000 Mouth-OC-1.0.1/mouth/definitions/template_email.json
--rw-rw-r--   0 bast      (1002) bast      (1002)     1046 2023-01-27 13:21:51.000000 Mouth-OC-1.0.1/mouth/definitions/template_sms.json
--rw-rw-r--   0 bast      (1002) bast      (1002)      305 2023-01-27 13:21:51.000000 Mouth-OC-1.0.1/mouth/errors.py
--rw-rw-r--   0 bast      (1002) bast      (1002)     3038 2023-01-27 13:21:51.000000 Mouth-OC-1.0.1/mouth/records.py
--rw-rw-r--   0 bast      (1002) bast      (1002)       79 2023-03-21 14:45:36.780460 Mouth-OC-1.0.1/setup.cfg
--rw-rw-r--   0 bast      (1002) bast      (1002)      999 2023-03-21 14:45:07.000000 Mouth-OC-1.0.1/setup.py
+drwxrwxr-x   0 bast      (1002) bast      (1002)        0 2023-03-26 13:22:07.494862 Mouth-OC-1.0.2/
+-rw-rw-r--   0 bast      (1002) bast      (1002)      360 2023-01-10 19:59:34.000000 Mouth-OC-1.0.2/LICENSE
+drwxrwxr-x   0 bast      (1002) bast      (1002)        0 2023-03-26 13:22:07.490862 Mouth-OC-1.0.2/Mouth_OC.egg-info/
+-rw-rw-r--   0 bast      (1002) bast      (1002)      873 2023-03-26 13:22:07.000000 Mouth-OC-1.0.2/Mouth_OC.egg-info/PKG-INFO
+-rw-rw-r--   0 bast      (1002) bast      (1002)      462 2023-03-26 13:22:07.000000 Mouth-OC-1.0.2/Mouth_OC.egg-info/SOURCES.txt
+-rw-rw-r--   0 bast      (1002) bast      (1002)        1 2023-03-26 13:22:07.000000 Mouth-OC-1.0.2/Mouth_OC.egg-info/dependency_links.txt
+-rw-rw-r--   0 bast      (1002) bast      (1002)       46 2023-03-26 13:22:07.000000 Mouth-OC-1.0.2/Mouth_OC.egg-info/entry_points.txt
+-rw-rw-r--   0 bast      (1002) bast      (1002)       61 2023-03-26 13:22:07.000000 Mouth-OC-1.0.2/Mouth_OC.egg-info/requires.txt
+-rw-rw-r--   0 bast      (1002) bast      (1002)        6 2023-03-26 13:22:07.000000 Mouth-OC-1.0.2/Mouth_OC.egg-info/top_level.txt
+-rw-rw-r--   0 bast      (1002) bast      (1002)        1 2023-01-16 14:54:06.000000 Mouth-OC-1.0.2/Mouth_OC.egg-info/zip-safe
+-rw-rw-r--   0 bast      (1002) bast      (1002)      873 2023-03-26 13:22:07.494862 Mouth-OC-1.0.2/PKG-INFO
+-rw-rw-r--   0 bast      (1002) bast      (1002)      244 2023-01-10 19:59:12.000000 Mouth-OC-1.0.2/README.md
+drwxrwxr-x   0 bast      (1002) bast      (1002)        0 2023-03-26 13:22:07.494862 Mouth-OC-1.0.2/mouth/
+-rw-rw-r--   0 bast      (1002) bast      (1002)    41045 2023-03-26 13:20:42.000000 Mouth-OC-1.0.2/mouth/__init__.py
+-rw-rw-r--   0 bast      (1002) bast      (1002)     3716 2023-03-11 19:54:34.000000 Mouth-OC-1.0.2/mouth/__main__.py
+drwxrwxr-x   0 bast      (1002) bast      (1002)        0 2023-03-26 13:22:07.494862 Mouth-OC-1.0.2/mouth/definitions/
+-rw-rw-r--   0 bast      (1002) bast      (1002)      892 2023-01-27 13:21:51.000000 Mouth-OC-1.0.2/mouth/definitions/locale.json
+-rw-rw-r--   0 bast      (1002) bast      (1002)      922 2023-01-27 13:21:51.000000 Mouth-OC-1.0.2/mouth/definitions/template.json
+-rw-rw-r--   0 bast      (1002) bast      (1002)     1257 2023-01-27 13:21:51.000000 Mouth-OC-1.0.2/mouth/definitions/template_email.json
+-rw-rw-r--   0 bast      (1002) bast      (1002)     1046 2023-01-27 13:21:51.000000 Mouth-OC-1.0.2/mouth/definitions/template_sms.json
+-rw-rw-r--   0 bast      (1002) bast      (1002)      305 2023-01-27 13:21:51.000000 Mouth-OC-1.0.2/mouth/errors.py
+-rw-rw-r--   0 bast      (1002) bast      (1002)     3038 2023-01-27 13:21:51.000000 Mouth-OC-1.0.2/mouth/records.py
+-rw-rw-r--   0 bast      (1002) bast      (1002)       79 2023-03-26 13:22:07.494862 Mouth-OC-1.0.2/setup.cfg
+-rw-rw-r--   0 bast      (1002) bast      (1002)      999 2023-03-26 13:17:58.000000 Mouth-OC-1.0.2/setup.py
```

### Comparing `Mouth-OC-1.0.1/Mouth_OC.egg-info/PKG-INFO` & `Mouth-OC-1.0.2/Mouth_OC.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Mouth-OC
-Version: 1.0.1
+Version: 1.0.2
 Summary: Mouth contains a service to run outgoing communications like email and sms messages
 Home-page: https://ouroboroscoding.com/body/mouth
 Author: Chris Nasr - Ouroboros Coding Inc.
 Author-email: chris@ouroboroscoding.com
 License: Custom
 Project-URL: Documentation, https://ouroboroscoding.com/body/mouth
 Project-URL: Source, https://github.com/ouroboroscoding/mouth
```

### Comparing `Mouth-OC-1.0.1/PKG-INFO` & `Mouth-OC-1.0.2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Mouth-OC
-Version: 1.0.1
+Version: 1.0.2
 Summary: Mouth contains a service to run outgoing communications like email and sms messages
 Home-page: https://ouroboroscoding.com/body/mouth
 Author: Chris Nasr - Ouroboros Coding Inc.
 Author-email: chris@ouroboroscoding.com
 License: Custom
 Project-URL: Documentation, https://ouroboroscoding.com/body/mouth
 Project-URL: Source, https://github.com/ouroboroscoding/mouth
```

### Comparing `Mouth-OC-1.0.1/mouth/__init__.py` & `Mouth-OC-1.0.2/mouth/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -157,21 +157,21 @@
 
 				# If we didn't get a dictionary
 				if not isinstance(opts['attachments'][i], dict):
 					return Services.Error(errors.ATTACHMENT_STRUCTURE, 'attachments.[%d]' % i)
 
 				# If the fields are missing
 				try:
-					DictHelper.eval(opts['attachments'][i], ['data', 'filename'])
+					DictHelper.eval(opts['attachments'][i], ['body', 'filename'])
 				except ValueError as e:
 					return Services.Error(body.errors.DATA_FIELDS, [['attachments.[%d].%s' % (i, s), 'invalid'] for s in e.args])
 
 				# Try to decode the base64
 				try:
-					opts['attachments'][i]['data'] = b64decode(opts['attachments'][i]['data'])
+					opts['attachments'][i]['body'] = b64decode(opts['attachments'][i]['body'])
 				except TypeError:
 					return Services.Response(errors.ATTACHMENT_DECODE)
 
 			# Set the attachments from the opts
 			mAttachments = opts['attachments']
 
 		# Only send if anyone is allowed, or the to is in the allowed
```

### Comparing `Mouth-OC-1.0.1/mouth/__main__.py` & `Mouth-OC-1.0.2/mouth/__main__.py`

 * *Files identical despite different names*

### Comparing `Mouth-OC-1.0.1/mouth/definitions/locale.json` & `Mouth-OC-1.0.2/mouth/definitions/locale.json`

 * *Files identical despite different names*

### Comparing `Mouth-OC-1.0.1/mouth/definitions/template.json` & `Mouth-OC-1.0.2/mouth/definitions/template.json`

 * *Files identical despite different names*

### Comparing `Mouth-OC-1.0.1/mouth/definitions/template_email.json` & `Mouth-OC-1.0.2/mouth/definitions/template_email.json`

 * *Files identical despite different names*

### Comparing `Mouth-OC-1.0.1/mouth/definitions/template_sms.json` & `Mouth-OC-1.0.2/mouth/definitions/template_sms.json`

 * *Files identical despite different names*

### Comparing `Mouth-OC-1.0.1/mouth/records.py` & `Mouth-OC-1.0.2/mouth/records.py`

 * *Files identical despite different names*

### Comparing `Mouth-OC-1.0.1/setup.py` & `Mouth-OC-1.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open('README.md', 'r') as oF:
 	long_description=oF.read()
 
 setup(
 	name='Mouth-OC',
-	version='1.0.1',
+	version='1.0.2',
 	description='Mouth contains a service to run outgoing communications like email and sms messages',
 	long_description=long_description,
 	long_description_content_type='text/markdown',
 	url='https://ouroboroscoding.com/body/mouth',
 	project_urls={
 		'Documentation': 'https://ouroboroscoding.com/body/mouth',
 		'Source': 'https://github.com/ouroboroscoding/mouth',
@@ -21,15 +21,15 @@
 	license='Custom',
 	packages=['mouth'],
 	package_data={'mouth': ['definitions/*.json']},
 	python_requires='>=3.10',
 	install_requires=[
 		'Rest-OC>=1.1.1',
 		'Body-OC>=1.0.1',
-		'Brain-OC>=1.0.0',
+		'Brain-OC>=1.0.1',
 		'twilio==7.16.1'
 	],
 	entry_points={
 		'console_scripts': ['mouth=mouth.__main__:cli']
 	},
 	zip_safe=True
 )
```

