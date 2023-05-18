# Comparing `tmp/oddsjam-api-0.2.7.tar.gz` & `tmp/oddsjam-api-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oddsjam-api-0.2.7.tar", last modified: Mon Jan 31 21:25:33 2022, max compression
+gzip compressed data, was "oddsjam-api-0.2.8.tar", last modified: Thu May 18 15:09:14 2023, max compression
```

## Comparing `oddsjam-api-0.2.7.tar` & `oddsjam-api-0.2.8.tar`

### file list

```diff
@@ -1,91 +1,92 @@
-drwxrwxrwx   0        0        0        0 2022-01-31 21:25:33.383482 oddsjam-api-0.2.7/
--rw-rw-rw-   0        0        0     1092 2022-01-31 13:55:06.000000 oddsjam-api-0.2.7/LICENSE
--rw-rw-rw-   0        0        0     4953 2022-01-31 21:25:33.383482 oddsjam-api-0.2.7/PKG-INFO
--rw-rw-rw-   0        0        0     4358 2022-01-31 21:09:47.000000 oddsjam-api-0.2.7/README.md
--rw-rw-rw-   0        0        0      108 2022-01-31 21:20:52.000000 oddsjam-api-0.2.7/pyproject.toml
--rw-rw-rw-   0        0        0      693 2022-01-31 21:25:33.385482 oddsjam-api-0.2.7/setup.cfg
-drwxrwxrwx   0        0        0        0 2022-01-31 21:25:33.316482 oddsjam-api-0.2.7/src/
-drwxrwxrwx   0        0        0        0 2022-01-31 21:25:33.324486 oddsjam-api-0.2.7/src/Base/
--rw-rw-rw-   0        0        0      843 2022-01-31 20:59:22.000000 oddsjam-api-0.2.7/src/Base/CustomExceptions.py
--rw-rw-rw-   0        0        0     1092 2022-01-31 20:12:55.000000 oddsjam-api-0.2.7/src/Base/EnforceTypes.py
--rw-rw-rw-   0        0        0      460 2022-01-31 15:33:33.000000 oddsjam-api-0.2.7/src/Base/ModelBase.py
--rw-rw-rw-   0        0        0     1084 2022-01-31 13:55:06.000000 oddsjam-api-0.2.7/src/Base/RequestBase.py
--rw-rw-rw-   0        0        0      529 2022-01-31 13:55:06.000000 oddsjam-api-0.2.7/src/Base/ResponseBase.py
--rw-rw-rw-   0        0        0      682 2022-01-31 14:15:57.000000 oddsjam-api-0.2.7/src/Base/ValidParameters.py
--rw-rw-rw-   0        0        0      292 2022-01-31 20:59:39.000000 oddsjam-api-0.2.7/src/Base/__init__.py
-drwxrwxrwx   0        0        0        0 2022-01-31 21:25:33.324486 oddsjam-api-0.2.7/src/Models/
-drwxrwxrwx   0        0        0        0 2022-01-31 21:25:33.330486 oddsjam-api-0.2.7/src/Models/V1/
--rw-rw-rw-   0        0        0      232 2022-01-31 16:45:45.000000 oddsjam-api-0.2.7/src/Models/V1/Future.py
--rw-rw-rw-   0        0        0      344 2022-01-31 16:48:56.000000 oddsjam-api-0.2.7/src/Models/V1/FutureOdds.py
--rw-rw-rw-   0        0        0      319 2022-01-31 16:46:02.000000 oddsjam-api-0.2.7/src/Models/V1/Game.py
--rw-rw-rw-   0        0        0      163 2022-01-31 16:46:10.000000 oddsjam-api-0.2.7/src/Models/V1/League.py
--rw-rw-rw-   0        0        0      216 2022-01-31 16:48:14.000000 oddsjam-api-0.2.7/src/Models/V1/Market.py
--rw-rw-rw-   0        0        0     1457 2022-01-31 16:48:39.000000 oddsjam-api-0.2.7/src/Models/V1/Odds.py
--rw-rw-rw-   0        0        0      223 2022-01-31 16:45:19.000000 oddsjam-api-0.2.7/src/Models/V1/PeriodScore.py
--rw-rw-rw-   0        0        0      653 2022-01-31 16:49:05.000000 oddsjam-api-0.2.7/src/Models/V1/Score.py
--rw-rw-rw-   0        0        0      230 2022-01-31 16:47:41.000000 oddsjam-api-0.2.7/src/Models/V1/__init__.py
-drwxrwxrwx   0        0        0        0 2022-01-31 21:25:33.336484 oddsjam-api-0.2.7/src/Models/V2/
--rw-rw-rw-   0        0        0      232 2022-01-31 14:35:05.000000 oddsjam-api-0.2.7/src/Models/V2/Future.py
--rw-rw-rw-   0        0        0      482 2022-01-31 16:51:01.000000 oddsjam-api-0.2.7/src/Models/V2/FutureOdds.py
--rw-rw-rw-   0        0        0      319 2022-01-31 14:17:05.000000 oddsjam-api-0.2.7/src/Models/V2/Game.py
--rw-rw-rw-   0        0        0      163 2022-01-31 13:55:06.000000 oddsjam-api-0.2.7/src/Models/V2/League.py
--rw-rw-rw-   0        0        0      216 2022-01-31 16:50:52.000000 oddsjam-api-0.2.7/src/Models/V2/Market.py
--rw-rw-rw-   0        0        0     1409 2022-01-31 20:31:57.000000 oddsjam-api-0.2.7/src/Models/V2/Odds.py
--rw-rw-rw-   0        0        0      223 2022-01-31 13:55:06.000000 oddsjam-api-0.2.7/src/Models/V2/PeriodScore.py
--rw-rw-rw-   0        0        0      653 2022-01-31 16:51:14.000000 oddsjam-api-0.2.7/src/Models/V2/Score.py
--rw-rw-rw-   0        0        0      241 2022-01-31 20:33:52.000000 oddsjam-api-0.2.7/src/Models/V2/__init__.py
--rw-rw-rw-   0        0        0        0 2022-01-31 16:45:29.000000 oddsjam-api-0.2.7/src/Models/__init__.py
-drwxrwxrwx   0        0        0        0 2022-01-31 21:25:33.338482 oddsjam-api-0.2.7/src/OddsJamClient/
--rw-rw-rw-   0        0        0     1790 2022-01-31 21:23:36.000000 oddsjam-api-0.2.7/src/OddsJamClient/OddsJamClient.py
-drwxrwxrwx   0        0        0        0 2022-01-31 21:25:33.340482 oddsjam-api-0.2.7/src/OddsJamClient/V1/
--rw-rw-rw-   0        0        0     3379 2022-01-31 16:37:42.000000 oddsjam-api-0.2.7/src/OddsJamClient/V1/Requestor.py
--rw-rw-rw-   0        0        0       35 2022-01-31 16:33:53.000000 oddsjam-api-0.2.7/src/OddsJamClient/V1/__init__.py
-drwxrwxrwx   0        0        0        0 2022-01-31 21:25:33.341483 oddsjam-api-0.2.7/src/OddsJamClient/V2/
--rw-rw-rw-   0        0        0     3634 2022-01-31 21:00:11.000000 oddsjam-api-0.2.7/src/OddsJamClient/V2/Requestor.py
--rw-rw-rw-   0        0        0       35 2022-01-31 16:33:58.000000 oddsjam-api-0.2.7/src/OddsJamClient/V2/__init__.py
--rw-rw-rw-   0        0        0       41 2022-01-31 13:55:06.000000 oddsjam-api-0.2.7/src/OddsJamClient/__init__.py
-drwxrwxrwx   0        0        0        0 2022-01-31 21:25:33.342485 oddsjam-api-0.2.7/src/Request/
-drwxrwxrwx   0        0        0        0 2022-01-31 21:25:33.348486 oddsjam-api-0.2.7/src/Request/V1/
--rw-rw-rw-   0        0        0      412 2022-01-31 16:28:43.000000 oddsjam-api-0.2.7/src/Request/V1/GetFutureOddsRequest.py
--rw-rw-rw-   0        0        0      324 2022-01-31 16:11:48.000000 oddsjam-api-0.2.7/src/Request/V1/GetFuturesRequest.py
--rw-rw-rw-   0        0        0      484 2022-01-31 16:12:05.000000 oddsjam-api-0.2.7/src/Request/V1/GetGamesRequest.py
--rw-rw-rw-   0        0        0      298 2022-01-31 16:12:08.000000 oddsjam-api-0.2.7/src/Request/V1/GetLeaguesRequest.py
--rw-rw-rw-   0        0        0      293 2022-01-31 15:52:01.000000 oddsjam-api-0.2.7/src/Request/V1/GetMarketsRequest.py
--rw-rw-rw-   0        0        0      450 2022-01-31 16:05:12.000000 oddsjam-api-0.2.7/src/Request/V1/GetOddsRequest.py
--rw-rw-rw-   0        0        0      289 2022-01-31 15:52:14.000000 oddsjam-api-0.2.7/src/Request/V1/GetScoresRequest.py
--rw-rw-rw-   0        0        0      350 2022-01-31 13:55:06.000000 oddsjam-api-0.2.7/src/Request/V1/__init__.py
-drwxrwxrwx   0        0        0        0 2022-01-31 21:25:33.353484 oddsjam-api-0.2.7/src/Request/V2/
--rw-rw-rw-   0        0        0      410 2022-01-31 16:03:08.000000 oddsjam-api-0.2.7/src/Request/V2/GetFutureOddsRequest.py
--rw-rw-rw-   0        0        0      322 2022-01-31 16:03:08.000000 oddsjam-api-0.2.7/src/Request/V2/GetFuturesRequest.py
--rw-rw-rw-   0        0        0      482 2022-01-31 16:28:43.000000 oddsjam-api-0.2.7/src/Request/V2/GetGamesRequest.py
--rw-rw-rw-   0        0        0      296 2022-01-31 16:03:08.000000 oddsjam-api-0.2.7/src/Request/V2/GetLeaguesRequest.py
--rw-rw-rw-   0        0        0      291 2022-01-31 16:04:52.000000 oddsjam-api-0.2.7/src/Request/V2/GetMarketsRequest.py
--rw-rw-rw-   0        0        0      466 2022-01-31 20:14:25.000000 oddsjam-api-0.2.7/src/Request/V2/GetOddsRequest.py
--rw-rw-rw-   0        0        0      287 2022-01-31 16:12:25.000000 oddsjam-api-0.2.7/src/Request/V2/GetScoresRequest.py
--rw-rw-rw-   0        0        0      350 2022-01-31 16:03:08.000000 oddsjam-api-0.2.7/src/Request/V2/__init__.py
--rw-rw-rw-   0        0        0        0 2022-01-31 16:33:16.000000 oddsjam-api-0.2.7/src/Request/__init__.py
-drwxrwxrwx   0        0        0        0 2022-01-31 21:25:33.354484 oddsjam-api-0.2.7/src/Response/
-drwxrwxrwx   0        0        0        0 2022-01-31 21:25:33.360483 oddsjam-api-0.2.7/src/Response/V1/
--rw-rw-rw-   0        0        0      713 2022-01-31 16:50:32.000000 oddsjam-api-0.2.7/src/Response/V1/GetFutureOddsResponse.py
--rw-rw-rw-   0        0        0      520 2022-01-31 16:50:20.000000 oddsjam-api-0.2.7/src/Response/V1/GetFuturesResponse.py
--rw-rw-rw-   0        0        0      504 2022-01-31 16:47:59.000000 oddsjam-api-0.2.7/src/Response/V1/GetGamesResponse.py
--rw-rw-rw-   0        0        0      530 2022-01-31 16:49:14.000000 oddsjam-api-0.2.7/src/Response/V1/GetLeaguesResponse.py
--rw-rw-rw-   0        0        0      636 2022-01-31 16:49:23.000000 oddsjam-api-0.2.7/src/Response/V1/GetMarketsResponse.py
--rw-rw-rw-   0        0        0     1015 2022-01-31 16:49:27.000000 oddsjam-api-0.2.7/src/Response/V1/GetOddsResponse.py
--rw-rw-rw-   0        0        0      895 2022-01-31 16:49:31.000000 oddsjam-api-0.2.7/src/Response/V1/GetScoresResponse.py
--rw-rw-rw-   0        0        0      363 2022-01-31 13:55:06.000000 oddsjam-api-0.2.7/src/Response/V1/__init__.py
-drwxrwxrwx   0        0        0        0 2022-01-31 21:25:33.365481 oddsjam-api-0.2.7/src/Response/V2/
--rw-rw-rw-   0        0        0      725 2022-01-31 16:49:36.000000 oddsjam-api-0.2.7/src/Response/V2/GetFutureOddsResponse.py
--rw-rw-rw-   0        0        0      574 2022-01-31 16:49:42.000000 oddsjam-api-0.2.7/src/Response/V2/GetFuturesResponse.py
--rw-rw-rw-   0        0        0      558 2022-01-31 16:49:47.000000 oddsjam-api-0.2.7/src/Response/V2/GetGamesResponse.py
--rw-rw-rw-   0        0        0      527 2022-01-31 16:49:51.000000 oddsjam-api-0.2.7/src/Response/V2/GetLeaguesResponse.py
--rw-rw-rw-   0        0        0      636 2022-01-31 16:50:00.000000 oddsjam-api-0.2.7/src/Response/V2/GetMarketsResponse.py
--rw-rw-rw-   0        0        0     1008 2022-01-31 20:34:15.000000 oddsjam-api-0.2.7/src/Response/V2/GetOddsResponse.py
--rw-rw-rw-   0        0        0      895 2022-01-31 16:50:10.000000 oddsjam-api-0.2.7/src/Response/V2/GetScoresResponse.py
--rw-rw-rw-   0        0        0      363 2022-01-31 16:08:28.000000 oddsjam-api-0.2.7/src/Response/V2/__init__.py
--rw-rw-rw-   0        0        0        0 2022-01-31 16:33:28.000000 oddsjam-api-0.2.7/src/Response/__init__.py
-drwxrwxrwx   0        0        0        0 2022-01-31 21:25:33.382481 oddsjam-api-0.2.7/src/oddsjam_api.egg-info/
--rw-rw-rw-   0        0        0     4953 2022-01-31 21:25:33.000000 oddsjam-api-0.2.7/src/oddsjam_api.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2221 2022-01-31 21:25:33.000000 oddsjam-api-0.2.7/src/oddsjam_api.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-01-31 21:25:33.000000 oddsjam-api-0.2.7/src/oddsjam_api.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       43 2022-01-31 21:25:33.000000 oddsjam-api-0.2.7/src/oddsjam_api.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:09:14.155375 oddsjam-api-0.2.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-18 15:09:02.000000 oddsjam-api-0.2.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4958 2023-05-18 15:09:14.151375 oddsjam-api-0.2.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4401 2023-05-18 15:09:02.000000 oddsjam-api-0.2.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      654 2023-05-18 15:09:04.000000 oddsjam-api-0.2.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-18 15:09:14.155375 oddsjam-api-0.2.8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:09:14.139375 oddsjam-api-0.2.8/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:09:14.139375 oddsjam-api-0.2.8/src/Base/
+-rw-r--r--   0 runner    (1001) docker     (123)      825 2023-05-18 15:09:02.000000 oddsjam-api-0.2.8/src/Base/CustomExceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-18 15:09:02.000000 oddsjam-api-0.2.8/src/Base/EnforceTypes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      443 2023-05-18 15:09:02.000000 oddsjam-api-0.2.8/src/Base/ModelBase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-05-18 15:09:02.000000 oddsjam-api-0.2.8/src/Base/RequestBase.py
+-rw-r--r--   0 runner    (1001) docker     (123)      510 2023-05-18 15:09:02.000000 oddsjam-api-0.2.8/src/Base/ResponseBase.py
+-rw-r--r--   0 runner    (1001) docker     (123)      681 2023-05-18 15:09:02.000000 oddsjam-api-0.2.8/src/Base/ValidParameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-05-18 15:09:02.000000 oddsjam-api-0.2.8/src/Base/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:09:14.139375 oddsjam-api-0.2.8/src/Models/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:09:14.143375 oddsjam-api-0.2.8/src/Models/V1/
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-05-18 15:09:02.000000 oddsjam-api-0.2.8/src/Models/V1/Future.py
+-rw-r--r--   0 runner    (1001) docker     (123)      331 2023-05-18 15:09:02.000000 oddsjam-api-0.2.8/src/Models/V1/FutureOdds.py
+-rw-r--r--   0 runner    (1001) docker     (123)      306 2023-05-18 15:09:02.000000 oddsjam-api-0.2.8/src/Models/V1/Game.py
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-05-18 15:09:02.000000 oddsjam-api-0.2.8/src/Models/V1/League.py
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-05-18 15:09:02.000000 oddsjam-api-0.2.8/src/Models/V1/Market.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-05-18 15:09:02.000000 oddsjam-api-0.2.8/src/Models/V1/Odds.py
+-rw-r--r--   0 runner    (1001) docker     (123)      214 2023-05-18 15:09:02.000000 oddsjam-api-0.2.8/src/Models/V1/PeriodScore.py
+-rw-r--r--   0 runner    (1001) docker     (123)      630 2023-05-18 15:09:02.000000 oddsjam-api-0.2.8/src/Models/V1/Score.py
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-05-18 15:09:02.000000 oddsjam-api-0.2.8/src/Models/V1/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:09:14.143375 oddsjam-api-0.2.8/src/Models/V2/
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-05-18 15:09:02.000000 oddsjam-api-0.2.8/src/Models/V2/Future.py
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-05-18 15:09:02.000000 oddsjam-api-0.2.8/src/Models/V2/FutureOdds.py
+-rw-r--r--   0 runner    (1001) docker     (123)      306 2023-05-18 15:09:02.000000 oddsjam-api-0.2.8/src/Models/V2/Game.py
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-05-18 15:09:02.000000 oddsjam-api-0.2.8/src/Models/V2/League.py
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-05-18 15:09:02.000000 oddsjam-api-0.2.8/src/Models/V2/Market.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1365 2023-05-18 15:09:02.000000 oddsjam-api-0.2.8/src/Models/V2/Odds.py
+-rw-r--r--   0 runner    (1001) docker     (123)      214 2023-05-18 15:09:02.000000 oddsjam-api-0.2.8/src/Models/V2/PeriodScore.py
+-rw-r--r--   0 runner    (1001) docker     (123)      630 2023-05-18 15:09:02.000000 oddsjam-api-0.2.8/src/Models/V2/Score.py
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-05-18 15:09:02.000000 oddsjam-api-0.2.8/src/Models/V2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 15:09:02.000000 oddsjam-api-0.2.8/src/Models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:09:14.143375 oddsjam-api-0.2.8/src/OddsJamClient/
+-rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-05-18 15:09:02.000000 oddsjam-api-0.2.8/src/OddsJamClient/OddsJamClient.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:09:14.143375 oddsjam-api-0.2.8/src/OddsJamClient/V1/
+-rw-r--r--   0 runner    (1001) docker     (123)     3308 2023-05-18 15:09:02.000000 oddsjam-api-0.2.8/src/OddsJamClient/V1/Requestor.py
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-05-18 15:09:02.000000 oddsjam-api-0.2.8/src/OddsJamClient/V1/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:09:14.147375 oddsjam-api-0.2.8/src/OddsJamClient/V2/
+-rw-r--r--   0 runner    (1001) docker     (123)     3559 2023-05-18 15:09:02.000000 oddsjam-api-0.2.8/src/OddsJamClient/V2/Requestor.py
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-05-18 15:09:02.000000 oddsjam-api-0.2.8/src/OddsJamClient/V2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-18 15:09:02.000000 oddsjam-api-0.2.8/src/OddsJamClient/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:09:14.147375 oddsjam-api-0.2.8/src/Request/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:09:14.147375 oddsjam-api-0.2.8/src/Request/V1/
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-05-18 15:09:02.000000 oddsjam-api-0.2.8/src/Request/V1/GetFutureOddsRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-05-18 15:09:02.000000 oddsjam-api-0.2.8/src/Request/V1/GetFuturesRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2023-05-18 15:09:02.000000 oddsjam-api-0.2.8/src/Request/V1/GetGamesRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-05-18 15:09:02.000000 oddsjam-api-0.2.8/src/Request/V1/GetLeaguesRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-05-18 15:09:02.000000 oddsjam-api-0.2.8/src/Request/V1/GetMarketsRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      432 2023-05-18 15:09:02.000000 oddsjam-api-0.2.8/src/Request/V1/GetOddsRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2023-05-18 15:09:02.000000 oddsjam-api-0.2.8/src/Request/V1/GetScoresRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-05-18 15:09:02.000000 oddsjam-api-0.2.8/src/Request/V1/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:09:14.147375 oddsjam-api-0.2.8/src/Request/V2/
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-05-18 15:09:02.000000 oddsjam-api-0.2.8/src/Request/V2/GetFutureOddsRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      309 2023-05-18 15:09:02.000000 oddsjam-api-0.2.8/src/Request/V2/GetFuturesRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      463 2023-05-18 15:09:02.000000 oddsjam-api-0.2.8/src/Request/V2/GetGamesRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-05-18 15:09:02.000000 oddsjam-api-0.2.8/src/Request/V2/GetLeaguesRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-05-18 15:09:02.000000 oddsjam-api-0.2.8/src/Request/V2/GetMarketsRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      448 2023-05-18 15:09:02.000000 oddsjam-api-0.2.8/src/Request/V2/GetOddsRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      275 2023-05-18 15:09:02.000000 oddsjam-api-0.2.8/src/Request/V2/GetScoresRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-05-18 15:09:02.000000 oddsjam-api-0.2.8/src/Request/V2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 15:09:02.000000 oddsjam-api-0.2.8/src/Request/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:09:14.147375 oddsjam-api-0.2.8/src/Response/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:09:14.151375 oddsjam-api-0.2.8/src/Response/V1/
+-rw-r--r--   0 runner    (1001) docker     (123)      693 2023-05-18 15:09:02.000000 oddsjam-api-0.2.8/src/Response/V1/GetFutureOddsResponse.py
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-05-18 15:09:02.000000 oddsjam-api-0.2.8/src/Response/V1/GetFuturesResponse.py
+-rw-r--r--   0 runner    (1001) docker     (123)      488 2023-05-18 15:09:02.000000 oddsjam-api-0.2.8/src/Response/V1/GetGamesResponse.py
+-rw-r--r--   0 runner    (1001) docker     (123)      514 2023-05-18 15:09:02.000000 oddsjam-api-0.2.8/src/Response/V1/GetLeaguesResponse.py
+-rw-r--r--   0 runner    (1001) docker     (123)      617 2023-05-18 15:09:02.000000 oddsjam-api-0.2.8/src/Response/V1/GetMarketsResponse.py
+-rw-r--r--   0 runner    (1001) docker     (123)      982 2023-05-18 15:09:02.000000 oddsjam-api-0.2.8/src/Response/V1/GetOddsResponse.py
+-rw-r--r--   0 runner    (1001) docker     (123)      871 2023-05-18 15:09:02.000000 oddsjam-api-0.2.8/src/Response/V1/GetScoresResponse.py
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-05-18 15:09:02.000000 oddsjam-api-0.2.8/src/Response/V1/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:09:14.151375 oddsjam-api-0.2.8/src/Response/V2/
+-rw-r--r--   0 runner    (1001) docker     (123)      705 2023-05-18 15:09:02.000000 oddsjam-api-0.2.8/src/Response/V2/GetFutureOddsResponse.py
+-rw-r--r--   0 runner    (1001) docker     (123)      557 2023-05-18 15:09:02.000000 oddsjam-api-0.2.8/src/Response/V2/GetFuturesResponse.py
+-rw-r--r--   0 runner    (1001) docker     (123)      541 2023-05-18 15:09:02.000000 oddsjam-api-0.2.8/src/Response/V2/GetGamesResponse.py
+-rw-r--r--   0 runner    (1001) docker     (123)      511 2023-05-18 15:09:02.000000 oddsjam-api-0.2.8/src/Response/V2/GetLeaguesResponse.py
+-rw-r--r--   0 runner    (1001) docker     (123)      617 2023-05-18 15:09:02.000000 oddsjam-api-0.2.8/src/Response/V2/GetMarketsResponse.py
+-rw-r--r--   0 runner    (1001) docker     (123)      975 2023-05-18 15:09:02.000000 oddsjam-api-0.2.8/src/Response/V2/GetOddsResponse.py
+-rw-r--r--   0 runner    (1001) docker     (123)      871 2023-05-18 15:09:02.000000 oddsjam-api-0.2.8/src/Response/V2/GetScoresResponse.py
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-05-18 15:09:02.000000 oddsjam-api-0.2.8/src/Response/V2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 15:09:02.000000 oddsjam-api-0.2.8/src/Response/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-18 15:09:02.000000 oddsjam-api-0.2.8/src/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:09:14.151375 oddsjam-api-0.2.8/src/oddsjam_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4958 2023-05-18 15:09:14.000000 oddsjam-api-0.2.8/src/oddsjam_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2227 2023-05-18 15:09:14.000000 oddsjam-api-0.2.8/src/oddsjam_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 15:09:14.000000 oddsjam-api-0.2.8/src/oddsjam_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-18 15:09:14.000000 oddsjam-api-0.2.8/src/oddsjam_api.egg-info/top_level.txt
```

### Comparing `oddsjam-api-0.2.7/PKG-INFO` & `oddsjam-api-0.2.8/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,146 +1,136 @@
-Metadata-Version: 2.1
-Name: oddsjam-api
-Version: 0.2.7
-Summary: A lightweight wrapper for the OddsJam API
-Home-page: https://github.com/cooperbrandon1/oddsjam-api/
-Author: Brandon Cooper
-Author-email: cooper.brandon@outlook.com
-License: UNKNOWN
-Project-URL: Bug Tracker, https://github.com/cooperbrandon1/oddsjam-api/issues
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# <code>oddsjam-api</code>: A lightweight OddsJam API wrapper
-
-## V2 Update
-V2 support is now available for the new endpoints/models listed at the [OddsJam Developer Page](https://developer.oddsjam.com/).  The client exposed by this package is backwards compatible, and runs in v1 by default. Versions can be switched as follows:
-``` python
-    from OddsJamClient import OddsJamClient;
-    Client = OddsJamClient(YOUR_API_KEY);
-    v1Results = Client.GetLeagues(); #Default v1 endpoints
-
-    Client.UseV2();
-    v2Results = Client.GetLeagues(); #v2 endpoints
-```
-
-This update comes with the following changes:
-<ul>
-<li>Type hinting for function calls is no longer available. Function calls will appear with <code>(*args: Any, **kwargs:Any) -> Any</code>. Please refer to the developer documentation for valid arguments.</li>
-<li>The V2 client does <strong>not</strong> contain a GetMarkets() function.</li>
-<li>The V2 client requires <i>at least one</i> argument for the GetOdds() function. This is due to the amount of data returned from the new V2 endpoint. Attempting a call to GetOdds() <i>without</i> a parameter will result in an <code>InvalidGetOddsV2Error</code>, and the endpoint will <i>not</i> be hit.</li>
-</ul>
-<br/>
-
-## What is <code>oddsjam-api</code>?
-<code>oddsjam-api</code> is a fast, lightweight wrapper for the [OddsJam API](https://developer.oddsjam.com/). It strives to be as intuitive to use as possible, providing strongly typed requests and responses to ensure predictability and consistency.
-
-
-
-## How do I use it?
-Start by installing the <code>oddsjam-api</code> package (currently only on TestPyPI):
-``` 
-    pip install oddsjam-api
-```
-
-Create an instance of the <code>OddsJamClient</code>:
-
-``` python
-    from OddsJamClient import OddsJamClient;
-    Client = OddsJamClient(YOUR_API_KEY);
-```
-
-Then simply call whichever function you'd like to:
-
-``` python 
-    from OddsJamClient import OddsJamClient;
-    Client = OddsJamClient(YOUR_API_KEY);
-    GamesResponse = Client.GetGames();
-```
-
-Parameters are not required for any function call, but can be provided as desired:
-
-``` python
-    from OddsJamClient import OddsJamClient;
-    Client = OddsJamClient(YOUR_API_KEY);
-    GamesResponse = Client.GetGames(league='ncaa', sport='football');
-```
-
-Parameters will raise specific errors:
-
-``` python
-    GamesResponse = Client.GetGames(sport='curling'); 
-    #Raises SportError, with a list of valid values
-
-    OddsResponse = Client.GetOdds(sportsbook='212 Bet');
-    #Raises SportsBookError, with a list of valid values
-```
-
-Note: Sport and SportsBook parameters are *case insensitive*
-
-Accessing the object of a response requires accessing the response's object:
-
-``` python    
-    from OddsJamClient import OddsJamClient;
-    Client = OddsJamClient(YOUR_API_KEY);
-    GamesResponse = Client.GetGames();
-    Games = GamesResponse.Games;
-```
-
-List comprehension can also be used to access objects:
-
-``` python
-    AwayTeams = [g.away_team for g in GamesResponse.Games];
-```
-
-Nested objects can be accessed similarly:
-
-``` python
-    OddsResponse = Client.GetOdds();
-    print(OddsResponse.Odds[0].game.sport)
-```
-
-The raw response from the API is also accessible via the *RawResponse* property of any *Response* object:
-
-``` python
-    Raw = GamesResponse.RawResponse;
-    Jobj = json.loads(raw);
-```
-
-## Built-in functions
-Convert entire Odds collection to decimal, then back to American:
-``` python
-    OddsResponse = Client.GetOdds();
-    OddsResponse.AsDecimal();
-    OddsResponse.AsAmerican();
-```
-
-Convert individual Odds object to decimal, then back to American:
-``` python
-    OddsResponse = Client.GetOdds();
-    FirstOdd = OddsResponse.Odds[0];
-    FirstOdd.AsDecimal();
-    FirstOdd.AsAmerican();
-```
-
-## Example usage
-Flatten and output data using pandas:
-``` python
-    import pandas as pd;
-    from OddsJamClient import OddsJamClient;
-
-    Client = OddsJamClient(YOUR_API_KEY);
-    Odds = Client.GetOdds().Odds;
-    df = pd.DataFrame(Odds);
-
-    #Lambda over rows to extract just the ID from the 'game' object in each row
-    df['game'] = df.apply(lambda row: row['game']['id'], axis=1)
-    
-    #Get odds for Moneyline markets only
-    df = df.loc[df['market_name'] == 'Moneyline']
-```
-
+# <code>oddsjam-api</code>: A lightweight OddsJam API wrapper
+
+## V2 Update
+V2 support is now available for the new endpoints/models listed at the [OddsJam Developer Page](https://developer.oddsjam.com/).  The client exposed by this package is backwards compatible, and runs in v1 by default. Versions can be switched as follows:
+``` python
+    from OddsJamClient import OddsJamClient;
+    Client = OddsJamClient(YOUR_API_KEY);
+    v1Results = Client.GetLeagues(); #Default v1 endpoints
+
+    Client.UseV2();
+    v2Results = Client.GetLeagues(); #v2 endpoints
+```
+
+This update comes with the following changes:
+<ul>
+<li>Type hinting for function calls is no longer available. Function calls will appear with <code>(*args: Any, **kwargs:Any) -> Any</code>. Please refer to the developer documentation for valid arguments.</li>
+<li>The V2 client does <strong>not</strong> contain a GetMarkets() function.</li>
+<li>The V2 client requires <i>at least one</i> argument for the GetOdds() function. This is due to the amount of data returned from the new V2 endpoint. Attempting a call to GetOdds() <i>without</i> a parameter will result in an <code>InvalidGetOddsV2Error</code>, and the endpoint will <i>not</i> be hit.</li>
+</ul>
+<br/>
+
+## What is <code>oddsjam-api</code>?
+<code>oddsjam-api</code> is a fast, lightweight wrapper for the [OddsJam API](https://developer.oddsjam.com/). It strives to be as intuitive to use as possible, providing strongly typed requests and responses to ensure predictability and consistency.
+
+
+
+## How do I use it?
+Start by installing the <code>oddsjam-api</code> package (currently only on TestPyPI):
+``` 
+    pip install oddsjam-api
+```
+
+Create an instance of the <code>OddsJamClient</code>:
+
+``` python
+    from OddsJamClient import OddsJamClient;
+    Client = OddsJamClient(YOUR_API_KEY);
+```
+
+Then simply call whichever function you'd like to:
+
+``` python 
+    from OddsJamClient import OddsJamClient;
+    Client = OddsJamClient(YOUR_API_KEY);
+    GamesResponse = Client.GetGames();
+```
+
+Parameters are not required for any function call, but can be provided as desired:
+
+``` python
+    from OddsJamClient import OddsJamClient;
+    Client = OddsJamClient(YOUR_API_KEY);
+    GamesResponse = Client.GetGames(league='ncaa', sport='football');
+```
+
+Parameters will raise specific errors:
+
+``` python
+    GamesResponse = Client.GetGames(sport='curling'); 
+    #Raises SportError, with a list of valid values
+
+    OddsResponse = Client.GetOdds(sportsbook='212 Bet');
+    #Raises SportsBookError, with a list of valid values
+```
+
+Note: Sport and SportsBook parameters are *case insensitive*
+
+Accessing the object of a response requires accessing the response's object:
+
+``` python    
+    from OddsJamClient import OddsJamClient;
+    Client = OddsJamClient(YOUR_API_KEY);
+    GamesResponse = Client.GetGames();
+    Games = GamesResponse.Games;
+```
+
+List comprehension can also be used to access objects:
+
+``` python
+    AwayTeams = [g.away_team for g in GamesResponse.Games];
+```
+
+Nested objects can be accessed similarly:
+
+``` python
+    OddsResponse = Client.GetOdds();
+    print(OddsResponse.Odds[0].game.sport)
+```
+
+The raw response from the API is also accessible via the *RawResponse* property of any *Response* object:
+
+``` python
+    Raw = GamesResponse.RawResponse;
+    Jobj = json.loads(raw);
+```
+
+## Built-in functions
+Convert entire Odds collection to decimal, then back to American:
+``` python
+    OddsResponse = Client.GetOdds();
+    OddsResponse.AsDecimal();
+    OddsResponse.AsAmerican();
+```
+
+Convert individual Odds object to decimal, then back to American:
+``` python
+    OddsResponse = Client.GetOdds();
+    FirstOdd = OddsResponse.Odds[0];
+    FirstOdd.AsDecimal();
+    FirstOdd.AsAmerican();
+```
+
+## Example usage
+Flatten and output data using pandas:
+``` python
+    import pandas as pd;
+    from OddsJamClient import OddsJamClient;
+
+    Client = OddsJamClient(YOUR_API_KEY);
+    Odds = Client.GetOdds().Odds;
+    df = pd.DataFrame(Odds);
+
+    #Lambda over rows to extract just the ID from the 'game' object in each row
+    df['game'] = df.apply(lambda row: row['game']['id'], axis=1)
+    
+    #Get odds for Moneyline markets only
+    df = df.loc[df['market_name'] == 'Moneyline']
+```
+
+# PyPi
+
+* Prod: https://pypi.org/project/oddsjam-api
+* Test: https://test.pypi.org/project/oddsjam-api-test
+
+
+ORIGINAL CREDIT GOES TO https://github.com/cooperbrandon1
```

### Comparing `oddsjam-api-0.2.7/src/Base/CustomExceptions.py` & `oddsjam-api-0.2.8/src/Base/CustomExceptions.py`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-import Base;
-
-class SportError(Exception):
-    def __init__(self, *args: object) -> None:
-        b = ', '.join(map(str,Base.ValidParameters.ValidSports));
-        self.message = 'Sport parameter must be one of the following values (case insensitive): ' + b;
-        super().__init__(self.message);
-
-class SportsBookError(Exception):
-    def __init__(self, *args: object) -> None:
-        b = ', '.join(map(str,Base.ValidParameters.ValidSportsBooks));
-        self.message = 'SportsBook parameter must be one of the following values (case insensitive): ' + b;
-        super().__init__(self.message);
-
-        
-class InvalidGetOddsV2Error(Exception):
-    def __init__(self, *args: object) -> None:
-        self.message = 'The v2 GetOdds function requires at least one valid parameter.';
+import Base;
+
+class SportError(Exception):
+    def __init__(self, *args: object) -> None:
+        b = ', '.join(map(str,Base.ValidParameters.ValidSports));
+        self.message = 'Sport parameter must be one of the following values (case insensitive): ' + b;
+        super().__init__(self.message);
+
+class SportsBookError(Exception):
+    def __init__(self, *args: object) -> None:
+        b = ', '.join(map(str,Base.ValidParameters.ValidSportsBooks));
+        self.message = 'SportsBook parameter must be one of the following values (case insensitive): ' + b;
+        super().__init__(self.message);
+
+        
+class InvalidGetOddsV2Error(Exception):
+    def __init__(self, *args: object) -> None:
+        self.message = 'The v2 GetOdds function requires at least one valid parameter.';
         super().__init__(self.message);
```

### Comparing `oddsjam-api-0.2.7/src/Base/EnforceTypes.py` & `oddsjam-api-0.2.8/src/Base/EnforceTypes.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,24 +1,24 @@
-#region Imports
-from dataclasses import fields;
-from datetime import date
-from Base.ValidParameters import ValidSports, ValidSportsBooks;
-from Base.CustomExceptions import SportError, SportsBookError;
-#endregion Imports
-
-def EnforceTypes(cls):
-    field_types = {field.name: field.type for field in fields(cls)}
-    for f in field_types:
-        classAttr = getattr(cls,f);
-        if(classAttr != None):
-            if(f == 'sport' and classAttr not in ValidSports):
-                raise SportError();
-            elif((f == 'sportsbook' and classAttr not in ValidSportsBooks) or (f =='sports_book_name' and classAttr not in ValidSportsBooks)):
-                raise SportsBookError();
-            elif(isinstance(classAttr,field_types[f]) == False):
-                raise TypeError(f + ' must be of type ' + field_types[f].__name__);
-            elif('Date' in f):
-                try:
-                    date.fromisoformat(classAttr);
-                except:
-                    raise ValueError(f + ' must be in ISO-8601 format (ex. 11-01-2021)');
+#region Imports
+from dataclasses import fields;
+from datetime import date
+from Base.ValidParameters import ValidSports, ValidSportsBooks;
+from Base.CustomExceptions import SportError, SportsBookError;
+#endregion Imports
+
+def EnforceTypes(cls):
+    field_types = {field.name: field.type for field in fields(cls)}
+    for f in field_types:
+        classAttr = getattr(cls,f);
+        if(classAttr != None):
+            if(f == 'sport' and classAttr not in ValidSports):
+                raise SportError();
+            elif((f == 'sportsbook' and classAttr not in ValidSportsBooks) or (f =='sports_book_name' and classAttr not in ValidSportsBooks)):
+                raise SportsBookError();
+            elif(isinstance(classAttr,field_types[f]) == False):
+                raise TypeError(f + ' must be of type ' + field_types[f].__name__);
+            elif('Date' in f):
+                try:
+                    date.fromisoformat(classAttr);
+                except:
+                    raise ValueError(f + ' must be in ISO-8601 format (ex. 11-01-2021)');
     return cls;
```

### Comparing `oddsjam-api-0.2.7/src/Base/RequestBase.py` & `oddsjam-api-0.2.8/src/Base/RequestBase.py`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,29 +1,29 @@
-#region Imports
-from Base.EnforceTypes import EnforceTypes;
-from Base.ValidParameters import ValidSportsBooks, ValidSports;
-from Base.CustomExceptions import SportError;
-#endregion Imports
-
-class RequestBase:
-
-    @classmethod
-    def GetArgString(cls):  
-        #Get the list of attributes of the given subclass 
-        props = [i for i in cls.__dict__.keys() if i[:1] != '_' and i != 'ApiPath'];
-        #Get any populated attributes (e.g Sport = Sports.Football)
-        #And convert them to a type that can be appended to a querystring
-        #Not using urllib here 
-        arguments = {p:cls.ConvertArg(getattr(cls,p)) for p in props if getattr(cls,p) != None}
-        argStr = '&'
-        argStr = ('&'.join("{!s}={!s}".format(key.lower(),val.lower().replace("'",'')) for (key,val) in arguments.items()))
-        if(len(argStr) > 1):
-            return argStr;
-        return '';
-    
-    @classmethod
-    def ConvertArg(cls,arg):
-        if(type(arg) is int):
-            return str(arg)
-
-    def __post_init__(cls):
-        EnforceTypes(cls);
+#region Imports
+from Base.EnforceTypes import EnforceTypes;
+from Base.ValidParameters import ValidSportsBooks, ValidSports;
+from Base.CustomExceptions import SportError;
+#endregion Imports
+
+class RequestBase:
+
+    @classmethod
+    def GetArgString(cls):  
+        #Get the list of attributes of the given subclass 
+        props = [i for i in cls.__dict__.keys() if i[:1] != '_' and i != 'ApiPath'];
+        #Get any populated attributes (e.g Sport = Sports.Football)
+        #And convert them to a type that can be appended to a querystring
+        #Not using urllib here 
+        arguments = {p:cls.ConvertArg(getattr(cls,p)) for p in props if getattr(cls,p) != None}
+        argStr = '&'
+        argStr = ('&'.join("{!s}={!s}".format(key.lower(),val.lower().replace("'",'')) for (key,val) in arguments.items()))
+        if(len(argStr) > 1):
+            return argStr;
+        return '';
+    
+    @classmethod
+    def ConvertArg(cls,arg):
+        if(type(arg) is int):
+            return str(arg)
+
+    def __post_init__(cls):
+        EnforceTypes(cls);
```

### Comparing `oddsjam-api-0.2.7/src/Base/ValidParameters.py` & `oddsjam-api-0.2.8/src/Base/ValidParameters.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1,2 +1,2 @@
-ValidSports = ['football', 'basketball', 'baseball', 'mma', 'boxing', 'hockey', 'soccer', 'tennis', 'golf', 'motorsports', 'esports']
+ValidSports = ['football', 'basketball', 'baseball', 'mma', 'boxing', 'hockey', 'soccer', 'tennis', 'golf', 'motorsports', 'esports']
 ValidSportsBooks = ['5Dimes','10bet','888sport','888sport (Canada)','Bally Bet','Barstool','BetAnySports','Betfair','Betfred','BetMGM','BetOnline','BetRivers','BetUS','Betway','Bodog','BookMaker','Borgata','Bovada','bwin','Caesars','Casumo','Circa Sports','Circa Vegas','ComeOn!','DraftKings','Elite Sportsbook','FanDuel','FOX Bet','Four Winds','Golden Nugget','Heritage','Ladbrokes','LeoVegas','MyBookie','OddsJam','Parx','PointsBet','SI','SugarHouse','SuperBook','theScore','TwinSpires','Unibet','Westgate','William Hill','Wind Creek','WynnBET']
```

### Comparing `oddsjam-api-0.2.7/src/Models/V1/Odds.py` & `oddsjam-api-0.2.8/src/Models/V1/Odds.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,47 +1,47 @@
-#region Imports
-import datetime;
-from dataclasses import dataclass;
-from Models.V1 import Game;
-from Base import ModelBase;
-#endregion Imports
-
-@dataclass
-class Odds(ModelBase):
-    game: Game = None
-    market_name: str = None
-    sports_book: str = None
-    name: str = None
-    price: float = None
-    is_main: bool = None
-    is_live: bool = None
-    checked_date: datetime = None
-    changed_date: datetime = None
-    __type__ = 'American';
-    
-    def AsDecimal(self):
-        try:
-            if(self.__type__ != 'Decimal'):
-                if(self.price < 0):
-                    self.price = 1 + (100/(self.price*-1))
-                elif self.price > 0:
-                    self.price = (self.price/100) + 1
-                self.__type__ = 'Decimal'
-            else:
-                print('Already decimal');
-        except Exception as ex:
-            return ex;
-    
-    def AsAmerican(self):
-        try:
-            if(self.__type__ != 'American'):
-                if(self.__type__ == 'Decimal'):
-                    if(self.price > 2):
-                        self.price = (self.price - 1) * 100
-                    else:
-                        self.price = (-100) / (self.price-1)
-                    self.price = round(self.price,1);
-                self.__type__ = 'American'
-            else:
-                print('Already American')
-        except Exception as ex:
+#region Imports
+import datetime;
+from dataclasses import dataclass;
+from Models.V1 import Game;
+from Base import ModelBase;
+#endregion Imports
+
+@dataclass
+class Odds(ModelBase):
+    game: Game = None
+    market_name: str = None
+    sports_book: str = None
+    name: str = None
+    price: float = None
+    is_main: bool = None
+    is_live: bool = None
+    checked_date: datetime = None
+    changed_date: datetime = None
+    __type__ = 'American';
+    
+    def AsDecimal(self):
+        try:
+            if(self.__type__ != 'Decimal'):
+                if(self.price < 0):
+                    self.price = 1 + (100/(self.price*-1))
+                elif self.price > 0:
+                    self.price = (self.price/100) + 1
+                self.__type__ = 'Decimal'
+            else:
+                print('Already decimal');
+        except Exception as ex:
+            return ex;
+    
+    def AsAmerican(self):
+        try:
+            if(self.__type__ != 'American'):
+                if(self.__type__ == 'Decimal'):
+                    if(self.price > 2):
+                        self.price = (self.price - 1) * 100
+                    else:
+                        self.price = (-100) / (self.price-1)
+                    self.price = round(self.price,1);
+                self.__type__ = 'American'
+            else:
+                print('Already American')
+        except Exception as ex:
             return ex;
```

### Comparing `oddsjam-api-0.2.7/src/Models/V1/Score.py` & `oddsjam-api-0.2.8/src/Models/V1/Score.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,24 +1,24 @@
-#region Imports
-from Base import ModelBase;
-from Models.V1 import Game;
-from datetime import datetime;
-from dataclasses import dataclass;
-#endregion Imports
-
-@dataclass
-class Score(ModelBase):
-    game: Game = None;
-    period_scores: list = None;
-    season_type: str = None;
-    season_week: str = None;
-    description: str = None;
-    venue_name: str = None;
-    venue_location: str = None;
-    status: str = None;
-    period: str = None;
-    clock: str = None;
-    last_play: str = None;
-    home_final_score: int = None;
-    away_final_score: int = None;
-    checked_date: datetime = None;
+#region Imports
+from Base import ModelBase;
+from Models.V1 import Game;
+from datetime import datetime;
+from dataclasses import dataclass;
+#endregion Imports
+
+@dataclass
+class Score(ModelBase):
+    game: Game = None;
+    period_scores: list = None;
+    season_type: str = None;
+    season_week: str = None;
+    description: str = None;
+    venue_name: str = None;
+    venue_location: str = None;
+    status: str = None;
+    period: str = None;
+    clock: str = None;
+    last_play: str = None;
+    home_final_score: int = None;
+    away_final_score: int = None;
+    checked_date: datetime = None;
     changed_date: datetime = None;
```

### Comparing `oddsjam-api-0.2.7/src/OddsJamClient/OddsJamClient.py` & `oddsjam-api-0.2.8/src/OddsJamClient/OddsJamClient.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,41 +1,41 @@
-#region Imports
-from __future__ import annotations;
-import Base;
-import requests;
-from OddsJamClient.V1 import v1Requestor;
-from OddsJamClient.V2 import v2Requestor;
-import types;
-#endregion Imports
-
-class OddsJamClient():
-    def __init__(self,APIKEY:str):
-        self.APIKEY = APIKEY;
-        self.BaseUrl = 'https://api-external.oddsjam.com/api/';
-        self.V1Requestor = v1Requestor;
-        self.V2Requestor = v2Requestor;
-        self.UseV1();
-
-    def UseV1(self):
-        self.Version = 1;
-        self.GetFutureOdds = types.MethodType(v1Requestor.GetFutureOdds, self);
-        self.GetFutures = types.MethodType(v1Requestor.GetFutures, self);
-        self.GetGames = types.MethodType(v1Requestor.GetGames, self);
-        self.GetLeagues = types.MethodType(v1Requestor.GetLeagues, self);
-        # self.GetMarkets = types.MethodType(v1Requestor.GetMarkets, self);
-        self.GetOdds = types.MethodType(v1Requestor.GetOdds, self);
-        self.GetScores = types.MethodType(v1Requestor.GetScores, self);
-    
-    def UseV2(self):
-        self.Version = 2;
-        self.GetFutureOdds = types.MethodType(v2Requestor.GetFutureOdds, self);
-        self.GetFutures = types.MethodType(v2Requestor.GetFutures, self);
-        self.GetGames = types.MethodType(v2Requestor.GetGames, self);
-        self.GetLeagues = types.MethodType(v2Requestor.GetLeagues, self);
-        self.GetMarkets = types.MethodType(v2Requestor.GetMarkets, self);
-        self.GetOdds = types.MethodType(v2Requestor.GetOdds, self);
-        self.GetScores = types.MethodType(v2Requestor.GetScores, self);
-
-    def SendRequest(self, request: Base.RequestBase):
-        return requests.get(self.BaseUrl + request.ApiPath() + '?key=' + self.APIKEY, request.__dict__).text;
-
+#region Imports
+from __future__ import annotations;
+import Base;
+import requests;
+from OddsJamClient.V1 import v1Requestor;
+from OddsJamClient.V2 import v2Requestor;
+import types;
+#endregion Imports
+
+class OddsJamClient():
+    def __init__(self,APIKEY:str):
+        self.APIKEY = APIKEY;
+        self.BaseUrl = 'https://api-external.oddsjam.com/api/';
+        self.V1Requestor = v1Requestor;
+        self.V2Requestor = v2Requestor;
+        self.UseV1();
+
+    def UseV1(self):
+        self.Version = 1;
+        self.GetFutureOdds = types.MethodType(v1Requestor.GetFutureOdds, self);
+        self.GetFutures = types.MethodType(v1Requestor.GetFutures, self);
+        self.GetGames = types.MethodType(v1Requestor.GetGames, self);
+        self.GetLeagues = types.MethodType(v1Requestor.GetLeagues, self);
+        # self.GetMarkets = types.MethodType(v1Requestor.GetMarkets, self);
+        self.GetOdds = types.MethodType(v1Requestor.GetOdds, self);
+        self.GetScores = types.MethodType(v1Requestor.GetScores, self);
+    
+    def UseV2(self):
+        self.Version = 2;
+        self.GetFutureOdds = types.MethodType(v2Requestor.GetFutureOdds, self);
+        self.GetFutures = types.MethodType(v2Requestor.GetFutures, self);
+        self.GetGames = types.MethodType(v2Requestor.GetGames, self);
+        self.GetLeagues = types.MethodType(v2Requestor.GetLeagues, self);
+        self.GetMarkets = types.MethodType(v2Requestor.GetMarkets, self);
+        self.GetOdds = types.MethodType(v2Requestor.GetOdds, self);
+        self.GetScores = types.MethodType(v2Requestor.GetScores, self);
+
+    def SendRequest(self, request: Base.RequestBase):
+        return requests.get(self.BaseUrl + request.ApiPath() + '?key=' + self.APIKEY, request.__dict__).text;
+
```

### Comparing `oddsjam-api-0.2.7/src/OddsJamClient/V1/Requestor.py` & `oddsjam-api-0.2.8/src/OddsJamClient/V1/Requestor.py`

 * *Ordering differences only*

 * *Files 7% similar despite different names*

```diff
@@ -1,71 +1,71 @@
-import Request.V1;
-import Response.V1;
-import datetime;
-
-class v1Requestor:
-
-    #region Leagues
-    def GetLeagues(self, sport: str = None, isLive: bool = None) -> Response.V1.GetLeaguesResponse:
-        '''Call Games endpoint of OddsJam API.
-        Required Parameters: None
-        Returns: GetLeaguesResponse 
-        Functions in response: GetLeagueNames()
-        '''
-        resp = self.SendRequest(Request.V1.GetLeaguesRequest(sport, isLive));
-        return Response.V1.GetLeaguesResponse(resp);
-    #endregion Leagues
-
-    #region Games
-    def GetGames(self, page: int = None, sport: str = None, league: str = None, isLive: bool = None, 
-    startDateBefore: str = None, startDateAfter: str = None) -> Response.V1.GetGamesResponse:
-        '''Call Games endpoint of OddsJam API.
-        Required Parameters: None
-        Returns: GetGamesResponse 
-        Functions in response: GetGameIDs()
-        '''
-        resp = self.SendRequest(Request.V1.GetGamesRequest(page, sport, league, isLive, startDateBefore, startDateAfter=startDateAfter)); 
-        return Response.V1.GetGamesResponse(resp);
-    #endregion Games
-
-    #region Markets
-    def GetMarkets(self, page: int = None, gameId: int = None, isLive: bool = None) -> Response.V1.GetMarketsResponse:
-        '''Call Markets endpoint of OddsJam API.
-        Required Parameters: None
-        Returns: GetMarketsResponse 
-        Functions in response: GetMarketNames()
-        '''
-        resp = self.SendRequest(Request.V1.GetMarketsRequest(page, gameId, isLive));
-        return Response.V1.GetMarketsResponse(resp);
-    #endregion Markets
-
-    #region Odds
-    def GetOdds(self, page: int = None, sportsbook: str = None, marketName: str = None, sport: str = None, 
-    league: str = None, gameId: int = None, isLive: bool = None, startDateBefore: datetime = None, startDateAfter: datetime = None) -> Response.V1.GetOddsResponse:
-        '''Call Odds endpoint of OddsJam API.
-        Required Parameters: None
-        Returns: GetOddsResponse
-        Functions in response: GetPrices()
-        '''
-        resp = self.SendRequest(Request.V1.GetOddsRequest(page, sportsbook, marketName, sport, league, gameId, isLive, startDateBefore, startDateAfter));
-        return Response.V1.GetOddsResponse(resp);
-
-    #endregion Odds
-
-    #region Futures
-    def GetFutures(self, page: int = None, sport: str = None, league: str = None) -> Response.V1.GetFuturesResponse:
-        resp = self.SendRequest(Request.V1.GetFuturesRequest(page, sport, league));
-        return Response.V1.GetFuturesResponse(resp);
-    #endregion Futures
-
-    #region Future Odds
-    def GetFutureOdds(self, page: int = None, sportsBook: str = None, 
-    futureName: str = None, sport: str = None, league: str = None, futureId: int = None) -> Response.V1.GetFutureOddsResponse:
-        resp = self.SendRequest(Request.V1.GetFutureOddsRequest(page, sportsBook, futureName, sport, league, futureId));
-        return Response.V1.GetFutureOddsResponse(resp);
-    #endregion Future Odds
-
-    #region Scores
-    def GetScores(self, page: int = None, sport: str = None, league: str = None) -> Response.V1.GetScoresResponse:
-        resp = self.SendRequest(Request.V1.GetScoresRequest(page, sport, league));
-        return Response.V1.GetScoresResponse(resp);
-    #endregion Scores
+import Request.V1;
+import Response.V1;
+import datetime;
+
+class v1Requestor:
+
+    #region Leagues
+    def GetLeagues(self, sport: str = None, isLive: bool = None) -> Response.V1.GetLeaguesResponse:
+        '''Call Games endpoint of OddsJam API.
+        Required Parameters: None
+        Returns: GetLeaguesResponse 
+        Functions in response: GetLeagueNames()
+        '''
+        resp = self.SendRequest(Request.V1.GetLeaguesRequest(sport, isLive));
+        return Response.V1.GetLeaguesResponse(resp);
+    #endregion Leagues
+
+    #region Games
+    def GetGames(self, page: int = None, sport: str = None, league: str = None, isLive: bool = None, 
+    startDateBefore: str = None, startDateAfter: str = None) -> Response.V1.GetGamesResponse:
+        '''Call Games endpoint of OddsJam API.
+        Required Parameters: None
+        Returns: GetGamesResponse 
+        Functions in response: GetGameIDs()
+        '''
+        resp = self.SendRequest(Request.V1.GetGamesRequest(page, sport, league, isLive, startDateBefore, startDateAfter=startDateAfter)); 
+        return Response.V1.GetGamesResponse(resp);
+    #endregion Games
+
+    #region Markets
+    def GetMarkets(self, page: int = None, gameId: int = None, isLive: bool = None) -> Response.V1.GetMarketsResponse:
+        '''Call Markets endpoint of OddsJam API.
+        Required Parameters: None
+        Returns: GetMarketsResponse 
+        Functions in response: GetMarketNames()
+        '''
+        resp = self.SendRequest(Request.V1.GetMarketsRequest(page, gameId, isLive));
+        return Response.V1.GetMarketsResponse(resp);
+    #endregion Markets
+
+    #region Odds
+    def GetOdds(self, page: int = None, sportsbook: str = None, marketName: str = None, sport: str = None, 
+    league: str = None, gameId: int = None, isLive: bool = None, startDateBefore: datetime = None, startDateAfter: datetime = None) -> Response.V1.GetOddsResponse:
+        '''Call Odds endpoint of OddsJam API.
+        Required Parameters: None
+        Returns: GetOddsResponse
+        Functions in response: GetPrices()
+        '''
+        resp = self.SendRequest(Request.V1.GetOddsRequest(page, sportsbook, marketName, sport, league, gameId, isLive, startDateBefore, startDateAfter));
+        return Response.V1.GetOddsResponse(resp);
+
+    #endregion Odds
+
+    #region Futures
+    def GetFutures(self, page: int = None, sport: str = None, league: str = None) -> Response.V1.GetFuturesResponse:
+        resp = self.SendRequest(Request.V1.GetFuturesRequest(page, sport, league));
+        return Response.V1.GetFuturesResponse(resp);
+    #endregion Futures
+
+    #region Future Odds
+    def GetFutureOdds(self, page: int = None, sportsBook: str = None, 
+    futureName: str = None, sport: str = None, league: str = None, futureId: int = None) -> Response.V1.GetFutureOddsResponse:
+        resp = self.SendRequest(Request.V1.GetFutureOddsRequest(page, sportsBook, futureName, sport, league, futureId));
+        return Response.V1.GetFutureOddsResponse(resp);
+    #endregion Future Odds
+
+    #region Scores
+    def GetScores(self, page: int = None, sport: str = None, league: str = None) -> Response.V1.GetScoresResponse:
+        resp = self.SendRequest(Request.V1.GetScoresRequest(page, sport, league));
+        return Response.V1.GetScoresResponse(resp);
+    #endregion Scores
```

### Comparing `oddsjam-api-0.2.7/src/OddsJamClient/V2/Requestor.py` & `oddsjam-api-0.2.8/src/OddsJamClient/V2/Requestor.py`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,75 +1,75 @@
-from argparse import ArgumentError
-import Request.V2;
-import Response.V2;
-import Base;
-import datetime;
-
-class v2Requestor:
-
-    #region Leagues
-    def GetLeagues(self, sport: str = None, isLive: bool = None) -> Response.V2.GetLeaguesResponse:
-        '''Call Games endpoint of OddsJam API.
-        Required Parameters: None
-        Returns: GetLeaguesResponse 
-        Functions in response: GetLeagueNames()
-        '''
-        resp = self.SendRequest(Request.V2.GetLeaguesRequest(sport, isLive));
-        return Response.V2.GetLeaguesResponse(resp);
-    #endregion Leagues
-
-    #region Games
-    def GetGames(self, page: int = None, sport: str = None, league: str = None, isLive: bool = None, 
-    startDateBefore: str = None, startDateAfter: str = None) -> Response.V2.GetGamesResponse:
-        '''Call Games endpoint of OddsJam API.
-        Required Parameters: None
-        Returns: GetGamesResponse 
-        Functions in response: GetGameIDs()
-        '''
-        resp = self.SendRequest(Request.V2.GetGamesRequest(page, sport, league, isLive, startDateBefore, startDateAfter=startDateAfter)); 
-        return Response.V2.GetGamesResponse(resp);
-    #endregion Games
-
-    #region Markets
-    def GetMarkets(self, page: int = None, gameId: int = None, isLive: bool = None) -> Response.V2.GetMarketsResponse:
-        '''Call Markets endpoint of OddsJam API.
-        Required Parameters: None
-        Returns: GetMarketsResponse 
-        Functions in response: GetMarketNames()
-        '''
-        resp = self.SendRequest(Request.V2.GetMarketsRequest(page, gameId, isLive));
-        return Response.V2.GetMarketsResponse(resp);
-    #endregion Markets
-
-    #region Odds
-    def GetOdds(self, sport: str = None, league: str = None, sportsbook: str = None, market_name: str = None, game_id: str = None, is_main: bool = None,
-        is_live: bool = None, start_date_before: str = None, start_date_after: str = None) -> Response.V2.GetOddsResponse:
-        '''Call Odds endpoint of OddsJam API.
-        Required Parameters: None
-        Returns: GetOddsResponse
-        Functions in response: GetPrices()
-        '''
-        if all(v is None for v in [sport, league, sportsbook, market_name, game_id, is_main, is_live, start_date_before, start_date_after]):
-            raise Base.InvalidGetOddsV2Error();
-        resp = self.SendRequest(Request.V2.GetOddsRequest(sport, league, sportsbook, market_name, game_id, is_main, is_live, start_date_before, start_date_after));
-        return Response.V2.GetOddsResponse(resp);
-
-    #endregion Odds
-
-    #region Futures
-    def GetFutures(self, page: int = None, sport: str = None, league: str = None) -> Response.V2.GetFuturesResponse:
-        resp = self.SendRequest(Request.V2.GetFuturesRequest(page, sport, league));
-        return Response.V2.GetFuturesResponse(resp);
-    #endregion Futures
-
-    #region Future Odds
-    def GetFutureOdds(self, page: int = None, sportsBook: str = None, 
-    futureName: str = None, sport: str = None, league: str = None, futureId: int = None) -> Response.V2.GetFutureOddsResponse:
-        resp = self.SendRequest(Request.V2.GetFutureOddsRequest(page, sportsBook, futureName, sport, league, futureId));
-        return Response.V2.GetFutureOddsResponse(resp);
-    #endregion Future Odds
-
-    #region Scores
-    def GetScores(self, page: int = None, sport: str = None, league: str = None) -> Response.V2.GetScoresResponse:
-        resp = self.SendRequest(Request.V2.GetScoresRequest(page, sport, league));
-        return Response.V2.GetScoresResponse(resp);
-    #endregion Scores
+from argparse import ArgumentError
+import Request.V2;
+import Response.V2;
+import Base;
+import datetime;
+
+class v2Requestor:
+
+    #region Leagues
+    def GetLeagues(self, sport: str = None, isLive: bool = None) -> Response.V2.GetLeaguesResponse:
+        '''Call Games endpoint of OddsJam API.
+        Required Parameters: None
+        Returns: GetLeaguesResponse 
+        Functions in response: GetLeagueNames()
+        '''
+        resp = self.SendRequest(Request.V2.GetLeaguesRequest(sport, isLive));
+        return Response.V2.GetLeaguesResponse(resp);
+    #endregion Leagues
+
+    #region Games
+    def GetGames(self, page: int = None, sport: str = None, league: str = None, isLive: bool = None, 
+    startDateBefore: str = None, startDateAfter: str = None) -> Response.V2.GetGamesResponse:
+        '''Call Games endpoint of OddsJam API.
+        Required Parameters: None
+        Returns: GetGamesResponse 
+        Functions in response: GetGameIDs()
+        '''
+        resp = self.SendRequest(Request.V2.GetGamesRequest(page, sport, league, isLive, startDateBefore, startDateAfter=startDateAfter)); 
+        return Response.V2.GetGamesResponse(resp);
+    #endregion Games
+
+    #region Markets
+    def GetMarkets(self, page: int = None, gameId: int = None, isLive: bool = None) -> Response.V2.GetMarketsResponse:
+        '''Call Markets endpoint of OddsJam API.
+        Required Parameters: None
+        Returns: GetMarketsResponse 
+        Functions in response: GetMarketNames()
+        '''
+        resp = self.SendRequest(Request.V2.GetMarketsRequest(page, gameId, isLive));
+        return Response.V2.GetMarketsResponse(resp);
+    #endregion Markets
+
+    #region Odds
+    def GetOdds(self, sport: str = None, league: str = None, sportsbook: str = None, market_name: str = None, game_id: str = None, is_main: bool = None,
+        is_live: bool = None, start_date_before: str = None, start_date_after: str = None) -> Response.V2.GetOddsResponse:
+        '''Call Odds endpoint of OddsJam API.
+        Required Parameters: None
+        Returns: GetOddsResponse
+        Functions in response: GetPrices()
+        '''
+        if all(v is None for v in [sport, league, sportsbook, market_name, game_id, is_main, is_live, start_date_before, start_date_after]):
+            raise Base.InvalidGetOddsV2Error();
+        resp = self.SendRequest(Request.V2.GetOddsRequest(sport, league, sportsbook, market_name, game_id, is_main, is_live, start_date_before, start_date_after));
+        return Response.V2.GetOddsResponse(resp);
+
+    #endregion Odds
+
+    #region Futures
+    def GetFutures(self, page: int = None, sport: str = None, league: str = None) -> Response.V2.GetFuturesResponse:
+        resp = self.SendRequest(Request.V2.GetFuturesRequest(page, sport, league));
+        return Response.V2.GetFuturesResponse(resp);
+    #endregion Futures
+
+    #region Future Odds
+    def GetFutureOdds(self, page: int = None, sportsBook: str = None, 
+    futureName: str = None, sport: str = None, league: str = None, futureId: int = None) -> Response.V2.GetFutureOddsResponse:
+        resp = self.SendRequest(Request.V2.GetFutureOddsRequest(page, sportsBook, futureName, sport, league, futureId));
+        return Response.V2.GetFutureOddsResponse(resp);
+    #endregion Future Odds
+
+    #region Scores
+    def GetScores(self, page: int = None, sport: str = None, league: str = None) -> Response.V2.GetScoresResponse:
+        resp = self.SendRequest(Request.V2.GetScoresRequest(page, sport, league));
+        return Response.V2.GetScoresResponse(resp);
+    #endregion Scores
```

### Comparing `oddsjam-api-0.2.7/src/Response/V1/GetFutureOddsResponse.py` & `oddsjam-api-0.2.8/src/Response/V1/GetFutureOddsResponse.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-#region Imports
-import json;
-from Models.V1 import FutureOdds, Future;
-from Base import ResponseBase;
-#endregion Imports
-
-class GetFutureOddsResponse(ResponseBase):
-    def __init__(self, response: str):
-        super().__init__(response);
-        self.FutureOdds = self.ParseResponse(response);
-        
-    def ParseResponse(self, response:str):
-        try:
-            obj = json.loads(response);
-            futureOdds = [FutureOdds.fromDict(m) for m in obj]; 
-            for f in futureOdds:
-                f.future = Future.fromDict(f.future);
-                f.sports_book = f.sports_book['name'];
-            return futureOdds;
-        except Exception as ex:
+#region Imports
+import json;
+from Models.V1 import FutureOdds, Future;
+from Base import ResponseBase;
+#endregion Imports
+
+class GetFutureOddsResponse(ResponseBase):
+    def __init__(self, response: str):
+        super().__init__(response);
+        self.FutureOdds = self.ParseResponse(response);
+        
+    def ParseResponse(self, response:str):
+        try:
+            obj = json.loads(response);
+            futureOdds = [FutureOdds.fromDict(m) for m in obj]; 
+            for f in futureOdds:
+                f.future = Future.fromDict(f.future);
+                f.sports_book = f.sports_book['name'];
+            return futureOdds;
+        except Exception as ex:
             return ex;
```

### Comparing `oddsjam-api-0.2.7/src/Response/V1/GetFuturesResponse.py` & `oddsjam-api-0.2.8/src/Response/V1/GetLeaguesResponse.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,17 +1,17 @@
-#region Imports
-import json;
-from Models.V1 import Future;
-from Base import ResponseBase;
-#endregion Imports
-
-class GetFuturesResponse(ResponseBase):
-    def __init__(self, response: str):
-        super().__init__(response);
-        obj = self.ParseResponse(response);
-        self.Futures = [f for f in obj]
-        
-    def ParseResponse(self, response:str):
-        try:
-            return json.loads(response, object_hook=lambda d: Future(**d));
-        except Exception as ex:
+#region Imports
+import json;
+from Base import ResponseBase;
+from Models.V1 import League;
+#endregion Imports
+
+class GetLeaguesResponse(ResponseBase):
+    def __init__(self, response: str):
+        super().__init__(response);
+        self.Leagues = self.ParseResponse(self.RawResponse);
+    
+    def ParseResponse(self, response: str):
+        try:
+            responseObj = json.loads(response);
+            return [League(l) for l in responseObj['leagues']];
+        except Exception as ex:
             return ex;
```

### Comparing `oddsjam-api-0.2.7/src/Response/V1/GetMarketsResponse.py` & `oddsjam-api-0.2.8/src/Response/V1/GetMarketsResponse.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-#region Imports
-import json;
-from Base import ResponseBase;
-from Models.V1 import Market, Game;
-#endregion Imports
-
-class GetMarketsResponse(ResponseBase):
-    def __init__(self, response: str):
-        super().__init__(response);
-        self.Markets = self.ParseResponse(response);
-
-    def ParseResponse(self, response: str):
-        try:
-            obj = json.loads(response);
-            marketObjects = [Market.fromDict(m) for m in obj];
-            for m in marketObjects:
-                m.game = Game.fromDict(m.game);
-            return marketObjects;
-        except Exception as ex:
+#region Imports
+import json;
+from Base import ResponseBase;
+from Models.V1 import Market, Game;
+#endregion Imports
+
+class GetMarketsResponse(ResponseBase):
+    def __init__(self, response: str):
+        super().__init__(response);
+        self.Markets = self.ParseResponse(response);
+
+    def ParseResponse(self, response: str):
+        try:
+            obj = json.loads(response);
+            marketObjects = [Market.fromDict(m) for m in obj];
+            for m in marketObjects:
+                m.game = Game.fromDict(m.game);
+            return marketObjects;
+        except Exception as ex:
             return ex;
```

### Comparing `oddsjam-api-0.2.7/src/Response/V1/GetOddsResponse.py` & `oddsjam-api-0.2.8/src/Response/V1/GetScoresResponse.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,34 +1,25 @@
-#region Imports
-import json;
-from Models.V1 import Odds, Game;
-from Base import ResponseBase;
-#endregion Imports
-
-class GetOddsResponse(ResponseBase):
-    def __init__(self, response: str):
-        super().__init__(response);
-        self.Odds = self.ParseResponse(response);
-        self.Type = 'American';
-        
-    def ParseResponse(self, response:str):
-        try:
-            obj = json.loads(response);
-            oddsObjects = [Odds.fromDict(m) for m in obj];
-            for o in oddsObjects:
-                o.game = Game.fromDict(o.game);
-                o.sports_book = o.sports_book['name']
-            return oddsObjects;
-        except Exception as ex:
-            return ex;
-
-    def AsDecimal(self):
-        try:
-            [o.AsDecimal() for o in self.Odds]
-        except Exception as ex:
-            return ex;
-    
-    def AsAmerican(self):
-        try:
-            [o.AsAmerican() for o in self.Odds]
-        except Exception as ex:
+#region Imports
+import json;
+from Models.V1 import Score, Game, PeriodScore;
+from Base import ResponseBase;
+#endregion Imports
+
+class GetScoresResponse(ResponseBase):
+    def __init__(self, response: str):
+        super().__init__(response);
+        self.Scores = self.ParseResponse(response);
+        self.Type = 'American';
+        
+    def ParseResponse(self, response:str):
+        try:
+            obj = json.loads(response);
+            scoresObject = [Score.fromDict(m) for m in obj];
+            for o in scoresObject:
+                o.game = Game.fromDict(o.game);
+                parsedPeriodScores = [];
+                for p in o.period_scores:
+                    parsedPeriodScores.append(PeriodScore.fromDict(p));
+                o.period_scores = parsedPeriodScores;
+            return scoresObject;
+        except Exception as ex:
             return ex;
```

### Comparing `oddsjam-api-0.2.7/src/Response/V1/GetScoresResponse.py` & `oddsjam-api-0.2.8/src/Response/V2/GetScoresResponse.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,25 +1,25 @@
-#region Imports
-import json;
-from Models.V1 import Score, Game, PeriodScore;
-from Base import ResponseBase;
-#endregion Imports
-
-class GetScoresResponse(ResponseBase):
-    def __init__(self, response: str):
-        super().__init__(response);
-        self.Scores = self.ParseResponse(response);
-        self.Type = 'American';
-        
-    def ParseResponse(self, response:str):
-        try:
-            obj = json.loads(response);
-            scoresObject = [Score.fromDict(m) for m in obj];
-            for o in scoresObject:
-                o.game = Game.fromDict(o.game);
-                parsedPeriodScores = [];
-                for p in o.period_scores:
-                    parsedPeriodScores.append(PeriodScore.fromDict(p));
-                o.period_scores = parsedPeriodScores;
-            return scoresObject;
-        except Exception as ex:
+#region Imports
+import json;
+from Models.V2 import Score, Game, PeriodScore;
+from Base import ResponseBase;
+#endregion Imports
+
+class GetScoresResponse(ResponseBase):
+    def __init__(self, response: str):
+        super().__init__(response);
+        self.Scores = self.ParseResponse(response);
+        self.Type = 'American';
+        
+    def ParseResponse(self, response:str):
+        try:
+            obj = json.loads(response);
+            scoresObject = [Score.fromDict(m) for m in obj];
+            for o in scoresObject:
+                o.game = Game.fromDict(o.game);
+                parsedPeriodScores = [];
+                for p in o.period_scores:
+                    parsedPeriodScores.append(PeriodScore.fromDict(p));
+                o.period_scores = parsedPeriodScores;
+            return scoresObject;
+        except Exception as ex:
             return ex;
```

### Comparing `oddsjam-api-0.2.7/src/Response/V2/GetFutureOddsResponse.py` & `oddsjam-api-0.2.8/src/Response/V2/GetMarketsResponse.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,21 +1,20 @@
-#region Imports
-import json;
-from Models.V2 import FutureOdds, FutureOdd;
-from Base import ResponseBase;
-#endregion Imports
-
-class GetFutureOddsResponse(ResponseBase):
-    def __init__(self, response: str):
-        super().__init__(response);
-        resp = json.loads(response);
-        self.FutureOdds = self.ParseResponse(json.dumps(resp['data']));
-        
-    def ParseResponse(self, response:str):
-        try:
-            obj = json.loads(response);
-            futureOdds = [FutureOdds.fromDict(m) for m in obj]; 
-            for f in futureOdds:
-                f.odds = [FutureOdd.fromDict(m) for m in f.odds]
-            return futureOdds;
-        except Exception as ex:
+#region Imports
+import json;
+from Base import ResponseBase;
+from Models.V2 import Market, Game;
+#endregion Imports
+
+class GetMarketsResponse(ResponseBase):
+    def __init__(self, response: str):
+        super().__init__(response);
+        self.Markets = self.ParseResponse(response);
+
+    def ParseResponse(self, response: str):
+        try:
+            obj = json.loads(response);
+            marketObjects = [Market.fromDict(m) for m in obj];
+            for m in marketObjects:
+                m.game = Game.fromDict(m.game);
+            return marketObjects;
+        except Exception as ex:
             return ex;
```

### Comparing `oddsjam-api-0.2.7/src/Response/V2/GetFuturesResponse.py` & `oddsjam-api-0.2.8/src/Response/V2/GetFuturesResponse.py`

 * *Ordering differences only*

 * *Files 27% similar despite different names*

```diff
@@ -1,18 +1,18 @@
-#region Imports
-import json;
-from Models.V2 import Future;
-from Base import ResponseBase;
-#endregion Imports
-
-class GetFuturesResponse(ResponseBase):
-    def __init__(self, response: str):
-        super().__init__(response);
-        resp = json.loads(response);
-        obj = self.ParseResponse(json.dumps(resp['data']));
-        self.Futures = [f for f in obj]
-        
-    def ParseResponse(self, response:str):
-        try:
-            return json.loads(response, object_hook=lambda d: Future(**d));
-        except Exception as ex:
+#region Imports
+import json;
+from Models.V2 import Future;
+from Base import ResponseBase;
+#endregion Imports
+
+class GetFuturesResponse(ResponseBase):
+    def __init__(self, response: str):
+        super().__init__(response);
+        resp = json.loads(response);
+        obj = self.ParseResponse(json.dumps(resp['data']));
+        self.Futures = [f for f in obj]
+        
+    def ParseResponse(self, response:str):
+        try:
+            return json.loads(response, object_hook=lambda d: Future(**d));
+        except Exception as ex:
             return ex;
```

### Comparing `oddsjam-api-0.2.7/src/oddsjam_api.egg-info/PKG-INFO` & `oddsjam-api-0.2.8/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,146 +1,150 @@
-Metadata-Version: 2.1
-Name: oddsjam-api
-Version: 0.2.7
-Summary: A lightweight wrapper for the OddsJam API
-Home-page: https://github.com/cooperbrandon1/oddsjam-api/
-Author: Brandon Cooper
-Author-email: cooper.brandon@outlook.com
-License: UNKNOWN
-Project-URL: Bug Tracker, https://github.com/cooperbrandon1/oddsjam-api/issues
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# <code>oddsjam-api</code>: A lightweight OddsJam API wrapper
-
-## V2 Update
-V2 support is now available for the new endpoints/models listed at the [OddsJam Developer Page](https://developer.oddsjam.com/).  The client exposed by this package is backwards compatible, and runs in v1 by default. Versions can be switched as follows:
-``` python
-    from OddsJamClient import OddsJamClient;
-    Client = OddsJamClient(YOUR_API_KEY);
-    v1Results = Client.GetLeagues(); #Default v1 endpoints
-
-    Client.UseV2();
-    v2Results = Client.GetLeagues(); #v2 endpoints
-```
-
-This update comes with the following changes:
-<ul>
-<li>Type hinting for function calls is no longer available. Function calls will appear with <code>(*args: Any, **kwargs:Any) -> Any</code>. Please refer to the developer documentation for valid arguments.</li>
-<li>The V2 client does <strong>not</strong> contain a GetMarkets() function.</li>
-<li>The V2 client requires <i>at least one</i> argument for the GetOdds() function. This is due to the amount of data returned from the new V2 endpoint. Attempting a call to GetOdds() <i>without</i> a parameter will result in an <code>InvalidGetOddsV2Error</code>, and the endpoint will <i>not</i> be hit.</li>
-</ul>
-<br/>
-
-## What is <code>oddsjam-api</code>?
-<code>oddsjam-api</code> is a fast, lightweight wrapper for the [OddsJam API](https://developer.oddsjam.com/). It strives to be as intuitive to use as possible, providing strongly typed requests and responses to ensure predictability and consistency.
-
-
-
-## How do I use it?
-Start by installing the <code>oddsjam-api</code> package (currently only on TestPyPI):
-``` 
-    pip install oddsjam-api
-```
-
-Create an instance of the <code>OddsJamClient</code>:
-
-``` python
-    from OddsJamClient import OddsJamClient;
-    Client = OddsJamClient(YOUR_API_KEY);
-```
-
-Then simply call whichever function you'd like to:
-
-``` python 
-    from OddsJamClient import OddsJamClient;
-    Client = OddsJamClient(YOUR_API_KEY);
-    GamesResponse = Client.GetGames();
-```
-
-Parameters are not required for any function call, but can be provided as desired:
-
-``` python
-    from OddsJamClient import OddsJamClient;
-    Client = OddsJamClient(YOUR_API_KEY);
-    GamesResponse = Client.GetGames(league='ncaa', sport='football');
-```
-
-Parameters will raise specific errors:
-
-``` python
-    GamesResponse = Client.GetGames(sport='curling'); 
-    #Raises SportError, with a list of valid values
-
-    OddsResponse = Client.GetOdds(sportsbook='212 Bet');
-    #Raises SportsBookError, with a list of valid values
-```
-
-Note: Sport and SportsBook parameters are *case insensitive*
-
-Accessing the object of a response requires accessing the response's object:
-
-``` python    
-    from OddsJamClient import OddsJamClient;
-    Client = OddsJamClient(YOUR_API_KEY);
-    GamesResponse = Client.GetGames();
-    Games = GamesResponse.Games;
-```
-
-List comprehension can also be used to access objects:
-
-``` python
-    AwayTeams = [g.away_team for g in GamesResponse.Games];
-```
-
-Nested objects can be accessed similarly:
-
-``` python
-    OddsResponse = Client.GetOdds();
-    print(OddsResponse.Odds[0].game.sport)
-```
-
-The raw response from the API is also accessible via the *RawResponse* property of any *Response* object:
-
-``` python
-    Raw = GamesResponse.RawResponse;
-    Jobj = json.loads(raw);
-```
-
-## Built-in functions
-Convert entire Odds collection to decimal, then back to American:
-``` python
-    OddsResponse = Client.GetOdds();
-    OddsResponse.AsDecimal();
-    OddsResponse.AsAmerican();
-```
-
-Convert individual Odds object to decimal, then back to American:
-``` python
-    OddsResponse = Client.GetOdds();
-    FirstOdd = OddsResponse.Odds[0];
-    FirstOdd.AsDecimal();
-    FirstOdd.AsAmerican();
-```
-
-## Example usage
-Flatten and output data using pandas:
-``` python
-    import pandas as pd;
-    from OddsJamClient import OddsJamClient;
-
-    Client = OddsJamClient(YOUR_API_KEY);
-    Odds = Client.GetOdds().Odds;
-    df = pd.DataFrame(Odds);
-
-    #Lambda over rows to extract just the ID from the 'game' object in each row
-    df['game'] = df.apply(lambda row: row['game']['id'], axis=1)
-    
-    #Get odds for Moneyline markets only
-    df = df.loc[df['market_name'] == 'Moneyline']
-```
-
+Metadata-Version: 2.1
+Name: oddsjam-api
+Version: 0.2.8
+Summary: A lightweight OddsJam API wrapper
+Author-email: Rohan Challa <rchalla769@gmail.com>, Brandon Cooper <cooper.brandon@outlook.com>
+Project-URL: Homepage, https://github.com/oddsjam/api-python
+Project-URL: Bug Tracker, https://github.com/oddsjam/api-python/issues
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# <code>oddsjam-api</code>: A lightweight OddsJam API wrapper
+
+## V2 Update
+V2 support is now available for the new endpoints/models listed at the [OddsJam Developer Page](https://developer.oddsjam.com/).  The client exposed by this package is backwards compatible, and runs in v1 by default. Versions can be switched as follows:
+``` python
+    from OddsJamClient import OddsJamClient;
+    Client = OddsJamClient(YOUR_API_KEY);
+    v1Results = Client.GetLeagues(); #Default v1 endpoints
+
+    Client.UseV2();
+    v2Results = Client.GetLeagues(); #v2 endpoints
+```
+
+This update comes with the following changes:
+<ul>
+<li>Type hinting for function calls is no longer available. Function calls will appear with <code>(*args: Any, **kwargs:Any) -> Any</code>. Please refer to the developer documentation for valid arguments.</li>
+<li>The V2 client does <strong>not</strong> contain a GetMarkets() function.</li>
+<li>The V2 client requires <i>at least one</i> argument for the GetOdds() function. This is due to the amount of data returned from the new V2 endpoint. Attempting a call to GetOdds() <i>without</i> a parameter will result in an <code>InvalidGetOddsV2Error</code>, and the endpoint will <i>not</i> be hit.</li>
+</ul>
+<br/>
+
+## What is <code>oddsjam-api</code>?
+<code>oddsjam-api</code> is a fast, lightweight wrapper for the [OddsJam API](https://developer.oddsjam.com/). It strives to be as intuitive to use as possible, providing strongly typed requests and responses to ensure predictability and consistency.
+
+
+
+## How do I use it?
+Start by installing the <code>oddsjam-api</code> package (currently only on TestPyPI):
+``` 
+    pip install oddsjam-api
+```
+
+Create an instance of the <code>OddsJamClient</code>:
+
+``` python
+    from OddsJamClient import OddsJamClient;
+    Client = OddsJamClient(YOUR_API_KEY);
+```
+
+Then simply call whichever function you'd like to:
+
+``` python 
+    from OddsJamClient import OddsJamClient;
+    Client = OddsJamClient(YOUR_API_KEY);
+    GamesResponse = Client.GetGames();
+```
+
+Parameters are not required for any function call, but can be provided as desired:
+
+``` python
+    from OddsJamClient import OddsJamClient;
+    Client = OddsJamClient(YOUR_API_KEY);
+    GamesResponse = Client.GetGames(league='ncaa', sport='football');
+```
+
+Parameters will raise specific errors:
+
+``` python
+    GamesResponse = Client.GetGames(sport='curling'); 
+    #Raises SportError, with a list of valid values
+
+    OddsResponse = Client.GetOdds(sportsbook='212 Bet');
+    #Raises SportsBookError, with a list of valid values
+```
+
+Note: Sport and SportsBook parameters are *case insensitive*
+
+Accessing the object of a response requires accessing the response's object:
+
+``` python    
+    from OddsJamClient import OddsJamClient;
+    Client = OddsJamClient(YOUR_API_KEY);
+    GamesResponse = Client.GetGames();
+    Games = GamesResponse.Games;
+```
+
+List comprehension can also be used to access objects:
+
+``` python
+    AwayTeams = [g.away_team for g in GamesResponse.Games];
+```
+
+Nested objects can be accessed similarly:
+
+``` python
+    OddsResponse = Client.GetOdds();
+    print(OddsResponse.Odds[0].game.sport)
+```
+
+The raw response from the API is also accessible via the *RawResponse* property of any *Response* object:
+
+``` python
+    Raw = GamesResponse.RawResponse;
+    Jobj = json.loads(raw);
+```
+
+## Built-in functions
+Convert entire Odds collection to decimal, then back to American:
+``` python
+    OddsResponse = Client.GetOdds();
+    OddsResponse.AsDecimal();
+    OddsResponse.AsAmerican();
+```
+
+Convert individual Odds object to decimal, then back to American:
+``` python
+    OddsResponse = Client.GetOdds();
+    FirstOdd = OddsResponse.Odds[0];
+    FirstOdd.AsDecimal();
+    FirstOdd.AsAmerican();
+```
+
+## Example usage
+Flatten and output data using pandas:
+``` python
+    import pandas as pd;
+    from OddsJamClient import OddsJamClient;
+
+    Client = OddsJamClient(YOUR_API_KEY);
+    Odds = Client.GetOdds().Odds;
+    df = pd.DataFrame(Odds);
+
+    #Lambda over rows to extract just the ID from the 'game' object in each row
+    df['game'] = df.apply(lambda row: row['game']['id'], axis=1)
+    
+    #Get odds for Moneyline markets only
+    df = df.loc[df['market_name'] == 'Moneyline']
+```
+
+# PyPi
+
+* Prod: https://pypi.org/project/oddsjam-api
+* Test: https://test.pypi.org/project/oddsjam-api-test
+
+
+ORIGINAL CREDIT GOES TO https://github.com/cooperbrandon1
```

### Comparing `oddsjam-api-0.2.7/src/oddsjam_api.egg-info/SOURCES.txt` & `oddsjam-api-0.2.8/src/oddsjam_api.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 LICENSE
 README.md
 pyproject.toml
-setup.cfg
+src/__init__.py
 src/Base/CustomExceptions.py
 src/Base/EnforceTypes.py
 src/Base/ModelBase.py
 src/Base/RequestBase.py
 src/Base/ResponseBase.py
 src/Base/ValidParameters.py
 src/Base/__init__.py
```

