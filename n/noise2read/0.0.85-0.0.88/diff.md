# Comparing `tmp/noise2read-0.0.85.tar.gz` & `tmp/noise2read-0.0.88.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "noise2read-0.0.85.tar", last modified: Wed May 17 10:42:43 2023, max compression
+gzip compressed data, was "noise2read-0.0.88.tar", last modified: Thu May 18 03:37:01 2023, max compression
```

## Comparing `noise2read-0.0.85.tar` & `noise2read-0.0.88.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 pping    (55472) Research  (5010)        0 2023-05-17 10:42:43.756609 noise2read-0.0.85/
--rw-r--r--   0 pping    (55472) Research  (5010)     1068 2023-04-20 03:30:20.000000 noise2read-0.0.85/LICENSE
--rw-r--r--   0 pping    (55472) Research  (5010)     5951 2023-05-17 10:42:43.758719 noise2read-0.0.85/PKG-INFO
--rw-r--r--   0 pping    (55472) Research  (5010)     5531 2023-05-13 12:21:26.000000 noise2read-0.0.85/README.rst
--rw-r--r--   0 pping    (55472) Research  (5010)       90 2023-04-20 03:30:20.000000 noise2read-0.0.85/pyproject.toml
--rw-r--r--   0 pping    (55472) Research  (5010)      999 2023-05-17 10:42:43.762772 noise2read-0.0.85/setup.cfg
-drwxr-xr-x   0 pping    (55472) Research  (5010)        0 2023-05-17 10:42:43.609934 noise2read-0.0.85/src/
-drwxr-xr-x   0 pping    (55472) Research  (5010)        0 2023-05-17 10:42:43.701669 noise2read-0.0.85/src/noise2read/
--rw-r--r--   0 pping    (55472) Research  (5010)      182 2023-05-17 10:40:53.000000 noise2read-0.0.85/src/noise2read/__init__.py
--rw-r--r--   0 pping    (55472) Research  (5010)    13443 2023-05-16 08:27:41.000000 noise2read-0.0.85/src/noise2read/classifier.py
--rw-r--r--   0 pping    (55472) Research  (5010)    17130 2023-05-17 06:03:22.000000 noise2read-0.0.85/src/noise2read/config.py
--rw-r--r--   0 pping    (55472) Research  (5010)     2701 2023-04-20 03:30:20.000000 noise2read-0.0.85/src/noise2read/coverage.py
--rw-r--r--   0 pping    (55472) Research  (5010)    70175 2023-04-20 03:30:20.000000 noise2read-0.0.85/src/noise2read/data_analysis.py
--rw-r--r--   0 pping    (55472) Research  (5010)    49753 2023-05-17 10:38:46.000000 noise2read-0.0.85/src/noise2read/data_generation.py
--rw-r--r--   0 pping    (55472) Research  (5010)    11534 2023-05-17 00:24:07.000000 noise2read-0.0.85/src/noise2read/data_preprocessing.py
--rw-r--r--   0 pping    (55472) Research  (5010)    30052 2023-05-14 01:00:24.000000 noise2read-0.0.85/src/noise2read/encoding.py
--rw-r--r--   0 pping    (55472) Research  (5010)    30699 2023-04-20 03:30:20.000000 noise2read-0.0.85/src/noise2read/error_orrection.py
--rw-r--r--   0 pping    (55472) Research  (5010)    16773 2023-04-20 03:30:20.000000 noise2read-0.0.85/src/noise2read/isolates_correction.py
--rw-r--r--   0 pping    (55472) Research  (5010)    26351 2023-05-16 13:42:25.000000 noise2read-0.0.85/src/noise2read/noise2read.py
--rw-r--r--   0 pping    (55472) Research  (5010)    34363 2023-05-17 09:58:46.000000 noise2read-0.0.85/src/noise2read/reads2vectors.py
--rw-r--r--   0 pping    (55472) Research  (5010)    18547 2023-05-17 00:19:59.000000 noise2read-0.0.85/src/noise2read/simulation.py
--rw-r--r--   0 pping    (55472) Research  (5010)     3475 2023-04-20 03:30:20.000000 noise2read-0.0.85/src/noise2read/umitest.py
--rw-r--r--   0 pping    (55472) Research  (5010)    15905 2023-04-20 03:30:20.000000 noise2read-0.0.85/src/noise2read/utils.py
-drwxr-xr-x   0 pping    (55472) Research  (5010)        0 2023-05-17 10:42:43.735936 noise2read-0.0.85/src/noise2read.egg-info/
--rw-r--r--   0 pping    (55472) Research  (5010)     5951 2023-05-17 10:42:43.000000 noise2read-0.0.85/src/noise2read.egg-info/PKG-INFO
--rw-r--r--   0 pping    (55472) Research  (5010)      837 2023-05-17 10:42:43.000000 noise2read-0.0.85/src/noise2read.egg-info/SOURCES.txt
--rw-r--r--   0 pping    (55472) Research  (5010)        1 2023-05-17 10:42:43.000000 noise2read-0.0.85/src/noise2read.egg-info/dependency_links.txt
--rw-r--r--   0 pping    (55472) Research  (5010)       58 2023-05-17 10:42:43.000000 noise2read-0.0.85/src/noise2read.egg-info/entry_points.txt
--rw-r--r--   0 pping    (55472) Research  (5010)        1 2023-04-20 03:31:42.000000 noise2read-0.0.85/src/noise2read.egg-info/not-zip-safe
--rw-r--r--   0 pping    (55472) Research  (5010)      217 2023-05-17 10:42:43.000000 noise2read-0.0.85/src/noise2read.egg-info/requires.txt
--rw-r--r--   0 pping    (55472) Research  (5010)       11 2023-05-17 10:42:43.000000 noise2read-0.0.85/src/noise2read.egg-info/top_level.txt
-drwxr-xr-x   0 pping    (55472) Research  (5010)        0 2023-05-17 10:42:43.751609 noise2read-0.0.85/tests/
--rw-r--r--   0 pping    (55472) Research  (5010)     3641 2023-04-20 03:30:20.000000 noise2read-0.0.85/tests/test_data_generation.py
--rw-r--r--   0 pping    (55472) Research  (5010)      985 2023-04-20 03:30:20.000000 noise2read-0.0.85/tests/test_reads2vector.py
--rw-r--r--   0 pping    (55472) Research  (5010)     4216 2023-04-20 03:30:20.000000 noise2read-0.0.85/tests/test_utils.py
+drwxr-xr-x   0 pping    (55472) Research  (5010)        0 2023-05-18 03:37:01.153546 noise2read-0.0.88/
+-rw-r--r--   0 pping    (55472) Research  (5010)     1068 2023-04-20 03:30:20.000000 noise2read-0.0.88/LICENSE
+-rw-r--r--   0 pping    (55472) Research  (5010)     5951 2023-05-18 03:37:01.155513 noise2read-0.0.88/PKG-INFO
+-rw-r--r--   0 pping    (55472) Research  (5010)     5531 2023-05-13 12:21:26.000000 noise2read-0.0.88/README.rst
+-rw-r--r--   0 pping    (55472) Research  (5010)       90 2023-04-20 03:30:20.000000 noise2read-0.0.88/pyproject.toml
+-rw-r--r--   0 pping    (55472) Research  (5010)      999 2023-05-18 03:37:01.160180 noise2read-0.0.88/setup.cfg
+drwxr-xr-x   0 pping    (55472) Research  (5010)        0 2023-05-18 03:37:00.988311 noise2read-0.0.88/src/
+drwxr-xr-x   0 pping    (55472) Research  (5010)        0 2023-05-18 03:37:01.101137 noise2read-0.0.88/src/noise2read/
+-rw-r--r--   0 pping    (55472) Research  (5010)      182 2023-05-18 03:05:29.000000 noise2read-0.0.88/src/noise2read/__init__.py
+-rw-r--r--   0 pping    (55472) Research  (5010)    13443 2023-05-16 08:27:41.000000 noise2read-0.0.88/src/noise2read/classifier.py
+-rw-r--r--   0 pping    (55472) Research  (5010)    17347 2023-05-18 03:36:23.000000 noise2read-0.0.88/src/noise2read/config.py
+-rw-r--r--   0 pping    (55472) Research  (5010)     2701 2023-04-20 03:30:20.000000 noise2read-0.0.88/src/noise2read/coverage.py
+-rw-r--r--   0 pping    (55472) Research  (5010)    70175 2023-04-20 03:30:20.000000 noise2read-0.0.88/src/noise2read/data_analysis.py
+-rw-r--r--   0 pping    (55472) Research  (5010)    56691 2023-05-18 03:23:55.000000 noise2read-0.0.88/src/noise2read/data_generation.py
+-rw-r--r--   0 pping    (55472) Research  (5010)    11534 2023-05-17 00:24:07.000000 noise2read-0.0.88/src/noise2read/data_preprocessing.py
+-rw-r--r--   0 pping    (55472) Research  (5010)    30052 2023-05-14 01:00:24.000000 noise2read-0.0.88/src/noise2read/encoding.py
+-rw-r--r--   0 pping    (55472) Research  (5010)    30699 2023-04-20 03:30:20.000000 noise2read-0.0.88/src/noise2read/error_orrection.py
+-rw-r--r--   0 pping    (55472) Research  (5010)    16773 2023-04-20 03:30:20.000000 noise2read-0.0.88/src/noise2read/isolates_correction.py
+-rw-r--r--   0 pping    (55472) Research  (5010)    26351 2023-05-16 13:42:25.000000 noise2read-0.0.88/src/noise2read/noise2read.py
+-rw-r--r--   0 pping    (55472) Research  (5010)    37237 2023-05-18 02:23:57.000000 noise2read-0.0.88/src/noise2read/reads2vectors.py
+-rw-r--r--   0 pping    (55472) Research  (5010)    18547 2023-05-17 00:19:59.000000 noise2read-0.0.88/src/noise2read/simulation.py
+-rw-r--r--   0 pping    (55472) Research  (5010)     3475 2023-04-20 03:30:20.000000 noise2read-0.0.88/src/noise2read/umitest.py
+-rw-r--r--   0 pping    (55472) Research  (5010)    15905 2023-04-20 03:30:20.000000 noise2read-0.0.88/src/noise2read/utils.py
+drwxr-xr-x   0 pping    (55472) Research  (5010)        0 2023-05-18 03:37:01.132408 noise2read-0.0.88/src/noise2read.egg-info/
+-rw-r--r--   0 pping    (55472) Research  (5010)     5951 2023-05-18 03:37:00.000000 noise2read-0.0.88/src/noise2read.egg-info/PKG-INFO
+-rw-r--r--   0 pping    (55472) Research  (5010)      837 2023-05-18 03:37:00.000000 noise2read-0.0.88/src/noise2read.egg-info/SOURCES.txt
+-rw-r--r--   0 pping    (55472) Research  (5010)        1 2023-05-18 03:37:00.000000 noise2read-0.0.88/src/noise2read.egg-info/dependency_links.txt
+-rw-r--r--   0 pping    (55472) Research  (5010)       58 2023-05-18 03:37:00.000000 noise2read-0.0.88/src/noise2read.egg-info/entry_points.txt
+-rw-r--r--   0 pping    (55472) Research  (5010)        1 2023-04-20 03:31:42.000000 noise2read-0.0.88/src/noise2read.egg-info/not-zip-safe
+-rw-r--r--   0 pping    (55472) Research  (5010)      217 2023-05-18 03:37:00.000000 noise2read-0.0.88/src/noise2read.egg-info/requires.txt
+-rw-r--r--   0 pping    (55472) Research  (5010)       11 2023-05-18 03:37:00.000000 noise2read-0.0.88/src/noise2read.egg-info/top_level.txt
+drwxr-xr-x   0 pping    (55472) Research  (5010)        0 2023-05-18 03:37:01.148531 noise2read-0.0.88/tests/
+-rw-r--r--   0 pping    (55472) Research  (5010)     3641 2023-04-20 03:30:20.000000 noise2read-0.0.88/tests/test_data_generation.py
+-rw-r--r--   0 pping    (55472) Research  (5010)      985 2023-04-20 03:30:20.000000 noise2read-0.0.88/tests/test_reads2vector.py
+-rw-r--r--   0 pping    (55472) Research  (5010)     4216 2023-04-20 03:30:20.000000 noise2read-0.0.88/tests/test_utils.py
```

### Comparing `noise2read-0.0.85/LICENSE` & `noise2read-0.0.88/LICENSE`

 * *Files identical despite different names*

### Comparing `noise2read-0.0.85/PKG-INFO` & `noise2read-0.0.88/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: noise2read
-Version: 0.0.85
+Version: 0.0.88
 Summary: Turn noise to read
 Home-page: https://github.com/Jappy0/noise2read
 Author: Penagyao Ping
 Author-email: ping.pengyao@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `noise2read-0.0.85/README.rst` & `noise2read-0.0.88/README.rst`

 * *Files identical despite different names*

