# Comparing `tmp/sec-certs-0.1.4.tar.gz` & `tmp/sec-certs-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sec-certs-0.1.4.tar", last modified: Wed May 10 12:00:38 2023, max compression
+gzip compressed data, was "sec-certs-0.1.5.tar", last modified: Thu May 18 13:19:26 2023, max compression
```

## Comparing `sec-certs-0.1.4.tar` & `sec-certs-0.1.5.tar`

### file list

```diff
@@ -1,270 +1,270 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:00:38.684648 sec-certs-0.1.4/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:00:38.640648 sec-certs-0.1.4/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:00:38.648648 sec-certs-0.1.4/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      619 2023-05-10 12:00:28.000000 sec-certs-0.1.4/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-05-10 12:00:28.000000 sec-certs-0.1.4/.github/ISSUE_TEMPLATE/feature_request.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:00:38.648648 sec-certs-0.1.4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-05-10 12:00:28.000000 sec-certs-0.1.4/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-05-10 12:00:28.000000 sec-certs-0.1.4/.github/workflows/lint.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-05-10 12:00:28.000000 sec-certs-0.1.4/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)      990 2023-05-10 12:00:28.000000 sec-certs-0.1.4/.github/workflows/tests.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-05-10 12:00:28.000000 sec-certs-0.1.4/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      516 2023-05-10 12:00:28.000000 sec-certs-0.1.4/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3347 2023-05-10 12:00:28.000000 sec-certs-0.1.4/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     4265 2023-05-10 12:00:28.000000 sec-certs-0.1.4/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)     1590 2023-05-10 12:00:28.000000 sec-certs-0.1.4/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-05-10 12:00:28.000000 sec-certs-0.1.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5312 2023-05-10 12:00:38.684648 sec-certs-0.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4250 2023-05-10 12:00:28.000000 sec-certs-0.1.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-05-10 12:00:28.000000 sec-certs-0.1.4/codecov.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:00:38.648648 sec-certs-0.1.4/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:00:38.648648 sec-certs-0.1.4/data/cert_id_eval/
--rw-r--r--   0 runner    (1001) docker     (123)     9830 2023-05-10 12:00:28.000000 sec-certs-0.1.4/data/cert_id_eval/duplicate_ids.csv
--rw-r--r--   0 runner    (1001) docker     (123)     3865 2023-05-10 12:00:28.000000 sec-certs-0.1.4/data/cert_id_eval/missing_ids.csv
--rw-r--r--   0 runner    (1001) docker     (123)     3358 2023-05-10 12:00:28.000000 sec-certs-0.1.4/data/cert_id_eval/random.csv
--rw-r--r--   0 runner    (1001) docker     (123)    18418 2023-05-10 12:00:28.000000 sec-certs-0.1.4/data/cert_id_eval/random_references.csv
--rw-r--r--   0 runner    (1001) docker     (123)     6264 2023-05-10 12:00:28.000000 sec-certs-0.1.4/data/cert_id_eval/truth.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:00:38.648648 sec-certs-0.1.4/data/cpe_eval/
--rw-r--r--   0 runner    (1001) docker     (123)   176434 2023-05-10 12:00:28.000000 sec-certs-0.1.4/data/cpe_eval/manual_cpe_labels.json
--rw-r--r--   0 runner    (1001) docker     (123)    68713 2023-05-10 12:00:28.000000 sec-certs-0.1.4/data/cpe_eval/random.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:00:38.652648 sec-certs-0.1.4/data/information_retrieval_split/
--rw-r--r--   0 runner    (1001) docker     (123)   117213 2023-05-10 12:00:28.000000 sec-certs-0.1.4/data/information_retrieval_split/metadata.csv
--rw-r--r--   0 runner    (1001) docker     (123)    85352 2023-05-10 12:00:28.000000 sec-certs-0.1.4/data/information_retrieval_split/sampled_images.json
--rw-r--r--   0 runner    (1001) docker     (123)    20260 2023-05-10 12:00:28.000000 sec-certs-0.1.4/data/information_retrieval_split/test.json
--rw-r--r--   0 runner    (1001) docker     (123)    72860 2023-05-10 12:00:28.000000 sec-certs-0.1.4/data/information_retrieval_split/train.json
--rw-r--r--   0 runner    (1001) docker     (123)     8100 2023-05-10 12:00:28.000000 sec-certs-0.1.4/data/information_retrieval_split/valid.json
--rw-r--r--   0 runner    (1001) docker     (123)     1046 2023-05-10 12:00:28.000000 sec-certs-0.1.4/data/label_studio_interface.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:00:38.652648 sec-certs-0.1.4/data/old_manual_cpe_labels/
--rw-r--r--   0 runner    (1001) docker     (123)  1552011 2023-05-10 12:00:28.000000 sec-certs-0.1.4/data/old_manual_cpe_labels/cc.json
--rw-r--r--   0 runner    (1001) docker     (123)  1467792 2023-05-10 12:00:28.000000 sec-certs-0.1.4/data/old_manual_cpe_labels/fips.json
--rw-r--r--   0 runner    (1001) docker     (123)     2051 2023-05-10 12:00:28.000000 sec-certs-0.1.4/data/readme.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:00:38.656648 sec-certs-0.1.4/data/reference_annotations_split/
--rw-r--r--   0 runner    (1001) docker     (123)    18674 2023-05-10 12:00:28.000000 sec-certs-0.1.4/data/reference_annotations_split/test.json
--rw-r--r--   0 runner    (1001) docker     (123)    11138 2023-05-10 12:00:28.000000 sec-certs-0.1.4/data/reference_annotations_split/train.json
--rw-r--r--   0 runner    (1001) docker     (123)     7442 2023-05-10 12:00:28.000000 sec-certs-0.1.4/data/reference_annotations_split/valid.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:00:38.656648 sec-certs-0.1.4/data/sar_correlations/
--rw-r--r--   0 runner    (1001) docker     (123)     1648 2023-05-10 12:00:28.000000 sec-certs-0.1.4/data/sar_correlations/all_certs_sar_cve_corr.csv
--rw-r--r--   0 runner    (1001) docker     (123)      767 2023-05-10 12:00:28.000000 sec-certs-0.1.4/data/sar_correlations/readme.md
--rw-r--r--   0 runner    (1001) docker     (123)     1365 2023-05-10 12:00:28.000000 sec-certs-0.1.4/data/sar_correlations/vuln_rich_certs_sar_cve_corr.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:00:38.644648 sec-certs-0.1.4/data/validation_test_split/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:00:38.656648 sec-certs-0.1.4/data/validation_test_split/cc/
--rw-r--r--   0 runner    (1001) docker     (123)    55394 2023-05-10 12:00:28.000000 sec-certs-0.1.4/data/validation_test_split/cc/test.json
--rw-r--r--   0 runner    (1001) docker     (123)    55394 2023-05-10 12:00:28.000000 sec-certs-0.1.4/data/validation_test_split/cc/validation.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:00:38.656648 sec-certs-0.1.4/data/validation_test_split/fips/
--rw-r--r--   0 runner    (1001) docker     (123)    23439 2023-05-10 12:00:28.000000 sec-certs-0.1.4/data/validation_test_split/fips/test.json
--rw-r--r--   0 runner    (1001) docker     (123)    23434 2023-05-10 12:00:28.000000 sec-certs-0.1.4/data/validation_test_split/fips/validation.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:00:38.656648 sec-certs-0.1.4/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-05-10 12:00:28.000000 sec-certs-0.1.4/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:00:38.660648 sec-certs-0.1.4/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)    41751 2023-05-10 12:00:28.000000 sec-certs-0.1.4/docs/_static/logo.png
--rw-r--r--   0 runner    (1001) docker     (123)     3359 2023-05-10 12:00:28.000000 sec-certs-0.1.4/docs/_static/logo.svg
--rw-r--r--   0 runner    (1001) docker     (123)    18611 2023-05-10 12:00:28.000000 sec-certs-0.1.4/docs/_static/logo_badge.png
--rw-r--r--   0 runner    (1001) docker     (123)     3575 2023-05-10 12:00:28.000000 sec-certs-0.1.4/docs/_static/logo_badge.svg
--rw-r--r--   0 runner    (1001) docker     (123)   363422 2023-05-10 12:00:28.000000 sec-certs-0.1.4/docs/_static/logolink_OP_VVV_hor_barva_eng.jpg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:00:38.660648 sec-certs-0.1.4/docs/api/
--rw-r--r--   0 runner    (1001) docker     (123)      860 2023-05-10 12:00:28.000000 sec-certs-0.1.4/docs/api/dataset.md
--rw-r--r--   0 runner    (1001) docker     (123)     1277 2023-05-10 12:00:28.000000 sec-certs-0.1.4/docs/api/model.md
--rw-r--r--   0 runner    (1001) docker     (123)      506 2023-05-10 12:00:28.000000 sec-certs-0.1.4/docs/api/sample.md
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-10 12:00:28.000000 sec-certs-0.1.4/docs/code_of_conduct.md
--rw-r--r--   0 runner    (1001) docker     (123)     2669 2023-05-10 12:00:28.000000 sec-certs-0.1.4/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     2081 2023-05-10 12:00:28.000000 sec-certs-0.1.4/docs/configuration.md
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-05-10 12:00:28.000000 sec-certs-0.1.4/docs/contributing.md
--rw-r--r--   0 runner    (1001) docker     (123)     2429 2023-05-10 12:00:28.000000 sec-certs-0.1.4/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (123)     1552 2023-05-10 12:00:28.000000 sec-certs-0.1.4/docs/installation.md
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-10 12:00:28.000000 sec-certs-0.1.4/docs/license.md
--rw-r--r--   0 runner    (1001) docker     (123)      800 2023-05-10 12:00:28.000000 sec-certs-0.1.4/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)     3303 2023-05-10 12:00:28.000000 sec-certs-0.1.4/docs/quickstart.md
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-05-10 12:00:28.000000 sec-certs-0.1.4/docs/readme.md
--rw-r--r--   0 runner    (1001) docker     (123)     1117 2023-05-10 12:00:28.000000 sec-certs-0.1.4/docs/user_guide.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:00:38.660648 sec-certs-0.1.4/notebooks/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:00:38.660648 sec-certs-0.1.4/notebooks/cc/
--rw-r--r--   0 runner    (1001) docker     (123)    13798 2023-05-10 12:00:28.000000 sec-certs-0.1.4/notebooks/cc/cert_id_eval.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     4892 2023-05-10 12:00:28.000000 sec-certs-0.1.4/notebooks/cc/cpe_eval.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:00:38.660648 sec-certs-0.1.4/notebooks/cc/reference_annotations/
--rw-r--r--   0 runner    (1001) docker     (123)     2659 2023-05-10 12:00:28.000000 sec-certs-0.1.4/notebooks/cc/reference_annotations/train_validation_test_split.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    42619 2023-05-10 12:00:28.000000 sec-certs-0.1.4/notebooks/cc/references.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    21943 2023-05-10 12:00:28.000000 sec-certs-0.1.4/notebooks/cc/temporal_trends.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    35405 2023-05-10 12:00:28.000000 sec-certs-0.1.4/notebooks/cc/vulnerabilities.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:00:38.660648 sec-certs-0.1.4/notebooks/examples/
--rw-r--r--   0 runner    (1001) docker     (123)     8017 2023-05-10 12:00:28.000000 sec-certs-0.1.4/notebooks/examples/cc.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)   337372 2023-05-10 12:00:28.000000 sec-certs-0.1.4/notebooks/examples/est_solution.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     3952 2023-05-10 12:00:28.000000 sec-certs-0.1.4/notebooks/examples/fips.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     1461 2023-05-10 12:00:28.000000 sec-certs-0.1.4/notebooks/examples/fips_iut.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-05-10 12:00:28.000000 sec-certs-0.1.4/notebooks/examples/fips_mip.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:00:38.664648 sec-certs-0.1.4/notebooks/examples/img/
--rw-r--r--   0 runner    (1001) docker     (123)    29981 2023-05-10 12:00:28.000000 sec-certs-0.1.4/notebooks/examples/img/boxplot_validity.png
--rw-r--r--   0 runner    (1001) docker     (123)   134946 2023-05-10 12:00:28.000000 sec-certs-0.1.4/notebooks/examples/img/cves_n_days_after_certification.png
--rw-r--r--   0 runner    (1001) docker     (123)     1755 2023-05-10 12:00:28.000000 sec-certs-0.1.4/notebooks/examples/model.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)   104006 2023-05-10 12:00:28.000000 sec-certs-0.1.4/notebooks/final_run.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:00:38.664648 sec-certs-0.1.4/notebooks/fips/
--rw-r--r--   0 runner    (1001) docker     (123)    15315 2023-05-10 12:00:28.000000 sec-certs-0.1.4/notebooks/fips/in_process.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     2957 2023-05-10 12:00:28.000000 sec-certs-0.1.4/notebooks/fips/references.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    12817 2023-05-10 12:00:28.000000 sec-certs-0.1.4/notebooks/fips/temporal_trends.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)   132824 2023-05-10 12:00:28.000000 sec-certs-0.1.4/notebooks/fips/vulnerabilities.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     9489 2023-05-10 12:00:28.000000 sec-certs-0.1.4/notebooks/latex_plotting.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     8645 2023-05-10 12:00:28.000000 sec-certs-0.1.4/notebooks/ocr.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     3383 2023-05-10 12:00:28.000000 sec-certs-0.1.4/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:00:38.664648 sec-certs-0.1.4/requirements/
--rwxr-xr-x   0 runner    (1001) docker     (123)      361 2023-05-10 12:00:28.000000 sec-certs-0.1.4/requirements/compile.sh
--rw-r--r--   0 runner    (1001) docker     (123)    10058 2023-05-10 12:00:28.000000 sec-certs-0.1.4/requirements/dev_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5836 2023-05-10 12:00:28.000000 sec-certs-0.1.4/requirements/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6252 2023-05-10 12:00:28.000000 sec-certs-0.1.4/requirements/test_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-10 12:00:28.000000 sec-certs-0.1.4/runtime.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-10 12:00:38.684648 sec-certs-0.1.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:00:38.644648 sec-certs-0.1.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:00:38.664648 sec-certs-0.1.4/src/sec_certs/
--rw-r--r--   0 runner    (1001) docker     (123)      521 2023-05-10 12:00:28.000000 sec-certs-0.1.4/src/sec_certs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-05-10 12:00:28.000000 sec-certs-0.1.4/src/sec_certs/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-10 12:00:38.000000 sec-certs-0.1.4/src/sec_certs/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     5927 2023-05-10 12:00:28.000000 sec-certs-0.1.4/src/sec_certs/cert_rules.py
--rw-r--r--   0 runner    (1001) docker     (123)     7820 2023-05-10 12:00:28.000000 sec-certs-0.1.4/src/sec_certs/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     7024 2023-05-10 12:00:28.000000 sec-certs-0.1.4/src/sec_certs/configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)     6847 2023-05-10 12:00:28.000000 sec-certs-0.1.4/src/sec_certs/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:00:38.668648 sec-certs-0.1.4/src/sec_certs/dataset/
--rw-r--r--   0 runner    (1001) docker     (123)      872 2023-05-10 12:00:28.000000 sec-certs-0.1.4/src/sec_certs/dataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    39043 2023-05-10 12:00:28.000000 sec-certs-0.1.4/src/sec_certs/dataset/cc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1854 2023-05-10 12:00:28.000000 sec-certs-0.1.4/src/sec_certs/dataset/cc_scheme.py
--rw-r--r--   0 runner    (1001) docker     (123)     4340 2023-05-10 12:00:28.000000 sec-certs-0.1.4/src/sec_certs/dataset/cpe.py
--rw-r--r--   0 runner    (1001) docker     (123)     7578 2023-05-10 12:00:28.000000 sec-certs-0.1.4/src/sec_certs/dataset/cve.py
--rw-r--r--   0 runner    (1001) docker     (123)    25690 2023-05-10 12:00:28.000000 sec-certs-0.1.4/src/sec_certs/dataset/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    14755 2023-05-10 12:00:28.000000 sec-certs-0.1.4/src/sec_certs/dataset/fips.py
--rw-r--r--   0 runner    (1001) docker     (123)     5106 2023-05-10 12:00:28.000000 sec-certs-0.1.4/src/sec_certs/dataset/fips_algorithm.py
--rw-r--r--   0 runner    (1001) docker     (123)     2187 2023-05-10 12:00:28.000000 sec-certs-0.1.4/src/sec_certs/dataset/fips_iut.py
--rw-r--r--   0 runner    (1001) docker     (123)     3749 2023-05-10 12:00:28.000000 sec-certs-0.1.4/src/sec_certs/dataset/fips_mip.py
--rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-05-10 12:00:28.000000 sec-certs-0.1.4/src/sec_certs/dataset/json_path_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     3078 2023-05-10 12:00:28.000000 sec-certs-0.1.4/src/sec_certs/dataset/protection_profile.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:00:38.668648 sec-certs-0.1.4/src/sec_certs/model/
--rw-r--r--   0 runner    (1001) docker     (123)      793 2023-05-10 12:00:28.000000 sec-certs-0.1.4/src/sec_certs/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4485 2023-05-10 12:00:28.000000 sec-certs-0.1.4/src/sec_certs/model/cc_matching.py
--rw-r--r--   0 runner    (1001) docker     (123)    18209 2023-05-10 12:00:28.000000 sec-certs-0.1.4/src/sec_certs/model/cpe_matching.py
--rw-r--r--   0 runner    (1001) docker     (123)     3719 2023-05-10 12:00:28.000000 sec-certs-0.1.4/src/sec_certs/model/evaluation.py
--rw-r--r--   0 runner    (1001) docker     (123)     3322 2023-05-10 12:00:28.000000 sec-certs-0.1.4/src/sec_certs/model/fips_matching.py
--rw-r--r--   0 runner    (1001) docker     (123)     1918 2023-05-10 12:00:28.000000 sec-certs-0.1.4/src/sec_certs/model/matching.py
--rw-r--r--   0 runner    (1001) docker     (123)     9532 2023-05-10 12:00:28.000000 sec-certs-0.1.4/src/sec_certs/model/reference_finder.py
--rw-r--r--   0 runner    (1001) docker     (123)     7337 2023-05-10 12:00:28.000000 sec-certs-0.1.4/src/sec_certs/model/sar_transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5186 2023-05-10 12:00:28.000000 sec-certs-0.1.4/src/sec_certs/model/transitive_vulnerability_finder.py
--rw-r--r--   0 runner    (1001) docker     (123)    27743 2023-05-10 12:00:28.000000 sec-certs-0.1.4/src/sec_certs/rules.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:00:38.672649 sec-certs-0.1.4/src/sec_certs/sample/
--rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-05-10 12:00:28.000000 sec-certs-0.1.4/src/sec_certs/sample/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    42917 2023-05-10 12:00:28.000000 sec-certs-0.1.4/src/sec_certs/sample/cc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4745 2023-05-10 12:00:28.000000 sec-certs-0.1.4/src/sec_certs/sample/cc_certificate_id.py
--rw-r--r--   0 runner    (1001) docker     (123)     2894 2023-05-10 12:00:28.000000 sec-certs-0.1.4/src/sec_certs/sample/cc_maintenance_update.py
--rw-r--r--   0 runner    (1001) docker     (123)    65455 2023-05-10 12:00:28.000000 sec-certs-0.1.4/src/sec_certs/sample/cc_scheme.py
--rw-r--r--   0 runner    (1001) docker     (123)     2599 2023-05-10 12:00:28.000000 sec-certs-0.1.4/src/sec_certs/sample/certificate.py
--rw-r--r--   0 runner    (1001) docker     (123)     6508 2023-05-10 12:00:28.000000 sec-certs-0.1.4/src/sec_certs/sample/cpe.py
--rw-r--r--   0 runner    (1001) docker     (123)     9310 2023-05-10 12:00:28.000000 sec-certs-0.1.4/src/sec_certs/sample/cve.py
--rw-r--r--   0 runner    (1001) docker     (123)    29341 2023-05-10 12:00:28.000000 sec-certs-0.1.4/src/sec_certs/sample/fips.py
--rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-05-10 12:00:28.000000 sec-certs-0.1.4/src/sec_certs/sample/fips_algorithm.py
--rw-r--r--   0 runner    (1001) docker     (123)     5541 2023-05-10 12:00:28.000000 sec-certs-0.1.4/src/sec_certs/sample/fips_iut.py
--rw-r--r--   0 runner    (1001) docker     (123)     9337 2023-05-10 12:00:28.000000 sec-certs-0.1.4/src/sec_certs/sample/fips_mip.py
--rw-r--r--   0 runner    (1001) docker     (123)     1951 2023-05-10 12:00:28.000000 sec-certs-0.1.4/src/sec_certs/sample/protection_profile.py
--rw-r--r--   0 runner    (1001) docker     (123)     1736 2023-05-10 12:00:28.000000 sec-certs-0.1.4/src/sec_certs/sample/sar.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:00:38.672649 sec-certs-0.1.4/src/sec_certs/serialization/
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-10 12:00:28.000000 sec-certs-0.1.4/src/sec_certs/serialization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6813 2023-05-10 12:00:28.000000 sec-certs-0.1.4/src/sec_certs/serialization/json.py
--rw-r--r--   0 runner    (1001) docker     (123)      385 2023-05-10 12:00:28.000000 sec-certs-0.1.4/src/sec_certs/serialization/pandas.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:00:38.672649 sec-certs-0.1.4/src/sec_certs/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-10 12:00:28.000000 sec-certs-0.1.4/src/sec_certs/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    38410 2023-05-10 12:00:28.000000 sec-certs-0.1.4/src/sec_certs/utils/extract.py
--rw-r--r--   0 runner    (1001) docker     (123)     7812 2023-05-10 12:00:28.000000 sec-certs-0.1.4/src/sec_certs/utils/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    14804 2023-05-10 12:00:28.000000 sec-certs-0.1.4/src/sec_certs/utils/nvd_dataset_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)    21941 2023-05-10 12:00:28.000000 sec-certs-0.1.4/src/sec_certs/utils/pandas.py
--rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-05-10 12:00:28.000000 sec-certs-0.1.4/src/sec_certs/utils/parallel_processing.py
--rw-r--r--   0 runner    (1001) docker     (123)     9625 2023-05-10 12:00:28.000000 sec-certs-0.1.4/src/sec_certs/utils/pdf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1549 2023-05-10 12:00:28.000000 sec-certs-0.1.4/src/sec_certs/utils/sanitization.py
--rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-05-10 12:00:28.000000 sec-certs-0.1.4/src/sec_certs/utils/strings.py
--rw-r--r--   0 runner    (1001) docker     (123)     2015 2023-05-10 12:00:28.000000 sec-certs-0.1.4/src/sec_certs/utils/tables.py
--rw-r--r--   0 runner    (1001) docker     (123)      269 2023-05-10 12:00:28.000000 sec-certs-0.1.4/src/sec_certs/utils/tqdm.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:00:38.664648 sec-certs-0.1.4/src/sec_certs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5312 2023-05-10 12:00:38.000000 sec-certs-0.1.4/src/sec_certs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7272 2023-05-10 12:00:38.000000 sec-certs-0.1.4/src/sec_certs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 12:00:38.000000 sec-certs-0.1.4/src/sec_certs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-10 12:00:38.000000 sec-certs-0.1.4/src/sec_certs.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-05-10 12:00:38.000000 sec-certs-0.1.4/src/sec_certs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-10 12:00:38.000000 sec-certs-0.1.4/src/sec_certs.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:00:38.672649 sec-certs-0.1.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 12:00:28.000000 sec-certs-0.1.4/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:00:38.676648 sec-certs-0.1.4/tests/cc/
--rw-r--r--   0 runner    (1001) docker     (123)     2223 2023-05-10 12:00:28.000000 sec-certs-0.1.4/tests/cc/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     8414 2023-05-10 12:00:28.000000 sec-certs-0.1.4/tests/cc/test_cc_analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)     2958 2023-05-10 12:00:28.000000 sec-certs-0.1.4/tests/cc/test_cc_certificate.py
--rw-r--r--   0 runner    (1001) docker     (123)     5997 2023-05-10 12:00:28.000000 sec-certs-0.1.4/tests/cc/test_cc_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     3199 2023-05-10 12:00:28.000000 sec-certs-0.1.4/tests/cc/test_cc_maintenance_updates.py
--rw-r--r--   0 runner    (1001) docker     (123)     1512 2023-05-10 12:00:28.000000 sec-certs-0.1.4/tests/cc/test_cc_misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     8012 2023-05-10 12:00:28.000000 sec-certs-0.1.4/tests/cc/test_cc_schemes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1400 2023-05-10 12:00:28.000000 sec-certs-0.1.4/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:00:38.676648 sec-certs-0.1.4/tests/data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 12:00:28.000000 sec-certs-0.1.4/tests/data/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:00:38.676648 sec-certs-0.1.4/tests/data/cc/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 12:00:28.000000 sec-certs-0.1.4/tests/data/cc/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:00:38.676648 sec-certs-0.1.4/tests/data/cc/analysis/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 12:00:28.000000 sec-certs-0.1.4/tests/data/cc/analysis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    30505 2023-05-10 12:00:28.000000 sec-certs-0.1.4/tests/data/cc/analysis/cc_full_dataset.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:00:38.644648 sec-certs-0.1.4/tests/data/cc/analysis/certs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:00:38.644648 sec-certs-0.1.4/tests/data/cc/analysis/certs/reports/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:00:38.676648 sec-certs-0.1.4/tests/data/cc/analysis/certs/reports/pdf/
--rw-r--r--   0 runner    (1001) docker     (123)  1174271 2023-05-10 12:00:28.000000 sec-certs-0.1.4/tests/data/cc/analysis/certs/reports/pdf/ebd276cca70fd723.pdf
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:00:38.676648 sec-certs-0.1.4/tests/data/cc/analysis/certs/reports/txt/
--rw-r--r--   0 runner    (1001) docker     (123)    58767 2023-05-10 12:00:28.000000 sec-certs-0.1.4/tests/data/cc/analysis/certs/reports/txt/ebd276cca70fd723.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:00:38.644648 sec-certs-0.1.4/tests/data/cc/analysis/certs/targets/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:00:38.676648 sec-certs-0.1.4/tests/data/cc/analysis/certs/targets/pdf/
--rw-r--r--   0 runner    (1001) docker     (123)   615034 2023-05-10 12:00:28.000000 sec-certs-0.1.4/tests/data/cc/analysis/certs/targets/pdf/ebd276cca70fd723.pdf
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:00:38.680648 sec-certs-0.1.4/tests/data/cc/analysis/certs/targets/txt/
--rw-r--r--   0 runner    (1001) docker     (123)    98275 2023-05-10 12:00:28.000000 sec-certs-0.1.4/tests/data/cc/analysis/certs/targets/txt/ebd276cca70fd723.txt
--rw-r--r--   0 runner    (1001) docker     (123)    53839 2023-05-10 12:00:28.000000 sec-certs-0.1.4/tests/data/cc/analysis/reference_dataset.json
--rw-r--r--   0 runner    (1001) docker     (123)   103359 2023-05-10 12:00:28.000000 sec-certs-0.1.4/tests/data/cc/analysis/transitive_vulnerability_dataset.json
--rw-r--r--   0 runner    (1001) docker     (123)     4797 2023-05-10 12:00:28.000000 sec-certs-0.1.4/tests/data/cc/analysis/vulnerable_dataset.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:00:38.680648 sec-certs-0.1.4/tests/data/cc/certificate/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 12:00:28.000000 sec-certs-0.1.4/tests/data/cc/certificate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3258 2023-05-10 12:00:28.000000 sec-certs-0.1.4/tests/data/cc/certificate/fictional_cert.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:00:38.680648 sec-certs-0.1.4/tests/data/cc/dataset/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 12:00:28.000000 sec-certs-0.1.4/tests/data/cc/dataset/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:00:38.644648 sec-certs-0.1.4/tests/data/cc/dataset/auxiliary_datasets/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:00:38.680648 sec-certs-0.1.4/tests/data/cc/dataset/auxiliary_datasets/maintenances/
--rw-r--r--   0 runner    (1001) docker     (123)     3515 2023-05-10 12:00:28.000000 sec-certs-0.1.4/tests/data/cc/dataset/auxiliary_datasets/maintenances/maintenance_updates.json
--rw-r--r--   0 runner    (1001) docker     (123)     1817 2023-05-10 12:00:28.000000 sec-certs-0.1.4/tests/data/cc/dataset/cc_products_active.csv
--rw-r--r--   0 runner    (1001) docker     (123)    31505 2023-05-10 12:00:28.000000 sec-certs-0.1.4/tests/data/cc/dataset/cc_products_active.html
--rw-r--r--   0 runner    (1001) docker     (123)    22545 2023-05-10 12:00:28.000000 sec-certs-0.1.4/tests/data/cc/dataset/report_309ac2fd7f2dcf17.txt
--rw-r--r--   0 runner    (1001) docker     (123)    72568 2023-05-10 12:00:28.000000 sec-certs-0.1.4/tests/data/cc/dataset/target_309ac2fd7f2dcf17.txt
--rw-r--r--   0 runner    (1001) docker     (123)    12359 2023-05-10 12:00:28.000000 sec-certs-0.1.4/tests/data/cc/dataset/toy_dataset.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:00:38.680648 sec-certs-0.1.4/tests/data/common/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 12:00:28.000000 sec-certs-0.1.4/tests/data/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1990 2023-05-10 12:00:28.000000 sec-certs-0.1.4/tests/data/common/cpe_dataset.json
--rw-r--r--   0 runner    (1001) docker     (123)    88427 2023-05-10 12:00:28.000000 sec-certs-0.1.4/tests/data/common/cpe_match_feed.json
--rw-r--r--   0 runner    (1001) docker     (123)    31329 2023-05-10 12:00:28.000000 sec-certs-0.1.4/tests/data/common/cve_dataset.json
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-10 12:00:28.000000 sec-certs-0.1.4/tests/data/common/settings_tests.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:00:38.644648 sec-certs-0.1.4/tests/data/fips/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:00:38.680648 sec-certs-0.1.4/tests/data/fips/certificate/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 12:00:28.000000 sec-certs-0.1.4/tests/data/fips/certificate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2741 2023-05-10 12:00:28.000000 sec-certs-0.1.4/tests/data/fips/certificate/fictional_cert.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:00:38.680648 sec-certs-0.1.4/tests/data/fips/dataset/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 12:00:28.000000 sec-certs-0.1.4/tests/data/fips/dataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-05-10 12:00:28.000000 sec-certs-0.1.4/tests/data/fips/dataset/alg_dataset.json
--rw-r--r--   0 runner    (1001) docker     (123)    45964 2023-05-10 12:00:28.000000 sec-certs-0.1.4/tests/data/fips/dataset/fips_modules_active.html
--rw-r--r--   0 runner    (1001) docker     (123)    54952 2023-05-10 12:00:28.000000 sec-certs-0.1.4/tests/data/fips/dataset/fips_modules_historical.html
--rw-r--r--   0 runner    (1001) docker     (123)    59674 2023-05-10 12:00:28.000000 sec-certs-0.1.4/tests/data/fips/dataset/fips_modules_revoked.html
--rw-r--r--   0 runner    (1001) docker     (123)    60283 2023-05-10 12:00:28.000000 sec-certs-0.1.4/tests/data/fips/dataset/template_policy_184097a88a9b4ad9.txt
--rw-r--r--   0 runner    (1001) docker     (123)    75670 2023-05-10 12:00:28.000000 sec-certs-0.1.4/tests/data/fips/dataset/toy_dataset.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:00:38.684648 sec-certs-0.1.4/tests/data/fips/iut/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 12:00:28.000000 sec-certs-0.1.4/tests/data/fips/iut/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    72808 2023-05-10 12:00:28.000000 sec-certs-0.1.4/tests/data/fips/iut/fips_iut_2020-10-25T06+01:00.html
--rw-r--r--   0 runner    (1001) docker     (123)    81803 2023-05-10 12:00:28.000000 sec-certs-0.1.4/tests/data/fips/iut/fips_iut_2021-12-10T06+01:00.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:00:38.684648 sec-certs-0.1.4/tests/data/fips/mip/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 12:00:28.000000 sec-certs-0.1.4/tests/data/fips/mip/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   104771 2023-05-10 12:00:28.000000 sec-certs-0.1.4/tests/data/fips/mip/fips_mip_2020-10-24T06+02:00.html
--rw-r--r--   0 runner    (1001) docker     (123)    85900 2023-05-10 12:00:28.000000 sec-certs-0.1.4/tests/data/fips/mip/fips_mip_2021-02-19T06+01:00.html
--rw-r--r--   0 runner    (1001) docker     (123)   150298 2023-05-10 12:00:28.000000 sec-certs-0.1.4/tests/data/fips/mip/fips_mip_2021-12-19T06+01:00.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:00:38.684648 sec-certs-0.1.4/tests/fips/
--rw-r--r--   0 runner    (1001) docker     (123)     1252 2023-05-10 12:00:28.000000 sec-certs-0.1.4/tests/fips/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1975 2023-05-10 12:00:28.000000 sec-certs-0.1.4/tests/fips/test_fips_algorithm_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     5492 2023-05-10 12:00:28.000000 sec-certs-0.1.4/tests/fips/test_fips_analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)     1875 2023-05-10 12:00:28.000000 sec-certs-0.1.4/tests/fips/test_fips_certificate.py
--rw-r--r--   0 runner    (1001) docker     (123)     4446 2023-05-10 12:00:28.000000 sec-certs-0.1.4/tests/fips/test_fips_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     1948 2023-05-10 12:00:28.000000 sec-certs-0.1.4/tests/fips/test_fips_iut.py
--rw-r--r--   0 runner    (1001) docker     (123)     1981 2023-05-10 12:00:28.000000 sec-certs-0.1.4/tests/fips/test_fips_mip.py
--rw-r--r--   0 runner    (1001) docker     (123)      313 2023-05-10 12:00:28.000000 sec-certs-0.1.4/tests/test_common.py
--rw-r--r--   0 runner    (1001) docker     (123)     2215 2023-05-10 12:00:28.000000 sec-certs-0.1.4/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2528 2023-05-10 12:00:28.000000 sec-certs-0.1.4/tests/test_cpe.py
--rw-r--r--   0 runner    (1001) docker     (123)     4101 2023-05-10 12:00:28.000000 sec-certs-0.1.4/tests/test_cve.py
--rw-r--r--   0 runner    (1001) docker     (123)     2464 2023-05-10 12:00:28.000000 sec-certs-0.1.4/tests/test_cve_matching.py
--rw-r--r--   0 runner    (1001) docker     (123)     3346 2023-05-10 12:00:28.000000 sec-certs-0.1.4/tests/test_nvd_dataset_builder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 13:19:26.665417 sec-certs-0.1.5/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 13:19:26.617414 sec-certs-0.1.5/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 13:19:26.625414 sec-certs-0.1.5/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      619 2023-05-18 13:19:13.000000 sec-certs-0.1.5/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-05-18 13:19:13.000000 sec-certs-0.1.5/.github/ISSUE_TEMPLATE/feature_request.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 13:19:26.625414 sec-certs-0.1.5/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-05-18 13:19:13.000000 sec-certs-0.1.5/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-05-18 13:19:13.000000 sec-certs-0.1.5/.github/workflows/lint.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1662 2023-05-18 13:19:13.000000 sec-certs-0.1.5/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      990 2023-05-18 13:19:13.000000 sec-certs-0.1.5/.github/workflows/tests.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-05-18 13:19:13.000000 sec-certs-0.1.5/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      516 2023-05-18 13:19:13.000000 sec-certs-0.1.5/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3347 2023-05-18 13:19:13.000000 sec-certs-0.1.5/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4265 2023-05-18 13:19:13.000000 sec-certs-0.1.5/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1590 2023-05-18 13:19:13.000000 sec-certs-0.1.5/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-05-18 13:19:13.000000 sec-certs-0.1.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5312 2023-05-18 13:19:26.665417 sec-certs-0.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4250 2023-05-18 13:19:13.000000 sec-certs-0.1.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-05-18 13:19:13.000000 sec-certs-0.1.5/codecov.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 13:19:26.625414 sec-certs-0.1.5/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 13:19:26.625414 sec-certs-0.1.5/data/cert_id_eval/
+-rw-r--r--   0 runner    (1001) docker     (123)     9830 2023-05-18 13:19:13.000000 sec-certs-0.1.5/data/cert_id_eval/duplicate_ids.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     3865 2023-05-18 13:19:13.000000 sec-certs-0.1.5/data/cert_id_eval/missing_ids.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     3358 2023-05-18 13:19:13.000000 sec-certs-0.1.5/data/cert_id_eval/random.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    18418 2023-05-18 13:19:13.000000 sec-certs-0.1.5/data/cert_id_eval/random_references.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     6264 2023-05-18 13:19:13.000000 sec-certs-0.1.5/data/cert_id_eval/truth.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 13:19:26.625414 sec-certs-0.1.5/data/cpe_eval/
+-rw-r--r--   0 runner    (1001) docker     (123)   176434 2023-05-18 13:19:13.000000 sec-certs-0.1.5/data/cpe_eval/manual_cpe_labels.json
+-rw-r--r--   0 runner    (1001) docker     (123)    68713 2023-05-18 13:19:13.000000 sec-certs-0.1.5/data/cpe_eval/random.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 13:19:26.629415 sec-certs-0.1.5/data/information_retrieval_split/
+-rw-r--r--   0 runner    (1001) docker     (123)   117213 2023-05-18 13:19:13.000000 sec-certs-0.1.5/data/information_retrieval_split/metadata.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    85352 2023-05-18 13:19:13.000000 sec-certs-0.1.5/data/information_retrieval_split/sampled_images.json
+-rw-r--r--   0 runner    (1001) docker     (123)    20260 2023-05-18 13:19:13.000000 sec-certs-0.1.5/data/information_retrieval_split/test.json
+-rw-r--r--   0 runner    (1001) docker     (123)    72860 2023-05-18 13:19:13.000000 sec-certs-0.1.5/data/information_retrieval_split/train.json
+-rw-r--r--   0 runner    (1001) docker     (123)     8100 2023-05-18 13:19:13.000000 sec-certs-0.1.5/data/information_retrieval_split/valid.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1046 2023-05-18 13:19:13.000000 sec-certs-0.1.5/data/label_studio_interface.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 13:19:26.629415 sec-certs-0.1.5/data/old_manual_cpe_labels/
+-rw-r--r--   0 runner    (1001) docker     (123)  1552011 2023-05-18 13:19:13.000000 sec-certs-0.1.5/data/old_manual_cpe_labels/cc.json
+-rw-r--r--   0 runner    (1001) docker     (123)  1467792 2023-05-18 13:19:13.000000 sec-certs-0.1.5/data/old_manual_cpe_labels/fips.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2051 2023-05-18 13:19:13.000000 sec-certs-0.1.5/data/readme.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 13:19:26.633415 sec-certs-0.1.5/data/reference_annotations_split/
+-rw-r--r--   0 runner    (1001) docker     (123)    18674 2023-05-18 13:19:13.000000 sec-certs-0.1.5/data/reference_annotations_split/test.json
+-rw-r--r--   0 runner    (1001) docker     (123)    11138 2023-05-18 13:19:13.000000 sec-certs-0.1.5/data/reference_annotations_split/train.json
+-rw-r--r--   0 runner    (1001) docker     (123)     7442 2023-05-18 13:19:13.000000 sec-certs-0.1.5/data/reference_annotations_split/valid.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 13:19:26.633415 sec-certs-0.1.5/data/sar_correlations/
+-rw-r--r--   0 runner    (1001) docker     (123)     1648 2023-05-18 13:19:13.000000 sec-certs-0.1.5/data/sar_correlations/all_certs_sar_cve_corr.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      767 2023-05-18 13:19:13.000000 sec-certs-0.1.5/data/sar_correlations/readme.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1365 2023-05-18 13:19:13.000000 sec-certs-0.1.5/data/sar_correlations/vuln_rich_certs_sar_cve_corr.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 13:19:26.621414 sec-certs-0.1.5/data/validation_test_split/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 13:19:26.633415 sec-certs-0.1.5/data/validation_test_split/cc/
+-rw-r--r--   0 runner    (1001) docker     (123)    55394 2023-05-18 13:19:13.000000 sec-certs-0.1.5/data/validation_test_split/cc/test.json
+-rw-r--r--   0 runner    (1001) docker     (123)    55394 2023-05-18 13:19:13.000000 sec-certs-0.1.5/data/validation_test_split/cc/validation.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 13:19:26.633415 sec-certs-0.1.5/data/validation_test_split/fips/
+-rw-r--r--   0 runner    (1001) docker     (123)    23439 2023-05-18 13:19:13.000000 sec-certs-0.1.5/data/validation_test_split/fips/test.json
+-rw-r--r--   0 runner    (1001) docker     (123)    23434 2023-05-18 13:19:13.000000 sec-certs-0.1.5/data/validation_test_split/fips/validation.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 13:19:26.633415 sec-certs-0.1.5/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-05-18 13:19:13.000000 sec-certs-0.1.5/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 13:19:26.637415 sec-certs-0.1.5/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)    41751 2023-05-18 13:19:13.000000 sec-certs-0.1.5/docs/_static/logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)     3359 2023-05-18 13:19:13.000000 sec-certs-0.1.5/docs/_static/logo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    18611 2023-05-18 13:19:13.000000 sec-certs-0.1.5/docs/_static/logo_badge.png
+-rw-r--r--   0 runner    (1001) docker     (123)     3575 2023-05-18 13:19:13.000000 sec-certs-0.1.5/docs/_static/logo_badge.svg
+-rw-r--r--   0 runner    (1001) docker     (123)   363422 2023-05-18 13:19:13.000000 sec-certs-0.1.5/docs/_static/logolink_OP_VVV_hor_barva_eng.jpg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 13:19:26.637415 sec-certs-0.1.5/docs/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      860 2023-05-18 13:19:13.000000 sec-certs-0.1.5/docs/api/dataset.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1277 2023-05-18 13:19:13.000000 sec-certs-0.1.5/docs/api/model.md
+-rw-r--r--   0 runner    (1001) docker     (123)      506 2023-05-18 13:19:13.000000 sec-certs-0.1.5/docs/api/sample.md
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-18 13:19:13.000000 sec-certs-0.1.5/docs/code_of_conduct.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2669 2023-05-18 13:19:13.000000 sec-certs-0.1.5/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2081 2023-05-18 13:19:13.000000 sec-certs-0.1.5/docs/configuration.md
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-05-18 13:19:13.000000 sec-certs-0.1.5/docs/contributing.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2429 2023-05-18 13:19:13.000000 sec-certs-0.1.5/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1552 2023-05-18 13:19:13.000000 sec-certs-0.1.5/docs/installation.md
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-18 13:19:13.000000 sec-certs-0.1.5/docs/license.md
+-rw-r--r--   0 runner    (1001) docker     (123)      800 2023-05-18 13:19:13.000000 sec-certs-0.1.5/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)     3303 2023-05-18 13:19:13.000000 sec-certs-0.1.5/docs/quickstart.md
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-05-18 13:19:13.000000 sec-certs-0.1.5/docs/readme.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1117 2023-05-18 13:19:13.000000 sec-certs-0.1.5/docs/user_guide.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 13:19:26.637415 sec-certs-0.1.5/notebooks/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 13:19:26.637415 sec-certs-0.1.5/notebooks/cc/
+-rw-r--r--   0 runner    (1001) docker     (123)    13798 2023-05-18 13:19:13.000000 sec-certs-0.1.5/notebooks/cc/cert_id_eval.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     4892 2023-05-18 13:19:13.000000 sec-certs-0.1.5/notebooks/cc/cpe_eval.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 13:19:26.637415 sec-certs-0.1.5/notebooks/cc/reference_annotations/
+-rw-r--r--   0 runner    (1001) docker     (123)     2659 2023-05-18 13:19:13.000000 sec-certs-0.1.5/notebooks/cc/reference_annotations/train_validation_test_split.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    42619 2023-05-18 13:19:13.000000 sec-certs-0.1.5/notebooks/cc/references.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    21943 2023-05-18 13:19:13.000000 sec-certs-0.1.5/notebooks/cc/temporal_trends.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    35405 2023-05-18 13:19:13.000000 sec-certs-0.1.5/notebooks/cc/vulnerabilities.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 13:19:26.641415 sec-certs-0.1.5/notebooks/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     8017 2023-05-18 13:19:13.000000 sec-certs-0.1.5/notebooks/examples/cc.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)   337372 2023-05-18 13:19:13.000000 sec-certs-0.1.5/notebooks/examples/est_solution.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     3952 2023-05-18 13:19:13.000000 sec-certs-0.1.5/notebooks/examples/fips.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     1461 2023-05-18 13:19:13.000000 sec-certs-0.1.5/notebooks/examples/fips_iut.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-05-18 13:19:13.000000 sec-certs-0.1.5/notebooks/examples/fips_mip.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 13:19:26.641415 sec-certs-0.1.5/notebooks/examples/img/
+-rw-r--r--   0 runner    (1001) docker     (123)    29981 2023-05-18 13:19:13.000000 sec-certs-0.1.5/notebooks/examples/img/boxplot_validity.png
+-rw-r--r--   0 runner    (1001) docker     (123)   134946 2023-05-18 13:19:13.000000 sec-certs-0.1.5/notebooks/examples/img/cves_n_days_after_certification.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1755 2023-05-18 13:19:13.000000 sec-certs-0.1.5/notebooks/examples/model.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)   104006 2023-05-18 13:19:13.000000 sec-certs-0.1.5/notebooks/final_run.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 13:19:26.641415 sec-certs-0.1.5/notebooks/fips/
+-rw-r--r--   0 runner    (1001) docker     (123)    15315 2023-05-18 13:19:13.000000 sec-certs-0.1.5/notebooks/fips/in_process.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     2957 2023-05-18 13:19:13.000000 sec-certs-0.1.5/notebooks/fips/references.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    12817 2023-05-18 13:19:13.000000 sec-certs-0.1.5/notebooks/fips/temporal_trends.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)   132824 2023-05-18 13:19:13.000000 sec-certs-0.1.5/notebooks/fips/vulnerabilities.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     9489 2023-05-18 13:19:13.000000 sec-certs-0.1.5/notebooks/latex_plotting.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     8645 2023-05-18 13:19:13.000000 sec-certs-0.1.5/notebooks/ocr.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     3383 2023-05-18 13:19:13.000000 sec-certs-0.1.5/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 13:19:26.641415 sec-certs-0.1.5/requirements/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      361 2023-05-18 13:19:13.000000 sec-certs-0.1.5/requirements/compile.sh
+-rw-r--r--   0 runner    (1001) docker     (123)    10058 2023-05-18 13:19:13.000000 sec-certs-0.1.5/requirements/dev_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5836 2023-05-18 13:19:13.000000 sec-certs-0.1.5/requirements/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6252 2023-05-18 13:19:13.000000 sec-certs-0.1.5/requirements/test_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-18 13:19:13.000000 sec-certs-0.1.5/runtime.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-18 13:19:26.665417 sec-certs-0.1.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 13:19:26.621414 sec-certs-0.1.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 13:19:26.641415 sec-certs-0.1.5/src/sec_certs/
+-rw-r--r--   0 runner    (1001) docker     (123)      521 2023-05-18 13:19:13.000000 sec-certs-0.1.5/src/sec_certs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-05-18 13:19:13.000000 sec-certs-0.1.5/src/sec_certs/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-18 13:19:26.000000 sec-certs-0.1.5/src/sec_certs/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5927 2023-05-18 13:19:13.000000 sec-certs-0.1.5/src/sec_certs/cert_rules.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7820 2023-05-18 13:19:13.000000 sec-certs-0.1.5/src/sec_certs/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7024 2023-05-18 13:19:13.000000 sec-certs-0.1.5/src/sec_certs/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6847 2023-05-18 13:19:13.000000 sec-certs-0.1.5/src/sec_certs/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 13:19:26.645416 sec-certs-0.1.5/src/sec_certs/dataset/
+-rw-r--r--   0 runner    (1001) docker     (123)      872 2023-05-18 13:19:13.000000 sec-certs-0.1.5/src/sec_certs/dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39111 2023-05-18 13:19:13.000000 sec-certs-0.1.5/src/sec_certs/dataset/cc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1854 2023-05-18 13:19:13.000000 sec-certs-0.1.5/src/sec_certs/dataset/cc_scheme.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4340 2023-05-18 13:19:13.000000 sec-certs-0.1.5/src/sec_certs/dataset/cpe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7578 2023-05-18 13:19:13.000000 sec-certs-0.1.5/src/sec_certs/dataset/cve.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25690 2023-05-18 13:19:13.000000 sec-certs-0.1.5/src/sec_certs/dataset/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14789 2023-05-18 13:19:13.000000 sec-certs-0.1.5/src/sec_certs/dataset/fips.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5106 2023-05-18 13:19:13.000000 sec-certs-0.1.5/src/sec_certs/dataset/fips_algorithm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2187 2023-05-18 13:19:13.000000 sec-certs-0.1.5/src/sec_certs/dataset/fips_iut.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3749 2023-05-18 13:19:13.000000 sec-certs-0.1.5/src/sec_certs/dataset/fips_mip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-05-18 13:19:13.000000 sec-certs-0.1.5/src/sec_certs/dataset/json_path_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3078 2023-05-18 13:19:13.000000 sec-certs-0.1.5/src/sec_certs/dataset/protection_profile.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 13:19:26.645416 sec-certs-0.1.5/src/sec_certs/model/
+-rw-r--r--   0 runner    (1001) docker     (123)      793 2023-05-18 13:19:13.000000 sec-certs-0.1.5/src/sec_certs/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4485 2023-05-18 13:19:13.000000 sec-certs-0.1.5/src/sec_certs/model/cc_matching.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18209 2023-05-18 13:19:13.000000 sec-certs-0.1.5/src/sec_certs/model/cpe_matching.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3719 2023-05-18 13:19:13.000000 sec-certs-0.1.5/src/sec_certs/model/evaluation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3322 2023-05-18 13:19:13.000000 sec-certs-0.1.5/src/sec_certs/model/fips_matching.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1918 2023-05-18 13:19:13.000000 sec-certs-0.1.5/src/sec_certs/model/matching.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9532 2023-05-18 13:19:13.000000 sec-certs-0.1.5/src/sec_certs/model/reference_finder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7337 2023-05-18 13:19:13.000000 sec-certs-0.1.5/src/sec_certs/model/sar_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5186 2023-05-18 13:19:13.000000 sec-certs-0.1.5/src/sec_certs/model/transitive_vulnerability_finder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27743 2023-05-18 13:19:13.000000 sec-certs-0.1.5/src/sec_certs/rules.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 13:19:26.649416 sec-certs-0.1.5/src/sec_certs/sample/
+-rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-05-18 13:19:13.000000 sec-certs-0.1.5/src/sec_certs/sample/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42917 2023-05-18 13:19:13.000000 sec-certs-0.1.5/src/sec_certs/sample/cc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4745 2023-05-18 13:19:13.000000 sec-certs-0.1.5/src/sec_certs/sample/cc_certificate_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2894 2023-05-18 13:19:13.000000 sec-certs-0.1.5/src/sec_certs/sample/cc_maintenance_update.py
+-rw-r--r--   0 runner    (1001) docker     (123)    65455 2023-05-18 13:19:13.000000 sec-certs-0.1.5/src/sec_certs/sample/cc_scheme.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2599 2023-05-18 13:19:13.000000 sec-certs-0.1.5/src/sec_certs/sample/certificate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6508 2023-05-18 13:19:13.000000 sec-certs-0.1.5/src/sec_certs/sample/cpe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9310 2023-05-18 13:19:13.000000 sec-certs-0.1.5/src/sec_certs/sample/cve.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29341 2023-05-18 13:19:13.000000 sec-certs-0.1.5/src/sec_certs/sample/fips.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-05-18 13:19:13.000000 sec-certs-0.1.5/src/sec_certs/sample/fips_algorithm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5541 2023-05-18 13:19:13.000000 sec-certs-0.1.5/src/sec_certs/sample/fips_iut.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9337 2023-05-18 13:19:13.000000 sec-certs-0.1.5/src/sec_certs/sample/fips_mip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1951 2023-05-18 13:19:13.000000 sec-certs-0.1.5/src/sec_certs/sample/protection_profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1736 2023-05-18 13:19:13.000000 sec-certs-0.1.5/src/sec_certs/sample/sar.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 13:19:26.649416 sec-certs-0.1.5/src/sec_certs/serialization/
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-18 13:19:13.000000 sec-certs-0.1.5/src/sec_certs/serialization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6813 2023-05-18 13:19:13.000000 sec-certs-0.1.5/src/sec_certs/serialization/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-05-18 13:19:13.000000 sec-certs-0.1.5/src/sec_certs/serialization/pandas.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 13:19:26.649416 sec-certs-0.1.5/src/sec_certs/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-18 13:19:13.000000 sec-certs-0.1.5/src/sec_certs/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38410 2023-05-18 13:19:13.000000 sec-certs-0.1.5/src/sec_certs/utils/extract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7812 2023-05-18 13:19:13.000000 sec-certs-0.1.5/src/sec_certs/utils/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14804 2023-05-18 13:19:13.000000 sec-certs-0.1.5/src/sec_certs/utils/nvd_dataset_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21941 2023-05-18 13:19:13.000000 sec-certs-0.1.5/src/sec_certs/utils/pandas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-05-18 13:19:13.000000 sec-certs-0.1.5/src/sec_certs/utils/parallel_processing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9625 2023-05-18 13:19:13.000000 sec-certs-0.1.5/src/sec_certs/utils/pdf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1549 2023-05-18 13:19:13.000000 sec-certs-0.1.5/src/sec_certs/utils/sanitization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-05-18 13:19:13.000000 sec-certs-0.1.5/src/sec_certs/utils/strings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2015 2023-05-18 13:19:13.000000 sec-certs-0.1.5/src/sec_certs/utils/tables.py
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-05-18 13:19:13.000000 sec-certs-0.1.5/src/sec_certs/utils/tqdm.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 13:19:26.641415 sec-certs-0.1.5/src/sec_certs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5312 2023-05-18 13:19:26.000000 sec-certs-0.1.5/src/sec_certs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7272 2023-05-18 13:19:26.000000 sec-certs-0.1.5/src/sec_certs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 13:19:26.000000 sec-certs-0.1.5/src/sec_certs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-18 13:19:26.000000 sec-certs-0.1.5/src/sec_certs.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-05-18 13:19:26.000000 sec-certs-0.1.5/src/sec_certs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-18 13:19:26.000000 sec-certs-0.1.5/src/sec_certs.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 13:19:26.653416 sec-certs-0.1.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 13:19:13.000000 sec-certs-0.1.5/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 13:19:26.653416 sec-certs-0.1.5/tests/cc/
+-rw-r--r--   0 runner    (1001) docker     (123)     2223 2023-05-18 13:19:13.000000 sec-certs-0.1.5/tests/cc/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8414 2023-05-18 13:19:13.000000 sec-certs-0.1.5/tests/cc/test_cc_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2958 2023-05-18 13:19:13.000000 sec-certs-0.1.5/tests/cc/test_cc_certificate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5997 2023-05-18 13:19:13.000000 sec-certs-0.1.5/tests/cc/test_cc_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3199 2023-05-18 13:19:13.000000 sec-certs-0.1.5/tests/cc/test_cc_maintenance_updates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1512 2023-05-18 13:19:13.000000 sec-certs-0.1.5/tests/cc/test_cc_misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8012 2023-05-18 13:19:13.000000 sec-certs-0.1.5/tests/cc/test_cc_schemes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1400 2023-05-18 13:19:13.000000 sec-certs-0.1.5/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 13:19:26.653416 sec-certs-0.1.5/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 13:19:13.000000 sec-certs-0.1.5/tests/data/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 13:19:26.653416 sec-certs-0.1.5/tests/data/cc/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 13:19:13.000000 sec-certs-0.1.5/tests/data/cc/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 13:19:26.653416 sec-certs-0.1.5/tests/data/cc/analysis/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 13:19:13.000000 sec-certs-0.1.5/tests/data/cc/analysis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30505 2023-05-18 13:19:13.000000 sec-certs-0.1.5/tests/data/cc/analysis/cc_full_dataset.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 13:19:26.621414 sec-certs-0.1.5/tests/data/cc/analysis/certs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 13:19:26.621414 sec-certs-0.1.5/tests/data/cc/analysis/certs/reports/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 13:19:26.653416 sec-certs-0.1.5/tests/data/cc/analysis/certs/reports/pdf/
+-rw-r--r--   0 runner    (1001) docker     (123)  1174271 2023-05-18 13:19:13.000000 sec-certs-0.1.5/tests/data/cc/analysis/certs/reports/pdf/ebd276cca70fd723.pdf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 13:19:26.657416 sec-certs-0.1.5/tests/data/cc/analysis/certs/reports/txt/
+-rw-r--r--   0 runner    (1001) docker     (123)    58767 2023-05-18 13:19:13.000000 sec-certs-0.1.5/tests/data/cc/analysis/certs/reports/txt/ebd276cca70fd723.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 13:19:26.621414 sec-certs-0.1.5/tests/data/cc/analysis/certs/targets/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 13:19:26.657416 sec-certs-0.1.5/tests/data/cc/analysis/certs/targets/pdf/
+-rw-r--r--   0 runner    (1001) docker     (123)   615034 2023-05-18 13:19:13.000000 sec-certs-0.1.5/tests/data/cc/analysis/certs/targets/pdf/ebd276cca70fd723.pdf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 13:19:26.657416 sec-certs-0.1.5/tests/data/cc/analysis/certs/targets/txt/
+-rw-r--r--   0 runner    (1001) docker     (123)    98275 2023-05-18 13:19:13.000000 sec-certs-0.1.5/tests/data/cc/analysis/certs/targets/txt/ebd276cca70fd723.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    53839 2023-05-18 13:19:13.000000 sec-certs-0.1.5/tests/data/cc/analysis/reference_dataset.json
+-rw-r--r--   0 runner    (1001) docker     (123)   103359 2023-05-18 13:19:13.000000 sec-certs-0.1.5/tests/data/cc/analysis/transitive_vulnerability_dataset.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4797 2023-05-18 13:19:13.000000 sec-certs-0.1.5/tests/data/cc/analysis/vulnerable_dataset.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 13:19:26.657416 sec-certs-0.1.5/tests/data/cc/certificate/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 13:19:13.000000 sec-certs-0.1.5/tests/data/cc/certificate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3258 2023-05-18 13:19:13.000000 sec-certs-0.1.5/tests/data/cc/certificate/fictional_cert.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 13:19:26.657416 sec-certs-0.1.5/tests/data/cc/dataset/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 13:19:13.000000 sec-certs-0.1.5/tests/data/cc/dataset/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 13:19:26.621414 sec-certs-0.1.5/tests/data/cc/dataset/auxiliary_datasets/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 13:19:26.657416 sec-certs-0.1.5/tests/data/cc/dataset/auxiliary_datasets/maintenances/
+-rw-r--r--   0 runner    (1001) docker     (123)     3515 2023-05-18 13:19:13.000000 sec-certs-0.1.5/tests/data/cc/dataset/auxiliary_datasets/maintenances/maintenance_updates.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1817 2023-05-18 13:19:13.000000 sec-certs-0.1.5/tests/data/cc/dataset/cc_products_active.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    31505 2023-05-18 13:19:13.000000 sec-certs-0.1.5/tests/data/cc/dataset/cc_products_active.html
+-rw-r--r--   0 runner    (1001) docker     (123)    22545 2023-05-18 13:19:13.000000 sec-certs-0.1.5/tests/data/cc/dataset/report_309ac2fd7f2dcf17.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    72568 2023-05-18 13:19:13.000000 sec-certs-0.1.5/tests/data/cc/dataset/target_309ac2fd7f2dcf17.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    12359 2023-05-18 13:19:13.000000 sec-certs-0.1.5/tests/data/cc/dataset/toy_dataset.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 13:19:26.661417 sec-certs-0.1.5/tests/data/common/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 13:19:13.000000 sec-certs-0.1.5/tests/data/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1990 2023-05-18 13:19:13.000000 sec-certs-0.1.5/tests/data/common/cpe_dataset.json
+-rw-r--r--   0 runner    (1001) docker     (123)    88427 2023-05-18 13:19:13.000000 sec-certs-0.1.5/tests/data/common/cpe_match_feed.json
+-rw-r--r--   0 runner    (1001) docker     (123)    31329 2023-05-18 13:19:13.000000 sec-certs-0.1.5/tests/data/common/cve_dataset.json
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-18 13:19:13.000000 sec-certs-0.1.5/tests/data/common/settings_tests.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 13:19:26.621414 sec-certs-0.1.5/tests/data/fips/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 13:19:26.661417 sec-certs-0.1.5/tests/data/fips/certificate/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 13:19:13.000000 sec-certs-0.1.5/tests/data/fips/certificate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2741 2023-05-18 13:19:13.000000 sec-certs-0.1.5/tests/data/fips/certificate/fictional_cert.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 13:19:26.661417 sec-certs-0.1.5/tests/data/fips/dataset/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 13:19:13.000000 sec-certs-0.1.5/tests/data/fips/dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-05-18 13:19:13.000000 sec-certs-0.1.5/tests/data/fips/dataset/alg_dataset.json
+-rw-r--r--   0 runner    (1001) docker     (123)    45964 2023-05-18 13:19:13.000000 sec-certs-0.1.5/tests/data/fips/dataset/fips_modules_active.html
+-rw-r--r--   0 runner    (1001) docker     (123)    54952 2023-05-18 13:19:13.000000 sec-certs-0.1.5/tests/data/fips/dataset/fips_modules_historical.html
+-rw-r--r--   0 runner    (1001) docker     (123)    59674 2023-05-18 13:19:13.000000 sec-certs-0.1.5/tests/data/fips/dataset/fips_modules_revoked.html
+-rw-r--r--   0 runner    (1001) docker     (123)    60283 2023-05-18 13:19:13.000000 sec-certs-0.1.5/tests/data/fips/dataset/template_policy_184097a88a9b4ad9.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    75670 2023-05-18 13:19:13.000000 sec-certs-0.1.5/tests/data/fips/dataset/toy_dataset.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 13:19:26.661417 sec-certs-0.1.5/tests/data/fips/iut/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 13:19:13.000000 sec-certs-0.1.5/tests/data/fips/iut/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    72808 2023-05-18 13:19:13.000000 sec-certs-0.1.5/tests/data/fips/iut/fips_iut_2020-10-25T06+01:00.html
+-rw-r--r--   0 runner    (1001) docker     (123)    81803 2023-05-18 13:19:13.000000 sec-certs-0.1.5/tests/data/fips/iut/fips_iut_2021-12-10T06+01:00.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 13:19:26.661417 sec-certs-0.1.5/tests/data/fips/mip/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 13:19:13.000000 sec-certs-0.1.5/tests/data/fips/mip/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   104771 2023-05-18 13:19:13.000000 sec-certs-0.1.5/tests/data/fips/mip/fips_mip_2020-10-24T06+02:00.html
+-rw-r--r--   0 runner    (1001) docker     (123)    85900 2023-05-18 13:19:13.000000 sec-certs-0.1.5/tests/data/fips/mip/fips_mip_2021-02-19T06+01:00.html
+-rw-r--r--   0 runner    (1001) docker     (123)   150298 2023-05-18 13:19:13.000000 sec-certs-0.1.5/tests/data/fips/mip/fips_mip_2021-12-19T06+01:00.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 13:19:26.665417 sec-certs-0.1.5/tests/fips/
+-rw-r--r--   0 runner    (1001) docker     (123)     1252 2023-05-18 13:19:13.000000 sec-certs-0.1.5/tests/fips/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1975 2023-05-18 13:19:13.000000 sec-certs-0.1.5/tests/fips/test_fips_algorithm_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5492 2023-05-18 13:19:13.000000 sec-certs-0.1.5/tests/fips/test_fips_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1875 2023-05-18 13:19:13.000000 sec-certs-0.1.5/tests/fips/test_fips_certificate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4446 2023-05-18 13:19:13.000000 sec-certs-0.1.5/tests/fips/test_fips_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1948 2023-05-18 13:19:13.000000 sec-certs-0.1.5/tests/fips/test_fips_iut.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1981 2023-05-18 13:19:13.000000 sec-certs-0.1.5/tests/fips/test_fips_mip.py
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-05-18 13:19:13.000000 sec-certs-0.1.5/tests/test_common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2215 2023-05-18 13:19:13.000000 sec-certs-0.1.5/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2528 2023-05-18 13:19:13.000000 sec-certs-0.1.5/tests/test_cpe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4101 2023-05-18 13:19:13.000000 sec-certs-0.1.5/tests/test_cve.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2464 2023-05-18 13:19:13.000000 sec-certs-0.1.5/tests/test_cve_matching.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3346 2023-05-18 13:19:13.000000 sec-certs-0.1.5/tests/test_nvd_dataset_builder.py
```

### Comparing `sec-certs-0.1.4/.github/ISSUE_TEMPLATE/bug_report.md` & `sec-certs-0.1.5/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `sec-certs-0.1.4/.github/ISSUE_TEMPLATE/feature_request.md` & `sec-certs-0.1.5/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `sec-certs-0.1.4/.github/workflows/docs.yml` & `sec-certs-0.1.5/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `sec-certs-0.1.4/.github/workflows/lint.yml` & `sec-certs-0.1.5/.github/workflows/lint.yml`

 * *Files identical despite different names*

