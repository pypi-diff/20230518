# Comparing `tmp/ibis-genome-0.7.1.tar.gz` & `tmp/ibis-genome-0.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ibis-genome-0.7.1.tar", last modified: Wed May 17 03:49:33 2023, max compression
+gzip compressed data, was "ibis-genome-0.7.2.tar", last modified: Thu May 18 01:14:15 2023, max compression
```

## Comparing `ibis-genome-0.7.1.tar` & `ibis-genome-0.7.2.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 03:49:33.678264 ibis-genome-0.7.1/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-17 03:49:20.000000 ibis-genome-0.7.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-17 03:49:20.000000 ibis-genome-0.7.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    44009 2023-05-17 03:49:33.678264 ibis-genome-0.7.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2963 2023-05-17 03:49:20.000000 ibis-genome-0.7.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 03:49:33.670264 ibis-genome-0.7.1/ibis/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-17 03:49:20.000000 ibis-genome-0.7.1/ibis/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 03:49:33.670264 ibis-genome-0.7.1/ibis/config/
--rw-r--r--   0 runner    (1001) docker     (123)      466 2023-05-17 03:49:20.000000 ibis-genome-0.7.1/ibis/config/template_coassemble.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-17 03:49:20.000000 ibis-genome-0.7.1/ibis/config/template_evaluate.yaml
--rwxr-xr-x   0 runner    (1001) docker     (123)    37806 2023-05-17 03:49:20.000000 ibis-genome-0.7.1/ibis/ibis.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 03:49:33.670264 ibis-genome-0.7.1/ibis/workflow/
--rw-r--r--   0 runner    (1001) docker     (123)    16160 2023-05-17 03:49:20.000000 ibis-genome-0.7.1/ibis/workflow/coassemble.smk
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 03:49:33.670264 ibis-genome-0.7.1/ibis/workflow/env/
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-05-17 03:49:20.000000 ibis-genome-0.7.1/ibis/workflow/env/aviary.yml
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-05-17 03:49:20.000000 ibis-genome-0.7.1/ibis/workflow/env/coverm.yml
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-05-17 03:49:20.000000 ibis-genome-0.7.1/ibis/workflow/env/kingfisher.yml
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-05-17 03:49:20.000000 ibis-genome-0.7.1/ibis/workflow/env/prodigal.yml
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-05-17 03:49:20.000000 ibis-genome-0.7.1/ibis/workflow/env/r.yml
--rw-r--r--   0 runner    (1001) docker     (123)      553 2023-05-17 03:49:20.000000 ibis-genome-0.7.1/ibis/workflow/env/singlem.yml
--rw-r--r--   0 runner    (1001) docker     (123)     5032 2023-05-17 03:49:20.000000 ibis-genome-0.7.1/ibis/workflow/evaluate.smk
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 03:49:33.674264 ibis-genome-0.7.1/ibis/workflow/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (123)     2548 2023-05-17 03:49:20.000000 ibis-genome-0.7.1/ibis/workflow/scripts/aviary_commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     8093 2023-05-17 03:49:20.000000 ibis-genome-0.7.1/ibis/workflow/scripts/cluster_graph.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3020 2023-05-17 03:49:20.000000 ibis-genome-0.7.1/ibis/workflow/scripts/collect_reference_bins.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    10121 2023-05-17 03:49:20.000000 ibis-genome-0.7.1/ibis/workflow/scripts/evaluate.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      922 2023-05-17 03:49:20.000000 ibis-genome-0.7.1/ibis/workflow/scripts/no_genomes.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3351 2023-05-17 03:49:20.000000 ibis-genome-0.7.1/ibis/workflow/scripts/query_processing.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      773 2023-05-17 03:49:20.000000 ibis-genome-0.7.1/ibis/workflow/scripts/separate_SingleM_seq.py
--rw-r--r--   0 runner    (1001) docker     (123)      708 2023-05-17 03:49:20.000000 ibis-genome-0.7.1/ibis/workflow/scripts/summarise_coassemblies.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3524 2023-05-17 03:49:20.000000 ibis-genome-0.7.1/ibis/workflow/scripts/target_elusive.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 03:49:33.674264 ibis-genome-0.7.1/ibis_genome.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    44009 2023-05-17 03:49:33.000000 ibis-genome-0.7.1/ibis_genome.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-05-17 03:49:33.000000 ibis-genome-0.7.1/ibis_genome.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 03:49:33.000000 ibis-genome-0.7.1/ibis_genome.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-17 03:49:33.000000 ibis-genome-0.7.1/ibis_genome.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-17 03:49:33.000000 ibis-genome-0.7.1/ibis_genome.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-17 03:49:33.000000 ibis-genome-0.7.1/ibis_genome.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      850 2023-05-17 03:49:20.000000 ibis-genome-0.7.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-17 03:49:33.678264 ibis-genome-0.7.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 03:49:33.678264 ibis-genome-0.7.1/test/
--rw-r--r--   0 runner    (1001) docker     (123)     9356 2023-05-17 03:49:21.000000 ibis-genome-0.7.1/test/test_cluster_graph.py
--rw-r--r--   0 runner    (1001) docker     (123)    40641 2023-05-17 03:49:21.000000 ibis-genome-0.7.1/test/test_coassemble.py
--rw-r--r--   0 runner    (1001) docker     (123)     3834 2023-05-17 03:49:21.000000 ibis-genome-0.7.1/test/test_collect_reference_bins.py
--rw-r--r--   0 runner    (1001) docker     (123)     9194 2023-05-17 03:49:21.000000 ibis-genome-0.7.1/test/test_evaluate.py
--rw-r--r--   0 runner    (1001) docker     (123)    31367 2023-05-17 03:49:21.000000 ibis-genome-0.7.1/test/test_evaluate_script.py
--rw-r--r--   0 runner    (1001) docker     (123)     7078 2023-05-17 03:49:21.000000 ibis-genome-0.7.1/test/test_iterate.py
--rw-r--r--   0 runner    (1001) docker     (123)     2620 2023-05-17 03:49:21.000000 ibis-genome-0.7.1/test/test_no_genomes.py
--rw-r--r--   0 runner    (1001) docker     (123)     9146 2023-05-17 03:49:21.000000 ibis-genome-0.7.1/test/test_query_processing.py
--rw-r--r--   0 runner    (1001) docker     (123)     7229 2023-05-17 03:49:21.000000 ibis-genome-0.7.1/test/test_target_elusive.py
--rw-r--r--   0 runner    (1001) docker     (123)    20277 2023-05-17 03:49:21.000000 ibis-genome-0.7.1/test/test_unmap.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 01:14:15.510722 ibis-genome-0.7.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-18 01:14:04.000000 ibis-genome-0.7.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-18 01:14:04.000000 ibis-genome-0.7.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    44009 2023-05-18 01:14:15.510722 ibis-genome-0.7.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2963 2023-05-18 01:14:04.000000 ibis-genome-0.7.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 01:14:15.502722 ibis-genome-0.7.2/ibis/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-18 01:14:04.000000 ibis-genome-0.7.2/ibis/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 01:14:15.502722 ibis-genome-0.7.2/ibis/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      466 2023-05-18 01:14:04.000000 ibis-genome-0.7.2/ibis/config/template_coassemble.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-18 01:14:04.000000 ibis-genome-0.7.2/ibis/config/template_evaluate.yaml
+-rwxr-xr-x   0 runner    (1001) docker     (123)    37806 2023-05-18 01:14:04.000000 ibis-genome-0.7.2/ibis/ibis.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 01:14:15.506723 ibis-genome-0.7.2/ibis/workflow/
+-rw-r--r--   0 runner    (1001) docker     (123)    16213 2023-05-18 01:14:04.000000 ibis-genome-0.7.2/ibis/workflow/coassemble.smk
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 01:14:15.506723 ibis-genome-0.7.2/ibis/workflow/env/
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-05-18 01:14:04.000000 ibis-genome-0.7.2/ibis/workflow/env/aviary.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-05-18 01:14:04.000000 ibis-genome-0.7.2/ibis/workflow/env/coverm.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-05-18 01:14:04.000000 ibis-genome-0.7.2/ibis/workflow/env/kingfisher.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-05-18 01:14:04.000000 ibis-genome-0.7.2/ibis/workflow/env/prodigal.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-05-18 01:14:04.000000 ibis-genome-0.7.2/ibis/workflow/env/r.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      553 2023-05-18 01:14:04.000000 ibis-genome-0.7.2/ibis/workflow/env/singlem.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     5032 2023-05-18 01:14:04.000000 ibis-genome-0.7.2/ibis/workflow/evaluate.smk
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 01:14:15.506723 ibis-genome-0.7.2/ibis/workflow/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2548 2023-05-18 01:14:04.000000 ibis-genome-0.7.2/ibis/workflow/scripts/aviary_commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8093 2023-05-18 01:14:04.000000 ibis-genome-0.7.2/ibis/workflow/scripts/cluster_graph.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3020 2023-05-18 01:14:04.000000 ibis-genome-0.7.2/ibis/workflow/scripts/collect_reference_bins.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10121 2023-05-18 01:14:04.000000 ibis-genome-0.7.2/ibis/workflow/scripts/evaluate.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      922 2023-05-18 01:14:04.000000 ibis-genome-0.7.2/ibis/workflow/scripts/no_genomes.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3715 2023-05-18 01:14:04.000000 ibis-genome-0.7.2/ibis/workflow/scripts/query_processing.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      773 2023-05-18 01:14:04.000000 ibis-genome-0.7.2/ibis/workflow/scripts/separate_SingleM_seq.py
+-rw-r--r--   0 runner    (1001) docker     (123)      708 2023-05-18 01:14:04.000000 ibis-genome-0.7.2/ibis/workflow/scripts/summarise_coassemblies.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3524 2023-05-18 01:14:04.000000 ibis-genome-0.7.2/ibis/workflow/scripts/target_elusive.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 01:14:15.506723 ibis-genome-0.7.2/ibis_genome.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    44009 2023-05-18 01:14:15.000000 ibis-genome-0.7.2/ibis_genome.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-05-18 01:14:15.000000 ibis-genome-0.7.2/ibis_genome.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 01:14:15.000000 ibis-genome-0.7.2/ibis_genome.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-18 01:14:15.000000 ibis-genome-0.7.2/ibis_genome.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-18 01:14:15.000000 ibis-genome-0.7.2/ibis_genome.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-18 01:14:15.000000 ibis-genome-0.7.2/ibis_genome.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      850 2023-05-18 01:14:04.000000 ibis-genome-0.7.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-18 01:14:15.510722 ibis-genome-0.7.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 01:14:15.510722 ibis-genome-0.7.2/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     9356 2023-05-18 01:14:04.000000 ibis-genome-0.7.2/test/test_cluster_graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45532 2023-05-18 01:14:04.000000 ibis-genome-0.7.2/test/test_coassemble.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3834 2023-05-18 01:14:04.000000 ibis-genome-0.7.2/test/test_collect_reference_bins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9194 2023-05-18 01:14:04.000000 ibis-genome-0.7.2/test/test_evaluate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31367 2023-05-18 01:14:04.000000 ibis-genome-0.7.2/test/test_evaluate_script.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7078 2023-05-18 01:14:04.000000 ibis-genome-0.7.2/test/test_iterate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2620 2023-05-18 01:14:04.000000 ibis-genome-0.7.2/test/test_no_genomes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10554 2023-05-18 01:14:04.000000 ibis-genome-0.7.2/test/test_query_processing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7229 2023-05-18 01:14:04.000000 ibis-genome-0.7.2/test/test_target_elusive.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20277 2023-05-18 01:14:04.000000 ibis-genome-0.7.2/test/test_unmap.py
```

### Comparing `ibis-genome-0.7.1/LICENSE` & `ibis-genome-0.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ibis-genome-0.7.1/PKG-INFO` & `ibis-genome-0.7.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ibis-genome
-Version: 0.7.1
+Version: 0.7.2
 Summary: Ibis (Australian bin chicken) - targeted recovery of low abundance genomes through intelligent coassembly
 Author-email: Samuel Aroney <samuel.aroney@outlook.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `ibis-genome-0.7.1/README.md` & `ibis-genome-0.7.2/README.md`

 * *Files identical despite different names*

