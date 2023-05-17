# Comparing `tmp/mqttwarn-0.34.0.tar.gz` & `tmp/mqttwarn-0.34.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mqttwarn-0.34.0.tar", last modified: Thu Apr 27 23:09:39 2023, max compression
+gzip compressed data, was "mqttwarn-0.34.1.tar", last modified: Wed May 17 23:13:24 2023, max compression
```

## Comparing `mqttwarn-0.34.0.tar` & `mqttwarn-0.34.1.tar`

### file list

```diff
@@ -1,115 +1,236 @@
-drwxr-xr-x   0 amo        (501) staff       (20)        0 2023-04-27 23:09:39.859610 mqttwarn-0.34.0/
--rw-r--r--   0 amo        (501) staff       (20)    14685 2023-04-27 23:02:20.000000 mqttwarn-0.34.0/CHANGES.rst
--rw-r--r--   0 amo        (501) staff       (20)    14197 2021-06-02 19:14:19.000000 mqttwarn-0.34.0/LICENSE
--rw-r--r--   0 amo        (501) staff       (20)      154 2023-03-12 10:52:16.000000 mqttwarn-0.34.0/MANIFEST.in
--rw-r--r--   0 amo        (501) staff       (20)    13136 2023-04-27 23:09:39.859302 mqttwarn-0.34.0/PKG-INFO
--rw-r--r--   0 amo        (501) staff       (20)    10150 2023-04-27 23:07:43.000000 mqttwarn-0.34.0/README.rst
-drwxr-xr-x   0 amo        (501) staff       (20)        0 2023-04-27 23:09:39.816368 mqttwarn-0.34.0/mqttwarn/
--rw-r--r--   0 amo        (501) staff       (20)      462 2023-03-12 10:52:16.000000 mqttwarn-0.34.0/mqttwarn/__init__.py
--rw-r--r--   0 amo        (501) staff       (20)       50 2023-03-12 10:52:16.000000 mqttwarn-0.34.0/mqttwarn/__main__.py
--rw-r--r--   0 amo        (501) staff       (20)     5906 2023-04-27 23:01:45.000000 mqttwarn-0.34.0/mqttwarn/commands.py
--rw-r--r--   0 amo        (501) staff       (20)     6341 2023-04-27 20:56:31.000000 mqttwarn-0.34.0/mqttwarn/configuration.py
--rw-r--r--   0 amo        (501) staff       (20)     8249 2023-04-27 20:56:31.000000 mqttwarn-0.34.0/mqttwarn/context.py
--rw-r--r--   0 amo        (501) staff       (20)    30225 2023-04-27 20:56:31.000000 mqttwarn-0.34.0/mqttwarn/core.py
--rw-r--r--   0 amo        (501) staff       (20)     2539 2023-04-27 20:56:31.000000 mqttwarn-0.34.0/mqttwarn/cron.py
-drwxr-xr-x   0 amo        (501) staff       (20)        0 2023-04-27 23:09:39.821459 mqttwarn-0.34.0/mqttwarn/examples/
--rw-r--r--   0 amo        (501) staff       (20)        0 2021-06-02 19:14:19.000000 mqttwarn-0.34.0/mqttwarn/examples/__init__.py
-drwxr-xr-x   0 amo        (501) staff       (20)        0 2023-04-27 23:09:39.822592 mqttwarn-0.34.0/mqttwarn/examples/basic/
--rwxr-xr-x   0 amo        (501) staff       (20)     3832 2023-04-18 22:55:29.000000 mqttwarn-0.34.0/mqttwarn/examples/basic/mqttwarn.ini
--rwxr-xr-x   0 amo        (501) staff       (20)     3060 2023-04-27 20:56:31.000000 mqttwarn-0.34.0/mqttwarn/examples/basic/udf.py
--rw-r--r--   0 amo        (501) staff       (20)     3733 2023-04-27 20:56:31.000000 mqttwarn-0.34.0/mqttwarn/model.py
-drwxr-xr-x   0 amo        (501) staff       (20)        0 2023-04-27 23:09:39.857833 mqttwarn-0.34.0/mqttwarn/services/
--rw-r--r--   0 amo        (501) staff       (20)        0 2021-06-02 19:14:19.000000 mqttwarn-0.34.0/mqttwarn/services/__init__.py
--rw-r--r--   0 amo        (501) staff       (20)     1317 2023-03-12 10:52:16.000000 mqttwarn-0.34.0/mqttwarn/services/alexa-notify-me.py
--rw-r--r--   0 amo        (501) staff       (20)     1322 2023-03-12 10:52:16.000000 mqttwarn-0.34.0/mqttwarn/services/amqp.py
--rw-r--r--   0 amo        (501) staff       (20)     1310 2023-04-27 20:56:31.000000 mqttwarn-0.34.0/mqttwarn/services/apns.py
--rw-r--r--   0 amo        (501) staff       (20)      316 2023-03-12 10:52:16.000000 mqttwarn-0.34.0/mqttwarn/services/apprise.py
--rw-r--r--   0 amo        (501) staff       (20)     2639 2023-04-26 22:18:29.000000 mqttwarn-0.34.0/mqttwarn/services/apprise_multi.py
--rw-r--r--   0 amo        (501) staff       (20)     2448 2023-04-26 22:18:29.000000 mqttwarn-0.34.0/mqttwarn/services/apprise_single.py
--rw-r--r--   0 amo        (501) staff       (20)     1392 2023-04-26 22:18:29.000000 mqttwarn-0.34.0/mqttwarn/services/apprise_util.py
--rw-r--r--   0 amo        (501) staff       (20)     1916 2023-03-12 10:52:16.000000 mqttwarn-0.34.0/mqttwarn/services/asterisk.py
--rw-r--r--   0 amo        (501) staff       (20)     1463 2023-03-12 10:52:16.000000 mqttwarn-0.34.0/mqttwarn/services/autoremote.py
--rw-r--r--   0 amo        (501) staff       (20)     2331 2023-03-12 10:52:16.000000 mqttwarn-0.34.0/mqttwarn/services/azure_iot.py
--rw-r--r--   0 amo        (501) staff       (20)     2114 2023-03-12 10:52:16.000000 mqttwarn-0.34.0/mqttwarn/services/carbon.py
--rw-r--r--   0 amo        (501) staff       (20)      862 2021-06-02 19:14:19.000000 mqttwarn-0.34.0/mqttwarn/services/celery.py
--rw-r--r--   0 amo        (501) staff       (20)     2160 2023-03-12 10:52:16.000000 mqttwarn-0.34.0/mqttwarn/services/chromecast.py
--rw-r--r--   0 amo        (501) staff       (20)     1369 2021-06-02 19:14:19.000000 mqttwarn-0.34.0/mqttwarn/services/dbus.py
--rw-r--r--   0 amo        (501) staff       (20)     1604 2023-04-27 20:56:31.000000 mqttwarn-0.34.0/mqttwarn/services/desktopnotify.py
--rw-r--r--   0 amo        (501) staff       (20)     1580 2021-06-02 19:14:19.000000 mqttwarn-0.34.0/mqttwarn/services/dnsupdate.py
--rw-r--r--   0 amo        (501) staff       (20)     1371 2023-04-27 20:56:31.000000 mqttwarn-0.34.0/mqttwarn/services/emoncms.py
--rw-r--r--   0 amo        (501) staff       (20)      886 2023-03-12 10:52:16.000000 mqttwarn-0.34.0/mqttwarn/services/execute.py
--rw-r--r--   0 amo        (501) staff       (20)     1084 2021-06-02 19:14:19.000000 mqttwarn-0.34.0/mqttwarn/services/fbchat.py
--rw-r--r--   0 amo        (501) staff       (20)     2242 2023-04-18 22:40:03.000000 mqttwarn-0.34.0/mqttwarn/services/file.py
--rw-r--r--   0 amo        (501) staff       (20)     2609 2021-06-02 19:14:19.000000 mqttwarn-0.34.0/mqttwarn/services/freeswitch.py
--rw-r--r--   0 amo        (501) staff       (20)     1477 2023-04-27 20:56:31.000000 mqttwarn-0.34.0/mqttwarn/services/gss.py
--rw-r--r--   0 amo        (501) staff       (20)     4586 2023-04-27 20:56:31.000000 mqttwarn-0.34.0/mqttwarn/services/gss2.py
--rw-r--r--   0 amo        (501) staff       (20)     1414 2023-03-12 10:52:16.000000 mqttwarn-0.34.0/mqttwarn/services/hangbot.py
--rw-r--r--   0 amo        (501) staff       (20)     1614 2023-04-27 20:56:31.000000 mqttwarn-0.34.0/mqttwarn/services/hipchat.py
--rw-r--r--   0 amo        (501) staff       (20)     4229 2023-04-27 20:56:31.000000 mqttwarn-0.34.0/mqttwarn/services/http_urllib.py
--rw-r--r--   0 amo        (501) staff       (20)     2263 2023-04-27 20:56:31.000000 mqttwarn-0.34.0/mqttwarn/services/icinga2.py
--rw-r--r--   0 amo        (501) staff       (20)     1084 2021-06-02 19:14:19.000000 mqttwarn-0.34.0/mqttwarn/services/ifttt.py
--rw-r--r--   0 amo        (501) staff       (20)     3671 2023-03-12 10:52:16.000000 mqttwarn-0.34.0/mqttwarn/services/influxdb.py
--rw-r--r--   0 amo        (501) staff       (20)     2615 2023-04-27 20:56:31.000000 mqttwarn-0.34.0/mqttwarn/services/ionic.py
--rw-r--r--   0 amo        (501) staff       (20)     1311 2023-03-12 10:52:16.000000 mqttwarn-0.34.0/mqttwarn/services/irccat.py
--rw-r--r--   0 amo        (501) staff       (20)     1022 2021-06-02 19:14:19.000000 mqttwarn-0.34.0/mqttwarn/services/linuxnotify.py
--rw-r--r--   0 amo        (501) staff       (20)      881 2023-03-12 10:52:16.000000 mqttwarn-0.34.0/mqttwarn/services/log.py
--rw-r--r--   0 amo        (501) staff       (20)     2491 2023-04-27 20:56:31.000000 mqttwarn-0.34.0/mqttwarn/services/mattermost.py
--rw-r--r--   0 amo        (501) staff       (20)     3468 2021-06-19 14:00:07.000000 mqttwarn-0.34.0/mqttwarn/services/mqtt.py
--rw-r--r--   0 amo        (501) staff       (20)     2337 2023-03-12 10:52:16.000000 mqttwarn-0.34.0/mqttwarn/services/mqtt_filter.py
--rw-r--r--   0 amo        (501) staff       (20)     1340 2023-03-12 10:52:16.000000 mqttwarn-0.34.0/mqttwarn/services/mqttpub.py
--rw-r--r--   0 amo        (501) staff       (20)     3064 2023-03-12 10:52:16.000000 mqttwarn-0.34.0/mqttwarn/services/mysql.py
--rw-r--r--   0 amo        (501) staff       (20)     4557 2023-03-12 10:52:16.000000 mqttwarn-0.34.0/mqttwarn/services/mysql_dynamic.py
--rw-r--r--   0 amo        (501) staff       (20)     3075 2023-03-12 10:52:16.000000 mqttwarn-0.34.0/mqttwarn/services/mysql_remap.py
--rw-r--r--   0 amo        (501) staff       (20)     1387 2021-06-02 19:14:19.000000 mqttwarn-0.34.0/mqttwarn/services/mythtv.py
--rw-r--r--   0 amo        (501) staff       (20)     1610 2021-06-02 19:14:19.000000 mqttwarn-0.34.0/mqttwarn/services/nntp.py
--rw-r--r--   0 amo        (501) staff       (20)     1135 2023-03-12 10:52:16.000000 mqttwarn-0.34.0/mqttwarn/services/nsca.py
--rw-r--r--   0 amo        (501) staff       (20)    10095 2023-04-27 20:12:45.000000 mqttwarn-0.34.0/mqttwarn/services/ntfy.py
--rw-r--r--   0 amo        (501) staff       (20)     1040 2021-06-02 19:14:19.000000 mqttwarn-0.34.0/mqttwarn/services/osxsay.py
--rw-r--r--   0 amo        (501) staff       (20)     1587 2021-06-19 14:00:07.000000 mqttwarn-0.34.0/mqttwarn/services/pastebinpub.py
--rw-r--r--   0 amo        (501) staff       (20)     1092 2023-03-12 10:52:16.000000 mqttwarn-0.34.0/mqttwarn/services/pipe.py
--rw-r--r--   0 amo        (501) staff       (20)     3360 2023-03-12 10:52:16.000000 mqttwarn-0.34.0/mqttwarn/services/postgres.py
--rw-r--r--   0 amo        (501) staff       (20)     1164 2023-03-12 10:52:16.000000 mqttwarn-0.34.0/mqttwarn/services/prowl.py
--rw-r--r--   0 amo        (501) staff       (20)     1318 2021-06-02 19:14:19.000000 mqttwarn-0.34.0/mqttwarn/services/pushalot.py
--rw-r--r--   0 amo        (501) staff       (20)     1204 2021-06-02 19:14:19.000000 mqttwarn-0.34.0/mqttwarn/services/pushbullet.py
--rw-r--r--   0 amo        (501) staff       (20)     5676 2023-03-12 10:52:16.000000 mqttwarn-0.34.0/mqttwarn/services/pushover.py
--rw-r--r--   0 amo        (501) staff       (20)     8091 2023-04-11 20:10:09.000000 mqttwarn-0.34.0/mqttwarn/services/pushsafer.py
--rw-r--r--   0 amo        (501) staff       (20)      955 2021-06-02 19:14:19.000000 mqttwarn-0.34.0/mqttwarn/services/redispub.py
--rw-r--r--   0 amo        (501) staff       (20)     1189 2021-06-02 19:14:19.000000 mqttwarn-0.34.0/mqttwarn/services/rrdtool.py
--rw-r--r--   0 amo        (501) staff       (20)     2202 2023-03-12 10:52:16.000000 mqttwarn-0.34.0/mqttwarn/services/serial.py
--rw-r--r--   0 amo        (501) staff       (20)     3480 2023-03-12 10:52:16.000000 mqttwarn-0.34.0/mqttwarn/services/slack.py
--rw-r--r--   0 amo        (501) staff       (20)     1910 2023-03-12 10:52:16.000000 mqttwarn-0.34.0/mqttwarn/services/slixmpp.py
--rw-r--r--   0 amo        (501) staff       (20)     2156 2023-03-12 10:52:16.000000 mqttwarn-0.34.0/mqttwarn/services/smtp.py
--rw-r--r--   0 amo        (501) staff       (20)     1157 2021-06-02 19:14:19.000000 mqttwarn-0.34.0/mqttwarn/services/sqlite.py
--rw-r--r--   0 amo        (501) staff       (20)     3024 2021-06-19 14:00:07.000000 mqttwarn-0.34.0/mqttwarn/services/sqlite_json2cols.py
--rw-r--r--   0 amo        (501) staff       (20)     1317 2021-06-02 19:14:19.000000 mqttwarn-0.34.0/mqttwarn/services/sqlite_timestamp.py
--rw-r--r--   0 amo        (501) staff       (20)     2116 2023-03-12 10:52:16.000000 mqttwarn-0.34.0/mqttwarn/services/ssh.py
--rw-r--r--   0 amo        (501) staff       (20)     2329 2021-06-02 19:14:19.000000 mqttwarn-0.34.0/mqttwarn/services/syslog.py
--rw-r--r--   0 amo        (501) staff       (20)     4471 2023-04-27 20:56:31.000000 mqttwarn-0.34.0/mqttwarn/services/telegram.py
--rw-r--r--   0 amo        (501) staff       (20)     2881 2021-06-19 14:00:07.000000 mqttwarn-0.34.0/mqttwarn/services/thingspeak.py
--rw-r--r--   0 amo        (501) staff       (20)     1780 2021-06-07 22:34:47.000000 mqttwarn-0.34.0/mqttwarn/services/tootpaste.py
--rw-r--r--   0 amo        (501) staff       (20)     1050 2021-06-02 19:14:19.000000 mqttwarn-0.34.0/mqttwarn/services/twilio.py
--rw-r--r--   0 amo        (501) staff       (20)     1070 2021-06-02 19:14:19.000000 mqttwarn-0.34.0/mqttwarn/services/twitter.py
--rw-r--r--   0 amo        (501) staff       (20)     1210 2023-03-12 10:52:16.000000 mqttwarn-0.34.0/mqttwarn/services/websocket.py
--rw-r--r--   0 amo        (501) staff       (20)     2168 2023-04-27 20:56:31.000000 mqttwarn-0.34.0/mqttwarn/services/xbmc.py
--rw-r--r--   0 amo        (501) staff       (20)     1209 2021-06-19 14:00:07.000000 mqttwarn-0.34.0/mqttwarn/services/xively.py
--rw-r--r--   0 amo        (501) staff       (20)     2457 2021-06-02 19:14:19.000000 mqttwarn-0.34.0/mqttwarn/services/xmpp.py
--rw-r--r--   0 amo        (501) staff       (20)     3265 2023-04-27 20:56:31.000000 mqttwarn-0.34.0/mqttwarn/services/zabbix.py
-drwxr-xr-x   0 amo        (501) staff       (20)        0 2023-04-27 23:09:39.858347 mqttwarn-0.34.0/mqttwarn/testing/
--rw-r--r--   0 amo        (501) staff       (20)        0 2023-03-12 10:52:16.000000 mqttwarn-0.34.0/mqttwarn/testing/__init__.py
--rw-r--r--   0 amo        (501) staff       (20)      375 2023-03-12 10:52:16.000000 mqttwarn-0.34.0/mqttwarn/testing/fixtures.py
--rw-r--r--   0 amo        (501) staff       (20)     6929 2023-04-27 20:56:31.000000 mqttwarn-0.34.0/mqttwarn/util.py
-drwxr-xr-x   0 amo        (501) staff       (20)        0 2023-04-27 23:09:39.858968 mqttwarn-0.34.0/mqttwarn/vendor/
--rw-r--r--   0 amo        (501) staff       (20)     2320 2023-04-27 20:56:31.000000 mqttwarn-0.34.0/mqttwarn/vendor/ZabbixSender.py
--rw-r--r--   0 amo        (501) staff       (20)        0 2023-03-12 10:52:16.000000 mqttwarn-0.34.0/mqttwarn/vendor/__init__.py
-drwxr-xr-x   0 amo        (501) staff       (20)        0 2023-04-27 23:09:39.821048 mqttwarn-0.34.0/mqttwarn.egg-info/
--rw-r--r--   0 amo        (501) staff       (20)    13136 2023-04-27 23:09:39.000000 mqttwarn-0.34.0/mqttwarn.egg-info/PKG-INFO
--rw-r--r--   0 amo        (501) staff       (20)     2924 2023-04-27 23:09:39.000000 mqttwarn-0.34.0/mqttwarn.egg-info/SOURCES.txt
--rw-r--r--   0 amo        (501) staff       (20)        1 2023-04-27 23:09:39.000000 mqttwarn-0.34.0/mqttwarn.egg-info/dependency_links.txt
--rw-r--r--   0 amo        (501) staff       (20)       51 2023-04-27 23:09:39.000000 mqttwarn-0.34.0/mqttwarn.egg-info/entry_points.txt
--rw-r--r--   0 amo        (501) staff       (20)        1 2021-06-02 19:17:07.000000 mqttwarn-0.34.0/mqttwarn.egg-info/not-zip-safe
--rw-r--r--   0 amo        (501) staff       (20)     2300 2023-04-27 23:09:39.000000 mqttwarn-0.34.0/mqttwarn.egg-info/requires.txt
--rw-r--r--   0 amo        (501) staff       (20)       24 2023-04-27 23:09:39.000000 mqttwarn-0.34.0/mqttwarn.egg-info/top_level.txt
--rw-r--r--   0 amo        (501) staff       (20)     2257 2023-04-27 20:56:31.000000 mqttwarn-0.34.0/pyproject.toml
--rw-r--r--   0 amo        (501) staff       (20)       14 2023-03-12 10:52:16.000000 mqttwarn-0.34.0/requirements-release.txt
--rw-r--r--   0 amo        (501) staff       (20)       38 2023-04-27 23:09:39.859691 mqttwarn-0.34.0/setup.cfg
--rw-r--r--   0 amo        (501) staff       (20)     6239 2023-04-27 20:56:31.000000 mqttwarn-0.34.0/setup.py
+drwxr-xr-x   0 amo        (501) staff       (20)        0 2023-05-17 23:13:24.545090 mqttwarn-0.34.1/
+-rw-r--r--   0 amo        (501) staff       (20)    15169 2023-05-17 22:54:38.000000 mqttwarn-0.34.1/CHANGES.rst
+-rw-r--r--   0 amo        (501) staff       (20)        3 2023-05-08 23:39:59.000000 mqttwarn-0.34.1/HelloWorld.txt
+-rw-r--r--   0 amo        (501) staff       (20)    14197 2021-06-02 19:14:19.000000 mqttwarn-0.34.1/LICENSE
+-rw-r--r--   0 amo        (501) staff       (20)      266 2023-05-07 17:07:28.000000 mqttwarn-0.34.1/MANIFEST.in
+-rw-r--r--   0 amo        (501) staff       (20)    11492 2023-05-17 23:13:24.544742 mqttwarn-0.34.1/PKG-INFO
+-rw-r--r--   0 amo        (501) staff       (20)     8535 2023-05-07 17:07:28.000000 mqttwarn-0.34.1/README.rst
+drwxr-xr-x   0 amo        (501) staff       (20)        0 2023-05-17 23:13:24.426381 mqttwarn-0.34.1/docs/
+-rw-r--r--   0 amo        (501) staff       (20)        7 2023-04-18 22:55:29.000000 mqttwarn-0.34.1/docs/.gitignore
+-rw-r--r--   0 amo        (501) staff       (20)      634 2023-04-18 22:55:29.000000 mqttwarn-0.34.1/docs/Makefile
+drwxr-xr-x   0 amo        (501) staff       (20)        0 2023-05-17 23:13:24.443712 mqttwarn-0.34.1/docs/assets/
+-rw-r--r--   0 amo        (501) staff       (20)    59218 2021-06-02 19:14:19.000000 mqttwarn-0.34.1/docs/assets/apns.png
+-rw-r--r--   0 amo        (501) staff       (20)    16884 2023-03-12 10:52:16.000000 mqttwarn-0.34.1/docs/assets/desktopnotify.jpg
+-rw-r--r--   0 amo        (501) staff       (20)    53037 2021-06-02 19:14:19.000000 mqttwarn-0.34.1/docs/assets/google-definition.jpg
+-rw-r--r--   0 amo        (501) staff       (20)    18659 2021-06-02 19:14:19.000000 mqttwarn-0.34.1/docs/assets/gss.png
+-rw-r--r--   0 amo        (501) staff       (20)     9543 2021-06-02 19:14:19.000000 mqttwarn-0.34.1/docs/assets/hipchat.png
+-rw-r--r--   0 amo        (501) staff       (20)    52220 2021-06-02 19:14:19.000000 mqttwarn-0.34.1/docs/assets/icinga.jpg
+-rw-r--r--   0 amo        (501) staff       (20)    14166 2021-06-02 19:14:19.000000 mqttwarn-0.34.1/docs/assets/ionic.png
+-rw-r--r--   0 amo        (501) staff       (20)    81604 2021-06-02 19:14:19.000000 mqttwarn-0.34.1/docs/assets/irccat.png
+-rw-r--r--   0 amo        (501) staff       (20)     6537 2021-06-02 19:14:19.000000 mqttwarn-0.34.1/docs/assets/linuxnotify.png
+drwxr-xr-x   0 amo        (501) staff       (20)        0 2023-05-17 23:13:24.413468 mqttwarn-0.34.1/docs/assets/logo/
+drwxr-xr-x   0 amo        (501) staff       (20)        0 2023-05-17 23:13:24.449664 mqttwarn-0.34.1/docs/assets/logo/img/
+-rw-r--r--   0 amo        (501) staff       (20)     2767 2021-06-02 19:14:19.000000 mqttwarn-0.34.1/docs/assets/logo/img/hz_wordmark_blk_200x75.png
+-rw-r--r--   0 amo        (501) staff       (20)     6981 2021-06-02 19:14:19.000000 mqttwarn-0.34.1/docs/assets/logo/img/hz_wordmark_blk_500x187.png
+-rw-r--r--   0 amo        (501) staff       (20)     3024 2021-06-02 19:14:19.000000 mqttwarn-0.34.1/docs/assets/logo/img/hz_wordmark_wht_200x75.png
+-rw-r--r--   0 amo        (501) staff       (20)     7583 2021-06-02 19:14:19.000000 mqttwarn-0.34.1/docs/assets/logo/img/hz_wordmark_wht_500x187.png
+-rw-r--r--   0 amo        (501) staff       (20)     8194 2021-06-02 19:14:19.000000 mqttwarn-0.34.1/docs/assets/logo/img/markonly_200x200.png
+-rw-r--r--   0 amo        (501) staff       (20)    22282 2021-06-02 19:14:19.000000 mqttwarn-0.34.1/docs/assets/logo/img/markonly_500x500.png
+-rw-r--r--   0 amo        (501) staff       (20)    11722 2021-06-02 19:14:19.000000 mqttwarn-0.34.1/docs/assets/logo/img/markword_200x200.png
+-rw-r--r--   0 amo        (501) staff       (20)    30766 2021-06-02 19:14:19.000000 mqttwarn-0.34.1/docs/assets/logo/img/markword_500x500.png
+drwxr-xr-x   0 amo        (501) staff       (20)        0 2023-05-17 23:13:24.452103 mqttwarn-0.34.1/docs/assets/logo/src/
+-rw-r--r--   0 amo        (501) staff       (20)    11742 2021-06-02 19:14:19.000000 mqttwarn-0.34.1/docs/assets/logo/src/hz_wordmark_blk.svg
+-rw-r--r--   0 amo        (501) staff       (20)    11978 2021-06-02 19:14:19.000000 mqttwarn-0.34.1/docs/assets/logo/src/hz_wordmark_wht.svg
+-rw-r--r--   0 amo        (501) staff       (20)     5872 2021-06-02 19:14:19.000000 mqttwarn-0.34.1/docs/assets/logo/src/markonly.svg
+-rw-r--r--   0 amo        (501) staff       (20)     6869 2021-06-02 19:14:19.000000 mqttwarn-0.34.1/docs/assets/logo/src/wordmark.svg
+-rw-r--r--   0 amo        (501) staff       (20)    30987 2021-06-02 19:14:19.000000 mqttwarn-0.34.1/docs/assets/mattermost.png
+-rw-r--r--   0 amo        (501) staff       (20)    24837 2021-06-02 19:14:19.000000 mqttwarn-0.34.1/docs/assets/mqttwarn.png
+-rw-r--r--   0 amo        (501) staff       (20)    17999 2021-06-02 19:14:19.000000 mqttwarn-0.34.1/docs/assets/pastebin.png
+-rw-r--r--   0 amo        (501) staff       (20)    12239 2021-06-02 19:14:19.000000 mqttwarn-0.34.1/docs/assets/prowl.jpg
+-rw-r--r--   0 amo        (501) staff       (20)    49652 2021-06-02 19:14:19.000000 mqttwarn-0.34.1/docs/assets/pushalot.png
+-rw-r--r--   0 amo        (501) staff       (20)     6254 2021-06-02 19:14:19.000000 mqttwarn-0.34.1/docs/assets/pushbullet.jpg
+-rw-r--r--   0 amo        (501) staff       (20)    45628 2021-06-02 19:14:19.000000 mqttwarn-0.34.1/docs/assets/pushover.png
+-rw-r--r--   0 amo        (501) staff       (20)    69330 2021-06-02 19:14:19.000000 mqttwarn-0.34.1/docs/assets/pushsafer.jpg
+-rw-r--r--   0 amo        (501) staff       (20)    10867 2021-06-02 19:14:19.000000 mqttwarn-0.34.1/docs/assets/slack.png
+-rw-r--r--   0 amo        (501) staff       (20)    36822 2021-06-02 19:14:19.000000 mqttwarn-0.34.1/docs/assets/telegram.png
+-rw-r--r--   0 amo        (501) staff       (20)    22281 2021-06-02 19:14:19.000000 mqttwarn-0.34.1/docs/assets/tootpaste.png
+-rw-r--r--   0 amo        (501) staff       (20)    14048 2023-05-07 15:37:15.000000 mqttwarn-0.34.1/docs/assets/twilio.jpg
+-rw-r--r--   0 amo        (501) staff       (20)    13550 2021-06-02 19:14:19.000000 mqttwarn-0.34.1/docs/assets/twitter.jpg
+-rw-r--r--   0 amo        (501) staff       (20)    54535 2021-06-02 19:14:19.000000 mqttwarn-0.34.1/docs/assets/zabbix.png
+-rw-r--r--   0 amo        (501) staff       (20)     2487 2023-04-18 22:55:29.000000 mqttwarn-0.34.1/docs/conf.py
+drwxr-xr-x   0 amo        (501) staff       (20)        0 2023-05-17 23:13:24.471377 mqttwarn-0.34.1/docs/configure/
+-rw-r--r--   0 amo        (501) staff       (20)     2346 2023-05-07 15:37:15.000000 mqttwarn-0.34.1/docs/configure/index.rst
+-rw-r--r--   0 amo        (501) staff       (20)     6353 2023-05-09 16:42:28.000000 mqttwarn-0.34.1/docs/configure/mqttwarn.ini.md
+-rw-r--r--   0 amo        (501) staff       (20)     8277 2023-05-07 16:41:44.000000 mqttwarn-0.34.1/docs/configure/service.md
+-rw-r--r--   0 amo        (501) staff       (20)     1226 2023-04-18 22:55:29.000000 mqttwarn-0.34.1/docs/configure/task.md
+-rw-r--r--   0 amo        (501) staff       (20)     6551 2023-05-07 15:37:15.000000 mqttwarn-0.34.1/docs/configure/topic.md
+-rw-r--r--   0 amo        (501) staff       (20)    20884 2023-05-17 22:52:19.000000 mqttwarn-0.34.1/docs/configure/transformation.md
+drwxr-xr-x   0 amo        (501) staff       (20)        0 2023-05-17 23:13:24.472856 mqttwarn-0.34.1/docs/examples/
+-rw-r--r--   0 amo        (501) staff       (20)        0 2021-06-02 19:14:19.000000 mqttwarn-0.34.1/docs/examples/__init__.py
+drwxr-xr-x   0 amo        (501) staff       (20)        0 2023-05-17 23:13:24.475700 mqttwarn-0.34.1/docs/examples/alexa/
+-rw-r--r--   0 amo        (501) staff       (20)      777 2023-03-12 10:52:16.000000 mqttwarn-0.34.1/docs/examples/alexa/alexa.ini
+-rw-r--r--   0 amo        (501) staff       (20)      289 2023-03-12 10:52:16.000000 mqttwarn-0.34.1/docs/examples/alexa/announce_stdin
+-rw-r--r--   0 amo        (501) staff       (20)      784 2023-04-18 22:55:29.000000 mqttwarn-0.34.1/docs/examples/alexa/readme.md
+-rw-r--r--   0 amo        (501) staff       (20)      258 2023-03-12 10:52:16.000000 mqttwarn-0.34.1/docs/examples/alexa/saystdin
+-rw-r--r--   0 amo        (501) staff       (20)      270 2023-03-12 10:52:16.000000 mqttwarn-0.34.1/docs/examples/alexa/secrets.sh
+drwxr-xr-x   0 amo        (501) staff       (20)        0 2023-05-17 23:13:24.476055 mqttwarn-0.34.1/docs/examples/arduino-temperature/
+-rw-r--r--   0 amo        (501) staff       (20)     1339 2023-04-18 22:55:29.000000 mqttwarn-0.34.1/docs/examples/arduino-temperature/readme.md
+-rw-r--r--   0 amo        (501) staff       (20)       58 2023-04-18 22:40:31.000000 mqttwarn-0.34.1/docs/examples/conftest.py
+drwxr-xr-x   0 amo        (501) staff       (20)        0 2023-05-17 23:13:24.480810 mqttwarn-0.34.1/docs/examples/frigate/
+-rw-r--r--   0 amo        (501) staff       (20)      194 2023-04-27 20:00:41.000000 mqttwarn-0.34.1/docs/examples/frigate/.env
+-rw-r--r--   0 amo        (501) staff       (20)       19 2023-04-18 22:40:03.000000 mqttwarn-0.34.1/docs/examples/frigate/.gitignore
+-rw-r--r--   0 amo        (501) staff       (20)     6037 2023-05-07 15:37:15.000000 mqttwarn-0.34.1/docs/examples/frigate/README.rst
+drwxr-xr-x   0 amo        (501) staff       (20)        0 2023-05-17 23:13:24.485208 mqttwarn-0.34.1/docs/examples/frigate/assets/
+-rw-r--r--   0 amo        (501) staff       (20)      831 2023-04-18 22:40:31.000000 mqttwarn-0.34.1/docs/examples/frigate/assets/frigate-event-end.json
+-rw-r--r--   0 amo        (501) staff       (20)      830 2023-04-18 22:40:31.000000 mqttwarn-0.34.1/docs/examples/frigate/assets/frigate-event-false-positive.json
+-rw-r--r--   0 amo        (501) staff       (20)     1369 2023-04-27 20:00:41.000000 mqttwarn-0.34.1/docs/examples/frigate/assets/frigate-event-full.json
+-rw-r--r--   0 amo        (501) staff       (20)      848 2023-04-18 22:40:31.000000 mqttwarn-0.34.1/docs/examples/frigate/assets/frigate-event-new-good.json
+-rw-r--r--   0 amo        (501) staff       (20)      822 2023-04-18 22:40:31.000000 mqttwarn-0.34.1/docs/examples/frigate/assets/frigate-event-new-ignored.json
+-rw-r--r--   0 amo        (501) staff       (20)      851 2023-04-27 20:00:41.000000 mqttwarn-0.34.1/docs/examples/frigate/assets/frigate-event-update-good.json
+-rw-r--r--   0 amo        (501) staff       (20)      815 2023-04-18 22:40:31.000000 mqttwarn-0.34.1/docs/examples/frigate/assets/frigate-event-update-samezone.json
+-rw-r--r--   0 amo        (501) staff       (20)      882 2023-04-18 22:40:31.000000 mqttwarn-0.34.1/docs/examples/frigate/assets/frigate-event-update-stationary.json
+-rw-r--r--   0 amo        (501) staff       (20)     1680 2023-04-27 20:00:41.000000 mqttwarn-0.34.1/docs/examples/frigate/docker-compose.yml
+-rw-r--r--   0 amo        (501) staff       (20)     2234 2023-04-27 20:13:19.000000 mqttwarn-0.34.1/docs/examples/frigate/frigate.ini
+-rw-r--r--   0 amo        (501) staff       (20)     6521 2023-04-27 20:08:12.000000 mqttwarn-0.34.1/docs/examples/frigate/frigate.py
+-rwxr-xr-x   0 amo        (501) staff       (20)      690 2023-04-27 20:00:41.000000 mqttwarn-0.34.1/docs/examples/frigate/publish.sh
+-rw-r--r--   0 amo        (501) staff       (20)     9407 2023-04-27 20:37:53.000000 mqttwarn-0.34.1/docs/examples/frigate/test_frigate.py
+drwxr-xr-x   0 amo        (501) staff       (20)        0 2023-05-17 23:13:24.486302 mqttwarn-0.34.1/docs/examples/hiveeyes/
+-rw-r--r--   0 amo        (501) staff       (20)        0 2021-06-02 19:14:19.000000 mqttwarn-0.34.1/docs/examples/hiveeyes/__init__.py
+-rw-r--r--   0 amo        (501) staff       (20)     2749 2023-05-07 15:37:15.000000 mqttwarn-0.34.1/docs/examples/hiveeyes/hiveeyes.ini
+-rw-r--r--   0 amo        (501) staff       (20)    10808 2023-04-20 19:05:51.000000 mqttwarn-0.34.1/docs/examples/hiveeyes/hiveeyes.py
+drwxr-xr-x   0 amo        (501) staff       (20)        0 2023-05-17 23:13:24.487550 mqttwarn-0.34.1/docs/examples/homie/
+-rw-r--r--   0 amo        (501) staff       (20)        0 2021-06-02 19:14:19.000000 mqttwarn-0.34.1/docs/examples/homie/__init__.py
+-rw-r--r--   0 amo        (501) staff       (20)     1631 2023-05-07 15:37:15.000000 mqttwarn-0.34.1/docs/examples/homie/homie.ini
+-rw-r--r--   0 amo        (501) staff       (20)      838 2023-04-20 19:05:51.000000 mqttwarn-0.34.1/docs/examples/homie/homie.py
+drwxr-xr-x   0 amo        (501) staff       (20)        0 2023-05-17 23:13:24.488582 mqttwarn-0.34.1/docs/examples/mediaplayer/
+-rw-r--r--   0 amo        (501) staff       (20)      316 2023-05-07 15:37:15.000000 mqttwarn-0.34.1/docs/examples/mediaplayer/mqttwarn-mplayer.ini
+-rw-r--r--   0 amo        (501) staff       (20)     1571 2023-05-09 16:42:20.000000 mqttwarn-0.34.1/docs/examples/mediaplayer/readme.md
+drwxr-xr-x   0 amo        (501) staff       (20)        0 2023-05-17 23:13:24.490232 mqttwarn-0.34.1/docs/examples/owntracks-ntfy/
+-rw-r--r--   0 amo        (501) staff       (20)      398 2023-05-13 12:14:01.000000 mqttwarn-0.34.1/docs/examples/owntracks-ntfy/mqttwarn-owntracks.ini
+-rw-r--r--   0 amo        (501) staff       (20)      432 2023-05-12 21:49:48.000000 mqttwarn-0.34.1/docs/examples/owntracks-ntfy/mqttwarn-owntracks.py
+-rw-r--r--   0 amo        (501) staff       (20)     4917 2023-05-17 22:52:19.000000 mqttwarn-0.34.1/docs/examples/owntracks-ntfy/readme.md
+-rw-r--r--   0 amo        (501) staff       (20)      350 2023-05-12 21:49:48.000000 mqttwarn-0.34.1/docs/examples/readme.md
+drwxr-xr-x   0 amo        (501) staff       (20)        0 2023-05-17 23:13:24.490574 mqttwarn-0.34.1/docs/examples/warntoggle/
+-rw-r--r--   0 amo        (501) staff       (20)     1917 2023-04-18 22:55:29.000000 mqttwarn-0.34.1/docs/examples/warntoggle/README.rst
+drwxr-xr-x   0 amo        (501) staff       (20)        0 2023-05-17 23:13:24.490975 mqttwarn-0.34.1/docs/examples/warntoggle/mqttwarn/
+-rw-r--r--   0 amo        (501) staff       (20)     1343 2023-04-20 19:05:51.000000 mqttwarn-0.34.1/docs/examples/warntoggle/mqttwarn/customfunctions.py
+drwxr-xr-x   0 amo        (501) staff       (20)        0 2023-05-17 23:13:24.492031 mqttwarn-0.34.1/docs/examples/warntoggle/www/
+-rw-r--r--   0 amo        (501) staff       (20)       97 2023-03-12 10:52:16.000000 mqttwarn-0.34.1/docs/examples/warntoggle/www/warntoggle.json
+-rw-r--r--   0 amo        (501) staff       (20)     1441 2023-04-20 19:05:51.000000 mqttwarn-0.34.1/docs/examples/warntoggle/www/warntoggle.py
+drwxr-xr-x   0 amo        (501) staff       (20)        0 2023-05-17 23:13:24.493566 mqttwarn-0.34.1/docs/examples/zabbix-iot/
+-rw-r--r--   0 amo        (501) staff       (20)      193 2023-05-09 16:42:20.000000 mqttwarn-0.34.1/docs/examples/zabbix-iot/mqttwarn-zabbix-iot.ini
+-rw-r--r--   0 amo        (501) staff       (20)      413 2023-05-09 16:42:20.000000 mqttwarn-0.34.1/docs/examples/zabbix-iot/mqttwarn-zabbix-iot.py
+-rw-r--r--   0 amo        (501) staff       (20)     3226 2023-05-09 16:42:20.000000 mqttwarn-0.34.1/docs/examples/zabbix-iot/readme.md
+-rw-r--r--   0 amo        (501) staff       (20)     4757 2023-05-07 17:07:28.000000 mqttwarn-0.34.1/docs/index.rst
+-rw-r--r--   0 amo        (501) staff       (20)      800 2023-04-18 22:55:29.000000 mqttwarn-0.34.1/docs/make.bat
+-rw-r--r--   0 amo        (501) staff       (20)     9597 2021-06-02 19:14:19.000000 mqttwarn-0.34.1/docs/mqttwarn-logo.png
+-rw-r--r--   0 amo        (501) staff       (20)   103691 2023-05-07 15:37:15.000000 mqttwarn-0.34.1/docs/notifier-catalog.md
+-rw-r--r--   0 amo        (501) staff       (20)     8535 2023-05-07 17:07:28.000000 mqttwarn-0.34.1/docs/readme.rst
+-rw-r--r--   0 amo        (501) staff       (20)      110 2023-04-18 22:55:29.000000 mqttwarn-0.34.1/docs/requirements.txt
+drwxr-xr-x   0 amo        (501) staff       (20)        0 2023-05-17 23:13:24.495857 mqttwarn-0.34.1/docs/usage/
+-rw-r--r--   0 amo        (501) staff       (20)     1562 2023-05-07 15:37:15.000000 mqttwarn-0.34.1/docs/usage/freebsd.md
+-rw-r--r--   0 amo        (501) staff       (20)     1540 2023-05-07 15:37:15.000000 mqttwarn-0.34.1/docs/usage/index.rst
+-rw-r--r--   0 amo        (501) staff       (20)     6318 2023-05-07 15:37:15.000000 mqttwarn-0.34.1/docs/usage/oci.md
+-rw-r--r--   0 amo        (501) staff       (20)      537 2023-05-17 22:52:19.000000 mqttwarn-0.34.1/docs/usage/pip.md
+-rw-r--r--   0 amo        (501) staff       (20)     3374 2023-05-07 15:37:15.000000 mqttwarn-0.34.1/docs/usage/standalone.md
+drwxr-xr-x   0 amo        (501) staff       (20)        0 2023-05-17 23:13:24.497613 mqttwarn-0.34.1/docs/workbench/
+-rw-r--r--   0 amo        (501) staff       (20)     8086 2023-05-17 22:52:15.000000 mqttwarn-0.34.1/docs/workbench/backlog.rst
+-rw-r--r--   0 amo        (501) staff       (20)    15169 2023-05-17 22:54:38.000000 mqttwarn-0.34.1/docs/workbench/changelog.rst
+-rw-r--r--   0 amo        (501) staff       (20)      183 2023-05-09 19:10:22.000000 mqttwarn-0.34.1/docs/workbench/ideas.md
+-rw-r--r--   0 amo        (501) staff       (20)     2909 2023-05-07 15:37:15.000000 mqttwarn-0.34.1/docs/workbench/sandbox.rst
+drwxr-xr-x   0 amo        (501) staff       (20)        0 2023-05-17 23:13:24.502060 mqttwarn-0.34.1/mqttwarn/
+-rw-r--r--   0 amo        (501) staff       (20)      481 2023-05-07 15:37:15.000000 mqttwarn-0.34.1/mqttwarn/__init__.py
+-rw-r--r--   0 amo        (501) staff       (20)       50 2023-03-12 10:52:16.000000 mqttwarn-0.34.1/mqttwarn/__main__.py
+-rw-r--r--   0 amo        (501) staff       (20)     5906 2023-04-27 23:01:45.000000 mqttwarn-0.34.1/mqttwarn/commands.py
+-rw-r--r--   0 amo        (501) staff       (20)     6269 2023-05-07 15:37:15.000000 mqttwarn-0.34.1/mqttwarn/configuration.py
+-rw-r--r--   0 amo        (501) staff       (20)     8105 2023-05-07 15:37:15.000000 mqttwarn-0.34.1/mqttwarn/context.py
+-rw-r--r--   0 amo        (501) staff       (20)    30482 2023-05-07 15:37:15.000000 mqttwarn-0.34.1/mqttwarn/core.py
+-rw-r--r--   0 amo        (501) staff       (20)     2539 2023-04-27 20:56:31.000000 mqttwarn-0.34.1/mqttwarn/cron.py
+drwxr-xr-x   0 amo        (501) staff       (20)        0 2023-05-17 23:13:24.504597 mqttwarn-0.34.1/mqttwarn/examples/
+-rw-r--r--   0 amo        (501) staff       (20)        0 2021-06-02 19:14:19.000000 mqttwarn-0.34.1/mqttwarn/examples/__init__.py
+drwxr-xr-x   0 amo        (501) staff       (20)        0 2023-05-17 23:13:24.505286 mqttwarn-0.34.1/mqttwarn/examples/basic/
+-rwxr-xr-x   0 amo        (501) staff       (20)     3831 2023-05-07 15:37:15.000000 mqttwarn-0.34.1/mqttwarn/examples/basic/mqttwarn.ini
+-rwxr-xr-x   0 amo        (501) staff       (20)     3060 2023-04-27 20:56:31.000000 mqttwarn-0.34.1/mqttwarn/examples/basic/udf.py
+-rw-r--r--   0 amo        (501) staff       (20)     4053 2023-05-07 15:37:15.000000 mqttwarn-0.34.1/mqttwarn/model.py
+drwxr-xr-x   0 amo        (501) staff       (20)        0 2023-05-17 23:13:24.542625 mqttwarn-0.34.1/mqttwarn/services/
+-rw-r--r--   0 amo        (501) staff       (20)        0 2021-06-02 19:14:19.000000 mqttwarn-0.34.1/mqttwarn/services/__init__.py
+-rw-r--r--   0 amo        (501) staff       (20)     1321 2023-05-07 15:37:15.000000 mqttwarn-0.34.1/mqttwarn/services/alexa-notify-me.py
+-rw-r--r--   0 amo        (501) staff       (20)     1322 2023-03-12 10:52:16.000000 mqttwarn-0.34.1/mqttwarn/services/amqp.py
+-rw-r--r--   0 amo        (501) staff       (20)     1310 2023-04-27 20:56:31.000000 mqttwarn-0.34.1/mqttwarn/services/apns.py
+-rw-r--r--   0 amo        (501) staff       (20)      316 2023-03-12 10:52:16.000000 mqttwarn-0.34.1/mqttwarn/services/apprise.py
+-rw-r--r--   0 amo        (501) staff       (20)     2639 2023-04-26 22:18:29.000000 mqttwarn-0.34.1/mqttwarn/services/apprise_multi.py
+-rw-r--r--   0 amo        (501) staff       (20)     2448 2023-04-26 22:18:29.000000 mqttwarn-0.34.1/mqttwarn/services/apprise_single.py
+-rw-r--r--   0 amo        (501) staff       (20)     1392 2023-04-26 22:18:29.000000 mqttwarn-0.34.1/mqttwarn/services/apprise_util.py
+-rw-r--r--   0 amo        (501) staff       (20)     1916 2023-03-12 10:52:16.000000 mqttwarn-0.34.1/mqttwarn/services/asterisk.py
+-rw-r--r--   0 amo        (501) staff       (20)     1467 2023-05-07 15:37:15.000000 mqttwarn-0.34.1/mqttwarn/services/autoremote.py
+-rw-r--r--   0 amo        (501) staff       (20)     2331 2023-03-12 10:52:16.000000 mqttwarn-0.34.1/mqttwarn/services/azure_iot.py
+-rw-r--r--   0 amo        (501) staff       (20)     2114 2023-03-12 10:52:16.000000 mqttwarn-0.34.1/mqttwarn/services/carbon.py
+-rw-r--r--   0 amo        (501) staff       (20)      862 2021-06-02 19:14:19.000000 mqttwarn-0.34.1/mqttwarn/services/celery.py
+-rw-r--r--   0 amo        (501) staff       (20)     2160 2023-03-12 10:52:16.000000 mqttwarn-0.34.1/mqttwarn/services/chromecast.py
+-rw-r--r--   0 amo        (501) staff       (20)     1369 2021-06-02 19:14:19.000000 mqttwarn-0.34.1/mqttwarn/services/dbus.py
+-rw-r--r--   0 amo        (501) staff       (20)     1604 2023-04-27 20:56:31.000000 mqttwarn-0.34.1/mqttwarn/services/desktopnotify.py
+-rw-r--r--   0 amo        (501) staff       (20)     1580 2021-06-02 19:14:19.000000 mqttwarn-0.34.1/mqttwarn/services/dnsupdate.py
+-rw-r--r--   0 amo        (501) staff       (20)     1371 2023-04-27 20:56:31.000000 mqttwarn-0.34.1/mqttwarn/services/emoncms.py
+-rw-r--r--   0 amo        (501) staff       (20)      878 2023-05-07 15:37:15.000000 mqttwarn-0.34.1/mqttwarn/services/execute.py
+-rw-r--r--   0 amo        (501) staff       (20)     1084 2021-06-02 19:14:19.000000 mqttwarn-0.34.1/mqttwarn/services/fbchat.py
+-rw-r--r--   0 amo        (501) staff       (20)     2242 2023-04-18 22:40:03.000000 mqttwarn-0.34.1/mqttwarn/services/file.py
+-rw-r--r--   0 amo        (501) staff       (20)     2609 2021-06-02 19:14:19.000000 mqttwarn-0.34.1/mqttwarn/services/freeswitch.py
+-rw-r--r--   0 amo        (501) staff       (20)     4586 2023-04-27 20:56:31.000000 mqttwarn-0.34.1/mqttwarn/services/gss2.py
+-rw-r--r--   0 amo        (501) staff       (20)     1418 2023-05-07 15:37:15.000000 mqttwarn-0.34.1/mqttwarn/services/hangbot.py
+-rw-r--r--   0 amo        (501) staff       (20)     4229 2023-04-27 20:56:31.000000 mqttwarn-0.34.1/mqttwarn/services/http_urllib.py
+-rw-r--r--   0 amo        (501) staff       (20)     2263 2023-04-27 20:56:31.000000 mqttwarn-0.34.1/mqttwarn/services/icinga2.py
+-rw-r--r--   0 amo        (501) staff       (20)     1084 2021-06-02 19:14:19.000000 mqttwarn-0.34.1/mqttwarn/services/ifttt.py
+-rw-r--r--   0 amo        (501) staff       (20)     3671 2023-03-12 10:52:16.000000 mqttwarn-0.34.1/mqttwarn/services/influxdb.py
+-rw-r--r--   0 amo        (501) staff       (20)     2615 2023-04-27 20:56:31.000000 mqttwarn-0.34.1/mqttwarn/services/ionic.py
+-rw-r--r--   0 amo        (501) staff       (20)     1315 2023-05-07 15:37:15.000000 mqttwarn-0.34.1/mqttwarn/services/irccat.py
+-rw-r--r--   0 amo        (501) staff       (20)     1022 2021-06-02 19:14:19.000000 mqttwarn-0.34.1/mqttwarn/services/linuxnotify.py
+-rw-r--r--   0 amo        (501) staff       (20)      881 2023-03-12 10:52:16.000000 mqttwarn-0.34.1/mqttwarn/services/log.py
+-rw-r--r--   0 amo        (501) staff       (20)     2491 2023-04-27 20:56:31.000000 mqttwarn-0.34.1/mqttwarn/services/mattermost.py
+-rw-r--r--   0 amo        (501) staff       (20)     3468 2021-06-19 14:00:07.000000 mqttwarn-0.34.1/mqttwarn/services/mqtt.py
+-rw-r--r--   0 amo        (501) staff       (20)     2337 2023-03-12 10:52:16.000000 mqttwarn-0.34.1/mqttwarn/services/mqtt_filter.py
+-rw-r--r--   0 amo        (501) staff       (20)     1340 2023-03-12 10:52:16.000000 mqttwarn-0.34.1/mqttwarn/services/mqttpub.py
+-rw-r--r--   0 amo        (501) staff       (20)     3064 2023-03-12 10:52:16.000000 mqttwarn-0.34.1/mqttwarn/services/mysql.py
+-rw-r--r--   0 amo        (501) staff       (20)     4557 2023-03-12 10:52:16.000000 mqttwarn-0.34.1/mqttwarn/services/mysql_dynamic.py
+-rw-r--r--   0 amo        (501) staff       (20)     3075 2023-03-12 10:52:16.000000 mqttwarn-0.34.1/mqttwarn/services/mysql_remap.py
+-rw-r--r--   0 amo        (501) staff       (20)     1387 2021-06-02 19:14:19.000000 mqttwarn-0.34.1/mqttwarn/services/mythtv.py
+-rw-r--r--   0 amo        (501) staff       (20)     1610 2021-06-02 19:14:19.000000 mqttwarn-0.34.1/mqttwarn/services/nntp.py
+-rw-r--r--   0 amo        (501) staff       (20)      468 2023-05-07 15:37:15.000000 mqttwarn-0.34.1/mqttwarn/services/noop.py
+-rw-r--r--   0 amo        (501) staff       (20)     1135 2023-03-12 10:52:16.000000 mqttwarn-0.34.1/mqttwarn/services/nsca.py
+-rw-r--r--   0 amo        (501) staff       (20)    10095 2023-04-27 20:12:45.000000 mqttwarn-0.34.1/mqttwarn/services/ntfy.py
+-rw-r--r--   0 amo        (501) staff       (20)     1040 2021-06-02 19:14:19.000000 mqttwarn-0.34.1/mqttwarn/services/osxsay.py
+-rw-r--r--   0 amo        (501) staff       (20)     1587 2021-06-19 14:00:07.000000 mqttwarn-0.34.1/mqttwarn/services/pastebinpub.py
+-rw-r--r--   0 amo        (501) staff       (20)     1092 2023-03-12 10:52:16.000000 mqttwarn-0.34.1/mqttwarn/services/pipe.py
+-rw-r--r--   0 amo        (501) staff       (20)     3360 2023-03-12 10:52:16.000000 mqttwarn-0.34.1/mqttwarn/services/postgres.py
+-rw-r--r--   0 amo        (501) staff       (20)     1164 2023-03-12 10:52:16.000000 mqttwarn-0.34.1/mqttwarn/services/prowl.py
+-rw-r--r--   0 amo        (501) staff       (20)     1204 2021-06-02 19:14:19.000000 mqttwarn-0.34.1/mqttwarn/services/pushbullet.py
+-rw-r--r--   0 amo        (501) staff       (20)     5676 2023-03-12 10:52:16.000000 mqttwarn-0.34.1/mqttwarn/services/pushover.py
+-rw-r--r--   0 amo        (501) staff       (20)     8091 2023-04-11 20:10:09.000000 mqttwarn-0.34.1/mqttwarn/services/pushsafer.py
+-rw-r--r--   0 amo        (501) staff       (20)      955 2021-06-02 19:14:19.000000 mqttwarn-0.34.1/mqttwarn/services/redispub.py
+-rw-r--r--   0 amo        (501) staff       (20)     1193 2023-05-07 15:37:15.000000 mqttwarn-0.34.1/mqttwarn/services/rrdtool.py
+-rw-r--r--   0 amo        (501) staff       (20)     2202 2023-03-12 10:52:16.000000 mqttwarn-0.34.1/mqttwarn/services/serial.py
+-rw-r--r--   0 amo        (501) staff       (20)     3480 2023-03-12 10:52:16.000000 mqttwarn-0.34.1/mqttwarn/services/slack.py
+-rw-r--r--   0 amo        (501) staff       (20)     1910 2023-03-12 10:52:16.000000 mqttwarn-0.34.1/mqttwarn/services/slixmpp.py
+-rw-r--r--   0 amo        (501) staff       (20)     2156 2023-03-12 10:52:16.000000 mqttwarn-0.34.1/mqttwarn/services/smtp.py
+-rw-r--r--   0 amo        (501) staff       (20)     1157 2021-06-02 19:14:19.000000 mqttwarn-0.34.1/mqttwarn/services/sqlite.py
+-rw-r--r--   0 amo        (501) staff       (20)     3024 2021-06-19 14:00:07.000000 mqttwarn-0.34.1/mqttwarn/services/sqlite_json2cols.py
+-rw-r--r--   0 amo        (501) staff       (20)     1317 2021-06-02 19:14:19.000000 mqttwarn-0.34.1/mqttwarn/services/sqlite_timestamp.py
+-rw-r--r--   0 amo        (501) staff       (20)     2116 2023-03-12 10:52:16.000000 mqttwarn-0.34.1/mqttwarn/services/ssh.py
+-rw-r--r--   0 amo        (501) staff       (20)     2329 2021-06-02 19:14:19.000000 mqttwarn-0.34.1/mqttwarn/services/syslog.py
+-rw-r--r--   0 amo        (501) staff       (20)     4472 2023-05-07 15:37:15.000000 mqttwarn-0.34.1/mqttwarn/services/telegram.py
+-rw-r--r--   0 amo        (501) staff       (20)     2881 2021-06-19 14:00:07.000000 mqttwarn-0.34.1/mqttwarn/services/thingspeak.py
+-rw-r--r--   0 amo        (501) staff       (20)     1780 2021-06-07 22:34:47.000000 mqttwarn-0.34.1/mqttwarn/services/tootpaste.py
+-rw-r--r--   0 amo        (501) staff       (20)     1050 2021-06-02 19:14:19.000000 mqttwarn-0.34.1/mqttwarn/services/twilio.py
+-rw-r--r--   0 amo        (501) staff       (20)     1070 2021-06-02 19:14:19.000000 mqttwarn-0.34.1/mqttwarn/services/twitter.py
+-rw-r--r--   0 amo        (501) staff       (20)     1210 2023-03-12 10:52:16.000000 mqttwarn-0.34.1/mqttwarn/services/websocket.py
+-rw-r--r--   0 amo        (501) staff       (20)     2168 2023-04-27 20:56:31.000000 mqttwarn-0.34.1/mqttwarn/services/xbmc.py
+-rw-r--r--   0 amo        (501) staff       (20)     2457 2021-06-02 19:14:19.000000 mqttwarn-0.34.1/mqttwarn/services/xmpp.py
+-rw-r--r--   0 amo        (501) staff       (20)     3265 2023-04-27 20:56:31.000000 mqttwarn-0.34.1/mqttwarn/services/zabbix.py
+drwxr-xr-x   0 amo        (501) staff       (20)        0 2023-05-17 23:13:24.543394 mqttwarn-0.34.1/mqttwarn/testing/
+-rw-r--r--   0 amo        (501) staff       (20)        0 2023-03-12 10:52:16.000000 mqttwarn-0.34.1/mqttwarn/testing/__init__.py
+-rw-r--r--   0 amo        (501) staff       (20)      375 2023-03-12 10:52:16.000000 mqttwarn-0.34.1/mqttwarn/testing/fixtures.py
+-rw-r--r--   0 amo        (501) staff       (20)     7095 2023-05-17 22:52:19.000000 mqttwarn-0.34.1/mqttwarn/util.py
+drwxr-xr-x   0 amo        (501) staff       (20)        0 2023-05-17 23:13:24.544274 mqttwarn-0.34.1/mqttwarn/vendor/
+-rw-r--r--   0 amo        (501) staff       (20)     2307 2023-05-07 15:37:15.000000 mqttwarn-0.34.1/mqttwarn/vendor/ZabbixSender.py
+-rw-r--r--   0 amo        (501) staff       (20)        0 2023-03-12 10:52:16.000000 mqttwarn-0.34.1/mqttwarn/vendor/__init__.py
+drwxr-xr-x   0 amo        (501) staff       (20)        0 2023-05-17 23:13:24.504345 mqttwarn-0.34.1/mqttwarn.egg-info/
+-rw-r--r--   0 amo        (501) staff       (20)    11492 2023-05-17 23:13:24.000000 mqttwarn-0.34.1/mqttwarn.egg-info/PKG-INFO
+-rw-r--r--   0 amo        (501) staff       (20)     6219 2023-05-17 23:13:24.000000 mqttwarn-0.34.1/mqttwarn.egg-info/SOURCES.txt
+-rw-r--r--   0 amo        (501) staff       (20)        1 2023-05-17 23:13:24.000000 mqttwarn-0.34.1/mqttwarn.egg-info/dependency_links.txt
+-rw-r--r--   0 amo        (501) staff       (20)       51 2023-05-17 23:13:24.000000 mqttwarn-0.34.1/mqttwarn.egg-info/entry_points.txt
+-rw-r--r--   0 amo        (501) staff       (20)        1 2021-06-02 19:17:07.000000 mqttwarn-0.34.1/mqttwarn.egg-info/not-zip-safe
+-rw-r--r--   0 amo        (501) staff       (20)     2265 2023-05-17 23:13:24.000000 mqttwarn-0.34.1/mqttwarn.egg-info/requires.txt
+-rw-r--r--   0 amo        (501) staff       (20)       24 2023-05-17 23:13:24.000000 mqttwarn-0.34.1/mqttwarn.egg-info/top_level.txt
+-rw-r--r--   0 amo        (501) staff       (20)     2847 2023-05-17 23:11:37.000000 mqttwarn-0.34.1/pyproject.toml
+-rw-r--r--   0 amo        (501) staff       (20)       20 2023-05-17 22:58:11.000000 mqttwarn-0.34.1/requirements-release.txt
+-rw-r--r--   0 amo        (501) staff       (20)       38 2023-05-17 23:13:24.545173 mqttwarn-0.34.1/setup.cfg
+-rw-r--r--   0 amo        (501) staff       (20)     6513 2023-05-17 22:52:19.000000 mqttwarn-0.34.1/setup.py
```

### Comparing `mqttwarn-0.34.0/CHANGES.rst` & `mqttwarn-0.34.1/CHANGES.rst`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,26 @@
 ##################
 
 
 in progress
 ===========
 
 
+2023-05-15 0.34.1
+=================
+
+- Add example "Simple MQTT media player". Thanks, @nagyrobi.
+- Add example "Forwarding data from IoT devices to Zabbix"
+- Remove support for Secure Sockets Layer Version 3.0 (SSLv3).
+  As per RFC 7568, SSLv3 has been deprecated in 2015 already.
+- Tests: Add more test cases to increase mqttwarn core coverage to ~100%
+- Improve example "Forward OwnTracks low-battery warnings to ntfy"
+- Migrate documentation to https://mqttwarn.readthedocs.io/
+
+
 2023-04-28 0.34.0
 =================
 
 - Fix: Don't crash when receiving non-UTF8 payloads. Thanks, @sevmonster.
 - Improve exception logging in ``is_filtered``, ``get_topic_data``, and
   ``get_all_data`` context functions. Thanks, @sevmonster.
 - [core] Allow processing of binary, non-UTF8 message payloads, for example
```

