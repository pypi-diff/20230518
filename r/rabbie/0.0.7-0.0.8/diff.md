# Comparing `tmp/rabbie-0.0.7.tar.gz` & `tmp/rabbie-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rabbie-0.0.7.tar", last modified: Thu May 11 11:44:22 2023, max compression
+gzip compressed data, was "rabbie-0.0.8.tar", last modified: Thu May 18 08:08:04 2023, max compression
```

## Comparing `rabbie-0.0.7.tar` & `rabbie-0.0.8.tar`

### file list

```diff
@@ -1,64 +1,68 @@
-drwxrwxrwx   0        0        0        0 2023-05-11 11:44:22.319122 rabbie-0.0.7/
--rw-rw-rw-   0        0        0     1077 2023-04-24 20:01:12.000000 rabbie-0.0.7/LICENSE
--rw-rw-rw-   0        0        0     7998 2023-05-11 11:44:22.318120 rabbie-0.0.7/PKG-INFO
--rw-rw-rw-   0        0        0     7522 2023-05-11 11:17:49.000000 rabbie-0.0.7/README.md
--rw-rw-rw-   0        0        0       63 2023-04-02 21:06:34.000000 rabbie-0.0.7/pyproject.toml
-drwxrwxrwx   0        0        0        0 2023-05-11 11:44:22.267123 rabbie-0.0.7/rabbie/
--rw-rw-rw-   0        0        0      230 2023-05-11 11:17:49.000000 rabbie-0.0.7/rabbie/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-11 11:44:22.284124 rabbie-0.0.7/rabbie/broker_types/
--rw-rw-rw-   0        0        0       60 2023-05-11 11:17:49.000000 rabbie-0.0.7/rabbie/broker_types/__init__.py
--rw-rw-rw-   0        0        0     4898 2023-05-11 11:34:26.000000 rabbie-0.0.7/rabbie/broker_types/channel.py
--rw-rw-rw-   0        0        0      182 2023-05-11 11:17:49.000000 rabbie-0.0.7/rabbie/broker_types/relayed_types.py
-drwxrwxrwx   0        0        0        0 2023-05-11 11:44:22.286121 rabbie-0.0.7/rabbie/connection/
--rw-rw-rw-   0        0        0       44 2023-05-11 11:17:49.000000 rabbie-0.0.7/rabbie/connection/__init__.py
--rw-rw-rw-   0        0        0      294 2023-05-11 11:17:49.000000 rabbie-0.0.7/rabbie/connection/details.py
-drwxrwxrwx   0        0        0        0 2023-05-11 11:44:22.289124 rabbie-0.0.7/rabbie/consumer/
--rw-rw-rw-   0        0        0      175 2023-05-11 11:17:49.000000 rabbie-0.0.7/rabbie/consumer/__init__.py
--rw-rw-rw-   0        0        0     6555 2023-05-11 11:42:49.000000 rabbie-0.0.7/rabbie/consumer/consumer.py
-drwxrwxrwx   0        0        0        0 2023-05-11 11:44:22.292122 rabbie-0.0.7/rabbie/consumer/listener/
--rw-rw-rw-   0        0        0       79 2023-04-24 20:01:12.000000 rabbie-0.0.7/rabbie/consumer/listener/__init__.py
--rw-rw-rw-   0        0        0     5200 2023-05-11 11:17:49.000000 rabbie-0.0.7/rabbie/consumer/listener/listener.py
--rw-rw-rw-   0        0        0      400 2023-05-11 11:17:49.000000 rabbie-0.0.7/rabbie/consumer/listener/listener_details.py
--rw-rw-rw-   0        0        0     3079 2023-05-11 11:17:49.000000 rabbie-0.0.7/rabbie/consumer/microconsumer.py
-drwxrwxrwx   0        0        0        0 2023-05-11 11:44:22.295121 rabbie-0.0.7/rabbie/decoder/
--rw-rw-rw-   0        0        0       78 2023-05-11 11:17:49.000000 rabbie-0.0.7/rabbie/decoder/__init__.py
--rw-rw-rw-   0        0        0      132 2023-04-24 20:01:12.000000 rabbie-0.0.7/rabbie/decoder/decoder.py
-drwxrwxrwx   0        0        0        0 2023-05-11 11:44:22.298121 rabbie-0.0.7/rabbie/decoder/decoders/
--rw-rw-rw-   0        0        0       78 2023-05-11 11:17:49.000000 rabbie-0.0.7/rabbie/decoder/decoders/__init__.py
--rw-rw-rw-   0        0        0      219 2023-05-11 11:17:49.000000 rabbie-0.0.7/rabbie/decoder/decoders/auto_decoder.py
--rw-rw-rw-   0        0        0      148 2023-04-24 20:01:12.000000 rabbie-0.0.7/rabbie/decoder/decoders/json_decoder.py
-drwxrwxrwx   0        0        0        0 2023-05-11 11:44:22.300125 rabbie-0.0.7/rabbie/decoder/exceptions/
--rw-rw-rw-   0        0        0       94 2023-03-29 12:21:12.000000 rabbie-0.0.7/rabbie/decoder/exceptions/__init__.py
--rw-rw-rw-   0        0        0       44 2023-03-29 12:19:53.000000 rabbie-0.0.7/rabbie/decoder/exceptions/decode_exception.py
-drwxrwxrwx   0        0        0        0 2023-05-11 11:44:22.302122 rabbie-0.0.7/rabbie/encoder/
--rw-rw-rw-   0        0        0       78 2023-05-11 11:17:49.000000 rabbie-0.0.7/rabbie/encoder/__init__.py
--rw-rw-rw-   0        0        0      197 2023-05-11 11:17:49.000000 rabbie-0.0.7/rabbie/encoder/encoder.py
-drwxrwxrwx   0        0        0        0 2023-05-11 11:44:22.305122 rabbie-0.0.7/rabbie/encoder/encoders/
--rw-rw-rw-   0        0        0       78 2023-05-11 11:17:49.000000 rabbie-0.0.7/rabbie/encoder/encoders/__init__.py
--rw-rw-rw-   0        0        0      461 2023-05-11 11:17:49.000000 rabbie-0.0.7/rabbie/encoder/encoders/auto_encoder.py
--rw-rw-rw-   0        0        0      215 2023-05-11 11:17:49.000000 rabbie-0.0.7/rabbie/encoder/encoders/json_encoder.py
-drwxrwxrwx   0        0        0        0 2023-05-11 11:44:22.306122 rabbie-0.0.7/rabbie/logger/
--rw-rw-rw-   0        0        0      312 2023-04-24 20:01:12.000000 rabbie-0.0.7/rabbie/logger/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-11 11:44:22.308122 rabbie-0.0.7/rabbie/producer/
--rw-rw-rw-   0        0        0       46 2023-05-11 11:17:49.000000 rabbie-0.0.7/rabbie/producer/__init__.py
--rw-rw-rw-   0        0        0     4584 2023-05-11 11:17:49.000000 rabbie-0.0.7/rabbie/producer/producer.py
-drwxrwxrwx   0        0        0        0 2023-05-11 11:44:22.311122 rabbie-0.0.7/rabbie/producer/publisher/
--rw-rw-rw-   0        0        0       34 2023-05-11 11:17:49.000000 rabbie-0.0.7/rabbie/producer/publisher/__init__.py
--rw-rw-rw-   0        0        0     3176 2023-05-11 11:17:49.000000 rabbie-0.0.7/rabbie/producer/publisher/publisher.py
-drwxrwxrwx   0        0        0        0 2023-05-11 11:44:22.313122 rabbie-0.0.7/rabbie/supervisor/
--rw-rw-rw-   0        0        0       50 2023-04-24 20:01:12.000000 rabbie-0.0.7/rabbie/supervisor/__init__.py
--rw-rw-rw-   0        0        0     4560 2023-04-24 20:01:12.000000 rabbie-0.0.7/rabbie/supervisor/supervisor.py
-drwxrwxrwx   0        0        0        0 2023-05-11 11:44:22.281121 rabbie-0.0.7/rabbie.egg-info/
--rw-rw-rw-   0        0        0     7998 2023-05-11 11:44:22.000000 rabbie-0.0.7/rabbie.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1338 2023-05-11 11:44:22.000000 rabbie-0.0.7/rabbie.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-11 11:44:22.000000 rabbie-0.0.7/rabbie.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       32 2023-05-11 11:44:22.000000 rabbie-0.0.7/rabbie.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-05-11 11:44:22.000000 rabbie-0.0.7/rabbie.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-11 11:44:22.319122 rabbie-0.0.7/setup.cfg
--rw-rw-rw-   0        0        0      854 2023-05-11 11:43:59.000000 rabbie-0.0.7/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-11 11:44:22.317120 rabbie-0.0.7/tests/
--rw-rw-rw-   0        0        0     4748 2023-05-11 11:17:49.000000 rabbie-0.0.7/tests/test_consumer.py
--rw-rw-rw-   0        0        0        0 2023-04-24 20:01:12.000000 rabbie-0.0.7/tests/test_decoder.py
--rw-rw-rw-   0        0        0        0 2023-04-24 20:01:12.000000 rabbie-0.0.7/tests/test_listener.py
--rw-rw-rw-   0        0        0        0 2023-04-24 20:01:12.000000 rabbie-0.0.7/tests/test_microconsumer.py
--rw-rw-rw-   0        0        0        0 2023-05-11 11:17:49.000000 rabbie-0.0.7/tests/test_producer.py
+drwxrwxrwx   0        0        0        0 2023-05-18 08:08:04.255935 rabbie-0.0.8/
+-rw-rw-rw-   0        0        0     1077 2023-04-24 20:01:12.000000 rabbie-0.0.8/LICENSE
+-rw-rw-rw-   0        0        0     9287 2023-05-18 08:08:04.254938 rabbie-0.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0     8813 2023-05-18 08:05:34.000000 rabbie-0.0.8/README.md
+-rw-rw-rw-   0        0        0       63 2023-04-02 21:06:34.000000 rabbie-0.0.8/pyproject.toml
+drwxrwxrwx   0        0        0        0 2023-05-18 08:08:04.196422 rabbie-0.0.8/rabbie/
+-rw-rw-rw-   0        0        0      265 2023-05-18 08:05:34.000000 rabbie-0.0.8/rabbie/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-18 08:08:04.212937 rabbie-0.0.8/rabbie/broker_types/
+-rw-rw-rw-   0        0        0       60 2023-05-11 11:17:49.000000 rabbie-0.0.8/rabbie/broker_types/__init__.py
+-rw-rw-rw-   0        0        0     4898 2023-05-11 11:34:26.000000 rabbie-0.0.8/rabbie/broker_types/channel.py
+-rw-rw-rw-   0        0        0      182 2023-05-11 11:17:49.000000 rabbie-0.0.8/rabbie/broker_types/relayed_types.py
+drwxrwxrwx   0        0        0        0 2023-05-18 08:08:04.214933 rabbie-0.0.8/rabbie/connection/
+-rw-rw-rw-   0        0        0       44 2023-05-11 11:17:49.000000 rabbie-0.0.8/rabbie/connection/__init__.py
+-rw-rw-rw-   0        0        0      294 2023-05-11 11:17:49.000000 rabbie-0.0.8/rabbie/connection/details.py
+drwxrwxrwx   0        0        0        0 2023-05-18 08:08:04.217934 rabbie-0.0.8/rabbie/consumer/
+-rw-rw-rw-   0        0        0      175 2023-05-11 11:17:49.000000 rabbie-0.0.8/rabbie/consumer/__init__.py
+-rw-rw-rw-   0        0        0     9107 2023-05-18 08:05:34.000000 rabbie-0.0.8/rabbie/consumer/consumer.py
+drwxrwxrwx   0        0        0        0 2023-05-18 08:08:04.221933 rabbie-0.0.8/rabbie/consumer/listener/
+-rw-rw-rw-   0        0        0      116 2023-05-18 08:05:34.000000 rabbie-0.0.8/rabbie/consumer/listener/__init__.py
+-rw-rw-rw-   0        0        0     7620 2023-05-18 08:05:34.000000 rabbie-0.0.8/rabbie/consumer/listener/listener.py
+-rw-rw-rw-   0        0        0      725 2023-05-18 08:05:34.000000 rabbie-0.0.8/rabbie/consumer/listener/listener_details.py
+-rw-rw-rw-   0        0        0      124 2023-05-18 08:05:34.000000 rabbie-0.0.8/rabbie/consumer/listener/listener_status.py
+-rw-rw-rw-   0        0        0     4150 2023-05-18 08:05:34.000000 rabbie-0.0.8/rabbie/consumer/microconsumer.py
+drwxrwxrwx   0        0        0        0 2023-05-18 08:08:04.223935 rabbie-0.0.8/rabbie/decoder/
+-rw-rw-rw-   0        0        0       78 2023-05-11 11:17:49.000000 rabbie-0.0.8/rabbie/decoder/__init__.py
+-rw-rw-rw-   0        0        0      132 2023-04-24 20:01:12.000000 rabbie-0.0.8/rabbie/decoder/decoder.py
+drwxrwxrwx   0        0        0        0 2023-05-18 08:08:04.226933 rabbie-0.0.8/rabbie/decoder/decoders/
+-rw-rw-rw-   0        0        0       78 2023-05-11 11:17:49.000000 rabbie-0.0.8/rabbie/decoder/decoders/__init__.py
+-rw-rw-rw-   0        0        0      219 2023-05-11 11:17:49.000000 rabbie-0.0.8/rabbie/decoder/decoders/auto_decoder.py
+-rw-rw-rw-   0        0        0      148 2023-04-24 20:01:12.000000 rabbie-0.0.8/rabbie/decoder/decoders/json_decoder.py
+drwxrwxrwx   0        0        0        0 2023-05-18 08:08:04.229934 rabbie-0.0.8/rabbie/decoder/exceptions/
+-rw-rw-rw-   0        0        0       94 2023-03-29 12:21:12.000000 rabbie-0.0.8/rabbie/decoder/exceptions/__init__.py
+-rw-rw-rw-   0        0        0       44 2023-03-29 12:19:53.000000 rabbie-0.0.8/rabbie/decoder/exceptions/decode_exception.py
+drwxrwxrwx   0        0        0        0 2023-05-18 08:08:04.231935 rabbie-0.0.8/rabbie/encoder/
+-rw-rw-rw-   0        0        0       78 2023-05-11 11:17:49.000000 rabbie-0.0.8/rabbie/encoder/__init__.py
+-rw-rw-rw-   0        0        0      197 2023-05-11 11:17:49.000000 rabbie-0.0.8/rabbie/encoder/encoder.py
+drwxrwxrwx   0        0        0        0 2023-05-18 08:08:04.234936 rabbie-0.0.8/rabbie/encoder/encoders/
+-rw-rw-rw-   0        0        0       78 2023-05-11 11:17:49.000000 rabbie-0.0.8/rabbie/encoder/encoders/__init__.py
+-rw-rw-rw-   0        0        0      461 2023-05-11 11:17:49.000000 rabbie-0.0.8/rabbie/encoder/encoders/auto_encoder.py
+-rw-rw-rw-   0        0        0      215 2023-05-11 11:17:49.000000 rabbie-0.0.8/rabbie/encoder/encoders/json_encoder.py
+drwxrwxrwx   0        0        0        0 2023-05-18 08:08:04.237934 rabbie-0.0.8/rabbie/events/
+-rw-rw-rw-   0        0        0       53 2023-05-18 08:05:34.000000 rabbie-0.0.8/rabbie/events/__init__.py
+-rw-rw-rw-   0        0        0     1274 2023-05-18 08:05:34.000000 rabbie-0.0.8/rabbie/events/event.py
+drwxrwxrwx   0        0        0        0 2023-05-18 08:08:04.239933 rabbie-0.0.8/rabbie/logger/
+-rw-rw-rw-   0        0        0      631 2023-05-18 08:05:34.000000 rabbie-0.0.8/rabbie/logger/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-18 08:08:04.241933 rabbie-0.0.8/rabbie/producer/
+-rw-rw-rw-   0        0        0       46 2023-05-11 11:17:49.000000 rabbie-0.0.8/rabbie/producer/__init__.py
+-rw-rw-rw-   0        0        0     4584 2023-05-11 11:17:49.000000 rabbie-0.0.8/rabbie/producer/producer.py
+drwxrwxrwx   0        0        0        0 2023-05-18 08:08:04.244935 rabbie-0.0.8/rabbie/producer/publisher/
+-rw-rw-rw-   0        0        0       34 2023-05-11 11:17:49.000000 rabbie-0.0.8/rabbie/producer/publisher/__init__.py
+-rw-rw-rw-   0        0        0     3176 2023-05-11 11:17:49.000000 rabbie-0.0.8/rabbie/producer/publisher/publisher.py
+drwxrwxrwx   0        0        0        0 2023-05-18 08:08:04.247934 rabbie-0.0.8/rabbie/supervisor/
+-rw-rw-rw-   0        0        0       50 2023-04-24 20:01:12.000000 rabbie-0.0.8/rabbie/supervisor/__init__.py
+-rw-rw-rw-   0        0        0     4560 2023-04-24 20:01:12.000000 rabbie-0.0.8/rabbie/supervisor/supervisor.py
+drwxrwxrwx   0        0        0        0 2023-05-18 08:08:04.209933 rabbie-0.0.8/rabbie.egg-info/
+-rw-rw-rw-   0        0        0     9287 2023-05-18 08:08:04.000000 rabbie-0.0.8/rabbie.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1431 2023-05-18 08:08:04.000000 rabbie-0.0.8/rabbie.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-18 08:08:04.000000 rabbie-0.0.8/rabbie.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       32 2023-05-18 08:08:04.000000 rabbie-0.0.8/rabbie.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-05-18 08:08:04.000000 rabbie-0.0.8/rabbie.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-18 08:08:04.255935 rabbie-0.0.8/setup.cfg
+-rw-rw-rw-   0        0        0      854 2023-05-18 08:05:34.000000 rabbie-0.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-18 08:08:04.253935 rabbie-0.0.8/tests/
+-rw-rw-rw-   0        0        0     4962 2023-05-18 08:05:34.000000 rabbie-0.0.8/tests/test_consumer.py
+-rw-rw-rw-   0        0        0        0 2023-04-24 20:01:12.000000 rabbie-0.0.8/tests/test_decoder.py
+-rw-rw-rw-   0        0        0        0 2023-04-24 20:01:12.000000 rabbie-0.0.8/tests/test_listener.py
+-rw-rw-rw-   0        0        0        0 2023-04-24 20:01:12.000000 rabbie-0.0.8/tests/test_microconsumer.py
+-rw-rw-rw-   0        0        0        0 2023-05-11 11:17:49.000000 rabbie-0.0.8/tests/test_producer.py
```

### Comparing `rabbie-0.0.7/LICENSE` & `rabbie-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `rabbie-0.0.7/PKG-INFO` & `rabbie-0.0.8/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,21 +1,7 @@
-Metadata-Version: 2.1
-Name: rabbie
-Version: 0.0.7
-Summary: A simple, decorator interface for AMQP based message brokers
-Home-page: https://github.com/scuffi/rabbie
-Author: Archie Ferguson
-Author-email: iamarchieferguson@gmail.com
-License: MIT license
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 
 # <p align="center">🥕 Rabbie 🥕</p>
 
 
 <p align="center">
 <img alt="GitHub last commit" src="https://img.shields.io/github/last-commit/scuffi/rabbie"> <img alt="PyPI - Python Version" src="https://img.shields.io/pypi/pyversions/rabbie"> <img alt="GitHub" src="https://img.shields.io/github/license/scuffi/rabbie"> <a href="https://pypi.org/project/rabbie/"><img alt="PyPI" src="https://img.shields.io/pypi/v/rabbie"></a>
 </p>
@@ -78,14 +64,16 @@
 
 if __name__ == "__main__":
     consumer.start()
 ```
 
 > ℹ️ Each Rabbie worker will be in use the entire time your custom function is running, i.e. if you have 3 workers, they can all process 1 message at a time and will not pick up anymore until the entire process has been complete. *(You can add a prefetch to allow for internal message queues)*
 
