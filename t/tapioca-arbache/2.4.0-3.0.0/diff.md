# Comparing `tmp/tapioca_arbache-2.4.0.tar.gz` & `tmp/tapioca_arbache-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tapioca_arbache-2.4.0.tar", max compression
+gzip compressed data, was "tapioca_arbache-3.0.0.tar", max compression
```

## Comparing `tapioca_arbache-2.4.0.tar` & `tapioca_arbache-3.0.0.tar`

### file list

```diff
@@ -1,6 +1,7 @@
--rw-r--r--   0        0        0     1073 2023-05-10 00:54:45.318021 tapioca_arbache-2.4.0/LICENSE
--rw-r--r--   0        0        0      506 2023-05-10 00:54:45.318021 tapioca_arbache-2.4.0/pyproject.toml
--rw-r--r--   0        0        0      280 2023-05-10 00:54:45.318021 tapioca_arbache-2.4.0/tapioca_arbache/__init__.py
--rw-r--r--   0        0        0     2327 2023-05-10 00:54:45.318021 tapioca_arbache-2.4.0/tapioca_arbache/resource_mapping.py
--rw-r--r--   0        0        0     6016 2023-05-10 00:54:45.318021 tapioca_arbache-2.4.0/tapioca_arbache/tapioca_arbache.py
--rw-r--r--   0        0        0      489 1970-01-01 00:00:00.000000 tapioca_arbache-2.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-05-18 14:21:44.189590 tapioca_arbache-3.0.0/LICENSE
+-rw-r--r--   0        0        0      506 2023-05-18 14:21:44.189590 tapioca_arbache-3.0.0/pyproject.toml
+-rw-r--r--   0        0        0      280 2023-05-18 14:21:44.189590 tapioca_arbache-3.0.0/tapioca_arbache/__init__.py
+-rw-r--r--   0        0        0      214 2023-05-18 14:21:44.189590 tapioca_arbache-3.0.0/tapioca_arbache/exceptions.py
+-rw-r--r--   0        0        0     2327 2023-05-18 14:21:44.189590 tapioca_arbache-3.0.0/tapioca_arbache/resource_mapping.py
+-rw-r--r--   0        0        0     6155 2023-05-18 14:21:44.189590 tapioca_arbache-3.0.0/tapioca_arbache/tapioca_arbache.py
+-rw-r--r--   0        0        0      489 1970-01-01 00:00:00.000000 tapioca_arbache-3.0.0/PKG-INFO
```

### Comparing `tapioca_arbache-2.4.0/LICENSE` & `tapioca_arbache-3.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tapioca_arbache-2.4.0/tapioca_arbache/resource_mapping.py` & `tapioca_arbache-3.0.0/tapioca_arbache/resource_mapping.py`

 * *Files identical despite different names*

### Comparing `tapioca_arbache-2.4.0/tapioca_arbache/tapioca_arbache.py` & `tapioca_arbache-3.0.0/tapioca_arbache/tapioca_arbache.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 import json
+
 from tapioca import (
     JSONAdapterMixin, TapiocaAdapter, generate_wrapper_from_adapter
 )
 from requests_oauthlib import OAuth2
+from tapioca.exceptions import ClientError
+
 from tapioca_arbache.resource_mapping import (
     CRM_EQUIPES_ENDPOINT, CRM_MIDIAS_ENDPOINT, CRM_PERFIL_ENDPOINT, CRM_OAUTH,
     CRM_LICENCA_ENDPOINT, INTERFACE, JOGO_SELF, PLAY_MIDIAS_ENDPOINT,
     RELATORIOS, CRM_JOGO_ENDPOINT, PLAY_RESULTADOS_JOGOS_ENDPOINT,
     PLAY_SUBDOMINIO_ENDPOINT, PLAY_JOGO_SUBDOMINIO_ENDPOINT
 )
-from tapioca.exceptions import ClientError
+from tapioca_arbache.exceptions import ConflictException
 
 
 class ArbacheAdapter(JSONAdapterMixin, TapiocaAdapter):
     prod_url = 'https://crm.arbache.com.br'
     homolog_url = 'https://crm-homolog.arbache.dev.br'
     dev_url = 'http://127.0.0.1:8000'
 
@@ -60,16 +63,18 @@
             iterator_request_kwargs['params']['pagina'] = 2
         else:
             iterator_request_kwargs['params']['pagina'] = pagina_atual + 1
 
         return iterator_request_kwargs
 
     def process_response(self, response):
+        if response.status_code == 409:
+            raise ConflictException()
 
-        if 400 <= response.status_code < 500:
+        elif 400 <= response.status_code < 500:
             if response.content and response.request.body:
                 response_body = json.loads(response.content)
                 request_body = json.loads(response.request.body)
 
                 message = json.dumps(
                     {
                         'status_code': response.status_code,
```

