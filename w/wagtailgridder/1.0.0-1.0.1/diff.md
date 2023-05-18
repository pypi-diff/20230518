# Comparing `tmp/wagtailgridder-1.0.0.tar.gz` & `tmp/wagtailgridder-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/wagtailgridder-1.0.0.tar", last modified: Mon Nov 14 21:31:08 2022, max compression
+gzip compressed data, was "dist/wagtailgridder-1.0.1.tar", last modified: Tue Nov 15 19:51:15 2022, max compression
```

## Comparing `wagtailgridder-1.0.0.tar` & `wagtailgridder-1.0.1.tar`

### file list

```diff
@@ -1,58 +1,58 @@
-drwx------   0 tallen   (86646) wrds     (60359)        0 2022-11-14 21:31:08.477378 wagtailgridder-1.0.0/
--rw-------   0 tallen   (86646) wrds     (60359)      344 2022-01-19 22:07:18.000000 wagtailgridder-1.0.0/.gitignore
--rw-------   0 tallen   (86646) wrds     (60359)     1577 2022-01-19 22:07:18.000000 wagtailgridder-1.0.0/LICENSE
--rw-------   0 tallen   (86646) wrds     (60359)      121 2022-01-19 22:07:17.000000 wagtailgridder-1.0.0/MANIFEST.in
--rw-------   0 tallen   (86646) wrds     (60359)     7203 2022-11-14 21:31:08.477378 wagtailgridder-1.0.0/PKG-INFO
--rw-------   0 tallen   (86646) wrds     (60359)     5173 2022-11-14 21:30:01.000000 wagtailgridder-1.0.0/README.md
-drwx------   0 tallen   (86646) wrds     (60359)        0 2022-11-14 21:31:08.435378 wagtailgridder-1.0.0/img/
--rw-------   0 tallen   (86646) wrds     (60359)    59774 2022-01-19 22:07:18.000000 wagtailgridder-1.0.0/img/edit_grid_index_page.jpg
--rw-------   0 tallen   (86646) wrds     (60359)    63538 2022-01-19 22:07:18.000000 wagtailgridder-1.0.0/img/edit_grid_item.jpg
--rw-------   0 tallen   (86646) wrds     (60359)   180893 2022-01-19 22:07:18.000000 wagtailgridder-1.0.0/img/featured_hero.jpg
--rw-------   0 tallen   (86646) wrds     (60359)   251725 2022-01-19 22:07:18.000000 wagtailgridder-1.0.0/img/grid_index_page.jpg
--rw-------   0 tallen   (86646) wrds     (60359)   229302 2022-01-19 22:07:18.000000 wagtailgridder-1.0.0/img/grid_index_page_expanded.jpg
--rw-------   0 tallen   (86646) wrds     (60359)    50821 2022-01-19 22:07:18.000000 wagtailgridder-1.0.0/img/grid_item.jpg
--rw-------   0 tallen   (86646) wrds     (60359)       38 2022-11-14 21:31:08.477378 wagtailgridder-1.0.0/setup.cfg
--rw-------   0 tallen   (86646) wrds     (60359)     1497 2022-11-14 21:30:01.000000 wagtailgridder-1.0.0/setup.py
-drwx------   0 tallen   (86646) wrds     (60359)        0 2022-11-14 21:31:08.444378 wagtailgridder-1.0.0/wagtailgridder/
--rw-------   0 tallen   (86646) wrds     (60359)        0 2022-01-19 22:07:31.000000 wagtailgridder-1.0.0/wagtailgridder/__init__.py
--rw-------   0 tallen   (86646) wrds     (60359)     1722 2022-11-14 21:30:01.000000 wagtailgridder-1.0.0/wagtailgridder/blocks.py
-drwx------   0 tallen   (86646) wrds     (60359)        0 2022-11-14 21:31:08.452378 wagtailgridder-1.0.0/wagtailgridder/migrations/
--rw-------   0 tallen   (86646) wrds     (60359)    21904 2022-11-14 21:30:01.000000 wagtailgridder-1.0.0/wagtailgridder/migrations/0001_squashed_0012_auto_20170607_1317.py
--rw-------   0 tallen   (86646) wrds     (60359)     1005 2022-11-14 21:30:01.000000 wagtailgridder-1.0.0/wagtailgridder/migrations/0002_auto_20180220_1101.py
--rw-------   0 tallen   (86646) wrds     (60359)      601 2022-11-14 21:30:01.000000 wagtailgridder-1.0.0/wagtailgridder/migrations/0003_alter_griditemtag_tag.py
--rw-------   0 tallen   (86646) wrds     (60359)     1076 2022-11-14 21:30:01.000000 wagtailgridder-1.0.0/wagtailgridder/migrations/0004_alter_griditem_buttons.py
--rw-------   0 tallen   (86646) wrds     (60359)        0 2022-01-19 22:07:31.000000 wagtailgridder-1.0.0/wagtailgridder/migrations/__init__.py
--rw-------   0 tallen   (86646) wrds     (60359)     9075 2022-11-14 21:30:01.000000 wagtailgridder-1.0.0/wagtailgridder/models.py
--rw-------   0 tallen   (86646) wrds     (60359)      685 2022-01-19 22:07:31.000000 wagtailgridder-1.0.0/wagtailgridder/settings.py
-drwx------   0 tallen   (86646) wrds     (60359)        0 2022-11-14 21:31:08.423378 wagtailgridder-1.0.0/wagtailgridder/static/
-drwx------   0 tallen   (86646) wrds     (60359)        0 2022-11-14 21:31:08.423378 wagtailgridder-1.0.0/wagtailgridder/static/wagtailgridder/
-drwx------   0 tallen   (86646) wrds     (60359)        0 2022-11-14 21:31:08.459378 wagtailgridder-1.0.0/wagtailgridder/static/wagtailgridder/css/
--rw-------   0 tallen   (86646) wrds     (60359)     9260 2022-01-19 22:07:30.000000 wagtailgridder-1.0.0/wagtailgridder/static/wagtailgridder/css/grid_index_page.css
--rw-------   0 tallen   (86646) wrds     (60359)      463 2022-01-19 22:07:30.000000 wagtailgridder-1.0.0/wagtailgridder/static/wagtailgridder/css/jquery.gridder.min.css
--rw-------   0 tallen   (86646) wrds     (60359)      596 2022-01-19 22:07:30.000000 wagtailgridder-1.0.0/wagtailgridder/static/wagtailgridder/css/jquery.gridder.min.css.map
-drwx------   0 tallen   (86646) wrds     (60359)        0 2022-11-14 21:31:08.466378 wagtailgridder-1.0.0/wagtailgridder/static/wagtailgridder/js/
--rw-------   0 tallen   (86646) wrds     (60359)     3754 2022-01-19 22:07:30.000000 wagtailgridder-1.0.0/wagtailgridder/static/wagtailgridder/js/jquery.gridder.min.js
--rw-------   0 tallen   (86646) wrds     (60359)    28935 2022-01-19 22:07:30.000000 wagtailgridder-1.0.0/wagtailgridder/static/wagtailgridder/js/jquery.mixitup.min.js
-drwx------   0 tallen   (86646) wrds     (60359)        0 2022-11-14 21:31:08.472378 wagtailgridder-1.0.0/wagtailgridder/templates/
--rw-------   0 tallen   (86646) wrds     (60359)     1087 2022-01-19 22:07:31.000000 wagtailgridder-1.0.0/wagtailgridder/templates/base.html
-drwx------   0 tallen   (86646) wrds     (60359)        0 2022-11-14 21:31:08.475378 wagtailgridder-1.0.0/wagtailgridder/templates/wagtailgridder/
-drwx------   0 tallen   (86646) wrds     (60359)        0 2022-11-14 21:31:08.476378 wagtailgridder-1.0.0/wagtailgridder/templates/wagtailgridder/blocks/
--rw-------   0 tallen   (86646) wrds     (60359)      294 2022-01-19 22:07:31.000000 wagtailgridder-1.0.0/wagtailgridder/templates/wagtailgridder/blocks/button_section.html
--rw-------   0 tallen   (86646) wrds     (60359)       95 2022-01-19 22:07:31.000000 wagtailgridder-1.0.0/wagtailgridder/templates/wagtailgridder/blocks/document_action_item.html
--rw-------   0 tallen   (86646) wrds     (60359)        8 2022-01-19 22:07:31.000000 wagtailgridder-1.0.0/wagtailgridder/templates/wagtailgridder/blocks/placeholder_action_item.html
--rw-------   0 tallen   (86646) wrds     (60359)       86 2022-01-19 22:07:31.000000 wagtailgridder-1.0.0/wagtailgridder/templates/wagtailgridder/blocks/url_action_item.html
--rw-------   0 tallen   (86646) wrds     (60359)     1347 2022-04-04 20:15:40.000000 wagtailgridder-1.0.0/wagtailgridder/templates/wagtailgridder/grid_index_page.html
--rw-------   0 tallen   (86646) wrds     (60359)     1459 2022-01-19 22:07:31.000000 wagtailgridder-1.0.0/wagtailgridder/templates/wagtailgridder/grid_item.html
-drwx------   0 tallen   (86646) wrds     (60359)        0 2022-11-14 21:31:08.476378 wagtailgridder-1.0.0/wagtailgridder/templates/wagtailgridder/index/
--rw-------   0 tallen   (86646) wrds     (60359)     2922 2022-01-19 22:07:31.000000 wagtailgridder-1.0.0/wagtailgridder/templates/wagtailgridder/index/__extra_footer_js.html
--rw-------   0 tallen   (86646) wrds     (60359)     1536 2022-01-19 22:07:31.000000 wagtailgridder-1.0.0/wagtailgridder/templates/wagtailgridder/index/__extra_head_bottom.html
--rw-------   0 tallen   (86646) wrds     (60359)     3637 2022-01-19 22:07:31.000000 wagtailgridder-1.0.0/wagtailgridder/templates/wagtailgridder/index/__hero_section.html
--rw-------   0 tallen   (86646) wrds     (60359)     6943 2022-01-19 22:07:31.000000 wagtailgridder-1.0.0/wagtailgridder/templates/wagtailgridder/index/__wg-content-container.html
--rw-------   0 tallen   (86646) wrds     (60359)     2742 2022-11-14 21:30:01.000000 wagtailgridder-1.0.0/wagtailgridder/wagtail_hooks.py
-drwx------   0 tallen   (86646) wrds     (60359)        0 2022-11-14 21:31:08.451378 wagtailgridder-1.0.0/wagtailgridder.egg-info/
--rw-------   0 tallen   (86646) wrds     (60359)     7203 2022-11-14 21:31:08.000000 wagtailgridder-1.0.0/wagtailgridder.egg-info/PKG-INFO
--rw-------   0 tallen   (86646) wrds     (60359)     1863 2022-11-14 21:31:08.000000 wagtailgridder-1.0.0/wagtailgridder.egg-info/SOURCES.txt
--rw-------   0 tallen   (86646) wrds     (60359)        1 2022-11-14 21:31:08.000000 wagtailgridder-1.0.0/wagtailgridder.egg-info/dependency_links.txt
--rw-------   0 tallen   (86646) wrds     (60359)        1 2022-01-19 22:07:18.000000 wagtailgridder-1.0.0/wagtailgridder.egg-info/not-zip-safe
--rw-------   0 tallen   (86646) wrds     (60359)       13 2022-11-14 21:31:08.000000 wagtailgridder-1.0.0/wagtailgridder.egg-info/requires.txt
--rw-------   0 tallen   (86646) wrds     (60359)       15 2022-11-14 21:31:08.000000 wagtailgridder-1.0.0/wagtailgridder.egg-info/top_level.txt
+drwx------   0 tallen   (86646) wrds     (60359)        0 2022-11-15 19:51:15.774372 wagtailgridder-1.0.1/
+-rw-------   0 tallen   (86646) wrds     (60359)      344 2022-01-19 22:07:18.000000 wagtailgridder-1.0.1/.gitignore
+-rw-------   0 tallen   (86646) wrds     (60359)     1577 2022-01-19 22:07:18.000000 wagtailgridder-1.0.1/LICENSE
+-rw-------   0 tallen   (86646) wrds     (60359)      121 2022-01-19 22:07:17.000000 wagtailgridder-1.0.1/MANIFEST.in
+-rw-------   0 tallen   (86646) wrds     (60359)     7203 2022-11-15 19:51:15.774372 wagtailgridder-1.0.1/PKG-INFO
+-rw-------   0 tallen   (86646) wrds     (60359)     5173 2022-11-14 21:30:01.000000 wagtailgridder-1.0.1/README.md
+drwx------   0 tallen   (86646) wrds     (60359)        0 2022-11-15 19:51:15.770372 wagtailgridder-1.0.1/img/
+-rw-------   0 tallen   (86646) wrds     (60359)    59774 2022-01-19 22:07:18.000000 wagtailgridder-1.0.1/img/edit_grid_index_page.jpg
+-rw-------   0 tallen   (86646) wrds     (60359)    63538 2022-01-19 22:07:18.000000 wagtailgridder-1.0.1/img/edit_grid_item.jpg
+-rw-------   0 tallen   (86646) wrds     (60359)   180893 2022-01-19 22:07:18.000000 wagtailgridder-1.0.1/img/featured_hero.jpg
+-rw-------   0 tallen   (86646) wrds     (60359)   251725 2022-01-19 22:07:18.000000 wagtailgridder-1.0.1/img/grid_index_page.jpg
+-rw-------   0 tallen   (86646) wrds     (60359)   229302 2022-01-19 22:07:18.000000 wagtailgridder-1.0.1/img/grid_index_page_expanded.jpg
+-rw-------   0 tallen   (86646) wrds     (60359)    50821 2022-01-19 22:07:18.000000 wagtailgridder-1.0.1/img/grid_item.jpg
+-rw-------   0 tallen   (86646) wrds     (60359)       38 2022-11-15 19:51:15.774372 wagtailgridder-1.0.1/setup.cfg
+-rw-------   0 tallen   (86646) wrds     (60359)     1497 2022-11-14 21:30:01.000000 wagtailgridder-1.0.1/setup.py
+drwx------   0 tallen   (86646) wrds     (60359)        0 2022-11-15 19:51:15.771372 wagtailgridder-1.0.1/wagtailgridder/
+-rw-------   0 tallen   (86646) wrds     (60359)        0 2022-01-19 22:07:31.000000 wagtailgridder-1.0.1/wagtailgridder/__init__.py
+-rw-------   0 tallen   (86646) wrds     (60359)     1722 2022-11-14 21:30:01.000000 wagtailgridder-1.0.1/wagtailgridder/blocks.py
+drwx------   0 tallen   (86646) wrds     (60359)        0 2022-11-15 19:51:15.772372 wagtailgridder-1.0.1/wagtailgridder/migrations/
+-rw-------   0 tallen   (86646) wrds     (60359)    21904 2022-11-14 21:30:01.000000 wagtailgridder-1.0.1/wagtailgridder/migrations/0001_squashed_0012_auto_20170607_1317.py
+-rw-------   0 tallen   (86646) wrds     (60359)     1005 2022-11-14 21:30:01.000000 wagtailgridder-1.0.1/wagtailgridder/migrations/0002_auto_20180220_1101.py
+-rw-------   0 tallen   (86646) wrds     (60359)      601 2022-11-14 21:30:01.000000 wagtailgridder-1.0.1/wagtailgridder/migrations/0003_alter_griditemtag_tag.py
+-rw-------   0 tallen   (86646) wrds     (60359)     1076 2022-11-14 21:30:01.000000 wagtailgridder-1.0.1/wagtailgridder/migrations/0004_alter_griditem_buttons.py
+-rw-------   0 tallen   (86646) wrds     (60359)        0 2022-01-19 22:07:31.000000 wagtailgridder-1.0.1/wagtailgridder/migrations/__init__.py
+-rw-------   0 tallen   (86646) wrds     (60359)     8968 2022-11-15 19:45:34.000000 wagtailgridder-1.0.1/wagtailgridder/models.py
+-rw-------   0 tallen   (86646) wrds     (60359)      685 2022-01-19 22:07:31.000000 wagtailgridder-1.0.1/wagtailgridder/settings.py
+drwx------   0 tallen   (86646) wrds     (60359)        0 2022-11-15 19:51:15.768372 wagtailgridder-1.0.1/wagtailgridder/static/
+drwx------   0 tallen   (86646) wrds     (60359)        0 2022-11-15 19:51:15.768372 wagtailgridder-1.0.1/wagtailgridder/static/wagtailgridder/
+drwx------   0 tallen   (86646) wrds     (60359)        0 2022-11-15 19:51:15.772372 wagtailgridder-1.0.1/wagtailgridder/static/wagtailgridder/css/
+-rw-------   0 tallen   (86646) wrds     (60359)     9260 2022-01-19 22:07:30.000000 wagtailgridder-1.0.1/wagtailgridder/static/wagtailgridder/css/grid_index_page.css
+-rw-------   0 tallen   (86646) wrds     (60359)      463 2022-01-19 22:07:30.000000 wagtailgridder-1.0.1/wagtailgridder/static/wagtailgridder/css/jquery.gridder.min.css
+-rw-------   0 tallen   (86646) wrds     (60359)      596 2022-01-19 22:07:30.000000 wagtailgridder-1.0.1/wagtailgridder/static/wagtailgridder/css/jquery.gridder.min.css.map
+drwx------   0 tallen   (86646) wrds     (60359)        0 2022-11-15 19:51:15.772372 wagtailgridder-1.0.1/wagtailgridder/static/wagtailgridder/js/
+-rw-------   0 tallen   (86646) wrds     (60359)     3754 2022-01-19 22:07:30.000000 wagtailgridder-1.0.1/wagtailgridder/static/wagtailgridder/js/jquery.gridder.min.js
+-rw-------   0 tallen   (86646) wrds     (60359)    28935 2022-01-19 22:07:30.000000 wagtailgridder-1.0.1/wagtailgridder/static/wagtailgridder/js/jquery.mixitup.min.js
+drwx------   0 tallen   (86646) wrds     (60359)        0 2022-11-15 19:51:15.773372 wagtailgridder-1.0.1/wagtailgridder/templates/
+-rw-------   0 tallen   (86646) wrds     (60359)     1087 2022-01-19 22:07:31.000000 wagtailgridder-1.0.1/wagtailgridder/templates/base.html
+drwx------   0 tallen   (86646) wrds     (60359)        0 2022-11-15 19:51:15.773372 wagtailgridder-1.0.1/wagtailgridder/templates/wagtailgridder/
+drwx------   0 tallen   (86646) wrds     (60359)        0 2022-11-15 19:51:15.773372 wagtailgridder-1.0.1/wagtailgridder/templates/wagtailgridder/blocks/
+-rw-------   0 tallen   (86646) wrds     (60359)      294 2022-01-19 22:07:31.000000 wagtailgridder-1.0.1/wagtailgridder/templates/wagtailgridder/blocks/button_section.html
+-rw-------   0 tallen   (86646) wrds     (60359)       95 2022-01-19 22:07:31.000000 wagtailgridder-1.0.1/wagtailgridder/templates/wagtailgridder/blocks/document_action_item.html
+-rw-------   0 tallen   (86646) wrds     (60359)        8 2022-01-19 22:07:31.000000 wagtailgridder-1.0.1/wagtailgridder/templates/wagtailgridder/blocks/placeholder_action_item.html
+-rw-------   0 tallen   (86646) wrds     (60359)       86 2022-01-19 22:07:31.000000 wagtailgridder-1.0.1/wagtailgridder/templates/wagtailgridder/blocks/url_action_item.html
+-rw-------   0 tallen   (86646) wrds     (60359)     1347 2022-04-04 20:15:40.000000 wagtailgridder-1.0.1/wagtailgridder/templates/wagtailgridder/grid_index_page.html
+-rw-------   0 tallen   (86646) wrds     (60359)     1459 2022-01-19 22:07:31.000000 wagtailgridder-1.0.1/wagtailgridder/templates/wagtailgridder/grid_item.html
+drwx------   0 tallen   (86646) wrds     (60359)        0 2022-11-15 19:51:15.774372 wagtailgridder-1.0.1/wagtailgridder/templates/wagtailgridder/index/
+-rw-------   0 tallen   (86646) wrds     (60359)     2922 2022-01-19 22:07:31.000000 wagtailgridder-1.0.1/wagtailgridder/templates/wagtailgridder/index/__extra_footer_js.html
+-rw-------   0 tallen   (86646) wrds     (60359)     1536 2022-01-19 22:07:31.000000 wagtailgridder-1.0.1/wagtailgridder/templates/wagtailgridder/index/__extra_head_bottom.html
+-rw-------   0 tallen   (86646) wrds     (60359)     3637 2022-01-19 22:07:31.000000 wagtailgridder-1.0.1/wagtailgridder/templates/wagtailgridder/index/__hero_section.html
+-rw-------   0 tallen   (86646) wrds     (60359)     6943 2022-01-19 22:07:31.000000 wagtailgridder-1.0.1/wagtailgridder/templates/wagtailgridder/index/__wg-content-container.html
+-rw-------   0 tallen   (86646) wrds     (60359)     2742 2022-11-14 21:30:01.000000 wagtailgridder-1.0.1/wagtailgridder/wagtail_hooks.py
+drwx------   0 tallen   (86646) wrds     (60359)        0 2022-11-15 19:51:15.771372 wagtailgridder-1.0.1/wagtailgridder.egg-info/
+-rw-------   0 tallen   (86646) wrds     (60359)     7203 2022-11-15 19:51:15.000000 wagtailgridder-1.0.1/wagtailgridder.egg-info/PKG-INFO
+-rw-------   0 tallen   (86646) wrds     (60359)     1863 2022-11-15 19:51:15.000000 wagtailgridder-1.0.1/wagtailgridder.egg-info/SOURCES.txt
+-rw-------   0 tallen   (86646) wrds     (60359)        1 2022-11-15 19:51:15.000000 wagtailgridder-1.0.1/wagtailgridder.egg-info/dependency_links.txt
+-rw-------   0 tallen   (86646) wrds     (60359)        1 2022-01-19 22:07:18.000000 wagtailgridder-1.0.1/wagtailgridder.egg-info/not-zip-safe
+-rw-------   0 tallen   (86646) wrds     (60359)       13 2022-11-15 19:51:15.000000 wagtailgridder-1.0.1/wagtailgridder.egg-info/requires.txt
+-rw-------   0 tallen   (86646) wrds     (60359)       15 2022-11-15 19:51:15.000000 wagtailgridder-1.0.1/wagtailgridder.egg-info/top_level.txt
```

### Comparing `wagtailgridder-1.0.0/LICENSE` & `wagtailgridder-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `wagtailgridder-1.0.0/PKG-INFO` & `wagtailgridder-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wagtailgridder
-Version: 1.0.0
+Version: 1.0.1
 Summary: Gridder layout for the Django CMS Wagtail.
 Home-page: https://github.com/wharton/wagtailgridder
 Author: Timothy Allen
 Author-email: tallen@wharton.upenn.edu
 License: UNKNOWN
 Description: # Wagtail Gridder
```

