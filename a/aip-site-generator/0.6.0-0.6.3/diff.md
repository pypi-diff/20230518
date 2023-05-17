# Comparing `tmp/aip-site-generator-0.6.0.tar.gz` & `tmp/aip-site-generator-0.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aip-site-generator-0.6.0.tar", last modified: Mon Jul 12 17:34:52 2021, max compression
+gzip compressed data, was "aip-site-generator-0.6.3.tar", last modified: Wed May 17 22:54:56 2023, max compression
```

## Comparing `aip-site-generator-0.6.0.tar` & `aip-site-generator-0.6.3.tar`

### file list

```diff
@@ -1,103 +1,103 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-12 17:34:52.542579 aip-site-generator-0.6.0/
--rw-r--r--   0 root         (0) root         (0)    11359 2021-07-12 17:34:44.000000 aip-site-generator-0.6.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)      138 2021-07-12 17:34:44.000000 aip-site-generator-0.6.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     5193 2021-07-12 17:34:52.542579 aip-site-generator-0.6.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4490 2021-07-12 17:34:44.000000 aip-site-generator-0.6.0/README.md
--rw-r--r--   0 root         (0) root         (0)        6 2021-07-12 17:34:51.000000 aip-site-generator-0.6.0/VERSION
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-12 17:34:52.526579 aip-site-generator-0.6.0/aip_site/
--rw-r--r--   0 root         (0) root         (0)        0 2021-07-12 17:34:44.000000 aip-site-generator-0.6.0/aip_site/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1446 2021-07-12 17:34:44.000000 aip-site-generator-0.6.0/aip_site/cli.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-12 17:34:52.526579 aip-site-generator-0.6.0/aip_site/jinja/
--rw-r--r--   0 root         (0) root         (0)        0 2021-07-12 17:34:44.000000 aip-site-generator-0.6.0/aip_site/jinja/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1044 2021-07-12 17:34:44.000000 aip-site-generator-0.6.0/aip_site/jinja/env.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-12 17:34:52.526579 aip-site-generator-0.6.0/aip_site/jinja/ext/
--rw-r--r--   0 root         (0) root         (0)        0 2021-07-12 17:34:44.000000 aip-site-generator-0.6.0/aip_site/jinja/ext/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5484 2021-07-12 17:34:44.000000 aip-site-generator-0.6.0/aip_site/jinja/ext/sample.py
--rw-r--r--   0 root         (0) root         (0)     2082 2021-07-12 17:34:44.000000 aip-site-generator-0.6.0/aip_site/jinja/ext/tab.py
--rw-r--r--   0 root         (0) root         (0)     3268 2021-07-12 17:34:44.000000 aip-site-generator-0.6.0/aip_site/jinja/loaders.py
--rw-r--r--   0 root         (0) root         (0)     5319 2021-07-12 17:34:44.000000 aip-site-generator-0.6.0/aip_site/md.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-12 17:34:52.530579 aip-site-generator-0.6.0/aip_site/models/
--rw-r--r--   0 root         (0) root         (0)        0 2021-07-12 17:34:44.000000 aip-site-generator-0.6.0/aip_site/models/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6222 2021-07-12 17:34:44.000000 aip-site-generator-0.6.0/aip_site/models/aip.py
--rw-r--r--   0 root         (0) root         (0)     4107 2021-07-12 17:34:44.000000 aip-site-generator-0.6.0/aip_site/models/page.py
--rw-r--r--   0 root         (0) root         (0)     4572 2021-07-12 17:34:44.000000 aip-site-generator-0.6.0/aip_site/models/scope.py
--rw-r--r--   0 root         (0) root         (0)     4611 2021-07-12 17:34:44.000000 aip-site-generator-0.6.0/aip_site/models/site.py
--rw-r--r--   0 root         (0) root         (0)     4681 2021-07-12 17:34:44.000000 aip-site-generator-0.6.0/aip_site/publisher.py
--rw-r--r--   0 root         (0) root         (0)     2735 2021-07-12 17:34:44.000000 aip-site-generator-0.6.0/aip_site/server.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-12 17:34:52.522579 aip-site-generator-0.6.0/aip_site/support/
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-12 17:34:52.530579 aip-site-generator-0.6.0/aip_site/support/assets/
--rw-r--r--   0 root         (0) root         (0)     5430 2021-07-12 17:34:44.000000 aip-site-generator-0.6.0/aip_site/support/assets/favicon.ico
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-12 17:34:52.530579 aip-site-generator-0.6.0/aip_site/support/assets/images/
--rw-r--r--   0 root         (0) root         (0)     4044 2021-07-12 17:34:44.000000 aip-site-generator-0.6.0/aip_site/support/assets/images/github.png
--rw-r--r--   0 root         (0) root         (0)    13956 2021-07-12 17:34:44.000000 aip-site-generator-0.6.0/aip_site/support/assets/images/glue-icons.svg
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-12 17:34:52.530579 aip-site-generator-0.6.0/aip_site/support/assets/js/
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-12 17:34:52.530579 aip-site-generator-0.6.0/aip_site/support/assets/js/aip/
--rw-r--r--   0 root         (0) root         (0)     1399 2021-07-12 17:34:44.000000 aip-site-generator-0.6.0/aip_site/support/assets/js/aip/aip-graphviz.js
--rw-r--r--   0 root         (0) root         (0)      992 2021-07-12 17:34:44.000000 aip-site-generator-0.6.0/aip_site/support/assets/js/aip/aip-index.js
--rw-r--r--   0 root         (0) root         (0)     2867 2021-07-12 17:34:44.000000 aip-site-generator-0.6.0/aip_site/support/assets/js/global.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-12 17:34:52.534579 aip-site-generator-0.6.0/aip_site/support/assets/js/graphviz/
--rw-r--r--   0 root         (0) root         (0)  1439383 2021-07-12 17:34:44.000000 aip-site-generator-0.6.0/aip_site/support/assets/js/graphviz/lite.render.js
--rw-r--r--   0 root         (0) root         (0)    11468 2021-07-12 17:34:44.000000 aip-site-generator-0.6.0/aip_site/support/assets/js/graphviz/viz.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-12 17:34:52.534579 aip-site-generator-0.6.0/aip_site/support/assets/js/search/
--rw-r--r--   0 root         (0) root         (0)      982 2021-07-12 17:34:44.000000 aip-site-generator-0.6.0/aip_site/support/assets/js/search/pagination.js
--rw-r--r--   0 root         (0) root         (0)    10308 2021-07-12 17:34:44.000000 aip-site-generator-0.6.0/aip_site/support/assets/js/search/tipuesearch.min.js
--rw-r--r--   0 root         (0) root         (0)     3456 2021-07-12 17:34:44.000000 aip-site-generator-0.6.0/aip_site/support/assets/js/search/tipuesearch_set.js
--rw-r--r--   0 root         (0) root         (0)     3925 2021-07-12 17:34:44.000000 aip-site-generator-0.6.0/aip_site/support/assets/js/syntax.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-12 17:34:52.534579 aip-site-generator-0.6.0/aip_site/support/assets/misc/
--rw-r--r--   0 root         (0) root         (0)     4775 2021-07-12 17:34:44.000000 aip-site-generator-0.6.0/aip_site/support/assets/misc/ebnf-filtering.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-12 17:34:52.534579 aip-site-generator-0.6.0/aip_site/support/scss/
--rw-r--r--   0 root         (0) root         (0)      851 2021-07-12 17:34:44.000000 aip-site-generator-0.6.0/aip_site/support/scss/hero.scss
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-12 17:34:52.534579 aip-site-generator-0.6.0/aip_site/support/scss/imports/
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-12 17:34:52.538579 aip-site-generator-0.6.0/aip_site/support/scss/imports/aip/
--rw-r--r--   0 root         (0) root         (0)      443 2021-07-12 17:34:44.000000 aip-site-generator-0.6.0/aip_site/support/scss/imports/aip/badges.scss
--rw-r--r--   0 root         (0) root         (0)      218 2021-07-12 17:34:44.000000 aip-site-generator-0.6.0/aip_site/support/scss/imports/aip/breadcrumbs.scss
--rw-r--r--   0 root         (0) root         (0)       67 2021-07-12 17:34:44.000000 aip-site-generator-0.6.0/aip_site/support/scss/imports/aip/header.scss
--rw-r--r--   0 root         (0) root         (0)      184 2021-07-12 17:34:44.000000 aip-site-generator-0.6.0/aip_site/support/scss/imports/aip/nav.scss
--rw-r--r--   0 root         (0) root         (0)      611 2021-07-12 17:34:44.000000 aip-site-generator-0.6.0/aip_site/support/scss/imports/aip/news.scss
--rw-r--r--   0 root         (0) root         (0)     1288 2021-07-12 17:34:44.000000 aip-site-generator-0.6.0/aip_site/support/scss/imports/aip/tables.scss
--rw-r--r--   0 root         (0) root         (0)      942 2021-07-12 17:34:44.000000 aip-site-generator-0.6.0/aip_site/support/scss/imports/callouts.scss
--rw-r--r--   0 root         (0) root         (0)     4017 2021-07-12 17:34:44.000000 aip-site-generator-0.6.0/aip_site/support/scss/imports/colors.scss
--rw-r--r--   0 root         (0) root         (0)      240 2021-07-12 17:34:44.000000 aip-site-generator-0.6.0/aip_site/support/scss/imports/footer.scss
--rw-r--r--   0 root         (0) root         (0)     1211 2021-07-12 17:34:44.000000 aip-site-generator-0.6.0/aip_site/support/scss/imports/header.scss
--rw-r--r--   0 root         (0) root         (0)      600 2021-07-12 17:34:44.000000 aip-site-generator-0.6.0/aip_site/support/scss/imports/headings.scss
--rw-r--r--   0 root         (0) root         (0)      128 2021-07-12 17:34:44.000000 aip-site-generator-0.6.0/aip_site/support/scss/imports/lists.scss
--rw-r--r--   0 root         (0) root         (0)     2655 2021-07-12 17:34:44.000000 aip-site-generator-0.6.0/aip_site/support/scss/imports/nav.scss
--rw-r--r--   0 root         (0) root         (0)     1266 2021-07-12 17:34:44.000000 aip-site-generator-0.6.0/aip_site/support/scss/imports/sidebar.scss
--rw-r--r--   0 root         (0) root         (0)     3426 2021-07-12 17:34:44.000000 aip-site-generator-0.6.0/aip_site/support/scss/imports/syntax.scss
--rw-r--r--   0 root         (0) root         (0)      102 2021-07-12 17:34:44.000000 aip-site-generator-0.6.0/aip_site/support/scss/imports/tables.scss
--rw-r--r--   0 root         (0) root         (0)      889 2021-07-12 17:34:44.000000 aip-site-generator-0.6.0/aip_site/support/scss/imports/tabs.scss
--rw-r--r--   0 root         (0) root         (0)     1053 2021-07-12 17:34:44.000000 aip-site-generator-0.6.0/aip_site/support/scss/print.scss
--rw-r--r--   0 root         (0) root         (0)     1429 2021-07-12 17:34:44.000000 aip-site-generator-0.6.0/aip_site/support/scss/search.scss
--rw-r--r--   0 root         (0) root         (0)      466 2021-07-12 17:34:44.000000 aip-site-generator-0.6.0/aip_site/support/scss/style.scss
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-12 17:34:52.538579 aip-site-generator-0.6.0/aip_site/support/templates/
--rw-r--r--   0 root         (0) root         (0)     1865 2021-07-12 17:34:44.000000 aip-site-generator-0.6.0/aip_site/support/templates/aip-listing.html.j2
--rw-r--r--   0 root         (0) root         (0)     2178 2021-07-12 17:34:44.000000 aip-site-generator-0.6.0/aip_site/support/templates/aip.html.j2
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-12 17:34:52.538579 aip-site-generator-0.6.0/aip_site/support/templates/includes/
--rw-r--r--   0 root         (0) root         (0)     1053 2021-07-12 17:34:44.000000 aip-site-generator-0.6.0/aip_site/support/templates/includes/breadcrumb.html.j2
--rw-r--r--   0 root         (0) root         (0)      415 2021-07-12 17:34:44.000000 aip-site-generator-0.6.0/aip_site/support/templates/includes/footer.html.j2
--rw-r--r--   0 root         (0) root         (0)     5106 2021-07-12 17:34:44.000000 aip-site-generator-0.6.0/aip_site/support/templates/includes/header.html.j2
--rw-r--r--   0 root         (0) root         (0)      986 2021-07-12 17:34:44.000000 aip-site-generator-0.6.0/aip_site/support/templates/includes/nav.html.j2
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-12 17:34:52.542579 aip-site-generator-0.6.0/aip_site/support/templates/includes/state_banners/
--rw-r--r--   0 root         (0) root         (0)      189 2021-07-12 17:34:44.000000 aip-site-generator-0.6.0/aip_site/support/templates/includes/state_banners/draft.html.j2
--rw-r--r--   0 root         (0) root         (0)      125 2021-07-12 17:34:44.000000 aip-site-generator-0.6.0/aip_site/support/templates/includes/state_banners/rejected.html.j2
--rw-r--r--   0 root         (0) root         (0)      212 2021-07-12 17:34:44.000000 aip-site-generator-0.6.0/aip_site/support/templates/includes/state_banners/replaced.html.j2
--rw-r--r--   0 root         (0) root         (0)      316 2021-07-12 17:34:44.000000 aip-site-generator-0.6.0/aip_site/support/templates/includes/state_banners/reviewing.html.j2
--rw-r--r--   0 root         (0) root         (0)      126 2021-07-12 17:34:44.000000 aip-site-generator-0.6.0/aip_site/support/templates/includes/state_banners/withdrawn.html.j2
--rw-r--r--   0 root         (0) root         (0)     1630 2021-07-12 17:34:44.000000 aip-site-generator-0.6.0/aip_site/support/templates/index.html.j2
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-12 17:34:52.542579 aip-site-generator-0.6.0/aip_site/support/templates/layouts/
--rw-r--r--   0 root         (0) root         (0)     2696 2021-07-12 17:34:44.000000 aip-site-generator-0.6.0/aip_site/support/templates/layouts/base.html.j2
--rw-r--r--   0 root         (0) root         (0)     1033 2021-07-12 17:34:44.000000 aip-site-generator-0.6.0/aip_site/support/templates/page.html.j2
--rw-r--r--   0 root         (0) root         (0)      544 2021-07-12 17:34:44.000000 aip-site-generator-0.6.0/aip_site/support/templates/redirect.html.j2
--rw-r--r--   0 root         (0) root         (0)     1508 2021-07-12 17:34:44.000000 aip-site-generator-0.6.0/aip_site/support/templates/search.html.j2
--rw-r--r--   0 root         (0) root         (0)      443 2021-07-12 17:34:44.000000 aip-site-generator-0.6.0/aip_site/support/templates/search.js.j2
--rw-r--r--   0 root         (0) root         (0)     1229 2021-07-12 17:34:44.000000 aip-site-generator-0.6.0/aip_site/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-12 17:34:52.542579 aip-site-generator-0.6.0/aip_site_generator.egg-info/
--rw-r--r--   0 root         (0) root         (0)     5193 2021-07-12 17:34:52.000000 aip-site-generator-0.6.0/aip_site_generator.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3071 2021-07-12 17:34:52.000000 aip-site-generator-0.6.0/aip_site_generator.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2021-07-12 17:34:52.000000 aip-site-generator-0.6.0/aip_site_generator.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      106 2021-07-12 17:34:52.000000 aip-site-generator-0.6.0/aip_site_generator.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2021-07-12 17:34:52.000000 aip-site-generator-0.6.0/aip_site_generator.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      190 2021-07-12 17:34:52.000000 aip-site-generator-0.6.0/aip_site_generator.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        9 2021-07-12 17:34:52.000000 aip-site-generator-0.6.0/aip_site_generator.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2021-07-12 17:34:52.542579 aip-site-generator-0.6.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2329 2021-07-12 17:34:44.000000 aip-site-generator-0.6.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 22:54:56.074308 aip-site-generator-0.6.3/
+-rw-r--r--   0 root         (0) root         (0)    11359 2023-05-17 22:54:47.000000 aip-site-generator-0.6.3/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      138 2023-05-17 22:54:47.000000 aip-site-generator-0.6.3/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     6051 2023-05-17 22:54:56.074308 aip-site-generator-0.6.3/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     5349 2023-05-17 22:54:47.000000 aip-site-generator-0.6.3/README.md
+-rw-r--r--   0 root         (0) root         (0)        6 2023-05-17 22:54:55.000000 aip-site-generator-0.6.3/VERSION
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 22:54:56.062308 aip-site-generator-0.6.3/aip_site/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-17 22:54:47.000000 aip-site-generator-0.6.3/aip_site/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1446 2023-05-17 22:54:47.000000 aip-site-generator-0.6.3/aip_site/cli.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 22:54:56.062308 aip-site-generator-0.6.3/aip_site/jinja/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-17 22:54:47.000000 aip-site-generator-0.6.3/aip_site/jinja/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1044 2023-05-17 22:54:47.000000 aip-site-generator-0.6.3/aip_site/jinja/env.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 22:54:56.062308 aip-site-generator-0.6.3/aip_site/jinja/ext/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-17 22:54:47.000000 aip-site-generator-0.6.3/aip_site/jinja/ext/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5484 2023-05-17 22:54:47.000000 aip-site-generator-0.6.3/aip_site/jinja/ext/sample.py
+-rw-r--r--   0 root         (0) root         (0)     2082 2023-05-17 22:54:47.000000 aip-site-generator-0.6.3/aip_site/jinja/ext/tab.py
+-rw-r--r--   0 root         (0) root         (0)     3264 2023-05-17 22:54:47.000000 aip-site-generator-0.6.3/aip_site/jinja/loaders.py
+-rw-r--r--   0 root         (0) root         (0)     5319 2023-05-17 22:54:47.000000 aip-site-generator-0.6.3/aip_site/md.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 22:54:56.066308 aip-site-generator-0.6.3/aip_site/models/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-17 22:54:47.000000 aip-site-generator-0.6.3/aip_site/models/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6280 2023-05-17 22:54:47.000000 aip-site-generator-0.6.3/aip_site/models/aip.py
+-rw-r--r--   0 root         (0) root         (0)     4107 2023-05-17 22:54:47.000000 aip-site-generator-0.6.3/aip_site/models/page.py
+-rw-r--r--   0 root         (0) root         (0)     4572 2023-05-17 22:54:47.000000 aip-site-generator-0.6.3/aip_site/models/scope.py
+-rw-r--r--   0 root         (0) root         (0)     4611 2023-05-17 22:54:47.000000 aip-site-generator-0.6.3/aip_site/models/site.py
+-rw-r--r--   0 root         (0) root         (0)     4681 2023-05-17 22:54:47.000000 aip-site-generator-0.6.3/aip_site/publisher.py
+-rw-r--r--   0 root         (0) root         (0)     3014 2023-05-17 22:54:47.000000 aip-site-generator-0.6.3/aip_site/server.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 22:54:56.062308 aip-site-generator-0.6.3/aip_site/support/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 22:54:56.066308 aip-site-generator-0.6.3/aip_site/support/assets/
+-rw-r--r--   0 root         (0) root         (0)     5430 2023-05-17 22:54:47.000000 aip-site-generator-0.6.3/aip_site/support/assets/favicon.ico
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 22:54:56.066308 aip-site-generator-0.6.3/aip_site/support/assets/images/
+-rw-r--r--   0 root         (0) root         (0)     4044 2023-05-17 22:54:47.000000 aip-site-generator-0.6.3/aip_site/support/assets/images/github.png
+-rw-r--r--   0 root         (0) root         (0)    13956 2023-05-17 22:54:47.000000 aip-site-generator-0.6.3/aip_site/support/assets/images/glue-icons.svg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 22:54:56.066308 aip-site-generator-0.6.3/aip_site/support/assets/js/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 22:54:56.066308 aip-site-generator-0.6.3/aip_site/support/assets/js/aip/
+-rw-r--r--   0 root         (0) root         (0)     1399 2023-05-17 22:54:47.000000 aip-site-generator-0.6.3/aip_site/support/assets/js/aip/aip-graphviz.js
+-rw-r--r--   0 root         (0) root         (0)      992 2023-05-17 22:54:47.000000 aip-site-generator-0.6.3/aip_site/support/assets/js/aip/aip-index.js
+-rw-r--r--   0 root         (0) root         (0)     2867 2023-05-17 22:54:47.000000 aip-site-generator-0.6.3/aip_site/support/assets/js/global.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 22:54:56.066308 aip-site-generator-0.6.3/aip_site/support/assets/js/graphviz/
+-rw-r--r--   0 root         (0) root         (0)  1439383 2023-05-17 22:54:47.000000 aip-site-generator-0.6.3/aip_site/support/assets/js/graphviz/lite.render.js
+-rw-r--r--   0 root         (0) root         (0)    11468 2023-05-17 22:54:47.000000 aip-site-generator-0.6.3/aip_site/support/assets/js/graphviz/viz.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 22:54:56.066308 aip-site-generator-0.6.3/aip_site/support/assets/js/search/
+-rw-r--r--   0 root         (0) root         (0)      982 2023-05-17 22:54:47.000000 aip-site-generator-0.6.3/aip_site/support/assets/js/search/pagination.js
+-rw-r--r--   0 root         (0) root         (0)    10308 2023-05-17 22:54:47.000000 aip-site-generator-0.6.3/aip_site/support/assets/js/search/tipuesearch.min.js
+-rw-r--r--   0 root         (0) root         (0)     3456 2023-05-17 22:54:47.000000 aip-site-generator-0.6.3/aip_site/support/assets/js/search/tipuesearch_set.js
+-rw-r--r--   0 root         (0) root         (0)     3925 2023-05-17 22:54:47.000000 aip-site-generator-0.6.3/aip_site/support/assets/js/syntax.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 22:54:56.066308 aip-site-generator-0.6.3/aip_site/support/assets/misc/
+-rw-r--r--   0 root         (0) root         (0)     4775 2023-05-17 22:54:47.000000 aip-site-generator-0.6.3/aip_site/support/assets/misc/ebnf-filtering.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 22:54:56.070309 aip-site-generator-0.6.3/aip_site/support/scss/
+-rw-r--r--   0 root         (0) root         (0)      851 2023-05-17 22:54:47.000000 aip-site-generator-0.6.3/aip_site/support/scss/hero.scss
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 22:54:56.070309 aip-site-generator-0.6.3/aip_site/support/scss/imports/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 22:54:56.070309 aip-site-generator-0.6.3/aip_site/support/scss/imports/aip/
+-rw-r--r--   0 root         (0) root         (0)      443 2023-05-17 22:54:47.000000 aip-site-generator-0.6.3/aip_site/support/scss/imports/aip/badges.scss
+-rw-r--r--   0 root         (0) root         (0)      218 2023-05-17 22:54:47.000000 aip-site-generator-0.6.3/aip_site/support/scss/imports/aip/breadcrumbs.scss
+-rw-r--r--   0 root         (0) root         (0)       67 2023-05-17 22:54:47.000000 aip-site-generator-0.6.3/aip_site/support/scss/imports/aip/header.scss
+-rw-r--r--   0 root         (0) root         (0)      184 2023-05-17 22:54:47.000000 aip-site-generator-0.6.3/aip_site/support/scss/imports/aip/nav.scss
+-rw-r--r--   0 root         (0) root         (0)      611 2023-05-17 22:54:47.000000 aip-site-generator-0.6.3/aip_site/support/scss/imports/aip/news.scss
+-rw-r--r--   0 root         (0) root         (0)     1288 2023-05-17 22:54:47.000000 aip-site-generator-0.6.3/aip_site/support/scss/imports/aip/tables.scss
+-rw-r--r--   0 root         (0) root         (0)      988 2023-05-17 22:54:47.000000 aip-site-generator-0.6.3/aip_site/support/scss/imports/callouts.scss
+-rw-r--r--   0 root         (0) root         (0)     4017 2023-05-17 22:54:47.000000 aip-site-generator-0.6.3/aip_site/support/scss/imports/colors.scss
+-rw-r--r--   0 root         (0) root         (0)      240 2023-05-17 22:54:47.000000 aip-site-generator-0.6.3/aip_site/support/scss/imports/footer.scss
+-rw-r--r--   0 root         (0) root         (0)     1211 2023-05-17 22:54:47.000000 aip-site-generator-0.6.3/aip_site/support/scss/imports/header.scss
+-rw-r--r--   0 root         (0) root         (0)      678 2023-05-17 22:54:47.000000 aip-site-generator-0.6.3/aip_site/support/scss/imports/headings.scss
+-rw-r--r--   0 root         (0) root         (0)      128 2023-05-17 22:54:47.000000 aip-site-generator-0.6.3/aip_site/support/scss/imports/lists.scss
+-rw-r--r--   0 root         (0) root         (0)     2655 2023-05-17 22:54:47.000000 aip-site-generator-0.6.3/aip_site/support/scss/imports/nav.scss
+-rw-r--r--   0 root         (0) root         (0)     1266 2023-05-17 22:54:47.000000 aip-site-generator-0.6.3/aip_site/support/scss/imports/sidebar.scss
+-rw-r--r--   0 root         (0) root         (0)     3426 2023-05-17 22:54:47.000000 aip-site-generator-0.6.3/aip_site/support/scss/imports/syntax.scss
+-rw-r--r--   0 root         (0) root         (0)      102 2023-05-17 22:54:47.000000 aip-site-generator-0.6.3/aip_site/support/scss/imports/tables.scss
+-rw-r--r--   0 root         (0) root         (0)      889 2023-05-17 22:54:47.000000 aip-site-generator-0.6.3/aip_site/support/scss/imports/tabs.scss
+-rw-r--r--   0 root         (0) root         (0)     1053 2023-05-17 22:54:47.000000 aip-site-generator-0.6.3/aip_site/support/scss/print.scss
+-rw-r--r--   0 root         (0) root         (0)     1429 2023-05-17 22:54:47.000000 aip-site-generator-0.6.3/aip_site/support/scss/search.scss
+-rw-r--r--   0 root         (0) root         (0)      466 2023-05-17 22:54:47.000000 aip-site-generator-0.6.3/aip_site/support/scss/style.scss
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 22:54:56.074308 aip-site-generator-0.6.3/aip_site/support/templates/
+-rw-r--r--   0 root         (0) root         (0)     1865 2023-05-17 22:54:47.000000 aip-site-generator-0.6.3/aip_site/support/templates/aip-listing.html.j2
+-rw-r--r--   0 root         (0) root         (0)     2178 2023-05-17 22:54:47.000000 aip-site-generator-0.6.3/aip_site/support/templates/aip.html.j2
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 22:54:56.074308 aip-site-generator-0.6.3/aip_site/support/templates/includes/
+-rw-r--r--   0 root         (0) root         (0)     1053 2023-05-17 22:54:47.000000 aip-site-generator-0.6.3/aip_site/support/templates/includes/breadcrumb.html.j2
+-rw-r--r--   0 root         (0) root         (0)      415 2023-05-17 22:54:47.000000 aip-site-generator-0.6.3/aip_site/support/templates/includes/footer.html.j2
+-rw-r--r--   0 root         (0) root         (0)     5106 2023-05-17 22:54:47.000000 aip-site-generator-0.6.3/aip_site/support/templates/includes/header.html.j2
+-rw-r--r--   0 root         (0) root         (0)      986 2023-05-17 22:54:47.000000 aip-site-generator-0.6.3/aip_site/support/templates/includes/nav.html.j2
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 22:54:56.074308 aip-site-generator-0.6.3/aip_site/support/templates/includes/state_banners/
+-rw-r--r--   0 root         (0) root         (0)      189 2023-05-17 22:54:47.000000 aip-site-generator-0.6.3/aip_site/support/templates/includes/state_banners/draft.html.j2
+-rw-r--r--   0 root         (0) root         (0)      125 2023-05-17 22:54:47.000000 aip-site-generator-0.6.3/aip_site/support/templates/includes/state_banners/rejected.html.j2
+-rw-r--r--   0 root         (0) root         (0)      212 2023-05-17 22:54:47.000000 aip-site-generator-0.6.3/aip_site/support/templates/includes/state_banners/replaced.html.j2
+-rw-r--r--   0 root         (0) root         (0)      316 2023-05-17 22:54:47.000000 aip-site-generator-0.6.3/aip_site/support/templates/includes/state_banners/reviewing.html.j2
+-rw-r--r--   0 root         (0) root         (0)      126 2023-05-17 22:54:47.000000 aip-site-generator-0.6.3/aip_site/support/templates/includes/state_banners/withdrawn.html.j2
+-rw-r--r--   0 root         (0) root         (0)     1630 2023-05-17 22:54:47.000000 aip-site-generator-0.6.3/aip_site/support/templates/index.html.j2
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 22:54:56.074308 aip-site-generator-0.6.3/aip_site/support/templates/layouts/
+-rw-r--r--   0 root         (0) root         (0)     2696 2023-05-17 22:54:47.000000 aip-site-generator-0.6.3/aip_site/support/templates/layouts/base.html.j2
+-rw-r--r--   0 root         (0) root         (0)     1033 2023-05-17 22:54:47.000000 aip-site-generator-0.6.3/aip_site/support/templates/page.html.j2
+-rw-r--r--   0 root         (0) root         (0)      544 2023-05-17 22:54:47.000000 aip-site-generator-0.6.3/aip_site/support/templates/redirect.html.j2
+-rw-r--r--   0 root         (0) root         (0)     1508 2023-05-17 22:54:47.000000 aip-site-generator-0.6.3/aip_site/support/templates/search.html.j2
+-rw-r--r--   0 root         (0) root         (0)      443 2023-05-17 22:54:47.000000 aip-site-generator-0.6.3/aip_site/support/templates/search.js.j2
+-rw-r--r--   0 root         (0) root         (0)     1229 2023-05-17 22:54:47.000000 aip-site-generator-0.6.3/aip_site/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 22:54:56.074308 aip-site-generator-0.6.3/aip_site_generator.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     6051 2023-05-17 22:54:56.000000 aip-site-generator-0.6.3/aip_site_generator.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3071 2023-05-17 22:54:56.000000 aip-site-generator-0.6.3/aip_site_generator.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-17 22:54:56.000000 aip-site-generator-0.6.3/aip_site_generator.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       90 2023-05-17 22:54:56.000000 aip-site-generator-0.6.3/aip_site_generator.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-17 22:54:56.000000 aip-site-generator-0.6.3/aip_site_generator.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      310 2023-05-17 22:54:56.000000 aip-site-generator-0.6.3/aip_site_generator.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2023-05-17 22:54:56.000000 aip-site-generator-0.6.3/aip_site_generator.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-17 22:54:56.074308 aip-site-generator-0.6.3/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2588 2023-05-17 22:54:47.000000 aip-site-generator-0.6.3/setup.py
```

### Comparing `aip-site-generator-0.6.0/LICENSE` & `aip-site-generator-0.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `aip-site-generator-0.6.0/PKG-INFO` & `aip-site-generator-0.6.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aip-site-generator
-Version: 0.6.0
+Version: 0.6.3
 Summary: Static site generator for aip.dev and forks.
 Home-page: https://github.com/aip-dev/site-generator.git
 Author: Luke Sneeringer
 Author-email: lukesneeringer@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X
 Classifier: Development Status :: 4 - Beta
@@ -130,11 +130,54 @@
 
 ## My mo-betta foo bar baz
 
 Lorem ipsum dolor set something-not-amet
 {% endblock %}
 ```
 