### Comparing `sec-certs-0.1.4/.github/workflows/release.yml` & `sec-certs-0.1.5/.github/workflows/release.yml`

 * *Files 14% similar despite different names*

```diff
@@ -4,14 +4,19 @@
     types: [published]
 
 jobs:
   pypi_release:
     name: Release on PyPi
     runs-on: ubuntu-latest
     if: github.repository == 'crocs-muni/sec-certs'
+    environment:
+      name: pypi
+      url: https://pypi.org/project/sec-certs/
+    permissions:
+      id-token: write
     steps:
       - uses: actions/checkout@v3
         with:
           fetch-depth: 0
       - name: Set up Python
         uses: actions/setup-python@v4
         with:
@@ -19,17 +24,14 @@
       - name: Install build dependencies
         run: python -m pip install build
       - name: Build distributions
         shell: bash -l {0}
         run: python -m build
       - name: Publish package to PyPI
         uses: pypa/gh-action-pypi-publish@release/v1
-        with:
-          user: ${{ secrets.PYPI_USERNAME }}
-          password: ${{ secrets.PYPI_PASSWORD }}
   docker_release:
     name: Release on DockerHub
     runs-on: ubuntu-latest
     if: github.repository == 'crocs-muni/sec-certs'
     steps:
       - name: Set up QEMU
         uses: docker/setup-qemu-action@v1
```

