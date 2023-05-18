# Comparing `tmp/neon_speech-3.3.2a2-py3-none-any.whl.zip` & `tmp/neon_speech-3.3.2a3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,16 +1,16 @@
-Zip file size: 23683 bytes, number of entries: 14
--rw-r--r--  2.0 unx     1831 b- defN 23-May-11 23:44 neon_speech/__init__.py
--rw-r--r--  2.0 unx     2632 b- defN 23-May-11 23:44 neon_speech/__main__.py
--rw-r--r--  2.0 unx     5085 b- defN 23-May-11 23:44 neon_speech/cli.py
--rw-r--r--  2.0 unx    10058 b- defN 23-May-11 23:44 neon_speech/listener.py
--rw-r--r--  2.0 unx     5115 b- defN 23-May-11 23:44 neon_speech/mic.py
--rw-r--r--  2.0 unx    21946 b- defN 23-May-11 23:44 neon_speech/service.py
--rw-r--r--  2.0 unx     4374 b- defN 23-May-11 23:44 neon_speech/stt.py
--rw-r--r--  2.0 unx     4294 b- defN 23-May-11 23:44 neon_speech/utils.py
--rw-r--r--  2.0 unx     1634 b- defN 23-May-11 23:44 neon_speech-3.3.2a2.dist-info/LICENSE.md
--rw-r--r--  2.0 unx     2559 b- defN 23-May-11 23:44 neon_speech-3.3.2a2.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-11 23:44 neon_speech-3.3.2a2.dist-info/WHEEL
--rw-r--r--  2.0 unx      111 b- defN 23-May-11 23:44 neon_speech-3.3.2a2.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       12 b- defN 23-May-11 23:44 neon_speech-3.3.2a2.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1144 b- defN 23-May-11 23:44 neon_speech-3.3.2a2.dist-info/RECORD
-14 files, 60887 bytes uncompressed, 21791 bytes compressed:  64.2%
+Zip file size: 23638 bytes, number of entries: 14
+-rw-r--r--  2.0 unx     1831 b- defN 23-May-18 04:21 neon_speech/__init__.py
+-rw-r--r--  2.0 unx     2649 b- defN 23-May-18 04:21 neon_speech/__main__.py
+-rw-r--r--  2.0 unx     5085 b- defN 23-May-18 04:21 neon_speech/cli.py
+-rw-r--r--  2.0 unx     9921 b- defN 23-May-18 04:21 neon_speech/listener.py
+-rw-r--r--  2.0 unx     5107 b- defN 23-May-18 04:21 neon_speech/mic.py
+-rw-r--r--  2.0 unx    21918 b- defN 23-May-18 04:21 neon_speech/service.py
+-rw-r--r--  2.0 unx     4478 b- defN 23-May-18 04:21 neon_speech/stt.py
+-rw-r--r--  2.0 unx     4285 b- defN 23-May-18 04:21 neon_speech/utils.py
+-rw-r--r--  2.0 unx     1634 b- defN 23-May-18 04:22 neon_speech-3.3.2a3.dist-info/LICENSE.md
+-rw-r--r--  2.0 unx     2577 b- defN 23-May-18 04:22 neon_speech-3.3.2a3.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-18 04:22 neon_speech-3.3.2a3.dist-info/WHEEL
+-rw-r--r--  2.0 unx      111 b- defN 23-May-18 04:22 neon_speech-3.3.2a3.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       12 b- defN 23-May-18 04:22 neon_speech-3.3.2a3.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1143 b- defN 23-May-18 04:22 neon_speech-3.3.2a3.dist-info/RECORD
+14 files, 60843 bytes uncompressed, 21746 bytes compressed:  64.3%
```

## zipnote {}

```diff
@@ -18,26 +18,26 @@
 
 Filename: neon_speech/stt.py
 Comment: 
 
 Filename: neon_speech/utils.py
 Comment: 
 
-Filename: neon_speech-3.3.2a2.dist-info/LICENSE.md
+Filename: neon_speech-3.3.2a3.dist-info/LICENSE.md
 Comment: 
 
