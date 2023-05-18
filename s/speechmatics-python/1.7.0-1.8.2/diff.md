# Comparing `tmp/speechmatics-python-1.7.0.tar.gz` & `tmp/speechmatics-python-1.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "speechmatics-python-1.7.0.tar", last modified: Wed Mar  1 14:57:14 2023, max compression
+gzip compressed data, was "speechmatics-python-1.8.2.tar", last modified: Thu May 18 18:45:48 2023, max compression
```

## Comparing `speechmatics-python-1.7.0.tar` & `speechmatics-python-1.8.2.tar`

### file list

```diff
@@ -1,39 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 14:57:14.513603 speechmatics-python-1.7.0/
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-03-01 14:57:04.000000 speechmatics-python-1.7.0/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (123)     6646 2023-03-01 14:57:04.000000 speechmatics-python-1.7.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-03-01 14:57:04.000000 speechmatics-python-1.7.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-03-01 14:57:04.000000 speechmatics-python-1.7.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     8660 2023-03-01 14:57:14.513603 speechmatics-python-1.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7707 2023-03-01 14:57:04.000000 speechmatics-python-1.7.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-03-01 14:57:04.000000 speechmatics-python-1.7.0/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)      213 2023-03-01 14:57:04.000000 speechmatics-python-1.7.0/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-03-01 14:57:04.000000 speechmatics-python-1.7.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-03-01 14:57:14.513603 speechmatics-python-1.7.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2583 2023-03-01 14:57:04.000000 speechmatics-python-1.7.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 14:57:14.513603 speechmatics-python-1.7.0/speechmatics/
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-03-01 14:57:04.000000 speechmatics-python-1.7.0/speechmatics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5509 2023-03-01 14:57:04.000000 speechmatics-python-1.7.0/speechmatics/adapters.py
--rw-r--r--   0 runner    (1001) docker     (123)    12309 2023-03-01 14:57:04.000000 speechmatics-python-1.7.0/speechmatics/batch_client.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    23781 2023-03-01 14:57:04.000000 speechmatics-python-1.7.0/speechmatics/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    16617 2023-03-01 14:57:04.000000 speechmatics-python-1.7.0/speechmatics/cli_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)    18065 2023-03-01 14:57:04.000000 speechmatics-python-1.7.0/speechmatics/client.py
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-03-01 14:57:04.000000 speechmatics-python-1.7.0/speechmatics/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)      577 2023-03-01 14:57:04.000000 speechmatics-python-1.7.0/speechmatics/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3398 2023-03-01 14:57:04.000000 speechmatics-python-1.7.0/speechmatics/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    10911 2023-03-01 14:57:04.000000 speechmatics-python-1.7.0/speechmatics/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 14:57:14.513603 speechmatics-python-1.7.0/speechmatics_python.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8660 2023-03-01 14:57:14.000000 speechmatics-python-1.7.0/speechmatics_python.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      790 2023-03-01 14:57:14.000000 speechmatics-python-1.7.0/speechmatics_python.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-01 14:57:14.000000 speechmatics-python-1.7.0/speechmatics_python.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-03-01 14:57:14.000000 speechmatics-python-1.7.0/speechmatics_python.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-03-01 14:57:14.000000 speechmatics-python-1.7.0/speechmatics_python.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-03-01 14:57:14.000000 speechmatics-python-1.7.0/speechmatics_python.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 14:57:14.513603 speechmatics-python-1.7.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-01 14:57:04.000000 speechmatics-python-1.7.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2178 2023-03-01 14:57:04.000000 speechmatics-python-1.7.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     8782 2023-03-01 14:57:05.000000 speechmatics-python-1.7.0/tests/mock_rt_server.py
--rw-r--r--   0 runner    (1001) docker     (123)     2161 2023-03-01 14:57:05.000000 speechmatics-python-1.7.0/tests/test_adapters.py
--rw-r--r--   0 runner    (1001) docker     (123)    30186 2023-03-01 14:57:05.000000 speechmatics-python-1.7.0/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    21224 2023-03-01 14:57:05.000000 speechmatics-python-1.7.0/tests/test_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-03-01 14:57:05.000000 speechmatics-python-1.7.0/tests/test_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1533 2023-03-01 14:57:05.000000 speechmatics-python-1.7.0/tests/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 18:45:48.554819 speechmatics-python-1.8.2/
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-18 18:45:37.000000 speechmatics-python-1.8.2/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (123)     7293 2023-05-18 18:45:37.000000 speechmatics-python-1.8.2/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-05-18 18:45:37.000000 speechmatics-python-1.8.2/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-05-18 18:45:37.000000 speechmatics-python-1.8.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     8245 2023-05-18 18:45:48.554819 speechmatics-python-1.8.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7292 2023-05-18 18:45:37.000000 speechmatics-python-1.8.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-18 18:45:37.000000 speechmatics-python-1.8.2/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-05-18 18:45:37.000000 speechmatics-python-1.8.2/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-18 18:45:37.000000 speechmatics-python-1.8.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-05-18 18:45:48.554819 speechmatics-python-1.8.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2583 2023-05-18 18:45:37.000000 speechmatics-python-1.8.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 18:45:48.550819 speechmatics-python-1.8.2/speechmatics/
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-05-18 18:45:37.000000 speechmatics-python-1.8.2/speechmatics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6378 2023-05-18 18:45:37.000000 speechmatics-python-1.8.2/speechmatics/adapters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12309 2023-05-18 18:45:37.000000 speechmatics-python-1.8.2/speechmatics/batch_client.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    28866 2023-05-18 18:45:37.000000 speechmatics-python-1.8.2/speechmatics/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18838 2023-05-18 18:45:37.000000 speechmatics-python-1.8.2/speechmatics/cli_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18426 2023-05-18 18:45:37.000000 speechmatics-python-1.8.2/speechmatics/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-05-18 18:45:37.000000 speechmatics-python-1.8.2/speechmatics/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      577 2023-05-18 18:45:37.000000 speechmatics-python-1.8.2/speechmatics/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3398 2023-05-18 18:45:37.000000 speechmatics-python-1.8.2/speechmatics/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12710 2023-05-18 18:45:37.000000 speechmatics-python-1.8.2/speechmatics/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 18:45:48.554819 speechmatics-python-1.8.2/speechmatics_python.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8245 2023-05-18 18:45:48.000000 speechmatics-python-1.8.2/speechmatics_python.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      817 2023-05-18 18:45:48.000000 speechmatics-python-1.8.2/speechmatics_python.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 18:45:48.000000 speechmatics-python-1.8.2/speechmatics_python.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-18 18:45:48.000000 speechmatics-python-1.8.2/speechmatics_python.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-18 18:45:48.000000 speechmatics-python-1.8.2/speechmatics_python.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-18 18:45:48.000000 speechmatics-python-1.8.2/speechmatics_python.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 18:45:48.554819 speechmatics-python-1.8.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 18:45:37.000000 speechmatics-python-1.8.2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2178 2023-05-18 18:45:37.000000 speechmatics-python-1.8.2/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8782 2023-05-18 18:45:37.000000 speechmatics-python-1.8.2/tests/mock_rt_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2161 2023-05-18 18:45:37.000000 speechmatics-python-1.8.2/tests/test_adapters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24250 2023-05-18 18:45:37.000000 speechmatics-python-1.8.2/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8711 2023-05-18 18:45:37.000000 speechmatics-python-1.8.2/tests/test_cli_handlers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21224 2023-05-18 18:45:37.000000 speechmatics-python-1.8.2/tests/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2640 2023-05-18 18:45:37.000000 speechmatics-python-1.8.2/tests/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1533 2023-05-18 18:45:37.000000 speechmatics-python-1.8.2/tests/utils.py
```

### Comparing `speechmatics-python-1.7.0/CHANGELOG.md` & `speechmatics-python-1.8.2/CHANGELOG.md`

 * *Files 5% similar despite different names*

```diff
@@ -3,14 +3,46 @@
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
 ## [Unreleased]
 
