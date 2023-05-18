# Comparing `tmp/proventosweb-0.7.tar.gz` & `tmp/proventosweb-0.70.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "proventosweb-0.7.tar", last modified: Tue May  9 18:04:31 2023, max compression
+gzip compressed data, was "proventosweb-0.70.tar", last modified: Thu May 18 18:55:15 2023, max compression
```

## Comparing `proventosweb-0.7.tar` & `proventosweb-0.70.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-05-09 18:04:31.038541 proventosweb-0.7/
--rw-rw-rw-   0        0        0      264 2023-05-09 18:04:31.037544 proventosweb-0.7/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-09 18:04:30.998090 proventosweb-0.7/proventosweb/
--rw-rw-rw-   0        0        0       44 2023-05-09 18:01:30.000000 proventosweb-0.7/proventosweb/__init__.py
--rw-rw-rw-   0        0        0    12340 2023-05-09 18:02:59.000000 proventosweb-0.7/proventosweb/proventosweb.py
-drwxrwxrwx   0        0        0        0 2023-05-09 18:04:31.035550 proventosweb-0.7/proventosweb.egg-info/
--rw-rw-rw-   0        0        0      264 2023-05-09 18:04:30.000000 proventosweb-0.7/proventosweb.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      276 2023-05-09 18:04:30.000000 proventosweb-0.7/proventosweb.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-09 18:04:30.000000 proventosweb-0.7/proventosweb.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-05-03 22:03:21.000000 proventosweb-0.7/proventosweb.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       35 2023-05-09 18:04:30.000000 proventosweb-0.7/proventosweb.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-05-09 18:04:30.000000 proventosweb-0.7/proventosweb.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-09 18:04:31.038541 proventosweb-0.7/setup.cfg
--rw-rw-rw-   0        0        0      516 2023-05-09 18:03:32.000000 proventosweb-0.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-18 18:55:15.135430 proventosweb-0.70/
+-rw-rw-rw-   0        0        0      315 2023-05-18 18:55:15.135430 proventosweb-0.70/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-18 18:55:15.103105 proventosweb-0.70/proventosweb/
+-rw-rw-rw-   0        0        0       44 2023-05-08 12:50:56.000000 proventosweb-0.70/proventosweb/__init__.py
+-rw-rw-rw-   0        0        0    12842 2023-05-18 18:48:39.000000 proventosweb-0.70/proventosweb/proventosweb.py
+drwxrwxrwx   0        0        0        0 2023-05-18 18:55:15.121372 proventosweb-0.70/proventosweb.egg-info/
+-rw-rw-rw-   0        0        0      315 2023-05-18 18:55:14.000000 proventosweb-0.70/proventosweb.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      276 2023-05-18 18:55:14.000000 proventosweb-0.70/proventosweb.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-18 18:55:14.000000 proventosweb-0.70/proventosweb.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-05-03 22:03:21.000000 proventosweb-0.70/proventosweb.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       35 2023-05-18 18:55:14.000000 proventosweb-0.70/proventosweb.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-05-18 18:55:14.000000 proventosweb-0.70/proventosweb.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-18 18:55:15.135430 proventosweb-0.70/setup.cfg
+-rw-rw-rw-   0        0        0      517 2023-05-18 18:48:57.000000 proventosweb-0.70/setup.py
```

### Comparing `proventosweb-0.7/proventosweb/proventosweb.py` & `proventosweb-0.70/proventosweb/proventosweb.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 import pandas as pd
-import datetime as dt
 import json
 import requests
 from bs4 import BeautifulSoup
 import numpy as np
-import re
 import time
 
+
 def percent_str_to_float(percent_str):
     decimal_str = percent_str.replace(',', '.')
     number_str = decimal_str.strip('%')
     number = float(number_str) / 100.0
     return number
 
+
 def tratamento(prov, dob, boni, sub):
     dfp = None
     dfb = None
     dfbo = None
     dfs = None
     if prov is not None and not prov.empty:
         prov['Executado'] = prov['Pagamento']
@@ -27,265 +27,272 @@
         dob['Quantia To'] = dob['Quantia To'].astype(float)
         dob['Valor'] = dob.apply(lambda row: row['Quantia From'] if row['Quantia To'] == 1 else row['Quantia To'],
                                  axis=1)
         dfb = dob.loc[:, ['Tipo', 'Data COM', 'Executado', 'Valor']]
 
     if boni is not None and not boni.empty:
         boni['Executado'] = boni['Data de incorporação']
