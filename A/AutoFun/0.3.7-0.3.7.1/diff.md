# Comparing `tmp/AutoFun-0.3.7.tar.gz` & `tmp/AutoFun-0.3.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "AutoFun-0.3.7.tar", last modified: Tue May 16 03:36:29 2023, max compression
+gzip compressed data, was "AutoFun-0.3.7.1.tar", last modified: Thu May 18 04:41:00 2023, max compression
```

## Comparing `AutoFun-0.3.7.tar` & `AutoFun-0.3.7.1.tar`

### file list

```diff
@@ -1,68 +1,71 @@
-drwxrwxrwx   0        0        0        0 2023-05-16 03:36:29.668067 AutoFun-0.3.7/
-drwxrwxrwx   0        0        0        0 2023-05-16 03:36:29.536191 AutoFun-0.3.7/AutoFun/
--rw-rw-rw-   0        0        0    97792 2023-05-16 01:18:21.000000 AutoFun-0.3.7/AutoFun/AutoFun.pyd
-drwxrwxrwx   0        0        0        0 2023-05-16 03:36:29.549075 AutoFun-0.3.7/AutoFun/CutPdf/
--rw-rw-rw-   0        0        0   245760 2023-05-05 08:57:48.000000 AutoFun-0.3.7/AutoFun/CutPdf/CutPdf.pyd
-drwxrwxrwx   0        0        0        0 2023-05-16 03:36:29.554075 AutoFun-0.3.7/AutoFun/CutPdf/Function/
--rw-rw-rw-   0        0        0        0 2023-02-28 09:51:16.000000 AutoFun-0.3.7/AutoFun/CutPdf/Function/__init__.py
--rw-rw-rw-   0        0        0    69632 2023-05-05 03:08:24.000000 AutoFun-0.3.7/AutoFun/CutPdf/Function/optionDb.pyd
-drwxrwxrwx   0        0        0        0 2023-05-16 03:36:29.562072 AutoFun-0.3.7/AutoFun/CutPdf/Ui/
--rw-rw-rw-   0        0        0    98816 2023-05-05 03:08:08.000000 AutoFun-0.3.7/AutoFun/CutPdf/Ui/CutPdfPicUi.pyd
--rw-rw-rw-   0        0        0        0 2023-02-28 09:51:16.000000 AutoFun-0.3.7/AutoFun/CutPdf/Ui/__init__.py
--rw-rw-rw-   0        0        0        0 2023-02-28 09:51:16.000000 AutoFun-0.3.7/AutoFun/CutPdf/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-16 03:36:29.566072 AutoFun-0.3.7/AutoFun/OcrFinish/
--rw-rw-rw-   0        0        0   177664 2023-05-16 01:18:58.000000 AutoFun-0.3.7/AutoFun/OcrFinish/OcrFinish.pyd
-drwxrwxrwx   0        0        0        0 2023-05-16 03:36:29.573073 AutoFun-0.3.7/AutoFun/OcrFinish/Ui/
--rw-rw-rw-   0        0        0    56832 2023-05-05 03:14:46.000000 AutoFun-0.3.7/AutoFun/OcrFinish/Ui/OcrfinishUi.pyd
--rw-rw-rw-   0        0        0        0 2023-02-28 09:51:16.000000 AutoFun-0.3.7/AutoFun/OcrFinish/Ui/__init__.py
--rw-rw-rw-   0        0        0        0 2023-02-28 09:51:16.000000 AutoFun-0.3.7/AutoFun/OcrFinish/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-16 03:36:29.579083 AutoFun-0.3.7/AutoFun/OcrPicFun/
-drwxrwxrwx   0        0        0        0 2023-05-16 03:36:29.591072 AutoFun-0.3.7/AutoFun/OcrPicFun/Function/
--rw-rw-rw-   0        0        0        0 2023-02-28 09:51:16.000000 AutoFun-0.3.7/AutoFun/OcrPicFun/Function/__init__.py
--rw-rw-rw-   0        0        0    35328 2023-05-05 03:22:58.000000 AutoFun-0.3.7/AutoFun/OcrPicFun/Function/dict_to_json.pyd
--rw-rw-rw-   0        0        0    60416 2023-05-05 03:24:04.000000 AutoFun-0.3.7/AutoFun/OcrPicFun/Function/get_json.pyd
--rw-rw-rw-   0        0        0    42496 2023-05-05 03:25:20.000000 AutoFun-0.3.7/AutoFun/OcrPicFun/Function/splitJpg.pyd
--rw-rw-rw-   0        0        0   303616 2023-05-06 06:48:22.000000 AutoFun-0.3.7/AutoFun/OcrPicFun/OcrPicFun.pyd
-drwxrwxrwx   0        0        0        0 2023-05-16 03:36:29.596100 AutoFun-0.3.7/AutoFun/OcrPicFun/Ui/
--rw-rw-rw-   0        0        0    96256 2023-05-05 03:24:34.000000 AutoFun-0.3.7/AutoFun/OcrPicFun/Ui/OcrparameterUi.pyd
--rw-rw-rw-   0        0        0        0 2023-02-28 09:51:16.000000 AutoFun-0.3.7/AutoFun/OcrPicFun/Ui/__init__.py
--rw-rw-rw-   0        0        0        0 2023-02-28 09:51:16.000000 AutoFun-0.3.7/AutoFun/OcrPicFun/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-16 03:36:29.601086 AutoFun-0.3.7/AutoFun/OcrTableFun/
-drwxrwxrwx   0        0        0        0 2023-05-16 03:36:29.620067 AutoFun-0.3.7/AutoFun/OcrTableFun/Function/
--rw-rw-rw-   0        0        0    47616 2023-04-28 05:46:44.000000 AutoFun-0.3.7/AutoFun/OcrTableFun/Function/DB_in_sqlite.pyd
--rw-rw-rw-   0        0        0        0 2023-04-27 11:59:52.000000 AutoFun-0.3.7/AutoFun/OcrTableFun/Function/__init__.py
--rw-rw-rw-   0        0        0    69632 2023-04-28 05:47:22.000000 AutoFun-0.3.7/AutoFun/OcrTableFun/Function/optionDb.pyd
--rw-rw-rw-   0        0        0    18608 2023-05-05 09:10:40.000000 AutoFun-0.3.7/AutoFun/OcrTableFun/Function/saveLoad.py
--rw-rw-rw-   0        0        0   175104 2023-04-28 05:48:00.000000 AutoFun-0.3.7/AutoFun/OcrTableFun/Function/sqlite_to_excel.pyd
--rw-rw-rw-   0        0        0        0 2023-04-27 11:59:48.000000 AutoFun-0.3.7/AutoFun/OcrTableFun/Function/txt_OCR.db
--rw-rw-rw-   0        0        0   195584 2023-05-16 01:19:44.000000 AutoFun-0.3.7/AutoFun/OcrTableFun/OcrTableFun.pyd
-drwxrwxrwx   0        0        0        0 2023-05-16 03:36:29.626067 AutoFun-0.3.7/AutoFun/OcrTableFun/Ui/
--rw-rw-rw-   0        0        0    80384 2023-05-05 03:30:36.000000 AutoFun-0.3.7/AutoFun/OcrTableFun/Ui/OcrTableUi.pyd
--rw-rw-rw-   0        0        0        0 2023-04-27 11:59:50.000000 AutoFun-0.3.7/AutoFun/OcrTableFun/Ui/__init__.py
--rw-rw-rw-   0        0        0        0 2023-04-27 11:59:54.000000 AutoFun-0.3.7/AutoFun/OcrTableFun/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-16 03:36:29.632068 AutoFun-0.3.7/AutoFun/SplitPdfFun/
-drwxrwxrwx   0        0        0        0 2023-05-16 03:36:29.657067 AutoFun-0.3.7/AutoFun/SplitPdfFun/Function/
--rw-rw-rw-   0        0        0    47616 2023-04-28 05:51:40.000000 AutoFun-0.3.7/AutoFun/SplitPdfFun/Function/DB_in_sqlite.pyd
--rw-rw-rw-   0        0        0        0 2023-04-27 11:59:58.000000 AutoFun-0.3.7/AutoFun/SplitPdfFun/Function/__init__.py
--rw-rw-rw-   0        0        0    69632 2023-04-28 05:51:48.000000 AutoFun-0.3.7/AutoFun/SplitPdfFun/Function/optionDb.pyd
--rw-rw-rw-   0        0        0    70656 2023-04-28 05:51:56.000000 AutoFun-0.3.7/AutoFun/SplitPdfFun/Function/pdf_utils.pyd
--rw-rw-rw-   0        0        0   146944 2023-04-28 05:52:08.000000 AutoFun-0.3.7/AutoFun/SplitPdfFun/Function/splite_pdf.pyd
--rw-rw-rw-   0        0        0   122368 2023-04-28 05:52:20.000000 AutoFun-0.3.7/AutoFun/SplitPdfFun/Function/splite_pdf_no_Table.pyd
--rw-rw-rw-   0        0        0   169472 2023-04-28 05:52:32.000000 AutoFun-0.3.7/AutoFun/SplitPdfFun/Function/sqlite_to_excel.pyd
--rw-rw-rw-   0        0        0   167936 2023-05-12 08:06:13.000000 AutoFun-0.3.7/AutoFun/SplitPdfFun/SplitPdfFun.pyd
-drwxrwxrwx   0        0        0        0 2023-05-16 03:36:29.665077 AutoFun-0.3.7/AutoFun/SplitPdfFun/Ui/
--rw-rw-rw-   0        0        0    72192 2023-05-12 08:06:23.000000 AutoFun-0.3.7/AutoFun/SplitPdfFun/Ui/SplitPdfUi.pyd
--rw-rw-rw-   0        0        0        0 2023-04-27 12:00:00.000000 AutoFun-0.3.7/AutoFun/SplitPdfFun/Ui/__init__.py
--rw-rw-rw-   0        0        0        0 2023-04-27 11:59:58.000000 AutoFun-0.3.7/AutoFun/SplitPdfFun/__init__.py
--rw-rw-rw-   0        0        0        0 2023-02-28 09:51:16.000000 AutoFun-0.3.7/AutoFun/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-16 03:36:29.543191 AutoFun-0.3.7/AutoFun.egg-info/
--rw-rw-rw-   0        0        0      396 2023-05-16 03:36:29.000000 AutoFun-0.3.7/AutoFun.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1695 2023-05-16 03:36:29.000000 AutoFun-0.3.7/AutoFun.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-16 03:36:29.000000 AutoFun-0.3.7/AutoFun.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-05-16 03:36:29.000000 AutoFun-0.3.7/AutoFun.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1090 2022-12-21 02:47:10.000000 AutoFun-0.3.7/LICENSE.txt
--rw-rw-rw-   0        0        0       89 2022-12-21 03:16:16.000000 AutoFun-0.3.7/MANIFEST.in
--rw-rw-rw-   0        0        0      396 2023-05-16 03:36:29.668067 AutoFun-0.3.7/PKG-INFO
--rw-rw-rw-   0        0        0       33 2023-02-21 06:55:26.000000 AutoFun-0.3.7/README.md
--rw-rw-rw-   0        0        0      136 2023-05-16 03:36:29.669077 AutoFun-0.3.7/setup.cfg
--rw-rw-rw-   0        0        0      967 2023-05-16 03:36:17.000000 AutoFun-0.3.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-18 04:41:00.401832 AutoFun-0.3.7.1/
+drwxrwxrwx   0        0        0        0 2023-05-18 04:41:00.286004 AutoFun-0.3.7.1/AutoFun/
+-rw-rw-rw-   0        0        0    97792 2023-05-16 01:18:21.000000 AutoFun-0.3.7.1/AutoFun/AutoFun.pyd
+drwxrwxrwx   0        0        0        0 2023-05-18 04:41:00.298942 AutoFun-0.3.7.1/AutoFun/CutPdf/
+-rw-rw-rw-   0        0        0   245760 2023-05-05 08:57:48.000000 AutoFun-0.3.7.1/AutoFun/CutPdf/CutPdf.pyd
+drwxrwxrwx   0        0        0        0 2023-05-18 04:41:00.301945 AutoFun-0.3.7.1/AutoFun/CutPdf/Function/
+-rw-rw-rw-   0        0        0        0 2023-02-28 09:51:16.000000 AutoFun-0.3.7.1/AutoFun/CutPdf/Function/__init__.py
+-rw-rw-rw-   0        0        0    69632 2023-05-05 03:08:24.000000 AutoFun-0.3.7.1/AutoFun/CutPdf/Function/optionDb.pyd
+drwxrwxrwx   0        0        0        0 2023-05-18 04:41:00.307939 AutoFun-0.3.7.1/AutoFun/CutPdf/Ui/
+-rw-rw-rw-   0        0        0    98816 2023-05-05 03:08:08.000000 AutoFun-0.3.7.1/AutoFun/CutPdf/Ui/CutPdfPicUi.pyd
+-rw-rw-rw-   0        0        0        0 2023-02-28 09:51:16.000000 AutoFun-0.3.7.1/AutoFun/CutPdf/Ui/__init__.py
+-rw-rw-rw-   0        0        0        0 2023-02-28 09:51:16.000000 AutoFun-0.3.7.1/AutoFun/CutPdf/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-18 04:41:00.313982 AutoFun-0.3.7.1/AutoFun/OcrFinish/
+-rw-rw-rw-   0        0        0   177664 2023-05-16 01:18:58.000000 AutoFun-0.3.7.1/AutoFun/OcrFinish/OcrFinish.pyd
+drwxrwxrwx   0        0        0        0 2023-05-18 04:41:00.317986 AutoFun-0.3.7.1/AutoFun/OcrFinish/Ui/
+-rw-rw-rw-   0        0        0    56832 2023-05-05 03:14:46.000000 AutoFun-0.3.7.1/AutoFun/OcrFinish/Ui/OcrfinishUi.pyd
+-rw-rw-rw-   0        0        0        0 2023-02-28 09:51:16.000000 AutoFun-0.3.7.1/AutoFun/OcrFinish/Ui/__init__.py
+-rw-rw-rw-   0        0        0        0 2023-02-28 09:51:16.000000 AutoFun-0.3.7.1/AutoFun/OcrFinish/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-18 04:41:00.323866 AutoFun-0.3.7.1/AutoFun/OcrPicFun/
+drwxrwxrwx   0        0        0        0 2023-05-18 04:41:00.334831 AutoFun-0.3.7.1/AutoFun/OcrPicFun/Function/
+-rw-rw-rw-   0        0        0        0 2023-02-28 09:51:16.000000 AutoFun-0.3.7.1/AutoFun/OcrPicFun/Function/__init__.py
+-rw-rw-rw-   0        0        0    35328 2023-05-05 03:22:58.000000 AutoFun-0.3.7.1/AutoFun/OcrPicFun/Function/dict_to_json.pyd
+-rw-rw-rw-   0        0        0    60416 2023-05-05 03:24:04.000000 AutoFun-0.3.7.1/AutoFun/OcrPicFun/Function/get_json.pyd
+-rw-rw-rw-   0        0        0    42496 2023-05-05 03:25:20.000000 AutoFun-0.3.7.1/AutoFun/OcrPicFun/Function/splitJpg.pyd
+-rw-rw-rw-   0        0        0   303616 2023-05-06 06:48:22.000000 AutoFun-0.3.7.1/AutoFun/OcrPicFun/OcrPicFun.pyd
+drwxrwxrwx   0        0        0        0 2023-05-18 04:41:00.338830 AutoFun-0.3.7.1/AutoFun/OcrPicFun/Ui/
+-rw-rw-rw-   0        0        0    96256 2023-05-05 03:24:34.000000 AutoFun-0.3.7.1/AutoFun/OcrPicFun/Ui/OcrparameterUi.pyd
+-rw-rw-rw-   0        0        0        0 2023-02-28 09:51:16.000000 AutoFun-0.3.7.1/AutoFun/OcrPicFun/Ui/__init__.py
+-rw-rw-rw-   0        0        0        0 2023-02-28 09:51:16.000000 AutoFun-0.3.7.1/AutoFun/OcrPicFun/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-18 04:41:00.342835 AutoFun-0.3.7.1/AutoFun/OcrTableFun/
+drwxrwxrwx   0        0        0        0 2023-05-18 04:41:00.364832 AutoFun-0.3.7.1/AutoFun/OcrTableFun/Function/
+-rw-rw-rw-   0        0        0    47616 2023-04-28 05:46:44.000000 AutoFun-0.3.7.1/AutoFun/OcrTableFun/Function/DB_in_sqlite.pyd
+-rw-rw-rw-   0        0        0        0 2023-04-27 11:59:52.000000 AutoFun-0.3.7.1/AutoFun/OcrTableFun/Function/__init__.py
+-rw-rw-rw-   0        0        0    35157 2023-04-27 11:59:50.000000 AutoFun-0.3.7.1/AutoFun/OcrTableFun/Function/corpus.pickle
+-rw-rw-rw-   0        0        0    23954 2023-04-27 11:59:54.000000 AutoFun-0.3.7.1/AutoFun/OcrTableFun/Function/dictionary.dict
+-rw-rw-rw-   0        0        0    69632 2023-04-28 05:47:22.000000 AutoFun-0.3.7.1/AutoFun/OcrTableFun/Function/optionDb.pyd
+-rw-rw-rw-   0        0        0    18608 2023-05-05 09:10:40.000000 AutoFun-0.3.7.1/AutoFun/OcrTableFun/Function/saveLoad.py
+-rw-rw-rw-   0        0        0   175104 2023-04-28 05:48:00.000000 AutoFun-0.3.7.1/AutoFun/OcrTableFun/Function/sqlite_to_excel.pyd
+-rw-rw-rw-   0        0        0    28753 2023-04-27 11:59:50.000000 AutoFun-0.3.7.1/AutoFun/OcrTableFun/Function/tfidf.model
+-rw-rw-rw-   0        0        0        0 2023-04-27 11:59:48.000000 AutoFun-0.3.7.1/AutoFun/OcrTableFun/Function/txt_OCR.db
+-rw-rw-rw-   0        0        0   195584 2023-05-16 01:19:44.000000 AutoFun-0.3.7.1/AutoFun/OcrTableFun/OcrTableFun.pyd
+drwxrwxrwx   0        0        0        0 2023-05-18 04:41:00.368830 AutoFun-0.3.7.1/AutoFun/OcrTableFun/Ui/
+-rw-rw-rw-   0        0        0    80384 2023-05-05 03:30:36.000000 AutoFun-0.3.7.1/AutoFun/OcrTableFun/Ui/OcrTableUi.pyd
+-rw-rw-rw-   0        0        0        0 2023-04-27 11:59:50.000000 AutoFun-0.3.7.1/AutoFun/OcrTableFun/Ui/__init__.py
+-rw-rw-rw-   0        0        0        0 2023-04-27 11:59:54.000000 AutoFun-0.3.7.1/AutoFun/OcrTableFun/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-18 04:41:00.373834 AutoFun-0.3.7.1/AutoFun/SplitPdfFun/
+drwxrwxrwx   0        0        0        0 2023-05-18 04:41:00.392838 AutoFun-0.3.7.1/AutoFun/SplitPdfFun/Function/
+-rw-rw-rw-   0        0        0    47616 2023-04-28 05:51:40.000000 AutoFun-0.3.7.1/AutoFun/SplitPdfFun/Function/DB_in_sqlite.pyd
+-rw-rw-rw-   0        0        0        0 2023-04-27 11:59:58.000000 AutoFun-0.3.7.1/AutoFun/SplitPdfFun/Function/__init__.py
+-rw-rw-rw-   0        0        0    69632 2023-04-28 05:51:48.000000 AutoFun-0.3.7.1/AutoFun/SplitPdfFun/Function/optionDb.pyd
+-rw-rw-rw-   0        0        0    70656 2023-04-28 05:51:56.000000 AutoFun-0.3.7.1/AutoFun/SplitPdfFun/Function/pdf_utils.pyd
+-rw-rw-rw-   0        0        0   146944 2023-04-28 05:52:08.000000 AutoFun-0.3.7.1/AutoFun/SplitPdfFun/Function/splite_pdf.pyd
+-rw-rw-rw-   0        0        0   122368 2023-04-28 05:52:20.000000 AutoFun-0.3.7.1/AutoFun/SplitPdfFun/Function/splite_pdf_no_Table.pyd
+-rw-rw-rw-   0        0        0   169472 2023-04-28 05:52:32.000000 AutoFun-0.3.7.1/AutoFun/SplitPdfFun/Function/sqlite_to_excel.pyd
+-rw-rw-rw-   0        0        0   167936 2023-05-12 08:06:13.000000 AutoFun-0.3.7.1/AutoFun/SplitPdfFun/SplitPdfFun.pyd
+drwxrwxrwx   0        0        0        0 2023-05-18 04:41:00.399833 AutoFun-0.3.7.1/AutoFun/SplitPdfFun/Ui/
+-rw-rw-rw-   0        0        0    72192 2023-05-12 08:06:23.000000 AutoFun-0.3.7.1/AutoFun/SplitPdfFun/Ui/SplitPdfUi.pyd
+-rw-rw-rw-   0        0        0        0 2023-04-27 12:00:00.000000 AutoFun-0.3.7.1/AutoFun/SplitPdfFun/Ui/__init__.py
+-rw-rw-rw-   0        0        0        0 2023-04-27 11:59:58.000000 AutoFun-0.3.7.1/AutoFun/SplitPdfFun/__init__.py
+-rw-rw-rw-   0        0        0        0 2023-02-28 09:51:16.000000 AutoFun-0.3.7.1/AutoFun/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-18 04:41:00.292010 AutoFun-0.3.7.1/AutoFun.egg-info/
+-rw-rw-rw-   0        0        0      398 2023-05-18 04:41:00.000000 AutoFun-0.3.7.1/AutoFun.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1824 2023-05-18 04:41:00.000000 AutoFun-0.3.7.1/AutoFun.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-18 04:41:00.000000 AutoFun-0.3.7.1/AutoFun.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-05-18 04:41:00.000000 AutoFun-0.3.7.1/AutoFun.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1090 2022-12-21 02:47:10.000000 AutoFun-0.3.7.1/LICENSE.txt
+-rw-rw-rw-   0        0        0       89 2022-12-21 03:16:16.000000 AutoFun-0.3.7.1/MANIFEST.in
+-rw-rw-rw-   0        0        0      398 2023-05-18 04:41:00.401832 AutoFun-0.3.7.1/PKG-INFO
+-rw-rw-rw-   0        0        0       33 2023-02-21 06:55:26.000000 AutoFun-0.3.7.1/README.md
+-rw-rw-rw-   0        0        0      136 2023-05-18 04:41:00.402835 AutoFun-0.3.7.1/setup.cfg
+-rw-rw-rw-   0        0        0      998 2023-05-18 04:40:17.000000 AutoFun-0.3.7.1/setup.py
```

### Comparing `AutoFun-0.3.7/AutoFun/OcrTableFun/Function/saveLoad.py` & `AutoFun-0.3.7.1/AutoFun/OcrTableFun/Function/saveLoad.py`

 * *Files identical despite different names*

### Comparing `AutoFun-0.3.7/AutoFun.egg-info/SOURCES.txt` & `AutoFun-0.3.7.1/AutoFun.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -27,17 +27,20 @@
 AutoFun/OcrPicFun/Function/splitJpg.pyd
 AutoFun/OcrPicFun/Ui/OcrparameterUi.pyd
 AutoFun/OcrPicFun/Ui/__init__.py
 AutoFun/OcrTableFun/OcrTableFun.pyd
 AutoFun/OcrTableFun/__init__.py
 AutoFun/OcrTableFun/Function/DB_in_sqlite.pyd
 AutoFun/OcrTableFun/Function/__init__.py
