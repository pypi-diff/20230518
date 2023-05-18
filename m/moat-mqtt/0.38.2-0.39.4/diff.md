# Comparing `tmp/moat-mqtt-0.38.2.tar.gz` & `tmp/moat-mqtt-0.39.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "moat-mqtt-0.38.2.tar", last modified: Fri Sep 23 13:51:40 2022, max compression
+gzip compressed data, was "moat-mqtt-0.39.4.tar", last modified: Thu May 18 12:52:13 2023, max compression
```

## Comparing `moat-mqtt-0.38.2.tar` & `moat-mqtt-0.39.4.tar`

### file list

```diff
@@ -1,133 +1,133 @@
-drwxr-xr-x   0 smurf      (501) smurf      (501)        0 2022-09-23 13:51:40.111356 moat-mqtt-0.38.2/
--rw-r--r--   0 smurf      (501) smurf      (501)      436 2022-09-19 16:10:40.000000 moat-mqtt-0.38.2/.gitignore
--rw-r--r--   0 smurf      (501) smurf      (501)      200 2022-09-06 09:13:47.000000 moat-mqtt-0.38.2/.pylintrc
--rw-r--r--   0 smurf      (501) smurf      (501)      307 2022-09-06 09:13:47.000000 moat-mqtt-0.38.2/.travis.yml
--rw-r--r--   0 smurf      (501) smurf      (501)      420 2022-09-06 09:13:47.000000 moat-mqtt-0.38.2/MANIFEST.in
--rw-r--r--   0 smurf      (501) smurf      (501)      239 2022-09-16 17:32:23.000000 moat-mqtt-0.38.2/Makefile
--rw-r--r--   0 smurf      (501) smurf      (501)      687 2022-09-23 13:51:40.111356 moat-mqtt-0.38.2/PKG-INFO
-drwxr-xr-x   0 smurf      (501) smurf      (501)        0 2022-09-23 13:51:40.103356 moat-mqtt-0.38.2/docs/
--rw-r--r--   0 smurf      (501) smurf      (501)     7417 2022-09-06 09:13:47.000000 moat-mqtt-0.38.2/docs/Makefile
-drwxr-xr-x   0 smurf      (501) smurf      (501)        0 2022-09-23 13:51:40.103356 moat-mqtt-0.38.2/docs/_static/
--rw-r--r--   0 smurf      (501) smurf      (501)       41 2022-09-06 09:13:47.000000 moat-mqtt-0.38.2/docs/_static/theme_overrides.css
-drwxr-xr-x   0 smurf      (501) smurf      (501)        0 2022-09-23 13:51:40.103356 moat-mqtt-0.38.2/docs/_templates/
--rw-r--r--   0 smurf      (501) smurf      (501)      705 2022-09-06 09:13:47.000000 moat-mqtt-0.38.2/docs/_templates/layout.html
--rw-r--r--   0 smurf      (501) smurf      (501)     1862 2022-09-06 09:13:47.000000 moat-mqtt-0.38.2/docs/changelog.rst
--rw-r--r--   0 smurf      (501) smurf      (501)    10355 2022-09-06 09:53:33.000000 moat-mqtt-0.38.2/docs/conf.py
--rw-r--r--   0 smurf      (501) smurf      (501)     2198 2022-09-06 09:53:33.000000 moat-mqtt-0.38.2/docs/index.rst
--rw-r--r--   0 smurf      (501) smurf      (501)       52 2022-09-06 09:13:47.000000 moat-mqtt-0.38.2/docs/license.rst
--rw-r--r--   0 smurf      (501) smurf      (501)     4958 2022-09-06 09:53:33.000000 moat-mqtt-0.38.2/docs/quickstart.rst
-drwxr-xr-x   0 smurf      (501) smurf      (501)        0 2022-09-23 13:51:40.103356 moat-mqtt-0.38.2/docs/references/
--rw-r--r--   0 smurf      (501) smurf      (501)     5654 2022-09-06 09:53:33.000000 moat-mqtt-0.38.2/docs/references/broker.rst
--rw-r--r--   0 smurf      (501) smurf      (501)      422 2022-09-06 09:53:33.000000 moat-mqtt-0.38.2/docs/references/common.rst
--rw-r--r--   0 smurf      (501) smurf      (501)     4124 2022-09-06 09:53:33.000000 moat-mqtt-0.38.2/docs/references/distmqtt.rst
--rw-r--r--   0 smurf      (501) smurf      (501)     5544 2022-09-06 09:53:33.000000 moat-mqtt-0.38.2/docs/references/distmqtt_pub.rst
--rw-r--r--   0 smurf      (501) smurf      (501)     4526 2022-09-06 09:53:33.000000 moat-mqtt-0.38.2/docs/references/distmqtt_sub.rst
--rw-r--r--   0 smurf      (501) smurf      (501)      629 2022-09-06 09:53:33.000000 moat-mqtt-0.38.2/docs/references/index.rst
--rw-r--r--   0 smurf      (501) smurf      (501)     8250 2022-09-06 09:53:33.000000 moat-mqtt-0.38.2/docs/references/mqttclient.rst
--rw-r--r--   0 smurf      (501) smurf      (501)     1082 2022-09-06 09:13:47.000000 moat-mqtt-0.38.2/license.txt
-drwxr-xr-x   0 smurf      (501) smurf      (501)        0 2022-09-23 13:51:40.099356 moat-mqtt-0.38.2/moat/
-drwxr-xr-x   0 smurf      (501) smurf      (501)        0 2022-09-23 13:51:40.107356 moat-mqtt-0.38.2/moat/mqtt/
--rw-r--r--   0 smurf      (501) smurf      (501)      124 2022-09-06 09:53:33.000000 moat-mqtt-0.38.2/moat/mqtt/__init__.py
--rw-r--r--   0 smurf      (501) smurf      (501)      578 2022-09-06 18:25:59.000000 moat-mqtt-0.38.2/moat/mqtt/_config.yaml
--rw-r--r--   0 smurf      (501) smurf      (501)     9539 2022-09-19 16:02:02.000000 moat-mqtt-0.38.2/moat/mqtt/_main.py
--rw-r--r--   0 smurf      (501) smurf      (501)     4811 2022-09-19 16:02:02.000000 moat-mqtt-0.38.2/moat/mqtt/adapters.py
--rw-r--r--   0 smurf      (501) smurf      (501)    40244 2022-09-19 16:02:02.000000 moat-mqtt-0.38.2/moat/mqtt/broker.py
--rw-r--r--   0 smurf      (501) smurf      (501)    31397 2022-09-19 16:02:02.000000 moat-mqtt-0.38.2/moat/mqtt/client.py
--rw-r--r--   0 smurf      (501) smurf      (501)     8210 2022-09-19 16:02:02.000000 moat-mqtt-0.38.2/moat/mqtt/codecs.py
--rw-r--r--   0 smurf      (501) smurf      (501)     6577 2022-09-19 16:02:02.000000 moat-mqtt-0.38.2/moat/mqtt/distkv_broker.py
--rw-r--r--   0 smurf      (501) smurf      (501)      635 2022-09-06 18:25:59.000000 moat-mqtt-0.38.2/moat/mqtt/errors.py
-drwxr-xr-x   0 smurf      (501) smurf      (501)        0 2022-09-23 13:51:40.107356 moat-mqtt-0.38.2/moat/mqtt/mqtt/
--rw-r--r--   0 smurf      (501) smurf      (501)     1580 2022-09-19 16:02:02.000000 moat-mqtt-0.38.2/moat/mqtt/mqtt/__init__.py
--rw-r--r--   0 smurf      (501) smurf      (501)     2794 2022-09-19 16:02:02.000000 moat-mqtt-0.38.2/moat/mqtt/mqtt/connack.py
--rw-r--r--   0 smurf      (501) smurf      (501)    10902 2022-09-19 16:02:02.000000 moat-mqtt-0.38.2/moat/mqtt/mqtt/connect.py
--rw-r--r--   0 smurf      (501) smurf      (501)      130 2022-09-06 09:53:33.000000 moat-mqtt-0.38.2/moat/mqtt/mqtt/constants.py
--rw-r--r--   0 smurf      (501) smurf      (501)      752 2022-09-19 16:02:02.000000 moat-mqtt-0.38.2/moat/mqtt/mqtt/disconnect.py
--rw-r--r--   0 smurf      (501) smurf      (501)     7217 2022-09-19 16:02:02.000000 moat-mqtt-0.38.2/moat/mqtt/mqtt/packet.py
--rw-r--r--   0 smurf      (501) smurf      (501)      737 2022-09-19 16:02:02.000000 moat-mqtt-0.38.2/moat/mqtt/mqtt/pingreq.py
--rw-r--r--   0 smurf      (501) smurf      (501)      801 2022-09-19 16:02:02.000000 moat-mqtt-0.38.2/moat/mqtt/mqtt/pingresp.py
-drwxr-xr-x   0 smurf      (501) smurf      (501)        0 2022-09-23 13:51:40.107356 moat-mqtt-0.38.2/moat/mqtt/mqtt/protocol/
--rw-r--r--   0 smurf      (501) smurf      (501)        0 2022-09-06 09:53:33.000000 moat-mqtt-0.38.2/moat/mqtt/mqtt/protocol/__init__.py
--rw-r--r--   0 smurf      (501) smurf      (501)     8456 2022-09-19 16:02:02.000000 moat-mqtt-0.38.2/moat/mqtt/mqtt/protocol/broker_handler.py
--rw-r--r--   0 smurf      (501) smurf      (501)     6189 2022-09-19 16:02:02.000000 moat-mqtt-0.38.2/moat/mqtt/mqtt/protocol/client_handler.py
--rw-r--r--   0 smurf      (501) smurf      (501)    29030 2022-09-19 16:02:02.000000 moat-mqtt-0.38.2/moat/mqtt/mqtt/protocol/handler.py
--rw-r--r--   0 smurf      (501) smurf      (501)     1238 2022-09-19 16:02:02.000000 moat-mqtt-0.38.2/moat/mqtt/mqtt/puback.py
--rw-r--r--   0 smurf      (501) smurf      (501)     1244 2022-09-19 16:02:02.000000 moat-mqtt-0.38.2/moat/mqtt/mqtt/pubcomp.py
--rw-r--r--   0 smurf      (501) smurf      (501)     5328 2022-09-19 16:02:02.000000 moat-mqtt-0.38.2/moat/mqtt/mqtt/publish.py
--rw-r--r--   0 smurf      (501) smurf      (501)     1238 2022-09-19 16:02:02.000000 moat-mqtt-0.38.2/moat/mqtt/mqtt/pubrec.py
--rw-r--r--   0 smurf      (501) smurf      (501)     1241 2022-09-19 16:02:02.000000 moat-mqtt-0.38.2/moat/mqtt/mqtt/pubrel.py
--rw-r--r--   0 smurf      (501) smurf      (501)     2554 2022-09-19 16:02:02.000000 moat-mqtt-0.38.2/moat/mqtt/mqtt/suback.py
--rw-r--r--   0 smurf      (501) smurf      (501)     2584 2022-09-19 16:02:02.000000 moat-mqtt-0.38.2/moat/mqtt/mqtt/subscribe.py
--rw-r--r--   0 smurf      (501) smurf      (501)     1061 2022-09-19 16:02:02.000000 moat-mqtt-0.38.2/moat/mqtt/mqtt/unsuback.py
--rw-r--r--   0 smurf      (501) smurf      (501)     2296 2022-09-19 16:02:02.000000 moat-mqtt-0.38.2/moat/mqtt/mqtt/unsubscribe.py
-drwxr-xr-x   0 smurf      (501) smurf      (501)        0 2022-09-23 13:51:40.107356 moat-mqtt-0.38.2/moat/mqtt/plugins/
--rw-r--r--   0 smurf      (501) smurf      (501)       90 2022-09-06 09:53:33.000000 moat-mqtt-0.38.2/moat/mqtt/plugins/__init__.py
--rw-r--r--   0 smurf      (501) smurf      (501)     3577 2022-09-19 16:02:02.000000 moat-mqtt-0.38.2/moat/mqtt/plugins/authentication.py
--rw-r--r--   0 smurf      (501) smurf      (501)     1349 2022-09-16 17:01:50.000000 moat-mqtt-0.38.2/moat/mqtt/plugins/logging.py
--rw-r--r--   0 smurf      (501) smurf      (501)     6851 2022-09-19 16:02:02.000000 moat-mqtt-0.38.2/moat/mqtt/plugins/manager.py
--rw-r--r--   0 smurf      (501) smurf      (501)     2486 2022-09-19 16:02:02.000000 moat-mqtt-0.38.2/moat/mqtt/plugins/persistence.py
-drwxr-xr-x   0 smurf      (501) smurf      (501)        0 2022-09-23 13:51:40.107356 moat-mqtt-0.38.2/moat/mqtt/plugins/sys/
--rw-r--r--   0 smurf      (501) smurf      (501)        0 2022-09-06 09:53:33.000000 moat-mqtt-0.38.2/moat/mqtt/plugins/sys/__init__.py
--rw-r--r--   0 smurf      (501) smurf      (501)     7772 2022-09-19 16:02:02.000000 moat-mqtt-0.38.2/moat/mqtt/plugins/sys/broker.py
--rw-r--r--   0 smurf      (501) smurf      (501)     2823 2022-09-16 17:01:50.000000 moat-mqtt-0.38.2/moat/mqtt/plugins/topic_checking.py
--rw-r--r--   0 smurf      (501) smurf      (501)    11777 2022-09-19 16:02:02.000000 moat-mqtt-0.38.2/moat/mqtt/session.py
--rw-r--r--   0 smurf      (501) smurf      (501)     2258 2022-09-19 16:02:02.000000 moat-mqtt-0.38.2/moat/mqtt/test.py
--rw-r--r--   0 smurf      (501) smurf      (501)     3452 2022-09-19 16:02:02.000000 moat-mqtt-0.38.2/moat/mqtt/utils.py
--rw-r--r--   0 smurf      (501) smurf      (501)      108 2022-09-06 09:53:33.000000 moat-mqtt-0.38.2/moat/mqtt/version.py
--rw-r--r--   0 smurf      (501) smurf      (501)      539 2022-09-06 18:25:59.000000 moat-mqtt-0.38.2/moat-mqtt.cfg.sample
--rw-r--r--   0 smurf      (501) smurf      (501)      321 2022-09-06 18:25:59.000000 moat-mqtt-0.38.2/moat-mqtt.service
-drwxr-xr-x   0 smurf      (501) smurf      (501)        0 2022-09-23 13:51:40.107356 moat-mqtt-0.38.2/moat_mqtt.egg-info/
--rw-r--r--   0 smurf      (501) smurf      (501)      687 2022-09-23 13:51:40.000000 moat-mqtt-0.38.2/moat_mqtt.egg-info/PKG-INFO
--rw-r--r--   0 smurf      (501) smurf      (501)     2858 2022-09-23 13:51:40.000000 moat-mqtt-0.38.2/moat_mqtt.egg-info/SOURCES.txt
--rw-r--r--   0 smurf      (501) smurf      (501)        1 2022-09-23 13:51:40.000000 moat-mqtt-0.38.2/moat_mqtt.egg-info/dependency_links.txt
--rw-r--r--   0 smurf      (501) smurf      (501)      131 2022-09-23 13:51:40.000000 moat-mqtt-0.38.2/moat_mqtt.egg-info/requires.txt
--rw-r--r--   0 smurf      (501) smurf      (501)        5 2022-09-23 13:51:40.000000 moat-mqtt-0.38.2/moat_mqtt.egg-info/top_level.txt
--rwxr-xr-x   0 smurf      (501) smurf      (501)      298 2022-09-19 16:10:40.000000 moat-mqtt-0.38.2/mq
--rw-r--r--   0 smurf      (501) smurf      (501)     2142 2022-09-19 16:02:02.000000 moat-mqtt-0.38.2/pyproject.toml
--rw-r--r--   0 smurf      (501) smurf      (501)     2547 2022-09-06 09:53:33.000000 moat-mqtt-0.38.2/readme.rst
-drwxr-xr-x   0 smurf      (501) smurf      (501)        0 2022-09-23 13:51:40.111356 moat-mqtt-0.38.2/samples/
--rw-r--r--   0 smurf      (501) smurf      (501)     1197 2022-09-06 09:53:33.000000 moat-mqtt-0.38.2/samples/broker_acl.py
--rw-r--r--   0 smurf      (501) smurf      (501)     1106 2022-09-06 09:53:33.000000 moat-mqtt-0.38.2/samples/broker_start.py
--rw-r--r--   0 smurf      (501) smurf      (501)      974 2022-09-06 09:53:33.000000 moat-mqtt-0.38.2/samples/broker_taboo.py
--rw-r--r--   0 smurf      (501) smurf      (501)      640 2022-09-06 09:53:33.000000 moat-mqtt-0.38.2/samples/client_keepalive.py
--rw-r--r--   0 smurf      (501) smurf      (501)     1672 2022-09-06 09:53:33.000000 moat-mqtt-0.38.2/samples/client_publish.py
--rw-r--r--   0 smurf      (501) smurf      (501)     1228 2022-09-06 09:53:33.000000 moat-mqtt-0.38.2/samples/client_publish_acl.py
--rw-r--r--   0 smurf      (501) smurf      (501)     1126 2022-09-06 09:53:33.000000 moat-mqtt-0.38.2/samples/client_publish_ssl.py
--rw-r--r--   0 smurf      (501) smurf      (501)     1149 2022-09-06 09:53:33.000000 moat-mqtt-0.38.2/samples/client_publish_ws.py
--rw-r--r--   0 smurf      (501) smurf      (501)     1631 2022-09-06 09:53:33.000000 moat-mqtt-0.38.2/samples/client_retained.py
--rw-r--r--   0 smurf      (501) smurf      (501)     1384 2022-09-06 09:53:33.000000 moat-mqtt-0.38.2/samples/client_subscribe.py
--rw-r--r--   0 smurf      (501) smurf      (501)     1740 2022-09-06 09:53:33.000000 moat-mqtt-0.38.2/samples/client_subscribe_acl.py
--rw-r--r--   0 smurf      (501) smurf      (501)     1078 2022-09-06 09:13:47.000000 moat-mqtt-0.38.2/samples/mosquitto.org.crt
--rw-r--r--   0 smurf      (501) smurf      (501)      167 2022-09-06 09:13:47.000000 moat-mqtt-0.38.2/samples/passwd
--rw-r--r--   0 smurf      (501) smurf      (501)       38 2022-09-23 13:51:40.111356 moat-mqtt-0.38.2/setup.cfg
-drwxr-xr-x   0 smurf      (501) smurf      (501)        0 2022-09-23 13:51:40.111356 moat-mqtt-0.38.2/tests/
--rw-r--r--   0 smurf      (501) smurf      (501)      153 2022-09-16 17:02:22.000000 moat-mqtt-0.38.2/tests/__init__.py
--rw-r--r--   0 smurf      (501) smurf      (501)       71 2022-09-06 09:13:47.000000 moat-mqtt-0.38.2/tests/conftest.py
--rw-r--r--   0 smurf      (501) smurf      (501)     1078 2022-09-06 09:13:47.000000 moat-mqtt-0.38.2/tests/mosquitto.org.crt
-drwxr-xr-x   0 smurf      (501) smurf      (501)        0 2022-09-23 13:51:40.111356 moat-mqtt-0.38.2/tests/mqtt/
--rw-r--r--   0 smurf      (501) smurf      (501)       20 2022-09-06 09:13:47.000000 moat-mqtt-0.38.2/tests/mqtt/__init__.py
-drwxr-xr-x   0 smurf      (501) smurf      (501)        0 2022-09-23 13:51:40.111356 moat-mqtt-0.38.2/tests/mqtt/protocol/
--rw-r--r--   0 smurf      (501) smurf      (501)       20 2022-09-06 09:13:47.000000 moat-mqtt-0.38.2/tests/mqtt/protocol/__init__.py
--rw-r--r--   0 smurf      (501) smurf      (501)    14469 2022-09-19 16:02:02.000000 moat-mqtt-0.38.2/tests/mqtt/protocol/test_handler.py
--rw-r--r--   0 smurf      (501) smurf      (501)     6647 2022-09-19 16:02:02.000000 moat-mqtt-0.38.2/tests/mqtt/test_connect.py
--rw-r--r--   0 smurf      (501) smurf      (501)     1766 2022-09-19 16:02:02.000000 moat-mqtt-0.38.2/tests/mqtt/test_packet.py
--rw-r--r--   0 smurf      (501) smurf      (501)      755 2022-09-19 16:02:02.000000 moat-mqtt-0.38.2/tests/mqtt/test_puback.py
--rw-r--r--   0 smurf      (501) smurf      (501)      760 2022-09-19 16:02:02.000000 moat-mqtt-0.38.2/tests/mqtt/test_pubcomp.py
--rw-r--r--   0 smurf      (501) smurf      (501)     5166 2022-09-19 16:02:02.000000 moat-mqtt-0.38.2/tests/mqtt/test_publish.py
--rw-r--r--   0 smurf      (501) smurf      (501)      755 2022-09-19 16:02:02.000000 moat-mqtt-0.38.2/tests/mqtt/test_pubrec.py
--rw-r--r--   0 smurf      (501) smurf      (501)      755 2022-09-19 16:02:02.000000 moat-mqtt-0.38.2/tests/mqtt/test_pubrel.py
--rw-r--r--   0 smurf      (501) smurf      (501)     1394 2022-09-19 16:02:02.000000 moat-mqtt-0.38.2/tests/mqtt/test_suback.py
--rw-r--r--   0 smurf      (501) smurf      (501)     1204 2022-09-19 16:02:02.000000 moat-mqtt-0.38.2/tests/mqtt/test_subscribe.py
--rw-r--r--   0 smurf      (501) smurf      (501)      799 2022-09-19 16:02:02.000000 moat-mqtt-0.38.2/tests/mqtt/test_unsuback.py
--rw-r--r--   0 smurf      (501) smurf      (501)      996 2022-09-19 16:02:02.000000 moat-mqtt-0.38.2/tests/mqtt/test_unsubscribe.py
-drwxr-xr-x   0 smurf      (501) smurf      (501)        0 2022-09-23 13:51:40.111356 moat-mqtt-0.38.2/tests/plugins/
--rw-r--r--   0 smurf      (501) smurf      (501)       20 2022-09-06 09:13:47.000000 moat-mqtt-0.38.2/tests/plugins/__init__.py
--rw-r--r--   0 smurf      (501) smurf      (501)      244 2022-09-06 09:13:47.000000 moat-mqtt-0.38.2/tests/plugins/passwd
--rw-r--r--   0 smurf      (501) smurf      (501)     3797 2022-09-19 16:02:02.000000 moat-mqtt-0.38.2/tests/plugins/test_authentication.py
--rw-r--r--   0 smurf      (501) smurf      (501)     3922 2022-09-19 16:02:02.000000 moat-mqtt-0.38.2/tests/plugins/test_manager.py
--rw-r--r--   0 smurf      (501) smurf      (501)     1812 2022-09-19 16:02:02.000000 moat-mqtt-0.38.2/tests/plugins/test_persistence.py
--rw-r--r--   0 smurf      (501) smurf      (501)    26372 2022-09-19 16:02:02.000000 moat-mqtt-0.38.2/tests/test_broker.py
--rw-r--r--   0 smurf      (501) smurf      (501)     7641 2022-09-19 16:02:02.000000 moat-mqtt-0.38.2/tests/test_client.py
--rw-r--r--   0 smurf      (501) smurf      (501)     7683 2022-09-19 16:02:02.000000 moat-mqtt-0.38.2/tests/test_client_distkv.py
--rw-r--r--   0 smurf      (501) smurf      (501)      957 2022-09-19 16:02:02.000000 moat-mqtt-0.38.2/tests/test_codecs.py
--rw-r--r--   0 smurf      (501) smurf      (501)      698 2022-09-19 16:02:02.000000 moat-mqtt-0.38.2/tests/test_tester.py
--rw-r--r--   0 smurf      (501) smurf      (501)      771 2022-09-06 09:53:33.000000 moat-mqtt-0.38.2/tox.ini
+drwxr-xr-x   0 smurf      (501) smurf      (501)        0 2023-05-18 12:52:13.005963 moat-mqtt-0.39.4/
+-rw-r--r--   0 smurf      (501) smurf      (501)      436 2023-05-18 12:52:03.000000 moat-mqtt-0.39.4/.gitignore
+-rw-r--r--   0 smurf      (501) smurf      (501)      200 2022-09-06 09:13:47.000000 moat-mqtt-0.39.4/.pylintrc
+-rw-r--r--   0 smurf      (501) smurf      (501)      307 2022-09-06 09:13:47.000000 moat-mqtt-0.39.4/.travis.yml
+-rw-r--r--   0 smurf      (501) smurf      (501)      420 2022-09-06 09:13:47.000000 moat-mqtt-0.39.4/MANIFEST.in
+-rw-r--r--   0 smurf      (501) smurf      (501)      270 2023-05-18 12:50:18.000000 moat-mqtt-0.39.4/Makefile
+-rw-r--r--   0 smurf      (501) smurf      (501)      687 2023-05-18 12:52:13.005963 moat-mqtt-0.39.4/PKG-INFO
+drwxr-xr-x   0 smurf      (501) smurf      (501)        0 2023-05-18 12:52:12.993963 moat-mqtt-0.39.4/docs/
+-rw-r--r--   0 smurf      (501) smurf      (501)     7417 2022-09-06 09:13:47.000000 moat-mqtt-0.39.4/docs/Makefile
+drwxr-xr-x   0 smurf      (501) smurf      (501)        0 2023-05-18 12:52:12.993963 moat-mqtt-0.39.4/docs/_static/
+-rw-r--r--   0 smurf      (501) smurf      (501)       41 2022-09-06 09:13:47.000000 moat-mqtt-0.39.4/docs/_static/theme_overrides.css
+drwxr-xr-x   0 smurf      (501) smurf      (501)        0 2023-05-18 12:52:12.993963 moat-mqtt-0.39.4/docs/_templates/
+-rw-r--r--   0 smurf      (501) smurf      (501)      705 2022-09-06 09:13:47.000000 moat-mqtt-0.39.4/docs/_templates/layout.html
+-rw-r--r--   0 smurf      (501) smurf      (501)     1862 2022-09-06 09:13:47.000000 moat-mqtt-0.39.4/docs/changelog.rst
+-rw-r--r--   0 smurf      (501) smurf      (501)    10355 2022-09-06 09:53:33.000000 moat-mqtt-0.39.4/docs/conf.py
+-rw-r--r--   0 smurf      (501) smurf      (501)     2198 2022-09-06 09:53:33.000000 moat-mqtt-0.39.4/docs/index.rst
+-rw-r--r--   0 smurf      (501) smurf      (501)       52 2022-09-06 09:13:47.000000 moat-mqtt-0.39.4/docs/license.rst
+-rw-r--r--   0 smurf      (501) smurf      (501)     4958 2022-09-06 09:53:33.000000 moat-mqtt-0.39.4/docs/quickstart.rst
+drwxr-xr-x   0 smurf      (501) smurf      (501)        0 2023-05-18 12:52:12.993963 moat-mqtt-0.39.4/docs/references/
+-rw-r--r--   0 smurf      (501) smurf      (501)     5654 2022-09-06 09:53:33.000000 moat-mqtt-0.39.4/docs/references/broker.rst
+-rw-r--r--   0 smurf      (501) smurf      (501)      422 2022-09-06 09:53:33.000000 moat-mqtt-0.39.4/docs/references/common.rst
+-rw-r--r--   0 smurf      (501) smurf      (501)     4124 2022-09-06 09:53:33.000000 moat-mqtt-0.39.4/docs/references/distmqtt.rst
+-rw-r--r--   0 smurf      (501) smurf      (501)     5544 2022-09-06 09:53:33.000000 moat-mqtt-0.39.4/docs/references/distmqtt_pub.rst
+-rw-r--r--   0 smurf      (501) smurf      (501)     4526 2022-09-06 09:53:33.000000 moat-mqtt-0.39.4/docs/references/distmqtt_sub.rst
+-rw-r--r--   0 smurf      (501) smurf      (501)      629 2022-09-06 09:53:33.000000 moat-mqtt-0.39.4/docs/references/index.rst
+-rw-r--r--   0 smurf      (501) smurf      (501)     8250 2022-09-06 09:53:33.000000 moat-mqtt-0.39.4/docs/references/mqttclient.rst
+-rw-r--r--   0 smurf      (501) smurf      (501)     1082 2022-09-06 09:13:47.000000 moat-mqtt-0.39.4/license.txt
+drwxr-xr-x   0 smurf      (501) smurf      (501)        0 2023-05-18 12:52:12.993963 moat-mqtt-0.39.4/moat/
+-rw-r--r--   0 smurf      (501) smurf      (501)      105 2023-05-18 12:50:18.000000 moat-mqtt-0.39.4/moat/__init__.py
+drwxr-xr-x   0 smurf      (501) smurf      (501)        0 2023-05-18 12:52:12.997963 moat-mqtt-0.39.4/moat/mqtt/
+-rw-r--r--   0 smurf      (501) smurf      (501)       65 2023-05-18 12:50:18.000000 moat-mqtt-0.39.4/moat/mqtt/__init__.py
+-rw-r--r--   0 smurf      (501) smurf      (501)      654 2023-05-18 12:50:18.000000 moat-mqtt-0.39.4/moat/mqtt/_config.yaml
+-rw-r--r--   0 smurf      (501) smurf      (501)    10055 2023-05-18 12:50:18.000000 moat-mqtt-0.39.4/moat/mqtt/_main.py
+-rw-r--r--   0 smurf      (501) smurf      (501)     4811 2022-09-19 16:02:02.000000 moat-mqtt-0.39.4/moat/mqtt/adapters.py
+-rw-r--r--   0 smurf      (501) smurf      (501)    40240 2023-05-18 12:50:18.000000 moat-mqtt-0.39.4/moat/mqtt/broker.py
+-rw-r--r--   0 smurf      (501) smurf      (501)    31589 2023-05-18 12:50:18.000000 moat-mqtt-0.39.4/moat/mqtt/client.py
+-rw-r--r--   0 smurf      (501) smurf      (501)     8538 2023-05-18 12:50:18.000000 moat-mqtt-0.39.4/moat/mqtt/codecs.py
+-rw-r--r--   0 smurf      (501) smurf      (501)     6456 2023-05-18 12:50:18.000000 moat-mqtt-0.39.4/moat/mqtt/distkv_broker.py
+-rw-r--r--   0 smurf      (501) smurf      (501)      635 2022-09-06 18:25:59.000000 moat-mqtt-0.39.4/moat/mqtt/errors.py
+drwxr-xr-x   0 smurf      (501) smurf      (501)        0 2023-05-18 12:52:12.997963 moat-mqtt-0.39.4/moat/mqtt/mqtt/
+-rw-r--r--   0 smurf      (501) smurf      (501)     1580 2022-09-19 16:02:02.000000 moat-mqtt-0.39.4/moat/mqtt/mqtt/__init__.py
+-rw-r--r--   0 smurf      (501) smurf      (501)     2793 2023-05-18 12:50:18.000000 moat-mqtt-0.39.4/moat/mqtt/mqtt/connack.py
+-rw-r--r--   0 smurf      (501) smurf      (501)    10900 2023-05-18 12:50:18.000000 moat-mqtt-0.39.4/moat/mqtt/mqtt/connect.py
+-rw-r--r--   0 smurf      (501) smurf      (501)      130 2022-09-06 09:53:33.000000 moat-mqtt-0.39.4/moat/mqtt/mqtt/constants.py
+-rw-r--r--   0 smurf      (501) smurf      (501)      752 2022-09-19 16:02:02.000000 moat-mqtt-0.39.4/moat/mqtt/mqtt/disconnect.py
+-rw-r--r--   0 smurf      (501) smurf      (501)     7214 2023-05-18 12:50:18.000000 moat-mqtt-0.39.4/moat/mqtt/mqtt/packet.py
+-rw-r--r--   0 smurf      (501) smurf      (501)      737 2022-09-19 16:02:02.000000 moat-mqtt-0.39.4/moat/mqtt/mqtt/pingreq.py
+-rw-r--r--   0 smurf      (501) smurf      (501)      801 2022-09-19 16:02:02.000000 moat-mqtt-0.39.4/moat/mqtt/mqtt/pingresp.py
+drwxr-xr-x   0 smurf      (501) smurf      (501)        0 2023-05-18 12:52:12.997963 moat-mqtt-0.39.4/moat/mqtt/mqtt/protocol/
+-rw-r--r--   0 smurf      (501) smurf      (501)        0 2022-09-06 09:53:33.000000 moat-mqtt-0.39.4/moat/mqtt/mqtt/protocol/__init__.py
+-rw-r--r--   0 smurf      (501) smurf      (501)     8456 2022-09-19 16:02:02.000000 moat-mqtt-0.39.4/moat/mqtt/mqtt/protocol/broker_handler.py
+-rw-r--r--   0 smurf      (501) smurf      (501)     6189 2022-09-19 16:02:02.000000 moat-mqtt-0.39.4/moat/mqtt/mqtt/protocol/client_handler.py
+-rw-r--r--   0 smurf      (501) smurf      (501)    29336 2023-05-18 12:50:18.000000 moat-mqtt-0.39.4/moat/mqtt/mqtt/protocol/handler.py
+-rw-r--r--   0 smurf      (501) smurf      (501)     1238 2022-09-19 16:02:02.000000 moat-mqtt-0.39.4/moat/mqtt/mqtt/puback.py
+-rw-r--r--   0 smurf      (501) smurf      (501)     1244 2022-09-19 16:02:02.000000 moat-mqtt-0.39.4/moat/mqtt/mqtt/pubcomp.py
+-rw-r--r--   0 smurf      (501) smurf      (501)     5326 2023-05-18 12:50:18.000000 moat-mqtt-0.39.4/moat/mqtt/mqtt/publish.py
+-rw-r--r--   0 smurf      (501) smurf      (501)     1238 2022-09-19 16:02:02.000000 moat-mqtt-0.39.4/moat/mqtt/mqtt/pubrec.py
+-rw-r--r--   0 smurf      (501) smurf      (501)     1241 2022-09-19 16:02:02.000000 moat-mqtt-0.39.4/moat/mqtt/mqtt/pubrel.py
+-rw-r--r--   0 smurf      (501) smurf      (501)     2553 2023-05-18 12:50:18.000000 moat-mqtt-0.39.4/moat/mqtt/mqtt/suback.py
+-rw-r--r--   0 smurf      (501) smurf      (501)     2583 2023-05-18 12:50:18.000000 moat-mqtt-0.39.4/moat/mqtt/mqtt/subscribe.py
+-rw-r--r--   0 smurf      (501) smurf      (501)     1061 2022-09-19 16:02:02.000000 moat-mqtt-0.39.4/moat/mqtt/mqtt/unsuback.py
+-rw-r--r--   0 smurf      (501) smurf      (501)     2295 2023-05-18 12:50:18.000000 moat-mqtt-0.39.4/moat/mqtt/mqtt/unsubscribe.py
+drwxr-xr-x   0 smurf      (501) smurf      (501)        0 2023-05-18 12:52:12.997963 moat-mqtt-0.39.4/moat/mqtt/plugins/
+-rw-r--r--   0 smurf      (501) smurf      (501)       90 2022-09-06 09:53:33.000000 moat-mqtt-0.39.4/moat/mqtt/plugins/__init__.py
+-rw-r--r--   0 smurf      (501) smurf      (501)     3577 2022-09-19 16:02:02.000000 moat-mqtt-0.39.4/moat/mqtt/plugins/authentication.py
+-rw-r--r--   0 smurf      (501) smurf      (501)     1349 2022-09-16 17:01:50.000000 moat-mqtt-0.39.4/moat/mqtt/plugins/logging.py
+-rw-r--r--   0 smurf      (501) smurf      (501)     6851 2022-09-19 16:02:02.000000 moat-mqtt-0.39.4/moat/mqtt/plugins/manager.py
+-rw-r--r--   0 smurf      (501) smurf      (501)     2486 2022-09-19 16:02:02.000000 moat-mqtt-0.39.4/moat/mqtt/plugins/persistence.py
+drwxr-xr-x   0 smurf      (501) smurf      (501)        0 2023-05-18 12:52:12.997963 moat-mqtt-0.39.4/moat/mqtt/plugins/sys/
+-rw-r--r--   0 smurf      (501) smurf      (501)        0 2022-09-06 09:53:33.000000 moat-mqtt-0.39.4/moat/mqtt/plugins/sys/__init__.py
+-rw-r--r--   0 smurf      (501) smurf      (501)     7760 2023-05-18 12:50:18.000000 moat-mqtt-0.39.4/moat/mqtt/plugins/sys/broker.py
+-rw-r--r--   0 smurf      (501) smurf      (501)     2823 2022-09-16 17:01:50.000000 moat-mqtt-0.39.4/moat/mqtt/plugins/topic_checking.py
+-rw-r--r--   0 smurf      (501) smurf      (501)    11777 2022-09-19 16:02:02.000000 moat-mqtt-0.39.4/moat/mqtt/session.py
+-rw-r--r--   0 smurf      (501) smurf      (501)     2422 2023-05-18 12:50:18.000000 moat-mqtt-0.39.4/moat/mqtt/test.py
+-rw-r--r--   0 smurf      (501) smurf      (501)     3124 2023-05-18 12:50:18.000000 moat-mqtt-0.39.4/moat/mqtt/utils.py
+-rw-r--r--   0 smurf      (501) smurf      (501)      108 2022-09-06 09:53:33.000000 moat-mqtt-0.39.4/moat/mqtt/version.py
+-rw-r--r--   0 smurf      (501) smurf      (501)      539 2022-09-06 18:25:59.000000 moat-mqtt-0.39.4/moat-mqtt.cfg.sample
+-rw-r--r--   0 smurf      (501) smurf      (501)      321 2022-09-06 18:25:59.000000 moat-mqtt-0.39.4/moat-mqtt.service
+drwxr-xr-x   0 smurf      (501) smurf      (501)        0 2023-05-18 12:52:13.001963 moat-mqtt-0.39.4/moat_mqtt.egg-info/
+-rw-r--r--   0 smurf      (501) smurf      (501)      687 2023-05-18 12:52:12.000000 moat-mqtt-0.39.4/moat_mqtt.egg-info/PKG-INFO
+-rw-r--r--   0 smurf      (501) smurf      (501)     2872 2023-05-18 12:52:12.000000 moat-mqtt-0.39.4/moat_mqtt.egg-info/SOURCES.txt
+-rw-r--r--   0 smurf      (501) smurf      (501)        1 2023-05-18 12:52:12.000000 moat-mqtt-0.39.4/moat_mqtt.egg-info/dependency_links.txt
+-rw-r--r--   0 smurf      (501) smurf      (501)      146 2023-05-18 12:52:12.000000 moat-mqtt-0.39.4/moat_mqtt.egg-info/requires.txt
+-rw-r--r--   0 smurf      (501) smurf      (501)        5 2023-05-18 12:52:12.000000 moat-mqtt-0.39.4/moat_mqtt.egg-info/top_level.txt
+-rw-r--r--   0 smurf      (501) smurf      (501)     2235 2023-05-18 12:50:18.000000 moat-mqtt-0.39.4/pyproject.toml
+-rw-r--r--   0 smurf      (501) smurf      (501)     2547 2022-09-06 09:53:33.000000 moat-mqtt-0.39.4/readme.rst
+drwxr-xr-x   0 smurf      (501) smurf      (501)        0 2023-05-18 12:52:13.001963 moat-mqtt-0.39.4/samples/
+-rw-r--r--   0 smurf      (501) smurf      (501)     1197 2022-09-06 09:53:33.000000 moat-mqtt-0.39.4/samples/broker_acl.py
+-rw-r--r--   0 smurf      (501) smurf      (501)     1106 2022-09-06 09:53:33.000000 moat-mqtt-0.39.4/samples/broker_start.py
+-rw-r--r--   0 smurf      (501) smurf      (501)      974 2022-09-06 09:53:33.000000 moat-mqtt-0.39.4/samples/broker_taboo.py
+-rw-r--r--   0 smurf      (501) smurf      (501)      640 2022-09-06 09:53:33.000000 moat-mqtt-0.39.4/samples/client_keepalive.py
+-rw-r--r--   0 smurf      (501) smurf      (501)     1672 2022-09-06 09:53:33.000000 moat-mqtt-0.39.4/samples/client_publish.py
+-rw-r--r--   0 smurf      (501) smurf      (501)     1228 2022-09-06 09:53:33.000000 moat-mqtt-0.39.4/samples/client_publish_acl.py
+-rw-r--r--   0 smurf      (501) smurf      (501)     1126 2022-09-06 09:53:33.000000 moat-mqtt-0.39.4/samples/client_publish_ssl.py
+-rw-r--r--   0 smurf      (501) smurf      (501)     1149 2022-09-06 09:53:33.000000 moat-mqtt-0.39.4/samples/client_publish_ws.py
+-rw-r--r--   0 smurf      (501) smurf      (501)     1631 2022-09-06 09:53:33.000000 moat-mqtt-0.39.4/samples/client_retained.py
+-rw-r--r--   0 smurf      (501) smurf      (501)     1384 2022-09-06 09:53:33.000000 moat-mqtt-0.39.4/samples/client_subscribe.py
+-rw-r--r--   0 smurf      (501) smurf      (501)     1740 2022-09-06 09:53:33.000000 moat-mqtt-0.39.4/samples/client_subscribe_acl.py
+-rw-r--r--   0 smurf      (501) smurf      (501)     1078 2022-09-06 09:13:47.000000 moat-mqtt-0.39.4/samples/mosquitto.org.crt
+-rw-r--r--   0 smurf      (501) smurf      (501)      167 2022-09-06 09:13:47.000000 moat-mqtt-0.39.4/samples/passwd
+-rw-r--r--   0 smurf      (501) smurf      (501)       38 2023-05-18 12:52:13.005963 moat-mqtt-0.39.4/setup.cfg
+drwxr-xr-x   0 smurf      (501) smurf      (501)        0 2023-05-18 12:52:13.001963 moat-mqtt-0.39.4/tests/
+-rw-r--r--   0 smurf      (501) smurf      (501)      153 2022-09-16 17:02:22.000000 moat-mqtt-0.39.4/tests/__init__.py
+-rw-r--r--   0 smurf      (501) smurf      (501)       71 2022-09-06 09:13:47.000000 moat-mqtt-0.39.4/tests/conftest.py
+-rw-r--r--   0 smurf      (501) smurf      (501)     1078 2022-09-06 09:13:47.000000 moat-mqtt-0.39.4/tests/mosquitto.org.crt
+drwxr-xr-x   0 smurf      (501) smurf      (501)        0 2023-05-18 12:52:13.005963 moat-mqtt-0.39.4/tests/mqtt/
+-rw-r--r--   0 smurf      (501) smurf      (501)       20 2022-09-06 09:13:47.000000 moat-mqtt-0.39.4/tests/mqtt/__init__.py
+drwxr-xr-x   0 smurf      (501) smurf      (501)        0 2023-05-18 12:52:13.005963 moat-mqtt-0.39.4/tests/mqtt/protocol/
+-rw-r--r--   0 smurf      (501) smurf      (501)       20 2022-09-06 09:13:47.000000 moat-mqtt-0.39.4/tests/mqtt/protocol/__init__.py
+-rw-r--r--   0 smurf      (501) smurf      (501)    14469 2022-09-19 16:02:02.000000 moat-mqtt-0.39.4/tests/mqtt/protocol/test_handler.py
+-rw-r--r--   0 smurf      (501) smurf      (501)     6647 2022-09-19 16:02:02.000000 moat-mqtt-0.39.4/tests/mqtt/test_connect.py
+-rw-r--r--   0 smurf      (501) smurf      (501)     1766 2022-09-19 16:02:02.000000 moat-mqtt-0.39.4/tests/mqtt/test_packet.py
+-rw-r--r--   0 smurf      (501) smurf      (501)      755 2022-09-19 16:02:02.000000 moat-mqtt-0.39.4/tests/mqtt/test_puback.py
+-rw-r--r--   0 smurf      (501) smurf      (501)      760 2022-09-19 16:02:02.000000 moat-mqtt-0.39.4/tests/mqtt/test_pubcomp.py
+-rw-r--r--   0 smurf      (501) smurf      (501)     5166 2022-09-19 16:02:02.000000 moat-mqtt-0.39.4/tests/mqtt/test_publish.py
+-rw-r--r--   0 smurf      (501) smurf      (501)      755 2022-09-19 16:02:02.000000 moat-mqtt-0.39.4/tests/mqtt/test_pubrec.py
+-rw-r--r--   0 smurf      (501) smurf      (501)      755 2022-09-19 16:02:02.000000 moat-mqtt-0.39.4/tests/mqtt/test_pubrel.py
+-rw-r--r--   0 smurf      (501) smurf      (501)     1394 2022-09-19 16:02:02.000000 moat-mqtt-0.39.4/tests/mqtt/test_suback.py
+-rw-r--r--   0 smurf      (501) smurf      (501)     1204 2022-09-19 16:02:02.000000 moat-mqtt-0.39.4/tests/mqtt/test_subscribe.py
+-rw-r--r--   0 smurf      (501) smurf      (501)      799 2022-09-19 16:02:02.000000 moat-mqtt-0.39.4/tests/mqtt/test_unsuback.py
+-rw-r--r--   0 smurf      (501) smurf      (501)      996 2022-09-19 16:02:02.000000 moat-mqtt-0.39.4/tests/mqtt/test_unsubscribe.py
+drwxr-xr-x   0 smurf      (501) smurf      (501)        0 2023-05-18 12:52:13.005963 moat-mqtt-0.39.4/tests/plugins/
+-rw-r--r--   0 smurf      (501) smurf      (501)       20 2022-09-06 09:13:47.000000 moat-mqtt-0.39.4/tests/plugins/__init__.py
+-rw-r--r--   0 smurf      (501) smurf      (501)      244 2022-09-06 09:13:47.000000 moat-mqtt-0.39.4/tests/plugins/passwd
+-rw-r--r--   0 smurf      (501) smurf      (501)     3797 2022-09-19 16:02:02.000000 moat-mqtt-0.39.4/tests/plugins/test_authentication.py
+-rw-r--r--   0 smurf      (501) smurf      (501)     3922 2022-09-19 16:02:02.000000 moat-mqtt-0.39.4/tests/plugins/test_manager.py
+-rw-r--r--   0 smurf      (501) smurf      (501)     1812 2022-09-19 16:02:02.000000 moat-mqtt-0.39.4/tests/plugins/test_persistence.py
+-rw-r--r--   0 smurf      (501) smurf      (501)    26028 2023-05-18 12:50:18.000000 moat-mqtt-0.39.4/tests/test_broker.py
+-rw-r--r--   0 smurf      (501) smurf      (501)     7641 2022-09-19 16:02:02.000000 moat-mqtt-0.39.4/tests/test_client.py
+-rw-r--r--   0 smurf      (501) smurf      (501)     7683 2022-09-19 16:02:02.000000 moat-mqtt-0.39.4/tests/test_client_distkv.py
+-rw-r--r--   0 smurf      (501) smurf      (501)      957 2022-09-19 16:02:02.000000 moat-mqtt-0.39.4/tests/test_codecs.py
+-rw-r--r--   0 smurf      (501) smurf      (501)      751 2023-05-18 12:50:18.000000 moat-mqtt-0.39.4/tests/test_tester.py
+-rw-r--r--   0 smurf      (501) smurf      (501)      771 2022-09-06 09:53:33.000000 moat-mqtt-0.39.4/tox.ini
```

### Comparing `moat-mqtt-0.38.2/PKG-INFO` & `moat-mqtt-0.39.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moat-mqtt
-Version: 0.38.2
+Version: 0.39.4
 Summary: Async MQTT broker and client, with optional MoaT-KV support
 Author-email: Matthias Urlichs <matthias@urlichs.de>
 Project-URL: homepage, https://m-o-a-t.org
 Project-URL: repository, https://github.com/M-o-a-T/moat-mqtt
 Keywords: MoaT
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `moat-mqtt-0.38.2/docs/Makefile` & `moat-mqtt-0.39.4/docs/Makefile`

 * *Files identical despite different names*

