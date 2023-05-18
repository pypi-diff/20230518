# Comparing `tmp/seaplayer-0.3.6.tar.gz` & `tmp/seaplayer-0.4a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "seaplayer-0.3.6.tar", max compression
+gzip compressed data, was "seaplayer-0.4a1.tar", max compression
```

## Comparing `seaplayer-0.3.6.tar` & `seaplayer-0.4a1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0     1085 2023-04-25 14:05:19.406661 seaplayer-0.3.6/LICENSE
--rw-r--r--   0        0        0     1020 2023-05-18 02:14:51.744856 seaplayer-0.3.6/pyproject.toml
--rw-r--r--   0        0        0     1117 2023-05-17 19:33:47.703429 seaplayer-0.3.6/README.md
--rw-r--r--   0        0        0        0 2023-05-02 23:42:08.763410 seaplayer-0.3.6/seaplayer/__init__.py
--rw-r--r--   0        0        0      295 2023-05-17 19:11:05.795693 seaplayer-0.3.6/seaplayer/__main__.py
--rw-r--r--   0        0        0    14705 2023-05-10 21:24:30.252393 seaplayer-0.3.6/seaplayer/assets/image-not-found.png
--rw-r--r--   0        0        0     3512 2023-05-18 02:07:26.903061 seaplayer-0.3.6/seaplayer/codecs.py
--rw-r--r--   0        0        0     1201 2023-05-18 01:55:53.292653 seaplayer-0.3.6/seaplayer/codeсbase.py
--rw-r--r--   0        0        0     5596 2023-05-16 23:08:28.381945 seaplayer-0.3.6/seaplayer/config.py
--rw-r--r--   0        0        0        0 2023-05-03 15:09:20.919585 seaplayer-0.3.6/seaplayer/css/configurate.css
--rw-r--r--   0        0        0      979 2023-05-05 21:48:10.082210 seaplayer-0.3.6/seaplayer/css/objects.css
--rw-r--r--   0        0        0      595 2023-05-03 14:02:48.505884 seaplayer-0.3.6/seaplayer/css/seaplayer.css
--rw-r--r--   0        0        0      278 2023-05-02 23:29:23.509840 seaplayer-0.3.6/seaplayer/css/unknown.css
--rw-r--r--   0        0        0      374 2023-05-10 16:57:45.981727 seaplayer-0.3.6/seaplayer/exceptions.py
--rw-r--r--   0        0        0     1404 2023-05-18 01:39:22.675700 seaplayer-0.3.6/seaplayer/functions.py
--rw-r--r--   0        0        0        0 2023-05-02 22:35:56.414811 seaplayer-0.3.6/seaplayer/modules/__init__.py
--rw-r--r--   0        0        0     2036 2023-05-12 20:40:27.939248 seaplayer-0.3.6/seaplayer/modules/colorizer.py
--rw-r--r--   0        0        0    11744 2023-05-18 01:37:18.892848 seaplayer-0.3.6/seaplayer/objects.py
--rw-r--r--   0        0        0     5980 2023-05-10 19:09:06.370823 seaplayer-0.3.6/seaplayer/screens.py
--rw-r--r--   0        0        0    15622 2023-05-18 02:09:10.796147 seaplayer-0.3.6/seaplayer/seaplayer.py
--rw-r--r--   0        0        0     4192 2023-05-18 01:32:00.602445 seaplayer-0.3.6/seaplayer/types.py
--rw-r--r--   0        0        0     2137 1970-01-01 00:00:00.000000 seaplayer-0.3.6/PKG-INFO
+-rw-r--r--   0        0        0     1085 2023-04-25 14:05:19.406661 seaplayer-0.4a1/LICENSE
+-rw-r--r--   0        0        0     1020 2023-05-18 13:45:29.858208 seaplayer-0.4a1/pyproject.toml
+-rw-r--r--   0        0        0     1117 2023-05-17 19:33:47.703429 seaplayer-0.4a1/README.md
+-rw-r--r--   0        0        0        0 2023-05-02 23:42:08.763410 seaplayer-0.4a1/seaplayer/__init__.py
+-rw-r--r--   0        0        0      295 2023-05-17 19:11:05.795693 seaplayer-0.4a1/seaplayer/__main__.py
+-rw-r--r--   0        0        0    14705 2023-05-10 21:24:30.252393 seaplayer-0.4a1/seaplayer/assets/image-not-found.png
+-rw-r--r--   0        0        0     4485 2023-05-18 13:23:04.171040 seaplayer-0.4a1/seaplayer/codecs.py
+-rw-r--r--   0        0        0     1201 2023-05-18 01:55:53.292653 seaplayer-0.4a1/seaplayer/codeсbase.py
+-rw-r--r--   0        0        0     5596 2023-05-16 23:08:28.381945 seaplayer-0.4a1/seaplayer/config.py
+-rw-r--r--   0        0        0        0 2023-05-03 15:09:20.919585 seaplayer-0.4a1/seaplayer/css/configurate.css
+-rw-r--r--   0        0        0      979 2023-05-05 21:48:10.082210 seaplayer-0.4a1/seaplayer/css/objects.css
+-rw-r--r--   0        0        0      595 2023-05-03 14:02:48.505884 seaplayer-0.4a1/seaplayer/css/seaplayer.css
+-rw-r--r--   0        0        0      278 2023-05-02 23:29:23.509840 seaplayer-0.4a1/seaplayer/css/unknown.css
+-rw-r--r--   0        0        0      374 2023-05-10 16:57:45.981727 seaplayer-0.4a1/seaplayer/exceptions.py
+-rw-r--r--   0        0        0     1282 2023-05-18 12:57:45.664141 seaplayer-0.4a1/seaplayer/functions.py
+-rw-r--r--   0        0        0        0 2023-05-02 22:35:56.414811 seaplayer-0.4a1/seaplayer/modules/__init__.py
+-rw-r--r--   0        0        0     2036 2023-05-12 20:40:27.939248 seaplayer-0.4a1/seaplayer/modules/colorizer.py
+-rw-r--r--   0        0        0    11808 2023-05-18 13:14:33.257395 seaplayer-0.4a1/seaplayer/objects.py
+-rw-r--r--   0        0        0     5980 2023-05-10 19:09:06.370823 seaplayer-0.4a1/seaplayer/screens.py
+-rw-r--r--   0        0        0    15585 2023-05-18 13:44:57.047839 seaplayer-0.4a1/seaplayer/seaplayer.py
+-rw-r--r--   0        0        0     4159 2023-05-18 12:58:01.336447 seaplayer-0.4a1/seaplayer/types.py
+-rw-r--r--   0        0        0     2137 1970-01-01 00:00:00.000000 seaplayer-0.4a1/PKG-INFO
```

### Comparing `seaplayer-0.3.6/LICENSE` & `seaplayer-0.4a1/LICENSE`

 * *Files identical despite different names*

### Comparing `seaplayer-0.3.6/pyproject.toml` & `seaplayer-0.4a1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "SeaPlayer"
-version = "0.3.6"
+version = "0.4a1"
 description = "SeaPlayer is a player that works in the terminal."
 repository = "https://github.com/romanin-rf/SeaPlayer"
 authors = ["Romanin <semina054@gmail.com>"]
 keywords = ["tui", "player", "seaplayer", "wav", "mp3", "ogg", "midi"]
 license = "MIT"
 readme = "README.md"
 packages = [{ include = "seaplayer" }]