-Filename: neon_speech-3.3.2a2.dist-info/METADATA
+Filename: neon_speech-3.3.2a3.dist-info/METADATA
 Comment: 
 
-Filename: neon_speech-3.3.2a2.dist-info/WHEEL
+Filename: neon_speech-3.3.2a3.dist-info/WHEEL
 Comment: 
 
-Filename: neon_speech-3.3.2a2.dist-info/entry_points.txt
+Filename: neon_speech-3.3.2a3.dist-info/entry_points.txt
 Comment: 
 
-Filename: neon_speech-3.3.2a2.dist-info/top_level.txt
+Filename: neon_speech-3.3.2a3.dist-info/top_level.txt
 Comment: 
 
-Filename: neon_speech-3.3.2a2.dist-info/RECORD
+Filename: neon_speech-3.3.2a3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## neon_speech/__main__.py

```diff
@@ -26,26 +26,26 @@
 # NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS
 # SOFTWARE,  EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
 from ovos_utils import wait_for_exit_signal
 from neon_utils.configuration_utils import init_config_dir
 from neon_utils.log_utils import init_log
 from ovos_utils.log import LOG
+from ovos_utils.process_utils import PIDLock as Lock
 
 
 def main(*args, **kwargs):
     # Initialize configuration
     init_config_dir()
     init_log(log_name="voice")
     if kwargs.get("config"):
         LOG.warning("Found config kwarg, updating to 'speech_config'")
         kwargs["speech_config"] = kwargs.pop("config")
 
-    from mycroft.lock import Lock
-    from mycroft.util.process_utils import reset_sigint_handler
+    from ovos_utils.process_utils import reset_sigint_handler
     from neon_speech.service import NeonSpeechClient
     reset_sigint_handler()
     Lock("speech")
     service = NeonSpeechClient(*args, **kwargs)
     service.start()
     wait_for_exit_signal()
     service.shutdown()
```

## neon_speech/listener.py

```diff
@@ -25,27 +25,24 @@
 # LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING
 # NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS
 # SOFTWARE,  EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
 from queue import Queue
 from threading import Event
 from typing import List
-
-# from neon_utils.configuration_utils import get_neon_device_type
 from ovos_utils.log import LOG
 from ovos_utils.metrics import Stopwatch
 from ovos_config.config import Configuration
-from mycroft.client.speech.listener import RecognizerLoop, AudioConsumer, \
-    AudioProducer, recognizer_conf_hash, \
-    find_input_device, RecognizerLoopState
-from mycroft.client.speech.mic import MutableMicrophone
+from ovos_listener.listener import RecognizerLoop, AudioConsumer, \
+    AudioProducer, recognizer_conf_hash, find_input_device, RecognizerLoopState
+from ovos_listener.mic import MutableMicrophone
+from neon_utils.parse_utils import clean_quotes
 
 from neon_speech.mic import NeonResponsiveRecognizer
 from neon_speech.stt import STTFactory
-from neon_utils.parse_utils import clean_quotes
 
 
 class NeonAudioConsumer(AudioConsumer):
     def process(self, audio, context=None):
         context = context or {}
         # NOTE: in the parent class context is a string for lang
         # in neon we pass a dict around instead
@@ -118,15 +115,16 @@
     """ EventEmitter loop running speech recognition.
 
     Local wake word recognizer and remote general speech recognition.
     """
     def __init__(self, bus, watchdog=None, stt=None, fallback_stt=None):
         self.config_loaded = Event()
         self.microphone = None
-        super().__init__(bus, watchdog, stt, fallback_stt)
+        stt = stt or STTFactory.create(Configuration())
+        RecognizerLoop.__init__(self, bus, watchdog, stt, fallback_stt)
 
     def _load_config(self):
         """
         Load configuration parameters from configuration and initialize
         self.microphone, self.responsive_recognizer
         """
         # self.config_core = self._init_config_core or Configuration.get()
@@ -166,14 +164,18 @@
                     LOG.exception(e)
         self.create_hotword_engines()
         self.state = RecognizerLoopState()
         self.responsive_recognizer = NeonResponsiveRecognizer(self)
         self.config_loaded.set()
         # TODO: Update recognizer to support passed config
 
+    def run(self):
+        LOG.debug("Running RecognizerLoop")
+        RecognizerLoop.run(self)
+
     def init_fallback_stt(self):
         if not self.fallback_stt:
             clazz = self.get_fallback_stt()
             if clazz:
                 LOG.debug(f"Initializing fallback STT engine")
                 self.fallback_stt = clazz()
 
@@ -185,22 +187,17 @@
         self.queue = Queue()
         self.audio_consumer = NeonAudioConsumer(self)
         self.audio_consumer.name = "audio_consumer"
         self.audio_consumer.start()
         self.audio_producer = AudioProducer(self)
         self.audio_producer.name = "audio_producer"
         try:
-            # TODO: Patching bug in ovos-core
-            self.microphone._start()
-            self.microphone._stop()
-            LOG.info("Microphone valid")
             self.audio_producer.start()
         except Exception as e:
             LOG.exception(e)
-            LOG.error("Skipping audio_producer init")
 
     def stop(self):
         self.state.running = False
         if self.audio_producer:
             self.audio_producer.stop()
 
         # stop wake word detectors
```