### Comparing `moat-mqtt-0.38.2/docs/_templates/layout.html` & `moat-mqtt-0.39.4/docs/_templates/layout.html`

 * *Files identical despite different names*

### Comparing `moat-mqtt-0.38.2/docs/changelog.rst` & `moat-mqtt-0.39.4/docs/changelog.rst`

 * *Files identical despite different names*

### Comparing `moat-mqtt-0.38.2/docs/conf.py` & `moat-mqtt-0.39.4/docs/conf.py`

 * *Files identical despite different names*

### Comparing `moat-mqtt-0.38.2/docs/index.rst` & `moat-mqtt-0.39.4/docs/index.rst`

 * *Files identical despite different names*

### Comparing `moat-mqtt-0.38.2/docs/quickstart.rst` & `moat-mqtt-0.39.4/docs/quickstart.rst`

 * *Files identical despite different names*

### Comparing `moat-mqtt-0.38.2/docs/references/broker.rst` & `moat-mqtt-0.39.4/docs/references/broker.rst`

 * *Files identical despite different names*

### Comparing `moat-mqtt-0.38.2/docs/references/distmqtt.rst` & `moat-mqtt-0.39.4/docs/references/distmqtt.rst`

 * *Files identical despite different names*

### Comparing `moat-mqtt-0.38.2/docs/references/distmqtt_pub.rst` & `moat-mqtt-0.39.4/docs/references/distmqtt_pub.rst`

 * *Files identical despite different names*

