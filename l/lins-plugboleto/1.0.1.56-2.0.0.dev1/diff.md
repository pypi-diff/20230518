# Comparing `tmp/lins_plugboleto-1.0.1.56.tar.gz` & `tmp/lins_plugboleto-2.0.0.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/lins_plugboleto-1.0.1.56.tar", last modified: Tue Apr 14 13:15:22 2020, max compression
+gzip compressed data, was "dist/lins_plugboleto-2.0.0.dev1.tar", last modified: Thu May 18 18:00:19 2023, max compression
```

## Comparing `lins_plugboleto-1.0.1.56.tar` & `lins_plugboleto-2.0.0.dev1.tar`

### file list

```diff
@@ -1,24 +1,34 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-04-14 13:15:22.000000 lins_plugboleto-1.0.1.56/
--rw-r--r--   0 root         (0) root         (0)      296 2020-04-14 13:15:22.000000 lins_plugboleto-1.0.1.56/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2080 2020-04-14 13:15:09.000000 lins_plugboleto-1.0.1.56/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-04-14 13:15:22.000000 lins_plugboleto-1.0.1.56/lins_plugboleto/
--rw-rw-rw-   0 root         (0) root         (0)      107 2020-04-14 13:15:09.000000 lins_plugboleto-1.0.1.56/lins_plugboleto/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      180 2020-04-14 13:15:09.000000 lins_plugboleto-1.0.1.56/lins_plugboleto/authorize.py
--rw-rw-rw-   0 root         (0) root         (0)     3577 2020-04-14 13:15:09.000000 lins_plugboleto-1.0.1.56/lins_plugboleto/criar_boleto.py
--rw-rw-rw-   0 root         (0) root         (0)      435 2020-04-14 13:15:09.000000 lins_plugboleto-1.0.1.56/lins_plugboleto/environment.py
--rw-rw-rw-   0 root         (0) root         (0)     1510 2020-04-14 13:15:09.000000 lins_plugboleto-1.0.1.56/lins_plugboleto/objectJSON.py
--rw-rw-rw-   0 root         (0) root         (0)      860 2020-04-14 13:15:09.000000 lins_plugboleto-1.0.1.56/lins_plugboleto/plugBoleto.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-04-14 13:15:22.000000 lins_plugboleto-1.0.1.56/lins_plugboleto/request/
--rw-rw-rw-   0 root         (0) root         (0)        0 2020-04-14 13:15:09.000000 lins_plugboleto-1.0.1.56/lins_plugboleto/request/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2089 2020-04-14 13:15:09.000000 lins_plugboleto-1.0.1.56/lins_plugboleto/request/base.py
--rw-rw-rw-   0 root         (0) root         (0)      361 2020-04-14 13:15:09.000000 lins_plugboleto-1.0.1.56/lins_plugboleto/request/busca_boleto.py
--rw-rw-rw-   0 root         (0) root         (0)      953 2020-04-14 13:15:09.000000 lins_plugboleto-1.0.1.56/lins_plugboleto/request/criar_boleto.py
--rw-rw-rw-   0 root         (0) root         (0)      320 2020-04-14 13:15:09.000000 lins_plugboleto-1.0.1.56/lins_plugboleto/request/numero_doc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-04-14 13:15:22.000000 lins_plugboleto-1.0.1.56/lins_plugboleto.egg-info/
--rw-rw-rw-   0 root         (0) root         (0)      296 2020-04-14 13:15:22.000000 lins_plugboleto-1.0.1.56/lins_plugboleto.egg-info/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      578 2020-04-14 13:15:22.000000 lins_plugboleto-1.0.1.56/lins_plugboleto.egg-info/SOURCES.txt
--rw-rw-rw-   0 root         (0) root         (0)        1 2020-04-14 13:15:22.000000 lins_plugboleto-1.0.1.56/lins_plugboleto.egg-info/dependency_links.txt
--rw-rw-rw-   0 root         (0) root         (0)        1 2020-04-14 13:15:16.000000 lins_plugboleto-1.0.1.56/lins_plugboleto.egg-info/not-zip-safe
--rw-rw-rw-   0 root         (0) root         (0)       16 2020-04-14 13:15:22.000000 lins_plugboleto-1.0.1.56/lins_plugboleto.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2020-04-14 13:15:22.000000 lins_plugboleto-1.0.1.56/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      477 2020-04-14 13:15:09.000000 lins_plugboleto-1.0.1.56/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 18:00:19.000000 lins_plugboleto-2.0.0.dev1/
+-rw-rw-rw-   0 root         (0) root         (0)       44 2023-05-18 17:59:53.000000 lins_plugboleto-2.0.0.dev1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      579 2023-05-18 18:00:19.000000 lins_plugboleto-2.0.0.dev1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2076 2023-05-18 17:59:53.000000 lins_plugboleto-2.0.0.dev1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 18:00:19.000000 lins_plugboleto-2.0.0.dev1/lins_plugboleto/
+-rw-rw-rw-   0 root         (0) root         (0)      106 2023-05-18 17:59:53.000000 lins_plugboleto-2.0.0.dev1/lins_plugboleto/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      178 2023-05-18 17:59:53.000000 lins_plugboleto-2.0.0.dev1/lins_plugboleto/authorize.py
+-rw-rw-rw-   0 root         (0) root         (0)     3595 2023-05-18 17:59:53.000000 lins_plugboleto-2.0.0.dev1/lins_plugboleto/criar_boleto.py
+-rw-rw-rw-   0 root         (0) root         (0)     1379 2023-05-18 17:59:53.000000 lins_plugboleto-2.0.0.dev1/lins_plugboleto/environment.py
+-rw-rw-rw-   0 root         (0) root         (0)     1410 2023-05-18 17:59:53.000000 lins_plugboleto-2.0.0.dev1/lins_plugboleto/objectJSON.py
+-rw-rw-rw-   0 root         (0) root         (0)      832 2023-05-18 17:59:53.000000 lins_plugboleto-2.0.0.dev1/lins_plugboleto/plugBoleto.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 18:00:19.000000 lins_plugboleto-2.0.0.dev1/lins_plugboleto/request/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-18 17:59:53.000000 lins_plugboleto-2.0.0.dev1/lins_plugboleto/request/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2124 2023-05-18 17:59:53.000000 lins_plugboleto-2.0.0.dev1/lins_plugboleto/request/base.py
+-rw-rw-rw-   0 root         (0) root         (0)      352 2023-05-18 17:59:53.000000 lins_plugboleto-2.0.0.dev1/lins_plugboleto/request/busca_boleto.py
+-rw-rw-rw-   0 root         (0) root         (0)     1011 2023-05-18 17:59:53.000000 lins_plugboleto-2.0.0.dev1/lins_plugboleto/request/criar_boleto.py
+-rw-rw-rw-   0 root         (0) root         (0)      315 2023-05-18 17:59:53.000000 lins_plugboleto-2.0.0.dev1/lins_plugboleto/request/numero_doc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 18:00:19.000000 lins_plugboleto-2.0.0.dev1/lins_plugboleto/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-18 17:59:53.000000 lins_plugboleto-2.0.0.dev1/lins_plugboleto/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4390 2023-05-18 17:59:53.000000 lins_plugboleto-2.0.0.dev1/lins_plugboleto/tests/test_base.py
+-rw-rw-rw-   0 root         (0) root         (0)     1079 2023-05-18 17:59:53.000000 lins_plugboleto-2.0.0.dev1/lins_plugboleto/tests/test_busca_boleto.py
+-rw-rw-rw-   0 root         (0) root         (0)     2589 2023-05-18 17:59:53.000000 lins_plugboleto-2.0.0.dev1/lins_plugboleto/tests/test_criar_boleto.py
+-rw-rw-rw-   0 root         (0) root         (0)     1032 2023-05-18 17:59:53.000000 lins_plugboleto-2.0.0.dev1/lins_plugboleto/tests/test_numero_doc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 18:00:19.000000 lins_plugboleto-2.0.0.dev1/lins_plugboleto.egg-info/
+-rw-rw-rw-   0 root         (0) root         (0)      579 2023-05-18 18:00:19.000000 lins_plugboleto-2.0.0.dev1/lins_plugboleto.egg-info/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      853 2023-05-18 18:00:19.000000 lins_plugboleto-2.0.0.dev1/lins_plugboleto.egg-info/SOURCES.txt
+-rw-rw-rw-   0 root         (0) root         (0)        1 2023-05-18 18:00:19.000000 lins_plugboleto-2.0.0.dev1/lins_plugboleto.egg-info/dependency_links.txt
+-rw-rw-rw-   0 root         (0) root         (0)        1 2023-05-18 18:00:12.000000 lins_plugboleto-2.0.0.dev1/lins_plugboleto.egg-info/not-zip-safe
+-rw-rw-rw-   0 root         (0) root         (0)       38 2023-05-18 18:00:19.000000 lins_plugboleto-2.0.0.dev1/lins_plugboleto.egg-info/requires.txt
+-rw-rw-rw-   0 root         (0) root         (0)       16 2023-05-18 18:00:19.000000 lins_plugboleto-2.0.0.dev1/lins_plugboleto.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)       38 2023-05-18 17:59:53.000000 lins_plugboleto-2.0.0.dev1/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-18 18:00:19.000000 lins_plugboleto-2.0.0.dev1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1121 2023-05-18 17:59:53.000000 lins_plugboleto-2.0.0.dev1/setup.py
+-rw-rw-rw-   0 root         (0) root         (0)       11 2023-05-18 17:59:53.000000 lins_plugboleto-2.0.0.dev1/version.txt
```

### Comparing `lins_plugboleto-1.0.1.56/README.md` & `lins_plugboleto-2.0.0.dev1/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -16,16 +16,15 @@
 ======================
   * Configurar authorize e enviroment
 
         config = configurar_ambiente_boleto()
 
         def configurar_ambiente_boleto():
 