### Comparing `sec-certs-0.1.4/.github/workflows/tests.yml` & `sec-certs-0.1.5/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `sec-certs-0.1.4/.gitignore` & `sec-certs-0.1.5/.gitignore`

 * *Files identical despite different names*

### Comparing `sec-certs-0.1.4/.pre-commit-config.yaml` & `sec-certs-0.1.5/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `sec-certs-0.1.4/CODE_OF_CONDUCT.md` & `sec-certs-0.1.5/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `sec-certs-0.1.4/CONTRIBUTING.md` & `sec-certs-0.1.5/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `sec-certs-0.1.4/Dockerfile` & `sec-certs-0.1.5/Dockerfile`

 * *Files identical despite different names*

### Comparing `sec-certs-0.1.4/LICENSE` & `sec-certs-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `sec-certs-0.1.4/PKG-INFO` & `sec-certs-0.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sec-certs
-Version: 0.1.4
+Version: 0.1.5
 Summary: A tool for data scraping and analysis of security certificates from Common Criteria and FIPS 140-2/3 frameworks
 Author: Jan Jancar, Petr Svenda, Jiri Michalik, Stanislav Bobon
 Author-email: Adam Janovsky <adamjanovsky@mail.muni.cz>
 License: MIT
 Project-URL: Homepage, https://seccerts.org
 Project-URL: GitHub, https://github.com/crocs-muni/sec-certs/
 Project-URL: Documentation, https://seccerts.org/docs
