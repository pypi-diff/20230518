# Comparing `tmp/gptsubtitler-0.0.8.tar.gz` & `tmp/gptsubtitler-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gptsubtitler-0.0.8.tar", last modified: Wed May 17 16:20:11 2023, max compression
+gzip compressed data, was "gptsubtitler-0.0.9.tar", last modified: Thu May 18 10:38:05 2023, max compression
```

## Comparing `gptsubtitler-0.0.8.tar` & `gptsubtitler-0.0.9.tar`

### file list

```diff
@@ -1,17 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-05-17 16:20:11.169638 gptsubtitler-0.0.8/
--rw-rw-rw-   0        0        0     1085 2023-05-17 07:34:14.000000 gptsubtitler-0.0.8/LICENSE
--rw-rw-rw-   0        0        0     2887 2023-05-17 16:20:11.168638 gptsubtitler-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0     2460 2023-05-17 14:41:56.000000 gptsubtitler-0.0.8/README.md
-drwxrwxrwx   0        0        0        0 2023-05-17 16:20:11.147633 gptsubtitler-0.0.8/gptsubtitler/
--rw-rw-rw-   0        0        0      126 2023-05-17 08:29:20.000000 gptsubtitler-0.0.8/gptsubtitler/__init__.py
--rw-rw-rw-   0        0        0     5550 2023-05-17 15:17:42.000000 gptsubtitler-0.0.8/gptsubtitler/transcriber.py
--rw-rw-rw-   0        0        0     3914 2023-05-17 14:49:59.000000 gptsubtitler-0.0.8/gptsubtitler/translator.py
--rw-rw-rw-   0        0        0     1360 2023-05-17 07:38:36.000000 gptsubtitler-0.0.8/gptsubtitler/video_utils.py
-drwxrwxrwx   0        0        0        0 2023-05-17 16:20:11.167637 gptsubtitler-0.0.8/gptsubtitler.egg-info/
--rw-rw-rw-   0        0        0     2887 2023-05-17 16:20:11.000000 gptsubtitler-0.0.8/gptsubtitler.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      313 2023-05-17 16:20:11.000000 gptsubtitler-0.0.8/gptsubtitler.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-17 16:20:11.000000 gptsubtitler-0.0.8/gptsubtitler.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       42 2023-05-17 16:20:11.000000 gptsubtitler-0.0.8/gptsubtitler.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-05-17 16:20:11.000000 gptsubtitler-0.0.8/gptsubtitler.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-17 16:20:11.169638 gptsubtitler-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0      739 2023-05-17 16:19:53.000000 gptsubtitler-0.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-18 10:38:05.150516 gptsubtitler-0.0.9/
+-rw-rw-rw-   0        0        0     1085 2023-05-17 07:34:14.000000 gptsubtitler-0.0.9/LICENSE
+-rw-rw-rw-   0        0        0     3312 2023-05-18 10:38:05.150516 gptsubtitler-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0     2934 2023-05-18 10:35:22.000000 gptsubtitler-0.0.9/README.md
+drwxrwxrwx   0        0        0        0 2023-05-18 10:38:05.130833 gptsubtitler-0.0.9/gptsubtitler/
+-rw-rw-rw-   0        0        0      126 2023-05-17 08:29:20.000000 gptsubtitler-0.0.9/gptsubtitler/__init__.py
+-rw-rw-rw-   0        0        0     1413 2023-05-18 10:27:37.000000 gptsubtitler-0.0.9/gptsubtitler/cli.py
+-rw-rw-rw-   0        0        0     6696 2023-05-18 10:37:04.000000 gptsubtitler-0.0.9/gptsubtitler/transcriber.py
+-rw-rw-rw-   0        0        0     3986 2023-05-18 10:24:51.000000 gptsubtitler-0.0.9/gptsubtitler/translator.py
+-rw-rw-rw-   0        0        0     1178 2023-05-18 09:29:34.000000 gptsubtitler-0.0.9/gptsubtitler/video_utils.py
+drwxrwxrwx   0        0        0        0 2023-05-18 10:38:05.149516 gptsubtitler-0.0.9/gptsubtitler.egg-info/
+-rw-rw-rw-   0        0        0     3312 2023-05-18 10:38:05.000000 gptsubtitler-0.0.9/gptsubtitler.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      372 2023-05-18 10:38:05.000000 gptsubtitler-0.0.9/gptsubtitler.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-18 10:38:05.000000 gptsubtitler-0.0.9/gptsubtitler.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       55 2023-05-18 10:38:05.000000 gptsubtitler-0.0.9/gptsubtitler.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       41 2023-05-18 10:38:05.000000 gptsubtitler-0.0.9/gptsubtitler.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-05-18 10:38:05.000000 gptsubtitler-0.0.9/gptsubtitler.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-18 10:38:05.151517 gptsubtitler-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0      801 2023-05-18 10:05:35.000000 gptsubtitler-0.0.9/setup.py
```

### Comparing `gptsubtitler-0.0.8/LICENSE` & `gptsubtitler-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `gptsubtitler-0.0.8/gptsubtitler/transcriber.py` & `gptsubtitler-0.0.9/gptsubtitler/transcriber.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,162 +1,187 @@
 import whisper
+from pywhispercpp.model import Model
 from .video_utils import convert_video_to_audio, create_video_with_subtitles
 from .translator import Translator
 import os
 
 
 class Transcriber(object):
     model = None
-    model_type = None
+    captioning_model_type = None
     target_language = None
+    source_language = None
     language_model_type = None
-    device = None
+    model_dir = None
     AVAILABLE_MODELS = ["tiny", "base", "small", "medium", "large"]
 
     @staticmethod
     def create_model():
         if Transcriber.model is None:
+            # Choose number of threads
+            threads = os.cpu_count()
+            if threads is None:
+                threads = 1
+            else:
+                threads = threads // 2
+
             try:
-                Transcriber.model = whisper.load_model(
-                    Transcriber.model_type, device=Transcriber.device
-                )
+                Transcriber.model = Model(Transcriber.captioning_model_type, n_threads=threads, models_dir=Transcriber.model_dir)
             except Exception as e:
                 print("Couldn't load model.")
                 print(e)
 
     @staticmethod
     def transcribe(
         video_file,
         output_video_file=None,
         output_subtitle_file="output.srt",
+        source_language=None,
         target_language=None,
-        model_type="base",
+        captioning_model_type="base",
         language_model_type="base",
-        device="cpu",
+        model_dir=None
     ):
         """Transcribe video file and generate SRT file.
-        
+
         Args:
             video_file (str): Path to video file.
 
             output_video_file (str, optional): Path to output video file. Defaults to None.
 
             output_subtitle_file (str, optional): Path to output SRT file. Defaults to "output.srt".
 
+            source_language (str, optional): Source language for translation. Defaults to None.
+
             target_language (str, optional): Target language for translation. Defaults to None.
 
-            model_type (str, optional): Model type. Defaults to "base".
+            captioning_model_type (str, optional): Model type. Defaults to "base".
 
             language_model_type (str, optional): Language model type. Defaults to "base".
 
-            device (str, optional): Device to use. Defaults to "cpu".
+            model_dir (str, optional): Path to model directory. Defaults to None.
         """
-        if model_type not in Transcriber.AVAILABLE_MODELS:
+        if captioning_model_type not in Transcriber.AVAILABLE_MODELS:
             print(
-                f"Invalid 'model_type'. Using base model. Available models: {Transcriber.AVAILABLE_MODELS}"
+                f"Invalid 'captioning_model_type'. Using base model. Available models: {Transcriber.AVAILABLE_MODELS}"
             )
-            model_type = "base"
+            captioning_model_type = "base"
 
-        # Set device
-        Transcriber.device = device
+        if source_language is None:
+            print("Source language not specified. Using English.")
+            source_language = "en"
 
         # Set target language
         Transcriber.target_language = target_language
 
+        # Set source language
+        Transcriber.source_language = source_language
+
         # Set language model type
         Transcriber.language_model_type = language_model_type
 
         # Set model type
-        Transcriber.model_type = model_type
+        Transcriber.captioning_model_type = captioning_model_type
+
+        # Set model directory
+        Transcriber.model_dir = model_dir
 
         # Create model
         Transcriber.create_model()
 
         if output_video_file is None:
-            output_video_file = video_file.replace(".mp4", "_subtitled.mp4")
+            # Set output video file
+            dot = video_file.rfind(".")
+            output_video_file = video_file[:dot] + "_subtitled" + video_file[dot:]
 
         # Try to transcribe audio
         transcript = None
         try:
+            print("Converting video to audio.")
             convert_video_to_audio(video_file, "temporary_audio.wav")
+            print("Video converted to audio.")
 
-            print("Transcribing audio.")
-            transcript = Transcriber.model.transcribe("temporary_audio.wav")
-            print("Finished transcription.")
+            print("Captioning audio.")
+            transcript = Transcriber.model.transcribe(
+                "temporary_audio.wav", language=Transcriber.source_language, speed_up=True, print_progress=False
+            )
+            print("Finished captioning.")
 
             os.remove("temporary_audio.wav")
         except Exception as e:
             print("Couldn't transcribe audio.")
             print(e)
 
         # Try to generate SRT file
         srt_content = None
         try:
+            print("Generating SRT file.")
             srt_content = Transcriber.generate_srt_file(transcript)
+            print("SRT file generated.")
         except Exception as e:
             print("Couldn't generate SRT file.")
             print(e)
 
-        print(srt_content)
         # Add .srt extension if not present
         if not output_subtitle_file.endswith(".srt"):
             output_subtitle_file += ".srt"
 
         # Write SRT file
         with open(output_subtitle_file, "w", encoding="utf-8") as f:
             f.write(srt_content)
 
+        # Create video with subtitles
+        print("Creating video with subtitles.")
         create_video_with_subtitles(video_file, output_subtitle_file, output_video_file)
+        print("Video with subtitles created.")
 
     @staticmethod
     def generate_srt_file(transcript):
         srt_content = ""
-
-        print("Starting generation of srt file.")
-        print(f"Total lines: {len(transcript['segments'])}")
-        for line in transcript["segments"]:
+        print(f"Total lines: {len(transcript)}")
+        for count, line in enumerate(transcript):
             # Add line number
-            srt_content += str(line["id"]) + "\n"
+            srt_content += str(count) + "\n"
 
             # Add timestamps
             srt_content += (
-                Transcriber.format_seconds_to_srt_timestamp(line["start"])
+                Transcriber.format_seconds_to_srt_timestamp(line.t0)
                 + " --> "
-                + Transcriber.format_seconds_to_srt_timestamp(line["end"])
+                + Transcriber.format_seconds_to_srt_timestamp(line.t1)
                 + "\n"
             )
 
             # Add text
-            text = line["text"].strip()
-            if Transcriber.target_language is not None:
+            text = line.text.strip()
+            if Transcriber.target_language is not None and Transcriber.target_language != Transcriber.source_language:
                 # Translate text only if user wanted to translate text
                 text = Translator.translate(
                     text,
-                    source_language=transcript["language"],
+                    source_language=Transcriber.source_language,
                     target_language=Transcriber.target_language,
                     model_type=Transcriber.language_model_type,
-                    device=Transcriber.device,
+                    model_dir=Transcriber.model_dir,
                 ).strip()
 
                 print(
-                    f"- Line {line['id'] + 1} of {len(transcript['segments'])}: {line['text']}\n --> {text}"
+                    f"- Line {count} of {len(transcript)}: {line.text}\n --> {text}"
                 )
             else:
                 print(
-                    f"- Line {line['id'] + 1} of {len(transcript['segments'])}: {line['text']}"
+                    f"- Line {count} of {len(transcript)}: {line.text}"
                 )
             srt_content += text + "\n"
 
             srt_content += "\n"
 
         return srt_content
 
     @staticmethod
     def format_seconds_to_srt_timestamp(seconds):
-        milliseconds = round(seconds * 1000.0)
+        milliseconds = round(seconds * 10.0)
 
         hours = milliseconds // 3_600_000
         milliseconds -= hours * 3_600_000
 
         minutes = milliseconds // 60_000
         milliseconds -= minutes * 60_000
```