-        boni['Proporção'] = boni['Proporção'].apply(lambda x: float(x.replace(',', '.'))) / 100
-        boni['Valor'] = boni['Valor base'].apply(lambda x: float(x.replace(',', '.')))
+        boni['Valor'] = boni['Valor Base']
         dfbo = boni.loc[:, ['Data COM', 'Executado', 'Valor', 'Proporção']]
         dfbo['Tipo'] = 'Bonificação'
 
     if sub is not None and not sub.empty:
         sub['Quantia'] = sub['Valor Base']
-        sub['Quantia'] = sub['Quantia'].str.replace('R$ ', '', regex=False).str.replace(',', '.', regex=False).astype(
-            float)
         sub['Valor'] = sub['Percentual']
-        sub['Valor'] = sub['Valor'].apply(percent_str_to_float)
-        sub['Executado'] = ''
-        for i in range(len(sub)):
-            try:
-                if sub.loc[i, 'Negociação'].str.split(' a ').str[1] != '31/12/9999':
-                    sub.loc[i, 'Executado'] = sub.loc[i, 'Negociação'].str.split(' a ').str[1]
-                elif sub.loc[i, 'Negociação'].str.split(' a ').str[0] != '31/12/9999':
-                    sub.loc[i, 'Executado'] = sub.loc[i, 'Negociação'].str.split(' a ').str[0]
-                else:
-                    sub.loc[i, 'Executado'] = sub.loc[i, 'Data COM']
-            except:
-                sub.loc[i, 'Executado'] = None
+        sub['Executado'] = sub['Negociação']
         dfs = sub.loc[:, ['Data COM', 'Executado', 'Valor', 'Quantia']]
         dfs['Tipo'] = 'Subscrição'
     dfcons = pd.DataFrame(columns=['Tipo', 'Data COM', 'Executado', 'Valor', 'Valor Original', 'Quantia', 'Proporção'])
     if dfp is None and dfb is None and dfbo is None and dfs is None:
         dfcons = None
     else:
         dfcons = pd.concat([dfp, dfb, dfbo, dfs], ignore_index=True)
         dfcons['Data COM'] = pd.to_datetime(dfcons['Data COM'], dayfirst=True).dt.date
         dfcons['Executado'] = dfcons['Executado'].replace('-', None)
         dfcons['Executado'] = pd.to_datetime(dfcons['Executado'], dayfirst=True).dt.date
         if sub is not None and not sub.empty:
             dfcons['Quantia'] = dfcons['Quantia'].replace({np.nan: None})
-            dfcons['Quantia'] = dfcons['Quantia'].replace({pd.NA: None})
         if prov is not None and not prov.empty:
             dfcons['Valor Original'] = dfcons['Valor Original'].replace({pd.NA: None})
-            dfcons['Valor Original'] = dfcons['Valor Original'].replace({np.nan: None})
         if boni is not None and not prov.empty:
             dfcons['Proporção'] = dfcons['Proporção'].replace({pd.NA: None})
-            dfcons['Proporção'] = dfcons['Proporção'].replace({np.nan: None})
         dfcons.sort_values(by=['Tipo', 'Data COM'])
     return dfcons
 
 