```

### Comparing `sec-certs-0.1.4/README.md` & `sec-certs-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `sec-certs-0.1.4/data/cert_id_eval/duplicate_ids.csv` & `sec-certs-0.1.5/data/cert_id_eval/duplicate_ids.csv`

 * *Files identical despite different names*

### Comparing `sec-certs-0.1.4/data/cert_id_eval/missing_ids.csv` & `sec-certs-0.1.5/data/cert_id_eval/missing_ids.csv`

 * *Files identical despite different names*

### Comparing `sec-certs-0.1.4/data/cert_id_eval/random.csv` & `sec-certs-0.1.5/data/cert_id_eval/random.csv`

 * *Files identical despite different names*

### Comparing `sec-certs-0.1.4/data/cert_id_eval/random_references.csv` & `sec-certs-0.1.5/data/cert_id_eval/random_references.csv`

 * *Files identical despite different names*

### Comparing `sec-certs-0.1.4/data/cert_id_eval/truth.csv` & `sec-certs-0.1.5/data/cert_id_eval/truth.csv`

 * *Files identical despite different names*

### Comparing `sec-certs-0.1.4/data/cpe_eval/manual_cpe_labels.json` & `sec-certs-0.1.5/data/cpe_eval/manual_cpe_labels.json`

 * *Files identical despite different names*

