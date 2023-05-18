# Comparing `tmp/secmarker-0.4.1.tar.gz` & `tmp/secmarker-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "secmarker-0.4.1.tar", last modified: Fri May 12 14:16:53 2023, max compression
+gzip compressed data, was "secmarker-1.0.0.tar", last modified: Thu May 18 13:43:11 2023, max compression
```

## Comparing `secmarker-0.4.1.tar` & `secmarker-1.0.0.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwx---   0 mserrazanetti (32148) CRG_Lab_Roderic_Guigo (32000)        0 2023-05-12 14:16:53.703851 secmarker-0.4.1/
--rwxrwxr--   0 mserrazanetti (32148) CRG_Lab_Roderic_Guigo (32000)     1076 2023-05-12 08:41:40.000000 secmarker-0.4.1/LICENSE
--rwxrwx---   0 mserrazanetti (32148) CRG_Lab_Roderic_Guigo (32000)       31 2023-05-12 08:42:35.000000 secmarker-0.4.1/MANIFEST.in
--rwxrwx---   0 mserrazanetti (32148) CRG_Lab_Roderic_Guigo (32000)     2748 2023-05-12 14:16:53.705931 secmarker-0.4.1/PKG-INFO
--rwxrwxr--   0 mserrazanetti (32148) CRG_Lab_Roderic_Guigo (32000)     2312 2023-05-12 08:42:56.000000 secmarker-0.4.1/README.md
--rwxrwxr--   0 mserrazanetti (32148) CRG_Lab_Roderic_Guigo (32000)      104 2023-05-12 08:41:40.000000 secmarker-0.4.1/pyproject.toml
--rwxrwxr--   0 mserrazanetti (32148) CRG_Lab_Roderic_Guigo (32000)      773 2023-05-12 14:16:53.711584 secmarker-0.4.1/setup.cfg
--rwxrwxr--   0 mserrazanetti (32148) CRG_Lab_Roderic_Guigo (32000)       69 2023-05-12 10:24:50.000000 secmarker-0.4.1/setup.py
-drwxrwx---   0 mserrazanetti (32148) CRG_Lab_Roderic_Guigo (32000)        0 2023-05-12 14:16:53.404952 secmarker-0.4.1/src/
-drwxrwx---   0 mserrazanetti (32148) CRG_Lab_Roderic_Guigo (32000)        0 2023-05-12 14:16:53.500626 secmarker-0.4.1/src/secmarker/
--rwxrwx---   0 mserrazanetti (32148) CRG_Lab_Roderic_Guigo (32000)   343996 2023-05-12 13:47:00.000000 secmarker-0.4.1/src/secmarker/MMlib3.py
--rwxrwx---   0 mserrazanetti (32148) CRG_Lab_Roderic_Guigo (32000)      185 2023-05-12 11:03:50.000000 secmarker-0.4.1/src/secmarker/__init__.py
--rwxrwx---   0 mserrazanetti (32148) CRG_Lab_Roderic_Guigo (32000)       22 2023-05-12 14:15:12.000000 secmarker-0.4.1/src/secmarker/_version.py
--rwxrwx---   0 mserrazanetti (32148) CRG_Lab_Roderic_Guigo (32000)    89186 2023-05-12 13:25:21.000000 secmarker-0.4.1/src/secmarker/argparse.py
-drwxrwx---   0 mserrazanetti (32148) CRG_Lab_Roderic_Guigo (32000)        0 2023-05-12 14:16:53.681814 secmarker-0.4.1/src/secmarker/models/
--rwxrwxr--   0 mserrazanetti (32148) CRG_Lab_Roderic_Guigo (32000)     2638 2023-05-12 08:41:40.000000 secmarker-0.4.1/src/secmarker/models/archaea.stk
--rwxrwxr--   0 mserrazanetti (32148) CRG_Lab_Roderic_Guigo (32000)    61755 2023-05-12 08:41:40.000000 secmarker-0.4.1/src/secmarker/models/archaea.stk.cm
--rwxrwxr--   0 mserrazanetti (32148) CRG_Lab_Roderic_Guigo (32000)    35205 2023-05-12 08:41:40.000000 secmarker-0.4.1/src/secmarker/models/bacteria.stk
--rwxrwxr--   0 mserrazanetti (32148) CRG_Lab_Roderic_Guigo (32000)    63662 2023-05-12 08:41:40.000000 secmarker-0.4.1/src/secmarker/models/bacteria.stk.cm
--rwxrwxr--   0 mserrazanetti (32148) CRG_Lab_Roderic_Guigo (32000)    17505 2023-05-12 08:41:40.000000 secmarker-0.4.1/src/secmarker/models/eukaryota.stk
--rwxrwxr--   0 mserrazanetti (32148) CRG_Lab_Roderic_Guigo (32000)    59751 2023-05-12 08:41:40.000000 secmarker-0.4.1/src/secmarker/models/eukaryota.stk.cm
--rwxrwxr--   0 mserrazanetti (32148) CRG_Lab_Roderic_Guigo (32000)   190157 2023-05-12 08:41:40.000000 secmarker-0.4.1/src/secmarker/models/tRNAsec_db.cm
--rwxrwxr--   0 mserrazanetti (32148) CRG_Lab_Roderic_Guigo (32000)    55348 2023-05-12 08:41:40.000000 secmarker-0.4.1/src/secmarker/models/tRNAsec_db.stk
--rwxrwxr--   0 mserrazanetti (32148) CRG_Lab_Roderic_Guigo (32000)     4968 2023-05-12 10:25:14.000000 secmarker-0.4.1/src/secmarker/plot_tRNA.py
--rwxrwxr-x   0 mserrazanetti (32148) CRG_Lab_Roderic_Guigo (32000)    31058 2023-05-12 14:15:22.000000 secmarker-0.4.1/src/secmarker/secmarker_lib.py
-drwxrwx---   0 mserrazanetti (32148) CRG_Lab_Roderic_Guigo (32000)        0 2023-05-12 14:16:53.542975 secmarker-0.4.1/src/secmarker.egg-info/
--rwxrwx---   0 mserrazanetti (32148) CRG_Lab_Roderic_Guigo (32000)     2748 2023-05-12 14:16:53.000000 secmarker-0.4.1/src/secmarker.egg-info/PKG-INFO
--rwxrwx---   0 mserrazanetti (32148) CRG_Lab_Roderic_Guigo (32000)      691 2023-05-12 14:16:53.000000 secmarker-0.4.1/src/secmarker.egg-info/SOURCES.txt
--rwxrwx---   0 mserrazanetti (32148) CRG_Lab_Roderic_Guigo (32000)        1 2023-05-12 14:16:53.000000 secmarker-0.4.1/src/secmarker.egg-info/dependency_links.txt
--rwxrwx---   0 mserrazanetti (32148) CRG_Lab_Roderic_Guigo (32000)       25 2023-05-12 14:16:53.000000 secmarker-0.4.1/src/secmarker.egg-info/requires.txt
--rwxrwx---   0 mserrazanetti (32148) CRG_Lab_Roderic_Guigo (32000)       10 2023-05-12 14:16:53.000000 secmarker-0.4.1/src/secmarker.egg-info/top_level.txt
+drwxrwx---   0 mserrazanetti (32148) CRG_Lab_Roderic_Guigo (32000)        0 2023-05-18 13:43:11.283935 secmarker-1.0.0/
+-rwxrwxr--   0 mserrazanetti (32148) CRG_Lab_Roderic_Guigo (32000)     1076 2023-05-18 12:39:42.000000 secmarker-1.0.0/LICENSE
+-rwxrwxr--   0 mserrazanetti (32148) CRG_Lab_Roderic_Guigo (32000)       31 2023-05-18 12:39:42.000000 secmarker-1.0.0/MANIFEST.in
+-rwxrwx---   0 mserrazanetti (32148) CRG_Lab_Roderic_Guigo (32000)      435 2023-05-18 13:43:11.285584 secmarker-1.0.0/PKG-INFO
+-rwxrwxr--   0 mserrazanetti (32148) CRG_Lab_Roderic_Guigo (32000)     2343 2023-05-18 13:31:37.000000 secmarker-1.0.0/README
+-rwxrwxr--   0 mserrazanetti (32148) CRG_Lab_Roderic_Guigo (32000)      104 2023-05-18 12:39:42.000000 secmarker-1.0.0/pyproject.toml
+-rwxrwxr--   0 mserrazanetti (32148) CRG_Lab_Roderic_Guigo (32000)      773 2023-05-18 13:43:11.291182 secmarker-1.0.0/setup.cfg
+-rwxrwxr-x   0 mserrazanetti (32148) CRG_Lab_Roderic_Guigo (32000)       69 2023-05-18 12:39:42.000000 secmarker-1.0.0/setup.py
+drwxrwx---   0 mserrazanetti (32148) CRG_Lab_Roderic_Guigo (32000)        0 2023-05-18 13:43:11.055913 secmarker-1.0.0/src/
+drwxrwx---   0 mserrazanetti (32148) CRG_Lab_Roderic_Guigo (32000)        0 2023-05-18 13:43:11.165334 secmarker-1.0.0/src/secmarker/
+-rwxrwxr--   0 mserrazanetti (32148) CRG_Lab_Roderic_Guigo (32000)   343996 2023-05-18 12:39:42.000000 secmarker-1.0.0/src/secmarker/MMlib3.py
+-rwxrwxr--   0 mserrazanetti (32148) CRG_Lab_Roderic_Guigo (32000)      185 2023-05-18 12:39:43.000000 secmarker-1.0.0/src/secmarker/__init__.py
+-rwxrwxr--   0 mserrazanetti (32148) CRG_Lab_Roderic_Guigo (32000)       22 2023-05-18 13:33:14.000000 secmarker-1.0.0/src/secmarker/_version.py
+-rwxrwxr--   0 mserrazanetti (32148) CRG_Lab_Roderic_Guigo (32000)    89186 2023-05-18 12:39:43.000000 secmarker-1.0.0/src/secmarker/argparse.py
+drwxrwx---   0 mserrazanetti (32148) CRG_Lab_Roderic_Guigo (32000)        0 2023-05-18 13:43:11.276589 secmarker-1.0.0/src/secmarker/models/
+-rwxrwxr--   0 mserrazanetti (32148) CRG_Lab_Roderic_Guigo (32000)     2638 2023-05-18 12:39:43.000000 secmarker-1.0.0/src/secmarker/models/archaea.stk
+-rwxrwxr--   0 mserrazanetti (32148) CRG_Lab_Roderic_Guigo (32000)    61755 2023-05-18 12:39:43.000000 secmarker-1.0.0/src/secmarker/models/archaea.stk.cm
+-rwxrwxr--   0 mserrazanetti (32148) CRG_Lab_Roderic_Guigo (32000)    35205 2023-05-18 12:39:43.000000 secmarker-1.0.0/src/secmarker/models/bacteria.stk
+-rwxrwxr--   0 mserrazanetti (32148) CRG_Lab_Roderic_Guigo (32000)    63662 2023-05-18 12:39:43.000000 secmarker-1.0.0/src/secmarker/models/bacteria.stk.cm
+-rwxrwxr--   0 mserrazanetti (32148) CRG_Lab_Roderic_Guigo (32000)    17505 2023-05-18 12:39:43.000000 secmarker-1.0.0/src/secmarker/models/eukaryota.stk
+-rwxrwxr--   0 mserrazanetti (32148) CRG_Lab_Roderic_Guigo (32000)    59751 2023-05-18 12:39:43.000000 secmarker-1.0.0/src/secmarker/models/eukaryota.stk.cm
+-rwxrwxr--   0 mserrazanetti (32148) CRG_Lab_Roderic_Guigo (32000)   190157 2023-05-18 12:39:43.000000 secmarker-1.0.0/src/secmarker/models/tRNAsec_db.cm
+-rwxrwxr--   0 mserrazanetti (32148) CRG_Lab_Roderic_Guigo (32000)    55348 2023-05-18 12:39:43.000000 secmarker-1.0.0/src/secmarker/models/tRNAsec_db.stk
+-rwxrwxr--   0 mserrazanetti (32148) CRG_Lab_Roderic_Guigo (32000)     4968 2023-05-18 12:39:43.000000 secmarker-1.0.0/src/secmarker/plot_tRNA.py
+-rwxrwxr--   0 mserrazanetti (32148) CRG_Lab_Roderic_Guigo (32000)    31104 2023-05-18 13:32:58.000000 secmarker-1.0.0/src/secmarker/secmarker_lib.py
+drwxrwx---   0 mserrazanetti (32148) CRG_Lab_Roderic_Guigo (32000)        0 2023-05-18 13:43:11.203164 secmarker-1.0.0/src/secmarker.egg-info/
+-rwxrwx---   0 mserrazanetti (32148) CRG_Lab_Roderic_Guigo (32000)      435 2023-05-18 13:43:10.000000 secmarker-1.0.0/src/secmarker.egg-info/PKG-INFO
+-rwxrwx---   0 mserrazanetti (32148) CRG_Lab_Roderic_Guigo (32000)      688 2023-05-18 13:43:11.000000 secmarker-1.0.0/src/secmarker.egg-info/SOURCES.txt
+-rwxrwx---   0 mserrazanetti (32148) CRG_Lab_Roderic_Guigo (32000)        1 2023-05-18 13:43:11.000000 secmarker-1.0.0/src/secmarker.egg-info/dependency_links.txt
+-rwxrwx---   0 mserrazanetti (32148) CRG_Lab_Roderic_Guigo (32000)       25 2023-05-18 13:43:11.000000 secmarker-1.0.0/src/secmarker.egg-info/requires.txt
+-rwxrwx---   0 mserrazanetti (32148) CRG_Lab_Roderic_Guigo (32000)       10 2023-05-18 13:43:11.000000 secmarker-1.0.0/src/secmarker.egg-info/top_level.txt
```

### Comparing `secmarker-0.4.1/LICENSE` & `secmarker-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `secmarker-0.4.1/PKG-INFO` & `secmarker-1.0.0/README`

 * *Files 18% similar despite different names*