### Comparing `mqttwarn-0.34.0/LICENSE` & `mqttwarn-0.34.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mqttwarn-0.34.0/PKG-INFO` & `mqttwarn-0.34.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: mqttwarn
-Version: 0.34.0
+Version: 0.34.1
 Summary: mqttwarn - subscribe to MQTT topics and notify pluggable services
-Home-page: https://github.com/jpmens/mqttwarn
+Home-page: https://github.com/mqtt-tools/mqttwarn
 Author: Jan-Piet Mens, Ben Jones, Andreas Motl
 Author-email: jpmens@gmail.com
 License: EPL 2.0
 Keywords: mqtt notification plugins data acquisition push transformation engine mosquitto
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Environment :: Plugins
@@ -49,18 +49,17 @@
 Provides-Extra: apns
 Provides-Extra: apprise
 Provides-Extra: asterisk
 Provides-Extra: celery
 Provides-Extra: chromecast
 Provides-Extra: dnsupdate
 Provides-Extra: fbchat
-Provides-Extra: gss
 Provides-Extra: gss2
 Provides-Extra: mysql
-Provides-Extra: nma
+Provides-Extra: mysql_dynamic
 Provides-Extra: nsca
 Provides-Extra: desktopnotify
 Provides-Extra: pastebinpub
 Provides-Extra: postgres
 Provides-Extra: prowl
 Provides-Extra: pushbullet
 Provides-Extra: redispub
