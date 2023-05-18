# Comparing `tmp/odoo_addon_upgrade_analysis-16.0.1.0.0.5-py3-none-any.whl.zip` & `tmp/odoo_addon_upgrade_analysis-16.0.1.0.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,56 +1,56 @@
-Zip file size: 65405 bytes, number of entries: 54
--rw-r--r--  2.0 unx     4374 b- defN 22-Nov-19 05:50 odoo/addons/upgrade_analysis/README.rst
--rw-r--r--  2.0 unx      140 b- defN 22-Nov-19 05:50 odoo/addons/upgrade_analysis/__init__.py
--rw-r--r--  2.0 unx     1077 b- defN 22-Nov-19 05:50 odoo/addons/upgrade_analysis/__manifest__.py
--rw-r--r--  2.0 unx      362 b- defN 22-Nov-19 05:50 odoo/addons/upgrade_analysis/blacklist.py
--rw-r--r--  2.0 unx    20132 b- defN 22-Nov-19 05:50 odoo/addons/upgrade_analysis/compare.py
--rw-r--r--  2.0 unx     8297 b- defN 22-Nov-19 05:50 odoo/addons/upgrade_analysis/upgrade_log.py
--rw-r--r--  2.0 unx    21729 b- defN 22-Nov-19 05:50 odoo/addons/upgrade_analysis/i18n/es_AR.po
--rw-r--r--  2.0 unx    19394 b- defN 22-Nov-19 05:50 odoo/addons/upgrade_analysis/i18n/fr.po
--rw-r--r--  2.0 unx    19158 b- defN 22-Nov-19 05:50 odoo/addons/upgrade_analysis/i18n/upgrade_analysis.pot
--rw-r--r--  2.0 unx      163 b- defN 22-Nov-19 05:50 odoo/addons/upgrade_analysis/models/__init__.py
--rw-r--r--  2.0 unx     1031 b- defN 22-Nov-19 05:50 odoo/addons/upgrade_analysis/models/ir_module_module.py
--rw-r--r--  2.0 unx    22546 b- defN 22-Nov-19 05:50 odoo/addons/upgrade_analysis/models/upgrade_analysis.py
--rw-r--r--  2.0 unx      536 b- defN 22-Nov-19 05:50 odoo/addons/upgrade_analysis/models/upgrade_attribute.py
--rw-r--r--  2.0 unx     3098 b- defN 22-Nov-19 05:50 odoo/addons/upgrade_analysis/models/upgrade_comparison_config.py
--rw-r--r--  2.0 unx     6006 b- defN 22-Nov-19 05:50 odoo/addons/upgrade_analysis/models/upgrade_record.py
--rw-r--r--  2.0 unx       65 b- defN 22-Nov-19 05:50 odoo/addons/upgrade_analysis/odoo_patch/__init__.py
--rw-r--r--  2.0 unx     1843 b- defN 22-Nov-19 05:50 odoo/addons/upgrade_analysis/odoo_patch/odoo_patch.py
--rw-r--r--  2.0 unx       66 b- defN 22-Nov-19 05:50 odoo/addons/upgrade_analysis/odoo_patch/addons/__init__.py
--rw-r--r--  2.0 unx      270 b- defN 22-Nov-19 05:50 odoo/addons/upgrade_analysis/odoo_patch/addons/mrp/__init__.py
--rw-r--r--  2.0 unx      371 b- defN 22-Nov-19 05:50 odoo/addons/upgrade_analysis/odoo_patch/addons/point_of_sale/__init__.py
--rw-r--r--  2.0 unx      259 b- defN 22-Nov-19 05:50 odoo/addons/upgrade_analysis/odoo_patch/addons/stock/__init__.py
--rw-r--r--  2.0 unx       84 b- defN 22-Nov-19 05:50 odoo/addons/upgrade_analysis/odoo_patch/odoo/__init__.py
--rw-r--r--  2.0 unx      739 b- defN 22-Nov-19 05:50 odoo/addons/upgrade_analysis/odoo_patch/odoo/models.py
--rw-r--r--  2.0 unx       19 b- defN 22-Nov-19 05:50 odoo/addons/upgrade_analysis/odoo_patch/odoo/addons/__init__.py
--rw-r--r--  2.0 unx       21 b- defN 22-Nov-19 05:50 odoo/addons/upgrade_analysis/odoo_patch/odoo/addons/base/__init__.py
--rw-r--r--  2.0 unx       23 b- defN 22-Nov-19 05:50 odoo/addons/upgrade_analysis/odoo_patch/odoo/addons/base/models/__init__.py
--rw-r--r--  2.0 unx     1482 b- defN 22-Nov-19 05:50 odoo/addons/upgrade_analysis/odoo_patch/odoo/addons/base/models/ir_model.py
--rw-r--r--  2.0 unx       23 b- defN 22-Nov-19 05:50 odoo/addons/upgrade_analysis/odoo_patch/odoo/modules/__init__.py
--rw-r--r--  2.0 unx     1032 b- defN 22-Nov-19 05:50 odoo/addons/upgrade_analysis/odoo_patch/odoo/modules/registry.py
--rw-r--r--  2.0 unx       22 b- defN 22-Nov-19 05:50 odoo/addons/upgrade_analysis/odoo_patch/odoo/tools/__init__.py
--rw-r--r--  2.0 unx      397 b- defN 22-Nov-19 05:50 odoo/addons/upgrade_analysis/odoo_patch/odoo/tools/convert.py
--rw-r--r--  2.0 unx      308 b- defN 22-Nov-19 05:50 odoo/addons/upgrade_analysis/readme/CONTRIBUTORS.rst
--rw-r--r--  2.0 unx      675 b- defN 22-Nov-19 05:50 odoo/addons/upgrade_analysis/readme/DESCRIPTION.rst
--rw-r--r--  2.0 unx      263 b- defN 22-Nov-19 05:50 odoo/addons/upgrade_analysis/readme/ROADMAP.rst
--rw-r--r--  2.0 unx       71 b- defN 22-Nov-19 05:50 odoo/addons/upgrade_analysis/readme/USAGE.rst
--rw-r--r--  2.0 unx      696 b- defN 22-Nov-19 05:50 odoo/addons/upgrade_analysis/security/ir.model.access.csv
--rw-r--r--  2.0 unx     9455 b- defN 22-Nov-19 05:50 odoo/addons/upgrade_analysis/static/description/icon.png
--rw-r--r--  2.0 unx    14699 b- defN 22-Nov-19 05:50 odoo/addons/upgrade_analysis/static/description/index.html
--rw-r--r--  2.0 unx      744 b- defN 22-Nov-19 05:50 odoo/addons/upgrade_analysis/static/src/module_coverage_template.rst.mako
--rw-r--r--  2.0 unx       26 b- defN 22-Nov-19 05:50 odoo/addons/upgrade_analysis/tests/__init__.py
--rw-r--r--  2.0 unx     1787 b- defN 22-Nov-19 05:50 odoo/addons/upgrade_analysis/tests/test_module.py
--rw-r--r--  2.0 unx      200 b- defN 22-Nov-19 05:50 odoo/addons/upgrade_analysis/views/menu.xml
--rw-r--r--  2.0 unx     2640 b- defN 22-Nov-19 05:50 odoo/addons/upgrade_analysis/views/view_upgrade_analysis.xml
--rw-r--r--  2.0 unx     2826 b- defN 22-Nov-19 05:50 odoo/addons/upgrade_analysis/views/view_upgrade_comparison_config.xml
--rw-r--r--  2.0 unx     2834 b- defN 22-Nov-19 05:50 odoo/addons/upgrade_analysis/views/view_upgrade_record.xml
--rw-r--r--  2.0 unx       82 b- defN 22-Nov-19 05:50 odoo/addons/upgrade_analysis/wizards/__init__.py
--rw-r--r--  2.0 unx     4527 b- defN 22-Nov-19 05:50 odoo/addons/upgrade_analysis/wizards/upgrade_generate_record_wizard.py
--rw-r--r--  2.0 unx     4040 b- defN 22-Nov-19 05:50 odoo/addons/upgrade_analysis/wizards/upgrade_install_wizard.py
--rw-r--r--  2.0 unx     1787 b- defN 22-Nov-19 05:50 odoo/addons/upgrade_analysis/wizards/view_upgrade_generate_record_wizard.xml
--rw-r--r--  2.0 unx     3289 b- defN 22-Nov-19 05:50 odoo/addons/upgrade_analysis/wizards/view_upgrade_install_wizard.xml
--rw-r--r--  2.0 unx     5095 b- defN 22-Nov-19 05:50 odoo_addon_upgrade_analysis-16.0.1.0.0.5.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 22-Nov-19 05:50 odoo_addon_upgrade_analysis-16.0.1.0.0.5.dist-info/WHEEL
--rw-r--r--  2.0 unx        5 b- defN 22-Nov-19 05:50 odoo_addon_upgrade_analysis-16.0.1.0.0.5.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     6025 b- defN 22-Nov-19 05:50 odoo_addon_upgrade_analysis-16.0.1.0.0.5.dist-info/RECORD
-54 files, 196925 bytes uncompressed, 55205 bytes compressed:  72.0%
+Zip file size: 65394 bytes, number of entries: 54
+-rw-r--r--  2.0 unx     4374 b- defN 23-May-18 08:36 odoo/addons/upgrade_analysis/README.rst
+-rw-r--r--  2.0 unx      140 b- defN 23-May-18 08:35 odoo/addons/upgrade_analysis/__init__.py
+-rw-r--r--  2.0 unx     1077 b- defN 23-May-18 08:36 odoo/addons/upgrade_analysis/__manifest__.py
+-rw-r--r--  2.0 unx      362 b- defN 23-May-18 08:35 odoo/addons/upgrade_analysis/blacklist.py
+-rw-r--r--  2.0 unx    20132 b- defN 23-May-18 08:35 odoo/addons/upgrade_analysis/compare.py
+-rw-r--r--  2.0 unx     8297 b- defN 23-May-18 08:35 odoo/addons/upgrade_analysis/upgrade_log.py
+-rw-r--r--  2.0 unx    21729 b- defN 23-May-18 08:35 odoo/addons/upgrade_analysis/i18n/es_AR.po
+-rw-r--r--  2.0 unx    19394 b- defN 23-May-18 08:35 odoo/addons/upgrade_analysis/i18n/fr.po
+-rw-r--r--  2.0 unx    19158 b- defN 23-May-18 08:35 odoo/addons/upgrade_analysis/i18n/upgrade_analysis.pot
+-rw-r--r--  2.0 unx      163 b- defN 23-May-18 08:35 odoo/addons/upgrade_analysis/models/__init__.py
+-rw-r--r--  2.0 unx     1031 b- defN 23-May-18 08:35 odoo/addons/upgrade_analysis/models/ir_module_module.py
+-rw-r--r--  2.0 unx    22546 b- defN 23-May-18 08:35 odoo/addons/upgrade_analysis/models/upgrade_analysis.py
+-rw-r--r--  2.0 unx      536 b- defN 23-May-18 08:35 odoo/addons/upgrade_analysis/models/upgrade_attribute.py
+-rw-r--r--  2.0 unx     3098 b- defN 23-May-18 08:35 odoo/addons/upgrade_analysis/models/upgrade_comparison_config.py
+-rw-r--r--  2.0 unx     6006 b- defN 23-May-18 08:35 odoo/addons/upgrade_analysis/models/upgrade_record.py
+-rw-r--r--  2.0 unx       65 b- defN 23-May-18 08:35 odoo/addons/upgrade_analysis/odoo_patch/__init__.py
+-rw-r--r--  2.0 unx     1843 b- defN 23-May-18 08:35 odoo/addons/upgrade_analysis/odoo_patch/odoo_patch.py
+-rw-r--r--  2.0 unx       66 b- defN 23-May-18 08:35 odoo/addons/upgrade_analysis/odoo_patch/addons/__init__.py
+-rw-r--r--  2.0 unx      270 b- defN 23-May-18 08:35 odoo/addons/upgrade_analysis/odoo_patch/addons/mrp/__init__.py
+-rw-r--r--  2.0 unx      371 b- defN 23-May-18 08:35 odoo/addons/upgrade_analysis/odoo_patch/addons/point_of_sale/__init__.py
+-rw-r--r--  2.0 unx      259 b- defN 23-May-18 08:35 odoo/addons/upgrade_analysis/odoo_patch/addons/stock/__init__.py
+-rw-r--r--  2.0 unx       84 b- defN 23-May-18 08:35 odoo/addons/upgrade_analysis/odoo_patch/odoo/__init__.py
+-rw-r--r--  2.0 unx      739 b- defN 23-May-18 08:35 odoo/addons/upgrade_analysis/odoo_patch/odoo/models.py
+-rw-r--r--  2.0 unx       19 b- defN 23-May-18 08:35 odoo/addons/upgrade_analysis/odoo_patch/odoo/addons/__init__.py
+-rw-r--r--  2.0 unx       21 b- defN 23-May-18 08:35 odoo/addons/upgrade_analysis/odoo_patch/odoo/addons/base/__init__.py
+-rw-r--r--  2.0 unx       23 b- defN 23-May-18 08:35 odoo/addons/upgrade_analysis/odoo_patch/odoo/addons/base/models/__init__.py
+-rw-r--r--  2.0 unx     1482 b- defN 23-May-18 08:35 odoo/addons/upgrade_analysis/odoo_patch/odoo/addons/base/models/ir_model.py
+-rw-r--r--  2.0 unx       23 b- defN 23-May-18 08:35 odoo/addons/upgrade_analysis/odoo_patch/odoo/modules/__init__.py
+-rw-r--r--  2.0 unx     1112 b- defN 23-May-18 08:36 odoo/addons/upgrade_analysis/odoo_patch/odoo/modules/registry.py
+-rw-r--r--  2.0 unx       22 b- defN 23-May-18 08:35 odoo/addons/upgrade_analysis/odoo_patch/odoo/tools/__init__.py
+-rw-r--r--  2.0 unx      397 b- defN 23-May-18 08:35 odoo/addons/upgrade_analysis/odoo_patch/odoo/tools/convert.py
+-rw-r--r--  2.0 unx      308 b- defN 23-May-18 08:35 odoo/addons/upgrade_analysis/readme/CONTRIBUTORS.rst
+-rw-r--r--  2.0 unx      675 b- defN 23-May-18 08:35 odoo/addons/upgrade_analysis/readme/DESCRIPTION.rst
+-rw-r--r--  2.0 unx      263 b- defN 23-May-18 08:35 odoo/addons/upgrade_analysis/readme/ROADMAP.rst
+-rw-r--r--  2.0 unx       71 b- defN 23-May-18 08:35 odoo/addons/upgrade_analysis/readme/USAGE.rst
+-rw-r--r--  2.0 unx      696 b- defN 23-May-18 08:35 odoo/addons/upgrade_analysis/security/ir.model.access.csv
+-rw-r--r--  2.0 unx     9455 b- defN 23-May-18 08:35 odoo/addons/upgrade_analysis/static/description/icon.png
+-rw-r--r--  2.0 unx    14699 b- defN 23-May-18 08:36 odoo/addons/upgrade_analysis/static/description/index.html
+-rw-r--r--  2.0 unx      744 b- defN 23-May-18 08:35 odoo/addons/upgrade_analysis/static/src/module_coverage_template.rst.mako
+-rw-r--r--  2.0 unx       26 b- defN 23-May-18 08:35 odoo/addons/upgrade_analysis/tests/__init__.py
+-rw-r--r--  2.0 unx     1787 b- defN 23-May-18 08:35 odoo/addons/upgrade_analysis/tests/test_module.py
+-rw-r--r--  2.0 unx      200 b- defN 23-May-18 08:35 odoo/addons/upgrade_analysis/views/menu.xml
+-rw-r--r--  2.0 unx     2640 b- defN 23-May-18 08:35 odoo/addons/upgrade_analysis/views/view_upgrade_analysis.xml
+-rw-r--r--  2.0 unx     2826 b- defN 23-May-18 08:35 odoo/addons/upgrade_analysis/views/view_upgrade_comparison_config.xml
+-rw-r--r--  2.0 unx     2834 b- defN 23-May-18 08:35 odoo/addons/upgrade_analysis/views/view_upgrade_record.xml
+-rw-r--r--  2.0 unx       82 b- defN 23-May-18 08:35 odoo/addons/upgrade_analysis/wizards/__init__.py
+-rw-r--r--  2.0 unx     4527 b- defN 23-May-18 08:35 odoo/addons/upgrade_analysis/wizards/upgrade_generate_record_wizard.py
+-rw-r--r--  2.0 unx     4040 b- defN 23-May-18 08:35 odoo/addons/upgrade_analysis/wizards/upgrade_install_wizard.py
+-rw-r--r--  2.0 unx     1787 b- defN 23-May-18 08:35 odoo/addons/upgrade_analysis/wizards/view_upgrade_generate_record_wizard.xml
+-rw-r--r--  2.0 unx     3289 b- defN 23-May-18 08:35 odoo/addons/upgrade_analysis/wizards/view_upgrade_install_wizard.xml
+-rw-r--r--  2.0 unx     5093 b- defN 23-May-18 08:36 odoo_addon_upgrade_analysis-16.0.1.0.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-18 08:36 odoo_addon_upgrade_analysis-16.0.1.0.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx        5 b- defN 23-May-18 08:36 odoo_addon_upgrade_analysis-16.0.1.0.1.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     6017 b- defN 23-May-18 08:36 odoo_addon_upgrade_analysis-16.0.1.0.1.dist-info/RECORD
+54 files, 196995 bytes uncompressed, 55210 bytes compressed:  72.0%
```

## zipnote {}

```diff
@@ -144,20 +144,20 @@
 
 Filename: odoo/addons/upgrade_analysis/wizards/view_upgrade_generate_record_wizard.xml
 Comment: 
 
 Filename: odoo/addons/upgrade_analysis/wizards/view_upgrade_install_wizard.xml
 Comment: 
 
