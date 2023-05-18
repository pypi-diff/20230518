# Comparing `tmp/anospp_analysis-0.1.3.tar.gz` & `tmp/anospp_analysis-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "anospp_analysis-0.1.3.tar", max compression
+gzip compressed data, was "anospp_analysis-0.2.0.tar", max compression
```

## Comparing `anospp_analysis-0.1.3.tar` & `anospp_analysis-0.2.0.tar`

### file list

```diff
@@ -1,9 +1,13 @@
--rw-r--r--   0        0        0     1067 2023-01-24 21:08:31.753757 anospp_analysis-0.1.3/LICENSE
--rw-r--r--   0        0        0     2498 2023-04-05 09:27:05.836973 anospp_analysis-0.1.3/README.md
--rw-r--r--   0        0        0        1 2023-03-28 09:17:49.841709 anospp_analysis-0.1.3/anospp_analysis/__init__.py
--rw-r--r--   0        0        0       44 2023-03-27 08:59:31.888140 anospp_analysis-0.1.3/anospp_analysis/anospp-analysis.code-workspace
--rw-r--r--   0        0        0     4457 2023-04-05 09:27:05.840619 anospp_analysis-0.1.3/anospp_analysis/prep.py
--rw-r--r--   0        0        0    10841 2023-04-05 09:27:05.842623 anospp_analysis-0.1.3/anospp_analysis/qc.py
--rw-r--r--   0        0        0    10190 2023-04-05 09:27:05.844040 anospp_analysis-0.1.3/anospp_analysis/util.py
--rw-r--r--   0        0        0      562 2023-04-05 09:27:05.851653 anospp_analysis-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     3040 1970-01-01 00:00:00.000000 anospp_analysis-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-01-24 21:08:31.753757 anospp_analysis-0.2.0/LICENSE
+-rw-r--r--   0        0        0     3134 2023-05-18 12:21:59.391252 anospp_analysis-0.2.0/README.md
+-rw-r--r--   0        0        0       21 2023-05-18 12:21:59.392047 anospp_analysis-0.2.0/anospp_analysis/__init__.py
+-rw-r--r--   0        0        0     6776 2023-05-18 09:50:03.443460 anospp_analysis-0.2.0/anospp_analysis/iplot.py
+-rw-r--r--   0        0        0    26194 2023-05-18 12:21:59.393337 anospp_analysis-0.2.0/anospp_analysis/nn.py
+-rw-r--r--   0        0        0    34887 2023-05-18 12:21:59.395203 anospp_analysis-0.2.0/anospp_analysis/plasm.py
+-rw-r--r--   0        0        0     4457 2023-04-05 09:27:05.840619 anospp_analysis-0.2.0/anospp_analysis/prep.py
+-rw-r--r--   0        0        0    10858 2023-05-18 12:21:59.397129 anospp_analysis-0.2.0/anospp_analysis/qc.py
+-rw-r--r--   0        0        0     8737 2023-05-18 12:05:29.523105 anospp_analysis-0.2.0/anospp_analysis/test_functions_vae.py
+-rw-r--r--   0        0        0    11738 2023-05-18 12:21:59.398743 anospp_analysis-0.2.0/anospp_analysis/util.py
+-rw-r--r--   0        0        0    27689 2023-05-18 12:05:29.523497 anospp_analysis-0.2.0/anospp_analysis/vae.py
+-rw-r--r--   0        0        0      744 2023-05-18 12:21:59.401753 anospp_analysis-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     3730 1970-01-01 00:00:00.000000 anospp_analysis-0.2.0/PKG-INFO
```

### Comparing `anospp_analysis-0.1.3/LICENSE` & `anospp_analysis-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `anospp_analysis-0.1.3/README.md` & `anospp_analysis-0.2.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,96 +1,123 @@
 # anospp-analysis
 
 Python package for ANOSPP data analysis
 
-ANOSPP is the multiplexed amplicon sequencing assay for Anopheles mosquito species identification and Plasmodium detection. This repository contains the code for analysis of the sequencing results pre-processed with [nf-core ampliseq](https://nf-co.re/ampliseq) pipeline. 
+ANOSPP is the multiplexed amplicon sequencing assay for Anopheles mosquito species identification and Plasmodium detection. This repository contains the code for analysis of the sequencing results pre-processed with [nf-core ampliseq](https://nf-co.re/ampliseq) pipeline.
+
+## Installation
+
+For released version
+
+```bash
+conda install -c bioconda anospp-analysis
+```
+
+For development setup, see instructions below
 
 ## Usage
 
 Key analysis steps are implemented as standalone scripts:
+
 - `anospp-prep` takes DADA2 output files and targets primer sequences, demultiplexes the amplicons and yields haplotypes table
-- `anospp-qc` takes haplotypes table, DADA2 stats table and samples manifest and produces QC plots 
+- `anospp-qc` takes haplotypes table, DADA2 stats table and samples manifest and produces QC plots
+- `anospp-plasm` blasts Plasmodium sequences against reference dataset to determine species and infer sample infection status
+- `anospp-nn` compares k-mer profiles of mosquito targets against a reference dataset and provides probabilistic species calls
+- `anospp-vae` provides finer scale species prediction for An. gambiae complex with VAE projection
 
 ## Development
 
 ### Setup
 
 Installation is hybrid with conda + poetry:
-```
+
+```bash
 git clone git@github.com:malariagen/anospp-analysis.git
 cd anospp-analysis
 mamba env create -f environment.yml
-conda activate anospp_analysis
+conda activate anospp_analysis_dev
 poetry install
 ```
 
