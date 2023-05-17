# Comparing `tmp/MetaCHIP-1.9.6.tar.gz` & `tmp/MetaCHIP-1.9.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/MetaCHIP-1.9.6.tar", last modified: Thu Jul 23 06:25:41 2020, max compression
+gzip compressed data, was "dist/MetaCHIP-1.9.7.tar", last modified: Thu Jul 23 06:41:50 2020, max compression
```

## Comparing `MetaCHIP-1.9.6.tar` & `MetaCHIP-1.9.7.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 songweizhi   (501) staff       (20)        0 2020-07-23 06:25:41.382762 MetaCHIP-1.9.6/
--rwxr-xr-x   0 songweizhi   (501) staff       (20)      296 2019-04-28 13:02:47.000000 MetaCHIP-1.9.6/MANIFEST.in
-drwxr-xr-x   0 songweizhi   (501) staff       (20)        0 2020-07-23 06:25:41.375526 MetaCHIP-1.9.6/MetaCHIP/
--rw-r--r--   0 songweizhi   (501) staff       (20)   197298 2020-07-23 06:24:49.000000 MetaCHIP-1.9.6/MetaCHIP/BP.py
--rw-r--r--   0 songweizhi   (501) staff       (20)   155959 2020-07-18 09:22:16.000000 MetaCHIP-1.9.6/MetaCHIP/BP_rewrote.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     4913 2019-04-30 01:18:08.000000 MetaCHIP-1.9.6/MetaCHIP/MetaCHIP_add_group_to_tree.R
--rw-r--r--   0 songweizhi   (501) staff       (20)     1934 2020-07-01 08:18:41.000000 MetaCHIP-1.9.6/MetaCHIP/MetaCHIP_circos_HGT.R
--rw-r--r--   0 songweizhi   (501) staff       (20)     1147 2019-04-29 00:06:05.000000 MetaCHIP-1.9.6/MetaCHIP/MetaCHIP_config.py
--rw-r--r--   0 songweizhi   (501) staff       (20)  3311562 2019-07-23 00:40:55.000000 MetaCHIP-1.9.6/MetaCHIP/MetaCHIP_phylo.hmm
--rw-r--r--   0 songweizhi   (501) staff       (20)    59404 2019-11-26 00:41:25.000000 MetaCHIP-1.9.6/MetaCHIP/PI.py
--rw-r--r--   0 songweizhi   (501) staff       (20)    46517 2020-07-04 13:15:32.000000 MetaCHIP-1.9.6/MetaCHIP/PI_rewrote.py
--rwxr-xr-x   0 songweizhi   (501) staff       (20)  1865930 2017-01-06 11:11:38.000000 MetaCHIP-1.9.6/MetaCHIP/Ranger-DTL-Dated.linux
--rwxr-xr-x   0 songweizhi   (501) staff       (20)   359716 2017-03-16 00:16:38.000000 MetaCHIP-1.9.6/MetaCHIP/Ranger-DTL-Dated.mac
--rwxr-xr-x   0 songweizhi   (501) staff       (20)     5822 2019-07-25 11:46:17.000000 MetaCHIP-1.9.6/MetaCHIP/SankeyTaxon.py
--rw-r--r--   0 songweizhi   (501) staff       (20)      656 2020-07-23 06:25:05.000000 MetaCHIP-1.9.6/MetaCHIP/VERSION
--rwxr-xr-x   0 songweizhi   (501) staff       (20)        0 2017-02-20 16:48:50.000000 MetaCHIP-1.9.6/MetaCHIP/__init__.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     1249 2019-08-11 09:14:15.000000 MetaCHIP-1.9.6/MetaCHIP/circos_HGT.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     5682 2019-09-15 22:24:16.000000 MetaCHIP-1.9.6/MetaCHIP/filter_HGT.py
--rw-r--r--   0 songweizhi   (501) staff       (20)    30251 2019-07-26 09:19:48.000000 MetaCHIP-1.9.6/MetaCHIP/get_SCG_tree.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     5773 2019-12-15 23:11:35.000000 MetaCHIP-1.9.6/MetaCHIP/get_flk_gene_functions.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     6409 2020-07-06 01:32:39.000000 MetaCHIP-1.9.6/MetaCHIP/rename_seqs.py
--rw-r--r--   0 songweizhi   (501) staff       (20)    61430 2020-07-11 12:35:16.000000 MetaCHIP-1.9.6/MetaCHIP/test_1.py
--rw-r--r--   0 songweizhi   (501) staff       (20)    10878 2019-08-08 09:58:23.000000 MetaCHIP-1.9.6/MetaCHIP/tuning_full_length_and_end_match.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     6698 2019-07-23 08:56:00.000000 MetaCHIP-1.9.6/MetaCHIP/update_hmms.py
-drwxr-xr-x   0 songweizhi   (501) staff       (20)        0 2020-07-23 06:25:41.379988 MetaCHIP-1.9.6/MetaCHIP.egg-info/
--rw-r--r--   0 songweizhi   (501) staff       (20)      560 2020-07-23 06:25:40.000000 MetaCHIP-1.9.6/MetaCHIP.egg-info/PKG-INFO
--rw-r--r--   0 songweizhi   (501) staff       (20)      745 2020-07-23 06:25:40.000000 MetaCHIP-1.9.6/MetaCHIP.egg-info/SOURCES.txt
--rw-r--r--   0 songweizhi   (501) staff       (20)        1 2020-07-23 06:25:40.000000 MetaCHIP-1.9.6/MetaCHIP.egg-info/dependency_links.txt
--rw-r--r--   0 songweizhi   (501) staff       (20)       48 2020-07-23 06:25:40.000000 MetaCHIP-1.9.6/MetaCHIP.egg-info/requires.txt
--rw-r--r--   0 songweizhi   (501) staff       (20)        9 2020-07-23 06:25:40.000000 MetaCHIP-1.9.6/MetaCHIP.egg-info/top_level.txt
--rw-r--r--   0 songweizhi   (501) staff       (20)      560 2020-07-23 06:25:41.382146 MetaCHIP-1.9.6/PKG-INFO
--rw-r--r--   0 songweizhi   (501) staff       (20)     8499 2020-06-03 03:11:33.000000 MetaCHIP-1.9.6/README.md
-drwxr-xr-x   0 songweizhi   (501) staff       (20)        0 2020-07-23 06:25:41.380493 MetaCHIP-1.9.6/bin/
--rwxr-xr-x   0 songweizhi   (501) staff       (20)    17260 2020-07-06 01:32:39.000000 MetaCHIP-1.9.6/bin/MetaCHIP
--rw-r--r--   0 songweizhi   (501) staff       (20)       38 2020-07-23 06:25:41.383114 MetaCHIP-1.9.6/setup.cfg
--rw-r--r--   0 songweizhi   (501) staff       (20)     1130 2019-04-29 00:08:32.000000 MetaCHIP-1.9.6/setup.py
+drwxr-xr-x   0 songweizhi   (501) staff       (20)        0 2020-07-23 06:41:50.323542 MetaCHIP-1.9.7/
+-rwxr-xr-x   0 songweizhi   (501) staff       (20)      296 2019-04-28 13:02:47.000000 MetaCHIP-1.9.7/MANIFEST.in
+drwxr-xr-x   0 songweizhi   (501) staff       (20)        0 2020-07-23 06:41:50.317486 MetaCHIP-1.9.7/MetaCHIP/
+-rw-r--r--   0 songweizhi   (501) staff       (20)   197298 2020-07-23 06:37:31.000000 MetaCHIP-1.9.7/MetaCHIP/BP.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)   155959 2020-07-18 09:22:16.000000 MetaCHIP-1.9.7/MetaCHIP/BP_rewrote.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     4913 2019-04-30 01:18:08.000000 MetaCHIP-1.9.7/MetaCHIP/MetaCHIP_add_group_to_tree.R
+-rw-r--r--   0 songweizhi   (501) staff       (20)     1934 2020-07-01 08:18:41.000000 MetaCHIP-1.9.7/MetaCHIP/MetaCHIP_circos_HGT.R
+-rw-r--r--   0 songweizhi   (501) staff       (20)     1147 2019-04-29 00:06:05.000000 MetaCHIP-1.9.7/MetaCHIP/MetaCHIP_config.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)  3311562 2019-07-23 00:40:55.000000 MetaCHIP-1.9.7/MetaCHIP/MetaCHIP_phylo.hmm
+-rw-r--r--   0 songweizhi   (501) staff       (20)    59404 2019-11-26 00:41:25.000000 MetaCHIP-1.9.7/MetaCHIP/PI.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)    46517 2020-07-04 13:15:32.000000 MetaCHIP-1.9.7/MetaCHIP/PI_rewrote.py
+-rwxr-xr-x   0 songweizhi   (501) staff       (20)  1865930 2017-01-06 11:11:38.000000 MetaCHIP-1.9.7/MetaCHIP/Ranger-DTL-Dated.linux
+-rwxr-xr-x   0 songweizhi   (501) staff       (20)   359716 2017-03-16 00:16:38.000000 MetaCHIP-1.9.7/MetaCHIP/Ranger-DTL-Dated.mac
+-rwxr-xr-x   0 songweizhi   (501) staff       (20)     5822 2019-07-25 11:46:17.000000 MetaCHIP-1.9.7/MetaCHIP/SankeyTaxon.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)      656 2020-07-23 06:41:26.000000 MetaCHIP-1.9.7/MetaCHIP/VERSION
+-rwxr-xr-x   0 songweizhi   (501) staff       (20)        0 2017-02-20 16:48:50.000000 MetaCHIP-1.9.7/MetaCHIP/__init__.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     1249 2019-08-11 09:14:15.000000 MetaCHIP-1.9.7/MetaCHIP/circos_HGT.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     5682 2019-09-15 22:24:16.000000 MetaCHIP-1.9.7/MetaCHIP/filter_HGT.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)    30251 2019-07-26 09:19:48.000000 MetaCHIP-1.9.7/MetaCHIP/get_SCG_tree.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     5773 2019-12-15 23:11:35.000000 MetaCHIP-1.9.7/MetaCHIP/get_flk_gene_functions.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     6409 2020-07-06 01:32:39.000000 MetaCHIP-1.9.7/MetaCHIP/rename_seqs.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)    61430 2020-07-11 12:35:16.000000 MetaCHIP-1.9.7/MetaCHIP/test_1.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)    10878 2019-08-08 09:58:23.000000 MetaCHIP-1.9.7/MetaCHIP/tuning_full_length_and_end_match.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     6698 2019-07-23 08:56:00.000000 MetaCHIP-1.9.7/MetaCHIP/update_hmms.py
+drwxr-xr-x   0 songweizhi   (501) staff       (20)        0 2020-07-23 06:41:50.320952 MetaCHIP-1.9.7/MetaCHIP.egg-info/
+-rw-r--r--   0 songweizhi   (501) staff       (20)      560 2020-07-23 06:41:50.000000 MetaCHIP-1.9.7/MetaCHIP.egg-info/PKG-INFO
+-rw-r--r--   0 songweizhi   (501) staff       (20)      745 2020-07-23 06:41:50.000000 MetaCHIP-1.9.7/MetaCHIP.egg-info/SOURCES.txt
+-rw-r--r--   0 songweizhi   (501) staff       (20)        1 2020-07-23 06:41:50.000000 MetaCHIP-1.9.7/MetaCHIP.egg-info/dependency_links.txt
+-rw-r--r--   0 songweizhi   (501) staff       (20)       48 2020-07-23 06:41:50.000000 MetaCHIP-1.9.7/MetaCHIP.egg-info/requires.txt
+-rw-r--r--   0 songweizhi   (501) staff       (20)        9 2020-07-23 06:41:50.000000 MetaCHIP-1.9.7/MetaCHIP.egg-info/top_level.txt
+-rw-r--r--   0 songweizhi   (501) staff       (20)      560 2020-07-23 06:41:50.322737 MetaCHIP-1.9.7/PKG-INFO
+-rw-r--r--   0 songweizhi   (501) staff       (20)     8499 2020-06-03 03:11:33.000000 MetaCHIP-1.9.7/README.md
+drwxr-xr-x   0 songweizhi   (501) staff       (20)        0 2020-07-23 06:41:50.321558 MetaCHIP-1.9.7/bin/
+-rwxr-xr-x   0 songweizhi   (501) staff       (20)    17260 2020-07-06 01:32:39.000000 MetaCHIP-1.9.7/bin/MetaCHIP
+-rw-r--r--   0 songweizhi   (501) staff       (20)       38 2020-07-23 06:41:50.323821 MetaCHIP-1.9.7/setup.cfg
+-rw-r--r--   0 songweizhi   (501) staff       (20)     1130 2019-04-29 00:08:32.000000 MetaCHIP-1.9.7/setup.py
```

### Comparing `MetaCHIP-1.9.6/MetaCHIP/BP.py` & `MetaCHIP-1.9.7/MetaCHIP/BP.py`

 * *Files 0% similar despite different names*

```diff
@@ -3397,15 +3397,15 @@
 
         for each_flk_plot in flanking_plot_file_list:
             pwd_each_flk_plot = '%s/%s_x%s_Flanking_region_plots/1_Plots_normal/%s' % (pwd_MetaCHIP_op_folder, output_prefix, group_num, each_flk_plot)
             os.system('mv %s %s/%s_x%s_Flanking_region_plots/' % (pwd_each_flk_plot, pwd_MetaCHIP_op_folder, output_prefix, group_num))
 
         ###################################### Get_circlize_plot #######################################
 