-Filename: odoo_addon_upgrade_analysis-16.0.1.0.0.5.dist-info/METADATA
+Filename: odoo_addon_upgrade_analysis-16.0.1.0.1.dist-info/METADATA
 Comment: 
 
-Filename: odoo_addon_upgrade_analysis-16.0.1.0.0.5.dist-info/WHEEL
+Filename: odoo_addon_upgrade_analysis-16.0.1.0.1.dist-info/WHEEL
 Comment: 
 
-Filename: odoo_addon_upgrade_analysis-16.0.1.0.0.5.dist-info/top_level.txt
+Filename: odoo_addon_upgrade_analysis-16.0.1.0.1.dist-info/top_level.txt
 Comment: 
 
-Filename: odoo_addon_upgrade_analysis-16.0.1.0.0.5.dist-info/RECORD
+Filename: odoo_addon_upgrade_analysis-16.0.1.0.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## odoo/addons/upgrade_analysis/__manifest__.py

```diff
@@ -1,15 +1,15 @@
 # Copyright 2011-2015 Therp BV <https://therp.nl>
 # Copyright 2016 Opener B.V. <https://opener.am>
 # License AGPL-3.0 or later (http://www.gnu.org/licenses/agpl).
 {
     "name": "Upgrade Analysis",
     "summary": "Performs a difference analysis between modules"
     " installed on two different Odoo instances",
-    "version": "16.0.1.0.0",
+    "version": "16.0.1.0.1",
     "category": "Migration",
     "author": "Therp BV, Opener B.V., GRAP, Odoo Community Association (OCA)",
     "maintainers": ["StefanRijnhart", "legalsylvain"],
     "website": "https://github.com/OCA/server-tools",
     "data": [
         "security/ir.model.access.csv",
         "views/menu.xml",
```