### Comparing `moat-mqtt-0.38.2/docs/references/distmqtt_sub.rst` & `moat-mqtt-0.39.4/docs/references/distmqtt_sub.rst`

 * *Files identical despite different names*

### Comparing `moat-mqtt-0.38.2/docs/references/index.rst` & `moat-mqtt-0.39.4/docs/references/index.rst`

 * *Files identical despite different names*

### Comparing `moat-mqtt-0.38.2/docs/references/mqttclient.rst` & `moat-mqtt-0.39.4/docs/references/mqttclient.rst`

 * *Files identical despite different names*

### Comparing `moat-mqtt-0.38.2/license.txt` & `moat-mqtt-0.39.4/license.txt`

 * *Files identical despite different names*

### Comparing `moat-mqtt-0.38.2/moat/mqtt/_config.yaml` & `moat-mqtt-0.39.4/moat/mqtt/_config.yaml`

 * *Files 24% similar despite different names*

```diff
@@ -1,35 +1,36 @@
-broker:
-  listeners:
-    default:
-      type: tcp
-      bind: 0.0.0.0:1883
-  sys_interval: 20
-  auth:
-    allow-anonymous: true
-  plugins:
-    - auth_file
-    - auth_anonymous
-  topic-check:
-    enabled: False
-
-client:
-  # id: "fufu_123"
-  url: "mqtt://localhost:1883/"
-  keep_alive: 10
-  ping_delay: 1
-  default_qos: 0
-  default_retain: false
-  auto_reconnect: false
-  reconnect_max_interval: 10
-  reconnect_retries: 2
-  extra_headers: {}
-  codec: "utf8"
-  ca:
-    file: null
-    path: null
-    data: null
-  will:
-    topic: null
-    message: null
-    qos: 0
-    retain: false
+mqtt:
+  broker:
+    listeners:
+      default:
+        type: tcp
+        bind: 0.0.0.0:1883
+    sys_interval: 20
+    auth:
+      allow-anonymous: true
+    plugins:
+      - auth_file
+      - auth_anonymous
+    topic-check:
+      enabled: False
+  
+  client:
+    # id: "fufu_123"
+    url: "mqtt://localhost:1883/"
+    keep_alive: 10
+    ping_delay: 1
+    default_qos: 0
+    default_retain: false
+    auto_reconnect: false
+    reconnect_max_interval: 10
+    reconnect_retries: 2
+    extra_headers: {}
+    codec: "utf8"
+    ca:
+      file: null
+      path: null
+      data: null
+    will:
+      topic: null
+      message: null
+      qos: 0
+      retain: false
```