### Comparing `noise2read-0.0.85/setup.cfg` & `noise2read-0.0.88/setup.cfg`

 * *Files identical despite different names*

### Comparing `noise2read-0.0.85/src/noise2read/classifier.py` & `noise2read-0.0.88/src/noise2read/classifier.py`

 * *Files identical despite different names*

### Comparing `noise2read-0.0.85/src/noise2read/config.py` & `noise2read-0.0.88/src/noise2read/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*-
 # @Author: Pengyao Ping
 # @Date:   2023-01-19 10:56:38
 # @Last Modified by:   Pengyao Ping
-# @Last Modified time: 2023-05-17 16:03:22
+# @Last Modified time: 2023-05-18 13:36:23
 
 import configparser
 import os
 
 class Config(object):
     def __init__(self, config_file, logger):
         conf = configparser.ConfigParser()
@@ -31,15 +31,19 @@
             if conf.has_option("SourceInputData", "correct_data"):
                 self.correct_data = conf.get("SourceInputData", "correct_data")
 
             # setting model parameters
             if conf.has_option("General", "num_workers"):
                 self.num_workers = conf.getint("General", "num_workers")
             else:
-                self.num_workers = -1   
+                self.num_workers = -1
+            if conf.has_option("General", "chunks_num"):
+                self.chunks_num = conf.getint("General", "chunks_num")
+            else:   
+                self.chunks_num = 100
             if conf.has_option("General", "verbose"):
                 self.verbose = conf.getboolean("General", "verbose")
             else:
                 self.verbose = False
             if conf.has_option("General", "min_iters"):
                 self.min_iters = conf.getint("General", "min_iters")
             else:
@@ -295,16 +299,17 @@
         if config_file == None:
             # path
             self.result_dir = os.path.join(base_path, 'result/')
             # input
             self.ground_truth_data = None  
             # general
             self.num_workers = -1 
+            self.chunks_num = 100
             self.min_iters = 1000
-            self.verbose = False 
+            self.verbose = True 
             self.iso_change_detail = False     
             self.top_n = 100      
             # self.over_sampling = True 
             self.negative_sample_num = 500000
             self.min_read_len = 30
 
             # GraphSetup
```

### Comparing `noise2read-0.0.85/src/noise2read/coverage.py` & `noise2read-0.0.88/src/noise2read/coverage.py`

 * *Files identical despite different names*

### Comparing `noise2read-0.0.85/src/noise2read/data_analysis.py` & `noise2read-0.0.88/src/noise2read/data_analysis.py`

 * *Files identical despite different names*

### Comparing `noise2read-0.0.85/src/noise2read/data_generation.py` & `noise2read-0.0.88/src/noise2read/data_generation.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*-
 # @Author: Pengyao Ping
 # @Date:   2023-01-16 15:52:44
 # @Last Modified by:   Pengyao Ping
-# @Last Modified time: 2023-05-17 20:38:46
+# @Last Modified time: 2023-05-18 13:23:55
 
 import editdistance
 import networkx as nx
 import os
 import csv
 from tqdm import tqdm
 from noise2read.utils import *
