# Comparing `tmp/ia_wumpus-0.2.22.tar.gz` & `tmp/ia_wumpus-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ia_wumpus-0.2.22.tar", max compression
+gzip compressed data, was "ia_wumpus-0.3.tar", max compression
```

## Comparing `ia_wumpus-0.2.22.tar` & `ia_wumpus-0.3.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1071 2023-05-06 13:51:13.656383 ia_wumpus-0.2.22/LICENSE
--rw-r--r--   0        0        0     3921 2023-05-14 23:26:43.291386 ia_wumpus-0.2.22/README.md
--rw-r--r--   0        0        0       68 2023-05-15 05:24:04.316474 ia_wumpus-0.2.22/ia_wumpus/__init__.py
--rw-r--r--   0        0        0     5003 2023-05-15 07:10:08.869769 ia_wumpus-0.2.22/ia_wumpus/ambiente.py
--rw-r--r--   0        0        0      477 2023-05-15 07:13:55.134336 ia_wumpus-0.2.22/pyproject.toml
--rw-r--r--   0        0        0     4498 1970-01-01 00:00:00.000000 ia_wumpus-0.2.22/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-05-06 13:51:13.656383 ia_wumpus-0.3/LICENSE
+-rw-r--r--   0        0        0     3921 2023-05-18 15:05:34.982478 ia_wumpus-0.3/README.md
+-rw-r--r--   0        0        0      556 2023-05-18 16:12:01.534500 ia_wumpus-0.3/ia_wumpus/__init__.py
+-rw-r--r--   0        0        0     7172 2023-05-18 16:11:42.806216 ia_wumpus-0.3/ia_wumpus/ambiente.py
+-rw-r--r--   0        0        0      474 2023-05-18 16:12:36.364693 ia_wumpus-0.3/pyproject.toml
+-rw-r--r--   0        0        0     4495 1970-01-01 00:00:00.000000 ia_wumpus-0.3/PKG-INFO
```

### Comparing `ia_wumpus-0.2.22/LICENSE` & `ia_wumpus-0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ia_wumpus-0.2.22/README.md` & `ia_wumpus-0.3/README.md`

 * *Files identical despite different names*

### Comparing `ia_wumpus-0.2.22/ia_wumpus/ambiente.py` & `ia_wumpus-0.3/ia_wumpus/ambiente.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,55 +1,98 @@
+# -----------------------------------------------------
+# Universidade Federal do Pará
+# Campus Universitário de Tucuruí
+# Faculdade de Engenharia Elétrica
+# -----------------------------------------------------
+#
+# Disciplina: Inteligência Computacional
+# Projeto: O Mundo do Wumpus
+#
+# Professor: Otávio Teixeira
+# Discentes: Ângelo Aragão,
+#            Johanes Martins,
+#            Oséias Farias
+#
+# Data: Maio - 2023
+#  ----------------------------------------------------
+
 import numpy as np
 from random import randint
 import numpy.typing as npt
+from typing import Tuple, Dict
 
 
 class Ambiente:
     """
         Classe que implementa o Ambiente e as percepções
         do Mundo do Wumpus.
     """
     def __init__(self, dimensao_ambiente: int = 3,
                  wumpus: int = 1, ouro: int = 1) -> None:
         self.pocos = dimensao_ambiente
         self.wumpus = wumpus
         self.ouro = ouro
         self.dimensoes = (dimensao_ambiente, dimensao_ambiente)
 
-        self.mundo = np.zeros(self.dimensoes, dtype=int)
-        self.mundo[:] = 0
+        self.__mundo = np.zeros(self.dimensoes, dtype=int)
+        self.__mundo[:] = 0
 
-        # Percepções
+        # Percepções dos Objetos no Ambiente.
         self.percepcoes: dict = {"pocos":  [],
                                  "wumpus": [],
                                  "ouro":   []}
+        # Posições dos Objetos no Ambiente.
+        self.pos_objetos: dict = {"pocos":  [],
+                                  "wumpus": [],
+                                  "ouro":   [],
+                                  "agente": []}
 
         # Posicionando o Agente no ambiente.
         self.__add_pos_agente()
         # Posicionando o(s) Wumpu(s) no ambiente.
         self.__add_pos_wumpus()
         # Posicionando o(s) Poço(s) no ambiente.
         self.__add_pos_pocos()
         # Posicionando o(s) Ouro(s) no ambiente.
         self.__add_pos_ouro()
         # Menu
         self.__menu()
 
-    def add_pos_obj(self, obj: int) -> npt.NDArray:
+    def atualiza_pos_agente(self, pos_agente: Tuple[int, int]) -> None:
+        """Atualiza a posição do Agente no Ambiente."""
+        self.__mundo[self.pos_objetos["agente"][-1]] = 0
+        print("antes ", self.pos_objetos["agente"][-1])
+        self.pos_objetos["agente"] = [pos_agente]
+        print("depois ", self.pos_objetos["agente"][-1])
+        self.__mundo[self.pos_objetos["agente"][-1]] = 4
+
+    def get_pos_objetos(self) -> Dict:
+        """Obtem as posições dos Objetos no Ambiente."""
+        return self.pos_objetos
+
+    def get_percepcoes(self) -> Dict:
+        """Obtem as percepções dos Objetos no Ambiente."""
+        return self.percepcoes
+
+    def add_pos_obj_map(self, obj: int) -> npt.NDArray:
         """Posiciona os Objetos no Ambiente."""
         self.pos_sort = self.__sortear_pos()