```

### Comparing `seaplayer-0.3.6/README.md` & `seaplayer-0.4a1/README.md`

 * *Files identical despite different names*

### Comparing `seaplayer-0.3.6/seaplayer/assets/image-not-found.png` & `seaplayer-0.4a1/seaplayer/assets/image-not-found.png`

 * *Files identical despite different names*

### Comparing `seaplayer-0.3.6/seaplayer/codecs.py` & `seaplayer-0.4a1/seaplayer/codecs.py`

 * *Files 20% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 from playsoundsimple import Sound
 from playsoundsimple.units import SOUND_FONTS_PATH
 # > Typing
 from typing import Optional
 # > Local Imports
 from .codeсbase import CodecBase
 
-# ! Codec for MP3 & OGG & WAV files
-class Mp3OggWaveCodec(CodecBase):
-    codec_name: str = "MP3/OGG/WAVE"
+# ! MP3 Codec
+class MP3Codec(CodecBase):
+    codec_name: str = "MP3"
     
     # ! Testing
     @staticmethod
     def is_this_codec(path: str) -> bool:
-        try: Sound(path) ; return True
-        except: return False
+        with open(path, "rb") as file:
+            return file.read(3) == b'ID3'
     
     @staticmethod
     async def aio_is_this_codec(path: str) -> bool:
-        try: Sound(path) ; return True
-        except: return False
+        async with aiofiles.open(path, "rb") as file:
+            return await file.read(3) == b'ID3'
     
     # ! Initialized
     def __init__(self, path: str, **kwargs) -> None:
         self.name = os.path.abspath(path)
         self._sound = Sound(self.name)
     
     def __sha1__(self, buffer_size: int) -> str:
@@ -79,16 +79,48 @@
     def pause(self) -> None: self._sound.pause()
     def unpause(self) -> None: self._sound.unpause()
     def get_volume(self) -> float: return self._sound.get_volume()
     def set_volume(self, value: float) -> None: self._sound.set_volume(value)
     def get_pos(self) -> float: return self._sound.get_pos()
     def set_pos(self, value: float) -> None: self._sound.set_pos(value)
 
+# ! OGG Codec
+class OGGCodec(MP3Codec):
+    codec_name: str = "OGG"
+    
+    # ! Testing
+    @staticmethod
+    def is_this_codec(path: str) -> bool:
+        with open(path, "rb") as file:
+            return file.read(4) == b'OggS'
+    
+    @staticmethod
+    async def aio_is_this_codec(path: str) -> bool:
+        async with aiofiles.open(path, "rb") as file:
+            return await file.read(4) == b'OggS'
+
+# ! WAVE Codec
+class WAVECodec(MP3Codec):
+    codec_name: str = "WAVE"
+    
+    # ! Testing
+    @staticmethod
+    def is_this_codec(path: str) -> bool:
+        with open(path, "rb") as file:
+            signature = file.read(4)
+        return (signature == b'WAVE') or (signature == b'RIFF')
+    
+    @staticmethod
+    async def aio_is_this_codec(path: str) -> bool:
+        async with aiofiles.open(path, "rb") as file:
+            signature = await file.read(4)
+        return (signature == b'WAVE') or (signature == b'RIFF')
+
 # ! MIDI Codec
-class MIDICodec(Mp3OggWaveCodec):
+class MIDICodec(MP3Codec):
     codec_name: str = "MIDI"
     
     # ! Testing
     @staticmethod
     def is_this_codec(path: str) -> bool:
         with open(path, 'rb') as file:
             return file.read(4) == b"MThd"
```