-            env_sandbox = True
-            env_boleto = Environment(sandbox=env_sandbox)
+            env_boleto = Environment.from_sandbox() ou Environment.from_production()
             authorize = Authorize('01001001000113', 'f22b97c0c9a3d41ac0a3875aba69e5aa', '01001001000113')
             return PlugBoleto(authorize, env_boleto)
 
   * Gerar numero de documento
 
         nosso_numero = config.gerar_nossonumero()
```

### Comparing `lins_plugboleto-1.0.1.56/lins_plugboleto/criar_boleto.py` & `lins_plugboleto-2.0.0.dev1/lins_plugboleto/criar_boleto.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,94 +1,96 @@
-from datetime import datetime, timedelta
+from datetime import timedelta
+
 from .objectJSON import ObjectJSON
 
 
 class Boleto(ObjectJSON):
-
     def __init__(self, titulo, cedente, mensagem, prazo_baixa):
         self.idintegracao = None
         self.situacao = None
         self.body = None
-        #sacado
+        # sacado
         self.SacadoCPFCNPJ = None
         self.SacadoNome = None
         self.SacadoEnderecoLogradouro = None
         self.SacadoEnderecoNumero = None
         self.SacadoEnderecoBairro = None
         self.SacadoEnderecoCep = None
         self.SacadoEnderecoCidade = None
         self.SacadoEnderecoComplemento = None
         self.SacadoEnderecoPais = None
         self.SacadoEnderecoUf = None
         self.SacadoEmail = None
         self.SacadoTelefone = None
         self.SacadoCelular = None
 