@@ -183,72 +183,122 @@
         Args:
             graph (object): A graph constructed using NetworkX.
             edit_dis (int): set edit distance 1 or 2 to search edges for constructing graph
 
         Returns:
             DataFrame: three or four pandas dataframes saving genuine, error-free records, ambiguous errors or high ambiguous errors
         """
-        subgraphs = [graph.subgraph(c).copy() for c in nx.connected_components(graph)]
+        # subgraphs = [graph.subgraph(c).copy() for c in nx.connected_components(graph)]
         # genuine errors and ambiguous errors
-        genuine_df, ambiguous_df = self.extract_genuine_ambi_errs(subgraphs, edit_dis)
+        # genuine_df, ambiguous_df = self.extract_genuine_ambi_errs(subgraphs, edit_dis)
+        # genuine_df, ambiguous_df = self.extract_genuine_ambi_errs(graph, edit_dis)
         # isolated negative samples
         negative_df = self.extract_isolated_negatives(graph, edit_dis)
-        # high ambiguous errors
+        # ambiguous errors
         if edit_dis == 1 and self.config.high_ambiguous: #
-            high_ambiguous_df = self.extract_high_ambiguous_errs(subgraphs)
+            # high_ambiguous_df = self.extract_high_ambiguous_errs(subgraphs)
+            genuine_df, ambiguous_df, high_ambiguous_df = self.extract_genuine_ambi_errs(graph, edit_dis)
             return genuine_df, negative_df, ambiguous_df, high_ambiguous_df
         else:
+            genuine_df, ambiguous_df = self.extract_genuine_ambi_errs(graph, edit_dis)
             return genuine_df, negative_df, ambiguous_df
 
     def extract_umi_genuine_errs(self):  
         """
         extract genuine errors from umi graph
 
         Returns:
             DataFrame: one pandas dataframe saving genuine errors
         """
         graph, seqs_lens_lst, seqs2id_dict, unique_seqs = self.generate_graph(self.config.input_file, edit_dis=1)
-        subgraphs = [graph.subgraph(c).copy() for c in nx.connected_components(graph)]
-        genuine_df = pd.DataFrame(columns= ["StartRead","StartReadCount", "StartDegree", "ErrorTye","ErrorPosition", "StartErrKmer", "EndErrKmer", "EndRead", "EndReadCount", "EndDegree"])
-        for sub_graph in tqdm(subgraphs, desc=self.logger.info("Extract samples with genuine errors"), miniters=int(len(subgraphs)/self.config.min_iters)):
-            edges_lst = [e for e in sub_graph.edges()]
-            if len(edges_lst) > 0:
-                nodes_lst = list(sub_graph.nodes)
-                for node in nodes_lst:
-                    node_count = sub_graph.nodes[node]['count']
-                    node_degree = sub_graph.degree[node]
-                    line = []
-                    if node_degree >= 1 and node_count <= self.config.max_error_freq and not sub_graph.nodes[node]['flag']: #and node_degree <= 4
-                        node_neis = [n for n in sub_graph.neighbors(node)]
-                        # nei2count = []
-                        nei_degree_count = []
-                        for nei in node_neis:
-                            nei_count = sub_graph.nodes[nei]['count']
-                            nei_degree = sub_graph.degree[nei]
-                            # nei2count.append((nei, nei_count))
-                            tt = nei_degree * 0.5 + nei_count * 0.5
-                            nei_degree_count.append((nei, tt, nei_count))
-                        # nei2count.sort(key=lambda x:x[1], reverse=True)
-                        nei_degree_count.sort(key=lambda x:x[1], reverse=True)
-                        # first_nei, first_nei_count = nei2count[0]
-                        first_nei, tt, first_nei_count = nei_degree_count[0]
-                        first_nei_degree = sub_graph.degree[first_nei]
-                        if first_nei_count > self.config.high_freq_thre:
-                            line = [first_nei, first_nei_count, first_nei_degree, node, node_count, node_degree]
-                            newline = self.err_type_classification(line)
-                            genuine_df.loc[len(genuine_df)] = newline
-                            sub_graph.nodes[node]['flag'] = True
-                    else:
-                        continue   
+        subgraphs = [graph.subgraph(c).copy() for c in nx.connected_components(graph) if len(c) >= 2]
+
+        chunk_size = len(subgraphs) // self.config.chunks_num
+        if chunk_size > 0:
+            groups = [subgraphs[i:i+chunk_size] for i in range(0, len(subgraphs), chunk_size)]
+        else:
+            groups = subgraphs
+
+        # Write each group of subgraphs to separate files
+        gexf_files = []
+        for i, group in enumerate(groups):
+            # Create a new graph for the group of subgraphs
+            group_G = nx.Graph()
+            for subgraph_nodes in group:
+                group_G.add_edges_from(graph.subgraph(subgraph_nodes).edges())
+                # Add node attributes to the new graph
+                for node in subgraph_nodes:
+                    group_G.nodes[node].update(graph.nodes[node])
+            # Generate the file name for the group
+            file_name = self.config.result_dir + f"group_{i}.gexf"
+
+            # Write the group of subgraphs to the file
+            nx.write_gexf(group_G, file_name)
+            gexf_files.append(file_name)
+        
+        del groups, subgraphs, graph
+
+        genuine_lst = []
+        for gexf_file in gexf_files:
+            graph = nx.read_gexf(gexf_file)
+            sub_graphs = [graph.subgraph(c).copy() for c in nx.connected_components(graph)]
+            
+            # Process the subgraphs in parallel
+            pool = Pool(processes=self.config.num_workers)
+            genuine_lsts = pool.starmap(self.extract_umi_genuine_errs_subgraph, [(sub_graph) for sub_graph in sub_graphs])
+            # Close the multiprocessing pool
+            pool.close()
+            pool.join()
+
+            for item1 in genuine_lsts:
+                genuine_lst.extend(item)
+
+            os.remove(gexf_file)
+            del graph, sub_graphs
+
+        genuine_df = pd.DataFrame(genuine_lst, columns=["StartRead","StartReadCount", "StartDegree", "ErrorTye","ErrorPosition", "StartErrKmer", "EndErrKmer", "EndRead", "EndReadCount", "EndDegree"])
+
         if self.config.verbose:
             genuine_csv = os.path.join(self.config.result_dir, "umi_gnuine.csv")
             genuine_df.to_csv(genuine_csv, index=False) 
         return genuine_df
 
-    def extract_genuine_ambi_errs(self, subgraphs, edit_dis):
+    def extract_umi_genuine_errs_subgraph(self, sub_graph): 
+        gen_lst = []
+        nodes_lst = list(sub_graph.nodes)
+        for node in nodes_lst:
+            node_count = sub_graph.nodes[node]['count']
+            node_degree = sub_graph.degree[node]
+            line = []
+            if node_degree >= 1 and node_count <= self.config.max_error_freq and not sub_graph.nodes[node]['flag']: #and node_degree <= 4
+                node_neis = [n for n in sub_graph.neighbors(node)]
+                # nei2count = []
+                nei_degree_count = []
+                for nei in node_neis:
+                    nei_count = sub_graph.nodes[nei]['count']
+                    nei_degree = sub_graph.degree[nei]
+                    # nei2count.append((nei, nei_count))
+                    tt = nei_degree * 0.5 + nei_count * 0.5
+                    nei_degree_count.append((nei, tt, nei_count))
+                # nei2count.sort(key=lambda x:x[1], reverse=True)
+                nei_degree_count.sort(key=lambda x:x[1], reverse=True)
+                # first_nei, first_nei_count = nei2count[0]
+                first_nei, tt, first_nei_count = nei_degree_count[0]
+                first_nei_degree = sub_graph.degree[first_nei]
+                if first_nei_count > self.config.high_freq_thre:
+                    line = [first_nei, first_nei_count, first_nei_degree, node, node_count, node_degree]
+                    newline = self.err_type_classification(line)
+                    # genuine_df.loc[len(genuine_df)] = newline
+                    gen_lst.append(newline)
+                    sub_graph.nodes[node]['flag'] = True
+            else:
+                continue   
+        return gen_lst
+        
+    def extract_genuine_ambi_errs(self, graph, edit_dis):
         """
         extract genuine and ambiguous errors from read graph
 
         Args:
             subgraphs (class): Subgraphs of graph constructed using NetworkX.
             edit_dis (int): set edit distance 1 or 2 to search edges for constructing graph
 
@@ -262,47 +312,112 @@
             ambiguous_csv = self.config.result_dir + "ambiguous1.csv"
         elif edit_dis == 2: #or edit_dis == 3:
             genu_columns = ["StartRead","StartReadCount", "StartDegree", "EndRead", "EndReadCount", "EndDegree"]
             ambiguous_df= pd.DataFrame(columns=["idx", "StartRead", "StartReadCount", "StartDegree", "EndRead", "EndReadCount", "EndDegree"])
             genuine_csv = self.config.result_dir + "genuine2.csv"
             ambiguous_csv = self.config.result_dir + "ambiguous2.csv"  
 