+## Developer Setup
+If you want to contribute to this project you will want to have a setup where
+you can make changes to the code and see the result of your changes as soon as
+possible. Here is a quick way to set up a local development environment that
+will enable you to work on the code without having to reinstall the command
+line scripts.
+
+### Dependencies
+
+You'll need venv. On Linux, install with,
+
+```
+sudo apt-get install python3-venv
+```
+
+### Running dev env
+
+1. Check out the source
+
+```bash
+$ mkdir src
+$ cd src
+$ git clone https://github.com/aip-dev/site-generator.git
+```
+
+2. Setup python virtual environment
+
+```bash
+$ python3 -m venv .venv
+$ source .venv/bin/activate
+```
+
+3. PIP Install with the editable option
+
+```bash
+$ pip install --editable .
+```
+
+4. Serve the aip.dev site
+
+```bash
+$ aip-site-serve /path/to/aip/data/on/your/system
+```
+
 [dataclasses]: https://docs.python.org/3/library/dataclasses.html
 [jekyll]: https://jekyllrb.com/
 [jinja2]: https://jinja.palletsprojects.com/en/2.11.x/
-
```

### Comparing `aip-site-generator-0.6.0/README.md` & `aip-site-generator-0.6.3/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -110,10 +110,54 @@
 
 ## My mo-betta foo bar baz
 
 Lorem ipsum dolor set something-not-amet
 {% endblock %}
 ```
 
+## Developer Setup
+If you want to contribute to this project you will want to have a setup where
+you can make changes to the code and see the result of your changes as soon as
+possible. Here is a quick way to set up a local development environment that
+will enable you to work on the code without having to reinstall the command
+line scripts.
+
+### Dependencies
+
+You'll need venv. On Linux, install with,
+
+```
+sudo apt-get install python3-venv
+```
+
+### Running dev env
+
+1. Check out the source
+
+```bash
+$ mkdir src
+$ cd src
+$ git clone https://github.com/aip-dev/site-generator.git
+```
+
+2. Setup python virtual environment
+
+```bash
+$ python3 -m venv .venv
+$ source .venv/bin/activate
+```
+
+3. PIP Install with the editable option
+
+```bash
+$ pip install --editable .
+```
+
+4. Serve the aip.dev site
+
+```bash
+$ aip-site-serve /path/to/aip/data/on/your/system
+```
+
 [dataclasses]: https://docs.python.org/3/library/dataclasses.html
 [jekyll]: https://jekyllrb.com/
 [jinja2]: https://jinja.palletsprojects.com/en/2.11.x/
```