### Comparing `ibis-genome-0.7.1/ibis/ibis.py` & `ibis-genome-0.7.2/ibis/ibis.py`

 * *Files identical despite different names*

### Comparing `ibis-genome-0.7.1/ibis/workflow/coassemble.smk` & `ibis-genome-0.7.2/ibis/workflow/coassemble.smk`

 * *Files 2% similar despite different names*

```diff
@@ -207,14 +207,15 @@
         unbinned=output_dir + "/appraise/unbinned.otu_table.tsv",
         binned=output_dir + "/appraise/binned.otu_table.tsv",
     log:
         logs_dir + "/query/processing.log"
     params:
         sequence_identity=config["appraise_sequence_identity"],
         window_size=60,
+        taxa_of_interest=config["taxa_of_interest"],
     threads:
         64
     script:
         "scripts/query_processing.py"
 
 ################################
 ### No genomes (alternative) ###
```

### Comparing `ibis-genome-0.7.1/ibis/workflow/env/singlem.yml` & `ibis-genome-0.7.2/ibis/workflow/env/singlem.yml`

 * *Files identical despite different names*

### Comparing `ibis-genome-0.7.1/ibis/workflow/evaluate.smk` & `ibis-genome-0.7.2/ibis/workflow/evaluate.smk`

 * *Files identical despite different names*