```diff
@@ -1,67 +1,52 @@
-Metadata-Version: 2.1
-Name: secmarker
-Version: 0.4.1
-Summary: secmarker description
-Home-page: https://github.com/pypa/sampleproject
-Author: Matteo Serrazanetti
-Author-email: matteoserrazanetti@gmail.com
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # secmarker
+
 Secmarker is a search tool for selenocysteine tRNA (tRNA-Sec) identification. 
-The presence of tRNA-Sec in a genome indicates the use of selenocysteine by the organism. 
+The presence of tRNA-Sec in a genome indicates the use of selenocysteine (SeC) by the organism. 
 Old version was written in python2 and now it's written in python3
 
-## SECMARKER 0.4
+# SECMARKER 0.4
 
 * Web server
   A SecMarker web server is available for online analysis:
   http://secmarker.crg.es/
 
 * Publication
- Didac Santesmasses, Marco Mariotti and Roderic Guigó. Computational identification of the selenocysteine tRNA (tRNASec) in genomes. PLoS Comput Biol. 2017 Feb 13;13(2):e1005383. doi: 10.1371/journal.pcbi.1005383. 
+  Didac Santesmasses, Marco Mariotti and Roderic Guigó. Computational identification of the selenocysteine tRNA (tRNASec) in genomes. PLoS Comput Biol. 2017 Feb 13;13(2):e1005383. doi: 10.1371/journal.pcbi.1005383. 
 
 * Dependencies
   cmsearch and esl-sfetch from the Infernal package (http://infernal.janelia.org/), specifically, version => 1.1 is required.
   RNAplot from ViennaRNA package (http://www.tbi.univie.ac.at/RNA/), version >= 2.0 is known to work fine.
 
 * Installation:
-  In order to use Secmarker run the following comands (where x.x corresponds to the current version):
-
-  tar xfz secmarker-x.x.tar.gz
-  cd secmarker-x.x
-  ./setup.py
-  ./run_test.py
+  In order to use Secmarker run the following comands:
 
+  conda create -y -n secmarker
+  conda activate secmarker
+  conda install -c bioconda –c matteoserrazanetti secmarker 
 
-* Running Secmarker.py
-usage: Secmarker.py [-h] -t TARGET [-o O] [-plot] [-T T] [-F F] [-cpu CPU]
+* Running secmarker
+  usage: secmarker [-h] -t TARGET [-o O] [-plot] [-T T] [-F F] [-cpu CPU]
                     [-cca] [-AT12] [-O O]
 
-search for selenocysteine tRNA (tRNA-Sec), marker of Sec trait
+  search for selenocysteine tRNA (tRNA-Sec), marker of Sec trait
 
-optional arguments:
-  -h, --help            show this help message and exit
-  -t TARGET, --target TARGET
-                        target nucleotide sequence
-  -o O                  output folder
-  -plot                 generate the tRNA plot(s). For each tRNA prediction,
-                        two files (.png and .ps) will be generated in the
-                        folder images/
-  -T T, --infernal_score T
-                        score threshold used by cmsearch (Infernal score)
-  -F F, --filtering_score F
-                        score threshold used to filter tRNAs. If the tRNA has
-                        the UCA anticodon or a G73, -T is used for filtering
-  -cpu CPU              number of available CPUs [default 1]
-  -cca                  include the 3 residues downstream the discriminator
-                        base if available (to check if the CCA sequence is
+  optional arguments:
+    -h, --help            show this help message and exit
+    -t TARGET, --target TARGET
+                          target nucleotide sequence
+    -o O                  output folder
+    -plot                 generate the tRNA plot(s). For each tRNA prediction,
+                          two files (.png and .ps) will be generated in the
+                          folder images/
+    -T T, --infernal_score T
+                          score threshold used by cmsearch (Infernal score)
+    -F F, --filtering_score F
+                          score threshold used to filter tRNAs. If the tRNA has
+                          the UCA anticodon or a G73, -T is used for filtering
+    -cpu CPU              number of available CPUs [default 1]
+    -cca                  include the 3 residues downstream the discriminator
+                          base if available (to check if the CCA sequence is
                         encoded in the sequence)
   -AT12                 force a 12 bp AT-stem, that is a 7/5 fold tRNA
   -O O, --options O     additional options for cmsearch
```