-Activate development environment:
-```
-poetry shell
-```
-
 ### Usage & testing
 
 The code in this repository can be accessed via wrapper scripts:
-```
+
+```bash
 anospp-qc \
     --haplotypes test_data/haplotypes.tsv \
     --samples test_data/samples.csv \
     --stats test_data/stats.tsv \
     --outdir test_data/qc
 ```
 
 Besides, individual components are available as a python API:
-```
+
+```bash
 $ python
 >>> from anospp_analysis.util import *
 >>> PLASM_TARGETS
 ['P1', 'P2']
 ```
 
-Automated testing & CI
+TODO Automated testing & CI
 
 ### Adding Python deps
 
 Introducing python dependencies should be done via poetry:
-```
+
+```bash
 poetry add package_name
-``` 
+```
+
 This should update both `pyproject.toml` and `poetry.lock` files
 
 If the package should be used in development environment only, use
-```
+
+```bash
 poetry add package_name --dev
 ```
 
+To update environment after changes made to `pyproject.toml` and/or `poetry.lock`
+
+```bash
+poetry install
+```
+
 ### Adding non-Python deps
 
-Introducing non-python dependencies should be done via conda: edit `environment.yml`, 
+Introducing non-python dependencies should be done via conda: edit `environment.yml`,
 then re-create the conda environment and poetry deps:
-```
+
+```bash
 mamba env create -f environment.yml
 conda activate anospp_analysis
 poetry install
 ```
 
-Changes in conda environment might also introduce changes to the python installation, 
+Changes in conda environment might also introduce changes to the python installation,
 in which case one should update poetry lock file
-```
+
+```bash
 poetry lock
 ```
 
 ## Release checklist
 
 While in dev branch
+
 - test functionality (TODO CI)
+- bump version in module init
 - bump version in `pyproject.toml`
 
-Then
+Then,
+
 - merge into master
 - github release
 - pypi release
 
 Conda recipe update `conda.recipe/meta.yaml`:
+
 - check deps vs `environment.yaml` and `pyproject.toml`
-- bump version  
+- bump version in meta yaml  
 - update sha256 from pypi project (download files > tar.gz > view hashes)
 - test conda recipe with `bioconda-utils build --git-range master` vs bioconda-recipes
```

