# Comparing `tmp/python-pptx-valutico-0.6.24.2.tar.gz` & `tmp/python-pptx-valutico-0.6.24.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/andy/python-pptx/dist/tmp0hdhyrkm/python-pptx-valutico-0.6.24.2.tar", last modified: Mon May 16 16:04:17 2022, max compression
+gzip compressed data, was "python-pptx-valutico-0.6.24.3.tar", last modified: Thu May 18 16:21:08 2023, max compression
```

## Comparing `python-pptx-valutico-0.6.24.2.tar` & `python-pptx-valutico-0.6.24.3.tar`

### file list

```diff
@@ -1,563 +1,563 @@
-drwxr-xr-x   0 andy      (1000) andy      (1000)        0 2022-05-16 16:04:17.475551 python-pptx-valutico-0.6.24.2/
--rw-r--r--   0 andy      (1000) andy      (1000)    16294 2022-05-16 16:02:12.000000 python-pptx-valutico-0.6.24.2/HISTORY.rst
--rw-r--r--   0 andy      (1000) andy      (1000)     1116 2022-02-10 15:28:55.000000 python-pptx-valutico-0.6.24.2/LICENSE
--rw-r--r--   0 andy      (1000) andy      (1000)      177 2022-02-10 15:28:55.000000 python-pptx-valutico-0.6.24.2/MANIFEST.in
--rw-r--r--   0 andy      (1000) andy      (1000)    18286 2022-05-16 16:04:17.475551 python-pptx-valutico-0.6.24.2/PKG-INFO
--rw-r--r--   0 andy      (1000) andy      (1000)     1041 2022-02-10 15:28:55.000000 python-pptx-valutico-0.6.24.2/README.rst
-drwxr-xr-x   0 andy      (1000) andy      (1000)        0 2022-05-16 16:04:16.905552 python-pptx-valutico-0.6.24.2/features/
--rw-r--r--   0 andy      (1000) andy      (1000)     3215 2022-02-10 15:34:27.000000 python-pptx-valutico-0.6.24.2/features/act-action.feature
--rw-r--r--   0 andy      (1000) andy      (1000)     2045 2022-02-10 15:34:27.000000 python-pptx-valutico-0.6.24.2/features/act-hyperlink.feature
--rw-r--r--   0 andy      (1000) andy      (1000)     6389 2022-02-10 15:34:27.000000 python-pptx-valutico-0.6.24.2/features/cht-axis-props.feature
--rw-r--r--   0 andy      (1000) andy      (1000)     1360 2022-02-10 15:28:55.000000 python-pptx-valutico-0.6.24.2/features/cht-axistitle-props.feature
--rw-r--r--   0 andy      (1000) andy      (1000)     2059 2022-02-10 15:28:55.000000 python-pptx-valutico-0.6.24.2/features/cht-category-access.feature
--rw-r--r--   0 andy      (1000) andy      (1000)      569 2022-02-10 15:28:55.000000 python-pptx-valutico-0.6.24.2/features/cht-category-props.feature
--rw-r--r--   0 andy      (1000) andy      (1000)     4227 2022-02-10 15:28:55.000000 python-pptx-valutico-0.6.24.2/features/cht-chart.feature
--rw-r--r--   0 andy      (1000) andy      (1000)     1374 2022-02-10 15:28:55.000000 python-pptx-valutico-0.6.24.2/features/cht-charttitle-props.feature
--rw-r--r--   0 andy      (1000) andy      (1000)     4641 2022-02-10 15:28:55.000000 python-pptx-valutico-0.6.24.2/features/cht-data-props.feature
--rw-r--r--   0 andy      (1000) andy      (1000)     6935 2022-02-10 15:28:55.000000 python-pptx-valutico-0.6.24.2/features/cht-datalabels.feature
--rw-r--r--   0 andy      (1000) andy      (1000)      406 2022-02-10 15:28:55.000000 python-pptx-valutico-0.6.24.2/features/cht-gridlines-props.feature
--rw-r--r--   0 andy      (1000) andy      (1000)     1034 2022-02-10 15:28:55.000000 python-pptx-valutico-0.6.24.2/features/cht-legend-access.feature
--rw-r--r--   0 andy      (1000) andy      (1000)     3185 2022-02-10 15:28:55.000000 python-pptx-valutico-0.6.24.2/features/cht-legend-props.feature
--rw-r--r--   0 andy      (1000) andy      (1000)     1765 2022-02-10 15:28:55.000000 python-pptx-valutico-0.6.24.2/features/cht-marker-props.feature
--rw-r--r--   0 andy      (1000) andy      (1000)     4323 2022-02-10 15:28:55.000000 python-pptx-valutico-0.6.24.2/features/cht-plot-props.feature
--rw-r--r--   0 andy      (1000) andy      (1000)      945 2022-02-10 15:28:55.000000 python-pptx-valutico-0.6.24.2/features/cht-point-access.feature
--rw-r--r--   0 andy      (1000) andy      (1000)      566 2022-02-10 15:28:55.000000 python-pptx-valutico-0.6.24.2/features/cht-point-props.feature
--rw-r--r--   0 andy      (1000) andy      (1000)     1471 2022-02-10 15:28:55.000000 python-pptx-valutico-0.6.24.2/features/cht-replace-data.feature
--rw-r--r--   0 andy      (1000) andy      (1000)     4648 2022-02-10 15:28:55.000000 python-pptx-valutico-0.6.24.2/features/cht-series.feature
--rw-r--r--   0 andy      (1000) andy      (1000)      972 2022-02-10 15:28:55.000000 python-pptx-valutico-0.6.24.2/features/cht-ticklabels-props.feature
--rw-r--r--   0 andy      (1000) andy      (1000)      687 2022-02-10 15:28:55.000000 python-pptx-valutico-0.6.24.2/features/dml-color.feature
--rw-r--r--   0 andy      (1000) andy      (1000)     1018 2022-02-10 15:28:55.000000 python-pptx-valutico-0.6.24.2/features/dml-effect.feature
--rw-r--r--   0 andy      (1000) andy      (1000)     3098 2022-02-10 15:28:55.000000 python-pptx-valutico-0.6.24.2/features/dml-fill.feature
--rw-r--r--   0 andy      (1000) andy      (1000)     2163 2022-02-10 15:28:55.000000 python-pptx-valutico-0.6.24.2/features/dml-line.feature
--rw-r--r--   0 andy      (1000) andy      (1000)      518 2022-02-10 15:28:55.000000 python-pptx-valutico-0.6.24.2/features/environment.py
--rw-r--r--   0 andy      (1000) andy      (1000)     1602 2022-02-10 15:28:55.000000 python-pptx-valutico-0.6.24.2/features/ph-inherit-props.feature
--rw-r--r--   0 andy      (1000) andy      (1000)     1391 2022-02-10 15:28:55.000000 python-pptx-valutico-0.6.24.2/features/ph-insert-shape.feature
--rw-r--r--   0 andy      (1000) andy      (1000)      815 2022-02-10 15:28:55.000000 python-pptx-valutico-0.6.24.2/features/ph-phfmt-props.feature
--rw-r--r--   0 andy      (1000) andy      (1000)     1427 2022-02-10 15:28:55.000000 python-pptx-valutico-0.6.24.2/features/ph-placeholder-props.feature
--rw-r--r--   0 andy      (1000) andy      (1000)      992 2022-02-10 15:28:55.000000 python-pptx-valutico-0.6.24.2/features/prs-coreprops.feature
--rw-r--r--   0 andy      (1000) andy      (1000)      466 2022-02-10 15:28:55.000000 python-pptx-valutico-0.6.24.2/features/prs-default-template.feature
--rw-r--r--   0 andy      (1000) andy      (1000)     1417 2022-02-10 15:34:27.000000 python-pptx-valutico-0.6.24.2/features/prs-open-save.feature
--rw-r--r--   0 andy      (1000) andy      (1000)     1134 2022-02-10 15:28:55.000000 python-pptx-valutico-0.6.24.2/features/prs-presentation-props.feature
--rw-r--r--   0 andy      (1000) andy      (1000)      761 2022-02-10 15:28:55.000000 python-pptx-valutico-0.6.24.2/features/shp-autoshape.feature
--rw-r--r--   0 andy      (1000) andy      (1000)     2720 2022-02-10 15:28:55.000000 python-pptx-valutico-0.6.24.2/features/shp-connector.feature
--rw-r--r--   0 andy      (1000) andy      (1000)     2245 2022-02-10 15:28:55.000000 python-pptx-valutico-0.6.24.2/features/shp-freeform.feature
--rw-r--r--   0 andy      (1000) andy      (1000)     1622 2022-02-10 15:34:27.000000 python-pptx-valutico-0.6.24.2/features/shp-graphicframe.feature
--rw-r--r--   0 andy      (1000) andy      (1000)     1353 2022-02-10 15:28:55.000000 python-pptx-valutico-0.6.24.2/features/shp-groupshape.feature
--rw-r--r--   0 andy      (1000) andy      (1000)      568 2022-02-10 15:28:55.000000 python-pptx-valutico-0.6.24.2/features/shp-movie-props.feature
--rw-r--r--   0 andy      (1000) andy      (1000)     2475 2022-02-10 15:28:55.000000 python-pptx-valutico-0.6.24.2/features/shp-picture.feature
--rw-r--r--   0 andy      (1000) andy      (1000)      612 2022-02-10 15:28:55.000000 python-pptx-valutico-0.6.24.2/features/shp-placeholder.feature
--rw-r--r--   0 andy      (1000) andy      (1000)    14081 2022-02-10 15:34:27.000000 python-pptx-valutico-0.6.24.2/features/shp-shapes.feature
--rw-r--r--   0 andy      (1000) andy      (1000)     6239 2022-02-10 15:28:55.000000 python-pptx-valutico-0.6.24.2/features/shp-shared.feature
--rw-r--r--   0 andy      (1000) andy      (1000)      488 2022-02-10 15:28:55.000000 python-pptx-valutico-0.6.24.2/features/sld-background.feature
--rw-r--r--   0 andy      (1000) andy      (1000)     4081 2022-02-10 15:28:55.000000 python-pptx-valutico-0.6.24.2/features/sld-slide.feature
--rw-r--r--   0 andy      (1000) andy      (1000)     2339 2022-02-10 15:28:55.000000 python-pptx-valutico-0.6.24.2/features/sld-slides.feature
-drwxr-xr-x   0 andy      (1000) andy      (1000)        0 2022-05-16 16:04:16.915552 python-pptx-valutico-0.6.24.2/features/steps/
--rw-r--r--   0 andy      (1000) andy      (1000)     3317 2022-02-10 15:34:27.000000 python-pptx-valutico-0.6.24.2/features/steps/action.py
--rw-r--r--   0 andy      (1000) andy      (1000)    11392 2022-02-10 15:34:27.000000 python-pptx-valutico-0.6.24.2/features/steps/axis.py
--rw-r--r--   0 andy      (1000) andy      (1000)     1018 2022-02-10 15:28:55.000000 python-pptx-valutico-0.6.24.2/features/steps/background.py
--rw-r--r--   0 andy      (1000) andy      (1000)     6013 2022-02-10 15:28:55.000000 python-pptx-valutico-0.6.24.2/features/steps/category.py
--rw-r--r--   0 andy      (1000) andy      (1000)    13879 2022-02-10 15:28:55.000000 python-pptx-valutico-0.6.24.2/features/steps/chart.py
--rw-r--r--   0 andy      (1000) andy      (1000)     7343 2022-02-10 15:28:55.000000 python-pptx-valutico-0.6.24.2/features/steps/chartdata.py
--rw-r--r--   0 andy      (1000) andy      (1000)     2114 2022-02-10 15:28:55.000000 python-pptx-valutico-0.6.24.2/features/steps/color.py
--rw-r--r--   0 andy      (1000) andy      (1000)     2756 2022-02-10 15:34:27.000000 python-pptx-valutico-0.6.24.2/features/steps/coreprops.py
--rw-r--r--   0 andy      (1000) andy      (1000)     8097 2022-02-10 15:28:55.000000 python-pptx-valutico-0.6.24.2/features/steps/datalabel.py
--rw-r--r--   0 andy      (1000) andy      (1000)     1173 2022-02-10 15:28:55.000000 python-pptx-valutico-0.6.24.2/features/steps/effect.py
--rw-r--r--   0 andy      (1000) andy      (1000)     5143 2022-02-10 15:28:55.000000 python-pptx-valutico-0.6.24.2/features/steps/fill.py
--rw-r--r--   0 andy      (1000) andy      (1000)     4980 2022-02-10 15:28:55.000000 python-pptx-valutico-0.6.24.2/features/steps/font.py
--rw-r--r--   0 andy      (1000) andy      (1000)     3371 2022-02-10 15:28:55.000000 python-pptx-valutico-0.6.24.2/features/steps/font_color.py
--rw-r--r--   0 andy      (1000) andy      (1000)     1523 2022-02-10 15:28:55.000000 python-pptx-valutico-0.6.24.2/features/steps/helpers.py
--rw-r--r--   0 andy      (1000) andy      (1000)     3144 2022-02-10 15:28:55.000000 python-pptx-valutico-0.6.24.2/features/steps/legend.py
--rw-r--r--   0 andy      (1000) andy      (1000)     3245 2022-02-10 15:28:55.000000 python-pptx-valutico-0.6.24.2/features/steps/line.py
--rw-r--r--   0 andy      (1000) andy      (1000)     2803 2022-02-10 15:34:27.000000 python-pptx-valutico-0.6.24.2/features/steps/picture.py
--rw-r--r--   0 andy      (1000) andy      (1000)    11179 2022-02-10 15:28:55.000000 python-pptx-valutico-0.6.24.2/features/steps/placeholder.py
--rw-r--r--   0 andy      (1000) andy      (1000)     4809 2022-02-10 15:28:55.000000 python-pptx-valutico-0.6.24.2/features/steps/plot.py
--rw-r--r--   0 andy      (1000) andy      (1000)     6035 2022-02-10 15:34:27.000000 python-pptx-valutico-0.6.24.2/features/steps/presentation.py
--rw-r--r--   0 andy      (1000) andy      (1000)    12340 2022-02-10 15:28:55.000000 python-pptx-valutico-0.6.24.2/features/steps/series.py
--rw-r--r--   0 andy      (1000) andy      (1000)    22389 2022-02-10 15:34:27.000000 python-pptx-valutico-0.6.24.2/features/steps/shape.py
--rw-r--r--   0 andy      (1000) andy      (1000)    12099 2022-02-10 15:34:27.000000 python-pptx-valutico-0.6.24.2/features/steps/shapes.py
--rw-r--r--   0 andy      (1000) andy      (1000)     7570 2022-02-10 15:28:55.000000 python-pptx-valutico-0.6.24.2/features/steps/slide.py
--rw-r--r--   0 andy      (1000) andy      (1000)     4644 2022-02-10 15:28:55.000000 python-pptx-valutico-0.6.24.2/features/steps/slides.py
--rw-r--r--   0 andy      (1000) andy      (1000)    10292 2022-02-10 15:28:55.000000 python-pptx-valutico-0.6.24.2/features/steps/table.py
-drwxr-xr-x   0 andy      (1000) andy      (1000)        0 2022-05-16 16:04:17.145552 python-pptx-valutico-0.6.24.2/features/steps/test_files/
--rw-r--r--   0 andy      (1000) andy      (1000)     9454 2022-02-10 15:28:55.000000 python-pptx-valutico-0.6.24.2/features/steps/test_files/72-dpi.tiff
--rw-r--r--   0 andy      (1000) andy      (1000)     1526 2022-02-10 15:28:55.000000 python-pptx-valutico-0.6.24.2/features/steps/test_files/CVS_LOGO.WMF
--rw-r--r--   0 andy      (1000) andy      (1000)   982098 2022-02-10 15:34:27.000000 python-pptx-valutico-0.6.24.2/features/steps/test_files/act-props.pptm
--rw-r--r--   0 andy      (1000) andy      (1000)   867288 2022-02-10 15:28:55.000000 python-pptx-valutico-0.6.24.2/features/steps/test_files/calibriz.ttf
--rw-r--r--   0 andy      (1000) andy      (1000)   366536 2022-02-10 15:34:27.000000 python-pptx-valutico-0.6.24.2/features/steps/test_files/cht-axis-props.pptx
--rw-r--r--   0 andy      (1000) andy      (1000)   222711 2022-02-10 15:28:55.000000 python-pptx-valutico-0.6.24.2/features/steps/test_files/cht-category-access.pptx
--rw-r--r--   0 andy      (1000) andy      (1000)   218303 2022-02-10 15:28:55.000000 python-pptx-valutico-0.6.24.2/features/steps/test_files/cht-chart-props.pptx
--rw-r--r--   0 andy      (1000) andy      (1000)  1393564 2022-02-10 15:28:55.000000 python-pptx-valutico-0.6.24.2/features/steps/test_files/cht-chart-type.pptx
--rw-r--r--   0 andy      (1000) andy      (1000)    77751 2022-02-10 15:28:55.000000 python-pptx-valutico-0.6.24.2/features/steps/test_files/cht-charts.pptx
--rw-r--r--   0 andy      (1000) andy      (1000)   243765 2022-02-10 15:28:55.000000 python-pptx-valutico-0.6.24.2/features/steps/test_files/cht-datalabels.pptx
--rw-r--r--   0 andy      (1000) andy      (1000)    62864 2022-02-10 15:28:55.000000 python-pptx-valutico-0.6.24.2/features/steps/test_files/cht-gridlines-props.pptx
--rw-r--r--   0 andy      (1000) andy      (1000)   145467 2022-02-10 15:28:55.000000 python-pptx-valutico-0.6.24.2/features/steps/test_files/cht-legend-props.pptx
--rw-r--r--   0 andy      (1000) andy      (1000)   125134 2022-02-10 15:28:55.000000 python-pptx-valutico-0.6.24.2/features/steps/test_files/cht-legend.pptx
--rw-r--r--   0 andy      (1000) andy      (1000)    78544 2022-02-10 15:28:55.000000 python-pptx-valutico-0.6.24.2/features/steps/test_files/cht-marker-props.pptx
--rw-r--r--   0 andy      (1000) andy      (1000)   214116 2022-02-10 15:28:55.000000 python-pptx-valutico-0.6.24.2/features/steps/test_files/cht-plot-props.pptx
--rw-r--r--   0 andy      (1000) andy      (1000)   145108 2022-02-10 15:28:55.000000 python-pptx-valutico-0.6.24.2/features/steps/test_files/cht-point-access.pptx
--rw-r--r--   0 andy      (1000) andy      (1000)   144812 2022-02-10 15:28:55.000000 python-pptx-valutico-0.6.24.2/features/steps/test_files/cht-point-props.pptx
--rw-r--r--   0 andy      (1000) andy      (1000)   323685 2022-02-10 15:28:55.000000 python-pptx-valutico-0.6.24.2/features/steps/test_files/cht-replace-data.pptx
--rw-r--r--   0 andy      (1000) andy      (1000)   518464 2022-02-10 15:28:55.000000 python-pptx-valutico-0.6.24.2/features/steps/test_files/cht-series.pptx
--rw-r--r--   0 andy      (1000) andy      (1000)   127056 2022-02-10 15:28:55.000000 python-pptx-valutico-0.6.24.2/features/steps/test_files/cht-ticklabels-props.pptx
--rw-r--r--   0 andy      (1000) andy      (1000)    21620 2022-02-10 15:28:55.000000 python-pptx-valutico-0.6.24.2/features/steps/test_files/dml-effect.pptx
--rw-r--r--   0 andy      (1000) andy      (1000)   778084 2022-02-10 15:28:55.000000 python-pptx-valutico-0.6.24.2/features/steps/test_files/dml-fill.pptx
--rw-r--r--   0 andy      (1000) andy      (1000)    27246 2022-02-10 15:28:55.000000 python-pptx-valutico-0.6.24.2/features/steps/test_files/dml-line.pptx
--rw-r--r--   0 andy      (1000) andy      (1000)    21457 2022-02-10 15:28:55.000000 python-pptx-valutico-0.6.24.2/features/steps/test_files/ext-rels.pptx
-drwxr-xr-x   0 andy      (1000) andy      (1000)        0 2022-05-16 16:04:17.145552 python-pptx-valutico-0.6.24.2/features/steps/test_files/extracted-pptx/
--rw-r--r--   0 andy      (1000) andy      (1000)     3332 2022-02-10 15:34:27.000000 python-pptx-valutico-0.6.24.2/features/steps/test_files/extracted-pptx/[Content_Types].xml
-drwxr-xr-x   0 andy      (1000) andy      (1000)        0 2022-05-16 16:04:17.145552 python-pptx-valutico-0.6.24.2/features/steps/test_files/extracted-pptx/_rels/
--rw-r--r--   0 andy      (1000) andy      (1000)      751 2022-02-10 15:34:27.000000 python-pptx-valutico-0.6.24.2/features/steps/test_files/extracted-pptx/_rels/.rels
-drwxr-xr-x   0 andy      (1000) andy      (1000)        0 2022-05-16 16:04:17.145552 python-pptx-valutico-0.6.24.2/features/steps/test_files/extracted-pptx/docProps/
--rw-r--r--   0 andy      (1000) andy      (1000)     1356 2022-02-10 15:34:27.000000 python-pptx-valutico-0.6.24.2/features/steps/test_files/extracted-pptx/docProps/app.xml
--rw-r--r--   0 andy      (1000) andy      (1000)      765 2022-02-10 15:34:27.000000 python-pptx-valutico-0.6.24.2/features/steps/test_files/extracted-pptx/docProps/core.xml
--rw-r--r--   0 andy      (1000) andy      (1000)     8147 2022-02-10 15:34:27.000000 python-pptx-valutico-0.6.24.2/features/steps/test_files/extracted-pptx/docProps/thumbnail.jpeg
-drwxr-xr-x   0 andy      (1000) andy      (1000)        0 2022-05-16 16:04:17.155552 python-pptx-valutico-0.6.24.2/features/steps/test_files/extracted-pptx/ppt/
-drwxr-xr-x   0 andy      (1000) andy      (1000)        0 2022-05-16 16:04:17.155552 python-pptx-valutico-0.6.24.2/features/steps/test_files/extracted-pptx/ppt/_rels/
--rw-r--r--   0 andy      (1000) andy      (1000)     1160 2022-02-10 15:34:27.000000 python-pptx-valutico-0.6.24.2/features/steps/test_files/extracted-pptx/ppt/_rels/presentation.xml.rels
--rw-r--r--   0 andy      (1000) andy      (1000)      692 2022-02-10 15:34:27.000000 python-pptx-valutico-0.6.24.2/features/steps/test_files/extracted-pptx/ppt/presProps.xml
--rw-r--r--   0 andy      (1000) andy      (1000)     4000 2022-02-10 15:34:27.000000 python-pptx-valutico-0.6.24.2/features/steps/test_files/extracted-pptx/ppt/presentation.xml
-drwxr-xr-x   0 andy      (1000) andy      (1000)        0 2022-05-16 16:04:17.165552 python-pptx-valutico-0.6.24.2/features/steps/test_files/extracted-pptx/ppt/printerSettings/
--rw-r--r--   0 andy      (1000) andy      (1000)     9395 2022-02-10 15:34:27.000000 python-pptx-valutico-0.6.24.2/features/steps/test_files/extracted-pptx/ppt/printerSettings/printerSettings1.bin
-drwxr-xr-x   0 andy      (1000) andy      (1000)        0 2022-05-16 16:04:17.185552 python-pptx-valutico-0.6.24.2/features/steps/test_files/extracted-pptx/ppt/slideLayouts/
-drwxr-xr-x   0 andy      (1000) andy      (1000)        0 2022-05-16 16:04:17.195551 python-pptx-valutico-0.6.24.2/features/steps/test_files/extracted-pptx/ppt/slideLayouts/_rels/
--rw-r--r--   0 andy      (1000) andy      (1000)      315 2022-02-10 15:34:27.000000 python-pptx-valutico-0.6.24.2/features/steps/test_files/extracted-pptx/ppt/slideLayouts/_rels/slideLayout1.xml.rels
--rw-r--r--   0 andy      (1000) andy      (1000)      315 2022-02-10 15:34:27.000000 python-pptx-valutico-0.6.24.2/features/steps/test_files/extracted-pptx/ppt/slideLayouts/_rels/slideLayout10.xml.rels
--rw-r--r--   0 andy      (1000) andy      (1000)      315 2022-02-10 15:34:27.000000 python-pptx-valutico-0.6.24.2/features/steps/test_files/extracted-pptx/ppt/slideLayouts/_rels/slideLayout11.xml.rels
--rw-r--r--   0 andy      (1000) andy      (1000)      315 2022-02-10 15:34:27.000000 python-pptx-valutico-0.6.24.2/features/steps/test_files/extracted-pptx/ppt/slideLayouts/_rels/slideLayout2.xml.rels
--rw-r--r--   0 andy      (1000) andy      (1000)      315 2022-02-10 15:34:27.000000 python-pptx-valutico-0.6.24.2/features/steps/test_files/extracted-pptx/ppt/slideLayouts/_rels/slideLayout3.xml.rels
--rw-r--r--   0 andy      (1000) andy      (1000)      315 2022-02-10 15:34:27.000000 python-pptx-valutico-0.6.24.2/features/steps/test_files/extracted-pptx/ppt/slideLayouts/_rels/slideLayout4.xml.rels
--rw-r--r--   0 andy      (1000) andy      (1000)      315 2022-02-10 15:34:27.000000 python-pptx-valutico-0.6.24.2/features/steps/test_files/extracted-pptx/ppt/slideLayouts/_rels/slideLayout5.xml.rels
--rw-r--r--   0 andy      (1000) andy      (1000)      315 2022-02-10 15:34:27.000000 python-pptx-valutico-0.6.24.2/features/steps/test_files/extracted-pptx/ppt/slideLayouts/_rels/slideLayout6.xml.rels
--rw-r--r--   0 andy      (1000) andy      (1000)      315 2022-02-10 15:34:27.000000 python-pptx-valutico-0.6.24.2/features/steps/test_files/extracted-pptx/ppt/slideLayouts/_rels/slideLayout7.xml.rels
--rw-r--r--   0 andy      (1000) andy      (1000)      315 2022-02-10 15:34:27.000000 python-pptx-valutico-0.6.24.2/features/steps/test_files/extracted-pptx/ppt/slideLayouts/_rels/slideLayout8.xml.rels
--rw-r--r--   0 andy      (1000) andy      (1000)      315 2022-02-10 15:34:27.000000 python-pptx-valutico-0.6.24.2/features/steps/test_files/extracted-pptx/ppt/slideLayouts/_rels/slideLayout9.xml.rels
--rw-r--r--   0 andy      (1000) andy      (1000)     7176 2022-02-10 15:34:27.000000 python-pptx-valutico-0.6.24.2/features/steps/test_files/extracted-pptx/ppt/slideLayouts/slideLayout1.xml
--rw-r--r--   0 andy      (1000) andy      (1000)     4616 2022-02-10 15:34:27.000000 python-pptx-valutico-0.6.24.2/features/steps/test_files/extracted-pptx/ppt/slideLayouts/slideLayout10.xml
--rw-r--r--   0 andy      (1000) andy      (1000)     4954 2022-02-10 15:34:27.000000 python-pptx-valutico-0.6.24.2/features/steps/test_files/extracted-pptx/ppt/slideLayouts/slideLayout11.xml
--rw-r--r--   0 andy      (1000) andy      (1000)     4561 2022-02-10 15:34:27.000000 python-pptx-valutico-0.6.24.2/features/steps/test_files/extracted-pptx/ppt/slideLayouts/slideLayout2.xml
--rw-r--r--   0 andy      (1000) andy      (1000)     7312 2022-02-10 15:34:27.000000 python-pptx-valutico-0.6.24.2/features/steps/test_files/extracted-pptx/ppt/slideLayouts/slideLayout3.xml
--rw-r--r--   0 andy      (1000) andy      (1000)     7811 2022-02-10 15:34:27.000000 python-pptx-valutico-0.6.24.2/features/steps/test_files/extracted-pptx/ppt/slideLayouts/slideLayout4.xml
--rw-r--r--   0 andy      (1000) andy      (1000)    12024 2022-02-10 15:34:27.000000 python-pptx-valutico-0.6.24.2/features/steps/test_files/extracted-pptx/ppt/slideLayouts/slideLayout5.xml
--rw-r--r--   0 andy      (1000) andy      (1000)     3198 2022-02-10 15:34:27.000000 python-pptx-valutico-0.6.24.2/features/steps/test_files/extracted-pptx/ppt/slideLayouts/slideLayout6.xml
--rw-r--r--   0 andy      (1000) andy      (1000)     2607 2022-02-10 15:34:27.000000 python-pptx-valutico-0.6.24.2/features/steps/test_files/extracted-pptx/ppt/slideLayouts/slideLayout7.xml
--rw-r--r--   0 andy      (1000) andy      (1000)     7768 2022-02-10 15:34:27.000000 python-pptx-valutico-0.6.24.2/features/steps/test_files/extracted-pptx/ppt/slideLayouts/slideLayout8.xml
--rw-r--r--   0 andy      (1000) andy      (1000)     7325 2022-02-10 15:34:27.000000 python-pptx-valutico-0.6.24.2/features/steps/test_files/extracted-pptx/ppt/slideLayouts/slideLayout9.xml
-drwxr-xr-x   0 andy      (1000) andy      (1000)        0 2022-05-16 16:04:17.195551 python-pptx-valutico-0.6.24.2/features/steps/test_files/extracted-pptx/ppt/slideMasters/
-drwxr-xr-x   0 andy      (1000) andy      (1000)        0 2022-05-16 16:04:17.195551 python-pptx-valutico-0.6.24.2/features/steps/test_files/extracted-pptx/ppt/slideMasters/_rels/
--rw-r--r--   0 andy      (1000) andy      (1000)     2028 2022-02-10 15:34:27.000000 python-pptx-valutico-0.6.24.2/features/steps/test_files/extracted-pptx/ppt/slideMasters/_rels/slideMaster1.xml.rels
--rw-r--r--   0 andy      (1000) andy      (1000)    17336 2022-02-10 15:34:27.000000 python-pptx-valutico-0.6.24.2/features/steps/test_files/extracted-pptx/ppt/slideMasters/slideMaster1.xml
-drwxr-xr-x   0 andy      (1000) andy      (1000)        0 2022-05-16 16:04:17.195551 python-pptx-valutico-0.6.24.2/features/steps/test_files/extracted-pptx/ppt/slides/
-drwxr-xr-x   0 andy      (1000) andy      (1000)        0 2022-05-16 16:04:17.205551 python-pptx-valutico-0.6.24.2/features/steps/test_files/extracted-pptx/ppt/slides/_rels/
--rw-r--r--   0 andy      (1000) andy      (1000)      315 2022-02-10 15:34:27.000000 python-pptx-valutico-0.6.24.2/features/steps/test_files/extracted-pptx/ppt/slides/_rels/slide1.xml.rels
--rw-r--r--   0 andy      (1000) andy      (1000)     2128 2022-02-10 15:34:27.000000 python-pptx-valutico-0.6.24.2/features/steps/test_files/extracted-pptx/ppt/slides/slide1.xml
--rw-r--r--   0 andy      (1000) andy      (1000)      182 2022-02-10 15:34:27.000000 python-pptx-valutico-0.6.24.2/features/steps/test_files/extracted-pptx/ppt/tableStyles.xml
-drwxr-xr-x   0 andy      (1000) andy      (1000)        0 2022-05-16 16:04:17.205551 python-pptx-valutico-0.6.24.2/features/steps/test_files/extracted-pptx/ppt/theme/
--rw-r--r--   0 andy      (1000) andy      (1000)    10013 2022-02-10 15:34:27.000000 python-pptx-valutico-0.6.24.2/features/steps/test_files/extracted-pptx/ppt/theme/theme1.xml
--rw-r--r--   0 andy      (1000) andy      (1000)     1022 2022-02-10 15:34:27.000000 python-pptx-valutico-0.6.24.2/features/steps/test_files/extracted-pptx/ppt/viewProps.xml
--rw-r--r--   0 andy      (1000) andy      (1000)    25061 2022-02-10 15:28:55.000000 python-pptx-valutico-0.6.24.2/features/steps/test_files/font-color.pptx
--rwxr-xr-x   0 andy      (1000) andy      (1000)   470987 2022-02-10 15:28:55.000000 python-pptx-valutico-0.6.24.2/features/steps/test_files/just-two-mice.mp4
--rw-r--r--   0 andy      (1000) andy      (1000)   179346 2022-02-10 15:28:55.000000 python-pptx-valutico-0.6.24.2/features/steps/test_files/just-two-mice.png
--rw-r--r--   0 andy      (1000) andy      (1000)    23202 2022-02-10 15:28:55.000000 python-pptx-valutico-0.6.24.2/features/steps/test_files/lyt-shapes.pptx
--rw-r--r--   0 andy      (1000) andy      (1000)    15802 2022-02-10 15:28:55.000000 python-pptx-valutico-0.6.24.2/features/steps/test_files/minimal.pptx
--rw-r--r--   0 andy      (1000) andy      (1000)    64276 2022-02-10 15:28:55.000000 python-pptx-valutico-0.6.24.2/features/steps/test_files/monty-truth.png
--rw-r--r--   0 andy      (1000) andy      (1000)    25251 2022-02-10 15:28:55.000000 python-pptx-valutico-0.6.24.2/features/steps/test_files/mst-placeholders.pptx
--rw-r--r--   0 andy      (1000) andy      (1000)    25539 2022-02-10 15:28:55.000000 python-pptx-valutico-0.6.24.2/features/steps/test_files/mst-shapes.pptx
--rw-r--r--   0 andy      (1000) andy      (1000)    21166 2022-02-10 15:28:55.000000 python-pptx-valutico-0.6.24.2/features/steps/test_files/mst-slide-layouts.pptx
--rw-r--r--   0 andy      (1000) andy      (1000)    23566 2022-02-10 15:28:55.000000 python-pptx-valutico-0.6.24.2/features/steps/test_files/ph-inherit-props.pptx
--rw-r--r--   0 andy      (1000) andy      (1000)   172254 2022-02-10 15:28:55.000000 python-pptx-valutico-0.6.24.2/features/steps/test_files/ph-populated-placeholders.pptx
--rw-r--r--   0 andy      (1000) andy      (1000)    34405 2022-02-10 15:28:55.000000 python-pptx-valutico-0.6.24.2/features/steps/test_files/ph-unpopulated-placeholders.pptx
--rwxr-xr-x   0 andy      (1000) andy      (1000)    49704 2022-02-10 15:28:55.000000 python-pptx-valutico-0.6.24.2/features/steps/test_files/pic.emf
--rw-r--r--   0 andy      (1000) andy      (1000)    19655 2022-02-10 15:28:55.000000 python-pptx-valutico-0.6.24.2/features/steps/test_files/prs-add-slide.pptx
--rw-r--r--   0 andy      (1000) andy      (1000)    86792 2022-02-10 15:28:55.000000 python-pptx-valutico-0.6.24.2/features/steps/test_files/prs-notes.pptx
--rw-r--r--   0 andy      (1000) andy      (1000)    15806 2022-02-10 15:28:55.000000 python-pptx-valutico-0.6.24.2/features/steps/test_files/prs-properties.pptx
--rw-r--r--   0 andy      (1000) andy      (1000)    21528 2022-02-10 15:28:55.000000 python-pptx-valutico-0.6.24.2/features/steps/test_files/prs-slide-masters.pptx
--rw-r--r--   0 andy      (1000) andy      (1000)     3277 2022-02-10 15:28:55.000000 python-pptx-valutico-0.6.24.2/features/steps/test_files/python-icon.jpeg
--rw-r--r--   0 andy      (1000) andy      (1000)     6111 2022-02-10 15:28:55.000000 python-pptx-valutico-0.6.24.2/features/steps/test_files/python-powered.png
--rw-r--r--   0 andy      (1000) andy      (1000)    45210 2022-02-10 15:28:55.000000 python-pptx-valutico-0.6.24.2/features/steps/test_files/python.bmp
--rw-r--r--   0 andy      (1000) andy      (1000)    80038 2022-02-10 15:28:55.000000 python-pptx-valutico-0.6.24.2/features/steps/test_files/shp-access-chart.pptx
--rw-r--r--   0 andy      (1000) andy      (1000)   119022 2022-02-10 15:34:27.000000 python-pptx-valutico-0.6.24.2/features/steps/test_files/shp-access-ole-object.pptx
--rw-r--r--   0 andy      (1000) andy      (1000)    17626 2022-02-10 15:28:55.000000 python-pptx-valutico-0.6.24.2/features/steps/test_files/shp-autoshape-adjustments.pptx
--rw-r--r--   0 andy      (1000) andy      (1000)    22929 2022-02-10 15:28:55.000000 python-pptx-valutico-0.6.24.2/features/steps/test_files/shp-autoshape-props.pptx
--rw-r--r--   0 andy      (1000) andy      (1000)    81639 2022-02-10 15:28:55.000000 python-pptx-valutico-0.6.24.2/features/steps/test_files/shp-common-props.pptx
--rw-r--r--   0 andy      (1000) andy      (1000)    22899 2022-02-10 15:28:55.000000 python-pptx-valutico-0.6.24.2/features/steps/test_files/shp-connector-props.pptx
--rw-r--r--   0 andy      (1000) andy      (1000)    11680 2022-02-10 15:34:27.000000 python-pptx-valutico-0.6.24.2/features/steps/test_files/shp-embedded-docx.docx
--rw-r--r--   0 andy      (1000) andy      (1000)    29214 2022-02-10 15:34:27.000000 python-pptx-valutico-0.6.24.2/features/steps/test_files/shp-embedded-pptx.pptx
--rw-r--r--   0 andy      (1000) andy      (1000)     8250 2022-02-10 15:34:27.000000 python-pptx-valutico-0.6.24.2/features/steps/test_files/shp-embedded-xlsx.xlsx
--rw-r--r--   0 andy      (1000) andy      (1000)    16704 2022-02-10 15:28:55.000000 python-pptx-valutico-0.6.24.2/features/steps/test_files/shp-freeform.pptx
--rw-r--r--   0 andy      (1000) andy      (1000)    23786 2022-02-10 15:28:55.000000 python-pptx-valutico-0.6.24.2/features/steps/test_files/shp-groupshape.pptx
--rw-r--r--   0 andy      (1000) andy      (1000)   684874 2022-02-10 15:28:55.000000 python-pptx-valutico-0.6.24.2/features/steps/test_files/shp-movie-props.pptx
--rw-r--r--   0 andy      (1000) andy      (1000)    91730 2022-02-10 15:28:55.000000 python-pptx-valutico-0.6.24.2/features/steps/test_files/shp-picture.pptx
--rw-r--r--   0 andy      (1000) andy      (1000)    94116 2022-02-10 15:28:55.000000 python-pptx-valutico-0.6.24.2/features/steps/test_files/shp-pos-and-size.pptx
--rw-r--r--   0 andy      (1000) andy      (1000)   125205 2022-02-10 15:28:55.000000 python-pptx-valutico-0.6.24.2/features/steps/test_files/shp-shapes.pptx
--rw-r--r--   0 andy      (1000) andy      (1000)    17676 2022-02-10 15:28:55.000000 python-pptx-valutico-0.6.24.2/features/steps/test_files/sld-background.pptx
--rw-r--r--   0 andy      (1000) andy      (1000)    16703 2022-02-10 15:28:55.000000 python-pptx-valutico-0.6.24.2/features/steps/test_files/sld-blank.pptx
--rw-r--r--   0 andy      (1000) andy      (1000)    22964 2022-02-10 15:28:55.000000 python-pptx-valutico-0.6.24.2/features/steps/test_files/sld-notes.pptx
--rw-r--r--   0 andy      (1000) andy      (1000)    18894 2022-02-10 15:28:55.000000 python-pptx-valutico-0.6.24.2/features/steps/test_files/sld-slide.pptx
--rw-r--r--   0 andy      (1000) andy      (1000)    18478 2022-02-10 15:28:55.000000 python-pptx-valutico-0.6.24.2/features/steps/test_files/sld-slides.pptx
--rw-r--r--   0 andy      (1000) andy      (1000)    33273 2022-02-10 15:28:55.000000 python-pptx-valutico-0.6.24.2/features/steps/test_files/sonic.gif
--rw-r--r--   0 andy      (1000) andy      (1000)    28247 2022-02-10 15:28:55.000000 python-pptx-valutico-0.6.24.2/features/steps/test_files/tbl-cell.pptx
--rw-r--r--   0 andy      (1000) andy      (1000)    37859 2022-02-10 15:28:55.000000 python-pptx-valutico-0.6.24.2/features/steps/test_files/test.pptx
--rw-r--r--   0 andy      (1000) andy      (1000)    21337 2022-02-10 15:28:55.000000 python-pptx-valutico-0.6.24.2/features/steps/test_files/txt-fit-text.pptx
--rw-r--r--   0 andy      (1000) andy      (1000)    18874 2022-02-10 15:28:55.000000 python-pptx-valutico-0.6.24.2/features/steps/test_files/txt-font-props.pptx
--rw-r--r--   0 andy      (1000) andy      (1000)    25817 2022-02-10 15:28:55.000000 python-pptx-valutico-0.6.24.2/features/steps/test_files/txt-font-typeface.pptx
--rw-r--r--   0 andy      (1000) andy      (1000)    24620 2022-02-10 15:28:55.000000 python-pptx-valutico-0.6.24.2/features/steps/test_files/txt-paragraph-spacing.pptx
--rw-r--r--   0 andy      (1000) andy      (1000)    27659 2022-02-10 15:28:55.000000 python-pptx-valutico-0.6.24.2/features/steps/test_files/txt-text-frame.pptx
--rw-r--r--   0 andy      (1000) andy      (1000)    16051 2022-02-10 15:28:55.000000 python-pptx-valutico-0.6.24.2/features/steps/test_files/txt-text.pptx
--rw-r--r--   0 andy      (1000) andy      (1000)     8264 2022-02-10 15:28:55.000000 python-pptx-valutico-0.6.24.2/features/steps/text.py
--rw-r--r--   0 andy      (1000) andy      (1000)     4615 2022-02-10 15:28:55.000000 python-pptx-valutico-0.6.24.2/features/steps/text_frame.py
--rw-r--r--   0 andy      (1000) andy      (1000)     3549 2022-02-10 15:28:55.000000 python-pptx-valutico-0.6.24.2/features/tbl-cell.feature
--rw-r--r--   0 andy      (1000) andy      (1000)      343 2022-02-10 15:28:55.000000 python-pptx-valutico-0.6.24.2/features/tbl-column.feature
--rw-r--r--   0 andy      (1000) andy      (1000)     1565 2022-02-10 15:28:55.000000 python-pptx-valutico-0.6.24.2/features/tbl-table.feature
--rw-r--r--   0 andy      (1000) andy      (1000)      471 2022-02-10 15:28:55.000000 python-pptx-valutico-0.6.24.2/features/txt-fit-text.feature
--rw-r--r--   0 andy      (1000) andy      (1000)     1733 2022-02-10 15:28:55.000000 python-pptx-valutico-0.6.24.2/features/txt-font-color.feature
--rw-r--r--   0 andy      (1000) andy      (1000)     4945 2022-02-10 15:28:55.000000 python-pptx-valutico-0.6.24.2/features/txt-font-props.feature
--rw-r--r--   0 andy      (1000) andy      (1000)     3969 2022-02-10 15:28:55.000000 python-pptx-valutico-0.6.24.2/features/txt-paragraph.feature
--rw-r--r--   0 andy      (1000) andy      (1000)      734 2022-02-10 15:28:55.000000 python-pptx-valutico-0.6.24.2/features/txt-text.feature
--rw-r--r--   0 andy      (1000) andy      (1000)     2371 2022-02-10 15:28:55.000000 python-pptx-valutico-0.6.24.2/features/txt-textframe.feature
-drwxr-xr-x   0 andy      (1000) andy      (1000)        0 2022-05-16 16:04:17.215551 python-pptx-valutico-0.6.24.2/pptx/
--rw-r--r--   0 andy      (1000) andy      (1000)     1949 2022-05-16 16:02:24.000000 python-pptx-valutico-0.6.24.2/pptx/__init__.py
--rw-r--r--   0 andy      (1000) andy      (1000)     8672 2022-02-10 15:34:27.000000 python-pptx-valutico-0.6.24.2/pptx/action.py
--rw-r--r--   0 andy      (1000) andy      (1000)     1593 2022-02-10 15:28:55.000000 python-pptx-valutico-0.6.24.2/pptx/api.py
-drwxr-xr-x   0 andy      (1000) andy      (1000)        0 2022-05-16 16:04:17.215551 python-pptx-valutico-0.6.24.2/pptx/chart/
--rw-r--r--   0 andy      (1000) andy      (1000)        0 2022-02-10 15:28:55.000000 python-pptx-valutico-0.6.24.2/pptx/chart/__init__.py
--rw-r--r--   0 andy      (1000) andy      (1000)    17304 2022-02-10 15:34:27.000000 python-pptx-valutico-0.6.24.2/pptx/chart/axis.py
--rw-r--r--   0 andy      (1000) andy      (1000)     7250 2022-02-10 15:28:55.000000 python-pptx-valutico-0.6.24.2/pptx/chart/category.py
--rw-r--r--   0 andy      (1000) andy      (1000)     9999 2022-02-10 15:34:27.000000 python-pptx-valutico-0.6.24.2/pptx/chart/chart.py
--rw-r--r--   0 andy      (1000) andy      (1000)    29740 2022-02-10 15:34:27.000000 python-pptx-valutico-0.6.24.2/pptx/chart/data.py
--rw-r--r--   0 andy      (1000) andy      (1000)     9528 2022-02-10 15:28:55.000000 python-pptx-valutico-0.6.24.2/pptx/chart/datalabel.py
--rw-r--r--   0 andy      (1000) andy      (1000)     2566 2022-02-10 15:28:55.000000 python-pptx-valutico-0.6.24.2/pptx/chart/legend.py
--rw-r--r--   0 andy      (1000) andy      (1000)     2130 2022-02-10 15:34:27.000000 python-pptx-valutico-0.6.24.2/pptx/chart/marker.py
--rw-r--r--   0 andy      (1000) andy      (1000)    13213 2022-02-10 15:28:55.000000 python-pptx-valutico-0.6.24.2/pptx/chart/plot.py
--rw-r--r--   0 andy      (1000) andy      (1000)     2797 2022-02-10 15:28:55.000000 python-pptx-valutico-0.6.24.2/pptx/chart/point.py
--rw-r--r--   0 andy      (1000) andy      (1000)     7484 2022-02-10 15:28:55.000000 python-pptx-valutico-0.6.24.2/pptx/chart/series.py
--rw-r--r--   0 andy      (1000) andy      (1000)    10942 2022-02-10 15:34:27.000000 python-pptx-valutico-0.6.24.2/pptx/chart/xlsx.py
--rw-r--r--   0 andy      (1000) andy      (1000)    67673 2022-02-10 15:34:27.000000 python-pptx-valutico-0.6.24.2/pptx/chart/xmlwriter.py
-drwxr-xr-x   0 andy      (1000) andy      (1000)        0 2022-05-16 16:04:17.215551 python-pptx-valutico-0.6.24.2/pptx/compat/
--rw-r--r--   0 andy      (1000) andy      (1000)      703 2022-02-10 15:34:27.000000 python-pptx-valutico-0.6.24.2/pptx/compat/__init__.py
--rw-r--r--   0 andy      (1000) andy      (1000)     1302 2022-02-10 15:34:27.000000 python-pptx-valutico-0.6.24.2/pptx/compat/python2.py
--rw-r--r--   0 andy      (1000) andy      (1000)      920 2022-02-10 15:28:55.000000 python-pptx-valutico-0.6.24.2/pptx/compat/python3.py
-drwxr-xr-x   0 andy      (1000) andy      (1000)        0 2022-05-16 16:04:17.225551 python-pptx-valutico-0.6.24.2/pptx/dml/
--rw-r--r--   0 andy      (1000) andy      (1000)        0 2022-02-10 15:28:55.000000 python-pptx-valutico-0.6.24.2/pptx/dml/__init__.py
--rw-r--r--   0 andy      (1000) andy      (1000)     1373 2022-02-10 15:34:27.000000 python-pptx-valutico-0.6.24.2/pptx/dml/chtfmt.py
--rw-r--r--   0 andy      (1000) andy      (1000)     9124 2022-02-10 15:28:55.000000 python-pptx-valutico-0.6.24.2/pptx/dml/color.py
--rw-r--r--   0 andy      (1000) andy      (1000)     1592 2022-02-10 15:28:55.000000 python-pptx-valutico-0.6.24.2/pptx/dml/effect.py
--rw-r--r--   0 andy      (1000) andy      (1000)    13237 2022-02-10 15:34:27.000000 python-pptx-valutico-0.6.24.2/pptx/dml/fill.py
--rw-r--r--   0 andy      (1000) andy      (1000)     3108 2022-02-10 15:28:55.000000 python-pptx-valutico-0.6.24.2/pptx/dml/line.py
-drwxr-xr-x   0 andy      (1000) andy      (1000)        0 2022-05-16 16:04:17.225551 python-pptx-valutico-0.6.24.2/pptx/enum/
--rw-r--r--   0 andy      (1000) andy      (1000)        0 2022-02-10 15:28:55.000000 python-pptx-valutico-0.6.24.2/pptx/enum/__init__.py
--rw-r--r--   0 andy      (1000) andy      (1000)     1548 2022-02-10 15:28:55.000000 python-pptx-valutico-0.6.24.2/pptx/enum/action.py
--rw-r--r--   0 andy      (1000) andy      (1000)    10697 2022-02-10 15:28:55.000000 python-pptx-valutico-0.6.24.2/pptx/enum/base.py
--rw-r--r--   0 andy      (1000) andy      (1000)    13226 2022-02-10 15:34:27.000000 python-pptx-valutico-0.6.24.2/pptx/enum/chart.py
--rw-r--r--   0 andy      (1000) andy      (1000)    11940 2022-02-10 15:34:27.000000 python-pptx-valutico-0.6.24.2/pptx/enum/dml.py
--rw-r--r--   0 andy      (1000) andy      (1000)    22808 2022-02-10 15:28:55.000000 python-pptx-valutico-0.6.24.2/pptx/enum/lang.py
--rw-r--r--   0 andy      (1000) andy      (1000)    31458 2022-02-10 15:34:27.000000 python-pptx-valutico-0.6.24.2/pptx/enum/shapes.py
--rw-r--r--   0 andy      (1000) andy      (1000)     8215 2022-02-10 15:28:55.000000 python-pptx-valutico-0.6.24.2/pptx/enum/text.py
--rw-r--r--   0 andy      (1000) andy      (1000)      457 2022-02-10 15:28:55.000000 python-pptx-valutico-0.6.24.2/pptx/exc.py
--rw-r--r--   0 andy      (1000) andy      (1000)    10532 2022-02-10 15:28:55.000000 python-pptx-valutico-0.6.24.2/pptx/media.py
-drwxr-xr-x   0 andy      (1000) andy      (1000)        0 2022-05-16 16:04:17.225551 python-pptx-valutico-0.6.24.2/pptx/opc/
--rw-r--r--   0 andy      (1000) andy      (1000)        0 2022-02-10 15:28:55.000000 python-pptx-valutico-0.6.24.2/pptx/opc/__init__.py
--rw-r--r--   0 andy      (1000) andy      (1000)    19950 2022-02-10 15:34:27.000000 python-pptx-valutico-0.6.24.2/pptx/opc/constants.py
--rw-r--r--   0 andy      (1000) andy      (1000)     4514 2022-02-10 15:34:27.000000 python-pptx-valutico-0.6.24.2/pptx/opc/oxml.py
--rw-r--r--   0 andy      (1000) andy      (1000)    26976 2022-02-10 15:34:27.000000 python-pptx-valutico-0.6.24.2/pptx/opc/package.py
--rw-r--r--   0 andy      (1000) andy      (1000)     3880 2022-02-10 15:34:27.000000 python-pptx-valutico-0.6.24.2/pptx/opc/packuri.py
--rw-r--r--   0 andy      (1000) andy      (1000)     9969 2022-02-10 15:34:27.000000 python-pptx-valutico-0.6.24.2/pptx/opc/serialized.py
--rw-r--r--   0 andy      (1000) andy      (1000)      692 2022-02-10 15:34:27.000000 python-pptx-valutico-0.6.24.2/pptx/opc/shared.py
--rw-r--r--   0 andy      (1000) andy      (1000)     1012 2022-02-10 15:28:55.000000 python-pptx-valutico-0.6.24.2/pptx/opc/spec.py
-drwxr-xr-x   0 andy      (1000) andy      (1000)        0 2022-05-16 16:04:17.235551 python-pptx-valutico-0.6.24.2/pptx/oxml/
--rw-r--r--   0 andy      (1000) andy      (1000)    15446 2022-02-10 15:34:27.000000 python-pptx-valutico-0.6.24.2/pptx/oxml/__init__.py
--rw-r--r--   0 andy      (1000) andy      (1000)     1604 2022-02-10 15:28:55.000000 python-pptx-valutico-0.6.24.2/pptx/oxml/action.py
-drwxr-xr-x   0 andy      (1000) andy      (1000)        0 2022-05-16 16:04:17.245551 python-pptx-valutico-0.6.24.2/pptx/oxml/chart/
--rw-r--r--   0 andy      (1000) andy      (1000)        0 2022-02-10 15:28:55.000000 python-pptx-valutico-0.6.24.2/pptx/oxml/chart/__init__.py
--rw-r--r--   0 andy      (1000) andy      (1000)     9428 2022-02-10 15:34:27.000000 python-pptx-valutico-0.6.24.2/pptx/oxml/chart/axis.py
--rw-r--r--   0 andy      (1000) andy      (1000)     8190 2022-02-10 15:28:55.000000 python-pptx-valutico-0.6.24.2/pptx/oxml/chart/chart.py
--rw-r--r--   0 andy      (1000) andy      (1000)     7765 2022-02-10 15:28:55.000000 python-pptx-valutico-0.6.24.2/pptx/oxml/chart/datalabel.py
--rw-r--r--   0 andy      (1000) andy      (1000)     2129 2022-02-10 15:28:55.000000 python-pptx-valutico-0.6.24.2/pptx/oxml/chart/legend.py
--rw-r--r--   0 andy      (1000) andy      (1000)     1838 2022-02-10 15:28:55.000000 python-pptx-valutico-0.6.24.2/pptx/oxml/chart/marker.py
--rw-r--r--   0 andy      (1000) andy      (1000)     9224 2022-02-10 15:28:55.000000 python-pptx-valutico-0.6.24.2/pptx/oxml/chart/plot.py
--rw-r--r--   0 andy      (1000) andy      (1000)     7625 2022-02-10 15:28:55.000000 python-pptx-valutico-0.6.24.2/pptx/oxml/chart/series.py
--rw-r--r--   0 andy      (1000) andy      (1000)     6097 2022-02-10 15:28:55.000000 python-pptx-valutico-0.6.24.2/pptx/oxml/chart/shared.py
--rw-r--r--   0 andy      (1000) andy      (1000)     9820 2022-02-10 15:34:27.000000 python-pptx-valutico-0.6.24.2/pptx/oxml/coreprops.py
-drwxr-xr-x   0 andy      (1000) andy      (1000)        0 2022-05-16 16:04:17.245551 python-pptx-valutico-0.6.24.2/pptx/oxml/dml/
--rw-r--r--   0 andy      (1000) andy      (1000)        0 2022-02-10 15:28:55.000000 python-pptx-valutico-0.6.24.2/pptx/oxml/dml/__init__.py
--rw-r--r--   0 andy      (1000) andy      (1000)     2477 2022-02-10 15:28:55.000000 python-pptx-valutico-0.6.24.2/pptx/oxml/dml/color.py
--rw-r--r--   0 andy      (1000) andy      (1000)     5981 2022-02-10 15:28:55.000000 python-pptx-valutico-0.6.24.2/pptx/oxml/dml/fill.py
--rw-r--r--   0 andy      (1000) andy      (1000)      446 2022-02-10 15:28:55.000000 python-pptx-valutico-0.6.24.2/pptx/oxml/dml/line.py
--rw-r--r--   0 andy      (1000) andy      (1000)     6779 2022-05-16 15:59:17.000000 python-pptx-valutico-0.6.24.2/pptx/oxml/ns.py
--rw-r--r--   0 andy      (1000) andy      (1000)     2795 2022-02-10 15:28:55.000000 python-pptx-valutico-0.6.24.2/pptx/oxml/presentation.py
-drwxr-xr-x   0 andy      (1000) andy      (1000)        0 2022-05-16 16:04:17.245551 python-pptx-valutico-0.6.24.2/pptx/oxml/shapes/
--rw-r--r--   0 andy      (1000) andy      (1000)        0 2022-02-10 15:28:55.000000 python-pptx-valutico-0.6.24.2/pptx/oxml/shapes/__init__.py
--rw-r--r--   0 andy      (1000) andy      (1000)    13400 2022-02-10 15:28:55.000000 python-pptx-valutico-0.6.24.2/pptx/oxml/shapes/autoshape.py
--rw-r--r--   0 andy      (1000) andy      (1000)     3518 2022-02-10 15:28:55.000000 python-pptx-valutico-0.6.24.2/pptx/oxml/shapes/connector.py
--rw-r--r--   0 andy      (1000) andy      (1000)    12053 2022-02-10 15:34:27.000000 python-pptx-valutico-0.6.24.2/pptx/oxml/shapes/graphfrm.py
--rw-r--r--   0 andy      (1000) andy      (1000)     9214 2022-02-10 15:28:55.000000 python-pptx-valutico-0.6.24.2/pptx/oxml/shapes/groupshape.py
--rw-r--r--   0 andy      (1000) andy      (1000)     8096 2022-02-10 15:34:27.000000 python-pptx-valutico-0.6.24.2/pptx/oxml/shapes/picture.py
--rw-r--r--   0 andy      (1000) andy      (1000)    12696 2022-02-10 15:28:55.000000 python-pptx-valutico-0.6.24.2/pptx/oxml/shapes/shared.py
--rw-r--r--   0 andy      (1000) andy      (1000)    19929 2022-02-10 15:34:27.000000 python-pptx-valutico-0.6.24.2/pptx/oxml/simpletypes.py
--rw-r--r--   0 andy      (1000) andy      (1000)    10213 2022-02-10 15:28:55.000000 python-pptx-valutico-0.6.24.2/pptx/oxml/slide.py
--rw-r--r--   0 andy      (1000) andy      (1000)    18277 2022-02-10 15:28:55.000000 python-pptx-valutico-0.6.24.2/pptx/oxml/table.py
--rw-r--r--   0 andy      (1000) andy      (1000)    16439 2022-02-10 15:28:55.000000 python-pptx-valutico-0.6.24.2/pptx/oxml/text.py
--rw-r--r--   0 andy      (1000) andy      (1000)      754 2022-02-10 15:28:55.000000 python-pptx-valutico-0.6.24.2/pptx/oxml/theme.py
--rw-r--r--   0 andy      (1000) andy      (1000)    25027 2022-02-10 15:28:55.000000 python-pptx-valutico-0.6.24.2/pptx/oxml/xmlchemy.py
--rw-r--r--   0 andy      (1000) andy      (1000)     7626 2022-02-10 15:34:27.000000 python-pptx-valutico-0.6.24.2/pptx/package.py
-drwxr-xr-x   0 andy      (1000) andy      (1000)        0 2022-05-16 16:04:17.255551 python-pptx-valutico-0.6.24.2/pptx/parts/
--rw-r--r--   0 andy      (1000) andy      (1000)        0 2022-02-10 15:28:55.000000 python-pptx-valutico-0.6.24.2/pptx/parts/__init__.py
--rw-r--r--   0 andy      (1000) andy      (1000)     3000 2022-02-10 15:34:27.000000 python-pptx-valutico-0.6.24.2/pptx/parts/chart.py
--rw-r--r--   0 andy      (1000) andy      (1000)     4052 2022-02-10 15:34:27.000000 python-pptx-valutico-0.6.24.2/pptx/parts/coreprops.py
--rw-r--r--   0 andy      (1000) andy      (1000)     2815 2022-02-10 15:34:27.000000 python-pptx-valutico-0.6.24.2/pptx/parts/embeddedpackage.py
--rw-r--r--   0 andy      (1000) andy      (1000)     9038 2022-02-10 15:34:27.000000 python-pptx-valutico-0.6.24.2/pptx/parts/image.py
--rw-r--r--   0 andy      (1000) andy      (1000)      901 2022-02-10 15:34:27.000000 python-pptx-valutico-0.6.24.2/pptx/parts/media.py
--rw-r--r--   0 andy      (1000) andy      (1000)     4477 2022-02-10 15:34:27.000000 python-pptx-valutico-0.6.24.2/pptx/parts/presentation.py
--rw-r--r--   0 andy      (1000) andy      (1000)    10432 2022-02-10 15:34:27.000000 python-pptx-valutico-0.6.24.2/pptx/parts/slide.py
--rw-r--r--   0 andy      (1000) andy      (1000)     4591 2022-03-25 20:05:51.000000 python-pptx-valutico-0.6.24.2/pptx/presentation.py
-drwxr-xr-x   0 andy      (1000) andy      (1000)        0 2022-05-16 16:04:17.255551 python-pptx-valutico-0.6.24.2/pptx/shapes/
--rw-r--r--   0 andy      (1000) andy      (1000)      589 2022-02-10 15:28:55.000000 python-pptx-valutico-0.6.24.2/pptx/shapes/__init__.py
--rw-r--r--   0 andy      (1000) andy      (1000)    13710 2022-02-10 15:28:55.000000 python-pptx-valutico-0.6.24.2/pptx/shapes/autoshape.py
--rw-r--r--   0 andy      (1000) andy      (1000)     7574 2022-02-10 15:28:55.000000 python-pptx-valutico-0.6.24.2/pptx/shapes/base.py
--rw-r--r--   0 andy      (1000) andy      (1000)    10063 2022-02-10 15:34:27.000000 python-pptx-valutico-0.6.24.2/pptx/shapes/connector.py
--rw-r--r--   0 andy      (1000) andy      (1000)    10933 2022-02-10 15:28:55.000000 python-pptx-valutico-0.6.24.2/pptx/shapes/freeform.py
--rw-r--r--   0 andy      (1000) andy      (1000)     5005 2022-02-10 15:34:27.000000 python-pptx-valutico-0.6.24.2/pptx/shapes/graphfrm.py
--rw-r--r--   0 andy      (1000) andy      (1000)     1859 2022-02-10 15:28:55.000000 python-pptx-valutico-0.6.24.2/pptx/shapes/group.py
--rw-r--r--   0 andy      (1000) andy      (1000)     6637 2022-02-10 15:28:55.000000 python-pptx-valutico-0.6.24.2/pptx/shapes/picture.py
--rw-r--r--   0 andy      (1000) andy      (1000)    14539 2022-02-10 15:34:27.000000 python-pptx-valutico-0.6.24.2/pptx/shapes/placeholder.py
--rw-r--r--   0 andy      (1000) andy      (1000)    41368 2022-02-10 15:34:27.000000 python-pptx-valutico-0.6.24.2/pptx/shapes/shapetree.py
--rw-r--r--   0 andy      (1000) andy      (1000)     2593 2022-02-10 15:34:27.000000 python-pptx-valutico-0.6.24.2/pptx/shared.py
--rw-r--r--   0 andy      (1000) andy      (1000)    17890 2022-02-10 15:34:27.000000 python-pptx-valutico-0.6.24.2/pptx/slide.py
--rw-r--r--   0 andy      (1000) andy      (1000)    23582 2022-02-10 15:34:27.000000 python-pptx-valutico-0.6.24.2/pptx/spec.py
--rw-r--r--   0 andy      (1000) andy      (1000)    17813 2022-02-10 15:44:13.000000 python-pptx-valutico-0.6.24.2/pptx/table.py
-drwxr-xr-x   0 andy      (1000) andy      (1000)        0 2022-05-16 16:04:17.275551 python-pptx-valutico-0.6.24.2/pptx/templates/
--rw-r--r--   0 andy      (1000) andy      (1000)    34030 2022-02-10 15:28:55.000000 python-pptx-valutico-0.6.24.2/pptx/templates/default.pptx
--rw-r--r--   0 andy      (1000) andy      (1000)   127228 2022-02-10 15:34:27.000000 python-pptx-valutico-0.6.24.2/pptx/templates/docx-icon.emf
--rw-r--r--   0 andy      (1000) andy      (1000)     5396 2022-02-10 15:34:27.000000 python-pptx-valutico-0.6.24.2/pptx/templates/generic-icon.emf
--rw-r--r--   0 andy      (1000) andy      (1000)      722 2022-02-10 15:28:55.000000 python-pptx-valutico-0.6.24.2/pptx/templates/notes.xml
--rw-r--r--   0 andy      (1000) andy      (1000)    11135 2022-02-10 15:28:55.000000 python-pptx-valutico-0.6.24.2/pptx/templates/notesMaster.xml
--rw-r--r--   0 andy      (1000) andy      (1000)     5492 2022-02-10 15:34:27.000000 python-pptx-valutico-0.6.24.2/pptx/templates/pptx-icon.emf
--rw-r--r--   0 andy      (1000) andy      (1000)    10964 2022-02-10 15:28:55.000000 python-pptx-valutico-0.6.24.2/pptx/templates/theme.xml
--rw-r--r--   0 andy      (1000) andy      (1000)   130380 2022-02-10 15:34:27.000000 python-pptx-valutico-0.6.24.2/pptx/templates/xlsx-icon.emf
-drwxr-xr-x   0 andy      (1000) andy      (1000)        0 2022-05-16 16:04:17.275551 python-pptx-valutico-0.6.24.2/pptx/text/
--rw-r--r--   0 andy      (1000) andy      (1000)        0 2022-02-10 15:28:55.000000 python-pptx-valutico-0.6.24.2/pptx/text/__init__.py
--rw-r--r--   0 andy      (1000) andy      (1000)    12900 2022-02-10 15:34:27.000000 python-pptx-valutico-0.6.24.2/pptx/text/fonts.py
--rw-r--r--   0 andy      (1000) andy      (1000)     9959 2022-02-10 15:34:27.000000 python-pptx-valutico-0.6.24.2/pptx/text/layout.py
--rw-r--r--   0 andy      (1000) andy      (1000)    25179 2022-02-10 15:34:27.000000 python-pptx-valutico-0.6.24.2/pptx/text/text.py
--rw-r--r--   0 andy      (1000) andy      (1000)     7826 2022-02-10 15:34:27.000000 python-pptx-valutico-0.6.24.2/pptx/util.py
-drwxr-xr-x   0 andy      (1000) andy      (1000)        0 2022-05-16 16:04:17.285551 python-pptx-valutico-0.6.24.2/python_pptx_valutico.egg-info/
--rw-r--r--   0 andy      (1000) andy      (1000)    18286 2022-05-16 16:04:16.000000 python-pptx-valutico-0.6.24.2/python_pptx_valutico.egg-info/PKG-INFO
--rw-r--r--   0 andy      (1000) andy      (1000)    18710 2022-05-16 16:04:16.000000 python-pptx-valutico-0.6.24.2/python_pptx_valutico.egg-info/SOURCES.txt
--rw-r--r--   0 andy      (1000) andy      (1000)        1 2022-05-16 16:04:16.000000 python-pptx-valutico-0.6.24.2/python_pptx_valutico.egg-info/dependency_links.txt
--rw-r--r--   0 andy      (1000) andy      (1000)        1 2022-02-10 16:06:22.000000 python-pptx-valutico-0.6.24.2/python_pptx_valutico.egg-info/not-zip-safe
--rw-r--r--   0 andy      (1000) andy      (1000)       44 2022-05-16 16:04:16.000000 python-pptx-valutico-0.6.24.2/python_pptx_valutico.egg-info/requires.txt
--rw-r--r--   0 andy      (1000) andy      (1000)        5 2022-05-16 16:04:16.000000 python-pptx-valutico-0.6.24.2/python_pptx_valutico.egg-info/top_level.txt
--rw-r--r--   0 andy      (1000) andy      (1000)       38 2022-05-16 16:04:17.475551 python-pptx-valutico-0.6.24.2/setup.cfg
--rwxr-xr-x   0 andy      (1000) andy      (1000)     2690 2022-02-10 16:27:53.000000 python-pptx-valutico-0.6.24.2/setup.py
-drwxr-xr-x   0 andy      (1000) andy      (1000)        0 2022-05-16 16:04:17.295551 python-pptx-valutico-0.6.24.2/tests/
--rw-r--r--   0 andy      (1000) andy      (1000)        0 2022-02-10 15:28:55.000000 python-pptx-valutico-0.6.24.2/tests/__init__.py
-drwxr-xr-x   0 andy      (1000) andy      (1000)        0 2022-05-16 16:04:17.295551 python-pptx-valutico-0.6.24.2/tests/chart/
--rw-r--r--   0 andy      (1000) andy      (1000)        0 2022-02-10 15:28:55.000000 python-pptx-valutico-0.6.24.2/tests/chart/__init__.py
--rw-r--r--   0 andy      (1000) andy      (1000)    48371 2022-02-10 15:34:27.000000 python-pptx-valutico-0.6.24.2/tests/chart/test_axis.py
--rw-r--r--   0 andy      (1000) andy      (1000)     9346 2022-02-10 15:28:55.000000 python-pptx-valutico-0.6.24.2/tests/chart/test_category.py
--rw-r--r--   0 andy      (1000) andy      (1000)    21201 2022-02-10 15:34:27.000000 python-pptx-valutico-0.6.24.2/tests/chart/test_chart.py
--rw-r--r--   0 andy      (1000) andy      (1000)    34116 2022-02-10 15:28:55.000000 python-pptx-valutico-0.6.24.2/tests/chart/test_data.py
--rw-r--r--   0 andy      (1000) andy      (1000)    26214 2022-02-10 15:28:55.000000 python-pptx-valutico-0.6.24.2/tests/chart/test_datalabel.py
--rw-r--r--   0 andy      (1000) andy      (1000)     6797 2022-02-10 15:28:55.000000 python-pptx-valutico-0.6.24.2/tests/chart/test_legend.py
--rw-r--r--   0 andy      (1000) andy      (1000)     4827 2022-02-10 15:28:55.000000 python-pptx-valutico-0.6.24.2/tests/chart/test_marker.py
--rw-r--r--   0 andy      (1000) andy      (1000)    18769 2022-02-10 15:28:55.000000 python-pptx-valutico-0.6.24.2/tests/chart/test_plot.py
--rw-r--r--   0 andy      (1000) andy      (1000)     7659 2022-02-10 15:28:55.000000 python-pptx-valutico-0.6.24.2/tests/chart/test_point.py
--rw-r--r--   0 andy      (1000) andy      (1000)    19055 2022-02-10 15:28:55.000000 python-pptx-valutico-0.6.24.2/tests/chart/test_series.py
--rw-r--r--   0 andy      (1000) andy      (1000)    15936 2022-02-10 15:34:27.000000 python-pptx-valutico-0.6.24.2/tests/chart/test_xlsx.py
--rw-r--r--   0 andy      (1000) andy      (1000)    28442 2022-02-10 15:34:27.000000 python-pptx-valutico-0.6.24.2/tests/chart/test_xmlwriter.py
-drwxr-xr-x   0 andy      (1000) andy      (1000)        0 2022-05-16 16:04:17.295551 python-pptx-valutico-0.6.24.2/tests/dml/
--rw-r--r--   0 andy      (1000) andy      (1000)        0 2022-02-10 15:28:55.000000 python-pptx-valutico-0.6.24.2/tests/dml/__init__.py
--rw-r--r--   0 andy      (1000) andy      (1000)     3235 2022-02-10 15:28:55.000000 python-pptx-valutico-0.6.24.2/tests/dml/test_chtfmt.py
--rw-r--r--   0 andy      (1000) andy      (1000)    11638 2022-02-10 15:28:55.000000 python-pptx-valutico-0.6.24.2/tests/dml/test_color.py
--rw-r--r--   0 andy      (1000) andy      (1000)     1923 2022-02-10 15:28:55.000000 python-pptx-valutico-0.6.24.2/tests/dml/test_effect.py
--rw-r--r--   0 andy      (1000) andy      (1000)    25636 2022-02-10 15:34:27.000000 python-pptx-valutico-0.6.24.2/tests/dml/test_fill.py
--rw-r--r--   0 andy      (1000) andy      (1000)     5963 2022-02-10 15:28:55.000000 python-pptx-valutico-0.6.24.2/tests/dml/test_line.py
-drwxr-xr-x   0 andy      (1000) andy      (1000)        0 2022-05-16 16:04:17.295551 python-pptx-valutico-0.6.24.2/tests/opc/
--rw-r--r--   0 andy      (1000) andy      (1000)        0 2022-02-10 15:28:55.000000 python-pptx-valutico-0.6.24.2/tests/opc/__init__.py
--rw-r--r--   0 andy      (1000) andy      (1000)     6460 2022-02-10 15:34:27.000000 python-pptx-valutico-0.6.24.2/tests/opc/test_oxml.py
--rw-r--r--   0 andy      (1000) andy      (1000)    38342 2022-02-10 15:34:27.000000 python-pptx-valutico-0.6.24.2/tests/opc/test_package.py
--rw-r--r--   0 andy      (1000) andy      (1000)     2976 2022-02-10 15:34:27.000000 python-pptx-valutico-0.6.24.2/tests/opc/test_packuri.py
--rw-r--r--   0 andy      (1000) andy      (1000)    14807 2022-02-10 15:34:27.000000 python-pptx-valutico-0.6.24.2/tests/opc/test_serialized.py
-drwxr-xr-x   0 andy      (1000) andy      (1000)        0 2022-05-16 16:04:17.295551 python-pptx-valutico-0.6.24.2/tests/opc/unitdata/
--rw-r--r--   0 andy      (1000) andy      (1000)        0 2022-02-10 15:28:55.000000 python-pptx-valutico-0.6.24.2/tests/opc/unitdata/__init__.py
--rw-r--r--   0 andy      (1000) andy      (1000)     7480 2022-02-10 15:34:27.000000 python-pptx-valutico-0.6.24.2/tests/opc/unitdata/rels.py
-drwxr-xr-x   0 andy      (1000) andy      (1000)        0 2022-05-16 16:04:17.305551 python-pptx-valutico-0.6.24.2/tests/oxml/
--rw-r--r--   0 andy      (1000) andy      (1000)        0 2022-02-10 15:28:55.000000 python-pptx-valutico-0.6.24.2/tests/oxml/__init__.py
-drwxr-xr-x   0 andy      (1000) andy      (1000)        0 2022-05-16 16:04:17.305551 python-pptx-valutico-0.6.24.2/tests/oxml/shapes/
--rw-r--r--   0 andy      (1000) andy      (1000)        0 2022-02-10 15:28:55.000000 python-pptx-valutico-0.6.24.2/tests/oxml/shapes/__init__.py
--rw-r--r--   0 andy      (1000) andy      (1000)    10011 2022-02-10 15:28:55.000000 python-pptx-valutico-0.6.24.2/tests/oxml/shapes/test_autoshape.py
--rw-r--r--   0 andy      (1000) andy      (1000)     3383 2022-02-10 15:34:27.000000 python-pptx-valutico-0.6.24.2/tests/oxml/shapes/test_graphfrm.py
--rw-r--r--   0 andy      (1000) andy      (1000)    10820 2022-02-10 15:34:27.000000 python-pptx-valutico-0.6.24.2/tests/oxml/shapes/test_groupshape.py
--rw-r--r--   0 andy      (1000) andy      (1000)     3591 2022-02-10 15:34:27.000000 python-pptx-valutico-0.6.24.2/tests/oxml/shapes/test_picture.py
--rw-r--r--   0 andy      (1000) andy      (1000)     3204 2022-02-10 15:28:55.000000 python-pptx-valutico-0.6.24.2/tests/oxml/test___init__.py
--rw-r--r--   0 andy      (1000) andy      (1000)     5059 2022-02-10 15:28:55.000000 python-pptx-valutico-0.6.24.2/tests/oxml/test_dml.py
--rw-r--r--   0 andy      (1000) andy      (1000)     2669 2022-02-10 15:28:55.000000 python-pptx-valutico-0.6.24.2/tests/oxml/test_ns.py
--rw-r--r--   0 andy      (1000) andy      (1000)     1436 2022-02-10 15:28:55.000000 python-pptx-valutico-0.6.24.2/tests/oxml/test_presentation.py
--rw-r--r--   0 andy      (1000) andy      (1000)     8990 2022-02-10 15:34:27.000000 python-pptx-valutico-0.6.24.2/tests/oxml/test_simpletypes.py
--rw-r--r--   0 andy      (1000) andy      (1000)      719 2022-02-10 15:34:27.000000 python-pptx-valutico-0.6.24.2/tests/oxml/test_slide.py
--rw-r--r--   0 andy      (1000) andy      (1000)    10125 2022-02-10 15:28:55.000000 python-pptx-valutico-0.6.24.2/tests/oxml/test_table.py
--rw-r--r--   0 andy      (1000) andy      (1000)      693 2022-02-10 15:28:55.000000 python-pptx-valutico-0.6.24.2/tests/oxml/test_theme.py
--rw-r--r--   0 andy      (1000) andy      (1000)    20871 2022-02-10 15:28:55.000000 python-pptx-valutico-0.6.24.2/tests/oxml/test_xmlchemy.py
-drwxr-xr-x   0 andy      (1000) andy      (1000)        0 2022-05-16 16:04:17.305551 python-pptx-valutico-0.6.24.2/tests/oxml/unitdata/
--rw-r--r--   0 andy      (1000) andy      (1000)        0 2022-02-10 15:28:55.000000 python-pptx-valutico-0.6.24.2/tests/oxml/unitdata/__init__.py
--rw-r--r--   0 andy      (1000) andy      (1000)     1946 2022-02-10 15:28:55.000000 python-pptx-valutico-0.6.24.2/tests/oxml/unitdata/dml.py
--rw-r--r--   0 andy      (1000) andy      (1000)     4060 2022-02-10 15:34:27.000000 python-pptx-valutico-0.6.24.2/tests/oxml/unitdata/shape.py
--rw-r--r--   0 andy      (1000) andy      (1000)     1792 2022-02-10 15:34:27.000000 python-pptx-valutico-0.6.24.2/tests/oxml/unitdata/text.py
-drwxr-xr-x   0 andy      (1000) andy      (1000)        0 2022-05-16 16:04:17.305551 python-pptx-valutico-0.6.24.2/tests/parts/
--rw-r--r--   0 andy      (1000) andy      (1000)        0 2022-02-10 15:28:55.000000 python-pptx-valutico-0.6.24.2/tests/parts/__init__.py
--rw-r--r--   0 andy      (1000) andy      (1000)     5973 2022-02-10 15:34:27.000000 python-pptx-valutico-0.6.24.2/tests/parts/test_chart.py
--rw-r--r--   0 andy      (1000) andy      (1000)     9096 2022-02-10 15:34:27.000000 python-pptx-valutico-0.6.24.2/tests/parts/test_coreprops.py
--rw-r--r--   0 andy      (1000) andy      (1000)     3007 2022-02-10 15:34:27.000000 python-pptx-valutico-0.6.24.2/tests/parts/test_embeddedpackage.py
--rw-r--r--   0 andy      (1000) andy      (1000)     7799 2022-02-10 15:34:27.000000 python-pptx-valutico-0.6.24.2/tests/parts/test_image.py
--rw-r--r--   0 andy      (1000) andy      (1000)     1185 2022-02-10 15:34:27.000000 python-pptx-valutico-0.6.24.2/tests/parts/test_media.py
--rw-r--r--   0 andy      (1000) andy      (1000)     9156 2022-02-10 15:34:27.000000 python-pptx-valutico-0.6.24.2/tests/parts/test_presentation.py
--rw-r--r--   0 andy      (1000) andy      (1000)    22548 2022-02-10 15:34:27.000000 python-pptx-valutico-0.6.24.2/tests/parts/test_slide.py
-drwxr-xr-x   0 andy      (1000) andy      (1000)        0 2022-05-16 16:04:17.315551 python-pptx-valutico-0.6.24.2/tests/shapes/
--rw-r--r--   0 andy      (1000) andy      (1000)        0 2022-02-10 15:28:55.000000 python-pptx-valutico-0.6.24.2/tests/shapes/__init__.py
--rw-r--r--   0 andy      (1000) andy      (1000)    18645 2022-02-10 15:28:55.000000 python-pptx-valutico-0.6.24.2/tests/shapes/test_autoshape.py
--rw-r--r--   0 andy      (1000) andy      (1000)    19691 2022-02-10 15:34:27.000000 python-pptx-valutico-0.6.24.2/tests/shapes/test_base.py
--rw-r--r--   0 andy      (1000) andy      (1000)    16235 2022-02-10 15:34:27.000000 python-pptx-valutico-0.6.24.2/tests/shapes/test_connector.py
--rw-r--r--   0 andy      (1000) andy      (1000)    20589 2022-02-10 15:34:27.000000 python-pptx-valutico-0.6.24.2/tests/shapes/test_freeform.py
--rw-r--r--   0 andy      (1000) andy      (1000)     6651 2022-02-10 15:34:27.000000 python-pptx-valutico-0.6.24.2/tests/shapes/test_graphfrm.py
--rw-r--r--   0 andy      (1000) andy      (1000)     2360 2022-02-10 15:28:55.000000 python-pptx-valutico-0.6.24.2/tests/shapes/test_group.py
--rw-r--r--   0 andy      (1000) andy      (1000)    10621 2022-02-10 15:28:55.000000 python-pptx-valutico-0.6.24.2/tests/shapes/test_picture.py
--rw-r--r--   0 andy      (1000) andy      (1000)    22431 2022-02-10 15:34:27.000000 python-pptx-valutico-0.6.24.2/tests/shapes/test_placeholder.py
--rw-r--r--   0 andy      (1000) andy      (1000)    87112 2022-02-10 15:34:27.000000 python-pptx-valutico-0.6.24.2/tests/shapes/test_shapetree.py
--rw-r--r--   0 andy      (1000) andy      (1000)    13970 2022-02-10 15:34:27.000000 python-pptx-valutico-0.6.24.2/tests/test_action.py
--rw-r--r--   0 andy      (1000) andy      (1000)     1527 2022-02-10 15:28:55.000000 python-pptx-valutico-0.6.24.2/tests/test_api.py
--rw-r--r--   0 andy      (1000) andy      (1000)     3739 2022-02-10 15:34:27.000000 python-pptx-valutico-0.6.24.2/tests/test_enum.py
-drwxr-xr-x   0 andy      (1000) andy      (1000)        0 2022-05-16 16:04:17.345551 python-pptx-valutico-0.6.24.2/tests/test_files/
--rw-r--r--   0 andy      (1000) andy      (1000)   867288 2022-02-10 15:28:55.000000 python-pptx-valutico-0.6.24.2/tests/test_files/calibriz.ttf
--rwxr-xr-x   0 andy      (1000) andy      (1000)    21818 2022-02-10 15:28:55.000000 python-pptx-valutico-0.6.24.2/tests/test_files/cdw-logo.eps
--rw-r--r--   0 andy      (1000) andy      (1000)       42 2022-02-10 15:28:55.000000 python-pptx-valutico-0.6.24.2/tests/test_files/dummy.mp4
-drwxr-xr-x   0 andy      (1000) andy      (1000)        0 2022-05-16 16:04:17.345551 python-pptx-valutico-0.6.24.2/tests/test_files/expanded_pptx/
--rw-r--r--   0 andy      (1000) andy      (1000)     3359 2022-02-10 15:28:55.000000 python-pptx-valutico-0.6.24.2/tests/test_files/expanded_pptx/[Content_Types].xml
-drwxr-xr-x   0 andy      (1000) andy      (1000)        0 2022-05-16 16:04:17.345551 python-pptx-valutico-0.6.24.2/tests/test_files/expanded_pptx/_rels/
--rw-r--r--   0 andy      (1000) andy      (1000)      758 2022-02-10 15:28:55.000000 python-pptx-valutico-0.6.24.2/tests/test_files/expanded_pptx/_rels/.rels
-drwxr-xr-x   0 andy      (1000) andy      (1000)        0 2022-05-16 16:04:17.355551 python-pptx-valutico-0.6.24.2/tests/test_files/expanded_pptx/docProps/
--rw-r--r--   0 andy      (1000) andy      (1000)     1354 2022-02-10 15:28:55.000000 python-pptx-valutico-0.6.24.2/tests/test_files/expanded_pptx/docProps/app.xml
--rw-r--r--   0 andy      (1000) andy      (1000)      750 2022-02-10 15:28:55.000000 python-pptx-valutico-0.6.24.2/tests/test_files/expanded_pptx/docProps/core.xml
--rw-r--r--   0 andy      (1000) andy      (1000)     8147 2022-02-10 15:28:55.000000 python-pptx-valutico-0.6.24.2/tests/test_files/expanded_pptx/docProps/thumbnail.jpeg
-drwxr-xr-x   0 andy      (1000) andy      (1000)        0 2022-05-16 16:04:17.365552 python-pptx-valutico-0.6.24.2/tests/test_files/expanded_pptx/ppt/
-drwxr-xr-x   0 andy      (1000) andy      (1000)        0 2022-05-16 16:04:17.365552 python-pptx-valutico-0.6.24.2/tests/test_files/expanded_pptx/ppt/_rels/
--rw-r--r--   0 andy      (1000) andy      (1000)     1170 2022-02-10 15:28:55.000000 python-pptx-valutico-0.6.24.2/tests/test_files/expanded_pptx/ppt/_rels/presentation.xml.rels
--rw-r--r--   0 andy      (1000) andy      (1000)      327 2022-02-10 15:28:55.000000 python-pptx-valutico-0.6.24.2/tests/test_files/expanded_pptx/ppt/presProps.xml
--rw-r--r--   0 andy      (1000) andy      (1000)     4157 2022-02-10 15:28:55.000000 python-pptx-valutico-0.6.24.2/tests/test_files/expanded_pptx/ppt/presentation.xml
-drwxr-xr-x   0 andy      (1000) andy      (1000)        0 2022-05-16 16:04:17.365552 python-pptx-valutico-0.6.24.2/tests/test_files/expanded_pptx/ppt/printerSettings/
--rw-r--r--   0 andy      (1000) andy      (1000)     9395 2022-02-10 15:28:55.000000 python-pptx-valutico-0.6.24.2/tests/test_files/expanded_pptx/ppt/printerSettings/printerSettings1.bin
-drwxr-xr-x   0 andy      (1000) andy      (1000)        0 2022-05-16 16:04:17.385552 python-pptx-valutico-0.6.24.2/tests/test_files/expanded_pptx/ppt/slideLayouts/
-drwxr-xr-x   0 andy      (1000) andy      (1000)        0 2022-05-16 16:04:17.395552 python-pptx-valutico-0.6.24.2/tests/test_files/expanded_pptx/ppt/slideLayouts/_rels/
--rw-r--r--   0 andy      (1000) andy      (1000)      319 2022-02-10 15:28:55.000000 python-pptx-valutico-0.6.24.2/tests/test_files/expanded_pptx/ppt/slideLayouts/_rels/slideLayout1.xml.rels
--rw-r--r--   0 andy      (1000) andy      (1000)      319 2022-02-10 15:28:55.000000 python-pptx-valutico-0.6.24.2/tests/test_files/expanded_pptx/ppt/slideLayouts/_rels/slideLayout10.xml.rels
--rw-r--r--   0 andy      (1000) andy      (1000)      319 2022-02-10 15:28:55.000000 python-pptx-valutico-0.6.24.2/tests/test_files/expanded_pptx/ppt/slideLayouts/_rels/slideLayout11.xml.rels
--rw-r--r--   0 andy      (1000) andy      (1000)      319 2022-02-10 15:28:55.000000 python-pptx-valutico-0.6.24.2/tests/test_files/expanded_pptx/ppt/slideLayouts/_rels/slideLayout2.xml.rels
--rw-r--r--   0 andy      (1000) andy      (1000)      319 2022-02-10 15:28:55.000000 python-pptx-valutico-0.6.24.2/tests/test_files/expanded_pptx/ppt/slideLayouts/_rels/slideLayout3.xml.rels
--rw-r--r--   0 andy      (1000) andy      (1000)      319 2022-02-10 15:28:55.000000 python-pptx-valutico-0.6.24.2/tests/test_files/expanded_pptx/ppt/slideLayouts/_rels/slideLayout4.xml.rels
--rw-r--r--   0 andy      (1000) andy      (1000)      319 2022-02-10 15:28:55.000000 python-pptx-valutico-0.6.24.2/tests/test_files/expanded_pptx/ppt/slideLayouts/_rels/slideLayout5.xml.rels
--rw-r--r--   0 andy      (1000) andy      (1000)      319 2022-02-10 15:28:55.000000 python-pptx-valutico-0.6.24.2/tests/test_files/expanded_pptx/ppt/slideLayouts/_rels/slideLayout6.xml.rels
--rw-r--r--   0 andy      (1000) andy      (1000)      319 2022-02-10 15:28:55.000000 python-pptx-valutico-0.6.24.2/tests/test_files/expanded_pptx/ppt/slideLayouts/_rels/slideLayout7.xml.rels
--rw-r--r--   0 andy      (1000) andy      (1000)      319 2022-02-10 15:28:55.000000 python-pptx-valutico-0.6.24.2/tests/test_files/expanded_pptx/ppt/slideLayouts/_rels/slideLayout8.xml.rels
--rw-r--r--   0 andy      (1000) andy      (1000)      319 2022-02-10 15:28:55.000000 python-pptx-valutico-0.6.24.2/tests/test_files/expanded_pptx/ppt/slideLayouts/_rels/slideLayout9.xml.rels
--rw-r--r--   0 andy      (1000) andy      (1000)     7473 2022-02-10 15:28:55.000000 python-pptx-valutico-0.6.24.2/tests/test_files/expanded_pptx/ppt/slideLayouts/slideLayout1.xml
--rw-r--r--   0 andy      (1000) andy      (1000)     4783 2022-02-10 15:28:55.000000 python-pptx-valutico-0.6.24.2/tests/test_files/expanded_pptx/ppt/slideLayouts/slideLayout10.xml
--rw-r--r--   0 andy      (1000) andy      (1000)     5131 2022-02-10 15:28:55.000000 python-pptx-valutico-0.6.24.2/tests/test_files/expanded_pptx/ppt/slideLayouts/slideLayout11.xml
--rw-r--r--   0 andy      (1000) andy      (1000)     4786 2022-02-10 15:28:55.000000 python-pptx-valutico-0.6.24.2/tests/test_files/expanded_pptx/ppt/slideLayouts/slideLayout2.xml
--rw-r--r--   0 andy      (1000) andy      (1000)     7613 2022-02-10 15:28:55.000000 python-pptx-valutico-0.6.24.2/tests/test_files/expanded_pptx/ppt/slideLayouts/slideLayout3.xml
--rw-r--r--   0 andy      (1000) andy      (1000)     8154 2022-02-10 15:28:55.000000 python-pptx-valutico-0.6.24.2/tests/test_files/expanded_pptx/ppt/slideLayouts/slideLayout4.xml
--rw-r--r--   0 andy      (1000) andy      (1000)    12501 2022-02-10 15:28:55.000000 python-pptx-valutico-0.6.24.2/tests/test_files/expanded_pptx/ppt/slideLayouts/slideLayout5.xml
--rw-r--r--   0 andy      (1000) andy      (1000)     3371 2022-02-10 15:28:55.000000 python-pptx-valutico-0.6.24.2/tests/test_files/expanded_pptx/ppt/slideLayouts/slideLayout6.xml
--rw-r--r--   0 andy      (1000) andy      (1000)     2757 2022-02-10 15:28:55.000000 python-pptx-valutico-0.6.24.2/tests/test_files/expanded_pptx/ppt/slideLayouts/slideLayout7.xml
--rw-r--r--   0 andy      (1000) andy      (1000)     8100 2022-02-10 15:28:55.000000 python-pptx-valutico-0.6.24.2/tests/test_files/expanded_pptx/ppt/slideLayouts/slideLayout8.xml
--rw-r--r--   0 andy      (1000) andy      (1000)     7633 2022-02-10 15:28:55.000000 python-pptx-valutico-0.6.24.2/tests/test_files/expanded_pptx/ppt/slideLayouts/slideLayout9.xml
-drwxr-xr-x   0 andy      (1000) andy      (1000)        0 2022-05-16 16:04:17.395552 python-pptx-valutico-0.6.24.2/tests/test_files/expanded_pptx/ppt/slideMasters/
-drwxr-xr-x   0 andy      (1000) andy      (1000)        0 2022-05-16 16:04:17.395552 python-pptx-valutico-0.6.24.2/tests/test_files/expanded_pptx/ppt/slideMasters/_rels/
--rw-r--r--   0 andy      (1000) andy      (1000)     2093 2022-02-10 15:28:55.000000 python-pptx-valutico-0.6.24.2/tests/test_files/expanded_pptx/ppt/slideMasters/_rels/slideMaster1.xml.rels
--rw-r--r--   0 andy      (1000) andy      (1000)    17871 2022-02-10 15:28:55.000000 python-pptx-valutico-0.6.24.2/tests/test_files/expanded_pptx/ppt/slideMasters/slideMaster1.xml
-drwxr-xr-x   0 andy      (1000) andy      (1000)        0 2022-05-16 16:04:17.395552 python-pptx-valutico-0.6.24.2/tests/test_files/expanded_pptx/ppt/slides/
-drwxr-xr-x   0 andy      (1000) andy      (1000)        0 2022-05-16 16:04:17.395552 python-pptx-valutico-0.6.24.2/tests/test_files/expanded_pptx/ppt/slides/_rels/
--rw-r--r--   0 andy      (1000) andy      (1000)      315 2022-02-10 15:28:55.000000 python-pptx-valutico-0.6.24.2/tests/test_files/expanded_pptx/ppt/slides/_rels/slide1.xml.rels
--rw-r--r--   0 andy      (1000) andy      (1000)     2198 2022-02-10 15:28:55.000000 python-pptx-valutico-0.6.24.2/tests/test_files/expanded_pptx/ppt/slides/slide1.xml
--rw-r--r--   0 andy      (1000) andy      (1000)      182 2022-02-10 15:28:55.000000 python-pptx-valutico-0.6.24.2/tests/test_files/expanded_pptx/ppt/tableStyles.xml
-drwxr-xr-x   0 andy      (1000) andy      (1000)        0 2022-05-16 16:04:17.395552 python-pptx-valutico-0.6.24.2/tests/test_files/expanded_pptx/ppt/theme/
--rw-r--r--   0 andy      (1000) andy      (1000)    10294 2022-02-10 15:28:55.000000 python-pptx-valutico-0.6.24.2/tests/test_files/expanded_pptx/ppt/theme/theme1.xml
--rw-r--r--   0 andy      (1000) andy      (1000)     1081 2022-02-10 15:28:55.000000 python-pptx-valutico-0.6.24.2/tests/test_files/expanded_pptx/ppt/viewProps.xml
--rw-r--r--   0 andy      (1000) andy      (1000)    15802 2022-02-10 15:28:55.000000 python-pptx-valutico-0.6.24.2/tests/test_files/minimal.pptx
--rw-r--r--   0 andy      (1000) andy      (1000)      477 2022-02-10 15:28:55.000000 python-pptx-valutico-0.6.24.2/tests/test_files/minimal_slide.xml
--rw-r--r--   0 andy      (1000) andy      (1000)    32944 2022-02-10 15:28:55.000000 python-pptx-valutico-0.6.24.2/tests/test_files/missing_rels_item.pptx
--rw-r--r--   0 andy      (1000) andy      (1000)    64276 2022-02-10 15:28:55.000000 python-pptx-valutico-0.6.24.2/tests/test_files/monty-truth.png
--rw-r--r--   0 andy      (1000) andy      (1000)    34436 2022-02-10 15:28:55.000000 python-pptx-valutico-0.6.24.2/tests/test_files/no-core-props.pptx
--rw-r--r--   0 andy      (1000) andy      (1000)    34036 2022-02-10 15:28:55.000000 python-pptx-valutico-0.6.24.2/tests/test_files/no-slides.pptx
--rw-r--r--   0 andy      (1000) andy      (1000)     4157 2022-02-10 15:28:55.000000 python-pptx-valutico-0.6.24.2/tests/test_files/presentation.xml
--rw-r--r--   0 andy      (1000) andy      (1000)     3277 2022-02-10 15:28:55.000000 python-pptx-valutico-0.6.24.2/tests/test_files/python-icon.jpeg
--rw-r--r--   0 andy      (1000) andy      (1000)     6111 2022-02-10 15:28:55.000000 python-pptx-valutico-0.6.24.2/tests/test_files/python-powered.png
--rw-r--r--   0 andy      (1000) andy      (1000)    45210 2022-02-10 15:28:55.000000 python-pptx-valutico-0.6.24.2/tests/test_files/python.bmp
--rw-r--r--   0 andy      (1000) andy      (1000)     8134 2022-02-10 15:28:55.000000 python-pptx-valutico-0.6.24.2/tests/test_files/slideLayout1.xml
-drwxr-xr-x   0 andy      (1000) andy      (1000)        0 2022-05-16 16:04:17.465551 python-pptx-valutico-0.6.24.2/tests/test_files/snippets/
--rw-r--r--   0 andy      (1000) andy      (1000)     4920 2022-02-10 15:28:55.000000 python-pptx-valutico-0.6.24.2/tests/test_files/snippets/2x2-area-date.txt
--rw-r--r--   0 andy      (1000) andy      (1000)     4916 2022-02-10 15:28:55.000000 python-pptx-valutico-0.6.24.2/tests/test_files/snippets/2x2-area-float.txt
--rw-r--r--   0 andy      (1000) andy      (1000)     4816 2022-02-10 15:28:55.000000 python-pptx-valutico-0.6.24.2/tests/test_files/snippets/2x2-area-stacked-100.txt
--rw-r--r--   0 andy      (1000) andy      (1000)     4809 2022-02-10 15:28:55.000000 python-pptx-valutico-0.6.24.2/tests/test_files/snippets/2x2-area-stacked.txt
--rw-r--r--   0 andy      (1000) andy      (1000)     4810 2022-02-10 15:28:55.000000 python-pptx-valutico-0.6.24.2/tests/test_files/snippets/2x2-area.txt
--rw-r--r--   0 andy      (1000) andy      (1000)     4308 2022-02-10 15:34:27.000000 python-pptx-valutico-0.6.24.2/tests/test_files/snippets/2x2-bar-clustered-date.txt
--rw-r--r--   0 andy      (1000) andy      (1000)     4246 2022-02-10 15:34:27.000000 python-pptx-valutico-0.6.24.2/tests/test_files/snippets/2x2-bar-clustered-float.txt
--rw-r--r--   0 andy      (1000) andy      (1000)     4140 2022-02-10 15:34:27.000000 python-pptx-valutico-0.6.24.2/tests/test_files/snippets/2x2-bar-clustered.txt
--rw-r--r--   0 andy      (1000) andy      (1000)     4176 2022-02-10 15:34:27.000000 python-pptx-valutico-0.6.24.2/tests/test_files/snippets/2x2-bar-stacked-100.txt
--rw-r--r--   0 andy      (1000) andy      (1000)     4169 2022-02-10 15:34:27.000000 python-pptx-valutico-0.6.24.2/tests/test_files/snippets/2x2-bar-stacked.txt
--rw-r--r--   0 andy      (1000) andy      (1000)     4140 2022-02-10 15:34:27.000000 python-pptx-valutico-0.6.24.2/tests/test_files/snippets/2x2-column-clustered.txt
--rw-r--r--   0 andy      (1000) andy      (1000)     4176 2022-02-10 15:34:27.000000 python-pptx-valutico-0.6.24.2/tests/test_files/snippets/2x2-column-stacked-100.txt
--rw-r--r--   0 andy      (1000) andy      (1000)     4169 2022-02-10 15:34:27.000000 python-pptx-valutico-0.6.24.2/tests/test_files/snippets/2x2-column-stacked.txt
--rw-r--r--   0 andy      (1000) andy      (1000)     4745 2022-02-10 15:28:55.000000 python-pptx-valutico-0.6.24.2/tests/test_files/snippets/2x2-line-date.txt
--rw-r--r--   0 andy      (1000) andy      (1000)     4683 2022-02-10 15:28:55.000000 python-pptx-valutico-0.6.24.2/tests/test_files/snippets/2x2-line-float.txt
--rw-r--r--   0 andy      (1000) andy      (1000)     4427 2022-02-10 15:28:55.000000 python-pptx-valutico-0.6.24.2/tests/test_files/snippets/2x2-line-markers-stacked-100.txt
--rw-r--r--   0 andy      (1000) andy      (1000)     4420 2022-02-10 15:28:55.000000 python-pptx-valutico-0.6.24.2/tests/test_files/snippets/2x2-line-markers-stacked.txt
--rw-r--r--   0 andy      (1000) andy      (1000)     4421 2022-02-10 15:28:55.000000 python-pptx-valutico-0.6.24.2/tests/test_files/snippets/2x2-line-markers.txt
--rw-r--r--   0 andy      (1000) andy      (1000)     4583 2022-02-10 15:28:55.000000 python-pptx-valutico-0.6.24.2/tests/test_files/snippets/2x2-line-stacked-100.txt
--rw-r--r--   0 andy      (1000) andy      (1000)     4576 2022-02-10 15:28:55.000000 python-pptx-valutico-0.6.24.2/tests/test_files/snippets/2x2-line-stacked.txt
--rw-r--r--   0 andy      (1000) andy      (1000)     4577 2022-02-10 15:28:55.000000 python-pptx-valutico-0.6.24.2/tests/test_files/snippets/2x2-line.txt
--rw-r--r--   0 andy      (1000) andy      (1000)     6440 2022-02-10 15:28:55.000000 python-pptx-valutico-0.6.24.2/tests/test_files/snippets/2x3-bubble-3d.txt
--rw-r--r--   0 andy      (1000) andy      (1000)     6440 2022-02-10 15:28:55.000000 python-pptx-valutico-0.6.24.2/tests/test_files/snippets/2x3-bubble.txt
--rw-r--r--   0 andy      (1000) andy      (1000)     5082 2022-02-10 15:28:55.000000 python-pptx-valutico-0.6.24.2/tests/test_files/snippets/2x3-xy-lines-no-markers.txt
--rw-r--r--   0 andy      (1000) andy      (1000)     4926 2022-02-10 15:28:55.000000 python-pptx-valutico-0.6.24.2/tests/test_files/snippets/2x3-xy-lines.txt
--rw-r--r--   0 andy      (1000) andy      (1000)     5084 2022-02-10 15:28:55.000000 python-pptx-valutico-0.6.24.2/tests/test_files/snippets/2x3-xy-smooth-no-markers.txt
--rw-r--r--   0 andy      (1000) andy      (1000)     4928 2022-02-10 15:28:55.000000 python-pptx-valutico-0.6.24.2/tests/test_files/snippets/2x3-xy-smooth.txt
--rw-r--r--   0 andy      (1000) andy      (1000)     5154 2022-02-10 15:28:55.000000 python-pptx-valutico-0.6.24.2/tests/test_files/snippets/2x3-xy.txt
--rw-r--r--   0 andy      (1000) andy      (1000)     6102 2022-02-10 15:34:27.000000 python-pptx-valutico-0.6.24.2/tests/test_files/snippets/2x5-radar.txt
--rw-r--r--   0 andy      (1000) andy      (1000)     2107 2022-02-10 15:34:27.000000 python-pptx-valutico-0.6.24.2/tests/test_files/snippets/3x1-pie-exploded.txt
--rw-r--r--   0 andy      (1000) andy      (1000)     2073 2022-02-10 15:34:27.000000 python-pptx-valutico-0.6.24.2/tests/test_files/snippets/3x1-pie.txt
--rw-r--r--   0 andy      (1000) andy      (1000)     4141 2022-02-10 15:28:55.000000 python-pptx-valutico-0.6.24.2/tests/test_files/snippets/3x2-doughnut-exploded.txt
--rw-r--r--   0 andy      (1000) andy      (1000)     4073 2022-02-10 15:28:55.000000 python-pptx-valutico-0.6.24.2/tests/test_files/snippets/3x2-doughnut.txt
--rw-r--r--   0 andy      (1000) andy      (1000)     5336 2022-02-10 15:34:27.000000 python-pptx-valutico-0.6.24.2/tests/test_files/snippets/4x2-multi-cat-bar.txt
--rw-r--r--   0 andy      (1000) andy      (1000)     3458 2022-02-10 15:28:55.000000 python-pptx-valutico-0.6.24.2/tests/test_files/snippets/adjust-ser-count.txt
--rw-r--r--   0 andy      (1000) andy      (1000)     3636 2022-02-10 15:28:55.000000 python-pptx-valutico-0.6.24.2/tests/test_files/snippets/cat-labels.txt
--rw-r--r--   0 andy      (1000) andy      (1000)      517 2022-02-10 15:34:27.000000 python-pptx-valutico-0.6.24.2/tests/test_files/snippets/content-types-xml.txt
--rw-r--r--   0 andy      (1000) andy      (1000)      666 2022-02-10 15:28:55.000000 python-pptx-valutico-0.6.24.2/tests/test_files/snippets/default-notes.txt
--rw-r--r--   0 andy      (1000) andy      (1000)    11062 2022-02-10 15:28:55.000000 python-pptx-valutico-0.6.24.2/tests/test_files/snippets/default-notesMaster.txt
--rw-r--r--   0 andy      (1000) andy      (1000)    10896 2022-02-10 15:28:55.000000 python-pptx-valutico-0.6.24.2/tests/test_files/snippets/default-theme.txt
--rw-r--r--   0 andy      (1000) andy      (1000)     1087 2022-02-10 15:28:55.000000 python-pptx-valutico-0.6.24.2/tests/test_files/snippets/freeform.txt
--rw-r--r--   0 andy      (1000) andy      (1000)      757 2022-02-10 15:34:27.000000 python-pptx-valutico-0.6.24.2/tests/test_files/snippets/package-rels-xml.txt
--rw-r--r--   0 andy      (1000) andy      (1000)     1763 2022-02-10 15:28:55.000000 python-pptx-valutico-0.6.24.2/tests/test_files/snippets/placeholders.txt
--rw-r--r--   0 andy      (1000) andy      (1000)      600 2022-02-10 15:34:27.000000 python-pptx-valutico-0.6.24.2/tests/test_files/snippets/presentation-rels-xml.txt
--rw-r--r--   0 andy      (1000) andy      (1000)      445 2022-02-10 15:34:27.000000 python-pptx-valutico-0.6.24.2/tests/test_files/snippets/relationships.txt
--rw-r--r--   0 andy      (1000) andy      (1000)      622 2022-02-10 15:34:27.000000 python-pptx-valutico-0.6.24.2/tests/test_files/snippets/rels-load-from-xml.txt
--rw-r--r--   0 andy      (1000) andy      (1000)    10545 2022-02-10 15:28:55.000000 python-pptx-valutico-0.6.24.2/tests/test_files/snippets/rewrite-ser.txt
--rw-r--r--   0 andy      (1000) andy      (1000)     2792 2022-02-10 15:28:55.000000 python-pptx-valutico-0.6.24.2/tests/test_files/snippets/timing.txt
--rw-r--r--   0 andy      (1000) andy      (1000)    37859 2022-02-10 15:28:55.000000 python-pptx-valutico-0.6.24.2/tests/test_files/test.pptx
--rw-r--r--   0 andy      (1000) andy      (1000)    38616 2022-02-10 15:28:55.000000 python-pptx-valutico-0.6.24.2/tests/test_files/test_slides.pptx
--rw-r--r--   0 andy      (1000) andy      (1000)     4604 2022-02-10 15:34:27.000000 python-pptx-valutico-0.6.24.2/tests/test_media.py
--rw-r--r--   0 andy      (1000) andy      (1000)    13510 2022-02-10 15:34:27.000000 python-pptx-valutico-0.6.24.2/tests/test_package.py
--rw-r--r--   0 andy      (1000) andy      (1000)     8925 2022-02-10 15:28:55.000000 python-pptx-valutico-0.6.24.2/tests/test_presentation.py
--rw-r--r--   0 andy      (1000) andy      (1000)     2455 2022-02-10 15:34:27.000000 python-pptx-valutico-0.6.24.2/tests/test_shared.py
--rw-r--r--   0 andy      (1000) andy      (1000)    39126 2022-02-10 15:34:27.000000 python-pptx-valutico-0.6.24.2/tests/test_slide.py
--rw-r--r--   0 andy      (1000) andy      (1000)    29166 2022-02-10 15:34:27.000000 python-pptx-valutico-0.6.24.2/tests/test_table.py
--rw-r--r--   0 andy      (1000) andy      (1000)     1878 2022-02-10 15:28:55.000000 python-pptx-valutico-0.6.24.2/tests/test_util.py
-drwxr-xr-x   0 andy      (1000) andy      (1000)        0 2022-05-16 16:04:17.475551 python-pptx-valutico-0.6.24.2/tests/text/
--rw-r--r--   0 andy      (1000) andy      (1000)        0 2022-02-10 15:28:55.000000 python-pptx-valutico-0.6.24.2/tests/text/__init__.py
--rw-r--r--   0 andy      (1000) andy      (1000)    25213 2022-02-10 15:34:27.000000 python-pptx-valutico-0.6.24.2/tests/text/test_fonts.py
--rw-r--r--   0 andy      (1000) andy      (1000)     9012 2022-02-10 15:34:27.000000 python-pptx-valutico-0.6.24.2/tests/text/test_layout.py
--rw-r--r--   0 andy      (1000) andy      (1000)    45716 2022-02-10 15:34:27.000000 python-pptx-valutico-0.6.24.2/tests/text/test_text.py
--rw-r--r--   0 andy      (1000) andy      (1000)     3661 2022-02-10 15:34:27.000000 python-pptx-valutico-0.6.24.2/tests/unitdata.py
-drwxr-xr-x   0 andy      (1000) andy      (1000)        0 2022-05-16 16:04:17.475551 python-pptx-valutico-0.6.24.2/tests/unitutil/
--rw-r--r--   0 andy      (1000) andy      (1000)      247 2022-02-10 15:28:55.000000 python-pptx-valutico-0.6.24.2/tests/unitutil/__init__.py
--rw-r--r--   0 andy      (1000) andy      (1000)     8312 2022-02-10 15:34:27.000000 python-pptx-valutico-0.6.24.2/tests/unitutil/cxml.py
--rw-r--r--   0 andy      (1000) andy      (1000)     1855 2022-02-10 15:34:27.000000 python-pptx-valutico-0.6.24.2/tests/unitutil/file.py
--rw-r--r--   0 andy      (1000) andy      (1000)     4129 2022-02-10 15:34:27.000000 python-pptx-valutico-0.6.24.2/tests/unitutil/mock.py
--rw-r--r--   0 andy      (1000) andy      (1000)      652 2022-02-10 15:34:27.000000 python-pptx-valutico-0.6.24.2/tox.ini
+drwxr-xr-x   0 andy      (1000) andy      (1000)        0 2023-05-18 16:21:08.250555 python-pptx-valutico-0.6.24.3/
+-rw-r--r--   0 andy      (1000) andy      (1000)    16391 2023-05-18 16:16:30.000000 python-pptx-valutico-0.6.24.3/HISTORY.rst
+-rw-r--r--   0 andy      (1000) andy      (1000)     1116 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/LICENSE
+-rw-r--r--   0 andy      (1000) andy      (1000)      177 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/MANIFEST.in
+-rw-r--r--   0 andy      (1000) andy      (1000)    18383 2023-05-18 16:21:08.250555 python-pptx-valutico-0.6.24.3/PKG-INFO
+-rw-r--r--   0 andy      (1000) andy      (1000)     1041 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/README.rst
+drwxr-xr-x   0 andy      (1000) andy      (1000)        0 2023-05-18 16:21:08.170555 python-pptx-valutico-0.6.24.3/features/
+-rw-r--r--   0 andy      (1000) andy      (1000)     3215 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/features/act-action.feature
+-rw-r--r--   0 andy      (1000) andy      (1000)     2045 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/features/act-hyperlink.feature
+-rw-r--r--   0 andy      (1000) andy      (1000)     6389 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/features/cht-axis-props.feature
+-rw-r--r--   0 andy      (1000) andy      (1000)     1360 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/features/cht-axistitle-props.feature
+-rw-r--r--   0 andy      (1000) andy      (1000)     2059 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/features/cht-category-access.feature
+-rw-r--r--   0 andy      (1000) andy      (1000)      569 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/features/cht-category-props.feature
+-rw-r--r--   0 andy      (1000) andy      (1000)     4227 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/features/cht-chart.feature
+-rw-r--r--   0 andy      (1000) andy      (1000)     1374 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/features/cht-charttitle-props.feature
+-rw-r--r--   0 andy      (1000) andy      (1000)     4641 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/features/cht-data-props.feature
+-rw-r--r--   0 andy      (1000) andy      (1000)     6935 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/features/cht-datalabels.feature
+-rw-r--r--   0 andy      (1000) andy      (1000)      406 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/features/cht-gridlines-props.feature
+-rw-r--r--   0 andy      (1000) andy      (1000)     1034 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/features/cht-legend-access.feature
+-rw-r--r--   0 andy      (1000) andy      (1000)     3185 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/features/cht-legend-props.feature
+-rw-r--r--   0 andy      (1000) andy      (1000)     1765 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/features/cht-marker-props.feature
+-rw-r--r--   0 andy      (1000) andy      (1000)     4323 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/features/cht-plot-props.feature
+-rw-r--r--   0 andy      (1000) andy      (1000)      945 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/features/cht-point-access.feature
+-rw-r--r--   0 andy      (1000) andy      (1000)      566 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/features/cht-point-props.feature
+-rw-r--r--   0 andy      (1000) andy      (1000)     1471 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/features/cht-replace-data.feature
+-rw-r--r--   0 andy      (1000) andy      (1000)     4648 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/features/cht-series.feature
+-rw-r--r--   0 andy      (1000) andy      (1000)      972 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/features/cht-ticklabels-props.feature
+-rw-r--r--   0 andy      (1000) andy      (1000)      687 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/features/dml-color.feature
+-rw-r--r--   0 andy      (1000) andy      (1000)     1018 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/features/dml-effect.feature
+-rw-r--r--   0 andy      (1000) andy      (1000)     3098 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/features/dml-fill.feature
+-rw-r--r--   0 andy      (1000) andy      (1000)     2163 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/features/dml-line.feature
+-rw-r--r--   0 andy      (1000) andy      (1000)      518 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/features/environment.py
+-rw-r--r--   0 andy      (1000) andy      (1000)     1602 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/features/ph-inherit-props.feature
+-rw-r--r--   0 andy      (1000) andy      (1000)     1391 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/features/ph-insert-shape.feature
+-rw-r--r--   0 andy      (1000) andy      (1000)      815 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/features/ph-phfmt-props.feature
+-rw-r--r--   0 andy      (1000) andy      (1000)     1427 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/features/ph-placeholder-props.feature
+-rw-r--r--   0 andy      (1000) andy      (1000)      992 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/features/prs-coreprops.feature
+-rw-r--r--   0 andy      (1000) andy      (1000)      466 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/features/prs-default-template.feature
+-rw-r--r--   0 andy      (1000) andy      (1000)     1417 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/features/prs-open-save.feature
+-rw-r--r--   0 andy      (1000) andy      (1000)     1134 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/features/prs-presentation-props.feature
+-rw-r--r--   0 andy      (1000) andy      (1000)      761 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/features/shp-autoshape.feature
+-rw-r--r--   0 andy      (1000) andy      (1000)     2720 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/features/shp-connector.feature
+-rw-r--r--   0 andy      (1000) andy      (1000)     2245 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/features/shp-freeform.feature
+-rw-r--r--   0 andy      (1000) andy      (1000)     1622 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/features/shp-graphicframe.feature
+-rw-r--r--   0 andy      (1000) andy      (1000)     1353 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/features/shp-groupshape.feature
+-rw-r--r--   0 andy      (1000) andy      (1000)      568 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/features/shp-movie-props.feature
+-rw-r--r--   0 andy      (1000) andy      (1000)     2475 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/features/shp-picture.feature
+-rw-r--r--   0 andy      (1000) andy      (1000)      612 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/features/shp-placeholder.feature
+-rw-r--r--   0 andy      (1000) andy      (1000)    14081 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/features/shp-shapes.feature
+-rw-r--r--   0 andy      (1000) andy      (1000)     6239 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/features/shp-shared.feature
+-rw-r--r--   0 andy      (1000) andy      (1000)      488 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/features/sld-background.feature
+-rw-r--r--   0 andy      (1000) andy      (1000)     4081 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/features/sld-slide.feature
+-rw-r--r--   0 andy      (1000) andy      (1000)     2339 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/features/sld-slides.feature
+drwxr-xr-x   0 andy      (1000) andy      (1000)        0 2023-05-18 16:21:08.170555 python-pptx-valutico-0.6.24.3/features/steps/
+-rw-r--r--   0 andy      (1000) andy      (1000)     3317 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/features/steps/action.py
+-rw-r--r--   0 andy      (1000) andy      (1000)    11392 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/features/steps/axis.py
+-rw-r--r--   0 andy      (1000) andy      (1000)     1018 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/features/steps/background.py
+-rw-r--r--   0 andy      (1000) andy      (1000)     6013 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/features/steps/category.py
+-rw-r--r--   0 andy      (1000) andy      (1000)    13879 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/features/steps/chart.py
+-rw-r--r--   0 andy      (1000) andy      (1000)     7343 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/features/steps/chartdata.py
+-rw-r--r--   0 andy      (1000) andy      (1000)     2114 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/features/steps/color.py
+-rw-r--r--   0 andy      (1000) andy      (1000)     2756 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/features/steps/coreprops.py
+-rw-r--r--   0 andy      (1000) andy      (1000)     8097 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/features/steps/datalabel.py
+-rw-r--r--   0 andy      (1000) andy      (1000)     1173 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/features/steps/effect.py
+-rw-r--r--   0 andy      (1000) andy      (1000)     5143 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/features/steps/fill.py
+-rw-r--r--   0 andy      (1000) andy      (1000)     4980 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/features/steps/font.py
+-rw-r--r--   0 andy      (1000) andy      (1000)     3371 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/features/steps/font_color.py
+-rw-r--r--   0 andy      (1000) andy      (1000)     1523 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/features/steps/helpers.py
+-rw-r--r--   0 andy      (1000) andy      (1000)     3144 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/features/steps/legend.py
+-rw-r--r--   0 andy      (1000) andy      (1000)     3245 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/features/steps/line.py
+-rw-r--r--   0 andy      (1000) andy      (1000)     2803 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/features/steps/picture.py
+-rw-r--r--   0 andy      (1000) andy      (1000)    11179 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/features/steps/placeholder.py
+-rw-r--r--   0 andy      (1000) andy      (1000)     4809 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/features/steps/plot.py
+-rw-r--r--   0 andy      (1000) andy      (1000)     6035 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/features/steps/presentation.py
+-rw-r--r--   0 andy      (1000) andy      (1000)    12340 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/features/steps/series.py
+-rw-r--r--   0 andy      (1000) andy      (1000)    22389 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/features/steps/shape.py
+-rw-r--r--   0 andy      (1000) andy      (1000)    12099 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/features/steps/shapes.py
+-rw-r--r--   0 andy      (1000) andy      (1000)     7570 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/features/steps/slide.py
+-rw-r--r--   0 andy      (1000) andy      (1000)     4644 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/features/steps/slides.py
+-rw-r--r--   0 andy      (1000) andy      (1000)    10292 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/features/steps/table.py
+drwxr-xr-x   0 andy      (1000) andy      (1000)        0 2023-05-18 16:21:08.200555 python-pptx-valutico-0.6.24.3/features/steps/test_files/
+-rw-r--r--   0 andy      (1000) andy      (1000)     9454 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/features/steps/test_files/72-dpi.tiff
+-rw-r--r--   0 andy      (1000) andy      (1000)     1526 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/features/steps/test_files/CVS_LOGO.WMF
+-rw-r--r--   0 andy      (1000) andy      (1000)   982098 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/features/steps/test_files/act-props.pptm
+-rw-r--r--   0 andy      (1000) andy      (1000)   867288 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/features/steps/test_files/calibriz.ttf
+-rw-r--r--   0 andy      (1000) andy      (1000)   366536 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/features/steps/test_files/cht-axis-props.pptx
+-rw-r--r--   0 andy      (1000) andy      (1000)   222711 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/features/steps/test_files/cht-category-access.pptx
+-rw-r--r--   0 andy      (1000) andy      (1000)   218303 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/features/steps/test_files/cht-chart-props.pptx
+-rw-r--r--   0 andy      (1000) andy      (1000)  1393564 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/features/steps/test_files/cht-chart-type.pptx
+-rw-r--r--   0 andy      (1000) andy      (1000)    77751 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/features/steps/test_files/cht-charts.pptx
+-rw-r--r--   0 andy      (1000) andy      (1000)   243765 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/features/steps/test_files/cht-datalabels.pptx
+-rw-r--r--   0 andy      (1000) andy      (1000)    62864 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/features/steps/test_files/cht-gridlines-props.pptx
+-rw-r--r--   0 andy      (1000) andy      (1000)   145467 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/features/steps/test_files/cht-legend-props.pptx
+-rw-r--r--   0 andy      (1000) andy      (1000)   125134 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/features/steps/test_files/cht-legend.pptx
+-rw-r--r--   0 andy      (1000) andy      (1000)    78544 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/features/steps/test_files/cht-marker-props.pptx
+-rw-r--r--   0 andy      (1000) andy      (1000)   214116 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/features/steps/test_files/cht-plot-props.pptx
+-rw-r--r--   0 andy      (1000) andy      (1000)   145108 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/features/steps/test_files/cht-point-access.pptx
+-rw-r--r--   0 andy      (1000) andy      (1000)   144812 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/features/steps/test_files/cht-point-props.pptx
+-rw-r--r--   0 andy      (1000) andy      (1000)   323685 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/features/steps/test_files/cht-replace-data.pptx
+-rw-r--r--   0 andy      (1000) andy      (1000)   518464 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/features/steps/test_files/cht-series.pptx
+-rw-r--r--   0 andy      (1000) andy      (1000)   127056 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/features/steps/test_files/cht-ticklabels-props.pptx
+-rw-r--r--   0 andy      (1000) andy      (1000)    21620 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/features/steps/test_files/dml-effect.pptx
+-rw-r--r--   0 andy      (1000) andy      (1000)   778084 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/features/steps/test_files/dml-fill.pptx
+-rw-r--r--   0 andy      (1000) andy      (1000)    27246 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/features/steps/test_files/dml-line.pptx
+-rw-r--r--   0 andy      (1000) andy      (1000)    21457 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/features/steps/test_files/ext-rels.pptx
+drwxr-xr-x   0 andy      (1000) andy      (1000)        0 2023-05-18 16:21:08.200555 python-pptx-valutico-0.6.24.3/features/steps/test_files/extracted-pptx/
+-rw-r--r--   0 andy      (1000) andy      (1000)     3332 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/features/steps/test_files/extracted-pptx/[Content_Types].xml
+drwxr-xr-x   0 andy      (1000) andy      (1000)        0 2023-05-18 16:21:08.200555 python-pptx-valutico-0.6.24.3/features/steps/test_files/extracted-pptx/_rels/
+-rw-r--r--   0 andy      (1000) andy      (1000)      751 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/features/steps/test_files/extracted-pptx/_rels/.rels
+drwxr-xr-x   0 andy      (1000) andy      (1000)        0 2023-05-18 16:21:08.200555 python-pptx-valutico-0.6.24.3/features/steps/test_files/extracted-pptx/docProps/
+-rw-r--r--   0 andy      (1000) andy      (1000)     1356 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/features/steps/test_files/extracted-pptx/docProps/app.xml
+-rw-r--r--   0 andy      (1000) andy      (1000)      765 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/features/steps/test_files/extracted-pptx/docProps/core.xml
+-rw-r--r--   0 andy      (1000) andy      (1000)     8147 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/features/steps/test_files/extracted-pptx/docProps/thumbnail.jpeg
+drwxr-xr-x   0 andy      (1000) andy      (1000)        0 2023-05-18 16:21:08.200555 python-pptx-valutico-0.6.24.3/features/steps/test_files/extracted-pptx/ppt/
+drwxr-xr-x   0 andy      (1000) andy      (1000)        0 2023-05-18 16:21:08.200555 python-pptx-valutico-0.6.24.3/features/steps/test_files/extracted-pptx/ppt/_rels/
+-rw-r--r--   0 andy      (1000) andy      (1000)     1160 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/features/steps/test_files/extracted-pptx/ppt/_rels/presentation.xml.rels
+-rw-r--r--   0 andy      (1000) andy      (1000)      692 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/features/steps/test_files/extracted-pptx/ppt/presProps.xml
+-rw-r--r--   0 andy      (1000) andy      (1000)     4000 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/features/steps/test_files/extracted-pptx/ppt/presentation.xml
+drwxr-xr-x   0 andy      (1000) andy      (1000)        0 2023-05-18 16:21:08.200555 python-pptx-valutico-0.6.24.3/features/steps/test_files/extracted-pptx/ppt/printerSettings/
+-rw-r--r--   0 andy      (1000) andy      (1000)     9395 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/features/steps/test_files/extracted-pptx/ppt/printerSettings/printerSettings1.bin
+drwxr-xr-x   0 andy      (1000) andy      (1000)        0 2023-05-18 16:21:08.200555 python-pptx-valutico-0.6.24.3/features/steps/test_files/extracted-pptx/ppt/slideLayouts/
+drwxr-xr-x   0 andy      (1000) andy      (1000)        0 2023-05-18 16:21:08.200555 python-pptx-valutico-0.6.24.3/features/steps/test_files/extracted-pptx/ppt/slideLayouts/_rels/
+-rw-r--r--   0 andy      (1000) andy      (1000)      315 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/features/steps/test_files/extracted-pptx/ppt/slideLayouts/_rels/slideLayout1.xml.rels
+-rw-r--r--   0 andy      (1000) andy      (1000)      315 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/features/steps/test_files/extracted-pptx/ppt/slideLayouts/_rels/slideLayout10.xml.rels
+-rw-r--r--   0 andy      (1000) andy      (1000)      315 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/features/steps/test_files/extracted-pptx/ppt/slideLayouts/_rels/slideLayout11.xml.rels
+-rw-r--r--   0 andy      (1000) andy      (1000)      315 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/features/steps/test_files/extracted-pptx/ppt/slideLayouts/_rels/slideLayout2.xml.rels
+-rw-r--r--   0 andy      (1000) andy      (1000)      315 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/features/steps/test_files/extracted-pptx/ppt/slideLayouts/_rels/slideLayout3.xml.rels
+-rw-r--r--   0 andy      (1000) andy      (1000)      315 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/features/steps/test_files/extracted-pptx/ppt/slideLayouts/_rels/slideLayout4.xml.rels
+-rw-r--r--   0 andy      (1000) andy      (1000)      315 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/features/steps/test_files/extracted-pptx/ppt/slideLayouts/_rels/slideLayout5.xml.rels
+-rw-r--r--   0 andy      (1000) andy      (1000)      315 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/features/steps/test_files/extracted-pptx/ppt/slideLayouts/_rels/slideLayout6.xml.rels
+-rw-r--r--   0 andy      (1000) andy      (1000)      315 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/features/steps/test_files/extracted-pptx/ppt/slideLayouts/_rels/slideLayout7.xml.rels
+-rw-r--r--   0 andy      (1000) andy      (1000)      315 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/features/steps/test_files/extracted-pptx/ppt/slideLayouts/_rels/slideLayout8.xml.rels
+-rw-r--r--   0 andy      (1000) andy      (1000)      315 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/features/steps/test_files/extracted-pptx/ppt/slideLayouts/_rels/slideLayout9.xml.rels
+-rw-r--r--   0 andy      (1000) andy      (1000)     7176 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/features/steps/test_files/extracted-pptx/ppt/slideLayouts/slideLayout1.xml
+-rw-r--r--   0 andy      (1000) andy      (1000)     4616 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/features/steps/test_files/extracted-pptx/ppt/slideLayouts/slideLayout10.xml
+-rw-r--r--   0 andy      (1000) andy      (1000)     4954 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/features/steps/test_files/extracted-pptx/ppt/slideLayouts/slideLayout11.xml
+-rw-r--r--   0 andy      (1000) andy      (1000)     4561 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/features/steps/test_files/extracted-pptx/ppt/slideLayouts/slideLayout2.xml
+-rw-r--r--   0 andy      (1000) andy      (1000)     7312 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/features/steps/test_files/extracted-pptx/ppt/slideLayouts/slideLayout3.xml
+-rw-r--r--   0 andy      (1000) andy      (1000)     7811 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/features/steps/test_files/extracted-pptx/ppt/slideLayouts/slideLayout4.xml
+-rw-r--r--   0 andy      (1000) andy      (1000)    12024 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/features/steps/test_files/extracted-pptx/ppt/slideLayouts/slideLayout5.xml
+-rw-r--r--   0 andy      (1000) andy      (1000)     3198 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/features/steps/test_files/extracted-pptx/ppt/slideLayouts/slideLayout6.xml
+-rw-r--r--   0 andy      (1000) andy      (1000)     2607 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/features/steps/test_files/extracted-pptx/ppt/slideLayouts/slideLayout7.xml
+-rw-r--r--   0 andy      (1000) andy      (1000)     7768 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/features/steps/test_files/extracted-pptx/ppt/slideLayouts/slideLayout8.xml
+-rw-r--r--   0 andy      (1000) andy      (1000)     7325 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/features/steps/test_files/extracted-pptx/ppt/slideLayouts/slideLayout9.xml
+drwxr-xr-x   0 andy      (1000) andy      (1000)        0 2023-05-18 16:21:08.200555 python-pptx-valutico-0.6.24.3/features/steps/test_files/extracted-pptx/ppt/slideMasters/
+drwxr-xr-x   0 andy      (1000) andy      (1000)        0 2023-05-18 16:21:08.200555 python-pptx-valutico-0.6.24.3/features/steps/test_files/extracted-pptx/ppt/slideMasters/_rels/
+-rw-r--r--   0 andy      (1000) andy      (1000)     2028 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/features/steps/test_files/extracted-pptx/ppt/slideMasters/_rels/slideMaster1.xml.rels
+-rw-r--r--   0 andy      (1000) andy      (1000)    17336 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/features/steps/test_files/extracted-pptx/ppt/slideMasters/slideMaster1.xml
+drwxr-xr-x   0 andy      (1000) andy      (1000)        0 2023-05-18 16:21:08.200555 python-pptx-valutico-0.6.24.3/features/steps/test_files/extracted-pptx/ppt/slides/
+drwxr-xr-x   0 andy      (1000) andy      (1000)        0 2023-05-18 16:21:08.200555 python-pptx-valutico-0.6.24.3/features/steps/test_files/extracted-pptx/ppt/slides/_rels/
+-rw-r--r--   0 andy      (1000) andy      (1000)      315 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/features/steps/test_files/extracted-pptx/ppt/slides/_rels/slide1.xml.rels
+-rw-r--r--   0 andy      (1000) andy      (1000)     2128 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/features/steps/test_files/extracted-pptx/ppt/slides/slide1.xml
+-rw-r--r--   0 andy      (1000) andy      (1000)      182 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/features/steps/test_files/extracted-pptx/ppt/tableStyles.xml
+drwxr-xr-x   0 andy      (1000) andy      (1000)        0 2023-05-18 16:21:08.200555 python-pptx-valutico-0.6.24.3/features/steps/test_files/extracted-pptx/ppt/theme/
+-rw-r--r--   0 andy      (1000) andy      (1000)    10013 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/features/steps/test_files/extracted-pptx/ppt/theme/theme1.xml
+-rw-r--r--   0 andy      (1000) andy      (1000)     1022 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/features/steps/test_files/extracted-pptx/ppt/viewProps.xml
+-rw-r--r--   0 andy      (1000) andy      (1000)    25061 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/features/steps/test_files/font-color.pptx
+-rwxr-xr-x   0 andy      (1000) andy      (1000)   470987 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/features/steps/test_files/just-two-mice.mp4
+-rw-r--r--   0 andy      (1000) andy      (1000)   179346 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/features/steps/test_files/just-two-mice.png
+-rw-r--r--   0 andy      (1000) andy      (1000)    23202 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/features/steps/test_files/lyt-shapes.pptx
+-rw-r--r--   0 andy      (1000) andy      (1000)    15802 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/features/steps/test_files/minimal.pptx
+-rw-r--r--   0 andy      (1000) andy      (1000)    64276 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/features/steps/test_files/monty-truth.png
+-rw-r--r--   0 andy      (1000) andy      (1000)    25251 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/features/steps/test_files/mst-placeholders.pptx
+-rw-r--r--   0 andy      (1000) andy      (1000)    25539 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/features/steps/test_files/mst-shapes.pptx
+-rw-r--r--   0 andy      (1000) andy      (1000)    21166 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/features/steps/test_files/mst-slide-layouts.pptx
+-rw-r--r--   0 andy      (1000) andy      (1000)    23566 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/features/steps/test_files/ph-inherit-props.pptx
+-rw-r--r--   0 andy      (1000) andy      (1000)   172254 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/features/steps/test_files/ph-populated-placeholders.pptx
+-rw-r--r--   0 andy      (1000) andy      (1000)    34405 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/features/steps/test_files/ph-unpopulated-placeholders.pptx
+-rwxr-xr-x   0 andy      (1000) andy      (1000)    49704 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/features/steps/test_files/pic.emf
+-rw-r--r--   0 andy      (1000) andy      (1000)    19655 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/features/steps/test_files/prs-add-slide.pptx
+-rw-r--r--   0 andy      (1000) andy      (1000)    86792 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/features/steps/test_files/prs-notes.pptx
+-rw-r--r--   0 andy      (1000) andy      (1000)    15806 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/features/steps/test_files/prs-properties.pptx
+-rw-r--r--   0 andy      (1000) andy      (1000)    21528 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/features/steps/test_files/prs-slide-masters.pptx
+-rw-r--r--   0 andy      (1000) andy      (1000)     3277 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/features/steps/test_files/python-icon.jpeg
+-rw-r--r--   0 andy      (1000) andy      (1000)     6111 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/features/steps/test_files/python-powered.png
+-rw-r--r--   0 andy      (1000) andy      (1000)    45210 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/features/steps/test_files/python.bmp
+-rw-r--r--   0 andy      (1000) andy      (1000)    80038 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/features/steps/test_files/shp-access-chart.pptx
+-rw-r--r--   0 andy      (1000) andy      (1000)   119022 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/features/steps/test_files/shp-access-ole-object.pptx
+-rw-r--r--   0 andy      (1000) andy      (1000)    17626 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/features/steps/test_files/shp-autoshape-adjustments.pptx
+-rw-r--r--   0 andy      (1000) andy      (1000)    22929 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/features/steps/test_files/shp-autoshape-props.pptx
+-rw-r--r--   0 andy      (1000) andy      (1000)    81639 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/features/steps/test_files/shp-common-props.pptx
+-rw-r--r--   0 andy      (1000) andy      (1000)    22899 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/features/steps/test_files/shp-connector-props.pptx
+-rw-r--r--   0 andy      (1000) andy      (1000)    11680 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/features/steps/test_files/shp-embedded-docx.docx
+-rw-r--r--   0 andy      (1000) andy      (1000)    29214 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/features/steps/test_files/shp-embedded-pptx.pptx
+-rw-r--r--   0 andy      (1000) andy      (1000)     8250 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/features/steps/test_files/shp-embedded-xlsx.xlsx
+-rw-r--r--   0 andy      (1000) andy      (1000)    16704 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/features/steps/test_files/shp-freeform.pptx
+-rw-r--r--   0 andy      (1000) andy      (1000)    23786 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/features/steps/test_files/shp-groupshape.pptx
+-rw-r--r--   0 andy      (1000) andy      (1000)   684874 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/features/steps/test_files/shp-movie-props.pptx
+-rw-r--r--   0 andy      (1000) andy      (1000)    91730 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/features/steps/test_files/shp-picture.pptx
+-rw-r--r--   0 andy      (1000) andy      (1000)    94116 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/features/steps/test_files/shp-pos-and-size.pptx
+-rw-r--r--   0 andy      (1000) andy      (1000)   125205 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/features/steps/test_files/shp-shapes.pptx
+-rw-r--r--   0 andy      (1000) andy      (1000)    17676 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/features/steps/test_files/sld-background.pptx
+-rw-r--r--   0 andy      (1000) andy      (1000)    16703 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/features/steps/test_files/sld-blank.pptx
+-rw-r--r--   0 andy      (1000) andy      (1000)    22964 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/features/steps/test_files/sld-notes.pptx
+-rw-r--r--   0 andy      (1000) andy      (1000)    18894 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/features/steps/test_files/sld-slide.pptx
+-rw-r--r--   0 andy      (1000) andy      (1000)    18478 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/features/steps/test_files/sld-slides.pptx
+-rw-r--r--   0 andy      (1000) andy      (1000)    33273 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/features/steps/test_files/sonic.gif
+-rw-r--r--   0 andy      (1000) andy      (1000)    28247 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/features/steps/test_files/tbl-cell.pptx
+-rw-r--r--   0 andy      (1000) andy      (1000)    37859 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/features/steps/test_files/test.pptx
+-rw-r--r--   0 andy      (1000) andy      (1000)    21337 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/features/steps/test_files/txt-fit-text.pptx
+-rw-r--r--   0 andy      (1000) andy      (1000)    18874 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/features/steps/test_files/txt-font-props.pptx
+-rw-r--r--   0 andy      (1000) andy      (1000)    25817 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/features/steps/test_files/txt-font-typeface.pptx
+-rw-r--r--   0 andy      (1000) andy      (1000)    24620 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/features/steps/test_files/txt-paragraph-spacing.pptx
+-rw-r--r--   0 andy      (1000) andy      (1000)    27659 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/features/steps/test_files/txt-text-frame.pptx
+-rw-r--r--   0 andy      (1000) andy      (1000)    16051 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/features/steps/test_files/txt-text.pptx
+-rw-r--r--   0 andy      (1000) andy      (1000)     8264 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/features/steps/text.py
+-rw-r--r--   0 andy      (1000) andy      (1000)     4615 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/features/steps/text_frame.py
+-rw-r--r--   0 andy      (1000) andy      (1000)     3549 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/features/tbl-cell.feature
+-rw-r--r--   0 andy      (1000) andy      (1000)      343 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/features/tbl-column.feature
+-rw-r--r--   0 andy      (1000) andy      (1000)     1565 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/features/tbl-table.feature
+-rw-r--r--   0 andy      (1000) andy      (1000)      471 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/features/txt-fit-text.feature
+-rw-r--r--   0 andy      (1000) andy      (1000)     1733 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/features/txt-font-color.feature
+-rw-r--r--   0 andy      (1000) andy      (1000)     4945 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/features/txt-font-props.feature
+-rw-r--r--   0 andy      (1000) andy      (1000)     3969 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/features/txt-paragraph.feature
+-rw-r--r--   0 andy      (1000) andy      (1000)      734 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/features/txt-text.feature
+-rw-r--r--   0 andy      (1000) andy      (1000)     2371 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/features/txt-textframe.feature
+drwxr-xr-x   0 andy      (1000) andy      (1000)        0 2023-05-18 16:21:08.200555 python-pptx-valutico-0.6.24.3/pptx/
+-rw-r--r--   0 andy      (1000) andy      (1000)     1949 2023-05-18 16:16:30.000000 python-pptx-valutico-0.6.24.3/pptx/__init__.py
+-rw-r--r--   0 andy      (1000) andy      (1000)     8672 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/pptx/action.py
+-rw-r--r--   0 andy      (1000) andy      (1000)     1593 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/pptx/api.py
+drwxr-xr-x   0 andy      (1000) andy      (1000)        0 2023-05-18 16:21:08.210555 python-pptx-valutico-0.6.24.3/pptx/chart/
+-rw-r--r--   0 andy      (1000) andy      (1000)        0 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/pptx/chart/__init__.py
+-rw-r--r--   0 andy      (1000) andy      (1000)    17304 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/pptx/chart/axis.py
+-rw-r--r--   0 andy      (1000) andy      (1000)     7250 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/pptx/chart/category.py
+-rw-r--r--   0 andy      (1000) andy      (1000)     9999 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/pptx/chart/chart.py
+-rw-r--r--   0 andy      (1000) andy      (1000)    29740 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/pptx/chart/data.py
+-rw-r--r--   0 andy      (1000) andy      (1000)     9528 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/pptx/chart/datalabel.py
+-rw-r--r--   0 andy      (1000) andy      (1000)     2566 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/pptx/chart/legend.py
+-rw-r--r--   0 andy      (1000) andy      (1000)     2130 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/pptx/chart/marker.py
+-rw-r--r--   0 andy      (1000) andy      (1000)    13213 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/pptx/chart/plot.py
+-rw-r--r--   0 andy      (1000) andy      (1000)     2797 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/pptx/chart/point.py
+-rw-r--r--   0 andy      (1000) andy      (1000)     7484 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/pptx/chart/series.py
+-rw-r--r--   0 andy      (1000) andy      (1000)    10942 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/pptx/chart/xlsx.py
+-rw-r--r--   0 andy      (1000) andy      (1000)    67673 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/pptx/chart/xmlwriter.py
+drwxr-xr-x   0 andy      (1000) andy      (1000)        0 2023-05-18 16:21:08.210555 python-pptx-valutico-0.6.24.3/pptx/compat/
+-rw-r--r--   0 andy      (1000) andy      (1000)      703 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/pptx/compat/__init__.py
+-rw-r--r--   0 andy      (1000) andy      (1000)     1302 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/pptx/compat/python2.py
+-rw-r--r--   0 andy      (1000) andy      (1000)      920 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/pptx/compat/python3.py
+drwxr-xr-x   0 andy      (1000) andy      (1000)        0 2023-05-18 16:21:08.210555 python-pptx-valutico-0.6.24.3/pptx/dml/
+-rw-r--r--   0 andy      (1000) andy      (1000)        0 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/pptx/dml/__init__.py
+-rw-r--r--   0 andy      (1000) andy      (1000)     1373 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/pptx/dml/chtfmt.py
+-rw-r--r--   0 andy      (1000) andy      (1000)     9124 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/pptx/dml/color.py
+-rw-r--r--   0 andy      (1000) andy      (1000)     1592 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/pptx/dml/effect.py
+-rw-r--r--   0 andy      (1000) andy      (1000)    13237 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/pptx/dml/fill.py
+-rw-r--r--   0 andy      (1000) andy      (1000)     3108 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/pptx/dml/line.py
+drwxr-xr-x   0 andy      (1000) andy      (1000)        0 2023-05-18 16:21:08.210555 python-pptx-valutico-0.6.24.3/pptx/enum/
+-rw-r--r--   0 andy      (1000) andy      (1000)        0 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/pptx/enum/__init__.py
+-rw-r--r--   0 andy      (1000) andy      (1000)     1548 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/pptx/enum/action.py
+-rw-r--r--   0 andy      (1000) andy      (1000)    10697 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/pptx/enum/base.py
+-rw-r--r--   0 andy      (1000) andy      (1000)    13226 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/pptx/enum/chart.py
+-rw-r--r--   0 andy      (1000) andy      (1000)    11940 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/pptx/enum/dml.py
+-rw-r--r--   0 andy      (1000) andy      (1000)    22808 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/pptx/enum/lang.py
+-rw-r--r--   0 andy      (1000) andy      (1000)    31458 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/pptx/enum/shapes.py
+-rw-r--r--   0 andy      (1000) andy      (1000)     8215 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/pptx/enum/text.py
+-rw-r--r--   0 andy      (1000) andy      (1000)      457 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/pptx/exc.py
+-rw-r--r--   0 andy      (1000) andy      (1000)    10532 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/pptx/media.py
+drwxr-xr-x   0 andy      (1000) andy      (1000)        0 2023-05-18 16:21:08.210555 python-pptx-valutico-0.6.24.3/pptx/opc/
+-rw-r--r--   0 andy      (1000) andy      (1000)        0 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/pptx/opc/__init__.py
+-rw-r--r--   0 andy      (1000) andy      (1000)    19950 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/pptx/opc/constants.py
+-rw-r--r--   0 andy      (1000) andy      (1000)     4514 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/pptx/opc/oxml.py
+-rw-r--r--   0 andy      (1000) andy      (1000)    26976 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/pptx/opc/package.py
+-rw-r--r--   0 andy      (1000) andy      (1000)     3880 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/pptx/opc/packuri.py
+-rw-r--r--   0 andy      (1000) andy      (1000)     9969 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/pptx/opc/serialized.py
+-rw-r--r--   0 andy      (1000) andy      (1000)      692 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/pptx/opc/shared.py
+-rw-r--r--   0 andy      (1000) andy      (1000)     1012 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/pptx/opc/spec.py
+drwxr-xr-x   0 andy      (1000) andy      (1000)        0 2023-05-18 16:21:08.210555 python-pptx-valutico-0.6.24.3/pptx/oxml/
+-rw-r--r--   0 andy      (1000) andy      (1000)    15446 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/pptx/oxml/__init__.py
+-rw-r--r--   0 andy      (1000) andy      (1000)     1604 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/pptx/oxml/action.py
+drwxr-xr-x   0 andy      (1000) andy      (1000)        0 2023-05-18 16:21:08.210555 python-pptx-valutico-0.6.24.3/pptx/oxml/chart/
+-rw-r--r--   0 andy      (1000) andy      (1000)        0 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/pptx/oxml/chart/__init__.py
+-rw-r--r--   0 andy      (1000) andy      (1000)     9428 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/pptx/oxml/chart/axis.py
+-rw-r--r--   0 andy      (1000) andy      (1000)     8190 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/pptx/oxml/chart/chart.py
+-rw-r--r--   0 andy      (1000) andy      (1000)     7765 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/pptx/oxml/chart/datalabel.py
+-rw-r--r--   0 andy      (1000) andy      (1000)     2129 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/pptx/oxml/chart/legend.py
+-rw-r--r--   0 andy      (1000) andy      (1000)     1838 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/pptx/oxml/chart/marker.py
+-rw-r--r--   0 andy      (1000) andy      (1000)     9224 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/pptx/oxml/chart/plot.py
+-rw-r--r--   0 andy      (1000) andy      (1000)     7625 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/pptx/oxml/chart/series.py
+-rw-r--r--   0 andy      (1000) andy      (1000)     6097 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/pptx/oxml/chart/shared.py
+-rw-r--r--   0 andy      (1000) andy      (1000)     9820 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/pptx/oxml/coreprops.py
+drwxr-xr-x   0 andy      (1000) andy      (1000)        0 2023-05-18 16:21:08.210555 python-pptx-valutico-0.6.24.3/pptx/oxml/dml/
+-rw-r--r--   0 andy      (1000) andy      (1000)        0 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/pptx/oxml/dml/__init__.py
+-rw-r--r--   0 andy      (1000) andy      (1000)     2477 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/pptx/oxml/dml/color.py
+-rw-r--r--   0 andy      (1000) andy      (1000)     5981 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/pptx/oxml/dml/fill.py
+-rw-r--r--   0 andy      (1000) andy      (1000)      446 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/pptx/oxml/dml/line.py
+-rw-r--r--   0 andy      (1000) andy      (1000)     6779 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/pptx/oxml/ns.py
+-rw-r--r--   0 andy      (1000) andy      (1000)     2795 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/pptx/oxml/presentation.py
+drwxr-xr-x   0 andy      (1000) andy      (1000)        0 2023-05-18 16:21:08.220555 python-pptx-valutico-0.6.24.3/pptx/oxml/shapes/
+-rw-r--r--   0 andy      (1000) andy      (1000)        0 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/pptx/oxml/shapes/__init__.py
+-rw-r--r--   0 andy      (1000) andy      (1000)    13400 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/pptx/oxml/shapes/autoshape.py
+-rw-r--r--   0 andy      (1000) andy      (1000)     3518 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/pptx/oxml/shapes/connector.py
+-rw-r--r--   0 andy      (1000) andy      (1000)    12053 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/pptx/oxml/shapes/graphfrm.py
+-rw-r--r--   0 andy      (1000) andy      (1000)     9214 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/pptx/oxml/shapes/groupshape.py
+-rw-r--r--   0 andy      (1000) andy      (1000)     8096 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/pptx/oxml/shapes/picture.py
+-rw-r--r--   0 andy      (1000) andy      (1000)    12696 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/pptx/oxml/shapes/shared.py
+-rw-r--r--   0 andy      (1000) andy      (1000)    19929 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/pptx/oxml/simpletypes.py
+-rw-r--r--   0 andy      (1000) andy      (1000)    10213 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/pptx/oxml/slide.py
+-rw-r--r--   0 andy      (1000) andy      (1000)    18277 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/pptx/oxml/table.py
+-rw-r--r--   0 andy      (1000) andy      (1000)    16439 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/pptx/oxml/text.py
+-rw-r--r--   0 andy      (1000) andy      (1000)      754 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/pptx/oxml/theme.py
+-rw-r--r--   0 andy      (1000) andy      (1000)    25027 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/pptx/oxml/xmlchemy.py
+-rw-r--r--   0 andy      (1000) andy      (1000)     7626 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/pptx/package.py
+drwxr-xr-x   0 andy      (1000) andy      (1000)        0 2023-05-18 16:21:08.220555 python-pptx-valutico-0.6.24.3/pptx/parts/
+-rw-r--r--   0 andy      (1000) andy      (1000)        0 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/pptx/parts/__init__.py
+-rw-r--r--   0 andy      (1000) andy      (1000)     3000 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/pptx/parts/chart.py
+-rw-r--r--   0 andy      (1000) andy      (1000)     4052 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/pptx/parts/coreprops.py
+-rw-r--r--   0 andy      (1000) andy      (1000)     2815 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/pptx/parts/embeddedpackage.py
+-rw-r--r--   0 andy      (1000) andy      (1000)     9038 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/pptx/parts/image.py
+-rw-r--r--   0 andy      (1000) andy      (1000)      901 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/pptx/parts/media.py
+-rw-r--r--   0 andy      (1000) andy      (1000)     4477 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/pptx/parts/presentation.py
+-rw-r--r--   0 andy      (1000) andy      (1000)    10432 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/pptx/parts/slide.py
+-rw-r--r--   0 andy      (1000) andy      (1000)     4510 2023-05-18 16:16:30.000000 python-pptx-valutico-0.6.24.3/pptx/presentation.py
+drwxr-xr-x   0 andy      (1000) andy      (1000)        0 2023-05-18 16:21:08.220555 python-pptx-valutico-0.6.24.3/pptx/shapes/
+-rw-r--r--   0 andy      (1000) andy      (1000)      589 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/pptx/shapes/__init__.py
+-rw-r--r--   0 andy      (1000) andy      (1000)    13710 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/pptx/shapes/autoshape.py
+-rw-r--r--   0 andy      (1000) andy      (1000)     7574 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/pptx/shapes/base.py
+-rw-r--r--   0 andy      (1000) andy      (1000)    10063 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/pptx/shapes/connector.py
+-rw-r--r--   0 andy      (1000) andy      (1000)    10933 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/pptx/shapes/freeform.py
+-rw-r--r--   0 andy      (1000) andy      (1000)     5005 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/pptx/shapes/graphfrm.py
+-rw-r--r--   0 andy      (1000) andy      (1000)     1859 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/pptx/shapes/group.py
+-rw-r--r--   0 andy      (1000) andy      (1000)     6637 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/pptx/shapes/picture.py
+-rw-r--r--   0 andy      (1000) andy      (1000)    14539 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/pptx/shapes/placeholder.py
+-rw-r--r--   0 andy      (1000) andy      (1000)    41368 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/pptx/shapes/shapetree.py
+-rw-r--r--   0 andy      (1000) andy      (1000)     2593 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/pptx/shared.py
+-rw-r--r--   0 andy      (1000) andy      (1000)    17890 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/pptx/slide.py
+-rw-r--r--   0 andy      (1000) andy      (1000)    23582 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/pptx/spec.py
+-rw-r--r--   0 andy      (1000) andy      (1000)    17813 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/pptx/table.py
+drwxr-xr-x   0 andy      (1000) andy      (1000)        0 2023-05-18 16:21:08.220555 python-pptx-valutico-0.6.24.3/pptx/templates/
+-rw-r--r--   0 andy      (1000) andy      (1000)    34030 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/pptx/templates/default.pptx
+-rw-r--r--   0 andy      (1000) andy      (1000)   127228 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/pptx/templates/docx-icon.emf
+-rw-r--r--   0 andy      (1000) andy      (1000)     5396 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/pptx/templates/generic-icon.emf
+-rw-r--r--   0 andy      (1000) andy      (1000)      722 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/pptx/templates/notes.xml
+-rw-r--r--   0 andy      (1000) andy      (1000)    11135 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/pptx/templates/notesMaster.xml
+-rw-r--r--   0 andy      (1000) andy      (1000)     5492 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/pptx/templates/pptx-icon.emf
+-rw-r--r--   0 andy      (1000) andy      (1000)    10964 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/pptx/templates/theme.xml
+-rw-r--r--   0 andy      (1000) andy      (1000)   130380 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/pptx/templates/xlsx-icon.emf
+drwxr-xr-x   0 andy      (1000) andy      (1000)        0 2023-05-18 16:21:08.220555 python-pptx-valutico-0.6.24.3/pptx/text/
+-rw-r--r--   0 andy      (1000) andy      (1000)        0 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/pptx/text/__init__.py
+-rw-r--r--   0 andy      (1000) andy      (1000)    12900 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/pptx/text/fonts.py
+-rw-r--r--   0 andy      (1000) andy      (1000)     9959 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/pptx/text/layout.py
+-rw-r--r--   0 andy      (1000) andy      (1000)    25179 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/pptx/text/text.py
+-rw-r--r--   0 andy      (1000) andy      (1000)     7826 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/pptx/util.py
+drwxr-xr-x   0 andy      (1000) andy      (1000)        0 2023-05-18 16:21:08.220555 python-pptx-valutico-0.6.24.3/python_pptx_valutico.egg-info/
+-rw-r--r--   0 andy      (1000) andy      (1000)    18383 2023-05-18 16:21:08.000000 python-pptx-valutico-0.6.24.3/python_pptx_valutico.egg-info/PKG-INFO
+-rw-r--r--   0 andy      (1000) andy      (1000)    18710 2023-05-18 16:21:08.000000 python-pptx-valutico-0.6.24.3/python_pptx_valutico.egg-info/SOURCES.txt
+-rw-r--r--   0 andy      (1000) andy      (1000)        1 2023-05-18 16:21:08.000000 python-pptx-valutico-0.6.24.3/python_pptx_valutico.egg-info/dependency_links.txt
+-rw-r--r--   0 andy      (1000) andy      (1000)        1 2023-05-18 16:21:08.000000 python-pptx-valutico-0.6.24.3/python_pptx_valutico.egg-info/not-zip-safe
+-rw-r--r--   0 andy      (1000) andy      (1000)       44 2023-05-18 16:21:08.000000 python-pptx-valutico-0.6.24.3/python_pptx_valutico.egg-info/requires.txt
+-rw-r--r--   0 andy      (1000) andy      (1000)        5 2023-05-18 16:21:08.000000 python-pptx-valutico-0.6.24.3/python_pptx_valutico.egg-info/top_level.txt
+-rw-r--r--   0 andy      (1000) andy      (1000)       38 2023-05-18 16:21:08.250555 python-pptx-valutico-0.6.24.3/setup.cfg
+-rwxr-xr-x   0 andy      (1000) andy      (1000)     2690 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/setup.py
+drwxr-xr-x   0 andy      (1000) andy      (1000)        0 2023-05-18 16:21:08.230555 python-pptx-valutico-0.6.24.3/tests/
+-rw-r--r--   0 andy      (1000) andy      (1000)        0 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/tests/__init__.py
+drwxr-xr-x   0 andy      (1000) andy      (1000)        0 2023-05-18 16:21:08.230555 python-pptx-valutico-0.6.24.3/tests/chart/
+-rw-r--r--   0 andy      (1000) andy      (1000)        0 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/tests/chart/__init__.py
+-rw-r--r--   0 andy      (1000) andy      (1000)    48371 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/tests/chart/test_axis.py
+-rw-r--r--   0 andy      (1000) andy      (1000)     9346 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/tests/chart/test_category.py
+-rw-r--r--   0 andy      (1000) andy      (1000)    21201 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/tests/chart/test_chart.py
+-rw-r--r--   0 andy      (1000) andy      (1000)    34116 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/tests/chart/test_data.py
+-rw-r--r--   0 andy      (1000) andy      (1000)    26214 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/tests/chart/test_datalabel.py
+-rw-r--r--   0 andy      (1000) andy      (1000)     6797 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/tests/chart/test_legend.py
+-rw-r--r--   0 andy      (1000) andy      (1000)     4827 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/tests/chart/test_marker.py
+-rw-r--r--   0 andy      (1000) andy      (1000)    18769 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/tests/chart/test_plot.py
+-rw-r--r--   0 andy      (1000) andy      (1000)     7659 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/tests/chart/test_point.py
+-rw-r--r--   0 andy      (1000) andy      (1000)    19055 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/tests/chart/test_series.py
+-rw-r--r--   0 andy      (1000) andy      (1000)    15936 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/tests/chart/test_xlsx.py
+-rw-r--r--   0 andy      (1000) andy      (1000)    28442 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/tests/chart/test_xmlwriter.py
+drwxr-xr-x   0 andy      (1000) andy      (1000)        0 2023-05-18 16:21:08.230555 python-pptx-valutico-0.6.24.3/tests/dml/
+-rw-r--r--   0 andy      (1000) andy      (1000)        0 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/tests/dml/__init__.py
+-rw-r--r--   0 andy      (1000) andy      (1000)     3235 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/tests/dml/test_chtfmt.py
+-rw-r--r--   0 andy      (1000) andy      (1000)    11638 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/tests/dml/test_color.py
+-rw-r--r--   0 andy      (1000) andy      (1000)     1923 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/tests/dml/test_effect.py
+-rw-r--r--   0 andy      (1000) andy      (1000)    25636 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/tests/dml/test_fill.py
+-rw-r--r--   0 andy      (1000) andy      (1000)     5963 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/tests/dml/test_line.py
+drwxr-xr-x   0 andy      (1000) andy      (1000)        0 2023-05-18 16:21:08.230555 python-pptx-valutico-0.6.24.3/tests/opc/
+-rw-r--r--   0 andy      (1000) andy      (1000)        0 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/tests/opc/__init__.py
+-rw-r--r--   0 andy      (1000) andy      (1000)     6460 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/tests/opc/test_oxml.py
+-rw-r--r--   0 andy      (1000) andy      (1000)    38342 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/tests/opc/test_package.py
+-rw-r--r--   0 andy      (1000) andy      (1000)     2976 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/tests/opc/test_packuri.py
+-rw-r--r--   0 andy      (1000) andy      (1000)    14807 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/tests/opc/test_serialized.py
+drwxr-xr-x   0 andy      (1000) andy      (1000)        0 2023-05-18 16:21:08.230555 python-pptx-valutico-0.6.24.3/tests/opc/unitdata/
+-rw-r--r--   0 andy      (1000) andy      (1000)        0 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/tests/opc/unitdata/__init__.py
+-rw-r--r--   0 andy      (1000) andy      (1000)     7480 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/tests/opc/unitdata/rels.py
+drwxr-xr-x   0 andy      (1000) andy      (1000)        0 2023-05-18 16:21:08.230555 python-pptx-valutico-0.6.24.3/tests/oxml/
+-rw-r--r--   0 andy      (1000) andy      (1000)        0 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/tests/oxml/__init__.py
+drwxr-xr-x   0 andy      (1000) andy      (1000)        0 2023-05-18 16:21:08.230555 python-pptx-valutico-0.6.24.3/tests/oxml/shapes/
+-rw-r--r--   0 andy      (1000) andy      (1000)        0 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/tests/oxml/shapes/__init__.py
+-rw-r--r--   0 andy      (1000) andy      (1000)    10011 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/tests/oxml/shapes/test_autoshape.py
+-rw-r--r--   0 andy      (1000) andy      (1000)     3383 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/tests/oxml/shapes/test_graphfrm.py
+-rw-r--r--   0 andy      (1000) andy      (1000)    10820 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/tests/oxml/shapes/test_groupshape.py
+-rw-r--r--   0 andy      (1000) andy      (1000)     3591 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/tests/oxml/shapes/test_picture.py
+-rw-r--r--   0 andy      (1000) andy      (1000)     3204 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/tests/oxml/test___init__.py
+-rw-r--r--   0 andy      (1000) andy      (1000)     5059 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/tests/oxml/test_dml.py
+-rw-r--r--   0 andy      (1000) andy      (1000)     2669 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/tests/oxml/test_ns.py
+-rw-r--r--   0 andy      (1000) andy      (1000)     1436 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/tests/oxml/test_presentation.py
+-rw-r--r--   0 andy      (1000) andy      (1000)     8990 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/tests/oxml/test_simpletypes.py
+-rw-r--r--   0 andy      (1000) andy      (1000)      719 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/tests/oxml/test_slide.py
+-rw-r--r--   0 andy      (1000) andy      (1000)    10125 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/tests/oxml/test_table.py
+-rw-r--r--   0 andy      (1000) andy      (1000)      693 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/tests/oxml/test_theme.py
+-rw-r--r--   0 andy      (1000) andy      (1000)    20871 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/tests/oxml/test_xmlchemy.py
+drwxr-xr-x   0 andy      (1000) andy      (1000)        0 2023-05-18 16:21:08.230555 python-pptx-valutico-0.6.24.3/tests/oxml/unitdata/
+-rw-r--r--   0 andy      (1000) andy      (1000)        0 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/tests/oxml/unitdata/__init__.py
+-rw-r--r--   0 andy      (1000) andy      (1000)     1946 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/tests/oxml/unitdata/dml.py
+-rw-r--r--   0 andy      (1000) andy      (1000)     4060 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/tests/oxml/unitdata/shape.py
+-rw-r--r--   0 andy      (1000) andy      (1000)     1792 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/tests/oxml/unitdata/text.py
+drwxr-xr-x   0 andy      (1000) andy      (1000)        0 2023-05-18 16:21:08.230555 python-pptx-valutico-0.6.24.3/tests/parts/
+-rw-r--r--   0 andy      (1000) andy      (1000)        0 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/tests/parts/__init__.py
+-rw-r--r--   0 andy      (1000) andy      (1000)     5973 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/tests/parts/test_chart.py
+-rw-r--r--   0 andy      (1000) andy      (1000)     9096 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/tests/parts/test_coreprops.py
+-rw-r--r--   0 andy      (1000) andy      (1000)     3007 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/tests/parts/test_embeddedpackage.py
+-rw-r--r--   0 andy      (1000) andy      (1000)     7799 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/tests/parts/test_image.py
+-rw-r--r--   0 andy      (1000) andy      (1000)     1185 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/tests/parts/test_media.py
+-rw-r--r--   0 andy      (1000) andy      (1000)     9156 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/tests/parts/test_presentation.py
+-rw-r--r--   0 andy      (1000) andy      (1000)    22548 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/tests/parts/test_slide.py
+drwxr-xr-x   0 andy      (1000) andy      (1000)        0 2023-05-18 16:21:08.240555 python-pptx-valutico-0.6.24.3/tests/shapes/
+-rw-r--r--   0 andy      (1000) andy      (1000)        0 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/tests/shapes/__init__.py
+-rw-r--r--   0 andy      (1000) andy      (1000)    18645 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/tests/shapes/test_autoshape.py
+-rw-r--r--   0 andy      (1000) andy      (1000)    19691 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/tests/shapes/test_base.py
+-rw-r--r--   0 andy      (1000) andy      (1000)    16235 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/tests/shapes/test_connector.py
+-rw-r--r--   0 andy      (1000) andy      (1000)    20589 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/tests/shapes/test_freeform.py
+-rw-r--r--   0 andy      (1000) andy      (1000)     6651 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/tests/shapes/test_graphfrm.py
+-rw-r--r--   0 andy      (1000) andy      (1000)     2360 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/tests/shapes/test_group.py
+-rw-r--r--   0 andy      (1000) andy      (1000)    10621 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/tests/shapes/test_picture.py
+-rw-r--r--   0 andy      (1000) andy      (1000)    22431 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/tests/shapes/test_placeholder.py
+-rw-r--r--   0 andy      (1000) andy      (1000)    87112 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/tests/shapes/test_shapetree.py
+-rw-r--r--   0 andy      (1000) andy      (1000)    13970 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/tests/test_action.py
+-rw-r--r--   0 andy      (1000) andy      (1000)     1527 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/tests/test_api.py
+-rw-r--r--   0 andy      (1000) andy      (1000)     3739 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/tests/test_enum.py
+drwxr-xr-x   0 andy      (1000) andy      (1000)        0 2023-05-18 16:21:08.240555 python-pptx-valutico-0.6.24.3/tests/test_files/
+-rw-r--r--   0 andy      (1000) andy      (1000)   867288 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/tests/test_files/calibriz.ttf
+-rwxr-xr-x   0 andy      (1000) andy      (1000)    21818 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/tests/test_files/cdw-logo.eps
+-rw-r--r--   0 andy      (1000) andy      (1000)       42 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/tests/test_files/dummy.mp4
+drwxr-xr-x   0 andy      (1000) andy      (1000)        0 2023-05-18 16:21:08.240555 python-pptx-valutico-0.6.24.3/tests/test_files/expanded_pptx/
+-rw-r--r--   0 andy      (1000) andy      (1000)     3359 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/tests/test_files/expanded_pptx/[Content_Types].xml
+drwxr-xr-x   0 andy      (1000) andy      (1000)        0 2023-05-18 16:21:08.240555 python-pptx-valutico-0.6.24.3/tests/test_files/expanded_pptx/_rels/
+-rw-r--r--   0 andy      (1000) andy      (1000)      758 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/tests/test_files/expanded_pptx/_rels/.rels
+drwxr-xr-x   0 andy      (1000) andy      (1000)        0 2023-05-18 16:21:08.240555 python-pptx-valutico-0.6.24.3/tests/test_files/expanded_pptx/docProps/
+-rw-r--r--   0 andy      (1000) andy      (1000)     1354 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/tests/test_files/expanded_pptx/docProps/app.xml
+-rw-r--r--   0 andy      (1000) andy      (1000)      750 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/tests/test_files/expanded_pptx/docProps/core.xml
+-rw-r--r--   0 andy      (1000) andy      (1000)     8147 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/tests/test_files/expanded_pptx/docProps/thumbnail.jpeg
+drwxr-xr-x   0 andy      (1000) andy      (1000)        0 2023-05-18 16:21:08.240555 python-pptx-valutico-0.6.24.3/tests/test_files/expanded_pptx/ppt/
+drwxr-xr-x   0 andy      (1000) andy      (1000)        0 2023-05-18 16:21:08.240555 python-pptx-valutico-0.6.24.3/tests/test_files/expanded_pptx/ppt/_rels/
+-rw-r--r--   0 andy      (1000) andy      (1000)     1170 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/tests/test_files/expanded_pptx/ppt/_rels/presentation.xml.rels
+-rw-r--r--   0 andy      (1000) andy      (1000)      327 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/tests/test_files/expanded_pptx/ppt/presProps.xml
+-rw-r--r--   0 andy      (1000) andy      (1000)     4157 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/tests/test_files/expanded_pptx/ppt/presentation.xml
+drwxr-xr-x   0 andy      (1000) andy      (1000)        0 2023-05-18 16:21:08.240555 python-pptx-valutico-0.6.24.3/tests/test_files/expanded_pptx/ppt/printerSettings/
+-rw-r--r--   0 andy      (1000) andy      (1000)     9395 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/tests/test_files/expanded_pptx/ppt/printerSettings/printerSettings1.bin
+drwxr-xr-x   0 andy      (1000) andy      (1000)        0 2023-05-18 16:21:08.240555 python-pptx-valutico-0.6.24.3/tests/test_files/expanded_pptx/ppt/slideLayouts/
+drwxr-xr-x   0 andy      (1000) andy      (1000)        0 2023-05-18 16:21:08.240555 python-pptx-valutico-0.6.24.3/tests/test_files/expanded_pptx/ppt/slideLayouts/_rels/
+-rw-r--r--   0 andy      (1000) andy      (1000)      319 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/tests/test_files/expanded_pptx/ppt/slideLayouts/_rels/slideLayout1.xml.rels
+-rw-r--r--   0 andy      (1000) andy      (1000)      319 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/tests/test_files/expanded_pptx/ppt/slideLayouts/_rels/slideLayout10.xml.rels
+-rw-r--r--   0 andy      (1000) andy      (1000)      319 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/tests/test_files/expanded_pptx/ppt/slideLayouts/_rels/slideLayout11.xml.rels
+-rw-r--r--   0 andy      (1000) andy      (1000)      319 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/tests/test_files/expanded_pptx/ppt/slideLayouts/_rels/slideLayout2.xml.rels
+-rw-r--r--   0 andy      (1000) andy      (1000)      319 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/tests/test_files/expanded_pptx/ppt/slideLayouts/_rels/slideLayout3.xml.rels
+-rw-r--r--   0 andy      (1000) andy      (1000)      319 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/tests/test_files/expanded_pptx/ppt/slideLayouts/_rels/slideLayout4.xml.rels
+-rw-r--r--   0 andy      (1000) andy      (1000)      319 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/tests/test_files/expanded_pptx/ppt/slideLayouts/_rels/slideLayout5.xml.rels
+-rw-r--r--   0 andy      (1000) andy      (1000)      319 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/tests/test_files/expanded_pptx/ppt/slideLayouts/_rels/slideLayout6.xml.rels
+-rw-r--r--   0 andy      (1000) andy      (1000)      319 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/tests/test_files/expanded_pptx/ppt/slideLayouts/_rels/slideLayout7.xml.rels
+-rw-r--r--   0 andy      (1000) andy      (1000)      319 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/tests/test_files/expanded_pptx/ppt/slideLayouts/_rels/slideLayout8.xml.rels
+-rw-r--r--   0 andy      (1000) andy      (1000)      319 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/tests/test_files/expanded_pptx/ppt/slideLayouts/_rels/slideLayout9.xml.rels
+-rw-r--r--   0 andy      (1000) andy      (1000)     7473 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/tests/test_files/expanded_pptx/ppt/slideLayouts/slideLayout1.xml
+-rw-r--r--   0 andy      (1000) andy      (1000)     4783 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/tests/test_files/expanded_pptx/ppt/slideLayouts/slideLayout10.xml
+-rw-r--r--   0 andy      (1000) andy      (1000)     5131 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/tests/test_files/expanded_pptx/ppt/slideLayouts/slideLayout11.xml
+-rw-r--r--   0 andy      (1000) andy      (1000)     4786 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/tests/test_files/expanded_pptx/ppt/slideLayouts/slideLayout2.xml
+-rw-r--r--   0 andy      (1000) andy      (1000)     7613 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/tests/test_files/expanded_pptx/ppt/slideLayouts/slideLayout3.xml
+-rw-r--r--   0 andy      (1000) andy      (1000)     8154 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/tests/test_files/expanded_pptx/ppt/slideLayouts/slideLayout4.xml
+-rw-r--r--   0 andy      (1000) andy      (1000)    12501 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/tests/test_files/expanded_pptx/ppt/slideLayouts/slideLayout5.xml
+-rw-r--r--   0 andy      (1000) andy      (1000)     3371 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/tests/test_files/expanded_pptx/ppt/slideLayouts/slideLayout6.xml
+-rw-r--r--   0 andy      (1000) andy      (1000)     2757 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/tests/test_files/expanded_pptx/ppt/slideLayouts/slideLayout7.xml
+-rw-r--r--   0 andy      (1000) andy      (1000)     8100 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/tests/test_files/expanded_pptx/ppt/slideLayouts/slideLayout8.xml
+-rw-r--r--   0 andy      (1000) andy      (1000)     7633 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/tests/test_files/expanded_pptx/ppt/slideLayouts/slideLayout9.xml
+drwxr-xr-x   0 andy      (1000) andy      (1000)        0 2023-05-18 16:21:08.240555 python-pptx-valutico-0.6.24.3/tests/test_files/expanded_pptx/ppt/slideMasters/
+drwxr-xr-x   0 andy      (1000) andy      (1000)        0 2023-05-18 16:21:08.240555 python-pptx-valutico-0.6.24.3/tests/test_files/expanded_pptx/ppt/slideMasters/_rels/
+-rw-r--r--   0 andy      (1000) andy      (1000)     2093 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/tests/test_files/expanded_pptx/ppt/slideMasters/_rels/slideMaster1.xml.rels
+-rw-r--r--   0 andy      (1000) andy      (1000)    17871 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/tests/test_files/expanded_pptx/ppt/slideMasters/slideMaster1.xml
+drwxr-xr-x   0 andy      (1000) andy      (1000)        0 2023-05-18 16:21:08.240555 python-pptx-valutico-0.6.24.3/tests/test_files/expanded_pptx/ppt/slides/
+drwxr-xr-x   0 andy      (1000) andy      (1000)        0 2023-05-18 16:21:08.240555 python-pptx-valutico-0.6.24.3/tests/test_files/expanded_pptx/ppt/slides/_rels/
+-rw-r--r--   0 andy      (1000) andy      (1000)      315 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/tests/test_files/expanded_pptx/ppt/slides/_rels/slide1.xml.rels
+-rw-r--r--   0 andy      (1000) andy      (1000)     2198 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/tests/test_files/expanded_pptx/ppt/slides/slide1.xml
+-rw-r--r--   0 andy      (1000) andy      (1000)      182 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/tests/test_files/expanded_pptx/ppt/tableStyles.xml
+drwxr-xr-x   0 andy      (1000) andy      (1000)        0 2023-05-18 16:21:08.240555 python-pptx-valutico-0.6.24.3/tests/test_files/expanded_pptx/ppt/theme/
+-rw-r--r--   0 andy      (1000) andy      (1000)    10294 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/tests/test_files/expanded_pptx/ppt/theme/theme1.xml
+-rw-r--r--   0 andy      (1000) andy      (1000)     1081 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/tests/test_files/expanded_pptx/ppt/viewProps.xml
+-rw-r--r--   0 andy      (1000) andy      (1000)    15802 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/tests/test_files/minimal.pptx
+-rw-r--r--   0 andy      (1000) andy      (1000)      477 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/tests/test_files/minimal_slide.xml
+-rw-r--r--   0 andy      (1000) andy      (1000)    32944 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/tests/test_files/missing_rels_item.pptx
+-rw-r--r--   0 andy      (1000) andy      (1000)    64276 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/tests/test_files/monty-truth.png
+-rw-r--r--   0 andy      (1000) andy      (1000)    34436 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/tests/test_files/no-core-props.pptx
+-rw-r--r--   0 andy      (1000) andy      (1000)    34036 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/tests/test_files/no-slides.pptx
+-rw-r--r--   0 andy      (1000) andy      (1000)     4157 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/tests/test_files/presentation.xml
+-rw-r--r--   0 andy      (1000) andy      (1000)     3277 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/tests/test_files/python-icon.jpeg
+-rw-r--r--   0 andy      (1000) andy      (1000)     6111 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/tests/test_files/python-powered.png
+-rw-r--r--   0 andy      (1000) andy      (1000)    45210 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/tests/test_files/python.bmp
+-rw-r--r--   0 andy      (1000) andy      (1000)     8134 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/tests/test_files/slideLayout1.xml
+drwxr-xr-x   0 andy      (1000) andy      (1000)        0 2023-05-18 16:21:08.250555 python-pptx-valutico-0.6.24.3/tests/test_files/snippets/
+-rw-r--r--   0 andy      (1000) andy      (1000)     4920 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/tests/test_files/snippets/2x2-area-date.txt
+-rw-r--r--   0 andy      (1000) andy      (1000)     4916 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/tests/test_files/snippets/2x2-area-float.txt
+-rw-r--r--   0 andy      (1000) andy      (1000)     4816 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/tests/test_files/snippets/2x2-area-stacked-100.txt
+-rw-r--r--   0 andy      (1000) andy      (1000)     4809 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/tests/test_files/snippets/2x2-area-stacked.txt
+-rw-r--r--   0 andy      (1000) andy      (1000)     4810 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/tests/test_files/snippets/2x2-area.txt
+-rw-r--r--   0 andy      (1000) andy      (1000)     4308 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/tests/test_files/snippets/2x2-bar-clustered-date.txt
+-rw-r--r--   0 andy      (1000) andy      (1000)     4246 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/tests/test_files/snippets/2x2-bar-clustered-float.txt
+-rw-r--r--   0 andy      (1000) andy      (1000)     4140 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/tests/test_files/snippets/2x2-bar-clustered.txt
+-rw-r--r--   0 andy      (1000) andy      (1000)     4176 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/tests/test_files/snippets/2x2-bar-stacked-100.txt
+-rw-r--r--   0 andy      (1000) andy      (1000)     4169 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/tests/test_files/snippets/2x2-bar-stacked.txt
+-rw-r--r--   0 andy      (1000) andy      (1000)     4140 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/tests/test_files/snippets/2x2-column-clustered.txt
+-rw-r--r--   0 andy      (1000) andy      (1000)     4176 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/tests/test_files/snippets/2x2-column-stacked-100.txt
+-rw-r--r--   0 andy      (1000) andy      (1000)     4169 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/tests/test_files/snippets/2x2-column-stacked.txt
+-rw-r--r--   0 andy      (1000) andy      (1000)     4745 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/tests/test_files/snippets/2x2-line-date.txt
+-rw-r--r--   0 andy      (1000) andy      (1000)     4683 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/tests/test_files/snippets/2x2-line-float.txt
+-rw-r--r--   0 andy      (1000) andy      (1000)     4427 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/tests/test_files/snippets/2x2-line-markers-stacked-100.txt
+-rw-r--r--   0 andy      (1000) andy      (1000)     4420 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/tests/test_files/snippets/2x2-line-markers-stacked.txt
+-rw-r--r--   0 andy      (1000) andy      (1000)     4421 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/tests/test_files/snippets/2x2-line-markers.txt
+-rw-r--r--   0 andy      (1000) andy      (1000)     4583 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/tests/test_files/snippets/2x2-line-stacked-100.txt
+-rw-r--r--   0 andy      (1000) andy      (1000)     4576 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/tests/test_files/snippets/2x2-line-stacked.txt
+-rw-r--r--   0 andy      (1000) andy      (1000)     4577 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/tests/test_files/snippets/2x2-line.txt
+-rw-r--r--   0 andy      (1000) andy      (1000)     6440 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/tests/test_files/snippets/2x3-bubble-3d.txt
+-rw-r--r--   0 andy      (1000) andy      (1000)     6440 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/tests/test_files/snippets/2x3-bubble.txt
+-rw-r--r--   0 andy      (1000) andy      (1000)     5082 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/tests/test_files/snippets/2x3-xy-lines-no-markers.txt
+-rw-r--r--   0 andy      (1000) andy      (1000)     4926 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/tests/test_files/snippets/2x3-xy-lines.txt
+-rw-r--r--   0 andy      (1000) andy      (1000)     5084 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/tests/test_files/snippets/2x3-xy-smooth-no-markers.txt
+-rw-r--r--   0 andy      (1000) andy      (1000)     4928 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/tests/test_files/snippets/2x3-xy-smooth.txt
+-rw-r--r--   0 andy      (1000) andy      (1000)     5154 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/tests/test_files/snippets/2x3-xy.txt
+-rw-r--r--   0 andy      (1000) andy      (1000)     6102 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/tests/test_files/snippets/2x5-radar.txt
+-rw-r--r--   0 andy      (1000) andy      (1000)     2107 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/tests/test_files/snippets/3x1-pie-exploded.txt
+-rw-r--r--   0 andy      (1000) andy      (1000)     2073 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/tests/test_files/snippets/3x1-pie.txt
+-rw-r--r--   0 andy      (1000) andy      (1000)     4141 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/tests/test_files/snippets/3x2-doughnut-exploded.txt
+-rw-r--r--   0 andy      (1000) andy      (1000)     4073 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/tests/test_files/snippets/3x2-doughnut.txt
+-rw-r--r--   0 andy      (1000) andy      (1000)     5336 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/tests/test_files/snippets/4x2-multi-cat-bar.txt
+-rw-r--r--   0 andy      (1000) andy      (1000)     3458 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/tests/test_files/snippets/adjust-ser-count.txt
+-rw-r--r--   0 andy      (1000) andy      (1000)     3636 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/tests/test_files/snippets/cat-labels.txt
+-rw-r--r--   0 andy      (1000) andy      (1000)      517 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/tests/test_files/snippets/content-types-xml.txt
+-rw-r--r--   0 andy      (1000) andy      (1000)      666 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/tests/test_files/snippets/default-notes.txt
+-rw-r--r--   0 andy      (1000) andy      (1000)    11062 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/tests/test_files/snippets/default-notesMaster.txt
+-rw-r--r--   0 andy      (1000) andy      (1000)    10896 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/tests/test_files/snippets/default-theme.txt
+-rw-r--r--   0 andy      (1000) andy      (1000)     1087 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/tests/test_files/snippets/freeform.txt
+-rw-r--r--   0 andy      (1000) andy      (1000)      757 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/tests/test_files/snippets/package-rels-xml.txt
+-rw-r--r--   0 andy      (1000) andy      (1000)     1763 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/tests/test_files/snippets/placeholders.txt
+-rw-r--r--   0 andy      (1000) andy      (1000)      600 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/tests/test_files/snippets/presentation-rels-xml.txt
+-rw-r--r--   0 andy      (1000) andy      (1000)      445 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/tests/test_files/snippets/relationships.txt
+-rw-r--r--   0 andy      (1000) andy      (1000)      622 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/tests/test_files/snippets/rels-load-from-xml.txt
+-rw-r--r--   0 andy      (1000) andy      (1000)    10545 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/tests/test_files/snippets/rewrite-ser.txt
+-rw-r--r--   0 andy      (1000) andy      (1000)     2792 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/tests/test_files/snippets/timing.txt
+-rw-r--r--   0 andy      (1000) andy      (1000)    37859 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/tests/test_files/test.pptx
+-rw-r--r--   0 andy      (1000) andy      (1000)    38616 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/tests/test_files/test_slides.pptx
+-rw-r--r--   0 andy      (1000) andy      (1000)     4604 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/tests/test_media.py
+-rw-r--r--   0 andy      (1000) andy      (1000)    13510 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/tests/test_package.py
+-rw-r--r--   0 andy      (1000) andy      (1000)     8925 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/tests/test_presentation.py
+-rw-r--r--   0 andy      (1000) andy      (1000)     2455 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/tests/test_shared.py
+-rw-r--r--   0 andy      (1000) andy      (1000)    39126 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/tests/test_slide.py
+-rw-r--r--   0 andy      (1000) andy      (1000)    29166 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/tests/test_table.py
+-rw-r--r--   0 andy      (1000) andy      (1000)     1878 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/tests/test_util.py
+drwxr-xr-x   0 andy      (1000) andy      (1000)        0 2023-05-18 16:21:08.250555 python-pptx-valutico-0.6.24.3/tests/text/
+-rw-r--r--   0 andy      (1000) andy      (1000)        0 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/tests/text/__init__.py
+-rw-r--r--   0 andy      (1000) andy      (1000)    25213 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/tests/text/test_fonts.py
+-rw-r--r--   0 andy      (1000) andy      (1000)     9012 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/tests/text/test_layout.py
+-rw-r--r--   0 andy      (1000) andy      (1000)    45716 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/tests/text/test_text.py
+-rw-r--r--   0 andy      (1000) andy      (1000)     3661 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/tests/unitdata.py
+drwxr-xr-x   0 andy      (1000) andy      (1000)        0 2023-05-18 16:21:08.250555 python-pptx-valutico-0.6.24.3/tests/unitutil/
+-rw-r--r--   0 andy      (1000) andy      (1000)      247 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/tests/unitutil/__init__.py
+-rw-r--r--   0 andy      (1000) andy      (1000)     8312 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/tests/unitutil/cxml.py
+-rw-r--r--   0 andy      (1000) andy      (1000)     1855 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/tests/unitutil/file.py
+-rw-r--r--   0 andy      (1000) andy      (1000)     4129 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/tests/unitutil/mock.py
+-rw-r--r--   0 andy      (1000) andy      (1000)      652 2022-07-11 13:34:46.000000 python-pptx-valutico-0.6.24.3/tox.ini
```

### Comparing `python-pptx-valutico-0.6.24.2/HISTORY.rst` & `python-pptx-valutico-0.6.24.3/HISTORY.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,15 @@
 .. :changelog:
 
 Release History
 ---------------
