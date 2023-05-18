# Comparing `tmp/dart-fss-0.4.3.tar.gz` & `tmp/dart-fss-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dart-fss-0.4.3.tar", last modified: Tue Apr 25 00:35:23 2023, max compression
+gzip compressed data, was "dart-fss-0.4.4.tar", last modified: Thu May 18 12:01:36 2023, max compression
```

## Comparing `dart-fss-0.4.3.tar` & `dart-fss-0.4.4.tar`

### file list

```diff
@@ -1,180 +1,180 @@
-drwxrwxrwx   0        0        0        0 2023-04-25 00:35:23.374908 dart-fss-0.4.3/
--rw-rw-rw-   0        0        0     1093 2023-03-06 00:18:03.000000 dart-fss-0.4.3/LICENSE
--rw-rw-rw-   0        0        0       77 2023-03-06 00:18:03.000000 dart-fss-0.4.3/MANIFEST.in
--rw-rw-rw-   0        0        0     3289 2023-04-25 00:35:23.374908 dart-fss-0.4.3/PKG-INFO
--rw-rw-rw-   0        0        0     2401 2023-04-25 00:23:22.000000 dart-fss-0.4.3/README.md
-drwxrwxrwx   0        0        0        0 2023-04-25 00:35:23.377140 dart-fss-0.4.3/dart_fss/
--rw-rw-rw-   0        0        0      619 2023-03-06 00:18:03.000000 dart-fss-0.4.3/dart_fss/__init__.py
--rw-rw-rw-   0        0        0      518 2023-04-25 00:35:23.377140 dart-fss-0.4.3/dart_fss/_version.py
-drwxrwxrwx   0        0        0        0 2023-04-25 00:35:22.893946 dart-fss-0.4.3/dart_fss/api/
--rw-rw-rw-   0        0        0      224 2023-03-06 00:18:03.000000 dart-fss-0.4.3/dart_fss/api/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-25 00:35:22.911651 dart-fss-0.4.3/dart_fss/api/filings/
--rw-rw-rw-   0        0        0      260 2023-03-06 00:18:03.000000 dart-fss-0.4.3/dart_fss/api/filings/__init__.py
--rw-rw-rw-   0        0        0      396 2023-03-06 00:18:03.000000 dart-fss-0.4.3/dart_fss/api/filings/company.py
--rw-rw-rw-   0        0        0     1320 2023-03-06 00:18:03.000000 dart-fss-0.4.3/dart_fss/api/filings/corp_code.py
--rw-rw-rw-   0        0        0      686 2023-03-06 00:18:03.000000 dart-fss-0.4.3/dart_fss/api/filings/document.py
--rw-rw-rw-   0        0        0     2680 2023-03-06 00:18:03.000000 dart-fss-0.4.3/dart_fss/api/filings/search_filings.py
-drwxrwxrwx   0        0        0        0 2023-04-25 00:35:22.932141 dart-fss-0.4.3/dart_fss/api/finance/
--rw-rw-rw-   0        0        0      394 2023-03-06 00:18:03.000000 dart-fss-0.4.3/dart_fss/api/finance/__init__.py
--rw-rw-rw-   0        0        0     1221 2023-03-06 00:18:03.000000 dart-fss-0.4.3/dart_fss/api/finance/fnltt_multi_acnt.py
--rw-rw-rw-   0        0        0     1183 2023-03-06 00:18:03.000000 dart-fss-0.4.3/dart_fss/api/finance/fnltt_singl_acnt.py
--rw-rw-rw-   0        0        0     1272 2023-03-06 00:18:03.000000 dart-fss-0.4.3/dart_fss/api/finance/fnltt_singl_acnt_all.py
--rw-rw-rw-   0        0        0     1349 2023-03-06 00:18:03.000000 dart-fss-0.4.3/dart_fss/api/finance/xbrl.py
--rw-rw-rw-   0        0        0      774 2023-03-06 00:18:03.000000 dart-fss-0.4.3/dart_fss/api/finance/xbrl_taxonomy.py
--rw-rw-rw-   0        0        0     3692 2023-03-06 00:18:03.000000 dart-fss-0.4.3/dart_fss/api/helper.py
-drwxrwxrwx   0        0        0        0 2023-04-25 00:35:23.011132 dart-fss-0.4.3/dart_fss/api/info/
--rw-rw-rw-   0        0        0     2590 2023-03-06 00:18:03.000000 dart-fss-0.4.3/dart_fss/api/info/__init__.py
--rw-rw-rw-   0        0        0     1184 2023-03-06 00:18:03.000000 dart-fss-0.4.3/dart_fss/api/info/accnut_adtor_nm_nd_adt_opinion.py
--rw-rw-rw-   0        0        0     1229 2023-03-06 00:18:03.000000 dart-fss-0.4.3/dart_fss/api/info/accnut_adtor_non_adt_servc_cncls_sttus.py
--rw-rw-rw-   0        0        0     1132 2023-03-06 00:18:03.000000 dart-fss-0.4.3/dart_fss/api/info/adt_servc_cncls_sttus.py
--rw-rw-rw-   0        0        0     1112 2023-03-06 00:18:03.000000 dart-fss-0.4.3/dart_fss/api/info/alot_matter.py
--rw-rw-rw-   0        0        0     1173 2023-03-06 00:18:03.000000 dart-fss-0.4.3/dart_fss/api/info/cndl_capl_scrits_nrdmp_blce.py
--rw-rw-rw-   0        0        0     1127 2023-03-06 00:18:03.000000 dart-fss-0.4.3/dart_fss/api/info/cprnd_nrdmp_blce.py
--rw-rw-rw-   0        0        0     1134 2023-03-06 00:18:03.000000 dart-fss-0.4.3/dart_fss/api/info/det_scrits_isu_acmslt.py
--rw-rw-rw-   0        0        0     1258 2023-03-06 00:18:03.000000 dart-fss-0.4.3/dart_fss/api/info/drctr_adt_all_mendng_sttus_gmtsck_confm_amount.py
--rw-rw-rw-   0        0        0     1271 2023-03-06 00:18:03.000000 dart-fss-0.4.3/dart_fss/api/info/drctr_adt_all_mendng_sttus_mendng_pymntamt_ty_cl.py
--rw-rw-rw-   0        0        0     1088 2023-03-06 00:18:03.000000 dart-fss-0.4.3/dart_fss/api/info/emp_sttus.py
--rw-rw-rw-   0        0        0     1169 2023-03-06 00:18:03.000000 dart-fss-0.4.3/dart_fss/api/info/entrprs_bil_scrits_nrdmp_blce.py
--rw-rw-rw-   0        0        0     1092 2023-03-06 00:18:03.000000 dart-fss-0.4.3/dart_fss/api/info/exctv_sttus.py
--rw-rw-rw-   0        0        0     1154 2023-03-06 00:18:03.000000 dart-fss-0.4.3/dart_fss/api/info/hmv_audit_all_sttus.py
--rw-rw-rw-   0        0        0     1173 2023-03-06 00:18:03.000000 dart-fss-0.4.3/dart_fss/api/info/hmv_audit_indvdl_by_sttus.py
--rw-rw-rw-   0        0        0     1123 2023-03-06 00:18:03.000000 dart-fss-0.4.3/dart_fss/api/info/hyslr_chg_sttus.py
--rw-rw-rw-   0        0        0     1104 2023-03-06 00:18:03.000000 dart-fss-0.4.3/dart_fss/api/info/hyslr_sttus.py
--rw-rw-rw-   0        0        0     1174 2023-03-06 00:18:03.000000 dart-fss-0.4.3/dart_fss/api/info/indvdl_by_pay.py
--rw-rw-rw-   0        0        0     1106 2023-03-06 00:18:03.000000 dart-fss-0.4.3/dart_fss/api/info/irds_sttus.py
--rw-rw-rw-   0        0        0     1102 2023-03-06 00:18:03.000000 dart-fss-0.4.3/dart_fss/api/info/mrhl_sttus.py
--rw-rw-rw-   0        0        0     1163 2023-03-06 00:18:03.000000 dart-fss-0.4.3/dart_fss/api/info/new_capl_scrits_nrdmp_blce.py
--rw-rw-rw-   0        0        0     1130 2023-03-06 00:18:03.000000 dart-fss-0.4.3/dart_fss/api/info/otr_cpr_invstmnt_sttus.py
--rw-rw-rw-   0        0        0     1167 2023-03-06 00:18:03.000000 dart-fss-0.4.3/dart_fss/api/info/outcmpny_drctr_nd_change_sttus.py
--rw-rw-rw-   0        0        0     1140 2023-03-06 00:18:03.000000 dart-fss-0.4.3/dart_fss/api/info/prvsrp_cptal_use_dtls.py
--rw-rw-rw-   0        0        0     1138 2023-03-06 00:18:03.000000 dart-fss-0.4.3/dart_fss/api/info/pssrp_cptal_use_dtls.py
--rw-rw-rw-   0        0        0     1146 2023-03-06 00:18:03.000000 dart-fss-0.4.3/dart_fss/api/info/srtpd_psndbt_nrdmp_blce.py
--rw-rw-rw-   0        0        0     1121 2023-03-06 00:18:03.000000 dart-fss-0.4.3/dart_fss/api/info/stock_totqy_sttus.py
--rw-rw-rw-   0        0        0     1160 2023-03-06 00:18:03.000000 dart-fss-0.4.3/dart_fss/api/info/tesstk_acqs_dsps_sttus.py
--rw-rw-rw-   0        0        0     1146 2023-03-06 00:18:03.000000 dart-fss-0.4.3/dart_fss/api/info/unrst_exctv_mendng_sttus.py
-drwxrwxrwx   0        0        0        0 2023-04-25 00:35:23.113728 dart-fss-0.4.3/dart_fss/api/issue/
--rw-rw-rw-   0        0        0     2421 2023-03-06 00:18:03.000000 dart-fss-0.4.3/dart_fss/api/issue/__init__.py
--rw-rw-rw-   0        0        0     1115 2023-03-06 00:18:03.000000 dart-fss-0.4.3/dart_fss/api/issue/ast_inhtrf_etc_ptbk_opt.py
--rw-rw-rw-   0        0        0     1103 2023-03-06 00:18:03.000000 dart-fss-0.4.3/dart_fss/api/issue/bdwt_is_decsn.py
--rw-rw-rw-   0        0        0     1101 2023-03-06 00:18:03.000000 dart-fss-0.4.3/dart_fss/api/issue/bnk_mngt_pcbg.py
--rw-rw-rw-   0        0        0     1101 2023-03-06 00:18:03.000000 dart-fss-0.4.3/dart_fss/api/issue/bnk_mngt_pcsp.py
--rw-rw-rw-   0        0        0     1061 2023-03-06 00:18:03.000000 dart-fss-0.4.3/dart_fss/api/issue/bsn_inh_decsn.py
--rw-rw-rw-   0        0        0     1034 2023-03-06 00:18:03.000000 dart-fss-0.4.3/dart_fss/api/issue/bsn_sp.py
--rw-rw-rw-   0        0        0     1061 2023-03-06 00:18:03.000000 dart-fss-0.4.3/dart_fss/api/issue/bsn_trf_decsn.py
--rw-rw-rw-   0        0        0     1059 2023-03-06 00:18:03.000000 dart-fss-0.4.3/dart_fss/api/issue/cmp_dv_decsn.py
--rw-rw-rw-   0        0        0     1075 2023-03-06 00:18:03.000000 dart-fss-0.4.3/dart_fss/api/issue/cmp_dvmg_decsn.py
--rw-rw-rw-   0        0        0     1059 2023-03-06 00:18:03.000000 dart-fss-0.4.3/dart_fss/api/issue/cmp_mg_decsn.py
--rw-rw-rw-   0        0        0     1040 2023-03-06 00:18:03.000000 dart-fss-0.4.3/dart_fss/api/issue/cr_decsn.py
--rw-rw-rw-   0        0        0     1070 2023-03-06 00:18:03.000000 dart-fss-0.4.3/dart_fss/api/issue/ctrcvs_bgrq.py
--rw-rw-rw-   0        0        0     1079 2023-03-06 00:18:03.000000 dart-fss-0.4.3/dart_fss/api/issue/cvbd_is_decsn.py
--rw-rw-rw-   0        0        0     1034 2023-03-06 00:18:03.000000 dart-fss-0.4.3/dart_fss/api/issue/df_ocr.py
--rw-rw-rw-   0        0        0     1053 2023-03-06 00:18:03.000000 dart-fss-0.4.3/dart_fss/api/issue/ds_rs_ocr.py
--rw-rw-rw-   0        0        0     1079 2023-03-06 00:18:03.000000 dart-fss-0.4.3/dart_fss/api/issue/exbd_is_decsn.py
--rw-rw-rw-   0        0        0     1056 2023-03-06 00:18:03.000000 dart-fss-0.4.3/dart_fss/api/issue/fric_decsn.py
--rw-rw-rw-   0        0        0     1052 2023-03-06 00:18:03.000000 dart-fss-0.4.3/dart_fss/api/issue/lwst_lg.py
--rw-rw-rw-   0        0        0     1139 2023-03-06 00:18:03.000000 dart-fss-0.4.3/dart_fss/api/issue/otcpr_stk_invscr_inh_decsn.py
--rw-rw-rw-   0        0        0     1139 2023-03-06 00:18:03.000000 dart-fss-0.4.3/dart_fss/api/issue/otcpr_stk_invscr_trf_decsn.py
--rw-rw-rw-   0        0        0     1096 2023-03-06 00:18:03.000000 dart-fss-0.4.3/dart_fss/api/issue/ov_dlst.py
--rw-rw-rw-   0        0        0     1121 2023-03-06 00:18:03.000000 dart-fss-0.4.3/dart_fss/api/issue/ov_dlst_decsn.py
--rw-rw-rw-   0        0        0     1082 2023-03-06 00:18:03.000000 dart-fss-0.4.3/dart_fss/api/issue/ov_lst.py
--rw-rw-rw-   0        0        0     1107 2023-03-06 00:18:03.000000 dart-fss-0.4.3/dart_fss/api/issue/ov_lst_decsn.py
--rw-rw-rw-   0        0        0     1066 2023-03-06 00:18:03.000000 dart-fss-0.4.3/dart_fss/api/issue/pifric_decsn.py
--rw-rw-rw-   0        0        0     1056 2023-03-06 00:18:03.000000 dart-fss-0.4.3/dart_fss/api/issue/piic_decsn.py
--rw-rw-rw-   0        0        0     1079 2023-03-06 00:18:03.000000 dart-fss-0.4.3/dart_fss/api/issue/stk_extr_decsn.py
--rw-rw-rw-   0        0        0     1105 2023-03-06 00:18:03.000000 dart-fss-0.4.3/dart_fss/api/issue/stkrtbd_inh_decsn.py
--rw-rw-rw-   0        0        0     1105 2023-03-06 00:18:03.000000 dart-fss-0.4.3/dart_fss/api/issue/stkrtbd_trf_decsn.py
--rw-rw-rw-   0        0        0     1079 2023-03-06 00:18:03.000000 dart-fss-0.4.3/dart_fss/api/issue/tgast_inh_decsn.py
--rw-rw-rw-   0        0        0     1079 2023-03-06 00:18:03.000000 dart-fss-0.4.3/dart_fss/api/issue/tgast_trf_decsn.py
--rw-rw-rw-   0        0        0     1077 2023-03-06 00:18:03.000000 dart-fss-0.4.3/dart_fss/api/issue/tsstk_aq_decsn.py
--rw-rw-rw-   0        0        0     1131 2023-03-06 00:18:03.000000 dart-fss-0.4.3/dart_fss/api/issue/tsstk_aq_trctr_cc_decsn.py
--rw-rw-rw-   0        0        0     1133 2023-03-06 00:18:03.000000 dart-fss-0.4.3/dart_fss/api/issue/tsstk_aq_trctr_cns_decsn.py
--rw-rw-rw-   0        0        0     1077 2023-03-06 00:18:03.000000 dart-fss-0.4.3/dart_fss/api/issue/tsstk_dp_decsn.py
--rw-rw-rw-   0        0        0     1120 2023-03-06 00:18:03.000000 dart-fss-0.4.3/dart_fss/api/issue/wd_cocobd_is_decsn.py
-drwxrwxrwx   0        0        0        0 2023-04-25 00:35:23.122301 dart-fss-0.4.3/dart_fss/api/market/
--rw-rw-rw-   0        0        0      187 2023-03-06 00:18:03.000000 dart-fss-0.4.3/dart_fss/api/market/__init__.py
--rw-rw-rw-   0        0        0     2066 2023-03-06 00:18:03.000000 dart-fss-0.4.3/dart_fss/api/market/stock_market.py
--rw-rw-rw-   0        0        0     2009 2023-03-06 00:18:03.000000 dart-fss-0.4.3/dart_fss/api/market/trading_halt.py
-drwxrwxrwx   0        0        0        0 2023-04-25 00:35:23.145189 dart-fss-0.4.3/dart_fss/api/registration/
--rw-rw-rw-   0        0        0      306 2023-03-06 00:18:03.000000 dart-fss-0.4.3/dart_fss/api/registration/__init__.py
--rw-rw-rw-   0        0        0     1026 2023-03-06 00:18:03.000000 dart-fss-0.4.3/dart_fss/api/registration/bd_rs.py
--rw-rw-rw-   0        0        0     1014 2023-03-06 00:18:03.000000 dart-fss-0.4.3/dart_fss/api/registration/dv_rs.py
--rw-rw-rw-   0        0        0     1030 2023-03-06 00:18:03.000000 dart-fss-0.4.3/dart_fss/api/registration/estk_rs.py
--rw-rw-rw-   0        0        0     1070 2023-03-06 00:18:03.000000 dart-fss-0.4.3/dart_fss/api/registration/extr_rs.py
--rw-rw-rw-   0        0        0     1014 2023-03-06 00:18:03.000000 dart-fss-0.4.3/dart_fss/api/registration/mg_rs.py
--rw-rw-rw-   0        0        0     1044 2023-03-06 00:18:03.000000 dart-fss-0.4.3/dart_fss/api/registration/stkdp_rs.py
-drwxrwxrwx   0        0        0        0 2023-04-25 00:35:23.155533 dart-fss-0.4.3/dart_fss/api/shareholder/
--rw-rw-rw-   0        0        0      149 2023-03-06 00:18:03.000000 dart-fss-0.4.3/dart_fss/api/shareholder/__init__.py
--rw-rw-rw-   0        0        0      830 2023-03-06 00:18:03.000000 dart-fss-0.4.3/dart_fss/api/shareholder/elestock.py
--rw-rw-rw-   0        0        0      794 2023-03-06 00:18:03.000000 dart-fss-0.4.3/dart_fss/api/shareholder/majorstock.py
-drwxrwxrwx   0        0        0        0 2023-04-25 00:35:23.156533 dart-fss-0.4.3/dart_fss/auth/
--rw-rw-rw-   0        0        0      124 2023-03-06 00:18:03.000000 dart-fss-0.4.3/dart_fss/auth/__init__.py
--rw-rw-rw-   0        0        0     2567 2023-03-06 00:18:03.000000 dart-fss-0.4.3/dart_fss/auth/auth.py
-drwxrwxrwx   0        0        0        0 2023-04-25 00:35:23.163032 dart-fss-0.4.3/dart_fss/corp/
--rw-rw-rw-   0        0        0      172 2023-03-06 00:18:03.000000 dart-fss-0.4.3/dart_fss/corp/__init__.py
--rw-rw-rw-   0        0        0     8929 2023-03-06 00:18:03.000000 dart-fss-0.4.3/dart_fss/corp/corp.py
--rw-rw-rw-   0        0        0     9456 2023-03-06 00:18:03.000000 dart-fss-0.4.3/dart_fss/corp/corp_list.py
-drwxrwxrwx   0        0        0        0 2023-04-25 00:35:23.176629 dart-fss-0.4.3/dart_fss/errors/
--rw-rw-rw-   0        0        0      459 2023-03-06 00:18:03.000000 dart-fss-0.4.3/dart_fss/errors/__init__.py
--rw-rw-rw-   0        0        0     1514 2023-03-06 00:18:03.000000 dart-fss-0.4.3/dart_fss/errors/checker.py
--rw-rw-rw-   0        0        0     1744 2023-03-06 00:18:03.000000 dart-fss-0.4.3/dart_fss/errors/errors.py
-drwxrwxrwx   0        0        0        0 2023-04-25 00:35:23.192675 dart-fss-0.4.3/dart_fss/filings/
--rw-rw-rw-   0        0        0       91 2023-03-06 00:18:03.000000 dart-fss-0.4.3/dart_fss/filings/__init__.py
--rw-rw-rw-   0        0        0     3897 2023-03-06 00:18:03.000000 dart-fss-0.4.3/dart_fss/filings/pages.py
--rw-rw-rw-   0        0        0    20300 2023-03-06 00:18:03.000000 dart-fss-0.4.3/dart_fss/filings/reports.py
--rw-rw-rw-   0        0        0     2513 2023-03-06 00:18:03.000000 dart-fss-0.4.3/dart_fss/filings/search.py
--rw-rw-rw-   0        0        0     2124 2023-03-06 00:18:03.000000 dart-fss-0.4.3/dart_fss/filings/search_result.py
-drwxrwxrwx   0        0        0        0 2023-04-25 00:35:23.257027 dart-fss-0.4.3/dart_fss/fs/
--rw-rw-rw-   0        0        0      158 2023-03-06 00:18:03.000000 dart-fss-0.4.3/dart_fss/fs/__init__.py
--rw-rw-rw-   0        0        0    54845 2023-03-06 00:19:24.000000 dart-fss-0.4.3/dart_fss/fs/extract.py
--rw-rw-rw-   0        0        0     7924 2023-04-24 06:22:06.000000 dart-fss-0.4.3/dart_fss/fs/fs.py
-drwxrwxrwx   0        0        0        0 2023-04-25 00:35:23.313837 dart-fss-0.4.3/dart_fss/tests/
--rw-rw-rw-   0        0        0        0 2023-03-06 00:18:03.000000 dart-fss-0.4.3/dart_fss/tests/__init__.py
--rw-rw-rw-   0        0        0      854 2023-03-06 00:18:03.000000 dart-fss-0.4.3/dart_fss/tests/test_api_filings.py
--rw-rw-rw-   0        0        0     1721 2023-03-06 00:18:03.000000 dart-fss-0.4.3/dart_fss/tests/test_api_finance.py
--rw-rw-rw-   0        0        0    10350 2023-03-06 00:18:03.000000 dart-fss-0.4.3/dart_fss/tests/test_api_info.py
--rw-rw-rw-   0        0        0    12724 2023-03-06 00:18:03.000000 dart-fss-0.4.3/dart_fss/tests/test_api_issue.py
--rw-rw-rw-   0        0        0      182 2023-03-06 00:18:03.000000 dart-fss-0.4.3/dart_fss/tests/test_api_market.py
--rw-rw-rw-   0        0        0     2136 2023-03-06 00:18:03.000000 dart-fss-0.4.3/dart_fss/tests/test_api_registration.py
--rw-rw-rw-   0        0        0      644 2023-03-06 00:18:03.000000 dart-fss-0.4.3/dart_fss/tests/test_api_shareholder.py
--rw-rw-rw-   0        0        0       88 2023-03-06 00:18:03.000000 dart-fss-0.4.3/dart_fss/tests/test_auth.py
-drwxrwxrwx   0        0        0        0 2023-04-25 00:35:23.321005 dart-fss-0.4.3/dart_fss/tests/test_case/
--rw-rw-rw-   0        0        0     5306 2023-03-06 00:18:03.000000 dart-fss-0.4.3/dart_fss/tests/test_case/crp_case.py
--rw-rw-rw-   0        0        0     2998 2023-03-06 00:18:03.000000 dart-fss-0.4.3/dart_fss/tests/test_case/testcrp.py
--rw-rw-rw-   0        0        0     2637 2023-03-07 00:59:43.000000 dart-fss-0.4.3/dart_fss/tests/test_corp.py
--rw-rw-rw-   0        0        0     1004 2023-03-31 07:24:27.000000 dart-fss-0.4.3/dart_fss/tests/test_errors.py
--rw-rw-rw-   0        0        0     4456 2023-04-24 05:50:55.000000 dart-fss-0.4.3/dart_fss/tests/test_fs.py
--rw-rw-rw-   0        0        0      775 2023-03-06 00:18:03.000000 dart-fss-0.4.3/dart_fss/tests/test_fs_search.py
--rw-rw-rw-   0        0        0      469 2023-03-06 00:18:03.000000 dart-fss-0.4.3/dart_fss/tests/test_regex.py
--rw-rw-rw-   0        0        0     1320 2023-03-06 00:18:03.000000 dart-fss-0.4.3/dart_fss/tests/test_reports.py
--rw-rw-rw-   0        0        0      804 2023-03-06 00:18:03.000000 dart-fss-0.4.3/dart_fss/tests/test_search_report.py
--rw-rw-rw-   0        0        0      653 2023-03-06 00:18:03.000000 dart-fss-0.4.3/dart_fss/tests/test_utils.py
--rw-rw-rw-   0        0        0     2706 2023-03-06 00:18:03.000000 dart-fss-0.4.3/dart_fss/tests/test_xbrl.py
-drwxrwxrwx   0        0        0        0 2023-04-25 00:35:23.358605 dart-fss-0.4.3/dart_fss/utils/
--rw-rw-rw-   0        0        0     1277 2023-03-06 00:18:03.000000 dart-fss-0.4.3/dart_fss/utils/__init__.py
--rw-rw-rw-   0        0        0      842 2023-03-06 00:18:03.000000 dart-fss-0.4.3/dart_fss/utils/cache.py
--rw-rw-rw-   0        0        0      704 2023-03-06 00:18:03.000000 dart-fss-0.4.3/dart_fss/utils/dataframe.py
--rw-rw-rw-   0        0        0     1434 2023-03-06 00:18:03.000000 dart-fss-0.4.3/dart_fss/utils/datetime.py
--rw-rw-rw-   0        0        0     2666 2023-03-06 00:18:03.000000 dart-fss-0.4.3/dart_fss/utils/file.py
--rw-rw-rw-   0        0        0     2733 2023-03-06 00:18:03.000000 dart-fss-0.4.3/dart_fss/utils/notebook.py
--rw-rw-rw-   0        0        0     3077 2023-03-06 00:18:03.000000 dart-fss-0.4.3/dart_fss/utils/regex.py
--rw-rw-rw-   0        0        0     7602 2023-03-06 00:18:03.000000 dart-fss-0.4.3/dart_fss/utils/request.py
--rw-rw-rw-   0        0        0      304 2023-03-06 00:18:03.000000 dart-fss-0.4.3/dart_fss/utils/singleton.py
--rw-rw-rw-   0        0        0     1019 2023-03-06 00:18:03.000000 dart-fss-0.4.3/dart_fss/utils/spinner.py
--rw-rw-rw-   0        0        0     2134 2023-03-06 00:18:03.000000 dart-fss-0.4.3/dart_fss/utils/string.py
-drwxrwxrwx   0        0        0        0 2023-04-25 00:35:23.374163 dart-fss-0.4.3/dart_fss/xbrl/
--rw-rw-rw-   0        0        0       97 2023-03-06 00:18:03.000000 dart-fss-0.4.3/dart_fss/xbrl/__init__.py
--rw-rw-rw-   0        0        0    10993 2023-03-06 00:18:03.000000 dart-fss-0.4.3/dart_fss/xbrl/dart_xbrl.py
--rw-rw-rw-   0        0        0    12749 2023-03-06 00:18:03.000000 dart-fss-0.4.3/dart_fss/xbrl/helper.py
--rw-rw-rw-   0        0        0     9229 2023-03-31 07:17:35.000000 dart-fss-0.4.3/dart_fss/xbrl/table.py
--rw-rw-rw-   0        0        0     1441 2023-03-07 00:46:47.000000 dart-fss-0.4.3/dart_fss/xbrl/xbrl.py
-drwxrwxrwx   0        0        0        0 2023-04-25 00:35:22.885001 dart-fss-0.4.3/dart_fss.egg-info/
--rw-rw-rw-   0        0        0     3289 2023-04-25 00:35:22.000000 dart-fss-0.4.3/dart_fss.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     5450 2023-04-25 00:35:22.000000 dart-fss-0.4.3/dart_fss.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-25 00:35:22.000000 dart-fss-0.4.3/dart_fss.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      133 2023-04-25 00:35:22.000000 dart-fss-0.4.3/dart_fss.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-04-25 00:35:22.000000 dart-fss-0.4.3/dart_fss.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1162 2023-04-25 00:34:38.000000 dart-fss-0.4.3/pyproject.toml
--rw-rw-rw-   0        0        0      108 2023-04-24 05:30:51.000000 dart-fss-0.4.3/requirements.txt
--rw-rw-rw-   0        0        0      186 2023-04-25 00:35:23.377140 dart-fss-0.4.3/setup.cfg
--rw-rw-rw-   0        0        0      165 2023-04-24 04:56:16.000000 dart-fss-0.4.3/setup.py
--rw-rw-rw-   0        0        0    85812 2023-04-24 02:48:24.000000 dart-fss-0.4.3/versioneer.py
+drwxrwxrwx   0        0        0        0 2023-05-18 12:01:36.119124 dart-fss-0.4.4/
+-rw-rw-rw-   0        0        0     1093 2023-04-22 05:20:52.000000 dart-fss-0.4.4/LICENSE
+-rw-rw-rw-   0        0        0       77 2023-04-22 05:20:52.000000 dart-fss-0.4.4/MANIFEST.in
+-rw-rw-rw-   0        0        0     3289 2023-05-18 12:01:36.120145 dart-fss-0.4.4/PKG-INFO
+-rw-rw-rw-   0        0        0     2401 2023-04-22 05:20:52.000000 dart-fss-0.4.4/README.md
+drwxrwxrwx   0        0        0        0 2023-05-18 12:01:36.121138 dart-fss-0.4.4/dart_fss/
+-rw-rw-rw-   0        0        0      619 2023-04-23 02:15:37.000000 dart-fss-0.4.4/dart_fss/__init__.py
+-rw-rw-rw-   0        0        0      518 2023-05-18 12:01:36.121138 dart-fss-0.4.4/dart_fss/_version.py
+drwxrwxrwx   0        0        0        0 2023-05-18 12:01:35.940929 dart-fss-0.4.4/dart_fss/api/
+-rw-rw-rw-   0        0        0      224 2023-04-22 05:20:52.000000 dart-fss-0.4.4/dart_fss/api/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-18 12:01:35.947703 dart-fss-0.4.4/dart_fss/api/filings/
+-rw-rw-rw-   0        0        0      260 2023-04-22 05:20:52.000000 dart-fss-0.4.4/dart_fss/api/filings/__init__.py
+-rw-rw-rw-   0        0        0      396 2023-04-22 05:20:52.000000 dart-fss-0.4.4/dart_fss/api/filings/company.py
+-rw-rw-rw-   0        0        0     1320 2023-04-22 05:20:52.000000 dart-fss-0.4.4/dart_fss/api/filings/corp_code.py
+-rw-rw-rw-   0        0        0      686 2023-04-22 05:20:52.000000 dart-fss-0.4.4/dart_fss/api/filings/document.py
+-rw-rw-rw-   0        0        0     2680 2023-04-22 05:20:52.000000 dart-fss-0.4.4/dart_fss/api/filings/search_filings.py
+drwxrwxrwx   0        0        0        0 2023-05-18 12:01:35.954715 dart-fss-0.4.4/dart_fss/api/finance/
+-rw-rw-rw-   0        0        0      394 2023-04-22 05:20:52.000000 dart-fss-0.4.4/dart_fss/api/finance/__init__.py
+-rw-rw-rw-   0        0        0     1221 2023-04-22 05:20:52.000000 dart-fss-0.4.4/dart_fss/api/finance/fnltt_multi_acnt.py
+-rw-rw-rw-   0        0        0     1183 2023-04-22 05:20:52.000000 dart-fss-0.4.4/dart_fss/api/finance/fnltt_singl_acnt.py
+-rw-rw-rw-   0        0        0     1272 2023-04-22 05:20:52.000000 dart-fss-0.4.4/dart_fss/api/finance/fnltt_singl_acnt_all.py
+-rw-rw-rw-   0        0        0     1349 2023-04-22 05:20:52.000000 dart-fss-0.4.4/dart_fss/api/finance/xbrl.py
+-rw-rw-rw-   0        0        0      774 2023-04-22 05:20:52.000000 dart-fss-0.4.4/dart_fss/api/finance/xbrl_taxonomy.py
+-rw-rw-rw-   0        0        0     3692 2023-04-22 05:20:52.000000 dart-fss-0.4.4/dart_fss/api/helper.py
+drwxrwxrwx   0        0        0        0 2023-05-18 12:01:35.991870 dart-fss-0.4.4/dart_fss/api/info/
+-rw-rw-rw-   0        0        0     2590 2023-04-22 05:20:52.000000 dart-fss-0.4.4/dart_fss/api/info/__init__.py
+-rw-rw-rw-   0        0        0     1184 2023-04-22 05:20:52.000000 dart-fss-0.4.4/dart_fss/api/info/accnut_adtor_nm_nd_adt_opinion.py
+-rw-rw-rw-   0        0        0     1229 2023-04-22 05:20:52.000000 dart-fss-0.4.4/dart_fss/api/info/accnut_adtor_non_adt_servc_cncls_sttus.py
+-rw-rw-rw-   0        0        0     1132 2023-04-22 05:20:52.000000 dart-fss-0.4.4/dart_fss/api/info/adt_servc_cncls_sttus.py
+-rw-rw-rw-   0        0        0     1112 2023-04-22 05:20:52.000000 dart-fss-0.4.4/dart_fss/api/info/alot_matter.py
+-rw-rw-rw-   0        0        0     1173 2023-04-22 05:20:52.000000 dart-fss-0.4.4/dart_fss/api/info/cndl_capl_scrits_nrdmp_blce.py
+-rw-rw-rw-   0        0        0     1127 2023-04-22 05:20:52.000000 dart-fss-0.4.4/dart_fss/api/info/cprnd_nrdmp_blce.py
+-rw-rw-rw-   0        0        0     1134 2023-04-22 05:20:52.000000 dart-fss-0.4.4/dart_fss/api/info/det_scrits_isu_acmslt.py
+-rw-rw-rw-   0        0        0     1258 2023-04-22 05:20:52.000000 dart-fss-0.4.4/dart_fss/api/info/drctr_adt_all_mendng_sttus_gmtsck_confm_amount.py
+-rw-rw-rw-   0        0        0     1271 2023-04-22 05:20:52.000000 dart-fss-0.4.4/dart_fss/api/info/drctr_adt_all_mendng_sttus_mendng_pymntamt_ty_cl.py
+-rw-rw-rw-   0        0        0     1088 2023-04-22 05:20:52.000000 dart-fss-0.4.4/dart_fss/api/info/emp_sttus.py
+-rw-rw-rw-   0        0        0     1169 2023-04-22 05:20:52.000000 dart-fss-0.4.4/dart_fss/api/info/entrprs_bil_scrits_nrdmp_blce.py
+-rw-rw-rw-   0        0        0     1092 2023-04-22 05:20:52.000000 dart-fss-0.4.4/dart_fss/api/info/exctv_sttus.py
+-rw-rw-rw-   0        0        0     1154 2023-04-22 05:20:52.000000 dart-fss-0.4.4/dart_fss/api/info/hmv_audit_all_sttus.py
+-rw-rw-rw-   0        0        0     1173 2023-04-22 05:20:52.000000 dart-fss-0.4.4/dart_fss/api/info/hmv_audit_indvdl_by_sttus.py
+-rw-rw-rw-   0        0        0     1123 2023-04-22 05:20:52.000000 dart-fss-0.4.4/dart_fss/api/info/hyslr_chg_sttus.py
+-rw-rw-rw-   0        0        0     1104 2023-04-22 05:20:52.000000 dart-fss-0.4.4/dart_fss/api/info/hyslr_sttus.py
+-rw-rw-rw-   0        0        0     1174 2023-04-22 05:20:52.000000 dart-fss-0.4.4/dart_fss/api/info/indvdl_by_pay.py
+-rw-rw-rw-   0        0        0     1106 2023-04-22 05:20:52.000000 dart-fss-0.4.4/dart_fss/api/info/irds_sttus.py
+-rw-rw-rw-   0        0        0     1102 2023-04-22 05:20:52.000000 dart-fss-0.4.4/dart_fss/api/info/mrhl_sttus.py
+-rw-rw-rw-   0        0        0     1163 2023-04-22 05:20:52.000000 dart-fss-0.4.4/dart_fss/api/info/new_capl_scrits_nrdmp_blce.py
+-rw-rw-rw-   0        0        0     1130 2023-04-22 05:20:52.000000 dart-fss-0.4.4/dart_fss/api/info/otr_cpr_invstmnt_sttus.py
+-rw-rw-rw-   0        0        0     1167 2023-04-22 05:20:52.000000 dart-fss-0.4.4/dart_fss/api/info/outcmpny_drctr_nd_change_sttus.py
+-rw-rw-rw-   0        0        0     1140 2023-04-22 05:20:52.000000 dart-fss-0.4.4/dart_fss/api/info/prvsrp_cptal_use_dtls.py
+-rw-rw-rw-   0        0        0     1138 2023-04-22 05:20:52.000000 dart-fss-0.4.4/dart_fss/api/info/pssrp_cptal_use_dtls.py
+-rw-rw-rw-   0        0        0     1146 2023-04-22 05:20:52.000000 dart-fss-0.4.4/dart_fss/api/info/srtpd_psndbt_nrdmp_blce.py
+-rw-rw-rw-   0        0        0     1121 2023-04-22 05:20:52.000000 dart-fss-0.4.4/dart_fss/api/info/stock_totqy_sttus.py
+-rw-rw-rw-   0        0        0     1160 2023-04-22 05:20:52.000000 dart-fss-0.4.4/dart_fss/api/info/tesstk_acqs_dsps_sttus.py
+-rw-rw-rw-   0        0        0     1146 2023-04-22 05:20:52.000000 dart-fss-0.4.4/dart_fss/api/info/unrst_exctv_mendng_sttus.py
+drwxrwxrwx   0        0        0        0 2023-05-18 12:01:36.038324 dart-fss-0.4.4/dart_fss/api/issue/
+-rw-rw-rw-   0        0        0     2421 2023-04-22 05:20:52.000000 dart-fss-0.4.4/dart_fss/api/issue/__init__.py
+-rw-rw-rw-   0        0        0     1115 2023-04-22 05:20:52.000000 dart-fss-0.4.4/dart_fss/api/issue/ast_inhtrf_etc_ptbk_opt.py
+-rw-rw-rw-   0        0        0     1103 2023-04-22 05:20:52.000000 dart-fss-0.4.4/dart_fss/api/issue/bdwt_is_decsn.py
+-rw-rw-rw-   0        0        0     1101 2023-04-22 05:20:52.000000 dart-fss-0.4.4/dart_fss/api/issue/bnk_mngt_pcbg.py
+-rw-rw-rw-   0        0        0     1101 2023-04-22 05:20:52.000000 dart-fss-0.4.4/dart_fss/api/issue/bnk_mngt_pcsp.py
+-rw-rw-rw-   0        0        0     1061 2023-04-22 05:20:52.000000 dart-fss-0.4.4/dart_fss/api/issue/bsn_inh_decsn.py
+-rw-rw-rw-   0        0        0     1034 2023-04-22 05:20:52.000000 dart-fss-0.4.4/dart_fss/api/issue/bsn_sp.py
+-rw-rw-rw-   0        0        0     1061 2023-04-22 05:20:52.000000 dart-fss-0.4.4/dart_fss/api/issue/bsn_trf_decsn.py
+-rw-rw-rw-   0        0        0     1059 2023-04-22 05:20:52.000000 dart-fss-0.4.4/dart_fss/api/issue/cmp_dv_decsn.py
+-rw-rw-rw-   0        0        0     1075 2023-04-22 05:20:52.000000 dart-fss-0.4.4/dart_fss/api/issue/cmp_dvmg_decsn.py
+-rw-rw-rw-   0        0        0     1059 2023-04-22 05:20:52.000000 dart-fss-0.4.4/dart_fss/api/issue/cmp_mg_decsn.py
+-rw-rw-rw-   0        0        0     1040 2023-04-22 05:20:52.000000 dart-fss-0.4.4/dart_fss/api/issue/cr_decsn.py
+-rw-rw-rw-   0        0        0     1070 2023-04-22 05:20:52.000000 dart-fss-0.4.4/dart_fss/api/issue/ctrcvs_bgrq.py
+-rw-rw-rw-   0        0        0     1079 2023-04-22 05:20:52.000000 dart-fss-0.4.4/dart_fss/api/issue/cvbd_is_decsn.py
+-rw-rw-rw-   0        0        0     1034 2023-04-22 05:20:52.000000 dart-fss-0.4.4/dart_fss/api/issue/df_ocr.py
+-rw-rw-rw-   0        0        0     1053 2023-04-22 05:20:52.000000 dart-fss-0.4.4/dart_fss/api/issue/ds_rs_ocr.py
+-rw-rw-rw-   0        0        0     1079 2023-04-22 05:20:52.000000 dart-fss-0.4.4/dart_fss/api/issue/exbd_is_decsn.py
+-rw-rw-rw-   0        0        0     1056 2023-04-22 05:20:52.000000 dart-fss-0.4.4/dart_fss/api/issue/fric_decsn.py
+-rw-rw-rw-   0        0        0     1052 2023-04-22 05:20:52.000000 dart-fss-0.4.4/dart_fss/api/issue/lwst_lg.py
+-rw-rw-rw-   0        0        0     1139 2023-04-22 05:20:52.000000 dart-fss-0.4.4/dart_fss/api/issue/otcpr_stk_invscr_inh_decsn.py
+-rw-rw-rw-   0        0        0     1139 2023-04-22 05:20:52.000000 dart-fss-0.4.4/dart_fss/api/issue/otcpr_stk_invscr_trf_decsn.py
+-rw-rw-rw-   0        0        0     1096 2023-04-22 05:20:52.000000 dart-fss-0.4.4/dart_fss/api/issue/ov_dlst.py
+-rw-rw-rw-   0        0        0     1121 2023-04-22 05:20:52.000000 dart-fss-0.4.4/dart_fss/api/issue/ov_dlst_decsn.py
+-rw-rw-rw-   0        0        0     1082 2023-04-22 05:20:52.000000 dart-fss-0.4.4/dart_fss/api/issue/ov_lst.py
+-rw-rw-rw-   0        0        0     1107 2023-04-22 05:20:52.000000 dart-fss-0.4.4/dart_fss/api/issue/ov_lst_decsn.py
+-rw-rw-rw-   0        0        0     1066 2023-04-22 05:20:52.000000 dart-fss-0.4.4/dart_fss/api/issue/pifric_decsn.py
+-rw-rw-rw-   0        0        0     1056 2023-04-22 05:20:52.000000 dart-fss-0.4.4/dart_fss/api/issue/piic_decsn.py
+-rw-rw-rw-   0        0        0     1079 2023-04-22 05:20:52.000000 dart-fss-0.4.4/dart_fss/api/issue/stk_extr_decsn.py
+-rw-rw-rw-   0        0        0     1105 2023-04-22 05:20:52.000000 dart-fss-0.4.4/dart_fss/api/issue/stkrtbd_inh_decsn.py
+-rw-rw-rw-   0        0        0     1105 2023-04-22 05:20:52.000000 dart-fss-0.4.4/dart_fss/api/issue/stkrtbd_trf_decsn.py
+-rw-rw-rw-   0        0        0     1079 2023-04-22 05:20:52.000000 dart-fss-0.4.4/dart_fss/api/issue/tgast_inh_decsn.py
+-rw-rw-rw-   0        0        0     1079 2023-04-22 05:20:52.000000 dart-fss-0.4.4/dart_fss/api/issue/tgast_trf_decsn.py
+-rw-rw-rw-   0        0        0     1077 2023-04-22 05:20:52.000000 dart-fss-0.4.4/dart_fss/api/issue/tsstk_aq_decsn.py
+-rw-rw-rw-   0        0        0     1131 2023-04-22 05:20:52.000000 dart-fss-0.4.4/dart_fss/api/issue/tsstk_aq_trctr_cc_decsn.py
+-rw-rw-rw-   0        0        0     1133 2023-04-22 05:20:52.000000 dart-fss-0.4.4/dart_fss/api/issue/tsstk_aq_trctr_cns_decsn.py
+-rw-rw-rw-   0        0        0     1077 2023-04-22 05:20:52.000000 dart-fss-0.4.4/dart_fss/api/issue/tsstk_dp_decsn.py
+-rw-rw-rw-   0        0        0     1120 2023-04-22 05:20:52.000000 dart-fss-0.4.4/dart_fss/api/issue/wd_cocobd_is_decsn.py
+drwxrwxrwx   0        0        0        0 2023-05-18 12:01:36.041326 dart-fss-0.4.4/dart_fss/api/market/
+-rw-rw-rw-   0        0        0      187 2023-04-22 05:20:52.000000 dart-fss-0.4.4/dart_fss/api/market/__init__.py
+-rw-rw-rw-   0        0        0     2066 2023-04-22 05:20:52.000000 dart-fss-0.4.4/dart_fss/api/market/stock_market.py
+-rw-rw-rw-   0        0        0     2009 2023-04-22 05:20:52.000000 dart-fss-0.4.4/dart_fss/api/market/trading_halt.py
+drwxrwxrwx   0        0        0        0 2023-05-18 12:01:36.050326 dart-fss-0.4.4/dart_fss/api/registration/
+-rw-rw-rw-   0        0        0      306 2023-04-22 05:20:52.000000 dart-fss-0.4.4/dart_fss/api/registration/__init__.py
+-rw-rw-rw-   0        0        0     1026 2023-04-22 05:20:52.000000 dart-fss-0.4.4/dart_fss/api/registration/bd_rs.py
+-rw-rw-rw-   0        0        0     1014 2023-04-22 05:20:52.000000 dart-fss-0.4.4/dart_fss/api/registration/dv_rs.py
+-rw-rw-rw-   0        0        0     1030 2023-04-22 05:20:52.000000 dart-fss-0.4.4/dart_fss/api/registration/estk_rs.py
+-rw-rw-rw-   0        0        0     1070 2023-04-22 05:20:52.000000 dart-fss-0.4.4/dart_fss/api/registration/extr_rs.py
+-rw-rw-rw-   0        0        0     1014 2023-04-22 05:20:52.000000 dart-fss-0.4.4/dart_fss/api/registration/mg_rs.py
+-rw-rw-rw-   0        0        0     1044 2023-04-22 05:20:52.000000 dart-fss-0.4.4/dart_fss/api/registration/stkdp_rs.py
+drwxrwxrwx   0        0        0        0 2023-05-18 12:01:36.053973 dart-fss-0.4.4/dart_fss/api/shareholder/
+-rw-rw-rw-   0        0        0      149 2023-04-22 05:20:52.000000 dart-fss-0.4.4/dart_fss/api/shareholder/__init__.py
+-rw-rw-rw-   0        0        0      830 2023-04-22 05:20:52.000000 dart-fss-0.4.4/dart_fss/api/shareholder/elestock.py
+-rw-rw-rw-   0        0        0      794 2023-04-22 05:20:52.000000 dart-fss-0.4.4/dart_fss/api/shareholder/majorstock.py
+drwxrwxrwx   0        0        0        0 2023-05-18 12:01:36.055956 dart-fss-0.4.4/dart_fss/auth/
+-rw-rw-rw-   0        0        0      124 2023-04-22 05:20:52.000000 dart-fss-0.4.4/dart_fss/auth/__init__.py
+-rw-rw-rw-   0        0        0     2567 2023-04-22 05:20:52.000000 dart-fss-0.4.4/dart_fss/auth/auth.py
+drwxrwxrwx   0        0        0        0 2023-05-18 12:01:36.059842 dart-fss-0.4.4/dart_fss/corp/
+-rw-rw-rw-   0        0        0      172 2023-04-22 05:20:52.000000 dart-fss-0.4.4/dart_fss/corp/__init__.py
+-rw-rw-rw-   0        0        0     8929 2023-04-22 05:20:52.000000 dart-fss-0.4.4/dart_fss/corp/corp.py
+-rw-rw-rw-   0        0        0     9456 2023-04-22 05:20:52.000000 dart-fss-0.4.4/dart_fss/corp/corp_list.py
+drwxrwxrwx   0        0        0        0 2023-05-18 12:01:36.063841 dart-fss-0.4.4/dart_fss/errors/
+-rw-rw-rw-   0        0        0      459 2023-04-22 05:20:52.000000 dart-fss-0.4.4/dart_fss/errors/__init__.py
+-rw-rw-rw-   0        0        0     1514 2023-04-22 05:20:52.000000 dart-fss-0.4.4/dart_fss/errors/checker.py
+-rw-rw-rw-   0        0        0     1744 2023-04-22 05:20:52.000000 dart-fss-0.4.4/dart_fss/errors/errors.py
+drwxrwxrwx   0        0        0        0 2023-05-18 12:01:36.069841 dart-fss-0.4.4/dart_fss/filings/
+-rw-rw-rw-   0        0        0       91 2023-04-22 05:20:52.000000 dart-fss-0.4.4/dart_fss/filings/__init__.py
+-rw-rw-rw-   0        0        0     3897 2023-04-22 05:20:52.000000 dart-fss-0.4.4/dart_fss/filings/pages.py
+-rw-rw-rw-   0        0        0    20300 2023-04-22 05:20:52.000000 dart-fss-0.4.4/dart_fss/filings/reports.py
+-rw-rw-rw-   0        0        0     2513 2023-04-22 05:20:52.000000 dart-fss-0.4.4/dart_fss/filings/search.py
+-rw-rw-rw-   0        0        0     2124 2023-04-22 05:20:52.000000 dart-fss-0.4.4/dart_fss/filings/search_result.py
+drwxrwxrwx   0        0        0        0 2023-05-18 12:01:36.073841 dart-fss-0.4.4/dart_fss/fs/
+-rw-rw-rw-   0        0        0      158 2023-04-22 05:20:52.000000 dart-fss-0.4.4/dart_fss/fs/__init__.py
+-rw-rw-rw-   0        0        0    55366 2023-05-18 11:59:32.000000 dart-fss-0.4.4/dart_fss/fs/extract.py
+-rw-rw-rw-   0        0        0     7924 2023-04-22 05:20:52.000000 dart-fss-0.4.4/dart_fss/fs/fs.py
+drwxrwxrwx   0        0        0        0 2023-05-18 12:01:36.096624 dart-fss-0.4.4/dart_fss/tests/
+-rw-rw-rw-   0        0        0        0 2023-04-22 05:20:52.000000 dart-fss-0.4.4/dart_fss/tests/__init__.py
+-rw-rw-rw-   0        0        0      854 2023-04-22 05:20:52.000000 dart-fss-0.4.4/dart_fss/tests/test_api_filings.py
+-rw-rw-rw-   0        0        0     1721 2023-04-22 05:20:52.000000 dart-fss-0.4.4/dart_fss/tests/test_api_finance.py
+-rw-rw-rw-   0        0        0    10350 2023-04-22 05:20:52.000000 dart-fss-0.4.4/dart_fss/tests/test_api_info.py
+-rw-rw-rw-   0        0        0    12724 2023-04-22 05:20:52.000000 dart-fss-0.4.4/dart_fss/tests/test_api_issue.py
+-rw-rw-rw-   0        0        0      182 2023-04-22 05:20:52.000000 dart-fss-0.4.4/dart_fss/tests/test_api_market.py
+-rw-rw-rw-   0        0        0     2136 2023-04-22 05:20:52.000000 dart-fss-0.4.4/dart_fss/tests/test_api_registration.py
+-rw-rw-rw-   0        0        0      644 2023-04-22 05:20:52.000000 dart-fss-0.4.4/dart_fss/tests/test_api_shareholder.py
+-rw-rw-rw-   0        0        0       88 2023-04-22 05:20:52.000000 dart-fss-0.4.4/dart_fss/tests/test_auth.py
+drwxrwxrwx   0        0        0        0 2023-05-18 12:01:36.098997 dart-fss-0.4.4/dart_fss/tests/test_case/
+-rw-rw-rw-   0        0        0     5306 2023-04-22 05:20:52.000000 dart-fss-0.4.4/dart_fss/tests/test_case/crp_case.py
+-rw-rw-rw-   0        0        0     2998 2023-04-22 05:20:52.000000 dart-fss-0.4.4/dart_fss/tests/test_case/testcrp.py
+-rw-rw-rw-   0        0        0     2637 2023-04-22 05:20:52.000000 dart-fss-0.4.4/dart_fss/tests/test_corp.py
+-rw-rw-rw-   0        0        0     1004 2023-05-18 11:59:32.000000 dart-fss-0.4.4/dart_fss/tests/test_errors.py
+-rw-rw-rw-   0        0        0     4456 2023-05-18 11:59:32.000000 dart-fss-0.4.4/dart_fss/tests/test_fs.py
+-rw-rw-rw-   0        0        0      775 2023-04-22 05:20:52.000000 dart-fss-0.4.4/dart_fss/tests/test_fs_search.py
+-rw-rw-rw-   0        0        0      469 2023-04-22 05:20:52.000000 dart-fss-0.4.4/dart_fss/tests/test_regex.py
+-rw-rw-rw-   0        0        0     1320 2023-04-22 05:20:52.000000 dart-fss-0.4.4/dart_fss/tests/test_reports.py
+-rw-rw-rw-   0        0        0      804 2023-04-22 05:20:52.000000 dart-fss-0.4.4/dart_fss/tests/test_search_report.py
+-rw-rw-rw-   0        0        0      653 2023-04-22 05:20:52.000000 dart-fss-0.4.4/dart_fss/tests/test_utils.py
+-rw-rw-rw-   0        0        0     2706 2023-05-18 11:59:32.000000 dart-fss-0.4.4/dart_fss/tests/test_xbrl.py
+drwxrwxrwx   0        0        0        0 2023-05-18 12:01:36.113011 dart-fss-0.4.4/dart_fss/utils/
+-rw-rw-rw-   0        0        0     1277 2023-04-22 05:20:52.000000 dart-fss-0.4.4/dart_fss/utils/__init__.py
+-rw-rw-rw-   0        0        0      842 2023-04-22 05:20:52.000000 dart-fss-0.4.4/dart_fss/utils/cache.py
+-rw-rw-rw-   0        0        0      704 2023-04-22 05:20:52.000000 dart-fss-0.4.4/dart_fss/utils/dataframe.py
+-rw-rw-rw-   0        0        0     1434 2023-04-22 05:20:52.000000 dart-fss-0.4.4/dart_fss/utils/datetime.py
+-rw-rw-rw-   0        0        0     2666 2023-04-22 05:20:52.000000 dart-fss-0.4.4/dart_fss/utils/file.py
+-rw-rw-rw-   0        0        0     2733 2023-04-22 05:20:52.000000 dart-fss-0.4.4/dart_fss/utils/notebook.py
+-rw-rw-rw-   0        0        0     3077 2023-04-22 05:20:52.000000 dart-fss-0.4.4/dart_fss/utils/regex.py
+-rw-rw-rw-   0        0        0     7602 2023-04-22 05:20:52.000000 dart-fss-0.4.4/dart_fss/utils/request.py
+-rw-rw-rw-   0        0        0      304 2023-04-22 05:20:52.000000 dart-fss-0.4.4/dart_fss/utils/singleton.py
+-rw-rw-rw-   0        0        0     1019 2023-04-22 05:20:52.000000 dart-fss-0.4.4/dart_fss/utils/spinner.py
+-rw-rw-rw-   0        0        0     2134 2023-04-22 05:20:52.000000 dart-fss-0.4.4/dart_fss/utils/string.py
+drwxrwxrwx   0        0        0        0 2023-05-18 12:01:36.119124 dart-fss-0.4.4/dart_fss/xbrl/
+-rw-rw-rw-   0        0        0       97 2023-04-22 05:20:52.000000 dart-fss-0.4.4/dart_fss/xbrl/__init__.py
+-rw-rw-rw-   0        0        0    11016 2023-05-18 11:59:32.000000 dart-fss-0.4.4/dart_fss/xbrl/dart_xbrl.py
+-rw-rw-rw-   0        0        0    12749 2023-04-22 05:20:52.000000 dart-fss-0.4.4/dart_fss/xbrl/helper.py
+-rw-rw-rw-   0        0        0     9704 2023-05-18 11:59:32.000000 dart-fss-0.4.4/dart_fss/xbrl/table.py
+-rw-rw-rw-   0        0        0     1441 2023-04-22 05:20:52.000000 dart-fss-0.4.4/dart_fss/xbrl/xbrl.py
+drwxrwxrwx   0        0        0        0 2023-05-18 12:01:35.938912 dart-fss-0.4.4/dart_fss.egg-info/
+-rw-rw-rw-   0        0        0     3289 2023-05-18 12:01:35.000000 dart-fss-0.4.4/dart_fss.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     5450 2023-05-18 12:01:35.000000 dart-fss-0.4.4/dart_fss.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-18 12:01:35.000000 dart-fss-0.4.4/dart_fss.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      133 2023-05-18 12:01:35.000000 dart-fss-0.4.4/dart_fss.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-05-18 12:01:35.000000 dart-fss-0.4.4/dart_fss.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1162 2023-05-18 11:59:32.000000 dart-fss-0.4.4/pyproject.toml
+-rw-rw-rw-   0        0        0      108 2023-05-18 11:59:32.000000 dart-fss-0.4.4/requirements.txt
+-rw-rw-rw-   0        0        0      186 2023-05-18 12:01:36.120145 dart-fss-0.4.4/setup.cfg
+-rw-rw-rw-   0        0        0      165 2023-05-18 11:59:32.000000 dart-fss-0.4.4/setup.py
+-rw-rw-rw-   0        0        0    85812 2023-05-18 11:59:32.000000 dart-fss-0.4.4/versioneer.py
```

### Comparing `dart-fss-0.4.3/LICENSE` & `dart-fss-0.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `dart-fss-0.4.3/PKG-INFO` & `dart-fss-0.4.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dart-fss
-Version: 0.4.3
+Version: 0.4.4
 Summary: Web-scraping https://dart.fss.or.kr
 Author-email: Sungwoo Jo <nonswing.z@gmail.com>
 Maintainer-email: Sungwoo Jo <nonswing.z@gmail.com>
 License: MIT
 Project-URL: homepage, https://github.com/josw123/dart-fss
 Project-URL: documentation, https://dart-fss.readthedocs.io/
 Project-URL: repository, https://github.com/josw123/dart-fss.git
```