### Comparing `sec-certs-0.1.4/data/cpe_eval/random.csv` & `sec-certs-0.1.5/data/cpe_eval/random.csv`

 * *Files identical despite different names*

### Comparing `sec-certs-0.1.4/data/information_retrieval_split/metadata.csv` & `sec-certs-0.1.5/data/information_retrieval_split/metadata.csv`

 * *Files identical despite different names*

### Comparing `sec-certs-0.1.4/data/information_retrieval_split/sampled_images.json` & `sec-certs-0.1.5/data/information_retrieval_split/sampled_images.json`

 * *Files identical despite different names*

### Comparing `sec-certs-0.1.4/data/information_retrieval_split/test.json` & `sec-certs-0.1.5/data/information_retrieval_split/test.json`

 * *Files identical despite different names*

### Comparing `sec-certs-0.1.4/data/information_retrieval_split/train.json` & `sec-certs-0.1.5/data/information_retrieval_split/train.json`

 * *Files identical despite different names*

### Comparing `sec-certs-0.1.4/data/information_retrieval_split/valid.json` & `sec-certs-0.1.5/data/information_retrieval_split/valid.json`

 * *Files identical despite different names*

### Comparing `sec-certs-0.1.4/data/label_studio_interface.txt` & `sec-certs-0.1.5/data/label_studio_interface.txt`

 * *Files identical despite different names*