@@ -68,28 +67,27 @@
 Provides-Extra: serial
 Provides-Extra: slack
 Provides-Extra: ssh
 Provides-Extra: tootpaste
 Provides-Extra: twilio
 Provides-Extra: twitter
 Provides-Extra: websocket
-Provides-Extra: xively
 Provides-Extra: xmpp
 Provides-Extra: slixmpp
 Provides-Extra: contrib
 Provides-Extra: all
 Provides-Extra: test
 Provides-Extra: develop
 License-File: LICENSE
 
-.. image:: https://github.com/jpmens/mqttwarn/workflows/Tests/badge.svg
-    :target: https://github.com/jpmens/mqttwarn/actions?workflow=Tests
+.. image:: https://github.com/mqtt-tools/mqttwarn/workflows/Tests/badge.svg
+    :target: https://github.com/mqtt-tools/mqttwarn/actions?workflow=Tests
 
-.. image:: https://codecov.io/gh/jpmens/mqttwarn/branch/main/graph/badge.svg
-    :target: https://codecov.io/gh/jpmens/mqttwarn
+.. image:: https://codecov.io/gh/mqtt-tools/mqttwarn/branch/main/graph/badge.svg
+    :target: https://codecov.io/gh/mqtt-tools/mqttwarn
 
 .. image:: https://img.shields.io/pypi/pyversions/mqttwarn.svg
     :target: https://pypi.org/project/mqttwarn/
 
 .. image:: https://img.shields.io/pypi/v/mqttwarn.svg
     :target: https://pypi.org/project/mqttwarn/
 
