# Comparing `tmp/enthought_sphinx_theme-0.7.2.tar.gz` & `tmp/enthought_sphinx_theme-0.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "enthought_sphinx_theme-0.7.2.tar", last modified: Wed Aug 10 13:03:13 2022, max compression
+gzip compressed data, was "enthought_sphinx_theme-0.7.3.tar", last modified: Thu May 18 15:56:36 2023, max compression
```

## Comparing `enthought_sphinx_theme-0.7.2.tar` & `enthought_sphinx_theme-0.7.3.tar`

### file list

```diff
@@ -1,98 +1,98 @@
-drwxr-xr-x   0 mdickinson   (501) staff       (20)        0 2022-08-10 13:03:13.017704 enthought_sphinx_theme-0.7.2/
--rw-r--r--   0 mdickinson   (501) staff       (20)     1589 2022-08-10 10:23:28.000000 enthought_sphinx_theme-0.7.2/LICENSE
--rw-r--r--   0 mdickinson   (501) staff       (20)      217 2022-08-10 10:23:28.000000 enthought_sphinx_theme-0.7.2/MANIFEST.in
--rw-r--r--   0 mdickinson   (501) staff       (20)      194 2022-08-10 10:23:28.000000 enthought_sphinx_theme-0.7.2/Makefile
--rw-r--r--   0 mdickinson   (501) staff       (20)     2309 2022-08-10 13:03:13.017374 enthought_sphinx_theme-0.7.2/PKG-INFO
--rw-r--r--   0 mdickinson   (501) staff       (20)     1726 2022-08-10 10:23:28.000000 enthought_sphinx_theme-0.7.2/README.rst
-drwxr-xr-x   0 mdickinson   (501) staff       (20)        0 2022-08-10 13:03:12.830186 enthought_sphinx_theme-0.7.2/enthought_sphinx_theme/
--rw-r--r--   0 mdickinson   (501) staff       (20)       98 2022-08-10 10:23:28.000000 enthought_sphinx_theme-0.7.2/enthought_sphinx_theme/__init__.py
-drwxr-xr-x   0 mdickinson   (501) staff       (20)        0 2022-08-10 13:03:12.869176 enthought_sphinx_theme-0.7.2/enthought_sphinx_theme/enthought/
--rw-r--r--   0 mdickinson   (501) staff       (20)     8954 2022-08-10 10:23:28.000000 enthought_sphinx_theme-0.7.2/enthought_sphinx_theme/enthought/layout.html
--rw-r--r--   0 mdickinson   (501) staff       (20)      224 2022-08-10 10:23:28.000000 enthought_sphinx_theme-0.7.2/enthought_sphinx_theme/enthought/sourcelink.html
-drwxr-xr-x   0 mdickinson   (501) staff       (20)        0 2022-08-10 13:03:12.870387 enthought_sphinx_theme-0.7.2/enthought_sphinx_theme/enthought/static/
-drwxr-xr-x   0 mdickinson   (501) staff       (20)        0 2022-08-10 13:03:12.875098 enthought_sphinx_theme-0.7.2/enthought_sphinx_theme/enthought/static/css/
--rw-r--r--   0 mdickinson   (501) staff       (20)     3916 2022-08-10 10:23:28.000000 enthought_sphinx_theme-0.7.2/enthought_sphinx_theme/enthought/static/css/pygments.css
--rw-r--r--   0 mdickinson   (501) staff       (20)   145710 2022-08-10 10:23:28.000000 enthought_sphinx_theme-0.7.2/enthought_sphinx_theme/enthought/static/css/spc-bootstrap.css
--rw-r--r--   0 mdickinson   (501) staff       (20)     1659 2022-08-10 10:23:28.000000 enthought_sphinx_theme-0.7.2/enthought_sphinx_theme/enthought/static/css/spc-extend.css
--rw-r--r--   0 mdickinson   (501) staff       (20)     8010 2022-08-10 10:23:28.000000 enthought_sphinx_theme-0.7.2/enthought_sphinx_theme/enthought/static/enthought.css_t
-drwxr-xr-x   0 mdickinson   (501) staff       (20)        0 2022-08-10 13:03:12.885291 enthought_sphinx_theme-0.7.2/enthought_sphinx_theme/enthought/static/fonts/
--rw-r--r--   0 mdickinson   (501) staff       (20)    57712 2022-08-10 10:23:28.000000 enthought_sphinx_theme-0.7.2/enthought_sphinx_theme/enthought/static/fonts/SourceCodePro-Regular.otf.woff
--rw-r--r--   0 mdickinson   (501) staff       (20)    57200 2022-08-10 10:23:28.000000 enthought_sphinx_theme-0.7.2/enthought_sphinx_theme/enthought/static/fonts/SourceCodePro-Semibold.otf.woff
--rw-r--r--   0 mdickinson   (501) staff       (20)     8000 2022-08-10 10:23:28.000000 enthought_sphinx_theme-0.7.2/enthought_sphinx_theme/enthought/static/fonts/poppins-v19-latin-600.woff2
--rw-r--r--   0 mdickinson   (501) staff       (20)     8724 2022-08-10 10:23:28.000000 enthought_sphinx_theme-0.7.2/enthought_sphinx_theme/enthought/static/fonts/poppins-v19-latin-600italic.woff2
--rw-r--r--   0 mdickinson   (501) staff       (20)     8668 2022-08-10 10:23:28.000000 enthought_sphinx_theme-0.7.2/enthought_sphinx_theme/enthought/static/fonts/poppins-v19-latin-italic.woff2
--rw-r--r--   0 mdickinson   (501) staff       (20)     7884 2022-08-10 10:23:28.000000 enthought_sphinx_theme-0.7.2/enthought_sphinx_theme/enthought/static/fonts/poppins-v19-latin-regular.woff2
-drwxr-xr-x   0 mdickinson   (501) staff       (20)        0 2022-08-10 13:03:12.895847 enthought_sphinx_theme-0.7.2/enthought_sphinx_theme/enthought/static/img/
--rw-r--r--   0 mdickinson   (501) staff       (20)      202 2022-08-10 10:23:28.000000 enthought_sphinx_theme-0.7.2/enthought_sphinx_theme/enthought/static/img/contents.png
--rw-r--r--   0 mdickinson   (501) staff       (20)     8325 2022-08-10 10:23:28.000000 enthought_sphinx_theme-0.7.2/enthought_sphinx_theme/enthought/static/img/e-logo.png
--rw-r--r--   0 mdickinson   (501) staff       (20)      696 2022-08-10 10:23:28.000000 enthought_sphinx_theme-0.7.2/enthought_sphinx_theme/enthought/static/img/favicon.png
--rw-r--r--   0 mdickinson   (501) staff       (20)     8777 2022-08-10 10:23:28.000000 enthought_sphinx_theme-0.7.2/enthought_sphinx_theme/enthought/static/img/glyphicons-halflings-white.png
--rw-r--r--   0 mdickinson   (501) staff       (20)    12799 2022-08-10 10:23:28.000000 enthought_sphinx_theme-0.7.2/enthought_sphinx_theme/enthought/static/img/glyphicons-halflings.png
--rw-r--r--   0 mdickinson   (501) staff       (20)      218 2022-08-10 10:23:28.000000 enthought_sphinx_theme-0.7.2/enthought_sphinx_theme/enthought/static/img/navigation.png
--rw-r--r--   0 mdickinson   (501) staff       (20)       43 2022-08-10 10:23:28.000000 enthought_sphinx_theme-0.7.2/enthought_sphinx_theme/enthought/static/img/transparent-pixel.gif
--rw-r--r--   0 mdickinson   (501) staff       (20)     1459 2022-08-10 10:23:28.000000 enthought_sphinx_theme-0.7.2/enthought_sphinx_theme/enthought/static/img/ui-anim_basic_16x16.gif
-drwxr-xr-x   0 mdickinson   (501) staff       (20)        0 2022-08-10 13:03:12.898168 enthought_sphinx_theme-0.7.2/enthought_sphinx_theme/enthought/static/js/
--rw-r--r--   0 mdickinson   (501) staff       (20)     2676 2022-08-10 10:23:28.000000 enthought_sphinx_theme-0.7.2/enthought_sphinx_theme/enthought/static/js/copybutton.js
--rw-r--r--   0 mdickinson   (501) staff       (20)      202 2022-08-10 10:23:28.000000 enthought_sphinx_theme-0.7.2/enthought_sphinx_theme/enthought/static/js/wrap_on_dot.js
--rw-r--r--   0 mdickinson   (501) staff       (20)      191 2022-08-10 10:23:28.000000 enthought_sphinx_theme-0.7.2/enthought_sphinx_theme/enthought/theme.conf
-drwxr-xr-x   0 mdickinson   (501) staff       (20)        0 2022-08-10 13:03:12.863788 enthought_sphinx_theme-0.7.2/enthought_sphinx_theme.egg-info/
--rw-r--r--   0 mdickinson   (501) staff       (20)     2309 2022-08-10 13:03:12.000000 enthought_sphinx_theme-0.7.2/enthought_sphinx_theme.egg-info/PKG-INFO
--rw-r--r--   0 mdickinson   (501) staff       (20)     3199 2022-08-10 13:03:12.000000 enthought_sphinx_theme-0.7.2/enthought_sphinx_theme.egg-info/SOURCES.txt
--rw-r--r--   0 mdickinson   (501) staff       (20)        1 2022-08-10 13:03:12.000000 enthought_sphinx_theme-0.7.2/enthought_sphinx_theme.egg-info/dependency_links.txt
--rw-r--r--   0 mdickinson   (501) staff       (20)       23 2022-08-10 13:03:12.000000 enthought_sphinx_theme-0.7.2/enthought_sphinx_theme.egg-info/top_level.txt
-drwxr-xr-x   0 mdickinson   (501) staff       (20)        0 2022-08-10 13:03:12.906981 enthought_sphinx_theme-0.7.2/less/
-drwxr-xr-x   0 mdickinson   (501) staff       (20)        0 2022-08-10 13:03:13.013327 enthought_sphinx_theme-0.7.2/less/bootstrap/
--rw-r--r--   0 mdickinson   (501) staff       (20)      636 2022-08-10 10:23:28.000000 enthought_sphinx_theme-0.7.2/less/bootstrap/accordion.less
--rw-r--r--   0 mdickinson   (501) staff       (20)     1369 2022-08-10 10:23:28.000000 enthought_sphinx_theme-0.7.2/less/bootstrap/alerts.less
--rw-r--r--   0 mdickinson   (501) staff       (20)     1489 2022-08-10 10:23:28.000000 enthought_sphinx_theme-0.7.2/less/bootstrap/bootstrap.less
--rw-r--r--   0 mdickinson   (501) staff       (20)      431 2022-08-10 10:23:28.000000 enthought_sphinx_theme-0.7.2/less/bootstrap/breadcrumbs.less
--rw-r--r--   0 mdickinson   (501) staff       (20)     5709 2022-08-10 10:23:28.000000 enthought_sphinx_theme-0.7.2/less/bootstrap/button-groups.less
--rw-r--r--   0 mdickinson   (501) staff       (20)     4766 2022-08-10 10:23:28.000000 enthought_sphinx_theme-0.7.2/less/bootstrap/buttons.less
--rw-r--r--   0 mdickinson   (501) staff       (20)     2482 2022-08-10 10:23:28.000000 enthought_sphinx_theme-0.7.2/less/bootstrap/carousel.less
--rw-r--r--   0 mdickinson   (501) staff       (20)      644 2022-08-10 10:23:28.000000 enthought_sphinx_theme-0.7.2/less/bootstrap/close.less
--rw-r--r--   0 mdickinson   (501) staff       (20)     1282 2022-08-10 10:23:28.000000 enthought_sphinx_theme-0.7.2/less/bootstrap/code.less
--rw-r--r--   0 mdickinson   (501) staff       (20)      306 2022-08-10 10:23:28.000000 enthought_sphinx_theme-0.7.2/less/bootstrap/component-animations.less
--rw-r--r--   0 mdickinson   (501) staff       (20)     5493 2022-08-10 10:23:28.000000 enthought_sphinx_theme-0.7.2/less/bootstrap/dropdowns.less
--rw-r--r--   0 mdickinson   (501) staff       (20)    15866 2022-08-10 10:23:28.000000 enthought_sphinx_theme-0.7.2/less/bootstrap/forms.less
--rw-r--r--   0 mdickinson   (501) staff       (20)      429 2022-08-10 10:23:28.000000 enthought_sphinx_theme-0.7.2/less/bootstrap/grid.less
--rw-r--r--   0 mdickinson   (501) staff       (20)      521 2022-08-10 10:23:28.000000 enthought_sphinx_theme-0.7.2/less/bootstrap/hero-unit.less
--rw-r--r--   0 mdickinson   (501) staff       (20)     1884 2022-08-10 10:23:28.000000 enthought_sphinx_theme-0.7.2/less/bootstrap/labels-badges.less
--rw-r--r--   0 mdickinson   (501) staff       (20)      329 2022-08-10 10:23:28.000000 enthought_sphinx_theme-0.7.2/less/bootstrap/layouts.less
--rw-r--r--   0 mdickinson   (501) staff       (20)      860 2022-08-10 10:23:28.000000 enthought_sphinx_theme-0.7.2/less/bootstrap/media.less
--rw-r--r--   0 mdickinson   (501) staff       (20)    23042 2022-08-10 10:23:28.000000 enthought_sphinx_theme-0.7.2/less/bootstrap/mixins.less
--rw-r--r--   0 mdickinson   (501) staff       (20)     1978 2022-08-10 10:23:28.000000 enthought_sphinx_theme-0.7.2/less/bootstrap/modals.less
--rw-r--r--   0 mdickinson   (501) staff       (20)    12002 2022-08-10 10:23:28.000000 enthought_sphinx_theme-0.7.2/less/bootstrap/navbar.less
--rw-r--r--   0 mdickinson   (501) staff       (20)     8163 2022-08-10 10:23:28.000000 enthought_sphinx_theme-0.7.2/less/bootstrap/navs.less
--rw-r--r--   0 mdickinson   (501) staff       (20)      760 2022-08-10 10:23:28.000000 enthought_sphinx_theme-0.7.2/less/bootstrap/pager.less
--rw-r--r--   0 mdickinson   (501) staff       (20)     2678 2022-08-10 10:23:28.000000 enthought_sphinx_theme-0.7.2/less/bootstrap/pagination.less
--rw-r--r--   0 mdickinson   (501) staff       (20)     3077 2022-08-10 10:23:28.000000 enthought_sphinx_theme-0.7.2/less/bootstrap/popovers.less
--rw-r--r--   0 mdickinson   (501) staff       (20)     2858 2022-08-10 10:23:28.000000 enthought_sphinx_theme-0.7.2/less/bootstrap/progress-bars.less
--rw-r--r--   0 mdickinson   (501) staff       (20)     4201 2022-08-10 10:23:28.000000 enthought_sphinx_theme-0.7.2/less/bootstrap/reset.less
--rw-r--r--   0 mdickinson   (501) staff       (20)      565 2022-08-10 10:23:28.000000 enthought_sphinx_theme-0.7.2/less/bootstrap/responsive-1200px-min.less
--rw-r--r--   0 mdickinson   (501) staff       (20)     3920 2022-08-10 10:23:28.000000 enthought_sphinx_theme-0.7.2/less/bootstrap/responsive-767px-max.less
--rw-r--r--   0 mdickinson   (501) staff       (20)      463 2022-08-10 10:23:28.000000 enthought_sphinx_theme-0.7.2/less/bootstrap/responsive-768px-979px.less
--rw-r--r--   0 mdickinson   (501) staff       (20)     4328 2022-08-10 10:23:28.000000 enthought_sphinx_theme-0.7.2/less/bootstrap/responsive-navbar.less
--rw-r--r--   0 mdickinson   (501) staff       (20)     1602 2022-08-10 10:23:28.000000 enthought_sphinx_theme-0.7.2/less/bootstrap/responsive-utilities.less
--rw-r--r--   0 mdickinson   (501) staff       (20)     1069 2022-08-10 10:23:28.000000 enthought_sphinx_theme-0.7.2/less/bootstrap/responsive.less
--rw-r--r--   0 mdickinson   (501) staff       (20)      885 2022-08-10 10:23:28.000000 enthought_sphinx_theme-0.7.2/less/bootstrap/scaffolding.less
--rw-r--r--   0 mdickinson   (501) staff       (20)    10841 2022-08-10 10:23:28.000000 enthought_sphinx_theme-0.7.2/less/bootstrap/sprites.less
--rw-r--r--   0 mdickinson   (501) staff       (20)     6255 2022-08-10 10:23:28.000000 enthought_sphinx_theme-0.7.2/less/bootstrap/tables.less
--rw-r--r--   0 mdickinson   (501) staff       (20)     1192 2022-08-10 10:23:28.000000 enthought_sphinx_theme-0.7.2/less/bootstrap/thumbnails.less
--rw-r--r--   0 mdickinson   (501) staff       (20)     1684 2022-08-10 10:23:28.000000 enthought_sphinx_theme-0.7.2/less/bootstrap/tooltip.less
--rw-r--r--   0 mdickinson   (501) staff       (20)     4857 2022-08-10 10:23:28.000000 enthought_sphinx_theme-0.7.2/less/bootstrap/type.less
--rw-r--r--   0 mdickinson   (501) staff       (20)      335 2022-08-10 10:23:28.000000 enthought_sphinx_theme-0.7.2/less/bootstrap/utilities.less
--rw-r--r--   0 mdickinson   (501) staff       (20)     9142 2022-08-10 10:23:28.000000 enthought_sphinx_theme-0.7.2/less/bootstrap/variables.less
--rw-r--r--   0 mdickinson   (501) staff       (20)      552 2022-08-10 10:23:28.000000 enthought_sphinx_theme-0.7.2/less/bootstrap/wells.less
--rw-r--r--   0 mdickinson   (501) staff       (20)      445 2022-08-10 10:23:28.000000 enthought_sphinx_theme-0.7.2/less/spc-bootstrap.less
--rw-r--r--   0 mdickinson   (501) staff       (20)      832 2022-08-10 10:23:28.000000 enthought_sphinx_theme-0.7.2/less/spc-content.less
--rw-r--r--   0 mdickinson   (501) staff       (20)      205 2022-08-10 10:23:28.000000 enthought_sphinx_theme-0.7.2/less/spc-extend.less
--rw-r--r--   0 mdickinson   (501) staff       (20)      154 2022-08-10 10:23:28.000000 enthought_sphinx_theme-0.7.2/less/spc-footer.less
--rw-r--r--   0 mdickinson   (501) staff       (20)      441 2022-08-10 10:23:28.000000 enthought_sphinx_theme-0.7.2/less/spc-header.less
--rw-r--r--   0 mdickinson   (501) staff       (20)      259 2022-08-10 10:23:28.000000 enthought_sphinx_theme-0.7.2/less/spc-rightsidebar.less
--rw-r--r--   0 mdickinson   (501) staff       (20)      425 2022-08-10 10:23:28.000000 enthought_sphinx_theme-0.7.2/less/spc-utils.less
-drwxr-xr-x   0 mdickinson   (501) staff       (20)        0 2022-08-10 13:03:13.016805 enthought_sphinx_theme-0.7.2/licenses/
--rw-r--r--   0 mdickinson   (501) staff       (20)     1179 2022-08-10 10:23:28.000000 enthought_sphinx_theme-0.7.2/licenses/bootstrap.txt
--rw-r--r--   0 mdickinson   (501) staff       (20)     5065 2022-08-10 10:23:28.000000 enthought_sphinx_theme-0.7.2/licenses/fonts.txt
--rw-r--r--   0 mdickinson   (501) staff       (20)     1791 2022-08-10 10:23:28.000000 enthought_sphinx_theme-0.7.2/licenses/scipy-sphinx-theme.txt
--rw-r--r--   0 mdickinson   (501) staff       (20)       38 2022-08-10 13:03:13.017795 enthought_sphinx_theme-0.7.2/setup.cfg
--rw-r--r--   0 mdickinson   (501) staff       (20)      891 2022-08-10 12:58:34.000000 enthought_sphinx_theme-0.7.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:56:36.529856 enthought_sphinx_theme-0.7.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1589 2023-05-18 15:56:21.000000 enthought_sphinx_theme-0.7.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-05-18 15:56:21.000000 enthought_sphinx_theme-0.7.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-05-18 15:56:21.000000 enthought_sphinx_theme-0.7.3/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     2309 2023-05-18 15:56:36.525856 enthought_sphinx_theme-0.7.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-05-18 15:56:21.000000 enthought_sphinx_theme-0.7.3/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:56:36.505854 enthought_sphinx_theme-0.7.3/enthought_sphinx_theme/
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-18 15:56:21.000000 enthought_sphinx_theme-0.7.3/enthought_sphinx_theme/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:56:36.509855 enthought_sphinx_theme-0.7.3/enthought_sphinx_theme/enthought/
+-rw-r--r--   0 runner    (1001) docker     (123)     8958 2023-05-18 15:56:21.000000 enthought_sphinx_theme-0.7.3/enthought_sphinx_theme/enthought/layout.html
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-05-18 15:56:21.000000 enthought_sphinx_theme-0.7.3/enthought_sphinx_theme/enthought/sourcelink.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:56:36.509855 enthought_sphinx_theme-0.7.3/enthought_sphinx_theme/enthought/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:56:36.509855 enthought_sphinx_theme-0.7.3/enthought_sphinx_theme/enthought/static/css/
+-rw-r--r--   0 runner    (1001) docker     (123)     3916 2023-05-18 15:56:21.000000 enthought_sphinx_theme-0.7.3/enthought_sphinx_theme/enthought/static/css/pygments.css
+-rw-r--r--   0 runner    (1001) docker     (123)   145710 2023-05-18 15:56:21.000000 enthought_sphinx_theme-0.7.3/enthought_sphinx_theme/enthought/static/css/spc-bootstrap.css
+-rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-05-18 15:56:21.000000 enthought_sphinx_theme-0.7.3/enthought_sphinx_theme/enthought/static/css/spc-extend.css
+-rw-r--r--   0 runner    (1001) docker     (123)     8010 2023-05-18 15:56:21.000000 enthought_sphinx_theme-0.7.3/enthought_sphinx_theme/enthought/static/enthought.css_t
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:56:36.509855 enthought_sphinx_theme-0.7.3/enthought_sphinx_theme/enthought/static/fonts/
+-rw-r--r--   0 runner    (1001) docker     (123)    57712 2023-05-18 15:56:21.000000 enthought_sphinx_theme-0.7.3/enthought_sphinx_theme/enthought/static/fonts/SourceCodePro-Regular.otf.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    57200 2023-05-18 15:56:21.000000 enthought_sphinx_theme-0.7.3/enthought_sphinx_theme/enthought/static/fonts/SourceCodePro-Semibold.otf.woff
+-rw-r--r--   0 runner    (1001) docker     (123)     8000 2023-05-18 15:56:21.000000 enthought_sphinx_theme-0.7.3/enthought_sphinx_theme/enthought/static/fonts/poppins-v19-latin-600.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)     8724 2023-05-18 15:56:21.000000 enthought_sphinx_theme-0.7.3/enthought_sphinx_theme/enthought/static/fonts/poppins-v19-latin-600italic.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)     8668 2023-05-18 15:56:21.000000 enthought_sphinx_theme-0.7.3/enthought_sphinx_theme/enthought/static/fonts/poppins-v19-latin-italic.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)     7884 2023-05-18 15:56:21.000000 enthought_sphinx_theme-0.7.3/enthought_sphinx_theme/enthought/static/fonts/poppins-v19-latin-regular.woff2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:56:36.513855 enthought_sphinx_theme-0.7.3/enthought_sphinx_theme/enthought/static/img/
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-05-18 15:56:21.000000 enthought_sphinx_theme-0.7.3/enthought_sphinx_theme/enthought/static/img/contents.png
+-rw-r--r--   0 runner    (1001) docker     (123)     8325 2023-05-18 15:56:21.000000 enthought_sphinx_theme-0.7.3/enthought_sphinx_theme/enthought/static/img/e-logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-05-18 15:56:21.000000 enthought_sphinx_theme-0.7.3/enthought_sphinx_theme/enthought/static/img/favicon.png
+-rw-r--r--   0 runner    (1001) docker     (123)     8777 2023-05-18 15:56:21.000000 enthought_sphinx_theme-0.7.3/enthought_sphinx_theme/enthought/static/img/glyphicons-halflings-white.png
+-rw-r--r--   0 runner    (1001) docker     (123)    12799 2023-05-18 15:56:21.000000 enthought_sphinx_theme-0.7.3/enthought_sphinx_theme/enthought/static/img/glyphicons-halflings.png
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-05-18 15:56:21.000000 enthought_sphinx_theme-0.7.3/enthought_sphinx_theme/enthought/static/img/navigation.png
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-18 15:56:21.000000 enthought_sphinx_theme-0.7.3/enthought_sphinx_theme/enthought/static/img/transparent-pixel.gif
+-rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-05-18 15:56:21.000000 enthought_sphinx_theme-0.7.3/enthought_sphinx_theme/enthought/static/img/ui-anim_basic_16x16.gif
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:56:36.513855 enthought_sphinx_theme-0.7.3/enthought_sphinx_theme/enthought/static/js/
+-rw-r--r--   0 runner    (1001) docker     (123)     2676 2023-05-18 15:56:21.000000 enthought_sphinx_theme-0.7.3/enthought_sphinx_theme/enthought/static/js/copybutton.js
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-05-18 15:56:21.000000 enthought_sphinx_theme-0.7.3/enthought_sphinx_theme/enthought/static/js/wrap_on_dot.js
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-05-18 15:56:21.000000 enthought_sphinx_theme-0.7.3/enthought_sphinx_theme/enthought/theme.conf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:56:36.505854 enthought_sphinx_theme-0.7.3/enthought_sphinx_theme.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2309 2023-05-18 15:56:36.000000 enthought_sphinx_theme-0.7.3/enthought_sphinx_theme.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3199 2023-05-18 15:56:36.000000 enthought_sphinx_theme-0.7.3/enthought_sphinx_theme.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 15:56:36.000000 enthought_sphinx_theme-0.7.3/enthought_sphinx_theme.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-18 15:56:36.000000 enthought_sphinx_theme-0.7.3/enthought_sphinx_theme.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:56:36.517855 enthought_sphinx_theme-0.7.3/less/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:56:36.525856 enthought_sphinx_theme-0.7.3/less/bootstrap/
+-rw-r--r--   0 runner    (1001) docker     (123)      636 2023-05-18 15:56:21.000000 enthought_sphinx_theme-0.7.3/less/bootstrap/accordion.less
+-rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-05-18 15:56:21.000000 enthought_sphinx_theme-0.7.3/less/bootstrap/alerts.less
+-rw-r--r--   0 runner    (1001) docker     (123)     1489 2023-05-18 15:56:21.000000 enthought_sphinx_theme-0.7.3/less/bootstrap/bootstrap.less
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2023-05-18 15:56:21.000000 enthought_sphinx_theme-0.7.3/less/bootstrap/breadcrumbs.less
+-rw-r--r--   0 runner    (1001) docker     (123)     5709 2023-05-18 15:56:21.000000 enthought_sphinx_theme-0.7.3/less/bootstrap/button-groups.less
+-rw-r--r--   0 runner    (1001) docker     (123)     4766 2023-05-18 15:56:21.000000 enthought_sphinx_theme-0.7.3/less/bootstrap/buttons.less
+-rw-r--r--   0 runner    (1001) docker     (123)     2482 2023-05-18 15:56:21.000000 enthought_sphinx_theme-0.7.3/less/bootstrap/carousel.less
+-rw-r--r--   0 runner    (1001) docker     (123)      644 2023-05-18 15:56:21.000000 enthought_sphinx_theme-0.7.3/less/bootstrap/close.less
+-rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-05-18 15:56:21.000000 enthought_sphinx_theme-0.7.3/less/bootstrap/code.less
+-rw-r--r--   0 runner    (1001) docker     (123)      306 2023-05-18 15:56:21.000000 enthought_sphinx_theme-0.7.3/less/bootstrap/component-animations.less
+-rw-r--r--   0 runner    (1001) docker     (123)     5493 2023-05-18 15:56:21.000000 enthought_sphinx_theme-0.7.3/less/bootstrap/dropdowns.less
+-rw-r--r--   0 runner    (1001) docker     (123)    15866 2023-05-18 15:56:21.000000 enthought_sphinx_theme-0.7.3/less/bootstrap/forms.less
+-rw-r--r--   0 runner    (1001) docker     (123)      429 2023-05-18 15:56:21.000000 enthought_sphinx_theme-0.7.3/less/bootstrap/grid.less
+-rw-r--r--   0 runner    (1001) docker     (123)      521 2023-05-18 15:56:21.000000 enthought_sphinx_theme-0.7.3/less/bootstrap/hero-unit.less
+-rw-r--r--   0 runner    (1001) docker     (123)     1884 2023-05-18 15:56:21.000000 enthought_sphinx_theme-0.7.3/less/bootstrap/labels-badges.less
+-rw-r--r--   0 runner    (1001) docker     (123)      329 2023-05-18 15:56:21.000000 enthought_sphinx_theme-0.7.3/less/bootstrap/layouts.less
+-rw-r--r--   0 runner    (1001) docker     (123)      860 2023-05-18 15:56:21.000000 enthought_sphinx_theme-0.7.3/less/bootstrap/media.less
+-rw-r--r--   0 runner    (1001) docker     (123)    23042 2023-05-18 15:56:21.000000 enthought_sphinx_theme-0.7.3/less/bootstrap/mixins.less
+-rw-r--r--   0 runner    (1001) docker     (123)     1978 2023-05-18 15:56:21.000000 enthought_sphinx_theme-0.7.3/less/bootstrap/modals.less
+-rw-r--r--   0 runner    (1001) docker     (123)    12002 2023-05-18 15:56:21.000000 enthought_sphinx_theme-0.7.3/less/bootstrap/navbar.less
+-rw-r--r--   0 runner    (1001) docker     (123)     8163 2023-05-18 15:56:21.000000 enthought_sphinx_theme-0.7.3/less/bootstrap/navs.less
+-rw-r--r--   0 runner    (1001) docker     (123)      760 2023-05-18 15:56:21.000000 enthought_sphinx_theme-0.7.3/less/bootstrap/pager.less
+-rw-r--r--   0 runner    (1001) docker     (123)     2678 2023-05-18 15:56:21.000000 enthought_sphinx_theme-0.7.3/less/bootstrap/pagination.less
+-rw-r--r--   0 runner    (1001) docker     (123)     3077 2023-05-18 15:56:21.000000 enthought_sphinx_theme-0.7.3/less/bootstrap/popovers.less
+-rw-r--r--   0 runner    (1001) docker     (123)     2858 2023-05-18 15:56:21.000000 enthought_sphinx_theme-0.7.3/less/bootstrap/progress-bars.less
+-rw-r--r--   0 runner    (1001) docker     (123)     4201 2023-05-18 15:56:21.000000 enthought_sphinx_theme-0.7.3/less/bootstrap/reset.less
+-rw-r--r--   0 runner    (1001) docker     (123)      565 2023-05-18 15:56:21.000000 enthought_sphinx_theme-0.7.3/less/bootstrap/responsive-1200px-min.less
+-rw-r--r--   0 runner    (1001) docker     (123)     3920 2023-05-18 15:56:21.000000 enthought_sphinx_theme-0.7.3/less/bootstrap/responsive-767px-max.less
+-rw-r--r--   0 runner    (1001) docker     (123)      463 2023-05-18 15:56:21.000000 enthought_sphinx_theme-0.7.3/less/bootstrap/responsive-768px-979px.less
+-rw-r--r--   0 runner    (1001) docker     (123)     4328 2023-05-18 15:56:21.000000 enthought_sphinx_theme-0.7.3/less/bootstrap/responsive-navbar.less
+-rw-r--r--   0 runner    (1001) docker     (123)     1602 2023-05-18 15:56:21.000000 enthought_sphinx_theme-0.7.3/less/bootstrap/responsive-utilities.less
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-18 15:56:21.000000 enthought_sphinx_theme-0.7.3/less/bootstrap/responsive.less
+-rw-r--r--   0 runner    (1001) docker     (123)      885 2023-05-18 15:56:21.000000 enthought_sphinx_theme-0.7.3/less/bootstrap/scaffolding.less
+-rw-r--r--   0 runner    (1001) docker     (123)    10841 2023-05-18 15:56:21.000000 enthought_sphinx_theme-0.7.3/less/bootstrap/sprites.less
+-rw-r--r--   0 runner    (1001) docker     (123)     6255 2023-05-18 15:56:21.000000 enthought_sphinx_theme-0.7.3/less/bootstrap/tables.less
+-rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-05-18 15:56:21.000000 enthought_sphinx_theme-0.7.3/less/bootstrap/thumbnails.less
+-rw-r--r--   0 runner    (1001) docker     (123)     1684 2023-05-18 15:56:21.000000 enthought_sphinx_theme-0.7.3/less/bootstrap/tooltip.less
+-rw-r--r--   0 runner    (1001) docker     (123)     4857 2023-05-18 15:56:21.000000 enthought_sphinx_theme-0.7.3/less/bootstrap/type.less
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-05-18 15:56:21.000000 enthought_sphinx_theme-0.7.3/less/bootstrap/utilities.less
+-rw-r--r--   0 runner    (1001) docker     (123)     9142 2023-05-18 15:56:21.000000 enthought_sphinx_theme-0.7.3/less/bootstrap/variables.less
+-rw-r--r--   0 runner    (1001) docker     (123)      552 2023-05-18 15:56:21.000000 enthought_sphinx_theme-0.7.3/less/bootstrap/wells.less
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-05-18 15:56:21.000000 enthought_sphinx_theme-0.7.3/less/spc-bootstrap.less
+-rw-r--r--   0 runner    (1001) docker     (123)      832 2023-05-18 15:56:21.000000 enthought_sphinx_theme-0.7.3/less/spc-content.less
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-05-18 15:56:21.000000 enthought_sphinx_theme-0.7.3/less/spc-extend.less
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-05-18 15:56:21.000000 enthought_sphinx_theme-0.7.3/less/spc-footer.less
+-rw-r--r--   0 runner    (1001) docker     (123)      441 2023-05-18 15:56:21.000000 enthought_sphinx_theme-0.7.3/less/spc-header.less
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-05-18 15:56:21.000000 enthought_sphinx_theme-0.7.3/less/spc-rightsidebar.less
+-rw-r--r--   0 runner    (1001) docker     (123)      425 2023-05-18 15:56:21.000000 enthought_sphinx_theme-0.7.3/less/spc-utils.less
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:56:36.525856 enthought_sphinx_theme-0.7.3/licenses/
+-rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-05-18 15:56:21.000000 enthought_sphinx_theme-0.7.3/licenses/bootstrap.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5065 2023-05-18 15:56:21.000000 enthought_sphinx_theme-0.7.3/licenses/fonts.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1791 2023-05-18 15:56:21.000000 enthought_sphinx_theme-0.7.3/licenses/scipy-sphinx-theme.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-18 15:56:36.529856 enthought_sphinx_theme-0.7.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      891 2023-05-18 15:56:21.000000 enthought_sphinx_theme-0.7.3/setup.py
```

### Comparing `enthought_sphinx_theme-0.7.2/LICENSE` & `enthought_sphinx_theme-0.7.3/LICENSE`

 * *Files identical despite different names*

### Comparing `enthought_sphinx_theme-0.7.2/PKG-INFO` & `enthought_sphinx_theme-0.7.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: enthought_sphinx_theme
-Version: 0.7.2
+Version: 0.7.3
 Summary: Sphinx theme for Enthought products
 Home-page: https://github.com/enthought/enthought-sphinx-theme
 Author: Enthought, Inc.
 Author-email: info@enthought.com
 License: BSD
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `enthought_sphinx_theme-0.7.2/README.rst` & `enthought_sphinx_theme-0.7.3/README.rst`

 * *Files identical despite different names*

