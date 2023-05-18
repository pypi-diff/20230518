# Comparing `tmp/pyvosklivesubtitle-0.1.6.tar.gz` & `tmp/pyvosklivesubtitle-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyvosklivesubtitle-0.1.6.tar", last modified: Mon May  8 21:18:06 2023, max compression
+gzip compressed data, was "dist\pyvosklivesubtitle-0.1.7.tar", last modified: Thu May 18 20:17:21 2023, max compression
```

## Comparing `pyvosklivesubtitle-0.1.6.tar` & `pyvosklivesubtitle-0.1.7.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-08 21:18:06.420709 pyvosklivesubtitle-0.1.6/
--rwxrwxrwx   0 root         (0) root         (0)     1088 2022-11-03 03:32:17.000000 pyvosklivesubtitle-0.1.6/LICENSE
--rwxrwxrwx   0 root         (0) root         (0)       34 2022-06-05 08:17:08.000000 pyvosklivesubtitle-0.1.6/MANIFEST.in
--rwxrwxrwx   0 root         (0) root         (0)     1588 2023-05-08 21:18:06.421023 pyvosklivesubtitle-0.1.6/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)     6636 2023-04-24 13:05:36.000000 pyvosklivesubtitle-0.1.6/README.md
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-08 21:18:06.408891 pyvosklivesubtitle-0.1.6/pyvosklivesubtitle/
--rwxrwxrwx   0 root         (0) root         (0)   146492 2023-05-08 21:17:21.000000 pyvosklivesubtitle-0.1.6/pyvosklivesubtitle/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-08 21:18:06.419909 pyvosklivesubtitle-0.1.6/pyvosklivesubtitle.egg-info/
--rwxrwxrwx   0 root         (0) root         (0)     1588 2023-05-08 21:18:06.000000 pyvosklivesubtitle-0.1.6/pyvosklivesubtitle.egg-info/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)      333 2023-05-08 21:18:06.000000 pyvosklivesubtitle-0.1.6/pyvosklivesubtitle.egg-info/SOURCES.txt
--rwxrwxrwx   0 root         (0) root         (0)        1 2023-05-08 21:18:06.000000 pyvosklivesubtitle-0.1.6/pyvosklivesubtitle.egg-info/dependency_links.txt
--rwxrwxrwx   0 root         (0) root         (0)       63 2023-05-08 21:18:06.000000 pyvosklivesubtitle-0.1.6/pyvosklivesubtitle.egg-info/entry_points.txt
--rwxrwxrwx   0 root         (0) root         (0)      139 2023-05-08 21:18:06.000000 pyvosklivesubtitle-0.1.6/pyvosklivesubtitle.egg-info/requires.txt
--rwxrwxrwx   0 root         (0) root         (0)       19 2023-05-08 21:18:06.000000 pyvosklivesubtitle-0.1.6/pyvosklivesubtitle.egg-info/top_level.txt
--rwxrwxrwx   0 root         (0) root         (0)      136 2023-05-08 21:18:06.422471 pyvosklivesubtitle-0.1.6/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)     1721 2023-05-08 18:46:09.000000 pyvosklivesubtitle-0.1.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-18 20:17:21.835658 pyvosklivesubtitle-0.1.7/
+-rw-rw-rw-   0        0        0     1088 2022-11-03 03:32:17.000000 pyvosklivesubtitle-0.1.7/LICENSE
+-rw-rw-rw-   0        0        0       34 2022-06-05 08:17:08.000000 pyvosklivesubtitle-0.1.7/MANIFEST.in
+-rw-rw-rw-   0        0        0     1490 2023-05-18 20:17:21.836408 pyvosklivesubtitle-0.1.7/PKG-INFO
+-rw-rw-rw-   0        0        0     6636 2023-04-24 13:05:36.000000 pyvosklivesubtitle-0.1.7/README.md
+drwxrwxrwx   0        0        0        0 2023-05-18 20:17:21.787343 pyvosklivesubtitle-0.1.7/pyvosklivesubtitle/
+-rw-rw-rw-   0        0        0   146375 2023-05-18 20:15:26.000000 pyvosklivesubtitle-0.1.7/pyvosklivesubtitle/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-18 20:17:21.833411 pyvosklivesubtitle-0.1.7/pyvosklivesubtitle.egg-info/
+-rw-rw-rw-   0        0        0     1490 2023-05-18 20:17:21.000000 pyvosklivesubtitle-0.1.7/pyvosklivesubtitle.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      333 2023-05-18 20:17:21.000000 pyvosklivesubtitle-0.1.7/pyvosklivesubtitle.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-18 20:17:21.000000 pyvosklivesubtitle-0.1.7/pyvosklivesubtitle.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       64 2023-05-18 20:17:21.000000 pyvosklivesubtitle-0.1.7/pyvosklivesubtitle.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      152 2023-05-18 20:17:21.000000 pyvosklivesubtitle-0.1.7/pyvosklivesubtitle.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2023-05-18 20:17:21.000000 pyvosklivesubtitle-0.1.7/pyvosklivesubtitle.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      147 2023-05-18 20:17:21.838656 pyvosklivesubtitle-0.1.7/setup.cfg
+-rw-rw-rw-   0        0        0     1721 2023-05-08 18:46:09.000000 pyvosklivesubtitle-0.1.7/setup.py
```

### Comparing `pyvosklivesubtitle-0.1.6/LICENSE` & `pyvosklivesubtitle-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `pyvosklivesubtitle-0.1.6/PKG-INFO` & `pyvosklivesubtitle-0.1.7/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,29 +1,31 @@
-Metadata-Version: 2.1
-Name: pyvosklivesubtitle
-Version: 0.1.6
-Summary: A Python based desktop aplication that can RECOGNIZE any live streaming in 21 languages that supported by VOSK then TRANSLATE and display it as LIVE SUBTITLES
-Home-page: https://github.com/botbahlul/pyvosklivesubtitle
-Author: Bot Bahlul
-Author-email: bot.bahlul@gmail.com
-License: MIT License
-        
-        Copyright (c) 2022 Bot Bahlul
-        
-        Permission is hereby granted, free of charge, to any person obtaining a copy
-        of this software and associated documentation files (the "Software"), to deal
-        in the Software without restriction, including without limitation the rights
-        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-        copies of the Software, and to permit persons to whom the Software is
-        furnished to do so, subject to the following conditions:
-        
-        The above copyright notice and this permission notice shall be included in all
-        copies or substantial portions of the Software.
-        
-        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-        SOFTWARE.
-        
+Metadata-Version: 1.0
+Name: pyvosklivesubtitle
+Version: 0.1.7
+Summary: A Python based desktop aplication that can RECOGNIZE any live streaming in 21 languages that supported by VOSK then TRANSLATE and display it as LIVE SUBTITLES
+Home-page: https://github.com/botbahlul/pyvosklivesubtitle
+Author: Bot Bahlul
+Author-email: bot.bahlul@gmail.com
+License: MIT License
+
+Copyright (c) 2022 Bot Bahlul
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
+
+Description: UNKNOWN
+Platform: UNKNOWN
```