### Comparing `dart-fss-0.4.3/README.md` & `dart-fss-0.4.4/README.md`

 * *Files identical despite different names*

### Comparing `dart-fss-0.4.3/dart_fss/__init__.py` & `dart-fss-0.4.4/dart_fss/__init__.py`

 * *Files identical despite different names*

### Comparing `dart-fss-0.4.3/dart_fss/_version.py` & `dart-fss-0.4.4/dart_fss/_version.py`

 * *Files 26% similar despite different names*

```diff
@@ -4,18 +4,18 @@
 # unpacked source archive. Distribution tarballs contain a pre-generated copy
 # of this file.
 
 import json
 
 version_json = '''
 {
- "date": "2023-04-25T09:31:43+0900",
+ "date": "2023-05-18T20:54:42+0900",
  "dirty": false,
  "error": null,
- "full-revisionid": "3a8f0b92ad00f7bf811bd0f6549ad06ee9084f9e",
- "version": "0.4.3"
+ "full-revisionid": "086846b1ffac9f86fcdf0a98147da93b1b9aa3a4",
+ "version": "0.4.4"
 }
 '''  # END VERSION_JSON
 
 
 def get_versions():
     return json.loads(version_json)
```

### Comparing `dart-fss-0.4.3/dart_fss/api/filings/corp_code.py` & `dart-fss-0.4.4/dart_fss/api/filings/corp_code.py`

 * *Files identical despite different names*