### Comparing `ibis-genome-0.7.1/ibis/workflow/scripts/aviary_commands.py` & `ibis-genome-0.7.2/ibis/workflow/scripts/aviary_commands.py`

 * *Files identical despite different names*

### Comparing `ibis-genome-0.7.1/ibis/workflow/scripts/cluster_graph.py` & `ibis-genome-0.7.2/ibis/workflow/scripts/cluster_graph.py`

 * *Files identical despite different names*

### Comparing `ibis-genome-0.7.1/ibis/workflow/scripts/collect_reference_bins.py` & `ibis-genome-0.7.2/ibis/workflow/scripts/collect_reference_bins.py`

 * *Files identical despite different names*

### Comparing `ibis-genome-0.7.1/ibis/workflow/scripts/evaluate.py` & `ibis-genome-0.7.2/ibis/workflow/scripts/evaluate.py`

 * *Files identical despite different names*

### Comparing `ibis-genome-0.7.1/ibis/workflow/scripts/no_genomes.py` & `ibis-genome-0.7.2/ibis/workflow/scripts/no_genomes.py`

 * *Files identical despite different names*

### Comparing `ibis-genome-0.7.1/ibis/workflow/scripts/query_processing.py` & `ibis-genome-0.7.2/ibis/workflow/scripts/query_processing.py`

 * *Files 11% similar despite different names*