+## [1.8.2]
+
+### Fixed
+
+- TranscriptionConfig.enable_partials defaults to False
+
+## [1.8.1]
+
+### Fixed
+
+- setting TranscriptionConfig.enable_partials bool value to a string raises exception
+
+### Added
+
+- Support for batch and realtime urls in config .toml files
+
+## [1.8.0]
+
+### Added
+
+- Added support for real-time translation
+- Added `--enable-translation-partials` to enable partials for translation only
+- Added `--enable-transcription-partials` to enable partials for transcription only
+
+### Changed
+
+- Updated `--enable-partials` to enable partials for both transcription and translation
+
+### Added
+
+- Add support for multiple profiles to the CLI tool
+
 ## [1.7.0] - 2023-03-01
 
 ### Added
 
 - Add support for language identification
 
 ### Fixed
@@ -42,15 +74,15 @@
 
 - Fix inconsistency in docs
 
 ## [1.6.0] - 2023-02-02
 
 ### Added
 
-- Add support for translation (DEL-9547)
+- Add support for translation
 
 ### Changed
 
 - Raises ConnectionClosedException rather than returning when the websocket connection closes unexpectedly
 
 ## [1.5.1] - 2023-01-17
```

### Comparing `speechmatics-python-1.7.0/LICENSE.txt` & `speechmatics-python-1.8.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `speechmatics-python-1.7.0/PKG-INFO` & `speechmatics-python-1.8.2/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: speechmatics-python
-Version: 1.7.0
+Version: 1.8.2
 Summary: Python library and CLI for Speechmatics
 Home-page: https://github.com/speechmatics/speechmatics-python/
 Author: Speechmatics
 Author-email: support@speechmatics.com
 License: MIT
 Project-URL: Documentation, https://speechmatics.github.io/speechmatics-python/
 Project-URL: Source Code, https://github.com/speechmatics/speechmatics-python/
@@ -17,15 +17,15 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Topic :: Multimedia :: Sound/Audio :: Speech
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
-# speechmatics-python &ensp; ![Tests](https://github.com/speechmatics/speechmatics-python/workflows/Tests/badge.svg) [![codecov](https://codecov.io/gh/speechmatics/speechmatics-python/branch/master/graph/badge.svg)](https://codecov.io/gh/speechmatics/speechmatics-python) [![License](https://img.shields.io/badge/license-MIT-yellow.svg)](https://github.com/speechmatics/speechmatics-python/blob/master/LICENSE.txt)
+# speechmatics-python &ensp; ![Tests](https://github.com/speechmatics/speechmatics-python/workflows/Tests/badge.svg) [![License](https://img.shields.io/badge/license-MIT-yellow.svg)](https://github.com/speechmatics/speechmatics-python/blob/master/LICENSE.txt)
 
 Python client library and CLI for Speechmatics Realtime and Batch ASR v2 APIs.
 
 
 ## Getting started
 
 To install from PyPI:
@@ -78,14 +78,24 @@
    ```
 
 - Unsetting generate temp token globally for CLI authentication:
    ```shell
    $ speechmatics config unset --generate-temp-token
    ```
 
+- Setting URLs for connecting to transcribers. These values can be used in places of the --url flag:
+   ```shell
+   $ speechmatics config set --rt-url wss://eu2.rt.speechmatics.com/v2 --batch-url https://asr.api.speechmatics.com/v2
+   ```
+
+- Unsetting transcriber URLs in the toml config:
+   ```shell
+   $ speechmatics config unset --rt-url --batch-url
+   ```
+
   ### Realtime ASR
 - Starting a real-time session for self-service SaaS customers using a .wav file as the input audio:
 
    ```shell
    $ speechmatics transcribe --lang en --generate-temp-token example_audio.wav
    ```
 
@@ -198,24 +208,14 @@
    $ speechmatics batch transcribe --language auto --langid-langs en,es example_audio.wav
     ```
     If Speechmatics is not able to identify a language with high enough confidence,  the job will be rejected. This is to reduce the risk of transcribing incorrectly.
    
     `--langid-langs` is optional and specifies what language(s) you expect to be detected in the source files.
 
 
-- Submit a job with translation (translation output only available as JSON)
-
-    ```shell
-   $ speechmatics batch transcribe --translation-langs de,es --output-format json-v2 example_audio.wav
-    ```
-  `--translation-langs` is supported in asynchronous mode as well, and translation output can be retrieved using `get-results` with `--output-format json-v2` set.
-  
-  When combining language identification with translation, we can't know if the identified language can be translated
-  to your translation targets. If the translation pair is not supported, the error will be recorded in the metadata of the transcript.
-
   ### Custom Transcription Config File
 - Instead of passing all the transcription options via the command line you can also pass a transcription config file.
   The config file is a JSON file that contains the transcription options.
   The config file can be passed to the CLI using the `--config-file` option.
 
     ```shell
   $ speechmatics transcribe --config-file transcription_config.json example_audio.wav
```

### Comparing `speechmatics-python-1.7.0/README.md` & `speechmatics-python-1.8.2/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# speechmatics-python &ensp; ![Tests](https://github.com/speechmatics/speechmatics-python/workflows/Tests/badge.svg) [![codecov](https://codecov.io/gh/speechmatics/speechmatics-python/branch/master/graph/badge.svg)](https://codecov.io/gh/speechmatics/speechmatics-python) [![License](https://img.shields.io/badge/license-MIT-yellow.svg)](https://github.com/speechmatics/speechmatics-python/blob/master/LICENSE.txt)
+# speechmatics-python &ensp; ![Tests](https://github.com/speechmatics/speechmatics-python/workflows/Tests/badge.svg) [![License](https://img.shields.io/badge/license-MIT-yellow.svg)](https://github.com/speechmatics/speechmatics-python/blob/master/LICENSE.txt)
 
 Python client library and CLI for Speechmatics Realtime and Batch ASR v2 APIs.
 
 
 ## Getting started
 
 To install from PyPI:
@@ -55,14 +55,24 @@
    ```
 
 - Unsetting generate temp token globally for CLI authentication:
    ```shell
    $ speechmatics config unset --generate-temp-token
    ```
 
+- Setting URLs for connecting to transcribers. These values can be used in places of the --url flag:
+   ```shell
+   $ speechmatics config set --rt-url wss://eu2.rt.speechmatics.com/v2 --batch-url https://asr.api.speechmatics.com/v2
+   ```
+
+- Unsetting transcriber URLs in the toml config:
+   ```shell
+   $ speechmatics config unset --rt-url --batch-url
+   ```
+
   ### Realtime ASR
 - Starting a real-time session for self-service SaaS customers using a .wav file as the input audio:
 
    ```shell
    $ speechmatics transcribe --lang en --generate-temp-token example_audio.wav
    ```
 
@@ -175,24 +185,14 @@
    $ speechmatics batch transcribe --language auto --langid-langs en,es example_audio.wav
     ```
     If Speechmatics is not able to identify a language with high enough confidence,  the job will be rejected. This is to reduce the risk of transcribing incorrectly.
    
     `--langid-langs` is optional and specifies what language(s) you expect to be detected in the source files.
 
 
-- Submit a job with translation (translation output only available as JSON)
-
-    ```shell
-   $ speechmatics batch transcribe --translation-langs de,es --output-format json-v2 example_audio.wav
-    ```
-  `--translation-langs` is supported in asynchronous mode as well, and translation output can be retrieved using `get-results` with `--output-format json-v2` set.
-  
-  When combining language identification with translation, we can't know if the identified language can be translated
-  to your translation targets. If the translation pair is not supported, the error will be recorded in the metadata of the transcript.
-
   ### Custom Transcription Config File
 - Instead of passing all the transcription options via the command line you can also pass a transcription config file.
   The config file is a JSON file that contains the transcription options.
   The config file can be passed to the CLI using the `--config-file` option.
 
     ```shell
   $ speechmatics transcribe --config-file transcription_config.json example_audio.wav
```

