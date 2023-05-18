# Comparing `tmp/21cmFAST-3.1.5.tar.gz` & `tmp/21cmFAST-3.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/tmp/tmp33u5pumd/tmpdexlspet/21cmFAST-3.1.5.tar", last modified: Thu Apr 28 22:27:51 2022, max compression
+gzip compressed data, was "/tmp/tmpg7mi7u1k/tmppiyqs_l2/21cmFAST-3.2.0.tar", last modified: Wed Jul 13 18:38:47 2022, max compression
```

## Comparing `21cmFAST-3.1.5.tar` & `21cmFAST-3.2.0.tar`

### file list

```diff
@@ -1,208 +1,208 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-04-28 22:27:51.000000 21cmFAST-3.1.5/
--rw-r--r--   0 runner    (1001) docker     (116)       93 2022-04-28 22:27:31.000000 21cmFAST-3.1.5/.bumpversion.cfg
--rw-r--r--   0 runner    (1001) docker     (116)      749 2022-04-28 22:27:31.000000 21cmFAST-3.1.5/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-04-28 22:27:51.000000 21cmFAST-3.1.5/.github/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-04-28 22:27:51.000000 21cmFAST-3.1.5/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (116)      637 2022-04-28 22:27:31.000000 21cmFAST-3.1.5/.github/workflows/merge-me.yaml
--rw-r--r--   0 runner    (1001) docker     (116)      727 2022-04-28 22:27:31.000000 21cmFAST-3.1.5/.github/workflows/merge-to-dev.yaml
--rw-r--r--   0 runner    (1001) docker     (116)      241 2022-04-28 22:27:31.000000 21cmFAST-3.1.5/.github/workflows/pre_commit.yaml
--rw-r--r--   0 runner    (1001) docker     (116)     2123 2022-04-28 22:27:31.000000 21cmFAST-3.1.5/.github/workflows/publish-to-pypi.yaml
--rw-r--r--   0 runner    (1001) docker     (116)      365 2022-04-28 22:27:31.000000 21cmFAST-3.1.5/.github/workflows/tag-release.yaml
--rw-r--r--   0 runner    (1001) docker     (116)     3248 2022-04-28 22:27:31.000000 21cmFAST-3.1.5/.github/workflows/test_suite.yaml
--rw-r--r--   0 runner    (1001) docker     (116)      541 2022-04-28 22:27:31.000000 21cmFAST-3.1.5/.gitignore
--rw-r--r--   0 runner    (1001) docker     (116)      243 2022-04-28 22:27:31.000000 21cmFAST-3.1.5/.isort.cfg
--rw-r--r--   0 runner    (1001) docker     (116)     1602 2022-04-28 22:27:31.000000 21cmFAST-3.1.5/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (116)      380 2022-04-28 22:27:31.000000 21cmFAST-3.1.5/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (116)      577 2022-04-28 22:27:31.000000 21cmFAST-3.1.5/.travis.yml
--rw-r--r--   0 runner    (1001) docker     (116)      178 2022-04-28 22:27:31.000000 21cmFAST-3.1.5/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (116)    11660 2022-04-28 22:27:31.000000 21cmFAST-3.1.5/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (116)     4263 2022-04-28 22:27:31.000000 21cmFAST-3.1.5/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (116)     7705 2022-04-28 22:27:31.000000 21cmFAST-3.1.5/INSTALLATION.rst
--rw-r--r--   0 runner    (1001) docker     (116)     1080 2022-04-28 22:27:31.000000 21cmFAST-3.1.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (116)    20065 2022-04-28 22:27:51.000000 21cmFAST-3.1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     8189 2022-04-28 22:27:31.000000 21cmFAST-3.1.5/README.rst
--rw-r--r--   0 runner    (1001) docker     (116)        6 2022-04-28 22:27:31.000000 21cmFAST-3.1.5/VERSION
--rwxr-xr-x   0 runner    (1001) docker     (116)     2155 2022-04-28 22:27:31.000000 21cmFAST-3.1.5/build_cffi.py
--rwxr-xr-x   0 runner    (1001) docker     (116)      389 2022-04-28 22:27:31.000000 21cmFAST-3.1.5/bump
--rw-r--r--   0 runner    (1001) docker     (116)      590 2022-04-28 22:27:31.000000 21cmFAST-3.1.5/changethelog.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-04-28 22:27:51.000000 21cmFAST-3.1.5/ci/
--rw-r--r--   0 runner    (1001) docker     (116)      375 2022-04-28 22:27:31.000000 21cmFAST-3.1.5/ci/macos-latest-env.yml
--rw-r--r--   0 runner    (1001) docker     (116)      322 2022-04-28 22:27:31.000000 21cmFAST-3.1.5/ci/ubuntu-latest-env.yml
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-04-28 22:27:51.000000 21cmFAST-3.1.5/devel/
--rw-r--r--   0 runner    (1001) docker     (116)     1871 2022-04-28 22:27:31.000000 21cmFAST-3.1.5/devel/TestFindHalos.py
--rw-r--r--   0 runner    (1001) docker     (116)      949 2022-04-28 22:27:31.000000 21cmFAST-3.1.5/devel/filter_valgrind.py
--rw-r--r--   0 runner    (1001) docker     (116)     1505 2022-04-28 22:27:31.000000 21cmFAST-3.1.5/devel/prepare_gh_logs_for_diff.py
--rw-r--r--   0 runner    (1001) docker     (116)      851 2022-04-28 22:27:31.000000 21cmFAST-3.1.5/devel/prepare_log_for_diff.py
--rw-r--r--   0 runner    (1001) docker     (116)     1858 2022-04-28 22:27:31.000000 21cmFAST-3.1.5/devel/simulate_mcmc_memory_leak.py
--rw-r--r--   0 runner    (1001) docker     (116)     1725 2022-04-28 22:27:31.000000 21cmFAST-3.1.5/devel/simulate_mcmc_memory_leak_lightcone.py
--rw-r--r--   0 runner    (1001) docker     (116)     8186 2022-04-28 22:27:31.000000 21cmFAST-3.1.5/devel/valgrind-python.supp
--rw-r--r--   0 runner    (1001) docker     (116)     7183 2022-04-28 22:27:31.000000 21cmFAST-3.1.5/devel/valgrind-suppress-all-but-c.supp
--rw-r--r--   0 runner    (1001) docker     (116)   116373 2022-04-28 22:27:31.000000 21cmFAST-3.1.5/devel/visualise_boxes_and_power.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-04-28 22:27:51.000000 21cmFAST-3.1.5/docs/
--rw-r--r--   0 runner    (1001) docker     (116)     5586 2022-04-28 22:27:31.000000 21cmFAST-3.1.5/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (116)       28 2022-04-28 22:27:31.000000 21cmFAST-3.1.5/docs/authors.rst
--rw-r--r--   0 runner    (1001) docker     (116)       30 2022-04-28 22:27:31.000000 21cmFAST-3.1.5/docs/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (116)     2876 2022-04-28 22:27:31.000000 21cmFAST-3.1.5/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (116)       71 2022-04-28 22:27:31.000000 21cmFAST-3.1.5/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (116)     6913 2022-04-28 22:27:31.000000 21cmFAST-3.1.5/docs/design.rst
--rw-r--r--   0 runner    (1001) docker     (116)      292 2022-04-28 22:27:31.000000 21cmFAST-3.1.5/docs/environment.yaml
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-04-28 22:27:51.000000 21cmFAST-3.1.5/docs/faqs/
--rw-r--r--   0 runner    (1001) docker     (116)      249 2022-04-28 22:27:31.000000 21cmFAST-3.1.5/docs/faqs/installation_faq.rst
--rw-r--r--   0 runner    (1001) docker     (116)     2856 2022-04-28 22:27:31.000000 21cmFAST-3.1.5/docs/faqs/misc.rst
--rw-r--r--   0 runner    (1001) docker     (116)      263 2022-04-28 22:27:31.000000 21cmFAST-3.1.5/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (116)       33 2022-04-28 22:27:31.000000 21cmFAST-3.1.5/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (116)    22414 2022-04-28 22:27:31.000000 21cmFAST-3.1.5/docs/notes_for_developers.rst
--rw-r--r--   0 runner    (1001) docker     (116)       27 2022-04-28 22:27:31.000000 21cmFAST-3.1.5/docs/readme.rst
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-04-28 22:27:51.000000 21cmFAST-3.1.5/docs/reference/
--rw-r--r--   0 runner    (1001) docker     (116)       87 2022-04-28 22:27:31.000000 21cmFAST-3.1.5/docs/reference/index.rst
--rw-r--r--   0 runner    (1001) docker     (116)      259 2022-04-28 22:27:31.000000 21cmFAST-3.1.5/docs/reference/py21cmfast.rst
--rw-r--r--   0 runner    (1001) docker     (116)      109 2022-04-28 22:27:31.000000 21cmFAST-3.1.5/docs/spelling_wordlist.txt
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-04-28 22:27:51.000000 21cmFAST-3.1.5/docs/templates/
--rw-r--r--   0 runner    (1001) docker     (116)      564 2022-04-28 22:27:31.000000 21cmFAST-3.1.5/docs/templates/class.rst
--rw-r--r--   0 runner    (1001) docker     (116)      727 2022-04-28 22:27:31.000000 21cmFAST-3.1.5/docs/templates/module.rst
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-04-28 22:27:51.000000 21cmFAST-3.1.5/docs/tutorials/
--rw-r--r--   0 runner    (1001) docker     (116)   758159 2022-04-28 22:27:31.000000 21cmFAST-3.1.5/docs/tutorials/coeval_cubes.ipynb
--rw-r--r--   0 runner    (1001) docker     (116)   297781 2022-04-28 22:27:31.000000 21cmFAST-3.1.5/docs/tutorials/gather_data.ipynb
--rw-r--r--   0 runner    (1001) docker     (116)   223452 2022-04-28 22:27:31.000000 21cmFAST-3.1.5/docs/tutorials/lightcones.ipynb
--rw-r--r--   0 runner    (1001) docker     (116)  1977676 2022-04-28 22:27:31.000000 21cmFAST-3.1.5/docs/tutorials/mini-halos.ipynb
--rw-r--r--   0 runner    (1001) docker     (116)   108656 2022-04-28 22:27:31.000000 21cmFAST-3.1.5/docs/tutorials/relative_velocities.ipynb
--rw-r--r--   0 runner    (1001) docker     (116)      470 2022-04-28 22:27:31.000000 21cmFAST-3.1.5/docs/tutorials.rst
--rw-r--r--   0 runner    (1001) docker     (116)     1601 2022-04-28 22:27:31.000000 21cmFAST-3.1.5/environment_dev.yml
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-04-28 22:27:51.000000 21cmFAST-3.1.5/examples/
--rw-r--r--   0 runner    (1001) docker     (116)      478 2022-04-28 22:27:31.000000 21cmFAST-3.1.5/examples/runconfig_example.yml
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-04-28 22:27:51.000000 21cmFAST-3.1.5/joss-paper/
--rw-r--r--   0 runner    (1001) docker     (116)       52 2022-04-28 22:27:31.000000 21cmFAST-3.1.5/joss-paper/.gitignore
--rw-r--r--   0 runner    (1001) docker     (116)     2104 2022-04-28 22:27:31.000000 21cmFAST-3.1.5/joss-paper/Makefile
--rw-r--r--   0 runner    (1001) docker     (116)    15040 2022-04-28 22:27:31.000000 21cmFAST-3.1.5/joss-paper/apa.csl
--rw-r--r--   0 runner    (1001) docker     (116)    98285 2022-04-28 22:27:31.000000 21cmFAST-3.1.5/joss-paper/joss-logo.png
--rw-r--r--   0 runner    (1001) docker     (116)    10730 2022-04-28 22:27:31.000000 21cmFAST-3.1.5/joss-paper/latex.template
--rw-r--r--   0 runner    (1001) docker     (116)   437687 2022-04-28 22:27:31.000000 21cmFAST-3.1.5/joss-paper/lightcone.pdf
--rw-r--r--   0 runner    (1001) docker     (116)     1427 2022-04-28 22:27:31.000000 21cmFAST-3.1.5/joss-paper/make-example-plots.py
--rw-r--r--   0 runner    (1001) docker     (116)     9102 2022-04-28 22:27:31.000000 21cmFAST-3.1.5/joss-paper/paper.bib
--rw-r--r--   0 runner    (1001) docker     (116)    14600 2022-04-28 22:27:31.000000 21cmFAST-3.1.5/joss-paper/paper.md
--rw-r--r--   0 runner    (1001) docker     (116)    10181 2022-04-28 22:27:31.000000 21cmFAST-3.1.5/joss-paper/xH_history.pdf
--rw-r--r--   0 runner    (1001) docker     (116)  1033531 2022-04-28 22:27:31.000000 21cmFAST-3.1.5/joss-paper/yuxiangs-plot-small.png
--rw-r--r--   0 runner    (1001) docker     (116)      308 2022-04-28 22:27:31.000000 21cmFAST-3.1.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (116)      448 2022-04-28 22:27:51.000000 21cmFAST-3.1.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (116)     2952 2022-04-28 22:27:31.000000 21cmFAST-3.1.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-04-28 22:27:51.000000 21cmFAST-3.1.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-04-28 22:27:51.000000 21cmFAST-3.1.5/src/21cmFAST.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)    20065 2022-04-28 22:27:50.000000 21cmFAST-3.1.5/src/21cmFAST.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     6155 2022-04-28 22:27:51.000000 21cmFAST-3.1.5/src/21cmFAST.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2022-04-28 22:27:50.000000 21cmFAST-3.1.5/src/21cmFAST.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)       49 2022-04-28 22:27:51.000000 21cmFAST-3.1.5/src/21cmFAST.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2022-04-28 22:27:50.000000 21cmFAST-3.1.5/src/21cmFAST.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (116)      402 2022-04-28 22:27:51.000000 21cmFAST-3.1.5/src/21cmFAST.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)       11 2022-04-28 22:27:51.000000 21cmFAST-3.1.5/src/21cmFAST.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-04-28 22:27:51.000000 21cmFAST-3.1.5/src/py21cmfast/
--rw-r--r--   0 runner    (1001) docker     (116)     1414 2022-04-28 22:27:31.000000 21cmFAST-3.1.5/src/py21cmfast/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     3518 2022-04-28 22:27:31.000000 21cmFAST-3.1.5/src/py21cmfast/_cfg.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-04-28 22:27:51.000000 21cmFAST-3.1.5/src/py21cmfast/_data/
--rw-r--r--   0 runner    (1001) docker     (116)     5998 2022-04-28 22:27:31.000000 21cmFAST-3.1.5/src/py21cmfast/_data/Transfers_z0.dat
--rw-r--r--   0 runner    (1001) docker     (116)       60 2022-04-28 22:27:31.000000 21cmFAST-3.1.5/src/py21cmfast/_data/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (116)      385 2022-04-28 22:27:31.000000 21cmFAST-3.1.5/src/py21cmfast/_data/kappa_eH_table.dat
--rwxr-xr-x   0 runner    (1001) docker     (116)      284 2022-04-28 22:27:31.000000 21cmFAST-3.1.5/src/py21cmfast/_data/kappa_pH_table.dat
--rwxr-xr-x   0 runner    (1001) docker     (116)    23554 2022-04-28 22:27:31.000000 21cmFAST-3.1.5/src/py21cmfast/_data/recfast_LCDM.dat
--rwxr-xr-x   0 runner    (1001) docker     (116)     1162 2022-04-28 22:27:31.000000 21cmFAST-3.1.5/src/py21cmfast/_data/stellar_spectra.dat
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-04-28 22:27:51.000000 21cmFAST-3.1.5/src/py21cmfast/_data/x_int_tables/
--rwxr-xr-x   0 runner    (1001) docker     (116)    19811 2022-04-28 22:27:31.000000 21cmFAST-3.1.5/src/py21cmfast/_data/x_int_tables/log_xi_-1.0.dat
--rwxr-xr-x   0 runner    (1001) docker     (116)    19641 2022-04-28 22:27:31.000000 21cmFAST-3.1.5/src/py21cmfast/_data/x_int_tables/log_xi_-1.3.dat
--rwxr-xr-x   0 runner    (1001) docker     (116)    19444 2022-04-28 22:27:31.000000 21cmFAST-3.1.5/src/py21cmfast/_data/x_int_tables/log_xi_-1.6.dat
--rwxr-xr-x   0 runner    (1001) docker     (116)    19318 2022-04-28 22:27:31.000000 21cmFAST-3.1.5/src/py21cmfast/_data/x_int_tables/log_xi_-2.0.dat
--rwxr-xr-x   0 runner    (1001) docker     (116)    19181 2022-04-28 22:27:31.000000 21cmFAST-3.1.5/src/py21cmfast/_data/x_int_tables/log_xi_-2.3.dat
--rwxr-xr-x   0 runner    (1001) docker     (116)    19021 2022-04-28 22:27:31.000000 21cmFAST-3.1.5/src/py21cmfast/_data/x_int_tables/log_xi_-2.6.dat
--rwxr-xr-x   0 runner    (1001) docker     (116)    18794 2022-04-28 22:27:31.000000 21cmFAST-3.1.5/src/py21cmfast/_data/x_int_tables/log_xi_-3.0.dat
--rwxr-xr-x   0 runner    (1001) docker     (116)    18612 2022-04-28 22:27:31.000000 21cmFAST-3.1.5/src/py21cmfast/_data/x_int_tables/log_xi_-3.3.dat
--rwxr-xr-x   0 runner    (1001) docker     (116)    18522 2022-04-28 22:27:31.000000 21cmFAST-3.1.5/src/py21cmfast/_data/x_int_tables/log_xi_-3.6.dat
--rwxr-xr-x   0 runner    (1001) docker     (116)    18812 2022-04-28 22:27:31.000000 21cmFAST-3.1.5/src/py21cmfast/_data/x_int_tables/log_xi_-4.0.dat
--rwxr-xr-x   0 runner    (1001) docker     (116)    20412 2022-04-28 22:27:31.000000 21cmFAST-3.1.5/src/py21cmfast/_data/x_int_tables/xi_0.500.dat
--rwxr-xr-x   0 runner    (1001) docker     (116)    20860 2022-04-28 22:27:31.000000 21cmFAST-3.1.5/src/py21cmfast/_data/x_int_tables/xi_0.900.dat
--rwxr-xr-x   0 runner    (1001) docker     (116)    20267 2022-04-28 22:27:31.000000 21cmFAST-3.1.5/src/py21cmfast/_data/x_int_tables/xi_0.990.dat
--rwxr-xr-x   0 runner    (1001) docker     (116)    18893 2022-04-28 22:27:31.000000 21cmFAST-3.1.5/src/py21cmfast/_data/x_int_tables/xi_0.999.dat
--rw-r--r--   0 runner    (1001) docker     (116)     1129 2022-04-28 22:27:31.000000 21cmFAST-3.1.5/src/py21cmfast/_logging.py
--rw-r--r--   0 runner    (1001) docker     (116)    55406 2022-04-28 22:27:31.000000 21cmFAST-3.1.5/src/py21cmfast/_utils.py
--rw-r--r--   0 runner    (1001) docker     (116)      142 2022-04-28 22:27:50.000000 21cmFAST-3.1.5/src/py21cmfast/_version.py
--rw-r--r--   0 runner    (1001) docker     (116)     6481 2022-04-28 22:27:31.000000 21cmFAST-3.1.5/src/py21cmfast/cache_tools.py
--rw-r--r--   0 runner    (1001) docker     (116)    26037 2022-04-28 22:27:31.000000 21cmFAST-3.1.5/src/py21cmfast/cli.py
--rw-r--r--   0 runner    (1001) docker     (116)    41085 2022-04-28 22:27:31.000000 21cmFAST-3.1.5/src/py21cmfast/inputs.py
--rw-r--r--   0 runner    (1001) docker     (116)    41153 2022-04-28 22:27:31.000000 21cmFAST-3.1.5/src/py21cmfast/outputs.py
--rw-r--r--   0 runner    (1001) docker     (116)    13303 2022-04-28 22:27:31.000000 21cmFAST-3.1.5/src/py21cmfast/plotting.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-04-28 22:27:51.000000 21cmFAST-3.1.5/src/py21cmfast/src/
--rw-r--r--   0 runner    (1001) docker     (116)     7038 2022-04-28 22:27:31.000000 21cmFAST-3.1.5/src/py21cmfast/src/21cmFAST.h
--rw-r--r--   0 runner    (1001) docker     (116)    28816 2022-04-28 22:27:31.000000 21cmFAST-3.1.5/src/py21cmfast/src/BrightnessTemperatureBox.c
--rw-r--r--   0 runner    (1001) docker     (116)     9303 2022-04-28 22:27:31.000000 21cmFAST-3.1.5/src/py21cmfast/src/Constants.h
--rw-r--r--   0 runner    (1001) docker     (116)    20041 2022-04-28 22:27:31.000000 21cmFAST-3.1.5/src/py21cmfast/src/FindHaloes.c
--rw-r--r--   0 runner    (1001) docker     (116)    39450 2022-04-28 22:27:31.000000 21cmFAST-3.1.5/src/py21cmfast/src/GenerateICs.c
--rw-r--r--   0 runner    (1001) docker     (116)     3484 2022-04-28 22:27:31.000000 21cmFAST-3.1.5/src/py21cmfast/src/Globals.h
--rw-r--r--   0 runner    (1001) docker     (116)   101598 2022-04-28 22:27:31.000000 21cmFAST-3.1.5/src/py21cmfast/src/IonisationBox.c
--rw-r--r--   0 runner    (1001) docker     (116)    28873 2022-04-28 22:27:31.000000 21cmFAST-3.1.5/src/py21cmfast/src/PerturbField.c
--rw-r--r--   0 runner    (1001) docker     (116)    12055 2022-04-28 22:27:31.000000 21cmFAST-3.1.5/src/py21cmfast/src/PerturbHaloField.c
--rw-r--r--   0 runner    (1001) docker     (116)   134934 2022-04-28 22:27:31.000000 21cmFAST-3.1.5/src/py21cmfast/src/SpinTemperatureBox.c
--rw-r--r--   0 runner    (1001) docker     (116)    34128 2022-04-28 22:27:31.000000 21cmFAST-3.1.5/src/py21cmfast/src/UsefulFunctions.c
--rwxr-xr-x   0 runner    (1001) docker     (116)    13110 2022-04-28 22:27:31.000000 21cmFAST-3.1.5/src/py21cmfast/src/bubble_helper_progs.c
--rw-r--r--   0 runner    (1001) docker     (116)    10244 2022-04-28 22:27:31.000000 21cmFAST-3.1.5/src/py21cmfast/src/cexcept.h
--rw-r--r--   0 runner    (1001) docker     (116)     4949 2022-04-28 22:27:31.000000 21cmFAST-3.1.5/src/py21cmfast/src/dft.c
--rwxr-xr-x   0 runner    (1001) docker     (116)    16857 2022-04-28 22:27:31.000000 21cmFAST-3.1.5/src/py21cmfast/src/elec_interp.c
--rw-r--r--   0 runner    (1001) docker     (116)      571 2022-04-28 22:27:31.000000 21cmFAST-3.1.5/src/py21cmfast/src/exceptions.h
--rwxr-xr-x   0 runner    (1001) docker     (116)    48021 2022-04-28 22:27:31.000000 21cmFAST-3.1.5/src/py21cmfast/src/heating_helper_progs.c
--rw-r--r--   0 runner    (1001) docker     (116)     3531 2022-04-28 22:27:31.000000 21cmFAST-3.1.5/src/py21cmfast/src/indexing.c
--rw-r--r--   0 runner    (1001) docker     (116)     4036 2022-04-28 22:27:31.000000 21cmFAST-3.1.5/src/py21cmfast/src/logger.h
--rw-r--r--   0 runner    (1001) docker     (116)   169875 2022-04-28 22:27:31.000000 21cmFAST-3.1.5/src/py21cmfast/src/ps.c
--rwxr-xr-x   0 runner    (1001) docker     (116)    11214 2022-04-28 22:27:31.000000 21cmFAST-3.1.5/src/py21cmfast/src/recombinations.c
--rw-r--r--   0 runner    (1001) docker     (116)   119277 2022-04-28 22:27:31.000000 21cmFAST-3.1.5/src/py21cmfast/wrapper.py
--rw-r--r--   0 runner    (1001) docker     (116)     1444 2022-04-28 22:27:31.000000 21cmFAST-3.1.5/src/py21cmfast/yaml.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-04-28 22:27:51.000000 21cmFAST-3.1.5/tests/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2022-04-28 22:27:31.000000 21cmFAST-3.1.5/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     3691 2022-04-28 22:27:31.000000 21cmFAST-3.1.5/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-04-28 22:27:51.000000 21cmFAST-3.1.5/tests/plots/
--rw-r--r--   0 runner    (1001) docker     (116)    35933 2022-04-28 22:27:31.000000 21cmFAST-3.1.5/tests/plots/tests.test_integration_features.py--test_power_spectra_coeval[18-kwargs12].pdf
--rw-r--r--   0 runner    (1001) docker     (116)    19739 2022-04-28 22:27:31.000000 21cmFAST-3.1.5/tests/produce_integration_test_data.py
--rw-r--r--   0 runner    (1001) docker     (116)     1222 2022-04-28 22:27:31.000000 21cmFAST-3.1.5/tests/test_cache_tools.py
--rw-r--r--   0 runner    (1001) docker     (116)     4243 2022-04-28 22:27:31.000000 21cmFAST-3.1.5/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (116)     1279 2022-04-28 22:27:31.000000 21cmFAST-3.1.5/tests/test_config.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-04-28 22:27:51.000000 21cmFAST-3.1.5/tests/test_data/
--rw-r--r--   0 runner    (1001) docker     (116)     6160 2022-04-28 22:27:31.000000 21cmFAST-3.1.5/tests/test_data/halo_field_data_halo_field.h5
--rw-r--r--   0 runner    (1001) docker     (116)     8496 2022-04-28 22:27:31.000000 21cmFAST-3.1.5/tests/test_data/perturb_field_data_highres.h5
--rw-r--r--   0 runner    (1001) docker     (116)     8496 2022-04-28 22:27:31.000000 21cmFAST-3.1.5/tests/test_data/perturb_field_data_linear.h5
--rw-r--r--   0 runner    (1001) docker     (116)     8496 2022-04-28 22:27:31.000000 21cmFAST-3.1.5/tests/test_data/perturb_field_data_no2lpt.h5
--rw-r--r--   0 runner    (1001) docker     (116)     8496 2022-04-28 22:27:31.000000 21cmFAST-3.1.5/tests/test_data/perturb_field_data_simple.h5
--rw-r--r--   0 runner    (1001) docker     (116)    18976 2022-04-28 22:27:31.000000 21cmFAST-3.1.5/tests/test_data/power_spectra_change_step_factor.h5
--rw-r--r--   0 runner    (1001) docker     (116)    18960 2022-04-28 22:27:31.000000 21cmFAST-3.1.5/tests/test_data/power_spectra_change_z_heat_max.h5
--rw-r--r--   0 runner    (1001) docker     (116)    19160 2022-04-28 22:27:31.000000 21cmFAST-3.1.5/tests/test_data/power_spectra_fast_fcoll_hiz.h5
--rw-r--r--   0 runner    (1001) docker     (116)    21296 2022-04-28 22:27:31.000000 21cmFAST-3.1.5/tests/test_data/power_spectra_fast_fcoll_lowz.h5
--rw-r--r--   0 runner    (1001) docker     (116)    18984 2022-04-28 22:27:31.000000 21cmFAST-3.1.5/tests/test_data/power_spectra_fftw_wisdom.h5
--rw-r--r--   0 runner    (1001) docker     (116)    21120 2022-04-28 22:27:31.000000 21cmFAST-3.1.5/tests/test_data/power_spectra_halo_field.h5
--rw-r--r--   0 runner    (1001) docker     (116)    27200 2022-04-28 22:27:31.000000 21cmFAST-3.1.5/tests/test_data/power_spectra_halo_field_mdz.h5
--rw-r--r--   0 runner    (1001) docker     (116)    21608 2022-04-28 22:27:31.000000 21cmFAST-3.1.5/tests/test_data/power_spectra_halo_field_mdz_highres.h5
--rw-r--r--   0 runner    (1001) docker     (116)    21928 2022-04-28 22:27:31.000000 21cmFAST-3.1.5/tests/test_data/power_spectra_inhomo.h5
--rw-r--r--   0 runner    (1001) docker     (116)    18992 2022-04-28 22:27:31.000000 21cmFAST-3.1.5/tests/test_data/power_spectra_interp_perturb_field.h5
--rw-r--r--   0 runner    (1001) docker     (116)    19096 2022-04-28 22:27:31.000000 21cmFAST-3.1.5/tests/test_data/power_spectra_larger_step_factor.h5
--rw-r--r--   0 runner    (1001) docker     (116)    21360 2022-04-28 22:27:31.000000 21cmFAST-3.1.5/tests/test_data/power_spectra_mdz_and_photoncons.h5
--rw-r--r--   0 runner    (1001) docker     (116)    27176 2022-04-28 22:27:31.000000 21cmFAST-3.1.5/tests/test_data/power_spectra_mdz_and_ts_fluct.h5
--rw-r--r--   0 runner    (1001) docker     (116)    27440 2022-04-28 22:27:31.000000 21cmFAST-3.1.5/tests/test_data/power_spectra_mdz_and_tsfluct_nthreads.h5
--rw-r--r--   0 runner    (1001) docker     (116)    27280 2022-04-28 22:27:31.000000 21cmFAST-3.1.5/tests/test_data/power_spectra_mdz_tsfluct_nthreads.h5
--rw-r--r--   0 runner    (1001) docker     (116)    18992 2022-04-28 22:27:31.000000 21cmFAST-3.1.5/tests/test_data/power_spectra_mdzeta.h5
--rw-r--r--   0 runner    (1001) docker     (116)    26552 2022-04-28 22:27:31.000000 21cmFAST-3.1.5/tests/test_data/power_spectra_mini_halos.h5
--rw-r--r--   0 runner    (1001) docker     (116)    27272 2022-04-28 22:27:31.000000 21cmFAST-3.1.5/tests/test_data/power_spectra_minihalos_no_tables.h5
--rw-r--r--   0 runner    (1001) docker     (116)    27264 2022-04-28 22:27:31.000000 21cmFAST-3.1.5/tests/test_data/power_spectra_minimize_mem.h5
--rw-r--r--   0 runner    (1001) docker     (116)    19104 2022-04-28 22:27:31.000000 21cmFAST-3.1.5/tests/test_data/power_spectra_mmin_in_mass.h5
--rw-r--r--   0 runner    (1001) docker     (116)    21096 2022-04-28 22:27:31.000000 21cmFAST-3.1.5/tests/test_data/power_spectra_nthreads.h5
--rw-r--r--   0 runner    (1001) docker     (116)    18992 2022-04-28 22:27:31.000000 21cmFAST-3.1.5/tests/test_data/power_spectra_perturb_high_res.h5
--rw-r--r--   0 runner    (1001) docker     (116)    21032 2022-04-28 22:27:31.000000 21cmFAST-3.1.5/tests/test_data/power_spectra_photoncons.h5
--rw-r--r--   0 runner    (1001) docker     (116)    23024 2022-04-28 22:27:31.000000 21cmFAST-3.1.5/tests/test_data/power_spectra_relvel.h5
--rw-r--r--   0 runner    (1001) docker     (116)    21120 2022-04-28 22:27:31.000000 21cmFAST-3.1.5/tests/test_data/power_spectra_rsd.h5
--rw-r--r--   0 runner    (1001) docker     (116)    14776 2022-04-28 22:27:31.000000 21cmFAST-3.1.5/tests/test_data/power_spectra_simple.h5
--rw-r--r--   0 runner    (1001) docker     (116)    27088 2022-04-28 22:27:31.000000 21cmFAST-3.1.5/tests/test_data/power_spectra_ts_fluct_no_tables.h5
--rw-r--r--   0 runner    (1001) docker     (116)    26752 2022-04-28 22:27:31.000000 21cmFAST-3.1.5/tests/test_data/power_spectra_tsfluct.h5
--rw-r--r--   0 runner    (1001) docker     (116)     9536 2022-04-28 22:27:31.000000 21cmFAST-3.1.5/tests/test_data/power_spectra_z9.00_INHOMO_RECO=True_MINIMIZE_MEMORY=True_PHOTON_CONS=True_USE_MASS_DEPENDENT_ZETA=True_USE_TS_FLUCT=True_z_heat_max=25_zprime_step_factor=1.1.h5
--rw-r--r--   0 runner    (1001) docker     (116)      458 2022-04-28 22:27:31.000000 21cmFAST-3.1.5/tests/test_data_exists.py
--rw-r--r--   0 runner    (1001) docker     (116)      615 2022-04-28 22:27:31.000000 21cmFAST-3.1.5/tests/test_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (116)     3370 2022-04-28 22:27:31.000000 21cmFAST-3.1.5/tests/test_high_level_io.py
--rw-r--r--   0 runner    (1001) docker     (116)     2818 2022-04-28 22:27:31.000000 21cmFAST-3.1.5/tests/test_initial_conditions.py
--rw-r--r--   0 runner    (1001) docker     (116)     3942 2022-04-28 22:27:31.000000 21cmFAST-3.1.5/tests/test_input_structs.py
--rw-r--r--   0 runner    (1001) docker     (116)     7949 2022-04-28 22:27:31.000000 21cmFAST-3.1.5/tests/test_integration_features.py
--rw-r--r--   0 runner    (1001) docker     (116)     4620 2022-04-28 22:27:31.000000 21cmFAST-3.1.5/tests/test_output_structs.py
--rw-r--r--   0 runner    (1001) docker     (116)     2364 2022-04-28 22:27:31.000000 21cmFAST-3.1.5/tests/test_plotting.py
--rw-r--r--   0 runner    (1001) docker     (116)      660 2022-04-28 22:27:31.000000 21cmFAST-3.1.5/tests/test_spin_temp.py
--rw-r--r--   0 runner    (1001) docker     (116)      108 2022-04-28 22:27:31.000000 21cmFAST-3.1.5/tests/test_tables.py
--rw-r--r--   0 runner    (1001) docker     (116)    14623 2022-04-28 22:27:31.000000 21cmFAST-3.1.5/tests/test_wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-07-13 18:38:47.000000 21cmFAST-3.2.0/
+-rw-r--r--   0 runner    (1001) docker     (116)       93 2022-07-13 18:38:26.000000 21cmFAST-3.2.0/.bumpversion.cfg
+-rw-r--r--   0 runner    (1001) docker     (116)      749 2022-07-13 18:38:26.000000 21cmFAST-3.2.0/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-07-13 18:38:47.000000 21cmFAST-3.2.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-07-13 18:38:47.000000 21cmFAST-3.2.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (116)      637 2022-07-13 18:38:26.000000 21cmFAST-3.2.0/.github/workflows/merge-me.yaml
+-rw-r--r--   0 runner    (1001) docker     (116)      727 2022-07-13 18:38:26.000000 21cmFAST-3.2.0/.github/workflows/merge-to-dev.yaml
+-rw-r--r--   0 runner    (1001) docker     (116)      241 2022-07-13 18:38:26.000000 21cmFAST-3.2.0/.github/workflows/pre_commit.yaml
+-rw-r--r--   0 runner    (1001) docker     (116)     2123 2022-07-13 18:38:26.000000 21cmFAST-3.2.0/.github/workflows/publish-to-pypi.yaml
+-rw-r--r--   0 runner    (1001) docker     (116)      365 2022-07-13 18:38:26.000000 21cmFAST-3.2.0/.github/workflows/tag-release.yaml
+-rw-r--r--   0 runner    (1001) docker     (116)     3248 2022-07-13 18:38:26.000000 21cmFAST-3.2.0/.github/workflows/test_suite.yaml
+-rw-r--r--   0 runner    (1001) docker     (116)      541 2022-07-13 18:38:26.000000 21cmFAST-3.2.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (116)      243 2022-07-13 18:38:26.000000 21cmFAST-3.2.0/.isort.cfg
+-rw-r--r--   0 runner    (1001) docker     (116)     1602 2022-07-13 18:38:26.000000 21cmFAST-3.2.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (116)      380 2022-07-13 18:38:26.000000 21cmFAST-3.2.0/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (116)      577 2022-07-13 18:38:26.000000 21cmFAST-3.2.0/.travis.yml
+-rw-r--r--   0 runner    (1001) docker     (116)      178 2022-07-13 18:38:26.000000 21cmFAST-3.2.0/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (116)    12465 2022-07-13 18:38:26.000000 21cmFAST-3.2.0/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (116)     4263 2022-07-13 18:38:26.000000 21cmFAST-3.2.0/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (116)     7705 2022-07-13 18:38:26.000000 21cmFAST-3.2.0/INSTALLATION.rst
+-rw-r--r--   0 runner    (1001) docker     (116)     1080 2022-07-13 18:38:26.000000 21cmFAST-3.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (116)    20850 2022-07-13 18:38:47.000000 21cmFAST-3.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (116)     8189 2022-07-13 18:38:26.000000 21cmFAST-3.2.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (116)        6 2022-07-13 18:38:26.000000 21cmFAST-3.2.0/VERSION
+-rwxr-xr-x   0 runner    (1001) docker     (116)     2155 2022-07-13 18:38:26.000000 21cmFAST-3.2.0/build_cffi.py
+-rwxr-xr-x   0 runner    (1001) docker     (116)      389 2022-07-13 18:38:26.000000 21cmFAST-3.2.0/bump
+-rw-r--r--   0 runner    (1001) docker     (116)      590 2022-07-13 18:38:26.000000 21cmFAST-3.2.0/changethelog.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-07-13 18:38:47.000000 21cmFAST-3.2.0/ci/
+-rw-r--r--   0 runner    (1001) docker     (116)      375 2022-07-13 18:38:26.000000 21cmFAST-3.2.0/ci/macos-latest-env.yml
+-rw-r--r--   0 runner    (1001) docker     (116)      322 2022-07-13 18:38:26.000000 21cmFAST-3.2.0/ci/ubuntu-latest-env.yml
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-07-13 18:38:47.000000 21cmFAST-3.2.0/devel/
+-rw-r--r--   0 runner    (1001) docker     (116)     1871 2022-07-13 18:38:26.000000 21cmFAST-3.2.0/devel/TestFindHalos.py
+-rw-r--r--   0 runner    (1001) docker     (116)      949 2022-07-13 18:38:26.000000 21cmFAST-3.2.0/devel/filter_valgrind.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1505 2022-07-13 18:38:26.000000 21cmFAST-3.2.0/devel/prepare_gh_logs_for_diff.py
+-rw-r--r--   0 runner    (1001) docker     (116)      851 2022-07-13 18:38:26.000000 21cmFAST-3.2.0/devel/prepare_log_for_diff.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1858 2022-07-13 18:38:26.000000 21cmFAST-3.2.0/devel/simulate_mcmc_memory_leak.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1725 2022-07-13 18:38:26.000000 21cmFAST-3.2.0/devel/simulate_mcmc_memory_leak_lightcone.py
+-rw-r--r--   0 runner    (1001) docker     (116)     8186 2022-07-13 18:38:26.000000 21cmFAST-3.2.0/devel/valgrind-python.supp
+-rw-r--r--   0 runner    (1001) docker     (116)     7183 2022-07-13 18:38:26.000000 21cmFAST-3.2.0/devel/valgrind-suppress-all-but-c.supp
+-rw-r--r--   0 runner    (1001) docker     (116)   116373 2022-07-13 18:38:26.000000 21cmFAST-3.2.0/devel/visualise_boxes_and_power.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-07-13 18:38:47.000000 21cmFAST-3.2.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (116)     5586 2022-07-13 18:38:26.000000 21cmFAST-3.2.0/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (116)       28 2022-07-13 18:38:26.000000 21cmFAST-3.2.0/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (116)       30 2022-07-13 18:38:26.000000 21cmFAST-3.2.0/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (116)     2876 2022-07-13 18:38:26.000000 21cmFAST-3.2.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (116)       71 2022-07-13 18:38:26.000000 21cmFAST-3.2.0/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (116)     6913 2022-07-13 18:38:26.000000 21cmFAST-3.2.0/docs/design.rst
+-rw-r--r--   0 runner    (1001) docker     (116)      292 2022-07-13 18:38:26.000000 21cmFAST-3.2.0/docs/environment.yaml
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-07-13 18:38:47.000000 21cmFAST-3.2.0/docs/faqs/
+-rw-r--r--   0 runner    (1001) docker     (116)      249 2022-07-13 18:38:26.000000 21cmFAST-3.2.0/docs/faqs/installation_faq.rst
+-rw-r--r--   0 runner    (1001) docker     (116)     2856 2022-07-13 18:38:26.000000 21cmFAST-3.2.0/docs/faqs/misc.rst
+-rw-r--r--   0 runner    (1001) docker     (116)      263 2022-07-13 18:38:26.000000 21cmFAST-3.2.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (116)       33 2022-07-13 18:38:26.000000 21cmFAST-3.2.0/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (116)    22414 2022-07-13 18:38:26.000000 21cmFAST-3.2.0/docs/notes_for_developers.rst
+-rw-r--r--   0 runner    (1001) docker     (116)       27 2022-07-13 18:38:26.000000 21cmFAST-3.2.0/docs/readme.rst
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-07-13 18:38:47.000000 21cmFAST-3.2.0/docs/reference/
+-rw-r--r--   0 runner    (1001) docker     (116)       87 2022-07-13 18:38:26.000000 21cmFAST-3.2.0/docs/reference/index.rst
+-rw-r--r--   0 runner    (1001) docker     (116)      259 2022-07-13 18:38:26.000000 21cmFAST-3.2.0/docs/reference/py21cmfast.rst
+-rw-r--r--   0 runner    (1001) docker     (116)      109 2022-07-13 18:38:26.000000 21cmFAST-3.2.0/docs/spelling_wordlist.txt
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-07-13 18:38:47.000000 21cmFAST-3.2.0/docs/templates/
+-rw-r--r--   0 runner    (1001) docker     (116)      564 2022-07-13 18:38:26.000000 21cmFAST-3.2.0/docs/templates/class.rst
+-rw-r--r--   0 runner    (1001) docker     (116)      727 2022-07-13 18:38:26.000000 21cmFAST-3.2.0/docs/templates/module.rst
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-07-13 18:38:47.000000 21cmFAST-3.2.0/docs/tutorials/
+-rw-r--r--   0 runner    (1001) docker     (116)   758159 2022-07-13 18:38:26.000000 21cmFAST-3.2.0/docs/tutorials/coeval_cubes.ipynb
+-rw-r--r--   0 runner    (1001) docker     (116)   297781 2022-07-13 18:38:26.000000 21cmFAST-3.2.0/docs/tutorials/gather_data.ipynb
+-rw-r--r--   0 runner    (1001) docker     (116)   223452 2022-07-13 18:38:26.000000 21cmFAST-3.2.0/docs/tutorials/lightcones.ipynb
+-rw-r--r--   0 runner    (1001) docker     (116)  1977676 2022-07-13 18:38:26.000000 21cmFAST-3.2.0/docs/tutorials/mini-halos.ipynb
+-rw-r--r--   0 runner    (1001) docker     (116)   108656 2022-07-13 18:38:26.000000 21cmFAST-3.2.0/docs/tutorials/relative_velocities.ipynb
+-rw-r--r--   0 runner    (1001) docker     (116)      470 2022-07-13 18:38:26.000000 21cmFAST-3.2.0/docs/tutorials.rst
+-rw-r--r--   0 runner    (1001) docker     (116)     1601 2022-07-13 18:38:26.000000 21cmFAST-3.2.0/environment_dev.yml
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-07-13 18:38:47.000000 21cmFAST-3.2.0/examples/
+-rw-r--r--   0 runner    (1001) docker     (116)      478 2022-07-13 18:38:26.000000 21cmFAST-3.2.0/examples/runconfig_example.yml
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-07-13 18:38:47.000000 21cmFAST-3.2.0/joss-paper/
+-rw-r--r--   0 runner    (1001) docker     (116)       52 2022-07-13 18:38:26.000000 21cmFAST-3.2.0/joss-paper/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (116)     2104 2022-07-13 18:38:26.000000 21cmFAST-3.2.0/joss-paper/Makefile
+-rw-r--r--   0 runner    (1001) docker     (116)    15040 2022-07-13 18:38:26.000000 21cmFAST-3.2.0/joss-paper/apa.csl
+-rw-r--r--   0 runner    (1001) docker     (116)    98285 2022-07-13 18:38:26.000000 21cmFAST-3.2.0/joss-paper/joss-logo.png
+-rw-r--r--   0 runner    (1001) docker     (116)    10730 2022-07-13 18:38:26.000000 21cmFAST-3.2.0/joss-paper/latex.template
+-rw-r--r--   0 runner    (1001) docker     (116)   437687 2022-07-13 18:38:26.000000 21cmFAST-3.2.0/joss-paper/lightcone.pdf
+-rw-r--r--   0 runner    (1001) docker     (116)     1427 2022-07-13 18:38:26.000000 21cmFAST-3.2.0/joss-paper/make-example-plots.py
+-rw-r--r--   0 runner    (1001) docker     (116)     9102 2022-07-13 18:38:26.000000 21cmFAST-3.2.0/joss-paper/paper.bib
+-rw-r--r--   0 runner    (1001) docker     (116)    14600 2022-07-13 18:38:26.000000 21cmFAST-3.2.0/joss-paper/paper.md
+-rw-r--r--   0 runner    (1001) docker     (116)    10181 2022-07-13 18:38:26.000000 21cmFAST-3.2.0/joss-paper/xH_history.pdf
+-rw-r--r--   0 runner    (1001) docker     (116)  1033531 2022-07-13 18:38:26.000000 21cmFAST-3.2.0/joss-paper/yuxiangs-plot-small.png
+-rw-r--r--   0 runner    (1001) docker     (116)      308 2022-07-13 18:38:26.000000 21cmFAST-3.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (116)      448 2022-07-13 18:38:47.000000 21cmFAST-3.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (116)     3053 2022-07-13 18:38:26.000000 21cmFAST-3.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-07-13 18:38:47.000000 21cmFAST-3.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-07-13 18:38:47.000000 21cmFAST-3.2.0/src/21cmFAST.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (116)    20850 2022-07-13 18:38:47.000000 21cmFAST-3.2.0/src/21cmFAST.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (116)     6155 2022-07-13 18:38:47.000000 21cmFAST-3.2.0/src/21cmFAST.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (116)        1 2022-07-13 18:38:47.000000 21cmFAST-3.2.0/src/21cmFAST.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (116)       49 2022-07-13 18:38:47.000000 21cmFAST-3.2.0/src/21cmFAST.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (116)        1 2022-07-13 18:38:47.000000 21cmFAST-3.2.0/src/21cmFAST.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (116)      402 2022-07-13 18:38:47.000000 21cmFAST-3.2.0/src/21cmFAST.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (116)       11 2022-07-13 18:38:47.000000 21cmFAST-3.2.0/src/21cmFAST.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-07-13 18:38:47.000000 21cmFAST-3.2.0/src/py21cmfast/
+-rw-r--r--   0 runner    (1001) docker     (116)     1414 2022-07-13 18:38:26.000000 21cmFAST-3.2.0/src/py21cmfast/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3655 2022-07-13 18:38:26.000000 21cmFAST-3.2.0/src/py21cmfast/_cfg.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-07-13 18:38:47.000000 21cmFAST-3.2.0/src/py21cmfast/_data/
+-rw-r--r--   0 runner    (1001) docker     (116)     5998 2022-07-13 18:38:26.000000 21cmFAST-3.2.0/src/py21cmfast/_data/Transfers_z0.dat
+-rw-r--r--   0 runner    (1001) docker     (116)       60 2022-07-13 18:38:26.000000 21cmFAST-3.2.0/src/py21cmfast/_data/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (116)      385 2022-07-13 18:38:26.000000 21cmFAST-3.2.0/src/py21cmfast/_data/kappa_eH_table.dat
+-rwxr-xr-x   0 runner    (1001) docker     (116)      284 2022-07-13 18:38:26.000000 21cmFAST-3.2.0/src/py21cmfast/_data/kappa_pH_table.dat
+-rwxr-xr-x   0 runner    (1001) docker     (116)    23554 2022-07-13 18:38:26.000000 21cmFAST-3.2.0/src/py21cmfast/_data/recfast_LCDM.dat
+-rwxr-xr-x   0 runner    (1001) docker     (116)     1162 2022-07-13 18:38:26.000000 21cmFAST-3.2.0/src/py21cmfast/_data/stellar_spectra.dat
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-07-13 18:38:47.000000 21cmFAST-3.2.0/src/py21cmfast/_data/x_int_tables/
+-rwxr-xr-x   0 runner    (1001) docker     (116)    19811 2022-07-13 18:38:26.000000 21cmFAST-3.2.0/src/py21cmfast/_data/x_int_tables/log_xi_-1.0.dat
+-rwxr-xr-x   0 runner    (1001) docker     (116)    19641 2022-07-13 18:38:26.000000 21cmFAST-3.2.0/src/py21cmfast/_data/x_int_tables/log_xi_-1.3.dat
+-rwxr-xr-x   0 runner    (1001) docker     (116)    19444 2022-07-13 18:38:26.000000 21cmFAST-3.2.0/src/py21cmfast/_data/x_int_tables/log_xi_-1.6.dat
+-rwxr-xr-x   0 runner    (1001) docker     (116)    19318 2022-07-13 18:38:26.000000 21cmFAST-3.2.0/src/py21cmfast/_data/x_int_tables/log_xi_-2.0.dat
+-rwxr-xr-x   0 runner    (1001) docker     (116)    19181 2022-07-13 18:38:26.000000 21cmFAST-3.2.0/src/py21cmfast/_data/x_int_tables/log_xi_-2.3.dat
+-rwxr-xr-x   0 runner    (1001) docker     (116)    19021 2022-07-13 18:38:26.000000 21cmFAST-3.2.0/src/py21cmfast/_data/x_int_tables/log_xi_-2.6.dat
+-rwxr-xr-x   0 runner    (1001) docker     (116)    18794 2022-07-13 18:38:26.000000 21cmFAST-3.2.0/src/py21cmfast/_data/x_int_tables/log_xi_-3.0.dat
+-rwxr-xr-x   0 runner    (1001) docker     (116)    18612 2022-07-13 18:38:26.000000 21cmFAST-3.2.0/src/py21cmfast/_data/x_int_tables/log_xi_-3.3.dat
+-rwxr-xr-x   0 runner    (1001) docker     (116)    18522 2022-07-13 18:38:26.000000 21cmFAST-3.2.0/src/py21cmfast/_data/x_int_tables/log_xi_-3.6.dat
+-rwxr-xr-x   0 runner    (1001) docker     (116)    18812 2022-07-13 18:38:26.000000 21cmFAST-3.2.0/src/py21cmfast/_data/x_int_tables/log_xi_-4.0.dat
+-rwxr-xr-x   0 runner    (1001) docker     (116)    20412 2022-07-13 18:38:26.000000 21cmFAST-3.2.0/src/py21cmfast/_data/x_int_tables/xi_0.500.dat
+-rwxr-xr-x   0 runner    (1001) docker     (116)    20860 2022-07-13 18:38:26.000000 21cmFAST-3.2.0/src/py21cmfast/_data/x_int_tables/xi_0.900.dat
+-rwxr-xr-x   0 runner    (1001) docker     (116)    20267 2022-07-13 18:38:26.000000 21cmFAST-3.2.0/src/py21cmfast/_data/x_int_tables/xi_0.990.dat
+-rwxr-xr-x   0 runner    (1001) docker     (116)    18893 2022-07-13 18:38:26.000000 21cmFAST-3.2.0/src/py21cmfast/_data/x_int_tables/xi_0.999.dat
+-rw-r--r--   0 runner    (1001) docker     (116)     1129 2022-07-13 18:38:26.000000 21cmFAST-3.2.0/src/py21cmfast/_logging.py
+-rw-r--r--   0 runner    (1001) docker     (116)    56285 2022-07-13 18:38:26.000000 21cmFAST-3.2.0/src/py21cmfast/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (116)      176 2022-07-13 18:38:47.000000 21cmFAST-3.2.0/src/py21cmfast/_version.py
+-rw-r--r--   0 runner    (1001) docker     (116)     6481 2022-07-13 18:38:26.000000 21cmFAST-3.2.0/src/py21cmfast/cache_tools.py
+-rw-r--r--   0 runner    (1001) docker     (116)    26037 2022-07-13 18:38:26.000000 21cmFAST-3.2.0/src/py21cmfast/cli.py
+-rw-r--r--   0 runner    (1001) docker     (116)    41085 2022-07-13 18:38:26.000000 21cmFAST-3.2.0/src/py21cmfast/inputs.py
+-rw-r--r--   0 runner    (1001) docker     (116)    41153 2022-07-13 18:38:26.000000 21cmFAST-3.2.0/src/py21cmfast/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (116)    13303 2022-07-13 18:38:26.000000 21cmFAST-3.2.0/src/py21cmfast/plotting.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-07-13 18:38:47.000000 21cmFAST-3.2.0/src/py21cmfast/src/
+-rw-r--r--   0 runner    (1001) docker     (116)     7038 2022-07-13 18:38:26.000000 21cmFAST-3.2.0/src/py21cmfast/src/21cmFAST.h
+-rw-r--r--   0 runner    (1001) docker     (116)    28816 2022-07-13 18:38:26.000000 21cmFAST-3.2.0/src/py21cmfast/src/BrightnessTemperatureBox.c
+-rw-r--r--   0 runner    (1001) docker     (116)     9303 2022-07-13 18:38:26.000000 21cmFAST-3.2.0/src/py21cmfast/src/Constants.h
+-rw-r--r--   0 runner    (1001) docker     (116)    20041 2022-07-13 18:38:26.000000 21cmFAST-3.2.0/src/py21cmfast/src/FindHaloes.c
+-rw-r--r--   0 runner    (1001) docker     (116)    39450 2022-07-13 18:38:26.000000 21cmFAST-3.2.0/src/py21cmfast/src/GenerateICs.c
+-rw-r--r--   0 runner    (1001) docker     (116)     3484 2022-07-13 18:38:26.000000 21cmFAST-3.2.0/src/py21cmfast/src/Globals.h
+-rw-r--r--   0 runner    (1001) docker     (116)   101598 2022-07-13 18:38:26.000000 21cmFAST-3.2.0/src/py21cmfast/src/IonisationBox.c
+-rw-r--r--   0 runner    (1001) docker     (116)    28873 2022-07-13 18:38:26.000000 21cmFAST-3.2.0/src/py21cmfast/src/PerturbField.c
+-rw-r--r--   0 runner    (1001) docker     (116)    12055 2022-07-13 18:38:26.000000 21cmFAST-3.2.0/src/py21cmfast/src/PerturbHaloField.c
+-rw-r--r--   0 runner    (1001) docker     (116)   134934 2022-07-13 18:38:26.000000 21cmFAST-3.2.0/src/py21cmfast/src/SpinTemperatureBox.c
+-rw-r--r--   0 runner    (1001) docker     (116)    34128 2022-07-13 18:38:26.000000 21cmFAST-3.2.0/src/py21cmfast/src/UsefulFunctions.c
+-rwxr-xr-x   0 runner    (1001) docker     (116)    13110 2022-07-13 18:38:26.000000 21cmFAST-3.2.0/src/py21cmfast/src/bubble_helper_progs.c
+-rw-r--r--   0 runner    (1001) docker     (116)    10244 2022-07-13 18:38:26.000000 21cmFAST-3.2.0/src/py21cmfast/src/cexcept.h
+-rw-r--r--   0 runner    (1001) docker     (116)     4949 2022-07-13 18:38:26.000000 21cmFAST-3.2.0/src/py21cmfast/src/dft.c
+-rwxr-xr-x   0 runner    (1001) docker     (116)    16857 2022-07-13 18:38:26.000000 21cmFAST-3.2.0/src/py21cmfast/src/elec_interp.c
+-rw-r--r--   0 runner    (1001) docker     (116)      571 2022-07-13 18:38:26.000000 21cmFAST-3.2.0/src/py21cmfast/src/exceptions.h
+-rwxr-xr-x   0 runner    (1001) docker     (116)    48021 2022-07-13 18:38:26.000000 21cmFAST-3.2.0/src/py21cmfast/src/heating_helper_progs.c
+-rw-r--r--   0 runner    (1001) docker     (116)     3531 2022-07-13 18:38:26.000000 21cmFAST-3.2.0/src/py21cmfast/src/indexing.c
+-rw-r--r--   0 runner    (1001) docker     (116)     4036 2022-07-13 18:38:26.000000 21cmFAST-3.2.0/src/py21cmfast/src/logger.h
+-rw-r--r--   0 runner    (1001) docker     (116)   169875 2022-07-13 18:38:26.000000 21cmFAST-3.2.0/src/py21cmfast/src/ps.c
+-rwxr-xr-x   0 runner    (1001) docker     (116)    11214 2022-07-13 18:38:26.000000 21cmFAST-3.2.0/src/py21cmfast/src/recombinations.c
+-rw-r--r--   0 runner    (1001) docker     (116)   119355 2022-07-13 18:38:26.000000 21cmFAST-3.2.0/src/py21cmfast/wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1444 2022-07-13 18:38:26.000000 21cmFAST-3.2.0/src/py21cmfast/yaml.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-07-13 18:38:47.000000 21cmFAST-3.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (116)        0 2022-07-13 18:38:26.000000 21cmFAST-3.2.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3691 2022-07-13 18:38:26.000000 21cmFAST-3.2.0/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-07-13 18:38:47.000000 21cmFAST-3.2.0/tests/plots/
+-rw-r--r--   0 runner    (1001) docker     (116)    35933 2022-07-13 18:38:26.000000 21cmFAST-3.2.0/tests/plots/tests.test_integration_features.py--test_power_spectra_coeval[18-kwargs12].pdf
+-rw-r--r--   0 runner    (1001) docker     (116)    19739 2022-07-13 18:38:26.000000 21cmFAST-3.2.0/tests/produce_integration_test_data.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1222 2022-07-13 18:38:26.000000 21cmFAST-3.2.0/tests/test_cache_tools.py
+-rw-r--r--   0 runner    (1001) docker     (116)     4243 2022-07-13 18:38:26.000000 21cmFAST-3.2.0/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1279 2022-07-13 18:38:26.000000 21cmFAST-3.2.0/tests/test_config.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-07-13 18:38:47.000000 21cmFAST-3.2.0/tests/test_data/
+-rw-r--r--   0 runner    (1001) docker     (116)     6160 2022-07-13 18:38:26.000000 21cmFAST-3.2.0/tests/test_data/halo_field_data_halo_field.h5
+-rw-r--r--   0 runner    (1001) docker     (116)     8496 2022-07-13 18:38:26.000000 21cmFAST-3.2.0/tests/test_data/perturb_field_data_highres.h5
+-rw-r--r--   0 runner    (1001) docker     (116)     8496 2022-07-13 18:38:26.000000 21cmFAST-3.2.0/tests/test_data/perturb_field_data_linear.h5
+-rw-r--r--   0 runner    (1001) docker     (116)     8496 2022-07-13 18:38:26.000000 21cmFAST-3.2.0/tests/test_data/perturb_field_data_no2lpt.h5
+-rw-r--r--   0 runner    (1001) docker     (116)     8496 2022-07-13 18:38:26.000000 21cmFAST-3.2.0/tests/test_data/perturb_field_data_simple.h5
+-rw-r--r--   0 runner    (1001) docker     (116)    18976 2022-07-13 18:38:26.000000 21cmFAST-3.2.0/tests/test_data/power_spectra_change_step_factor.h5
+-rw-r--r--   0 runner    (1001) docker     (116)    18960 2022-07-13 18:38:26.000000 21cmFAST-3.2.0/tests/test_data/power_spectra_change_z_heat_max.h5
+-rw-r--r--   0 runner    (1001) docker     (116)    19160 2022-07-13 18:38:26.000000 21cmFAST-3.2.0/tests/test_data/power_spectra_fast_fcoll_hiz.h5
+-rw-r--r--   0 runner    (1001) docker     (116)    21296 2022-07-13 18:38:26.000000 21cmFAST-3.2.0/tests/test_data/power_spectra_fast_fcoll_lowz.h5
+-rw-r--r--   0 runner    (1001) docker     (116)    18984 2022-07-13 18:38:26.000000 21cmFAST-3.2.0/tests/test_data/power_spectra_fftw_wisdom.h5
+-rw-r--r--   0 runner    (1001) docker     (116)    21120 2022-07-13 18:38:26.000000 21cmFAST-3.2.0/tests/test_data/power_spectra_halo_field.h5
+-rw-r--r--   0 runner    (1001) docker     (116)    27200 2022-07-13 18:38:26.000000 21cmFAST-3.2.0/tests/test_data/power_spectra_halo_field_mdz.h5
+-rw-r--r--   0 runner    (1001) docker     (116)    21608 2022-07-13 18:38:26.000000 21cmFAST-3.2.0/tests/test_data/power_spectra_halo_field_mdz_highres.h5
+-rw-r--r--   0 runner    (1001) docker     (116)    21928 2022-07-13 18:38:26.000000 21cmFAST-3.2.0/tests/test_data/power_spectra_inhomo.h5
+-rw-r--r--   0 runner    (1001) docker     (116)    18992 2022-07-13 18:38:26.000000 21cmFAST-3.2.0/tests/test_data/power_spectra_interp_perturb_field.h5
+-rw-r--r--   0 runner    (1001) docker     (116)    19096 2022-07-13 18:38:26.000000 21cmFAST-3.2.0/tests/test_data/power_spectra_larger_step_factor.h5
+-rw-r--r--   0 runner    (1001) docker     (116)    21360 2022-07-13 18:38:26.000000 21cmFAST-3.2.0/tests/test_data/power_spectra_mdz_and_photoncons.h5
+-rw-r--r--   0 runner    (1001) docker     (116)    27176 2022-07-13 18:38:26.000000 21cmFAST-3.2.0/tests/test_data/power_spectra_mdz_and_ts_fluct.h5
+-rw-r--r--   0 runner    (1001) docker     (116)    27440 2022-07-13 18:38:26.000000 21cmFAST-3.2.0/tests/test_data/power_spectra_mdz_and_tsfluct_nthreads.h5
+-rw-r--r--   0 runner    (1001) docker     (116)    27280 2022-07-13 18:38:26.000000 21cmFAST-3.2.0/tests/test_data/power_spectra_mdz_tsfluct_nthreads.h5
+-rw-r--r--   0 runner    (1001) docker     (116)    18992 2022-07-13 18:38:26.000000 21cmFAST-3.2.0/tests/test_data/power_spectra_mdzeta.h5
+-rw-r--r--   0 runner    (1001) docker     (116)    26552 2022-07-13 18:38:26.000000 21cmFAST-3.2.0/tests/test_data/power_spectra_mini_halos.h5
+-rw-r--r--   0 runner    (1001) docker     (116)    27272 2022-07-13 18:38:26.000000 21cmFAST-3.2.0/tests/test_data/power_spectra_minihalos_no_tables.h5
+-rw-r--r--   0 runner    (1001) docker     (116)    27264 2022-07-13 18:38:26.000000 21cmFAST-3.2.0/tests/test_data/power_spectra_minimize_mem.h5
+-rw-r--r--   0 runner    (1001) docker     (116)    19104 2022-07-13 18:38:26.000000 21cmFAST-3.2.0/tests/test_data/power_spectra_mmin_in_mass.h5
+-rw-r--r--   0 runner    (1001) docker     (116)    21096 2022-07-13 18:38:26.000000 21cmFAST-3.2.0/tests/test_data/power_spectra_nthreads.h5
+-rw-r--r--   0 runner    (1001) docker     (116)    18992 2022-07-13 18:38:26.000000 21cmFAST-3.2.0/tests/test_data/power_spectra_perturb_high_res.h5
+-rw-r--r--   0 runner    (1001) docker     (116)    21032 2022-07-13 18:38:26.000000 21cmFAST-3.2.0/tests/test_data/power_spectra_photoncons.h5
+-rw-r--r--   0 runner    (1001) docker     (116)    23024 2022-07-13 18:38:26.000000 21cmFAST-3.2.0/tests/test_data/power_spectra_relvel.h5
+-rw-r--r--   0 runner    (1001) docker     (116)    21120 2022-07-13 18:38:26.000000 21cmFAST-3.2.0/tests/test_data/power_spectra_rsd.h5
+-rw-r--r--   0 runner    (1001) docker     (116)    14776 2022-07-13 18:38:26.000000 21cmFAST-3.2.0/tests/test_data/power_spectra_simple.h5
+-rw-r--r--   0 runner    (1001) docker     (116)    27088 2022-07-13 18:38:26.000000 21cmFAST-3.2.0/tests/test_data/power_spectra_ts_fluct_no_tables.h5
+-rw-r--r--   0 runner    (1001) docker     (116)    26752 2022-07-13 18:38:26.000000 21cmFAST-3.2.0/tests/test_data/power_spectra_tsfluct.h5
+-rw-r--r--   0 runner    (1001) docker     (116)     9536 2022-07-13 18:38:26.000000 21cmFAST-3.2.0/tests/test_data/power_spectra_z9.00_INHOMO_RECO=True_MINIMIZE_MEMORY=True_PHOTON_CONS=True_USE_MASS_DEPENDENT_ZETA=True_USE_TS_FLUCT=True_z_heat_max=25_zprime_step_factor=1.1.h5
+-rw-r--r--   0 runner    (1001) docker     (116)      458 2022-07-13 18:38:26.000000 21cmFAST-3.2.0/tests/test_data_exists.py
+-rw-r--r--   0 runner    (1001) docker     (116)      615 2022-07-13 18:38:26.000000 21cmFAST-3.2.0/tests/test_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3370 2022-07-13 18:38:26.000000 21cmFAST-3.2.0/tests/test_high_level_io.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2818 2022-07-13 18:38:26.000000 21cmFAST-3.2.0/tests/test_initial_conditions.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3942 2022-07-13 18:38:26.000000 21cmFAST-3.2.0/tests/test_input_structs.py
+-rw-r--r--   0 runner    (1001) docker     (116)     7949 2022-07-13 18:38:26.000000 21cmFAST-3.2.0/tests/test_integration_features.py
+-rw-r--r--   0 runner    (1001) docker     (116)     4620 2022-07-13 18:38:26.000000 21cmFAST-3.2.0/tests/test_output_structs.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2364 2022-07-13 18:38:26.000000 21cmFAST-3.2.0/tests/test_plotting.py
+-rw-r--r--   0 runner    (1001) docker     (116)      660 2022-07-13 18:38:26.000000 21cmFAST-3.2.0/tests/test_spin_temp.py
+-rw-r--r--   0 runner    (1001) docker     (116)      108 2022-07-13 18:38:26.000000 21cmFAST-3.2.0/tests/test_tables.py
+-rw-r--r--   0 runner    (1001) docker     (116)    14623 2022-07-13 18:38:26.000000 21cmFAST-3.2.0/tests/test_wrapper.py
```

### Comparing `21cmFAST-3.1.5/.flake8` & `21cmFAST-3.2.0/.flake8`

 * *Files identical despite different names*

### Comparing `21cmFAST-3.1.5/.github/workflows/merge-me.yaml` & `21cmFAST-3.2.0/.github/workflows/merge-me.yaml`

 * *Files identical despite different names*

### Comparing `21cmFAST-3.1.5/.github/workflows/merge-to-dev.yaml` & `21cmFAST-3.2.0/.github/workflows/merge-to-dev.yaml`

 * *Files identical despite different names*

### Comparing `21cmFAST-3.1.5/.github/workflows/publish-to-pypi.yaml` & `21cmFAST-3.2.0/.github/workflows/publish-to-pypi.yaml`

 * *Files identical despite different names*

### Comparing `21cmFAST-3.1.5/.github/workflows/test_suite.yaml` & `21cmFAST-3.2.0/.github/workflows/test_suite.yaml`

 * *Files identical despite different names*

### Comparing `21cmFAST-3.1.5/.gitignore` & `21cmFAST-3.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `21cmFAST-3.1.5/.pre-commit-config.yaml` & `21cmFAST-3.2.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `21cmFAST-3.1.5/.travis.yml` & `21cmFAST-3.2.0/.travis.yml`

 * *Files identical despite different names*

### Comparing `21cmFAST-3.1.5/CHANGELOG.rst` & `21cmFAST-3.2.0/CHANGELOG.rst`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,42 @@
 Changelog
 =========
 
 dev-version
 -----------
 
+v3.2.0 [11 Jul 2022]
+----------------------
+
+Changed
+~~~~~~~
+
+* Floats are now represented to a specific number of significant digits in the hash of
+  an output object. This fixes problems with very close redshifts not being read from
+  cache (#80). Note that this means that very close astro/cosmo params will now be read
+  from cache. This could cause issues when creating large databases with many random
+  parameters. The behaviour can modified in the configuration by setting the
+  ``cache_param_sigfigs`` and ``cache_redshift_sigfigs`` parameters (these are 6 and
+  4 by default, respectively).
+  **NOTE**: updating to this version will cause your previous cached files to become
+  unusable. Remove them before updating.
+
+Fixed
+~~~~~
+
+* Added a missing C-based error to the known errors in Python.
+
 v3.1.5 [27 Apr 2022]
 ----------------------
 
 v3.1.4 [10 Feb 2022]
 ----------------------
 
 Fixed
------
+~~~~~
 
 * error in FFT normalization in FindHaloes
 * docs not compiling on RTD due to missing ``scipy.integrate`` mock module
 * Updated matplotlib removed support for setting vmin/vmax and norm. Now passes vmin/vmax
   to the norm() constructor.
 
 v3.1.3 [27 Oct 2021]
```

