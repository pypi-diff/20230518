# Comparing `tmp/py_volley-1.0.0.tar.gz` & `tmp/py_volley-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py_volley-1.0.0.tar", max compression
+gzip compressed data, was "py_volley-1.1.0.tar", max compression
```

## Comparing `py_volley-1.0.0.tar` & `py_volley-1.1.0.tar`

### file list

```diff
@@ -1,30 +1,29 @@
--rw-r--r--   0        0        0     1068 2023-05-04 20:51:04.032201 py_volley-1.0.0/LICENSE.md
--rw-r--r--   0        0        0     8734 2023-05-04 20:51:04.032201 py_volley-1.0.0/README.md
--rw-r--r--   0        0        0     2751 2023-05-04 20:51:04.036201 py_volley-1.0.0/pyproject.toml
--rw-r--r--   0        0        0      132 2023-05-04 20:51:04.036201 py_volley-1.0.0/volley/__init__.py
--rw-r--r--   0        0        0     1922 2023-05-04 20:51:04.036201 py_volley-1.0.0/volley/concurrency.py
--rw-r--r--   0        0        0     4897 2023-05-04 20:51:04.036201 py_volley-1.0.0/volley/config.py
--rw-r--r--   0        0        0        0 2023-05-04 20:51:04.036201 py_volley-1.0.0/volley/connectors/__init__.py
--rw-r--r--   0        0        0     2361 2023-05-04 20:51:04.036201 py_volley-1.0.0/volley/connectors/base.py
--rw-r--r--   0        0        0    16383 2023-05-04 20:51:04.036201 py_volley-1.0.0/volley/connectors/confluent.py
--rw-r--r--   0        0        0     7372 2023-05-04 20:51:04.036201 py_volley-1.0.0/volley/connectors/rsmq.py
--rw-r--r--   0        0        0     3018 2023-05-04 20:51:04.036201 py_volley-1.0.0/volley/connectors/zmq.py
--rw-r--r--   0        0        0      393 2023-05-04 20:51:04.036201 py_volley-1.0.0/volley/data_models.py
--rw-r--r--   0        0        0    12250 2023-05-04 20:51:04.036201 py_volley-1.0.0/volley/engine.py
--rw-r--r--   0        0        0     3150 2023-05-04 20:51:04.036201 py_volley-1.0.0/volley/global.yml
--rw-r--r--   0        0        0       53 2023-05-04 20:51:04.036201 py_volley-1.0.0/volley/logging.py
--rw-r--r--   0        0        0     1686 2023-05-04 20:51:04.036201 py_volley-1.0.0/volley/metrics.py
--rw-r--r--   0        0        0      253 2023-05-04 20:51:04.036201 py_volley-1.0.0/volley/models/__init__.py
--rw-r--r--   0        0        0     4858 2023-05-04 20:51:04.036201 py_volley-1.0.0/volley/models/base.py
--rw-r--r--   0        0        0     2113 2023-05-04 20:51:04.036201 py_volley-1.0.0/volley/models/pydantic_model.py
--rw-r--r--   0        0        0     4271 2023-05-04 20:51:04.036201 py_volley-1.0.0/volley/profiles.py
--rw-r--r--   0        0        0     4078 2023-05-04 20:51:04.036201 py_volley-1.0.0/volley/queues.py
--rw-r--r--   0        0        0      285 2023-05-04 20:51:04.036201 py_volley-1.0.0/volley/serializers/__init__.py
--rw-r--r--   0        0        0      537 2023-05-04 20:51:04.036201 py_volley-1.0.0/volley/serializers/base.py
--rw-r--r--   0        0        0      453 2023-05-04 20:51:04.036201 py_volley-1.0.0/volley/serializers/json_serializer.py
--rw-r--r--   0        0        0      439 2023-05-04 20:51:04.036201 py_volley-1.0.0/volley/serializers/msgpack_serializer.py
--rw-r--r--   0        0        0      475 2023-05-04 20:51:04.036201 py_volley-1.0.0/volley/serializers/orjson_serializer.py
--rw-r--r--   0        0        0     4663 2023-05-04 20:51:04.036201 py_volley-1.0.0/volley/transport.py
--rw-r--r--   0        0        0     1742 2023-05-04 20:51:04.036201 py_volley-1.0.0/volley/util.py
--rw-r--r--   0        0        0    10190 1970-01-01 00:00:00.000000 py_volley-1.0.0/setup.py
--rw-r--r--   0        0        0    10102 1970-01-01 00:00:00.000000 py_volley-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-05-18 15:46:30.487841 py_volley-1.1.0/LICENSE.md
+-rw-r--r--   0        0        0     8734 2023-05-18 15:46:30.487841 py_volley-1.1.0/README.md
+-rw-r--r--   0        0        0     2751 2023-05-18 15:46:30.491842 py_volley-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0      132 2023-05-18 15:46:30.503843 py_volley-1.1.0/volley/__init__.py
+-rw-r--r--   0        0        0     1922 2023-05-18 15:46:30.503843 py_volley-1.1.0/volley/concurrency.py
+-rw-r--r--   0        0        0     4897 2023-05-18 15:46:30.503843 py_volley-1.1.0/volley/config.py
+-rw-r--r--   0        0        0        0 2023-05-18 15:46:30.503843 py_volley-1.1.0/volley/connectors/__init__.py
+-rw-r--r--   0        0        0     2361 2023-05-18 15:46:30.503843 py_volley-1.1.0/volley/connectors/base.py
+-rw-r--r--   0        0        0    16383 2023-05-18 15:46:30.503843 py_volley-1.1.0/volley/connectors/confluent.py
+-rw-r--r--   0        0        0     7372 2023-05-18 15:46:30.503843 py_volley-1.1.0/volley/connectors/rsmq.py
+-rw-r--r--   0        0        0     3018 2023-05-18 15:46:30.503843 py_volley-1.1.0/volley/connectors/zmq.py
+-rw-r--r--   0        0        0      393 2023-05-18 15:46:30.503843 py_volley-1.1.0/volley/data_models.py
+-rw-r--r--   0        0        0    12250 2023-05-18 15:46:30.503843 py_volley-1.1.0/volley/engine.py
+-rw-r--r--   0        0        0     3150 2023-05-18 15:46:30.503843 py_volley-1.1.0/volley/global.yml
+-rw-r--r--   0        0        0       53 2023-05-18 15:46:30.503843 py_volley-1.1.0/volley/logging.py
+-rw-r--r--   0        0        0     1686 2023-05-18 15:46:30.503843 py_volley-1.1.0/volley/metrics.py
+-rw-r--r--   0        0        0      253 2023-05-18 15:46:30.503843 py_volley-1.1.0/volley/models/__init__.py
+-rw-r--r--   0        0        0     4858 2023-05-18 15:46:30.503843 py_volley-1.1.0/volley/models/base.py
+-rw-r--r--   0        0        0     2113 2023-05-18 15:46:30.503843 py_volley-1.1.0/volley/models/pydantic_model.py
+-rw-r--r--   0        0        0     4271 2023-05-18 15:46:30.503843 py_volley-1.1.0/volley/profiles.py
+-rw-r--r--   0        0        0     4078 2023-05-18 15:46:30.503843 py_volley-1.1.0/volley/queues.py
+-rw-r--r--   0        0        0      285 2023-05-18 15:46:30.503843 py_volley-1.1.0/volley/serializers/__init__.py
+-rw-r--r--   0        0        0      537 2023-05-18 15:46:30.503843 py_volley-1.1.0/volley/serializers/base.py
+-rw-r--r--   0        0        0      453 2023-05-18 15:46:30.503843 py_volley-1.1.0/volley/serializers/json_serializer.py
+-rw-r--r--   0        0        0      439 2023-05-18 15:46:30.503843 py_volley-1.1.0/volley/serializers/msgpack_serializer.py
+-rw-r--r--   0        0        0      475 2023-05-18 15:46:30.503843 py_volley-1.1.0/volley/serializers/orjson_serializer.py
+-rw-r--r--   0        0        0     4663 2023-05-18 15:46:30.503843 py_volley-1.1.0/volley/transport.py
+-rw-r--r--   0        0        0     1742 2023-05-18 15:46:30.503843 py_volley-1.1.0/volley/util.py
+-rw-r--r--   0        0        0    10107 1970-01-01 00:00:00.000000 py_volley-1.1.0/PKG-INFO
```

### Comparing `py_volley-1.0.0/LICENSE.md` & `py_volley-1.1.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `py_volley-1.0.0/README.md` & `py_volley-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `py_volley-1.0.0/pyproject.toml` & `py_volley-1.1.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "py_volley"
-version = "1.0.0"
+version = "1.1.0"
 description = "Pluggable message queueing for Python"
 authors = ["ask-machine-learning <shipt@shipt.com>"]
 readme = "README.md"
 
 packages = [
     { include = "volley" },
 ]