### Comparing `speechmatics-python-1.7.0/setup.py` & `speechmatics-python-1.8.2/setup.py`

 * *Files identical despite different names*

### Comparing `speechmatics-python-1.7.0/speechmatics/adapters.py` & `speechmatics-python-1.8.2/speechmatics/adapters.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,38 @@
 # (c) 2020, Cantab Research Ltd.
 """
 Functions for converting our JSON transcription results to other formats.
 """
 from typing import Any, List
 
 
+def get_txt_translation(translations: List[dict]):
+    """
+    Extract translation content and speaker labels to plain text format.
+
+    :param translations: list of dicts containing translation content.
+    :return: the plain text as a string.
+    """
+    sentences = []
+    current_speaker = None
+    for translation in translations:
+        sentence_delimiter = " "
+        if translation.get("content", None):
+            if (
+                translation.get("speaker", None)
+                and translation.get("speaker") != current_speaker
+            ):
+                current_speaker = translation["speaker"]
+                sentences.append(f"SPEAKER: {current_speaker}\n")
+                sentence_delimiter = "\n"
+            sentences.append(translation["content"])
+            sentences.append(sentence_delimiter)
+    return "".join(sentences).rstrip()
+
+
 def convert_to_txt(
     tokens: List[dict],
     language: str,
     language_pack_info: dict = None,
     speaker_labels: bool = True,
     speaker_change_token: bool = False,
 ) -> str:
```

### Comparing `speechmatics-python-1.7.0/speechmatics/batch_client.py` & `speechmatics-python-1.8.2/speechmatics/batch_client.py`

 * *Files identical despite different names*

### Comparing `speechmatics-python-1.7.0/speechmatics/cli.py` & `speechmatics-python-1.8.2/speechmatics/cli.py`

 * *Files 13% similar despite different names*

```diff
@@ -31,15 +31,15 @@
     AudioSettings,
     ClientMessageType,
     ServerMessageType,
     ConnectionSettings,
     BatchTranscriptionConfig,
     BatchSpeakerDiarizationConfig,
     RTSpeakerDiarizationConfig,
-    BatchTranslationConfig,
+    RTTranslationConfig,
     BatchLanguageIdentificationConfig,
 )
 from speechmatics.cli_parser import (
     parse_args,
 )
 from speechmatics.constants import (
     BATCH_SELF_SERVICE_URL,
@@ -137,28 +137,45 @@
     :type args: dict
 
     :return: Settings for the WebSocket connection.
     :rtype: speechmatics.models.ConnectionSettings
     """
     auth_token = args.get("auth_token")
     generate_temp_token = args.get("generate_temp_token")
+    url = args.get("url")
 
     home_directory = os.path.expanduser("~")
     if os.path.exists(f"{home_directory}/.speechmatics/config"):
         cli_config = {"default": {}}
         with open(
             f"{home_directory}/.speechmatics/config", "r", encoding="UTF-8"
         ) as file:
             cli_config = toml.load(file)
-        if cli_config["default"].get("auth_token") is not None and auth_token is None:
-            auth_token = cli_config["default"].get("auth_token", None)
-        if generate_temp_token is None:
-            generate_temp_token = cli_config["default"].get("generate_temp_token")
+        profile = args.get("profile", "default")
+        if profile not in cli_config:
+            raise SystemExit(
+                f"Cannot unset config for profile {profile}. Profile does not exist."
+            )
+        if "auth_token" in cli_config[profile] and auth_token is None:
+            auth_token = cli_config[profile].get("auth_token")
+        if "generate_temp_token" in cli_config[profile]:
+            generate_temp_token = cli_config[profile].get("generate_temp_token")
+        if (
+            url is None
+            and args.get("mode") == "batch"
+            and "batch_url" in cli_config[profile]
+        ):
+            url = cli_config[profile].get("batch_url")
+        if (
+            url is None
+            and args.get("mode") == "rt"
+            and "realtime_url" in cli_config[profile]
+        ):
+            url = cli_config[profile].get("realtime_url")
 
-    url = args.get("url", None)
     if url is None:
         if args.get("mode") == "batch":
             url = BATCH_SELF_SERVICE_URL
         else:
             url = f"{RT_SELF_SERVICE_URL}/{lang}"
 
     settings = ConnectionSettings(
@@ -218,14 +235,16 @@
         "speaker_diarization_sensitivity",
     ]:
         if args.get(option) is not None:
             config[option] = args[option]
     for option in [
         "enable_partials",
         "enable_entities",
+        "enable_translation_partials",
+        "enable_transcription_partials",
     ]:
         config[option] = True if args.get(option) else config.get(option)
 
     if args.get("additional_vocab_file"):
         additional_vocab = parse_additional_vocab(args["additional_vocab_file"])
         config["additional_vocab"] = additional_vocab
         LOGGER.info(
@@ -265,16 +284,20 @@
         speaker_sensitivity = args.get("speaker_diarization_sensitivity")
         config["speaker_diarization_config"] = BatchSpeakerDiarizationConfig(
             speaker_sensitivity=speaker_sensitivity
         )
 
     if args.get("translation_target_languages") is not None:
         translation_target_languages = args.get("translation_target_languages")
-        config["translation_config"] = BatchTranslationConfig(
-            target_languages=translation_target_languages.split(",")
+        enable_partials = args.get("enable_partials", False) or args.get(
+            "enable_translation_partials", False
+        )
+        config["translation_config"] = RTTranslationConfig(
+            target_languages=translation_target_languages.split(","),
+            enable_partials=enable_partials,
         )
 
     if args.get("langid_expected_languages") is not None:
         langid_expected_languages = args.get("langid_expected_languages")
         config["language_identification_config"] = BatchLanguageIdentificationConfig(
             expected_languages=langid_expected_languages.split(",")
         )
@@ -302,39 +325,51 @@
         sample_rate=args["sample_rate"],
         chunk_size=args["chunk_size"],
         encoding=args["raw"],
     )
     return settings
 
 
-# pylint: disable=too-many-arguments
+# pylint: disable=too-many-arguments,too-many-statements
 def add_printing_handlers(
     api,
     transcripts,
     enable_partials=False,
+    enable_transcription_partials=False,
+    enable_translation_partials=False,
     debug_handlers_too=False,
     speaker_change_token=False,
     print_json=False,
+    translation_config=None,
 ):
     """
     Adds a set of handlers to the websocket client which print out transcripts
     as they are received. This includes partials if they are enabled.
 
     Args:
         api (speechmatics.client.WebsocketClient): Client instance.
         transcripts (Transcripts): Allows the transcripts to be concatenated to
             produce a final result.
-        enable_partials (bool, optional): Whether or not partials are enabled.
-        debug_handlers_too (bool, optional): Whether or not to enable 'debug'
+        enable_partials (bool, optional): Whether partials are enabled
+            for both transcription and translation.
+        enable_transcription_partials (bool, optional): Whether partials are enabled
+            for transcription only.
+        enable_translation_partials (bool, optional): Whether partials are enabled
+            for translation only.
+        debug_handlers_too (bool, optional): Whether to enable 'debug'
             handlers that print out an ASCII symbol representing messages being
             received and sent.
         speaker_change_token (bool, optional): Whether to explicitly include a
             speaker change token '<sc>' in the output to indicate speaker
             changes.
+        print_json (bool, optional): Whether to print json transcript messages.
+        translation_config (TranslationConfig, optional): Translation config with target languages.
     """
+    escape_seq = "\33[2K" if sys.stdout.isatty() else ""
+
     if debug_handlers_too:
         api.add_event_handler(
             ServerMessageType.AudioAdded, lambda *args: print_symbol("-")
         )
         api.add_event_handler(
             ServerMessageType.AddPartialTranscript, lambda *args: print_symbol(".")
         )
@@ -352,15 +387,14 @@
             message["results"],
             api.transcription_config.language,
             language_pack_info=api.get_language_pack_info(),
             speaker_labels=True,
             speaker_change_token=speaker_change_token,
         )
         if plaintext:
-            escape_seq = "\33[2K" if sys.stderr.isatty() else ""
             sys.stderr.write(f"{escape_seq}{plaintext}\r")
 
     def transcript_handler(message):
         transcripts.json.append(message)
         if print_json:
             print(json.dumps(message))
             return
@@ -368,28 +402,78 @@
             message["results"],
             api.transcription_config.language,
             language_pack_info=api.get_language_pack_info(),
             speaker_labels=True,
             speaker_change_token=speaker_change_token,
         )
         if plaintext:
-            escape_seq = "\33[2K" if sys.stdout.isatty() else ""
             sys.stdout.write(f"{escape_seq}{plaintext}\n")
         transcripts.text += plaintext
 
+    def partial_translation_handler(message):
+        if print_json:
+            print(json.dumps(message))
+            return
+        # Translations for all requested languages should be available
+        # but, we're only going to print one translation
+        if translation_config.target_languages[0] == message["language"]:
+            plaintext = speechmatics.adapters.get_txt_translation(message["results"])
+            sys.stderr.write(f"{escape_seq}{plaintext}\r")
+
+    def translation_handler(message):
+        transcripts.json.append(message)
+        if print_json:
+            print(json.dumps(message))
+            return
+        # Translations for all requested languages should be available
+        # but, we're only going to print one translation
+        if translation_config.target_languages[0] == message["language"]:
+            plaintext = speechmatics.adapters.get_txt_translation(message["results"])
+            if plaintext:
+                sys.stdout.write(f"{escape_seq}{plaintext}\n")
+            transcripts.text += plaintext
+
     def end_of_transcript_handler(_):
         if enable_partials:
             print("\n", file=sys.stderr)
 
-    api.add_event_handler(
-        ServerMessageType.AddPartialTranscript, partial_transcript_handler
-    )
-    api.add_event_handler(ServerMessageType.AddTranscript, transcript_handler)
     api.add_event_handler(ServerMessageType.EndOfTranscript, end_of_transcript_handler)
 
+    # print both transcription and translation messages (if json was requested)
+    # print translation (if text was requested then)
+    # print transcription (if text was requested without translation)
+    if print_json:
+        if enable_partials or enable_translation_partials:
+            api.add_event_handler(
+                ServerMessageType.AddPartialTranslation,
+                partial_translation_handler,
+            )
+        api.add_event_handler(ServerMessageType.AddTranslation, translation_handler)
+        if enable_partials or enable_transcription_partials:
+            api.add_event_handler(
+                ServerMessageType.AddPartialTranscript,
+                partial_transcript_handler,
+            )
+        api.add_event_handler(ServerMessageType.AddTranscript, transcript_handler)
+    else:
+        if translation_config is not None:
+            if enable_partials or enable_translation_partials:
+                api.add_event_handler(
+                    ServerMessageType.AddPartialTranslation,
+                    partial_translation_handler,
+                )
+            api.add_event_handler(ServerMessageType.AddTranslation, translation_handler)
+        else:
+            if enable_partials or enable_transcription_partials:
+                api.add_event_handler(
+                    ServerMessageType.AddPartialTranscript,
+                    partial_transcript_handler,
+                )
+            api.add_event_handler(ServerMessageType.AddTranscript, transcript_handler)
+
 
 def join_words(words, language="en"):
     """
     Joins a list of words with a language specific separator. Because not all
     languages use the standard English white-space between words.
 
     :param words: List of words
@@ -447,15 +531,15 @@
 # pylint: disable=too-many-branches
 # pylint: disable=too-many-statements
 def main(args=None):
     """
     Main entrypoint.
 
     :param args: command-line arguments; defaults to None in which
-            case arguments will retrieved from `sys.argv` (this is useful
+            case arguments will be retrieved from `sys.argv` (this is useful
             mainly for unit tests).
     :type args: List[str]
     """
     if not args:
         args = vars(parse_args())
 
     mode = args["mode"]
@@ -543,23 +627,26 @@
         )
 
     transcripts = Transcripts(text="", json=[])
     add_printing_handlers(
         api,
         transcripts,
         enable_partials=args["enable_partials"],
+        enable_transcription_partials=args["enable_transcription_partials"],
+        enable_translation_partials=args["enable_translation_partials"],
         debug_handlers_too=args["debug"],
         speaker_change_token=args["speaker_change_token"],
         print_json=args["print_json"],
+        translation_config=transcription_config.translation_config,
     )
 
     def run(stream):
         try:
             api.run_synchronously(
-                stream, get_transcription_config(args), get_audio_settings(args)
+                stream, transcription_config, get_audio_settings(args)
             )
         except KeyboardInterrupt:
             # Gracefully handle Ctrl-C, else we get a huge stack-trace.
             LOGGER.warning("Keyboard interrupt received.")
 
     if args["files"][0] == "-":
         run(sys.stdin.buffer)
