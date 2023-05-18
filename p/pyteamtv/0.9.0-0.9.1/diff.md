# Comparing `tmp/pyteamtv-0.9.0.tar.gz` & `tmp/pyteamtv-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyteamtv-0.9.0.tar", last modified: Fri Jul  1 14:06:55 2022, max compression
+gzip compressed data, was "pyteamtv-0.9.1.tar", last modified: Fri Jul  1 19:35:25 2022, max compression
```

## Comparing `pyteamtv-0.9.0.tar` & `pyteamtv-0.9.1.tar`

### file list

```diff
@@ -1,62 +1,62 @@
-drwxr-xr-x   0 koen       (501) staff       (20)        0 2022-07-01 14:06:55.847220 pyteamtv-0.9.0/
--rw-r--r--   0 koen       (501) staff       (20)     1048 2022-07-01 14:06:55.847083 pyteamtv-0.9.0/PKG-INFO
--rw-r--r--   0 koen       (501) staff       (20)      294 2022-04-01 20:56:44.000000 pyteamtv-0.9.0/README.md
-drwxr-xr-x   0 koen       (501) staff       (20)        0 2022-07-01 14:06:55.839737 pyteamtv-0.9.0/pyteamtv/
--rw-r--r--   0 koen       (501) staff       (20)      485 2022-07-01 14:06:19.000000 pyteamtv-0.9.0/pyteamtv/__init__.py
-drwxr-xr-x   0 koen       (501) staff       (20)        0 2022-07-01 14:06:55.841023 pyteamtv-0.9.0/pyteamtv/_integrations/
--rw-r--r--   0 koen       (501) staff       (20)        0 2022-01-14 10:55:26.000000 pyteamtv-0.9.0/pyteamtv/_integrations/__init__.py
--rw-r--r--   0 koen       (501) staff       (20)     1165 2022-06-03 14:51:56.000000 pyteamtv-0.9.0/pyteamtv/_integrations/_dash.py
--rw-r--r--   0 koen       (501) staff       (20)      351 2022-06-03 14:51:56.000000 pyteamtv-0.9.0/pyteamtv/_integrations/_streamlit.py
--rw-r--r--   0 koen       (501) staff       (20)     3594 2022-06-03 14:51:56.000000 pyteamtv-0.9.0/pyteamtv/_integrations/app.py
-drwxr-xr-x   0 koen       (501) staff       (20)        0 2022-07-01 14:06:55.841663 pyteamtv-0.9.0/pyteamtv/api/
--rw-r--r--   0 koen       (501) staff       (20)       56 2022-01-14 10:55:26.000000 pyteamtv-0.9.0/pyteamtv/api/__init__.py
--rw-r--r--   0 koen       (501) staff       (20)      795 2022-06-03 14:51:56.000000 pyteamtv-0.9.0/pyteamtv/api/app.py
--rw-r--r--   0 koen       (501) staff       (20)       95 2022-06-03 14:51:56.000000 pyteamtv-0.9.0/pyteamtv/api/endpoint.py
--rw-r--r--   0 koen       (501) staff       (20)       97 2022-06-03 14:51:56.000000 pyteamtv-0.9.0/pyteamtv/api/token.py
--rw-r--r--   0 koen       (501) staff       (20)     2042 2022-06-03 14:51:56.000000 pyteamtv-0.9.0/pyteamtv/api/user.py
--rw-r--r--   0 koen       (501) staff       (20)       42 2022-01-14 10:55:26.000000 pyteamtv-0.9.0/pyteamtv/dash.py
--rw-r--r--   0 koen       (501) staff       (20)      131 2022-01-14 14:17:34.000000 pyteamtv-0.9.0/pyteamtv/exceptions.py
-drwxr-xr-x   0 koen       (501) staff       (20)        0 2022-07-01 14:06:55.841835 pyteamtv-0.9.0/pyteamtv/infra/
--rw-r--r--   0 koen       (501) staff       (20)        0 2022-01-14 10:55:26.000000 pyteamtv-0.9.0/pyteamtv/infra/__init__.py
--rw-r--r--   0 koen       (501) staff       (20)     1170 2022-06-03 14:51:56.000000 pyteamtv-0.9.0/pyteamtv/infra/requester.py
-drwxr-xr-x   0 koen       (501) staff       (20)        0 2022-07-01 14:06:55.844546 pyteamtv-0.9.0/pyteamtv/models/
--rw-r--r--   0 koen       (501) staff       (20)        0 2022-01-14 10:55:26.000000 pyteamtv-0.9.0/pyteamtv/models/__init__.py
--rw-r--r--   0 koen       (501) staff       (20)      846 2022-06-03 14:51:56.000000 pyteamtv-0.9.0/pyteamtv/models/app_storage.py
--rw-r--r--   0 koen       (501) staff       (20)      330 2022-06-03 14:51:56.000000 pyteamtv-0.9.0/pyteamtv/models/club.py
--rw-r--r--   0 koen       (501) staff       (20)      499 2022-06-29 15:02:44.000000 pyteamtv-0.9.0/pyteamtv/models/event_stream.py
--rw-r--r--   0 koen       (501) staff       (20)     1476 2022-06-03 14:51:56.000000 pyteamtv-0.9.0/pyteamtv/models/exercise.py
--rw-r--r--   0 koen       (501) staff       (20)     1844 2022-07-01 13:55:18.000000 pyteamtv-0.9.0/pyteamtv/models/line_up.py
--rw-r--r--   0 koen       (501) staff       (20)     1530 2022-07-01 12:39:49.000000 pyteamtv-0.9.0/pyteamtv/models/list.py
--rw-r--r--   0 koen       (501) staff       (20)     1042 2022-06-03 14:51:56.000000 pyteamtv-0.9.0/pyteamtv/models/membership.py
--rw-r--r--   0 koen       (501) staff       (20)     1696 2022-06-03 14:51:56.000000 pyteamtv-0.9.0/pyteamtv/models/membership_list.py
--rw-r--r--   0 koen       (501) staff       (20)     1180 2022-06-03 14:51:56.000000 pyteamtv-0.9.0/pyteamtv/models/observation.py
--rw-r--r--   0 koen       (501) staff       (20)     3937 2022-06-03 14:51:56.000000 pyteamtv-0.9.0/pyteamtv/models/observation_log.py
--rw-r--r--   0 koen       (501) staff       (20)     1057 2022-07-01 13:11:50.000000 pyteamtv-0.9.0/pyteamtv/models/person.py
--rw-r--r--   0 koen       (501) staff       (20)      592 2022-07-01 13:11:56.000000 pyteamtv-0.9.0/pyteamtv/models/player.py
-drwxr-xr-x   0 koen       (501) staff       (20)        0 2022-07-01 14:06:55.846891 pyteamtv-0.9.0/pyteamtv/models/resource_group/
--rw-r--r--   0 koen       (501) staff       (20)      859 2022-06-03 14:51:56.000000 pyteamtv-0.9.0/pyteamtv/models/resource_group/__init__.py
--rw-r--r--   0 koen       (501) staff       (20)      272 2022-06-03 14:51:56.000000 pyteamtv-0.9.0/pyteamtv/models/resource_group/app_developer.py
--rw-r--r--   0 koen       (501) staff       (20)     4833 2022-06-30 14:30:47.000000 pyteamtv-0.9.0/pyteamtv/models/resource_group/capabilities.py
--rw-r--r--   0 koen       (501) staff       (20)      317 2022-06-03 14:51:56.000000 pyteamtv-0.9.0/pyteamtv/models/resource_group/club.py
--rw-r--r--   0 koen       (501) staff       (20)       86 2022-06-30 14:25:11.000000 pyteamtv-0.9.0/pyteamtv/models/resource_group/education.py
--rw-r--r--   0 koen       (501) staff       (20)      185 2022-06-03 14:51:56.000000 pyteamtv-0.9.0/pyteamtv/models/resource_group/exchange.py
--rw-r--r--   0 koen       (501) staff       (20)     1371 2022-06-30 14:25:11.000000 pyteamtv-0.9.0/pyteamtv/models/resource_group/factory.py
--rw-r--r--   0 koen       (501) staff       (20)      231 2022-06-03 14:51:56.000000 pyteamtv-0.9.0/pyteamtv/models/resource_group/person.py
--rw-r--r--   0 koen       (501) staff       (20)      233 2022-06-03 14:51:56.000000 pyteamtv-0.9.0/pyteamtv/models/resource_group/reseller.py
--rw-r--r--   0 koen       (501) staff       (20)      728 2022-06-03 14:51:56.000000 pyteamtv-0.9.0/pyteamtv/models/resource_group/sharing_group.py
--rw-r--r--   0 koen       (501) staff       (20)      303 2022-06-30 14:30:47.000000 pyteamtv-0.9.0/pyteamtv/models/resource_group/team.py
--rw-r--r--   0 koen       (501) staff       (20)      229 2022-06-03 14:51:56.000000 pyteamtv-0.9.0/pyteamtv/models/resource_group/user.py
--rw-r--r--   0 koen       (501) staff       (20)      891 2022-06-03 14:51:56.000000 pyteamtv-0.9.0/pyteamtv/models/sharing_group.py
--rw-r--r--   0 koen       (501) staff       (20)     7607 2022-07-01 13:13:50.000000 pyteamtv-0.9.0/pyteamtv/models/sporting_event.py
--rw-r--r--   0 koen       (501) staff       (20)     1739 2022-07-01 13:14:01.000000 pyteamtv-0.9.0/pyteamtv/models/team.py
--rw-r--r--   0 koen       (501) staff       (20)      321 2022-01-14 14:14:11.000000 pyteamtv-0.9.0/pyteamtv/models/teamtv_object.py
--rw-r--r--   0 koen       (501) staff       (20)      772 2022-06-03 14:51:56.000000 pyteamtv-0.9.0/pyteamtv/models/video.py
--rw-r--r--   0 koen       (501) staff       (20)       54 2022-01-14 10:55:26.000000 pyteamtv-0.9.0/pyteamtv/streamlit.py
-drwxr-xr-x   0 koen       (501) staff       (20)        0 2022-07-01 14:06:55.840351 pyteamtv-0.9.0/pyteamtv.egg-info/
--rw-r--r--   0 koen       (501) staff       (20)     1048 2022-07-01 14:06:55.000000 pyteamtv-0.9.0/pyteamtv.egg-info/PKG-INFO
--rw-r--r--   0 koen       (501) staff       (20)     1604 2022-07-01 14:06:55.000000 pyteamtv-0.9.0/pyteamtv.egg-info/SOURCES.txt
--rw-r--r--   0 koen       (501) staff       (20)        1 2022-07-01 14:06:55.000000 pyteamtv-0.9.0/pyteamtv.egg-info/dependency_links.txt
--rw-r--r--   0 koen       (501) staff       (20)       92 2022-07-01 14:06:55.000000 pyteamtv-0.9.0/pyteamtv.egg-info/requires.txt
--rw-r--r--   0 koen       (501) staff       (20)        9 2022-07-01 14:06:55.000000 pyteamtv-0.9.0/pyteamtv.egg-info/top_level.txt
--rw-r--r--   0 koen       (501) staff       (20)       38 2022-07-01 14:06:55.847266 pyteamtv-0.9.0/setup.cfg
--rw-r--r--   0 koen       (501) staff       (20)     1501 2022-06-03 14:52:48.000000 pyteamtv-0.9.0/setup.py
+drwxr-xr-x   0 koen       (501) staff       (20)        0 2022-07-01 19:35:25.585258 pyteamtv-0.9.1/
+-rw-r--r--   0 koen       (501) staff       (20)     1048 2022-07-01 19:35:25.585101 pyteamtv-0.9.1/PKG-INFO
+-rw-r--r--   0 koen       (501) staff       (20)      294 2022-04-01 20:56:44.000000 pyteamtv-0.9.1/README.md
+drwxr-xr-x   0 koen       (501) staff       (20)        0 2022-07-01 19:35:25.577399 pyteamtv-0.9.1/pyteamtv/
+-rw-r--r--   0 koen       (501) staff       (20)      485 2022-07-01 19:32:22.000000 pyteamtv-0.9.1/pyteamtv/__init__.py
+drwxr-xr-x   0 koen       (501) staff       (20)        0 2022-07-01 19:35:25.578539 pyteamtv-0.9.1/pyteamtv/_integrations/
+-rw-r--r--   0 koen       (501) staff       (20)        0 2022-01-14 10:55:26.000000 pyteamtv-0.9.1/pyteamtv/_integrations/__init__.py
+-rw-r--r--   0 koen       (501) staff       (20)     1165 2022-06-03 14:51:56.000000 pyteamtv-0.9.1/pyteamtv/_integrations/_dash.py
+-rw-r--r--   0 koen       (501) staff       (20)      351 2022-06-03 14:51:56.000000 pyteamtv-0.9.1/pyteamtv/_integrations/_streamlit.py
+-rw-r--r--   0 koen       (501) staff       (20)     3594 2022-06-03 14:51:56.000000 pyteamtv-0.9.1/pyteamtv/_integrations/app.py
+drwxr-xr-x   0 koen       (501) staff       (20)        0 2022-07-01 19:35:25.579656 pyteamtv-0.9.1/pyteamtv/api/
+-rw-r--r--   0 koen       (501) staff       (20)       56 2022-01-14 10:55:26.000000 pyteamtv-0.9.1/pyteamtv/api/__init__.py
+-rw-r--r--   0 koen       (501) staff       (20)      795 2022-06-03 14:51:56.000000 pyteamtv-0.9.1/pyteamtv/api/app.py
+-rw-r--r--   0 koen       (501) staff       (20)       95 2022-06-03 14:51:56.000000 pyteamtv-0.9.1/pyteamtv/api/endpoint.py
+-rw-r--r--   0 koen       (501) staff       (20)       97 2022-06-03 14:51:56.000000 pyteamtv-0.9.1/pyteamtv/api/token.py
+-rw-r--r--   0 koen       (501) staff       (20)     2042 2022-06-03 14:51:56.000000 pyteamtv-0.9.1/pyteamtv/api/user.py
+-rw-r--r--   0 koen       (501) staff       (20)       42 2022-01-14 10:55:26.000000 pyteamtv-0.9.1/pyteamtv/dash.py
+-rw-r--r--   0 koen       (501) staff       (20)      131 2022-01-14 14:17:34.000000 pyteamtv-0.9.1/pyteamtv/exceptions.py
+drwxr-xr-x   0 koen       (501) staff       (20)        0 2022-07-01 19:35:25.579861 pyteamtv-0.9.1/pyteamtv/infra/
+-rw-r--r--   0 koen       (501) staff       (20)        0 2022-01-14 10:55:26.000000 pyteamtv-0.9.1/pyteamtv/infra/__init__.py
+-rw-r--r--   0 koen       (501) staff       (20)     1170 2022-06-03 14:51:56.000000 pyteamtv-0.9.1/pyteamtv/infra/requester.py
+drwxr-xr-x   0 koen       (501) staff       (20)        0 2022-07-01 19:35:25.583093 pyteamtv-0.9.1/pyteamtv/models/
+-rw-r--r--   0 koen       (501) staff       (20)        0 2022-01-14 10:55:26.000000 pyteamtv-0.9.1/pyteamtv/models/__init__.py
+-rw-r--r--   0 koen       (501) staff       (20)      846 2022-06-03 14:51:56.000000 pyteamtv-0.9.1/pyteamtv/models/app_storage.py
+-rw-r--r--   0 koen       (501) staff       (20)      330 2022-06-03 14:51:56.000000 pyteamtv-0.9.1/pyteamtv/models/club.py
+-rw-r--r--   0 koen       (501) staff       (20)      499 2022-06-29 15:02:44.000000 pyteamtv-0.9.1/pyteamtv/models/event_stream.py
+-rw-r--r--   0 koen       (501) staff       (20)     1476 2022-06-03 14:51:56.000000 pyteamtv-0.9.1/pyteamtv/models/exercise.py
+-rw-r--r--   0 koen       (501) staff       (20)     1937 2022-07-01 19:31:35.000000 pyteamtv-0.9.1/pyteamtv/models/line_up.py
+-rw-r--r--   0 koen       (501) staff       (20)     1530 2022-07-01 12:39:49.000000 pyteamtv-0.9.1/pyteamtv/models/list.py
+-rw-r--r--   0 koen       (501) staff       (20)     1042 2022-06-03 14:51:56.000000 pyteamtv-0.9.1/pyteamtv/models/membership.py
+-rw-r--r--   0 koen       (501) staff       (20)     1696 2022-06-03 14:51:56.000000 pyteamtv-0.9.1/pyteamtv/models/membership_list.py
+-rw-r--r--   0 koen       (501) staff       (20)     1180 2022-06-03 14:51:56.000000 pyteamtv-0.9.1/pyteamtv/models/observation.py
+-rw-r--r--   0 koen       (501) staff       (20)     3937 2022-06-03 14:51:56.000000 pyteamtv-0.9.1/pyteamtv/models/observation_log.py
+-rw-r--r--   0 koen       (501) staff       (20)     1057 2022-07-01 13:11:50.000000 pyteamtv-0.9.1/pyteamtv/models/person.py
+-rw-r--r--   0 koen       (501) staff       (20)      592 2022-07-01 13:11:56.000000 pyteamtv-0.9.1/pyteamtv/models/player.py
+drwxr-xr-x   0 koen       (501) staff       (20)        0 2022-07-01 19:35:25.584906 pyteamtv-0.9.1/pyteamtv/models/resource_group/
+-rw-r--r--   0 koen       (501) staff       (20)      859 2022-06-03 14:51:56.000000 pyteamtv-0.9.1/pyteamtv/models/resource_group/__init__.py
+-rw-r--r--   0 koen       (501) staff       (20)      272 2022-06-03 14:51:56.000000 pyteamtv-0.9.1/pyteamtv/models/resource_group/app_developer.py
+-rw-r--r--   0 koen       (501) staff       (20)     4833 2022-06-30 14:30:47.000000 pyteamtv-0.9.1/pyteamtv/models/resource_group/capabilities.py
+-rw-r--r--   0 koen       (501) staff       (20)      317 2022-06-03 14:51:56.000000 pyteamtv-0.9.1/pyteamtv/models/resource_group/club.py
+-rw-r--r--   0 koen       (501) staff       (20)       86 2022-06-30 14:25:11.000000 pyteamtv-0.9.1/pyteamtv/models/resource_group/education.py
+-rw-r--r--   0 koen       (501) staff       (20)      185 2022-06-03 14:51:56.000000 pyteamtv-0.9.1/pyteamtv/models/resource_group/exchange.py
+-rw-r--r--   0 koen       (501) staff       (20)     1371 2022-06-30 14:25:11.000000 pyteamtv-0.9.1/pyteamtv/models/resource_group/factory.py
+-rw-r--r--   0 koen       (501) staff       (20)      231 2022-06-03 14:51:56.000000 pyteamtv-0.9.1/pyteamtv/models/resource_group/person.py
+-rw-r--r--   0 koen       (501) staff       (20)      233 2022-06-03 14:51:56.000000 pyteamtv-0.9.1/pyteamtv/models/resource_group/reseller.py
+-rw-r--r--   0 koen       (501) staff       (20)      728 2022-06-03 14:51:56.000000 pyteamtv-0.9.1/pyteamtv/models/resource_group/sharing_group.py
+-rw-r--r--   0 koen       (501) staff       (20)      303 2022-06-30 14:30:47.000000 pyteamtv-0.9.1/pyteamtv/models/resource_group/team.py
+-rw-r--r--   0 koen       (501) staff       (20)      229 2022-06-03 14:51:56.000000 pyteamtv-0.9.1/pyteamtv/models/resource_group/user.py
+-rw-r--r--   0 koen       (501) staff       (20)      891 2022-06-03 14:51:56.000000 pyteamtv-0.9.1/pyteamtv/models/sharing_group.py
+-rw-r--r--   0 koen       (501) staff       (20)     7607 2022-07-01 13:13:50.000000 pyteamtv-0.9.1/pyteamtv/models/sporting_event.py
+-rw-r--r--   0 koen       (501) staff       (20)     1739 2022-07-01 13:14:01.000000 pyteamtv-0.9.1/pyteamtv/models/team.py
+-rw-r--r--   0 koen       (501) staff       (20)      321 2022-01-14 14:14:11.000000 pyteamtv-0.9.1/pyteamtv/models/teamtv_object.py
+-rw-r--r--   0 koen       (501) staff       (20)      772 2022-06-03 14:51:56.000000 pyteamtv-0.9.1/pyteamtv/models/video.py
+-rw-r--r--   0 koen       (501) staff       (20)       54 2022-01-14 10:55:26.000000 pyteamtv-0.9.1/pyteamtv/streamlit.py
+drwxr-xr-x   0 koen       (501) staff       (20)        0 2022-07-01 19:35:25.578114 pyteamtv-0.9.1/pyteamtv.egg-info/
+-rw-r--r--   0 koen       (501) staff       (20)     1048 2022-07-01 19:35:25.000000 pyteamtv-0.9.1/pyteamtv.egg-info/PKG-INFO
+-rw-r--r--   0 koen       (501) staff       (20)     1604 2022-07-01 19:35:25.000000 pyteamtv-0.9.1/pyteamtv.egg-info/SOURCES.txt
+-rw-r--r--   0 koen       (501) staff       (20)        1 2022-07-01 19:35:25.000000 pyteamtv-0.9.1/pyteamtv.egg-info/dependency_links.txt
+-rw-r--r--   0 koen       (501) staff       (20)       92 2022-07-01 19:35:25.000000 pyteamtv-0.9.1/pyteamtv.egg-info/requires.txt
+-rw-r--r--   0 koen       (501) staff       (20)        9 2022-07-01 19:35:25.000000 pyteamtv-0.9.1/pyteamtv.egg-info/top_level.txt
+-rw-r--r--   0 koen       (501) staff       (20)       38 2022-07-01 19:35:25.585303 pyteamtv-0.9.1/setup.cfg
+-rw-r--r--   0 koen       (501) staff       (20)     1501 2022-06-03 14:52:48.000000 pyteamtv-0.9.1/setup.py
```

### Comparing `pyteamtv-0.9.0/PKG-INFO` & `pyteamtv-0.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyteamtv
-Version: 0.9.0
+Version: 0.9.1
 Summary: API for TeamTV Platform
 Home-page: https://github.com/teamtv/pyteamtv
 Author: Koen Vossen
 Author-email: info@koenvossen.nl
 License: GPL-3
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