-def eventos(acao):
-    acao = acao.upper()
-    tipos = ['acoes', 'bdrs', 'fundos-imobiliarios', 'fiinfras', 'fiagros', 'etfs']
-    t = 0
-    dfin = None
-    for tipo in tipos:
-        url = 'https://statusinvest.com.br/' + tipo + '/' + acao
-        headers = {
-            'User-Agent': 'Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/58.0.3029.110 Safari/537.36'}
-        resposta = requests.get(url, headers=headers)
-        amostra = resposta.text
-        soup1 = BeautifulSoup(amostra, 'html.parser')
-        if soup1.find('title').text != 'OPS. . .Não encontramos o que você está procurando | Status Invest':
-            soup = soup1
-            t = 1
-            tipo2 = tipo
-
-    if t == 1 and tipo2 != 'etfs':
-        # Proventos
-        value = soup.find('input', {'id': 'results'}).get('value')
-        if value == '[]':
-            print(acao + ' sem dividendos')
-            df = None
-        else:
-            data = json.loads(value)
-            try:
-                df = pd.DataFrame(data)
-                data = json.loads(value)
-                df = df.loc[:, ['et', 'ed', 'pd', 'ov', 'v']]
-                df = df.rename(
-                    columns={'et': 'Tipo', 'ed': 'Data COM', 'pd': 'Pagamento', 'v': 'Valor', 'ov': 'Valor Original'})
-            except:
-                print(f"Erro desconhecido na ação {acao}")
-
-        # Desdobramento ou Grupamento
-        a = soup.find('div', class_='white')
-        b = a.find('div', class_='pt-5')
-        if b != None:
-            c = b.find('div', class_='card-body')
-            texto = c.text.strip()
-            if texto != 'NÃO HÁ DESDOBRAMENTO OU GRUPAMENTO':
-                dobs = dobramento(texto)
-            else:
-                dobs = None
-        else:
-            dobs = None
-        # Bonificação
-        b1 = a.find('div', class_='card p-2 p-xs-3')
-        if b1 != None:
-            c1 = b1.find('div', class_='card-body')
-            texto1 = c1.text.strip()
-            if texto1 != "NÃO HÁ BONIFICAÇÃO":
-                bons = bonificacao(texto1)
-                if bons['Ativo emitido'].unique() != acao:
-                    print('Ativo diferente emitido')
-            else:
-                bons = None
-        else:
-            bons = None
-        # Subscrição
-        a2 = soup.find_all('div', class_='pt-5')[2]
-        b2 = a2.find_all('strong')
-        if len(b2) > 0:
-            subs = subscricao(b2)
-        else:
-            subs = None
-        dfin = tratamento(df, dobs, bons, subs)
-        if dfin is not None:
-            dfin['Ativo'] = acao
-    return dfin
-
-
 def dobramento(strings):
-    pattern = r'(Grupamento|Desdobramento)[\s\S]*?Data do anúncio\n([\d/]+)[\s\S]*?Data COM\n([\d/]+)[\s\S]*?Fator\n([\d,]+) para ([\d,]+)'
-    tipos = []
-    datas_announced = []
-    datas_com = []
-    quantias_from = []
-    quantias_to = []
-    for s in [strings]:
-        matches = re.findall(pattern, s)
-        for match in matches:
-            tipos.append(match[0])
-            datas_announced.append(match[1])
-            datas_com.append(match[2])
-            quantias_from.append(match[4].replace(',', '.'))
-            quantias_to.append(match[3].replace(',', '.'))
-    df = pd.DataFrame({
-        'Tipo': tipos,
-        'Data Anuncio': datas_announced,
-        'Data COM': datas_com,
-        'Quantia From': quantias_from,
-        'Quantia To': quantias_to
-    })
+    data = []
+    for string in strings:
+        txt = string.text
+        lines = txt.split('\n')
+        tipo = lines[3].strip()
+        data_anuncio = lines[8].strip()
+        data_com = lines[12].strip()
+        fator_line = lines[16].strip()
+        quantia_values = fator_line.split(' ')
+        quantia_from = float(quantia_values[0].replace(',', '.'))
+        quantia_to = float(quantia_values[2].replace(',', '.'))
+        data.append([tipo, data_anuncio, data_com, quantia_from, quantia_to])
+    df = pd.DataFrame(data, columns=['Tipo', 'Data Anuncio', 'Data COM', 'Quantia From', 'Quantia To'])
     return df
 
 
 def bonificacao(texto):