@@ -20,15 +20,15 @@
 pydantic = ">=1.8.2, <2"
 PyYAML = ">=5.4.1, <6.1"
 orjson = ">=3.6.4, <4.0"
 msgpack = "^1.0.3, <2"
 starlette = "<1"
 uvicorn = "<1"
 
-confluent-kafka = {version ="^1.8.2", optional = true}
+confluent-kafka = {version ="^2.0.0", optional = true}
 PyRSMQ = {version ="^0.4.5", optional = true}
 hiredis = {version ="^2.0", optional = true}
 tenacity = {version ="^8.0.1", optional = true}
 pyzmq = {version =">=22.3.0", optional = true}
 
 [tool.poetry.extras]
 all = ["confluent-kafka", "PyRSMQ", "hiredis", "tenacity", "pyzmq"]
```

### Comparing `py_volley-1.0.0/volley/concurrency.py` & `py_volley-1.1.0/volley/concurrency.py`

 * *Files identical despite different names*

### Comparing `py_volley-1.0.0/volley/config.py` & `py_volley-1.1.0/volley/config.py`

 * *Files identical despite different names*

### Comparing `py_volley-1.0.0/volley/connectors/base.py` & `py_volley-1.1.0/volley/connectors/base.py`

 * *Files identical despite different names*

### Comparing `py_volley-1.0.0/volley/connectors/confluent.py` & `py_volley-1.1.0/volley/connectors/confluent.py`

 * *Files identical despite different names*

### Comparing `py_volley-1.0.0/volley/connectors/rsmq.py` & `py_volley-1.1.0/volley/connectors/rsmq.py`

 * *Files identical despite different names*

### Comparing `py_volley-1.0.0/volley/connectors/zmq.py` & `py_volley-1.1.0/volley/connectors/zmq.py`

 * *Files identical despite different names*

### Comparing `py_volley-1.0.0/volley/engine.py` & `py_volley-1.1.0/volley/engine.py`

 * *Files identical despite different names*

### Comparing `py_volley-1.0.0/volley/global.yml` & `py_volley-1.1.0/volley/global.yml`

 * *Files identical despite different names*

### Comparing `py_volley-1.0.0/volley/metrics.py` & `py_volley-1.1.0/volley/metrics.py`

 * *Files identical despite different names*

### Comparing `py_volley-1.0.0/volley/models/base.py` & `py_volley-1.1.0/volley/models/base.py`

 * *Files identical despite different names*

### Comparing `py_volley-1.0.0/volley/models/pydantic_model.py` & `py_volley-1.1.0/volley/models/pydantic_model.py`

 * *Files identical despite different names*

### Comparing `py_volley-1.0.0/volley/profiles.py` & `py_volley-1.1.0/volley/profiles.py`

 * *Files identical despite different names*

### Comparing `py_volley-1.0.0/volley/queues.py` & `py_volley-1.1.0/volley/queues.py`

 * *Files identical despite different names*

### Comparing `py_volley-1.0.0/volley/serializers/base.py` & `py_volley-1.1.0/volley/serializers/base.py`

 * *Files identical despite different names*

### Comparing `py_volley-1.0.0/volley/transport.py` & `py_volley-1.1.0/volley/transport.py`

 * *Files identical despite different names*

### Comparing `py_volley-1.0.0/volley/util.py` & `py_volley-1.1.0/volley/util.py`

 * *Files identical despite different names*

### Comparing `py_volley-1.0.0/setup.py` & `py_volley-1.1.0/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,49 +1,264 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: py-volley
+Version: 1.1.0
+Summary: Pluggable message queueing for Python
+Author: ask-machine-learning
+Author-email: shipt@shipt.com
+Requires-Python: >=3.8,<4
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Provides-Extra: all
+Provides-Extra: kafka
+Provides-Extra: rsmq
+Provides-Extra: zmq
+Requires-Dist: PyRSMQ (>=0.4.5,<0.5.0) ; extra == "all" or extra == "rsmq"
+Requires-Dist: PyYAML (>=5.4.1,<6.1)
+Requires-Dist: confluent-kafka (>=2.0.0,<3.0.0) ; extra == "all" or extra == "kafka"
+Requires-Dist: hiredis (>=2.0,<3.0) ; extra == "all" or extra == "rsmq"
+Requires-Dist: msgpack (>=1.0.3,<2.0.0)
+Requires-Dist: orjson (>=3.6.4,<4.0)
+Requires-Dist: prometheus-client (>=0.11.0,<1)
+Requires-Dist: pydantic (>=1.8.2,<2)
+Requires-Dist: pyzmq (>=22.3.0) ; extra == "all" or extra == "zmq"
+Requires-Dist: starlette (<1)
+Requires-Dist: tenacity (>=8.0.1,<9.0.0) ; extra == "all" or extra == "rsmq"
+Requires-Dist: uvicorn (<1)
+Project-URL: Documentation, https://shipt.github.io/py-volley/
+Project-URL: Homepage, https://github.com/shipt/py-volley
+Project-URL: Repository, https://github.com/shipt/py-volley
+Description-Content-Type: text/markdown
 