## odoo/addons/upgrade_analysis/odoo_patch/odoo/modules/registry.py

```diff
@@ -11,23 +11,24 @@
 
 
 class RegistryPatch(OdooPatch):
     target = Registry
     method_names = ["init_models"]
 
     def init_models(self, cr, model_names, context, install=True):
-        module_name = context["module"]
-        _logger.debug("Logging models of module %s", module_name)
-        upg_registry = current_thread()._upgrade_registry
-        local_registry = {}
-        env = api.Environment(cr, SUPERUSER_ID, {})
-        for model in env.values():
-            if not model._auto:
-                continue
-            upgrade_log.log_model(model, local_registry)
-        upgrade_log.compare_registries(
-            cr, context["module"], upg_registry, local_registry
-        )
+        if "module" in context:
+            module_name = context["module"]
+            _logger.debug("Logging models of module %s", module_name)
+            upg_registry = current_thread()._upgrade_registry
+            local_registry = {}
+            env = api.Environment(cr, SUPERUSER_ID, {})
+            for model in env.values():
+                if not model._auto:
+                    continue
+                upgrade_log.log_model(model, local_registry)
+            upgrade_log.compare_registries(
+                cr, context["module"], upg_registry, local_registry
+            )
 
         return RegistryPatch.init_models._original_method(
             self, cr, model_names, context, install=install
         )
```