### Comparing `aip-site-generator-0.6.0/aip_site/cli.py` & `aip-site-generator-0.6.3/aip_site/cli.py`

 * *Files identical despite different names*

### Comparing `aip-site-generator-0.6.0/aip_site/jinja/env.py` & `aip-site-generator-0.6.3/aip_site/jinja/env.py`

 * *Files identical despite different names*

### Comparing `aip-site-generator-0.6.0/aip_site/jinja/ext/sample.py` & `aip-site-generator-0.6.3/aip_site/jinja/ext/sample.py`

 * *Files identical despite different names*

### Comparing `aip-site-generator-0.6.0/aip_site/jinja/ext/tab.py` & `aip-site-generator-0.6.3/aip_site/jinja/ext/tab.py`

 * *Files identical despite different names*

### Comparing `aip-site-generator-0.6.0/aip_site/jinja/loaders.py` & `aip-site-generator-0.6.3/aip_site/jinja/loaders.py`

 * *Files 1% similar despite different names*

```diff
@@ -70,15 +70,15 @@
             # Iterate over the individual components in the table
             # of contents and make each into a block.
             contents = MarkdownDocument(contents).blocked_content
 
         # Return the template information.
         return contents, fn, None
 
-    def list_templates(self) -> typing.Sequence[str]:
+    def list_templates(self) -> typing.List[str]:
         answer = []
 
         # We sort the files in the directory to read more specific
         # files first.
         exts_regex = r'(\.(j2|md|proto|oas|yaml))*$'
         for fn in sorted(os.listdir(self.aip.path),
                 key=lambda p: len(re.sub(exts_regex, '', p).split('.')),
```

