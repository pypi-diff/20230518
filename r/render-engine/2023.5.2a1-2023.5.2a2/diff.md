# Comparing `tmp/render_engine-2023.5.2a1.tar.gz` & `tmp/render_engine-2023.5.2a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "render_engine-2023.5.2a1.tar", last modified: Mon May 15 21:44:14 2023, max compression
+gzip compressed data, was "render_engine-2023.5.2a2.tar", last modified: Thu May 18 14:36:44 2023, max compression
```

## Comparing `render_engine-2023.5.2a1.tar` & `render_engine-2023.5.2a2.tar`

### file list

```diff
@@ -1,125 +1,125 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 21:44:14.181126 render_engine-2023.5.2a1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 21:44:14.169125 render_engine-2023.5.2a1/.chglog/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1142 2023-05-15 21:43:57.000000 render_engine-2023.5.2a1/.chglog/CHANGELOG.tpl.md
--rwxr-xr-x   0 runner    (1001) docker     (123)      330 2023-05-15 21:43:57.000000 render_engine-2023.5.2a1/.chglog/config.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 21:44:14.169125 render_engine-2023.5.2a1/.devcontainer/
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-05-15 21:43:57.000000 render_engine-2023.5.2a1/.devcontainer/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-05-15 21:43:57.000000 render_engine-2023.5.2a1/.devcontainer/devcontainer.json
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-05-15 21:43:57.000000 render_engine-2023.5.2a1/.devcontainer/setup.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 21:44:14.169125 render_engine-2023.5.2a1/.github/
--rw-r--r--   0 runner    (1001) docker     (123)     4511 2023-05-15 21:43:57.000000 render_engine-2023.5.2a1/.github/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     1743 2023-05-15 21:43:57.000000 render_engine-2023.5.2a1/.github/CONTRIBUTION.md
--rw-r--r--   0 runner    (1001) docker     (123)      722 2023-05-15 21:43:57.000000 render_engine-2023.5.2a1/.github/FUNDING.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-05-15 21:43:57.000000 render_engine-2023.5.2a1/.github/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 21:44:14.169125 render_engine-2023.5.2a1/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      332 2023-05-15 21:43:57.000000 render_engine-2023.5.2a1/.github/PULL_REQUEST_TEMPLATE/pull_request_template.md
--rw-r--r--   0 runner    (1001) docker     (123)      673 2023-05-15 21:43:57.000000 render_engine-2023.5.2a1/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 21:44:14.169125 render_engine-2023.5.2a1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      783 2023-05-15 21:43:57.000000 render_engine-2023.5.2a1/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      414 2023-05-15 21:43:57.000000 render_engine-2023.5.2a1/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2832 2023-05-15 21:43:57.000000 render_engine-2023.5.2a1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      478 2023-05-15 21:43:57.000000 render_engine-2023.5.2a1/.readthedocs.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 21:44:14.169125 render_engine-2023.5.2a1/.vscode/
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-05-15 21:43:57.000000 render_engine-2023.5.2a1/.vscode/tasks.json
--rw-r--r--   0 runner    (1001) docker     (123)      437 2023-05-15 21:43:57.000000 render_engine-2023.5.2a1/Contributing.md
--rw-r--r--   0 runner    (1001) docker     (123)     2475 2023-05-15 21:44:14.181126 render_engine-2023.5.2a1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2085 2023-05-15 21:43:57.000000 render_engine-2023.5.2a1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)    12647 2023-05-15 21:43:57.000000 render_engine-2023.5.2a1/changelog.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 21:44:14.169125 render_engine-2023.5.2a1/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 21:44:14.169125 render_engine-2023.5.2a1/docs/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      920 2023-05-15 21:43:57.000000 render_engine-2023.5.2a1/docs/docs/archive.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 21:44:14.173126 render_engine-2023.5.2a1/docs/docs/assets/
--rw-r--r--   0 runner    (1001) docker     (123)   273561 2023-05-15 21:43:57.000000 render_engine-2023.5.2a1/docs/docs/assets/create-app-help.png
--rw-r--r--   0 runner    (1001) docker     (123)   288201 2023-05-15 21:43:57.000000 render_engine-2023.5.2a1/docs/docs/assets/render-engine-init-help.png
--rw-r--r--   0 runner    (1001) docker     (123)    90538 2023-05-15 21:43:57.000000 render_engine-2023.5.2a1/docs/docs/assets/render-engine-init.png
--rw-r--r--   0 runner    (1001) docker     (123)     2713 2023-05-15 21:43:57.000000 render_engine-2023.5.2a1/docs/docs/cli.md
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-15 21:43:57.000000 render_engine-2023.5.2a1/docs/docs/collection.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 21:44:14.173126 render_engine-2023.5.2a1/docs/docs/contributing/
--rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-05-15 21:43:57.000000 render_engine-2023.5.2a1/docs/docs/contributing/pages.md
--rw-r--r--   0 runner    (1001) docker     (123)     3023 2023-05-15 21:43:57.000000 render_engine-2023.5.2a1/docs/docs/custom_collections.md
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-15 21:43:57.000000 render_engine-2023.5.2a1/docs/docs/feeds.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 21:44:14.173126 render_engine-2023.5.2a1/docs/docs/getting-started/
--rw-r--r--   0 runner    (1001) docker     (123)      692 2023-05-15 21:43:57.000000 render_engine-2023.5.2a1/docs/docs/getting-started/building-your-site.md
--rw-r--r--   0 runner    (1001) docker     (123)     1777 2023-05-15 21:43:57.000000 render_engine-2023.5.2a1/docs/docs/getting-started/creating-a-collection.md
--rw-r--r--   0 runner    (1001) docker     (123)     2460 2023-05-15 21:43:57.000000 render_engine-2023.5.2a1/docs/docs/getting-started/creating-a-page.md
--rw-r--r--   0 runner    (1001) docker     (123)      453 2023-05-15 21:43:57.000000 render_engine-2023.5.2a1/docs/docs/getting-started/creating-your-app.md
--rw-r--r--   0 runner    (1001) docker     (123)      727 2023-05-15 21:43:57.000000 render_engine-2023.5.2a1/docs/docs/getting-started/installation.md
--rw-r--r--   0 runner    (1001) docker     (123)     4598 2023-05-15 21:43:57.000000 render_engine-2023.5.2a1/docs/docs/getting-started/layout.md
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-15 21:43:57.000000 render_engine-2023.5.2a1/docs/docs/hookspecs.md
--rw-r--r--   0 runner    (1001) docker     (123)      906 2023-05-15 21:43:57.000000 render_engine-2023.5.2a1/docs/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (123)      679 2023-05-15 21:43:57.000000 render_engine-2023.5.2a1/docs/docs/page.md
--rw-r--r--   0 runner    (1001) docker     (123)     3041 2023-05-15 21:43:57.000000 render_engine-2023.5.2a1/docs/docs/parsers.md
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-15 21:43:57.000000 render_engine-2023.5.2a1/docs/docs/plugins.md
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-15 21:43:57.000000 render_engine-2023.5.2a1/docs/docs/site.md
--rw-r--r--   0 runner    (1001) docker     (123)     2866 2023-05-15 21:43:57.000000 render_engine-2023.5.2a1/docs/docs/templates.md
--rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-05-15 21:43:57.000000 render_engine-2023.5.2a1/docs/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-15 21:43:57.000000 render_engine-2023.5.2a1/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1436 2023-05-15 21:43:57.000000 render_engine-2023.5.2a1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-05-15 21:43:57.000000 render_engine-2023.5.2a1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-15 21:44:14.181126 render_engine-2023.5.2a1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 21:44:14.173126 render_engine-2023.5.2a1/src/
--rw-r--r--   0 runner    (1001) docker     (123)     6148 2023-05-15 21:43:57.000000 render_engine-2023.5.2a1/src/.DS_Store
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 21:44:14.177126 render_engine-2023.5.2a1/src/render_engine/
--rw-r--r--   0 runner    (1001) docker     (123)     6148 2023-05-15 21:43:57.000000 render_engine-2023.5.2a1/src/render_engine/.DS_Store
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-15 21:43:57.000000 render_engine-2023.5.2a1/src/render_engine/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-15 21:43:57.000000 render_engine-2023.5.2a1/src/render_engine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-05-15 21:43:57.000000 render_engine-2023.5.2a1/src/render_engine/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1879 2023-05-15 21:43:57.000000 render_engine-2023.5.2a1/src/render_engine/_base_object.py
--rw-r--r--   0 runner    (1001) docker     (123)     1378 2023-05-15 21:43:57.000000 render_engine-2023.5.2a1/src/render_engine/archive.py
--rw-r--r--   0 runner    (1001) docker     (123)      714 2023-05-15 21:43:57.000000 render_engine-2023.5.2a1/src/render_engine/blog.py
--rw-r--r--   0 runner    (1001) docker     (123)    10320 2023-05-15 21:43:57.000000 render_engine-2023.5.2a1/src/render_engine/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     6271 2023-05-15 21:43:57.000000 render_engine-2023.5.2a1/src/render_engine/collection.py
--rw-r--r--   0 runner    (1001) docker     (123)     2025 2023-05-15 21:43:57.000000 render_engine-2023.5.2a1/src/render_engine/engine.py
--rw-r--r--   0 runner    (1001) docker     (123)      907 2023-05-15 21:43:57.000000 render_engine-2023.5.2a1/src/render_engine/feeds.py
--rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-05-15 21:43:57.000000 render_engine-2023.5.2a1/src/render_engine/hookspecs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1914 2023-05-15 21:43:57.000000 render_engine-2023.5.2a1/src/render_engine/links.py
--rw-r--r--   0 runner    (1001) docker     (123)     5826 2023-05-15 21:43:57.000000 render_engine-2023.5.2a1/src/render_engine/page.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 21:44:14.177126 render_engine-2023.5.2a1/src/render_engine/parsers/
--rw-r--r--   0 runner    (1001) docker     (123)     6148 2023-05-15 21:43:57.000000 render_engine-2023.5.2a1/src/render_engine/parsers/.DS_Store
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-05-15 21:43:57.000000 render_engine-2023.5.2a1/src/render_engine/parsers/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      681 2023-05-15 21:43:57.000000 render_engine-2023.5.2a1/src/render_engine/parsers/README_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-15 21:43:57.000000 render_engine-2023.5.2a1/src/render_engine/parsers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1729 2023-05-15 21:43:57.000000 render_engine-2023.5.2a1/src/render_engine/parsers/base_parsers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 21:44:14.177126 render_engine-2023.5.2a1/src/render_engine/parsers/markdown/
--rw-r--r--   0 runner    (1001) docker     (123)      982 2023-05-15 21:43:57.000000 render_engine-2023.5.2a1/src/render_engine/parsers/markdown/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-05-15 21:43:57.000000 render_engine-2023.5.2a1/src/render_engine/parsers/markdown/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-05-15 21:43:57.000000 render_engine-2023.5.2a1/src/render_engine/plugins.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 21:44:14.177126 render_engine-2023.5.2a1/src/render_engine/render_engine_templates/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 21:43:57.000000 render_engine-2023.5.2a1/src/render_engine/render_engine_templates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      448 2023-05-15 21:43:57.000000 render_engine-2023.5.2a1/src/render_engine/render_engine_templates/base.html
--rw-r--r--   0 runner    (1001) docker     (123)      430 2023-05-15 21:43:57.000000 render_engine-2023.5.2a1/src/render_engine/render_engine_templates/base_collection_path.md
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-15 21:43:57.000000 render_engine-2023.5.2a1/src/render_engine/render_engine_templates/content.html
--rw-r--r--   0 runner    (1001) docker     (123)      880 2023-05-15 21:43:57.000000 render_engine-2023.5.2a1/src/render_engine/render_engine_templates/create_app_py.txt
--rw-r--r--   0 runner    (1001) docker     (123)      525 2023-05-15 21:43:57.000000 render_engine-2023.5.2a1/src/render_engine/render_engine_templates/index.html
--rw-r--r--   0 runner    (1001) docker     (123)     1786 2023-05-15 21:43:57.000000 render_engine-2023.5.2a1/src/render_engine/render_engine_templates/rss2.0.xml
--rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-05-15 21:43:57.000000 render_engine-2023.5.2a1/src/render_engine/render_engine_templates/rss2.0_items.xml
--rwxr-xr-x   0 runner    (1001) docker     (123)      180 2023-05-15 21:43:57.000000 render_engine-2023.5.2a1/src/render_engine/render_engine_templates/sitemap.xml
--rwxr-xr-x   0 runner    (1001) docker     (123)      283 2023-05-15 21:43:57.000000 render_engine-2023.5.2a1/src/render_engine/render_engine_templates/sitemap_item.xml
--rw-r--r--   0 runner    (1001) docker     (123)     7549 2023-05-15 21:43:57.000000 render_engine-2023.5.2a1/src/render_engine/site.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 21:44:14.177126 render_engine-2023.5.2a1/src/render_engine.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2475 2023-05-15 21:44:14.000000 render_engine-2023.5.2a1/src/render_engine.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3191 2023-05-15 21:44:14.000000 render_engine-2023.5.2a1/src/render_engine.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 21:44:14.000000 render_engine-2023.5.2a1/src/render_engine.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-15 21:44:14.000000 render_engine-2023.5.2a1/src/render_engine.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-05-15 21:44:14.000000 render_engine-2023.5.2a1/src/render_engine.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-15 21:44:14.000000 render_engine-2023.5.2a1/src/render_engine.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 21:44:14.181126 render_engine-2023.5.2a1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      991 2023-05-15 21:43:57.000000 render_engine-2023.5.2a1/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      576 2023-05-15 21:43:57.000000 render_engine-2023.5.2a1/tests/create_app_check_file.txt
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-05-15 21:43:57.000000 render_engine-2023.5.2a1/tests/create_app_check_file_no_site_vars.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 21:44:14.181126 render_engine-2023.5.2a1/tests/site_test/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 21:44:14.181126 render_engine-2023.5.2a1/tests/site_test/blog/
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-05-15 21:43:57.000000 render_engine-2023.5.2a1/tests/site_test/blog/test_blog_content.md
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-05-15 21:43:57.000000 render_engine-2023.5.2a1/tests/site_test/build.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 21:44:14.181126 render_engine-2023.5.2a1/tests/site_test/templates/
--rw-r--r--   0 runner    (1001) docker     (123)      279 2023-05-15 21:43:57.000000 render_engine-2023.5.2a1/tests/site_test/templates/index.html
--rw-r--r--   0 runner    (1001) docker     (123)      506 2023-05-15 21:43:57.000000 render_engine-2023.5.2a1/tests/test_archive.py
--rw-r--r--   0 runner    (1001) docker     (123)     2058 2023-05-15 21:43:57.000000 render_engine-2023.5.2a1/tests/test_base_object.py
--rw-r--r--   0 runner    (1001) docker     (123)     1586 2023-05-15 21:43:57.000000 render_engine-2023.5.2a1/tests/test_base_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-05-15 21:43:57.000000 render_engine-2023.5.2a1/tests/test_blog.py
--rw-r--r--   0 runner    (1001) docker     (123)     3930 2023-05-15 21:43:57.000000 render_engine-2023.5.2a1/tests/test_collections.py
--rw-r--r--   0 runner    (1001) docker     (123)     1775 2023-05-15 21:43:57.000000 render_engine-2023.5.2a1/tests/test_create_app.py
--rw-r--r--   0 runner    (1001) docker     (123)     3308 2023-05-15 21:43:57.000000 render_engine-2023.5.2a1/tests/test_feeds.py
--rw-r--r--   0 runner    (1001) docker     (123)     1441 2023-05-15 21:43:57.000000 render_engine-2023.5.2a1/tests/test_page.py
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-05-15 21:43:57.000000 render_engine-2023.5.2a1/tests/test_parser_markdown_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     8607 2023-05-15 21:43:57.000000 render_engine-2023.5.2a1/tests/test_site.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 14:36:44.676370 render_engine-2023.5.2a2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 14:36:44.664371 render_engine-2023.5.2a2/.chglog/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1142 2023-05-18 14:36:26.000000 render_engine-2023.5.2a2/.chglog/CHANGELOG.tpl.md
+-rwxr-xr-x   0 runner    (1001) docker     (123)      330 2023-05-18 14:36:26.000000 render_engine-2023.5.2a2/.chglog/config.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 14:36:44.664371 render_engine-2023.5.2a2/.devcontainer/
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-05-18 14:36:26.000000 render_engine-2023.5.2a2/.devcontainer/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-05-18 14:36:26.000000 render_engine-2023.5.2a2/.devcontainer/devcontainer.json
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-05-18 14:36:26.000000 render_engine-2023.5.2a2/.devcontainer/setup.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 14:36:44.668371 render_engine-2023.5.2a2/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)     4511 2023-05-18 14:36:26.000000 render_engine-2023.5.2a2/.github/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1743 2023-05-18 14:36:26.000000 render_engine-2023.5.2a2/.github/CONTRIBUTION.md
+-rw-r--r--   0 runner    (1001) docker     (123)      722 2023-05-18 14:36:26.000000 render_engine-2023.5.2a2/.github/FUNDING.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-05-18 14:36:26.000000 render_engine-2023.5.2a2/.github/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 14:36:44.668371 render_engine-2023.5.2a2/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-05-18 14:36:26.000000 render_engine-2023.5.2a2/.github/PULL_REQUEST_TEMPLATE/pull_request_template.md
+-rw-r--r--   0 runner    (1001) docker     (123)      673 2023-05-18 14:36:26.000000 render_engine-2023.5.2a2/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 14:36:44.668371 render_engine-2023.5.2a2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      783 2023-05-18 14:36:26.000000 render_engine-2023.5.2a2/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      414 2023-05-18 14:36:26.000000 render_engine-2023.5.2a2/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2832 2023-05-18 14:36:26.000000 render_engine-2023.5.2a2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-05-18 14:36:26.000000 render_engine-2023.5.2a2/.readthedocs.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 14:36:44.668371 render_engine-2023.5.2a2/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-05-18 14:36:26.000000 render_engine-2023.5.2a2/.vscode/tasks.json
+-rw-r--r--   0 runner    (1001) docker     (123)      437 2023-05-18 14:36:26.000000 render_engine-2023.5.2a2/Contributing.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2475 2023-05-18 14:36:44.676370 render_engine-2023.5.2a2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2085 2023-05-18 14:36:26.000000 render_engine-2023.5.2a2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)    12647 2023-05-18 14:36:26.000000 render_engine-2023.5.2a2/changelog.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 14:36:44.668371 render_engine-2023.5.2a2/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 14:36:44.668371 render_engine-2023.5.2a2/docs/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      920 2023-05-18 14:36:26.000000 render_engine-2023.5.2a2/docs/docs/archive.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 14:36:44.668371 render_engine-2023.5.2a2/docs/docs/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)   273561 2023-05-18 14:36:26.000000 render_engine-2023.5.2a2/docs/docs/assets/create-app-help.png
+-rw-r--r--   0 runner    (1001) docker     (123)   288201 2023-05-18 14:36:26.000000 render_engine-2023.5.2a2/docs/docs/assets/render-engine-init-help.png
+-rw-r--r--   0 runner    (1001) docker     (123)    90538 2023-05-18 14:36:26.000000 render_engine-2023.5.2a2/docs/docs/assets/render-engine-init.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2713 2023-05-18 14:36:26.000000 render_engine-2023.5.2a2/docs/docs/cli.md
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-18 14:36:26.000000 render_engine-2023.5.2a2/docs/docs/collection.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 14:36:44.668371 render_engine-2023.5.2a2/docs/docs/contributing/
+-rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-05-18 14:36:26.000000 render_engine-2023.5.2a2/docs/docs/contributing/pages.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3023 2023-05-18 14:36:26.000000 render_engine-2023.5.2a2/docs/docs/custom_collections.md
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-18 14:36:26.000000 render_engine-2023.5.2a2/docs/docs/feeds.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 14:36:44.668371 render_engine-2023.5.2a2/docs/docs/getting-started/
+-rw-r--r--   0 runner    (1001) docker     (123)      692 2023-05-18 14:36:26.000000 render_engine-2023.5.2a2/docs/docs/getting-started/building-your-site.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1777 2023-05-18 14:36:26.000000 render_engine-2023.5.2a2/docs/docs/getting-started/creating-a-collection.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2460 2023-05-18 14:36:26.000000 render_engine-2023.5.2a2/docs/docs/getting-started/creating-a-page.md
+-rw-r--r--   0 runner    (1001) docker     (123)      453 2023-05-18 14:36:26.000000 render_engine-2023.5.2a2/docs/docs/getting-started/creating-your-app.md
+-rw-r--r--   0 runner    (1001) docker     (123)      727 2023-05-18 14:36:26.000000 render_engine-2023.5.2a2/docs/docs/getting-started/installation.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4598 2023-05-18 14:36:26.000000 render_engine-2023.5.2a2/docs/docs/getting-started/layout.md
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-18 14:36:26.000000 render_engine-2023.5.2a2/docs/docs/hookspecs.md
+-rw-r--r--   0 runner    (1001) docker     (123)      906 2023-05-18 14:36:26.000000 render_engine-2023.5.2a2/docs/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)      679 2023-05-18 14:36:26.000000 render_engine-2023.5.2a2/docs/docs/page.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3041 2023-05-18 14:36:26.000000 render_engine-2023.5.2a2/docs/docs/parsers.md
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-18 14:36:26.000000 render_engine-2023.5.2a2/docs/docs/plugins.md
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-18 14:36:26.000000 render_engine-2023.5.2a2/docs/docs/site.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2866 2023-05-18 14:36:26.000000 render_engine-2023.5.2a2/docs/docs/templates.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-05-18 14:36:26.000000 render_engine-2023.5.2a2/docs/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-18 14:36:26.000000 render_engine-2023.5.2a2/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1436 2023-05-18 14:36:26.000000 render_engine-2023.5.2a2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-05-18 14:36:26.000000 render_engine-2023.5.2a2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-18 14:36:44.676370 render_engine-2023.5.2a2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 14:36:44.668371 render_engine-2023.5.2a2/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     6148 2023-05-18 14:36:26.000000 render_engine-2023.5.2a2/src/.DS_Store
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 14:36:44.672371 render_engine-2023.5.2a2/src/render_engine/
+-rw-r--r--   0 runner    (1001) docker     (123)     6148 2023-05-18 14:36:26.000000 render_engine-2023.5.2a2/src/render_engine/.DS_Store
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-18 14:36:26.000000 render_engine-2023.5.2a2/src/render_engine/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-18 14:36:26.000000 render_engine-2023.5.2a2/src/render_engine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-05-18 14:36:26.000000 render_engine-2023.5.2a2/src/render_engine/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1953 2023-05-18 14:36:26.000000 render_engine-2023.5.2a2/src/render_engine/_base_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1378 2023-05-18 14:36:26.000000 render_engine-2023.5.2a2/src/render_engine/archive.py
+-rw-r--r--   0 runner    (1001) docker     (123)      688 2023-05-18 14:36:26.000000 render_engine-2023.5.2a2/src/render_engine/blog.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10320 2023-05-18 14:36:26.000000 render_engine-2023.5.2a2/src/render_engine/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6271 2023-05-18 14:36:26.000000 render_engine-2023.5.2a2/src/render_engine/collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2025 2023-05-18 14:36:26.000000 render_engine-2023.5.2a2/src/render_engine/engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)      907 2023-05-18 14:36:26.000000 render_engine-2023.5.2a2/src/render_engine/feeds.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-05-18 14:36:26.000000 render_engine-2023.5.2a2/src/render_engine/hookspecs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1914 2023-05-18 14:36:26.000000 render_engine-2023.5.2a2/src/render_engine/links.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5826 2023-05-18 14:36:26.000000 render_engine-2023.5.2a2/src/render_engine/page.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 14:36:44.672371 render_engine-2023.5.2a2/src/render_engine/parsers/
+-rw-r--r--   0 runner    (1001) docker     (123)     6148 2023-05-18 14:36:26.000000 render_engine-2023.5.2a2/src/render_engine/parsers/.DS_Store
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-05-18 14:36:26.000000 render_engine-2023.5.2a2/src/render_engine/parsers/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      681 2023-05-18 14:36:26.000000 render_engine-2023.5.2a2/src/render_engine/parsers/README_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-18 14:36:26.000000 render_engine-2023.5.2a2/src/render_engine/parsers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1729 2023-05-18 14:36:26.000000 render_engine-2023.5.2a2/src/render_engine/parsers/base_parsers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 14:36:44.672371 render_engine-2023.5.2a2/src/render_engine/parsers/markdown/
+-rw-r--r--   0 runner    (1001) docker     (123)      982 2023-05-18 14:36:26.000000 render_engine-2023.5.2a2/src/render_engine/parsers/markdown/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-05-18 14:36:26.000000 render_engine-2023.5.2a2/src/render_engine/parsers/markdown/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-05-18 14:36:26.000000 render_engine-2023.5.2a2/src/render_engine/plugins.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 14:36:44.676370 render_engine-2023.5.2a2/src/render_engine/render_engine_templates/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 14:36:26.000000 render_engine-2023.5.2a2/src/render_engine/render_engine_templates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      448 2023-05-18 14:36:26.000000 render_engine-2023.5.2a2/src/render_engine/render_engine_templates/base.html
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-05-18 14:36:26.000000 render_engine-2023.5.2a2/src/render_engine/render_engine_templates/base_collection_path.md
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-18 14:36:26.000000 render_engine-2023.5.2a2/src/render_engine/render_engine_templates/content.html
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-05-18 14:36:26.000000 render_engine-2023.5.2a2/src/render_engine/render_engine_templates/create_app_py.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-05-18 14:36:26.000000 render_engine-2023.5.2a2/src/render_engine/render_engine_templates/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1786 2023-05-18 14:36:26.000000 render_engine-2023.5.2a2/src/render_engine/render_engine_templates/rss2.0.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-05-18 14:36:26.000000 render_engine-2023.5.2a2/src/render_engine/render_engine_templates/rss2.0_items.xml
+-rwxr-xr-x   0 runner    (1001) docker     (123)      180 2023-05-18 14:36:26.000000 render_engine-2023.5.2a2/src/render_engine/render_engine_templates/sitemap.xml
+-rwxr-xr-x   0 runner    (1001) docker     (123)      283 2023-05-18 14:36:26.000000 render_engine-2023.5.2a2/src/render_engine/render_engine_templates/sitemap_item.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     7549 2023-05-18 14:36:26.000000 render_engine-2023.5.2a2/src/render_engine/site.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 14:36:44.672371 render_engine-2023.5.2a2/src/render_engine.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2475 2023-05-18 14:36:44.000000 render_engine-2023.5.2a2/src/render_engine.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3191 2023-05-18 14:36:44.000000 render_engine-2023.5.2a2/src/render_engine.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 14:36:44.000000 render_engine-2023.5.2a2/src/render_engine.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-18 14:36:44.000000 render_engine-2023.5.2a2/src/render_engine.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-05-18 14:36:44.000000 render_engine-2023.5.2a2/src/render_engine.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-18 14:36:44.000000 render_engine-2023.5.2a2/src/render_engine.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 14:36:44.676370 render_engine-2023.5.2a2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      991 2023-05-18 14:36:26.000000 render_engine-2023.5.2a2/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      576 2023-05-18 14:36:26.000000 render_engine-2023.5.2a2/tests/create_app_check_file.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-05-18 14:36:26.000000 render_engine-2023.5.2a2/tests/create_app_check_file_no_site_vars.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 14:36:44.676370 render_engine-2023.5.2a2/tests/site_test/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 14:36:44.676370 render_engine-2023.5.2a2/tests/site_test/blog/
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-05-18 14:36:26.000000 render_engine-2023.5.2a2/tests/site_test/blog/test_blog_content.md
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-05-18 14:36:26.000000 render_engine-2023.5.2a2/tests/site_test/build.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 14:36:44.676370 render_engine-2023.5.2a2/tests/site_test/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-05-18 14:36:26.000000 render_engine-2023.5.2a2/tests/site_test/templates/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)      506 2023-05-18 14:36:26.000000 render_engine-2023.5.2a2/tests/test_archive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2109 2023-05-18 14:36:26.000000 render_engine-2023.5.2a2/tests/test_base_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1586 2023-05-18 14:36:26.000000 render_engine-2023.5.2a2/tests/test_base_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-05-18 14:36:26.000000 render_engine-2023.5.2a2/tests/test_blog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3948 2023-05-18 14:36:26.000000 render_engine-2023.5.2a2/tests/test_collections.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1775 2023-05-18 14:36:26.000000 render_engine-2023.5.2a2/tests/test_create_app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3308 2023-05-18 14:36:26.000000 render_engine-2023.5.2a2/tests/test_feeds.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1944 2023-05-18 14:36:26.000000 render_engine-2023.5.2a2/tests/test_page.py
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-05-18 14:36:26.000000 render_engine-2023.5.2a2/tests/test_parser_markdown_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8607 2023-05-18 14:36:26.000000 render_engine-2023.5.2a2/tests/test_site.py
```

### Comparing `render_engine-2023.5.2a1/.chglog/CHANGELOG.tpl.md` & `render_engine-2023.5.2a2/.chglog/CHANGELOG.tpl.md`

 * *Files identical despite different names*

### Comparing `render_engine-2023.5.2a1/.devcontainer/devcontainer.json` & `render_engine-2023.5.2a2/.devcontainer/devcontainer.json`

 * *Files identical despite different names*

### Comparing `render_engine-2023.5.2a1/.github/CODE_OF_CONDUCT.md` & `render_engine-2023.5.2a2/.github/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `render_engine-2023.5.2a1/.github/CONTRIBUTION.md` & `render_engine-2023.5.2a2/.github/CONTRIBUTION.md`

 * *Files identical despite different names*