@@ -615,63 +702,97 @@
 
 def config_main(args):
     """Main dispatch for "config" command set
 
     :param args: arguments from parse_args()
     :type args: argparse.Namespace
     """
-    home_directory = os.path.expanduser("~")
     command = args.get("command")
     if command == "set":
-        cli_config = {"default": {}}
-        if os.path.exists(f"{home_directory}/.speechmatics"):
-            if os.path.exists(f"{home_directory}/.speechmatics/config"):
-                with open(
-                    f"{home_directory}/.speechmatics/config", "r", encoding="UTF-8"
-                ) as file:
-                    toml_string = file.read()
-                    cli_config = toml.loads(toml_string)
-        else:
-            os.makedirs(f"{home_directory}/.speechmatics")
+        set_config(args)
+    if command == "unset":
+        unset_config(args)
 
-        if args.get("auth_token"):
-            cli_config["default"]["auth_token"] = args.get("auth_token")
-        if args.get("generate_temp_token"):
-            cli_config["default"]["generate_temp_token"] = True
 
-        with open(
-            f"{home_directory}/.speechmatics/config", "w", encoding="UTF-8"
-        ) as file:
-            toml.dump(cli_config, file)
+def set_config(args):
+    """
+    Function which handles the config set commands, storing values in the toml file.
 
-    if command == "unset":
-        cli_config = {"default": {}}
+    :param args: arguments from parse_args()
+    :type args: argparse.Namespace
+    """
+    home_directory = os.path.expanduser("~")
+    cli_config = {"default": {}}
+    if os.path.exists(f"{home_directory}/.speechmatics"):
+        if os.path.exists(f"{home_directory}/.speechmatics/config"):
+            with open(
+                f"{home_directory}/.speechmatics/config", "r", encoding="UTF-8"
+            ) as file:
+                toml_string = file.read()
+                cli_config = toml.loads(toml_string)
+    else:
+        os.makedirs(f"{home_directory}/.speechmatics")
 
-        if os.path.exists(f"{home_directory}/.speechmatics"):
-            if os.path.exists(f"{home_directory}/.speechmatics/config"):
-                with open(
-                    f"{home_directory}/.speechmatics/config", "r", encoding="UTF-8"
-                ) as file:
-                    toml_string = file.read()
-                    cli_config = toml.loads(toml_string)
-
-                if args.get("auth_token") and cli_config["default"].get("auth_token"):
-                    cli_config["default"].pop("auth_token")
-                if (
-                    args.get("generate_temp_token")
-                    and cli_config["default"].get("generate_temp_token") is not None
-                ):
-                    cli_config["default"].pop("generate_temp_token")
-
-                with open(
-                    f"{home_directory}/.speechmatics/config", "w", encoding="UTF-8"
-                ) as file:
-                    toml.dump(cli_config, file)
-                return
+    profile = args.get("profile", "default")
+    if profile not in cli_config:
+        cli_config[profile] = {}
+    if args.get("auth_token"):
+        cli_config[profile]["auth_token"] = args.get("auth_token")
+    if args.get("generate_temp_token"):
+        cli_config[profile]["generate_temp_token"] = True
+    if args.get("batch_url"):
+        cli_config[profile]["batch_url"] = args.get("batch_url")
+    if args.get("realtime_url"):
+        cli_config[profile]["realtime_url"] = args.get("realtime_url")
 