### Comparing `dart-fss-0.4.3/dart_fss/api/filings/document.py` & `dart-fss-0.4.4/dart_fss/api/filings/document.py`

 * *Files identical despite different names*

### Comparing `dart-fss-0.4.3/dart_fss/api/filings/search_filings.py` & `dart-fss-0.4.4/dart_fss/api/filings/search_filings.py`

 * *Files identical despite different names*

### Comparing `dart-fss-0.4.3/dart_fss/api/finance/fnltt_multi_acnt.py` & `dart-fss-0.4.4/dart_fss/api/finance/fnltt_multi_acnt.py`

 * *Files identical despite different names*

### Comparing `dart-fss-0.4.3/dart_fss/api/finance/fnltt_singl_acnt.py` & `dart-fss-0.4.4/dart_fss/api/finance/fnltt_singl_acnt.py`

 * *Files identical despite different names*

### Comparing `dart-fss-0.4.3/dart_fss/api/finance/fnltt_singl_acnt_all.py` & `dart-fss-0.4.4/dart_fss/api/finance/fnltt_singl_acnt_all.py`

 * *Files identical despite different names*

### Comparing `dart-fss-0.4.3/dart_fss/api/finance/xbrl.py` & `dart-fss-0.4.4/dart_fss/api/finance/xbrl.py`

 * *Files identical despite different names*