### Comparing `aip-site-generator-0.6.0/aip_site/md.py` & `aip-site-generator-0.6.3/aip_site/md.py`

 * *Files identical despite different names*

### Comparing `aip-site-generator-0.6.0/aip_site/models/aip.py` & `aip-site-generator-0.6.3/aip_site/models/aip.py`

 * *Files 4% similar despite different names*

```diff
@@ -53,23 +53,24 @@
         answer = re.sub(
             r'\.?\./0([\d]{1,3})\.md',
             lambda m: f'{self.site.relative_uri}/{int(m.groups()[0]):d}',
             answer,
         )
 
         # Hotlink AIP references.
-        # We only hotlink the generally-applicable ones for now until we have
-        # a prefix system implemented.
+        # We can (now) link to AIPs outside of general, those that are numbered
+        # > 999, because the site redirects from 4221 to client-libraries/4221
+        # now, for example.
         answer = re.sub(
-            r'\b(?<!\[)AIP-([\d]{1,3})\b',  # AIP-###, but not after a `[`.
+            r'\b(?<!\[)AIP-(\d+)\b',  # AIP-###, but not after a `[`.
             fr'[AIP-\1]({self.site.relative_uri}/\1)',
             answer,
         )
         answer = re.sub(
-            r'(?<=\])\[aip-([\d]{1,3})\]',  # [aip-###], after a `]`.
+            r'(?<=\])\[aip-(\d+)\]',  # [aip-###], after a `]`.
             fr'({self.site.relative_uri}/\1)',
             answer,
         )
 
         # Append the changelog if there is one.
         if self.changelog:
             answer += '\n\n## Changelog\n\n'
```