### Comparing `enthought_sphinx_theme-0.7.2/enthought_sphinx_theme/enthought/layout.html` & `enthought_sphinx_theme-0.7.3/enthought_sphinx_theme/enthought/layout.html`

 * *Files 0% similar despite different names*

```diff
@@ -108,15 +108,15 @@
     <script type="text/javascript" src="{{ pathto('_static/js/copybutton.js', 1) }}"></script>
     <script type="text/javascript" src="{{ pathto('_static/js/wrap_on_dot.js', 1) }}"></script>
 {%- endmacro %}
 
 {%- macro css() %}
     <link rel="stylesheet" type="text/css" href="{{ pathto('_static/css/spc-bootstrap.css', 1) }}">
     <link rel="stylesheet" type="text/css" href="{{ pathto('_static/css/spc-extend.css', 1) }}">
-    <link rel="stylesheet" href="{{ pathto('_static/' + style, 1) }}" type="text/css" >
+    <link rel="stylesheet" href="{{ pathto('_static/' + styles[0], 1) }}" type="text/css" >
     <link rel="stylesheet" href="{{ pathto('_static/pygments.css', 1) }}" type="text/css" >
     {%- for cssfile in css_files %}
     <link rel="stylesheet" href="{{ pathto(cssfile, 1) }}" type="text/css" >
     {%- endfor %}
 {%- endmacro %}
 
 <html>
```