-        raise SystemExit(
-            f"Unable to remove config. No config file stored found at {home_directory}/.speechmatics/config"
-        )
+    with open(f"{home_directory}/.speechmatics/config", "w", encoding="UTF-8") as file:
+        toml.dump(cli_config, file)
+
+
+def unset_config(args):
+    """
+    Function which handles the config unset commands, removing values from the toml file.
+
+    :param args: arguments from parse_args()
+    :type args: argparse.Namespace
+    """
+    home_directory = os.path.expanduser("~")
+    cli_config = {"default": {}}
+
+    if os.path.exists(f"{home_directory}/.speechmatics"):
+        if os.path.exists(f"{home_directory}/.speechmatics/config"):
+            with open(
+                f"{home_directory}/.speechmatics/config", "r", encoding="UTF-8"
+            ) as file:
+                toml_string = file.read()
+                cli_config = toml.loads(toml_string)
+
+            profile = args.get("profile", "default")
+            if profile not in cli_config:
+                raise SystemExit(
+                    f"Cannot unset config for profile {profile}. Profile does not exist."
+                )
+            if "auth_token" in cli_config[profile] and args.get("auth_token"):
+                cli_config[profile].pop("auth_token")
+            if (
+                args.get("generate_temp_token")
+                and "generate_temp_token" in cli_config[profile]
+            ):
+                cli_config[profile].pop("generate_temp_token")
+            if "batch_url" in cli_config[profile] and args.get("batch_url"):
+                cli_config[profile].pop("batch_url")
+            if "realtime_url" in cli_config[profile] and args.get("realtime_url"):
+                cli_config[profile].pop("realtime_url")
+
+            with open(
+                f"{home_directory}/.speechmatics/config", "w", encoding="UTF-8"
+            ) as file:
+                toml.dump(cli_config, file)
+            return
+
+    raise SystemExit(
+        f"Unable to remove config. No config file stored found at {home_directory}/.speechmatics/config"
+    )
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `speechmatics-python-1.7.0/speechmatics/cli_parser.py` & `speechmatics-python-1.8.2/speechmatics/cli_parser.py`

 * *Files 4% similar despite different names*

```diff
@@ -128,14 +128,23 @@
         action="store_true",
         help=(
             "Automatically generate a temporary token for authentication."
             "Non-enterprise customers must set this to True."
             "Enterprise customers should set this to False."
         ),
     )
+    connection_parser.add_argument(
+        "--profile",
+        default="default",
+        type=str,
+        help=(
+            "Determines the local config toml profile to use."
+            "Profiles can be used to maintain multiple different user accounts and setups locally."
+        ),
+    )
 
     # Parent parser for shared params related to building a job config
     config_parser = argparse.ArgumentParser(add_help=False)
 
     config_parser.add_argument(
         "--config-file",
         dest="config_file",
@@ -264,19 +273,37 @@
     # Parent parser for RT transcribe arguments
     rt_transcribe_command_parser = argparse.ArgumentParser(add_help=False)
     rt_transcribe_command_parser.add_argument(
         "--enable-partials",
         default=False,
         action="store_true",
         help=(
+            "Whether to return partials for both transcripts and translation which can be updated by later,"
+            "final transcripts."
+        ),
+    )
+    rt_transcribe_command_parser.add_argument(
+        "--enable-transcription-partials",
+        default=False,
+        action="store_true",
+        help=(
             "Whether to return partial transcripts which can be updated by later,"
             "final transcripts."
         ),
     )
     rt_transcribe_command_parser.add_argument(
+        "--enable-translation-partials",
+        default=False,
+        action="store_true",
+        help=(
+            "Whether to return partial translation which can be updated by later,"
+            "final translation."
+        ),
+    )
+    rt_transcribe_command_parser.add_argument(
         "--punctuation-sensitivity",
         type=float,
         help="Sensitivity level for advanced punctuation.",
     )
     rt_transcribe_command_parser.add_argument(
         "--speaker-diarization-max-speakers",
         type=int,
@@ -459,32 +486,70 @@
     cli_set_config_parser = cli_config_subparsers.add_parser(
         "set", help="Set config for the local CLI environment."
     )
     cli_set_config_parser.add_argument(
         "--auth-token", type=str, help="Auth token to use as default for all requests."
     )
     cli_set_config_parser.add_argument(
+        "--realtime-url",
+        "--rt-url",
+        type=str,
+        dest="realtime_url",
+        help="Default URL to use for RT transcription. Overriden by the --url flag.",
+    )
+    cli_set_config_parser.add_argument(
+        "--batch-url",
+        type=str,
+        help="Default URL to use for Batch transcription. Overriden by the --url flag.",
+    )
+    cli_set_config_parser.add_argument(
         "--generate-temp-token",
         action="store_true",
         help="Sets generate_temp_token to true in the config file."
         "This will set the --generate-temp-token to true globally wherever it is a valid command line flag.",
     )
-    cli_set_config_parser = cli_config_subparsers.add_parser(
+    cli_set_config_parser.add_argument(
+        "--profile",
+        type=str,
+        default="default",
+        help="Specifies the profile to set the config for."
+        "Profiles can be used to maintain multiple different sets of config locally.",
+    )
+    cli_unset_config_parser = cli_config_subparsers.add_parser(
         "unset", help="Remove specified config values from the CLI config file."
     )
-    cli_set_config_parser.add_argument(
+    cli_unset_config_parser.add_argument(
         "--auth-token",
         action="store_true",
         help="If flag is set, removes the auth token value from the config file.",
     )
-    cli_set_config_parser.add_argument(
+    cli_unset_config_parser.add_argument(
         "--generate-temp-token",
         action="store_true",
         help="If flag is set, removes the generate temp token value from the config file.",
     )
+    cli_unset_config_parser.add_argument(
+        "--profile",
+        type=str,
+        default="default",
+        help="Specifies the profile to unset the config for."
+        "Profiles can be used to maintain multiple different sets of config locally.",
+    )
+    cli_unset_config_parser.add_argument(
+        "--realtime-url",
+        "--rt-url",
+        dest="realtime_url",
+        action="store_true",
+        help="Remove the default URL to use for RT transcription.",
+    )
+    cli_unset_config_parser.add_argument(
+        "--batch-url",
+        action="store_true",
+        help="Remove the default URL to use for Batch transcription.",
+    )
     return parser
 
 
 def parse_args(args=None):
     """
     Parses command-line arguments.
```

### Comparing `speechmatics-python-1.7.0/speechmatics/client.py` & `speechmatics-python-1.8.2/speechmatics/client.py`

 * *Files 5% similar despite different names*