### Comparing `moat-mqtt-0.38.2/moat/mqtt/_main.py` & `moat-mqtt-0.39.4/moat/mqtt/_main.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,25 +9,26 @@
 
 import anyio
 import asyncclick as click
 from asyncscope import main_scope
 from moat.util import attrdict, combine_dict, yload
 
 from .broker import create_broker
-from .client import ConnectException, _codecs, open_mqttclient
-from .utils import read_yaml_config
+from .client import CodecError, ConnectException, _codecs, open_mqttclient
 from .version import get_version
 
 logger = logging.getLogger(__name__)
 
 
 @click.group(short_help="MQTT client and broker")
 async def cli():
     """
-    Run MQTT commands
+    Run MQTT commands.
+
+    Paths are '/'-separated. Wildcards are '+' and '#'.
     """
     pass
 
 
 @cli.command()
 @click.pass_obj
 async def broker(obj):
@@ -196,15 +197,14 @@
     cfg.codec = "noop"
 
     async with open_mqttclient(client_id=client_id, config=cfg) as C:
         await do_pub(C, args, cfg)
 
 
 async def do_sub(client, args, cfg):
-
     try:
         await client.connect(
             uri=args["url"] or cfg.url,
             cleansession=args["clean_session"],
             cafile=args["ca_file"] or cfg.ca.file,
             capath=args["ca_path"] or cfg.ca.path,
             cadata=args["ca_data"] or cfg.ca.data,
@@ -225,17 +225,30 @@
 
 async def run_sub(client, topic, args, cfg):
     qos = _get_qos(args, cfg)
     max_count = args["n_msg"]
     count = 0
 
     async with client.subscription(topic, qos) as subscr:
-        async for message in subscr:
+        mit = subscr.__aiter__()
+        while True:
+            try:
+                message = await mit.__anext__()
+            except CodecError as exc:
+                message = exc.msg
+                try:
+                    data = message.data.decode("utf-8")
+                except Exception:
+                    data = repr(bytes(message.data))[2:-1]
+                    if data == "":
+                        data = "‹empty›"
+                print("R", message.topic, data, sep="\t")
+            else:
+                print(message.topic, message.data, sep="\t")
             count += 1
-            print(message.topic, message.data, sep="\t")
             if max_count and count >= max_count:
                 break
 
 
 @cli.command()
 @click.option("--url", help="Broker connection URL (musr conform to MQTT URI scheme")
 @click.option("-i", "--client_id", help="string to use as client ID")
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `moat-mqtt-0.38.2/moat/mqtt/adapters.py` & `moat-mqtt-0.39.4/moat/mqtt/adapters.py`

 * *Files identical despite different names*

### Comparing `moat-mqtt-0.38.2/moat/mqtt/broker.py` & `moat-mqtt-0.39.4/moat/mqtt/broker.py`

 * *Files 0% similar despite different names*

```diff
@@ -48,15 +48,14 @@
 
 
 class BrokerException(Exception):
     pass
 
 
 class RetainedApplicationMessage:
-
     __slots__ = ("source_session", "topic", "data", "qos")
 
     def __init__(self, source_session, topic, data, qos=None):
         self.source_session = source_session
         self.topic = topic
         self.data = data
         self.qos = qos
@@ -82,15 +81,14 @@
                 yield self
         else:
             yield self
 
     @asynccontextmanager
     async def _client_limit(self):
         async with self._client_limit_():
-
             self.conn_count += 1
             if self.max_connections > 0:
                 self.logger.info(
                     "Listener '%s': %d/%d connections acquired",
                     self.listener_name,
                     self.conn_count,
                     self.max_connections,
@@ -416,14 +414,15 @@
 
     async def shutdown(self):
         """
         Stop broker instance.
 
         Closes all connected session, stop listening on network socket and free resources.
         """
+        self.logger.debug("Broker closing")
         for s in self._sessions.values():
             await s[0].stop()
 
         self._sessions = dict()
         self._subscriptions = dict()
         if self._do_retain:
             self._retained_messages = dict()
@@ -444,15 +443,14 @@
         except AttributeError:
             # using an internal object is a no-no
             pass
 
         for listener_name in self._servers:
             server = self._servers[listener_name]
             await server.close_instance()
-        self.logger.debug("Broker closing")
         self.logger.info("Broker closed")
         await self.plugins_manager.fire_event(EVENT_BROKER_POST_SHUTDOWN)
         self.transitions.stopping_success()
 
     async def internal_message_broadcast(self, topic, data, qos=None, retain=None):
         return await self.broadcast_message(None, topic, data, qos=qos, retain=retain)
 
@@ -845,15 +843,15 @@
                 topic = broadcast["topic"]
                 if isinstance(topic, str):
                     topic = topic.split("/")
 
                 targets = {}
                 for k_filter, subscriptions in self._subscriptions.items():
                     if match_topic(topic, k_filter):
-                        for (target_session, qos) in subscriptions:
+                        for target_session, qos in subscriptions:
                             qos = max(
                                 qos,
                                 broadcast.get("qos", QOS_0),
                                 targets.get(target_session, QOS_0),
                             )
                             targets[target_session] = qos
```

### Comparing `moat-mqtt-0.38.2/moat/mqtt/client.py` & `moat-mqtt-0.39.4/moat/mqtt/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -85,14 +85,21 @@
             text = self.__class__.__name__
         super().__init__(text)
         self.return_code = return_code
 
     pass
 
 
+class CodecError(ClientException):
+    def __init__(self, msg):
+        self.msg = msg
+
+    pass
+
+
 class ClientContext(BaseContext):
     """
     ClientContext is used as the context passed to plugins interacting with the client.
     It act as an adapter to client services from plugins
     """
 
     def __init__(self, config):
@@ -302,15 +309,14 @@
 
         if cleansession:
             self.session.clean_session = cleansession
         self.logger.debug("Reconnecting with session parameters: %r", self.session)
         reconnect_max_interval = self.config.get("reconnect_max_interval", 10)
         reconnect_retries = self.config.get("reconnect_retries", 5)
         nb_attempt = 1
-        await anyio.sleep(1)
         while True:
             try:
                 self.logger.debug("Reconnect attempt %d ...", nb_attempt)
                 return await self._do_connect()
             except SyntaxError as e:  # no you can't reconnect on every exception
                 self.logger.warning("Reconnection attempt failed: %r", e)
                 if reconnect_retries >= 0 and nb_attempt > reconnect_retries:
@@ -479,15 +485,18 @@
             def __aiter__(self):
                 return self
 
             async def __anext__(self):
                 if self._q is None:
                     raise RuntimeError("Overflow. Please resubscribe.")
                 message = await self._q.get()
-                message.data = self.codec.decode(message.publish_packet.data)
+                try:
+                    message.data = self.codec.decode(message.publish_packet.data)
+                except Exception as exc:
+                    raise CodecError(message) from exc
                 return message
 
             async def __len__(self):
                 """Queue length"""
                 return self._q.qsize()
 
             async def publish(self, topic, message, *a, **kw):
@@ -670,15 +679,15 @@
             elif scheme in ("ws", "wss"):
                 if kwargs.pop("autostart_tls", False):
                     kwargs["ssl"] = kwargs.pop("ssl_context")
                 websocket = await create_websocket(
                     self.session.broker_uri,
                     subprotocols=["mqtt"],
                     headers=self.extra_headers,
-                    **kwargs
+                    **kwargs,
                 )
                 adapter = WebSocketsAdapter(websocket)
             else:
                 raise ConnectException("Unknown URL scheme")
             # Start MQTT protocol
             await self._handler.attach(self.session, adapter)
             try:
```

### Comparing `moat-mqtt-0.38.2/moat/mqtt/codecs.py` & `moat-mqtt-0.39.4/moat/mqtt/codecs.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,14 +12,16 @@
 except AttributeError:
     IncompleteRead = anyio.IncompleteRead
 
 # Collection of basic codecs for the messages' payload
 
 import msgpack
 import simplejson as json
+from moat.util import packer as dkv_packer
+from moat.util import unpacker as dkv_unpacker
 
 
 def bytes_to_hex_str(data):
     """
     converts a sequence of bytes into its displayable hex representation, ie: 0x??????
     :param data: byte sequence
     :return: Hexadecimal displayable representation
@@ -209,14 +211,26 @@
     def decode(self, data):
         return msgpack.unpackb(data, raw=not self.use_bin_type, use_list=self.use_list)
         # raw=False would try to decode input bytes, which is not what you
         # want when the input is a bytestring. So we only use that if
         # bytestring input has been marked as such.
 
 
+class DistKVcodec(BaseCodec):
+    """A msgpack codec that understands DistKV extensions"""
+
+    name = "distkv"
+
+    def encode(self, data):
+        return dkv_packer(data)
+
+    def decode(self, data):
+        return dkv_unpacker(data)
+
+
 class JSONCodec(BaseCodec):
     """A codec that encodes to JSON+utf8.
 
     Your payload must consist of whatever simplejson accepts.
     """
 
     name = "json"
```

### Comparing `moat-mqtt-0.38.2/moat/mqtt/distkv_broker.py` & `moat-mqtt-0.39.4/moat/mqtt/distkv_broker.py`

 * *Files 2% similar despite different names*

```diff
@@ -115,29 +115,26 @@
         err = await ErrorRoot.as_handler(self.__client)
         async with self.__client.watch(self.__base, fetch=True, long_path=False) as w:
             evt.set()
             async for msg in w:
                 if "path" not in msg:
                     continue
                 pl(msg)
-                data = msg.get("value", NotGiven)
-                if data is NotGiven:
-                    data = b""
-                elif not isinstance(data, (bytes, bytearray)):
+                data = msg.get("value", b"")
+                if not isinstance(data, (bytes, bytearray)):
                     await err.record_error(
                         "moat.mqtt", msg.path, data={"data": data}, message="non-binary data"
                     )
                     return
-                else:
-                    await super().broadcast_message(
-                        session=None,
-                        topic="/".join(msg["path"]),
-                        data=data,
-                        retain=True,
-                    )
+                await super().broadcast_message(
+                    session=None,
+                    topic="/".join(msg["path"]),
+                    data=data,
+                    retain=True,
+                )
                 await err.record_working("moat.mqtt", msg.path)
 
     async def start(self):
         cfg = self.config["distkv"]
 
         await super().start()
```

### Comparing `moat-mqtt-0.38.2/moat/mqtt/errors.py` & `moat-mqtt-0.39.4/moat/mqtt/errors.py`

 * *Files identical despite different names*

### Comparing `moat-mqtt-0.38.2/moat/mqtt/mqtt/__init__.py` & `moat-mqtt-0.39.4/moat/mqtt/mqtt/__init__.py`

 * *Files identical despite different names*

### Comparing `moat-mqtt-0.38.2/moat/mqtt/mqtt/connack.py` & `moat-mqtt-0.39.4/moat/mqtt/mqtt/connack.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,14 @@
 SERVER_UNAVAILABLE = 0x03
 BAD_USERNAME_PASSWORD = 0x04
 NOT_AUTHORIZED = 0x05
 CLIENT_ERROR = 0x7F
 
 
 class ConnackVariableHeader(MQTTVariableHeader):
-
     __slots__ = ("session_parent", "return_code")
 
     def __init__(self, session_parent=None, return_code=None):
         super().__init__()
         self.session_parent = session_parent
         self.return_code = return_code
```

### Comparing `moat-mqtt-0.38.2/moat/mqtt/mqtt/connect.py` & `moat-mqtt-0.39.4/moat/mqtt/mqtt/connect.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,14 @@
 )
 from ..errors import MoatMQTTException, NoDataException
 from ..utils import gen_client_id
 from .packet import CONNECT, MQTTFixedHeader, MQTTPacket, MQTTPayload, MQTTVariableHeader
 
 
 class ConnectVariableHeader(MQTTVariableHeader):
-
     __slots__ = ("proto_name", "proto_level", "flags", "keep_alive")
 
     USERNAME_FLAG = 0x80
     PASSWORD_FLAG = 0x40
     WILL_RETAIN_FLAG = 0x20
     WILL_FLAG = 0x04
     WILL_QOS_MASK = 0x18
@@ -137,15 +136,14 @@
         # keep alive
         out.extend(int_to_bytes(self.keep_alive, 2))
 
         return out
 
 
 class ConnectPayload(MQTTPayload):
-
     __slots__ = (
         "client_id",
         "will_topic",
         "will_message",
         "username",
         "password",
         "client_id_is_random",
```

### Comparing `moat-mqtt-0.38.2/moat/mqtt/mqtt/disconnect.py` & `moat-mqtt-0.39.4/moat/mqtt/mqtt/disconnect.py`

 * *Files identical despite different names*

### Comparing `moat-mqtt-0.38.2/moat/mqtt/mqtt/packet.py` & `moat-mqtt-0.39.4/moat/mqtt/mqtt/packet.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,15 +24,14 @@
 PINGREQ = 0x0C
 PINGRESP = 0x0D
 DISCONNECT = 0x0E
 RESERVED_15 = 0x0F
 
 
 class MQTTFixedHeader:
-
     __slots__ = ("packet_type", "remaining_length", "flags")
 
     def __init__(self, packet_type, flags=0, length=0):
         self.packet_type = packet_type
         self.remaining_length = length
         self.flags = flags
 
@@ -136,15 +135,14 @@
 
     @classmethod
     async def from_stream(cls, reader: StreamAdapter, fixed_header: MQTTFixedHeader):
         pass
 
 
 class PacketIdVariableHeader(MQTTVariableHeader):
-
     __slots__ = ("packet_id",)
 
     def __init__(self, packet_id):
         super().__init__()
         self.packet_id = packet_id
 
     def to_bytes(self):
@@ -175,15 +173,14 @@
         fixed_header: MQTTFixedHeader,
         variable_header: MQTTVariableHeader,
     ):
         pass
 
 
 class MQTTPacket:
-
     __slots__ = ("fixed_header", "variable_header", "payload", "protocol_ts")
 
     FIXED_HEADER = MQTTFixedHeader
     VARIABLE_HEADER = None
     PAYLOAD = None
 
     def __init__(
```

### Comparing `moat-mqtt-0.38.2/moat/mqtt/mqtt/pingreq.py` & `moat-mqtt-0.39.4/moat/mqtt/mqtt/pingreq.py`

 * *Files identical despite different names*

### Comparing `moat-mqtt-0.38.2/moat/mqtt/mqtt/pingresp.py` & `moat-mqtt-0.39.4/moat/mqtt/mqtt/pingresp.py`

 * *Files identical despite different names*

### Comparing `moat-mqtt-0.38.2/moat/mqtt/mqtt/protocol/broker_handler.py` & `moat-mqtt-0.39.4/moat/mqtt/mqtt/protocol/broker_handler.py`

 * *Files identical despite different names*

### Comparing `moat-mqtt-0.38.2/moat/mqtt/mqtt/protocol/client_handler.py` & `moat-mqtt-0.39.4/moat/mqtt/mqtt/protocol/client_handler.py`

 * *Files identical despite different names*

### Comparing `moat-mqtt-0.38.2/moat/mqtt/mqtt/protocol/handler.py` & `moat-mqtt-0.39.4/moat/mqtt/mqtt/protocol/handler.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,16 +51,20 @@
 from ..suback import SubackPacket
 from ..subscribe import SubscribePacket
 from ..unsuback import UnsubackPacket
 from ..unsubscribe import UnsubscribePacket
 
 try:
     ClosedResourceError = anyio.exceptions.ClosedResourceError
+    BrokenResourceError = anyio.exceptions.BrokenResourceError
+    EndOfStream = anyio.exceptions.EndOfStream
 except AttributeError:
     ClosedResourceError = anyio.ClosedResourceError
+    BrokenResourceError = anyio.BrokenResourceError
+    EndOfStream = anyio.EndOfStream
 
 EVENT_MQTT_PACKET_SENT = "mqtt_packet_sent"
 EVENT_MQTT_PACKET_RECEIVED = "mqtt_packet_received"
 
 PACKET_TYPES = {
     CONNACK: ("connack", False),
     SUBSCRIBE: ("subscribe", True),
@@ -150,18 +154,21 @@
         self.logger.debug("Handler tasks started")
         await self._retry_deliveries()
         self.logger.debug(
             "%s %s ready",
             "Broker" if "Broker" in type(self).__name__ else "Client",
             self.session.client_id if self.session else "?",
         )
-        await anyio.sleep(0.01)
         if self._reader_task is None:
             return
-        self._reader_task.start_soon(self._timeout_loop)
+        try:
+            self._reader_task.start_soon(self._timeout_loop)
+        except RuntimeError:
+            # This can happen when stuff overlaps
+            pass
 
     async def stop(self):
         # Stop messages flow waiter
         self.logger.debug(
             "%s %s stopping",
             "Broker" if "Broker" in type(self).__name__ else "Client",
             self.session.client_id if self.session else "?",
@@ -242,22 +249,15 @@
         :param data:  data to send on topic
         :param qos: quality of service to use for message flow. Can be QOS_0, QOS_1 or QOS_2
         :param retain: retain message flag
         :param ack_timeout: acknowledge timeout. If set, this method will return a TimeOut error if the acknowledgment
         is not completed before ack_timeout second
         :return: ApplicationMessage used during inflight operations
         """
-        if qos in (QOS_1, QOS_2):
-            packet_id = self.session.next_packet_id
-            if packet_id in self.session.inflight_out:
-                raise MoatMQTTException(
-                    "A message with the same packet ID '%d' is already in flight" % packet_id
-                )
-        else:
-            packet_id = None
+        packet_id = self.session.next_packet_id if qos in (QOS_1, QOS_2) else None
 
         message = OutgoingApplicationMessage(packet_id, topic, qos, data, retain)
         await self._handle_message_flow(message)
 
         return message
 
     async def _handle_message_flow(self, app_message):
@@ -506,33 +506,40 @@
                         else:
                             try:
                                 if direct:
                                     await fn(packet)
                                 else:
                                     tg.start_soon(fn, packet)
                             except StopAsyncIteration:
-                                self.logger.debug("%s Read Loop break", self.session.client_id)
                                 break
 
                     except MQTTException:
                         self.logger.debug("Message discarded")
                     except NoDataException:
                         self.logger.debug("%s No data available", self.session.client_id)
                         break  # XXX
+                    except (
+                        anyio.BrokenResourceError,
+                        anyio.ClosedResourceError,
+                        anyio.EndOfStream,
+                    ):
+                        self.logger.debug("%s No data available", self.session.client_id)
+                        break
+
                     except anyio.get_cancelled_exc_class():
-                        self.logger.warning("%s CANCEL", type(self).__name__)
+                        self.logger.debug("%s CANCEL", type(self).__name__)
                         raise
                     except BaseException as e:
                         self.logger.warning(
                             "%s Unhandled exception in reader coro",
                             type(self).__name__,
                             exc_info=e,
                         )
                         raise
-                tg.cancel_scope.cancel()
+                # tg.cancel_scope.cancel()  # XXX is that needed?
         finally:
             with anyio.fail_after(2, shield=True):
                 self.logger.debug(
                     "%s %s coro stopped",
                     "Broker" if "Broker" in type(self).__name__ else "Client",
                     self.session.client_id if self.session else "?",
                 )
@@ -563,15 +570,15 @@
                         await self.handle_write_timeout()
                         continue
                     self.logger.debug(
                         "%s > %r", "B" if "Broker" in type(self).__name__ else "C", packet
                     )
                     try:
                         await packet.to_stream(self.stream)
-                    except ClosedResourceError:
+                    except (ClosedResourceError, BrokenResourceError, EndOfStream):
                         return
                     await self.plugins_manager.fire_event(
                         EVENT_MQTT_PACKET_SENT, packet=packet, session=self.session
                     )
         except ConnectionResetError:
             await self.handle_connection_closed()
         except anyio.get_cancelled_exc_class():
```

### Comparing `moat-mqtt-0.38.2/moat/mqtt/mqtt/puback.py` & `moat-mqtt-0.39.4/moat/mqtt/mqtt/puback.py`

 * *Files identical despite different names*

### Comparing `moat-mqtt-0.38.2/moat/mqtt/mqtt/pubcomp.py` & `moat-mqtt-0.39.4/moat/mqtt/mqtt/pubcomp.py`

 * *Files identical despite different names*

### Comparing `moat-mqtt-0.38.2/moat/mqtt/mqtt/publish.py` & `moat-mqtt-0.39.4/moat/mqtt/mqtt/publish.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 
 from ..codecs import decode_packet_id, decode_string, encode_string, int_to_bytes
 from ..errors import MoatMQTTException, MQTTException
 from .packet import PUBLISH, MQTTFixedHeader, MQTTPacket, MQTTPayload, MQTTVariableHeader
 
 
 class PublishVariableHeader(MQTTVariableHeader):
-
     __slots__ = ("topic_name", "packet_id")
 
     def __init__(self, topic_name: str, packet_id: int = None):
         super().__init__()
         if "*" in topic_name:
             raise MQTTException(
                 "[MQTT-3.3.2-2] Topic name in the PUBLISH Packet MUST NOT contain wildcard characters."
@@ -43,15 +42,14 @@
             packet_id = await decode_packet_id(reader)
         else:
             packet_id = None
         return cls(topic_name, packet_id)
 
 
 class PublishPayload(MQTTPayload):
-
     __slots__ = ("data",)
 
     def __init__(self, data: bytes = None):
         super().__init__()
         self.data = data
 
     def to_bytes(self, fixed_header: MQTTFixedHeader, variable_header: MQTTVariableHeader):
```

### Comparing `moat-mqtt-0.38.2/moat/mqtt/mqtt/pubrec.py` & `moat-mqtt-0.39.4/moat/mqtt/mqtt/pubrec.py`

 * *Files identical despite different names*

### Comparing `moat-mqtt-0.38.2/moat/mqtt/mqtt/pubrel.py` & `moat-mqtt-0.39.4/moat/mqtt/mqtt/pubrel.py`

 * *Files identical despite different names*

### Comparing `moat-mqtt-0.38.2/moat/mqtt/mqtt/suback.py` & `moat-mqtt-0.39.4/moat/mqtt/mqtt/suback.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,15 +12,14 @@
     MQTTPayload,
     MQTTVariableHeader,
     PacketIdVariableHeader,
 )
 
 
 class SubackPayload(MQTTPayload):
-
     __slots__ = ("return_codes",)
 
     RETURN_CODE_00 = 0x00
     RETURN_CODE_01 = 0x01
     RETURN_CODE_02 = 0x02
     RETURN_CODE_80 = 0x80
```

### Comparing `moat-mqtt-0.38.2/moat/mqtt/mqtt/subscribe.py` & `moat-mqtt-0.39.4/moat/mqtt/mqtt/subscribe.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,14 @@
     MQTTPayload,
     MQTTVariableHeader,
     PacketIdVariableHeader,
 )
 
 
 class SubscribePayload(MQTTPayload):