### Comparing `pyvosklivesubtitle-0.1.6/README.md` & `pyvosklivesubtitle-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `pyvosklivesubtitle-0.1.6/pyvosklivesubtitle/__init__.py` & `pyvosklivesubtitle-0.1.7/pyvosklivesubtitle/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -557,15 +557,15 @@
     def GetPendingChunks(self):
         return _c.vosk_batch_recognizer_get_pending_chunks(self._handle)
 
 #=======================================================================================================================================#
 
 #============================================================== APP PARTS ==============================================================#
 
-VERSION = '0.1.6'
+VERSION = '0.1.7'
 
 arraylist_models = []
 arraylist_models.append("ca-es");
 arraylist_models.append("zh-cn")
 arraylist_models.append("cs-cz");
 arraylist_models.append("nl-nl");
 arraylist_models.append("en-us")
@@ -1009,14 +1009,15 @@
 
     start_time = None
     end_time = None
     first_streaming_duration_recorded = None
     absolute_start_time = None
     audio_filename, SampleRate = None, None
     first_regions = None
+    model = None
 
     time_value_filename = "time_value"
     time_value_filepath = os.path.join(tempfile.gettempdir(), time_value_filename)
     #print("time_value_filepath = {}".format(time_value_filepath))
     #print("os.path.isfile(time_value_filepath) = {}".format(os.path.isfile(time_value_filepath)))
     if os.path.isfile(time_value_filepath):
         time_value_file = open(time_value_filepath, "r")