```diff
@@ -45,14 +45,15 @@
 
     # pylint: disable=too-many-instance-attributes
 
     def __init__(self, connection_settings):
         self.connection_settings = connection_settings
         self.websocket = None
         self.transcription_config = None
+        self.translation_config = None
 
         self.event_handlers = {x: [] for x in ServerMessageType}
         self.middlewares = {x: [] for x in ClientMessageType}
 
         self.seq_no = 0
         self.session_running = False
         self._language_pack_info = None
@@ -109,16 +110,18 @@
         """
         Constructs a
         :py:attr:`speechmatics.models.ClientMessageType.SetRecognitionConfig`
         message.
         """
         msg = {
             "message": ClientMessageType.SetRecognitionConfig,
-            "transcription_config": self.transcription_config.asdict(),
+            "transcription_config": self.transcription_config.as_config(),
         }
+        if self.translation_config is not None:
+            msg["translation_config"] = self.translation_config.asdict()
         self._call_middleware(ClientMessageType.SetRecognitionConfig, msg, False)
         return msg
 
     @json_utf8
     def _start_recognition(self, audio_settings):
         """
         Constructs a
@@ -128,16 +131,18 @@
 
         :param audio_settings: Audio settings to use.
         :type audio_settings: speechmatics.models.AudioSettings
         """
         msg = {
             "message": ClientMessageType.StartRecognition,
             "audio_format": audio_settings.asdict(),
-            "transcription_config": self.transcription_config.asdict(),
+            "transcription_config": self.transcription_config.as_config(),
         }
+        if self.translation_config is not None:
+            msg["translation_config"] = self.translation_config.asdict()
         self.session_running = True
         self._call_middleware(ClientMessageType.StartRecognition, msg, False)
         LOGGER.debug(msg)
         return msg
 
     @json_utf8
     def _end_of_stream(self):
@@ -394,14 +399,15 @@
         :param audio_settings: Configuration for the audio stream.
         :type audio_settings: speechmatics.models.AudioSettings
 
         :raises Exception: Can raise any exception returned by the
             consumer/producer tasks.
         """
         self.transcription_config = transcription_config
+        self.translation_config = transcription_config.translation_config
         self.seq_no = 0
         self._language_pack_info = None
         await self._init_synchronization_primitives()
         extra_headers = {}
         if (
             not self.connection_settings.generate_temp_token
             and self.connection_settings.auth_token is not None
```

### Comparing `speechmatics-python-1.7.0/speechmatics/exceptions.py` & `speechmatics-python-1.8.2/speechmatics/exceptions.py`

 * *Files identical despite different names*

### Comparing `speechmatics-python-1.7.0/speechmatics/helpers.py` & `speechmatics-python-1.8.2/speechmatics/helpers.py`

 * *Files identical despite different names*

### Comparing `speechmatics-python-1.7.0/speechmatics/models.py` & `speechmatics-python-1.8.2/speechmatics/models.py`

 * *Files 9% similar despite different names*

```diff
@@ -122,42 +122,63 @@
     """Real-time mode: Speaker diarization config."""
 
     max_speakers: int = None
     """This enforces the maximum number of speakers allowed in a single audio stream."""
 
 
 @dataclass
+class TranslationConfig:
+    """Translation config."""
+
+    target_languages: List[str] = None
+    """Target languages for which translation should be produced."""
+
+    def asdict(self):
+        return asdict(self)
+
+
+@dataclass
+class RTTranslationConfig(TranslationConfig):
+    """Real-time mode: Translation config."""
+
+    enable_partials: bool = False
+    """Indicates if partial translation, where sentences are produced
+    immediately, is enabled."""
+
+
+@dataclass
 class BatchSpeakerDiarizationConfig:
     """Batch mode: Speaker diarization config."""
 
     speaker_sensitivity: float = None
     """The sensitivity of the speaker detection.
     This is a number between 0 and 1, where 0 means least sensitive and 1 means
     most sensitive."""
 
 
 @dataclass
-class BatchTranslationConfig:
+class BatchTranslationConfig(TranslationConfig):
     """Batch mode: Translation config."""
 
-    target_languages: List[str] = None
-    """Target languages for which translation should be produced"""
-
 
 @dataclass
 class BatchLanguageIdentificationConfig:
     """Batch mode: Language identification config."""
 
     expected_languages: List[str] = None
     """Expected languages for language identification"""
 
 
 @dataclass(init=False)
 class TranscriptionConfig(_TranscriptionConfig):
-    """Real-time: Defines transcription parameters."""
+    # pylint: disable=too-many-instance-attributes
+    """
+    Real-time: Defines transcription parameters.
+    The `.as_config()` method removes translation_config and returns it wrapped into a Speechmatics json config.
+    """
 
     max_delay: float = None
     """Maximum acceptable delay."""
 
     max_delay_mode: str = None
     """Determines whether the threshold specified in max_delay can be exceeded
     if a potential entity is detected. Flexible means if a potential entity
@@ -168,16 +189,40 @@
     speaker_diarization_config: RTSpeakerDiarizationConfig = None
     """Configuration for speaker diarization."""
 
     speaker_change_sensitivity: float = None
     """Sensitivity level for speaker change."""
 
     enable_partials: bool = None
-    """Indicates if partial transcription, where words are produced
-    immediately, is enabled. """
+    """Indicates if partials for both transcripts and translation, where words are produced
+    immediately, is enabled."""
+
+    enable_transcription_partials: bool = None
+    """Indicates if partial transcripts, where words are produced
+    immediately, is enabled."""
+
+    enable_translation_partials: bool = None
+    """Indicates if partial translation, where words are produced
+    immediately, is enabled."""
+
+    translation_config: TranslationConfig = None
+    """Optional configuration for translation."""
+
+    def as_config(self):
+        dictionary = self.asdict()
+        dictionary.pop("translation_config", None)
+        dictionary.pop("enable_translation_partials", None)
+        enable_transcription_partials = dictionary.pop(
+            "enable_transcription_partials", False
+        )
+        # set enable_partials to True if either one is True
+        if dictionary.get("enable_partials") is True or enable_transcription_partials:
+            dictionary["enable_partials"] = True
+
+        return dictionary
 
 
 @dataclass(init=False)
 class BatchTranscriptionConfig(_TranscriptionConfig):
     """Batch: Defines transcription parameters for batch requests.
     The `.as_config()` method will return it wrapped into a Speechmatics json config."""
 
@@ -186,15 +231,15 @@
 
     notification_config: NotificationConfig = None
     """Optional configuration for callback notification."""
 
     language_identification_config: BatchLanguageIdentificationConfig = None
     """Optional configuration for language identification."""
 
-    translation_config: BatchTranslationConfig = None
+    translation_config: TranslationConfig = None
     """Optional configuration for translation."""
 
     srt_overrides: SRTOverrides = None
     """Optional configuration for SRT output."""
 
     speaker_diarization_config: BatchSpeakerDiarizationConfig = None
     """The sensitivity of the speaker detection."""
@@ -322,14 +367,22 @@
     """Indicates a partial transcript, which is an incomplete transcript that
     is immediately produced and may change as more context becomes available.
     """
 
     AddTranscript = "AddTranscript"
     """Indicates the final transcript of a part of the audio."""
 
+    AddPartialTranslation = "AddPartialTranslation"
+    """Indicates a partial translation, which is an incomplete translation that
+    is immediately produced and may change as more context becomes available.
+    """
+
+    AddTranslation = "AddTranslation"
+    """Indicates the final translation of a part of the audio."""
+
     EndOfTranscript = "EndOfTranscript"
     """Server response to :py:attr:`ClientMessageType.EndOfStream`,
     after the server has finished sending all :py:attr:`AddTranscript`
     messages."""
 
     Info = "Info"
     """Indicates a generic info message."""
```

### Comparing `speechmatics-python-1.7.0/speechmatics_python.egg-info/PKG-INFO` & `speechmatics-python-1.8.2/speechmatics_python.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: speechmatics-python
-Version: 1.7.0
+Version: 1.8.2
 Summary: Python library and CLI for Speechmatics
 Home-page: https://github.com/speechmatics/speechmatics-python/
 Author: Speechmatics
 Author-email: support@speechmatics.com
 License: MIT
 Project-URL: Documentation, https://speechmatics.github.io/speechmatics-python/
 Project-URL: Source Code, https://github.com/speechmatics/speechmatics-python/