-
     __slots__ = ("topics",)
 
     def __init__(self, topics=()):
         super().__init__()
         self.topics = topics
 
     def to_bytes(self, fixed_header: MQTTFixedHeader, variable_header: MQTTVariableHeader):
```

### Comparing `moat-mqtt-0.38.2/moat/mqtt/mqtt/unsuback.py` & `moat-mqtt-0.39.4/moat/mqtt/mqtt/unsuback.py`

 * *Files identical despite different names*

### Comparing `moat-mqtt-0.38.2/moat/mqtt/mqtt/unsubscribe.py` & `moat-mqtt-0.39.4/moat/mqtt/mqtt/unsubscribe.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,14 @@
     MQTTPayload,
     MQTTVariableHeader,
     PacketIdVariableHeader,
 )
 
 
 class UnubscribePayload(MQTTPayload):
-
     __slots__ = ("topics",)
 
     def __init__(self, topics=()):
         super().__init__()
         self.topics = topics
 
     def to_bytes(self, fixed_header: MQTTFixedHeader, variable_header: MQTTVariableHeader):
```

### Comparing `moat-mqtt-0.38.2/moat/mqtt/plugins/authentication.py` & `moat-mqtt-0.39.4/moat/mqtt/plugins/authentication.py`

 * *Files identical despite different names*

### Comparing `moat-mqtt-0.38.2/moat/mqtt/plugins/logging.py` & `moat-mqtt-0.39.4/moat/mqtt/plugins/logging.py`

 * *Files identical despite different names*

### Comparing `moat-mqtt-0.38.2/moat/mqtt/plugins/manager.py` & `moat-mqtt-0.39.4/moat/mqtt/plugins/manager.py`

 * *Files identical despite different names*

### Comparing `moat-mqtt-0.38.2/moat/mqtt/plugins/persistence.py` & `moat-mqtt-0.39.4/moat/mqtt/plugins/persistence.py`

 * *Files identical despite different names*

### Comparing `moat-mqtt-0.38.2/moat/mqtt/plugins/sys/broker.py` & `moat-mqtt-0.39.4/moat/mqtt/plugins/sys/broker.py`

 * *Files 2% similar despite different names*

```diff
@@ -80,15 +80,15 @@
 
     async def on_broker_pre_stop(self, *args, **kwargs):  # pylint: disable=unused-argument
         # Stop $SYS topics broadcasting
         if self.sys_handle:
             await self.sys_handle.cancel()
 
     async def broadcast_dollar_sys_topics_loop(self, interval, evt):