### Comparing `wagtailgridder-1.0.0/README.md` & `wagtailgridder-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `wagtailgridder-1.0.0/img/edit_grid_index_page.jpg` & `wagtailgridder-1.0.1/img/edit_grid_index_page.jpg`

 * *Files identical despite different names*

### Comparing `wagtailgridder-1.0.0/img/edit_grid_item.jpg` & `wagtailgridder-1.0.1/img/edit_grid_item.jpg`

 * *Files identical despite different names*

### Comparing `wagtailgridder-1.0.0/img/featured_hero.jpg` & `wagtailgridder-1.0.1/img/featured_hero.jpg`

 * *Files identical despite different names*

### Comparing `wagtailgridder-1.0.0/img/grid_index_page.jpg` & `wagtailgridder-1.0.1/img/grid_index_page.jpg`

 * *Files identical despite different names*

### Comparing `wagtailgridder-1.0.0/img/grid_index_page_expanded.jpg` & `wagtailgridder-1.0.1/img/grid_index_page_expanded.jpg`

 * *Files identical despite different names*

### Comparing `wagtailgridder-1.0.0/img/grid_item.jpg` & `wagtailgridder-1.0.1/img/grid_item.jpg`

 * *Files identical despite different names*

### Comparing `wagtailgridder-1.0.0/setup.py` & `wagtailgridder-1.0.1/setup.py`

 * *Files identical despite different names*

