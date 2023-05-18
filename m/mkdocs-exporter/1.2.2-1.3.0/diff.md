# Comparing `tmp/mkdocs_exporter-1.2.2.tar.gz` & `tmp/mkdocs_exporter-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mkdocs_exporter-1.2.2.tar", max compression
+gzip compressed data, was "mkdocs_exporter-1.3.0.tar", max compression
```

## Comparing `mkdocs_exporter-1.2.2.tar` & `mkdocs_exporter-1.3.0.tar`

### file list

```diff
@@ -1,23 +1,25 @@
--rw-r--r--   0        0        0     1071 2023-05-09 09:23:22.592488 mkdocs_exporter-1.2.2/LICENSE
--rw-r--r--   0        0        0     3066 2023-05-10 11:42:02.282235 mkdocs_exporter-1.2.2/README.md
--rw-r--r--   0        0        0        0 2023-05-09 09:23:22.592488 mkdocs_exporter-1.2.2/mkdocs_exporter/__init__.py
--rw-r--r--   0        0        0     1899 2023-05-09 15:43:28.836677 mkdocs_exporter-1.2.2/mkdocs_exporter/browser.py
--rw-r--r--   0        0        0       96 2023-05-09 09:23:22.592488 mkdocs_exporter-1.2.2/mkdocs_exporter/logging.py
--rw-r--r--   0        0        0      440 2023-05-09 09:23:22.592488 mkdocs_exporter-1.2.2/mkdocs_exporter/page.py
--rw-r--r--   0        0        0      705 2023-05-09 17:06:53.963165 mkdocs_exporter-1.2.2/mkdocs_exporter/plugin.py
--rw-r--r--   0        0        0        0 2023-05-09 09:23:22.592488 mkdocs_exporter-1.2.2/mkdocs_exporter/plugins/__init__.py
--rw-r--r--   0        0        0        0 2023-05-09 09:23:22.592488 mkdocs_exporter-1.2.2/mkdocs_exporter/plugins/extras/__init__.py
--rw-r--r--   0        0        0      977 2023-05-09 09:28:39.475500 mkdocs_exporter-1.2.2/mkdocs_exporter/plugins/extras/config.py
--rw-r--r--   0        0        0      812 2023-05-09 11:28:30.480215 mkdocs_exporter-1.2.2/mkdocs_exporter/plugins/extras/plugin.py
--rw-r--r--   0        0        0        0 2023-05-09 09:23:22.592488 mkdocs_exporter-1.2.2/mkdocs_exporter/plugins/pdf/__init__.py
--rw-r--r--   0        0        0      731 2023-05-09 09:23:22.592488 mkdocs_exporter-1.2.2/mkdocs_exporter/plugins/pdf/button.py
--rw-r--r--   0        0        0     1120 2023-05-12 06:29:50.585343 mkdocs_exporter-1.2.2/mkdocs_exporter/plugins/pdf/config.py
--rw-r--r--   0        0        0     4477 2023-05-16 11:51:18.093013 mkdocs_exporter-1.2.2/mkdocs_exporter/plugins/pdf/plugin.py
--rw-r--r--   0        0        0     2330 2023-05-09 10:49:37.916810 mkdocs_exporter-1.2.2/mkdocs_exporter/plugins/pdf/renderer.py
--rw-r--r--   0        0        0     4080 2023-05-10 11:42:02.282235 mkdocs_exporter-1.2.2/mkdocs_exporter/preprocessor.py
--rw-r--r--   0        0        0      241 2023-05-09 09:23:22.592488 mkdocs_exporter-1.2.2/mkdocs_exporter/renderer.py
--rw-r--r--   0        0        0        0 2023-05-09 09:23:22.592488 mkdocs_exporter-1.2.2/mkdocs_exporter/resources/__init__.py
--rw-r--r--   0        0        0        0 2023-05-09 09:23:22.592488 mkdocs_exporter-1.2.2/mkdocs_exporter/resources/js/__init__.py
--rw-r--r--   0        0        0   499714 2023-05-09 09:23:22.592488 mkdocs_exporter-1.2.2/mkdocs_exporter/resources/js/pagedjs.min.js
--rw-r--r--   0        0        0     1525 2023-05-16 11:51:18.093013 mkdocs_exporter-1.2.2/pyproject.toml
--rw-r--r--   0        0        0     4426 1970-01-01 00:00:00.000000 mkdocs_exporter-1.2.2/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-05-08 13:15:16.904792 mkdocs_exporter-1.3.0/LICENSE
+-rw-r--r--   0        0        0     3246 2023-05-18 17:31:28.191563 mkdocs_exporter-1.3.0/README.md
+-rw-r--r--   0        0        0        0 2023-05-08 15:45:32.453553 mkdocs_exporter-1.3.0/mkdocs_exporter/__init__.py
+-rw-r--r--   0        0        0     1899 2023-05-09 17:07:37.227188 mkdocs_exporter-1.3.0/mkdocs_exporter/browser.py
+-rw-r--r--   0        0        0       96 2023-05-08 19:25:05.801769 mkdocs_exporter-1.3.0/mkdocs_exporter/logging.py
+-rw-r--r--   0        0        0      440 2023-05-08 15:32:49.823552 mkdocs_exporter-1.3.0/mkdocs_exporter/page.py
+-rw-r--r--   0        0        0      705 2023-05-18 15:00:47.504058 mkdocs_exporter-1.3.0/mkdocs_exporter/plugin.py
+-rw-r--r--   0        0        0        0 2023-05-06 21:44:34.488343 mkdocs_exporter-1.3.0/mkdocs_exporter/plugins/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-07 17:00:48.574613 mkdocs_exporter-1.3.0/mkdocs_exporter/plugins/extras/__init__.py
+-rw-r--r--   0        0        0     1052 2023-05-18 17:25:44.201656 mkdocs_exporter-1.3.0/mkdocs_exporter/plugins/extras/config.py
+-rw-r--r--   0        0        0      685 2023-05-18 17:25:44.201656 mkdocs_exporter-1.3.0/mkdocs_exporter/plugins/extras/icon.py
+-rw-r--r--   0        0        0      870 2023-05-18 17:25:44.201656 mkdocs_exporter-1.3.0/mkdocs_exporter/plugins/extras/plugin.py
+-rw-r--r--   0        0        0      855 2023-05-18 17:25:44.201656 mkdocs_exporter-1.3.0/mkdocs_exporter/plugins/extras/preprocessor.py
+-rw-r--r--   0        0        0        0 2023-05-07 17:48:51.834620 mkdocs_exporter-1.3.0/mkdocs_exporter/plugins/pdf/__init__.py
+-rw-r--r--   0        0        0      526 2023-05-18 17:25:44.201656 mkdocs_exporter-1.3.0/mkdocs_exporter/plugins/pdf/button.py
+-rw-r--r--   0        0        0     1120 2023-05-18 16:23:49.312684 mkdocs_exporter-1.3.0/mkdocs_exporter/plugins/pdf/config.py
+-rw-r--r--   0        0        0     4612 2023-05-18 17:25:44.201656 mkdocs_exporter-1.3.0/mkdocs_exporter/plugins/pdf/plugin.py
+-rw-r--r--   0        0        0     2330 2023-05-09 11:31:09.967140 mkdocs_exporter-1.3.0/mkdocs_exporter/plugins/pdf/renderer.py
+-rw-r--r--   0        0        0     3560 2023-05-18 17:25:44.201656 mkdocs_exporter-1.3.0/mkdocs_exporter/preprocessor.py
+-rw-r--r--   0        0        0      241 2023-05-07 12:23:00.605366 mkdocs_exporter-1.3.0/mkdocs_exporter/renderer.py
+-rw-r--r--   0        0        0        0 2023-05-08 14:16:51.163540 mkdocs_exporter-1.3.0/mkdocs_exporter/resources/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-08 14:16:39.063540 mkdocs_exporter-1.3.0/mkdocs_exporter/resources/js/__init__.py
+-rw-r--r--   0        0        0   499714 2023-05-08 14:10:56.413538 mkdocs_exporter-1.3.0/mkdocs_exporter/resources/js/pagedjs.min.js
+-rw-r--r--   0        0        0     1563 2023-05-18 17:25:51.841654 mkdocs_exporter-1.3.0/pyproject.toml
+-rw-r--r--   0        0        0     4665 1970-01-01 00:00:00.000000 mkdocs_exporter-1.3.0/PKG-INFO
```

### Comparing `mkdocs_exporter-1.2.2/LICENSE` & `mkdocs_exporter-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mkdocs_exporter-1.2.2/README.md` & `mkdocs_exporter-1.3.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,27 +1,31 @@
 # MkDocs Exporter
 
 A highly-configurable plugin for [*MkDocs*](https://github.com/mkdocs/mkdocs) that exports your pages to PDF files.
 
+- [Documentation][https://adrienbrignon.github.io/mkdocs-exporter]
+- [PyPI](https://pypi.org/project/mkdocs-exporter)
+
 ## Features
 
 - 🚀 **Fast** - PDF documents are generated concurrently!
+- 🎨 **Customizable** - full control over the resulting documents
+  - Compatible with [`mkdocs-material`](https://github.com/squidfunk/mkdocs-material)
+  - Cover pages (supports [`macros`](https://github.com/fralau/mkdocs_macros_plugin) plugin)
+  - Define custom scripts and stylesheets to customize your PDF documents
+  - Define "buttons" at the top of your documentation pages ([example](https://adrienbrignon.github.io/mkdocs-exporter/setup/setting-up-buttons/))
 - ⭐ **Powerful** - it uses a headless browser and some awesome libraries under the hood to generate PDF files
+  - [*Playwright*](https://github.com/microsoft/playwright-python) to automate browsers
   - [*Paged.js*](https://github.com/pagedjs/pagedjs) polyfills are included by default ([Paged Media](https://www.w3.org/TR/css-page-3/) and [Generated Content](https://www.w3.org/TR/css-gcpm-3/) CSS modules)
   - [*Sass*](https://sass-lang.com/) support (via [`libsass`](https://github.com/sass/libsass-python)) for your stylesheets
-- 🎨 **Customizable** - full control over the resulting documents
-  - Built for and compatible with [`mkdocs-material`](https://github.com/squidfunk/mkdocs-material)
-  - Cover pages with templating support (for instance, with the [`macros`](https://github.com/fralau/mkdocs_macros_plugin) plugin)
-  - Define custom scripts and stylesheets to customize your PDF documents
-  - Define "buttons" at the top of your documentation pages
 
 ## Prerequisites
 
 - Python `>= 3.7`
-- MkDocs `>= 1.1`
+- MkDocs `>= 1.4`
 
 ## Installation
 
 The plugin is hosted on [*PyPI*](https://pypi.org/project/mkdocs-exporter/) and can be installed via `pip` (or your favourite package manager):
 
 ```bash
 pip install mkdocs-exporter
@@ -59,15 +63,14 @@
 ```
 
 Check out a [sample PDF generated by this plugin](examples/example.pdf) from the default page of the [Material for MkDocs](https://squidfunk.github.io/mkdocs-material) theme.  
 It has been built with some custom CSS and features cover pages.
 
 ## Roadmap
 
-- Documentation (based on `MkDocs` and featuring this plugin)
 - Ensure full compatibility with other themes than `mkdocs-material`
 - Combine all pages as one PDF
 
 Feel free to request additional features by submitting an issue or by contributing through a pull request.
 
 ## License
```

### Comparing `mkdocs_exporter-1.2.2/mkdocs_exporter/browser.py` & `mkdocs_exporter-1.3.0/mkdocs_exporter/browser.py`

 * *Files identical despite different names*

### Comparing `mkdocs_exporter-1.2.2/mkdocs_exporter/plugin.py` & `mkdocs_exporter-1.3.0/mkdocs_exporter/plugin.py`

 * *Files identical despite different names*

### Comparing `mkdocs_exporter-1.2.2/mkdocs_exporter/plugins/extras/config.py` & `mkdocs_exporter-1.3.0/mkdocs_exporter/plugins/extras/config.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,14 +5,17 @@
 
 class ButtonConfig(BaseConfig):
   """The configuration of a button."""
 
   enabled = c.Type((bool, Callable), default=True)
   """Is the button enabled?"""
 
+  id = c.Optional(c.Type(str, Callable))
+  """The button's identifier."""
+
   title = c.Type((str, Callable))
   """The button's title."""
 
   icon = c.Type((str, Callable))
   """The button's icon (typically, an SVG element)."""
 
   href = c.Type((str, Callable))
```

### Comparing `mkdocs_exporter-1.2.2/mkdocs_exporter/plugins/extras/plugin.py` & `mkdocs_exporter-1.3.0/mkdocs_exporter/plugins/extras/plugin.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,31 +1,28 @@
 from typing import Optional
 from mkdocs.plugins import BasePlugin
 from mkdocs_exporter.page import Page
 from mkdocs.plugins import event_priority
-from mkdocs_exporter.preprocessor import Preprocessor
 from mkdocs_exporter.plugins.extras.config import Config
+from mkdocs_exporter.plugins.extras.preprocessor import Preprocessor
 
 
 class Plugin(BasePlugin[Config]):
   """The plugin."""
 
 
   @event_priority(-85)
   def on_post_page(self, html: str, page: Page, **kwargs) -> Optional[str]:
     """Invoked after a page has been built."""
 
     def resolve(value):
-      if callable(value):
-        return value(page)
-
-      return value
+      return value(page) if callable(value) else value
 
     preprocessor = Preprocessor()
 
     preprocessor.preprocess(html)
 
-    for button in self.config.buttons:
-      if resolve(button['enabled']):
+    for button in [*self.config.buttons, *page.meta.get('buttons', [])]:
+      if 'enabled' not in button or resolve(button['enabled']):
         preprocessor.button(**{k: resolve(v) for k, v in button.items()})
 
     return preprocessor.done()
```

### Comparing `mkdocs_exporter-1.2.2/mkdocs_exporter/plugins/pdf/config.py` & `mkdocs_exporter-1.3.0/mkdocs_exporter/plugins/pdf/config.py`

 * *Files identical despite different names*

### Comparing `mkdocs_exporter-1.2.2/mkdocs_exporter/plugins/pdf/plugin.py` & `mkdocs_exporter-1.3.0/mkdocs_exporter/plugins/pdf/plugin.py`

 * *Files 3% similar despite different names*

```diff
@@ -80,19 +80,21 @@
     for script in self.config.scripts:
       self.renderer.add_script(script)
 
 
   def on_pre_page(self, page: Page, config: dict, **kwargs):
     """Invoked before building the page."""
 
+    if not hasattr(page, 'html'):
+      raise Exception('Missing `mkdocs/exporter` plugin or your plugins are not ordered properly!')
     if not self._enabled():
       return
 
     directory = os.path.dirname(page.file.abs_dest_path)
-    filename = os.path.splitext(os.path.basename(page.file.abs_src_path))[0] + '.pdf'
+    filename = os.path.splitext(os.path.basename(page.file.abs_dest_path))[0] + '.pdf'
     fullpath = os.path.join(directory, filename)
 
     page.formats['pdf'] = os.path.relpath(fullpath, config['site_dir'])
 
 
   @event_priority(-75)
   def on_post_page(self, html: str, page: Page, config: dict) -> Optional[str]:
```

### Comparing `mkdocs_exporter-1.2.2/mkdocs_exporter/plugins/pdf/renderer.py` & `mkdocs_exporter-1.3.0/mkdocs_exporter/plugins/pdf/renderer.py`

 * *Files identical despite different names*

### Comparing `mkdocs_exporter-1.2.2/mkdocs_exporter/preprocessor.py` & `mkdocs_exporter-1.3.0/mkdocs_exporter/preprocessor.py`

 * *Files 8% similar despite different names*

```diff
@@ -22,31 +22,14 @@
     """Gives the preprocessor some HTML to work on."""
 
     self.html = BeautifulSoup(html, 'lxml') if isinstance(html, str) else None
 
     return self
 
 
-  def button(self, title: str, href: str, icon: str, **kwargs) -> Preprocessor:
-    """Adds a button at the top of the page."""
-
-    tags = self.html.find('nav', {'class': 'md-tags'})
-    button = self.html.new_tag('a', title=title, href=href, **kwargs, attrs={'class': 'md-content__button md-icon'})
-    svg = BeautifulSoup(icon, 'lxml')
-
-    button.append(svg)
-
-    if tags:
-      tags.insert_after(button)
-    else:
-      self.html.find('article', {'class': 'md-content__inner'}).insert(0, button)
-
-    return self
-
-
   def teleport(self) -> Preprocessor:
     """Teleport elements to their destination."""
 
     for element in self.html.select('*[data-teleport]'):
       selector = element.attrs['data-teleport']
       destination = self.html.select_one(selector)
       tag = Tag(None, name=element.name, attrs=element.attrs)
```

### Comparing `mkdocs_exporter-1.2.2/mkdocs_exporter/resources/js/pagedjs.min.js` & `mkdocs_exporter-1.3.0/mkdocs_exporter/resources/js/pagedjs.min.js`

 * *Files identical despite different names*

### Comparing `mkdocs_exporter-1.2.2/pyproject.toml` & `mkdocs_exporter-1.3.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "mkdocs-exporter"
-version = "1.2.2"
+version = "1.3.0"
 repository = "https://github.com/adrienbrignon/mkdocs-exporter"
 keywords = ["mkdocs", "pdf", "exporter"]
 description = "A highly-configurable plugin for MkDocs that exports your pages to PDF files."
 authors = ["Adrien Brignon <adrien@brignon.dev>"]
 readme = "README.md"
 classifiers = [
   "License :: OSI Approved :: MIT License",
@@ -24,14 +24,15 @@
 mkdocs = ">=1.4"
 playwright = ">=1.33"
 beautifulsoup4 = ">=4.12.2"
 lxml = ">=4.9"
 libsass = ">=0.22.0"
 importlib-resources = ">=5.0"
 importlib-metadata = "<5.0"
+mkdocs-material-extensions = "^1.1.1"
 
 [tool.poetry.plugins."mkdocs.plugins"]
 "mkdocs/exporter" = "mkdocs_exporter.plugin:Plugin"
 "mkdocs/exporter/pdf" = "mkdocs_exporter.plugins.pdf.plugin:Plugin"
 "mkdocs/exporter/extras" = "mkdocs_exporter.plugins.extras.plugin:Plugin"
 
 [tool.poetry.urls]
```

### Comparing `mkdocs_exporter-1.2.2/PKG-INFO` & `mkdocs_exporter-1.3.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdocs-exporter
-Version: 1.2.2
+Version: 1.3.0
 Summary: A highly-configurable plugin for MkDocs that exports your pages to PDF files.
 Home-page: https://github.com/adrienbrignon/mkdocs-exporter
 Keywords: mkdocs,pdf,exporter
 Author: Adrien Brignon
 Author-email: adrien@brignon.dev
 Requires-Python: >=3.7
 Classifier: License :: OSI Approved :: MIT License
@@ -21,39 +21,44 @@
 Classifier: Topic :: Text Processing :: Markup :: HTML
 Requires-Dist: beautifulsoup4 (>=4.12.2)
 Requires-Dist: importlib-metadata (<5.0)
 Requires-Dist: importlib-resources (>=5.0)
 Requires-Dist: libsass (>=0.22.0)
 Requires-Dist: lxml (>=4.9)
 Requires-Dist: mkdocs (>=1.4)
+Requires-Dist: mkdocs-material-extensions (>=1.1.1,<2.0.0)
 Requires-Dist: playwright (>=1.33)
 Project-URL: Bug Tracker, https://github.com/adrienbrignon/mkdocs-exporter/issues
 Project-URL: Repository, https://github.com/adrienbrignon/mkdocs-exporter
 Description-Content-Type: text/markdown
 
 # MkDocs Exporter
 
 A highly-configurable plugin for [*MkDocs*](https://github.com/mkdocs/mkdocs) that exports your pages to PDF files.
 
+- [Documentation][https://adrienbrignon.github.io/mkdocs-exporter]
+- [PyPI](https://pypi.org/project/mkdocs-exporter)
+
 ## Features
 
 - 🚀 **Fast** - PDF documents are generated concurrently!
+- 🎨 **Customizable** - full control over the resulting documents
+  - Compatible with [`mkdocs-material`](https://github.com/squidfunk/mkdocs-material)
+  - Cover pages (supports [`macros`](https://github.com/fralau/mkdocs_macros_plugin) plugin)
+  - Define custom scripts and stylesheets to customize your PDF documents
+  - Define "buttons" at the top of your documentation pages ([example](https://adrienbrignon.github.io/mkdocs-exporter/setup/setting-up-buttons/))
 - ⭐ **Powerful** - it uses a headless browser and some awesome libraries under the hood to generate PDF files
+  - [*Playwright*](https://github.com/microsoft/playwright-python) to automate browsers
   - [*Paged.js*](https://github.com/pagedjs/pagedjs) polyfills are included by default ([Paged Media](https://www.w3.org/TR/css-page-3/) and [Generated Content](https://www.w3.org/TR/css-gcpm-3/) CSS modules)
   - [*Sass*](https://sass-lang.com/) support (via [`libsass`](https://github.com/sass/libsass-python)) for your stylesheets
-- 🎨 **Customizable** - full control over the resulting documents
-  - Built for and compatible with [`mkdocs-material`](https://github.com/squidfunk/mkdocs-material)
-  - Cover pages with templating support (for instance, with the [`macros`](https://github.com/fralau/mkdocs_macros_plugin) plugin)
-  - Define custom scripts and stylesheets to customize your PDF documents
-  - Define "buttons" at the top of your documentation pages
 
 ## Prerequisites
 
 - Python `>= 3.7`
-- MkDocs `>= 1.1`
+- MkDocs `>= 1.4`
 
 ## Installation
 
 The plugin is hosted on [*PyPI*](https://pypi.org/project/mkdocs-exporter/) and can be installed via `pip` (or your favourite package manager):
 
 ```bash
 pip install mkdocs-exporter
@@ -91,15 +96,14 @@
 ```
 
 Check out a [sample PDF generated by this plugin](examples/example.pdf) from the default page of the [Material for MkDocs](https://squidfunk.github.io/mkdocs-material) theme.  
 It has been built with some custom CSS and features cover pages.
 
 ## Roadmap
 
-- Documentation (based on `MkDocs` and featuring this plugin)
 - Ensure full compatibility with other themes than `mkdocs-material`
 - Combine all pages as one PDF
 
 Feel free to request additional features by submitting an issue or by contributing through a pull request.
 
 ## License
```