### Comparing `enthought_sphinx_theme-0.7.2/enthought_sphinx_theme/enthought/static/css/pygments.css` & `enthought_sphinx_theme-0.7.3/enthought_sphinx_theme/enthought/static/css/pygments.css`

 * *Files identical despite different names*

### Comparing `enthought_sphinx_theme-0.7.2/enthought_sphinx_theme/enthought/static/css/spc-bootstrap.css` & `enthought_sphinx_theme-0.7.3/enthought_sphinx_theme/enthought/static/css/spc-bootstrap.css`

 * *Files identical despite different names*

### Comparing `enthought_sphinx_theme-0.7.2/enthought_sphinx_theme/enthought/static/css/spc-extend.css` & `enthought_sphinx_theme-0.7.3/enthought_sphinx_theme/enthought/static/css/spc-extend.css`

 * *Files identical despite different names*

### Comparing `enthought_sphinx_theme-0.7.2/enthought_sphinx_theme/enthought/static/enthought.css_t` & `enthought_sphinx_theme-0.7.3/enthought_sphinx_theme/enthought/static/enthought.css_t`

 * *Files identical despite different names*

### Comparing `enthought_sphinx_theme-0.7.2/enthought_sphinx_theme/enthought/static/fonts/SourceCodePro-Regular.otf.woff` & `enthought_sphinx_theme-0.7.3/enthought_sphinx_theme/enthought/static/fonts/SourceCodePro-Regular.otf.woff`

 * *Files identical despite different names*

