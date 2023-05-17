# Comparing `tmp/collective.documentviewer-6.0.2.tar.gz` & `tmp/collective.documentviewer-6.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "collective.documentviewer-6.0.2.tar", last modified: Thu Apr 27 08:54:08 2023, max compression
+gzip compressed data, was "collective.documentviewer-6.0.3.tar", last modified: Wed May 17 21:58:49 2023, max compression
```

## Comparing `collective.documentviewer-6.0.2.tar` & `collective.documentviewer-6.0.3.tar`

### file list

```diff
@@ -1,155 +1,155 @@
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-27 08:54:08.604399 collective.documentviewer-6.0.2/
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-27 08:54:08.567917 collective.documentviewer-6.0.2/.tx/
--rw-r--r--   0 maurits    (501) staff       (20)      542 2023-04-27 08:54:08.000000 collective.documentviewer-6.0.2/.tx/config
--rw-r--r--   0 maurits    (501) staff       (20)    10353 2023-04-27 08:54:08.000000 collective.documentviewer-6.0.2/CENTOS-INSTALL.rst
--rw-r--r--   0 maurits    (501) staff       (20)     3081 2023-04-27 08:54:08.000000 collective.documentviewer-6.0.2/DEBIAN-INSTALL.rst
--rw-r--r--   0 maurits    (501) staff       (20)     2559 2023-04-27 08:54:08.000000 collective.documentviewer-6.0.2/Gruntfile.js
--rw-r--r--   0 maurits    (501) staff       (20)      200 2023-04-27 08:54:08.000000 collective.documentviewer-6.0.2/MANIFEST.in
--rw-r--r--   0 maurits    (501) staff       (20)       65 2023-04-27 08:54:08.000000 collective.documentviewer-6.0.2/Makefile
--rw-r--r--   0 maurits    (501) staff       (20)    19308 2023-04-27 08:54:08.604533 collective.documentviewer-6.0.2/PKG-INFO
--rw-r--r--   0 maurits    (501) staff       (20)     7156 2023-04-27 08:54:08.000000 collective.documentviewer-6.0.2/README.rst
--rw-r--r--   0 maurits    (501) staff       (20)     2789 2023-04-27 08:54:08.000000 collective.documentviewer-6.0.2/_cleanup_file_storage.py
--rw-r--r--   0 maurits    (501) staff       (20)      651 2023-04-27 08:54:08.000000 collective.documentviewer-6.0.2/buildout.cfg
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-27 08:54:08.568169 collective.documentviewer-6.0.2/collective/
--rw-r--r--   0 maurits    (501) staff       (20)      244 2023-04-27 08:54:08.000000 collective.documentviewer-6.0.2/collective/__init__.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-27 08:54:08.577549 collective.documentviewer-6.0.2/collective/documentviewer/
--rw-r--r--   0 maurits    (501) staff       (20)      346 2023-04-27 08:54:08.000000 collective.documentviewer-6.0.2/collective/documentviewer/CUSTOMIZATIONS.txt
--rw-r--r--   0 maurits    (501) staff       (20)    15532 2023-04-27 08:54:08.000000 collective.documentviewer-6.0.2/collective/documentviewer/ISO-639-2_utf-8.txt
--rw-r--r--   0 maurits    (501) staff       (20)      182 2023-04-27 08:54:08.000000 collective.documentviewer-6.0.2/collective/documentviewer/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)     2298 2023-04-27 08:54:08.000000 collective.documentviewer-6.0.2/collective/documentviewer/adapters.py
--rw-r--r--   0 maurits    (501) staff       (20)     3085 2023-04-27 08:54:08.000000 collective.documentviewer-6.0.2/collective/documentviewer/async_utils.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-27 08:54:08.579598 collective.documentviewer-6.0.2/collective/documentviewer/browser/
--rw-r--r--   0 maurits    (501) staff       (20)        0 2023-04-27 08:54:08.000000 collective.documentviewer-6.0.2/collective/documentviewer/browser/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)     3380 2023-04-27 08:54:08.000000 collective.documentviewer-6.0.2/collective/documentviewer/browser/configure.zcml
--rw-r--r--   0 maurits    (501) staff       (20)     1205 2023-04-27 08:54:08.000000 collective.documentviewer-6.0.2/collective/documentviewer/browser/controlpanel.py
--rw-r--r--   0 maurits    (501) staff       (20)     1330 2023-04-27 08:54:08.000000 collective.documentviewer-6.0.2/collective/documentviewer/browser/settings.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-27 08:54:08.580937 collective.documentviewer-6.0.2/collective/documentviewer/browser/templates/
--rw-r--r--   0 maurits    (501) staff       (20)     2602 2023-04-27 08:54:08.000000 collective.documentviewer-6.0.2/collective/documentviewer/browser/templates/async-monitor.pt
--rw-r--r--   0 maurits    (501) staff       (20)     2155 2023-04-27 08:54:08.000000 collective.documentviewer-6.0.2/collective/documentviewer/browser/templates/converting.pt
--rw-r--r--   0 maurits    (501) staff       (20)     1972 2023-04-27 08:54:08.000000 collective.documentviewer-6.0.2/collective/documentviewer/browser/templates/documentviewer.pt
--rw-r--r--   0 maurits    (501) staff       (20)     4363 2023-04-27 08:54:08.000000 collective.documentviewer-6.0.2/collective/documentviewer/browser/templates/group-view.pt
--rw-r--r--   0 maurits    (501) staff       (20)     6475 2023-04-27 08:54:08.000000 collective.documentviewer-6.0.2/collective/documentviewer/browser/traverse.py
--rw-r--r--   0 maurits    (501) staff       (20)    17638 2023-04-27 08:54:08.000000 collective.documentviewer-6.0.2/collective/documentviewer/browser/views.py
--rw-r--r--   0 maurits    (501) staff       (20)      808 2023-04-27 08:54:08.000000 collective.documentviewer-6.0.2/collective/documentviewer/catalog.py
--rw-r--r--   0 maurits    (501) staff       (20)     1545 2023-04-27 08:54:08.000000 collective.documentviewer-6.0.2/collective/documentviewer/config.py
--rw-r--r--   0 maurits    (501) staff       (20)     2632 2023-04-27 08:54:08.000000 collective.documentviewer-6.0.2/collective/documentviewer/configure.zcml
--rw-r--r--   0 maurits    (501) staff       (20)    28388 2023-04-27 08:54:08.000000 collective.documentviewer-6.0.2/collective/documentviewer/convert.py
--rw-r--r--   0 maurits    (501) staff       (20)     1900 2023-04-27 08:54:08.000000 collective.documentviewer-6.0.2/collective/documentviewer/convert_all.py
--rw-r--r--   0 maurits    (501) staff       (20)      341 2023-04-27 08:54:08.000000 collective.documentviewer-6.0.2/collective/documentviewer/events.py
--rw-r--r--   0 maurits    (501) staff       (20)    10445 2023-04-27 08:54:08.000000 collective.documentviewer-6.0.2/collective/documentviewer/interfaces.py
--rw-r--r--   0 maurits    (501) staff       (20)      998 2023-04-27 08:54:08.000000 collective.documentviewer-6.0.2/collective/documentviewer/iso639_2_utf8.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-27 08:54:08.582739 collective.documentviewer-6.0.2/collective/documentviewer/locales/
--rw-r--r--   0 maurits    (501) staff       (20)     1838 2023-04-27 08:54:08.000000 collective.documentviewer-6.0.2/collective/documentviewer/locales/collective.documentviewer-manual.pot
--rw-r--r--   0 maurits    (501) staff       (20)    10823 2023-04-27 08:54:08.000000 collective.documentviewer-6.0.2/collective/documentviewer/locales/collective.documentviewer.pot
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-27 08:54:08.559424 collective.documentviewer-6.0.2/collective/documentviewer/locales/de/
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-27 08:54:08.583389 collective.documentviewer-6.0.2/collective/documentviewer/locales/de/LC_MESSAGES/
--rw-r--r--   0 maurits    (501) staff       (20)    19398 2023-04-27 08:54:08.000000 collective.documentviewer-6.0.2/collective/documentviewer/locales/de/LC_MESSAGES/collective.documentviewer.po
--rw-r--r--   0 maurits    (501) staff       (20)     1534 2023-04-27 08:54:08.000000 collective.documentviewer-6.0.2/collective/documentviewer/locales/de/LC_MESSAGES/plone.po
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-27 08:54:08.559697 collective.documentviewer-6.0.2/collective/documentviewer/locales/en/
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-27 08:54:08.584183 collective.documentviewer-6.0.2/collective/documentviewer/locales/en/LC_MESSAGES/
--rw-r--r--   0 maurits    (501) staff       (20)    14916 2023-04-27 08:54:08.000000 collective.documentviewer-6.0.2/collective/documentviewer/locales/en/LC_MESSAGES/collective.documentviewer.po
--rw-r--r--   0 maurits    (501) staff       (20)     1482 2023-04-27 08:54:08.000000 collective.documentviewer-6.0.2/collective/documentviewer/locales/en/LC_MESSAGES/plone.po
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-27 08:54:08.559997 collective.documentviewer-6.0.2/collective/documentviewer/locales/es/
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-27 08:54:08.584933 collective.documentviewer-6.0.2/collective/documentviewer/locales/es/LC_MESSAGES/
--rw-r--r--   0 maurits    (501) staff       (20)    20787 2023-04-27 08:54:08.000000 collective.documentviewer-6.0.2/collective/documentviewer/locales/es/LC_MESSAGES/collective.documentviewer.po
--rw-r--r--   0 maurits    (501) staff       (20)     2098 2023-04-27 08:54:08.000000 collective.documentviewer-6.0.2/collective/documentviewer/locales/es/LC_MESSAGES/plone.po
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-27 08:54:08.560296 collective.documentviewer-6.0.2/collective/documentviewer/locales/eu/
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-27 08:54:08.585694 collective.documentviewer-6.0.2/collective/documentviewer/locales/eu/LC_MESSAGES/
--rw-r--r--   0 maurits    (501) staff       (20)    19077 2023-04-27 08:54:08.000000 collective.documentviewer-6.0.2/collective/documentviewer/locales/eu/LC_MESSAGES/collective.documentviewer.po
--rw-r--r--   0 maurits    (501) staff       (20)     1571 2023-04-27 08:54:08.000000 collective.documentviewer-6.0.2/collective/documentviewer/locales/eu/LC_MESSAGES/plone.po
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-27 08:54:08.560673 collective.documentviewer-6.0.2/collective/documentviewer/locales/fr/
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-27 08:54:08.586363 collective.documentviewer-6.0.2/collective/documentviewer/locales/fr/LC_MESSAGES/
--rw-r--r--   0 maurits    (501) staff       (20)    19941 2023-04-27 08:54:08.000000 collective.documentviewer-6.0.2/collective/documentviewer/locales/fr/LC_MESSAGES/collective.documentviewer.po
--rw-r--r--   0 maurits    (501) staff       (20)     1534 2023-04-27 08:54:08.000000 collective.documentviewer-6.0.2/collective/documentviewer/locales/fr/LC_MESSAGES/plone.po
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-27 08:54:08.560971 collective.documentviewer-6.0.2/collective/documentviewer/locales/it/
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-27 08:54:08.587020 collective.documentviewer-6.0.2/collective/documentviewer/locales/it/LC_MESSAGES/
--rw-r--r--   0 maurits    (501) staff       (20)    15443 2023-04-27 08:54:08.000000 collective.documentviewer-6.0.2/collective/documentviewer/locales/it/LC_MESSAGES/collective.documentviewer.po
--rw-r--r--   0 maurits    (501) staff       (20)     1547 2023-04-27 08:54:08.000000 collective.documentviewer-6.0.2/collective/documentviewer/locales/it/LC_MESSAGES/plone.po
--rw-r--r--   0 maurits    (501) staff       (20)      528 2023-04-27 08:54:08.000000 collective.documentviewer-6.0.2/collective/documentviewer/locales/plone-manual.pot
--rw-r--r--   0 maurits    (501) staff       (20)     1495 2023-04-27 08:54:08.000000 collective.documentviewer-6.0.2/collective/documentviewer/locales/plone.pot
--rwxr-xr-x   0 maurits    (501) staff       (20)     2242 2023-04-27 08:54:08.000000 collective.documentviewer-6.0.2/collective/documentviewer/locales/rebuild_i18n.sh
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-27 08:54:08.561248 collective.documentviewer-6.0.2/collective/documentviewer/locales/zh_CN/
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-27 08:54:08.587720 collective.documentviewer-6.0.2/collective/documentviewer/locales/zh_CN/LC_MESSAGES/
--rw-r--r--   0 maurits    (501) staff       (20)    14994 2023-04-27 08:54:08.000000 collective.documentviewer-6.0.2/collective/documentviewer/locales/zh_CN/LC_MESSAGES/collective.documentviewer.po
--rw-r--r--   0 maurits    (501) staff       (20)     1532 2023-04-27 08:54:08.000000 collective.documentviewer-6.0.2/collective/documentviewer/locales/zh_CN/LC_MESSAGES/plone.po
--rw-r--r--   0 maurits    (501) staff       (20)     1221 2023-04-27 08:54:08.000000 collective.documentviewer-6.0.2/collective/documentviewer/migration.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-27 08:54:08.561952 collective.documentviewer-6.0.2/collective/documentviewer/profiles/
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-27 08:54:08.589271 collective.documentviewer-6.0.2/collective/documentviewer/profiles/default/
--rw-r--r--   0 maurits    (501) staff       (20)     1549 2023-04-27 08:54:08.000000 collective.documentviewer-6.0.2/collective/documentviewer/profiles/default/actions.xml
--rw-r--r--   0 maurits    (501) staff       (20)      194 2023-04-27 08:54:08.000000 collective.documentviewer-6.0.2/collective/documentviewer/profiles/default/browserlayer.xml
--rw-r--r--   0 maurits    (501) staff       (20)     1134 2023-04-27 08:54:08.000000 collective.documentviewer-6.0.2/collective/documentviewer/profiles/default/controlpanel.xml
--rw-r--r--   0 maurits    (501) staff       (20)       71 2023-04-27 08:54:08.000000 collective.documentviewer-6.0.2/collective/documentviewer/profiles/default/metadata.xml
--rw-r--r--   0 maurits    (501) staff       (20)      456 2023-04-27 08:54:08.000000 collective.documentviewer-6.0.2/collective/documentviewer/profiles/default/registry.xml
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-27 08:54:08.589606 collective.documentviewer-6.0.2/collective/documentviewer/profiles/default/types/
--rw-r--r--   0 maurits    (501) staff       (20)      289 2023-04-27 08:54:08.000000 collective.documentviewer-6.0.2/collective/documentviewer/profiles/default/types/File.xml
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-27 08:54:08.590690 collective.documentviewer-6.0.2/collective/documentviewer/profiles/uninstall/
--rw-r--r--   0 maurits    (501) staff       (20)      504 2023-04-27 08:54:08.000000 collective.documentviewer-6.0.2/collective/documentviewer/profiles/uninstall/actions.xml
--rw-r--r--   0 maurits    (501) staff       (20)      151 2023-04-27 08:54:08.000000 collective.documentviewer-6.0.2/collective/documentviewer/profiles/uninstall/browserlayer.xml
--rw-r--r--   0 maurits    (501) staff       (20)      275 2023-04-27 08:54:08.000000 collective.documentviewer-6.0.2/collective/documentviewer/profiles/uninstall/registry.xml
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-27 08:54:08.562736 collective.documentviewer-6.0.2/collective/documentviewer/resources/
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-27 08:54:08.594475 collective.documentviewer-6.0.2/collective/documentviewer/resources/assets/
--rw-r--r--   0 maurits    (501) staff       (20)    55721 2023-04-27 08:54:08.000000 collective.documentviewer-6.0.2/collective/documentviewer/resources/assets/fallback-datauri.css
--rw-r--r--   0 maurits    (501) staff       (20)    36966 2023-04-27 08:54:08.000000 collective.documentviewer-6.0.2/collective/documentviewer/resources/assets/fallback.css
--rw-r--r--   0 maurits    (501) staff       (20)     2055 2023-04-27 08:54:08.000000 collective.documentviewer-6.0.2/collective/documentviewer/resources/assets/plain-datauri.css
--rw-r--r--   0 maurits    (501) staff       (20)     2055 2023-04-27 08:54:08.000000 collective.documentviewer-6.0.2/collective/documentviewer/resources/assets/plain.css
--rw-r--r--   0 maurits    (501) staff       (20)      143 2023-04-27 08:54:08.000000 collective.documentviewer-6.0.2/collective/documentviewer/resources/assets/print-datauri.css
--rw-r--r--   0 maurits    (501) staff       (20)      143 2023-04-27 08:54:08.000000 collective.documentviewer-6.0.2/collective/documentviewer/resources/assets/print.css
--rw-r--r--   0 maurits    (501) staff       (20)      143 2023-04-27 08:54:08.000000 collective.documentviewer-6.0.2/collective/documentviewer/resources/assets/printviewer.css
--rw-r--r--   0 maurits    (501) staff       (20)    17636 2023-04-27 08:54:08.000000 collective.documentviewer-6.0.2/collective/documentviewer/resources/assets/templates.js
--rw-r--r--   0 maurits    (501) staff       (20)    76295 2023-04-27 08:54:08.000000 collective.documentviewer-6.0.2/collective/documentviewer/resources/assets/viewer-datauri.css
--rw-r--r--   0 maurits    (501) staff       (20)    39563 2023-04-27 08:54:08.000000 collective.documentviewer-6.0.2/collective/documentviewer/resources/assets/viewer.css
--rw-r--r--   0 maurits    (501) staff       (20)   270143 2023-04-27 08:54:08.000000 collective.documentviewer-6.0.2/collective/documentviewer/resources/assets/viewer.js
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-27 08:54:08.596197 collective.documentviewer-6.0.2/collective/documentviewer/resources/images/
--rwxr-xr-x   0 maurits    (501) staff       (20)     1117 2023-04-27 08:54:08.000000 collective.documentviewer-6.0.2/collective/documentviewer/resources/images/application-pdf.png
--rw-r--r--   0 maurits    (501) staff       (20)      541 2023-04-27 08:54:08.000000 collective.documentviewer-6.0.2/collective/documentviewer/resources/images/clear.png
--rw-r--r--   0 maurits    (501) staff       (20)     9927 2023-04-27 08:54:08.000000 collective.documentviewer-6.0.2/collective/documentviewer/resources/images/pdf.png
--rw-r--r--   0 maurits    (501) staff       (20)      420 2023-04-27 08:54:08.000000 collective.documentviewer-6.0.2/collective/documentviewer/resources/images/search.png
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-27 08:54:08.598479 collective.documentviewer-6.0.2/collective/documentviewer/resources/javascripts/
--rw-r--r--   0 maurits    (501) staff       (20)   452712 2023-04-27 08:54:08.000000 collective.documentviewer-6.0.2/collective/documentviewer/resources/javascripts/build.min.js
--rw-r--r--   0 maurits    (501) staff       (20)   291433 2023-04-27 08:54:08.000000 collective.documentviewer-6.0.2/collective/documentviewer/resources/javascripts/build.min.js.map
--rw-r--r--   0 maurits    (501) staff       (20)      955 2023-04-27 08:54:08.000000 collective.documentviewer-6.0.2/collective/documentviewer/resources/javascripts/group.js
--rw-r--r--   0 maurits    (501) staff       (20)      591 2023-04-27 08:54:08.000000 collective.documentviewer-6.0.2/collective/documentviewer/resources/javascripts/viewer.js
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-27 08:54:08.599682 collective.documentviewer-6.0.2/collective/documentviewer/resources/stylesheets/
--rw-r--r--   0 maurits    (501) staff       (20)     1254 2023-04-27 08:54:08.000000 collective.documentviewer-6.0.2/collective/documentviewer/resources/stylesheets/group.css
--rw-r--r--   0 maurits    (501) staff       (20)      399 2023-04-27 08:54:08.000000 collective.documentviewer-6.0.2/collective/documentviewer/resources/stylesheets/viewer.css
--rw-r--r--   0 maurits    (501) staff       (20)      714 2023-04-27 08:54:08.000000 collective.documentviewer-6.0.2/collective/documentviewer/resources/stylesheets/viewer.css.map
--rw-r--r--   0 maurits    (501) staff       (20)      388 2023-04-27 08:54:08.000000 collective.documentviewer-6.0.2/collective/documentviewer/resources/stylesheets/viewer.less
--rw-r--r--   0 maurits    (501) staff       (20)     1620 2023-04-27 08:54:08.000000 collective.documentviewer-6.0.2/collective/documentviewer/settings.py
--rw-r--r--   0 maurits    (501) staff       (20)     2514 2023-04-27 08:54:08.000000 collective.documentviewer-6.0.2/collective/documentviewer/setuphandlers.py
--rw-r--r--   0 maurits    (501) staff       (20)     1084 2023-04-27 08:54:08.000000 collective.documentviewer-6.0.2/collective/documentviewer/storage.py
--rw-r--r--   0 maurits    (501) staff       (20)     3241 2023-04-27 08:54:08.000000 collective.documentviewer-6.0.2/collective/documentviewer/subscribers.py
--rw-r--r--   0 maurits    (501) staff       (20)     1610 2023-04-27 08:54:08.000000 collective.documentviewer-6.0.2/collective/documentviewer/testing.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-27 08:54:08.601246 collective.documentviewer-6.0.2/collective/documentviewer/tests/
--rw-r--r--   0 maurits    (501) staff       (20)     1252 2023-04-27 08:54:08.000000 collective.documentviewer-6.0.2/collective/documentviewer/tests/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)     8035 2023-04-27 08:54:08.000000 collective.documentviewer-6.0.2/collective/documentviewer/tests/test_convert.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-27 08:54:08.602271 collective.documentviewer-6.0.2/collective/documentviewer/tests/test_files/
--rw-r--r--   0 maurits    (501) staff       (20)    10752 2023-04-27 08:54:08.000000 collective.documentviewer-6.0.2/collective/documentviewer/tests/test_files/test.doc
--rw-r--r--   0 maurits    (501) staff       (20)    12842 2023-04-27 08:54:08.000000 collective.documentviewer-6.0.2/collective/documentviewer/tests/test_files/test.odp
--rw-r--r--   0 maurits    (501) staff       (20)     6365 2023-04-27 08:54:08.000000 collective.documentviewer-6.0.2/collective/documentviewer/tests/test_files/test.pdf
--rw-r--r--   0 maurits    (501) staff       (20)     2459 2023-04-27 08:54:08.000000 collective.documentviewer-6.0.2/collective/documentviewer/tests/test_migrate.py
--rw-r--r--   0 maurits    (501) staff       (20)     5961 2023-04-27 08:54:08.000000 collective.documentviewer-6.0.2/collective/documentviewer/tests/test_storage.py
--rw-r--r--   0 maurits    (501) staff       (20)     4905 2023-04-27 08:54:08.000000 collective.documentviewer-6.0.2/collective/documentviewer/tests/test_views.py
--rw-r--r--   0 maurits    (501) staff       (20)     4600 2023-04-27 08:54:08.000000 collective.documentviewer-6.0.2/collective/documentviewer/upgrades.py
--rw-r--r--   0 maurits    (501) staff       (20)     1750 2023-04-27 08:54:08.000000 collective.documentviewer-6.0.2/collective/documentviewer/upgrades.zcml
--rw-r--r--   0 maurits    (501) staff       (20)     1012 2023-04-27 08:54:08.000000 collective.documentviewer-6.0.2/collective/documentviewer/utils.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-27 08:54:08.570583 collective.documentviewer-6.0.2/collective.documentviewer.egg-info/
--rw-r--r--   0 maurits    (501) staff       (20)    19308 2023-04-27 08:54:08.000000 collective.documentviewer-6.0.2/collective.documentviewer.egg-info/PKG-INFO
--rw-r--r--   0 maurits    (501) staff       (20)     5589 2023-04-27 08:54:08.000000 collective.documentviewer-6.0.2/collective.documentviewer.egg-info/SOURCES.txt
--rw-r--r--   0 maurits    (501) staff       (20)        1 2023-04-27 08:54:08.000000 collective.documentviewer-6.0.2/collective.documentviewer.egg-info/dependency_links.txt
--rw-r--r--   0 maurits    (501) staff       (20)      111 2023-04-27 08:54:08.000000 collective.documentviewer-6.0.2/collective.documentviewer.egg-info/entry_points.txt
--rw-r--r--   0 maurits    (501) staff       (20)       11 2023-04-27 08:54:08.000000 collective.documentviewer-6.0.2/collective.documentviewer.egg-info/namespace_packages.txt
--rw-r--r--   0 maurits    (501) staff       (20)        1 2023-04-27 08:54:08.000000 collective.documentviewer-6.0.2/collective.documentviewer.egg-info/not-zip-safe
--rw-r--r--   0 maurits    (501) staff       (20)      245 2023-04-27 08:54:08.000000 collective.documentviewer-6.0.2/collective.documentviewer.egg-info/requires.txt
--rw-r--r--   0 maurits    (501) staff       (20)       11 2023-04-27 08:54:08.000000 collective.documentviewer-6.0.2/collective.documentviewer.egg-info/top_level.txt
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-27 08:54:08.603642 collective.documentviewer-6.0.2/docs/
--rw-r--r--   0 maurits    (501) staff       (20)    11108 2023-04-27 08:54:08.000000 collective.documentviewer-6.0.2/docs/HISTORY.txt
--rw-r--r--   0 maurits    (501) staff       (20)     1557 2023-04-27 08:54:08.000000 collective.documentviewer-6.0.2/docs/INSTALL.txt
--rw-r--r--   0 maurits    (501) staff       (20)    17987 2023-04-27 08:54:08.000000 collective.documentviewer-6.0.2/docs/LICENSE.GPL
--rw-r--r--   0 maurits    (501) staff       (20)      742 2023-04-27 08:54:08.000000 collective.documentviewer-6.0.2/docs/LICENSE.txt
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-27 08:54:08.604011 collective.documentviewer-6.0.2/docs/_static/
--rw-r--r--   0 maurits    (501) staff       (20)    26670 2023-04-27 08:54:08.000000 collective.documentviewer-6.0.2/docs/_static/wildcardcorp_logo.png
--rw-r--r--   0 maurits    (501) staff       (20)      424 2023-04-27 08:54:08.000000 collective.documentviewer-6.0.2/package.json
--rw-r--r--   0 maurits    (501) staff       (20)       62 2023-04-27 08:54:08.000000 collective.documentviewer-6.0.2/requirements.txt
--rw-r--r--   0 maurits    (501) staff       (20)      225 2023-04-27 08:54:08.605023 collective.documentviewer-6.0.2/setup.cfg
--rw-r--r--   0 maurits    (501) staff       (20)     2260 2023-04-27 08:54:08.000000 collective.documentviewer-6.0.2/setup.py
--rw-r--r--   0 maurits    (501) staff       (20)       51 2023-04-27 08:54:08.000000 collective.documentviewer-6.0.2/travis.cfg
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-17 21:58:49.914318 collective.documentviewer-6.0.3/
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-17 21:58:49.865035 collective.documentviewer-6.0.3/.tx/
+-rw-r--r--   0 maurits    (501) staff       (20)      542 2023-05-17 21:58:49.000000 collective.documentviewer-6.0.3/.tx/config
+-rw-r--r--   0 maurits    (501) staff       (20)    10353 2023-05-17 21:58:49.000000 collective.documentviewer-6.0.3/CENTOS-INSTALL.rst
+-rw-r--r--   0 maurits    (501) staff       (20)     3081 2023-05-17 21:58:49.000000 collective.documentviewer-6.0.3/DEBIAN-INSTALL.rst
+-rw-r--r--   0 maurits    (501) staff       (20)     2559 2023-05-17 21:58:49.000000 collective.documentviewer-6.0.3/Gruntfile.js
+-rw-r--r--   0 maurits    (501) staff       (20)      200 2023-05-17 21:58:49.000000 collective.documentviewer-6.0.3/MANIFEST.in
+-rw-r--r--   0 maurits    (501) staff       (20)       65 2023-05-17 21:58:49.000000 collective.documentviewer-6.0.3/Makefile
+-rw-r--r--   0 maurits    (501) staff       (20)    19466 2023-05-17 21:58:49.914511 collective.documentviewer-6.0.3/PKG-INFO
+-rw-r--r--   0 maurits    (501) staff       (20)     7156 2023-05-17 21:58:49.000000 collective.documentviewer-6.0.3/README.rst
+-rw-r--r--   0 maurits    (501) staff       (20)     2789 2023-05-17 21:58:49.000000 collective.documentviewer-6.0.3/_cleanup_file_storage.py
+-rw-r--r--   0 maurits    (501) staff       (20)      651 2023-05-17 21:58:49.000000 collective.documentviewer-6.0.3/buildout.cfg
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-17 21:58:49.865461 collective.documentviewer-6.0.3/collective/
+-rw-r--r--   0 maurits    (501) staff       (20)      244 2023-05-17 21:58:49.000000 collective.documentviewer-6.0.3/collective/__init__.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-17 21:58:49.878529 collective.documentviewer-6.0.3/collective/documentviewer/
+-rw-r--r--   0 maurits    (501) staff       (20)      346 2023-05-17 21:58:49.000000 collective.documentviewer-6.0.3/collective/documentviewer/CUSTOMIZATIONS.txt
+-rw-r--r--   0 maurits    (501) staff       (20)    15532 2023-05-17 21:58:49.000000 collective.documentviewer-6.0.3/collective/documentviewer/ISO-639-2_utf-8.txt
+-rw-r--r--   0 maurits    (501) staff       (20)      182 2023-05-17 21:58:49.000000 collective.documentviewer-6.0.3/collective/documentviewer/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2298 2023-05-17 21:58:49.000000 collective.documentviewer-6.0.3/collective/documentviewer/adapters.py
+-rw-r--r--   0 maurits    (501) staff       (20)     3085 2023-05-17 21:58:49.000000 collective.documentviewer-6.0.3/collective/documentviewer/async_utils.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-17 21:58:49.881114 collective.documentviewer-6.0.3/collective/documentviewer/browser/
+-rw-r--r--   0 maurits    (501) staff       (20)        0 2023-05-17 21:58:49.000000 collective.documentviewer-6.0.3/collective/documentviewer/browser/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)     3380 2023-05-17 21:58:49.000000 collective.documentviewer-6.0.3/collective/documentviewer/browser/configure.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)     1205 2023-05-17 21:58:49.000000 collective.documentviewer-6.0.3/collective/documentviewer/browser/controlpanel.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1330 2023-05-17 21:58:49.000000 collective.documentviewer-6.0.3/collective/documentviewer/browser/settings.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-17 21:58:49.883076 collective.documentviewer-6.0.3/collective/documentviewer/browser/templates/
+-rw-r--r--   0 maurits    (501) staff       (20)     2602 2023-05-17 21:58:49.000000 collective.documentviewer-6.0.3/collective/documentviewer/browser/templates/async-monitor.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     2155 2023-05-17 21:58:49.000000 collective.documentviewer-6.0.3/collective/documentviewer/browser/templates/converting.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     1972 2023-05-17 21:58:49.000000 collective.documentviewer-6.0.3/collective/documentviewer/browser/templates/documentviewer.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     4363 2023-05-17 21:58:49.000000 collective.documentviewer-6.0.3/collective/documentviewer/browser/templates/group-view.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     6475 2023-05-17 21:58:49.000000 collective.documentviewer-6.0.3/collective/documentviewer/browser/traverse.py
+-rw-r--r--   0 maurits    (501) staff       (20)    17638 2023-05-17 21:58:49.000000 collective.documentviewer-6.0.3/collective/documentviewer/browser/views.py
+-rw-r--r--   0 maurits    (501) staff       (20)      808 2023-05-17 21:58:49.000000 collective.documentviewer-6.0.3/collective/documentviewer/catalog.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1545 2023-05-17 21:58:49.000000 collective.documentviewer-6.0.3/collective/documentviewer/config.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2632 2023-05-17 21:58:49.000000 collective.documentviewer-6.0.3/collective/documentviewer/configure.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)    28851 2023-05-17 21:58:49.000000 collective.documentviewer-6.0.3/collective/documentviewer/convert.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1900 2023-05-17 21:58:49.000000 collective.documentviewer-6.0.3/collective/documentviewer/convert_all.py
+-rw-r--r--   0 maurits    (501) staff       (20)      341 2023-05-17 21:58:49.000000 collective.documentviewer-6.0.3/collective/documentviewer/events.py
+-rw-r--r--   0 maurits    (501) staff       (20)    10445 2023-05-17 21:58:49.000000 collective.documentviewer-6.0.3/collective/documentviewer/interfaces.py
+-rw-r--r--   0 maurits    (501) staff       (20)      998 2023-05-17 21:58:49.000000 collective.documentviewer-6.0.3/collective/documentviewer/iso639_2_utf8.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-17 21:58:49.885350 collective.documentviewer-6.0.3/collective/documentviewer/locales/
+-rw-r--r--   0 maurits    (501) staff       (20)     1838 2023-05-17 21:58:49.000000 collective.documentviewer-6.0.3/collective/documentviewer/locales/collective.documentviewer-manual.pot
+-rw-r--r--   0 maurits    (501) staff       (20)    10823 2023-05-17 21:58:49.000000 collective.documentviewer-6.0.3/collective/documentviewer/locales/collective.documentviewer.pot
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-17 21:58:49.853084 collective.documentviewer-6.0.3/collective/documentviewer/locales/de/
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-17 21:58:49.886298 collective.documentviewer-6.0.3/collective/documentviewer/locales/de/LC_MESSAGES/
+-rw-r--r--   0 maurits    (501) staff       (20)    19398 2023-05-17 21:58:49.000000 collective.documentviewer-6.0.3/collective/documentviewer/locales/de/LC_MESSAGES/collective.documentviewer.po
+-rw-r--r--   0 maurits    (501) staff       (20)     1534 2023-05-17 21:58:49.000000 collective.documentviewer-6.0.3/collective/documentviewer/locales/de/LC_MESSAGES/plone.po
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-17 21:58:49.853539 collective.documentviewer-6.0.3/collective/documentviewer/locales/en/
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-17 21:58:49.887201 collective.documentviewer-6.0.3/collective/documentviewer/locales/en/LC_MESSAGES/
+-rw-r--r--   0 maurits    (501) staff       (20)    14916 2023-05-17 21:58:49.000000 collective.documentviewer-6.0.3/collective/documentviewer/locales/en/LC_MESSAGES/collective.documentviewer.po
+-rw-r--r--   0 maurits    (501) staff       (20)     1482 2023-05-17 21:58:49.000000 collective.documentviewer-6.0.3/collective/documentviewer/locales/en/LC_MESSAGES/plone.po
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-17 21:58:49.854002 collective.documentviewer-6.0.3/collective/documentviewer/locales/es/
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-17 21:58:49.888172 collective.documentviewer-6.0.3/collective/documentviewer/locales/es/LC_MESSAGES/
+-rw-r--r--   0 maurits    (501) staff       (20)    20787 2023-05-17 21:58:49.000000 collective.documentviewer-6.0.3/collective/documentviewer/locales/es/LC_MESSAGES/collective.documentviewer.po
+-rw-r--r--   0 maurits    (501) staff       (20)     2098 2023-05-17 21:58:49.000000 collective.documentviewer-6.0.3/collective/documentviewer/locales/es/LC_MESSAGES/plone.po
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-17 21:58:49.854468 collective.documentviewer-6.0.3/collective/documentviewer/locales/eu/
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-17 21:58:49.889125 collective.documentviewer-6.0.3/collective/documentviewer/locales/eu/LC_MESSAGES/
+-rw-r--r--   0 maurits    (501) staff       (20)    19077 2023-05-17 21:58:49.000000 collective.documentviewer-6.0.3/collective/documentviewer/locales/eu/LC_MESSAGES/collective.documentviewer.po
+-rw-r--r--   0 maurits    (501) staff       (20)     1571 2023-05-17 21:58:49.000000 collective.documentviewer-6.0.3/collective/documentviewer/locales/eu/LC_MESSAGES/plone.po
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-17 21:58:49.854918 collective.documentviewer-6.0.3/collective/documentviewer/locales/fr/
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-17 21:58:49.890081 collective.documentviewer-6.0.3/collective/documentviewer/locales/fr/LC_MESSAGES/
+-rw-r--r--   0 maurits    (501) staff       (20)    19941 2023-05-17 21:58:49.000000 collective.documentviewer-6.0.3/collective/documentviewer/locales/fr/LC_MESSAGES/collective.documentviewer.po
+-rw-r--r--   0 maurits    (501) staff       (20)     1534 2023-05-17 21:58:49.000000 collective.documentviewer-6.0.3/collective/documentviewer/locales/fr/LC_MESSAGES/plone.po
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-17 21:58:49.855370 collective.documentviewer-6.0.3/collective/documentviewer/locales/it/
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-17 21:58:49.890967 collective.documentviewer-6.0.3/collective/documentviewer/locales/it/LC_MESSAGES/
+-rw-r--r--   0 maurits    (501) staff       (20)    15443 2023-05-17 21:58:49.000000 collective.documentviewer-6.0.3/collective/documentviewer/locales/it/LC_MESSAGES/collective.documentviewer.po
+-rw-r--r--   0 maurits    (501) staff       (20)     1547 2023-05-17 21:58:49.000000 collective.documentviewer-6.0.3/collective/documentviewer/locales/it/LC_MESSAGES/plone.po
+-rw-r--r--   0 maurits    (501) staff       (20)      528 2023-05-17 21:58:49.000000 collective.documentviewer-6.0.3/collective/documentviewer/locales/plone-manual.pot
+-rw-r--r--   0 maurits    (501) staff       (20)     1495 2023-05-17 21:58:49.000000 collective.documentviewer-6.0.3/collective/documentviewer/locales/plone.pot
+-rwxr-xr-x   0 maurits    (501) staff       (20)     2242 2023-05-17 21:58:49.000000 collective.documentviewer-6.0.3/collective/documentviewer/locales/rebuild_i18n.sh
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-17 21:58:49.855829 collective.documentviewer-6.0.3/collective/documentviewer/locales/zh_CN/
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-17 21:58:49.891876 collective.documentviewer-6.0.3/collective/documentviewer/locales/zh_CN/LC_MESSAGES/
+-rw-r--r--   0 maurits    (501) staff       (20)    14994 2023-05-17 21:58:49.000000 collective.documentviewer-6.0.3/collective/documentviewer/locales/zh_CN/LC_MESSAGES/collective.documentviewer.po
+-rw-r--r--   0 maurits    (501) staff       (20)     1532 2023-05-17 21:58:49.000000 collective.documentviewer-6.0.3/collective/documentviewer/locales/zh_CN/LC_MESSAGES/plone.po
+-rw-r--r--   0 maurits    (501) staff       (20)     1221 2023-05-17 21:58:49.000000 collective.documentviewer-6.0.3/collective/documentviewer/migration.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-17 21:58:49.856824 collective.documentviewer-6.0.3/collective/documentviewer/profiles/
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-17 21:58:49.894098 collective.documentviewer-6.0.3/collective/documentviewer/profiles/default/
+-rw-r--r--   0 maurits    (501) staff       (20)     1549 2023-05-17 21:58:49.000000 collective.documentviewer-6.0.3/collective/documentviewer/profiles/default/actions.xml
+-rw-r--r--   0 maurits    (501) staff       (20)      194 2023-05-17 21:58:49.000000 collective.documentviewer-6.0.3/collective/documentviewer/profiles/default/browserlayer.xml
+-rw-r--r--   0 maurits    (501) staff       (20)     1134 2023-05-17 21:58:49.000000 collective.documentviewer-6.0.3/collective/documentviewer/profiles/default/controlpanel.xml
+-rw-r--r--   0 maurits    (501) staff       (20)       71 2023-05-17 21:58:49.000000 collective.documentviewer-6.0.3/collective/documentviewer/profiles/default/metadata.xml
+-rw-r--r--   0 maurits    (501) staff       (20)      456 2023-05-17 21:58:49.000000 collective.documentviewer-6.0.3/collective/documentviewer/profiles/default/registry.xml
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-17 21:58:49.894550 collective.documentviewer-6.0.3/collective/documentviewer/profiles/default/types/
+-rw-r--r--   0 maurits    (501) staff       (20)      289 2023-05-17 21:58:49.000000 collective.documentviewer-6.0.3/collective/documentviewer/profiles/default/types/File.xml
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-17 21:58:49.895880 collective.documentviewer-6.0.3/collective/documentviewer/profiles/uninstall/
+-rw-r--r--   0 maurits    (501) staff       (20)      504 2023-05-17 21:58:49.000000 collective.documentviewer-6.0.3/collective/documentviewer/profiles/uninstall/actions.xml
+-rw-r--r--   0 maurits    (501) staff       (20)      151 2023-05-17 21:58:49.000000 collective.documentviewer-6.0.3/collective/documentviewer/profiles/uninstall/browserlayer.xml
+-rw-r--r--   0 maurits    (501) staff       (20)      275 2023-05-17 21:58:49.000000 collective.documentviewer-6.0.3/collective/documentviewer/profiles/uninstall/registry.xml
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-17 21:58:49.858049 collective.documentviewer-6.0.3/collective/documentviewer/resources/
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-17 21:58:49.901204 collective.documentviewer-6.0.3/collective/documentviewer/resources/assets/
+-rw-r--r--   0 maurits    (501) staff       (20)    55721 2023-05-17 21:58:49.000000 collective.documentviewer-6.0.3/collective/documentviewer/resources/assets/fallback-datauri.css
+-rw-r--r--   0 maurits    (501) staff       (20)    36966 2023-05-17 21:58:49.000000 collective.documentviewer-6.0.3/collective/documentviewer/resources/assets/fallback.css
+-rw-r--r--   0 maurits    (501) staff       (20)     2055 2023-05-17 21:58:49.000000 collective.documentviewer-6.0.3/collective/documentviewer/resources/assets/plain-datauri.css
+-rw-r--r--   0 maurits    (501) staff       (20)     2055 2023-05-17 21:58:49.000000 collective.documentviewer-6.0.3/collective/documentviewer/resources/assets/plain.css
+-rw-r--r--   0 maurits    (501) staff       (20)      143 2023-05-17 21:58:49.000000 collective.documentviewer-6.0.3/collective/documentviewer/resources/assets/print-datauri.css
+-rw-r--r--   0 maurits    (501) staff       (20)      143 2023-05-17 21:58:49.000000 collective.documentviewer-6.0.3/collective/documentviewer/resources/assets/print.css
+-rw-r--r--   0 maurits    (501) staff       (20)      143 2023-05-17 21:58:49.000000 collective.documentviewer-6.0.3/collective/documentviewer/resources/assets/printviewer.css
+-rw-r--r--   0 maurits    (501) staff       (20)    17636 2023-05-17 21:58:49.000000 collective.documentviewer-6.0.3/collective/documentviewer/resources/assets/templates.js
+-rw-r--r--   0 maurits    (501) staff       (20)    76295 2023-05-17 21:58:49.000000 collective.documentviewer-6.0.3/collective/documentviewer/resources/assets/viewer-datauri.css
+-rw-r--r--   0 maurits    (501) staff       (20)    39563 2023-05-17 21:58:49.000000 collective.documentviewer-6.0.3/collective/documentviewer/resources/assets/viewer.css
+-rw-r--r--   0 maurits    (501) staff       (20)   270143 2023-05-17 21:58:49.000000 collective.documentviewer-6.0.3/collective/documentviewer/resources/assets/viewer.js
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-17 21:58:49.903464 collective.documentviewer-6.0.3/collective/documentviewer/resources/images/
+-rwxr-xr-x   0 maurits    (501) staff       (20)     1117 2023-05-17 21:58:49.000000 collective.documentviewer-6.0.3/collective/documentviewer/resources/images/application-pdf.png
+-rw-r--r--   0 maurits    (501) staff       (20)      541 2023-05-17 21:58:49.000000 collective.documentviewer-6.0.3/collective/documentviewer/resources/images/clear.png
+-rw-r--r--   0 maurits    (501) staff       (20)     9927 2023-05-17 21:58:49.000000 collective.documentviewer-6.0.3/collective/documentviewer/resources/images/pdf.png
+-rw-r--r--   0 maurits    (501) staff       (20)      420 2023-05-17 21:58:49.000000 collective.documentviewer-6.0.3/collective/documentviewer/resources/images/search.png
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-17 21:58:49.906539 collective.documentviewer-6.0.3/collective/documentviewer/resources/javascripts/
+-rw-r--r--   0 maurits    (501) staff       (20)   452712 2023-05-17 21:58:49.000000 collective.documentviewer-6.0.3/collective/documentviewer/resources/javascripts/build.min.js
+-rw-r--r--   0 maurits    (501) staff       (20)   291433 2023-05-17 21:58:49.000000 collective.documentviewer-6.0.3/collective/documentviewer/resources/javascripts/build.min.js.map
+-rw-r--r--   0 maurits    (501) staff       (20)      955 2023-05-17 21:58:49.000000 collective.documentviewer-6.0.3/collective/documentviewer/resources/javascripts/group.js
+-rw-r--r--   0 maurits    (501) staff       (20)      591 2023-05-17 21:58:49.000000 collective.documentviewer-6.0.3/collective/documentviewer/resources/javascripts/viewer.js
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-17 21:58:49.908285 collective.documentviewer-6.0.3/collective/documentviewer/resources/stylesheets/
+-rw-r--r--   0 maurits    (501) staff       (20)     1254 2023-05-17 21:58:49.000000 collective.documentviewer-6.0.3/collective/documentviewer/resources/stylesheets/group.css
+-rw-r--r--   0 maurits    (501) staff       (20)      399 2023-05-17 21:58:49.000000 collective.documentviewer-6.0.3/collective/documentviewer/resources/stylesheets/viewer.css
+-rw-r--r--   0 maurits    (501) staff       (20)      714 2023-05-17 21:58:49.000000 collective.documentviewer-6.0.3/collective/documentviewer/resources/stylesheets/viewer.css.map
+-rw-r--r--   0 maurits    (501) staff       (20)      388 2023-05-17 21:58:49.000000 collective.documentviewer-6.0.3/collective/documentviewer/resources/stylesheets/viewer.less
+-rw-r--r--   0 maurits    (501) staff       (20)     1620 2023-05-17 21:58:49.000000 collective.documentviewer-6.0.3/collective/documentviewer/settings.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2514 2023-05-17 21:58:49.000000 collective.documentviewer-6.0.3/collective/documentviewer/setuphandlers.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1084 2023-05-17 21:58:49.000000 collective.documentviewer-6.0.3/collective/documentviewer/storage.py
+-rw-r--r--   0 maurits    (501) staff       (20)     3241 2023-05-17 21:58:49.000000 collective.documentviewer-6.0.3/collective/documentviewer/subscribers.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1610 2023-05-17 21:58:49.000000 collective.documentviewer-6.0.3/collective/documentviewer/testing.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-17 21:58:49.910423 collective.documentviewer-6.0.3/collective/documentviewer/tests/
+-rw-r--r--   0 maurits    (501) staff       (20)     1252 2023-05-17 21:58:49.000000 collective.documentviewer-6.0.3/collective/documentviewer/tests/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)     8035 2023-05-17 21:58:49.000000 collective.documentviewer-6.0.3/collective/documentviewer/tests/test_convert.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-17 21:58:49.911732 collective.documentviewer-6.0.3/collective/documentviewer/tests/test_files/
+-rw-r--r--   0 maurits    (501) staff       (20)    10752 2023-05-17 21:58:49.000000 collective.documentviewer-6.0.3/collective/documentviewer/tests/test_files/test.doc
+-rw-r--r--   0 maurits    (501) staff       (20)    12842 2023-05-17 21:58:49.000000 collective.documentviewer-6.0.3/collective/documentviewer/tests/test_files/test.odp
+-rw-r--r--   0 maurits    (501) staff       (20)     6365 2023-05-17 21:58:49.000000 collective.documentviewer-6.0.3/collective/documentviewer/tests/test_files/test.pdf
+-rw-r--r--   0 maurits    (501) staff       (20)     2459 2023-05-17 21:58:49.000000 collective.documentviewer-6.0.3/collective/documentviewer/tests/test_migrate.py
+-rw-r--r--   0 maurits    (501) staff       (20)     5961 2023-05-17 21:58:49.000000 collective.documentviewer-6.0.3/collective/documentviewer/tests/test_storage.py
+-rw-r--r--   0 maurits    (501) staff       (20)     4905 2023-05-17 21:58:49.000000 collective.documentviewer-6.0.3/collective/documentviewer/tests/test_views.py
+-rw-r--r--   0 maurits    (501) staff       (20)     4600 2023-05-17 21:58:49.000000 collective.documentviewer-6.0.3/collective/documentviewer/upgrades.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1750 2023-05-17 21:58:49.000000 collective.documentviewer-6.0.3/collective/documentviewer/upgrades.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)     1012 2023-05-17 21:58:49.000000 collective.documentviewer-6.0.3/collective/documentviewer/utils.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-17 21:58:49.869044 collective.documentviewer-6.0.3/collective.documentviewer.egg-info/
+-rw-r--r--   0 maurits    (501) staff       (20)    19466 2023-05-17 21:58:49.000000 collective.documentviewer-6.0.3/collective.documentviewer.egg-info/PKG-INFO
+-rw-r--r--   0 maurits    (501) staff       (20)     5589 2023-05-17 21:58:49.000000 collective.documentviewer-6.0.3/collective.documentviewer.egg-info/SOURCES.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        1 2023-05-17 21:58:49.000000 collective.documentviewer-6.0.3/collective.documentviewer.egg-info/dependency_links.txt
+-rw-r--r--   0 maurits    (501) staff       (20)      111 2023-05-17 21:58:49.000000 collective.documentviewer-6.0.3/collective.documentviewer.egg-info/entry_points.txt
+-rw-r--r--   0 maurits    (501) staff       (20)       11 2023-05-17 21:58:49.000000 collective.documentviewer-6.0.3/collective.documentviewer.egg-info/namespace_packages.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        1 2023-05-17 21:58:49.000000 collective.documentviewer-6.0.3/collective.documentviewer.egg-info/not-zip-safe
+-rw-r--r--   0 maurits    (501) staff       (20)      245 2023-05-17 21:58:49.000000 collective.documentviewer-6.0.3/collective.documentviewer.egg-info/requires.txt
+-rw-r--r--   0 maurits    (501) staff       (20)       11 2023-05-17 21:58:49.000000 collective.documentviewer-6.0.3/collective.documentviewer.egg-info/top_level.txt
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-17 21:58:49.913478 collective.documentviewer-6.0.3/docs/
+-rw-r--r--   0 maurits    (501) staff       (20)    11266 2023-05-17 21:58:49.000000 collective.documentviewer-6.0.3/docs/HISTORY.txt
+-rw-r--r--   0 maurits    (501) staff       (20)     1557 2023-05-17 21:58:49.000000 collective.documentviewer-6.0.3/docs/INSTALL.txt
+-rw-r--r--   0 maurits    (501) staff       (20)    17987 2023-05-17 21:58:49.000000 collective.documentviewer-6.0.3/docs/LICENSE.GPL
+-rw-r--r--   0 maurits    (501) staff       (20)      742 2023-05-17 21:58:49.000000 collective.documentviewer-6.0.3/docs/LICENSE.txt
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-17 21:58:49.913910 collective.documentviewer-6.0.3/docs/_static/
+-rw-r--r--   0 maurits    (501) staff       (20)    26670 2023-05-17 21:58:49.000000 collective.documentviewer-6.0.3/docs/_static/wildcardcorp_logo.png
+-rw-r--r--   0 maurits    (501) staff       (20)      424 2023-05-17 21:58:49.000000 collective.documentviewer-6.0.3/package.json
+-rw-r--r--   0 maurits    (501) staff       (20)       62 2023-05-17 21:58:49.000000 collective.documentviewer-6.0.3/requirements.txt
+-rw-r--r--   0 maurits    (501) staff       (20)      225 2023-05-17 21:58:49.915291 collective.documentviewer-6.0.3/setup.cfg
+-rw-r--r--   0 maurits    (501) staff       (20)     2260 2023-05-17 21:58:49.000000 collective.documentviewer-6.0.3/setup.py
+-rw-r--r--   0 maurits    (501) staff       (20)       51 2023-05-17 21:58:49.000000 collective.documentviewer-6.0.3/travis.cfg
```

### Comparing `collective.documentviewer-6.0.2/.tx/config` & `collective.documentviewer-6.0.3/.tx/config`

 * *Files identical despite different names*

### Comparing `collective.documentviewer-6.0.2/CENTOS-INSTALL.rst` & `collective.documentviewer-6.0.3/CENTOS-INSTALL.rst`

 * *Files identical despite different names*

### Comparing `collective.documentviewer-6.0.2/DEBIAN-INSTALL.rst` & `collective.documentviewer-6.0.3/DEBIAN-INSTALL.rst`

 * *Files identical despite different names*

### Comparing `collective.documentviewer-6.0.2/Gruntfile.js` & `collective.documentviewer-6.0.3/Gruntfile.js`

 * *Files identical despite different names*

### Comparing `collective.documentviewer-6.0.2/PKG-INFO` & `collective.documentviewer-6.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: collective.documentviewer
-Version: 6.0.2
+Version: 6.0.3
 Summary: Document cloud's document viewer integration into plone.
 Home-page: https://github.com/collective/collective.documentviewer
 Author: Nathan Van Gheem
 Author-email: vangheem@gmail.com
 License: GPL
 Keywords: plone documentviewer pdf ocr doc viewer
 Classifier: Development Status :: 5 - Production/Stable