### Comparing `wagtailgridder-1.0.0/wagtailgridder/blocks.py` & `wagtailgridder-1.0.1/wagtailgridder/blocks.py`

 * *Files identical despite different names*

### Comparing `wagtailgridder-1.0.0/wagtailgridder/migrations/0001_squashed_0012_auto_20170607_1317.py` & `wagtailgridder-1.0.1/wagtailgridder/migrations/0001_squashed_0012_auto_20170607_1317.py`

 * *Files identical despite different names*

### Comparing `wagtailgridder-1.0.0/wagtailgridder/migrations/0002_auto_20180220_1101.py` & `wagtailgridder-1.0.1/wagtailgridder/migrations/0002_auto_20180220_1101.py`

 * *Files identical despite different names*

### Comparing `wagtailgridder-1.0.0/wagtailgridder/migrations/0003_alter_griditemtag_tag.py` & `wagtailgridder-1.0.1/wagtailgridder/migrations/0003_alter_griditemtag_tag.py`

 * *Files identical despite different names*

### Comparing `wagtailgridder-1.0.0/wagtailgridder/migrations/0004_alter_griditem_buttons.py` & `wagtailgridder-1.0.1/wagtailgridder/migrations/0004_alter_griditem_buttons.py`

 * *Files identical despite different names*