### Comparing `render_engine-2023.5.2a1/.github/FUNDING.yml` & `render_engine-2023.5.2a2/.github/FUNDING.yml`

 * *Files identical despite different names*

### Comparing `render_engine-2023.5.2a1/.github/LICENSE` & `render_engine-2023.5.2a2/.github/LICENSE`

 * *Files identical despite different names*

### Comparing `render_engine-2023.5.2a1/.github/dependabot.yml` & `render_engine-2023.5.2a2/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `render_engine-2023.5.2a1/.github/workflows/publish.yml` & `render_engine-2023.5.2a2/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `render_engine-2023.5.2a1/.gitignore` & `render_engine-2023.5.2a2/.gitignore`

 * *Files identical despite different names*

### Comparing `render_engine-2023.5.2a1/PKG-INFO` & `render_engine-2023.5.2a2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: render_engine
-Version: 2023.5.2a1
+Version: 2023.5.2a2
 Summary: A Flexible Static Site Generator for Python
 Project-URL: homepage, https://github.com/kjaymiller/render_engine/
 Project-URL: repository, https://github.com/kjaymiller/render_engine/
 Project-URL: documentation, https://render-engine.readthedocs.io/en/latest/
 Description-Content-Type: text/markdown
 Provides-Extra: dev
```

### Comparing `render_engine-2023.5.2a1/README.md` & `render_engine-2023.5.2a2/README.md`

 * *Files identical despite different names*

### Comparing `render_engine-2023.5.2a1/changelog.md` & `render_engine-2023.5.2a2/changelog.md`

 * *Files identical despite different names*

### Comparing `render_engine-2023.5.2a1/docs/docs/archive.md` & `render_engine-2023.5.2a2/docs/docs/archive.md`

 * *Files identical despite different names*

### Comparing `render_engine-2023.5.2a1/docs/docs/assets/create-app-help.png` & `render_engine-2023.5.2a2/docs/docs/assets/create-app-help.png`

 * *Files identical despite different names*

### Comparing `render_engine-2023.5.2a1/docs/docs/assets/render-engine-init-help.png` & `render_engine-2023.5.2a2/docs/docs/assets/render-engine-init-help.png`

 * *Files identical despite different names*

### Comparing `render_engine-2023.5.2a1/docs/docs/assets/render-engine-init.png` & `render_engine-2023.5.2a2/docs/docs/assets/render-engine-init.png`

 * *Files identical despite different names*

### Comparing `render_engine-2023.5.2a1/docs/docs/cli.md` & `render_engine-2023.5.2a2/docs/docs/cli.md`

 * *Files identical despite different names*

### Comparing `render_engine-2023.5.2a1/docs/docs/contributing/pages.md` & `render_engine-2023.5.2a2/docs/docs/contributing/pages.md`

 * *Files identical despite different names*

### Comparing `render_engine-2023.5.2a1/docs/docs/custom_collections.md` & `render_engine-2023.5.2a2/docs/docs/custom_collections.md`

 * *Files identical despite different names*

### Comparing `render_engine-2023.5.2a1/docs/docs/getting-started/building-your-site.md` & `render_engine-2023.5.2a2/docs/docs/getting-started/building-your-site.md`

 * *Files identical despite different names*

### Comparing `render_engine-2023.5.2a1/docs/docs/getting-started/creating-a-collection.md` & `render_engine-2023.5.2a2/docs/docs/getting-started/creating-a-collection.md`

 * *Files identical despite different names*

### Comparing `render_engine-2023.5.2a1/docs/docs/getting-started/creating-a-page.md` & `render_engine-2023.5.2a2/docs/docs/getting-started/creating-a-page.md`

 * *Files identical despite different names*

### Comparing `render_engine-2023.5.2a1/docs/docs/getting-started/installation.md` & `render_engine-2023.5.2a2/docs/docs/getting-started/installation.md`

 * *Files identical despite different names*

### Comparing `render_engine-2023.5.2a1/docs/docs/getting-started/layout.md` & `render_engine-2023.5.2a2/docs/docs/getting-started/layout.md`

 * *Files identical despite different names*

### Comparing `render_engine-2023.5.2a1/docs/docs/index.md` & `render_engine-2023.5.2a2/docs/docs/index.md`

 * *Files identical despite different names*

### Comparing `render_engine-2023.5.2a1/docs/docs/page.md` & `render_engine-2023.5.2a2/docs/docs/page.md`

 * *Files identical despite different names*

### Comparing `render_engine-2023.5.2a1/docs/docs/parsers.md` & `render_engine-2023.5.2a2/docs/docs/parsers.md`

 * *Files identical despite different names*

### Comparing `render_engine-2023.5.2a1/docs/docs/templates.md` & `render_engine-2023.5.2a2/docs/docs/templates.md`

 * *Files identical despite different names*

### Comparing `render_engine-2023.5.2a1/docs/mkdocs.yml` & `render_engine-2023.5.2a2/docs/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `render_engine-2023.5.2a1/pyproject.toml` & `render_engine-2023.5.2a2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `render_engine-2023.5.2a1/requirements.txt` & `render_engine-2023.5.2a2/requirements.txt`

 * *Files 0% similar despite different names*

```diff
@@ -40,11 +40,11 @@
     # via render-engine (pyproject.toml)
 six==1.16.0
     # via python-dateutil
 smmap==5.0.0
     # via gitdb
 text-unidecode==1.3
     # via python-slugify