## Comparing `odoo_addon_upgrade_analysis-16.0.1.0.0.5.dist-info/METADATA` & `odoo_addon_upgrade_analysis-16.0.1.0.1.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: odoo-addon-upgrade-analysis
-Version: 16.0.1.0.0.5
+Version: 16.0.1.0.1
 Summary: Performs a difference analysis between modules installed on two different Odoo instances
 Home-page: https://github.com/OCA/server-tools
 Author: Therp BV, Opener B.V., GRAP, Odoo Community Association (OCA)
 Author-email: support@odoo-community.org
 License: AGPL-3
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
```

## Comparing `odoo_addon_upgrade_analysis-16.0.1.0.0.5.dist-info/RECORD` & `odoo_addon_upgrade_analysis-16.0.1.0.1.dist-info/RECORD`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 odoo/addons/upgrade_analysis/README.rst,sha256=L7fJmx5z1ACd9xMUYSPAYUCMyK-_myiqZNYyH-OMuRk,4374
 odoo/addons/upgrade_analysis/__init__.py,sha256=1X8E6viDvX9QCI3au33OFkjFkJbFw6TazruSkrDurdI,140
-odoo/addons/upgrade_analysis/__manifest__.py,sha256=hHU1qBDS8QdOrjuAwMFG_oton_QcFy25XQFyu7cFWjM,1077
+odoo/addons/upgrade_analysis/__manifest__.py,sha256=2OZzZt_W_D_UHpRmz5g55BHdbvtbP0Mf9sflPZLieyY,1077
 odoo/addons/upgrade_analysis/blacklist.py,sha256=BIu8cYUB6j3FYtSaRcs4nSxB6yUwyjhxzOaex1AiIHY,362
 odoo/addons/upgrade_analysis/compare.py,sha256=XSetlfvLS0LBy9nI5kF1gcneaaMo7kjd2uAwPz4KSoQ,20132
 odoo/addons/upgrade_analysis/upgrade_log.py,sha256=aUeWhlnpxJIF5lgHoLfbZTlqHpgXcK-GNsYs92IidGw,8297
 odoo/addons/upgrade_analysis/i18n/es_AR.po,sha256=-YEVyBWFRo-zlhetYhVNY7UEOVJ8jMupvB8Wnmab-Eo,21729
 odoo/addons/upgrade_analysis/i18n/fr.po,sha256=xJ7BoW6ECLVdZ16y2Mkx9UKKCg908RX-mya-ujdY0II,19394
 odoo/addons/upgrade_analysis/i18n/upgrade_analysis.pot,sha256=734gkxUCJftNZDDpZwY72jMURStqFssecT0K2eq6MD0,19158
 odoo/addons/upgrade_analysis/models/__init__.py,sha256=V3z7qRHAST0ArkG6eGCgABdDHniOvY7Mcna8I4M5duk,163
@@ -22,15 +22,15 @@
 odoo/addons/upgrade_analysis/odoo_patch/odoo/__init__.py,sha256=P0ZkY7Ql1glqQNYEitW3cJFlD89_uz1Dg7FXW_QuSjE,84
 odoo/addons/upgrade_analysis/odoo_patch/odoo/models.py,sha256=BhN0_2AMJMI_PqmqnjTGTp2ZsJd-KC9zNSlB__YZrKI,739
 odoo/addons/upgrade_analysis/odoo_patch/odoo/addons/__init__.py,sha256=9pIQnc7H3xgVNpi7n3I18hg04S4IkX5mnAfl9cv7RBE,19
 odoo/addons/upgrade_analysis/odoo_patch/odoo/addons/base/__init__.py,sha256=X9EJGOE2GtZbS0G82PtSXmWSZ_R8jEM0rlJTDliQjp4,21
 odoo/addons/upgrade_analysis/odoo_patch/odoo/addons/base/models/__init__.py,sha256=V8hR-ja8zu7sRkJuB9_inZfZFWYcwxeQvG6GVWyN_yg,23
 odoo/addons/upgrade_analysis/odoo_patch/odoo/addons/base/models/ir_model.py,sha256=w28WshZ2DEcHec555-r6uBqOii75aklfqSBirDOPjdI,1482
 odoo/addons/upgrade_analysis/odoo_patch/odoo/modules/__init__.py,sha256=ZMVa5M4OJIjWngqfYFqhva1pLHhv-TrO-FUtSs7Zwzs,23
-odoo/addons/upgrade_analysis/odoo_patch/odoo/modules/registry.py,sha256=r1cyPVsGXXx6rkEiKb9f47guY1-4rH-wUwkSywy6YME,1032
+odoo/addons/upgrade_analysis/odoo_patch/odoo/modules/registry.py,sha256=VpujgZkFhccw0iVIIsMc85mnlXspUQf-sEgNaYo_Y3g,1112
 odoo/addons/upgrade_analysis/odoo_patch/odoo/tools/__init__.py,sha256=zJUx6tg2hBfTh6fQkU4JtHhC_0WRgfr81PIVua4SMA0,22
 odoo/addons/upgrade_analysis/odoo_patch/odoo/tools/convert.py,sha256=LinbMWmbr_G8KMfaNLyQAIL71thuH7YlSLCFGrNBrFk,397
 odoo/addons/upgrade_analysis/readme/CONTRIBUTORS.rst,sha256=40ZZbhFjmQBvBE1i_ISe1pQBFrDt7o-0i22_XsG2aaU,308
 odoo/addons/upgrade_analysis/readme/DESCRIPTION.rst,sha256=fTmsisjHxmm9Q5XjYJzS2I0C89_tHb6xlKv4HPbFf3o,675
 odoo/addons/upgrade_analysis/readme/ROADMAP.rst,sha256=sYjmNy1G_Ff37KIyZ1kqeLSPdQAG5xIEfrsU6kIaJbU,263
 odoo/addons/upgrade_analysis/readme/USAGE.rst,sha256=V8paWY9hBt0qz60d4UOVJRPtCiCR2aFxnCxRqwM7SiA,71
 odoo/addons/upgrade_analysis/security/ir.model.access.csv,sha256=72UaOy9pjuAUMUICrj9cYpBBm65CbHSrn3WrgxNQ7Uc,696
@@ -44,11 +44,11 @@
 odoo/addons/upgrade_analysis/views/view_upgrade_comparison_config.xml,sha256=pBTVmGOGkohO1tguxKFXAWGHkrSVJdok3jjuhERcGa4,2826
 odoo/addons/upgrade_analysis/views/view_upgrade_record.xml,sha256=oBxhlkz42bJxhrFMydpKpEDYt1sX0Z9WMipuA5Bpq2M,2834
 odoo/addons/upgrade_analysis/wizards/__init__.py,sha256=6973yn8jkeAaHm-ofIILbHUCB6KQ7RUMSDCK0Xk18xE,82
 odoo/addons/upgrade_analysis/wizards/upgrade_generate_record_wizard.py,sha256=DTeLN_1rez_v82EA16H2Bsk4TGk9aA_n7Wn6_qQoKUE,4527
 odoo/addons/upgrade_analysis/wizards/upgrade_install_wizard.py,sha256=4g8E1EdR83R84hGVWHx45JVjnz8naQlBfvHNj5bNE6Q,4040
 odoo/addons/upgrade_analysis/wizards/view_upgrade_generate_record_wizard.xml,sha256=80IblSl5Jux1jYoh0bJGBJikNRk39HDgiRylMWPdkJo,1787
 odoo/addons/upgrade_analysis/wizards/view_upgrade_install_wizard.xml,sha256=_6uw3NVhdBp_gP5mybo--AI97n3_v6tIcyX2Z0WoCrE,3289
-odoo_addon_upgrade_analysis-16.0.1.0.0.5.dist-info/METADATA,sha256=6nEQrP-mB2pZ-ELvlWY0eRu78Rq-MhiRCWM7sC8phk4,5095
-odoo_addon_upgrade_analysis-16.0.1.0.0.5.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-odoo_addon_upgrade_analysis-16.0.1.0.0.5.dist-info/top_level.txt,sha256=qBj40grFkGOfDZ2WDSw3y1RnDlgG0u8rP8pvGNdbz4w,5
-odoo_addon_upgrade_analysis-16.0.1.0.0.5.dist-info/RECORD,,
+odoo_addon_upgrade_analysis-16.0.1.0.1.dist-info/METADATA,sha256=vURFSRPnJIq6BXGn-td8-g_vcRyighNcDzo7HAIpzP4,5093
+odoo_addon_upgrade_analysis-16.0.1.0.1.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+odoo_addon_upgrade_analysis-16.0.1.0.1.dist-info/top_level.txt,sha256=qBj40grFkGOfDZ2WDSw3y1RnDlgG0u8rP8pvGNdbz4w,5
+odoo_addon_upgrade_analysis-16.0.1.0.1.dist-info/RECORD,,
```