### Comparing `enthought_sphinx_theme-0.7.2/enthought_sphinx_theme/enthought/static/fonts/SourceCodePro-Semibold.otf.woff` & `enthought_sphinx_theme-0.7.3/enthought_sphinx_theme/enthought/static/fonts/SourceCodePro-Semibold.otf.woff`

 * *Files identical despite different names*

### Comparing `enthought_sphinx_theme-0.7.2/enthought_sphinx_theme/enthought/static/fonts/poppins-v19-latin-600.woff2` & `enthought_sphinx_theme-0.7.3/enthought_sphinx_theme/enthought/static/fonts/poppins-v19-latin-600.woff2`

 * *Files identical despite different names*

### Comparing `enthought_sphinx_theme-0.7.2/enthought_sphinx_theme/enthought/static/fonts/poppins-v19-latin-600italic.woff2` & `enthought_sphinx_theme-0.7.3/enthought_sphinx_theme/enthought/static/fonts/poppins-v19-latin-600italic.woff2`

 * *Files identical despite different names*

### Comparing `enthought_sphinx_theme-0.7.2/enthought_sphinx_theme/enthought/static/fonts/poppins-v19-latin-italic.woff2` & `enthought_sphinx_theme-0.7.3/enthought_sphinx_theme/enthought/static/fonts/poppins-v19-latin-italic.woff2`

 * *Files identical despite different names*

