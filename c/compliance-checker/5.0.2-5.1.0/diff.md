# Comparing `tmp/compliance-checker-5.0.2.tar.gz` & `tmp/compliance-checker-5.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "compliance-checker-5.0.2.tar", last modified: Wed May 25 17:38:26 2022, max compression
+gzip compressed data, was "compliance-checker-5.1.0.tar", last modified: Wed May 17 22:30:11 2023, max compression
```

## Comparing `compliance-checker-5.0.2.tar` & `compliance-checker-5.1.0.tar`

### file list

```diff
@@ -1,276 +1,231 @@
-drwxrwxr-x   0 filipe    (1000) filipe    (1000)        0 2022-05-25 17:38:26.148293 compliance-checker-5.0.2/
--rw-r--r--   0 filipe    (1000) filipe    (1000)       76 2022-01-25 23:31:09.000000 compliance-checker-5.0.2/.coveragerc
-drwxrwxr-x   0 filipe    (1000) filipe    (1000)        0 2022-05-25 17:38:26.100293 compliance-checker-5.0.2/.github/
-drwxrwxr-x   0 filipe    (1000) filipe    (1000)        0 2022-05-25 17:38:26.104294 compliance-checker-5.0.2/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 filipe    (1000) filipe    (1000)      677 2021-08-16 20:06:40.000000 compliance-checker-5.0.2/.github/ISSUE_TEMPLATE/compliance-checker-issue-report.md
-drwxrwxr-x   0 filipe    (1000) filipe    (1000)        0 2022-05-25 17:38:26.104294 compliance-checker-5.0.2/.github/workflows/
--rw-rw-r--   0 filipe    (1000) filipe    (1000)     1132 2022-05-25 17:21:24.000000 compliance-checker-5.0.2/.github/workflows/cc-checker-ugrid-test.yml
--rw-rw-r--   0 filipe    (1000) filipe    (1000)     1081 2022-05-25 17:21:24.000000 compliance-checker-5.0.2/.github/workflows/cc-plugin-glider-test.yml
--rw-rw-r--   0 filipe    (1000) filipe    (1000)     1077 2022-05-25 17:21:24.000000 compliance-checker-5.0.2/.github/workflows/cc-plugin-sgrid-test.yml
--rw-rw-r--   0 filipe    (1000) filipe    (1000)     1398 2022-05-25 17:21:24.000000 compliance-checker-5.0.2/.github/workflows/codecov.yml
--rw-rw-r--   0 filipe    (1000) filipe    (1000)     1079 2022-05-25 17:21:24.000000 compliance-checker-5.0.2/.github/workflows/default-tests.yml
--rw-rw-r--   0 filipe    (1000) filipe    (1000)      926 2022-05-25 17:21:24.000000 compliance-checker-5.0.2/.github/workflows/integration-tests.yml
--rw-rw-r--   0 filipe    (1000) filipe    (1000)     1019 2022-05-25 17:21:24.000000 compliance-checker-5.0.2/.github/workflows/publish.yml
--rw-r--r--   0 filipe    (1000) filipe    (1000)     1275 2022-01-25 23:31:09.000000 compliance-checker-5.0.2/.gitignore
--rw-rw-r--   0 filipe    (1000) filipe    (1000)      205 2022-05-25 17:34:57.000000 compliance-checker-5.0.2/.isort.cfg
--rw-rw-r--   0 filipe    (1000) filipe    (1000)     1499 2022-05-25 17:34:57.000000 compliance-checker-5.0.2/.pre-commit-config.yaml
--rw-r--r--   0 filipe    (1000) filipe    (1000)    11357 2020-07-02 17:13:22.000000 compliance-checker-5.0.2/LICENSE
--rw-r--r--   0 filipe    (1000) filipe    (1000)      354 2020-06-17 16:18:59.000000 compliance-checker-5.0.2/MANIFEST.in
--rw-rw-r--   0 filipe    (1000) filipe    (1000)    24271 2022-05-25 17:38:26.148293 compliance-checker-5.0.2/PKG-INFO
--rw-rw-r--   0 filipe    (1000) filipe    (1000)    23464 2022-05-25 17:34:57.000000 compliance-checker-5.0.2/README.md
--rwxrwxr-x   0 filipe    (1000) filipe    (1000)    11605 2022-05-25 17:34:57.000000 compliance-checker-5.0.2/cchecker.py
-drwxrwxr-x   0 filipe    (1000) filipe    (1000)        0 2022-05-25 17:38:26.104294 compliance-checker-5.0.2/compliance_checker/
--rw-rw-r--   0 filipe    (1000) filipe    (1000)     1496 2022-05-25 17:34:57.000000 compliance-checker-5.0.2/compliance_checker/__init__.py
--rw-rw-r--   0 filipe    (1000) filipe    (1000)       21 2022-05-25 17:38:25.000000 compliance-checker-5.0.2/compliance_checker/_version.py
--rw-rw-r--   0 filipe    (1000) filipe    (1000)    29826 2022-05-25 17:34:57.000000 compliance-checker-5.0.2/compliance_checker/acdd.py
--rw-rw-r--   0 filipe    (1000) filipe    (1000)    19847 2022-05-25 17:34:57.000000 compliance-checker-5.0.2/compliance_checker/base.py
-drwxrwxr-x   0 filipe    (1000) filipe    (1000)        0 2022-05-25 17:38:26.104294 compliance-checker-5.0.2/compliance_checker/cf/
--rw-rw-r--   0 filipe    (1000) filipe    (1000)      367 2022-05-25 17:34:57.000000 compliance-checker-5.0.2/compliance_checker/cf/__init__.py
--rw-rw-r--   0 filipe    (1000) filipe    (1000)      433 2022-05-25 17:34:57.000000 compliance-checker-5.0.2/compliance_checker/cf/appendix_c.py
--rw-rw-r--   0 filipe    (1000) filipe    (1000)     4822 2022-05-25 17:34:57.000000 compliance-checker-5.0.2/compliance_checker/cf/appendix_d.py
--rw-r--r--   0 filipe    (1000) filipe    (1000)      589 2021-06-11 17:13:31.000000 compliance-checker-5.0.2/compliance_checker/cf/appendix_e.py
--rw-r--r--   0 filipe    (1000) filipe    (1000)    24131 2021-06-28 16:22:04.000000 compliance-checker-5.0.2/compliance_checker/cf/appendix_f.py
--rw-rw-r--   0 filipe    (1000) filipe    (1000)     1136 2022-05-25 17:34:57.000000 compliance-checker-5.0.2/compliance_checker/cf/cf.py
--rw-rw-r--   0 filipe    (1000) filipe    (1000)   144373 2022-05-25 17:34:57.000000 compliance-checker-5.0.2/compliance_checker/cf/cf_1_6.py
--rw-rw-r--   0 filipe    (1000) filipe    (1000)    35431 2022-05-25 17:34:57.000000 compliance-checker-5.0.2/compliance_checker/cf/cf_1_7.py
--rw-rw-r--   0 filipe    (1000) filipe    (1000)    29127 2022-05-25 17:34:57.000000 compliance-checker-5.0.2/compliance_checker/cf/cf_1_8.py
--rw-rw-r--   0 filipe    (1000) filipe    (1000)    53724 2022-05-25 17:34:57.000000 compliance-checker-5.0.2/compliance_checker/cf/cf_base.py
--rw-rw-r--   0 filipe    (1000) filipe    (1000)    17223 2022-05-25 17:34:57.000000 compliance-checker-5.0.2/compliance_checker/cf/util.py
--rw-rw-r--   0 filipe    (1000) filipe    (1000)    61033 2022-05-25 17:34:57.000000 compliance-checker-5.0.2/compliance_checker/cfutil.py
-drwxrwxr-x   0 filipe    (1000) filipe    (1000)        0 2022-05-25 17:38:26.108294 compliance-checker-5.0.2/compliance_checker/data/
--rw-r--r--   0 filipe    (1000) filipe    (1000)  3942260 2020-06-11 18:41:56.000000 compliance-checker-5.0.2/compliance_checker/data/cf-standard-name-table.xml
--rw-r--r--   0 filipe    (1000) filipe    (1000)     3976 2020-06-11 18:41:56.000000 compliance-checker-5.0.2/compliance_checker/data/seanames.csv
-drwxrwxr-x   0 filipe    (1000) filipe    (1000)        0 2022-05-25 17:38:26.108294 compliance-checker-5.0.2/compliance_checker/data/templates/
--rw-r--r--   0 filipe    (1000) filipe    (1000)     6273 2020-07-30 15:57:44.000000 compliance-checker-5.0.2/compliance_checker/data/templates/ccheck.html.j2
--rw-r--r--   0 filipe    (1000) filipe    (1000)     6408 2020-06-11 18:41:56.000000 compliance-checker-5.0.2/compliance_checker/data/templates/ccheck_wrapper.html.j2
--rw-rw-r--   0 filipe    (1000) filipe    (1000)    71333 2022-05-25 17:34:57.000000 compliance-checker-5.0.2/compliance_checker/ioos.py
-drwxrwxr-x   0 filipe    (1000) filipe    (1000)        0 2022-05-25 17:38:26.108294 compliance-checker-5.0.2/compliance_checker/protocols/
--rw-r--r--   0 filipe    (1000) filipe    (1000)        0 2019-04-17 09:39:36.000000 compliance-checker-5.0.2/compliance_checker/protocols/__init__.py
--rw-r--r--   0 filipe    (1000) filipe    (1000)      822 2020-04-17 14:56:21.000000 compliance-checker-5.0.2/compliance_checker/protocols/cdl.py
--rw-r--r--   0 filipe    (1000) filipe    (1000)      218 2020-06-11 20:20:09.000000 compliance-checker-5.0.2/compliance_checker/protocols/erddap.py
--rw-rw-r--   0 filipe    (1000) filipe    (1000)     2338 2022-05-25 17:34:57.000000 compliance-checker-5.0.2/compliance_checker/protocols/netcdf.py
--rw-r--r--   0 filipe    (1000) filipe    (1000)     1898 2021-06-11 17:13:31.000000 compliance-checker-5.0.2/compliance_checker/protocols/opendap.py
--rw-rw-r--   0 filipe    (1000) filipe    (1000)    10458 2022-05-25 17:34:57.000000 compliance-checker-5.0.2/compliance_checker/runner.py
--rw-rw-r--   0 filipe    (1000) filipe    (1000)    38267 2022-05-25 17:34:57.000000 compliance-checker-5.0.2/compliance_checker/suite.py
-drwxrwxr-x   0 filipe    (1000) filipe    (1000)        0 2022-05-25 17:38:26.108294 compliance-checker-5.0.2/compliance_checker/tests/
--rw-r--r--   0 filipe    (1000) filipe    (1000)     1885 2021-10-29 15:51:49.000000 compliance-checker-5.0.2/compliance_checker/tests/__init__.py
--rw-rw-r--   0 filipe    (1000) filipe    (1000)     2919 2022-05-25 17:34:57.000000 compliance-checker-5.0.2/compliance_checker/tests/conftest.py
-drwxrwxr-x   0 filipe    (1000) filipe    (1000)        0 2022-05-25 17:38:26.144293 compliance-checker-5.0.2/compliance_checker/tests/data/
--rw-r--r--   0 filipe    (1000) filipe    (1000)    17408 2020-06-11 18:41:48.000000 compliance-checker-5.0.2/compliance_checker/tests/data/20160919092000-ABOM-L3S_GHRSST-SSTfnd-AVHRR_D-1d_dn_truncate.cdl
--rw-r--r--   0 filipe    (1000) filipe    (1000)    76161 2021-11-02 19:19:51.000000 compliance-checker-5.0.2/compliance_checker/tests/data/20160919092000-ABOM-L3S_GHRSST-SSTfnd-AVHRR_D-1d_dn_truncate.nc
--rw-r--r--   0 filipe    (1000) filipe    (1000)      977 2020-06-11 19:35:10.000000 compliance-checker-5.0.2/compliance_checker/tests/data/2d-regular-grid.cdl
--rw-r--r--   0 filipe    (1000) filipe    (1000)    14178 2021-11-02 19:19:52.000000 compliance-checker-5.0.2/compliance_checker/tests/data/2d-regular-grid.nc
--rw-r--r--   0 filipe    (1000) filipe    (1000)      373 2020-06-11 18:41:48.000000 compliance-checker-5.0.2/compliance_checker/tests/data/2d-static-grid.cdl
--rw-r--r--   0 filipe    (1000) filipe    (1000)     8192 2021-11-02 19:19:53.000000 compliance-checker-5.0.2/compliance_checker/tests/data/2d-static-grid.nc
--rw-r--r--   0 filipe    (1000) filipe    (1000)      774 2020-06-11 18:41:48.000000 compliance-checker-5.0.2/compliance_checker/tests/data/2dim-grid.cdl
--rw-r--r--   0 filipe    (1000) filipe    (1000)     8974 2021-11-02 19:19:52.000000 compliance-checker-5.0.2/compliance_checker/tests/data/2dim-grid.nc
--rw-r--r--   0 filipe    (1000) filipe    (1000)      994 2020-06-11 19:35:10.000000 compliance-checker-5.0.2/compliance_checker/tests/data/3d-regular-grid.cdl
--rw-r--r--   0 filipe    (1000) filipe    (1000)    16813 2021-11-02 19:19:53.000000 compliance-checker-5.0.2/compliance_checker/tests/data/3d-regular-grid.nc
--rw-r--r--   0 filipe    (1000) filipe    (1000)      520 2020-06-11 19:35:10.000000 compliance-checker-5.0.2/compliance_checker/tests/data/3d-static-grid.cdl
--rw-r--r--   0 filipe    (1000) filipe    (1000)     6819 2021-11-02 19:19:53.000000 compliance-checker-5.0.2/compliance_checker/tests/data/3d-static-grid.nc
--rw-r--r--   0 filipe    (1000) filipe    (1000)     7621 2020-06-11 18:41:48.000000 compliance-checker-5.0.2/compliance_checker/tests/data/NCEI_profile_template_v2.0_2016-09-22_181835.151325.cdl
--rw-r--r--   0 filipe    (1000) filipe    (1000)    38400 2021-11-02 19:19:52.000000 compliance-checker-5.0.2/compliance_checker/tests/data/NCEI_profile_template_v2.0_2016-09-22_181835.151325.nc
-drwxrwxr-x   0 filipe    (1000) filipe    (1000)        0 2022-05-25 17:38:26.144293 compliance-checker-5.0.2/compliance_checker/tests/data/appendix_h/
--rw-r--r--   0 filipe    (1000) filipe    (1000)     1274 2020-06-11 18:41:48.000000 compliance-checker-5.0.2/compliance_checker/tests/data/appendix_h/point.cdl
--rw-r--r--   0 filipe    (1000) filipe    (1000)     1996 2020-06-11 18:41:48.000000 compliance-checker-5.0.2/compliance_checker/tests/data/appendix_h/timeseries-incomplete.cdl
--rw-r--r--   0 filipe    (1000) filipe    (1000)     2271 2020-06-11 18:41:48.000000 compliance-checker-5.0.2/compliance_checker/tests/data/appendix_h/timeseries-non-static.cdl
--rw-r--r--   0 filipe    (1000) filipe    (1000)     1454 2020-06-11 18:41:48.000000 compliance-checker-5.0.2/compliance_checker/tests/data/appendix_h/timeseries-orthogonal.cdl
--rw-r--r--   0 filipe    (1000) filipe    (1000)     1766 2020-06-11 18:41:48.000000 compliance-checker-5.0.2/compliance_checker/tests/data/appendix_h/timeseries-single.cdl
--rw-r--r--   0 filipe    (1000) filipe    (1000)      657 2020-06-11 18:41:48.000000 compliance-checker-5.0.2/compliance_checker/tests/data/bad-instance.cdl
--rw-r--r--   0 filipe    (1000) filipe    (1000)      788 2022-01-25 23:31:09.000000 compliance-checker-5.0.2/compliance_checker/tests/data/bad-instance.nc
--rw-r--r--   0 filipe    (1000) filipe    (1000)      784 2020-06-11 19:35:10.000000 compliance-checker-5.0.2/compliance_checker/tests/data/bad-trajectory.cdl
--rw-r--r--   0 filipe    (1000) filipe    (1000)      828 2022-01-25 23:31:09.000000 compliance-checker-5.0.2/compliance_checker/tests/data/bad-trajectory.nc
--rw-r--r--   0 filipe    (1000) filipe    (1000)      812 2020-06-11 19:35:10.000000 compliance-checker-5.0.2/compliance_checker/tests/data/bad_cell_measure1.cdl
--rw-r--r--   0 filipe    (1000) filipe    (1000)      992 2022-01-25 23:31:09.000000 compliance-checker-5.0.2/compliance_checker/tests/data/bad_cell_measure1.nc
--rw-r--r--   0 filipe    (1000) filipe    (1000)      820 2020-06-11 19:35:10.000000 compliance-checker-5.0.2/compliance_checker/tests/data/bad_cell_measure2.cdl
--rw-r--r--   0 filipe    (1000) filipe    (1000)      992 2022-01-25 23:31:09.000000 compliance-checker-5.0.2/compliance_checker/tests/data/bad_cell_measure2.nc
--rw-r--r--   0 filipe    (1000) filipe    (1000)      841 2020-06-11 19:35:10.000000 compliance-checker-5.0.2/compliance_checker/tests/data/bad_cf_role.cdl
--rw-r--r--   0 filipe    (1000) filipe    (1000)     1060 2022-01-25 23:31:09.000000 compliance-checker-5.0.2/compliance_checker/tests/data/bad_cf_role.nc
--rw-r--r--   0 filipe    (1000) filipe    (1000)     1519 2020-06-11 19:35:10.000000 compliance-checker-5.0.2/compliance_checker/tests/data/bad_data_type.cdl
--rw-r--r--   0 filipe    (1000) filipe    (1000)    13207 2022-01-25 23:31:09.000000 compliance-checker-5.0.2/compliance_checker/tests/data/bad_data_type.nc
--rw-r--r--   0 filipe    (1000) filipe    (1000)     1272 2020-06-11 18:41:48.000000 compliance-checker-5.0.2/compliance_checker/tests/data/bad_missing_data.cdl
--rw-r--r--   0 filipe    (1000) filipe    (1000)    23864 2022-01-25 23:31:09.000000 compliance-checker-5.0.2/compliance_checker/tests/data/bad_missing_data.nc
--rw-r--r--   0 filipe    (1000) filipe    (1000)      332 2020-06-11 18:41:48.000000 compliance-checker-5.0.2/compliance_checker/tests/data/bad_reference.cdl
--rw-r--r--   0 filipe    (1000) filipe    (1000)      328 2022-01-25 23:31:09.000000 compliance-checker-5.0.2/compliance_checker/tests/data/bad_reference.nc
--rw-r--r--   0 filipe    (1000) filipe    (1000)     1093 2020-06-11 18:41:48.000000 compliance-checker-5.0.2/compliance_checker/tests/data/bad_region.cdl
--rw-r--r--   0 filipe    (1000) filipe    (1000)     1044 2022-01-25 23:31:09.000000 compliance-checker-5.0.2/compliance_checker/tests/data/bad_region.nc
--rw-r--r--   0 filipe    (1000) filipe    (1000)      912 2020-06-11 18:41:48.000000 compliance-checker-5.0.2/compliance_checker/tests/data/bad_units.cdl
--rw-r--r--   0 filipe    (1000) filipe    (1000)      820 2022-01-25 23:31:09.000000 compliance-checker-5.0.2/compliance_checker/tests/data/bad_units.nc
--rw-r--r--   0 filipe    (1000) filipe    (1000)      745 2020-06-11 19:35:10.000000 compliance-checker-5.0.2/compliance_checker/tests/data/cell_measure.cdl
--rw-r--r--   0 filipe    (1000) filipe    (1000)    10859 2021-11-02 19:19:50.000000 compliance-checker-5.0.2/compliance_checker/tests/data/cell_measure.nc
--rw-r--r--   0 filipe    (1000) filipe    (1000)      735 2020-06-11 18:41:48.000000 compliance-checker-5.0.2/compliance_checker/tests/data/cf_example_cell_measures.cdl
--rw-r--r--   0 filipe    (1000) filipe    (1000)      889 2020-06-11 18:41:48.000000 compliance-checker-5.0.2/compliance_checker/tests/data/chap2.cdl
--rw-r--r--   0 filipe    (1000) filipe    (1000)     8686 2021-11-02 19:19:50.000000 compliance-checker-5.0.2/compliance_checker/tests/data/chap2.nc
--rw-r--r--   0 filipe    (1000) filipe    (1000)      654 2020-06-11 18:41:48.000000 compliance-checker-5.0.2/compliance_checker/tests/data/climatology.cdl
--rw-r--r--   0 filipe    (1000) filipe    (1000)     7213 2021-11-02 19:19:50.000000 compliance-checker-5.0.2/compliance_checker/tests/data/climatology.nc
--rw-r--r--   0 filipe    (1000) filipe    (1000)     1692 2020-06-11 18:41:48.000000 compliance-checker-5.0.2/compliance_checker/tests/data/cont_ragged.cdl
--rw-r--r--   0 filipe    (1000) filipe    (1000)    13882 2021-11-02 19:19:50.000000 compliance-checker-5.0.2/compliance_checker/tests/data/cont_ragged.nc
--rw-r--r--   0 filipe    (1000) filipe    (1000)      434 2020-06-11 18:41:48.000000 compliance-checker-5.0.2/compliance_checker/tests/data/conv_bad.cdl
--rw-r--r--   0 filipe    (1000) filipe    (1000)      674 2021-11-02 19:19:50.000000 compliance-checker-5.0.2/compliance_checker/tests/data/conv_bad.nc
--rw-r--r--   0 filipe    (1000) filipe    (1000)      351 2020-06-11 18:41:48.000000 compliance-checker-5.0.2/compliance_checker/tests/data/conv_multi.cdl
--rw-r--r--   0 filipe    (1000) filipe    (1000)      590 2021-11-02 19:19:50.000000 compliance-checker-5.0.2/compliance_checker/tests/data/conv_multi.nc
--rw-r--r--   0 filipe    (1000) filipe    (1000)     1256 2020-06-11 19:35:10.000000 compliance-checker-5.0.2/compliance_checker/tests/data/coordinate_types.cdl
--rw-r--r--   0 filipe    (1000) filipe    (1000)     6995 2021-11-02 19:19:50.000000 compliance-checker-5.0.2/compliance_checker/tests/data/coordinate_types.nc
--rw-r--r--   0 filipe    (1000) filipe    (1000)      385 2020-06-11 18:41:48.000000 compliance-checker-5.0.2/compliance_checker/tests/data/coordinates_and_metadata.cdl
--rw-r--r--   0 filipe    (1000) filipe    (1000)     6900 2021-11-02 19:19:50.000000 compliance-checker-5.0.2/compliance_checker/tests/data/coordinates_and_metadata.nc
--rw-r--r--   0 filipe    (1000) filipe    (1000)     1125 2020-06-11 18:41:48.000000 compliance-checker-5.0.2/compliance_checker/tests/data/dimension_order.cdl
--rw-r--r--   0 filipe    (1000) filipe    (1000)     7468 2021-11-02 19:19:51.000000 compliance-checker-5.0.2/compliance_checker/tests/data/dimension_order.nc
--rw-r--r--   0 filipe    (1000) filipe    (1000)      491 2020-06-11 18:41:48.000000 compliance-checker-5.0.2/compliance_checker/tests/data/dimensionless.cdl
--rw-r--r--   0 filipe    (1000) filipe    (1000)     7799 2021-11-02 19:19:50.000000 compliance-checker-5.0.2/compliance_checker/tests/data/dimensionless.nc
--rw-r--r--   0 filipe    (1000) filipe    (1000)     1528 2020-06-11 18:41:48.000000 compliance-checker-5.0.2/compliance_checker/tests/data/duplicate_axis.cdl
--rw-r--r--   0 filipe    (1000) filipe    (1000)    13844 2021-11-02 19:19:51.000000 compliance-checker-5.0.2/compliance_checker/tests/data/duplicate_axis.nc
--rw-r--r--   0 filipe    (1000) filipe    (1000)     1197 2020-06-11 18:41:48.000000 compliance-checker-5.0.2/compliance_checker/tests/data/example-grid.cdl
--rw-r--r--   0 filipe    (1000) filipe    (1000)    18294 2021-11-02 19:19:51.000000 compliance-checker-5.0.2/compliance_checker/tests/data/example-grid.nc
-drwxrwxr-x   0 filipe    (1000) filipe    (1000)        0 2022-05-25 17:38:26.148293 compliance-checker-5.0.2/compliance_checker/tests/data/examples/
--rw-r--r--   0 filipe    (1000) filipe    (1000)     9070 2020-06-11 18:41:48.000000 compliance-checker-5.0.2/compliance_checker/tests/data/examples/3mf07.cdl
--rw-r--r--   0 filipe    (1000) filipe    (1000)      926 2022-01-07 16:22:59.000000 compliance-checker-5.0.2/compliance_checker/tests/data/examples/bio_taxa.cdl
--rw-r--r--   0 filipe    (1000) filipe    (1000)      829 2020-06-11 18:41:48.000000 compliance-checker-5.0.2/compliance_checker/tests/data/examples/cf_example_cell_measures.cdl
--rw-r--r--   0 filipe    (1000) filipe    (1000)     9443 2020-06-11 18:41:48.000000 compliance-checker-5.0.2/compliance_checker/tests/data/examples/fvcom.cdl
--rw-r--r--   0 filipe    (1000) filipe    (1000)     4416 2020-06-11 18:41:48.000000 compliance-checker-5.0.2/compliance_checker/tests/data/examples/glcfs.cdl
--rw-r--r--   0 filipe    (1000) filipe    (1000)     1206 2020-06-11 18:41:48.000000 compliance-checker-5.0.2/compliance_checker/tests/data/examples/hycom_global.cdl
--rw-r--r--   0 filipe    (1000) filipe    (1000)     5779 2020-06-11 18:41:48.000000 compliance-checker-5.0.2/compliance_checker/tests/data/examples/kibesillah.cdl
--rw-r--r--   0 filipe    (1000) filipe    (1000)    12628 2020-06-11 18:41:48.000000 compliance-checker-5.0.2/compliance_checker/tests/data/examples/l01-met.cdl
--rw-r--r--   0 filipe    (1000) filipe    (1000)    20715 2020-06-11 18:41:48.000000 compliance-checker-5.0.2/compliance_checker/tests/data/examples/ocos.cdl
--rw-r--r--   0 filipe    (1000) filipe    (1000)    11614 2020-06-11 18:41:48.000000 compliance-checker-5.0.2/compliance_checker/tests/data/examples/ooi_glider.cdl
--rw-r--r--   0 filipe    (1000) filipe    (1000)    11003 2020-06-11 18:41:48.000000 compliance-checker-5.0.2/compliance_checker/tests/data/examples/pr_inundation.cdl
--rw-r--r--   0 filipe    (1000) filipe    (1000)     2642 2020-06-11 19:35:10.000000 compliance-checker-5.0.2/compliance_checker/tests/data/examples/sldmb_43093_agg.cdl
--rw-r--r--   0 filipe    (1000) filipe    (1000)    29171 2020-06-11 18:41:48.000000 compliance-checker-5.0.2/compliance_checker/tests/data/examples/sp041.cdl
--rw-r--r--   0 filipe    (1000) filipe    (1000)     7257 2020-06-11 18:41:48.000000 compliance-checker-5.0.2/compliance_checker/tests/data/examples/swan.cdl
--rw-r--r--   0 filipe    (1000) filipe    (1000)     3751 2020-06-11 18:41:48.000000 compliance-checker-5.0.2/compliance_checker/tests/data/examples/usgs_dem_saipan.cdl
--rw-r--r--   0 filipe    (1000) filipe    (1000)     1242 2020-06-11 18:41:48.000000 compliance-checker-5.0.2/compliance_checker/tests/data/examples/ww3.cdl
--rw-r--r--   0 filipe    (1000) filipe    (1000)      996 2020-06-11 18:41:48.000000 compliance-checker-5.0.2/compliance_checker/tests/data/forecast_reference.cdl
--rw-r--r--   0 filipe    (1000) filipe    (1000)    10458 2021-11-02 19:19:51.000000 compliance-checker-5.0.2/compliance_checker/tests/data/forecast_reference.nc
--rw-r--r--   0 filipe    (1000) filipe    (1000)     1229 2020-06-11 19:35:10.000000 compliance-checker-5.0.2/compliance_checker/tests/data/grid-boundaries.cdl
--rw-r--r--   0 filipe    (1000) filipe    (1000)    15976 2021-11-02 19:19:51.000000 compliance-checker-5.0.2/compliance_checker/tests/data/grid-boundaries.nc
--rw-r--r--   0 filipe    (1000) filipe    (1000)     1820 2020-06-11 18:41:48.000000 compliance-checker-5.0.2/compliance_checker/tests/data/grid_mapping_coordinates.cdl
--rw-r--r--   0 filipe    (1000) filipe    (1000)    13955 2021-11-02 19:19:51.000000 compliance-checker-5.0.2/compliance_checker/tests/data/grid_mapping_coordinates.nc
-drwxrwxr-x   0 filipe    (1000) filipe    (1000)        0 2022-05-25 17:38:26.148293 compliance-checker-5.0.2/compliance_checker/tests/data/http_mocks/
--rw-r--r--   0 filipe    (1000) filipe    (1000)    17660 2020-06-11 18:41:48.000000 compliance-checker-5.0.2/compliance_checker/tests/data/http_mocks/ncsos_describesensor.xml
--rw-r--r--   0 filipe    (1000) filipe    (1000)    10033 2020-06-11 19:35:10.000000 compliance-checker-5.0.2/compliance_checker/tests/data/http_mocks/ncsos_getcapabilities.xml
--rw-r--r--   0 filipe    (1000) filipe    (1000)      748 2020-06-11 18:41:48.000000 compliance-checker-5.0.2/compliance_checker/tests/data/illegal-aux-coords.cdl
--rw-r--r--   0 filipe    (1000) filipe    (1000)     7836 2021-11-02 19:19:51.000000 compliance-checker-5.0.2/compliance_checker/tests/data/illegal-aux-coords.nc
--rw-r--r--   0 filipe    (1000) filipe    (1000)      384 2020-06-11 18:41:48.000000 compliance-checker-5.0.2/compliance_checker/tests/data/illegal-vertical.cdl
--rw-r--r--   0 filipe    (1000) filipe    (1000)     8192 2021-11-02 19:19:51.000000 compliance-checker-5.0.2/compliance_checker/tests/data/illegal-vertical.nc
--rw-r--r--   0 filipe    (1000) filipe    (1000)    15780 2020-06-11 18:41:48.000000 compliance-checker-5.0.2/compliance_checker/tests/data/index_ragged.cdl
--rw-r--r--   0 filipe    (1000) filipe    (1000)    59022 2021-11-02 19:19:51.000000 compliance-checker-5.0.2/compliance_checker/tests/data/index_ragged.nc
--rw-r--r--   0 filipe    (1000) filipe    (1000)      720 2021-08-10 19:13:32.000000 compliance-checker-5.0.2/compliance_checker/tests/data/index_ragged2.cdl
--rw-r--r--   0 filipe    (1000) filipe    (1000)     8181 2021-11-02 19:19:51.000000 compliance-checker-5.0.2/compliance_checker/tests/data/index_ragged2.nc
--rw-r--r--   0 filipe    (1000) filipe    (1000)      434 2020-06-11 18:41:48.000000 compliance-checker-5.0.2/compliance_checker/tests/data/ints64.cdl
--rw-r--r--   0 filipe    (1000) filipe    (1000)     6224 2021-11-02 19:19:51.000000 compliance-checker-5.0.2/compliance_checker/tests/data/ints64.nc
--rw-r--r--   0 filipe    (1000) filipe    (1000)     5951 2020-06-11 18:41:48.000000 compliance-checker-5.0.2/compliance_checker/tests/data/ioos_1_1.cdl
--rw-r--r--   0 filipe    (1000) filipe    (1000)    30161 2021-11-02 19:19:51.000000 compliance-checker-5.0.2/compliance_checker/tests/data/ioos_1_1.nc
--rw-r--r--   0 filipe    (1000) filipe    (1000)     1430 2022-01-07 16:22:59.000000 compliance-checker-5.0.2/compliance_checker/tests/data/line_geometry.cdl
--rw-r--r--   0 filipe    (1000) filipe    (1000)    13945 2021-11-02 19:19:51.000000 compliance-checker-5.0.2/compliance_checker/tests/data/line_geometry.nc
--rw-r--r--   0 filipe    (1000) filipe    (1000)     7038 2020-06-11 18:41:48.000000 compliance-checker-5.0.2/compliance_checker/tests/data/mapping.cdl
--rw-r--r--   0 filipe    (1000) filipe    (1000) 43008441 2021-11-02 19:19:51.000000 compliance-checker-5.0.2/compliance_checker/tests/data/mapping.nc
--rw-r--r--   0 filipe    (1000) filipe    (1000)      582 2020-06-11 18:41:48.000000 compliance-checker-5.0.2/compliance_checker/tests/data/multi-dim-coordinates.cdl
--rw-r--r--   0 filipe    (1000) filipe    (1000)     8012 2021-11-02 19:19:51.000000 compliance-checker-5.0.2/compliance_checker/tests/data/multi-dim-coordinates.nc
--rw-r--r--   0 filipe    (1000) filipe    (1000)     1014 2020-06-11 19:35:10.000000 compliance-checker-5.0.2/compliance_checker/tests/data/multi-timeseries-incomplete.cdl
--rw-r--r--   0 filipe    (1000) filipe    (1000)     8502 2021-11-02 19:19:52.000000 compliance-checker-5.0.2/compliance_checker/tests/data/multi-timeseries-incomplete.nc
--rw-r--r--   0 filipe    (1000) filipe    (1000)     1000 2020-06-11 19:35:10.000000 compliance-checker-5.0.2/compliance_checker/tests/data/multi-timeseries-orthogonal.cdl
--rw-r--r--   0 filipe    (1000) filipe    (1000)    10231 2021-11-02 19:19:51.000000 compliance-checker-5.0.2/compliance_checker/tests/data/multi-timeseries-orthogonal.nc
--rw-r--r--   0 filipe    (1000) filipe    (1000)     6737 2020-06-11 18:41:48.000000 compliance-checker-5.0.2/compliance_checker/tests/data/ncei_gold_point_1.cdl
--rw-r--r--   0 filipe    (1000) filipe    (1000)    38895 2021-11-02 19:19:52.000000 compliance-checker-5.0.2/compliance_checker/tests/data/ncei_gold_point_1.nc
--rw-r--r--   0 filipe    (1000) filipe    (1000)     7666 2020-06-11 18:41:48.000000 compliance-checker-5.0.2/compliance_checker/tests/data/ncei_gold_point_2.cdl
--rw-r--r--   0 filipe    (1000) filipe    (1000)    39212 2021-11-02 19:19:52.000000 compliance-checker-5.0.2/compliance_checker/tests/data/ncei_gold_point_2.nc
-drwxrwxr-x   0 filipe    (1000) filipe    (1000)        0 2022-05-25 17:38:26.148293 compliance-checker-5.0.2/compliance_checker/tests/data/non-comp/
--rw-r--r--   0 filipe    (1000) filipe    (1000)     1318 2020-06-11 18:41:48.000000 compliance-checker-5.0.2/compliance_checker/tests/data/non-comp/1d_bound_bad.cdl
--rw-r--r--   0 filipe    (1000) filipe    (1000)     1224 2020-06-11 18:41:48.000000 compliance-checker-5.0.2/compliance_checker/tests/data/non-comp/bad-rhgrid.cdl
--rw-r--r--   0 filipe    (1000) filipe    (1000)     1616 2020-06-11 18:41:48.000000 compliance-checker-5.0.2/compliance_checker/tests/data/non-comp/bad.cdl
--rw-r--r--   0 filipe    (1000) filipe    (1000)      843 2020-06-11 18:41:48.000000 compliance-checker-5.0.2/compliance_checker/tests/data/non-comp/bad2dim.cdl
--rw-r--r--   0 filipe    (1000) filipe    (1000)      255 2020-06-11 18:41:48.000000 compliance-checker-5.0.2/compliance_checker/tests/data/non-comp/badname.netcdf
--rw-r--r--   0 filipe    (1000) filipe    (1000)     1308 2020-06-11 18:41:48.000000 compliance-checker-5.0.2/compliance_checker/tests/data/non-comp/bounds_bad_num_coords.cdl
--rw-r--r--   0 filipe    (1000) filipe    (1000)     1318 2020-06-11 18:41:48.000000 compliance-checker-5.0.2/compliance_checker/tests/data/non-comp/bounds_bad_order.cdl
--rw-r--r--   0 filipe    (1000) filipe    (1000)        4 2020-06-11 18:41:48.000000 compliance-checker-5.0.2/compliance_checker/tests/data/non-comp/empty.file
--rw-r--r--   0 filipe    (1000) filipe    (1000)    24004 2020-06-11 18:41:48.000000 compliance-checker-5.0.2/compliance_checker/tests/data/non-comp/self_referencing.cdl
--rw-r--r--   0 filipe    (1000) filipe    (1000)      373 2020-06-11 18:41:48.000000 compliance-checker-5.0.2/compliance_checker/tests/data/non-comp/time_units.cdl
--rw-r--r--   0 filipe    (1000) filipe    (1000)      930 2020-06-11 18:41:48.000000 compliance-checker-5.0.2/compliance_checker/tests/data/point.cdl
--rw-r--r--   0 filipe    (1000) filipe    (1000)     7856 2021-11-02 19:19:52.000000 compliance-checker-5.0.2/compliance_checker/tests/data/point.nc
--rw-r--r--   0 filipe    (1000) filipe    (1000)     1829 2022-01-07 16:22:59.000000 compliance-checker-5.0.2/compliance_checker/tests/data/polygon_geometry.cdl
--rw-r--r--   0 filipe    (1000) filipe    (1000)    15815 2021-11-02 19:19:52.000000 compliance-checker-5.0.2/compliance_checker/tests/data/polygon_geometry.nc
--rw-r--r--   0 filipe    (1000) filipe    (1000)     1020 2020-06-11 19:35:10.000000 compliance-checker-5.0.2/compliance_checker/tests/data/profile-incomplete.cdl
--rw-r--r--   0 filipe    (1000) filipe    (1000)     8560 2021-11-02 19:19:52.000000 compliance-checker-5.0.2/compliance_checker/tests/data/profile-incomplete.nc
--rw-r--r--   0 filipe    (1000) filipe    (1000)     1010 2020-06-11 19:35:10.000000 compliance-checker-5.0.2/compliance_checker/tests/data/profile-orthogonal.cdl
--rw-r--r--   0 filipe    (1000) filipe    (1000)    10338 2021-11-02 19:19:52.000000 compliance-checker-5.0.2/compliance_checker/tests/data/profile-orthogonal.nc
--rw-r--r--   0 filipe    (1000) filipe    (1000)      628 2020-06-11 18:41:48.000000 compliance-checker-5.0.2/compliance_checker/tests/data/reduced_horizontal_grid.cdl
--rw-r--r--   0 filipe    (1000) filipe    (1000)     8228 2021-11-02 19:19:52.000000 compliance-checker-5.0.2/compliance_checker/tests/data/reduced_horizontal_grid.nc
--rw-r--r--   0 filipe    (1000) filipe    (1000)      421 2020-06-11 18:41:48.000000 compliance-checker-5.0.2/compliance_checker/tests/data/rhgrid.cdl
--rw-r--r--   0 filipe    (1000) filipe    (1000)     7232 2021-11-02 19:19:52.000000 compliance-checker-5.0.2/compliance_checker/tests/data/rhgrid.nc
--rw-r--r--   0 filipe    (1000) filipe    (1000)     1362 2020-06-11 18:41:48.000000 compliance-checker-5.0.2/compliance_checker/tests/data/rotated_pole_grid.cdl
--rw-r--r--   0 filipe    (1000) filipe    (1000)    13237 2021-11-02 19:19:52.000000 compliance-checker-5.0.2/compliance_checker/tests/data/rotated_pole_grid.nc
--rw-r--r--   0 filipe    (1000) filipe    (1000)    43335 2020-06-11 18:41:48.000000 compliance-checker-5.0.2/compliance_checker/tests/data/ru07-20130824T170228_rt0.cdl
--rw-r--r--   0 filipe    (1000) filipe    (1000)   227687 2021-11-02 19:19:52.000000 compliance-checker-5.0.2/compliance_checker/tests/data/ru07-20130824T170228_rt0.nc
--rw-r--r--   0 filipe    (1000) filipe    (1000)      390 2020-06-11 18:41:48.000000 compliance-checker-5.0.2/compliance_checker/tests/data/scalar_coordinate_variable.cdl
--rw-r--r--   0 filipe    (1000) filipe    (1000)     5522 2021-11-02 19:19:52.000000 compliance-checker-5.0.2/compliance_checker/tests/data/scalar_coordinate_variable.nc
--rw-r--r--   0 filipe    (1000) filipe    (1000)      697 2020-06-11 18:41:48.000000 compliance-checker-5.0.2/compliance_checker/tests/data/self-referencing-var.cdl
--rw-r--r--   0 filipe    (1000) filipe    (1000)     8224 2021-11-02 19:19:52.000000 compliance-checker-5.0.2/compliance_checker/tests/data/self-referencing-var.nc
--rw-r--r--   0 filipe    (1000) filipe    (1000)      509 2020-11-29 00:41:12.000000 compliance-checker-5.0.2/compliance_checker/tests/data/string_type_variable.cdl
--rw-r--r--   0 filipe    (1000) filipe    (1000)     8192 2021-11-02 19:19:52.000000 compliance-checker-5.0.2/compliance_checker/tests/data/string_type_variable.nc
--rw-r--r--   0 filipe    (1000) filipe    (1000)     1160 2022-01-07 16:22:59.000000 compliance-checker-5.0.2/compliance_checker/tests/data/taxonomy_example.cdl
--rw-r--r--   0 filipe    (1000) filipe    (1000)     7959 2021-12-20 16:02:35.000000 compliance-checker-5.0.2/compliance_checker/tests/data/taxonomy_example.nc
--rw-r--r--   0 filipe    (1000) filipe    (1000)      924 2020-06-11 19:35:10.000000 compliance-checker-5.0.2/compliance_checker/tests/data/test_cdl.cdl
--rw-r--r--   0 filipe    (1000) filipe    (1000)     1033 2020-06-11 18:41:48.000000 compliance-checker-5.0.2/compliance_checker/tests/data/test_cdl_nc4_file.cdl
--rw-r--r--   0 filipe    (1000) filipe    (1000)    11301 2021-11-02 19:20:10.000000 compliance-checker-5.0.2/compliance_checker/tests/data/test_cdl_nc4_file.nc
--rw-r--r--   0 filipe    (1000) filipe    (1000)      924 2020-06-11 19:35:10.000000 compliance-checker-5.0.2/compliance_checker/tests/data/test_cdl_nc_file.cdl
--rw-r--r--   0 filipe    (1000) filipe    (1000)      936 2021-11-02 19:21:26.000000 compliance-checker-5.0.2/compliance_checker/tests/data/test_cdl_nc_file.nc
--rw-r--r--   0 filipe    (1000) filipe    (1000)     1033 2020-06-11 18:41:48.000000 compliance-checker-5.0.2/compliance_checker/tests/data/timeseries-profile-incomplete.cdl
--rw-r--r--   0 filipe    (1000) filipe    (1000)     9230 2021-11-02 19:19:52.000000 compliance-checker-5.0.2/compliance_checker/tests/data/timeseries-profile-incomplete.nc
--rw-r--r--   0 filipe    (1000) filipe    (1000)     1027 2020-06-11 19:35:10.000000 compliance-checker-5.0.2/compliance_checker/tests/data/timeseries-profile-multi-ortho-time.cdl
--rw-r--r--   0 filipe    (1000) filipe    (1000)    10933 2021-11-02 19:19:52.000000 compliance-checker-5.0.2/compliance_checker/tests/data/timeseries-profile-multi-ortho-time.nc
--rw-r--r--   0 filipe    (1000) filipe    (1000)     1007 2020-06-11 18:41:48.000000 compliance-checker-5.0.2/compliance_checker/tests/data/timeseries-profile-multi-station.cdl
--rw-r--r--   0 filipe    (1000) filipe    (1000)    12415 2021-11-02 19:19:52.000000 compliance-checker-5.0.2/compliance_checker/tests/data/timeseries-profile-multi-station.nc
--rw-r--r--   0 filipe    (1000) filipe    (1000)     1013 2020-06-11 19:35:10.000000 compliance-checker-5.0.2/compliance_checker/tests/data/timeseries-profile-ortho-depth.cdl
--rw-r--r--   0 filipe    (1000) filipe    (1000)    10733 2021-11-02 19:19:52.000000 compliance-checker-5.0.2/compliance_checker/tests/data/timeseries-profile-ortho-depth.nc
--rw-r--r--   0 filipe    (1000) filipe    (1000)      974 2020-06-11 19:35:10.000000 compliance-checker-5.0.2/compliance_checker/tests/data/timeseries-profile-single-ortho-time.cdl
--rw-r--r--   0 filipe    (1000) filipe    (1000)     9788 2021-11-02 19:19:52.000000 compliance-checker-5.0.2/compliance_checker/tests/data/timeseries-profile-single-ortho-time.nc
--rw-r--r--   0 filipe    (1000) filipe    (1000)      968 2020-06-11 19:35:10.000000 compliance-checker-5.0.2/compliance_checker/tests/data/timeseries-profile-single-station.cdl
--rw-r--r--   0 filipe    (1000) filipe    (1000)    11536 2021-11-02 19:19:52.000000 compliance-checker-5.0.2/compliance_checker/tests/data/timeseries-profile-single-station.nc
--rw-r--r--   0 filipe    (1000) filipe    (1000)      924 2020-06-11 19:35:10.000000 compliance-checker-5.0.2/compliance_checker/tests/data/timeseries.cdl
--rw-r--r--   0 filipe    (1000) filipe    (1000)     8922 2021-11-02 19:19:52.000000 compliance-checker-5.0.2/compliance_checker/tests/data/timeseries.nc
--rw-r--r--   0 filipe    (1000) filipe    (1000)      832 2020-06-11 18:41:48.000000 compliance-checker-5.0.2/compliance_checker/tests/data/trajectory-complete.cdl
--rw-r--r--   0 filipe    (1000) filipe    (1000)     8673 2021-11-02 19:19:52.000000 compliance-checker-5.0.2/compliance_checker/tests/data/trajectory-complete.nc
--rw-r--r--   0 filipe    (1000) filipe    (1000)      880 2020-06-11 18:41:48.000000 compliance-checker-5.0.2/compliance_checker/tests/data/trajectory-implied.cdl
--rw-r--r--   0 filipe    (1000) filipe    (1000)     8669 2021-11-02 19:19:52.000000 compliance-checker-5.0.2/compliance_checker/tests/data/trajectory-implied.nc
--rw-r--r--   0 filipe    (1000) filipe    (1000)     1063 2020-06-11 18:41:48.000000 compliance-checker-5.0.2/compliance_checker/tests/data/trajectory-profile-incomplete.cdl
--rw-r--r--   0 filipe    (1000) filipe    (1000)     9329 2021-11-02 19:19:52.000000 compliance-checker-5.0.2/compliance_checker/tests/data/trajectory-profile-incomplete.nc
--rw-r--r--   0 filipe    (1000) filipe    (1000)     1038 2020-06-11 19:35:10.000000 compliance-checker-5.0.2/compliance_checker/tests/data/trajectory-profile-orthogonal.cdl
--rw-r--r--   0 filipe    (1000) filipe    (1000)    10827 2021-11-02 19:19:52.000000 compliance-checker-5.0.2/compliance_checker/tests/data/trajectory-profile-orthogonal.nc
--rw-r--r--   0 filipe    (1000) filipe    (1000)     1023 2020-06-11 19:35:10.000000 compliance-checker-5.0.2/compliance_checker/tests/data/trajectory-single.cdl
--rw-r--r--   0 filipe    (1000) filipe    (1000)     9904 2021-11-02 19:19:52.000000 compliance-checker-5.0.2/compliance_checker/tests/data/trajectory-single.nc
--rw-r--r--   0 filipe    (1000) filipe    (1000)     1042 2020-06-11 19:35:10.000000 compliance-checker-5.0.2/compliance_checker/tests/data/trajectory.cdl
--rw-r--r--   0 filipe    (1000) filipe    (1000)     8796 2021-11-02 19:19:52.000000 compliance-checker-5.0.2/compliance_checker/tests/data/trajectory.nc
--rw-r--r--   0 filipe    (1000) filipe    (1000)     1346 2020-06-11 18:41:48.000000 compliance-checker-5.0.2/compliance_checker/tests/data/units_check.cdl
--rw-r--r--   0 filipe    (1000) filipe    (1000)     8398 2021-11-02 19:19:52.000000 compliance-checker-5.0.2/compliance_checker/tests/data/units_check.nc
--rw-r--r--   0 filipe    (1000) filipe    (1000)    14798 2020-06-11 18:41:48.000000 compliance-checker-5.0.2/compliance_checker/tests/data/valid_coordinates.cdl
--rw-r--r--   0 filipe    (1000) filipe    (1000)    71451 2021-11-02 19:19:52.000000 compliance-checker-5.0.2/compliance_checker/tests/data/valid_coordinates.nc
--rw-r--r--   0 filipe    (1000) filipe    (1000)      797 2020-06-11 18:41:48.000000 compliance-checker-5.0.2/compliance_checker/tests/data/vertical_coords.cdl
--rw-r--r--   0 filipe    (1000) filipe    (1000)     8192 2021-11-02 19:19:52.000000 compliance-checker-5.0.2/compliance_checker/tests/data/vertical_coords.nc
--rw-rw-r--   0 filipe    (1000) filipe    (1000)     8625 2022-05-25 17:34:57.000000 compliance-checker-5.0.2/compliance_checker/tests/helpers.py
--rw-r--r--   0 filipe    (1000) filipe    (1000)     8362 2022-01-07 16:22:59.000000 compliance-checker-5.0.2/compliance_checker/tests/resources.py
--rw-rw-r--   0 filipe    (1000) filipe    (1000)    21179 2022-05-25 17:34:57.000000 compliance-checker-5.0.2/compliance_checker/tests/test_acdd.py
--rw-rw-r--   0 filipe    (1000) filipe    (1000)     6706 2022-05-25 17:34:57.000000 compliance-checker-5.0.2/compliance_checker/tests/test_base.py
--rw-rw-r--   0 filipe    (1000) filipe    (1000)   138010 2022-05-25 17:34:57.000000 compliance-checker-5.0.2/compliance_checker/tests/test_cf.py
--rw-rw-r--   0 filipe    (1000) filipe    (1000)    22550 2022-05-25 17:34:57.000000 compliance-checker-5.0.2/compliance_checker/tests/test_cf_integration.py
--rw-rw-r--   0 filipe    (1000) filipe    (1000)     6859 2022-05-25 17:34:57.000000 compliance-checker-5.0.2/compliance_checker/tests/test_cli.py
--rw-r--r--   0 filipe    (1000) filipe    (1000)    29429 2021-08-10 19:13:32.000000 compliance-checker-5.0.2/compliance_checker/tests/test_feature_detection.py
--rw-rw-r--   0 filipe    (1000) filipe    (1000)    49590 2022-05-25 17:34:57.000000 compliance-checker-5.0.2/compliance_checker/tests/test_ioos_profile.py
--rw-rw-r--   0 filipe    (1000) filipe    (1000)     2533 2022-05-25 17:34:57.000000 compliance-checker-5.0.2/compliance_checker/tests/test_ioos_sos.py
--rw-rw-r--   0 filipe    (1000) filipe    (1000)     1882 2022-05-25 17:34:57.000000 compliance-checker-5.0.2/compliance_checker/tests/test_protocols.py
--rw-rw-r--   0 filipe    (1000) filipe    (1000)     9911 2022-05-25 17:34:57.000000 compliance-checker-5.0.2/compliance_checker/tests/test_suite.py
--rw-r--r--   0 filipe    (1000) filipe    (1000)     1602 2022-01-25 23:31:09.000000 compliance-checker-5.0.2/compliance_checker/tests/test_util.py
--rw-rw-r--   0 filipe    (1000) filipe    (1000)     1469 2022-05-25 17:34:57.000000 compliance-checker-5.0.2/compliance_checker/util.py
-drwxrwxr-x   0 filipe    (1000) filipe    (1000)        0 2022-05-25 17:38:26.104294 compliance-checker-5.0.2/compliance_checker.egg-info/
--rw-rw-r--   0 filipe    (1000) filipe    (1000)    24271 2022-05-25 17:38:25.000000 compliance-checker-5.0.2/compliance_checker.egg-info/PKG-INFO
--rw-rw-r--   0 filipe    (1000) filipe    (1000)    12180 2022-05-25 17:38:26.000000 compliance-checker-5.0.2/compliance_checker.egg-info/SOURCES.txt
--rw-rw-r--   0 filipe    (1000) filipe    (1000)        1 2022-05-25 17:38:25.000000 compliance-checker-5.0.2/compliance_checker.egg-info/dependency_links.txt
--rw-rw-r--   0 filipe    (1000) filipe    (1000)      509 2022-05-25 17:38:25.000000 compliance-checker-5.0.2/compliance_checker.egg-info/entry_points.txt
--rw-rw-r--   0 filipe    (1000) filipe    (1000)      224 2022-05-25 17:38:25.000000 compliance-checker-5.0.2/compliance_checker.egg-info/requires.txt
--rw-rw-r--   0 filipe    (1000) filipe    (1000)       19 2022-05-25 17:38:26.000000 compliance-checker-5.0.2/compliance_checker.egg-info/top_level.txt
-drwxrwxr-x   0 filipe    (1000) filipe    (1000)        0 2022-05-25 17:38:26.148293 compliance-checker-5.0.2/doc/
--rw-r--r--   0 filipe    (1000) filipe    (1000)     1170 2020-07-02 17:13:22.000000 compliance-checker-5.0.2/doc/ubuntu-install-guide.md
--rw-rw-r--   0 filipe    (1000) filipe    (1000)      343 2022-05-25 17:34:57.000000 compliance-checker-5.0.2/pyproject.toml
--rw-rw-r--   0 filipe    (1000) filipe    (1000)      224 2022-05-25 17:34:57.000000 compliance-checker-5.0.2/requirements.txt
--rw-rw-r--   0 filipe    (1000) filipe    (1000)       38 2022-05-25 17:38:26.148293 compliance-checker-5.0.2/setup.cfg
--rw-rw-r--   0 filipe    (1000) filipe    (1000)     2967 2022-05-25 17:34:57.000000 compliance-checker-5.0.2/setup.py
--rw-rw-r--   0 filipe    (1000) filipe    (1000)      104 2022-05-25 17:34:57.000000 compliance-checker-5.0.2/test_requirements.txt
--rw-r--r--   0 filipe    (1000) filipe    (1000)      395 2020-07-02 17:13:22.000000 compliance-checker-5.0.2/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:30:11.091334 compliance-checker-5.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:30:11.055334 compliance-checker-5.1.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:30:11.055334 compliance-checker-5.1.0/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      677 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/.github/ISSUE_TEMPLATE/compliance-checker-issue-report.md
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:30:11.059334 compliance-checker-5.1.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      953 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/.github/workflows/cc-checker-ugrid-test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      955 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/.github/workflows/cc-plugin-glider-test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      847 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/.github/workflows/cc-plugin-sgrid-test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      953 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/.github/workflows/cc-plugin-ugrid-test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/.github/workflows/codecov.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      933 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/.github/workflows/default-tests.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/.github/workflows/deploy-docs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      725 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/.github/workflows/integration-tests.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/.github/workflows/pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1320 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/.isort.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    24320 2023-05-17 22:30:11.091334 compliance-checker-5.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    23513 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (123)    11641 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/cchecker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:30:11.059334 compliance-checker-5.1.0/compliance_checker/
+-rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/compliance_checker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-17 22:30:10.000000 compliance-checker-5.1.0/compliance_checker/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30003 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/compliance_checker/acdd.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19822 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/compliance_checker/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:30:11.063334 compliance-checker-5.1.0/compliance_checker/cf/
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/compliance_checker/cf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      433 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/compliance_checker/cf/appendix_c.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4813 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/compliance_checker/cf/appendix_d.py
+-rw-r--r--   0 runner    (1001) docker     (123)      590 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/compliance_checker/cf/appendix_e.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24133 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/compliance_checker/cf/appendix_f.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/compliance_checker/cf/cf.py
+-rw-r--r--   0 runner    (1001) docker     (123)   156976 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/compliance_checker/cf/cf_1_6.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38843 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/compliance_checker/cf/cf_1_7.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29294 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/compliance_checker/cf/cf_1_8.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6813 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/compliance_checker/cf/cf_1_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)    54398 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/compliance_checker/cf/cf_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12177 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/compliance_checker/cf/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    61097 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/compliance_checker/cfutil.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:30:11.067334 compliance-checker-5.1.0/compliance_checker/data/
+-rw-r--r--   0 runner    (1001) docker     (123)  3942260 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/compliance_checker/data/cf-standard-name-table.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     3976 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/compliance_checker/data/seanames.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:30:11.067334 compliance-checker-5.1.0/compliance_checker/data/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     6273 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/compliance_checker/data/templates/ccheck.html.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     6408 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/compliance_checker/data/templates/ccheck_wrapper.html.j2
+-rw-r--r--   0 runner    (1001) docker     (123)    71588 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/compliance_checker/ioos.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:30:11.067334 compliance-checker-5.1.0/compliance_checker/protocols/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/compliance_checker/protocols/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      822 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/compliance_checker/protocols/cdl.py
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/compliance_checker/protocols/erddap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2355 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/compliance_checker/protocols/netcdf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1875 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/compliance_checker/protocols/opendap.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10644 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/compliance_checker/runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38029 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/compliance_checker/suite.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:30:11.071334 compliance-checker-5.1.0/compliance_checker/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/compliance_checker/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:30:11.071334 compliance-checker-5.1.0/compliance_checker/tests/cassettes/
+-rw-r--r--   0 runner    (1001) docker     (123)     7986 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/compliance_checker/tests/cassettes/test_erddap.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    16262 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/compliance_checker/tests/cassettes/test_netcdf_content_type.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2919 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/compliance_checker/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:30:11.083334 compliance-checker-5.1.0/compliance_checker/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)    17408 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/compliance_checker/tests/data/20160919092000-ABOM-L3S_GHRSST-SSTfnd-AVHRR_D-1d_dn_truncate.cdl
+-rw-r--r--   0 runner    (1001) docker     (123)      977 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/compliance_checker/tests/data/2d-regular-grid.cdl
+-rw-r--r--   0 runner    (1001) docker     (123)      373 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/compliance_checker/tests/data/2d-static-grid.cdl
+-rw-r--r--   0 runner    (1001) docker     (123)      774 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/compliance_checker/tests/data/2dim-grid.cdl
+-rw-r--r--   0 runner    (1001) docker     (123)      994 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/compliance_checker/tests/data/3d-regular-grid.cdl
+-rw-r--r--   0 runner    (1001) docker     (123)      520 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/compliance_checker/tests/data/3d-static-grid.cdl
+-rw-r--r--   0 runner    (1001) docker     (123)     7621 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/compliance_checker/tests/data/NCEI_profile_template_v2.0_2016-09-22_181835.151325.cdl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:30:11.087334 compliance-checker-5.1.0/compliance_checker/tests/data/appendix_h/
+-rw-r--r--   0 runner    (1001) docker     (123)     1274 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/compliance_checker/tests/data/appendix_h/point.cdl
+-rw-r--r--   0 runner    (1001) docker     (123)     1996 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/compliance_checker/tests/data/appendix_h/timeseries-incomplete.cdl
+-rw-r--r--   0 runner    (1001) docker     (123)     2271 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/compliance_checker/tests/data/appendix_h/timeseries-non-static.cdl
+-rw-r--r--   0 runner    (1001) docker     (123)     1454 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/compliance_checker/tests/data/appendix_h/timeseries-orthogonal.cdl
+-rw-r--r--   0 runner    (1001) docker     (123)     1766 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/compliance_checker/tests/data/appendix_h/timeseries-single.cdl
+-rw-r--r--   0 runner    (1001) docker     (123)      657 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/compliance_checker/tests/data/bad-instance.cdl
+-rw-r--r--   0 runner    (1001) docker     (123)      788 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/compliance_checker/tests/data/bad-instance.nc
+-rw-r--r--   0 runner    (1001) docker     (123)      784 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/compliance_checker/tests/data/bad-trajectory.cdl
+-rw-r--r--   0 runner    (1001) docker     (123)      828 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/compliance_checker/tests/data/bad-trajectory.nc
+-rw-r--r--   0 runner    (1001) docker     (123)      812 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/compliance_checker/tests/data/bad_cell_measure1.cdl
+-rw-r--r--   0 runner    (1001) docker     (123)      992 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/compliance_checker/tests/data/bad_cell_measure1.nc
+-rw-r--r--   0 runner    (1001) docker     (123)      820 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/compliance_checker/tests/data/bad_cell_measure2.cdl
+-rw-r--r--   0 runner    (1001) docker     (123)      992 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/compliance_checker/tests/data/bad_cell_measure2.nc
+-rw-r--r--   0 runner    (1001) docker     (123)      841 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/compliance_checker/tests/data/bad_cf_role.cdl
+-rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/compliance_checker/tests/data/bad_cf_role.nc
+-rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/compliance_checker/tests/data/bad_data_type.cdl
+-rw-r--r--   0 runner    (1001) docker     (123)    13207 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/compliance_checker/tests/data/bad_data_type.nc
+-rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/compliance_checker/tests/data/bad_missing_data.cdl
+-rw-r--r--   0 runner    (1001) docker     (123)    23864 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/compliance_checker/tests/data/bad_missing_data.nc
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/compliance_checker/tests/data/bad_reference.cdl
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/compliance_checker/tests/data/bad_reference.nc
+-rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/compliance_checker/tests/data/bad_region.cdl
+-rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/compliance_checker/tests/data/bad_region.nc
+-rw-r--r--   0 runner    (1001) docker     (123)      912 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/compliance_checker/tests/data/bad_units.cdl
+-rw-r--r--   0 runner    (1001) docker     (123)      820 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/compliance_checker/tests/data/bad_units.nc
+-rw-r--r--   0 runner    (1001) docker     (123)      745 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/compliance_checker/tests/data/cell_measure.cdl
+-rw-r--r--   0 runner    (1001) docker     (123)      735 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/compliance_checker/tests/data/cf_example_cell_measures.cdl
+-rw-r--r--   0 runner    (1001) docker     (123)      889 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/compliance_checker/tests/data/chap2.cdl
+-rw-r--r--   0 runner    (1001) docker     (123)      654 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/compliance_checker/tests/data/climatology.cdl
+-rw-r--r--   0 runner    (1001) docker     (123)     1692 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/compliance_checker/tests/data/cont_ragged.cdl
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/compliance_checker/tests/data/conv_bad.cdl
+-rw-r--r--   0 runner    (1001) docker     (123)      351 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/compliance_checker/tests/data/conv_multi.cdl
+-rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/compliance_checker/tests/data/coordinate_types.cdl
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/compliance_checker/tests/data/coordinates_and_metadata.cdl
+-rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/compliance_checker/tests/data/dimension_order.cdl
+-rw-r--r--   0 runner    (1001) docker     (123)      491 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/compliance_checker/tests/data/dimensionless.cdl
+-rw-r--r--   0 runner    (1001) docker     (123)     1528 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/compliance_checker/tests/data/duplicate_axis.cdl
+-rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/compliance_checker/tests/data/example-grid.cdl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:30:11.087334 compliance-checker-5.1.0/compliance_checker/tests/data/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     9070 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/compliance_checker/tests/data/examples/3mf07.cdl
+-rw-r--r--   0 runner    (1001) docker     (123)      926 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/compliance_checker/tests/data/examples/bio_taxa.cdl
+-rw-r--r--   0 runner    (1001) docker     (123)      829 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/compliance_checker/tests/data/examples/cf_example_cell_measures.cdl
+-rw-r--r--   0 runner    (1001) docker     (123)     9443 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/compliance_checker/tests/data/examples/fvcom.cdl
+-rw-r--r--   0 runner    (1001) docker     (123)     4416 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/compliance_checker/tests/data/examples/glcfs.cdl
+-rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/compliance_checker/tests/data/examples/hycom_global.cdl
+-rw-r--r--   0 runner    (1001) docker     (123)     5779 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/compliance_checker/tests/data/examples/kibesillah.cdl
+-rw-r--r--   0 runner    (1001) docker     (123)    12628 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/compliance_checker/tests/data/examples/l01-met.cdl
+-rw-r--r--   0 runner    (1001) docker     (123)    20715 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/compliance_checker/tests/data/examples/ocos.cdl
+-rw-r--r--   0 runner    (1001) docker     (123)    11614 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/compliance_checker/tests/data/examples/ooi_glider.cdl
+-rw-r--r--   0 runner    (1001) docker     (123)    11003 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/compliance_checker/tests/data/examples/pr_inundation.cdl
+-rw-r--r--   0 runner    (1001) docker     (123)     2642 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/compliance_checker/tests/data/examples/sldmb_43093_agg.cdl
+-rw-r--r--   0 runner    (1001) docker     (123)    29171 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/compliance_checker/tests/data/examples/sp041.cdl
+-rw-r--r--   0 runner    (1001) docker     (123)     7257 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/compliance_checker/tests/data/examples/swan.cdl
+-rw-r--r--   0 runner    (1001) docker     (123)     3751 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/compliance_checker/tests/data/examples/usgs_dem_saipan.cdl
+-rw-r--r--   0 runner    (1001) docker     (123)     1242 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/compliance_checker/tests/data/examples/ww3.cdl
+-rw-r--r--   0 runner    (1001) docker     (123)      996 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/compliance_checker/tests/data/forecast_reference.cdl
+-rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/compliance_checker/tests/data/grid-boundaries.cdl
+-rw-r--r--   0 runner    (1001) docker     (123)     1820 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/compliance_checker/tests/data/grid_mapping_coordinates.cdl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:30:11.087334 compliance-checker-5.1.0/compliance_checker/tests/data/http_mocks/
+-rw-r--r--   0 runner    (1001) docker     (123)    17660 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/compliance_checker/tests/data/http_mocks/ncsos_describesensor.xml
+-rw-r--r--   0 runner    (1001) docker     (123)    10033 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/compliance_checker/tests/data/http_mocks/ncsos_getcapabilities.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      748 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/compliance_checker/tests/data/illegal-aux-coords.cdl
+-rw-r--r--   0 runner    (1001) docker     (123)      384 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/compliance_checker/tests/data/illegal-vertical.cdl
+-rw-r--r--   0 runner    (1001) docker     (123)    15780 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/compliance_checker/tests/data/index_ragged.cdl
+-rw-r--r--   0 runner    (1001) docker     (123)      720 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/compliance_checker/tests/data/index_ragged2.cdl
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/compliance_checker/tests/data/ints64.cdl
+-rw-r--r--   0 runner    (1001) docker     (123)     5951 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/compliance_checker/tests/data/ioos_1_1.cdl
+-rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/compliance_checker/tests/data/line_geometry.cdl
+-rw-r--r--   0 runner    (1001) docker     (123)     7038 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/compliance_checker/tests/data/mapping.cdl
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/compliance_checker/tests/data/multi-dim-coordinates.cdl
+-rw-r--r--   0 runner    (1001) docker     (123)     1014 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/compliance_checker/tests/data/multi-timeseries-incomplete.cdl
+-rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/compliance_checker/tests/data/multi-timeseries-orthogonal.cdl
+-rw-r--r--   0 runner    (1001) docker     (123)     6737 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/compliance_checker/tests/data/ncei_gold_point_1.cdl
+-rw-r--r--   0 runner    (1001) docker     (123)     7666 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/compliance_checker/tests/data/ncei_gold_point_2.cdl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:30:11.091334 compliance-checker-5.1.0/compliance_checker/tests/data/non-comp/
+-rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/compliance_checker/tests/data/non-comp/1d_bound_bad.cdl
+-rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/compliance_checker/tests/data/non-comp/bad-rhgrid.cdl
+-rw-r--r--   0 runner    (1001) docker     (123)     1616 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/compliance_checker/tests/data/non-comp/bad.cdl
+-rw-r--r--   0 runner    (1001) docker     (123)      843 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/compliance_checker/tests/data/non-comp/bad2dim.cdl
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/compliance_checker/tests/data/non-comp/badname.netcdf
+-rw-r--r--   0 runner    (1001) docker     (123)     1308 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/compliance_checker/tests/data/non-comp/bounds_bad_num_coords.cdl
+-rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/compliance_checker/tests/data/non-comp/bounds_bad_order.cdl
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/compliance_checker/tests/data/non-comp/empty.file
+-rw-r--r--   0 runner    (1001) docker     (123)    24004 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/compliance_checker/tests/data/non-comp/self_referencing.cdl
+-rw-r--r--   0 runner    (1001) docker     (123)      373 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/compliance_checker/tests/data/non-comp/time_units.cdl
+-rw-r--r--   0 runner    (1001) docker     (123)      930 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/compliance_checker/tests/data/point.cdl
+-rw-r--r--   0 runner    (1001) docker     (123)     1829 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/compliance_checker/tests/data/polygon_geometry.cdl
+-rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/compliance_checker/tests/data/profile-incomplete.cdl
+-rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/compliance_checker/tests/data/profile-orthogonal.cdl
+-rw-r--r--   0 runner    (1001) docker     (123)      628 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/compliance_checker/tests/data/reduced_horizontal_grid.cdl
+-rw-r--r--   0 runner    (1001) docker     (123)      421 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/compliance_checker/tests/data/rhgrid.cdl
+-rw-r--r--   0 runner    (1001) docker     (123)     1362 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/compliance_checker/tests/data/rotated_pole_grid.cdl
+-rw-r--r--   0 runner    (1001) docker     (123)    43335 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/compliance_checker/tests/data/ru07-20130824T170228_rt0.cdl
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/compliance_checker/tests/data/scalar_coordinate_variable.cdl
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/compliance_checker/tests/data/self-referencing-var.cdl
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/compliance_checker/tests/data/string_type_variable.cdl
+-rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/compliance_checker/tests/data/taxonomy_example.cdl
+-rw-r--r--   0 runner    (1001) docker     (123)      924 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/compliance_checker/tests/data/test_cdl.cdl
+-rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/compliance_checker/tests/data/test_cdl_nc4_file.cdl
+-rw-r--r--   0 runner    (1001) docker     (123)      924 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/compliance_checker/tests/data/test_cdl_nc_file.cdl
+-rw-r--r--   0 runner    (1001) docker     (123)      936 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/compliance_checker/tests/data/test_cdl_nc_file.nc
+-rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/compliance_checker/tests/data/timeseries-profile-incomplete.cdl
+-rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/compliance_checker/tests/data/timeseries-profile-multi-ortho-time.cdl
+-rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/compliance_checker/tests/data/timeseries-profile-multi-station.cdl
+-rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/compliance_checker/tests/data/timeseries-profile-ortho-depth.cdl
+-rw-r--r--   0 runner    (1001) docker     (123)      974 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/compliance_checker/tests/data/timeseries-profile-single-ortho-time.cdl
+-rw-r--r--   0 runner    (1001) docker     (123)      968 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/compliance_checker/tests/data/timeseries-profile-single-station.cdl
+-rw-r--r--   0 runner    (1001) docker     (123)      924 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/compliance_checker/tests/data/timeseries.cdl
+-rw-r--r--   0 runner    (1001) docker     (123)      832 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/compliance_checker/tests/data/trajectory-complete.cdl
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/compliance_checker/tests/data/trajectory-implied.cdl
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/compliance_checker/tests/data/trajectory-profile-incomplete.cdl
+-rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/compliance_checker/tests/data/trajectory-profile-orthogonal.cdl
+-rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/compliance_checker/tests/data/trajectory-single.cdl
+-rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/compliance_checker/tests/data/trajectory.cdl
+-rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/compliance_checker/tests/data/units_check.cdl
+-rw-r--r--   0 runner    (1001) docker     (123)    14798 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/compliance_checker/tests/data/valid_coordinates.cdl
+-rw-r--r--   0 runner    (1001) docker     (123)      797 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/compliance_checker/tests/data/vertical_coords.cdl
+-rw-r--r--   0 runner    (1001) docker     (123)     8520 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/compliance_checker/tests/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8379 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/compliance_checker/tests/resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21272 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/compliance_checker/tests/test_acdd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6756 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/compliance_checker/tests/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)   159694 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/compliance_checker/tests/test_cf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23267 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/compliance_checker/tests/test_cf_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6835 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/compliance_checker/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30458 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/compliance_checker/tests/test_feature_detection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49736 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/compliance_checker/tests/test_ioos_profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2717 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/compliance_checker/tests/test_ioos_sos.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1673 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/compliance_checker/tests/test_protocols.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10610 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/compliance_checker/tests/test_suite.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1578 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/compliance_checker/tests/test_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1469 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/compliance_checker/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:30:11.059334 compliance-checker-5.1.0/compliance_checker.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    24320 2023-05-17 22:30:10.000000 compliance-checker-5.1.0/compliance_checker.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9359 2023-05-17 22:30:11.000000 compliance-checker-5.1.0/compliance_checker.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 22:30:10.000000 compliance-checker-5.1.0/compliance_checker.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-05-17 22:30:10.000000 compliance-checker-5.1.0/compliance_checker.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-05-17 22:30:10.000000 compliance-checker-5.1.0/compliance_checker.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-17 22:30:10.000000 compliance-checker-5.1.0/compliance_checker.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:30:11.091334 compliance-checker-5.1.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:30:11.091334 compliance-checker-5.1.0/docs/source/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:30:11.091334 compliance-checker-5.1.0/docs/source/_templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:30:11.091334 compliance-checker-5.1.0/docs/source/_templates/autosummary/
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/docs/source/_templates/autosummary/base.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/docs/source/_templates/autosummary/class.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/docs/source/_templates/autosummary/module.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      654 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/docs/source/_templates/layout.html
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/docs/source/_templates/versions.html
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/docs/source/compliance_checker_api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4878 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2583 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/docs/source/faq.md
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      819 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-17 22:30:11.091334 compliance-checker-5.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2948 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/test_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/tox.ini
```

### Comparing `compliance-checker-5.0.2/.github/ISSUE_TEMPLATE/compliance-checker-issue-report.md` & `compliance-checker-5.1.0/.github/ISSUE_TEMPLATE/compliance-checker-issue-report.md`

 * *Files identical despite different names*

### Comparing `compliance-checker-5.0.2/.github/workflows/cc-checker-ugrid-test.yml` & `compliance-checker-5.1.0/.github/workflows/cc-checker-ugrid-test.yml`

 * *Files 24% similar despite different names*

```diff
@@ -1,43 +1,34 @@
 name: UGRID Plugin Tests
 
 on:
   pull_request:
   push:
-    branches: [master]
 
 jobs:
   run:
     runs-on: ubuntu-latest
 
     steps:
-    - uses: actions/checkout@v2
+    - uses: actions/checkout@v3
 
-    - name: Setup Conda
-      uses: s-weigand/setup-conda@v1
+    - name: Setup Micromamba
+      uses: mamba-org/provision-with-micromamba@v15
       with:
-        activate-conda: false
-        conda-channels: conda-forge
+        environment-file: false
 
-    - name: Python ${{ matrix.python-version }}
+    - name: Setup Env
       shell: bash -l {0}
-      run: |
-        conda create --name TEST python=${{ matrix.python-version }} python=3 pip --file requirements.txt --file test_requirements.txt --strict-channel-priority
-        source activate TEST
-        pip install -e . --no-deps --force-reinstall
-
-    - name: Conda Info
-      shell: bash -l {0}
-      run: |
-        source activate TEST
-        conda info --all
-        conda list
+      run: >
+        micromamba create --name TEST python=3 pip --file requirements.txt --file test_requirements.txt --channel conda-forge
+        && micromamba activate TEST
+        && pip install -e . --no-deps --force-reinstall
 
     - name: cc-plugin-glider tests
       shell: bash -l {0}
-      run: |
-        source activate TEST
-        git clone https://github.com/ioos/cc-checker-ugrid.git
-        cd cc-checker-ugrid
-        pip install -e . --no-deps --force-reinstall
-        conda install --file requirements.txt --file requirements-dev.txt ;
-        pytest -s -rxs -v cc_plugin_ugrid
+      run: >
+        micromamba activate TEST
+        && git clone https://github.com/ioos/cc-checker-ugrid.git
+        && cd cc-checker-ugrid
+        && micromamba install --file requirements.txt --file requirements-dev.txt --channel conda-forge
+        && pip install -e . --no-deps --force-reinstall
+        && pytest -s -rxs -v cc_plugin_ugrid
```

### Comparing `compliance-checker-5.0.2/.github/workflows/cc-plugin-glider-test.yml` & `compliance-checker-5.1.0/.github/workflows/cc-plugin-sgrid-test.yml`

 * *Files 17% similar despite different names*

```diff
@@ -1,42 +1,33 @@
-name: Glider Plugin Tests
+name: SGRID Plugin Tests
 
 on:
   pull_request:
   push:
-    branches: [master]
 
 jobs:
   run:
     runs-on: ubuntu-latest
 
     steps:
-    - uses: actions/checkout@v2
+    - uses: actions/checkout@v3
 
-    - name: Setup Conda
-      uses: s-weigand/setup-conda@v1
+    - name: Setup Micromamba
+      uses: mamba-org/provision-with-micromamba@v15
       with:
-        activate-conda: false
-        conda-channels: conda-forge
+        environment-file: false
 
-    - name: Python ${{ matrix.python-version }}
+    - name: Setup Env
       shell: bash -l {0}
-      run: |
-        conda create --name TEST python=${{ matrix.python-version }} python=3 pip --file requirements.txt --file test_requirements.txt --strict-channel-priority
-        source activate TEST
-        pip install -e . --no-deps --force-reinstall
-
-    - name: Conda Info
-      shell: bash -l {0}
-      run: |
-        source activate TEST
-        conda info --all
-        conda list
+      run: >
+        micromamba create --name TEST python=3 pip --file requirements.txt --file test_requirements.txt --channel conda-forge
+        && micromamba activate TEST
+        && pip install -e . --no-deps --force-reinstall
 
     - name: cc-plugin-glider tests
       shell: bash -l {0}
-      run: |
-        source activate TEST
-        git clone https://github.com/ioos/cc-plugin-glider.git
-        cd cc-plugin-glider
-        conda install --file requirements.txt --file requirements-dev.txt ;
-        pytest -s -rxs -v cc_plugin_glider
+      run: >
+        micromamba activate TEST
+        && git clone https://github.com/ioos/cc-plugin-sgrid.git
+        && cd cc-plugin-sgrid
+        && pip install -e . --no-deps --force-reinstall
+        && pytest -s -rxs -v cc_plugin_sgrid
```

### Comparing `compliance-checker-5.0.2/.github/workflows/cc-plugin-sgrid-test.yml` & `compliance-checker-5.1.0/.github/workflows/default-tests.yml`

 * *Files 26% similar despite different names*

```diff
@@ -1,42 +1,35 @@
-name: SGRID Plugin Tests
+name: Default Tests
 
 on:
   pull_request:
   push:
-    branches: [master]
 
 jobs:
   run:
-    runs-on: ubuntu-latest
+    runs-on: ${{ matrix.os }}
+    strategy:
+      matrix:
+        python-version: ["3.7", "3.8", "3.9", "3.10", "3.11"]
+        os: [windows-latest, ubuntu-latest, macos-latest]
+      fail-fast: false
 
     steps:
-    - uses: actions/checkout@v2
+    - uses: actions/checkout@v3
 
-    - name: Setup Conda
-      uses: s-weigand/setup-conda@v1
+    - name: Setup Micromamba
+      uses: mamba-org/provision-with-micromamba@v15
       with:
-        activate-conda: false
-        conda-channels: conda-forge
+        environment-file: false
 
-    - name: Python ${{ matrix.python-version }}
+    - name: Setup Env ${{ matrix.python-version }}
       shell: bash -l {0}
-      run: |
-        conda create --name TEST python=${{ matrix.python-version }} python=3 pip --file requirements.txt --file test_requirements.txt --strict-channel-priority
-        source activate TEST
-        pip install -e . --no-deps --force-reinstall
-
-    - name: Conda Info
-      shell: bash -l {0}
-      run: |
-        source activate TEST
-        conda info --all
-        conda list
+      run: >
+        micromamba create --name TEST python=${{ matrix.python-version }} pip --file requirements.txt --file test_requirements.txt --channel conda-forge
+        && micromamba activate TEST
+        && pip install -e . --no-deps --force-reinstall
 
-    - name: cc-plugin-glider tests
+    - name: Default Tests
       shell: bash -l {0}
       run: |
-        source activate TEST
-        git clone https://github.com/ioos/cc-plugin-sgrid.git
-        cd cc-plugin-sgrid
-        conda install --file requirements.txt --file requirements-dev.txt ;
-        pytest -s -rxs -v cc_plugin_sgrid
+        micromamba activate TEST
+        pytest -s -rxs -v -k "not integration" compliance_checker
```

### Comparing `compliance-checker-5.0.2/.github/workflows/codecov.yml` & `compliance-checker-5.1.0/.github/workflows/codecov.yml`

 * *Files 18% similar despite different names*

```diff
@@ -1,55 +1,39 @@
 name: Code coverage report
 
 on:
   pull_request:
   push:
-    branches:
-    - master
-    - develop
 
 jobs:
   run:
-    runs-on: ${{ matrix.os }}
-    strategy:
-      matrix:
-        python-version: ["3.10"]
-        os: [ubuntu-latest]
-      fail-fast: false
+    runs-on: ubuntu-latest
 
     steps:
-    - uses: actions/checkout@v2
+    - uses: actions/checkout@v3
 
-    - name: Setup Conda
-      uses: s-weigand/setup-conda@v1
+    - name: Setup Micromamba
+      uses: mamba-org/provision-with-micromamba@v15
       with:
-        activate-conda: false
-        conda-channels: conda-forge
+        environment-file: false
 
-    - name: Python ${{ matrix.python-version }}
+    - name: Setup Env
       shell: bash -l {0}
-      run: |
-        conda create --name TEST python=${{ matrix.python-version }} pip --file requirements.txt --file test_requirements.txt --strict-channel-priority
-        source activate TEST
-        pip install -e . --no-deps --force-reinstall
-
-    - name: Conda Info
-      shell: bash -l {0}
-      run: |
-        source activate TEST
-        conda info --all
-        conda list
+      run: >
+        micromamba create --name TEST python=3 pip --file requirements.txt --file test_requirements.txt --channel conda-forge
+        && micromamba activate TEST
+        && pip install -e . --no-deps --force-reinstall
 
     - name: Run tests with coverage
       shell: bash -l {0}
       run: |
-        source activate TEST
+        micromamba activate TEST
         pytest --cov=compliance_checker --cov-report=xml compliance_checker/tests
       # pass this step even if there are individual test failures, we are
       # interested in the overall level of coverage and other checks can
       # report on test failures.
       continue-on-error: true
 
     - name: Upload to codecov
-      uses: codecov/codecov-action@v2
+      uses: codecov/codecov-action@v3
       with:
         files: coverage.xml
```

### Comparing `compliance-checker-5.0.2/.github/workflows/integration-tests.yml` & `compliance-checker-5.1.0/.github/workflows/integration-tests.yml`

 * *Files 25% similar despite different names*

```diff
@@ -1,39 +1,30 @@
 name: Integration Tests
 
 on:
   pull_request:
   push:
-    branches: [master]
 
 jobs:
   run:
     runs-on: ubuntu-latest
 
     steps:
-    - uses: actions/checkout@v2
+    - uses: actions/checkout@v3
 
-    - name: Setup Conda
-      uses: s-weigand/setup-conda@v1
+    - name: Setup Micromamba
+      uses: mamba-org/provision-with-micromamba@v15
       with:
-        activate-conda: false
-        conda-channels: conda-forge
+        environment-file: false
 
-    - name: Python ${{ matrix.python-version }}
+    - name: Setup Env
       shell: bash -l {0}
-      run: |
-        conda create --name TEST python=${{ matrix.python-version }} python=3 pip --file requirements.txt --file test_requirements.txt --strict-channel-priority
-        source activate TEST
-        pip install -e . --no-deps --force-reinstall
-
-    - name: Conda Info
-      shell: bash -l {0}
-      run: |
-        source activate TEST
-        conda info --all
-        conda list
+      run: >
+        micromamba create --name TEST python=3 pip --file requirements.txt --file test_requirements.txt --channel conda-forge
+        && micromamba activate TEST
+        && pip install -e . --no-deps --force-reinstall
 
     - name: Integration Tests
       shell: bash -l {0}
       run: |
-        source activate TEST
-        pytest -m "integration" -s -rxs -v compliance_checker
+        micromamba activate TEST
+        pytest -m "integration" -s -rxs -v --vcr-record=none compliance_checker
```

### Comparing `compliance-checker-5.0.2/.github/workflows/publish.yml` & `compliance-checker-5.1.0/.github/workflows/pypi.yml`

 * *Files 15% similar despite different names*

```diff
@@ -1,46 +1,53 @@
 name: Publish to PyPI
 
 on:
+  pull_request:
+  push:
   release:
     types:
       - published
 
+defaults:
+  run:
+    shell: bash
+
 jobs:
   packages:
     runs-on: ubuntu-latest
     steps:
-    - uses: actions/checkout@v2
-
-    - name: Set up Python
-      uses: actions/setup-python@v1
+    - uses: actions/checkout@v3
       with:
-        python-version: 3.x
+        # Should be enough for setuptools-scm
+        fetch-depth: 100
+        persist-credentials: false
 
     - name: Get tags
-      run: git fetch --depth=1 origin +refs/tags/*:refs/tags/*
-      shell: bash
+      run: git fetch origin 'refs/tags/*:refs/tags/*'
+
+    - name: Set up Python
+      uses: actions/setup-python@v4
+      with:
+        python-version: "3.11"
 
     - name: Install build tools
       run: |
-        python -m pip install --upgrade pip wheel "setuptools>=41.2" setuptools_scm build twine
-      shell: bash
+        python -m pip install --upgrade pip build twine
 
-    - name: Build source distribution and binary wheel
+    - name: Build binary wheel
       run: python -m build --sdist --wheel . --outdir dist
 
     - name: CheckFiles
       run: |
-        ls dist
-      shell: bash
+        ls -lh dist
 
     - name: Test wheels
       run: |
         cd dist && python -m pip install compliance_checker*.whl
         python -m twine check *
-      shell: bash
 
-    - name: PyPI build
-      uses: pypa/gh-action-pypi-publish@master
+    - name: Publish a Python distribution to PyPI
+      if: success() && github.event_name == 'release'
+      uses: pypa/gh-action-pypi-publish@release/v1
       with:
         user: __token__
         password: ${{ secrets.PYPI_ACCESS_TOKEN }}
```

### Comparing `compliance-checker-5.0.2/.gitignore` & `compliance-checker-5.1.0/.gitignore`

 * *Files 14% similar despite different names*

```diff
@@ -85,15 +85,14 @@
 .venv/
 venv/
 ENV/
 
 # IDE project settings
 .spyderproject
 .vscode
-pyrightconfig.json
 
 # Rope project settings
 .ropeproject
 
 # Mac
 .DS_Store
 
@@ -107,7 +106,11 @@
 compliance_checker/_version.py
 .venv
 activate
 
 # coverage output
 coverage/
 coverage.xml
+
+# shpinx docs
+docs/source/generated/
+docs/source/quickintro.md
```

### Comparing `compliance-checker-5.0.2/.pre-commit-config.yaml` & `compliance-checker-5.1.0/.pre-commit-config.yaml`

 * *Files 25% similar despite different names*

```diff
@@ -1,51 +1,60 @@
 repos:
 - repo: https://github.com/pre-commit/pre-commit-hooks
-  rev: v4.2.0
+  rev: v4.4.0
   hooks:
     - id: trailing-whitespace
       exclude: compliance_checker/tests/data
     - id: check-ast
     - id: debug-statements
     - id: end-of-file-fixer
       exclude: compliance_checker/tests/data
     - id: check-docstring-first
     - id: check-added-large-files
+    - id: check-json
+    - id: check-merge-conflict
+    - id: check-yaml
     - id: requirements-txt-fixer
-
-- repo: https://github.com/PyCQA/flake8
-  rev: 4.0.1
-  hooks:
-    - id: flake8
-      exclude: docs/source/conf.py
-      args: [--max-line-length=200, "--ignore=E203,E501,W503", "--select=select=C,E,F,W,B,B950"]
-
-- repo: https://github.com/pycqa/isort
-  rev: 5.10.1
-  hooks:
-  - id: isort
-    additional_dependencies: [toml]
-    args: ["--profile", "black", "--filter-files"]
+      args:
+        - requirements.txt
+        - test_requirements.txt
 
 - repo: https://github.com/psf/black
-  rev: 22.3.0
+  rev: 23.3.0
   hooks:
   - id: black
     language_version: python3
 
+- repo: https://github.com/asottile/add-trailing-comma
+  rev: v2.4.0
+  hooks:
+    - id: add-trailing-comma
+
+
+- repo: https://github.com/charliermarsh/ruff-pre-commit
+  rev: v0.0.267
+  hooks:
+    - id: ruff
+
+- repo: https://github.com/tox-dev/pyproject-fmt
+  rev: 0.11.2
+  hooks:
+    - id: pyproject-fmt
+
 - repo: https://github.com/codespell-project/codespell
-  rev: v2.1.0
+  rev: v2.2.4
   hooks:
     - id: codespell
       args:
-        - --ignore-words-list=degreee,varn,poit,uint,sur,herat,claus
+        - --ignore-words-list=degreeE,degreee,varn,poit,uint,sur,herat,claus,tung,messsages
       exclude: >
           (?x)^(
               .*\.xml|
               .*\.cdl|
+              .*\.yaml|
               .*_version.py|
               .*versioneer.py
           )$
 
 ci:
     autofix_commit_msg: |
         [pre-commit.ci] auto fixes from pre-commit.com hooks
```

### Comparing `compliance-checker-5.0.2/LICENSE` & `compliance-checker-5.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `compliance-checker-5.0.2/PKG-INFO` & `compliance-checker-5.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: compliance-checker
-Version: 5.0.2
+Version: 5.1.0
 Summary: Checks Datasets and SOS endpoints for standards compliance
 Home-page: https://github.com/ioos/compliance-checker
 Author: Dave Foster
 Author-email: dave@axiomdatascience.com
 License: Apache License 2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -17,44 +17,44 @@
 Classifier: Topic :: Scientific/Engineering
 Requires-Python: ~=3.5
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # IOOS Compliance Checker
 
-[![Build Status](https://travis-ci.org/ioos/compliance-checker.svg)](https://travis-ci.org/ioos/compliance-checker)
-[![codecov](https://codecov.io/gh/ioos/compliance-checker/branch/master/graph/badge.svg)](https://codecov.io/gh/ioos/compliance-checker)
+[![Tests](https://github.com/ioos/compliance-checker/actions/workflows/default-tests.yml/badge.svg)](https://github.com/ioos/compliance-checker/actions/workflows/default-tests.yml)
+[![codecov](https://codecov.io/gh/ioos/compliance-checker/branch/develop/graph/badge.svg)](https://app.codecov.io/gh/ioos/compliance-checker)
 
 The IOOS Compliance Checker is a python based tool for data providers to check
 for completeness and community standard compliance of local or remote
 [netCDF](https://en.wikipedia.org/wiki/NetCDF) files against
 [CF](http://cfconventions.org/Data/cf-conventions/cf-conventions-1.7/cf-conventions.html) and
-[ACDD](http://wiki.esipfed.org/index.php/Attribute_Convention_for_Data_Discovery_1-3)
+[ACDD](https://wiki.esipfed.org/Attribute_Convention_for_Data_Discovery_1-3)
 file standards. The python module can be used as a command-line tool or as a
 library that can be integrated into other software.
 
-A [web-based version](https://data.ioos.us/compliance/index.html) of the Compliance
+A [web-based version](https://compliance.ioos.us/index.html) of the Compliance
 Checker was developed to enable a broader audience and improve accessibility for the
 checker. With the web version, providers can simply provide a link or upload their
 datasets and get the full suite of capabilities that Compliance Checker offers.
 
 
 It currently supports the following sources and standards:
 
-| Standard                                                                                                                            | Source                                                            | .nc/OPeNDAP/.cdl | SOS                             |
-| ----------------------------------------------------------------------------------------------------                                | -----------                                                       | ------           | ------------------------------- |
-| [ACDD (1.1, 1.3)](http://wiki.esipfed.org/index.php/Attribute_Convention_for_Data_Discovery_1-3)                                    | Built-in                                                          | X                | -                               |
-| [CF (1.8)](http://cfconventions.org/Data/cf-conventions/cf-conventions-1.8/cf-conventions.html)                                     | Built-in                                                          | X                | -                               |
-| [CF (1.7)](http://cfconventions.org/Data/cf-conventions/cf-conventions-1.7/cf-conventions.html)                                     | Built-in                                                          | X                | -                               |
-| [CF (1.6)](http://cfconventions.org/cf-conventions/v1.6.0/cf-conventions.html)                                                      | Built-in                                                          | X                | -                               |
-| IOOS SOS                                                                                                                            | Built-in                                                          | -                | GetCapabilities, DescribeSensor |
+| Standard                                                                                                                   | Source                                                            | .nc/OPeNDAP/.cdl | SOS                             |
+| ----------------------------------------------------------------------------------------------------                       | -----------                                                       | ------           | ------------------------------- |
+| [ACDD (1.1, 1.3)](https://wiki.esipfed.org/Attribute_Convention_for_Data_Discovery_1-3)                                    | Built-in                                                          | X                | -                               |
+| [CF (1.8)](http://cfconventions.org/Data/cf-conventions/cf-conventions-1.8/cf-conventions.html)                            | Built-in                                                          | X                | -                               |
+| [CF (1.7)](http://cfconventions.org/Data/cf-conventions/cf-conventions-1.7/cf-conventions.html)                            | Built-in                                                          | X                | -                               |
+| [CF (1.6)](http://cfconventions.org/cf-conventions/v1.6.0/cf-conventions.html)                                             | Built-in                                                          | X                | -                               |
+| IOOS SOS                                                                                                                   | Built-in                                                          | -                | GetCapabilities, DescribeSensor |
 | [IOOS (1.1)](https://ioos.github.io/ioos-metadata/ioos-metadata-profile-v1-1.html#ioos-netcdf-metadata-profile-attributes) | Built-in                                                          | X                | -                               |
-| [IOOS (1.2)](https://ioos.github.io/ioos-metadata/ioos-metadata-profile-v1-2.html) | Built-in                                                          | X                | -                               |
-| [Glider DAC](https://github.com/ioos/ioosngdac/wiki/NGDAC-NetCDF-File-Format-Version-2)                                             | [ioos/cc-plugin-glider](https://github.com/ioos/cc-plugin-glider) | X                | -                               |
-| [NCEI (1.1, 2.0)](https://www.nodc.noaa.gov/data/formats/netcdf/v2.0/)                                                              | [ioos/cc-plugin-ncei](https://github.com/ioos/cc-plugin-ncei)     | X                | -                               |
+| [IOOS (1.2)](https://ioos.github.io/ioos-metadata/ioos-metadata-profile-v1-2.html)                                         | Built-in                                                          | X                | -                               |
+| [Glider DAC](https://github.com/ioos/ioosngdac/wiki/NetCDF-Specification)                                                  | [ioos/cc-plugin-glider](https://github.com/ioos/cc-plugin-glider) | X                | -                               |
+| [NCEI (1.1, 2.0)](https://www.ncei.noaa.gov/data/oceans/ncei/formats/netcdf/v2.0/index.html)                               | [ioos/cc-plugin-ncei](https://github.com/ioos/cc-plugin-ncei)     | X                | -                               |
 
 
 ## Advice to data providers
 
 While the command-line version of this tool can be run in a loop, it is not necessary to check
 every file if they are all created the same way. In short, this tool is not meant for
 identifying bugs in your data processing stream. It is, however, intended to help you identify
@@ -62,19 +62,19 @@
 for any reason it would be worth your while to run one file through the Compliance Checker to
 insure you procedure change does not impact your file’s compliance.
 
 If you feel you will need to run a batch of files through the Compliance Checker, please contact
 the IOOS Program Office Operations Division for assistance.
 
 
-# [The Compliance Checker Web Tool](https://data.ioos.us/compliance/)
+# [The Compliance Checker Web Tool](https://compliance.ioos.us/index.html)
 
 The IOOS Compliance Checker front end companion.
 
-[https://data.ioos.us/compliance/](https://data.ioos.us/compliance/)
+[https://compliance.ioos.us/index.html](https://compliance.ioos.us/index.html)
 
 Source Code is available on GitHub:
 
 [https://github.com/ioos/compliance-checker-web](https://github.com/ioos/compliance-checker-web)
 
 ## Usage
 Select the test you want to run from the dropdown menu. Then, either upload your dataset or provide a url to a
@@ -91,19 +91,19 @@
 users interested in batch processing files hosted via OPeNDAP. Details on how to use the API are
 available on the Compliance Checker Web [wiki page](https://github.com/ioos/compliance-checker-web/wiki/API).
 
 Here are a couple examples:
 
 **HTML Output**
 
-https://data.ioos.us/compliance/api/run?report_format=html&test=acdd&url=http://sos.maracoos.org/stable/dodsC/hrecos/stationHRMARPH-agg.ncml
+https://compliance.ioos.us/index.htmlapi/run?report_format=html&test=acdd&url=http://sos.maracoos.org/stable/dodsC/hrecos/stationHRMARPH-agg.ncml
 
 **JSON Output**
 
-https://data.ioos.us/compliance/api/run?report_format=json&test=acdd&url=http://sos.maracoos.org/stable/dodsC/hrecos/stationHRMARPH-agg.ncml
+https://compliance.ioos.us/index.htmlapi/run?report_format=json&test=acdd&url=http://sos.maracoos.org/stable/dodsC/hrecos/stationHRMARPH-agg.ncml
 
 # The Compliance Checker Command Line Tool
 
 
 ## Concepts & Terminology
 
 Each compliance standard is executed by a Check Suite,
@@ -388,28 +388,28 @@
     scored = cc_data[cc_test[0]]['scored_points']
     possible = cc_data[cc_test[0]]['possible_points']
     log.debug('CC Scored {} out of {} possible points'.format(scored, possible))
 ```
 
 ## Compliance Checker Plug-Ins
 
-Separate Plug-ins have been developed to complement the master Compliance Checker tool with
+Separate Plug-ins have been developed to complement the Compliance Checker tool with
 specifications for preparing data to be submitted to different data assembly centers.
 The version numbering of these plug-ins are not necessarily link to the version of the
-master Compliance Checker, but they are all designed to run with the master Compliance Checker tool.
+Compliance Checker, but they are all designed to run with the Compliance Checker tool.
 
 ### Current Plug-in Releases:
 
 - [GliderDAC](https://github.com/ioos/cc-plugin-glider/releases)
 
-This is a checker for [GliderDAC](https://github.com/ioos/ioosngdac/wiki/NGDAC-NetCDF-File-Format-Version-2) files
+This is a checker for [GliderDAC](https://github.com/ioos/ioosngdac/wiki/NetCDF-Specification) files
 
 - [NCEI](https://github.com/ioos/cc-plugin-ncei/releases) - [link](https://github.com/ioos/cc-plugin-ncei)
 
-This is a checker for NCEI netCDF Templates [v1.1](https://www.nodc.noaa.gov/data/formats/netcdf/v1.1/) and [v2.0](https://www.nodc.noaa.gov/data/formats/netcdf/v2.0/) files.
+This is a checker for NCEI netCDF Templates [v1.1](https://www.ncei.noaa.gov/data/oceans/ncei/formats/netcdf/v1.1/index.html) and [v2.0](https://www.ncei.noaa.gov/data/oceans/ncei/formats/netcdf/v2.0/index.html) files.
 
 These plug-ins must be installed separately but work on top of the base compliance checker software.
 
 ```
 pip install cc-plugin-ncei
 ```
```

### Comparing `compliance-checker-5.0.2/README.md` & `compliance-checker-5.1.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,39 +1,39 @@
 # IOOS Compliance Checker
 
-[![Build Status](https://travis-ci.org/ioos/compliance-checker.svg)](https://travis-ci.org/ioos/compliance-checker)
-[![codecov](https://codecov.io/gh/ioos/compliance-checker/branch/master/graph/badge.svg)](https://codecov.io/gh/ioos/compliance-checker)
+[![Tests](https://github.com/ioos/compliance-checker/actions/workflows/default-tests.yml/badge.svg)](https://github.com/ioos/compliance-checker/actions/workflows/default-tests.yml)
+[![codecov](https://codecov.io/gh/ioos/compliance-checker/branch/develop/graph/badge.svg)](https://app.codecov.io/gh/ioos/compliance-checker)
 
 The IOOS Compliance Checker is a python based tool for data providers to check
 for completeness and community standard compliance of local or remote
 [netCDF](https://en.wikipedia.org/wiki/NetCDF) files against
 [CF](http://cfconventions.org/Data/cf-conventions/cf-conventions-1.7/cf-conventions.html) and
-[ACDD](http://wiki.esipfed.org/index.php/Attribute_Convention_for_Data_Discovery_1-3)
+[ACDD](https://wiki.esipfed.org/Attribute_Convention_for_Data_Discovery_1-3)
 file standards. The python module can be used as a command-line tool or as a
 library that can be integrated into other software.
 
-A [web-based version](https://data.ioos.us/compliance/index.html) of the Compliance
+A [web-based version](https://compliance.ioos.us/index.html) of the Compliance
 Checker was developed to enable a broader audience and improve accessibility for the
 checker. With the web version, providers can simply provide a link or upload their
 datasets and get the full suite of capabilities that Compliance Checker offers.
 
 
 It currently supports the following sources and standards:
 
-| Standard                                                                                                                            | Source                                                            | .nc/OPeNDAP/.cdl | SOS                             |
-| ----------------------------------------------------------------------------------------------------                                | -----------                                                       | ------           | ------------------------------- |
-| [ACDD (1.1, 1.3)](http://wiki.esipfed.org/index.php/Attribute_Convention_for_Data_Discovery_1-3)                                    | Built-in                                                          | X                | -                               |
-| [CF (1.8)](http://cfconventions.org/Data/cf-conventions/cf-conventions-1.8/cf-conventions.html)                                     | Built-in                                                          | X                | -                               |
-| [CF (1.7)](http://cfconventions.org/Data/cf-conventions/cf-conventions-1.7/cf-conventions.html)                                     | Built-in                                                          | X                | -                               |
-| [CF (1.6)](http://cfconventions.org/cf-conventions/v1.6.0/cf-conventions.html)                                                      | Built-in                                                          | X                | -                               |
-| IOOS SOS                                                                                                                            | Built-in                                                          | -                | GetCapabilities, DescribeSensor |
+| Standard                                                                                                                   | Source                                                            | .nc/OPeNDAP/.cdl | SOS                             |
+| ----------------------------------------------------------------------------------------------------                       | -----------                                                       | ------           | ------------------------------- |
+| [ACDD (1.1, 1.3)](https://wiki.esipfed.org/Attribute_Convention_for_Data_Discovery_1-3)                                    | Built-in                                                          | X                | -                               |
+| [CF (1.8)](http://cfconventions.org/Data/cf-conventions/cf-conventions-1.8/cf-conventions.html)                            | Built-in                                                          | X                | -                               |
+| [CF (1.7)](http://cfconventions.org/Data/cf-conventions/cf-conventions-1.7/cf-conventions.html)                            | Built-in                                                          | X                | -                               |
+| [CF (1.6)](http://cfconventions.org/cf-conventions/v1.6.0/cf-conventions.html)                                             | Built-in                                                          | X                | -                               |
+| IOOS SOS                                                                                                                   | Built-in                                                          | -                | GetCapabilities, DescribeSensor |
 | [IOOS (1.1)](https://ioos.github.io/ioos-metadata/ioos-metadata-profile-v1-1.html#ioos-netcdf-metadata-profile-attributes) | Built-in                                                          | X                | -                               |
-| [IOOS (1.2)](https://ioos.github.io/ioos-metadata/ioos-metadata-profile-v1-2.html) | Built-in                                                          | X                | -                               |
-| [Glider DAC](https://github.com/ioos/ioosngdac/wiki/NGDAC-NetCDF-File-Format-Version-2)                                             | [ioos/cc-plugin-glider](https://github.com/ioos/cc-plugin-glider) | X                | -                               |
-| [NCEI (1.1, 2.0)](https://www.nodc.noaa.gov/data/formats/netcdf/v2.0/)                                                              | [ioos/cc-plugin-ncei](https://github.com/ioos/cc-plugin-ncei)     | X                | -                               |
+| [IOOS (1.2)](https://ioos.github.io/ioos-metadata/ioos-metadata-profile-v1-2.html)                                         | Built-in                                                          | X                | -                               |
+| [Glider DAC](https://github.com/ioos/ioosngdac/wiki/NetCDF-Specification)                                                  | [ioos/cc-plugin-glider](https://github.com/ioos/cc-plugin-glider) | X                | -                               |
+| [NCEI (1.1, 2.0)](https://www.ncei.noaa.gov/data/oceans/ncei/formats/netcdf/v2.0/index.html)                               | [ioos/cc-plugin-ncei](https://github.com/ioos/cc-plugin-ncei)     | X                | -                               |
 
 
 ## Advice to data providers
 
 While the command-line version of this tool can be run in a loop, it is not necessary to check
 every file if they are all created the same way. In short, this tool is not meant for
 identifying bugs in your data processing stream. It is, however, intended to help you identify
@@ -41,19 +41,19 @@
 for any reason it would be worth your while to run one file through the Compliance Checker to
 insure you procedure change does not impact your file’s compliance.
 
 If you feel you will need to run a batch of files through the Compliance Checker, please contact
 the IOOS Program Office Operations Division for assistance.
 
 
-# [The Compliance Checker Web Tool](https://data.ioos.us/compliance/)
+# [The Compliance Checker Web Tool](https://compliance.ioos.us/index.html)
 
 The IOOS Compliance Checker front end companion.
 
-[https://data.ioos.us/compliance/](https://data.ioos.us/compliance/)
+[https://compliance.ioos.us/index.html](https://compliance.ioos.us/index.html)
 
 Source Code is available on GitHub:
 
 [https://github.com/ioos/compliance-checker-web](https://github.com/ioos/compliance-checker-web)
 
 ## Usage
 Select the test you want to run from the dropdown menu. Then, either upload your dataset or provide a url to a
@@ -70,19 +70,19 @@
 users interested in batch processing files hosted via OPeNDAP. Details on how to use the API are
 available on the Compliance Checker Web [wiki page](https://github.com/ioos/compliance-checker-web/wiki/API).
 
 Here are a couple examples:
 
 **HTML Output**
 
-https://data.ioos.us/compliance/api/run?report_format=html&test=acdd&url=http://sos.maracoos.org/stable/dodsC/hrecos/stationHRMARPH-agg.ncml
+https://compliance.ioos.us/index.htmlapi/run?report_format=html&test=acdd&url=http://sos.maracoos.org/stable/dodsC/hrecos/stationHRMARPH-agg.ncml
 
 **JSON Output**
 
-https://data.ioos.us/compliance/api/run?report_format=json&test=acdd&url=http://sos.maracoos.org/stable/dodsC/hrecos/stationHRMARPH-agg.ncml
+https://compliance.ioos.us/index.htmlapi/run?report_format=json&test=acdd&url=http://sos.maracoos.org/stable/dodsC/hrecos/stationHRMARPH-agg.ncml
 
 # The Compliance Checker Command Line Tool
 
 
 ## Concepts & Terminology
 
 Each compliance standard is executed by a Check Suite,
@@ -367,28 +367,28 @@
     scored = cc_data[cc_test[0]]['scored_points']
     possible = cc_data[cc_test[0]]['possible_points']
     log.debug('CC Scored {} out of {} possible points'.format(scored, possible))
 ```
 
 ## Compliance Checker Plug-Ins
 
-Separate Plug-ins have been developed to complement the master Compliance Checker tool with
+Separate Plug-ins have been developed to complement the Compliance Checker tool with
 specifications for preparing data to be submitted to different data assembly centers.
 The version numbering of these plug-ins are not necessarily link to the version of the
-master Compliance Checker, but they are all designed to run with the master Compliance Checker tool.
+Compliance Checker, but they are all designed to run with the Compliance Checker tool.
 
 ### Current Plug-in Releases:
 
 - [GliderDAC](https://github.com/ioos/cc-plugin-glider/releases)
 
-This is a checker for [GliderDAC](https://github.com/ioos/ioosngdac/wiki/NGDAC-NetCDF-File-Format-Version-2) files
+This is a checker for [GliderDAC](https://github.com/ioos/ioosngdac/wiki/NetCDF-Specification) files
 
 - [NCEI](https://github.com/ioos/cc-plugin-ncei/releases) - [link](https://github.com/ioos/cc-plugin-ncei)
 
-This is a checker for NCEI netCDF Templates [v1.1](https://www.nodc.noaa.gov/data/formats/netcdf/v1.1/) and [v2.0](https://www.nodc.noaa.gov/data/formats/netcdf/v2.0/) files.
+This is a checker for NCEI netCDF Templates [v1.1](https://www.ncei.noaa.gov/data/oceans/ncei/formats/netcdf/v1.1/index.html) and [v2.0](https://www.ncei.noaa.gov/data/oceans/ncei/formats/netcdf/v2.0/index.html) files.
 
 These plug-ins must be installed separately but work on top of the base compliance checker software.
 
 ```
 pip install cc-plugin-ncei
 ```
```

### Comparing `compliance-checker-5.0.2/cchecker.py` & `compliance-checker-5.1.0/cchecker.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,15 +30,15 @@
     :return: Dictionary with keys as checker type (i.e. "cf", "acdd")
     """
     options_dict = defaultdict(set)
     for opt_str in opts:
         try:
             checker_type, checker_opt = opt_str.split(":", 1)
         except ValueError:
-            warnings.warn("Could not split option {}, ignoring".format(opt_str))
+            warnings.warn(f"Could not split option {opt_str}, ignoring", stacklevel=2)
         else:
             options_dict[checker_type].add(checker_opt)
     return options_dict
 
 
 def main():
     # Load all available checker classes
@@ -108,28 +108,28 @@
                                     all checks and is equivalent to calling
                                     the first form. "M" will only show high
                                     priority output from the given check and
                                     will skip medium and low.  "L" will show
                                     both high and medium priority issues, while
                                     skipping low priority issues.  Cannot be
                                     used with `-i`/`--include-checks` option.
-                                    """
+                                    """,
         ),
         action="append",
     )
 
     include_exclude.add_argument(
         "--include-checks",
         "-i",
         help=dedent(
             """
                                     Specifies checks to include. Can only take the form
                                     of `<check_name>`.  Cannot be specified along with
                                     `-s`/`skip_checks`.
-                                    """
+                                    """,
         ),
         action="append",
     )
 
     parser.add_argument(
         "-f",
         "--format",
@@ -177,15 +177,15 @@
                                     checker name followed by the option, e.g.
                                     '<checker>:<option_name>'
 
                                     Available options:
                                     'cf:enable_appendix_a_checks' - Allow check
                                     results against CF Appendix A for attribute
                                     location and data types.
-                                    """
+                                    """,
         ),
     )
 
     parser.add_argument(
         "-V",
         "--version",
         action="store_true",
@@ -202,15 +202,18 @@
             "'application/x-netcdf', or an ERDDAP TableDAP endpoint. "
             "Note that the ERDDAP TableDAP endpoint will currently attempt "
             "to fetch the entire TableDAP dataset."
         ),
     )
 
     parser.add_argument(
-        "-l", "--list-tests", action="store_true", help="List the available tests"
+        "-l",
+        "--list-tests",
+        action="store_true",
+        help="List the available tests",
     )
 
     parser.add_argument(
         "-d",
         "--download-standard-names",
         help=(
             "Specify a version of the cf standard name table"
@@ -287,15 +290,15 @@
     # 2 modes, concatenated output file or multiple output files
     return_values = []
     had_errors = []
     if output_len == 1:
         if args.format != "json":
             print(
                 "Running Compliance Checker on the datasets from: {}".format(
-                    args.dataset_location
+                    args.dataset_location,
                 ),
                 file=sys.stderr,
             )
         return_value, errors = ComplianceChecker.run_checker(
             args.dataset_location,
             args.test or ["acdd"],
             args.verbose,
@@ -309,15 +312,15 @@
         return_values.append(return_value)
         had_errors.append(errors)
     else:
         for output, dataset in zip(args.output, args.dataset_location):
             if args.format != "json":
                 print(
                     "Running Compliance Checker on the dataset from: {}".format(
-                        dataset
+                        dataset,
                     ),
                     file=sys.stderr,
                 )
             return_value, errors = ComplianceChecker.run_checker(
                 [dataset],
                 args.test or ["acdd"],
                 args.verbose,
```

### Comparing `compliance-checker-5.0.2/compliance_checker/__init__.py` & `compliance-checker-5.1.0/compliance_checker/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     order to speed up repeated calls to the function.  This should only really
     be used against netCDF Datasets opened in 'r' mode, as the attributes should
     not change upon reading the files.
     """
 
     @lru_cache(128)
     def get_variables_by_attributes(self, **kwargs):
-        return super(MemoizedDataset, self).get_variables_by_attributes(**kwargs)
+        return super().get_variables_by_attributes(**kwargs)
 
 
 @contextmanager
 def tempnc(data: BinaryIO) -> Generator[str, None, None]:
     """
     Create a temporary in-memory NetCDF file using a NamedTemporaryFile.
     Close the file automatically after scope is exited.
```

### Comparing `compliance-checker-5.0.2/compliance_checker/acdd.py` & `compliance-checker-5.1.0/compliance_checker/acdd.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,22 +22,20 @@
     ratable_result,
 )
 from compliance_checker.cf.util import _possiblexunits, _possibleyunits
 from compliance_checker.util import dateparse, datetime_is_iso, kvp_convert
 
 
 class ACDDBaseCheck(BaseCheck):
-
     _cc_spec = "acdd"
     _cc_description = "Attribute Conventions for Dataset Discovery (ACDD)"
     _cc_url = "http://wiki.esipfed.org/index.php?title=Category:Attribute_Conventions_Dataset_Discovery"
     _cc_display_headers = {3: "Highly Recommended", 2: "Recommended", 1: "Suggested"}
 
     def __init__(self):
-
         self.high_rec_atts = ["title", "keywords", "summary"]
 
         self.rec_atts = [
             "id",
             "naming_authority",
             "history",
             "comment",
@@ -151,15 +149,15 @@
         for variable in self.get_applicable_variables(ds):
             msgs = []
             long_name = getattr(ds.variables[variable], "long_name", None)
             check = long_name is not None
             if not check:
                 msgs.append("long_name")
             results.append(
-                Result(BaseCheck.HIGH, check, self._var_header.format(variable), msgs)
+                Result(BaseCheck.HIGH, check, self._var_header.format(variable), msgs),
             )
 
         return results
 
     def check_var_standard_name(self, ds):
         """
         Checks each applicable variable for the standard_name attribute
@@ -170,15 +168,15 @@
         for variable in self.get_applicable_variables(ds):
             msgs = []
             std_name = getattr(ds.variables[variable], "standard_name", None)
             check = std_name is not None
             if not check:
                 msgs.append("standard_name")
             results.append(
-                Result(BaseCheck.HIGH, check, self._var_header.format(variable), msgs)
+                Result(BaseCheck.HIGH, check, self._var_header.format(variable), msgs),
             )
 
         return results
 
     def check_var_units(self, ds):
         """
         Checks each applicable variable for the units attribute
@@ -186,25 +184,28 @@
         :param netCDF4.Dataset ds: An open netCDF dataset
         """
         results = []
         for variable in self.get_applicable_variables(ds):
             msgs = []
             # Check units and dims for variable
             unit_check = hasattr(ds.variables[variable], "units")
-            no_dim_check = getattr(ds.variables[variable], "dimensions") == tuple()
+            no_dim_check = ds.variables[variable].dimensions == ()
             # Check if we have no dimensions.  If no dims, skip test
             if no_dim_check:
                 continue
             # Check if we have no units
             if not unit_check:
                 msgs.append("units")
             results.append(
                 Result(
-                    BaseCheck.HIGH, unit_check, self._var_header.format(variable), msgs
-                )
+                    BaseCheck.HIGH,
+                    unit_check,
+                    self._var_header.format(variable),
+                    msgs,
+                ),
             )
 
         return results
 
     def check_acknowledgment(self, ds):
         """
         Check if acknowledgment/acknowledgment attribute is present. Because
@@ -245,22 +246,21 @@
         except ValueError:
             return Result(
                 BaseCheck.MEDIUM,
                 False,
                 "geospatial_lat_extents_match",
                 [
                     "Could not convert one of geospatial_lat_min ({}) or max ({}) to float see CF-1.6 spec chapter 4.1"
-                    "".format(ds.geospatial_lat_min, ds.geospatial_lat_max)
+                    "".format(ds.geospatial_lat_min, ds.geospatial_lat_max),
                 ],
             )
 
         # identify lat var(s) as per CF 4.1
         lat_vars = {}  # var -> number of criteria passed
-        for name, var in ds.variables.items():
-
+        for _name, var in ds.variables.items():
             # must have units
             if not hasattr(var, "units"):
                 continue
 
             lat_vars[var] = 0
 
             # units in this set
@@ -280,47 +280,48 @@
 
         if len(lat_vars) == 0:
             return Result(
                 BaseCheck.MEDIUM,
                 False,
                 "geospatial_lat_extents_match",
                 [
-                    "Could not find lat variable to test extent of geospatial_lat_min/max, see CF-1.6 spec chapter 4.1"
+                    "Could not find lat variable to test extent of geospatial_lat_min/max, see CF-1.6 spec chapter 4.1",
                 ],
             )
 
         # sort by criteria passed
         final_lats = sorted(lat_vars, key=lambda x: lat_vars[x], reverse=True)
 
         obs_mins = {
             var._name: np.nanmin(var) for var in final_lats if not np.isnan(var).all()
         }
         obs_maxs = {
             var._name: np.nanmax(var) for var in final_lats if not np.isnan(var).all()
         }
 
-        min_pass = any((np.isclose(lat_min, min_val) for min_val in obs_mins.values()))
-        max_pass = any((np.isclose(lat_max, max_val) for max_val in obs_maxs.values()))
+        min_pass = any(np.isclose(lat_min, min_val) for min_val in obs_mins.values())
+        max_pass = any(np.isclose(lat_max, max_val) for max_val in obs_maxs.values())
 
         allpass = sum((min_pass, max_pass))
 
         msgs = []
         if not min_pass:
             msgs.append(
-                "Data for possible latitude variables (%s) did not match geospatial_lat_min value (%s)"
-                % (obs_mins, lat_min)
+                f"Data for possible latitude variables ({obs_mins}) did not match geospatial_lat_min value ({lat_min})",
             )
         if not max_pass:
             msgs.append(
-                "Data for possible latitude variables (%s) did not match geospatial_lat_max value (%s)"
-                % (obs_maxs, lat_max)
+                f"Data for possible latitude variables ({obs_maxs}) did not match geospatial_lat_max value ({lat_max})",
             )
 
         return Result(
-            BaseCheck.MEDIUM, (allpass, 2), "geospatial_lat_extents_match", msgs
+            BaseCheck.MEDIUM,
+            (allpass, 2),
+            "geospatial_lat_extents_match",
+            msgs,
         )
 
     def check_lon_extents(self, ds):
         """
         Check that the values of geospatial_lon_min/geospatial_lon_max
         approximately match the data.
 
@@ -343,22 +344,21 @@
         except ValueError:
             return Result(
                 BaseCheck.MEDIUM,
                 False,
                 "geospatial_lon_extents_match",
                 [
                     "Could not convert one of geospatial_lon_min ({}) or max ({}) to float see CF-1.6 spec chapter 4.1"
-                    "".format(ds.geospatial_lon_min, ds.geospatial_lon_max)
+                    "".format(ds.geospatial_lon_min, ds.geospatial_lon_max),
                 ],
             )
 
         # identify lon var(s) as per CF 4.2
         lon_vars = {}  # var -> number of criteria passed
-        for name, var in ds.variables.items():
-
+        for _name, var in ds.variables.items():
             # must have units
             if not hasattr(var, "units"):
                 continue
 
             lon_vars[var] = 0
 
             # units in this set
@@ -378,47 +378,48 @@
 
         if len(lon_vars) == 0:
             return Result(
                 BaseCheck.MEDIUM,
                 False,
                 "geospatial_lon_extents_match",
                 [
-                    "Could not find lon variable to test extent of geospatial_lon_min/max, see CF-1.6 spec chapter 4.2"
+                    "Could not find lon variable to test extent of geospatial_lon_min/max, see CF-1.6 spec chapter 4.2",
                 ],
             )
 
         # sort by criteria passed
         final_lons = sorted(lon_vars, key=lambda x: lon_vars[x], reverse=True)
 
         obs_mins = {
             var._name: np.nanmin(var) for var in final_lons if not np.isnan(var).all()
         }
         obs_maxs = {
             var._name: np.nanmax(var) for var in final_lons if not np.isnan(var).all()
         }
 
-        min_pass = any((np.isclose(lon_min, min_val) for min_val in obs_mins.values()))
-        max_pass = any((np.isclose(lon_max, max_val) for max_val in obs_maxs.values()))
+        min_pass = any(np.isclose(lon_min, min_val) for min_val in obs_mins.values())
+        max_pass = any(np.isclose(lon_max, max_val) for max_val in obs_maxs.values())
 
         allpass = sum((min_pass, max_pass))
 
         msgs = []
         if not min_pass:
             msgs.append(
-                "Data for possible longitude variables (%s) did not match geospatial_lon_min value (%s)"
-                % (obs_mins, lon_min)
+                f"Data for possible longitude variables ({obs_mins}) did not match geospatial_lon_min value ({lon_min})",
             )
         if not max_pass:
             msgs.append(
-                "Data for possible longitude variables (%s) did not match geospatial_lon_max value (%s)"
-                % (obs_maxs, lon_max)
+                f"Data for possible longitude variables ({obs_maxs}) did not match geospatial_lon_max value ({lon_max})",
             )
 
         return Result(
-            BaseCheck.MEDIUM, (allpass, 2), "geospatial_lon_extents_match", msgs
+            BaseCheck.MEDIUM,
+            (allpass, 2),
+            "geospatial_lon_extents_match",
+            msgs,
         )
 
     def verify_geospatial_bounds(self, ds):
         """Checks that the geospatial bounds is well formed OGC WKT"""
         var = getattr(ds, "geospatial_bounds", None)
         check = var is not None
         if not check:
@@ -436,21 +437,21 @@
             return ratable_result(
                 False,
                 "Global Attributes",  # grouped with Globals
                 [
                     (
                         "Could not parse WKT from geospatial_bounds,"
                         ' possible bad value: "{}"'.format(ds.geospatial_bounds)
-                    )
+                    ),
                 ],
                 variable_name="geospatial_bounds",
             )
         # parsed OK
         else:
-            return ratable_result(True, "Global Attributes", tuple())
+            return ratable_result(True, "Global Attributes", ())
 
     def _check_total_z_extents(self, ds, z_variable):
         """
         Check the entire array of Z for minimum and maximum and compare that to
         the vertical extents defined in the global attributes
 
         :param netCDF4.Dataset ds: An open netCDF dataset
@@ -465,44 +466,48 @@
 
         try:
             vert_max = float(ds.geospatial_vertical_max)
         except ValueError:
             msgs.append("geospatial_vertical_max cannot be cast to float")
         if len(msgs) > 0:
             return Result(
-                BaseCheck.MEDIUM, (0, total), "geospatial_vertical_extents_match", msgs
+                BaseCheck.MEDIUM,
+                (0, total),
+                "geospatial_vertical_extents_match",
+                msgs,
             )
 
         zvalue = ds.variables[z_variable][:]
         # If the array has fill values, which is allowed in the case of point
         # features
         if hasattr(zvalue, "mask"):
             zvalue = zvalue[~zvalue.mask]
 
         if zvalue.size == 0:
             msgs.append(
                 "Cannot compare geospatial vertical extents "
                 "against min/max of data, as non-masked data "
-                "length is zero"
+                "length is zero",
             )
             return Result(
-                BaseCheck.MEDIUM, (0, total), "geospatial_vertical_extents_match", msgs
+                BaseCheck.MEDIUM,
+                (0, total),
+                "geospatial_vertical_extents_match",
+                msgs,
             )
         else:
             zmin = zvalue.min()
             zmax = zvalue.max()
             if not np.isclose(vert_min, zmin):
                 msgs.append(
-                    "geospatial_vertical_min != min(%s) values, %s != %s"
-                    % (z_variable, vert_min, zmin)
+                    f"geospatial_vertical_min != min({z_variable}) values, {vert_min} != {zmin}",
                 )
             if not np.isclose(vert_max, zmax):
                 msgs.append(
-                    "geospatial_vertical_max != max(%s) values, %s != %s"
-                    % (z_variable, vert_min, zmax)
+                    f"geospatial_vertical_max != max({z_variable}) values, {vert_min} != {zmax}",
                 )
 
         return Result(
             BaseCheck.MEDIUM,
             (total - len(msgs), total),
             "geospatial_vertical_extents_match",
             msgs,
@@ -520,22 +525,20 @@
         vert_max = ds.geospatial_vertical_max
         msgs = []
         total = 2
 
         zvalue = ds.variables[z_variable][:].item()
         if not np.isclose(vert_min, vert_max):
             msgs.append(
-                "geospatial_vertical_min != geospatial_vertical_max for scalar depth values, %s != %s"
-                % (vert_min, vert_max)
+                f"geospatial_vertical_min != geospatial_vertical_max for scalar depth values, {vert_min} != {vert_max}",
             )
 
         if not np.isclose(vert_max, zvalue):
             msgs.append(
-                "geospatial_vertical_max != %s values, %s != %s"
-                % (z_variable, vert_max, zvalue)
+                f"geospatial_vertical_max != {z_variable} values, {vert_max} != {zvalue}",
             )
 
         return Result(
             BaseCheck.MEDIUM,
             (total - len(msgs), total),
             "geospatial_vertical_extents_match",
             msgs,
@@ -556,18 +559,18 @@
         z_variable = cfutil.get_z_variable(ds)
         if not z_variable:
             return Result(
                 BaseCheck.MEDIUM,
                 False,
                 "geospatial_vertical_extents_match",
                 [
-                    "Could not find vertical variable to test extent of geospatial_vertical_min/geospatial_vertical_max, see CF-1.6 spec chapter 4.3"
+                    "Could not find vertical variable to test extent of geospatial_vertical_min/geospatial_vertical_max, see CF-1.6 spec chapter 4.3",
                 ],
             )
-        if ds.variables[z_variable].dimensions == tuple():
+        if ds.variables[z_variable].dimensions == ():
             return self._check_scalar_vertical_extents(ds, z_variable)
 
         return self._check_total_z_extents(ds, z_variable)
 
     def check_time_extents(self, ds):
         """
         Check that the values of time_coverage_start/time_coverage_end approximately match the data.
@@ -583,39 +586,40 @@
             t_max = dateparse(ds.time_coverage_end)
         except (TypeError, pendulum.parsing.exceptions.ParserError):
             return Result(
                 BaseCheck.MEDIUM,
                 False,
                 "time_coverage_extents_match",
                 [
-                    "time_coverage attributes are not formatted properly. Use the ISO 8601:2004 date format, preferably the extended format."
+                    "time_coverage attributes are not formatted properly. Use the ISO 8601:2004 date format, preferably the extended format.",
                 ],
             )
 
         timevar = cfutil.get_time_variable(ds)
 
         if not timevar:
             return Result(
                 BaseCheck.MEDIUM,
                 False,
                 "time_coverage_extents_match",
                 [
-                    "Could not find time variable to test extent of time_coverage_start/time_coverage_end, see CF-1.6 spec chapter 4.4"
+                    "Could not find time variable to test extent of time_coverage_start/time_coverage_end, see CF-1.6 spec chapter 4.4",
                 ],
             )
 
         # Time should be monotonically increasing, so we make that assumption here so we don't have to download THE ENTIRE ARRAY
         try:
             # num2date returns as naive date, but with time adjusted to UTC
             # we need to attach timezone information here, or the date
             # subtraction from t_min/t_max will assume that a naive timestamp is
             # in the same time zone and cause erroneous results.
             # Pendulum uses UTC by default, but we are being explicit here
             time0 = pendulum.instance(
-                num2pydate(ds.variables[timevar][0], ds.variables[timevar].units), "UTC"
+                num2pydate(ds.variables[timevar][0], ds.variables[timevar].units),
+                "UTC",
             )
             time1 = pendulum.instance(
                 num2pydate(ds.variables[timevar][-1], ds.variables[timevar].units),
                 "UTC",
             )
         except ValueError:
             return Result(
@@ -629,23 +633,27 @@
         end_dt = abs(time1 - t_max)
 
         score = 2
         msgs = []
         if start_dt > timedelta(hours=1):
             msgs.append(
                 "Date time mismatch between time_coverage_start and actual "
-                "time values %s (time_coverage_start) != %s (time[0])"
-                % (t_min.isoformat(), time0.isoformat())
+                "time values {} (time_coverage_start) != {} (time[0])".format(
+                    t_min.isoformat(),
+                    time0.isoformat(),
+                ),
             )
             score -= 1
         if end_dt > timedelta(hours=1):
             msgs.append(
                 "Date time mismatch between time_coverage_end and actual "
-                "time values %s (time_coverage_end) != %s (time[N])"
-                % (t_max.isoformat(), time1.isoformat())
+                "time values {} (time_coverage_end) != {} (time[N])".format(
+                    t_max.isoformat(),
+                    time1.isoformat(),
+                ),
             )
             score -= 1
 
         return Result(BaseCheck.MEDIUM, (score, 2), "time_coverage_extents_match", msgs)
 
     def verify_convention_version(self, ds):
         """
@@ -653,75 +661,75 @@
         """
         try:
             for convention in (
                 getattr(ds, "Conventions", "").replace(" ", "").split(",")
             ):
                 if convention == "ACDD-" + self._cc_spec_version:
                     return ratable_result(
-                        (2, 2), None, []
+                        (2, 2),
+                        None,
+                        [],
                     )  # name=None so grouped with Globals
 
             # if no/wrong ACDD convention, return appropriate result
             # Result will have name "Global Attributes" to group with globals
-            m = ["Conventions does not contain 'ACDD-{}'".format(self._cc_spec_version)]
+            m = [f"Conventions does not contain 'ACDD-{self._cc_spec_version}'"]
             return ratable_result((1, 2), "Global Attributes", m)
         except AttributeError:  # NetCDF attribute not found
             m = [
                 "No Conventions attribute present; must contain ACDD-{}".format(
-                    self._cc_spec_version
-                )
+                    self._cc_spec_version,
+                ),
             ]
             # Result will have name "Global Attributes" to group with globals
             return ratable_result((0, 2), "Global Attributes", m)
 
 
 class ACDDNCCheck(BaseNCCheck, ACDDBaseCheck):
     pass
 
 
 class ACDD1_1Check(ACDDNCCheck):
-
     _cc_spec_version = "1.1"
     _cc_description = "Attribute Conventions for Dataset Discovery (ACDD) 1.1"
     register_checker = True
 
     def __init__(self):
-        super(ACDD1_1Check, self).__init__()
+        super().__init__()
         self.rec_atts.extend(["keywords_vocabulary"])
 
         self.sug_atts.extend(
             [
                 "publisher_name",  # publisher,dataCenter
                 "publisher_url",  # publisher
                 "publisher_email",  # publisher
                 "geospatial_vertical_positive",
-            ]
+            ],
         )
 
 
 class ACDD1_3Check(ACDDNCCheck):
-
     _cc_spec_version = "1.3"
     _cc_description = "Attribute Conventions for Dataset Discovery (ACDD) 1.3"
     register_checker = True
 
     def __init__(self):
-        super(ACDD1_3Check, self).__init__()
+        super().__init__()
         self.high_rec_atts.extend([("Conventions", self.verify_convention_version)])
 
         self.rec_atts.extend(
             [
                 "geospatial_vertical_positive",
                 "geospatial_bounds_crs",
                 "geospatial_bounds_vertical_crs",
                 "publisher_name",  # publisher,dataCenter
                 "publisher_url",  # publisher
                 "publisher_email",  # publisher
                 "source",
-            ]
+            ],
         )
 
         self.sug_atts.extend(
             [
                 ("creator_type", ["person", "group", "institution", "position"]),
                 "creator_institution",
                 "platform",
@@ -732,64 +740,64 @@
                 "product_version",
                 "references",
                 ("publisher_type", ["person", "group", "institution", "position"]),
                 "instrument_vocabulary",
                 "date_metadata_modified",
                 "program",
                 "publisher_institution",
-            ]
+            ],
         )
 
         # override the ISO date checks in
         def _check_attr_is_iso_date(attr, ds):
-            result_name = "{}_is_iso".format(attr)
+            result_name = f"{attr}_is_iso"
             if not hasattr(ds, attr):
                 return ratable_result(
-                    (0, 2), result_name, ["Attr {} is not present".format(attr)]
+                    (0, 2),
+                    result_name,
+                    [f"Attr {attr} is not present"],
                 )
             else:
                 iso_check, msgs = datetime_is_iso(getattr(ds, attr))
                 return ratable_result((1 + iso_check, 2), result_name, msgs)
 
         # run ISO 8601 date checks against the date_created, date_issued,
         # date_modified, and date_metadata_modified global attributes
         self.rec_atts = kvp_convert(self.rec_atts)
         self.rec_atts["date_created"] = partial(_check_attr_is_iso_date, "date_created")
         self.sug_atts = kvp_convert(self.sug_atts)
         for k in (
-            "date_{}".format(suffix)
-            for suffix in ("issued", "modified", "metadata_modified")
+            f"date_{suffix}" for suffix in ("issued", "modified", "metadata_modified")
         ):
-
             self.sug_atts[k] = partial(_check_attr_is_iso_date, k)
 
     def check_metadata_link(self, ds):
         """
         Checks if metadata link is formed in a rational manner
 
         :param netCDF4.Dataset ds: An open netCDF dataset
         """
         if not hasattr(ds, "metadata_link"):
             return
         msgs = []
-        meta_link = getattr(ds, "metadata_link")
+        meta_link = ds.metadata_link
         if "http" not in meta_link:
             msgs.append("Metadata URL should include http:// or https://")
         valid_link = len(msgs) == 0
         return Result(BaseCheck.LOW, valid_link, "metadata_link_valid", msgs)
 
     def check_id_has_no_blanks(self, ds):
         """
         Check if there are blanks in the id field
 
         :param netCDF4.Dataset ds: An open netCDF dataset
         """
         if not hasattr(ds, "id"):
             return
-        if " " in getattr(ds, "id"):
+        if " " in ds.id:
             return Result(
                 BaseCheck.MEDIUM,
                 False,
                 "no_blanks_in_id",
                 msgs=["There should be no blanks in the id field"],
             )
         else:
@@ -806,16 +814,19 @@
             msgs = []
             ctype = getattr(ds.variables[variable], "coverage_content_type", None)
             check = ctype is not None
             if not check:
                 msgs.append("coverage_content_type")
                 results.append(
                     Result(
-                        BaseCheck.HIGH, check, self._var_header.format(variable), msgs
-                    )
+                        BaseCheck.HIGH,
+                        check,
+                        self._var_header.format(variable),
+                        msgs,
+                    ),
                 )
                 continue
 
             # ISO 19115-1 codes
             valid_ctypes = {
                 "image",
                 "thematicClassification",
@@ -824,20 +835,19 @@
                 "qualityInformation",
                 "referenceInformation",
                 "modelResult",
                 "coordinate",
             }
             if ctype not in valid_ctypes:
                 msgs.append(
-                    'coverage_content_type "%s" not in %s'
-                    % (variable, sorted(valid_ctypes))
+                    f'coverage_content_type "{variable}" not in {sorted(valid_ctypes)}',
                 )
                 results.append(
                     Result(
                         BaseCheck.HIGH,
                         check,  # append to list
                         self._var_header.format(variable),
                         msgs,
-                    )
+                    ),
                 )
 
         return results
```

### Comparing `compliance-checker-5.0.2/compliance_checker/base.py` & `compliance-checker-5.1.0/compliance_checker/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -55,15 +55,15 @@
     list of str
         A flattened list from the CSV processing contents
     """
     csv_contents = csv.reader(StringIO(input_string))
     return list(itertools.chain.from_iterable(csv_contents))
 
 
-class ValidationObject(object):
+class ValidationObject:
     validator_fail_msg = ""
     expected_type = None
 
     def __init__(self, split_func=None):
         if split_func is None:
             self.split_func = lambda x: [x]
         else:
@@ -122,27 +122,27 @@
     expected_type = str
 
     def validator_func(self, input_value):
         return bool(validators.url(input_value))
 
 
 # Simple class for Generic File type (default to this if file not recognised)
-class GenericFile(object):
+class GenericFile:
     """
     Simple class for any file. Has same path lookup as netCDF4.Dataset.
     """
 
     def __init__(self, fpath):
         self.fpath = fpath
 
     def filepath(self):
         return self.fpath
 
 
-class BaseCheck(object):
+class BaseCheck:
     HIGH = 3
     MEDIUM = 2
     LOW = 1
 
     _cc_checker_version = __version__
     _cc_display_headers = {3: "High Priority", 2: "Medium Priority", 1: "Low Priority"}
 
@@ -175,30 +175,32 @@
         :returns: A new or or existing `TestCtx` instance taken from this
                   instance's _defined_results dict
         """
         # Is it necessary to key out by severity?  Is severity level unique
         # per check?  If so, it could be eliminated from key hierarchy
         if severity not in self._defined_results[name][variable]:
             self._defined_results[name][variable][severity] = TestCtx(
-                severity, name, variable=variable
+                severity,
+                name,
+                variable=variable,
             )
         return self._defined_results[name][variable][severity]
 
     def __del__(self):
         """
         Finalizer. Ensure any caches shared by multiple checkers
         are cleared before the next checker uses it. Some caches were
         inadvertently mutated by other functions.
         """
 
         cfutil.get_geophysical_variables.cache_clear()
         cfutil.get_time_variables.cache_clear()
 
 
-class BaseNCCheck(object):
+class BaseNCCheck:
     """
     Base Class for NetCDF Dataset supporting Check Suites.
     """
 
     supported_ds = {Dataset, MemoizedDataset}
 
     @classmethod
@@ -216,31 +218,31 @@
         return ret_val
 
     @classmethod
     def std_check(cls, dataset, name):
         return name in dataset.ncattrs()
 
 
-class BaseSOSGCCheck(object):
+class BaseSOSGCCheck:
     """
     Base class for SOS-GetCapabilities supporting Check Suites.
     """
 
     supported_ds = [SensorObservationService_1_0_0]
 
 
-class BaseSOSDSCheck(object):
+class BaseSOSDSCheck:
     """
     Base class for SOS-DescribeSensor supporting Check Suites.
     """
 
     supported_ds = [SensorML]
 
 
-class Result(object):
+class Result:
     """
     Holds the result of a check method.
 
     Stores such information as the check's value (True, False, a 2-tuple of (pass, total) or None for a skip),
     weight of the check, any granular messages, or a hierarchy of results. If given value is not a tuple, it
     is cast as a boolean using the bool() function.
 
@@ -254,15 +256,14 @@
         name=None,
         msgs=None,
         children=None,
         checker=None,
         check_method=None,
         variable_name=None,
     ):
-
         self.weight = weight
 
         if value is None:
             self.value = None
         elif isinstance(value, tuple):
             assert len(value) == 2, "Result value must be 2-tuple or boolean!"
             self.value = value
@@ -274,24 +275,24 @@
         self.children = children or []
 
         self.checker = checker
         self.check_method = check_method
         self.variable_name = variable_name
 
     def __repr__(self):
-        ret = "{} (*{}): {}".format(self.name, self.weight, self.value)
+        ret = f"{self.name} (*{self.weight}): {self.value}"
 
         if len(self.msgs):
             if len(self.msgs) == 1:
-                ret += " ({})".format(self.msgs[0])
+                ret += f" ({self.msgs[0]})"
             else:
-                ret += " ({!s} msgs)".format(len(self.msgs))
+                ret += f" ({len(self.msgs)!s} msgs)"
 
         if len(self.children):
-            ret += " ({!s} children)".format(len(self.children))
+            ret += f" ({len(self.children)!s} children)"
             ret += "\n" + pprint.pformat(self.children)
 
         return ret
 
     def serialize(self):
         """
         Returns a serializable dictionary that represents the result object
@@ -304,15 +305,15 @@
             "children": [i.serialize() for i in self.children],
         }
 
     def __eq__(self, other):
         return self.serialize() == other.serialize()
 
 
-class TestCtx(object):
+class TestCtx:
     """
     Simple struct object that holds score values and messages to compile into a result
     """
 
     def __init__(
         self,
         category=None,
@@ -436,78 +437,83 @@
     :param str or None gname        : group name assigned to a group of attribute Results
     :param str or None var_name     : name of the variable which contains this attribute
     """
 
     msgs = []
     name, other = kvp
     if var_name is not None:
-        display_name = "attribute {} in variable {}".format(name, var_name)
+        display_name = f"attribute {name} in variable {var_name}"
         base_context = ds.variables[var_name]
     else:
         display_name = name
         base_context = ds
     if other is None:
         res = std_check(ds, name)
         if not res:
-            msgs = ["{} not present".format(display_name)]
+            msgs = [f"{display_name} not present"]
         else:
             try:
                 # see if this attribute is a string, try stripping
                 # whitespace, and return an error if empty
                 att_strip = base_context.getncattr(name).strip()
                 if not att_strip:
                     res = False
-                    msgs = ["{} is empty or completely whitespace".format(display_name)]
+                    msgs = [f"{display_name} is empty or completely whitespace"]
             # if not a string/has no strip method we should be OK
             except AttributeError:
                 pass
 
         # gname arg allows the global attrs to be grouped together
         ret_val.append(
             Result(
                 priority,
                 value=res,
                 name=gname if gname else name,
                 msgs=msgs,
                 variable_name=var_name,
-            )
+            ),
         )
     elif hasattr(other, "__iter__"):
         # redundant, we could easily do this with a hasattr
         # check instead
         res = std_check_in(base_context, name, other)
         if res == 0:
-            msgs.append("{} not present".format(display_name))
+            msgs.append(f"{display_name} not present")
         elif res == 1:
             msgs.append(
                 "{} present, but not in expected value list ({})".format(
-                    display_name, sorted(other)
-                )
+                    display_name,
+                    sorted(other),
+                ),
             )
 
         ret_val.append(
             Result(
                 priority,
                 (res, 2),
                 gname if gname else name,  # groups Globals if supplied
                 msgs,
                 variable_name=var_name,
-            )
+            ),
         )
     # if we have an XPath expression, call it on the document
     elif type(other) is etree.XPath:
         # TODO: store tree instead of creating it each time?
         # no execution path for variable
         res = xpath_check(ds._root, other)
         if not res:
-            msgs = ["XPath for {} not found".format(display_name)]
+            msgs = [f"XPath for {display_name} not found"]
         ret_val.append(
             Result(
-                priority, res, gname if gname else name, msgs, variable_name=var_name
-            )
+                priority,
+                res,
+                gname if gname else name,
+                msgs,
+                variable_name=var_name,
+            ),
         )
     # check if this is a subclass of ValidationObject
     elif isinstance(other, ValidationObject):
         attr_result = maybe_get_global_attr(name, ds)
         if not attr_result[0]:
             res_tup = attr_result
         else:
@@ -521,57 +527,57 @@
         attr_result = maybe_get_global_attr(name, ds)
         if not attr_result[0]:
             return attr_result
         else:
             check_val = attr_result[1]
         if not isinstance(check_val, str):
             res = False
-            msgs = ["{} must be a string".format(name)]
+            msgs = [f"{name} must be a string"]
         elif not other.search(check_val):
             res = False
-            msgs = ["{} must match regular expression {}".format(name, other)]
+            msgs = [f"{name} must match regular expression {other}"]
         else:
             res = True
             msgs = []
 
         ret_val.append(
-            Result(priority, value=res, name=gname if gname else name, msgs=msgs)
+            Result(priority, value=res, name=gname if gname else name, msgs=msgs),
         )
 
     # if the attribute is a function, call it
     # right now only supports single attribute
     # important note: current magic approach uses all functions
     # starting with "check".  Avoid naming check functions
     # starting with check if you want to pass them in with
     # a tuple to avoid them being checked more than once
-    elif hasattr(other, "__call__"):
+    elif callable(other):
         # check that the attribute is actually present.
         # This reduces boilerplate in functions by not needing
         # to check whether the attribute is present every time
         # and instead focuses on the core functionality of the
         # test
 
         res = other(base_context)  # call the method on the dataset
         if not res:
-            msgs = ["{} not present".format(display_name)]
+            msgs = [f"{display_name} not present"]
             ret_val.append(
                 Result(
                     priority,
                     res,
                     gname if gname else name,
                     msgs,
                     variable_name=var_name,
-                )
+                ),
             )
         else:
             ret_val.append(res(priority))
     # unsupported second type in second
     else:
         raise TypeError(
-            "Second arg in tuple has unsupported type: {}".format(type(other))
+            f"Second arg in tuple has unsupported type: {type(other)}",
         )
 
     return ret_val
 
 
 def check_has(priority=BaseCheck.HIGH, gname=None):
     """Decorator to wrap a function to check if a dataset has given attributes.
@@ -619,15 +625,18 @@
 def score_group(group_name=None):
     """
     Warning this is deprecated as of Compliance Checker v3.2!
 
     Please do not using scoring groups and update your plugins
     if necessary
     """
-    warnings.warn("Score_group is deprecated as of Compliance Checker v3.2.")
+    warnings.warn(
+        "Score_group is deprecated as of Compliance Checker v3.2.",
+        stacklevel=2,
+    )
 
     def _inner(func):
         def _dec(s, ds):
             ret_val = func(s, ds)
             """
             if group_name != None and not isinstance(ret_val[0], tuple):
                 return tuple([(group_name, ret_val[0])] + list(ret_val[1:]))
```

### Comparing `compliance-checker-5.0.2/compliance_checker/cf/appendix_d.py` & `compliance-checker-5.1.0/compliance_checker/cf/appendix_d.py`

 * *Files 2% similar despite different names*

```diff
@@ -69,15 +69,15 @@
         ocean_computed_standard_names,
     ),
     "ocean_s_coordinate": (
         {"s", "eta", "depth", "a", "b", "depth_c"},
         ocean_computed_standard_names,
     ),
     "ocean_sigma_z_coordinate": (
-        {"sigma", "eta", "depth", "depth_c", "nsigma", "zlev"},
+        {"sigma", "eta", "depth", "depth_c", "zlev"},
         ocean_computed_standard_names,
     ),
     "ocean_double_sigma_coordinate": (
         {"sigma", "depth", "z1", "z2", "a", "href", "k_c"},
         ocean_computed_standard_names,
     ),
 }
@@ -91,15 +91,15 @@
             {"s", "C", "eta", "depth", "depth_c"},
             ocean_computed_standard_names,
         ),
         "ocean_s_coordinate_g2": (
             {"s", "C", "eta", "depth", "depth_c"},
             ocean_computed_standard_names,
         ),
-    }
+    },
 )
 
 
 def no_missing_terms(formula_name, term_set, dimless_vertical_coordinates):
     """
     Returns true if the set is not missing terms corresponding to the
     entries in Appendix D, False otherwise.  The set of terms should be exactly
```

### Comparing `compliance-checker-5.0.2/compliance_checker/cf/appendix_e.py` & `compliance-checker-5.1.0/compliance_checker/cf/appendix_e.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,9 +23,9 @@
     {  # returns new set with elements from both
         "maximum_absolute_value",
         "minimum_absolute_value",
         "mean_absolute_value",
         "mean_of_upper_decile",
         "range",
         "root_mean_square",
-    }
+    },
 )
```

### Comparing `compliance-checker-5.0.2/compliance_checker/cf/appendix_f.py` & `compliance-checker-5.1.0/compliance_checker/cf/appendix_f.py`

 * *Files 0% similar despite different names*

```diff
@@ -73,15 +73,15 @@
         "geoid_name": {"type": "S", "extra_condition": False},
         "geopotential_datum_name": {"type": "S", "extra_condition": False},
         "horizontal_datum_name": {"type": "S", "extra_condition": True},
         "prime_meridian_name": {"type": "S", "extra_condition": True},
         "projected_crs_name": {"type": "S", "extra_condition": True},
         "reference_ellipsoid_name": {"type": "S", "extra_condition": False},
         "towgs84": {"type": "N", "extra_condition": True},
-    }
+    },
 )
 
 
 grid_mapping_dict16 = {
     "albers_conical_equal_area": [
         ("longitude_of_central_meridian", "latitude_of_projection_origin"),
         ("false_easting", "false_northing"),
@@ -189,15 +189,15 @@
             ("projection_x_coordinate", "projection_y_coordinate"),
         ],
         "sinusoidal": [
             ("longitude_of_projection_origin"),
             ("false_easting", "false_northing"),
             ("projection_x_coordinate", "projection_y_coordinate"),
         ],
-    }
+    },
 )
 
 # horizontal datum names from https://github.com/cf-convention/cf-conventions/wiki/csv/horiz_datum.csv
 horizontal_datum_names17 = {
     "Hungarian Datum 1909",
     "Taiwan Datum 1967",
     "Taiwan Datum 1997",
```

### Comparing `compliance-checker-5.0.2/compliance_checker/cf/cf.py` & `compliance-checker-5.1.0/compliance_checker/cf/cf.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,7 +26,8 @@
     prime_meridian_names17,
 )
 
 # Version specific checkers organized in other modules
 from compliance_checker.cf.cf_1_6 import CF1_6Check  # noqa: F401
 from compliance_checker.cf.cf_1_7 import CF1_7Check  # noqa: F401
 from compliance_checker.cf.cf_1_8 import CF1_8Check  # noqa: F401
+from compliance_checker.cf.cf_1_9 import CF1_9Check  # noqa: F401
```

### Comparing `compliance-checker-5.0.2/compliance_checker/cf/cf_1_6.py` & `compliance-checker-5.1.0/compliance_checker/cf/cf_1_6.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import difflib
 import logging
 from collections import defaultdict
 
+import cftime
 import numpy as np
 import regex
 from cf_units import Unit
 
 from compliance_checker import cfutil
 from compliance_checker.base import BaseCheck, Result, TestCtx
 from compliance_checker.cf import util
@@ -21,28 +22,36 @@
 logger = logging.getLogger(__name__)
 
 
 class CF1_6Check(CFNCCheck):
     """CF-1.6-specific implementation of CFBaseCheck; supports checking
     netCDF datasets.
     These checks are translated documents:
-        http://cf-pcmdi.llnl.gov/documents/cf-conventions/1.6/cf-conventions.html
-        http://cf-pcmdi.llnl.gov/conformance/requirements-and-recommendations/1.6/"""
+        https://cfconventions.org/cf-conventions/v1.6.0/cf-conventions.html"""
 
     register_checker = True
     _cc_spec = "cf"
     _cc_spec_version = "1.6"
     _cc_description = "Climate and Forecast Conventions (CF)"
     _cc_url = "http://cfconventions.org/cf-conventions/v1.6.0/cf-conventions.html"
     _cc_display_headers = {3: "Errors", 2: "Warnings", 1: "Info"}
     appendix_a = appendix_a_base
     appendix_d_parametric_coords = dimless_vertical_coordinates_1_6
+    _allowed_numeric_var_types = {
+        np.character,
+        np.bytes_,  # "|S1" dtype, byte array used as string
+        np.int8,
+        np.int16,
+        np.int32,
+        np.float32,
+        np.float64,
+    }
 
     def __init__(self, options=None):  # initialize with parent methods and data
-        super(CF1_6Check, self).__init__(options)
+        super().__init__(options)
 
         self.cell_methods = cell_methods16
         self.grid_mapping_dict = grid_mapping_dict16
         self.grid_mapping_attr_types = grid_mapping_attr_types16
 
     ###############################################################################
     # Chapter 2: NetCDF Files and Components
@@ -72,31 +81,21 @@
         fails = []
         total = len(ds.variables)
 
         for k, v in ds.variables.items():
             if (
                 v.dtype is not str
                 and v.dtype.kind != "S"
-                and all(
-                    v.dtype.type != t
-                    for t in (
-                        np.character,
-                        np.dtype("|S1"),
-                        np.dtype("b"),
-                        np.dtype("i2"),
-                        np.dtype("i4"),
-                        np.float32,
-                        np.double,
-                    )
-                )
+                and v.dtype.type not in self._allowed_numeric_var_types
             ):
                 fails.append(
                     "The variable {} failed because the datatype is {}".format(
-                        k, v.datatype
-                    )
+                        k,
+                        v.datatype,
+                    ),
                 )
         return Result(
             BaseCheck.HIGH,
             (total - len(fails), total),
             self.section_titles["2.2"],
             msgs=fails,
         )
@@ -123,15 +122,15 @@
             "actual_range",
             "valid_min",
             "valid_max",
             "valid_range",
             "_FillValue",
         }
 
-        for var_name, var in ds.variables.items():
+        for _var_name, var in ds.variables.items():
             for att_name in special_attrs.intersection(var.ncattrs()):
                 self._parent_var_attr_type_check(att_name, var, ctx)
         return ctx.to_result()
 
     # TODO: consider renaming to avoid confusion with non-underscore
     #       primary function version
     def _check_add_offset_scale_factor_type(self, variable, attr_name):
@@ -151,16 +150,15 @@
             val = False
 
         else:
             val = (
                 att.dtype == variable.dtype
             ) or (  # will short-circuit or if first condition is true
                 isinstance(att, (np.float32, np.float64, float))
-                and variable.dtype
-                in (np.byte, np.short, np.int16, np.int, np.int32, int)
+                and variable.dtype in (np.byte, np.short, np.int16, np.int32, int)
             )
         if not val:
             msgs.append(error_msg)
 
         return Result(BaseCheck.MEDIUM, val, self.section_titles["8.1"], msgs)
 
     def check_add_offset_scale_factor_type(self, ds):
@@ -169,51 +167,50 @@
         check that the variables and attributes are of the same type
         OR that the variable is of type byte, short or int and the
         attributes are of type float or double.
         """
 
         results = []
         add_offset_vars = ds.get_variables_by_attributes(
-            add_offset=lambda x: x is not None
+            add_offset=lambda x: x is not None,
         )
         scale_factor_vars = ds.get_variables_by_attributes(
-            scale_factor=lambda x: x is not None
+            scale_factor=lambda x: x is not None,
         )
 
         both = set(add_offset_vars).intersection(scale_factor_vars)
         both_msgs = []
         for both_var in sorted(both, key=lambda var: var.name):
             if both_var.scale_factor.dtype != both_var.add_offset.dtype:
                 both_msgs.append(
                     "When both scale_factor and add_offset "
                     f"are supplied for variable {both_var.name}, "
-                    "they must have the same type"
+                    "they must have the same type",
                 )
         results.append(
             Result(
                 BaseCheck.MEDIUM,
                 not bool(both_msgs),
                 self.section_titles["8.1"],
                 both_msgs,
-            )
+            ),
         )
 
         for _att_vars_tup in (
             ("add_offset", add_offset_vars),
             ("scale_factor", scale_factor_vars),
         ):
             results.extend(
-                list(
-                    map(
-                        lambda var: self._check_add_offset_scale_factor_type(
-                            var, _att_vars_tup[0]
-                        ),
-                        _att_vars_tup[1],
+                [
+                    self._check_add_offset_scale_factor_type(
+                        var,
+                        _att_vars_tup[0],
                     )
-                )
+                    for var in _att_vars_tup[1]
+                ],
             )
 
         return results
 
     def check_naming_conventions(self, ds):
         """
         Checks the variable names to ensure they are valid CF variable names under CF.
@@ -231,14 +228,15 @@
 
         ignore_attributes = [
             "_FillValue",
             "DODS",
             "_ChunkSizes",
             "_Coordinate",
             "_Unsigned",
+            "_Encoding",
         ]
 
         rname = regex.compile("^[A-Za-z][A-Za-z0-9_]*$")
 
         # IMPLEMENTATION CONFORMANCE 2.3 REQUIRED
         for name, variable in ds.variables.items():
             variable_naming.assert_true(
@@ -336,15 +334,15 @@
             for d in v.dimensions:
                 dims[d] += 1
 
             # IMPLEMENTATION CONFORMANCE 2.4 REQUIRED
             for dimension, count in dims.items():
                 if count > 1:
                     fails.append(
-                        "%s has two or more dimensions named %s" % (k, dimension)
+                        f"{k} has two or more dimensions named {dimension}",
                     )
 
         return Result(
             BaseCheck.HIGH,
             (total - len(fails), total),
             self.section_titles["2.4"],
             msgs=fails,
@@ -394,20 +392,85 @@
                     "{}'s spatio-temporal dimensions are not in the "
                     "recommended order T, Z, Y, X and/or further dimensions "
                     "are not located left of T, Z, Y, X. The dimensions (and "
                     "their guessed types) are {} (with U: other/unknown; L: "
                     "unlimited).".format(
                         name,
                         self._get_pretty_dimension_order_with_type(
-                            ds, name, dimension_order
+                            ds,
+                            name,
+                            dimension_order,
                         ),
                     ),
                 )
         return valid_dimension_order.to_result()
 
+    def check_fill_value_equal_missing_value(self, ds):
+        """
+        If both missing_value and _FillValue be used, they should have the same value.
+        This according to CF §2.5.1 Recommendations:
+
+        :param netCDF4.Dataset ds: An open netCDF dataset
+        :rtype: list
+        :return: List of Results
+        """
+        fails = []
+        total = 0
+
+        for _name, variable in ds.variables.items():
+            # If the variable have a defined _FillValue a defined missing_value check it.
+
+            if hasattr(variable, "_FillValue") and hasattr(variable, "missing_value"):
+                total = total + 1
+                if variable._FillValue != variable.missing_value:
+                    fails.append(
+                        "For the variable {} the missing_value must be equal to the _FillValue".format(
+                            variable.name,
+                        ),
+                    )
+
+        return Result(
+            BaseCheck.MEDIUM,
+            (len(fails), total),
+            self.section_titles["2.5"],
+            msgs=fails,
+        )
+
+    def check_valid_range_or_valid_min_max_present(self, ds):
+        """
+        The valid_range attribute must not be present if the valid_min
+        and/or valid_max attributes are present. This according to 2.5.1 Requirements.
+
+        :param netCDF4.Dataset ds: An open netCDF dataset
+        :rtype: list
+        :return: List of Results
+        """
+        fails = []
+        total = 0
+
+        for _name, variable in ds.variables.items():
+            if hasattr(variable, "valid_max") and (
+                hasattr(variable, "valid_min") or hasattr(variable, "valid_range")
+            ):
+                total = total + 1
+
+                fails.append(
+                    "For the variable {} the valid_range attribute must not be present "
+                    "if the valid_min and/or valid_max attributes are present".format(
+                        variable.name,
+                    ),
+                )
+
+        return Result(
+            BaseCheck.MEDIUM,
+            (len(fails), total),
+            self.section_titles["2.5"],
+            msgs=fails,
+        )
+
     def check_fill_value_outside_valid_range(self, ds):
         """
         Checks each variable's _FillValue to ensure that it's in valid_range or
         between valid_min and valid_max according to CF §2.5.1
 
         CF §2.5.1 The _FillValue should be outside the range specified by
         valid_range (if used) for a variable.
@@ -430,34 +493,36 @@
 
             if "valid_range" in attrs:
                 if isinstance(variable.valid_range, str):
                     m = "§2.5.1 Fill Values should be outside the range specified by valid_range"  # subsection message
                     valid_fill_range.assert_true(
                         False,
                         "{};\n\t{}:valid_range must be a numeric type not a string".format(
-                            m, name
+                            m,
+                            name,
                         ),
                     )
                     continue
                 rmin, rmax = variable.valid_range
                 spec_by = "valid_range"
 
             elif "valid_min" in attrs and "valid_max" in attrs:
                 if isinstance(variable.valid_min, str):
                     valid_fill_range.assert_true(
                         False,
-                        "{}:valid_min must be a numeric type not a string".format(name),
+                        f"{name}:valid_min must be a numeric type not a string",
                     )
                 if isinstance(variable.valid_max, str):
                     valid_fill_range.assert_true(
                         False,
-                        "{}:valid_max must be a numeric type not a string".format(name),
+                        f"{name}:valid_max must be a numeric type not a string",
                     )
                 if isinstance(variable.valid_min, str) or isinstance(
-                    variable.valid_max, str
+                    variable.valid_max,
+                    str,
                 ):
                     continue
                 rmin = variable.valid_min
                 rmax = variable.valid_max
                 spec_by = "valid_min/valid_max"
             else:
                 continue
@@ -496,14 +561,34 @@
             valid_globals.assert_true(
                 is_string and len(dataset_attr),
                 "§2.6.2 global attribute {} should exist and be a non-empty string"  # subsection message
                 "".format(attr),
             )
         return valid_globals.to_result()
 
+    # IMPLEMENTATION
+    def check_coordinate_variables_strict_monotonicity(self, ds):
+        """
+        Checks that data in coordinate variables is either monotonically
+        increasing or decreasing
+        """
+
+        ret_val = []
+        for coord_var_name in self._find_coord_vars(ds):
+            coord_var = ds.variables[coord_var_name]
+            arr_diff = np.diff(coord_var)
+            monotonicity = TestCtx(BaseCheck.HIGH, self.section_titles["5"])
+            monotonicity.assert_true(
+                np.all(arr_diff > 0) or np.all(arr_diff < 0),
+                f'Coordinate variable "{coord_var_name}" must be strictly monotonic',
+            )
+            ret_val.append(monotonicity.to_result())
+
+        return ret_val
+
     def check_convention_possibly_var_attrs(self, ds):
         """
         Check variable and global attributes are strings for recommended attributes under CF §2.6.2
 
         CF §2.6.2 institution, source, references, and comment, either global
         or assigned to individual variables.  When an attribute appears both
         globally and as a variable attribute, the variable's version has
@@ -581,27 +666,27 @@
         geophysical_variables = self._find_geophysical_vars(ds)
         modifier_variables = cfutil._find_standard_name_modifier_variables(ds)
         forecast_variables = cfutil.get_forecast_metadata_variables(ds)
 
         dimless_vert = {
             var.name
             for var in ds.get_variables_by_attributes(
-                standard_name=lambda s: s in self.appendix_d_parametric_coords
+                standard_name=lambda s: s in self.appendix_d_parametric_coords,
             )
             if not hasattr(var, "units")
         }
         # check anything remaining that has units
         # unit_containing =
         unit_required_variables = (
             set(
                 coordinate_variables
                 + auxiliary_coordinates
                 + geophysical_variables
                 + forecast_variables
-                + modifier_variables
+                + modifier_variables,
             )  # standard names with modifiers require proper units, *except* for flags, where they should not be present
             - dimless_vert
         )
 
         for name in unit_required_variables:
             # For reduced horizontal grids, the compression index variable does
             # not require units.
@@ -618,29 +703,30 @@
             if (
                 hasattr(variable.dtype, "char") and variable.dtype.char == "S"
             ) or variable.dtype == str:
                 continue
 
             standard_name = getattr(variable, "standard_name", None)
             standard_name, standard_name_modifier = self._split_standard_name(
-                standard_name
+                standard_name,
             )
 
             units = getattr(variable, "units", None)
 
             valid_units = self._check_valid_cf_units(ds, name)
             ret_val.append(valid_units)
 
             units_attr_is_string = TestCtx(BaseCheck.MEDIUM, self.section_titles["3.1"])
 
             # side effects, but better than teasing out the individual result
             if units is not None and units_attr_is_string.assert_true(
                 isinstance(units, str),
                 "units ({}) attribute of '{}' must be a string compatible with UDUNITS".format(
-                    units, variable.name
+                    units,
+                    variable.name,
                 ),
             ):
                 valid_udunits = self._check_valid_udunits(ds, name)
                 ret_val.append(valid_udunits)
             ret_val.append(units_attr_is_string.to_result())
 
             if isinstance(standard_name, str):
@@ -665,24 +751,25 @@
         deprecated = ["level", "layer", "sigma_level"]
         variable = ds.variables[variable_name]
 
         valid_units = TestCtx(BaseCheck.HIGH, self.section_titles["3.1"])
         units = getattr(variable, "units", None)
         standard_name_full = getattr(variable, "standard_name", None)
         standard_name, standard_name_modifier = self._split_standard_name(
-            standard_name_full
+            standard_name_full,
         )
         std_name_units_dimensionless = cfutil.is_dimensionless_standard_name(
-            self._std_names._root, standard_name
+            self._std_names._root,
+            standard_name,
         )
 
         # 3) units are not deprecated
         valid_units.assert_true(
             units not in deprecated,
-            'units for {}, "{}" are deprecated by CF 1.6'.format(variable_name, units),
+            f'units for {variable_name}, "{units}" are deprecated by CF 1.6',
         )
         # 4/5) Modifiers, if present, have the appropriate units, or none for
         #    status_flag
         if standard_name_modifier is not None:
             if standard_name_modifier not in valid_modifiers:
                 # standard name modifier warning given elsewhere
                 return valid_units.to_result()
@@ -718,32 +805,32 @@
             or standard_name is None
         )
 
         # 1) Units must exist
         valid_units.assert_true(
             should_be_dimensionless or units is not None,
             "units attribute is required for {} when variable is not a dimensionless quantity".format(
-                variable_name
+                variable_name,
             ),
         )
 
         # Don't bother checking the rest
         if units is None and not should_be_dimensionless:
             return valid_units.to_result()
         # 2) units attribute must be a string
         valid_units.assert_true(
             should_be_dimensionless or isinstance(units, str),
-            "units attribute for {} needs to be a string".format(variable_name),
+            f"units attribute for {variable_name} needs to be a string",
         )
 
         try:
             units_conv = Unit(units)
         except ValueError:
             valid_units.messages.append(
-                f'Unit string "{units}" is not recognized by UDUnits'
+                f'Unit string "{units}" is not recognized by UDUnits',
             )
             valid_units.out_of += 1
             return valid_units
         else:
             valid_units.score += 1
             valid_units.out_of += 1
 
@@ -769,30 +856,32 @@
         """
         variable = ds.variables[variable_name]
 
         units = getattr(variable, "units", None)
         standard_name = getattr(variable, "standard_name", None)
         standard_name, standard_name_modifier = self._split_standard_name(standard_name)
         std_name_units_dimensionless = cfutil.is_dimensionless_standard_name(
-            self._std_names._root, standard_name
+            self._std_names._root,
+            standard_name,
         )
 
         # If the variable is supposed to be dimensionless, it automatically passes
         should_be_dimensionless = (
             variable.dtype is str
             or (hasattr(variable.dtype, "char") and variable.dtype.char == "S")
             or std_name_units_dimensionless
         )
 
         valid_udunits = TestCtx(BaseCheck.HIGH, self.section_titles["3.1"])
         are_udunits = units is not None and util.units_known(units)
         valid_udunits.assert_true(
             should_be_dimensionless or are_udunits or units is None,
             'units for {}, "{}" are not recognized by UDUNITS'.format(
-                variable_name, units
+                variable_name,
+                units,
             ),
         )
         return valid_udunits.to_result()
 
     def _check_valid_standard_units(self, ds, variable_name):
         """
         Checks that the variable's units are appropriate for the standard name
@@ -806,15 +895,16 @@
         units = getattr(variable, "units", None)
         standard_name = getattr(variable, "standard_name", None)
 
         valid_standard_units = TestCtx(BaseCheck.HIGH, self.section_titles["3.1"])
 
         # If the variable is supposed to be dimensionless, it automatically passes
         std_name_units_dimensionless = cfutil.is_dimensionless_standard_name(
-            self._std_names._root, standard_name
+            self._std_names._root,
+            standard_name,
         )
 
         if std_name_units_dimensionless:
             return valid_standard_units.to_result()
 
         standard_name, standard_name_modifier = self._split_standard_name(standard_name)
 
@@ -833,14 +923,17 @@
                 )
                 valid_standard_units.messages.append(err_msg)
             else:
                 valid_standard_units.score += 1
             # number_of_observations should short circuit and not continue
             # on to further units checks
             return valid_standard_units.to_result()
+        elif standard_name_modifier == "status_flag":
+            # no units required - skip further checks
+            return valid_standard_units.to_result()
 
         # This section represents the different cases where simple udunits
         # comparison isn't comprehensive enough to determine if the units are
         # appropriate under CF
 
         # UDUnits accepts "s" as a unit of time but it should be <unit> since <epoch>
         # TODO: forecast_reference_time.  Include upcoming merge.
@@ -917,23 +1010,23 @@
             if hasattr(ncvar.dtype, "char") and ncvar.dtype.char == "S":
                 continue
             elif ncvar.dtype == str:
                 continue
 
             standard_name = getattr(ncvar, "standard_name", None)
             standard_name, standard_name_modifier = self._split_standard_name(
-                standard_name
+                standard_name,
             )
             long_name = getattr(ncvar, "long_name", None)
             long_or_std_name = TestCtx(BaseCheck.HIGH, self.section_titles["3.3"])
             if long_name is not None:
                 long_name_present = True
                 long_or_std_name.assert_true(
                     isinstance(long_name, str),
-                    "Attribute long_name for variable {} must be a string".format(name),
+                    f"Attribute long_name for variable {name} must be a string",
                 )
             else:
                 long_name_present = False
             # §1.3 The long_name and standard_name attributes are used to
             # describe the content of each variable. For backwards
             # compatibility with COARDS neither is required, but use of at
             # least one of them is strongly recommended.
@@ -943,24 +1036,26 @@
             # IMPLEMENTATION CONFORMANCE 3.3 REQUIRED 1, 2, 3 / 3
             if standard_name is not None:
                 standard_name_present = True
                 valid_std_name = TestCtx(BaseCheck.HIGH, self.section_titles["3.3"])
                 valid_std_name.assert_true(
                     isinstance(standard_name, str),
                     "Attribute standard_name for variable {} must be a string".format(
-                        name
+                        name,
                     ),
                 )
                 valid_std_name.out_of += 1
                 if standard_name not in self._std_names:
                     err_msg = "standard_name {} is not defined in Standard Name Table v{}.".format(
-                        standard_name or "undefined", self._std_names._version
+                        standard_name or "undefined",
+                        self._std_names._version,
                     )
                     close_matches = difflib.get_close_matches(
-                        standard_name, self._std_names
+                        standard_name,
+                        self._std_names,
                     )
                     if close_matches:
                         err_msg += f" Possible close match(es): {close_matches}"
                     valid_std_name.messages.append(err_msg)
                 else:
                     valid_std_name.score += 1
 
@@ -969,27 +1064,28 @@
                 # 2) optional - if modifiers, should be in table
                 if standard_name_modifier is not None:
                     valid_modifier = TestCtx(BaseCheck.HIGH, self.section_titles["3.3"])
                     valid_modifier.assert_true(
                         standard_name_modifier in valid_modifiers,
                         'Standard name modifier "{}" for variable {} is not a valid modifier '
                         "according to CF Appendix C".format(
-                            standard_name_modifier, name
+                            standard_name_modifier,
+                            name,
                         ),
                     )
 
                     ret_val.append(valid_modifier.to_result())
             else:
                 standard_name_present = False
 
             # IMPLEMENTATION CONFORMANCE 3 RECOMMENDED
             long_or_std_name.assert_true(
                 long_name_present or standard_name_present,
                 "Attribute long_name or/and standard_name is highly recommended for variable {}".format(
-                    name
+                    name,
                 ),
             )
             ret_val.append(long_or_std_name.to_result())
         return ret_val
 
     def check_ancillary_variables(self, ds):
         """
@@ -1007,15 +1103,15 @@
         :param netCDF4.Dataset ds: An open netCDF dataset
         :rtype: list
         :return: List of results
         """
         ret_val = []
 
         for ncvar in ds.get_variables_by_attributes(
-            ancillary_variables=lambda x: x is not None
+            ancillary_variables=lambda x: x is not None,
         ):
             name = ncvar.name
             valid_ancillary = TestCtx(BaseCheck.HIGH, self.section_titles["3.4"])
             ancillary_variables = ncvar.ancillary_variables
 
             valid_ancillary.assert_true(
                 isinstance(ancillary_variables, str),
@@ -1027,15 +1123,15 @@
             if not isinstance(ancillary_variables, str):
                 ret_val.append(valid_ancillary.to_result())
                 continue
 
             for ancillary_variable in ancillary_variables.split():
                 valid_ancillary.assert_true(
                     ancillary_variable in ds.variables,
-                    "{} is not a variable in this dataset".format(ancillary_variable),
+                    f"{ancillary_variable} is not a variable in this dataset",
                 )
 
             ret_val.append(valid_ancillary.to_result())
 
         return ret_val
 
     def check_flags(self, ds):
@@ -1078,15 +1174,15 @@
             flag_values = getattr(variable, "flag_values", None)
             flag_masks = getattr(variable, "flag_masks", None)
 
             valid_flags_var = TestCtx(BaseCheck.HIGH, self.section_titles["3.5"])
             # Check that the variable defines mask or values
             valid_flags_var.assert_true(
                 flag_values is not None or flag_masks is not None,
-                "{} does not define either flag_masks or flag_values".format(name),
+                f"{name} does not define either flag_masks or flag_values",
             )
             ret_val.append(valid_flags_var.to_result())
 
             valid_meanings = self._check_flag_meanings(ds, name)
             ret_val.append(valid_meanings)
 
             # check flag_values
@@ -1110,16 +1206,16 @@
                 else:
                     allv = np.all(vals_arr & masks_arr == vals_arr)
 
                 allvr = Result(BaseCheck.MEDIUM, allv, self.section_titles["3.5"])
                 if not allvr.value:
                     allvr.msgs = [
                         "flag masks and flag values for '{}' combined don't equal flag values".format(
-                            name
-                        )
+                            name,
+                        ),
                     ]
 
                 ret_val.append(allvr)
 
         return ret_val
 
     def _check_flag_values(self, ds, name):
@@ -1148,15 +1244,15 @@
             "defined when flag_values attribute is present",
         )
 
         # the flag values must be independent, no repeating values
         flag_set = np.unique(flag_values)
         valid_values.assert_true(
             flag_set.size == np.array(flag_values).size,
-            "{}'s flag_values must be independent and can not be repeated".format(name),
+            f"{name}'s flag_values must be independent and can not be repeated",
         )
 
         # IMPLEMENTATION CONFORMANCE 3.5 REQUIRED 1/8
         # the data type for flag_values should be the same as the variable
         valid_values.assert_true(
             variable.dtype.type == flag_values.dtype.type,
             "flag_values ({}) must be the same data type as {} ({})"
@@ -1210,15 +1306,15 @@
             0 not in np.array(flag_masks),
             f"flag_masks for variable {variable.name} must "
             "not contain zero as an element",
         )
 
         valid_masks.assert_true(
             type_ok,
-            "{}'s data type must be capable of bit-field expression".format(name),
+            f"{name}'s data type must be capable of bit-field expression",
         )
 
         if isinstance(flag_meanings, str):
             flag_meanings = flag_meanings.split()
             valid_masks.assert_true(
                 # cast to array here as single element arrays are returned as
                 # scalars from netCDF4 Python
@@ -1243,41 +1339,42 @@
         """
         variable = ds.variables[name]
         flag_meanings = getattr(variable, "flag_meanings", None)
         valid_meanings = TestCtx(BaseCheck.HIGH, self.section_titles["3.5"])
 
         valid_meanings.assert_true(
             flag_meanings is not None,
-            "{}'s flag_meanings attribute is required for flag variables".format(name),
+            f"{name}'s flag_meanings attribute is required for flag variables",
         )
 
         valid_meanings.assert_true(
             isinstance(flag_meanings, str),
-            "{}'s flag_meanings attribute must be a string".format(name),
+            f"{name}'s flag_meanings attribute must be a string",
         )
 
         # We can't perform any additional checks if it's not a string
         if not isinstance(flag_meanings, str):
             return valid_meanings.to_result()
 
         valid_meanings.assert_true(
-            len(flag_meanings) > 0, "{}'s flag_meanings can't be empty".format(name)
+            len(flag_meanings) > 0,
+            f"{name}'s flag_meanings can't be empty",
         )
 
         # IMPLEMENTATION CONFORMANCE REQUIRED 3.5 3/8
         flag_regx = regex.compile(r"^[0-9A-Za-z_\-.+@]+$")
         meanings = flag_meanings.split()
         for meaning in meanings:
             if flag_regx.match(meaning) is None:
                 valid_meanings.assert_true(
                     False,
                     "{}'s flag_meanings attribute defined an illegal flag meaning ".format(
-                        name
+                        name,
                     )
-                    + "{}".format(meaning),
+                    + f"{meaning}",
                 )
         return valid_meanings.to_result()
 
     ###############################################################################
     # Chapter 4: Coordinate Types
     ###############################################################################
 
@@ -1339,25 +1436,24 @@
         variable = ds.variables[name]
         axis = variable.axis
 
         valid_axis = TestCtx(BaseCheck.HIGH, self.section_titles["4"])
         axis_is_string = (isinstance(axis, str),)
         valid_axis.assert_true(
             axis_is_string and len(axis) > 0,
-            "{}'s axis attribute must be a non-empty string".format(name),
+            f"{name}'s axis attribute must be a non-empty string",
         )
 
         # If axis isn't a string we can't continue any checks
         if not axis_is_string or len(axis) == 0:
             return valid_axis.to_result()
 
         valid_axis.assert_true(
             axis in allowed_axis,
-            "{}'s axis attribute must be T, X, Y, or Z, ".format(name)
-            + "currently {}".format(axis),
+            f"{name}'s axis attribute must be T, X, Y, or Z, " + f"currently {axis}",
         )
 
         return valid_axis.to_result()
 
     def check_latitude(self, ds):
         """
         Check variable(s) that define latitude and are defined correctly according to CF.
@@ -1409,15 +1505,15 @@
             standard_name = getattr(variable, "standard_name", None)
             axis = getattr(variable, "axis", None)
 
             # Check that latitude defines units
             valid_latitude = TestCtx(BaseCheck.HIGH, self.section_titles["4.1"])
             valid_latitude.assert_true(
                 units is not None,
-                "latitude variable '{}' must define units".format(latitude),
+                f"latitude variable '{latitude}' must define units",
             )
             ret_val.append(valid_latitude.to_result())
 
             # Check that latitude uses allowed units
             allowed_units = TestCtx(BaseCheck.MEDIUM, self.section_titles["4.1"])
             if standard_name == "grid_latitude":
                 e_n_units = cfutil.VALID_LAT_UNITS | cfutil.VALID_LON_UNITS
@@ -1441,15 +1537,18 @@
                 # This is only a recommendation and we won't penalize but we
                 # will include a recommended action.
                 msg = (
                     "CF recommends latitude variable '{}' to use units degrees_north"
                     "".format(latitude)
                 )
                 recommended_units = Result(
-                    BaseCheck.LOW, (1, 1), self.section_titles["4.1"], [msg]
+                    BaseCheck.LOW,
+                    (1, 1),
+                    self.section_titles["4.1"],
+                    [msg],
                 )
                 ret_val.append(recommended_units)
 
             y_variables = ds.get_variables_by_attributes(axis="Y")
             # Check that latitude defines either standard_name or axis
             definition = TestCtx(BaseCheck.MEDIUM, self.section_titles["4.1"])
             definition.assert_true(
@@ -1515,15 +1614,15 @@
             axis = getattr(variable, "axis", None)
 
             # NOTE see docstring--should below be 4.1 or 4.2?
             # Check that longitude defines units
             valid_longitude = TestCtx(BaseCheck.HIGH, self.section_titles["4.2"])
             valid_longitude.assert_true(
                 units is not None,
-                "longitude variable '{}' must define units".format(longitude),
+                f"longitude variable '{longitude}' must define units",
             )
             ret_val.append(valid_longitude.to_result())
 
             # Check that longitude uses allowed units
             allowed_units = TestCtx(BaseCheck.MEDIUM, self.section_titles["4.2"])
             if standard_name == "grid_longitude":
                 e_n_units = cfutil.VALID_LAT_UNITS | cfutil.VALID_LON_UNITS
@@ -1547,15 +1646,18 @@
                 # This is only a recommendation and we won't penalize but we
                 # will include a recommended action.
                 msg = (
                     "CF recommends longitude variable '{}' to use units degrees_east"
                     "".format(longitude)
                 )
                 recommended_units = Result(
-                    BaseCheck.LOW, (1, 1), self.section_titles["4.2"], [msg]
+                    BaseCheck.LOW,
+                    (1, 1),
+                    self.section_titles["4.2"],
+                    [msg],
                 )
                 ret_val.append(recommended_units)
 
             x_variables = ds.get_variables_by_attributes(axis="X")
             # Check that longitude defines either standard_name or axis
             definition = TestCtx(BaseCheck.MEDIUM, self.section_titles["4.2"])
             definition.assert_true(
@@ -1564,15 +1666,17 @@
                 "".format(longitude),
             )
             ret_val.append(definition.to_result())
 
         return ret_val
 
     def check_dimensional_vertical_coordinate(
-        self, ds, dimless_vertical_coordinates=dimless_vertical_coordinates_1_6
+        self,
+        ds,
+        dimless_vertical_coordinates=dimless_vertical_coordinates_1_6,
     ):
         """
         Check units for variables defining vertical position are valid under
         CF.
 
         CF §4.3.1 The units attribute for dimensional coordinates will be a string
         formatted as per the udunits.dat file.
@@ -1628,15 +1732,20 @@
             # already verifies that this coordinate has valid units
 
             ret_val.append(valid_vertical_coord.to_result())
 
         return ret_val
 
     def _check_dimensionless_vertical_coordinate_1_6(
-        self, ds, vname, deprecated_units, ret_val, dim_vert_coords_dict
+        self,
+        ds,
+        vname,
+        deprecated_units,
+        ret_val,
+        dim_vert_coords_dict,
     ):
         """
         Check that a dimensionless vertical coordinate variable is valid under
         CF-1.6.
 
         :param netCDF4.Dataset ds: open netCDF4 dataset
         :param str name: variable name
@@ -1691,15 +1800,15 @@
 
         ret_val.extend(
             self._check_dimensionless_vertical_coordinates(
                 ds,
                 deprecated_units,
                 self._check_dimensionless_vertical_coordinate_1_6,
                 dimless_vertical_coordinates_1_6,
-            )
+            ),
         )
 
         return ret_val
 
     def check_time_coordinate(self, ds):
         """
         Check variables defining time are valid under CF
@@ -1750,19 +1859,52 @@
             # TODO: year zero climatological time warning
             result = Result(BaseCheck.HIGH, True, self.section_titles["4.4"])
             ret_val.append(result)
             correct_units = util.units_temporal(variable.units)
             reasoning = None
             if not correct_units:
                 reasoning = ["%s does not have correct time units" % name]
-            result = Result(
-                BaseCheck.HIGH, correct_units, self.section_titles["4.4"], reasoning
-            )
-            ret_val.append(result)
-
+                result = Result(
+                    BaseCheck.HIGH,
+                    correct_units,
+                    self.section_titles["4.4"],
+                    reasoning,
+                )
+                ret_val.append(result)
+                continue
+            # IMPLEMENTATION CONFORMANCE 4.4 RECOMMENDED 1/2
+            if hasattr(variable, "climatology"):
+                year_match = regex.match(r"\w+ since (?P<year>\d{1,4})", variable.units)
+                # year should always exist at this point if it's been parsed as
+                # valid date
+                if int(year_match.group("year")) == 0:
+                    message = (
+                        f"Time coordinate variable {variable.name}'s "
+                        "use of year 0 for climatological time is "
+                        "deprecated"
+                    )
+                    result = Result(
+                        BaseCheck.MEDIUM,
+                        False,
+                        self.section_titles["4.4"],
+                        [message],
+                    )
+                    ret_val.append(result)
+            # IMPLEMENTATION CONFORMANCE 4.4 RECOMMENDED 2/2
+            # catch non-recommended months or years time interval
+            unit = Unit(variable.units)
+            if unit.is_long_time_interval():
+                message = f"Using relative time interval of months or years is not recommended for coordinate variable {variable.name}"
+                result = Result(
+                    BaseCheck.MEDIUM,
+                    False,
+                    self.section_titles["4.4"],
+                    [message],
+                )
+                ret_val.append(result)
         return ret_val
 
     def check_calendar(self, ds):
         """
         Check the calendar attribute for variables defining time and ensure it
         is a valid calendar prescribed by CF.
 
@@ -1799,48 +1941,121 @@
         non-standard values and in that case defining the non-standard calendar
         using the appropriate attributes is required.
 
         :param netCDF4.Dataset ds: An open netCDF dataset
         :rtype: list
         :return: List of results
         """
-        valid_calendars = {
+        standard_calendars = {
             "gregorian",
             "standard",
             "proleptic_gregorian",
             "noleap",
             "365_day",
             "all_leap",
             "366_day",
             "360_day",
             "julian",
             "none",
         }
 
         ret_val = []
 
+        def check_standard_calendar_no_cross(time_var):
+            """
+            Check that the time variable does not cross the date
+            1582-10-15 when standard or gregorian calendars are used
+            """
+            # IMPLEMENTATION CONFORMANCE 4.4.1 RECOMMENDED 2/2
+            # Only get non-nan/FillValue times, as these are the only things
+            # that make sense for conversion.  Furthermore, non-null checks
+            # should be made for time coordinate variables anyways, so errors
+            # should be caught where implemented there
+            crossover_date = cftime.DatetimeGregorian(1582, 10, 15)
+            # has_year_zero set to true in order to just check crossover,
+            # actual year less than or equal to zero check handled elsewhere
+            # when standard/Gregorian, or Julian calendars used.
+
+            # WARNING: might fail here if months_since are used and suppress
+            #          usual warning
+            try:
+                times = cftime.num2date(
+                    time_var[:].compressed(),
+                    time_var.units,
+                    has_year_zero=True,
+                )
+            except ValueError:
+                return Result(
+                    BaseCheck.LOW,
+                    False,
+                    self.section_titles["4.4"],
+                    [
+                        "Miscellaneous failure when attempting to calculate crossover, possible malformed date",
+                    ],
+                )
+
+            crossover_1582 = np.any(times < crossover_date) and np.any(
+                times >= crossover_date,
+            )
+            if not crossover_1582:
+                reasoning = (
+                    f"Variable {time_var.name} has standard or Gregorian "
+                    "calendar and does not cross 1582-10-15T00:00Z"
+                )
+            else:
+                reasoning = (
+                    f"Variable {time_var.name} has time values "
+                    "prior to 1582-10-15T00:00Z and utilizes "
+                    "the standard or Gregorian calendar"
+                )
+
+            return Result(
+                BaseCheck.LOW,
+                not crossover_1582,
+                self.section_titles["4.4"],
+                [reasoning],
+            )
+
         # if has a calendar, check that it is within the valid values
         # otherwise no calendar is valid
-        for time_var in ds.get_variables_by_attributes(
-            calendar=lambda c: c is not None
-        ):
-            reasoning = None
-            standard_calendar = time_var.calendar in valid_calendars
 
+        # this will only fetch variables with time units defined
+        for time_var_name in cfutil.get_time_variables(ds):
+            if time_var_name not in {var.name for var in util.find_coord_vars(ds)}:
+                continue
+            time_var = ds.variables[time_var_name]
+            if not hasattr(time_var, "calendar"):
+                continue
+            if time_var.calendar.lower() == "gregorian":
+                reasoning = (
+                    f"For time variable {time_var.name}, when using "
+                    "the standard Gregorian calendar, the value "
+                    '"standard" is preferred over "gregorian" for '
+                    "the calendar attribute"
+                )
+                result = Result(
+                    BaseCheck.LOW,
+                    False,
+                    self.section_titles["4.4.1"],
+                    [reasoning],
+                )
+                ret_val.append(result)
+                # check here and in the below case that time does not cross
+                # thee date 1582-10-15 as requested by CF conformance
+                ret_val.append(check_standard_calendar_no_cross(time_var))
+            elif time_var.calendar == "standard":
+                ret_val.append(check_standard_calendar_no_cross(time_var))
             # if a nonstandard calendar, then leap_years and leap_months must
             # must be present
-            if not standard_calendar:
+            if time_var.calendar.lower() not in standard_calendars:
                 result = self._check_leap_time(time_var)
             # passes if the calendar is valid, otherwise notify of invalid
             # calendar
             else:
-                result = Result(
-                    BaseCheck.LOW, True, self.section_titles["4.4"], reasoning
-                )
-
+                result = Result(BaseCheck.LOW, True, self.section_titles["4.4.1"])
             ret_val.append(result)
 
         return ret_val
 
     def _check_leap_time(self, time_variable):
         """
         Helper method to handle checking custom calendar leap time specifiations
@@ -1852,15 +2067,15 @@
             hasattr(time_variable.month_lengths, "dtype")
             and np.issubdtype(time_variable.month_lengths.dtype, np.integer)
             and time_variable.month_lengths.size == 12
         ):
             leap_time.messages.append(
                 f"For nonstandard calendar on variable {time_variable.name}, "
                 "attribute month_lengths must be supplied as a 12-element "
-                "integer array"
+                "integer array",
             )
             return leap_time.to_result()
         # If leap years are included, then attributes leap_month and
         # leap_year must be included.
         has_leap_year = hasattr(time_variable, "leap_year")
         # IMPLEMENTATION CONFORMANCE 4.4.1 REQUIRED 4,5/5
         if hasattr(time_variable, "leap_month"):
@@ -1921,20 +2136,20 @@
 
         # for contiguous ragged array/indexed ragged array representations,
         # coordinates are not required to adhere to the same principles;
         # these representaitions can be identified by two attributes:
 
         # required for contiguous
         count_vars = ds.get_variables_by_attributes(
-            sample_dimension=lambda x: x is not None
+            sample_dimension=lambda x: x is not None,
         )
 
         # required for indexed
         index_vars = ds.get_variables_by_attributes(
-            instance_dimension=lambda x: x is not None
+            instance_dimension=lambda x: x is not None,
         )
 
         # if these attributes exist, we don't need to test
         # the coordinates
         if count_vars or index_vars:
             return ret_val
 
@@ -1972,15 +2187,18 @@
 
                 aux_coord_dims = set(ds.variables[aux_coord].dimensions)
                 valid_aux_coords.assert_true(
                     aux_coord_dims.issubset(dim_set),
                     "dimensions for auxiliary coordinate variable {} ({}) "
                     "are not a subset of dimensions for variable {} ({})"
                     "".format(
-                        aux_coord, ", ".join(aux_coord_dims), name, ", ".join(dim_set)
+                        aux_coord,
+                        ", ".join(aux_coord_dims),
+                        name,
+                        ", ".join(dim_set),
                     ),
                 )
             ret_val.append(valid_aux_coords.to_result())
         return ret_val
 
     def check_duplicate_axis(self, ds):
         """
@@ -2013,15 +2231,17 @@
             # coordinates. axis_map includes coordinates that don't actually have
             # an axis attribute, so we need to ignore those here.
             for axis, coords in axis_map.items():
                 coords = [c for c in coords if hasattr(ds.variables[c], "axis")]
                 no_duplicates.assert_true(
                     len(coords) <= 1,
                     "'{}' has duplicate axis {} defined by [{}]".format(
-                        name, axis, ", ".join(sorted(coords))
+                        name,
+                        axis,
+                        ", ".join(sorted(coords)),
                     ),
                 )
 
             ret_val.append(no_duplicates.to_result())
 
         return ret_val
 
@@ -2109,15 +2329,15 @@
             msg = (
                 '{}\'s coordinate variable "{}" is not one of the variables identifying true '
                 + "latitude/longitude and its dimensions are not a subset of {}'s dimensions"
             )
 
             alt = (
                 "{} has no coordinate associated with a variable identified as true latitude/longitude; "
-                + "its coordinate variable should also share a subset of {}'s dimensions"
+                "its coordinate variable should also share a subset of {}'s dimensions"
             )
 
             # Make sure we can find latitude and its dimensions are a subset
             _lat = None
             found_lat = False
             for lat in axis_map["Y"]:
                 _lat = lat
@@ -2188,19 +2408,19 @@
                 continue
 
             coord_set = set(coords.split())
 
             # Make sure it's associated with valid lat and valid lon
             valid_rgrid.assert_true(
                 len(coord_set.intersection(lons)) > 0,
-                "{} must be associated with a valid longitude coordinate".format(name),
+                f"{name} must be associated with a valid longitude coordinate",
             )
             valid_rgrid.assert_true(
                 len(coord_set.intersection(lats)) > 0,
-                "{} must be associated with a valid latitude coordinate".format(name),
+                f"{name} must be associated with a valid latitude coordinate",
             )
             valid_rgrid.assert_true(
                 len(axis_map["C"]) == 1,
                 "{} can not be associated with more than one compressed coordinates: "
                 "({})".format(name, ", ".join(axis_map["C"])),
             )
 
@@ -2257,15 +2477,15 @@
             return self._evaluate_standard_parallel(attr)
 
         elif attr_name == "straight_vertical_longitude_from_pole":
             return self._evaluate_straight_vertical_longitude_from_pole(attr)
 
         else:
             raise NotImplementedError(
-                "Evaluation for {} not yet implemented".format(attr_name)
+                f"Evaluation for {attr_name} not yet implemented",
             )
 
     def _evaluate_latitude_of_projection_origin(self, val):
         """
         Evaluate the condition for `latitude_of_projection_origin` attribute.
         Return result. Value must be -90 <= x <= 90.
 
@@ -2473,15 +2693,16 @@
             valid_region = TestCtx(BaseCheck.MEDIUM, self.section_titles["6.1"])
             region = var[:]
             if np.ma.isMA(region):
                 region = region.data
             valid_region.assert_true(
                 "".join(region.astype(str)).lower() in region_list,
                 "6.1.1 '{}' specified by '{}' is not a valid region".format(
-                    "".join(region.astype(str)), var.name
+                    "".join(region.astype(str)),
+                    var.name,
                 ),
             )
             ret_val.append(valid_region.to_result())
         return ret_val
 
     ###############################################################################
     # Chapter 7: Data Representative of Cells
@@ -2528,59 +2749,60 @@
         :return: List of results
         """
 
         # Note that test does not check monotonicity
         ret_val = []
         reasoning = []
         for variable_name, boundary_variable_name in cfutil.get_cell_boundary_map(
-            ds
+            ds,
         ).items():
             variable = ds.variables[variable_name]
             valid = True
             reasoning = []
             if boundary_variable_name not in ds.variables:
                 valid = False
                 reasoning.append(
                     "Boundary variable {} referenced by {} not ".format(
-                        boundary_variable_name, variable.name
+                        boundary_variable_name,
+                        variable.name,
                     )
-                    + "found in dataset variables"
+                    + "found in dataset variables",
                 )
             else:
                 boundary_variable = ds.variables[boundary_variable_name]
             # The number of dimensions in the bounds variable should always be
             # the number of dimensions in the referring variable + 1
             if boundary_variable.ndim < 2:
                 valid = False
                 reasoning.append(
                     "Boundary variable {} specified by {}".format(
-                        boundary_variable.name, variable.name
+                        boundary_variable.name,
+                        variable.name,
                     )
                     + " should have at least two dimensions to enclose the base "
-                    + "case of a one dimensionsal variable"
+                    + "case of a one dimensionsal variable",
                 )
             if boundary_variable.ndim != variable.ndim + 1:
                 valid = False
                 reasoning.append(
-                    "The number of dimensions of the variable %s is %s, but the "
-                    "number of dimensions of the boundary variable %s is %s. The boundary variable "
-                    "should have %s dimensions"
-                    % (
+                    "The number of dimensions of the variable {} is {}, but the "
+                    "number of dimensions of the boundary variable {} is {}. The boundary variable "
+                    "should have {} dimensions".format(
                         variable.name,
                         variable.ndim,
                         boundary_variable.name,
                         boundary_variable.ndim,
                         variable.ndim + 1,
-                    )
+                    ),
                 )
             if variable.dimensions[:] != boundary_variable.dimensions[: variable.ndim]:
                 valid = False
                 reasoning.append(
                     "Boundary variable coordinates (for {}) are in improper order: {}. Bounds-specific dimensions should be last"
-                    "".format(variable.name, boundary_variable.dimensions)
+                    "".format(variable.name, boundary_variable.dimensions),
                 )
 
             # ensure p vertices form a valid simplex given previous a...n
             # previous auxiliary coordinates
             if (
                 ds.dimensions[boundary_variable.dimensions[-1]].size
                 < len(boundary_variable.dimensions[:-1]) + 1
@@ -2588,22 +2810,110 @@
                 valid = False
                 reasoning.append(
                     "Dimension {} of boundary variable (for {}) must have at least {} elements to form a simplex/closed cell with previous dimensions {}.".format(
                         boundary_variable.name,
                         variable.name,
                         len(variable.dimensions) + 1,
                         boundary_variable.dimensions[:-1],
-                    )
+                    ),
                 )
             result = Result(
-                BaseCheck.MEDIUM, valid, self.section_titles["7.1"], reasoning
+                BaseCheck.MEDIUM,
+                valid,
+                self.section_titles["7.1"],
+                reasoning,
             )
             ret_val.append(result)
         return ret_val
 
+    def _cell_measures_core(self, ds, var, external_set, variable_template):
+        # IMPLEMENTATION CONFORMANCE REQUIRED 1/2
+        reasoning = []
+        search_str = (
+            r"^(?P<measure_type>area|volume):\s+(?P<cell_measure_var_name>\w+)$"
+        )
+        search_res = regex.match(search_str, var.cell_measures)
+        if not search_res:
+            valid = False
+            reasoning.append(
+                "The cell_measures attribute for variable {} "
+                "is formatted incorrectly. It should take the "
+                "form of either 'area: cell_var' or "
+                "'volume: cell_var' where cell_var is an existing name of "
+                "a variable describing the cell measures.".format(var.name),
+            )
+        else:
+            valid = True
+            cell_measure_var_name = search_res.group("cell_measure_var_name")
+            cell_measure_type = search_res.group("measure_type")
+            # TODO: cache previous results
+            if cell_measure_var_name not in set(ds.variables.keys()).union(
+                external_set,
+            ):
+                valid = False
+                reasoning.append(
+                    f"Cell measure variable {cell_measure_var_name} referred to by "
+                    f"{var.name} is not present in {variable_template}s".format(
+                        cell_measure_var_name,
+                        var.name,
+                    ),
+                )
+            # CF 1.7+ assume external variables -- further checks can't be run here
+            elif cell_measure_var_name in external_set:
+                # can't test anything on an external var
+                return Result(
+                    BaseCheck.MEDIUM,
+                    valid,
+                    (self.section_titles["7.2"]),
+                    reasoning,
+                )
+
+            else:
+                cell_measure_var = ds.variables[cell_measure_var_name]
+                if not hasattr(cell_measure_var, "units"):
+                    valid = False
+                    reasoning.append(
+                        "Cell measure variable {} is required "
+                        "to have units attribute defined".format(cell_measure_var_name),
+                    )
+                else:
+                    # IMPLEMENTATION CONFORMANCE REQUIRED 2/2
+                    # verify this combination {area: 'm2', volume: 'm3'}
+
+                    # key is valid measure types, value is expected
+                    # exponent
+                    exponent_lookup = {"area": 2, "volume": 3}
+                    exponent = exponent_lookup[search_res.group("measure_type")]
+                    conversion_failure_msg = (
+                        f'Variable "{cell_measure_var.name}" must have units which are convertible '
+                        f'to UDUNITS "m{exponent}" when variable is referred to by a {variable_template} with '
+                        f'cell_methods attribute with a measure type of "{cell_measure_type}".'
+                    )
+                    try:
+                        cell_measure_units = Unit(cell_measure_var.units)
+                    except ValueError:
+                        valid = False
+                        reasoning.append(conversion_failure_msg)
+                    else:
+                        if not cell_measure_units.is_convertible(Unit(f"m{exponent}")):
+                            valid = False
+                            reasoning.append(conversion_failure_msg)
+                    if not set(cell_measure_var.dimensions).issubset(var.dimensions):
+                        valid = False
+                        reasoning.append(
+                            "Cell measure variable {} must have "
+                            "dimensions which are a subset of "
+                            "those defined in variable {}.".format(
+                                cell_measure_var_name,
+                                var.name,
+                            ),
+                        )
+
+        return Result(BaseCheck.MEDIUM, valid, (self.section_titles["7.2"]), reasoning)
+
     def check_cell_measures(self, ds):
         """
         7.2 To indicate extra information about the spatial properties of a
         variable's grid cells, a cell_measures attribute may be defined for a
         variable. This is a string attribute comprising a list of
         blank-separated pairs of words of the form "measure: name". "area" and
         "volume" are the only defined measures.
@@ -2618,66 +2928,19 @@
         such as a standard_name.
 
         :param netCDF4.Dataset ds: An open netCDF dataset
         :rtype: list
         :return: List of results
         """
         ret_val = []
-        reasoning = []
         variables = ds.get_variables_by_attributes(
-            cell_measures=lambda c: c is not None
+            cell_measures=lambda c: c is not None,
         )
         for var in variables:
-            # IMPLEMENTATION CONFORMANCE REQUIRED 1/2
-            search_str = r"^(?:area|volume): (\w+)$"
-            search_res = regex.search(search_str, var.cell_measures)
-            if not search_res:
-                valid = False
-                reasoning.append(
-                    "The cell_measures attribute for variable {} "
-                    "is formatted incorrectly.  It should take the"
-                    " form of either 'area: cell_var' or "
-                    "'volume: cell_var' where cell_var is the "
-                    "variable describing the cell measures".format(var.name)
-                )
-            else:
-                valid = True
-                cell_meas_var_name = search_res.groups()[0]
-                # TODO: cache previous results
-                if cell_meas_var_name not in ds.variables:
-                    valid = False
-                    reasoning.append(
-                        "Cell measure variable {} referred to by "
-                        "{} is not present in dataset variables".format(
-                            cell_meas_var_name, var.name
-                        )
-                    )
-                else:
-                    cell_meas_var = ds.variables[cell_meas_var_name]
-                    if not hasattr(cell_meas_var, "units"):
-                        valid = False
-                        reasoning.append(
-                            "Cell measure variable {} is required "
-                            "to have units attribute defined.".format(
-                                cell_meas_var_name
-                            )
-                        )
-                    if not set(cell_meas_var.dimensions).issubset(var.dimensions):
-                        valid = False
-                        reasoning.append(
-                            "Cell measure variable {} must have "
-                            "dimensions which are a subset of "
-                            "those defined in variable {}.".format(
-                                cell_meas_var_name, var.name
-                            )
-                        )
-
-            result = Result(
-                BaseCheck.MEDIUM, valid, (self.section_titles["7.2"]), reasoning
-            )
+            result = self._cell_measures_core(ds, var, set(), "dataset variable")
             ret_val.append(result)
 
         return ret_val
 
     def check_cell_methods(self, ds):
         """
         7.3 To describe the characteristic of a field that is represented by cell values, we define the cell_methods attribute
@@ -2702,25 +2965,26 @@
         :return: List of results
         """
 
         ret_val = []
         # CONFORMANCE IMPLEMENTATION 7.3 1/3
         psep = regex.compile(
             r"(?P<vars>\w+: )+(?P<method>\w+) ?(?P<where>where (?P<wtypevar>\w+) "
-            r"?(?P<over>over (?P<otypevar>\w+))?| ?)(?:\((?P<paren_contents>[^)]*)\))?"
+            r"?(?P<over>over (?P<otypevar>\w+))?| ?)(?:\((?P<paren_contents>[^)]*)\))?",
         )
 
         for var in ds.get_variables_by_attributes(cell_methods=lambda x: x is not None):
             if not getattr(var, "cell_methods", ""):
                 continue
 
             method = getattr(var, "cell_methods", "")
 
             valid_attribute = TestCtx(
-                BaseCheck.HIGH, self.section_titles["7.3"]
+                BaseCheck.HIGH,
+                self.section_titles["7.3"],
             )  # changed from 7.1 to 7.3
             valid_attribute.assert_true(
                 regex.match(psep, method) is not None,
                 '"{}" is not a valid format for cell_methods attribute of "{}"'
                 "".format(method, var.name),
             )
             ret_val.append(valid_attribute.to_result())
@@ -2735,15 +2999,14 @@
                     # strip off the ' :' at the end of each match
                     var_str = var_raw_str[:-2]
                     if (
                         var_str in var.dimensions
                         or var_str == "area"
                         or var_str in getattr(var, "coordinates", "")
                     ):
-
                         valid = True
                     else:
                         valid = False
 
                     valid_cell_names.assert_true(
                         valid,
                         "{}'s cell_methods name component {} does not match a dimension, "
@@ -2767,16 +3030,17 @@
 
             for match in regex.finditer(psep, method):
                 if match.group("paren_contents") is not None:
                     # split along spaces followed by words with a colon
                     # not sure what to do if a comment contains a colon!
                     ret_val.append(
                         self._check_cell_methods_paren_info(
-                            match.group("paren_contents"), var
-                        ).to_result()
+                            match.group("paren_contents"),
+                            var,
+                        ).to_result(),
                     )
 
         return ret_val
 
     def _check_cell_methods_paren_info(self, paren_contents, var):
         """
         Checks that the spacing and/or comment info contained inside the
@@ -2793,89 +3057,95 @@
         # otherwise, split into k/v pairs
         kv_pair_pat = r"(\S+:)\s+(.*(?=\s+\w+:)|[^:]+$)\s*"
         # otherwise, we must split further with intervals coming
         # first, followed by non-standard comments
         # we need the count of the matches, and re.findall() only returns
         # groups if they are present and we wish to see if the entire match
         # object concatenated together is the same as the original string
-        pmatches = [m for m in regex.finditer(kv_pair_pat, paren_contents)]
+        pmatches = list(regex.finditer(kv_pair_pat, paren_contents))
         for i, pmatch in enumerate(pmatches):
             keyword, val = pmatch.groups()
             if keyword == "interval:":
                 valid_info.out_of += 2
                 interval_matches = regex.match(
-                    r"^\s*(?P<interval_number>\S+)\s+(?P<interval_units>\S+)\s*$", val
+                    r"^\s*(?P<interval_number>\S+)\s+(?P<interval_units>\S+)\s*$",
+                    val,
                 )
                 # attempt to get the number for the interval
                 if not interval_matches:
                     valid_info.messages.append(
                         '§7.3.3 {}:cell_methods contains an interval specification that does not parse: "{}". Should be in format "interval: <number> <units>"'.format(
-                            var.name, val
-                        )
+                            var.name,
+                            val,
+                        ),
                     )
                 else:
                     try:
                         float(interval_matches.group("interval_number"))
                     except ValueError:
                         valid_info.messages.append(
                             '§7.3.3 {}:cell_methods contains an interval value that does not parse as a numeric value: "{}".'.format(
-                                var.name, interval_matches.group("interval_number")
-                            )
+                                var.name,
+                                interval_matches.group("interval_number"),
+                            ),
                         )
                     else:
                         valid_info.score += 1
 
                     # then the units
                     try:
                         Unit(interval_matches.group("interval_units"))
                     except ValueError:
                         valid_info.messages.append(
                             '§7.3.3 {}:cell_methods interval units "{}" is not parsable by UDUNITS.'.format(
-                                var.name, interval_matches.group("interval_units")
-                            )
+                                var.name,
+                                interval_matches.group("interval_units"),
+                            ),
                         )
                     else:
                         valid_info.score += 1
             elif keyword == "comment:":
                 # comments can't really be invalid, except
                 # if they come first or aren't last, and
                 # maybe if they contain colons embedded in the
                 # comment string
                 valid_info.out_of += 1
                 if len(pmatches) == 1:
                     valid_info.messages.append(
                         "§7.3.3 If there is no standardized information, the keyword comment: should be omitted for variable {}".format(
-                            var.name
-                        )
+                            var.name,
+                        ),
                     )
                 # otherwise check that the comment is the last
                 # item in the parentheses
                 elif i != len(pmatches) - 1:
                     valid_info.messages.append(
                         '§7.3.3 The non-standard "comment:" element must come after any standard elements in cell_methods for variable {}'.format(
-                            var.name
-                        )
+                            var.name,
+                        ),
                     )
                 #
                 else:
                     valid_info.score += 1
             else:
                 valid_info.out_of += 1
                 valid_info.messages.append(
                     '§7.3.3 Invalid cell_methods keyword "{}" for variable {}. Must be one of [interval, comment]'.format(
-                        keyword, var.name
-                    )
+                        keyword,
+                        var.name,
+                    ),
                 )
 
         # Ensure concatenated reconstructed matches are the same as the
         # original string.  If they're not, there's likely a formatting error
         valid_info.assert_true(
             "".join(m.group(0) for m in pmatches) == paren_contents,
             "§7.3.3 Parenthetical content inside {}:cell_methods is not well formed: {}".format(
-                var.name, paren_contents
+                var.name,
+                paren_contents,
             ),
         )
 
         return valid_info
 
     def check_climatological_statistics(self, ds):
         """
@@ -2918,68 +3188,89 @@
             "mode",
             "median",
         ]
 
         # find any climatology axis variables; any variables which contain climatological stats will use
         # these variables as coordinates
         clim_time_coord_vars = ds.get_variables_by_attributes(
-            climatology=lambda s: s is not None
+            climatology=lambda s: s is not None,
         )
 
         # first, to determine whether or not we have a valid climatological time
         # coordinate variable, we need to make sure it has the attribute "climatology",
         # but not the attribute "bounds"
-
+        time_vars = cfutil.get_time_variables(ds)
         for clim_coord_var in clim_time_coord_vars:
             climatology_ctx = TestCtx(BaseCheck.MEDIUM, self.section_titles["7.3"])
+            # IMPLEMENTATION CONFORMANCE 7.4 REQUIRED 1/6
+            if clim_coord_var.name not in time_vars:
+                climatology_ctx.out_of += 1
+                climatology_ctx.messages.append(
+                    f"Variable {clim_coord_var.name} is not detected as a time "
+                    "coordinate variable, but has climatology attribute",
+                )
+            # IMPLEMENTATION CONFORMANCE 7.4 REQUIRED
             if hasattr(clim_coord_var, "bounds"):
                 climatology_ctx.out_of += 1
                 climatology_ctx.messages.append(
                     f"Variable {clim_coord_var.name} has a climatology "
-                    "attribute and cannot also have a bounds attribute."
+                    "attribute and cannot also have a bounds attribute.",
                 )
                 result = Result(
-                    BaseCheck.MEDIUM, False, (self.section_titles["7.4"]), reasoning
+                    BaseCheck.MEDIUM,
+                    False,
+                    (self.section_titles["7.4"]),
+                    reasoning,
                 )
 
             # IMPLEMENTATION CONFORMANCE 7.4 REQUIRED 2/6
             # make sure the climatology variable referenced actually exists
+            elif not isinstance(clim_coord_var.climatology, str):
+                climatology_ctx.out_of += 1
+                climatology_ctx.messages.append(
+                    f"Variable {clim_coord_var.name} must have a climatology "
+                    "attribute which is a string",
+                )
+                ret_val.append(climatology_ctx.to_result())
+                continue
             elif clim_coord_var.climatology not in ds.variables:
                 climatology_ctx.out_of += 1
                 climatology_ctx.messages.append(
                     "Variable {} referenced in time's climatology attribute does not exist".format(
-                        ds.variables["time"].climatology
-                    )
+                        ds.variables["time"].climatology,
+                    ),
                 )
             else:
-                # IMPLEMENTATION CONFORMANCE 7.4 REQUIRED 4/6
                 clim_var = ds.variables[clim_coord_var.climatology]
+                #
+                # IMPLEMENTATION CONFORMANCE 7.4 REQUIRED 4/6
                 if clim_var.dtype is str or not np.issubdtype(clim_var, np.number):
                     climatology_ctx.out_of += 1
                     climatology_ctx.messages.append(
-                        f"Climatology variable {clim_var.name} is not a numeric type"
+                        f"Climatology variable {clim_var.name} is not a numeric type",
                     )
-                # IMPLEMENTATION CONFORMANCE REQUIRED 6/6
+                # IMPLEMENTATION CONFORMANCE 7.4 REQUIRED 6/6
                 if hasattr(clim_var, "_FillValue") or hasattr(
-                    clim_var, "missing_value"
+                    clim_var,
+                    "missing_value",
                 ):
                     climatology_ctx.out_of += 1
                     climatology_ctx.messages.append(
-                        f"Climatology variable {clim_var.name} may not contain"
-                        "attributes _FillValue or missing_value"
+                        f"Climatology variable {clim_var.name} may not contain "
+                        "attributes _FillValue or missing_value",
                     )
 
                 # IMPLEMENTATION CONFORMANCE 7.4 REQUIRED 5/6
                 for same_attr in ("units", "standard_name", "calendar"):
                     if hasattr(clim_var, same_attr):
                         climatology_ctx.assert_true(
                             getattr(clim_var, same_attr)
                             == getattr(clim_coord_var, same_attr, None),
                             f"Attribute {same_attr} must have the same value in both "
-                            "variables {clim_var.name} and {clim_coord_var.name}",
+                            f"variables {clim_var.name} and {clim_coord_var.name}",
                         )
             ret_val.append(climatology_ctx.to_result())
 
             # check that coordinate bounds are in the proper order.
             # make sure last elements are boundary variable specific dimensions
             # IMPLEMENTATION CONFORMANCE 7.4 REQUIRED 3/6
             if (
@@ -2987,16 +3278,16 @@
                 != ds.variables[clim_coord_var.climatology].dimensions[
                     : clim_coord_var.ndim
                 ]
             ):
                 total_climate_count += 1
                 reasoning.append(
                     "Climatology variable coordinates are in improper order: {}. Bounds-specific dimensions should be last".format(
-                        ds.variables[clim_coord_var.climatology].dimensions
-                    )
+                        ds.variables[clim_coord_var.climatology].dimensions,
+                    ),
                 )
                 result = Result(
                     BaseCheck.MEDIUM,
                     (valid_climate_count, total_climate_count),
                     (self.section_titles["7.4"]),
                     reasoning,
                 )
@@ -3008,16 +3299,16 @@
                 ds.dimensions[
                     ds.variables[clim_coord_var.climatology].dimensions[-1]
                 ].size
                 != 2
             ):
                 reasoning.append(
                     'Climatology dimension "{}" should only contain two elements'.format(
-                        ds.variables[clim_coord_var.climatology].name
-                    )
+                        ds.variables[clim_coord_var.climatology].name,
+                    ),
                 )
                 total_climate_count += 1
                 result = Result(
                     BaseCheck.MEDIUM,
                     (valid_climate_count, total_climate_count),
                     (self.section_titles["7.4"]),
                     reasoning,
@@ -3033,35 +3324,35 @@
         #     time: method1 within days time: method2 over days
         #     time: method1 within days time: method2 over days time: method3 over years
         # optionally followed by parentheses for explaining additional
         # info, e.g.
         # "time: method1 within years time: method2 over years (sidereal years)"
 
         meth_regex = "(?:{})".format(
-            "|".join(methods)
+            "|".join(methods),
         )  # "or" comparison for the methods
         re_string = (
             r"^time: {0} within (years|days)"  # regex string to test
             r" time: {0} over \1(?<=days)(?: time: {0} over years)?"
             r"(?: \([^)]+\))?$".format(meth_regex)
         )
 
         # find any variables with a valid climatological cell_methods
         for cell_method_var in ds.get_variables_by_attributes(
-            cell_methods=lambda s: s is not None
+            cell_methods=lambda s: s is not None,
         ):
             if any(
-                [dim in all_clim_coord_var_names for dim in cell_method_var.dimensions]
+                dim in all_clim_coord_var_names for dim in cell_method_var.dimensions
             ):
                 total_climate_count += 1
                 if not regex.search(re_string, cell_method_var.cell_methods):
                     reasoning.append(
                         'The "time: method within years/days over years/days" format is not correct in variable {}.'.format(
-                            cell_method_var.name
-                        )
+                            cell_method_var.name,
+                        ),
                     )
                 else:
                     valid_climate_count += 1
 
                 result = Result(
                     BaseCheck.MEDIUM,
                     (valid_climate_count, total_climate_count),
@@ -3096,15 +3387,14 @@
 
         :param netCDF4.Dataset ds: An open netCDF dataset
         :rtype: list
         :return: List of results
         """
         ret_val = []
         for name, var in ds.variables.items():
-
             add_offset = getattr(var, "add_offset", None)
             scale_factor = getattr(var, "scale_factor", None)
             if not (add_offset or scale_factor):
                 continue
 
             valid = True
             reasoning = []
@@ -3117,83 +3407,85 @@
                 scale_factor = add_offset
 
             # IMPLEMENTATION CONFORMANCE 8.1 REQUIRED 1/3
             # scale_factor and add_offset same type
             if type(add_offset) != type(scale_factor):
                 valid = False
                 reasoning.append(
-                    "Attributes add_offset and scale_factor have different data type."
+                    "Attributes add_offset and scale_factor have different data type.",
                 )
             # IMPLEMENTATION CONFORMANCE 8.1 REQUIRED 2/3
             # scale_factor and add_offset must be floating point or double
             # if not the same type
             # FIXME: Check add_offset too.
 
             elif type(scale_factor) != var.dtype.type:
                 # Check both attributes are type float or double
                 if not isinstance(scale_factor, (float, np.floating)):
                     valid = False
                     reasoning.append(
-                        "Attributes add_offset and scale_factor are not of type float or double."
+                        "Attributes add_offset and scale_factor are not of type float or double.",
                     )
                 else:
                     # Check variable type is byte, short or int
                     if var.dtype.type not in [
-                        np.int,
+                        int,
                         np.int8,
                         np.int16,
                         np.int32,
                         np.int64,
                     ]:
                         valid = False
                         # IMPLEMENTATION CONFORMANCE REQUIRED 3/3
                         # IMPLEMENTATION CONFORMANCE REQUIRED 3/3
                         reasoning.append(
-                            "Variable is not of type byte, short, or int as required for different type add_offset/scale_factor."
+                            "Variable is not of type byte, short, or int as required for different type add_offset/scale_factor.",
                         )
 
             result = Result(
-                BaseCheck.MEDIUM, valid, self.section_titles["8.1"], reasoning
+                BaseCheck.MEDIUM,
+                valid,
+                self.section_titles["8.1"],
+                reasoning,
             )
             ret_val.append(result)
             reasoning = []
 
             valid = True
             # test further with  _FillValue , valid_min , valid_max , valid_range
             if hasattr(var, "_FillValue"):
                 if var._FillValue.dtype.type != var.dtype.type:
                     valid = False
                     reasoning.append(
-                        "Type of %s:_FillValue attribute (%s) does not match variable type (%s)"
-                        % (name, var._FillValue.dtype.name, var.dtype.name)
+                        f"Type of {name}:_FillValue attribute ({var._FillValue.dtype.name}) does not match variable type ({var.dtype.name})",
                     )
             if hasattr(var, "valid_min"):
                 if var.valid_min.dtype.type != var.dtype.type:
                     valid = False
                     reasoning.append(
-                        "Type of %svalid_min attribute (%s) does not match variable type (%s)"
-                        % (name, var.valid_min.dtype.name, var.dtype.name)
+                        f"Type of {name}valid_min attribute ({var.valid_min.dtype.name}) does not match variable type ({var.dtype.name})",
                     )
             if hasattr(var, "valid_max"):
                 if var.valid_max.dtype.type != var.dtype.type:
                     valid = False
                     reasoning.append(
-                        "Type of %s:valid_max attribute (%s) does not match variable type (%s)"
-                        % (name, var.valid_max.dtype.name, var.dtype.name)
+                        f"Type of {name}:valid_max attribute ({var.valid_max.dtype.name}) does not match variable type ({var.dtype.name})",
                     )
             if hasattr(var, "valid_range"):
                 if var.valid_range.dtype.type != var.dtype.type:
                     valid = False
                     reasoning.append(
-                        "Type of %s:valid_range attribute (%s) does not match variable type (%s)"
-                        % (name, var.valid_range.dtype.name, var.dtype.name)
+                        f"Type of {name}:valid_range attribute ({var.valid_range.dtype.name}) does not match variable type ({var.dtype.name})",
                     )
 
             result = Result(
-                BaseCheck.MEDIUM, valid, self.section_titles["8.1"], reasoning
+                BaseCheck.MEDIUM,
+                valid,
+                self.section_titles["8.1"],
+                reasoning,
             )
             ret_val.append(result)
 
         return ret_val
 
     def check_compression_gathering(self, ds):
         """
@@ -3231,53 +3523,79 @@
 
         :param netCDF4.Dataset ds: An open netCDF dataset
         :rtype: list
         :return: List of results
         """
         ret_val = []
         for compress_var in ds.get_variables_by_attributes(
-            compress=lambda s: s is not None
+            compress=lambda s: s is not None,
         ):
             valid = True
             reasoning = []
             # puts the referenced variable being compressed into a set
             compress_set = set(compress_var.compress.split(" "))
             if compress_var.ndim != 1:
                 valid = False
                 reasoning.append(
                     "Compression variable {} may only have one dimension".format(
-                        compress_var.name
-                    )
+                        compress_var.name,
+                    ),
                 )
             # IMPLEMENTATION CONFORMANCE 8.2 REQUIRED 1/3
             # ensure compression variable is a proper index, and thus is an
             # signed or unsigned integer type of some sort
             if (compress_var.dtype is str) or (
                 compress_var.dtype.kind not in {"i", "u"}
             ):
                 valid = False
                 reasoning.append(
                     "Compression variable {} must be an integer type to form a proper array index".format(
-                        compress_var.name
-                    )
+                        compress_var.name,
+                    ),
                 )
             # IMPLEMENTATION CONFORMANCE 8.2 REQUIRED 2/3
             # make sure all the variables referred to are contained by the
             # variables.
             if not compress_set.issubset(ds.dimensions):
                 not_in_dims = sorted(compress_set.difference(ds.dimensions))
                 valid = False
                 reasoning.append(
                     "The following dimensions referenced by the compress attribute of variable {} do not exist: {}".format(
-                        compress_var.name, not_in_dims
-                    )
+                        compress_var.name,
+                        not_in_dims,
+                    ),
                 )
+            # IMPLEMENTATION CONFORMANCE 8.2 REQUIRED 3/3
+            # The values of the associated coordinate variable must be in the range
+            # starting with 0 and going up to the product of the compressed dimension
+            # sizes minus 1 (CDL index conventions).
+
+            # Put the the values of the associated coordinate variable into a list
+            coord_list_size = [
+                item.size
+                for item in ds.dimensions.values()
+                if item.name in compress_set
+            ]
+            # get the upper limt of the dimenssion size
+            upper_limit_size = np.prod(coord_list_size) - 1
 
+            for coord_size in coord_list_size:
+                if coord_size not in range(0, upper_limit_size):
+                    valid = False
+                    reasoning.append(
+                        "The dimenssion size {} referenced by the compress attribute is not "
+                        "in the range (0, The product of the compressed dimension sizes minus 1)".format(
+                            coord_size,
+                        ),
+                    )
             result = Result(
-                BaseCheck.MEDIUM, valid, self.section_titles["8.2"], reasoning
+                BaseCheck.MEDIUM,
+                valid,
+                self.section_titles["8.2"],
+                reasoning,
             )
             ret_val.append(result)
 
         return ret_val
 
     ###############################################################################
     # Chapter 9: Discrete Sampling Geometries
@@ -3304,15 +3622,16 @@
             "profile",
             "timeseriesprofile",
             "trajectoryprofile",
         ]
 
         feature_type = getattr(ds, "featureType", None)
         valid_feature_type = TestCtx(
-            BaseCheck.HIGH, "§9.1 Dataset contains a valid featureType"
+            BaseCheck.HIGH,
+            "§9.1 Dataset contains a valid featureType",
         )
         valid_feature_type.assert_true(
             feature_type is None or feature_type.lower() in feature_list,
             "{} is not a valid CF featureType. It must be one of {}"
             "".format(feature_type, ", ".join(feature_list)),
         )
         return valid_feature_type.to_result()
@@ -3389,15 +3708,15 @@
 
         # create explanation of all of the different featureTypes
         # found in the dataset
         feature_description = ", ".join(
             [
                 "{} ({})".format(ftr, ", ".join(vrs))
                 for ftr, vrs in feature_types_found.items()
-            ]
+            ],
         )
         all_same_features = TestCtx(BaseCheck.HIGH, self.section_titles["9.1"])
         all_same_features.assert_true(
             len(feature_types_found) < 2,
             "Different feature types discovered in this dataset: {}"
             "".format(feature_description),
         )
```

### Comparing `compliance-checker-5.0.2/compliance_checker/cf/cf_1_7.py` & `compliance-checker-5.1.0/compliance_checker/cf/cf_1_7.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 import logging
 import os
 import sqlite3
 from warnings import warn
 
 import numpy as np
 import pyproj
-import regex
 
 from compliance_checker import cfutil
 from compliance_checker.base import BaseCheck, Result, TestCtx
 from compliance_checker.cf.appendix_d import dimless_vertical_coordinates_1_7
 from compliance_checker.cf.appendix_e import cell_methods17
 from compliance_checker.cf.appendix_f import (
     ellipsoid_names17,
@@ -47,19 +46,19 @@
             },
             "external_variables": {
                 "Type": "S",
                 "attr_loc": {"G"},
                 "cf_section": "2.6.3",
             },
             "scale_factor": {"Type": "N", "attr_loc": {"D", "C"}, "cf_section": "8.1"},
-        }
+        },
     )
 
     def __init__(self, options=None):
-        super(CF1_7Check, self).__init__(options)
+        super().__init__(options)
 
         self.cell_methods = cell_methods17
         self.grid_mapping_dict = grid_mapping_dict17
         self.grid_mapping_attr_types = grid_mapping_attr_types17
 
     def check_external_variables(self, ds):
         """
@@ -120,106 +119,111 @@
             msgs = []
             score = 0
             out_of = 0
 
             if not hasattr(variable, "actual_range"):
                 continue  # having this attr is only suggested, no Result needed
             else:
-
                 out_of += 1
                 try:
                     if (
                         len(variable.actual_range) != 2
                     ):  # TODO is the attr also a numpy array? if so, .size
                         msgs.append(
-                            "actual_range of '{}' must be 2 elements".format(name)
+                            f"actual_range of '{name}' must be 2 elements",
                         )
                         ret_val.append(
                             Result(  # putting result into list
                                 BaseCheck.HIGH,
                                 (score, out_of),
                                 self.section_titles["2.5"],
                                 msgs,
-                            )
+                            ),
                         )
                         continue  # no need to keep checking if already completely wrong
                     else:
                         score += 1
                 except TypeError:  # in case it's just a single number
-                    msgs.append("actual_range of '{}' must be 2 elements".format(name))
+                    msgs.append(f"actual_range of '{name}' must be 2 elements")
                     ret_val.append(
                         Result(  # putting result into list
                             BaseCheck.HIGH,
                             (score, out_of),
                             self.section_titles["2.5"],
                             msgs,
-                        )
+                        ),
                     )
                     continue
 
                 # check equality to existing min/max values
                 # NOTE this is a data check
                 # If every value is masked, a data check of actual_range isn't
                 # appropriate, so skip.
                 if not (hasattr(variable[:], "mask") and variable[:].mask.all()):
                     # if min/max values aren't close to actual_range bounds,
                     # fail.
                     out_of += 1
                     if not np.isclose(
-                        variable.actual_range[0], variable[:].min()
+                        variable.actual_range[0],
+                        variable[:].min(),
                     ) or not np.isclose(variable.actual_range[1], variable[:].max()):
                         msgs.append(
                             "actual_range elements of '{}' inconsistent with its min/max values".format(
-                                name
-                            )
+                                name,
+                            ),
                         )
                     else:
                         score += 1
 
                 # check that the actual range is within the valid range
                 if hasattr(variable, "valid_range"):  # check within valid_range
                     out_of += 1
                     if (variable.actual_range[0] < variable.valid_range[0]) or (
                         variable.actual_range[1] > variable.valid_range[1]
                     ):
                         msgs.append(
                             '"{}"\'s actual_range must be within valid_range'.format(
-                                name
-                            )
+                                name,
+                            ),
                         )
                     else:
                         score += 1
 
                 # check the elements of the actual range have the appropriate
                 # relationship to the valid_min and valid_max
                 if hasattr(variable, "valid_min"):
                     out_of += 1
                     if variable.actual_range[0] < variable.valid_min:
                         msgs.append(
                             '"{}"\'s actual_range first element must be >= valid_min ({})'.format(
-                                name, variable.valid_min
-                            )
+                                name,
+                                variable.valid_min,
+                            ),
                         )
                     else:
                         score += 1
                 if hasattr(variable, "valid_max"):
                     out_of += 1
                     if variable.actual_range[1] > variable.valid_max:
                         msgs.append(
                             '"{}"\'s actual_range second element must be <= valid_max ({})'.format(
-                                name, variable.valid_max
-                            )
+                                name,
+                                variable.valid_max,
+                            ),
                         )
                     else:
                         score += 1
 
             ret_val.append(
                 Result(  # putting result into list
-                    BaseCheck.HIGH, (score, out_of), self.section_titles["2.5"], msgs
-                )
+                    BaseCheck.HIGH,
+                    (score, out_of),
+                    self.section_titles["2.5"],
+                    msgs,
+                ),
             )
         return ret_val
 
     def check_cell_boundaries(self, ds):
         """
         Checks the dimensions of cell boundary variables to ensure they are CF compliant
         per section 7.1.
@@ -234,94 +238,213 @@
         :returns list: List of results
         """
 
         # Note that test does not check monotonicity
         ret_val = []
         reasoning = []
         for variable_name, boundary_variable_name in cfutil.get_cell_boundary_map(
-            ds
+            ds,
         ).items():
             variable = ds.variables[variable_name]
             valid = True
             reasoning = []
+
+            # 7.1 Required 1/5:
+            # The type of the bounds attribute is a string whose value is a single variable name.
+            # The specified variable must exist in the file.
             if boundary_variable_name not in ds.variables:
                 valid = False
                 reasoning.append(
                     "Boundary variable {} referenced by {} not ".format(
-                        boundary_variable_name, variable.name
+                        boundary_variable_name,
+                        variable.name,
                     )
-                    + "found in dataset variables"
+                    + "found in dataset variables",
                 )
             else:
                 boundary_variable = ds.variables[boundary_variable_name]
+
+            # 7.1 Required 2/5:
             # The number of dimensions in the bounds variable should always be
             # the number of dimensions in the referring variable + 1
             if boundary_variable.ndim < 2:
                 valid = False
                 reasoning.append(
                     "Boundary variable {} specified by {}".format(
-                        boundary_variable.name, variable.name
+                        boundary_variable.name,
+                        variable.name,
                     )
                     + " should have at least two dimensions to enclose the base "
-                    + "case of a one dimensionsal variable"
+                    + "case of a one dimensionsal variable",
                 )
             if boundary_variable.ndim != variable.ndim + 1:
                 valid = False
                 reasoning.append(
-                    "The number of dimensions of the variable %s is %s, but the "
-                    "number of dimensions of the boundary variable %s is %s. The boundary variable "
-                    "should have %s dimensions"
-                    % (
+                    "The number of dimensions of the variable {} is {}, but the "
+                    "number of dimensions of the boundary variable {} is {}. The boundary variable "
+                    "should have {} dimensions".format(
                         variable.name,
                         variable.ndim,
                         boundary_variable.name,
                         boundary_variable.ndim,
                         variable.ndim + 1,
-                    )
+                    ),
                 )
             if variable.dimensions[:] != boundary_variable.dimensions[: variable.ndim]:
                 valid = False
                 reasoning.append(
                     "Boundary variable coordinates (for {}) are in improper order: {}. Bounds-specific dimensions should be last"
-                    "".format(variable.name, boundary_variable.dimensions)
+                    "".format(variable.name, boundary_variable.dimensions),
                 )
 
-            # ensure p vertices form a valid simplex given previous a...n
+            # 7.1 Required 2/5: continue
+            # Ensure p vertices form a valid simplex given previous a...n
             # previous auxiliary coordinates
             if (
                 ds.dimensions[boundary_variable.dimensions[-1]].size
                 < len(boundary_variable.dimensions[:-1]) + 1
             ):
                 valid = False
                 reasoning.append(
                     "Dimension {} of boundary variable (for {}) must have at least {} elements to form a simplex/closed cell with previous dimensions {}.".format(
                         boundary_variable.name,
                         variable.name,
                         len(variable.dimensions) + 1,
                         boundary_variable.dimensions[:-1],
+                    ),
+                )
+
+            # 7.1 Required 3/5:
+            # A boundary variable must be a numeric data type
+            if boundary_variable.dtype.kind not in "biufc":
+                valid = False
+                reasoning.append(
+                    "Boundary variable {} specified by {}".format(
+                        boundary_variable.name,
+                        variable.name,
                     )
+                    + "must be a numeric data type ",
                 )
 
+            # 7.1 Required 4/5:
+            # If a boundary variable has units, standard_name, axis, positive, calendar, leap_month,
+            # leap_year or month_lengths attributes, they must agree with those of its associated variable.
+            if boundary_variable.__dict__.keys():
+                for item in boundary_variable.__dict__.keys():
+                    if hasattr(variable, item):
+                        if getattr(variable, item) != getattr(boundary_variable, item):
+                            valid = False
+                            reasoning.append(
+                                "'{}' has attr '{}' with value '{}' that does not agree "
+                                "with its associated variable ('{}')'s attr value '{}'"
+                                "".format(
+                                    boundary_variable_name,
+                                    item,
+                                    getattr(boundary_variable, item),
+                                    variable.name,
+                                    getattr(variable, item),
+                                ),
+                            )
+
+            # 7.1 Required 5/5:
             # check if formula_terms is present in the var; if so,
             # the bounds variable must also have a formula_terms attr
             if hasattr(variable, "formula_terms"):
                 if not hasattr(boundary_variable, "formula_terms"):
                     valid = False
                     reasoning.append(
                         "'{}' has 'formula_terms' attr, bounds variable '{}' must also have 'formula_terms'".format(
-                            variable_name, boundary_variable_name
-                        )
+                            variable_name,
+                            boundary_variable_name,
+                        ),
+                    )
+
+            # 7.1 Recommendations 2/2
+            # Boundary variables should not have the _FillValue, missing_value, units, standard_name, axis,
+            # positive, calendar, leap_month, leap_year or month_lengths attributes.
+            attributes_to_check = {
+                "_FillValue",
+                "missing_value",
+                "units",
+                "standard_name",
+                "axis",
+                "positive",
+                "calendar",
+                "leap_month",
+                "leap_year",
+                "month_lengths",
+            }
+            if boundary_variable.__dict__.keys():
+                lst1 = boundary_variable.__dict__.keys()
+                lst2 = attributes_to_check
+                unwanted_attributes = [value for value in lst1 if value in lst2]
+                if unwanted_attributes:
+                    valid = False
+                    reasoning.append(
+                        "The Boundary variables '{}' should not have the attributes: '{}'".format(
+                            boundary_variable_name,
+                            unwanted_attributes,
+                        ),
                     )
 
             result = Result(
-                BaseCheck.MEDIUM, valid, self.section_titles["7.1"], reasoning
+                BaseCheck.MEDIUM,
+                valid,
+                self.section_titles["7.1"],
+                reasoning,
             )
             ret_val.append(result)
         return ret_val
 
+    def check_cell_boundaries_interval(self, ds):
+        """
+        7.1 Cell Boundaries
+        Recommendations: (1/2)
+        The points specified by a coordinate or auxiliary coordinate variable
+        should lie within, or on the boundary, of the cells specified by the
+        associated boundary variable.
+        """
+        ret_val = []
+        reasoning = []
+        for variable_name, boundary_variable_name in cfutil.get_cell_boundary_map(
+            ds,
+        ).items():
+            valid = True
+
+            variable = ds.variables[variable_name]
+            boundary_variable = ds.variables[boundary_variable_name]
+
+            for ii in range(len(variable[:])):
+                if abs(boundary_variable[ii][1]) >= abs(boundary_variable[ii][0]):
+                    if not (
+                        (abs(variable[ii]) >= abs(boundary_variable[ii][0]))
+                        and (abs(variable[ii]) <= abs(boundary_variable[ii][1]))
+                    ):
+                        valid = False
+                        reasoning.append(
+                            "The points specified by the coordinate variable {} ({})"
+                            " lie outside the boundary of the cell specified by the "
+                            "associated boundary variable {} ({})".format(
+                                variable_name,
+                                variable[ii],
+                                boundary_variable_name,
+                                boundary_variable[ii],
+                            ),
+                        )
+
+                result = Result(
+                    BaseCheck.MEDIUM,
+                    valid,
+                    self.section_titles["7.1"],
+                    reasoning,
+                )
+                ret_val.append(result)
+                print(ret_val)
+            return ret_val
+
     def check_cell_measures(self, ds):
         """
         A method to over-ride the CF1_6Check method. In CF 1.7, it is specified
         that variable referenced by cell_measures must be in the dataset OR
         referenced by the global attribute "external_variables", which represent
         all the variables used in the dataset but not found in the dataset.
 
@@ -341,82 +464,34 @@
         such as a standard_name.
 
         :param netCDF4.Dataset ds: An open netCDF dataset
         :rtype: list
         :return: List of results
         """
         ret_val = []
-        reasoning = []
         variables = ds.get_variables_by_attributes(
-            cell_measures=lambda c: c is not None
+            cell_measures=lambda c: c is not None,
         )
-        for var in variables:
-            search_str = r"^(?:area|volume): (\w+)$"
-            search_res = regex.search(search_str, var.cell_measures)
-            if not search_res:
-                valid = False
-                reasoning.append(
-                    "The cell_measures attribute for variable {} "
-                    "is formatted incorrectly.  It should take the"
-                    " form of either 'area: cell_var' or "
-                    "'volume: cell_var' where cell_var is the "
-                    "variable describing the cell measures".format(var.name)
-                )
+        try:
+            external_variables_str = ds.getncattr("external_variables")
+            if external_variables_str is not None:
+                external_variables_names = set(external_variables_str.split(" "))
             else:
-                valid = True
-                cell_meas_var_name = search_res.groups()[0]
-                # TODO: cache previous results
-
-                # if the dataset has external_variables, get it
-                try:
-                    external_variables = ds.getncattr("external_variables")
-                except AttributeError:
-                    external_variables = []
-                if cell_meas_var_name not in ds.variables:
-                    if cell_meas_var_name not in external_variables:
-                        valid = False
-                        reasoning.append(
-                            "Cell measure variable {} referred to by {} is not present in dataset variables".format(
-                                cell_meas_var_name, var.name
-                            )
-                        )
-                    else:
-                        valid = True
-
-                    # make Result
-                    result = Result(
-                        BaseCheck.MEDIUM, valid, (self.section_titles["7.2"]), reasoning
-                    )
-                    ret_val.append(result)
-                    continue  # can't test anything on an external var
-
-                else:
-                    cell_meas_var = ds.variables[cell_meas_var_name]
-                    if not hasattr(cell_meas_var, "units"):
-                        valid = False
-                        reasoning.append(
-                            "Cell measure variable {} is required "
-                            "to have units attribute defined.".format(
-                                cell_meas_var_name
-                            )
-                        )
-                    if not set(cell_meas_var.dimensions).issubset(var.dimensions):
-                        valid = False
-                        reasoning.append(
-                            "Cell measure variable {} must have "
-                            "dimensions which are a subset of "
-                            "those defined in variable {}.".format(
-                                cell_meas_var_name, var.name
-                            )
-                        )
-
-            result = Result(
-                BaseCheck.MEDIUM, valid, (self.section_titles["7.2"]), reasoning
+                external_variables_names = set()
+        except (ValueError, AttributeError):
+            external_variables_names = set()
+        for var in variables:
+            ret_val.append(
+                self._cell_measures_core(
+                    ds,
+                    var,
+                    external_variables_names,
+                    "dataset or external variable",
+                ),
             )
-            ret_val.append(result)
 
         return ret_val
 
     def _check_grid_mapping_attr_condition(self, attr, attr_name):
         """
         Evaluate a condition (or series of conditions) for a particular
         attribute. Implementation for CF-1.7.
@@ -448,16 +523,17 @@
         elif attr_name == "reference_ellipsoid_name":
             return self._evaluate_reference_ellipsoid_name(attr)
 
         elif attr_name == "towgs84":
             return self._evaluate_towgs84(attr)
 
         else:  # invoke method from 1.6, as these names are all still valid
-            return super(CF1_7Check, self)._check_grid_mapping_attr_condition(
-                attr, attr_name
+            return super()._check_grid_mapping_attr_condition(
+                attr,
+                attr_name,
             )
 
     def _check_gmattr_existence_condition_geoid_name_geoptl_datum_name(self, var):
         """
         Check to see if both geoid_name and geopotential_datum_name exist as attributes
         for `var`. They should not.
 
@@ -491,30 +567,26 @@
             "If any of reference_ellipsoid_name, prime_meridian_name, "
             "or horizontal_datum_name are defined, all must be defined."
         )
 
         _ncattrs = set(var.ncattrs())
 
         if any(
-            [
-                x in _ncattrs
-                for x in [
-                    "reference_ellipsoid_name",
-                    "prime_meridian_name",
-                    "horizontal_datum_name",
-                ]
+            x in _ncattrs
+            for x in [
+                "reference_ellipsoid_name",
+                "prime_meridian_name",
+                "horizontal_datum_name",
             ]
         ) and (
-            not set(
-                [
-                    "reference_ellipsoid_name",
-                    "prime_meridian_name",
-                    "horizontal_datum_name",
-                ]
-            ).issubset(_ncattrs)
+            not {
+                "reference_ellipsoid_name",
+                "prime_meridian_name",
+                "horizontal_datum_name",
+            }.issubset(_ncattrs)
         ):
             return (False, msg)
 
         else:
             return (True, msg)
 
     def _get_projdb_conn(self):
@@ -711,28 +783,31 @@
         elif val.dtype != np.float64:
             return (False, msg)
 
         # must be of length 3, 6, or 7
         elif not val.shape:  # single value
             return (False, msg)
 
-        elif not (val.size in (3, 6, 7)):
+        elif val.size not in (3, 6, 7):
             return (False, msg)
 
         else:
             return (True, msg)
 
     def check_grid_mapping(self, ds):
-        super(CF1_7Check, self).check_grid_mapping.__doc__
-        prev_return = super(CF1_7Check, self).check_grid_mapping(ds)
+        # FIXME: Looks like this is not needed.
+        # super().check_grid_mapping.__doc__
+        prev_return = super().check_grid_mapping(ds)
         grid_mapping_variables = cfutil.get_grid_mapping_variables(ds)
         for var_name in sorted(grid_mapping_variables):
             var = ds.variables[var_name]
             test_ctx = self.get_test_ctx(
-                BaseCheck.HIGH, self.section_titles["5.6"], var.name
+                BaseCheck.HIGH,
+                self.section_titles["5.6"],
+                var.name,
             )
 
             # TODO: check cases where crs_wkt provides part of a necessary
             #       grid_mapping attribute, or where a grid_mapping attribute
             #       overrides what has been provided in crs_wkt.
             # attempt to parse crs_wkt if it is present
             if "crs_wkt" in var.ncattrs():
@@ -742,16 +817,16 @@
                     test_ctx.out_of += 1
                 else:
                     try:
                         pyproj.CRS.from_wkt(crs_wkt)
                     except pyproj.exceptions.CRSError as crs_error:
                         test_ctx.messages.append(
                             "Cannot parse crs_wkt attribute to CRS using Proj4. Proj4 error: {}".format(
-                                str(crs_error)
-                            )
+                                str(crs_error),
+                            ),
                         )
                     else:
                         test_ctx.score += 1
                     test_ctx.out_of += 1
 
             # existence_conditions
             exist_cond_1 = (
@@ -769,96 +844,114 @@
             # check that geoid_name and geopotential_datum_name are not both
             # present in the grid_mapping variable
             if len_vdatum_name_attrs == 2:
                 test_ctx.out_of += 1
                 test_ctx.messages.append(
                     "Cannot have both 'geoid_name' and "
                     "'geopotential_datum_name' attributes in "
-                    "grid mapping variable '{}'".format(var.name)
+                    "grid mapping variable '{}'".format(var.name),
                 )
             elif len_vdatum_name_attrs == 1:
                 # should be one or zero attrs
                 proj_db_path = os.path.join(pyproj.datadir.get_data_dir(), "proj.db")
                 try:
                     with sqlite3.connect(proj_db_path) as conn:
                         v_datum_attr = next(iter(vert_datum_attrs))
                         v_datum_value = getattr(var, v_datum_attr)
                         v_datum_str_valid = self._process_v_datum_str(
-                            v_datum_value, conn
+                            v_datum_value,
+                            conn,
                         )
 
                         invalid_msg = (
                             "Vertical datum value '{}' for "
                             "attribute '{}' in grid mapping "
                             "variable '{}' is not valid".format(
-                                v_datum_value, v_datum_attr, var.name
+                                v_datum_value,
+                                v_datum_attr,
+                                var.name,
                             )
                         )
                         test_ctx.assert_true(v_datum_str_valid, invalid_msg)
                 except sqlite3.Error as e:
                     # if we hit an error, skip the check
                     warn(
                         "Error occurred while trying to query "
-                        "Proj4 SQLite database at {}: {}".format(proj_db_path, str(e))
+                        "Proj4 SQLite database at {}: {}".format(proj_db_path, str(e)),
+                        stacklevel=2,
                     )
             prev_return[var.name] = test_ctx.to_result()
 
         return prev_return
 
     def check_standard_name_deprecated_modifiers(self, ds):
         """
         Not a standard check in that it won't raise pass/fail values,
         but instead warns upon finding deprecated CF standard name modifiers.
         :param netCDF4.Dataset ds: netCDF dataset
         """
         deprecated_var_names = cfutil._find_standard_name_modifier_variables(ds, True)
         if deprecated_var_names:
             warn(
-                f"Deprecated standard_name modifiers found on variables {deprecated_var_names}"
+                f"Deprecated standard_name modifiers found on variables {deprecated_var_names}",
+                stacklevel=2,
             )
 
     def _process_v_datum_str(self, v_datum_str, conn):
         vdatum_query = """SELECT 1 FROM alias_name WHERE
                             table_name = 'vertical_datum' AND
                             alt_name = ?
                                 UNION ALL
                             SELECT 1 FROM vertical_datum WHERE
                             name = ?
                             LIMIT 1"""
         res_set = conn.execute(vdatum_query, (v_datum_str, v_datum_str))
         return len(res_set.fetchall()) > 0
 
     def _check_dimensionless_vertical_coordinate_1_7(
-        self, ds, vname, deprecated_units, ret_val, dim_vert_coords_dict
+        self,
+        ds,
+        vname,
+        deprecated_units,
+        ret_val,
+        dim_vert_coords_dict,
     ):
         """
         Check that a dimensionless vertical coordinate variable is valid under
         CF-1.7.
 
         :param netCDF4.Dataset ds: open netCDF4 dataset
         :param str name: variable name
         :param list ret_val: array to append Results to
         :rtype None
         """
         variable = ds.variables[vname]
         standard_name = getattr(variable, "standard_name", None)
         formula_terms = getattr(variable, "formula_terms", None)
         # Skip the variable if it's dimensional
+        correct_computed_std_name_ctx = TestCtx(
+            BaseCheck.MEDIUM,
+            self.section_titles["4.3"],
+        )
+        # IMPLEMENTATION CONFORMANCE 4.3.3 REQUIRED
+        correct_computed_std_name_ctx.assert_true(
+            not (formula_terms is None and hasattr(variable, "computed_standard_name")),
+            f"Variable {vname} should have formula_terms attribute when "
+            "computed_standard_name attribute is defined",
+        )
         if formula_terms is None and standard_name not in dim_vert_coords_dict:
             return
 
         # assert that the computed_standard_name is maps to the standard_name correctly
-        correct_computed_std_name_ctx = TestCtx(
-            BaseCheck.MEDIUM, self.section_titles["4.3"]
-        )
         _comp_std_name = dim_vert_coords_dict[standard_name][1]
         correct_computed_std_name_ctx.assert_true(
             getattr(variable, "computed_standard_name", None) in _comp_std_name,
             "§4.3.3 The standard_name of `{}` must map to the correct computed_standard_name, `{}`".format(
-                vname, sorted(_comp_std_name)
+                vname,
+                sorted(_comp_std_name),
             ),
         )
         ret_val.append(correct_computed_std_name_ctx.to_result())
 
     def check_dimensionless_vertical_coordinates(self, ds):
         """
         Check the validity of dimensionless coordinates under CF
@@ -889,20 +982,20 @@
         # and then extend it using a CF-1.7 addition
         ret_val.extend(
             self._check_dimensionless_vertical_coordinates(
                 ds,
                 deprecated_units,
                 self._check_dimensionless_vertical_coordinate_1_6,
                 dimless_vertical_coordinates_1_7,
-            )
+            ),
         )
 
         ret_val.extend(
             self._check_dimensionless_vertical_coordinates(
                 ds,
                 deprecated_units,
                 self._check_dimensionless_vertical_coordinate_1_7,
                 dimless_vertical_coordinates_1_7,
-            )
+            ),
         )
 
         return ret_val
```

### Comparing `compliance-checker-5.0.2/compliance_checker/cf/cf_1_8.py` & `compliance-checker-5.1.0/compliance_checker/cf/cf_1_8.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,21 +33,21 @@
     _cc_spec_version = "1.8"
     _cc_url = "http://cfconventions.org/Data/cf-conventions/cf-conventions-1.8/cf-conventions.html"
 
     ROOT_GROUP_ONLY_ATTRS = ["Conventions", "external_variables"]
     NON_ROOT_GROUP_OPT = ["title", "history"]
 
     def __init__(self, options=None):
-        super(CF1_8Check, self).__init__(options)
+        super().__init__(options)
         self.section_titles.update(
             {
                 "2.7": "§2.7 Groups",
                 "6.1.2": "§6.1.2 Taxon Names and Identifiers",
                 "7.5": "§7.5 Geometries",
-            }
+            },
         )
 
     def check_groups(self, ds: MemoizedDataset):
         """
         2.7.2. Application of attributes
 
         The following attributes are optional for non-root groups. They are allowed in order to
@@ -81,81 +81,78 @@
         """
 
         results = []
 
         ctx_hi = TestCtx(BaseCheck.HIGH, self.section_titles["2.7"])
         ctx_lo = TestCtx(BaseCheck.LOW, self.section_titles["2.7"])
 
+        # IMPLEMENTATION CONFORMANCE 2.7 REQUIRED 1/4
         # Make sure `Conventions` & `external_variables` attributes are only present in the
         # root group.
         for gname in ds.groups:
-            ginstance = ds.createGroup(
-                gname
-            )  # returns existing Group; doesn't create a new one
+            ginstance = ds.groups[gname]
 
             for attr in ginstance.ncattrs():
                 if attr in CF1_8Check.ROOT_GROUP_ONLY_ATTRS:
-
                     ctx_hi.messages.append(
                         f'§2.7.2 Attribute "{ attr }" MAY ONLY be used in the root group '
-                        "and SHALL NOT be duplicated or overridden in child groups."
+                        "and SHALL NOT be duplicated or overridden in child groups.",
                     )
 
                     results.append(ctx_hi.to_result())
 
                 elif attr in CF1_8Check.NON_ROOT_GROUP_OPT:
-
                     ctx_lo.messages.append(
                         f"§2.7.2 Note: attribute '{ attr }' found on non-root group '{ gname }'. "
                         "This is optional for non-root groups. It is allowed in order to provide additional "
                         "provenance and description of the subsidiary data. It does not override "
-                        "attributes from parent groups."
+                        "attributes from parent groups.",
                     )
                     results.append(ctx_lo.to_result())
 
         return results
 
     def check_geometry(self, ds: Dataset):
         """Runs any necessary checks for geometry well-formedness
         :param netCDF4.Dataset ds: An open netCDF dataset
         :returns list: List of error messages
         """
         vars_with_geometry = ds.get_variables_by_attributes(
-            geometry=lambda g: g is not None
+            geometry=lambda g: g is not None,
         )
         results = []
         unique_geometry_var_names = {var.geometry for var in vars_with_geometry}
         if unique_geometry_var_names:
             geom_valid = TestCtx(BaseCheck.MEDIUM, self.section_titles["7.5"])
             geom_valid.out_of += 1
         for geometry_var_name in unique_geometry_var_names:
             if geometry_var_name not in ds.variables:
                 geom_valid.messages.append(
-                    "Cannot find geometry variable " f"named {geometry_var_name}"
+                    "Cannot find geometry variable " f"named {geometry_var_name}",
                 )
                 results.append(geom_valid.to_result())
                 continue
             else:
                 geometry_var = ds.variables[geometry_var_name]
 
-            geometry_type = getattr(geometry_var, "geometry_type")
+            geometry_type = geometry_var.geometry_type
             try:
                 node_coord_var_names = geometry_var.node_coordinates
             except AttributeError:
                 geom_valid.messages.append(
                     "Could not find required attribute "
                     '"node_coordinates" in geometry '
-                    f'variable "{geometry_var_name}"'
+                    f'variable "{geometry_var_name}"',
                 )
                 results.append(geom_valid.to_result())
             if not isinstance(node_coord_var_names, str):
                 geom_valid.messages.append(
                     'Attribute "node_coordinates" in geometry '
                     f'variable "{geometry_var_name}" must be '
-                    "a string"
+                    "a string",
                 )
                 results.append(geom_valid.to_result())
                 continue
             split_coord_names = node_coord_var_names.strip().split(" ")
             node_coord_vars, not_found_node_vars = [], []
             for coord_var_name in split_coord_names:
                 try:
@@ -164,45 +161,51 @@
                     not_found_node_vars.append(coord_var_name)
             # If any variables weren't found, we can't continue
             if not_found_node_vars:
                 geom_valid.messages.append(
                     "The following referenced node coordinate"
                     "variables for geometry variable"
                     f'"{geometry_var_name}" were not found: '
-                    f"{not_found_node_vars}"
+                    f"{not_found_node_vars}",
                 )
                 results.append(geom_valid.to_result())
                 continue
 
             node_count = reference_attr_variables(
-                ds, getattr(geometry_var, "node_count", None)
+                ds,
+                getattr(geometry_var, "node_count", None),
             )
             # multipart lines and polygons only
             part_node_count = reference_attr_variables(
-                ds, getattr(geometry_var, "part_node_count", None)
+                ds,
+                getattr(geometry_var, "part_node_count", None),
             )
             # polygons with interior geometry only
             interior_ring = reference_attr_variables(
-                ds, getattr(geometry_var, "interior_ring", None)
+                ds,
+                getattr(geometry_var, "interior_ring", None),
             )
 
             if geometry_type == "point":
                 geometry = PointGeometry(node_coord_vars, node_count)
             elif geometry_type == "line":
                 geometry = LineGeometry(node_coord_vars, node_count, part_node_count)
             elif geometry_type == "polygon":
                 geometry = PolygonGeometry(
-                    node_coord_vars, node_count, part_node_count, interior_ring
+                    node_coord_vars,
+                    node_count,
+                    part_node_count,
+                    interior_ring,
                 )
             else:
                 geom_valid.messages.append(
                     f'For geometry variable "{geometry_var_name}'
                     'the attribute "geometry_type" must exist'
                     "and have one of the following values:"
-                    '"point", "line", "polygon"'
+                    '"point", "line", "polygon"',
                 )
                 results.append(geom_valid.to_result())
                 continue
             # check geometry
             messages = geometry.check_geometry()
             if not messages:
                 geom_valid.score += 1
@@ -253,43 +256,44 @@
                 and "taxon" in standard_name_string
                 and standard_name_string  # exclude the identifiers we just looked at
                 not in {"biological_taxon_lsid", "biological_taxon_name"}
                 and standard_name_string in self._std_names
             )
 
         taxa_quantifier_variables = ds.get_variables_by_attributes(
-            standard_name=match_taxa_standard_names
+            standard_name=match_taxa_standard_names,
         )
         # If there are no matches, there either are no taxa variables
         # or the standard names are not appropriate, which will be picked up
         # by the standard_name check
         if not taxa_quantifier_variables:
             return
 
         for taxon_quantifier_variable in taxa_quantifier_variables:
             valid_taxa = TestCtx(BaseCheck.HIGH, self.section_titles["6.1.2"])
             if not isinstance(
-                getattr(taxon_quantifier_variable, "coordinates", None), str
+                getattr(taxon_quantifier_variable, "coordinates", None),
+                str,
             ):
                 valid_taxa.add_failure(
-                    f'{taxon_quantifier_variable.name} must have a string valued "coordinates" attribute'
+                    f'{taxon_quantifier_variable.name} must have a string valued "coordinates" attribute',
                 )
                 continue
 
             coordinate_var_names = taxon_quantifier_variable.coordinates.split(" ")
             invalid_coord_vars = set(coordinate_var_names) - ds.variables.keys()
             if invalid_coord_vars:
                 valid_taxa.add_failure(
                     'The following values for "coordinates" attributes were not found in the dataset\'s variables '
-                    f"{invalid_coord_vars}"
+                    f"{invalid_coord_vars}",
                 )
 
             if len(coordinate_var_names) > 2:
                 valid_taxa.add_failure(
-                    "coordinates attribute for taxon data must either reference one or two variable names"
+                    "coordinates attribute for taxon data must either reference one or two variable names",
                 )
                 continue
 
             coordinate_vars = [
                 ds.variables[var_name] for var_name in coordinate_var_names
             ]
 
@@ -314,15 +318,15 @@
                 if lsid_messages:
                     valid_taxa.messages.extend(lsid_messages)
                 else:
                     valid_taxa.score += 1
             else:
                 valid_taxa.add_failure(
                     f"coordinates attribute for variable {taxon_quantifier_variable} must consist of "
-                    'variables containing standard names of either just "biological_taxon_name", or "biological_taxon_name" and "biological_taxon_identifier"'
+                    'variables containing standard names of either just "biological_taxon_name", or "biological_taxon_name" and "biological_taxon_identifier"',
                 )
             ret_val.append(valid_taxa.to_result())
 
         return ret_val
 
     def handle_lsid(self, taxon_lsid_variable, taxon_name_variable):
         """
@@ -334,15 +338,16 @@
         messages = []
         match_str = (
             r"(?:http://(?:www\.)?lsid.info/)?urn:lsid:"
             r"(?P<authority>[^:]+):(?P<namespace>[^:]+):"
             r"(?P<object_id>\w+)(?::(?P<version>\w+))?"
         )
         for taxon_lsid, taxon_name in zip(
-            taxon_lsid_variable[:], taxon_name_variable[:]
+            taxon_lsid_variable[:],
+            taxon_name_variable[:],
         ):
             # TODO: handle case where LSID is not present.  This can happen
             #       if the species is not present in the database desired.
             taxon_name_str = string_from_var_type(taxon_name)
             lsid_str = string_from_var_type(taxon_lsid)
             # if nodata/empty string for LSID, skip validity check
             if lsid_str == "":
@@ -356,15 +361,15 @@
                     "- www.lsid.info/urn:lsid.info:<authority>:<namespace>/<object_id>\n"
                     "- www.lsid.info/urn:lsid.info:<authority>:<namespace>/<object_id>:<version>\n"
                     "- lsid.info/urn:lsid.info:<authority>:<namespace>/<object_id>\n"
                     "- lsid.info/urn:lsid.info:<authority>:<namespace>/<object_id>:<version>\n"
                     "- http://lsid.info/urn:lsid.info:<authority>:<namespace>/<object_id>\n"
                     "- http://lsid.info/urn:lsid.info:<authority>:<namespace>/<object_id>:<version>\n"
                     "- http://www.lsid.info/urn:lsid.info:<authority>:<namespace>/<object_id>\n"
-                    "- http://www.lsid.info/urn:lsid.info:<authority>:<namespace>/<object_id>:<version>"
+                    "- http://www.lsid.info/urn:lsid.info:<authority>:<namespace>/<object_id>:<version>",
                 )
                 continue
             if lsid_str.startswith("urn"):
                 lsid_url = f"http://www.lsid.info/{lsid_str}"
             else:
                 lsid_url = lsid_str
 
@@ -376,20 +381,20 @@
                 # end
                 if response.status_code == 400:
                     tree = etree.HTML(response.text)
                     problem_text = tree.find("./body/p").text
                     messages.append(
                         "http://lsid.info returned an error message "
                         f"for submitted LSID string '{lsid_str}': "
-                        f"{problem_text}"
+                        f"{problem_text}",
                     )
                 else:
                     messages.append(
                         "Error occurred attempting to check LSID "
-                        f"'{lsid_str}': {str(e)}"
+                        f"'{lsid_str}': {str(e)}",
                     )
                 continue
 
             # WoRMS -- marine bio data
             if (
                 taxon_match["authority"] == "marinespecies.org"
                 and taxon_match["namespace"] == "taxname"
@@ -399,37 +404,37 @@
                         f"http://www.marinespecies.org/rest/AphiaRecordByAphiaID/{taxon_match['object_id']}",
                         timeout=15,
                     )
                     response.raise_for_status()
                 except requests.exceptions.RequestException as e:  # noqa: F841
                     messages.append(
                         "Aphia ID {taxon_match['object_id'] returned "
-                        "other error: {str(e)}"
+                        "other error: {str(e)}",
                     )
                 # record not found in database
                 if response.status_code == 204:
                     messages.append(
                         "Aphia ID {taxon_match['object_id'] "
-                        "not found in WoRMS database"
+                        "not found in WoRMS database",
                     )
                 # good case, parse JSON
                 elif response.status_code == 200:
                     valid_name = response.json()["valid_name"]
                     if valid_name != taxon_name_str:
                         messages.append(
                             "Supplied taxon name and WoRMS valid name do not match. "
                             f"Supplied taxon name is '{taxon_name_str}', WoRMS valid name "
-                            f"is '{valid_name}.'"
+                            f"is '{valid_name}.'",
                         )
                 # Misc non-error code.  Should not reach here.
                 else:
                     messages.append(
                         f"Aphia ID {taxon_match['object_id']}"
                         "returned an unhandled HTTP status "
-                        f"code {response.status_code}"
+                        f"code {response.status_code}",
                     )
                     continue
 
             # ITIS -- freshwater bio data
             elif (
                 taxon_match["authority"] == "itis.gov"
                 and taxon_match["namespace"] == "itis_tsn"
@@ -437,64 +442,65 @@
                 itis_url = f"https://www.itis.gov/ITISWebService/jsonservice/getFullRecordFromTSN?tsn={taxon_match['object_id']}"
                 try:
                     itis_response = requests.get(itis_url, timeout=15)
                     itis_response.raise_for_status()
                 except requests.exceptions.RequestException as e:
                     if itis_response.status_code == 404:
                         messages.append(
-                            "itis.gov TSN " f"{taxon_match['object_id']} not found."
+                            "itis.gov TSN " f"{taxon_match['object_id']} not found.",
                         )
                         continue
                     else:
                         messages.append(
-                            "itis.gov identifier returned other " f"error: {str(e)}"
+                            "itis.gov identifier returned other " f"error: {str(e)}",
                         )
                         continue
                 json_contents = itis_response.json()
                 combined_name = json_contents["scientificName"]["combinedName"]
 
                 if taxon_name_str != combined_name:
                     messages.append(
                         "Supplied taxon name and ITIS scientific name do not match. "
                         f"Supplied taxon name is '{taxon_name_str}', ITIS scientific name "
-                        f"for TSN {taxon_match['object_id']} is '{combined_name}.'"
+                        f"for TSN {taxon_match['object_id']} is '{combined_name}.'",
                     )
 
             else:
                 warnings.warn(
                     "Compliance checker only supports checking valid "
                     "LSID URNs of the form "
                     "'urn:lsid:marinespecies.org:taxname:<AphiaID>' or "
                     "'urn:lsid:itis.gov:itis_tsn:<TSN>'.  Assuming "
-                    "pass condition"
+                    "pass condition",
+                    stacklevel=1,
                 )
 
         return messages
 
 
-class GeometryStorage(object):
+class GeometryStorage:
     """Abstract base class for geometries"""
 
     def __init__(self, coord_vars, node_count):
         self.coord_vars = coord_vars
         self.node_count = node_count
         self.errors = []
         # geometry is later parsed after sanity checks are run
         self.geometry = None
 
     def check_geometry(self):
         invalid_vars = []
         for coord_var in self.coord_vars:
-            if not np.issubdtype(coord_var, np.float):
+            if not np.issubdtype(coord_var, float):
                 invalid_vars.append(coord_var.name)
         # can't continue if the geometry variables are not the correct size
         if invalid_vars:
             self.errors.append(
                 "The following geometry variables "
-                f"have non-numeric contents: {invalid_vars}"
+                f"have non-numeric contents: {invalid_vars}",
             )
 
     def _split_mulitpart_geometry(self):
         arr_extents_filt = self.part_node_count[self.part_node_count > 0]
         splits = np.split(np.vstack(self.coord_vars).T, arr_extents_filt.cumsum()[:-1])
         return splits
 
@@ -509,15 +515,15 @@
             same_dim_group = itertools.groupby(self.coord_vars, lambda x: x.dimensions)
             same_dim = next(same_dim_group, True) and not next(same_dim_group, False)
             if not same_dim:
                 self.errors.append(
                     "For a point geometry, coordinate "
                     "variables must be the same length as "
                     "node_count defined, or must be "
-                    "length 1 if node_count is not set"
+                    "length 1 if node_count is not set",
                 )
         return self.errors
 
 
 class LineGeometry(GeometryStorage):
     """Class for validating Line/MultiLine geometries"""
 
@@ -532,37 +538,37 @@
         same_dim_group = itertools.groupby(self.coord_vars, lambda x: x.dimensions)
         same_dim = next(same_dim_group, True) and not next(same_dim_group, False)
         if not same_dim:
             raise IndexError(
                 "Coordinate variables must be the same length. "
                 "If node_count is specified, this value must "
                 "also sum to the length of the coordinate "
-                "variables."
+                "variables.",
             )
         # if a multipart
         if self.node_count is not None:
             same_length = len(self.coord_vars[0]) == self.node_count[:].sum()
             if not same_length:
                 geom_errors.append(
                     "Coordinate variables must be the same "
                     "length. If node_count is specified, this "
                     "value must also sum to the length of the "
-                    "coordinate variables."
+                    "coordinate variables.",
                 )
         if self.part_node_count is not None:
             if not np.issubdtype(self.part_node_count.dtype, np.integer):
                 geom_errors.append(
                     "when part_node_count is specified, it must "
-                    "be an array of integers"
+                    "be an array of integers",
                 )
             same_node_count = len(self.coord_vars[0]) == self.node_count[:].sum()
             if not same_node_count:
                 geom_errors.append(
                     "The sum of part_node_count must be equal "
-                    "to the value of node_count"
+                    "to the value of node_count",
                 )
         return geom_errors
 
 
 class PolygonGeometry(LineGeometry):
     """Class for validating Line/MultiLine geometries"""
 
@@ -588,17 +594,17 @@
         :rtype bool:
         :returns: True if the polygon follows the proper orientation,
                   False if it fails the orientation test.
         """
 
         try:
             polygon = Polygon(transposed_coords.tolist())
-        except ValueError:
-            raise ValueError(
-                "Polygon contains too few points to perform orientation test"
+        except ValueError as err:
+            raise ValueError from err(
+                "Polygon contains too few points to perform orientation test",
             )
 
         ccw = polygon.exterior.is_ccw
         return not ccw if interior else ccw
 
     def check_geometry(self):
         messages = super().check_geometry()
@@ -621,15 +627,16 @@
         #       node_count in the polygon, i.e. first (3, 3, 3) will consume
         #       a node part of 9, follow by next 3 will consume a node part of
         #       3 after consuming
         for i in range(node_indexer_len):
             extent_slice = slice(extents[i], extents[i + 1])
             poly_sliced = np.vstack([cv[extent_slice] for cv in self.coord_vars]).T
             pass_orientation = self.check_polygon_orientation(
-                poly_sliced, ring_orientation[i]
+                poly_sliced,
+                ring_orientation[i],
             )
             if not pass_orientation:
                 orient_fix = (
                     ("exterior", "counterclockwise")
                     if not ring_orientation[i]
                     else ("interior", "clockwise")
                 )
```

### Comparing `compliance-checker-5.0.2/compliance_checker/cf/cf_base.py` & `compliance-checker-5.1.0/compliance_checker/cf/cf_base.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 #!/usr/bin/env python
-# -*- coding: utf-8 -*-
 import logging
 import os
 import sys
 from collections import OrderedDict, defaultdict
 from warnings import warn
 
 import numpy as np
@@ -25,15 +24,15 @@
     def __init__(self, options=None):
         # The compliance checker can be run on multiple datasets in a single
         # instantiation, so caching values has be done by the unique identifier
         # for each dataset loaded.
 
         # Each default dict is a key, value mapping from the dataset object to
         # a list of variables
-        super(CFBaseCheck, self).__init__(options)
+        super().__init__(options)
         self._coord_vars = defaultdict(list)
         self._ancillary_vars = defaultdict(list)
         self._clim_vars = defaultdict(list)
         self._metadata_vars = defaultdict(list)
         self._boundary_vars = defaultdict(list)
         self._geophysical_vars = defaultdict(list)
         self._aux_coords = defaultdict(list)
@@ -54,14 +53,15 @@
             "3.4": "§3.4 Ancillary Data",
             "3.5": "§3.5 Flags",
             "4": "§4 Coordinate Types",
             "4.1": "§4.1 Latitude Coordinate",
             "4.2": "§4.2 Longitude Coordinate",
             "4.3": "§4.3 Vertical Coordinate",
             "4.4": "§4.4 Time Coordinate",
+            "4.4.1": "§4.4.1 Calendar",
             "4.5": "§4.5 Discrete Axis",
             "5": "§5 Coordinate Systems",
             "5.1": "§5.1 Independent Latitude, Longitude, Vertical, and Time Axes",
             "5.2": "§5.2 2-D Latitude, Longitude, Coordinate Variables",
             "5.3": "§5.3 Reduced Horizontal Grid",
             "5.4": "§5.4 Timeseries of Station Data",
             "5.5": "§5.5 Trajectories",
@@ -99,15 +99,15 @@
         self._find_ancillary_vars(ds)
         self._find_clim_vars(ds)
         self._find_boundary_vars(ds)
         self._find_metadata_vars(ds)
         self._find_cf_standard_name_table(ds)
         self._find_geophysical_vars(ds)
         coord_containing_vars = ds.get_variables_by_attributes(
-            coordinates=lambda val: isinstance(val, str)
+            coordinates=lambda val: isinstance(val, str),
         )
 
         # coordinate data variables
 
         # Excerpt from "§1.3 Overview" on coordinate data
         # There are two methods used to identify variables that contain
         # coordinate data. The first is to use the NUG-defined "coordinate
@@ -171,77 +171,83 @@
         """
 
         ret_val = OrderedDict()
         grid_mapping_variables = cfutil.get_grid_mapping_variables(ds)
 
         # Check the grid_mapping attribute to be a non-empty string and that its reference exists
         for variable in ds.get_variables_by_attributes(
-            grid_mapping=lambda x: x is not None
+            grid_mapping=lambda x: x is not None,
         ):
             grid_mapping = getattr(variable, "grid_mapping", None)
             defines_grid_mapping = self.get_test_ctx(
-                BaseCheck.HIGH, self.section_titles["5.6"], variable.name
+                BaseCheck.HIGH,
+                self.section_titles["5.6"],
+                variable.name,
             )
             defines_grid_mapping.assert_true(
                 (isinstance(grid_mapping, str) and grid_mapping),
                 "{}'s grid_mapping attribute must be a "
                 "space-separated non-empty string".format(variable.name),
             )
             if isinstance(grid_mapping, str):
                 # TODO (badams): refactor functionality to split functionality
                 #                into requisite classes
                 if ":" in grid_mapping and self._cc_spec_version >= "1.7":
                     colon_count = grid_mapping.count(":")
                     re_all = regex.findall(
-                        r"(\w+):\s*((?:\w+\s+)*(?:\w+)(?![\w:]))", grid_mapping
+                        r"(\w+):\s*((?:\w+\s+)*(?:\w+)(?![\w:]))",
+                        grid_mapping,
                     )
                     if colon_count != len(re_all):
                         defines_grid_mapping.out_of += 1
                         defines_grid_mapping.messages.append(
-                            "Could not consume entire grid_mapping expression, please check for well-formedness"
+                            "Could not consume entire grid_mapping expression, please check for well-formedness",
                         )
                     else:
                         for grid_var_name, coord_var_str in re_all:
                             defines_grid_mapping.assert_true(
                                 grid_var_name in ds.variables,
                                 "grid mapping variable {} must exist in this dataset".format(
-                                    grid_var_name
+                                    grid_var_name,
                                 ),
                             )
                             for ref_var in coord_var_str.split():
                                 defines_grid_mapping.assert_true(
                                     ref_var in ds.variables,
                                     "Coordinate-related variable {} referenced by grid_mapping variable {} must exist in this dataset".format(
-                                        ref_var, grid_var_name
+                                        ref_var,
+                                        grid_var_name,
                                     ),
                                 )
 
                 else:
                     for grid_var_name in grid_mapping.split():
                         defines_grid_mapping.assert_true(
                             grid_var_name in ds.variables,
                             "grid mapping variable {} must exist in this dataset".format(
-                                grid_var_name
+                                grid_var_name,
                             ),
                         )
             ret_val[variable.name] = defines_grid_mapping.to_result()
 
         # Check the grid mapping variables themselves
         for grid_var_name in grid_mapping_variables:
             valid_grid_mapping = self.get_test_ctx(
-                BaseCheck.HIGH, self.section_titles["5.6"], grid_var_name
+                BaseCheck.HIGH,
+                self.section_titles["5.6"],
+                grid_var_name,
             )
             grid_var = ds.variables[grid_var_name]
 
             grid_mapping_name = getattr(grid_var, "grid_mapping_name", None)
 
             # Grid mapping name must be in appendix F
             valid_grid_mapping.assert_true(
                 grid_mapping_name in self.grid_mapping_dict,
-                "{} is not a valid grid_mapping_name.".format(grid_mapping_name)
+                f"{grid_mapping_name} is not a valid grid_mapping_name."
                 + " See Appendix F for valid grid mappings",
             )
 
             # The self.grid_mapping_dict has a values of:
             # - required attributes
             # - optional attributes (can't check)
             # - required standard_names defined
@@ -255,43 +261,44 @@
             grid_mapping = self.grid_mapping_dict[grid_mapping_name]
             required_attrs = grid_mapping[0]
             # Make sure all the required attributes are defined
             for req in required_attrs:
                 valid_grid_mapping.assert_true(
                     hasattr(grid_var, req),
                     "{} is a required attribute for grid mapping {}".format(
-                        req, grid_mapping_name
+                        req,
+                        grid_mapping_name,
                     ),
                 )
 
             # Make sure that exactly one of the exclusive attributes exist
             if len(grid_mapping) == 4:
                 at_least_attr = grid_mapping[3]
                 number_found = 0
                 for attr in at_least_attr:
                     if hasattr(grid_var, attr):
                         number_found += 1
                 valid_grid_mapping.assert_true(
                     number_found == 1,
-                    "grid mapping {}".format(grid_mapping_name)
+                    f"grid mapping {grid_mapping_name}"
                     + "must define exactly one of these attributes: "
                     + "{}".format(" or ".join(at_least_attr)),
                 )
 
             # Make sure that exactly one variable is defined for each of the required standard_names
             expected_std_names = grid_mapping[2]
             for expected_std_name in expected_std_names:
                 found_vars = ds.get_variables_by_attributes(
-                    standard_name=expected_std_name
+                    standard_name=expected_std_name,
                 )
                 valid_grid_mapping.assert_true(
                     len(found_vars) == 1,
-                    "grid mapping {} requires exactly ".format(grid_mapping_name)
+                    f"grid mapping {grid_mapping_name} requires exactly "
                     + "one variable with standard_name "
-                    + "{} to be defined".format(expected_std_name),
+                    + f"{expected_std_name} to be defined",
                 )
 
             ret_val[grid_var_name] = valid_grid_mapping.to_result()
 
         return ret_val
 
     def check_conventions_version(self, ds):
@@ -303,32 +310,36 @@
         :param netCDF4.Dataset ds: An open netCDF dataset
         :rtype: compliance_checker.base.Result
         """
 
         valid = False
         reasoning = []
         correct_version_string = "{}-{}".format(
-            self._cc_spec, self._cc_spec_version
+            self._cc_spec,
+            self._cc_spec_version,
         ).upper()
         if hasattr(ds, "Conventions"):
             conventions = regex.split(r",|\s+", getattr(ds, "Conventions", ""))
             for convention in conventions:
                 if convention == correct_version_string:
                     valid = True
                     break
             else:
                 reasoning = [
                     "§2.6.1 Conventions global attribute does not contain "
-                    '"{}"'.format(correct_version_string)
+                    '"{}"'.format(correct_version_string),
                 ]
         else:
             valid = False
             reasoning = ["§2.6.1 Conventions field is not present"]
         return Result(
-            BaseCheck.MEDIUM, valid, self.section_titles["2.6"], msgs=reasoning
+            BaseCheck.MEDIUM,
+            valid,
+            self.section_titles["2.6"],
+            msgs=reasoning,
         )
 
     def _check_dimensionless_vertical_coordinates(
         self,
         ds,
         deprecated_units,
         version_specific_check,
@@ -384,29 +395,38 @@
         if not formula_terms:
             return valid_formula_terms.to_result()
 
         # check that the formula_terms are well formed and are present
         # The pattern for formula terms is always component: variable_name
         # the regex grouping always has component names in even positions and
         # the corresponding variable name in odd positions.
-        matches = regex.findall(
-            r"([A-Za-z][A-Za-z0-9_]*: )([A-Za-z][A-Za-z0-9_]*)", variable.formula_terms
+        poorly_formed_formula_terms = ("Attribute formula_terms is not well-formed",)
+        matches = list(
+            regex.finditer(
+                r"(\w+):\s+(\w+)(?:\s+(?!$)|$)",
+                variable.formula_terms,
+            ),
         )
-        terms = set(m[0][:-2] for m in matches)
+        if not matches:
+            valid_formula_terms.add_failure(poorly_formed_formula_terms)
+            return valid_formula_terms.to_result()
+
+        terms = {m.group(1) for m in matches}
         # get the variables named in the formula terms and check if any
         # are not present in the dataset
-        missing_vars = sorted(set(m[1] for m in matches) - set(ds.variables))
+        missing_vars = sorted({m.group(2) for m in matches} - set(ds.variables))
         missing_fmt = "The following variable(s) referenced in {}:formula_terms are not present in the dataset: {}"
         valid_formula_terms.assert_true(
-            len(missing_vars) == 0, missing_fmt.format(coord, ", ".join(missing_vars))
+            len(missing_vars) == 0,
+            missing_fmt.format(coord, ", ".join(missing_vars)),
         )
         # try to reconstruct formula_terms by adding space in between the regex
         # matches.  If it doesn't exactly match the original, the formatting
         # of the attribute is incorrect
-        reconstructed_formula = " ".join(m[0] + m[1] for m in matches)
+        reconstructed_formula = "".join(m.group(0) for m in matches)
         valid_formula_terms.assert_true(
             reconstructed_formula == formula_terms,
             "Attribute formula_terms is not well-formed",
         )
 
         valid_formula_terms.assert_true(
             standard_name in dimless_coords_dict,
@@ -467,15 +487,18 @@
             val_type = attr_val.dtype.type
             type_match = val_type == var.dtype.type
 
         ctx.assert_true(
             type_match,
             "Attribute '{}' (type: {}) and parent variable '{}' (type: {}) "
             "must have equivalent datatypes".format(
-                attr_name, val_type, var.name, var.dtype.type
+                attr_name,
+                val_type,
+                var.name,
+                var.dtype.type,
             ),
         )
 
     def _find_aux_coord_vars(self, ds, refresh=False):
         """
         Returns a list of auxiliary coordinate variables
 
@@ -540,15 +563,15 @@
         # Used the cached version if it exists and is not empty
         if self._ancillary_vars.get(ds, None) and refresh is False:
             return self._ancillary_vars[ds]
 
         # Invalidate the cache at all costs
         self._ancillary_vars[ds] = []
 
-        for name, var in ds.variables.items():
+        for _name, var in ds.variables.items():
             if hasattr(var, "ancillary_variables"):
                 for anc_name in var.ancillary_variables.split(" "):
                     if anc_name in ds.variables:
                         self._ancillary_vars[ds].append(anc_name)
 
             if hasattr(var, "grid_mapping"):
                 gm_name = var.grid_mapping
@@ -610,69 +633,74 @@
                     return False
                 else:
                     try:
                         version = version[0]
                     except IndexError:
                         warn(
                             "Cannot extract CF standard name version number "
-                            "from standard_name_vocabulary string"
+                            "from standard_name_vocabulary string",
+                            stacklevel=2,
                         )
                         return False
             else:
                 # Can't parse the attribute, use the packaged version
                 return False
         # usually raised from .lower() with an incompatible (non-string)
         # data type
         except AttributeError:
             warn(
                 "Cannot convert standard name table to lowercase.  This can "
                 "occur if a non-string standard_name_vocabulary global "
-                "attribute is supplied"
+                "attribute is supplied",
+                stacklevel=2,
             )
             return False
 
         if version.startswith("v"):  # i.e 'v34' -> '34' drop the v
             version = version[1:]
 
         # If the packaged version is what we're after, then we're good
         if version == self._std_names._version:
             print(
-                "Using packaged standard name table v{0}".format(version),
+                f"Using packaged standard name table v{version}",
                 file=sys.stderr,
             )
             return False
 
         # Try to download the version specified
         try:
             data_directory = util.create_cached_data_dir()
             location = os.path.join(
-                data_directory, "cf-standard-name-table-test-{0}.xml".format(version)
+                data_directory,
+                f"cf-standard-name-table-test-{version}.xml",
             )
             # Did we already download this before?
             if not os.path.isfile(location):
                 util.download_cf_standard_name_table(version, location)
                 print(
-                    "Using downloaded standard name table v{0}".format(version),
+                    f"Using downloaded standard name table v{version}",
                     file=sys.stderr,
                 )
             else:
                 print(
-                    "Using cached standard name table v{0} from {1}".format(
-                        version, location
+                    "Using cached standard name table v{} from {}".format(
+                        version,
+                        location,
                     ),
                     file=sys.stderr,
                 )
 
             self._std_names = util.StandardNameTable(location)
             return True
         except Exception as e:
             # There was an error downloading the CF table. That's ok, we'll just use the packaged version
             warn(
-                "Problem fetching standard name table:\n{0}\n"
-                "Using packaged v{1}".format(e, self._std_names._version)
+                f"Problem fetching standard name table:\n{e}\n"
+                f"Using packaged v{self._std_names._version}",
+                stacklevel=2,
             )
             return False
 
     def _find_coord_vars(self, ds, refresh=False):
         """
         Returns a list of variable names that identify as coordinate variables.
 
@@ -725,17 +753,16 @@
 
         """
         if self._metadata_vars.get(ds, None) and refresh is False:
             return self._metadata_vars[ds]
 
         self._metadata_vars[ds] = []
         for name, var in ds.variables.items():
-
             if name in self._find_ancillary_vars(ds) or name in self._find_coord_vars(
-                ds
+                ds,
             ):
                 continue
 
             if name in (
                 "platform_name",
                 "station_name",
                 "instrument_name",
@@ -878,15 +905,15 @@
         :param netCDF4.Dataset ds: An open netCDF dataset
 
         :rtype: list
         :returns: A list of variable dimensions
         """
         ret_val = []
         for variable in ds.get_variables_by_attributes(
-            cf_role=lambda x: isinstance(x, str)
+            cf_role=lambda x: isinstance(x, str),
         ):
             if variable.ndim > 0:
                 ret_val.append(variable.dimensions[0])
         return ret_val
 
     def _get_pretty_dimension_order(self, ds, name):
         """
@@ -918,15 +945,15 @@
         :param list dim_types: A list of strings returned by
                                _get_dimension_order for the same "name"
         :rtype: str
         :return: A comma separated string of the variable's dimensions
         """
         dim_names = []
         for dim, dim_type in zip(ds.variables[name].dimensions, dim_types):
-            dim_name = "{} ({}".format(dim, dim_type)
+            dim_name = f"{dim} ({dim_type}"
             if ds.dimensions[dim].isunlimited():
                 dim_name += ", unlimited)"
             else:
                 dim_name += ")"
             dim_names.append(dim_name)
         return ", ".join(dim_names)
 
@@ -1000,15 +1027,16 @@
                                    "Use" column in CF Appendix A
             :rtype: str
             :return: A string with a human-readable name followed by the input
                      letter specified
             """
 
             return "{} ({})".format(
-                attr_location_ident.get(att_letter, "other"), att_letter
+                attr_location_ident.get(att_letter, "other"),
+                att_letter,
             )
 
         def _att_loc_msg(att_loc):
             """
             Helper method for formatting an error message when an attribute
             appears in the improper location corresponding to the "Use" column
             in CF Appendix A.
@@ -1025,45 +1053,47 @@
             # it generally should not occur
             valid_loc = "no locations in the dataset"
             loc_sort = sorted(att_loc)
             if att_loc_len == 1:
                 valid_loc = att_loc_print_helper(loc_sort[0])
             elif att_loc_len == 2:
                 valid_loc = "{} and {}".format(
-                    att_loc_print_helper(loc_sort[0]), att_loc_print_helper(loc_sort[1])
+                    att_loc_print_helper(loc_sort[0]),
+                    att_loc_print_helper(loc_sort[1]),
                 )
             # shouldn't be reached under normal circumstances, as any attribute
             # should be either G, C, or D but if another
             # category is added, this will be useful.
             else:
                 valid_loc = ", ".join(loc_sort[:-1]) + ", and {}".format(
-                    att_loc_print_helper(loc_sort[-1])
+                    att_loc_print_helper(loc_sort[-1]),
                 )
-            return "This attribute may only appear in {}.".format(valid_loc)
+            return f"This attribute may only appear in {valid_loc}."
 
         for global_att_name in possible_global_atts:
             global_att = ds.getncattr(global_att_name)
             att_dict = self.appendix_a[global_att_name]
             att_loc = att_dict["attr_loc"]
             valid_loc_warn = _att_loc_msg(att_loc)
             if att_dict["cf_section"] is not None:
                 subsection_test = ".".join(att_dict["cf_section"].split(".")[:2])
 
                 section_loc = self.section_titles.get(
-                    subsection_test, att_dict["cf_section"]
+                    subsection_test,
+                    att_dict["cf_section"],
                 )
             else:
                 section_loc = None
             test_ctx = TestCtx(BaseCheck.HIGH, section_loc)
 
             test_ctx.out_of += 1
             if "G" not in att_loc:
                 test_ctx.messages.append(
                     '[Appendix A] Attribute "{}" should not be present in global (G) '
-                    "attributes. {}".format(global_att_name, valid_loc_warn)
+                    "attributes. {}".format(global_att_name, valid_loc_warn),
                 )
             else:
                 result = self._handle_dtype_check(global_att, global_att_name, att_dict)
                 if not result[0]:
                     test_ctx.messages.append(result[1])
                 else:
                     test_ctx.score += 1
@@ -1077,19 +1107,20 @@
             for var_name in var_set:
                 var = ds.variables[var_name]
                 possible_attrs = set(var.ncattrs()).intersection(self.appendix_a.keys())
                 for att_name in possible_attrs:
                     att_dict = self.appendix_a[att_name]
                     if att_dict["cf_section"] is not None:
                         subsection_test = ".".join(
-                            att_dict["cf_section"].split(".")[:2]
+                            att_dict["cf_section"].split(".")[:2],
                         )
 
                         section_loc = self.section_titles.get(
-                            subsection_test, att_dict["cf_section"]
+                            subsection_test,
+                            att_dict["cf_section"],
                         )
                     else:
                         section_loc = None
                     test_ctx = TestCtx(BaseCheck.HIGH, section_loc, variable=var_name)
                     att_loc = att_dict["attr_loc"]
                     valid_loc_warn = _att_loc_msg(att_loc)
                     att = var.getncattr(att_name)
@@ -1098,15 +1129,15 @@
                         test_ctx.messages.append(
                             '[Appendix A] Attribute "{}" should not be present in {} '
                             'variable "{}". {}'.format(
                                 att_name,
                                 att_loc_print_helper(coord_letter),
                                 var_name,
                                 valid_loc_warn,
-                            )
+                            ),
                         )
                     else:
                         result = self._handle_dtype_check(att, att_name, att_dict, var)
                         if not result[0]:
                             test_ctx.messages.append(result[1])
                         else:
                             test_ctx.score += 1
@@ -1131,45 +1162,46 @@
         :rtype tuple
         :return A two-tuple that contains pass/fail status as a boolean and
                 a message string (or None if unset) as the second element.
         """
 
         if attr_type == "S":
             if not isinstance(attribute, str):
-                return [False, "{} must be a string".format(attr_name)]
+                return [False, f"{attr_name} must be a string"]
         else:
             # if it's not a string, it should have a numpy dtype
             underlying_dtype = getattr(attribute, "dtype", None)
 
             # TODO check for np.nan separately
             if underlying_dtype is None:
-                return [False, "{} must be a numeric type".format(attr_name)]
+                return [False, f"{attr_name} must be a numeric type"]
 
             # both D and N should be some kind of numeric value
             is_numeric = np.issubdtype(underlying_dtype, np.number)
             if attr_type == "N":
                 if not is_numeric:
-                    return [False, "{} must be a numeric type".format(attr_name)]
+                    return [False, f"{attr_name} must be a numeric type"]
             elif attr_type == "D":
                 # TODO: handle edge case where variable is unset here
                 temp_ctx = TestCtx()
                 self._parent_var_attr_type_check(attr_name, variable, temp_ctx)
                 var_dtype = getattr(variable, "dtype", None)
                 if temp_ctx.messages:
                     return (
                         False,
                         "{} must be numeric and must be equivalent to {} dtype".format(
-                            attr_name, var_dtype
+                            attr_name,
+                            var_dtype,
                         ),
                     )
             else:
                 # If we reached here, we fell off with an unrecognized type
                 return (
                     False,
-                    "{} has unrecognized type '{}'".format(attr_name, attr_type),
+                    f"{attr_name} has unrecognized type '{attr_type}'",
                 )
         # pass if all other possible failure conditions have been evaluated
         return (True, None)
 
     def _handle_dtype_check(self, attribute, attr_name, attr_dict, variable=None):
         """
         Helper function for Appendix A checks.
@@ -1182,20 +1214,20 @@
         :rtype: tuple
         :return: A two-tuple that contains pass/fail status as a boolean and
                  a message string (or None if unset) as the second element.
         """
         attr_type = attr_dict["Type"]
         if variable is None and "G" not in attr_dict["attr_loc"]:
             raise ValueError(
-                "Non-global attributes must be associated with a " " variable"
+                "Non-global attributes must be associated with a " " variable",
             )
         attr_str = (
-            "Global attribute {}".format(attr_name)
+            f"Global attribute {attr_name}"
             if "G" in attr_dict["attr_loc"] and variable is None
-            else "Attribute {} in variable {}".format(attr_name, variable.name)
+            else f"Attribute {attr_name} in variable {variable.name}"
         )
 
         # check the type
         return_value = self._check_attr_type(attr_name, attr_type, attribute, variable)
 
         # if the second element is a string, format it
         if isinstance(return_value[1], str):
```

### Comparing `compliance-checker-5.0.2/compliance_checker/cfutil.py` & `compliance-checker-5.1.0/compliance_checker/cfutil.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 #!/usr/bin/env python
-# -*- coding: utf-8 -*-
 """
 compliance_checker/cfutil.py
 """
 import csv
 import re
 import warnings
 from collections import defaultdict
@@ -64,37 +63,37 @@
 
     """
     if attr_val is None:
         return False
 
     if not isinstance(attr_val, attr_type):
         warnings.warn(
-            "Attribute is of type {}, {} expected. "
-            "Attempting to cast to expected type.".format(type(attr_val), attr_type)
+            f"Attribute is of type {type(attr_val)!r}, {attr_type!r} expected. Attempting to cast to expected type.",
+            stacklevel=2,
         )
         try:
             # if the expected type is str, try casting to unicode type
             # since str can't be instantiated
             if attr_type is str:
                 new_attr_val = str(attr_val)
             else:
                 new_attr_val = attr_type(attr_val)
         # catch casting errors
         except (ValueError, UnicodeEncodeError):
-            warnings.warn("Could not cast to type {}".format(attr_type))
+            warnings.warn(f"Could not cast to type {attr_type}", stacklevel=2)
             return False
     else:
         new_attr_val = attr_val
 
     try:
         is_in_set = modifier_fn(new_attr_val) in value_set
     except Exception as e:
         warnings.warn(
-            "Could not apply modifier function {} to value: "
-            " {}".format(modifier_fn, e.msg)
+            f"Could not apply modifier function {modifier_fn} to value: {e.msg}",
+            stacklevel=2,
         )
         return False
 
     return is_in_set
 
 
 @lru_cache(128)
@@ -105,35 +104,35 @@
     units and units that are defined as constant units in the CF standard name
     table i.e. '1', or '1e-3'.
     """
     # standard_name must be string, so if it is not, it is *wrong* by default
     if not isinstance(standard_name, str):
         return False
     found_standard_name = standard_name_table.find(
-        ".//entry[@id='{}']".format(standard_name)
+        f".//entry[@id='{standard_name}']",
     )
     if found_standard_name is not None:
         canonical_units = Unit(found_standard_name.find("canonical_units").text)
         return canonical_units.is_dimensionless()
     # if the standard name is not found, assume we need units for the time being
     else:
         return False
 
 
 def get_sea_names():
     """
     Returns a list of NODC sea names
 
-    source of list: https://www.nodc.noaa.gov/General/NODC-Archive/seanamelist.txt
+    source of list: https://www.ncei.noaa.gov/resources/ocean-data-format-codes
     """
     global _SEA_NAMES
     if _SEA_NAMES is None:
         buf = {}
         with open(
-            resource_filename("compliance_checker", "data/seanames.csv"), "r"
+            resource_filename("compliance_checker", "data/seanames.csv"),
         ) as f:
             reader = csv.reader(f)
             for code, sea_name in reader:
                 buf[sea_name] = code
         _SEA_NAMES = buf
     return _SEA_NAMES
 
@@ -169,23 +168,23 @@
         return False
 
     standard_name_test = getattr(ncvar, "standard_name", "")
     unitless = is_unitless(ds, variable)
 
     if not isinstance(standard_name_test, str):
         warnings.warn(
-            "Variable {} has non string standard name, "
-            "Attempting cast to string".format(variable)
+            f"Variable {variable} has non string standard name, Attempting cast to string",
+            stacklevel=2,
         )
         try:
             standard_name = str(standard_name_test)
         except ValueError:
             warnings.warn(
-                "Unable to cast standard name to string, excluding "
-                "from geophysical variables"
+                "Unable to cast standard name to string, excluding from geophysical variables",
+                stacklevel=2,
             )
     else:
         standard_name = standard_name_test
 
     # Is the standard name associated with coordinates
     if standard_name in {
         "time",
@@ -238,14 +237,15 @@
     # Skip count/index variables too
     if hasattr(ncvar, "sample_dimension") or hasattr(ncvar, "instance_dimension"):
         return False
 
     return True
 
 
+@lru_cache(128)
 def get_coordinate_variables(ds):
     """
     Returns a list of variable names that identify as coordinate variables.
 
     A coordinate variable is a netCDF variable with exactly one dimension. The
     name of this dimension must be equivalent to the variable name.
 
@@ -275,15 +275,15 @@
     defined by CF).
 
     :param netCDf4.Dataset ds: An open netCDF dataset
     """
     aux_vars = []
     # get any variables referecned by the coordinates attribute
     for ncvar in ds.get_variables_by_attributes(
-        coordinates=lambda x: isinstance(x, str)
+        coordinates=lambda x: isinstance(x, str),
     ):
         # split the coordinates into individual variable names
         referenced_variables = ncvar.coordinates.split(" ")
         # if the variable names exist, add them
         for referenced_variable in referenced_variables:
             if (
                 referenced_variable in ds.variables
@@ -305,15 +305,15 @@
         "depth",
         "altitude",
     ]
     coordinate_standard_names += DIMENSIONLESS_VERTICAL_COORDINATES
 
     # Some datasets like ROMS use multiple variables to define coordinates
     for ncvar in ds.get_variables_by_attributes(
-        standard_name=lambda x: x in coordinate_standard_names
+        standard_name=lambda x: x in coordinate_standard_names,
     ):
         if ncvar.name not in aux_vars:
             aux_vars.append(ncvar.name)
 
     # Remove any that are purely coordinate variables
     ret_val = []
     for aux_var in aux_vars:
@@ -498,15 +498,17 @@
 
     # Then axis
     for variable in nc.get_variables_by_attributes(axis="Y"):
         if variable.name not in latitude_variables:
             latitude_variables.append(variable.name)
 
     check_fn = partial(
-        attr_membership, value_set=VALID_LAT_UNITS, modifier_fn=lambda s: s.lower()
+        attr_membership,
+        value_set=VALID_LAT_UNITS,
+        modifier_fn=lambda s: s.lower(),
     )
     for variable in nc.get_variables_by_attributes(units=check_fn):
         if variable.name not in latitude_variables:
             latitude_variables.append(variable.name)
 
     return latitude_variables
 
@@ -563,15 +565,17 @@
 
     # Then axis
     for variable in nc.get_variables_by_attributes(axis="X"):
         if variable.name not in longitude_variables:
             longitude_variables.append(variable.name)
 
     check_fn = partial(
-        attr_membership, value_set=VALID_LON_UNITS, modifier_fn=lambda s: s.lower()
+        attr_membership,
+        value_set=VALID_LON_UNITS,
+        modifier_fn=lambda s: s.lower(),
     )
     for variable in nc.get_variables_by_attributes(units=check_fn):
         if variable.name not in longitude_variables:
             longitude_variables.append(variable.name)
 
     return longitude_variables
 
@@ -736,22 +740,23 @@
     def match_modifier_variables(standard_name_str):
         if standard_name_str is None:
             return False
         if not return_deprecated:
             matches = re.search(r"^\w+ +\w+", standard_name_str)
         else:
             matches = re.search(
-                r"^\w+ +(?:status_flag|number_of_observations)$", standard_name_str
+                r"^\w+ +(?:status_flag|number_of_observations)$",
+                standard_name_str,
             )
         return bool(matches)
 
     return [
         var.name
         for var in ds.get_variables_by_attributes(
-            standard_name=match_modifier_variables
+            standard_name=match_modifier_variables,
         )
     ]
 
 
 def get_flag_variables(ds):
     """
     Returns a list of variables that are defined as flag variables
@@ -924,15 +929,15 @@
     cf_role_vars = nc.get_variables_by_attributes(cf_role=lambda x: x is not None)
     if (
         not cf_role_vars
         or (len(cf_role_vars) > 1 and not is_compound)
         or (len(cf_role_vars) > 2 and is_compound)
     ):
         return False
-    cf_role_var = nc.get_variables_by_attributes(cf_role="{}_id".format(ftype))[0]
+    cf_role_var = nc.get_variables_by_attributes(cf_role=f"{ftype}_id")[0]
     if (
         cf_role_var.cf_role.split("_id")[0].lower() != ftype
     ):  # if cf_role_var returns None, this should raise an error?
         return False
 
     # now we'll check dimensions for singular feature types and/or
     # the first half of the compound featureType
@@ -943,18 +948,18 @@
     # Wow we check for the presence of an index variable or count variable;
     # NOTE that if no index or count variables exist, we can't determine with
     # certainty that this is invalid, because single-instance data sets
     # are valid representations of the ragged array structures. Instead,
     # if the index/count variable is present, we check that only one of
     # each is present and that their dimensions are correct
     index_vars = nc.get_variables_by_attributes(
-        instance_dimension=lambda x: x is not None
+        instance_dimension=lambda x: x is not None,
     )
     count_vars = nc.get_variables_by_attributes(
-        sample_dimension=lambda x: x is not None
+        sample_dimension=lambda x: x is not None,
     )
 
     # if the featureType isn't compound, shouldn't have both count and index
     if index_vars and count_vars and not is_compound:
         return False
 
     # single featureType, checking for valid index variable
@@ -1746,15 +1751,16 @@
     """
     Wrapper method
     """
 
     # NOTE
     # does this take into account single trajectory profile?
     if is_trajectory_profile_orthogonal(
-        nc, variable
+        nc,
+        variable,
     ) or is_trajectory_profile_incomplete(nc, variable):
         return True
 
     return False
 
 
 def is_2d_regular_grid(nc, variable):
```

### Comparing `compliance-checker-5.0.2/compliance_checker/data/cf-standard-name-table.xml` & `compliance-checker-5.1.0/compliance_checker/data/cf-standard-name-table.xml`

 * *Files identical despite different names*

### Comparing `compliance-checker-5.0.2/compliance_checker/data/seanames.csv` & `compliance-checker-5.1.0/compliance_checker/data/seanames.csv`

 * *Files identical despite different names*

### Comparing `compliance-checker-5.0.2/compliance_checker/data/templates/ccheck.html.j2` & `compliance-checker-5.1.0/compliance_checker/data/templates/ccheck.html.j2`

 * *Files identical despite different names*

### Comparing `compliance-checker-5.0.2/compliance_checker/data/templates/ccheck_wrapper.html.j2` & `compliance-checker-5.1.0/compliance_checker/data/templates/ccheck_wrapper.html.j2`

 * *Files identical despite different names*

### Comparing `compliance-checker-5.0.2/compliance_checker/ioos.py` & `compliance-checker-5.1.0/compliance_checker/ioos.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,15 +19,14 @@
     Result,
     TestCtx,
     check_has,
 )
 from compliance_checker.cf import util as cf_util  # not to be confused with cfutil.py
 from compliance_checker.cf.cf import CF1_6Check, CF1_7Check
 from compliance_checker.cfutil import (
-    get_coordinate_variables,
     get_geophysical_variables,
     get_instrument_variables,
     get_z_variables,
 )
 
 
 class IOOSBaseCheck(BaseCheck):
@@ -44,16 +43,17 @@
         """
         val = cls.std_check(ds, attr)
         msgs = []
 
         if not val:
             msgs.append(
                 "Attr '{}' (IOOS concept: '{}') not found in dataset".format(
-                    attr, concept_name
-                )
+                    attr,
+                    concept_name,
+                ),
             )
 
         return Result(priority, val, concept_name, msgs)
 
     @classmethod
     def _has_var_attr(cls, dataset, vname, attr, concept_name, priority=BaseCheck.HIGH):
         """
@@ -61,25 +61,29 @@
         """
         val = True
         msgs = []
         if vname not in dataset.variables:
             val = False
             msgs.append(
                 "Variable '{}' not present while checking for attr '{}' for IOOS concept: '{}'".format(
-                    vname, attr, concept_name
-                )
+                    vname,
+                    attr,
+                    concept_name,
+                ),
             )
         else:
             v = dataset.variables[vname]
             if attr not in v.ncattrs():
                 val = False
                 msgs.append(
                     "Attr '{}' not present on var '{}' while checking for IOOS concept: '{}'".format(
-                        attr, vname, concept_name
-                    )
+                        attr,
+                        vname,
+                        concept_name,
+                    ),
                 )
 
         return Result(priority, val, concept_name, msgs)
 
 
 class IOOSNCCheck(BaseNCCheck, IOOSBaseCheck):
     def check_time_period(self, ds):
@@ -148,27 +152,42 @@
 
         :param netCDF4.Dataset ds: An open netCDF dataset
         """
         return [
             self._has_attr(ds, "acknowledgement", "Platform Sponsor"),
             self._has_attr(ds, "publisher_email", "Station Publisher Email"),
             self._has_attr(
-                ds, "publisher_email", "Service Contact Email", BaseCheck.MEDIUM
+                ds,
+                "publisher_email",
+                "Service Contact Email",
+                BaseCheck.MEDIUM,
             ),
             self._has_attr(
-                ds, "institution", "Service Provider Name", BaseCheck.MEDIUM
+                ds,
+                "institution",
+                "Service Provider Name",
+                BaseCheck.MEDIUM,
             ),
             self._has_attr(
-                ds, "publisher_name", "Service Contact Name", BaseCheck.MEDIUM
+                ds,
+                "publisher_name",
+                "Service Contact Name",
+                BaseCheck.MEDIUM,
             ),
             self._has_attr(
-                ds, "Conventions", "Data Format Template Version", BaseCheck.MEDIUM
+                ds,
+                "Conventions",
+                "Data Format Template Version",
+                BaseCheck.MEDIUM,
             ),
             self._has_attr(
-                ds, "publisher_name", "Station Publisher Name", BaseCheck.HIGH
+                ds,
+                "publisher_name",
+                "Station Publisher Name",
+                BaseCheck.HIGH,
             ),
         ]
 
     def check_variable_attributes(self, ds):
         """
         Check IOOS concepts that come from NC variable attributes.
 
@@ -190,18 +209,21 @@
         msgs = []
         count = 0
 
         for k, v in ds.variables.items():
             if "standard_name" in v.ncattrs():
                 count += 1
             else:
-                msgs.append("Variable '{}' missing standard_name attr".format(k))
+                msgs.append(f"Variable '{k}' missing standard_name attr")
 
         return Result(
-            BaseCheck.MEDIUM, (count, len(ds.variables)), "Variable Names", msgs
+            BaseCheck.MEDIUM,
+            (count, len(ds.variables)),
+            "Variable Names",
+            msgs,
         )
 
     def check_altitude_units(self, ds):
         """
         If there's a variable named z, it must have units.
 
         @TODO: this is duplicated with check_variable_units
@@ -211,32 +233,38 @@
             msgs = []
             val = "units" in ds.variables["z"].ncattrs()
             if not val:
                 msgs.append("Variable 'z' has no units attr")
             return Result(BaseCheck.LOW, val, "Altitude Units", msgs)
 
         return Result(
-            BaseCheck.LOW, (0, 0), "Altitude Units", ["Dataset has no 'z' variable"]
+            BaseCheck.LOW,
+            (0, 0),
+            "Altitude Units",
+            ["Dataset has no 'z' variable"],
         )
 
     def check_variable_units(self, ds):
         """
         Ensures all variables have units.
         """
         msgs = []
         count = 0
 
         for k, v in ds.variables.items():
             if "units" in v.ncattrs():
                 count += 1
             else:
-                msgs.append("Variable '{}' missing units attr".format(k))
+                msgs.append(f"Variable '{k}' missing units attr")
 
         return Result(
-            BaseCheck.MEDIUM, (count, len(ds.variables)), "Variable Units", msgs
+            BaseCheck.MEDIUM,
+            (count, len(ds.variables)),
+            "Variable Units",
+            msgs,
         )
 
 
 class IOOS1_1Check(IOOSNCCheck):
     """
     Compliance checker implementation of IOOS Metadata Profile, Version 1.1
 
@@ -326,15 +354,15 @@
         if not val:
             msgs = [
                 (
                     'The value of "platform" global attribute should be set to another variable '
                     "which contains the details of the platform. If multiple platforms are "
                     "involved, a variable should be defined for each platform and referenced "
                     "from the geophysical variable in a space separated string."
-                )
+                ),
             ]
         return [Result(BaseCheck.HIGH, val, "platform variables", msgs)]
 
     def check_platform_variable_attributes(self, ds):
         """
         Platform variables must contain the following attributes:
             ioos_code
@@ -348,15 +376,18 @@
         platform_name = getattr(ds, "platform", "")
         # There can be multiple platforms defined here (space separated)
         for platform in platform_name.split(" "):
             if platform in ds.variables:
                 results += [
                     self._has_var_attr(ds, platform, "long_name", "Platform Long Name"),
                     self._has_var_attr(
-                        ds, platform, "short_name", "Platform Short Name"
+                        ds,
+                        platform,
+                        "short_name",
+                        "Platform Short Name",
                     ),
                     self._has_var_attr(ds, platform, "ioos_code", "Platform IOOS Code"),
                     self._has_var_attr(ds, platform, "type", "Platform Type"),
                 ]
         return results
 
     def check_geophysical_vars_fill_value(self, ds):
@@ -365,30 +396,37 @@
 
         :param netCDF4.Dataset ds: An open netCDF dataset
         """
         results = []
         for geo_var in get_geophysical_variables(ds):
             results.append(
                 self._has_var_attr(
-                    ds, geo_var, "_FillValue", "_FillValue", BaseCheck.MEDIUM
+                    ds,
+                    geo_var,
+                    "_FillValue",
+                    "_FillValue",
+                    BaseCheck.MEDIUM,
                 ),
             )
         return results
 
     def check_geophysical_vars_standard_name(self, ds):
         """
         Check that geophysical variables contain standard names.
 
         :param netCDF4.Dataset ds: An open netCDF dataset
         """
         results = []
         for geo_var in get_geophysical_variables(ds):
             results.append(
                 self._has_var_attr(
-                    ds, geo_var, "standard_name", "geophysical variables standard_name"
+                    ds,
+                    geo_var,
+                    "standard_name",
+                    "geophysical variables standard_name",
                 ),
             )
         return results
 
     def check_units(self, ds):
         """
         Required for most all variables that represent dimensional quantities.
@@ -437,15 +475,14 @@
 
     _cc_spec_version = "1.2"
     _cc_description = "IOOS Metadata Profile, Version 1.2"
     _cc_url = "https://ioos.github.io/ioos-metadata/ioos-metadata-profile-v1-2.html"
     register_checker = True
 
     def __init__(self):
-
         # instantiate objects used for delegation
         self.acdd1_6 = ACDD1_3Check()
         self.cf1_7 = CF1_7Check()
 
         # extend standard_names set to include QARTOD standard_names
         self._qartod_std_names = [
             "aggregate_quality_flag",
@@ -459,75 +496,64 @@
             "neighbor_test_quality_flag",
             "rate_of_change_test_quality_flag",
             "spike_test_quality_flag",
             "syntax_test_quality_flag",
         ]
         self.cf1_7._std_names._names.extend(self._qartod_std_names)
 
-        self._default_check_var_attrs = set(
-            [
-                ("_FillValue", BaseCheck.MEDIUM),
-                ("missing_value", BaseCheck.MEDIUM),
-                # ( "standard_name", BaseCheck.HIGH # already checked in CF1_7Check.check_standard_name()
-                # ( "units", BaseCheck.HIGH # already checked in CF1_7Check.check_units()
-            ]
-        )
+        self._default_check_var_attrs = {
+            ("_FillValue", BaseCheck.MEDIUM),
+            ("missing_value", BaseCheck.MEDIUM),
+            # ( "standard_name", BaseCheck.HIGH # already checked in CF1_7Check.check_standard_name()
+            # ( "units", BaseCheck.HIGH # already checked in CF1_7Check.check_units()
+        }
 
         # geophysical variables must have the following attrs:
         self.geophys_check_var_attrs = self._default_check_var_attrs.union(
-            set(
-                [
-                    ("standard_name_url", BaseCheck.MEDIUM),
-                    # ( "platform", BaseCheck.HIGH) # checked under check_single_platform()
-                    # ( "wmo_platform_code", BaseCheck.HIGH) # only "if applicable", see check_wmo_platform_code()
-                    # ( "ancillary_variables", BaseCheck.HIGH) # only "if applicable", see _check_var_gts_ingest()
-                    # ("accuracy", BaseCheck.MEDIUM), see check_accuracy
-                    ("precision", BaseCheck.MEDIUM),
-                    ("resolution", BaseCheck.MEDIUM),
-                ]
-            )
+            {
+                ("standard_name_url", BaseCheck.MEDIUM),
+                # ( "platform", BaseCheck.HIGH) # checked under check_single_platform()
+                # ( "wmo_platform_code", BaseCheck.HIGH) # only "if applicable", see check_wmo_platform_code()
+                # ( "ancillary_variables", BaseCheck.HIGH) # only "if applicable", see _check_var_gts_ingest()
+                # ("accuracy", BaseCheck.MEDIUM), see check_accuracy
+                ("precision", BaseCheck.MEDIUM),
+                ("resolution", BaseCheck.MEDIUM),
+            },
         )
 
-        # geospatial vars must have the following attrs:
-        self.geospat_check_var_attrs = self._default_check_var_attrs
-
         # valid contributor_role values
-        self.valid_contributor_roles = set(
-            [  # NERC and NOAA
-                "author",
-                "coAuthor",
-                "collaborator",
-                "contributor",
-                "custodian",
-                "distributor",
-                "editor",
-                "funder",
-                "mediator",
-                "originator",
-                "owner",
-                "pointOfContact",
-                "principalInvestigator",
-                "processor",
-                "publisher",
-                "resourceProvider",
-                "rightsHolder",
-                "sponsor",
-                "stakeholder",
-                "user",
-            ]
-        )
+        self.valid_contributor_roles = {  # NERC and NOAA
+            "author",
+            "coAuthor",
+            "collaborator",
+            "contributor",
+            "custodian",
+            "distributor",
+            "editor",
+            "funder",
+            "mediator",
+            "originator",
+            "owner",
+            "pointOfContact",
+            "principalInvestigator",
+            "processor",
+            "publisher",
+            "resourceProvider",
+            "rightsHolder",
+            "sponsor",
+            "stakeholder",
+            "user",
+        }
 
-        self.valid_contributor_role_vocabs = set(
-            [
-                "http://vocab.nerc.ac.uk/collection/G04/current/",
-                "https://vocab.nerc.ac.uk/collection/G04/current/",
-                "http://www.ngdc.noaa.gov/wiki/index.php?title=ISO_19115_and_19115-2_CodeList_Dictionaries#CI_RoleCode",
-                "https://www.ngdc.noaa.gov/wiki/index.php?title=ISO_19115_and_19115-2_CodeList_Dictionaries#CI_RoleCode",
-            ]
-        )
+        self.valid_contributor_role_vocabs = {
+            "http://vocab.nerc.ac.uk/collection/G04/current/",
+            "https://vocab.nerc.ac.uk/collection/G04/current/",
+            "http://www.ngdc.noaa.gov/wiki/index.php?title=ISO_19115_and_19115-2_CodeList_Dictionaries#CI_RoleCode",
+            "https://www.ngdc.noaa.gov/wiki/index.php?title=ISO_19115_and_19115-2_CodeList_Dictionaries#CI_RoleCode",
+        }
 
         self.required_atts = [
             ("Conventions", IOOS1_2_ConventionsValidator()),
             "creator_country",
             ("creator_email", base.EmailValidator()),
             "creator_institution",
             (
@@ -610,15 +636,15 @@
 
         Returns
         -------
         set of netCDF4.Variable
             Set of variables which are platform variables.
         """
         plat_vars = ds.get_variables_by_attributes(
-            platform=lambda p: isinstance(p, str)
+            platform=lambda p: isinstance(p, str),
         )
         return {
             ds.variables[var.platform]
             for var in plat_vars
             if var.platform in ds.variables
         }
 
@@ -724,70 +750,70 @@
                     role_val = _role in self.valid_contributor_roles
                     role_results.append(
                         Result(
                             BaseCheck.MEDIUM,
                             role_val,
                             "contributor_role",
                             None if role_val else [role_msg.format(_role)],
-                        )
+                        ),
                     )
             except TypeError:
                 role_results.append(
                     Result(
                         BaseCheck.MEDIUM,
                         False,
                         "contributor_role",
-                        ["contributor_role '{}' must be of type 'string'".format(role)],
-                    )
+                        [f"contributor_role '{role}' must be of type 'string'"],
+                    ),
                 )
         else:
             role_results.append(
                 Result(
                     BaseCheck.MEDIUM,
                     False,
                     "contributor_role",
                     ["contributor_role should be present"],
-                )
+                ),
             )
 
         vocb_results = []
         if vocb:
             try:
                 _vocbs = base.csv_splitter(vocb)
                 for _vocb in _vocbs:
                     vocb_val = _vocb in self.valid_contributor_role_vocabs
                     vocb_results.append(
                         Result(
                             BaseCheck.MEDIUM,
                             vocb_val,
                             "contributor_role_vocabulary",
                             None if vocb_val else [vocb_msg.format(_vocb)],
-                        )
+                        ),
                     )
             except TypeError:
                 vocb_results.append(
                     Result(
                         BaseCheck.MEDIUM,
                         False,
                         "contributor_role_vocabulary",
                         [
                             "contributor_role_vocabulary '{}' must be of type 'string'".format(
-                                vocb
-                            )
+                                vocb,
+                            ),
                         ],
-                    )
+                    ),
                 )
         else:
             vocb_results.append(
                 Result(
                     BaseCheck.MEDIUM,
                     False,
                     "contributor_role_vocabulary",
                     ["contributor_role_vocabulary should be present"],
-                )
+                ),
             )
 
         return role_results + vocb_results
 
     def check_geophysical_vars_have_attrs(self, ds):
         """
         All geophysical variables must have certain attributes.
@@ -800,15 +826,17 @@
         -------
         list: list of Result objects
         """
 
         # get geophysical variables
         geophys_vars = get_geophysical_variables(ds)  # list of str
         results = self._check_vars_have_attrs(  # list
-            ds, geophys_vars, self.geophys_check_var_attrs
+            ds,
+            geophys_vars,
+            self.geophys_check_var_attrs,
         )
 
         return results
 
     def check_accuracy(self, ds):
         """
         Special check for accuracy when in the salinity context.
@@ -842,36 +870,19 @@
 
             results.append(
                 Result(
                     BaseCheck.MEDIUM,
                     r,
                     "geophysical_variable:accuracy",
                     [msg.format(v=v)],
-                )
+                ),
             )
 
         return results
 
-    def check_geospatial_vars_have_attrs(self, ds):
-        """
-        All geospatial variables must have certain attributes.
-
-        Parameters
-        ----------
-        ds: netCDF4.Dataset
-
-        Returns
-        -------
-        list: list of Result objects
-        """
-
-        return self._check_vars_have_attrs(
-            ds, get_coordinate_variables(ds), self.geospat_check_var_attrs
-        )
-
     def _check_vars_have_attrs(self, ds, vars_to_check, atts_to_check):
         """
         Check that the variables in vars_to_check have the attributes in
         atts_to_check.
 
         Parameters
         ----------
@@ -888,15 +899,15 @@
                 results.append(
                     self._has_var_attr(
                         ds,
                         var,
                         attr_tuple[0],  # attribute name
                         attr_tuple[0],  # attribute name used as 'concept_name'
                         attr_tuple[1],  # priority level
-                    )
+                    ),
                 )
         return results
 
     def check_cf_role_variables(self, ds):
         """
         The IOOS-1.2 specification details the following requirements regarding
         the cf_role attribute and its relation to variable dimensionality:
@@ -928,15 +939,15 @@
                 BaseCheck.MEDIUM,
                 False,
                 "CF DSG: Invalid featureType",
                 [
                     (
                         f"Invalid featureType '{feature_type_attr}'; please see the "
                         "IOOS 1.2 Profile and CF-1.7 Conformance documents for valid featureType"
-                    )
+                    ),
                 ],
             )
 
         feature_type = feature_type_attr.lower()
 
         if feature_type == "timeseries":
             return self._check_feattype_timeseries_cf_role(ds)
@@ -951,33 +962,34 @@
             return self._check_feattype_trajectoryprof_cf_role(ds)
 
         elif feature_type == "profile":
             return self._check_feattype_profile_cf_role(ds)
 
         elif feature_type == "point":
             return Result(
-                BaseCheck.MEDIUM, True, "CF DSG: featureType=trajectoryProfile"
+                BaseCheck.MEDIUM,
+                True,
+                "CF DSG: featureType=trajectoryProfile",
             )
 
         else:
             return Result(
                 BaseCheck.MEDIUM,
                 False,
                 "CF DSG: Unknown featureType",
                 [
                     (
                         f"Invalid featureType '{feature_type_attr}'; "
                         "please see the IOOS 1.2 Profile and CF-1.7 "
                         "Conformance documents for valid featureType"
-                    )
+                    ),
                 ],
             )
 
     def _check_feattype_timeseries_cf_role(self, ds):
-
         ts_msg = (
             "Dimension length of variable with cf_role={cf_role} "
             "(the '{dim_type}' dimension) is {dim_len}. "
             "The IOOS Profile restricts timeSeries "
             "datasets with multiple features to share the same lat/lon position "
             "(i.e. to exist on the same platform). Datasets that include multiple "
             "platforms are not valid and will cause harvesting errors."
@@ -987,42 +999,43 @@
         cf_role_vars = ds.get_variables_by_attributes(cf_role="timeseries_id")
         if (not cf_role_vars) or (len(cf_role_vars) > 1):
             _val = False
             msgs = [
                 (
                     "The IOOS-1.2 Profile specifies a single variable "
                     "must be present with attribute cf_role=timeseries_id"
-                )
+                ),
             ]
 
         else:
             _v = cf_role_vars[0]
             _dims = _v.get_dims()
             if not _dims:
                 _dimsize = 0
             else:
                 _dimsize = _dims[0].size
 
             # dimension size must be == 1
             _val = _dimsize == 1
             msgs = [
                 ts_msg.format(
-                    cf_role="timeseries_id", dim_type="station", dim_len=_dimsize
-                )
+                    cf_role="timeseries_id",
+                    dim_type="station",
+                    dim_len=_dimsize,
+                ),
             ]
 
         return Result(
             BaseCheck.HIGH,
             _val,
             "CF DSG: featureType=timeseries",
             msgs,
         )
 
     def _check_feattype_timeseriesprof_cf_role(self, ds):
-
         ts_prof_msg = (
             "Dimension length of non-platform variable with cf_role={cf_role} "
             " (the '{dim_type}' dimension) is {dim_len}. "
             "The IOOS profile restricts timeSeriesProfile datasets to a "
             "single platform (ie. station) per dataset "
             "(the profile dimension is permitted to be >= 1."
         )
@@ -1034,15 +1047,15 @@
 
         if len(cf_role_vars) != 2:
             _val = False
             msgs = [
                 (
                     "Datasets of featureType=timeSeriesProfile must have variables "
                     "containing cf_role=timeseries_id and cf_role=profile_id"
-                )
+                ),
             ]
 
         else:
             _ts_id_dims = cf_role_vars[0].get_dims()  # timeseries_id dimensions
             if not _ts_id_dims:
                 _ts_id_dimsize = 0
             else:
@@ -1054,20 +1067,25 @@
             else:
                 _pf_id_dimsize = _pf_id_dims[0].size
 
             # timeseries_id must be == 1, profile >= 1
             _val = _ts_id_dimsize == 1 and _pf_id_dimsize >= 1
             msgs = [
                 ts_prof_msg.format(
-                    cf_role="timeseries_id", dim_type="station", dim_len=_ts_id_dimsize
-                )
+                    cf_role="timeseries_id",
+                    dim_type="station",
+                    dim_len=_ts_id_dimsize,
+                ),
             ]
 
         return Result(
-            BaseCheck.HIGH, _val, "CF DSG: featureType=timeSeriesProfile", msgs
+            BaseCheck.HIGH,
+            _val,
+            "CF DSG: featureType=timeSeriesProfile",
+            msgs,
         )
 
     def _check_feattype_trajectory_cf_role(self, ds):
         trj_msg = (
             "Dimension length of non-platform variable with cf_role={cf_role} "
             " (the '{dim_type}' dimension) is {dim_len}. "
             "The IOOS profile restricts trjectory "
@@ -1078,31 +1096,33 @@
 
         if len(cf_role_vars) != 1:
             _val = False
             msgs = [
                 (
                     "Datasets of featureType=trajectory must have a variable "
                     "containing cf_role=trajectory_id"
-                )
+                ),
             ]
 
         else:
             _v = cf_role_vars[0]
             _dims = _v.get_dims()
             if not _dims:
                 _dimsize = 0
             else:
                 _dimsize = _dims[0].size
 
             # trajectory dimension must be 1
             _val = _dimsize == 1
             msgs = [
                 trj_msg.format(
-                    cf_role="trajectory_id", dim_type="station", dim_len=_dimsize
-                )
+                    cf_role="trajectory_id",
+                    dim_type="station",
+                    dim_len=_dimsize,
+                ),
             ]
 
         return Result(BaseCheck.HIGH, _val, "CF DSG: featureType=trajectory", msgs)
 
     def _check_feattype_trajectoryprof_cf_role(self, ds):
         trj_prof_msg = (
             "Dimension length of non-platform variable with cf_role={cf_role} "
@@ -1119,15 +1139,15 @@
 
         if len(cf_role_vars) != 2:
             _val = False
             msgs = [
                 (
                     "Datasets of featureType=trajectoryProfile must have variables "
                     "containing cf_role=trajectory_id and cf_role=profile_id"
-                )
+                ),
             ]
 
         else:
             _trj_id_dims = cf_role_vars[0].get_dims()
             if not _trj_id_dims:
                 _trj_id_dimsize = 0
             else:
@@ -1140,20 +1160,25 @@
             else:
                 _prf_id_dimsize = _prf_id_dims[0].size
 
             # trajectory dim must be == 1, profile must be >= 1
             _val = _trj_id_dimsize == 1 and _prf_id_dimsize >= 1
             msgs = [
                 trj_prof_msg.format(
-                    cf_role="trajectory_id", dim_type="station", dim_len=_trj_id_dimsize
-                )
+                    cf_role="trajectory_id",
+                    dim_type="station",
+                    dim_len=_trj_id_dimsize,
+                ),
             ]
 
         return Result(
-            BaseCheck.HIGH, _val, "CF DSG: featureType=trajectoryProfile", msgs
+            BaseCheck.HIGH,
+            _val,
+            "CF DSG: featureType=trajectoryProfile",
+            msgs,
         )
 
     def _check_feattype_profile_cf_role(self, ds):
         prof_msg = (
             "Dimension length of non-platform variable with cf_role={cf_role} "
             " (the '{dim_type}' dimension) is {dim_len}. "
             "The IOOS profile restricts profile datasets to a single "
@@ -1161,31 +1186,33 @@
         )
 
         # looking for cf_role=profile_id
         cf_role_vars = ds.get_variables_by_attributes(cf_role="profile_id")
         if (not cf_role_vars) or (len(cf_role_vars) > 1):
             _val = False
             msgs = [
-                "None or multiple variables found with cf_role=profile_id; only one is allowed"
+                "None or multiple variables found with cf_role=profile_id; only one is allowed",
             ]
 
         else:
             _v = cf_role_vars[0]
             _dims = _v.get_dims()
             if not _dims:
                 _dimsize = 0
             else:
                 _dimsize = _dims[0].size
 
             # only one profile valid
             _val = _dimsize == 1
             msgs = [
                 prof_msg.format(
-                    cf_role="profile_id", dim_type="profile", dim_len=_dimsize
-                )
+                    cf_role="profile_id",
+                    dim_type="profile",
+                    dim_len=_dimsize,
+                ),
             ]
 
         return Result(BaseCheck.HIGH, _val, "CF DSG: featureType=profile", msgs)
 
     def check_creator_and_publisher_type(self, ds):
         """
         Check if global attribute creator_type and publisher_type
@@ -1215,19 +1242,19 @@
                 expected_types = {"person", "group", "institution", "position"}
                 if att_value in expected_types:
                     pass_stat = True
                 else:
                     pass_stat = False
                     messages.append(
                         "If specified, {} must be in value list "
-                        "({})".format(global_att_name, sorted(expected_types))
+                        "({})".format(global_att_name, sorted(expected_types)),
                     )
 
             result_list.append(
-                Result(BaseCheck.MEDIUM, pass_stat, global_att_name, messages)
+                Result(BaseCheck.MEDIUM, pass_stat, global_att_name, messages),
             )
 
         return result_list
 
     def check_platform_global(self, ds):
         """
         The "platform" attribute must be a single string containing
@@ -1272,15 +1299,15 @@
         platform_set = set()
         for v in ds.get_variables_by_attributes(platform=lambda x: x is not None):
             platform_set.add(v.getncattr("platform"))
 
         num_platforms = len(platform_set)
         if num_platforms > 1 and glb_platform:
             msg = "A dataset may only have one platform; {} found".format(
-                len(platform_set)
+                len(platform_set),
             )
             val = False
 
         elif (not glb_platform) and num_platforms > 0:
             msg = 'If a platform variable exists, a global attribute "platform" must also exist'
             val = False
 
@@ -1296,30 +1323,33 @@
             val = True
 
         return Result(BaseCheck.HIGH, val, "platform", None if val else [msg])
 
     def check_platform_vocabulary(self, ds):
         """
         The platform_vocabulary attribute is recommended to be a URL to
-        http://mmisw.org/ont/ioos/platform or
+        https://mmisw.org/ont/ioos/platform or
         http://vocab.nerc.ac.uk/collection/L06/current/. However,
         it is required to at least be a URL.
 
         Args:
             ds (netCDF4.Dataset): open Dataset
 
         Returns:
             Result
         """
 
         m = "platform_vocabulary must be a valid URL"
         pvocab = getattr(ds, "platform_vocabulary", "")
         val = bool(validators.url(pvocab))
         return Result(
-            BaseCheck.MEDIUM, val, "platform_vocabulary", None if val else [m]
+            BaseCheck.MEDIUM,
+            val,
+            "platform_vocabulary",
+            None if val else [m],
         )
 
     def _check_gts_ingest_val(self, val):
         """
         Check that `val` is a str and is equal to "true" or "false"
 
         Parameters
@@ -1407,15 +1437,15 @@
         gts_ingest_value = getattr(ds, "gts_ingest", None)
 
         is_valid_string = True
         if isinstance(gts_ingest_value, str):
             is_valid_string = self._check_gts_ingest_val(gts_ingest_value)
 
         fail_message = [
-            'Global attribute "gts_ingest" must be a string "true" or "false"'
+            'Global attribute "gts_ingest" must be a string "true" or "false"',
         ]
         return Result(
             BaseCheck.HIGH,
             is_valid_string,
             "NDBC/GTS Ingest Requirements",
             None if is_valid_string else fail_message,
         )
@@ -1472,15 +1502,15 @@
 
         return avar_val and valid_std_name and has_udunits
 
     def check_gts_ingest_requirements(self, ds):
         """
         Check which variables qualify for ingest.
 
-        According to https://ioos.github.io/ioos-metadata/ioos-metadata-profile-v1-2.html#requirements-for-ioos-dataset-gts-ingest,
+        According to https://ioos.github.io/ioos-metadata/ioos-metadata-profile-v1-2.html#requirements-for-ioos-dataset-ndbcgts-ingest,
         the gts_ingest is "required, if applicable". Any variables which a user
         would like ingested must also contain the gts_ingest attribute with a
         value of true. The variable must:
           - have a valid CF standard_name attribute (already checked)
           - have an ancillary variable reqpresenting QARTOD aggregate flags
           - have a valid udunits units attribute (already checked)
 
@@ -1508,26 +1538,24 @@
         var_passed_ingest_msg = (
             "The following variables qualified for NDBC/GTS Ingest: {}\n"
         )
 
         var_passed_ingest_reqs = set()
         for v in ds.get_variables_by_attributes(gts_ingest=lambda x: x == "true"):
             var_passed_ingest_reqs.add(
-                (v.name, self._var_qualifies_for_gts_ingest(ds, v))
+                (v.name, self._var_qualifies_for_gts_ingest(ds, v)),
             )
 
         # always show which variables have passed
-        _var_passed = map(
-            lambda y: y[0], filter(lambda x: x[1], var_passed_ingest_reqs)
-        )
+        _var_passed = (y[0] for y in filter(lambda x: x[1], var_passed_ingest_reqs))
 
-        all_passed_ingest_reqs = all(map(lambda x: x[1], var_passed_ingest_reqs))
+        all_passed_ingest_reqs = all(x[1] for x in var_passed_ingest_reqs)
         if not all_passed_ingest_reqs:
-            _var_failed = map(
-                lambda y: y[0], filter(lambda x: not x[1], var_passed_ingest_reqs)
+            _var_failed = (
+                y[0] for y in filter(lambda x: not x[1], var_passed_ingest_reqs)
             )
 
         return Result(
             BaseCheck.HIGH,
             False,  # always fail
             "NDBC/GTS Ingest Requirements",
             [var_passed_ingest_msg.format(", ".join(_var_passed))]
@@ -1555,49 +1583,51 @@
 
         # check for component, disciminant
         for instr in instr_vars:
             if instr in ds.variables:
                 compnt = getattr(ds.variables[instr], "component", None)
                 m = [
                     "component attribute of {} ({}) must be a string".format(
-                        instr, compnt
-                    )
+                        instr,
+                        compnt,
+                    ),
                 ]
                 if compnt:
                     results.append(
                         Result(
                             BaseCheck.MEDIUM,
                             isinstance(compnt, str),
                             "instrument_variable",
                             m,
-                        )
+                        ),
                     )
                 else:
                     results.append(
-                        Result(BaseCheck.MEDIUM, True, "instrument_variable", m)
+                        Result(BaseCheck.MEDIUM, True, "instrument_variable", m),
                     )
 
                 disct = getattr(ds.variables[instr], "discriminant", None)
                 m = [
                     "discriminant attribute of {} ({}) must be a string".format(
-                        instr, disct
-                    )
+                        instr,
+                        disct,
+                    ),
                 ]
                 if disct:
                     results.append(
                         Result(
                             BaseCheck.MEDIUM,
                             isinstance(disct, str),
                             "instrument_variable",
                             m,
-                        )
+                        ),
                     )
                 else:
                     results.append(
-                        Result(BaseCheck.MEDIUM, True, "instrument_variable", m)
+                        Result(BaseCheck.MEDIUM, True, "instrument_variable", m),
                     )
 
         return results
 
     def check_qartod_variables_flags(self, ds):
         """
         https://ioos.github.io/ioos-metadata/ioos-metadata-profile-v1-2.html#quality-controlqartod
@@ -1613,42 +1643,41 @@
         -------
         list of Result objects
         """
 
         results = []
         # get qartod variables
         for v in ds.get_variables_by_attributes(
-            standard_name=lambda x: x in self._qartod_std_names
+            standard_name=lambda x: x in self._qartod_std_names,
         ):
-
             missing_msg = "flag_{} not present on {}"
 
             # check if each has flag_values, flag_meanings
             # need isinstance() as can't compare truth value of array
             if getattr(v, "flag_values", None) is None:
                 results.append(
                     Result(
                         BaseCheck.MEDIUM,
                         False,
                         "qartod_variables flags",
                         missing_msg.format("values", v.name),
-                    )
+                    ),
                 )
 
             else:  # if exist, test
                 results.append(self.cf1_7._check_flag_values(ds, v.name))
 
             if getattr(v, "flag_meanings", None) is None:
                 results.append(
                     Result(
                         BaseCheck.MEDIUM,
                         False,
                         "qartod_variables flags",
                         missing_msg.format("meanings", v.name),
-                    )
+                    ),
                 )
 
             else:  # if exist, test
                 results.append(self.cf1_7._check_flag_meanings(ds, v.name))
 
         # Ensure message name is "qartod_variables flags"
         # NOTE this is a bit of a hack to shove into CF results
@@ -1668,36 +1697,36 @@
 
         Returns:
             list of Results
         """
 
         results = []
         for v in ds.get_variables_by_attributes(
-            standard_name=lambda x: x in self._qartod_std_names
+            standard_name=lambda x: x in self._qartod_std_names,
         ):
             attval = getattr(v, "references", None)
             if attval is None:
                 msg = (
                     '"references" attribute not present for variable {}.'
                     "If present, it should be a valid URL."
                 ).format(v.name)
                 val = False
             else:
                 msg = '"references" attribute for variable "{}" must be a valid URL'.format(
-                    v.name
+                    v.name,
                 )
                 val = bool(validators.url(attval))
 
             results.append(
                 Result(
                     BaseCheck.MEDIUM,
                     val,
                     "qartod_variable:references",
                     None if val else [msg],
-                )
+                ),
             )
 
         return results
 
     def check_wmo_platform_code(self, ds):
         """
         Per the spec:
@@ -1757,37 +1786,37 @@
                 Result(
                     BaseCheck.MEDIUM,
                     valid,
                     "instrument_variable:make_model",
                     None
                     if valid
                     else [f"Attribute {v}:make_model ({mm}) should be a string"],
-                )
+                ),
             )
 
             # calibration_date
             cd = getattr(_v, "calibration_date", "")
             # thanks folks https://stackoverflow.com/questions/41129921/validate-an-iso-8601-datetime-string-in-python
             valid = bool(
                 re.match(
                     r"^(-?(?:[1-9][0-9]*)?[0-9]{4})-(1[0-2]|0[1-9])-(3[01]|0[1-9]|[12][0-9])T(2[0-3]|[01][0-9]):([0-5][0-9]):([0-5][0-9])(\.[0-9]+)?(Z|[+-](?:2[0-3]|[01][0-9]):[0-5][0-9])?$",
                     cd,
-                )
+                ),
             )
             results.append(
                 Result(
                     BaseCheck.MEDIUM,
                     valid,
                     "instrument_variable:calibration_date",
                     None
                     if valid
                     else [
-                        f"Attribute {v}:calibration_date ({cd}) should be an ISO-8601 string"
+                        f"Attribute {v}:calibration_date ({cd}) should be an ISO-8601 string",
                     ],
-                )
+                ),
             )
 
         return results
 
 
 class IOOSBaseSOSCheck(BaseCheck):
     _cc_spec = "ioos_sos"
@@ -1798,15 +1827,14 @@
     )
     register_checker = True
     # requires login
     _cc_url = "http://sdf.ndbc.noaa.gov/sos/"
 
 
 class IOOSSOSGCCheck(BaseSOSGCCheck, IOOSBaseSOSCheck):
-
     # set up namespaces for XPath
     ns = Namespaces().get_namespaces(["sos", "gml", "xlink"])
     ns["ows"] = Namespaces().get_namespace("ows110")
 
     @check_has(BaseCheck.HIGH)
     def check_high(self, ds):
         return []
@@ -1877,15 +1905,14 @@
 
     @check_has(BaseCheck.LOW)
     def check_suggested(self, ds):
         return ["altitude_units"]
 
 
 class IOOSSOSDSCheck(BaseSOSDSCheck, IOOSBaseSOSCheck):
-
     # set up namespaces for XPath
     ns = Namespaces().get_namespaces(["sml", "swe", "gml", "xlink"])
 
     @check_has(BaseCheck.HIGH)
     def check_high(self, ds):
         return [
             (
```

### Comparing `compliance-checker-5.0.2/compliance_checker/protocols/cdl.py` & `compliance-checker-5.1.0/compliance_checker/protocols/cdl.py`

 * *Files identical despite different names*

### Comparing `compliance-checker-5.0.2/compliance_checker/protocols/netcdf.py` & `compliance-checker-5.1.0/compliance_checker/protocols/netcdf.py`

 * *Files 2% similar despite different names*

```diff
@@ -79,15 +79,16 @@
     # Some datasets do not support HEAD requests!  The vast majority will,
     # however, support GET requests
     try:
         head_req = requests.head(ds_str, allow_redirects=True, timeout=10)
         head_req.raise_for_status()
     except requests.exceptions.RequestException as e:
         warnings.warn(
-            "Received exception when making HEAD request to {}: {}".format(ds_str, e)
+            f"Received exception when making HEAD request to {ds_str}: {e}",
+            stacklevel=2,
         )
         content_type = None
     else:
         content_type = head_req.headers.get("content-type")
 
     # if the Content-Type header returned was "application/x-netcdf",
     # or a netCDF file (not OPeNDAP) we can open this into a Dataset
```

### Comparing `compliance-checker-5.0.2/compliance_checker/protocols/opendap.py` & `compliance-checker-5.1.0/compliance_checker/protocols/opendap.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,27 +21,27 @@
 
     Returns
     -------
     str
     """
 
     # get dds
-    with urllib.request.urlopen("{}.dds".format(url)) as resp:
+    with urllib.request.urlopen(f"{url}.dds") as resp:
         _str = resp.read().decode()[8:]
 
     # remove beginning and ending braces, split on newlines
     no_braces_newlines = list(
-        filter(lambda x: "{" not in x and "}" not in x, _str.split("\n"))
+        filter(lambda x: "{" not in x and "}" not in x, _str.split("\n")),
     )
 
     # remove all the extra space used in the DDS string
-    no_spaces = list(filter(None, map(lambda x: x.strip(" "), no_braces_newlines)))
+    no_spaces = list(filter(None, (x.strip(" ") for x in no_braces_newlines)))
 
     # now need to split from type, grab only the variable and remove ;
-    vars_only = list(map(lambda x: x.split(" ")[-1].strip(";"), no_spaces))
+    vars_only = [x.split(" ")[-1].strip(";") for x in no_spaces]
 
     # encode as proper URL characters
     varstr = urllib.parse.quote(",".join(vars_only))
     return varstr
 
 
 def is_opendap(url):
```

### Comparing `compliance-checker-5.0.2/compliance_checker/runner.py` & `compliance-checker-5.1.0/compliance_checker/runner.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-import io
 import json
 import os
 import sys
 import traceback
 from collections import OrderedDict
 from contextlib import contextmanager
 
@@ -18,15 +17,15 @@
     sys.stdout = stream
     try:
         yield
     finally:
         sys.stdout = old_stdout
 
 
-class ComplianceChecker(object):
+class ComplianceChecker:
     """
     Compliance Checker runner class.
 
     Ties together the entire compliance checker framework, is used from
     the command line or can be used via import.
     """
 
@@ -37,15 +36,15 @@
         ds_loc,
         checker_names,
         verbose,
         criteria,
         skip_checks=None,
         include_checks=None,
         output_filename="-",
-        output_format=["text"],
+        output_format="text",
         options=None,
     ):
         """
         Static check runner.
 
         @param  ds_loc          Dataset location (url or file)
         @param  checker_names   List of string names to run, should match keys of checkers dict (empty list means run all)
@@ -81,15 +80,15 @@
                 all_groups.append(group[0])
             # TODO: consider wrapping in a proper context manager instead
             if hasattr(ds, "close"):
                 ds.close()
 
             if not score_groups:
                 raise ValueError(
-                    "No checks found, please check the name of the checker(s) and that they are installed"
+                    "No checks found, please check the name of the checker(s) and that they are installed",
                 )
             else:
                 score_dict[loc] = score_groups
 
         # define a score limit to truncate the output to the strictness level
         # specified by the user
         if criteria == "normal":
@@ -105,33 +104,33 @@
                     cls.stdout_output(cs, score_dict, verbose, limit)
                 # need to redirect output from stdout since print functions are
                 # presently used to generate the standard report output
                 else:
                     if len(output_format) > 1:
                         # Update file name if needed
                         output_filename = "{}.txt".format(
-                            os.path.splitext(output_filename)[0]
+                            os.path.splitext(output_filename)[0],
                         )
-                    with io.open(output_filename, "w", encoding="utf-8") as f:
+                    with open(output_filename, "w", encoding="utf-8") as f:
                         with stdout_redirector(f):
                             cls.stdout_output(cs, score_dict, verbose, limit)
 
             elif out_fmt == "html":
                 # Update file name if needed
                 if len(output_format) > 1 and output_filename != "-":
                     output_filename = "{}.html".format(
-                        os.path.splitext(output_filename)[0]
+                        os.path.splitext(output_filename)[0],
                     )
                 cls.html_output(cs, score_dict, output_filename, ds_loc, limit)
 
             elif out_fmt in {"json", "json_new"}:
                 # Update file name if needed
                 if len(output_format) > 1 and output_filename != "-":
                     output_filename = "{}.json".format(
-                        os.path.splitext(output_filename)[0]
+                        os.path.splitext(output_filename)[0],
                     )
                 cls.json_output(cs, score_dict, output_filename, ds_loc, limit, out_fmt)
 
             else:
                 raise TypeError("Invalid format %s" % out_fmt)
 
             errors_occurred = cls.check_errors(score_groups, verbose)
@@ -154,19 +153,26 @@
         @param limit        The degree of strictness, 1 being the strictest, and going up from there.
         """
 
         for ds, score_groups in score_dict.items():
             for checker, rpair in score_groups.items():
                 groups, errors = rpair
                 score_list, points, out_of = cs.standard_output(
-                    ds, limit, checker, groups
+                    ds,
+                    limit,
+                    checker,
+                    groups,
                 )
                 # send list of grouped result objects to stdout & reasoning_routine
                 cs.standard_output_generation(
-                    groups, limit, points, out_of, check=checker
+                    groups,
+                    limit,
+                    points,
+                    out_of,
+                    check=checker,
                 )
         return groups
 
     @classmethod
     def html_output(cls, cs, score_dict, output_filename, ds_loc, limit):
         """
         Generates rendered HTML output for the compliance score(s)
@@ -174,29 +180,35 @@
         @param score_groups    List of results
         @param output_filename The file path to output to
         @param ds_loc          List of source datasets
         @param limit           The degree of strictness, 1 being the strictest, and going up from there.
         """
         checkers_html = []
         for ds, score_groups in score_dict.items():
-            for checker, (groups, errors) in score_groups.items():
+            for checker, (groups, _errors) in score_groups.items():
                 checkers_html.append(cs.checker_html_output(checker, groups, ds, limit))
 
         html = cs.html_output(checkers_html)
         if output_filename == "-":
             print(html)
         else:
-            with io.open(output_filename, "w", encoding="utf8") as f:
+            with open(output_filename, "w", encoding="utf8") as f:
                 f.write(html)
 
         return groups
 
     @classmethod
     def json_output(
-        cls, cs, score_dict, output_filename, ds_loc, limit, output_type="json"
+        cls,
+        cs,
+        score_dict,
+        output_filename,
+        ds_loc,
+        limit,
+        output_type="json",
     ):
         """
         Generates JSON output for the ocmpliance score(s)
         @param cs              Compliance Checker Suite
         @param score_groups    List of results
         @param output_filename The file path to output to
         @param ds_loc          List of source datasets
@@ -205,15 +217,15 @@
         @param output_type     Either 'json' or 'json_new'. json_new is the new
                                json output format that supports multiple datasets
         """
         results = {}
         # json output keys out at the top level by
         if len(score_dict) > 1 and output_type != "json_new":
             raise ValueError(
-                "output_type must be set to 'json_new' if outputting multiple datasets to a single json file or stdout"
+                "output_type must be set to 'json_new' if outputting multiple datasets to a single json file or stdout",
             )
 
         if output_type == "json":
             for ds, score_groups in score_dict.items():
                 for checker, rpair in score_groups.items():
                     groups, errors = rpair
                     results[checker] = cs.dict_output(
@@ -229,15 +241,15 @@
                     results[ds] = {}
                     results[ds][checker] = cs.dict_output(checker, groups, ds, limit)
         json_results = json.dumps(results, indent=2, ensure_ascii=False)
 
         if output_filename == "-":
             print(json_results)
         else:
-            with io.open(output_filename, "w", encoding="utf8") as f:
+            with open(output_filename, "w", encoding="utf8") as f:
                 f.write(json_results)
 
         return groups
 
     @classmethod
     def check_errors(cls, score_groups, verbose):
         """
@@ -255,17 +267,18 @@
                 print(
                     "WARNING: The following exceptions occurred during the %s checker (possibly indicate compliance checker issues):"
                     % checker,
                     file=sys.stderr,
                 )
                 for check_name, epair in errors.items():
                     print(
-                        "%s.%s: %s" % (checker, check_name, epair[0]), file=sys.stderr
+                        f"{checker}.{check_name}: {epair[0]}",
+                        file=sys.stderr,
                     )
 
                     if verbose > 0:
                         traceback.print_tb(
-                            epair[1].tb_next.tb_next
+                            epair[1].tb_next.tb_next,
                         )  # skip first two as they are noise from the running itself @TODO search for check_name
                         print(file=sys.stderr)
 
         return errors_occurred
```

### Comparing `compliance-checker-5.0.2/compliance_checker/suite.py` & `compliance-checker-5.1.0/compliance_checker/suite.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,20 +9,20 @@
 import re
 import subprocess
 import sys
 import textwrap
 import warnings
 from collections import defaultdict
 from datetime import datetime, timezone
+from distutils.version import StrictVersion
 from operator import itemgetter
 from pathlib import Path
 from urllib.parse import urlparse
 
 import requests
-from distutils.version import StrictVersion
 from lxml import etree as ET
 from netCDF4 import Dataset
 from owslib.sos import SensorObservationService
 from owslib.swe.sensor.sml import SensorML
 from pkg_resources import working_set
 
 from compliance_checker import MemoizedDataset, __version__, tempnc
@@ -45,21 +45,21 @@
     """
     # return a dedented, then indented two spaces docstring with leading and
     # trailing whitespace removed.
     return re.sub(
         r"^(?=.)",
         "  ",
         textwrap.dedent(
-            re.split(r"\n\s*:\w", docstring, flags=re.MULTILINE)[0]
+            re.split(r"\n\s*:\w", docstring, flags=re.MULTILINE)[0],
         ).strip(),
         flags=re.MULTILINE,
     )
 
 
-class CheckSuite(object):
+class CheckSuite:
     checkers = (
         {}
     )  # Base dict of checker names to BaseCheck derived types, override this in your CheckSuite implementation
     templates_root = "compliance_checker"  # modify to load alternative Jinja2 templates
 
     def __init__(self, options=None):
         self.col_width = 40
@@ -86,34 +86,34 @@
         :param check_suite: Check suite object
         :param verbose: Integer indicating whether to print verbose output
         :type verbose: int
         """
         for checker in sorted(self.checkers.keys()):
             version = getattr(self.checkers[checker], "_cc_checker_version", "???")
             if verbose > 0:
-                print(" - {} (v{})".format(checker, version))
+                print(f" - {checker} (v{version})")
             elif ":" in checker and not checker.endswith(
-                ":latest"
+                ":latest",
             ):  # Skip the "latest" output
-                print(" - {}".format(checker))
+                print(f" - {checker}")
 
     def _print_checker(self, checker_obj):
         """
         Prints each available check and a description with an abridged
         docstring for a given checker object
         :param checker_obj: Checker object on which to operate
         :type checker_obj: subclass of compliance_checker.base.BaseChecker
         """
 
-        check_functions = self._get_checks(checker_obj, defaultdict(lambda: None))
+        check_functions = self._get_checks(checker_obj, {}, defaultdict(lambda: None))
         for c, _ in check_functions:
-            print("- {}".format(c.__name__))
+            print(f"- {c.__name__}")
             if c.__doc__ is not None:
                 u_doc = c.__doc__
-                print("\n{}\n".format(extract_docstring_summary(u_doc)))
+                print(f"\n{extract_docstring_summary(u_doc)}\n")
 
     @classmethod
     def add_plugin_args(cls, parser):
         """
         Add command line arguments for external plugins that generate checker
         classes
         """
@@ -145,38 +145,42 @@
         :param checkers: An iterable containing the checker objects
         """
 
         for c in checkers:
             try:
                 check_obj = c.resolve()
                 if hasattr(check_obj, "_cc_spec") and hasattr(
-                    check_obj, "_cc_spec_version"
+                    check_obj,
+                    "_cc_spec_version",
                 ):
                     check_version_str = ":".join(
-                        (check_obj._cc_spec, check_obj._cc_spec_version)
+                        (check_obj._cc_spec, check_obj._cc_spec_version),
                     )
                     cls.checkers[check_version_str] = check_obj
                 # TODO: remove this once all checkers move over to the new
                 #       _cc_spec, _cc_spec_version
                 else:
                     # if _cc_spec and _cc_spec_version attributes aren't
                     # present, fall back to using name attribute
                     checker_name = getattr(check_obj, "name", None) or getattr(
-                        check_obj, "_cc_spec", None
+                        check_obj,
+                        "_cc_spec",
+                        None,
                     )
                     warnings.warn(
                         "Checker for {} should implement both "
                         '"_cc_spec" and "_cc_spec_version" '
                         'attributes. "name" attribute is deprecated. '
                         "Assuming checker is latest version.",
                         DeprecationWarning,
+                        stacklevel=2,
                     )
                     # append "unknown" to version string since no versioning
                     # info was provided
-                    cls.checkers["{}:unknown".format(checker_name)] = check_obj
+                    cls.checkers[f"{checker_name}:unknown"] = check_obj
 
             except Exception as e:
                 print("Could not load", c, ":", e, file=sys.stderr)
         # find the latest version of versioned checkers and set that as the
         # default checker for compliance checker if no version is specified
         ver_checkers = sorted([c.split(":", 1) for c in cls.checkers if ":" in c])
         for spec, versions in itertools.groupby(ver_checkers, itemgetter(0)):
@@ -249,15 +253,18 @@
                 )
                 if max_level is None or res.weight > max_level:
                     check_val.append(res)
 
             return check_val
         else:
             check_val = fix_return_value(
-                val, check_method.__func__.__name__, check_method, check_method.__self__
+                val,
+                check_method.__func__.__name__,
+                check_method,
+                check_method.__self__,
             )
             if max_level is None or check_val.weight > max_level:
                 return [check_val]
             else:
                 return []
 
     def _get_check_versioned_name(self, check_name):
@@ -266,15 +273,15 @@
         check without a version number but we want the report
         to specify the version number.
 
         Returns the check name with the version number it checked
         """
         if ":" not in check_name or ":latest" in check_name:
             check_name = ":".join(
-                (check_name.split(":")[0], self.checkers[check_name]._cc_spec_version)
+                (check_name.split(":")[0], self.checkers[check_name]._cc_spec_version),
             )
         return check_name
 
     def _get_check_url(self, check_name):
         """
         Return the check's reference URL if it exists. If not, return empty str.
         @param check_name str: name of the check being run returned by
@@ -296,15 +303,15 @@
         args = [
             (name, self.checkers[name])
             for name in checker_names
             if name in self.checkers
         ]
         valid = []
 
-        all_checked = set(a[1] for a in args)  # only class types
+        all_checked = {a[1] for a in args}  # only class types
         checker_queue = set(args)
         while len(checker_queue):
             name, a = checker_queue.pop()
             # is the current dataset type in the supported filetypes
             # for the checker class?
             if type(ds) in a().supported_ds:
                 valid.append((name, a))
@@ -337,40 +344,30 @@
             else:
                 try:
                     check_max_level = check_lookup[split_check_spec[1]]
                 except KeyError:
                     warnings.warn(
                         "Skip specifier '{}' on check '{}' not found,"
                         " defaulting to skip entire check".format(
-                            split_check_spec[1], check_name
-                        )
+                            split_check_spec[1],
+                            check_name,
+                        ),
+                        stacklevel=2,
                     )
                     check_max_level = BaseCheck.HIGH
-                else:
-                    try:
-                        check_max_level = check_lookup[split_check_spec[1]]
-                    except KeyError:
-                        warnings.warn(
-                            "Skip specifier '{}' on check '{}' not found,"
-                            " defaulting to skip entire check".format(
-                                split_check_spec[1], check_name
-                            )
-                        )
-                        check_max_level = BaseCheck.HIGH
 
-                check_dict[check_name] = check_max_level
-        else:
-            for check_name in skip_checks:
-                # always process
-                check_dict[check_name] = 0
+            check_dict[check_name] = check_max_level
 
         return check_dict
 
     def run(self, ds, skip_checks, *checker_names):
-        warnings.warn("suite.run is deprecated, use suite.run_all in calls " "instead")
+        warnings.warn(
+            "suite.run is deprecated, use suite.run_all in calls instead",
+            stacklevel=2,
+        )
         return self.run_all(ds, checker_names, skip_checks=skip_checks)
 
     def run_all(self, ds, checker_names, include_checks=None, skip_checks=None):
         """
         Runs this CheckSuite on the dataset with all the passed Checker instances.
 
         Returns a dictionary mapping checker names to a 2-tuple of their grouped scores and errors/exceptions while running checks.
@@ -387,15 +384,17 @@
         if include_checks:
             include_dict = {check_name: 0 for check_name in include_checks}
         else:
             include_dict = {}
 
         if len(checkers) == 0:
             print(
-                "No valid checkers found for tests '{}'".format(",".join(checker_names))
+                "No valid checkers found for tests '{}'".format(
+                    ",".join(checker_names),
+                ),
             )
 
         for checker_name, checker_class in checkers:
             # TODO: maybe this a little more reliable than depending on
             #       a string to determine the type of the checker -- perhaps
             #       use some kind of checker object with checker type and
             #       version baked in
@@ -521,15 +520,15 @@
         aggregates["all_priorities"] = all_priorities
         aggregates["testname"] = self._get_check_versioned_name(check_name)
         aggregates["source_name"] = source_name
         aggregates["scoreheader"] = self.checkers[check_name]._cc_display_headers
         aggregates["cc_spec_version"] = self.checkers[check_name]._cc_spec_version
         aggregates["cc_url"] = self._get_check_url(aggregates["testname"])
         aggregates["report_timestamp"] = datetime.now(timezone.utc).strftime(
-            "%Y-%m-%dT%H:%M:%SZ"
+            "%Y-%m-%dT%H:%M:%SZ",
         )
         aggregates["cc_version"] = __version__
         return aggregates
 
     def dict_output(self, check_name, groups, source_name, limit):
         """
         Builds the results into a JSON structure and writes it to the file buffer.
@@ -568,15 +567,15 @@
         @param groups          List of results from compliance checker
         @param source_name     Source of the dataset, used for title
         @param limit           Integer value for limiting output
         """
         from jinja2 import Environment, PackageLoader
 
         self.j2 = Environment(
-            loader=PackageLoader(self.templates_root, "data/templates")
+            loader=PackageLoader(self.templates_root, "data/templates"),
         )
         template = self.j2.get_template("ccheck.html.j2")
 
         template_vars = self.build_structure(check_name, groups, source_name, limit)
         return template.render(**template_vars)
 
     def html_output(self, checkers_html):
@@ -628,30 +627,32 @@
         # As a future enhancement, a string.Template string might work best here
         # but for the time being individual lines are printed and centered with
         # .center()
 
         print("\n")
         print("-" * width)
         print("IOOS Compliance Checker Report".center(width))
-        print("Version {}".format(__version__).center(width))
+        print(f"Version {__version__}".center(width))
         print(
             "Report generated {}".format(
-                datetime.now(timezone.utc).strftime("%Y-%m-%dT%H:%M:%SZ")
-            ).center(width)
+                datetime.now(timezone.utc).strftime("%Y-%m-%dT%H:%M:%SZ"),
+            ).center(width),
         )
-        print("{}".format(check_name).center(width))
-        print("{}".format(check_url).center(width))
+        print(f"{check_name}".center(width))
+        print(f"{check_url}".center(width))
         print("-" * width)
         if issue_count > 0:
             print("Corrective Actions".center(width))
             plural = "" if issue_count == 1 else "s"
             print(
                 "{} has {} potential issue{}".format(
-                    os.path.basename(ds), issue_count, plural
-                )
+                    os.path.basename(ds),
+                    issue_count,
+                    plural,
+                ),
             )
 
         return [groups, points, out_of]
 
     def standard_output_generation(self, groups, limit, points, out_of, check):
         """
         Generates the Terminal Output
@@ -690,15 +691,17 @@
             @param str check: checker name"""
 
             issue = res.name
             if not res.children:
                 reasons = res.msgs
             else:
                 child_reasons = self.reasoning_routine(
-                    res.children, check, _top_level=False
+                    res.children,
+                    check,
+                    _top_level=False,
                 )
                 # there shouldn't be messages if there are children
                 # is this a valid assumption?
                 reasons = child_reasons
 
             return issue, reasons
 
@@ -730,17 +733,17 @@
                 for issue, reasons in data_issues:
                     # if this isn't the first printed issue, add a newline
                     # separating this and the previous level
                     if has_printed:
                         print("")
                     # join alphabetized reasons together
                     reason_str = "\n".join(
-                        "* {}".format(r) for r in sorted(reasons, key=lambda x: x[0])
+                        f"* {r}" for r in sorted(reasons, key=lambda x: x[0])
                     )
-                    proc_str = "{}\n{}".format(issue, reason_str)
+                    proc_str = f"{issue}\n{reason_str}"
                     print(proc_str)
                     proc_strs.append(proc_str)
                     has_printed = True
         return "\n".join(proc_strs)
 
     def process_doc(self, doc):
         """
@@ -753,15 +756,15 @@
             # SensorObservationService does not store the etree doc root,
             # so maybe use monkey patching here for now?
             ds._root = xml_doc
 
         elif xml_doc.tag == "{http://www.opengis.net/sensorML/1.0.1}SensorML":
             ds = SensorML(xml_doc)
         else:
-            raise ValueError("Unrecognized XML root element: {}".format(xml_doc.tag))
+            raise ValueError(f"Unrecognized XML root element: {xml_doc.tag}")
         return ds
 
     def generate_dataset(self, cdl_path):
         """
         Use ncgen to generate a netCDF file from a .cdl file
         Returns the path to the generated netcdf file. If ncgen fails, uses
         sys.exit(1) to terminate program so a long stack trace is not reported
@@ -774,32 +777,34 @@
         ):  # it's possible the filename doesn't have the .cdl extension
             ds_str = cdl_path.replace(".cdl", ".nc")
         else:
             ds_str = cdl_path + ".nc"
 
         # generate netCDF-4 file
         iostat = subprocess.run(
-            ["ncgen", "-k", "nc4", "-o", ds_str, cdl_path], stderr=subprocess.PIPE
+            ["ncgen", "-k", "nc4", "-o", ds_str, cdl_path],
+            stderr=subprocess.PIPE,
         )
         if iostat.returncode != 0:
             # if not successful, create netCDF classic file
             print(
-                "netCDF-4 file could not be generated from cdl file with " + "message:"
+                "netCDF-4 file could not be generated from cdl file with " + "message:",
             )
             print(iostat.stderr.decode())
             print("Trying to create netCDF Classic file instead.")
             iostat = subprocess.run(
-                ["ncgen", "-k", "nc3", "-o", ds_str, cdl_path], stderr=subprocess.PIPE
+                ["ncgen", "-k", "nc3", "-o", ds_str, cdl_path],
+                stderr=subprocess.PIPE,
             )
             if iostat.returncode != 0:
                 # Exit program if neither a netCDF Classic nor a netCDF-4 file
                 # could be created.
                 print(
                     "netCDF Classic file could not be generated from cdl file"
-                    + "with message:"
+                    + "with message:",
                 )
                 print(iostat.stderr.decode())
                 sys.exit(1)
         return ds_str
 
     def load_dataset(self, ds_str):
         """
@@ -820,15 +825,16 @@
             return self.load_local_dataset(ds_str)
 
     def check_remote_netcdf(self, ds_str):
         if netcdf.is_remote_netcdf(ds_str):
             response = requests.get(ds_str, allow_redirects=True, timeout=60)
             try:
                 return MemoizedDataset(
-                    urlparse(response.url).path, memory=response.content
+                    urlparse(response.url).path,
+                    memory=response.content,
                 )
             except OSError:
                 # handle case when netCDF C libs weren't compiled with
                 # in-memory support by using tempfile
                 with tempnc(response.content) as _nc:
                     return MemoizedDataset(_nc)
 
@@ -850,15 +856,15 @@
         # and this is some kind of erddap tabledap form, then try to get the
         # .ncCF file from ERDDAP
         elif "tabledap" in ds_str and not url_parsed.query:
             # modify ds_str to contain the full variable request
             variables_str = opendap.create_DAP_variable_str(ds_str)
 
             # join to create a URL to an .ncCF resource
-            ds_str = "{}.ncCF?{}".format(ds_str, variables_str)
+            ds_str = f"{ds_str}.ncCF?{variables_str}"
 
         nc_remote_result = self.check_remote_netcdf(ds_str)
         if nc_remote_result:
             return nc_remote_result
 
         # if it's just an OPeNDAP endpoint, use that
         elif opendap.is_opendap(ds_str):
@@ -870,15 +876,15 @@
         # Issue GET instead if we reach here and can't get the response
         response = requests.get(ds_str, allow_redirects=True, timeout=60)
         content_type = response.headers.get("content-type")
         if content_type.split(";")[0] == "text/xml":
             return self.process_doc(response.content)
         else:
             raise ValueError(
-                "Unknown service with content-type: {}".format(content_type)
+                f"Unknown service with content-type: {content_type}",
             )
 
     def load_local_dataset(self, ds_str):
         """
         Returns a dataset instance for the local resource
 
         :param ds_str: Path to the resource
@@ -955,36 +961,39 @@
         #  (('Global Attributes', 3), <itertools._grouper at 0x7f10982b5438>),
         #  (('Not a Global Attr', 1), <itertools._grouper at 0x7f10982b5470>)]
         #  (('Some Variable', 2),     <itertools._grouper at 0x7f10982b5400>),
 
         ret_val = []
 
         for k, v in grouped:  # iterate through the grouped tuples
-
             k = k[0]  # slice ("name", weight_val) --> "name"
             v = list(v)  # from itertools._grouper to list
 
             cv = self._group_raw(list(map(trim_groups, v)), k, level + 1)
             if len(cv):
                 # if this node has children, max weight of children + sum of all the scores
                 max_weight = max([x.weight for x in cv])
                 sum_scores = tuple(map(sum, list(zip(*([x.value for x in cv])))))
                 msgs = []
 
             else:
                 max_weight = max([x.weight for x in v])
                 sum_scores = tuple(
-                    map(sum, list(zip(*([self._translate_value(x.value) for x in v]))))
+                    map(sum, list(zip(*([self._translate_value(x.value) for x in v])))),
                 )
                 msgs = sum([x.msgs for x in v], [])
 
             ret_val.append(
                 Result(
-                    name=k, weight=max_weight, value=sum_scores, children=cv, msgs=msgs
-                )
+                    name=k,
+                    weight=max_weight,
+                    value=sum_scores,
+                    children=cv,
+                    msgs=msgs,
+                ),
             )
 
         return ret_val
 
     def _translate_value(self, val):
         """
         Turns shorthand True/False/None checks into full scores (1, 1)/(0, 1)/(0, 0).
```

### Comparing `compliance-checker-5.0.2/compliance_checker/tests/__init__.py` & `compliance-checker-5.1.0/compliance_checker/tests/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -10,15 +10,18 @@
 
     def shortDescription(self):
         return None
 
     def __repr__(self):
         name = self.id()
         name = name.split(".")
-        return "%s ( %s )" % (name[-1], ".".join(name[:-2]) + ":" + ".".join(name[-2:]))
+        return "{} ( {} )".format(
+            name[-1],
+            ".".join(name[:-2]) + ":" + ".".join(name[-2:]),
+        )
 
     __str__ = __repr__
 
     def load_dataset(self, nc_dataset):
         """
         Return a loaded NC Dataset for the given path
         """
@@ -47,15 +50,18 @@
 
     def shortDescription(self):
         return None
 
     def __repr__(self):
         name = self.id()
         name = name.split(".")
-        return "%s ( %s )" % (name[-1], ".".join(name[:-2]) + ":" + ".".join(name[-2:]))
+        return "{} ( {} )".format(
+            name[-1],
+            ".".join(name[:-2]) + ":" + ".".join(name[-2:]),
+        )
 
     __str__ = __repr__
 
     def assert_result_is_good(self, result):
         if isinstance(result.value, bool):
             assert result.value is True
         else:
```

### Comparing `compliance-checker-5.0.2/compliance_checker/tests/conftest.py` & `compliance-checker-5.1.0/compliance_checker/tests/conftest.py`

 * *Files 1% similar despite different names*

```diff
@@ -88,25 +88,25 @@
 @pytest.fixture
 def new_nc_file(tmpdir):
     """
     Make a new temporary netCDF file for the scope of the test
     """
     nc_file_path = os.path.join(tmpdir, "example.nc")
     if os.path.exists(nc_file_path):
-        raise IOError("File Exists: %s" % nc_file_path)
+        raise OSError("File Exists: %s" % nc_file_path)
     nc = Dataset(nc_file_path, "w")
     # no need for cleanup, built-in tmpdir fixture will handle it
     return nc
 
 
 @pytest.fixture
 def tmp_txt_file(tmpdir):
     file_path = os.path.join(tmpdir, "output.txt")
     if os.path.exists(file_path):
-        raise IOError("File Exists: %s" % file_path)
+        raise OSError("File Exists: %s" % file_path)
 
     return file_path
 
 
 @pytest.fixture
 def checksuite_setup():
     """For test_cli"""
```

### Comparing `compliance-checker-5.0.2/compliance_checker/tests/data/20160919092000-ABOM-L3S_GHRSST-SSTfnd-AVHRR_D-1d_dn_truncate.cdl` & `compliance-checker-5.1.0/compliance_checker/tests/data/20160919092000-ABOM-L3S_GHRSST-SSTfnd-AVHRR_D-1d_dn_truncate.cdl`

 * *Files identical despite different names*

### Comparing `compliance-checker-5.0.2/compliance_checker/tests/data/2d-regular-grid.cdl` & `compliance-checker-5.1.0/compliance_checker/tests/data/2d-regular-grid.cdl`

 * *Files identical despite different names*

### Comparing `compliance-checker-5.0.2/compliance_checker/tests/data/2dim-grid.cdl` & `compliance-checker-5.1.0/compliance_checker/tests/data/2dim-grid.cdl`

 * *Files identical despite different names*

### Comparing `compliance-checker-5.0.2/compliance_checker/tests/data/3d-regular-grid.cdl` & `compliance-checker-5.1.0/compliance_checker/tests/data/3d-regular-grid.cdl`

 * *Files identical despite different names*

### Comparing `compliance-checker-5.0.2/compliance_checker/tests/data/3d-static-grid.cdl` & `compliance-checker-5.1.0/compliance_checker/tests/data/3d-static-grid.cdl`

 * *Files identical despite different names*

### Comparing `compliance-checker-5.0.2/compliance_checker/tests/data/NCEI_profile_template_v2.0_2016-09-22_181835.151325.cdl` & `compliance-checker-5.1.0/compliance_checker/tests/data/NCEI_profile_template_v2.0_2016-09-22_181835.151325.cdl`

 * *Files identical despite different names*

### Comparing `compliance-checker-5.0.2/compliance_checker/tests/data/appendix_h/point.cdl` & `compliance-checker-5.1.0/compliance_checker/tests/data/appendix_h/point.cdl`

 * *Files identical despite different names*

### Comparing `compliance-checker-5.0.2/compliance_checker/tests/data/appendix_h/timeseries-incomplete.cdl` & `compliance-checker-5.1.0/compliance_checker/tests/data/appendix_h/timeseries-incomplete.cdl`

 * *Files identical despite different names*

### Comparing `compliance-checker-5.0.2/compliance_checker/tests/data/appendix_h/timeseries-non-static.cdl` & `compliance-checker-5.1.0/compliance_checker/tests/data/appendix_h/timeseries-non-static.cdl`

 * *Files identical despite different names*

### Comparing `compliance-checker-5.0.2/compliance_checker/tests/data/appendix_h/timeseries-orthogonal.cdl` & `compliance-checker-5.1.0/compliance_checker/tests/data/appendix_h/timeseries-orthogonal.cdl`

 * *Files identical despite different names*

### Comparing `compliance-checker-5.0.2/compliance_checker/tests/data/appendix_h/timeseries-single.cdl` & `compliance-checker-5.1.0/compliance_checker/tests/data/appendix_h/timeseries-single.cdl`

 * *Files identical despite different names*

### Comparing `compliance-checker-5.0.2/compliance_checker/tests/data/bad-instance.cdl` & `compliance-checker-5.1.0/compliance_checker/tests/data/bad-instance.cdl`

 * *Files identical despite different names*

### Comparing `compliance-checker-5.0.2/compliance_checker/tests/data/bad-instance.nc` & `compliance-checker-5.1.0/compliance_checker/tests/data/bad-instance.nc`

 * *Files identical despite different names*

### Comparing `compliance-checker-5.0.2/compliance_checker/tests/data/bad-trajectory.cdl` & `compliance-checker-5.1.0/compliance_checker/tests/data/bad-trajectory.cdl`

 * *Files identical despite different names*

### Comparing `compliance-checker-5.0.2/compliance_checker/tests/data/bad-trajectory.nc` & `compliance-checker-5.1.0/compliance_checker/tests/data/bad-trajectory.nc`

 * *Files identical despite different names*

### Comparing `compliance-checker-5.0.2/compliance_checker/tests/data/bad_cell_measure1.cdl` & `compliance-checker-5.1.0/compliance_checker/tests/data/bad_cell_measure1.cdl`

 * *Files identical despite different names*

### Comparing `compliance-checker-5.0.2/compliance_checker/tests/data/bad_cell_measure1.nc` & `compliance-checker-5.1.0/compliance_checker/tests/data/bad_cell_measure1.nc`

 * *Files identical despite different names*

### Comparing `compliance-checker-5.0.2/compliance_checker/tests/data/bad_cell_measure2.cdl` & `compliance-checker-5.1.0/compliance_checker/tests/data/bad_cell_measure2.cdl`

 * *Files identical despite different names*

### Comparing `compliance-checker-5.0.2/compliance_checker/tests/data/bad_cell_measure2.nc` & `compliance-checker-5.1.0/compliance_checker/tests/data/bad_cell_measure2.nc`

 * *Files identical despite different names*

### Comparing `compliance-checker-5.0.2/compliance_checker/tests/data/bad_cf_role.cdl` & `compliance-checker-5.1.0/compliance_checker/tests/data/bad_cf_role.cdl`

 * *Files identical despite different names*

### Comparing `compliance-checker-5.0.2/compliance_checker/tests/data/bad_cf_role.nc` & `compliance-checker-5.1.0/compliance_checker/tests/data/bad_cf_role.nc`

 * *Files identical despite different names*

### Comparing `compliance-checker-5.0.2/compliance_checker/tests/data/bad_data_type.cdl` & `compliance-checker-5.1.0/compliance_checker/tests/data/bad_data_type.cdl`

 * *Files identical despite different names*

### Comparing `compliance-checker-5.0.2/compliance_checker/tests/data/bad_data_type.nc` & `compliance-checker-5.1.0/compliance_checker/tests/data/bad_data_type.nc`

 * *Files identical despite different names*

### Comparing `compliance-checker-5.0.2/compliance_checker/tests/data/bad_missing_data.cdl` & `compliance-checker-5.1.0/compliance_checker/tests/data/bad_missing_data.cdl`

 * *Files identical despite different names*

### Comparing `compliance-checker-5.0.2/compliance_checker/tests/data/bad_missing_data.nc` & `compliance-checker-5.1.0/compliance_checker/tests/data/bad_missing_data.nc`

 * *Files identical despite different names*

### Comparing `compliance-checker-5.0.2/compliance_checker/tests/data/bad_region.cdl` & `compliance-checker-5.1.0/compliance_checker/tests/data/bad_region.cdl`

 * *Files identical despite different names*

### Comparing `compliance-checker-5.0.2/compliance_checker/tests/data/bad_region.nc` & `compliance-checker-5.1.0/compliance_checker/tests/data/bad_region.nc`

 * *Files identical despite different names*

### Comparing `compliance-checker-5.0.2/compliance_checker/tests/data/bad_units.cdl` & `compliance-checker-5.1.0/compliance_checker/tests/data/bad_units.cdl`

 * *Files identical despite different names*

### Comparing `compliance-checker-5.0.2/compliance_checker/tests/data/bad_units.nc` & `compliance-checker-5.1.0/compliance_checker/tests/data/bad_units.nc`

 * *Files identical despite different names*

### Comparing `compliance-checker-5.0.2/compliance_checker/tests/data/cell_measure.cdl` & `compliance-checker-5.1.0/compliance_checker/tests/data/cell_measure.cdl`

 * *Files identical despite different names*

### Comparing `compliance-checker-5.0.2/compliance_checker/tests/data/cf_example_cell_measures.cdl` & `compliance-checker-5.1.0/compliance_checker/tests/data/cf_example_cell_measures.cdl`

 * *Files identical despite different names*

### Comparing `compliance-checker-5.0.2/compliance_checker/tests/data/chap2.cdl` & `compliance-checker-5.1.0/compliance_checker/tests/data/chap2.cdl`

 * *Files identical despite different names*

### Comparing `compliance-checker-5.0.2/compliance_checker/tests/data/climatology.cdl` & `compliance-checker-5.1.0/compliance_checker/tests/data/climatology.cdl`

 * *Files identical despite different names*

### Comparing `compliance-checker-5.0.2/compliance_checker/tests/data/cont_ragged.cdl` & `compliance-checker-5.1.0/compliance_checker/tests/data/cont_ragged.cdl`

 * *Files identical despite different names*

### Comparing `compliance-checker-5.0.2/compliance_checker/tests/data/coordinate_types.cdl` & `compliance-checker-5.1.0/compliance_checker/tests/data/coordinate_types.cdl`

 * *Files identical despite different names*

### Comparing `compliance-checker-5.0.2/compliance_checker/tests/data/dimension_order.cdl` & `compliance-checker-5.1.0/compliance_checker/tests/data/dimension_order.cdl`

 * *Files identical despite different names*

### Comparing `compliance-checker-5.0.2/compliance_checker/tests/data/duplicate_axis.cdl` & `compliance-checker-5.1.0/compliance_checker/tests/data/duplicate_axis.cdl`

 * *Files identical despite different names*

### Comparing `compliance-checker-5.0.2/compliance_checker/tests/data/example-grid.cdl` & `compliance-checker-5.1.0/compliance_checker/tests/data/example-grid.cdl`

 * *Files identical despite different names*

### Comparing `compliance-checker-5.0.2/compliance_checker/tests/data/examples/3mf07.cdl` & `compliance-checker-5.1.0/compliance_checker/tests/data/examples/3mf07.cdl`

 * *Files identical despite different names*

### Comparing `compliance-checker-5.0.2/compliance_checker/tests/data/examples/bio_taxa.cdl` & `compliance-checker-5.1.0/compliance_checker/tests/data/examples/bio_taxa.cdl`

 * *Files identical despite different names*

### Comparing `compliance-checker-5.0.2/compliance_checker/tests/data/examples/cf_example_cell_measures.cdl` & `compliance-checker-5.1.0/compliance_checker/tests/data/examples/cf_example_cell_measures.cdl`

 * *Files identical despite different names*

### Comparing `compliance-checker-5.0.2/compliance_checker/tests/data/examples/fvcom.cdl` & `compliance-checker-5.1.0/compliance_checker/tests/data/examples/fvcom.cdl`

 * *Files identical despite different names*

### Comparing `compliance-checker-5.0.2/compliance_checker/tests/data/examples/glcfs.cdl` & `compliance-checker-5.1.0/compliance_checker/tests/data/examples/glcfs.cdl`

 * *Files identical despite different names*

### Comparing `compliance-checker-5.0.2/compliance_checker/tests/data/examples/hycom_global.cdl` & `compliance-checker-5.1.0/compliance_checker/tests/data/examples/hycom_global.cdl`

 * *Files identical despite different names*

### Comparing `compliance-checker-5.0.2/compliance_checker/tests/data/examples/kibesillah.cdl` & `compliance-checker-5.1.0/compliance_checker/tests/data/examples/kibesillah.cdl`

 * *Files identical despite different names*

### Comparing `compliance-checker-5.0.2/compliance_checker/tests/data/examples/l01-met.cdl` & `compliance-checker-5.1.0/compliance_checker/tests/data/examples/l01-met.cdl`

 * *Files identical despite different names*

### Comparing `compliance-checker-5.0.2/compliance_checker/tests/data/examples/ocos.cdl` & `compliance-checker-5.1.0/compliance_checker/tests/data/examples/ocos.cdl`

 * *Files identical despite different names*

### Comparing `compliance-checker-5.0.2/compliance_checker/tests/data/examples/ooi_glider.cdl` & `compliance-checker-5.1.0/compliance_checker/tests/data/examples/ooi_glider.cdl`

 * *Files identical despite different names*

### Comparing `compliance-checker-5.0.2/compliance_checker/tests/data/examples/pr_inundation.cdl` & `compliance-checker-5.1.0/compliance_checker/tests/data/examples/pr_inundation.cdl`

 * *Files identical despite different names*

### Comparing `compliance-checker-5.0.2/compliance_checker/tests/data/examples/sldmb_43093_agg.cdl` & `compliance-checker-5.1.0/compliance_checker/tests/data/examples/sldmb_43093_agg.cdl`

 * *Files identical despite different names*

### Comparing `compliance-checker-5.0.2/compliance_checker/tests/data/examples/sp041.cdl` & `compliance-checker-5.1.0/compliance_checker/tests/data/examples/sp041.cdl`

 * *Files identical despite different names*

### Comparing `compliance-checker-5.0.2/compliance_checker/tests/data/examples/swan.cdl` & `compliance-checker-5.1.0/compliance_checker/tests/data/examples/swan.cdl`

 * *Files identical despite different names*

### Comparing `compliance-checker-5.0.2/compliance_checker/tests/data/examples/usgs_dem_saipan.cdl` & `compliance-checker-5.1.0/compliance_checker/tests/data/examples/usgs_dem_saipan.cdl`

 * *Files identical despite different names*

### Comparing `compliance-checker-5.0.2/compliance_checker/tests/data/examples/ww3.cdl` & `compliance-checker-5.1.0/compliance_checker/tests/data/examples/ww3.cdl`

 * *Files identical despite different names*

### Comparing `compliance-checker-5.0.2/compliance_checker/tests/data/forecast_reference.cdl` & `compliance-checker-5.1.0/compliance_checker/tests/data/forecast_reference.cdl`

 * *Files identical despite different names*

### Comparing `compliance-checker-5.0.2/compliance_checker/tests/data/grid-boundaries.cdl` & `compliance-checker-5.1.0/compliance_checker/tests/data/grid-boundaries.cdl`

 * *Files identical despite different names*

### Comparing `compliance-checker-5.0.2/compliance_checker/tests/data/grid_mapping_coordinates.cdl` & `compliance-checker-5.1.0/compliance_checker/tests/data/grid_mapping_coordinates.cdl`

 * *Files identical despite different names*

### Comparing `compliance-checker-5.0.2/compliance_checker/tests/data/http_mocks/ncsos_describesensor.xml` & `compliance-checker-5.1.0/compliance_checker/tests/data/http_mocks/ncsos_describesensor.xml`

 * *Files identical despite different names*

### Comparing `compliance-checker-5.0.2/compliance_checker/tests/data/http_mocks/ncsos_getcapabilities.xml` & `compliance-checker-5.1.0/compliance_checker/tests/data/http_mocks/ncsos_getcapabilities.xml`

 * *Files identical despite different names*

### Comparing `compliance-checker-5.0.2/compliance_checker/tests/data/illegal-aux-coords.cdl` & `compliance-checker-5.1.0/compliance_checker/tests/data/illegal-aux-coords.cdl`

 * *Files identical despite different names*

### Comparing `compliance-checker-5.0.2/compliance_checker/tests/data/index_ragged.cdl` & `compliance-checker-5.1.0/compliance_checker/tests/data/index_ragged.cdl`

 * *Files identical despite different names*

### Comparing `compliance-checker-5.0.2/compliance_checker/tests/data/index_ragged2.cdl` & `compliance-checker-5.1.0/compliance_checker/tests/data/index_ragged2.cdl`

 * *Files identical despite different names*

### Comparing `compliance-checker-5.0.2/compliance_checker/tests/data/ioos_1_1.cdl` & `compliance-checker-5.1.0/compliance_checker/tests/data/ioos_1_1.cdl`

 * *Files identical despite different names*

### Comparing `compliance-checker-5.0.2/compliance_checker/tests/data/line_geometry.cdl` & `compliance-checker-5.1.0/compliance_checker/tests/data/line_geometry.cdl`

 * *Files identical despite different names*

### Comparing `compliance-checker-5.0.2/compliance_checker/tests/data/mapping.cdl` & `compliance-checker-5.1.0/compliance_checker/tests/data/mapping.cdl`

 * *Files identical despite different names*

### Comparing `compliance-checker-5.0.2/compliance_checker/tests/data/multi-dim-coordinates.cdl` & `compliance-checker-5.1.0/compliance_checker/tests/data/multi-dim-coordinates.cdl`

 * *Files identical despite different names*

### Comparing `compliance-checker-5.0.2/compliance_checker/tests/data/multi-timeseries-incomplete.cdl` & `compliance-checker-5.1.0/compliance_checker/tests/data/multi-timeseries-incomplete.cdl`

 * *Files identical despite different names*

### Comparing `compliance-checker-5.0.2/compliance_checker/tests/data/multi-timeseries-orthogonal.cdl` & `compliance-checker-5.1.0/compliance_checker/tests/data/multi-timeseries-orthogonal.cdl`

 * *Files identical despite different names*

### Comparing `compliance-checker-5.0.2/compliance_checker/tests/data/ncei_gold_point_1.cdl` & `compliance-checker-5.1.0/compliance_checker/tests/data/ncei_gold_point_1.cdl`

 * *Files identical despite different names*

### Comparing `compliance-checker-5.0.2/compliance_checker/tests/data/ncei_gold_point_2.cdl` & `compliance-checker-5.1.0/compliance_checker/tests/data/ncei_gold_point_2.cdl`

 * *Files identical despite different names*

### Comparing `compliance-checker-5.0.2/compliance_checker/tests/data/non-comp/1d_bound_bad.cdl` & `compliance-checker-5.1.0/compliance_checker/tests/data/non-comp/1d_bound_bad.cdl`

 * *Files identical despite different names*

### Comparing `compliance-checker-5.0.2/compliance_checker/tests/data/non-comp/bad-rhgrid.cdl` & `compliance-checker-5.1.0/compliance_checker/tests/data/non-comp/bad-rhgrid.cdl`

 * *Files identical despite different names*

### Comparing `compliance-checker-5.0.2/compliance_checker/tests/data/non-comp/bad.cdl` & `compliance-checker-5.1.0/compliance_checker/tests/data/non-comp/bad.cdl`

 * *Files identical despite different names*

### Comparing `compliance-checker-5.0.2/compliance_checker/tests/data/non-comp/bad2dim.cdl` & `compliance-checker-5.1.0/compliance_checker/tests/data/non-comp/bad2dim.cdl`

 * *Files identical despite different names*

### Comparing `compliance-checker-5.0.2/compliance_checker/tests/data/non-comp/bounds_bad_num_coords.cdl` & `compliance-checker-5.1.0/compliance_checker/tests/data/non-comp/bounds_bad_num_coords.cdl`

 * *Files identical despite different names*

### Comparing `compliance-checker-5.0.2/compliance_checker/tests/data/non-comp/bounds_bad_order.cdl` & `compliance-checker-5.1.0/compliance_checker/tests/data/non-comp/bounds_bad_order.cdl`

 * *Files identical despite different names*

### Comparing `compliance-checker-5.0.2/compliance_checker/tests/data/non-comp/self_referencing.cdl` & `compliance-checker-5.1.0/compliance_checker/tests/data/non-comp/self_referencing.cdl`

 * *Files identical despite different names*

### Comparing `compliance-checker-5.0.2/compliance_checker/tests/data/point.cdl` & `compliance-checker-5.1.0/compliance_checker/tests/data/point.cdl`

 * *Files identical despite different names*

### Comparing `compliance-checker-5.0.2/compliance_checker/tests/data/polygon_geometry.cdl` & `compliance-checker-5.1.0/compliance_checker/tests/data/polygon_geometry.cdl`

 * *Files identical despite different names*

### Comparing `compliance-checker-5.0.2/compliance_checker/tests/data/profile-incomplete.cdl` & `compliance-checker-5.1.0/compliance_checker/tests/data/profile-incomplete.cdl`

 * *Files identical despite different names*

### Comparing `compliance-checker-5.0.2/compliance_checker/tests/data/profile-orthogonal.cdl` & `compliance-checker-5.1.0/compliance_checker/tests/data/profile-orthogonal.cdl`

 * *Files identical despite different names*

### Comparing `compliance-checker-5.0.2/compliance_checker/tests/data/reduced_horizontal_grid.cdl` & `compliance-checker-5.1.0/compliance_checker/tests/data/reduced_horizontal_grid.cdl`

 * *Files identical despite different names*

### Comparing `compliance-checker-5.0.2/compliance_checker/tests/data/rotated_pole_grid.cdl` & `compliance-checker-5.1.0/compliance_checker/tests/data/rotated_pole_grid.cdl`

 * *Files identical despite different names*

### Comparing `compliance-checker-5.0.2/compliance_checker/tests/data/ru07-20130824T170228_rt0.cdl` & `compliance-checker-5.1.0/compliance_checker/tests/data/ru07-20130824T170228_rt0.cdl`

 * *Files identical despite different names*

### Comparing `compliance-checker-5.0.2/compliance_checker/tests/data/self-referencing-var.cdl` & `compliance-checker-5.1.0/compliance_checker/tests/data/self-referencing-var.cdl`

 * *Files identical despite different names*

### Comparing `compliance-checker-5.0.2/compliance_checker/tests/data/taxonomy_example.cdl` & `compliance-checker-5.1.0/compliance_checker/tests/data/taxonomy_example.cdl`

 * *Files identical despite different names*

### Comparing `compliance-checker-5.0.2/compliance_checker/tests/data/test_cdl.cdl` & `compliance-checker-5.1.0/compliance_checker/tests/data/test_cdl.cdl`

 * *Files identical despite different names*

### Comparing `compliance-checker-5.0.2/compliance_checker/tests/data/test_cdl_nc4_file.cdl` & `compliance-checker-5.1.0/compliance_checker/tests/data/test_cdl_nc4_file.cdl`

 * *Files identical despite different names*

### Comparing `compliance-checker-5.0.2/compliance_checker/tests/data/test_cdl_nc_file.cdl` & `compliance-checker-5.1.0/compliance_checker/tests/data/test_cdl_nc_file.cdl`

 * *Files identical despite different names*

### Comparing `compliance-checker-5.0.2/compliance_checker/tests/data/test_cdl_nc_file.nc` & `compliance-checker-5.1.0/compliance_checker/tests/data/test_cdl_nc_file.nc`

 * *Files identical despite different names*

### Comparing `compliance-checker-5.0.2/compliance_checker/tests/data/timeseries-profile-incomplete.cdl` & `compliance-checker-5.1.0/compliance_checker/tests/data/timeseries-profile-incomplete.cdl`

 * *Files identical despite different names*

### Comparing `compliance-checker-5.0.2/compliance_checker/tests/data/timeseries-profile-multi-ortho-time.cdl` & `compliance-checker-5.1.0/compliance_checker/tests/data/timeseries-profile-multi-ortho-time.cdl`

 * *Files identical despite different names*

### Comparing `compliance-checker-5.0.2/compliance_checker/tests/data/timeseries-profile-multi-station.cdl` & `compliance-checker-5.1.0/compliance_checker/tests/data/timeseries-profile-multi-station.cdl`

 * *Files identical despite different names*

### Comparing `compliance-checker-5.0.2/compliance_checker/tests/data/timeseries-profile-ortho-depth.cdl` & `compliance-checker-5.1.0/compliance_checker/tests/data/timeseries-profile-ortho-depth.cdl`

 * *Files identical despite different names*

### Comparing `compliance-checker-5.0.2/compliance_checker/tests/data/timeseries-profile-single-ortho-time.cdl` & `compliance-checker-5.1.0/compliance_checker/tests/data/timeseries-profile-single-ortho-time.cdl`

 * *Files identical despite different names*

### Comparing `compliance-checker-5.0.2/compliance_checker/tests/data/timeseries-profile-single-station.cdl` & `compliance-checker-5.1.0/compliance_checker/tests/data/timeseries-profile-single-station.cdl`

 * *Files identical despite different names*

### Comparing `compliance-checker-5.0.2/compliance_checker/tests/data/timeseries.cdl` & `compliance-checker-5.1.0/compliance_checker/tests/data/timeseries.cdl`

 * *Files identical despite different names*

### Comparing `compliance-checker-5.0.2/compliance_checker/tests/data/trajectory-complete.cdl` & `compliance-checker-5.1.0/compliance_checker/tests/data/trajectory-complete.cdl`

 * *Files identical despite different names*

### Comparing `compliance-checker-5.0.2/compliance_checker/tests/data/trajectory-implied.cdl` & `compliance-checker-5.1.0/compliance_checker/tests/data/trajectory-implied.cdl`

 * *Files identical despite different names*

### Comparing `compliance-checker-5.0.2/compliance_checker/tests/data/trajectory-profile-incomplete.cdl` & `compliance-checker-5.1.0/compliance_checker/tests/data/trajectory-profile-incomplete.cdl`

 * *Files identical despite different names*

### Comparing `compliance-checker-5.0.2/compliance_checker/tests/data/trajectory-profile-orthogonal.cdl` & `compliance-checker-5.1.0/compliance_checker/tests/data/trajectory-profile-orthogonal.cdl`

 * *Files identical despite different names*

### Comparing `compliance-checker-5.0.2/compliance_checker/tests/data/trajectory-single.cdl` & `compliance-checker-5.1.0/compliance_checker/tests/data/trajectory-single.cdl`

 * *Files identical despite different names*

### Comparing `compliance-checker-5.0.2/compliance_checker/tests/data/trajectory.cdl` & `compliance-checker-5.1.0/compliance_checker/tests/data/trajectory.cdl`

 * *Files identical despite different names*

### Comparing `compliance-checker-5.0.2/compliance_checker/tests/data/units_check.cdl` & `compliance-checker-5.1.0/compliance_checker/tests/data/units_check.cdl`

 * *Files identical despite different names*

### Comparing `compliance-checker-5.0.2/compliance_checker/tests/data/valid_coordinates.cdl` & `compliance-checker-5.1.0/compliance_checker/tests/data/valid_coordinates.cdl`

 * *Files identical despite different names*

### Comparing `compliance-checker-5.0.2/compliance_checker/tests/data/vertical_coords.cdl` & `compliance-checker-5.1.0/compliance_checker/tests/data/vertical_coords.cdl`

 * *Files identical despite different names*

### Comparing `compliance-checker-5.0.2/compliance_checker/tests/helpers.py` & `compliance-checker-5.1.0/compliance_checker/tests/helpers.py`

 * *Files 22% similar despite different names*

```diff
@@ -12,53 +12,53 @@
         # taken from test/tst_diskless.py NetCDF library
         # even though we aren't persisting data to disk, the constructor
         # requires a filename not currently in use by another Dataset object..
         if filename is None:
             temp_filename = tempfile.NamedTemporaryFile(suffix=".nc", delete=True).name
         else:
             temp_filename = filename
-        super(MockNetCDF, self).__init__(
-            temp_filename, "w", diskless=True, persist=False
+        super().__init__(
+            temp_filename,
+            "w",
+            diskless=True,
+            persist=False,
         )
 
 
 class MockTimeSeries(MockNetCDF):
     """
     Mock time series with time dimension and time, lon, lat, and depth
     variables defined
     """
 
     def __init__(self, filename=None, default_fill_value=None):
-        super(MockTimeSeries, self).__init__(filename)
+        super().__init__(filename)
         self.createDimension("time", 500)
-        for name, std_name, units in (
-            ("time", "time", "seconds since 1970-01-01"),
-            ("lon", "longitude", "degrees_east"),
-            ("lat", "latitude", "degrees_north"),
-            ("depth", "depth", "m"),
+        for name, std_name, units, axis in (
+            ("time", "time", "seconds since 1970-01-01 00:00:00", "T"),
+            ("lon", "longitude", "degrees_east", "X"),
+            ("lat", "latitude", "degrees_north", "Y"),
+            ("depth", "depth", "m", "Z"),
         ):
             var = self.createVariable(
-                name, "d", ("time",), fill_value=default_fill_value
+                name,
+                "d",
+                ("time",),
+                fill_value=default_fill_value,
             )
             var.standard_name = std_name
             var.units = units
+            var.axis = axis
 
         # give some applicable units
-        self.variables["time"].units = "seconds since 2019-04-11T00:00:00"
-        self.variables["time"].axis = "T"
-        self.variables["lat"].units = "degree_north"
-        self.variables["lat"].axis = "Y"
-        self.variables["lon"].units = "degree_east"
-        self.variables["lon"].axis = "X"
-        self.variables["depth"].units = "meters"
-        self.variables["depth"].axis = "Z"
+        self.variables["time"].calendar = "standard"
         self.variables["depth"].positive = "down"
 
 
-class MockVariable(object):
+class MockVariable:
     """
     For mocking a dataset variable. Constructor optionally takes a NetCDF
     variable, the NetCDF attributes of which will be copied over to this
     object.
     """
 
     def __init__(self, copy_var=None):
@@ -122,15 +122,15 @@
         profile, timeseries, trajectory,
         timeseriesprofile, trajectoryprofile)
 
     structure: str (contiguous|indexed)
     """
 
     def __init__(self, feature_type: str, structure="contiguous"):
-        super(MockRaggedArrayRepr, self).__init__()
+        super().__init__()
 
         if structure.lower() not in ("contiguous", "indexed"):
             raise ValueError("Must initialize MockRaggedArray as contiguous or indexed")
 
         if feature_type.lower() not in {
             "point",
             "profile",
@@ -157,86 +157,96 @@
             # become the "station dimension"
             self.createDimension("STATION_DIMENSION", 5)
 
             # one variable for "timeseries" or "trajectory" which
             # has the station dimension and cf_role
             _var_name = feature_type.lower().split("profile")[0]
             self.createVariable(
-                "{}_id_variable".format(_var_name),
+                f"{_var_name}_id_variable",
                 str,
                 ("STATION_DIMENSION",),
                 fill_value=None,
             )
 
             # set the cf_role
-            self.variables["{}_id_variable".format(_var_name)].setncattr(
-                "cf_role", "{}_id".format(_var_name)
+            self.variables[f"{_var_name}_id_variable"].setncattr(
+                "cf_role",
+                f"{_var_name}_id",
             )
 
             # there will be one for the profile
             self.createVariable(
-                "profile_id_variable", str, ("INSTANCE_DIMENSION",), fill_value=None
+                "profile_id_variable",
+                str,
+                ("INSTANCE_DIMENSION",),
+                fill_value=None,
             )
             self.variables["profile_id_variable"].setncattr("cf_role", "profile_id")
 
             # will need a station index variable
             self.createVariable(
-                "station_index_variable", int, ("INSTANCE_DIMENSION",), fill_value=None
+                "station_index_variable",
+                int,
+                ("INSTANCE_DIMENSION",),
+                fill_value=None,
             )
 
             self.variables["station_index_variable"].setncattr(
-                "instance_dimension", "STATION_DIMENSION"
+                "instance_dimension",
+                "STATION_DIMENSION",
             )
 
             # also need counter variable, as compound featureTypes
             # are represented by having a contiguous repr for the
             # profiles and the indexed repr for the timeseries/trajectory
             # organization
             self.createVariable(
                 "counter_var",
                 "i",  # integer type
                 ("INSTANCE_DIMENSION",),
                 fill_value=None,
             )
 
             self.variables["counter_var"].setncattr(
-                "sample_dimension", "SAMPLE_DIMENSION"
+                "sample_dimension",
+                "SAMPLE_DIMENSION",
             )
 
         else:  # just a single featureType
             self.createVariable(
-                "{}_id_variable".format(feature_type),
+                f"{feature_type}_id_variable",
                 str,
                 ("INSTANCE_DIMENSION",),
                 fill_value=None,
             )
 
-            self.variables["{}_id_variable".format(feature_type)].setncattr(
-                "cf_role", "{}_id".format(feature_type)
+            self.variables[f"{feature_type}_id_variable"].setncattr(
+                "cf_role",
+                f"{feature_type}_id",
             )
 
             if structure == "contiguous":
-
                 # create count variable
                 self.createVariable(
                     "counter_var",
                     "i",  # integer type
                     ("INSTANCE_DIMENSION",),
                     fill_value=None,
                 )
 
                 self.variables["counter_var"].setncattr(
-                    "sample_dimension", "SAMPLE_DIMENSION"
+                    "sample_dimension",
+                    "SAMPLE_DIMENSION",
                 )
 
             else:
-
                 # create index variable
                 self.createVariable(
                     "index_var",
                     "i",  # integer type
                     ("SAMPLE_DIMENSION",),
                     fill_value=None,
                 )
                 self.variables["index_var"].setncattr(
-                    "instance_dimension", "INSTANCE_DIMENSION"
+                    "instance_dimension",
+                    "INSTANCE_DIMENSION",
                 )
```

### Comparing `compliance-checker-5.0.2/compliance_checker/tests/resources.py` & `compliance-checker-5.1.0/compliance_checker/tests/resources.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,19 +33,19 @@
     "bad_missing_data": get_filename("tests/data/bad_missing_data.cdl"),
     "bad_reference": get_filename("tests/data/bad_reference.cdl"),
     "bad_region": get_filename("tests/data/bad_region.cdl"),
     "bad_units": get_filename("tests/data/bad_units.cdl"),
     "bad2dim": get_filename("tests/data/non-comp/bad2dim.cdl"),
     "bounds_bad_order": get_filename("tests/data/non-comp/bounds_bad_order.cdl"),
     "bounds_bad_num_coords": get_filename(
-        "tests/data/non-comp/bounds_bad_num_coords.cdl"
+        "tests/data/non-comp/bounds_bad_num_coords.cdl",
     ),
     "cell_measure": get_filename("tests/data/cell_measure.cdl"),
     "cf_example_cell_measures": get_filename(
-        "tests/data/examples/cf_example_cell_measures.cdl"
+        "tests/data/examples/cf_example_cell_measures.cdl",
     ),
     "chap2": get_filename("tests/data/chap2.cdl"),
     "climatology": get_filename("tests/data/climatology.cdl"),
     "cont_ragged": get_filename("tests/data/cont_ragged.cdl"),
     "conv_multi": get_filename("tests/data/conv_multi.cdl"),
     "conv_bad": get_filename("tests/data/conv_bad.cdl"),
     "coordinates_and_metadata": get_filename("tests/data/coordinates_and_metadata.cdl"),
@@ -54,98 +54,98 @@
     "duplicate_axis": get_filename("tests/data/duplicate_axis.cdl"),
     "dimension_order": get_filename("tests/data/dimension_order.cdl"),
     "example-grid": get_filename("tests/data/example-grid.cdl"),
     "featureType": get_filename("tests/data/example-grid.cdl"),
     "forecast_reference": get_filename("tests/data/forecast_reference.cdl"),
     "fvcom": get_filename("tests/data/examples/fvcom.cdl"),
     "ghrsst": get_filename(
-        "tests/data/20160919092000-ABOM-L3S_GHRSST-SSTfnd-AVHRR_D-1d_dn_truncate.cdl"
+        "tests/data/20160919092000-ABOM-L3S_GHRSST-SSTfnd-AVHRR_D-1d_dn_truncate.cdl",
     ),
     "glcfs": get_filename("tests/data/examples/glcfs.cdl"),
     "grid-boundaries": get_filename("tests/data/grid-boundaries.cdl"),
     "grid_mapping_coordinates": get_filename("tests/data/grid_mapping_coordinates.cdl"),
     "hycom_global": get_filename("tests/data/examples/hycom_global.cdl"),
     "h_point": get_filename("tests/data/appendix_h/point.cdl"),
     "h_timeseries-incomplete": get_filename(
-        "tests/data/appendix_h/timeseries-incomplete.cdl"
+        "tests/data/appendix_h/timeseries-incomplete.cdl",
     ),
     "h_timeseries-orthogonal": get_filename(
-        "tests/data/appendix_h/timeseries-orthogonal.cdl"
+        "tests/data/appendix_h/timeseries-orthogonal.cdl",
     ),
     "h_timeseries-single": get_filename("tests/data/appendix_h/timeseries-single.cdl"),
     "illegal-vertical": get_filename("tests/data/illegal-vertical.cdl"),
     "illegal-aux-coords": get_filename("tests/data/illegal-aux-coords.cdl"),
     "index_ragged": get_filename("tests/data/index_ragged.cdl"),
     "index_ragged2": get_filename("tests/data/index_ragged2.cdl"),
     "ints64": get_filename("tests/data/ints64.cdl"),
     "ioos_gold_1_1": get_filename("tests/data/ioos_1_1.cdl"),
     "kibesillah": get_filename("tests/data/examples/kibesillah.cdl"),
     "l01-met": get_filename("tests/data/examples/l01-met.cdl"),
     "line_geometry": get_filename("tests/data/line_geometry.cdl"),
     "mapping": get_filename("tests/data/mapping.cdl"),
     "multi-dim-coordinates": get_filename("tests/data/multi-dim-coordinates.cdl"),
     "multi-timeseries-orthogonal": get_filename(
-        "tests/data/multi-timeseries-orthogonal.cdl"
+        "tests/data/multi-timeseries-orthogonal.cdl",
     ),
     "multi-timeseries-incomplete": get_filename(
-        "tests/data/multi-timeseries-incomplete.cdl"
+        "tests/data/multi-timeseries-incomplete.cdl",
     ),
     "ncei_gold_point_1": get_filename("tests/data/ncei_gold_point_1.cdl"),
     "ncei_gold_point_2": get_filename("tests/data/ncei_gold_point_2.cdl"),
     "NCEI_profile_template_v2_0": get_filename(
-        "tests/data/NCEI_profile_template_v2.0_2016-09-22_181835.151325.cdl"
+        "tests/data/NCEI_profile_template_v2.0_2016-09-22_181835.151325.cdl",
     ),
     "ocos": get_filename("tests/data/examples/ocos.cdl"),
     "ooi_glider": get_filename("tests/data/examples/ooi_glider.cdl"),
     "point": get_filename("tests/data/point.cdl"),
     "polygon_geometry": get_filename("tests/data/polygon_geometry.cdl"),
     "profile-orthogonal": get_filename("tests/data/profile-orthogonal.cdl"),
     "profile-incomplete": get_filename("tests/data/profile-incomplete.cdl"),
     "pr_inundation": get_filename("tests/data/examples/pr_inundation.cdl"),
     "reduced_horizontal_grid": get_filename("tests/data/reduced_horizontal_grid.cdl"),
     "rotated_pole_grid": get_filename("tests/data/rotated_pole_grid.cdl"),
     "rhgrid": get_filename("tests/data/rhgrid.cdl"),
     "rutgers": get_filename("tests/data/ru07-20130824T170228_rt0.cdl"),
     "scalar_coordinate_variable": get_filename(
-        "tests/data/scalar_coordinate_variable.cdl"
+        "tests/data/scalar_coordinate_variable.cdl",
     ),
     "self-referencing-var": get_filename("tests/data/self-referencing-var.cdl"),
     "self_referencing": get_filename("tests/data/non-comp/self_referencing.cdl"),
     "sldmb_43093_agg": get_filename("tests/data/examples/sldmb_43093_agg.cdl"),
     "string": get_filename("tests/data/string_type_variable.cdl"),
     "swan": get_filename("tests/data/examples/swan.cdl"),
     "sp041": get_filename("tests/data/examples/sp041.cdl"),
     "taxonomy_example": get_filename("tests/data/taxonomy_example.cdl"),
     "timeseries": get_filename("tests/data/timeseries.cdl"),
     "timeseries-profile-single-station": get_filename(
-        "tests/data/timeseries-profile-single-station.cdl"
+        "tests/data/timeseries-profile-single-station.cdl",
     ),
     "timeseries-profile-multi-station": get_filename(
-        "tests/data/timeseries-profile-multi-station.cdl"
+        "tests/data/timeseries-profile-multi-station.cdl",
     ),
     "timeseries-profile-single-ortho-time": get_filename(
-        "tests/data/timeseries-profile-single-ortho-time.cdl"
+        "tests/data/timeseries-profile-single-ortho-time.cdl",
     ),
     "timeseries-profile-multi-ortho-time": get_filename(
-        "tests/data/timeseries-profile-multi-ortho-time.cdl"
+        "tests/data/timeseries-profile-multi-ortho-time.cdl",
     ),
     "timeseries-profile-ortho-depth": get_filename(
-        "tests/data/timeseries-profile-ortho-depth.cdl"
+        "tests/data/timeseries-profile-ortho-depth.cdl",
     ),
     "timeseries-profile-incomplete": get_filename(
-        "tests/data/timeseries-profile-incomplete.cdl"
+        "tests/data/timeseries-profile-incomplete.cdl",
     ),
     "time_units": get_filename("tests/data/non-comp/time_units.cdl"),
     "trajectory-complete": get_filename("tests/data/trajectory-complete.cdl"),
     "trajectory-implied": get_filename("tests/data/trajectory-implied.cdl"),
     "trajectory-profile-orthogonal": get_filename(
-        "tests/data/trajectory-profile-orthogonal.cdl"
+        "tests/data/trajectory-profile-orthogonal.cdl",
     ),
     "trajectory-profile-incomplete": get_filename(
-        "tests/data/trajectory-profile-incomplete.cdl"
+        "tests/data/trajectory-profile-incomplete.cdl",
     ),
     "trajectory": get_filename("tests/data/trajectory.cdl"),
     "trajectory-single": get_filename("tests/data/trajectory-single.cdl"),
     "units_check": get_filename("tests/data/units_check.cdl"),
     "usgs_dem_saipan": get_filename("tests/data/examples/usgs_dem_saipan.cdl"),
     "valid_coordinates": get_filename("tests/data/valid_coordinates.cdl"),
     "vertical_coords": get_filename("tests/data/vertical_coords.cdl"),
```

### Comparing `compliance-checker-5.0.2/compliance_checker/tests/test_acdd.py` & `compliance-checker-5.1.0/compliance_checker/tests/test_acdd.py`

 * *Files 1% similar despite different names*

```diff
@@ -102,22 +102,23 @@
         assert self.acdd._cc_spec_version == "1.1"
 
     def test_highly_recommended(self):
         """
         Checks that all highly recommended attributes are present
         """
         assert check_varset_nonintersect(
-            self.expected["Highly Recommended"], self.acdd_highly_recommended
+            self.expected["Highly Recommended"],
+            self.acdd_highly_recommended,
         )
 
         # Check the reference dataset, NCEI 1.1 Gold Standard Point
         missing = ["\"Conventions\" does not contain 'ACDD-1.3'"]
         results = self.acdd.check_high(self.ds)
         for result in results:
-            if result.msgs and all([m in missing for m in result.msgs]):
+            if result.msgs and all(m in missing for m in result.msgs):
                 # only the Conventions check should have failed
                 self.assert_result_is_bad(result)
             self.assert_result_is_good(result)
 
         # Create an empty dataset that writes to /dev/null This acts as a
         # temporary netCDF file in-memory that never gets written to disk.
         empty_ds = Dataset(os.devnull, "w", diskless=True)
@@ -129,26 +130,27 @@
     def test_recommended(self):
         """
         Checks that all recommended attributes are present
         """
         # 'geospatial_bounds' attribute currently has its own separate check
         # from the list of required atts
         assert check_varset_nonintersect(
-            self.expected["Recommended"], self.acdd_recommended
+            self.expected["Recommended"],
+            self.acdd_recommended,
         )
 
         ncei_exceptions = [
             "geospatial_bounds not present",
             "time_coverage_duration not present",
             "time_coverage_resolution not present",
         ]
         results = self.acdd.check_recommended(self.ds)
         for result in results:
             if (result.msgs) and all(
-                [m in ncei_exceptions for m in result.msgs]
+                m in ncei_exceptions for m in result.msgs
             ):  # we're doing string comparisons, this is kind of hacky...
                 self.assert_result_is_bad(result)
                 continue
 
             self.assert_result_is_good(result)
 
         # Create an empty dataset that writes to /dev/null This acts as a
@@ -161,28 +163,29 @@
             self.assert_result_is_bad(result)
 
     def test_suggested(self):
         """
         Checks that all suggested attributes are present
         """
         assert check_varset_nonintersect(
-            self.expected["Suggested"], self.acdd_suggested
+            self.expected["Suggested"],
+            self.acdd_suggested,
         )
 
         # Attributes that are missing from NCEI but should be there
         missing = [
             "geospatial_lat_resolution not present",
             "geospatial_lon_resolution not present",
             "geospatial_vertical_resolution not present",
         ]
 
         results = self.acdd.check_suggested(self.ds)
         for result in results:
             if (result.msgs) and all(
-                [m in missing for m in result.msgs]
+                m in missing for m in result.msgs
             ):  # we're doing string comparisons, this is kind of hacky...
                 self.assert_result_is_bad(result)
                 continue
 
             self.assert_result_is_good(result)
 
         # Create an empty dataset that writes to /dev/null This acts as a
@@ -307,62 +310,65 @@
         assert self.acdd._cc_spec_version == "1.3"
 
     def test_highly_recommended(self):
         """
         Checks that all highly recommended attributes are present
         """
         assert check_varset_nonintersect(
-            self.expected["Highly Recommended"], self.acdd_highly_recommended
+            self.expected["Highly Recommended"],
+            self.acdd_highly_recommended,
         )
 
         results = self.acdd.check_high(self.ds)
         for result in results:
             # NODC 2.0 has a different value in the conventions field
             self.assert_result_is_good(result)
 
     def test_recommended(self):
         """
         Checks that all recommended attributes are present
         """
         assert check_varset_nonintersect(
-            self.expected["Recommended"], self.acdd_recommended
+            self.expected["Recommended"],
+            self.acdd_recommended,
         )
 
         results = self.acdd.check_recommended(self.ds)
         ncei_exceptions = [
             "time_coverage_duration not present",
             "time_coverage_resolution not present",
         ]
         for result in results:
             if (result.msgs) and all(
-                [m in ncei_exceptions for m in result.msgs]
+                m in ncei_exceptions for m in result.msgs
             ):  # we're doing string comparisons, this is kind of hacky...
                 self.assert_result_is_bad(result)
                 continue
 
             self.assert_result_is_good(result)
 
     def test_suggested(self):
         """
         Checks that all suggested attributes are present
         """
         assert check_varset_nonintersect(
-            self.expected["Suggested"], self.acdd_suggested
+            self.expected["Suggested"],
+            self.acdd_suggested,
         )
 
         results = self.acdd.check_suggested(self.ds)
         # NCEI does not require or suggest resolution attributes
         ncei_exceptions = [
             "geospatial_lat_resolution not present",
             "geospatial_lon_resolution not present",
             "geospatial_vertical_resolution not present",
         ]
         for result in results:
             if (result.msgs) and all(
-                [m in ncei_exceptions for m in result.msgs]
+                m in ncei_exceptions for m in result.msgs
             ):  # we're doing string comparisons, this is kind of hacky...
                 self.assert_result_is_bad(result)
                 continue
             self.assert_result_is_good(result)
 
     def test_variables(self):
         """
@@ -466,15 +472,17 @@
 
     def test_check_lat_extents(self):
         """Test the check_lat_extents() method behaves expectedly"""
 
         # create dataset using MockDataset, give it lat/lon dimensions
         ds = MockTimeSeries()
         ds.variables["lat"][:] = np.linspace(
-            -135.0, -130.0, num=500
+            -135.0,
+            -130.0,
+            num=500,
         )  # arbitrary, but matches time dim size
 
         # test no values, expect failure
         result = self.acdd.check_lat_extents(ds)
         self.assert_result_is_bad(result)
 
         # give integer geospatial_lat_max/min, test
```

### Comparing `compliance-checker-5.0.2/compliance_checker/tests/test_base.py` & `compliance-checker-5.1.0/compliance_checker/tests/test_base.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 #!/usr/bin/env python
-# -*- coding: utf-8 -*-
 """Tests for base compliance checker class"""
 
 import os
 from unittest import TestCase
 
 from netCDF4 import Dataset
 
@@ -29,21 +28,27 @@
         attr = ("test", None)
         base.attr_check(attr, self.ds, priority, rv1)
         assert rv1[0] == base.Result(priority, False, "test", ["test not present"])
         # test with empty string
         self.ds.test = ""
         base.attr_check(attr, self.ds, priority, rv2)
         assert rv2[0] == base.Result(
-            priority, False, "test", ["test is empty or completely whitespace"]
+            priority,
+            False,
+            "test",
+            ["test is empty or completely whitespace"],
         )
         # test with whitespace in the form of a space and a tab
         self.ds.test = " 	"
         base.attr_check(attr, self.ds, priority, rv3)
         assert rv3[0] == base.Result(
-            priority, False, "test", ["test is empty or completely whitespace"]
+            priority,
+            False,
+            "test",
+            ["test is empty or completely whitespace"],
         )
         # test with actual string contents
         self.ds.test = "abc 123"
         base.attr_check(attr, self.ds, priority, rv4)
         assert rv4[0] == base.Result(priority, True, "test", [])
 
     def test_attr_in_valid_choices(self):
```

### Comparing `compliance-checker-5.0.2/compliance_checker/tests/test_cf.py` & `compliance-checker-5.1.0/compliance_checker/tests/test_cf.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 #!/usr/bin/env python
-# -*- coding: utf-8 -*-
 
 import copy
 import json
 import os
 import re
 import sqlite3
 from itertools import chain
@@ -16,14 +15,15 @@
 
 from compliance_checker import cfutil
 from compliance_checker.cf.appendix_d import no_missing_terms
 from compliance_checker.cf.cf import (
     CF1_6Check,
     CF1_7Check,
     CF1_8Check,
+    CF1_9Check,
     dimless_vertical_coordinates_1_6,
     dimless_vertical_coordinates_1_7,
 )
 from compliance_checker.cf.util import (
     StandardNameTable,
     create_cached_data_dir,
     download_cf_standard_name_table,
@@ -31,14 +31,15 @@
     is_vertical_coordinate,
     units_convertible,
     units_temporal,
 )
 from compliance_checker.suite import CheckSuite
 from compliance_checker.tests import BaseTestCase
 from compliance_checker.tests.helpers import (
+    MockNetCDF,
     MockRaggedArrayRepr,
     MockTimeSeries,
     MockVariable,
 )
 from compliance_checker.tests.resources import STATIC_FILES
 
 
@@ -81,15 +82,15 @@
 
     def new_nc_file(self):
         """
         Make a new temporary netCDF file for the scope of the test
         """
         nc_file_path = os.path.join(gettempdir(), "example.nc")
         if os.path.exists(nc_file_path):
-            raise IOError("File Exists: %s" % nc_file_path)
+            raise OSError("File Exists: %s" % nc_file_path)
         nc = Dataset(nc_file_path, "w")
         self.addCleanup(os.remove, nc_file_path)
         self.addCleanup(nc.close)
         return nc
 
     def test_extension(self):
         # TEST CONFORMANCE 2.1
@@ -105,25 +106,31 @@
         ds = MockTimeSeries()
         ds.createDimension("siglev", 20)
 
         temp = ds.createVariable(
             "temp",
             np.float64,
             dimensions=("time",),
-            fill_value=np.float(99999999999999999999.0),
+            fill_value=float(99999999999999999999.0),
         )
         temp.coordinates = "sigma noexist"
         ds.createVariable("sigma", np.float64, dimensions=("siglev",))
         self.cf.setup(ds)
         # time is a NUG coordinate variable, sigma is not, but is referred to in
         # variables, so both should show up in cf_coord_data_vars.
         # noexist does not exist in the dataset's variables, so it is not
         # present in coord_data_vars
         self.assertEqual(self.cf.coord_data_vars, {"time", "sigma"})
 
+        ds = MockTimeSeries()
+        ds.variables["time"][:3] = np.array([20, -2, 0])
+        result = self.cf.check_coordinate_variables_strict_monotonicity(ds)
+        _, _, messages = get_results(result)
+        assert 'Coordinate variable "time" must be strictly monotonic' in messages
+
     # --------------------------------------------------------------------------------
     # Compliance Tests
     # --------------------------------------------------------------------------------
 
     def test_check_data_types(self):
         """
         Invoke check_data_types() and loop through all variables to check data
@@ -140,15 +147,15 @@
         result = self.cf.check_data_types(dataset)
         assert result.value[0] == result.value[1]
 
         # check if variables of type `string` is properly processed
         dataset = self.load_dataset(STATIC_FILES["string"])
         if dataset.file_format != "NETCDF4":
             raise RuntimeError(
-                "netCDF file of wrong format (not netCDF4) was created for checking"
+                "netCDF file of wrong format (not netCDF4) was created for checking",
             )
         result = self.cf.check_data_types(dataset)
         assert result.value[0] == result.value[1]
 
         # check bad data types
         dataset = self.load_dataset(STATIC_FILES["bad_data_type"])
         result = self.cf.check_data_types(dataset)
@@ -164,31 +171,33 @@
         """
         Tests check_child_attr_data_types() to ensure the attributes specified in Section 2.5.1
         have a matching data type to their parent variables."""
 
         # create dataset using MockDataset (default constructor gives it time dimension)
         ds = MockTimeSeries()
         ds.createVariable(
-            "temp", np.float64, dimensions=("time")
+            "temp",
+            np.float64,
+            dimensions=("time"),
         )  # add variable "temp" with dimension "time"
 
         # check where no special data attrs are present, should result good
         result = self.cf.check_child_attr_data_types(
-            ds
+            ds,
         )  # checks all special attrs for all variables
         self.assert_result_is_good(result)
 
         # delete the dataset and start over to create the variable with _FillValue at time of creation
         del ds
         ds = MockTimeSeries()
         ds.createVariable(
             "temp",
             np.float64,
             dimensions=("time",),
-            fill_value=np.float(99999999999999999999.0),
+            fill_value=float(99999999999999999999.0),
         )
 
         # give temp _FillValue as a float, expect good result
         result = self.cf.check_child_attr_data_types(ds)
         self.assert_result_is_good(result)
 
         # give temp valid_range as an array of floats, all should check out
@@ -211,15 +220,16 @@
         var.setncattr("valid_max", "@")
         result = self.cf.check_child_attr_data_types(ds)
         self.assert_result_is_good(result)
         var.setncattr("valid_max", b"@")
         result = self.cf.check_child_attr_data_types(ds)
         self.assert_result_is_good(result)
 
-        # now give invalid integer for valid_min; above two should still check out, this one should fail
+        # now give invalid integer for valid_min; above two should still check
+        # out, this one should fail
         ds.variables["temp"].setncattr("valid_min", 45)
         result = self.cf.check_child_attr_data_types(ds)
         self.assert_result_is_bad(result)
 
         # now give invalid string for valid_max
         ds.variables["temp"].setncattr("valid_max", "eighty")
         result = self.cf.check_child_attr_data_types(ds)
@@ -279,14 +289,28 @@
         results = self.cf.check_naming_conventions(dataset)
         scored, out_of, messages = get_results(results)
         assert len(results) == 3
         assert scored < out_of
         assert len([r for r in results if r.value[0] < r.value[1]]) == 2
         assert all(r.name == "§2.3 Naming Conventions" for r in results)
 
+        dataset = MockTimeSeries()
+        # test for ignored attributes
+        temp = dataset.createVariable("temperature", "f8", ("time",), fill_value=-9999)
+        temp.standard_name = "sea_water_temperature"
+        temp.units = "degrees_C"
+        temp.DODS = ""
+        temp._ChunkSizes = 5
+        temp._Coordinate = ""
+        temp._Unsigned = 0
+        temp._Encoding = "utf-8"
+        results = self.cf.check_naming_conventions(dataset)
+        scored, out_of, messages = get_results(results)
+        assert scored == out_of
+
     def test_check_names_unique(self):
         """
         2.3 names should not be distinguished purely by case, i.e., if case is disregarded, no two names should be the same.
         """
         # TEST CONFORMANCE 2.3 Recommended
         dataset = self.load_dataset(STATIC_FILES["rutgers"])
         result = self.cf.check_names_unique(dataset)
@@ -339,14 +363,85 @@
         )
 
         dataset = self.load_dataset(STATIC_FILES["dimension_order"])
         result = self.cf.check_dimension_order(dataset)
         self.assertEqual((3, 3), result.value)
         self.assertEqual([], result.msgs)
 
+    def test_check_fill_value_equal_missing_value(self):
+        """
+        According to CF §2.5.1 Recommendations: If both missing_value and _FillValue be used,
+        they should have the same value.
+        """
+        # TEST CONFORMANCE 2.5.1 RECOMMENDED
+        dataset = MockTimeSeries()
+        # Case of _FillValue and missing_value are not equal
+        dataset.createVariable("a", "d", ("time",), fill_value=9999.9)
+        dataset.variables["a"][0] = 1
+        dataset.variables["a"][1] = 2
+        dataset.variables["a"].setncattr("missing_value", [9939.9])
+
+        # Case of _FillValue and missing_value are equal
+        dataset.createVariable("b", "d", ("time",), fill_value=9999.9)
+        dataset.variables["b"][0] = 1
+        dataset.variables["b"][1] = 2
+        dataset.variables["b"].setncattr("missing_value", [9999.9])
+
+        result = self.cf.check_fill_value_equal_missing_value(dataset)
+
+        # check if the test fails when when variable "a" is checked.
+        expected_msgs = [
+            f"For the variable {v_name} the missing_value must be equal to the _FillValue"
+            for v_name in ("a")
+        ]
+
+        assert result.msgs == expected_msgs
+
+    def test_check_valid_range_or_valid_min_max_present(self):
+        """
+        2.5.1 Missing data, valid and actual range of data
+        Requirements:
+        The valid_range attribute must not be present if the
+        valid_min and/or valid_max attributes are present.
+        """
+        # TEST CONFORMANCE 2.5.1 REQUIRED
+        dataset = MockTimeSeries()
+        # Case of valid_min, valid_max, and valid_range are present
+        dataset.createVariable("a", "d", ("time",), fill_value=9999.9)
+        dataset.variables["a"][0] = 1
+        dataset.variables["a"][1] = 2
+        dataset.variables["a"].setncattr("valid_min", [-10])
+        dataset.variables["a"].setncattr("valid_max", [10])
+        dataset.variables["a"].setncattr("valid_range", [-10, 10])
+
+        # Case of valid_min and valid_max are present and valid_range is absent
+        dataset.createVariable("b", "d", ("time",), fill_value=9999.9)
+        dataset.variables["b"][0] = 1
+        dataset.variables["b"][1] = 2
+        dataset.variables["a"].setncattr("valid_min", [-10])
+        dataset.variables["a"].setncattr("valid_max", [10])
+
+        # Case of valid_min and valid_max are absent and valid_range is present
+        dataset.createVariable("c", "d", ("time",), fill_value=9999.9)
+        dataset.variables["c"][0] = 1
+        dataset.variables["c"][1] = 2
+        dataset.variables["c"].setncattr("valid_range", [-10, 10])
+
+        result = self.cf.check_valid_range_or_valid_min_max_present(dataset)
+
+        # check if the test fails when when variable "a" is checked.
+        expected_msgs = [
+            f"For the variable {v_name} the valid_range attribute must not be present "
+            f"if the valid_min and/or valid_max attributes are present"
+            for v_name in ("a")
+        ]
+
+        assert result.msgs == expected_msgs
+        assert result.value[0] == result.value[1]
+
     def test_check_fill_value_outside_valid_range(self):
         """
         2.5.1 The _FillValue should be outside the range specified by valid_range (if used) for a variable.
         """
         # TEST CONFORMANCE 2.5.1 REQUIRED
         dataset = self.load_dataset(STATIC_FILES["bad_data_type"])
         result = self.cf.check_fill_value_outside_valid_range(dataset)
@@ -550,39 +645,76 @@
         score, out_of, messages = get_results(results)
         assert score == out_of
         assert score > 0
 
         dataset = self.load_dataset(STATIC_FILES["bad_cell_measure1"])
         results = self.cf.check_cell_measures(dataset)
         score, out_of, messages = get_results(results)
-        message = (
-            "The cell_measures attribute for variable PS is formatted incorrectly.  "
+        expected_message = (
+            "The cell_measures attribute for variable PS is formatted incorrectly. "
             "It should take the form of either 'area: cell_var' or 'volume: cell_var' "
-            "where cell_var is the variable describing the cell measures"
+            "where cell_var is an existing name of a variable describing the "
+            "cell measures."
         )
-        assert message in messages
+        assert expected_message in messages
 
         dataset = self.load_dataset(STATIC_FILES["bad_cell_measure2"])
         results = self.cf.check_cell_measures(dataset)
         score, out_of, messages = get_results(results)
         message = "Cell measure variable box_area referred to by PS is not present in dataset variables"
         assert message in messages
 
+        dataset = MockTimeSeries()
+        dataset.createVariable("PS", "d", ("time",))  # dtype=double, dims=time
+        dataset.variables["PS"].setncattr("cell_measures", "area: cell_area")
+        # ensure the cell_measures var is in the dataset
+        dataset.createVariable("cell_area", "d", ("time",))
+        dataset.variables["cell_area"].setncattr("units", "m3")
+        # TEST CONFORMANCE 7.2 REQUIRED
+        # inappropriate length exponent for area
+        expected_fail_msg = (
+            'Variable "cell_area" must have units which are convertible '
+            'to UDUNITS "m2" when variable is referred to by a dataset variable with '
+            'cell_methods attribute with a measure type of "area".'
+        )
+        results = self.cf.check_cell_measures(dataset)
+        score, out_of, messages = get_results(results)
+        assert expected_fail_msg in messages
+
+        # set erroneous units that aren't convertible to UDUnits length
+        # units
+        dataset.variables["cell_area"].setncattr("units", "s3")
+        results = self.cf.check_cell_measures(dataset)
+        score, out_of, messages = get_results(results)
+        assert expected_fail_msg in messages
+
+        # TEST CONFORMANCE 7.2 REQUIRED 1/2
+        dataset.createDimension("depth2", 5)
+        dataset.variables["PS"].setncattr("cell_measures", "area: cell_area2")
+        dataset.createVariable("cell_area2", "f8", ("time", "depth2"))
+        dataset.variables["cell_area2"].setncattr("units", "m2")
+        results = self.cf.check_cell_measures(dataset)
+        score, out_of, messages = get_results(results)
+        assert (
+            "Cell measure variable cell_area2 must have dimensions which are a subset of those defined in variable PS."
+            in messages
+        )
+
     def test_climatology_cell_methods(self):
         """
         Checks that climatology cell_methods strings are properly validated
         """
         dataset = self.load_dataset(STATIC_FILES["climatology"])
         results = self.cf.check_climatological_statistics(dataset)
         # cell methods in this file is
         # "time: mean within days time: mean over days"
         score, out_of, messages = get_results(results)
         self.assertEqual(score, out_of)
         temp_var = dataset.variables["temperature"] = MockVariable(
-            dataset.variables["temperature"]
+            dataset.variables["temperature"],
         )
         temp_var.cell_methods = "INVALID"
         results = self.cf.check_climatological_statistics(dataset)
         score, out_of, messages = get_results(results)
         self.assertNotEqual(score, out_of)
         # incorrect time units
         temp_var.cell_methods = "time: mean within years time: mean over days"
@@ -608,26 +740,65 @@
         temp_var.cell_methods = (
             "time: sum within days time: maximum over days (ENSO years)"
         )
         results = self.cf.check_climatological_statistics(dataset)
         score, out_of, messages = get_results(results)
         self.assertEqual(score, out_of)
 
+        # TEST CONFORMANCE 7.4 REQUIRED 5/6
+        dataset.variables["climatology_bounds"] = MockVariable(
+            dataset.variables["climatology_bounds"],
+        )
+        clim_bounds = dataset.variables["climatology_bounds"]
+        clim_bounds.standard_name = "forecast_reference_time"
+        clim_bounds.calendar = "proleptic_gregorian"
+        clim_bounds.units = "hours since 1999-02-01"
+        results = self.cf.check_climatological_statistics(dataset)
+        score, out_of, messages = get_results(results)
+        for attr_name in ("calendar", "standard_name", "units"):
+            assert (
+                f"Attribute {attr_name} must have the same value in both variables {clim_bounds.name} and time"
+                in messages
+            )
+        # TEST CONFORMANCE 7.4 REQUIRED 6/6
+        clim_bounds.missing_value = clim_bounds._FillValue = -9999.99
+        results = self.cf.check_climatological_statistics(dataset)
+        score, out_of, messages = get_results(results)
+        assert (
+            f"Climatology variable {clim_bounds.name} may not contain attributes _FillValue or missing_value"
+            in messages
+        )
+
+        # TEST CONFORMANCE 7.4 REQUIRED 3/6
         bad_dim_ds = MockTimeSeries()
         bad_dim_ds.createDimension("clim_bounds", 3)
 
         temp = bad_dim_ds.createVariable("temperature", "f8", ("time",))
         bad_dim_ds.createVariable("clim_bounds", "f8", ("time"))
         temp.climatology = "clim_bounds"
         results = self.cf.check_climatological_statistics(bad_dim_ds)
         assert results[1].value[0] < results[1].value[1]
         assert (
             results[1].msgs[0] == 'Climatology dimension "clim_bounds" '
             "should only contain two elements"
         )
+        # TEST CONFORMANCE 7.4 REQUIRED 1/6
+        assert (
+            results[0].msgs[0]
+            == "Variable temperature is not detected as a time coordinate "
+            "variable, but has climatology attribute"
+        )
+
+        # TEST CONFORMANCE 7.4 REQUIRED 2/6
+        bad_dim_ds.variables["time"].climatology = 1
+        results = self.cf.check_climatological_statistics(bad_dim_ds)
+        assert (
+            results[0].msgs[0]
+            == "Variable time must have a climatology attribute which is a string"
+        )
 
     def test_check_ancillary_variables(self):
         """
         Test to ensure that ancillary variables are properly checked
         """
 
         dataset = self.load_dataset(STATIC_FILES["rutgers"])
@@ -647,15 +818,16 @@
         """
         Test that a user can download a specific standard name table
         """
         version = "35"
 
         data_directory = create_cached_data_dir()
         location = os.path.join(
-            data_directory, "cf-standard-name-table-test-{0}.xml".format(version)
+            data_directory,
+            f"cf-standard-name-table-test-{version}.xml",
         )
         download_cf_standard_name_table(version, location)
 
         # Test that the file now exists in location and is the right version
         self.assertTrue(os.path.isfile(location))
         std_names = StandardNameTable(location)
         self.assertEqual(std_names._version, version)
@@ -691,15 +863,15 @@
         results = self.cf.check_flags(dataset)
         scored, out_of, messages = get_results(results)
 
         # only 4 variables in this dataset do not have perfect scores
         imperfect = [r.value for r in results if r.value[0] < r.value[1]]
         assert len(imperfect) == 4
         dataset.variables["conductivity_qc"] = MockVariable(
-            dataset.variables["conductivity_qc"]
+            dataset.variables["conductivity_qc"],
         )
         # Test with single element.  Will fail, but should not throw exception.
         dataset.variables["conductivity_qc"].flag_values = np.array([1], dtype=np.int8)
         results = self.cf.check_flags(dataset)
 
     def test_check_flag_masks(self):
         dataset = self.load_dataset(STATIC_FILES["ghrsst"])
@@ -926,104 +1098,104 @@
         # For each of the listed dimensionless vertical coordinates,
         # verify that the formula_terms match the provided set of terms
         self.assertTrue(
             no_missing_terms(
                 "atmosphere_ln_pressure_coordinate",
                 {"p0", "lev"},
                 dimless_vertical_coordinates_1_6,
-            )
+            ),
         )
         self.assertTrue(
             no_missing_terms(
                 "atmosphere_sigma_coordinate",
                 {"sigma", "ps", "ptop"},
                 dimless_vertical_coordinates_1_6,
-            )
+            ),
         )
         self.assertTrue(
             no_missing_terms(
                 "atmosphere_hybrid_sigma_pressure_coordinate",
                 {"a", "b", "ps"},
                 dimless_vertical_coordinates_1_6,
-            )
+            ),
         )
         # test alternative terms for
         # 'atmosphere_hybrid_sigma_pressure_coordinate'
         self.assertTrue(
             no_missing_terms(
                 "atmosphere_hybrid_sigma_pressure_coordinate",
                 {"ap", "b", "ps"},
                 dimless_vertical_coordinates_1_6,
-            )
+            ),
         )
         # check that an invalid set of terms fails
         self.assertFalse(
             no_missing_terms(
                 "atmosphere_hybrid_sigma_pressure_coordinate",
                 {"a", "b", "p"},
                 dimless_vertical_coordinates_1_6,
-            )
+            ),
         )
         self.assertTrue(
             no_missing_terms(
                 "atmosphere_hybrid_height_coordinate",
                 {"a", "b", "orog"},
                 dimless_vertical_coordinates_1_6,
-            )
+            ),
         )
         # missing terms should cause failure
         self.assertFalse(
             no_missing_terms(
                 "atmosphere_hybrid_height_coordinate",
                 {"a", "b"},
                 dimless_vertical_coordinates_1_6,
-            )
+            ),
         )
         # excess terms should cause failure
         self.assertFalse(
             no_missing_terms(
                 "atmosphere_hybrid_height_coordinate",
                 {"a", "b", "c", "orog"},
                 dimless_vertical_coordinates_1_6,
-            )
+            ),
         )
         self.assertTrue(
             no_missing_terms(
                 "atmosphere_sleve_coordinate",
                 {"a", "b1", "b2", "ztop", "zsurf1", "zsurf2"},
                 dimless_vertical_coordinates_1_6,
-            )
+            ),
         )
         self.assertTrue(
             no_missing_terms(
                 "ocean_sigma_coordinate",
                 {"sigma", "eta", "depth"},
                 dimless_vertical_coordinates_1_6,
-            )
+            ),
         )
         self.assertTrue(
             no_missing_terms(
                 "ocean_s_coordinate",
                 {"s", "eta", "depth", "a", "b", "depth_c"},
                 dimless_vertical_coordinates_1_6,
-            )
+            ),
         )
         self.assertTrue(
             no_missing_terms(
                 "ocean_sigma_z_coordinate",
-                {"sigma", "eta", "depth", "depth_c", "nsigma", "zlev"},
+                {"sigma", "eta", "depth", "depth_c", "zlev"},
                 dimless_vertical_coordinates_1_6,
-            )
+            ),
         )
         self.assertTrue(
             no_missing_terms(
                 "ocean_double_sigma_coordinate",
                 {"sigma", "depth", "z1", "z2", "a", "href", "k_c"},
                 dimless_vertical_coordinates_1_6,
-            )
+            ),
         )
 
     def test_dimensionless_vertical(self):
         """
         Section 4.3.2
         """
         # Check affirmative compliance
@@ -1057,14 +1229,19 @@
         scored, out_of, messages = get_results(results)
 
         assert len(results) == 4
         assert scored <= out_of
         assert len([r for r in results if r.value[0] < r.value[1]]) == 2
         assert all(r.name == "§4.3 Vertical Coordinate" for r in results)
 
+        # blank string is not valid and won't match, ensure this is caught
+        lev2.formula_terms = ""
+        results = self.cf.check_dimensionless_vertical_coordinates(dataset)
+        assert "Attribute formula_terms is not well-formed"
+
     def test_is_time_variable(self):
         var1 = MockVariable()
         var1.standard_name = "time"
         self.assertTrue(is_time_variable("not_time", var1))
 
         var2 = MockVariable()
         self.assertTrue(is_time_variable("time", var2))
@@ -1081,43 +1258,64 @@
 
     def test_dimensionless_standard_names(self):
         """Check that dimensionless standard names are properly detected"""
         std_names_xml_root = self.cf._std_names._root
         # canonical_units are K, should be False
         self.assertFalse(
             cfutil.is_dimensionless_standard_name(
-                std_names_xml_root, "sea_water_temperature"
-            )
+                std_names_xml_root,
+                "sea_water_temperature",
+            ),
         )
         # canonical_units are 1, should be True
         self.assertTrue(
             cfutil.is_dimensionless_standard_name(
-                std_names_xml_root, "sea_water_practical_salinity"
-            )
+                std_names_xml_root,
+                "sea_water_practical_salinity",
+            ),
         )
         # canonical_units are 1e-3, should be True
         self.assertTrue(
             cfutil.is_dimensionless_standard_name(
-                std_names_xml_root, "sea_water_salinity"
-            )
+                std_names_xml_root,
+                "sea_water_salinity",
+            ),
         )
 
     def test_check_time_coordinate(self):
         dataset = self.load_dataset(STATIC_FILES["example-grid"])
         results = self.cf.check_time_coordinate(dataset)
         for r in results:
             self.assertTrue(r.value)
 
+        # TEST CONFORMANCE 4.4 REQUIRED 1/2
         dataset = self.load_dataset(STATIC_FILES["bad"])
         results = self.cf.check_time_coordinate(dataset)
 
         scored, out_of, messages = get_results(results)
 
         assert "time does not have correct time units" in messages
         assert (scored, out_of) == (1, 2)
+        # TEST CONFORMANCE 4.4 REQUIRED 2/2, RECOMMENDED 1, 2/2
+        dataset = MockTimeSeries()
+        # NB: >= 60 seconds is nonstandard, but isn't actually a CF requirement
+        # until CF 1.9 onwards
+        dataset.variables["time"].units = "months since 0-1-1 23:00:60"
+        dataset.variables[
+            "time"
+        ].climatology = (
+            "nonexistent_variable_reference_only_used_to_test_year_zero_failure"
+        )
+        results = self.cf.check_time_coordinate(dataset)
+        scored, out_of, messages = get_results(results)
+        assert scored < out_of
+        assert (
+            "Using relative time interval of months or years is not recommended for coordinate variable time"
+            in messages
+        )
 
     def test_check_calendar(self):
         """Load a dataset with an invalid calendar attribute (non-comp/bad.nc).
         This dataset has a variable, "time" with  calendar attribute "nope"."""
 
         dataset = self.load_dataset(STATIC_FILES["example-grid"])
         results = self.cf.check_calendar(dataset)
@@ -1128,27 +1326,55 @@
         results = self.cf.check_calendar(dataset)
         scored, out_of, messages = get_results(results)
         # TEST CONFORMANCE 4.4.1 REQUIRED 2, 3 / 5
         bad_month_msg = (
             "For nonstandard calendar on variable time, attribute "
             "month_lengths must be supplied as a 12-element integer array"
         )
-
         assert bad_month_msg in messages
 
         dataset = MockTimeSeries()
-        dataset.variables["time"]
+        # no calendar should not raise an issue on time coordinate variables
+        del dataset.variables["time"].calendar
+        results = self.cf.check_calendar(dataset)
+        scored, out_of, messages = get_results(results)
+        assert not messages
+
+        # test case insensivity
+        valid_calendars = (
+            "GREGORIAN",
+            "STANDARD",
+            "PROLEPTIC_GREGORIAN",
+            "NOLEAP",
+            "365_DAY",
+            "ALL_LEAP",
+            "366_DAY",
+            "360_DAY",
+            "JULIAN",
+            "NONE",
+        )
+        for calendar_uppercase in valid_calendars:
+            # need to make a new MockTimeSeries when attribute deleted for
+            # calendar attributes to work properly
+            dataset = MockTimeSeries()
+            dataset.calendar = calendar_uppercase
+            results = self.cf.check_calendar(dataset)
+            scored, out_of, messages = get_results(results)
+            assert scored == out_of
+
+        # test custom month length calendars
         dataset.variables["time"].calendar = "custom"
         dataset.variables["time"].month_lengths = np.array([30.3], dtype=np.double)
         results = self.cf.check_calendar(dataset)
         scored, out_of, messages = get_results(results)
         assert bad_month_msg in messages
 
         dataset.variables["time"].month_lengths = np.array(
-            [31, 29, 31, 30, 31, 30, 31, 31, 30, 31, 30, 31], dtype=np.int
+            [31, 29, 31, 30, 31, 30, 31, 31, 30, 31, 30, 31],
+            dtype=int,
         )
         results = self.cf.check_calendar(dataset)
         scored, out_of, messages = get_results(results)
         assert bad_month_msg not in messages
 
         # TEST CONFORMANCE 4.4.1 REQUIRED 4,5/5
         leap_month_msg = (
@@ -1183,14 +1409,44 @@
         assert leap_year_msg in messages
 
         dataset.variables["time"].leap_year = 4
         results = self.cf.check_calendar(dataset)
         scored, out_of, messages = get_results(results)
         assert leap_year_msg not in messages
 
+        for calendar in ("standard", "gregorian"):
+            dataset.variables["time"].calendar = calendar
+            dataset.variables["time"].units = "seconds since 1582-10-15T00:00Z"
+            # 500 element array with some failing values
+            # _FillValue at first element even though should not be present
+            # in time coordinate variable to test bad data handling
+            # TEST CONFORMANCE 4.4.1 RECOMMENDED 4/4
+            dataset.variables["time"][1:] = np.arange(-2, 497)
+            results = self.cf.check_calendar(dataset)
+            scored, out_of, messages = get_results(results)
+            assert messages[-1] == (
+                "Variable time has time values prior to "
+                "1582-10-15T00:00Z and utilizes the "
+                "standard or Gregorian calendar"
+            )
+            dataset.variables["time"][:] = np.arange(0, 500)
+            results = self.cf.check_calendar(dataset)
+            scored, out_of, messages = get_results(results)
+            assert messages[-1] == (
+                "Variable time has standard or Gregorian "
+                "calendar and does not cross 1582-10-15T00:00Z"
+            )
+            # TEST CONFORMANCE 4.4.1 RECOMMENDED 3/4
+            if calendar == "gregorian":
+                assert (
+                    "For time variable time, when using the standard "
+                    'Gregorian calendar, the value "standard" is preferred '
+                    'over "gregorian" for the calendar attribute' in messages
+                )
+
     def test_check_aux_coordinates(self):
         dataset = self.load_dataset(STATIC_FILES["illegal-aux-coords"])
         results = self.cf.check_aux_coordinates(dataset)
         result_dict = {result.name: result for result in results}
         result = result_dict["§5 Coordinate Systems"]
         assert result.msgs == []  # shouldn't have any messages
         assert result.value == (4, 4)
@@ -1251,29 +1507,28 @@
         assert len([r.value for r in results.values() if r.value[0] < r.value[1]]) == 0
         expected_name = (
             "§5.6 Horizontal Coordinate Reference Systems, Grid Mappings, Projections"
         )
         assert all(r.name == expected_name for r in results.values())
 
     def test_is_geophysical(self):
-
         # check whether string type variable, which are not `cf_role`, are
         # properly processed
         dataset = self.load_dataset(STATIC_FILES["string"])
         if dataset.file_format != "NETCDF4":
             raise RuntimeError(
-                "netCDF file of wrong format (not netCDF4) was created for checking"
+                "netCDF file of wrong format (not netCDF4) was created for checking",
             )
         try:
             result = cfutil.is_geophysical(dataset, "j")
         except AttributeError:
             pytest.fail(
                 "Test probably fails because var.dtype.kind or var.dtype.char "
                 "was tested on string-type variable. Consider checking for "
-                "`var.dtype is str`"
+                "`var.dtype is str`",
             )
         assert not result
         # assert False
 
     # TODO: overhaul to use netCDF global attributes or mocks and variable
     #       attributes
     def test_check_attr_type(self):
@@ -1332,15 +1587,16 @@
         _var = nc_obj.variables["temperature"]
         att_name = "test_att"
         att = np.int32(2)
         att_type = "D"  # should be same datatypes
         res = self.cf._check_attr_type(att_name, att_type, att, _var)
         self.assertFalse(res[0])
         self.assertEqual(
-            res[1], "test_att must be numeric and must be equivalent to float64 dtype"
+            res[1],
+            "test_att must be numeric and must be equivalent to float64 dtype",
         )
 
     def test_check_grid_mapping_attr_condition(self):
         """
         Ensure the check_grid_mapping_attr_condition() method works as expected.
         """
 
@@ -1479,21 +1735,30 @@
         temp.units = "degree_C"
 
         temp_flag = dataset.createVariable("temp_flag", "i1", ("time",))
         temp_flag.standard_name = "sea_water_temperature status_flag"
         # units should not exist for
         temp_flag.units = "1"
 
+        time_flag = dataset.createVariable("time_flag", "i1", ("time",))
+        time_flag.standard_name = "time status_flag"
+        time_flag.flag_values = np.array([1, 2], dtype=np.int8)
+        time_flag.flag_meanings = "good bad"
+
+        lat_flag = dataset.createVariable("lat_flag", "i1", ("time",))
+        lat_flag.standard_name = "latitude status_flag"
+
         temp.ancillary_variables = "temp_flag"
         scored, out_of, messages = get_results(self.cf.check_units(dataset))
-        assert scored != out_of
-        assert (
-            "units attribute for variable temperature_flag must be unset "
-            "when status_flag modifier is set"
-        )
+        n_failed = out_of - scored
+        assert n_failed == 1
+        expected_messages = {
+            "units attribute for variable temp_flag must be unset when status_flag standard name modifier is set",
+        }
+        assert set(messages) == expected_messages
 
         del temp_flag.units
         scored, out_of, messages = get_results(self.cf.check_units(dataset))
         assert scored == out_of
 
         dataset.createVariable("temp_counts", "i1", ("time",))
         temp.ancillary_variables += " temp_counts"
@@ -1530,15 +1795,14 @@
     def test_64bit(self):
         dataset = self.load_dataset(STATIC_FILES["ints64"])
         suite = CheckSuite()
         suite.checkers = {"cf": CF1_6Check}
         suite.run(dataset, "cf")
 
     def test_variable_feature_check(self):
-
         # non-compliant dataset -- 1/1 fail
         dataset = self.load_dataset(STATIC_FILES["bad-trajectory"])
         results = self.cf.check_variable_features(dataset)
         scored, out_of, messages = get_results(results)
         assert len(results) == 2
         assert scored < out_of
         assert len([r for r in results if r.value[0] < r.value[1]]) == 1
@@ -1566,16 +1830,16 @@
         results = self.cf.check_cell_methods(dataset)
         scored, out_of, messages = get_results(results)
 
         # use itertools.chain() to unpack the lists of messages
         results_list = list(chain(*(r.msgs for r in results if r.msgs)))
 
         # check the results only have expected headers
-        assert set([r.name for r in results]).issubset(
-            set(["§7.1 Cell Boundaries", "§7.3 Cell Methods"])
+        assert {r.name for r in results}.issubset(
+            {"§7.1 Cell Boundaries", "§7.3 Cell Methods"},
         )
 
         # check that all the expected variables have been hit
         assert all("temperature" in msg for msg in results_list)
 
         # check that all the results have come back passing
         assert all(r.value[0] == r.value[1] for r in results)
@@ -1600,15 +1864,15 @@
             "lat: lon: mean depth: mean (comment: should not go here interval: 2.5 m)"
         )
         results = self.cf.check_cell_methods(nc_obj)
         scored, out_of, messages = get_results(results)
 
         self.assertTrue(
             '§7.3.3 The non-standard "comment:" element must come after any standard elements in cell_methods for variable temperature'
-            in messages
+            in messages,
         )
 
         # standalone comments require no keyword
         temp.cell_methods = "lon: mean (This is a standalone comment)"
         results = self.cf.check_cell_methods(nc_obj)
         scored, out_of, messages = get_results(results)
         assert "standalone" not in messages
@@ -1617,15 +1881,15 @@
         temp.cell_methods = (
             "lat: lon: mean depth: mean (invalid_keyword: this is invalid)"
         )
         results = self.cf.check_cell_methods(nc_obj)
         scored, out_of, messages = get_results(results)
         self.assertTrue(
             '§7.3.3 Invalid cell_methods keyword "invalid_keyword:" for variable temperature. Must be one of [interval, comment]'
-            in messages
+            in messages,
         )
 
         # check that "parenthetical elements" are well-formed (they should not be)
         temp.cell_methods = (
             "lat: lon: mean depth: mean (interval 0.2 m interval: 0.01 degrees)"
         )
         results = self.cf.check_cell_methods(nc_obj)
@@ -1804,15 +2068,15 @@
         """
         Check our over-ridden check_cell_boundaries method behaves as expected
         """
 
         dataset = self.load_dataset(STATIC_FILES["grid-boundaries"])
         results = self.cf.check_cell_boundaries(dataset)
         score, out_of, messages = get_results(results)
-        assert (score, out_of) == (2, 2)
+        assert (score, out_of) == (0, 2)
 
         dataset = self.load_dataset(STATIC_FILES["cf_example_cell_measures"])
         results = self.cf.check_cell_boundaries(dataset)
 
         dataset = self.load_dataset(STATIC_FILES["bad_data_type"])
         results = self.cf.check_cell_boundaries(dataset)
 
@@ -1842,61 +2106,126 @@
             score, out_of, messages = get_results(results)
             assert score < out_of
             assert (
                 "'a' has 'formula_terms' attr, bounds variable 'b' must also have 'formula_terms'"
                 in messages
             )
 
-    def test_cell_measures(self):
-        """Over-ride the test_cell_measures from CF1_6"""
+    def test_check_cell_boundaries_interval(self):
+        """
+        7.1 Cell Boundaries
+        Recommendations: (1/2)
+        The points specified by a coordinate or auxiliary coordinate variable
+        should lie within, or on the boundary, of the cells specified by the
+        associated boundary variable.
+        """
 
+        # create Cells on a longitude axis
+        dataset = MockTimeSeries()
+        dataset.createDimension("rnv", 2)
+        dataset.createDimension("rlon", 2)
+        dataset.createVariable("rlon", "d", ("rlon",))
+        dataset.createVariable("rlon_bnds", "d", ("rlon", "rnv"))
+
+        rlon = dataset.variables["rlon"]
+        rlon.standard_name = "longitude"
+        rlon.units = "degrees_east"
+        rlon.axis = "X"
+        rlon.long_name = "Longitude"
+        rlon.bounds = "rlon_bnds"
+        rlon[:] = np.array([-97.5, -99.5], dtype=np.float64)
+
+        rlon_bnds = dataset.variables["rlon_bnds"]
+        rlon_bnds.long_name = "Longitude Cell Boundaries"
+        rlon_bnds[:] = np.array([[-97, -98], [-98, -99]], dtype=np.float64)
+
+        results = self.cf.check_cell_boundaries_interval(dataset)
+        score, out_of, messages = get_results(results)
+        assert (score, out_of) == (1, 2)
+
+    def test_cell_measures(self):
         # create a temporary variable and test this only
         with MockTimeSeries() as dataset:
             dataset.createVariable("PS", "d", ("time",))  # dtype=double, dims=time
             dataset.variables["PS"].setncattr("cell_measures", "area: cell_area")
             # ensure the cell_measures var is in the dataset
             dataset.createVariable("cell_area", "d", ("time",))
             dataset.variables["cell_area"].setncattr("units", "m2")
 
             # run the check
             results = self.cf.check_cell_measures(dataset)
             score, out_of, messages = get_results(results)
             assert (score == out_of) and (score > 0)
 
-        # same thing, but test that the cell_area variable is in
-        # the global attr "external_variables"
+            # bad measure, not area or volume
+            dataset.variables["PS"].cell_measures = "length: cell_area"
+            results = self.cf.check_cell_measures(dataset)
+            score, out_of, messages = get_results(results)
+            assert (
+                "The cell_measures attribute for variable PS is formatted "
+                "incorrectly. It should take the form of either 'area: "
+                "cell_var' or 'volume: cell_var' where cell_var is an "
+                "existing name of a variable describing the cell measures." in messages
+            )
 
-        with MockTimeSeries() as dataset:
-            dataset.createVariable("PS", "d", ("time",))  # dtype=double, dims=time
-            dataset.variables["PS"].setncattr("cell_measures", "area: cell_area")
-            dataset.setncattr("external_variables", ["cell_area"])
+            # proper measure type, but referenced variable does not exist
+            dataset.variables["PS"].cell_measures = "area: NONEXISTENT_VAR"
+            results = self.cf.check_cell_measures(dataset)
+            score, out_of, messages = get_results(results)
+            assert (
+                "Cell measure variable NONEXISTENT_VAR referred to by "
+                "PS is not present in dataset or external variables" in messages
+            )
 
-            # run the check
+            dataset.variables["PS"].cell_measures = "area: no_units"
+            dataset.createVariable("no_units", "i2", ())
             results = self.cf.check_cell_measures(dataset)
             score, out_of, messages = get_results(results)
-            assert score > 0
-            assert score == out_of
+            assert (
+                "Cell measure variable no_units is required to have units "
+                "attribute defined" in messages
+            )
+
+        # cell_area variable is in
+        # the global attr "external_variables"
+
+        dataset = MockTimeSeries()
+        dataset.createVariable("PS", "d", ("time",))  # dtype=double, dims=time
+        dataset.variables["PS"].setncattr("cell_measures", "area: cell_area")
+        dataset.setncattr("external_variables", "cell_area")
+
+        # run the check
+        results = self.cf.check_cell_measures(dataset)
+        score, out_of, messages = get_results(results)
+        assert score > 0
+        assert score == out_of
+
+        # Non-string external variables, just treat as empty
+        dataset.setncattr("external_variables", 1)
+        results = self.cf.check_cell_measures(dataset)
+        score, out_of, messages = get_results(results)
+        message = "Cell measure variable cell_area referred to by PS is not present in dataset or external variables"
 
         # now test a dataset with a poorly formatted cell_measure attr
         dataset = self.load_dataset(STATIC_FILES["bad_cell_measure1"])
         results = self.cf.check_cell_measures(dataset)
         score, out_of, messages = get_results(results)
-        message = (
-            "The cell_measures attribute for variable PS is formatted incorrectly.  "
+        expected_message = (
+            "The cell_measures attribute for variable PS is formatted incorrectly. "
             "It should take the form of either 'area: cell_var' or 'volume: cell_var' "
-            "where cell_var is the variable describing the cell measures"
+            "where cell_var is an existing name of a variable describing the cell measures."
         )
-        assert message in messages
+        assert expected_message in messages
 
         # test a dataset where the cell_measure attr is not in the dataset or external_variables
         # check for the variable should fail
         dataset = self.load_dataset(STATIC_FILES["bad_cell_measure2"])
         results = self.cf.check_cell_measures(dataset)
         score, out_of, messages = get_results(results)
-        message = "Cell measure variable box_area referred to by PS is not present in dataset variables"
+        message = "Cell measure variable box_area referred to by PS is not present in dataset or external variables"
         assert message in messages
 
     def test_variable_features(self):
         with MockTimeSeries() as dataset:
             # I hope to never see an attribute value like this, but since
             # it's case insensitive, it still should work
             dataset.featureType = "tImEsERiEs"
@@ -1923,41 +2252,41 @@
                     'projected_crs', 'vertical_crs', 'compound_crs', 'conversion', 'grid_transformation',
                     'helmert_transformation', 'other_transformation', 'concatenated_operation')),
             auth_name TEXT NOT NULL CHECK (length(auth_name) >= 1),
             code TEXT NOT NULL CHECK (length(code) >= 1),
             alt_name TEXT NOT NULL CHECK (length(alt_name) >= 2),
             source TEXT
         );
-        """
+        """,
         )
         cur.execute(
             """
         CREATE TABLE vertical_datum (
             auth_name TEXT NOT NULL CHECK (length(auth_name) >= 1),
             code TEXT NOT NULL CHECK (length(code) >= 1),
             name TEXT NOT NULL CHECK (length(name) >= 2),
             description TEXT,
             scope TEXT,
             area_of_use_auth_name TEXT NOT NULL,
             area_of_use_code TEXT NOT NULL,
             deprecated BOOLEAN NOT NULL CHECK (deprecated IN (0, 1)),
             CONSTRAINT pk_vertical_datum PRIMARY KEY (auth_name, code)
         );
-        """
+        """,
         )
         cur.execute(
             """INSERT INTO alias_name VALUES
                        ('vertical_datum', 'EPSG', '5103', 'NAVD88', 'EPSG');
-                    """
+                    """,
         )
 
         cur.execute(
             """INSERT INTO vertical_datum VALUES
                     ('EPSG', '5101', 'Ordnance Datum Newlyn', NULL, NULL,
-                     'EPSG', '2792', '0')"""
+                     'EPSG', '2792', '0')""",
         )
 
         cur.close()
 
         self.assertTrue(self.cf._process_v_datum_str("NAVD88", conn))
         self.assertTrue(self.cf._process_v_datum_str("Ordnance Datum Newlyn", conn))
         # NAD83 isn't a vertical datum to begin with, expect failure
@@ -2003,15 +2332,15 @@
         # without false_easting warning in current file
         msg_len = len(
             [
                 m
                 for m in messages
                 if m
                 != "false_easting is a required attribute for grid mapping stereographic"
-            ]
+            ],
         )
         self.assertEqual(msg_len, 0)
 
     def test_check_grid_mapping_coordinates(self):
         """
         Checks that coordinates variables referred to by a grid mapping
         are well-formed and exist.
@@ -2114,22 +2443,22 @@
         # For each of the listed dimensionless vertical coordinates,
         # verify that the formula_terms match the provided set of terms
         self.assertTrue(
             no_missing_terms(
                 "ocean_s_coordinate_g1",
                 {"s", "C", "eta", "depth", "depth_c"},
                 dimless_vertical_coordinates_1_7,
-            )
+            ),
         )
         self.assertTrue(
             no_missing_terms(
                 "ocean_s_coordinate_g2",
                 {"s", "C", "eta", "depth", "depth_c"},
                 dimless_vertical_coordinates_1_7,
-            )
+            ),
         )
 
     def test_check_dimensionless_vertical_coordinate_1_7(self):
         """
         Unit test for _check_dimensionless_vertical_coordinate_1_7 method.
         """
         # IMPLEMENTATION 3.1 Recommended
@@ -2137,18 +2466,20 @@
 
         ret_val = []
 
         # create mock dataset for test; create three variables, one as dimensionless
         with MockTimeSeries() as dataset:
             dataset.createVariable("lev", "d")  # dtype=double, dims=1
             dataset.variables["lev"].setncattr(
-                "standard_name", "atmosphere_sigma_coordinate"
+                "standard_name",
+                "atmosphere_sigma_coordinate",
             )
             dataset.variables["lev"].setncattr(
-                "formula_terms", "sigma: lev ps: PS ptop: PTOP"
+                "formula_terms",
+                "sigma: lev ps: PS ptop: PTOP",
             )
 
             dataset.createVariable("PS", "d", ("time",))  # dtype=double, dims=time
             dataset.createVariable("PTOP", "d", ("time",))  # dtype=double, dims=time
 
             # run the check
             self.cf._check_dimensionless_vertical_coordinate_1_7(
@@ -2157,16 +2488,15 @@
                 deprecated_units,
                 ret_val,
                 dimless_vertical_coordinates_1_7,
             )
 
             # one should have failed, as no computed_standard_name is assigned
             score, out_of, messages = get_results(ret_val)
-            assert score == 0
-            assert out_of == 1
+            assert score < out_of
 
             # this time, assign computed_standard_name
             ret_val = []
             dataset.variables["lev"].setncattr("computed_standard_name", "air_pressure")
 
             # run the check
             self.cf._check_dimensionless_vertical_coordinate_1_7(
@@ -2203,56 +2533,73 @@
         results = self.cf.check_dimensionless_vertical_coordinates(dataset)
         scored, out_of, messages = get_results(results)
 
         assert len(results) == 3
         assert scored < out_of
         assert all(r.name == "§4.3 Vertical Coordinate" for r in results)
 
+        # TEST CONFORMANCE 4.3.3 REQUIRED
+        del dataset.variables["lev"].formula_terms
+        results = self.cf.check_dimensionless_vertical_coordinates(dataset)
+
+        # FIXME: get_results messages variable doesn't return message here
+        assert (
+            "Variable lev should have formula_terms attribute when "
+            "computed_standard_name attribute is defined" in results[-1].msgs
+        )
+
     def test_check_attr_type(self):
         """
         Ensure the _check_attr_type method works as expected.
         """
 
         # create a temporary variable and test this only
         nc_obj = MockTimeSeries()
         nc_obj.createVariable("temperature", "d", ("time",))
-        nc_obj.variables["temperature"].setncattr("test_att", np.float64(45))
         att_name = "test_att"
         _var = nc_obj.variables["temperature"]
 
         # first, test all valid checks show that it's valid
-        attr = "my_attr_value"  # string
+        _var.test_att = "my_attr_value"  # string
         attr_type = "S"
-        result = self.cf._check_attr_type(att_name, attr_type, attr)
+        result = self.cf._check_attr_type(att_name, attr_type, _var.test_att)
         self.assertTrue(result[0])
 
-        attr = np.int64(1)
+        _var.test_att = np.int8(1)
         attr_type = "N"
-        self.assertTrue(self.cf._check_attr_type(att_name, attr_type, attr)[0])
+        self.assertTrue(self.cf._check_attr_type(att_name, attr_type, _var.test_att)[0])
 
-        attr = np.float64(45)
+        _var.test_att = np.float64(45)
         attr_type = "D"
-        self.assertTrue(self.cf._check_attr_type(att_name, attr_type, attr, _var)[0])
+        self.assertTrue(
+            self.cf._check_attr_type(att_name, attr_type, _var.test_att, _var)[0],
+        )
 
         # check failures
-        attr = "my_attr_value"
+        _var.test_att = "my_attr_value"
         attr_type = "N"  # should be numeric
-        self.assertFalse(self.cf._check_attr_type(att_name, attr_type, attr)[0])
+        self.assertFalse(
+            self.cf._check_attr_type(att_name, attr_type, _var.test_att)[0],
+        )
 
-        attr = np.int(64)
+        _var.test_att = np.int8(64)
         attr_type = "S"  # should be string
-        self.assertFalse(self.cf._check_attr_type(att_name, attr_type, attr)[0])
+        self.assertFalse(
+            self.cf._check_attr_type(att_name, attr_type, _var.test_att)[0],
+        )
 
         nc_obj = MockTimeSeries()
         nc_obj.createVariable("temperature", "d", ("time",))
-        nc_obj.variables["temperature"].setncattr("test_att", np.int32(45))
+        nc_obj.variables["temperature"].setncattr("test_att", 45)
         _var = nc_obj.variables["temperature"]
-        attr = np.int32(45)
+        _var.test_att = np.int8(45)
         attr_type = "D"  # should match
-        self.assertFalse(self.cf._check_attr_type(att_name, attr_type, attr, _var)[0])
+        self.assertFalse(
+            self.cf._check_attr_type(att_name, attr_type, _var.test_att, _var)[0],
+        )
 
     def test_check_grid_mapping_attr_condition(self):
         """
         Ensure the CF-1.7 implementation of _check_grid_mapping_attr_condition()
         works as expected.
         """
 
@@ -2364,70 +2711,69 @@
         # create mock dataset for test; create three variables, one as dimensionless
 
         # test good (either-or)
         dataset = MockTimeSeries()
         dataset.createVariable("lev", "d")  # dtype=double, dims=1
         dataset.variables["lev"].setncattr("geoid_name", "blah")
         res = self.cf._check_gmattr_existence_condition_geoid_name_geoptl_datum_name(
-            dataset.variables["lev"]
+            dataset.variables["lev"],
         )
         self.assertTrue(res[0])
         dataset.close()
 
         dataset = MockTimeSeries()
         dataset.createVariable("lev", "d")  # dtype=double, dims=1
         dataset.variables["lev"].setncattr("geopotential_datum_name", "blah")
         res = self.cf._check_gmattr_existence_condition_geoid_name_geoptl_datum_name(
-            dataset.variables["lev"]
+            dataset.variables["lev"],
         )
         self.assertTrue(res[0])
         dataset.close()
 
         # bad
         dataset = MockTimeSeries()
         dataset.createVariable("lev", "d")  # dtype=double, dims=1
         dataset.variables["lev"].setncattr("geopotential_datum_name", "blah")
         dataset.variables["lev"].setncattr("geoid_name", "blah")
         res = self.cf._check_gmattr_existence_condition_geoid_name_geoptl_datum_name(
-            dataset.variables["lev"]
+            dataset.variables["lev"],
         )
         self.assertFalse(res[0])
         dataset.close()
 
     def test_check_gmattr_existence_condition_ell_pmerid_hdatum(self):
-
         # test good (all)
         dataset = MockTimeSeries()
         dataset.createVariable("lev", "d")  # dtype=double, dims=1
         dataset.variables["lev"].setncattr("reference_ellipsoid_name", "blah")
         dataset.variables["lev"].setncattr("prime_meridian_name", "blah")
         dataset.variables["lev"].setncattr("horizontal_datum_name", "blah")
         res = self.cf._check_gmattr_existence_condition_ell_pmerid_hdatum(
-            dataset.variables["lev"]
+            dataset.variables["lev"],
         )
         self.assertTrue(res[0])
         dataset.close()
 
         # test bad (not all)
         dataset = MockTimeSeries()
         dataset.createVariable("lev", "d")  # dtype=double, dims=1
         dataset.variables["lev"].setncattr("reference_ellipsoid_name", "blah")
         res = self.cf._check_gmattr_existence_condition_ell_pmerid_hdatum(
-            dataset.variables["lev"]
+            dataset.variables["lev"],
         )
         self.assertFalse(res[0])
         dataset.close()
 
         # test bad (not all)
         dataset = MockTimeSeries()
         dataset.createVariable("lev", "d")  # dtype=double, dims=1
         dataset.variables["lev"].setncattr("reference_ellipsoid_name", "blah")
         dataset.variables["lev"].setncattr("prime_meridian_name", "blah")
         res = self.cf._check_gmattr_existence_condition_ell_pmerid_hdatum(
-            dataset.variables["lev"]
+            dataset.variables["lev"],
         )
         self.assertFalse(res[0])
         dataset.close()
 
     def test_check_add_offset_scale_factor_type(self):
         dataset = MockTimeSeries()  # time lat lon depth
         temp = dataset.createVariable("temp", "d", dimensions=("time",))
@@ -2447,43 +2793,45 @@
 
         # set bad np val
         temp.setncattr("scale_factor", np.float32(5))
         r = self.cf.check_add_offset_scale_factor_type(dataset)
         self.assertFalse(r[1].value)
         self.assertTrue(r[1].msgs)
 
-        temp.setncattr("scale_factor", np.uint(5))
+        temp.setncattr("scale_factor", np.uint32(5))
         r = self.cf.check_add_offset_scale_factor_type(dataset)
         self.assertFalse(r[1].value)
         self.assertTrue(r[1].msgs)
 
         # set good
-        temp.setncattr("scale_factor", np.float(5))
+        temp.setncattr("scale_factor", float(5))
         r = self.cf.check_add_offset_scale_factor_type(dataset)
         self.assertTrue(r[1].value)
         self.assertFalse(r[1].msgs)
 
         temp.setncattr("scale_factor", np.double(5))
         r = self.cf.check_add_offset_scale_factor_type(dataset)
         self.assertTrue(r[1].value)
         self.assertFalse(r[1].msgs)
 
         # set same dtype
         dataset = MockTimeSeries()  # time lat lon depth
-        temp = dataset.createVariable("temp", np.int, dimensions=("time",))
-        temp.setncattr("scale_factor", np.int(5))
+        temp = dataset.createVariable("temp", int, dimensions=("time",))
+        temp.setncattr("scale_factor", int(5))
         r = self.cf.check_add_offset_scale_factor_type(dataset)
         self.assertTrue(r[1].value)
         self.assertFalse(r[1].msgs)
 
         # integer variable type (int8, int16, int32) compared against
         # floating point add_offset/scale_factor
         for var_bytes in ("1", "2", "4"):
             coarse_temp = dataset.createVariable(
-                f"coarse_temp_{var_bytes}", f"i{var_bytes}", dimensions=("time",)
+                f"coarse_temp_{var_bytes}",
+                f"i{var_bytes}",
+                dimensions=("time",),
             )
             coarse_temp.setncattr("scale_factor", np.float32(23.0))
             coarse_temp.setncattr("add_offset", np.double(-2.1))
             r = self.cf.check_add_offset_scale_factor_type(dataset)
             # First value which checks if add_offset and scale_factor
             # are same type should be false
             self.assertFalse(r[0].value)
@@ -2501,14 +2849,28 @@
             del dataset.variables[f"coarse_temp_{var_bytes}"]
 
 
 class TestCF1_8(BaseTestCase):
     def setUp(self):
         self.cf = CF1_8Check()
 
+    def test_groups(self):
+        dataset = MockTimeSeries()
+        # TEST CONFORMANCE 2.7 REQUIRED 1/4
+        nonroot_group = dataset.createGroup("nonroot")
+        nonroot_group.setncattr("Conventions", "CF-1.8")
+        nonroot_group.setncattr("external_variables", "ext1")
+        results = self.cf.check_groups(dataset)
+        bad_msg_template = '§2.7.2 Attribute "{}" MAY ONLY be used in the root group and SHALL NOT be duplicated or overridden in child groups.'
+        bad_messages = {
+            bad_msg_template.format(attr_name)
+            for attr_name in ["Conventions", "external_variables"]
+        }
+        assert bad_messages == set(results[0].msgs)
+
     def test_point_geometry_simple(self):
         dataset = MockTimeSeries()
         fake_data = dataset.createVariable("someData", "f8", ("time",))
         fake_data.geometry = "geometry"
         x = dataset.createVariable("x", "f8", ())
         y = dataset.createVariable("y", "f8", ())
         geom_var = dataset.createVariable("geometry", "i4", ())
@@ -2544,15 +2906,15 @@
         dataset = self.load_dataset(STATIC_FILES["line_geometry"])
         self.cf.check_geometry(dataset)
 
     def test_polygon_geometry(self):
         dataset = self.load_dataset(STATIC_FILES["polygon_geometry"])
         self.cf.check_geometry(dataset)
         dataset.variables["interior_ring"] = MockVariable(
-            dataset.variables["interior_ring"]
+            dataset.variables["interior_ring"],
         )
         # Flip sign indicator for interior rings.  Should cause failure
         flip_ring_bits = (dataset.variables["interior_ring"][:] == 0).astype(int)
         dataset.variables["interior_ring"][:] = flip_ring_bits
         results = self.cf.check_geometry(dataset)
         # There should be messages regarding improper polygon order
         assert results[0].value[0] < results[0].value[1]
@@ -2591,28 +2953,28 @@
             assert results[0].value[0] < results[0].value[1]
             assert len(messages) == 1
             taxon_lsid[
                 0
             ] = "http://www.lsid.info/urn:lsid:marinespecies.org:taxname:99999999999"
             results = self.cf.check_taxa(dataset)
             assert messages[0].startswith(
-                "Taxon id must match one of the following forms:"
+                "Taxon id must match one of the following forms:",
             )
             assert results[0].value[0] < results[0].value[1]
 
     def test_taxonomy_data_worms_valid(self):
         """
         Tests taxonomy data with a mocked pyworms call
         """
         with requests_mock.Mocker() as m:
             # assume LSID lookups for WoRMS return valid HTTP status code
             m.get(
                 re.compile(
-                    r"^http://www.lsid.info/urn:lsid:marinespecies.org:taxname:\d+$"
-                )
+                    r"^http://www.lsid.info/urn:lsid:marinespecies.org:taxname:\d+$",
+                ),
             )
             response_1 = json.dumps(
                 {
                     "AphiaID": 104464,
                     "url": "http://www.marinespecies.org/aphia.php?p=taxdetails&id=104464",
                     "scientificname": "Calanus finmarchicus",
                     "authority": "(Gunnerus, 1770)",
@@ -2635,15 +2997,15 @@
                     "isMarine": 1,
                     "isBrackish": 0,
                     "isFreshwater": 0,
                     "isTerrestrial": 0,
                     "isExtinct": None,
                     "match_type": "exact",
                     "modified": "2020-10-06T15:25:25.040Z",
-                }
+                },
             )
             m.get(
                 "http://www.marinespecies.org/rest/AphiaRecordByAphiaID/104464",
                 text=response_1,
             )
             response_2 = json.dumps(
                 {
@@ -2670,15 +3032,15 @@
                     "isMarine": 1,
                     "isBrackish": 0,
                     "isFreshwater": 0,
                     "isTerrestrial": 0,
                     "isExtinct": None,
                     "match_type": "exact",
                     "modified": "2004-12-21T15:54:05Z",
-                }
+                },
             )
             m.get(
                 "http://www.marinespecies.org/rest/AphiaRecordByAphiaID/104466",
                 text=response_2,
             )
             dataset = self.load_dataset(STATIC_FILES["taxonomy_example"])
 
@@ -2722,15 +3084,15 @@
             # try non-matching name
             taxon_name[0] = "Morone saxitilis"
             results = self.cf.check_taxa(dataset)
             result = results[0]
             assert result.msgs == [
                 "Supplied taxon name and ITIS scientific name do not match. "
                 "Supplied taxon name is 'Morone saxitilis', ITIS scientific name "
-                "for TSN 162139 is 'Esox lucius.'"
+                "for TSN 162139 is 'Esox lucius.'",
             ]
 
     def test_taxonomy_skip_lsid(self):
         """
         Tests that nodata/unset LSID values are skipped for validation
         """
         dataset = MockTimeSeries()
@@ -2770,326 +3132,476 @@
         fake_str = "No check"
         taxon_name[0] = stringtoarr(fake_str, 80)
         results = self.cf.check_taxa(dataset)
         assert len(results[0].msgs) == 0
         assert results[0].value[0] == results[0].value[1]
 
 
+class TestCF1_9(BaseTestCase):
+    def setUp(self):
+        self.cf = CF1_9Check()
+
+    def test_check_data_types(self):
+        """Check the unsigned int datatypes for variables CF 1.9 added"""
+        dataset = MockTimeSeries()
+        for bytes_count in [1, 2, 4, 8]:
+            dataset.createVariable(f"var_{bytes_count}_ubytes", f"u{bytes_count}", ())
+
+        result = self.cf.check_data_types(dataset)
+        assert result.value[0] == result.value[1]
+
+    def test_time_variable_over_sixty_seconds(self):
+        dataset = MockTimeSeries()
+        # TEST CF CONFORMANCE 4.4 REQUIRED
+        dataset.variables["time"].units = "months since 0-1-1 23:00:60"
+        results = self.cf.check_time_coordinate(dataset)
+        scored, out_of, messages = get_results(results)
+        assert (
+            'Time coordinate variable "time" must have units with seconds less than 60'
+            in messages
+        )
+
+    def test_time_variable_has_calendar(self):
+        self.cf = CF1_9Check()
+        # TEST CONFORMANCE 4.4.1 RECOMMENDED CF 1.9
+        dataset = MockTimeSeries()
+        del dataset.variables["time"].calendar
+        results = self.cf.check_time_coordinate_variable_has_calendar(dataset)
+        scored, out_of, messages = get_results(results)
+        assert (
+            'Time coordinate variable "time" should have a string valued attribute "calendar"'
+            in messages
+        )
+        # FIXME: NetCDF files shouldn't normally be modified so we can usually
+        # depend on cached results. Here we need to recreate the checker
+        # instance in order to not have previous results included pass condition
+        dataset.variables["time"].calendar = "standard"
+        results = self.cf.check_calendar(dataset)
+        # no time coordinate present, i.e. there is no time variable name with
+        # the same name as the time dimension name.
+        self.cf = CF1_9Check()
+        # need to manually construct the netCDF object here --
+        # get_variables_by_attributes appears to be interfering here
+        dataset = MockNetCDF()
+        dataset.createDimension("time", 500)
+        dataset.createVariable("time2", "f8", ("time",))
+        dataset.variables["time2"].standard_name = "time"
+        dataset.variables["time2"].units = "seconds since 1970-01-01 00:00:00"
+        dataset.variables["time2"].axis = "T"
+        results = self.cf.check_calendar(dataset)
+        # results array should be empty as no time coordinate variable detected
+        assert not results
+
+        # TEST CONFORMANCE 4.4.1
+        dataset = MockTimeSeries()
+        dataset.variables["time"].units = "months since 0-1-1 23:00:60"
+        results = self.cf.check_calendar(dataset)
+        scored, out_of, messages = get_results(results)
+
+        # test greater than or equal to one zero year for Julian and Gregorian
+        # calendars
+        dataset = MockTimeSeries()
+        dataset.variables["time"].units = "seconds since 0-01-01 00:00:00"
+        for calendar_name in ("standard", "julian", "gregorian"):
+            dataset.variables["time"].calendar = calendar_name
+            results = self.cf.check_time_coordinate_variable_has_calendar(dataset)
+            scored, out_of, messages = get_results(results)
+            assert (
+                'For time variable "time", when using the Gregorian or Julian '
+                "calendars, the use of year zero is not recommended. "
+                "Furthermore, the use of year zero to signify a climatological "
+                "variable as in COARDS is deprecated in CF." in messages
+            )
+
+    def test_domain(self):
+        dataset = MockTimeSeries()
+        domain_var = dataset.createVariable("domain", "c", ())
+        domain_var.long_name = "Domain variable"
+        domain_var.coordinates = "lon lat depth"
+        results = self.cf.check_domain_variables(dataset)
+        self.assertEqual(results[0].value[0], results[0].value[1])
+        self.assertFalse(results[0].msgs)
+
+        # missing long_name attribute
+        del domain_var.long_name
+        results = self.cf.check_domain_variables(dataset)
+        self.assertNotEqual(results[0].value[0], results[0].value[1])
+        self.assertTrue(results[0].msgs)
+        self.assertTrue(
+            results[0].msgs[0]
+            == "For domain variable domain it is recommended that attribute long_name be present and a string",
+        )
+
+        # bad coordinates variable
+        domain_var.coordinates = "lon lat depth xyxz abc"
+        domain_var.long_name = "Domain variable"
+        results = self.cf.check_domain_variables(dataset)
+        self.assertNotEqual(results[0].value[0], results[0].value[1])
+        self.assertTrue(
+            results[0].msgs[0]
+            == "Could not find the following variables referenced in "
+            "coordinates attribute from domain variable domain: "
+            "xyxz, abc",
+        )
+
+        del dataset
+        dataset = MockTimeSeries()
+        # domain should be dimensionless -- currently not an error in
+        # compliance checker, but not detected as a domain variable either
+        domain_var = dataset.createVariable("domain", "c", ("time",))
+        domain_var.long_name = "Domain variable"
+        domain_var.coordinates = "lon lat depth"
+        results = self.cf.check_domain_variables(dataset)
+        assert len(results) == 0
+
+
 class TestCFUtil(BaseTestCase):
     """
     Class to test the cfutil module.
     """
 
     def test_is_variable_valid_ragged_array_repr_featureType(self):
         nc = MockRaggedArrayRepr("timeseries", "indexed")
 
         # add a variable that isn't recognized as geophysical
         v = nc.createVariable("data1", "d", ("SAMPLE_DIMENSION",), fill_value=None)
         v.setncattr("cf_role", "blah")
         self.assertFalse(
-            cfutil.is_variable_valid_ragged_array_repr_featureType(nc, "data1")
+            cfutil.is_variable_valid_ragged_array_repr_featureType(nc, "data1"),
         )
 
         # add geophysical variable with correct dimension
         nc = MockRaggedArrayRepr("timeseries", "indexed")
         v = nc.createVariable("data1", "d", ("SAMPLE_DIMENSION",), fill_value=None)
         v.setncattr("standard_name", "sea_water_pressure")
         # test the variable
         self.assertTrue(
-            cfutil.is_variable_valid_ragged_array_repr_featureType(nc, "data1")
+            cfutil.is_variable_valid_ragged_array_repr_featureType(nc, "data1"),
         )
 
         # add good variable and another variable, this time with the improper dimension
         nc = MockRaggedArrayRepr("timeseries", "indexed")
         v = nc.createVariable("data1", "d", ("SAMPLE_DIMENSION",), fill_value=None)
         v.setncattr("standard_name", "sea_water_pressure")
         v2 = nc.createVariable("data2", "d", ("INSTANCE_DIMENSION",), fill_value=None)
         v2.setncattr("standard_name", "sea_water_salinity")
 
         # good variable should pass, second should fail
         self.assertTrue(
-            cfutil.is_variable_valid_ragged_array_repr_featureType(nc, "data1")
+            cfutil.is_variable_valid_ragged_array_repr_featureType(nc, "data1"),
         )
         self.assertFalse(
-            cfutil.is_variable_valid_ragged_array_repr_featureType(nc, "data2")
+            cfutil.is_variable_valid_ragged_array_repr_featureType(nc, "data2"),
         )
 
     def test_is_dataset_valid_ragged_array_repr_featureType(self):
-
         # first test single featureType
 
         # ----- timeseries, indexed ----- #
 
         nc = MockRaggedArrayRepr("timeseries", "indexed")
         self.assertTrue(
-            cfutil.is_dataset_valid_ragged_array_repr_featureType(nc, "timeseries")
+            cfutil.is_dataset_valid_ragged_array_repr_featureType(nc, "timeseries"),
         )
 
         # we'll add another cf_role variable
         nc = MockRaggedArrayRepr("timeseries", "indexed")
         v = nc.createVariable("var2", "i", ("INSTANCE_DIMENSION",), fill_value=None)
         v.setncattr("cf_role", "yeetyeet_id")
         self.assertFalse(
-            cfutil.is_dataset_valid_ragged_array_repr_featureType(nc, "timeseries")
+            cfutil.is_dataset_valid_ragged_array_repr_featureType(nc, "timeseries"),
         )
 
         # we'll add another index variable, also bad
         nc = MockRaggedArrayRepr("timeseries", "indexed")
         v = nc.createVariable("index_var2", "i", ("SAMPLE_DIMENSION",), fill_value=None)
         v.setncattr("instance_dimension", "INSTANCE_DIMENSION")
         self.assertFalse(
-            cfutil.is_dataset_valid_ragged_array_repr_featureType(nc, "timeseries")
+            cfutil.is_dataset_valid_ragged_array_repr_featureType(nc, "timeseries"),
         )
 
         # ----- timeseries, contiguous ----- #
         nc = MockRaggedArrayRepr("timeseries", "contiguous")
         self.assertTrue(
-            cfutil.is_dataset_valid_ragged_array_repr_featureType(nc, "timeseries")
+            cfutil.is_dataset_valid_ragged_array_repr_featureType(nc, "timeseries"),
         )
 
         # add another cf_role var, bad
         nc = MockRaggedArrayRepr("timeseries", "contiguous")
         v = nc.createVariable("var2", "i", ("INSTANCE_DIMENSION",), fill_value=None)
         v.setncattr("cf_role", "yeetyeet_id")
         self.assertFalse(
-            cfutil.is_dataset_valid_ragged_array_repr_featureType(nc, "timeseries")
+            cfutil.is_dataset_valid_ragged_array_repr_featureType(nc, "timeseries"),
         )
 
         # add another count variable, bad
         v = nc.createVariable(
-            "count_var2", "i", ("INSTANCE_DIMENSION",), fill_value=None
+            "count_var2",
+            "i",
+            ("INSTANCE_DIMENSION",),
+            fill_value=None,
         )
         v.setncattr("sample_dimension", "SAMPLE_DIMENSION")
         self.assertFalse(
-            cfutil.is_dataset_valid_ragged_array_repr_featureType(nc, "timeseries")
+            cfutil.is_dataset_valid_ragged_array_repr_featureType(nc, "timeseries"),
         )
 
         # ----- profile, indexed ----- #
 
         nc = MockRaggedArrayRepr("profile", "indexed")
         self.assertTrue(
-            cfutil.is_dataset_valid_ragged_array_repr_featureType(nc, "profile")
+            cfutil.is_dataset_valid_ragged_array_repr_featureType(nc, "profile"),
         )
 
         # add another cf_role var
         nc = MockRaggedArrayRepr("profile", "indexed")
         v = nc.createVariable("var2", "i", ("INSTANCE_DIMENSION",), fill_value=None)
         v.setncattr("cf_role", "yeetyeet_id")
         self.assertFalse(
-            cfutil.is_dataset_valid_ragged_array_repr_featureType(nc, "profile")
+            cfutil.is_dataset_valid_ragged_array_repr_featureType(nc, "profile"),
         )
 
         # we'll add another index variable, also bad
         nc = MockRaggedArrayRepr("profile", "indexed")
         v = nc.createVariable("index_var2", "i", ("SAMPLE_DIMENSION",), fill_value=None)
         v.setncattr("instance_dimension", "INSTANCE_DIMENSION")
         self.assertFalse(
-            cfutil.is_dataset_valid_ragged_array_repr_featureType(nc, "profile")
+            cfutil.is_dataset_valid_ragged_array_repr_featureType(nc, "profile"),
         )
 
         # ----- profile, contiguous ----- #
         nc = MockRaggedArrayRepr("profile", "contiguous")
         self.assertTrue(
-            cfutil.is_dataset_valid_ragged_array_repr_featureType(nc, "profile")
+            cfutil.is_dataset_valid_ragged_array_repr_featureType(nc, "profile"),
         )
 
         # add another cf_role var
         nc = MockRaggedArrayRepr("profile", "contiguous")
         v = nc.createVariable("var2", "i", ("INSTANCE_DIMENSION",), fill_value=None)
         v.setncattr("cf_role", "yeetyeet_id")
         self.assertFalse(
-            cfutil.is_dataset_valid_ragged_array_repr_featureType(nc, "profile")
+            cfutil.is_dataset_valid_ragged_array_repr_featureType(nc, "profile"),
         )
 
         # we'll add another count variable, also bad
         nc = MockRaggedArrayRepr("profile", "contiguous")
         v = nc.createVariable(
-            "index_var2", "i", ("INSTANCE_DIMENSION",), fill_value=None
+            "index_var2",
+            "i",
+            ("INSTANCE_DIMENSION",),
+            fill_value=None,
         )
         v.setncattr("sample_dimension", "SAMPLE_DIMENSION")
         self.assertFalse(
-            cfutil.is_dataset_valid_ragged_array_repr_featureType(nc, "profile")
+            cfutil.is_dataset_valid_ragged_array_repr_featureType(nc, "profile"),
         )
 
         # ----- trajectory, indexed ----- #
         nc = MockRaggedArrayRepr("trajectory", "indexed")
         self.assertTrue(
-            cfutil.is_dataset_valid_ragged_array_repr_featureType(nc, "trajectory")
+            cfutil.is_dataset_valid_ragged_array_repr_featureType(nc, "trajectory"),
         )
 
         # add another cf_role var
         nc = MockRaggedArrayRepr("trajectory", "indexed")
         v = nc.createVariable("var2", "i", ("INSTANCE_DIMENSION",), fill_value=None)
         v.setncattr("cf_role", "yeetyeet_id")
         self.assertFalse(
-            cfutil.is_dataset_valid_ragged_array_repr_featureType(nc, "trajectory")
+            cfutil.is_dataset_valid_ragged_array_repr_featureType(nc, "trajectory"),
         )
 
         # we'll add another index variable, also bad
         nc = MockRaggedArrayRepr("trajectory", "indexed")
         v = nc.createVariable("index_var2", "i", ("SAMPLE_DIMENSION",), fill_value=None)
         v.setncattr("instance_dimension", "INSTANCE_DIMENSION")
         self.assertFalse(
-            cfutil.is_dataset_valid_ragged_array_repr_featureType(nc, "trajectory")
+            cfutil.is_dataset_valid_ragged_array_repr_featureType(nc, "trajectory"),
         )
 
         # ----- trajectory, contiguous ----- #
         nc = MockRaggedArrayRepr("trajectory", "contiguous")
         self.assertTrue(
-            cfutil.is_dataset_valid_ragged_array_repr_featureType(nc, "trajectory")
+            cfutil.is_dataset_valid_ragged_array_repr_featureType(nc, "trajectory"),
         )
 
         # add another cf_role var
         nc = MockRaggedArrayRepr("trajectory", "contiguous")
         v = nc.createVariable("var2", "i", ("INSTANCE_DIMENSION",), fill_value=None)
         v.setncattr("cf_role", "yeetyeet_id")
         self.assertFalse(
-            cfutil.is_dataset_valid_ragged_array_repr_featureType(nc, "trajectory")
+            cfutil.is_dataset_valid_ragged_array_repr_featureType(nc, "trajectory"),
         )
 
         # we'll add another count variable, also bad
         nc = MockRaggedArrayRepr("trajectory", "contiguous")
         v = nc.createVariable(
-            "index_var2", "i", ("INSTANCE_DIMENSION",), fill_value=None
+            "index_var2",
+            "i",
+            ("INSTANCE_DIMENSION",),
+            fill_value=None,
         )
         v.setncattr("sample_dimension", "SAMPLE_DIMENSION")
         self.assertFalse(
-            cfutil.is_dataset_valid_ragged_array_repr_featureType(nc, "trajectory")
+            cfutil.is_dataset_valid_ragged_array_repr_featureType(nc, "trajectory"),
         )
 
         # ----- now test compound featureType ----- #
 
         # ----- timeSeriesProfile ----- #
         nc = MockRaggedArrayRepr("timeSeriesProfile")
 
         # NOTE
         # has no geophysical vars, so should (?) (will) fail
         self.assertFalse(
             cfutil.is_dataset_valid_ragged_array_repr_featureType(
-                nc, "timeseriesprofile"
-            )
+                nc,
+                "timeseriesprofile",
+            ),
         )
 
         # add a geophysical variable and test again
         nc = MockRaggedArrayRepr("timeSeriesProfile")
         v1 = nc.createVariable("data1", "i", ("SAMPLE_DIMENSION",), fill_value=None)
         v1.setncattr("standard_name", "pressure")
         self.assertTrue(
             cfutil.is_dataset_valid_ragged_array_repr_featureType(
-                nc, "timeseriesprofile"
-            )
+                nc,
+                "timeseriesprofile",
+            ),
         )
 
         nc = MockRaggedArrayRepr("timeSeriesProfile")
         v1 = nc.createVariable("data1", "i", ("SAMPLE_DIMENSION",), fill_value=None)
         # add a third cf_role variable - this should fail
         v = nc.createVariable(
-            "cf_role_var3", "i", ("INSTANCE_DIMENSION",), fill_value=None
+            "cf_role_var3",
+            "i",
+            ("INSTANCE_DIMENSION",),
+            fill_value=None,
         )
         v.setncattr("cf_role", "yeetyeet_id")
         self.assertFalse(
             cfutil.is_dataset_valid_ragged_array_repr_featureType(
-                nc, "timeseriesprofile"
-            )
+                nc,
+                "timeseriesprofile",
+            ),
         )
 
         # set the index variable to have an incorrect attr
         nc = MockRaggedArrayRepr("timeSeriesProfile")
         v1 = nc.createVariable("data1", "i", ("SAMPLE_DIMENSION",), fill_value=None)
         nc.variables["station_index_variable"].instance_dimension = "SIKE!"
 
         self.assertFalse(
             cfutil.is_dataset_valid_ragged_array_repr_featureType(
-                nc, "timeseriesprofile"
-            )
+                nc,
+                "timeseriesprofile",
+            ),
         )
 
         # change the sample_dimension attr on the count variable, bad
         nc = MockRaggedArrayRepr("timeSeriesProfile")
         v1 = nc.createVariable("data1", "i", ("SAMPLE_DIMENSION",), fill_value=None)
         nc.variables["counter_var"].sample_dimension = "SIKE!"
 
         self.assertFalse(
             cfutil.is_dataset_valid_ragged_array_repr_featureType(
-                nc, "timeseriesprofile"
-            )
+                nc,
+                "timeseriesprofile",
+            ),
         )
 
         # give another geophysical data variable a different dimension
         nc = MockRaggedArrayRepr("timeSeriesProfile")
         v1 = nc.createVariable("data1", "i", ("SAMPLE_DIMENSION",), fill_value=None)
         v1 = nc.createVariable(
-            "data2", "i", ("STATION_DIMENSION",), fill_value=None  # bad!
+            "data2",
+            "i",
+            ("STATION_DIMENSION",),
+            fill_value=None,  # bad!
         )
         self.assertFalse(
             cfutil.is_dataset_valid_ragged_array_repr_featureType(
-                nc, "timeseriesprofile"
-            )
+                nc,
+                "timeseriesprofile",
+            ),
         )
 
         # ----- trajectoryProfile ----- #
         nc = MockRaggedArrayRepr("trajectoryProfile")
 
         # NOTE
         # has no geophysical vars, so should (?) (will) fail
         self.assertFalse(
             cfutil.is_dataset_valid_ragged_array_repr_featureType(
-                nc, "trajectoryprofile"
-            )
+                nc,
+                "trajectoryprofile",
+            ),
         )
 
         # add a geophysical variable and test again
         nc = MockRaggedArrayRepr("trajectoryProfile")
         v1 = nc.createVariable("data1", "i", ("SAMPLE_DIMENSION",), fill_value=None)
         v1.setncattr("standard_name", "pressure")
         self.assertTrue(
             cfutil.is_dataset_valid_ragged_array_repr_featureType(
-                nc, "trajectoryprofile"
-            )
+                nc,
+                "trajectoryprofile",
+            ),
         )
 
         nc = MockRaggedArrayRepr("trajectoryProfile")
         v1 = nc.createVariable("data1", "i", ("SAMPLE_DIMENSION",), fill_value=None)
         # add a third cf_role variable - this should fail
         v = nc.createVariable(
-            "cf_role_var3", "i", ("INSTANCE_DIMENSION",), fill_value=None
+            "cf_role_var3",
+            "i",
+            ("INSTANCE_DIMENSION",),
+            fill_value=None,
         )
         v.setncattr("cf_role", "yeetyeet_id")
         self.assertFalse(
             cfutil.is_dataset_valid_ragged_array_repr_featureType(
-                nc, "trajectoryprofile"
-            )
+                nc,
+                "trajectoryprofile",
+            ),
         )
 
         # set the index variable to have an incorrect attr
         nc = MockRaggedArrayRepr("trajectoryProfile")
         v1 = nc.createVariable("data1", "i", ("SAMPLE_DIMENSION",), fill_value=None)
         nc.variables["station_index_variable"].instance_dimension = "SIKE!"
 
         self.assertFalse(
             cfutil.is_dataset_valid_ragged_array_repr_featureType(
-                nc, "trajectoryprofile"
-            )
+                nc,
+                "trajectoryprofile",
+            ),
         )
 
         # change the sample_dimension attr on the count variable, bad
         nc = MockRaggedArrayRepr("trajectoryProfile")
         v1 = nc.createVariable("data1", "i", ("SAMPLE_DIMENSION",), fill_value=None)
         nc.variables["counter_var"].sample_dimension = "SIKE!"
 
         self.assertFalse(
             cfutil.is_dataset_valid_ragged_array_repr_featureType(
-                nc, "trajectoryprofile"
-            )
+                nc,
+                "trajectoryprofile",
+            ),
         )
 
         # give another geophysical data variable a different dimension
         nc = MockRaggedArrayRepr("trajectoryProfile")
         v1 = nc.createVariable("data1", "i", ("SAMPLE_DIMENSION",), fill_value=None)
         v1 = nc.createVariable(
-            "data2", "i", ("STATION_DIMENSION",), fill_value=None  # bad!
+            "data2",
+            "i",
+            ("STATION_DIMENSION",),
+            fill_value=None,  # bad!
         )
         self.assertFalse(
             cfutil.is_dataset_valid_ragged_array_repr_featureType(
-                nc, "trajectoryprofile"
-            )
+                nc,
+                "trajectoryprofile",
+            ),
         )
```

### Comparing `compliance-checker-5.0.2/compliance_checker/tests/test_cf_integration.py` & `compliance-checker-5.1.0/compliance_checker/tests/test_cf_integration.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 #!/usr/bin/env python
-# -*- coding: utf-8 -*-
 
 import pytest
 
 from compliance_checker.cf import util
 
 # get current std names table version (it changes)
 std_names = util.StandardNameTable()
@@ -18,16 +17,16 @@
     (
         "sldmb_43093_agg",
         [
             "attribute time:_CoordianteAxisType should begin with a letter and be composed of letters, digits, and underscores",
             "attribute lat:_CoordianteAxisType should begin with a letter and be composed of letters, digits, and underscores",
             "attribute lon:_CoordianteAxisType should begin with a letter and be composed of letters, digits, and underscores",
             "§2.6.2 global attribute history should exist and be a non-empty string",
-            "standard_name temperature is not defined in Standard Name Table v{}".format(
-                std_names._version
+            "standard_name temperature is not defined in Standard Name Table v{}. Possible close match(es): ['air_temperature', 'soil_temperature', 'snow_temperature']".format(
+                std_names._version,
             ),
             "temperature's auxiliary coordinate specified by the coordinates attribute, precise_lat, is not a variable in this dataset",
             "temperature's auxiliary coordinate specified by the coordinates attribute, precise_lon, is not a variable in this dataset",
         ],
     ),
     (
         "usgs_dem_saipan",
@@ -42,37 +41,37 @@
             "Attribute 'valid_range' (type: <class 'numpy.int16'>) and parent variable 'wind_gust_qc' (type: <class 'numpy.int8'>) must have equivalent datatypes",
             "Attribute 'valid_range' (type: <class 'numpy.float64'>) and parent variable 'wind_speed' (type: <class 'numpy.float32'>) must have equivalent datatypes",
             "Attribute 'valid_range' (type: <class 'numpy.int16'>) and parent variable 'wind_speed_qc' (type: <class 'numpy.int8'>) must have equivalent datatypes",
             "Attribute 'valid_range' (type: <class 'numpy.float64'>) and parent variable 'wind_direction' (type: <class 'numpy.float32'>) must have equivalent datatypes",
             "Attribute 'valid_range' (type: <class 'numpy.int16'>) and parent variable 'wind_direction_qc' (type: <class 'numpy.int8'>) must have equivalent datatypes",
             "Attribute 'valid_range' (type: <class 'numpy.int16'>) and parent variable 'visibility_qc' (type: <class 'numpy.int8'>) must have equivalent datatypes",
             '§2.6.1 Conventions global attribute does not contain "CF-1.8"',
-            "standard_name visibility is not defined in Standard Name Table v{}".format(
-                std_names._version
+            "standard_name visibility is not defined in Standard Name Table v{}. Possible close match(es): ['visibility_in_air']".format(
+                std_names._version,
             ),
             'Standard name modifier "data_quality" for variable visibility_qc is not a valid modifier according to CF Appendix C',
-            "standard_name wind_direction is not defined in Standard Name Table v{}".format(
-                std_names._version
+            "standard_name wind_direction is not defined in Standard Name Table v{}. Possible close match(es): ['wind_to_direction', 'wind_from_direction', 'wind_gust_from_direction']".format(
+                std_names._version,
             ),
             'Standard name modifier "data_quality" for variable wind_direction_qc is not a valid modifier according to CF Appendix C',
-            "standard_name wind_gust is not defined in Standard Name Table v{}".format(
-                std_names._version
+            "standard_name wind_gust is not defined in Standard Name Table v{}. Possible close match(es): ['y_wind_gust', 'x_wind_gust', 'wind_speed_of_gust']".format(
+                std_names._version,
             ),
             'Standard name modifier "data_quality" for variable wind_gust_qc is not a valid modifier according to CF Appendix C',
             'Standard name modifier "data_quality" for variable air_temperature_qc is not a valid modifier according to CF Appendix C',
-            "standard_name use_wind is not defined in Standard Name Table v{}".format(
-                std_names._version
+            "standard_name use_wind is not defined in Standard Name Table v{}. Possible close match(es): ['y_wind', 'x_wind']".format(
+                std_names._version,
             ),
-            "standard_name barometric_pressure is not defined in Standard Name Table v{}".format(
-                std_names._version
+            "standard_name barometric_pressure is not defined in Standard Name Table v{}. Possible close match(es): ['air_pressure', 'reference_pressure', 'barometric_altitude']".format(
+                std_names._version,
             ),
             'Standard name modifier "data_quality" for variable barometric_pressure_qc is not a valid modifier according to CF Appendix C',
             'Standard name modifier "data_quality" for variable wind_speed_qc is not a valid modifier according to CF Appendix C',
-            "standard_name barometric_pressure is not defined in Standard Name Table v{}".format(
-                std_names._version
+            "standard_name barometric_pressure is not defined in Standard Name Table v{}. Possible close match(es): ['air_pressure', 'reference_pressure', 'barometric_altitude']".format(
+                std_names._version,
             ),
             "CF recommends latitude variable 'lat' to use units degrees_north",
             "CF recommends longitude variable 'lon' to use units degrees_east",
         ],
     ),
     ("sp041", ["lat_qc is not a variable in this dataset"]),
     (
@@ -148,19 +147,19 @@
         ],
     ),
     (
         "glcfs",
         [
             # TODO: referenced/relative time is treated like time units
             'Units "hours since 2016-01-01T12:00:00Z" for variable time_offset must be convertible to canonical units "s"',
-            "standard_name cloud_cover is not defined in Standard Name Table v{}".format(
-                std_names._version
+            "standard_name cloud_cover is not defined in Standard Name Table v{}. Possible close match(es): ['land_cover', 'land_cover_lccs', 'cloud_albedo']".format(
+                std_names._version,
             ),
-            "standard_name dew_point is not defined in Standard Name Table v{}".format(
-                std_names._version
+            "standard_name dew_point is not defined in Standard Name Table v{}. Possible close match(es): ['dew_point_depression', 'dew_point_temperature']".format(
+                std_names._version,
             ),
             (
                 "GRID is not a valid CF featureType. It must be one of point, timeseries, "
                 "trajectory, profile, timeseriesprofile, trajectoryprofile"
             ),
             (
                 "global attribute _CoordSysBuilder should begin with a letter and "
@@ -216,27 +215,29 @@
 
 mult_msgs_diff = "Failed to find the following messages:\n{missing_msgs}\n\n\
         These were the messages captured:\n{found_msgs}\n\
             Please check wording and section names if messages have been altered since this test was written"
 
 
 class TestCFIntegration:
-
     # --------------------------------------------------------------------------------
     # Helper Methods
     # --------------------------------------------------------------------------------
 
     def get_results(self, check_results, checksuite):
         """
         Returns a tuple of the value scored, possible, and a list of messages
         in the result set.\n
         cs: instance of CheckSuite object
         """
         aggregation = checksuite.build_structure(
-            "cf", check_results["cf"][0], "test", 1
+            "cf",
+            check_results["cf"][0],
+            "test",
+            1,
         )
         out_of = 0
         scored = 0
         results = aggregation["all_priorities"]
         for r in results:
             if isinstance(r.value, tuple):
                 out_of += r.value[1]
@@ -254,24 +255,24 @@
 
     # --------------------------------------------------------------------------------
 
     @pytest.mark.parametrize(
         "loaded_dataset,expected_messages",
         dataset_stem__expected_messages,
         indirect=[
-            "loaded_dataset"
+            "loaded_dataset",
         ],  # must be specified to load this param at runtime, instead of at collection
     )
     def test_cf_integration(self, loaded_dataset, expected_messages, cs):
         check_results = cs.run(loaded_dataset, [], "cf")
         scored, out_of, messages = self.get_results(check_results, cs)
 
         assert scored < out_of
 
-        assert all([m in messages for m in expected_messages]), mult_msgs_diff.format(
+        assert all(m in messages for m in expected_messages), mult_msgs_diff.format(
             missing_msgs="\n".join([m for m in expected_messages if m not in messages]),
             found_msgs="\n".join(messages),
         )
 
     @pytest.mark.parametrize(
         "loaded_dataset,wrong_message",
         # From Github issue #845:\n
@@ -302,15 +303,15 @@
             if msg.startswith("dimensions for auxiliary coordinate variable siglay"):
                 break
         # it's not clear to me what this is supposed to be doing -- this else clause is outside of the if
         else:
             raise AssertionError(
                 '"dimensions for auxiliary coordinate variable siglay (node, siglay) '
                 'are not a subset of dimensions for variable u (siglay, nele, time)"'
-                " not in messages"
+                " not in messages",
             )
         assert (
             '§2.6.1 Conventions global attribute does not contain "CF-1.8"'
         ) in messages
 
     @pytest.mark.parametrize(
         "loaded_dataset",
```

### Comparing `compliance-checker-5.0.2/compliance_checker/tests/test_cli.py` & `compliance-checker-5.1.0/compliance_checker/tests/test_cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 #!/usr/bin/env python
-# -*- coding: utf-8 -*-
 """
 Tests for command line output and parsing
 
 """
 import io
 import json
 import os
```

### Comparing `compliance-checker-5.0.2/compliance_checker/tests/test_feature_detection.py` & `compliance-checker-5.1.0/compliance_checker/tests/test_feature_detection.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 #!/usr/bin/env python
-# -*- coding: utf-8 -*-
 """
 compliance_checker/tests/test_feature_detection.py
 """
 
 from unittest import TestCase
 
 from netCDF4 import Dataset
@@ -20,209 +19,226 @@
 
     def test_point(self):
         """
         Ensures point detection works
         """
         with Dataset(resources.STATIC_FILES["point"]) as nc:
             for variable in util.get_geophysical_variables(nc):
-                assert util.is_point(nc, variable), "{} is point".format(variable)
+                assert util.is_point(nc, variable), f"{variable} is point"
 
     def test_timeseries(self):
         """
         Ensures timeseries detection works
         """
         with Dataset(resources.STATIC_FILES["timeseries"]) as nc:
             for variable in util.get_geophysical_variables(nc):
                 assert util.is_timeseries(nc, variable), "{} is timeseries".format(
-                    variable
+                    variable,
                 )
 
     def test_multi_timeseries_orthogonal(self):
         """
         Ensures multi-timeseries-orthogonal detection works
         """
         with Dataset(resources.STATIC_FILES["multi-timeseries-orthogonal"]) as nc:
             for variable in util.get_geophysical_variables(nc):
                 assert util.is_multi_timeseries_orthogonal(
-                    nc, variable
-                ), "{} is multi-timeseries orthogonal".format(variable)
+                    nc,
+                    variable,
+                ), f"{variable} is multi-timeseries orthogonal"
 
     def test_multi_timeseries_incomplete(self):
         """
         Ensures multi-timeseries-incomplete detection works
         """
         with Dataset(resources.STATIC_FILES["multi-timeseries-incomplete"]) as nc:
             for variable in util.get_geophysical_variables(nc):
                 assert util.is_multi_timeseries_incomplete(
-                    nc, variable
-                ), "{} is multi-timeseries incomplete".format(variable)
+                    nc,
+                    variable,
+                ), f"{variable} is multi-timeseries incomplete"
 
     def test_trajectory(self):
         """
         Ensures trajectory detection works
         """
         with Dataset(resources.STATIC_FILES["trajectory"]) as nc:
             for variable in util.get_geophysical_variables(nc):
                 assert util.is_cf_trajectory(nc, variable), "{} is trajectory".format(
-                    variable
+                    variable,
                 )
 
     def test_trajectory_single(self):
         """
         Ensures trajectory-single detection works
         """
         with Dataset(resources.STATIC_FILES["trajectory-single"]) as nc:
             for variable in util.get_geophysical_variables(nc):
                 assert util.is_single_trajectory(
-                    nc, variable
-                ), "{} is trajectory-single".format(variable)
+                    nc,
+                    variable,
+                ), f"{variable} is trajectory-single"
 
     def test_profile_orthogonal(self):
         """
         Ensures profile-orthogonal detection works
         """
         with Dataset(resources.STATIC_FILES["profile-orthogonal"]) as nc:
             for variable in util.get_geophysical_variables(nc):
                 assert util.is_profile_orthogonal(
-                    nc, variable
-                ), "{} is profile-orthogonal".format(variable)
+                    nc,
+                    variable,
+                ), f"{variable} is profile-orthogonal"
 
     def test_profile_incomplete(self):
         """
         Ensures profile-incomplete detection works
         """
         with Dataset(resources.STATIC_FILES["profile-incomplete"]) as nc:
             for variable in util.get_geophysical_variables(nc):
                 assert util.is_profile_incomplete(
-                    nc, variable
-                ), "{} is profile-incomplete".format(variable)
+                    nc,
+                    variable,
+                ), f"{variable} is profile-incomplete"
 
     def test_timeseries_profile_single_station(self):
         """
         Ensures timeseries profile single station detection works
         """
         with Dataset(resources.STATIC_FILES["timeseries-profile-single-station"]) as nc:
             for variable in util.get_geophysical_variables(nc):
                 assert util.is_timeseries_profile_single_station(
-                    nc, variable
-                ), "{} is timeseries-profile-single-station".format(variable)
+                    nc,
+                    variable,
+                ), f"{variable} is timeseries-profile-single-station"
 
     def test_timeseries_profile_multi_station(self):
         """
         Ensures timeseries profile multi station detection works
         """
         with Dataset(resources.STATIC_FILES["timeseries-profile-multi-station"]) as nc:
             for variable in util.get_geophysical_variables(nc):
                 assert util.is_timeseries_profile_multi_station(
-                    nc, variable
-                ), "{} is timeseries-profile-multi-station".format(variable)
+                    nc,
+                    variable,
+                ), f"{variable} is timeseries-profile-multi-station"
 
     def test_timeseries_profile_single_ortho_time(self):
         """
         Ensures timeseries profile single station ortho time detection works
         """
         with Dataset(
-            resources.STATIC_FILES["timeseries-profile-single-ortho-time"]
+            resources.STATIC_FILES["timeseries-profile-single-ortho-time"],
         ) as nc:
             for variable in util.get_geophysical_variables(nc):
                 assert util.is_timeseries_profile_single_ortho_time(
-                    nc, variable
-                ), "{} is timeseries-profile-single-ortho-time".format(variable)
+                    nc,
+                    variable,
+                ), f"{variable} is timeseries-profile-single-ortho-time"
 
     def test_timeseries_profile_multi_ortho_time(self):
         """
         Ensures timeseries profile multi station ortho time detection works
         """
         with Dataset(
-            resources.STATIC_FILES["timeseries-profile-multi-ortho-time"]
+            resources.STATIC_FILES["timeseries-profile-multi-ortho-time"],
         ) as nc:
             for variable in util.get_geophysical_variables(nc):
                 assert util.is_timeseries_profile_multi_ortho_time(
-                    nc, variable
-                ), "{} is timeseries-profile-multi-ortho-time".format(variable)
+                    nc,
+                    variable,
+                ), f"{variable} is timeseries-profile-multi-ortho-time"
 
     def test_timeseries_profile_ortho_depth(self):
         """
         Ensures timeseries profile ortho depth detection works
         """
         with Dataset(resources.STATIC_FILES["timeseries-profile-ortho-depth"]) as nc:
             for variable in util.get_geophysical_variables(nc):
                 assert util.is_timeseries_profile_ortho_depth(
-                    nc, variable
-                ), "{} is timeseries-profile-ortho-depth".format(variable)
+                    nc,
+                    variable,
+                ), f"{variable} is timeseries-profile-ortho-depth"
 
     def test_timeseries_profile_incomplete(self):
         """
         Ensures timeseries profile station incomplete detection works
         """
         with Dataset(resources.STATIC_FILES["timeseries-profile-incomplete"]) as nc:
             for variable in util.get_geophysical_variables(nc):
                 assert util.is_timeseries_profile_incomplete(
-                    nc, variable
-                ), "{} is timeseries-profile-incomplete".format(variable)
+                    nc,
+                    variable,
+                ), f"{variable} is timeseries-profile-incomplete"
 
     def test_trajectory_profile_orthogonal(self):
         """
         Ensures trajectory profile orthogonal detection works
         """
         with Dataset(resources.STATIC_FILES["trajectory-profile-orthogonal"]) as nc:
             for variable in util.get_geophysical_variables(nc):
                 assert util.is_trajectory_profile_orthogonal(
-                    nc, variable
-                ), "{} is trajectory profile orthogonal".format(variable)
+                    nc,
+                    variable,
+                ), f"{variable} is trajectory profile orthogonal"
 
     def test_trajectory_profile_incomplete(self):
         """
         Ensures trajectory profile incomplete detection works
         """
         with Dataset(resources.STATIC_FILES["trajectory-profile-incomplete"]) as nc:
             for variable in util.get_geophysical_variables(nc):
                 assert util.is_trajectory_profile_incomplete(
-                    nc, variable
-                ), "{} is trajectory profile incomplete".format(variable)
+                    nc,
+                    variable,
+                ), f"{variable} is trajectory profile incomplete"
 
     def test_2d_regular_grid(self):
         """
         Ensures 2D Regular Grid detection works
         """
         with Dataset(resources.STATIC_FILES["2d-regular-grid"]) as nc:
             for variable in util.get_geophysical_variables(nc):
                 assert util.is_2d_regular_grid(
-                    nc, variable
-                ), "{} is 2D regular grid".format(variable)
+                    nc,
+                    variable,
+                ), f"{variable} is 2D regular grid"
 
     def test_2d_static_grid(self):
         """
         Ensures 2D Static Grid detection works
         """
         with Dataset(resources.STATIC_FILES["2d-static-grid"]) as nc:
             for variable in util.get_geophysical_variables(nc):
                 assert util.is_2d_static_grid(
-                    nc, variable
-                ), "{} is a 2D static grid".format(variable)
+                    nc,
+                    variable,
+                ), f"{variable} is a 2D static grid"
 
     def test_3d_regular_grid(self):
         """
         Ensures 2U Regular Grid detection works
         """
         with Dataset(resources.STATIC_FILES["3d-regular-grid"]) as nc:
             for variable in util.get_geophysical_variables(nc):
                 assert util.is_3d_regular_grid(
-                    nc, variable
-                ), "{} is 3d regular grid".format(variable)
+                    nc,
+                    variable,
+                ), f"{variable} is 3d regular grid"
 
     def test_3d_static_grid(self):
         """
         Ensures 3D Static Grid detection works
         """
         with Dataset(resources.STATIC_FILES["3d-static-grid"]) as nc:
             for variable in util.get_geophysical_variables(nc):
                 assert util.is_3d_static_grid(
-                    nc, variable
-                ), "{} is a 3D static grid".format(variable)
+                    nc,
+                    variable,
+                ), f"{variable} is a 3D static grid"
 
     def test_boundaries(self):
         """
         Ensures that boundary variables are not listed as geophysical variables
         """
         with Dataset(resources.STATIC_FILES["grid-boundaries"]) as nc:
             assert "lat_bnds" not in util.get_geophysical_variables(nc)
@@ -251,29 +267,29 @@
         """
         with Dataset(resources.STATIC_FILES["rotated_pole_grid"]) as nc:
             grid_mapping = util.get_grid_mapping_variables(nc)
             coordinate_variables = util.get_coordinate_variables(nc)
             axis_variables = util.get_axis_variables(nc)
 
             assert "rotated_pole" in grid_mapping
-            assert set(["rlon", "rlat", "lev"]) == set(coordinate_variables)
-            assert set(["rlon", "rlat", "lev"]) == set(axis_variables)
+            assert {"rlon", "rlat", "lev"} == set(coordinate_variables)
+            assert {"rlon", "rlat", "lev"} == set(axis_variables)
             assert "lat" == util.get_lat_variable(nc)
             assert "lon" == util.get_lon_variable(nc)
 
     def test_auxiliary_coordinates(self):
         """
         Ensures variables are classified as auxiliary coordinate variables
         """
         with Dataset(resources.STATIC_FILES["bad_units"]) as nc:
             coordinate_variables = util.get_coordinate_variables(nc)
-            assert set(["time"]) == set(coordinate_variables)
+            assert {"time"} == set(coordinate_variables)
 
             aux_coord_vards = util.get_auxiliary_coordinate_variables(nc)
-            assert set(["lat", "lon"]) == set(aux_coord_vards)
+            assert {"lat", "lon"} == set(aux_coord_vards)
 
     def test_forecast_reference_metadata(self):
         """
         Tests variables used for forecast reference metadata to ensure they are
         not misclassified as geophysical variables.
         """
         with Dataset(resources.STATIC_FILES["forecast_reference"]) as nc:
@@ -412,290 +428,346 @@
     def test_is_variable_valid_ragged_array_repr_featureType(self):
         nc = MockRaggedArrayRepr("timeseries", "indexed")
 
         # add a variable that isn't recognized as geophysical
         v = nc.createVariable("data1", "d", ("SAMPLE_DIMENSION",), fill_value=None)
         v.setncattr("cf_role", "blah")
         self.assertFalse(
-            util.is_variable_valid_ragged_array_repr_featureType(nc, "data1")
+            util.is_variable_valid_ragged_array_repr_featureType(nc, "data1"),
         )
 
         # add geophysical variable with correct dimension
         nc = MockRaggedArrayRepr("timeseries", "indexed")
         v = nc.createVariable("data1", "d", ("SAMPLE_DIMENSION",), fill_value=None)
         v.setncattr("standard_name", "sea_water_pressure")
         # test the variable
         self.assertTrue(
-            util.is_variable_valid_ragged_array_repr_featureType(nc, "data1")
+            util.is_variable_valid_ragged_array_repr_featureType(nc, "data1"),
         )
 
         # add good variable and another variable, this time with the improper dimension
         nc = MockRaggedArrayRepr("timeseries", "indexed")
         v = nc.createVariable("data1", "d", ("SAMPLE_DIMENSION",), fill_value=None)
         v.setncattr("standard_name", "sea_water_pressure")
         v2 = nc.createVariable("data2", "d", ("INSTANCE_DIMENSION",), fill_value=None)
         v2.setncattr("standard_name", "sea_water_salinity")
 
         # good variable should pass, second should fail
         self.assertTrue(
-            util.is_variable_valid_ragged_array_repr_featureType(nc, "data1")
+            util.is_variable_valid_ragged_array_repr_featureType(nc, "data1"),
         )
         self.assertFalse(
-            util.is_variable_valid_ragged_array_repr_featureType(nc, "data2")
+            util.is_variable_valid_ragged_array_repr_featureType(nc, "data2"),
         )
 
     def test_is_dataset_valid_ragged_array_repr_featureType(self):
-
         # first test single featureType
 
         # ----- timeseries, indexed ----- #
 
         nc = MockRaggedArrayRepr("timeseries", "indexed")
         self.assertTrue(
-            util.is_dataset_valid_ragged_array_repr_featureType(nc, "timeseries")
+            util.is_dataset_valid_ragged_array_repr_featureType(nc, "timeseries"),
         )
 
         # we'll add another cf_role variable
         nc = MockRaggedArrayRepr("timeseries", "indexed")
         v = nc.createVariable("var2", "i", ("INSTANCE_DIMENSION",), fill_value=None)
         v.setncattr("cf_role", "yeetyeet_id")
         self.assertFalse(
-            util.is_dataset_valid_ragged_array_repr_featureType(nc, "timeseries")
+            util.is_dataset_valid_ragged_array_repr_featureType(nc, "timeseries"),
         )
 
         # we'll add another index variable, also bad
         nc = MockRaggedArrayRepr("timeseries", "indexed")
         v = nc.createVariable("index_var2", "i", ("SAMPLE_DIMENSION",), fill_value=None)
         v.setncattr("instance_dimension", "INSTANCE_DIMENSION")
         self.assertFalse(
-            util.is_dataset_valid_ragged_array_repr_featureType(nc, "timeseries")
+            util.is_dataset_valid_ragged_array_repr_featureType(nc, "timeseries"),
         )
 
         # ----- timeseries, contiguous ----- #
         nc = MockRaggedArrayRepr("timeseries", "contiguous")
         self.assertTrue(
-            util.is_dataset_valid_ragged_array_repr_featureType(nc, "timeseries")
+            util.is_dataset_valid_ragged_array_repr_featureType(nc, "timeseries"),
         )
 
         # add another cf_role var, bad
         nc = MockRaggedArrayRepr("timeseries", "contiguous")
         v = nc.createVariable("var2", "i", ("INSTANCE_DIMENSION",), fill_value=None)
         v.setncattr("cf_role", "yeetyeet_id")
         self.assertFalse(
-            util.is_dataset_valid_ragged_array_repr_featureType(nc, "timeseries")
+            util.is_dataset_valid_ragged_array_repr_featureType(nc, "timeseries"),
         )
 
         # add another count variable, bad
         v = nc.createVariable(
-            "count_var2", "i", ("INSTANCE_DIMENSION",), fill_value=None
+            "count_var2",
+            "i",
+            ("INSTANCE_DIMENSION",),
+            fill_value=None,
         )
         v.setncattr("sample_dimension", "SAMPLE_DIMENSION")
         self.assertFalse(
-            util.is_dataset_valid_ragged_array_repr_featureType(nc, "timeseries")
+            util.is_dataset_valid_ragged_array_repr_featureType(nc, "timeseries"),
         )
 
         # ----- profile, indexed ----- #
 
         nc = MockRaggedArrayRepr("profile", "indexed")
         self.assertTrue(
-            util.is_dataset_valid_ragged_array_repr_featureType(nc, "profile")
+            util.is_dataset_valid_ragged_array_repr_featureType(nc, "profile"),
         )
 
         # add another cf_role var
         nc = MockRaggedArrayRepr("profile", "indexed")
         v = nc.createVariable("var2", "i", ("INSTANCE_DIMENSION",), fill_value=None)
         v.setncattr("cf_role", "yeetyeet_id")
         self.assertFalse(
-            util.is_dataset_valid_ragged_array_repr_featureType(nc, "profile")
+            util.is_dataset_valid_ragged_array_repr_featureType(nc, "profile"),
         )
 
         # we'll add another index variable, also bad
         nc = MockRaggedArrayRepr("profile", "indexed")
         v = nc.createVariable("index_var2", "i", ("SAMPLE_DIMENSION",), fill_value=None)
         v.setncattr("instance_dimension", "INSTANCE_DIMENSION")
         self.assertFalse(
-            util.is_dataset_valid_ragged_array_repr_featureType(nc, "profile")
+            util.is_dataset_valid_ragged_array_repr_featureType(nc, "profile"),
         )
 
         # ----- profile, contiguous ----- #
         nc = MockRaggedArrayRepr("profile", "contiguous")
         self.assertTrue(
-            util.is_dataset_valid_ragged_array_repr_featureType(nc, "profile")
+            util.is_dataset_valid_ragged_array_repr_featureType(nc, "profile"),
         )
 
         # add another cf_role var
         nc = MockRaggedArrayRepr("profile", "contiguous")
         v = nc.createVariable("var2", "i", ("INSTANCE_DIMENSION",), fill_value=None)
         v.setncattr("cf_role", "yeetyeet_id")
         self.assertFalse(
-            util.is_dataset_valid_ragged_array_repr_featureType(nc, "profile")
+            util.is_dataset_valid_ragged_array_repr_featureType(nc, "profile"),
         )
 
         # we'll add another count variable, also bad
         nc = MockRaggedArrayRepr("profile", "contiguous")
         v = nc.createVariable(
-            "index_var2", "i", ("INSTANCE_DIMENSION",), fill_value=None
+            "index_var2",
+            "i",
+            ("INSTANCE_DIMENSION",),
+            fill_value=None,
         )
         v.setncattr("sample_dimension", "SAMPLE_DIMENSION")
         self.assertFalse(
-            util.is_dataset_valid_ragged_array_repr_featureType(nc, "profile")
+            util.is_dataset_valid_ragged_array_repr_featureType(nc, "profile"),
         )
 
         # ----- trajectory, indexed ----- #
         nc = MockRaggedArrayRepr("trajectory", "indexed")
         self.assertTrue(
-            util.is_dataset_valid_ragged_array_repr_featureType(nc, "trajectory")
+            util.is_dataset_valid_ragged_array_repr_featureType(nc, "trajectory"),
         )
 
         # add another cf_role var
         nc = MockRaggedArrayRepr("trajectory", "indexed")
         v = nc.createVariable("var2", "i", ("INSTANCE_DIMENSION",), fill_value=None)
         v.setncattr("cf_role", "yeetyeet_id")
         self.assertFalse(
-            util.is_dataset_valid_ragged_array_repr_featureType(nc, "trajectory")
+            util.is_dataset_valid_ragged_array_repr_featureType(nc, "trajectory"),
         )
 
         # we'll add another index variable, also bad
         nc = MockRaggedArrayRepr("trajectory", "indexed")
         v = nc.createVariable("index_var2", "i", ("SAMPLE_DIMENSION",), fill_value=None)
         v.setncattr("instance_dimension", "INSTANCE_DIMENSION")
         self.assertFalse(
-            util.is_dataset_valid_ragged_array_repr_featureType(nc, "trajectory")
+            util.is_dataset_valid_ragged_array_repr_featureType(nc, "trajectory"),
         )
 
         # ----- trajectory, contiguous ----- #
         nc = MockRaggedArrayRepr("trajectory", "contiguous")
         self.assertTrue(
-            util.is_dataset_valid_ragged_array_repr_featureType(nc, "trajectory")
+            util.is_dataset_valid_ragged_array_repr_featureType(nc, "trajectory"),
         )
 
         # add another cf_role var
         nc = MockRaggedArrayRepr("trajectory", "contiguous")
         v = nc.createVariable("var2", "i", ("INSTANCE_DIMENSION",), fill_value=None)
         v.setncattr("cf_role", "yeetyeet_id")
         self.assertFalse(
-            util.is_dataset_valid_ragged_array_repr_featureType(nc, "trajectory")
+            util.is_dataset_valid_ragged_array_repr_featureType(nc, "trajectory"),
         )
 
         # we'll add another count variable, also bad
         nc = MockRaggedArrayRepr("trajectory", "contiguous")
         v = nc.createVariable(
-            "index_var2", "i", ("INSTANCE_DIMENSION",), fill_value=None
+            "index_var2",
+            "i",
+            ("INSTANCE_DIMENSION",),
+            fill_value=None,
         )
         v.setncattr("sample_dimension", "SAMPLE_DIMENSION")
         self.assertFalse(
-            util.is_dataset_valid_ragged_array_repr_featureType(nc, "trajectory")
+            util.is_dataset_valid_ragged_array_repr_featureType(nc, "trajectory"),
         )
 
         # ----- now test compound featureType ----- #
 
         # ----- timeSeriesProfile ----- #
         nc = MockRaggedArrayRepr("timeSeriesProfile")
 
         # NOTE
         # has no geophysical vars, so should (?) (will) fail
         self.assertFalse(
-            util.is_dataset_valid_ragged_array_repr_featureType(nc, "timeseriesprofile")
+            util.is_dataset_valid_ragged_array_repr_featureType(
+                nc,
+                "timeseriesprofile",
+            ),
         )
 
         # add a geophysical variable and test again
         nc = MockRaggedArrayRepr("timeSeriesProfile")
         v1 = nc.createVariable("data1", "i", ("SAMPLE_DIMENSION",), fill_value=None)
         v1.setncattr("standard_name", "pressure")
         self.assertTrue(
-            util.is_dataset_valid_ragged_array_repr_featureType(nc, "timeseriesprofile")
+            util.is_dataset_valid_ragged_array_repr_featureType(
+                nc,
+                "timeseriesprofile",
+            ),
         )
 
         nc = MockRaggedArrayRepr("timeSeriesProfile")
         v1 = nc.createVariable("data1", "i", ("SAMPLE_DIMENSION",), fill_value=None)
         # add a third cf_role variable - this should fail
         v = nc.createVariable(
-            "cf_role_var3", "i", ("INSTANCE_DIMENSION",), fill_value=None
+            "cf_role_var3",
+            "i",
+            ("INSTANCE_DIMENSION",),
+            fill_value=None,
         )
         v.setncattr("cf_role", "yeetyeet_id")
         self.assertFalse(
-            util.is_dataset_valid_ragged_array_repr_featureType(nc, "timeseriesprofile")
+            util.is_dataset_valid_ragged_array_repr_featureType(
+                nc,
+                "timeseriesprofile",
+            ),
         )
 
         # set the index variable to have an incorrect attr
         nc = MockRaggedArrayRepr("timeSeriesProfile")
         v1 = nc.createVariable("data1", "i", ("SAMPLE_DIMENSION",), fill_value=None)
         nc.variables["station_index_variable"].instance_dimension = "SIKE!"
 
         self.assertFalse(
-            util.is_dataset_valid_ragged_array_repr_featureType(nc, "timeseriesprofile")
+            util.is_dataset_valid_ragged_array_repr_featureType(
+                nc,
+                "timeseriesprofile",
+            ),
         )
 
         # change the sample_dimension attr on the count variable, bad
         nc = MockRaggedArrayRepr("timeSeriesProfile")
         v1 = nc.createVariable("data1", "i", ("SAMPLE_DIMENSION",), fill_value=None)
         nc.variables["counter_var"].sample_dimension = "SIKE!"
 
         self.assertFalse(
-            util.is_dataset_valid_ragged_array_repr_featureType(nc, "timeseriesprofile")
+            util.is_dataset_valid_ragged_array_repr_featureType(
+                nc,
+                "timeseriesprofile",
+            ),
         )
 
         # give another geophysical data variable a different dimension
         nc = MockRaggedArrayRepr("timeSeriesProfile")
         v1 = nc.createVariable("data1", "i", ("SAMPLE_DIMENSION",), fill_value=None)
         v1 = nc.createVariable(
-            "data2", "i", ("STATION_DIMENSION",), fill_value=None  # bad!
+            "data2",
+            "i",
+            ("STATION_DIMENSION",),
+            fill_value=None,  # bad!
         )
         self.assertFalse(
-            util.is_dataset_valid_ragged_array_repr_featureType(nc, "timeseriesprofile")
+            util.is_dataset_valid_ragged_array_repr_featureType(
+                nc,
+                "timeseriesprofile",
+            ),
         )
 
         # ----- trajectoryProfile ----- #
         nc = MockRaggedArrayRepr("trajectoryProfile")
 
         # NOTE
         # has no geophysical vars, so should (?) (will) fail
         self.assertFalse(
-            util.is_dataset_valid_ragged_array_repr_featureType(nc, "trajectoryprofile")
+            util.is_dataset_valid_ragged_array_repr_featureType(
+                nc,
+                "trajectoryprofile",
+            ),
         )
 
         # add a geophysical variable and test again
         nc = MockRaggedArrayRepr("trajectoryProfile")
         v1 = nc.createVariable("data1", "i", ("SAMPLE_DIMENSION",), fill_value=None)
         v1.setncattr("standard_name", "pressure")
         self.assertTrue(
-            util.is_dataset_valid_ragged_array_repr_featureType(nc, "trajectoryprofile")
+            util.is_dataset_valid_ragged_array_repr_featureType(
+                nc,
+                "trajectoryprofile",
+            ),
         )
 
         nc = MockRaggedArrayRepr("trajectoryProfile")
         v1 = nc.createVariable("data1", "i", ("SAMPLE_DIMENSION",), fill_value=None)
         # add a third cf_role variable - this should fail
         v = nc.createVariable(
-            "cf_role_var3", "i", ("INSTANCE_DIMENSION",), fill_value=None
+            "cf_role_var3",
+            "i",
+            ("INSTANCE_DIMENSION",),
+            fill_value=None,
         )
         v.setncattr("cf_role", "yeetyeet_id")
         self.assertFalse(
-            util.is_dataset_valid_ragged_array_repr_featureType(nc, "trajectoryprofile")
+            util.is_dataset_valid_ragged_array_repr_featureType(
+                nc,
+                "trajectoryprofile",
+            ),
         )
 
         # set the index variable to have an incorrect attr
         nc = MockRaggedArrayRepr("trajectoryProfile")
         v1 = nc.createVariable("data1", "i", ("SAMPLE_DIMENSION",), fill_value=None)
         nc.variables["station_index_variable"].instance_dimension = "SIKE!"
 
         self.assertFalse(
-            util.is_dataset_valid_ragged_array_repr_featureType(nc, "trajectoryprofile")
+            util.is_dataset_valid_ragged_array_repr_featureType(
+                nc,
+                "trajectoryprofile",
+            ),
         )
 
         # change the sample_dimension attr on the count variable, bad
         nc = MockRaggedArrayRepr("trajectoryProfile")
         v1 = nc.createVariable("data1", "i", ("SAMPLE_DIMENSION",), fill_value=None)
         nc.variables["counter_var"].sample_dimension = "SIKE!"
 
         self.assertFalse(
-            util.is_dataset_valid_ragged_array_repr_featureType(nc, "trajectoryprofile")
+            util.is_dataset_valid_ragged_array_repr_featureType(
+                nc,
+                "trajectoryprofile",
+            ),
         )
 
         # give another geophysical data variable a different dimension
         nc = MockRaggedArrayRepr("trajectoryProfile")
         v1 = nc.createVariable("data1", "i", ("SAMPLE_DIMENSION",), fill_value=None)
         v1 = nc.createVariable(
-            "data2", "i", ("STATION_DIMENSION",), fill_value=None  # bad!
+            "data2",
+            "i",
+            ("STATION_DIMENSION",),
+            fill_value=None,  # bad!
         )
         self.assertFalse(
-            util.is_dataset_valid_ragged_array_repr_featureType(nc, "trajectoryprofile")
+            util.is_dataset_valid_ragged_array_repr_featureType(
+                nc,
+                "trajectoryprofile",
+            ),
         )
```

### Comparing `compliance-checker-5.0.2/compliance_checker/tests/test_ioos_profile.py` & `compliance-checker-5.1.0/compliance_checker/tests/test_ioos_profile.py`

 * *Files 1% similar despite different names*

```diff
@@ -310,28 +310,29 @@
     for NetCDF, Version 1.1
     """
 
     def setUp(self):
         self.ioos = IOOS1_2Check()
 
     def test_check_geophysical_vars_have_attrs(self):
-
         # create geophysical variable
         ds = MockTimeSeries()  # time, lat, lon, depth
         temp = ds.createVariable("temp", np.float64, dimensions=("time",))
 
         # should fail here
         results = self.ioos.check_geophysical_vars_have_attrs(ds)
         scored, out_of, messages = get_results(results)
         self.assertLess(scored, out_of)
 
         # set the necessary attributes
         ds = MockTimeSeries(default_fill_value=9999999999.0)  # time, lat, lon, depth
         temp = ds.createVariable(
-            "temp", np.float64, fill_value=9999999999.0
+            "temp",
+            np.float64,
+            fill_value=9999999999.0,
         )  # _FillValue
         temp.setncattr("missing_value", 9999999999.0)
         temp.setncattr("standard_name", "sea_surface_temperature")
         temp.setncattr(
             "standard_name_url",
             "http://cfconventions.org/Data/cf-standard-names/64/build/cf-standard-name-table.html",
         )
@@ -345,15 +346,18 @@
         self.assertEqual(scored, out_of)
 
     def test_check_accuracy_precision_resolution(self):
         # doesn't have accuracy, precision, resolution, should fail
 
         ds = MockTimeSeries()  # time, lat, lon, depth
         temp = ds.createVariable(
-            "temp", np.float64, dimensions=("time",), fill_value=9999999999.0
+            "temp",
+            np.float64,
+            dimensions=("time",),
+            fill_value=9999999999.0,
         )  # _FillValue
         temp.setncattr("standard_name", "sea_water_temperature")
         results = self.ioos.check_accuracy(ds)
         scored, out_of, messages = get_results(results)
         self.assertLess(scored, out_of)
 
         # add non-numeric vals for accuracy
@@ -376,19 +380,21 @@
         temp.setncattr("standard_name", "sea_water_practical_salinity")
         temp.setncattr("accuracy", 45)
         results = self.ioos.check_accuracy(ds)
         scored, out_of, messages = get_results(results)
         self.assertEqual(scored, out_of)
 
     def test_check_geospatial_vars_have_attrs(self):
-
         # create geophysical variable
         ds = MockTimeSeries()  # time, lat, lon, depth
         temp = ds.createVariable(
-            "temp", np.float64, dimensions=("time",), fill_value=9999999999.0
+            "temp",
+            np.float64,
+            dimensions=("time",),
+            fill_value=9999999999.0,
         )  # _FillValue
         temp.setncattr("standard_name", "sea_water_temperature")
         results = self.ioos.check_accuracy(ds)
         scored, out_of, messages = get_results(results)
         self.assertLess(scored, out_of)
 
         # add non-numeric vals for accuracy
@@ -521,19 +527,19 @@
 
         # good ancillary var stdname, good units, pass
         tmp.setncattr("standard_name", "aggregate_quality_flag")
         ds.variables["time"].setncattr("units", "seconds since 1970-01-01T00:00:00Z")
         result = self.ioos.check_gts_ingest_requirements(ds)
         self.assertFalse(result.value)
         self.assertIn(
-            "The following variables qualified for NDBC/GTS Ingest: time\n", result.msgs
+            "The following variables qualified for NDBC/GTS Ingest: time\n",
+            result.msgs,
         )
 
     def test_check_instrument_variables(self):
-
         ds = MockTimeSeries()  # time, lat, lon, depth
 
         # no instrument variable, should pass
         results = self.ioos.check_instrument_variables(ds)
         scored, out_of, messages = get_results(results)
         self.assertEqual(scored, out_of)
 
@@ -642,15 +648,15 @@
         # email address is neither of the above, so should fail
         bad_result = validator.validate(test_attr_name, "webmaster.ioos.us@noaa.gov")
         self.assertFalse(bad_result[0])
         self.assertEqual(
             bad_result[1],
             [
                 "naming_authority should either be a URL or a "
-                'reversed DNS name (e.g "edu.ucar.unidata")'
+                'reversed DNS name (e.g "edu.ucar.unidata")',
             ],
         )
 
     def test_platform_id_validation(self):
         attn = "platform_id"
         attv = "alphaNum3R1C"
         v = IOOS1_2_PlatformIDValidator()
@@ -685,15 +691,14 @@
         # good value
         ds.setncattr("platform", "single_string")
         res = self.ioos.check_platform_global(ds)
         self.assertTrue(res.value)
         self.assertEqual(res.msgs, [])
 
     def test_check_single_platform(self):
-
         ds = MockTimeSeries()  # time, lat, lon, depth
 
         # no global attr but also no platform variables, should pass
         result = self.ioos.check_single_platform(ds)
         self.assertTrue(result.value)
         self.assertEqual(result.msgs, [])
 
@@ -796,15 +801,16 @@
         qr.setncattr("references", "http://services.cormp.org/quality.php")
         results = self.ioos.check_qartod_variables_references(ds)
         self.assertTrue(all(r.value for r in results))
         self.assertEqual(results[0].msgs, [])  # only one Result to test
 
         # QARTOD variable with bad references (fail)
         qr.setncattr(
-            "references", r"p9q384ht09q38@@####???????////??//\/\/\/\//\/\74ht"
+            "references",
+            r"p9q384ht09q38@@####???????////??//\/\/\/\//\/\74ht",
         )
         results = self.ioos.check_qartod_variables_references(ds)
         self.assertFalse(all(r.value for r in results))
 
     def test_check_ioos_ingest(self):
         ds = MockTimeSeries()
 
@@ -939,15 +945,14 @@
         ds.setncattr("contributor_role", "editor,coAuthor")
         ds.setncattr("contributor_role_vocabulary", 64)
         results = self.ioos.check_contributor_role_and_vocabulary(ds)
         scored, out_of, messages = get_results(results)
         self.assertLess(scored, out_of)
 
     def test_check_feattype_timeseries_cf_role(self):
-
         # featureType: timeseries and timeseries - msingle station require same tests
 
         # for ftype in ("timeseries", "timeseries - single station", "timeseries - multiple station"):
         ftype = "timeseries"
         ds = MockTimeSeries()  # time, lat, lon, depth
         ds.setncattr("featureType", ftype)
         ds.createVariable("temp", "d", ("time"))
@@ -1191,15 +1196,17 @@
         scored, out_of, messages = get_results(results)
         self.assertEqual(scored, out_of)
 
         # make an instrument variable
         temp = ds.createVariable("temperature", "d", dimensions=("time",))
         temp.setncattr("instrument", "inst")
         inst = ds.createVariable(
-            "inst", "d", dimensions=()
+            "inst",
+            "d",
+            dimensions=(),
         )  # no make_model or calibration_date
         results = self.ioos.check_instrument_make_model_calib_date(ds)
         scored, out_of, messages = get_results(results)
         self.assertLess(scored, out_of)
 
         # add make_model
         inst.setncattr("make_model", "yessir")
```

### Comparing `compliance-checker-5.0.2/compliance_checker/tests/test_ioos_sos.py` & `compliance-checker-5.1.0/compliance_checker/tests/test_ioos_sos.py`

 * *Files 25% similar despite different names*

```diff
@@ -8,41 +8,49 @@
 
 
 # TODO: Use inheritance to eliminate redundant code in test setup, etc
 class TestIOOSSOSGetCapabilities(unittest.TestCase):
     def setUp(self):
         with open(
             os.path.join(
-                os.path.dirname(__file__), "data/http_mocks/ncsos_getcapabilities.xml"
-            )
+                os.path.dirname(__file__),
+                "data/http_mocks/ncsos_getcapabilities.xml",
+            ),
         ) as f:
             self.resp = f.read()
         # need to monkey patch checkers prior to running tests, or no checker
         # classes will show up
         CheckSuite().load_all_available_checkers()
 
     @httpretty.activate
     def test_retrieve_getcaps(self):
         """Method that simulates retrieving SOS GetCapabilities"""
         url = "http://data.oceansmap.com/thredds/sos/caricoos_ag/VIA/VIA.ncml"
         httpretty.register_uri(
-            httpretty.GET, url, content_type="text/xml", body=self.resp
+            httpretty.GET,
+            url,
+            content_type="text/xml",
+            body=self.resp,
         )
         httpretty.register_uri(
-            httpretty.HEAD, url, content_type="text/xml", body="HTTP/1.1 200"
+            httpretty.HEAD,
+            url,
+            content_type="text/xml",
+            body="HTTP/1.1 200",
         )
         ComplianceChecker.run_checker(url, ["ioos_sos"], 1, "normal")
 
 
 class TestIOOSSOSDescribeSensor(unittest.TestCase):
     def setUp(self):
         with open(
             os.path.join(
-                os.path.dirname(__file__), "data/http_mocks/ncsos_describesensor.xml"
-            )
+                os.path.dirname(__file__),
+                "data/http_mocks/ncsos_describesensor.xml",
+            ),
         ) as f:
             self.resp = f.read()
         # need to monkey patch checkers prior to running tests, or no checker
         # classes will show up
         CheckSuite().load_all_available_checkers()
 
     @httpretty.activate
@@ -53,16 +61,22 @@
             "request=describesensor"
             "&service=sos"
             "&procedure=urn:ioos:station:ncsos:VIA"
             "&outputFormat=text/xml%3Bsubtype%3D%22sensorML/1.0.1/profiles/ioos_sos/1.0%22"
             "&version=1.0.0"
         )
         httpretty.register_uri(
-            httpretty.GET, url, content_type="text/xml", body=self.resp
+            httpretty.GET,
+            url,
+            content_type="text/xml",
+            body=self.resp,
         )
         httpretty.register_uri(
-            httpretty.HEAD, url, content_type="text/xml", body="HTTP/1.1 200"
+            httpretty.HEAD,
+            url,
+            content_type="text/xml",
+            body="HTTP/1.1 200",
         )
         # need to mock out the HEAD response so that compliance checker
         # recognizes this as some sort of XML doc instead of an OPeNDAP
         # source
         ComplianceChecker.run_checker(url, ["ioos_sos"], 1, "normal")
```

### Comparing `compliance-checker-5.0.2/compliance_checker/tests/test_protocols.py` & `compliance-checker-5.1.0/compliance_checker/tests/test_protocols.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,63 +1,65 @@
 #!/usr/bin/env python
 """
 compliance_checker/tests/test_protocols.py
 
 Unit tests that ensure the compliance checker can successfully identify protocol endpoints
 """
-from unittest import TestCase
-
 import pytest
 
 from compliance_checker.suite import CheckSuite
 
+pytestmark = [pytest.mark.integration]
+
 
-@pytest.mark.integration
-class TestProtocols(TestCase):
-    def test_netcdf_content_type(self):
-        """
-        Check that urls with Content-Type header of "application/x-netcdf" can
-        successfully be read into memory for checks.
-        """
-        url = "https://gliders.ioos.us/erddap/tabledap/amelia-20180501T0000.ncCF?&time%3E=max(time)-1%20hour"
-        cs = CheckSuite()
-        ds = cs.load_dataset(url)
-        assert ds is not None
-
-    def test_erddap(self):
-        """
-        Tests that a connection can be made to ERDDAP's GridDAP
-        """
-        url = "http://coastwatch.pfeg.noaa.gov/erddap/griddap/osuChlaAnom"
-        cs = CheckSuite()
-        ds = cs.load_dataset(url)
-        assert ds is not None
-
-    def test_hyrax(self):
-        """
-        Tests that a connection can be made to Hyrax
-        """
-        url = "http://test.opendap.org:8080/opendap/ioos/mday_joinExist.ncml"
-        cs = CheckSuite()
-        ds = cs.load_dataset(url)
-        assert ds is not None
-
-    def test_thredds(self):
-        """
-        Tests that a connection can be made to a remote THREDDS endpoint
-        """
-        url = (
-            "http://thredds.ucar.edu/thredds/dodsC/grib/NCEP/GFS/Global_0p25deg_ana/TP"
-        )
-
-        cs = CheckSuite()
-        ds = cs.load_dataset(url)
-        assert ds is not None
-
-    def test_sos(self):
-        """
-        Tests that a connection can be made to an SOS endpoint
-        """
-        url = "https://thredds.aoos.org/thredds/sos/aoos/cruises/ecofoci/2dy12.nc"
-        cs = CheckSuite()
-        ds = cs.load_dataset(url)
-        assert ds is not None
+@pytest.mark.vcr()
+def test_netcdf_content_type():
+    """
+    Check that urls with Content-Type header of "application/x-netcdf" can
+    successfully be read into memory for checks.
+    """
+    url = "https://gliders.ioos.us/erddap/tabledap/amelia-20180501T0000.ncCF?&time%3E=max(time)-1%20hour"
+    cs = CheckSuite()
+    ds = cs.load_dataset(url)
+    assert ds is not None
+
+
+@pytest.mark.vcr()
+def test_erddap():
+    """
+    Tests that a connection can be made to ERDDAP's GridDAP
+    """
+    url = "https://coastwatch.pfeg.noaa.gov/erddap/griddap/osu2ChlaAnom"
+    cs = CheckSuite()
+    ds = cs.load_dataset(url)
+    assert ds is not None
+
+
+def test_hyrax():
+    """
+    Tests that a connection can be made to Hyrax
+    """
+    url = "http://test.opendap.org:8080/opendap/ioos/mday_joinExist.ncml"
+    cs = CheckSuite()
+    ds = cs.load_dataset(url)
+    assert ds is not None
+
+
+def test_thredds():
+    """
+    Tests that a connection can be made to a remote THREDDS endpoint
+    """
+    url = "http://thredds.ucar.edu/thredds/dodsC/grib/NCEP/GFS/Global_0p25deg_ana/TP"
+
+    cs = CheckSuite()
+    ds = cs.load_dataset(url)
+    assert ds is not None
+
+
+def test_sos():
+    """
+    Tests that a connection can be made to an SOS endpoint
+    """
+    url = "https://thredds.aoos.org/thredds/dodsC/aoos/cruises/ecofoci/2dy12.nc"
+    cs = CheckSuite()
+    ds = cs.load_dataset(url)
+    assert ds is not None
```

### Comparing `compliance-checker-5.0.2/compliance_checker/tests/test_suite.py` & `compliance-checker-5.1.0/compliance_checker/tests/test_suite.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,34 +1,38 @@
-# coding=utf-8
 import os
 import unittest
 from pathlib import Path
 
 import numpy as np
 from pkg_resources import resource_filename
 
+from compliance_checker.acdd import ACDDBaseCheck
 from compliance_checker.base import BaseCheck, GenericFile, Result
 from compliance_checker.suite import CheckSuite
 
 static_files = {
     "2dim": resource_filename("compliance_checker", "tests/data/2dim-grid.nc"),
     "bad_region": resource_filename("compliance_checker", "tests/data/bad_region.nc"),
     "bad_data_type": resource_filename(
-        "compliance_checker", "tests/data/bad_data_type.nc"
+        "compliance_checker",
+        "tests/data/bad_data_type.nc",
     ),
     "test_cdl": resource_filename("compliance_checker", "tests/data/test_cdl.cdl"),
     "test_cdl_nc": resource_filename(
-        "compliance_checker", "tests/data/test_cdl_nc_file.nc"
+        "compliance_checker",
+        "tests/data/test_cdl_nc_file.nc",
     ),
     "empty": resource_filename("compliance_checker", "tests/data/non-comp/empty.file"),
     "ru07": resource_filename(
-        "compliance_checker", "tests/data/ru07-20130824T170228_rt0.nc"
+        "compliance_checker",
+        "tests/data/ru07-20130824T170228_rt0.nc",
     ),
     "netCDF4": resource_filename(
-        "compliance_checker", "tests/data/test_cdl_nc4_file.cdl"
+        "compliance_checker",
+        "tests/data/test_cdl_nc4_file.cdl",
     ),
 }
 
 
 class TestSuite(unittest.TestCase):
     # @see
     # http://www.saltycrane.com/blog/2012/07/how-prevent-nose-unittest-using-docstring-when-verbosity-2/
@@ -42,17 +46,17 @@
 
     # override __str__ and __repr__ behavior to show a copy-pastable nosetest name for ion tests
     #  ion.module:TestClassName.test_function_name
     def __repr__(self):
         name = self.id()
         name = name.split(".")
         if name[0] not in ["ion", "pyon"]:
-            return "%s (%s)" % (name[-1], ".".join(name[:-1]))
+            return "{} ({})".format(name[-1], ".".join(name[:-1]))
         else:
-            return "%s ( %s )" % (
+            return "{} ( {} )".format(
                 name[-1],
                 ".".join(name[:-2]) + ":" + ".".join(name[-2:]),
             )
 
     __str__ = __repr__
 
     def test_suite(self):
@@ -70,15 +74,18 @@
         ds = self.cs.load_dataset(static_files["bad_region"])
         score_groups = self.cs.run(ds, [], "cf")
 
         limit = 2
         for checker, rpair in score_groups.items():
             groups, errors = rpair
             score_list, points, out_of = self.cs.standard_output(
-                ds.filepath(), limit, checker, groups
+                ds.filepath(),
+                limit,
+                checker,
+                groups,
             )
             # This asserts that print is able to generate all of the unicode
             # output
             self.cs.standard_output_generation(groups, limit, points, out_of, checker)
 
     def test_generate_dataset_netCDF4(self):
         """
@@ -102,18 +109,25 @@
         assert first_check.value[0] < first_check.value[1]
 
     def test_skip_checks(self):
         """Tests that checks are properly skipped when specified"""
         ds = self.cs.load_dataset(static_files["2dim"])
         # exclude title from the check attributes
         score_groups = self.cs.run_all(ds, ["acdd"], skip_checks=["check_high"])
-        assert all(
-            sg.name not in {"Conventions", "title", "keywords", "summary"}
+        msg_set = {
+            msg
             for sg in score_groups["acdd"][0]
-        )
+            for msg in sg.msgs
+            if sg.weight == BaseCheck.HIGH
+        }
+        skipped_messages = {
+            att + " not present" for att in ACDDBaseCheck().high_rec_atts
+        }
+        # none of the skipped messages should be in the result set
+        self.assertTrue(len(msg_set & skipped_messages) == 0)
 
     def test_skip_check_level(self):
         """Checks level limited skip checks"""
         ds = self.cs.load_dataset(static_files["ru07"])
         score_groups = self.cs.run_all(
             ds,
             ["cf"],
@@ -152,15 +166,18 @@
         ds = self.cs.load_dataset(static_files["bad_data_type"])
         score_groups = self.cs.run(ds, [], "cf")
 
         limit = 2
         for checker, rpair in score_groups.items():
             groups, errors = rpair
             score_list, points, out_of = self.cs.standard_output(
-                ds.filepath(), limit, checker, groups
+                ds.filepath(),
+                limit,
+                checker,
+                groups,
             )
             # This asserts that print is able to generate all of the unicode output
             self.cs.standard_output_generation(groups, limit, points, out_of, checker)
 
     def test_score_grouping(self):
         # Testing the grouping of results for output, which can fail
         # if some assumptions are not met, e.g. if a Result object has
@@ -184,35 +201,49 @@
         ds = self.cs.load_dataset(static_files["test_cdl"])
         vals = self.cs.run(ds, [], "cf")
 
         limit = 2
         for checker, rpair in vals.items():
             groups, errors = rpair
             score_list, cdl_points, cdl_out_of = self.cs.standard_output(
-                ds.filepath(), limit, checker, groups
+                ds.filepath(),
+                limit,
+                checker,
+                groups,
             )
             # This asserts that print is able to generate all of the unicode output
             self.cs.standard_output_generation(
-                groups, limit, cdl_points, cdl_out_of, checker
+                groups,
+                limit,
+                cdl_points,
+                cdl_out_of,
+                checker,
             )
         ds.close()
 
         # Ok now load the nc file that it came from
         ds = self.cs.load_dataset(static_files["test_cdl_nc"])
         vals = self.cs.run(ds, [], "cf")
 
         limit = 2
         for checker, rpair in vals.items():
             groups, errors = rpair
             score_list, nc_points, nc_out_of = self.cs.standard_output(
-                ds.filepath(), limit, checker, groups
+                ds.filepath(),
+                limit,
+                checker,
+                groups,
             )
             # This asserts that print is able to generate all of the unicode output
             self.cs.standard_output_generation(
-                groups, limit, nc_points, nc_out_of, checker
+                groups,
+                limit,
+                nc_points,
+                nc_out_of,
+                checker,
             )
         ds.close()
 
         nc_file_path = static_files["test_cdl"].replace(".cdl", ".nc")
         self.addCleanup(os.remove, nc_file_path)
 
         # Ok the scores should be equal!
@@ -229,15 +260,18 @@
         of potential issues, rather than the weighted score
         """
         ds = self.cs.load_dataset(static_files["bad_region"])
         score_groups = self.cs.run(ds, [], "cf")
         limit = 2
         groups, errors = score_groups["cf"]
         score_list, all_passed, out_of = self.cs.standard_output(
-            ds.filepath(), limit, "cf", groups
+            ds.filepath(),
+            limit,
+            "cf",
+            groups,
         )
         assert all_passed < out_of
 
     def test_netCDF4_features(self):
         """
         Check if a proper netCDF4 file with netCDF4-datatypes is created.
         """
```

### Comparing `compliance-checker-5.0.2/compliance_checker/tests/test_util.py` & `compliance-checker-5.1.0/compliance_checker/tests/test_util.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 #!/usr/bin/env python
-# -*- coding: utf-8 -*-
 """
 compliance_checker/tests/test_util.py
 """
 import unittest
 
 from compliance_checker import util
```

### Comparing `compliance-checker-5.0.2/compliance_checker/util.py` & `compliance-checker-5.1.0/compliance_checker/util.py`

 * *Files identical despite different names*

### Comparing `compliance-checker-5.0.2/compliance_checker.egg-info/PKG-INFO` & `compliance-checker-5.1.0/compliance_checker.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: compliance-checker
-Version: 5.0.2
+Version: 5.1.0
 Summary: Checks Datasets and SOS endpoints for standards compliance
 Home-page: https://github.com/ioos/compliance-checker
 Author: Dave Foster
 Author-email: dave@axiomdatascience.com
 License: Apache License 2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -17,44 +17,44 @@
 Classifier: Topic :: Scientific/Engineering
 Requires-Python: ~=3.5
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # IOOS Compliance Checker
 
-[![Build Status](https://travis-ci.org/ioos/compliance-checker.svg)](https://travis-ci.org/ioos/compliance-checker)
-[![codecov](https://codecov.io/gh/ioos/compliance-checker/branch/master/graph/badge.svg)](https://codecov.io/gh/ioos/compliance-checker)
+[![Tests](https://github.com/ioos/compliance-checker/actions/workflows/default-tests.yml/badge.svg)](https://github.com/ioos/compliance-checker/actions/workflows/default-tests.yml)
+[![codecov](https://codecov.io/gh/ioos/compliance-checker/branch/develop/graph/badge.svg)](https://app.codecov.io/gh/ioos/compliance-checker)
 
 The IOOS Compliance Checker is a python based tool for data providers to check
 for completeness and community standard compliance of local or remote
 [netCDF](https://en.wikipedia.org/wiki/NetCDF) files against
 [CF](http://cfconventions.org/Data/cf-conventions/cf-conventions-1.7/cf-conventions.html) and
-[ACDD](http://wiki.esipfed.org/index.php/Attribute_Convention_for_Data_Discovery_1-3)
+[ACDD](https://wiki.esipfed.org/Attribute_Convention_for_Data_Discovery_1-3)
 file standards. The python module can be used as a command-line tool or as a
 library that can be integrated into other software.
 
-A [web-based version](https://data.ioos.us/compliance/index.html) of the Compliance
+A [web-based version](https://compliance.ioos.us/index.html) of the Compliance
 Checker was developed to enable a broader audience and improve accessibility for the
 checker. With the web version, providers can simply provide a link or upload their
 datasets and get the full suite of capabilities that Compliance Checker offers.
 
 
 It currently supports the following sources and standards:
 
-| Standard                                                                                                                            | Source                                                            | .nc/OPeNDAP/.cdl | SOS                             |
-| ----------------------------------------------------------------------------------------------------                                | -----------                                                       | ------           | ------------------------------- |
-| [ACDD (1.1, 1.3)](http://wiki.esipfed.org/index.php/Attribute_Convention_for_Data_Discovery_1-3)                                    | Built-in                                                          | X                | -                               |
-| [CF (1.8)](http://cfconventions.org/Data/cf-conventions/cf-conventions-1.8/cf-conventions.html)                                     | Built-in                                                          | X                | -                               |
-| [CF (1.7)](http://cfconventions.org/Data/cf-conventions/cf-conventions-1.7/cf-conventions.html)                                     | Built-in                                                          | X                | -                               |
-| [CF (1.6)](http://cfconventions.org/cf-conventions/v1.6.0/cf-conventions.html)                                                      | Built-in                                                          | X                | -                               |
-| IOOS SOS                                                                                                                            | Built-in                                                          | -                | GetCapabilities, DescribeSensor |
+| Standard                                                                                                                   | Source                                                            | .nc/OPeNDAP/.cdl | SOS                             |
+| ----------------------------------------------------------------------------------------------------                       | -----------                                                       | ------           | ------------------------------- |
+| [ACDD (1.1, 1.3)](https://wiki.esipfed.org/Attribute_Convention_for_Data_Discovery_1-3)                                    | Built-in                                                          | X                | -                               |
+| [CF (1.8)](http://cfconventions.org/Data/cf-conventions/cf-conventions-1.8/cf-conventions.html)                            | Built-in                                                          | X                | -                               |
+| [CF (1.7)](http://cfconventions.org/Data/cf-conventions/cf-conventions-1.7/cf-conventions.html)                            | Built-in                                                          | X                | -                               |
+| [CF (1.6)](http://cfconventions.org/cf-conventions/v1.6.0/cf-conventions.html)                                             | Built-in                                                          | X                | -                               |
+| IOOS SOS                                                                                                                   | Built-in                                                          | -                | GetCapabilities, DescribeSensor |
 | [IOOS (1.1)](https://ioos.github.io/ioos-metadata/ioos-metadata-profile-v1-1.html#ioos-netcdf-metadata-profile-attributes) | Built-in                                                          | X                | -                               |
-| [IOOS (1.2)](https://ioos.github.io/ioos-metadata/ioos-metadata-profile-v1-2.html) | Built-in                                                          | X                | -                               |
-| [Glider DAC](https://github.com/ioos/ioosngdac/wiki/NGDAC-NetCDF-File-Format-Version-2)                                             | [ioos/cc-plugin-glider](https://github.com/ioos/cc-plugin-glider) | X                | -                               |
-| [NCEI (1.1, 2.0)](https://www.nodc.noaa.gov/data/formats/netcdf/v2.0/)                                                              | [ioos/cc-plugin-ncei](https://github.com/ioos/cc-plugin-ncei)     | X                | -                               |
+| [IOOS (1.2)](https://ioos.github.io/ioos-metadata/ioos-metadata-profile-v1-2.html)                                         | Built-in                                                          | X                | -                               |
+| [Glider DAC](https://github.com/ioos/ioosngdac/wiki/NetCDF-Specification)                                                  | [ioos/cc-plugin-glider](https://github.com/ioos/cc-plugin-glider) | X                | -                               |
+| [NCEI (1.1, 2.0)](https://www.ncei.noaa.gov/data/oceans/ncei/formats/netcdf/v2.0/index.html)                               | [ioos/cc-plugin-ncei](https://github.com/ioos/cc-plugin-ncei)     | X                | -                               |
 
 
 ## Advice to data providers
 
 While the command-line version of this tool can be run in a loop, it is not necessary to check
 every file if they are all created the same way. In short, this tool is not meant for
 identifying bugs in your data processing stream. It is, however, intended to help you identify
@@ -62,19 +62,19 @@
 for any reason it would be worth your while to run one file through the Compliance Checker to
 insure you procedure change does not impact your file’s compliance.
 
 If you feel you will need to run a batch of files through the Compliance Checker, please contact
 the IOOS Program Office Operations Division for assistance.
 
 
-# [The Compliance Checker Web Tool](https://data.ioos.us/compliance/)
+# [The Compliance Checker Web Tool](https://compliance.ioos.us/index.html)
 
 The IOOS Compliance Checker front end companion.
 
-[https://data.ioos.us/compliance/](https://data.ioos.us/compliance/)
+[https://compliance.ioos.us/index.html](https://compliance.ioos.us/index.html)
 
 Source Code is available on GitHub:
 
 [https://github.com/ioos/compliance-checker-web](https://github.com/ioos/compliance-checker-web)
 
 ## Usage
 Select the test you want to run from the dropdown menu. Then, either upload your dataset or provide a url to a
@@ -91,19 +91,19 @@
 users interested in batch processing files hosted via OPeNDAP. Details on how to use the API are
 available on the Compliance Checker Web [wiki page](https://github.com/ioos/compliance-checker-web/wiki/API).
 
 Here are a couple examples:
 
 **HTML Output**
 
-https://data.ioos.us/compliance/api/run?report_format=html&test=acdd&url=http://sos.maracoos.org/stable/dodsC/hrecos/stationHRMARPH-agg.ncml
+https://compliance.ioos.us/index.htmlapi/run?report_format=html&test=acdd&url=http://sos.maracoos.org/stable/dodsC/hrecos/stationHRMARPH-agg.ncml
 
 **JSON Output**
 
-https://data.ioos.us/compliance/api/run?report_format=json&test=acdd&url=http://sos.maracoos.org/stable/dodsC/hrecos/stationHRMARPH-agg.ncml
+https://compliance.ioos.us/index.htmlapi/run?report_format=json&test=acdd&url=http://sos.maracoos.org/stable/dodsC/hrecos/stationHRMARPH-agg.ncml
 
 # The Compliance Checker Command Line Tool
 
 
 ## Concepts & Terminology
 
 Each compliance standard is executed by a Check Suite,
@@ -388,28 +388,28 @@
     scored = cc_data[cc_test[0]]['scored_points']
     possible = cc_data[cc_test[0]]['possible_points']
     log.debug('CC Scored {} out of {} possible points'.format(scored, possible))
 ```
 
 ## Compliance Checker Plug-Ins
 
-Separate Plug-ins have been developed to complement the master Compliance Checker tool with
+Separate Plug-ins have been developed to complement the Compliance Checker tool with
 specifications for preparing data to be submitted to different data assembly centers.
 The version numbering of these plug-ins are not necessarily link to the version of the
-master Compliance Checker, but they are all designed to run with the master Compliance Checker tool.
+Compliance Checker, but they are all designed to run with the Compliance Checker tool.
 
 ### Current Plug-in Releases:
 
 - [GliderDAC](https://github.com/ioos/cc-plugin-glider/releases)
 
-This is a checker for [GliderDAC](https://github.com/ioos/ioosngdac/wiki/NGDAC-NetCDF-File-Format-Version-2) files
+This is a checker for [GliderDAC](https://github.com/ioos/ioosngdac/wiki/NetCDF-Specification) files
 
 - [NCEI](https://github.com/ioos/cc-plugin-ncei/releases) - [link](https://github.com/ioos/cc-plugin-ncei)
 
-This is a checker for NCEI netCDF Templates [v1.1](https://www.nodc.noaa.gov/data/formats/netcdf/v1.1/) and [v2.0](https://www.nodc.noaa.gov/data/formats/netcdf/v2.0/) files.
+This is a checker for NCEI netCDF Templates [v1.1](https://www.ncei.noaa.gov/data/oceans/ncei/formats/netcdf/v1.1/index.html) and [v2.0](https://www.ncei.noaa.gov/data/oceans/ncei/formats/netcdf/v2.0/index.html) files.
 
 These plug-ins must be installed separately but work on top of the base compliance checker software.
 
 ```
 pip install cc-plugin-ncei
 ```
```

### Comparing `compliance-checker-5.0.2/setup.py` & `compliance-checker-5.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,18 @@
-import io
-
 from setuptools import find_packages, setup
 
 
 def readme():
-    with io.open("README.md", encoding="utf-8") as f:
+    with open("README.md", encoding="utf-8") as f:
         return f.read()
 
 
 def pip_requirements(fname="requirements.txt"):
     reqs = []
-    with open(fname, "r") as f:
+    with open(fname) as f:
         for line in f:
             line = line.strip()
             if not line or line.startswith("#"):
                 continue
             reqs.append(line)
 
     return reqs
```