```diff
@@ -16,20 +16,27 @@
     "found_in": str,
     }
 
 def processing(
     query_read,
     pipe_read,
     SEQUENCE_IDENTITY=0.86,
-    WINDOW_SIZE=60):
+    WINDOW_SIZE=60,
+    TAXA_OF_INTEREST=None):
 
     if len(query_read) == 0:
         empty_output = pl.DataFrame(schema=OUTPUT_COLUMNS)
         return empty_output, empty_output
 
+    # Filter TAXA_OF_INTEREST
+    if TAXA_OF_INTEREST:
+        pipe_read = pipe_read.filter(
+            pl.col("taxonomy").str.contains(TAXA_OF_INTEREST, literal=True)
+        )
+
     appraised = query_read.rename(
         # Rename to match appraise output
         # Query output: query_name, query_sequence, divergence, num_hits, coverage, sample, marker, hit_sequence, taxonomy
         # Appraise output: gene, sample, sequence, num_hits, coverage, taxonomy, found_in
         {"marker": "gene", "query_name":"sample", "query_sequence": "sequence", "sample": "found_in"}
     ).drop([
         # Query taxonomy, num_hits and coverage are from database (e.g. the genomes)
@@ -60,42 +67,46 @@
 
     return binned, unbinned
 
 def pipeline(
     query_reads,
     pipe_reads,
     SEQUENCE_IDENTITY=0.86,
-    WINDOW_SIZE=60):
+    WINDOW_SIZE=60,
+    TAXA_OF_INTEREST=None):
 
     print(f"Polars using {str(pl.threadpool_size())} threads")
 
     for query, pipe in zip(query_reads, pipe_reads):
         binned, unbinned = processing(
             pl.read_csv(query, separator="\t"),
             pl.read_csv(pipe, separator="\t"),
             SEQUENCE_IDENTITY,
-            WINDOW_SIZE)
+            WINDOW_SIZE,
+            TAXA_OF_INTEREST)
         yield binned, unbinned
 
 if __name__ == "__main__":
     os.environ["POLARS_MAX_THREADS"] = str(snakemake.threads)
     import polars as pl
 
     SEQUENCE_IDENTITY = snakemake.params.sequence_identity
     WINDOW_SIZE = snakemake.params.window_size
+    TAXA_OF_INTEREST = snakemake.params.taxa_of_interest
     query_reads = snakemake.input.query_reads
     pipe_reads = snakemake.input.pipe_reads
     binned_path = snakemake.output.binned
     unbinned_path = snakemake.output.unbinned
 
     outputs = pipeline(
         query_reads,
         pipe_reads,
         SEQUENCE_IDENTITY=SEQUENCE_IDENTITY,
-        WINDOW_SIZE=WINDOW_SIZE
+        WINDOW_SIZE=WINDOW_SIZE,
+        TAXA_OF_INTEREST=TAXA_OF_INTEREST
         )
 
     with open(binned_path, "ab") as binned_file, open(unbinned_path, "ab") as unbinned_file:
         first = True
         for binned, unbinned in outputs:
             binned.write_csv(binned_file, separator="\t", has_header=first)
             unbinned.write_csv(unbinned_file, separator="\t", has_header=first)
```