### Comparing `pyteamtv-0.9.0/pyteamtv/_integrations/_dash.py` & `pyteamtv-0.9.1/pyteamtv/_integrations/_dash.py`

 * *Files identical despite different names*

### Comparing `pyteamtv-0.9.0/pyteamtv/_integrations/app.py` & `pyteamtv-0.9.1/pyteamtv/_integrations/app.py`

 * *Files identical despite different names*

### Comparing `pyteamtv-0.9.0/pyteamtv/api/app.py` & `pyteamtv-0.9.1/pyteamtv/api/app.py`

 * *Files identical despite different names*

### Comparing `pyteamtv-0.9.0/pyteamtv/api/user.py` & `pyteamtv-0.9.1/pyteamtv/api/user.py`

 * *Files identical despite different names*

### Comparing `pyteamtv-0.9.0/pyteamtv/infra/requester.py` & `pyteamtv-0.9.1/pyteamtv/infra/requester.py`

 * *Files identical despite different names*

### Comparing `pyteamtv-0.9.0/pyteamtv/models/app_storage.py` & `pyteamtv-0.9.1/pyteamtv/models/app_storage.py`

 * *Files identical despite different names*

### Comparing `pyteamtv-0.9.0/pyteamtv/models/exercise.py` & `pyteamtv-0.9.1/pyteamtv/models/exercise.py`

 * *Files identical despite different names*

