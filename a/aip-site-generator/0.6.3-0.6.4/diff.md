# Comparing `tmp/aip-site-generator-0.6.3.tar.gz` & `tmp/aip-site-generator-0.6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aip-site-generator-0.6.3.tar", last modified: Wed May 17 22:54:56 2023, max compression
+gzip compressed data, was "aip-site-generator-0.6.4.tar", last modified: Thu May 18 18:39:29 2023, max compression
```

## Comparing `aip-site-generator-0.6.3.tar` & `aip-site-generator-0.6.4.tar`

### file list

```diff
@@ -1,103 +1,103 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 22:54:56.074308 aip-site-generator-0.6.3/
--rw-r--r--   0 root         (0) root         (0)    11359 2023-05-17 22:54:47.000000 aip-site-generator-0.6.3/LICENSE
--rw-r--r--   0 root         (0) root         (0)      138 2023-05-17 22:54:47.000000 aip-site-generator-0.6.3/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     6051 2023-05-17 22:54:56.074308 aip-site-generator-0.6.3/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     5349 2023-05-17 22:54:47.000000 aip-site-generator-0.6.3/README.md
--rw-r--r--   0 root         (0) root         (0)        6 2023-05-17 22:54:55.000000 aip-site-generator-0.6.3/VERSION
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 22:54:56.062308 aip-site-generator-0.6.3/aip_site/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-17 22:54:47.000000 aip-site-generator-0.6.3/aip_site/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1446 2023-05-17 22:54:47.000000 aip-site-generator-0.6.3/aip_site/cli.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 22:54:56.062308 aip-site-generator-0.6.3/aip_site/jinja/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-17 22:54:47.000000 aip-site-generator-0.6.3/aip_site/jinja/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1044 2023-05-17 22:54:47.000000 aip-site-generator-0.6.3/aip_site/jinja/env.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 22:54:56.062308 aip-site-generator-0.6.3/aip_site/jinja/ext/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-17 22:54:47.000000 aip-site-generator-0.6.3/aip_site/jinja/ext/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5484 2023-05-17 22:54:47.000000 aip-site-generator-0.6.3/aip_site/jinja/ext/sample.py
--rw-r--r--   0 root         (0) root         (0)     2082 2023-05-17 22:54:47.000000 aip-site-generator-0.6.3/aip_site/jinja/ext/tab.py
--rw-r--r--   0 root         (0) root         (0)     3264 2023-05-17 22:54:47.000000 aip-site-generator-0.6.3/aip_site/jinja/loaders.py
--rw-r--r--   0 root         (0) root         (0)     5319 2023-05-17 22:54:47.000000 aip-site-generator-0.6.3/aip_site/md.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 22:54:56.066308 aip-site-generator-0.6.3/aip_site/models/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-17 22:54:47.000000 aip-site-generator-0.6.3/aip_site/models/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6280 2023-05-17 22:54:47.000000 aip-site-generator-0.6.3/aip_site/models/aip.py
--rw-r--r--   0 root         (0) root         (0)     4107 2023-05-17 22:54:47.000000 aip-site-generator-0.6.3/aip_site/models/page.py
--rw-r--r--   0 root         (0) root         (0)     4572 2023-05-17 22:54:47.000000 aip-site-generator-0.6.3/aip_site/models/scope.py
--rw-r--r--   0 root         (0) root         (0)     4611 2023-05-17 22:54:47.000000 aip-site-generator-0.6.3/aip_site/models/site.py
--rw-r--r--   0 root         (0) root         (0)     4681 2023-05-17 22:54:47.000000 aip-site-generator-0.6.3/aip_site/publisher.py
--rw-r--r--   0 root         (0) root         (0)     3014 2023-05-17 22:54:47.000000 aip-site-generator-0.6.3/aip_site/server.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 22:54:56.062308 aip-site-generator-0.6.3/aip_site/support/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 22:54:56.066308 aip-site-generator-0.6.3/aip_site/support/assets/
--rw-r--r--   0 root         (0) root         (0)     5430 2023-05-17 22:54:47.000000 aip-site-generator-0.6.3/aip_site/support/assets/favicon.ico
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 22:54:56.066308 aip-site-generator-0.6.3/aip_site/support/assets/images/
--rw-r--r--   0 root         (0) root         (0)     4044 2023-05-17 22:54:47.000000 aip-site-generator-0.6.3/aip_site/support/assets/images/github.png
--rw-r--r--   0 root         (0) root         (0)    13956 2023-05-17 22:54:47.000000 aip-site-generator-0.6.3/aip_site/support/assets/images/glue-icons.svg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 22:54:56.066308 aip-site-generator-0.6.3/aip_site/support/assets/js/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 22:54:56.066308 aip-site-generator-0.6.3/aip_site/support/assets/js/aip/
--rw-r--r--   0 root         (0) root         (0)     1399 2023-05-17 22:54:47.000000 aip-site-generator-0.6.3/aip_site/support/assets/js/aip/aip-graphviz.js
--rw-r--r--   0 root         (0) root         (0)      992 2023-05-17 22:54:47.000000 aip-site-generator-0.6.3/aip_site/support/assets/js/aip/aip-index.js
--rw-r--r--   0 root         (0) root         (0)     2867 2023-05-17 22:54:47.000000 aip-site-generator-0.6.3/aip_site/support/assets/js/global.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 22:54:56.066308 aip-site-generator-0.6.3/aip_site/support/assets/js/graphviz/
--rw-r--r--   0 root         (0) root         (0)  1439383 2023-05-17 22:54:47.000000 aip-site-generator-0.6.3/aip_site/support/assets/js/graphviz/lite.render.js
--rw-r--r--   0 root         (0) root         (0)    11468 2023-05-17 22:54:47.000000 aip-site-generator-0.6.3/aip_site/support/assets/js/graphviz/viz.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 22:54:56.066308 aip-site-generator-0.6.3/aip_site/support/assets/js/search/
--rw-r--r--   0 root         (0) root         (0)      982 2023-05-17 22:54:47.000000 aip-site-generator-0.6.3/aip_site/support/assets/js/search/pagination.js
--rw-r--r--   0 root         (0) root         (0)    10308 2023-05-17 22:54:47.000000 aip-site-generator-0.6.3/aip_site/support/assets/js/search/tipuesearch.min.js
--rw-r--r--   0 root         (0) root         (0)     3456 2023-05-17 22:54:47.000000 aip-site-generator-0.6.3/aip_site/support/assets/js/search/tipuesearch_set.js
--rw-r--r--   0 root         (0) root         (0)     3925 2023-05-17 22:54:47.000000 aip-site-generator-0.6.3/aip_site/support/assets/js/syntax.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 22:54:56.066308 aip-site-generator-0.6.3/aip_site/support/assets/misc/
--rw-r--r--   0 root         (0) root         (0)     4775 2023-05-17 22:54:47.000000 aip-site-generator-0.6.3/aip_site/support/assets/misc/ebnf-filtering.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 22:54:56.070309 aip-site-generator-0.6.3/aip_site/support/scss/
--rw-r--r--   0 root         (0) root         (0)      851 2023-05-17 22:54:47.000000 aip-site-generator-0.6.3/aip_site/support/scss/hero.scss
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 22:54:56.070309 aip-site-generator-0.6.3/aip_site/support/scss/imports/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 22:54:56.070309 aip-site-generator-0.6.3/aip_site/support/scss/imports/aip/
--rw-r--r--   0 root         (0) root         (0)      443 2023-05-17 22:54:47.000000 aip-site-generator-0.6.3/aip_site/support/scss/imports/aip/badges.scss
--rw-r--r--   0 root         (0) root         (0)      218 2023-05-17 22:54:47.000000 aip-site-generator-0.6.3/aip_site/support/scss/imports/aip/breadcrumbs.scss
--rw-r--r--   0 root         (0) root         (0)       67 2023-05-17 22:54:47.000000 aip-site-generator-0.6.3/aip_site/support/scss/imports/aip/header.scss
--rw-r--r--   0 root         (0) root         (0)      184 2023-05-17 22:54:47.000000 aip-site-generator-0.6.3/aip_site/support/scss/imports/aip/nav.scss
--rw-r--r--   0 root         (0) root         (0)      611 2023-05-17 22:54:47.000000 aip-site-generator-0.6.3/aip_site/support/scss/imports/aip/news.scss
--rw-r--r--   0 root         (0) root         (0)     1288 2023-05-17 22:54:47.000000 aip-site-generator-0.6.3/aip_site/support/scss/imports/aip/tables.scss
--rw-r--r--   0 root         (0) root         (0)      988 2023-05-17 22:54:47.000000 aip-site-generator-0.6.3/aip_site/support/scss/imports/callouts.scss
--rw-r--r--   0 root         (0) root         (0)     4017 2023-05-17 22:54:47.000000 aip-site-generator-0.6.3/aip_site/support/scss/imports/colors.scss
--rw-r--r--   0 root         (0) root         (0)      240 2023-05-17 22:54:47.000000 aip-site-generator-0.6.3/aip_site/support/scss/imports/footer.scss
--rw-r--r--   0 root         (0) root         (0)     1211 2023-05-17 22:54:47.000000 aip-site-generator-0.6.3/aip_site/support/scss/imports/header.scss
--rw-r--r--   0 root         (0) root         (0)      678 2023-05-17 22:54:47.000000 aip-site-generator-0.6.3/aip_site/support/scss/imports/headings.scss
--rw-r--r--   0 root         (0) root         (0)      128 2023-05-17 22:54:47.000000 aip-site-generator-0.6.3/aip_site/support/scss/imports/lists.scss
--rw-r--r--   0 root         (0) root         (0)     2655 2023-05-17 22:54:47.000000 aip-site-generator-0.6.3/aip_site/support/scss/imports/nav.scss
--rw-r--r--   0 root         (0) root         (0)     1266 2023-05-17 22:54:47.000000 aip-site-generator-0.6.3/aip_site/support/scss/imports/sidebar.scss
--rw-r--r--   0 root         (0) root         (0)     3426 2023-05-17 22:54:47.000000 aip-site-generator-0.6.3/aip_site/support/scss/imports/syntax.scss
--rw-r--r--   0 root         (0) root         (0)      102 2023-05-17 22:54:47.000000 aip-site-generator-0.6.3/aip_site/support/scss/imports/tables.scss
--rw-r--r--   0 root         (0) root         (0)      889 2023-05-17 22:54:47.000000 aip-site-generator-0.6.3/aip_site/support/scss/imports/tabs.scss
--rw-r--r--   0 root         (0) root         (0)     1053 2023-05-17 22:54:47.000000 aip-site-generator-0.6.3/aip_site/support/scss/print.scss
--rw-r--r--   0 root         (0) root         (0)     1429 2023-05-17 22:54:47.000000 aip-site-generator-0.6.3/aip_site/support/scss/search.scss
--rw-r--r--   0 root         (0) root         (0)      466 2023-05-17 22:54:47.000000 aip-site-generator-0.6.3/aip_site/support/scss/style.scss
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 22:54:56.074308 aip-site-generator-0.6.3/aip_site/support/templates/
--rw-r--r--   0 root         (0) root         (0)     1865 2023-05-17 22:54:47.000000 aip-site-generator-0.6.3/aip_site/support/templates/aip-listing.html.j2
--rw-r--r--   0 root         (0) root         (0)     2178 2023-05-17 22:54:47.000000 aip-site-generator-0.6.3/aip_site/support/templates/aip.html.j2
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 22:54:56.074308 aip-site-generator-0.6.3/aip_site/support/templates/includes/
--rw-r--r--   0 root         (0) root         (0)     1053 2023-05-17 22:54:47.000000 aip-site-generator-0.6.3/aip_site/support/templates/includes/breadcrumb.html.j2
--rw-r--r--   0 root         (0) root         (0)      415 2023-05-17 22:54:47.000000 aip-site-generator-0.6.3/aip_site/support/templates/includes/footer.html.j2
--rw-r--r--   0 root         (0) root         (0)     5106 2023-05-17 22:54:47.000000 aip-site-generator-0.6.3/aip_site/support/templates/includes/header.html.j2
--rw-r--r--   0 root         (0) root         (0)      986 2023-05-17 22:54:47.000000 aip-site-generator-0.6.3/aip_site/support/templates/includes/nav.html.j2
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 22:54:56.074308 aip-site-generator-0.6.3/aip_site/support/templates/includes/state_banners/
--rw-r--r--   0 root         (0) root         (0)      189 2023-05-17 22:54:47.000000 aip-site-generator-0.6.3/aip_site/support/templates/includes/state_banners/draft.html.j2
--rw-r--r--   0 root         (0) root         (0)      125 2023-05-17 22:54:47.000000 aip-site-generator-0.6.3/aip_site/support/templates/includes/state_banners/rejected.html.j2
--rw-r--r--   0 root         (0) root         (0)      212 2023-05-17 22:54:47.000000 aip-site-generator-0.6.3/aip_site/support/templates/includes/state_banners/replaced.html.j2
--rw-r--r--   0 root         (0) root         (0)      316 2023-05-17 22:54:47.000000 aip-site-generator-0.6.3/aip_site/support/templates/includes/state_banners/reviewing.html.j2
--rw-r--r--   0 root         (0) root         (0)      126 2023-05-17 22:54:47.000000 aip-site-generator-0.6.3/aip_site/support/templates/includes/state_banners/withdrawn.html.j2
--rw-r--r--   0 root         (0) root         (0)     1630 2023-05-17 22:54:47.000000 aip-site-generator-0.6.3/aip_site/support/templates/index.html.j2
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 22:54:56.074308 aip-site-generator-0.6.3/aip_site/support/templates/layouts/
--rw-r--r--   0 root         (0) root         (0)     2696 2023-05-17 22:54:47.000000 aip-site-generator-0.6.3/aip_site/support/templates/layouts/base.html.j2
--rw-r--r--   0 root         (0) root         (0)     1033 2023-05-17 22:54:47.000000 aip-site-generator-0.6.3/aip_site/support/templates/page.html.j2
--rw-r--r--   0 root         (0) root         (0)      544 2023-05-17 22:54:47.000000 aip-site-generator-0.6.3/aip_site/support/templates/redirect.html.j2
--rw-r--r--   0 root         (0) root         (0)     1508 2023-05-17 22:54:47.000000 aip-site-generator-0.6.3/aip_site/support/templates/search.html.j2
--rw-r--r--   0 root         (0) root         (0)      443 2023-05-17 22:54:47.000000 aip-site-generator-0.6.3/aip_site/support/templates/search.js.j2
--rw-r--r--   0 root         (0) root         (0)     1229 2023-05-17 22:54:47.000000 aip-site-generator-0.6.3/aip_site/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 22:54:56.074308 aip-site-generator-0.6.3/aip_site_generator.egg-info/
--rw-r--r--   0 root         (0) root         (0)     6051 2023-05-17 22:54:56.000000 aip-site-generator-0.6.3/aip_site_generator.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3071 2023-05-17 22:54:56.000000 aip-site-generator-0.6.3/aip_site_generator.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-17 22:54:56.000000 aip-site-generator-0.6.3/aip_site_generator.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       90 2023-05-17 22:54:56.000000 aip-site-generator-0.6.3/aip_site_generator.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-17 22:54:56.000000 aip-site-generator-0.6.3/aip_site_generator.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      310 2023-05-17 22:54:56.000000 aip-site-generator-0.6.3/aip_site_generator.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        9 2023-05-17 22:54:56.000000 aip-site-generator-0.6.3/aip_site_generator.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-17 22:54:56.074308 aip-site-generator-0.6.3/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2588 2023-05-17 22:54:47.000000 aip-site-generator-0.6.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 18:39:29.424228 aip-site-generator-0.6.4/
+-rw-r--r--   0 root         (0) root         (0)    11359 2023-05-18 18:39:20.000000 aip-site-generator-0.6.4/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      138 2023-05-18 18:39:20.000000 aip-site-generator-0.6.4/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     6051 2023-05-18 18:39:29.424228 aip-site-generator-0.6.4/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     5349 2023-05-18 18:39:20.000000 aip-site-generator-0.6.4/README.md
+-rw-r--r--   0 root         (0) root         (0)        6 2023-05-18 18:39:28.000000 aip-site-generator-0.6.4/VERSION
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 18:39:29.412228 aip-site-generator-0.6.4/aip_site/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 18:39:20.000000 aip-site-generator-0.6.4/aip_site/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1446 2023-05-18 18:39:20.000000 aip-site-generator-0.6.4/aip_site/cli.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 18:39:29.412228 aip-site-generator-0.6.4/aip_site/jinja/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 18:39:20.000000 aip-site-generator-0.6.4/aip_site/jinja/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1044 2023-05-18 18:39:20.000000 aip-site-generator-0.6.4/aip_site/jinja/env.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 18:39:29.416228 aip-site-generator-0.6.4/aip_site/jinja/ext/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 18:39:20.000000 aip-site-generator-0.6.4/aip_site/jinja/ext/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5484 2023-05-18 18:39:20.000000 aip-site-generator-0.6.4/aip_site/jinja/ext/sample.py
+-rw-r--r--   0 root         (0) root         (0)     2082 2023-05-18 18:39:20.000000 aip-site-generator-0.6.4/aip_site/jinja/ext/tab.py
+-rw-r--r--   0 root         (0) root         (0)     3264 2023-05-18 18:39:20.000000 aip-site-generator-0.6.4/aip_site/jinja/loaders.py
+-rw-r--r--   0 root         (0) root         (0)     5319 2023-05-18 18:39:20.000000 aip-site-generator-0.6.4/aip_site/md.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 18:39:29.416228 aip-site-generator-0.6.4/aip_site/models/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 18:39:20.000000 aip-site-generator-0.6.4/aip_site/models/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6280 2023-05-18 18:39:20.000000 aip-site-generator-0.6.4/aip_site/models/aip.py
+-rw-r--r--   0 root         (0) root         (0)     4107 2023-05-18 18:39:20.000000 aip-site-generator-0.6.4/aip_site/models/page.py
+-rw-r--r--   0 root         (0) root         (0)     4572 2023-05-18 18:39:20.000000 aip-site-generator-0.6.4/aip_site/models/scope.py
+-rw-r--r--   0 root         (0) root         (0)     4611 2023-05-18 18:39:20.000000 aip-site-generator-0.6.4/aip_site/models/site.py
+-rw-r--r--   0 root         (0) root         (0)     4681 2023-05-18 18:39:20.000000 aip-site-generator-0.6.4/aip_site/publisher.py
+-rw-r--r--   0 root         (0) root         (0)     3014 2023-05-18 18:39:20.000000 aip-site-generator-0.6.4/aip_site/server.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 18:39:29.412228 aip-site-generator-0.6.4/aip_site/support/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 18:39:29.416228 aip-site-generator-0.6.4/aip_site/support/assets/
+-rw-r--r--   0 root         (0) root         (0)     5430 2023-05-18 18:39:20.000000 aip-site-generator-0.6.4/aip_site/support/assets/favicon.ico
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 18:39:29.416228 aip-site-generator-0.6.4/aip_site/support/assets/images/
+-rw-r--r--   0 root         (0) root         (0)     4044 2023-05-18 18:39:20.000000 aip-site-generator-0.6.4/aip_site/support/assets/images/github.png
+-rw-r--r--   0 root         (0) root         (0)    13956 2023-05-18 18:39:20.000000 aip-site-generator-0.6.4/aip_site/support/assets/images/glue-icons.svg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 18:39:29.416228 aip-site-generator-0.6.4/aip_site/support/assets/js/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 18:39:29.416228 aip-site-generator-0.6.4/aip_site/support/assets/js/aip/
+-rw-r--r--   0 root         (0) root         (0)     1399 2023-05-18 18:39:20.000000 aip-site-generator-0.6.4/aip_site/support/assets/js/aip/aip-graphviz.js
+-rw-r--r--   0 root         (0) root         (0)      992 2023-05-18 18:39:20.000000 aip-site-generator-0.6.4/aip_site/support/assets/js/aip/aip-index.js
+-rw-r--r--   0 root         (0) root         (0)     2867 2023-05-18 18:39:20.000000 aip-site-generator-0.6.4/aip_site/support/assets/js/global.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 18:39:29.420228 aip-site-generator-0.6.4/aip_site/support/assets/js/graphviz/
+-rw-r--r--   0 root         (0) root         (0)  1439383 2023-05-18 18:39:20.000000 aip-site-generator-0.6.4/aip_site/support/assets/js/graphviz/lite.render.js
+-rw-r--r--   0 root         (0) root         (0)    11468 2023-05-18 18:39:20.000000 aip-site-generator-0.6.4/aip_site/support/assets/js/graphviz/viz.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 18:39:29.420228 aip-site-generator-0.6.4/aip_site/support/assets/js/search/
+-rw-r--r--   0 root         (0) root         (0)      982 2023-05-18 18:39:20.000000 aip-site-generator-0.6.4/aip_site/support/assets/js/search/pagination.js
+-rw-r--r--   0 root         (0) root         (0)    10308 2023-05-18 18:39:20.000000 aip-site-generator-0.6.4/aip_site/support/assets/js/search/tipuesearch.min.js
+-rw-r--r--   0 root         (0) root         (0)     3456 2023-05-18 18:39:20.000000 aip-site-generator-0.6.4/aip_site/support/assets/js/search/tipuesearch_set.js
+-rw-r--r--   0 root         (0) root         (0)     3925 2023-05-18 18:39:20.000000 aip-site-generator-0.6.4/aip_site/support/assets/js/syntax.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 18:39:29.420228 aip-site-generator-0.6.4/aip_site/support/assets/misc/
+-rw-r--r--   0 root         (0) root         (0)     4775 2023-05-18 18:39:20.000000 aip-site-generator-0.6.4/aip_site/support/assets/misc/ebnf-filtering.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 18:39:29.420228 aip-site-generator-0.6.4/aip_site/support/scss/
+-rw-r--r--   0 root         (0) root         (0)      851 2023-05-18 18:39:20.000000 aip-site-generator-0.6.4/aip_site/support/scss/hero.scss
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 18:39:29.420228 aip-site-generator-0.6.4/aip_site/support/scss/imports/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 18:39:29.420228 aip-site-generator-0.6.4/aip_site/support/scss/imports/aip/
+-rw-r--r--   0 root         (0) root         (0)      443 2023-05-18 18:39:20.000000 aip-site-generator-0.6.4/aip_site/support/scss/imports/aip/badges.scss
+-rw-r--r--   0 root         (0) root         (0)      218 2023-05-18 18:39:20.000000 aip-site-generator-0.6.4/aip_site/support/scss/imports/aip/breadcrumbs.scss
+-rw-r--r--   0 root         (0) root         (0)       67 2023-05-18 18:39:20.000000 aip-site-generator-0.6.4/aip_site/support/scss/imports/aip/header.scss
+-rw-r--r--   0 root         (0) root         (0)      184 2023-05-18 18:39:20.000000 aip-site-generator-0.6.4/aip_site/support/scss/imports/aip/nav.scss
+-rw-r--r--   0 root         (0) root         (0)      611 2023-05-18 18:39:20.000000 aip-site-generator-0.6.4/aip_site/support/scss/imports/aip/news.scss
+-rw-r--r--   0 root         (0) root         (0)     1288 2023-05-18 18:39:20.000000 aip-site-generator-0.6.4/aip_site/support/scss/imports/aip/tables.scss
+-rw-r--r--   0 root         (0) root         (0)      988 2023-05-18 18:39:20.000000 aip-site-generator-0.6.4/aip_site/support/scss/imports/callouts.scss
+-rw-r--r--   0 root         (0) root         (0)     4017 2023-05-18 18:39:20.000000 aip-site-generator-0.6.4/aip_site/support/scss/imports/colors.scss
+-rw-r--r--   0 root         (0) root         (0)      240 2023-05-18 18:39:20.000000 aip-site-generator-0.6.4/aip_site/support/scss/imports/footer.scss
+-rw-r--r--   0 root         (0) root         (0)     1211 2023-05-18 18:39:20.000000 aip-site-generator-0.6.4/aip_site/support/scss/imports/header.scss
+-rw-r--r--   0 root         (0) root         (0)      678 2023-05-18 18:39:20.000000 aip-site-generator-0.6.4/aip_site/support/scss/imports/headings.scss
+-rw-r--r--   0 root         (0) root         (0)      128 2023-05-18 18:39:20.000000 aip-site-generator-0.6.4/aip_site/support/scss/imports/lists.scss
+-rw-r--r--   0 root         (0) root         (0)     2655 2023-05-18 18:39:20.000000 aip-site-generator-0.6.4/aip_site/support/scss/imports/nav.scss
+-rw-r--r--   0 root         (0) root         (0)     1266 2023-05-18 18:39:20.000000 aip-site-generator-0.6.4/aip_site/support/scss/imports/sidebar.scss
+-rw-r--r--   0 root         (0) root         (0)     3426 2023-05-18 18:39:20.000000 aip-site-generator-0.6.4/aip_site/support/scss/imports/syntax.scss
+-rw-r--r--   0 root         (0) root         (0)      102 2023-05-18 18:39:20.000000 aip-site-generator-0.6.4/aip_site/support/scss/imports/tables.scss
+-rw-r--r--   0 root         (0) root         (0)      889 2023-05-18 18:39:20.000000 aip-site-generator-0.6.4/aip_site/support/scss/imports/tabs.scss
+-rw-r--r--   0 root         (0) root         (0)     1053 2023-05-18 18:39:20.000000 aip-site-generator-0.6.4/aip_site/support/scss/print.scss
+-rw-r--r--   0 root         (0) root         (0)     1429 2023-05-18 18:39:20.000000 aip-site-generator-0.6.4/aip_site/support/scss/search.scss
+-rw-r--r--   0 root         (0) root         (0)      466 2023-05-18 18:39:20.000000 aip-site-generator-0.6.4/aip_site/support/scss/style.scss
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 18:39:29.424228 aip-site-generator-0.6.4/aip_site/support/templates/
+-rw-r--r--   0 root         (0) root         (0)     1865 2023-05-18 18:39:20.000000 aip-site-generator-0.6.4/aip_site/support/templates/aip-listing.html.j2
+-rw-r--r--   0 root         (0) root         (0)     2178 2023-05-18 18:39:20.000000 aip-site-generator-0.6.4/aip_site/support/templates/aip.html.j2
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 18:39:29.424228 aip-site-generator-0.6.4/aip_site/support/templates/includes/
+-rw-r--r--   0 root         (0) root         (0)     1053 2023-05-18 18:39:20.000000 aip-site-generator-0.6.4/aip_site/support/templates/includes/breadcrumb.html.j2
+-rw-r--r--   0 root         (0) root         (0)      415 2023-05-18 18:39:20.000000 aip-site-generator-0.6.4/aip_site/support/templates/includes/footer.html.j2
+-rw-r--r--   0 root         (0) root         (0)     5106 2023-05-18 18:39:20.000000 aip-site-generator-0.6.4/aip_site/support/templates/includes/header.html.j2
+-rw-r--r--   0 root         (0) root         (0)      986 2023-05-18 18:39:20.000000 aip-site-generator-0.6.4/aip_site/support/templates/includes/nav.html.j2
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 18:39:29.424228 aip-site-generator-0.6.4/aip_site/support/templates/includes/state_banners/
+-rw-r--r--   0 root         (0) root         (0)      189 2023-05-18 18:39:20.000000 aip-site-generator-0.6.4/aip_site/support/templates/includes/state_banners/draft.html.j2
+-rw-r--r--   0 root         (0) root         (0)      125 2023-05-18 18:39:20.000000 aip-site-generator-0.6.4/aip_site/support/templates/includes/state_banners/rejected.html.j2
+-rw-r--r--   0 root         (0) root         (0)      212 2023-05-18 18:39:20.000000 aip-site-generator-0.6.4/aip_site/support/templates/includes/state_banners/replaced.html.j2
+-rw-r--r--   0 root         (0) root         (0)      316 2023-05-18 18:39:20.000000 aip-site-generator-0.6.4/aip_site/support/templates/includes/state_banners/reviewing.html.j2
+-rw-r--r--   0 root         (0) root         (0)      126 2023-05-18 18:39:20.000000 aip-site-generator-0.6.4/aip_site/support/templates/includes/state_banners/withdrawn.html.j2
+-rw-r--r--   0 root         (0) root         (0)     1630 2023-05-18 18:39:20.000000 aip-site-generator-0.6.4/aip_site/support/templates/index.html.j2
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 18:39:29.424228 aip-site-generator-0.6.4/aip_site/support/templates/layouts/
+-rw-r--r--   0 root         (0) root         (0)     2696 2023-05-18 18:39:20.000000 aip-site-generator-0.6.4/aip_site/support/templates/layouts/base.html.j2
+-rw-r--r--   0 root         (0) root         (0)     1033 2023-05-18 18:39:20.000000 aip-site-generator-0.6.4/aip_site/support/templates/page.html.j2
+-rw-r--r--   0 root         (0) root         (0)      544 2023-05-18 18:39:20.000000 aip-site-generator-0.6.4/aip_site/support/templates/redirect.html.j2
+-rw-r--r--   0 root         (0) root         (0)     1508 2023-05-18 18:39:20.000000 aip-site-generator-0.6.4/aip_site/support/templates/search.html.j2
+-rw-r--r--   0 root         (0) root         (0)      443 2023-05-18 18:39:20.000000 aip-site-generator-0.6.4/aip_site/support/templates/search.js.j2
+-rw-r--r--   0 root         (0) root         (0)     1229 2023-05-18 18:39:20.000000 aip-site-generator-0.6.4/aip_site/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 18:39:29.424228 aip-site-generator-0.6.4/aip_site_generator.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     6051 2023-05-18 18:39:29.000000 aip-site-generator-0.6.4/aip_site_generator.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3071 2023-05-18 18:39:29.000000 aip-site-generator-0.6.4/aip_site_generator.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-18 18:39:29.000000 aip-site-generator-0.6.4/aip_site_generator.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       90 2023-05-18 18:39:29.000000 aip-site-generator-0.6.4/aip_site_generator.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-18 18:39:29.000000 aip-site-generator-0.6.4/aip_site_generator.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      234 2023-05-18 18:39:29.000000 aip-site-generator-0.6.4/aip_site_generator.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2023-05-18 18:39:29.000000 aip-site-generator-0.6.4/aip_site_generator.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-18 18:39:29.424228 aip-site-generator-0.6.4/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2395 2023-05-18 18:39:20.000000 aip-site-generator-0.6.4/setup.py
```

### Comparing `aip-site-generator-0.6.3/LICENSE` & `aip-site-generator-0.6.4/LICENSE`

 * *Files identical despite different names*

### Comparing `aip-site-generator-0.6.3/PKG-INFO` & `aip-site-generator-0.6.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aip-site-generator
-Version: 0.6.3
+Version: 0.6.4
 Summary: Static site generator for aip.dev and forks.
 Home-page: https://github.com/aip-dev/site-generator.git
 Author: Luke Sneeringer
 Author-email: lukesneeringer@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X
 Classifier: Development Status :: 4 - Beta