+        subgraphs = [graph.subgraph(c).copy() for c in nx.connected_components(graph) if len(c) >= 2]
+
+        self.logger.info("Extracting genuine and ambiguous errors...")
+
+        # Split subgraphs into groups based on the number of CPUs
+        # groups = [subgraphs[i::self.config.num_workers] for i in range(self.config.num_workers)]
+
+        chunk_size = len(subgraphs) // self.config.chunks_num
+        if chunk_size > 0:
+            groups = [subgraphs[i:i+chunk_size] for i in range(0, len(subgraphs), chunk_size)]
+        else:
+            groups = subgraphs
+
+        # Write each group of subgraphs to separate files
+        gexf_files = []
+        for i, group in enumerate(groups):
+            # Create a new graph for the group of subgraphs
+            group_G = nx.Graph()
+            for subgraph_nodes in group:
+                group_G.add_edges_from(graph.subgraph(subgraph_nodes).edges())
+                # Add node attributes to the new graph
+                for node in subgraph_nodes:
+                    group_G.nodes[node].update(graph.nodes[node])
+            # Generate the file name for the group
+            file_name = self.config.result_dir + f"group_{i}.gexf"
+
+            # Write the group of subgraphs to the file
+            nx.write_gexf(group_G, file_name)
+            gexf_files.append(file_name)
+        
+        del groups, subgraphs, graph
+
+        genuine_lst = []
+        ambiguous_lst = []
+
+        if self.config.high_ambiguous:
+            high_ambiguous_df = pd.DataFrame(columns=["idx", "StartRead", "StartReadCount", "StartDegree", "ErrorTye","ErrorPosition", "StartErrKmer", "EndErrKmer", "EndRead", "EndReadCount", "EndDegree"])    
+            high_ambi_lst = []        
+
+        high_idx = 0
+        for gexf_file in gexf_files:
+            graph = nx.read_gexf(gexf_file)
+            sub_graphs = [graph.subgraph(c).copy() for c in nx.connected_components(graph)]
+            
+            # Process the subgraphs in parallel
+            pool = Pool(processes=self.config.num_workers)
+            results = pool.starmap(self.extract_genuine_ambi_errs_subgraph, [(sub_graph, edit_dis) for sub_graph in sub_graphs])
+            # Close the multiprocessing pool
+            pool.close()
+            pool.join()
+            
+            genuine_lsts, ambiguous_lsts = zip(*results)
+            for item1, item2 in zip(genuine_lsts, ambiguous_lsts):
+                genuine_lst.extend(item1)
+                ambiguous_lst.extend(item2)
+
+            if self.config.high_ambiguous:
+                cur_lst, cur_idx = self.extract_high_ambiguous_errs(sub_graphs, high_idx)
+                high_ambi_lst.extend(cur_lst)
+                high_idx = cur_idx + 1
+            os.remove(gexf_file)
+            del graph, sub_graphs
+        
         # genuine_lst = []
         # ambiguous_lst = []
         # subgraph_num = len(subgraphs)
         # shared_obs = subgraphs, edit_dis
-        
-        self.logger.info("Extracting genuine and ambiguous errors...")
-
-        pool = Pool(processes=self.config.num_workers)
-        # Process the subgraphs in parallel
-        results = [pool.apply_async(self.extract_genuine_ambi_errs_subgraph, (subgraph, edit_dis)) for subgraph in subgraphs]
-        genuine_lst, ambiguous_lst = zip(*results)
-
         # with WorkerPool(self.config.num_workers, shared_objects=shared_obs, start_method='fork') as pool:
         #     for genu_ambi_lst in pool.imap(self.extract_genuine_ambi_errs_subgraph, range(subgraph_num), progress_bar=self.config.verbose):
         #         if genu_ambi_lst[0]:
         #             genuine_lst.extend(genu_ambi_lst[0])
         #             ambiguous_lst.extend(genu_ambi_lst[1])
-        self.logger.info("Done!")                    
 
         genuine_df = pd.DataFrame(genuine_lst, columns=genu_columns)
 
         idx = 0
         for a_item in ambiguous_lst:
             for sub_item in a_item:
                 sub_item.insert(0, idx)
                 ambiguous_df.loc[len(ambiguous_df)] = sub_item
             idx += 1
-                
+
+        if self.config.high_ambiguous: 
+            for item in high_ambi_lst:
+                high_ambiguous_df.loc[len(high_ambiguous_df)] = item
+            
         if self.config.verbose:
             genuine_df.to_csv(genuine_csv, index=False)  