+0.6.24.3 (2023-05-18)
++++++++++++++++++++
+
+- Fix issue with broken presentation after copy slide
 
 0.6.24.2 (2022-05-16)
 +++++++++++++++++++
 
 - Expand namespaces in ns.py to allow a wider variety of shapes to be used.
 
 0.6.21 (2021-09-20)
```

### Comparing `python-pptx-valutico-0.6.24.2/LICENSE` & `python-pptx-valutico-0.6.24.3/LICENSE`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/PKG-INFO` & `python-pptx-valutico-0.6.24.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-pptx-valutico
-Version: 0.6.24.2
+Version: 0.6.24.3
 Summary: Generate and manipulate Open XML PowerPoint (.pptx) files
 Home-page: https://github.com/AndreasSteiner/python-pptx
 Author: Andreas Steiner
 Author-email: a.steiner@valutico.ai
 License: MIT License
 Keywords: powerpoint ppt pptx office open xml
 Classifier: Development Status :: 4 - Beta
@@ -47,14 +47,18 @@
    https://python-pptx.readthedocs.org/en/latest/user/quickstart.html
 
 
 .. :changelog:
 
 Release History
 ---------------
+0.6.24.3 (2023-05-18)
++++++++++++++++++++
+
+- Fix issue with broken presentation after copy slide
 
 0.6.24.2 (2022-05-16)
 +++++++++++++++++++
 
 - Expand namespaces in ns.py to allow a wider variety of shapes to be used.
 
 0.6.21 (2021-09-20)
```