## neon_speech/mic.py

```diff
@@ -26,15 +26,15 @@
 # NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS
 # SOFTWARE,  EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
 from ovos_utils.log import LOG
 from speech_recognition import AudioSource, AudioData
 from neon_transformers.audio_transformers import AudioTransformersService
 
-from mycroft.client.speech.mic import ResponsiveRecognizer
+from ovos_listener.mic import ResponsiveRecognizer
 
 
 class NeonResponsiveRecognizer(ResponsiveRecognizer):
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self._in_speech = False
```

## neon_speech/service.py

```diff
@@ -28,28 +28,28 @@
 
 import os
 from tempfile import mkstemp
 
 from threading import Thread, Lock
 from time import time
 
-from mycroft.listener.mic import ListeningMode
+from ovos_listener.mic import ListeningMode
 from ovos_utils.process_utils import StatusCallbackMap, ProcessStatus
 from pydub import AudioSegment
 from speech_recognition import AudioData
 
 from neon_utils.file_utils import decode_base64_string_to_file
 from neon_utils.messagebus_utils import get_messagebus
 from ovos_utils.log import LOG
 from neon_utils.configuration_utils import get_neon_user_config
 from neon_utils.user_utils import apply_local_user_profile_updates
 from ovos_utils.json_helper import merge_dict
-from mycroft_bus_client import Message
+from ovos_bus_client import Message
 
-from mycroft.client.speech.service import SpeechService
+from ovos_listener.service import SpeechService
 from ovos_config.config import Configuration, update_mycroft_config
 
 from neon_speech.listener import NeonRecognizerLoop
 from neon_speech.stt import STTFactory
 
 
 def on_ready():
@@ -90,15 +90,15 @@
         """
         if speech_config:
             LOG.info("Updating global config with passed config")
             from neon_speech.utils import patch_config
             patch_config(speech_config)
         # Don't init SpeechClient, because we're overriding self.loop
         Thread.__init__(self)
-        self.setDaemon(daemonic)
+        self.daemon = daemonic
         # Init messagebus and handlers
         self.bus = bus or get_messagebus()
         from neon_utils.signal_utils import init_signal_handlers, \
             init_signal_bus
         init_signal_bus(self.bus)
         init_signal_handlers()
 
@@ -127,15 +127,15 @@
 
     def shutdown(self):
         LOG.info("Shutting Down")
         self.status.set_stopping()
         self.loop.stop()
 
     def connect_bus_events(self):
-        super(NeonSpeechClient, self).connect_bus_events()
+        SpeechService.connect_bus_events(self)
         # Register handler for internet (re-)connection
         self.bus.on("mycroft.internet.connected",
                     self.handle_internet_connected)
         self.bus.on("ovos.phal.wifi.plugin.fully_offline",
                     self.handle_offline)
         self.bus.once("mycroft.ready", self.handle_ready)
```

## neon_speech/stt.py