### Comparing `gptsubtitler-0.0.8/gptsubtitler/translator.py` & `gptsubtitler-0.0.9/gptsubtitler/translator.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,19 +1,27 @@
 from transformers import M2M100ForConditionalGeneration, M2M100Tokenizer
-import torch
+import os
 
 
 class Translator(object):
     model = None
     tokenizer = None
     model_type = None
+    model_dir = None
     AVAILABLE_MODELS = ["base", "large"]
 
     @staticmethod
     def create_model_and_tokenizer():
+        # Set model directory
+        if Translator.model_dir is not None:
+            if os.environ.get("HF_HOME") is None:
+                raise Exception(
+                    "HF_HOME environment variable not set! Please set HF_HOME environment variable! Otherwise, run without model_dir parameter."
+                )
+
         if Translator.model is None:
             try:
                 if Translator.model_type == "base":
                     Translator.model = M2M100ForConditionalGeneration.from_pretrained(
                         "facebook/m2m100_418M"
                     )
                 elif Translator.model_type == "large":
@@ -40,62 +48,55 @@
 
     @staticmethod
     def translate(
         text,
         source_language="en",
         target_language="ro",
         model_type="base",
-        device="cpu",
+        model_dir=None,
     ):
         """Translate text.
-        
+
         Args:
             text (str): Text to translate.
 
             source_language (str, optional): Source language. Defaults to "en".
 
             target_language (str, optional): Target language. Defaults to "ro".
 
             model_type (str, optional): Model type. Defaults to "base".
-
-            device (str, optional): Device to use. Defaults to "cpu".
         Returns:
             str: Translated text.
         """
         if model_type not in Translator.AVAILABLE_MODELS:
             print(
                 f"Invalid 'model_type'. Using base model. Available models: {Translator.AVAILABLE_MODELS}"
             )
             model_type = "base"
 