### Comparing `pyteamtv-0.9.0/pyteamtv/models/line_up.py` & `pyteamtv-0.9.1/pyteamtv/models/line_up.py`

 * *Files 11% similar despite different names*

```diff
@@ -48,10 +48,12 @@
                     }
                 )
 
     def _use_attributes(self, attributes: dict):
         self._sporting_event = attributes['sportingEvent']
         self._line_up_id = attributes["lineUpId"]
         self._roles_per_team = attributes["rolesPerTeam"]
+        if not isinstance(self._roles_per_team, dict):
+            self._roles_per_team = {}
 
     def __repr__(self):
         return f"<LineUp sportingEvent={self.sporting_event}>"
```

### Comparing `pyteamtv-0.9.0/pyteamtv/models/list.py` & `pyteamtv-0.9.1/pyteamtv/models/list.py`

 * *Files identical despite different names*

### Comparing `pyteamtv-0.9.0/pyteamtv/models/membership.py` & `pyteamtv-0.9.1/pyteamtv/models/membership.py`

 * *Files identical despite different names*

### Comparing `pyteamtv-0.9.0/pyteamtv/models/membership_list.py` & `pyteamtv-0.9.1/pyteamtv/models/membership_list.py`

 * *Files identical despite different names*

### Comparing `pyteamtv-0.9.0/pyteamtv/models/observation.py` & `pyteamtv-0.9.1/pyteamtv/models/observation.py`

 * *Files identical despite different names*