### Comparing `dart-fss-0.4.3/dart_fss/api/finance/xbrl_taxonomy.py` & `dart-fss-0.4.4/dart_fss/api/finance/xbrl_taxonomy.py`

 * *Files identical despite different names*

### Comparing `dart-fss-0.4.3/dart_fss/api/helper.py` & `dart-fss-0.4.4/dart_fss/api/helper.py`

 * *Files identical despite different names*

### Comparing `dart-fss-0.4.3/dart_fss/api/info/__init__.py` & `dart-fss-0.4.4/dart_fss/api/info/__init__.py`

 * *Files identical despite different names*

### Comparing `dart-fss-0.4.3/dart_fss/api/info/accnut_adtor_nm_nd_adt_opinion.py` & `dart-fss-0.4.4/dart_fss/api/info/accnut_adtor_nm_nd_adt_opinion.py`

 * *Files identical despite different names*

### Comparing `dart-fss-0.4.3/dart_fss/api/info/accnut_adtor_non_adt_servc_cncls_sttus.py` & `dart-fss-0.4.4/dart_fss/api/info/accnut_adtor_non_adt_servc_cncls_sttus.py`

 * *Files identical despite different names*

### Comparing `dart-fss-0.4.3/dart_fss/api/info/adt_servc_cncls_sttus.py` & `dart-fss-0.4.4/dart_fss/api/info/adt_servc_cncls_sttus.py`

 * *Files identical despite different names*