### Comparing `seaplayer-0.3.6/seaplayer/codeсbase.py` & `seaplayer-0.4a1/seaplayer/codeсbase.py`

 * *Files identical despite different names*

### Comparing `seaplayer-0.3.6/seaplayer/config.py` & `seaplayer-0.4a1/seaplayer/config.py`

 * *Files identical despite different names*

### Comparing `seaplayer-0.3.6/seaplayer/css/objects.css` & `seaplayer-0.4a1/seaplayer/css/objects.css`

 * *Files identical despite different names*

### Comparing `seaplayer-0.3.6/seaplayer/css/seaplayer.css` & `seaplayer-0.4a1/seaplayer/css/seaplayer.css`

 * *Files identical despite different names*

### Comparing `seaplayer-0.3.6/seaplayer/functions.py` & `seaplayer-0.4a1/seaplayer/functions.py`

 * *Files 4% similar despite different names*

```diff
@@ -38,10 +38,7 @@
         return f"{sound.title}"
     try: return f"{os.path.basename(sound.name)}"
     except: return sound.name
 
 def image_from_bytes(data: Optional[bytes]) -> Optional[Image.Image]:
     if data is not None: return Image.open(BytesIO(data))
 
-def is_midi_file(filepath: str) -> bool:
-    with open(filepath, 'rb') as file:
-        return file.read(4) == b"MThd"
```

### Comparing `seaplayer-0.3.6/seaplayer/modules/colorizer.py` & `seaplayer-0.4a1/seaplayer/modules/colorizer.py`

 * *Files identical despite different names*

### Comparing `seaplayer-0.3.6/seaplayer/objects.py` & `seaplayer-0.4a1/seaplayer/objects.py`

 * *Files 1% similar despite different names*

```diff
@@ -73,19 +73,20 @@
     def get_sound(self, sound_uuid: str) -> Optional[CodecBase]: return self.music_list.get(sound_uuid)
     
     async def aio_add_sound(self, sound: CodecBase):
         sound_uuid = await self.music_list.aio_add(sound)
         await self.append(
             MusicListViewItem(
                 f"{get_sound_basename(sound)}",
-                "{duration} sec, {channel_mode}, {samplerate} Hz, {bitrate} kbps".format(
+                "{duration} sec, {channel_mode}, {samplerate} Hz, {bitrate} kbps, {codec_name}".format(
                     duration=round(sound.duration),
                     channel_mode="Mono" if sound.channels <= 1 else "Stereo",
                     samplerate=round(sound.samplerate),
-                    bitrate=round(sound.bitrate / 1000)
+                    bitrate=round(sound.bitrate / 1000),
+                    codec_name=sound.codec_name
                 ),
                 sound.name,
                 sound_uuid
             )
         )
         return sound_uuid
```