### Comparing `python-pptx-valutico-0.6.24.2/README.rst` & `python-pptx-valutico-0.6.24.3/README.rst`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/features/act-action.feature` & `python-pptx-valutico-0.6.24.3/features/act-action.feature`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/features/act-hyperlink.feature` & `python-pptx-valutico-0.6.24.3/features/act-hyperlink.feature`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/features/cht-axis-props.feature` & `python-pptx-valutico-0.6.24.3/features/cht-axis-props.feature`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/features/cht-axistitle-props.feature` & `python-pptx-valutico-0.6.24.3/features/cht-axistitle-props.feature`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/features/cht-category-access.feature` & `python-pptx-valutico-0.6.24.3/features/cht-category-access.feature`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/features/cht-category-props.feature` & `python-pptx-valutico-0.6.24.3/features/cht-category-props.feature`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/features/cht-chart.feature` & `python-pptx-valutico-0.6.24.3/features/cht-chart.feature`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/features/cht-charttitle-props.feature` & `python-pptx-valutico-0.6.24.3/features/cht-charttitle-props.feature`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/features/cht-data-props.feature` & `python-pptx-valutico-0.6.24.3/features/cht-data-props.feature`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/features/cht-datalabels.feature` & `python-pptx-valutico-0.6.24.3/features/cht-datalabels.feature`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/features/cht-legend-access.feature` & `python-pptx-valutico-0.6.24.3/features/cht-legend-access.feature`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/features/cht-legend-props.feature` & `python-pptx-valutico-0.6.24.3/features/cht-legend-props.feature`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/features/cht-marker-props.feature` & `python-pptx-valutico-0.6.24.3/features/cht-marker-props.feature`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/features/cht-plot-props.feature` & `python-pptx-valutico-0.6.24.3/features/cht-plot-props.feature`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/features/cht-point-access.feature` & `python-pptx-valutico-0.6.24.3/features/cht-point-access.feature`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/features/cht-point-props.feature` & `python-pptx-valutico-0.6.24.3/features/cht-point-props.feature`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/features/cht-replace-data.feature` & `python-pptx-valutico-0.6.24.3/features/cht-replace-data.feature`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/features/cht-series.feature` & `python-pptx-valutico-0.6.24.3/features/cht-series.feature`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/features/cht-ticklabels-props.feature` & `python-pptx-valutico-0.6.24.3/features/cht-ticklabels-props.feature`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/features/dml-color.feature` & `python-pptx-valutico-0.6.24.3/features/dml-color.feature`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/features/dml-effect.feature` & `python-pptx-valutico-0.6.24.3/features/dml-effect.feature`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/features/dml-fill.feature` & `python-pptx-valutico-0.6.24.3/features/dml-fill.feature`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/features/dml-line.feature` & `python-pptx-valutico-0.6.24.3/features/dml-line.feature`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/features/environment.py` & `python-pptx-valutico-0.6.24.3/features/environment.py`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/features/ph-inherit-props.feature` & `python-pptx-valutico-0.6.24.3/features/ph-inherit-props.feature`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/features/ph-insert-shape.feature` & `python-pptx-valutico-0.6.24.3/features/ph-insert-shape.feature`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/features/ph-phfmt-props.feature` & `python-pptx-valutico-0.6.24.3/features/ph-phfmt-props.feature`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/features/ph-placeholder-props.feature` & `python-pptx-valutico-0.6.24.3/features/ph-placeholder-props.feature`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/features/prs-coreprops.feature` & `python-pptx-valutico-0.6.24.3/features/prs-coreprops.feature`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/features/prs-open-save.feature` & `python-pptx-valutico-0.6.24.3/features/prs-open-save.feature`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/features/prs-presentation-props.feature` & `python-pptx-valutico-0.6.24.3/features/prs-presentation-props.feature`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/features/shp-autoshape.feature` & `python-pptx-valutico-0.6.24.3/features/shp-autoshape.feature`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/features/shp-connector.feature` & `python-pptx-valutico-0.6.24.3/features/shp-connector.feature`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/features/shp-freeform.feature` & `python-pptx-valutico-0.6.24.3/features/shp-freeform.feature`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/features/shp-graphicframe.feature` & `python-pptx-valutico-0.6.24.3/features/shp-graphicframe.feature`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/features/shp-groupshape.feature` & `python-pptx-valutico-0.6.24.3/features/shp-groupshape.feature`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/features/shp-movie-props.feature` & `python-pptx-valutico-0.6.24.3/features/shp-movie-props.feature`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/features/shp-picture.feature` & `python-pptx-valutico-0.6.24.3/features/shp-picture.feature`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/features/shp-placeholder.feature` & `python-pptx-valutico-0.6.24.3/features/shp-placeholder.feature`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/features/shp-shapes.feature` & `python-pptx-valutico-0.6.24.3/features/shp-shapes.feature`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/features/shp-shared.feature` & `python-pptx-valutico-0.6.24.3/features/shp-shared.feature`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/features/sld-slide.feature` & `python-pptx-valutico-0.6.24.3/features/sld-slide.feature`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/features/sld-slides.feature` & `python-pptx-valutico-0.6.24.3/features/sld-slides.feature`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/features/steps/action.py` & `python-pptx-valutico-0.6.24.3/features/steps/action.py`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/features/steps/axis.py` & `python-pptx-valutico-0.6.24.3/features/steps/axis.py`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/features/steps/background.py` & `python-pptx-valutico-0.6.24.3/features/steps/background.py`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/features/steps/category.py` & `python-pptx-valutico-0.6.24.3/features/steps/category.py`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/features/steps/chart.py` & `python-pptx-valutico-0.6.24.3/features/steps/chart.py`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/features/steps/chartdata.py` & `python-pptx-valutico-0.6.24.3/features/steps/chartdata.py`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/features/steps/color.py` & `python-pptx-valutico-0.6.24.3/features/steps/color.py`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/features/steps/coreprops.py` & `python-pptx-valutico-0.6.24.3/features/steps/coreprops.py`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/features/steps/datalabel.py` & `python-pptx-valutico-0.6.24.3/features/steps/datalabel.py`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/features/steps/effect.py` & `python-pptx-valutico-0.6.24.3/features/steps/effect.py`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/features/steps/fill.py` & `python-pptx-valutico-0.6.24.3/features/steps/fill.py`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/features/steps/font.py` & `python-pptx-valutico-0.6.24.3/features/steps/font.py`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/features/steps/font_color.py` & `python-pptx-valutico-0.6.24.3/features/steps/font_color.py`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/features/steps/helpers.py` & `python-pptx-valutico-0.6.24.3/features/steps/helpers.py`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/features/steps/legend.py` & `python-pptx-valutico-0.6.24.3/features/steps/legend.py`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/features/steps/line.py` & `python-pptx-valutico-0.6.24.3/features/steps/line.py`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/features/steps/picture.py` & `python-pptx-valutico-0.6.24.3/features/steps/picture.py`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/features/steps/placeholder.py` & `python-pptx-valutico-0.6.24.3/features/steps/placeholder.py`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/features/steps/plot.py` & `python-pptx-valutico-0.6.24.3/features/steps/plot.py`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/features/steps/presentation.py` & `python-pptx-valutico-0.6.24.3/features/steps/presentation.py`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/features/steps/series.py` & `python-pptx-valutico-0.6.24.3/features/steps/series.py`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/features/steps/shape.py` & `python-pptx-valutico-0.6.24.3/features/steps/shape.py`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/features/steps/shapes.py` & `python-pptx-valutico-0.6.24.3/features/steps/shapes.py`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/features/steps/slide.py` & `python-pptx-valutico-0.6.24.3/features/steps/slide.py`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/features/steps/slides.py` & `python-pptx-valutico-0.6.24.3/features/steps/slides.py`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/features/steps/table.py` & `python-pptx-valutico-0.6.24.3/features/steps/table.py`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/features/steps/test_files/72-dpi.tiff` & `python-pptx-valutico-0.6.24.3/features/steps/test_files/72-dpi.tiff`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/features/steps/test_files/CVS_LOGO.WMF` & `python-pptx-valutico-0.6.24.3/features/steps/test_files/CVS_LOGO.WMF`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/features/steps/test_files/act-props.pptm` & `python-pptx-valutico-0.6.24.3/features/steps/test_files/act-props.pptm`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/features/steps/test_files/calibriz.ttf` & `python-pptx-valutico-0.6.24.3/features/steps/test_files/calibriz.ttf`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/features/steps/test_files/cht-axis-props.pptx` & `python-pptx-valutico-0.6.24.3/features/steps/test_files/cht-axis-props.pptx`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/features/steps/test_files/cht-category-access.pptx` & `python-pptx-valutico-0.6.24.3/features/steps/test_files/cht-category-access.pptx`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/features/steps/test_files/cht-chart-props.pptx` & `python-pptx-valutico-0.6.24.3/features/steps/test_files/cht-chart-props.pptx`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/features/steps/test_files/cht-chart-type.pptx` & `python-pptx-valutico-0.6.24.3/features/steps/test_files/cht-chart-type.pptx`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/features/steps/test_files/cht-charts.pptx` & `python-pptx-valutico-0.6.24.3/features/steps/test_files/cht-charts.pptx`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/features/steps/test_files/cht-datalabels.pptx` & `python-pptx-valutico-0.6.24.3/features/steps/test_files/cht-datalabels.pptx`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/features/steps/test_files/cht-gridlines-props.pptx` & `python-pptx-valutico-0.6.24.3/features/steps/test_files/cht-gridlines-props.pptx`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/features/steps/test_files/cht-legend-props.pptx` & `python-pptx-valutico-0.6.24.3/features/steps/test_files/cht-legend-props.pptx`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/features/steps/test_files/cht-legend.pptx` & `python-pptx-valutico-0.6.24.3/features/steps/test_files/cht-legend.pptx`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/features/steps/test_files/cht-marker-props.pptx` & `python-pptx-valutico-0.6.24.3/features/steps/test_files/cht-marker-props.pptx`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/features/steps/test_files/cht-plot-props.pptx` & `python-pptx-valutico-0.6.24.3/features/steps/test_files/cht-plot-props.pptx`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/features/steps/test_files/cht-point-access.pptx` & `python-pptx-valutico-0.6.24.3/features/steps/test_files/cht-point-access.pptx`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/features/steps/test_files/cht-point-props.pptx` & `python-pptx-valutico-0.6.24.3/features/steps/test_files/cht-point-props.pptx`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/features/steps/test_files/cht-replace-data.pptx` & `python-pptx-valutico-0.6.24.3/features/steps/test_files/cht-replace-data.pptx`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/features/steps/test_files/cht-series.pptx` & `python-pptx-valutico-0.6.24.3/features/steps/test_files/cht-series.pptx`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/features/steps/test_files/cht-ticklabels-props.pptx` & `python-pptx-valutico-0.6.24.3/features/steps/test_files/cht-ticklabels-props.pptx`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/features/steps/test_files/dml-effect.pptx` & `python-pptx-valutico-0.6.24.3/features/steps/test_files/dml-effect.pptx`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/features/steps/test_files/dml-fill.pptx` & `python-pptx-valutico-0.6.24.3/features/steps/test_files/dml-fill.pptx`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/features/steps/test_files/dml-line.pptx` & `python-pptx-valutico-0.6.24.3/features/steps/test_files/dml-line.pptx`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/features/steps/test_files/ext-rels.pptx` & `python-pptx-valutico-0.6.24.3/features/steps/test_files/ext-rels.pptx`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/features/steps/test_files/extracted-pptx/[Content_Types].xml` & `python-pptx-valutico-0.6.24.3/features/steps/test_files/extracted-pptx/[Content_Types].xml`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/features/steps/test_files/extracted-pptx/_rels/.rels` & `python-pptx-valutico-0.6.24.3/features/steps/test_files/extracted-pptx/_rels/.rels`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/features/steps/test_files/extracted-pptx/docProps/app.xml` & `python-pptx-valutico-0.6.24.3/features/steps/test_files/extracted-pptx/docProps/app.xml`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/features/steps/test_files/extracted-pptx/docProps/core.xml` & `python-pptx-valutico-0.6.24.3/features/steps/test_files/extracted-pptx/docProps/core.xml`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/features/steps/test_files/extracted-pptx/docProps/thumbnail.jpeg` & `python-pptx-valutico-0.6.24.3/features/steps/test_files/extracted-pptx/docProps/thumbnail.jpeg`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/features/steps/test_files/extracted-pptx/ppt/_rels/presentation.xml.rels` & `python-pptx-valutico-0.6.24.3/features/steps/test_files/extracted-pptx/ppt/_rels/presentation.xml.rels`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/features/steps/test_files/extracted-pptx/ppt/presProps.xml` & `python-pptx-valutico-0.6.24.3/features/steps/test_files/extracted-pptx/ppt/presProps.xml`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/features/steps/test_files/extracted-pptx/ppt/presentation.xml` & `python-pptx-valutico-0.6.24.3/features/steps/test_files/extracted-pptx/ppt/presentation.xml`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/features/steps/test_files/extracted-pptx/ppt/printerSettings/printerSettings1.bin` & `python-pptx-valutico-0.6.24.3/features/steps/test_files/extracted-pptx/ppt/printerSettings/printerSettings1.bin`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/features/steps/test_files/extracted-pptx/ppt/slideLayouts/slideLayout1.xml` & `python-pptx-valutico-0.6.24.3/features/steps/test_files/extracted-pptx/ppt/slideLayouts/slideLayout1.xml`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/features/steps/test_files/extracted-pptx/ppt/slideLayouts/slideLayout10.xml` & `python-pptx-valutico-0.6.24.3/features/steps/test_files/extracted-pptx/ppt/slideLayouts/slideLayout10.xml`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/features/steps/test_files/extracted-pptx/ppt/slideLayouts/slideLayout11.xml` & `python-pptx-valutico-0.6.24.3/features/steps/test_files/extracted-pptx/ppt/slideLayouts/slideLayout11.xml`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/features/steps/test_files/extracted-pptx/ppt/slideLayouts/slideLayout2.xml` & `python-pptx-valutico-0.6.24.3/features/steps/test_files/extracted-pptx/ppt/slideLayouts/slideLayout2.xml`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/features/steps/test_files/extracted-pptx/ppt/slideLayouts/slideLayout3.xml` & `python-pptx-valutico-0.6.24.3/features/steps/test_files/extracted-pptx/ppt/slideLayouts/slideLayout3.xml`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/features/steps/test_files/extracted-pptx/ppt/slideLayouts/slideLayout4.xml` & `python-pptx-valutico-0.6.24.3/features/steps/test_files/extracted-pptx/ppt/slideLayouts/slideLayout4.xml`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/features/steps/test_files/extracted-pptx/ppt/slideLayouts/slideLayout5.xml` & `python-pptx-valutico-0.6.24.3/features/steps/test_files/extracted-pptx/ppt/slideLayouts/slideLayout5.xml`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/features/steps/test_files/extracted-pptx/ppt/slideLayouts/slideLayout6.xml` & `python-pptx-valutico-0.6.24.3/features/steps/test_files/extracted-pptx/ppt/slideLayouts/slideLayout6.xml`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/features/steps/test_files/extracted-pptx/ppt/slideLayouts/slideLayout7.xml` & `python-pptx-valutico-0.6.24.3/features/steps/test_files/extracted-pptx/ppt/slideLayouts/slideLayout7.xml`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/features/steps/test_files/extracted-pptx/ppt/slideLayouts/slideLayout8.xml` & `python-pptx-valutico-0.6.24.3/features/steps/test_files/extracted-pptx/ppt/slideLayouts/slideLayout8.xml`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/features/steps/test_files/extracted-pptx/ppt/slideLayouts/slideLayout9.xml` & `python-pptx-valutico-0.6.24.3/features/steps/test_files/extracted-pptx/ppt/slideLayouts/slideLayout9.xml`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/features/steps/test_files/extracted-pptx/ppt/slideMasters/_rels/slideMaster1.xml.rels` & `python-pptx-valutico-0.6.24.3/features/steps/test_files/extracted-pptx/ppt/slideMasters/_rels/slideMaster1.xml.rels`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/features/steps/test_files/extracted-pptx/ppt/slideMasters/slideMaster1.xml` & `python-pptx-valutico-0.6.24.3/features/steps/test_files/extracted-pptx/ppt/slideMasters/slideMaster1.xml`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/features/steps/test_files/extracted-pptx/ppt/slides/slide1.xml` & `python-pptx-valutico-0.6.24.3/features/steps/test_files/extracted-pptx/ppt/slides/slide1.xml`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/features/steps/test_files/extracted-pptx/ppt/theme/theme1.xml` & `python-pptx-valutico-0.6.24.3/features/steps/test_files/extracted-pptx/ppt/theme/theme1.xml`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/features/steps/test_files/extracted-pptx/ppt/viewProps.xml` & `python-pptx-valutico-0.6.24.3/features/steps/test_files/extracted-pptx/ppt/viewProps.xml`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/features/steps/test_files/font-color.pptx` & `python-pptx-valutico-0.6.24.3/features/steps/test_files/font-color.pptx`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/features/steps/test_files/just-two-mice.mp4` & `python-pptx-valutico-0.6.24.3/features/steps/test_files/just-two-mice.mp4`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/features/steps/test_files/just-two-mice.png` & `python-pptx-valutico-0.6.24.3/features/steps/test_files/just-two-mice.png`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/features/steps/test_files/lyt-shapes.pptx` & `python-pptx-valutico-0.6.24.3/features/steps/test_files/lyt-shapes.pptx`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/features/steps/test_files/minimal.pptx` & `python-pptx-valutico-0.6.24.3/features/steps/test_files/minimal.pptx`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/features/steps/test_files/monty-truth.png` & `python-pptx-valutico-0.6.24.3/features/steps/test_files/monty-truth.png`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/features/steps/test_files/mst-placeholders.pptx` & `python-pptx-valutico-0.6.24.3/features/steps/test_files/mst-placeholders.pptx`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/features/steps/test_files/mst-shapes.pptx` & `python-pptx-valutico-0.6.24.3/features/steps/test_files/mst-shapes.pptx`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/features/steps/test_files/mst-slide-layouts.pptx` & `python-pptx-valutico-0.6.24.3/features/steps/test_files/mst-slide-layouts.pptx`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/features/steps/test_files/ph-inherit-props.pptx` & `python-pptx-valutico-0.6.24.3/features/steps/test_files/ph-inherit-props.pptx`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/features/steps/test_files/ph-populated-placeholders.pptx` & `python-pptx-valutico-0.6.24.3/features/steps/test_files/ph-populated-placeholders.pptx`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/features/steps/test_files/ph-unpopulated-placeholders.pptx` & `python-pptx-valutico-0.6.24.3/features/steps/test_files/ph-unpopulated-placeholders.pptx`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/features/steps/test_files/pic.emf` & `python-pptx-valutico-0.6.24.3/features/steps/test_files/pic.emf`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/features/steps/test_files/prs-add-slide.pptx` & `python-pptx-valutico-0.6.24.3/features/steps/test_files/prs-add-slide.pptx`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/features/steps/test_files/prs-notes.pptx` & `python-pptx-valutico-0.6.24.3/features/steps/test_files/prs-notes.pptx`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/features/steps/test_files/prs-properties.pptx` & `python-pptx-valutico-0.6.24.3/features/steps/test_files/prs-properties.pptx`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/features/steps/test_files/prs-slide-masters.pptx` & `python-pptx-valutico-0.6.24.3/features/steps/test_files/prs-slide-masters.pptx`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/features/steps/test_files/python-icon.jpeg` & `python-pptx-valutico-0.6.24.3/features/steps/test_files/python-icon.jpeg`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/features/steps/test_files/python-powered.png` & `python-pptx-valutico-0.6.24.3/features/steps/test_files/python-powered.png`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/features/steps/test_files/python.bmp` & `python-pptx-valutico-0.6.24.3/features/steps/test_files/python.bmp`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/features/steps/test_files/shp-access-chart.pptx` & `python-pptx-valutico-0.6.24.3/features/steps/test_files/shp-access-chart.pptx`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/features/steps/test_files/shp-access-ole-object.pptx` & `python-pptx-valutico-0.6.24.3/features/steps/test_files/shp-access-ole-object.pptx`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/features/steps/test_files/shp-autoshape-adjustments.pptx` & `python-pptx-valutico-0.6.24.3/features/steps/test_files/shp-autoshape-adjustments.pptx`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/features/steps/test_files/shp-autoshape-props.pptx` & `python-pptx-valutico-0.6.24.3/features/steps/test_files/shp-autoshape-props.pptx`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/features/steps/test_files/shp-common-props.pptx` & `python-pptx-valutico-0.6.24.3/features/steps/test_files/shp-common-props.pptx`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/features/steps/test_files/shp-connector-props.pptx` & `python-pptx-valutico-0.6.24.3/features/steps/test_files/shp-connector-props.pptx`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/features/steps/test_files/shp-embedded-docx.docx` & `python-pptx-valutico-0.6.24.3/features/steps/test_files/shp-embedded-docx.docx`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/features/steps/test_files/shp-embedded-pptx.pptx` & `python-pptx-valutico-0.6.24.3/features/steps/test_files/shp-embedded-pptx.pptx`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/features/steps/test_files/shp-embedded-xlsx.xlsx` & `python-pptx-valutico-0.6.24.3/features/steps/test_files/shp-embedded-xlsx.xlsx`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/features/steps/test_files/shp-freeform.pptx` & `python-pptx-valutico-0.6.24.3/features/steps/test_files/shp-freeform.pptx`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/features/steps/test_files/shp-groupshape.pptx` & `python-pptx-valutico-0.6.24.3/features/steps/test_files/shp-groupshape.pptx`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/features/steps/test_files/shp-movie-props.pptx` & `python-pptx-valutico-0.6.24.3/features/steps/test_files/shp-movie-props.pptx`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/features/steps/test_files/shp-picture.pptx` & `python-pptx-valutico-0.6.24.3/features/steps/test_files/shp-picture.pptx`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/features/steps/test_files/shp-pos-and-size.pptx` & `python-pptx-valutico-0.6.24.3/features/steps/test_files/shp-pos-and-size.pptx`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/features/steps/test_files/shp-shapes.pptx` & `python-pptx-valutico-0.6.24.3/features/steps/test_files/shp-shapes.pptx`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/features/steps/test_files/sld-background.pptx` & `python-pptx-valutico-0.6.24.3/features/steps/test_files/sld-background.pptx`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/features/steps/test_files/sld-blank.pptx` & `python-pptx-valutico-0.6.24.3/features/steps/test_files/sld-blank.pptx`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/features/steps/test_files/sld-notes.pptx` & `python-pptx-valutico-0.6.24.3/features/steps/test_files/sld-notes.pptx`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/features/steps/test_files/sld-slide.pptx` & `python-pptx-valutico-0.6.24.3/features/steps/test_files/sld-slide.pptx`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/features/steps/test_files/sld-slides.pptx` & `python-pptx-valutico-0.6.24.3/features/steps/test_files/sld-slides.pptx`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/features/steps/test_files/sonic.gif` & `python-pptx-valutico-0.6.24.3/features/steps/test_files/sonic.gif`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/features/steps/test_files/tbl-cell.pptx` & `python-pptx-valutico-0.6.24.3/features/steps/test_files/tbl-cell.pptx`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/features/steps/test_files/test.pptx` & `python-pptx-valutico-0.6.24.3/features/steps/test_files/test.pptx`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/features/steps/test_files/txt-fit-text.pptx` & `python-pptx-valutico-0.6.24.3/features/steps/test_files/txt-fit-text.pptx`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/features/steps/test_files/txt-font-props.pptx` & `python-pptx-valutico-0.6.24.3/features/steps/test_files/txt-font-props.pptx`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/features/steps/test_files/txt-font-typeface.pptx` & `python-pptx-valutico-0.6.24.3/features/steps/test_files/txt-font-typeface.pptx`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/features/steps/test_files/txt-paragraph-spacing.pptx` & `python-pptx-valutico-0.6.24.3/features/steps/test_files/txt-paragraph-spacing.pptx`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/features/steps/test_files/txt-text-frame.pptx` & `python-pptx-valutico-0.6.24.3/features/steps/test_files/txt-text-frame.pptx`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/features/steps/test_files/txt-text.pptx` & `python-pptx-valutico-0.6.24.3/features/steps/test_files/txt-text.pptx`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/features/steps/text.py` & `python-pptx-valutico-0.6.24.3/features/steps/text.py`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/features/steps/text_frame.py` & `python-pptx-valutico-0.6.24.3/features/steps/text_frame.py`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/features/tbl-cell.feature` & `python-pptx-valutico-0.6.24.3/features/tbl-cell.feature`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/features/tbl-table.feature` & `python-pptx-valutico-0.6.24.3/features/tbl-table.feature`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/features/txt-font-color.feature` & `python-pptx-valutico-0.6.24.3/features/txt-font-color.feature`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/features/txt-font-props.feature` & `python-pptx-valutico-0.6.24.3/features/txt-font-props.feature`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/features/txt-paragraph.feature` & `python-pptx-valutico-0.6.24.3/features/txt-paragraph.feature`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/features/txt-text.feature` & `python-pptx-valutico-0.6.24.3/features/txt-text.feature`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/features/txt-textframe.feature` & `python-pptx-valutico-0.6.24.3/features/txt-textframe.feature`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/pptx/__init__.py` & `python-pptx-valutico-0.6.24.3/pptx/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # encoding: utf-8
 
 """Initialization module for python-pptx package."""
 