### Comparing `secmarker-0.4.1/setup.cfg` & `secmarker-1.0.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `secmarker-0.4.1/src/secmarker/MMlib3.py` & `secmarker-1.0.0/src/secmarker/MMlib3.py`

 * *Files identical despite different names*

### Comparing `secmarker-0.4.1/src/secmarker/argparse.py` & `secmarker-1.0.0/src/secmarker/argparse.py`

 * *Files identical despite different names*

### Comparing `secmarker-0.4.1/src/secmarker/models/archaea.stk` & `secmarker-1.0.0/src/secmarker/models/archaea.stk`

 * *Files identical despite different names*

### Comparing `secmarker-0.4.1/src/secmarker/models/archaea.stk.cm` & `secmarker-1.0.0/src/secmarker/models/archaea.stk.cm`

 * *Files identical despite different names*

### Comparing `secmarker-0.4.1/src/secmarker/models/bacteria.stk` & `secmarker-1.0.0/src/secmarker/models/bacteria.stk`

 * *Files identical despite different names*

### Comparing `secmarker-0.4.1/src/secmarker/models/bacteria.stk.cm` & `secmarker-1.0.0/src/secmarker/models/bacteria.stk.cm`

 * *Files identical despite different names*

### Comparing `secmarker-0.4.1/src/secmarker/models/eukaryota.stk` & `secmarker-1.0.0/src/secmarker/models/eukaryota.stk`

 * *Files identical despite different names*