-        #cedente
-        self.CedenteContaCodigoBanco = str(cedente['CedenteContaCodigoBanco'])
-        self.CedenteContaNumero = str(cedente['CedenteContaNumero'])
-        self.CedenteContaNumeroDV = str(cedente['CedenteContaNumeroDV'])
-        self.CedenteConvenioNumero = str(cedente['CedenteConvenioNumero'])
+        # cedente
+        self.CedenteContaCodigoBanco = str(cedente["CedenteContaCodigoBanco"])
+        self.CedenteContaNumero = str(cedente["CedenteContaNumero"])
+        self.CedenteContaNumeroDV = str(cedente["CedenteContaNumeroDV"])
+        self.CedenteConvenioNumero = str(cedente["CedenteConvenioNumero"])
 
-        #titulo
+        # titulo
         self.TituloNossoNumero = None
         self.TituloNumeroDocumento = None
-        self.TituloValor = str(titulo['TituloValor'])
-        dataemissao = titulo['TituloDataEmissao'].strftime('%d/%m/%Y')
+        self.TituloValor = str(titulo["TituloValor"])
+        dataemissao = titulo["TituloDataEmissao"].strftime("%d/%m/%Y")
         self.TituloDataEmissao = dataemissao
-        datavencimento = (titulo['TituloDataEmissao'] + timedelta(days=titulo['PrazoVencimento']))
-        datavencimento = datavencimento.strftime('%d/%m/%Y')
+        datavencimento = titulo["TituloDataEmissao"] + timedelta(
+            days=titulo["PrazoVencimento"]
+        )
+        datavencimento = datavencimento.strftime("%d/%m/%Y")
         self.TituloDataVencimento = datavencimento
         self.TituloAceite = None
         self.TituloDocEspecie = None
-        self.TituloLocalPagamento = titulo['TituloLocalPagamento']
+        self.TituloLocalPagamento = titulo["TituloLocalPagamento"]
 
-        #juros
+        # juros
         self.TituloCodigoJuros = None
         self.TituloDataJuros = None
         self.TituloValorJuros = None
 
