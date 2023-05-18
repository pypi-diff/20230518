# Comparing `tmp/fenjing-0.3.1.tar.gz` & `tmp/fenjing-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fenjing-0.3.1.tar", last modified: Wed May 17 11:29:38 2023, max compression
+gzip compressed data, was "fenjing-0.3.2.tar", last modified: Thu May 18 06:14:58 2023, max compression
```

## Comparing `fenjing-0.3.1.tar` & `fenjing-0.3.2.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 11:29:38.229593 fenjing-0.3.1/
--rw-r--r--   0 runner    (1001) docker     (123)    16725 2023-05-17 11:29:26.000000 fenjing-0.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-05-17 11:29:26.000000 fenjing-0.3.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6165 2023-05-17 11:29:38.229593 fenjing-0.3.1/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (123)     5727 2023-05-17 11:29:26.000000 fenjing-0.3.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-17 11:29:26.000000 fenjing-0.3.1/VERSION
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 11:29:38.229593 fenjing-0.3.1/fenjing/
--rwxr-xr-x   0 runner    (1001) docker     (123)      202 2023-05-17 11:29:26.000000 fenjing-0.3.1/fenjing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-17 11:29:26.000000 fenjing-0.3.1/fenjing/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6389 2023-05-17 11:29:26.000000 fenjing-0.3.1/fenjing/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      800 2023-05-17 11:29:26.000000 fenjing-0.3.1/fenjing/colorize.py
--rw-r--r--   0 runner    (1001) docker     (123)      838 2023-05-17 11:29:26.000000 fenjing-0.3.1/fenjing/config_payload.py
--rw-r--r--   0 runner    (1001) docker     (123)     1486 2023-05-17 11:29:26.000000 fenjing-0.3.1/fenjing/const.py
--rwxr-xr-x   0 runner    (1001) docker     (123)       37 2023-05-17 11:29:26.000000 fenjing-0.3.1/fenjing/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2670 2023-05-17 11:29:26.000000 fenjing-0.3.1/fenjing/form.py
--rw-r--r--   0 runner    (1001) docker     (123)     5450 2023-05-17 11:29:26.000000 fenjing-0.3.1/fenjing/form_cracker.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3992 2023-05-17 11:29:26.000000 fenjing-0.3.1/fenjing/full_payload_gen.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2846 2023-05-17 11:29:26.000000 fenjing-0.3.1/fenjing/int_vars.py
--rw-r--r--   0 runner    (1001) docker     (123)    27358 2023-05-17 11:29:26.000000 fenjing-0.3.1/fenjing/payload_gen.py
--rw-r--r--   0 runner    (1001) docker     (123)     1549 2023-05-17 11:29:26.000000 fenjing-0.3.1/fenjing/requester.py
--rw-r--r--   0 runner    (1001) docker     (123)     1180 2023-05-17 11:29:26.000000 fenjing-0.3.1/fenjing/scan_url.py
--rw-r--r--   0 runner    (1001) docker     (123)      941 2023-05-17 11:29:26.000000 fenjing-0.3.1/fenjing/shell_payload.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 11:29:38.229593 fenjing-0.3.1/fenjing/static/
--rw-r--r--   0 runner    (1001) docker     (123)      639 2023-05-17 11:29:26.000000 fenjing-0.3.1/fenjing/static/style.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 11:29:38.229593 fenjing-0.3.1/fenjing/templates/
--rw-r--r--   0 runner    (1001) docker     (123)     6139 2023-05-17 11:29:26.000000 fenjing-0.3.1/fenjing/templates/index.html
--rw-r--r--   0 runner    (1001) docker     (123)     3192 2023-05-17 11:29:26.000000 fenjing-0.3.1/fenjing/waf_func_gen.py
--rw-r--r--   0 runner    (1001) docker     (123)     8403 2023-05-17 11:29:26.000000 fenjing-0.3.1/fenjing/webui.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 11:29:38.229593 fenjing-0.3.1/fenjing.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6165 2023-05-17 11:29:38.000000 fenjing-0.3.1/fenjing.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      629 2023-05-17 11:29:38.000000 fenjing-0.3.1/fenjing.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 11:29:38.000000 fenjing-0.3.1/fenjing.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-17 11:29:38.000000 fenjing-0.3.1/fenjing.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-17 11:29:38.000000 fenjing-0.3.1/fenjing.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-17 11:29:26.000000 fenjing-0.3.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-17 11:29:38.229593 fenjing-0.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      945 2023-05-17 11:29:26.000000 fenjing-0.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 06:14:58.441087 fenjing-0.3.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    16725 2023-05-18 06:14:39.000000 fenjing-0.3.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-05-18 06:14:39.000000 fenjing-0.3.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6255 2023-05-18 06:14:58.441087 fenjing-0.3.2/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5817 2023-05-18 06:14:39.000000 fenjing-0.3.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-18 06:14:39.000000 fenjing-0.3.2/VERSION
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 06:14:58.437087 fenjing-0.3.2/fenjing/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      202 2023-05-18 06:14:39.000000 fenjing-0.3.2/fenjing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-18 06:14:39.000000 fenjing-0.3.2/fenjing/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6389 2023-05-18 06:14:39.000000 fenjing-0.3.2/fenjing/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      800 2023-05-18 06:14:39.000000 fenjing-0.3.2/fenjing/colorize.py
+-rw-r--r--   0 runner    (1001) docker     (123)      838 2023-05-18 06:14:39.000000 fenjing-0.3.2/fenjing/config_payload.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1486 2023-05-18 06:14:39.000000 fenjing-0.3.2/fenjing/const.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)       37 2023-05-18 06:14:39.000000 fenjing-0.3.2/fenjing/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2670 2023-05-18 06:14:39.000000 fenjing-0.3.2/fenjing/form.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5450 2023-05-18 06:14:39.000000 fenjing-0.3.2/fenjing/form_cracker.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3992 2023-05-18 06:14:39.000000 fenjing-0.3.2/fenjing/full_payload_gen.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2846 2023-05-18 06:14:39.000000 fenjing-0.3.2/fenjing/int_vars.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27358 2023-05-18 06:14:39.000000 fenjing-0.3.2/fenjing/payload_gen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1549 2023-05-18 06:14:39.000000 fenjing-0.3.2/fenjing/requester.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1180 2023-05-18 06:14:39.000000 fenjing-0.3.2/fenjing/scan_url.py
+-rw-r--r--   0 runner    (1001) docker     (123)      941 2023-05-18 06:14:39.000000 fenjing-0.3.2/fenjing/shell_payload.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 06:14:58.441087 fenjing-0.3.2/fenjing/static/
+-rw-r--r--   0 runner    (1001) docker     (123)      639 2023-05-18 06:14:39.000000 fenjing-0.3.2/fenjing/static/style.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 06:14:58.441087 fenjing-0.3.2/fenjing/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     6139 2023-05-18 06:14:39.000000 fenjing-0.3.2/fenjing/templates/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3192 2023-05-18 06:14:39.000000 fenjing-0.3.2/fenjing/waf_func_gen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8580 2023-05-18 06:14:39.000000 fenjing-0.3.2/fenjing/webui.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 06:14:58.441087 fenjing-0.3.2/fenjing.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6255 2023-05-18 06:14:58.000000 fenjing-0.3.2/fenjing.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      629 2023-05-18 06:14:58.000000 fenjing-0.3.2/fenjing.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 06:14:58.000000 fenjing-0.3.2/fenjing.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-18 06:14:58.000000 fenjing-0.3.2/fenjing.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-18 06:14:58.000000 fenjing-0.3.2/fenjing.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-18 06:14:39.000000 fenjing-0.3.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-18 06:14:58.441087 fenjing-0.3.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      945 2023-05-18 06:14:39.000000 fenjing-0.3.2/setup.py
```

### Comparing `fenjing-0.3.1/LICENSE` & `fenjing-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `fenjing-0.3.1/PKG-INFO` & `fenjing-0.3.2/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,20 +1,7 @@
-Metadata-Version: 2.1
-Name: fenjing
-Version: 0.3.1
-Summary: A Jinja2 SSTI cracker for CTF competitions
-Home-page: https://github.com/Marven11/Fenjing
-Author: Marven11
-Author-email: marven11@example.com
-Classifier: Programming Language :: Python :: 3.9
-Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
-Classifier: Operating System :: OS Independent
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 ![焚靖](assets/fenjing.webp)
 
 > Bypass the WAF without knowing WAF
 
 焚靖是一个针对Jinja2 SSTI的命令行脚本，具有强大的自动绕过WAF功能
 
 ## 演示
@@ -195,10 +182,10 @@
     print(f"{shell_payload=}")
     print(f"{config_payload=}")
 
 ```
 
 ## 项目结构
 