-typer==0.7.0
+typer==0.9.0
     # via
     #   dtyper
     #   render-engine (pyproject.toml)
```

### Comparing `render_engine-2023.5.2a1/src/.DS_Store` & `render_engine-2023.5.2a2/src/.DS_Store`

 * *Files identical despite different names*

### Comparing `render_engine-2023.5.2a1/src/render_engine/.DS_Store` & `render_engine-2023.5.2a2/src/render_engine/.DS_Store`

 * *Files identical despite different names*

### Comparing `render_engine-2023.5.2a1/src/render_engine/_base_object.py` & `render_engine-2023.5.2a2/src/render_engine/_base_object.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """Shared Properties and methods across render_engine objects."""
 
 from slugify import slugify
 
+
 class BaseObject:
     """
     Shared properties for render_engine objects.
 
     This ensures that the behavior around the title, slug, and path_name are consistent
 
     This is not intended to be used directly.
@@ -44,25 +45,30 @@
     @property
     def path_name(self) -> str:
         """
         Returns the [`url_for`][src.render_engine.page.Page.url_for] for the page including the first route.
         """
         return f"{self._slug}{self.extension}"
 
+    def url_for(self):
+        pass
+
+
     def to_dict(self):
         """
         Returns a dict of the page's attributes.
 
         This is often used to pass attributes into the page's `template`.
 
         """
         base_dict ={
             **vars(self),
             "title": self._title,
             "slug": self._slug,
+            "url": self.url_for(),
         }
 
         # Pull out template_vars
         if hasattr(self, "template_vars"):
             for key, value in self.template_vars.items():
                 base_dict[key] = value
```

### Comparing `render_engine-2023.5.2a1/src/render_engine/archive.py` & `render_engine-2023.5.2a2/src/render_engine/archive.py`

 * *Files identical despite different names*

### Comparing `render_engine-2023.5.2a1/src/render_engine/blog.py` & `render_engine-2023.5.2a2/src/render_engine/blog.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 from .feeds import RSSFeed
 from .page import Page
 from .parsers.markdown import MarkdownPageParser
 
 
 class BlogPost(Page):
     """Page Like object with slight modifications to work with BlogPosts."""
-    list_attrs = ["tags"]
     invalid_attrs = ["slug"]
 
 
 class Blog(Collection):
     """
     Custom :py:class:`collection.Collection` class with archiving enabled, sort by `date` by default.