-__version__ = "0.6.24.2"
+__version__ = "0.6.24.3"
 
 
 import sys
 
 import pptx.exc as exceptions
 
 sys.modules["pptx.exceptions"] = exceptions
```

### Comparing `python-pptx-valutico-0.6.24.2/pptx/action.py` & `python-pptx-valutico-0.6.24.3/pptx/action.py`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/pptx/api.py` & `python-pptx-valutico-0.6.24.3/pptx/api.py`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/pptx/chart/axis.py` & `python-pptx-valutico-0.6.24.3/pptx/chart/axis.py`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/pptx/chart/category.py` & `python-pptx-valutico-0.6.24.3/pptx/chart/category.py`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/pptx/chart/chart.py` & `python-pptx-valutico-0.6.24.3/pptx/chart/chart.py`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/pptx/chart/data.py` & `python-pptx-valutico-0.6.24.3/pptx/chart/data.py`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/pptx/chart/datalabel.py` & `python-pptx-valutico-0.6.24.3/pptx/chart/datalabel.py`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/pptx/chart/legend.py` & `python-pptx-valutico-0.6.24.3/pptx/chart/legend.py`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/pptx/chart/marker.py` & `python-pptx-valutico-0.6.24.3/pptx/chart/marker.py`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/pptx/chart/plot.py` & `python-pptx-valutico-0.6.24.3/pptx/chart/plot.py`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/pptx/chart/point.py` & `python-pptx-valutico-0.6.24.3/pptx/chart/point.py`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/pptx/chart/series.py` & `python-pptx-valutico-0.6.24.3/pptx/chart/series.py`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/pptx/chart/xlsx.py` & `python-pptx-valutico-0.6.24.3/pptx/chart/xlsx.py`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/pptx/chart/xmlwriter.py` & `python-pptx-valutico-0.6.24.3/pptx/chart/xmlwriter.py`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/pptx/compat/__init__.py` & `python-pptx-valutico-0.6.24.3/pptx/compat/__init__.py`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/pptx/compat/python2.py` & `python-pptx-valutico-0.6.24.3/pptx/compat/python2.py`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/pptx/compat/python3.py` & `python-pptx-valutico-0.6.24.3/pptx/compat/python3.py`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/pptx/dml/chtfmt.py` & `python-pptx-valutico-0.6.24.3/pptx/dml/chtfmt.py`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/pptx/dml/color.py` & `python-pptx-valutico-0.6.24.3/pptx/dml/color.py`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/pptx/dml/effect.py` & `python-pptx-valutico-0.6.24.3/pptx/dml/effect.py`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/pptx/dml/fill.py` & `python-pptx-valutico-0.6.24.3/pptx/dml/fill.py`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/pptx/dml/line.py` & `python-pptx-valutico-0.6.24.3/pptx/dml/line.py`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/pptx/enum/action.py` & `python-pptx-valutico-0.6.24.3/pptx/enum/action.py`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/pptx/enum/base.py` & `python-pptx-valutico-0.6.24.3/pptx/enum/base.py`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/pptx/enum/chart.py` & `python-pptx-valutico-0.6.24.3/pptx/enum/chart.py`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/pptx/enum/dml.py` & `python-pptx-valutico-0.6.24.3/pptx/enum/dml.py`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/pptx/enum/lang.py` & `python-pptx-valutico-0.6.24.3/pptx/enum/lang.py`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/pptx/enum/shapes.py` & `python-pptx-valutico-0.6.24.3/pptx/enum/shapes.py`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/pptx/enum/text.py` & `python-pptx-valutico-0.6.24.3/pptx/enum/text.py`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/pptx/media.py` & `python-pptx-valutico-0.6.24.3/pptx/media.py`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/pptx/opc/constants.py` & `python-pptx-valutico-0.6.24.3/pptx/opc/constants.py`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/pptx/opc/oxml.py` & `python-pptx-valutico-0.6.24.3/pptx/opc/oxml.py`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/pptx/opc/package.py` & `python-pptx-valutico-0.6.24.3/pptx/opc/package.py`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/pptx/opc/packuri.py` & `python-pptx-valutico-0.6.24.3/pptx/opc/packuri.py`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/pptx/opc/serialized.py` & `python-pptx-valutico-0.6.24.3/pptx/opc/serialized.py`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/pptx/opc/shared.py` & `python-pptx-valutico-0.6.24.3/pptx/opc/shared.py`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/pptx/opc/spec.py` & `python-pptx-valutico-0.6.24.3/pptx/opc/spec.py`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/pptx/oxml/__init__.py` & `python-pptx-valutico-0.6.24.3/pptx/oxml/__init__.py`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/pptx/oxml/action.py` & `python-pptx-valutico-0.6.24.3/pptx/oxml/action.py`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/pptx/oxml/chart/axis.py` & `python-pptx-valutico-0.6.24.3/pptx/oxml/chart/axis.py`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/pptx/oxml/chart/chart.py` & `python-pptx-valutico-0.6.24.3/pptx/oxml/chart/chart.py`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/pptx/oxml/chart/datalabel.py` & `python-pptx-valutico-0.6.24.3/pptx/oxml/chart/datalabel.py`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/pptx/oxml/chart/legend.py` & `python-pptx-valutico-0.6.24.3/pptx/oxml/chart/legend.py`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/pptx/oxml/chart/marker.py` & `python-pptx-valutico-0.6.24.3/pptx/oxml/chart/marker.py`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/pptx/oxml/chart/plot.py` & `python-pptx-valutico-0.6.24.3/pptx/oxml/chart/plot.py`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/pptx/oxml/chart/series.py` & `python-pptx-valutico-0.6.24.3/pptx/oxml/chart/series.py`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/pptx/oxml/chart/shared.py` & `python-pptx-valutico-0.6.24.3/pptx/oxml/chart/shared.py`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/pptx/oxml/coreprops.py` & `python-pptx-valutico-0.6.24.3/pptx/oxml/coreprops.py`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/pptx/oxml/dml/color.py` & `python-pptx-valutico-0.6.24.3/pptx/oxml/dml/color.py`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/pptx/oxml/dml/fill.py` & `python-pptx-valutico-0.6.24.3/pptx/oxml/dml/fill.py`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/pptx/oxml/ns.py` & `python-pptx-valutico-0.6.24.3/pptx/oxml/ns.py`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/pptx/oxml/presentation.py` & `python-pptx-valutico-0.6.24.3/pptx/oxml/presentation.py`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/pptx/oxml/shapes/autoshape.py` & `python-pptx-valutico-0.6.24.3/pptx/oxml/shapes/autoshape.py`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/pptx/oxml/shapes/connector.py` & `python-pptx-valutico-0.6.24.3/pptx/oxml/shapes/connector.py`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/pptx/oxml/shapes/graphfrm.py` & `python-pptx-valutico-0.6.24.3/pptx/oxml/shapes/graphfrm.py`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/pptx/oxml/shapes/groupshape.py` & `python-pptx-valutico-0.6.24.3/pptx/oxml/shapes/groupshape.py`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/pptx/oxml/shapes/picture.py` & `python-pptx-valutico-0.6.24.3/pptx/oxml/shapes/picture.py`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/pptx/oxml/shapes/shared.py` & `python-pptx-valutico-0.6.24.3/pptx/oxml/shapes/shared.py`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/pptx/oxml/simpletypes.py` & `python-pptx-valutico-0.6.24.3/pptx/oxml/simpletypes.py`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/pptx/oxml/slide.py` & `python-pptx-valutico-0.6.24.3/pptx/oxml/slide.py`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/pptx/oxml/table.py` & `python-pptx-valutico-0.6.24.3/pptx/oxml/table.py`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/pptx/oxml/text.py` & `python-pptx-valutico-0.6.24.3/pptx/oxml/text.py`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/pptx/oxml/theme.py` & `python-pptx-valutico-0.6.24.3/pptx/oxml/theme.py`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/pptx/oxml/xmlchemy.py` & `python-pptx-valutico-0.6.24.3/pptx/oxml/xmlchemy.py`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/pptx/package.py` & `python-pptx-valutico-0.6.24.3/pptx/package.py`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/pptx/parts/chart.py` & `python-pptx-valutico-0.6.24.3/pptx/parts/chart.py`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/pptx/parts/coreprops.py` & `python-pptx-valutico-0.6.24.3/pptx/parts/coreprops.py`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/pptx/parts/embeddedpackage.py` & `python-pptx-valutico-0.6.24.3/pptx/parts/embeddedpackage.py`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/pptx/parts/image.py` & `python-pptx-valutico-0.6.24.3/pptx/parts/image.py`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/pptx/parts/media.py` & `python-pptx-valutico-0.6.24.3/pptx/parts/media.py`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/pptx/parts/presentation.py` & `python-pptx-valutico-0.6.24.3/pptx/parts/presentation.py`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/pptx/parts/slide.py` & `python-pptx-valutico-0.6.24.3/pptx/parts/slide.py`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/pptx/presentation.py` & `python-pptx-valutico-0.6.24.3/pptx/presentation.py`

 * *Files 2% similar despite different names*

```diff
@@ -123,14 +123,12 @@
         # Copy shapes from source, in order
         for shape in source.shapes:
             new_shape = copy.deepcopy(shape.element)
             dest.shapes._spTree.insert_element_before(new_shape, "p:extLst")
         # Copy rels from source
         for rel in source.part.rels:
             _rels: _Relationships = dest.part.rels