@@ -98,24 +96,31 @@
 
 .. image:: https://img.shields.io/pypi/status/mqttwarn.svg
     :target: https://pypi.org/project/mqttwarn/
 
 .. image:: https://pepy.tech/badge/mqttwarn/month
     :target: https://pepy.tech/project/mqttwarn
 
-.. image:: https://cloud.githubusercontent.com/assets/2345521/6320105/4dd7a826-bade-11e4-9a61-72aa163a40a9.png
+`GitHub <https://github.com/mqtt-tools/mqttwarn>`_
+| `PyPI <https://pypi.org/project/mqttwarn/>`_
+| `Documentation <https://mqttwarn.readthedocs.io>`_
+| `Issues <https://github.com/mqtt-tools/mqttwarn/issues>`_
+| `Changelog <https://github.com/mqtt-tools/mqttwarn/blob/main/CHANGES.rst>`_
+
+|
 
+.. image:: https://cloud.githubusercontent.com/assets/2345521/6320105/4dd7a826-bade-11e4-9a61-72aa163a40a9.png
 
 ########
 mqttwarn
 ########
 
 To *warn*, *alert*, or *notify*.
 
-.. image:: https://raw.githubusercontent.com/jpmens/mqttwarn/main/assets/google-definition.jpg
+.. image:: https://raw.githubusercontent.com/mqtt-tools/mqttwarn/main/assets/google-definition.jpg
 
 
 
 *****
 About
 *****
 
@@ -127,23 +132,23 @@
 
 *mqttwarn* subscribes to any number of MQTT topics and publishes received
 payloads to one or more notification services after optionally applying
 sophisticated transformations.
 
 A picture says a thousand words.
 
-.. image:: https://raw.githubusercontent.com/jpmens/mqttwarn/main/assets/mqttwarn.png
+.. image:: https://raw.githubusercontent.com/mqtt-tools/mqttwarn/main/assets/mqttwarn.png
     :target: #
 
 
 Notification service coverage
 =============================
 
-*mqttwarn* comes with **over 70 notification handler plugins** for a wide
-range of notification services and is very open to further contributions.
+*mqttwarn* comes with **over 70 notification handler plugins**, covering a
+wide range of notification services and is very open to further contributions.
 You can enjoy the alphabetical list of plugins on the `mqttwarn notifier
 catalog`_ page.
 
 On top of that, it integrates with the excellent `Apprise`_ notification
 library. `Apprise notification services`_ has a complete list of the **80+
 notification services** supported by Apprise.
 
@@ -183,16 +188,16 @@
 OCI container image
 ===================
 
 For running ``mqttwarn`` on a container infrastructure like Docker or
 Kubernetes, corresponding images are automatically published to the
 GitHub Container Registry (GHCR).
 
-- ``ghcr.io/jpmens/mqttwarn-standard:latest``
-- ``ghcr.io/jpmens/mqttwarn-full:latest``
+- ``ghcr.io/mqtt-tools/mqttwarn-standard:latest``
+- ``ghcr.io/mqtt-tools/mqttwarn-full:latest``
 
 To learn more about this topic, please follow up reading the `Using the OCI image
 with Docker or Podman`_ documentation section.
 
 
 *************
 Configuration
@@ -202,16 +207,16 @@
 section about the `mqttwarn configuration`_.
 
 
 *****
 Usage
 *****
 
-Running interactively
-=====================
+Interactive service
+===================
 Just launch ``mqttwarn``::
 
     # Run mqttwarn
     mqttwarn
 
 
 To supply a different configuration file or log file, optionally use::
@@ -221,88 +226,54 @@
 
     # Define log file
     export MQTTWARNLOG=/var/log/mqttwarn.log
 
     # Run mqttwarn
     mqttwarn
 
-
-Running notification plugins
-============================
-For debugging, or other purposes, you might want to directly run an individual
-notification plugin without the dispatching and transformation machinery of
-*mqttwarn*.
-
-We have you covered. To launch a plugin standalone, those commands will give
-you an idea how to pass relevant information on the command line using JSON::
-
-    # Launch "log" service plugin
-    mqttwarn --plugin=log --options='{"message": "Hello world", "addrs": ["crit"]}'
-
-    # Launch "file" service plugin
-    mqttwarn --plugin=file --options='{"message": "Hello world\n", "addrs": ["/tmp/mqttwarn.err"]}'
-
-    # Launch "pushover" service plugin
-    mqttwarn --plugin=pushover --options='{"title": "About", "message": "Hello world", "addrs": ["userkey", "token"], "priority": 6}'
-
-    # Launch "ntfy" service plugin
-    mqttwarn --plugin=ntfy --options='{"addrs": {"url": "http://localhost:5555/testdrive"}, "title": "Example notification", "message": "Hello world"}' --data='{"tags": "foo,bar,äöü", "priority": "high"}'
-
-    # Launch "ntfy" service plugin, and add remote attachment
-    mqttwarn --plugin=ntfy --options='{"addrs": {"url": "http://localhost:5555/testdrive"}, "title": "Example notification", "message": "Hello world"}' --data='{"attach": "https://unsplash.com/photos/spdQ1dVuIHw/download?w=320", "filename": "goat.jpg"}'
-
-    # Launch "ntfy" service plugin, and add attachment from local filesystem
-    mqttwarn --plugin=ntfy --options='{"addrs": {"url": "http://localhost:5555/testdrive", "file": "goat.jpg"}, "title": "Example notification", "message": "Hello world"}'
-
-    # Launch "ssh" service plugin
-    mqttwarn --plugin=ssh --config='{"host": "ssh.example.org", "port": 22, "user": "foo", "password": "bar"}' --options='{"addrs": ["command with substitution %s"], "payload": "{\"args\": \"192.168.0.1\"}"}'
-
-    # Launch "cloudflare_zone" service plugin from "mqttwarn-contrib"
-    pip install mqttwarn-contrib
-    mqttwarn --plugin=mqttwarn_contrib.services.cloudflare_zone --config='{"auth-email": "foo", "auth-key": "bar"}' --options='{"addrs": ["0815", "www.example.org", ""], "message": "192.168.0.1"}'
-
-
-Also, the ``--config-file`` parameter can be used to optionally specify the
-path to a configuration file.
-
-
-Running as system daemon
-========================
+System daemon
+=============
 
 There are different ways to run mqttwarn as a system daemon. There are examples
 for systemd, traditional init, OpenRC, and Supervisor_ in the ``etc`` directory
 of this repository, for example `supervisor.ini`_ (Supervisor) and
 `mqttwarn.service`_ (systemd).
 
-Running in a development sandbox
-================================
+Standalone
+==========
+
+In order to directly invoke notification plugins from custom programs, or for
+debugging them, see `Running notification plugins standalone`_.
+
+Development sandbox
+===================
 
 For hacking on mqttwarn, please install it in development mode, using a
 `mqttwarn development sandbox`_ installation.
 
 
 *******************
 Project information
 *******************
 
 About
 =====
 These links will guide you to the source code of *mqttwarn* and its documentation.
 
-- `mqttwarn on GitHub <https://github.com/jpmens/mqttwarn>`_
+- `mqttwarn on GitHub <https://github.com/mqtt-tools/mqttwarn>`_
 - `mqttwarn on the Python Package Index (PyPI) <https://pypi.org/project/mqttwarn/>`_
 - `mqttwarn documentation <https://mqttwarn.readthedocs.io/>`_
 
 
 Requirements
 ============
 You will need at least the following components:
 
 * Python 3.x or PyPy 3.x.
-* An MQTT broker. We recommend `Mosquitto`_.
+* An MQTT broker. We recommend `Eclipse Mosquitto`_.
 * For invoking specific service plugins, additional Python modules may be required.
   See ``setup.py`` file.
 
 
 Contributing
 ============
 
@@ -345,37 +316,37 @@
 Acknowledgements
 ================
 Thanks to all the contributors of *mqttwarn* who helped to conceive it in one
 way or another. You know who you are.
 
 Legal stuff
 ===========