### Comparing `sec-certs-0.1.4/data/old_manual_cpe_labels/cc.json` & `sec-certs-0.1.5/data/old_manual_cpe_labels/cc.json`

 * *Files identical despite different names*

### Comparing `sec-certs-0.1.4/data/old_manual_cpe_labels/fips.json` & `sec-certs-0.1.5/data/old_manual_cpe_labels/fips.json`

 * *Files identical despite different names*

### Comparing `sec-certs-0.1.4/data/readme.md` & `sec-certs-0.1.5/data/readme.md`

 * *Files identical despite different names*

### Comparing `sec-certs-0.1.4/data/reference_annotations_split/test.json` & `sec-certs-0.1.5/data/reference_annotations_split/test.json`

 * *Files identical despite different names*

### Comparing `sec-certs-0.1.4/data/reference_annotations_split/train.json` & `sec-certs-0.1.5/data/reference_annotations_split/train.json`

 * *Files identical despite different names*

### Comparing `sec-certs-0.1.4/data/reference_annotations_split/valid.json` & `sec-certs-0.1.5/data/reference_annotations_split/valid.json`

 * *Files identical despite different names*

### Comparing `sec-certs-0.1.4/data/sar_correlations/all_certs_sar_cve_corr.csv` & `sec-certs-0.1.5/data/sar_correlations/all_certs_sar_cve_corr.csv`

 * *Files identical despite different names*

### Comparing `sec-certs-0.1.4/data/sar_correlations/readme.md` & `sec-certs-0.1.5/data/sar_correlations/readme.md`

 * *Files identical despite different names*

### Comparing `sec-certs-0.1.4/data/sar_correlations/vuln_rich_certs_sar_cve_corr.csv` & `sec-certs-0.1.5/data/sar_correlations/vuln_rich_certs_sar_cve_corr.csv`

 * *Files identical despite different names*

### Comparing `sec-certs-0.1.4/data/validation_test_split/cc/test.json` & `sec-certs-0.1.5/data/validation_test_split/cc/test.json`

 * *Files identical despite different names*

### Comparing `sec-certs-0.1.4/data/validation_test_split/cc/validation.json` & `sec-certs-0.1.5/data/validation_test_split/cc/validation.json`

 * *Files identical despite different names*

### Comparing `sec-certs-0.1.4/data/validation_test_split/fips/test.json` & `sec-certs-0.1.5/data/validation_test_split/fips/test.json`

 * *Files identical despite different names*

### Comparing `sec-certs-0.1.4/data/validation_test_split/fips/validation.json` & `sec-certs-0.1.5/data/validation_test_split/fips/validation.json`

 * *Files identical despite different names*

### Comparing `sec-certs-0.1.4/docs/Makefile` & `sec-certs-0.1.5/docs/Makefile`

 * *Files identical despite different names*

### Comparing `sec-certs-0.1.4/docs/_static/logo.png` & `sec-certs-0.1.5/docs/_static/logo.png`

 * *Files identical despite different names*

### Comparing `sec-certs-0.1.4/docs/_static/logo.svg` & `sec-certs-0.1.5/docs/_static/logo.svg`

 * *Files identical despite different names*

### Comparing `sec-certs-0.1.4/docs/_static/logo_badge.png` & `sec-certs-0.1.5/docs/_static/logo_badge.png`

 * *Files identical despite different names*

### Comparing `sec-certs-0.1.4/docs/_static/logo_badge.svg` & `sec-certs-0.1.5/docs/_static/logo_badge.svg`

 * *Files identical despite different names*

### Comparing `sec-certs-0.1.4/docs/_static/logolink_OP_VVV_hor_barva_eng.jpg` & `sec-certs-0.1.5/docs/_static/logolink_OP_VVV_hor_barva_eng.jpg`

 * *Files identical despite different names*

### Comparing `sec-certs-0.1.4/docs/api/dataset.md` & `sec-certs-0.1.5/docs/api/dataset.md`

 * *Files identical despite different names*

### Comparing `sec-certs-0.1.4/docs/api/model.md` & `sec-certs-0.1.5/docs/api/model.md`

 * *Files identical despite different names*

### Comparing `sec-certs-0.1.4/docs/conf.py` & `sec-certs-0.1.5/docs/conf.py`

 * *Files identical despite different names*

### Comparing `sec-certs-0.1.4/docs/configuration.md` & `sec-certs-0.1.5/docs/configuration.md`

 * *Files identical despite different names*

### Comparing `sec-certs-0.1.4/docs/index.md` & `sec-certs-0.1.5/docs/index.md`

 * *Files identical despite different names*

### Comparing `sec-certs-0.1.4/docs/installation.md` & `sec-certs-0.1.5/docs/installation.md`

 * *Files identical despite different names*

### Comparing `sec-certs-0.1.4/docs/make.bat` & `sec-certs-0.1.5/docs/make.bat`

 * *Files identical despite different names*

### Comparing `sec-certs-0.1.4/docs/quickstart.md` & `sec-certs-0.1.5/docs/quickstart.md`

 * *Files identical despite different names*

### Comparing `sec-certs-0.1.4/docs/user_guide.md` & `sec-certs-0.1.5/docs/user_guide.md`

 * *Files identical despite different names*

### Comparing `sec-certs-0.1.4/notebooks/cc/cert_id_eval.ipynb` & `sec-certs-0.1.5/notebooks/cc/cert_id_eval.ipynb`

 * *Files identical despite different names*

### Comparing `sec-certs-0.1.4/notebooks/cc/cpe_eval.ipynb` & `sec-certs-0.1.5/notebooks/cc/cpe_eval.ipynb`

 * *Files identical despite different names*

### Comparing `sec-certs-0.1.4/notebooks/cc/reference_annotations/train_validation_test_split.ipynb` & `sec-certs-0.1.5/notebooks/cc/reference_annotations/train_validation_test_split.ipynb`

 * *Files identical despite different names*

### Comparing `sec-certs-0.1.4/notebooks/cc/references.ipynb` & `sec-certs-0.1.5/notebooks/cc/references.ipynb`

 * *Files identical despite different names*

### Comparing `sec-certs-0.1.4/notebooks/cc/temporal_trends.ipynb` & `sec-certs-0.1.5/notebooks/cc/temporal_trends.ipynb`

 * *Files identical despite different names*

### Comparing `sec-certs-0.1.4/notebooks/cc/vulnerabilities.ipynb` & `sec-certs-0.1.5/notebooks/cc/vulnerabilities.ipynb`

 * *Files identical despite different names*

### Comparing `sec-certs-0.1.4/notebooks/examples/cc.ipynb` & `sec-certs-0.1.5/notebooks/examples/cc.ipynb`

 * *Files identical despite different names*

### Comparing `sec-certs-0.1.4/notebooks/examples/est_solution.ipynb` & `sec-certs-0.1.5/notebooks/examples/est_solution.ipynb`

 * *Files identical despite different names*

### Comparing `sec-certs-0.1.4/notebooks/examples/fips.ipynb` & `sec-certs-0.1.5/notebooks/examples/fips.ipynb`

 * *Files identical despite different names*

### Comparing `sec-certs-0.1.4/notebooks/examples/fips_iut.ipynb` & `sec-certs-0.1.5/notebooks/examples/fips_iut.ipynb`

 * *Files identical despite different names*

### Comparing `sec-certs-0.1.4/notebooks/examples/fips_mip.ipynb` & `sec-certs-0.1.5/notebooks/examples/fips_mip.ipynb`

 * *Files identical despite different names*

### Comparing `sec-certs-0.1.4/notebooks/examples/img/boxplot_validity.png` & `sec-certs-0.1.5/notebooks/examples/img/boxplot_validity.png`

 * *Files identical despite different names*

### Comparing `sec-certs-0.1.4/notebooks/examples/img/cves_n_days_after_certification.png` & `sec-certs-0.1.5/notebooks/examples/img/cves_n_days_after_certification.png`

 * *Files identical despite different names*

### Comparing `sec-certs-0.1.4/notebooks/examples/model.ipynb` & `sec-certs-0.1.5/notebooks/examples/model.ipynb`

 * *Files identical despite different names*

### Comparing `sec-certs-0.1.4/notebooks/final_run.ipynb` & `sec-certs-0.1.5/notebooks/final_run.ipynb`

 * *Files identical despite different names*

### Comparing `sec-certs-0.1.4/notebooks/fips/in_process.ipynb` & `sec-certs-0.1.5/notebooks/fips/in_process.ipynb`

 * *Files identical despite different names*

### Comparing `sec-certs-0.1.4/notebooks/fips/references.ipynb` & `sec-certs-0.1.5/notebooks/fips/references.ipynb`

 * *Files identical despite different names*

### Comparing `sec-certs-0.1.4/notebooks/fips/temporal_trends.ipynb` & `sec-certs-0.1.5/notebooks/fips/temporal_trends.ipynb`

 * *Files identical despite different names*

### Comparing `sec-certs-0.1.4/notebooks/fips/vulnerabilities.ipynb` & `sec-certs-0.1.5/notebooks/fips/vulnerabilities.ipynb`

 * *Files identical despite different names*