```

### Comparing `aip-site-generator-0.6.3/README.md` & `aip-site-generator-0.6.4/README.md`

 * *Files identical despite different names*

### Comparing `aip-site-generator-0.6.3/aip_site/cli.py` & `aip-site-generator-0.6.4/aip_site/cli.py`

 * *Files identical despite different names*

### Comparing `aip-site-generator-0.6.3/aip_site/jinja/env.py` & `aip-site-generator-0.6.4/aip_site/jinja/env.py`

 * *Files identical despite different names*

### Comparing `aip-site-generator-0.6.3/aip_site/jinja/ext/sample.py` & `aip-site-generator-0.6.4/aip_site/jinja/ext/sample.py`

 * *Files identical despite different names*

### Comparing `aip-site-generator-0.6.3/aip_site/jinja/ext/tab.py` & `aip-site-generator-0.6.4/aip_site/jinja/ext/tab.py`

 * *Files identical despite different names*

### Comparing `aip-site-generator-0.6.3/aip_site/jinja/loaders.py` & `aip-site-generator-0.6.4/aip_site/jinja/loaders.py`

 * *Files identical despite different names*

### Comparing `aip-site-generator-0.6.3/aip_site/md.py` & `aip-site-generator-0.6.4/aip_site/md.py`

 * *Files identical despite different names*

### Comparing `aip-site-generator-0.6.3/aip_site/models/aip.py` & `aip-site-generator-0.6.4/aip_site/models/aip.py`

 * *Files identical despite different names*

### Comparing `aip-site-generator-0.6.3/aip_site/models/page.py` & `aip-site-generator-0.6.4/aip_site/models/page.py`

 * *Files identical despite different names*

### Comparing `aip-site-generator-0.6.3/aip_site/models/scope.py` & `aip-site-generator-0.6.4/aip_site/models/scope.py`

 * *Files identical despite different names*

### Comparing `aip-site-generator-0.6.3/aip_site/models/site.py` & `aip-site-generator-0.6.4/aip_site/models/site.py`

 * *Files identical despite different names*

### Comparing `aip-site-generator-0.6.3/aip_site/publisher.py` & `aip-site-generator-0.6.4/aip_site/publisher.py`

 * *Files identical despite different names*

### Comparing `aip-site-generator-0.6.3/aip_site/server.py` & `aip-site-generator-0.6.4/aip_site/server.py`

 * *Files identical despite different names*

### Comparing `aip-site-generator-0.6.3/aip_site/support/assets/favicon.ico` & `aip-site-generator-0.6.4/aip_site/support/assets/favicon.ico`

 * *Files identical despite different names*

### Comparing `aip-site-generator-0.6.3/aip_site/support/assets/images/github.png` & `aip-site-generator-0.6.4/aip_site/support/assets/images/github.png`

 * *Files identical despite different names*

### Comparing `aip-site-generator-0.6.3/aip_site/support/assets/images/glue-icons.svg` & `aip-site-generator-0.6.4/aip_site/support/assets/images/glue-icons.svg`

 * *Files identical despite different names*

### Comparing `aip-site-generator-0.6.3/aip_site/support/assets/js/aip/aip-graphviz.js` & `aip-site-generator-0.6.4/aip_site/support/assets/js/aip/aip-graphviz.js`

 * *Files identical despite different names*

### Comparing `aip-site-generator-0.6.3/aip_site/support/assets/js/aip/aip-index.js` & `aip-site-generator-0.6.4/aip_site/support/assets/js/aip/aip-index.js`

 * *Files identical despite different names*

### Comparing `aip-site-generator-0.6.3/aip_site/support/assets/js/global.js` & `aip-site-generator-0.6.4/aip_site/support/assets/js/global.js`

 * *Files identical despite different names*

### Comparing `aip-site-generator-0.6.3/aip_site/support/assets/js/graphviz/lite.render.js` & `aip-site-generator-0.6.4/aip_site/support/assets/js/graphviz/lite.render.js`

 * *Files identical despite different names*

### Comparing `aip-site-generator-0.6.3/aip_site/support/assets/js/graphviz/viz.js` & `aip-site-generator-0.6.4/aip_site/support/assets/js/graphviz/viz.js`

 * *Files identical despite different names*

### Comparing `aip-site-generator-0.6.3/aip_site/support/assets/js/search/pagination.js` & `aip-site-generator-0.6.4/aip_site/support/assets/js/search/pagination.js`

 * *Files identical despite different names*

### Comparing `aip-site-generator-0.6.3/aip_site/support/assets/js/search/tipuesearch.min.js` & `aip-site-generator-0.6.4/aip_site/support/assets/js/search/tipuesearch.min.js`

 * *Files identical despite different names*

### Comparing `aip-site-generator-0.6.3/aip_site/support/assets/js/search/tipuesearch_set.js` & `aip-site-generator-0.6.4/aip_site/support/assets/js/search/tipuesearch_set.js`

 * *Files identical despite different names*

### Comparing `aip-site-generator-0.6.3/aip_site/support/assets/js/syntax.js` & `aip-site-generator-0.6.4/aip_site/support/assets/js/syntax.js`

 * *Files identical despite different names*

### Comparing `aip-site-generator-0.6.3/aip_site/support/assets/misc/ebnf-filtering.txt` & `aip-site-generator-0.6.4/aip_site/support/assets/misc/ebnf-filtering.txt`

 * *Files identical despite different names*

### Comparing `aip-site-generator-0.6.3/aip_site/support/scss/hero.scss` & `aip-site-generator-0.6.4/aip_site/support/scss/hero.scss`

 * *Files identical despite different names*

### Comparing `aip-site-generator-0.6.3/aip_site/support/scss/imports/aip/news.scss` & `aip-site-generator-0.6.4/aip_site/support/scss/imports/aip/news.scss`

 * *Files identical despite different names*

### Comparing `aip-site-generator-0.6.3/aip_site/support/scss/imports/aip/tables.scss` & `aip-site-generator-0.6.4/aip_site/support/scss/imports/aip/tables.scss`

 * *Files identical despite different names*

### Comparing `aip-site-generator-0.6.3/aip_site/support/scss/imports/callouts.scss` & `aip-site-generator-0.6.4/aip_site/support/scss/imports/callouts.scss`

 * *Files identical despite different names*

### Comparing `aip-site-generator-0.6.3/aip_site/support/scss/imports/colors.scss` & `aip-site-generator-0.6.4/aip_site/support/scss/imports/colors.scss`

 * *Files identical despite different names*

### Comparing `aip-site-generator-0.6.3/aip_site/support/scss/imports/header.scss` & `aip-site-generator-0.6.4/aip_site/support/scss/imports/header.scss`

 * *Files identical despite different names*

### Comparing `aip-site-generator-0.6.3/aip_site/support/scss/imports/headings.scss` & `aip-site-generator-0.6.4/aip_site/support/scss/imports/headings.scss`

 * *Files identical despite different names*

### Comparing `aip-site-generator-0.6.3/aip_site/support/scss/imports/nav.scss` & `aip-site-generator-0.6.4/aip_site/support/scss/imports/nav.scss`

 * *Files identical despite different names*

### Comparing `aip-site-generator-0.6.3/aip_site/support/scss/imports/sidebar.scss` & `aip-site-generator-0.6.4/aip_site/support/scss/imports/sidebar.scss`

 * *Files identical despite different names*

### Comparing `aip-site-generator-0.6.3/aip_site/support/scss/imports/syntax.scss` & `aip-site-generator-0.6.4/aip_site/support/scss/imports/syntax.scss`

 * *Files identical despite different names*

### Comparing `aip-site-generator-0.6.3/aip_site/support/scss/imports/tabs.scss` & `aip-site-generator-0.6.4/aip_site/support/scss/imports/tabs.scss`

 * *Files identical despite different names*

### Comparing `aip-site-generator-0.6.3/aip_site/support/scss/print.scss` & `aip-site-generator-0.6.4/aip_site/support/scss/print.scss`

 * *Files identical despite different names*

### Comparing `aip-site-generator-0.6.3/aip_site/support/scss/search.scss` & `aip-site-generator-0.6.4/aip_site/support/scss/search.scss`

 * *Files identical despite different names*

### Comparing `aip-site-generator-0.6.3/aip_site/support/templates/aip-listing.html.j2` & `aip-site-generator-0.6.4/aip_site/support/templates/aip-listing.html.j2`

 * *Files identical despite different names*

### Comparing `aip-site-generator-0.6.3/aip_site/support/templates/aip.html.j2` & `aip-site-generator-0.6.4/aip_site/support/templates/aip.html.j2`

 * *Files identical despite different names*

### Comparing `aip-site-generator-0.6.3/aip_site/support/templates/includes/breadcrumb.html.j2` & `aip-site-generator-0.6.4/aip_site/support/templates/includes/breadcrumb.html.j2`

 * *Files identical despite different names*

### Comparing `aip-site-generator-0.6.3/aip_site/support/templates/includes/header.html.j2` & `aip-site-generator-0.6.4/aip_site/support/templates/includes/header.html.j2`

 * *Files identical despite different names*

### Comparing `aip-site-generator-0.6.3/aip_site/support/templates/includes/nav.html.j2` & `aip-site-generator-0.6.4/aip_site/support/templates/includes/nav.html.j2`

 * *Files identical despite different names*

### Comparing `aip-site-generator-0.6.3/aip_site/support/templates/index.html.j2` & `aip-site-generator-0.6.4/aip_site/support/templates/index.html.j2`

 * *Files identical despite different names*

### Comparing `aip-site-generator-0.6.3/aip_site/support/templates/layouts/base.html.j2` & `aip-site-generator-0.6.4/aip_site/support/templates/layouts/base.html.j2`

 * *Files identical despite different names*

### Comparing `aip-site-generator-0.6.3/aip_site/support/templates/page.html.j2` & `aip-site-generator-0.6.4/aip_site/support/templates/page.html.j2`

 * *Files identical despite different names*

### Comparing `aip-site-generator-0.6.3/aip_site/support/templates/redirect.html.j2` & `aip-site-generator-0.6.4/aip_site/support/templates/redirect.html.j2`

 * *Files identical despite different names*

### Comparing `aip-site-generator-0.6.3/aip_site/support/templates/search.html.j2` & `aip-site-generator-0.6.4/aip_site/support/templates/search.html.j2`

 * *Files identical despite different names*

### Comparing `aip-site-generator-0.6.3/aip_site/utils.py` & `aip-site-generator-0.6.4/aip_site/utils.py`

 * *Files identical despite different names*

### Comparing `aip-site-generator-0.6.3/aip_site_generator.egg-info/PKG-INFO` & `aip-site-generator-0.6.4/aip_site_generator.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aip-site-generator
-Version: 0.6.3
+Version: 0.6.4
 Summary: Static site generator for aip.dev and forks.
 Home-page: https://github.com/aip-dev/site-generator.git
 Author: Luke Sneeringer
 Author-email: lukesneeringer@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X
 Classifier: Development Status :: 4 - Beta