-"MQTT" is a trademark of the OASIS open standards consortium, which publishes
-the MQTT specifications.
-
+"MQTT" is a trademark of the OASIS open standards consortium, which publishes the
+MQTT specifications. "Eclipse Mosquitto" is a trademark of the Eclipse Foundation.
 
 ----
 
 Have fun!
 
 
 .. _Apprise: https://github.com/caronc/apprise
 .. _Apprise notification services: https://github.com/caronc/apprise/wiki#notification-services
-.. _backlog: https://github.com/jpmens/mqttwarn/blob/main/doc/backlog.rst
+.. _backlog: https://github.com/mqtt-tools/mqttwarn/blob/main/doc/backlog.rst
+.. _Eclipse Mosquitto: https://mosquitto.org
 .. _EPL-2.0: https://www.eclipse.org/legal/epl-2.0/
-.. _hacking: https://github.com/jpmens/mqttwarn/blob/main/doc/hacking.rst
+.. _hacking: https://github.com/mqtt-tools/mqttwarn/blob/main/doc/hacking.rst
 .. _How do your servers talk to you?: https://jpmens.net/2014/04/03/how-do-your-servers-talk-to-you/
 .. _Installing mqttwarn with pip: https://mqttwarn.readthedocs.io/en/latest/usage/pip.html
-.. _issue: https://github.com/jpmens/mqttwarn/issues/new
-.. _LICENSE: https://github.com/jpmens/mqttwarn/blob/main/LICENSE
-.. _Mosquitto: https://mosquitto.org
+.. _issue: https://github.com/mqtt-tools/mqttwarn/issues/new
+.. _LICENSE: https://github.com/mqtt-tools/mqttwarn/blob/main/LICENSE
 .. _MQTTwarn\: Ein Rundum-Sorglos-Notifier: https://web.archive.org/web/20140611040637/http://jaxenter.de/news/MQTTwarn-Ein-Rundum-Sorglos-Notifier-171312
 .. _mqttwarn configuration: https://mqttwarn.readthedocs.io/en/latest/configure/
 .. _mqttwarn development sandbox: https://mqttwarn.readthedocs.io/en/latest/workbench/sandbox.html
 .. _mqttwarn documentation: https://mqttwarn.readthedocs.io/
 .. _mqttwarn notifier catalog: https://mqttwarn.readthedocs.io/en/latest/notifier-catalog.html
-.. _mqttwarn.service: https://github.com/jpmens/mqttwarn/blob/main/etc/mqttwarn.service
-.. _opening an issue on GitHub: https://github.com/jpmens/mqttwarn/issues/new
+.. _mqttwarn.service: https://github.com/mqtt-tools/mqttwarn/blob/main/etc/mqttwarn.service
+.. _opening an issue on GitHub: https://github.com/mqtt-tools/mqttwarn/issues/new
+.. _Running notification plugins standalone: https://mqttwarn.readthedocs.io/en/latest/usage/standalone.html
 .. _Schwarmalarm using mqttwarn: https://hiveeyes.org/docs/system/schwarmalarm-mqttwarn.html
 .. _Supervisor: https://jpmens.net/2014/02/13/in-my-toolbox-supervisord/
-.. _supervisor.ini: https://github.com/jpmens/mqttwarn/blob/main/etc/supervisor.ini
+.. _supervisor.ini: https://github.com/mqtt-tools/mqttwarn/blob/main/etc/supervisor.ini
 .. _Using the OCI image with Docker or Podman: https://mqttwarn.readthedocs.io/en/latest/usage/oci.html
```

### Comparing `mqttwarn-0.34.0/README.rst` & `mqttwarn-0.34.1/mqttwarn.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,12 +1,93 @@
-.. image:: https://github.com/jpmens/mqttwarn/workflows/Tests/badge.svg
-    :target: https://github.com/jpmens/mqttwarn/actions?workflow=Tests
+Metadata-Version: 2.1
+Name: mqttwarn
+Version: 0.34.1
+Summary: mqttwarn - subscribe to MQTT topics and notify pluggable services
+Home-page: https://github.com/mqtt-tools/mqttwarn
+Author: Jan-Piet Mens, Ben Jones, Andreas Motl
+Author-email: jpmens@gmail.com
+License: EPL 2.0
+Keywords: mqtt notification plugins data acquisition push transformation engine mosquitto
+Classifier: Development Status :: 4 - Beta
+Classifier: Environment :: Console
+Classifier: Environment :: Plugins
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Education
+Classifier: Intended Audience :: Information Technology
+Classifier: Intended Audience :: Manufacturing
+Classifier: Intended Audience :: Science/Research
+Classifier: Intended Audience :: System Administrators
+Classifier: Intended Audience :: Telecommunications Industry
+Classifier: License :: OSI Approved :: Eclipse Public License 2.0 (EPL-2.0)
+Classifier: Operating System :: POSIX
+Classifier: Operating System :: Unix
+Classifier: Operating System :: MacOS
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Communications
+Classifier: Topic :: Education
+Classifier: Topic :: Internet
+Classifier: Topic :: Internet :: WWW/HTTP
+Classifier: Topic :: Internet :: XMPP
+Classifier: Topic :: Scientific/Engineering :: Interface Engine/Protocol Translator
+Classifier: Topic :: Software Development :: Embedded Systems
+Classifier: Topic :: Software Development :: Libraries
+Classifier: Topic :: Software Development :: Pre-processors
+Classifier: Topic :: Software Development :: Testing
+Classifier: Topic :: System :: Archiving
+Classifier: Topic :: System :: Distributed Computing
+Classifier: Topic :: System :: Monitoring
+Classifier: Topic :: System :: Networking :: Monitoring
+Classifier: Topic :: System :: Systems Administration
+Classifier: Topic :: Text Processing
+Classifier: Topic :: Utilities
+Provides-Extra: amqp
+Provides-Extra: apns
+Provides-Extra: apprise
+Provides-Extra: asterisk
+Provides-Extra: celery
+Provides-Extra: chromecast
+Provides-Extra: dnsupdate
+Provides-Extra: fbchat
+Provides-Extra: gss2
+Provides-Extra: mysql
+Provides-Extra: mysql_dynamic
+Provides-Extra: nsca
+Provides-Extra: desktopnotify
+Provides-Extra: pastebinpub
+Provides-Extra: postgres
+Provides-Extra: prowl
+Provides-Extra: pushbullet
+Provides-Extra: redispub
+Provides-Extra: rrdtool
+Provides-Extra: serial
+Provides-Extra: slack
+Provides-Extra: ssh
+Provides-Extra: tootpaste
+Provides-Extra: twilio
+Provides-Extra: twitter
+Provides-Extra: websocket
+Provides-Extra: xmpp
+Provides-Extra: slixmpp
+Provides-Extra: contrib
+Provides-Extra: all
+Provides-Extra: test
+Provides-Extra: develop
+License-File: LICENSE
 
-.. image:: https://codecov.io/gh/jpmens/mqttwarn/branch/main/graph/badge.svg
-    :target: https://codecov.io/gh/jpmens/mqttwarn
+.. image:: https://github.com/mqtt-tools/mqttwarn/workflows/Tests/badge.svg
+    :target: https://github.com/mqtt-tools/mqttwarn/actions?workflow=Tests
+
+.. image:: https://codecov.io/gh/mqtt-tools/mqttwarn/branch/main/graph/badge.svg
+    :target: https://codecov.io/gh/mqtt-tools/mqttwarn
 
 .. image:: https://img.shields.io/pypi/pyversions/mqttwarn.svg
     :target: https://pypi.org/project/mqttwarn/
 
 .. image:: https://img.shields.io/pypi/v/mqttwarn.svg
     :target: https://pypi.org/project/mqttwarn/
 
@@ -15,24 +96,31 @@
 
 .. image:: https://img.shields.io/pypi/status/mqttwarn.svg
     :target: https://pypi.org/project/mqttwarn/
 
 .. image:: https://pepy.tech/badge/mqttwarn/month
     :target: https://pepy.tech/project/mqttwarn
 
-.. image:: https://cloud.githubusercontent.com/assets/2345521/6320105/4dd7a826-bade-11e4-9a61-72aa163a40a9.png
+`GitHub <https://github.com/mqtt-tools/mqttwarn>`_
+| `PyPI <https://pypi.org/project/mqttwarn/>`_
+| `Documentation <https://mqttwarn.readthedocs.io>`_
+| `Issues <https://github.com/mqtt-tools/mqttwarn/issues>`_
+| `Changelog <https://github.com/mqtt-tools/mqttwarn/blob/main/CHANGES.rst>`_
+
+|
 
+.. image:: https://cloud.githubusercontent.com/assets/2345521/6320105/4dd7a826-bade-11e4-9a61-72aa163a40a9.png
 
 ########
 mqttwarn
 ########
 
 To *warn*, *alert*, or *notify*.
 
-.. image:: https://raw.githubusercontent.com/jpmens/mqttwarn/main/assets/google-definition.jpg
+.. image:: https://raw.githubusercontent.com/mqtt-tools/mqttwarn/main/assets/google-definition.jpg
 
 
 
 *****
 About
 *****
 
@@ -44,23 +132,23 @@
 
 *mqttwarn* subscribes to any number of MQTT topics and publishes received
 payloads to one or more notification services after optionally applying
 sophisticated transformations.
 
 A picture says a thousand words.
 
-.. image:: https://raw.githubusercontent.com/jpmens/mqttwarn/main/assets/mqttwarn.png
+.. image:: https://raw.githubusercontent.com/mqtt-tools/mqttwarn/main/assets/mqttwarn.png
     :target: #
 
 
 Notification service coverage
 =============================
 
-*mqttwarn* comes with **over 70 notification handler plugins** for a wide
-range of notification services and is very open to further contributions.
+*mqttwarn* comes with **over 70 notification handler plugins**, covering a
+wide range of notification services and is very open to further contributions.
 You can enjoy the alphabetical list of plugins on the `mqttwarn notifier
 catalog`_ page.
 
 On top of that, it integrates with the excellent `Apprise`_ notification
 library. `Apprise notification services`_ has a complete list of the **80+
 notification services** supported by Apprise.
 
@@ -100,16 +188,16 @@
 OCI container image
 ===================
 
 For running ``mqttwarn`` on a container infrastructure like Docker or
 Kubernetes, corresponding images are automatically published to the
 GitHub Container Registry (GHCR).
 
-- ``ghcr.io/jpmens/mqttwarn-standard:latest``
-- ``ghcr.io/jpmens/mqttwarn-full:latest``
+- ``ghcr.io/mqtt-tools/mqttwarn-standard:latest``
+- ``ghcr.io/mqtt-tools/mqttwarn-full:latest``
 
 To learn more about this topic, please follow up reading the `Using the OCI image
 with Docker or Podman`_ documentation section.
 
 
 *************
 Configuration
@@ -119,16 +207,16 @@
 section about the `mqttwarn configuration`_.
 
 
 *****
 Usage
 *****
 
-Running interactively
-=====================
+Interactive service
+===================
 Just launch ``mqttwarn``::
 
     # Run mqttwarn
     mqttwarn
 
 
 To supply a different configuration file or log file, optionally use::
@@ -138,88 +226,54 @@
 
     # Define log file
     export MQTTWARNLOG=/var/log/mqttwarn.log
 
     # Run mqttwarn
     mqttwarn
 
-
-Running notification plugins
-============================
-For debugging, or other purposes, you might want to directly run an individual
-notification plugin without the dispatching and transformation machinery of
-*mqttwarn*.
-
-We have you covered. To launch a plugin standalone, those commands will give
-you an idea how to pass relevant information on the command line using JSON::
-
-    # Launch "log" service plugin
-    mqttwarn --plugin=log --options='{"message": "Hello world", "addrs": ["crit"]}'
-
-    # Launch "file" service plugin
-    mqttwarn --plugin=file --options='{"message": "Hello world\n", "addrs": ["/tmp/mqttwarn.err"]}'
-
-    # Launch "pushover" service plugin
-    mqttwarn --plugin=pushover --options='{"title": "About", "message": "Hello world", "addrs": ["userkey", "token"], "priority": 6}'
-
-    # Launch "ntfy" service plugin
-    mqttwarn --plugin=ntfy --options='{"addrs": {"url": "http://localhost:5555/testdrive"}, "title": "Example notification", "message": "Hello world"}' --data='{"tags": "foo,bar,äöü", "priority": "high"}'
-
-    # Launch "ntfy" service plugin, and add remote attachment
-    mqttwarn --plugin=ntfy --options='{"addrs": {"url": "http://localhost:5555/testdrive"}, "title": "Example notification", "message": "Hello world"}' --data='{"attach": "https://unsplash.com/photos/spdQ1dVuIHw/download?w=320", "filename": "goat.jpg"}'
-
-    # Launch "ntfy" service plugin, and add attachment from local filesystem
-    mqttwarn --plugin=ntfy --options='{"addrs": {"url": "http://localhost:5555/testdrive", "file": "goat.jpg"}, "title": "Example notification", "message": "Hello world"}'
-
-    # Launch "ssh" service plugin
-    mqttwarn --plugin=ssh --config='{"host": "ssh.example.org", "port": 22, "user": "foo", "password": "bar"}' --options='{"addrs": ["command with substitution %s"], "payload": "{\"args\": \"192.168.0.1\"}"}'
-
-    # Launch "cloudflare_zone" service plugin from "mqttwarn-contrib"
-    pip install mqttwarn-contrib
-    mqttwarn --plugin=mqttwarn_contrib.services.cloudflare_zone --config='{"auth-email": "foo", "auth-key": "bar"}' --options='{"addrs": ["0815", "www.example.org", ""], "message": "192.168.0.1"}'
-
-
-Also, the ``--config-file`` parameter can be used to optionally specify the
-path to a configuration file.
-
-
-Running as system daemon
-========================
+System daemon
+=============
 
 There are different ways to run mqttwarn as a system daemon. There are examples
 for systemd, traditional init, OpenRC, and Supervisor_ in the ``etc`` directory
 of this repository, for example `supervisor.ini`_ (Supervisor) and
 `mqttwarn.service`_ (systemd).
 
-Running in a development sandbox
-================================
+Standalone
+==========
+
+In order to directly invoke notification plugins from custom programs, or for
+debugging them, see `Running notification plugins standalone`_.
+
+Development sandbox
+===================
 
 For hacking on mqttwarn, please install it in development mode, using a
 `mqttwarn development sandbox`_ installation.
 
 
 *******************
 Project information
 *******************
 
 About
 =====
 These links will guide you to the source code of *mqttwarn* and its documentation.
 
-- `mqttwarn on GitHub <https://github.com/jpmens/mqttwarn>`_
+- `mqttwarn on GitHub <https://github.com/mqtt-tools/mqttwarn>`_
 - `mqttwarn on the Python Package Index (PyPI) <https://pypi.org/project/mqttwarn/>`_
 - `mqttwarn documentation <https://mqttwarn.readthedocs.io/>`_
 
 
 Requirements
 ============
 You will need at least the following components:
 
 * Python 3.x or PyPy 3.x.
-* An MQTT broker. We recommend `Mosquitto`_.
+* An MQTT broker. We recommend `Eclipse Mosquitto`_.
 * For invoking specific service plugins, additional Python modules may be required.
   See ``setup.py`` file.
 
 
 Contributing
 ============
 
@@ -262,37 +316,37 @@
 Acknowledgements
 ================
 Thanks to all the contributors of *mqttwarn* who helped to conceive it in one
 way or another. You know who you are.
 
 Legal stuff
 ===========
-"MQTT" is a trademark of the OASIS open standards consortium, which publishes
-the MQTT specifications.
-
+"MQTT" is a trademark of the OASIS open standards consortium, which publishes the
+MQTT specifications. "Eclipse Mosquitto" is a trademark of the Eclipse Foundation.
 
 ----
 
 Have fun!
 
 
 .. _Apprise: https://github.com/caronc/apprise
 .. _Apprise notification services: https://github.com/caronc/apprise/wiki#notification-services
-.. _backlog: https://github.com/jpmens/mqttwarn/blob/main/doc/backlog.rst
+.. _backlog: https://github.com/mqtt-tools/mqttwarn/blob/main/doc/backlog.rst
+.. _Eclipse Mosquitto: https://mosquitto.org
 .. _EPL-2.0: https://www.eclipse.org/legal/epl-2.0/
-.. _hacking: https://github.com/jpmens/mqttwarn/blob/main/doc/hacking.rst
+.. _hacking: https://github.com/mqtt-tools/mqttwarn/blob/main/doc/hacking.rst
 .. _How do your servers talk to you?: https://jpmens.net/2014/04/03/how-do-your-servers-talk-to-you/
 .. _Installing mqttwarn with pip: https://mqttwarn.readthedocs.io/en/latest/usage/pip.html
-.. _issue: https://github.com/jpmens/mqttwarn/issues/new
-.. _LICENSE: https://github.com/jpmens/mqttwarn/blob/main/LICENSE
-.. _Mosquitto: https://mosquitto.org
+.. _issue: https://github.com/mqtt-tools/mqttwarn/issues/new
+.. _LICENSE: https://github.com/mqtt-tools/mqttwarn/blob/main/LICENSE
 .. _MQTTwarn\: Ein Rundum-Sorglos-Notifier: https://web.archive.org/web/20140611040637/http://jaxenter.de/news/MQTTwarn-Ein-Rundum-Sorglos-Notifier-171312
 .. _mqttwarn configuration: https://mqttwarn.readthedocs.io/en/latest/configure/
 .. _mqttwarn development sandbox: https://mqttwarn.readthedocs.io/en/latest/workbench/sandbox.html
 .. _mqttwarn documentation: https://mqttwarn.readthedocs.io/
 .. _mqttwarn notifier catalog: https://mqttwarn.readthedocs.io/en/latest/notifier-catalog.html
-.. _mqttwarn.service: https://github.com/jpmens/mqttwarn/blob/main/etc/mqttwarn.service
-.. _opening an issue on GitHub: https://github.com/jpmens/mqttwarn/issues/new
+.. _mqttwarn.service: https://github.com/mqtt-tools/mqttwarn/blob/main/etc/mqttwarn.service
+.. _opening an issue on GitHub: https://github.com/mqtt-tools/mqttwarn/issues/new
+.. _Running notification plugins standalone: https://mqttwarn.readthedocs.io/en/latest/usage/standalone.html
 .. _Schwarmalarm using mqttwarn: https://hiveeyes.org/docs/system/schwarmalarm-mqttwarn.html
 .. _Supervisor: https://jpmens.net/2014/02/13/in-my-toolbox-supervisord/