### Comparing `seaplayer-0.3.6/seaplayer/screens.py` & `seaplayer-0.4a1/seaplayer/screens.py`

 * *Files identical despite different names*

### Comparing `seaplayer-0.3.6/seaplayer/seaplayer.py` & `seaplayer-0.4a1/seaplayer/seaplayer.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,36 +1,33 @@
 import os
 import sys
 import glob
 import asyncio
 from platformdirs import user_config_dir
-# > Sound Works
-from playsoundsimple.units import SOUND_FONTS_PATH
 # > Graphics
 from textual import on
+from textual.binding import Binding
 from textual.app import App, ComposeResult
 from textual.containers import Horizontal, Vertical
 from textual.widgets import Header, Footer, Static, Label, Input, Button
-from textual.binding import Binding
 # > Image Works
 from PIL.Image import Resampling
 # > Typing
 from typing import Optional, Literal, Tuple, List, Type
 # > Local Imports
 from .config import *
 from .objects import *
 from .codeсbase import CodecBase
-from .codecs import Mp3OggWaveCodec, MIDICodec
 from .functions import check_status, image_from_bytes
-from .screens import Unknown, UNKNOWN_OPEN_KEY, Configurate
-
+from .screens import Unknown, Configurate, UNKNOWN_OPEN_KEY
+from .codecs import MP3Codec, WAVECodec, OGGCodec, MIDICodec
 
 # ! Metadata
 __title__ = "SeaPlayer"
-__version__ = "0.3.6"
+__version__ = "0.4a1"
 __author__ = "Romanin"
 __email__ = "semina054@gmail.com"
 __url__ = "https://github.com/romanin-rf/SeaPlayer"
 
 # ! Paths
 if getattr(sys, 'frozen', False) and hasattr(sys, '_MEIPASS'):
     LOCALDIR = os.path.dirname(sys.executable)
@@ -97,15 +94,15 @@
     last_playback_status: Optional[Literal["Stoped", "Playing", "Paused"]] = None
     playback_mode: int = 0
     playback_mode_blocked: bool = False
     last_paths_globalized: List[str] = []
     started: bool = True
     
     # ! Codecs Configuration
-    CODECS: List[Type[CodecBase]] = [ Mp3OggWaveCodec, MIDICodec ]
+    CODECS: List[Type[CodecBase]] = [ MP3Codec, WAVECodec, OGGCodec, MIDICodec ]
     CODECS_KWARGS: Dict[str, Any] = {"sound_font_path": config.sound_font_path}
     
     # ! Inherited Functions
     async def action_push_screen(self, screen: str) -> None:
         if self.SCREENS[screen].id != self.screen.id:
             await super().action_push_screen(screen)
     
@@ -268,15 +265,15 @@
     @on(Button.Pressed, "#plus-sound")
     async def bp_plus_sound(self) -> None:
         path = self.music_list_add_input.value
         self.music_list_add_input.value = ""
         
         if path.replace(" ", "") != "":
             try: self.last_paths_globalized = glob.glob(path, recursive=self.config.recursive_search)
-            except: self.last_paths_globalized = []
+            except: self.last_paths_globalized = [ path ]
             if len(self.last_paths_globalized) > 0:
                 self.run_worker(
                     self.add_sounds_to_list,
                     name="ADD_SOUND",
                     group="PLAYLIST_UPDATE",
                     description="The process of adding sounds to a playlist."
                 )
```

### Comparing `seaplayer-0.3.6/seaplayer/types.py` & `seaplayer-0.4a1/seaplayer/types.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-import aiofiles
-import hashlib
 from pathlib import Path
 # > Typing
 from typing import Dict, Optional, Tuple, Any
 # > Local Imports
 from .codeсbase import CodecBase
 from .exceptions import (
     PathNotExistsError,
```

### Comparing `seaplayer-0.3.6/PKG-INFO` & `seaplayer-0.4a1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seaplayer
-Version: 0.3.6
+Version: 0.4a1
 Summary: SeaPlayer is a player that works in the terminal.
 Home-page: https://github.com/romanin-rf/SeaPlayer
 License: MIT
 Keywords: tui,player,seaplayer,wav,mp3,ogg,midi
 Author: Romanin
 Author-email: semina054@gmail.com
 Requires-Python: >=3.9,<4.0
```