-        if device == "cuda":
-            if not torch.cuda.is_available():
-                device = "cpu"
-            else:
-                device = "cuda:0"
+        # Set model directory
+        Translator.model_dir = model_dir
 
         # Set model type
         Translator.model_type = model_type
 
         Translator.create_model_and_tokenizer()
 
         # Set source language for tokenizer
         Translator.tokenizer.src_lang = source_language
 
         # Try to encode text
         try:
-            encoded_text = Translator.tokenizer(text, return_tensors="pt").to(device)
+            encoded_text = Translator.tokenizer(text, return_tensors="pt")
         except Exception as e:
             print("Couldn't encode text.")
             print(e)
 
         # Try to generate tokens
         try:
-            # Move to device first
-            Translator.model = Translator.model.to(device)
             generated_tokens = Translator.model.generate(
                 **encoded_text,
                 forced_bos_token_id=Translator.tokenizer.get_lang_id(target_language),
             )
         except Exception as e:
             print("Couldn't generate tokens. Maybe language is not supported.")
             print(e)
```

### Comparing `gptsubtitler-0.0.8/gptsubtitler/video_utils.py` & `gptsubtitler-0.0.9/gptsubtitler/video_utils.py`

 * *Files 17% similar despite different names*

```diff
@@ -4,41 +4,33 @@
     try:
         return ffmpeg.input(file_path)
     except Exception as e:
         print("Couldn't get video.")
         print(e)
 
 def convert_video_to_audio(video_path, output_path):