-.. _supervisor.ini: https://github.com/jpmens/mqttwarn/blob/main/etc/supervisor.ini
+.. _supervisor.ini: https://github.com/mqtt-tools/mqttwarn/blob/main/etc/supervisor.ini
 .. _Using the OCI image with Docker or Podman: https://mqttwarn.readthedocs.io/en/latest/usage/oci.html
```

### Comparing `mqttwarn-0.34.0/mqttwarn/commands.py` & `mqttwarn-0.34.1/mqttwarn/commands.py`

 * *Files identical despite different names*

### Comparing `mqttwarn-0.34.0/mqttwarn/configuration.py` & `mqttwarn-0.34.1/mqttwarn/configuration.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # (c) 2014-2023 The mqttwarn developers
 import ast
 import codecs
 import logging
 import os
 import sys
 import typing as t
-from configparser import NoOptionError, RawConfigParser
+from configparser import NoOptionError, NoSectionError, RawConfigParser
 
 from mqttwarn.util import load_functions
 
 HAVE_TLS = True
 try:
     import ssl
 except ImportError:
@@ -84,32 +84,26 @@
         if self.tls_version is not None:
             if self.tls_version == "tlsv1_2":
                 self.tls_version = ssl.PROTOCOL_TLSv1_2
             if self.tls_version == "tlsv1_1":
                 self.tls_version = ssl.PROTOCOL_TLSv1_1
             if self.tls_version == "tlsv1":
                 self.tls_version = ssl.PROTOCOL_TLSv1
-            if self.tls_version == "sslv3":
-                self.tls_version = ssl.PROTOCOL_SSLv3
 
         self.loglevelnumber = self.level2number(self.loglevel)
         self.filteredmessagesloglevelnumber = self.level2number(self.filteredmessagesloglevel)
 
         if self.functions is not None and self.functions.strip() != "":
 
             logger.info("Loading user-defined functions from %s" % self.functions)
 
-            # Load function file as given (backward-compatibility).
+            # Load function file as given.
             if os.path.isfile(self.functions):
                 functions_file = self.functions
 
-            # Load function file as given if path is absolute.
-            elif os.path.isabs(self.functions):
-                functions_file = self.functions
-
             # Load function file relative to path of configuration file if path is relative.
             else:
                 functions_file = os.path.join(self.configuration_path, self.functions)
 
             self.functions = load_functions(functions_file)
 
     def level2number(self, level: str) -> int:
@@ -130,15 +124,15 @@
     def g(self, section: str, key: str, default=None) -> t.Any:
         val = None
         try:
             val = self.get(section, key)
             if isinstance(val, str) and val.upper() in self.specials:
                 return self.specials[val.upper()]
             return ast.literal_eval(val)
-        except NoOptionError:
+        except (NoOptionError, NoSectionError):
             return default
         except ValueError:  # e.g. %(xxx)s in string
             return val
         except SyntaxError:  # If not python value, e.g. list of targets coma separated
             return val
         except:
             raise
@@ -171,23 +165,28 @@
             [config:mqtt]
             host = 'localhost'
             username = None
             list = [1, 'aaa', 'bbb', 4]
 
         into
 
-            {u'username': None, u'host': 'localhost', u'list': [1, 'aaa', 'bbb', 4]}
+            {'username': None, 'host': 'localhost', 'list': [1, 'aaa', 'bbb', 4]}
 
         Cannot use config.items() because I want each value to be
         retrieved with g() as above"""
 
-        d = {}
         if self.has_section(section):
-            d = dict((key, self.g(section, key)) for (key) in self.options(section) if key not in ["targets", "module"])
-        return d
+            return dict(
+                (key, self.g(section, key)) for (key) in self.options(section) if key not in ["targets", "module"]
+            )
+        else:
+            if section == "defaults":
+                return {}
+            else:
+                raise KeyError(f"Configuration section does not exist: {section}")
 
 
 def load_configuration(configfile: t.Optional[str] = None, name: str = "mqttwarn") -> Config:
 
     if configfile is None:
         configfile = str(os.getenv(name.upper() + "INI", name + ".ini"))
```

### Comparing `mqttwarn-0.34.0/mqttwarn/context.py` & `mqttwarn-0.34.1/mqttwarn/context.py`

 * *Files 4% similar despite different names*

```diff
@@ -108,23 +108,19 @@
 
     def get_service_targets(self, service: str) -> t.List[TopicTargetType]:
         """
         Resolve target address descriptor.
 
         2021-10-18 [amo]: Be more graceful with jobs w/o any target address information.
         """
-        targets: t.List[TopicTargetType] = []
-        try:
-            targets = self.config.getdict("config:" + service, "targets")
-        except:
-            logger.exception("Unable to access targets for service `%s'" % service)
+        targets: t.List[TopicTargetType] = self.config.getdict("config:" + service, "targets")
 
         # TODO: The target address descriptor may be of any type these days,
         #       and not necessarily a list.
-        # TODO: Currently, this makes sure to always return one element.
+        # TODO: Currently, make sure to always return one element.
         #       Verify if this is really needed.
         targets = targets or [None]
         return targets
 
 
 @attr.s
 class FunctionInvoker:
```

### Comparing `mqttwarn-0.34.0/mqttwarn/core.py` & `mqttwarn-0.34.1/mqttwarn/core.py`

 * *Files 3% similar despite different names*

```diff
@@ -51,21 +51,23 @@
 logger = logging.getLogger(__name__)
 
 # Name of calling program
 SCRIPTNAME = "mqttwarn"
 
 # Global runtime context object
 context: RuntimeContext
+context = None  # type: ignore[assignment]
 
 # Global configuration object
 cf: mqttwarn.configuration.Config
+cf = None  # type: ignore[assignment]
 
 # Global handle to MQTT client
 mqttc: paho.Client
-mqttc = None
+mqttc = None  # type: ignore[assignment]
 
 # Initialize processor queue
 q_in: Queue = Queue(maxsize=0)
 exit_flag = False
 
 # Instances of PeriodicThread objects
 ptlist: t.Dict[str, PeriodicThread] = {}
@@ -230,27 +232,27 @@
     except:
         pass
     dispatcher_dict = cf.getdict(section, "targets")
 
     # `targets` is a function symbol.
     if function_name is not None:
         targetlist = context.get_topic_targets(section, topic, data)
-        # TODO: Verify if this is still the case. @amotl thinks that the
-        #       target address descriptor may be of any type these days.
+
+        # Make sure the function returned a target _list_ of elements.
         if not isinstance(targetlist, list):
             targetlist_type = type(targetlist)
             logger.error(
                 'Topic target definition by function "{function_name}" '
                 'in section "{section}" is empty or incorrect. Should be a list. '
                 "targetlist={targetlist}, type={targetlist_type}".format(**locals())
             )
             return
 
     # `targets` is a dictionary.
-    elif isinstance(dispatcher_dict, dict):
+    elif isinstance(dispatcher_dict, dict) and dispatcher_dict:
 
         def get_key(item):
             # precede a key with the number of topic levels and then use reverse alphabetic sort order
             # '+' is after '#' in ascii table
             # caveat: for instance space is allowed in topic name but will be less specific than '+', '#'
             # so replace '#' with first ascii character and '+' with second ascii character
             # http://public.dhe.ibm.com/software/dw/webservices/ws-mqtt/mqtt-v3r1.html#appendix-a
@@ -274,34 +276,36 @@
             # Not found then no action. This could be configured intentionally.
             logger.debug("Dispatcher definition does not contain matching topic/target pair in section [%s]" % section)
             return
 
     else:
         targetlist = cf.getlist(section, "targets")
 
-        # Exit if `targets` is not a `list`.
+        # Make sure targets are actually a _list_ of elements.
         # TODO: Not tested yet. How can this code be reached?
-        if not isinstance(targetlist, list):
-            logger.error("Target definition in section [%s] is incorrect, should be dictionary or list." % section)
-            # TODO: Review this.
-            cleanup(0)
+        if targetlist is None:
+            logger.error(
+                f'Topic target definition in section "{section}" is empty or incorrect. Should be a list. '
+                "targetlist={targetlist}".format(**locals())
+            )
             return
 
-    # interpolate transformation data values into topic targets
-    # be graceful if interpolation fails, but log a meaningful message
+    # Interpolate transformation data values into topic targets.
+    # Be graceful if interpolation fails, but log a meaningful message.
     targetlist_resolved = []
     for target in targetlist:
         try:
             target = target.format(**data)
             targetlist_resolved.append(target)
         except Exception as ex:
             error = repr(ex)
             logger.error(
-                f"Cannot interpolate transformation data into topic target '{target}': {error}. "
-                f"section={section}, topic={topic}, payload={truncate(payload)}, data={data}"
+                f"Interpolating transformation data into topic target '{target}' failed. Reason: {error}. "
+                f"section={section}, topic={topic}, payload={truncate(payload)}, data=%s",
+                data,
             )
     targetlist = targetlist_resolved
 
     for item in targetlist:
         logger.debug("Message on %s going to %s" % (topic, item))
         # Each target is either "service" or "service:target"
         # If no target specified then notify ALL targets
@@ -309,18 +313,18 @@
         target = None
 
         # Check if this is for a specific target
         if item.find(":") != -1:
             try:
                 service, target = item.split(":", 2)
             except:
-                logger.warning("Invalid target %s - should be 'service:target'" % (item))
+                logger.error(f"Invalid topic target: {item}. Should be 'service:target'.")
                 continue
 
-        # skip targets with invalid services
+        # Skip targets with invalid services.
         if service not in service_plugins:
             logger.error("Invalid configuration: Topic '%s' points to non-existing service '%s'" % (topic, service))
             continue
 
         service_config = context.get_service_config(service)
         payload_out: t.Union[str, bytes]
         if asbool(service_config.get("decode_utf8", True)) and isinstance(payload, bytes):
@@ -373,23 +377,23 @@
 
     if function is not None:
         try:
             function_name = sanitize_function_name(function)
             try:
                 res = context.invoker.datamap(function_name, transform_data)
                 return res
-            except Exception:
-                logger.exception(f"Invoking function '{function}' failed")
+            except:
+                logger.exception(f"Invoking function failed: {function}")
         except:
             pass
 
         try:
             res = Formatter().format(function, **transform_data)
-        except Exception:
-            logger.exception(f"Formatting message with function '{function}' failed")
+        except:
+            logger.exception(f"Formatting message with function failed: {function}")
 
     if isinstance(res, str):
         res = res.replace("\\n", "\n")
 
     return res
 
 
@@ -433,18 +437,28 @@
 
 
 def processor(worker_id=None):
     """
     Queue runner. Pull a job from the queue, find the module in charge
     of handling the service, and invoke the module's plugin to do so.
     """
-
     while not exit_flag:
         logger.debug("Job queue has %s items to process" % q_in.qsize())
         job = q_in.get()
+        if process_job(job=job, worker_id=worker_id):
+            q_in.task_done()
+    logger.debug("Worker thread exiting")
+
+
+def process_job(job, worker_id=None):
+    """
+    Process a single job item.
+    """
+
+    if True:
 
         service = job.service
         section = job.section
         target = job.target
         topic = job.topic
 
         logger.debug("Processor #%s is handling: `%s' for %s" % (worker_id, service, target))
@@ -461,16 +475,15 @@
                     "Invalid configuration: Topic '{topic}' points to "
                     "non-existing target '{target}' in service '{service}'".format(**locals())
                 )
                 raise KeyError(error_message)
 
         except Exception:
             logger.exception(f"Cannot handle service={service}, target={target}")
-            q_in.task_done()
-            continue
+            return True
 
         # Be more graceful with jobs w/o any target address information (2021-10-18 [amo]).
         if target is None:
             addrs = []
         else:
             addrs = service_targets[target]
 
@@ -495,30 +508,30 @@
         origin_title = "{}: {}".format(SCRIPTNAME, topic)
         item["title"] = xform(context.get_config(section, "title"), origin_title, transform_data)
         item["image"] = xform(context.get_config(section, "image"), "", transform_data)
         item["message"] = xform(context.get_config(section, "format"), job.payload, transform_data)
 
         try:
             item["priority"] = int(xform(context.get_config(section, "priority"), 0, transform_data))
-        except Exception as e:
+        except:
             item["priority"] = 0
-            logger.warning("Failed to determine the priority, defaulting to zero: %s" % e)
+            logger.exception("Failed to determine the priority, defaulting to zero")
 
         if HAVE_JINJA is False and context.get_config(section, "template"):
             logger.warning("Templating not possible because Jinja2 is not installed")
 
         if HAVE_JINJA is True:
             template = context.get_config(section, "template")
             if template is not None:
                 try:
                     text = render_template(template, transform_data)
                     if text is not None:
                         item["message"] = text
-                except Exception as e:
-                    logger.warning("Cannot render `%s' template: %s" % (template, e))
+                except:
+                    logger.exception(f"Rendering template failed: {template}")
 
         if item.get("message") is not None and len(item.get("message")) > 0:
             st = Struct(**item)
             notified = False
             logger.info("Invoking service plugin for `%s'" % service)
             try:
                 # Fire the plugin in a separate thread and kill it if it doesn't return in 10s
@@ -526,40 +539,34 @@
                 if "." in service:
                     service_logger_name = service
                 else:
                     service_logger_name = "mqttwarn.services.{}".format(service)
                 srv = make_service(mqttc=mqttc, name=service_logger_name)
                 notified = timeout(module.plugin, (srv, st))
             except Exception as ex:
-                logger.exception(f"Invoking service '{service}' failed: {ex}")
+                logger.exception(f"Invoking service failed. Reason: {ex}. service={service}, topic={topic}")
 
             if not notified:
-                logger.warning("Notification of %s for `%s' FAILED or TIMED OUT" % (service, item.get("topic")))
+                logger.warning(f"Notification failed or timed out. service={service}, topic={topic}")
         else:
-            logger.warning("Notification of %s for `%s' suppressed: text is empty" % (service, item.get("topic")))
+            logger.info(f"Notification suppressed. Reason: Payload is empty. service={service}, topic={topic}")
 
-        q_in.task_done()
-
-    logger.debug("Thread exiting")
+        return True
 
 
 def load_services(services):
 
     if services is None:
         logger.warning("No services defined")
         return
 
     for service in services:
         service_plugins[service] = {}
 
         service_config = cf.config("config:" + service)
-        if service_config is None:
-            logger.error("Service `%s' has no config section" % service)
-            sys.exit(1)
-
         service_plugins[service]["config"] = service_config
 
         module = cf.g("config:" + service, "module", service)
 
         # Load external service from file.
         modulefile_candidates = []
         if module.endswith(".py"):
@@ -571,46 +578,47 @@
         # Load external service with module specification.
         elif "." in module:
             logger.debug('Trying to load service "{}" from module "{}"'.format(service, module))
             try:
                 service_plugins[service]["module"] = load_module_by_name(module)
                 logger.info('Successfully loaded service "{}" from module "{}"'.format(service, module))
                 continue
-            except Exception:
+            except:
                 logger.exception('Loading service "{}" from module "{}" failed'.format(service, module))
 
         # Load built-in service module.
         else:
             # Backward-compatibility patch for honoring the renaming of the `http.py` module.
             if module == "http":
                 module = "http_urllib"
             logger.debug('Trying to load built-in service "{}" from "{}"'.format(service, module))
             modulefile_candidates = [resource_filename("mqttwarn.services", module + ".py")]
 
         success = False
         for modulefile in modulefile_candidates:
             if not os.path.isfile(modulefile):
+                logger.error('Module "{}" is not a file'.format(modulefile))
                 continue
             logger.debug('Trying to load service "{}" from file "{}"'.format(service, modulefile))
             try:
                 service_plugins[service]["module"] = load_module_from_file(modulefile)
                 logger.info('Successfully loaded service "{}"'.format(service))
                 success = True
-            except Exception:
+            except:
                 logger.exception(f'Loading service "{service}" from file "{modulefile}" failed')
 
         if not success:
             logger.critical('Unable to load service "{}"'.format(service))
             # TODO: Review this.
             sys.exit(1)
 
 
 def connect():
     """
-    Load service plugins, connect to the broker, launch daemon threads and listen forever
+    Load service plugins, connect to the MQTT broker, launch daemon threads, and listen forever.
     """
 
     # FIXME: Remove global variables
     global mqttc
 
     try:
         services = cf.getlist("defaults", "launch")
@@ -796,15 +804,15 @@
     invoker = FunctionInvoker(config=config, srv=make_service(mqttc=None, name="mqttwarn.context"))
     context = RuntimeContext(config=config, invoker=invoker)
     cf = config
     if scriptname is not None:
         SCRIPTNAME = scriptname
 
 
-def run_plugin(config=None, name=None, options=None, data=None):
+def run_plugin(config=None, name=None, options=None, data=None, message=None):
     """
     Run service plugins directly without the
     dispatching and transformation machinery.
 
     On the one hand, this might look like a bit of a hack.
     On the other hand, it shows very clearly how some of
     the innards of mqttwarn interact so it might also please
@@ -824,20 +832,22 @@
     if "." in name:
         service_logger_name = name
     else:
         service_logger_name = "mqttwarn.services.{}".format(name)
     srv = make_service(mqttc=None, name=service_logger_name)
 
     # Build a mimikry item instance for feeding to the service plugin
-    item = Struct(**options)
+    item = Struct(**options or {})
     # TODO: Read configuration optionally from data.
     item.config = config.config("config:" + name)
     item.service = srv
     item.target = "mqttwarn"
     item.data = data or {}
+    if not hasattr(item, "message"):
+        item.message = message
 
     # Launch plugin
     module = service_plugins[name]["module"]
     response = module.plugin(srv, item)
     logger.info("Plugin response: {}".format(response))
     if response is False:
         sys.exit(1)
```

### Comparing `mqttwarn-0.34.0/mqttwarn/cron.py` & `mqttwarn-0.34.1/mqttwarn/cron.py`

 * *Files identical despite different names*

### Comparing `mqttwarn-0.34.0/mqttwarn/examples/basic/mqttwarn.ini` & `mqttwarn-0.34.1/mqttwarn/examples/basic/mqttwarn.ini`

 * *Files 4% similar despite different names*

```diff
@@ -94,15 +94,15 @@
 ; ------------------------------------------
 ;                  Basic
 ; ------------------------------------------
 
 [hello/1]
 ; echo '{"name": "temperature", "number": 42.42}' | mosquitto_pub -h localhost -t hello/1 -l
 targets = log:info
-format = u'{name}: {number} => {_dthhmm}'
+format = '{name}: {number} => {_dthhmm}'
 
 
 ; ------------------------------------------
 ;                OwnTracks
 ; ------------------------------------------
 
 [owntracks-location]