+AutoFun/OcrTableFun/Function/corpus.pickle
+AutoFun/OcrTableFun/Function/dictionary.dict
 AutoFun/OcrTableFun/Function/optionDb.pyd
 AutoFun/OcrTableFun/Function/saveLoad.py
 AutoFun/OcrTableFun/Function/sqlite_to_excel.pyd
+AutoFun/OcrTableFun/Function/tfidf.model
 AutoFun/OcrTableFun/Function/txt_OCR.db
 AutoFun/OcrTableFun/Ui/OcrTableUi.pyd
 AutoFun/OcrTableFun/Ui/__init__.py
 AutoFun/SplitPdfFun/SplitPdfFun.pyd
 AutoFun/SplitPdfFun/__init__.py
 AutoFun/SplitPdfFun/Function/DB_in_sqlite.pyd
 AutoFun/SplitPdfFun/Function/__init__.py
```

### Comparing `AutoFun-0.3.7/LICENSE.txt` & `AutoFun-0.3.7.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `AutoFun-0.3.7/setup.py` & `AutoFun-0.3.7.1/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #-*- coding:utf-8 -*-
 import os 
 from setuptools import setup, find_packages
 
 MAJOR = 0
 MINOR = 3
 PATCH = 7
-VERSION = f"{MAJOR}.{MINOR}.{PATCH}"
+VERSION = f"{MAJOR}.{MINOR}.{PATCH}.1"
 
 def get_install_requires():
     reqs = []
     return reqs
 setup(
 	name = "AutoFun",
 	version = VERSION,
@@ -26,11 +26,11 @@
     packages=find_packages(),
     # license = '',
     classifiers=[
         'Programming Language :: Python',
 
     ],
     # 包含的类型
-    package_data={'': ['*.csv', '*.txt', '.toml', "*.pyd", '*.exe', '*.db']},  # 这个很重要
+    package_data={'': ['*.csv', '*.txt', '.toml', "*.pyd", '*.exe', '*.db', "*pickle", '*model','*dict']},  # 这个很重要
     include_package_data=True  # 也选上
 
 )
```