-        pwd_plot_circos =               '%s/%s_x%s_HGT_circos.png'                   % (pwd_MetaCHIP_op_folder, output_prefix, group_num)
+        pwd_plot_circos =               '%s/%s_x%s_HGT_circos.pdf'                   % (pwd_MetaCHIP_op_folder, output_prefix, group_num)
 
         # get genome to group dict
         genome_to_group_dict = {}
         for genome in open(grouping_file):
             group_id2 = genome.strip().split(',')[0]
             genome_name = genome.strip().split(',')[1]
             genome_to_group_dict[genome_name] = group_id2
@@ -3480,15 +3480,15 @@
 
             ###################################### Get_circlize_plot #######################################
 
             grouping_file_re = '%s_MetaCHIP_wd/%s_%s*_grouping.txt' % (output_prefix, output_prefix, detection_rank_list)
             grouping_file = [os.path.basename(file_name) for file_name in glob.glob(grouping_file_re)][0]
             taxon_rank_num = grouping_file[len(output_prefix) + 1:].split('_')[0]
             pwd_grouping_file =         '%s_MetaCHIP_wd/%s'                         % (output_prefix, grouping_file)
-            pwd_plot_circos =           '%s/%s_%s_HGT_circos.png'                   % (pwd_MetaCHIP_op_folder, output_prefix, taxon_rank_num)
+            pwd_plot_circos =           '%s/%s_%s_HGT_circos.pdf'                   % (pwd_MetaCHIP_op_folder, output_prefix, taxon_rank_num)
 
             taxon_to_group_id_dict = {}
             for group in open(pwd_grouping_file):
                 group_id = group.strip().split(',')[0]
                 group_taxon = group.strip().split(',')[2]
                 if group_id not in taxon_to_group_id_dict:
                     taxon_to_group_id_dict[group_id] = group_taxon