+> ℹ️ If you're not using default connection details (Username & Password), you can provide a pika.Parameters object (such as URLParameters) into the `Consumer(connection_parameters=...)`
+
 ### 🎱 Parameters
 Rabbie automatically picks up the parameters your function wants depending on the types of them:
 ```python
 from rabbie import Consumer, Channel, Method, Properties
 
 consumer = Consumer(
     ...
@@ -176,14 +164,47 @@
     def encoder(self, body: bytes):
         return # Your custom logic here
 
     def content_type(self):
         return "application/my_type"
 ```
     
+### 🎫 Event Handling
+If you want to add custom logic depending on whether or not your listeners are connected, or any error handling, you can use event handlers.
+
+Event handlers allow you to create callbacks for specific events that happen, such as on start and on stop.
+
+```python
+from rabbie import Consumer, event_handler
+
+@event_handler.register("on_start")
+def on_start():
+    print("I know all my listeners have started now!")
+
+@event_handler.register("on_stop")
+def on_stop():
+    print("All my listeners are dead")
+
+consumer = Consumer(
+    ...
+)
+
+if __name__ == "__main__":
+    consumer.start()
+```
+The defined functions will then get called when the given event is triggered behind the scenes.
+
+> ℹ️ Events can have multiple callbacks associated with them, so you can have as many on_start handlers as you please!
+
+List of current events:
+| Event ID | Trigger |
+|---|---|
+| on_start | When the application starts and all registered listeners have successfully connected. |
+| on_stop | When all active listeners have closed their connections. |
+
 ### 🖨️ Producers
 Producers allow for a simple way to publish messages to exchanges. A simple example would be like so:
 ```python
 from rabbie import Producer, JSONEncoder
 
 producer = Producer(
     host="localhost",
```