-            ambiguous_df.to_csv(ambiguous_csv, index=False)    
-        return genuine_df, ambiguous_df
-    
+            ambiguous_df.to_csv(ambiguous_csv, index=False) 
+            if self.config.high_ambiguous:   
+                high_ambiguous_csv = self.config.result_dir + "high_ambiguous_1nt.csv"
+                high_ambiguous_df.to_csv(high_ambiguous_csv, index=False)  
+        self.logger.info("Done!")
+        if self.config.high_ambiguous:
+            return genuine_df, ambiguous_df, high_ambiguous_df
+        else:
+            return genuine_df, ambiguous_df
+
     def add_genu_sample(self, shared_obs, i):
         """
         add samples to pd DataFrame
 
         Args:
             item_lst (list): a list containing samples
 
@@ -332,108 +447,103 @@
         for a_item in item_lst:
             for sub_item in a_item:
                 sub_item.insert(0, idx)
                 tmp_df.loc[len(tmp_df)] = sub_item
             idx += 1
         return tmp_df
 
-    def extract_genuine_ambi_errs_subgraph(self, sub_graphs, edit_dis):
+    def extract_genuine_ambi_errs_subgraph(self, sub_graph, edit_dis):
         gen_lst = []
         ambi_lst = []
-        # sub_graphs, edit_dis = shared_obs 
-        # sub_graph = sub_graphs[ii]
-        for sub_graph in sub_graphs:
-            edges_lst = [e for e in sub_graph.edges()]
-            if len(edges_lst) > 0:
-                nodes_lst = list(sub_graph.nodes)
-                for node in nodes_lst:
-                    node_count = sub_graph.nodes[node]['count']
-                    node_degree = sub_graph.degree[node]
-                    if node_count <= self.config.max_error_freq and not sub_graph.nodes[node]['flag']:
-                        node_neis = [n for n in sub_graph.neighbors(node)]
-                        if node_degree == 1:
-                            nei = node_neis[0]
-                            nei_count = sub_graph.nodes[nei]['count']
-                            nei_degree = sub_graph.degree[nei]
-                            # if nei_count >= self.config.high_freq_thre:
-                            if nei_count > self.config.high_freq_thre:
-                                line = [nei, nei_count, nei_degree, node, node_count, node_degree]
-                                if edit_dis == 1:
-                                    newline = self.err_type_classification(line)
-                                    # gen_df.loc[len(gen_df)] = newline
-                                    gen_lst.append(newline)
-                                    del line, newline 
-                                else:
-                                    # gen_df.loc[len(gen_df)] = line 
-                                    gen_lst.append(line)
-                                    del line                                   
-                        # elif node_degree <= self.config.ambiguous_error_node_degree: # comment this line on 13 May 2023
+        nodes_lst = list(sub_graph.nodes)
+        for node in nodes_lst:
+            node_count = sub_graph.nodes[node]['count']
+            node_degree = sub_graph.degree[node]
+            if node_count <= self.config.max_error_freq and not sub_graph.nodes[node]['flag']:
+                node_neis = [n for n in sub_graph.neighbors(node)]
+                if node_degree == 1:
+                    nei = node_neis[0]
+                    nei_count = sub_graph.nodes[nei]['count']
+                    nei_degree = sub_graph.degree[nei]
+                    # if nei_count >= self.config.high_freq_thre:
+                    if nei_count > self.config.high_freq_thre:
+                        line = [nei, nei_count, nei_degree, node, node_count, node_degree]
+                        if edit_dis == 1:
+                            newline = self.err_type_classification(line)
+                            # gen_df.loc[len(gen_df)] = newline
+                            gen_lst.append(newline)
+                            del line, newline 
                         else:
-                            high_num = 0
-                            nei2count = []
-                            for nei in node_neis:
-                                nei_count = sub_graph.nodes[nei]['count']
-                                nei_degree = sub_graph.degree[nei]
-                                # if nei_count >= self.config.high_freq_thre:
-                                if nei_count > self.config.high_freq_thre:
-                                    high_num += 1
-                                    nei2count.append((nei, nei_count))
-                            if high_num == 1:             
-                                nei2count.sort(key=lambda x:x[1], reverse=True)
-                                first_nei, first_nei_count = nei2count[0]
-                                first_nei_degree = sub_graph.degree[first_nei]
-                                # if first_nei_count >= self.config.high_freq_thre:
-                                if first_nei_count > self.config.high_freq_thre:
-                                    line = [first_nei, first_nei_count, first_nei_degree, node, node_count, node_degree]
-                                    if edit_dis == 1:
-                                        newline = self.err_type_classification(line)
-                                        # gen_df.loc[len(gen_df)] = newline
-                                        gen_lst.append(newline)
-                                        del line, newline  
-                                    else:
-                                        # gen_df.loc[len(gen_df)] = line 
-                                        gen_lst.append(line)
-                                        del line
+                            # gen_df.loc[len(gen_df)] = line 
+                            gen_lst.append(line)
+                            del line                                   
+                # elif node_degree <= self.config.ambiguous_error_node_degree: # comment this line on 13 May 2023
+                else:
+                    high_num = 0
+                    nei2count = []
+                    for nei in node_neis:
+                        nei_count = sub_graph.nodes[nei]['count']
+                        nei_degree = sub_graph.degree[nei]
+                        # if nei_count >= self.config.high_freq_thre:
+                        if nei_count > self.config.high_freq_thre:
+                            high_num += 1
+                            nei2count.append((nei, nei_count))
+                    if high_num == 1:             
+                        nei2count.sort(key=lambda x:x[1], reverse=True)
+                        first_nei, first_nei_count = nei2count[0]
+                        first_nei_degree = sub_graph.degree[first_nei]
+                        # if first_nei_count >= self.config.high_freq_thre:
+                        if first_nei_count > self.config.high_freq_thre:
+                            line = [first_nei, first_nei_count, first_nei_degree, node, node_count, node_degree]
+                            if edit_dis == 1:
+                                newline = self.err_type_classification(line)
+                                # gen_df.loc[len(gen_df)] = newline
+                                gen_lst.append(newline)
+                                del line, newline  
                             else:
-                                # ambiguous errors
-                                tmp_lst = []
-                                for cre_nei, cur_nei_count in nei2count:
-                                    # if cur_nei_count >= self.config.high_freq_thre:
-                                    if cur_nei_count > self.config.high_freq_thre:
-                                        cur_nei_degree = sub_graph.degree[nei]
-                                        line = [cre_nei, cur_nei_count, cur_nei_degree, node, node_count, node_degree]
-                                        if edit_dis == 1:
-                                            newline = self.err_type_classification(line)
-                                        else:
-                                            newline = line
-                                        # newline.insert(0, idx)
-                                        # ambi_df.loc[len(ambi_df)] = newline
-                                        tmp_lst.append(newline)
-                                        del newline 
-                                if tmp_lst:
-                                    ambi_lst.append(tmp_lst)  
-                                # idx += 1 
-                        sub_graph.nodes[node]['flag'] = True        
+                                # gen_df.loc[len(gen_df)] = line 
+                                gen_lst.append(line)
+                                del line
                     else:
-                        continue
+                        # ambiguous errors
+                        tmp_lst = []
+                        for cre_nei, cur_nei_count in nei2count:
+                            # if cur_nei_count >= self.config.high_freq_thre:
+                            if cur_nei_count > self.config.high_freq_thre:
+                                cur_nei_degree = sub_graph.degree[nei]
+                                line = [cre_nei, cur_nei_count, cur_nei_degree, node, node_count, node_degree]
+                                if edit_dis == 1:
+                                    newline = self.err_type_classification(line)
+                                else:
+                                    newline = line
+                                # newline.insert(0, idx)
+                                # ambi_df.loc[len(ambi_df)] = newline
+                                tmp_lst.append(newline)
+                                del newline 
+                        if tmp_lst:
+                            ambi_lst.append(tmp_lst)  
+                        # idx += 1 
+                sub_graph.nodes[node]['flag'] = True        
+            else:
+                continue
         return gen_lst, ambi_lst
 
     def data_files(self, edit_dis):
         """
         function to return the results produced by DataGneration class
 
         Args:
             edit_dis (int): set edit distance 1 or 2 to search edges for constructing graph
 
         Returns:
             MultiVariables: MultiVariables for next step error correction
         """
         # 1nt-edit-distance-based graph
-        self.logger.info("-------------------------------------------------------------")
-        self.logger.info("1nt-edit-distance read graph error correction")
+        # self.logger.info("-------------------------------------------------------------")
+        # self.logger.info("1nt-edit-distance read graph error correction")
         graph, seqs_lens_lst, seqs2id_dict, unique_seqs = self.generate_graph(self.config.input_file, edit_dis)
         seq_max_len = max(seqs_lens_lst)
         seq_min_len = min(seqs_lens_lst)
         self.logger.debug(seqs_lens_lst)
         self.logger.debug("Reads Max length: {}".format(seq_max_len))
         self.logger.debug("Reads Min length: {}".format(seq_min_len))
         if edit_dis == 1 and self.config.high_ambiguous:
@@ -558,20 +668,21 @@
             seq = str(item.seq)
             ll = len(seq)
             seq_lens_set.add(ll)
             total_seqs.append(seq)
             seqs2id_dict.setdefault(seq, []).append(str(item.id))
         unique_seqs = set(total_seqs)
 
+        self.logger.info("Constructing " + str(edit_dis) + "nt-edit-distance read graph...")
         graph = nx.Graph()
         read_count = Counter(total_seqs)
         high_freq = []
         low_freq = []
 
-        for read, frequency in tqdm(read_count.items(), desc=self.logger.info("Adding nodes to " + str(edit_dis) + "nt-edit-distance read graph..."), miniters=int(len(read_count)/self.config.min_iters)):
+        for read, frequency in tqdm(read_count.items(), miniters=int(len(read_count)/self.config.min_iters)):
             if not graph.has_node(read):
                 graph.add_node(read, count = frequency, flag=False)  
             # if frequency >= self.config.high_freq_thre:
             if frequency > self.config.high_freq_thre:
                 high_freq.append(read)
             else:
                 low_freq.append(read)
@@ -583,28 +694,29 @@
         ######################################################
         edges_lst = []
         if edit_dis == 1:
             shared_unique_seqs = unique_seqs
         elif edit_dis == 2:
             shared_unique_seqs = low_freq
         
-        self.logger.info("Searching edges for constructing " + str(edit_dis) + "nt-edit-distance read graph...")
+        self.logger.debug("Searching edges for constructing " + str(edit_dis) + "nt-edit-distance read graph...")
         with WorkerPool(self.config.num_workers, shared_objects=shared_unique_seqs, start_method='fork') as pool:
             if edit_dis == 1:
                 for edge_lst in pool.imap(self.real_ed1_seqs, high_freq, progress_bar=self.config.verbose):
                     edges_lst.extend(edge_lst)
             elif edit_dis == 2:
                 for edge_lst in pool.imap(self.real_ed2_seqs, high_freq, progress_bar=self.config.verbose):
                     edges_lst.extend(edge_lst)
 
         if len(edges_lst) > 0:
             self.logger.debug(len(edges_lst))
             self.logger.debug(edges_lst[0])
             graph.add_edges_from(edges_lst)
-        self.logger.info(str(edit_dis) + "nt-edit-distance read graph construction finished.")
+        # self.logger.info(str(edit_dis) + "nt-edit-distance read graph construction done.")
+        self.logger.info("Done!")
         ########################################################
         # save graphs
         if self.config.graph_visualization or self.config.save_graph:
             if edit_dis == 1:
                 subdir = self.config.result_dir + "graph1/"                
             elif edit_dis == 2:
                 subdir = self.config.result_dir + "graph2/"
@@ -684,23 +796,66 @@
         self.logger.info("Constructing the second 1nt-edit-distance based graph for further amplicon sequencing data correction.")
         graph, seq_lens_set, seqs2id_dict, unique_seqs = self.generate_graph(data_set, edit_dis=1)
         self.graph_summary(graph)
         
         subgraphs = [graph.subgraph(c).copy() for c in nx.connected_components(graph)]
         
         amplicon_df = pd.DataFrame(columns=["idx", "StartRead","StartReadCount", "StartDegree", "ErrorTye", "ErrorPosition", "StartErrKmer", "EndErrKmer", "EndRead", "EndReadCount", "EndDegree"])
-        for sub_graph in tqdm(subgraphs, desc=self.logger.info("Extract samples with genuine errors"), miniters=int(len(subgraphs)/self.config.min_iters)):
+        for sub_graph in subgraphs:
             edges_lst = [e for e in sub_graph.edges()]
             if len(edges_lst) > 0:
                 nodes_lst = list(sub_graph.nodes)
                 for node in nodes_lst:
                     # reset node visit status
                     sub_graph.nodes[node]['flag'] = False
-        idx = 0            
-        for sub_graph in tqdm(subgraphs, desc=self.logger.info("Extract samples with genuine errors"), miniters=int(len(subgraphs)/self.config.min_iters)):
+
+        chunk_size = len(subgraphs) // self.config.chunks_num
+        if chunk_size > 0:
+            groups = [subgraphs[i:i+chunk_size] for i in range(0, len(subgraphs), chunk_size)]
+        else:
+            groups = subgraphs
+
+        # Write each group of subgraphs to separate files
+        gexf_files = []
+        for i, group in enumerate(groups):
+            # Create a new graph for the group of subgraphs
+            group_G = nx.Graph()
+            for subgraph_nodes in group:
+                group_G.add_edges_from(graph.subgraph(subgraph_nodes).edges())
+                # Add node attributes to the new graph
+                for node in subgraph_nodes:
+                    group_G.nodes[node].update(graph.nodes[node])
+            # Generate the file name for the group
+            file_name = self.config.result_dir + f"group_{i}.gexf"
+
+            # Write the group of subgraphs to the file
+            nx.write_gexf(group_G, file_name)
+            gexf_files.append(file_name)
+
+        amplicon_lst = []
+        idx = 0
+        for gexf_file in gexf_files:
+            graph = nx.read_gexf(gexf_file)
+            sub_graphs = [graph.subgraph(c).copy() for c in nx.connected_components(graph)]
+            
+            cur_lst, cur_idx = self.extract_amplicon_errs(sub_graphs, idx)
+            amplicon_lst.extend(cur_lst)
+            idx = cur_idx + 1
+            os.remove(gexf_file)
+            del graph, sub_graphs
+
+        for item in amplicon_lst:
+            amplicon_df.loc[len(amplicon_df)] = item
+        if self.config.verbose:
+            amplicon_df.to_csv(self.config.result_dir + "amplicon.csv", index=False)  
+        return amplicon_df
+        
+    def extract_amplicon_errs(self, subgraphs, idx):  
+        amplicon_errs_lst = []     
+        for sub_graph in subgraphs:
             edges_lst = [e for e in sub_graph.edges()]
             if len(edges_lst) > 0:
                 nodes_lst = list(sub_graph.nodes)
                 for node in nodes_lst:
                     node_count = sub_graph.nodes[node]['count']
                     node_degree = sub_graph.degree[node]
                     line = []
@@ -712,24 +867,22 @@
                             nei_count = sub_graph.nodes[nei]['count']
                             nei_degree = sub_graph.degree[nei]
                             if nei_count > amplicon_high_freq:
                                 line = [nei, nei_count, nei_degree, node, node_count, node_degree]
                                 new_line = self.err_type_classification(line) 
                                 new_line.insert(0, idx) 
                                 # writer.writerow(new_line)
-                                amplicon_df.loc[len(amplicon_df)] = new_line
+                                # amplicon_df.loc[len(amplicon_df)] = new_line
+                                amplicon_errs_lst.append(new_line)
                         idx += 1
                         sub_graph.nodes[node]['flag'] = True
                     else:
                         continue     
-        if self.config.verbose:
-            amplicon_csv = self.config.result_dir + "amplicon.csv"
-            amplicon_df.to_csv(amplicon_csv, index=False)                                            
-        return amplicon_df     
-
+        return amplicon_errs_lst
+  
     def draw_graph(self, graph, sub_dir, drawing_graph_num = 50):
         """
         draw subgraphs from edit-distance-based read graph
 
         Args:
             graph (object): A graph constructed using NetworkX.
             sub_dir (str): Directory for saving subgraphs.