```

### Comparing `render_engine-2023.5.2a1/src/render_engine/cli.py` & `render_engine-2023.5.2a2/src/render_engine/cli.py`

 * *Files identical despite different names*

### Comparing `render_engine-2023.5.2a1/src/render_engine/collection.py` & `render_engine-2023.5.2a2/src/render_engine/collection.py`

 * *Files identical despite different names*

### Comparing `render_engine-2023.5.2a1/src/render_engine/engine.py` & `render_engine-2023.5.2a2/src/render_engine/engine.py`

 * *Files identical despite different names*

### Comparing `render_engine-2023.5.2a1/src/render_engine/feeds.py` & `render_engine-2023.5.2a2/src/render_engine/feeds.py`

 * *Files identical despite different names*

### Comparing `render_engine-2023.5.2a1/src/render_engine/hookspecs.py` & `render_engine-2023.5.2a2/src/render_engine/hookspecs.py`

 * *Files identical despite different names*

### Comparing `render_engine-2023.5.2a1/src/render_engine/links.py` & `render_engine-2023.5.2a2/src/render_engine/links.py`

 * *Files identical despite different names*

### Comparing `render_engine-2023.5.2a1/src/render_engine/page.py` & `render_engine-2023.5.2a2/src/render_engine/page.py`

 * *Files identical despite different names*

### Comparing `render_engine-2023.5.2a1/src/render_engine/parsers/.DS_Store` & `render_engine-2023.5.2a2/src/render_engine/parsers/.DS_Store`

 * *Files identical despite different names*

### Comparing `render_engine-2023.5.2a1/src/render_engine/parsers/README_TEMPLATE.md` & `render_engine-2023.5.2a2/src/render_engine/parsers/README_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `render_engine-2023.5.2a1/src/render_engine/parsers/base_parsers.py` & `render_engine-2023.5.2a2/src/render_engine/parsers/base_parsers.py`

 * *Files identical despite different names*