### Comparing `dart-fss-0.4.3/dart_fss/api/info/alot_matter.py` & `dart-fss-0.4.4/dart_fss/api/info/alot_matter.py`

 * *Files identical despite different names*

### Comparing `dart-fss-0.4.3/dart_fss/api/info/cndl_capl_scrits_nrdmp_blce.py` & `dart-fss-0.4.4/dart_fss/api/info/cndl_capl_scrits_nrdmp_blce.py`

 * *Files identical despite different names*

### Comparing `dart-fss-0.4.3/dart_fss/api/info/cprnd_nrdmp_blce.py` & `dart-fss-0.4.4/dart_fss/api/info/cprnd_nrdmp_blce.py`

 * *Files identical despite different names*

### Comparing `dart-fss-0.4.3/dart_fss/api/info/det_scrits_isu_acmslt.py` & `dart-fss-0.4.4/dart_fss/api/info/det_scrits_isu_acmslt.py`

 * *Files identical despite different names*

### Comparing `dart-fss-0.4.3/dart_fss/api/info/drctr_adt_all_mendng_sttus_gmtsck_confm_amount.py` & `dart-fss-0.4.4/dart_fss/api/info/drctr_adt_all_mendng_sttus_gmtsck_confm_amount.py`

 * *Files identical despite different names*