@@ -756,51 +909,51 @@
                 i += 1
                 del nodes_num
                 plt.close()
                 if i == drawing_graph_num:
                     break
         return
 
-    def extract_high_ambiguous_errs(self, subgraphs):
+    def extract_high_ambiguous_errs(self, subgraphs, idx):
         """
         extract high ambiguous errors from read graph
 
         Args:
             subgraphs (class): Subgraphs of graph constructed using NetworkX.
 
         Returns:
             DataFrame: One pandas dataframe saving high ambiguous errors
         """
-        high_ambiguous_df = pd.DataFrame(columns=["idx", "StartRead", "StartReadCount", "StartDegree", "ErrorTye","ErrorPosition", "StartErrKmer", "EndErrKmer", "EndRead", "EndReadCount", "EndDegree"])
-        idx = 0
-        for s in tqdm(subgraphs, desc=self.logger.info("Extracting high ambiguous errors from 1nt-edit-distance graph"), miniters=int(len(subgraphs)/self.config.min_iters)):
+        high_ambi_lst = []
+        for s in subgraphs:
             edges_lst = [e for e in s.edges()]
-            if len(edges_lst) > 0:
-                for (a, b) in edges_lst:
-                    a_count = s.nodes[a]['count']
-                    b_count = s.nodes[b]['count']
-                    a_degree = s.degree[a]
-                    b_degree = s.degree[b]
-                    if a_count > self.config.high_freq_thre and b_count > self.config.high_freq_thre: 
-                    # if a_count >= self.config.high_freq_thre and b_count >= self.config.high_freq_thre: # comment this line on 13 May 2023
-                        a2b = [a, a_count, a_degree, b, b_count, b_degree]
-                        new_a2b = self.err_type_classification(a2b) 
-                        new_a2b.insert(0, idx)     
-                        high_ambiguous_df.loc[len(high_ambiguous_df)] = new_a2b 
-                        b2a = [b, b_count, b_degree, a, a_count, a_degree]
-                        new_b2a = self.err_type_classification(b2a)
-                        new_b2a.insert(0, idx)
-                        high_ambiguous_df.loc[len(high_ambiguous_df)] = new_b2a
-                        idx += 1
+            for (a, b) in edges_lst:
+                a_count = s.nodes[a]['count']
+                b_count = s.nodes[b]['count']
+                a_degree = s.degree[a]
+                b_degree = s.degree[b]
+                if a_count > self.config.high_freq_thre and b_count > self.config.high_freq_thre: 
+                    a2b = [a, a_count, a_degree, b, b_count, b_degree]
+                    new_a2b = self.err_type_classification(a2b) 
+                    new_a2b.insert(0, idx)     
+                    high_ambi_lst.append(new_a2b)
+                    # high_ambiguous_df.loc[len(high_ambiguous_df)] = new_a2b 
+                    b2a = [b, b_count, b_degree, a, a_count, a_degree]
+                    new_b2a = self.err_type_classification(b2a)
+                    new_b2a.insert(0, idx)
+                    high_ambi_lst.append(new_b2a)
+                    # high_ambiguous_df.loc[len(high_ambiguous_df)] = new_b2a
+                    idx += 1
             del edges_lst