### Comparing `aip-site-generator-0.6.0/aip_site/models/page.py` & `aip-site-generator-0.6.3/aip_site/models/page.py`

 * *Files identical despite different names*

### Comparing `aip-site-generator-0.6.0/aip_site/models/scope.py` & `aip-site-generator-0.6.3/aip_site/models/scope.py`

 * *Files identical despite different names*

### Comparing `aip-site-generator-0.6.0/aip_site/models/site.py` & `aip-site-generator-0.6.3/aip_site/models/site.py`

 * *Files identical despite different names*

### Comparing `aip-site-generator-0.6.0/aip_site/publisher.py` & `aip-site-generator-0.6.3/aip_site/publisher.py`

 * *Files identical despite different names*

### Comparing `aip-site-generator-0.6.0/aip_site/server.py` & `aip-site-generator-0.6.3/aip_site/server.py`

 * *Files 10% similar despite different names*

```diff
@@ -45,20 +45,27 @@
         site=flask.g.site,
         path=flask.request.path,
     )
 
 
 @app.route('/<page>')
 @app.route('/<collection>/<page>')
-def page(page: str, collection: str = 'general'):
+def page(page: str, collection: str = "general"):
     """Display a static page or listing of AIPs in a given scope."""
     site = flask.g.site
     if page in site.scopes:
         return site.scopes[page].render()
-    return site.collections[collection].pages[page].render()
+    if (
+        collection in site.collections and
+        page in site.collections[collection].pages
+    ):
+        return site.collections[collection].pages[page].render()
+    if collection in site.scopes and int(page) in site.scopes[collection].aips:
+        return site.scopes[collection].aips[int(page)].render()
+    flask.abort(404)
 
 
 @app.route('/assets/css/<path:css_file>')
 def scss(css_file: str):
     """Compile the given SCSS file and return it."""
     scss_file = re.sub(r'\.css$', '.scss', css_file)
     css = compile_file(f'{ROOT}/aip_site/support/scss/{scss_file}')
```

