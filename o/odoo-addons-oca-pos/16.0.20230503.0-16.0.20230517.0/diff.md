# Comparing `tmp/odoo_addons_oca_pos-16.0.20230503.0-py3-none-any.whl.zip` & `tmp/odoo_addons_oca_pos-16.0.20230517.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,6 +1,6 @@
-Zip file size: 1478 bytes, number of entries: 4
--rw-r--r--  2.0 unx     1462 b- defN 23-May-04 06:11 odoo_addons_oca_pos-16.0.20230503.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-04 06:11 odoo_addons_oca_pos-16.0.20230503.0.dist-info/WHEEL
--rw-r--r--  2.0 unx        1 b- defN 23-May-04 06:11 odoo_addons_oca_pos-16.0.20230503.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      385 b- defN 23-May-04 06:11 odoo_addons_oca_pos-16.0.20230503.0.dist-info/RECORD
-4 files, 1940 bytes uncompressed, 720 bytes compressed:  62.9%
+Zip file size: 1485 bytes, number of entries: 4
+-rw-r--r--  2.0 unx     1528 b- defN 23-May-18 06:26 odoo_addons_oca_pos-16.0.20230517.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-18 06:26 odoo_addons_oca_pos-16.0.20230517.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx        1 b- defN 23-May-18 06:26 odoo_addons_oca_pos-16.0.20230517.0.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      385 b- defN 23-May-18 06:26 odoo_addons_oca_pos-16.0.20230517.0.dist-info/RECORD
+4 files, 2006 bytes uncompressed, 727 bytes compressed:  63.8%
```

## zipnote {}

```diff
@@ -1,13 +1,13 @@
-Filename: odoo_addons_oca_pos-16.0.20230503.0.dist-info/METADATA
+Filename: odoo_addons_oca_pos-16.0.20230517.0.dist-info/METADATA
 Comment: 
 
-Filename: odoo_addons_oca_pos-16.0.20230503.0.dist-info/WHEEL
+Filename: odoo_addons_oca_pos-16.0.20230517.0.dist-info/WHEEL
 Comment: 
 
-Filename: odoo_addons_oca_pos-16.0.20230503.0.dist-info/top_level.txt
+Filename: odoo_addons_oca_pos-16.0.20230517.0.dist-info/top_level.txt
 Comment: 
 
-Filename: odoo_addons_oca_pos-16.0.20230503.0.dist-info/RECORD
+Filename: odoo_addons_oca_pos-16.0.20230517.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `odoo_addons_oca_pos-16.0.20230503.0.dist-info/METADATA` & `odoo_addons_oca_pos-16.0.20230517.0.dist-info/METADATA`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: odoo-addons-oca-pos
-Version: 16.0.20230503.0
+Version: 16.0.20230517.0
 Summary: Meta package for oca-pos Odoo addons
 Home-page: UNKNOWN
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
 Classifier: Framework :: Odoo
 Classifier: Framework :: Odoo :: 16.0
@@ -16,14 +16,15 @@
 Requires-Dist: odoo-addon-pos-lot-barcode (<16.1dev,>=16.0dev)
 Requires-Dist: odoo-addon-pos-lot-selection (<16.1dev,>=16.0dev)
 Requires-Dist: odoo-addon-pos-membership (<16.1dev,>=16.0dev)
 Requires-Dist: odoo-addon-pos-order-remove-line (<16.1dev,>=16.0dev)
 Requires-Dist: odoo-addon-pos-order-reorder (<16.1dev,>=16.0dev)
 Requires-Dist: odoo-addon-pos-order-to-sale-order (<16.1dev,>=16.0dev)
 Requires-Dist: odoo-addon-pos-partner-birthdate (<16.1dev,>=16.0dev)
+Requires-Dist: odoo-addon-pos-payment-change (<16.1dev,>=16.0dev)
 Requires-Dist: odoo-addon-pos-payment-terminal (<16.1dev,>=16.0dev)
 Requires-Dist: odoo-addon-pos-product-display-default-code (<16.1dev,>=16.0dev)
 Requires-Dist: odoo-addon-pos-product-quick-info (<16.1dev,>=16.0dev)
 Requires-Dist: odoo-addon-pos-receipt-hide-price (<16.1dev,>=16.0dev)
 Requires-Dist: odoo-addon-pos-stock-available-online (<16.1dev,>=16.0dev)
 
 UNKNOWN
```