@@ -17,15 +17,15 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Topic :: Multimedia :: Sound/Audio :: Speech
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
-# speechmatics-python &ensp; ![Tests](https://github.com/speechmatics/speechmatics-python/workflows/Tests/badge.svg) [![codecov](https://codecov.io/gh/speechmatics/speechmatics-python/branch/master/graph/badge.svg)](https://codecov.io/gh/speechmatics/speechmatics-python) [![License](https://img.shields.io/badge/license-MIT-yellow.svg)](https://github.com/speechmatics/speechmatics-python/blob/master/LICENSE.txt)
+# speechmatics-python &ensp; ![Tests](https://github.com/speechmatics/speechmatics-python/workflows/Tests/badge.svg) [![License](https://img.shields.io/badge/license-MIT-yellow.svg)](https://github.com/speechmatics/speechmatics-python/blob/master/LICENSE.txt)
 
 Python client library and CLI for Speechmatics Realtime and Batch ASR v2 APIs.
 
 
 ## Getting started
 
 To install from PyPI:
@@ -78,14 +78,24 @@
    ```
 
 - Unsetting generate temp token globally for CLI authentication:
    ```shell
    $ speechmatics config unset --generate-temp-token
    ```
 
+- Setting URLs for connecting to transcribers. These values can be used in places of the --url flag:
+   ```shell
+   $ speechmatics config set --rt-url wss://eu2.rt.speechmatics.com/v2 --batch-url https://asr.api.speechmatics.com/v2
+   ```
+
+- Unsetting transcriber URLs in the toml config:
+   ```shell
+   $ speechmatics config unset --rt-url --batch-url
+   ```
+
   ### Realtime ASR
 - Starting a real-time session for self-service SaaS customers using a .wav file as the input audio:
 
    ```shell
    $ speechmatics transcribe --lang en --generate-temp-token example_audio.wav
    ```
 
@@ -198,24 +208,14 @@
    $ speechmatics batch transcribe --language auto --langid-langs en,es example_audio.wav
     ```
     If Speechmatics is not able to identify a language with high enough confidence,  the job will be rejected. This is to reduce the risk of transcribing incorrectly.
    
     `--langid-langs` is optional and specifies what language(s) you expect to be detected in the source files.
 
 
-- Submit a job with translation (translation output only available as JSON)
-
-    ```shell
-   $ speechmatics batch transcribe --translation-langs de,es --output-format json-v2 example_audio.wav
-    ```
-  `--translation-langs` is supported in asynchronous mode as well, and translation output can be retrieved using `get-results` with `--output-format json-v2` set.
-  
-  When combining language identification with translation, we can't know if the identified language can be translated
-  to your translation targets. If the translation pair is not supported, the error will be recorded in the metadata of the transcript.
-
   ### Custom Transcription Config File
 - Instead of passing all the transcription options via the command line you can also pass a transcription config file.
   The config file is a JSON file that contains the transcription options.
   The config file can be passed to the CLI using the `--config-file` option.
 
     ```shell
   $ speechmatics transcribe --config-file transcription_config.json example_audio.wav
```

### Comparing `speechmatics-python-1.7.0/speechmatics_python.egg-info/SOURCES.txt` & `speechmatics-python-1.8.2/speechmatics_python.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -25,10 +25,11 @@
 speechmatics_python.egg-info/requires.txt
 speechmatics_python.egg-info/top_level.txt
 tests/__init__.py
 tests/conftest.py
 tests/mock_rt_server.py
 tests/test_adapters.py
 tests/test_cli.py
+tests/test_cli_handlers.py
 tests/test_client.py
 tests/test_models.py
 tests/utils.py
```

### Comparing `speechmatics-python-1.7.0/tests/conftest.py` & `speechmatics-python-1.8.2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `speechmatics-python-1.7.0/tests/mock_rt_server.py` & `speechmatics-python-1.8.2/tests/mock_rt_server.py`

 * *Files identical despite different names*

### Comparing `speechmatics-python-1.7.0/tests/test_adapters.py` & `speechmatics-python-1.8.2/tests/test_adapters.py`

 * *Files identical despite different names*

### Comparing `speechmatics-python-1.7.0/tests/test_cli.py` & `speechmatics-python-1.8.2/tests/test_cli.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 import argparse
 import collections
-import copy
 import logging
 import os