@@ -2952,15 +2953,14 @@
             if recognizing:
                 #print("VOSK Live Subtitle is START LISTENING now")
                 #print("recognizing = {}".format(recognizing))
 
                 start_button_click_time = datetime.now()
                 #print("start_button_click_time = {}".format(start_button_click_time))
 
-                #if tmp_recorded_streaming_filepath and os.path.isfile(tmp_recorded_streaming_filepath): os.remove(tmp_recorded_streaming_filepath)
                 if partial_result_filepath and os.path.isfile(partial_result_filepath): os.remove(partial_result_filepath)
                 if time_value_filepath and os.path.isfile(time_value_filepath): os.remove(time_value_filepath)
                 if tmp_src_subtitle_filepath and os.path.isfile(tmp_src_subtitle_filepath): os.remove(tmp_src_subtitle_filepath)
                 if tmp_dst_subtitle_filepath and os.path.isfile(tmp_dst_subtitle_filepath): os.remove(tmp_dst_subtitle_filepath)
                 if tmp_src_txt_transcription_filepath and os.path.isfile(tmp_src_txt_transcription_filepath): os.remove(tmp_src_txt_transcription_filepath)
                 if tmp_dst_txt_transcription_filepath and os.path.isfile(tmp_dst_txt_transcription_filepath): os.remove(tmp_dst_txt_transcription_filepath)
 
@@ -3041,17 +3041,14 @@
 
                 if overlay_translation_window:
                     overlay_translation_window.Hide()
 
                 if thread_recognize and thread_recognize.is_alive(): stop_thread(thread_recognize)
                 if thread_timed_translate and thread_timed_translate.is_alive(): stop_thread(thread_timed_translate)
 
-                #if thread_recognize and thread_recognize.is_alive(): thread_recognize.join()
-                #if thread_timed_translate and thread_timed_translate.is_alive(): thread_timed_translate.join()
-
                 # IF RECORD STREAMING
                 if main_window['-URL-'].get() != (None or "") and main_window['-RECORD-STREAMING-'].get() == True:
 
                     if sys.platform == "win32":
                         #print("thread_record_streaming.is_alive() = {}".format(thread_record_streaming.is_alive()))
                         stop_record_streaming_windows()
 
@@ -3125,32 +3122,37 @@
 
         elif event == '-EVENT-RESULTS-' and recognizing==True:
 
             line = str(values[event]).strip().lower()
             main_window['-ML-SRC-RESULTS-'].update(line + "\n", background_color_for_value='yellow1', append=True, autoscroll=True)
             translated_line = GoogleTranslate(line, src, dst, error_messages_callback=show_error_messages)
             main_window['-ML-DST-RESULTS-'].update(translated_line + "\n", background_color_for_value='yellow1', append=True, autoscroll=True)
-            if overlay_translation_window is not None:
+
+            if overlay_translation_window:
                 overlay_translation_window.UnHide
                 overlay_translation_window['-ML-OVERLAY-DST-PARTIAL-RESULTS-'].update(translated_line, background_color_for_value='black', visible=True, autoscroll=True)
             else:
                 overlay_translation_window = make_overlay_translation_window(100*' ')
                 overlay_translation_window['-ML-OVERLAY-DST-PARTIAL-RESULTS-'].update(translated_line, background_color_for_value='black', visible=True, autoscroll=True)
 
 
         elif event == '-EVENT-VOICE-TRANSLATED-' and recognizing==True:
 
             translated_text = str(values[event]).strip().lower()
             if translated_text:
                 main_window['-ML-DST-PARTIAL-RESULTS-'].update(translated_text,background_color_for_value='yellow1',autoscroll=True)
 
                 # SHOWING OVERLAY TRANSLATION WINDOW
-                if not overlay_translation_window:
+                if overlay_translation_window:
+                    overlay_translation_window.UnHide()
+                    overlay_translation_window['-ML-OVERLAY-DST-PARTIAL-RESULTS-'].update(translated_text,background_color_for_value='black', visible=True, autoscroll=True)
+                else:
                     overlay_translation_window = make_overlay_translation_window(100*' ')