### Comparing `wagtailgridder-1.0.0/wagtailgridder/models.py` & `wagtailgridder-1.0.1/wagtailgridder/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 from django.db import models
 from django.forms import CheckboxSelectMultiple
 from django.utils import timezone
 
 from wagtail.fields import StreamField, RichTextField
 from wagtail.models import Page, Orderable
 from wagtail.admin.panels import FieldPanel, InlinePanel, MultiFieldPanel
-from wagtail.images.edit_handlers import ImageChooserPanel
 from wagtail.search import index
 
 from modelcluster.fields import ParentalKey, ParentalManyToManyField
 from modelcluster.tags import ClusterTaggableManager
 from taggit.models import TaggedItemBase
 
 from .blocks import ButtonBlock
@@ -99,20 +98,20 @@
     search_fields = Page.search_fields + [
         index.SearchField("summary_text"),
         index.SearchField("description_text"),
         index.SearchField("landing_page_text"),
     ]
 
     CARD_PANELS = [
-        ImageChooserPanel("summary_image"),
+        FieldPanel("summary_image"),
         FieldPanel("summary_text"),
     ]
 
     DETAIL_PANELS = [
-        ImageChooserPanel("description_image"),
+        FieldPanel("description_image"),
         FieldPanel("description_text"),
         FieldPanel("description_video"),
         FieldPanel("landing_page_text"),
     ]
 
     META_PANELS = [
         FieldPanel("tags"),
@@ -138,15 +137,15 @@
             heading="Metadata",
             classname="collapsible",
         ),
     ]
 
     def save(self, *args, **kwargs):
         self.modified = timezone.now()