-        async with anyio.open_cancel_scope() as scope:
+        with anyio.CancelScope() as scope:
             self.sys_handle = scope
             await evt.set()
             while True:
                 await anyio.sleep(interval)
                 await self.broadcast_dollar_sys_topics()
 
     async def broadcast_dollar_sys_topics(self):
```

### Comparing `moat-mqtt-0.38.2/moat/mqtt/plugins/topic_checking.py` & `moat-mqtt-0.39.4/moat/mqtt/plugins/topic_checking.py`

 * *Files identical despite different names*

### Comparing `moat-mqtt-0.38.2/moat/mqtt/session.py` & `moat-mqtt-0.39.4/moat/mqtt/session.py`

 * *Files identical despite different names*

### Comparing `moat-mqtt-0.38.2/moat/mqtt/test.py` & `moat-mqtt-0.39.4/moat/mqtt/test.py`

 * *Files 23% similar despite different names*

```diff
@@ -2,33 +2,38 @@
 This module contains code that helps with DistKV testing.
 """
 import os
 from contextlib import asynccontextmanager
 from functools import partial
 
 import anyio
-from distkv.client import open_client
+from distkv.client import client_scope, open_client
 from distkv.server import Server as _Server
 
 from .broker import create_broker
 
 
 class Server(_Server):
     @asynccontextmanager
-    async def test_client(self):
+    async def test_client(self, name=None):
         """
         An async context manager that returns a client that's connected to
         this server.
         """
-        async with open_client(connect=dict(host="127.0.0.1", port=self.distkv_port)) as client:
-            yield client
+        async with open_client(
+            connect=dict(host="127.0.0.1", port=self.distkv_port, name=name)
+        ) as c:
+            yield c
+
+    async def test_client_scope(self, name=None):
+        return await client_scope(connect=dict(host="127.0.0.1", port=self.distkv_port, name=name))
 
 
 @asynccontextmanager
-async def test_server(mqtt_port: int = None, distkv_port: int = None):
+async def server(mqtt_port: int = None, distkv_port: int = None):
     """
     An async context manager which creates a stand-alone DistKV server.
 
     The server has a `test_client` method: an async context manager that
     returns a client taht's connected to this server.
 
     Ports are allocated based on the current process's PID.