-[![](https://mermaid.ink/img/pako:eNqFVMtugzAQ_BXLUm7hBzj0UPUP2iMS2thrsGps6keiNMq_F5pS2xhan2BmdryeNdwoMxxpTYUyF9aD9eTtudFkWi6cOgtjT4KXypEHOC9mlLHyEyNi8SOg82gjJIwd0hLt_OMVNV_5w8kEX41wVQa4i0VS-_YMNkFcj0q1P8rMXciuxEWI6rZDHZkC3OsqP4ZjoNtgVUQuIFoRNMvt56qWWWDvSyS__ocDYUqSqnpKIkqRvG5h8p0Tk1X0CZOPaSJS91UDW2zpXEjyLVb0vMHmAAqbMsR14besNNpS5bcmvxpkv6n5eFt2RYr_CpZR7YSY0XEC2dX-u880ru0WCkU26YJNmqRHOqAdQPLpn3CbSxrqexywofX0yFFAUL6hjb5PUgjevF41o7W3AY80jBw8vkiYPqGB1gKUw_sXrbFnVA?type=png)](https://mermaid.live/edit#pako:eNqFVMtugzAQ_BXLUm7hBzj0UPUP2iMS2thrsGps6keiNMq_F5pS2xhan2BmdryeNdwoMxxpTYUyF9aD9eTtudFkWi6cOgtjT4KXypEHOC9mlLHyEyNi8SOg82gjJIwd0hLt_OMVNV_5w8kEX41wVQa4i0VS-_YMNkFcj0q1P8rMXciuxEWI6rZDHZkC3OsqP4ZjoNtgVUQuIFoRNMvt56qWWWDvSyS__ocDYUqSqnpKIkqRvG5h8p0Tk1X0CZOPaSJS91UDW2zpXEjyLVb0vMHmAAqbMsR14besNNpS5bcmvxpkv6n5eFt2RYr_CpZR7YSY0XEC2dX-u880ru0WCkU26YJNmqRHOqAdQPLpn3CbSxrqexywofX0yFFAUL6hjb5PUgjevF41o7W3AY80jBw8vkiYPqGB1gKUw_sXrbFnVA)
+[![](https://mermaid.ink/img/pako:eNp1U01TwyAQ_SsMM-2p-QM5eHA86kU9aTqZLVkaRgKRD2vt9L8LwZQkrRwYeLzdfbyFE2W6QVpSLvWBtWAceb2vFAnD-t3eQN8S74S0JIFxMC21ET-YEYOfHq1DkyGuTTcNUdblbVqhapaVLJpCqJCIA8NpSSneOdiSQxEOO6FARmybGQfc-cjZRQ4XBrn-TuB2loYUxV3CLyLIQkWUbnPQakWakI85oRV5fpyUBF5zr1i9RzW_eM0MsI-pHZaBqr2Rt3lJ1FW6waCFuB6OUkMz0ZfFjZ2LI7hYf4GZ8GyLUtZ_8bPWcLG_xrnP7PkNb4LzNGQ9LzdccJlxAKf79UL15YGMfbv2djyZ-5vmocv_xC3cvyUvWk83tAvvDUQTvsgphlbUtdhhRcuwVOidAVnRSp0DFbzTL0fFaOmMxw31fQMOHwSE1nU0PExpA9qDetM677ERTpun9A2H33j-BR2iIbY?type=png)](https://mermaid.live/edit#pako:eNp1U01TwyAQ_SsMM-2p-QM5eHA86kU9aTqZLVkaRgKRD2vt9L8LwZQkrRwYeLzdfbyFE2W6QVpSLvWBtWAceb2vFAnD-t3eQN8S74S0JIFxMC21ET-YEYOfHq1DkyGuTTcNUdblbVqhapaVLJpCqJCIA8NpSSneOdiSQxEOO6FARmybGQfc-cjZRQ4XBrn-TuB2loYUxV3CLyLIQkWUbnPQakWakI85oRV5fpyUBF5zr1i9RzW_eM0MsI-pHZaBqr2Rt3lJ1FW6waCFuB6OUkMz0ZfFjZ2LI7hYf4GZ8GyLUtZ_8bPWcLG_xrnP7PkNb4LzNGQ9LzdccJlxAKf79UL15YGMfbv2djyZ-5vmocv_xC3cvyUvWk83tAvvDUQTvsgphlbUtdhhRcuwVOidAVnRSp0DFbzTL0fFaOmMxw31fQMOHwSE1nU0PExpA9qDetM677ERTpun9A2H33j-BR2iIbY)
```

### Comparing `fenjing-0.3.1/README.md` & `fenjing-0.3.2/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,20 @@
+Metadata-Version: 2.1
+Name: fenjing
+Version: 0.3.2
+Summary: A Jinja2 SSTI cracker for CTF competitions
+Home-page: https://github.com/Marven11/Fenjing
+Author: Marven11
+Author-email: marven11@example.com
+Classifier: Programming Language :: Python :: 3.9
+Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
+Classifier: Operating System :: OS Independent
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 ![焚靖](assets/fenjing.webp)
 
 > Bypass the WAF without knowing WAF
 
 焚靖是一个针对Jinja2 SSTI的命令行脚本，具有强大的自动绕过WAF功能
 
 ## 演示
@@ -182,10 +195,10 @@
     print(f"{shell_payload=}")
     print(f"{config_payload=}")
 
 ```
 
 ## 项目结构
 
-[![](https://mermaid.ink/img/pako:eNqFVMtugzAQ_BXLUm7hBzj0UPUP2iMS2thrsGps6keiNMq_F5pS2xhan2BmdryeNdwoMxxpTYUyF9aD9eTtudFkWi6cOgtjT4KXypEHOC9mlLHyEyNi8SOg82gjJIwd0hLt_OMVNV_5w8kEX41wVQa4i0VS-_YMNkFcj0q1P8rMXciuxEWI6rZDHZkC3OsqP4ZjoNtgVUQuIFoRNMvt56qWWWDvSyS__ocDYUqSqnpKIkqRvG5h8p0Tk1X0CZOPaSJS91UDW2zpXEjyLVb0vMHmAAqbMsR14besNNpS5bcmvxpkv6n5eFt2RYr_CpZR7YSY0XEC2dX-u880ru0WCkU26YJNmqRHOqAdQPLpn3CbSxrqexywofX0yFFAUL6hjb5PUgjevF41o7W3AY80jBw8vkiYPqGB1gKUw_sXrbFnVA?type=png)](https://mermaid.live/edit#pako:eNqFVMtugzAQ_BXLUm7hBzj0UPUP2iMS2thrsGps6keiNMq_F5pS2xhan2BmdryeNdwoMxxpTYUyF9aD9eTtudFkWi6cOgtjT4KXypEHOC9mlLHyEyNi8SOg82gjJIwd0hLt_OMVNV_5w8kEX41wVQa4i0VS-_YMNkFcj0q1P8rMXciuxEWI6rZDHZkC3OsqP4ZjoNtgVUQuIFoRNMvt56qWWWDvSyS__ocDYUqSqnpKIkqRvG5h8p0Tk1X0CZOPaSJS91UDW2zpXEjyLVb0vMHmAAqbMsR14besNNpS5bcmvxpkv6n5eFt2RYr_CpZR7YSY0XEC2dX-u880ru0WCkU26YJNmqRHOqAdQPLpn3CbSxrqexywofX0yFFAUL6hjb5PUgjevF41o7W3AY80jBw8vkiYPqGB1gKUw_sXrbFnVA)
+[![](https://mermaid.ink/img/pako:eNp1U01TwyAQ_SsMM-2p-QM5eHA86kU9aTqZLVkaRgKRD2vt9L8LwZQkrRwYeLzdfbyFE2W6QVpSLvWBtWAceb2vFAnD-t3eQN8S74S0JIFxMC21ET-YEYOfHq1DkyGuTTcNUdblbVqhapaVLJpCqJCIA8NpSSneOdiSQxEOO6FARmybGQfc-cjZRQ4XBrn-TuB2loYUxV3CLyLIQkWUbnPQakWakI85oRV5fpyUBF5zr1i9RzW_eM0MsI-pHZaBqr2Rt3lJ1FW6waCFuB6OUkMz0ZfFjZ2LI7hYf4GZ8GyLUtZ_8bPWcLG_xrnP7PkNb4LzNGQ9LzdccJlxAKf79UL15YGMfbv2djyZ-5vmocv_xC3cvyUvWk83tAvvDUQTvsgphlbUtdhhRcuwVOidAVnRSp0DFbzTL0fFaOmMxw31fQMOHwSE1nU0PExpA9qDetM677ERTpun9A2H33j-BR2iIbY?type=png)](https://mermaid.live/edit#pako:eNp1U01TwyAQ_SsMM-2p-QM5eHA86kU9aTqZLVkaRgKRD2vt9L8LwZQkrRwYeLzdfbyFE2W6QVpSLvWBtWAceb2vFAnD-t3eQN8S74S0JIFxMC21ET-YEYOfHq1DkyGuTTcNUdblbVqhapaVLJpCqJCIA8NpSSneOdiSQxEOO6FARmybGQfc-cjZRQ4XBrn-TuB2loYUxV3CLyLIQkWUbnPQakWakI85oRV5fpyUBF5zr1i9RzW_eM0MsI-pHZaBqr2Rt3lJ1FW6waCFuB6OUkMz0ZfFjZ2LI7hYf4GZ8GyLUtZ_8bPWcLG_xrnP7PkNb4LzNGQ9LzdccJlxAKf79UL15YGMfbv2djyZ-5vmocv_xC3cvyUvWk83tAvvDUQTvsgphlbUtdhhRcuwVOidAVnRSp0DFbzTL0fFaOmMxw31fQMOHwSE1nU0PExpA9qDetM677ERTpun9A2H33j-BR2iIbY)
```

### Comparing `fenjing-0.3.1/fenjing/cli.py` & `fenjing-0.3.2/fenjing/cli.py`

 * *Files identical despite different names*

### Comparing `fenjing-0.3.1/fenjing/colorize.py` & `fenjing-0.3.2/fenjing/colorize.py`

 * *Files identical despite different names*

### Comparing `fenjing-0.3.1/fenjing/config_payload.py` & `fenjing-0.3.2/fenjing/config_payload.py`

 * *Files identical despite different names*

### Comparing `fenjing-0.3.1/fenjing/const.py` & `fenjing-0.3.2/fenjing/const.py`

 * *Files identical despite different names*

### Comparing `fenjing-0.3.1/fenjing/form.py` & `fenjing-0.3.2/fenjing/form.py`

 * *Files identical despite different names*

### Comparing `fenjing-0.3.1/fenjing/form_cracker.py` & `fenjing-0.3.2/fenjing/form_cracker.py`

 * *Files identical despite different names*

### Comparing `fenjing-0.3.1/fenjing/full_payload_gen.py` & `fenjing-0.3.2/fenjing/full_payload_gen.py`

 * *Files identical despite different names*

### Comparing `fenjing-0.3.1/fenjing/int_vars.py` & `fenjing-0.3.2/fenjing/int_vars.py`

 * *Files identical despite different names*

### Comparing `fenjing-0.3.1/fenjing/payload_gen.py` & `fenjing-0.3.2/fenjing/payload_gen.py`

 * *Files identical despite different names*

### Comparing `fenjing-0.3.1/fenjing/requester.py` & `fenjing-0.3.2/fenjing/requester.py`

 * *Files identical despite different names*

### Comparing `fenjing-0.3.1/fenjing/scan_url.py` & `fenjing-0.3.2/fenjing/scan_url.py`

 * *Files identical despite different names*

### Comparing `fenjing-0.3.1/fenjing/shell_payload.py` & `fenjing-0.3.2/fenjing/shell_payload.py`

 * *Files identical despite different names*

### Comparing `fenjing-0.3.1/fenjing/static/style.css` & `fenjing-0.3.2/fenjing/static/style.css`

 * *Files identical despite different names*

### Comparing `fenjing-0.3.1/fenjing/templates/index.html` & `fenjing-0.3.2/fenjing/templates/index.html`

 * *Files identical despite different names*

### Comparing `fenjing-0.3.1/fenjing/waf_func_gen.py` & `fenjing-0.3.2/fenjing/waf_func_gen.py`

 * *Files identical despite different names*

### Comparing `fenjing-0.3.1/fenjing/webui.py` & `fenjing-0.3.2/fenjing/webui.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,35 +10,39 @@
 from .requester import Requester
 from .const import *
 
 logger = logging.getLogger("webui")
 app = Flask(__name__)
 tasks = {}
 
+
 class CallBackLogger:
     def __init__(self, flash_messages, messages):
         self.flash_messages = flash_messages
         self.messages = messages
 
     def callback_prepare_fullpayloadgen(self, data):
         self.messages.append(
             f"已经分析完毕所有上下文payload。"
         )
         if data["context"]:
+            context_repr = ', '.join(repr(value)
+                                     for value in data['context'].values())
             self.messages.append(
-                f"以下是在上下文中的值：{', '.join(data['context'].values())}"
+                f"以下是在上下文中的值：{context_repr}"
             )
         else:
             self.messages.append(
                 f"没有上下文payload可以通过waf。。。"
             )
         if not data["will_print"]:
             self.messages.append(
                 f"生成的payload将不会具有回显。"
             )
+
     def callback_generate_fullpayload(self, data):
         self.messages.append(
             f"分析完毕，已为类型{data['gen_type']}生成payload {data['payload']}"
         )
         if not data["will_print"]:
             self.messages.append(
                 f"payload将不会产生回显"
@@ -46,16 +50,16 @@
 
     def callback_generate_payload(self, data):
         payload_repr = data['payload']
         if len(payload_repr) > 30:
             payload_repr = payload_repr[:30] + "..."
         self.flash_messages.append(
             "请求{req}对应的payload可以是{payload}".format(
-                req = f"{data['gen_type']}({', '.join(repr(arg) for arg in data['args'])})",
-                payload = payload_repr
+                req=f"{data['gen_type']}({', '.join(repr(arg) for arg in data['args'])})",
+                payload=payload_repr
             )
         )
 
     def callback_submit(self, data):
         self.flash_messages.append(
             f"提交表单完成，返回值为{data['response'].status_code}，输入为{data['inputs']}，表单为{data['form']}"
         )
@@ -66,15 +70,16 @@
         testsuccess_msg = "payload测试成功！" if data["test_success"] else "payload测试失败。"
         will_print_msg = "其会产生回显。" if data["will_print"] else "其不会产生回显。"
         self.messages.append(
             testsuccess_msg + will_print_msg
         )
 
     def __call__(self, callback_type, data):
-        default_handler = lambda data: logger.warning(f"{callback_type=} not found")
+        def default_handler(data): 
+            return logger.warning(f"{callback_type=} not found")
         return {
             CALLBACK_PREPARE_FULLPAYLOADGEN: self.callback_prepare_fullpayloadgen,
             CALLBACK_GENERATE_FULLPAYLOAD: self.callback_generate_fullpayload,
             CALLBACK_GENERATE_PAYLOAD: self.callback_generate_payload,
             CALLBACK_SUBMIT: self.callback_submit,
             CALLBACK_TEST_FORM_INPUT: self.callback_test_form_input
         }.get(callback_type, default_handler)(data)
@@ -86,15 +91,15 @@
         self.result = None
         self.taskid = taskid
         self.form = form
 
         self.flash_messages = []
         self.messages = []
         self.callback = CallBackLogger(self.flash_messages, self.messages)
-        
+
         self.cracker = FormCracker(
             url=url,
             form=form,
             requester=Requester(
                 interval=interval,
                 user_agent=DEFAULT_USER_AGENT
             ),
@@ -104,79 +109,101 @@
     def run(self):
         self.result = self.cracker.crack()
         if self.result:
             self.messages.append(
                 f"WAF已绕过"
             )
 
+
 class InteractiveTaskThread(threading.Thread):
     def __init__(self, taskid, cracker, field, full_payload_gen, cmd):
         super().__init__()
         self.taskid = taskid
         self.cracker = cracker
         self.field = field
         self.full_payload_gen = full_payload_gen
         self.cmd = cmd
 
         self.flash_messages = []
         self.messages = []
         self.callback = CallBackLogger(self.flash_messages, self.messages)
-        
+
         self.cracker.callback = self.callback
 
     def run(self):
         payload, will_print = self.full_payload_gen.generate(
-            OS_POPEN_READ, 
+            OS_POPEN_READ,
             self.cmd
         )
         if not will_print:
             self.messages.append(
                 f"此payload不会产生回显"
             )
         r = self.cracker.submit({self.field: payload})
         assert r is not None
         self.messages.append(
             f"提交payload的回显如下："
         )
         self.messages.append(r.text)
 
 
-
 @app.route("/")
 def index():
     return render_template("index.html")
 
-@app.route("/createTask", methods = ["POST", ]) # type: ignore
+def create_crack_task(url, method, inputs, action, interval):
+    form = Form(
+        action=action or urlparse(url).path,
+        method=method,
+        inputs=inputs.split(",")
+    )
+    taskid = uuid.uuid4().hex
+    task = CrackTaskThread(taskid, url, form, float(interval))
+    task.daemon = True
+    task.start()
+    tasks[taskid] = task
+    return taskid
+
+def create_interactive_id(cmd, last_task):
+    cracker, field, full_payload_gen = (
+        last_task.cracker,
+        last_task.result.input_field,
+        last_task.result.full_payload_gen
+    )
+    taskid = uuid.uuid4().hex
+    task = InteractiveTaskThread(
+        taskid,
+        cracker,
+        field,
+        full_payload_gen,
+        cmd
+    )
+    task.daemon = True
+    task.start()
+    tasks[taskid] = task
+    return taskid
+
+
+@app.route("/createTask", methods=["POST", ])  # type: ignore
 def create_task():
     if request.form.get("type", None) not in ["crack", "interactive"]:
         logging.info(request.form)
         return jsonify({
             "code": APICODE_WRONG_INPUT,
             "message": f"unknown type {request.form.get('type', None)}"
         })
     task_type = request.form.get("type", None)
     if task_type == "crack":
-        url, method, inputs, action, interval = (
+        taskid = create_crack_task(
             request.form["url"],
             request.form["method"],
             request.form["inputs"],
             request.form["action"],
             request.form["interval"],
-
         )
-        form = Form(
-            action=action or urlparse(url).path,
-            method=method,
-            inputs=inputs.split(",")
-        )
-        taskid = uuid.uuid4().hex
-        task = CrackTaskThread(taskid, url, form, float(interval))
-        task.daemon = True
-        task.start()
-        tasks[taskid] = task
         return jsonify({
             "code": APICODE_OK,
             "taskid": taskid
         })
     elif task_type == "interactive":
         cmd, last_task_id = (
             request.form["cmd"],
@@ -194,36 +221,22 @@
                 "message": f"last_task_id not found: {last_task_id}"
             })
         if last_task.result is None:
             return jsonify({
                 "code": APICODE_WRONG_INPUT,
                 "message": f"specified last_task failed: {last_task_id}"
             })
-        cracker, field, full_payload_gen = (
-            last_task.cracker,
-            last_task.result.input_field,
-            last_task.result.full_payload_gen
-        )
-        taskid = uuid.uuid4().hex
-        task = InteractiveTaskThread(
-            taskid, 
-            cracker, 
-            field, 
-            full_payload_gen, 
-            cmd
-        )
-        task.daemon = True
-        task.start()
-        tasks[taskid] = task
+        taskid = create_interactive_id(cmd, last_task)
         return jsonify({
             "code": APICODE_OK,
             "taskid": taskid
         })
 
-@app.route("/watchTask", methods = ["POST", ]) # type: ignore
+
+@app.route("/watchTask", methods=["POST", ])  # type: ignore
 def watchTask():
     if "taskid" not in request.form:
         return jsonify({
             "code": APICODE_WRONG_INPUT,
             "message": "taskid not provided"
         })
     if request.form["taskid"] not in tasks:
@@ -246,12 +259,14 @@
             "code": APICODE_OK,
             "taskid": task.taskid,
             "done": not task.is_alive(),
             "messages": task.messages,
             "flash_messages": task.flash_messages,
         })
 
+
 def main():
     app.run(host="127.0.0.1", port=11451)
 
+
 if __name__ == "__main__":
-    main()
+    main()
```

### Comparing `fenjing-0.3.1/fenjing.egg-info/PKG-INFO` & `fenjing-0.3.2/fenjing.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fenjing
-Version: 0.3.1
+Version: 0.3.2
 Summary: A Jinja2 SSTI cracker for CTF competitions
 Home-page: https://github.com/Marven11/Fenjing
 Author: Marven11
 Author-email: marven11@example.com
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Operating System :: OS Independent
@@ -195,10 +195,10 @@
     print(f"{shell_payload=}")
     print(f"{config_payload=}")
 
 ```
 
 ## 项目结构
 
-[![](https://mermaid.ink/img/pako:eNqFVMtugzAQ_BXLUm7hBzj0UPUP2iMS2thrsGps6keiNMq_F5pS2xhan2BmdryeNdwoMxxpTYUyF9aD9eTtudFkWi6cOgtjT4KXypEHOC9mlLHyEyNi8SOg82gjJIwd0hLt_OMVNV_5w8kEX41wVQa4i0VS-_YMNkFcj0q1P8rMXciuxEWI6rZDHZkC3OsqP4ZjoNtgVUQuIFoRNMvt56qWWWDvSyS__ocDYUqSqnpKIkqRvG5h8p0Tk1X0CZOPaSJS91UDW2zpXEjyLVb0vMHmAAqbMsR14besNNpS5bcmvxpkv6n5eFt2RYr_CpZR7YSY0XEC2dX-u880ru0WCkU26YJNmqRHOqAdQPLpn3CbSxrqexywofX0yFFAUL6hjb5PUgjevF41o7W3AY80jBw8vkiYPqGB1gKUw_sXrbFnVA?type=png)](https://mermaid.live/edit#pako:eNqFVMtugzAQ_BXLUm7hBzj0UPUP2iMS2thrsGps6keiNMq_F5pS2xhan2BmdryeNdwoMxxpTYUyF9aD9eTtudFkWi6cOgtjT4KXypEHOC9mlLHyEyNi8SOg82gjJIwd0hLt_OMVNV_5w8kEX41wVQa4i0VS-_YMNkFcj0q1P8rMXciuxEWI6rZDHZkC3OsqP4ZjoNtgVUQuIFoRNMvt56qWWWDvSyS__ocDYUqSqnpKIkqRvG5h8p0Tk1X0CZOPaSJS91UDW2zpXEjyLVb0vMHmAAqbMsR14besNNpS5bcmvxpkv6n5eFt2RYr_CpZR7YSY0XEC2dX-u880ru0WCkU26YJNmqRHOqAdQPLpn3CbSxrqexywofX0yFFAUL6hjb5PUgjevF41o7W3AY80jBw8vkiYPqGB1gKUw_sXrbFnVA)
+[![](https://mermaid.ink/img/pako:eNp1U01TwyAQ_SsMM-2p-QM5eHA86kU9aTqZLVkaRgKRD2vt9L8LwZQkrRwYeLzdfbyFE2W6QVpSLvWBtWAceb2vFAnD-t3eQN8S74S0JIFxMC21ET-YEYOfHq1DkyGuTTcNUdblbVqhapaVLJpCqJCIA8NpSSneOdiSQxEOO6FARmybGQfc-cjZRQ4XBrn-TuB2loYUxV3CLyLIQkWUbnPQakWakI85oRV5fpyUBF5zr1i9RzW_eM0MsI-pHZaBqr2Rt3lJ1FW6waCFuB6OUkMz0ZfFjZ2LI7hYf4GZ8GyLUtZ_8bPWcLG_xrnP7PkNb4LzNGQ9LzdccJlxAKf79UL15YGMfbv2djyZ-5vmocv_xC3cvyUvWk83tAvvDUQTvsgphlbUtdhhRcuwVOidAVnRSp0DFbzTL0fFaOmMxw31fQMOHwSE1nU0PExpA9qDetM677ERTpun9A2H33j-BR2iIbY?type=png)](https://mermaid.live/edit#pako:eNp1U01TwyAQ_SsMM-2p-QM5eHA86kU9aTqZLVkaRgKRD2vt9L8LwZQkrRwYeLzdfbyFE2W6QVpSLvWBtWAceb2vFAnD-t3eQN8S74S0JIFxMC21ET-YEYOfHq1DkyGuTTcNUdblbVqhapaVLJpCqJCIA8NpSSneOdiSQxEOO6FARmybGQfc-cjZRQ4XBrn-TuB2loYUxV3CLyLIQkWUbnPQakWakI85oRV5fpyUBF5zr1i9RzW_eM0MsI-pHZaBqr2Rt3lJ1FW6waCFuB6OUkMz0ZfFjZ2LI7hYf4GZ8GyLUtZ_8bPWcLG_xrnP7PkNb4LzNGQ9LzdccJlxAKf79UL15YGMfbv2djyZ-5vmocv_xC3cvyUvWk83tAvvDUQTvsgphlbUtdhhRcuwVOidAVnRSp0DFbzTL0fFaOmMxw31fQMOHwSE1nU0PExpA9qDetM677ERTpun9A2H33j-BR2iIbY)
```

### Comparing `fenjing-0.3.1/fenjing.egg-info/SOURCES.txt` & `fenjing-0.3.2/fenjing.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fenjing-0.3.1/setup.py` & `fenjing-0.3.2/setup.py`

 * *Files identical despite different names*