### Comparing `21cmFAST-3.1.5/CONTRIBUTING.rst` & `21cmFAST-3.2.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `21cmFAST-3.1.5/INSTALLATION.rst` & `21cmFAST-3.2.0/INSTALLATION.rst`

 * *Files identical despite different names*

### Comparing `21cmFAST-3.1.5/LICENSE` & `21cmFAST-3.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `21cmFAST-3.1.5/PKG-INFO` & `21cmFAST-3.2.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: 21cmFAST
-Version: 3.1.5
+Version: 3.2.0
 Summary: A semi-numerical cosmological simulation code for the 21cm signal
 Home-page: https://github.com/21cmFAST/21cmFAST
 Author: The 21cmFAST coredev team
 Author-email: 21cmfast.coredev@gmail.com
 License: MIT license
 Keywords: Epoch of Reionization,Cosmology
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Unix
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
@@ -193,22 +192,43 @@
 
 Changelog
 =========
 
 dev-version
 -----------
 
+v3.2.0 [11 Jul 2022]
+----------------------
+
+Changed
+~~~~~~~
+
+* Floats are now represented to a specific number of significant digits in the hash of
+  an output object. This fixes problems with very close redshifts not being read from
+  cache (#80). Note that this means that very close astro/cosmo params will now be read
+  from cache. This could cause issues when creating large databases with many random
+  parameters. The behaviour can modified in the configuration by setting the
+  ``cache_param_sigfigs`` and ``cache_redshift_sigfigs`` parameters (these are 6 and
+  4 by default, respectively).
+  **NOTE**: updating to this version will cause your previous cached files to become
+  unusable. Remove them before updating.
+
+Fixed
+~~~~~
+
+* Added a missing C-based error to the known errors in Python.
+
 v3.1.5 [27 Apr 2022]
 ----------------------
 
 v3.1.4 [10 Feb 2022]
 ----------------------
 
 Fixed
------
+~~~~~
 
 * error in FFT normalization in FindHaloes
 * docs not compiling on RTD due to missing ``scipy.integrate`` mock module
 * Updated matplotlib removed support for setting vmin/vmax and norm. Now passes vmin/vmax
   to the norm() constructor.
 
 v3.1.3 [27 Oct 2021]
@@ -446,9 +466,7 @@
   conditions and prints out an ASCII file with the associated power spectrum.
 - Parameter in Ts.c for the maximum allowed kinetic temperature, which increases
   stability of the code when the redshift step size and the X-ray efficiencies are large.
 
 Fixed
 ~~~~~
 - Oversight adding support for a Gaussian filter for the lower resolution field.
-
-
```

### Comparing `21cmFAST-3.1.5/README.rst` & `21cmFAST-3.2.0/README.rst`

 * *Files identical despite different names*

### Comparing `21cmFAST-3.1.5/build_cffi.py` & `21cmFAST-3.2.0/build_cffi.py`

 * *Files identical despite different names*

### Comparing `21cmFAST-3.1.5/changethelog.py` & `21cmFAST-3.2.0/changethelog.py`

 * *Files identical despite different names*

### Comparing `21cmFAST-3.1.5/devel/TestFindHalos.py` & `21cmFAST-3.2.0/devel/TestFindHalos.py`

 * *Files identical despite different names*

### Comparing `21cmFAST-3.1.5/devel/filter_valgrind.py` & `21cmFAST-3.2.0/devel/filter_valgrind.py`

 * *Files identical despite different names*

### Comparing `21cmFAST-3.1.5/devel/prepare_gh_logs_for_diff.py` & `21cmFAST-3.2.0/devel/prepare_gh_logs_for_diff.py`

 * *Files identical despite different names*

### Comparing `21cmFAST-3.1.5/devel/prepare_log_for_diff.py` & `21cmFAST-3.2.0/devel/prepare_log_for_diff.py`

 * *Files identical despite different names*

### Comparing `21cmFAST-3.1.5/devel/simulate_mcmc_memory_leak.py` & `21cmFAST-3.2.0/devel/simulate_mcmc_memory_leak.py`

 * *Files identical despite different names*

### Comparing `21cmFAST-3.1.5/devel/simulate_mcmc_memory_leak_lightcone.py` & `21cmFAST-3.2.0/devel/simulate_mcmc_memory_leak_lightcone.py`

 * *Files identical despite different names*

### Comparing `21cmFAST-3.1.5/devel/valgrind-python.supp` & `21cmFAST-3.2.0/devel/valgrind-python.supp`

 * *Files identical despite different names*

### Comparing `21cmFAST-3.1.5/devel/valgrind-suppress-all-but-c.supp` & `21cmFAST-3.2.0/devel/valgrind-suppress-all-but-c.supp`

 * *Files identical despite different names*

### Comparing `21cmFAST-3.1.5/devel/visualise_boxes_and_power.ipynb` & `21cmFAST-3.2.0/devel/visualise_boxes_and_power.ipynb`

 * *Files identical despite different names*

### Comparing `21cmFAST-3.1.5/docs/Makefile` & `21cmFAST-3.2.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `21cmFAST-3.1.5/docs/conf.py` & `21cmFAST-3.2.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `21cmFAST-3.1.5/docs/design.rst` & `21cmFAST-3.2.0/docs/design.rst`

 * *Files identical despite different names*

### Comparing `21cmFAST-3.1.5/docs/faqs/misc.rst` & `21cmFAST-3.2.0/docs/faqs/misc.rst`

 * *Files identical despite different names*

### Comparing `21cmFAST-3.1.5/docs/notes_for_developers.rst` & `21cmFAST-3.2.0/docs/notes_for_developers.rst`

 * *Files identical despite different names*

### Comparing `21cmFAST-3.1.5/docs/templates/class.rst` & `21cmFAST-3.2.0/docs/templates/class.rst`

 * *Files identical despite different names*

### Comparing `21cmFAST-3.1.5/docs/templates/module.rst` & `21cmFAST-3.2.0/docs/templates/module.rst`

 * *Files identical despite different names*

### Comparing `21cmFAST-3.1.5/docs/tutorials/coeval_cubes.ipynb` & `21cmFAST-3.2.0/docs/tutorials/coeval_cubes.ipynb`

 * *Files identical despite different names*

### Comparing `21cmFAST-3.1.5/docs/tutorials/gather_data.ipynb` & `21cmFAST-3.2.0/docs/tutorials/gather_data.ipynb`

 * *Files identical despite different names*

### Comparing `21cmFAST-3.1.5/docs/tutorials/lightcones.ipynb` & `21cmFAST-3.2.0/docs/tutorials/lightcones.ipynb`

 * *Files identical despite different names*

### Comparing `21cmFAST-3.1.5/docs/tutorials/mini-halos.ipynb` & `21cmFAST-3.2.0/docs/tutorials/mini-halos.ipynb`

 * *Files identical despite different names*

### Comparing `21cmFAST-3.1.5/docs/tutorials/relative_velocities.ipynb` & `21cmFAST-3.2.0/docs/tutorials/relative_velocities.ipynb`

 * *Files identical despite different names*

### Comparing `21cmFAST-3.1.5/environment_dev.yml` & `21cmFAST-3.2.0/environment_dev.yml`

 * *Files identical despite different names*

### Comparing `21cmFAST-3.1.5/joss-paper/Makefile` & `21cmFAST-3.2.0/joss-paper/Makefile`

 * *Files identical despite different names*

### Comparing `21cmFAST-3.1.5/joss-paper/apa.csl` & `21cmFAST-3.2.0/joss-paper/apa.csl`

 * *Files identical despite different names*

### Comparing `21cmFAST-3.1.5/joss-paper/joss-logo.png` & `21cmFAST-3.2.0/joss-paper/joss-logo.png`

 * *Files identical despite different names*

### Comparing `21cmFAST-3.1.5/joss-paper/latex.template` & `21cmFAST-3.2.0/joss-paper/latex.template`

 * *Files identical despite different names*

### Comparing `21cmFAST-3.1.5/joss-paper/lightcone.pdf` & `21cmFAST-3.2.0/joss-paper/lightcone.pdf`

 * *Files identical despite different names*

### Comparing `21cmFAST-3.1.5/joss-paper/make-example-plots.py` & `21cmFAST-3.2.0/joss-paper/make-example-plots.py`

 * *Files identical despite different names*

### Comparing `21cmFAST-3.1.5/joss-paper/paper.bib` & `21cmFAST-3.2.0/joss-paper/paper.bib`

 * *Files identical despite different names*

### Comparing `21cmFAST-3.1.5/joss-paper/paper.md` & `21cmFAST-3.2.0/joss-paper/paper.md`

 * *Files identical despite different names*

### Comparing `21cmFAST-3.1.5/joss-paper/xH_history.pdf` & `21cmFAST-3.2.0/joss-paper/xH_history.pdf`

 * *Files identical despite different names*

### Comparing `21cmFAST-3.1.5/joss-paper/yuxiangs-plot-small.png` & `21cmFAST-3.2.0/joss-paper/yuxiangs-plot-small.png`

 * *Files identical despite different names*

### Comparing `21cmFAST-3.1.5/setup.py` & `21cmFAST-3.2.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -86,9 +86,13 @@
         "matplotlib",
         "bidict",
     ],
     extras_require={"tests": test_req, "docs": doc_req, "dev": test_req + doc_req},
     setup_requires=["cffi>=1.0", "setuptools_scm"],
     entry_points={"console_scripts": ["21cmfast = py21cmfast.cli:main"]},
     cffi_modules=[f"{pkgdir}/build_cffi.py:ffi"],