### Comparing `pyteamtv-0.9.0/pyteamtv/models/observation_log.py` & `pyteamtv-0.9.1/pyteamtv/models/observation_log.py`

 * *Files identical despite different names*

### Comparing `pyteamtv-0.9.0/pyteamtv/models/person.py` & `pyteamtv-0.9.1/pyteamtv/models/person.py`

 * *Files identical despite different names*

### Comparing `pyteamtv-0.9.0/pyteamtv/models/player.py` & `pyteamtv-0.9.1/pyteamtv/models/player.py`

 * *Files identical despite different names*

### Comparing `pyteamtv-0.9.0/pyteamtv/models/resource_group/__init__.py` & `pyteamtv-0.9.1/pyteamtv/models/resource_group/__init__.py`

 * *Files identical despite different names*

### Comparing `pyteamtv-0.9.0/pyteamtv/models/resource_group/capabilities.py` & `pyteamtv-0.9.1/pyteamtv/models/resource_group/capabilities.py`

 * *Files identical despite different names*

### Comparing `pyteamtv-0.9.0/pyteamtv/models/resource_group/factory.py` & `pyteamtv-0.9.1/pyteamtv/models/resource_group/factory.py`

 * *Files identical despite different names*

### Comparing `pyteamtv-0.9.0/pyteamtv/models/resource_group/sharing_group.py` & `pyteamtv-0.9.1/pyteamtv/models/resource_group/sharing_group.py`

 * *Files identical despite different names*