### Comparing `render_engine-2023.5.2a1/src/render_engine/parsers/markdown/README.md` & `render_engine-2023.5.2a2/src/render_engine/parsers/markdown/README.md`

 * *Files identical despite different names*

### Comparing `render_engine-2023.5.2a1/src/render_engine/plugins.py` & `render_engine-2023.5.2a2/src/render_engine/plugins.py`

 * *Files identical despite different names*

### Comparing `render_engine-2023.5.2a1/src/render_engine/render_engine_templates/create_app_py.txt` & `render_engine-2023.5.2a2/src/render_engine/render_engine_templates/create_app_py.txt`

 * *Files identical despite different names*

### Comparing `render_engine-2023.5.2a1/src/render_engine/render_engine_templates/index.html` & `render_engine-2023.5.2a2/src/render_engine/render_engine_templates/index.html`

 * *Files identical despite different names*

### Comparing `render_engine-2023.5.2a1/src/render_engine/render_engine_templates/rss2.0.xml` & `render_engine-2023.5.2a2/src/render_engine/render_engine_templates/rss2.0.xml`

 * *Files identical despite different names*

### Comparing `render_engine-2023.5.2a1/src/render_engine/render_engine_templates/rss2.0_items.xml` & `render_engine-2023.5.2a2/src/render_engine/render_engine_templates/rss2.0_items.xml`

 * *Files identical despite different names*