### Comparing `enthought_sphinx_theme-0.7.2/enthought_sphinx_theme/enthought/static/fonts/poppins-v19-latin-regular.woff2` & `enthought_sphinx_theme-0.7.3/enthought_sphinx_theme/enthought/static/fonts/poppins-v19-latin-regular.woff2`

 * *Files identical despite different names*

### Comparing `enthought_sphinx_theme-0.7.2/enthought_sphinx_theme/enthought/static/img/e-logo.png` & `enthought_sphinx_theme-0.7.3/enthought_sphinx_theme/enthought/static/img/e-logo.png`

 * *Files identical despite different names*

### Comparing `enthought_sphinx_theme-0.7.2/enthought_sphinx_theme/enthought/static/img/favicon.png` & `enthought_sphinx_theme-0.7.3/enthought_sphinx_theme/enthought/static/img/favicon.png`

 * *Files identical despite different names*

### Comparing `enthought_sphinx_theme-0.7.2/enthought_sphinx_theme/enthought/static/img/glyphicons-halflings-white.png` & `enthought_sphinx_theme-0.7.3/enthought_sphinx_theme/enthought/static/img/glyphicons-halflings-white.png`

 * *Files identical despite different names*

### Comparing `enthought_sphinx_theme-0.7.2/enthought_sphinx_theme/enthought/static/img/glyphicons-halflings.png` & `enthought_sphinx_theme-0.7.3/enthought_sphinx_theme/enthought/static/img/glyphicons-halflings.png`

 * *Files identical despite different names*