### Comparing `ibis-genome-0.7.1/ibis/workflow/scripts/separate_SingleM_seq.py` & `ibis-genome-0.7.2/ibis/workflow/scripts/separate_SingleM_seq.py`

 * *Files identical despite different names*

### Comparing `ibis-genome-0.7.1/ibis/workflow/scripts/summarise_coassemblies.py` & `ibis-genome-0.7.2/ibis/workflow/scripts/summarise_coassemblies.py`

 * *Files identical despite different names*

### Comparing `ibis-genome-0.7.1/ibis/workflow/scripts/target_elusive.py` & `ibis-genome-0.7.2/ibis/workflow/scripts/target_elusive.py`

 * *Files identical despite different names*

### Comparing `ibis-genome-0.7.1/ibis_genome.egg-info/PKG-INFO` & `ibis-genome-0.7.2/ibis_genome.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ibis-genome
-Version: 0.7.1
+Version: 0.7.2
 Summary: Ibis (Australian bin chicken) - targeted recovery of low abundance genomes through intelligent coassembly
 Author-email: Samuel Aroney <samuel.aroney@outlook.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `ibis-genome-0.7.1/ibis_genome.egg-info/SOURCES.txt` & `ibis-genome-0.7.2/ibis_genome.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ibis-genome-0.7.1/pyproject.toml` & `ibis-genome-0.7.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ibis-genome-0.7.1/test/test_cluster_graph.py` & `ibis-genome-0.7.2/test/test_cluster_graph.py`

 * *Files identical despite different names*

### Comparing `ibis-genome-0.7.1/test/test_coassemble.py` & `ibis-genome-0.7.2/test/test_coassemble.py`

 * *Files 12% similar despite different names*