@@ -47,25 +52,25 @@
         "server": {
             "bind_default": {"host": "127.0.0.1", "port": distkv_port},
             "backend": "mqtt",
             "mqtt": {"uri": "mqtt://127.0.0.1:%d/" % mqtt_port},
         }
     }
 
-    server = Server(name="gpio_test", cfg=server_cfg, init="GPIO")
+    s = Server(name="gpio_test", cfg=server_cfg, init="GPIO")
     async with create_broker(config=broker_cfg) as broker:
         evt = anyio.Event()
-        broker._tg.start_soon(partial(server.serve, ready_evt=evt))
+        broker._tg.start_soon(partial(s.serve, ready_evt=evt))
         await evt.wait()
 
-        server.distkv_port = distkv_port  # pylint: disable=attribute-defined-outside-init
-        yield server
+        s.distkv_port = distkv_port  # pylint: disable=attribute-defined-outside-init
+        yield s
 
 
 @asynccontextmanager
-async def test_client(mqtt_port: int = None, distkv_port: int = None):
+async def client(mqtt_port: int = None, distkv_port: int = None):
     """
     An async context manager which creates a stand-alone DistKV client.
     """
-    async with test_server(mqtt_port=mqtt_port, distkv_port=distkv_port) as s:
+    async with server(mqtt_port=mqtt_port, distkv_port=distkv_port) as s:
         async with s.test_client() as c:
             yield c
```

### Comparing `moat-mqtt-0.38.2/moat/mqtt/utils.py` & `moat-mqtt-0.39.4/moat/mqtt/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 # Copyright (c) 2015 Nicolas JOUANIN
 #
 # See the file license.txt for copying permission.
 import logging
 
 import anyio
 import attr
-import yaml
 
 from .errors import InvalidStateError
 
 logger = logging.getLogger(__name__)
 
 
 def format_client_message(session=None, address=None, port=None):
@@ -31,24 +30,14 @@
     gen_id = "moat-mqtt-"
 
     for _ in range(16):
         gen_id += chr(random.randint(0, 26) + 97)
     return gen_id
 
 
-def read_yaml_config(config_file):
-    config = None
-    try:
-        with open(config_file, "r") as stream:  # pylint: disable=unspecified-encoding
-            config = yaml.safe_load(stream)
-    except yaml.YAMLError as exc:
-        logger.error("Invalid config_file %s: %r", config_file, exc)
-    return config
-
-
 # utility code
 
 
 class CancelledError(RuntimeError):
     # This intentionally does not descend from any toolkit's cancellation exception
     # (much less from all of them)
     pass
```

### Comparing `moat-mqtt-0.38.2/moat-mqtt.cfg.sample` & `moat-mqtt-0.39.4/moat-mqtt.cfg.sample`

 * *Files identical despite different names*

### Comparing `moat-mqtt-0.38.2/moat_mqtt.egg-info/PKG-INFO` & `moat-mqtt-0.39.4/moat_mqtt.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moat-mqtt
-Version: 0.38.2
+Version: 0.39.4
 Summary: Async MQTT broker and client, with optional MoaT-KV support
 Author-email: Matthias Urlichs <matthias@urlichs.de>
 Project-URL: homepage, https://m-o-a-t.org
 Project-URL: repository, https://github.com/M-o-a-T/moat-mqtt
 Keywords: MoaT
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `moat-mqtt-0.38.2/moat_mqtt.egg-info/SOURCES.txt` & `moat-mqtt-0.39.4/moat_mqtt.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 .pylintrc
 .travis.yml
 MANIFEST.in
 Makefile
 license.txt
 moat-mqtt.cfg.sample
 moat-mqtt.service
-mq
 pyproject.toml
 readme.rst
 tox.ini
 docs/Makefile
 docs/changelog.rst
 docs/conf.py
 docs/index.rst
@@ -21,14 +20,15 @@
 docs/references/broker.rst
 docs/references/common.rst
 docs/references/distmqtt.rst
 docs/references/distmqtt_pub.rst
 docs/references/distmqtt_sub.rst
 docs/references/index.rst
 docs/references/mqttclient.rst
+moat/__init__.py
 moat/mqtt/__init__.py
 moat/mqtt/_config.yaml
 moat/mqtt/_main.py
 moat/mqtt/adapters.py
 moat/mqtt/broker.py
 moat/mqtt/client.py
 moat/mqtt/codecs.py
```

### Comparing `moat-mqtt-0.38.2/pyproject.toml` & `moat-mqtt-0.39.4/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -19,18 +19,18 @@
 	"transitions",
 	"asyncwebsockets >= 0.9.2",
 	"passlib",
 	"pyyaml",
 	"attrs >= 19",
 	"simplejson",
 	"msgpack",
-	"moat-util",
+	"moat-util ~= 0.35.0",
 	"transitions",
 	"wsproto",
-	"asyncscope",
+	"asyncscope >= 0.6.0",
 	]
 dynamic = [ "version",]
 keywords = [ "MoaT",]
 requires-python = ">=3.8"
 name = "moat-mqtt"
 description = "Async MQTT broker and client, with optional MoaT-KV support"
 readme = "README.rst"
@@ -52,47 +52,53 @@
 [tool.isort]
 line_length = 99
 multi_line_output = 3
 profile = "black"
 
 [tool.setuptools]
 packages = [ "moat.mqtt",]
+[tool.setuptools.package-data]
+"*" = ["*.yaml"]
 
 [tool.setuptools_scm]
 
 [tool.black]
 line-length = 99
 
 [tool.tox]
 legacy_tox_ini = """
 [tox]
 isolated_build = True
-envlist = py310,py39,check
+envlist = py310,check
 
 [testenv]
 setenv = 
     PYTHONPATH = {env:PYTHONPATH}{:}{toxinidir}
 deps = 
+    anyio
+    asyncwebsockets
+    asyncclick
+    asyncscope
     trio
     pytest
-    pytest-trio
-    distkv
 commands = 
     python3 -mpytest tests/
 
 [testenv:check]
 commands = 
-    pylint moat/mqtt tests
-    flake8p moat/mqtt tests
-    black --check moat/mqtt tests
+    pylint moat tests
+    flake8p moat tests
+    black --check moat tests
 deps = 
     pytest
     pylint
     black
     flake8-pyproject
     flake8
 
 """
 
 [tool.pylint]
 [tool.pylint.messages_control]
 disable = "wrong-import-order,ungrouped-imports,too-many-nested-blocks,use-dict-literal,unspecified-encoding,too-many-statements,too-many-return-statements,too-many-locals,too-many-instance-attributes,too-many-branches,too-many-arguments,too-few-public-methods,superfluous-parens,no-else-return,no-else-continue,invalid-name,fixme"