```diff
@@ -68,15 +68,15 @@
 class STTFactory(OVOSSTTFactory):
     @staticmethod
     def create(config=None, results_event: Event = None):
         get_stt_config(config)
         if config and not config.get("module"):
             # No module, try getting stt config from passed config
             config = config.get("stt")
-            LOG.info("Using passed config")
+            LOG.debug("Using passed config")
         if not config:  # No config, go get it
             config = Configuration().get("stt", {})
             from ovos_config.locations import USER_CONFIG
             LOG.info(f"Getting config from disk: {USER_CONFIG}")
 
         LOG.info(f"Create STT with config: {config}")
         clazz = OVOSSTTFactory.get_class(config)
@@ -84,11 +84,13 @@
             LOG.warning(f"{config.get('module')} plugin not found, "
                         f"falling back to Chromium STT")
             config["module"] = config.get("fallback_module") or "google"
             clazz = OVOSSTTFactory.get_class(config)
             if not clazz:
                 raise ValueError("fallback plugin not found")
         if issubclass(clazz, StreamingSTT):
+            LOG.debug(f"Returning WrappedSTT {clazz}")
             return WrappedSTT(clazz, config=config.get(config['module']),
                               results_event=results_event)
         else:
+            LOG.debug(f"Returning STT {clazz}")
             return clazz(config=config)
```

## neon_speech/utils.py

```diff
@@ -21,31 +21,31 @@
 # CONTRIBUTORS  BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL,
 # EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO,
 # PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA,
 # OR PROFITS;  OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF
 # LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING
 # NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS
 # SOFTWARE,  EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+import importlib
 
 from tempfile import mkstemp
 from ovos_utils.log import LOG
 from neon_utils.packaging_utils import get_package_dependencies
 
 
 def patch_config(config: dict = None):
     """
     Write the specified speech configuration to the global config file
     :param config: Mycroft-compatible configuration override
     """
-    from ovos_config import USER_CONFIG, LocalConf
+    import ovos_config.config
 
     config = config or dict()
-    local_config = LocalConf(USER_CONFIG)
-    local_config.update(config)
-    local_config.store()
+    ovos_config.config.update_mycroft_config(config)
+    importlib.reload(ovos_config.config)
 
 
 def _plugin_to_package(plugin: str) -> str:
     """
     Get a PyPI spec for a known plugin entrypoint
     :param plugin: plugin spec (i.e. config['stt']['module'])
     :returns: package name associated with `plugin` or `plugin`
```

## Comparing `neon_speech-3.3.2a2.dist-info/LICENSE.md` & `neon_speech-3.3.2a3.dist-info/LICENSE.md`

 * *Files identical despite different names*

## Comparing `neon_speech-3.3.2a2.dist-info/METADATA` & `neon_speech-3.3.2a3.dist-info/METADATA`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: neon-speech
-Version: 3.3.2a2
+Version: 3.3.2a3
 Summary: Neon Speech Module
 Home-page: https://github.com/NeonGeckoCom/neon_speech
 Author: Neongecko
 Author-email: developers@neon.ai
 License: BSD-3-Clause
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
-Requires-Dist: ovos-core (~=0.0.7)
+Requires-Dist: ovos-listener (>=0.0.2a11,~=0.0.1)
 Requires-Dist: SpeechRecognition (~=3.8)
 Requires-Dist: PyAudio (~=0.2)
-Requires-Dist: mycroft-messagebus-client (~=0.10)
+Requires-Dist: ovos-bus-client (~=0.0.3)
 Requires-Dist: ovos-utils (~=0.0.30)
-Requires-Dist: ovos-plugin-manager (~=0.0.19)
+Requires-Dist: ovos-plugin-manager (>=0.0.23a17,~=0.0.19)
 Requires-Dist: pydub (~=0.23)
 Requires-Dist: click (~=8.0)
 Requires-Dist: click-default-group (~=1.2)
 Requires-Dist: neon-transformers (~=0.2)
 Requires-Dist: neon-utils[audio,network] (~=1.3)
 Requires-Dist: ovos-config (~=0.0.7)
 Requires-Dist: ovos-vad-plugin-webrtcvad (~=0.0.1)