@@ -3621,15 +3621,15 @@
 
             for detection_rank in detection_rank_list:
 
                 grouping_file_re = '%s_MetaCHIP_wd/%s_%s*_grouping.txt' % (output_prefix, output_prefix, detection_rank)
                 grouping_file = [os.path.basename(file_name) for file_name in glob.glob(grouping_file_re)][0]
                 taxon_rank_num = grouping_file[len(output_prefix) + 1:].split('_')[0]
                 pwd_grouping_file =         '%s_MetaCHIP_wd/%s'                         % (output_prefix, grouping_file)
-                pwd_plot_circos =           '%s/%s_%s_HGT_circos.png'                   % (pwd_combined_prediction_folder, output_prefix, taxon_rank_num)
+                pwd_plot_circos =           '%s/%s_%s_HGT_circos.pdf'                   % (pwd_combined_prediction_folder, output_prefix, taxon_rank_num)
 
                 # get genome to taxon dict
                 genome_to_taxon_dict = {}
                 for genome in open(pwd_grouping_file):
                     genome_name = genome.strip().split(',')[1]
                     genome_taxon = genome.strip().split(',')[2]
                     genome_to_taxon_dict[genome_name] = genome_taxon
@@ -3772,15 +3772,15 @@
 
         print('%s Get circlize plot at rank %s' % (datetime.now().strftime(time_format), detection_rank))
 
         grouping_file_re = '%s_MetaCHIP_wd/%s_%s*_grouping.txt' % (output_prefix, output_prefix, detection_rank)
         grouping_file = [os.path.basename(file_name) for file_name in glob.glob(grouping_file_re)][0]
         taxon_rank_num = grouping_file[len(output_prefix) + 1:].split('_')[0]
         pwd_grouping_file =         '%s_MetaCHIP_wd/%s'                         % (output_prefix, grouping_file)