+
+[tool.moat]
```

### Comparing `moat-mqtt-0.38.2/readme.rst` & `moat-mqtt-0.39.4/readme.rst`

 * *Files identical despite different names*

### Comparing `moat-mqtt-0.38.2/samples/broker_acl.py` & `moat-mqtt-0.39.4/samples/broker_acl.py`

 * *Files identical despite different names*

### Comparing `moat-mqtt-0.38.2/samples/broker_start.py` & `moat-mqtt-0.39.4/samples/broker_start.py`

 * *Files identical despite different names*

### Comparing `moat-mqtt-0.38.2/samples/broker_taboo.py` & `moat-mqtt-0.39.4/samples/broker_taboo.py`

 * *Files identical despite different names*

### Comparing `moat-mqtt-0.38.2/samples/client_keepalive.py` & `moat-mqtt-0.39.4/samples/client_keepalive.py`

 * *Files identical despite different names*

### Comparing `moat-mqtt-0.38.2/samples/client_publish.py` & `moat-mqtt-0.39.4/samples/client_publish.py`

 * *Files identical despite different names*

### Comparing `moat-mqtt-0.38.2/samples/client_publish_acl.py` & `moat-mqtt-0.39.4/samples/client_publish_acl.py`

 * *Files identical despite different names*

### Comparing `moat-mqtt-0.38.2/samples/client_publish_ssl.py` & `moat-mqtt-0.39.4/samples/client_publish_ssl.py`

 * *Files identical despite different names*

### Comparing `moat-mqtt-0.38.2/samples/client_publish_ws.py` & `moat-mqtt-0.39.4/samples/client_publish_ws.py`

 * *Files identical despite different names*

### Comparing `moat-mqtt-0.38.2/samples/client_retained.py` & `moat-mqtt-0.39.4/samples/client_retained.py`

 * *Files identical despite different names*

### Comparing `moat-mqtt-0.38.2/samples/client_subscribe.py` & `moat-mqtt-0.39.4/samples/client_subscribe.py`

 * *Files identical despite different names*

### Comparing `moat-mqtt-0.38.2/samples/client_subscribe_acl.py` & `moat-mqtt-0.39.4/samples/client_subscribe_acl.py`

 * *Files identical despite different names*

### Comparing `moat-mqtt-0.38.2/samples/mosquitto.org.crt` & `moat-mqtt-0.39.4/samples/mosquitto.org.crt`

 * *Files identical despite different names*

### Comparing `moat-mqtt-0.38.2/tests/mosquitto.org.crt` & `moat-mqtt-0.39.4/tests/mosquitto.org.crt`

 * *Files identical despite different names*

### Comparing `moat-mqtt-0.38.2/tests/mqtt/protocol/test_handler.py` & `moat-mqtt-0.39.4/tests/mqtt/protocol/test_handler.py`

 * *Files identical despite different names*

### Comparing `moat-mqtt-0.38.2/tests/mqtt/test_connect.py` & `moat-mqtt-0.39.4/tests/mqtt/test_connect.py`

 * *Files identical despite different names*

### Comparing `moat-mqtt-0.38.2/tests/mqtt/test_packet.py` & `moat-mqtt-0.39.4/tests/mqtt/test_packet.py`

 * *Files identical despite different names*

### Comparing `moat-mqtt-0.38.2/tests/mqtt/test_puback.py` & `moat-mqtt-0.39.4/tests/mqtt/test_puback.py`

 * *Files identical despite different names*

### Comparing `moat-mqtt-0.38.2/tests/mqtt/test_pubcomp.py` & `moat-mqtt-0.39.4/tests/mqtt/test_pubcomp.py`

 * *Files identical despite different names*

### Comparing `moat-mqtt-0.38.2/tests/mqtt/test_publish.py` & `moat-mqtt-0.39.4/tests/mqtt/test_publish.py`

 * *Files identical despite different names*

### Comparing `moat-mqtt-0.38.2/tests/mqtt/test_pubrec.py` & `moat-mqtt-0.39.4/tests/mqtt/test_pubrec.py`

 * *Files identical despite different names*

### Comparing `moat-mqtt-0.38.2/tests/mqtt/test_pubrel.py` & `moat-mqtt-0.39.4/tests/mqtt/test_pubrel.py`

 * *Files identical despite different names*

### Comparing `moat-mqtt-0.38.2/tests/mqtt/test_suback.py` & `moat-mqtt-0.39.4/tests/mqtt/test_suback.py`

 * *Files identical despite different names*

### Comparing `moat-mqtt-0.38.2/tests/mqtt/test_subscribe.py` & `moat-mqtt-0.39.4/tests/mqtt/test_subscribe.py`

 * *Files identical despite different names*

### Comparing `moat-mqtt-0.38.2/tests/mqtt/test_unsuback.py` & `moat-mqtt-0.39.4/tests/mqtt/test_unsuback.py`

 * *Files identical despite different names*

### Comparing `moat-mqtt-0.38.2/tests/mqtt/test_unsubscribe.py` & `moat-mqtt-0.39.4/tests/mqtt/test_unsubscribe.py`

 * *Files identical despite different names*

### Comparing `moat-mqtt-0.38.2/tests/plugins/test_authentication.py` & `moat-mqtt-0.39.4/tests/plugins/test_authentication.py`

 * *Files identical despite different names*

### Comparing `moat-mqtt-0.38.2/tests/plugins/test_manager.py` & `moat-mqtt-0.39.4/tests/plugins/test_manager.py`

 * *Files identical despite different names*

### Comparing `moat-mqtt-0.38.2/tests/plugins/test_persistence.py` & `moat-mqtt-0.39.4/tests/plugins/test_persistence.py`

 * *Files identical despite different names*

### Comparing `moat-mqtt-0.38.2/tests/test_broker.py` & `moat-mqtt-0.39.4/tests/test_broker.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 )
 from moat.mqtt.mqtt.connect import ConnectPayload, ConnectVariableHeader
 from moat.mqtt.mqtt.constants import QOS_0, QOS_1, QOS_2
 
 from . import anyio_run
 
 formatter = "%(asctime)s %(name)s:%(lineno)d %(levelname)s - %(message)s"
-logging.basicConfig(level=logging.INFO, format=formatter)
+logging.basicConfig(level=logging.DEBUG, format=formatter)
 log = logging.getLogger(__name__)
 
 PORT = 40000 + (os.getpid() + 3) % 10000
 URL = "mqtt://127.0.0.1:%d/" % PORT
 
 test_config = {
     "listeners": {
@@ -87,42 +87,29 @@
                 any_order=True,
             )
             self.assertTrue(broker.transitions.is_stopped())
 
         anyio_run(test_coro, backend="trio")
 
     @patch("moat.mqtt.broker.PluginManager", new_callable=AsyncMock)
-    def test_client_connect(self, MockPluginManager):
+    def test_client_connect(self, MockPluginManager):  # pylint: disable=unused-argument
         async def test_coro():
             async with create_broker(
                 test_config, plugin_namespace="moat.mqtt.test.plugins"
             ) as broker:
                 broker.plugins_manager._tg = broker._tg
                 self.assertTrue(broker.transitions.is_started())
                 async with open_mqttclient() as client:
                     ret = await client.connect(URL)
                     self.assertEqual(ret, 0)
                     self.assertEqual(len(broker._sessions), 1)
                     self.assertIn(client.session.client_id, broker._sessions)
                 await anyio.sleep(0.1)  # let the broker task process the packet
             self.assertTrue(broker.transitions.is_stopped())
             self.assertDictEqual(broker._sessions, {})
-            MockPluginManager.assert_has_calls(
-                [
-                    call().fire_event(
-                        EVENT_BROKER_CLIENT_CONNECTED,
-                        client_id=client.session.client_id,
-                    ),
-                    call().fire_event(
-                        EVENT_BROKER_CLIENT_DISCONNECTED,
-                        client_id=client.session.client_id,
-                    ),
-                ],
-                any_order=True,
-            )
 
         anyio_run(test_coro)
 
     @patch("moat.mqtt.broker.PluginManager", new_callable=AsyncMock)
     def test_client_connect_will_flag(self, MockPluginManager):  # pylint: disable=unused-argument
         async def test_coro():
             async with create_broker(
@@ -576,36 +563,38 @@
     def test_client_publish_retain_subscribe(
         self, MockPluginManager
     ):  # pylint: disable=unused-argument
         async def test_coro():
             async with create_broker(
                 test_config, plugin_namespace="moat.mqtt.test.plugins"
             ) as broker:
-                broker.plugins_manager._tg = broker._tg
-                self.assertTrue(broker.transitions.is_started())
-                async with open_mqttclient() as sub_client:
-                    await sub_client.connect(URL, cleansession=False)
-                    ret = await sub_client.subscribe(
-                        [("/qos0", QOS_0), ("/qos1", QOS_1), ("/qos2", QOS_2)]
-                    )
-                    self.assertEqual(ret, [QOS_0, QOS_1, QOS_2])
-                    await sub_client.disconnect()
-
-                    await self._client_publish("/qos0", b"data", QOS_0, retain=True)
-                    await self._client_publish("/qos1", b"data", QOS_1, retain=True)
-                    await self._client_publish("/qos2", b"data", QOS_2, retain=True)
-                    await sub_client.reconnect()
-                    for qos in [QOS_0, QOS_1, QOS_2]:
-                        log.debug("TEST QOS: %d", qos)
-                        message = await sub_client.deliver_message()
-                        log.debug("Message: %r", message.publish_packet)
-                        self.assertIsNotNone(message)
-                        self.assertEqual(message.topic, "/qos%s" % qos)
-                        self.assertEqual(message.data, b"data")
-                        self.assertEqual(message.qos, qos)
+                with anyio.fail_after(3):
+                    broker.plugins_manager._tg = broker._tg
+                    self.assertTrue(broker.transitions.is_started())
+                    async with open_mqttclient() as sub_client:
+                        await sub_client.connect(URL, cleansession=False)
+                        ret = await sub_client.subscribe(
+                            [("/qos0", QOS_0), ("/qos1", QOS_1), ("/qos2", QOS_2)]
+                        )
+                        self.assertEqual(ret, [QOS_0, QOS_1, QOS_2])
+                        await sub_client.disconnect()
+
+                        await self._client_publish("/qos0", b"data", QOS_0, retain=True)
+                        await self._client_publish("/qos1", b"data", QOS_1, retain=True)
+                        await self._client_publish("/qos2", b"data", QOS_2, retain=True)
+                        await sub_client.reconnect()
+                        seen = set()
+                        for qos in [QOS_1, QOS_2]:
+                            log.error("TEST QOS: %d", qos)
+                            message = await sub_client.deliver_message()
+                            log.error("Message: %r", message.publish_packet)
+                            assert message.topic == f"/qos{qos}"
+                            assert message.data == b"data"
+                            seen.add(qos)
+                        assert seen == set((1, 2))
             self.assertTrue(broker.transitions.is_stopped())
 
         anyio_run(test_coro)
 
     async def _client_publish(self, topic, data, qos, retain=False):
         async with open_mqttclient() as pub_client:
             ret = await pub_client.connect(URL)
```

### Comparing `moat-mqtt-0.38.2/tests/test_client.py` & `moat-mqtt-0.39.4/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `moat-mqtt-0.38.2/tests/test_client_distkv.py` & `moat-mqtt-0.39.4/tests/test_client_distkv.py`

 * *Files identical despite different names*

### Comparing `moat-mqtt-0.38.2/tests/test_codecs.py` & `moat-mqtt-0.39.4/tests/test_codecs.py`

 * *Files identical despite different names*

### Comparing `moat-mqtt-0.38.2/tox.ini` & `moat-mqtt-0.39.4/tox.ini`

 * *Files identical despite different names*