### Comparing `anospp_analysis-0.1.3/anospp_analysis/prep.py` & `anospp_analysis-0.2.0/anospp_analysis/prep.py`

 * *Files identical despite different names*

### Comparing `anospp_analysis-0.1.3/anospp_analysis/qc.py` & `anospp_analysis-0.2.0/anospp_analysis/qc.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,16 +10,15 @@
 
 DADA2_COLS = OrderedDict([
     ('input','removed by filterAndTrim'), 
     ('filtered','removed by denoising'),
     ('denoised','removed by merging'), 
     ('merged','removde by rmchimera'), 
     ('nonchim','removed by post-filtering'),
-    ('final','retained') 
-
+    ('final','retained')
 ])
 
 def plot_target_balance(hap_df):
 
     logging.info('plotting targets balance')
 
     reads_per_sample = hap_df.groupby(['sample_id','target'])['reads'].sum().reset_index()
@@ -177,15 +176,15 @@
 def plot_sample_success(comb_stats_df):
 
     logging.info('plotting sample success')
 
     fig, axs = plt.subplots(1,2,figsize=(12,6))
     for col, ax in zip(('final_log10','filter_rate'), axs):
         sns.scatterplot(data=comb_stats_df,
-                x='mosq_targets_recovered',
+                x='raw_mosq_targets_recovered',
                 y=col,
                 hue='plate_id',
                 alpha=.5, 
                 ax=ax)
         ax.axvline(30, alpha=.5)
     axs[0].axhline(3, alpha=.5)
     axs[1].axhline(.5, alpha=.5)
@@ -228,16 +227,16 @@
 
     setup_logging(verbose=args.verbose)
 
     os.makedirs(args.outdir, exist_ok = True)
     
     logging.info('ANOSPP QC data import started')
 
-    hap_df = prep_hap(args.haplotypes)
     samples_df = prep_samples(args.manifest)
+    hap_df = prep_hap(args.haplotypes)
     stats_df = prep_stats(args.stats)
 
     comb_stats_df = combine_stats(stats_df, hap_df, samples_df)
 
     logging.info('ANOSPP QC plotting started')
 
     fig, _ = plot_target_balance(hap_df)
@@ -270,20 +269,20 @@
         'annot':True,
         'cmap':'coolwarm',
         'fmt':'.2g'
     }
     for col in ('input_log10', 
                 'final_log10',
                 'filter_rate',
-                'mosq_targets_recovered',
+                'raw_mosq_targets_recovered',
                 'P1_log10_reads',
                 'P2_log10_reads',
-                'multiallelic_targets'):
+                'raw_multiallelic_mosq_targets'):
         for lims_plate in (True, False):
-            if col == 'mosq_targets_recovered':
+            if col == 'raw_mosq_targets_recovered':
                 heatmap_kwargs['vmin'] = 0
                 heatmap_kwargs['vmax'] = 62
             elif col == 'filter_rate':
                 heatmap_kwargs['vmin'] = 0
                 heatmap_kwargs['vmax'] = 1 
             else:
                 heatmap_kwargs['vmin'] = None
@@ -296,15 +295,15 @@
             if lims_plate:
                 plate_hm_fn  = f'{args.outdir}/lims_plate_hm_{col}.png' 
             else:
                 plate_hm_fn  = f'{args.outdir}/plate_hm_{col}.png' 
             fig.savefig(plate_hm_fn)
             plt.close(fig)
 
-    logging.info('ANOSPP data QC ended')
+    logging.info('ANOSPP QC complete')
 
 def main():
     
     parser = argparse.ArgumentParser("QC for ANOSPP sequencing data")
     parser.add_argument('-a', '--haplotypes', help='Haplotypes tsv file', required=True)
     parser.add_argument('-m', '--manifest', help='Samples manifest tsv file', required=True)
     parser.add_argument('-s', '--stats', help='DADA2 stats tsv file', required=True)