### Comparing `render_engine-2023.5.2a1/src/render_engine/site.py` & `render_engine-2023.5.2a2/src/render_engine/site.py`

 * *Files identical despite different names*

### Comparing `render_engine-2023.5.2a1/src/render_engine.egg-info/PKG-INFO` & `render_engine-2023.5.2a2/src/render_engine.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: render-engine
-Version: 2023.5.2a1
+Version: 2023.5.2a2
 Summary: A Flexible Static Site Generator for Python
 Project-URL: homepage, https://github.com/kjaymiller/render_engine/
 Project-URL: repository, https://github.com/kjaymiller/render_engine/
 Project-URL: documentation, https://render-engine.readthedocs.io/en/latest/
 Description-Content-Type: text/markdown
 Provides-Extra: dev
```

### Comparing `render_engine-2023.5.2a1/src/render_engine.egg-info/SOURCES.txt` & `render_engine-2023.5.2a2/src/render_engine.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `render_engine-2023.5.2a1/tests/conftest.py` & `render_engine-2023.5.2a2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `render_engine-2023.5.2a1/tests/create_app_check_file.txt` & `render_engine-2023.5.2a2/tests/create_app_check_file.txt`

 * *Files identical despite different names*

### Comparing `render_engine-2023.5.2a1/tests/test_base_object.py` & `render_engine-2023.5.2a2/tests/test_base_object.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from render_engine._base_object import BaseObject
 