-        if self.config.verbose:
-            high_ambiguous_csv = self.config.result_dir + "high_ambiguous_1nt.csv"
-            high_ambiguous_df.to_csv(high_ambiguous_csv, index=False)  
-        self.logger.info("Done!")
-        return high_ambiguous_df
+        # if self.config.verbose:
+        #     high_ambiguous_csv = self.config.result_dir + "high_ambiguous_1nt.csv"
+        #     high_ambiguous_df.to_csv(high_ambiguous_csv, index=False)  
+        # self.logger.info("Done!")
+        # return high_ambiguous_df
+        return high_ambi_lst, idx
 
 
 '''
     def extract_genuine_ambi_errs(self, subgraphs, edit_dis):
         """
         extract genuine and ambiguous errors from read graph
 
@@ -965,8 +1118,48 @@
                             if tmp_lst:
                                 ambi_lst.append(tmp_lst)  
                             # idx += 1 
                     sub_graph.nodes[node]['flag'] = True        
                 else:
                     continue
         return [gen_lst, ambi_lst]
+'''
+
+'''
+    def extract_high_ambiguous_errs(self, subgraphs):
+        """
+        extract high ambiguous errors from read graph
+
+        Args:
+            subgraphs (class): Subgraphs of graph constructed using NetworkX.
+
+        Returns:
+            DataFrame: One pandas dataframe saving high ambiguous errors
+        """
+        high_ambiguous_df = pd.DataFrame(columns=["idx", "StartRead", "StartReadCount", "StartDegree", "ErrorTye","ErrorPosition", "StartErrKmer", "EndErrKmer", "EndRead", "EndReadCount", "EndDegree"])
+        idx = 0
+        for s in tqdm(subgraphs, desc=self.logger.info("Extracting high ambiguous errors from 1nt-edit-distance graph"), miniters=int(len(subgraphs)/self.config.min_iters)):
+            edges_lst = [e for e in s.edges()]
+            if len(edges_lst) > 0:
+                for (a, b) in edges_lst:
+                    a_count = s.nodes[a]['count']
+                    b_count = s.nodes[b]['count']
+                    a_degree = s.degree[a]
+                    b_degree = s.degree[b]
+                    if a_count > self.config.high_freq_thre and b_count > self.config.high_freq_thre: 
+                    # if a_count >= self.config.high_freq_thre and b_count >= self.config.high_freq_thre: # comment this line on 13 May 2023
+                        a2b = [a, a_count, a_degree, b, b_count, b_degree]
+                        new_a2b = self.err_type_classification(a2b) 
+                        new_a2b.insert(0, idx)     
+                        high_ambiguous_df.loc[len(high_ambiguous_df)] = new_a2b 
+                        b2a = [b, b_count, b_degree, a, a_count, a_degree]
+                        new_b2a = self.err_type_classification(b2a)
+                        new_b2a.insert(0, idx)
+                        high_ambiguous_df.loc[len(high_ambiguous_df)] = new_b2a
+                        idx += 1
+            del edges_lst
+        if self.config.verbose:
+            high_ambiguous_csv = self.config.result_dir + "high_ambiguous_1nt.csv"
+            high_ambiguous_df.to_csv(high_ambiguous_csv, index=False)  
+        self.logger.info("Done!")
+        return high_ambiguous_df
 '''
```

### Comparing `noise2read-0.0.85/src/noise2read/data_preprocessing.py` & `noise2read-0.0.88/src/noise2read/data_preprocessing.py`

 * *Files identical despite different names*

### Comparing `noise2read-0.0.85/src/noise2read/encoding.py` & `noise2read-0.0.88/src/noise2read/encoding.py`

 * *Files identical despite different names*

### Comparing `noise2read-0.0.85/src/noise2read/error_orrection.py` & `noise2read-0.0.88/src/noise2read/error_orrection.py`

 * *Files identical despite different names*

### Comparing `noise2read-0.0.85/src/noise2read/isolates_correction.py` & `noise2read-0.0.88/src/noise2read/isolates_correction.py`

 * *Files identical despite different names*

### Comparing `noise2read-0.0.85/src/noise2read/noise2read.py` & `noise2read-0.0.88/src/noise2read/noise2read.py`

 * *Files identical despite different names*

### Comparing `noise2read-0.0.85/src/noise2read/reads2vectors.py` & `noise2read-0.0.88/src/noise2read/reads2vectors.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,29 +1,32 @@
 # -*- coding: utf-8 -*-
 # @Author: Pengyao Ping
 # @Date:   2023-02-16 11:01:06
 # @Last Modified by:   Pengyao Ping
-# @Last Modified time: 2023-05-17 19:58:46
+# @Last Modified time: 2023-05-18 12:23:57
 
 from typing import Counter
 import numpy as np
 # import os
 from sklearn.preprocessing import StandardScaler
 from noise2read.encoding import EncodeScheme
 from mpire import WorkerPool
 from tqdm import tqdm
 from noise2read.utils import *
 import itertools
+import pickle
+import multiprocessing as mp
+
 
 class Reads2Vectors():
     def __init__(self, logger, config, edit_dis):
         self.logger = logger
         self.edit_dis = edit_dis
         self.config = config
-
+    '''
     def read2features(self, shared_objects, i):
         ES, reads_lst1, reads_lst2, other_features = shared_objects
         features = []
         # pd_fe = ES.descriptors("PairDistance", reads_lst[i])
         # features.extend(pd_fe)    
         ###########################################################################
         # features.append(read_count_lst[i]) 
@@ -58,15 +61,15 @@
         features.extend(atomic_fea1)
         features.extend(atomic_fea2)
         # onehot_fea = ES.descriptors("OneHot", reads_lst1[i])
         # features.extend(onehot_fea)
         features.extend(other_features[i])
         # self.logger.debug(f'FourierTransform: {len(ft_fea)}, ChaosGame: {len(cg_fea)}, Entropy: {len(entropy_fea)}, FickettScore: {len(fs_fea)}')
         return features 
-
+    '''
     def high_all_in_one_embedding(self, genuine_df, negative_df, new_negative_df, ambiguous_df):
         self.logger.info("Embedding genuine and high ambiguous data.")
         genuine_reads_lst1 = []
         negtive_reads_lst1 = []
         ambiguous_reads_lst1 = []
 
         genuine_reads_lst2 = []
@@ -165,28 +168,28 @@
             cur_kmer2 = row['EndErrKmer']
             cur_err_tye_val = (err_tyes2count[cur_err_tye] + error_tye_priors[cur_err_tye]) / (total_err_tyes_count + 1)
             cur_err_kmer_val1 = (err_kmers2count[cur_kmer1] + kmers_priors[cur_kmer1]) / (total_err_kmers_count + 1)
             cur_err_kmer_val2 = (err_kmers2count[cur_kmer2] + kmers_priors[cur_kmer2]) / (total_err_kmers_count + 1)
             negtive_reads_features.append([cur_err_tye_val, cur_err_kmer_val1, cur_err_kmer_val2]) #, row["StartDegree"]
 
         # isolates negative
-        # for idx, row in negative_df.iterrows():
-        #     read = row['StartRead']
-        #     pos_reads = enumerate_ed1_seqs(read)
-        #     for read2 in pos_reads:
-        #         negtive_reads_lst1.append(read) 
-        #         negtive_reads_lst2.append(read2)  
-        #         cur_err_tye_kmers = error_type_classification(read, read2)
-        #         cur_err_tye = cur_err_tye_kmers[0]
-        #         cur_kmer1 = cur_err_tye_kmers[1]
-        #         cur_kmer2 = cur_err_tye_kmers[2]
-        #         cur_err_tye_val = (err_tyes2count[cur_err_tye] + error_tye_priors[cur_err_tye]) / (total_err_tyes_count + 1)
-        #         cur_err_kmer_val1 = (err_kmers2count[cur_kmer1] + kmers_priors[cur_kmer1]) / (total_err_kmers_count + 1)
-        #         cur_err_kmer_val2 = (err_kmers2count[cur_kmer2] + kmers_priors[cur_kmer2]) / (total_err_kmers_count + 1)
-        #         negtive_reads_features.append([cur_err_tye_val, cur_err_kmer_val1, cur_err_kmer_val2])  
+        for idx, row in negative_df.iterrows():
+            read = row['StartRead']
+            pos_reads = enumerate_ed1_seqs(read)
+            for read2 in pos_reads:
+                negtive_reads_lst1.append(read) 
+                negtive_reads_lst2.append(read2)  
+                cur_err_tye_kmers = error_type_classification(read, read2)
+                cur_err_tye = cur_err_tye_kmers[0]
+                cur_kmer1 = cur_err_tye_kmers[1]
+                cur_kmer2 = cur_err_tye_kmers[2]
+                cur_err_tye_val = (err_tyes2count[cur_err_tye] + error_tye_priors[cur_err_tye]) / (total_err_tyes_count + 1)
+                cur_err_kmer_val1 = (err_kmers2count[cur_kmer1] + kmers_priors[cur_kmer1]) / (total_err_kmers_count + 1)
+                cur_err_kmer_val2 = (err_kmers2count[cur_kmer2] + kmers_priors[cur_kmer2]) / (total_err_kmers_count + 1)
+                negtive_reads_features.append([cur_err_tye_val, cur_err_kmer_val1, cur_err_kmer_val2])  
 
         for idx, row in ambiguous_df.iterrows():
             ambiguous_reads_lst1.append(row['StartRead'])
             ambiguous_reads_lst2.append(row['EndRead'])
             cur_err_tye = row['ErrorTye']
             cur_kmer1 = row['StartErrKmer']
             cur_kmer2 = row['EndErrKmer']