```

### Comparing `anospp_analysis-0.1.3/anospp_analysis/util.py` & `anospp_analysis-0.2.0/anospp_analysis/util.py`

 * *Files 5% similar despite different names*

```diff
@@ -72,14 +72,18 @@
 
     # edge case
     lims_well_ids[0] = 'P24'
 
     return lims_well_ids
 
 def seqid_generator(hap_df):
+    '''
+    assign identifyer to unique haplotypes
+    used in nn/construct_unique_kmer_table
+    '''
 
     seqids = dict()
     for tgt, group in hap_df.groupby('target'):
         for (i, cons) in enumerate(group['consensus'].unique()):
             seqids[tgt + cons] = '{}-{}'.format(tgt, i)
     hap_df['seqid'] = (hap_df.target + hap_df.consensus).replace(seqids)
 
@@ -116,14 +120,16 @@
 
     if 'reads_fraction' not in hap_df.columns:
         hap_df['reads_fraction'] = hap_df['reads'] / hap_df['total_reads']
 
     if 'nalleles' not in hap_df.columns:
         hap_df['nalleles'] = hap_df.groupby(by=['sample_id', 'target']) \
             ['consensus'].transform('nunique')
+
+    hap_df['consensus'] = hap_df['consensus'].str.upper()
         
     hap_df = seqid_generator(hap_df)
 
     hap_df['target'] = pd.Categorical(hap_df['target'], 
                                     categories=CUTADAPT_TARGETS, 
                                     ordered=True)
     
@@ -135,55 +141,67 @@
     return hap_df
 
 def prep_samples(samples_fn):
     '''
     load sample manifest used for anospp pipeline
     '''
 
-    logging.info(f'preparing sample manifest from {samples_fn}')
-
     # allow reading from tsv (new style) or csv (old style)
     if samples_fn.endswith('csv'):
-        samples_df = pd.read_csv(samples_fn, sep=',')
+        logging.info(f'preparing sample manifest from legacy file {samples_fn}')
+        samples_df = pd.read_csv(samples_fn, sep=',', dtype='str')
+        samples_df.rename(columns=({
+            'Source_sample':'sample_id',
+            'Run':'run_id',
+            'Lane':'lane_index',
+            'Tag':'tag_index',
+            'Replicate':'replicate_id'
+            }), 
+            inplace=True)
     elif samples_fn.endswith('tsv'):
-        samples_df = pd.read_csv(samples_fn, sep='\t')
+        logging.info(f'preparing sample manifest from new file {samples_fn}')
+        samples_df = pd.read_csv(samples_fn, sep='\t', dtype='str')
+        samples_df.rename(columns=({'derived_sample_id':'sample_id'}), inplace=True)
+        assert samples_df.irods_path.str.match('/seq/\d{5}/\d{5}_\d#\d+.cram').all()
+        samples_df['run_id'] = samples_df.irods_path.str.split('/').str.get(2)
+        samples_df[['lane_index', 'tag_index']] = samples_df.irods_path \
+            .str.split('/').str.get(3) \
+            .str.split('_').str.get(1) \
+            .str.split('.').str.get(0) \
+            .str.split('#', expand=True)
     else:
-        raise ValueError(f'Expected {samples_fn} to be in either tsv or csv format')
-
-    # compatibility with old style samples column names
-    samples_df.rename(columns=({
-        'Source_sample':'sample_id',
-        # 'sample':'sample_id',
-        'Run':'run_id',
-        'Lane':'lane_index',
-        'Tag':'tag_index',
-        'Replicate':'replicate_id'
-        }), 
-    inplace=True)
+        raise ValueError(f'Expected {samples_fn} to be in either tsv or csv format')    
 
     for col in ('sample_id',
                 'run_id',
                 'lane_index',
                 'tag_index'):
         assert col in samples_df.columns, f'samples column {col} not found'