-        pwd_plot_circos =           '%s/%s_%s_HGT_circos.png'                   % (pwd_combined_prediction_folder, output_prefix, taxon_rank_num)
+        pwd_plot_circos =           '%s/%s_%s_HGT_circos.pdf'                   % (pwd_combined_prediction_folder, output_prefix, taxon_rank_num)
 
         # get genome to taxon dict
         genome_to_taxon_dict = {}
         for genome in open(pwd_grouping_file):
             genome_name = genome.strip().split(',')[1]
             genome_taxon = genome.strip().split(',')[2]
             genome_to_taxon_dict[genome_name] = genome_taxon
```

### Comparing `MetaCHIP-1.9.6/MetaCHIP/BP_rewrote.py` & `MetaCHIP-1.9.7/MetaCHIP/BP_rewrote.py`

 * *Files identical despite different names*

### Comparing `MetaCHIP-1.9.6/MetaCHIP/MetaCHIP_add_group_to_tree.R` & `MetaCHIP-1.9.7/MetaCHIP/MetaCHIP_add_group_to_tree.R`

 * *Files identical despite different names*

### Comparing `MetaCHIP-1.9.6/MetaCHIP/MetaCHIP_circos_HGT.R` & `MetaCHIP-1.9.7/MetaCHIP/MetaCHIP_circos_HGT.R`

 * *Files identical despite different names*

### Comparing `MetaCHIP-1.9.6/MetaCHIP/MetaCHIP_config.py` & `MetaCHIP-1.9.7/MetaCHIP/MetaCHIP_config.py`

 * *Files identical despite different names*

### Comparing `MetaCHIP-1.9.6/MetaCHIP/MetaCHIP_phylo.hmm` & `MetaCHIP-1.9.7/MetaCHIP/MetaCHIP_phylo.hmm`

 * *Files identical despite different names*

### Comparing `MetaCHIP-1.9.6/MetaCHIP/PI.py` & `MetaCHIP-1.9.7/MetaCHIP/PI.py`

 * *Files identical despite different names*

### Comparing `MetaCHIP-1.9.6/MetaCHIP/PI_rewrote.py` & `MetaCHIP-1.9.7/MetaCHIP/PI_rewrote.py`

 * *Files identical despite different names*

### Comparing `MetaCHIP-1.9.6/MetaCHIP/Ranger-DTL-Dated.linux` & `MetaCHIP-1.9.7/MetaCHIP/Ranger-DTL-Dated.linux`

 * *Files identical despite different names*

### Comparing `MetaCHIP-1.9.6/MetaCHIP/Ranger-DTL-Dated.mac` & `MetaCHIP-1.9.7/MetaCHIP/Ranger-DTL-Dated.mac`

 * *Files identical despite different names*

### Comparing `MetaCHIP-1.9.6/MetaCHIP/SankeyTaxon.py` & `MetaCHIP-1.9.7/MetaCHIP/SankeyTaxon.py`

 * *Files identical despite different names*

### Comparing `MetaCHIP-1.9.6/MetaCHIP/circos_HGT.py` & `MetaCHIP-1.9.7/MetaCHIP/circos_HGT.py`

 * *Files identical despite different names*

### Comparing `MetaCHIP-1.9.6/MetaCHIP/filter_HGT.py` & `MetaCHIP-1.9.7/MetaCHIP/filter_HGT.py`

 * *Files identical despite different names*

### Comparing `MetaCHIP-1.9.6/MetaCHIP/get_SCG_tree.py` & `MetaCHIP-1.9.7/MetaCHIP/get_SCG_tree.py`

 * *Files identical despite different names*

### Comparing `MetaCHIP-1.9.6/MetaCHIP/get_flk_gene_functions.py` & `MetaCHIP-1.9.7/MetaCHIP/get_flk_gene_functions.py`

 * *Files identical despite different names*

### Comparing `MetaCHIP-1.9.6/MetaCHIP/rename_seqs.py` & `MetaCHIP-1.9.7/MetaCHIP/rename_seqs.py`

 * *Files identical despite different names*

### Comparing `MetaCHIP-1.9.6/MetaCHIP/test_1.py` & `MetaCHIP-1.9.7/MetaCHIP/test_1.py`

 * *Files identical despite different names*

### Comparing `MetaCHIP-1.9.6/MetaCHIP/tuning_full_length_and_end_match.py` & `MetaCHIP-1.9.7/MetaCHIP/tuning_full_length_and_end_match.py`

 * *Files identical despite different names*

### Comparing `MetaCHIP-1.9.6/MetaCHIP/update_hmms.py` & `MetaCHIP-1.9.7/MetaCHIP/update_hmms.py`

 * *Files identical despite different names*

### Comparing `MetaCHIP-1.9.6/MetaCHIP.egg-info/PKG-INFO` & `MetaCHIP-1.9.7/MetaCHIP.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: MetaCHIP
-Version: 1.9.6
+Version: 1.9.7
 Summary: HGT detection pipeline
 Home-page: https://github.com/songweizhi/MetaCHIP
 Author: Weizhi Song, Torsten Thomas
 Author-email: songwz03@gmail.com
 License: GPL3+
 Description:
```

### Comparing `MetaCHIP-1.9.6/MetaCHIP.egg-info/SOURCES.txt` & `MetaCHIP-1.9.7/MetaCHIP.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `MetaCHIP-1.9.6/PKG-INFO` & `MetaCHIP-1.9.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: MetaCHIP
-Version: 1.9.6
+Version: 1.9.7
 Summary: HGT detection pipeline
 Home-page: https://github.com/songweizhi/MetaCHIP
 Author: Weizhi Song, Torsten Thomas
 Author-email: songwz03@gmail.com
 License: GPL3+
 Description:
```

### Comparing `MetaCHIP-1.9.6/README.md` & `MetaCHIP-1.9.7/README.md`

 * *Files identical despite different names*

### Comparing `MetaCHIP-1.9.6/bin/MetaCHIP` & `MetaCHIP-1.9.7/bin/MetaCHIP`

 * *Files identical despite different names*

### Comparing `MetaCHIP-1.9.6/setup.py` & `MetaCHIP-1.9.7/setup.py`

 * *Files identical despite different names*