```diff
@@ -330,14 +330,119 @@
                     ]),
                     ""
                 ]
             )
             with open(cluster_path) as f:
                 self.assertEqual(expected, f.read())
 
+    def test_coassemble_query_input_taxa_of_interest(self):
+        with in_tempdir():
+            cmd = (
+                f"ibis coassemble "
+                f"--forward {SAMPLE_READS_FORWARD} "
+                f"--reverse {SAMPLE_READS_REVERSE} "
+                f"--genomes {GENOMES} "
+                f"--genome-transcripts {GENOME_TRANSCRIPTS} "
+                f"--sample-query {SAMPLE_QUERY} "
+                f"--sample-singlem {SAMPLE_QUERY_SINGLEM} "
+                f"--sample-read-size {SAMPLE_READ_SIZE} "
+                f"--taxa-of-interest \"p__Actinobacteriota\" "
+                f"--output test "
+                f"--conda-prefix {path_to_conda} "
+                f"--snakemake-args \"cluster_graph\" "
+            )
+            extern.run(cmd)
+
+            config_path = os.path.join("test", "config.yaml")
+            self.assertTrue(os.path.exists(config_path))
+
+            binned_path = os.path.join("test", "coassemble", "appraise", "binned.otu_table.tsv")
+            self.assertTrue(os.path.exists(binned_path))
+            expected = "\n".join(
+                [
+                    "\t".join(["gene", "sample", "sequence", "num_hits", "coverage", "taxonomy", "found_in"]),
+                    ""
+                ]
+            )
+            with open(binned_path) as f:
+                self.assertEqual(expected, f.read())
+
+            unbinned_path = os.path.join("test", "coassemble", "appraise", "unbinned.otu_table.tsv")
+            self.assertTrue(os.path.exists(unbinned_path))
+            expected = "\n".join(
+                [
+                    "\t".join([
+                        "gene",
+                        "sample",
+                        "sequence",
+                        "num_hits",
+                        "coverage",
+                        "taxonomy",
+                        "found_in",
+                    ]),
+                    "\t".join([
+                        "S3.7.ribosomal_protein_S7",
+                        "sample_1",
+                        "TACCAGGTCCCGGTCGAGGTCCGTCCGATCCGCCAGACGACGCTCGCCCTGCGCTGGCTC",
+                        "5",
+                        "8.21",
+                        "Root; d__Bacteria; p__Actinobacteriota; c__Actinomycetia; o__Mycobacteriales; f__Mycobacteriaceae; g__Nocardia; s__Nocardia grenadensis",
+                        "",
+                    ]),
+                    "\t".join([
+                        "S3.7.ribosomal_protein_S7",
+                        "sample_1",
+                        "TATCAGGTGCCTATTGAGGTAAGACCTGAAAGAAGACAGACTTTAGCGCTTCGCTGGATA",
+                        "1",
+                        "1.64",
+                        "Root; d__Bacteria; p__Actinobacteriota; c__Actinomycetia; o__Mycobacteriales; f__Mycobacteriaceae; g__Nocardia; s__Nocardia grenadensis2",
+                        "",
+                    ]),
+                    "\t".join([
+                        "S3.7.ribosomal_protein_S7",
+                        "sample_1",
+                        "TATCAGGTGCCTATTGAGGTAAGACCTGAAAGAAGACAGACTTTAGCGCTTCGCTGGATC",
+                        "5",
+                        "8.21",
+                        "Root; d__Bacteria; p__Actinobacteriota; c__Actinomycetia; o__Mycobacteriales; f__Mycobacteriaceae; g__Nocardia; s__Nocardia grenadensis3",
+                        "",
+                    ]),
+                    "\t".join([
+                        "S3.7.ribosomal_protein_S7",
+                        "sample_2",
+                        "TACCAGGTCCCGGTCGAGGTCCGTCCGATCCGCCAGACGACGCTCGCCCTGCGCTGGCTC",
+                        "3",
+                        "4.92",
+                        "Root; d__Bacteria; p__Actinobacteriota; c__Actinomycetia; o__Mycobacteriales; f__Mycobacteriaceae; g__Nocardia; s__Nocardia grenadensis",
+                        "",
+                    ]),
+                    "\t".join([
+                        "S3.7.ribosomal_protein_S7",
+                        "sample_3",
+                        "TATCAGGTGCCTATTGAGGTAAGACCTGAAAGAAGACAGACTTTAGCGCTTCGCTGGATA",
+                        "6",
+                        "9.85",
+                        "Root; d__Bacteria; p__Actinobacteriota; c__Actinomycetia; o__Mycobacteriales; f__Mycobacteriaceae; g__Nocardia; s__Nocardia grenadensis2",
+                        "",
+                    ]),
+                    ""
+                ]
+            )
+            with open(unbinned_path) as f:
+                self.assertEqual(expected, f.read())
+
+            edges_path = os.path.join("test", "coassemble", "target", "targets.tsv")
+            self.assertTrue(os.path.exists(edges_path))
+
+            edges_path = os.path.join("test", "coassemble", "target", "elusive_edges.tsv")
+            self.assertTrue(os.path.exists(edges_path))
+
+            cluster_path = os.path.join("test", "coassemble", "target", "elusive_clusters.tsv")
+            self.assertTrue(os.path.exists(cluster_path))
+
     def test_coassemble_single_assembly(self):
         with in_tempdir():
             cmd = (
                 f"ibis coassemble "
                 f"--forward {SAMPLE_READS_FORWARD} "
                 f"--reverse {SAMPLE_READS_REVERSE} "
                 f"--singlem-metapackage {METAPACKAGE} "
```