```

### Comparing `mqttwarn-0.34.0/mqttwarn/examples/basic/udf.py` & `mqttwarn-0.34.1/mqttwarn/examples/basic/udf.py`

 * *Files identical despite different names*

### Comparing `mqttwarn-0.34.0/mqttwarn/model.py` & `mqttwarn-0.34.1/mqttwarn/model.py`

 * *Files 14% similar despite different names*

```diff
@@ -55,28 +55,40 @@
     """
     Data container for feeding information into service plugins - V2.
     """
 
     service: Optional[str] = None
     target: Optional[str] = None
     config: Dict = field(default_factory=dict)
+    section: Optional[str] = None
     # TODO: `addrs` can also be a string or dictionary now.
     addrs: TopicTargetType = field(default_factory=list)  # type: ignore[assignment]
     priority: Optional[int] = None
     topic: Optional[str] = None
     title: Optional[str] = None
     message: Optional[Union[str, bytes]] = None
     data: Optional[Dict] = None
 
     def asdict(self):
         return dataclasses.asdict(self)
 
     def get(self, key, default=None):
         return getattr(self, key, default)
 
+    def to_job(self) -> "Job":
+        return Job(
+            prio=self.priority,
+            service=self.service,
+            section=self.section,
+            topic=self.topic,
+            payload=self.message,
+            data=self.data,
+            target=self.target,
+        )
+
 
 @dataclasses.dataclass
 class StatusInformation:
     """
     Different bits of information published to `mqttwarn/$SYS` when the `status_publish` feature is enabled.
     """
```

### Comparing `mqttwarn-0.34.0/mqttwarn/services/alexa-notify-me.py` & `mqttwarn-0.34.1/mqttwarn/services/alexa-notify-me.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 """
 __author__    = 'Bram Hendrickx'
 __copyright__ = 'Copyright 2016 Bram Hendrickx'
 __license__   = 'Eclipse Public License - v 1.0 (http://www.eclipse.org/legal/epl-v10.html)'
 
-Original script by Bram Hendrickx. https://github.com/jpmens/mqttwarn/blob/main/mqttwarn/services/ifttt.py
+Original script by Bram Hendrickx. https://github.com/mqtt-tools/mqttwarn/blob/main/mqttwarn/services/ifttt.py
 Modified to work with notify-me app for Alexa. http://www.thomptronics.com/notify-me
 """
 
 __author__ = 'Michael Brougham'
 __copyright__ = 'Copyright 2018 Michael Brougham'
 __license__ = 'Eclipse Public License - v 1.0 (http://www.eclipse.org/legal/epl-v10.html)'
```

### Comparing `mqttwarn-0.34.0/mqttwarn/services/amqp.py` & `mqttwarn-0.34.1/mqttwarn/services/amqp.py`

 * *Files identical despite different names*

### Comparing `mqttwarn-0.34.0/mqttwarn/services/apns.py` & `mqttwarn-0.34.1/mqttwarn/services/apns.py`

 * *Files identical despite different names*

### Comparing `mqttwarn-0.34.0/mqttwarn/services/apprise_multi.py` & `mqttwarn-0.34.1/mqttwarn/services/apprise_multi.py`

 * *Files identical despite different names*

### Comparing `mqttwarn-0.34.0/mqttwarn/services/apprise_single.py` & `mqttwarn-0.34.1/mqttwarn/services/apprise_single.py`

 * *Files identical despite different names*

### Comparing `mqttwarn-0.34.0/mqttwarn/services/apprise_util.py` & `mqttwarn-0.34.1/mqttwarn/services/apprise_util.py`

 * *Files identical despite different names*

### Comparing `mqttwarn-0.34.0/mqttwarn/services/asterisk.py` & `mqttwarn-0.34.1/mqttwarn/services/asterisk.py`

 * *Files identical despite different names*

### Comparing `mqttwarn-0.34.0/mqttwarn/services/autoremote.py` & `mqttwarn-0.34.1/mqttwarn/services/autoremote.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 """
 __author__    = 'Bram Hendrickx'
 __copyright__ = 'Copyright 2016 Bram Hendrickx'
 __license__   = 'Eclipse Public License - v 1.0 (http://www.eclipse.org/legal/epl-v10.html)'
 
-Original script by Bram Hendrickx. https://github.com/jpmens/mqttwarn/blob/main/mqttwarn/services/ifttt.py
+Original script by Bram Hendrickx. https://github.com/mqtt-tools/mqttwarn/blob/main/mqttwarn/services/ifttt.py
 Modified to work with the autoremote api https://joaoapps.com/autoremote/
 """
 
 __author__    = 'Michael Brougham'
 __copyright__ = 'Copyright 2018 Michael Brougham'
 __license__   = 'Eclipse Public License - v 1.0 (http://www.eclipse.org/legal/epl-v10.html)'
```

### Comparing `mqttwarn-0.34.0/mqttwarn/services/azure_iot.py` & `mqttwarn-0.34.1/mqttwarn/services/azure_iot.py`

 * *Files identical despite different names*

### Comparing `mqttwarn-0.34.0/mqttwarn/services/carbon.py` & `mqttwarn-0.34.1/mqttwarn/services/carbon.py`

 * *Files identical despite different names*

### Comparing `mqttwarn-0.34.0/mqttwarn/services/celery.py` & `mqttwarn-0.34.1/mqttwarn/services/celery.py`

 * *Files identical despite different names*

### Comparing `mqttwarn-0.34.0/mqttwarn/services/chromecast.py` & `mqttwarn-0.34.1/mqttwarn/services/chromecast.py`

 * *Files identical despite different names*

### Comparing `mqttwarn-0.34.0/mqttwarn/services/dbus.py` & `mqttwarn-0.34.1/mqttwarn/services/dbus.py`

 * *Files identical despite different names*

### Comparing `mqttwarn-0.34.0/mqttwarn/services/desktopnotify.py` & `mqttwarn-0.34.1/mqttwarn/services/desktopnotify.py`

 * *Files identical despite different names*

### Comparing `mqttwarn-0.34.0/mqttwarn/services/dnsupdate.py` & `mqttwarn-0.34.1/mqttwarn/services/dnsupdate.py`

 * *Files identical despite different names*

### Comparing `mqttwarn-0.34.0/mqttwarn/services/emoncms.py` & `mqttwarn-0.34.1/mqttwarn/services/emoncms.py`

 * *Files identical despite different names*

### Comparing `mqttwarn-0.34.0/mqttwarn/services/execute.py` & `mqttwarn-0.34.1/mqttwarn/services/execute.py`

 * *Files 13% similar despite different names*

```diff
@@ -16,13 +16,13 @@
     else:
         replace = '[TEXT]'
 
     text = item.message
     cmd = [i.replace(replace, text) for i in item.addrs]
 
     try:
-        res = subprocess.check_output(cmd, stdin=None, stderr=subprocess.STDOUT, shell=False, universal_newlines=True, cwd='/tmp')
+        subprocess.check_call(cmd, stdin=None, stderr=subprocess.STDOUT, shell=False, universal_newlines=True, cwd='/tmp')
     except Exception as e:
         srv.logging.warning("Cannot execute %s because %s" % (cmd, e))
         return False
 
     return True
```

### Comparing `mqttwarn-0.34.0/mqttwarn/services/fbchat.py` & `mqttwarn-0.34.1/mqttwarn/services/fbchat.py`

 * *Files identical despite different names*

### Comparing `mqttwarn-0.34.0/mqttwarn/services/file.py` & `mqttwarn-0.34.1/mqttwarn/services/file.py`

 * *Files identical despite different names*

### Comparing `mqttwarn-0.34.0/mqttwarn/services/freeswitch.py` & `mqttwarn-0.34.1/mqttwarn/services/freeswitch.py`

 * *Files identical despite different names*

### Comparing `mqttwarn-0.34.0/mqttwarn/services/gss2.py` & `mqttwarn-0.34.1/mqttwarn/services/gss2.py`

 * *Files identical despite different names*

### Comparing `mqttwarn-0.34.0/mqttwarn/services/hangbot.py` & `mqttwarn-0.34.1/mqttwarn/services/hangbot.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 """
 __author__    = 'Bram Hendrickx'
 __copyright__ = 'Copyright 2016 Bram Hendrickx'
 __license__   = 'Eclipse Public License - v 1.0 (http://www.eclipse.org/legal/epl-v10.html)'
 
-Original script by Bram Hendrickx. https://github.com/jpmens/mqttwarn/blob/main/mqttwarn/services/ifttt.py
+Original script by Bram Hendrickx. https://github.com/mqtt-tools/mqttwarn/blob/main/mqttwarn/services/ifttt.py
 Modified to work with hangoutsbot api plugin https://github.com/hangoutsbot/hangoutsbot/wiki/API-Plugin
 """
 
 __author__    = 'Michael Brougham'
 __copyright__ = 'Copyright 2018 Michael Brougham'
 __license__   = 'Eclipse Public License - v 1.0 (http://www.eclipse.org/legal/epl-v10.html)'
```

### Comparing `mqttwarn-0.34.0/mqttwarn/services/hipchat.py` & `mqttwarn-0.34.1/mqttwarn/services/xbmc.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,53 +1,67 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
-__author__    = 'Leonardo Rizzi <l.rizzi()wide-net.org>'
-__copyright__ = 'Copyright 2017 Leonardo Rizzi'
+__author__    = 'Ben Jones <ben.jones12()gmail.com>'
+__copyright__ = 'Copyright 2014 Ben Jones'
 __license__   = 'Eclipse Public License - v 1.0 (http://www.eclipse.org/legal/epl-v10.html)'
 
 from future import standard_library
 standard_library.install_aliases()
-from builtins import str
 
 import urllib.request, urllib.parse, urllib.error
+import base64
 try:
     import simplejson as json
 except ImportError:
     import json  # type: ignore[no-redef]
 
 
 def plugin(srv, item):
-    """ addrs: (token, roomid, color, notify) """
 
     srv.logging.debug("*** MODULE=%s: service=%s, target=%s", __file__, item.service, item.target)
 
-    token   = item.addrs[0]
-    roomid  = item.addrs[1]
-    color   = item.addrs[2]
-    notify  = item.addrs[3]
-    timeout = item.config.get('timeout', 60)
-    server  = item.config.get('server', 'api.hipchat.com')
+    xbmchost = item.addrs[0]
+    xbmcusername = None
+    xbmcpassword = None
+
+    if len(item.addrs) == 3:
+        xbmcusername = item.addrs[1]
+        xbmcpassword = item.addrs[2]
 
-    url = 'https://' + str(server) + '/v2/room/' + str(roomid) + '/notification'
+    title    = item.title
     message  = item.message
+    image    = item.image
 
-    try:
-        headers = {
-                'Content-Type': 'application/json',
-                'Authorization': 'Bearer %s' % token}
-
-        datastr = json.dumps({
-                'message': message,
-                'color': color,
-                'message_format': 'html',
-                'notify': notify})
-
-        request = urllib.request.Request(url, headers=headers, data=datastr.encode("utf-8"))
-        resp = urllib.request.urlopen(request, timeout=timeout)
-        data = resp.read()
+    jsonparams = {
+        "jsonrpc" : "2.0",
+        "method"  : "GUI.ShowNotification",
+        "id"      : 1,
+        "params"  : {
+            "title"       : title,
+            "message"     : message,
+            "image"       : image,
+            "displaytime" : 10000
+        }
+    }
+    jsoncommand = json.dumps(jsonparams).encode("utf-8")
 
+    url = 'http://%s/jsonrpc' % (xbmchost)
+    try:
+        srv.logging.debug("Sending XBMC notification to %s [%s]..." % (item.target, xbmchost))
+        req = urllib.request.Request(url, jsoncommand)
+        req.add_header("Content-type", "application/json")
+        if xbmcpassword is not None:
+            credentials = '%s:%s' % (xbmcusername, xbmcpassword)
+            basicauth_token = base64.b64encode(credentials.encode('utf-8')).decode()
+            authheader = "Basic %s" % basicauth_token
+            req.add_header("Authorization", authheader)
+        response = urllib.request.urlopen(req, timeout = 2)
+        srv.logging.debug("Successfully sent XBMC notification")
+    except urllib.error.URLError as e:
+        srv.logging.error("URLError: %s" % e)
+        return False
     except Exception as e:
-        srv.logging.warn("Cannot POST %s: %s" % (url, e))
+        srv.logging.error("Error sending XBMC notification to %s [%s]: %s" % (item.target, xbmchost, e))
         return False
 
     return True
```

### Comparing `mqttwarn-0.34.0/mqttwarn/services/http_urllib.py` & `mqttwarn-0.34.1/mqttwarn/services/http_urllib.py`

 * *Files identical despite different names*

### Comparing `mqttwarn-0.34.0/mqttwarn/services/icinga2.py` & `mqttwarn-0.34.1/mqttwarn/services/icinga2.py`

 * *Files identical despite different names*

### Comparing `mqttwarn-0.34.0/mqttwarn/services/ifttt.py` & `mqttwarn-0.34.1/mqttwarn/services/ifttt.py`

 * *Files identical despite different names*

### Comparing `mqttwarn-0.34.0/mqttwarn/services/influxdb.py` & `mqttwarn-0.34.1/mqttwarn/services/influxdb.py`

 * *Files identical despite different names*

### Comparing `mqttwarn-0.34.0/mqttwarn/services/ionic.py` & `mqttwarn-0.34.1/mqttwarn/services/ionic.py`

 * *Files identical despite different names*

### Comparing `mqttwarn-0.34.0/mqttwarn/services/irccat.py` & `mqttwarn-0.34.1/mqttwarn/services/irccat.py`

 * *Files 5% similar despite different names*

```diff
@@ -27,15 +27,15 @@
         color = '%RED'
     if color is not None:
         message = color + message
 
     srv.logging.debug("Sending to IRCcat: %s" % (message))
 
     # Apparently, a trailing newline is needed.
-    # https://github.com/jpmens/mqttwarn/issues/547#issuecomment-944632712
+    # https://github.com/mqtt-tools/mqttwarn/issues/547#issuecomment-944632712
     message += "\n"
 
     try:
         sock = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
         sock.connect((addr, port))
         sock.send(message.encode())
         sock.close()
```

### Comparing `mqttwarn-0.34.0/mqttwarn/services/linuxnotify.py` & `mqttwarn-0.34.1/mqttwarn/services/linuxnotify.py`

 * *Files identical despite different names*

### Comparing `mqttwarn-0.34.0/mqttwarn/services/log.py` & `mqttwarn-0.34.1/mqttwarn/services/log.py`

 * *Files identical despite different names*

### Comparing `mqttwarn-0.34.0/mqttwarn/services/mattermost.py` & `mqttwarn-0.34.1/mqttwarn/services/mattermost.py`

 * *Files identical despite different names*

### Comparing `mqttwarn-0.34.0/mqttwarn/services/mqtt.py` & `mqttwarn-0.34.1/mqttwarn/services/mqtt.py`

 * *Files identical despite different names*

### Comparing `mqttwarn-0.34.0/mqttwarn/services/mqtt_filter.py` & `mqttwarn-0.34.1/mqttwarn/services/mqtt_filter.py`

 * *Files identical despite different names*

### Comparing `mqttwarn-0.34.0/mqttwarn/services/mqttpub.py` & `mqttwarn-0.34.1/mqttwarn/services/mqttpub.py`

 * *Files identical despite different names*

### Comparing `mqttwarn-0.34.0/mqttwarn/services/mysql.py` & `mqttwarn-0.34.1/mqttwarn/services/mysql.py`

 * *Files identical despite different names*

### Comparing `mqttwarn-0.34.0/mqttwarn/services/mysql_dynamic.py` & `mqttwarn-0.34.1/mqttwarn/services/mysql_dynamic.py`

 * *Files identical despite different names*

### Comparing `mqttwarn-0.34.0/mqttwarn/services/mysql_remap.py` & `mqttwarn-0.34.1/mqttwarn/services/mysql_remap.py`

 * *Files identical despite different names*

### Comparing `mqttwarn-0.34.0/mqttwarn/services/mythtv.py` & `mqttwarn-0.34.1/mqttwarn/services/mythtv.py`

 * *Files identical despite different names*

### Comparing `mqttwarn-0.34.0/mqttwarn/services/nntp.py` & `mqttwarn-0.34.1/mqttwarn/services/nntp.py`

 * *Files identical despite different names*

### Comparing `mqttwarn-0.34.0/mqttwarn/services/nsca.py` & `mqttwarn-0.34.1/mqttwarn/services/nsca.py`

 * *Files identical despite different names*

### Comparing `mqttwarn-0.34.0/mqttwarn/services/ntfy.py` & `mqttwarn-0.34.1/mqttwarn/services/ntfy.py`

 * *Files identical despite different names*

### Comparing `mqttwarn-0.34.0/mqttwarn/services/osxsay.py` & `mqttwarn-0.34.1/mqttwarn/services/osxsay.py`

 * *Files identical despite different names*

### Comparing `mqttwarn-0.34.0/mqttwarn/services/pastebinpub.py` & `mqttwarn-0.34.1/mqttwarn/services/pastebinpub.py`

 * *Files identical despite different names*

### Comparing `mqttwarn-0.34.0/mqttwarn/services/pipe.py` & `mqttwarn-0.34.1/mqttwarn/services/pipe.py`

 * *Files identical despite different names*

### Comparing `mqttwarn-0.34.0/mqttwarn/services/postgres.py` & `mqttwarn-0.34.1/mqttwarn/services/postgres.py`

 * *Files identical despite different names*

### Comparing `mqttwarn-0.34.0/mqttwarn/services/prowl.py` & `mqttwarn-0.34.1/mqttwarn/services/prowl.py`

 * *Files identical despite different names*

### Comparing `mqttwarn-0.34.0/mqttwarn/services/pushbullet.py` & `mqttwarn-0.34.1/mqttwarn/services/pushbullet.py`

 * *Files identical despite different names*

### Comparing `mqttwarn-0.34.0/mqttwarn/services/pushover.py` & `mqttwarn-0.34.1/mqttwarn/services/pushover.py`

 * *Files identical despite different names*

### Comparing `mqttwarn-0.34.0/mqttwarn/services/pushsafer.py` & `mqttwarn-0.34.1/mqttwarn/services/pushsafer.py`

 * *Files identical despite different names*

### Comparing `mqttwarn-0.34.0/mqttwarn/services/redispub.py` & `mqttwarn-0.34.1/mqttwarn/services/redispub.py`

 * *Files identical despite different names*

### Comparing `mqttwarn-0.34.0/mqttwarn/services/rrdtool.py` & `mqttwarn-0.34.1/mqttwarn/services/rrdtool.py`

 * *Files 12% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
     try:
         # addrs is a list[] associated with a particular target.
         # it can contain an arbitrary amount of entries that are just
         # passed along to rrdtool
         # mofified by otfdr @ github to accept abitray arguments with
         # the payload and to not always add the 'N' in front
-        # 2017-06-05 - fix/enhancement for https://github.com/jpmens/mqttwarn/issues/248
+        # 2017-06-05 - fix/enhancement for https://github.com/mqtt-tools/mqttwarn/issues/248
         if re.match( "^\d+$", text ):
                 rrdtool.update(item.addrs, "N:" + text)
         else:
                 rrdtool.update(item.addrs + text.split())
     except Exception as e:
         srv.logging.warning("Cannot call rrdtool")
         return False
```