### Comparing `sec-certs-0.1.4/notebooks/latex_plotting.ipynb` & `sec-certs-0.1.5/notebooks/latex_plotting.ipynb`

 * *Files identical despite different names*

### Comparing `sec-certs-0.1.4/notebooks/ocr.ipynb` & `sec-certs-0.1.5/notebooks/ocr.ipynb`

 * *Files identical despite different names*

### Comparing `sec-certs-0.1.4/pyproject.toml` & `sec-certs-0.1.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `sec-certs-0.1.4/requirements/dev_requirements.txt` & `sec-certs-0.1.5/requirements/dev_requirements.txt`

 * *Files identical despite different names*

### Comparing `sec-certs-0.1.4/requirements/requirements.txt` & `sec-certs-0.1.5/requirements/requirements.txt`

 * *Files identical despite different names*

### Comparing `sec-certs-0.1.4/requirements/test_requirements.txt` & `sec-certs-0.1.5/requirements/test_requirements.txt`

 * *Files identical despite different names*

### Comparing `sec-certs-0.1.4/src/sec_certs/__init__.py` & `sec-certs-0.1.5/src/sec_certs/__init__.py`

 * *Files identical despite different names*

### Comparing `sec-certs-0.1.4/src/sec_certs/cert_rules.py` & `sec-certs-0.1.5/src/sec_certs/cert_rules.py`

 * *Files identical despite different names*

### Comparing `sec-certs-0.1.4/src/sec_certs/cli.py` & `sec-certs-0.1.5/src/sec_certs/cli.py`

 * *Files identical despite different names*

### Comparing `sec-certs-0.1.4/src/sec_certs/configuration.py` & `sec-certs-0.1.5/src/sec_certs/configuration.py`

 * *Files identical despite different names*

### Comparing `sec-certs-0.1.4/src/sec_certs/constants.py` & `sec-certs-0.1.5/src/sec_certs/constants.py`

 * *Files identical despite different names*

### Comparing `sec-certs-0.1.4/src/sec_certs/dataset/__init__.py` & `sec-certs-0.1.5/src/sec_certs/dataset/__init__.py`

 * *Files identical despite different names*

### Comparing `sec-certs-0.1.4/src/sec_certs/dataset/cc.py` & `sec-certs-0.1.5/src/sec_certs/dataset/cc.py`

 * *Files 0% similar despite different names*

```diff
@@ -75,16 +75,16 @@
     def to_pandas(self) -> pd.DataFrame:
         """
         Return self serialized into pandas DataFrame
         """
         df = pd.DataFrame([x.pandas_tuple for x in self.certs.values()], columns=CCCertificate.pandas_columns)
         df = df.set_index("dgst")
 
-        df.not_valid_before = pd.to_datetime(df.not_valid_before, infer_datetime_format=True)
-        df.not_valid_after = pd.to_datetime(df.not_valid_after, infer_datetime_format=True)
+        df.not_valid_before = pd.to_datetime(df.not_valid_before, infer_datetime_format=True, errors="coerce")
+        df.not_valid_after = pd.to_datetime(df.not_valid_after, infer_datetime_format=True, errors="coerce")
         df = df.astype(
             {"category": "category", "status": "category", "scheme": "category", "cert_lab": "category"}
         ).fillna(value=np.nan)
         df = df.loc[
             ~df.manufacturer.isnull()
         ]  # Manually delete one certificate with None manufacturer (seems to have many blank fields)
 
@@ -357,15 +357,15 @@
         df = df.rename(columns=dict(zip(list(df.columns), csv_header)))
 
         df["is_maintenance"] = ~df.maintenance_title.isnull()
         df = df.fillna(value="")
 
         df[["not_valid_before", "not_valid_after", "maintenance_date"]] = df[
             ["not_valid_before", "not_valid_after", "maintenance_date"]
-        ].apply(pd.to_datetime)
+        ].apply(pd.to_datetime, errors="coerce")
 
         df["dgst"] = df.apply(lambda row: helpers.get_first_16_bytes_sha256(_get_primary_key_str(row)), axis=1)
 
         df_base = df.loc[~df.is_maintenance].copy()
         df_main = df.loc[df.is_maintenance].copy()
 
         df_base.report_link = df_base.report_link.map(map_ip_to_hostname)
@@ -893,15 +893,15 @@
         return dset
 
     def to_pandas(self) -> pd.DataFrame:
         df = pd.DataFrame([x.pandas_tuple for x in self.certs.values()], columns=CCMaintenanceUpdate.pandas_columns)
         df = df.set_index("dgst")
         df.index.name = "dgst"
 
-        df.maintenance_date = pd.to_datetime(df.maintenance_date, infer_datetime_format=True)
+        df.maintenance_date = pd.to_datetime(df.maintenance_date, infer_datetime_format=True, errors="coerce")
         return df.fillna(value=np.nan)
 
     @classmethod
     def from_web_latest(cls) -> CCDatasetMaintenanceUpdates:
         with tempfile.TemporaryDirectory() as tmp_dir:
             dset_path = Path(tmp_dir) / "cc_maintenances_latest_dataset.json"
             helpers.download_file(config.cc_maintenances_latest_snapshot, dset_path)
```

### Comparing `sec-certs-0.1.4/src/sec_certs/dataset/cc_scheme.py` & `sec-certs-0.1.5/src/sec_certs/dataset/cc_scheme.py`

 * *Files identical despite different names*

### Comparing `sec-certs-0.1.4/src/sec_certs/dataset/cpe.py` & `sec-certs-0.1.5/src/sec_certs/dataset/cpe.py`

 * *Files identical despite different names*

### Comparing `sec-certs-0.1.4/src/sec_certs/dataset/cve.py` & `sec-certs-0.1.5/src/sec_certs/dataset/cve.py`

 * *Files identical despite different names*

### Comparing `sec-certs-0.1.4/src/sec_certs/dataset/dataset.py` & `sec-certs-0.1.5/src/sec_certs/dataset/dataset.py`

 * *Files identical despite different names*

### Comparing `sec-certs-0.1.4/src/sec_certs/dataset/fips.py` & `sec-certs-0.1.5/src/sec_certs/dataset/fips.py`

 * *Files 1% similar despite different names*

```diff
@@ -325,16 +325,16 @@
                 cert.dgst, keep_unknowns
             )
 
     def to_pandas(self) -> pd.DataFrame:
         df = pd.DataFrame([x.pandas_tuple for x in self.certs.values()], columns=FIPSCertificate.pandas_columns)
         df = df.set_index("dgst")
 
-        df.date_validation = pd.to_datetime(df.date_validation, infer_datetime_format=True)
-        df.date_sunset = pd.to_datetime(df.date_sunset, infer_datetime_format=True)
+        df.date_validation = pd.to_datetime(df.date_validation, infer_datetime_format=True, errors="coerce")
+        df.date_sunset = pd.to_datetime(df.date_sunset, infer_datetime_format=True, errors="coerce")
 
         # Manually delete one certificate with bad embodiment (seems to have many blank fields)
         df = df.loc[~(df.embodiment == "*")]
 
         df = df.astype(
             {"type": "category", "status": "category", "standard": "category", "embodiment": "category"}
         ).fillna(value=np.nan)
```

### Comparing `sec-certs-0.1.4/src/sec_certs/dataset/fips_algorithm.py` & `sec-certs-0.1.5/src/sec_certs/dataset/fips_algorithm.py`

 * *Files identical despite different names*

### Comparing `sec-certs-0.1.4/src/sec_certs/dataset/fips_iut.py` & `sec-certs-0.1.5/src/sec_certs/dataset/fips_iut.py`

 * *Files identical despite different names*

### Comparing `sec-certs-0.1.4/src/sec_certs/dataset/fips_mip.py` & `sec-certs-0.1.5/src/sec_certs/dataset/fips_mip.py`

 * *Files identical despite different names*

### Comparing `sec-certs-0.1.4/src/sec_certs/dataset/json_path_dataset.py` & `sec-certs-0.1.5/src/sec_certs/dataset/json_path_dataset.py`

 * *Files identical despite different names*

### Comparing `sec-certs-0.1.4/src/sec_certs/dataset/protection_profile.py` & `sec-certs-0.1.5/src/sec_certs/dataset/protection_profile.py`

 * *Files identical despite different names*

### Comparing `sec-certs-0.1.4/src/sec_certs/model/__init__.py` & `sec-certs-0.1.5/src/sec_certs/model/__init__.py`

 * *Files identical despite different names*

### Comparing `sec-certs-0.1.4/src/sec_certs/model/cc_matching.py` & `sec-certs-0.1.5/src/sec_certs/model/cc_matching.py`

 * *Files identical despite different names*

### Comparing `sec-certs-0.1.4/src/sec_certs/model/cpe_matching.py` & `sec-certs-0.1.5/src/sec_certs/model/cpe_matching.py`

 * *Files identical despite different names*

### Comparing `sec-certs-0.1.4/src/sec_certs/model/evaluation.py` & `sec-certs-0.1.5/src/sec_certs/model/evaluation.py`

 * *Files identical despite different names*

### Comparing `sec-certs-0.1.4/src/sec_certs/model/fips_matching.py` & `sec-certs-0.1.5/src/sec_certs/model/fips_matching.py`

 * *Files identical despite different names*

### Comparing `sec-certs-0.1.4/src/sec_certs/model/matching.py` & `sec-certs-0.1.5/src/sec_certs/model/matching.py`

 * *Files identical despite different names*

### Comparing `sec-certs-0.1.4/src/sec_certs/model/reference_finder.py` & `sec-certs-0.1.5/src/sec_certs/model/reference_finder.py`

 * *Files identical despite different names*

### Comparing `sec-certs-0.1.4/src/sec_certs/model/sar_transformer.py` & `sec-certs-0.1.5/src/sec_certs/model/sar_transformer.py`

 * *Files identical despite different names*

### Comparing `sec-certs-0.1.4/src/sec_certs/model/transitive_vulnerability_finder.py` & `sec-certs-0.1.5/src/sec_certs/model/transitive_vulnerability_finder.py`

 * *Files identical despite different names*

### Comparing `sec-certs-0.1.4/src/sec_certs/rules.yaml` & `sec-certs-0.1.5/src/sec_certs/rules.yaml`

 * *Files identical despite different names*

### Comparing `sec-certs-0.1.4/src/sec_certs/sample/__init__.py` & `sec-certs-0.1.5/src/sec_certs/sample/__init__.py`

 * *Files identical despite different names*

### Comparing `sec-certs-0.1.4/src/sec_certs/sample/cc.py` & `sec-certs-0.1.5/src/sec_certs/sample/cc.py`

 * *Files identical despite different names*

### Comparing `sec-certs-0.1.4/src/sec_certs/sample/cc_certificate_id.py` & `sec-certs-0.1.5/src/sec_certs/sample/cc_certificate_id.py`

 * *Files identical despite different names*

### Comparing `sec-certs-0.1.4/src/sec_certs/sample/cc_maintenance_update.py` & `sec-certs-0.1.5/src/sec_certs/sample/cc_maintenance_update.py`

 * *Files identical despite different names*

### Comparing `sec-certs-0.1.4/src/sec_certs/sample/cc_scheme.py` & `sec-certs-0.1.5/src/sec_certs/sample/cc_scheme.py`

 * *Files identical despite different names*

### Comparing `sec-certs-0.1.4/src/sec_certs/sample/certificate.py` & `sec-certs-0.1.5/src/sec_certs/sample/certificate.py`

 * *Files identical despite different names*

### Comparing `sec-certs-0.1.4/src/sec_certs/sample/cpe.py` & `sec-certs-0.1.5/src/sec_certs/sample/cpe.py`

 * *Files identical despite different names*

### Comparing `sec-certs-0.1.4/src/sec_certs/sample/cve.py` & `sec-certs-0.1.5/src/sec_certs/sample/cve.py`

 * *Files identical despite different names*

### Comparing `sec-certs-0.1.4/src/sec_certs/sample/fips.py` & `sec-certs-0.1.5/src/sec_certs/sample/fips.py`

 * *Files identical despite different names*

### Comparing `sec-certs-0.1.4/src/sec_certs/sample/fips_algorithm.py` & `sec-certs-0.1.5/src/sec_certs/sample/fips_algorithm.py`

 * *Files identical despite different names*

### Comparing `sec-certs-0.1.4/src/sec_certs/sample/fips_iut.py` & `sec-certs-0.1.5/src/sec_certs/sample/fips_iut.py`

 * *Files identical despite different names*

### Comparing `sec-certs-0.1.4/src/sec_certs/sample/fips_mip.py` & `sec-certs-0.1.5/src/sec_certs/sample/fips_mip.py`

 * *Files identical despite different names*

### Comparing `sec-certs-0.1.4/src/sec_certs/sample/protection_profile.py` & `sec-certs-0.1.5/src/sec_certs/sample/protection_profile.py`

 * *Files identical despite different names*

### Comparing `sec-certs-0.1.4/src/sec_certs/sample/sar.py` & `sec-certs-0.1.5/src/sec_certs/sample/sar.py`

 * *Files identical despite different names*

### Comparing `sec-certs-0.1.4/src/sec_certs/serialization/json.py` & `sec-certs-0.1.5/src/sec_certs/serialization/json.py`

 * *Files identical despite different names*

### Comparing `sec-certs-0.1.4/src/sec_certs/utils/extract.py` & `sec-certs-0.1.5/src/sec_certs/utils/extract.py`

 * *Files identical despite different names*