-packages = \
-['volley', 'volley.connectors', 'volley.models', 'volley.serializers']
+![VolleyFull-Horizontal](https://user-images.githubusercontent.com/81711984/149005139-f0441dcf-c76e-4112-baf1-998d0a6abdbb.png)
 
-package_data = \
-{'': ['*']}
+Documentation: https://shipt.github.io/py-volley/
 
-install_requires = \
-['PyYAML>=5.4.1,<6.1',
- 'msgpack>=1.0.3,<2.0.0',
- 'orjson>=3.6.4,<4.0',
- 'prometheus-client>=0.11.0,<1',
- 'pydantic>=1.8.2,<2',
- 'starlette<1',
- 'uvicorn<1']
-
-extras_require = \
-{'all': ['confluent-kafka>=1.8.2,<2.0.0',
-         'PyRSMQ>=0.4.5,<0.5.0',
-         'hiredis>=2.0,<3.0',
-         'tenacity>=8.0.1,<9.0.0',
-         'pyzmq>=22.3.0'],
- 'kafka': ['confluent-kafka>=1.8.2,<2.0.0'],
- 'rsmq': ['PyRSMQ>=0.4.5,<0.5.0',
-          'hiredis>=2.0,<3.0',
-          'tenacity>=8.0.1,<9.0.0'],
- 'zmq': ['pyzmq>=22.3.0']}
-
-setup_kwargs = {
-    'name': 'py-volley',
-    'version': '1.0.0',
-    'description': 'Pluggable message queueing for Python',
-    'long_description': '![VolleyFull-Horizontal](https://user-images.githubusercontent.com/81711984/149005139-f0441dcf-c76e-4112-baf1-998d0a6abdbb.png)\n\nDocumentation: https://shipt.github.io/py-volley/\n\nVolley makes building event stream applications easier and more accessible. Use Volley if you need to quickly develop an application to consume messages, processes them (and do other things), then publish results to one or many places. Volley was inspired ease of use and developer experience provided by the [Flask](https://github.com/pallets/flask) and [FastAPI](https://github.com/tiangolo/fastapi) projects, and aims to make working with queue based and event driven system as accessible as REST APIs.\n\nVolley handles a number of operations that need to happen before and after processing a message. Reading the data, serialization, data validation, all need to happen before data reaches your application. If these fail, Volley can route the message to a dead-letter-queue. After processing, Volley again handles data validation, serialization, and the writing/publishing of data to any number of output queues. Finally, upon successfully delivery of that message to the target queue, Volley handles marking it as read or deleting it from the input queue.\n\nAll of Volley\'s major operations (connectors, serializers, data validation/model handling) can be extended with plugins, and comes with built in support for queues-like technologies [Apache Kafka](https://kafka.apache.org/) and [RSMQ](https://github.com/mlasevich/PyRSMQ) (Redis Simple Message Queue). There is a plugin built for a Postgres queue in our [examples](./example/plugins/my_plugin.py).\n\n\n[![Build Status](https://drone.shipt.com/api/badges/shipt/py-volley/status.svg?ref=refs/heads/main)](https://drone.shipt.com/shipt/py-volley)\n[![Coverage](https://sonarqube.shipt.com/api/project_badges/measure?project=shipt_py-volley_AYImTs5MsYUjTdFQ7Awt&metric=coverage&token=squ_e98968a6b1bce0281e001fd0e70e538f6228b47f)](https://sonarqube.shipt.com/dashboard?id=shipt_py-volley_AYImTs5MsYUjTdFQ7Awt)\n\n# Installation\n\nRequires Python >= 3.8\n\n```bash\npip install py-volley[all]\n```\n\nYou can also limit the dependencies by:\n```bash\npip install py-volley[kafka]  # Kafka dependencies\npip install py-volley[rsmq]  # RSMQ dependencies\npip install py-volley[zmq]  # ZeroMQ dependencies\n```\n\n## Features\n- Built in support for [Apache Kafka](https://kafka.apache.org/), [RSMQ](https://github.com/smrchy/rsmq), [ZeroMQ](https://zeromq.org/)\n- [Prometheus](https://prometheus.io/) metrics for all operations such as function processing time, and consumption and production count.\n- Serialization in JSON and [MessagePack](https://msgpack.org/index.html)\n- Data validation via [Pydantic](https://pydantic-docs.helpmanual.io/)\n- Optionally configured integration with dead-letter-queues\n- Extendible connectors (consumer/producers), serializers, model handlers, and model handlers via plugins.\n\n## Getting started\n\nVolley handles the process of consuming/producing by providing developers with extendible interfaces and handlers:\n- connectors - consumer and producer interfaces which define how the application should read messages, write messages, and what actions to take when a message is successfully or fails processing.\n- serializers - handlers and interface which describe the behavior for reading an byte objects from connectors. For example, Json or MessagePack serializers.\n- model_handler - handler and interface which works very closely with serializers. Typically used to turn serialized data into a structured Python data model. Pydantic is Volley\'s most supported data_model and can handler serialization itself.\n- data_model - When your application receives data from a queue, what schema and object do you expect it in? The data_model is provided by the user. And the `model_handler` describes how to construct your `data_model`.\n\n\nTo demonstrate, let\'s create an application with two worker nodes. One consumes from Kafka, finds the maximum value in a list then publishes it to Redis. The other consumes the message from Redis - if the max value is > 10, it logs to console otherwise it constructs a new list and publishes to the same Kafka topic. \n\n```mermaid\nflowchart LR\nA[(Kafka)] --> |consume| B[Worker 1]\nB --> |publish| C[(Redis)]\nC --> |consume| D[Worker 2]\nD --> E{>10}\nE --> | no | A\nE --> | yes | F[Log to Console]\n```\n\nYou can skip the details and just run `make intro.start`, which runs this example through `./example/intro/docker-compose.yml`\n\n1. start Kafka and Redis instance\n\n```\ndocker run -d -p 6379:6379 redis:5.0.0\ndocker run -d -p 9092:9092 bashj79/kafka-kraft\n```\n\n2. Configure the queues and data models. Let\'s put this in `./my_config.py`.\n\n```python\n# ./my_config.py\nfrom typing import List, Tuple\nfrom pydantic import BaseModel\n\nfrom volley import Engine, QueueConfig\n\n# define the schemas for the first and second worker nodes.\nclass InputMessage(BaseModel):\n  my_values: List[float]\n\nclass OutputMessage(BaseModel):\n  the_max: float\n\n# define the configurations for the two queues, one in Kafka and the other in Redis.\nqueue_config = [\n  QueueConfig(\n    name="my-kafka-input",\n    value="my.kafka.topic.name",\n    profile="confluent",\n    data_model=InputMessage,\n    config={\n      "group.id": "my.consumer.group",\n      "bootstrap.servers": "localhost:9092",\n    }\n  ),\n  QueueConfig(\n    name="my-redis-output",\n    value="my.redis.output.queue.name",\n    profile="rsmq",\n    data_model=OutputMessage,\n    config={\n      "host": "localhost",\n      "port": 6379,\n    }\n  )\n]\n```\n\n3. Build the first worker node - consume from Kafka, find the max value, publish to Redis\n\n```python\n# ./app_0.py\nfrom typing import List, Tuple\nfrom volley import Engine\n\nfrom my_config import queue_config, InputMessage, OutputMessage\n# the first node - reads from kafka and writes to redis\napp_0 = Engine(\n  app_name="app_0",\n  input_queue="my-kafka-input",  # one input\n  output_queues=["my-redis-output"],  # zero to many outputs\n  queue_config=queue_config\n)\n\n@app_0.stream_app\ndef kafka_to_redis(msg: InputMessage) -> List[Tuple[str, OutputMessage]]:\n  print(f"Received {msg.json()}")\n  max_val = max(msg.my_values)\n  out = OutputMessage(the_max=max_val)\n  print(out)\n  return [("my-redis-output", out)]  # a list of one or many output targets and messages\n\nif __name__ == "__main__":\n  kafka_to_redis()\n\n```\n\n4. Run the first application in a terminal\n```bash\npython app_0.py\n```\n\n\n5. Build the second worker node - consume from Redis, determine if we log to console or recycle the message as a new list.\n```python\n# ./app_1.py\nfrom typing import List, Tuple, Union\nfrom volley import Engine\n\nfrom my_config import OutputMessage, queue_config, InputMessage\n\n# the second node\napp_1 = Engine(\n  app_name="app_1",\n  input_queue="my-redis-output",\n  output_queues=["my-kafka-input"],\n  queue_config=queue_config,\n  metrics_port=None\n)\n\n@app_1.stream_app\ndef redis_to_kafka(msg: OutputMessage) -> Union[bool, List[Tuple[str, InputMessage]]]:\n  print(f"The maximum: {msg.the_max}")\n  if msg.the_max > 10:\n    print("That\'s it, we are done!")\n    return True\n  else:\n    out = InputMessage(my_values=[msg.the_max, msg.the_max+1, msg.the_max+2])\n    return [("my-kafka-input", out)]  # a list of one or many output targets and messages\n\nif __name__ == "__main__":\n    redis_to_kafka()\n```\n\n6. Run the second worker node in another terminal\n```bash\npython app_1.py\n```\n\n7. Finally, let\'s manually publish a message to the input kafka topic:\n```python\nfrom confluent_kafka import Producer\nimport json\nproducer = Producer({"bootstrap.servers": "localhost:9092"})\nproducer.produce(topic="my.kafka.topic.name", value=json.dumps({"my_values":[1,2,3]}))\nproducer.flush(5)\n```\n\nYou should see the following in your two terminals\n\n__./app_0.py__\n```\nReceived {"my_values": [1.0, 2.0, 3.0]}\nthe_max=3.0\nReceived {"my_values": [3.0, 4.0, 5.0]}\nthe_max=5.0\nReceived {"my_values": [5.0, 6.0, 7.0]}\nthe_max=7.0\nReceived {"my_values": [7.0, 8.0, 9.0]}\nthe_max=9.0\nReceived {"my_values": [9.0, 10.0, 11.0]}\nthe_max=11.0\n```\n\n__./app_1.py__\n```\nThe maximum: 3.0\nThe maximum: 5.0\nThe maximum: 7.0\nThe maximum: 9.0\nThe maximum: 11.0\nThat\'s it, we are done!\n```\n\n# Complete example\n\nClone this repo and `make run.example` to see a complete example of:\n- consuming a message from a Kafka topic\n- producing to RSMQ\n- consuming from RSMQ and publishing to Kafka and Postgres using custom plugin for Postgres.\n\n# Contributing\n\nSee our [contributing guide](./CONTRIBUTING.md).\n\nThanks goes to great [projects](./ATTRIBUTIONS.md) and these incredible people.\n\n<a href="https://github.com/shipt/py-volley/graphs/contributors">\n  <img src="https://contrib.rocks/image?repo=shipt/py-volley" />\n</a>\n',
-    'author': 'ask-machine-learning',
-    'author_email': 'shipt@shipt.com',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'None',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'extras_require': extras_require,
-    'python_requires': '>=3.8,<4',
-}
+Volley makes building event stream applications easier and more accessible. Use Volley if you need to quickly develop an application to consume messages, processes them (and do other things), then publish results to one or many places. Volley was inspired ease of use and developer experience provided by the [Flask](https://github.com/pallets/flask) and [FastAPI](https://github.com/tiangolo/fastapi) projects, and aims to make working with queue based and event driven system as accessible as REST APIs.
 
+Volley handles a number of operations that need to happen before and after processing a message. Reading the data, serialization, data validation, all need to happen before data reaches your application. If these fail, Volley can route the message to a dead-letter-queue. After processing, Volley again handles data validation, serialization, and the writing/publishing of data to any number of output queues. Finally, upon successfully delivery of that message to the target queue, Volley handles marking it as read or deleting it from the input queue.
+
+All of Volley's major operations (connectors, serializers, data validation/model handling) can be extended with plugins, and comes with built in support for queues-like technologies [Apache Kafka](https://kafka.apache.org/) and [RSMQ](https://github.com/mlasevich/PyRSMQ) (Redis Simple Message Queue). There is a plugin built for a Postgres queue in our [examples](./example/plugins/my_plugin.py).
+
+
+[![Build Status](https://drone.shipt.com/api/badges/shipt/py-volley/status.svg?ref=refs/heads/main)](https://drone.shipt.com/shipt/py-volley)
+[![Coverage](https://sonarqube.shipt.com/api/project_badges/measure?project=shipt_py-volley_AYImTs5MsYUjTdFQ7Awt&metric=coverage&token=squ_e98968a6b1bce0281e001fd0e70e538f6228b47f)](https://sonarqube.shipt.com/dashboard?id=shipt_py-volley_AYImTs5MsYUjTdFQ7Awt)
+
+# Installation
+
+Requires Python >= 3.8
+
+```bash
+pip install py-volley[all]
+```
+
+You can also limit the dependencies by:
+```bash
+pip install py-volley[kafka]  # Kafka dependencies
+pip install py-volley[rsmq]  # RSMQ dependencies
+pip install py-volley[zmq]  # ZeroMQ dependencies
+```
+
+## Features
+- Built in support for [Apache Kafka](https://kafka.apache.org/), [RSMQ](https://github.com/smrchy/rsmq), [ZeroMQ](https://zeromq.org/)
+- [Prometheus](https://prometheus.io/) metrics for all operations such as function processing time, and consumption and production count.
+- Serialization in JSON and [MessagePack](https://msgpack.org/index.html)
+- Data validation via [Pydantic](https://pydantic-docs.helpmanual.io/)
+- Optionally configured integration with dead-letter-queues
+- Extendible connectors (consumer/producers), serializers, model handlers, and model handlers via plugins.
+
+## Getting started
+
+Volley handles the process of consuming/producing by providing developers with extendible interfaces and handlers:
+- connectors - consumer and producer interfaces which define how the application should read messages, write messages, and what actions to take when a message is successfully or fails processing.
+- serializers - handlers and interface which describe the behavior for reading an byte objects from connectors. For example, Json or MessagePack serializers.
+- model_handler - handler and interface which works very closely with serializers. Typically used to turn serialized data into a structured Python data model. Pydantic is Volley's most supported data_model and can handler serialization itself.
+- data_model - When your application receives data from a queue, what schema and object do you expect it in? The data_model is provided by the user. And the `model_handler` describes how to construct your `data_model`.
+
+
+To demonstrate, let's create an application with two worker nodes. One consumes from Kafka, finds the maximum value in a list then publishes it to Redis. The other consumes the message from Redis - if the max value is > 10, it logs to console otherwise it constructs a new list and publishes to the same Kafka topic. 
+
+```mermaid
+flowchart LR
+A[(Kafka)] --> |consume| B[Worker 1]
+B --> |publish| C[(Redis)]
+C --> |consume| D[Worker 2]
+D --> E{>10}
+E --> | no | A
+E --> | yes | F[Log to Console]
+```
+
+You can skip the details and just run `make intro.start`, which runs this example through `./example/intro/docker-compose.yml`
+
+1. start Kafka and Redis instance
+
+```
+docker run -d -p 6379:6379 redis:5.0.0
+docker run -d -p 9092:9092 bashj79/kafka-kraft
+```
+
+2. Configure the queues and data models. Let's put this in `./my_config.py`.
+
+```python
+# ./my_config.py
+from typing import List, Tuple
+from pydantic import BaseModel
+
+from volley import Engine, QueueConfig
+
+# define the schemas for the first and second worker nodes.
+class InputMessage(BaseModel):
+  my_values: List[float]
+
+class OutputMessage(BaseModel):
+  the_max: float
+
+# define the configurations for the two queues, one in Kafka and the other in Redis.
+queue_config = [
+  QueueConfig(
+    name="my-kafka-input",
+    value="my.kafka.topic.name",
+    profile="confluent",
+    data_model=InputMessage,
+    config={
+      "group.id": "my.consumer.group",
+      "bootstrap.servers": "localhost:9092",
+    }
+  ),
+  QueueConfig(
+    name="my-redis-output",
+    value="my.redis.output.queue.name",
+    profile="rsmq",
+    data_model=OutputMessage,
+    config={
+      "host": "localhost",
+      "port": 6379,
+    }
+  )
+]
+```
+
+3. Build the first worker node - consume from Kafka, find the max value, publish to Redis
+
+```python
+# ./app_0.py
+from typing import List, Tuple
+from volley import Engine
+
+from my_config import queue_config, InputMessage, OutputMessage
+# the first node - reads from kafka and writes to redis
+app_0 = Engine(
+  app_name="app_0",
+  input_queue="my-kafka-input",  # one input
+  output_queues=["my-redis-output"],  # zero to many outputs
+  queue_config=queue_config
+)
+
+@app_0.stream_app
+def kafka_to_redis(msg: InputMessage) -> List[Tuple[str, OutputMessage]]:
+  print(f"Received {msg.json()}")
+  max_val = max(msg.my_values)
+  out = OutputMessage(the_max=max_val)
+  print(out)
+  return [("my-redis-output", out)]  # a list of one or many output targets and messages
+
+if __name__ == "__main__":
+  kafka_to_redis()
+
+```
+
+4. Run the first application in a terminal
+```bash
+python app_0.py
+```
+
+
+5. Build the second worker node - consume from Redis, determine if we log to console or recycle the message as a new list.
+```python
+# ./app_1.py
+from typing import List, Tuple, Union
+from volley import Engine
+
+from my_config import OutputMessage, queue_config, InputMessage
+
+# the second node
+app_1 = Engine(
+  app_name="app_1",
+  input_queue="my-redis-output",
+  output_queues=["my-kafka-input"],
+  queue_config=queue_config,
+  metrics_port=None
+)
+
+@app_1.stream_app
+def redis_to_kafka(msg: OutputMessage) -> Union[bool, List[Tuple[str, InputMessage]]]:
+  print(f"The maximum: {msg.the_max}")
+  if msg.the_max > 10:
+    print("That's it, we are done!")
+    return True
+  else:
+    out = InputMessage(my_values=[msg.the_max, msg.the_max+1, msg.the_max+2])
+    return [("my-kafka-input", out)]  # a list of one or many output targets and messages
+
+if __name__ == "__main__":
+    redis_to_kafka()
+```
+
+6. Run the second worker node in another terminal
+```bash
+python app_1.py
+```
+
+7. Finally, let's manually publish a message to the input kafka topic:
+```python
+from confluent_kafka import Producer
+import json
+producer = Producer({"bootstrap.servers": "localhost:9092"})
+producer.produce(topic="my.kafka.topic.name", value=json.dumps({"my_values":[1,2,3]}))
+producer.flush(5)
+```
+
+You should see the following in your two terminals
+
+__./app_0.py__
+```
+Received {"my_values": [1.0, 2.0, 3.0]}
+the_max=3.0
+Received {"my_values": [3.0, 4.0, 5.0]}
+the_max=5.0
+Received {"my_values": [5.0, 6.0, 7.0]}
+the_max=7.0
+Received {"my_values": [7.0, 8.0, 9.0]}
+the_max=9.0
+Received {"my_values": [9.0, 10.0, 11.0]}
+the_max=11.0
+```
+
+__./app_1.py__
+```
+The maximum: 3.0
+The maximum: 5.0
+The maximum: 7.0
+The maximum: 9.0
+The maximum: 11.0
+That's it, we are done!
+```
+
+# Complete example
+
+Clone this repo and `make run.example` to see a complete example of:
+- consuming a message from a Kafka topic
+- producing to RSMQ
+- consuming from RSMQ and publishing to Kafka and Postgres using custom plugin for Postgres.
+
+# Contributing
+
+See our [contributing guide](./CONTRIBUTING.md).
+
+Thanks goes to great [projects](./ATTRIBUTIONS.md) and these incredible people.
+
+<a href="https://github.com/shipt/py-volley/graphs/contributors">
+  <img src="https://contrib.rocks/image?repo=shipt/py-volley" />
+</a>
 
-setup(**setup_kwargs)
```