-        super(GridItem, self).save(*args, **kwargs)
+        super().save(*args, **kwargs)
 
 
 class GridIndexGridItemRelationship(Orderable, models.Model):
     """
     Allows the content creator to associate Grid Items on a
     Grid Index Page.
     """
@@ -276,16 +275,16 @@
     HERO_PANELS = [
         FieldPanel("hero_background_image"),
         FieldPanel("hero_logo_image"),
         FieldPanel("hero_description"),
         FieldPanel("hero_button_text"),
         FieldPanel("hero_button_url"),
         FieldPanel("featured_description"),
-        FieldPanel("featured_grid_item_1", GridItem),
-        FieldPanel("featured_grid_item_2", GridItem),
+        FieldPanel("featured_grid_item_1"),
+        FieldPanel("featured_grid_item_2"),
     ]
 
     content_panels = Page.content_panels + [
         MultiFieldPanel(
             HERO_PANELS,
             heading="Hero Section (Optional)",
             classname="collapsible collapsed",
```

### Comparing `wagtailgridder-1.0.0/wagtailgridder/settings.py` & `wagtailgridder-1.0.1/wagtailgridder/settings.py`

 * *Files identical despite different names*

### Comparing `wagtailgridder-1.0.0/wagtailgridder/static/wagtailgridder/css/grid_index_page.css` & `wagtailgridder-1.0.1/wagtailgridder/static/wagtailgridder/css/grid_index_page.css`

 * *Files identical despite different names*

### Comparing `wagtailgridder-1.0.0/wagtailgridder/static/wagtailgridder/css/jquery.gridder.min.css.map` & `wagtailgridder-1.0.1/wagtailgridder/static/wagtailgridder/css/jquery.gridder.min.css.map`

 * *Files identical despite different names*

### Comparing `wagtailgridder-1.0.0/wagtailgridder/static/wagtailgridder/js/jquery.gridder.min.js` & `wagtailgridder-1.0.1/wagtailgridder/static/wagtailgridder/js/jquery.gridder.min.js`

 * *Files identical despite different names*

### Comparing `wagtailgridder-1.0.0/wagtailgridder/static/wagtailgridder/js/jquery.mixitup.min.js` & `wagtailgridder-1.0.1/wagtailgridder/static/wagtailgridder/js/jquery.mixitup.min.js`

 * *Files identical despite different names*

### Comparing `wagtailgridder-1.0.0/wagtailgridder/templates/base.html` & `wagtailgridder-1.0.1/wagtailgridder/templates/base.html`

 * *Files identical despite different names*

### Comparing `wagtailgridder-1.0.0/wagtailgridder/templates/wagtailgridder/grid_index_page.html` & `wagtailgridder-1.0.1/wagtailgridder/templates/wagtailgridder/grid_index_page.html`

 * *Files identical despite different names*

### Comparing `wagtailgridder-1.0.0/wagtailgridder/templates/wagtailgridder/grid_item.html` & `wagtailgridder-1.0.1/wagtailgridder/templates/wagtailgridder/grid_item.html`

 * *Files identical despite different names*

### Comparing `wagtailgridder-1.0.0/wagtailgridder/templates/wagtailgridder/index/__extra_footer_js.html` & `wagtailgridder-1.0.1/wagtailgridder/templates/wagtailgridder/index/__extra_footer_js.html`

 * *Files identical despite different names*

### Comparing `wagtailgridder-1.0.0/wagtailgridder/templates/wagtailgridder/index/__extra_head_bottom.html` & `wagtailgridder-1.0.1/wagtailgridder/templates/wagtailgridder/index/__extra_head_bottom.html`

 * *Files identical despite different names*

### Comparing `wagtailgridder-1.0.0/wagtailgridder/templates/wagtailgridder/index/__hero_section.html` & `wagtailgridder-1.0.1/wagtailgridder/templates/wagtailgridder/index/__hero_section.html`

 * *Files identical despite different names*

### Comparing `wagtailgridder-1.0.0/wagtailgridder/templates/wagtailgridder/index/__wg-content-container.html` & `wagtailgridder-1.0.1/wagtailgridder/templates/wagtailgridder/index/__wg-content-container.html`

 * *Files identical despite different names*

### Comparing `wagtailgridder-1.0.0/wagtailgridder/wagtail_hooks.py` & `wagtailgridder-1.0.1/wagtailgridder/wagtail_hooks.py`

 * *Files identical despite different names*

### Comparing `wagtailgridder-1.0.0/wagtailgridder.egg-info/PKG-INFO` & `wagtailgridder-1.0.1/wagtailgridder.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wagtailgridder
-Version: 1.0.0
+Version: 1.0.1
 Summary: Gridder layout for the Django CMS Wagtail.
 Home-page: https://github.com/wharton/wagtailgridder
 Author: Timothy Allen
 Author-email: tallen@wharton.upenn.edu
 License: UNKNOWN
 Description: # Wagtail Gridder
```

### Comparing `wagtailgridder-1.0.0/wagtailgridder.egg-info/SOURCES.txt` & `wagtailgridder-1.0.1/wagtailgridder.egg-info/SOURCES.txt`

 * *Files identical despite different names*