### Comparing `dart-fss-0.4.3/dart_fss/api/info/drctr_adt_all_mendng_sttus_mendng_pymntamt_ty_cl.py` & `dart-fss-0.4.4/dart_fss/api/info/drctr_adt_all_mendng_sttus_mendng_pymntamt_ty_cl.py`

 * *Files identical despite different names*

### Comparing `dart-fss-0.4.3/dart_fss/api/info/emp_sttus.py` & `dart-fss-0.4.4/dart_fss/api/info/emp_sttus.py`

 * *Files identical despite different names*

### Comparing `dart-fss-0.4.3/dart_fss/api/info/entrprs_bil_scrits_nrdmp_blce.py` & `dart-fss-0.4.4/dart_fss/api/info/entrprs_bil_scrits_nrdmp_blce.py`

 * *Files identical despite different names*

### Comparing `dart-fss-0.4.3/dart_fss/api/info/exctv_sttus.py` & `dart-fss-0.4.4/dart_fss/api/info/exctv_sttus.py`

 * *Files identical despite different names*

### Comparing `dart-fss-0.4.3/dart_fss/api/info/hmv_audit_all_sttus.py` & `dart-fss-0.4.4/dart_fss/api/info/hmv_audit_all_sttus.py`

 * *Files identical despite different names*

### Comparing `dart-fss-0.4.3/dart_fss/api/info/hmv_audit_indvdl_by_sttus.py` & `dart-fss-0.4.4/dart_fss/api/info/hmv_audit_indvdl_by_sttus.py`

 * *Files identical despite different names*

### Comparing `dart-fss-0.4.3/dart_fss/api/info/hyslr_chg_sttus.py` & `dart-fss-0.4.4/dart_fss/api/info/hyslr_chg_sttus.py`

 * *Files identical despite different names*

### Comparing `dart-fss-0.4.3/dart_fss/api/info/hyslr_sttus.py` & `dart-fss-0.4.4/dart_fss/api/info/hyslr_sttus.py`

 * *Files identical despite different names*

### Comparing `dart-fss-0.4.3/dart_fss/api/info/indvdl_by_pay.py` & `dart-fss-0.4.4/dart_fss/api/info/indvdl_by_pay.py`

 * *Files identical despite different names*

### Comparing `dart-fss-0.4.3/dart_fss/api/info/irds_sttus.py` & `dart-fss-0.4.4/dart_fss/api/info/irds_sttus.py`

 * *Files identical despite different names*

### Comparing `dart-fss-0.4.3/dart_fss/api/info/mrhl_sttus.py` & `dart-fss-0.4.4/dart_fss/api/info/mrhl_sttus.py`

 * *Files identical despite different names*

### Comparing `dart-fss-0.4.3/dart_fss/api/info/new_capl_scrits_nrdmp_blce.py` & `dart-fss-0.4.4/dart_fss/api/info/new_capl_scrits_nrdmp_blce.py`

 * *Files identical despite different names*

### Comparing `dart-fss-0.4.3/dart_fss/api/info/otr_cpr_invstmnt_sttus.py` & `dart-fss-0.4.4/dart_fss/api/info/otr_cpr_invstmnt_sttus.py`

 * *Files identical despite different names*

### Comparing `dart-fss-0.4.3/dart_fss/api/info/outcmpny_drctr_nd_change_sttus.py` & `dart-fss-0.4.4/dart_fss/api/info/outcmpny_drctr_nd_change_sttus.py`

 * *Files identical despite different names*

### Comparing `dart-fss-0.4.3/dart_fss/api/info/prvsrp_cptal_use_dtls.py` & `dart-fss-0.4.4/dart_fss/api/info/prvsrp_cptal_use_dtls.py`

 * *Files identical despite different names*

### Comparing `dart-fss-0.4.3/dart_fss/api/info/pssrp_cptal_use_dtls.py` & `dart-fss-0.4.4/dart_fss/api/info/pssrp_cptal_use_dtls.py`

 * *Files identical despite different names*

### Comparing `dart-fss-0.4.3/dart_fss/api/info/srtpd_psndbt_nrdmp_blce.py` & `dart-fss-0.4.4/dart_fss/api/info/srtpd_psndbt_nrdmp_blce.py`

 * *Files identical despite different names*

### Comparing `dart-fss-0.4.3/dart_fss/api/info/stock_totqy_sttus.py` & `dart-fss-0.4.4/dart_fss/api/info/stock_totqy_sttus.py`

 * *Files identical despite different names*

### Comparing `dart-fss-0.4.3/dart_fss/api/info/tesstk_acqs_dsps_sttus.py` & `dart-fss-0.4.4/dart_fss/api/info/tesstk_acqs_dsps_sttus.py`

 * *Files identical despite different names*

### Comparing `dart-fss-0.4.3/dart_fss/api/info/unrst_exctv_mendng_sttus.py` & `dart-fss-0.4.4/dart_fss/api/info/unrst_exctv_mendng_sttus.py`

 * *Files identical despite different names*

### Comparing `dart-fss-0.4.3/dart_fss/api/issue/__init__.py` & `dart-fss-0.4.4/dart_fss/api/issue/__init__.py`

 * *Files identical despite different names*

### Comparing `dart-fss-0.4.3/dart_fss/api/issue/ast_inhtrf_etc_ptbk_opt.py` & `dart-fss-0.4.4/dart_fss/api/issue/ast_inhtrf_etc_ptbk_opt.py`

 * *Files identical despite different names*

### Comparing `dart-fss-0.4.3/dart_fss/api/issue/bdwt_is_decsn.py` & `dart-fss-0.4.4/dart_fss/api/issue/bdwt_is_decsn.py`

 * *Files identical despite different names*

### Comparing `dart-fss-0.4.3/dart_fss/api/issue/bnk_mngt_pcbg.py` & `dart-fss-0.4.4/dart_fss/api/issue/bnk_mngt_pcbg.py`

 * *Files identical despite different names*

### Comparing `dart-fss-0.4.3/dart_fss/api/issue/bnk_mngt_pcsp.py` & `dart-fss-0.4.4/dart_fss/api/issue/bnk_mngt_pcsp.py`

 * *Files identical despite different names*

### Comparing `dart-fss-0.4.3/dart_fss/api/issue/bsn_inh_decsn.py` & `dart-fss-0.4.4/dart_fss/api/issue/bsn_inh_decsn.py`

 * *Files identical despite different names*

### Comparing `dart-fss-0.4.3/dart_fss/api/issue/bsn_sp.py` & `dart-fss-0.4.4/dart_fss/api/issue/bsn_sp.py`

 * *Files identical despite different names*

### Comparing `dart-fss-0.4.3/dart_fss/api/issue/bsn_trf_decsn.py` & `dart-fss-0.4.4/dart_fss/api/issue/bsn_trf_decsn.py`

 * *Files identical despite different names*