-
-    # plate ids
-    if 'plate_id' in samples_df.columns:
-        samples_df['plate_id'] = samples_df.plate_id
-    else:
-        samples_df['plate_id'] = samples_df.apply(lambda r: f'p_{r.run_id}_{(r.tag_index - 1) // 96 + 1}',
-            axis=1)
-    if 'well_id' in samples_df.columns:
-        samples_df['well_id'] = samples_df.well_id
+    samples_df['run_id'] = samples_df['run_id'].astype(int)
+    samples_df['lane_index'] = samples_df['lane_index'].astype(int)
+    samples_df['tag_index'] = samples_df['tag_index'].astype(int)
+    
+    # plate/well ids were recorded in legacy filetypes, keep as is
+    if 'plate_id' in samples_df.columns and 'well_id' in samples_df.columns:
+        pass
     else:
-        samples_df['well_id'] = (samples_df.tag_index % 96).replace(well_id_mapper())
+        # sample_id as `{plate_id}_{well_id}-{sanger_sample_id}` 
+        try:
+            plate_well_ids = samples_df['sample_id'].str.rsplit('-', n = 1).str.get(0)
+            samples_df[['plate_id', 'well_id']] = plate_well_ids.str.rsplit('_', n = 1, expand=True)
+            assert samples_df.well_id.isin(well_id_mapper().values()).all()
+        except:
+            samples_df['plate_id'] = samples_df.apply(lambda r: f'p_{r.run_id}_{(r.tag_index - 1) // 96 + 1}',
+                axis=1)
+            samples_df['well_id'] = (samples_df.tag_index % 96).replace(well_id_mapper())
+    
     assert ~samples_df.plate_id.isna().any(), 'Could not infer plate_id for all samples'
     assert ~samples_df.well_id.isna().any(), 'Could not infer well_id for all samples'
     assert samples_df.well_id.isin(well_id_mapper().values()).all(), 'Found well_id outside A1...H12'