-    use_scm_version={"write_to": "src/py21cmfast/_version.py"},
+    use_scm_version={
+        "write_to": "src/py21cmfast/_version.py",
+        "parentdir_prefix_version": "21cmFAST-",
+        "fallback_version": "0.0.0",
+    },
 )
```

### Comparing `21cmFAST-3.1.5/src/21cmFAST.egg-info/PKG-INFO` & `21cmFAST-3.2.0/src/21cmFAST.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: 21cmFAST
-Version: 3.1.5
+Version: 3.2.0
 Summary: A semi-numerical cosmological simulation code for the 21cm signal
 Home-page: https://github.com/21cmFAST/21cmFAST
 Author: The 21cmFAST coredev team
 Author-email: 21cmfast.coredev@gmail.com
 License: MIT license
 Keywords: Epoch of Reionization,Cosmology
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Unix
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
@@ -193,22 +192,43 @@
 
 Changelog
 =========
 
 dev-version
 -----------
 
+v3.2.0 [11 Jul 2022]
+----------------------
+
+Changed
+~~~~~~~
+
+* Floats are now represented to a specific number of significant digits in the hash of
+  an output object. This fixes problems with very close redshifts not being read from
+  cache (#80). Note that this means that very close astro/cosmo params will now be read
+  from cache. This could cause issues when creating large databases with many random
+  parameters. The behaviour can modified in the configuration by setting the
+  ``cache_param_sigfigs`` and ``cache_redshift_sigfigs`` parameters (these are 6 and
+  4 by default, respectively).
+  **NOTE**: updating to this version will cause your previous cached files to become
+  unusable. Remove them before updating.
+
+Fixed
+~~~~~
+
+* Added a missing C-based error to the known errors in Python.
+
 v3.1.5 [27 Apr 2022]
 ----------------------
 
 v3.1.4 [10 Feb 2022]
 ----------------------
 
 Fixed
------
+~~~~~
 
 * error in FFT normalization in FindHaloes
 * docs not compiling on RTD due to missing ``scipy.integrate`` mock module
 * Updated matplotlib removed support for setting vmin/vmax and norm. Now passes vmin/vmax
   to the norm() constructor.
 
 v3.1.3 [27 Oct 2021]
@@ -446,9 +466,7 @@
   conditions and prints out an ASCII file with the associated power spectrum.
 - Parameter in Ts.c for the maximum allowed kinetic temperature, which increases
   stability of the code when the redshift step size and the X-ray efficiencies are large.
 
 Fixed
 ~~~~~
 - Oversight adding support for a Gaussian filter for the lower resolution field.
-
-
```

### Comparing `21cmFAST-3.1.5/src/21cmFAST.egg-info/SOURCES.txt` & `21cmFAST-3.2.0/src/21cmFAST.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `21cmFAST-3.1.5/src/py21cmfast/__init__.py` & `21cmFAST-3.2.0/src/py21cmfast/__init__.py`

 * *Files identical despite different names*

### Comparing `21cmFAST-3.1.5/src/py21cmfast/_cfg.py` & `21cmFAST-3.2.0/src/py21cmfast/_cfg.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,10 @@
 """Open and read the configuration file."""
+from __future__ import annotations
+
 import contextlib
 import copy
 import warnings
 from pathlib import Path
 
 from . import yaml
 
@@ -12,15 +14,21 @@
 
     pass
 
 
 class Config(dict):
     """Simple over-ride of dict that adds a context manager."""
 
-    _defaults = {"direc": "~/21cmFAST-cache", "regenerate": False, "write": True}
+    _defaults = {
+        "direc": "~/21cmFAST-cache",
+        "regenerate": False,
+        "write": True,
+        "cache_param_sigfigs": 6,
+        "cache_redshift_sigfigs": 4,
+    }
 
     _aliases = {"direc": ("boxdir",)}
 
     def __init__(self, *args, write=True, file_name=None, **kwargs):
 
         super().__init__(*args, **kwargs)
         self.file_name = file_name
@@ -69,30 +77,30 @@
         backup = self.copy()
         for k, v in kwargs.items():
             self[k] = Path(v).expanduser().absolute() if k == "direc" else v
         yield self
         for k in kwargs:
             self[k] = backup[k]
 
-    def write(self, fname: [str, Path, None] = None):
+    def write(self, fname: str | Path | None = None):
         """Write current configuration to file to make it permanent."""
         fname = Path(fname or self.file_name)
         if fname:
             if not fname.parent.exists():
                 fname.parent.mkdir(parents=True)
 
             with open(fname, "w") as fl:
                 yaml.dump(self._as_dict(), fl)
 
     def _as_dict(self):
         """The plain dict defining the instance."""
         return {k: str(Path) if isinstance(v, Path) else v for k, v in self.items()}
 
     @classmethod
-    def load(cls, file_name: [str, Path]):
+    def load(cls, file_name: str | Path):
         """Create a Config object from a config file."""
         file_name = Path(file_name).expanduser().absolute()
 
         if file_name.exists():
             with open(file_name) as fl:
                 cfg = yaml.load(fl)
             return cls(cfg, file_name=file_name)
```

### Comparing `21cmFAST-3.1.5/src/py21cmfast/_data/Transfers_z0.dat` & `21cmFAST-3.2.0/src/py21cmfast/_data/Transfers_z0.dat`

 * *Files identical despite different names*

### Comparing `21cmFAST-3.1.5/src/py21cmfast/_data/recfast_LCDM.dat` & `21cmFAST-3.2.0/src/py21cmfast/_data/recfast_LCDM.dat`

 * *Files identical despite different names*

### Comparing `21cmFAST-3.1.5/src/py21cmfast/_data/stellar_spectra.dat` & `21cmFAST-3.2.0/src/py21cmfast/_data/stellar_spectra.dat`

 * *Files identical despite different names*

### Comparing `21cmFAST-3.1.5/src/py21cmfast/_data/x_int_tables/log_xi_-1.0.dat` & `21cmFAST-3.2.0/src/py21cmfast/_data/x_int_tables/log_xi_-1.0.dat`

 * *Files identical despite different names*

### Comparing `21cmFAST-3.1.5/src/py21cmfast/_data/x_int_tables/log_xi_-1.3.dat` & `21cmFAST-3.2.0/src/py21cmfast/_data/x_int_tables/log_xi_-1.3.dat`

 * *Files identical despite different names*

### Comparing `21cmFAST-3.1.5/src/py21cmfast/_data/x_int_tables/log_xi_-1.6.dat` & `21cmFAST-3.2.0/src/py21cmfast/_data/x_int_tables/log_xi_-1.6.dat`

 * *Files identical despite different names*

### Comparing `21cmFAST-3.1.5/src/py21cmfast/_data/x_int_tables/log_xi_-2.0.dat` & `21cmFAST-3.2.0/src/py21cmfast/_data/x_int_tables/log_xi_-2.0.dat`

 * *Files identical despite different names*

### Comparing `21cmFAST-3.1.5/src/py21cmfast/_data/x_int_tables/log_xi_-2.3.dat` & `21cmFAST-3.2.0/src/py21cmfast/_data/x_int_tables/log_xi_-2.3.dat`

 * *Files identical despite different names*

### Comparing `21cmFAST-3.1.5/src/py21cmfast/_data/x_int_tables/log_xi_-2.6.dat` & `21cmFAST-3.2.0/src/py21cmfast/_data/x_int_tables/log_xi_-2.6.dat`

 * *Files identical despite different names*

### Comparing `21cmFAST-3.1.5/src/py21cmfast/_data/x_int_tables/log_xi_-3.0.dat` & `21cmFAST-3.2.0/src/py21cmfast/_data/x_int_tables/log_xi_-3.0.dat`

 * *Files identical despite different names*

### Comparing `21cmFAST-3.1.5/src/py21cmfast/_data/x_int_tables/log_xi_-3.3.dat` & `21cmFAST-3.2.0/src/py21cmfast/_data/x_int_tables/log_xi_-3.3.dat`

 * *Files identical despite different names*

### Comparing `21cmFAST-3.1.5/src/py21cmfast/_data/x_int_tables/log_xi_-3.6.dat` & `21cmFAST-3.2.0/src/py21cmfast/_data/x_int_tables/log_xi_-3.6.dat`

 * *Files identical despite different names*

### Comparing `21cmFAST-3.1.5/src/py21cmfast/_data/x_int_tables/log_xi_-4.0.dat` & `21cmFAST-3.2.0/src/py21cmfast/_data/x_int_tables/log_xi_-4.0.dat`

 * *Files identical despite different names*

### Comparing `21cmFAST-3.1.5/src/py21cmfast/_data/x_int_tables/xi_0.500.dat` & `21cmFAST-3.2.0/src/py21cmfast/_data/x_int_tables/xi_0.500.dat`

 * *Files identical despite different names*

### Comparing `21cmFAST-3.1.5/src/py21cmfast/_data/x_int_tables/xi_0.900.dat` & `21cmFAST-3.2.0/src/py21cmfast/_data/x_int_tables/xi_0.900.dat`

 * *Files identical despite different names*

### Comparing `21cmFAST-3.1.5/src/py21cmfast/_data/x_int_tables/xi_0.990.dat` & `21cmFAST-3.2.0/src/py21cmfast/_data/x_int_tables/xi_0.990.dat`

 * *Files identical despite different names*

### Comparing `21cmFAST-3.1.5/src/py21cmfast/_data/x_int_tables/xi_0.999.dat` & `21cmFAST-3.2.0/src/py21cmfast/_data/x_int_tables/xi_0.999.dat`

 * *Files identical despite different names*

### Comparing `21cmFAST-3.1.5/src/py21cmfast/_logging.py` & `21cmFAST-3.2.0/src/py21cmfast/_logging.py`

 * *Files identical despite different names*

### Comparing `21cmFAST-3.1.5/src/py21cmfast/_utils.py` & `21cmFAST-3.2.0/src/py21cmfast/_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -190,14 +190,15 @@
                 raise {
                     IOERROR: FileIOError,
                     GSLERROR: GSLError,
                     VALUEERROR: ArgumentValueError,
                     PHOTONCONSERROR: PhotonConsError,
                     TABLEGENERATIONERROR: TableGenerationError,
                     TABLEEVALUATIONERROR: TableEvaluationError,
+                    INFINITYORNANERROR: InfinityorNaNError,
                     MASSDEPZETAERROR: MassDepZetaError,
                     MEMORYALLOCERROR: MemoryAllocError,
                 }[exitcode]
             except KeyError:  # pragma: no cover
                 raise FatalCError(
                     "Unknown error in C. Please report this error!"
                 )  # Unknown C code
@@ -512,15 +513,26 @@
         return dct
 
     def __repr__(self):
         """Full unique representation of the instance."""
         return (
             self.__class__.__name__
             + "("
-            + ", ".join(sorted(k + ":" + str(v) for k, v in self.defining_dict.items()))
+            + ", ".join(
+                sorted(
+                    k
+                    + ":"
+                    + (
+                        float_to_string_precision(v, config["cache_redshift_sigfigs"])
+                        if isinstance(v, (float, np.float32))
+                        else str(v)
+                    )
+                    for k, v in self.defining_dict.items()
+                )
+            )
             + ")"
         )
 
     def __eq__(self, other):
         """Check whether this instance is equal to another object (by checking the __repr__)."""
         return self.__repr__() == repr(other)
 
@@ -552,14 +564,22 @@
 
     if not depublicize:
         word = word.lstrip("_")
 
     return word
 
 
+def float_to_string_precision(x, n):
+    """Prints out a standard float number at a given number of significant digits.
+
+    Code here: https://stackoverflow.com/a/48812729
+    """
+    return f'{float(f"{x:.{int(n)}g}"):g}'
+
+
 def get_all_subclasses(cls):
     """Get a list of all subclasses of a given class, recursively."""
     all_subclasses = []
 
     for subclass in cls.__subclasses__():
         all_subclasses.append(subclass)
         all_subclasses.extend(get_all_subclasses(subclass))
@@ -1209,15 +1229,21 @@
                 + "("
                 + "; ".join(
                     repr(v)
                     if isinstance(v, StructWithDefaults)
                     else (
                         v.filtered_repr(self._filter_params)
                         if isinstance(v, StructInstanceWrapper)
-                        else k.lstrip("_") + ":" + repr(v)
+                        else k.lstrip("_")
+                        + ":"
+                        + (
+                            float_to_string_precision(v, config["cache_param_sigfigs"])
+                            if isinstance(v, (float, np.float32))
+                            else repr(v)
+                        )
                     )
                     for k, v in [
                         (k, getattr(self, k))
                         for k in self._inputs + ("_global_params",)
                         if k != "_random_seed"
                     ]
                 )
```

### Comparing `21cmFAST-3.1.5/src/py21cmfast/cache_tools.py` & `21cmFAST-3.2.0/src/py21cmfast/cache_tools.py`

 * *Files identical despite different names*

### Comparing `21cmFAST-3.1.5/src/py21cmfast/cli.py` & `21cmFAST-3.2.0/src/py21cmfast/cli.py`

 * *Files identical despite different names*

### Comparing `21cmFAST-3.1.5/src/py21cmfast/inputs.py` & `21cmFAST-3.2.0/src/py21cmfast/inputs.py`

 * *Files identical despite different names*

### Comparing `21cmFAST-3.1.5/src/py21cmfast/outputs.py` & `21cmFAST-3.2.0/src/py21cmfast/outputs.py`

 * *Files identical despite different names*

### Comparing `21cmFAST-3.1.5/src/py21cmfast/plotting.py` & `21cmFAST-3.2.0/src/py21cmfast/plotting.py`

 * *Files identical despite different names*

### Comparing `21cmFAST-3.1.5/src/py21cmfast/src/21cmFAST.h` & `21cmFAST-3.2.0/src/py21cmfast/src/21cmFAST.h`

 * *Files identical despite different names*

### Comparing `21cmFAST-3.1.5/src/py21cmfast/src/BrightnessTemperatureBox.c` & `21cmFAST-3.2.0/src/py21cmfast/src/BrightnessTemperatureBox.c`

 * *Files identical despite different names*

### Comparing `21cmFAST-3.1.5/src/py21cmfast/src/Constants.h` & `21cmFAST-3.2.0/src/py21cmfast/src/Constants.h`

 * *Files identical despite different names*

### Comparing `21cmFAST-3.1.5/src/py21cmfast/src/FindHaloes.c` & `21cmFAST-3.2.0/src/py21cmfast/src/FindHaloes.c`

 * *Files identical despite different names*

### Comparing `21cmFAST-3.1.5/src/py21cmfast/src/GenerateICs.c` & `21cmFAST-3.2.0/src/py21cmfast/src/GenerateICs.c`

 * *Files identical despite different names*

### Comparing `21cmFAST-3.1.5/src/py21cmfast/src/Globals.h` & `21cmFAST-3.2.0/src/py21cmfast/src/Globals.h`

 * *Files identical despite different names*

### Comparing `21cmFAST-3.1.5/src/py21cmfast/src/IonisationBox.c` & `21cmFAST-3.2.0/src/py21cmfast/src/IonisationBox.c`

 * *Files identical despite different names*

### Comparing `21cmFAST-3.1.5/src/py21cmfast/src/PerturbField.c` & `21cmFAST-3.2.0/src/py21cmfast/src/PerturbField.c`

 * *Files identical despite different names*

### Comparing `21cmFAST-3.1.5/src/py21cmfast/src/PerturbHaloField.c` & `21cmFAST-3.2.0/src/py21cmfast/src/PerturbHaloField.c`

 * *Files identical despite different names*

### Comparing `21cmFAST-3.1.5/src/py21cmfast/src/SpinTemperatureBox.c` & `21cmFAST-3.2.0/src/py21cmfast/src/SpinTemperatureBox.c`

 * *Files identical despite different names*

### Comparing `21cmFAST-3.1.5/src/py21cmfast/src/UsefulFunctions.c` & `21cmFAST-3.2.0/src/py21cmfast/src/UsefulFunctions.c`

 * *Files identical despite different names*

### Comparing `21cmFAST-3.1.5/src/py21cmfast/src/bubble_helper_progs.c` & `21cmFAST-3.2.0/src/py21cmfast/src/bubble_helper_progs.c`

 * *Files identical despite different names*

### Comparing `21cmFAST-3.1.5/src/py21cmfast/src/cexcept.h` & `21cmFAST-3.2.0/src/py21cmfast/src/cexcept.h`

 * *Files identical despite different names*

### Comparing `21cmFAST-3.1.5/src/py21cmfast/src/dft.c` & `21cmFAST-3.2.0/src/py21cmfast/src/dft.c`

 * *Files identical despite different names*

### Comparing `21cmFAST-3.1.5/src/py21cmfast/src/elec_interp.c` & `21cmFAST-3.2.0/src/py21cmfast/src/elec_interp.c`

 * *Files identical despite different names*

### Comparing `21cmFAST-3.1.5/src/py21cmfast/src/exceptions.h` & `21cmFAST-3.2.0/src/py21cmfast/src/exceptions.h`

 * *Files identical despite different names*

### Comparing `21cmFAST-3.1.5/src/py21cmfast/src/heating_helper_progs.c` & `21cmFAST-3.2.0/src/py21cmfast/src/heating_helper_progs.c`

 * *Files identical despite different names*

### Comparing `21cmFAST-3.1.5/src/py21cmfast/src/indexing.c` & `21cmFAST-3.2.0/src/py21cmfast/src/indexing.c`

 * *Files identical despite different names*

### Comparing `21cmFAST-3.1.5/src/py21cmfast/src/logger.h` & `21cmFAST-3.2.0/src/py21cmfast/src/logger.h`

 * *Files identical despite different names*

### Comparing `21cmFAST-3.1.5/src/py21cmfast/src/ps.c` & `21cmFAST-3.2.0/src/py21cmfast/src/ps.c`

 * *Files identical despite different names*

### Comparing `21cmFAST-3.1.5/src/py21cmfast/src/recombinations.c` & `21cmFAST-3.2.0/src/py21cmfast/src/recombinations.c`

 * *Files identical despite different names*

### Comparing `21cmFAST-3.1.5/src/py21cmfast/wrapper.py` & `21cmFAST-3.2.0/src/py21cmfast/wrapper.py`

 * *Files 0% similar despite different names*

```diff
@@ -119,15 +119,15 @@
 logger = logging.getLogger(__name__)
 
 
 def _configure_inputs(
     defaults: list,
     *datasets,
     ignore: list = ["redshift"],
-    flag_none: [list, None] = None,
+    flag_none: Union[list, None] = None,
 ):
     """Configure a set of input parameter structs.
 
     This is useful for basing parameters on a previous output.
     The logic is this: the struct _cannot_ be present and different in both defaults and
     a dataset. If it is present in _either_ of them, that will be returned. If it is
     present in _neither_, either an error will be raised (if that item is in `flag_none`)
@@ -257,25 +257,27 @@
 
 
 def _get_config_options(
     direc, regenerate, write, hooks
 ) -> Tuple[str, bool, Dict[Callable, Dict[str, Any]]]:
 
     direc = str(os.path.expanduser(config["direc"] if direc is None else direc))
-    hooks = hooks or {}
 
-    if callable(write) and write not in hooks:
-        hooks[write] = {"direc": direc}
+    if hooks is None or len(hooks) > 0:
+        hooks = hooks or {}
 
-    if not hooks:
-        if write is None:
-            write = config["write"]
+        if callable(write) and write not in hooks:
+            hooks[write] = {"direc": direc}
 
-        if not callable(write) and write:
-            hooks["write"] = {"direc": direc}
+        if not hooks:
+            if write is None:
+                write = config["write"]
+
+            if not callable(write) and write:
+                hooks["write"] = {"direc": direc}
 
     return (
         direc,
         bool(config["regenerate"] if regenerate is None else regenerate),
         hooks,
     )
```

### Comparing `21cmFAST-3.1.5/src/py21cmfast/yaml.py` & `21cmFAST-3.2.0/src/py21cmfast/yaml.py`

 * *Files identical despite different names*

### Comparing `21cmFAST-3.1.5/tests/conftest.py` & `21cmFAST-3.2.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `21cmFAST-3.1.5/tests/plots/tests.test_integration_features.py--test_power_spectra_coeval[18-kwargs12].pdf` & `21cmFAST-3.2.0/tests/plots/tests.test_integration_features.py--test_power_spectra_coeval[18-kwargs12].pdf`

 * *Files identical despite different names*

### Comparing `21cmFAST-3.1.5/tests/produce_integration_test_data.py` & `21cmFAST-3.2.0/tests/produce_integration_test_data.py`

 * *Files identical despite different names*

### Comparing `21cmFAST-3.1.5/tests/test_cache_tools.py` & `21cmFAST-3.2.0/tests/test_cache_tools.py`

 * *Files identical despite different names*

### Comparing `21cmFAST-3.1.5/tests/test_cli.py` & `21cmFAST-3.2.0/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `21cmFAST-3.1.5/tests/test_config.py` & `21cmFAST-3.2.0/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `21cmFAST-3.1.5/tests/test_data/halo_field_data_halo_field.h5` & `21cmFAST-3.2.0/tests/test_data/halo_field_data_halo_field.h5`

 * *Files identical despite different names*

### Comparing `21cmFAST-3.1.5/tests/test_data/perturb_field_data_highres.h5` & `21cmFAST-3.2.0/tests/test_data/perturb_field_data_highres.h5`

 * *Files identical despite different names*

### Comparing `21cmFAST-3.1.5/tests/test_data/perturb_field_data_linear.h5` & `21cmFAST-3.2.0/tests/test_data/perturb_field_data_linear.h5`

 * *Files identical despite different names*

### Comparing `21cmFAST-3.1.5/tests/test_data/perturb_field_data_no2lpt.h5` & `21cmFAST-3.2.0/tests/test_data/perturb_field_data_no2lpt.h5`

 * *Files identical despite different names*

### Comparing `21cmFAST-3.1.5/tests/test_data/perturb_field_data_simple.h5` & `21cmFAST-3.2.0/tests/test_data/perturb_field_data_simple.h5`

 * *Files identical despite different names*

### Comparing `21cmFAST-3.1.5/tests/test_data/power_spectra_change_step_factor.h5` & `21cmFAST-3.2.0/tests/test_data/power_spectra_change_step_factor.h5`

 * *Files identical despite different names*

### Comparing `21cmFAST-3.1.5/tests/test_data/power_spectra_change_z_heat_max.h5` & `21cmFAST-3.2.0/tests/test_data/power_spectra_change_z_heat_max.h5`

 * *Files identical despite different names*

### Comparing `21cmFAST-3.1.5/tests/test_data/power_spectra_fast_fcoll_hiz.h5` & `21cmFAST-3.2.0/tests/test_data/power_spectra_fast_fcoll_hiz.h5`

 * *Files identical despite different names*

### Comparing `21cmFAST-3.1.5/tests/test_data/power_spectra_fast_fcoll_lowz.h5` & `21cmFAST-3.2.0/tests/test_data/power_spectra_fast_fcoll_lowz.h5`

 * *Files identical despite different names*

### Comparing `21cmFAST-3.1.5/tests/test_data/power_spectra_fftw_wisdom.h5` & `21cmFAST-3.2.0/tests/test_data/power_spectra_fftw_wisdom.h5`

 * *Files identical despite different names*

### Comparing `21cmFAST-3.1.5/tests/test_data/power_spectra_halo_field.h5` & `21cmFAST-3.2.0/tests/test_data/power_spectra_halo_field.h5`

 * *Files identical despite different names*

### Comparing `21cmFAST-3.1.5/tests/test_data/power_spectra_halo_field_mdz.h5` & `21cmFAST-3.2.0/tests/test_data/power_spectra_halo_field_mdz.h5`

 * *Files identical despite different names*

### Comparing `21cmFAST-3.1.5/tests/test_data/power_spectra_halo_field_mdz_highres.h5` & `21cmFAST-3.2.0/tests/test_data/power_spectra_halo_field_mdz_highres.h5`

 * *Files identical despite different names*

### Comparing `21cmFAST-3.1.5/tests/test_data/power_spectra_inhomo.h5` & `21cmFAST-3.2.0/tests/test_data/power_spectra_inhomo.h5`

 * *Files identical despite different names*

### Comparing `21cmFAST-3.1.5/tests/test_data/power_spectra_interp_perturb_field.h5` & `21cmFAST-3.2.0/tests/test_data/power_spectra_interp_perturb_field.h5`

 * *Files identical despite different names*

### Comparing `21cmFAST-3.1.5/tests/test_data/power_spectra_larger_step_factor.h5` & `21cmFAST-3.2.0/tests/test_data/power_spectra_larger_step_factor.h5`

 * *Files identical despite different names*

### Comparing `21cmFAST-3.1.5/tests/test_data/power_spectra_mdz_and_photoncons.h5` & `21cmFAST-3.2.0/tests/test_data/power_spectra_mdz_and_photoncons.h5`

 * *Files identical despite different names*

### Comparing `21cmFAST-3.1.5/tests/test_data/power_spectra_mdz_and_ts_fluct.h5` & `21cmFAST-3.2.0/tests/test_data/power_spectra_mdz_and_ts_fluct.h5`

 * *Files identical despite different names*

### Comparing `21cmFAST-3.1.5/tests/test_data/power_spectra_mdz_and_tsfluct_nthreads.h5` & `21cmFAST-3.2.0/tests/test_data/power_spectra_mdz_and_tsfluct_nthreads.h5`

 * *Files identical despite different names*

### Comparing `21cmFAST-3.1.5/tests/test_data/power_spectra_mdz_tsfluct_nthreads.h5` & `21cmFAST-3.2.0/tests/test_data/power_spectra_mdz_tsfluct_nthreads.h5`

 * *Files identical despite different names*

### Comparing `21cmFAST-3.1.5/tests/test_data/power_spectra_mdzeta.h5` & `21cmFAST-3.2.0/tests/test_data/power_spectra_mdzeta.h5`

 * *Files identical despite different names*

### Comparing `21cmFAST-3.1.5/tests/test_data/power_spectra_mini_halos.h5` & `21cmFAST-3.2.0/tests/test_data/power_spectra_mini_halos.h5`

 * *Files identical despite different names*

### Comparing `21cmFAST-3.1.5/tests/test_data/power_spectra_minihalos_no_tables.h5` & `21cmFAST-3.2.0/tests/test_data/power_spectra_minihalos_no_tables.h5`

 * *Files identical despite different names*

### Comparing `21cmFAST-3.1.5/tests/test_data/power_spectra_minimize_mem.h5` & `21cmFAST-3.2.0/tests/test_data/power_spectra_minimize_mem.h5`

 * *Files identical despite different names*

### Comparing `21cmFAST-3.1.5/tests/test_data/power_spectra_mmin_in_mass.h5` & `21cmFAST-3.2.0/tests/test_data/power_spectra_mmin_in_mass.h5`

 * *Files identical despite different names*

### Comparing `21cmFAST-3.1.5/tests/test_data/power_spectra_nthreads.h5` & `21cmFAST-3.2.0/tests/test_data/power_spectra_nthreads.h5`

 * *Files identical despite different names*

### Comparing `21cmFAST-3.1.5/tests/test_data/power_spectra_perturb_high_res.h5` & `21cmFAST-3.2.0/tests/test_data/power_spectra_perturb_high_res.h5`

 * *Files identical despite different names*

### Comparing `21cmFAST-3.1.5/tests/test_data/power_spectra_photoncons.h5` & `21cmFAST-3.2.0/tests/test_data/power_spectra_photoncons.h5`

 * *Files identical despite different names*

### Comparing `21cmFAST-3.1.5/tests/test_data/power_spectra_relvel.h5` & `21cmFAST-3.2.0/tests/test_data/power_spectra_relvel.h5`

 * *Files identical despite different names*

### Comparing `21cmFAST-3.1.5/tests/test_data/power_spectra_rsd.h5` & `21cmFAST-3.2.0/tests/test_data/power_spectra_rsd.h5`

 * *Files identical despite different names*

### Comparing `21cmFAST-3.1.5/tests/test_data/power_spectra_simple.h5` & `21cmFAST-3.2.0/tests/test_data/power_spectra_simple.h5`

 * *Files identical despite different names*

### Comparing `21cmFAST-3.1.5/tests/test_data/power_spectra_ts_fluct_no_tables.h5` & `21cmFAST-3.2.0/tests/test_data/power_spectra_ts_fluct_no_tables.h5`

 * *Files identical despite different names*

### Comparing `21cmFAST-3.1.5/tests/test_data/power_spectra_tsfluct.h5` & `21cmFAST-3.2.0/tests/test_data/power_spectra_tsfluct.h5`

 * *Files identical despite different names*

### Comparing `21cmFAST-3.1.5/tests/test_data/power_spectra_z9.00_INHOMO_RECO=True_MINIMIZE_MEMORY=True_PHOTON_CONS=True_USE_MASS_DEPENDENT_ZETA=True_USE_TS_FLUCT=True_z_heat_max=25_zprime_step_factor=1.1.h5` & `21cmFAST-3.2.0/tests/test_data/power_spectra_z9.00_INHOMO_RECO=True_MINIMIZE_MEMORY=True_PHOTON_CONS=True_USE_MASS_DEPENDENT_ZETA=True_USE_TS_FLUCT=True_z_heat_max=25_zprime_step_factor=1.1.h5`

 * *Files identical despite different names*

### Comparing `21cmFAST-3.1.5/tests/test_exceptions.py` & `21cmFAST-3.2.0/tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `21cmFAST-3.1.5/tests/test_high_level_io.py` & `21cmFAST-3.2.0/tests/test_high_level_io.py`

 * *Files identical despite different names*

### Comparing `21cmFAST-3.1.5/tests/test_initial_conditions.py` & `21cmFAST-3.2.0/tests/test_initial_conditions.py`

 * *Files identical despite different names*

### Comparing `21cmFAST-3.1.5/tests/test_input_structs.py` & `21cmFAST-3.2.0/tests/test_input_structs.py`

 * *Files identical despite different names*

### Comparing `21cmFAST-3.1.5/tests/test_integration_features.py` & `21cmFAST-3.2.0/tests/test_integration_features.py`

 * *Files identical despite different names*

### Comparing `21cmFAST-3.1.5/tests/test_output_structs.py` & `21cmFAST-3.2.0/tests/test_output_structs.py`

 * *Files identical despite different names*

### Comparing `21cmFAST-3.1.5/tests/test_plotting.py` & `21cmFAST-3.2.0/tests/test_plotting.py`

 * *Files identical despite different names*

### Comparing `21cmFAST-3.1.5/tests/test_spin_temp.py` & `21cmFAST-3.2.0/tests/test_spin_temp.py`

 * *Files identical despite different names*

### Comparing `21cmFAST-3.1.5/tests/test_wrapper.py` & `21cmFAST-3.2.0/tests/test_wrapper.py`

 * *Files identical despite different names*