+
 class TestObject(BaseObject):
     pass
     
 
 class TestBaseObjectProperties:
 
     test_object = TestObject()
@@ -43,20 +44,22 @@
         assert self.test_object.path_name == "testobject.html"
 
     def test_base_object_to_dict(self):
         """Tests that the to_dict method returns a dict of the object's attributes"""
         assert self.test_object.to_dict() == {
             "title": "TestObject",
             "slug": "testobject",
+            "url": None,
         }
 
     def test_base_object_to_dict_with_template_vars(self):
         """Tests that the `to_dict` adds template_vars extracted method returns a dict of the object's attributes"""
         self.test_object.template_vars = {"test": "test"}
 
         assert self.test_object.to_dict() == {
             "title": "TestObject",
             "slug": "testobject",
+            "url": None,
             "test": "test",
         }
 
         assert self.test_object.template_vars == {"test": "test"}
```

### Comparing `render_engine-2023.5.2a1/tests/test_base_parser.py` & `render_engine-2023.5.2a2/tests/test_base_parser.py`

 * *Files identical despite different names*

### Comparing `render_engine-2023.5.2a1/tests/test_collections.py` & `render_engine-2023.5.2a2/tests/test_collections.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,29 +6,28 @@
 from render_engine.collection import Collection
 from render_engine.page import Page
 from render_engine.parsers import BasePageParser
 
 pm = pluggy.PluginManager("fake_test")
 
 