-import sys
 
 import pytest
 import toml
 
 from speechmatics import cli
 from speechmatics import cli_parser
 from speechmatics.constants import (
@@ -127,14 +125,22 @@
         (
             ["batch", "transcribe", "--operating-point=enhanced"],
             {"operating_point": "enhanced"},
         ),
         (["rt", "transcribe", "--ssl-mode=insecure"], {"ssl_mode": "insecure"}),
         (["rt", "transcribe", "--ssl-mode=none"], {"ssl_mode": "none"}),
         (["rt", "transcribe", "--enable-partials"], {"enable_partials": True}),
+        (
+            ["rt", "transcribe", "--enable-transcription-partials"],
+            {"enable_transcription_partials": True},
+        ),
+        (
+            ["rt", "transcribe", "--enable-translation-partials"],
+            {"enable_translation_partials": True},
+        ),
         (["rt", "transcribe", "--enable-entities"], {"enable_entities": True}),
         (["batch", "transcribe", "--enable-entities"], {"enable_entities": True}),
         (
             ["batch", "transcribe", "--speaker-diarization-sensitivity=0.7"],
             {"speaker_diarization_sensitivity": 0.7},
         ),
         (
@@ -657,197 +663,14 @@
     assert msg["transcription_config"]["domain"] == "different"
     assert msg["transcription_config"]["enable_entities"] is True
     assert msg["transcription_config"]["output_locale"] == "en-US"
     assert msg["transcription_config"]["speaker_change_sensitivity"] == 0.8
     assert msg["transcription_config"]["operating_point"] == "enhanced"
 
 
-@pytest.mark.parametrize("check_tty", [False, True])
-def test_add_printing_handlers_transcript_handler(mocker, capsys, check_tty):
-    # patch in isatty, in order to check beheviour with and without tty
-    sys.stderr.isatty = lambda: check_tty
-    sys.stdout.isatty = lambda: check_tty
-
-    api = mocker.MagicMock()
-    api.get_language_pack_info = mocker.MagicMock(return_value={"word_delimiter": " "})
-    transcripts = cli.Transcripts(text="", json=[])
-
-    cli.add_printing_handlers(api, transcripts)
-    assert not transcripts.text
-    assert not transcripts.json
-    out, err = capsys.readouterr()
-    assert not out
-    assert not err
-    assert api.add_event_handler.called
-    call_args_dict = {i[0][0]: i[0][1] for i in api.add_event_handler.call_args_list}
-
-    finals_msg_type = "AddTranscript"
-    assert finals_msg_type in call_args_dict
-    transcript_handler_cb_func = call_args_dict[finals_msg_type]
-
-    transcript = ""
-    msg_empty_transcript = {
-        "message": "AddTranscript",
-        "results": [],
-        "metadata": {
-            "start_time": 58.920005798339844,
-            "end_time": 60.0000057220459,
-            "transcript": transcript,
-        },
-        "format": "2.4",
-    }
-    transcript_handler_cb_func(msg_empty_transcript)
-    assert transcripts.text == transcript
-    assert transcripts.json == [msg_empty_transcript]
-
-    out, err = capsys.readouterr()
-    assert not out, "Don't print a newline when the transcript is empty"
-    assert not err
-
-    transcript = "Howdy"
-    msg_single_word_transcript = copy.deepcopy(msg_empty_transcript)
-    msg_single_word_transcript["metadata"]["transcript"] = transcript
-    msg_single_word_transcript["results"].append(
-        {
-            "type": "word",
-            "start_time": 0.08999999612569809,
-            "end_time": 0.29999998211860657,
-            "alternatives": [
-                {"confidence": 1.0, "content": transcript.strip(), "language": "en"}
-            ],
-        }
-    )
-    transcript_handler_cb_func(msg_single_word_transcript)
-    assert transcripts.text == transcript
-    assert transcripts.json == [msg_empty_transcript, msg_single_word_transcript]
-    out, err = capsys.readouterr()
-
-    escape_seq = "\33[2K" if sys.stdout.isatty() else ""
-    assert out == escape_seq + transcript + "\n"
-    assert not err
-
-    transcript_handler_cb_func(msg_empty_transcript)
-    transcript_handler_cb_func(msg_single_word_transcript)
-    transcript_handler_cb_func(msg_empty_transcript)
-    assert transcripts.text == transcript * 2
-    assert transcripts.json == [
-        msg_empty_transcript,
-        msg_single_word_transcript,
-        msg_empty_transcript,
-        msg_single_word_transcript,
-        msg_empty_transcript,
-    ]
-
-    escape_seq = "\33[2K" if sys.stdout.isatty() else ""
-    out, err = capsys.readouterr()
-    assert out == escape_seq + transcript + "\n"
-    assert not err
-
-
-TRANSCRIPT_TXT_WITH_SC = "Hey\nHello"
-TRANSCRIPT_WITH_SC = {
-    "message": "AddTranscript",
-    "results": [
-        {
-            "type": "word",
-            "start_time": 0.08999999612569809,
-            "end_time": 0.29999998211860657,
-            "alternatives": [{"confidence": 1.0, "content": "Hey", "language": "en"}],
-        },
-        {
-            "type": "speaker_change",
-            "start_time": 0.08999999612569809,
-            "end_time": 0.29999998211860657,
-            "score": 1,
-        },
-        {
-            "type": "word",
-            "start_time": 0.08999999612569809,
-            "end_time": 0.29999998211860657,
-            "alternatives": [{"confidence": 1.0, "content": "Hello", "language": "en"}],
-        },
-    ],
-    "metadata": {
-        "start_time": 58.920005798339844,
-        "end_time": 60.0000057220459,
-        "transcript": TRANSCRIPT_TXT_WITH_SC,
-    },
-    "format": "2.4",
-}
-
-
-def check_printing_handlers(
-    mocker,
-    capsys,
-    transcript,
-    expected_transcript_txt,
-    speaker_change_token,
-):
-
-    api = mocker.MagicMock()
-    api.get_language_pack_info = mocker.MagicMock(return_value={"word_delimiter": " "})
-    transcripts = cli.Transcripts(text="", json=[])
-
-    cli.add_printing_handlers(
-        api, transcripts, speaker_change_token=speaker_change_token
-    )
-    assert not transcripts.text
-    assert not transcripts.json
-    out, err = capsys.readouterr()
-    assert not out
-    assert not err
-    assert api.add_event_handler.called
-    call_args_dict = {i[0][0]: i[0][1] for i in api.add_event_handler.call_args_list}
-
-    finals_msg_type = "AddTranscript"
-    assert finals_msg_type in call_args_dict
-    transcript_handler_cb_func = call_args_dict[finals_msg_type]
-
-    transcript_handler_cb_func(transcript)
-    assert transcripts.text == expected_transcript_txt
-    assert transcripts.json == [transcript]
-
-    escape_seq = "\33[2K" if sys.stdout.isatty() else ""
-    out, err = capsys.readouterr()
-    assert out == escape_seq + expected_transcript_txt + "\n"
-    assert not err
-
-
-@pytest.mark.parametrize("check_tty", [False, True])
-def test_add_printing_handlers_with_speaker_change_token(mocker, capsys, check_tty):
-    # patch in isatty, in order to check beheviour with and without tty
-    sys.stderr.isatty = lambda: check_tty
-    sys.stdout.isatty = lambda: check_tty
-
-    expected_transcript = "Hey\n<sc>\nHello"
-    check_printing_handlers(
-        mocker,
-        capsys,
-        TRANSCRIPT_WITH_SC,
-        expected_transcript,
-        speaker_change_token=True,
-    )
-
-
-@pytest.mark.parametrize("check_tty", [False, True])
-def test_add_printing_handlers_with_speaker_change_no_token(mocker, capsys, check_tty):
-    # patch in isatty, in order to check beheviour with and without tty
-    sys.stderr.isatty = lambda: check_tty
-    sys.stdout.isatty = lambda: check_tty
-
-    expected_transcript = "Hey\nHello"
-    check_printing_handlers(
-        mocker,
-        capsys,
-        TRANSCRIPT_WITH_SC,
-        expected_transcript,
-        speaker_change_token=False,
-    )
-
-
 @pytest.mark.parametrize(
     "args, values",
     (
         (
             ["config", "set", "--auth-token=faketoken", "--generate-temp-token"],
             {"auth_token": "faketoken", "generate_temp_token": True},
         ),
@@ -861,81 +684,66 @@
 
     actual_values = vars(cli.parse_args(args=args))
 
     for (key, val) in values.items():
         assert actual_values[key] == val
 
 
-def test_config_set_toml():
-    args = {
-        "command": "set",
-        "auth_token": "faketoken",
-    }
-    try:
-        cli.config_main(args)
-    except Exception:  # pylint: disable=broad-except
-        assert False
-    home_dir = os.path.expanduser("~")
-    cli_config = {"default": {}}
-    with open(f"{home_dir}/.speechmatics/config", "r", encoding="UTF-8") as file:
-        cli_config = toml.load(file)
-
-    del args["command"]
-    for (key, val) in args.items():
-        assert cli_config["default"][key] == val
-
-
 @pytest.mark.parametrize(
     "args",
     (
         {
             "auth_token": "faketoken",
             "generate_temp_token": True,
         },
         {
             "auth_token": "faketoken",
         },
         {
             "generate_temp_token": True,
         },
+        {"generate_temp_token": True, "auth_token": "faketoken", "profile": "test"},
+        {"realtime_url": "wss://speechmatics.io"},
+        {"batch_url": "https://speechmatics.io"},
     ),
 )
 def test_config_set_and_remove_toml(args):
     set_args = {"command": "set"}
     set_args = {**set_args, **args}
     try:
         cli.config_main(set_args)
     except Exception:  # pylint: disable=broad-except
         assert False
     home_dir = os.path.expanduser("~")
-    cli_config = {"default": {}}
+    cli_config = {}
     with open(f"{home_dir}/.speechmatics/config", "r", encoding="UTF-8") as file:
         cli_config = toml.load(file)
-
+    profile = args.get("profile", "default")
     for (key, val) in args.items():
-        assert cli_config["default"][key] == val
+        if key != "profile":
+            assert cli_config[profile][key] == val
 
-    unset_args = {"command": "unset"}
-    for key in ["auth_token", "generate_temp_token"]:
+    unset_args = {"command": "unset", "profile": profile}
+    for key in ["auth_token", "generate_temp_token", "realtime_url", "batch_url"]:
         if key in args:
             unset_args[key] = True
         else:
             unset_args[key] = False
 
     try:
         cli.config_main(unset_args)
     except Exception:  # pylint: disable=broad-except
         assert False
     home_dir = os.path.expanduser("~")
-    cli_config = {"default": {}}
     with open(f"{home_dir}/.speechmatics/config", "r", encoding="UTF-8") as file:
         cli_config = toml.load(file)
 
     for (key, val) in args.items():
-        assert key not in cli_config["default"]
+        if key != "profile":
+            assert key not in cli_config[profile]
 
 
 def test_default_urls_connection_config():
     rt_args = {"mode": "rt"}
     settings = cli.get_connection_settings(rt_args, lang="es")
     assert settings.url == f"{RT_SELF_SERVICE_URL}/es"
```

### Comparing `speechmatics-python-1.7.0/tests/test_client.py` & `speechmatics-python-1.8.2/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `speechmatics-python-1.7.0/tests/utils.py` & `speechmatics-python-1.8.2/tests/utils.py`

 * *Files identical despite different names*