### Comparing `sec-certs-0.1.4/src/sec_certs/utils/helpers.py` & `sec-certs-0.1.5/src/sec_certs/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `sec-certs-0.1.4/src/sec_certs/utils/nvd_dataset_builder.py` & `sec-certs-0.1.5/src/sec_certs/utils/nvd_dataset_builder.py`

 * *Files identical despite different names*

### Comparing `sec-certs-0.1.4/src/sec_certs/utils/pandas.py` & `sec-certs-0.1.5/src/sec_certs/utils/pandas.py`

 * *Files identical despite different names*

### Comparing `sec-certs-0.1.4/src/sec_certs/utils/parallel_processing.py` & `sec-certs-0.1.5/src/sec_certs/utils/parallel_processing.py`

 * *Files identical despite different names*

### Comparing `sec-certs-0.1.4/src/sec_certs/utils/pdf.py` & `sec-certs-0.1.5/src/sec_certs/utils/pdf.py`

 * *Files identical despite different names*

### Comparing `sec-certs-0.1.4/src/sec_certs/utils/sanitization.py` & `sec-certs-0.1.5/src/sec_certs/utils/sanitization.py`

 * *Files identical despite different names*

### Comparing `sec-certs-0.1.4/src/sec_certs/utils/strings.py` & `sec-certs-0.1.5/src/sec_certs/utils/strings.py`

 * *Files identical despite different names*

### Comparing `sec-certs-0.1.4/src/sec_certs/utils/tables.py` & `sec-certs-0.1.5/src/sec_certs/utils/tables.py`

 * *Files identical despite different names*

### Comparing `sec-certs-0.1.4/src/sec_certs.egg-info/PKG-INFO` & `sec-certs-0.1.5/src/sec_certs.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sec-certs
-Version: 0.1.4
+Version: 0.1.5
 Summary: A tool for data scraping and analysis of security certificates from Common Criteria and FIPS 140-2/3 frameworks
 Author: Jan Jancar, Petr Svenda, Jiri Michalik, Stanislav Bobon
 Author-email: Adam Janovsky <adamjanovsky@mail.muni.cz>
 License: MIT
 Project-URL: Homepage, https://seccerts.org
 Project-URL: GitHub, https://github.com/crocs-muni/sec-certs/
 Project-URL: Documentation, https://seccerts.org/docs
```

### Comparing `sec-certs-0.1.4/src/sec_certs.egg-info/SOURCES.txt` & `sec-certs-0.1.5/src/sec_certs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sec-certs-0.1.4/src/sec_certs.egg-info/requires.txt` & `sec-certs-0.1.5/src/sec_certs.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `sec-certs-0.1.4/tests/cc/conftest.py` & `sec-certs-0.1.5/tests/cc/conftest.py`

 * *Files identical despite different names*

### Comparing `sec-certs-0.1.4/tests/cc/test_cc_analysis.py` & `sec-certs-0.1.5/tests/cc/test_cc_analysis.py`

 * *Files identical despite different names*

### Comparing `sec-certs-0.1.4/tests/cc/test_cc_certificate.py` & `sec-certs-0.1.5/tests/cc/test_cc_certificate.py`

 * *Files identical despite different names*

### Comparing `sec-certs-0.1.4/tests/cc/test_cc_dataset.py` & `sec-certs-0.1.5/tests/cc/test_cc_dataset.py`

 * *Files identical despite different names*

### Comparing `sec-certs-0.1.4/tests/cc/test_cc_maintenance_updates.py` & `sec-certs-0.1.5/tests/cc/test_cc_maintenance_updates.py`

 * *Files identical despite different names*

### Comparing `sec-certs-0.1.4/tests/cc/test_cc_misc.py` & `sec-certs-0.1.5/tests/cc/test_cc_misc.py`

 * *Files identical despite different names*

### Comparing `sec-certs-0.1.4/tests/cc/test_cc_schemes.py` & `sec-certs-0.1.5/tests/cc/test_cc_schemes.py`

 * *Files identical despite different names*

### Comparing `sec-certs-0.1.4/tests/conftest.py` & `sec-certs-0.1.5/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `sec-certs-0.1.4/tests/data/cc/analysis/cc_full_dataset.json` & `sec-certs-0.1.5/tests/data/cc/analysis/cc_full_dataset.json`

 * *Files identical despite different names*

### Comparing `sec-certs-0.1.4/tests/data/cc/analysis/certs/reports/pdf/ebd276cca70fd723.pdf` & `sec-certs-0.1.5/tests/data/cc/analysis/certs/reports/pdf/ebd276cca70fd723.pdf`

 * *Files identical despite different names*

### Comparing `sec-certs-0.1.4/tests/data/cc/analysis/certs/reports/txt/ebd276cca70fd723.txt` & `sec-certs-0.1.5/tests/data/cc/analysis/certs/reports/txt/ebd276cca70fd723.txt`

 * *Files identical despite different names*

### Comparing `sec-certs-0.1.4/tests/data/cc/analysis/certs/targets/pdf/ebd276cca70fd723.pdf` & `sec-certs-0.1.5/tests/data/cc/analysis/certs/targets/pdf/ebd276cca70fd723.pdf`

 * *Files identical despite different names*

### Comparing `sec-certs-0.1.4/tests/data/cc/analysis/certs/targets/txt/ebd276cca70fd723.txt` & `sec-certs-0.1.5/tests/data/cc/analysis/certs/targets/txt/ebd276cca70fd723.txt`

 * *Files identical despite different names*

### Comparing `sec-certs-0.1.4/tests/data/cc/analysis/reference_dataset.json` & `sec-certs-0.1.5/tests/data/cc/analysis/reference_dataset.json`

 * *Files identical despite different names*

### Comparing `sec-certs-0.1.4/tests/data/cc/analysis/transitive_vulnerability_dataset.json` & `sec-certs-0.1.5/tests/data/cc/analysis/transitive_vulnerability_dataset.json`

 * *Files identical despite different names*

### Comparing `sec-certs-0.1.4/tests/data/cc/analysis/vulnerable_dataset.json` & `sec-certs-0.1.5/tests/data/cc/analysis/vulnerable_dataset.json`

 * *Files identical despite different names*

### Comparing `sec-certs-0.1.4/tests/data/cc/certificate/fictional_cert.json` & `sec-certs-0.1.5/tests/data/cc/certificate/fictional_cert.json`

 * *Files identical despite different names*

### Comparing `sec-certs-0.1.4/tests/data/cc/dataset/auxiliary_datasets/maintenances/maintenance_updates.json` & `sec-certs-0.1.5/tests/data/cc/dataset/auxiliary_datasets/maintenances/maintenance_updates.json`

 * *Files identical despite different names*

### Comparing `sec-certs-0.1.4/tests/data/cc/dataset/cc_products_active.csv` & `sec-certs-0.1.5/tests/data/cc/dataset/cc_products_active.csv`

 * *Files identical despite different names*

### Comparing `sec-certs-0.1.4/tests/data/cc/dataset/cc_products_active.html` & `sec-certs-0.1.5/tests/data/cc/dataset/cc_products_active.html`

 * *Files identical despite different names*

### Comparing `sec-certs-0.1.4/tests/data/cc/dataset/report_309ac2fd7f2dcf17.txt` & `sec-certs-0.1.5/tests/data/cc/dataset/report_309ac2fd7f2dcf17.txt`

 * *Files identical despite different names*

### Comparing `sec-certs-0.1.4/tests/data/cc/dataset/target_309ac2fd7f2dcf17.txt` & `sec-certs-0.1.5/tests/data/cc/dataset/target_309ac2fd7f2dcf17.txt`

 * *Files identical despite different names*

### Comparing `sec-certs-0.1.4/tests/data/cc/dataset/toy_dataset.json` & `sec-certs-0.1.5/tests/data/cc/dataset/toy_dataset.json`

 * *Files identical despite different names*

### Comparing `sec-certs-0.1.4/tests/data/common/cpe_dataset.json` & `sec-certs-0.1.5/tests/data/common/cpe_dataset.json`

 * *Files identical despite different names*

### Comparing `sec-certs-0.1.4/tests/data/common/cpe_match_feed.json` & `sec-certs-0.1.5/tests/data/common/cpe_match_feed.json`

 * *Files identical despite different names*

### Comparing `sec-certs-0.1.4/tests/data/common/cve_dataset.json` & `sec-certs-0.1.5/tests/data/common/cve_dataset.json`

 * *Files identical despite different names*

### Comparing `sec-certs-0.1.4/tests/data/fips/certificate/fictional_cert.json` & `sec-certs-0.1.5/tests/data/fips/certificate/fictional_cert.json`

 * *Files identical despite different names*

### Comparing `sec-certs-0.1.4/tests/data/fips/dataset/alg_dataset.json` & `sec-certs-0.1.5/tests/data/fips/dataset/alg_dataset.json`

 * *Files identical despite different names*

### Comparing `sec-certs-0.1.4/tests/data/fips/dataset/fips_modules_active.html` & `sec-certs-0.1.5/tests/data/fips/dataset/fips_modules_active.html`

 * *Files identical despite different names*

### Comparing `sec-certs-0.1.4/tests/data/fips/dataset/fips_modules_historical.html` & `sec-certs-0.1.5/tests/data/fips/dataset/fips_modules_historical.html`

 * *Files identical despite different names*

### Comparing `sec-certs-0.1.4/tests/data/fips/dataset/fips_modules_revoked.html` & `sec-certs-0.1.5/tests/data/fips/dataset/fips_modules_revoked.html`

 * *Files identical despite different names*

### Comparing `sec-certs-0.1.4/tests/data/fips/dataset/template_policy_184097a88a9b4ad9.txt` & `sec-certs-0.1.5/tests/data/fips/dataset/template_policy_184097a88a9b4ad9.txt`

 * *Files identical despite different names*

### Comparing `sec-certs-0.1.4/tests/data/fips/dataset/toy_dataset.json` & `sec-certs-0.1.5/tests/data/fips/dataset/toy_dataset.json`

 * *Files identical despite different names*

### Comparing `sec-certs-0.1.4/tests/data/fips/iut/fips_iut_2020-10-25T06+01:00.html` & `sec-certs-0.1.5/tests/data/fips/iut/fips_iut_2020-10-25T06+01:00.html`

 * *Files identical despite different names*

### Comparing `sec-certs-0.1.4/tests/data/fips/iut/fips_iut_2021-12-10T06+01:00.html` & `sec-certs-0.1.5/tests/data/fips/iut/fips_iut_2021-12-10T06+01:00.html`

 * *Files identical despite different names*

### Comparing `sec-certs-0.1.4/tests/data/fips/mip/fips_mip_2020-10-24T06+02:00.html` & `sec-certs-0.1.5/tests/data/fips/mip/fips_mip_2020-10-24T06+02:00.html`

 * *Files identical despite different names*

### Comparing `sec-certs-0.1.4/tests/data/fips/mip/fips_mip_2021-02-19T06+01:00.html` & `sec-certs-0.1.5/tests/data/fips/mip/fips_mip_2021-02-19T06+01:00.html`

 * *Files identical despite different names*

### Comparing `sec-certs-0.1.4/tests/data/fips/mip/fips_mip_2021-12-19T06+01:00.html` & `sec-certs-0.1.5/tests/data/fips/mip/fips_mip_2021-12-19T06+01:00.html`

 * *Files identical despite different names*

### Comparing `sec-certs-0.1.4/tests/fips/conftest.py` & `sec-certs-0.1.5/tests/fips/conftest.py`

 * *Files identical despite different names*

### Comparing `sec-certs-0.1.4/tests/fips/test_fips_algorithm_dataset.py` & `sec-certs-0.1.5/tests/fips/test_fips_algorithm_dataset.py`

 * *Files identical despite different names*

### Comparing `sec-certs-0.1.4/tests/fips/test_fips_analysis.py` & `sec-certs-0.1.5/tests/fips/test_fips_analysis.py`

 * *Files identical despite different names*

### Comparing `sec-certs-0.1.4/tests/fips/test_fips_certificate.py` & `sec-certs-0.1.5/tests/fips/test_fips_certificate.py`

 * *Files identical despite different names*

### Comparing `sec-certs-0.1.4/tests/fips/test_fips_dataset.py` & `sec-certs-0.1.5/tests/fips/test_fips_dataset.py`

 * *Files identical despite different names*

### Comparing `sec-certs-0.1.4/tests/fips/test_fips_iut.py` & `sec-certs-0.1.5/tests/fips/test_fips_iut.py`

 * *Files identical despite different names*

### Comparing `sec-certs-0.1.4/tests/fips/test_fips_mip.py` & `sec-certs-0.1.5/tests/fips/test_fips_mip.py`

 * *Files identical despite different names*

### Comparing `sec-certs-0.1.4/tests/test_config.py` & `sec-certs-0.1.5/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `sec-certs-0.1.4/tests/test_cpe.py` & `sec-certs-0.1.5/tests/test_cpe.py`

 * *Files identical despite different names*

### Comparing `sec-certs-0.1.4/tests/test_cve.py` & `sec-certs-0.1.5/tests/test_cve.py`

 * *Files identical despite different names*

### Comparing `sec-certs-0.1.4/tests/test_cve_matching.py` & `sec-certs-0.1.5/tests/test_cve_matching.py`

 * *Files identical despite different names*

### Comparing `sec-certs-0.1.4/tests/test_nvd_dataset_builder.py` & `sec-certs-0.1.5/tests/test_nvd_dataset_builder.py`

 * *Files identical despite different names*