```

## Comparing `neon_speech-3.3.2a2.dist-info/RECORD` & `neon_speech-3.3.2a3.dist-info/RECORD`

 * *Files 27% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 neon_speech/__init__.py,sha256=UDwbScPcnqA05m_zQmXnY6YeoL5j6NS_TaLj0mQdU_8,1831
-neon_speech/__main__.py,sha256=GYsKldh4iN7sY2kLnHtSYj1D56GQgdHuMXlUIf-d5ks,2632
+neon_speech/__main__.py,sha256=DfSfk3c7BYzyZesU0VcITr4MPu7LIXMqxD7dLew4PuE,2649
 neon_speech/cli.py,sha256=2BiU-fTcmOyT3CJ6gmoCtUsP7bAUcDOt8-MkPEfMJX0,5085
-neon_speech/listener.py,sha256=A0Q7wcznohmHI6YX9f7Jx7djl3AR97k2fLS0FZ9INIQ,10058
-neon_speech/mic.py,sha256=6M2l1zOqR6tPYrpIVWA76R8-GUfPKtt5iwiBCfqVTdg,5115
-neon_speech/service.py,sha256=AHGtBFu2eYK3YYyv027nTXkIaBlfChy8VquEhp6rNVg,21946
-neon_speech/stt.py,sha256=6zl0SgQ9ghsKbzoHG36TvV1qDGJnGx4qyPpwz0CQ3sA,4374
-neon_speech/utils.py,sha256=5RNtze-kwo-_WvYNk8GoqG8vVdkbPs6hBdpF7Pn7Iqc,4294
-neon_speech-3.3.2a2.dist-info/LICENSE.md,sha256=gxKa3HnxC7fSIlGFpLAiSAhQS22pIyVEyXmPQR2KlXM,1634
-neon_speech-3.3.2a2.dist-info/METADATA,sha256=ObDL8g3h6djapSet7yQOPyb_4xZAMqselCFyFFfZkSY,2559
-neon_speech-3.3.2a2.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-neon_speech-3.3.2a2.dist-info/entry_points.txt,sha256=Y5nCn6RrdZVozA3UnFkIX_43MJ5TF-bmlqsz3LA_9rM,111
-neon_speech-3.3.2a2.dist-info/top_level.txt,sha256=fXNizEfCNvNDWenv5znkv_2KPpvzwwsRM7S3sG7bllw,12
-neon_speech-3.3.2a2.dist-info/RECORD,,
+neon_speech/listener.py,sha256=Abwh5UxXYtnRlty4wA8dW0fW69YxbYRg6Gd0SJE8cGo,9921
+neon_speech/mic.py,sha256=uA_yi3hX_2yYx0G1ZkiCUu-IKZk37sCJUBERjGm3WhQ,5107
+neon_speech/service.py,sha256=RsbXxys1OqUDMwzMATndDqoTKnJXVhoWXWuYeYFTGUw,21918
+neon_speech/stt.py,sha256=K6z7Wvbl1uT-h1bxI6jCnuQHfijfDeNULlifF8LVh2A,4478
+neon_speech/utils.py,sha256=6axY_oHDqmIKIBvYhnuUIJoRZTwKyYif-isfc2wKPcI,4285
+neon_speech-3.3.2a3.dist-info/LICENSE.md,sha256=gxKa3HnxC7fSIlGFpLAiSAhQS22pIyVEyXmPQR2KlXM,1634
+neon_speech-3.3.2a3.dist-info/METADATA,sha256=d8Ff9lxIwAfxdSOW6jwDRKKylPjLMUPF6dpx7hVRZzI,2577
+neon_speech-3.3.2a3.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+neon_speech-3.3.2a3.dist-info/entry_points.txt,sha256=Y5nCn6RrdZVozA3UnFkIX_43MJ5TF-bmlqsz3LA_9rM,111
+neon_speech-3.3.2a3.dist-info/top_level.txt,sha256=fXNizEfCNvNDWenv5znkv_2KPpvzwwsRM7S3sG7bllw,12
+neon_speech-3.3.2a3.dist-info/RECORD,,
```