-    # lims plate ids
+    # id_library_lims as `{lims_plate_id}:{lims_well_id}`
     if ('id_library_lims' in samples_df.columns and
         samples_df.id_library_lims.str.contains(':').all()):
             samples_df[['lims_plate_id','lims_well_id']] = samples_df.id_library_lims.str.split(':', 
                                                                                                 n = 1, 
                                                                                                 expand=True)
     else:
         samples_df['lims_plate_id'] = samples_df.apply(lambda r: f'lp_{r.run_id}_{(r.tag_index - 1) // 384 + 1}',
@@ -201,17 +219,21 @@
     
     For legacy stats table, summarise across targets
     '''
 
     logging.info(f'preparing DADA2 statistics from {stats_fn}')
 
     stats_df = pd.read_csv(stats_fn, sep='\t')
-    # compatibility with legacy samples column names
+
     stats_df.rename(columns={
-        's_Sample':'sample_id'
+        # compatibility with legacy format
+        's_Sample':'sample_id',
+        # compatibility with new format 
+        'sample':'sample_id',
+        'DADA2_input':'input'
         },
         inplace=True)
     
     for col in ('sample_id',
                 'input',
                 'filtered',
                 'denoisedF',
@@ -221,14 +243,15 @@
         assert col in stats_df.columns, f'stats column {col} not found'
 
     # denoising happens for F and R reads independently, we take minimum of those 
     # as an estimate for retained read count
     stats_df['denoised'] = stats_df[['denoisedF','denoisedR']].min(axis=1)
     # legacy stats calculated separately for each target, merging
     if 'target' in stats_df.columns:
+        logging.info(f'summarising legacy DADA2 statistics across targets')
         stats_df = stats_df.groupby('sample_id').sum(numeric_only=True).reset_index()
     # add final read counts for comatibility with legacy pipeline
     # that had a post-filtering step
     if 'final' not in stats_df.columns:
         stats_df['final'] = stats_df['nonchim']
     # logscale read counts, placeholder value for zero - -1
     for col in stats_df.columns.drop(['sample_id']):
@@ -253,26 +276,27 @@
         logging.error('sample_id mismatch between haps and samples, QC results will be compromised')
 
     comb_stats_df = pd.merge(stats_df, samples_df, on='sample_id', how='inner')
     comb_stats_df.set_index('sample_id', inplace=True)
     comb_stats_df['targets_recovered'] = hap_df.groupby('sample_id') \
         ['target'].nunique()
     comb_stats_df['targets_recovered'] = comb_stats_df['targets_recovered'].fillna(0)
-    comb_stats_df['mosq_targets_recovered'] = hap_df[hap_df.target.isin(MOSQ_TARGETS)] \
+    comb_stats_df['raw_mosq_targets_recovered'] = hap_df[hap_df.target.isin(MOSQ_TARGETS)] \
         .groupby('sample_id')['target'].nunique()
-    comb_stats_df['mosq_targets_recovered'] = comb_stats_df['mosq_targets_recovered'].fillna(0)
-    comb_stats_df['mosq_reads'] = hap_df[hap_df.target.isin(MOSQ_TARGETS)] \
+    comb_stats_df['raw_mosq_targets_recovered'] = comb_stats_df['raw_mosq_targets_recovered'].fillna(0)
+    comb_stats_df['raw_mosq_reads'] = hap_df[hap_df.target.isin(MOSQ_TARGETS)] \
         .groupby('sample_id')['reads'].sum()
-    comb_stats_df['mosq_reads'] = comb_stats_df['mosq_reads'].fillna(0)
-    comb_stats_df['mosq_log10_reads'] = comb_stats_df['mosq_reads'] \
+    comb_stats_df['raw_mosq_reads'] = comb_stats_df['raw_mosq_reads'].fillna(0)
+    comb_stats_df['raw_mosq_log10_reads'] = comb_stats_df['raw_mosq_reads'] \
         .replace(0,0.1).apply(lambda x: np.log10(x))
     for pt in PLASM_TARGETS:
         comb_stats_df[f'{pt}_reads'] = hap_df[hap_df.target == pt] \
             .groupby('sample_id')['reads'].sum()
         comb_stats_df[f'{pt}_reads'] = comb_stats_df[f'{pt}_reads'].fillna(0)
         comb_stats_df[f'{pt}_log10_reads'] = comb_stats_df[f'{pt}_reads'] \
             .replace(0,0.1).apply(lambda x: np.log10(x))
-    comb_stats_df['multiallelic_targets'] = (hap_df.groupby('sample_id')['target'].value_counts() > 2).groupby(level='sample_id').sum()
-    comb_stats_df['multiallelic_targets'] = comb_stats_df['multiallelic_targets'].fillna(0)
+    comb_stats_df['raw_multiallelic_mosq_targets'] = (hap_df[hap_df.target.isin(MOSQ_TARGETS)] \
+        .groupby('sample_id')['target'].value_counts() > 2).groupby(level='sample_id').sum()
+    comb_stats_df['raw_multiallelic_mosq_targets'] = comb_stats_df['raw_multiallelic_mosq_targets'].fillna(0)
     comb_stats_df.reset_index(inplace=True)
         
     return comb_stats_df
```

### Comparing `anospp_analysis-0.1.3/PKG-INFO` & `anospp_analysis-0.2.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,116 +1,145 @@
 Metadata-Version: 2.1
 Name: anospp-analysis
-Version: 0.1.3
+Version: 0.2.0
 Summary: ANOSPP data analysis
 License: MIT
 Author: Alex Makunin
 Author-email: am60@sanger.ac.uk
-Requires-Python: >=3.10,<4.0
+Requires-Python: >=3.10,<3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: BioPython
+Requires-Dist: bokeh
 Requires-Dist: cutadapt
+Requires-Dist: keras (>=2.12.0,<3.0.0)
 Requires-Dist: numpy
 Requires-Dist: pandas
 Requires-Dist: seaborn
+Requires-Dist: tensorflow (>=2.12.0,<3.0.0)
 Description-Content-Type: text/markdown
 
 # anospp-analysis
 
 Python package for ANOSPP data analysis
 
-ANOSPP is the multiplexed amplicon sequencing assay for Anopheles mosquito species identification and Plasmodium detection. This repository contains the code for analysis of the sequencing results pre-processed with [nf-core ampliseq](https://nf-co.re/ampliseq) pipeline. 
+ANOSPP is the multiplexed amplicon sequencing assay for Anopheles mosquito species identification and Plasmodium detection. This repository contains the code for analysis of the sequencing results pre-processed with [nf-core ampliseq](https://nf-co.re/ampliseq) pipeline.
+
+## Installation
+
+For released version
+
+```bash
+conda install -c bioconda anospp-analysis
+```
+
+For development setup, see instructions below
 
 ## Usage
 
 Key analysis steps are implemented as standalone scripts:
+
 - `anospp-prep` takes DADA2 output files and targets primer sequences, demultiplexes the amplicons and yields haplotypes table
-- `anospp-qc` takes haplotypes table, DADA2 stats table and samples manifest and produces QC plots 
+- `anospp-qc` takes haplotypes table, DADA2 stats table and samples manifest and produces QC plots
+- `anospp-plasm` blasts Plasmodium sequences against reference dataset to determine species and infer sample infection status
+- `anospp-nn` compares k-mer profiles of mosquito targets against a reference dataset and provides probabilistic species calls
+- `anospp-vae` provides finer scale species prediction for An. gambiae complex with VAE projection
 
 ## Development
 
 ### Setup
 
 Installation is hybrid with conda + poetry:
-```
+
+```bash
 git clone git@github.com:malariagen/anospp-analysis.git
 cd anospp-analysis
 mamba env create -f environment.yml
-conda activate anospp_analysis
+conda activate anospp_analysis_dev
 poetry install
 ```
 
-Activate development environment:
-```
-poetry shell
-```
-
 ### Usage & testing
 
 The code in this repository can be accessed via wrapper scripts:
-```
+
+```bash
 anospp-qc \
     --haplotypes test_data/haplotypes.tsv \
     --samples test_data/samples.csv \
     --stats test_data/stats.tsv \
     --outdir test_data/qc
 ```
 
 Besides, individual components are available as a python API:
-```
+
+```bash
 $ python
 >>> from anospp_analysis.util import *
 >>> PLASM_TARGETS
 ['P1', 'P2']
 ```
 
-Automated testing & CI
+TODO Automated testing & CI
 
 ### Adding Python deps
 
 Introducing python dependencies should be done via poetry:
-```
+
+```bash
 poetry add package_name
-``` 
+```
+
 This should update both `pyproject.toml` and `poetry.lock` files
 
 If the package should be used in development environment only, use
-```
+
+```bash
 poetry add package_name --dev
 ```
 
+To update environment after changes made to `pyproject.toml` and/or `poetry.lock`
+
+```bash
+poetry install
+```
+
 ### Adding non-Python deps
 
-Introducing non-python dependencies should be done via conda: edit `environment.yml`, 
+Introducing non-python dependencies should be done via conda: edit `environment.yml`,
 then re-create the conda environment and poetry deps:
-```
+
+```bash
 mamba env create -f environment.yml
 conda activate anospp_analysis
 poetry install
 ```
 
-Changes in conda environment might also introduce changes to the python installation, 
+Changes in conda environment might also introduce changes to the python installation,
 in which case one should update poetry lock file
-```
+
+```bash
 poetry lock
 ```
 
 ## Release checklist
 
 While in dev branch
+
 - test functionality (TODO CI)
+- bump version in module init
 - bump version in `pyproject.toml`
 
-Then
+Then,
+
 - merge into master
 - github release
 - pypi release
 
 Conda recipe update `conda.recipe/meta.yaml`:
+
 - check deps vs `environment.yaml` and `pyproject.toml`
-- bump version  
+- bump version in meta yaml  
 - update sha256 from pypi project (download files > tar.gz > view hashes)
 - test conda recipe with `bioconda-utils build --git-range master` vs bioconda-recipes
```

