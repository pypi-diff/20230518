# Comparing `tmp/appmode-0.8.0.tar.gz` & `tmp/appmode-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/appmode-0.8.0.tar", last modified: Tue Jun  9 08:19:09 2020, max compression
+gzip compressed data, was "appmode-0.9.0.tar", last modified: Thu May 18 14:21:18 2023, max compression
```

## Comparing `appmode-0.8.0.tar` & `appmode-0.9.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxr-x   0 ole       (1000) ole       (1000)        0 2020-06-09 08:19:09.000000 appmode-0.8.0/
-drwxrwxr-x   0 ole       (1000) ole       (1000)        0 2020-06-09 08:19:09.000000 appmode-0.8.0/appmode/
--rw-rw-r--   0 ole       (1000) ole       (1000)      331 2020-06-09 08:14:58.000000 appmode-0.8.0/appmode/__init__.py
--rw-rw-r--   0 ole       (1000) ole       (1000)      197 2019-07-25 20:26:57.000000 appmode-0.8.0/appmode/appmode_top.css
--rw-rw-r--   0 ole       (1000) ole       (1000)      862 2019-07-25 20:26:57.000000 appmode-0.8.0/appmode/appmode.html
-drwxrwxr-x   0 ole       (1000) ole       (1000)        0 2020-06-09 08:19:09.000000 appmode-0.8.0/appmode/static/
--rw-rw-r--   0 ole       (1000) ole       (1000)     7157 2020-06-06 12:15:12.000000 appmode-0.8.0/appmode/static/main.js
--rw-rw-r--   0 ole       (1000) ole       (1000)     2528 2019-07-25 20:26:57.000000 appmode-0.8.0/appmode/static/gears.svg
--rw-rw-r--   0 ole       (1000) ole       (1000)     6168 2020-06-06 12:18:33.000000 appmode-0.8.0/appmode/server_extension.py
--rw-rw-r--   0 ole       (1000) ole       (1000)      789 2019-07-25 20:26:57.000000 appmode-0.8.0/appmode/appmode_bottom.css
-drwxrwxr-x   0 ole       (1000) ole       (1000)        0 2020-06-09 08:19:09.000000 appmode-0.8.0/appmode.egg-info/
--rw-rw-r--   0 ole       (1000) ole       (1000)       12 2020-06-09 08:19:09.000000 appmode-0.8.0/appmode.egg-info/requires.txt
--rw-rw-r--   0 ole       (1000) ole       (1000)      364 2020-06-09 08:19:09.000000 appmode-0.8.0/appmode.egg-info/SOURCES.txt
--rw-rw-r--   0 ole       (1000) ole       (1000)        1 2020-06-09 08:19:09.000000 appmode-0.8.0/appmode.egg-info/dependency_links.txt
--rw-rw-r--   0 ole       (1000) ole       (1000)        8 2020-06-09 08:19:09.000000 appmode-0.8.0/appmode.egg-info/top_level.txt
--rw-rw-r--   0 ole       (1000) ole       (1000)      572 2020-06-09 08:19:09.000000 appmode-0.8.0/appmode.egg-info/PKG-INFO
--rw-rw-r--   0 ole       (1000) ole       (1000)     3462 2019-07-25 20:44:36.000000 appmode-0.8.0/README.md
--rw-rw-r--   0 ole       (1000) ole       (1000)     1086 2019-07-25 20:26:57.000000 appmode-0.8.0/LICENSE.txt
--rw-rw-r--   0 ole       (1000) ole       (1000)      180 2019-07-25 20:26:57.000000 appmode-0.8.0/MANIFEST.in
--rw-rw-r--   0 ole       (1000) ole       (1000)     1433 2019-07-25 20:26:57.000000 appmode-0.8.0/setup.py
--rw-rw-r--   0 ole       (1000) ole       (1000)      572 2020-06-09 08:19:09.000000 appmode-0.8.0/PKG-INFO
--rw-rw-r--   0 ole       (1000) ole       (1000)       38 2020-06-09 08:19:09.000000 appmode-0.8.0/setup.cfg
+drwxrwxr-x   0 ole       (1000) ole       (1000)        0 2023-05-18 14:21:18.633572 appmode-0.9.0/
+-rw-rw-r--   0 ole       (1000) ole       (1000)     1086 2023-05-18 11:58:38.000000 appmode-0.9.0/LICENSE.txt
+-rw-rw-r--   0 ole       (1000) ole       (1000)      180 2023-05-18 11:58:38.000000 appmode-0.9.0/MANIFEST.in
+-rw-rw-r--   0 ole       (1000) ole       (1000)      512 2023-05-18 14:21:18.633572 appmode-0.9.0/PKG-INFO
+-rw-rw-r--   0 ole       (1000) ole       (1000)     3819 2023-05-18 14:01:34.000000 appmode-0.9.0/README.md
+drwxrwxr-x   0 ole       (1000) ole       (1000)        0 2023-05-18 14:21:18.633572 appmode-0.9.0/appmode/
+-rw-rw-r--   0 ole       (1000) ole       (1000)      331 2023-05-18 14:19:59.000000 appmode-0.9.0/appmode/__init__.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)      862 2023-05-18 11:58:38.000000 appmode-0.9.0/appmode/appmode.html
+-rw-rw-r--   0 ole       (1000) ole       (1000)      789 2023-05-18 11:58:38.000000 appmode-0.9.0/appmode/appmode_bottom.css
+-rw-rw-r--   0 ole       (1000) ole       (1000)      197 2023-05-18 11:58:38.000000 appmode-0.9.0/appmode/appmode_top.css
+-rw-rw-r--   0 ole       (1000) ole       (1000)     7366 2023-05-18 12:09:02.000000 appmode-0.9.0/appmode/server_extension.py
+drwxrwxr-x   0 ole       (1000) ole       (1000)        0 2023-05-18 14:21:18.633572 appmode-0.9.0/appmode/static/
+-rw-rw-r--   0 ole       (1000) ole       (1000)     2528 2023-05-18 11:58:38.000000 appmode-0.9.0/appmode/static/gears.svg
+-rw-rw-r--   0 ole       (1000) ole       (1000)     7157 2023-05-18 11:58:38.000000 appmode-0.9.0/appmode/static/main.js
+drwxrwxr-x   0 ole       (1000) ole       (1000)        0 2023-05-18 14:21:18.633572 appmode-0.9.0/appmode.egg-info/
+-rw-rw-r--   0 ole       (1000) ole       (1000)      512 2023-05-18 14:21:18.000000 appmode-0.9.0/appmode.egg-info/PKG-INFO
+-rw-rw-r--   0 ole       (1000) ole       (1000)      364 2023-05-18 14:21:18.000000 appmode-0.9.0/appmode.egg-info/SOURCES.txt
+-rw-rw-r--   0 ole       (1000) ole       (1000)        1 2023-05-18 14:21:18.000000 appmode-0.9.0/appmode.egg-info/dependency_links.txt
+-rw-rw-r--   0 ole       (1000) ole       (1000)       12 2023-05-18 14:21:18.000000 appmode-0.9.0/appmode.egg-info/requires.txt
+-rw-rw-r--   0 ole       (1000) ole       (1000)        8 2023-05-18 14:21:18.000000 appmode-0.9.0/appmode.egg-info/top_level.txt
+-rw-rw-r--   0 ole       (1000) ole       (1000)       38 2023-05-18 14:21:18.633572 appmode-0.9.0/setup.cfg
+-rw-rw-r--   0 ole       (1000) ole       (1000)     1366 2023-05-18 11:58:38.000000 appmode-0.9.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `appmode-0.8.0/appmode/appmode.html` & `appmode-0.9.0/appmode/appmode.html`

 * *Files identical despite different names*

