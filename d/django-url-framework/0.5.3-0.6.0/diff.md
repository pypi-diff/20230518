# Comparing `tmp/django-url-framework-0.5.3.tar.gz` & `tmp/django-url-framework-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/django-url-framework-0.5.3.tar", last modified: Fri Aug 21 17:54:59 2020, max compression
+gzip compressed data, was "django-url-framework-0.6.0.tar", last modified: Thu May 18 07:50:43 2023, max compression
```

## Comparing `django-url-framework-0.5.3.tar` & `django-url-framework-0.6.0.tar`

### file list

```diff
@@ -1,38 +1,39 @@
-drwxrwxr-x   0 zeraien   (1000) zeraien   (1000)        0 2020-08-21 17:54:59.119258 django-url-framework-0.5.3/
--rwxrwxr-x   0 zeraien   (1000) zeraien   (1000)      424 2020-04-11 02:30:16.000000 django-url-framework-0.5.3/.gitignore
--rw-rw-r--   0 zeraien   (1000) zeraien   (1000)     1092 2015-03-30 14:19:19.000000 django-url-framework-0.5.3/LICENSE
--rw-rw-r--   0 zeraien   (1000) zeraien   (1000)    21883 2020-08-21 17:54:59.119258 django-url-framework-0.5.3/PKG-INFO
--rw-rw-r--   0 zeraien   (1000) zeraien   (1000)    17093 2020-08-21 17:52:20.000000 django-url-framework-0.5.3/README.md
-drwxrwxr-x   0 zeraien   (1000) zeraien   (1000)        0 2020-08-21 17:54:59.116258 django-url-framework-0.5.3/django_url_framework/
--rw-rw-r--   0 zeraien   (1000) zeraien   (1000)      762 2020-08-21 17:09:16.000000 django-url-framework-0.5.3/django_url_framework/__init__.py
--rw-rw-r--   0 zeraien   (1000) zeraien   (1000)      216 2020-04-09 19:52:05.000000 django-url-framework-0.5.3/django_url_framework/apps.py
--rw-rw-r--   0 zeraien   (1000) zeraien   (1000)    37533 2020-08-21 17:49:56.000000 django-url-framework-0.5.3/django_url_framework/controller.py
-drwxrwxr-x   0 zeraien   (1000) zeraien   (1000)        0 2020-08-21 17:54:59.118258 django-url-framework-0.5.3/django_url_framework/decorators/
--rw-rw-r--   0 zeraien   (1000) zeraien   (1000)      100 2020-04-09 22:08:35.000000 django-url-framework-0.5.3/django_url_framework/decorators/__init__.py
--rw-rw-r--   0 zeraien   (1000) zeraien   (1000)     3222 2015-03-30 18:16:39.000000 django-url-framework-0.5.3/django_url_framework/decorators/action_options.py
--rw-rw-r--   0 zeraien   (1000) zeraien   (1000)     2761 2020-01-12 10:28:52.000000 django-url-framework-0.5.3/django_url_framework/decorators/auth.py
--rw-rw-r--   0 zeraien   (1000) zeraien   (1000)     1730 2017-02-23 02:28:35.000000 django-url-framework-0.5.3/django_url_framework/decorators/http_methods.py
--rw-rw-r--   0 zeraien   (1000) zeraien   (1000)     1816 2020-04-29 13:50:33.000000 django-url-framework-0.5.3/django_url_framework/decorators/render.py
--rw-rw-r--   0 zeraien   (1000) zeraien   (1000)      243 2020-04-11 02:04:11.000000 django-url-framework-0.5.3/django_url_framework/exceptions.py
--rw-rw-r--   0 zeraien   (1000) zeraien   (1000)     2909 2020-01-12 10:28:49.000000 django-url-framework-0.5.3/django_url_framework/flash.py
--rw-rw-r--   0 zeraien   (1000) zeraien   (1000)     2767 2020-04-10 00:27:05.000000 django-url-framework-0.5.3/django_url_framework/helper.py
--rw-rw-r--   0 zeraien   (1000) zeraien   (1000)     4760 2020-08-21 17:49:14.000000 django-url-framework-0.5.3/django_url_framework/renderers.py
--rw-rw-r--   0 zeraien   (1000) zeraien   (1000)     7150 2020-04-09 23:38:27.000000 django-url-framework-0.5.3/django_url_framework/site.py
-drwxrwxr-x   0 zeraien   (1000) zeraien   (1000)        0 2020-08-21 17:54:59.118258 django-url-framework-0.5.3/django_url_framework/templatetags/
--rw-rw-r--   0 zeraien   (1000) zeraien   (1000)        0 2009-05-09 13:20:16.000000 django-url-framework-0.5.3/django_url_framework/templatetags/__init__.py
--rw-rw-r--   0 zeraien   (1000) zeraien   (1000)     2897 2020-01-12 10:28:49.000000 django-url-framework-0.5.3/django_url_framework/templatetags/url_framework.py
-drwxrwxr-x   0 zeraien   (1000) zeraien   (1000)        0 2020-08-21 17:54:59.117258 django-url-framework-0.5.3/django_url_framework.egg-info/
--rwxrwxr-x   0 zeraien   (1000) zeraien   (1000)    21883 2020-08-21 17:54:59.000000 django-url-framework-0.5.3/django_url_framework.egg-info/PKG-INFO
--rwxrwxr-x   0 zeraien   (1000) zeraien   (1000)     1002 2020-08-21 17:54:59.000000 django-url-framework-0.5.3/django_url_framework.egg-info/SOURCES.txt
--rwxrwxr-x   0 zeraien   (1000) zeraien   (1000)        1 2020-08-21 17:54:59.000000 django-url-framework-0.5.3/django_url_framework.egg-info/dependency_links.txt
--rwxrwxr-x   0 zeraien   (1000) zeraien   (1000)       47 2015-08-19 17:33:33.000000 django-url-framework-0.5.3/django_url_framework.egg-info/pbr.json
--rwxrwxr-x   0 zeraien   (1000) zeraien   (1000)       21 2020-08-21 17:54:59.000000 django-url-framework-0.5.3/django_url_framework.egg-info/top_level.txt
--rw-rw-r--   0 zeraien   (1000) zeraien   (1000)       38 2020-08-21 17:54:59.120258 django-url-framework-0.5.3/setup.cfg
--rw-rw-rw-   0 zeraien   (1000) zeraien   (1000)     1177 2020-04-29 14:05:46.000000 django-url-framework-0.5.3/setup.py
-drwxrwxr-x   0 zeraien   (1000) zeraien   (1000)        0 2020-08-21 17:54:59.119258 django-url-framework-0.5.3/tests/
--rw-rw-r--   0 zeraien   (1000) zeraien   (1000)      362 2020-04-11 02:21:01.000000 django-url-framework-0.5.3/tests/__init__.py
--rw-rw-r--   0 zeraien   (1000) zeraien   (1000)      701 2020-04-29 13:41:28.000000 django-url-framework-0.5.3/tests/duf_test_case.py
--rw-rw-r--   0 zeraien   (1000) zeraien   (1000)    11896 2020-04-29 13:41:49.000000 django-url-framework-0.5.3/tests/test_controller_action_renderers.py
--rw-rw-r--   0 zeraien   (1000) zeraien   (1000)     2590 2020-04-14 02:31:40.000000 django-url-framework-0.5.3/tests/test_get_actions.py
--rw-rw-r--   0 zeraien   (1000) zeraien   (1000)     1300 2020-04-11 02:40:32.000000 django-url-framework-0.5.3/tests/test_name_generation.py
--rw-rw-r--   0 zeraien   (1000) zeraien   (1000)      939 2020-04-29 13:51:15.000000 django-url-framework-0.5.3/tests/test_renderer_decorators.py
+drwxrwxrwx   0 zeraien   (1000) zeraien   (1000)        0 2023-05-18 14:04:48.091328 django-url-framework-0.6.0/
+-rwxrwxrwx   0 zeraien   (1000) zeraien   (1000)      424 2020-04-11 02:30:16.000000 django-url-framework-0.6.0/.gitignore
+-rwxrwxrwx   0 zeraien   (1000) zeraien   (1000)     1092 2015-03-30 14:19:19.000000 django-url-framework-0.6.0/LICENSE
+-rwxrwxrwx   0 zeraien   (1000) zeraien   (1000)    17838 2023-05-18 14:04:48.081237 django-url-framework-0.6.0/PKG-INFO
+-rwxrwxrwx   0 zeraien   (1000) zeraien   (1000)    17093 2020-08-21 17:52:20.000000 django-url-framework-0.6.0/README.md
+drwxrwxrwx   0 zeraien   (1000) zeraien   (1000)        0 2023-05-18 14:04:46.572068 django-url-framework-0.6.0/django_url_framework/
+-rwxrwxrwx   0 zeraien   (1000) zeraien   (1000)      762 2023-03-13 13:17:42.000000 django-url-framework-0.6.0/django_url_framework/__init__.py
+-rwxrwxrwx   0 zeraien   (1000) zeraien   (1000)      216 2023-03-13 13:16:08.000000 django-url-framework-0.6.0/django_url_framework/apps.py
+-rwxrwxrwx   0 zeraien   (1000) zeraien   (1000)    37219 2023-03-13 14:01:15.000000 django-url-framework-0.6.0/django_url_framework/controller.py
+drwxrwxrwx   0 zeraien   (1000) zeraien   (1000)        0 2023-05-18 14:04:47.421972 django-url-framework-0.6.0/django_url_framework/decorators/
+-rwxrwxrwx   0 zeraien   (1000) zeraien   (1000)      100 2020-04-09 22:08:35.000000 django-url-framework-0.6.0/django_url_framework/decorators/__init__.py
+-rwxrwxrwx   0 zeraien   (1000) zeraien   (1000)     3222 2015-03-30 18:16:39.000000 django-url-framework-0.6.0/django_url_framework/decorators/action_options.py
+-rwxrwxrwx   0 zeraien   (1000) zeraien   (1000)     2776 2023-03-13 14:13:45.000000 django-url-framework-0.6.0/django_url_framework/decorators/auth.py
+-rwxrwxrwx   0 zeraien   (1000) zeraien   (1000)     1730 2017-02-23 02:28:35.000000 django-url-framework-0.6.0/django_url_framework/decorators/http_methods.py
+-rwxrwxrwx   0 zeraien   (1000) zeraien   (1000)     2017 2023-03-13 13:16:30.000000 django-url-framework-0.6.0/django_url_framework/decorators/render.py
+-rwxrwxrwx   0 zeraien   (1000) zeraien   (1000)      243 2020-04-11 02:04:11.000000 django-url-framework-0.6.0/django_url_framework/exceptions.py
+-rwxrwxrwx   0 zeraien   (1000) zeraien   (1000)     2906 2023-01-08 20:28:06.000000 django-url-framework-0.6.0/django_url_framework/flash.py
+-rwxrwxrwx   0 zeraien   (1000) zeraien   (1000)     2671 2023-03-13 13:14:14.000000 django-url-framework-0.6.0/django_url_framework/helper.py
+-rwxrwxrwx   0 zeraien   (1000) zeraien   (1000)       91 2023-01-08 20:25:19.000000 django-url-framework-0.6.0/django_url_framework/lib.py
+-rwxrwxrwx   0 zeraien   (1000) zeraien   (1000)     4760 2020-08-21 17:49:14.000000 django-url-framework-0.6.0/django_url_framework/renderers.py
+-rwxrwxrwx   0 zeraien   (1000) zeraien   (1000)     7175 2023-03-13 14:02:46.000000 django-url-framework-0.6.0/django_url_framework/site.py
+drwxrwxrwx   0 zeraien   (1000) zeraien   (1000)        0 2023-05-18 14:04:47.536792 django-url-framework-0.6.0/django_url_framework/templatetags/
+-rwxrwxrwx   0 zeraien   (1000) zeraien   (1000)        0 2009-05-09 13:20:16.000000 django-url-framework-0.6.0/django_url_framework/templatetags/__init__.py
+-rwxrwxrwx   0 zeraien   (1000) zeraien   (1000)     2897 2020-01-12 10:28:49.000000 django-url-framework-0.6.0/django_url_framework/templatetags/url_framework.py
+drwxrwxrwx   0 zeraien   (1000) zeraien   (1000)        0 2023-05-18 14:04:47.014388 django-url-framework-0.6.0/django_url_framework.egg-info/
+-rwxrwxrwx   0 zeraien   (1000) zeraien   (1000)    17838 2023-05-18 14:04:44.000000 django-url-framework-0.6.0/django_url_framework.egg-info/PKG-INFO
+-rwxrwxrwx   0 zeraien   (1000) zeraien   (1000)     1030 2023-05-18 14:04:45.000000 django-url-framework-0.6.0/django_url_framework.egg-info/SOURCES.txt
+-rwxrwxrwx   0 zeraien   (1000) zeraien   (1000)        1 2023-05-18 14:04:44.000000 django-url-framework-0.6.0/django_url_framework.egg-info/dependency_links.txt
+-rwxrwxrwx   0 zeraien   (1000) zeraien   (1000)       47 2015-08-19 17:33:33.000000 django-url-framework-0.6.0/django_url_framework.egg-info/pbr.json
+-rwxrwxrwx   0 zeraien   (1000) zeraien   (1000)       21 2023-05-18 14:04:44.000000 django-url-framework-0.6.0/django_url_framework.egg-info/top_level.txt
+-rwxrwxrwx   0 zeraien   (1000) zeraien   (1000)       38 2023-05-18 14:04:48.093391 django-url-framework-0.6.0/setup.cfg
+-rwxrwxrwx   0 zeraien   (1000) zeraien   (1000)     1177 2020-04-29 14:05:46.000000 django-url-framework-0.6.0/setup.py
+drwxrwxrwx   0 zeraien   (1000) zeraien   (1000)        0 2023-05-18 14:04:47.993463 django-url-framework-0.6.0/tests/
+-rwxrwxrwx   0 zeraien   (1000) zeraien   (1000)      362 2020-04-11 02:21:01.000000 django-url-framework-0.6.0/tests/__init__.py
+-rwxrwxrwx   0 zeraien   (1000) zeraien   (1000)      701 2020-04-29 13:41:28.000000 django-url-framework-0.6.0/tests/duf_test_case.py
+-rwxrwxrwx   0 zeraien   (1000) zeraien   (1000)    11896 2020-04-29 13:41:49.000000 django-url-framework-0.6.0/tests/test_controller_action_renderers.py
+-rwxrwxrwx   0 zeraien   (1000) zeraien   (1000)     2590 2020-04-14 02:31:40.000000 django-url-framework-0.6.0/tests/test_get_actions.py
+-rwxrwxrwx   0 zeraien   (1000) zeraien   (1000)     1300 2020-04-11 02:40:32.000000 django-url-framework-0.6.0/tests/test_name_generation.py
+-rwxrwxrwx   0 zeraien   (1000) zeraien   (1000)      939 2020-04-29 13:51:15.000000 django-url-framework-0.6.0/tests/test_renderer_decorators.py
```

### Comparing `django-url-framework-0.5.3/LICENSE` & `django-url-framework-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django-url-framework-0.5.3/PKG-INFO` & `django-url-framework-0.6.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,526 +1,529 @@
 Metadata-Version: 2.1
 Name: django-url-framework