### Comparing `enthought_sphinx_theme-0.7.2/enthought_sphinx_theme/enthought/static/img/ui-anim_basic_16x16.gif` & `enthought_sphinx_theme-0.7.3/enthought_sphinx_theme/enthought/static/img/ui-anim_basic_16x16.gif`

 * *Files identical despite different names*

### Comparing `enthought_sphinx_theme-0.7.2/enthought_sphinx_theme/enthought/static/js/copybutton.js` & `enthought_sphinx_theme-0.7.3/enthought_sphinx_theme/enthought/static/js/copybutton.js`

 * *Files identical despite different names*

### Comparing `enthought_sphinx_theme-0.7.2/enthought_sphinx_theme.egg-info/PKG-INFO` & `enthought_sphinx_theme-0.7.3/enthought_sphinx_theme.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: enthought-sphinx-theme
-Version: 0.7.2
+Version: 0.7.3
 Summary: Sphinx theme for Enthought products
 Home-page: https://github.com/enthought/enthought-sphinx-theme
 Author: Enthought, Inc.
 Author-email: info@enthought.com
 License: BSD
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `enthought_sphinx_theme-0.7.2/enthought_sphinx_theme.egg-info/SOURCES.txt` & `enthought_sphinx_theme-0.7.3/enthought_sphinx_theme.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `enthought_sphinx_theme-0.7.2/less/bootstrap/accordion.less` & `enthought_sphinx_theme-0.7.3/less/bootstrap/accordion.less`

 * *Files identical despite different names*

### Comparing `enthought_sphinx_theme-0.7.2/less/bootstrap/alerts.less` & `enthought_sphinx_theme-0.7.3/less/bootstrap/alerts.less`

 * *Files identical despite different names*

### Comparing `enthought_sphinx_theme-0.7.2/less/bootstrap/bootstrap.less` & `enthought_sphinx_theme-0.7.3/less/bootstrap/bootstrap.less`

 * *Files identical despite different names*

### Comparing `enthought_sphinx_theme-0.7.2/less/bootstrap/button-groups.less` & `enthought_sphinx_theme-0.7.3/less/bootstrap/button-groups.less`

 * *Files identical despite different names*

### Comparing `enthought_sphinx_theme-0.7.2/less/bootstrap/buttons.less` & `enthought_sphinx_theme-0.7.3/less/bootstrap/buttons.less`

 * *Files identical despite different names*

### Comparing `enthought_sphinx_theme-0.7.2/less/bootstrap/carousel.less` & `enthought_sphinx_theme-0.7.3/less/bootstrap/carousel.less`

 * *Files identical despite different names*

### Comparing `enthought_sphinx_theme-0.7.2/less/bootstrap/close.less` & `enthought_sphinx_theme-0.7.3/less/bootstrap/close.less`

 * *Files identical despite different names*

### Comparing `enthought_sphinx_theme-0.7.2/less/bootstrap/code.less` & `enthought_sphinx_theme-0.7.3/less/bootstrap/code.less`

 * *Files identical despite different names*

### Comparing `enthought_sphinx_theme-0.7.2/less/bootstrap/dropdowns.less` & `enthought_sphinx_theme-0.7.3/less/bootstrap/dropdowns.less`

 * *Files identical despite different names*

### Comparing `enthought_sphinx_theme-0.7.2/less/bootstrap/forms.less` & `enthought_sphinx_theme-0.7.3/less/bootstrap/forms.less`

 * *Files identical despite different names*

### Comparing `enthought_sphinx_theme-0.7.2/less/bootstrap/hero-unit.less` & `enthought_sphinx_theme-0.7.3/less/bootstrap/hero-unit.less`

 * *Files identical despite different names*

### Comparing `enthought_sphinx_theme-0.7.2/less/bootstrap/labels-badges.less` & `enthought_sphinx_theme-0.7.3/less/bootstrap/labels-badges.less`

 * *Files identical despite different names*

### Comparing `enthought_sphinx_theme-0.7.2/less/bootstrap/media.less` & `enthought_sphinx_theme-0.7.3/less/bootstrap/media.less`

 * *Files identical despite different names*

### Comparing `enthought_sphinx_theme-0.7.2/less/bootstrap/mixins.less` & `enthought_sphinx_theme-0.7.3/less/bootstrap/mixins.less`

 * *Files identical despite different names*

### Comparing `enthought_sphinx_theme-0.7.2/less/bootstrap/modals.less` & `enthought_sphinx_theme-0.7.3/less/bootstrap/modals.less`

 * *Files identical despite different names*

### Comparing `enthought_sphinx_theme-0.7.2/less/bootstrap/navbar.less` & `enthought_sphinx_theme-0.7.3/less/bootstrap/navbar.less`

 * *Files identical despite different names*

### Comparing `enthought_sphinx_theme-0.7.2/less/bootstrap/navs.less` & `enthought_sphinx_theme-0.7.3/less/bootstrap/navs.less`

 * *Files identical despite different names*

### Comparing `enthought_sphinx_theme-0.7.2/less/bootstrap/pager.less` & `enthought_sphinx_theme-0.7.3/less/bootstrap/pager.less`

 * *Files identical despite different names*

### Comparing `enthought_sphinx_theme-0.7.2/less/bootstrap/pagination.less` & `enthought_sphinx_theme-0.7.3/less/bootstrap/pagination.less`

 * *Files identical despite different names*

### Comparing `enthought_sphinx_theme-0.7.2/less/bootstrap/popovers.less` & `enthought_sphinx_theme-0.7.3/less/bootstrap/popovers.less`

 * *Files identical despite different names*

### Comparing `enthought_sphinx_theme-0.7.2/less/bootstrap/progress-bars.less` & `enthought_sphinx_theme-0.7.3/less/bootstrap/progress-bars.less`

 * *Files identical despite different names*

### Comparing `enthought_sphinx_theme-0.7.2/less/bootstrap/reset.less` & `enthought_sphinx_theme-0.7.3/less/bootstrap/reset.less`

 * *Files identical despite different names*

### Comparing `enthought_sphinx_theme-0.7.2/less/bootstrap/responsive-1200px-min.less` & `enthought_sphinx_theme-0.7.3/less/bootstrap/responsive-1200px-min.less`

 * *Files identical despite different names*

### Comparing `enthought_sphinx_theme-0.7.2/less/bootstrap/responsive-767px-max.less` & `enthought_sphinx_theme-0.7.3/less/bootstrap/responsive-767px-max.less`

 * *Files identical despite different names*

### Comparing `enthought_sphinx_theme-0.7.2/less/bootstrap/responsive-navbar.less` & `enthought_sphinx_theme-0.7.3/less/bootstrap/responsive-navbar.less`

 * *Files identical despite different names*

### Comparing `enthought_sphinx_theme-0.7.2/less/bootstrap/responsive-utilities.less` & `enthought_sphinx_theme-0.7.3/less/bootstrap/responsive-utilities.less`

 * *Files identical despite different names*

### Comparing `enthought_sphinx_theme-0.7.2/less/bootstrap/responsive.less` & `enthought_sphinx_theme-0.7.3/less/bootstrap/responsive.less`

 * *Files identical despite different names*

### Comparing `enthought_sphinx_theme-0.7.2/less/bootstrap/scaffolding.less` & `enthought_sphinx_theme-0.7.3/less/bootstrap/scaffolding.less`

 * *Files identical despite different names*

### Comparing `enthought_sphinx_theme-0.7.2/less/bootstrap/sprites.less` & `enthought_sphinx_theme-0.7.3/less/bootstrap/sprites.less`

 * *Files identical despite different names*

### Comparing `enthought_sphinx_theme-0.7.2/less/bootstrap/tables.less` & `enthought_sphinx_theme-0.7.3/less/bootstrap/tables.less`

 * *Files identical despite different names*

### Comparing `enthought_sphinx_theme-0.7.2/less/bootstrap/thumbnails.less` & `enthought_sphinx_theme-0.7.3/less/bootstrap/thumbnails.less`

 * *Files identical despite different names*

### Comparing `enthought_sphinx_theme-0.7.2/less/bootstrap/tooltip.less` & `enthought_sphinx_theme-0.7.3/less/bootstrap/tooltip.less`

 * *Files identical despite different names*

### Comparing `enthought_sphinx_theme-0.7.2/less/bootstrap/type.less` & `enthought_sphinx_theme-0.7.3/less/bootstrap/type.less`

 * *Files identical despite different names*

### Comparing `enthought_sphinx_theme-0.7.2/less/bootstrap/variables.less` & `enthought_sphinx_theme-0.7.3/less/bootstrap/variables.less`

 * *Files identical despite different names*

### Comparing `enthought_sphinx_theme-0.7.2/less/bootstrap/wells.less` & `enthought_sphinx_theme-0.7.3/less/bootstrap/wells.less`

 * *Files identical despite different names*

### Comparing `enthought_sphinx_theme-0.7.2/less/spc-content.less` & `enthought_sphinx_theme-0.7.3/less/spc-content.less`

 * *Files identical despite different names*

### Comparing `enthought_sphinx_theme-0.7.2/licenses/bootstrap.txt` & `enthought_sphinx_theme-0.7.3/licenses/bootstrap.txt`

 * *Files identical despite different names*

### Comparing `enthought_sphinx_theme-0.7.2/licenses/fonts.txt` & `enthought_sphinx_theme-0.7.3/licenses/fonts.txt`

 * *Files identical despite different names*

### Comparing `enthought_sphinx_theme-0.7.2/licenses/scipy-sphinx-theme.txt` & `enthought_sphinx_theme-0.7.3/licenses/scipy-sphinx-theme.txt`

 * *Files identical despite different names*

### Comparing `enthought_sphinx_theme-0.7.2/setup.py` & `enthought_sphinx_theme-0.7.3/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 with open(os.path.join(os.path.dirname(__file__), 'README.rst')) as f:
     long_description = f.read().strip()
 
 
 setup(
     name='enthought_sphinx_theme',
-    version='0.7.2',
+    version='0.7.3',
     author='Enthought, Inc.',
     author_email='info@enthought.com',
     description='Sphinx theme for Enthought products',
     long_description=long_description,
     long_description_content_type="text/x-rst",
     url='https://github.com/enthought/enthought-sphinx-theme',
     packages=find_packages(),
```