```

### Comparing `aip-site-generator-0.6.3/aip_site_generator.egg-info/SOURCES.txt` & `aip-site-generator-0.6.4/aip_site_generator.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aip-site-generator-0.6.3/setup.py` & `aip-site-generator-0.6.4/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 # Copyright 2020 Google LLC
 #
-# Licensed under the Apache License, Version 2.0 (the 'License');
+# Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     https://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an 'AS IS' BASIS,
+# distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import io
 import os
 
@@ -33,32 +33,30 @@
     author='Luke Sneeringer',
     author_email='lukesneeringer@google.com',
     url='https://github.com/aip-dev/site-generator.git',
     packages=find_packages(exclude=['tests']),
     description='Static site generator for aip.dev and forks.',
     long_description=long_description,
     long_description_content_type='text/markdown',
-    entry_points='''[console_scripts]
+    entry_points="""[console_scripts]
         aip-site-gen=aip_site.cli:publish
         aip-site-serve=aip_site.cli:serve
-    ''',
+    """,
     platforms='Posix; MacOS X',
     include_package_data=True,
     install_requires=(
         'click==8.1.3',
         'flask==2.2.2',
         'itsdangerous==2.1.2',
         'jinja2==3.1.2',
         'markdown==3.4.1',
         'markupsafe==2.1.1',
         'pygments==2.13.0',
         'pymdown-extensions==9.7',
-        # pinning via GitHub release until https://github.com/Kronuz/pyScss/pull/426
-        # is released on PyPi.
-        'pyscss @ git+https://github.com/Kronuz/pyScss.git@73559d047706ccd4593cf6aa092de71f35164723',
+        'pyscss==1.4.0',
         'pyyaml==6.0',
         'six==1.16.0',
         'types-Markdown==3.4.2.1',
         'types-PyYAML==6.0.12',
         'werkzeug==2.2.2',
     ),
     python_requires='>=3.8',
```