### Comparing `pyteamtv-0.9.0/pyteamtv/models/sharing_group.py` & `pyteamtv-0.9.1/pyteamtv/models/sharing_group.py`

 * *Files identical despite different names*

### Comparing `pyteamtv-0.9.0/pyteamtv/models/sporting_event.py` & `pyteamtv-0.9.1/pyteamtv/models/sporting_event.py`

 * *Files identical despite different names*

### Comparing `pyteamtv-0.9.0/pyteamtv/models/team.py` & `pyteamtv-0.9.1/pyteamtv/models/team.py`

 * *Files identical despite different names*

### Comparing `pyteamtv-0.9.0/pyteamtv/models/video.py` & `pyteamtv-0.9.1/pyteamtv/models/video.py`

 * *Files identical despite different names*

### Comparing `pyteamtv-0.9.0/pyteamtv.egg-info/PKG-INFO` & `pyteamtv-0.9.1/pyteamtv.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyteamtv
-Version: 0.9.0
+Version: 0.9.1
 Summary: API for TeamTV Platform
 Home-page: https://github.com/teamtv/pyteamtv
 Author: Koen Vossen
 Author-email: info@koenvossen.nl
 License: GPL-3
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

### Comparing `pyteamtv-0.9.0/pyteamtv.egg-info/SOURCES.txt` & `pyteamtv-0.9.1/pyteamtv.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyteamtv-0.9.0/setup.py` & `pyteamtv-0.9.1/setup.py`

 * *Files identical despite different names*