### Comparing `mqttwarn-0.34.0/mqttwarn/services/serial.py` & `mqttwarn-0.34.1/mqttwarn/services/serial.py`

 * *Files identical despite different names*

### Comparing `mqttwarn-0.34.0/mqttwarn/services/slack.py` & `mqttwarn-0.34.1/mqttwarn/services/slack.py`

 * *Files identical despite different names*

### Comparing `mqttwarn-0.34.0/mqttwarn/services/slixmpp.py` & `mqttwarn-0.34.1/mqttwarn/services/slixmpp.py`

 * *Files identical despite different names*

### Comparing `mqttwarn-0.34.0/mqttwarn/services/smtp.py` & `mqttwarn-0.34.1/mqttwarn/services/smtp.py`

 * *Files identical despite different names*

### Comparing `mqttwarn-0.34.0/mqttwarn/services/sqlite.py` & `mqttwarn-0.34.1/mqttwarn/services/sqlite.py`

 * *Files identical despite different names*

### Comparing `mqttwarn-0.34.0/mqttwarn/services/sqlite_json2cols.py` & `mqttwarn-0.34.1/mqttwarn/services/sqlite_json2cols.py`

 * *Files identical despite different names*

### Comparing `mqttwarn-0.34.0/mqttwarn/services/sqlite_timestamp.py` & `mqttwarn-0.34.1/mqttwarn/services/sqlite_timestamp.py`

 * *Files identical despite different names*

### Comparing `mqttwarn-0.34.0/mqttwarn/services/ssh.py` & `mqttwarn-0.34.1/mqttwarn/services/ssh.py`

 * *Files identical despite different names*

### Comparing `mqttwarn-0.34.0/mqttwarn/services/syslog.py` & `mqttwarn-0.34.1/mqttwarn/services/syslog.py`

 * *Files identical despite different names*

### Comparing `mqttwarn-0.34.0/mqttwarn/services/telegram.py` & `mqttwarn-0.34.1/mqttwarn/services/telegram.py`

 * *Files 1% similar despite different names*

```diff
@@ -105,15 +105,15 @@
                 return False
             else:
                 return answer_json
 
     try:
         tg = TelegramAPI(token, parse_mode)
         if useChatId:
-            srv.logging.debug("Setting chatid directly to %r", tg_contact)
+            srv.logging.debug("Setting chat_id directly to %r", tg_contact)
             uid = int(tg_contact)
         else:
             uid = tg.get_uid(tg_contact)
         if uid == 0:
             srv.logging.warn("Cannot get chat_id for user %r", tg_contact)
             return False
         reply = tg.send_message(uid, item.message)
```

### Comparing `mqttwarn-0.34.0/mqttwarn/services/thingspeak.py` & `mqttwarn-0.34.1/mqttwarn/services/thingspeak.py`

 * *Files identical despite different names*

### Comparing `mqttwarn-0.34.0/mqttwarn/services/tootpaste.py` & `mqttwarn-0.34.1/mqttwarn/services/tootpaste.py`

 * *Files identical despite different names*

### Comparing `mqttwarn-0.34.0/mqttwarn/services/twilio.py` & `mqttwarn-0.34.1/mqttwarn/services/twilio.py`

 * *Files identical despite different names*

### Comparing `mqttwarn-0.34.0/mqttwarn/services/twitter.py` & `mqttwarn-0.34.1/mqttwarn/services/twitter.py`

 * *Files identical despite different names*

### Comparing `mqttwarn-0.34.0/mqttwarn/services/websocket.py` & `mqttwarn-0.34.1/mqttwarn/services/websocket.py`

 * *Files identical despite different names*

### Comparing `mqttwarn-0.34.0/mqttwarn/services/xmpp.py` & `mqttwarn-0.34.1/mqttwarn/services/xmpp.py`

 * *Files identical despite different names*

### Comparing `mqttwarn-0.34.0/mqttwarn/services/zabbix.py` & `mqttwarn-0.34.1/mqttwarn/services/zabbix.py`

 * *Files identical despite different names*

### Comparing `mqttwarn-0.34.0/mqttwarn/util.py` & `mqttwarn-0.34.1/mqttwarn/util.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 import json
 import logging
 import os
 import re
 import string
 import types
 import typing as t
+from pathlib import Path
 
 import funcy
 import pkg_resources
 from six import string_types
 
 logger = logging.getLogger(__name__)
 
@@ -29,15 +30,15 @@
         The conversion field causes a type coercion before formatting.
         By default, two conversion flags are supported: '!s' which calls
         str() on the value, and '!r' which calls repr().
 
         This also adds the '!j' conversion flag, which serializes the
         value to JSON format.
 
-        See also https://github.com/jpmens/mqttwarn/issues/146.
+        See also https://github.com/mqtt-tools/mqttwarn/issues/146.
         """
         if conversion == "j":
             value = json.dumps(value)
         return value
 
 
 def asbool(obj: t.Any) -> bool:
@@ -227,23 +228,26 @@
     s = str(s)
     s = s.strip()
     if len(s) > limit:
         return s[:limit].strip() + ellipsis
     return s
 
 
-def load_file(path: str, retry_tries=None, retry_interval=0.075, unlink=False) -> t.IO[bytes]:
+def load_file(path: t.Union[str, Path], retry_tries=None, retry_interval=0.075, unlink=False) -> t.IO[bytes]:
     """
     Load file content from filesystem gracefully, with optional retrying.
+
+    TODO: Use better variant.
+          https://github.com/Suor/funcy/issues/126#issuecomment-1527279230
     """
     call = functools.partial(open, path, "rb")
     if retry_tries:
         logger.info(f"Retry loading file {path} for {retry_tries} times")
-        payload = funcy.retry(tries=int(retry_tries), timeout=float(retry_interval))(call)()
+        reader = funcy.retry(tries=int(retry_tries), timeout=float(retry_interval))(call)()
     else:
-        payload = call()
+        reader = call()
     if unlink:
         try:
             os.unlink(path)
-        except:
+        except:  # pragma: nocover
             pass
-    return payload
+    return reader
```

### Comparing `mqttwarn-0.34.0/mqttwarn/vendor/ZabbixSender.py` & `mqttwarn-0.34.1/mqttwarn/vendor/ZabbixSender.py`

 * *Files 8% similar despite different names*

```diff
@@ -18,25 +18,25 @@
     import simplejson as json  # type: ignore[no-redef]
 
 
 class ZabbixSender:
     
     zbx_header = b'ZBXD'
     zbx_version = 1
-    zbx_sender_data = {u'request': u'sender data', u'data': []}
+    zbx_sender_data = {'request': 'sender data', 'data': []}
     send_data = ''
     
     def __init__(self, server_host, server_port = 10051):
         self.server_ip = socket.gethostbyname(server_host)
         self.server_port = server_port
     
     def AddData(self, host, key, value, clock = None):
-        add_data = {u'host': host, u'key': key, u'value': value}
+        add_data = {'host': host, 'key': key, 'value': value}
         if clock != None:
-            add_data[u'clock'] = clock
+            add_data['clock'] = clock
         self.zbx_sender_data['data'].append(add_data)
         return self.zbx_sender_data
     
     def ClearData(self):
         self.zbx_sender_data['data'] = []
         return self.zbx_sender_data
     
@@ -45,27 +45,27 @@
         json_byte = len(zbx_sender_json)
         self.send_data = struct.pack("<4sBq" + str(json_byte) + "s", self.zbx_header, self.zbx_version, json_byte, zbx_sender_json)
     
     def Send(self):
         self.__MakeSendData()
         so = socket.socket()
         so.connect((self.server_ip, self.server_port))
-        wobj = so.makefile(u'wb')
+        wobj = so.makefile('wb')
         wobj.write(self.send_data)
         wobj.close()
-        robj = so.makefile(u'rb')
+        robj = so.makefile('rb')
         recv_data = robj.read()
         robj.close()
         so.close()
         tmp_data = struct.unpack("<4sBq" + str(len(recv_data) - struct.calcsize("<4sBq")) + "s", recv_data)
         recv_json = json.loads(tmp_data[3])
         #JPM return recv_data
         return recv_json
 
 
 if __name__ == '__main__':
-    sender = ZabbixSender(u'127.0.0.1')
+    sender = ZabbixSender('127.0.0.1')
     for num in range(0, 2):
-        sender.AddData(u'HostA', u'AppX_Logger', u'sent data 第' + str(num))
+        sender.AddData('HostA', 'AppX_Logger', 'sent data 第' + str(num))
     res = sender.Send()
     print(sender.send_data)
     print(res)
```

### Comparing `mqttwarn-0.34.0/mqttwarn.egg-info/requires.txt` & `mqttwarn-0.34.1/mqttwarn.egg-info/requires.txt`

 * *Files 10% similar despite different names*

```diff
@@ -15,33 +15,31 @@
 apns>=2.0.1
 apprise<2,>=1.3
 pyst2>=0.5.0
 celery
 pychromecast>=7.5.0
 dnspython>=1.15.0
 fbchat>=1.3.6
-gdata>=2.0.18
+google-api-python-client<2
 gspread>=2.1.1
 oauth2client>=4.1.2
-PyNMA>=1.0
 pynsca>=1.6
 desktop-notifier<4
 Pastebin>=1.1.2
 psycopg2-binary>=2.7.4
 pyprowl>=3.0.1
 PushbulletPythonLibrary>=2.3
 redis>=2.10.6
 pyserial>=3.4
 slack-sdk>=3.1.0
 paramiko>=2.4.1
 Mastodon.py>=1.2.2
 twilio>=6.11.0
 python-twitter>=3.4.1
 websocket-client>=0.47.0
-xively-python
 xmpppy>=0.6.1
 dnspython>=1.16.0
 slixmpp>=1.5.2
 mqttwarn-contrib
 
 [amqp]
 puka>=0.0.7
@@ -80,26 +78,24 @@
 
 [dnsupdate]
 dnspython>=1.15.0
 
 [fbchat]
 fbchat>=1.3.6
 
-[gss]
-gdata>=2.0.18
-
 [gss2]
+google-api-python-client<2
 gspread>=2.1.1
 oauth2client>=4.1.2
 
 [mysql]
 mysql
 
-[nma]
-PyNMA>=1.0
+[mysql_dynamic]
+mysqlclient
 
 [nsca]
 pynsca>=1.6
 
 [pastebinpub]
 Pastebin>=1.1.2
 
@@ -132,44 +128,42 @@
 
 [test]
 pytest<8
 pytest-cov<5
 pytest-mock<4
 pytest-mqtt<1
 tox<4
-requests-toolbelt<1,>=0.9.1
+requests-toolbelt<2,>=1
 responses<1,>=0.13.3
 pyfakefs<5,>=4.5
 puka>=0.0.7
 apns>=2.0.1
 apprise<2,>=1.3
 pyst2>=0.5.0
 celery
 pychromecast>=7.5.0
 dnspython>=1.15.0
 fbchat>=1.3.6
-gdata>=2.0.18
+google-api-python-client<2
 gspread>=2.1.1
 oauth2client>=4.1.2
-PyNMA>=1.0
 pynsca>=1.6
 desktop-notifier<4
 Pastebin>=1.1.2
 psycopg2-binary>=2.7.4
 pyprowl>=3.0.1
 PushbulletPythonLibrary>=2.3
 redis>=2.10.6
 pyserial>=3.4
 slack-sdk>=3.1.0
 paramiko>=2.4.1
 Mastodon.py>=1.2.2
 twilio>=6.11.0
 python-twitter>=3.4.1
 websocket-client>=0.47.0
-xively-python
 xmpppy>=0.6.1
 dnspython>=1.16.0
 slixmpp>=1.5.2
 mqttwarn-contrib
 
 [test:python_version < "3.7"]
 dataclasses
@@ -182,13 +176,10 @@
 
 [twitter]
 python-twitter>=3.4.1
 
 [websocket]
 websocket-client>=0.47.0
 
-[xively]
-xively-python
-
 [xmpp]
 xmpppy>=0.6.1
 dnspython>=1.16.0
```

### Comparing `mqttwarn-0.34.0/pyproject.toml` & `mqttwarn-0.34.1/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -82,16 +82,17 @@
 # ==================
 # Test configuration
 # ==================
 
 [tool.pytest.ini_options]
 minversion = "2.0"
 addopts = "-rsfEX -p pytester --strict-markers --verbosity=3 --cov --cov-report=term-missing --cov-report=xml --cov-report html:.pytest_results/htmlcov"
-log_level = "DEBUG"
+# log_cli = true  # Enable to receive way more log details on stdout.
 log_cli_level = "DEBUG"
+log_level = "DEBUG"
 testpaths = ["examples", "mqttwarn", "tests"]
 xfail_strict = true
 markers = [
   "e2e",  # Full end-to-end system tests, needing an MQTT broker.
 ]
 
 [tool.coverage.run]
@@ -123,7 +124,17 @@
   {cmd="mypy --install-types --non-interactive"},
 ]
 test = [
   {cmd="pytest"},
 ]
 build = {cmd="python -m build"}
 check = ["lint", "test"]
+release = [
+  { cmd = "pip install --upgrade --requirement requirements-release.txt" },
+  # TODO: Add a basic bump step, which only runs the `git tag` and `git push` commands,
+  #       but offers a convenience option to bump by "patch", "minor", or "major" levels.
+  # TODO: Remind user about updating the changelog file accordingly. Or use `towncrier`?
+  { cmd = "git push" },
+  { cmd = "git push --tags" },
+  { cmd = "python -m build" },
+  { cmd = "twine upload --skip-existing --verbose dist/*{{.tar.gz,.whl}}" },
+]
```

### Comparing `mqttwarn-0.34.0/setup.py` & `mqttwarn-0.34.1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # -*- coding: utf-8 -*-
 # (c) 2014-2023 The mqttwarn developers
 import os
 import platform
+import sys
 
 from setuptools import find_packages, setup
 from versioningit import get_cmdclasses
 
 here = os.path.abspath(os.path.dirname(__file__))
 README = open(os.path.join(here, "README.rst")).read()
 
@@ -42,27 +43,24 @@
     ],
     "dnsupdate": [
         "dnspython>=1.15.0",
     ],
     "fbchat": [
         "fbchat>=1.3.6",
     ],
-    "gss": [
-        "gdata>=2.0.18",
-    ],
     "gss2": [
+        "google-api-python-client<2",
         "gspread>=2.1.1",
         "oauth2client>=4.1.2",
-        #'google-api-python-client>=1.7.11',
     ],
     "mysql": [
         "mysql",
     ],
-    "nma": [
-        "PyNMA>=1.0",
+    "mysql_dynamic": [
+        "mysqlclient",
     ],
     "nsca": [
         "pynsca>=1.6",
     ],
     "desktopnotify": [
         "desktop-notifier<4",
     ],
@@ -101,17 +99,14 @@
     ],
     "twitter": [
         "python-twitter>=3.4.1",
     ],
     "websocket": [
         "websocket-client>=0.47.0",
     ],
-    "xively": [
-        "xively-python",
-    ],
     "xmpp": [
         "xmpppy>=0.6.1",
         "dnspython>=1.16.0",
     ],
     "slixmpp": [
         "slixmpp>=1.5.2",
     ],
@@ -128,22 +123,28 @@
 for extra, packages in extras.items():
 
     # FIXME: Skip specific packages having build issues.
     # https://github.com/commx/python-rrdtool/issues/36
     if extra in ["mysql", "rrdtool"]:
         continue
 
+    # FIXME: `mysqlclient` needs MySQL or MariaDB client libraries.
+    if extra in ["mysql_dynamic"] and sys.platform in ["darwin", "win32"]:
+        continue
+
     # FIXME: Skip specific packages on specific platforms,
     #        because they would also need a build toolchain.
     machine = platform.uname()[4]
     if machine in ["armv7l", "aarch64"] and extra in ["postgres", "slixmpp", "ssh"]:
         continue
 
-    # FIXME: The `cryptography` package is not available as binary wheel on arm32v7.
-    if machine in ["armv7l"] and extra in ["apprise"]:
+    # FIXME: A few packages are not available as wheels on arm32v7, and take quite an amount
+    #        of time to build, so let's mask them to improve build times significantly.
+    #        Examples: `cryptography`, `aiohttp`, `frozenlist`, `multidict`, `yarl`.
+    if machine in ["armv7l"] and extra in ["apprise", "twilio"]:
         continue
 
     for package in packages:
         extras_all.append(package)
 
 extras["all"] = extras_all
 
@@ -152,15 +153,15 @@
 extras["test"] = [
     "pytest<8",
     "pytest-cov<5",
     "pytest-mock<4",
     "pytest-mqtt<1",
     "tox<4",
     'dataclasses; python_version<"3.7"',
-    "requests-toolbelt>=0.9.1,<1",
+    "requests-toolbelt>=1,<2",
     "responses>=0.13.3,<1",
     "pyfakefs>=4.5,<5",
 ] + extras["all"]
 
 # Packages needed for development and running CI.
 extras["develop"] = [
     "isort<6",
@@ -217,15 +218,15 @@
         "Topic :: System :: Networking :: Monitoring",
         "Topic :: System :: Systems Administration",
         "Topic :: Text Processing",
         "Topic :: Utilities",
     ],
     author="Jan-Piet Mens, Ben Jones, Andreas Motl",
     author_email="jpmens@gmail.com",
-    url="https://github.com/jpmens/mqttwarn",
+    url="https://github.com/mqtt-tools/mqttwarn",
     keywords="mqtt notification plugins data acquisition push transformation engine mosquitto",
     packages=find_packages(),
     include_package_data=True,
     package_data={
         "mqttwarn": [
             "*.ini",
         ],
```

