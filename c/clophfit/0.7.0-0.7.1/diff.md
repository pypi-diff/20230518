# Comparing `tmp/clophfit-0.7.0.tar.gz` & `tmp/clophfit-0.7.1.tar.gz`

## Comparing `clophfit-0.7.0.tar` & `clophfit-0.7.1.tar`

### file list

```diff
@@ -1,227 +1,228 @@
--rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 clophfit-0.7.0/.codespellrc
--rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 clophfit-0.7.0/.darglint
--rw-r--r--   0        0        0     2998 2020-02-02 00:00:00.000000 clophfit-0.7.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 clophfit-0.7.0/.python-version
--rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 clophfit-0.7.0/.readthedocs.yml
--rw-r--r--   0        0        0    14540 2020-02-02 00:00:00.000000 clophfit-0.7.0/CHANGELOG.md
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 clophfit-0.7.0/bandit.yml
--rw-r--r--   0        0        0     1285 2020-02-02 00:00:00.000000 clophfit-0.7.0/cz_customize_info.txt
--rw-r--r--   0        0        0      377 2020-02-02 00:00:00.000000 clophfit-0.7.0/.github/dependabot.yml
--rw-r--r--   0        0        0     6258 2020-02-02 00:00:00.000000 clophfit-0.7.0/.github/workflows/ci.yml
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 clophfit-0.7.0/.github/workflows/constraints.txt
--rw-r--r--   0        0        0     1800 2020-02-02 00:00:00.000000 clophfit-0.7.0/.github/workflows/docs.yml
--rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 clophfit-0.7.0/docs/Makefile
--rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 clophfit-0.7.0/docs/click.rst
--rw-r--r--   0        0        0     2574 2020-02-02 00:00:00.000000 clophfit-0.7.0/docs/conf.py
--rw-r--r--   0        0        0      963 2020-02-02 00:00:00.000000 clophfit-0.7.0/docs/index.rst
--rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 clophfit-0.7.0/docs/make.bat
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 clophfit-0.7.0/docs/_static/.gitkeep
--rw-r--r--   0        0        0    49846 2020-02-02 00:00:00.000000 clophfit-0.7.0/docs/_static/bs_pd_f1.png
--rw-r--r--   0        0        0    55458 2020-02-02 00:00:00.000000 clophfit-0.7.0/docs/_static/bs_pd_f2.png
--rw-r--r--   0        0        0    16105 2020-02-02 00:00:00.000000 clophfit-0.7.0/docs/_static/bs_pd_f3.png
--rw-r--r--   0        0        0    36779 2020-02-02 00:00:00.000000 clophfit-0.7.0/docs/_static/bs_pd_f4.png
--rw-r--r--   0        0        0    16293 2020-02-02 00:00:00.000000 clophfit-0.7.0/docs/_static/bs_pd_f5.png
--rw-r--r--   0        0        0    23529 2020-02-02 00:00:00.000000 clophfit-0.7.0/docs/_static/bs_pd_f6.png
--rw-r--r--   0        0        0    41234 2020-02-02 00:00:00.000000 clophfit-0.7.0/docs/_static/bs_pd_f7.png
--rw-r--r--   0        0        0     4101 2020-02-02 00:00:00.000000 clophfit-0.7.0/docs/_static/csvtable.png
--rw-r--r--   0        0        0    20158 2020-02-02 00:00:00.000000 clophfit-0.7.0/docs/_static/emcee-01.png
--rw-r--r--   0        0        0   109446 2020-02-02 00:00:00.000000 clophfit-0.7.0/docs/_static/emcee-02.png
--rw-r--r--   0        0        0    18582 2020-02-02 00:00:00.000000 clophfit-0.7.0/docs/_static/emcee-11.png
--rw-r--r--   0        0        0   420822 2020-02-02 00:00:00.000000 clophfit-0.7.0/docs/_static/emcee-12.png
--rw-r--r--   0        0        0    14293 2020-02-02 00:00:00.000000 clophfit-0.7.0/docs/_static/f01.png
--rw-r--r--   0        0        0     2156 2020-02-02 00:00:00.000000 clophfit-0.7.0/docs/_static/file.png
--rw-r--r--   0        0        0     7787 2020-02-02 00:00:00.000000 clophfit-0.7.0/docs/_static/gR_fit1.png
--rw-r--r--   0        0        0    32629 2020-02-02 00:00:00.000000 clophfit-0.7.0/docs/_static/gR_fit2.png
--rw-r--r--   0        0        0   117478 2020-02-02 00:00:00.000000 clophfit-0.7.0/docs/_static/gR_fit3.png
--rw-r--r--   0        0        0    42999 2020-02-02 00:00:00.000000 clophfit-0.7.0/docs/_static/gR_fit4.png
--rw-r--r--   0        0        0    83505 2020-02-02 00:00:00.000000 clophfit-0.7.0/docs/_static/gR_fit5.png
--rw-r--r--   0        0        0    12423 2020-02-02 00:00:00.000000 clophfit-0.7.0/docs/_static/gR_fit6.png
--rw-r--r--   0        0        0    14823 2020-02-02 00:00:00.000000 clophfit-0.7.0/docs/_static/gR_fit7.png
--rw-r--r--   0        0        0    18894 2020-02-02 00:00:00.000000 clophfit-0.7.0/docs/_static/glmfit0.png
--rw-r--r--   0        0        0    21702 2020-02-02 00:00:00.000000 clophfit-0.7.0/docs/_static/glmfit1.png
--rw-r--r--   0        0        0    33541 2020-02-02 00:00:00.000000 clophfit-0.7.0/docs/_static/glmfit2.png
--rw-r--r--   0        0        0    10655 2020-02-02 00:00:00.000000 clophfit-0.7.0/docs/_static/glmfit3.png
--rw-r--r--   0        0        0    34747 2020-02-02 00:00:00.000000 clophfit-0.7.0/docs/_static/glmfit_np.r_.png
--rw-r--r--   0        0        0    16358 2020-02-02 00:00:00.000000 clophfit-0.7.0/docs/_static/lmfit1.png
--rw-r--r--   0        0        0    29012 2020-02-02 00:00:00.000000 clophfit-0.7.0/docs/_static/lmfit2.png
--rw-r--r--   0        0        0    45332 2020-02-02 00:00:00.000000 clophfit-0.7.0/docs/_static/lmfit3.png
--rw-r--r--   0        0        0    48655 2020-02-02 00:00:00.000000 clophfit-0.7.0/docs/_static/lmfit4.png
--rw-r--r--   0        0        0    16400 2020-02-02 00:00:00.000000 clophfit-0.7.0/docs/_static/lmfit5.png
--rw-r--r--   0        0        0    21693 2020-02-02 00:00:00.000000 clophfit-0.7.0/docs/_static/lmodel1.png
--rw-r--r--   0        0        0    28428 2020-02-02 00:00:00.000000 clophfit-0.7.0/docs/_static/lmodel2.png
--rw-r--r--   0        0        0    11916 2020-02-02 00:00:00.000000 clophfit-0.7.0/docs/_static/lmodel3.png
--rw-r--r--   0        0        0    29389 2020-02-02 00:00:00.000000 clophfit-0.7.0/docs/_static/lmodel4.png
--rw-r--r--   0        0        0    23708 2020-02-02 00:00:00.000000 clophfit-0.7.0/docs/_static/lmodel5.png
--rw-r--r--   0        0        0   187683 2020-02-02 00:00:00.000000 clophfit-0.7.0/docs/_static/lmodel6.png
--rw-r--r--   0        0        0    24709 2020-02-02 00:00:00.000000 clophfit-0.7.0/docs/_static/lmodel_H04.png
--rw-r--r--   0        0        0     3195 2020-02-02 00:00:00.000000 clophfit-0.7.0/docs/_static/note_file.png
--rw-r--r--   0        0        0   101706 2020-02-02 00:00:00.000000 clophfit-0.7.0/docs/_static/r_bs.png
--rw-r--r--   0        0        0    24754 2020-02-02 00:00:00.000000 clophfit-0.7.0/docs/_static/ratio2P-lmodel1.png
--rw-r--r--   0        0        0    63411 2020-02-02 00:00:00.000000 clophfit-0.7.0/docs/_static/ratio2P-lmodel2.png
--rw-r--r--   0        0        0    31838 2020-02-02 00:00:00.000000 clophfit-0.7.0/docs/_static/ratio2P_R1.png
--rw-r--r--   0        0        0   114443 2020-02-02 00:00:00.000000 clophfit-0.7.0/docs/_static/ratio2P_R2.png
--rw-r--r--   0        0        0    43555 2020-02-02 00:00:00.000000 clophfit-0.7.0/docs/_static/ratio2P_R3.png
--rw-r--r--   0        0        0    94094 2020-02-02 00:00:00.000000 clophfit-0.7.0/docs/_static/ratio2P_R4.png
--rw-r--r--   0        0        0    10140 2020-02-02 00:00:00.000000 clophfit-0.7.0/docs/_static/ratio2P_R5.png
--rw-r--r--   0        0        0    14971 2020-02-02 00:00:00.000000 clophfit-0.7.0/docs/_static/ratio2P_R6.png
--rw-r--r--   0        0        0   101706 2020-02-02 00:00:00.000000 clophfit-0.7.0/docs/_static/rpy_bs.png
--rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 clophfit-0.7.0/docs/api/api.rst
--rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 clophfit-0.7.0/docs/api/binding.rst
--rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 clophfit-0.7.0/docs/api/prenspire.rst
--rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 clophfit-0.7.0/docs/api/prtecan.rst
--rw-r--r--   0        0        0     1359 2020-02-02 00:00:00.000000 clophfit-0.7.0/docs/references/contributing.rst
--rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 clophfit-0.7.0/docs/references/description.rst
--rw-r--r--   0        0        0     3983 2020-02-02 00:00:00.000000 clophfit-0.7.0/docs/references/development.rst
--rw-r--r--   0        0        0     1851 2020-02-02 00:00:00.000000 clophfit-0.7.0/docs/references/older.rst
--rw-r--r--   0        0        0     2542 2020-02-02 00:00:00.000000 clophfit-0.7.0/docs/references/prenspire.rst
--rw-r--r--   0        0        0     3552 2020-02-02 00:00:00.000000 clophfit-0.7.0/docs/references/prtecan.rst
--rw-r--r--   0        0        0     2574 2020-02-02 00:00:00.000000 clophfit-0.7.0/docs/references/prtecan.uml.rst
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 clophfit-0.7.0/docs/references/references.rst
--rw-r--r--   0        0        0   174462 2020-02-02 00:00:00.000000 clophfit-0.7.0/docs/tutorials/prenspire.ipynb
--rw-r--r--   0        0        0  1959014 2020-02-02 00:00:00.000000 clophfit-0.7.0/docs/tutorials/prtecan.ipynb
--rw-r--r--   0        0        0      377 2020-02-02 00:00:00.000000 clophfit-0.7.0/docs/tutorials/tutorials.rst
--rw-r--r--   0        0        0     9075 2020-02-02 00:00:00.000000 clophfit-0.7.0/docs/tutorials/usage.org
--rw-r--r--   0        0        0    14299 2020-02-02 00:00:00.000000 clophfit-0.7.0/docs/tutorials/usage.rst
--rw-r--r--   0        0        0    30911 2020-02-02 00:00:00.000000 clophfit-0.7.0/docs/tutorials/usage2.org
--rw-r--r--   0        0        0    58554 2020-02-02 00:00:00.000000 clophfit-0.7.0/docs/tutorials/usage2.rst
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 clophfit-0.7.0/src/clophfit/__init__.py
--rw-r--r--   0        0        0     7913 2020-02-02 00:00:00.000000 clophfit-0.7.0/src/clophfit/__main__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 clophfit-0.7.0/src/clophfit/py.typed
--rw-r--r--   0        0        0      333 2020-02-02 00:00:00.000000 clophfit-0.7.0/src/clophfit/binding/__init__.py
--rw-r--r--   0        0        0     6321 2020-02-02 00:00:00.000000 clophfit-0.7.0/src/clophfit/binding/fitting.py
--rwxr-xr-x   0        0        0     1386 2020-02-02 00:00:00.000000 clophfit-0.7.0/src/clophfit/old/dil_buffer.py
--rwxr-xr-x   0        0        0     1320 2020-02-02 00:00:00.000000 clophfit-0.7.0/src/clophfit/old/dil_correction.py
--rwxr-xr-x   0        0        0     5639 2020-02-02 00:00:00.000000 clophfit-0.7.0/src/clophfit/old/fit_rpy.py
--rwxr-xr-x   0        0        0     7936 2020-02-02 00:00:00.000000 clophfit-0.7.0/src/clophfit/old/fit_titration.py
--rwxr-xr-x   0        0        0     6060 2020-02-02 00:00:00.000000 clophfit-0.7.0/src/clophfit/old/fit_titration_global.py
--rwxr-xr-x   0        0        0      634 2020-02-02 00:00:00.000000 clophfit-0.7.0/src/clophfit/old/merge.py
--rwxr-xr-x   0        0        0      891 2020-02-02 00:00:00.000000 clophfit-0.7.0/src/clophfit/old/plot_tecan.py
--rwxr-xr-x   0        0        0      119 2020-02-02 00:00:00.000000 clophfit-0.7.0/src/clophfit/old/bash/fit.tecan
--rwxr-xr-x   0        0        0      115 2020-02-02 00:00:00.000000 clophfit-0.7.0/src/clophfit/old/bash/fit.tecan.cl
--rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 clophfit-0.7.0/src/clophfit/old/bash/new_sort_K.sh
--rwxr-xr-x   0        0        0      222 2020-02-02 00:00:00.000000 clophfit-0.7.0/src/clophfit/old/bash/sum_all
--rwxr-xr-x   0        0        0      260 2020-02-02 00:00:00.000000 clophfit-0.7.0/src/clophfit/old/bash/sum_e2
--rwxr-xr-x   0        0        0      352 2020-02-02 00:00:00.000000 clophfit-0.7.0/src/clophfit/old/bash/sum_lib
--rwxr-xr-x   0        0        0      427 2020-02-02 00:00:00.000000 clophfit-0.7.0/src/clophfit/old/bash/sum_lib2
--rwxr-xr-x   0        0        0      260 2020-02-02 00:00:00.000000 clophfit-0.7.0/src/clophfit/old/bash/sum_s202n
--rwxr-xr-x   0        0        0      260 2020-02-02 00:00:00.000000 clophfit-0.7.0/src/clophfit/old/bash/sum_v224q
--rwxr-xr-x   0        0        0      572 2020-02-02 00:00:00.000000 clophfit-0.7.0/src/clophfit/old/bash/w_ave.sh
--rw-r--r--   0        0        0      605 2020-02-02 00:00:00.000000 clophfit-0.7.0/src/clophfit/prenspire/__init__.py
--rw-r--r--   0        0        0    17676 2020-02-02 00:00:00.000000 clophfit-0.7.0/src/clophfit/prenspire/prenspire.py
--rw-r--r--   0        0        0     2007 2020-02-02 00:00:00.000000 clophfit-0.7.0/src/clophfit/prtecan/__init__.py
--rw-r--r--   0        0        0    54191 2020-02-02 00:00:00.000000 clophfit-0.7.0/src/clophfit/prtecan/prtecan.py
--rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 clophfit-0.7.0/tests/conftest.py
--rw-r--r--   0        0        0     1261 2020-02-02 00:00:00.000000 clophfit-0.7.0/tests/test_binding.py
--rw-r--r--   0        0        0     2190 2020-02-02 00:00:00.000000 clophfit-0.7.0/tests/test_cli.py
--rw-r--r--   0        0        0     5923 2020-02-02 00:00:00.000000 clophfit-0.7.0/tests/test_oldscripts.py
--rw-r--r--   0        0        0     8407 2020-02-02 00:00:00.000000 clophfit-0.7.0/tests/test_prenspire.py
--rw-r--r--   0        0        0    26298 2020-02-02 00:00:00.000000 clophfit-0.7.0/tests/test_prtecan.py
--rw-r--r--   0        0        0    34305 2020-02-02 00:00:00.000000 clophfit-0.7.0/tests/EnSpire/24well_clop0_95.csv
--rw-r--r--   0        0        0   103231 2020-02-02 00:00:00.000000 clophfit-0.7.0/tests/EnSpire/e2-T-without_sample_column.csv
--rw-r--r--   0        0        0      812 2020-02-02 00:00:00.000000 clophfit-0.7.0/tests/EnSpire/h148g-spettroC-nota
--rw-r--r--   0        0        0      737 2020-02-02 00:00:00.000000 clophfit-0.7.0/tests/EnSpire/h148g-spettroC-nota-Err
--rw-r--r--   0        0        0   373790 2020-02-02 00:00:00.000000 clophfit-0.7.0/tests/EnSpire/h148g-spettroC.csv
--rw-r--r--   0        0        0    98464 2020-02-02 00:00:00.000000 clophfit-0.7.0/tests/EnSpire/cli/NTT_37C_pKa.csv
--rw-r--r--   0        0        0    17235 2020-02-02 00:00:00.000000 clophfit-0.7.0/tests/EnSpire/cli/output/NTT_37C_pKa_A.csv
--rw-r--r--   0        0        0    68449 2020-02-02 00:00:00.000000 clophfit-0.7.0/tests/EnSpire/cli/output/NTT_37C_pKa_A.png
--rw-r--r--   0        0        0    18266 2020-02-02 00:00:00.000000 clophfit-0.7.0/tests/EnSpire/cli/output/NTT_37C_pKa_B.csv
--rw-r--r--   0        0        0    53309 2020-02-02 00:00:00.000000 clophfit-0.7.0/tests/EnSpire/cli/output/NTT_37C_pKa_B.png
--rw-r--r--   0        0        0    13404 2020-02-02 00:00:00.000000 clophfit-0.7.0/tests/EnSpire/exceptions/M1-A6-G12_11columns.csv
--rw-r--r--   0        0        0    13405 2020-02-02 00:00:00.000000 clophfit-0.7.0/tests/EnSpire/exceptions/M1-A6-G12_missing_emptyline_fin.csv
--rw-r--r--   0        0        0    13405 2020-02-02 00:00:00.000000 clophfit-0.7.0/tests/EnSpire/exceptions/M1-A6-G12_missing_emptyline_ini.csv
--rw-r--r--   0        0        0   103682 2020-02-02 00:00:00.000000 clophfit-0.7.0/tests/EnSpire/exceptions/e2dan-emwavelength.csv
--rw-r--r--   0        0        0   104940 2020-02-02 00:00:00.000000 clophfit-0.7.0/tests/EnSpire/exceptions/e2dan-exwavelength.csv
--rw-r--r--   0        0        0   104940 2020-02-02 00:00:00.000000 clophfit-0.7.0/tests/EnSpire/exceptions/e2dan-exwavelength2.csv
--rw-r--r--   0        0        0   104939 2020-02-02 00:00:00.000000 clophfit-0.7.0/tests/EnSpire/exceptions/e2dan-exwavelengthstrange.csv
--rw-r--r--   0        0        0   344763 2020-02-02 00:00:00.000000 clophfit-0.7.0/tests/EnSpire/exceptions/h148g-spettroC-idx0.csv
--rw-r--r--   0        0        0   373857 2020-02-02 00:00:00.000000 clophfit-0.7.0/tests/EnSpire/exceptions/h148g-spettroC-idx2.csv
--rw-r--r--   0        0        0   344941 2020-02-02 00:00:00.000000 clophfit-0.7.0/tests/EnSpire/warnings/h148g-spettroC-incomplete.csv
--rw-r--r--   0        0        0    12062 2020-02-02 00:00:00.000000 clophfit-0.7.0/tests/Tecan/290212_100.xls
--rw-r--r--   0        0        0    12073 2020-02-02 00:00:00.000000 clophfit-0.7.0/tests/Tecan/290212_150.xls
--rw-r--r--   0        0        0    12069 2020-02-02 00:00:00.000000 clophfit-0.7.0/tests/Tecan/290212_20.xls
--rw-r--r--   0        0        0    13122 2020-02-02 00:00:00.000000 clophfit-0.7.0/tests/Tecan/290212_5.78.xls
--rw-r--r--   0        0        0    12062 2020-02-02 00:00:00.000000 clophfit-0.7.0/tests/Tecan/290212_50.xls
--rw-r--r--   0        0        0    13140 2020-02-02 00:00:00.000000 clophfit-0.7.0/tests/Tecan/290212_6.38.xls
--rw-r--r--   0        0        0    13137 2020-02-02 00:00:00.000000 clophfit-0.7.0/tests/Tecan/290212_6.83.xls
--rw-r--r--   0        0        0    13146 2020-02-02 00:00:00.000000 clophfit-0.7.0/tests/Tecan/290212_7.24.xls
--rw-r--r--   0        0        0    13141 2020-02-02 00:00:00.000000 clophfit-0.7.0/tests/Tecan/290212_7.67.xls
--rw-r--r--   0        0        0    13173 2020-02-02 00:00:00.000000 clophfit-0.7.0/tests/Tecan/290212_8.23.xls
--rw-r--r--   0        0        0    13171 2020-02-02 00:00:00.000000 clophfit-0.7.0/tests/Tecan/290212_8.82.xls
--rw-r--r--   0        0        0    13152 2020-02-02 00:00:00.000000 clophfit-0.7.0/tests/Tecan/290212_9.31.xls
--rw-r--r--   0        0        0    12930 2020-02-02 00:00:00.000000 clophfit-0.7.0/tests/Tecan/290513_5.5.xls
--rw-r--r--   0        0        0    11262 2020-02-02 00:00:00.000000 clophfit-0.7.0/tests/Tecan/290513_5.5_bad.xls
--rw-r--r--   0        0        0    12946 2020-02-02 00:00:00.000000 clophfit-0.7.0/tests/Tecan/290513_7.2.xls
--rw-r--r--   0        0        0    12975 2020-02-02 00:00:00.000000 clophfit-0.7.0/tests/Tecan/290513_8.8.xls
--rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 clophfit-0.7.0/tests/Tecan/list.cl
--rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 clophfit-0.7.0/tests/Tecan/list.cl20
--rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 clophfit-0.7.0/tests/Tecan/list.pH
--rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 clophfit-0.7.0/tests/Tecan/list.pH2
--rw-r--r--   0        0        0    14438 2020-02-02 00:00:00.000000 clophfit-0.7.0/tests/Tecan/140220/200214 pH data.ods
--rw-r--r--   0        0        0    12835 2020-02-02 00:00:00.000000 clophfit-0.7.0/tests/Tecan/140220/NaCl1_200214.xls
--rw-r--r--   0        0        0    12812 2020-02-02 00:00:00.000000 clophfit-0.7.0/tests/Tecan/140220/NaCl2_200214.xls
--rw-r--r--   0        0        0    12802 2020-02-02 00:00:00.000000 clophfit-0.7.0/tests/Tecan/140220/NaCl3_200214.xls
--rw-r--r--   0        0        0    12799 2020-02-02 00:00:00.000000 clophfit-0.7.0/tests/Tecan/140220/NaCl4_200214.xls
--rw-r--r--   0        0        0    12812 2020-02-02 00:00:00.000000 clophfit-0.7.0/tests/Tecan/140220/NaCl5_200214.xls
--rw-r--r--   0        0        0    12773 2020-02-02 00:00:00.000000 clophfit-0.7.0/tests/Tecan/140220/NaCl6_200214.xls
--rw-r--r--   0        0        0    12783 2020-02-02 00:00:00.000000 clophfit-0.7.0/tests/Tecan/140220/NaCl7_200214.xls
--rw-r--r--   0        0        0    12790 2020-02-02 00:00:00.000000 clophfit-0.7.0/tests/Tecan/140220/NaCl8_200214.xls
--rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 clophfit-0.7.0/tests/Tecan/140220/additions.cl
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 clophfit-0.7.0/tests/Tecan/140220/additions.pH
--rw-r--r--   0        0        0    21877 2020-02-02 00:00:00.000000 clophfit-0.7.0/tests/Tecan/140220/fit0-1.csv
--rw-r--r--   0        0        0    21592 2020-02-02 00:00:00.000000 clophfit-0.7.0/tests/Tecan/140220/fit0.csv
--rw-r--r--   0        0        0    23056 2020-02-02 00:00:00.000000 clophfit-0.7.0/tests/Tecan/140220/fit1-1.csv
--rw-r--r--   0        0        0    23182 2020-02-02 00:00:00.000000 clophfit-0.7.0/tests/Tecan/140220/fit1.csv
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 clophfit-0.7.0/tests/Tecan/140220/list.cl
--rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 clophfit-0.7.0/tests/Tecan/140220/list.pH
--rw-r--r--   0        0        0    12865 2020-02-02 00:00:00.000000 clophfit-0.7.0/tests/Tecan/140220/pH5.0_200214.xls
--rw-r--r--   0        0        0    12901 2020-02-02 00:00:00.000000 clophfit-0.7.0/tests/Tecan/140220/pH5.8_200214.xls
--rw-r--r--   0        0        0    12889 2020-02-02 00:00:00.000000 clophfit-0.7.0/tests/Tecan/140220/pH6.5_200214.xls
--rw-r--r--   0        0        0    12914 2020-02-02 00:00:00.000000 clophfit-0.7.0/tests/Tecan/140220/pH7.1_200214.xls
--rw-r--r--   0        0        0    12934 2020-02-02 00:00:00.000000 clophfit-0.7.0/tests/Tecan/140220/pH7.6_200214.xls
--rw-r--r--   0        0        0    12939 2020-02-02 00:00:00.000000 clophfit-0.7.0/tests/Tecan/140220/pH8.3_200214.xls
--rw-r--r--   0        0        0    12937 2020-02-02 00:00:00.000000 clophfit-0.7.0/tests/Tecan/140220/pH9.1_200214.xls
--rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 clophfit-0.7.0/tests/Tecan/140220/scheme.txt
--rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 clophfit-0.7.0/tests/Tecan/140220/scheme0.txt
--rw-r--r--   0        0        0     9176 2020-02-02 00:00:00.000000 clophfit-0.7.0/tests/Tecan/exceptions/0_Labelblocks_290513_5.5.xlsx
--rw-r--r--   0        0        0    12275 2020-02-02 00:00:00.000000 clophfit-0.7.0/tests/Tecan/exceptions/290212_7.67_repeated_lb.xls
--rw-r--r--   0        0        0    10209 2020-02-02 00:00:00.000000 clophfit-0.7.0/tests/Tecan/exceptions/84wells_290212_20.xlsx
--rw-r--r--   0        0        0    10431 2020-02-02 00:00:00.000000 clophfit-0.7.0/tests/Tecan/exceptions/88wells_290212_20.xlsx
--rw-r--r--   0        0        0      525 2020-02-02 00:00:00.000000 clophfit-0.7.0/tests/data/A01-20140311a.dat
--rw-r--r--   0        0        0      525 2020-02-02 00:00:00.000000 clophfit-0.7.0/tests/data/A01.dat
--rw-r--r--   0        0        0      508 2020-02-02 00:00:00.000000 clophfit-0.7.0/tests/data/A11.dat
--rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 clophfit-0.7.0/tests/data/B01.dat
--rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 clophfit-0.7.0/tests/data/H04.dat
--rw-r--r--   0        0        0      537 2020-02-02 00:00:00.000000 clophfit-0.7.0/tests/data/NTT-A04-Cl_note
--rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 clophfit-0.7.0/tests/data/copyIP.txt
--rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 clophfit-0.7.0/tests/data/ratio2P.txt
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 clophfit-0.7.0/tests/data/w.txt
--rw-r--r--   0        0        0    43486 2020-02-02 00:00:00.000000 clophfit-0.7.0/tests/data/Meas/A04 Cl_A.csv
--rw-r--r--   0        0        0   138192 2020-02-02 00:00:00.000000 clophfit-0.7.0/tests/data/Meas/A04 Cl_A.png
--rw-r--r--   0        0        0    29087 2020-02-02 00:00:00.000000 clophfit-0.7.0/tests/data/Meas/A04 Cl_B.csv
--rw-r--r--   0        0        0    97762 2020-02-02 00:00:00.000000 clophfit-0.7.0/tests/data/Meas/A04 Cl_B.png
--rw-r--r--   0        0        0    35910 2020-02-02 00:00:00.000000 clophfit-0.7.0/tests/data/Meas/A04 Cl_C.csv
--rw-r--r--   0        0        0   138239 2020-02-02 00:00:00.000000 clophfit-0.7.0/tests/data/Meas/A04 Cl_C.png
--rw-r--r--   0        0        0    29248 2020-02-02 00:00:00.000000 clophfit-0.7.0/tests/data/Meas/A04 Cl_D.csv
--rw-r--r--   0        0        0    84749 2020-02-02 00:00:00.000000 clophfit-0.7.0/tests/data/Meas/A04 Cl_D.png
--rw-r--r--   0        0        0    35312 2020-02-02 00:00:00.000000 clophfit-0.7.0/tests/data/Meas/A04 Cl_E.csv
--rw-r--r--   0        0        0   145114 2020-02-02 00:00:00.000000 clophfit-0.7.0/tests/data/Meas/A04 Cl_E.png
--rw-r--r--   0        0        0    43756 2020-02-02 00:00:00.000000 clophfit-0.7.0/tests/data/Meas/A04 Cl_F.csv
--rw-r--r--   0        0        0   126442 2020-02-02 00:00:00.000000 clophfit-0.7.0/tests/data/Meas/A04 Cl_F.png
--rw-r--r--   0        0        0      508 2020-02-02 00:00:00.000000 clophfit-0.7.0/tests/data/global/Cl/A11-failed.dat
--rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 clophfit-0.7.0/tests/data/global/Cl/B05-20130628-cor.dat
--rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 clophfit-0.7.0/tests/data/global/pH/B01-failed.dat
--rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 clophfit-0.7.0/tests/data/global/pH/D05.dat
--rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 clophfit-0.7.0/tests/data/global/pH/H04-with_nan.dat
--rw-r--r--   0        0        0   235947 2020-02-02 00:00:00.000000 clophfit-0.7.0/tests/data/k/D05.dat-bs.png
--rw-r--r--   0        0        0    28093 2020-02-02 00:00:00.000000 clophfit-0.7.0/tests/data/k/D05.dat.png
--rw-r--r--   0        0        0    12506 2020-02-02 00:00:00.000000 clophfit-0.7.0/tests/data/output/band_A04 Cl_A_NTT-A04-Cl_note.pdf
--rw-r--r--   0        0        0    12433 2020-02-02 00:00:00.000000 clophfit-0.7.0/tests/data/output/band_A04 Cl_B_NTT-A04-Cl_note.pdf
--rw-r--r--   0        0        0    66713 2020-02-02 00:00:00.000000 clophfit-0.7.0/tests/data/output/svd_A04 Cl_A_NTT-A04-Cl_note.pdf
--rw-r--r--   0        0        0    39832 2020-02-02 00:00:00.000000 clophfit-0.7.0/tests/data/output/svd_A04 Cl_B_NTT-A04-Cl_note.pdf
--rw-r--r--   0        0        0    32564 2020-02-02 00:00:00.000000 clophfit-0.7.0/tests/data/output/global/Cl/B05-20130628-cor.dat.png
--rw-r--r--   0        0        0    36956 2020-02-02 00:00:00.000000 clophfit-0.7.0/tests/data/output/global/pH/D05.dat.png
--rw-r--r--   0        0        0      821 2020-02-02 00:00:00.000000 clophfit-0.7.0/.gitignore
--rw-r--r--   0        0        0     1480 2020-02-02 00:00:00.000000 clophfit-0.7.0/LICENSE.txt
--rw-r--r--   0        0        0     3475 2020-02-02 00:00:00.000000 clophfit-0.7.0/README.md
--rw-r--r--   0        0        0    11259 2020-02-02 00:00:00.000000 clophfit-0.7.0/pyproject.toml
--rw-r--r--   0        0        0     6266 2020-02-02 00:00:00.000000 clophfit-0.7.0/PKG-INFO
+-rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 clophfit-0.7.1/.codespellrc
+-rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 clophfit-0.7.1/.darglint
+-rw-r--r--   0        0        0     2998 2020-02-02 00:00:00.000000 clophfit-0.7.1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 clophfit-0.7.1/.python-version
+-rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 clophfit-0.7.1/.readthedocs.yml
+-rw-r--r--   0        0        0    15185 2020-02-02 00:00:00.000000 clophfit-0.7.1/CHANGELOG.md
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 clophfit-0.7.1/bandit.yml
+-rw-r--r--   0        0        0     1285 2020-02-02 00:00:00.000000 clophfit-0.7.1/cz_customize_info.txt
+-rw-r--r--   0        0        0      377 2020-02-02 00:00:00.000000 clophfit-0.7.1/.github/dependabot.yml
+-rw-r--r--   0        0        0     6258 2020-02-02 00:00:00.000000 clophfit-0.7.1/.github/workflows/ci.yml
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 clophfit-0.7.1/.github/workflows/constraints.txt
+-rw-r--r--   0        0        0     1800 2020-02-02 00:00:00.000000 clophfit-0.7.1/.github/workflows/docs.yml
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 clophfit-0.7.1/docs/Makefile
+-rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 clophfit-0.7.1/docs/click.rst
+-rw-r--r--   0        0        0     2574 2020-02-02 00:00:00.000000 clophfit-0.7.1/docs/conf.py
+-rw-r--r--   0        0        0      963 2020-02-02 00:00:00.000000 clophfit-0.7.1/docs/index.rst
+-rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 clophfit-0.7.1/docs/make.bat
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 clophfit-0.7.1/docs/_static/.gitkeep
+-rw-r--r--   0        0        0    49846 2020-02-02 00:00:00.000000 clophfit-0.7.1/docs/_static/bs_pd_f1.png
+-rw-r--r--   0        0        0    55458 2020-02-02 00:00:00.000000 clophfit-0.7.1/docs/_static/bs_pd_f2.png
+-rw-r--r--   0        0        0    16105 2020-02-02 00:00:00.000000 clophfit-0.7.1/docs/_static/bs_pd_f3.png
+-rw-r--r--   0        0        0    36779 2020-02-02 00:00:00.000000 clophfit-0.7.1/docs/_static/bs_pd_f4.png
+-rw-r--r--   0        0        0    16293 2020-02-02 00:00:00.000000 clophfit-0.7.1/docs/_static/bs_pd_f5.png
+-rw-r--r--   0        0        0    23529 2020-02-02 00:00:00.000000 clophfit-0.7.1/docs/_static/bs_pd_f6.png
+-rw-r--r--   0        0        0    41234 2020-02-02 00:00:00.000000 clophfit-0.7.1/docs/_static/bs_pd_f7.png
+-rw-r--r--   0        0        0     4101 2020-02-02 00:00:00.000000 clophfit-0.7.1/docs/_static/csvtable.png
+-rw-r--r--   0        0        0    20158 2020-02-02 00:00:00.000000 clophfit-0.7.1/docs/_static/emcee-01.png
+-rw-r--r--   0        0        0   109446 2020-02-02 00:00:00.000000 clophfit-0.7.1/docs/_static/emcee-02.png
+-rw-r--r--   0        0        0    18582 2020-02-02 00:00:00.000000 clophfit-0.7.1/docs/_static/emcee-11.png
+-rw-r--r--   0        0        0   420822 2020-02-02 00:00:00.000000 clophfit-0.7.1/docs/_static/emcee-12.png
+-rw-r--r--   0        0        0    14293 2020-02-02 00:00:00.000000 clophfit-0.7.1/docs/_static/f01.png
+-rw-r--r--   0        0        0     2156 2020-02-02 00:00:00.000000 clophfit-0.7.1/docs/_static/file.png
+-rw-r--r--   0        0        0     7787 2020-02-02 00:00:00.000000 clophfit-0.7.1/docs/_static/gR_fit1.png
+-rw-r--r--   0        0        0    32629 2020-02-02 00:00:00.000000 clophfit-0.7.1/docs/_static/gR_fit2.png
+-rw-r--r--   0        0        0   117478 2020-02-02 00:00:00.000000 clophfit-0.7.1/docs/_static/gR_fit3.png
+-rw-r--r--   0        0        0    42999 2020-02-02 00:00:00.000000 clophfit-0.7.1/docs/_static/gR_fit4.png
+-rw-r--r--   0        0        0    83505 2020-02-02 00:00:00.000000 clophfit-0.7.1/docs/_static/gR_fit5.png
+-rw-r--r--   0        0        0    12423 2020-02-02 00:00:00.000000 clophfit-0.7.1/docs/_static/gR_fit6.png
+-rw-r--r--   0        0        0    14823 2020-02-02 00:00:00.000000 clophfit-0.7.1/docs/_static/gR_fit7.png
+-rw-r--r--   0        0        0    18894 2020-02-02 00:00:00.000000 clophfit-0.7.1/docs/_static/glmfit0.png
+-rw-r--r--   0        0        0    21702 2020-02-02 00:00:00.000000 clophfit-0.7.1/docs/_static/glmfit1.png
+-rw-r--r--   0        0        0    33541 2020-02-02 00:00:00.000000 clophfit-0.7.1/docs/_static/glmfit2.png
+-rw-r--r--   0        0        0    10655 2020-02-02 00:00:00.000000 clophfit-0.7.1/docs/_static/glmfit3.png
+-rw-r--r--   0        0        0    34747 2020-02-02 00:00:00.000000 clophfit-0.7.1/docs/_static/glmfit_np.r_.png
+-rw-r--r--   0        0        0    16358 2020-02-02 00:00:00.000000 clophfit-0.7.1/docs/_static/lmfit1.png
+-rw-r--r--   0        0        0    29012 2020-02-02 00:00:00.000000 clophfit-0.7.1/docs/_static/lmfit2.png
+-rw-r--r--   0        0        0    45332 2020-02-02 00:00:00.000000 clophfit-0.7.1/docs/_static/lmfit3.png
+-rw-r--r--   0        0        0    48655 2020-02-02 00:00:00.000000 clophfit-0.7.1/docs/_static/lmfit4.png
+-rw-r--r--   0        0        0    16400 2020-02-02 00:00:00.000000 clophfit-0.7.1/docs/_static/lmfit5.png
+-rw-r--r--   0        0        0    21693 2020-02-02 00:00:00.000000 clophfit-0.7.1/docs/_static/lmodel1.png
+-rw-r--r--   0        0        0    28428 2020-02-02 00:00:00.000000 clophfit-0.7.1/docs/_static/lmodel2.png
+-rw-r--r--   0        0        0    11916 2020-02-02 00:00:00.000000 clophfit-0.7.1/docs/_static/lmodel3.png
+-rw-r--r--   0        0        0    29389 2020-02-02 00:00:00.000000 clophfit-0.7.1/docs/_static/lmodel4.png
+-rw-r--r--   0        0        0    23708 2020-02-02 00:00:00.000000 clophfit-0.7.1/docs/_static/lmodel5.png
+-rw-r--r--   0        0        0   187683 2020-02-02 00:00:00.000000 clophfit-0.7.1/docs/_static/lmodel6.png
+-rw-r--r--   0        0        0    24709 2020-02-02 00:00:00.000000 clophfit-0.7.1/docs/_static/lmodel_H04.png
+-rw-r--r--   0        0        0     3195 2020-02-02 00:00:00.000000 clophfit-0.7.1/docs/_static/note_file.png
+-rw-r--r--   0        0        0   101706 2020-02-02 00:00:00.000000 clophfit-0.7.1/docs/_static/r_bs.png
+-rw-r--r--   0        0        0    24754 2020-02-02 00:00:00.000000 clophfit-0.7.1/docs/_static/ratio2P-lmodel1.png
+-rw-r--r--   0        0        0    63411 2020-02-02 00:00:00.000000 clophfit-0.7.1/docs/_static/ratio2P-lmodel2.png
+-rw-r--r--   0        0        0    31838 2020-02-02 00:00:00.000000 clophfit-0.7.1/docs/_static/ratio2P_R1.png
+-rw-r--r--   0        0        0   114443 2020-02-02 00:00:00.000000 clophfit-0.7.1/docs/_static/ratio2P_R2.png
+-rw-r--r--   0        0        0    43555 2020-02-02 00:00:00.000000 clophfit-0.7.1/docs/_static/ratio2P_R3.png
+-rw-r--r--   0        0        0    94094 2020-02-02 00:00:00.000000 clophfit-0.7.1/docs/_static/ratio2P_R4.png
+-rw-r--r--   0        0        0    10140 2020-02-02 00:00:00.000000 clophfit-0.7.1/docs/_static/ratio2P_R5.png
+-rw-r--r--   0        0        0    14971 2020-02-02 00:00:00.000000 clophfit-0.7.1/docs/_static/ratio2P_R6.png
+-rw-r--r--   0        0        0   101706 2020-02-02 00:00:00.000000 clophfit-0.7.1/docs/_static/rpy_bs.png
+-rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 clophfit-0.7.1/docs/api/api.rst
+-rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 clophfit-0.7.1/docs/api/binding.rst
+-rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 clophfit-0.7.1/docs/api/prenspire.rst
+-rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 clophfit-0.7.1/docs/api/prtecan.rst
+-rw-r--r--   0        0        0     1359 2020-02-02 00:00:00.000000 clophfit-0.7.1/docs/references/contributing.rst
+-rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 clophfit-0.7.1/docs/references/description.rst
+-rw-r--r--   0        0        0     3983 2020-02-02 00:00:00.000000 clophfit-0.7.1/docs/references/development.rst
+-rw-r--r--   0        0        0     1851 2020-02-02 00:00:00.000000 clophfit-0.7.1/docs/references/older.rst
+-rw-r--r--   0        0        0      501 2020-02-02 00:00:00.000000 clophfit-0.7.1/docs/references/prenspire.rst
+-rw-r--r--   0        0        0     1015 2020-02-02 00:00:00.000000 clophfit-0.7.1/docs/references/prenspire.uml.rst
+-rw-r--r--   0        0        0     3538 2020-02-02 00:00:00.000000 clophfit-0.7.1/docs/references/prtecan.rst
+-rw-r--r--   0        0        0     2574 2020-02-02 00:00:00.000000 clophfit-0.7.1/docs/references/prtecan.uml.rst
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 clophfit-0.7.1/docs/references/references.rst
+-rw-r--r--   0        0        0   172988 2020-02-02 00:00:00.000000 clophfit-0.7.1/docs/tutorials/prenspire.ipynb
+-rw-r--r--   0        0        0  1959014 2020-02-02 00:00:00.000000 clophfit-0.7.1/docs/tutorials/prtecan.ipynb
+-rw-r--r--   0        0        0      377 2020-02-02 00:00:00.000000 clophfit-0.7.1/docs/tutorials/tutorials.rst
+-rw-r--r--   0        0        0     9075 2020-02-02 00:00:00.000000 clophfit-0.7.1/docs/tutorials/usage.org
+-rw-r--r--   0        0        0    14299 2020-02-02 00:00:00.000000 clophfit-0.7.1/docs/tutorials/usage.rst
+-rw-r--r--   0        0        0    30911 2020-02-02 00:00:00.000000 clophfit-0.7.1/docs/tutorials/usage2.org
+-rw-r--r--   0        0        0    58554 2020-02-02 00:00:00.000000 clophfit-0.7.1/docs/tutorials/usage2.rst
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 clophfit-0.7.1/src/clophfit/__init__.py
+-rw-r--r--   0        0        0     7868 2020-02-02 00:00:00.000000 clophfit-0.7.1/src/clophfit/__main__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 clophfit-0.7.1/src/clophfit/py.typed
+-rw-r--r--   0        0        0      333 2020-02-02 00:00:00.000000 clophfit-0.7.1/src/clophfit/binding/__init__.py
+-rw-r--r--   0        0        0     6321 2020-02-02 00:00:00.000000 clophfit-0.7.1/src/clophfit/binding/fitting.py
+-rwxr-xr-x   0        0        0     1386 2020-02-02 00:00:00.000000 clophfit-0.7.1/src/clophfit/old/dil_buffer.py
+-rwxr-xr-x   0        0        0     1320 2020-02-02 00:00:00.000000 clophfit-0.7.1/src/clophfit/old/dil_correction.py
+-rwxr-xr-x   0        0        0     5639 2020-02-02 00:00:00.000000 clophfit-0.7.1/src/clophfit/old/fit_rpy.py
+-rwxr-xr-x   0        0        0     7936 2020-02-02 00:00:00.000000 clophfit-0.7.1/src/clophfit/old/fit_titration.py
+-rwxr-xr-x   0        0        0     6060 2020-02-02 00:00:00.000000 clophfit-0.7.1/src/clophfit/old/fit_titration_global.py
+-rwxr-xr-x   0        0        0      634 2020-02-02 00:00:00.000000 clophfit-0.7.1/src/clophfit/old/merge.py
+-rwxr-xr-x   0        0        0      891 2020-02-02 00:00:00.000000 clophfit-0.7.1/src/clophfit/old/plot_tecan.py
+-rwxr-xr-x   0        0        0      119 2020-02-02 00:00:00.000000 clophfit-0.7.1/src/clophfit/old/bash/fit.tecan
+-rwxr-xr-x   0        0        0      115 2020-02-02 00:00:00.000000 clophfit-0.7.1/src/clophfit/old/bash/fit.tecan.cl
+-rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 clophfit-0.7.1/src/clophfit/old/bash/new_sort_K.sh
+-rwxr-xr-x   0        0        0      222 2020-02-02 00:00:00.000000 clophfit-0.7.1/src/clophfit/old/bash/sum_all
+-rwxr-xr-x   0        0        0      260 2020-02-02 00:00:00.000000 clophfit-0.7.1/src/clophfit/old/bash/sum_e2
+-rwxr-xr-x   0        0        0      352 2020-02-02 00:00:00.000000 clophfit-0.7.1/src/clophfit/old/bash/sum_lib
+-rwxr-xr-x   0        0        0      427 2020-02-02 00:00:00.000000 clophfit-0.7.1/src/clophfit/old/bash/sum_lib2
+-rwxr-xr-x   0        0        0      260 2020-02-02 00:00:00.000000 clophfit-0.7.1/src/clophfit/old/bash/sum_s202n
+-rwxr-xr-x   0        0        0      260 2020-02-02 00:00:00.000000 clophfit-0.7.1/src/clophfit/old/bash/sum_v224q
+-rwxr-xr-x   0        0        0      572 2020-02-02 00:00:00.000000 clophfit-0.7.1/src/clophfit/old/bash/w_ave.sh
+-rw-r--r--   0        0        0      535 2020-02-02 00:00:00.000000 clophfit-0.7.1/src/clophfit/prenspire/__init__.py
+-rw-r--r--   0        0        0    18269 2020-02-02 00:00:00.000000 clophfit-0.7.1/src/clophfit/prenspire/prenspire.py
+-rw-r--r--   0        0        0     2007 2020-02-02 00:00:00.000000 clophfit-0.7.1/src/clophfit/prtecan/__init__.py
+-rw-r--r--   0        0        0    54541 2020-02-02 00:00:00.000000 clophfit-0.7.1/src/clophfit/prtecan/prtecan.py
+-rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 clophfit-0.7.1/tests/conftest.py
+-rw-r--r--   0        0        0     1261 2020-02-02 00:00:00.000000 clophfit-0.7.1/tests/test_binding.py
+-rw-r--r--   0        0        0     2190 2020-02-02 00:00:00.000000 clophfit-0.7.1/tests/test_cli.py
+-rw-r--r--   0        0        0     5923 2020-02-02 00:00:00.000000 clophfit-0.7.1/tests/test_oldscripts.py
+-rw-r--r--   0        0        0     8247 2020-02-02 00:00:00.000000 clophfit-0.7.1/tests/test_prenspire.py
+-rw-r--r--   0        0        0    26719 2020-02-02 00:00:00.000000 clophfit-0.7.1/tests/test_prtecan.py
+-rw-r--r--   0        0        0    34305 2020-02-02 00:00:00.000000 clophfit-0.7.1/tests/EnSpire/24well_clop0_95.csv
+-rw-r--r--   0        0        0   103231 2020-02-02 00:00:00.000000 clophfit-0.7.1/tests/EnSpire/e2-T-without_sample_column.csv
+-rw-r--r--   0        0        0      812 2020-02-02 00:00:00.000000 clophfit-0.7.1/tests/EnSpire/h148g-spettroC-nota
+-rw-r--r--   0        0        0      737 2020-02-02 00:00:00.000000 clophfit-0.7.1/tests/EnSpire/h148g-spettroC-nota-Err
+-rw-r--r--   0        0        0   373790 2020-02-02 00:00:00.000000 clophfit-0.7.1/tests/EnSpire/h148g-spettroC.csv
+-rw-r--r--   0        0        0    98464 2020-02-02 00:00:00.000000 clophfit-0.7.1/tests/EnSpire/cli/NTT_37C_pKa.csv
+-rw-r--r--   0        0        0    17235 2020-02-02 00:00:00.000000 clophfit-0.7.1/tests/EnSpire/cli/output/NTT_37C_pKa_A.csv
+-rw-r--r--   0        0        0    68449 2020-02-02 00:00:00.000000 clophfit-0.7.1/tests/EnSpire/cli/output/NTT_37C_pKa_A.png
+-rw-r--r--   0        0        0    18266 2020-02-02 00:00:00.000000 clophfit-0.7.1/tests/EnSpire/cli/output/NTT_37C_pKa_B.csv
+-rw-r--r--   0        0        0    53309 2020-02-02 00:00:00.000000 clophfit-0.7.1/tests/EnSpire/cli/output/NTT_37C_pKa_B.png
+-rw-r--r--   0        0        0    13404 2020-02-02 00:00:00.000000 clophfit-0.7.1/tests/EnSpire/exceptions/M1-A6-G12_11columns.csv
+-rw-r--r--   0        0        0    13405 2020-02-02 00:00:00.000000 clophfit-0.7.1/tests/EnSpire/exceptions/M1-A6-G12_missing_emptyline_fin.csv
+-rw-r--r--   0        0        0    13405 2020-02-02 00:00:00.000000 clophfit-0.7.1/tests/EnSpire/exceptions/M1-A6-G12_missing_emptyline_ini.csv
+-rw-r--r--   0        0        0   103682 2020-02-02 00:00:00.000000 clophfit-0.7.1/tests/EnSpire/exceptions/e2dan-emwavelength.csv
+-rw-r--r--   0        0        0   104940 2020-02-02 00:00:00.000000 clophfit-0.7.1/tests/EnSpire/exceptions/e2dan-exwavelength.csv
+-rw-r--r--   0        0        0   104940 2020-02-02 00:00:00.000000 clophfit-0.7.1/tests/EnSpire/exceptions/e2dan-exwavelength2.csv
+-rw-r--r--   0        0        0   104939 2020-02-02 00:00:00.000000 clophfit-0.7.1/tests/EnSpire/exceptions/e2dan-exwavelengthstrange.csv
+-rw-r--r--   0        0        0   344763 2020-02-02 00:00:00.000000 clophfit-0.7.1/tests/EnSpire/exceptions/h148g-spettroC-idx0.csv
+-rw-r--r--   0        0        0   373857 2020-02-02 00:00:00.000000 clophfit-0.7.1/tests/EnSpire/exceptions/h148g-spettroC-idx2.csv
+-rw-r--r--   0        0        0   344941 2020-02-02 00:00:00.000000 clophfit-0.7.1/tests/EnSpire/warnings/h148g-spettroC-incomplete.csv
+-rw-r--r--   0        0        0    12062 2020-02-02 00:00:00.000000 clophfit-0.7.1/tests/Tecan/290212_100.xls
+-rw-r--r--   0        0        0    12073 2020-02-02 00:00:00.000000 clophfit-0.7.1/tests/Tecan/290212_150.xls
+-rw-r--r--   0        0        0    12069 2020-02-02 00:00:00.000000 clophfit-0.7.1/tests/Tecan/290212_20.xls
+-rw-r--r--   0        0        0    13122 2020-02-02 00:00:00.000000 clophfit-0.7.1/tests/Tecan/290212_5.78.xls
+-rw-r--r--   0        0        0    12062 2020-02-02 00:00:00.000000 clophfit-0.7.1/tests/Tecan/290212_50.xls
+-rw-r--r--   0        0        0    13140 2020-02-02 00:00:00.000000 clophfit-0.7.1/tests/Tecan/290212_6.38.xls
+-rw-r--r--   0        0        0    13137 2020-02-02 00:00:00.000000 clophfit-0.7.1/tests/Tecan/290212_6.83.xls
+-rw-r--r--   0        0        0    13146 2020-02-02 00:00:00.000000 clophfit-0.7.1/tests/Tecan/290212_7.24.xls
+-rw-r--r--   0        0        0    13141 2020-02-02 00:00:00.000000 clophfit-0.7.1/tests/Tecan/290212_7.67.xls
+-rw-r--r--   0        0        0    13173 2020-02-02 00:00:00.000000 clophfit-0.7.1/tests/Tecan/290212_8.23.xls
+-rw-r--r--   0        0        0    13171 2020-02-02 00:00:00.000000 clophfit-0.7.1/tests/Tecan/290212_8.82.xls
+-rw-r--r--   0        0        0    13152 2020-02-02 00:00:00.000000 clophfit-0.7.1/tests/Tecan/290212_9.31.xls
+-rw-r--r--   0        0        0    12930 2020-02-02 00:00:00.000000 clophfit-0.7.1/tests/Tecan/290513_5.5.xls
+-rw-r--r--   0        0        0    11262 2020-02-02 00:00:00.000000 clophfit-0.7.1/tests/Tecan/290513_5.5_bad.xls
+-rw-r--r--   0        0        0    12946 2020-02-02 00:00:00.000000 clophfit-0.7.1/tests/Tecan/290513_7.2.xls
+-rw-r--r--   0        0        0    12975 2020-02-02 00:00:00.000000 clophfit-0.7.1/tests/Tecan/290513_8.8.xls
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 clophfit-0.7.1/tests/Tecan/list.cl
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 clophfit-0.7.1/tests/Tecan/list.cl20
+-rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 clophfit-0.7.1/tests/Tecan/list.pH
+-rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 clophfit-0.7.1/tests/Tecan/list.pH2
+-rw-r--r--   0        0        0    14438 2020-02-02 00:00:00.000000 clophfit-0.7.1/tests/Tecan/140220/200214 pH data.ods
+-rw-r--r--   0        0        0    12835 2020-02-02 00:00:00.000000 clophfit-0.7.1/tests/Tecan/140220/NaCl1_200214.xls
+-rw-r--r--   0        0        0    12812 2020-02-02 00:00:00.000000 clophfit-0.7.1/tests/Tecan/140220/NaCl2_200214.xls
+-rw-r--r--   0        0        0    12802 2020-02-02 00:00:00.000000 clophfit-0.7.1/tests/Tecan/140220/NaCl3_200214.xls
+-rw-r--r--   0        0        0    12799 2020-02-02 00:00:00.000000 clophfit-0.7.1/tests/Tecan/140220/NaCl4_200214.xls
+-rw-r--r--   0        0        0    12812 2020-02-02 00:00:00.000000 clophfit-0.7.1/tests/Tecan/140220/NaCl5_200214.xls
+-rw-r--r--   0        0        0    12773 2020-02-02 00:00:00.000000 clophfit-0.7.1/tests/Tecan/140220/NaCl6_200214.xls
+-rw-r--r--   0        0        0    12783 2020-02-02 00:00:00.000000 clophfit-0.7.1/tests/Tecan/140220/NaCl7_200214.xls
+-rw-r--r--   0        0        0    12790 2020-02-02 00:00:00.000000 clophfit-0.7.1/tests/Tecan/140220/NaCl8_200214.xls
+-rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 clophfit-0.7.1/tests/Tecan/140220/additions.cl
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 clophfit-0.7.1/tests/Tecan/140220/additions.pH
+-rw-r--r--   0        0        0    21877 2020-02-02 00:00:00.000000 clophfit-0.7.1/tests/Tecan/140220/fit0-1.csv
+-rw-r--r--   0        0        0    21592 2020-02-02 00:00:00.000000 clophfit-0.7.1/tests/Tecan/140220/fit0.csv
+-rw-r--r--   0        0        0    23056 2020-02-02 00:00:00.000000 clophfit-0.7.1/tests/Tecan/140220/fit1-1.csv
+-rw-r--r--   0        0        0    23182 2020-02-02 00:00:00.000000 clophfit-0.7.1/tests/Tecan/140220/fit1.csv
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 clophfit-0.7.1/tests/Tecan/140220/list.cl
+-rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 clophfit-0.7.1/tests/Tecan/140220/list.pH
+-rw-r--r--   0        0        0    12865 2020-02-02 00:00:00.000000 clophfit-0.7.1/tests/Tecan/140220/pH5.0_200214.xls
+-rw-r--r--   0        0        0    12901 2020-02-02 00:00:00.000000 clophfit-0.7.1/tests/Tecan/140220/pH5.8_200214.xls
+-rw-r--r--   0        0        0    12889 2020-02-02 00:00:00.000000 clophfit-0.7.1/tests/Tecan/140220/pH6.5_200214.xls
+-rw-r--r--   0        0        0    12914 2020-02-02 00:00:00.000000 clophfit-0.7.1/tests/Tecan/140220/pH7.1_200214.xls
+-rw-r--r--   0        0        0    12934 2020-02-02 00:00:00.000000 clophfit-0.7.1/tests/Tecan/140220/pH7.6_200214.xls
+-rw-r--r--   0        0        0    12939 2020-02-02 00:00:00.000000 clophfit-0.7.1/tests/Tecan/140220/pH8.3_200214.xls
+-rw-r--r--   0        0        0    12937 2020-02-02 00:00:00.000000 clophfit-0.7.1/tests/Tecan/140220/pH9.1_200214.xls
+-rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 clophfit-0.7.1/tests/Tecan/140220/scheme.txt
+-rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 clophfit-0.7.1/tests/Tecan/140220/scheme0.txt
+-rw-r--r--   0        0        0     9176 2020-02-02 00:00:00.000000 clophfit-0.7.1/tests/Tecan/exceptions/0_Labelblocks_290513_5.5.xlsx
+-rw-r--r--   0        0        0    12275 2020-02-02 00:00:00.000000 clophfit-0.7.1/tests/Tecan/exceptions/290212_7.67_repeated_lb.xls
+-rw-r--r--   0        0        0    10209 2020-02-02 00:00:00.000000 clophfit-0.7.1/tests/Tecan/exceptions/84wells_290212_20.xlsx
+-rw-r--r--   0        0        0    10431 2020-02-02 00:00:00.000000 clophfit-0.7.1/tests/Tecan/exceptions/88wells_290212_20.xlsx
+-rw-r--r--   0        0        0      525 2020-02-02 00:00:00.000000 clophfit-0.7.1/tests/data/A01-20140311a.dat
+-rw-r--r--   0        0        0      525 2020-02-02 00:00:00.000000 clophfit-0.7.1/tests/data/A01.dat
+-rw-r--r--   0        0        0      508 2020-02-02 00:00:00.000000 clophfit-0.7.1/tests/data/A11.dat
+-rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 clophfit-0.7.1/tests/data/B01.dat
+-rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 clophfit-0.7.1/tests/data/H04.dat
+-rw-r--r--   0        0        0      537 2020-02-02 00:00:00.000000 clophfit-0.7.1/tests/data/NTT-A04-Cl_note
+-rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 clophfit-0.7.1/tests/data/copyIP.txt
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 clophfit-0.7.1/tests/data/ratio2P.txt
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 clophfit-0.7.1/tests/data/w.txt
+-rw-r--r--   0        0        0    43486 2020-02-02 00:00:00.000000 clophfit-0.7.1/tests/data/Meas/A04 Cl_A.csv
+-rw-r--r--   0        0        0   138192 2020-02-02 00:00:00.000000 clophfit-0.7.1/tests/data/Meas/A04 Cl_A.png
+-rw-r--r--   0        0        0    29087 2020-02-02 00:00:00.000000 clophfit-0.7.1/tests/data/Meas/A04 Cl_B.csv
+-rw-r--r--   0        0        0    97762 2020-02-02 00:00:00.000000 clophfit-0.7.1/tests/data/Meas/A04 Cl_B.png
+-rw-r--r--   0        0        0    35910 2020-02-02 00:00:00.000000 clophfit-0.7.1/tests/data/Meas/A04 Cl_C.csv
+-rw-r--r--   0        0        0   138239 2020-02-02 00:00:00.000000 clophfit-0.7.1/tests/data/Meas/A04 Cl_C.png
+-rw-r--r--   0        0        0    29248 2020-02-02 00:00:00.000000 clophfit-0.7.1/tests/data/Meas/A04 Cl_D.csv
+-rw-r--r--   0        0        0    84749 2020-02-02 00:00:00.000000 clophfit-0.7.1/tests/data/Meas/A04 Cl_D.png
+-rw-r--r--   0        0        0    35312 2020-02-02 00:00:00.000000 clophfit-0.7.1/tests/data/Meas/A04 Cl_E.csv
+-rw-r--r--   0        0        0   145114 2020-02-02 00:00:00.000000 clophfit-0.7.1/tests/data/Meas/A04 Cl_E.png
+-rw-r--r--   0        0        0    43756 2020-02-02 00:00:00.000000 clophfit-0.7.1/tests/data/Meas/A04 Cl_F.csv
+-rw-r--r--   0        0        0   126442 2020-02-02 00:00:00.000000 clophfit-0.7.1/tests/data/Meas/A04 Cl_F.png
+-rw-r--r--   0        0        0      508 2020-02-02 00:00:00.000000 clophfit-0.7.1/tests/data/global/Cl/A11-failed.dat
+-rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 clophfit-0.7.1/tests/data/global/Cl/B05-20130628-cor.dat
+-rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 clophfit-0.7.1/tests/data/global/pH/B01-failed.dat
+-rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 clophfit-0.7.1/tests/data/global/pH/D05.dat
+-rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 clophfit-0.7.1/tests/data/global/pH/H04-with_nan.dat
+-rw-r--r--   0        0        0   235947 2020-02-02 00:00:00.000000 clophfit-0.7.1/tests/data/k/D05.dat-bs.png
+-rw-r--r--   0        0        0    28093 2020-02-02 00:00:00.000000 clophfit-0.7.1/tests/data/k/D05.dat.png
+-rw-r--r--   0        0        0    12506 2020-02-02 00:00:00.000000 clophfit-0.7.1/tests/data/output/band_A04 Cl_A_NTT-A04-Cl_note.pdf
+-rw-r--r--   0        0        0    12433 2020-02-02 00:00:00.000000 clophfit-0.7.1/tests/data/output/band_A04 Cl_B_NTT-A04-Cl_note.pdf
+-rw-r--r--   0        0        0    66713 2020-02-02 00:00:00.000000 clophfit-0.7.1/tests/data/output/svd_A04 Cl_A_NTT-A04-Cl_note.pdf
+-rw-r--r--   0        0        0    39832 2020-02-02 00:00:00.000000 clophfit-0.7.1/tests/data/output/svd_A04 Cl_B_NTT-A04-Cl_note.pdf
+-rw-r--r--   0        0        0    32564 2020-02-02 00:00:00.000000 clophfit-0.7.1/tests/data/output/global/Cl/B05-20130628-cor.dat.png
+-rw-r--r--   0        0        0    36956 2020-02-02 00:00:00.000000 clophfit-0.7.1/tests/data/output/global/pH/D05.dat.png
+-rw-r--r--   0        0        0      821 2020-02-02 00:00:00.000000 clophfit-0.7.1/.gitignore
+-rw-r--r--   0        0        0     1480 2020-02-02 00:00:00.000000 clophfit-0.7.1/LICENSE.txt
+-rw-r--r--   0        0        0     3462 2020-02-02 00:00:00.000000 clophfit-0.7.1/README.md
+-rw-r--r--   0        0        0    11259 2020-02-02 00:00:00.000000 clophfit-0.7.1/pyproject.toml
+-rw-r--r--   0        0        0     6253 2020-02-02 00:00:00.000000 clophfit-0.7.1/PKG-INFO
```

### Comparing `clophfit-0.7.0/.pre-commit-config.yaml` & `clophfit-0.7.1/.pre-commit-config.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -27,23 +27,23 @@
         args: [--pytest-test-first]
       - id: requirements-txt-fixer
       - id: detect-private-key
       - id: trailing-whitespace # hyper
         exclude: "^tests/EnSpire/"
 
   - repo: https://github.com/macisamuele/language-formatters-pre-commit-hooks
-    rev: v2.8.0
+    rev: v2.9.0
     hooks:
       - id: pretty-format-ini
         args: [--autofix]
       - id: pretty-format-toml
         args: [--autofix]
 
   - repo: https://github.com/charliermarsh/ruff-pre-commit
-    rev: v0.0.265
+    rev: v0.0.267
     hooks:
       - id: ruff
         # args: [--exclude, "src/clophfit/prenspire/*"]
 
   - repo: https://github.com/psf/black
     rev: 23.3.0
     hooks:
@@ -97,12 +97,12 @@
   - repo: https://github.com/shellcheck-py/shellcheck-py
     rev: v0.9.0.2
     hooks:
       - id: shellcheck
         args: [-x]
 
   - repo: https://github.com/commitizen-tools/commitizen
-    rev: 3.2.1
+    rev: 3.2.2
     hooks:
       - id: commitizen
       - id: commitizen-branch
         stages: [push]
```

### Comparing `clophfit-0.7.0/CHANGELOG.md` & `clophfit-0.7.1/CHANGELOG.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,34 @@
 <!-- markdownlint-disable MD024 -->
 <!-- vale write-good.TooWordy = NO -->
 
 # Changelog
 
+## v0.7.1 (2023-05-18)
+
+### Fix
+
+- **docs**: README links to pages
+
+### Docs
+
+- Enhance the alignment between the changelog and tags
+
+### Build
+
+- bump codecov/codecov-action from 3.1.3 to 3.1.4 (#262)
+
+### Refactor
+
+- **enspire**: Adopt dataclass with helper functions
+
+### chore
+
+- update pre-commit hooks (#261)
+
 ## v0.7.0 (2023-05-15)
 
 ### Feat
 
 - **prtecan**: Typecheck PlateScheme and improve docs
 
 ### Test
@@ -438,32 +460,32 @@
 ### Refactor
 
 - Removed temperatures attribute as already present in metadata.
 - Slightly improved design for TecanfilesGroup(List[Tecanfile]).
 - Prototyped NormalizedLabelblock class.
 - Removed of os.path in favor of pathlib.Path
 
-## 0.3.8 (2022-09-24)
+## v0.3.8 (2022-09-24)
 
 ### Fix
 
 - missing xlrd issue.
 
-## 0.3.7 (2022-09-23)
+## v0.3.7 (2022-09-23)
 
 ### Fix
 
 - `clop prtecan` Install from pipx.
 
 ### Refactor
 
 - Path and str are mixing.
 - tests do not use os.chdir() anymore.
 
-## 0.3.6 (2022-09-21)
+## v0.3.6 (2022-09-21)
 
 ### Feat
 
 - [docs] Add click-sphinx.
 
 ### Fix
 
@@ -474,68 +496,87 @@
 
 - dataclasses in prtecan.
 - string normalization to black default.
 - [ci] isort and pyupgrade from pre-commit.
 - [ci] safety.
 - [docs] README.md and CHANGELOG.md.
 
-## 0.3.5 (2022-09-07)
+## v0.3.5 (2022-09-11)
+
+### Changed
+
+- Update poetry 1.2.0 and notebook.
+
+## v0.3.4 (2022-09-07)
 
 ### Fixed
 
 - Python deps \"\>3.8, \<3.11\" in pyproject.
 
 ### Changed
 
 - Update poetry 1.2.0 and notebook.
 
-## 0.3.4 (2022-03-14)
+## v0.3.3 (2022-05-27)
+
+- Update deps for notebooks.
+
+## v0.3.2 (2022-03-15)
+
+- Add zenodo.
+
+## v0.3.1 (2022-03-14)
 
 ### Fixed
 
-- Read the docs.
-- Removed :math: directive from README.rst.
+- Removed :math: directive from README.rst and plantuml.
+
+## v0.3.0 (2022-03-14)
+
+### Fixed
+
+- warning for keys_unk set used as index in pd.
 
 ### Added
 
 - Tecan file parser.
+- Import fit_titrations scripts with many test data.
 - usage.org (exported to .rst) serves as tutorial in docs and includes:
   - liaisan-data
   - new-bootstrap
   - lmfit global
   - emcee (extremely slow)
 - command `clop`.
+- (docs) usage.org.
+- Adopt pre-commit, poetry and nox.
 - <https://pypi.org/project/readme-renderer/> in lint.
+- (build) Github actions.
 
 ### Changed
 
 - Update to python 3.9 and 3.10.
 - Update dependencies:
 
       poetry show --outdated
 
   with required minor changes in old scripts.
 
 - nox-poetry.
 - pandas.rpy (\<=0.19) now lives in rpy2.
 
-### Fixed
-
-- warning for keys_unk set used as index in pd.
-
-## 0.2.1 (2021-11-18)
+## v0.2.1 (2021-11-18)
 
 - Update to python 3.6.
 - Py.test for:
   - `fit_titration.py`
   - `fit_titration_global.py`
 - lmfit==0.8.3 to prevent `fit-titration_global.py` to fail.
 - [\_tmpoutput]{.title-ref} is not deleted; watch out for false positive.
 
-## 0.2.0 (2021-11-14)
+## v0.2.0 (2021-11-14)
 
 - Reference for running older scripts; reproducibility thanks to
   [Poetry](https://python-poetry.org) and
   [Pyenv](https://github.com/pyenv/pyenv):
 
       LDFLAGS=-L/usr/lib/openssl-1.0/ CFLAGS=-I/usr/include/openssl-1.0/ \
         pyenv install 3.4.10
```

### Comparing `clophfit-0.7.0/cz_customize_info.txt` & `clophfit-0.7.1/cz_customize_info.txt`

 * *Files identical despite different names*

### Comparing `clophfit-0.7.0/.github/workflows/ci.yml` & `clophfit-0.7.1/.github/workflows/ci.yml`

 * *Files 0% similar despite different names*

```diff
@@ -138,15 +138,15 @@
           name: coverage-data
       - name: Create coverage report
         run: |
           hatch run coverage:combine
           hatch run coverage:report
           hatch run coverage:xml
       - name: Upload coverage report
-        uses: codecov/codecov-action@v3.1.3
+        uses: codecov/codecov-action@v3.1.4
 
   testpypi:
     needs: [pre-commit, typeguard, checks, tests, coverage]
     runs-on: ubuntu-latest
     if: "startsWith(github.event.head_commit.message, 'bump:')"
     outputs:
       version: ${{ steps.version.outputs.ver }}
```

### Comparing `clophfit-0.7.0/.github/workflows/docs.yml` & `clophfit-0.7.1/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `clophfit-0.7.0/docs/Makefile` & `clophfit-0.7.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `clophfit-0.7.0/docs/conf.py` & `clophfit-0.7.1/docs/conf.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 
 # -- Project information -----------------------------------------------------
 
 project = "ClopHfit"
 copyright = "2023, Daniele Arosio"  # noqa: A001
 author = "Daniele Arosio"
-release = "0.7.0"
+release = "0.7.1"
 html_title = "ClopHfit"
 
 # -- General configuration ---------------------------------------------------
 
 # Add any Sphinx extension module names here, as strings. They can be
 # extensions coming with Sphinx (named 'sphinx.ext.*') or your custom
 # ones.
```

### Comparing `clophfit-0.7.0/docs/index.rst` & `clophfit-0.7.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `clophfit-0.7.0/docs/make.bat` & `clophfit-0.7.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `clophfit-0.7.0/docs/_static/bs_pd_f1.png` & `clophfit-0.7.1/docs/_static/bs_pd_f1.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.7.0/docs/_static/bs_pd_f2.png` & `clophfit-0.7.1/docs/_static/bs_pd_f2.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.7.0/docs/_static/bs_pd_f3.png` & `clophfit-0.7.1/docs/_static/bs_pd_f3.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.7.0/docs/_static/bs_pd_f4.png` & `clophfit-0.7.1/docs/_static/bs_pd_f4.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.7.0/docs/_static/bs_pd_f5.png` & `clophfit-0.7.1/docs/_static/bs_pd_f5.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.7.0/docs/_static/bs_pd_f6.png` & `clophfit-0.7.1/docs/_static/bs_pd_f6.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.7.0/docs/_static/bs_pd_f7.png` & `clophfit-0.7.1/docs/_static/bs_pd_f7.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.7.0/docs/_static/csvtable.png` & `clophfit-0.7.1/docs/_static/csvtable.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.7.0/docs/_static/emcee-01.png` & `clophfit-0.7.1/docs/_static/emcee-01.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.7.0/docs/_static/emcee-02.png` & `clophfit-0.7.1/docs/_static/emcee-02.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.7.0/docs/_static/emcee-11.png` & `clophfit-0.7.1/docs/_static/emcee-11.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.7.0/docs/_static/emcee-12.png` & `clophfit-0.7.1/docs/_static/emcee-12.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.7.0/docs/_static/f01.png` & `clophfit-0.7.1/docs/_static/f01.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.7.0/docs/_static/file.png` & `clophfit-0.7.1/docs/_static/file.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.7.0/docs/_static/gR_fit1.png` & `clophfit-0.7.1/docs/_static/gR_fit1.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.7.0/docs/_static/gR_fit2.png` & `clophfit-0.7.1/docs/_static/gR_fit2.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.7.0/docs/_static/gR_fit3.png` & `clophfit-0.7.1/docs/_static/gR_fit3.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.7.0/docs/_static/gR_fit4.png` & `clophfit-0.7.1/docs/_static/gR_fit4.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.7.0/docs/_static/gR_fit5.png` & `clophfit-0.7.1/docs/_static/gR_fit5.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.7.0/docs/_static/gR_fit6.png` & `clophfit-0.7.1/docs/_static/gR_fit6.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.7.0/docs/_static/gR_fit7.png` & `clophfit-0.7.1/docs/_static/gR_fit7.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.7.0/docs/_static/glmfit0.png` & `clophfit-0.7.1/docs/_static/glmfit0.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.7.0/docs/_static/glmfit1.png` & `clophfit-0.7.1/docs/_static/glmfit1.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.7.0/docs/_static/glmfit2.png` & `clophfit-0.7.1/docs/_static/glmfit2.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.7.0/docs/_static/glmfit3.png` & `clophfit-0.7.1/docs/_static/glmfit3.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.7.0/docs/_static/glmfit_np.r_.png` & `clophfit-0.7.1/docs/_static/glmfit_np.r_.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.7.0/docs/_static/lmfit1.png` & `clophfit-0.7.1/docs/_static/lmfit1.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.7.0/docs/_static/lmfit2.png` & `clophfit-0.7.1/docs/_static/lmfit2.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.7.0/docs/_static/lmfit3.png` & `clophfit-0.7.1/docs/_static/lmfit3.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.7.0/docs/_static/lmfit4.png` & `clophfit-0.7.1/docs/_static/lmfit4.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.7.0/docs/_static/lmfit5.png` & `clophfit-0.7.1/docs/_static/lmfit5.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.7.0/docs/_static/lmodel1.png` & `clophfit-0.7.1/docs/_static/lmodel1.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.7.0/docs/_static/lmodel2.png` & `clophfit-0.7.1/docs/_static/lmodel2.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.7.0/docs/_static/lmodel3.png` & `clophfit-0.7.1/docs/_static/lmodel3.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.7.0/docs/_static/lmodel4.png` & `clophfit-0.7.1/docs/_static/lmodel4.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.7.0/docs/_static/lmodel5.png` & `clophfit-0.7.1/docs/_static/lmodel5.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.7.0/docs/_static/lmodel6.png` & `clophfit-0.7.1/docs/_static/lmodel6.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.7.0/docs/_static/lmodel_H04.png` & `clophfit-0.7.1/docs/_static/lmodel_H04.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.7.0/docs/_static/note_file.png` & `clophfit-0.7.1/docs/_static/note_file.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.7.0/docs/_static/r_bs.png` & `clophfit-0.7.1/docs/_static/r_bs.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.7.0/docs/_static/ratio2P-lmodel1.png` & `clophfit-0.7.1/docs/_static/ratio2P-lmodel1.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.7.0/docs/_static/ratio2P-lmodel2.png` & `clophfit-0.7.1/docs/_static/ratio2P-lmodel2.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.7.0/docs/_static/ratio2P_R1.png` & `clophfit-0.7.1/docs/_static/ratio2P_R1.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.7.0/docs/_static/ratio2P_R2.png` & `clophfit-0.7.1/docs/_static/ratio2P_R2.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.7.0/docs/_static/ratio2P_R3.png` & `clophfit-0.7.1/docs/_static/ratio2P_R3.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.7.0/docs/_static/ratio2P_R4.png` & `clophfit-0.7.1/docs/_static/ratio2P_R4.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.7.0/docs/_static/ratio2P_R5.png` & `clophfit-0.7.1/docs/_static/ratio2P_R5.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.7.0/docs/_static/ratio2P_R6.png` & `clophfit-0.7.1/docs/_static/ratio2P_R6.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.7.0/docs/_static/rpy_bs.png` & `clophfit-0.7.1/docs/_static/rpy_bs.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.7.0/docs/references/contributing.rst` & `clophfit-0.7.1/docs/references/contributing.rst`

 * *Files identical despite different names*

### Comparing `clophfit-0.7.0/docs/references/development.rst` & `clophfit-0.7.1/docs/references/development.rst`

 * *Files identical despite different names*

### Comparing `clophfit-0.7.0/docs/references/older.rst` & `clophfit-0.7.1/docs/references/older.rst`

 * *Files identical despite different names*

### Comparing `clophfit-0.7.0/docs/references/prtecan.rst` & `clophfit-0.7.1/docs/references/prtecan.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-prtecan parser
-~~~~~~~~~~~~~~
+prtecan
+~~~~~~~
 
 **Tecan** file has the following structure.
 
 	+------------+
 	|  metadata  |
 	+------------+
 	|  label 1   |
```

### Comparing `clophfit-0.7.0/docs/references/prtecan.uml.rst` & `clophfit-0.7.1/docs/references/prtecan.uml.rst`

 * *Files identical despite different names*

### Comparing `clophfit-0.7.0/docs/tutorials/prenspire.ipynb` & `clophfit-0.7.1/docs/tutorials/prenspire.ipynb`

 * *Files 3% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.971956559065934%*

 * *Differences: {"'cells'": '{3: {\'outputs\': {0: {\'data\': {\'text/plain\': ["([\'A03\', \'A04\', \'A05\', '*

 * *            '\'A06\', \'B01\', \'B02\', \'C01\', \'C02\', \'C03\'],\\n", " [\'A03\', \'A04\', '*

 * *            '\'A05\', \'A06\', \'B01\', \'B02\', \'C01\', \'C02\', \'C03\'],\\n", " [[\'A\', \'  '*

 * *            '\', \'  \', \'- \', \'- \', \'- \', \'- \'],\\n", "  [\'B\', \'- \', \'- \', \'  \', '*

 * *            '\'  \', \'  \', \'  \'],\\n", "  [\'C\', \'- \', \'- \', \'- \', \'  \', \'  \', \'  '*

 * *            '\'],\\n" […]*

```diff
@@ -37,125 +37,63 @@
             "cell_type": "code",
             "execution_count": 3,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
-                            "[['A', '  ', '  ', '- ', '- ', '- ', '- '],\n",
-                            " ['B', '- ', '- ', '  ', '  ', '  ', '  '],\n",
-                            " ['C', '- ', '- ', '- ', '  ', '  ', '  '],\n",
-                            " ['D', '  ', '  ', '  ', '  ', '  ', '  ']]"
+                            "(['A03', 'A04', 'A05', 'A06', 'B01', 'B02', 'C01', 'C02', 'C03'],\n",
+                            " ['A03', 'A04', 'A05', 'A06', 'B01', 'B02', 'C01', 'C02', 'C03'],\n",
+                            " [['A', '  ', '  ', '- ', '- ', '- ', '- '],\n",
+                            "  ['B', '- ', '- ', '  ', '  ', '  ', '  '],\n",
+                            "  ['C', '- ', '- ', '- ', '  ', '  ', '  '],\n",
+                            "  ['D', '  ', '  ', '  ', '  ', '  ', '  ']])"
                         ]
                     },
                     "execution_count": 3,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
-                "ef3._platemap"
+                "ef3.wells, ef3._wells_platemap, ef3._platemap"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 4,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
-                            "(['A03', 'A04', 'A05', 'A06', 'B01', 'B02', 'C01', 'C02', 'C03'],\n",
-                            " ['A03', 'A04', 'A05', 'A06', 'B01', 'B02', 'C01', 'C02', 'C03'])"
+                            "dict_keys(['file', 'verbose', 'metadata', 'measurements', 'wells', '_ini', '_fin', '_wells_platemap', '_platemap'])"
                         ]
                     },
                     "execution_count": 4,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
-                "ef3.extract_measurements()\n",
-                "ef3.wells, ef3._well_list_platemap"
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": 5,
-            "metadata": {},
-            "outputs": [
-                {
-                    "data": {
-                        "text/plain": [
-                            "dict_keys(['_ini', '_fin', '_data_list', '_metadata_post', '_well_list_platemap', '_platemap', 'metadata', '_filename'])"
-                        ]
-                    },
-                    "execution_count": 5,
-                    "metadata": {},
-                    "output_type": "execute_result"
-                }
-            ],
-            "source": [
                 "ef1.__dict__.keys()"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 6,
-            "metadata": {},
-            "outputs": [
-                {
-                    "data": {
-                        "text/plain": [
-                            "dict_keys(['_ini', '_fin', '_data_list', '_metadata_post', '_well_list_platemap', '_platemap', 'metadata', '_filename', 'measurements', 'wells'])"
-                        ]
-                    },
-                    "execution_count": 6,
-                    "metadata": {},
-                    "output_type": "execute_result"
-                }
-            ],
-            "source": [
-                "ef1.extract_measurements()\n",
-                "ef1.__dict__.keys()"
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": 7,
-            "metadata": {},
-            "outputs": [
-                {
-                    "data": {
-                        "text/plain": [
-                            "['F01', 'F02', 'F03', 'F04', 'F05', 'F06', 'F07']"
-                        ]
-                    },
-                    "execution_count": 7,
-                    "metadata": {},
-                    "output_type": "execute_result"
-                }
-            ],
-            "source": [
-                "ef2.extract_measurements()\n",
-                "ef2.wells"
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": 8,
+            "execution_count": 5,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "(dict_keys(['A']), dict_keys(['B', 'A', 'C', 'D', 'E', 'F', 'G', 'H']))"
                         ]
                     },
-                    "execution_count": 8,
+                    "execution_count": 5,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "ef1.measurements.keys(), ef2.measurements.keys()"
             ]
@@ -165,15 +103,15 @@
             "metadata": {},
             "source": [
                 "when testing each spectra for the presence of a single wavelength in the appropriate monochromator"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 9,
+            "execution_count": 6,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "{'temp': '25',\n",
                             " 'Monochromator': 'Excitation',\n",
@@ -183,254 +121,242 @@
                             " 'Using of excitation filter': 'Top',\n",
                             " 'Measurement height': '8.9',\n",
                             " 'Number of flashes': '50',\n",
                             " 'Number of flashes integrated': '50',\n",
                             " 'Flash power': '100'}"
                         ]
                     },
-                    "execution_count": 9,
+                    "execution_count": 6,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "ef2.measurements[\"A\"][\"metadata\"]"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 10,
+            "execution_count": 7,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
-                            "['Well',\n",
-                            " 'MeasB:WavelengthEms',\n",
-                            " 'MeasA:WavelengthExc',\n",
-                            " 'MeasA:Result',\n",
-                            " 'MeasC:WavelengthEms',\n",
-                            " 'MeasD:WavelengthExc',\n",
-                            " 'MeasD:Result',\n",
-                            " 'MeasE:WavelengthEms',\n",
-                            " 'MeasF:WavelengthExc',\n",
-                            " 'MeasF:Result',\n",
-                            " 'MeasG:WavelengthEms',\n",
-                            " 'MeasH:WavelengthExc',\n",
-                            " 'MeasH:Result']"
+                            "dict_keys(['metadata', 'lambda', 'F01', 'F02', 'F03', 'F04', 'F05', 'F06', 'F07'])"
                         ]
                     },
-                    "execution_count": 10,
+                    "execution_count": 7,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
-                "ef2._data_list[0][::2]"
+                "ef2.measurements[\"A\"].keys()"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 11,
+            "execution_count": 8,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "[2163.0, 607.0, 1846.0, 517.0, 572.0, 2145.0, 2028.0]"
                         ]
                     },
-                    "execution_count": 11,
+                    "execution_count": 8,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "random.seed(11)\n",
                 "random.sample(ef1.measurements[\"A\"][\"F01\"], 7)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 12,
+            "execution_count": 9,
             "metadata": {},
             "outputs": [],
             "source": [
                 "en1 = prenspire.ExpNote(tpath / \"h148g-spettroC-nota\")"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 13,
+            "execution_count": 10,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "['A01', 'A02', 'A03', 'A04', 'A05', 'A06', 'A07']"
                         ]
                     },
-                    "execution_count": 13,
+                    "execution_count": 10,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "en1.wells[:7]"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 14,
+            "execution_count": 11,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "[['Well', 'pH', 'Chloride'],\n",
                             " ['A01', '5.2', '0'],\n",
                             " ['A02', '5.2', '6.7'],\n",
                             " ['A03', '5.2', '13.3'],\n",
                             " ['A04', '5.2', '26.7']]"
                         ]
                     },
-                    "execution_count": 14,
+                    "execution_count": 11,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
-                "en1.note_list[:5]"
+                "en1._note_list[:5]"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 15,
+            "execution_count": 12,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "(True, False)"
                         ]
                     },
-                    "execution_count": 15,
+                    "execution_count": 12,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
-                "en1.check_wells(ef1), en1.check_wells(ef2)"
+                "en1.wells == ef1.wells, en1.wells == ef2.wells"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 16,
+            "execution_count": 13,
             "metadata": {},
             "outputs": [],
             "source": [
                 "en1.build_titrations(ef1)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 17,
+            "execution_count": 14,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
-                            "dict_keys(['note_list', 'wells', 'titrations', 'pH_values'])"
+                            "dict_keys(['note_file', 'verbose', 'wells', '_note_list', 'titrations', 'pH_values'])"
                         ]
                     },
-                    "execution_count": 17,
+                    "execution_count": 14,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "en1.__dict__.keys()"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 18,
+            "execution_count": 15,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "['5.2', '6.3', '7.4', '8.1', '8.2']"
                         ]
                     },
-                    "execution_count": 18,
+                    "execution_count": 15,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "en1.pH_values"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 19,
+            "execution_count": 16,
             "metadata": {},
             "outputs": [],
             "source": [
                 "tit0 = en1.titrations[0]\n",
                 "tit3 = en1.titrations[3]"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 20,
+            "execution_count": 17,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "dict_keys(['conc', 'data', 'cl'])"
                         ]
                     },
-                    "execution_count": 20,
+                    "execution_count": 17,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "tit0.__dict__.keys()"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 21,
+            "execution_count": 18,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "([5.2, 6.3, 7.4, 8.1, 8.2],\n",
                             " '0',\n",
                             " [0.0, 6.7, 13.3, 26.7, 40.0, 60.0, 87.0, 120.0, 267.0, 400.0, 667.0],\n",
                             " '7.4')"
                         ]
                     },
-                    "execution_count": 21,
+                    "execution_count": 18,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "tit0.conc, tit0.cl, tit3.conc, tit3.ph"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 22,
+            "execution_count": 19,
             "metadata": {
                 "scrolled": true
             },
             "outputs": [
                 {
                     "data": {
                         "text/html": [
@@ -588,26 +514,26 @@
                             "498.0    632.0  4900.0  46725.0  93452.0   94101.0\n",
                             "499.0    854.0  5140.0  48452.0  96643.0   97506.0\n",
                             "500.0    573.0  5573.0  50025.0  99847.0  100715.0\n",
                             "\n",
                             "[229 rows x 5 columns]"
                         ]
                     },
-                    "execution_count": 22,
+                    "execution_count": 19,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "tit0.data[\"A\"]"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 23,
+            "execution_count": 20,
             "metadata": {
                 "scrolled": false
             },
             "outputs": [
                 {
                     "data": {
                         "image/png": "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pp7wXIMHD2bu3Lns2rWLJUuWoJRi3LhxuFyuRmUKDg7m0KFDHDp0iC1btpCamsrVV19NRkaGp83zzz/Pa6+9xttvv826desICAggNTWV2tpaT5u6ujquuuoq7rzzzuP2NXXqVN566y2cTmejMgohhGicgoz6GaWDqnMwDxygbZjjUeK4LBaLApTFYjlqn81mUzt37lQ2m02DZKfns88+U1FRUV7bysrKlNlsVj/99NNpnXvr1q0KUPv27WvwMXPnzlUhISFe21wul/Lx8VELFixQSinldrtVbGyseuGFFzxtKioqlMlkUh9//HGDznmY3W5XJpPphO+1Lf98hRCitZg38yf1+h3L1Lqr727Rfk/0+X0kuSLUlJSCuhptXko1OOaqVasYPNj7EuXSpUtxu93k5eXRq1cvOnbsyNVXX01ubm6Dz1tTU8PcuXNJSko6rYVcXS4X77//PgCDBg0C6lexLygo8ForLCQkhGHDhrF27dpGnd/X15cBAwawatWqU84ohBDixGzVdVRb6wdHx/WO0zjN8cmiq03JYYVn4rXp+6F88A1oUNPs7Gzi471zHjhwALfbzTPPPMOrr75KSEgIjzzyCBdeeCHbtm3D19f3uOd78803uf/++6mpqaFnz54sXbr0hO2PxWKxEBgYCIDNZsPHx4d33nmHrl27AlBQUABATEyM13ExMTGefY0RHx9PdnZ2o48TQgjRMMU5VQCYrYWEnN1f4zTHJ1eE2iGbzYafn5/XNrfbjcPh4LXXXiM1NZXhw4fz8ccfs3fvXn7++ecTnm/KlCls2bKFX375hR49enD11Vd7jdtpiKCgINLS0khLS2PLli0888wz/PnPf+a7775r9PtrCLPZjNVqbZZzCyGEgKLf5w8KqsrFPLh1DpQGuSLUtHz866/MaNV3A0VGRlJeXu61LS6u/rJl797/e7wxKiqKyMhIcnJyTni+kJAQQkJC6N69O8OHDycsLIyvvvqKyZMnNziTXq+nW7dunq/POussfvzxR5577jkuueQSYn+fhKuwsNCT9fDXAwYMaHA/h5WVlXmuNgkhhGh6BTsOAhBqqMTniKv5rYlcEWpKOl397SktXo2YpGrgwIHs3LnTa9uIESMAvJ7SKisro6SkhM6dOzf43EoplFLY7fYGH3M8BoMBm80GQFJSErGxsSxbtsyzv7KyknXr1pGSktLoc+/YsYOBAweedkYhhBDHVnKo/s5AVFKotkFOQgqhdig1NZX09HSvq0I9evRg4sSJ3HvvvaxZs4YdO3Zw0003kZyczJgxYwDIy8sjOTmZ9evXA/XjimbPns2mTZvIyclhzZo1XHXVVZjNZi6++OJGZVJKUVBQQEFBAZmZmbzzzjssWbKEiRMnAqDT6ZgxYwZPPfUU3377Ldu3b+fGG28kPj6eSZMmec6Tk5NDWloaOTk5uFwuz+226upqT5usrCzy8vK8Bl4LIYRoOnargxqHCYC4od1O0lpbcmusHerXrx+DBg1iwYIF3HHHHZ7tH3zwATNnzmTChAno9XrOO+88Fi9ejI+PDwAOh4OMjAzP2Bo/Pz9WrVrFK6+8Qnl5OTExMYwaNYo1a9YQHR3tOW9iYiI333wzTzzxxHEzVVZWem55mUwmOnfuzJNPPskDDzzgaXN4QPbtt99ORUUF5557LosXL/Ya7/TYY495njgDPFd9fv75Z0aPHg3Axx9/zLhx4xp1pUsIIUTDFe2tnz/Iz1ZC+DkjNE5zYjqlGvHcdTtTWVlJSEgIFouF4OBgr321tbVkZmaSlJR01MDjtmDhwoXcd9997NixA72++S4MWq1WIiIi+OGHHzyFiJbq6uro3r078+fP99wOPJa2/vMVQggtrXvnFzZudhFTvZsrP/xLi/d/os/vI8kVoXZqwoQJ7N27l7y8vNOa8+dkfv75Z84///xWUQRB/a2zhx566IRFkBBCiNNTf0UonIio1l9mtP6EotnMmDGj2fuYMGECEyZMaPZ+Gqpbt25eT6cJIYRoeqUVOjBATCueSPEwGSwthBBCiCZjL6ukRh8CQIdRZ2mc5uSkEBJCCCFEk8lathV0evwcFYT0bP0PpUghJIQQQogmk72lftmjWP8qjZM0jBRCQgghhGgy+SX1w48Tepz4aa3WQgohIYQQQjQJy6EqavQh6Nwuksb0PvkBrYAUQkIIIYRoEgdW7AIgpCaHwN7dNU7TMFIICSGEEKJJZG8rAiA2qBpdM07W25TaRkrR5EpLS4mOjiYrK0vrKC1q586ddOzYkZqaGq2jCCHEGcXldFNQXr8kU0KvUG3DNIIUQu3U008/zcSJE0lMTARg3rx56HS6Y76KiopOej673c6AAQPQ6XSkpaU1Ok9lZSUPP/wwycnJ+Pn5ERsby9ixY/nyyy85vAqMUorHHnuMuLg4zGYzY8eOZe/evUe9r3POOQd/f39CQ0OP6qd3794MHz6cl19+udEZhRBCHF/ennJc+OBbV0mHc/tqHafBpBBqh6xWK3PmzGHatGmebddccw2HDh3yeqWmpnLeeed5LaB6PPfffz/x8fGnlKeiooJzzjmHDz74gAcffJDNmzezcuVKrrnmGu6//34sFgsAzz//PK+99hpvv/0269atIyAggNTUVGpraz3nqqur46qrruLOO+88bn9Tp07lrbfewul0nlJeIYQQR9v3yz4AIsvTMfdtO4WQLLHRDi1atAiTycTw4cM928xmM2az2fN1cXExy5cvZ86cOSc93w8//MCPP/7IF198wQ8//NDoPA899BBZWVns2bPHq5jq0aMHkydPxs/PD6UUr7zyCo888ggTJ04E4IMPPiAmJoavv/6aa6+9FoB//OMfQP0VruO58MILKSsr45dffuGCCy5odF4hhBDelFJk76wAfEiIcaI3mbSO1GBSCDUhpRQ2p02Tvs1GMzqdrkFtV61axeDBg0/Y5oMPPsDf358rr7zyhO0KCwu57bbb+Prrr/H3929w3sPcbjeffPIJU6ZMOeYVpcDAQAAOHDhAQUEBY8eO9ewLCQlh2LBhrF271lMINYSvry8DBgxg1apVUggJIUQTKMmtxurwweCyk3RhP63jNIoUQk3I5rQxbP4wTfped906/H0aVohkZ2ef9DbWnDlzuO6667yuEh1JKcXNN9/Mn//8Z4YMGXJKA69LSkooLy8nOTn5hO0KCupnKo2JifHaHhMT49nXGPHx8WRnZzf6OCGEEEfbu3I/AOHluwi5cKrGaRpHCqF2yGaz4efnd9z9a9euZdeuXfz3v/894Xn+/e9/U1VVxYMPPnjKWQ4PhG5pZrMZq9WqSd9CCHGmydxUAPjSIbgaY1iY1nEapckLIZfLxRNPPMGHH35IQUEB8fHx3HzzzTzyyCOeWzdKKR5//HH+85//UFFRwYgRI3jrrbfo3v1/ky+VlZVx9913891336HX67niiit49dVXPbdKALZt28b06dPZsGEDUVFR3H333dx///1eeT777DMeffRRsrKy6N69O8899xwXX3xxU79toP721Lrr1jXLuRvSd0NFRkZSXl5+3P3vvvsuAwYMOOnts+XLl7N27VpMR9wLHjJkCFOmTOH9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xx9/rJRSaufOnQpQGzZs8LT54YcflE6nU3l5eUoppd58800VFham7Ha7V989e/b0fH311VerCRMmePU/bNgwdccddzTovVgsFgUoi8XSoPZCCCGEluxWh3rrjh/V63csUzsefFHrOJppzOd3k18R+vbbbxkyZAhXXXUV0dHRDBw4kP/85z+e/ZmZmRQUFDB27FjPtpCQEIYNG8batWsBWLt2LaGhoQwZMsTTZuzYsej1etatW+dpM2rUKHx9fT1tUlNTycjIoLy83NPmj/0cbnO4nyPZ7XYqKyu9XkIIIURbsXvFAVwYCKg5RJfrL9I6TpvQ5IXQgQMHeOutt+jevTtLlizhzjvv5J577uH9998HoKCgAICYmBiv42JiYjz7CgoKiI6O9tpvNBoJDw/3anOsc/yxj+O1Obz/SLNnzyYkJMTzSkhIaPT7F0IIIbSye1n9eNsEXRbm3r01TtM2NHkh5Ha7GTRoEM888wwDBw7k9ttv57bbbuPtt99u6q6a3IMPPojFYvG8cnNztY4khBBCNIjd6qCkygRAzwt7aZym7WjyQiguLo7eR1ShvXr1IicnB4DY2FgACgsLvdoUFhZ69sXGxlJUVOS13+l0UlZW5tXmWOf4Yx/Ha3N4/5FMJhPBwcFeLyGEEKItyN6cj9Lp8a85REzquVrHaTOavBAaMWIEGRkZXtv27NlD586dAUhKSiI2NpZly5Z59ldWVrJu3TpSUlIASElJoaKigk2bNnnaLF++HLfbzbBhwzxtVq5cicPh8LRZunQpPXv29DyhlpKS4tXP4TaH+xFCCCHOFAdW7wcg2nkQnyOGl4jja/JCaObMmfz2228888wz7Nu3j/nz5/POO+8wffp0AHQ6HTNmzOCpp57i22+/Zfv27dx4443Ex8czadIkoP4K0vjx47nttttYv349q1ev5q677uLaa68lPj4egOuuuw5fX1+mTZtGeno6n376Ka+++iqzZs3yZLn33ntZvHgxL730Ert37+aJJ55g48aN3HXXXU39toUQQgjNKLciL6f+wkCHBKPGadqY5nhs7bvvvlN9+/ZVJpNJJScnq3feecdrv9vtVo8++qiKiYlRJpNJXXDBBSojI8OrTWlpqZo8ebIKDAxUwcHBaurUqaqqqsqrzdatW9W5556rTCaT6tChg3r22WePyrJgwQLVo0cP5evrq/r06aMWLlzY4Pchj88LIYRoC4qyK9XrdyxTb926SJV+8bXWcTTXmM9vnVJKaV2MtVaVlZWEhIRgsVhkvJAQQohWa8M3e1j/w0EiS7Zx+atX4dOhg9aRNNWYz29Za0wIIYRo47I25gEQ7TrY7ougxpJCSAghhGjDamscFBW7AUjoFqhxmrZHCiEhhBCiDcvdVQboCKg5ROSwvlrHaXOkEBJCCCHasMz19ZP/RpSlEzh6tLZh2iAphIQQQog2SrkVuTvLAIiPURgjIzVO1PZIISSEEEK0USUHq6l1GjE4a+k8doDWcdokKYSEEEKINurAr/WzSYdVZBA6/kKN07RNUggJIYQQbVT25vrH5uNCazGGh2ucpm2SQkgIIYRog5wOF6VVPgB0Pre7xmnaLimEhBBCiDYoP70At86Ir72CuAtlMfFTJYWQEEII0QblrMoAINxxCF+ZTfqUSSEkhBBCtEH5+ywAxMbLavOnQwohIYQQoo1xOdyU1gYA0OnsRG3DtHFSCAkhhBBtTH5aNm6dEZ+6SmIvOFvrOG2aFEJCCCFEG5P9+/igCHcRPvLY/GmRQkgIIYRoYw4eqAEgtqOvxknaPimEhBBCiDakutxGqSMEgG6jZP6g0yWFkBBCCNGGZCzaBjo9wdXZRI+W8UGnSwohIYQQog3Zv6kQgISQanS+cmvsdEkhJIQQQrQR1so6imv8Aeh2bieN05wZpBASQggh2oi9K/aBTk9QZRaxqSO1jnNGkEJICCGEaCP2/5YNQAefIlltvolIISSEEEK0AS6Hm8JSAwCdB8ZqnObMIYWQEEII0Qbk7yz8fbV5Cx0uktXmm4oUQkIIIUQbkLliFwAR9hz8evTQOM2ZQwohIYQQog04uLcSgA6d/NDpdBqnOX11rjru/OlOvtjzBQ6XQ7McUggJIYQQrZytuo5yRxAAiWN6a5ymaazIXcGveb/y5tY30eu0K0ekEBJCCCFauayftoNOR4C1gKjRQ7WO0yS+2f8NAJd2vRSD3qBZDimEhBBCiFYue30WADGB1ehNJm3DNIFiazGr81YDMLHrRE2zSCEkhBBCtHKHSuo/rjv2jdY4SdP4/sD3uJSLAVEDSAxJ1DSLFEJCCCFEK1aRb8GqD0GnXCRdcJbWcU6bUopv9tXfFpvYTdurQSCFkBBCCNGqZS3fAUCI9SABPZI0TnP6dpbuZL9lPyaDidTEVK3jSCEkhBBCtGa5O4oBiAmpPSMem/8h8wcARieMJsg3SOM0UggJIYQQrZZyKwrKfQHo2DtC4zSnz63cLMleAsBFiRdpnKaeFEJCCCFEK1WSXUGdzg+Dy07C6P5axzltW4u3UlBTQIBPAOd2PFfrOIAUQkIIIUSrlbkqA4DQ6kz8k7trnOb0Hb4tdkGnCzAZWsc0AFIICSGEEK3UwfQSAGJD7ej0bfsj2+V28WPWjwCMTxyvcZr/advfVSGEEOIM5XK4KaqoHx+UcAbMH7Tu0DpKa0sJMYUwPH641nE8pBASQgghWqFDu4pw6Yz41FXSIXWY1nFO29f7vgbqB0n76H20DfMHUggJIYQQrdCBn3cCEFmbg6lrV43TnB6L3cKynGUAXNb9Mo3TeJNCSAghhGiF8vZZAIjvZGrz8wf9kPkDde46eoT1oFd4L63jeJFCSAghhGhlaq0OyuvqJxtMHNVT4zSn76t9XwEwqdukVlfUSSEkhBBCtDLZK3aidHr8bUVEn996BhafigMVB9hZuhOj3siELhO0jnMUKYSEEEKIViZr7QEAov0q0fv5aZzm9CzPXQ7AsLhhhPuFa5zmaFIICSGEEK1MfmH97aOE3q2vcGisFbkrADg/4XxNcxyPFEJCCCFEK1KeZ8GqD0bndpJ04VlaxzktJbYSthVvA2BUx1Eapzk2KYSEEEKIVmT/0h0AhFpzCOzVtpfVWHVwFQpF74jexAbEah3nmKQQEkIIIVqRnB31y2rEh9lb3RNWjfVz7s8AjE4YrW2QE5BCSAghhGglnA4XhVVmADoPaJ1XUBrK5rSxNn8tAGMSxmic5vikEBJCCCFaiYM7inDrjJjs5cRfMFjrOKfly71fUuuqpWNgR3qGtd65kKQQEkIIIVqJzJV7AIi0ZeHbubPGaU6d3WXnve3vATC179RWfYtPCiEhhBCilcjdVwNAh3hdqy4eTuarvV9RZCsixj+GSd0maR3nhKQQEkIIIVoBS7GVKocfOuVq08tq2F125uyYA8C0ftPwNfhqnOjEpBASQgghWoH9S+rn2wmpyiYitXVOPtgQc7bPoaCmgGj/aC7vfrnWcU5KCiEhhBCiFcjacBCA+CgnerNZ4zSnJrsym3e3vwvA/Wffj8lg0jjRyUkhJIQQQmjMabVTZA0AoOv5vTVOc2qUUjz929M43A7OiT+HcZ3HaR2pQZq9EHr22WfR6XTMmDHDs622tpbp06cTERFBYGAgV1xxBYWFhV7H5eTkMGHCBPz9/YmOjua+++7D6XR6tVmxYgWDBg3CZDLRrVs35s2bd1T/b7zxBomJifj5+TFs2DDWr1/fHG9TCCGEOGWZ36/FZTDh66ii48UpWsc5JV/v+5q1h9biq/fl4WEPt5nB3s1aCG3YsIH/+7//46yzvNdKmTlzJt999x2fffYZv/zyC/n5+Vx++f/uI7pcLiZMmEBdXR1r1qzh/fffZ968eTz22GOeNpmZmUyYMIExY8aQlpbGjBkzuPXWW1myZImnzaeffsqsWbN4/PHH2bx5M/379yc1NZWioqLmfNtCCCFEo+z7NQuAuGAreh8fbcOcgvzqfJ7b8BwA0wdOp1NwJ40TNYJqJlVVVap79+5q6dKl6rzzzlP33nuvUkqpiooK5ePjoz777DNP2127dilArV27Viml1KJFi5Rer1cFBQWeNm+99ZYKDg5WdrtdKaXU/fffr/r06ePV5zXXXKNSU1M9Xw8dOlRNnz7d87XL5VLx8fFq9uzZDXoPFotFAcpisTTuzQshhBANVFdtU29P+169fscylfHlGq3jNJrb7VbTFk9Tfef1VdcvvF45XU6tIzXq87vZrghNnz6dCRMmMHbsWK/tmzZtwuFweG1PTk6mU6dOrF1bPxX32rVr6devHzExMZ42qampVFZWkp6e7mlz5LlTU1M956irq2PTpk1ebfR6PWPHjvW0OZLdbqeystLrJYQQQjSn9C/W4zSa8asrp9ufztY6TqOtL1jPuoJ1+Bn8ePrcpzHoDVpHapRmKYQ++eQTNm/ezOzZs4/aV1BQgK+vL6GhoV7bY2JiKCgo8LT5YxF0eP/hfSdqU1lZic1mo6SkBJfLdcw2h89xpNmzZxMSEuJ5JSQkNPxNCyGEEKdg14ZSALqEVaD3MWqcpvE+3PkhAJO6TWpbt8R+1+SFUG5uLvfeey8fffQRfn5+TX36ZvXggw9isVg8r9zcXK0jCSGEOIMV51goc4Sgc7voO77tTaKYU5nDLwd/AWBKrykapzk1TV4Ibdq0iaKiIgYNGoTRaMRoNPLLL7/w2muvYTQaiYmJoa6ujoqKCq/jCgsLiY2tX2k3Njb2qKfIDn99sjbBwcGYzWYiIyMxGAzHbHP4HEcymUwEBwd7vYQQQojmkv7tdgCiLDuJPG+oxmkab/7u+SgUIzuMJDEkUes4p6TJC6ELLriA7du3k5aW5nkNGTKEKVOmeP7dx8eHZcuWeY7JyMggJyeHlJT6RwZTUlLYvn2719NdS5cuJTg4mN69e3va/PEch9scPoevry+DBw/2auN2u1m2bJmnjRBCCKEVpRRZu+vHoiZ2cKHzbd1LURxpc+Fmvtz7JQDX975e4zSnrslvRgYFBdG3b1+vbQEBAURERHi2T5s2jVmzZhEeHk5wcDB33303KSkpDB8+HIBx48bRu3dvbrjhBp5//nkKCgp45JFHmD59OiZT/SyVf/7zn3n99de5//77ueWWW1i+fDkLFixg4cKFnn5nzZrFTTfdxJAhQxg6dCivvPIKNTU1TJ06tanfthBCCNEopXnV1Dj90LsddE3tr3WcRvk171dm/jyTWlctw+KGkRLXdi8waDIq61//+hd6vZ4rrrgCu91Oamoqb775pme/wWDg+++/58477yQlJYWAgABuuukmnnzySU+bpKQkFi5cyMyZM3n11Vfp2LEj7777LqmpqZ4211xzDcXFxTz22GMUFBQwYMAAFi9efNQAaiGEEKKl7V1a/xR0uGUvoefdqnGahsuvzvcUQSM7jOSl0S+1mckTj0WnlFJah2itKisrCQkJwWKxyHghIYQQTWr+vd9Rbg9ggHErI16fqXWcBntg5QMsylzEoOhBvDvuXXwMrW8CyMZ8fstaY0IIIUQLqyqvpdweAMpNt/PbztNi24q3sShzETp0PDD0gVZZBDWWFEJCCCFEC9v7404AQqqyiRx3nsZpGia7Mpt//vZPAC7teim9I9rm4rBHanszNwkhhBBtmFKKXWsPAWY6BldiCAzQOtJJ/d/W/+PtbW/jdDsJ9Ank7oF3ax2pycgVISGEEKIFFRywUFFrRu+qo/eF3bSOc1LrDq3j9bTXcbqdjOwwko8mfERMwJnz0JFcERJCCCFa0LZvdgAQU7aNyIvu0jjNiTndTp5d/ywA1/a8loeHP6xxoqYnV4SEEEKIFlJb4+DAHhsAPRKd6P39NU50Yp/s/oR9FfsINYVy18DWXbSdKrkiJIQQQrSQjDV5uDEQWJVL5ymjtI5zXBsKNvDW1rfYULABgLsH3k2IKUTjVM1DCiEhhBCihWT8cgCADtXbCUxpnYuUbinawu1Lb8fpdmLQGbi066Vc0f0KrWM1GymEhBBCiBZQXW6nuKT+37sN7YDO2Po+ggtqCpj580ycbiejO47m4eEPExtw7IXKzxQyRkgIIYRoAXt/2QtAiGU/cZMnaRvmGA5UHOCOpXdQWltKz7CePDfquTO+CAIphIQQQogWsffwbTH/ckxdkjRO4+27/d9x7cJrOWA5QKQ5klfPfxV/n9Y9kLuptL7rcuKElFLUZWdTtHorQR0jCT57YKt/6kAIIdq7mpJqiq3+oIOeE1rXSvPzdszjpU0vATA8bjizR84m0hypcaqWI4VQG6CcTso//ZSqtevZm2cmN/AsrAGxGJwVxL84m36D/On89xnozWatowohhDiGnZ+tAZ2RYOtB4i6ZrHUcAGqdtby6+VU+3PUhADf3uZmZg2ei17Wvm0VSCLUBxa+8QsaXv7Gn+1XUxkTVb1QKl9FMbocxFORWcdYN9zPwuRmYunbVNqwQQoij7N1qASJI7KRH56P9QqVpRWk8svoRsiuzAbh30L3c2u9WjVNpQwqhVq5y6U9s+KmArLP+AoC/v44hFyfSY0QCh/ZVsHb+dsrKg9gUeRmVs97hvBdvxdS9u8aphRBCHFa8O59yItApF32vHqp1HDLKMrh96e3YnDaizFE8MvwRzu90vtaxNNO+rn+1MTVbt7H87Q1kJV4MwFnnd2TKMyPpNzYJk9lIYr9Irn7yPPqm1N/L3Rt7IRvvfgb7/v1axhZCCPEH2z/fCEBUXQ5hZ/XQNEuRtYjpy6Zjc9oYGjuUryd93a6LIJBCqNWq+uUXfvzH9+RFDQOlGHVNN0Ze3QNfP++LeAYfPefddBa9h0WCTs+ODpezZ8YjuG02jZILIYQ4zO1WHMjRAdDjrCBNszhcDmb8PINCayFJIUm8PPplgn2DNc3UGkgh1ArVbNzI8peWkx89HJSbsTd0p9+YTic8ZtT1fYnu6I/TJ4DNwakcev7lFkorhBDieDJX7MKuD8DHUU3y5NGaZnl186tsL9lOsG8wb5z/xhm7ZEZjSSHUyriqqlj/9KccjD8PgPOv70nPc09cBEH9laHxfxmAyQTVQZ34bXP9VSUhhBDa2bYoA4COhjxMsdGa5Vh5cCXv73wfgCdHPElCcIJmWVobKYRamd2Pv8LuqLEADJuQQK+RDf+PNSjcj9Q7BwCKgrgUNr/xA8rtbp6gQgghTqiyoJL8qvrbYf1Su2mWI8uSxd9X/R2A65Kv44JOF2iWpTWSQqgVKfnqO9aVdMOt9yGhkw+D/9T4/3ESksMZdlF98bQ76FyKF/7U1DGFEEI0wJb/rgadnjBrFh0njtEkg8Vu4a7ld1FVV0X/qP78dchfNcnRmkkh1ErYcw/yy/w92PxjMBsdjLtnODqd7pTONeiS7oSYbDh9/Pnt8wyUUk2cVgghxIk4nS727nECkNzbT5MFVpVSPLjqQbIrs4kLiOOVMa/ga/Bt8RytnRRCrYByuVj36HsURAxEp9yMv3sIfoGnPuGWXq/jvJvOAiDXrxc5365qqqhCCCEaIOPrjdgNAfjWVdLnlnGaZPjuwHesyluFr96Xf5//73a1bEZjSCHUChz84HPSfeon2RpyfhTxPSNO+5wJgxJI8C8FnZ7fvj6AcrlO+5xCCCFOTinFlp/yAOgSVIwpuuULkBJbCc+tfw6AOwfcSc/wni2eoa2QQkhjzvJyNi08gNvgS1SwnbOvOqvJzj1y+rnolIsSUyf2/efLJjuvEEKI49v3UzoWQjG47AyZNlKTDLPXzaayrpJe4b24uc/NmmRoK6QQ0lj2C2+QHz4YgHOnDUWnP7VxQccS1jWOxBg7AJtXFOIsK2uycwshhDiaUoqN3+wBINGYTchZyS2eYeXBlfyY/SMGnYF/nPMPjHpZTetEpBDSUNXPP7NjuwOlNxIbZ2ySW2JHSrljFCg3JaG92ffK+01+fiGEEP+TtWY/Zc5Q9G4HZ98wrMX7tzqsPP3b0wDc0PsGekX0avEMbY0UQhqx793L3kdeID/uHACGXduvWfoJ6xBMUlL9XwPpu1y4qmuapR8hhGjv3G7F6vnpAHRy7yPinIEtnuHtbW+TX5NPXEAcd/a/s8X7b4ukENKAs7ycA3fNIq3rDbj1PnRMDqVDj9Bm62/QNfX/MxaF9qXkq++brR8hhGjPdnyzFYsrCKPTSsotw1u8/4yyDD5I/wCAh4c9jL+Pf4tnaIukENKALX0nW0PHY/OPITDUh3HT+p7ynEENEZMYTIh/HW6DL7u+3ybzCgkhRBOrq3Wyfkk+AMm++wg/Z3CL9u9Wbp787UlcysWFnS/kvITzWrT/tkwKIQ0UmrtTGtYLg1HHxX8ZgDmoeSe40ul09LmgKwA5hm7YNm1q1v6EEKK9WTf3N+z4YbYWcfbMS1u8/wUZC9hWvI0AnwAeOPuBFu+/LZNCSANdB0Ux8poeXHBTb6I6BbVIn8mjOqPDTVVwZ7I/WdwifQohRHtgKbGyI80KQP/4Ivy7d2nR/rcXb+eFDS8AcPfAu4kJiGnR/ts6KYQ0oNPpOGtMR7qf3XL/sZqDfOmUVH/lae9+N6qursX6FkKIM9mqt9bg1hkJs+zlrFnXtmjfxdZiZvw8gzp3HaMTRjM5eXKL9n8mkEKoHel7Uf1jlAXhA6j8dY3GaYQQou3LzyglO08Pys3Zg/T4REe3aP9P/fYURbYiuoR0Yfa5s9Hr5GO9seQ71o506hOBn96OwyeQPYvStI4jhBBt3ur/1P9RGV++hS53XteifWdaMlmeuxyAF897kUDfwBbt/0whhVA7ojfo6d63/n+U/Xm+KIdD40RCCNF2Zf6wgaLqAHRuF0OvSMYQGNCi/f93538BGJ0wmu5h3Vu07zOJFELtTL/LBgBQGtyDouW/aRtGCCHaKFd1Db99vB2Azr55xF/9pxbtv6y2jG/3fwvATb1vatG+zzRSCLUzYXFBRPhaQKdn14+7tY4jhBBt0o5XPqHMPxGdcjHi/j8161xwx/LRro+wu+z0jejL4JiWnbPoTCOFUDvUc0gUALnFJrk9JoQQjWTZn8+6A5EAJHfXE9opskX7zyjL4L0d7wFwS79bWrwIO9NIIdQO9fjTIFBuKv07UrxivdZxhBCizVBuxY+vrsHhG0SQq4yRd7fsDM4Ol4OHf30Yp9vJmIQxjO00tkX7PxNJIdQOBYT7E+FbBcCeJTs0TiOEEG3Htq/SKKoLR++qY+w1nfAxGVu0/zk75pBRnkGYKYzHUh6Tq0FNQAqhdiqxXzgAuYd0KKdT4zRCCNH62Sy1rPt9PbFePruJHzu0RfuvcdTwwc76RVX/PvTvRJpb9pbcmUoKoXaq54T6FenLA5IoX71R4zRCCNH6/fLiEhx6MwHWQ6Q8fE2L9//5ns+pqqsiKSSJ8UnjW7z/M5UUQu1UWIdgggzVKL2B/YvTtI4jhBCtWu7aPewvqp8nKGVkAKYOcS3af52rjg/S668GTe0zVWaQbkLynWzHOnev/586J1dujQkhxPE46lws+2A36PR0cO2nx60TWzzDwgMLKbIVEW2OZkKXCS3e/5lMCqF2rOsFfQAoMXWiNjNL2zBCCNFKrX53HTUqEF97BWOmj2jxAco2p4030t4A4IbeN+Br8G3R/s90Ugi1Y/G9o/FRdpw+geQslsfohRDiSAczykjfVgvA4LADhAzo3eIZ5u2YR6G1kPiAeK5NbtnV7dsDKYTaMb1BT2x4/YSK2VsLNU4jhBCtS12tk59er/8jMb5gLf3+1rKLqgIU1BR4Jk+cOWQmfka/Fs9wppNCqJ1LHNIRgILqINx1dRqnEUKI1mPZP76hxuGLn62Ecy5NwCc+vsUz/GvTv6h11TIoehCpnVNbvP/2QAqhdq7LBfWXeSsDOlK+ZpPGaYQQonXY/d+lHCgPAyBlgIOYW25s8QxpRWksylyEDh0PDH1AJk9sJlIItXOBoX6EGKpAp2f/UpllWgghrEUV/LqiBoBuIUX0njmlxTO4lZvn1j8HwKRuk+gd0fJjk9oLKYQEnXoEAZBzoBbldmucRgghtLXs2SXYfYLxd5Qx+uFLNMnw/YHv2VG6gwCfAO4ZdI8mGdoLKYQE3S/uD0BJQFeq1sks00KI9mvT+6vJsUaBcjP60lhMwQEtnsHqsPLKplcAuK3fbbKURjOTQkgQ2zUcs74Wl9GP/d+t0zqOEEJoYs+Kvfy2xgZAb/9Mkiaeq0mOd7e/S7GtmI6BHbmh9w2aZGhPpBAS6PQ6Onf3ByBrX60swiqEaHcK95ex7OMs0OlJqNnOqKdbflwQQF51Hu+nvw/AX4f8VSZPbAFSCAkAeoyrn2W6OLAHVWt/0ziNEEK0HFulnUUvrsWtMxBZvpMLH78Eg7+/Jlle3vgyde46zo49mws6XaBJhvamyQuh2bNnc/bZZxMUFER0dDSTJk0iIyPDq01tbS3Tp08nIiKCwMBArrjiCgoLvSf0y8nJYcKECfj7+xMdHc19992H84grFStWrGDQoEGYTCa6devGvHnzjsrzxhtvkJiYiJ+fH8OGDWP9eplB+Vg6JEfgq3Pg8A0ia9EGreMIIUSLcLsVCx9fhFWZMduKGDutD+ZuXTTJsrFgIz9m/4hep+eBs+Vx+ZbS5IXQL7/8wvTp0/ntt99YunQpDoeDcePGUVNT42kzc+ZMvvvuOz777DN++eUX8vPzufzyyz37XS4XEyZMoK6ujjVr1vD+++8zb948HnvsMU+bzMxMJkyYwJgxY0hLS2PGjBnceuutLFmyxNPm008/ZdasWTz++ONs3ryZ/v37k5qaSlFRUVO/7TZPb9CTkFh/CTb7gB2llMaJhBCi+S178hsKbSHoXXWMucCfiHFjNMnhcrt4fsPzAFze/XJ6hvfUJEe7pJpZUVGRAtQvv/yilFKqoqJC+fj4qM8++8zTZteuXQpQa9euVUoptWjRIqXX61VBQYGnzVtvvaWCg4OV3W5XSil1//33qz59+nj1dc0116jU1FTP10OHDlXTp0/3fO1yuVR8fLyaPXt2g7JbLBYFKIvF0sh33TbtW3dQvX7HMvWfmz5Ttj17tI4jhBDN6rdXF6nX71imXr9jmdr83HxNs8zfNV/1nddXDf9ouCqxlmia5UzQmM/vZh8jZLFYAAgPDwdg06ZNOBwOxo4d62mTnJxMp06dWLt2LQBr166lX79+xMTEeNqkpqZSWVlJenq6p80fz3G4zeFz1NXVsWnTJq82er2esWPHetocyW63U1lZ6fVqTzoPiMWgnNj9wsn9QZ4eE0KcmZxl5Sz/23ts3GkCoG9oLgPu024x082Fmz1Xg/4y4C9EmCM0y9IeNWsh5Ha7mTFjBiNGjKBv374AFBQU4OvrS2hoqFfbmJgYCgoKPG3+WAQd3n9434naVFZWYrPZKCkpweVyHbPN4XMcafbs2YSEhHheCQkJp/bG2yijr4H4yPpFWA9sLdE4jRBCND3LhjS+uOtjdlUnAtA9II+RT1+v2XicgpoCZq6YidPt5MLOF3J9r+s1ydGeNWshNH36dHbs2MEnn3zSnN00mQcffBCLxeJ55ebmah2pxXU7pzMAh+qicFVXa5xGCCGaTu6XP/HF6xmUBCejV07OHWli3Es3oDcYNMv0/IbnKasto2dYT54a8ZQMkNZAsxVCd911F99//z0///wzHTt29GyPjY2lrq6OiooKr/aFhYXExsZ62hz5FNnhr0/WJjg4GLPZTGRkJAaD4ZhtDp/jSCaTieDgYK9Xe9N1TE90ykVNQByHlqzROo4QQpw2Z52LVS8u4vsfnNjMUZhVDZfNHED/KSM0zZVeks7S7KXo0DF75Gz8fbR5ZL+9Mzb1CZVS3H333Xz11VesWLGCpKQkr/2DBw/Gx8eHZcuWccUVVwCQkZFBTk4OKSkpAKSkpPD0009TVFREdHQ0AEuXLiU4OJjevXt72ixatMjr3EuXLvWcw9fXl8GDB7Ns2TImTZoE1N+qW7ZsGXfddVdTv+1mVWwt5vM9n7O1eCt7yveg1+kJNYWi0+lwKzejE0Zza79bMRvNp92Xyd+HaHM1hbUh7Fm+h45XjGuCdyCEEC1PKUXm1hJWzkujptYPDBDtU8aEJy/GP0z7ouPVza8CMKHLBLqHddc4TfvV5IXQ9OnTmT9/Pt988w1BQUGe8TghISGYzWZCQkKYNm0as2bNIjw8nODgYO6++25SUlIYPnw4AOPGjaN3797ccMMNPP/88xQUFPDII48wffp0TKb6wW1//vOfef3117n//vu55ZZbWL58OQsWLGDhwoWeLLNmzeKmm25iyJAhDB06lFdeeYWamhqmTp3a1G+7WRRbi3lr61t8ve9rHG6H175C6/+udO0p38PCAwt5aNhDjOo46rT77X5uZwp/qiC3MgRnaSnGCBm4J4RoW+psTpbO2U7WjnLAgMleTv/YIgY/dbumt8IOW523mrWH1mLUGfnLgL9oHadd0ynVtBPGHO/+5ty5c7n55puB+gkV//rXv/Lxxx9jt9tJTU3lzTff9LpllZ2dzZ133smKFSsICAjgpptu4tlnn8Vo/F/ttmLFCmbOnMnOnTvp2LEjjz76qKePw15//XVeeOEFCgoKGDBgAK+99hrDhg1r0HuprKwkJCQEi8XSorfJap21/Hfnf/nP9v9gc9avezMweiATkiaQHJGMUWekwl4BQImthH9v+benMBrbaSwPDnuQaP/oU++/xsF7s1agdAYu6pdPl+kyeE8I0XbUVNj59vm1lJW50bmddDq4jEEXdiRuxl2tYgzO/or93PjDjVTWVXJtz2t5ePjDWkc64zTm87vJC6EzSUsXQkoplmQv4V8b/0V+TT4AZ0WexczBMxkSO+S4x1kdVt5Me5MPd32IS7kI9wvn2ZHPkhKfcspZvn74B/JKTXStWEvqxw+1il8eQghxPG6Xmw0Ls9i/Po+KEjsKPb51lQzMmU/yP+4lcIS244EOK7YWM2XRFA7VHKJ/VH/+M+4/TTKsQXiTQqiJtGQhlF6SznMbnmNL0RYAYvxjmDl4JhclXYRe17Ax7RllGTz868NklGegQ8djKY9xZY8rTynP7lXZLPtoP2ZbMdfc1YWAs88+pfMIIURzq6uuZdFLq8k79L8/2AKq8xiRkE3S/dMxhoVpmM7b3375G0uylpAYnMh/L/ovoX6hWkc6IzXm81sWXdVYnauOlze9zOSFk9lStAWz0cxfBvyF7y77jgldJjS4CALoGd6TDy/+kMu7X45CMXvdbPaU7zmlXF2HdsSAC5s5iqyvfzmlcwghRHMrSdvDp/d8Rd4hHXpXHcm7P+RC3SKumtWH7rMfaVVFUFpRGkuylqBDx4vnvShFUCvR5IOlRcPlVedxz/J7PMXKxUkXM3PwTGIDjv14f0P4Gf14IuUJSm2l/HLwF/6+6u98POFjTAZTo87jYzKQ0NlIVrbiQEYtvV0udK1ggKEQQkD9WMaMz9ewblUVDt8YfJw1nNs5l64PPoqpS9LJT9DClFK8sPEFAC7rfpmsJdaKyBUhjaSXpDNl4RT2lO8h3C+cV8e8ynOjnjutIugwnU7HP875B+F+4ewt38uDqx70DLpujF7jkgEoCOpN9YaNp51LCCFOV2VBJd/OXsWcv67k17UuHEZ/QpzFXPXAYHo/+pdWWQQBfL3va7YVb8NsNHPXgLY1hcuZTgohDaw/tJ6pS6ZSWltKz7CeLPjTAs7vdH6T9hFhjuCpEU9h1BlZmr2Um364iYKaYy8tcjydz4rBR+egzhRK1vfrmzSfEEI0hnV/Fiumv8b8R38lN9sB6PC3FpAcdJCrX7mUsO7xWkc8rp2lO3l63dMA3H7W7UT5R2mcSPyR3BrTQNfQroT7hZMYkshL571EgE9As/QzsuNI/jPuP8xaMYtdZbuY8fMM/nvRf/Ex+DToeIOPns6JPuzLhAN7a+nrdqPTS+0shGgZ1b+upvTH5ewrDmG/vTMO375ggJDqLAaH7afLY1MxdeumdcwTKqwpZObPM7G77IzqOIpb+t6idSRxBHlq7ASa86mxgpoCIs2RGPXNX4serDrINd9fQ2VdJdP6TmPG4BkNPjZnexHfvbEDo6Oa6/7cgaCzBzdfUCFEu1ZZYuPQfgt6g47SH34if2MmRVEDcf3+eLm/qmbQ2A70u3wgekPr/6NscdZinvrtKSx2CwlBCXzyp08I9m1/SzdpoTGf33JFSCNNMRaooToGdeQf5/yDmStm8t6O9zgn/hyGxg1t2LF9ojDparH7BLL3s18ZJIWQEKIJKZcL2559bF2axdZdBlzqcIETB3FxAIT4O+k/NIjeV56Hwdg2Htr4aNdHPLv+WQB6hffixfNelCKolZJCqJ0Y23ksV3S/gi/2fsGjqx/ly4lfNuiWnF6vo1vvINLTHWTk+NK/qgpDUFALJBZCnIncbkXJmjSKl6/Fvu8AJcUO8qKGYfWv/+MwsCoXo6sWvXIRN7AzXS4ZTkKvcHT6tjOp67pD63hhQ/0TYlP7TOXuQXfjo2/YkATR8uTW2AlotcRGc7E6rFz+7eXkVedxdY+reTTl0QYdV1Fk5aNH14BOz0WDiuly+zXNnFQIcaapLq7k13c3kJnlwq07+m9wo6qjr98euiUpzL174T9wIMaotjeoOLcql+sWXkeFvYJLu17KUyOekpn5NSC3xsQx+fv48+Q5TzLtx2ks2LOACxMvZHjc8JMeFxrtT0KkndxSM9tXFZB0m5L/sYUQKJcLx6ECdD4+GAID0AfUX2V2FBVRuW4TmdvLOFTgxl7jpFQXjdNoBp0RnduJv8GOwd8Pc4iZnqM603NYHL7m8Rq/o9NTaivlz0v/TIW9gj4RfXh0+KPyu7INkEKonRkaN5Rrel7DpxmfMnvdbL649IsGDdgefM1Act/cTb45mbJV64kY1bCFa4UQLaN21y6U3Y5Px44Yfp9N2bpuHZVrN+Dfrw9BY8/HbrFRvGoTjvIKsNsJ7x5LYHI3ynfnkrUhG5Wfi7EoC78uSfgPGULUWUmYQv0pXJlG/pZsrIUV2KtqcfsF4tL7oC/MxWAtx+ETiN0UhjWkI3bfEHDU4fQJwGWoH+PD73eFgmvzGdS5gq7TJuHXqaM236hmUlZbxp0/3UlOVQ4dAjvw7/P/jZ/RT+tYogHk1tgJnGm3xg6rrKvkT1/+iXJ7OQ8Ne4jJyZNPeoxSio/v/oZyZzBdnTsY/+49LZBUCOGuraU2PZ3aHTvQ+fvX3zKKjUXp9OzbbiHtx2zqCgrxKcnFZTBRawpDp1wYXXXU+QRSZwoBQKdcKJ33QGOd24XZVoz1BA9vGB3VOH0CTyl7gN5Kp0gbwbHBhHSJpcuF/TC0gae9GkMpxQ+ZP/Ds+mcpt5cT7hfOBxd9QOfgzlpHa9dk0dUmcqYWQgCf7P6Ep9c9TagplO8v+56Q339Znsje5Rn8uCAPg8vOVZODiTi/dazmLMSZxOV0U3aohuKMQhxrf8Hn23dR1VVUBXWiIqQblpAu2H1DsJtCqDOFNvr8Ps4aDAZw64zU8fvSO0oRritF7+9PrfLDbbfjsjuw+9T/3tMpJxG+1QSEmjCF+GNUdeidDpxBEThNgZiDTJj9FAHOcszOSvySk/GNCic8PuCMvjWUXpLOCxtfYFPhJgB6hPVg9sjZ9AjroXEyIYVQEzmTCyGn28mV317Jfst+pvaZyqwhs056jFKK+fd8R4UjkC62NMbPm3lG/5IToqUopSjLr2Hn6nwyfivAbnV69hmctSi9Hrfe96jjjA4rnXJ/JMy3BvOUWwno0ZWAQD2uGiv2SiuBCdGExAThKCqifMkyApPiCLtgNDofH5RSVJXWUpJjISoxlKDwo2/j2KrtWPIsRCRG4GNqG4+tt5QP0j/gxY0volCYDCZu7Xcr0/pOa/CEtaJ5SSHURM7kQghg5cGVTF82HZPBxKLLFxHtH33SY/avzmTxfzPRu+q4fALETGrbgxuFaClut8JWWUdtjQN0YNI7KVy3i8y0Ig4W+1Dj/F8hYnRYCazJwxYUh91Qf1vKL8CHuG4hxHULISTcFx8jhIe4MNhr8E1MRG9q3MLK4tS4lZuXNr7EBzs/AOCipIuYNXhWi84NJ05OnhoTDTKyw0gGRg9kS9EW/m/r/zXocfou5yQS/vlOymxmVn+6nUkXjvQ8KSKEOLb8fRUsm5tOZan9GHvr5+XSux2El6bT4dBqwst2EXHTDUTNmkppkR2DQU9YnL9cgdWYUsqrCJo1eBY397lZfi5tnFwROoEz/YoQwMaCjUxdMhWjzsi3k74lITjhpMcc2l3Ml//aCjo958bto//jt7dAUiHaBqUUtTUOrJY6ig+Ukrsljz07bYAOlBsflw2lFE6fQHycVmJ8iukY5aBDBwM+JgPKZsPcvz8B55yj9VsRf6CU4r0d7/HK5lcAePKcJ7ms+2XahhLHJVeERIMNiR3CiPgRrM5fzSubX+Gl0S+d9Ji45Ch699Szcw9syIqky44Mgvr2bIG0QrRehZmV7F57iMytxdRY6o7YqyO24Dd67Psco9MGQOhNNxMzcwZ6P7ml1Zq5lZuPd3/MZxmfsd+yH4C/DfmbFEFnELkidALt4YoQQEZZBld/fzVu5ea91Pc4O/bskx7jqHPx0T0LqSGQKHsWl785BaNZfqGL9kUpRWleDZt+yGLfpiKvfT6OavxsJYTZ84mPctBr2p8w9eqNbcsWjFGR+CUna5RaNMbLG19mbvpcAEwGE7efdTu3nyVXwVs7GSzdRNpLIQTw1G9P8WnGp/QI68Gnf/q0QZMs5m/J5pu3duHW+9ItpJDU504+H5EQbZXb5ebg7nJ2rs6n5GA1BpcdW5UDW93vT1MpNzGFG4kt2kCEKiLyhsmEXXMNxogIbYOLU/b5ns/5x9p/ADBz8Eyu6nEVQb6y1mJbIIVQE2lPhVBFbQUTvppAZV0ljwx7hGuSG7ae2I73l/HL2vqBgv272Tj3bxOaM6YQLabggIW9GwqxFNuoKLRSWWJFqaMHxepddYSX7yIp5wfiBnUlZNIkAs8fg9736MfdRdtgsVt4M+1NPsn4BLdy85cBf+HO/ndqHUs0ghRCTaQ9FUIA83fNZ/b62YSYQlh42cIGTbII8Mt977GjKhGA3qF5jH5mCjr9mTV7rGgfXC43NRV2ti07yNafc+GI345Gh5XYwvVElm5DFxKGuUtnouN8MXfpTHBqKsbISG2Ci9Nmd9n5dPenrM5fzZaiLdh+H8t1VY+rZM2wNkgKoSbS3gohp9vJVd9dxb6KfUxOnsxDwx5q0HHK7WbVE5+yvSgGgD5BmZz3/C3yi0O0GdXFVaz6aCeZGTX88TdiTOEGQiv24G8rJtDXQYdbrsXUrRs+8fH4JiXKf+NniLX5a3nqt6fIqcrxbOsW2o0Hhj7QoIWpResjhVATaW+FEMC6Q+u49cdbMegMfPqnT+kZ3vCnwdb86we2ZNQPmB4cc5BhT9wgHxSi1akuryV/bwU1FXXUlFZTtnYLh2qCcfrUz4elczvxtxbS7cDXRFbvw++sfgQMG074jTdgCGnYVVLRNpTYSnhhwwssylwEQLQ5mpv73szQ2KF0D+uOXidXttsqKYSaSHsshABmrZjF0uyldA/rzvyL5zdqBeUVz3xHek4AKDdddPs478FL8O/coRnTCnFySin2by5m609ZFGRWH7NNUM1B+lQsI7iuAGNgECETJxJy2SQMQTI49kxRWFNIgbUAh8vB0uylfL3va6xOKzp0TE6ezN0D7ybQ99QWmBWtixRCTaS9FkIlthKu+PYKymrLuKrHVTyW8liDj1VK8dOT37HnUP0vE3NtKRde05GEi1KaK64Qx+Wwu8jcVkza0lyKc6o824MrMzHbSvCts2A2QcfJf6LHZcMwGGU9rTNNnauOVQdX8fnez1mdtxp1xMCv3hG9eWz4Y/SJ7KNRQtEcpBBqIu21EIL6e+Z3LL0DheLVMa9yfqfzG3X8vh+388vnmdTqAzG47Jx3UTi9Lh/WTGmFqF/Lqyy/BpfTjdViZ+/GIjLTinA66n/FGZy1JBxcTqJPLnFXXoy7rn7Sw9Arr8QYFqZldNEMDlgO8OHOD1mcuZgqx/+K4PiAeHQ6Hd3DujM5eTIpcSlyC/8MJIVQE2nPhRDAvzb9i/d2vEeHwA58M+kbTIbGTZhoK6/h2we+pkQfB8rN0IFw9p/HNlNa0d643YrCzEosxVZKcqrZu7EQa+WRMzqD2VZMTOEGOpauI2HmnYRde6081XgGsbvsZFmyKLQWUmGv4EDFAdKK09hUuMnTJtoczcVdLubKHlfSObizhmlFS5FCqIm090LI6rByydeXUGQt4t5B93Jrv1sbfQ5HdQ1L7v2AbJ/6Qde9gnI578lrMJgbPu5ICABLsZWsbaX4BfpgMOrZuCiL0jzv8T5GVy1GR039AqZlu4gp3kRklB7/Pn2JuON2TF26aJRenC6lFPsr9rO9ZDuZlkwOWA5wwHKAvOo83Mp9VHsdOsYkjGFKrykMiR0iA5/bGSmEmkh7L4QAvtv/HQ/9+hBmo5nvL/ueaP/oRp/DbbfzyxOfsbM8HoAQRwFjpg2iwzmyxIA4uYoiK79+tpfsHaVHz+ujcxLqLMa3NJvIwi2El+3CNzKcqBkz8B82DJ/oKHTtcGJDpRQFNQWEm8MbfSVXC2lFaWSUZdAnsg9GvZHv93/P7vLdnp+3QpFTlUNBTcExjw/yDaJjYEdCTaHEB8bTN7Ivw2KHNWgRaXFmkkKoiUghVL/g4PWLrmd7yXYGRA3g3dR3T/kX65a5K1i3xorL4IdOuRjSp46h98hM1OL4cneVseQ/O7BbnQCE1WThdjipM4UQWbKVxOwl+DitAPgmJRF27TWEXnkl+oAALWOftlJbKT9m/0hFbQX+Pv7odXrcyk2gTyCxAbEU1BSwo3QHJdYSqhxV+Bn8iDBHEOEXgdlo5qecn9hTvodo/2juO/s+Iv0iSS9Nx+l24qP3wcfgg8lgIj4wnsTgRIx6I063kzpXHU7lxN/oT4BPAAG/TylwsOoguVW5hPqFEm2u/2NIp9MR4ReBTqdjb/leVuWtwuFyYNAb6BTUidiAWKrqqrA6rZ7zBfkGkWXJ4oOdH5BRnkH/qP643C7WFaxr0PfFZDDRP6o/XUO70iWkS/0rtIsnhxCHSSHURKQQqnfAcoDrF11PVV0V4xPH89yo5075MrNlXx7Lnl3CIWMiAF18sxn7zyvxCZFHlNszt1tRVWqjvMBKRaGV0uxyDqUfwlLjAzodIdaD9No+B39bERiN+CUn49spAWNUNKYe3fHr3RtTcnKb+jBUSrEidwX/Tvs31XXVnBN/DkG+Qewu283Ggo04lVPriOjQYdQbcbgdx9zfIbADsQGxXuNxToVRb2RA1AAyyjKwuWyM7jiaUR1Hef7o0ul0hJhCGBQ9qFHTeYj2SwqhJiKF0P+sP7SeO5begVM5ua3fbdwz6J5TPpfb6WT1U1+wrSAKgMC6Ys6/IZmEMf2bKq5oI+psTrYszWHrTzk46o4e5wEQd2g1PfYuwBQZTuTddxHypz+hN5tbOGnDuZWbXWW7WJu/lhJbCf5Gf7qGdmVc4jhQ8PX+r9lcuJn9FfvZVbbruOfpF9mP5PBkrE4rbuXGoDNQYa+ov+XlF06/yH50DOpIoG8gtc5aSm2llNaWYrFbSA5PZnzieD7b8xnvp79PgE8A/aP6E+ATgMPtwOF2UOusJacqh9yqXNzKjY/eB1+DL3qdHpvThtP9v0LMV+9Lp+BOWOwWSmwl6HQ6lFKeR9H1Oj0jO4wkyj8Ku9NOdmU2hdZCQkwhBPgEYHPaqKqrosZRg4/eh0ndJjE6YTRpRWlUO6qZ2G0iHQI74HK76rMYfJr95yTObFIINREphLx9ve9rHl39KABPnvMkl3W/7LTOt/vL31i1qIg6YyA65aJXRysjH/gTRl+Zy+VMplT9Y+671x5i95p8aq0uoH7xUrOtGH9rIf62QsKDXHS+aCgh3TqiMxowDxjQqguglQdX8t3+7/jt0G9U2CuO2t8hsAM6dBysPujZZtQbubH3jQyJGcJvh37D6XbSNbQrg2MG0zW0a5PkOvwr/nhXy1xuF3qd3mu/Uoo6dx1VdVXYXXZi/GMw6o2efTqdDqvDysbCjWRXZjO642gZjyNaFSmEmogUQkf795Z/8862dzDqjDw54kku6XrJaZ2vOq+EpU8tJF/V/xINUJWcNTKGvlcMwdcsfxWeCarL7WRuLaI8r4qKYhvF2VXU2v539cffWkiXA9/SubuZ8KuuxJTcC0NwEIaI1jvuw+F2sLVoK4dqDhHkG8S3+79lafZSz/4AnwDOjj2briFdqXZUszR7KWW1ZQBEmiO5uufVdA3pyllRZxEbEKvV2xDijCWFUBORQuhoSike/PVBFh5YCMAV3a/ggaEPYDae+l/qSim2vfol67YZcfjWjxUyumvp1U0xZNoo/CNk/FBbo9yKzG0lbF2WS/7eiqP2H368Pf7QauIiHMQ9/BABw4a2fNDjcLgd7C7dzcbCjWws3Eh+dT4RfhH4Gf2osFewv2I/1Q7vR/cNOgOTkydzYecL6RfVDx/9/wp5m9PGV3u/wul2cmWPK/H38W/ptyREuyKFUBORQujYXG4X72x7h7e2voVCkRSSxDPnPkPfyL6ndd7K9L2kvbeMfSVh2Mz144dQbgJVJdHROvpPTiGud0yrvUrQXjnsLnb8kket1UFgqInyQivZO0qpLLZ52oRY9hNi2Y/ZVkqws5iwCANBgwcSNG4c/kMGozNoczvU4XaQUZbBwaqDhPuFU+WoYtGBRfya9yvW359GO54wUxg9wntQXVdNmF8YMwbNaNQixUKI5iOFUBORQujE1uSv4ZFfH6HYVoxBZ+CG3jdwZ/87T/uvXUdZOTvmLGZ7uqLKz/u2QZDRSoeACjp0DaTDpAvQm3yxFNkwB/kQFtu2H5luCxx1LtxON75mI3W1Lg7uKmP1Z3uoKj96Rmejy0aHgyvpkL+S2InjiP7bX9EZDOj8/TUpZg/PrVNaW8q+in0sy17Gb4d+o9ZVe8z2wb7BDI4Z7BmvU2GvoNZZS5gpjLjAOHqG9cSgl/FsQrRGUgg1ESmETs5it/DUb0+xOGsxADH+MVzf63ou634ZIaaQ0zq3cruxpO/n4Mod7F17kAJzd9yG40+OFxaiSOofSUzXcKJ7RBEQapKrR6ep7FANFYVWXE432dtL2be5CJfDjY+vHkedC6j//vrVlhJRugO7bwimOgth5RmEl+/GLzyYyOl/IfSaa1r0Z6GUYnX+atbkr6FTUCf8jH58tOsjdpftPqptsG+wp9BxuV2MThjNxV0upld4L5mNWIjmZqsAvRFMgU16WimEmogUQg33S+4vPLPuGfJr8oH6ic8uSrqIq3tcTZ/IPqf9gaKcTkq+/YHsrcXkVQVRWqHH5lNfaPnVlmE3haJ+f6rlMF9VixkrOrsNXz8DwcmJRPfuSIeeoQRF1M9FUpFVTNHaHYR3j6Pjef3abeGk3Iqq8loqCqzYbU50Oh171heQubXkhMf52UqILtlCd+d2Ant1x3/gAHR+ZpylJZi6dSNozBh0Ps036L3WWcuqvFX8ll9/ZcfhduB0O8mqzGJv+d6j2hv1RiLNkUSbozm3w7mc3+l8uod1l4JHCC3krofPp0HiCLjs7SY9tRRCTUQKocapdday8MBCPsn4xOsv73C/cEZ2GMndA+8mJiCmSfpSdXWUL1qCo6AA37AQqvbmsH9bKWXOUKr846kJiINGfrgFUEVsnA+BQXpCk6II752Ev6EWfd4+zL2S8Ylu/PIirVGNxU7hgUpK8qqpKKihvNBKRYEVp+NY8/gogm356Ow2/K2FxB9aQ2BNPrWmUIL79iTm6ksIOv/8FpnJ2eqw8nPuz+RV53Go5hD7K/azu2w3NqftmO3NRjPjE8dTZCuiyFrEuM7juLbntYT6hTZ7ViHECdRWwrq3YcWzoFwQlgi3/Qz+4U3WhRRCTUQKoVOjlGJr8VY+3v0xP+f+7PmgCvIJYsbgGYztPJZwv6b7D/5IbpuNmt17KVifgd1lRBcajmXDViw7M6kM6kx5aHdcvz/l5lNXRYC7kkqfqOPedtO5XRjcdgy+BgxGPQblwuBrwGj2xWDUYzRAXI9wuo5IJDjCjMFHj9ulcLsVviYDOn3zXGVyudzsWVdIYVYl5iAfTGYjLqebOpuL6vJadDodCb3CCIowU5RdSWFmJQWZFqrL7Md5n078bcX4OKpQOgNmaxGdc5cSYC1E5+ODb5cuGMLD8OvVm9Arr2jSBUwPz1xs1BkptBayv2I/+yr2kVuVS7hfOL4GXz7c+SGltaVHHRsfEM8FnS8gyhyFUW/EoDMQ4BPA6ITRp317VghxmtxuOPAzbPsUrGWgN0DmKnDU1O/veyX86V/g17SfsVIINREphE6fw+UgrTiNf236F9tLtnu29wzryeXdL+fSrpcS6Nu094aPm6WwEOehQ7isVty2Wty1tZh7dMfUvTtVO/ew+/2lWCxurA5fqm06bD4h2E3hqNMYEKvDja/BhZ+PG18fhcupcDjBiQ9KryckUBESBC63DodLh8NtwOHSo9DjVjrcLjcul6ovrFwKp0MBiuBAhd2uqLGdyi0dRaC1gEBLFgHWAgKsBfhbC/GrLUWv3BhjYwkYcQ5+yb3Q+ZnwiY/Hf9CgZpnM0K3c/Hfnf3kj7Q1sTptnzavj6RDYgbNjzybaP5ouIV3oEdaDbqHd2u0tTSFaHVsFlO4HSy5krYKMxVB58Oh2kT1g5F/hrGugGf7/lUKoiTRbIVRXA/lp4LSBoxacteCwef/TWQt+oRCaAOZw8A0AH3P9P0MS6qvqNsTpdvLRro/4Zv83XmM3zEYzl3S5hGuSr6FHWA8NE3pTTif2AwcwREZh1/lTtXkrFT8uw+XWgcmMvbSCuqIS3EqPXe9Hka4D5WE9cetbdhJIn7pKYgvX49abcBr90LudGFy1mOwVOI1mSiP64vAJIKgql+DKTEIqMwmqysHosmMICcGvTx/8+vUjIGU4fr16oQ8IQGc0nrzj07CxYCOfZnyKzWmjrLbMq0CG+vl4Ogd3pmtoVzoHd6astowiaxGjOo7iyu5XyvILQrQ2LifkbYRN78OOL8B1xFVnUwj0vwbi+td/tkX3hk4pzVIAHSaFUBNptkKoaDe8OezUjzeHQdcLoEcqdBvbpPdVW0JFbQWLMhfxacanHLAc8GwfEDWAi5IuIikkiW6h3Yjyj9IwZeO47XbsWVk4a2px2urQOetQ9lpqsvKpziul1urCXgdGPx98/QzoqspxWyxYVAhWXSBGdx0GVy2G2ir0tkp01mpUrQ29TmHQ1Q93MugVBp0bZTJji+yCW+9D+J4V6KyV+A8biiEklOply3BbrZgHDCBo7AX4dumCMSIC5XLjLC3BnrEHdBA4ahR+ffqg0zf9IOFSWyk7S3dSYiuhsq6SPeV72Fm6E6hfk2pP+R6v9n4GP+47+z7GdR6HzWkjwhyB7wmeDhRCaKyuBsqzIHcd7P8ZMn+BWsv/9gfF1f/BHtMbelwEXc6r/0O+BUkh1ESarRCyHIQPJoHRD3z8fv+n2fufRlP9/VRLbv1/YHVWcFjBXuVdbev0EBANAVEQ1hmikqFzCnQ+t/7crZhSig0FG/gk4xOW5yzHpVxe+5NCkhgeN5zhccMZEjuEYF+5PXmkI9eRctfW4rZaMYY3T3GcU5lDsa0Yk8FEpiWTTYWbKK0txeV2UWGvoLCmkCJb0QnPYdQbubzb5fSO6I3dZefcDufSKbhTs+QVQhzB5aj/HDGH1V+RcdbVj9cxmKBoV/0VneLd4Kr7w8tR/886K9gr619H8guBHuNh6O3QcUjLv68jSCHURFrlGCGXEw5ugL1LYM+PUJR+7HZGM3QYBPEDodNw6DyiVV85KrYW883+b9hStIXcqlyyK7NxK++nmDoHdybGP4ZaVy3hpnCGxg0lMTgRt3LjUvWrVjuVE7fbTYQ5guTwZEJMIZ5FIkXDZFmyeGXzKxRZi+gd0ZvOwZ0xGUwsz1nO6vzVJz1eh46kkCQ6BHYg0DeQTkGd6BfZD5PRRHVdNX0j+8r6WkI0J7e7/g9nh62+yKnIgey1kLMGcjfUbzP6gY8/2MpOrQ+/0PpbXF3HQNfz6z9rWtGQDSmEmkhzFUKHLDamzt2AyajHz8dAVJCJpMgAfAx6qmodhAX40j06iO7RgSSE+2M40VNH1UVQmQ81xVC6Dwp2wP7lUJV/REMdxPSFxHOhz2WQMLRZ78+eLovdwsaCjaw9tJZ1h9aRVZl1Sucx6Ay4lIsgnyDiA+MJ8wvD3+hPZV0lhdZCzEYz8QG/b/fxJ686j0xLJkE+QXQM6kiRtYgDlgMYdAaCfIMINgUTYAygpLaEImsREX4RdArqREJwAh0CO6DX6XG6nTjcDpRSJIYk0i20G5X2SoptxejQYTKY6BHegzBTGGnFaWSUZdA7ojd9Ivtg0BlwK7dnpe/DquqqyKnMIdA3ED+DH5Y6Cw63gxj/GML9wtHr9JTYSvgl9xdKbCUMjhlMgE8AP+X8REFNAQlBCSQGJ9I5uDOhplCqHFUcqDjA5qLN5FTlYKm1oNfpCTeHsyZvDXXuo2eKhvpbWwlBCdicNqLN0ZwddzYJQQkYdUaCTcHE+MfQObgzQb6yPpwQzUYpqCmB6oL6caNQfzUndz3sX1b/OcApfLT7+EPPi6HLaPD1B4Pv7y+f+itGPn71430CIuqvKLViUgg1keYqhPYVVTH25ZUNamsy6ukQaiYqyERiRADdYwIJ8/fF5KOnU7g/PWKC8PM5ogpXCoozIH8zHNwI2f/f3p0Gx1GdCx//d88+mk37Zkm2bNnyDhjsKLlgElMhXMhNQt4KFbiBJJWQVEheZykS+JC9KnArCSGQhVRRN1CUs2CykHsJBGyWvGE1wgZsbGHZkiXL2qXZl57pPu+HtgbLlhdAtmTr+VVNaWa6e+bMHJ2ep59z+vSzdqrzSBVL4Pz/hNWfhMDsH4sznh3njdE3iOVieJ1eeuI9vDDwAmOZMXRNx6E7cGj2Tdd0+pJ99CX7ZrrYJ+R1eCdd3mEiaNPQqAvU0RBsIOgOEs/FaR9sp6CmPptqIrjKmTnUO9n5TeG9de/lquar6BjrYCgzRKaQoTHYyCdbP8m84LxpeY9zkpmHl/8bEv1wwfVQugBG3oTuf8GB5+x1Fr7fPpJWFliFybdgLVQuhfQI7Plf+0AHmJjBG3eJndktW2iPv9j/NLz2IHhC9utWLLZ/oEJ1s+roXEwDy7TPwtq+CTqfgMz4qW3n8tsn3DSshab32reyhfb/aD4NgRr71HXTeCvoOQdIIDRNTlcglMoV2N4TJZs3yeRNBmJZukZTKKUIeJwMJ3K8OZhk33CSXGGqSe7e4tA1FlUGWF4XYlldiOV1Yc5riOBzH7UTTA7ZO+O9j8MbD9sNAEBzQPlCqFpq9++2XjXt8znMlLgRJ1vI4tAcRHNR+pJ9xHIxMoUMAVeA6pJq0vk0/al+4kacpJGk0l/JosgikkaS3kQv5b5yWkpb0NCIG3HiRpxUPkWZt4xKXyVj2TF6E730xHuKs2q7dBdO3YmpTPaO7+VA/AART4QqfxWappEwEnTHulEoQu4QKypWsGt0F7Fc7ISfp9xbTqaQIWfmCHvCODUnI9mRSV2Iy8uXUx+oZ9vANlL5FBfPu5jWslb6kn0ciB+gO9ZNMp8k6A5S7a/m/KrzaS1rJeKJYCmLwfQg9YF6Lpl3ybndnZjP2F0DR35GIw3ZKOgusPIQ7bWDmP4dkB61x9+VLwJ/ub39oVcg1meP03N57QBk9/8ccdCh2UFL+ti5j07EdIfQ80k0deK2fyLK6UOrWmoHQ5mo/aNpJO3PsOBie5zioe32j6vDZX9mpwfKmu0graTCDq68IfAE7fueoH1z+e3Xy6ftifAk4JoeSsF4lz0mNJ+x982mASMd9gHt3seP+l/S7Hoy0nYQXbkYalbZ2Zym94EvYg+ROA0nRJwNJBCaJjM9Rsi0FAfH0/THsgzGs+wbTrFvOEkyWyBtFOgcSjKezh+znduhc0FThIZSPxG/iwsaS7l4cSUBz+HulmzcHhC3/QHoa5+8sdNrn4224v/YR5ge6eI4HZJGkv5UPwvCC3DqTixlMZQewqW7UCgOxA/Ql+wjnU+jazrratfRFGo65nXyVp5oNophGXgdXsp95YA9P49S6uy/KKhZAJQdbGRj9iDNYB043fYP/ODOw+vl7dN3h3bbR7/+ckgd7jaO9UE2hqpYTMFfievg8/YZL7oL5Q1jKTDzWdyF5LQUOaaFOeBqZpWxHYCscvGK1cIL1jIcmsV6/VVqtXEM5aCAjomDAg4UGo3aICWafTLEDquZXdaCYo5PA0q0DOXEadV7qdRijKkAfzTfj47FJa49VKpRQiqBWzOnLtx085XZp0Hruj0ANzFojz9pWGffcgn7ICw5aP9YL9pgjydBs2cUdgftYDR20P7xL2u2s16je+2MWe15s7oL/x0z83agU8hCz/PQucUOomO9J97OG4EVH7fn3qlddcbPxDqbSCA0TWY6EDoZpRQD8Sy7+uLsOhTnjf4Yrx2M0R879mraLodGY5mfBRUlrJoXYU1TKQsrA1SpUfSR3fYAup1/sndAE3QnzLvIPsJovhTq15wzaVNxGigFQ2/YwXRZ8+QfsGzczpSMvGkf1eaSh7MoZZjeUjoTLmJakILTjy/ZS2h8F/Wjz+I59BLaURMsmpqDpKuKkDGANk1dgRMKSsepWRTQ6bfK6VFV7FTzGVUhWrQ+GvUhwqRQwOtWM12qFgCflqWUJKOE+O/Ch4gToFEbpJw4u9R8PB4f/3FeHYlsgf997RCWArdTpy7sxeN0EPQ6qQ55SWayFPp3ciDt4qCqIuJ38YHWKlbPi1DicfJc5wiP7hzAUhbnlRWIlFXg9fr455vDxYMiHYsmbZAlWi8WGlEVIEYJOVxcoO3lQv1N+lQFr6gWUsqLiwIuzcRPloXaIVq0PsJaigAZglq6+DdIBq9mv4eJjqU5campx5JNm/JFdqbaMu0gODloB8XVyyHSZO+PPEGINNrdOol+e3mk6fBzZ3h/VTDszJtpHA7CD9rBzcTf6OH76eNcw8/hsbM8Tq8dCGqa/R1UL7enTGl8j+yDT5EEQtNktgdCU1FKsX8kxbauMUZTBoPxLP98c5ju0fSU6zt1DYeu4XboXNxSzn/Oj7M6ugX/vkfQxrsnr+wO2oOtmy+10+tlzXJEMlOUsjMkTo+94zdS9hG3N2IfZQ7utDMmZc1QtsBebyqWZe+Ux7rsHW+k0V43NWIf2VsWeAJYwXpMM48r2k1+71asjsfQjQSavwxHWROUt5De+Qglw3YWJBdsJFO9hhFnDeGxVykffhFdvfssRU458WhvBUa9ViU5XGgodqsmXrcWENJSlJJghDD9qpx+VU5SeWnVe6nRxnjFamG7tQgveYJaGpcOLbVlLGpeSFYv4f7nu0nm8qDptNaEuPr8euoiPu79135298dprgiwpCbI4uogzZUlVIe8BDxOCpZFMltgJGlgmBalfhelfjelJW4qAx7cTruL4lA0QzSdp6U6gMsxdbeFZSlSRgG/23nMyRIF00LXNPQjns/mTZ7bN4Lf7WRFfZjRZI6dfXFyBROloGcszf6RFBUBN82VAQ6OpXmjP46maTh1jc6hJD1jaaqCHhZXB0kbBQbjOYYTOQzzrS46FwW8GCTx4sBitbaPlXoXeZyklYchIig03qfvZInWS5QgwyrMsIrgJ8uHHNtYph0gjxMTHf/h7FfKVUoeN+H8EBqKlCOMUxl4rKmvI3dKPGFYepV9MKc77S48zWH/1R12V2akEdwBO0Pj9tvtZyKAtyy7q8o07O5Aq2AHOUbKbnuDO+1ByaXz7XE3u/9mj9cy32ZwGKqH5vdD67/b2TLZp04LCYSmydkYCB1PXzRD13CKzqEE7T1RdvSOcyiaxbSmrv6wz8X7ypNc5nmDC8xXqR/fhis3xeC8kkp74qxIoz0LdrjxiPsNZ+94o0zUvjZOJmrvGANVEJ4HqVH7VFRfBAJVqLFuCoN7MEwLAxfK5bMvUzGwHe/YHoadNbyp5hH2uanxgxcDzcySz6Yw8gWSzlJyzhAVaoyAGSWj+Uhrfpy6hksz0YwUzkIKn8rg0BRGZBEZzYdv8GUC5onHFE2wdDeHSpYyRBnVRg/B/ChOlcOl8rg4/uUs3omcctmXFZmia6ZfldFp1TFEhJTy4cWgVEsS1pKU60nKtBQBlWRYr6LL0cTWzGKeNFehl1Rw3dp6sloJe4az1DBCnTXA9kwVr4y5SWQLZPImYZ+LyoCHi+aX8p7mcnRdI1ewA5KKgIeKgAef21HsbtaAEo+TFXXhSWPqYpk8XSMpFlUF3upOngOMglUM1iYopYhnC5iWIm0U2D+c4sBoilzBImOY9EUzDMazeF0OvC4HedMibZgMJ3LEs3kCHidKQedwEqNg4XJolPpcoGmMpgywCjiw2w6ABwMfOaIEKSHDvzteZInWi9vjJ4mXrmwJHvIs1Xqo0ccp9zup92QpzQ/gUAW0YK3d5TZ+wJ65/+1yuO19mr/MbufZU2tjx5rYZzTY+42J/eHE41D94S/YsjNA52L33wyTQGianEuB0FTypsVIMoelYCSR439ePcTWPUMcGE1xdHykYbFMO8BVgQ4ucexkkbEHjzV1lmkSp9dOa2va4cGXYfs2MejSFzmctTicuQjW2ulhK293oegue6JIzQHxPvvIzVdqb/d2xr8Yafv1XD57/Iim2VmVvY9D+31QyKL8FRieUnKmhv+N3+M8yeDl2axPlTOmgszXBglqJ/5BsJTGIcoxlU6dNopLM4mqElJ4MZVOSEsT0ewLJA6pCDut+WxVazmoVRI048zXBmjR+zio1XBw0XUkLTdW979YovXS6hllxFXL/3P9G+H6JVyxspbasJdYJs/u/jgdAwmW14X56Pl1+N2Tg46MYbJ/JMnCysCxZ0aKs0rBtIhl8pT63cVMVn8sw+9f7OGN/ji1YR8Rv4uxlIFRsKiL+EjmCmzZPciBI7LZHqd9tux42mAkOTnzomng0nUqgx7OnxfiQ6EuLkr/k1BuAMssoGGhKwsdC10VcGTH0KI9dgZVd9oZn6M5vfaYpVzSDpLcJfbNE4DyFrvLamg39L5gD1R+7/+1hxDoDgluTiKbN3E59BNPD/MuSCB0lF/+8pf8+Mc/ZmBggNWrV3P33Xezdu3ak253rgdCx5PNm+wfTtE5nOTNgQS7++O80R8/auyRIkyKedoI9drw4b/2bZ42TL02Qqk2PYNPLXTQdPQjTh9XaBjOIIY7jOUtxamD24iCpmO4S8l7IhTcYVzpQfxju3EZ0eK2pu4i7wqha+Ce4mrmE9606tlmtaJjUa2NU6eNMq6CHFQVBLUM1do4faqCDmselu4k5DTxYKArk17nAg75F/PeijSrvUMcjBnsi5okTSc55SYSDlEd9hE2x3HlYnTnQxw0glR78pS7DNIFi1wBdF+QgqOErqTOeCLNvMJByhwpPPPXUbv4QjJGnn0DMZ7qSjGWyvPBRfY4sPYheHMwQX8sw3xtiGtremkJFoiWzCfnryMcCuHy+EiaLuKWl3heI20USGVzuDSNspAfv9uJpRQRv5ulZRAu8ZLFi9elE/a50DSNXMEkkS2QyBaoDnmOCWaEeLfGUgadQ0lMS3F+Y6QYFHePpHh05wD/6hym/cA42fzbO8uuKujh8mXVlJa42T+SwsxlKNfjrI4YfKBRo7y6wZ57bZaMycnmTbpGUvjdDkpL3IS8k8tVMC36Y1kchzOh+4aSjCRzlJa4qQp6WFgVKG6TNy06BhJk8ybnNURwHtFFOxjPMpLMEfA4qQh4KDmcFc0VTPYNpdg7lKBgKuZX+DEKio6BOOm8SdDjpCbsY2ltkGzeYtehGIlsAU2DdM5kLG3gctj7juc6R3j6zWEqAx4+d/ECPrm2sfg+00UCoSP88Y9/5Prrr+eee+5h3bp13HnnnWzevJmOjg6qqqpOuO1cDYSOZzxlsHsgzr6hJHuHkuwdTNI7niaZK5DLWwS8Tpy6xkgyR95UlJChVEuSVw50FEEtTYgUocMDMH2aQTkx5muDNOmDLNAGKCeGQ1OYSiNKAA95ApodgBnKQQ73STMcx2MoxzFdNknlZZO5gTetBsq0OOVanDI9zRuulbxY8n6CJV4iPhdhn4uI30VLVZBldSECHiemUpS4nYR9LrwufVaebn70JTiEOBcZBYto2iBvKQ6MptjRG2V7T5QdvVFimTzew11+uYJ10ilJwE7mRHwu8qbCMC3ypkXY56I27KM27KUmbO8X/G4Hg/EcfdEMi6oCrF9cScdAghf2j1Jf6mPdgjLShkn3aJoDoyn6o1mqQh4ayvxE03n6Yxn6o1lGUzlqwl5qQj76ohkORTMEPE7KStxE/Hbwsq17bFKwF/G7mF9ewvxyP7qu8dSeoSnPIj5SxO/C5dCJZ/LF76GsxM0FjRFSOZMDoykOHXWyzbxSH26nzoHR9HGHUrxbFQE3T9/8/mntipZA6Ajr1q3joosu4he/+AUAlmXR0NDAV77yFW655ZYTbiuB0DujlCKRK5DNm8TSeQ5GMwzHc2QLJhnDnjspkzfJGia5goWlFJm8nToHmBd2E/C6yOQVqVweV2YEw8hxyAyD7qTCr1OqpXDnY+jZcbT0GLGcSW/WhxOLWneGCkeKsIqT0ILscy6k31FDhhIiXmh0J9CNBKlUknSwmUWNdSyvC7GiPkx9xCfdMEKcw5RSZPImL3aNseWNQUxL0VxZQsDjInW4O+7Frnd42YnTLOh1UjDt8k/FfTizo+vQXBGgOuQhmslzKJphMD75ivBBrz0QP3pU8KRrUFbiIZUrHPM+Ia+TJTVBXA47MNJ1aK0JEfa5SGTzHBhNs284iUPXWFYboiroxVTKzmL53eRNi7GUwYKKEv7jvDq290S555l9rJ4X4a5Pnj+N35QEQkWGYeD3+3nooYf46Ec/Wnz+hhtuIBqN8vDDD09aP5fLkcu99c8Sj8dpaGiQQEgIIeaQwXiWeCaPy6Hjcuo4DwcMh2IZBmJZ+mP28rRRoCLgoTbs5eUD47ywf5T55SVcuqSK3vE0rxwYp9TvZn6Fn6byEmrDXgbjWQ6OZ4j43dRHvNSGfZSVuDkUzdAfy1If8dFQ5idtFBhPG4yl8uQKJmuaSllSHUTTNFK5AgcOZ5m6RlMkswX+raWCtfPLJnVzHSmWyTMYz1IwFT63g6YyP6ZSvLB/lO6RFCGfi6qgl5XzwsXMzHjKYM9AgoJlsbg6SFXQc9Lscv7wWY2nOvanYFqkciZh//R2Qb6dQOic7tAfGRnBNE2qq6snPV9dXc2ePXuOWf+2227j+9///pkqnhBCiFmoOuSlOuQ95rklNcefYPZTbfPf1XuuqA+f8rolHifLDl9N4FSFD3fxH0lH4+KWSi5umfoyS6UlbtoWlp/yewDHnRLieJwOnbB/Zme/nptzbx/HrbfeSiwWK956e08yy6cQQgghzmrndEaooqICh8PB4ODgpOcHBwepqak5Zn2Px4PHc5yJ54QQQghxzjmnM0Jut5s1a9awdevW4nOWZbF161ba2tpmsGRCCCGEmA3O6YwQwNe//nVuuOEGLrzwQtauXcudd95JKpXiM5/5zEwXTQghhBAz7JwPhK655hqGh4f5zne+w8DAAOeddx6PPfbYMQOohRBCCDH3nNOnz79bMo+QEEIIcfZ5O7/f5/QYISGEEEKIE5FASAghhBBzlgRCQgghhJizJBASQgghxJwlgZAQQggh5iwJhIQQQggxZ0kgJIQQQog5SwIhIYQQQsxZ5/zM0u/GxFyT8Xh8hksihBBCiFM18bt9KnNGSyB0AolEAoCGhoYZLokQQggh3q5EIkE4HD7hOnKJjROwLItDhw4RDAbRNG2mi3PWiMfjNDQ00NvbK5cmmWFSF7OH1MXsIXUxe5yuulBKkUgkqKurQ9dPPApIMkInoOs68+bNm+linLVCoZDsZGYJqYvZQ+pi9pC6mD1OR12cLBM0QQZLCyGEEGLOkkBICCGEEHOWBEJi2nk8Hr773e/i8XhmuihzntTF7CF1MXtIXcwes6EuZLC0EEIIIeYsyQgJIYQQYs6SQEgIIYQQc5YEQkIIIYSYsyQQEkIIIcScJYGQOCW//vWvWbVqVXHSq7a2Nh599NHi8mw2y0033UR5eTmBQICPf/zjDA4OTnqNnp4errzySvx+P1VVVdx8880UCoUz/VHOeieri0svvRRN0ybdvvjFL056DamL0+P2229H0zS++tWvFp+TtnHmTVUP0i7OnO9973vHfNetra3F5bOtTcjM0uKUzJs3j9tvv52WlhaUUtx///185CMfYfv27Sxfvpyvfe1rPPLII2zevJlwOMyXv/xlrr76ap599lkATNPkyiuvpKamhueee47+/n6uv/56XC4XP/rRj2b4051dTlYXAJ///Of5wQ9+UNzG7/cX70tdnB7btm3jN7/5DatWrZr0vLSNM+t49QDSLs6k5cuXs2XLluJjp/OtcGPWtQklxDtUWlqq7r33XhWNRpXL5VKbN28uLtu9e7cC1PPPP6+UUurvf/+70nVdDQwMFNf59a9/rUKhkMrlcme87OeaibpQSqn169erjRs3HnddqYvpl0gkVEtLi3riiScmff/SNs6s49WDUtIuzqTvfve7avXq1VMum41tQrrGxNtmmiZ/+MMfSKVStLW10d7eTj6f57LLLiuu09raSmNjI88//zwAzz//PCtXrqS6urq4zuWXX048HmfXrl1n/DOcK46uiwmbNm2ioqKCFStWcOutt5JOp4vLpC6m30033cSVV145qQ0A0jbOsOPVwwRpF2fO3r17qauro7m5meuuu46enh5gdrYJ6RoTp+z111+nra2NbDZLIBDgL3/5C8uWLWPHjh243W4ikcik9aurqxkYGABgYGBg0j/1xPKJZeLtOV5dAFx77bU0NTVRV1fHa6+9xre+9S06Ojr485//DEhdTLc//OEPvPLKK2zbtu2YZQMDA9I2zpAT1QNIuziT1q1bx3333ceSJUvo7+/n+9//PhdffDE7d+6clW1CAiFxypYsWcKOHTuIxWI89NBD3HDDDTzzzDMzXaw56Xh1sWzZMm688cbieitXrqS2tpYNGzawb98+Fi5cOIOlPvf09vayceNGnnjiCbxe70wXZ846lXqQdnHmXHHFFcX7q1atYt26dTQ1NfHggw/i8/lmsGRTk64xccrcbjeLFi1izZo13HbbbaxevZqf//zn1NTUYBgG0Wh00vqDg4PU1NQAUFNTc8xZAROPJ9YRp+54dTGVdevWAdDZ2QlIXUyn9vZ2hoaGuOCCC3A6nTidTp555hnuuusunE4n1dXV0jbOgJPVg2max2wj7eLMiUQiLF68mM7Ozln5eyGBkHjHLMsil8uxZs0aXC4XW7duLS7r6Oigp6enOG6lra2N119/naGhoeI6TzzxBKFQqNilI965ibqYyo4dOwCora0FpC6m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",
@@ -621,15 +547,15 @@
             ],
             "source": [
                 "tit0.plot()"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 24,
+            "execution_count": 21,
             "metadata": {
                 "scrolled": true
             },
             "outputs": [
                 {
                     "data": {
                         "image/png": "iVBORw0KGgoAAAANSUhEUgAAAjkAAAGwCAYAAABLvHTgAAAAOXRFWHRTb2Z0d2FyZQBNYXRwbG90bGliIHZlcnNpb24zLjcuMSwgaHR0cHM6Ly9tYXRwbG90bGliLm9yZy/bCgiHAAAACXBIWXMAAA9hAAAPYQGoP6dpAAEAAElEQVR4nOzdeViUVfvA8e+wgwqobCKIuIK7YiqammlORmavVqaVpqZpWLmkZW9pb/3U0qy0XCpJtFypbFHT3KUkFxAVEEXZFB1UVtmXOb8/JiYnthkWB/B8rmsuZp7nPOfc4zUyN+c5i0IIIZAkSZIkSWpgTIwdgCRJkiRJUm2QSY4kSZIkSQ2STHIkSZIkSWqQZJIjSZIkSVKDJJMcSZIkSZIaJJnkSJIkSZLUIMkkR5IkSZKkBsnM2AEYk1qt5vr16zRp0gSFQmHscCRJkiRJ0oMQgjt37uDq6oqJSfn9Nfd1knP9+nXc3d2NHYYkSZIkSVVw9epV3Nzcyj1/Xyc5TZo0ATT/SLa2tkaORpIkSZIkfWRmZuLu7q79Hi/PfZ3klNyisrW1lUmOJEmSJNUzlQ01kQOPJUmSJElqkGSSI0mSJElSgySTHEmSJEmSGqT7ekyOJDVExcXFFBYWGjsMqQ4xNzfH1NTU2GFI0j0nkxxJaiCEEKhUKtLT040dilQH2dvb4+LiItcEk+4rMsmRpAaiJMFxcnLCxsZGfplJgCb5zcnJ4ebNmwC0aNHCyBFJ0r0jkxxJagCKi4u1CU7z5s2NHY5Ux1hbWwNw8+ZNnJyc5K0r6b4hBx5LUgNQMgbHxsbGyJFIdVXJZ0OO15LuJzLJkaQGRN6iksojPxvS/UgmOZIkSZIkNUgGJTnvvfceCoVC5+Hl5aU9n5eXh7+/P82bN6dx48aMGTOG5ORknToSExPx8/PDxsYGJycn5s2bR1FRkU6ZI0eO0KtXLywtLWnXrh2BgYGlYlm9ejWtW7fGysqKvn37cvLkSUPeiiRJkiRJDZzBPTmdO3fmxo0b2scff/yhPTd79mx+/fVXgoKCOHr0KNevX2f06NHa88XFxfj5+VFQUMDx48fZuHEjgYGBLFy4UFsmLi4OPz8/hgwZQnh4OLNmzeKll15i37592jLbt29nzpw5LFq0iLCwMLp3745SqdTOHpAkSZIkSUIYYNGiRaJ79+5lnktPTxfm5uYiKChIe+zChQsCECEhIUIIIfbs2SNMTEyESqXSllm7dq2wtbUV+fn5Qggh5s+fLzp37qxT99ixY4VSqdS+7tOnj/D399e+Li4uFq6urmLp0qWGvB2RkZEhAJGRkWHQdZJU1+Tm5oqoqCiRm5trtBgmTpwogFL/D3fu3CkM/FVT4+Li4gQgHB0dRWZmps657t27i0WLFhknsHuoLnxGpPtLZFKGSM8pqJW69f3+NrgnJyYmBldXV9q0acNzzz1HYmIiAKGhoRQWFjJs2DBtWS8vL1q1akVISAgAISEhdO3aFWdnZ20ZpVJJZmYmkZGR2jJ311FSpqSOgoICQkNDdcqYmJgwbNgwbZny5Ofnk5mZqfOQJKnmWFlZ8dFHH5GWlmbsUMp0584dPv74Y2OHIUkNnhCCcV//Rff//c5F1R2jxWFQktO3b18CAwPZu3cva9euJS4ujoEDB3Lnzh1UKhUWFhbY29vrXOPs7IxKpQI0i5XdneCUnC85V1GZzMxMcnNzuX37NsXFxWWWKamjPEuXLsXOzk77cHd3N+TtS5JUiWHDhuHi4sLSpUvLLfPDDz/QuXNnLC0tad26NStWrNA537p1a5YsWcLkyZNp0qQJrVq14quvvtIpc/XqVZ555hns7e1p1qwZo0aNIj4+vtL4Xn31VT755JMKb22npaUxYcIEmjZtio2NDSNGjCAmJkZ7PjAwEHt7e/bt24e3tzeNGzfm0Ucf5caNGzr1rF+/Hm9vb6ysrPDy8mLNmjWVxidJDcX1jDwycgsxM1HQ2sF4S1sYlOSMGDGCp59+mm7duqFUKtmzZw/p6ens2LGjtuKrUQsWLCAjI0P7uHr1qrFDkqQGxdTUlCVLlvD5559z7dq1UudDQ0N55plnePbZZzl//jzvvfce7777bqnJBStWrKB3796cOXOGV155hRkzZnDx4kVAs86LUqmkSZMmBAcH8+eff2oTjYKCggrjGzduHO3ateP9998vt8yLL77I6dOn+eWXXwgJCUEIwWOPPaazvkxOTg4ff/wx3377LceOHSMxMZE33nhDe37z5s0sXLiQxYsXc+HCBZYsWcK7777Lxo0b9flnlKR678J1zZ2Sdk6NsTQz3uKT1ZpCbm9vT4cOHbh8+TIuLi4UFBSU2jcnOTkZFxcXAFxcXErNtip5XVkZW1tbrK2tcXBwwNTUtMwyJXWUx9LSEltbW52HJEk16z//+Q89evRg0aJFpc598sknDB06lHfffZcOHTrw4osvMnPmTJYvX65T7rHHHuOVV16hXbt2vPnmmzg4OHD48GFAM/FArVazfv16unbtire3Nxs2bCAxMZEjR45UGJtCoeDDDz/kq6++4sqVK6XOx8TE8Msvv7B+/XoGDhxI9+7d2bx5M0lJSfz000/acoWFhaxbt47evXvTq1cvZs6cycGDB7XnFy1axIoVKxg9ejSenp6MHj2a2bNn8+WXXxrwLylJ9VfUDU2S06mFcb9nq5XkZGVlceXKFVq0aIGPjw/m5uY6/9EvXrxIYmIivr6+APj6+nL+/HmdruL9+/dja2tLp06dtGXurqOkTEkdFhYW+Pj46JRRq9UcPHhQW0aSJOP66KOP2LhxIxcuXNA5fuHCBQYMGKBzbMCAAcTExFBcXKw91q1bN+1zhUKBi4uL9vfG2bNnuXz5Mk2aNKFx48Y0btyYZs2akZeXV2bi8m9KpZIHH3yQd999t9S5CxcuYGZmRt++fbXHmjdvTseOHXXei42NDW3bttW+btGihTa+7Oxsrly5wpQpU7TxNW7cmP/7v//TKz5Jaggu/J3keBs5yTFo76o33niDkSNH4uHhwfXr11m0aBGmpqaMGzcOOzs7pkyZwpw5c2jWrBm2tra8+uqr+Pr60q9fPwCGDx9Op06deOGFF1i2bBkqlYp33nkHf39/LC0tAZg+fTpffPEF8+fPZ/LkyRw6dIgdO3awe/dubRxz5sxh4sSJ9O7dmz59+vDZZ5+RnZ3NpEmTavCfRpKkqho0aBBKpZIFCxbw4osvGny9ubm5zmuFQoFarQY0f1z5+PiwefPmUtc5OjrqVf+HH36Ir68v8+bNMzi28uITQmjjA/j66691kiVA7hkl3Te0PTmu9SjJuXbtGuPGjSMlJQVHR0cefPBB/vrrL+0vlk8//RQTExPGjBlDfn4+SqVSZ7Cdqakpu3btYsaMGfj6+tKoUSMmTpyoc3/c09OT3bt3M3v2bFauXImbmxvr169HqVRqy4wdO5Zbt26xcOFCVCoVPXr0YO/evaUGI0uSZDwffvghPXr0oGPHjtpj3t7e/Pnnnzrl/vzzTzp06KB3AtCrVy+2b9+Ok5NTlW859+nTh9GjR/PWW2/pHPf29qaoqIgTJ07Qv39/AFJSUrh48aK2t7kyzs7OuLq6Ehsby3PPPVel+CSpPsvKLyIhJQeoZz0527Ztq/C8lZUVq1evZvXq1eWW8fDwYM+ePRXW89BDD3HmzJkKy8ycOZOZM2dWWEaSJOPp2rUrzz33HKtWrdIemzt3Lg888AAffPABY8eOJSQkhC+++MKgmUfPPfccy5cvZ9SoUbz//vu4ubmRkJDAjz/+yPz583Fzc9OrnsWLF9O5c2fMzP75Ndi+fXtGjRrF1KlT+fLLL2nSpAlvvfUWLVu2ZNSoUXrH+L///Y/XXnsNOzs7Hn30UfLz8zl9+jRpaWnMmTNH73okqT6K/rsXx9nWkmaNLIwai9y7SpKkWvP+++9rbzOBphdmx44dbNu2jS5durBw4ULef/99g25p2djYcOzYMVq1asXo0aPx9vZmypQp5OXlaXt2jhw5gkKhqHBaeYcOHZg8eTJ5eXk6xzds2ICPjw+PP/44vr6+CCHYs2dPqVtUFXnppZdYv349GzZsoGvXrgwePJjAwEA8PT31rkOS6qsLdWTQMYBClNxIvg9lZmZiZ2dHRkaGnGkl1Wt5eXnExcXh6emJlZWVscMxug0bNrBkyRKioqIMSk4aMvkZke6VBT+eY+vJq7zyUFvmP+pV+QVVoO/3t+zJkSSpwdmzZw9LliyRCY4kGUHUDc0Kx8YejwMGjsmRJEmqD4KCgowdgiTdl9RqwUVV3Zg+DrInR5IkSZKkGnI1LYe8QjUWZiZ4OjQydjgyyZEkSZIkqWaUbMbZ1rExpiYKI0cjkxxJkiRJkmpIzE3NYpgdnRsbORINmeRIkiRJklQjLiVrenLaOzcxciQaMsmRJEmSJKlGXErW9OR0kEmOJEmSJEkNRbFacOVWSZIjb1dJkiQBmv2hnJycKlyhuCGKiorCzc2N7OxsY4ciSdWWkJJNQZEaK3MT3JvaGDscQCY5kiTVAYsXL2bUqFG0bt1aeywxMRE/Pz9sbGxwcnJi3rx5FBUVVVhPamoqzz33HLa2ttjb2zNlyhTtruCGyMzM5L///S9eXl5YWVnh4uLCsGHD+PHHH7W7jQshWLhwIS1atMDa2pphw4YRExNT6n31798fGxsb7O3tS7XTqVMn+vXrxyeffGJwjJJU12jH4zg1waQOzKwCmeRIkmRkOTk5BAQEMGXKFO2x4uJi/Pz8KCgo4Pjx42zcuJHAwEAWLlxYYV3PPfcckZGR7N+/n127dnHs2DGmTZtmUDzp6en079+fTZs2sWDBAsLCwjh27Bhjx45l/vz5ZGRkALBs2TJWrVrFunXrOHHiBI0aNUKpVOrshVVQUMDTTz/NjBkzym1v0qRJrF27ttIETpLqupLxOO3ryK0qAMR9LCMjQwAiIyPD2KFIUrXk5uaKqKgokZuba+xQDBYUFCQcHR11ju3Zs0eYmJgIlUqlPbZ27Vpha2sr8vPzy6wnKipKAOLUqVPaY7/99ptQKBQiKSlJ73hmzJghGjVqVOY1d+7cEYWFhUKtVgsXFxexfPly7bn09HRhaWkptm7dWuq6DRs2CDs7uzLby8/PF5aWluLAgQN6x1gV9fkzItUP/ptDhcebu8TaI5drvS19v79lT44kNVBCCHIKiozyEAbs+xscHIyPj4/OsZCQELp27Yqzs7P2mFKpJDMzk8jIyDLrCQkJwd7ent69e2uPDRs2DBMTE06cOKFXLGq1mm3btvHcc8/h6upa6nzjxo0xMzMjLi4OlUrFsGHDtOfs7Ozo27cvISEherVVwsLCgh49ehAcHGzQdZJU18Qkl6yRUzdmVoHcu0qSGqzcwmI6LdxnlLaj3ldiY6Hfr5eEhIRSCYVKpdJJcADta5VKVWY9KpUKJycnnWNmZmY0a9as3Gv+7fbt26SlpeHlVfHOySX1lRWjvm3dzdXVlYSEBIOvk6S6oqBITeztune7SvbkSJJkVLm5uVhZWRk7DACDeqBqkrW1NTk5OUZpW5JqQszNOxQWC2ytzGhpb23scLRkT44kNVDW5qZEva80Wtv6cnBwIC0tTeeYi4sLJ0+e1DmWnJysPVcWFxcXbt68qXOsqKiI1NTUcq/5N0dHR+zt7YmOjq6wXEl9ycnJtGjRQifGHj166NXW3VJTU2nbtq3B10lSXRF1XbPzeCdXWxSKujGzCmRPjiQ1WAqFAhsLM6M8DPkl17NnT6KionSO+fr6cv78eZ2kZf/+/dja2tKpU6cy6/H19SU9PZ3Q0FDtsUOHDqFWq+nbt69esZiYmPDss8+yefNmrl+/Xup8VlYWRUVFeHp64uLiwsGDB7XnMjMzOXHiBL6+vnq1dbeIiAh69uxp8HWSVFdE3fg7yWlhZ+RIdMkkR5Iko1IqlURGRur05gwfPpxOnTrxwgsvcPbsWfbt28c777yDv78/lpaWAJw8eRIvLy+SkpIA8Pb25tFHH2Xq1KmcPHmSP//8k5kzZ/Lss8+WOYi4PIsXL8bd3Z2+ffuyadMmoqKiiImJ4ZtvvqFnz55kZWWhUCiYNWsW//d//8cvv/zC+fPnmTBhAq6urjz55JPauhITEwkPDycxMZHi4mLCw8MJDw/XWbsnPj6epKQknUHMklTf3N2TU6fU+jyvOkxOIZcaivo+PbhPnz5i3bp1Osfi4+PFiBEjhLW1tXBwcBBz584VhYWF2vOHDx8WgIiLi9MeS0lJEePGjRONGzcWtra2YtKkSeLOnTs69QJiw4YNFcaTnp4u3nrrLdG+fXthYWEhnJ2dxbBhw8TOnTuFWq0WQgihVqvFu+++K5ydnYWlpaUYOnSouHjxok49EydOFECpx+HDh7VllixZIpRKpQH/WlVT3z8jUt2lVqtFl0V7hcebu0Rk0r35PtX3+1shhJFG2tUBmZmZ2NnZkZGRga1tHcs+JckAeXl5xMXF4enpWWcG8Rpi9+7dzJs3j4iICExMaq+DOS4ujg4dOhAVFUX79u1rrR19FRQU0L59e7Zs2cKAAQNqta36/hmR6q6rqTkMXHYYc1MFkf97FAuz2r9JpO/3txx4LEmS0fn5+RETE0NSUhLu7u611s6ePXuYNm1anUhwQHM76+233671BEeSalPJeJwOzk3uSYJjCJnkSJJUJ8yaNavW2/D396/1NgzRrl072rVrZ+wwJKlatONxWtS9OyJ1K+WSJEmSJKle0c6sqmuDjpFJjiRJkiRJ1SB7ciRJkiRJanByCopISs8FoH0d2rOqhExyJEmSJEmqkvjbmu1I7G3MadbIwsjRlCaTHEmSJEmSqiTudjYAbRwaGTmSsskkR5IkSZKkKom9pVm929Oh7uw8fjeZ5EiSJEmSVCXanhxH2ZMjSZJUppSUFJycnIiPjzd2KPdUVFQUbm5uZGdnGzsUSaqSK/J2lSRJUsUWL17MqFGjaN26tc7xwMBAunXrhpWVFU5OThUu5hcfH49CoSjzERQUZFA8BQUFLFu2jO7du2NjY4ODgwMDBgxgw4YNFBYWasutXr2a1q1bY2VlRd++fTl58qT2XGpqKq+++iodO3bE2tqaVq1a8dprr5GRkaEt06lTJ/r168cnn3xiUHySVBcIIYgruV1VR3ty5IrHkiQZVU5ODgEBAezbt0/n+CeffMKKFStYvnw5ffv2JTs7u8KeHnd3d27cuKFz7KuvvmL58uWMGDFC73gKCgpQKpWcPXuWDz74gAEDBmBra8tff/3Fxx9/TM+ePenRowfbt29nzpw5rFu3jr59+/LZZ5+hVCq5ePEiTk5OXL9+nevXr/Pxxx/TqVMnEhISmD59OtevX+f777/Xtjdp0iSmTp3KggULMDOTv5Kl+iM1u4DMvCIUCmjdvG4mOXIXcrkLudQA1OcdpoOCgoSjo6POsdTUVGFtbS0OHDhQrbp79OghJk+ebNA1H330kTAxMRFhYWGlzhUUFIisrCwhhGbndH9/f+254uJi4erqKpYuXVpu3Tt27BAWFhY6u6nn5+cLS0vLar/XytTnz4hUN52MSxEeb+4S/ZcevOdt6/v9LW9XSVJDJQQUZBvnIYTeYQYHB+Pj46NzbP/+/ajVapKSkvD29sbNzY1nnnmGq1ev6l1vaGgo4eHhTJkyRe9rADZv3sywYcPo2bNnqXPm5uY0atSIgoICQkNDGTZsmPaciYkJw4YNIyQkpNy6S3ZMvrvHxsLCgh49ehAcHGxQnJJkbHG36vagY5C3qySp4SrMgSWuxmn77etgod8vvoSEBFxddeOMjY1FrVazZMkSVq5ciZ2dHe+88w6PPPII586dw8Ki8kXHAgIC8Pb2pn///gaFHhMTw0MPPVRhmdu3b1NcXIyzs7POcWdnZ6Kjo8u95oMPPmDatGmlzrm6upKQkGBQnJJkbLF/Dzr2rKODjkEOPJYkychyc3OxsrLSOaZWqyksLGTVqlUolUr69evH1q1biYmJ4fDhw3rVuWXLFoN7cUAzmLKmZWZm4ufnR6dOnXjvvfdKnbe2tiYnJ6fG25Wk2lSyRk5dnVkFsidHkhoucxtNj4qx2taTg4MDaWlpOsdatGgBaGYflXB0dMTBwYHExMRK6/z+++/JyclhwoQJesdRokOHDuX2xtwds6mpKcnJyTrHk5OTcXFx0Tl2584dHn30UZo0acLOnTsxNzcvVV9qaipt27Y1OFZJMiZtT45j3VwIEGRPjiQ1XAqF5paRMR4Khd5h9uzZk6ioKJ1jAwYMAODixYvaY6mpqdy+fRsPD49K6wwICOCJJ57A0dFR7zhKjB8/ngMHDnDmzJlS5woLC8nOzsbCwgIfHx8OHjyoPadWqzl48CC+vr7aY5mZmQwfPhwLCwt++eWXUj1WJSIiIsocAyRJdVVmXqG2J8fLpe5tzFlCJjmSJBmVUqkkMjJSpzenQ4cOjBo1itdff53jx48TERHBxIkT8fLyYsiQIQAkJSXh5eWlszYNwOXLlzl27BgvvfRSleKZNWsWAwYMYOjQoaxevZqzZ88SGxvLjh076NevHzExMQDMmTOHr7/+mo0bN3LhwgVmzJhBdnY2kyZNAv5JcLKzswkICCAzMxOVSoVKpaK4uFjbXnx8PElJSTqDmCWprgtNSEMtwKO5Dc62ZSfvdYG8XSVJklF17dqVXr16sWPHDl5++WXt8U2bNjF79mz8/PwwMTFh8ODB7N27V3u7p7CwkIsXL5Yay/LNN9/g5ubG8OHDy2yvdevWvPjii2WOjQGwtLRk//79fPrpp3z55Ze88cYb2NjY4O3tzWuvvUaXLl0AGDt2LLdu3WLhwoWoVCp69OjB3r17tYORw8LCOHHiBADt2rXTaSMuLk678OHWrVsZPny4Xj1UklRXnIxLBaBP62ZGjqRiClEbo+zqiczMTOzs7LTTOiWpvsrLyyMuLg5PT89yb4nUZbt372bevHlERERgYlJ7Hcw5OTk0b96c3377rdIZVPdCQUEB7du3Z8uWLdpbdLWlvn9GpLpl9Jo/CUtM5+Onu/OUj9s9b1/f72/ZkyNJktH5+fkRExNDUlIS7u7utdbO4cOHefjhh+tEggOQmJjI22+/XesJjiTVpNyCYs5d02xP0tezbvfkyCRHkqQ6YdasWbXehp+fH35+frXejr7atWtX6laWJNV1ZxLTKFILWthZ4dbU2tjhVEgOPJYkSZIkSW9/lYzH8WyGwoCZlMYgkxxJkiRJkvR2Mi4FgL6ezY0cSeVkkiNJkiRJkl6y8osIS0gHoG+buj0eB2SSI0mSJEmSnoIv3aKgWE3r5jZ1ejuHEjLJkSRJkiRJL/svaLYyGebtXOfH44BMciRJkiRJ0kOxWnDk4i0Ahno7Gzka/cgkR5IkSZKkSp1JTCM1uwBbKzN6t25q7HD0IpMcSZKMLiUlBScnJ+Lj440dSp2zbt06Ro4caewwJEl7q+qhjk6Ym9aP9KF+RClJUoO2ePFiRo0apd3PCeC1117Dx8cHS0tLevToUeqaixcvMmTIEJydnbGysqJNmza88847FBYWlttOSkoKjz76KK6urlhaWuLu7s7MmTPJzMw0OGaVSsWrr75KmzZttHWNHDlSZ2fyvLw8/P39ad68OY0bN2bMmDEkJycbFM/kyZMJCwsjODjY4BglqaYIITgQ9fd4nE7141YVyBWPJUkyspycHAICAti3b1+pc5MnT+bEiROcO3eu1Dlzc3MmTJhAr169sLe35+zZs0ydOhW1Ws2SJUvKbMvExIRRo0bxf//3fzg6OnL58mX8/f1JTU1ly5YtesccHx/PgAEDsLe3Z/ny5XTt2pXCwkL27duHv78/0dHRAMyePZvdu3cTFBSEnZ0dM2fOZPTo0fz55596x2NhYcH48eNZtWoVAwcO1DtGSapJl5KzuHIrGwtTEx7q6GjscPQn7mMZGRkCEBkZGcYORZKqJTc3V0RFRYnc3Fxjh2KwoKAg4ejoWO75RYsWie7du+tV1+zZs8WDDz5oUPsrV64Ubm5uBl0zYsQI0bJlS5GVlVXqXFpamhBCiPT0dGFubi6CgoK05y5cuCAAERISYlA8R48eFRYWFiInJ8egOO9Wnz8jkvGt2BctPN7cJaYEnjJ2KEII/b+/ZU+OJDVQQghyi3KN0ra1mbXe00uDg4Px8fGpdpuXL19m7969jB49Wu9rrl+/zo8//sjgwYP1viY1NZW9e/eyePFiGjUqvU6Ivb09AKGhoRQWFjJs2DDtOS8vL1q1akVISAj9+vXTO57evXtTVFTEiRMn6szmotL9QwjBrvM3AHi8WwsjR2OYaiU5H374IQsWLOD111/ns88+AzT3oOfOncu2bdvIz89HqVSyZs0anJ3/uYeXmJjIjBkzOHz4MI0bN2bixIksXboUM7N/wjly5Ahz5swhMjISd3d33nnnHV588UWd9levXs3y5ctRqVR0796dzz//nD59+lTnLUlSg5FblEvfLX2N0vaJ8SewMbfRq2xCQgKurq5Vbqt///6EhYWRn5/PtGnTeP/99yu9Zty4cfz888/k5uYycuRI1q9fr3d7ly9fRgiBl5dXheVUKhUWFhbapKeEs7MzKpXKoHhsbGyws7MjISFB7zglqaZEq+4QeysbCzMThno7GTscg1R54PGpU6f48ssv6datm87x2bNn8+uvvxIUFMTRo0e5fv26zl9WxcXF+Pn5UVBQwPHjx9m4cSOBgYEsXLhQWyYuLg4/Pz+GDBlCeHg4s2bN4qWXXtK5Z799+3bmzJnDokWLCAsLo3v37iiVSm7evFnVtyRJkhHk5uZiZWVV5eu3b99OWFgYW7ZsYffu3Xz88ceVXvPpp58SFhbGzz//zJUrV5gzZ47e7QkhqhxrdeKxtrYmJyenxtuWpMrsPqfpxXmogyNNrMyNHI2BqnIv7M6dO6J9+/Zi//79YvDgweL1118XQuh3D3rPnj3CxMREqFQqbZm1a9cKW1tbkZ+fL4QQYv78+aJz5846bY4dO1YolUrt6z59+gh/f3/t6+LiYuHq6iqWLl2q9/uQY3KkhqKs8RZqtVpkF2Qb5aFWq/WOffz48WLcuHHlnjdkTM63334rrK2tRVFRkd7tBwcHC0Bcv35dr/IpKSlCoVCIJUuWVFju4MGDAtCO0SnRqlUr8cknnxgcj5WVlc7vVkPJMTlSVQ3/5KjweHOX+OnMNWOHoqXv93eVenL8/f3x8/PTudcMld+DBggJCaFr1646t6+USiWZmZlERkZqy/y7bqVSqa2joKCA0NBQnTImJiYMGzZMW6Ys+fn5ZGZm6jwkqaFSKBTYmNsY5WHIcu89e/YkKiqqRt6zWq2msLAQtVpt0DWg+f2gj2bNmqFUKlm9ejXZ2dmlzqenpwPg4+ODubm5zpTyixcvkpiYiK+vr0HxXLlyhby8PHr27KlXjJJUU+7kFXLp5h0ABrRzMHI0hjN4TM62bdsICwvj1KlTpc7pcw9apVLpJDgl50vOVVQmMzOT3Nxc0tLSKC4uLrNMydTNsixdupT//e9/+r1RSZLuCaVSyYIFC0hLS6Np039WUb18+TJZWVmoVCpyc3MJDw8HoFOnTlhYWLB582bMzc3p2rUrlpaWnD59mgULFjB27FjMzTVd6jt37mTBggXa3wt79uwhOTmZBx54gMaNGxMZGcm8efMYMGCAzho9lVm9ejUDBgygT58+vP/++3Tr1o2ioiL279/P2rVruXDhAnZ2dkyZMoU5c+bQrFkzbG1tefXVV/H19dUOOtY3nuDgYNq0aUPbtm2r948tSQY6dy0DIcCtqTUOjS2NHY7BDEpyrl69yuuvv87+/furdQ/dWBYsWKBzrzszMxN3d3cjRiRJUteuXenVqxc7duzg5Zdf1h5/6aWXOHr0qPZ1SS9GXFwcrVu3xszMjI8++ohLly4hhMDDw4OZM2cye/Zs7TUZGRlcvHhR+9ra2pqvv/6a2bNnk5+fj7u7O6NHj+att97SlomPj8fT05PDhw+XO5OpTZs2hIWFsXjxYubOncuNGzdwdHTEx8eHtWvXast9+umnmJiYMGbMGJ2JGIbEA7B161amTp1q4L+sJFVf+NV0AHq42xs1jioz5B7Yzp07BSBMTU21D0AoFAphamoqDhw4UOk96HfffbfU/fXY2FgBiLCwMCGEEAMHDtSO8ynxzTffCFtbWyGEEPn5+cLU1FTs3LlTp8yECRPEE088off7kWNypIaivo+32LVrl/D29hbFxcXGDkUcOnRI2Nvbi9TUVGOHIoQQIiIiQjg5OYn09PRq1VPfPyOScUwJPCU83twlvj52xdih6KiVMTlDhw7l/PnzhIeHax+9e/fmueee0z6v7B60r68v58+f15kFtX//fmxtbenUqZO2zN11lJQpqcPCwgIfHx+dMmq1moMHD1Z4r1uSpLrJz8+PadOmkZSUZOxQ2LNnD2+//bbOrTNjunHjBps2bcLOzs7YoUj3GSGEtienZyt7o8ZSVQbdrmrSpAldunTROdaoUSOaN2+uPV7ZPejhw4fTqVMnXnjhBZYtW4ZKpeKdd97B398fS0vN/b7p06fzxRdfMH/+fCZPnsyhQ4fYsWMHu3fv1rY7Z84cJk6cSO/evenTpw+fffYZ2dnZTJo0qVr/IJIkGcesWbOMHQIAy5cvN3YIOv49CUOS7pVrabnczsrHzERBZ9f6mWTX+IrHld2DNjU1ZdeuXcyYMQNfX18aNWrExIkTdRbw8vT0ZPfu3cyePZuVK1fi5ubG+vXrUSqV2jJjx47l1q1bLFy4EJVKRY8ePdi7d2+pwciSJEmSJBmupBfHu4UtVuamxg2mihRC1MLKVvVEZmYmdnZ2ZGRkYGtra+xwJKnK8vLyiIuLw9PTs15OCpBqn/yMSIb6YFcUAX/E8UI/Dz54skvlF9xD+n5/V3nFY0mSJEmSGiYhBCFXUoB6PLMKmeRIkiRJkvQvBy7cJOpGJlbmJgzq4GjscKpMJjmSJEmSJGkVqwXL92kW0Jw8wBPHJvVvEcASMsmRJEmSJEnr5/AkLiVnYWtlxsuD6vcq2zU+u0qSJEmSpPor4I84AKY/1BY7m2rsOr53ATRygJ4vQGOnGorOMLInR5Iko0tJScHJyYn4+Hhjh1LnrFu3jpEjRxo7DOk+cetOPpHXNZtXP9O7Gtse5WfBya/g4PtQmFtD0RlOJjmSJBnd4sWLGTVqlHZTyrNnzzJu3Djc3d2xtrbG29ublStXlrouPz+f//73v3h4eGBpaUnr1q355ptvym0nMDAQhUJR5uPuVdj1oVKpePXVV2nTpg2Wlpa4u7szcuRInZXY8/Ly8Pf3p3nz5jRu3JgxY8aQnJxcZn0pKSm4ubmhUCi0O5kDTJ48mbCwMIKDgw2KT5KqIjjmFgBdWtpWb0POxL9AXQT2raCpRw1FZzh5u0qSJKPKyckhICCAffv2aY+Fhobi5OTEd999h7u7O8ePH2fatGmYmpoyc+ZMbblnnnmG5ORkAgICaNeuHTdu3ECtVpfb1tixY3n00Ud1jr344ovk5eXh5KR/d3p8fDwDBgzA3t6e5cuX07VrVwoLC9m3bx/+/v7aXc9nz57N7t27CQoKws7OjpkzZzJ69Gj+/PPPUnVOmTKFbt26ldrawsLCgvHjx7Nq1SoGDhyod4ySVBXHLmmSnEHtqzmjKv7vpLz1oGpGVD0yyZEkyaj27NmDpaWldusX0PRe3K1NmzaEhITw448/apOcvXv3cvToUWJjY2nWrBmAtieoPNbW1lhbW2tf37p1i0OHDhEQEGBQzK+88goKhYKTJ0/SqFEj7fHOnTtrY8/IyCAgIIAtW7bw8MMPA7Bhwwa8vb3566+/dN7v2rVrSU9PZ+HChfz222+l2hs5ciSPPPIIubm5OvFLUk1SqwXBMbcBqj9tXJvkPFjNqKpH3q6SpAZKCIE6J8coD0MWUg8ODsbHx6fSchkZGdpkBuCXX36hd+/eLFu2jJYtW9KhQwfeeOMNcnP1v/+/adMmbGxseOqpp/S+JjU1lb179+Lv76+T4JSwt7cHNL1RhYWFOntPeXl50apVK0JCQrTHoqKieP/999m0aRMmJmX/Su7duzdFRUWcOHFC7zglyVBRNzJJyS6gkYUpvVpVY4PavEy4Hq55buQkR/bkSFIDJXJzudir8uShNnQMC0VhY6NX2YSEBFxdXSssc/z4cbZv366zSW9sbCx//PEHVlZW7Ny5k9u3b/PKK6+QkpLChg0b9Go7ICCA8ePHG9Q7cvnyZYQQeHl5VVhOpVJhYWGhTXpKODs7o1KpAM2YonHjxrF8+XJatWpFbGxsmXXZ2NhgZ2dHQkKC3nFKkqGO/n2ryretAxZm1egDSfwLRDE0bQ321Ri8XANkkiNJklHl5uZWuJdSREQEo0aNYtGiRQwfPlx7XK1Wo1Ao2Lx5M3Z2mh2SP/nkE5566inWrFlTaeISEhLChQsX+Pbbbw2Ktya3+1uwYAHe3t48//zzlZa1trYmJyenxtqWpLulZhew/dRVAAZ3cKheZfHHND9bG38MmUxyJKmBUlhb0zEs1Ght68vBwYG0tLQyz0VFRTF06FCmTZvGO++8o3OuRYsWtGzZUpvgAHh7eyOE4Nq1a7Rv377CdtevX0+PHj30ulV2t/bt26NQKLSDi8vj4uJCQUEB6enpOr05ycnJuLi4AHDo0CHOnz/P999/D/yTQDk4OPDf//6X//3vf9rrUlNTcXSsv8vrS3VXXmEx0zadJjE1h5b21ozsXnHPaqXi/9D8lEmOJEm1RaFQ6H3LyJh69uzJd999V+p4ZGQkDz/8MBMnTmTx4sWlzg8YMICgoCCysrJo3LgxAJcuXcLExAQ3N7cK28zKymLHjh0sXbrU4HibNWuGUqlk9erVvPbaa6XG5ZQkNT4+Ppibm3Pw4EHGjBkDwMWLF0lMTMTX1xeAH374QWcM0alTp5g8eTLBwcG0bfvPSrNXrlwhLy+Pnj17GhyvJFVm6Z4LnE5Io4mVGYGTHsDexqLqlRVkw42zmudGHo8DcuCxJElGplQqiYyM1OnNiYiIYMiQIQwfPpw5c+agUqlQqVTcunVLW2b8+PE0b96cSZMmERUVxbFjx5g3bx6TJ0/W3qrauXNnmWNntm/fTlFRkV63icqyevVqiouL6dOnDz/88AMxMTFcuHCBVatWaRMYOzs7pkyZwpw5czh8+DChoaFMmjQJX19f7cyqtm3b0qVLF+3D09MT0PRI3T2lPTg4mDZt2ugkPpJUE4rVgp/PXgfgk2d60N65SfUqvHEWhBqatAC7ljUQYfXIJEeSJKPq2rUrvXr1YseOHdpj33//Pbdu3eK7776jRYsW2scDDzygLdO4cWP2799Peno6vXv35rnnnmPkyJGsWrVKWyYjI4OLFy+WajMgIIDRo0eXGhQMmjVwFAoFR44cKTfmNm3aEBYWxpAhQ5g7dy5dunThkUce4eDBg6xdu1Zb7tNPP+Xxxx9nzJgxDBo0CBcXF3788UcD/4Vg69atTJ061eDrJKky4VfTSc8pxNbKjCEda+B2aFKY5qdrr+rXVQMUoiZH0dUzmZmZ2NnZkZGRga2trbHDkaQqy8vLIy4uDk9PzwoH8dZVu3fvZt68eURERJQ7jfpeOXz4MKNHjyY2NpamTasxjbaGlNy2u3Tpks74I0PV98+IVDtW/H6Rzw9d5vFuLfhifA0kJt9Phogf4OF3YdAb1a+vHPp+f8sxOZIkGZ2fnx8xMTEkJSXh7m7cKad79uzh7bffrhMJDsCNGzfYtGlTtRIcSSrPkYuaW8APdayhDTST/p7s0LJu9OTIJEeSpDph1qxZxg4BgOXLlxs7BB13LyYoSTXp5p08zidlADC4uiscA+SkQlq85rlr3RgkL8fkSJIkSdJ96NglzRYOXVva4dikGptxlrj+93icZm3Bum70hMokR5IkSZLuMylZ+XzzRxxAzQw4Bkg6o/lZR25VgbxdJUmSJEn3ldhbWUzccJKrqbnYWpkxxqfidaX0VjIep47MrALZkyNJkiRJ95W3fjzP1dRcPJrbsNN/AB7NS280azAh/rld1dI4e+aVRfbkSJIkSdJ9Iib5DifjUjE1UbBlaj9a2uu/BUuF0hMgKxlMzKFFt5qpswbInhxJkiRJuk9sOZkIwMNeTjWX4ABcPan52aI7mNdgvdUkkxxJkiRJug/kFRbzY1gSAOP7tqrZyq+e0Px071uz9VaTTHIkSTK6lJQUnJyciI+PN3Yodc5bb73Fq6++auwwpAZgz/kbZOQW0tLemkHta3hHe22S06dm660mmeRIkmR0ixcvZtSoUbRu3brUuZSUFNzc3FAoFKSnp+ucO3LkCL169cLS0pJ27doRGBhYaVvnzp1j4MCBWFlZ4e7uzrJly6oU8+XLl5k0aRJubm5YWlri6enJuHHjOH36tLZMamoqzz33HLa2ttjb2zNlyhSysrK050v2yfr346+//tKWeeONN9i4cSOxsbFVilOSAHILill1MAaAZx9wx9REUXOV59+B5EjNc9mTI0mS9I+cnBwCAgKYMmVKmeenTJlCt26lBzLGxcXh5+fHkCFDCA8PZ9asWbz00kvs27ev3LYyMzMZPnw4Hh4ehIaGsnz5ct577z2++uorg2I+ffo0Pj4+XLp0iS+//JKoqCjtjudz587VlnvuueeIjIxk//797Nq1i2PHjjFt2rRS9R04cIAbN25oHz4+/8xOcXBwQKlU6mz8KUmGWrYvmviUHFrYWTFxQOuarfzaac3O4/atwLZFzdZdXeI+lpGRIQCRkZFh7FAkqVpyc3NFVFSUyM3N1R5Tq9WiIK/IKA+1Wq137EFBQcLR0bHMc2vWrBGDBw8WBw8eFIBIS0vTnps/f77o3LmzTvmxY8cKpVJZbltr1qwRTZs2Ffn5+dpjb775pujYsaPe8arVatG5c2fh4+MjiouLS50viTEqKkoA4tSpU9pzv/32m1AoFCIpKUkIIURcXJwAxJkzZypsc+PGjcLNzU3vGMtS1mdEuj+ciE0RHm/uEh5v7hJHLt6s+QYOfyjEIlshvp9S83WXQ9/vbzmFXJIaqKICNV+9ftQobU9bORhzS1O9ygYHB+v0XJSIiori/fff58SJE2XeqgkJCSm1r5NSqaxwD6yQkBAGDRqEhYWFzjUfffQRaWlpem3KGR4eTmRkJFu2bClzx3R7e3ttW/b29vTu3Vt7btiwYZiYmHDixAn+85//aI8/8cQT5OXl0aFDB+bPn88TTzyhU2efPn24du0a8fHxZd7Sk6TyqNWCRb9obiWN7e1eM3tU/VsdHXQM8naVJElGlpCQgKurq86x/Px8xo0bx/Lly2nVquxZICqVCmdnZ51jzs7OZGZmkpuba9A1Jef0EROjGdfg5eVVYTmVSoWTk+7OzmZmZjRr1kzbVuPGjVmxYgVBQUHs3r2bBx98kCeffJJffvlF57qSf5+EhAS9YpSkEr+eu86FG5k0sTTjrREVf2arpLgIrp3SPK9jg45BLgYoSQ2WmYUJ01YONlrb+srNzcXKykrn2IIFC/D29ub555+v6dCqTQhRY3U5ODgwZ84c7esHHniA69evs3z5cp3eHGtrzbojOTk5Nda21PAVFqv5ZP8lAF4e3IamjSwquaIKVOcgPxMs7cC5S83XX02yJ0eSGiiFQoG5palRHgqF/jM3HBwcSEtL0zl26NAhgoKCMDMzw8zMjKFDh2rLLlq0CAAXFxeSk5N1rktOTsbW1labFPxbedeUnNNHhw4dAIiOjq6wnIuLCzdv3tQ5VlRURGpqaoVt9e3bl8uXL+scS01NBcDRsRZuNUgN1pYTiSSk5ODQ2IJJAzxrp5GEPzU/PXzBRL9b1PeSTHIkSTKqnj17EhUVpXPshx9+4OzZs4SHhxMeHs769esBzfgdf39/AHx9fTl48KDOdfv378fX17fctnx9fTl27BiFhYU613Ts2FGv8TgAPXr0oFOnTqxYsQK1Wl3qfMk0d19fX9LT0wkNDdWeO3ToEGq1mr59yx+7EB4eTosWujNUIiIiMDc3p3PnznrFKEkXbmSy9LcLALw2tD2NLGvpxk38H5qfrR+snfqrSSY5kiQZlVKpJDIyUqc3p23btnTp0kX78PTU/BXq7e2tHecyffp0YmNjmT9/PtHR0axZs4YdO3Ywe/ZsbT1ffPGFthcIYPz48VhYWDBlyhQiIyPZvn07K1eu1LllVBmFQsGGDRu4dOkSAwcOZM+ePcTGxnLu3Dntej8lsT766KNMnTqVkydP8ueffzJz5kyeffZZ7RibjRs3snXrVqKjo4mOjmbJkiV88803pRb/Cw4OZuDAgeX2UEnS3e7kFfLK5jDyCtUM6uDI8309aqchdTEkHNc8l0mOJElSaV27dqVXr17s2LHDoOs8PT3ZvXs3+/fvp3v37qxYsYL169ejVCq1ZW7fvs2VK1e0r+3s7Pj999+Ji4vDx8eHuXPnsnDhQp21a44cOYJCoahw9eU+ffpw+vRp2rVrx9SpU/H29uaJJ54gMjKSzz77TFtu8+bNeHl5MXToUB577DEefPDBUmvyfPDBB/j4+NC3b19+/vlntm/fzqRJk3TKbNu2jalTpxr07yPdv1b8fom429m42lnx2dgemNTkwn93047HsQWXurMp590UoiZH0dUzmZmZ2NnZkZGRga2trbHDkaQqy8vLIy4uDk9Pz1KDeOuD3bt3M2/ePCIiIsqcln0vbdiwgSVLlhAVFYW5ublRYwH47bffmDt3LufOncPMrOq3HOr7Z0TSz528QvotOUh2QTEbJ/epnSnjJY5/Dr+/Ax0ehfHba6+dMuj7/S1nV0mSZHR+fn7ExMSQlJSEu7u7UWPZs2cPS5YsqRMJDkB2djYbNmyoVoIj3T9+DEsiu6CYdk6NGdTeoXYbq+PjcUAmOZIk1REVLeJ3LwUFBRk7BB1PPfWUsUOQ6gkhBN/+pVlL6YV+HgbNcjRYcWGdH48DckyOJEmSJDUIIVdSuHwzi0YWpozu1bJ2G0v8SzMex8YBXLrXblvVIJMcSZIkSWoAtpxMBOA/vVrSxKqWb7fG/K752f4RMPI4uorU3cgkSZIkSdJLZl4hv0dpFrYc27vsrVBq1N1JTh0mkxxJkiRJqud+O3+DgiI17Zwa06VlLc8WTkuAW9GgMIW2D9duW9UkkxxJkiRJqud+CEsCYHSvlrU74Bjg8n7NT/e+YK3fSuHGIpMcSZIkSarHrqbmcDIuFYUCnuxRywOOAS7Vj1tVIJMcSZIkSarXfjqj6cXp59kcV/ta3voj6yZcOaR53uHR2m2rBsgkR5Iko0tJScHJyanCrRTuV3v37qVHjx5lbgYqScVqwbZTVwF4yset9hsM2wjqQnB7AJw71X571SSTHEmSjK5kY8vWrVvrHA8MDKRbt25YWVnh5OSk3YG8xLlz5xg4cCBWVla4u7uzbNmySttKTEzEz88PGxsbnJycmDdvHkVFRQbHrFKpePXVV2nTpg2Wlpa4u7szcuRInZ3R8/Ly8Pf3p3nz5jRu3JgxY8aQnJxcqq6K3uejjz6Kubk5mzdvNjhGqeE7HH2TpPRc7G3M8evWovILqqO4CE5v0Dx/4KXabauGyBWPJUkyqpycHAICAti3b5/O8U8++YQVK1awfPly+vbtS3Z2tk5PT2ZmJsOHD2fYsGGsW7eO8+fPM3nyZOzt7XU23LxbcXExfn5+uLi4cPz4cW7cuMGECRMwNzdnyZIlesccHx/PgAEDsLe3Z/ny5XTt2pXCwkL27duHv78/0dHRAMyePZvdu3cTFBSEnZ0dM2fOZPTo0fz55596v0+AF198kVWrVvHCCy/oHaN0fyhZ4fiZ3u5YmZvWbmOX9kJmEtg0h05P1m5bNUXcxzIyMgQgMjIyjB2KJFVLbm6uiIqKErm5udpjarVaFOTmGuWhVqv1jj0oKEg4OjrqHEtNTRXW1tbiwIED5V63Zs0a0bRpU5Gfn6899uabb4qOHTuWe82ePXuEiYmJUKlU2mNr164Vtra2OvVUZsSIEaJly5YiKyur1Lm0tDQhhBDp6enC3NxcBAUFac9duHBBACIkJETv9ymEEAkJCQIQly9f1jvGfyvrMyLVbwm3s0Xrt3YJjzd3ifjbpT+LNW7jKCEW2Qqxf1Htt1UJfb+/ZU+OJDVQRfn5rJponH2PXtv4PeZ67nQdHByMj4+PzrH9+/ejVqtJSkrC29ubO3fu0L9/f1asWKHdwDMkJIRBgwZhYWGhvU6pVPLRRx+RlpZG06alp7aGhITQtWtXnJ2dda6ZMWMGkZGR9OzZs9J4U1NT2bt3L4sXL6ZRo0alztvb2wMQGhpKYWEhw4YN057z8vKiVatWhISE0K9fP73eJ0CrVq1wdnYmODiYtm3bVhqjdH/YcfoqQsCgDo54NC/9WaxRd1QQe0TzvNdEvS7JKsiisUXj2otJD3JMjiRJRpWQkICrq6vOsdjYWNRqNUuWLOGzzz7j+++/JzU1lUceeYSCggJAMybm7mQF0L5WqVRltlWVa/7t8uXLCCHw8vKqsJxKpcLCwkKb9NzdXklb+rzPEq6uriQkJOgVo9TwCSHYc/4GAGNqe58qgKifAaEZcNzMs9LiQgjG7xnPmF/GEJMWU/vxlUP25EhSA2VmaclrG783Wtv6ys3NxepfvT5qtZrCwkJWrVrF8OHDAdi6dSsuLi4cPnwYpVJZo/EaQghRY3UZ8j6tra3Jycmpsbal+u3yzSxib2djYWrCw15Otd9gxA+an13G6FX8SvoV4jLiMDcxx6WRSy0GVjGZ5EhSA6VQKPS+ZWRMDg4OpKWl6Rxr0UIzS6RTp3+mqDo6OuLg4EBiomYTQhcXl1IzlUpeu7iU/UvVxcWFkydPGnTNv7Vv3x6FQqEdXFweFxcXCgoKSE9P1+nNSU5O1ralz/sskZqaiqOjo14xSg3f3ghNb+CD7R1qfzPO9ES4egJQ6D3g+PcEzYKBA1wH0MSiSe3FVgl5u0qSJKPq2bMnUVFROscGDBgAwMWLF7XHUlNTuX37Nh4eHgD4+vpy7NgxCgsLtWX2799Px44dyxyPU3LN+fPnuXnzps41tra2OolGRZo1a4ZSqWT16tVkZ2eXOp+eng6Aj48P5ubmOlPKL168SGJiIr6+vnq/T9BMRb9y5YpeY4ak+8PeSE2S82jne9BLErlT87P1g2Cr3zT13+M1Sc4jrY27KrJMciRJMiqlUklkZKROb06HDh0YNWoUr7/+OsePHyciIoKJEyfi5eXFkCFDABg/fjwWFhZMmTKFyMhItm/fzsqVK5kzZ462np07d+qMnRk+fDidOnXihRde4OzZs+zbt4933nkHf39/LA24xbZ69WqKi4vp06cPP/zwAzExMVy4cIFVq1ZpExg7OzumTJnCnDlzOHz4MKGhoUyaNAlfX1/69eun9/sE+Ouvv7C0tNTWLd3frqbmEHk9ExMFDOvkXPkF1aEuhjN/r9FkwK2qKxlXMDMx4yH3h2ovNj0YlOSsXbuWbt26YWtri62tLb6+vvz222/a8/osfKXPQlxHjhyhV69eWFpa0q5dOwIDA0vFsnr1alq3bo2VlRV9+/Yt1QUtSVL90LVrV3r16sWOHTt0jm/atIm+ffvi5+fH4MGDMTc3Z+/evZiba7rm7ezs+P3334mLi8PHx4e5c+eycOFCnTVyMjIydHpJTE1N2bVrF6ampvj6+vL8888zYcIE3n//fW2Z+Ph4FAoFR44cKTfmNm3aEBYWxpAhQ5g7dy5dunThkUce4eDBg6xdu1Zb7tNPP+Xxxx9nzJgxDBo0CBcXF3788UeD3idoxuk899xz2NjYGPaPKzVI+/7uxenr2ZxmjSwqKV1NZ76F2xfByh46/0evS0p6cfq79sfWopZ3RK+MIfPSf/nlF7F7925x6dIlcfHiRfH2228Lc3NzERERIYQQYvr06cLd3V0cPHhQnD59WvTr10/0799fe31RUZHo0qWLGDZsmDhz5ozYs2ePcHBwEAsWLNCWiY2NFTY2NmLOnDkiKipKfP7558LU1FTs3btXW2bbtm3CwsJCfPPNNyIyMlJMnTpV2Nvbi+TkZEPejlwnR2ow6vsaKLt27RLe3t6iuLjY2KGIQ4cOCXt7e5GammrsUIQQQty6dUs0a9ZMxMbGVque+v4Zkf7x9LrjwuPNXeKbP6r3mahUXqYQy9pq1sYJWaP3ZU/+9KToEthF/BTzU62Fpu/3d7UXA2zatKlYv369Xgtf6bMQ1/z580Xnzp112hg7dqxQKpXa13369BH+/v7a18XFxcLV1VUsXbrUoNhlkiM1FA3hC+zTTz8ViYmJxg5DvPHGG2LZsmXGDkPr1KlTYtu2bdWupyF8RiQhUrLyheffCwBeTc2u3cYOvK9JcFb2FKJQv8Uyb2bfFF0Cu4iugV1Fel56rYWm7/d3lcfkFBcXs23bNrKzs/H19a104SsofyGuzMxMIiMjtWXurqOkTEkdBQUFhIaG6pQxMTFh2LBh2jLlyc/PJzMzU+chSVLdMGvWLJ0F8Ixl+fLlzJs3z9hhaPXu3ZuxY8caOwypjjgUfRO1AO8Wtrg1rcXbl2o1hG3SPB+2CMz0uy0WejMUgI7NOmJnaVdb0enN4CTn/PnzNG7cGEtLS6ZPn87OnTvp1KmTXgtf6bMQV3llMjMzyc3N5fbt2xQXF5dZprLFvJYuXYqdnZ32URd+oUqSJEmSvg5Eaca5PlLbA46Tz0P2TTBvBB1G6H1ZqEqT5Pg4+1RS8t4wOMnp2LEj4eHhnDhxghkzZjBx4sRS0z/rqgULFpCRkaF9XL161dghSZIkSZJe8gqLORZzC4BHvGs5ybl8QPOzzWC9e3Hgn56cXk69aiMqgxm8GKCFhQXt2rUDNOtAnDp1ipUrVzJ27NhKF77SZyGu8hb4srW1xdraGlNTU0xNTcssU9liXpaWlgZNE5UkSZKkuiLkSgo5BcW0sLOiS8tanrV0+e/1ndoN1fuSjPwMLqddBqCXc91Icqq9To5arSY/P1+vha/0WYjL19dXp46SMiV1WFhY4OPjo1NGrVZz8OBBuYaEJEmS1GD9/vetqmHezigUitprKC/j7xWOgbb6Jzlnbp5BIGht2xoHa4daCs4wBvXkLFiwgBEjRtCqVSvu3LnDli1bOHLkCPv27dNZ+KpZs2bY2try6quv6ix8dfdCXMuWLUOlUpVaiGv69Ol88cUXzJ8/n8mTJ3Po0CF27NjB7t27tXHMmTOHiRMn0rt3b/r06cNnn31GdnY2kyZNqsF/GkmSJEmqG9RqwYELfyc5tT0eJ+4YqIugeTu9NuMsEZpct8bjgIFJzs2bN5kwYQI3btzAzs6Obt26sW/fPh55RLNs86effoqJiQljxowhPz8fpVLJmjVrtNeXLMQ1Y8YMfH19adSoERMnTtRZiMvT05Pdu3cze/ZsVq5ciZubG+vXr9fZqG7s2LHcunWLhQsXolKp6NGjB3v37i01GFmSJEmSGoJzSRncupNPY0sz+rVpVruNldyqMqAXByAsOQyoW0mOQoga3FK3nsnMzMTOzo6MjAxsbY28KqMkVUNeXh5xcXF4enqW2tFbkkB+Ruq75fuiWX34Cn7dWrB6fC2Od8m6Bat6QsEdeO4HaD+s8muAnMIcBmwdQJEoYt+Yfbg2dq29GNH/+1vuXSVJktGlpKTg5OREfHy8sUOpc9atW8fIkSONHYZkZAeiNGNZa31W1dGPNAlOi+7Q9mG9Lzt76yxFogiXRi61nuAYQiY5kiQZ3eLFixk1ahStW7fWHjt16hRDhw7F3t6epk2bolQqOXv2rPb8e++9h0KhKPVo1KhRhW3ps3+ePlQqFa+++ipt2rTB0tISd3d3Ro4cqTMporL9/AIDA8t8DwqFQjtBY/LkyYSFhREcHGxwjFLDkJiSw8XkO5iaKBjS0an2Grp9GUI3aJ4/8gGY6J8i1MXxOCCTHEmSjCwnJ4eAgACmTJmiPZaVlcWjjz5Kq1atOHHiBH/88QdNmjRBqVRSWFgIwBtvvMGNGzd0Hp06deLpp58ut63i4mL8/PwoKCjg+PHjbNy4kcDAQBYuXGhQzPHx8fj4+HDo0CGWL1/O+fPn2bt3L0OGDMHf319bbvbs2fz6668EBQVx9OhRrl+/zujRo7Xnx44dW+o9KJVKBg8ejJOT5svMwsKC8ePHs2rVKoNilBqOvZE3AOjr2Qw7G/NKSlfDgUWaAcftlZr1cQwQdrPujccBDNugs6GRe1dJDUVZ+xKp1WpRnF9klIdardY79qCgIOHo6Khz7NSpUwLQ2cvq3LlzAhAxMTFl1hMeHi4AcezYsXLb0mf/PH2MGDFCtGzZUmRlZZU6l5aWJoQQeu3n9283b94U5ubmYtOmTTrHjx49KiwsLEROTo7eMf6b3LuqflKr1WLIx4eFx5u7xOa/Emqvofjjmn2q3rMXIvmCQZfmF+ULn299RJfALuJK+pVaClCXvt/fBi8GKElS/SAK1VxfeNwobbu+3x+FhaleZYODg/Hx0f3rr2PHjjRv3pyAgADefvttiouLCQgIwNvbW+eW1t3Wr19Phw4dGDhwYLltlbd/3owZM4iMjKRnz56VxpuamsrevXtZvHhxmbfGShZDrWw/v5KlNe62adMmbGxseOqpp3SO9+7dm6KiIk6cOMFDDz1UaYxSw3EyLpXYW9nYWJjyRI9aGusiBOx/V/O85wvg5GXQ5ZEpkeQX59PMqhmetvpPOb8X5O0qSZKMKiEhAVdX3V/eTZo04ciRI3z33XdYW1vTuHFj9u7dy2+//YaZWem/zfLy8ti8ebPOLa+y6LN/XmUuX76MEAIvr4q/CPTZz+/fAgICGD9+PNbW1jrHbWxssLOzIyEhQa8YpYZj68lEAEb1cKWxZS31S0T9BNdOafapGvK2wZeXjMfp5dSrdhcprALZkyNJDZTC3ATX9/sbrW195ebmlprSnJuby5QpUxgwYABbt26luLiYjz/+GD8/P06dOlUqCdi5cyd37txh4sSJNRJ/RUQtrboREhLChQsX+Pbbb8s8b21tTU5OTq20LdVNadkF7InQJMTj+3jUTiO56bD378Sm/6vQpOLtkcpSVwcdg0xyJKnBUigUet8yMiYHBwfS0tJ0jm3ZsoX4+HhCQkIw+XuGx5YtW2jatCk///wzzz77rE759evX8/jjj1e6IKg+++dVpn379igUCqKjoyttq7L9/P79Hnr06FHq1l2J1NRUHB0d9YpRahh2nbtOQZGaLi1t6epmVzuN7F0Ad65DszYw4DWDL88pzKnTSY68XSVJklH17NmTqKgonWM5OTmYmJjodH2XvFar1Tpl4+LiOHz4cKW3qkC//fMq06xZM5RKJatXryY7O7vU+fT0dAC99vMrkZWVxY4dO8p9D1euXCEvL0+vMUNSw3EyXpP8KzsZ3ruil+jdcHYLoIAn14JFxcsvlOX3hN/JLcqlVZNWeDUzbCzPvSCTHEmSjEqpVBIZGanTm/PII4+QlpaGv78/Fy5cIDIykkmTJmFmZsaQIUN0rv/mm29o0aIFI0aMKFX3zp07dcbO3L1/3tmzZ9m3b1+p/fP0sXr1aoqLi+nTpw8//PADMTExXLhwgVWrVmkTmLv38zt8+DChoaFMmjRJZz+/Etu3b6eoqIjnn3++zPaCg4Np06YNbdu21TtGqf4LS9D8n+jl0bTmK48Lhh9e0jzvPxNalR4Ir4+fLv8EwJPtnqxz43FAJjmSJBlZ165d6dWrFzt27NAe8/Ly4tdff+XcuXP4+voycOBArl+/zt69e2nRooW2nFqtJjAwkBdffBFT09K35jIyMrh48aL2dcn+eaampvj6+vL8888zYcIEnf3z4uPjUSgUHDlypNyY27RpQ1hYGEOGDGHu3Ll06dKFRx55hIMHD7J27VptuU8//ZTHH3+cMWPGMGjQIFxcXPjxxx9L1RcQEMDo0aNLDVIusXXrVqZOnVpuPFLDczMzj6T0XEwU0N3dvmYrTwiBLc9AYQ60GwYPv1u1ajITCE0OxURhwsi2dXNVbrl3ldy7SmoA6vu+RLt372bevHlERERox+AYy+HDhxk9ejSxsbE0bVoLf0EbKDIykocffphLly5hZ1f1cRn1/TNyv9kbcYPp34Xh5dKEvbMG1VzFBTmwug9kXNUkOGM3g3nVPg+rwlbx9fmvGdByAOuGrau5GPWg7/e3HHgsSZLR+fn5ERMTQ1JSEu7u7kaNZc+ePbz99tt1IsEBuHHjBps2bapWgiPVP2GJ6UAt3KoKXqFJcOzc4ZlNVU5w1ELNr7G/AppbVXWVTHIkSaoTZs2aZewQAFi+fLmxQ9Bx92KC0v1DOx6nVQ0mOSlX4Pjf24M8urRKA41LRN6ORJWtwtrMmofcHqqZ+GqBHJMjSZIkSXVIQZGac0kZAPRqZV8zlRblw87pUFyguU3l9Xi1qjuQeACAQW6DsDKru7c/ZZIjSZIkSXVI1I1MCorUNLUxx9Oh6r0tWkLA7jlw7SRY2sFjy6EaM6GEEBxM1CyNMKxV3e5plEmOJEmSJNUhJ2JTAOjZqmn1p2ULAcEfw5nvQGECT3+jWfivGq6kXyEhMwFzE3MGupW/V1xdIMfkSJIkSVIdUrKVw5CO1VzhWq2G3/8Lf63RvB7+f5pbVdVUcquqv2t/GpnXQE9TLZJJjiRJkiTVEVdTczh7NR0TBSi7VHOl431vw4m/120avhh8/asdnxCC3xN+B2Boq6HVrq+2ySRHkiRJkuqIPedvANDXszlOTaoxoDd69z8Jzn++gu5jayA6OHPzDDFpMViZWvFwq4drpM7aJMfkSJIkSVIdsfvvJMevW4tKSlYg4xr89Irmef9XayzBAdh8YTMAfm38sLOs+2s3ySRHkiSjS0lJwcnJifj4eGOHUi+99dZbvPrqq8YOQ6qmxJQczl3LwEQBj1bnVtWe+ZCXDi194OGFNRafKlulnVU1zmtcjdVbm2SSI0mS0S1evJhRo0bRunVr7bHXXnsNHx8fLC0t6dGjR6lrjhw5wqhRo2jRogWNGjWiR48ebN68uVS5oKAgvLy8sLKyomvXruzZs6fSeI4cOUKvXr2wtLSkXbt2BAYGVul9nTlzhqeffhpnZ2esrKxo3749U6dO5dKlS9oyiYmJ+Pn5YWNjg5OTE/PmzaOoqEinns2bN9O9e3dsbGxo0aIFkydPJiUlRXv+jTfeYOPGjcTGxlYpTqluOHAhGYB+bZrj0Fj/DWN1XDsNF3drZlI9uRbMLGosvh0Xd1AsivFx9qFjs441Vm9tkkmOJElGlZOTQ0BAAFOmTCl1bvLkyYwdW3ZX+/Hjx+nWrRs//PAD586dY9KkSUyYMIFdu3bplBk3bhxTpkzhzJkzPPnkkzz55JNERESUG09cXBx+fn4MGTKE8PBwZs2axUsvvcS+ffsMel+7du2iX79+5Ofns3nzZi5cuMB3332HnZ0d776r2RCxuLgYPz8/CgoKOH78OBs3biQwMJCFC//56/vPP/9kwoQJTJkyhcjISIKCgjh58qTOhp0ODg4olUqdzUGl+ud0QioAA9o5VL2Sg//T/Ow+HhxrLhHJLsxmxyXNJrrjvcbXWL21TtzHMjIyBCAyMjKMHYokVUtubq6IiooSubm52mNqtVrk5+cb5aFWq/WOPSgoSDg6OpZ7ftGiRaJ79+561fXYY4+JSZMmaV8/88wzws/PT6dM3759xcsvv1xuHfPnzxedO3fWOTZ27FihVCr1ikEIIbKzs4WDg4N48sknyzyflpYmhBBiz549wsTERKhUKu25tWvXCltbW5Gfny+EEGL58uWiTZs2OtevWrVKtGzZUufYxo0bhZubW7kxlfUZkeoOtVot+izeLzze3CVCrtyuWiWXDwmxyFaI9x2ESEuo0fi+Pve16BLYRTz+4+OisLiwRuuuCn2/v+XsKklqoAoLC1myZIlR2n777bexsNCvmzw4OBgfH58aaTcjIwNvb2/t65CQEObMmaNTRqlU8tNPP5VbR0hISKn9opRKpUF7a+3bt4/bt28zf/78Ms/b29tr2+ratSvOzs46bc2YMYPIyEh69uyJr68vb7/9Nnv27GHEiBHcvHmT77//nscee0ynzj59+nDt2jXi4+N1bvtJ9cO1tFySM/MxM1HQ3c3e8Arys2DXbM3z3pPBvlWNxZZdmM3GyI0ATOs2DTOT+pM6yNtVkiQZVUJCAq6urtWuZ8eOHZw6dYpJkyZpj6lUKp0EAsDZ2RmVSlVuPeVdk5mZSW5url6xxMTEAODl5VVhufLaKjkHMGDAADZv3szYsWOxsLDAxcUFOzs7Vq9erXNdyb9hQkKCXjFKdUvo3xtydm5ph7WFqeEV7FsAaXFg6wYPLajR2LZGbyU9Px0PWw9GeI6o0bprW/1JxyRJMoi5uTlvv/220drWV25uLlZW1dvg7/Dhw0yaNImvv/6azp07V6uumiCEqLG6oqKieP3111m4cCFKpZIbN24wb948pk+fTkBAgLactbU1oBnjJNU/JeNxfKqy6/ilfRC2CVDAf9aBtX2NxZVfnM+3Ud8C9a8XB2SSI0kNlkKh0PuWkTE5ODiQlpZW5euPHj3KyJEj+fTTT5kwYYLOORcXF5KTk3WOJScn4+JS/vTc8q6xtbXVJhKV6dChAwDR0dH4+vpW2NbJkydLtVVyDmDp0qUMGDCAefPmAdCtWzcaNWrEwIED+b//+z9atNCsp5KaqvmSdHSs5lYAklGEJqQD0Lu1gUmOEHDo/zTPff3Bs2b3ktoTu4fUvFRcGrnUu14ckLerJEkysp49exIVFVWla48cOYKfnx8fffQR06ZNK3Xe19eXgwcP6hzbv39/hYlHVa75t+HDh+Pg4MCyZcvKPJ+enq5t6/z589y8eVOnLVtbWzp16gRoemZMTHR/VZuaam5n3N1jFBERgbm5eZ3oyZIMcyevkIuqTAB6exiY5MQdA9U5MLOGgXNrNC4hBJuiNgHwnNdzmJvo30NbV8gkR5Iko1IqlURGRpbqzbl8+TLh4eGoVCpyc3MJDw8nPDycgoICQHOLys/Pj9dee40xY8agUqlQqVTaHg2A119/nb1797JixQqio6N57733OH36NDNnztSWWbBggU4P0PTp04mNjWX+/PlER0ezZs0aduzYwezZs/V+T40aNWL9+vXs3r2bJ554ggMHDhAfH8/p06eZP38+06dPBzTJUKdOnXjhhRc4e/Ys+/bt45133sHf3x9LS806KSNHjuTHH39k7dq1xMbG8ueff/Laa6/Rp08fnbFMwcHBDBw4UO/eJqnuOJOYjlqAezNrnGwNvHV7fJXmZ8/nwaZZjcYVcj2Ey+mXsTGzYXSH0TVa9z1zL6Z61VVyCrnUUNT36cF9+vQR69at0zk2ePBgAZR6xMXFCSGEmDhxYpnnBw8erFPPjh07RIcOHYSFhYXo3Lmz2L17t875iRMnlrrm8OHDokePHsLCwkK0adNGbNiwQef8hg0bhD6/Pk+dOiVGjx4tHB0dhaWlpWjXrp2YNm2aiImJ0ZaJj48XI0aMENbW1sLBwUHMnTtXFBbqTtFdtWqV6NSpk7C2thYtWrQQzz33nLh27ZpOmY4dO4qtW7eWG0t9/4w0ZEv2RAmPN3eJ2dvOGHahKlIzZfw9eyFSrtR4XC/te0l0CewiPjzxYY3XXV36fn8rhKjBEXL1TGZmJnZ2dmRkZGBra2vscCSpyvLy8oiLi8PT07Pag3iNYffu3cybN4+IiIhSt2bqokWLFnH06FGOHDli7FAA+O2335g7dy7nzp3DzKzsoZb1/TPSkD362TGiVXdY+WwPRvVoqf+FP/vDme/A+wkY+22NxnRKdYrJ+yZjpjDj1//8ilsTtxqtv7r0/f6WA48lSTI6Pz8/YmJiSEpKwt3d3djhVOq3337jiy++MHYYWtnZ2WzYsKHcBEequ1QZeUSr7qBQwMD2Bgwaz0mF899rnvv612hMQghWhq0EYEyHMXUuwTGE/B8hSVKdYMhie8b27xlRxvbUU08ZOwSpio5dugVANzd7mjUyYDZk2CYoygOXruDet0ZjOnrtKGdvncXK1IqXu71co3Xfa3W/X1iSJEmSGqijfyc5gzsY0IujLoZTf6+R1OdlUChqLJ4idZG2F2e893gcber3kgQyyZEkSZIkIygqVhMco0lyHupoQDJxaR9kJIJ1U+has714P8b8yOX0y9hZ2jG5y+QardsYZJIjSZIkSUYQfjWdzLwi7G3MDduv6uSXmp89XwDzmlsy4E7BHb44oxlr9kr3V7CztKuxuo1FJjmSJEmSZAQlt6oGtnfE1ETPW063LkLsEUABD7xUo/F8fuZz0vLT8LTz5OmOT9do3cYikxxJkiRJMoIjF6swHufk15qfHUdAU48ai2XLhS1sjd4KwPwH5tfL1Y3LIpMcSZIkSbrHbmflcz4pA4BBHRz0uygvE85qEhH6lN7GpKoOJhzkw5MfAjCzx0webPlgjdVtbDLJkSRJkqR7rGTAcWdXW5ya6Lk447ntUJAFDh2gzUM1Esedgju8/9f7CATPdHiGad1qLnmqC2SSI0mS0aWkpODk5ER8fLyxQ6mX3nrrLV599VVjhyEZoEq3qs5u0/z0mVRj08a/Pvc1qXmpeNp58lbft1DU4HT0ukAmOZIkGd3ixYsZNWoUrVu3BuDs2bOMGzcOd3d3rK2t8fb2ZuXKlaWuy8/P57///S8eHh5YWlrSunVrvvnmG+35hx56CIVCUerh5+dXYTxHjhyhV69eWFpa0q5dOwIDA6v0vs6cOcPTTz+Ns7MzVlZWtG/fnqlTp3Lp0iVtmcTERPz8/LCxscHJyYl58+ZRVFSkU8/q1avx9vbG2tqajh07smnTJp3zb7zxBhs3biQ2NrZKcUr3VrFaaBcB1DvJSY2FpNOgMIEuY2okjquZV/nuwncAvNH7jQYzDuducsVjSZKMKicnh4CAAPbt26c9FhoaipOTE9999x3u7u4cP36cadOmYWpqqrOD+DPPPENycjIBAQG0a9eOGzduoFarted//PFH7a7loOkx6t69O08/Xf7Mkbi4OPz8/Jg+fTqbN2/m4MGDvPTSS7Ro0QKlUqn3+9q1axdjxoxBqVSyefNm2rZty82bNwkKCuLdd99l+/btFBcX4+fnh4uLC8ePH+fGjRtMmDABc3NzlixZAsDatWtZsGABX3/9NQ888AAnT55k6tSpNG3alJEjRwLg4OCAUqlk7dq1LF++XO8YJeOISMogLaeQJpZm9PJoqt9FJVs4eA6GJs7VjuF27m3mH5tPoboQ3xa+DGw5sNp11kn3YrfQukruQi41FGXtMK1Wq0VRUbZRHmq1Wu/Yg4KChKOjY6XlXnnlFTFkyBDt699++03Y2dmJlJQUvdv69NNPRZMmTURWVla5ZebPny86d+6sc2zs2LFCqVTq3U52drZwcHAQTz75ZJnn09LShBBC7NmzR5iYmAiVSqU9t3btWmFrayvy8/OFEEL4+vqKN954Q+f6OXPmiAEDBugc27hxo3Bzcys3JrkLed3x2f5LwuPNXeLlTaf1u0CtFmKVj2bH8TObq91+TGqMeCToEdElsIvw3eIrrqTV/A7mtU3f72/ZkyNJDZRancuRo12N0vZDg89jamqjV9ng4GB8fHwqLZeRkUGzZs20r3/55Rd69+7NsmXL+Pbbb2nUqBFPPPEEH3zwAdbWZS+QFhAQwLPPPkujRo3KbSckJIRhw4bpHFMqlQbtrbVv3z5u377N/Pnzyzxvb2+vbatr1644O//zl7lSqWTGjBlERkbSs2dP8vPzS+0abm1tzcmTJyksLMTcXHOLoU+fPly7do34+HjtbT+pbjp66SZgwCrHN85CSgyYWYHX49VqO7col9cPv86N7Bt42HrwxcNf0NqudbXqrMvkmBxJkowqISEBV1fXCsscP36c7du3M23aPzM/YmNj+eOPP4iIiGDnzp189tlnfP/997zyyitl1nHy5EkiIiJ46aWKF1BTqVQ6SQeAs7MzmZmZ5Obm6vWeYmJiAPDy8qpSWyXnQJP0rF+/ntDQUIQQnD59mvXr11NYWMjt27e115X8GyYkJOgVo2Qc6TkFhF9NB2CQvuNxzgdpfnZ4FKxsq9X+52c+J/FOIk42Tnw74tsGneCAHJMjSQ2WiYk1Dw0+b7S29ZWbm1uqp+JuERERjBo1ikWLFjF8+HDtcbVajUKhYPPmzdjZaZaf/+STT3jqqadYs2ZNqd6cgIAAunbtSp8+fQx8N4YTQtRYXe+++y4qlYp+/fohhMDZ2ZmJEyeybNkyTEz++Tu15P3m5OTUWNtSzQuOuY1aQAfnxrja6/H/RF38z3icbs9Uq+1TqlN8F6UZaLzIdxFNrfQcD1SPyZ4cSWqgFAoFpqY2RnkYMg3VwcGBtLS0Ms9FRUUxdOhQpk2bxjvvvKNzrkWLFrRs2VKb4AB4e3sjhODatWs6ZbOzs9m2bRtTpkypNB4XFxeSk5N1jiUnJ2Nra1vubbB/69ChAwDR0dFVaqvkHGiSl2+++YacnBzi4+NJTEykdevWNGnSBEfHf3oCUlNTAXSOSXVPyVYOD3V00u+C+D8gSwVW9tDukSq1WaguZN3ZdUz7fRoCwai2oxjkNqhKdRkiKziYgn/9X7zXZJIjSZJR9ezZk6ioqFLHIyMjGTJkCBMnTmTx4sWlzg8YMIDr16+TlZWlPXbp0iVMTExwc3PTKRsUFER+fj7PP/98pfH4+vpy8OBBnWP79+/H19dX37fE8OHDcXBwYNmyZWWeT09P17Z1/vx5bt68qdOWra0tnTp10rnG3NwcNzc3TE1N2bZtG48//rhOT05ERATm5uZ07txZ7zile0utFtokR++p4+d3aH52GgVmFga3eTntMs/veZ7V4aspEkUMazWMBX0XGFyPodT5+Vyf/yZXhivJCQur9fbKI5McSZKMSqlUEhkZqdObExERwZAhQxg+fDhz5sxBpVKhUqm4deuWtsz48eNp3rw5kyZNIioqimPHjjFv3jwmT55c5q2qJ598kubNm5dqf8GCBUyYMEH7evr06cTGxjJ//nyio6NZs2YNO3bsYPbs2Xq/p0aNGrF+/Xp2797NE088wYEDB4iPj+f06dPMnz+f6dOnA5pkqFOnTrzwwgucPXuWffv28c477+Dv74+lpSWgSdy+++47YmJiOHnyJM8++ywRERHaKeYlgoODGThwoN69TdK9d0GVya07+dhYmNK7tR63igrzIOpXzfMq3Kr6Le43ntn1DFEpUdha2PLRwI/45KFPaGRe/sD7mpK5axfFaWmYuThj3a1brbdXrnsw06vOklPIpYaivk8P7tOnj1i3bp329aJFiwRQ6uHh4aFz3YULF8SwYcOEtbW1cHNzE3PmzBE5OTk6ZaKjowUgfv/99zLbnjhxohg8eLDOscOHD4sePXoICwsL0aZNG7Fhwwad8xs2bBD6/Po8deqUGD16tHB0dBSWlpaiXbt2Ytq0aSImJkZbJj4+XowYMUJYW1sLBwcHMXfuXFFYWKg9HxUVJXr06CGsra2Fra2tGDVqlIiOji7VVseOHcXWrVvLjaW+f0YagtWHY4THm7vElMCT+l0Q+bNm2viKTkIUFxvUVlx6nHjguwdEl8Auwv+Av7iZfbMKEVeNWq0WV54YJaI6eonb69fXShv6fn8rhKjBEXL1TGZmJnZ2dmRkZGBrW70R65JkTHl5ecTFxeHp6VnhIN66avfu3cybN4+IiAidWzB11aJFizh69ChHjhwxdigA/Pbbb8ydO5dz585hZlb2fJL6/hlpCJ75MoSTcal8MKozL/i2rvyC756Cy/thwCx45H96t1OoLmTCnglEpETQ16UvXw3/ChPFvft/lf3XCRJffBGFtTXtjxzG9K5xczVF3+9vObtKkiSj8/PzIyYmhqSkJNzd3Y0dTqV+++03vvjiC2OHoZWdnc2GDRvKTXAk48vMKyQsQXNLdnAHPQYdpyXA5QOa570mVFz2LmqhZsmJJUSkRGBrYcv/Pfh/9zTBAUj99lsA7EY9USsJjiHk/whJkuoEQxbbM7aTJ08aOwQdTz31lLFDkCpx/HIKRWpBG4dGtGqux0KZZ74FhGa38eZt9WqjWF3MouOL+PnKzyhQ8H7/93Fp5FKtuA1VmHyTrMOHAWj2wgv3tO2y1P1+YUmSJEmq50pWOdZrAcDiQgjT9Ibg86LebXwW9hk/X/kZU4UpSwcuZajH0CpEWj2Zu3aBWo11z55YttUvOatNBiU5S5cu5YEHHqBJkyY4OTnx5JNPcvHiRZ0yeXl5+Pv707x5cxo3bsyYMWNKrQOhz667+uwCvHr1alq3bo2VlRV9+/atc39dSZIkSZIQgqMXS9bH0SPJufibZm2cRo7Q0U+vNiJuR7ApSrM7/dKBS/Fro991NS3j558BsBs1yijt/5tBSc7Ro0fx9/fnr7/+Yv/+/RQWFjJ8+HCys7O1ZWbPns2vv/5KUFAQR48e5fr164wePVp7vmTX3YKCAo4fP87GjRsJDAxk4cKF2jIluwAPGTKE8PBwZs2axUsvvaSzS/H27duZM2cOixYtIiwsjO7du6NUKnXWm5AkSZIkY4u5mcX1jDwszUzo16b0MgalhPw93qvXBL3WxilUF7Lo+CLUQo1fGz9GeI6oZsRVkxcdTf6lSyjMzbEd8ahRYiilOlO4bt68KQBx9OhRIYQQ6enpwtzcXAQFBWnLXLhwQQAiJCRECKHfrrv67ALcp08f4e/vr31dXFwsXF1dxdKlS/WOX04hlxoKOT1Yqoz8jBjPkj1RwuPNXWLSBj2mjif8pZk2/r6DEJk39Ko/MCJQdAnsIh7c+qBIyU2pZrRVp1r6oYjq6CWuvvZ6rbel7/d3tcbkZGRkAGh3Bg4NDaWwsFBnB18vLy9atWpFSEgIUP6uu5mZmURGRmrLlLULcEkdBQUFhIaG6pQxMTFh2LBh2jJlyc/PJzMzU+chSZIkSbWloEjN96c1WxuMfUCPmYPHV2l+dhsLTSofNFykLuK7C5r9qF7v9TrNrJpVOdbqUBcUkPGrZuFCu1FPGCWGslQ5yVGr1cyaNYsBAwbQpUsXQLNrroWFBfb29jplnZ2dtTvq6rPrbmW7AN++fZvi4uIyy5TUUZalS5diZ2enfdSHqaqSJElS/bUvUkVKdgHOtpYM9apk6vjtGIjerXne/1W96j9y9QiqbBVNLZsysu3I6gVbDZm7dlOckoKZszONBw40Whz/VuUkx9/fn4iICLZt21aT8dSqBQsWkJGRoX1cvXrV2CFJkiRJDdiWE4kAjH2gFWamlXzlnv8eENBeCY4d9as/egsAYzqMwdLUsjqhVpkQgtS/Jwc1e+F5FObmRomjLFVKcmbOnMmuXbs4fPiwzkZ4Li4uFBQUaDefK5GcnKzdUVefXXcr2wXYwcEBU1PTMsuU1FEWS0tLbG1tdR6SJBlfSkoKTk5OxMfHGzuUeunZZ59lxYoVxg5D+pe429mExKZgooBn9blVdeWQ5qf343rVfyntEqdUpzBVmDK249hqRFo92cePawYc29hg//TTRoujLAYlOUIIZs6cyc6dOzl06BCenp465318fDA3N9fZwffixYskJiZqd/DVZ9fdynYBtrCwwMfHR6eMWq3m4MGDBu0ULElS3bB48WJGjRpF69atS51LSUnBzc0NhUJR6g+o2lpqIigoCC8vL6ysrOjatSt79uyp0vs6fPgwjz32GM2bN8fGxoZOnToxd+5ckpKSAM2SGy+++CJdu3bFzMyMJ598ssx6Knuf77zzDosXL9aOk5TqhsPRmu+5/m0dcLWvZOPU3DRIOq153vZhvepfE74GgIdbPXzPF/27W2rgRgDsR482+grHpRgymnnGjBnCzs5OHDlyRNy4cUP7uHtDvOnTp4tWrVqJQ4cOidOnTwtfX1/h6+urPV9UVCS6dOkihg8fLsLDw8XevXuFo6OjWLBggbZMbGyssLGxEfPmzRMXLlwQq1evFqampmLv3r3aMtu2bROWlpYiMDBQREVFiWnTpgl7e3udWVuVkbOrpIaiPs+cyc7OFra2ttoZmP82atQoMWLECAGItLQ07fGS3xNz5swRUVFR4vPPPy/z94SFhYX45ptvRGRkpJg6daqwt7cXycnJ5cbz559/ClNTU7Fs2TIRFRUl3nnnHWFubi7Onz9v0Ptat26dMDExEZMmTRKHDx8WcXFx4ujRo2LKlCli9uzZQgghsrKyxPTp08VXX30llEqlGDVqVKl69HmfQgjRu3dv8cUXX5QbT33+jNRXUwJPCo83d4m1Ry5XXjjyJ82sqs8f0Kvu3+N/F10Cu4geG3uI6JTSG7beK3mXLomojl4iystb5Ccm3rN29f3+NijJoYxdgQGdHXpzc3PFK6+8Ipo2bSpsbGzEf/7zH3Hjhu40uMp23RWi8l2AhRDi888/F61atRIWFhaiT58+4q+//jLk7cgkR2owyvoCU6vVIquoyCgPtVqtd+xBQUHC0dGxzHNr1qwRgwcPFgcPHiyV5NTWUhPPPPOM8PPz0znWt29f8fLLL+v9nq5evSosLCzErFmzyjx/9/soMXHixDKTHH3epxBC/O9//xMPPvhguTHJJOfeKiwqFl0W7hUeb+4S566mV37Bz69qkpw9b1ZaND0vXQzeNlh0CewiVoWtqoFoqy7pv//VTBuf+eo9bVff72+D9q4SemxYbmVlxerVq1m9enW5ZTw8PCrt/n3ooYc4c+ZMhWVmzpzJzJkzK41Jku5HOWo1bY+dN0rbVwZ1pZGpqV5lg4OD8fHxKXU8KiqK999/nxMnThAbG1vqfHlLTZTsgVWy1MSCBQu05/VZaiIkJIQ5c+aUqvenn37S6/2A5nZXQUEB8+fPL/P8v2egVqSy91miT58+LF68mPz8fCwtjTMAVfrH+aQM7uQXYWtlRifXSsZ/CgFXNPs96XOr6oszX5CSl4KnnScvd3u5BqKtmqLbt8n8RTNtvNmkSUaLoyJyg846IiIpg+9Dr5GRW0gbh0Y0tjIjp6AY37bN6dWqqbHDk6Rak5CQgKurq86x/Px8xo0bx/Lly2nVqlWZSU5lS02kpaWVu9REdHR0ufGUV29Fy1P8W0xMDLa2trRo0ULvawyNp+R9Wltrxnq4urpSUFCASqXCw8Oj2u1K1XP8SgoAvm2bY2qiqLhwyhXISARTC2g9oMKicRlxBF0KAuCdvu9gYVr5isi1JW3rNkRBAVbdu2Hds4fR4qiITHKMLCOnkBmbQ7X/If7NRAEbJvVhsD6buknSXWxMTLgyqKvR2tZXbm4uVlZWOscWLFiAt7c3zz//fE2Hdk8IIVAoKvliq2ElyU5OTs49bVcq2/ErtwHNoONKRfyg+dmqH1g0qrDoZ6GfUSyKGew2mD4t+lQ3zCorzsoibfNmAJpPmnTPP+/6kkmOEd3OyueFgJNcuJGJhakJyi4ueLk0IfZWNnlFxdzMzONUfBozN4ex078/7ZyaGDtkqR5RKBR63zIyJgcHB9LS0nSOHTp0iPPnz/P9998D/9wqd3Bw4L///S//+9//Kl1qwtTUtEpLTZRXb0XX/FuHDh3IyMjgxo0b1e7Nqex9lkhNTQXA0VH+QWRseYXFnI7XfKb7t61kr6rCXDj5peZ5r4kVFj1z8wyHrh7CRGHCbJ/ZNRFqlaVu3EhxejoWnp40+dft1LqkWts6SFWXll3AuK/+4sKNTBwaW/LLqwP4fFxP/Ie0Y8Uz3Vk9vhffvdSXB1o35U5+EVM2niYjt9DYYUtSjevZsydRUVE6x3744QfOnj1LeHg44eHhrF+/HtCM3/H39wdqb6mJyurVx1NPPYWFhQXLli0r8/y/p8JXRN94IiIicHNzw8FBj54DqVYdv3Kb/CI1jk0saefUuOLC4ZshJwXsW0GnJyss+tW5rwD4T7v/0Na+bQ1Fa7ji9HRSNwQC4PjaqyjM6m5/iUxyjCC3oJgpG08RczMLF1srdrzcDy+X0gPTLM1MWfe8Dy3trUlIyWFe0Fm9Bn9LUn2iVCqJjIzU6c1p27YtXbp00T5K1uTy9vbGyUmzNP706dOJjY1l/vz5REdHs2bNGnbs2MHs2f/8hTtnzhy+/vprNm7cyIULF5gxYwbZ2dlMumuQ5IQJE3QGJ7/++uvs3buXFStWEB0dzXvvvcfp06cNmuTg7u7Op59+ysqVK5kyZQpHjx4lISGBP//8k5dffpkPPvhAWzYqKorw8HBSU1PJyMjQJnYl9HmfoEkAhw8frneMUu3Z8Gc8AE90d634Nk5xERz/XPPc91UwLT9ZuJJ+hT+S/kCBgsldJtdgtIZLCQhAnZWFpZcXTZRKo8ZSqXsw06vOMsYU8qJitZgSeEp4vLlLdF20V1xUZVZ6TXhimmj/9h7h8eYu8eVRPdZbkO479X16cJ8+fcS6devKPX/48OFSU8hLjld3qYnBgweLiRMn6hzbsWOH6NChg7CwsBCdO3cWu3fv1jm/aNEi4eHhUen72r9/v1AqlaJp06bCyspKeHl5iTfeeENcv35dW8bDw6PMpTkMeZ+5ubnCzs6u3LWGSsrU589IfXFRlSk83twlPN/aJRJTsisufGG3Ztr4h62FyM+qsOjCPxeKLoFdxOuHXq+5YKugKCNDXOjZS0R19BKZBw8ZLQ59v78VQty/XQOZmZnY2dmRkZFxz7Z4+GBXFAF/xGFpZvL37Sj9doz99q8E3v0pAnNTBbtfG0gHZzk+R/pHXl4ecXFxeHp6lhrEWx/s3r2befPmERERgYkBg5aNZeLEiSgUijJXWDaGtWvXsnPnTn7//fdyy9T3z0h98dYP59h26iojuriw9vnSSyPo+PV1CA2EPi/DY2Xf2gS4nXub4d8Pp1BdyKYRm+jp1LNmgzZAyvr13Px4BZYdOuD5809GG3Cs7/d33f9t0oBsPpFAwB9xAKx4prveCQ7A831bMczbicJiwfzvz1Gsvm9zU6kB8vPzY9q0adrtDuoyIQRHjhzRueVkbObm5nz++efGDuO+l5ZdwM4zms/wlAc9Ky4sxD97VbUbWmHRwIhACtWFdHPoRg/HHjUQadWIggJSv/0OgGYvvlhnZ1TdTSY598gfMbdZ+HMkAHMf6cDj3VwruUKXQqHggye70MTSjPCr6Ww8Hl8LUUqS8cyaNQt3dz02MTQyhUJBQkJCnYr1pZdeomNH/XatlmrPoeib5Bep8W5hi49HJeubpcZCeiKYmINH+WvjJGQmsDlaM1X75e4vGzWxyNy3j6LkZEwdHLB93M9ocRhCJjn3wOWbWczYHEqxWjC6Z0tmPtyuSvW0sLNmwWPeAHx24BL5RcU1GaYkSZJUDcdibgEw1Mup8mSkpBenVT+wLH8G1orTKyhSFzGg5QAGuQ2qqVANJgoLSflKM7ur2XPjMbEw3iKEhpBJTi3Lyi9i6qbT3MkrordHU5aO6VqtTPzZB9xxtrUkM6+IY5du12CkkiRJUlWp1YLgGM3v5EH6LN6q3cZhSLlFTqlOcfjqYUwVpszvXfYWIfdKSsA35MdcxtTODvtnn9XrmoK8olqOqnIyyalli36OJO52Ni3trfnyBR8szaq3OJuJiUJ7q+uXs9drIkRJkiSpmiKvZ5KaXUBjSzN6trKvuHBxIcQd0zyvYK+q7Re3AzC6/Wja2LepoUgNlx8bx+01awBw/u/bmDWtfKshIQS/rjrLz5+dIU2VXdshlksmObXo5/Akfgi7hokCPnu2B80b18ymeU901yQ5B6KSySkwfqYsSZJ0vyu5VeXbtjnmppV8tV47BQV3wLoZuHQvs0hmQSaHEzW9PU91eKpGYzVEbng412bMQBQU0GjQQGxHjtTruuuX0lHFZnDjcgYW1sZbLFAmObUkLbtAO9B45sPtDZpJVZlubnZ4NLcht7CY/VHJlV8gSZIk1apjlzRJjl63qs5rtiuh/SNQzpIJ++P3U6AuoK1dW7ybeddUmAZJ2RBI/PjnKEhIwMzJiRbvvaf3cIvTv8UD4D2gBY3sauYP/KqQSU4tWXkwhozcQrxcmvBaFQcal0ehUDCy5JZVuLxlJUmSZExZ+UWEJmhW7B7UvpJtNQrzIOLvJKf7uHKL/Rr7KwAj2440yoyq/MuXubliBajV2D4xkja//Iy5q36zglVxGVyLTsPEREHP4a1qOdKKySSnFly+mcW3fyUA8O7jnTCrrOuyCp7sqfmwHYy+SWhCao3XL0mSJOlnf5SKIrWgdXMbPJpXvIs4F/dAXgbYuoFn2bOlkrKSCE0ORYECvzb3fqq2EALV4sVQVETjhx+m5bJlmNrb63396T3xAHTo64xtc+uKC9cymeTUgiV7LlCsFgzzdmJAu9rZLK+dUxOe9nED4J2fIikqVtdKO5J0L6SkpODk5ER8fLyxQ6mX9u7dS48ePVCr5e8BY9h28ioAY3q5VV747FbNz+7PgknZE1G+i9IsuNfHpQ8ujVxqJEZD3Nm/n5yQv1BYWOC84C2Drr1w/AYJ51NQKKCX0qOWItSfTHJq2M07eZy7loGZiYK3H6vd+6hvjfDCztqcCzcy2RSSUKttSVJtWrx4MaNGjaJ169Y6xwMDA+nWrRtWVlY4OTlpdyAvIYTg448/pkOHDlhaWtKyZUsWL16sPf/i36uy/vvRuXPnCuM5d+4cAwcOxMrKCnd393J3E6/M5cuXmTRpEm5ublhaWuLp6cm4ceM4ffq0znvv378/NjY22Jfz1/Jrr72Gj48PlpaW9OjRo9T5Rx99FHNzczZv3lylOKWqi72VxYm4VEwU8FTvSpKcOyq4fEDzvMf4MovEZ8SzLXobAJO73vuNOAtv3kT1vmY172ZTJmNhwKKXqdezObbtIgB9RnrS1KWSXq17QCY5NcypiRVH5j3EVxN8aONY/gJPNaF5Y0vmKTWrnK45cln25kj1Uk5ODgEBAUyZMkXn+CeffMJ///tf3nrrLSIjIzlw4ADKf+14/Prrr7N+/Xo+/vhjoqOj+eWXX+jTp4/2/MqVK7lx44b2cfXqVZo1a8bTTz9dbjyZmZkMHz4cDw8PQkNDWb58Oe+99x5f/b0Qmr5Onz6Nj48Ply5d4ssvvyQqKoqdO3fi5eXF3LlzteUKCgp4+umnmTFjRoX1TZ48mbFjx5Z7/sUXX2TVqlUGxShV347T1wB4qKMTLewquTVzbjsINbj3g+ZtyyzySegnFIkiBrkNor9r/5oOt0KisJCkOXMovn0byw4dcJg2Te9riwvV/B4QQVGBGjevpvR6tHXtBWqIWt8qtA4zxi7kNa2gqFj0fP934fHmLnHk4k1jhyMZSVk7TKvVapGdX2iUh1qt1jv2oKAg4ejoqHMsNTVVWFtbiwMHDpR7XVRUlDAzMxPR0dF6t7Vz506hUChEfHx8uWXWrFkjmjZtKvLz87XH3nzzTdGxY0e921Gr1aJz587Cx8dHFBcXlzr/793UhRBiw4YNws7OrsJ6Fy1aJLp3717muYSEBAGIy5cvl3le7kJe8/ILi4XPB/uFx5u7xN6IGxUXVquF+KKPZtfx04FlFjmtOi26BHYR3Td2F1fSrtRCxOUrTE0V1+bMFVEdvUR0Lx+RFxtr0PUnfrkivnj5oAh445jIzsiv/IJq0vf723iT16UaYW5qwuPdWrApJIGfzyQxWJ/pi9J9IbewmE4L9xml7aj3ldhY6PfrJTg4GB8f3d2a9+/fj1qtJikpCW9vb+7cuUP//v1ZsWKFds+oX3/9lTZt2rBr1y4effRRhBAMGzaMZcuW0axZ2Us2BAQEMGzYMDw8yh8rEBISwqBBg7C4a9l6pVLJRx99RFpaGk31WAgtPDycyMhItmzZUuau6uXdlqqOVq1a4ezsTHBwMG3blt1LINWsVQdjuJ2Vj2MTSx72cqq48PUwuBUNZtbQ+ckyi2y+oLnd+J/2/7mni//dOXSIG2//l+L0dFAoaLFkCZaelWwwepeUpCxC92qGTAwc2wEb27qz5YO8XdUAjOqhmWm1L1JFboHcz0qqXxISEnD919TU2NhY1Go1S5Ys4bPPPuP7778nNTWVRx55hIKCAm2ZhIQEgoKC2LRpE4GBgYSGhvLUU2UvnHb9+nV+++03XnrppQrjUalUODs76xwrea1SqfR6TzExMQB4eXnpVb6muLq6kpAgx+fdC3/FprD6yGUA3hvZufIFAMO3aH56jwQru1Knb+Xc4lCiZj+rcV7lTy2vaTmhoSS9Povi9HQs27fH47tvsVUON6iOo1suoi4WeHZ3oJ1PJcnePSZ7chqAXq2a4tbUmmtpuRy4kMzI7obtcC41TNbmpkS9r6y8YC21ra/c3FysrKx0jqnVagoLC1m1ahXDh2t+4W7duhUXFxcOHz6MUqlErVaTn5/Ppk2b6NChA6DpqfHx8eHixYulduXeuHEj9vb2PPnkk9V7c3oQQtR6G2WxtrYmJyfHKG3fT3IKipizPRwh4GkfN/y6taj4gsK8fxYALGfA8c7LOykWxfRw7EGHph1qOOKyFcTHc81/JqKwkCaPDKPlJ5+gMDc3qI6UpCxuXMnAxFTBoGc7GnWX9LLInpwGQKFQaHtzfg5PMnI0Ul2hUCiwsTAzysOQX3QODg6kpaXpHGvRQvOl0alTJ+0xR0dHHBwcSExM1JYxMzPTJjgA3t6aGY0lZUoIIfjmm2944YUXdG5DlcXFxYXkZN2VxEteu7joN523JKbo6Gi9yteU1NRUHB3lLeva9kv4da5n5NHS3pr3nqh4ph4AET9AXjrYtixzbZxidTE/XPoBgKc7lj8oviZl7t1L3DNjKU5Px6prV1yXLTM4wQG4dFLTu+nRpTmNmxpvZePyyCSngXiie0sAjl26TWZeoZGjkST99ezZk6ioKJ1jAwYMAODixYvaY6mpqdy+fVs7nmbAgAEUFRVx5coVbZlLly4BlBpzc/ToUS5fvlxqBldZfH19OXbsGIWF//w/2r9/Px07dtRrPA5Ajx496NSpEytWrChz7Zr09HS96jFEXl4eV65coWfPnjVet6Rr6ynNujgTfD1oZFnJDZHiIji2XPO878tlro3z5/U/uZ59HVsLW4Z7GHaryFCFN25wbfZskmbNRp2ZiVWXLrivWY2JteGL9gm14NJJzR8AHfve+/V89CGTnAaig3Nj2jo2oqBYzaELN40djiTpTalUEhkZqdOb06FDB0aNGsXrr7/O8ePHiYiIYOLEiXh5eTFkyBAAhg0bRq9evZg8eTJnzpwhNDSUl19+mUceeUSndwc0t7H69u1Lly5dSrX/xRdfMHToUO3r8ePHY2FhwZQpU4iMjGT79u2sXLmSOXPm6P2eFAoFGzZs4NKlSwwcOJA9e/YQGxvLuXPntGsClUhMTCQ8PJzExESKi4sJDw8nPDycrKwsbZnLly8THh6OSqUiNzdXW6ZkfBLAX3/9haWlJb6+vnrHKRku6nomZ6+mY26qYIyPHov/ndsGaXFg4wAPlD0eLOhSEABPtH0CKzOrMstUlzo/n9vr1nHlMT/u/LYXTExoPv1lWm/dglkVe/+SYtLJSsvH0sYMj67NazjiGlLr87zqsIYwhfxuH++LFh5v7hJTN54ydijSPVbfpwf36dNHrFu3TudYRkaGmDx5srC3txfNmjUT//nPf0RiYqJOmaSkJDF69GjRuHFj4ezsLF588UWRkpKiUyY9PV1YW1uLr776qsy2Fy1aJDw8PHSOnT17Vjz44IPC0tJStGzZUnz44Yc65w8fPiwAERcXV+H7unjxopgwYYJwdXUVFhYWwsPDQ4wbN06EhYVpy0ycOFEApR6HDx/Wlhk8eHCZZe5uf9q0aeLll18uN5b6/hmpK9796bzweHOXeOW70MoLFxUI8WlXzbTxP1aWWeRG1g3RbWM30SWwS61NG88ODRMxjwwXUR29RFRHLxE3/jmRGxVV7XoPbIwSX7x8UBz69kINRGkYfb+/FUIYaYRcHZCZmYmdnR0ZGRnY2toaO5xqu3AjkxErg7EwMyHs3UdoXFk3qtRg5OXlERcXh6enZ6lBvPXB7t27mTdvHhEREWVOua5rNmzYwJIlS4iKisK8CuMYatrt27fp2LEjp0+fxrOcqb/1/TNSF+QUFNF3yUHu5BXx3ZS+PFjZZpznv4cfpkAjR3j9LFiUXgF4Tfga1p5dS2/n3mx4dEPNxxwWRuJLUxE5OZg5OuI0fx62jz9e7QHCt6/dIejD06iLBP+Z2wvX9vY1E7Ce9P3+lt+CDYiXSxM8HRoRdzubw9E35Swrqd7w8/MjJiaGpKQk7To4ddmePXtYsmRJnUhwAOLj41mzZk25CY5UM34IvcadvCI8mtvQv60et2dOBWh+PvBSmQlOkbqIH2L+HnDcoWYHHOfHxpEdfIxbK1chcnJo1N+Xlqs+x7Rx9bdaKCoo5veAKNRFgtbdHGjRrvSU+LpCJjnGJgSEBsKVQ5B9G7JvaR727vDAVOj2DJjrNyBMoVAwoosLa45cYc/5GzLJkeqVWbNmGTsEvQUFBRk7BB29e/emd+/exg6jQVOrBQF/xAEweYAnJiaV9IQkR0HicVCYQq8JZRY5kHCAmzk3aWrZlGEew2os1psrV5Kydp32tU3fvritrtrg4rIc33mFtBvZ2Nha8PALXnVu2vjdZJJjbH9+BgfeK31clQ6/vgbBH8PTgdDSp3SZMjz6d5ITHHObgiI1FmZ1v+tfkiSprjsYfZP4lBxsrcx4Sp8Bx6e/0fz0egxsS//BmVeUx2dhnwHwrNezWJjWzCrBmb//rk1wbHz70XjQYJo+O7bGEpzrl9M5f1izX9fQid5YN6k7qxuXRSY5xqIu1vTglCQ4/fzB/QHNvVvrpnDlMPy1BtIT4ZtHYcRH0LvyHWm7uNrRvJEFKdkFhCWm0a9NHR3xLkmSVI98HRwLwPi+ekwbz8+Cs5qdxOld9rIFm6I2kZSVhLONMy92frFGYsyPi+PGgrcBaDZpEs5vzq+ReksUF6o58p1m7Sfv/i1o1bnuf7/IJOdeU6sh5Av4ay3cua455jsTlIt1yzl3hl4vwE+vQPQu2DUbMm/AkLehgq5BExMFA9s78FP4dY5duiWTnPvMfTyPQKqE/GxU3c/hSZyMS8XMRMHE/uXve6YVthEK7kCztuA5uNTpmzk3WX9+PQBzfOZgY25T7RjVOTkkvfY66uxsrHv74DRndrXr/LdTu+NIU+Vg3cSc/mPa1Xj9tUHey7iXCnPhh8mw/11NgmPdFAbNh0c+KLu8lR2M/Q6G/Ffz+tgy2Lug0mYGd9SseXD00q2ailyq40oGwMol/aXylHw26spg6friyq0s3v7xPACvPNSWFnaV3PYpzIU/V2qePzgLypgt+NPln8gtyqWbQzdGeI6odoxCCG689x75MTGYOjpUaXuGiqjVgj++j9HZhNOqUf34HMmenHsl6yZsHQdJp8HEHEZ8CD1fALNKlsFWKGDwfLBpBrvfgBNrwckLfF4s95KB7TVJTuT1TG7d0eyQKzVspqam2Nvbc/OmZiFIGxubOj0YULp3hBDk5ORw8+ZN7O3tMTXVf1+x+11WfhH+m8PILiimX5tmvD5Mjz2lQjdCVjLYtYJuz5ZZZG/8XgCe6vBUtf+fCrWaW6tWkfnLr2Bqitsnn2DuVHObZAq14MA3kcSc1vxu6TuqTZ3bhLMiMsm5F25egC3PaMbXWNnDs5uh9YOG1fHAS5CXAQffhz3zwLkruJU9GNmhsSVdWtoSkZRJcMwtRvfSY5CcVO+V7KtUkuhI0t3s7e313ntLgsJiNa9sDiNadQeHxhaserYnppXNqCrM00wmARg4G8xKD8qNTY8lJi0GMxMzHm71cLViLM7K5vpbb5J14CAATvPewOaBB6pV592E0PTgxJy+iYmpgqEvetPhgfr1GZJJTm1LjYNAP8hJgWZtYHwQOFTxXuaDcyApTDNGJ2gizPhTc0urDIPaOxKRlMnRSzLJuV8oFApatGiBk5OTzr5LkmRubi57cAz0353nOXbpFtbmpgRMfAAnWz0WUDy7Be7c0GzE2eO5MouU9OL0d+2PnWXV15cpzsrm6tSp5J45g8LcHJf33sN+zOgq13c3tVqQdDGNS6eSiT5+A6BeJjggk5zalZcBW5/VJDgtusMLP2luO1WVQgFProUvIyAtHva+DU+uLrPooA6OrDlyhT8vpyCEkLcu7iOmpqbyC02SquHopVvsOH0NUxMFq5/rSXd3+8ovKi76ZyxO/1fLHIoghNAmOcrWyirHp87O5urLL5N75gwmtra4f7kOmxrcmPX39RFcCftnTGf/0e3qZYIDcuBx7RECfpwGt6KhSQsYt616CU4JK1tNooMCwr+D6D1lFuvZyh4rcxNuZ+UTczOrzDKSJEmSrmK1YOmeCwC82L81D3s563dh1E+aPz6tm5W7+N+F1AvEZcRhbmLOEPchVY5R9X+LyQ0NxaRJE1oFBNRogpMYmcKVsFuYmCrwHtCCka92p8cjVVuFPGzPz5zetdOoM/tkklNbwjbCpb1gagnjtpa5GFSVefSH/jM1z3fN0vQY/YulmSkPtNYkVccv3665tiVJkhqwH0KvEa26g62VGa8+rOfQAiHgj880z/tOL3MLh2J1MYtPaJYKGdpqKE0smlQpvuzjx8nYuRMUCtzXrMa6a5cq1VMWtVpw/MfLAHR9yI2HX/CmVefmVboTEHvmFEc2BXD02wASzp2psRgNJZOc2pCeCPve0TwfuhBcay7L1hryjmYNhqxkOPJhmUV8/95b5fiVlJpvX5IkqYHJKyxmxf6LALz6cHvsbfRczffyAUg+DxaNoc/UMot8d+E7zt06RyPzRsztPbdK8alzc7mx6D0Amo4fX6ODjAEijl4jJSkbSxszej/Wusr13L6awO6VyxBCTdeHh+PRrRa+A/Ukk5yaJgT8PFOzEJR7P+g3o3baMbeCx5Zrnp/4ElQRpYr0b6vZIfev2BSK1XIhMEmSpIr8HJ5EcmY+LeysmKDPon8lgj/R/PR5scxhCVfvXOXzM58D8EbvN3BpVLXxLbe++ILCq1cxc3HBcXbNLfZ3JzWPPWvPEbw9BgCfEa2rvA5Ofk42Py3/gILcXNw7dWXolBlGHRMqk5yalpUMGVfBzBqeXAMmtTgAtN1Q6DQKRDH89qYmwbpLl/9n77zDqyjTPnzP6f2k90ZISCD03ouCqAii2Htb/eyufdVV17LuKtZde1m7WBBFRaSD9F5CCSG995zeZ74/BgIxCQYEy+65r4uLZOadck7OmfnN8z7P70myYNaqsHuD7Km2n7zzCBMmTJg/OJIk8daPcgPOq8dkoFV189pdvl5uxKlQw6ibOx3y/Jbn8YV8DE8YzqzsWcd1fp7du2n+z7sAJDzy8AnpJg5QW2zj86c2UbKjEUEhMHBKGgNOOb6KXEmSWPzmy9jqarHExjP9zr+gVP22poFhkXOiMSfA/62By76A6J4n/3hT/y7n/ZSthpKV7VaplApGZB7MyykK5+WECRMmTFes2N9AYb0Tk1bFRcPTur/h6ufl/wde3Gnu5bb6bSwuW4xCUHDf8PuOK6ohBQLUPPRXEEUsZ56BedLxJy0fScGGWr56bhseR4CYVBMXPjSMMbOyUCiPTxrkr1hMwdpVKJRKzrr9XvRmywk5z19CWOScDDSGYzL7EyWRtVVruXvl3fx5+Z/5rvg73IFu2vNbU2Do1fLPK/7RIZoz6uCU1ZpwXk6YMGHCdEowJPLaiiIALhyWikXXzehD0TK5wAQBxtzRYbUkSczeNBuAc7LOoVdkNxyTf0LIbqfqzrvw7d2Lwmol/oEHjnkfPyXoD7H8w30s+c8eQkGRjP4xnHPXYKKTTMe9T1drCyveexOA0RdcRmJ2zi8+zxNB2CfnN2R7/XbmF81nTdUaql3VbcuXlC9Bp9QxIXUCZ/Q4g7HJY9Eqj9KaYcwdsPk/UL5OjuZkTmxbNTZLFjkbipvw+EPoNWH/lDBhwoQ5RL3dyy2fbGtrwHn1mIzubdhSBl9cI/889OpOI/fLK5azs3EnepWeWwbdcszn5q+spPyqqwlUVoJaTeLf/oYqJuaY93MkrXVuFr6RT1OVEwQYekYGw87qgeLn3Jx/hjWffoDf4yGhZzbDZxzflNzJICxyfiOWly/nzyv+TEgKAWBUG5mZNROj2sjCkoWUO8r5ofQHfij9AZPaxHm9zuO2QbehVnbyhGFJlL9kG16Dlc+0Ezm94k0kWXVU27ysL25iUu4fp+dImDBhwpxM/EGR819fR1mTG6NGybMXDCAlshsdwYN++PQy8LRA0mCY+lSnw/6T/x8ALsm9hBj9sYuThhdeJFBZiTo5meQXnkffr98x7+NICjfXsfyDfQR8IfRmNVOuySO19y/3b6svLWbX8sUATLzyeoROmpL+VoRFzm/AxpqN3L3ybkJSiAkpE7gg5wKGxg/FoJa/XLcMvIU9zXv4vvh7vi/9nnp3Pe/ufpcdDTt4buJznX9ZxtwOG9+Uc3Ma9kOsHBYVBIEJOXF8srGcFQX1YZETJkyYMAf5Pr+GsiY3MSYtn94wkp6x3Zyu2T0PanfKxn8XfiBXu/6E7fXb2d6wHbVCzaW9O2/xcDQCVVXYv/8egJR/vYSuT59j3schgv4Qa+YeIH9lFQBJ2RGcdl0eRusvb94sSRIr3n8LJImcUeNIzun9i/d5Ivn9yK3/ASRJYu7+udy45Eb8op9JqZN4YdILjE8Z3yZwQBYmedF53D3sbhaft5jnJz6PWW1mW/02rvj+Chx+R8edW5Ig+zT5523vt1s1KUfuSr68oOE3dZ4MEyZMmN8TH6wrA+DykendFziSBOsPttMZdbOcF9kJh6I403tOJ9YQe8zn1vz+BxAKYRg18rgEjt8bpOZAK+u/KuK9B9a2CZwhp6dz9h0DT4jAASjavIGK3TtRqtWMv/TqE7LPE0k4kvMr0ehp5JlNz7CgRG7DMDFlIs9MeAaV4uh/AoWgYHL6ZLIisrhh8Q1UOCp4ZO0jPDvh2Y5Z+oOvgP3fw445cMrDbR1wR2fFoFYKlDe7KWl0kdndL3OYMGHC/Jeyu9rG5rIWVAqBi4cfQ9uCsrVQswNUOhjS+U19bdVallcsB+DKPlce87mF7HZaP/8cgOhrrjm2bYMia788wK4VVUhH+KOZIrVMvDSX9L7Rx3w+XR8rwMoP3wZg6FnnYIn9/c0UhCM5JxlJkvis4DOmz5vOgpIFKAQFtw++nRdPefHoycQ/IcOawewJs1EpVCwuW8wn+z7pOCj7NDAlgKvhYMa/jEmrYngPed51eUFDx+3ChAkT5n+MQ1GcM/oldq/D+CHWvyL/P+AiMHYUDMvKl3HLsluQkJiWOY3MiMxjPrf6Z59DdLvRZmdjHNv9Sl17o4cvZ29l57JKJFHCGKElo38Mp1/fl8ufGHWCBU6Q9V9+RmttDcaISIaffd4J2/eJJBzJOYn4Qj4eW/cY84vmA9Anug8PjXiIfrHHlzzWL7Yfdw65k6c3Pc2zm59leMJwsiKP6K2iVMHAS2D1c7D1fegzo23VxF5xrDnQxIqCeq4d2+MXva4wYcKE+SOzsaSZuVsrAbhi1DE4GxcugX3fyT+P6OhmX9RaxF0r7iIoBZmcNpnHRj92zOfWOu8rWj/9FASBuHvv7bavTunORpa8uwefO4jWoOLUq/rQo/8vq8TqDEmS2PzNl2ycPxevQzaZHXPh5Wj03UjY/g0IR3JOErWuWq76/irmF81HKSi5a8hdfHzmx8ctcA5xWe/LGJs8Fr/o54HVDxAIBdoPGHSZ/P+BJWCrbFs8KVeeE95Q0ozbH/xF5xAmTJgwf1TKm9zc8MFmAiGJaf0SGZoe2b0Nq7bAZ1cAEgy8DOJyOwz5YM8HBKUgo5NG88yEZ9Aou9n76iC+wkJqH30UgJibb8Y07uejOC6bj2Xv7+W7V3bicweJy7BwwYPDTprAWf3Je6z66D94HXYM1ghGnXcxeRNPPeHHOlGERc5JYGvdVi789kLym/Kxaq28NuU1rup7FcoT0OJBEAQeG/0YVq2Vvc17eW3na+0HRPeEjHGABNs/blvcM9ZEcoQef1BkXdgYMEyYMP9jeAMh3ltbyvmvr6XFHaB/ipXZ5w/oXqSkqQg+ugACLsicBGc932FIi7eFb4u/BeCG/jf8bL7lT5Ekidon/47k82EcN46Ym36+72HF3mY+fHg9e9fWANB/Ugrn3j0YS7T+mI7dXdZ98Qkbv/4CgAmXXcMNr77H6PMvRXEy2xf9QsIi5wRT66rlT4v+RLO3mV6RvZgzbQ4jE0ee0GPEGmJ5aKTc5fzNnW+yrnpd+wGDr5D/3/oBiCIgi6ND0ZwV4bycMGHC/A/h8AaY+fIaHpm/mzq7j/RoA29eMbR75qjOevjwXHA3QuIAuWRc1TFCM7dwLr6Qj95RvRkUd+xdt53Ll+Nevx5BoyHhkUd+1mtGDImsmrOfoC9EXIaFWfcOYdyFvVCqTs5tvbG8lPVz5wAw6aobGDr9XBTK36+4OURY5JxgEowJXN//eqZmTOWDMz4gxXx8jc5+jtMzTufc7HORkLhv1X3UumoPr+w9HbRWsJVDyYq2xRN7yZnvywvqw6XkYcKE+Z9AFCXu/nwH+2odRBs1PDGzL4v+PJ747iQbOxvgw1nQUgqRGXDpF6A1dxgWFIPM2ScLgEt7X3rM/akkv5+6f/4TgKirrkKTkvyz2+zfVEdrnRutUcXZtw8kIdN6TMc8pvOTJFZ88DaSJJI9fDSDz5h+0o51ogmLnJPA9f2v55nxz7TzvjkZ/GX4X8iNyqXF18J9q+5DlOSoDWo99L9A/nnrYc+c0VnRaJQKKls8FDW4Tuq5hQkTJszvgVdXFvHD7jo0SgVvXTmUy0amd6/DeGMhvD1ZNv0zxMBlX4Kp8xLpLwu/pM5dR5QuijN6nHHM59j88ccEyspRxsQQff31Pzs+FBLZ9K3cMX3waelo9Ce3hqh46ybKdm5DqVIx/rJjK2n/rTlmkbNq1SqmT59OUlISgiDw1VdftVsvSRIPP/wwiYmJ6PV6Jk+eTGFhYbsxzc3NXHrppVgsFiIiIrj22mtxOp3txuzcuZNx48ah0+lITU3l6aef7nAun3/+Obm5ueh0Ovr168eCBQuO9eWcFARBOK5Os8eKTqXjuQnPoVfp2Vq/la8OfHV45aCDDpsFC8EvCxqDRtXWlXxFQf1JP78wYcKE+S1ZUVDP7EUFADx2dh6D0rqZZOy1w3/OlCM4EelwzcJOe1MBOP1OXt4umwNe3//6Y042Dra00PjKqwDE3XE7SpOxy7GSKLFvfQ3zX9iOvdGL3qym38STM1twiMbyUha/8S8ABk+bSUR8wkk93onmmEWOy+ViwIABvPzyy52uf/rpp3nppZd47bXX2LBhA0ajkalTp+L1etvGXHrppezevZvFixfz7bffsmrVKq4/Qr3a7XZOO+000tPT2bJlC8888wyPPvoob7zxRtuYtWvXcvHFF3Pttdeybds2Zs6cycyZM8nPzz/Wl/SHJtWSys0DbwbguS3P0eJtkVckDpS/nEEPFC5uGz+hl5yXs3hP3a99qmHChAnzq1HW5OK2T7YhSXDx8DQuGp7W/Y23vAuueojKhOuWQkx2l0Pfzn+bZm8zGZYMLsi54JjPs/Ff/0a029H27o31nHOOOnbdV0UsfXcv1YWtIMDoc7NQa098XowkSTRXV7F39Qo+fewBXK0txKZlMPKcY399vznSLwCQ5s2b1/a7KIpSQkKC9Mwzz7Qta21tlbRarfTJJ59IkiRJe/bskQBp06ZNbWO+//57SRAEqaqqSpIkSXrllVekyMhIyefztY257777pJycnLbfL7jgAmnatGntzmfEiBHSDTfc0O3zt9lsEiDZbLZub/N7xB/yS+d+fa7U992+0sNrHj684oeHJOkRiyR9fnXboopml5R+37dS+n3fSpUt7t/gbMOECRPm5FLe5JImPbNcSr/vW2nmy6slbyDY/Y0DPkmanStfO7e8f9Shxa3F0pAPhkh93+0rLStbdszn6d6VL+3pkyftycmVnOvWH3VsU5VTeuXGZdK/b1gqrZ13QGqtPznX72AgIH31zOPS7Aumtf378IE/S26H/aQc73jp7v37hObklJSUUFtby+TJk9uWWa1WRowYwbp1cgXQunXriIiIYOjQoW1jJk+ejEKhYMOGDW1jxo8fj0ZzOOw3depUCgoKaGlpaRtz5HEOjTl0nM7w+XzY7fZ2//4bUCvU/HXkXwH4+sDXVDur5RV9Zsr/7/8BAh4AUiINjDjofvzVtqpf+1TDhAkT5qRQY/Mwb1slH20o49xX11Lc6CLJquPVS4d0LwfnELu/BEc1mOIP5zZ2gi/k456V9+AL+RiVOIqJqROP6Xx9xSVUXH89hEKYp0zBOHJEl2MlSWLVpwWIokSPATGMmtkTa+yJLxOXJInFb/6bA5vWo1CqiM/MZvAZMzjvwSfQmzomXP8ROKHZSrW1coVPfHx8u+Xx8fFt62pra4mLa5+8pVKpiIqKajemR48eHfZxaF1kZCS1tbVHPU5nPPXUU/ztb387jlf2+2dg3EBGJo5kfc16PtjzAfcNvw+SB4MlBeyVULQMcqcBMGtwChtKmpm3rYqbJvb8VfKHwoQJE+Zksbygnts+3obDd9joNDfBzLtXDyfBegwtG0JBWPOS/POIG0DVdeud2ZtmU9BSQJQuiifGPnFM19FgQwPl115LqLkZXZ8+JP79yS7HOpq9bPymmKqCVpRqBWPP73rq7HhprChj98ql1B7YT+XefARBwYy7HqDnkOEn/Fi/Nv9T1VV/+ctfsNlsbf8qKip+61M6oVzdV24WN7dwLjafDQQB+pwtr9z9Vdu4M/oloFUpOFDvJL/qvyOaFSZMmP89QqLEKysOcO27m3D4gmTHmZiUE8tVozP47P9GHZvAAVj0ENTvBq0FhnZdRbSkbAlzCuSS8SfHPkmc4dgaU9a/8ALBmho0PXqQ+tabKM0doyRuu5/VnxXy4cPr2LdOfngfeXYmlpgTG8HZt2YlHz1wJ5u/+ZLKvXJO66nX3viLBE6g3o1zXTX2JWW0zi9CCoon6nSPmRMayUlIkLOu6+rqSExMbFteV1fHwIED28bU17ev7AkGgzQ3N7dtn5CQQF1d+8TYQ7//3JhD6ztDq9Wi1Z6Y9vK/R0YljiI3Kpd9zfv4tOBTru9/PeTNhPUvw75vwecArRmzTs2UPvF8u7OGL7dV0i/l5PkrhAkTJszJoLrVw52fbWd9cTMAFw9P5W8z+qI5XjO8bR/CBrnKiZmvgr7zSqxqZzUPr30YgKvzrmZscvcbaAJ4CwqwfTkPgKSn/o4qKqrDmNoSG/Nf2E7AF5LHZUcwcmZPEnueuGu13+Pmx0/eZ/sPsktzWt8B5IweR1J2LjFpGce9X8++Zpo+3APBw15s5kmpKM3HVnV2ojihkZwePXqQkJDA0qVL25bZ7XY2bNjAqFGjABg1ahStra1s2bKlbcyyZcsQRZERI0a0jVm1ahWBwOG+TIsXLyYnJ4fIyMi2MUce59CYQ8f5X0QQBK7Ok6M5H+/9GH/IDynDIDobAm7YPa9t7NkDZbOpxXvqwsaAYcKE+UOxt8bO2S+vYX1xMwaNkn/O6sffz+n3ywTO/Nvknyf+BXqf1ekwm8/GPSvvweF30D+mP7cOvvWYD1X/zGyQJMynn47+4MP/kUiSxJrPDxDwhYhJNTHjtoHMvHPQCRE49sYGdi1bxKqP/sN/7rqpTeAMmzGLWQ8+Rv9TT/9lAie/kaYPZIGjSTVjHJ6AeWIqKH67lIhjjuQ4nU4OHDjQ9ntJSQnbt28nKiqKtLQ07rjjDp544gmys7Pp0aMHf/3rX0lKSmLmzJkA9O7dm9NPP50//elPvPbaawQCAW655RYuuugikpKSALjkkkv429/+xrXXXst9991Hfn4+L774Is8/f7hfyO23386ECRN49tlnmTZtGnPmzGHz5s3tysz/F5mSMYXntjxHnbuOhaULmdFzhuyZs+RR2PZRW8uHMUcYA5Y0usiMNf22Jx4mTJgwP4MoSizdV8+dn23H4Q2Sm2DmtcuGkBHTtbfMUZEkWPk0rPi7/PuAi2H8vZ0O3Va/jftW3UeNqwaz2sw/x/8TtUJ9TIdzLFuOa/VqUKuJu/PPnY6p2NtMbbENpVrBWbcMwGj95bMPVfv2sPaLjynP3yG/5oNY4xOYfN3NZPQ/9jYUP8Vf7aRpzj4ISegHxBJ1QS8E5W+fEXPMImfz5s1MmjSp7fc777wTgCuvvJJ3332Xe++9F5fLxfXXX09raytjx45l4cKF6HSH50Y/+ugjbrnlFk499VQUCgWzZs3ipZdealtvtVpZtGgRN998M0OGDCEmJoaHH364nZfO6NGj+fjjj3nooYd44IEHyM7O5quvvqJv377H9Ub8t6BWqLko9yJe3PoiH+75kOmZ0xEGXAxLH4eK9bKLZ0w2Bo2K4T2iWH2gkRUFDWGREyZMmN8lFc1uVh9opKjeybKCeooPurUPy4jkrSuHYdUfm9BoIxSE7+6Ere/Jv4+9E059WM5l/AkFzQVc+8O1BMQAqeZUnpnwzDG37Am2tFDziDzNFXXF5WjSOvr2SJLExm9kJ+O+45J/scBx221s+XYeG+fPbRM3STl9iMvIJCY1nT7jJ6HWHmPeUieIviDNH++DoIQuN4qoC3MQfsPozZEI0v/wXIXdbsdqtWKz2bBYLL/JOUjBII4lSwnW16PJzETbMxNVQsIvqnhq9bYy5YspeENe3jv9PQbHD4aPL4T9C2HMHTBFrjB7c1UxTy7Yy4Resbx3zR8/iz5MmDB/fCRJoqjBxZoDjSzMr2VdcVO79SatiouHp3LnlJzuNdjsjIAXPr8K9n8PggLOfAaGXdf5UDHApd9dyt7mvYxMHMnzE5/HpDn2h8KqO+/CvmABmp496fHlXBSd5IcWbatn4ev5qNQKLnti1HGJnNbaGrYv+paC9WtwNjW2Lc+bcCojZ118wh2LpaBI85x9ePKbUFq1xN02CKXxOIXnMdDd+/fJbXgRpktCra3YFy+m+e138JeWtlunMBjQDxlC5MUXYxo3FlSqYxI9EboIpmVOY27hXD7c+6EscgZdJouc7R/DpAdBpWFCTixPLtjL+uImvIEQOvXvv6NsmDBh/jupbHHz0YZyvt9VQ2mTu225IMCwjCjykiz0TrBwRr8EzLpfcBMNeGDOJbKthkoP573dZq/RGW/vepu9zXuxaCz8fezfj0vgNL//AfYFC0CpJOkfT3UqcOxNHpZ/sA+A/qekHpfA2fTNl6z66D/tpqSiklMZe+HlZI8Yfcz7+zlET5CmD/fgK7KBQiDq4pxfReAcC2GR8yvjLy+nfvazOJYtg6Ds6aCMiEA/eDD+0lL85eWIbjeuH3/E9eOP8kaCgGH4cJKe/ifqn3gDdcVlvS9jbuFclpYvpdpZTVKv02VzK2cdFHwHeeeQHWci0aqjxuZlfXETE3OOrQwyTJgwYY4Vf1BkW3kL3qDYVvSwpayFN1YV4ztYaqxRKRiaHsnY7BjOHphMcsQJKpsOBQ8LHLURLv0MMjqvjgqKQV7f+Tqv73gdgL+M+AuxhthjPmTrl/Oo+7uc8xN7++3o+/Xr5LREFr21G587SFy6meHTe3QY83PkL1/Mqg/fASC9/yAGnX4WqX36odGfnEbRUkCk4a1dBKqcCBolUZfmos34/VXqhkXOr4AUCuHZuhX7wh9o/ewzpINVY9qcHKzTzyLioovbmrJJfj++khJsX8+nde5cRJsNJAn3hg2UzDqPlJdewjD455PEsiKz2swB5+ybw51D75STjlc9A5v/A3nnIAgCE3rFMmdTBSsKGsIiJ0yYPwiNTh9KQSDS+NuU5R4Lm0qbeWNVMVP6xDM4LZLb52xjd3Xn/lwjekRx2ch0JuXGYdKehNvT8icPC5zLvoD0zqMb3qCXW5bewoZa2YX/wpwLmdaj62hPV7g2bKTmoYcAiLrqKqL/1HFKzOcOsPCNfOpK7GgNKqb+qS/KblaJVezeyZYF83HbW6k9sB+AYWefx/hLrjrmcz1WWr8rJlDlRGFUEXNtPzRJv8+8znBOzknOyXFt3EjtI4/iLylpW2YcPZq4++5Dl9PrqNtKwSAhh4NgfQPVd9+Nr7AQ1GoS/voQkRf8fKO0lRUruWXZLZg1ZpactwSDqwle7A+SCLdsgZgsluyp47r3NxNpULPuL6eGp6zChPkdEBIlqlo8VLS4EQTITbAQdVDQfL29inu+2IlBo2TeTWPocbyVRSeJ1YWNvLz8AKflxZMTb+ba9zbjCYTajTHrVKRGGtpyfE1aFVePyWBq3i/LRzwq+3+Ajw9eN2e9Df3O63SYJEk8sPoBvi3+FoPKwMOjHmZa5rELnJDNRvHZMwnW1mI9ewaJ//hHh9fmtvv5+oVtNFe7UGmVnHlDP1L7dPTN6bDvYIDVcz5g87fz2k1N5U2YzNQbbz+pLvYhhx/39gZs3xUDEHNNX3S9utnd/QQSzsn5jZEkibqnnqLl/Q8AUFgsmCdNwnLWWRjHjunWh1BQqVBFRqKKjCRjzidU/+UBHIsWUfvwI/j2FRD/4AMIyq5FybiUcaSZ0yh3lPNN0TdcmHshZE2Bwh9gy39g6pNMzIklOUJPVauHb3ZUc/7Q1BP2HoQJE6YjvmCIF5YUsqG4iWiTFrNWhS8kYtaqGJIeSZ3dy/vryqh3+NptF2fWkhZlYHOZ3L/PHxT50/ub+ce5/fh8cyVVrXJ/OoNGSZxFS98kK6flJbSJI39QxO0PYtKqUB1R2uvxh1hX3IhVr6ZvsrVDn6eKZjfPLiqgwSmfz4CUCE7tHYfTF6K8yYVaqcCqV5MebWR/nYN7vthBICS1SxgekGKlqtVDo9PPsIxIXrp4EInWE997qVOCflj9vBzFBhh+fZcCB+D9Pe/zbfG3KAUlL53yEiMSu+4p1RWSJFH72OMEa2tRp6eR8PDDnV7zV39eSHO1C6NVw7SbBxCb1r3+UEveeoX85YsB6DvpNDKHDMMUEUVCVq+TJnBCdj8tXxbi3dfctsw8MfU3ETjHQjiSc5IiOXVPP0PzO/L8aMSFFxJ3150of+ExJEmi6fXXaXjxJdlM6rTTSHrm6U6T2A7x0d6P+MfGf5BmTuPrmV+jKlwCn1wIOivcuRc0Rl5ZcYCnFxbQN9nCN7eMDfeyChPmBPHZpgrWFDVy/fhM8pKslDS6uGPONnZU2n52W41KQWqknkBIorzZ3W7dVaMzWJhfS63de9R9KBUCVr0apzeIP3Qw30WpIDPWSKJVh0alYO2BpraeTxqlAq1KgT8kMr5XLOcPSeGhr/I7CK6fY0xWNAW1ThqdPkZlRvOfq4chSbC72sbA1Ih2IuukIUmwd75sn9FUKC/LPQvOe6fLnlTv7X6P2ZtnA3D/8Pu5tPelx35YUaT+n0/T/N57oFSS8fFH6AcM6DCuYm8z81/cjiDAefcPJS69e/eHPT8u5/t/PwuCwFm330fOqGNzXD4evIUtNM/Zh+iSPyfqBCO6vGgsp6Qe1QtHFEWam5uJiYk54efU3ft3WOScBJHT9NZb1M9+FoDEJ58kYta5J2zfAPaFP1B9zz1IgQCG4cNJeeVllKbO50PdATenzz2dFl8LT459khk9zoJ/DYaWEpj2HAy7lmaXn5FPLcUfFJl742iGpP++lXmYMH8Evt9Vw40fbQVkw9ecBAt7a+RclAiDmnum5iBJ4PIF0aoU1Np9bC5tRqkQuGh4KtP6JbU5+Dp9QfbXOSioddAjxsjIzGh2VLRy4Rvr8AdFpvVP4pTcWAQEHN4A1TYvq/Y3dJn78lOSrDp8QZEml7/T9TnxZm6c2BNfMMSq/Y2sLWok2qSlR4wRUZRocfspanDh8gW5bGQ6fz2rD55AiM2lzYzqGX1sXcBPBO5muUS8ZKX8uyEGzvgn9J3VqQ8OwItbX+StXW8BcGWfK7lr6F3H/MAnBYNU33c/9u++AyD+oYeIuqyjUAoGQsx5fCO2eg/9JqUw/sKjpy4coqpgL3Of/CsBn5dR513M6POPXYQdK75yOw1v7IKgiDrRSNRFOajjjz5Fmp+fz44dOygvLycYDHL//fejVp/YqquwyOkGJ0PkBGprKZp6OpLPR9w99xB9bddN3n4JrvXrqbz5FkSXC23v3qS98Tqq2M4z/9/Jf4fntzx/OJqz8U1YeD/E5MDNG0AQuPvzHXyxpZKzBybx4kW/3P0yTJj/VUKixNqiRv70/ma8AZHsOBOF9U5Avr+OzYrhqXP7kRL5y6teqls9CAJdTv1UtXpw+YIYtSpMGhUGrZJam5f9dQ6anH6cviC5iWZG9ohGEKCyxUNQlHD5gry4tJDFe+oYmh7J21cOw2o4+k1KkiT8IfHXFzTtTwJqdsDca6HpAKgNMOoWGH0r6Lq+xi8qXcRdK+8C4I7Bd3BN32uOK6Jd98wzNL/9DqhUJD31d6zTp3c6bvUXhexYUoHBouGSv41Eqz965ojP7WLF+2+1TVGl9unHeX99AoXi5L7XwWYv9a9sR3QG0OVGEX1Zb4SjJEWLosiyZctYvXp12zKtVss111xDfDcrg7tLWOR0g5MVyXFt3Ih74yZib7n5hO2zM7x79lD+p+sJNTWhzc4i47PPUOg7Xuw6RHOSJ8JzfcDvgMu+hKxTya+ycda/VqNWCqy5/xTizL/cBTNMmP9GHN4ALy4pZHlBPZEGDb0SzNw5pRcxJi3vrC7hX8sKaXHLFZTje8XyzpVD2Vllo6jeyfhescRb/jjfrRqbhzizDuXvxL22SyQJfpwNG9+UbTIArKlwyacQn3fUTRvcDZwz/xxsPhvX9r2WO4bccVynYF+0iKrbbgcg+fnnsJxxRqfjynY38e2/dgBw5o396DHg6GXpHqeDuU8+TF2xPOWWN+FUJlxxHXpT9/J3jhUpJCEoBQINbhr/s5tQsxd1kpHYGwag0HYtqkRR5Ouvv2bHDvm1jRo1in79+pGQkIBCceKnJ8Mipxv81o7HYkikpdZNQ4WDxnInjVUOLDF6Rs3sib6bHVv95eWUXnopoYZGIs4/j8THH+903KFoToYlg69nfo1i4V9gw2vQ6wy4ZA4A576yhq3lrfx5ci9un5x9wl5nmDD/DQRCIvO2VjF7UUGHHJXcBDPTByTxzA8FAJi1Kqb0ieeRGXnH33YgTPcIBeHb2+UmmwAqHfQ8Bc56HsxHd/dt9jZz14q72Fy3md5RvfnozI9QK4/97xWoqaH4rOmILhdRV11F/P33dTqupsjG96/txOMI0G9CMuMvzjnqfj1OB188/hD1pUXozRZm3P0gKblHF23HS7DZS/NnBfjL7GjSLAQb3YiuIMooHXE39Ed5FHNCURSZN28eu3btQqFQMH36dAYNOrkzAmGR0w1+K5Hj8wTZvaqKHcsqcNs6zoEbLBp6jUjAVu/GGqtn8NT0o4oe1/r1lF99DUgSSc/OxjqtY7mjK+Bi8ueTcQacvHzqy4zXJsDLw0BQwl37wBTH19uruH3OduLMWlbfd8rxd/QNE+a/jLVFjdw3dycVzXIFU0a0gTtPy0GSJJ78bm870XPrKVncdmo26t9Bc8L/WsSQHLEpXgkbX4fqbXJ7hjOehkGXg/ro0TJP0MOC4gW8uPVFWnwt6JQ65pw1h54RPY/rdKrvuw/b1/PRDxhA+ocfIPwk/yTgD7H8g30UbpKjTNHJRs67byiqo7SlkCSJ+c8+yYFN6zFYIzj/oSd+UYfwLo8jSri31NH6bTGSr32pvzrFRMyVeSiPcv/xer3Mnz+fPXv2oFAoOP/88+ndu/cJP8+fEi4h/x0hihJBXwiNXkX57iaWvLcXj10WN2qdkpgUE7GpZiITjexcXklLjYvti8vbtt+zpoYRM3rQd0IKik7CxsaRI4n+vxtoevU16h5/AtP48SjN7UOZRrWR83qdx7u73+W93e8xfurbkDwEqrbArs9h1M2c0TeRJ8zyBXvh7lpmDEg6uW9MmDB/AMqb3NzwwRYc3iAxJi03jM/k8lHpbZ5SeUlWLnpjPY1OH1eMSufOKSevjPd/kuIVcGCpHJUJBWDfd/J1SzrihtyN9gyHeGvXW7yz6x0cAQcAvSJ78fiYx49b4Hh278Y2/xsA4h96sIPAAdg4v1gWOAL0GZ3IyJk9OxU4YijE/g1riEpKob6kiAOb1qNQqjj3/kdPuMAJtvrwFbXiXFtNoErOGdOkW4g4KxN/pYOQM4B5fMpRp6jKysqYN28era2tCILAeeed96sInGMhHMk5iZEcSZIo2trA6s8LcbX6MEfrcDTJJZ8R8QaGnJ5O9rD4du6WAX+IHUsqcLZ4scYZ2L+xlsYK+QOYkGlh0uW9iUrsmNkuBYMUzzgbf3Ex0ddfT9ydf+4wptZVyxlzzyAoBfnsrM/oXbQaFtwN8f3gRjlR7PnF+3lxaSE9Yox8f/u4sDlgmP9Jam1efixsIMasZfYPBeyutjM4LYKPrhvZaVPIeruX3TV2JmTHdvogEuY4sFXCkr/Brs86Xy8oIaoHDLhYdnM3/bxj+3fF33H/j/cDkGxK5qKci7i096XHNUUFcqFJ9d334N68GctZZ5E8+5kOYxorHXz2981IosQZ/9ePzIFd5+CsnvM+G+bJr1cQFEiSyLhLrmL42V37+nSXkMOPr7gVX5ENX1ErwabD9gOCVonl1DRMY5IRlD//+W1tbWXRokXs2bMHAKvVyrnnnkt6evovPs/uEp6u6gYnU+TUl9lZN6+Iyn0tHdb1m5DM6FlZRw1VHkIUJfb8WMXaeUUEvCEUCoG88ckMOysDval9CNGxbBmVN92MoNXS84eFqBM6zkfft+o+FpQs4KzMs3hqyD3wbA6E/PB/qyGhH3ZvgCnPraTO7uPGiT257/Tc438TwoT5neP0Bdla1kJShJ60KAPVB00xX1lR1M6lN8qo4bvbxv56Bnb/SwS8ULYamorBVgF+FzTuh9LVgCRPQ/U9T75OBb2QNRmyp8iJxd2sLgqIASrsFVz83cW4g27+1O9P3DLoFhTC8U0phmw2Km+9DffGjQAIGg2ZCxagSUluN04UJb58Zgt1JXZ6Do7l9Os79q06RHN1Je/dfQtiKIhCqUQMhUjO7cMFjzx1XFVUkiThL7Pj3tGAr8hGsL691xICaFLMaLMjMI1OQmnqXh6ox+Ph1VdfxW6X7QkGDx7Maaedhk736ybUh6erfiO8zgArPt5H0dYGABQqgcFT0+k7PpnmKhc6k7rbrpYACoVA3wkppPeLYdWc/ZTubGTXikpKdjRw9h2DiIg/XIZqmjQJ/ZAheLZsof7pp0l69tkOYfMr8q5gQckCFpYs5PbBt5PQ63TZMGvbh3DGP7Ho1Dx+dl+u/2ALb6wqZlq/RPom//6aroUJ80uot3t5fVUxn22qaDPC+ym5CWZEScLuCfLcBQN+XwIn4AGEn809+V0T9MHur2DpY2Cv7HxMxjiY8jd5av14DiEGuW/VfSwqW9S2bGj8UG4eePNxCxwpFKLq7ntkgSMI6AcMIPr6P3UQOAB7VldTV2JHrVMy9vyuvXAkSWLpO68hhoL0GDSUM265i8o9u0jrO/CYBY7oCeLeVo9zQw3BuiOEjQDqRCPazAi0WRFoMywodMcuAb7//nvsdjuRkZFceOGFJHTyMP17IixyTjBqvZLGSicI0Gt4PMPPysQaK18cjUfJTv85zFE6pt3Un8p9zaz8ZD+tdW7mPbeVmX8eRGSCPH0lCALx995D6cWXYF/wPar4BOLuvaed0MmLzmNo/FA2123m430fc+eQK2WRs+U9GHsnmOM5LS+Baf0S+W5XDXd9toOvbxkTnrYK81+BNxDitZVFvL6yuC1Sk2DRYfME8ARCaFUKchLMXDu2BzMGJP22uTUVG2Hxw3KvufPfA0uivHzXF/DdXbJr7wXvg8YI390NWjOc9jjEHcyJkCSo2w1qPUQfX77JcRMKQvFy2bMmd5p8Tjs/h41vHIzI+GQXYvGgwDTFQ8owiEiXX4chGnJOh4i0X3Qar+54tZ3A6WntyVPjnkJ5nP4yottNw0v/wvXjjwg6HekffYg+r/NqJ5fNx7p5RQCMmJGJKbLz678kiqz57EPKd21HqVZzylU3oDeZyR7eefPQrvBXOHBuqMGzowEpILtbC2oF+v6x6HtHoc20ovgZr6OjIUkSu3btYufOnQiCwLnnnvu7FzgQnq46KdNV1YWtaA0qopNPTlfWI5u66S0aZt4xiKikw3k6rXPnUvOg3Pk27u67iL6ufefbFRUruHXZrZjVZpactxjD+2dD5SYYfgOc+TQgdzk+/YVVNDr9XDU6g0dnnJyyxTBhTia+YIitZa3EW7QEQhK3fbKNgjo54XRQWgS3n5rN+OxYJKDJ5SPaqD05njCSJE/D+F2yI6Ax9rDzbtAPdfnyjT9pILSUwernYOenh7eP7AGnPAT5X0LBd4eXKw7etMTAwd9V0OdsiO8L+xdChdxFm+QhsojQGCGqJ6SNhKhM+RwkCcrXQ2Q6WLpZbGCrgvJ1ULtLbhFjTYX4PrKz8Oa3YfM74Go4fE6pI6BsTcf9GGNh5E0w8kZZjJ0A6t315Dfm0+hp5In1TyAh8fexf+eUtFPQq/THFcGR/H5qHnsM+7ffIXnlXJakZ57BOv2s9uMkicJNdfi9Icp2NVK6q4nYNDPn3T+001ytgN/Hwn8/x/4N8nsz8YrrGDJtZvfPKyji2lqHa0NtW/IwgCregGlkIoZBcccVrTlEa2srBw4cwOFwUFhYSHV1NQBjx45l8uTJx73fE0E4J6cb/NY+Ob8Ej9PP1y9sp6nSid6sZsbtg4hJOSyqmt97j7qn/iHn5yxahDr+cFKeKImc/dXZlNpL5f4s2mR4/2xQauDWrRAhN+lcXlDP1f/ZBMA7Vw3llNwT61gZJszJwuMP8e7aUt5ZU0LDTzxtYkxaHp3Rh2n9Ek9epKZ4JeyeJ9/g3U2yIHDUHF6v0smCQBBkMRA8mASqUB8WLCAn1Zathdayw8sEBYy7W85b2fOVvCxnmryvfd+2Pw+lRi63ltqXBgMQlwfDrpXPs/RH+Vz7zoLEAXL0qMM/CXwOKFomi7KfwxADMb2gfO0R530XpAyXf47NAWtKl20Wukurt5XC1kLiDfGsqFjBv7f/G0/Q07b+nKxzeGzMY7/oGDWPPErrp7LoVKekEHX1VURd2rGlwtYfytqiN8BR+1L5vR6+evpxKnbvRKFUMeX6W+g7sfvCIWT30/ThHvzlsmhHKWDoH4txRAKadMsv+myLosimTZtYsmQJgcDhz6NSqWTw4MFMnToVleq3nQgKi5xu8EcWOQBeV4D5L26nodyBWqdk8pV9yBwkZ+5LkkTZJZfi2baNyEsvJeGvD7Xb9rOCz3h8/ePEG+JZcM53aD6cJV/oBl8JM15qG/fo/N28u7YUi07FN7eOJT366D1LwoT5LZEkiU2lLdw3dycljS5AThp2+YL4gnLTyWfPH0Cs+finjrtEDMmJsI2F8PoECLg6jhEUsljgJ5ddXYQsfJy18u+5Z8mCIHkw2Kvh4wvA1Qh9ZsKgyyChr7yfnZ/KEZDeM+Q7atk6OWG3fjdEZsCI/5OPuXe+vB+vXY6+VG+Vp40OoVAdnjrqDoICEvrL5xfwQEsp1ObLLuqJA2DMHdB7OijVUPC9PMU27FpIP7YpmK6QJImQFOKrA1/x3Obn2srBD5FhycCitZBsTObR0Y9iUB9/C42WOZ9S++ijIAgkv/AC5tOmdCogKvfJDTclCZJ7RRDwi2QPjWPg5I5Tbj63m7lPPUzN/n1o9Hpm3vswqX26Tko+hOgO4FxbTbDFh7ewBdHuR9CpsJySimFIPErjLzeebGlpYf78+ZSUlACQlJREYmIi0dHRDBgwAKPx93EPCIucbvBbiZxQMIAoiqg1Wlpra9i+6DvctlYik5KJy8gkOTcPnbF7U10+d4AFr+6iurAVgOHTezBsWg/goEngVVcjqNX0XPQD6sTEw9uFfJz55ZnUu+t5cMSDXGTIgHemymWZt2xqm8P3BUNc+Pp6tle0khNv5subRmPUhlO5wvy+KKxz8Ni3e9hVZaP1YEuFBIuOu6fmMGNAEgoBWtwBYkyaEx+98dpg3v9B0XIYdRMULpKFRPIQ2XlXpZOna5IGgsYkiwl7ldxEEuTpnqhM+efWMjmaY+2YxHpC8bTIU0pb3pXFytS/yxGnbR+Czy6LmLZ/wuGfFSpIHgq9poIhqv0+RRE8zXI+zQl+jyVJYmv9VpaULWF9zXqKbcWIkti2PloXjTPgRK/Sc9vg25iVPeu4E4uPxL1lC2VXXQ2BALF33knM9X/qdFxjpZP5L27D4wiQOzKBU67s3eXnLBQMMu+ff6Ns5zZ0RhPnPvA3ErOO7nwM8tRUw5u78JcdbrqqitMTfUUe6phfNtXn9/upra1l//79bNy4Eb/fj1qtZvLkyQwbNuyktGX4pYRFTjf4NUVOKBhg3RdzOLBpHS01VYihEKbIKFytrUhHfFkBEAQiExKxxMZjiYnFEhtPRv9BJGR1np0fComsm1vEjmUVAIw6tyeDT5P9CsquuBL3xo2dtnyYs28OT254kjhDHAvOXYD2k0vhwGLofyGc+0bbuFqbl+n/Xk2Dw8fQ9EjeuGIoUcbulRuGCXMyKG9y88+F+8iKMzEwLYI7P93e1i9KqRA4b3AKD0zrfWJbKgT9sOLvkD8XNGYwx8tNbouWQWNB+7GGaPi/NYeThcN0i6AYJL8xn33N+/CFfLgCLurd9Wyt30qJraTDeKPayM0Db+aS3EtQCAokpBMibkD2wCk573xCjY2YTz+d5Oef61S4lO9uYuGb+QS8IWJSTcy6Z0iX9iCSJLHkzZfZuXQhKq2WCx/5Bwk9u9dCp+XrA7jW1SBolZgnpqC0aNH3jUZxnA+dtbW1bNiwgf379+NytY86pqamMnPmTKKjo49r378GYZHTDU6myAn6/VTu2YWjpQmDxcqGeZ9RU1jQ6dgeA4eQnJtHS00V1YUFtFR3Uk4pCAw96xzGXHg5qi5a1h85Hzzpslz6jE3CvXUrZZfIc8fpH3+EYfDgtvH+kJ9p86ZR66rlvmH3cVlEHrwxERDgpnWHqzSAreUtXPnORhzeIGlRBt65ahhZcScnsTpMmKNxoN7BpW9toM7ePtdmQGoET87sS1ac6cRXAzYVwRfXQM32ztebE+XqxHX/lqeFLv5E9nIJ046gGESlOHxTliSJ7Q3bWV6xnL1Ne9nduLvD1NMh9Co9UzOmMi55HP1j+6NT6jCqjcdt5NcZ/vJyqu+7H9/+/QCILhfaXr3ImPMJCkPHKa+y/CYWvLITUZRI7hXB6Tf0Q9fFlJHf42bRG/+mYO0qEATOvvshsoaO+PlzqnDgWFWJZ1cjANFX9EHf59jFhyiK1NTUcODAAfbu3UttbW279QaDgczMTHJycsjLy/tdRm+OJCxyusHJEDl+r4fv//0cZTu3EfB5263TGo1MuvJ6UvP6o9JosNXVojObiUxoX9Hgam2huaoCe2MDtvo66kuLKdq8HgBTdAw5I8eQN3EKsZ3YfK+bd4CtP5SDAFOv60vWkDiqH3wQ29wv0WRm0uOreSg0h6Mwh3Jz9Co9X0z/grTvH4C930D6WLhyfjuzrQP1Dq5+dxMVzR7MOhWvXTaEMVkxJ+R9CxOmM8qb3Dy3uIDiRhdNTj+iJNHqlsu9s+JMRBrUbCptYUxWNK9fPhTT8TzViiIcuqAH/VC1Wa5mOtTccccncol2wAX6SDj9n2CKlR15GwrkpNzRt8lRm1BQnu756VTOUQiJIV7b+RprqtYgCAJZEVn8efCfidBFHPtr+Z3iDrh5csOTfFf8HQnGBPpE9yEoBimxlVBqL2031qKxMChuEGaNGb1KT6whllRzKhNTJmLSnJwHK9Hlwrl2LbUP/ZWQzda2XBkRQcbnn6FJTe2wTV2Jna+e30rQL5I1NI7JV/Vp515/JK7WFj77219orq5EoVRy6rU30f/UqUc/J2+Q1m+KcW+pa1tmmZqOZdLPl9W3traSn5+PUilfv8vKyigtLcXrPcLlWBDo06cPQ4cOJSEhAb3+d+QD1Q3CIqcbnAyRI0kSb992Hbb6OkyRUcSkZeBsacYcHcMpV/8fEfHH5ytwYNN6Fr3xLzz2g19AQaDvxMmMufByTJGHL6iSJLHi4wL2/FiNQikw7eb+JCcpKTprOqHGxg4tH0JiiOsWXcfmus3kRefxwYhHUb9xinxBn/gXmHh/u/Nocvq4/oMtbClrQaUQuGFCJjdM6IlFF+60HObE4Q+KzN1ayRPf7sHl71gZ1C/ZynvXDCfKqKHe7iXGpD2+dgpb3oVFD8PoW2H0LfDxhVCyUl6nMUPAfbgyKWMcnPP6ceXLNHoaKbGVkBuVi1lz2Aw0KAZ5cPWDLChZ0G58ojGRvwz/C3GGOLRKLSqFipWVK5mzbw4AF+VeRIYlgy11Wyi2FVPtqqZ3VG/uHXYvVq1s3ukP+dlStwVJkkgxp5BsSj5uf5iukCSJKmcVxbZi8qLziNbLEQZv0MvL219m3oF5xOhi8Ia8VDmrOt2HXqVnctpkBscPpnd0b3Ijc0/4eXaFv6yM2sefwLVuHYTkv7OuXz8SHn0ERAl1chKqqI6CtWJPM4ve3o3XFSC1TxTTbu6PsouGrJIk8eU/HqV0+xZMUdGcdcf9JOccvb+Tv9JB04d7CbX6QADDoDhM41LQdNLS56eUlZXx6aef4na7O6zTarVkZGSQk5NDTk7O7yaJ+HgIi5xucLKmq0q2bcZgjSCuR88TmuQY8Pso3bGVvauWU7hRLstUa3UMP/s8hpw1E7VWdj8VRYnFb+/mwJZ6tEYVFz88gtC6FVTdcQcAyS+9iOW009r2W+uqZdb8Wdj9dv7U70/cpoyHedcDAlw2F7JObXce3kCI++bu5OvtsmdClFHDq5cOZkTm73f+Nszvn4pmN+uKmthS1sIPe2rbEoiHZ0Rx3bgexJq1bZ29eydajs3PxmuXE4ItyZAyVK76qdkBb556uGTbkiI77yrUsrA5lCun1ML4e2DcnUdtI+AP+VEr1Oxv2c8LW1+gqLWIB0c8SIIxgRsW30CTtwkBgZyoHM7ueTbxxng+3PMhW+u3ohJU3DX0LmL0Mfxr278od5R3eZyjkWxKZkbPGexr3seGmg24g4dvdBaNhdFJo0k1pyIhUemo5EDrAXwhH0pBiUqhQqVQ0cPag6HxQxmTPIZkUzIBMcC2um2srFzJptpNBMQASkGJL+TD5rPR4pNb16gEFSOTRmLRWMhvzO/wGuIN8Tw2Wi7lLrIVoVPpiNRGMjJx5EmL0ByN5o8+ov6Z2W2+N6rERMyTJxN3150oumhR0FrnJn9VlZz/KEFcupmz/zwIzVG8aLb98C3L3nkNlVrDZf94geiUo0di3Dvqaf68EIIiyigdURf0QpvR0XVeFEUaGxupr68HIBAIUFpaSn5+PqFQiLi4OGJjYwkGgyQnJ5OZmUliYmJbdOePTljkdIM/cgl59f69rHj/rbY8n6ikFM65/9G2SFEoKPLFPzfTWOEko180Z97Un7q/P0XLBx8g6PVkfPwRuiO6xS4qXcRdK+9CJaj4bPpnZK96Qa60UOlkV9Ve7UOrkiSxeE8d/1y4j6IGF7FmLQtuG3dySnPD/Nfzw+5abv5oK0Hx8OUozqzlunE9uHZs5i8z6KveBp9fJZc5A6iNsnCv2w3NRRDbGxr2ARKoDXDpF5A0SJ6O0prlqSeV/Ll2BVwExWBbtATkqMUDqx9gcdli9Co93qAX6YgScb1Kjyfoafv/p2gUGmZPmM2ktEkAOPwOntn0DFvrt+IL+fCH/HiDXpJMSVzW+zIEQWDOvjl4gh6GxA+hT3QfLFoLL255kUpn+3y+OH0cFq2FSkcl3pC3w7F/jl6Rvah2VuMMOLsco1KoSDAkdDh2rD6W+4ffj06lo9nbzKTUSe3et9+Spnf+Q/3TsvGpYdRIEv76MNrMHl2O97kDfP96PlUFh3sR5o1LYuz52V0mGbtaW9i28Fu2fDuPYMDPpKuuZ/AZM7o8hugNYltQgmujnCujy40i6qKcDmZ+kiSxceNGli1bhs/n62xX9O7dm3POOQeN5r+3QCQscrrBryVyRH8IKSCiNKqRQiLewlZEVwBNiolgkxf3ljpEXwhNmhlBoyTY6EFQKVAnGNBlR6KK7nyuVJIkCtb9yMr338LZ0ozebGHmvX8lqZcsXpqqnHz21CbEoMQpV+SSOzyOiutvwLV2LarERHp8/hmqmMM5Nbctu43lFcsZFDeId099DcXca6FggVw2Ov0lGNTR/MobCHH2v9dQUOdgfK9Y3r1qWLgLc5ijIkkSW8tb+GZHDTq1koxoAw9/vRt/SKR/ipVRmdGMzY5hdM+Y7okbv1s2vVMevBkE/bIvzK4voLlYFjJiEEwJ8v/uxsPbmhPhxrWyG++mt2H83ZAxFrvfzrrqdUxImYBOpePrA1/zwtYXaPTI217W+zLuHHIn7qCb25ffzpa6Le1OaWrGVCK0EXxaIBvIDY4bzL9O/ReBUIDFZYv5svBLWnwtnNnjTM7vdT4p5pRf/L7a/XZe3/E6zd5mcqNy2wSQQlAQFIPsatzF+ur12Pw2JEki3hhPdkQ2Zo2ZoBgkJIXwBr3sadrD+pr1bG/Y3lamHaWLYlzyOMamjCVSG0lIDKFVaTGqjWRYMtCpdBS1FrG6ajUCAhat5XclagACVVU4167Ft7+Qlg8+ACDmlluIufmmo0bcQwGR+S9tp7qwFUEhkNo7kr4TUujRv/N8xKbKcjZ/+xV7f1xGKCh7D2UOGc7Mux9C+EkyrxSScG+vx1fUind/C6JTjiqaxqdgPT0D4Seff7/fz/z588nPl80Y1Wo1CQkJbUnCKSkpZGVlkZGR8du2JPkVCIucbnCycnJEux9/lZNAtRNfsQ1fmR1CEsooHZIvhOgK/PyODqEUsJ7RA9PopA4f+EM4m5uY9/Rj1JcUodEbuOixp9uSkg9VXKm1Si54YBhmXYDSCy/CX1qKftAg0t57ty0RudZVy4yvZuAJemTvnOxZ8NVNsOsz+UAj/g9Oe0IO9R/B/joHM/69Gm9AZGh6JLdPzmZcduwxv3dh/jv5cmslVS0e4i06CusdLNlb32bUdyRT8+J5+ZLBqLrIbeiUA0vlPBokMCfJ/iyeFjn590hyz4Kz/w1aK9TugL3fyhGeiX+B1GHthvpCPq74/gr2NO1heMJwrsy7ktuW3UboJ67Bcfo4mrxNhKQQJrWJ5yc9T7JRzntJMsnFBKsqV7G3aS9X5F2BXvXHSuxs9DSyqXYTyaZk+sb0PWGl2b8F7m3bqLj2OsQj8lR+mp/YGY5mb1tjZLVOyTl3DSY2tfMGy5V789k0fy7FWze1LUvMzmHY9Fn0HDaiQ6NNSZJomVuIe/PhxGJVtI7IWb3QZnYUh06nk48//pjq6moUCgVTpkxhxIgRv/sqqJNFWOR0g5MickIiVY+shWDXb6vCpEYVoydQ5URQKzAMiUcVo8df7kAKiXLkJiTiK7G3GT+pU0wY+seiHxCLqpNGnwGvly//8SiVe/MxRcdwyROzMUfFIIoS81/YRtX+VmJSTZx371CCFWWUXnghosNB5BWXk/DAA237+XDPh/xz0z9RKVS8MeUNhsUNgZX/hJX/kAdkjIPz3wVj+6eYr7dXcc8XO/EH5Se/y0em8+iMvJPTByjMH4bvdtZw88dbOyzXq5Wc2S+RoCiyan8Dg9MiefnSwcdW+u21wysjZWO9n2JOlN2700bKzr9RXU9F/JS/rfsbX+z/osPyszLP4sERD7K5bjMPrn4Qu1/+bmZFZPHk2CfpE92n++ce5qQRam3FvXkzvuISRJcLpdVK4yuvIDqdaHv1Qj+gP/rBQ7DOPLtDtEOSJEp2NFJTZKOl1kXF7mZEUUKhFDjr1gGk5nZMQg74faz84B12LDrYU0wQyBo6kqHTzz1qgrF9SRn2JXIlrGl8CtoMC7qsSAS1Ap/Px+bNm6msrKSxsRGtVovdbsdut6PX67noootIT08/oe/bH42wyOkGJ2u6qv6V7fL0U7IJTaoZXXYkCpNa7jEigDYzAkEpIIkSCLR90YLBIAqFok2ZS5KEa0Mtrd8WQ/BQEqSAcWg85gmpqKLaJ8d5nA4++es9tFRXEpmYzDn3PUxkYjKuVh9zntiI1xmg/6QUxl3YC8eKFVT+342gVpP1w0LUSfKTpyiJ3LvqXn4o/QGr1sqHZ3xIhjVDfvKddwP4nXIzvos+ku3bj6DO7uXVFUW8t64USYLT8xJ44aKB4Q7m/6PUO7xMfX4VLe4AozKjUasUxJg0nJobz4Sc2GMv9/a0gNZyOPn32z/Lrr2RPeDyL+W2ByC3OYjN7RBxPBJREim1lRKSQkhINLgbKLWXsr5mPSsqViAgcOugW3lz15t4gh56R/Xm/TPeR6eSv3ONnkZ2NuwkNyq3LWoT5tdHCgQI2WyILhdSMIhj8WKa3nwL0dUxUmgYNozU11/r1O8GoPpAK2vnHqCupH0UMDknguHTM0nKiuiwjb2hnnlPP0ZjeSkA/U45jWEzZhGZ2HUFXqDBjf2HUjz5TQBEzMzCNPKwaaTD4eCjjz7q4GMDEBERwWWXXUZMTNi6IyxyusHJEjmSKLWbWmppaaG8vJy6ujrq6uqor69HkiQSEhIwGAy4XC5aWlpoaWlBq9XSr18/Bg0aRGKi3EAwZPfh2dWIe2fjYUtvAbTZkZhGJqLLjWo7nq2+lk8f/QuOpgZ0RhMz7n6Q1D79KN3VyHcv7wTgzBv70WNA7GE35IsvIvGRR9rO1xv0cs0P17CrcRdRuiheOuUlBsQOgPp9MOdiOc9BpYcZ/4L+53d4/d/urObOT3e05Vi8dtkQkiL+WKH6MMeHyxfk0fm72Vtrx+ULUdLoIi/JwrybxqDpwkPkZ7FXw/InYfvHEJEGo26Rp5q2fySvv/Jb6DGu002bPE0sLV/Kj1U/kt+YT4Ylg0xrJj9W/UiNq6bTbQBuHXQr1/e/nl0Nu/i+9Huu7HMl8cZwg9rfAkkU8ZeWEmq1gRhCnZyMv6KCxldexb1+fafbaDIy0PXti9JiJlBXjzopibg7bkfRScl0a52bdfOKKN4ud01XaZXkjkwgMsFIYk8rsWmdT0/Vlxbz5VOP4GptwWCN4Iyb/kzGwCFdvo6Qw499aTmujTUgAgJYJqdjOVWutgoGg+zZs4elS5dis9kwGAyMGTOGuLg4AoEAfr+fXr16YehCpP2vERY53eBkiZwff/wRn88ne0hUVVFaWnpc+4mLi2PAgAH07dsXq1Weo/UVt2JfXoHvYK8qAFWcAevUDPR5cgm3q7WFr2c/QU1hARq9gcueep7IxGRWf1HIjiUVaI0qLnxwOIrCnZRfeaXc22rxItQJhz18Gj2N3LTkJvY270Wr1HLroFu5MOdCdAEvzL1Obv8AcpfkKY+B6XCXc4B1RU3c+NEWWg/2C3r5knCJ+X8rgZCIPyiiEASufncj64ub29ZplAq+uXUsOQmd3yg6xeeQHYYbC2Hv17D/h/bNJI9k9K1ynthBdjfu5tUdr+INegmIAXY07OiQS3MIvUqPXqVHlERiDbEkGZMYGDeQUYmjyIvJ6/75hjkhBBsacK5Zg0KnRxUXi75vXwL19VT9+U68u3Z1vaEgyNEZlQp1XBzRN9yA5cwzOiT5/hRRlNixtIINXxcTCooIAvQZm8Sws3pg7CQl4EhKd27jm+f+jt/jISYtg3PvfxRzdNfRFV+pjcb/7EbyHfTiyY3CekYGUqSajRs3Ul5eTkVFBR6PXH0XHR3NpZdeSlQnHj1/JEIhL07nPqzWgSd832GR0w1OlsiZPXs2Tmf7ksvU1FQSEhKIj48nPl5+IqytrcXn82EymbBYLMTExFBfX8/27dvZu3cvodDhi3N6ejr9+vUjNzcXk8lEsMmDc2MtrvU1bV8c86lpWE5NQ1AIBP1+vnjyIar27SEmLYNLHp+NQqVh7tNbaCh3EJVkZPqtA2i69U+4N2/GMm0aSbOfaTdH7Q64uXfVvayslM3R4gxxPDLqEcYnjZGfrH98Vh6otcBpj8s5EEdsX9Hs5voPtrC3xo5KIfDXs/pwyYi0Nq+TMH9MJEmixR2gotnNd7tqmLOxHLs3iEGjxO0PYdKqeHRGHsGQSE6CmUFpkT/dgfxPoQBHrSxigj7QmuSf93132LvmIKG0kVSM+BMxzeWYdn+JJ7IHO3InY0oeQpolDX/Iz6rKVTy5/kn8YntB1De6L6ekncLg+MGU2Eo40HqAQXGDmJg6Ea3y92N5IEnSf31FjCRJOJYswbFoMYJCQGGxYhgyGMnno/bvTyEe4TZ8KOoiulwIWi2qOPlBKlBTgyAIWM+bRfTVV6NOTkbopvfLoZyb4u0N1BTZsDfIoiK1dyRjzs8mOqlrv56W2moaykpora1hzacfIIZCpOb15+y7H0Rr6NpUL1Dnov7VnUjeIOpkExHTeqDNjMDr9fLxxx9TXn7YT8hsNjN06FCGDx/+h3MgPoQo+rHbd1Jb9w11dfORpBBjx6xDpTqxxoNhkdMNTpbIWbZsGX6/fKE1m83tIjHdxePxkJ+fz65du9p9CUCO8GRlZdG7d2+SYhJwLCnHuUY25tP3jSbyghwUGiXOlmY+vP92XK0t9Bw6krPuuA9Xa5AvZ2/BbfNjitQyZbIG261XgSgSc9NNxN52a7tjhcQQXxd9zas7XqXWVYuAwE0Db+L6/tejqNoK3911uJ9P1mQ44+m2DuYAbn+Qe7/Yybc75akBs1bF2OwYbp6URd/k3095aZifp8Xl58ttVby/rpSypo5uqgAGjZL3rxnO0IwunkD3fA3f3w+uBjDFH0wa7uQSZIxFikxnXXw2Hys9bGndjzPgRCkoyY7MptRW2qXvy4SUCZzR4wwCYoDBcYNJs/y8Df5viehyUXnrbQSqqkh67ln0eYejSJIo4t2zF9eaNQQqKxBdbrTZWURdfXWXhnWH8BUX41y2DHVqGubTphBqbaXpzbdQRUVimTEDdVzcUbfvimBzM+5Nm1FazKhT01AnJ7UTZ77CQlo+/xxBoUQVE41+0CC0vXrhXLGC5vc/OGpURpOZiTIyUp6eapJzVvQDB5L83LNteYNSMIgkiu3a03R5roEQxdsacDR7iYg3ULixjqJtDW3r1VolY87Los/YpA4CUxRDCIICQRAoWPcj3730DJJ4uJly7pgJTL3xji57CYbsPtzbG3D8WIXo8KNJMxNzXT8UGiUul4sPP/yQmpoatFotEydOJDk5meTk5D+sWZ/NvoOysjdoalqBKB7+bmq1iQzo/zpm84mNjoZFTjf4o5gBHupDkp+f3yEZLSYmhlNOOYU0VyStXxVBSEKdaCT6yjxUEVoq9+bzxRMPEQoGSe8/iLPvehCPS+Lbf+2gpdaNJUbHab2raH78YQDiH3yQqMsv63AOvpCP2ZtmM6dAtpUfEj+Eh0c+TKYlHda/Cksfg5APBCUMvhwm3AeWgxclSeKtH0t4ZcWBtk7RggDnDU7hjim9SA7n6/zucHgDvL+ujG3lLfiCIpUtng5l37FmLX2TLFw+Kp0haVGUNcumkInWTv6e7mZYcLfcwfunJA+VWyW4myE2l52Zo1nhqWRl5Ur2t+xvG6ZRaNpFaeIN8YSkEI2eRgQEonRRXJR7kSzAf8Ny50BdPfX//CfeffuIu+duTOPGYZv/Dd59e9FmZqLNykKVkIAqLg4BqLjxJlxr1gAgGAzE/Ok6/KWleAv24y8rQ/J0YiCYno75tCl49+xFlRBP7E03IYVCNL39Dr6iA4Qam/AfMU1uGD4cX3ExocaDydlKJYZBg9APG4pp9Gj0gwYhulxyVdKBIgKVlWizemKaNAnf/v04V/1IsLmJYEMD3l35cr+vg6hTUzFPnoy2Vy+C9fU0vvwykr+L6cWDrzHyootQRUcRqK3DtXYtwfp6oi6/nJgb/w9BrZbF3e7dhFpaMI4ahdCFkOgKnyfI9sXl7FpZic8VbLdOoRDoNzGFlN6RJGRaO22oWVtUyDfP/4OAz0uPAYPZu2YlkigSk5aBwWIlY8Bghp51TpdTYu4dDTR/XtBWZauK0xN7wwCURjV2u53333+fxsZGDAYDl19+OYmJf9xu9aGQm9177qah4Ye2ZWp1FFFRY0lMnEVU5CgE4cQLt7DI6QZ/FJFzJC6Xi5KSEgoKCigoKGiLGKWnp3Pm0FMJfVWN6AqgMKmJvrwP2nQLZTu38/XsJwj4vKT26ce5DzxG0AefPbUJR5OX7GHxDHAsofm11wCIvuEGYu+4vdPQ+ZeFX/KPjf/AE/SgUqiYlT2La/peQ5LHCYselK3zQbbCH/4nmHAv6OSITUiUyK+y8c6akraWEGqlwIXDUrl6TA96xoa7mv8aHPrKH/n3DYkSLy7Zz/KCBqx6NfnVtra2CkeSm2Dm8lHpzByYjLGz6qjmYln01uaDu0l2C04aDLs+B1e9LILH/hkGX0HQXoPSmoIQIRvhBUIBntvyHB/u/bBtd3qVnlnZs5jeczq9InvR4G5gR+MO0sxp9I7qjSAIuANutErtr9bv6EikQAD3lq241q3DV1gIoRDuzZvbVfeoYmMJNjR0ur3CaJSnY/R6dLm5eLZt63SMYeRIdHl9EFRqWj78kOBBK/9DCBqNHGUIHnFDVyoxDBuGZ9s2pIPOuJqsnigtVjxb25f1K0wm2UPmCPFyNLTZ2UihEIGKCqRAx8+JcexYtDm9CFRV416/nlBrK+q0NKzTpxN5ycWootvn53U2VRfwhWiscBARb0BvPnrURpIknC0+6krs1JXY2LeuFu9BPzJTpJbEnlZa6tzojGpGz8rq0usm4PWy58dlrHjvLYKB9kItb8JkTvu/Wzv43RzCV2oj1OIj0OjBsaxcNtBOMWEcGo9hYBwKnYqGhgY++ugjWltbsVgsXH755cTG/vE8xWpr52N37MRiGUBFxX+w23cgCCoS4s8mNfUqTKbeJ33qNSxyusEfUeQcidfrZe3ataxbt45AIIBGo+G08ZNJ2aQkWOcGpUDE2T0xDkugprCAuX//K36Ph16jxnHWbfdQV+rgy9lbkUSJSZfnErvjKxpf+hcA5imTSXjsMVSRkR2OW+Ws4h8b/sGKyhWA3LNmRtYMru17LWktlXJUp3ydPNiSAjNfhsyJ7faxtbyF2T8UsLaoqW1ZXpIFX1BEq1Jw3bgenD0gOeyefIIRRYk7P9vOoj11zBiQxPlDU0mK0PHEt3v5blf7aqPMWCOXj0wnwqAmyqhlQIqVCEMXN5v6vXKOVv7cwz2fDuIWBBYbDXwTGUujNQG11kKrr5V6dz1apZZ0SzomtYkGTwNl9jIATks/jXEp45iQMoFIXcfP4K9Fy+ef0/LJJ+iye6EfOgTrmWeiMBqRgkFs33xL4yuvEKio6LCdbkB/9Hl9afnkE5AklJGRmE+fSqCyCn9pKcG6usPRDpWK1FdexjhyJPXPPouvuAR9v37o+vZF0yMDTWoqguqwoAzZ7TS99TbBpkZ0ffrg+GER7o0bATCOG4d15tmoIiPR5uSgio7GX1pKw0svocnIIPqGG1BotfjLy3Ft2IB7w0acP/7YlgujycxE368vqvgE3Js349m6Ve7pNGUy2syeKMwmDAMHok6WS6RFtxvnj6txrf6RQFU1osuFdda5RJx/fttNTgqFCDY2ypGrozkLB0XcdnkavbnGxYJXdmJvlKc9LDE6zFE6zDF6UnpFoNIoyV9VRUO5A41ORTAQwuNoL7YiEwyMmJFJj4GxR72O7Fq+iJKtm/E6HdQU7Sd4UBBmDh5Gv1Omsn/DGiwxsYy+4NJOBY4UFGn9thjX+vbfH+OoRCKm92yrfN23bx9ffvklfr+fyMhIrrjiCiI7ub7+npEkkaLiZykre63dcpUqgoED3sJqHfSrnUtY5HSDP7rIOURzczPz5s2j4uDFNie7F2P8uSgK5KdJbXYEkedmU1W5jy+fehQxFCRz8DDGXXwlpfmwYX4xCqXA9NsGYspfRs2jf4NAAFVsLEmzZ2McMbzT426q3cTrO15nQ+0GAJSCkst6X8bNA29CX7pGnp441C8oe6r8BJ8+qt0+1hc38daPxSzdV89PP4nxFi0qhQJRkto8VeodPnRqBTMHJjMpN45ASMSgUdE/xdouoVkU5e5BPzUj/GkUo8npwx8SSbDo2l2A6+1etGolVv1/V3f1V1cU8c+F+zpdp1YKPHBmb6x6NSatilNy437efbh6O/w4G/Z+c3hZ1hQYcBEFko9PyxbyffMunHRe4fRTzGozT459sq2P08lC8vtxb90KkoTk9+NYsgTPrnyi/3Qd1mnTkCSJhpdeounV9hdzZWQkplNPwbVyVVt0Rmm1Yhw/Hv2ggSi0WpRRUZjGj0dQKnFv3YZ37x6sZ5+N0nQ4UilJEqHWVoJ1dShMJjQpx9bWweP0EwqIaPQqVBoFng0bUBiN6Pv3P/b3IhjEu68AVUx0uwpLANHrRdBqj+mpPOgPUVNswxqjxxLT9VS0vdFD8fYGnK0+WmvdVBW2EvSF0JvVBP0iAV8ItVZJwNe9z45CIRCdYiI+w0JSrwh6DopF8TOf3+2LFrD07VfaLbPGJ9D/1NMZOv2cLqM2h/BXO2n9uki29hBAk2FFUIC+bwzGkbIFSG1tLcuXL6egQO4zmJ6ezvnnn4/J9PuNXEuSRFPTckrLXsPh2IVGE49abcHvb8bnk8VcbOxUPJ4yQEHfvBcwGnt2ui9XKITxJOQZhUVON/hvETkgd6Rds2YNy5cvRxRFdDod49KHkrZbhxCUUJjUxFzdl+LSLSz417NIkgiCwMhzL8LROoCirfVo9CrOuWswRlsZ1ffci7+4GJRK4u65m6grr+zyQre9fjuv73yd1VWrAUgzp3FR7kVMSRxDwpp/y4Zth5JLU0fAmNvlG6HqcFSgotnN7mobFr2abeWtvLayCIc32MnROsegUdI32Uq8RUer28+28lZCosTQjEj6p1hJsOrZV2Pnu101SBJMzIml2eVn9YFGJAlMWhVpUQZizVrKmlyUNrkRBMiOMzEuO5Zp/ROJM2upd/gIhiSUCugVb8asO7oIqmh2E2/RHb9HzBHY3AHWlzQxNisGo1bFlrJmlu6tJy/JyvheMe3OJSRKLNhVww+7aylucGH3BshNMLNsXz2iBDdO7El5s5sNxc00u3xEGbW8cOFAxmZ3UgZbuQVsFXL3blslrHtZjtyIAWgpxSEIVKpVuHqMQ9H/IrQJfZmzbw5fHfiqbRcpphTOzT6X/rH9CYgBTGoTSaYkXAEXZfYyvCEvSkHJoLhBxOiP3+hMCoVwLFuGd+cu/BUV6PL6YDn9dDSpqW1jAjU1VN5+B96dOzvdh+XMM/CVlOLbuxeAqCuvRGE0YPv2OwJHFAEoIyOJuuZqoi69tIPBnCRJeJ0BdEY1AX+IsvwmHE1erLF6YlJNWGMNBAMhti8ux97opc/YJOJ7WBAEAUmSOLClntpiG4JCIDrJSM7IRPyeIKvm7KdiT3PbVAzIEYuhZ2aQNTS+LWIhSRIN5Q6Ktjag1inpOSiWyITuV7dIkoSr1Yej2UdUogGtoXtiv2JvMys+LmirWrLE6olNNWON1eNzB/C65PfE7wlyYGuDbIh6JAJtl4qk7AjOuKEfCHIfPpfNR1Oli4q9zXidAbKHxZM1JI5QSERAIDrZ2GWzTIBQMEB1wV7Kd+/E7/FgsFhZ89mHSKLIgClnkpzbh6ikFOJ69DyqqAu2+vAVtuDd34InvxEkELRKoi7KQd87Wm7tI4q4XC6WL1/OtoNTkIIgMGLECKZMmfK7SS6WpBBOZwFO1358vjqUCh0+fz11dd/h9XaMUAIIgpreuU+SmDirw7oyj4/dTg/xGjWFbi9f1LZwwO1j86g+qE5wVD4scrrByRI5FZUfIAhKEhPOQaHQ0WrbjMdThkYdjUYTjVodjVptRak0IJzgBMmamhq++uor6urkfijJ8UmMdmdjbVAhaJVEX9EHp8bGui8+Yf96WZSccs1NFO+Ip7bYhkqjYNwFvcgZHEHd3x7D9vXXAOgHDybmxhsxjhrZLnR+JCsrVvLYuseo98j5AgICM3rO4NaMGcRv+0g2czvkd6K1Qq/TIHca9DwVdO3ff5snwL4aO1q1EgHZZE6UIM6ipbTRxaebKjjQ4ESvVlJn97YlNB8PSoVA6CcXW4UAP73+/hS9WslZ/RMJSRLbylvxB0V0agWjekYzc2Ay/1lbync7a0iO0HPH5GwyY43YvUHykizEmQ9XxqwvbmLOxnIsejVJEXpqbV7q7F6y480MSY8kzqylsN7JY9/sodHpI86sZWxWDPO2V7VFv9RKgRE9ohmWEUWzy8eqwsZO+0MBnDsomWcvGNB2IT/02pUKQTbeK1oOrWXsF92UV6xlTNlWdJLEfrUaj0Kgr8+PBKw26PnGZGSF0Uigswop5GmnC3MuZGjC0JOeDBxyuqi6605cK1d1WKfr2xfTxIkEmxpxLPyBUEsLCpMJdWICkj+AYcQIFHodze+937aNoNEQdd9D+AafSlKvCBSSiG3+N3h27cQ4ejSG0eNQGXX4vUF2LK2gvtTOgFNTMVi1LH5nN40VTpRqBUjyVMyRJGRa8LmDtNQerlKLSzfTb1IKlXtbKNjQvsAgvocFjzPQJh5AjlyIR3xINTol5mg9ggI8dj8uW/ucEq1BhcGiIegXcTv8CAKodSo0WiVqnRKNToVKo8Rl82GrdxP0y+esUivIGhKHQilga/TgcwcJ+EIEvCFCQZGk7AjS8qIp2lpP5b6WtmP5vaGOIuYnJOdEEJtqxhSlIyk7gsgEA/WlDpwtXnoOjkP5Cx8OJEmioayEPT8uZ/fKpXgd9g5jeo+bxBk33/mz0SrRHcC+tBznupp2Fwf9gFisUzNQRmrZuXMnixYtwvUTx+W8vDwmTpz4u8m/cbtLqKn9ipqaL/D5OjorAyiVRlKSLyUh4RyCQTvBoAO12open45G09HzbF5dC3fsK8fXyd/8u8HZDLGGS8h/dU6GyAmFPKxeM5ZgsBWVKgKNJgq3u7jL8TpdCnFxp6PTpeBy7UerTSA15QpUKjMuVzEqlQmt9thKPUOhEBs3bmT58uX4/X4EQaCfIZOBTSlolGqiLsrF0C+GdV98wtrPP0JQKDjj5vvZv1nfdpFKyY1k9KwslCvnU//00235A4JajSYri6hLL8F67rkdqgscfgdfH/iaxWWL2VovJzfqVXquzLuSq9OnYdjyLmz7SE5CPRJ9JFhTIH0sZIyRnW0j0kEf8bOvVxQl9tU6KKx30ODwoVEpGJIeiVIhsKG4mQP1TmpsHiINGmYMTEKnVrKioB6dSsnZA5NJsOoobXJR1eqhwe4j2qRhWI8o/EGRTcUNLMyvY/G+BoIhiVizFq1KgcsfpM7uO6a/yyEEAQanRdIr3oTNE2DBrs4vMp2hVgoEQoe/sqfkxlHa5KK4oaOgiTCouWxEOgNTIzBoleyqtOHyh7hxQk/0aoUclXE1gCUZ6vJh1WwoXwvAcoOeu2Nj8CsEjKJIBEqqFPJxIwQVglJHS/CwF1SULgqLxoIoiTgDTjIsGfx5yJ8ZGDfwuN6jQ0iShGfbdhBDaHr2xLliJfYFCzCOGkXUlVfgWLqUhudfAEFA8vkIVFUh6HRYZ8xAnZyMa/063Bs2dkio1fbpTcpLL3WYJrItW07tF98TPXoAilGn8v37pbTWuUnsaeW06/IwRepwtvhY9sFeKvY0Y4rUEgyIeJ2HRfZPxQeANVZPXLoZW4OHhgpn283fYNGQnBNJ8baGdkJIEKDPuGSUKoF9a2vwew96YUXrOPWK3sT1sKBSK/C5g+SvqmL74nJ87vaRT6VaQY8BMfg9ISr3Nnc4p59DoRDQmtR47F1XSv0UQSHQd3wyI8/OBKCm2EZzlQtHkwetSY3OoMbrDhDyi2QNjSMu/fB1d9eyRexavoik7Fx6DBpKcm4eKrWahvJSGspKMEfHYIyIQpJEAh4PjqZG6suKKdu1HTEYZOSsi8kaOgK3rZWyndso3bmNsp3bcLW2tB3DYI0gre8ADNYIGivKMEVEMuX6W1EdUY4uiRL+cjvefS2EnH4EpUCwwYOv3NHWXkeTakbbMwJd32jqxBbKyso4cOAAZWVl7d6P5ORkpk6dSlraybcxkCQRm20rLa0bCAVdICiIjp5AhHUIbncJrbbNOBx7aG3dgMtV2LadUmnCbO6DTpeMKPpQCGpiYk4lJmYSSuXPuys7gyFml9byWoU8fZup1+ITRUwqJTPjIpgVH0ma/sT7UYVFTjc4OSLHy9byL/BUv0PAJ3/glUoDFstAgkEbfn8Tfn8zktT1hUOjiUGjicPp3INSaWLgwHeIsHZtF94VdrudhQsXsmfPHgCMSj2jPdmkS7FYJqdjGpfED2++xJ5VyxAUCk695kZEKY/184sQg3JfrZ6D4ug3xITyh4+xfTG3XRdfXV4exjFj5HLWqVNRmtor9Z0NO5m9eTbb6uVwrUFlQK1Uo1FouCRxHJe5A+gKvpcrcjpFkPtjxeeBsw7sNeCoBrUBhlwNPSdB7U5Q6SDvXFDr5P5G9hrQGOUeRwGvvNycKP8eCsDOT2HNS3L0aPqLENUTCr6D8g1QvwcUKojOguZivOVrUCs0KBIHQK/TEYZeDRojkiSxuayFNRs3Eqt00zvRhCo+l3qfljmbKli6r47+yVYenp7HptJmPlxfhiCAVeknvyEov7ZDr1KAC4ak0kNZj6FuC7aEkeijU9ldbWdnZSs2TwBJgktHpnP9+EzmbCxnRUED14zN4JRc2ViyuMHJ0r317K21E2/R0SPGyLR+iRhVwPpXoGytXNqf0I/qFU+wt3QZY2yN6CQ5d6lRqaBCpaZCreJAVAofKL2EkDAJKpySfPPUKbVolVpsBxtTRuuimZY5jRk9Z5ATlXPUz6Lo8eBauxbJ70eTkYE2K6tdWbCvpITWz79A8npQxcaiHzwE/cAB1D78MLav53e6T03PnviLitotU8bGkPrKK4hpvdj2QznRKSbSM5Q4li6ndnMhjYZMmoQ4gmojoggpvaPIHhqHRqeiqcrJloVltNa50RpVINFOOGj0KqKTjDTXuDoICmusnqTsCArW1yKKEim5kZx6ZW9CQQlJlLDG6dsiBS6bj4L1tfg8QQZNSUNnVONx+Nm9upr8lVVIksSUa/JIyZGTUp0tXtZ+WQSSxPiLctCZOk4dBQMh7A1e7E1ypEdnUhOVYESjl6Oufm8QZ7MPt8OPSq3AYNEcXB7C7w0SOPS/L4TBoiEizoA5RodCIVBbZJOnvfRKIuIM6Exq1FolGp2SUFCiaEs9VYWtJGZZ6T8pBUv0z1tCSKLInh+XU7ZrO8k5fXC1NrPui0/ajVFrdZiiomipqf7Z/bX9HeITsNW1f2hQabWk9xtEv1NOo8egIZ0nD4uSPP20qxHvviZEV+dT5ap4AxHTMvEnKNm+fTvbtm2jpeWwiFIqlUycOJEhQ4agVCrRak+O2aQo+nE699HQsEgWNSE3Pl8DgUBTh7FKpYFQqL2vlSCoiIocTWLiLGJjp6BQHPt5BkWJj2uaeLqklsaA/H7dnBbHA5mJKH8FU8uwyOkGJ2u66rTNBZS4fQwzeolXeqghAZ+kIF2nxapS4gqFqPL62OfyEhT9pAh19FTWMcIUwmT/AY+vigha0CILIaXSQGaPPyMoVKiURrS6JMymPNTq7p3zgQMHWLBgAc3Nst3+gGAGQ4KZqK06LNPSWbXqQ/b8uByA/pNPZ+Dpl7D1h2oObD4cbUnsaaX/KSmkxvpwLlna1tX3EKrERBIe/iumiRPbhX0lSWJJ+RKe3/I8FY72c7xRuiiyI7LJMCYwITKPkaIKRcmPSDXbUdlrOkZ7joY1FRL6QeHiDm65ACjUoDGA34UoBtmg03JAo6FFpUal1BDndeAVFFSqVPgFUEmwR6thl1ZDZEhklsNJpChSaDBhtfagrzGJnjV7SazdQ7NSQbFaTZFWR1V0BgMMiZxKJPr+5yJkT5FbFCx7HCo2gr0KUWul0dQLp6QnIAn4rEo208gZFbtJDIVkETf2zzDsOrkEG0AMycZ59moQg3IUZscn8j6tKRDTC2KyQW2E4uXQVERTfG8OeGpRNhdjFkUy/QHW63XcFxuDQ6nAEhIZEJTYrYLmTnIEZvScwaOjHyW/MR+H38HQ+KFolBq21W9DlESGxA9Bpeh86lL0eKi4/gb8ZWWo4uLwFRcjHSGQ1SkpJD7xOAqjkaY338KxeDE/zTwXDAZ5G6USVXQ0wfp6VImJiOOm4/1hPhqbfDOLuvJKjOPHEWpqwjh6NJI5ki9nb6GxQv58CgrhZ6dNuiIm1cS4C3vx46f7aaxwIoZsiMEy4nsO59Qr+hHwyeIgtU8USqWCpupWaovq6D06G4VSgSRJBH0+FColCqUKQRAQQyGcLU1UF+zlwOYNOBobMFgjiEpKptfIscSk9UCpOvz3cDY3UbFnFz6XC4PVSkxaD6KSum4AeSTOZvmmZ4yMaju2x2HH63RgjIhC10nya0N5KWs/+4iU3nkMOmP6UZNvJUmics8uDmxajzU+gcTsHFwtLdgbG0jomU1kUjJbF8yneMtGIhOTSOiZjc/joWTbZuqKCzvsb8CUMwn6/ZTu2NIWgVGqVMT37IW7tQW3vRWFQolKq8UcHUNEfCKpef1pqa1m8zdftpn1xWZkktF/EBkDBpOU06dTw75gixd/hYNgkwf3tnqC9YenAgWdCl1uJOp4A1JQwqsNcsBXRYOrua0X4aFbp0ajISsri5SUFHJzc09qK4amplUcOPAPXO4DSJ20K1GpzERHTUCjjSMQaKahYTGhkAuFQoPFMgiLpT8Wc1+iosZ3+/7hDYmsa3WS7/RQ7w/gCUkYVQqWNdkpdB+sRNNreSQriakxsl2I0xckGBK7rsY8AYRFTjc4GSLHExLp++oq/N6g3IRNLSBG65B0SgS7fPMVozVIFo2c+NEFRkWIqxItjHU8i2hb3GG9UmkgMfF8EhPPxWTMQaE4emJgIBBgyZIlbNggV0JFCSb6+lPpGUrAPDyJ/YEtrPlS9iexxMYz9qLLiU4dyK4V1ezfWId4cIokvoeFSZflYtV6sX37LYHyCpwrVxKoqgJAnZSEcfw4rGedhX7IkDbBExADFLcWo1ao2d20m5e2vUStq/0Tl4CAdDC3Q6vUEquLYrIhnQlKK9GWFGIie2KO7Al1u/Gt/zchWwWG+H7QsB/JUY1HELApFIg6M5F+H/pQEEltoCXkpUIpUaFWUaJWs9BkpuIEJAIfjdRAgFPcHuLjBrC5dT9bNAryfH7Odzgp1KhZrddjkESUEqzV65AEgbhgkDfdajKbymhUKCjVaNgTm8ESPBQoQox3e5jqcrPQaGCHTstwj5dJbg8lajkCkxwMEhUKUaJWs12rJV+rQTpCcOpFCZ8AoiCgU6jxHiEGFYKCRGMiKeYUUkwpDIgdwNlZZ3crj0YKBgk2NiIFQ6hiY1BotdQ99VS7/BYAdXIyqthYfAcOtBPIABIC+omnouuVRaiqEteK5YguFwqTieQXXsA0dgwhm40d61pY95Uc+TMrXcQl64kZlEVztUtuV5JoxO8NUrmvBZ1Jjc6oprVOFlcGq4bkXpGk5UVhjtQR8Ico3FxH5d4WBEGO1OSMTCBvXDItNS6aa1xkD4tHo1MRCokUby3mh1cfweeyyTYMt9/blijscdjZt3oFG776HLetFUtsPDGpadQc2I/HfrhVgVKlQgyJcuJ/F8SkpjNw6jRUGi3bFn5DXfGBDmOSevXGFBVNdeE+rLFxnHL1/6HSaNg0fy5epwNzdCy1RfupKZQrerQGI4JCgdflbCcmo5JTMVjkG1NEQhKmqGg2z5/b5hGTmJ1D5qBh+L0e6ooP0FBWgt5sISIhEUGhwF5fR8PBDtydIggdxOshNHo9fcafSuXefJqrKphw2TUMPvNs+fMgitSVFOOoryO134BOxdhPaa6upKmynKRevTFGdF6aLYkS3oJmXOtr8O5vaWe2LWiVGIfEo8uLRpthQVAqqKmpYdWqVezbt4+f3irT0tIYNGgQeXl5aLrhvvxz+P3N+P0NhEIetNo4tNp4XK4iHM49aNTRuD2lFBY+3iZulEoT0VHjiIk5BY02DqVSj8Xct11UJhTy4HIXYTRkoVR2dMi2BYJssbuxBUMEJIlotYpYjYo4jZoKr593KhtY2GjD08VDQpRayZ0ZCVyZFIP64P2s2eVnxr9XU2f3cvnIDG49JYtI44kXO2GR0w1OViRn+JNLqHccPV9DpRRIjjJgNaqx+0O4kbCrwKdXIlnUeC1qUClQCTBU28AIRT59NU0kSRV4vSV4vVVt+1IoNFitQ4mLnUpc3JloNF0/SezatYtvvvmmzUQwWjRzaqAfkdYIAv0U/PD9q9gb5KRlY0QkA6acSdaIUyja4mTnikoC3hCCQsAcrcMcqSUxK4LkTAOq7z6g9aMP2zmdqtPTME2YgGncOIxjxrTL3/GFfOxq2EW1q5qdDTtZUraEJm/HUOtPyY7MxqKxsLNhJ6IkMjJxJAn6WNaWLaUm6PjZ7Q9hVpsZlTSKaK+TgCRSr1ajVelIMaWgV+vxh/wkmZIYlTiKPU17+KboGxSCQHZIoNlRSb67hgrJh1P0o1aoybBk0FMXQ4y7le+cxbSIx5avE6nU0xLyYNFY0EtQF+iYIHk8pKvMKPSRNPpacPjl92dW9izuH34/m2o3Ue4op090H/pE9+lWHycpGMSxdBmS14N5yhS8u3dTdc+9BA86cSutViIuOJ+mt94GSSLh8cdQRUWhio1F168fgiAQcrqof3Y2LZ/MoS5xBKW55+OWDk9xCAoBtUaBkiBRiUbSBiUSm2KmudbF6s8OPv0fUYVzJGKwjqB3E2p9X2bddy4JPa04mryodeBorMFta0USRVLy+qHWaAkFA9TsLyAhq1dbXkbQ72fFB2+zZ9UycseMZ9iMWYjBEN88/xRNlYerq0accyGu1mYObN7QaULr0VAoVUQmJtFzyHDievTEbbdRuXsXRVs3EvqpuZ4gEN8jC3N0DK7WZmqLCtu1F5D3p0SSpA7LEQT54eFIUSUIaA0GfK7OE9MBknL60Fheit/TefuOI1GpNfQaNRZXawv1pcWYoqIxRUZRtW8Pfo+b6JQ0hkybibO5icbyUvRmC9boePqccirGiEgCjW68pTa0CSYUBjWePU14C5rxlzuQAiFMI5MwDIrDvqwcf5UTy6lpGIcltPnPwMGSfLufUKsPyRsk5PATaPAgOg5ejw5+VnwlNkKth7+b6lQz6mgdQqKeKqsdt9+DxWLBbrdTUFBA0RHToSkpKWRnZxMREUFycjIxMcdfBXgkoZCXouLZVFS8y5EfakFQdhqtSUg4h56Zd6HVJnSZLN0aCLK+1UWyTk0vow6tQo4qrm5xsrLFgUYhUOUNML++pUsBcySJWjWjIkwkadUYlAqcQZFItZIrkqKxqg9HcyVJ4rr3NrN03+EovFmn4t2rhzMk/cR6AoVFTjc4WSLnq21V+EOyqV1Fs5uV+xuweQL0SbTgD4msLmzE/jPl0UqFgC5WT2u0hlCiHlQKECVidWpOi7YwQFWF2fY1BucKVKHDbqpKpYn09OtJS70GpbLzuXGPx8OWLVtYs2YNHo8HDSpG+XuRJSagybBQYSxk85pvcLXI01sKpYqc0ePIGT2FgvUiJTubO+zTFKUlZ2gM6doapLWLcXy/sF3+jmHYMBIekVtHhBwOdHl57XrPhMQQTd4m1Ao1AgLuoJu9TXtZULJAni4JONpu0kdDrVCjEBT4QocvZAICCcYEUs2ppJpT6R/bn9MzTsegPnpSneT341q3Dtf6DXh27kSdnETEeedhGDYMQRAINjRQ99knaCOjiZhyGqqDlRPugJsfSn9gf9FCqirX0SsimxGj7mJZ1Y8sKV9CL0MGZ0SMIRQbQavfxuik0cTqY/m/Jf/H7qbd8nsuKEjUx5KhMjMudhA5CUP5vGoFW+q3MjppNBNTJ7KiYgU7G3aSFZlFD2sPqp3VNHmb6GHpQW5ULqOSRhFnkJPWRUmk1FZKSAqRFZHV5cVRCgRw/vgjgcoqtDk5BOvraPnoYwI1NWhzc/AXFROorJTP0WpFdDjkpF6lEkGhaOd+az3nHJKe+jsglwBvX1qBzxXAEqsn4A1RW9BAU52DgHspCmU0St2IDuclSRJILhB0CIJ8Me03MZYe/TWU5ZfSUFaNvbERS0wMpkgt+cs+RwwFEBRKzrnvYUKBAFsXfE1NYUE7B9u4jJ6cdsOtLH37VWoOFGCOiWXEzAsQBIEdi7+nvrR9rs8hjJFR5I0/hY1ff9F+hSAQlZjMkGkz6TVqLBV7duFobCAuqgdWSxyqFANiKEgoGEChVGG0RoAInt2NBBs8KC1aBI0CX4uL+r2FNJdU4hc9mAYlkjv9FHn8QZwtzexbsxLJHSJOn0bx7k1s3fY9AJlDhpPebxCOpgbM0bHkjBqL1mCkpbYaATnxVmcyo1Aqcdtt1BbtJ+D1IYohGspKaCwvJb3fIAafMR1HcxNbF3yF3+tFpdYQnZJKfGY2XpcTW12tLEZ1etL7DcRgsSL6gvgKW1FG6lAnGhHFIPbGBqxx8QiCAskfwl/uwL6kHH+ZHWWEFqVVK3vMHCOqOAOCUkD0hUCSED1BJG/3/HTQK2jNUVBjtNPqtRMIBCgvL8fr7bwXWr9+/Rg3bhxxx9nr62i0tKxnX8HDuN3y502tjmor45akIAqFHrO5D4FAK4FACykpV5CWfjNLmhysbHEwwmrkzFgrflGi1CNf83Y6PTxRVE1zQH4/VAJkG3QIwB5Xx9eYodeQpNWgFgSaAkEa/AEaA0HUgsA58ZFcmRTDALP+Z6vPAN5cVcyTC/aiUSl4ZHofPlxfTovLz/K7J6I/Snn/8RAWOd3gt/LJCYkSlS1uDtQ7cXiDaFQK3P4QNa0eCuoc7KhspaL58PywWq1A0CjxuwKIFjX+gVGgP6yeTQoYqm/hXPEDot1yx3CtJp7MzD+TmHhul31DbDYbn3/+OZUHb1rRkpnBgR6kSjHoMqw4NK3sLFpOceHmtm0EhQJTZAzmmGQM1mQEVTb1Zep2iZjJvSJIyTJjtRcj7NmCb+FXKNztBYqg12MYPBhNejqa9DR0/fqjy+uDQqtFCgbxFRUhutzoB/Rv6zDc5Glia/1WnH4ng+IGIQgCP5T+gN1nZ0TiCAbGDcSkNiEIAp6gB0/Qg4CAQW1oF6U4VLHjWrcW7658JDGEOjkZbY8eqHr2ItTYiGf9WhxLlyLaO16AVYmJGIYNxbl02WH7fkFAlZiAKjoGVUwMqhjZL0NyewjW1xOor0cKBJCCAUINcv8g/YABJD71d9Tx8fgOHMC+5kMt4gAAMPZJREFUN5/9e1Zjysqhx5BJKBta8JeUErK1Inm8KEwmVDHR6PLy0PXufdR+PlIwSMvHn+DeuhXD4MHo+vXFt28fgZpa2fQtJUUWa1otzuUr8GzbRrCxEfeGDV22IADwaSxUZZ2B05SM6PUhSCK6hGgMffsSDIFYXYGwawPoDSjGTsXrC9JQshC3Q0KlG4kgHD5nSRIJur8i5C8FYNAZMxl13hWEAiK2+ga2LphLef5WvM5mBIUWlS4Lrd6Ns7m0yykQkIWIq6VZvrEeEcHQGo2Yo2NxNjXK0zY/QSEoEQ8+OevNFkZfcBn71/1I+Z5dGHVWMpMH0TdpPFKNHykUQpREBEFAoVdhGpOMZXwaCo0SSZRwb67Dua6aQI38+VDF6jGNTUaXFQESuLfX49xYi9iNyiV1iomI6T1RJxrx7mnCV2LDX+kkUO1se/CX4pUoco1EpSYjBURC7gCiO4joDqA0adCkmlEYVEgBEaVVizJSNvgTvUEElQJBpSBo8+EvsSFolajjjW1jQG426clvwlfciirWgK53FEqT5tAfkkCti9b5xYRs8o1WYVChitGjMGkINnkINnoIhUI4BS9mSYcCOaobQkQhCGiSzASaPLi9bmyJIXzxCiyp0ViURrSrbISafejyotGkmHAsq5BfIyJNggOb4CYghIjESIwlGoNej8KoRhWjx2+QKGuWc2ncfg8tfjv19iaCwY4PmRaLhcTEROx2O1qtlqysLHJzc09YxMbnb0QMeVEo1Nhs26mt+7qt35NGE0vv3KeIiZlElddPg8+L09dM/4gELBod7pDI6hYHa1qc/NBko9Rz+HNjUCpwhzpOfyZp1bhDIq3Bw+JPrxCYEReJXinPEsyIjWCY1dixOakkIUp06W1T3OBkwa4a1hc3ExRFLh6exu5qO2+skqeSHz87j8tHZbTd69KjT2z5OIRFTrf4PZsBFjU4WbS7js83V1D8E78TnV5FdJ8o6oNBXAqQdEokgwpBpWCowUuGbzk5wbX0Yh86tZXIyFFERY4mKmosen1qu30Fg0HWrl3L6tWrD3dOF/Wki7EkihEki1Go4nRUBvazJX8BXr8TpaAiJB2+SCRm5xCVPACnLZG6MmWHaQRBgJhQNdH7l2ENNqAX3ARs8mvS+G0c+TVSGAxIooh08KlKFReH6ZRJKCMjUUVGoemZiUKnw7tvH4JKjfWsaSiMRkI2m9yAsLUVRBFlRATBhgbcGzfhLSjAX1KCoNNiHD4C34EDePPzkRBoiB2IVxeFIIZojcji/9u78+C4zjrR+9+z9r5I3VqtzfK+J7HjhQAJJBAgZChgBt4JdwLMC4EC7oSBywB1i4GBqknmDpMJBIbM+1JALpWBIQwMzA0EshMSk9hKnDiOI1u2ZEnW0q2l9+Vsz/2jZdmyZMeAV+X5VHWV1Od06/R59Jzz62f5PZOJ9QCE80PUZQ7Q7AyiX7GNqfgqqqlJ3MMHcV0PTzUJFUfoqCuiqy65A4P4qllU4WDrQY62vpZsbBnFYDOxXD+dg78iXKxlChWApxqonoOiqeCe4TfQE8+p34++YTOVVVuJb1xB3aoO7N79WP2HwBMUn3iC/IEjTCQ3kE5upOqL05h6jpaxpzDt2rn3DB9OOIkxPYJlRhhpeQ3lQAMxb4r61hDu4GEsPUJ50xspBxuxskVSORPPm7nx2UMgSqjGUhTFpMtU8asw4QgmHYEnbOzCz/Gc2ixDX6iJ1tWbmRw8gGaYmAGT8UN70HQdd+ams/zK7cSaWtj78K+wyiV0xSTha0VVVDzhEjESxH2NqIaGCIATcxENOrmJcXLpNOs3voFlSzYz/sg+Qm6UdHUYZ61K1+YthMwY/u4Y+cIkP7n97xBpm+aGbi7f9jaq+6fRKzpZfYpKs0Xn8o2Mj02w8+geRu1JttsrWOMen27+ojbIYS3FNns5TSLOtFJgyl9idfsKRNauLasCoCoohopXdShQIa3mqCo2CS9CUPiohDzU9iBqxUNzVcygj0g0ii/ixxkvUXp5EuF6qKgopoqYyV0jZkavmU0hnMny7EKQZ0qNGOAKvJIDSi0oOXlGkVbnw7+yDnusdMatLWrEQFQ9hOUiEEwpBY6oaYa1KSaUHJ4i0BWNZDJJLpejVC2jqiqGYWBZ1rxxLwDRSJSu9k6qroXneXQv6UJkbHYe2E2+ND9YDYfDRCIRKpUKmUxmwfcMBAIsX76c1tZWDMOgvr6erq4u1FMsuPn7KpeHeXHfJ9H12riZqemdTE4+usCeKkuW/DnLuv+atBvii30j/Fc6M7vVVBQ2RAK8VCjP6VaK6xrXJ2M8PpVnzKq1niYMHV0BU1X5wJIkt7Q1oCswUrXZVygzYTu8OREjaS48WQCgYrs8fiDNEwfTDE+X6agPsrYlyg0bW4j4DVL5Ct94pI97nx6cl1vsmI9evYzPvmWVXLvqYnAxBznHCCF4bihDxXapD5l88od7eHls4W4bL6jjJX24bSFExCBEke3it7yN/6KZ2g22ru41rFr5pXkpuIvFIk899RQ9PT1zmm0DwmSt00ZY+EFVaPSixLwgdsRhzBvgwKGnyVUnsLzaaxLtS6lfcgW2lSQ3ZVLO5XCsIqCgKCaKNnf9Gr9mU+em8Kf6CKUPkpjci+Y55BtXU/HXUT+8G22B2VLH/mn1ujp8q1dR2rV7dnFCgULFX4+r+dCdEo4epBBqoRhqpRiqrfYbrE4y3XYleXF8oT5FVOk2XSy1yLCaxucF6KCNXHWMI7nfoig+NHMVilYPeKhunrBWJWo0EDWbcXQdvd7l8KjAcuZfLDWtNt7EdUQtZ4mXRbXGiZXL1NtTGIkEbqSeSqaEVaziNwX+uElVEzjYtJoOydwAR/srjEbWMZFYhzhhwLniOehOiUB5AkV45GJLESe14il41KvT6PkJJnwduHoA1bMRqobgzC7wzd0RVJ7hcE+ti0TVTTa3/wndHP+fqigWzxV/w+B4DyFfPapPI5+rtRDV+1oIaOHZQHnrjX9KuZxn5y9/SE6zsGL1BPGzPbyVNtpRRO2mXqCCHxODuZ9Ji9W6etysRc4u0KeOMa0WKChVYiJAkxen3gsTFyH8oQDhq1opPp/CHS/j4pFTyuSUEnmlTFGpklfKTKh5Csrcpv3X6GvYcsVmnvMO88Tup2bKVGPdkpW8OPgyHoJON8kb7Q2k/UXKK3Xat6ygXC3x6K8fIZV/5TFnAIZhsH37dgKBAE/+ttal3OREafXqaQs3Md1o05N+iapt0dDYwJKGFtryMexsheFKGk1TaQo3oPt08lSwi1VE1kL1FDRVxS05eMIjIAwiIkBOKZNWc0RFgJVN3RiuyvTENLZn4+LhKrVWE6XBh94SoqEawThSpWCXOKiMclSZIq3k8Js+4o31xGJRdEfl8NAAuZNacFVVxTvNIqCKopBIJKivr6dUKpFKpWa/fC0kEAjQ1NSEaZqkUikymcy8fRobG+nq6iISiRCLxWhtbaW+vv6sBTQnc5w8u3v+bE4umhoFVfXheRWCwW7q6l5HQ8ufUTKX8e3hNP/76CRlz0MFmn0GAhitHr/2tftN3lAf4TXxMG9KRglpGrYneLlYptVnkjhN8HIqtusxlq3QEPGxe2Caz/3kBYan5696HzI1VjZHeH4oM5sH8fUrG7huTSPTRZv/vXOAquPxv/50I2/bcH5WVJdBzhm4FIKck+UrNl/9VS/9kyUUYLpkMTxdZqo490Kg1vuoLAki4iZosCYwyhrvd6wTz7FcOUIstBRV9VFffxXtbTdjmrUmWcuy6O3tZWBggIMHD5JboLsm6gVo9uIkRZSAMPELgxh+CuUJxssDjJX6yVjjeMy/mClaBFVfiarXo6gRUEIoahRFqXUnBYIakTqd1NFas3fAL+gKjGNZHuWSR7kMFTVE1YigeTYN4z0kJvehOyXKrWsYr99EVm/EW6CLznOncUqPILwCItBJyEywwteIa5TodwbQg/VkdIu8erySt7hxtjor0Col+it9pMIeuuojqdQRVEPYikdKzTKmZlCFQhAfPldH8TxCik5IBJhQCqTVAkKpjbWJeD6CtkJJ98hpVZKWiX+qgt9cjuc3mHI98rZNvDLIEk0hZ6dJVYaouEVQ69DN1ajmGnRsGrUcljVM2R4h41RR1AhCFBHCQYSX4ks20uXzU+f66a+4TE+5uNXn8dwUdWY7ISPKaPElPK9EZ3wz8UgDh0v9WJaLEAqNvkbaw+1oeBzI7GKiOIBh+GnTl9MW34SraxSsSYL+JNNKkWo1w1qlm6AWZpoCRxilqLsEFR+tZhjVUhnzirh4hIWfglJhXM1QVWxsXKbVua2WdV6IFiPBOBkm3RymorOmaTlrG5aTqAQ50tvPQe8ojuJh4TCkTiKUU1/SWtw6urwGppQCI9o0eWX+BX22DikK6zpXY4b89Oybvzp4Y2MjqdT8NAcBw0/Znj/2QVVVmhqbCAYCjKXGKZfLhMNhTNPEcRxs28ayLOwFVvU+X9SZAaqnuy0oikJrayujo6OnDVgAdF1n2bJlrFq1is7OTurq6picnGRiYoJYLEY8Hse2bWzbxufzEQgE0E/IqG7bNgcPHmR8fJxwOIxlWbz88suUSiW2bNnCli1bME7Mt1Stkk6nKZVKBAIBotEosVjsjz8xp1CtjjNw5G5A0JB8E55nMTj4baYzv8M0G2lv+wtS07t5wHsD95U3gqLR5jPIOR5DFQvrpPO8LRbi71e2sS5cG0/ZV6qwO1tkbTjAhnCAQtVh/2ie7oYQiZDJvpEcO2cWOQ6YGt0NIVY0RvAZKpmizRN9afYM1nJtFaoO+YqD7Xp0JoKYusbjval540Oboj7esq6ZFU0RhqZLPPTSOIdOSDZ6RUec/3H9Kl6z7Hg3nu16s+sIni8yyDkDl2KQcyrpfJXnhzL8uGeYB/ePz2tK9IIablsItzmA32+ziv2s4UW2sZNmNUNT4420tr6HWOyK2aUmXNflxRdfZO/evXieh12xODo2suCFTRUKCRGZnQYe94KEbZWoZxBWTPLeBEczByiWM9heFcez5gRBvnADwothW2UQDqoWRvfFcJ0gihIGNTITCNm1Va4VExSjNsZDCaAoOsIrY5cfA6+IGdiIP9xCvtSP7rOJBHxYlXEsu4AViZENnvpbnCKgUUSZUPK4MzfMRi/ClFLAUQSGWSIcmkZVXTxPQwgVAQQDOULhKarVENlME/l8EiFqwZam2cRiY0SjaSw7QKkYp1iMY9u1i5kmVFzlpPMqIC6COIpHGWt2u+6B5jgsUZqpJ0pKzZFTSkQcA6+cRfdFyRg2Wa0883kUOr0krVaYI9k9ZKNBMINs81bT5TVwRIwxok7iaCoKCtEqjJYPU47XM6WVEYpAFQpREcDnaeiKTk6pzAkGT2R4HlE1zCRzZ+aoQkHAaYMQRSh0eQ1YOIxo07MpBRbi9/sXHCza3d3NsmXLiEajpNNphoeGSU+kyefnt4CaZpHmlmFcZzOxWAfRaJRoNEpTczMi0cCyaG3q8m9+8xueeOIJHMdBURTe9KY3sX37dh588EF6e3u55pprCIfD/OAHP8C2bTRNo6Ojg1Qqheu6bNmyhR07dhAKHR+bIIRYcKB1b28vjz/+ONVqlde+9rW0t7czMDDA4cOHGRgYIBAIcNVVV9HZ2cn4+DiHDh2ir68PTdPo7q5lGj569CiKohCPxzEMA9d18TwP13VRFAVFUcjn80xPTxOJRGhra2N4eHh2ORjDMPD7/ei6jq7raJqGrus4jsPY2PHUDx0dHaxfv5729nYcxyGbzda6oUol2tra6O7uPuPp1QXHpeqJP6hF4mwSwsPzbBRFw7JSFIoHcOxs7X9ReAi82jgke5qBI3fjOLUUAWO0MMBSUjQRVcpcv/ojvGg3c8/IBP3l04+92h4L8d87m9geDvDrl8aJBQyu6KjD9QRD02We7Jvg8QNpnj0yjTNzba8PmfO+3P4hji1hoyhw8/ZOPvOW1bMLItfOh+DJvkmGp0u8dkWStrpXzoJ8Psgg5wwspiDnROO5Cv++a4ifPDtMKl+lbLlzbhVeWMeLmYigDvUGl0f3sIJeAl6Rlb5JNsQaaajbQjx+JeHwWtQTEr5VKhWOHDnC8PAwY2NjlMtlcrncgi0+x2hCZYXbzFq3nbgIzg46dIRNxkmTs7MEzXoM1Ue+NMxYeQBLV3E0BdWyMDwI6zECWhhD9c08TLSZQaxCUTDUIAoehqJT0lyG9AwDWppJ9RQzsoSgLpwlkjyCpjr4qgnigSDxbo1Q1ETXTTIl+M1LLoo3yNqmvQTMCp6nMVGJ88DIdRi6w6r6PsqOn5FCC12BI1xWvxdddSjaQTJWnBfLW3m6tInhUjPL4oe5teku/EqFnBUhZBQx1Aj5bIRsPkzVCmKVouSrjZQck2SsHyum0qyOYGgW6XQXE+kOItEJGhqOUBcfxR/Ic/DgdlLjta4iwyij6zaep+JUosREkCk1PxOQzb95+DGosHDLgaZZaJpDsRrGQ8GnHM/UrCgera29hIIKqdFlKF6Cpo5WBgcHKc3MqlMUhfZkK61dbQwODDI+NYjr6rS3tlPfkCCTyRAKhejo6CAej9cWWfTC+CYERmsIp9mgr+8p0unvYPr8dLS/ActawQsvHOXAgQOzwcTGjRtpaGhACEF3dzctLfOby2urKg+zd+8hXhgaYkVDku6lEUbT/5ODto+1QZ1tm3+IYUTJOy5/ubePJzJl/rQpxldXdeKfSexXKpVQFIVgcOEL/djYGAMDA6xfv55wODzbIuIBRdcjqs9tYRRC4Dg5VNWPqprnfBzDK5menkbXdcLh8CmPZWJigv7+flpbW1my5NRJCYUQuG4RXV84x82UZfGT0WGezFTpyTukZmYDvSsyzH/jXuLBdiLRDQRj2ylqrcScARx7glB4FT6zaeZdvFNOrDgd1y1TLg8hhI3P14zrFsnl9jI59RsmJh7GtqcXfN00ce7nHdiYrGYfMbJU/Rt4TLyO3Vbzgq8BSBo6H03Wk3DhSL6C6gqCAlYkw2zuqCMZNOmfKPLR7/fQO376WaQNER/pmRQlPl3ldSsaiPh18hWb3vH87KQVTVW4oiPOa5YlaYz6CPt0on4DFBiYKJIt21y1PMkVHXXkK7Ws6ucin825IoOcM7BYg5yTFasO978wyn09Q/QcmZ638KTwqeCBYnu4DX7UdQG2mzv5E37KEi1HOLyegjCZclXW1q+kreWd6EYMhIfP1wwoTE9PMzIygqZpeJ7HSP8wR4ePMjY5TsWemzPGFDoqtW/1Fs6cb/am0DHQKCon5LIQGn5h4MPALwx0NARQViymlAIuHnERwkQjr5QpKce/3fiMIg0BG0Otrepw2I1hhQSXd+6m14nz2MjrmHLrKIcjaCULJW2BI9BUj0wxghC1gExRPELBCqrhkcucOjGZogFCILyFbxCqX0HzXGxLRVE8wqEyakIlF0tgjBaw0gqzgURYobqiDnOigJEuoSoeqgGG6WD4bBJikqSSZklolHUNK2hVHkALHuFIfgkPjl7LuFiBpdexOrmXKwMPkko1MzDZSabcilACtOkDEPDRbyzFFwhxdWIfRvEIvx3sYMyN40U0SpafiVQc11PZ3LyPjiVpUqFNqGRZXtjJ8FQLz6Q2U7AiKIaGEdJpbjRoSThEEkXs9DRH+wSuY1FXN4kXi1GMXkZXUxNvTVS5KpEg5m/mu/3P843hPA1qnj+PpXih3MrPDwUxvBLdRh+xSIGCP04D42wOlNkeC2PYOkawgYPUUXVt8laRB7IBdqdbaKqzeU0iwtsCh0gWfslQboAH3e08pV7PUZFgR7DI2+3/n+9Yb+OQspJmMcKfB3YRMEL8W2YFwwfjaONl7NUxupsnuK7eoLtuPXrpWYLlF1gdMvGbMcrlQRynTFPjm4nVX8NvJsboLdm0hpK0mRBI/388m5nkm/b/w5it8YWldbwjXubH035eygxTn/8Fmj1CP924epJ6+zLqtQTvXpOnUc2RqN8OKExN/RbXKxOLXoHha+F32SJhTeOy6PFgSwjB09kitifYEQ+f1VWfhRBM5Q/wVKqPrnA9a5Ib0LQAtp1nz8Q+9mTSbKhrZ2vTJnK550iN38/E5CNUKkeJx64k1PQeRqd2M5Z9iYy2lBfFGv6PtZEq8xPUAbSIoyRJkyXGMB14ioZflOniMJvZxWqln7SIkFPq8fuaaAo2cl0ySTK0BMueIJfdQyr9a4Rw6Oj4f4nHr2R87Odkc89RLg9hWQvPICzj5yCrmaYOgUJJiZDXl4Jam4H0YHUtJRbOJ6UCl0eDdJgG45bDS6UKXQEf76yP0vdcivt2nWpVbwgaGlXHw/EEybBJxG/MLrCbCJlc0VnH61c2cPWKBjoSQaaKFofSBda0ROe0ukCt60iIWguNrp3bpKcXkgxyzsCrJcg50XTRYufhSQ6OF3h5LMejvWkq9tzZPcKn4tXVKrJqCPCr2H4f+DRiTLNB7KFImCkS1Bk5loVLdPv6aWGAjuhSlsQ3UqkexaqmiEY3USo18XLvY2Qz/ZQrQSrlCI5rYFsBLKt2kdZUDZRaFxmAoVvUh2ymywq27UPXLRRFYNu14/L5iqiqR6USnmmh8NA0B0238fsrdLSZNDQM4njP4QFj5Sa+dfBDjIzVcl0IrdZGe5qeEwC8gIbiCZTqSV1JSR+6quJMVlAMFTVq4mSrc/YTmoKiQbJOp7shzK4D2dnZMacjdAUEKO7vVzVDiQpmI0z3+llgONTCf0vhFc/BH0qocHIP3Ow2TcFtDoCmoE1XEaqCFzJQECglFyVrzTsuL6zjJf14dSZq3sY/lcNqCmN1xAFQpqsY+7OoeRsvbmJtSaJmLCJ9Y1Q8P56p4TYH8VoCx7ONC4FSdGqPkoPieKipCmphZpyCAtblCZSKizpdxQsZiJCOYVWJiCzlljpKRpg407jo5JS54z9U4c4bH+YTZarK/BxW6ngZc08tB5W9No7ZBsuVw3QwTEhMAgoZ6nhW2cYEtVWgN7GXtxs7WRpfwT2FdTxRrv1/16k2DVqZCUcjQIkOBgjrOoqvk4hSpt5+mTbDZm39ctbUryASXEK6OMwTqWGqno2pCIp2gUw1S84qMmop/MbbRk6pnetmMYKOTZY4+RM+c4QcLeIoCSZIiAnsssp+cwODRq0bDVegHSmgjZVBBb9ZpTs+yJa63VwWeZ4BtZu7C39FKa+hOLU7tdvgR/ExbxA9rgDXg5n8K4aospJeNFwClFjBAZKkmCLBJA1MkKRABAsTHYekmqNCgINWO0XCBE2HggjiCgVsD6XiIgz1eLoOxwPbY10kyApV47mRHJWqgw+FjqCP1yYi7B/M8OjLaUxdZWNbDMcTvDyamx330pUIEg0YRPw6Pl2jdyzP0czxbt8ru+r45k1X0Bj1k6/Y+A0NYxEHKn8MGeScgVdjkHOysuXSc2SaeNDA8QSf/tGeOYPMzpTwa7hJHyJsoPgg4JQIiBJd9UN0BwfIFsMMTixhONuMVdJp8E2y0neA+oBJJLqEdEQjaxo05XI0WyOsi91PwMjRxwryxFjFS0QokCXGFAk8FDxUqq7BuNfJYaOLoXwrkwdD2AUV03QQqkLV9eFVaq1UMDMry1RRZoKN+qYgXckQhUwV3adhNAdxghquLWirC3BVex2e57EvXSCTrWJVHLa1x/ng6lbCJ3U9DJQq/OxwbXZLezzAxliIrsDxLojBfIXbdvfjCxh0NoQ4miszMFakMlpkeqJEd1uUpWuTGBGTYtnmyHMpnn4pxaal9Sxfk0DXPUqlCSwrQrrg8lKpTNZyUQs2aroyN6BI+GiJl9HKRUYnoriWqM2+i5uIsI5S9dCOFlEcgaIINNPFtnRQFbxGP8QM2rxaXqT+eK2JWx8oYGQtRKXWbeUG9NosvtYAWxtLNNlHGB7N8/JIA9lcBM9TUVRw20OIgE40a6GWytiVCpXqwt/gT9QYKxIL+UiXw2SmF07UBqC3mxi2Q3lsbkQVjFkUc+a8YCkRymE1RJnSI4TGK1j5+d118ZDB2uYoTx06/Ywo4VOxV8YQMROEIDCdJVFJo4RVMqEkea82e++q4JMs0Yb4cfk9eGgkgpNsU59lxNtKxU7Qpik89dgQrlu7oQkVrB21gEWpuLV/XMut/Wyo+Bpdqr4Qrq3WgrOSA4aKElcI6pU5gcfcA54ZfDHzs1JyUXWPpDnJBA24il4LREZKeBGjNnFBCJS8DR6E9CqlYADvWBd21cUczhGYKFENmljJ2sxOXIGxP4OatREKiJCOYqgoZRdOkbRPAYKmQtGaW2CqAutaApQ8jazlUtGh5LiIjI3wBL6gilKnkY+F8GK1TPFCAWWmyVoY6ux5PPZAUfBiBupkFf1QHgS4XWGET8U/WMQ9YTp9c0utVezoSP506ZlOqysR5LZ3bWTHssS8bZOFKsVq7Zy0159Z0j1JBjlnRAY585Ush//zwijFqkPB8RjPV0jlKmQLFul8lbzjUvIEpqbgUxTyZYtS2T1t5RcnBBVnTAHqdFxNn+m9EeiKi3MsmZwyc9HK1L7xC1MFy+N0lwe9zsdfvXUVH1u3hN6x/MxshFdeE+dCsl3vlN/kPCE4UKowULJ4YTTLTx88xGi6xLu2t3Pb29fjm1mfy/UExaqNZmoMli2ezZWYth02hwIkXWiNVtE1hZwXY6BcIeEzafLphGaSMB4pVzlasVkZ8pM09ZnZN/BSsUzB9bgyFpqz6rBtT+N6OkdzCvVBk4BfR1HANzNl17ZzPNM/wX/tLeAKiyXJLE2BesbzIUxdpTUWYFN7nKXJ44N0p4oWv+2b4DcH0uwemKK5LoA/bPLYntHZfY6t5v6G1Y381Q+ew5pJkLZyWR03XtYKeZvv/Laf6dLcoMZvqKxqitCVDFEXNGmI+HjPlnYifp0PfncXOw9P0lbn521rQ4wVTIamygSCOgfHC6Qzpw6+TicRMogFDA5PzB2cfWW7g+dZ9Bw9/eBOTYGACYXqyc8LlidtotECFccgnQlheTqKplKuOpTLgmDIJd4aIJ32sDIuQgGvwY/X4CfhL1HutbBn0s8EYipORWBXj1dwv6HS0RQkX3IYn67M6/6eY4HlN5qjfj553QrqQybD02V+d3iSniPTTM4Mog2ZGpva48SDBmPZCs8OZk57Ls6VRMhkqmTNubaZmoorBPUhk1VNERoiPnRVwXY9ipbLsoYwf7KpFUWB54cyBEyNrkSIta1R2SJzlskg5wzIIOfsKFkOvzs8yTP90xxKFziaLePzaRQsl76judqXR1WhuSXMFV11NNYF+NnwJKlcFVwPpexiTFXwHFCDKo6qHu8u+D1tXpXkNRubmShbKJ5geSTAirogyxtCNAV9qIv4W5LrCSYKVZqir9xKslj8Yu8oX/z5Pi5vj/PpN69iVXOt5eSXe0f5ws/28e4rlvDZt6xGnemeKlQdHnhxjJdGcoxkyrx2RZJ3XNZKxL9w9mjb9dg/mmNdawztpDEuFdvlXx7t4+fPjzCeq+J6gss74nQmgrw0mmM0UyFgatiux3iuFo0ETQ0hoDzTRawq0JkI4Xgeq5ujfPVPN1F1XN729SeYKFgEDI2O+iA+QyXqN2iJ+Tkwnuf54eOLfjZFfXQmQoxlKwxOvfJaUyfSVGXBpG71IZNCxZkNFCM+nWjAIFexyZ805fjyjjjvvqKNwakSvzs8yeF0kaLl8Lb1LXzh7WsRCPaP5ihZLpqicPWqhgWnGqfzVSYKVZY3hucEBAMTRV4cyRLy6RiqykShiuMJruiI0xj189zgNLv6p3i6f4rDE0WKVQfHFfgMFSFqZQ6QDJu0xAK0xv0Uqy57hjKEfTqfevNKIj6d//WrXmzX40OvXcqfbWkn5NM5milz/wsjqIrCtWua5gTe0oX1qglyvvnNb/KP//iPjI2NsWnTJu666y62bt16Rq+VQc65l85XOZjKs2FJbM6NRAjBSNWm5HqYqkKraVCsOkQDBkerNj3DGfrH8jSbBkLAtGWTtV2Spo5GbeXnqN9g69J6GiI+DqYKhH06yxsv7pYZ6fxZaIr2ufxbQjAbTJ2sbLmULIf6kInlejx7JEOh6rC1q55YcH6ANVmoMlm06E6GFhw8OjhZolB16EoG5wQMQ1Mlnh/OsG8kR9DQ2NAWIxYwKFkuIZ9OQ8RHz5FpHutN0VEf5L9t72SiUOXne0Z4bjDD4YkCVy1L8rc3rsV2BQ/tH2dJPMCOZQmMmRlmveN5nh/K0Bjxs7Y1Oi+oFkJQdTz8xtldq+gPZTkeAoHvpO5lzxNzyuvYrVB2F10aXhVBzr//+79z8803c/fdd7Nt2zbuvPNO7rvvPnp7e89oMTUZ5EiSJEnSpedM79+XdCfhHXfcwYc//GE++MEPsnbtWu6++26CwSDf+c53LvShSZIkSZJ0gV2yQY5lWfT09HDdddfNPqeqKtdddx07d+5c8DXVanU2cd0rJbCTJEmSJOnSdskGORMTE7iuS1NT05znm5qa5qQdP9Ftt91GLBabfbS3ty+4nyRJkiRJl75LNsj5Q3z+858nm83OPoaGFs5AKUmSJEnSpe/CroT2R0gmk2iaNrug3DHj4+M0Ny+8hojP58PnWzgltyRJkiRJi8sl25JjmiabN2/m4Ycfnn3O8zwefvhhduzYcQGPTJIkSZKki8El25ID8KlPfYr3v//9bNmyha1bt3LnnXdSLBb54Ac/eKEPTZIkSZKkC+ySDnLe+973kk6n+du//VvGxsa47LLLeOCBB+YNRpYkSZIk6dXnkk4G+MeSyQAlSZIk6dLzqkgGKEmSJEmSdCoyyJEkSZIkaVGSQY4kSZIkSYuSDHIkSZIkSVqUZJAjSZIkSdKidElPIf9jHZtYJhfqlCRJkqRLx7H79itNEH9VBzn5fB5ALtQpSZIkSZegfD5PLBY75fZXdZ4cz/MYGRkhEomgKMqFPpxLRi6Xo729naGhIZlf6AKS5XDxkGVx8ZBlcfE4l2UhhCCfz9Pa2oqqnnrkzau6JUdVVdra2i70YVyyotGovIhcBGQ5XDxkWVw8ZFlcPM5VWZyuBecYOfBYkiRJkqRFSQY5kiRJkiQtSjLIkX5vPp+PL37xi/h8vgt9KK9qshwuHrIsLh6yLC4eF0NZvKoHHkuSJEmStHjJlhxJkiRJkhYlGeRIkiRJkrQoySBHkiRJkqRFSQY5kiRJkiQtSjLIkfjWt77Fxo0bZxM27dixg1/+8pez2yuVCh//+MdJJBKEw2He/e53Mz4+Puc9BgcHueGGGwgGgzQ2NvKZz3wGx3HO90e55L1SWVxzzTUoijLn8dGPfnTOe8iyODduv/12FEXhk5/85Oxzsm5cGAuVhawb58eXvvSleed59erVs9svtjrxqs54LNW0tbVx++23s2LFCoQQ3HPPPbzjHe/gueeeY926dfz1X/81999/P/fddx+xWIxPfOITvOtd7+LJJ58EwHVdbrjhBpqbm3nqqacYHR3l5ptvxjAM/v7v//4Cf7pLyyuVBcCHP/xhvvzlL8++JhgMzv4sy+Lc2LVrF//6r//Kxo0b5zwv68b5d6qyAFk3zpd169bx0EMPzf6u68dDiYuuTghJWkBdXZ349re/LTKZjDAMQ9x3332z2/bv3y8AsXPnTiGEEL/4xS+EqqpibGxsdp9vfetbIhqNimq1et6PfbE5VhZCCHH11VeLW2+99ZT7yrI4+/L5vFixYoV48MEH55x/WTfOv1OVhRCybpwvX/ziF8WmTZsW3HYx1gnZXSXN4bouP/zhDykWi+zYsYOenh5s2+a6666b3Wf16tV0dHSwc+dOAHbu3MmGDRtoamqa3ef6668nl8uxb9++8/4ZFouTy+KYe++9l2Qyyfr16/n85z9PqVSa3SbL4uz7+Mc/zg033DCnDgCyblwApyqLY2TdOD8OHjxIa2sr3d3dvO9972NwcBC4OOuE7K6SANi7dy87duygUqkQDof56U9/ytq1a9mzZw+maRKPx+fs39TUxNjYGABjY2Nz/mGPbT+2Tfr9nKosAG666SY6OztpbW3lhRde4LOf/Sy9vb385Cc/AWRZnG0//OEPefbZZ9m1a9e8bWNjY7JunEenKwuQdeN82bZtG9/73vdYtWoVo6Oj/N3f/R2ve93rePHFFy/KOiGDHAmAVatWsWfPHrLZLD/+8Y95//vfz+OPP36hD+tV6VRlsXbtWm655ZbZ/TZs2EBLSwvXXnsthw4dYtmyZRfwqBefoaEhbr31Vh588EH8fv+FPpxXtTMpC1k3zo+3vvWtsz9v3LiRbdu20dnZyY9+9CMCgcAFPLKFye4qCQDTNFm+fDmbN2/mtttuY9OmTXzta1+jubkZy7LIZDJz9h8fH6e5uRmA5ubmeaPnj/1+bB/pzJ2qLBaybds2APr6+gBZFmdTT08PqVSKK664Al3X0XWdxx9/nK9//evouk5TU5OsG+fJK5WF67rzXiPrxvkRj8dZuXIlfX19F+X9QgY50oI8z6NarbJ582YMw+Dhhx+e3dbb28vg4ODsOJEdO3awd+9eUqnU7D4PPvgg0Wh0tptF+sMdK4uF7NmzB4CWlhZAlsXZdO2117J371727Nkz+9iyZQvve9/7Zn+WdeP8eKWy0DRt3mtk3Tg/CoUChw4doqWl5eK8X5z1oczSJedzn/ucePzxx0V/f7944YUXxOc+9zmhKIr49a9/LYQQ4qMf/ajo6OgQjzzyiNi9e7fYsWOH2LFjx+zrHccR69evF29+85vFnj17xAMPPCAaGhrE5z//+Qv1kS5ZpyuLvr4+8eUvf1ns3r1b9Pf3i5/97Geiu7tbvP71r599vSyLc+vkGTyyblw4J5aFrBvnz6c//Wnx2GOPif7+fvHkk0+K6667TiSTSZFKpYQQF1+dkEGOJP7yL/9SdHZ2CtM0RUNDg7j22mtnAxwhhCiXy+JjH/uYqKurE8FgULzzne8Uo6Ojc95jYGBAvPWtbxWBQEAkk0nx6U9/Wti2fb4/yiXvdGUxODgoXv/614v6+nrh8/nE8uXLxWc+8xmRzWbnvIcsi3Pn5CBH1o0L58SykHXj/Hnve98rWlpahGmaYsmSJeK9732v6Ovrm91+sdUJRQghzn77kCRJkiRJ0oUlx+RIkiRJkrQoySBHkiRJkqRFSQY5kiRJkiQtSjLIkSRJkiRpUZJBjiRJkiRJi5IMciRJkiRJWpRkkCNJkiRJ0qIkgxxJkiRJkhYlGeRIknRBXHPNNXzyk5+8KP9GV1cXd95551k/HkmSzi8Z5EiSJEmStCjJIEeSJEmSpEVJBjmSJF1w3//+99myZQuRSITm5mZuuukmUqnU7PbHHnsMRVH41a9+xeWXX04gEOCNb3wjqVSKX/7yl6xZs4ZoNMpNN91EqVSa896O4/CJT3yCWCxGMpnkC1/4Aicu2ZdKpbjxxhsJBAIsXbqUe++9d97x3XHHHWzYsIFQKER7ezsf+9jHKBQK5+6ESJJ0VsggR5KkC862bb7yla/w/PPP85//+Z8MDAzwgQ98YN5+X/rSl/jGN77BU089xdDQEO95z3u48847+bd/+zfuv/9+fv3rX3PXXXfNec0999yDrus888wzfO1rX+OOO+7g29/+9uz2D3zgAwwNDfHoo4/y4x//mH/5l3+ZE2ABqKrK17/+dfbt28c999zDI488wt/8zd+ck3MhSdJZdE7WNpckSXoFV199tbj11lsX3LZr1y4BiHw+L4QQ4tFHHxWAeOihh2b3ue222wQgDh06NPvcRz7yEXH99dfP+Rtr1qwRnufNPvfZz35WrFmzRgghRG9vrwDEM888M7t9//79AhD//M//fMpjv++++0Qikfi9Pq8kSeefbMmRJOmC6+np4cYbb6Sjo4NIJMLVV18NwODg4Jz9Nm7cOPtzU1MTwWCQ7u7uOc+d3Aqzfft2FEWZ/X3Hjh0cPHgQ13XZv38/uq6zefPm2e2rV68mHo/PeY+HHnqIa6+9liVLlhCJRPiLv/gLJicn53WNSZJ0cZFBjiRJF1SxWOT6668nGo1y7733smvXLn76058CYFnWnH0Nw5j9WVGUOb8fe87zvLN6fAMDA7z97W9n48aN/Md//Ac9PT1885vfXPD4JEm6uOgX+gAkSXp1e/nll5mcnOT222+nvb0dgN27d5+193/66afn/P673/2OFStWoGkaq1evxnEcenp6uPLKKwHo7e0lk8nM7t/T04PnefzTP/0Tqlr7XvijH/3orB2fJEnnjmzJkSTpguro6MA0Te666y4OHz7Mz3/+c77yla+ctfcfHBzkU5/6FL29vfzgBz/grrvu4tZbbwVg1apVvOUtb+EjH/kITz/9ND09PXzoQx8iEAjMvn758uXYtj17fN///ve5++67z9rxSZJ07sggR5KkC6qhoYHvfe973Hfffaxdu5bbb7+dr371q2ft/W+++WbK5TJbt27l4x//OLfeeiu33HLL7Pbvfve7tLa2cvXVV/Oud72LW265hcbGxtntmzZt4o477uAf/uEfWL9+Pffeey+33XbbWTs+SZLOHUWIExJGSJIkSZIkLRKyJUeSJEmSpEVJBjmSJEmSJC1KMsiRJEmSJGlRkkGOJEmSJEmLkgxyJEmSJElalGSQI0mSJEnSoiSDHEmSJEmSFiUZ5EiSJEmStCjJIEeSJEmSpEVJBjmSJEmSJC1KMsiRJEmSJGlR+r8l5wDw5/80iwAAAABJRU5ErkJggg==",
@@ -658,13 +584,13 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.11.3"
+            "version": "3.10.8"
         }
     },
     "nbformat": 4,
     "nbformat_minor": 1
 }
```

### Comparing `clophfit-0.7.0/docs/tutorials/prtecan.ipynb` & `clophfit-0.7.1/docs/tutorials/prtecan.ipynb`

 * *Files identical despite different names*

### Comparing `clophfit-0.7.0/docs/tutorials/usage.org` & `clophfit-0.7.1/docs/tutorials/usage.org`

 * *Files identical despite different names*

### Comparing `clophfit-0.7.0/docs/tutorials/usage.rst` & `clophfit-0.7.1/docs/tutorials/usage.rst`

 * *Files identical despite different names*

### Comparing `clophfit-0.7.0/docs/tutorials/usage2.org` & `clophfit-0.7.1/docs/tutorials/usage2.org`

 * *Files identical despite different names*

### Comparing `clophfit-0.7.0/docs/tutorials/usage2.rst` & `clophfit-0.7.1/docs/tutorials/usage2.rst`

 * *Files identical despite different names*

### Comparing `clophfit-0.7.0/src/clophfit/__main__.py` & `clophfit-0.7.1/src/clophfit/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -275,9 +275,8 @@
     help="Path to output results.",
     show_default=True,
 )
 @click.option("--verbose", "-v", count=True, help="Verbosity of messages.")
 def enspire(csv, out, verbose):  # type: ignore
     """Save spectra as csv tables from EnSpire xls file."""
     ef = EnspireFile(csv, verbose=verbose)
-    ef.extract_measurements(verbose=verbose)
     ef.export_measurements(out)
```

### Comparing `clophfit-0.7.0/src/clophfit/binding/fitting.py` & `clophfit-0.7.1/src/clophfit/binding/fitting.py`

 * *Files identical despite different names*

### Comparing `clophfit-0.7.0/src/clophfit/old/dil_buffer.py` & `clophfit-0.7.1/src/clophfit/old/dil_buffer.py`

 * *Files identical despite different names*

### Comparing `clophfit-0.7.0/src/clophfit/old/dil_correction.py` & `clophfit-0.7.1/src/clophfit/old/dil_correction.py`

 * *Files identical despite different names*

### Comparing `clophfit-0.7.0/src/clophfit/old/fit_rpy.py` & `clophfit-0.7.1/src/clophfit/old/fit_rpy.py`

 * *Files identical despite different names*

### Comparing `clophfit-0.7.0/src/clophfit/old/fit_titration.py` & `clophfit-0.7.1/src/clophfit/old/fit_titration.py`

 * *Files identical despite different names*

### Comparing `clophfit-0.7.0/src/clophfit/old/fit_titration_global.py` & `clophfit-0.7.1/src/clophfit/old/fit_titration_global.py`

 * *Files identical despite different names*

### Comparing `clophfit-0.7.0/src/clophfit/old/merge.py` & `clophfit-0.7.1/src/clophfit/old/merge.py`

 * *Files identical despite different names*

### Comparing `clophfit-0.7.0/src/clophfit/old/plot_tecan.py` & `clophfit-0.7.1/src/clophfit/old/plot_tecan.py`

 * *Files identical despite different names*

### Comparing `clophfit-0.7.0/src/clophfit/old/bash/w_ave.sh` & `clophfit-0.7.1/src/clophfit/old/bash/w_ave.sh`

 * *Files identical despite different names*

### Comparing `clophfit-0.7.0/src/clophfit/prenspire/__init__.py` & `clophfit-0.7.1/src/clophfit/prenspire/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,19 +1,17 @@
 """Parse EnSpire files and optionally build titrations using a note file."""
 
 from clophfit.prenspire.prenspire import CsvLineError
 from clophfit.prenspire.prenspire import EnspireFile
 from clophfit.prenspire.prenspire import ExpNote
 from clophfit.prenspire.prenspire import ManyLinesFoundError
 from clophfit.prenspire.prenspire import Titration
-from clophfit.prenspire.prenspire import line_index
 from clophfit.prenspire.prenspire import verbose_print
 
 __all__ = [
     "CsvLineError",
     "EnspireFile",
     "ExpNote",
     "ManyLinesFoundError",
     "Titration",
-    "line_index",
     "verbose_print",
 ]
```

### Comparing `clophfit-0.7.0/src/clophfit/prenspire/prenspire.py` & `clophfit-0.7.1/src/clophfit/prenspire/prenspire.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,268 +1,341 @@
 """Parses EnSpire data files."""
 from __future__ import annotations
 
 import csv
+import typing
 import warnings
 from collections import Counter
 from collections import namedtuple
 from dataclasses import dataclass
+from dataclasses import field
 from pathlib import Path
-from typing import Any
-from typing import Callable
-from typing import Sequence
 
 import matplotlib.pyplot as plt  # type: ignore
 import numpy as np
 import pandas as pd
-import pyparsing  # TODO: indentBlock, ParseResults
+import pyparsing
 
 # TODO: kd1.csv kd2.csv kd3.csv kd1-nota kd2-nota kd3-nota --> Titration
 # TODO: Titration.data ['A' 'B' 'C'] -- global fit
+from clophfit.prtecan import lookup_listoflines
 
 
-def verbose_print(verbose: int) -> None | Callable[..., Any]:
-    """Print when verbose output is True."""
-    return print if verbose else lambda *_, **__: None
+def verbose_print(verbose: int) -> typing.Callable[..., typing.Any]:
+    """Return print function when verbose output is True."""
+    if verbose:
+        return print
+    else:
+        return lambda *_, **__: None
 
 
 class ManyLinesFoundError(Exception):
     """Raised when there are multiple lines containing a specified search string."""
 
 
-def line_index(lines: list[list[str]], search: list[str]) -> int:
-    """Index function checking the existence of a unique match.
-
-    It behaves like list.index() but raise an Exception if the search string
-    occurs multiple times. Returns 0 otherwise.
-
-    Parameters
-    ----------
-    lines : list[list[str]]
-        List of lines.
-    search : list[str]
-        The search term.
-
-    Returns
-    -------
-    int
-        The position index of search within lines.
-
-    Raises
-    ------
-    ManyLinesFoundError
-        If search term is present 2 or more times.
-
-    """
-    count: int = lines.count(search)
-    if count <= 1:
-        return lines.index(search)  # [].index ValueError if count == 0
-    else:
-        raise ManyLinesFoundError("Many " + str(search) + " lines.")
-
-
 class CsvLineError(Exception):
     """Exception raised when the lines list has issues."""
 
 
+@dataclass
 class EnspireFile:
     """Read an EnSpire-generated csv file.
 
     Read the files and check the formats.
     extract_measurements(): create the measurements dictionary structure storing
     all data and metadata (description of measurement).
 
     Parameters
     ----------
-    file : str
-        filename
-    **kwargs : dict
-        keywords
+    file : Path
+        Path to the EnSpire csv file
+    verbose : int
+        Level of verbosity; 0 is silent, higher values are more verbose (default=0).
 
     Raises
     ------
     Exception
         If unexpected format is found.
 
     Examples
     --------
     >>> from clophfit.prenspire import EnspireFile
     >>> ef = EnspireFile("tests/EnSpire/h148g-spettroC.csv", verbose=0)
-    >>> ef.extract_measurements()
     >>> ef.measurements['A']['lambda'][2]
     274.0
     """
 
-    def __init__(self, file: Path, verbose: int = 0) -> None:  # noqa: PLR0915
-        def get_data_ini(lines: list[list[str]]) -> int:
-            """Find the line index containing Well and Sample headers in a list of lines.
-
-            Get index of the line ['Well', 'Sample', ...].
-            Check for the presence of a unique ['well', 'sample', ...] line.
-
-            Parameters
-            ----------
-            lines : list
-                List of lines.
-
-            Raises
-            ------
-            CsvLineError
-                If not unique or absent.
-
-            Returns
-            -------
-            int
-
-            """
-            min_line_length = 2  # for key: value
-            count = 0
-            for i, line in enumerate(lines):
-                if len(line) >= min_line_length and line[:1] == ["Well"]:
-                    count += 1
-                    idx = i
-            if count == 0:
-                msg = f"No line starting with ['Well', ...] found in {lines[:9]}"
-                raise CsvLineError(msg)
-            elif count == 1:
-                return idx
-            else:  # count > 1
-                msg = f"Multiple lines starting with ['Well', ...] in {lines[:9]}"
-                raise CsvLineError(msg)
+    file: Path
+    verbose: int = 0
+    #: General metadata.
+    metadata: dict[str, str | list[str]] = field(default_factory=dict, init=False)
+    #: Spectra and metadata for each label, such as "MeasB".
+    measurements: dict[str, typing.Any] = field(default_factory=dict, init=False)
+    #: List of exported wells.
+    wells: list[str] = field(default_factory=list, init=False)
 
-        def get_list_from_platemap() -> tuple[list[str], list[list[str]]]:
-            """Extract well list and Platemap from _metadata_post.
+    def __post_init__(self) -> None:
+        """Complete initialization."""
+        verboseprint = verbose_print(self.verbose)
+        csvl = self._read_csv_file(Path(self.file), verboseprint)
+        ini, fin = self._find_data_indices(csvl, verboseprint)
+        self._ini, self._fin = ini, fin
+        self._check_csvl_format(csvl, ini, fin, verboseprint)
+        self._wells_platemap, self._platemap = self._extract_platemap(
+            csvl[fin + 1 :], verboseprint
+        )
+        self.metadata = self._create_metadata(csvl[0 : ini - 2], csvl[fin + 1 :])
+        self.wells, self.measurements = self._extract_measurements(
+            csvl[ini - 1 : fin], csvl[fin + 1 :], verboseprint
+        )
 
-            Returns
-            -------
-            tuple[list[str], list[list[str]]]
-                A tuple containing:
-                - A list of well IDs in the format "A01", "A02", etc.
-                - A list of lists representing the Platemap.
-
-            Raises
-            ------
-            CsvLineError
-                If the column '01' is not present 3 lines below ['Platemap:'].
-
-            """
-            lines: list[list[str]] = self._metadata_post
-            idx: int = line_index(lines, ["Platemap:"])
-            if "01" not in lines[idx + 3]:
-                msg = "stop: Platemap format unexpected"
-                raise CsvLineError(msg)
-            plate: list[list[str]] = []
-            for i in range(idx + 4, len(lines)):
-                if not lines[i]:
-                    break
-                plate.append(lines[i])
-            well_list: list[str] = [
-                f"{r[0]}{c:02}" for r in plate for c in range(1, len(r)) if r[c].strip()
-            ]
-            return well_list, plate
+    def export_measurements(self, output_dir: Path = Path("Meas")) -> None:
+        """Create table as DataFrame and plot; save into Meas folder."""
+        output_dir.mkdir(parents=True, exist_ok=True)
+        for m in self.measurements:
+            data_dict = {"lambda": list(map(float, self.measurements[m]["lambda"]))}
+            data_dict.update(
+                {w: list(map(float, self.measurements[m][w])) for w in self.wells}
+            )
+            dfdata = pd.DataFrame(data=data_dict).set_index("lambda")
+            # Create plot
+            dfdata.plot(title=m, legend=False)
+            # Save files
+            file = output_dir / (self.file.stem + "_" + m + ".csv")
+            while file.exists():
+                # because with_stem was introduced in py3.9
+                file = file.with_name(file.stem + "-b" + file.suffix)
+            dfdata.to_csv(str(file))
+            plt.savefig(str(file.with_suffix(".png")))
 
-        def create_metadata() -> None:
-            """Create metadata dictionary."""
-            self.metadata: dict[str, str | list[str]] = {}
-            self.metadata[pre[1][3]] = pre[2][3]
-            self.metadata[pre[1][4]] = pre[2][4]
-            self.metadata[pre[1][5]] = pre[2][5]
-            self.metadata[pre[1][6]] = pre[2][6]
-            self.metadata[pre[1][7]] = pre[2][7]
-            self.metadata["Protocol name"] = self._metadata_post[7][4]
-            self.metadata["Exported data"] = [
-                ll[4]
-                for ll in [line for line in self._metadata_post if line[:-1]]
-                if ll[0] == "Exported data"
-            ][0]
-            self.metadata["warnings"] = [
-                line[0]
-                for line in self._metadata_post
-                if len(line) == 1 and "WARNING:" in line[0]
-            ]
+    # Helpers
+    def _read_csv_file(
+        self, file: Path, verboseprint: typing.Callable[..., typing.Any]
+    ) -> list[list[str]]:
+        """Read EnSpire exported file into csvl."""
+        csvl = list(csv.reader(file.open(encoding="iso-8859-1"), dialect="excel-tab"))
+        verboseprint("read file csv")
+        return csvl
+
+    def _find_data_indices(
+        self, csvl: list[list[str]], verboseprint: typing.Callable[..., typing.Any]
+    ) -> tuple[int, int]:
+        """Find the indices of the data blocks in the input file."""
+        inil = lookup_listoflines(csvl, pattern="Well", col=0)
+        if len(inil) == 0:
+            msg = f"No line starting with ['Well', ...] found in {csvl[:9]}"
+            raise CsvLineError(msg)
+        elif len(inil) == 1:
+            ini = 1 + inil[0]
+        else:
+            msg = f"Multiple lines starting with ['Well', ...] in {csvl[:9]}"
+            raise CsvLineError(msg)
+        verboseprint("ini =", ini)
+        fin = -1
+        fin += lookup_listoflines(csvl, pattern="Basic assay information ", col=0)[0]
+        verboseprint("fin =", fin)
+        return ini, fin
 
-        verboseprint = verbose_print(verbose)
-        csvl = list(
-            csv.reader(Path(file).open(encoding="iso-8859-1"), dialect="excel-tab")
-        )
-        verboseprint("read file csv")  # type: ignore
-        # TODO: try prparser.line_index()
-        self._ini = 1 + get_data_ini(csvl)
-        verboseprint("ini =", self._ini)  # type: ignore
-        self._fin = -1 + line_index(csvl, ["Basic assay information "])
-        verboseprint("fin =", self._fin)  # type: ignore
-        # check csv format around ini and fin
-        if not (csvl[self._ini - 3] == csvl[self._ini - 2] == []):
+    def _check_csvl_format(
+        self,
+        csvl: list[list[str]],
+        ini: int,
+        fin: int,
+        verboseprint: typing.Callable[..., typing.Any],
+    ) -> None:
+        """Check csv format around ini and fin."""
+        if not (csvl[ini - 3] == csvl[ini - 2] == []):
             msg = "Expecting two empty lines before _ini"
             raise CsvLineError(msg)
-        if csvl[self._fin] != []:
+        if csvl[fin] != []:
             msg = "Expecting an empty line after _fin"
             raise CsvLineError(msg)
-        verboseprint("checked csv format around ini and fin")  # type: ignore
-        pre = csvl[0 : self._ini - 2]  # -3
-        verboseprint("saved metadata_pre attribute")  # type: ignore
-        self._data_list = csvl[self._ini - 1 : self._fin]
-        verboseprint("saved _data_list attribute")  # type: ignore
-        self._metadata_post = csvl[self._fin + 1 :]
-        verboseprint("saved metadata_post attribute")  # type: ignore
-        self._well_list_platemap, self._platemap = get_list_from_platemap()
-        verboseprint("saved _well_list_platemap attribute")  # type: ignore
-        create_metadata()
-        self._filename = str(file)
+        verboseprint("checked csv format around ini and fin")
+
+    def _extract_platemap(
+        self, post: list[list[str]], verboseprint: typing.Callable[..., typing.Any]
+    ) -> tuple[list[str], list[list[str]]]:
+        """Extract well list and Platemap from _metadata_post.
+
+        Parameters
+        ----------
+        post: list[list[str]]
+            List of lines of metadata post containing plate map.
+        verboseprint : typing.Callable[..., typing.Any]
+            Function to print verbose information.
+
+        Returns
+        -------
+        tuple[list[str], list[list[str]]]
+            A tuple containing:
+            - A list of well IDs in the format "A01", "A02", etc.
+            - A list of lists representing the Platemap.
+
+        Raises
+        ------
+        CsvLineError
+            If the column '01' is not present 3 lines below ['Platemap:'].
+
+        """
+        idx = lookup_listoflines(post, pattern="Platemap:", col=0)[0]
+        if "01" not in post[idx + 3]:
+            msg = "stop: Platemap format unexpected"
+            raise CsvLineError(msg)
+        platemap: list[list[str]] = []
+        for i in range(idx + 4, len(post)):
+            if not post[i]:
+                break
+            platemap.append(post[i])
+        wells: list[str] = [
+            f"{r[0]}{c:02}" for r in platemap for c in range(1, len(r)) if r[c].strip()
+        ]
+        verboseprint("Created attributes _wells_platemap and _platemap.")
+        return wells, platemap
+
+    def _create_metadata(
+        self, pre: list[list[str]], post: list[list[str]]
+    ) -> dict[str, str | list[str]]:
+        """Create metadata dictionary."""
+        pre_md_start_line = 3
+        pre_md_end_line = 8
+        metadata: dict[str, str | list[str]] = {}
+        for i in range(pre_md_start_line, pre_md_end_line):
+            metadata[pre[1][i]] = pre[2][i]
+        metadata["Protocol name"] = post[7][4]
+        metadata["Exported data"] = [
+            ll[4]
+            for ll in [line for line in post if line[:-1]]
+            if ll[0] == "Exported data"
+        ][0]
+        metadata["warnings"] = [
+            line[0] for line in post if len(line) == 1 and "WARNING:" in line[0]
+        ]
+        return metadata
 
-    def extract_measurements(self, verbose: int = 0) -> None:  # noqa: PLR0915
+    def _extract_measurements(
+        self,
+        csvl_data: list[list[str]],
+        csvl_post: list[list[str]],
+        verboseprint: typing.Callable[..., typing.Any],
+    ) -> tuple[list[str], dict[str, typing.Any]]:
         """Extract the measurements dictionary.
 
-        Add 3 attributes: wells, samples, measurements (as list, list, dict)
+        For each measurement label extracts metadata, lambda and for each well the spectrum.
 
         Parameters
         ----------
-        verbose : int
-            It passes extra parameters.
+        csvl_data : list[list[str]]
+            Lines of csvl containing data.
+        csvl_post : list[list[str]]
+            Lines of csvl containing metadata after data.
+        verboseprint : typing.Callable[..., typing.Any]
+            Function to print verbose information.
+
+        Returns
+        -------
+        tuple[list[str], dict[str, typing.Any]]
+            A tuple containing a list of wells and the measurements dictionary.
 
         Raises
         ------
         CsvLineError
-            When something went wrong.
+            When an error occurs during the extraction process.
         """
-        verboseprint = verbose_print(verbose)
+        measurements = self._parse_measurements_metadata(csvl_post, verboseprint)
+        header = csvl_data[0]
+        if not self._check_header_measurements_keys(header, measurements, verboseprint):
+            msg = "check header and measurements.keys() FAILED."
+            raise CsvLineError(msg)
+        columns = [r.replace(":", "") for r in header]
+        dfdata = pd.DataFrame(csvl_data[1:], columns=columns)
+        w = dfdata.drop_duplicates(["Well"])
+        wells = w.Well.tolist()
+        if wells != self._wells_platemap:
+            msg = "well_list from data_list and platemap differ. It might be that you did not export data for all acquired wells"
+            warnings.warn(msg, stacklevel=2)
+
+        # Monochromator is expected to be either Exc or Ems
+        for k, measurement in measurements.items():
+            label = f"Meas{k}"
+            heading = namedtuple("heading", "ex em res")
+            head = heading(
+                f"{label}WavelengthExc", f"{label}WavelengthEms", f"{label}Result"
+            )
+            # excitation spectra must have only one emission wavelength
+            if measurement["metadata"]["Monochromator"] == "Excitation":
+                x = [r for r in dfdata[head.em] if r]
+                c = Counter(x)
+                if (
+                    len(c) != 1
+                    or list(c.keys())[0] != measurement["metadata"]["Wavelength"]
+                ):
+                    msg = f"Excitation spectra with unexpected emission in {label}"
+                    raise CsvLineError(msg)
+                measurement["lambda"] = [
+                    float(r) for r in dfdata[head.ex][dfdata.Well == wells[0]] if r
+                ]
+            # emission spectra must have only one excitation wavelength
+            elif measurement["metadata"]["Monochromator"] == "Emission":
+                x = [r for r in dfdata[head.ex] if r]
+                c = Counter(x)
+                if (
+                    len(c) != 1
+                    or list(c.keys())[0] != measurement["metadata"]["Wavelength"]
+                ):
+                    msg = f"Emission spectra with unexpected excitation in {label}"
+                    raise CsvLineError(msg)
+                measurement["lambda"] = [
+                    float(r) for r in dfdata[head.em][dfdata.Well == wells[0]] if r
+                ]
+            else:
+                msg = f'Unknown "Monochromator": {measurement["metadata"]["Monochromator"]} in {label}'
+                raise CsvLineError(msg)
+            for w in wells:
+                measurement[w] = [
+                    float(r) for r in dfdata[head.res][dfdata.Well == w] if r
+                ]
+        return wells, measurements
+
+    def _parse_measurements_metadata(
+        self, csvl_post: list[list[str]], verboseprint: typing.Callable[..., typing.Any]
+    ) -> dict[str, typing.Any]:
+        """Initialize measurements with metadata for each label."""
         pyparsing.ParserElement.setDefaultWhitespaceChars(" \t")
 
         def line(keyword: str) -> pyparsing.ParserElement:
             EOL = pyparsing.LineEnd().suppress()  # type: ignore # noqa: N806
             w = pyparsing.Word(pyparsing.alphanums + ".\u00B0%")  # . | deg | %
             return (
                 pyparsing.ZeroOrMore(pyparsing.White(" \t")).suppress()
                 + pyparsing.Keyword(keyword)("name")
                 + pyparsing.ZeroOrMore(pyparsing.White(" \t")).suppress()
                 + w("value")
                 + pyparsing.Optional(w)
                 + EOL
             )
 
-        meas: dict[str, Any] = {}
-        temp = [0]
-        meas_key = ["zz"]
+        measurements: dict[str, typing.Any] = {}
+        temp = [0.0]
+        meas_key = [""]
 
         def aa(tokens: pyparsing.ParseResults) -> None:
             name = tokens[0]
             value = tokens[1]
-            verboseprint(name, "=", value)  # type: ignore
+            verboseprint(name, "=", value)
             if name == "Measurement chamber temperature":
                 temp[0] = value
                 return
             if name == "Meas":
                 meas_key[0] = value
-                if value not in meas.keys():
-                    # Initialize new "Measurement"
-                    meas[meas_key[0]] = {}
-                    meas[value]["metadata"] = {}
-                    meas[value]["metadata"]["temp"] = temp[0]
+                if value not in measurements.keys():
+                    measurements[meas_key[0]] = {}
+                    measurements[value]["metadata"] = {}
+                    measurements[value]["metadata"]["temp"] = temp[0]
                 return
-            meas[meas_key[0]]["metadata"][name] = value
+            measurements[meas_key[0]]["metadata"][name] = value
 
         block_lines = (
             line("Measurement chamber temperature")
             | line("Meas")
             | line("Monochromator")
             | line("Min wavelength")
             | line("Max wavelength")
@@ -270,172 +343,106 @@
             | line("Using of excitation filter")
             | line("Measurement height")
             | line("Number of flashes integrated")
             | line("Number of flashes")
             | line("Flash power")
         )
         pr = block_lines.setParseAction(aa)
-
-        ps1 = ["\t".join(line) for line in self._metadata_post]
-        verboseprint("metadata_post ps1 conversion... done")  # type: ignore
+        ps1 = ["\t".join(line) for line in csvl_post]
         ps2 = "\n".join(ps1)
-        verboseprint("metadata_post ps2 conversion... done")  # type: ignore
         pr.searchString(ps2)
-        verboseprint("metadata_post pyparsing... done")  # type: ignore
-        self.measurements = meas
-
-        def headerdata_measurementskeys_check() -> bool:
-            """Check header and measurements.keys()."""
-            counter_constant = 3  # Not sure, maybe for md with units.
-            meas = [line.split(":")[0].replace("Meas", "") for line in headerdata]
-            b = {k for k, v in Counter(meas).items() if v == counter_constant}
-            a = set(self.measurements.keys())
-            verboseprint("check header and measurements.keys()", a == b, a, b)  # type: ignore
-            return a == b
-
-        headerdata = self._data_list[0]
-        if not headerdata_measurementskeys_check():
-            msg = "check header and measurements.keys() FAILED."
-            raise CsvLineError(msg)
-
-        def check_lists() -> bool:
-            """Check that lists derived from .csv data and Platemap metadata are identical.
-
-            if not raises an *Exception*.
-            Will Raise *Exception* if well_list from csv (data_list) and note
-            disagree. Raise *Warning* if well_list from csv (data_list) and
-            platemap disagree.
-
-            Returns
-            -------
-            bool
-                Ckeck correctness.
-
-            """
-            if self.wells != self._well_list_platemap:
-                warnings.warn(
-                    "well_list from data_list and platemap differ. It might be you did not exported data for all acquired wells",
-                    stacklevel=2,
-                )
-            return True
-
-        columns = [r.replace(":", "") for r in headerdata]
-        dfdata = pd.DataFrame(self._data_list[1:], columns=columns)
-        w = dfdata.drop_duplicates(["Well"])
-        self.wells = w.Well.tolist()
-        check_lists()
-        # Monochromator is expected to be either Exc or Ems
-        for k, v in self.measurements.items():
-            label = f"Meas{k}"
-            heading = namedtuple("heading", "ex em res")
-            head = heading(
-                f"{label}WavelengthExc", f"{label}WavelengthEms", f"{label}Result"
-            )
-            # excitation spectra must have only one emission wavelength
-            if v["metadata"]["Monochromator"] == "Excitation":
-                x = [r for r in dfdata[head.em] if r]
-                c = Counter(x)
-                if len(c) != 1 or list(c.keys())[0] != v["metadata"]["Wavelength"]:
-                    msg = f"Excitation spectra with unexpected emission in {label}"
-                    raise CsvLineError(msg)
-                v["lambda"] = [
-                    float(r) for r in dfdata[head.ex][dfdata.Well == self.wells[0]] if r
-                ]
-            # emission spectra must have only one excitation wavelength
-            elif v["metadata"]["Monochromator"] == "Emission":
-                x = [r for r in dfdata[head.ex] if r]
-                c = Counter(x)
-                if len(c) != 1 or list(c.keys())[0] != v["metadata"]["Wavelength"]:
-                    msg = f"Emission spectra with unexpected excitation in {label}"
-                    raise CsvLineError(msg)
-                v["lambda"] = [
-                    float(r) for r in dfdata[head.em][dfdata.Well == self.wells[0]] if r
-                ]
-            else:
-                msg = f'Unknown "Monochromator": {v["metadata"]["Monochromator"]} in {label}'
-                raise CsvLineError(msg)
-            for w in self.wells:
-                v[w] = [float(r) for r in dfdata[head.res][dfdata.Well == w] if r]
+        return measurements
 
-    def export_measurements(self, output_dir: Path = Path("Meas")) -> None:
-        """Create table as DataFrame and plot; save into Meas folder."""
-        output_dir.mkdir(parents=True, exist_ok=True)
-        for m in self.measurements:
-            data_dict = {"lambda": list(map(float, self.measurements[m]["lambda"]))}
-            data_dict.update(
-                {w: list(map(float, self.measurements[m][w])) for w in self.wells}
-            )
-            dfdata = pd.DataFrame(data=data_dict).set_index("lambda")
-            # Create plot
-            dfdata.plot(title=m, legend=False)
-            # Save files
-            file = output_dir / (Path(self._filename).stem + "_" + m + ".csv")
-            while file.exists():
-                # because with_stem was introduced in py3.9
-                file = file.with_name(file.stem + "-b" + file.suffix)
-            dfdata.to_csv(str(file))
-            plt.savefig(str(file.with_suffix(".png")))
+    def _check_header_measurements_keys(
+        self,
+        headerdata: list[str],
+        measurements: dict[str, typing.Any],
+        verboseprint: typing.Callable[..., typing.Any],
+    ) -> bool:
+        """Check header and measurements.keys()."""
+        counter_constant = 3  # Not sure, maybe for md with units. <Exc, Ems, F>
+        meas = [line.split(":")[0].replace("Meas", "") for line in headerdata]
+        b = {k for k, v in Counter(meas).items() if v == counter_constant}
+        a = set(measurements.keys())
+        verboseprint("check header and measurements.keys()", a == b, a, b)
+        return a == b
 
 
 @dataclass
 class ExpNote:
-    """Read an Experimental Note file.
+    """Read and processes an Experimental Note file.
+
+    This class is responsible for handling Experimental Note files
+    that describe an EnSpire experiment collecting spectrum. It reads the files and
+    stores the extracted information as a list of lines: note_list and list of wells.
 
-    For describing an EnSpire experiment collecting spectrum. Store info as list
-    of lines: note_list and well_list.
+    Parameters
+    ----------
+    note_file : Path
+        The path to the Experimental Note file to be processed.
+    verbose : int
+        Level of verbosity; 0 is silent, higher values are more verbose (default=0).
 
     Example
     -------
     >>> from clophfit.prenspire import ExpNote
     >>> en = ExpNote("tests/EnSpire/h148g-spettroC-nota")
     >>> en.wells[2]
     'A03'
     """
 
     note_file: Path
     verbose: int = 0
+    #: A list of wells generated from the note file.
+    wells: list[str] = field(init=False, default_factory=list)
+    # A list of lines extracted from the note file.
+    _note_list: list[list[str]] = field(init=False, default_factory=list)
+    #: A list of titrations extracted from the note file.
+    titrations: list[Titration] = field(init=False, default_factory=list)
 
     def __post_init__(self) -> None:
-        """Complete the initialization."""
+        """Complete the initialization generating wells and _note_list."""
         verboseprint = verbose_print(self.verbose)
         with Path(self.note_file).open(encoding="iso-8859-1") as f:
             # Differ from pandas because all fields/cells are strings.
-            self.note_list = list(csv.reader(f, dialect="excel-tab"))
-        verboseprint("read (experimental) note file")  # type: ignore
-        self.wells: list[str] = np.array(self.note_list)[1:, 0].tolist()
-        verboseprint("wells generated")  # type: ignore
-
-    def check_wells(self, ef: EnspireFile) -> bool:
-        """Is (EnspireFile) ef.wells == ExpNote.wells? Return False-or-True."""
-        return self.wells == ef.wells
+            self._note_list = list(csv.reader(f, dialect="excel-tab"))
+        if callable(verboseprint):
+            verboseprint("Read (experimental) note file")
+        self.wells: list[str] = np.array(self._note_list)[1:, 0].tolist()
+        if callable(verboseprint):
+            verboseprint("Wells generated")
 
     def build_titrations(self, ef: EnspireFile) -> None:
         """Extract titrations from the given ef (_note file like: <well, pH, Cl>)."""
         # 1 pH titration
-        conc_well = [(line[1], line[0]) for line in self.note_list if line[2] == "0"]
+        conc_well = [(line[1], line[0]) for line in self._note_list if line[2] == "0"]
         conc = [float(tpl[0]) for tpl in conc_well]
         well = [tpl[1] for tpl in conc_well]
         data = {}
         for m, measurement in ef.measurements.items():
             data[m] = pd.DataFrame(
                 data=np.transpose([list(map(float, measurement[w])) for w in well]),
                 columns=[conc, well],
                 index=pd.Index(
                     data=list(map(float, measurement["lambda"])), name="lambda"
                 ),
             )
         self.titrations = [Titration(conc, data, cl="0")]
         # n cl titrations
         self.pH_values = sorted(
-            {line[1] for line in self.note_list if line[2].replace(".", "").isnumeric()}
+            {
+                line[1]
+                for line in self._note_list
+                if line[2].replace(".", "").isnumeric()
+            }
         )
         for ph in self.pH_values:
             conc_well = [
                 (line[2], line[0])
-                for line in self.note_list
+                for line in self._note_list
                 if line[1] == ph and line[2].replace(".", "").isnumeric()
             ]
             conc = [float(tpl[0]) for tpl in conc_well]
             well = [tpl[1] for tpl in conc_well]
             data = {}
             for m, measurement in ef.measurements.items():
                 data[m] = pd.DataFrame(
@@ -444,23 +451,23 @@
                     index=pd.Index(
                         data=list(map(float, measurement["lambda"])),
                         name="lambda",
                     ),
                 )
             self.titrations.append(Titration(conc, data, ph=ph))
 
-    # TODO: BUFFER
+        # TODO: BUFFER
 
 
 class Titration:
     """Store titration data and fit results."""
 
     def __init__(
         self,
-        conc: Sequence[float],
+        conc: typing.Sequence[float],
         data: dict[str, pd.DataFrame],
         cl: str | None = None,
         ph: str | None = None,
     ) -> None:
         self.conc = conc
         self.data = data
         if ph:
```

### Comparing `clophfit-0.7.0/src/clophfit/prtecan/__init__.py` & `clophfit-0.7.1/src/clophfit/prtecan/__init__.py`

 * *Files identical despite different names*

### Comparing `clophfit-0.7.0/src/clophfit/prtecan/prtecan.py` & `clophfit-0.7.1/src/clophfit/prtecan/prtecan.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 """prtecan/prtecan.py."""
 from __future__ import annotations
 
 import hashlib
 import itertools
+import typing
 import warnings
 from contextlib import suppress
 from dataclasses import InitVar
 from dataclasses import dataclass
 from dataclasses import field
 from pathlib import Path
-from typing import Callable
-from typing import ClassVar
 from typing import Sequence
 
 import matplotlib.pyplot as plt  # type: ignore
 import numpy as np
 import pandas as pd
 import seaborn as sb  # type: ignore  # noqa: ICN001
 from matplotlib.backends.backend_pdf import PdfPages  # type: ignore
@@ -53,17 +52,31 @@
     sheet = pd.read_excel(path)
     n0 = pd.DataFrame([[np.nan] * len(sheet.columns)], columns=sheet.columns)
     sheet = pd.concat([n0, sheet], ignore_index=True)
     sheet = sheet.fillna("")
     return list(sheet.to_numpy().tolist())
 
 
+@typing.overload
+def lookup_listoflines(csvl: list[list[str]], pattern: str, col: int) -> list[int]:
+    ...
+
+
+@typing.overload
 def lookup_listoflines(
     csvl: list[list[str | int | float]], pattern: str = "Label: Label", col: int = 0
 ) -> list[int]:
+    ...
+
+
+def lookup_listoflines(
+    csvl: list[list[str | int | float]] | list[list[str]],
+    pattern: str = "Label: Label",
+    col: int = 0,
+) -> list[int]:
     """Lookup line numbers (row index) where given pattern occurs.
 
     Parameters
     ----------
     csvl : list_of_lines
         Lines of a csv/xls file.
     pattern : str
@@ -75,19 +88,18 @@
     -------
     list[int]
         Row/line index for all occurrences of pattern. Empty list for no occurrences.
 
     """
     indexes = []
     for i, line in enumerate(csvl):
-        try:
-            if isinstance(line[col], str) and pattern in str(line[col]):
+        if isinstance(line, list) and col < len(line):
+            element = line[col]
+            if isinstance(element, (str, int, float)) and pattern in str(element):
                 indexes.append(i)
-        except IndexError:
-            continue
     return indexes
 
 
 def strip_lines(lines: list[list[str | int | float]]) -> list[list[str | int | float]]:
     """Remove empty fields/cells from lines read from a csv file.
 
     Parameters
@@ -305,27 +317,31 @@
 
     _lines: InitVar[list[list[str | int | float]]]
     path: Path | None = None
     #: Metadata specific for this Labelblock.
     metadata: dict[str, Metadata] = field(init=False, repr=True)
     #: The 96 data values as {'well_name', value}.
     data: dict[str, float] = field(init=False, repr=True)
-    _KEYS: ClassVar[list[str]] = [
+    _KEYS: typing.ClassVar[list[str]] = [
         "Emission Bandwidth",
         "Emission Wavelength",
         "Excitation Bandwidth",
         "Excitation Wavelength",
         "Mode",
         "Integration Time",
         "Number of Flashes",
     ]
-    _NORM_KEYS: ClassVar[list[str]] = ["Integration Time", "Number of Flashes", "Gain"]
+    _NORM_KEYS: typing.ClassVar[list[str]] = [
+        "Integration Time",
+        "Number of Flashes",
+        "Gain",
+    ]
 
     def __post_init__(self, lines: list[list[str | int | float]]) -> None:
-        """Generate metadata and data for this labelblock."""
+        """Create metadata and data; initialize labelblock's properties."""
         self._buffer_wells: list[str] | None = None
         self._buffer: float | None = None
         self._buffer_norm: float | None = None
         self._buffer_sd: float | None = None
         self._buffer_norm_sd: float | None = None
         self._data_norm: dict[str, float] | None = None
         self._data_buffersubtracted: dict[str, float] | None = None
@@ -1014,15 +1030,15 @@
     ValueError
         For unexpected file format, e.g. header `names`.
     """
 
     #: List of result dataframes.
     fittings: list[pd.DataFrame] = field(init=False, default_factory=list)
     #: Function used in the fitting.
-    fz: Callable[
+    fz: typing.Callable[
         [float, NDArray[np.float_] | Sequence[float], NDArray[np.float_]],
         NDArray[np.float_],
     ] = field(init=False)
     #: A list of wells containing samples that are neither buffer nor CTR samples.
     keys_unk: list[str] = field(init=False, default_factory=list)
 
     def __post_init__(self) -> None:
```

### Comparing `clophfit-0.7.0/tests/test_binding.py` & `clophfit-0.7.1/tests/test_binding.py`

 * *Files identical despite different names*

### Comparing `clophfit-0.7.0/tests/test_cli.py` & `clophfit-0.7.1/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `clophfit-0.7.0/tests/test_oldscripts.py` & `clophfit-0.7.1/tests/test_oldscripts.py`

 * *Files identical despite different names*

### Comparing `clophfit-0.7.0/tests/test_prenspire.py` & `clophfit-0.7.1/tests/test_prenspire.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,23 +13,21 @@
 esff = data_files_dir.joinpath
 
 
 @pytest.fixture(scope="module")
 def ef1() -> EnspireFile:
     """Read in file."""
     ef = EnspireFile(esff("h148g-spettroC.csv"))
-    ef.extract_measurements()
     return ef
 
 
 @pytest.fixture(scope="module")
 def ef2() -> EnspireFile:
     """Read in file without 'Samples' column."""
     ef = EnspireFile(esff("e2-T-without_sample_column.csv"))
-    ef.extract_measurements()
     return ef
 
 
 class TestEnspireFile:
     """Test EnspireFile class."""
 
     def test_exceptions(self) -> None:
@@ -48,64 +46,66 @@
             EnspireFile(esf("M1-A6-G12_missing_emptyline_ini.csv"))
         with pytest.raises(Exception, match="Expecting an empty line after _fin"):
             EnspireFile(esf("M1-A6-G12_missing_emptyline_fin.csv"))
         # Test multiple emission wavelengths in excitation spectra
         with pytest.raises(
             Exception, match="Excitation spectra with unexpected emission in MeasA"
         ):
-            EnspireFile(esf("e2dan-exwavelength.csv")).extract_measurements()
+            EnspireFile(esf("e2dan-exwavelength.csv"))
         with pytest.raises(
             Exception, match="Excitation spectra with unexpected emission in MeasA"
         ):
-            EnspireFile(esf("e2dan-exwavelength2.csv")).extract_measurements()
+            EnspireFile(esf("e2dan-exwavelength2.csv"))
         with pytest.raises(
             Exception, match="Emission spectra with unexpected excitation in MeasC"
         ):
-            EnspireFile(esf("e2dan-emwavelength.csv")).extract_measurements()
+            EnspireFile(esf("e2dan-emwavelength.csv"))
         with pytest.raises(
             Exception, match='Unknown "Monochromator": Strange in MeasB'
         ):
-            EnspireFile(esf("e2dan-exwavelengthstrange.csv")).extract_measurements()
+            EnspireFile(esf("e2dan-exwavelengthstrange.csv"))
 
     def test_get_data_ini(self, ef1: EnspireFile, ef2: EnspireFile) -> None:
         """Test get_data_ini."""
         assert ef1._ini == 12
         assert ef2._ini == 9
 
     def test_fin(self, ef1: EnspireFile, ef2: EnspireFile) -> None:
         """Test _fin (line_index())."""
         assert ef1._fin == 14897
         assert ef2._fin == 856
 
-    def test_metadata_post(self, ef1: EnspireFile, ef2: EnspireFile) -> None:
-        """Identify correctly the beginning of metadata after data block."""
-        assert ef1._metadata_post[0] == ["Basic assay information "]
-        assert ef2._metadata_post[0] == ["Basic assay information "]
-
-    def test_localegen_in_metadata_post(
-        self, ef1: EnspireFile, ef2: EnspireFile
-    ) -> None:
-        """Test locales."""
-        assert ef1._metadata_post[31][4] == "300 µl"
-        assert ef2._metadata_post[31][4] == "300 µl"
-
-    def test_data_list(self, ef1: EnspireFile, ef2: EnspireFile) -> None:
-        """Test data_list."""
-        assert ef1._data_list[0][2] == "MeasA:Result"
-        assert ef2._data_list[0][2] == "MeasB:WavelengthEms"
-        assert ef1._data_list[1][2] == "3151"
-        assert ef2._data_list[1][3] == "3739"
-        # Important to check for last line
-        assert ef1._data_list[-1][2] == "97612"
-        assert ef2._data_list[-1][3] == "512"
+    """
+    # def test_metadata_post(self, ef1: EnspireFile, ef2: EnspireFile) -> None:
+    #     \"Identify correctly the beginning of metadata after data block.\"
+    #     assert ef1._metadata_post[0] == ["Basic assay information "]
+    #     assert ef2._metadata_post[0] == ["Basic assay information "]
+
+    # def test_localegen_in_metadata_post(
+    #     self, ef1: EnspireFile, ef2: EnspireFile
+    # ) -> None:
+    #     \"Test locales.\"
+    #     assert ef1._metadata_post[31][4] == "300 µl"
+    #     assert ef2._metadata_post[31][4] == "300 µl"
+
+    # def test_data_list(self, ef1: EnspireFile, ef2: EnspireFile) -> None:
+    #     \"Test data_list.\"
+    #     assert ef1._data_list[0][2] == "MeasA:Result"
+    #     assert ef2._data_list[0][2] == "MeasB:WavelengthEms"
+    #     assert ef1._data_list[1][2] == "3151"
+    #     assert ef2._data_list[1][3] == "3739"
+    #     # Important to check for last line
+    #     assert ef1._data_list[-1][2] == "97612"
+    #     assert ef2._data_list[-1][3] == "512"
+    """
 
     def test_get_list_from_platemap(self, ef1: EnspireFile, ef2: EnspireFile) -> None:
         """Test list from platemap."""
-        assert ef1._well_list_platemap[2] == "A03"
-        assert ef2._well_list_platemap[1] == "F02"
+        assert ef1._wells_platemap[2] == "A03"
+        assert ef2._wells_platemap[1] == "F02"
 
     def test_metadata(self, ef1: EnspireFile) -> None:
         """Test metadata dictionary."""
         assert ef1.metadata["Measurement date"] == "2011-10-03 17:12:33"
         assert ef1.metadata["Chamber temperature at start"] == "20"
         assert ef1.metadata["Chamber temperature at end"] == "20"
         assert ef1.metadata["Ambient temperature at start"] == "6"
@@ -149,16 +149,15 @@
 
         """
         esf = (data_files_dir / "warnings").joinpath
 
         with warnings.catch_warnings(record=True) as w:
             # Cause all warnings to always be triggered.
             warnings.simplefilter("always")
-            ef = EnspireFile(esf("h148g-spettroC-incomplete.csv"))
-            ef.extract_measurements()
+            EnspireFile(esf("h148g-spettroC-incomplete.csv"))
             assert len(w) == 2
             assert issubclass(w[-1].category, Warning)
             assert "platemap" in str(w[-1].message)
 
     # placemark def test_get_maxx(self):
     # placemark    "really need to be completed"
     # placemark    self.assertEqual(self.s.get_maxx(self.s.ex, self.s.y), 272)
@@ -179,23 +178,23 @@
 class TestExpNote:
     """Experimental notes."""
 
     def test_get_list_from_note(self, en1: ExpNote) -> None:
         """Test get_well_list_from_note method."""
         assert en1.wells[2] == "A03"
 
-    def test_note_list(self, en1: ExpNote) -> None:
+    def test__note_list(self, en1: ExpNote) -> None:
         """Test well_list from note."""
-        assert en1.note_list[3][0] == "A03"
-        assert en1.note_list[65][1] == "8.2"
+        assert en1._note_list[3][0] == "A03"
+        assert en1._note_list[65][1] == "8.2"
 
-    def test_check_list(self, en1: ExpNote, ef1: EnspireFile, en1err: ExpNote) -> None:
-        """Test check list from note vs. Enspirefile."""
-        assert en1.check_wells(ef1) is True
-        assert en1err.check_wells(ef1) is False
+    def test_wells(self, en1: ExpNote, ef1: EnspireFile, en1err: ExpNote) -> None:
+        """Check wells from ExpNote vs. EnspireFile."""
+        assert en1.wells == ef1.wells
+        assert (en1err.wells == ef1.wells) is False
 
     def test_build_titrations(self, en1: ExpNote, ef1: EnspireFile) -> None:
         """Test the method extract_titrations()."""
         en1.build_titrations(ef1)
         assert len(en1.titrations) == 6
         tit0 = en1.titrations[0]
         assert tit0.conc == [5.2, 6.3, 7.4, 8.1, 8.2]
```

### Comparing `clophfit-0.7.0/tests/test_prtecan.py` & `clophfit-0.7.1/tests/test_prtecan.py`

 * *Files 3% similar despite different names*

```diff
@@ -163,31 +163,34 @@
         assert lb1.data_buffersubtracted_norm["H12"] == pytest.approx(43.4152)
         # Can also assign a buffer_norm value.
         lb0.buffer_norm = 1
         lb1.buffer_norm = 0.4821
         assert lb0.data_buffersubtracted_norm["F06"] == pytest.approx(1050.13)
         assert lb1.data_buffersubtracted_norm["H12"] == pytest.approx(48.0)
 
-    def test___eq__(self, labelblocks: tuple[Labelblock, Labelblock]) -> None:
-        """It is equal to itself. TODO and different from other."""
+    def test_eq(self, labelblocks: tuple[Labelblock, Labelblock]) -> None:
+        """Check if a Labelblock is equal to itself and not equal to a different Labelblock."""
         lb0, lb1 = labelblocks
-        tmp = lb0
-        assert lb0 == tmp
-        assert lb0 != lb1
-        assert lb0.__eq__(1) == NotImplemented
+        assert lb0 == lb0, "Labelblock is not equal to itself"
+        assert lb0 != lb1, "Different Labelblocks are incorrectly reported as equal"
+        assert (
+            lb0.__eq__(1) == NotImplemented
+        ), "Equality check against non-Labelblock object did not return NotImplemented"
 
-    def test___almost_eq__(self, labelblocks: tuple[Labelblock, Labelblock]) -> None:
-        """It is equal to itself. TODO and different from other."""
+    def test_almost_eq(self, labelblocks: tuple[Labelblock, Labelblock]) -> None:
+        """Test the __almost_eq__ method of the Labelblock class."""
         lb0, _ = labelblocks
-        csvl = prtecan.read_xls(data_tests / "290513_7.2.xls")  # Gain=98
-        idxs = prtecan.lookup_listoflines(csvl)
-        lb11 = Labelblock(csvl[idxs[1] :])
-        csvl = prtecan.read_xls(data_tests / "290513_8.8.xls")  # Gain=99
-        idxs = prtecan.lookup_listoflines(csvl)
-        lb12 = Labelblock(csvl[idxs[1] :])
+        file_path1 = Path(data_tests) / "290513_7.2.xls"
+        csvl1 = prtecan.read_xls(file_path1)  # Gain=98
+        idxs1 = prtecan.lookup_listoflines(csvl1)
+        lb11 = Labelblock(csvl1[idxs1[1] :])
+        file_path2 = Path(data_tests) / "290513_8.8.xls"
+        csvl2 = prtecan.read_xls(file_path2)  # Gain=99
+        idxs2 = prtecan.lookup_listoflines(csvl2)
+        lb12 = Labelblock(csvl2[idxs2[1] :])
         assert lb11 != lb12
         assert lb11.__almost_eq__(lb12)
         assert not lb11.__almost_eq__(lb0)
 
     def test_overvalue(self) -> None:
         """It detects saturated data ("OVER")."""
         csvl = prtecan.read_xls(data_tests / "140220/pH6.5_200214.xls")
@@ -246,19 +249,20 @@
     def test_labelblocks(self) -> None:
         """It parses "Temperature" metadata and cell data from 2 labelblocks."""
         assert self.tf.labelblocks[0].metadata["Temperature"].value == 25.3
         assert self.tf.labelblocks[1].metadata["Temperature"].value == 25.7
         assert self.tf.labelblocks[0].data["A01"] == 17260
         assert self.tf.labelblocks[1].data["H12"] == 4196
 
-    def test___eq__(self) -> None:
-        """It is equal to itself. TODO and different from other."""
-        assert self.tf == prtecan.Tecanfile(data_tests / "140220/pH8.3_200214.xls")
+    def test_eq(self) -> None:
+        """Check if a Tecanfile is equal to itself and not equal to a different Tecanfile."""
+        tf1 = prtecan.Tecanfile(data_tests / "140220/pH8.3_200214.xls")
+        assert self.tf == tf1, "Tecanfile is not equal to itself"
         tf2 = prtecan.Tecanfile(data_tests / "140220/pH9.1_200214.xls")
-        assert tf2 != self.tf
+        assert self.tf != tf2, "Different Tecanfiles are incorrectly reported as equal"
 
     def test_warn(self) -> None:
         """It warns when labelblocks are repeated in a Tf as it might compromise grouping."""
         with pytest.warns(UserWarning, match="Repeated labelblocks"):
             prtecan.Tecanfile(data_tests / "exceptions/290212_7.67_repeated_lb.xls")
 
     def test_filenotfound(self) -> None:
```

### Comparing `clophfit-0.7.0/tests/EnSpire/24well_clop0_95.csv` & `clophfit-0.7.1/tests/EnSpire/24well_clop0_95.csv`

 * *Files identical despite different names*

### Comparing `clophfit-0.7.0/tests/EnSpire/e2-T-without_sample_column.csv` & `clophfit-0.7.1/tests/EnSpire/e2-T-without_sample_column.csv`

 * *Files identical despite different names*

### Comparing `clophfit-0.7.0/tests/EnSpire/h148g-spettroC-nota` & `clophfit-0.7.1/tests/EnSpire/h148g-spettroC-nota`

 * *Files identical despite different names*

### Comparing `clophfit-0.7.0/tests/EnSpire/h148g-spettroC-nota-Err` & `clophfit-0.7.1/tests/EnSpire/h148g-spettroC-nota-Err`

 * *Files identical despite different names*

### Comparing `clophfit-0.7.0/tests/EnSpire/h148g-spettroC.csv` & `clophfit-0.7.1/tests/EnSpire/h148g-spettroC.csv`

 * *Files identical despite different names*

### Comparing `clophfit-0.7.0/tests/EnSpire/cli/NTT_37C_pKa.csv` & `clophfit-0.7.1/tests/EnSpire/cli/NTT_37C_pKa.csv`

 * *Files identical despite different names*

### Comparing `clophfit-0.7.0/tests/EnSpire/cli/output/NTT_37C_pKa_A.csv` & `clophfit-0.7.1/tests/EnSpire/cli/output/NTT_37C_pKa_A.csv`

 * *Files identical despite different names*

### Comparing `clophfit-0.7.0/tests/EnSpire/cli/output/NTT_37C_pKa_A.png` & `clophfit-0.7.1/tests/EnSpire/cli/output/NTT_37C_pKa_A.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.7.0/tests/EnSpire/cli/output/NTT_37C_pKa_B.csv` & `clophfit-0.7.1/tests/EnSpire/cli/output/NTT_37C_pKa_B.csv`

 * *Files identical despite different names*

### Comparing `clophfit-0.7.0/tests/EnSpire/cli/output/NTT_37C_pKa_B.png` & `clophfit-0.7.1/tests/EnSpire/cli/output/NTT_37C_pKa_B.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.7.0/tests/EnSpire/exceptions/M1-A6-G12_11columns.csv` & `clophfit-0.7.1/tests/EnSpire/exceptions/M1-A6-G12_11columns.csv`

 * *Files identical despite different names*

### Comparing `clophfit-0.7.0/tests/EnSpire/exceptions/M1-A6-G12_missing_emptyline_fin.csv` & `clophfit-0.7.1/tests/EnSpire/exceptions/M1-A6-G12_missing_emptyline_fin.csv`

 * *Files identical despite different names*

### Comparing `clophfit-0.7.0/tests/EnSpire/exceptions/M1-A6-G12_missing_emptyline_ini.csv` & `clophfit-0.7.1/tests/EnSpire/exceptions/M1-A6-G12_missing_emptyline_ini.csv`

 * *Files identical despite different names*

### Comparing `clophfit-0.7.0/tests/EnSpire/exceptions/e2dan-emwavelength.csv` & `clophfit-0.7.1/tests/EnSpire/exceptions/e2dan-emwavelength.csv`

 * *Files identical despite different names*

### Comparing `clophfit-0.7.0/tests/EnSpire/exceptions/e2dan-exwavelength.csv` & `clophfit-0.7.1/tests/EnSpire/exceptions/e2dan-exwavelength.csv`

 * *Files identical despite different names*

### Comparing `clophfit-0.7.0/tests/EnSpire/exceptions/e2dan-exwavelength2.csv` & `clophfit-0.7.1/tests/EnSpire/exceptions/e2dan-exwavelength2.csv`

 * *Files identical despite different names*

### Comparing `clophfit-0.7.0/tests/EnSpire/exceptions/e2dan-exwavelengthstrange.csv` & `clophfit-0.7.1/tests/EnSpire/exceptions/e2dan-exwavelengthstrange.csv`

 * *Files identical despite different names*

### Comparing `clophfit-0.7.0/tests/EnSpire/exceptions/h148g-spettroC-idx0.csv` & `clophfit-0.7.1/tests/EnSpire/exceptions/h148g-spettroC-idx0.csv`

 * *Files identical despite different names*

### Comparing `clophfit-0.7.0/tests/EnSpire/exceptions/h148g-spettroC-idx2.csv` & `clophfit-0.7.1/tests/EnSpire/exceptions/h148g-spettroC-idx2.csv`

 * *Files identical despite different names*

### Comparing `clophfit-0.7.0/tests/EnSpire/warnings/h148g-spettroC-incomplete.csv` & `clophfit-0.7.1/tests/EnSpire/warnings/h148g-spettroC-incomplete.csv`

 * *Files identical despite different names*

### Comparing `clophfit-0.7.0/tests/Tecan/290212_100.xls` & `clophfit-0.7.1/tests/Tecan/290212_100.xls`

 * *Files identical despite different names*

### Comparing `clophfit-0.7.0/tests/Tecan/290212_150.xls` & `clophfit-0.7.1/tests/Tecan/290212_150.xls`

 * *Files identical despite different names*

### Comparing `clophfit-0.7.0/tests/Tecan/290212_20.xls` & `clophfit-0.7.1/tests/Tecan/290212_20.xls`

 * *Files identical despite different names*

### Comparing `clophfit-0.7.0/tests/Tecan/290212_5.78.xls` & `clophfit-0.7.1/tests/Tecan/290212_5.78.xls`

 * *Files identical despite different names*

### Comparing `clophfit-0.7.0/tests/Tecan/290212_50.xls` & `clophfit-0.7.1/tests/Tecan/290212_50.xls`

 * *Files identical despite different names*

### Comparing `clophfit-0.7.0/tests/Tecan/290212_6.38.xls` & `clophfit-0.7.1/tests/Tecan/290212_6.38.xls`

 * *Files identical despite different names*

### Comparing `clophfit-0.7.0/tests/Tecan/290212_6.83.xls` & `clophfit-0.7.1/tests/Tecan/290212_6.83.xls`

 * *Files identical despite different names*

### Comparing `clophfit-0.7.0/tests/Tecan/290212_7.24.xls` & `clophfit-0.7.1/tests/Tecan/290212_7.24.xls`

 * *Files identical despite different names*

### Comparing `clophfit-0.7.0/tests/Tecan/290212_7.67.xls` & `clophfit-0.7.1/tests/Tecan/290212_7.67.xls`

 * *Files identical despite different names*

### Comparing `clophfit-0.7.0/tests/Tecan/290212_8.23.xls` & `clophfit-0.7.1/tests/Tecan/290212_8.23.xls`

 * *Files identical despite different names*

### Comparing `clophfit-0.7.0/tests/Tecan/290212_8.82.xls` & `clophfit-0.7.1/tests/Tecan/290212_8.82.xls`

 * *Files identical despite different names*

### Comparing `clophfit-0.7.0/tests/Tecan/290212_9.31.xls` & `clophfit-0.7.1/tests/Tecan/290212_9.31.xls`

 * *Files identical despite different names*

### Comparing `clophfit-0.7.0/tests/Tecan/290513_5.5.xls` & `clophfit-0.7.1/tests/Tecan/290513_5.5.xls`

 * *Files identical despite different names*

### Comparing `clophfit-0.7.0/tests/Tecan/290513_5.5_bad.xls` & `clophfit-0.7.1/tests/Tecan/290513_5.5_bad.xls`

 * *Files identical despite different names*

### Comparing `clophfit-0.7.0/tests/Tecan/290513_7.2.xls` & `clophfit-0.7.1/tests/Tecan/290513_7.2.xls`

 * *Files identical despite different names*

### Comparing `clophfit-0.7.0/tests/Tecan/290513_8.8.xls` & `clophfit-0.7.1/tests/Tecan/290513_8.8.xls`

 * *Files identical despite different names*

### Comparing `clophfit-0.7.0/tests/Tecan/140220/200214 pH data.ods` & `clophfit-0.7.1/tests/Tecan/140220/200214 pH data.ods`

 * *Files identical despite different names*

### Comparing `clophfit-0.7.0/tests/Tecan/140220/NaCl1_200214.xls` & `clophfit-0.7.1/tests/Tecan/140220/NaCl1_200214.xls`

 * *Files identical despite different names*

### Comparing `clophfit-0.7.0/tests/Tecan/140220/NaCl2_200214.xls` & `clophfit-0.7.1/tests/Tecan/140220/NaCl2_200214.xls`

 * *Files identical despite different names*

### Comparing `clophfit-0.7.0/tests/Tecan/140220/NaCl3_200214.xls` & `clophfit-0.7.1/tests/Tecan/140220/NaCl3_200214.xls`

 * *Files identical despite different names*

### Comparing `clophfit-0.7.0/tests/Tecan/140220/NaCl4_200214.xls` & `clophfit-0.7.1/tests/Tecan/140220/NaCl4_200214.xls`

 * *Files identical despite different names*

### Comparing `clophfit-0.7.0/tests/Tecan/140220/NaCl5_200214.xls` & `clophfit-0.7.1/tests/Tecan/140220/NaCl5_200214.xls`

 * *Files identical despite different names*

### Comparing `clophfit-0.7.0/tests/Tecan/140220/NaCl6_200214.xls` & `clophfit-0.7.1/tests/Tecan/140220/NaCl6_200214.xls`

 * *Files identical despite different names*

### Comparing `clophfit-0.7.0/tests/Tecan/140220/NaCl7_200214.xls` & `clophfit-0.7.1/tests/Tecan/140220/NaCl7_200214.xls`

 * *Files identical despite different names*

### Comparing `clophfit-0.7.0/tests/Tecan/140220/NaCl8_200214.xls` & `clophfit-0.7.1/tests/Tecan/140220/NaCl8_200214.xls`

 * *Files identical despite different names*

### Comparing `clophfit-0.7.0/tests/Tecan/140220/fit0-1.csv` & `clophfit-0.7.1/tests/Tecan/140220/fit0-1.csv`

 * *Files identical despite different names*

### Comparing `clophfit-0.7.0/tests/Tecan/140220/fit0.csv` & `clophfit-0.7.1/tests/Tecan/140220/fit0.csv`

 * *Files identical despite different names*

### Comparing `clophfit-0.7.0/tests/Tecan/140220/fit1-1.csv` & `clophfit-0.7.1/tests/Tecan/140220/fit1-1.csv`

 * *Files identical despite different names*

### Comparing `clophfit-0.7.0/tests/Tecan/140220/fit1.csv` & `clophfit-0.7.1/tests/Tecan/140220/fit1.csv`

 * *Files identical despite different names*

### Comparing `clophfit-0.7.0/tests/Tecan/140220/pH5.0_200214.xls` & `clophfit-0.7.1/tests/Tecan/140220/pH5.0_200214.xls`

 * *Files identical despite different names*

### Comparing `clophfit-0.7.0/tests/Tecan/140220/pH5.8_200214.xls` & `clophfit-0.7.1/tests/Tecan/140220/pH5.8_200214.xls`

 * *Files identical despite different names*

### Comparing `clophfit-0.7.0/tests/Tecan/140220/pH6.5_200214.xls` & `clophfit-0.7.1/tests/Tecan/140220/pH6.5_200214.xls`

 * *Files identical despite different names*

### Comparing `clophfit-0.7.0/tests/Tecan/140220/pH7.1_200214.xls` & `clophfit-0.7.1/tests/Tecan/140220/pH7.1_200214.xls`

 * *Files identical despite different names*

### Comparing `clophfit-0.7.0/tests/Tecan/140220/pH7.6_200214.xls` & `clophfit-0.7.1/tests/Tecan/140220/pH7.6_200214.xls`

 * *Files identical despite different names*

### Comparing `clophfit-0.7.0/tests/Tecan/140220/pH8.3_200214.xls` & `clophfit-0.7.1/tests/Tecan/140220/pH8.3_200214.xls`

 * *Files identical despite different names*

### Comparing `clophfit-0.7.0/tests/Tecan/140220/pH9.1_200214.xls` & `clophfit-0.7.1/tests/Tecan/140220/pH9.1_200214.xls`

 * *Files identical despite different names*

### Comparing `clophfit-0.7.0/tests/Tecan/exceptions/0_Labelblocks_290513_5.5.xlsx` & `clophfit-0.7.1/tests/Tecan/exceptions/0_Labelblocks_290513_5.5.xlsx`

 * *Files identical despite different names*

### Comparing `clophfit-0.7.0/tests/Tecan/exceptions/290212_7.67_repeated_lb.xls` & `clophfit-0.7.1/tests/Tecan/exceptions/290212_7.67_repeated_lb.xls`

 * *Files identical despite different names*

### Comparing `clophfit-0.7.0/tests/Tecan/exceptions/84wells_290212_20.xlsx` & `clophfit-0.7.1/tests/Tecan/exceptions/84wells_290212_20.xlsx`

 * *Files identical despite different names*

### Comparing `clophfit-0.7.0/tests/Tecan/exceptions/88wells_290212_20.xlsx` & `clophfit-0.7.1/tests/Tecan/exceptions/88wells_290212_20.xlsx`

 * *Files identical despite different names*

### Comparing `clophfit-0.7.0/tests/data/A01-20140311a.dat` & `clophfit-0.7.1/tests/data/A01-20140311a.dat`

 * *Files identical despite different names*

### Comparing `clophfit-0.7.0/tests/data/A01.dat` & `clophfit-0.7.1/tests/data/A01.dat`

 * *Files identical despite different names*

### Comparing `clophfit-0.7.0/tests/data/NTT-A04-Cl_note` & `clophfit-0.7.1/tests/data/NTT-A04-Cl_note`

 * *Files identical despite different names*

### Comparing `clophfit-0.7.0/tests/data/Meas/A04 Cl_A.csv` & `clophfit-0.7.1/tests/data/Meas/A04 Cl_A.csv`

 * *Files identical despite different names*

### Comparing `clophfit-0.7.0/tests/data/Meas/A04 Cl_A.png` & `clophfit-0.7.1/tests/data/Meas/A04 Cl_A.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.7.0/tests/data/Meas/A04 Cl_B.csv` & `clophfit-0.7.1/tests/data/Meas/A04 Cl_B.csv`

 * *Files identical despite different names*

### Comparing `clophfit-0.7.0/tests/data/Meas/A04 Cl_B.png` & `clophfit-0.7.1/tests/data/Meas/A04 Cl_B.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.7.0/tests/data/Meas/A04 Cl_C.csv` & `clophfit-0.7.1/tests/data/Meas/A04 Cl_C.csv`

 * *Files identical despite different names*

### Comparing `clophfit-0.7.0/tests/data/Meas/A04 Cl_C.png` & `clophfit-0.7.1/tests/data/Meas/A04 Cl_C.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.7.0/tests/data/Meas/A04 Cl_D.csv` & `clophfit-0.7.1/tests/data/Meas/A04 Cl_D.csv`

 * *Files identical despite different names*

### Comparing `clophfit-0.7.0/tests/data/Meas/A04 Cl_D.png` & `clophfit-0.7.1/tests/data/Meas/A04 Cl_D.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.7.0/tests/data/Meas/A04 Cl_E.csv` & `clophfit-0.7.1/tests/data/Meas/A04 Cl_E.csv`

 * *Files identical despite different names*

### Comparing `clophfit-0.7.0/tests/data/Meas/A04 Cl_E.png` & `clophfit-0.7.1/tests/data/Meas/A04 Cl_E.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.7.0/tests/data/Meas/A04 Cl_F.csv` & `clophfit-0.7.1/tests/data/Meas/A04 Cl_F.csv`

 * *Files identical despite different names*

### Comparing `clophfit-0.7.0/tests/data/Meas/A04 Cl_F.png` & `clophfit-0.7.1/tests/data/Meas/A04 Cl_F.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.7.0/tests/data/k/D05.dat-bs.png` & `clophfit-0.7.1/tests/data/k/D05.dat-bs.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.7.0/tests/data/k/D05.dat.png` & `clophfit-0.7.1/tests/data/k/D05.dat.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.7.0/tests/data/output/band_A04 Cl_A_NTT-A04-Cl_note.pdf` & `clophfit-0.7.1/tests/data/output/band_A04 Cl_A_NTT-A04-Cl_note.pdf`

 * *Files identical despite different names*

### Comparing `clophfit-0.7.0/tests/data/output/band_A04 Cl_B_NTT-A04-Cl_note.pdf` & `clophfit-0.7.1/tests/data/output/band_A04 Cl_B_NTT-A04-Cl_note.pdf`

 * *Files identical despite different names*

### Comparing `clophfit-0.7.0/tests/data/output/svd_A04 Cl_A_NTT-A04-Cl_note.pdf` & `clophfit-0.7.1/tests/data/output/svd_A04 Cl_A_NTT-A04-Cl_note.pdf`

 * *Files identical despite different names*

### Comparing `clophfit-0.7.0/tests/data/output/svd_A04 Cl_B_NTT-A04-Cl_note.pdf` & `clophfit-0.7.1/tests/data/output/svd_A04 Cl_B_NTT-A04-Cl_note.pdf`

 * *Files identical despite different names*

### Comparing `clophfit-0.7.0/tests/data/output/global/Cl/B05-20130628-cor.dat.png` & `clophfit-0.7.1/tests/data/output/global/Cl/B05-20130628-cor.dat.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.7.0/tests/data/output/global/pH/D05.dat.png` & `clophfit-0.7.1/tests/data/output/global/pH/D05.dat.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.7.0/.gitignore` & `clophfit-0.7.1/.gitignore`

 * *Files identical despite different names*

### Comparing `clophfit-0.7.0/LICENSE.txt` & `clophfit-0.7.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `clophfit-0.7.0/README.md` & `clophfit-0.7.1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![RtD](https://readthedocs.org/projects/clophfit/badge/)](https://clophfit.readthedocs.io/)
 [![zenodo](https://zenodo.org/badge/DOI/10.5281/zenodo.6354112.svg)](https://doi.org/10.5281/zenodo.6354112)
 
 This package provides a command line interface for fitting pH titration or
 binding assay data for macromolecules, such as fluorescence spectra. With this
 tool, users can easily analyze their data and obtain accurate fitting results.
 
-- Version: "0.7.0"
+- Version: "0.7.1"
 
 ## Installation
 
 You can get the library directly from
 [PyPI](https://pypi.org/project/ClopHfit/):
 
     pip install clophfit
@@ -93,10 +93,10 @@
 All code is licensed under the terms of the [revised BSD license](LICENSE.txt).
 
 ## Contributing
 
 If you are interested in contributing to the project, please read our
 [contributing](https://darosio.github.io/ClopHfit/references/contributing.html)
 and
-[development environment](https://darosio.github.io/ClopHfit/references/contributing.html#development)
+[development environment](https://darosio.github.io/ClopHfit/references/development.html)
 guides, which outline the guidelines and conventions that we follow for
 contributing code, documentation, and other resources.
```

### Comparing `clophfit-0.7.0/pyproject.toml` & `clophfit-0.7.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -44,15 +44,15 @@
   "macromolecule binding"
 ]
 license = "BSD-3-Clause"
 license-files = {paths = ["LICENSE.txt"]}
 name = "clophfit"
 readme = "README.md"
 requires-python = ">=3.8, <3.12"
-version = "0.7.0"
+version = "0.7.1"
 
 [project.optional-dependencies]
 dev = [
   "commitizen < 3.2.3",
   "ipykernel",
   "jupyter",
   "ruff == 0.0.267",
@@ -106,15 +106,15 @@
 '''
 line-length = 88
 skip-string-normalization = false
 
 [tool.commitizen]
 name = "cz_customize"
 tag_format = "v$version"
-version = "0.7.0"
+version = "0.7.1"
 version_files = [
   "pyproject.toml:version",
   "docs/conf.py:release",
   "README.md:Version"
 ]
 
 [tool.commitizen.customize]
```

### Comparing `clophfit-0.7.0/PKG-INFO` & `clophfit-0.7.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clophfit
-Version: 0.7.0
+Version: 0.7.1
 Summary: Cli for fitting macromolecule pH titration or binding assays data e.g. fluorescence spectra.
 Project-URL: Bug Tracker, https://github.com/darosio/ClopHfit/issues
 Project-URL: Changelog, https://darosio.github.io/ClopHfit/misc/CHANGELOG.html
 Project-URL: Discussions, https://github.com/darosio/ClopHfit/discussions
 Project-URL: Documentation, https://clophfit.readthedocs.io
 Project-URL: Github releases, https://github.com/darosio/ClopHfit/releases
 Project-URL: Homepage, https://github.com/darosio/ClopHfit
@@ -71,15 +71,15 @@
 [![RtD](https://readthedocs.org/projects/clophfit/badge/)](https://clophfit.readthedocs.io/)
 [![zenodo](https://zenodo.org/badge/DOI/10.5281/zenodo.6354112.svg)](https://doi.org/10.5281/zenodo.6354112)
 
 This package provides a command line interface for fitting pH titration or
 binding assay data for macromolecules, such as fluorescence spectra. With this
 tool, users can easily analyze their data and obtain accurate fitting results.
 
-- Version: "0.7.0"
+- Version: "0.7.1"
 
 ## Installation
 
 You can get the library directly from
 [PyPI](https://pypi.org/project/ClopHfit/):
 
     pip install clophfit
@@ -158,10 +158,10 @@
 All code is licensed under the terms of the [revised BSD license](LICENSE.txt).
 
 ## Contributing
 
 If you are interested in contributing to the project, please read our
 [contributing](https://darosio.github.io/ClopHfit/references/contributing.html)
 and
-[development environment](https://darosio.github.io/ClopHfit/references/contributing.html#development)
+[development environment](https://darosio.github.io/ClopHfit/references/development.html)
 guides, which outline the guidelines and conventions that we follow for
 contributing code, documentation, and other resources.
```