### Comparing `dart-fss-0.4.3/dart_fss/api/issue/cmp_dv_decsn.py` & `dart-fss-0.4.4/dart_fss/api/issue/cmp_dv_decsn.py`

 * *Files identical despite different names*

### Comparing `dart-fss-0.4.3/dart_fss/api/issue/cmp_dvmg_decsn.py` & `dart-fss-0.4.4/dart_fss/api/issue/cmp_dvmg_decsn.py`

 * *Files identical despite different names*

### Comparing `dart-fss-0.4.3/dart_fss/api/issue/cmp_mg_decsn.py` & `dart-fss-0.4.4/dart_fss/api/issue/cmp_mg_decsn.py`

 * *Files identical despite different names*

### Comparing `dart-fss-0.4.3/dart_fss/api/issue/cr_decsn.py` & `dart-fss-0.4.4/dart_fss/api/issue/cr_decsn.py`

 * *Files identical despite different names*

### Comparing `dart-fss-0.4.3/dart_fss/api/issue/ctrcvs_bgrq.py` & `dart-fss-0.4.4/dart_fss/api/issue/ctrcvs_bgrq.py`

 * *Files identical despite different names*

### Comparing `dart-fss-0.4.3/dart_fss/api/issue/cvbd_is_decsn.py` & `dart-fss-0.4.4/dart_fss/api/issue/cvbd_is_decsn.py`

 * *Files identical despite different names*

### Comparing `dart-fss-0.4.3/dart_fss/api/issue/df_ocr.py` & `dart-fss-0.4.4/dart_fss/api/issue/df_ocr.py`

 * *Files identical despite different names*

### Comparing `dart-fss-0.4.3/dart_fss/api/issue/ds_rs_ocr.py` & `dart-fss-0.4.4/dart_fss/api/issue/ds_rs_ocr.py`

 * *Files identical despite different names*

### Comparing `dart-fss-0.4.3/dart_fss/api/issue/exbd_is_decsn.py` & `dart-fss-0.4.4/dart_fss/api/issue/exbd_is_decsn.py`

 * *Files identical despite different names*

### Comparing `dart-fss-0.4.3/dart_fss/api/issue/fric_decsn.py` & `dart-fss-0.4.4/dart_fss/api/issue/fric_decsn.py`

 * *Files identical despite different names*

### Comparing `dart-fss-0.4.3/dart_fss/api/issue/lwst_lg.py` & `dart-fss-0.4.4/dart_fss/api/issue/lwst_lg.py`

 * *Files identical despite different names*

### Comparing `dart-fss-0.4.3/dart_fss/api/issue/otcpr_stk_invscr_inh_decsn.py` & `dart-fss-0.4.4/dart_fss/api/issue/otcpr_stk_invscr_inh_decsn.py`

 * *Files identical despite different names*

### Comparing `dart-fss-0.4.3/dart_fss/api/issue/otcpr_stk_invscr_trf_decsn.py` & `dart-fss-0.4.4/dart_fss/api/issue/otcpr_stk_invscr_trf_decsn.py`

 * *Files identical despite different names*

### Comparing `dart-fss-0.4.3/dart_fss/api/issue/ov_dlst.py` & `dart-fss-0.4.4/dart_fss/api/issue/ov_dlst.py`

 * *Files identical despite different names*

### Comparing `dart-fss-0.4.3/dart_fss/api/issue/ov_dlst_decsn.py` & `dart-fss-0.4.4/dart_fss/api/issue/ov_dlst_decsn.py`

 * *Files identical despite different names*

### Comparing `dart-fss-0.4.3/dart_fss/api/issue/ov_lst.py` & `dart-fss-0.4.4/dart_fss/api/issue/ov_lst.py`

 * *Files identical despite different names*

### Comparing `dart-fss-0.4.3/dart_fss/api/issue/ov_lst_decsn.py` & `dart-fss-0.4.4/dart_fss/api/issue/ov_lst_decsn.py`

 * *Files identical despite different names*

### Comparing `dart-fss-0.4.3/dart_fss/api/issue/pifric_decsn.py` & `dart-fss-0.4.4/dart_fss/api/issue/pifric_decsn.py`

 * *Files identical despite different names*

### Comparing `dart-fss-0.4.3/dart_fss/api/issue/piic_decsn.py` & `dart-fss-0.4.4/dart_fss/api/issue/piic_decsn.py`

 * *Files identical despite different names*

### Comparing `dart-fss-0.4.3/dart_fss/api/issue/stk_extr_decsn.py` & `dart-fss-0.4.4/dart_fss/api/issue/stk_extr_decsn.py`

 * *Files identical despite different names*

### Comparing `dart-fss-0.4.3/dart_fss/api/issue/stkrtbd_inh_decsn.py` & `dart-fss-0.4.4/dart_fss/api/issue/stkrtbd_inh_decsn.py`

 * *Files identical despite different names*

### Comparing `dart-fss-0.4.3/dart_fss/api/issue/stkrtbd_trf_decsn.py` & `dart-fss-0.4.4/dart_fss/api/issue/stkrtbd_trf_decsn.py`

 * *Files identical despite different names*

### Comparing `dart-fss-0.4.3/dart_fss/api/issue/tgast_inh_decsn.py` & `dart-fss-0.4.4/dart_fss/api/issue/tgast_inh_decsn.py`

 * *Files identical despite different names*

### Comparing `dart-fss-0.4.3/dart_fss/api/issue/tgast_trf_decsn.py` & `dart-fss-0.4.4/dart_fss/api/issue/tgast_trf_decsn.py`

 * *Files identical despite different names*

### Comparing `dart-fss-0.4.3/dart_fss/api/issue/tsstk_aq_decsn.py` & `dart-fss-0.4.4/dart_fss/api/issue/tsstk_aq_decsn.py`

 * *Files identical despite different names*

### Comparing `dart-fss-0.4.3/dart_fss/api/issue/tsstk_aq_trctr_cc_decsn.py` & `dart-fss-0.4.4/dart_fss/api/issue/tsstk_aq_trctr_cc_decsn.py`

 * *Files identical despite different names*

### Comparing `dart-fss-0.4.3/dart_fss/api/issue/tsstk_aq_trctr_cns_decsn.py` & `dart-fss-0.4.4/dart_fss/api/issue/tsstk_aq_trctr_cns_decsn.py`

 * *Files identical despite different names*

### Comparing `dart-fss-0.4.3/dart_fss/api/issue/tsstk_dp_decsn.py` & `dart-fss-0.4.4/dart_fss/api/issue/tsstk_dp_decsn.py`

 * *Files identical despite different names*

### Comparing `dart-fss-0.4.3/dart_fss/api/issue/wd_cocobd_is_decsn.py` & `dart-fss-0.4.4/dart_fss/api/issue/wd_cocobd_is_decsn.py`

 * *Files identical despite different names*

### Comparing `dart-fss-0.4.3/dart_fss/api/market/stock_market.py` & `dart-fss-0.4.4/dart_fss/api/market/stock_market.py`

 * *Files identical despite different names*

### Comparing `dart-fss-0.4.3/dart_fss/api/market/trading_halt.py` & `dart-fss-0.4.4/dart_fss/api/market/trading_halt.py`

 * *Files identical despite different names*

### Comparing `dart-fss-0.4.3/dart_fss/api/registration/bd_rs.py` & `dart-fss-0.4.4/dart_fss/api/registration/bd_rs.py`

 * *Files identical despite different names*

### Comparing `dart-fss-0.4.3/dart_fss/api/registration/dv_rs.py` & `dart-fss-0.4.4/dart_fss/api/registration/dv_rs.py`

 * *Files identical despite different names*

### Comparing `dart-fss-0.4.3/dart_fss/api/registration/estk_rs.py` & `dart-fss-0.4.4/dart_fss/api/registration/estk_rs.py`

 * *Files identical despite different names*

### Comparing `dart-fss-0.4.3/dart_fss/api/registration/extr_rs.py` & `dart-fss-0.4.4/dart_fss/api/registration/extr_rs.py`

 * *Files identical despite different names*

### Comparing `dart-fss-0.4.3/dart_fss/api/registration/mg_rs.py` & `dart-fss-0.4.4/dart_fss/api/registration/mg_rs.py`

 * *Files identical despite different names*

### Comparing `dart-fss-0.4.3/dart_fss/api/registration/stkdp_rs.py` & `dart-fss-0.4.4/dart_fss/api/registration/stkdp_rs.py`

 * *Files identical despite different names*

### Comparing `dart-fss-0.4.3/dart_fss/api/shareholder/elestock.py` & `dart-fss-0.4.4/dart_fss/api/shareholder/elestock.py`

 * *Files identical despite different names*

### Comparing `dart-fss-0.4.3/dart_fss/api/shareholder/majorstock.py` & `dart-fss-0.4.4/dart_fss/api/shareholder/majorstock.py`

 * *Files identical despite different names*

### Comparing `dart-fss-0.4.3/dart_fss/auth/auth.py` & `dart-fss-0.4.4/dart_fss/auth/auth.py`

 * *Files identical despite different names*

### Comparing `dart-fss-0.4.3/dart_fss/corp/corp.py` & `dart-fss-0.4.4/dart_fss/corp/corp.py`

 * *Files identical despite different names*

### Comparing `dart-fss-0.4.3/dart_fss/corp/corp_list.py` & `dart-fss-0.4.4/dart_fss/corp/corp_list.py`

 * *Files identical despite different names*

### Comparing `dart-fss-0.4.3/dart_fss/errors/checker.py` & `dart-fss-0.4.4/dart_fss/errors/checker.py`

 * *Files identical despite different names*

### Comparing `dart-fss-0.4.3/dart_fss/errors/errors.py` & `dart-fss-0.4.4/dart_fss/errors/errors.py`

 * *Files identical despite different names*

### Comparing `dart-fss-0.4.3/dart_fss/filings/pages.py` & `dart-fss-0.4.4/dart_fss/filings/pages.py`

 * *Files identical despite different names*

### Comparing `dart-fss-0.4.3/dart_fss/filings/reports.py` & `dart-fss-0.4.4/dart_fss/filings/reports.py`

 * *Files identical despite different names*

### Comparing `dart-fss-0.4.3/dart_fss/filings/search.py` & `dart-fss-0.4.4/dart_fss/filings/search.py`

 * *Files identical despite different names*

### Comparing `dart-fss-0.4.3/dart_fss/filings/search_result.py` & `dart-fss-0.4.4/dart_fss/filings/search_result.py`

 * *Files identical despite different names*

### Comparing `dart-fss-0.4.3/dart_fss/fs/extract.py` & `dart-fss-0.4.4/dart_fss/fs/extract.py`

 * *Files 1% similar despite different names*

```diff
@@ -234,25 +234,33 @@
     # 최대 Col
     col_length = sum(th_colspan_list)
     # 최대 Row
     row_length = len(thead.find_all('tr'))
     row_length = row_length + 1 if row_length == 1 else row_length
     # row-sapn, col-span을 처리하기 위한 Matrix
     columns_matrix = [[None for _y in range(col_length)] for _x in range(row_length)]
+
+    # Bug fix (#141): Return an empty array if a duplicate column exists
+    duplicate_check = []
+
     for idx, tr in enumerate(thead.find_all('tr')):
         start_idx = 0
         for ele_idx, element in enumerate(columns_matrix[idx]):
             if element is None:
                 start_idx = ele_idx
                 break
 
         for jdx, th in enumerate(tr.find_all('th')):
             row_span = int(th.attrs.get('rowspan', 1))
             col_span = int(th.attrs.get('colspan', 1))
             text = re.sub(r'\s+', '', th.text)
+            # Bug fix (#141): Return an empty array if a duplicate column exists
+            if text in duplicate_check:
+                return []
+            duplicate_check.append(text)
             # Fix bug(#76)
             if len(text) == 0:
                 continue
             date_list = [datetime(1900, 1, 1)]
             if idx == 0:
                 if jdx == 0:
                     text = '과목'
@@ -272,14 +280,17 @@
             for mdx in range(row_span):
                 for ndx in range(col_span):
                     new_text = text
                     if mdx == 0 and regex.search(text):
                         new_text = fs_string[fs_tp]
                     columns_matrix[idx + mdx][start_idx + ndx] = new_text
             start_idx = start_idx + ndx + 1
+    # Bug fix (#141): Return an empty array if a duplicate '과목' exists
+    if len(columns_matrix) < 2 or columns_matrix[1].count('과목') > 1:
+        return []
 
     regex_3month = re.compile(r'3개월')
     regex_total = str_to_regex(r'누적 OR 금액')
 
     columns = []
 
     for jdx in range(len(columns_matrix[0])):
@@ -1120,15 +1131,16 @@
     option = {
         'label': 'Separate' if separate else 'Consolidated',
         'lang': lang,
         'show_abstract': show_abstract,
         'show_class': show_class,
         'show_depth': show_depth,
         'show_concept': show_concept,
-        'separator': separator
+        'separator': separator,
+        'ignore_subclass': True,# 하위 class 무시
     }
 
     statements = OrderedDict()
     for tp in fs_tp:
         statements[tp] = func_fs[tp]()
         if statements[tp]:
             statements[tp] = statements[tp].to_DataFrame(**option)
```