-Version: 0.5.3
+Version: 0.6.0
 Summary: Automagically discover urls in a django application, similar to the Ruby on Rails Controller/Action/View implementation.
 Home-page: https://github.com/zeraien/django-url-framework/
 Author: Dimo Fedortchenko
 Author-email: d@angelhill.net
 License: MIT
-Description: The django-url-framework will help you get your django applications done faster.
-        
-        ![build](https://github.com/zeraien/django-url-framework/workflows/build/badge.svg)
-        [![Documentation Status](https://readthedocs.org/projects/django-url-framework/badge/?version=latest)](https://django-url-framework.readthedocs.io/en/latest/?badge=latest)
-        [![Join the chat at https://gitter.im/zeraien/django-url-framework](https://badges.gitter.im/zeraien/django-url-framework.svg)](https://gitter.im/zeraien/django-url-framework?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge)
-        
-        It automatically detects urls in a django application, similar to the way Ruby on Rails does it with the Controller-Action-View implementation.
-        
-        Controllers are created in each django application with a predefined file naming scheme (`foo_controller.py`) and extending `ActionController`. The `ActionController` contains methods often used in a web context, and does common request-related processing.
-        
-        Each application can have multiple controllers thus allowing for smaller classes in a larger application.
-        
-        Each function not starting with an underscore becomes it's own action. By simply returning a dictionary from the action, it will be rendered with the template named using the `controller/action.html` naming scheme.
-        
-        Each action and controller can override certain global settings such as using a custom template name or giving the action (or controller) a custom name.
-        
-        ## Install
-        
-        From pypi:
-        
-        ```
-        pip install django-url-framework
-        ```
-        
-        Alternatively just check out the source here and run `python setup.py install` or `pip install .`
-        
-        ## Add to your project
-        
-        ### settings.py
-        
-        ```python
-        INSTALLED_APPS = (
-          ...,
-          'django_url_framework',
-          ...
-        )
-        ```
-        ### urls.py
-        ```python
-        import django_url_framework
-        from django.conf import settings
-        from django.conf.urls import patterns, include
-        
-        django_url_framework.site.autodiscover(new_inflection_library=True)
-        
-        urlpatterns = patterns('',
-            (r'^', include(django_url_framework.site.urls) ),
-        )
-        ```
-        
-        ## Example
-        
-        ### Folder structure
-        
-        ```
-        project/
-          app/
-              cart_controller.py
-              id_controller.py
-              templates/
-                   cart/
-                      add.html
-                      index.html
-                      remove.html
-                   id_manager/
-                      bar.html
-        ```
-        
-        ### cart_controller.py 
-        
-        ```python
-        from django_url_framework.controller import ActionController
-        
-        class CartController(ActionController):
-            def edit(self, request, id = None):
-                return {}
-            def remove(self, request, id):
-                return {}
-            def index(self, request):
-              return {}
-        ```
-        
-        ### id_controller.py
-        
-        ```python
-        from django_url_framework.controller import ActionController
-        
-        class IDManagerController(ActionController):
-            def index(self, request, object_id = None):
-                return {}
-            def bar(self, request):
-                return {}
-            def bar__delete(self, request):
-                return {}
-        ```
-        
-        ### Result
-        
-        The following URLs will be created:
-        
-        ```
-        /cart/ <- will go to *index action*
-        /cart/(\w+)/
-        /cart/edit/
-        /cart/edit/(\w+)/
-        /cart/remove/(\w+)/
-        /foo/
-        /foo/(\w+)/
-        /foo/bar/
-        /foo/bar/delete/
-        ```
-        
-        You can easily access your URLs using django's built-in `{% url ... %}` tag. Simply call `{% url cart_index %}` or `{% url cart_delete id %}` and it will work as you would expect.
-        
-        There is also a helper tag for faster linking within the same controller.
-        `{% go_action remove %}` will take you to `/cart/remove/`. To use it, `{% load url_framework %}` in your templates.
-        
-        The names of the controller files do not affect your URLs, however, the files must have `_controller.py` suffix. The URL name of the controller is derived from the class name, minus the Controller part. You can also manually specify controller names using the `controller_name` attribute on the controller class.
-        
-        ### Controller names
-        
-        The controller name is derived from it's class name, by converting camelcase into underscores.
-        For instance `FooController` is simple `foo`, while `FooBarController` becomes `foo_bar`.
-        
-        The latest version uses the `inflection` library, however to avoid breaking old code, this is still optional until 2021.
-        
-        The biggest difference is that with `inflection`, `HTTPResponse` becomes `http_response`, while the old name would be `httpresponse`. I suggest enabling the `inflection` library for all new and existing projects. You can manually specify names for controllers whose name change would break your code, or disable the inflection library for those controllers using a flag.
-        
-        You can give the controller a custom name with the `controller_name` parameter:
-        ```python
-        class Controller(ActionController):
-          controller_name = "foo"
-        ```
-        
-        Enable or disable the use of the new `inflection` library using a flag
-        ```python
-        class Controller(ActionController):
-          use_inflection_library = True
-        ```
-        
-        ### Other useful controller settings
-        
-        ```python
-        class BarController(ActionController):
-            
-            # default filename extension for all templates
-            template_extension = "pug" 
-            
-            # will require every template file to start with this string
-            template_prefix = "foo_" 
-            
-            # will not look for templates in subdirectories, but in the root templates/ folder
-            no_subdirectories = False 
-            
-            # do not prefix templates with `_` (underscore) when they are called using an AJAX request
-            no_ajax_prefix = False 
-        
-            # Set a prefix for the controller's name, applies even if
-            # you set controller_name (template name is based on controller_name, sans prefix)
-            # NOTE: The urlconf name will not include the prefix, only the actual URL itself
-            # Thus: FooController.list will have the URL /prefixed_foo/list/, but the url name will be
-            # `foo_list`.
-            controller_prefix = "prefixed_" 
-            
-            # completely override the name of the controller
-            controller_name = "shopping_cart" 
-        
-            # When used with custom urlconf in actions, these arguments will not be passed to the action
-            # example: "/<id:int>/<skip:bool>/" Only `id` will be passed to the `action`, while `skip` will not be.
-            consume_urlconf_keyword_arguments = ['skip']
-        
-            # set a prefix for all the URLs in this controller
-            # So, what normally would be `/controller/action/`, becomes `^prefix/controller/action/`
-            urlconf_prefix:list = ["^prefix"]
-        
-            # A custom json encoder, subclassing JSONEncoder 
-            json_default_encoder:JSONEncoder = None
-        
-            # use the yaml default flow style
-            yaml_default_flow_style:bool = True
-        
-            # use the new inflection library to generate controller url
-            # if this is None, will use the global setting, otherwise override this on a per controller basis
-            use_inflection_library:Union[bool,None] = None
-        
-        ```
-        
-        ### Template filenames
-        
-        By default templates are stored in the subdirectory with the controller's name, and the templates are given the same filename as the action name.
-        If a request is determinned to be AJAX in nature, the template filename is prefixed with an underscore.
-        Example:
-        ```python
-        class FooController(ActionController):
-            def foo_action(self, request):
-              return {}
-        ```
-        
-        File structure:
-        ```python
-        /foo/foo_action.html
-        /foo/_foo_action.html <--- for AJAX requests.
-        ```
-        
-        You can disable this prefixing on a per action or per controller level.
-        
-        For all actions in a controller:
-        ```python
-        class FooController(ActionController):
-            no_ajax_prefix = True
-        ```
-        
-        For a single action:
-        ```python
-        from django_url_framework.decorators.action_options
-        class FooController(ActionController):
-            @no_ajax_prefix
-            def foo_action(self, request):
-              return {}
-        ```
-        
-        
-        ## Action names
-        
-        ```python
-        class FooController(ActionController):
-            def action(self, request):
-              return {}
-        ```
-        Creates the following URL:
-        ```
-        /controller/action/
-        ```
-        
-        Double underscores `__` in action names are converted to slashes in the urlconf, so: `action__name` becomes `/action/name/`.
-        
-        ```python
-        class Controller(ActionController):
-            def action__foo(self, request):
-              return {}
-        ```
-        Creates the following URL:
-        ```
-        /controller/action/foo/
-        ```
-        
-        
-        ### Decorate to name
-        
-        You can also decorate functions to give them different names and prefixes and urls. See decorator package for more details, here is an example:
-        ```python
-        @action_options.name("foo")
-        @action_options.prefix("prefix_")
-        def bar(self, request):
-          return {}
-        ```
-        will result in:
-        ```
-        /controller/prefix_foo/
-        ```
-        
-        The action will now have the template `/controller/foo.html`. Prefixes do not affect template naming.
-        
-        ## Action parameters
-        
-        Providing a third parameter to an action will create a URLconf for that parameter, like so:
-        ```python
-        def action(self, request, object_id):
-            return {}
-        ```
-        Will allow you to call that action with:
-        ```
-        /controller/action/(\w+)/ <--- parameter consisting of A-Za-z0-9_
-        ```
-        If you make the argument optional, an additional URLconf entry is created allowing you to call the action without the third argument.
-        ```python
-        def action(self, request, object_id = None):
-            return {}
-        ```
-        Results in:
-        
-        ```
-        /controller/action/
-        /controller/action/(\w+)/  <--- optional argument consisting of A-Za-z0-9_
-        ```
-        
-        ### Decorate for JSON, YAML or Automatic
-        
-        You can decorate any action to have a default renderer.
-        Instead of using `self._as_json` as before, you can just put a decorator like so:
-        
-        ```python
-        from django_url_framework.decorators import json_action
-            @json_action(json_encoder=None)
-            def action(self, request, year, month):
-                ...
-                return {}
-        ```
-        Other decorators include `@yaml_action(default_flow_style:bool)` and `@auto()`.
-        YaML is self-explanatory, however `@auto` is a bit interesting, it will automatically determine the renderer based on the `HTTP_ACCEPT` header. 
-        
-        *Warning* - if you expose raw data in your actions, that normally would be massaged inside a Server-Side template, DO NOT USE the `@auto` decorator as this allows an attacker to download raw data from your server.
-        However, if your responses are designed for an API, the `@auto` decorator will enable the API client to request data as it sees fit, for example, it can request a Server-Side rendered HTML, or the same data as JSON or YaML.
-        
-        Here is a list of supported renderers:
-        - text/html - `TemplateRenderer` - renders using the appropriate Django template
-        - text/plain - `TextRenderer` - prints text data as is, or prints object types using `pprint.pformat`
-        - application/json - `JSONRenderer` - renders data as JSON
-        - application/yaml - `YamlRenderer` - renders data as YaML
-        
-        `@auto()` accepts the following parameters:
-        - json_encoder
-        - yaml_default_flow_style
-        The work the same as if passed to `@json_action()` or `@yaml_action()`
-        
-        ### Set HTTP Status Codes easily
-        
-        Any action can return a tuple of two items, the second item should be an `int` and will become the HTTP status code for your response.
-        
-        ```python
-            @json_action()
-            def update(self, request, year, month):
-                ...
-                return False, 304 #not modified
-        
-            @json_action()
-            def create(self, request, year, month):
-                ...
-                return True, 201 #created
-        ```
-        
-        ### Decorate for custom parameters
-        
-        You can also create your own custom parameters by using the `@url_parameters` decorator to the function.
-        ```python
-        from django_url_framework.decorators.action_options import url_paramters
-        class Controller(ActionController):
-            @url_parameters(r'(?P<year>\d{4})/(?P<month>\d\d)')
-            def action(self, request, year, month):
-                ...
-                return {}
-        ```
-        The above will create the following url patterns:
-        ```
-        /controller/action/(?P<year>\d{4})/(?P<month>\d\d)
-        ```
-        *Note the lack of trailing slash - you must provide this yourself.*
-        
-        ### Custom url for any action
-        
-        You can write your own urlconf for each action, by decorating it with `@urlconf`.
-        ```python
-        from django_url_framework.decorators.action_options import urlconf
-        class Controller(ActionController):
-            @action_options.urlconf([
-                    r'^bar/(?P<year>\d{4})/$',
-                    r'^bar/(?P<year>\d{4})/(?P<month>\d\d)/$',
-                    r'^foo/(?P<year>\d{4})/(?P<month>\d\d)/(?P<day>\d\d)/$'
-                ],
-                do_not_autogenerate=True)
-            def action(self, request, year, month=None, day=None):
-                ...
-                return {}
-        ```
-        The above will create the following url patterns:
-        ```
-        /controller/bar/(?P<year>\d{4})/
-        /controller/bar/(?P<year>\d{4})/(?P<month>\d\d)/$
-        /controller/foo/(?P<year>\d{4})/(?P<month>\d\d)/(?P<day>\d\d)/$
-        ```
-        
-        The `do_not_autogenerate` argument is **true** by default and will prevent any urls for this action
-        from being autogenerated. If `do_not_autogenerate` were to be set to false in the example below,
-        the following url would also be created:
-        ```
-        /controller/action/
-        ```
-        This URL would not actually work since the `year` argument is required the `action` function.
-        
-        ## Flash messages
-        
-        The ActionController also has a `_flash` instance variable that allows you to send messages to the user that can survive a redirect. Simply use 
-        
-        ```python
-        self._flash.append("Message")
-        
-        self._flash.error("Error message")
-        ```
-        
-        The flash messages can be either messages or error messages. The flash object is automatically exported into the context and you can use it as such:
-        
-        ```HTML+Django
-        {% if flash.has_messages %}
-          {% for message in flash.get_and_clear %}
-        
-              {% if message.is_error %}<span class='icon-error'></span>{% endif %}
-        
-              <p class="{{message.type}}">{{message}}</p>
-              
-          {% endfor %}
-        {% endif }
-        ```
-        
-        ## Before and After each action
-        
-        You can override `_before_filter` and/or `_after_filter` to perform certain actions and checks before or after an action. Read more in `ActionController` docs.
-        
-        These methods accept the "request" parameter which is an HTTP request object for this request.
-        
-        ```python
-        class AccountController(ActionController):
-        
-            def _before_filter(self, request):
-                campaign_id = request.GET.get("campaign_id")
-                try:
-                  self._campaign = Campaign.objects.get(pk=campaign_id)
-                except Campaign.DoesNotExist:
-                  self._campaign = None
-        ```
-        
-        You can disable the before and after filters by decorating any action with the `@disable_filters` decorator.
-        
-        Example:
-        ```python
-        from django_url_framework.decorators.action_options import disable_filters
-        @disable_filters
-        def action(self, request):
-          return {}
-        ```
-        
-        One of the great features of django url framework is that you can require login for all actions in a controller by simply decorating the before_filter with a decorator to require logging in, see next section!
-        
-        ## Authentication
-        
-        To require login on an action use the `@login_required` decorator provided by django-url-framework. The decorator also works on `_before_filter`.
-        
-        ```python
-        from django_url_framework.decorators import login_required
-        class AccountController(ActionController):
-        
-            @login_required
-            def action(self, request):
-                return {}
-        ```
-        
-        If the user isn’t logged in, redirect to `settings.LOGIN_URL`, passing the current absolute path in the query string. Example: `/accounts/login/?next=/polls/3/`.
-        `login_required()` also takes an optional `login_url` parameter. Example:
-        
-        ```python
-        from django_url_framework.decorators import login_required
-        class AccountController(ActionController):
-        
-            @login_required(login_url="/login/")
-            def action(self, request):
-                return {}
-        ```
-        
-        By default, the path that the user should be redirected to upon successful authentication is stored in a query string parameter called "next". If you would prefer to use a different name for this parameter, `login_required()` takes an optional `redirect_field_name` parameter.
-        
-        Additionally you can use `@superuser_required`, `@permission_required(permission_instance)` and `@must_be_member_of_group(group_name="some_group")`.
-        
-        Another example makes it easy to limiting access to a subset of data based on the logged in user for the whole controller.
-        
-        ```python
-        from django_url_framework.decorators import login_required
-        class ItemController(ActionController):
-            @login_required()
-            def _before_filter(self):
-                self.my_items = Item.objects.filter(user=request.user)
-                self.my_products = Product.objects.filter(item__in=self.my_items)
-                return {
-                    "page_title": "Item Page"
-                }
-            def item(self, request, pk):
-                item = get_object_or_404(self.my_items, pk=pk)
-                return {"item":item}
-            def product(self, request, pk):
-                item = get_object_or_404(self.my_products, pk=pk)
-                return {"product":product}
-        
-        
-        ```
-        
-        ## Only POST? (or GET or anything...)
-        You can limit what http methods a function can be called with.
-        
-        The example below limits the `update` action to only **POST** and **DELETE** http methods.
-        
-        ```python
-        from django_url_framework.decorators import http_methods
-        class Controller(ActionController):
-            @http_methods.POST
-            @http_methods.DELETE
-            def update(self, request):
-                return {}
-        ```
-        
-        By default all actions can be called with all http methods.
-        
-        ## Custom template extensions
-        When using jade or something similar you can specify a custom extension for all templates in the controller.
-        
-        ```python
-        class FooController(ActionController):
-            #custom extension for all templates in this controller
-            template_extension = "jade"
-        ```
-        
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Utilities
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+The django-url-framework will help you get your django applications done faster.
+
+![build](https://github.com/zeraien/django-url-framework/workflows/build/badge.svg)
+[![Documentation Status](https://readthedocs.org/projects/django-url-framework/badge/?version=latest)](https://django-url-framework.readthedocs.io/en/latest/?badge=latest)
+[![Join the chat at https://gitter.im/zeraien/django-url-framework](https://badges.gitter.im/zeraien/django-url-framework.svg)](https://gitter.im/zeraien/django-url-framework?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge)
+
+It automatically detects urls in a django application, similar to the way Ruby on Rails does it with the Controller-Action-View implementation.
+
+Controllers are created in each django application with a predefined file naming scheme (`foo_controller.py`) and extending `ActionController`. The `ActionController` contains methods often used in a web context, and does common request-related processing.
+
+Each application can have multiple controllers thus allowing for smaller classes in a larger application.
+
+Each function not starting with an underscore becomes it's own action. By simply returning a dictionary from the action, it will be rendered with the template named using the `controller/action.html` naming scheme.
+
+Each action and controller can override certain global settings such as using a custom template name or giving the action (or controller) a custom name.
+
+## Install
+
+From pypi:
+
+```
+pip install django-url-framework
+```
+
+Alternatively just check out the source here and run `python setup.py install` or `pip install .`
+
+## Add to your project
+
+### settings.py
+
+```python
+INSTALLED_APPS = (
+  ...,
+  'django_url_framework',
+  ...
+)
+```
+### urls.py
+```python
+import django_url_framework
+from django.conf import settings
+from django.conf.urls import patterns, include
+
+django_url_framework.site.autodiscover(new_inflection_library=True)
+
+urlpatterns = patterns('',
+    (r'^', include(django_url_framework.site.urls) ),
+)
+```
+
+## Example
+
+### Folder structure
+
+```
+project/
+  app/
+      cart_controller.py
+      id_controller.py
+      templates/
+           cart/
+              add.html
+              index.html
+              remove.html
+           id_manager/
+              bar.html
+```
+
+### cart_controller.py 
+
+```python
+from django_url_framework.controller import ActionController
+
+class CartController(ActionController):
+    def edit(self, request, id = None):
+        return {}
+    def remove(self, request, id):
+        return {}
+    def index(self, request):
+      return {}
+```
+
+### id_controller.py
+
+```python
+from django_url_framework.controller import ActionController
+
+class IDManagerController(ActionController):
+    def index(self, request, object_id = None):
+        return {}
+    def bar(self, request):
+        return {}
+    def bar__delete(self, request):
+        return {}
+```
+
+### Result
+
+The following URLs will be created:
+
+```
+/cart/ <- will go to *index action*
+/cart/(\w+)/
+/cart/edit/
+/cart/edit/(\w+)/
+/cart/remove/(\w+)/
+/foo/
+/foo/(\w+)/
+/foo/bar/
+/foo/bar/delete/
+```
+
+You can easily access your URLs using django's built-in `{% url ... %}` tag. Simply call `{% url cart_index %}` or `{% url cart_delete id %}` and it will work as you would expect.
+
+There is also a helper tag for faster linking within the same controller.
+`{% go_action remove %}` will take you to `/cart/remove/`. To use it, `{% load url_framework %}` in your templates.
+
+The names of the controller files do not affect your URLs, however, the files must have `_controller.py` suffix. The URL name of the controller is derived from the class name, minus the Controller part. You can also manually specify controller names using the `controller_name` attribute on the controller class.
+
+### Controller names
+
+The controller name is derived from it's class name, by converting camelcase into underscores.
+For instance `FooController` is simple `foo`, while `FooBarController` becomes `foo_bar`.
+
+The latest version uses the `inflection` library, however to avoid breaking old code, this is still optional until 2021.
+
+The biggest difference is that with `inflection`, `HTTPResponse` becomes `http_response`, while the old name would be `httpresponse`. I suggest enabling the `inflection` library for all new and existing projects. You can manually specify names for controllers whose name change would break your code, or disable the inflection library for those controllers using a flag.
+
+You can give the controller a custom name with the `controller_name` parameter:
+```python
+class Controller(ActionController):
+  controller_name = "foo"
+```
+
+Enable or disable the use of the new `inflection` library using a flag
+```python
+class Controller(ActionController):
+  use_inflection_library = True
+```
+
+### Other useful controller settings
+
+```python
+class BarController(ActionController):
+    
+    # default filename extension for all templates
+    template_extension = "pug" 
+    
+    # will require every template file to start with this string
+    template_prefix = "foo_" 
+    
+    # will not look for templates in subdirectories, but in the root templates/ folder
+    no_subdirectories = False 
+    
+    # do not prefix templates with `_` (underscore) when they are called using an AJAX request
+    no_ajax_prefix = False 
+
+    # Set a prefix for the controller's name, applies even if
+    # you set controller_name (template name is based on controller_name, sans prefix)
+    # NOTE: The urlconf name will not include the prefix, only the actual URL itself
+    # Thus: FooController.list will have the URL /prefixed_foo/list/, but the url name will be
+    # `foo_list`.
+    controller_prefix = "prefixed_" 
+    
+    # completely override the name of the controller
+    controller_name = "shopping_cart" 
+
+    # When used with custom urlconf in actions, these arguments will not be passed to the action
+    # example: "/<id:int>/<skip:bool>/" Only `id` will be passed to the `action`, while `skip` will not be.
+    consume_urlconf_keyword_arguments = ['skip']
+
+    # set a prefix for all the URLs in this controller
+    # So, what normally would be `/controller/action/`, becomes `^prefix/controller/action/`
+    urlconf_prefix:list = ["^prefix"]
+
+    # A custom json encoder, subclassing JSONEncoder 
+    json_default_encoder:JSONEncoder = None
+
+    # use the yaml default flow style
+    yaml_default_flow_style:bool = True
+
+    # use the new inflection library to generate controller url
+    # if this is None, will use the global setting, otherwise override this on a per controller basis
+    use_inflection_library:Union[bool,None] = None
+
+```
+
+### Template filenames
+
+By default templates are stored in the subdirectory with the controller's name, and the templates are given the same filename as the action name.
+If a request is determinned to be AJAX in nature, the template filename is prefixed with an underscore.
+Example:
+```python
+class FooController(ActionController):
+    def foo_action(self, request):
+      return {}
+```
+
+File structure:
+```python
+/foo/foo_action.html
+/foo/_foo_action.html <--- for AJAX requests.
+```
+
+You can disable this prefixing on a per action or per controller level.
+
+For all actions in a controller:
+```python
+class FooController(ActionController):
+    no_ajax_prefix = True
+```
+
+For a single action:
+```python
+from django_url_framework.decorators.action_options
+class FooController(ActionController):
+    @no_ajax_prefix
+    def foo_action(self, request):
+      return {}
+```
+
+
+## Action names
+
+```python
+class FooController(ActionController):
+    def action(self, request):
+      return {}
+```
+Creates the following URL:
+```
+/controller/action/
+```
+
+Double underscores `__` in action names are converted to slashes in the urlconf, so: `action__name` becomes `/action/name/`.
+
+```python
+class Controller(ActionController):
+    def action__foo(self, request):
+      return {}
+```
+Creates the following URL:
+```
+/controller/action/foo/
+```
+
+
+### Decorate to name
+
+You can also decorate functions to give them different names and prefixes and urls. See decorator package for more details, here is an example:
+```python
+@action_options.name("foo")
+@action_options.prefix("prefix_")
+def bar(self, request):
+  return {}
+```
+will result in:
+```
+/controller/prefix_foo/
+```
+
+The action will now have the template `/controller/foo.html`. Prefixes do not affect template naming.
+
+## Action parameters
+
+Providing a third parameter to an action will create a URLconf for that parameter, like so:
+```python
+def action(self, request, object_id):
+    return {}
+```
+Will allow you to call that action with:
+```
+/controller/action/(\w+)/ <--- parameter consisting of A-Za-z0-9_
+```
+If you make the argument optional, an additional URLconf entry is created allowing you to call the action without the third argument.
+```python
+def action(self, request, object_id = None):
+    return {}
+```
+Results in:
+
+```
+/controller/action/
+/controller/action/(\w+)/  <--- optional argument consisting of A-Za-z0-9_
+```
+
+### Decorate for JSON, YAML or Automatic
+
+You can decorate any action to have a default renderer.
+Instead of using `self._as_json` as before, you can just put a decorator like so:
+
+```python
+from django_url_framework.decorators import json_action
+    @json_action(json_encoder=None)
+    def action(self, request, year, month):
+        ...
+        return {}
+```
+Other decorators include `@yaml_action(default_flow_style:bool)` and `@auto()`.
+YaML is self-explanatory, however `@auto` is a bit interesting, it will automatically determine the renderer based on the `HTTP_ACCEPT` header. 
+
+*Warning* - if you expose raw data in your actions, that normally would be massaged inside a Server-Side template, DO NOT USE the `@auto` decorator as this allows an attacker to download raw data from your server.
+However, if your responses are designed for an API, the `@auto` decorator will enable the API client to request data as it sees fit, for example, it can request a Server-Side rendered HTML, or the same data as JSON or YaML.
+
+Here is a list of supported renderers:
+- text/html - `TemplateRenderer` - renders using the appropriate Django template
+- text/plain - `TextRenderer` - prints text data as is, or prints object types using `pprint.pformat`
+- application/json - `JSONRenderer` - renders data as JSON
+- application/yaml - `YamlRenderer` - renders data as YaML
+
+`@auto()` accepts the following parameters:
+- json_encoder
+- yaml_default_flow_style
+The work the same as if passed to `@json_action()` or `@yaml_action()`
+
+### Set HTTP Status Codes easily
+
+Any action can return a tuple of two items, the second item should be an `int` and will become the HTTP status code for your response.
+
+```python
+    @json_action()
+    def update(self, request, year, month):
+        ...
+        return False, 304 #not modified
+
+    @json_action()
+    def create(self, request, year, month):
+        ...
+        return True, 201 #created
+```
+
+### Decorate for custom parameters
+
+You can also create your own custom parameters by using the `@url_parameters` decorator to the function.
+```python
+from django_url_framework.decorators.action_options import url_paramters
+class Controller(ActionController):
+    @url_parameters(r'(?P<year>\d{4})/(?P<month>\d\d)')
+    def action(self, request, year, month):
+        ...
+        return {}
+```
+The above will create the following url patterns:
+```
+/controller/action/(?P<year>\d{4})/(?P<month>\d\d)
+```
+*Note the lack of trailing slash - you must provide this yourself.*
+
+### Custom url for any action
+
+You can write your own urlconf for each action, by decorating it with `@urlconf`.
+```python
+from django_url_framework.decorators.action_options import urlconf
+class Controller(ActionController):
+    @action_options.urlconf([
+            r'^bar/(?P<year>\d{4})/$',
+            r'^bar/(?P<year>\d{4})/(?P<month>\d\d)/$',
+            r'^foo/(?P<year>\d{4})/(?P<month>\d\d)/(?P<day>\d\d)/$'
+        ],
+        do_not_autogenerate=True)
+    def action(self, request, year, month=None, day=None):
+        ...
+        return {}
+```
+The above will create the following url patterns:
+```
+/controller/bar/(?P<year>\d{4})/
+/controller/bar/(?P<year>\d{4})/(?P<month>\d\d)/$
+/controller/foo/(?P<year>\d{4})/(?P<month>\d\d)/(?P<day>\d\d)/$
+```
+
+The `do_not_autogenerate` argument is **true** by default and will prevent any urls for this action
+from being autogenerated. If `do_not_autogenerate` were to be set to false in the example below,
+the following url would also be created:
+```
+/controller/action/
+```
+This URL would not actually work since the `year` argument is required the `action` function.
+
+## Flash messages
+
+The ActionController also has a `_flash` instance variable that allows you to send messages to the user that can survive a redirect. Simply use 
+
+```python
+self._flash.append("Message")
+
+self._flash.error("Error message")
+```
+
+The flash messages can be either messages or error messages. The flash object is automatically exported into the context and you can use it as such:
+
+```HTML+Django
+{% if flash.has_messages %}
+  {% for message in flash.get_and_clear %}
+
+      {% if message.is_error %}<span class='icon-error'></span>{% endif %}
+
+      <p class="{{message.type}}">{{message}}</p>
+      
+  {% endfor %}
+{% endif }
+```
+
+## Before and After each action
+
+You can override `_before_filter` and/or `_after_filter` to perform certain actions and checks before or after an action. Read more in `ActionController` docs.
+
+These methods accept the "request" parameter which is an HTTP request object for this request.
+
+```python
+class AccountController(ActionController):
+
+    def _before_filter(self, request):
+        campaign_id = request.GET.get("campaign_id")
+        try:
+          self._campaign = Campaign.objects.get(pk=campaign_id)
+        except Campaign.DoesNotExist:
+          self._campaign = None
+```
+
+You can disable the before and after filters by decorating any action with the `@disable_filters` decorator.
+
+Example:
+```python
+from django_url_framework.decorators.action_options import disable_filters
+@disable_filters
+def action(self, request):
+  return {}
+```
+
+One of the great features of django url framework is that you can require login for all actions in a controller by simply decorating the before_filter with a decorator to require logging in, see next section!
+
+## Authentication
+
+To require login on an action use the `@login_required` decorator provided by django-url-framework. The decorator also works on `_before_filter`.
+
+```python
+from django_url_framework.decorators import login_required
+class AccountController(ActionController):
+
+    @login_required
+    def action(self, request):
+        return {}
+```
+
+If the user isn’t logged in, redirect to `settings.LOGIN_URL`, passing the current absolute path in the query string. Example: `/accounts/login/?next=/polls/3/`.
+`login_required()` also takes an optional `login_url` parameter. Example:
+
+```python
+from django_url_framework.decorators import login_required
+class AccountController(ActionController):
+
+    @login_required(login_url="/login/")
+    def action(self, request):
+        return {}
+```
+
+By default, the path that the user should be redirected to upon successful authentication is stored in a query string parameter called "next". If you would prefer to use a different name for this parameter, `login_required()` takes an optional `redirect_field_name` parameter.
+
+Additionally you can use `@superuser_required`, `@permission_required(permission_instance)` and `@must_be_member_of_group(group_name="some_group")`.
+
+Another example makes it easy to limiting access to a subset of data based on the logged in user for the whole controller.
+
+```python
+from django_url_framework.decorators import login_required
+class ItemController(ActionController):
+    @login_required()
+    def _before_filter(self):
+        self.my_items = Item.objects.filter(user=request.user)
+        self.my_products = Product.objects.filter(item__in=self.my_items)
+        return {
+            "page_title": "Item Page"
+        }
+    def item(self, request, pk):
+        item = get_object_or_404(self.my_items, pk=pk)
+        return {"item":item}
+    def product(self, request, pk):
+        item = get_object_or_404(self.my_products, pk=pk)
+        return {"product":product}
+
+
+```
+
+## Only POST? (or GET or anything...)
+You can limit what http methods a function can be called with.
+
+The example below limits the `update` action to only **POST** and **DELETE** http methods.
+
+```python
+from django_url_framework.decorators import http_methods
+class Controller(ActionController):
+    @http_methods.POST
+    @http_methods.DELETE
+    def update(self, request):
+        return {}
+```
+
+By default all actions can be called with all http methods.
+
+## Custom template extensions
+When using jade or something similar you can specify a custom extension for all templates in the controller.
+
+```python
+class FooController(ActionController):
+    #custom extension for all templates in this controller
+    template_extension = "jade"
+```
+
+
```

### Comparing `django-url-framework-0.5.3/README.md` & `django-url-framework-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `django-url-framework-0.5.3/django_url_framework/__init__.py` & `django-url-framework-0.6.0/django_url_framework/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-VERSION = (0, 5, 3)
+VERSION = (0, 6, 0)
 default_app_config = 'django_url_framework.apps.URLFrameworkAppConfig'
 
 
 # Dynamically calculate the version based on VERSION tuple
 if len(VERSION)>2 and VERSION[2] is not None:
     str_version = "%d.%d.%s" % VERSION[:3]
 else:
```

### Comparing `django-url-framework-0.5.3/django_url_framework/controller.py` & `django-url-framework-0.6.0/django_url_framework/controller.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,20 +13,18 @@
 
 from django.http import *
 import re
 import sys
 
 import warnings
 
+from .lib import is_ajax
 from .renderers import JSONRenderer, YAMLRenderer, TextRenderer, TemplateRenderer, Renderer, RedirectRenderer
 from .helper import ApplicationHelper
-from django.conf.urls import url, include
-from django import VERSION
-if VERSION[:2]<(1,9):
-    from django.conf.urls import patterns
+from django.urls import re_path, include
 
 from .exceptions import ConfigurationError
 from .exceptions import MethodNotAllowed
 from .exceptions import InvalidActionError
 
 def get_controller_name(controller_class:'ActionController.__class__', with_prefix:bool = True) -> str:
     if isinstance(controller_class, ActionController):
@@ -131,25 +129,19 @@
         if arg_name in arg_spec.annotations:
             datatype = arg_spec.annotations[arg_name]
         else:
             datatype = None
         return arg_name, has_default, datatype
     return None, True, None
 
-def url_patterns(*args):
-    if VERSION[:2]>=(1,9):
-        return list(args)
-    else:
-        return patterns('', *args)
-
 def get_controller_urlconf(controller_class:'ActionController.__class__', site=None):
     controller_name = get_controller_name(controller_class)
     actions = get_actions(controller_class)
-    urlpatterns = url_patterns()
-    urlpatterns_with_args = url_patterns()
+    urlpatterns = []
+    urlpatterns_with_args = []
     def wrap_call(_controller_name, _action_name, _action_func):
         """Wrapper for the function called by the url."""
         def wrapper(*args, **kwargs):
             request, args = args[0], args[1:]
             return autoview_function(site=site,
                                      request=request,
                                      controller_name=_controller_name,
@@ -159,67 +151,67 @@
 
     for action_name, action_func in list(actions.items()):
         named_url = '%s_%s' % (get_controller_name(controller_class, with_prefix=False), get_action_name(action_func) )
         named_url = getattr(action_func, 'named_url', named_url)
         replace_dict = {'action':action_name.replace("__","/")}
         wrapped_call = wrap_call(controller_name, action_name, action_func)
         urlconf_prefix = getattr(controller_class, 'urlconf_prefix', None)
-        action_urlpatterns = url_patterns()
-        index_action_with_args_urlconf = url_patterns()
+        action_urlpatterns = []
+        index_action_with_args_urlconf = []
 
         if hasattr(action_func, 'urlconf'):
             """Define custom urlconf patterns for this action."""
             for new_urlconf in action_func.urlconf:
-                action_urlpatterns += url_patterns(url(new_urlconf, view=wrapped_call, name=named_url))
+                action_urlpatterns.append(re_path(new_urlconf, view=wrapped_call, name=named_url))
 
         if not getattr(action_func, 'urlconf_erase', False):
             """Do not generate default URL patterns if we define 'urlconf_erase' for this action."""
 
             if action_name == 'index':
                 # No root URL is generated if we have no index action.
 
                 object_id_arg_name, has_default, datatype = _get_arg_name_and_default(action_func)
                 if object_id_arg_name is not None:
                     replace_dict['object_id_arg_name'] = object_id_arg_name
                     replace_dict['type'] = _get_urlconf_param_type(datatype)
-                    index_action_with_args_urlconf += url_patterns(path("<%(type)s:%(object_id_arg_name)s>/" % replace_dict, view=wrapped_call, name=named_url))
+                    index_action_with_args_urlconf.append(path("<%(type)s:%(object_id_arg_name)s>/" % replace_dict, view=wrapped_call, name=named_url))
                 if has_default:
-                    action_urlpatterns += url_patterns(url(r'^$', view=wrapped_call, name=named_url))
+                    action_urlpatterns.append(path("", view=wrapped_call, name=named_url))
 
             else:
                 if hasattr(action_func, 'url_parameters'):
                     arguments = action_func.url_parameters
                     replace_dict['url_parameters'] = arguments
-                    action_urlpatterns += url_patterns(url(r'^%(action)s/%(url_parameters)s$' % replace_dict, view=wrapped_call, name=named_url))
+                    action_urlpatterns.append(path("%(action)s/%(url_parameters)s" % replace_dict, view=wrapped_call, name=named_url))
 
                 else:
                     object_id_arg_name, has_default, datatype = _get_arg_name_and_default(action_func)
                     if object_id_arg_name is not None:
                         replace_dict['object_id_arg_name'] = object_id_arg_name
                         replace_dict['type'] = _get_urlconf_param_type(datatype)
-                        action_urlpatterns += url_patterns(path('%(action)s/<%(type)s:%(object_id_arg_name)s>/' % replace_dict, view=wrapped_call, name=named_url))
+                        action_urlpatterns.append(path('%(action)s/<%(type)s:%(object_id_arg_name)s>/' % replace_dict, view=wrapped_call, name=named_url))
                     if has_default:
-                        action_urlpatterns += url_patterns(path('%(action)s/' % replace_dict, view=wrapped_call, name=named_url))
+                        action_urlpatterns.append(path('%(action)s/' % replace_dict, view=wrapped_call, name=named_url))
 
         if urlconf_prefix:
-            action_urlpatterns_with_prefix = url_patterns()
+            action_urlpatterns_with_prefix = []
             for _urlconf in urlconf_prefix:
-                action_urlpatterns_with_prefix+=url_patterns(url(_urlconf, include(action_urlpatterns)))
-            urlpatterns+=action_urlpatterns_with_prefix
+                action_urlpatterns_with_prefix.append(re_path(_urlconf, include(action_urlpatterns)))
+            urlpatterns += action_urlpatterns_with_prefix
 
-            action_urlpatterns_with_args_with_prefix = url_patterns()
+            action_urlpatterns_with_args_with_prefix = []
             for _urlconf in urlconf_prefix:
-                action_urlpatterns_with_args_with_prefix+=url_patterns(url(_urlconf, include(action_urlpatterns_with_args_with_prefix)))
+                action_urlpatterns_with_args_with_prefix.append(re_path(_urlconf, include(action_urlpatterns_with_args_with_prefix)))
 
-            urlpatterns_with_args+=action_urlpatterns_with_args_with_prefix
+            urlpatterns_with_args += action_urlpatterns_with_args_with_prefix
         else:
-            urlpatterns+=action_urlpatterns
-            urlpatterns_with_args+=index_action_with_args_urlconf
+            urlpatterns += action_urlpatterns
+            urlpatterns_with_args += index_action_with_args_urlconf
 
-    return urlpatterns+urlpatterns_with_args
+    return urlpatterns + urlpatterns_with_args
 CACHED_ACTIONS = {}
 
 def get_action_name(func, with_prefix = False):
     if callable(func):
         func_name = func.__name__
         if not re.match(r'^[_\-A-Z0-9]',func_name[0]):
             if hasattr(func, 'action_name'):
@@ -360,15 +352,15 @@
 
         if hasattr(self, 'ignore_ajax'):
             warnings.warn("ActionController.ignore_ajax is deprecated, remove 2017-01-01", DeprecationWarning)
             self._no_ajax_prefix = getattr(self, 'ignore_ajax', False)
         else:
             self._no_ajax_prefix = getattr(self, 'no_ajax_prefix', False)
 
-        self._is_ajax = request.is_ajax()
+        self._is_ajax = is_ajax(request)
         self._url_params = url_params
 
         self._template_extension = getattr(self, 'template_extension', 'html')
 
         if getattr(self, 'template_prefix') is not None:
             self._template_prefix = getattr(self, 'template_prefix')
         else:
```

### Comparing `django-url-framework-0.5.3/django_url_framework/decorators/action_options.py` & `django-url-framework-0.6.0/django_url_framework/decorators/action_options.py`

 * *Files identical despite different names*

### Comparing `django-url-framework-0.5.3/django_url_framework/decorators/auth.py` & `django-url-framework-0.6.0/django_url_framework/decorators/auth.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 try:
     from functools import update_wrapper, wraps
 except ImportError:
     from django.utils.functional import update_wrapper, wraps  # Python 2.4 fallback.
 
 from django.contrib.auth import REDIRECT_FIELD_NAME
 from django.http import HttpResponseRedirect, HttpResponseForbidden
-from django.utils.http import urlquote
+from urllib.parse import quote
+
+from ..lib import is_ajax
 
 def user_passes_test(test_func, login_url=None, redirect_field_name=REDIRECT_FIELD_NAME):
     """
     Decorator for views that checks that the user passes the given test,
     redirecting to the log-in page if necessary. The test should be a callable
     that takes the user object and returns True if the user passes.
     """
@@ -18,17 +20,17 @@
         login_url = settings.LOGIN_URL
 
     def decorator(view_func):
         @wraps(view_func)
         def _wrapped_view(self, request, *args, **kwargs):
             if test_func(request.user):
                 return view_func(self, request, *args, **kwargs)
-            path = urlquote(request.get_full_path())
+            path = quote(request.get_full_path())
             tup = login_url, redirect_field_name, path
-            if request.is_ajax():
+            if is_ajax(request):
                 return HttpResponseForbidden()
             else:
                 return HttpResponseRedirect('%s?%s=%s' % tup)
         return _wrapped_view
     return decorator
 
 def must_be_member_of_group(group_name=None, redirect_field_name=REDIRECT_FIELD_NAME, login_url=None):
```

### Comparing `django-url-framework-0.5.3/django_url_framework/decorators/http_methods.py` & `django-url-framework-0.6.0/django_url_framework/decorators/http_methods.py`

 * *Files identical despite different names*

### Comparing `django-url-framework-0.5.3/django_url_framework/decorators/render.py` & `django-url-framework-0.6.0/django_url_framework/decorators/render.py`

 * *Files 7% similar despite different names*

```diff
@@ -14,19 +14,25 @@
             return getattr(self,renderer)(response, **renderer_kwargs)
         return _wrapped_action
     return decorator
 
 def json_action(json_encoder=None):
     """
     Decorator that ensures any data returned from this function is encoded into JSON.
+    Usage: @json_action() or @json_action(json_encoder=CustomJsonEncoder)
     """
     return _action_renderer(json_encoder=json_encoder, renderer="_as_json")
 
 def yaml_action(default_flow_style=None):
+    """
+    Usage: @yaml_action() or @yaml_action(default_flow_style=True)
 
+    :param default_flow_style:
+    :return:
+    """
     return _action_renderer(default_flow_style=default_flow_style, renderer="_as_yaml")
 
 
 def auto(json_encoder=None, yaml_default_flow_style=None):
     """
         Decorator that determines the returned data renderer based on the Accept header.
         Be careful, if used incorrectly this can expose your data to an attacker.
```

### Comparing `django-url-framework-0.5.3/django_url_framework/flash.py` & `django-url-framework-0.6.0/django_url_framework/flash.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from django.conf import settings
 import hashlib
-from django.utils.encoding import smart_text
+from django.utils.encoding import smart_str
 from django.utils.safestring import mark_safe
 
 class FlashMessage(object):
     def __init__(self, message, is_error=False, kind='normal'):
-        self.message = smart_text(message, encoding="utf8")
+        self.message = smart_str(message, encoding="utf8")
         self.is_error = is_error
         self.kind = kind
         self.digest = hashlib.sha1(self.message.encode('utf8') + kind.encode('utf8')).hexdigest()
     
     def hash(self):
         return self.digest
 
@@ -73,15 +73,15 @@
     
     def append_error(self, msg):
         self.append(msg=msg, msg_type='error')
         
     def append(self, msg, msg_type='normal'):
 
         new_message = FlashMessage(**{
-            'message': smart_text(msg, encoding="utf8"),
+            'message': smart_str(msg, encoding="utf8"),
             'kind': msg_type,
             'is_error': msg_type == 'error'
         })
         new_hash = new_message.hash()
 
         for message in self.messages:
             if message.hash() == new_hash:
```

### Comparing `django-url-framework-0.5.3/django_url_framework/helper.py` & `django-url-framework-0.6.0/django_url_framework/helper.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,10 @@
 from django.utils.http import urlencode
 
-#django <2 compat
-try:
-    from django.urls import reverse
-except ImportError:
-    from django.core.urlresolvers import reverse
+from django.urls import reverse
 
 from .exceptions import InvalidActionError
 from .exceptions import InvalidControllerError
 
 class ApplicationHelper(object):
     """ApplicationHelpers can contain functions useful in a controller. Each controller is assigned a helper.
     Either the global ApplicationHelper, or a class with the same name as the controller such as foo_helper.py,
```

### Comparing `django-url-framework-0.5.3/django_url_framework/renderers.py` & `django-url-framework-0.6.0/django_url_framework/renderers.py`

 * *Files identical despite different names*

### Comparing `django-url-framework-0.5.3/django_url_framework/site.py` & `django-url-framework-0.6.0/django_url_framework/site.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,22 @@
 import sys
 import inspect
 import logging
 import re
 import os
 import importlib
-import importlib.util
 
 from django.apps import apps
 
 from .helper import ApplicationHelper
 from .controller import ActionController
-from .controller import url_patterns
 from .controller import get_controller_name
 from .controller import get_controller_urlconf
 
-from django.conf.urls import include, url
+from django.urls import include, path
 
 class Site(object):
     def __init__(self):
         self.controllers = {}
         self.helpers = {}
         self.logger = logging.getLogger("django_url_framework")
         self._use_inflection_lib = False
@@ -154,13 +152,19 @@
             except ImportError:
                 self.logger.warning("Failed to find proper controller in %s" % controller_file, exc_info=True)
             finally:
                 if found_controller:
                     found_controller[0].close()
             
     def _get_urls(self):
-        urlpatterns = url_patterns()
-        
+        urlpatterns = []
+
         for controller_name, controller_class in list(self.controllers.items()):
-            urlpatterns += url_patterns(url(r'^%(controller)s/' % {'controller':controller_name}, include(get_controller_urlconf(controller_class, site=self))))
-        return urlpatterns, None, 'django-url-framework'
+            urlpatterns.append(
+                path("%(controller)s/" % {'controller': controller_name},
+                     include(
+                         get_controller_urlconf(controller_class, site=self)
+                     )
+                 )
+            )
+        return urlpatterns, 'django-url-framework', None
     urls = property(_get_urls)
```

### Comparing `django-url-framework-0.5.3/django_url_framework/templatetags/url_framework.py` & `django-url-framework-0.6.0/django_url_framework/templatetags/url_framework.py`

 * *Files identical despite different names*

### Comparing `django-url-framework-0.5.3/django_url_framework.egg-info/PKG-INFO` & `django-url-framework-0.6.0/django_url_framework.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,526 +1,529 @@
 Metadata-Version: 2.1
 Name: django-url-framework
-Version: 0.5.3
+Version: 0.6.0
 Summary: Automagically discover urls in a django application, similar to the Ruby on Rails Controller/Action/View implementation.
 Home-page: https://github.com/zeraien/django-url-framework/
 Author: Dimo Fedortchenko
 Author-email: d@angelhill.net
 License: MIT
-Description: The django-url-framework will help you get your django applications done faster.
-        
-        ![build](https://github.com/zeraien/django-url-framework/workflows/build/badge.svg)
-        [![Documentation Status](https://readthedocs.org/projects/django-url-framework/badge/?version=latest)](https://django-url-framework.readthedocs.io/en/latest/?badge=latest)
-        [![Join the chat at https://gitter.im/zeraien/django-url-framework](https://badges.gitter.im/zeraien/django-url-framework.svg)](https://gitter.im/zeraien/django-url-framework?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge)
-        
-        It automatically detects urls in a django application, similar to the way Ruby on Rails does it with the Controller-Action-View implementation.
-        
-        Controllers are created in each django application with a predefined file naming scheme (`foo_controller.py`) and extending `ActionController`. The `ActionController` contains methods often used in a web context, and does common request-related processing.
-        
-        Each application can have multiple controllers thus allowing for smaller classes in a larger application.
-        
-        Each function not starting with an underscore becomes it's own action. By simply returning a dictionary from the action, it will be rendered with the template named using the `controller/action.html` naming scheme.
-        
-        Each action and controller can override certain global settings such as using a custom template name or giving the action (or controller) a custom name.
-        
-        ## Install
-        
-        From pypi:
-        
-        ```
-        pip install django-url-framework
-        ```
-        
-        Alternatively just check out the source here and run `python setup.py install` or `pip install .`
-        
-        ## Add to your project
-        
-        ### settings.py
-        
-        ```python
-        INSTALLED_APPS = (
-          ...,
-          'django_url_framework',
-          ...
-        )
-        ```
-        ### urls.py
-        ```python
-        import django_url_framework
-        from django.conf import settings
-        from django.conf.urls import patterns, include
-        
-        django_url_framework.site.autodiscover(new_inflection_library=True)
-        
-        urlpatterns = patterns('',
-            (r'^', include(django_url_framework.site.urls) ),
-        )
-        ```
-        
-        ## Example
-        
-        ### Folder structure
-        
-        ```
-        project/
-          app/
-              cart_controller.py
-              id_controller.py
-              templates/
-                   cart/
-                      add.html
-                      index.html
-                      remove.html
-                   id_manager/
-                      bar.html
-        ```
-        
-        ### cart_controller.py 
-        
-        ```python
-        from django_url_framework.controller import ActionController
-        
-        class CartController(ActionController):
-            def edit(self, request, id = None):
-                return {}
-            def remove(self, request, id):
-                return {}
-            def index(self, request):
-              return {}
-        ```
-        
-        ### id_controller.py
-        
-        ```python
-        from django_url_framework.controller import ActionController
-        
-        class IDManagerController(ActionController):
-            def index(self, request, object_id = None):
-                return {}
-            def bar(self, request):
-                return {}
-            def bar__delete(self, request):
-                return {}
-        ```
-        
-        ### Result
-        
-        The following URLs will be created:
-        
-        ```
-        /cart/ <- will go to *index action*
-        /cart/(\w+)/
-        /cart/edit/
-        /cart/edit/(\w+)/
-        /cart/remove/(\w+)/
-        /foo/
-        /foo/(\w+)/
-        /foo/bar/
-        /foo/bar/delete/
-        ```
-        
-        You can easily access your URLs using django's built-in `{% url ... %}` tag. Simply call `{% url cart_index %}` or `{% url cart_delete id %}` and it will work as you would expect.
-        
-        There is also a helper tag for faster linking within the same controller.
-        `{% go_action remove %}` will take you to `/cart/remove/`. To use it, `{% load url_framework %}` in your templates.
-        
-        The names of the controller files do not affect your URLs, however, the files must have `_controller.py` suffix. The URL name of the controller is derived from the class name, minus the Controller part. You can also manually specify controller names using the `controller_name` attribute on the controller class.
-        
-        ### Controller names
-        
-        The controller name is derived from it's class name, by converting camelcase into underscores.
-        For instance `FooController` is simple `foo`, while `FooBarController` becomes `foo_bar`.
-        
-        The latest version uses the `inflection` library, however to avoid breaking old code, this is still optional until 2021.
-        
-        The biggest difference is that with `inflection`, `HTTPResponse` becomes `http_response`, while the old name would be `httpresponse`. I suggest enabling the `inflection` library for all new and existing projects. You can manually specify names for controllers whose name change would break your code, or disable the inflection library for those controllers using a flag.
-        
-        You can give the controller a custom name with the `controller_name` parameter:
-        ```python
-        class Controller(ActionController):
-          controller_name = "foo"
-        ```
-        
-        Enable or disable the use of the new `inflection` library using a flag
-        ```python
-        class Controller(ActionController):
-          use_inflection_library = True
-        ```
-        
-        ### Other useful controller settings
-        
-        ```python
-        class BarController(ActionController):
-            
-            # default filename extension for all templates
-            template_extension = "pug" 
-            
-            # will require every template file to start with this string
-            template_prefix = "foo_" 
-            
-            # will not look for templates in subdirectories, but in the root templates/ folder
-            no_subdirectories = False 
-            
-            # do not prefix templates with `_` (underscore) when they are called using an AJAX request
-            no_ajax_prefix = False 
-        
-            # Set a prefix for the controller's name, applies even if
-            # you set controller_name (template name is based on controller_name, sans prefix)
-            # NOTE: The urlconf name will not include the prefix, only the actual URL itself
-            # Thus: FooController.list will have the URL /prefixed_foo/list/, but the url name will be
-            # `foo_list`.
-            controller_prefix = "prefixed_" 
-            
-            # completely override the name of the controller
-            controller_name = "shopping_cart" 
-        
-            # When used with custom urlconf in actions, these arguments will not be passed to the action
-            # example: "/<id:int>/<skip:bool>/" Only `id` will be passed to the `action`, while `skip` will not be.
-            consume_urlconf_keyword_arguments = ['skip']
-        
-            # set a prefix for all the URLs in this controller
-            # So, what normally would be `/controller/action/`, becomes `^prefix/controller/action/`
-            urlconf_prefix:list = ["^prefix"]
-        
-            # A custom json encoder, subclassing JSONEncoder 
-            json_default_encoder:JSONEncoder = None
-        
-            # use the yaml default flow style
-            yaml_default_flow_style:bool = True
-        
-            # use the new inflection library to generate controller url
-            # if this is None, will use the global setting, otherwise override this on a per controller basis
-            use_inflection_library:Union[bool,None] = None
-        
-        ```
-        
-        ### Template filenames
-        
-        By default templates are stored in the subdirectory with the controller's name, and the templates are given the same filename as the action name.
-        If a request is determinned to be AJAX in nature, the template filename is prefixed with an underscore.
-        Example:
-        ```python
-        class FooController(ActionController):
-            def foo_action(self, request):
-              return {}
-        ```
-        
-        File structure:
-        ```python
-        /foo/foo_action.html
-        /foo/_foo_action.html <--- for AJAX requests.
-        ```
-        
-        You can disable this prefixing on a per action or per controller level.
-        
-        For all actions in a controller:
-        ```python
-        class FooController(ActionController):
-            no_ajax_prefix = True
-        ```
-        
-        For a single action:
-        ```python
-        from django_url_framework.decorators.action_options
-        class FooController(ActionController):
-            @no_ajax_prefix
-            def foo_action(self, request):
-              return {}
-        ```
-        
-        
-        ## Action names
-        
-        ```python
-        class FooController(ActionController):
-            def action(self, request):
-              return {}
-        ```
-        Creates the following URL:
-        ```
-        /controller/action/
-        ```
-        
-        Double underscores `__` in action names are converted to slashes in the urlconf, so: `action__name` becomes `/action/name/`.
-        
-        ```python
-        class Controller(ActionController):
-            def action__foo(self, request):
-              return {}
-        ```
-        Creates the following URL:
-        ```
-        /controller/action/foo/
-        ```
-        
-        
-        ### Decorate to name
-        
-        You can also decorate functions to give them different names and prefixes and urls. See decorator package for more details, here is an example:
-        ```python
-        @action_options.name("foo")
-        @action_options.prefix("prefix_")
-        def bar(self, request):
-          return {}
-        ```
-        will result in:
-        ```
-        /controller/prefix_foo/
-        ```
-        
-        The action will now have the template `/controller/foo.html`. Prefixes do not affect template naming.
-        
-        ## Action parameters
-        
-        Providing a third parameter to an action will create a URLconf for that parameter, like so:
-        ```python
-        def action(self, request, object_id):
-            return {}
-        ```
-        Will allow you to call that action with:
-        ```
-        /controller/action/(\w+)/ <--- parameter consisting of A-Za-z0-9_
-        ```
-        If you make the argument optional, an additional URLconf entry is created allowing you to call the action without the third argument.
-        ```python
-        def action(self, request, object_id = None):
-            return {}
-        ```
-        Results in:
-        
-        ```
-        /controller/action/
-        /controller/action/(\w+)/  <--- optional argument consisting of A-Za-z0-9_
-        ```
-        
-        ### Decorate for JSON, YAML or Automatic
-        
-        You can decorate any action to have a default renderer.
-        Instead of using `self._as_json` as before, you can just put a decorator like so:
-        
-        ```python
-        from django_url_framework.decorators import json_action
-            @json_action(json_encoder=None)
-            def action(self, request, year, month):
-                ...
-                return {}
-        ```
-        Other decorators include `@yaml_action(default_flow_style:bool)` and `@auto()`.
-        YaML is self-explanatory, however `@auto` is a bit interesting, it will automatically determine the renderer based on the `HTTP_ACCEPT` header. 
-        
-        *Warning* - if you expose raw data in your actions, that normally would be massaged inside a Server-Side template, DO NOT USE the `@auto` decorator as this allows an attacker to download raw data from your server.
-        However, if your responses are designed for an API, the `@auto` decorator will enable the API client to request data as it sees fit, for example, it can request a Server-Side rendered HTML, or the same data as JSON or YaML.
-        
-        Here is a list of supported renderers:
-        - text/html - `TemplateRenderer` - renders using the appropriate Django template
-        - text/plain - `TextRenderer` - prints text data as is, or prints object types using `pprint.pformat`
-        - application/json - `JSONRenderer` - renders data as JSON
-        - application/yaml - `YamlRenderer` - renders data as YaML
-        
-        `@auto()` accepts the following parameters:
-        - json_encoder
-        - yaml_default_flow_style
-        The work the same as if passed to `@json_action()` or `@yaml_action()`
-        
-        ### Set HTTP Status Codes easily
-        
-        Any action can return a tuple of two items, the second item should be an `int` and will become the HTTP status code for your response.
-        
-        ```python
-            @json_action()
-            def update(self, request, year, month):
-                ...
-                return False, 304 #not modified
-        
-            @json_action()
-            def create(self, request, year, month):
-                ...
-                return True, 201 #created
-        ```
-        
-        ### Decorate for custom parameters
-        
-        You can also create your own custom parameters by using the `@url_parameters` decorator to the function.
-        ```python
-        from django_url_framework.decorators.action_options import url_paramters
-        class Controller(ActionController):
-            @url_parameters(r'(?P<year>\d{4})/(?P<month>\d\d)')
-            def action(self, request, year, month):
-                ...
-                return {}
-        ```
-        The above will create the following url patterns:
-        ```
-        /controller/action/(?P<year>\d{4})/(?P<month>\d\d)
-        ```
-        *Note the lack of trailing slash - you must provide this yourself.*
-        
-        ### Custom url for any action
-        
-        You can write your own urlconf for each action, by decorating it with `@urlconf`.
-        ```python
-        from django_url_framework.decorators.action_options import urlconf
-        class Controller(ActionController):
-            @action_options.urlconf([
-                    r'^bar/(?P<year>\d{4})/$',
-                    r'^bar/(?P<year>\d{4})/(?P<month>\d\d)/$',
-                    r'^foo/(?P<year>\d{4})/(?P<month>\d\d)/(?P<day>\d\d)/$'
-                ],
-                do_not_autogenerate=True)
-            def action(self, request, year, month=None, day=None):
-                ...
-                return {}
-        ```
-        The above will create the following url patterns:
-        ```
-        /controller/bar/(?P<year>\d{4})/
-        /controller/bar/(?P<year>\d{4})/(?P<month>\d\d)/$
-        /controller/foo/(?P<year>\d{4})/(?P<month>\d\d)/(?P<day>\d\d)/$
-        ```
-        
-        The `do_not_autogenerate` argument is **true** by default and will prevent any urls for this action
-        from being autogenerated. If `do_not_autogenerate` were to be set to false in the example below,
-        the following url would also be created:
-        ```
-        /controller/action/
-        ```
-        This URL would not actually work since the `year` argument is required the `action` function.
-        
-        ## Flash messages
-        
-        The ActionController also has a `_flash` instance variable that allows you to send messages to the user that can survive a redirect. Simply use 
-        
-        ```python
-        self._flash.append("Message")
-        
-        self._flash.error("Error message")
-        ```
-        
-        The flash messages can be either messages or error messages. The flash object is automatically exported into the context and you can use it as such:
-        
-        ```HTML+Django
-        {% if flash.has_messages %}
-          {% for message in flash.get_and_clear %}
-        
-              {% if message.is_error %}<span class='icon-error'></span>{% endif %}
-        
-              <p class="{{message.type}}">{{message}}</p>
-              
-          {% endfor %}
-        {% endif }
-        ```
-        
-        ## Before and After each action
-        
-        You can override `_before_filter` and/or `_after_filter` to perform certain actions and checks before or after an action. Read more in `ActionController` docs.
-        
-        These methods accept the "request" parameter which is an HTTP request object for this request.
-        
-        ```python
-        class AccountController(ActionController):
-        
-            def _before_filter(self, request):
-                campaign_id = request.GET.get("campaign_id")
-                try:
-                  self._campaign = Campaign.objects.get(pk=campaign_id)
-                except Campaign.DoesNotExist:
-                  self._campaign = None
-        ```
-        
-        You can disable the before and after filters by decorating any action with the `@disable_filters` decorator.
-        
-        Example:
-        ```python
-        from django_url_framework.decorators.action_options import disable_filters
-        @disable_filters
-        def action(self, request):
-          return {}
-        ```
-        
-        One of the great features of django url framework is that you can require login for all actions in a controller by simply decorating the before_filter with a decorator to require logging in, see next section!
-        
-        ## Authentication
-        
-        To require login on an action use the `@login_required` decorator provided by django-url-framework. The decorator also works on `_before_filter`.
-        
-        ```python
-        from django_url_framework.decorators import login_required
-        class AccountController(ActionController):
-        
-            @login_required
-            def action(self, request):
-                return {}
-        ```
-        
-        If the user isn’t logged in, redirect to `settings.LOGIN_URL`, passing the current absolute path in the query string. Example: `/accounts/login/?next=/polls/3/`.
-        `login_required()` also takes an optional `login_url` parameter. Example:
-        
-        ```python
-        from django_url_framework.decorators import login_required
-        class AccountController(ActionController):
-        
-            @login_required(login_url="/login/")
-            def action(self, request):
-                return {}
-        ```
-        
-        By default, the path that the user should be redirected to upon successful authentication is stored in a query string parameter called "next". If you would prefer to use a different name for this parameter, `login_required()` takes an optional `redirect_field_name` parameter.
-        
-        Additionally you can use `@superuser_required`, `@permission_required(permission_instance)` and `@must_be_member_of_group(group_name="some_group")`.
-        
-        Another example makes it easy to limiting access to a subset of data based on the logged in user for the whole controller.
-        
-        ```python
-        from django_url_framework.decorators import login_required
-        class ItemController(ActionController):
-            @login_required()
-            def _before_filter(self):
-                self.my_items = Item.objects.filter(user=request.user)
-                self.my_products = Product.objects.filter(item__in=self.my_items)
-                return {
-                    "page_title": "Item Page"
-                }
-            def item(self, request, pk):
-                item = get_object_or_404(self.my_items, pk=pk)
-                return {"item":item}
-            def product(self, request, pk):
-                item = get_object_or_404(self.my_products, pk=pk)
-                return {"product":product}
-        
-        
-        ```
-        
-        ## Only POST? (or GET or anything...)
-        You can limit what http methods a function can be called with.
-        
-        The example below limits the `update` action to only **POST** and **DELETE** http methods.
-        
-        ```python
-        from django_url_framework.decorators import http_methods
-        class Controller(ActionController):
-            @http_methods.POST
-            @http_methods.DELETE
-            def update(self, request):
-                return {}
-        ```
-        
-        By default all actions can be called with all http methods.
-        
-        ## Custom template extensions
-        When using jade or something similar you can specify a custom extension for all templates in the controller.
-        
-        ```python
-        class FooController(ActionController):
-            #custom extension for all templates in this controller
-            template_extension = "jade"
-        ```
-        
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Utilities
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+The django-url-framework will help you get your django applications done faster.
+
+![build](https://github.com/zeraien/django-url-framework/workflows/build/badge.svg)
+[![Documentation Status](https://readthedocs.org/projects/django-url-framework/badge/?version=latest)](https://django-url-framework.readthedocs.io/en/latest/?badge=latest)
+[![Join the chat at https://gitter.im/zeraien/django-url-framework](https://badges.gitter.im/zeraien/django-url-framework.svg)](https://gitter.im/zeraien/django-url-framework?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge)
+
+It automatically detects urls in a django application, similar to the way Ruby on Rails does it with the Controller-Action-View implementation.
+
+Controllers are created in each django application with a predefined file naming scheme (`foo_controller.py`) and extending `ActionController`. The `ActionController` contains methods often used in a web context, and does common request-related processing.
+
+Each application can have multiple controllers thus allowing for smaller classes in a larger application.
+
+Each function not starting with an underscore becomes it's own action. By simply returning a dictionary from the action, it will be rendered with the template named using the `controller/action.html` naming scheme.
+
+Each action and controller can override certain global settings such as using a custom template name or giving the action (or controller) a custom name.
+
+## Install
+
+From pypi:
+
+```
+pip install django-url-framework
+```
+
+Alternatively just check out the source here and run `python setup.py install` or `pip install .`
+
+## Add to your project
+
+### settings.py
+
+```python
+INSTALLED_APPS = (
+  ...,
+  'django_url_framework',
+  ...
+)
+```
+### urls.py
+```python
+import django_url_framework
+from django.conf import settings
+from django.conf.urls import patterns, include
+
+django_url_framework.site.autodiscover(new_inflection_library=True)
+
+urlpatterns = patterns('',
+    (r'^', include(django_url_framework.site.urls) ),
+)
+```
+
+## Example
+
+### Folder structure
+
+```
+project/
+  app/
+      cart_controller.py
+      id_controller.py
+      templates/
+           cart/
+              add.html
+              index.html
+              remove.html
+           id_manager/
+              bar.html
+```
+
+### cart_controller.py 
+
+```python
+from django_url_framework.controller import ActionController
+
+class CartController(ActionController):
+    def edit(self, request, id = None):
+        return {}
+    def remove(self, request, id):
+        return {}
+    def index(self, request):
+      return {}
+```
+
+### id_controller.py
+
+```python
+from django_url_framework.controller import ActionController
+
+class IDManagerController(ActionController):
+    def index(self, request, object_id = None):
+        return {}
+    def bar(self, request):
+        return {}
+    def bar__delete(self, request):
+        return {}
+```
+
+### Result
+
+The following URLs will be created:
+
+```
+/cart/ <- will go to *index action*
+/cart/(\w+)/
+/cart/edit/
+/cart/edit/(\w+)/
+/cart/remove/(\w+)/
+/foo/
+/foo/(\w+)/
+/foo/bar/
+/foo/bar/delete/
+```
+
+You can easily access your URLs using django's built-in `{% url ... %}` tag. Simply call `{% url cart_index %}` or `{% url cart_delete id %}` and it will work as you would expect.
+
+There is also a helper tag for faster linking within the same controller.
+`{% go_action remove %}` will take you to `/cart/remove/`. To use it, `{% load url_framework %}` in your templates.
+
+The names of the controller files do not affect your URLs, however, the files must have `_controller.py` suffix. The URL name of the controller is derived from the class name, minus the Controller part. You can also manually specify controller names using the `controller_name` attribute on the controller class.
+
+### Controller names
+
+The controller name is derived from it's class name, by converting camelcase into underscores.
+For instance `FooController` is simple `foo`, while `FooBarController` becomes `foo_bar`.
+
+The latest version uses the `inflection` library, however to avoid breaking old code, this is still optional until 2021.
+
+The biggest difference is that with `inflection`, `HTTPResponse` becomes `http_response`, while the old name would be `httpresponse`. I suggest enabling the `inflection` library for all new and existing projects. You can manually specify names for controllers whose name change would break your code, or disable the inflection library for those controllers using a flag.
+
+You can give the controller a custom name with the `controller_name` parameter:
+```python
+class Controller(ActionController):
+  controller_name = "foo"
+```
+
+Enable or disable the use of the new `inflection` library using a flag
+```python
+class Controller(ActionController):
+  use_inflection_library = True
+```
+
+### Other useful controller settings
+
+```python
+class BarController(ActionController):
+    
+    # default filename extension for all templates
+    template_extension = "pug" 
+    
+    # will require every template file to start with this string
+    template_prefix = "foo_" 
+    
+    # will not look for templates in subdirectories, but in the root templates/ folder
+    no_subdirectories = False 
+    
+    # do not prefix templates with `_` (underscore) when they are called using an AJAX request
+    no_ajax_prefix = False 
+
+    # Set a prefix for the controller's name, applies even if
+    # you set controller_name (template name is based on controller_name, sans prefix)
+    # NOTE: The urlconf name will not include the prefix, only the actual URL itself
+    # Thus: FooController.list will have the URL /prefixed_foo/list/, but the url name will be
+    # `foo_list`.
+    controller_prefix = "prefixed_" 
+    
+    # completely override the name of the controller
+    controller_name = "shopping_cart" 
+
+    # When used with custom urlconf in actions, these arguments will not be passed to the action
+    # example: "/<id:int>/<skip:bool>/" Only `id` will be passed to the `action`, while `skip` will not be.
+    consume_urlconf_keyword_arguments = ['skip']
+
+    # set a prefix for all the URLs in this controller
+    # So, what normally would be `/controller/action/`, becomes `^prefix/controller/action/`
+    urlconf_prefix:list = ["^prefix"]
+
+    # A custom json encoder, subclassing JSONEncoder 
+    json_default_encoder:JSONEncoder = None
+
+    # use the yaml default flow style
+    yaml_default_flow_style:bool = True
+
+    # use the new inflection library to generate controller url
+    # if this is None, will use the global setting, otherwise override this on a per controller basis
+    use_inflection_library:Union[bool,None] = None
+
+```
+
+### Template filenames
+
+By default templates are stored in the subdirectory with the controller's name, and the templates are given the same filename as the action name.
+If a request is determinned to be AJAX in nature, the template filename is prefixed with an underscore.
+Example:
+```python
+class FooController(ActionController):
+    def foo_action(self, request):
+      return {}
+```
+
+File structure:
+```python
+/foo/foo_action.html
+/foo/_foo_action.html <--- for AJAX requests.
+```
+
+You can disable this prefixing on a per action or per controller level.
+
+For all actions in a controller:
+```python
+class FooController(ActionController):
+    no_ajax_prefix = True
+```
+
+For a single action:
+```python
+from django_url_framework.decorators.action_options
+class FooController(ActionController):
+    @no_ajax_prefix
+    def foo_action(self, request):
+      return {}
+```
+
+
+## Action names
+
+```python
+class FooController(ActionController):
+    def action(self, request):
+      return {}
+```
+Creates the following URL:
+```
+/controller/action/
+```
+
+Double underscores `__` in action names are converted to slashes in the urlconf, so: `action__name` becomes `/action/name/`.
+
+```python
+class Controller(ActionController):
+    def action__foo(self, request):
+      return {}
+```
+Creates the following URL:
+```
+/controller/action/foo/
+```
+
+
+### Decorate to name
+
+You can also decorate functions to give them different names and prefixes and urls. See decorator package for more details, here is an example:
+```python
+@action_options.name("foo")
+@action_options.prefix("prefix_")
+def bar(self, request):
+  return {}
+```
+will result in:
+```
+/controller/prefix_foo/
+```
+
+The action will now have the template `/controller/foo.html`. Prefixes do not affect template naming.
+
+## Action parameters
+
+Providing a third parameter to an action will create a URLconf for that parameter, like so:
+```python
+def action(self, request, object_id):
+    return {}
+```
+Will allow you to call that action with:
+```
+/controller/action/(\w+)/ <--- parameter consisting of A-Za-z0-9_
+```
+If you make the argument optional, an additional URLconf entry is created allowing you to call the action without the third argument.
+```python
+def action(self, request, object_id = None):
+    return {}
+```
+Results in:
+
+```
+/controller/action/
+/controller/action/(\w+)/  <--- optional argument consisting of A-Za-z0-9_
+```
+
+### Decorate for JSON, YAML or Automatic
+
+You can decorate any action to have a default renderer.
+Instead of using `self._as_json` as before, you can just put a decorator like so:
+
+```python
+from django_url_framework.decorators import json_action
+    @json_action(json_encoder=None)
+    def action(self, request, year, month):
+        ...
+        return {}
+```
+Other decorators include `@yaml_action(default_flow_style:bool)` and `@auto()`.
+YaML is self-explanatory, however `@auto` is a bit interesting, it will automatically determine the renderer based on the `HTTP_ACCEPT` header. 
+
+*Warning* - if you expose raw data in your actions, that normally would be massaged inside a Server-Side template, DO NOT USE the `@auto` decorator as this allows an attacker to download raw data from your server.
+However, if your responses are designed for an API, the `@auto` decorator will enable the API client to request data as it sees fit, for example, it can request a Server-Side rendered HTML, or the same data as JSON or YaML.
+
+Here is a list of supported renderers:
+- text/html - `TemplateRenderer` - renders using the appropriate Django template
+- text/plain - `TextRenderer` - prints text data as is, or prints object types using `pprint.pformat`
+- application/json - `JSONRenderer` - renders data as JSON
+- application/yaml - `YamlRenderer` - renders data as YaML
+
+`@auto()` accepts the following parameters:
+- json_encoder
+- yaml_default_flow_style
+The work the same as if passed to `@json_action()` or `@yaml_action()`
+
+### Set HTTP Status Codes easily
+
+Any action can return a tuple of two items, the second item should be an `int` and will become the HTTP status code for your response.
+
+```python
+    @json_action()
+    def update(self, request, year, month):
+        ...
+        return False, 304 #not modified
+
+    @json_action()
+    def create(self, request, year, month):
+        ...
+        return True, 201 #created
+```
+
+### Decorate for custom parameters
+
+You can also create your own custom parameters by using the `@url_parameters` decorator to the function.
+```python
+from django_url_framework.decorators.action_options import url_paramters
+class Controller(ActionController):
+    @url_parameters(r'(?P<year>\d{4})/(?P<month>\d\d)')
+    def action(self, request, year, month):
+        ...
+        return {}
+```
+The above will create the following url patterns:
+```
+/controller/action/(?P<year>\d{4})/(?P<month>\d\d)
+```
+*Note the lack of trailing slash - you must provide this yourself.*
+
+### Custom url for any action
+
+You can write your own urlconf for each action, by decorating it with `@urlconf`.
+```python
+from django_url_framework.decorators.action_options import urlconf
+class Controller(ActionController):
+    @action_options.urlconf([
+            r'^bar/(?P<year>\d{4})/$',
+            r'^bar/(?P<year>\d{4})/(?P<month>\d\d)/$',
+            r'^foo/(?P<year>\d{4})/(?P<month>\d\d)/(?P<day>\d\d)/$'
+        ],
+        do_not_autogenerate=True)
+    def action(self, request, year, month=None, day=None):
+        ...
+        return {}
+```
+The above will create the following url patterns:
+```
+/controller/bar/(?P<year>\d{4})/
+/controller/bar/(?P<year>\d{4})/(?P<month>\d\d)/$
+/controller/foo/(?P<year>\d{4})/(?P<month>\d\d)/(?P<day>\d\d)/$
+```
+
+The `do_not_autogenerate` argument is **true** by default and will prevent any urls for this action
+from being autogenerated. If `do_not_autogenerate` were to be set to false in the example below,
+the following url would also be created:
+```
+/controller/action/
+```
+This URL would not actually work since the `year` argument is required the `action` function.
+
+## Flash messages
+
+The ActionController also has a `_flash` instance variable that allows you to send messages to the user that can survive a redirect. Simply use 
+
+```python
+self._flash.append("Message")
+
+self._flash.error("Error message")
+```
+
+The flash messages can be either messages or error messages. The flash object is automatically exported into the context and you can use it as such:
+
+```HTML+Django
+{% if flash.has_messages %}
+  {% for message in flash.get_and_clear %}
+
+      {% if message.is_error %}<span class='icon-error'></span>{% endif %}
+
+      <p class="{{message.type}}">{{message}}</p>
+      
+  {% endfor %}
+{% endif }
+```
+
+## Before and After each action
+
+You can override `_before_filter` and/or `_after_filter` to perform certain actions and checks before or after an action. Read more in `ActionController` docs.
+
+These methods accept the "request" parameter which is an HTTP request object for this request.
+
+```python
+class AccountController(ActionController):
+
+    def _before_filter(self, request):
+        campaign_id = request.GET.get("campaign_id")
+        try:
+          self._campaign = Campaign.objects.get(pk=campaign_id)
+        except Campaign.DoesNotExist:
+          self._campaign = None
+```
+
+You can disable the before and after filters by decorating any action with the `@disable_filters` decorator.
+
+Example:
+```python
+from django_url_framework.decorators.action_options import disable_filters
+@disable_filters
+def action(self, request):
+  return {}
+```
+
+One of the great features of django url framework is that you can require login for all actions in a controller by simply decorating the before_filter with a decorator to require logging in, see next section!
+
+## Authentication
+
+To require login on an action use the `@login_required` decorator provided by django-url-framework. The decorator also works on `_before_filter`.
+
+```python
+from django_url_framework.decorators import login_required
+class AccountController(ActionController):
+
+    @login_required
+    def action(self, request):
+        return {}
+```
+
+If the user isn’t logged in, redirect to `settings.LOGIN_URL`, passing the current absolute path in the query string. Example: `/accounts/login/?next=/polls/3/`.
+`login_required()` also takes an optional `login_url` parameter. Example:
+
+```python
+from django_url_framework.decorators import login_required
+class AccountController(ActionController):
+
+    @login_required(login_url="/login/")
+    def action(self, request):
+        return {}
+```
+
+By default, the path that the user should be redirected to upon successful authentication is stored in a query string parameter called "next". If you would prefer to use a different name for this parameter, `login_required()` takes an optional `redirect_field_name` parameter.
+
+Additionally you can use `@superuser_required`, `@permission_required(permission_instance)` and `@must_be_member_of_group(group_name="some_group")`.
+
+Another example makes it easy to limiting access to a subset of data based on the logged in user for the whole controller.
+
+```python
+from django_url_framework.decorators import login_required
+class ItemController(ActionController):
+    @login_required()
+    def _before_filter(self):
+        self.my_items = Item.objects.filter(user=request.user)
+        self.my_products = Product.objects.filter(item__in=self.my_items)
+        return {
+            "page_title": "Item Page"
+        }
+    def item(self, request, pk):
+        item = get_object_or_404(self.my_items, pk=pk)
+        return {"item":item}
+    def product(self, request, pk):
+        item = get_object_or_404(self.my_products, pk=pk)
+        return {"product":product}
+
+
+```
+
+## Only POST? (or GET or anything...)
+You can limit what http methods a function can be called with.
+
+The example below limits the `update` action to only **POST** and **DELETE** http methods.
+
+```python
+from django_url_framework.decorators import http_methods
+class Controller(ActionController):
+    @http_methods.POST
+    @http_methods.DELETE
+    def update(self, request):
+        return {}
+```
+
+By default all actions can be called with all http methods.
+
+## Custom template extensions
+When using jade or something similar you can specify a custom extension for all templates in the controller.
+
+```python
+class FooController(ActionController):
+    #custom extension for all templates in this controller
+    template_extension = "jade"
+```
+
+
```

### Comparing `django-url-framework-0.5.3/django_url_framework.egg-info/SOURCES.txt` & `django-url-framework-0.6.0/django_url_framework.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 setup.py
 django_url_framework/__init__.py
 django_url_framework/apps.py
 django_url_framework/controller.py
 django_url_framework/exceptions.py
 django_url_framework/flash.py
 django_url_framework/helper.py
+django_url_framework/lib.py
 django_url_framework/renderers.py
 django_url_framework/site.py
 django_url_framework.egg-info/PKG-INFO
 django_url_framework.egg-info/SOURCES.txt
 django_url_framework.egg-info/dependency_links.txt
 django_url_framework.egg-info/pbr.json
 django_url_framework.egg-info/top_level.txt
```

### Comparing `django-url-framework-0.5.3/setup.py` & `django-url-framework-0.6.0/setup.py`

 * *Files identical despite different names*

### Comparing `django-url-framework-0.5.3/tests/duf_test_case.py` & `django-url-framework-0.6.0/tests/duf_test_case.py`

 * *Files identical despite different names*

### Comparing `django-url-framework-0.5.3/tests/test_controller_action_renderers.py` & `django-url-framework-0.6.0/tests/test_controller_action_renderers.py`

 * *Files identical despite different names*

### Comparing `django-url-framework-0.5.3/tests/test_get_actions.py` & `django-url-framework-0.6.0/tests/test_get_actions.py`

 * *Files identical despite different names*

### Comparing `django-url-framework-0.5.3/tests/test_name_generation.py` & `django-url-framework-0.6.0/tests/test_name_generation.py`

 * *Files identical despite different names*

### Comparing `django-url-framework-0.5.3/tests/test_renderer_decorators.py` & `django-url-framework-0.6.0/tests/test_renderer_decorators.py`

 * *Files identical despite different names*