@@ -473,19 +476,19 @@
         genuine_fea = self.read2vec(genuine_reads_lst1, genuine_reads_lst2, genuine_reads_features)
         negative_fea = self.read2vec(negtive_reads_lst1, negtive_reads_lst2, negtive_reads_features)
         ambiguous_fea = self.read2vec(ambiguous_reads_lst1, ambiguous_reads_lst2, ambiguous_reads_features)
         del genuine_reads_lst1, genuine_reads_lst2, genuine_reads_features, negtive_reads_lst1, negtive_reads_lst2, negtive_reads_features, ambiguous_reads_lst1, ambiguous_reads_lst2, ambiguous_reads_features
 
         read_features = genuine_fea + negative_fea
         labels = np.array([1] * len(genuine_fea) + [0] * len(negative_fea))
-        train_data = np.array(read_features)
+        train_data = np.array(read_features, dtype=object)
         shape1 = (len(labels), len(read_features[0]))
         train_data.reshape(shape1)   
-
-        ambiguous_data = np.array(ambiguous_fea)
+        print(train_data.size)
+        ambiguous_data = np.array(ambiguous_fea, dtype=object)
         shape2 = (len(ambiguous_fea), len(ambiguous_fea[0]))
         ambiguous_data.reshape(shape2) 
         # scaling data
         self.logger.debug(train_data.shape)
         self.logger.debug(ambiguous_data.shape)
         if self.edit_dis == 1:
             train, ambiguous = self.scaler(train_data, ambiguous_data, high_flag)
@@ -574,14 +577,82 @@
             del lab_scale_f0, lab_scale_f1, lab_scale_f3, ulab_scale_f0, ulab_scale_f1, ulab_scale_f3
                 
         # lab_scale_f = np.hstack((lab_scale_f0, lab_scale_f1, lab_scale_f2, lab_scale_f3))
         # ulab_scale_f = np.hstack((ulab_scale_f0, ulab_scale_f1, ulab_scale_f2, ulab_scale_f3))
         
         return lab_scale_f, ulab_scale_f 
 
+
+    # def read2features(self, shared_objects, i):
+    def read2features(self, ES, ori_feature):
+        # ES, reads_lst1, reads_lst2, other_features = shared_objects
+        features = []
+        
+        ###########################################################################
+        ft_fea1 = ES.descriptors("FourierTransform", ori_feature[0])
+        cg_fea1 = ES.descriptors("ChaosGame", ori_feature[0])
+        entropy_fea1 = ES.descriptors("Entropy", ori_feature[0])
+        fs_fea1 = ES.descriptors("FickettScore", ori_feature[0])
+        features.extend(ft_fea1)
+        features.extend(cg_fea1)
+        features.extend(entropy_fea1)
+        features.extend(fs_fea1)
+        atomic_fea1 = ES.descriptors("atomic_number",ori_feature[0])
+        atomic_fea2 = ES.descriptors("atomic_number", ori_feature[1])
+        features.extend(atomic_fea1)
+        features.extend(atomic_fea2)
+        
+        features.extend(ori_feature[2:])
+        return features 
+
+    def read2vec(self, reads_lst1, reads_lst2, other_features):  
+        ES = EncodeScheme(self.config.read_max_len, self.config.entropy_kmer, self.config.entropy_q, self.config.kmer_freq, self.config.read_type)
+
+        # Combine the features of each sample into one list
+        combined_features = []
+        for seq1, seq2, lst in zip(reads_lst1, reads_lst2, other_features):
+            tmp_lst = []
+            tmp_lst.append(seq1)
+            tmp_lst.append(seq2)
+            tmp_lst.extend(lst)
+            combined_features.append(tmp_lst)
+            del tmp_lst
+
+        chunk_size = len(combined_features) // self.config.chunks_num
+        if chunk_size > 0:
+            chunks = [combined_features[i:i+chunk_size] for i in range(0, len(combined_features), chunk_size)]
+        else:
+            chunks = combined_features
+        
+        # Use multiprocessing to write each chunk to a separate pickle file
+        chunk_names = []
+        for i, chunk in enumerate(chunks):
+            pool = mp.Pool(processes=self.config.num_workers)
+            vectors = pool.starmap(self.read2features, [(ES, sequence) for sequence in chunk])
+            pool.close()
+            pool.join()
+            # Generate the pickle file name
+            file_name = self.config.result_dir + f"chunk_{i}.pickle"
+            # Write the vectors to the pickle file
+            with open(file_name, "wb") as file:
+                pickle.dump(vectors, file)
+
+            chunk_names.append(file_name)
+
+        combined_data = []
+        for file_name in chunk_names:
+            with open(file_name, "rb") as file:
+                vectors = pickle.load(file)
+                combined_data.extend(vectors)
+            os.remove(file_name)
+
+        del combined_features, chunks      
+        return combined_data
+    
+'''
     def read2vec(self, reads_lst1, reads_lst2, other_features):
         read_features = []    
         ES = EncodeScheme(self.config.read_max_len, self.config.entropy_kmer, self.config.entropy_q, self.config.kmer_freq, self.config.read_type)
 
         shared_objects = ES, reads_lst1, reads_lst2, other_features
         # with WorkerPool(self.config.num_workers, shared_objects=shared_objects, start_method='fork') as pool:
         #     with tqdm(total=len(reads_lst1), desc=self.logger.info("Encoding reads")) as pbar:   
@@ -589,8 +660,9 @@
         #             read_features.append(fea_lst)
         #             pbar.update()  
         with WorkerPool(self.config.num_workers, shared_objects=shared_objects, start_method='fork') as pool:
             for fea_lst in pool.imap(self.read2features, range(len(reads_lst1)), progress_bar=self.config.verbose):
                 read_features.append(fea_lst)
         
         self.logger.debug(f'{len(read_features)}, {len(read_features[0])}')
-        return read_features
+        return read_features
+'''
```

### Comparing `noise2read-0.0.85/src/noise2read/simulation.py` & `noise2read-0.0.88/src/noise2read/simulation.py`

 * *Files identical despite different names*

### Comparing `noise2read-0.0.85/src/noise2read/umitest.py` & `noise2read-0.0.88/src/noise2read/umitest.py`

 * *Files identical despite different names*

### Comparing `noise2read-0.0.85/src/noise2read/utils.py` & `noise2read-0.0.88/src/noise2read/utils.py`

 * *Files identical despite different names*

### Comparing `noise2read-0.0.85/src/noise2read.egg-info/PKG-INFO` & `noise2read-0.0.88/src/noise2read.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: noise2read
-Version: 0.0.85
+Version: 0.0.88
 Summary: Turn noise to read
 Home-page: https://github.com/Jappy0/noise2read
 Author: Penagyao Ping
 Author-email: ping.pengyao@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `noise2read-0.0.85/src/noise2read.egg-info/SOURCES.txt` & `noise2read-0.0.88/src/noise2read.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `noise2read-0.0.85/tests/test_data_generation.py` & `noise2read-0.0.88/tests/test_data_generation.py`

 * *Files identical despite different names*

### Comparing `noise2read-0.0.85/tests/test_reads2vector.py` & `noise2read-0.0.88/tests/test_reads2vector.py`

 * *Files identical despite different names*

### Comparing `noise2read-0.0.85/tests/test_utils.py` & `noise2read-0.0.88/tests/test_utils.py`

 * *Files identical despite different names*