### Comparing `secmarker-0.4.1/src/secmarker/models/eukaryota.stk.cm` & `secmarker-1.0.0/src/secmarker/models/eukaryota.stk.cm`

 * *Files identical despite different names*

### Comparing `secmarker-0.4.1/src/secmarker/models/tRNAsec_db.cm` & `secmarker-1.0.0/src/secmarker/models/tRNAsec_db.cm`

 * *Files identical despite different names*

### Comparing `secmarker-0.4.1/src/secmarker/models/tRNAsec_db.stk` & `secmarker-1.0.0/src/secmarker/models/tRNAsec_db.stk`

 * *Files identical despite different names*

### Comparing `secmarker-0.4.1/src/secmarker/plot_tRNA.py` & `secmarker-1.0.0/src/secmarker/plot_tRNA.py`

 * *Files identical despite different names*

### Comparing `secmarker-0.4.1/src/secmarker/secmarker_lib.py` & `secmarker-1.0.0/src/secmarker/secmarker_lib.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,16 +16,15 @@
 #    GNU General Public License for more details.
 #
 #    You should have received a copy of the GNU General Public License
 #    along with Secmarker.  If not, see <http://www.gnu.org/licenses/>.
 #
 ##########################################################################
 
-__VERSION__="secmarker-0.4.1" 
-
+from ._version import __version__
 import sys,os
 from . import argparse
 sys.path.insert(0, os.path.dirname(os.path.realpath(__file__)) +'/library')
 from .MMlib3 import *
 os.environ['PATH'] = os.path.dirname(os.path.realpath(__file__)) +'/bin:'+os.environ['PATH']
 
 def get_parser():
@@ -740,11 +739,12 @@
         if b[0]:
             if 'command not found' in b[1]:
                 raise Exception('ERROR: RNAplot program not available')
             else:
                 raise Exception(b[1])
 
 if __name__=='__main__':
+    print("secmarker v" + str(__version__))
     parser = get_parser()
     args = parser.parse_args()
     main(args)
```

### Comparing `secmarker-0.4.1/src/secmarker.egg-info/SOURCES.txt` & `secmarker-1.0.0/src/secmarker.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 LICENSE
 MANIFEST.in
-README.md
+README
 pyproject.toml
 setup.cfg
 setup.py
 src/secmarker/MMlib3.py
 src/secmarker/__init__.py
 src/secmarker/_version.py
 src/secmarker/argparse.py
```