@@ -300,14 +300,21 @@
 .. _Nginx: https://nginx.org/
 .. _cron: https://crontab.guru/
 .. _`opening a ticket`: https://github.com/collective/collective.documentviewer/issues
 
 Changelog
 =========
 
+6.0.3 (2023-05-17)
+------------------
+
+- Allow usage of extra parameters with qpdf using `DOCUMENTVIEWER_QPDF_PARAMETERS` environment variable
+  [mpeeters]
+
+
 6.0.2 (2023-04-27)
 ------------------
 
 - escape querystring search value [kleier]
 
 
 6.0.1 (2021-02-03)
```

### Comparing `collective.documentviewer-6.0.2/README.rst` & `collective.documentviewer-6.0.3/README.rst`

 * *Files identical despite different names*

### Comparing `collective.documentviewer-6.0.2/_cleanup_file_storage.py` & `collective.documentviewer-6.0.3/_cleanup_file_storage.py`

 * *Files identical despite different names*

### Comparing `collective.documentviewer-6.0.2/buildout.cfg` & `collective.documentviewer-6.0.3/buildout.cfg`

 * *Files identical despite different names*

### Comparing `collective.documentviewer-6.0.2/collective/documentviewer/ISO-639-2_utf-8.txt` & `collective.documentviewer-6.0.3/collective/documentviewer/ISO-639-2_utf-8.txt`

 * *Files identical despite different names*

### Comparing `collective.documentviewer-6.0.2/collective/documentviewer/adapters.py` & `collective.documentviewer-6.0.3/collective/documentviewer/adapters.py`

 * *Files identical despite different names*

### Comparing `collective.documentviewer-6.0.2/collective/documentviewer/async_utils.py` & `collective.documentviewer-6.0.3/collective/documentviewer/async_utils.py`

 * *Files identical despite different names*

### Comparing `collective.documentviewer-6.0.2/collective/documentviewer/browser/configure.zcml` & `collective.documentviewer-6.0.3/collective/documentviewer/browser/configure.zcml`

 * *Files identical despite different names*

### Comparing `collective.documentviewer-6.0.2/collective/documentviewer/browser/controlpanel.py` & `collective.documentviewer-6.0.3/collective/documentviewer/browser/controlpanel.py`

 * *Files identical despite different names*

### Comparing `collective.documentviewer-6.0.2/collective/documentviewer/browser/settings.py` & `collective.documentviewer-6.0.3/collective/documentviewer/browser/settings.py`

 * *Files identical despite different names*

### Comparing `collective.documentviewer-6.0.2/collective/documentviewer/browser/templates/async-monitor.pt` & `collective.documentviewer-6.0.3/collective/documentviewer/browser/templates/async-monitor.pt`

 * *Files identical despite different names*

### Comparing `collective.documentviewer-6.0.2/collective/documentviewer/browser/templates/converting.pt` & `collective.documentviewer-6.0.3/collective/documentviewer/browser/templates/converting.pt`

 * *Files identical despite different names*

### Comparing `collective.documentviewer-6.0.2/collective/documentviewer/browser/templates/documentviewer.pt` & `collective.documentviewer-6.0.3/collective/documentviewer/browser/templates/documentviewer.pt`

 * *Files identical despite different names*

### Comparing `collective.documentviewer-6.0.2/collective/documentviewer/browser/templates/group-view.pt` & `collective.documentviewer-6.0.3/collective/documentviewer/browser/templates/group-view.pt`

 * *Files identical despite different names*

### Comparing `collective.documentviewer-6.0.2/collective/documentviewer/browser/traverse.py` & `collective.documentviewer-6.0.3/collective/documentviewer/browser/traverse.py`

 * *Files identical despite different names*

### Comparing `collective.documentviewer-6.0.2/collective/documentviewer/browser/views.py` & `collective.documentviewer-6.0.3/collective/documentviewer/browser/views.py`

 * *Files identical despite different names*

### Comparing `collective.documentviewer-6.0.2/collective/documentviewer/catalog.py` & `collective.documentviewer-6.0.3/collective/documentviewer/catalog.py`

 * *Files identical despite different names*

### Comparing `collective.documentviewer-6.0.2/collective/documentviewer/config.py` & `collective.documentviewer-6.0.3/collective/documentviewer/config.py`

 * *Files identical despite different names*

### Comparing `collective.documentviewer-6.0.2/collective/documentviewer/configure.zcml` & `collective.documentviewer-6.0.3/collective/documentviewer/configure.zcml`

 * *Files identical despite different names*

### Comparing `collective.documentviewer-6.0.2/collective/documentviewer/convert.py` & `collective.documentviewer-6.0.3/collective/documentviewer/convert.py`

 * *Files 2% similar despite different names*

```diff
@@ -210,37 +210,48 @@
     And to strip a page for the screenshot process.
     """
     if os.name == 'nt':
         bin_name = 'qpdf.exe'
     else:
         bin_name = 'qpdf'
 
+    @property
+    def extra_parameters(self):
+        """Return extra parameters that can be defined using environment variable
+        `DOCUMENTVIEWER_QPDF_PARAMETERS`"""
+        return os.getenv("DOCUMENTVIEWER_QPDF_PARAMETERS", "").split()
+
     def __call__(self, filepath):
         outfile = '{}-processed.pdf'.format(filepath[:-4])
-        cmd = [self.binary, '--linearize', filepath, outfile]
+        cmd = [self.binary, '--linearize']
+        cmd.extend(self.extra_parameters)
+        cmd.extend([filepath, outfile])
         self._run_command(cmd)
         shutil.copy(outfile, filepath)
 
     def strip_page(self, filepath, output_dir):
         output_file = os.path.join(output_dir, 'dump_%d.pdf')
-        cmd = [self.bin_name, '--split-pages', filepath,
-               output_file]
-
+        cmd = [self.bin_name, '--split-pages']
+        cmd.extend(self.extra_parameters)
+        cmd.extend([filepath, output_file])
         self._run_command(cmd)
 
     def get_num_pages(self, filepath):
-        cmd = [self.binary, "--show-npages", filepath]
+        cmd = [self.binary, "--show-npages"]
+        cmd.extend(self.extra_parameters)
+        cmd.append(filepath)
         return int(self._run_command(cmd).strip())
 
     def split_pages(self, filepath, output_dir):
         output_dir = os.path.join(output_dir, TEXT_REL_PATHNAME)
         os.mkdir(output_dir)
         output_file = os.path.join(output_dir, 'dump_%d.pdf')
-        cmd = [self.bin_name, '--split-pages', filepath,
-               output_file]
+        cmd = [self.bin_name, '--split-pages']
+        cmd.extend(self.extra_parameters)
+        cmd.extend([filepath, output_file])
         self._run_command(cmd)
         return output_dir
 
 
 try:
     qpdf = QpdfSubProcess()
 except IOError:
```

### Comparing `collective.documentviewer-6.0.2/collective/documentviewer/convert_all.py` & `collective.documentviewer-6.0.3/collective/documentviewer/convert_all.py`

 * *Files identical despite different names*

### Comparing `collective.documentviewer-6.0.2/collective/documentviewer/interfaces.py` & `collective.documentviewer-6.0.3/collective/documentviewer/interfaces.py`

 * *Files identical despite different names*

### Comparing `collective.documentviewer-6.0.2/collective/documentviewer/iso639_2_utf8.py` & `collective.documentviewer-6.0.3/collective/documentviewer/iso639_2_utf8.py`

 * *Files identical despite different names*

### Comparing `collective.documentviewer-6.0.2/collective/documentviewer/locales/collective.documentviewer-manual.pot` & `collective.documentviewer-6.0.3/collective/documentviewer/locales/collective.documentviewer-manual.pot`

 * *Files identical despite different names*

### Comparing `collective.documentviewer-6.0.2/collective/documentviewer/locales/collective.documentviewer.pot` & `collective.documentviewer-6.0.3/collective/documentviewer/locales/collective.documentviewer.pot`

 * *Files identical despite different names*

### Comparing `collective.documentviewer-6.0.2/collective/documentviewer/locales/de/LC_MESSAGES/collective.documentviewer.po` & `collective.documentviewer-6.0.3/collective/documentviewer/locales/de/LC_MESSAGES/collective.documentviewer.po`

 * *Files identical despite different names*

### Comparing `collective.documentviewer-6.0.2/collective/documentviewer/locales/de/LC_MESSAGES/plone.po` & `collective.documentviewer-6.0.3/collective/documentviewer/locales/de/LC_MESSAGES/plone.po`

 * *Files identical despite different names*

### Comparing `collective.documentviewer-6.0.2/collective/documentviewer/locales/en/LC_MESSAGES/collective.documentviewer.po` & `collective.documentviewer-6.0.3/collective/documentviewer/locales/en/LC_MESSAGES/collective.documentviewer.po`

 * *Files identical despite different names*

### Comparing `collective.documentviewer-6.0.2/collective/documentviewer/locales/en/LC_MESSAGES/plone.po` & `collective.documentviewer-6.0.3/collective/documentviewer/locales/en/LC_MESSAGES/plone.po`

 * *Files identical despite different names*

### Comparing `collective.documentviewer-6.0.2/collective/documentviewer/locales/es/LC_MESSAGES/collective.documentviewer.po` & `collective.documentviewer-6.0.3/collective/documentviewer/locales/es/LC_MESSAGES/collective.documentviewer.po`

 * *Files identical despite different names*

### Comparing `collective.documentviewer-6.0.2/collective/documentviewer/locales/es/LC_MESSAGES/plone.po` & `collective.documentviewer-6.0.3/collective/documentviewer/locales/es/LC_MESSAGES/plone.po`

 * *Files identical despite different names*

### Comparing `collective.documentviewer-6.0.2/collective/documentviewer/locales/eu/LC_MESSAGES/collective.documentviewer.po` & `collective.documentviewer-6.0.3/collective/documentviewer/locales/eu/LC_MESSAGES/collective.documentviewer.po`

 * *Files identical despite different names*

### Comparing `collective.documentviewer-6.0.2/collective/documentviewer/locales/eu/LC_MESSAGES/plone.po` & `collective.documentviewer-6.0.3/collective/documentviewer/locales/eu/LC_MESSAGES/plone.po`

 * *Files identical despite different names*

### Comparing `collective.documentviewer-6.0.2/collective/documentviewer/locales/fr/LC_MESSAGES/collective.documentviewer.po` & `collective.documentviewer-6.0.3/collective/documentviewer/locales/fr/LC_MESSAGES/collective.documentviewer.po`

 * *Files identical despite different names*

### Comparing `collective.documentviewer-6.0.2/collective/documentviewer/locales/fr/LC_MESSAGES/plone.po` & `collective.documentviewer-6.0.3/collective/documentviewer/locales/fr/LC_MESSAGES/plone.po`

 * *Files identical despite different names*

### Comparing `collective.documentviewer-6.0.2/collective/documentviewer/locales/it/LC_MESSAGES/collective.documentviewer.po` & `collective.documentviewer-6.0.3/collective/documentviewer/locales/it/LC_MESSAGES/collective.documentviewer.po`

 * *Files identical despite different names*

### Comparing `collective.documentviewer-6.0.2/collective/documentviewer/locales/it/LC_MESSAGES/plone.po` & `collective.documentviewer-6.0.3/collective/documentviewer/locales/it/LC_MESSAGES/plone.po`

 * *Files identical despite different names*

### Comparing `collective.documentviewer-6.0.2/collective/documentviewer/locales/plone-manual.pot` & `collective.documentviewer-6.0.3/collective/documentviewer/locales/plone-manual.pot`

 * *Files identical despite different names*

### Comparing `collective.documentviewer-6.0.2/collective/documentviewer/locales/plone.pot` & `collective.documentviewer-6.0.3/collective/documentviewer/locales/plone.pot`

 * *Files identical despite different names*

### Comparing `collective.documentviewer-6.0.2/collective/documentviewer/locales/rebuild_i18n.sh` & `collective.documentviewer-6.0.3/collective/documentviewer/locales/rebuild_i18n.sh`

 * *Files identical despite different names*

### Comparing `collective.documentviewer-6.0.2/collective/documentviewer/locales/zh_CN/LC_MESSAGES/collective.documentviewer.po` & `collective.documentviewer-6.0.3/collective/documentviewer/locales/zh_CN/LC_MESSAGES/collective.documentviewer.po`

 * *Files identical despite different names*

### Comparing `collective.documentviewer-6.0.2/collective/documentviewer/locales/zh_CN/LC_MESSAGES/plone.po` & `collective.documentviewer-6.0.3/collective/documentviewer/locales/zh_CN/LC_MESSAGES/plone.po`

 * *Files identical despite different names*

### Comparing `collective.documentviewer-6.0.2/collective/documentviewer/migration.py` & `collective.documentviewer-6.0.3/collective/documentviewer/migration.py`

 * *Files identical despite different names*

### Comparing `collective.documentviewer-6.0.2/collective/documentviewer/profiles/default/actions.xml` & `collective.documentviewer-6.0.3/collective/documentviewer/profiles/default/actions.xml`

 * *Files identical despite different names*

### Comparing `collective.documentviewer-6.0.2/collective/documentviewer/profiles/default/controlpanel.xml` & `collective.documentviewer-6.0.3/collective/documentviewer/profiles/default/controlpanel.xml`

 * *Files identical despite different names*

### Comparing `collective.documentviewer-6.0.2/collective/documentviewer/resources/assets/fallback-datauri.css` & `collective.documentviewer-6.0.3/collective/documentviewer/resources/assets/fallback-datauri.css`

 * *Files identical despite different names*

### Comparing `collective.documentviewer-6.0.2/collective/documentviewer/resources/assets/fallback.css` & `collective.documentviewer-6.0.3/collective/documentviewer/resources/assets/fallback.css`

 * *Files identical despite different names*

### Comparing `collective.documentviewer-6.0.2/collective/documentviewer/resources/assets/plain-datauri.css` & `collective.documentviewer-6.0.3/collective/documentviewer/resources/assets/plain-datauri.css`

 * *Files identical despite different names*

### Comparing `collective.documentviewer-6.0.2/collective/documentviewer/resources/assets/plain.css` & `collective.documentviewer-6.0.3/collective/documentviewer/resources/assets/plain.css`

 * *Files identical despite different names*

### Comparing `collective.documentviewer-6.0.2/collective/documentviewer/resources/assets/templates.js` & `collective.documentviewer-6.0.3/collective/documentviewer/resources/assets/templates.js`

 * *Files identical despite different names*

### Comparing `collective.documentviewer-6.0.2/collective/documentviewer/resources/assets/viewer-datauri.css` & `collective.documentviewer-6.0.3/collective/documentviewer/resources/assets/viewer-datauri.css`

 * *Files identical despite different names*

### Comparing `collective.documentviewer-6.0.2/collective/documentviewer/resources/assets/viewer.css` & `collective.documentviewer-6.0.3/collective/documentviewer/resources/assets/viewer.css`

 * *Files identical despite different names*

### Comparing `collective.documentviewer-6.0.2/collective/documentviewer/resources/assets/viewer.js` & `collective.documentviewer-6.0.3/collective/documentviewer/resources/assets/viewer.js`

 * *Files identical despite different names*

### Comparing `collective.documentviewer-6.0.2/collective/documentviewer/resources/images/application-pdf.png` & `collective.documentviewer-6.0.3/collective/documentviewer/resources/images/application-pdf.png`

 * *Files identical despite different names*

### Comparing `collective.documentviewer-6.0.2/collective/documentviewer/resources/images/clear.png` & `collective.documentviewer-6.0.3/collective/documentviewer/resources/images/clear.png`

 * *Files identical despite different names*

### Comparing `collective.documentviewer-6.0.2/collective/documentviewer/resources/images/pdf.png` & `collective.documentviewer-6.0.3/collective/documentviewer/resources/images/pdf.png`

 * *Files identical despite different names*

### Comparing `collective.documentviewer-6.0.2/collective/documentviewer/resources/javascripts/build.min.js` & `collective.documentviewer-6.0.3/collective/documentviewer/resources/javascripts/build.min.js`

 * *Files identical despite different names*

### Comparing `collective.documentviewer-6.0.2/collective/documentviewer/resources/javascripts/build.min.js.map` & `collective.documentviewer-6.0.3/collective/documentviewer/resources/javascripts/build.min.js.map`

 * *Files identical despite different names*

### Comparing `collective.documentviewer-6.0.2/collective/documentviewer/resources/javascripts/group.js` & `collective.documentviewer-6.0.3/collective/documentviewer/resources/javascripts/group.js`

 * *Files identical despite different names*

### Comparing `collective.documentviewer-6.0.2/collective/documentviewer/resources/javascripts/viewer.js` & `collective.documentviewer-6.0.3/collective/documentviewer/resources/javascripts/viewer.js`

 * *Files identical despite different names*

### Comparing `collective.documentviewer-6.0.2/collective/documentviewer/resources/stylesheets/group.css` & `collective.documentviewer-6.0.3/collective/documentviewer/resources/stylesheets/group.css`

 * *Files identical despite different names*

### Comparing `collective.documentviewer-6.0.2/collective/documentviewer/resources/stylesheets/viewer.css.map` & `collective.documentviewer-6.0.3/collective/documentviewer/resources/stylesheets/viewer.css.map`

 * *Files identical despite different names*

### Comparing `collective.documentviewer-6.0.2/collective/documentviewer/settings.py` & `collective.documentviewer-6.0.3/collective/documentviewer/settings.py`

 * *Files identical despite different names*

### Comparing `collective.documentviewer-6.0.2/collective/documentviewer/setuphandlers.py` & `collective.documentviewer-6.0.3/collective/documentviewer/setuphandlers.py`

 * *Files identical despite different names*

### Comparing `collective.documentviewer-6.0.2/collective/documentviewer/storage.py` & `collective.documentviewer-6.0.3/collective/documentviewer/storage.py`

 * *Files identical despite different names*

### Comparing `collective.documentviewer-6.0.2/collective/documentviewer/subscribers.py` & `collective.documentviewer-6.0.3/collective/documentviewer/subscribers.py`

 * *Files identical despite different names*

### Comparing `collective.documentviewer-6.0.2/collective/documentviewer/testing.py` & `collective.documentviewer-6.0.3/collective/documentviewer/testing.py`

 * *Files identical despite different names*

### Comparing `collective.documentviewer-6.0.2/collective/documentviewer/tests/__init__.py` & `collective.documentviewer-6.0.3/collective/documentviewer/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `collective.documentviewer-6.0.2/collective/documentviewer/tests/test_convert.py` & `collective.documentviewer-6.0.3/collective/documentviewer/tests/test_convert.py`

 * *Files identical despite different names*

### Comparing `collective.documentviewer-6.0.2/collective/documentviewer/tests/test_files/test.doc` & `collective.documentviewer-6.0.3/collective/documentviewer/tests/test_files/test.doc`

 * *Files identical despite different names*

### Comparing `collective.documentviewer-6.0.2/collective/documentviewer/tests/test_files/test.odp` & `collective.documentviewer-6.0.3/collective/documentviewer/tests/test_files/test.odp`

 * *Files identical despite different names*

### Comparing `collective.documentviewer-6.0.2/collective/documentviewer/tests/test_files/test.pdf` & `collective.documentviewer-6.0.3/collective/documentviewer/tests/test_files/test.pdf`

 * *Files identical despite different names*

### Comparing `collective.documentviewer-6.0.2/collective/documentviewer/tests/test_migrate.py` & `collective.documentviewer-6.0.3/collective/documentviewer/tests/test_migrate.py`

 * *Files identical despite different names*

### Comparing `collective.documentviewer-6.0.2/collective/documentviewer/tests/test_storage.py` & `collective.documentviewer-6.0.3/collective/documentviewer/tests/test_storage.py`

 * *Files identical despite different names*

### Comparing `collective.documentviewer-6.0.2/collective/documentviewer/tests/test_views.py` & `collective.documentviewer-6.0.3/collective/documentviewer/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `collective.documentviewer-6.0.2/collective/documentviewer/upgrades.py` & `collective.documentviewer-6.0.3/collective/documentviewer/upgrades.py`

 * *Files identical despite different names*

### Comparing `collective.documentviewer-6.0.2/collective/documentviewer/upgrades.zcml` & `collective.documentviewer-6.0.3/collective/documentviewer/upgrades.zcml`

 * *Files identical despite different names*

### Comparing `collective.documentviewer-6.0.2/collective/documentviewer/utils.py` & `collective.documentviewer-6.0.3/collective/documentviewer/utils.py`

 * *Files identical despite different names*

### Comparing `collective.documentviewer-6.0.2/collective.documentviewer.egg-info/PKG-INFO` & `collective.documentviewer-6.0.3/collective.documentviewer.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: collective.documentviewer
-Version: 6.0.2
+Version: 6.0.3
 Summary: Document cloud's document viewer integration into plone.
 Home-page: https://github.com/collective/collective.documentviewer
 Author: Nathan Van Gheem
 Author-email: vangheem@gmail.com
 License: GPL
 Keywords: plone documentviewer pdf ocr doc viewer
 Classifier: Development Status :: 5 - Production/Stable
@@ -300,14 +300,21 @@
 .. _Nginx: https://nginx.org/
 .. _cron: https://crontab.guru/
 .. _`opening a ticket`: https://github.com/collective/collective.documentviewer/issues
 
 Changelog
 =========
 
+6.0.3 (2023-05-17)
+------------------
+
+- Allow usage of extra parameters with qpdf using `DOCUMENTVIEWER_QPDF_PARAMETERS` environment variable
+  [mpeeters]
+
+
 6.0.2 (2023-04-27)
 ------------------
 
 - escape querystring search value [kleier]
 
 
 6.0.1 (2021-02-03)
```

### Comparing `collective.documentviewer-6.0.2/collective.documentviewer.egg-info/SOURCES.txt` & `collective.documentviewer-6.0.3/collective.documentviewer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `collective.documentviewer-6.0.2/docs/HISTORY.txt` & `collective.documentviewer-6.0.3/docs/HISTORY.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,17 @@
 Changelog
 =========
 
+6.0.3 (2023-05-17)
+------------------
+
+- Allow usage of extra parameters with qpdf using `DOCUMENTVIEWER_QPDF_PARAMETERS` environment variable
+  [mpeeters]
+
+
 6.0.2 (2023-04-27)
 ------------------
 
 - escape querystring search value [kleier]
 
 
 6.0.1 (2021-02-03)
```

### Comparing `collective.documentviewer-6.0.2/docs/INSTALL.txt` & `collective.documentviewer-6.0.3/docs/INSTALL.txt`

 * *Files identical despite different names*

### Comparing `collective.documentviewer-6.0.2/docs/LICENSE.GPL` & `collective.documentviewer-6.0.3/docs/LICENSE.GPL`

 * *Files identical despite different names*

### Comparing `collective.documentviewer-6.0.2/docs/LICENSE.txt` & `collective.documentviewer-6.0.3/docs/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `collective.documentviewer-6.0.2/docs/_static/wildcardcorp_logo.png` & `collective.documentviewer-6.0.3/docs/_static/wildcardcorp_logo.png`

 * *Files identical despite different names*

### Comparing `collective.documentviewer-6.0.2/setup.py` & `collective.documentviewer-6.0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup, find_packages
 import os
 
-version = '6.0.2'
+version = '6.0.3'
 
 setup(name='collective.documentviewer',
       version=version,
       description="Document cloud's document viewer integration into plone.",
       long_description="%s\n%s" % (
           open("README.rst").read(),
           open(os.path.join("docs", "HISTORY.txt")).read()
```