### Comparing `appmode-0.8.0/appmode/static/main.js` & `appmode-0.9.0/appmode/static/main.js`

 * *Files identical despite different names*

### Comparing `appmode-0.8.0/appmode/static/gears.svg` & `appmode-0.9.0/appmode/static/gears.svg`

 * *Files identical despite different names*

### Comparing `appmode-0.8.0/appmode/server_extension.py` & `appmode-0.9.0/appmode/server_extension.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,26 +1,41 @@
 # -*- coding: utf-8 -*-
 
 import os
+import inspect
 import itertools
 from notebook.utils import url_path_join
 from notebook.base.handlers import IPythonHandler, FilesRedirectHandler, path_regex
 import notebook.notebook.handlers as orig_handler
-from tornado import web, gen
+import notebook
+from tornado import web
 from traitlets.config import LoggingConfigurable
 from traitlets import Bool, Unicode
 
 
+async def await_if_awaitable(obj):
+    """Convert a non-awaitable object to a coroutine if needed,
+    and await if it was a coroutine.
+
+    Designed to be called on the result of calling a function,
+    when that function could be asynchronous or not.
+    """
+    if inspect.isawaitable(obj):
+        obj = await obj
+    return obj
+
+
 class Appmode(LoggingConfigurable):
     """Object containing server-side configuration settings for Appmode.
     Defined separately from the AppmodeHandler to avoid multiple inheritance.
     """
     trusted_path = Unicode('', help="Run only notebooks below this path in Appmode.", config=True)
     show_edit_button = Bool(True, help="Show Edit App button during Appmode.", config=True)
     show_other_buttons = Bool(True, help="Show other buttons, e.g. Logout, during Appmode.", config=True)