### Comparing `dart-fss-0.4.3/dart_fss/fs/fs.py` & `dart-fss-0.4.4/dart_fss/fs/fs.py`

 * *Files identical despite different names*

### Comparing `dart-fss-0.4.3/dart_fss/tests/test_api_filings.py` & `dart-fss-0.4.4/dart_fss/tests/test_api_filings.py`

 * *Files identical despite different names*

### Comparing `dart-fss-0.4.3/dart_fss/tests/test_api_finance.py` & `dart-fss-0.4.4/dart_fss/tests/test_api_finance.py`

 * *Files identical despite different names*

### Comparing `dart-fss-0.4.3/dart_fss/tests/test_api_info.py` & `dart-fss-0.4.4/dart_fss/tests/test_api_info.py`

 * *Files identical despite different names*

### Comparing `dart-fss-0.4.3/dart_fss/tests/test_api_issue.py` & `dart-fss-0.4.4/dart_fss/tests/test_api_issue.py`

 * *Files identical despite different names*

### Comparing `dart-fss-0.4.3/dart_fss/tests/test_api_registration.py` & `dart-fss-0.4.4/dart_fss/tests/test_api_registration.py`

 * *Files identical despite different names*

### Comparing `dart-fss-0.4.3/dart_fss/tests/test_api_shareholder.py` & `dart-fss-0.4.4/dart_fss/tests/test_api_shareholder.py`

 * *Files identical despite different names*

### Comparing `dart-fss-0.4.3/dart_fss/tests/test_case/crp_case.py` & `dart-fss-0.4.4/dart_fss/tests/test_case/crp_case.py`

 * *Files identical despite different names*

### Comparing `dart-fss-0.4.3/dart_fss/tests/test_case/testcrp.py` & `dart-fss-0.4.4/dart_fss/tests/test_case/testcrp.py`

 * *Files identical despite different names*

### Comparing `dart-fss-0.4.3/dart_fss/tests/test_corp.py` & `dart-fss-0.4.4/dart_fss/tests/test_corp.py`

 * *Files identical despite different names*

### Comparing `dart-fss-0.4.3/dart_fss/tests/test_errors.py` & `dart-fss-0.4.4/dart_fss/tests/test_errors.py`

 * *Files identical despite different names*

### Comparing `dart-fss-0.4.3/dart_fss/tests/test_fs.py` & `dart-fss-0.4.4/dart_fss/tests/test_fs.py`

 * *Files identical despite different names*

### Comparing `dart-fss-0.4.3/dart_fss/tests/test_fs_search.py` & `dart-fss-0.4.4/dart_fss/tests/test_fs_search.py`

 * *Files identical despite different names*

### Comparing `dart-fss-0.4.3/dart_fss/tests/test_reports.py` & `dart-fss-0.4.4/dart_fss/tests/test_reports.py`

 * *Files identical despite different names*

### Comparing `dart-fss-0.4.3/dart_fss/tests/test_search_report.py` & `dart-fss-0.4.4/dart_fss/tests/test_search_report.py`

 * *Files identical despite different names*

### Comparing `dart-fss-0.4.3/dart_fss/tests/test_utils.py` & `dart-fss-0.4.4/dart_fss/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `dart-fss-0.4.3/dart_fss/tests/test_xbrl.py` & `dart-fss-0.4.4/dart_fss/tests/test_xbrl.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,16 +33,16 @@
     actual = int(audit.iloc[5][3])
     expected = 260295
     assert actual == expected
 
 
 def test_xbrl_get_entity_information(samsung_xbrl):
     entity = samsung_xbrl.get_entity_information()
-    actual = entity.iloc[2][2]
-    expected = int(126380)
+    actual = int(entity.iloc[2][2])
+    expected = 126380
     assert actual == expected
 
 
 def test_xbrl_get_entity_address_information(samsung_xbrl):
     address = samsung_xbrl.get_entity_address_information()
     actual = address.iloc[2][2]
     expected = 'http://www.samsung.com/sec/'
```

### Comparing `dart-fss-0.4.3/dart_fss/utils/__init__.py` & `dart-fss-0.4.4/dart_fss/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `dart-fss-0.4.3/dart_fss/utils/cache.py` & `dart-fss-0.4.4/dart_fss/utils/cache.py`

 * *Files identical despite different names*

### Comparing `dart-fss-0.4.3/dart_fss/utils/dataframe.py` & `dart-fss-0.4.4/dart_fss/utils/dataframe.py`

 * *Files identical despite different names*

### Comparing `dart-fss-0.4.3/dart_fss/utils/datetime.py` & `dart-fss-0.4.4/dart_fss/utils/datetime.py`

 * *Files identical despite different names*

### Comparing `dart-fss-0.4.3/dart_fss/utils/file.py` & `dart-fss-0.4.4/dart_fss/utils/file.py`

 * *Files identical despite different names*

### Comparing `dart-fss-0.4.3/dart_fss/utils/notebook.py` & `dart-fss-0.4.4/dart_fss/utils/notebook.py`

 * *Files identical despite different names*

### Comparing `dart-fss-0.4.3/dart_fss/utils/regex.py` & `dart-fss-0.4.4/dart_fss/utils/regex.py`

 * *Files identical despite different names*

### Comparing `dart-fss-0.4.3/dart_fss/utils/request.py` & `dart-fss-0.4.4/dart_fss/utils/request.py`

 * *Files identical despite different names*

### Comparing `dart-fss-0.4.3/dart_fss/utils/spinner.py` & `dart-fss-0.4.4/dart_fss/utils/spinner.py`

 * *Files identical despite different names*

### Comparing `dart-fss-0.4.3/dart_fss/utils/string.py` & `dart-fss-0.4.4/dart_fss/utils/string.py`

 * *Files identical despite different names*

### Comparing `dart-fss-0.4.3/dart_fss/xbrl/dart_xbrl.py` & `dart-fss-0.4.4/dart_fss/xbrl/dart_xbrl.py`

 * *Files 1% similar despite different names*

```diff
@@ -87,15 +87,15 @@
 
         Returns
         -------
         DataFrame
             Pandas DataFrame
         """
         table = self.get_table_by_code(code)
-        return table.to_DataFrame(lang=lang, show_class=False, show_concept=False, separator=False)
+        return table.to_DataFrame(lang=lang, show_class=False, show_concept=False, separator=False, ignore_subclass=False)
 
     def get_document_information(self, lang: str = 'ko') -> DataFrame:
         """ 공시 문서 정보
 
         Parameters
         ----------
         lang: str
```

### Comparing `dart-fss-0.4.3/dart_fss/xbrl/helper.py` & `dart-fss-0.4.4/dart_fss/xbrl/helper.py`

 * *Files identical despite different names*

### Comparing `dart-fss-0.4.3/dart_fss/xbrl/table.py` & `dart-fss-0.4.4/dart_fss/xbrl/table.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # -*- coding: utf-8 -*-
 import re
 
+import numpy as np
 import pandas as pd
 from pandas import DataFrame
 
 from dateutil.relativedelta import relativedelta
 
 from arelle.ModelXbrl import ModelXbrl
 from arelle import XbrlConst
@@ -156,40 +157,41 @@
             for root_concept in relationship_set.rootConcepts:
                 labels = get_label_list(relationship_set, root_concept)
                 self._labels.append(labels)
         return self._labels
 
     def to_DataFrame(self, cls=None, lang='ko', start_dt=None, end_dt=None,
                      label=None, show_abstract=False, show_class=True, show_depth=10,
-                     show_concept=True, separator=True):
-        """ Pandas DataFrame으로 변환하는 함수
+                     show_concept=True, separator=True, ignore_subclass=True):
+        """ Pandas DataFrame으로 변환 하는 함수
 
         Parameters
         ----------
         cls: dict, optional
             classification
         lang: str, optional
             'ko' 한글 or 'en' 영문
         start_dt: str, optional
             검색 시작 일자
         end_dt: str, optional
             검색 종료 일자
         label: str, optional
-            Column Label에 포함될 단어
+            Column label에 포함될 단어
         show_abstract: bool, optional
-            abtract 표시 여부
+            abstract 표시 여부
         show_class: bool, optional
-            class 표시여부
+            class 표시 여부
         show_depth: int, optional
             class 표시 깊이
         show_concept: bool, optional
             concept_id 표시 여부
         separator: bool, optional
             숫자 첫단위 표시 여부
-
+        ignore_subclass: bool, optional
+            대분류인 연결재무제표 및 별도재무제표를 제외한 나머지 column의 표시 여부 (('연결재무제표', '자본금') / ('연결재무제표', '주식발행초과금') 등)
         Returns
         -------
         DataFrame
             재무제표 DataFrame
         """
         if cls is None:
             cls = self.cls_filter(start_dt, end_dt, label)
@@ -225,17 +227,22 @@
 
         regex_pass = str_to_regex('concept_id OR label_ko OR label_en OR class')
         df_count = df.count()
         drop_columns = []
         for key, count in df_count.items():
             if regex_pass.search(' '.join(key[1])):
                 pass
-            elif count <= 1:
+            elif count < 1:
                 drop_columns.append(key)
         df = df.drop(drop_columns, axis=1)
+
+        if ignore_subclass:
+            columns = np.array([x for x in df.columns if not isinstance(x[1], tuple) or len(x[1]) == 1], dtype=object)
+            return df[columns]
+
         return df
 
     def get_value_by_concept_id(self, concept_id, start_dt=None, end_dt=None, label=None, lang='en'):
         """ concept_id을 이용하여 값을 찾아 주는 함수
 
         Parameters
         ----------
```

### Comparing `dart-fss-0.4.3/dart_fss/xbrl/xbrl.py` & `dart-fss-0.4.4/dart_fss/xbrl/xbrl.py`

 * *Files identical despite different names*

### Comparing `dart-fss-0.4.3/dart_fss.egg-info/PKG-INFO` & `dart-fss-0.4.4/dart_fss.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dart-fss
-Version: 0.4.3
+Version: 0.4.4
 Summary: Web-scraping https://dart.fss.or.kr
 Author-email: Sungwoo Jo <nonswing.z@gmail.com>
 Maintainer-email: Sungwoo Jo <nonswing.z@gmail.com>
 License: MIT
 Project-URL: homepage, https://github.com/josw123/dart-fss
 Project-URL: documentation, https://dart-fss.readthedocs.io/
 Project-URL: repository, https://github.com/josw123/dart-fss.git
```

### Comparing `dart-fss-0.4.3/dart_fss.egg-info/SOURCES.txt` & `dart-fss-0.4.4/dart_fss.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dart-fss-0.4.3/pyproject.toml` & `dart-fss-0.4.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dart-fss-0.4.3/versioneer.py` & `dart-fss-0.4.4/versioneer.py`

 * *Files identical despite different names*