-    records = re.split(r'\n{2,}Data do anúncio', texto)
-    if records and not records[0].strip():
-        records.pop(0)
-    data = []
-    for record in records:
-        record = re.sub(r'\n{2,}', '\n', record)
-        record = 'Data do anúncio' + record
-        date_anuncio = re.search(r'Data do anúncio\n([\d/]+)', record)
-        date_com = re.search(r'Data com\n([\d/]+)', record)
-        date_ex = re.search(r'Data ex\n([\d/]+)', record)
-        date_incorporacao = re.search(r'Data de incorporação\n([\d/]+)', record)
-        ativo = re.search(r'Ativo emitido\n([\w]+)', record)
-        valor_base = re.search(r'Valor base\nR\$ ([\d,]+)', record)
-        proporcao = re.search(r'Proporção\n([\d,]+)%', record)
-        row = {
-            'Data do anúncio': date_anuncio.group(1) if date_anuncio else None,
-            'Data COM': date_com.group(1) if date_com else None,
-            'Data EX': date_ex.group(1) if date_ex else None,
-            'Data de incorporação': date_incorporacao.group(1) if date_incorporacao else None,
-            'Ativo emitido': ativo.group(1) if ativo else None,
-            'Valor base': valor_base.group(1) if valor_base else None,
-            'Proporção': proporcao.group(1) if proporcao else None,
+    dfs = []  # List to store individual DataFrames
+
+    for string in texto:
+        txt = string.text
+        lines = txt.split('\n')
+
+        tipo = "Bonificação"  # Fixed value
+        data_anuncio = lines[lines.index('Data do anúncio') + 1].strip()
+        data_com = lines[lines.index('Data com') + 1].strip()
+        data_ex = lines[lines.index('Data ex') + 1].strip()
+        data_incorporacao = lines[lines.index('Data de incorporação') + 1].strip()
+        ativo_emitido = lines[lines.index('Ativo emitido') + 1].strip()
+
+        valor_base = float(lines[lines.index('Valor base') + 1].replace('R$', '').strip().replace(',', '.'))
+        proporcao = float(lines[lines.index('Proporção') + 1].replace('%', '').strip().replace(',', '.')) / 100
+
+        data = {
+            'Tipo': [tipo],
+            'Data do anúncio': [data_anuncio],
+            'Data COM': [data_com],
+            'Data EX': [data_ex],
+            'Data de incorporação': [data_incorporacao],
+            'Ativo Emitido': [ativo_emitido],
+            'Valor Base': [valor_base],
+            'Proporção': [proporcao]
         }
-        data.append(row)
-    df = pd.DataFrame(data)
-    df = df[
-        ['Data do anúncio', 'Data COM', 'Data EX', 'Data de incorporação', 'Ativo emitido', 'Valor base', 'Proporção']]
-    return df
 
+        df = pd.DataFrame(data)
+        dfs.append(df)
+
+    df_concat = pd.concat(dfs, ignore_index=True)
+    df_concat = df_concat[
+        ['Data do anúncio', 'Data COM', 'Data EX', 'Data de incorporação', 'Ativo Emitido', 'Valor Base', 'Proporção']]
+    return df_concat
+
+
+def subscricao(texto):
+    dfs = []  # List to store individual DataFrames
+
+    for string in texto:
+        txt = string.text
+        lines = txt.split('\n')
+
+        data_anuncio = lines[lines.index('Anúncio') + 1].strip()
+        data_com = lines[lines.index('DATA COM') + 1].strip()
+        fim_subscricao = lines[lines.index('Fim de subscrição') + 1].strip()
+        incorporacao = lines[lines.index('Incorporação') + 1].strip()
+        negociacao = lines[lines.index('Negociação') + 1].strip().split(' a ')[1]
+        valor_base_str = lines[lines.index('Valor base') + 1].replace('R$', '').strip().replace('.', '')
+        valor_base = float(valor_base_str.replace(',', '.'))
+        percentual = float(lines[lines.index('Percentual') + 1].replace('%', '').strip().replace(',', '.')) / 100
+        ativo = lines[lines.index('Ativo emitido') + 1].strip()
+
+        data = {
+            'Data Anuncio': [data_anuncio],
+            'Data COM': [data_com],
+            'Fim Subscrição': [fim_subscricao],
+            'Incorporação': [incorporacao],
+            'Ativo': [ativo],
+            'Negociação': [negociacao],
+            'Valor Base': [valor_base],
+            'Percentual': [percentual]
+        }
 
-def subscricao(b):
-    anuncio = []
-    fimd = []
-    datacom = []
-    incop = []
-    negoc = []
-    valb = []
-    perc = []
-    atv = []
-    for j in range(int(len(b) / 8)):
-        i = j * 8
-        anuncio.append(b[i].text.strip())
-        fimd.append(b[i + 3].text.strip())
-        datacom.append(b[i + 1].text.strip())
-        incop.append(b[i + 4].text.strip())
-        negoc.append(b[i + 2].text.strip())
-        valb.append(b[i + 5].text.strip())
-        perc.append(b[i + 6].text.strip())
-        atv.append(b[i + 7].text.strip())
-    df = pd.DataFrame({
-        'Data Anuncio': anuncio,
-        'Data COM': datacom,
-        'Fim Subscrição': fimd,
-        'Incorporação': incop,
-        'Ativo': atv,
-        'Negociação': negoc,
-        'Valor Base': valb,
-        'Percentual': perc
-    })
+        df = pd.DataFrame(data)
+        dfs.append(df)
+
+    df_concat = pd.concat(dfs, ignore_index=True)
     return df
 
+
 def provlista(acoes, testtime=0):
+    session = requests.Session()
+    headers = {
+        'User-Agent': 'Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/58.0.3029.110 Safari/537.36'}
+    dfprov = pd.DataFrame(columns=['Ativo', 'Tipo', 'Data COM', 'Executado', 'Valor', 'Valor Original', 'Quantia'])
+    cortes = [0.25, 0.5, 0.75, 1]
     if testtime == 1:
-        import time
-        dfprov = pd.DataFrame(columns=['Ativo', 'Tipo', 'Data COM', 'Executado', 'Valor', 'Valor Original', 'Quantia'])
-        cortes = [0.25,0.5,0.75,1]
-        print('Buscando proventos de '+str(len(acoes))+' ações!')
+        print('Buscando proventos de ' + str(len(acoes)) + ' ações!')
         start_time = time.time()
         longest_atv = None
         longest_time = 0
         j = 0
         for i, atv in enumerate(acoes):
-            if i/len(acoes)>cortes[j]:
-                print('Já foi '+str(cortes[j]*100)+"% das ações!")
-                j = j+1
-            print(f'Processando {atv} ({i+1}/{len(acoes)})...')
+            if i / len(acoes) >= cortes[j]:
+                print('Já foi ' + str(cortes[j] * 100) + "% das ações!")
+                j = j + 1
+            print(f'Processando {atv} ({i + 1}/{len(acoes)})...')
             atv_start_time = time.time()
-            dfnovo = eventos(atv)
+            dfnovo = eventos(atv, session, headers)
             atv_time = time.time() - atv_start_time
             if atv_time > longest_time:
                 longest_atv = atv
                 longest_time = atv_time
             if dfnovo is not None:
-                dfprov = pd.concat([dfprov,dfnovo])
+                dfprov = pd.concat([dfprov, dfnovo])
         if 'Valor Original' in dfprov.columns:
             dfprov['Valor Original'] = dfprov['Valor Original'].replace({pd.NA: None})
         if 'Quantia' in dfprov.columns:
             dfprov['Quantia'] = dfprov['Quantia'].replace({np.nan: None})
         if 'Proporção' in dfprov.columns:
             dfprov['Proporção'] = dfprov['Proporção'].replace({pd.NA: None})
         print('Acabou!')
         total_time = time.time() - start_time
         print(f'Tempo total: {total_time:.2f} segundos')
-        print(f'Média por ativo: {(total_time/len(acoes)):.2f} segundos')
+        print(f'Média por ativo: {(total_time / len(acoes)):.2f} segundos')
         print(f'Tempo máximo: {longest_atv} ({longest_time:.2f} segundos)')
+    elif testtime == 2:
+        for i in range(len(acoes)):
+            atv = acoes[i]
+            dfnovo = eventos(atv, session, headers)
+            if dfnovo is not None:
+                dfprov = pd.concat([dfprov, dfnovo])
+        if 'Valor Original' in dfprov.columns:
+            dfprov['Valor Original'] = dfprov['Valor Original'].replace({pd.NA: None})
+        if 'Quantia' in dfprov.columns:
+            dfprov['Quantia'] = dfprov['Quantia'].replace({np.nan: None})
+        if 'Proporção' in dfprov.columns:
+            dfprov['Proporção'] = dfprov['Proporção'].replace({pd.NA: None})
     else:
-        dfprov = pd.DataFrame(columns=['Ativo', 'Tipo', 'Data COM', 'Executado', 'Valor', 'Valor Original', 'Quantia'])
-        cortes =[0.25,0.5,0.75]
-        print('Buscando proventos de '+str(len(acoes))+' ações!')
+        print('Buscando proventos de ' + str(len(acoes)) + ' ações!')
         j = 0
         for i in range(len(acoes)):
-            if i/len(acoes)>cortes[j]:
-                print('Já foi '+str(cortes[j]*100)+"% das ações!")
+            if i / len(acoes) >= cortes[j]:
+                print('Já foi ' + str(cortes[j] * 100) + "% das ações!")
+                j += 1
             atv = acoes[i]
-            dfnovo = eventos(atv)
+            dfnovo = eventos(atv, session, headers)
             if dfnovo is not None:
-                dfprov = pd.concat([dfprov,dfnovo])
+                dfprov = pd.concat([dfprov, dfnovo])
         if 'Valor Original' in dfprov.columns:
             dfprov['Valor Original'] = dfprov['Valor Original'].replace({pd.NA: None})
         if 'Quantia' in dfprov.columns:
             dfprov['Quantia'] = dfprov['Quantia'].replace({np.nan: None})
         if 'Proporção' in dfprov.columns:
             dfprov['Proporção'] = dfprov['Proporção'].replace({pd.NA: None})
         print('Acabou!')
     return dfprov
+
+
+def procurandotipo(acao, tempo, session, headers, tipos):
+    tipo2 = None
+    soup = None
+    for tipo in tipos:
+        try:
+            url = 'https://statusinvest.com.br/' + tipo + '/' + acao
+            resposta = session.get(url, headers=headers, timeout=tempo)
+            if resposta.status_code == 200:
+                amostra = resposta.text
+                soup1 = BeautifulSoup(amostra, 'html.parser')
+                if soup1.find('title').text != 'OPS. . .Não encontramos o que você está procurando | Status Invest':
+                    soup = soup1
+                    tipo2 = tipo
+                    break
+        except requests.exceptions.RequestException:
+            continue
+    return soup, tipo2
+
+
+def eventos(acao, session=0, headers=0):
+    acao = acao.upper()
+    tempos = [x / 10 for x in range(3, 10)]
+    if acao[-2:] == '34':
+        tipos = ['bdrs', 'acoes', 'fundos-imobiliarios', 'fiinfras', 'fiagros', 'etfs']
+    elif acao[-2:] == '11':
+        tipos = ['fundos-imobiliarios', 'acoes', 'fiinfras', 'fiagros', 'etfs', 'bdrs']
+    else:
+        tipos = ['acoes', 'fundos-imobiliarios', 'fiinfras', 'fiagros', 'etfs', 'bdrs']
+    if session == 0:
+        headers = {
+            'User-Agent': 'Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/58.0.3029.110 Safari/537.36'}
+        session = requests.Session()
+    for tempo in tempos:
+        soup, tipo2 = procurandotipo(acao, tempo, session, headers, tipos)
+        if soup is not None:
+            break
+    dfin = None
+    if soup is None:
+        print("Tipo não encontrado")
+    else:
+        value = soup.find('input', {'id': 'results'}).get('value')
+        if value == '[]':
+            print(acao + ' sem dividendos')
+            df = None
+        else:
+            data = json.loads(value)
+            try:
+                df = pd.DataFrame(data)
+                data = json.loads(value)
+                df = df.loc[:, ['et', 'ed', 'pd', 'ov', 'v']]
+                df = df.rename(
+                    columns={'et': 'Tipo', 'ed': 'Data COM', 'pd': 'Pagamento', 'v': 'Valor', 'ov': 'Valor Original'})
+            except:
+                print(f"Erro desconhecido na ação {acao}")
+        caixas = soup.find_all('div', class_='card p-2 p-xs-3')
+        dobs = None
+        bons = None
+        subs = None
+        for i in range(len(caixas)):
+            texto = caixas[i].find('h3').text
+            insert = caixas[i].find_all('div',
+                                        class_="d-flex justify-between align-items-center flex-wrap flex-md-nowrap")
+            if texto == "DESDOBRAMENTO/GRUPAMENTO":
+                if len(insert) > 0:
+                    dobs = dobramento(insert)
+            elif texto == "BONIFICAÇÃO":
+                if len(insert) > 0:
+                    bons = bonificacao(insert)
+            elif texto == "SUBSCRIÇÃO":
+                A = caixas[i].find_all('div',
+                                       class_="d-flex justify-between align-items-center flex-wrap flex-lg-nowrap")
+                if len(A) > 0:
+                    subs = subscricao(A)
+            else:
+                print(texto)
+        dfin = tratamento(df, dobs, bons, subs)
+        if dfin is not None:
+            dfin['Ativo'] = acao
+    return dfin
```

### Comparing `proventosweb-0.7/setup.py` & `proventosweb-0.70/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup
 
 setup(name='proventosweb',
-      version='0.7',
+      version='0.70',
       description='Uma biblioteca para buscar proventos de ações na plataforma Status Invest',
       url='https://github.com/rafaelpsampaio/proventosweb',
       author='Rafael Sampaio',
       author_email='rafapsampaio@gmail.com',
       packages=['proventosweb'],
       install_requires=[
           'pandas',
```