### Comparing `aip-site-generator-0.6.0/aip_site/support/assets/favicon.ico` & `aip-site-generator-0.6.3/aip_site/support/assets/favicon.ico`

 * *Files identical despite different names*

### Comparing `aip-site-generator-0.6.0/aip_site/support/assets/images/github.png` & `aip-site-generator-0.6.3/aip_site/support/assets/images/github.png`

 * *Files identical despite different names*

### Comparing `aip-site-generator-0.6.0/aip_site/support/assets/images/glue-icons.svg` & `aip-site-generator-0.6.3/aip_site/support/assets/images/glue-icons.svg`

 * *Files identical despite different names*

### Comparing `aip-site-generator-0.6.0/aip_site/support/assets/js/aip/aip-graphviz.js` & `aip-site-generator-0.6.3/aip_site/support/assets/js/aip/aip-graphviz.js`

 * *Files identical despite different names*

### Comparing `aip-site-generator-0.6.0/aip_site/support/assets/js/aip/aip-index.js` & `aip-site-generator-0.6.3/aip_site/support/assets/js/aip/aip-index.js`

 * *Files identical despite different names*

### Comparing `aip-site-generator-0.6.0/aip_site/support/assets/js/global.js` & `aip-site-generator-0.6.3/aip_site/support/assets/js/global.js`

 * *Files identical despite different names*