-            if not rel.is_external:
-                _rels.get_or_add(rel.reltype, rel._target)
-            else:
+            if rel.is_external:
                 _rels.get_or_add_ext_rel(rel.reltype, rel._target)
         # Move appended slide into target_index
         self.slides.element.insert(target_index, self.slides.element[-1])
         return dest
```

### Comparing `python-pptx-valutico-0.6.24.2/pptx/shapes/__init__.py` & `python-pptx-valutico-0.6.24.3/pptx/shapes/__init__.py`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/pptx/shapes/autoshape.py` & `python-pptx-valutico-0.6.24.3/pptx/shapes/autoshape.py`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/pptx/shapes/base.py` & `python-pptx-valutico-0.6.24.3/pptx/shapes/base.py`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/pptx/shapes/connector.py` & `python-pptx-valutico-0.6.24.3/pptx/shapes/connector.py`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/pptx/shapes/freeform.py` & `python-pptx-valutico-0.6.24.3/pptx/shapes/freeform.py`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/pptx/shapes/graphfrm.py` & `python-pptx-valutico-0.6.24.3/pptx/shapes/graphfrm.py`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/pptx/shapes/group.py` & `python-pptx-valutico-0.6.24.3/pptx/shapes/group.py`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/pptx/shapes/picture.py` & `python-pptx-valutico-0.6.24.3/pptx/shapes/picture.py`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/pptx/shapes/placeholder.py` & `python-pptx-valutico-0.6.24.3/pptx/shapes/placeholder.py`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/pptx/shapes/shapetree.py` & `python-pptx-valutico-0.6.24.3/pptx/shapes/shapetree.py`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/pptx/shared.py` & `python-pptx-valutico-0.6.24.3/pptx/shared.py`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/pptx/slide.py` & `python-pptx-valutico-0.6.24.3/pptx/slide.py`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/pptx/spec.py` & `python-pptx-valutico-0.6.24.3/pptx/spec.py`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/pptx/table.py` & `python-pptx-valutico-0.6.24.3/pptx/table.py`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/pptx/templates/default.pptx` & `python-pptx-valutico-0.6.24.3/pptx/templates/default.pptx`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/pptx/templates/docx-icon.emf` & `python-pptx-valutico-0.6.24.3/pptx/templates/docx-icon.emf`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/pptx/templates/generic-icon.emf` & `python-pptx-valutico-0.6.24.3/pptx/templates/generic-icon.emf`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/pptx/templates/notes.xml` & `python-pptx-valutico-0.6.24.3/pptx/templates/notes.xml`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/pptx/templates/notesMaster.xml` & `python-pptx-valutico-0.6.24.3/pptx/templates/notesMaster.xml`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/pptx/templates/pptx-icon.emf` & `python-pptx-valutico-0.6.24.3/pptx/templates/pptx-icon.emf`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/pptx/templates/theme.xml` & `python-pptx-valutico-0.6.24.3/pptx/templates/theme.xml`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/pptx/templates/xlsx-icon.emf` & `python-pptx-valutico-0.6.24.3/pptx/templates/xlsx-icon.emf`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/pptx/text/fonts.py` & `python-pptx-valutico-0.6.24.3/pptx/text/fonts.py`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/pptx/text/layout.py` & `python-pptx-valutico-0.6.24.3/pptx/text/layout.py`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/pptx/text/text.py` & `python-pptx-valutico-0.6.24.3/pptx/text/text.py`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/pptx/util.py` & `python-pptx-valutico-0.6.24.3/pptx/util.py`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/python_pptx_valutico.egg-info/PKG-INFO` & `python-pptx-valutico-0.6.24.3/python_pptx_valutico.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-pptx-valutico
-Version: 0.6.24.2
+Version: 0.6.24.3
 Summary: Generate and manipulate Open XML PowerPoint (.pptx) files
 Home-page: https://github.com/AndreasSteiner/python-pptx
 Author: Andreas Steiner
 Author-email: a.steiner@valutico.ai
 License: MIT License
 Keywords: powerpoint ppt pptx office open xml
 Classifier: Development Status :: 4 - Beta