+    temp_dir = Unicode('', help="Create temporary Appmode notebooks in this directory.", config=True)
 
 #===============================================================================
 class AppmodeHandler(IPythonHandler):
     @property
     def trusted_path(self):
         return self.settings['appmode'].trusted_path
 
@@ -28,48 +43,50 @@
     def show_edit_button(self):
         return self.settings['appmode'].show_edit_button
 
     @property
     def show_other_buttons(self):
         return self.settings['appmode'].show_other_buttons
 
+    @property
+    def temp_dir(self):
+        return self.settings['appmode'].temp_dir
+
     #===========================================================================
     @web.authenticated
-    def get(self, path):
+    async def get(self, path):
         """get renders the notebook template if a name is given, or
         redirects to the '/files/' handler if the name is not given."""
-
         path = path.strip('/')
         self.log.info('Appmode get: %s', path)
 
         # Abort if the app path is not below configured trusted_path.
         if not path.startswith(self.trusted_path):
             self.log.warn('Appmode refused to launch %s outside trusted path %s.', path, self.trusted_path)
             raise web.HTTPError(401, 'Notebook is not within trusted Appmode path.')
 
         cm = self.contents_manager
-
         # will raise 404 on not found
         try:
-            model = cm.get(path, content=False)
+            model = await await_if_awaitable(cm.get(path, content=False))
         except web.HTTPError as e:
             if e.status_code == 404 and 'files' in path.split('/'):
                 # 404, but '/files/' in URL, let FilesRedirect take care of it
                 return FilesRedirectHandler.redirect_to_files(self, path)
             else:
                 raise
         if model['type'] != 'notebook':
             # not a notebook, redirect to files
             return FilesRedirectHandler.redirect_to_files(self, path)
 
         # fix back button navigation
         self.add_header("Cache-Control", "cache-control: private, max-age=0, no-cache, no-store")
 
         # gather template parameters