### Comparing `aip-site-generator-0.6.0/aip_site/support/assets/js/graphviz/lite.render.js` & `aip-site-generator-0.6.3/aip_site/support/assets/js/graphviz/lite.render.js`

 * *Files identical despite different names*

### Comparing `aip-site-generator-0.6.0/aip_site/support/assets/js/graphviz/viz.js` & `aip-site-generator-0.6.3/aip_site/support/assets/js/graphviz/viz.js`

 * *Files identical despite different names*

### Comparing `aip-site-generator-0.6.0/aip_site/support/assets/js/search/pagination.js` & `aip-site-generator-0.6.3/aip_site/support/assets/js/search/pagination.js`

 * *Files identical despite different names*

### Comparing `aip-site-generator-0.6.0/aip_site/support/assets/js/search/tipuesearch.min.js` & `aip-site-generator-0.6.3/aip_site/support/assets/js/search/tipuesearch.min.js`

 * *Files identical despite different names*

### Comparing `aip-site-generator-0.6.0/aip_site/support/assets/js/search/tipuesearch_set.js` & `aip-site-generator-0.6.3/aip_site/support/assets/js/search/tipuesearch_set.js`

 * *Files identical despite different names*

### Comparing `aip-site-generator-0.6.0/aip_site/support/assets/js/syntax.js` & `aip-site-generator-0.6.3/aip_site/support/assets/js/syntax.js`

 * *Files identical despite different names*

### Comparing `aip-site-generator-0.6.0/aip_site/support/assets/misc/ebnf-filtering.txt` & `aip-site-generator-0.6.3/aip_site/support/assets/misc/ebnf-filtering.txt`

 * *Files identical despite different names*

### Comparing `aip-site-generator-0.6.0/aip_site/support/scss/hero.scss` & `aip-site-generator-0.6.3/aip_site/support/scss/hero.scss`

 * *Files identical despite different names*

### Comparing `aip-site-generator-0.6.0/aip_site/support/scss/imports/aip/news.scss` & `aip-site-generator-0.6.3/aip_site/support/scss/imports/aip/news.scss`

 * *Files identical despite different names*

### Comparing `aip-site-generator-0.6.0/aip_site/support/scss/imports/aip/tables.scss` & `aip-site-generator-0.6.3/aip_site/support/scss/imports/aip/tables.scss`

 * *Files identical despite different names*

### Comparing `aip-site-generator-0.6.0/aip_site/support/scss/imports/callouts.scss` & `aip-site-generator-0.6.3/aip_site/support/scss/imports/callouts.scss`

 * *Files 7% similar despite different names*

```diff
@@ -1,17 +1,21 @@
 @import 'imports/colors';
 
 .callout {
-  margin-top: 5px;
+  margin-top: 10px;
   margin-left: 20px;
   margin-right: 20px;
   padding: 10px 20px;
   color: $glue-grey-800;
 }
 
+.callout + .callout {
+  margin-top: 15px;
+}
+
 .important {
   @extend .callout;
   background-color: $glue-yellow-50;
   border: 1px solid $glue-yellow-200;
 }
 
 .note {
```

### Comparing `aip-site-generator-0.6.0/aip_site/support/scss/imports/colors.scss` & `aip-site-generator-0.6.3/aip_site/support/scss/imports/colors.scss`

 * *Files identical despite different names*

### Comparing `aip-site-generator-0.6.0/aip_site/support/scss/imports/header.scss` & `aip-site-generator-0.6.3/aip_site/support/scss/imports/header.scss`

 * *Files identical despite different names*

### Comparing `aip-site-generator-0.6.0/aip_site/support/scss/imports/headings.scss` & `aip-site-generator-0.6.3/aip_site/support/scss/imports/headings.scss`

 * *Files 22% similar despite different names*

```diff
@@ -1,31 +1,37 @@
 // Headers
 .docs-component-main {
   h1,
   h2,
   h3,
   h4,
-  h5 {
+  h5,
+  a[name] {
     // This creates a "fake block" above the header that does not show up
     // anywhere but tricks the browser into thinking that the anchor is 80px
     // higher than it actually is.
+    cursor: default;
+    outline: none;
+
     &::before {
       display: block;
       content: ' ';
       height: 80px;
       margin-top: -80px;
       pointer-events: none;
       visibility: hidden;
     }
 
     a {
       text-decoration: none;
     }
   }
   h4 {
+    padding-bottom: 5px;
+
     &.aip-number {
       line-height: 1em;
 
       & + h1 {
         margin-top: 0px;
         margin-left: -2px;
       }
```

### Comparing `aip-site-generator-0.6.0/aip_site/support/scss/imports/nav.scss` & `aip-site-generator-0.6.3/aip_site/support/scss/imports/nav.scss`

 * *Files identical despite different names*

### Comparing `aip-site-generator-0.6.0/aip_site/support/scss/imports/sidebar.scss` & `aip-site-generator-0.6.3/aip_site/support/scss/imports/sidebar.scss`

 * *Files identical despite different names*

### Comparing `aip-site-generator-0.6.0/aip_site/support/scss/imports/syntax.scss` & `aip-site-generator-0.6.3/aip_site/support/scss/imports/syntax.scss`

 * *Files identical despite different names*

### Comparing `aip-site-generator-0.6.0/aip_site/support/scss/imports/tabs.scss` & `aip-site-generator-0.6.3/aip_site/support/scss/imports/tabs.scss`

 * *Files identical despite different names*

### Comparing `aip-site-generator-0.6.0/aip_site/support/scss/print.scss` & `aip-site-generator-0.6.3/aip_site/support/scss/print.scss`

 * *Files identical despite different names*

### Comparing `aip-site-generator-0.6.0/aip_site/support/scss/search.scss` & `aip-site-generator-0.6.3/aip_site/support/scss/search.scss`

 * *Files identical despite different names*

### Comparing `aip-site-generator-0.6.0/aip_site/support/templates/aip-listing.html.j2` & `aip-site-generator-0.6.3/aip_site/support/templates/aip-listing.html.j2`

 * *Files identical despite different names*