### Comparing `rabbie-0.0.7/README.md` & `rabbie-0.0.8/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,7 +1,21 @@
+Metadata-Version: 2.1
+Name: rabbie
+Version: 0.0.8
+Summary: A simple, decorator interface for AMQP based message brokers
+Home-page: https://github.com/scuffi/rabbie
+Author: Archie Ferguson
+Author-email: iamarchieferguson@gmail.com
+License: MIT license
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 
 # <p align="center">🥕 Rabbie 🥕</p>
 
 
 <p align="center">
 <img alt="GitHub last commit" src="https://img.shields.io/github/last-commit/scuffi/rabbie"> <img alt="PyPI - Python Version" src="https://img.shields.io/pypi/pyversions/rabbie"> <img alt="GitHub" src="https://img.shields.io/github/license/scuffi/rabbie"> <a href="https://pypi.org/project/rabbie/"><img alt="PyPI" src="https://img.shields.io/pypi/v/rabbie"></a>
 </p>
@@ -64,14 +78,16 @@
 
 if __name__ == "__main__":
     consumer.start()
 ```
 
 > ℹ️ Each Rabbie worker will be in use the entire time your custom function is running, i.e. if you have 3 workers, they can all process 1 message at a time and will not pick up anymore until the entire process has been complete. *(You can add a prefetch to allow for internal message queues)*
 
+> ℹ️ If you're not using default connection details (Username & Password), you can provide a pika.Parameters object (such as URLParameters) into the `Consumer(connection_parameters=...)`
+
 ### 🎱 Parameters
 Rabbie automatically picks up the parameters your function wants depending on the types of them:
 ```python
 from rabbie import Consumer, Channel, Method, Properties
 
 consumer = Consumer(
     ...
@@ -162,14 +178,47 @@
     def encoder(self, body: bytes):
         return # Your custom logic here
 
     def content_type(self):
         return "application/my_type"
 ```
     
+### 🎫 Event Handling
+If you want to add custom logic depending on whether or not your listeners are connected, or any error handling, you can use event handlers.
+
+Event handlers allow you to create callbacks for specific events that happen, such as on start and on stop.
+
+```python
+from rabbie import Consumer, event_handler
+
+@event_handler.register("on_start")
+def on_start():
+    print("I know all my listeners have started now!")
+
+@event_handler.register("on_stop")
+def on_stop():
+    print("All my listeners are dead")
+
+consumer = Consumer(
+    ...
+)
+
+if __name__ == "__main__":
+    consumer.start()
+```
+The defined functions will then get called when the given event is triggered behind the scenes.
+
+> ℹ️ Events can have multiple callbacks associated with them, so you can have as many on_start handlers as you please!
+
+List of current events:
+| Event ID | Trigger |
+|---|---|
+| on_start | When the application starts and all registered listeners have successfully connected. |
+| on_stop | When all active listeners have closed their connections. |
+
 ### 🖨️ Producers
 Producers allow for a simple way to publish messages to exchanges. A simple example would be like so:
 ```python
 from rabbie import Producer, JSONEncoder
 
 producer = Producer(
     host="localhost",
@@ -204,8 +253,8 @@
 # TODO
 - Hot Reloading (Refresh listeners on file changes) 🔄
 
 
 ## ➤ License
 Distributed under the MIT License. See [LICENSE](LICENSE) for more information.
         
-        
+
```

### Comparing `rabbie-0.0.7/rabbie/broker_types/channel.py` & `rabbie-0.0.8/rabbie/broker_types/channel.py`

 * *Files identical despite different names*

### Comparing `rabbie-0.0.7/rabbie/producer/producer.py` & `rabbie-0.0.8/rabbie/producer/producer.py`

 * *Files identical despite different names*

### Comparing `rabbie-0.0.7/rabbie/producer/publisher/publisher.py` & `rabbie-0.0.8/rabbie/producer/publisher/publisher.py`

 * *Files identical despite different names*

### Comparing `rabbie-0.0.7/rabbie/supervisor/supervisor.py` & `rabbie-0.0.8/rabbie/supervisor/supervisor.py`

 * *Files identical despite different names*

### Comparing `rabbie-0.0.7/rabbie.egg-info/PKG-INFO` & `rabbie-0.0.8/rabbie.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rabbie
-Version: 0.0.7
+Version: 0.0.8
 Summary: A simple, decorator interface for AMQP based message brokers
 Home-page: https://github.com/scuffi/rabbie
 Author: Archie Ferguson
 Author-email: iamarchieferguson@gmail.com
 License: MIT license
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -78,14 +78,16 @@
 
 if __name__ == "__main__":
     consumer.start()
 ```
 
 > ℹ️ Each Rabbie worker will be in use the entire time your custom function is running, i.e. if you have 3 workers, they can all process 1 message at a time and will not pick up anymore until the entire process has been complete. *(You can add a prefetch to allow for internal message queues)*
 
+> ℹ️ If you're not using default connection details (Username & Password), you can provide a pika.Parameters object (such as URLParameters) into the `Consumer(connection_parameters=...)`
+
 ### 🎱 Parameters
 Rabbie automatically picks up the parameters your function wants depending on the types of them:
 ```python
 from rabbie import Consumer, Channel, Method, Properties
 
 consumer = Consumer(
     ...
@@ -176,14 +178,47 @@
     def encoder(self, body: bytes):
         return # Your custom logic here
 
     def content_type(self):
         return "application/my_type"
 ```
     
+### 🎫 Event Handling
+If you want to add custom logic depending on whether or not your listeners are connected, or any error handling, you can use event handlers.
+
+Event handlers allow you to create callbacks for specific events that happen, such as on start and on stop.
+
+```python
+from rabbie import Consumer, event_handler
+
+@event_handler.register("on_start")
+def on_start():
+    print("I know all my listeners have started now!")
+
+@event_handler.register("on_stop")
+def on_stop():
+    print("All my listeners are dead")
+
+consumer = Consumer(
+    ...
+)
+
+if __name__ == "__main__":
+    consumer.start()
+```
+The defined functions will then get called when the given event is triggered behind the scenes.
+
+> ℹ️ Events can have multiple callbacks associated with them, so you can have as many on_start handlers as you please!
+
+List of current events:
+| Event ID | Trigger |
+|---|---|
+| on_start | When the application starts and all registered listeners have successfully connected. |
+| on_stop | When all active listeners have closed their connections. |
+
 ### 🖨️ Producers
 Producers allow for a simple way to publish messages to exchanges. A simple example would be like so:
 ```python
 from rabbie import Producer, JSONEncoder
 
 producer = Producer(
     host="localhost",
```

### Comparing `rabbie-0.0.7/rabbie.egg-info/SOURCES.txt` & `rabbie-0.0.8/rabbie.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -15,26 +15,29 @@
 rabbie/connection/details.py
 rabbie/consumer/__init__.py
 rabbie/consumer/consumer.py
 rabbie/consumer/microconsumer.py
 rabbie/consumer/listener/__init__.py
 rabbie/consumer/listener/listener.py
 rabbie/consumer/listener/listener_details.py
+rabbie/consumer/listener/listener_status.py
 rabbie/decoder/__init__.py
 rabbie/decoder/decoder.py
 rabbie/decoder/decoders/__init__.py
 rabbie/decoder/decoders/auto_decoder.py
 rabbie/decoder/decoders/json_decoder.py
 rabbie/decoder/exceptions/__init__.py
 rabbie/decoder/exceptions/decode_exception.py
 rabbie/encoder/__init__.py
 rabbie/encoder/encoder.py
 rabbie/encoder/encoders/__init__.py
 rabbie/encoder/encoders/auto_encoder.py
 rabbie/encoder/encoders/json_encoder.py
+rabbie/events/__init__.py
+rabbie/events/event.py
 rabbie/logger/__init__.py
 rabbie/producer/__init__.py
 rabbie/producer/producer.py
 rabbie/producer/publisher/__init__.py
 rabbie/producer/publisher/publisher.py
 rabbie/supervisor/__init__.py
 rabbie/supervisor/supervisor.py
```

### Comparing `rabbie-0.0.7/setup.py` & `rabbie-0.0.8/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
-version = "0.0.7"
+version = "0.0.8"
 requirements = ["pika", "multiprocess", "rich", "watchdog"]
 
 setup(
     name="rabbie",
     version=version,
     author="Archie Ferguson",
     author_email="iamarchieferguson@gmail.com",
```

### Comparing `rabbie-0.0.7/tests/test_consumer.py` & `rabbie-0.0.8/tests/test_consumer.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,127 +1,127 @@
-from rabbie import Consumer, MicroConsumer
-from rabbie.consumer import Listener, ListenerDetails
+# from rabbie import Consumer, MicroConsumer
+# from rabbie.consumer import Listener, ListenerDetails
 
 
-# Dependencies:
-# pip install pytest-mock
-import pytest
-
-
-class TestConsumer:
-    # Tests that a Consumer object can be created with valid parameters.
-    def test_create_consumer_with_valid_parameters(self):
-        # Happy path
-        consumer = Consumer(
-            host="localhost", port="5672", username="guest", password="guest"
-        )
-        assert consumer._host == "localhost"
-        assert consumer._port == "5672"
-        assert consumer._username == "guest"
-        assert consumer._password == "guest"
-
-    # Tests that the listen method can be called with valid parameters and a decorated function.
-    def test_listen_method_with_valid_parameters(self):
-        # Happy path
-        consumer = Consumer(
-            host="localhost", port="5672", username="guest", password="guest"
-        )
-
-        @consumer.listen(queue="test_queue", workers=2)
-        def test_function():
-            pass
-
-        assert len(consumer.listeners) == 1
-        assert consumer.listeners[0].details.queue_name == "test_queue"
-        assert consumer.listeners[0].details.workers == 2
-
-    # Tests that the start method can be called with valid parameters.
-    def test_start_method_with_valid_parameters(self, mocker):
-        # Happy path
-        consumer = Consumer(
-            host="localhost", port="5672", username="guest", password="guest"
-        )
-        listener_mock = mocker.Mock()
-        listener_mock.start.return_value = None
-        consumer.listeners.append(listener_mock)
-        consumer.start(reload=False, halt=False)
-        listener_mock.start.assert_called_once()
-
-    # Tests that a valid Consumer or MicroConsumer object can be added to the listeners list.
-    def test_add_consumer_method_with_valid_parameters(self):
-        # Happy Path
-        consumer1 = Consumer(
-            host="localhost", port="5672", username="guest", password="guest"
-        )
-        consumer2 = Consumer(
-            host="localhost", port="5672", username="guest", password="guest"
-        )
-        microconsumer = MicroConsumer()
-
-        consumer1.add_consumer(consumer2)
-        assert len(consumer1.listeners) == len(consumer2.listeners)
-
-        consumer1.add_consumer(microconsumer)
-        assert len(consumer1.listeners) == len(consumer2.listeners) + len(
-            microconsumer._build_listeners(consumer1.connection_parameters)
-        )
-
-        # Edge Case
-        consumer1.add_consumer(None)
-        assert len(consumer1.listeners) == len(consumer2.listeners) + len(
-            microconsumer._build_listeners(consumer1.connection_parameters)
-        )
-
-    # Tests that the stop method stops all Listeners.
-    def test_stop_method(self):
-        # Important
-        consumer = Consumer(
-            host="localhost", port="5672", username="guest", password="guest"
-        )
-        listener1 = Listener(
-            connection_parameters=consumer.connection_parameters,
-            details=ListenerDetails(
-                callback=lambda x: x,
-                queue_name="test_queue",
-                workers=1,
-                decoder=None,
-                restart=False,
-                auto_ack=True,
-            ),
-        )
-        listener2 = Listener(
-            connection_parameters=consumer.connection_parameters,
-            details=ListenerDetails(
-                callback=lambda x: x,
-                queue_name="test_queue",
-                workers=1,
-                decoder=None,
-                restart=False,
-                auto_ack=True,
-            ),
-        )
-        consumer.listeners = [listener1, listener2]
-
-        for listener in consumer.listeners:
-            listener.start()
-
-        assert all([listener.is_listening() for listener in consumer.listeners])
-
-        consumer._stop_listeners()
-
-        assert not any([listener.is_listening() for listener in consumer.listeners])
-
-    # Tests that the _start_listeners method starts all Listeners.
-    def test_start_listeners_method(self, mocker):
-        # Create a mock Listener object
-        mock_listener = mocker.Mock()
-        mock_listener.start.return_value = None
-
-        # Add the mock Listener to the Consumer's listeners list
-        consumer = Consumer(
-            host="localhost", port="5672", username="guest", password="guest"
-        )
-        consumer.listeners.append(mock_listener)
-
-        # Call the _start_listeners method and assert that the mock Listener's start method was called
-        consumer._start_listeners()
-        mock_listener.start.assert_called_once()
+# # Dependencies:
+# # pip install pytest-mock
+# import pytest
+
+
+# class TestConsumer:
+#     # Tests that a Consumer object can be created with valid parameters.
+#     def test_create_consumer_with_valid_parameters(self):
+#         # Happy path
+#         consumer = Consumer(
+#             host="localhost", port="5672", username="guest", password="guest"
+#         )
+#         assert consumer._host == "localhost"
+#         assert consumer._port == "5672"
+#         assert consumer._username == "guest"
+#         assert consumer._password == "guest"
+
+#     # Tests that the listen method can be called with valid parameters and a decorated function.
+#     def test_listen_method_with_valid_parameters(self):
+#         # Happy path
+#         consumer = Consumer(
+#             host="localhost", port="5672", username="guest", password="guest"
+#         )
+
+#         @consumer.listen(queue="test_queue", workers=2)
+#         def test_function():
+#             pass
+
+#         assert len(consumer.listeners) == 1
+#         assert consumer.listeners[0].details.queue_name == "test_queue"
+#         assert consumer.listeners[0].details.workers == 2
+
+#     # Tests that the start method can be called with valid parameters.
+#     def test_start_method_with_valid_parameters(self, mocker):
+#         # Happy path
+#         consumer = Consumer(
+#             host="localhost", port="5672", username="guest", password="guest"
+#         )
+#         listener_mock = mocker.Mock()
+#         listener_mock.start.return_value = None
+#         consumer.listeners.append(listener_mock)
+#         consumer.start(reload=False, halt=False)
+#         listener_mock.start.assert_called_once()
+
+#     # Tests that a valid Consumer or MicroConsumer object can be added to the listeners list.
+#     def test_add_consumer_method_with_valid_parameters(self):
+#         # Happy Path
+#         consumer1 = Consumer(
+#             host="localhost", port="5672", username="guest", password="guest"
+#         )
+#         consumer2 = Consumer(
+#             host="localhost", port="5672", username="guest", password="guest"
+#         )
+#         microconsumer = MicroConsumer()
+
+#         consumer1.add_consumer(consumer2)
+#         assert len(consumer1.listeners) == len(consumer2.listeners)
+
+#         consumer1.add_consumer(microconsumer)
+#         assert len(consumer1.listeners) == len(consumer2.listeners) + len(
+#             microconsumer._build_listeners(consumer1.connection_parameters)
+#         )
+
+#         # Edge Case
+#         consumer1.add_consumer(None)
+#         assert len(consumer1.listeners) == len(consumer2.listeners) + len(
+#             microconsumer._build_listeners(consumer1.connection_parameters)
+#         )
+
+#     # Tests that the stop method stops all Listeners.
+#     def test_stop_method(self):
+#         # Important
+#         consumer = Consumer(
+#             host="localhost", port="5672", username="guest", password="guest"
+#         )
+#         listener1 = Listener(
+#             connection_parameters=consumer.connection_parameters,
+#             details=ListenerDetails(
+#                 callback=lambda x: x,
+#                 queue_name="test_queue",
+#                 workers=1,
+#                 decoder=None,
+#                 restart=False,
+#                 auto_ack=True,
+#             ),
+#         )
+#         listener2 = Listener(
+#             connection_parameters=consumer.connection_parameters,
+#             details=ListenerDetails(
+#                 callback=lambda x: x,
+#                 queue_name="test_queue",
+#                 workers=1,
+#                 decoder=None,
+#                 restart=False,
+#                 auto_ack=True,
+#             ),
+#         )
+#         consumer.listeners = [listener1, listener2]
+
+#         for listener in consumer.listeners:
+#             listener.start()
+
+#         assert all([listener.is_listening() for listener in consumer.listeners])
+
+#         consumer._stop_listeners()
+
+#         assert not any([listener.is_listening() for listener in consumer.listeners])
+
+#     # Tests that the _start_listeners method starts all Listeners.
+#     def test_start_listeners_method(self, mocker):
+#         # Create a mock Listener object
+#         mock_listener = mocker.Mock()
+#         mock_listener.start.return_value = None
+
+#         # Add the mock Listener to the Consumer's listeners list
+#         consumer = Consumer(
+#             host="localhost", port="5672", username="guest", password="guest"
+#         )
+#         consumer.listeners.append(mock_listener)
+
+#         # Call the _start_listeners method and assert that the mock Listener's start method was called
+#         consumer._start_listeners()
+#         mock_listener.start.assert_called_once()
```