-        tmp_path = self.mk_tmp_copy(path)
+        tmp_path = await self.mk_tmp_copy(path)
         tmp_name = tmp_path.rsplit('/', 1)[-1]
         render_kwargs = {
             'notebook_path': tmp_path,
             'notebook_name': tmp_name,
             'kill_kernel': False,
             'mathjax_url': self.mathjax_url,
             'mathjax_config': self.mathjax_config,
@@ -83,70 +100,74 @@
                 render_kwargs[parameter] = getattr(orig_handler, parameter)
 
         # Ok let's roll ....
         self.write(self.render_template('appmode.html', **render_kwargs))
 
     #===========================================================================
     @web.authenticated
-    @gen.coroutine
-    def post(self, path):
+    async def post(self, path):
         assert self.get_body_arguments("appmode_action")[0] == "delete"
         path = path.strip('/')
         self.log.info('Appmode deleting: %s', path)
 
         # delete session, including the kernel
         sm = self.session_manager
-        if gen.is_coroutine_function(sm.get_session):
-            s = yield sm.get_session(path=path)
-        else:
-            s = sm.get_session(path=path)
-        if gen.is_coroutine_function(sm.delete_session):
-            yield sm.delete_session(session_id=s['id'])
-        else:
-            sm.delete_session(session_id=s['id'])
+
+        s = await await_if_awaitable(sm.get_session(path=path))
+        await await_if_awaitable(sm.delete_session(session_id=s['id']))
 
         # delete tmp copy
         cm = self.contents_manager
-        cm.delete(path)
-        self.finish()
+        await await_if_awaitable(cm.delete(path))
+        await self.finish()
 
     #===========================================================================
-    def mk_tmp_copy(self, path):
+    async def mk_tmp_copy(self, path):
         cm = self.contents_manager
-
         # find tmp_path
-        dirname = os.path.dirname(path)
+        dirname = self.temp_dir or os.path.dirname(path)
+        if dirname and not os.path.exists(dirname):
+            os.makedirs(dirname)
         fullbasename = os.path.basename(path)
         basename, ext = os.path.splitext(fullbasename)
+        if cm.allow_hidden:
+            basename = '.' + basename
         for i in itertools.count():
-            tmp_path = "%s/.%s-%i%s"%(dirname, basename, i, ext)
+            tmp_path = "%s/%s-%i%s"%(dirname, basename, i, ext)
             if not cm.exists(tmp_path):
                 break
 
         # create tmp copy - allows opening same notebook multiple times
         self.log.info("Appmode creating tmp copy: "+tmp_path)
-        cm.copy(path, tmp_path)
+        await await_if_awaitable(cm.copy(path, tmp_path))
+        return tmp_path
 
-        return(tmp_path)
 
 #===============================================================================
 def load_jupyter_server_extension(nbapp):
     tmpl_dir = os.path.dirname(__file__)
+    notebook_tmpl_dir = os.path.join(os.path.dirname(notebook.__file__), 'templates')
     # does not work, because init_webapp() happens before init_server_extensions()
-    #nbapp.extra_template_paths.append(tmpl_dir) # dows
+    # nbapp.extra_template_paths.append(tmpl_dir) # dows
+
+    # For jupyter server, the notebook templates are not available in the default search paths. This can be addressed
+    # by using --ServerApp.extra_template_paths='***site-packages***\notebook\templates', but this is messy.
+    # To emulate this instead insert the notebook template directory at the start of the searchpath
+    # These will be used last, so the notebook.html resolves, but the page.html is still from jupyter server templates
 
     # For configuration values that can be set server side
     appmode = Appmode(parent=nbapp)
     nbapp.web_app.settings['appmode'] = appmode
 
     # slight violation of Demeter's Law
     rootloader = nbapp.web_app.settings['jinja2_env'].loader
     for loader in getattr(rootloader, 'loaders', [rootloader]):
         if hasattr(loader, 'searchpath') and tmpl_dir not in loader.searchpath:
             loader.searchpath.append(tmpl_dir)
+            loader.searchpath.insert(0, notebook_tmpl_dir)
 
     web_app = nbapp.web_app
     host_pattern = '.*$'
     route_pattern = url_path_join(web_app.settings['base_url'], r'/apps%s' % path_regex)
     web_app.add_handlers(host_pattern, [(route_pattern, AppmodeHandler)])
 
     if appmode.trusted_path:
```

### Comparing `appmode-0.8.0/appmode/appmode_bottom.css` & `appmode-0.9.0/appmode/appmode_bottom.css`

 * *Files identical despite different names*

### Comparing `appmode-0.8.0/README.md` & `appmode-0.9.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -47,14 +47,21 @@
 
 ## Server Side Configuration
 
 Appmode adds the following [configuration options](https://jupyter-notebook.readthedocs.io/en/stable/config.html):
 - `Appmode.trusted_path` Run only notebooks below this path in Appmode. Default: No restrictions.
 - `Appmode.show_edit_button` Show _Edit App_ button during Appmode. Default: True.
 - `Appmode.show_other_buttons` Show other buttons, e.g. Logout, during Appmode. Default: True.
+- `Appmode.temp_dir` Create temp notebooks under this directory. Default: Same directory as current notebook
+
+Writing hidden files is by default disabled in newer versions of Jupyter.
+To allow Appmode to hide its temporary notebook copies the option `ContentsManager.allow_hidden` has to be set:
+```
+jupyter notebook --ContentsManager.allow_hidden=True
+```
 
 ## Client Side Customization
 
 The UI elements of Appmode can be customized via the [custom.js](http://jupyter-notebook.readthedocs.io/en/stable/examples/Notebook/JavaScript%20Notebook%20Extensions.html#custom.js) file. Some examples are:
 ```
 $('#appmode-leave').hide();                          // Hides the edit app button.
 $('#appmode-busy').hide();                           // Hides the kernel busy indicator.
```

### Comparing `appmode-0.8.0/LICENSE.txt` & `appmode-0.9.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `appmode-0.8.0/setup.py` & `appmode-0.9.0/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -22,22 +22,21 @@
     author_email = 'ole.schuett@cp2k.org',
     url='http://github.com/oschuett/appmode',
     description='A Jupyter extensions that turns notebooks into web applications.',
 
     packages=["appmode"],
     include_package_data = True,
     install_requires=['notebook>=5'],
+    python_requires='>=3.5',
     data_files=[('share/jupyter/nbextensions/appmode', [
                     'appmode/static/main.js',
                     'appmode/static/gears.svg'
     ])],
 
     classifiers=[
-        "Programming Language :: Python :: 2",
-        "Programming Language :: Python :: 2.7",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.5",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
 
 )
```