-        #multa
+        # multa
         self.TituloCodigoMulta = None
         self.TituloDataMulta = None
         self.TituloValorMultaTaxa = None
 
-        #protesto
+        # protesto
         self.TituloCodProtesto = None
         self.TituloPrazoProtesto = None
 
-        #baixa = None
-        if (prazo_baixa > 0):
-            self.TituloCodBaixaDevolucao = '1'
+        # baixa = None
+        if prazo_baixa > 0:
+            self.TituloCodBaixaDevolucao = "1"
             self.TituloPrazoBaixa = str(prazo_baixa)
 
-        #mensagens
-        self.TituloMensagem01 = str(mensagem['TituloMensagem01'])
-        self.TituloMensagem02 = str(mensagem['TituloMensagem02'])
-        self.TituloMensagem03 = str(mensagem['TituloMensagem03'])
+        # mensagens
+        self.TituloMensagem01 = str(mensagem["TituloMensagem01"])
+        self.TituloMensagem02 = str(mensagem["TituloMensagem02"])
+        self.TituloMensagem03 = str(mensagem["TituloMensagem03"])
         self.sacadoravalista = None
 
-        #outros
+        # outros
         self.TituloEmissaoBoleto = None
         self.TituloCategoria = None
         self.TituloPostagemBoleto = None
         self.TituloCodEmissaoBloqueto = None
         self.TituloCodDistribuicaoBloqueto = None
         self.TituloOutrosAcrescimos = None
         self.TituloInformacoesAdicionais = None
         self.TituloInstrucoes = None
         self.TituloParcela = None
         self.TituloVariacaoCarteira = None
         self.TituloCodigoReferencia = None
         self.TituloTipoCobranca = None
 
     def update_return(self, r, body):
-        dados = r.get('_dados') or {}
-        sucesso = dados.get('_sucesso') or {}
+        dados = r.get("_dados") or {}
+        sucesso = dados.get("_sucesso") or {}
         self.body = body
-        self.idintegracao = sucesso[0]['idintegracao']
-        self.situacao = sucesso[0]['situacao']
-        self.TituloNumeroDocumento = sucesso[0]['TituloNumeroDocumento']
-        self.TituloNossoNumero = sucesso[0]['TituloNossoNumero']
-        self.CedenteContaCodigoBanco = sucesso[0]['CedenteContaCodigoBanco']
-        self.CedenteContaNumero = sucesso[0]['CedenteContaNumero']
-        self.CedenteConvenioNumero = sucesso[0]['CedenteConvenioNumero']
+        self.idintegracao = sucesso[0]["idintegracao"]
+        self.situacao = sucesso[0]["situacao"]
+        self.TituloNumeroDocumento = sucesso[0]["TituloNumeroDocumento"]
+        self.TituloNossoNumero = sucesso[0]["TituloNossoNumero"]
+        self.CedenteContaCodigoBanco = sucesso[0]["CedenteContaCodigoBanco"]
+        self.CedenteContaNumero = sucesso[0]["CedenteContaNumero"]
+        self.CedenteConvenioNumero = sucesso[0]["CedenteConvenioNumero"]
```

### Comparing `lins_plugboleto-1.0.1.56/lins_plugboleto/plugBoleto.py` & `lins_plugboleto-2.0.0.dev1/lins_plugboleto/plugBoleto.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,21 +1,18 @@
-from .request.criar_boleto import CriarBoleto
 from .request.busca_boleto import BuscaBoleto
+from .request.criar_boleto import CriarBoleto
 from .request.numero_doc import NumeroDoc
 
 
 class PlugBoleto(object):
-
     def __init__(self, authorize, environment):
-
         self.environment = environment
         self.authorize = authorize
 
     def criar_boleto(self, criar_boleto):
-
         request = CriarBoleto(self.authorize, self.environment)
 
         return request.execute(criar_boleto)
 
     def gerar_nossonumero(self):
         request = NumeroDoc(None, self.environment)
 
@@ -23,10 +20,8 @@
 
     def consulta_boleto(self, id_integracao):
         request = BuscaBoleto(self.authorize, self.environment)
 
         return request.execute(id_integracao)
 
     def link_boleto(self, id_integracao):
-        uri = '%sboletos/impressao/%s' % (self.environment.api, id_integracao)
-
-        return uri
+        return f"{self.environment.api}boletos/impressao/{id_integracao}"
```

### Comparing `lins_plugboleto-1.0.1.56/lins_plugboleto/request/base.py` & `lins_plugboleto-2.0.0.dev1/lins_plugboleto/request/base.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,83 +1,75 @@
-import uuid
 import json