@@ -47,14 +47,18 @@
    https://python-pptx.readthedocs.org/en/latest/user/quickstart.html
 
 
 .. :changelog:
 
 Release History
 ---------------
+0.6.24.3 (2023-05-18)
++++++++++++++++++++
+
+- Fix issue with broken presentation after copy slide
 
 0.6.24.2 (2022-05-16)
 +++++++++++++++++++
 
 - Expand namespaces in ns.py to allow a wider variety of shapes to be used.
 
 0.6.21 (2021-09-20)
```

### Comparing `python-pptx-valutico-0.6.24.2/python_pptx_valutico.egg-info/SOURCES.txt` & `python-pptx-valutico-0.6.24.3/python_pptx_valutico.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/setup.py` & `python-pptx-valutico-0.6.24.3/setup.py`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/tests/chart/test_axis.py` & `python-pptx-valutico-0.6.24.3/tests/chart/test_axis.py`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/tests/chart/test_category.py` & `python-pptx-valutico-0.6.24.3/tests/chart/test_category.py`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/tests/chart/test_chart.py` & `python-pptx-valutico-0.6.24.3/tests/chart/test_chart.py`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/tests/chart/test_data.py` & `python-pptx-valutico-0.6.24.3/tests/chart/test_data.py`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/tests/chart/test_datalabel.py` & `python-pptx-valutico-0.6.24.3/tests/chart/test_datalabel.py`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/tests/chart/test_legend.py` & `python-pptx-valutico-0.6.24.3/tests/chart/test_legend.py`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/tests/chart/test_marker.py` & `python-pptx-valutico-0.6.24.3/tests/chart/test_marker.py`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/tests/chart/test_plot.py` & `python-pptx-valutico-0.6.24.3/tests/chart/test_plot.py`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/tests/chart/test_point.py` & `python-pptx-valutico-0.6.24.3/tests/chart/test_point.py`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/tests/chart/test_series.py` & `python-pptx-valutico-0.6.24.3/tests/chart/test_series.py`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/tests/chart/test_xlsx.py` & `python-pptx-valutico-0.6.24.3/tests/chart/test_xlsx.py`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/tests/chart/test_xmlwriter.py` & `python-pptx-valutico-0.6.24.3/tests/chart/test_xmlwriter.py`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/tests/dml/test_chtfmt.py` & `python-pptx-valutico-0.6.24.3/tests/dml/test_chtfmt.py`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/tests/dml/test_color.py` & `python-pptx-valutico-0.6.24.3/tests/dml/test_color.py`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/tests/dml/test_effect.py` & `python-pptx-valutico-0.6.24.3/tests/dml/test_effect.py`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/tests/dml/test_fill.py` & `python-pptx-valutico-0.6.24.3/tests/dml/test_fill.py`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/tests/dml/test_line.py` & `python-pptx-valutico-0.6.24.3/tests/dml/test_line.py`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/tests/opc/test_oxml.py` & `python-pptx-valutico-0.6.24.3/tests/opc/test_oxml.py`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/tests/opc/test_package.py` & `python-pptx-valutico-0.6.24.3/tests/opc/test_package.py`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/tests/opc/test_packuri.py` & `python-pptx-valutico-0.6.24.3/tests/opc/test_packuri.py`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/tests/opc/test_serialized.py` & `python-pptx-valutico-0.6.24.3/tests/opc/test_serialized.py`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/tests/opc/unitdata/rels.py` & `python-pptx-valutico-0.6.24.3/tests/opc/unitdata/rels.py`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/tests/oxml/shapes/test_autoshape.py` & `python-pptx-valutico-0.6.24.3/tests/oxml/shapes/test_autoshape.py`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/tests/oxml/shapes/test_graphfrm.py` & `python-pptx-valutico-0.6.24.3/tests/oxml/shapes/test_graphfrm.py`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/tests/oxml/shapes/test_groupshape.py` & `python-pptx-valutico-0.6.24.3/tests/oxml/shapes/test_groupshape.py`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/tests/oxml/shapes/test_picture.py` & `python-pptx-valutico-0.6.24.3/tests/oxml/shapes/test_picture.py`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/tests/oxml/test___init__.py` & `python-pptx-valutico-0.6.24.3/tests/oxml/test___init__.py`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/tests/oxml/test_dml.py` & `python-pptx-valutico-0.6.24.3/tests/oxml/test_dml.py`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/tests/oxml/test_ns.py` & `python-pptx-valutico-0.6.24.3/tests/oxml/test_ns.py`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/tests/oxml/test_presentation.py` & `python-pptx-valutico-0.6.24.3/tests/oxml/test_presentation.py`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/tests/oxml/test_simpletypes.py` & `python-pptx-valutico-0.6.24.3/tests/oxml/test_simpletypes.py`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/tests/oxml/test_slide.py` & `python-pptx-valutico-0.6.24.3/tests/oxml/test_slide.py`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/tests/oxml/test_table.py` & `python-pptx-valutico-0.6.24.3/tests/oxml/test_table.py`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/tests/oxml/test_theme.py` & `python-pptx-valutico-0.6.24.3/tests/oxml/test_theme.py`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/tests/oxml/test_xmlchemy.py` & `python-pptx-valutico-0.6.24.3/tests/oxml/test_xmlchemy.py`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/tests/oxml/unitdata/dml.py` & `python-pptx-valutico-0.6.24.3/tests/oxml/unitdata/dml.py`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/tests/oxml/unitdata/shape.py` & `python-pptx-valutico-0.6.24.3/tests/oxml/unitdata/shape.py`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/tests/oxml/unitdata/text.py` & `python-pptx-valutico-0.6.24.3/tests/oxml/unitdata/text.py`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/tests/parts/test_chart.py` & `python-pptx-valutico-0.6.24.3/tests/parts/test_chart.py`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/tests/parts/test_coreprops.py` & `python-pptx-valutico-0.6.24.3/tests/parts/test_coreprops.py`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/tests/parts/test_embeddedpackage.py` & `python-pptx-valutico-0.6.24.3/tests/parts/test_embeddedpackage.py`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/tests/parts/test_image.py` & `python-pptx-valutico-0.6.24.3/tests/parts/test_image.py`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/tests/parts/test_media.py` & `python-pptx-valutico-0.6.24.3/tests/parts/test_media.py`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/tests/parts/test_presentation.py` & `python-pptx-valutico-0.6.24.3/tests/parts/test_presentation.py`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/tests/parts/test_slide.py` & `python-pptx-valutico-0.6.24.3/tests/parts/test_slide.py`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/tests/shapes/test_autoshape.py` & `python-pptx-valutico-0.6.24.3/tests/shapes/test_autoshape.py`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/tests/shapes/test_base.py` & `python-pptx-valutico-0.6.24.3/tests/shapes/test_base.py`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/tests/shapes/test_connector.py` & `python-pptx-valutico-0.6.24.3/tests/shapes/test_connector.py`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/tests/shapes/test_freeform.py` & `python-pptx-valutico-0.6.24.3/tests/shapes/test_freeform.py`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/tests/shapes/test_graphfrm.py` & `python-pptx-valutico-0.6.24.3/tests/shapes/test_graphfrm.py`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/tests/shapes/test_group.py` & `python-pptx-valutico-0.6.24.3/tests/shapes/test_group.py`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/tests/shapes/test_picture.py` & `python-pptx-valutico-0.6.24.3/tests/shapes/test_picture.py`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/tests/shapes/test_placeholder.py` & `python-pptx-valutico-0.6.24.3/tests/shapes/test_placeholder.py`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/tests/shapes/test_shapetree.py` & `python-pptx-valutico-0.6.24.3/tests/shapes/test_shapetree.py`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/tests/test_action.py` & `python-pptx-valutico-0.6.24.3/tests/test_action.py`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/tests/test_api.py` & `python-pptx-valutico-0.6.24.3/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/tests/test_enum.py` & `python-pptx-valutico-0.6.24.3/tests/test_enum.py`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/tests/test_files/calibriz.ttf` & `python-pptx-valutico-0.6.24.3/tests/test_files/calibriz.ttf`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/tests/test_files/cdw-logo.eps` & `python-pptx-valutico-0.6.24.3/tests/test_files/cdw-logo.eps`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/tests/test_files/expanded_pptx/[Content_Types].xml` & `python-pptx-valutico-0.6.24.3/tests/test_files/expanded_pptx/[Content_Types].xml`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/tests/test_files/expanded_pptx/_rels/.rels` & `python-pptx-valutico-0.6.24.3/tests/test_files/expanded_pptx/_rels/.rels`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/tests/test_files/expanded_pptx/docProps/app.xml` & `python-pptx-valutico-0.6.24.3/tests/test_files/expanded_pptx/docProps/app.xml`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/tests/test_files/expanded_pptx/docProps/core.xml` & `python-pptx-valutico-0.6.24.3/tests/test_files/expanded_pptx/docProps/core.xml`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/tests/test_files/expanded_pptx/docProps/thumbnail.jpeg` & `python-pptx-valutico-0.6.24.3/tests/test_files/expanded_pptx/docProps/thumbnail.jpeg`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/tests/test_files/expanded_pptx/ppt/_rels/presentation.xml.rels` & `python-pptx-valutico-0.6.24.3/tests/test_files/expanded_pptx/ppt/_rels/presentation.xml.rels`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/tests/test_files/expanded_pptx/ppt/presentation.xml` & `python-pptx-valutico-0.6.24.3/tests/test_files/expanded_pptx/ppt/presentation.xml`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/tests/test_files/expanded_pptx/ppt/printerSettings/printerSettings1.bin` & `python-pptx-valutico-0.6.24.3/tests/test_files/expanded_pptx/ppt/printerSettings/printerSettings1.bin`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/tests/test_files/expanded_pptx/ppt/slideLayouts/slideLayout1.xml` & `python-pptx-valutico-0.6.24.3/tests/test_files/expanded_pptx/ppt/slideLayouts/slideLayout1.xml`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/tests/test_files/expanded_pptx/ppt/slideLayouts/slideLayout10.xml` & `python-pptx-valutico-0.6.24.3/tests/test_files/expanded_pptx/ppt/slideLayouts/slideLayout10.xml`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/tests/test_files/expanded_pptx/ppt/slideLayouts/slideLayout11.xml` & `python-pptx-valutico-0.6.24.3/tests/test_files/expanded_pptx/ppt/slideLayouts/slideLayout11.xml`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/tests/test_files/expanded_pptx/ppt/slideLayouts/slideLayout2.xml` & `python-pptx-valutico-0.6.24.3/tests/test_files/expanded_pptx/ppt/slideLayouts/slideLayout2.xml`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/tests/test_files/expanded_pptx/ppt/slideLayouts/slideLayout3.xml` & `python-pptx-valutico-0.6.24.3/tests/test_files/expanded_pptx/ppt/slideLayouts/slideLayout3.xml`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/tests/test_files/expanded_pptx/ppt/slideLayouts/slideLayout4.xml` & `python-pptx-valutico-0.6.24.3/tests/test_files/expanded_pptx/ppt/slideLayouts/slideLayout4.xml`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/tests/test_files/expanded_pptx/ppt/slideLayouts/slideLayout5.xml` & `python-pptx-valutico-0.6.24.3/tests/test_files/expanded_pptx/ppt/slideLayouts/slideLayout5.xml`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/tests/test_files/expanded_pptx/ppt/slideLayouts/slideLayout6.xml` & `python-pptx-valutico-0.6.24.3/tests/test_files/expanded_pptx/ppt/slideLayouts/slideLayout6.xml`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/tests/test_files/expanded_pptx/ppt/slideLayouts/slideLayout7.xml` & `python-pptx-valutico-0.6.24.3/tests/test_files/expanded_pptx/ppt/slideLayouts/slideLayout7.xml`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/tests/test_files/expanded_pptx/ppt/slideLayouts/slideLayout8.xml` & `python-pptx-valutico-0.6.24.3/tests/test_files/expanded_pptx/ppt/slideLayouts/slideLayout8.xml`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/tests/test_files/expanded_pptx/ppt/slideLayouts/slideLayout9.xml` & `python-pptx-valutico-0.6.24.3/tests/test_files/expanded_pptx/ppt/slideLayouts/slideLayout9.xml`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/tests/test_files/expanded_pptx/ppt/slideMasters/_rels/slideMaster1.xml.rels` & `python-pptx-valutico-0.6.24.3/tests/test_files/expanded_pptx/ppt/slideMasters/_rels/slideMaster1.xml.rels`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/tests/test_files/expanded_pptx/ppt/slideMasters/slideMaster1.xml` & `python-pptx-valutico-0.6.24.3/tests/test_files/expanded_pptx/ppt/slideMasters/slideMaster1.xml`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/tests/test_files/expanded_pptx/ppt/slides/slide1.xml` & `python-pptx-valutico-0.6.24.3/tests/test_files/expanded_pptx/ppt/slides/slide1.xml`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/tests/test_files/expanded_pptx/ppt/theme/theme1.xml` & `python-pptx-valutico-0.6.24.3/tests/test_files/expanded_pptx/ppt/theme/theme1.xml`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/tests/test_files/expanded_pptx/ppt/viewProps.xml` & `python-pptx-valutico-0.6.24.3/tests/test_files/expanded_pptx/ppt/viewProps.xml`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/tests/test_files/minimal.pptx` & `python-pptx-valutico-0.6.24.3/tests/test_files/minimal.pptx`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/tests/test_files/missing_rels_item.pptx` & `python-pptx-valutico-0.6.24.3/tests/test_files/missing_rels_item.pptx`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/tests/test_files/monty-truth.png` & `python-pptx-valutico-0.6.24.3/tests/test_files/monty-truth.png`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/tests/test_files/no-core-props.pptx` & `python-pptx-valutico-0.6.24.3/tests/test_files/no-core-props.pptx`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/tests/test_files/no-slides.pptx` & `python-pptx-valutico-0.6.24.3/tests/test_files/no-slides.pptx`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/tests/test_files/presentation.xml` & `python-pptx-valutico-0.6.24.3/tests/test_files/presentation.xml`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/tests/test_files/python-icon.jpeg` & `python-pptx-valutico-0.6.24.3/tests/test_files/python-icon.jpeg`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/tests/test_files/python-powered.png` & `python-pptx-valutico-0.6.24.3/tests/test_files/python-powered.png`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/tests/test_files/python.bmp` & `python-pptx-valutico-0.6.24.3/tests/test_files/python.bmp`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/tests/test_files/slideLayout1.xml` & `python-pptx-valutico-0.6.24.3/tests/test_files/slideLayout1.xml`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/tests/test_files/snippets/2x2-area-date.txt` & `python-pptx-valutico-0.6.24.3/tests/test_files/snippets/2x2-area-date.txt`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/tests/test_files/snippets/2x2-area-float.txt` & `python-pptx-valutico-0.6.24.3/tests/test_files/snippets/2x2-area-float.txt`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/tests/test_files/snippets/2x2-area-stacked-100.txt` & `python-pptx-valutico-0.6.24.3/tests/test_files/snippets/2x2-area-stacked-100.txt`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/tests/test_files/snippets/2x2-area-stacked.txt` & `python-pptx-valutico-0.6.24.3/tests/test_files/snippets/2x2-area-stacked.txt`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/tests/test_files/snippets/2x2-area.txt` & `python-pptx-valutico-0.6.24.3/tests/test_files/snippets/2x2-area.txt`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/tests/test_files/snippets/2x2-bar-clustered-date.txt` & `python-pptx-valutico-0.6.24.3/tests/test_files/snippets/2x2-bar-clustered-date.txt`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/tests/test_files/snippets/2x2-bar-clustered-float.txt` & `python-pptx-valutico-0.6.24.3/tests/test_files/snippets/2x2-bar-clustered-float.txt`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/tests/test_files/snippets/2x2-bar-clustered.txt` & `python-pptx-valutico-0.6.24.3/tests/test_files/snippets/2x2-bar-clustered.txt`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/tests/test_files/snippets/2x2-bar-stacked-100.txt` & `python-pptx-valutico-0.6.24.3/tests/test_files/snippets/2x2-bar-stacked-100.txt`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/tests/test_files/snippets/2x2-bar-stacked.txt` & `python-pptx-valutico-0.6.24.3/tests/test_files/snippets/2x2-bar-stacked.txt`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/tests/test_files/snippets/2x2-column-clustered.txt` & `python-pptx-valutico-0.6.24.3/tests/test_files/snippets/2x2-column-clustered.txt`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/tests/test_files/snippets/2x2-column-stacked-100.txt` & `python-pptx-valutico-0.6.24.3/tests/test_files/snippets/2x2-column-stacked-100.txt`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/tests/test_files/snippets/2x2-column-stacked.txt` & `python-pptx-valutico-0.6.24.3/tests/test_files/snippets/2x2-column-stacked.txt`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/tests/test_files/snippets/2x2-line-date.txt` & `python-pptx-valutico-0.6.24.3/tests/test_files/snippets/2x2-line-date.txt`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/tests/test_files/snippets/2x2-line-float.txt` & `python-pptx-valutico-0.6.24.3/tests/test_files/snippets/2x2-line-float.txt`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/tests/test_files/snippets/2x2-line-markers-stacked-100.txt` & `python-pptx-valutico-0.6.24.3/tests/test_files/snippets/2x2-line-markers-stacked-100.txt`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/tests/test_files/snippets/2x2-line-markers-stacked.txt` & `python-pptx-valutico-0.6.24.3/tests/test_files/snippets/2x2-line-markers-stacked.txt`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/tests/test_files/snippets/2x2-line-markers.txt` & `python-pptx-valutico-0.6.24.3/tests/test_files/snippets/2x2-line-markers.txt`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/tests/test_files/snippets/2x2-line-stacked-100.txt` & `python-pptx-valutico-0.6.24.3/tests/test_files/snippets/2x2-line-stacked-100.txt`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/tests/test_files/snippets/2x2-line-stacked.txt` & `python-pptx-valutico-0.6.24.3/tests/test_files/snippets/2x2-line-stacked.txt`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/tests/test_files/snippets/2x2-line.txt` & `python-pptx-valutico-0.6.24.3/tests/test_files/snippets/2x2-line.txt`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/tests/test_files/snippets/2x3-bubble-3d.txt` & `python-pptx-valutico-0.6.24.3/tests/test_files/snippets/2x3-bubble-3d.txt`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/tests/test_files/snippets/2x3-bubble.txt` & `python-pptx-valutico-0.6.24.3/tests/test_files/snippets/2x3-bubble.txt`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/tests/test_files/snippets/2x3-xy-lines-no-markers.txt` & `python-pptx-valutico-0.6.24.3/tests/test_files/snippets/2x3-xy-lines-no-markers.txt`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/tests/test_files/snippets/2x3-xy-lines.txt` & `python-pptx-valutico-0.6.24.3/tests/test_files/snippets/2x3-xy-lines.txt`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/tests/test_files/snippets/2x3-xy-smooth-no-markers.txt` & `python-pptx-valutico-0.6.24.3/tests/test_files/snippets/2x3-xy-smooth-no-markers.txt`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/tests/test_files/snippets/2x3-xy-smooth.txt` & `python-pptx-valutico-0.6.24.3/tests/test_files/snippets/2x3-xy-smooth.txt`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/tests/test_files/snippets/2x3-xy.txt` & `python-pptx-valutico-0.6.24.3/tests/test_files/snippets/2x3-xy.txt`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/tests/test_files/snippets/2x5-radar.txt` & `python-pptx-valutico-0.6.24.3/tests/test_files/snippets/2x5-radar.txt`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/tests/test_files/snippets/3x1-pie-exploded.txt` & `python-pptx-valutico-0.6.24.3/tests/test_files/snippets/3x1-pie-exploded.txt`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/tests/test_files/snippets/3x1-pie.txt` & `python-pptx-valutico-0.6.24.3/tests/test_files/snippets/3x1-pie.txt`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/tests/test_files/snippets/3x2-doughnut-exploded.txt` & `python-pptx-valutico-0.6.24.3/tests/test_files/snippets/3x2-doughnut-exploded.txt`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/tests/test_files/snippets/3x2-doughnut.txt` & `python-pptx-valutico-0.6.24.3/tests/test_files/snippets/3x2-doughnut.txt`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/tests/test_files/snippets/4x2-multi-cat-bar.txt` & `python-pptx-valutico-0.6.24.3/tests/test_files/snippets/4x2-multi-cat-bar.txt`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/tests/test_files/snippets/adjust-ser-count.txt` & `python-pptx-valutico-0.6.24.3/tests/test_files/snippets/adjust-ser-count.txt`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/tests/test_files/snippets/cat-labels.txt` & `python-pptx-valutico-0.6.24.3/tests/test_files/snippets/cat-labels.txt`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/tests/test_files/snippets/content-types-xml.txt` & `python-pptx-valutico-0.6.24.3/tests/test_files/snippets/content-types-xml.txt`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/tests/test_files/snippets/default-notes.txt` & `python-pptx-valutico-0.6.24.3/tests/test_files/snippets/default-notes.txt`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/tests/test_files/snippets/default-notesMaster.txt` & `python-pptx-valutico-0.6.24.3/tests/test_files/snippets/default-notesMaster.txt`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/tests/test_files/snippets/default-theme.txt` & `python-pptx-valutico-0.6.24.3/tests/test_files/snippets/default-theme.txt`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/tests/test_files/snippets/freeform.txt` & `python-pptx-valutico-0.6.24.3/tests/test_files/snippets/freeform.txt`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/tests/test_files/snippets/package-rels-xml.txt` & `python-pptx-valutico-0.6.24.3/tests/test_files/snippets/package-rels-xml.txt`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/tests/test_files/snippets/placeholders.txt` & `python-pptx-valutico-0.6.24.3/tests/test_files/snippets/placeholders.txt`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/tests/test_files/snippets/presentation-rels-xml.txt` & `python-pptx-valutico-0.6.24.3/tests/test_files/snippets/presentation-rels-xml.txt`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/tests/test_files/snippets/rels-load-from-xml.txt` & `python-pptx-valutico-0.6.24.3/tests/test_files/snippets/rels-load-from-xml.txt`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/tests/test_files/snippets/rewrite-ser.txt` & `python-pptx-valutico-0.6.24.3/tests/test_files/snippets/rewrite-ser.txt`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/tests/test_files/snippets/timing.txt` & `python-pptx-valutico-0.6.24.3/tests/test_files/snippets/timing.txt`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/tests/test_files/test.pptx` & `python-pptx-valutico-0.6.24.3/tests/test_files/test.pptx`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/tests/test_files/test_slides.pptx` & `python-pptx-valutico-0.6.24.3/tests/test_files/test_slides.pptx`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/tests/test_media.py` & `python-pptx-valutico-0.6.24.3/tests/test_media.py`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/tests/test_package.py` & `python-pptx-valutico-0.6.24.3/tests/test_package.py`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/tests/test_presentation.py` & `python-pptx-valutico-0.6.24.3/tests/test_presentation.py`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/tests/test_shared.py` & `python-pptx-valutico-0.6.24.3/tests/test_shared.py`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/tests/test_slide.py` & `python-pptx-valutico-0.6.24.3/tests/test_slide.py`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/tests/test_table.py` & `python-pptx-valutico-0.6.24.3/tests/test_table.py`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/tests/test_util.py` & `python-pptx-valutico-0.6.24.3/tests/test_util.py`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/tests/text/test_fonts.py` & `python-pptx-valutico-0.6.24.3/tests/text/test_fonts.py`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/tests/text/test_layout.py` & `python-pptx-valutico-0.6.24.3/tests/text/test_layout.py`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/tests/text/test_text.py` & `python-pptx-valutico-0.6.24.3/tests/text/test_text.py`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/tests/unitdata.py` & `python-pptx-valutico-0.6.24.3/tests/unitdata.py`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/tests/unitutil/cxml.py` & `python-pptx-valutico-0.6.24.3/tests/unitutil/cxml.py`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/tests/unitutil/file.py` & `python-pptx-valutico-0.6.24.3/tests/unitutil/file.py`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/tests/unitutil/mock.py` & `python-pptx-valutico-0.6.24.3/tests/unitutil/mock.py`

 * *Files identical despite different names*

### Comparing `python-pptx-valutico-0.6.24.2/tox.ini` & `python-pptx-valutico-0.6.24.3/tox.ini`

 * *Files identical despite different names*