### Comparing `aip-site-generator-0.6.0/aip_site/support/templates/aip.html.j2` & `aip-site-generator-0.6.3/aip_site/support/templates/aip.html.j2`

 * *Files identical despite different names*

### Comparing `aip-site-generator-0.6.0/aip_site/support/templates/includes/breadcrumb.html.j2` & `aip-site-generator-0.6.3/aip_site/support/templates/includes/breadcrumb.html.j2`

 * *Files identical despite different names*

### Comparing `aip-site-generator-0.6.0/aip_site/support/templates/includes/header.html.j2` & `aip-site-generator-0.6.3/aip_site/support/templates/includes/header.html.j2`

 * *Files identical despite different names*

### Comparing `aip-site-generator-0.6.0/aip_site/support/templates/includes/nav.html.j2` & `aip-site-generator-0.6.3/aip_site/support/templates/includes/nav.html.j2`

 * *Files identical despite different names*

### Comparing `aip-site-generator-0.6.0/aip_site/support/templates/index.html.j2` & `aip-site-generator-0.6.3/aip_site/support/templates/index.html.j2`

 * *Files identical despite different names*

### Comparing `aip-site-generator-0.6.0/aip_site/support/templates/layouts/base.html.j2` & `aip-site-generator-0.6.3/aip_site/support/templates/layouts/base.html.j2`

 * *Files identical despite different names*

### Comparing `aip-site-generator-0.6.0/aip_site/support/templates/page.html.j2` & `aip-site-generator-0.6.3/aip_site/support/templates/page.html.j2`

 * *Files identical despite different names*

### Comparing `aip-site-generator-0.6.0/aip_site/support/templates/redirect.html.j2` & `aip-site-generator-0.6.3/aip_site/support/templates/redirect.html.j2`

 * *Files identical despite different names*

### Comparing `aip-site-generator-0.6.0/aip_site/support/templates/search.html.j2` & `aip-site-generator-0.6.3/aip_site/support/templates/search.html.j2`

 * *Files identical despite different names*

### Comparing `aip-site-generator-0.6.0/aip_site/utils.py` & `aip-site-generator-0.6.3/aip_site/utils.py`

 * *Files identical despite different names*

### Comparing `aip-site-generator-0.6.0/aip_site_generator.egg-info/PKG-INFO` & `aip-site-generator-0.6.3/aip_site_generator.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aip-site-generator
-Version: 0.6.0
+Version: 0.6.3
 Summary: Static site generator for aip.dev and forks.
 Home-page: https://github.com/aip-dev/site-generator.git
 Author: Luke Sneeringer
 Author-email: lukesneeringer@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X
 Classifier: Development Status :: 4 - Beta
@@ -130,11 +130,54 @@
 
 ## My mo-betta foo bar baz
 
 Lorem ipsum dolor set something-not-amet
 {% endblock %}
 ```
 
+## Developer Setup
+If you want to contribute to this project you will want to have a setup where
+you can make changes to the code and see the result of your changes as soon as
+possible. Here is a quick way to set up a local development environment that
+will enable you to work on the code without having to reinstall the command
+line scripts.
+
+### Dependencies
+
+You'll need venv. On Linux, install with,
+
+```
+sudo apt-get install python3-venv
+```
+
+### Running dev env
+
+1. Check out the source
+
+```bash
+$ mkdir src
+$ cd src
+$ git clone https://github.com/aip-dev/site-generator.git
+```
+
+2. Setup python virtual environment
+
+```bash
+$ python3 -m venv .venv
+$ source .venv/bin/activate
+```
+
+3. PIP Install with the editable option
+
+```bash
+$ pip install --editable .
+```
+
+4. Serve the aip.dev site
+
+```bash
+$ aip-site-serve /path/to/aip/data/on/your/system
+```
+
 [dataclasses]: https://docs.python.org/3/library/dataclasses.html
 [jekyll]: https://jekyllrb.com/
 [jinja2]: https://jinja.palletsprojects.com/en/2.11.x/
-
```

### Comparing `aip-site-generator-0.6.0/aip_site_generator.egg-info/SOURCES.txt` & `aip-site-generator-0.6.3/aip_site_generator.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aip-site-generator-0.6.0/setup.py` & `aip-site-generator-0.6.3/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 # Copyright 2020 Google LLC
 #
-# Licensed under the Apache License, Version 2.0 (the "License");
+# Licensed under the Apache License, Version 2.0 (the 'License');
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     https://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
+# distributed under the License is distributed on an 'AS IS' BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import io
 import os
 
@@ -33,39 +33,43 @@
     author='Luke Sneeringer',
     author_email='lukesneeringer@google.com',
     url='https://github.com/aip-dev/site-generator.git',
     packages=find_packages(exclude=['tests']),
     description='Static site generator for aip.dev and forks.',
     long_description=long_description,
     long_description_content_type='text/markdown',
-    entry_points="""[console_scripts]
+    entry_points='''[console_scripts]
         aip-site-gen=aip_site.cli:publish
         aip-site-serve=aip_site.cli:serve
-    """,
+    ''',
     platforms='Posix; MacOS X',
     include_package_data=True,
     install_requires=(
-        'click==8.0.1',
-        'flask==2.0.1',
-        'itsdangerous==2.0.1',
-        'jinja2==3.0.1',
-        'markdown==3.3.4',
-        'markupsafe==2.0.1',
-        'pygments==2.9.0',
-        'pymdown-extensions==8.2',
-        'pyscss==1.3.7',
-        'pyyaml==5.4.1',
+        'click==8.1.3',
+        'flask==2.2.2',
+        'itsdangerous==2.1.2',
+        'jinja2==3.1.2',
+        'markdown==3.4.1',
+        'markupsafe==2.1.1',
+        'pygments==2.13.0',
+        'pymdown-extensions==9.7',
+        # pinning via GitHub release until https://github.com/Kronuz/pyScss/pull/426
+        # is released on PyPi.
+        'pyscss @ git+https://github.com/Kronuz/pyScss.git@73559d047706ccd4593cf6aa092de71f35164723',
+        'pyyaml==6.0',
         'six==1.16.0',
-        'werkzeug==2.0.1',
+        'types-Markdown==3.4.2.1',
+        'types-PyYAML==6.0.12',
+        'werkzeug==2.2.2',
     ),
     python_requires='>=3.8',
-    classifiers=(
+    classifiers=[
         'Development Status :: 4 - Beta',
         'Environment :: Console',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: Apache Software License',
         'Operating System :: POSIX',
         'Programming Language :: Python :: 3.8',
         'Topic :: Software Development :: Code Generators',
-    ),
+    ],
     zip_safe=False,
 )
```