-def test_collection_information_parser_passes_to_page():
+def test_collection_information_parser_passes_to_page(tmp_path):
     """
     Tests that information page parser is passed into the page
     """
 
     class SimpleBasePageParser(BasePageParser):
         pass
 
     class BasicCollection(Collection):
         PageParser = SimpleBasePageParser
         content_type = Page
 
     collection = BasicCollection()
     page = collection.get_page()
-
     assert page.Parser == SimpleBasePageParser
 
 
 def test_pages_generate_from_collection_content_path(tmp_path: pathlib.Path):
     """
     Tests that pages are generated from a collection
     """
@@ -130,17 +129,17 @@
 
 
 @pytest.mark.parametrize(
         "attr,attrval",
         [
             ("template", "test.html"),
             ("routes", ["/test/long/route"]),
-        ]
+        ],
 )
-def test_collection_attrs_pass_to_page(attr: str, attrval: str | list[str]):
+def test_collection_attrs_pass_to_page(tmp_path, attr: str, attrval: str | list[str]):
     """Tests that the template attribute for the collection is passed to the page"""
 
     class SimpleBasePageParser(BasePageParser):
         pass
 
     class BasicCollection(Collection):
         PageParser = SimpleBasePageParser
```

### Comparing `render_engine-2023.5.2a1/tests/test_create_app.py` & `render_engine-2023.5.2a2/tests/test_create_app.py`

 * *Files identical despite different names*

### Comparing `render_engine-2023.5.2a1/tests/test_feeds.py` & `render_engine-2023.5.2a2/tests/test_feeds.py`

 * *Files identical despite different names*

### Comparing `render_engine-2023.5.2a1/tests/test_page.py` & `render_engine-2023.5.2a2/tests/test_page.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,11 @@
+import pathlib
+
 import jinja2
 import pytest
-import pathlib
 
 from render_engine import Page
 
 
 @pytest.fixture
 def page_from_file(tmp_path: pathlib.Path):
     d = tmp_path / "test_page.md"
@@ -16,23 +17,23 @@
 # Test Page
 This is a test page
 """
 
     d.write_text(content)
     return Page(content_path=d)
 
-def test_page_attrs_from_file(page_from_file):
+def test_page_attrs_from_file(page_from_file: Page):
     """
     Tests that expected page attrsibutes are set from the file.
     Currently this is handled by the BasePageParser and the logic in the Page.
     """
     assert page_from_file._title == "Test Page"
 
 
-def test_page_custom_attrs_from_file(page_from_file):
+def test_page_custom_attrs_from_file(page_from_file: Page):
     """Tests that unique page attrsibutes are set from the file"""
     assert page_from_file.custom == "test"
 
 
 def test_page_from_template(tmp_path: pathlib.Path):
     """Tests that page attributes are set from a template"""
 
@@ -45,17 +46,31 @@
         loader=jinja2.DictLoader({"test.html": "{{ title }}"})
     )
 
     page = CustomPage()
     assert page._render_content(engine=environment) == "Test Page"
 
 
-
 def test_page_content_renders_jinja():
     """Tests that page content is rendered with jinja"""
 
     class CustomPage(Page):
         content = "Test Page"
 
     page = CustomPage()
     assert page.content == "Test Page"
-    assert page._content == "Test Page"
+    assert page._content == "Test Page"
+
+
+def test_rendered_page_from_template_has_attributes():
+    """Tests that selected page attributes are available in a template"""
+    template = "{{title}}-{{slug}}-{{url}}"
+
+    environment = jinja2.Environment(
+        loader=jinja2.DictLoader({"test.html": template})
+    )
+
+    class CustomPage(Page):
+        template = environment.get_template("test.html")
+
+    
+    assert CustomPage()._render_from_template(template=CustomPage.template) == "CustomPage-custompage-/custompage.html"
```

### Comparing `render_engine-2023.5.2a1/tests/test_site.py` & `render_engine-2023.5.2a2/tests/test_site.py`

 * *Files identical despite different names*