-    print("Converting video to audio.")
-
     try:
         video = get_video(video_path)
         video.output(output_path, acodec="pcm_s16le", ac=1, ar="16k").run(quiet=True, overwrite_output=True)
     except Exception as e:
         print("Couldn't convert video to audio.")
         print(e)
 
-    print("Video converted to audio.")
-
 def create_video_with_subtitles(video_path, subtitles_path, output_path):
     """Create video with subtitles.
     
     Args:
         video_path (str): Path to video file.
 
         subtitles_path (str): Path to subtitles file.
         
         output_path (str): Path to output video file.
     """
-    print("Creating video with subtitles.")
-
     try:
         video = get_video(video_path)
 
         ffmpeg.concat(
             video.filter('subtitles', subtitles_path, force_style="OutlineColour=&H40000000,BorderStyle=3"), video.audio, v=1, a=1
         ).output(output_path).run(quiet=True, overwrite_output=True)
     except Exception as e:
         print("Couldn't create video with subtitles.")
         print(e)
-    
-    print("Video with subtitles created.")
```

### Comparing `gptsubtitler-0.0.8/setup.py` & `gptsubtitler-0.0.9/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -2,25 +2,28 @@
 
 def readme():
     with open('README.md') as f:
         return f.read()
 
 setup(
     name="gptsubtitler",
-    version="0.0.8",
+    version="0.0.9",
     author="extremq",
     author_email="extremqcontact@gmail.com",
     description="Automatically subtitle any video spoken in any language to a language of your choice.",
     install_requires=[
-        "transformers",
-        "openai-whisper",
-        "sentencepiece"
+        "transformers>=4.29.1",
+        "pywhispercpp>=1.0.8"
     ],
     packages=["gptsubtitler"],
     classifiers=[
-        "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
+    entry_points = {
+        "console_scripts": [
+            "gptsubtitler = gptsubtitler.cli:main"
+        ]
+    },
     long_description=readme(),
     long_description_content_type = "text/markdown"
 )
```