+
 from requests import Request, Session
 
 
 class Base(object):
-
     def __init__(self, authorize):
-
         self.authorize = authorize
 
     def send_request(self, method, uri, data=None, params=None):
-
-        s = Session()
+        session = Session()
 
         body = data
 
         headers = {
-            'cnpj-sh': self.authorize.cnpjsh,
-            'token-sh': self.authorize.tokensh,
-            'cnpj-cedente': self.authorize.cnpjcedente
+            "cnpj-sh": self.authorize.cnpjsh,
+            "token-sh": self.authorize.tokensh,
+            "cnpj-cedente": self.authorize.cnpjcedente,
         }
 
         if not body:
-            headers['Content-Length'] = '0'
+            headers["Content-Length"] = "0"
         else:
             headers["Content-Type"] = "application/json"
 
             if not isinstance(data, dict):
                 body = body.toJSON()
 
         req = Request(method, uri, data=body, headers=headers, params=params)
 
-        prep = s.prepare_request(req)
+        prep = session.prepare_request(req)
 
-        response = s.send(prep)
+        response = session.send(prep)
 
-        if 'json' in response.headers['Content-Type'].lower():
+        if "json" in response.headers["Content-Type"].lower():
             answers = response.json()
         else:
-            answers = [{
-                'Code': str(response.status_code),
-                'Message': response.text
-            }]
+            answers = [{"Code": str(response.status_code), "Message": response.text}]
 
         if response.status_code >= 400:
             errors = response.json()
             raise Exception(errors)
 
         return answers, body
 
     def request_numerodoc(self, method, uri):
-
         s = Session()
-
         req = Request(method, uri)
-
         prep = s.prepare_request(req)
-
         response = s.send(prep)
-
         body = None
 
-        if 'json' in response.headers['Content-Type'].lower():
+        if "json" in response.headers["Content-Type"].lower():
             answers = response.json()
         else:
-            answers = [{
-                'Code': str(response.status_code),
-                'Message': response.text
-            }]
+            answers = [{"Code": str(response.status_code), "Message": response.text}]
 
         if response.status_code >= 400:
-            errors = []
-
-            for answer in answers:
-                errors.append('\r\n * [%s] %s\r\n' % (answer['Code'], answer['Message']))
-
-            data_send = json.loads(body or 'null')
-
-            raise Exception('\r\n%s\r\nMethod: %s\r\nUri: %s\r\nData: %s' % (
-                ''.join(errors), method, response.url, json.dumps(data_send, indent=2)))
+            errors = [
+                "\r\n * [%s] %s\r\n" % (answer["Code"], answer["Message"])
+                for answer in answers
+            ]
+            data_send = json.loads(body or "null")
+
+            raise Exception(
+                "\r\n%s\r\nMethod: %s\r\nUri: %s\r\nData: %s"
+                % (
+                    "".join(errors),
+                    method,
+                    response.url,
+                    json.dumps(data_send, indent=2),
+                )
+            )
 
         return answers
```

### Comparing `lins_plugboleto-1.0.1.56/lins_plugboleto.egg-info/SOURCES.txt` & `lins_plugboleto-2.0.0.dev1/lins_plugboleto.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,27 @@
+MANIFEST.in
 README.md
+requirements.txt
 setup.py
+version.txt
 lins_plugboleto/__init__.py
 lins_plugboleto/authorize.py
 lins_plugboleto/criar_boleto.py
 lins_plugboleto/environment.py
 lins_plugboleto/objectJSON.py
 lins_plugboleto/plugBoleto.py
 lins_plugboleto.egg-info/PKG-INFO
 lins_plugboleto.egg-info/SOURCES.txt
 lins_plugboleto.egg-info/dependency_links.txt
 lins_plugboleto.egg-info/not-zip-safe
+lins_plugboleto.egg-info/requires.txt
 lins_plugboleto.egg-info/top_level.txt
 lins_plugboleto/request/__init__.py
 lins_plugboleto/request/base.py
 lins_plugboleto/request/busca_boleto.py
 lins_plugboleto/request/criar_boleto.py
-lins_plugboleto/request/numero_doc.py
+lins_plugboleto/request/numero_doc.py
+lins_plugboleto/tests/__init__.py
+lins_plugboleto/tests/test_base.py
+lins_plugboleto/tests/test_busca_boleto.py
+lins_plugboleto/tests/test_criar_boleto.py
+lins_plugboleto/tests/test_numero_doc.py
```