-                overlay_translation_window['-ML-OVERLAY-DST-PARTIAL-RESULTS-'].update(translated_text,background_color_for_value='black', visible=True, autoscroll=True)
+                    overlay_translation_window['-ML-OVERLAY-DST-PARTIAL-RESULTS-'].update(translated_text,background_color_for_value='black', visible=True, autoscroll=True)
+
             else:
                 overlay_translation_window.Hide()
 
             if not (sys.platform == "win32"):
                 main_window.TKroot.attributes('-topmost', 1)
                 main_window.TKroot.attributes('-topmost', 0)
 
@@ -3181,47 +3183,47 @@
             total = pb[1]
             percentage = pb[2]
             progress = pb[3]
 
             FONT = ("Helvetica", 10)
             sg.set_options(font=FONT)
 
-            progressbar.UnHide()
+            if progressbar:
+                progressbar.UnHide()
+            else:
+                progressbar = make_progress_bar_window("", 100)
 
             progressbar['-INFO-'].update(info)
             progressbar['-PERCENTAGE-'].update(percentage)
             progressbar['-PROGRESS-'].update(progress)
             if progress == total:
                 time.sleep(1)
-                progressbar.close()
+                progressbar.Hide()
 
 
         elif event == '-EVENT-TRANSCRIBE-PREPARE-WINDOW-':
 
             prepare = values[event]
 
             if prepare:
 
                 FONT = ("Helvetica", 10)
                 sg.set_options(font=FONT)
-                #transcribe_window.UnHide()
                 transcribe_window = make_transcribe_window("", 100)
 
                 for element in transcribe_window.element_list():
                     if isinstance(element, sg.Text) or isinstance(element, sg.Multiline):
                         element.update(font=FONT)
                     if isinstance(element, sg.Button):
                         transcribe_window['-CANCEL-'].Widget.config(font=FONT)
 
                 transcribe_window['-OUTPUT-MESSAGES-'].update("")
                 transcribe_window['-INFO-'].update("Progress info")
                 transcribe_window['-PROGRESS-'].update(0)
                 transcribe_window['-PERCENTAGE-'].update("0%")
-                move_center(transcribe_window)
-                transcribe_window.refresh()
 
 
         elif event == '-EVENT-TRANSCRIBE-SEND-MESSAGES-':
 
             m = values[event]
             window_key = m[0]
             msg = m[1]
```

### Comparing `pyvosklivesubtitle-0.1.6/pyvosklivesubtitle.egg-info/PKG-INFO` & `pyvosklivesubtitle-0.1.7/pyvosklivesubtitle.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,29 +1,31 @@
-Metadata-Version: 2.1
-Name: pyvosklivesubtitle
-Version: 0.1.6
-Summary: A Python based desktop aplication that can RECOGNIZE any live streaming in 21 languages that supported by VOSK then TRANSLATE and display it as LIVE SUBTITLES
-Home-page: https://github.com/botbahlul/pyvosklivesubtitle
-Author: Bot Bahlul
-Author-email: bot.bahlul@gmail.com
-License: MIT License
-        
-        Copyright (c) 2022 Bot Bahlul
-        
-        Permission is hereby granted, free of charge, to any person obtaining a copy
-        of this software and associated documentation files (the "Software"), to deal
-        in the Software without restriction, including without limitation the rights
-        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-        copies of the Software, and to permit persons to whom the Software is
-        furnished to do so, subject to the following conditions:
-        
-        The above copyright notice and this permission notice shall be included in all
-        copies or substantial portions of the Software.
-        
-        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-        SOFTWARE.
-        
+Metadata-Version: 1.0
+Name: pyvosklivesubtitle
+Version: 0.1.7
+Summary: A Python based desktop aplication that can RECOGNIZE any live streaming in 21 languages that supported by VOSK then TRANSLATE and display it as LIVE SUBTITLES
+Home-page: https://github.com/botbahlul/pyvosklivesubtitle
+Author: Bot Bahlul
+Author-email: bot.bahlul@gmail.com
+License: MIT License
+
+Copyright (c) 2022 Bot Bahlul
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
+
+Description: UNKNOWN
+Platform: UNKNOWN
```

### Comparing `pyvosklivesubtitle-0.1.6/setup.py` & `pyvosklivesubtitle-0.1.7/setup.py`

 * *Files identical despite different names*