-        if self.mundo[self.pos_sort[0], self.pos_sort[1]] == 0:
-            self.mundo[self.pos_sort[0], self.pos_sort[1]] = obj
+        if self.__mundo[self.pos_sort[0], self.pos_sort[1]] == 0:
+            self.__mundo[self.pos_sort[0], self.pos_sort[1]] = obj
             return self.pos_sort
         elif ((self.pos_sort[0] == 0) and (self.pos_sort[1] == 0)):
-            self.add_pos_obj(obj)
+            self.add_pos_obj_map(obj)
         else:
-            self.add_pos_obj(obj)
+            self.add_pos_obj_map(obj)
         return self.pos_sort
 
+    def salvar_pos_objetos(self, objeto: str, pos_objeto) -> None:
+        """Armazena as posições dos Objetos em um dicionário Python."""
+        self.pos_objetos[objeto].append(pos_objeto)
+
     def __sortear_pos(self) -> npt.NDArray:
         """Sortea as posições dos Objetos no Ambiente."""
         x = randint(0, self.dimensoes[0]-1)
         y = randint(0, self.dimensoes[0]-1)
         return np.array([x, y])
 
     def __add_percepcoes_obj(self, objeto: str, pos: npt.NDArray) -> None:
@@ -69,61 +112,71 @@
         elif (pos[1] > 0) and (pos[1] < (self.dimensoes[0] - 1)):
             self.percepcoes[objeto].append((pos[1] + 1, pos[0]))
             self.percepcoes[objeto].append((pos[1] - 1, pos[0]))
 
     def __add_pos_wumpus(self) -> None:
         """Posicionando os Wumpo(s) no Ambiente."""
         for i in range(self.wumpus):
-            pos_wumpus = self.add_pos_obj(1)
+            pos_wumpus = self.add_pos_obj_map(1)
+            self.salvar_pos_objetos(objeto="wumpus", pos_objeto=pos_wumpus)
             self.__add_percepcoes_obj(objeto="wumpus", pos=pos_wumpus)
             # print(f"Wumpus pos: {pos_wumpus}")
 
     def __add_pos_pocos(self) -> None:
         """Posicionando os Poços no Ambiente."""
         for i in range(self.pocos):
-            pos_poco = self.add_pos_obj(2)
+            pos_poco = self.add_pos_obj_map(2)
+            self.salvar_pos_objetos(objeto="pocos", pos_objeto=pos_poco)
             self.__add_percepcoes_obj(objeto="pocos", pos=pos_poco)
             # print(f"Poço pos: {pos_poco}")
 
     def __add_pos_ouro(self) -> None:
         """Posicionando o(s) Ouro(s) no Ambiente."""
         for i in range(self.ouro):
-            pos_ouro = self.add_pos_obj(3)
+            pos_ouro = self.add_pos_obj_map(3)
+            self.salvar_pos_objetos(objeto="ouro", pos_objeto=pos_ouro)
             self.percepcoes["ouro"].append((pos_ouro[1], pos_ouro[0]))
             # print(f"Ouro pos: {pos_ouro}")
 
     def __add_pos_agente(self) -> None:
         """Posicionando o(s) Agente(s) no Ambiente."""
-        self.mundo[0, 0] = 4
+        self.__mundo[(0, 0)] = 4
+        self.salvar_pos_objetos(objeto="agente", pos_objeto=((0, 0)))
 
     @classmethod
     def __menu(self) -> None:
         """Menu com a descrições dos Objetos."""
         print("\n====== Menu - Mundo do Wumpus ======")
         print("\t+ 1 - Wumpus")
         print("\t+ 2 - Poços")
         print("\t+ 3 - Ouro")
         print("\t+ 4 - Agente")
         print("====================================")
 
     def infos_ambiente(self) -> None:
         """Exibe a dimensão do mundo do Wumpus."""
-        print(f"\nTamanho do Ambiente: {self.mundo.shape}")
+        print(f"\nTamanho do Ambiente: {self.__mundo.shape}")
 
     def mostrar_ambiente(self) -> None:
         """Exibe o Mundo do Wumpus com os objetos em suas posições."""
-        print(f"\nMundo do Wumpus:\n{self.mundo}")
+        print(f"\nMundo do Wumpus:\n{self.__mundo}")
 
     def mostrar_percepcoes(self):
         """Exibe o dicionário com as posições das percepções."""
         print("\n======== Posições das Percepções - Mundo do Wumpus ========")
         print(f"\tPos - Percepção do Wumpus:\n\t{self.percepcoes['wumpus']}\n")
         print(f"\tPos - Percepção do Poços:\n\t{self.percepcoes['pocos']}\n")
         print(f"\tPos - Percepção do Ouro:\n\t{self.percepcoes['ouro']}")
         print("============================================================\n")
 
 
 if __name__ == "__main__":
-    amb = Ambiente(dimensao_ambiente=3)
+    amb = Ambiente(dimensao_ambiente=5)
     # amb.infos_ambiente()
     amb.mostrar_ambiente()
-    amb.mostrar_percepcoes()
+    # amb.mostrar_percepcoes()
+    amb.atualiza_pos_agente((1, 1))
+    amb.mostrar_ambiente()
+    amb.atualiza_pos_agente((2, 2))
+    amb.mostrar_ambiente()
+    amb.atualiza_pos_agente((3, 3))
+    amb.mostrar_ambiente()
```

### Comparing `ia_wumpus-0.2.22/PKG-INFO` & `ia_wumpus-0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ia-wumpus
-Version: 0.2.22
+Version: 0.3
 Summary: Projeto O Mundo do Wumpus - Anbiente para estudo da disciplina de Inteligencia Computacional.
 Author: Oseiasdfarias
 Author-email: oseias.dfarias@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