### Comparing `ibis-genome-0.7.1/test/test_collect_reference_bins.py` & `ibis-genome-0.7.2/test/test_collect_reference_bins.py`

 * *Files identical despite different names*

### Comparing `ibis-genome-0.7.1/test/test_evaluate.py` & `ibis-genome-0.7.2/test/test_evaluate.py`

 * *Files identical despite different names*

### Comparing `ibis-genome-0.7.1/test/test_evaluate_script.py` & `ibis-genome-0.7.2/test/test_evaluate_script.py`

 * *Files identical despite different names*

### Comparing `ibis-genome-0.7.1/test/test_iterate.py` & `ibis-genome-0.7.2/test/test_iterate.py`

 * *Files identical despite different names*

### Comparing `ibis-genome-0.7.1/test/test_no_genomes.py` & `ibis-genome-0.7.2/test/test_no_genomes.py`

 * *Files identical despite different names*

### Comparing `ibis-genome-0.7.1/test/test_query_processing.py` & `ibis-genome-0.7.2/test/test_query_processing.py`

 * *Files 13% similar despite different names*

```diff
@@ -220,10 +220,35 @@
             ["S3.1", "sample_1", "AAB", 5, 10, "Root", None],
         ], schema=APPRAISE_COLUMNS)
 
         observed_binned, observed_unbinned = processing(query, pipe)
         self.assertDataFrameEqual(expected_binned, observed_binned)
         self.assertDataFrameEqual(expected_unbinned, observed_unbinned)
 
+    def test_query_processing_target_taxa(self):
+        query = pl.DataFrame([
+            ["sample_1", "AAA", 1, 5, 10, "genome_1", "S3.1", "AAA", "Root; d__Bacteria"],
+            ["sample_1", "AAB", 10, 5, 10, "genome_1", "S3.1", "AAA", "Root; d__Bacteria"],
+            ["sample_1", "CCC", 1, 5, 10, "genome_1", "S3.1", "AAA", "Root"],
+            ["sample_1", "CCD", 10, 5, 10, "genome_1", "S3.1", "AAA", "Root"],
+        ], schema=QUERY_COLUMNS)
+        pipe = pl.DataFrame([
+            ["S3.1", "sample_1", "AAA", 5, 10, "Root; d__Bacteria; p__Planctomycetota"],
+            ["S3.1", "sample_1", "AAB", 5, 10, "Root; d__Bacteria; p__Planctomycetota"],
+            ["S3.1", "sample_1", "CCC", 5, 10, "Root"],
+            ["S3.1", "sample_1", "CCD", 5, 10, "Root"],
+        ], schema=PIPE_COLUMNS)
+
+        expected_binned = pl.DataFrame([
+            ["S3.1", "sample_1", "AAA", 5, 10, "Root; d__Bacteria; p__Planctomycetota", "genome_1"],
+        ], schema=APPRAISE_COLUMNS)
+        expected_unbinned = pl.DataFrame([
+            ["S3.1", "sample_1", "AAB", 5, 10, "Root; d__Bacteria; p__Planctomycetota", None],
+        ], schema=APPRAISE_COLUMNS)
+
+        observed_binned, observed_unbinned = processing(query, pipe, TAXA_OF_INTEREST="p__Planctomycetota")
+        self.assertDataFrameEqual(expected_binned, observed_binned)
+        self.assertDataFrameEqual(expected_unbinned, observed_unbinned)
+
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `ibis-genome-0.7.1/test/test_target_elusive.py` & `ibis-genome-0.7.2/test/test_target_elusive.py`

 * *Files identical despite different names*

### Comparing `ibis-genome-0.7.1/test/test_unmap.py` & `ibis-genome-0.7.2/test/test_unmap.py`

 * *Files identical despite different names*

