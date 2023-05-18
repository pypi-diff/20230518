# Comparing `tmp/flasgger-0.9.7.1.tar.gz` & `tmp/flasgger-0.9.7b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flasgger-0.9.7.1.tar", last modified: Thu May 18 17:14:52 2023, max compression
+gzip compressed data, was "flasgger-0.9.7b2.tar", last modified: Thu May 11 17:50:36 2023, max compression
```

## Comparing `flasgger-0.9.7.1.tar` & `flasgger-0.9.7b2.tar`

### file list

```diff
@@ -1,354 +1,354 @@
-drwxr-xr-x   0 zixuanrao   (501) staff       (20)        0 2023-05-18 17:14:52.259262 flasgger-0.9.7.1/
--rw-r--r--   0 zixuanrao   (501) staff       (20)     3218 2020-12-23 09:11:59.000000 flasgger-0.9.7.1/CODE_OF_CONDUCT.md
--rw-r--r--   0 zixuanrao   (501) staff       (20)     1078 2020-12-23 09:11:59.000000 flasgger-0.9.7.1/LICENSE
--rw-r--r--   0 zixuanrao   (501) staff       (20)     1023 2020-12-23 09:11:59.000000 flasgger-0.9.7.1/MANIFEST.in
--rw-r--r--   0 zixuanrao   (501) staff       (20)    28508 2023-05-18 17:14:52.259422 flasgger-0.9.7.1/PKG-INFO
--rw-r--r--   0 zixuanrao   (501) staff       (20)    28035 2023-05-18 17:11:43.000000 flasgger-0.9.7.1/README.md
--rw-r--r--   0 zixuanrao   (501) staff       (20)    23841 2023-05-05 16:18:04.000000 flasgger-0.9.7.1/README.zh.md
-drwxr-xr-x   0 zixuanrao   (501) staff       (20)        0 2023-05-18 17:14:52.104139 flasgger-0.9.7.1/demo_app/
--rw-r--r--   0 zixuanrao   (501) staff       (20)      213 2020-12-23 09:11:59.000000 flasgger-0.9.7.1/demo_app/README.md
--rw-r--r--   0 zixuanrao   (501) staff       (20)        0 2020-12-23 09:11:59.000000 flasgger-0.9.7.1/demo_app/__init__.py
--rw-r--r--   0 zixuanrao   (501) staff       (20)     1607 2020-12-23 09:19:56.000000 flasgger-0.9.7.1/demo_app/app.py
--rw-r--r--   0 zixuanrao   (501) staff       (20)       53 2020-12-23 09:11:59.000000 flasgger-0.9.7.1/demo_app/requirements.txt
-drwxr-xr-x   0 zixuanrao   (501) staff       (20)        0 2023-05-18 17:14:52.111952 flasgger-0.9.7.1/demo_app/templates/
--rw-r--r--   0 zixuanrao   (501) staff       (20)     5095 2020-12-23 09:11:59.000000 flasgger-0.9.7.1/demo_app/templates/flasgger.html
--rw-r--r--   0 zixuanrao   (501) staff       (20)       97 2020-12-23 09:11:59.000000 flasgger-0.9.7.1/demo_app/templates/index.html
--rw-r--r--   0 zixuanrao   (501) staff       (20)       23 2020-12-23 09:11:59.000000 flasgger-0.9.7.1/demo_app/update.sh
-drwxr-xr-x   0 zixuanrao   (501) staff       (20)        0 2023-05-18 17:14:52.112237 flasgger-0.9.7.1/etc/
--rw-r--r--   0 zixuanrao   (501) staff       (20)     6148 2022-11-01 14:07:16.000000 flasgger-0.9.7.1/etc/.DS_Store
-drwxr-xr-x   0 zixuanrao   (501) staff       (20)        0 2023-05-18 17:14:52.113031 flasgger-0.9.7.1/etc/flasgger_package/
--rw-r--r--   0 zixuanrao   (501) staff       (20)       37 2020-12-23 09:11:59.000000 flasgger-0.9.7.1/etc/flasgger_package/MANIFEST.in
-drwxr-xr-x   0 zixuanrao   (501) staff       (20)        0 2023-05-18 17:14:52.093567 flasgger-0.9.7.1/etc/flasgger_package/build/
-drwxr-xr-x   0 zixuanrao   (501) staff       (20)        0 2023-05-18 17:14:52.093641 flasgger-0.9.7.1/etc/flasgger_package/build/lib/
-drwxr-xr-x   0 zixuanrao   (501) staff       (20)        0 2023-05-18 17:14:52.114044 flasgger-0.9.7.1/etc/flasgger_package/build/lib/flasgger_package/
--rw-r--r--   0 zixuanrao   (501) staff       (20)      161 2020-12-23 09:11:59.000000 flasgger-0.9.7.1/etc/flasgger_package/build/lib/flasgger_package/__init__.py
--rw-r--r--   0 zixuanrao   (501) staff       (20)      574 2020-12-23 09:11:59.000000 flasgger-0.9.7.1/etc/flasgger_package/build/lib/flasgger_package/package_specs.yml
--rw-r--r--   0 zixuanrao   (501) staff       (20)       80 2020-12-23 09:11:59.000000 flasgger-0.9.7.1/etc/flasgger_package/build/lib/flasgger_package/parameters.yml
-drwxr-xr-x   0 zixuanrao   (501) staff       (20)        0 2023-05-18 17:14:52.115524 flasgger-0.9.7.1/etc/flasgger_package/dist/
--rw-r--r--   0 zixuanrao   (501) staff       (20)     2533 2023-05-10 17:09:06.000000 flasgger-0.9.7.1/etc/flasgger_package/dist/flasgger_package-0.0.1-py3.11.egg
--rw-r--r--   0 zixuanrao   (501) staff       (20)     2002 2020-12-23 10:44:18.000000 flasgger-0.9.7.1/etc/flasgger_package/dist/flasgger_package-0.0.1-py3.8.egg
--rw-r--r--   0 zixuanrao   (501) staff       (20)     2444 2023-05-10 17:44:25.000000 flasgger-0.9.7.1/etc/flasgger_package/dist/flasgger_package-0.0.1-py3.9.egg
-drwxr-xr-x   0 zixuanrao   (501) staff       (20)        0 2023-05-18 17:14:52.116535 flasgger-0.9.7.1/etc/flasgger_package/flasgger_package/
--rw-r--r--   0 zixuanrao   (501) staff       (20)      161 2020-12-23 09:11:59.000000 flasgger-0.9.7.1/etc/flasgger_package/flasgger_package/__init__.py
--rw-r--r--   0 zixuanrao   (501) staff       (20)      574 2020-12-23 09:11:59.000000 flasgger-0.9.7.1/etc/flasgger_package/flasgger_package/package_specs.yml
--rw-r--r--   0 zixuanrao   (501) staff       (20)       80 2020-12-23 09:11:59.000000 flasgger-0.9.7.1/etc/flasgger_package/flasgger_package/parameters.yml
-drwxr-xr-x   0 zixuanrao   (501) staff       (20)        0 2023-05-18 17:14:52.118852 flasgger-0.9.7.1/etc/flasgger_package/flasgger_package.egg-info/
--rw-r--r--   0 zixuanrao   (501) staff       (20)      247 2023-05-10 17:44:25.000000 flasgger-0.9.7.1/etc/flasgger_package/flasgger_package.egg-info/PKG-INFO
--rw-r--r--   0 zixuanrao   (501) staff       (20)      354 2023-05-10 17:44:25.000000 flasgger-0.9.7.1/etc/flasgger_package/flasgger_package.egg-info/SOURCES.txt
--rw-r--r--   0 zixuanrao   (501) staff       (20)        1 2023-05-10 17:44:25.000000 flasgger-0.9.7.1/etc/flasgger_package/flasgger_package.egg-info/dependency_links.txt
--rw-r--r--   0 zixuanrao   (501) staff       (20)        1 2020-12-23 09:21:46.000000 flasgger-0.9.7.1/etc/flasgger_package/flasgger_package.egg-info/not-zip-safe
--rw-r--r--   0 zixuanrao   (501) staff       (20)       21 2023-05-10 17:44:25.000000 flasgger-0.9.7.1/etc/flasgger_package/flasgger_package.egg-info/requires.txt
--rw-r--r--   0 zixuanrao   (501) staff       (20)       17 2023-05-10 17:44:25.000000 flasgger-0.9.7.1/etc/flasgger_package/flasgger_package.egg-info/top_level.txt
--rw-r--r--   0 zixuanrao   (501) staff       (20)      550 2020-12-23 09:11:59.000000 flasgger-0.9.7.1/etc/flasgger_package/setup.py
-drwxr-xr-x   0 zixuanrao   (501) staff       (20)        0 2023-05-18 17:14:52.119115 flasgger-0.9.7.1/etc/pythonanywhere/
--rw-r--r--   0 zixuanrao   (501) staff       (20)     1858 2020-12-23 09:11:59.000000 flasgger-0.9.7.1/etc/pythonanywhere/pythonanywhere_com_wsgi.py
-drwxr-xr-x   0 zixuanrao   (501) staff       (20)        0 2023-05-18 17:14:52.137264 flasgger-0.9.7.1/examples/
--rw-r--r--   0 zixuanrao   (501) staff       (20)     1176 2020-12-23 09:11:59.000000 flasgger-0.9.7.1/examples/README.md
--rw-r--r--   0 zixuanrao   (501) staff       (20)        0 2020-12-23 09:11:59.000000 flasgger-0.9.7.1/examples/__init__.py
-drwxr-xr-x   0 zixuanrao   (501) staff       (20)        0 2023-05-18 17:14:52.170966 flasgger-0.9.7.1/examples/__pycache__/
--rw-r--r--   0 zixuanrao   (501) staff       (20)      171 2023-05-10 16:57:35.000000 flasgger-0.9.7.1/examples/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0 zixuanrao   (501) staff       (20)      153 2023-05-10 17:28:14.000000 flasgger-0.9.7.1/examples/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 zixuanrao   (501) staff       (20)     3434 2023-05-10 17:09:08.000000 flasgger-0.9.7.1/examples/__pycache__/apispec_example.cpython-311.pyc
--rw-r--r--   0 zixuanrao   (501) staff       (20)     2369 2023-05-10 17:29:26.000000 flasgger-0.9.7.1/examples/__pycache__/apispec_example.cpython-39.pyc
--rw-r--r--   0 zixuanrao   (501) staff       (20)     2773 2023-05-10 17:09:08.000000 flasgger-0.9.7.1/examples/__pycache__/apispec_example_uiversion3.cpython-311.pyc
--rw-r--r--   0 zixuanrao   (501) staff       (20)     1830 2023-05-10 17:29:26.000000 flasgger-0.9.7.1/examples/__pycache__/apispec_example_uiversion3.cpython-39.pyc
--rw-r--r--   0 zixuanrao   (501) staff       (20)     2849 2023-05-10 17:09:08.000000 flasgger-0.9.7.1/examples/__pycache__/base_model_view.cpython-311.pyc
--rw-r--r--   0 zixuanrao   (501) staff       (20)     2222 2023-05-10 17:29:26.000000 flasgger-0.9.7.1/examples/__pycache__/base_model_view.cpython-39.pyc
--rw-r--r--   0 zixuanrao   (501) staff       (20)     4099 2023-05-10 17:09:08.000000 flasgger-0.9.7.1/examples/__pycache__/basic_auth.cpython-311.pyc
--rw-r--r--   0 zixuanrao   (501) staff       (20)     3126 2023-05-10 17:29:26.000000 flasgger-0.9.7.1/examples/__pycache__/basic_auth.cpython-39.pyc
--rw-r--r--   0 zixuanrao   (501) staff       (20)     2536 2023-05-10 17:09:08.000000 flasgger-0.9.7.1/examples/__pycache__/callbacks.cpython-311.pyc
--rw-r--r--   0 zixuanrao   (501) staff       (20)     1907 2023-05-10 17:29:26.000000 flasgger-0.9.7.1/examples/__pycache__/callbacks.cpython-39.pyc
--rw-r--r--   0 zixuanrao   (501) staff       (20)     2719 2023-05-10 17:09:08.000000 flasgger-0.9.7.1/examples/__pycache__/changelog_090.cpython-311.pyc
--rw-r--r--   0 zixuanrao   (501) staff       (20)     2213 2023-05-10 17:29:26.000000 flasgger-0.9.7.1/examples/__pycache__/changelog_090.cpython-39.pyc
--rw-r--r--   0 zixuanrao   (501) staff       (20)     2999 2023-05-10 17:09:08.000000 flasgger-0.9.7.1/examples/__pycache__/colors.cpython-311.pyc
--rw-r--r--   0 zixuanrao   (501) staff       (20)     2338 2023-05-10 17:29:26.000000 flasgger-0.9.7.1/examples/__pycache__/colors.cpython-39.pyc
--rw-r--r--   0 zixuanrao   (501) staff       (20)     3459 2023-05-10 17:09:08.000000 flasgger-0.9.7.1/examples/__pycache__/colors_external_js.cpython-311.pyc
--rw-r--r--   0 zixuanrao   (501) staff       (20)     2741 2023-05-10 17:29:26.000000 flasgger-0.9.7.1/examples/__pycache__/colors_external_js.cpython-39.pyc
--rw-r--r--   0 zixuanrao   (501) staff       (20)     2634 2023-05-10 17:09:08.000000 flasgger-0.9.7.1/examples/__pycache__/colors_from_specdict.cpython-311.pyc
--rw-r--r--   0 zixuanrao   (501) staff       (20)     1946 2023-05-10 17:29:26.000000 flasgger-0.9.7.1/examples/__pycache__/colors_from_specdict.cpython-39.pyc
--rw-r--r--   0 zixuanrao   (501) staff       (20)     1498 2023-05-10 17:09:08.000000 flasgger-0.9.7.1/examples/__pycache__/colors_template_json.cpython-311.pyc
--rw-r--r--   0 zixuanrao   (501) staff       (20)     1056 2023-05-10 17:29:26.000000 flasgger-0.9.7.1/examples/__pycache__/colors_template_json.cpython-39.pyc
--rw-r--r--   0 zixuanrao   (501) staff       (20)     1493 2023-05-10 17:09:08.000000 flasgger-0.9.7.1/examples/__pycache__/colors_template_yaml.cpython-311.pyc
--rw-r--r--   0 zixuanrao   (501) staff       (20)     1050 2023-05-10 17:29:26.000000 flasgger-0.9.7.1/examples/__pycache__/colors_template_yaml.cpython-39.pyc
--rw-r--r--   0 zixuanrao   (501) staff       (20)     3024 2023-05-10 17:09:08.000000 flasgger-0.9.7.1/examples/__pycache__/colors_uiversion2.cpython-311.pyc
--rw-r--r--   0 zixuanrao   (501) staff       (20)     2365 2023-05-10 17:29:26.000000 flasgger-0.9.7.1/examples/__pycache__/colors_uiversion2.cpython-39.pyc
--rw-r--r--   0 zixuanrao   (501) staff       (20)     2565 2023-05-10 17:09:08.000000 flasgger-0.9.7.1/examples/__pycache__/colors_with_schema.cpython-311.pyc
--rw-r--r--   0 zixuanrao   (501) staff       (20)     1734 2023-05-10 17:29:26.000000 flasgger-0.9.7.1/examples/__pycache__/colors_with_schema.cpython-39.pyc
--rw-r--r--   0 zixuanrao   (501) staff       (20)     1551 2023-05-10 17:09:08.000000 flasgger-0.9.7.1/examples/__pycache__/compat.cpython-311.pyc
--rw-r--r--   0 zixuanrao   (501) staff       (20)     1134 2023-05-10 17:29:26.000000 flasgger-0.9.7.1/examples/__pycache__/compat.cpython-39.pyc
--rw-r--r--   0 zixuanrao   (501) staff       (20)    11159 2023-05-10 17:09:08.000000 flasgger-0.9.7.1/examples/__pycache__/custom_validation_function.cpython-311.pyc
--rw-r--r--   0 zixuanrao   (501) staff       (20)     6016 2023-05-10 17:29:26.000000 flasgger-0.9.7.1/examples/__pycache__/custom_validation_function.cpython-39.pyc
--rw-r--r--   0 zixuanrao   (501) staff       (20)     1798 2023-05-10 17:09:08.000000 flasgger-0.9.7.1/examples/__pycache__/decorator_package.cpython-311.pyc
--rw-r--r--   0 zixuanrao   (501) staff       (20)     1148 2023-05-10 17:29:26.000000 flasgger-0.9.7.1/examples/__pycache__/decorator_package.cpython-39.pyc
--rw-r--r--   0 zixuanrao   (501) staff       (20)     4594 2023-05-10 17:09:08.000000 flasgger-0.9.7.1/examples/__pycache__/decorators_in_init_app.cpython-311.pyc
--rw-r--r--   0 zixuanrao   (501) staff       (20)     3569 2023-05-10 17:29:26.000000 flasgger-0.9.7.1/examples/__pycache__/decorators_in_init_app.cpython-39.pyc
--rw-r--r--   0 zixuanrao   (501) staff       (20)     4166 2023-05-10 17:09:08.000000 flasgger-0.9.7.1/examples/__pycache__/definition_object_test.cpython-311-pytest-7.3.1.pyc
--rw-r--r--   0 zixuanrao   (501) staff       (20)     2953 2023-05-10 17:29:26.000000 flasgger-0.9.7.1/examples/__pycache__/definition_object_test.cpython-39-pytest-7.3.1.pyc
--rw-r--r--   0 zixuanrao   (501) staff       (20)     1767 2023-05-10 17:09:08.000000 flasgger-0.9.7.1/examples/__pycache__/disable_swagger_ui.cpython-311.pyc
--rw-r--r--   0 zixuanrao   (501) staff       (20)     1229 2023-05-10 17:29:26.000000 flasgger-0.9.7.1/examples/__pycache__/disable_swagger_ui.cpython-39.pyc
--rw-r--r--   0 zixuanrao   (501) staff       (20)    18008 2023-05-10 17:09:08.000000 flasgger-0.9.7.1/examples/__pycache__/example_app.cpython-311.pyc
--rw-r--r--   0 zixuanrao   (501) staff       (20)    13276 2023-05-10 17:29:26.000000 flasgger-0.9.7.1/examples/__pycache__/example_app.cpython-39.pyc
--rw-r--r--   0 zixuanrao   (501) staff       (20)     3091 2023-05-10 17:09:08.000000 flasgger-0.9.7.1/examples/__pycache__/example_blueprint.cpython-311.pyc
--rw-r--r--   0 zixuanrao   (501) staff       (20)     2053 2023-05-10 17:29:26.000000 flasgger-0.9.7.1/examples/__pycache__/example_blueprint.cpython-39.pyc
--rw-r--r--   0 zixuanrao   (501) staff       (20)     3364 2023-05-10 17:09:08.000000 flasgger-0.9.7.1/examples/__pycache__/get_schema.cpython-311.pyc
--rw-r--r--   0 zixuanrao   (501) staff       (20)     2055 2023-05-10 17:29:26.000000 flasgger-0.9.7.1/examples/__pycache__/get_schema.cpython-39.pyc
--rw-r--r--   0 zixuanrao   (501) staff       (20)     4754 2023-05-10 17:09:08.000000 flasgger-0.9.7.1/examples/__pycache__/lazy_string.cpython-311.pyc
--rw-r--r--   0 zixuanrao   (501) staff       (20)     3554 2023-05-10 17:29:26.000000 flasgger-0.9.7.1/examples/__pycache__/lazy_string.cpython-39.pyc
--rw-r--r--   0 zixuanrao   (501) staff       (20)     2352 2023-05-10 17:09:08.000000 flasgger-0.9.7.1/examples/__pycache__/marshmallow_apispec.cpython-311.pyc
--rw-r--r--   0 zixuanrao   (501) staff       (20)     1598 2023-05-10 17:29:26.000000 flasgger-0.9.7.1/examples/__pycache__/marshmallow_apispec.cpython-39.pyc
--rw-r--r--   0 zixuanrao   (501) staff       (20)     2842 2023-05-10 17:09:08.000000 flasgger-0.9.7.1/examples/__pycache__/multiple_specs_dropdown_example.cpython-311.pyc
--rw-r--r--   0 zixuanrao   (501) staff       (20)     2058 2023-05-10 17:29:26.000000 flasgger-0.9.7.1/examples/__pycache__/multiple_specs_dropdown_example.cpython-39.pyc
--rw-r--r--   0 zixuanrao   (501) staff       (20)     2021 2023-05-10 17:09:08.000000 flasgger-0.9.7.1/examples/__pycache__/no_routes.cpython-311.pyc
--rw-r--r--   0 zixuanrao   (501) staff       (20)     1310 2023-05-10 17:29:26.000000 flasgger-0.9.7.1/examples/__pycache__/no_routes.cpython-39.pyc
--rw-r--r--   0 zixuanrao   (501) staff       (20)     3111 2023-05-10 17:09:08.000000 flasgger-0.9.7.1/examples/__pycache__/openapi3_examples.cpython-311.pyc
--rw-r--r--   0 zixuanrao   (501) staff       (20)     2408 2023-05-10 17:29:26.000000 flasgger-0.9.7.1/examples/__pycache__/openapi3_examples.cpython-39.pyc
--rw-r--r--   0 zixuanrao   (501) staff       (20)     2388 2023-05-10 17:09:08.000000 flasgger-0.9.7.1/examples/__pycache__/package_example.cpython-311.pyc
--rw-r--r--   0 zixuanrao   (501) staff       (20)     1805 2023-05-10 17:29:26.000000 flasgger-0.9.7.1/examples/__pycache__/package_example.cpython-39.pyc
--rw-r--r--   0 zixuanrao   (501) staff       (20)     2164 2023-05-10 17:09:08.000000 flasgger-0.9.7.1/examples/__pycache__/parse_openapi3.cpython-311.pyc
--rw-r--r--   0 zixuanrao   (501) staff       (20)     1531 2023-05-10 17:29:26.000000 flasgger-0.9.7.1/examples/__pycache__/parse_openapi3.cpython-39.pyc
--rw-r--r--   0 zixuanrao   (501) staff       (20)     2174 2023-05-10 17:09:08.000000 flasgger-0.9.7.1/examples/__pycache__/parse_openapi3_json.cpython-311.pyc
--rw-r--r--   0 zixuanrao   (501) staff       (20)     1541 2023-05-10 17:29:26.000000 flasgger-0.9.7.1/examples/__pycache__/parse_openapi3_json.cpython-39.pyc
--rw-r--r--   0 zixuanrao   (501) staff       (20)     8446 2023-05-10 17:09:08.000000 flasgger-0.9.7.1/examples/__pycache__/parsed_view_func.cpython-311.pyc
--rw-r--r--   0 zixuanrao   (501) staff       (20)     5572 2023-05-10 17:29:26.000000 flasgger-0.9.7.1/examples/__pycache__/parsed_view_func.cpython-39.pyc
--rw-r--r--   0 zixuanrao   (501) staff       (20)     3462 2023-05-10 17:09:08.000000 flasgger-0.9.7.1/examples/__pycache__/request_body.cpython-311.pyc
--rw-r--r--   0 zixuanrao   (501) staff       (20)     2350 2023-05-10 17:29:26.000000 flasgger-0.9.7.1/examples/__pycache__/request_body.cpython-39.pyc
--rw-r--r--   0 zixuanrao   (501) staff       (20)     6220 2023-05-10 17:09:08.000000 flasgger-0.9.7.1/examples/__pycache__/restful.cpython-311.pyc
--rw-r--r--   0 zixuanrao   (501) staff       (20)     4598 2023-05-10 17:29:26.000000 flasgger-0.9.7.1/examples/__pycache__/restful.cpython-39.pyc
--rw-r--r--   0 zixuanrao   (501) staff       (20)     1765 2023-05-10 17:09:08.000000 flasgger-0.9.7.1/examples/__pycache__/specs_route_example.cpython-311.pyc
--rw-r--r--   0 zixuanrao   (501) staff       (20)     1282 2023-05-10 17:29:26.000000 flasgger-0.9.7.1/examples/__pycache__/specs_route_example.cpython-39.pyc
--rw-r--r--   0 zixuanrao   (501) staff       (20)     4569 2023-05-10 16:57:35.000000 flasgger-0.9.7.1/examples/__pycache__/swag_annotation.cpython-311.pyc
--rw-r--r--   0 zixuanrao   (501) staff       (20)     3119 2023-05-10 17:28:14.000000 flasgger-0.9.7.1/examples/__pycache__/swag_annotation.cpython-39.pyc
--rw-r--r--   0 zixuanrao   (501) staff       (20)     1834 2023-05-10 17:09:08.000000 flasgger-0.9.7.1/examples/__pycache__/swag_from_merging.cpython-311.pyc
--rw-r--r--   0 zixuanrao   (501) staff       (20)     1147 2023-05-10 17:29:26.000000 flasgger-0.9.7.1/examples/__pycache__/swag_from_merging.cpython-39.pyc
--rw-r--r--   0 zixuanrao   (501) staff       (20)     1725 2023-05-10 17:09:08.000000 flasgger-0.9.7.1/examples/__pycache__/swag_from_overriding.cpython-311.pyc
--rw-r--r--   0 zixuanrao   (501) staff       (20)     1102 2023-05-10 17:29:26.000000 flasgger-0.9.7.1/examples/__pycache__/swag_from_overriding.cpython-39.pyc
--rw-r--r--   0 zixuanrao   (501) staff       (20)     3714 2023-05-10 17:09:08.000000 flasgger-0.9.7.1/examples/__pycache__/swagger_config_2.cpython-311.pyc
--rw-r--r--   0 zixuanrao   (501) staff       (20)     2864 2023-05-10 17:29:26.000000 flasgger-0.9.7.1/examples/__pycache__/swagger_config_2.cpython-39.pyc
--rw-r--r--   0 zixuanrao   (501) staff       (20)     3436 2023-05-10 17:09:08.000000 flasgger-0.9.7.1/examples/__pycache__/swagger_config_3.cpython-311.pyc
--rw-r--r--   0 zixuanrao   (501) staff       (20)     2701 2023-05-10 17:29:26.000000 flasgger-0.9.7.1/examples/__pycache__/swagger_config_3.cpython-39.pyc
--rw-r--r--   0 zixuanrao   (501) staff       (20)     3487 2023-05-10 17:09:08.000000 flasgger-0.9.7.1/examples/__pycache__/swagger_config_3_with_components_schemas.cpython-311.pyc
--rw-r--r--   0 zixuanrao   (501) staff       (20)     2748 2023-05-10 17:29:26.000000 flasgger-0.9.7.1/examples/__pycache__/swagger_config_3_with_components_schemas.cpython-39.pyc
--rw-r--r--   0 zixuanrao   (501) staff       (20)     3706 2023-05-10 17:09:08.000000 flasgger-0.9.7.1/examples/__pycache__/swagger_config_merge.cpython-311.pyc
--rw-r--r--   0 zixuanrao   (501) staff       (20)     2856 2023-05-10 17:29:26.000000 flasgger-0.9.7.1/examples/__pycache__/swagger_config_merge.cpython-39.pyc
--rw-r--r--   0 zixuanrao   (501) staff       (20)     8661 2023-05-10 17:09:08.000000 flasgger-0.9.7.1/examples/__pycache__/test_refs.cpython-311-pytest-7.3.1.pyc
--rw-r--r--   0 zixuanrao   (501) staff       (20)     3631 2023-05-10 17:29:26.000000 flasgger-0.9.7.1/examples/__pycache__/test_refs.cpython-39-pytest-7.3.1.pyc
--rw-r--r--   0 zixuanrao   (501) staff       (20)     1213 2023-05-10 17:09:08.000000 flasgger-0.9.7.1/examples/__pycache__/top_level_vendor_extension.cpython-311.pyc
--rw-r--r--   0 zixuanrao   (501) staff       (20)      891 2023-05-10 17:29:26.000000 flasgger-0.9.7.1/examples/__pycache__/top_level_vendor_extension.cpython-39.pyc
--rw-r--r--   0 zixuanrao   (501) staff       (20)     1278 2023-05-10 17:09:08.000000 flasgger-0.9.7.1/examples/__pycache__/use_openapi.cpython-311.pyc
--rw-r--r--   0 zixuanrao   (501) staff       (20)      908 2023-05-10 17:29:26.000000 flasgger-0.9.7.1/examples/__pycache__/use_openapi.cpython-39.pyc
--rw-r--r--   0 zixuanrao   (501) staff       (20)    13073 2023-05-10 17:09:08.000000 flasgger-0.9.7.1/examples/__pycache__/validation.cpython-311.pyc
--rw-r--r--   0 zixuanrao   (501) staff       (20)     9126 2023-05-10 17:29:26.000000 flasgger-0.9.7.1/examples/__pycache__/validation.cpython-39.pyc
--rw-r--r--   0 zixuanrao   (501) staff       (20)     8819 2023-05-10 17:09:08.000000 flasgger-0.9.7.1/examples/__pycache__/validation_error_handler.cpython-311.pyc
--rw-r--r--   0 zixuanrao   (501) staff       (20)     5498 2023-05-10 17:29:26.000000 flasgger-0.9.7.1/examples/__pycache__/validation_error_handler.cpython-39.pyc
--rw-r--r--   0 zixuanrao   (501) staff       (20)     2257 2023-05-05 16:18:04.000000 flasgger-0.9.7.1/examples/apispec_example.py
--rw-r--r--   0 zixuanrao   (501) staff       (20)     1767 2020-12-23 09:11:59.000000 flasgger-0.9.7.1/examples/apispec_example_uiversion3.py
--rw-r--r--   0 zixuanrao   (501) staff       (20)     1773 2020-12-23 09:11:59.000000 flasgger-0.9.7.1/examples/base_model_view.py
--rw-r--r--   0 zixuanrao   (501) staff       (20)     3079 2020-12-23 09:11:59.000000 flasgger-0.9.7.1/examples/basic_auth.py
--rw-r--r--   0 zixuanrao   (501) staff       (20)     1686 2020-12-23 09:11:59.000000 flasgger-0.9.7.1/examples/callbacks.py
--rw-r--r--   0 zixuanrao   (501) staff       (20)     3037 2020-12-23 09:11:59.000000 flasgger-0.9.7.1/examples/changelog_090.py
--rw-r--r--   0 zixuanrao   (501) staff       (20)     2133 2023-05-05 16:18:04.000000 flasgger-0.9.7.1/examples/colors.py
--rw-r--r--   0 zixuanrao   (501) staff       (20)     2584 2023-05-05 16:18:04.000000 flasgger-0.9.7.1/examples/colors_external_js.py
--rw-r--r--   0 zixuanrao   (501) staff       (20)     2195 2023-05-05 16:18:04.000000 flasgger-0.9.7.1/examples/colors_from_specdict.py
--rw-r--r--   0 zixuanrao   (501) staff       (20)     2105 2020-12-23 09:11:59.000000 flasgger-0.9.7.1/examples/colors_template.json
--rw-r--r--   0 zixuanrao   (501) staff       (20)     1384 2020-12-23 09:11:59.000000 flasgger-0.9.7.1/examples/colors_template.yaml
--rw-r--r--   0 zixuanrao   (501) staff       (20)      874 2023-05-05 16:18:04.000000 flasgger-0.9.7.1/examples/colors_template_json.py
--rw-r--r--   0 zixuanrao   (501) staff       (20)      867 2023-05-05 16:18:04.000000 flasgger-0.9.7.1/examples/colors_template_yaml.py
--rw-r--r--   0 zixuanrao   (501) staff       (20)     2156 2023-05-05 16:18:04.000000 flasgger-0.9.7.1/examples/colors_uiversion2.py
--rw-r--r--   0 zixuanrao   (501) staff       (20)     1446 2023-05-05 16:18:04.000000 flasgger-0.9.7.1/examples/colors_with_schema.py
--rw-r--r--   0 zixuanrao   (501) staff       (20)      999 2020-12-23 09:11:59.000000 flasgger-0.9.7.1/examples/compat.py
--rw-r--r--   0 zixuanrao   (501) staff       (20)     7135 2020-12-23 09:11:59.000000 flasgger-0.9.7.1/examples/custom_validation_function.py
--rw-r--r--   0 zixuanrao   (501) staff       (20)      698 2020-12-23 09:11:59.000000 flasgger-0.9.7.1/examples/decorator_package.py
--rw-r--r--   0 zixuanrao   (501) staff       (20)     3535 2020-12-23 09:11:59.000000 flasgger-0.9.7.1/examples/decorators_in_init_app.py
--rw-r--r--   0 zixuanrao   (501) staff       (20)     2594 2020-12-23 09:11:59.000000 flasgger-0.9.7.1/examples/definition_object_test.py
--rw-r--r--   0 zixuanrao   (501) staff       (20)      963 2020-12-23 09:11:59.000000 flasgger-0.9.7.1/examples/disable_swagger_ui.py
-drwxr-xr-x   0 zixuanrao   (501) staff       (20)        0 2023-05-18 17:14:52.171704 flasgger-0.9.7.1/examples/docs/
-drwxr-xr-x   0 zixuanrao   (501) staff       (20)        0 2023-05-18 17:14:52.172330 flasgger-0.9.7.1/examples/docs/item/
--rw-r--r--   0 zixuanrao   (501) staff       (20)      211 2020-12-23 09:11:59.000000 flasgger-0.9.7.1/examples/docs/item/get.yml
--rw-r--r--   0 zixuanrao   (501) staff       (20)      423 2020-12-23 09:11:59.000000 flasgger-0.9.7.1/examples/docs/item/put.yml
-drwxr-xr-x   0 zixuanrao   (501) staff       (20)        0 2023-05-18 17:14:52.172795 flasgger-0.9.7.1/examples/docs/items/
--rw-r--r--   0 zixuanrao   (501) staff       (20)      397 2020-12-23 09:11:59.000000 flasgger-0.9.7.1/examples/docs/items/get.yml
--rw-r--r--   0 zixuanrao   (501) staff       (20)      377 2020-12-23 09:11:59.000000 flasgger-0.9.7.1/examples/docs/items/post.yml
--rw-r--r--   0 zixuanrao   (501) staff       (20)      424 2020-12-23 09:11:59.000000 flasgger-0.9.7.1/examples/docs/template.yml
--rw-r--r--   0 zixuanrao   (501) staff       (20)      176 2020-12-23 09:11:59.000000 flasgger-0.9.7.1/examples/docs/user.yml
--rw-r--r--   0 zixuanrao   (501) staff       (20)    12749 2020-12-23 09:11:59.000000 flasgger-0.9.7.1/examples/example_app.py
--rw-r--r--   0 zixuanrao   (501) staff       (20)     1958 2020-12-23 09:11:59.000000 flasgger-0.9.7.1/examples/example_blueprint.py
--rw-r--r--   0 zixuanrao   (501) staff       (20)     1768 2020-12-23 09:11:59.000000 flasgger-0.9.7.1/examples/get_schema.py
--rw-r--r--   0 zixuanrao   (501) staff       (20)     3055 2023-05-10 06:09:07.000000 flasgger-0.9.7.1/examples/lazy_string.py
-drwxr-xr-x   0 zixuanrao   (501) staff       (20)        0 2023-05-18 17:14:52.173029 flasgger-0.9.7.1/examples/legacy/
--rw-r--r--   0 zixuanrao   (501) staff       (20)     5440 2023-05-10 04:02:27.000000 flasgger-0.9.7.1/examples/legacy/jwt_auth.py
--rw-r--r--   0 zixuanrao   (501) staff       (20)     1655 2020-12-23 09:11:59.000000 flasgger-0.9.7.1/examples/marshmallow_apispec.py
--rw-r--r--   0 zixuanrao   (501) staff       (20)     1757 2023-05-05 16:18:04.000000 flasgger-0.9.7.1/examples/multiple_specs_dropdown_example.py
--rw-r--r--   0 zixuanrao   (501) staff       (20)      794 2020-12-23 09:11:59.000000 flasgger-0.9.7.1/examples/no_routes.py
--rw-r--r--   0 zixuanrao   (501) staff       (20)       28 2020-12-23 09:11:59.000000 flasgger-0.9.7.1/examples/not_found.yaml
--rw-r--r--   0 zixuanrao   (501) staff       (20)      864 2020-12-23 09:11:59.000000 flasgger-0.9.7.1/examples/officer_specs.yml
--rw-r--r--   0 zixuanrao   (501) staff       (20)     2565 2020-12-23 09:19:56.000000 flasgger-0.9.7.1/examples/openapi3_examples.py
--rw-r--r--   0 zixuanrao   (501) staff       (20)     1519 2020-12-23 09:11:59.000000 flasgger-0.9.7.1/examples/package_example.py
--rw-r--r--   0 zixuanrao   (501) staff       (20)     1133 2023-05-05 16:18:04.000000 flasgger-0.9.7.1/examples/parse_openapi3.py
--rw-r--r--   0 zixuanrao   (501) staff       (20)     1138 2023-05-05 16:18:04.000000 flasgger-0.9.7.1/examples/parse_openapi3_json.py
--rw-r--r--   0 zixuanrao   (501) staff       (20)     1198 2023-05-05 16:18:04.000000 flasgger-0.9.7.1/examples/parse_openapi3_json_product_schema.yml
--rw-r--r--   0 zixuanrao   (501) staff       (20)     1198 2023-05-05 16:18:04.000000 flasgger-0.9.7.1/examples/parse_openapi3_product_schema.yml
--rw-r--r--   0 zixuanrao   (501) staff       (20)     5260 2023-05-10 04:45:21.000000 flasgger-0.9.7.1/examples/parsed_view_func.py
--rw-r--r--   0 zixuanrao   (501) staff       (20)     1848 2023-05-05 16:18:04.000000 flasgger-0.9.7.1/examples/request_body.py
--rw-r--r--   0 zixuanrao   (501) staff       (20)     3993 2020-12-23 09:11:59.000000 flasgger-0.9.7.1/examples/restful.py
--rw-r--r--   0 zixuanrao   (501) staff       (20)     1097 2020-12-23 09:11:59.000000 flasgger-0.9.7.1/examples/specs_route_example.py
--rw-r--r--   0 zixuanrao   (501) staff       (20)     2679 2023-05-10 18:08:22.000000 flasgger-0.9.7.1/examples/swag_annotation.py
--rw-r--r--   0 zixuanrao   (501) staff       (20)     1030 2020-12-23 09:11:59.000000 flasgger-0.9.7.1/examples/swag_from_merging.py
--rw-r--r--   0 zixuanrao   (501) staff       (20)      939 2020-12-23 09:11:59.000000 flasgger-0.9.7.1/examples/swag_from_overriding.py
--rw-r--r--   0 zixuanrao   (501) staff       (20)     3178 2023-05-05 16:18:04.000000 flasgger-0.9.7.1/examples/swagger_config_2.py
--rw-r--r--   0 zixuanrao   (501) staff       (20)     3291 2020-12-23 09:11:59.000000 flasgger-0.9.7.1/examples/swagger_config_3.py
--rw-r--r--   0 zixuanrao   (501) staff       (20)     3353 2023-05-05 16:18:04.000000 flasgger-0.9.7.1/examples/swagger_config_3_with_components_schemas.py
--rw-r--r--   0 zixuanrao   (501) staff       (20)     3164 2023-05-05 16:18:04.000000 flasgger-0.9.7.1/examples/swagger_config_merge.py
--rw-r--r--   0 zixuanrao   (501) staff       (20)     2067 2020-12-23 09:11:59.000000 flasgger-0.9.7.1/examples/test_refs.py
--rw-r--r--   0 zixuanrao   (501) staff       (20)     3145 2020-12-23 09:11:59.000000 flasgger-0.9.7.1/examples/test_refs_basePath_API.yaml
--rw-r--r--   0 zixuanrao   (501) staff       (20)      803 2020-12-23 09:11:59.000000 flasgger-0.9.7.1/examples/test_validation.yml
--rw-r--r--   0 zixuanrao   (501) staff       (20)      671 2020-12-23 09:11:59.000000 flasgger-0.9.7.1/examples/top_level_vendor_extension.py
--rw-r--r--   0 zixuanrao   (501) staff       (20)      757 2020-12-23 09:11:59.000000 flasgger-0.9.7.1/examples/use_openapi.py
--rw-r--r--   0 zixuanrao   (501) staff       (20)      477 2020-12-23 09:11:59.000000 flasgger-0.9.7.1/examples/user_with_id_specs.yml
--rw-r--r--   0 zixuanrao   (501) staff       (20)      508 2020-12-23 09:11:59.000000 flasgger-0.9.7.1/examples/user_without_id_specs.yml
--rw-r--r--   0 zixuanrao   (501) staff       (20)      768 2020-12-23 09:11:59.000000 flasgger-0.9.7.1/examples/username_specs.yml
--rw-r--r--   0 zixuanrao   (501) staff       (20)      771 2020-12-23 09:11:59.000000 flasgger-0.9.7.1/examples/username_specs_bom.yml
--rw-r--r--   0 zixuanrao   (501) staff       (20)      326 2020-12-23 09:11:59.000000 flasgger-0.9.7.1/examples/username_specs_no_descr.yml
--rw-r--r--   0 zixuanrao   (501) staff       (20)      322 2020-12-23 09:11:59.000000 flasgger-0.9.7.1/examples/username_specs_no_sep.yml
--rw-r--r--   0 zixuanrao   (501) staff       (20)     1530 2020-12-23 09:11:59.000000 flasgger-0.9.7.1/examples/username_specs_utf16.yml
--rw-r--r--   0 zixuanrao   (501) staff       (20)     3060 2020-12-23 09:11:59.000000 flasgger-0.9.7.1/examples/username_specs_utf32.yml
--rw-r--r--   0 zixuanrao   (501) staff       (20)    12127 2023-05-05 16:18:04.000000 flasgger-0.9.7.1/examples/validation.py
--rw-r--r--   0 zixuanrao   (501) staff       (20)     6179 2020-12-23 09:11:59.000000 flasgger-0.9.7.1/examples/validation_error_handler.py
-drwxr-xr-x   0 zixuanrao   (501) staff       (20)        0 2023-05-18 17:14:52.175969 flasgger-0.9.7.1/flasgger/
--rw-r--r--   0 zixuanrao   (501) staff       (20)     6148 2022-11-01 14:07:16.000000 flasgger-0.9.7.1/flasgger/.DS_Store
--rw-r--r--   0 zixuanrao   (501) staff       (20)      544 2023-05-18 17:13:12.000000 flasgger-0.9.7.1/flasgger/__init__.py
--rw-r--r--   0 zixuanrao   (501) staff       (20)    33148 2023-05-10 17:09:33.000000 flasgger-0.9.7.1/flasgger/base.py
--rw-r--r--   0 zixuanrao   (501) staff       (20)     1222 2023-05-05 16:18:04.000000 flasgger-0.9.7.1/flasgger/commands.py
--rw-r--r--   0 zixuanrao   (501) staff       (20)      820 2023-05-10 18:24:16.000000 flasgger-0.9.7.1/flasgger/compatible.py
--rw-r--r--   0 zixuanrao   (501) staff       (20)      519 2020-12-23 09:51:59.000000 flasgger-0.9.7.1/flasgger/constants.py
--rw-r--r--   0 zixuanrao   (501) staff       (20)     4795 2023-05-05 16:18:04.000000 flasgger-0.9.7.1/flasgger/marshmallow_apispec.py
-drwxr-xr-x   0 zixuanrao   (501) staff       (20)        0 2023-05-18 17:14:52.096873 flasgger-0.9.7.1/flasgger/ui2/
-drwxr-xr-x   0 zixuanrao   (501) staff       (20)        0 2023-05-18 17:14:52.189418 flasgger-0.9.7.1/flasgger/ui2/static/
-drwxr-xr-x   0 zixuanrao   (501) staff       (20)        0 2023-05-18 17:14:52.196657 flasgger-0.9.7.1/flasgger/ui2/static/css/
--rw-r--r--   0 zixuanrao   (501) staff       (20)    41666 2020-12-23 09:11:59.000000 flasgger-0.9.7.1/flasgger/ui2/static/css/print.css
--rw-r--r--   0 zixuanrao   (501) staff       (20)      773 2020-12-23 09:11:59.000000 flasgger-0.9.7.1/flasgger/ui2/static/css/reset.css
--rw-r--r--   0 zixuanrao   (501) staff       (20)    43644 2020-12-23 09:11:59.000000 flasgger-0.9.7.1/flasgger/ui2/static/css/screen.css
--rw-r--r--   0 zixuanrao   (501) staff       (20)     3488 2020-12-23 09:11:59.000000 flasgger-0.9.7.1/flasgger/ui2/static/css/style.css
--rw-r--r--   0 zixuanrao   (501) staff       (20)        0 2020-12-23 09:11:59.000000 flasgger-0.9.7.1/flasgger/ui2/static/css/typography.css
-drwxr-xr-x   0 zixuanrao   (501) staff       (20)        0 2023-05-18 17:14:52.202521 flasgger-0.9.7.1/flasgger/ui2/static/fonts/
--rw-r--r--   0 zixuanrao   (501) staff       (20)    42480 2020-12-23 09:11:59.000000 flasgger-0.9.7.1/flasgger/ui2/static/fonts/DroidSans-Bold.ttf
--rw-r--r--   0 zixuanrao   (501) staff       (20)    41028 2020-12-23 09:11:59.000000 flasgger-0.9.7.1/flasgger/ui2/static/fonts/DroidSans.ttf
--rw-r--r--   0 zixuanrao   (501) staff       (20)    22922 2020-12-23 09:11:59.000000 flasgger-0.9.7.1/flasgger/ui2/static/fonts/droid-sans-v6-latin-700.eot
--rw-r--r--   0 zixuanrao   (501) staff       (20)    73575 2020-12-23 09:11:59.000000 flasgger-0.9.7.1/flasgger/ui2/static/fonts/droid-sans-v6-latin-700.svg
--rw-r--r--   0 zixuanrao   (501) staff       (20)    40513 2020-12-23 09:11:59.000000 flasgger-0.9.7.1/flasgger/ui2/static/fonts/droid-sans-v6-latin-700.ttf
--rw-r--r--   0 zixuanrao   (501) staff       (20)    25992 2020-12-23 09:11:59.000000 flasgger-0.9.7.1/flasgger/ui2/static/fonts/droid-sans-v6-latin-700.woff
--rw-r--r--   0 zixuanrao   (501) staff       (20)    11480 2020-12-23 09:11:59.000000 flasgger-0.9.7.1/flasgger/ui2/static/fonts/droid-sans-v6-latin-700.woff2
--rw-r--r--   0 zixuanrao   (501) staff       (20)    22008 2020-12-23 09:11:59.000000 flasgger-0.9.7.1/flasgger/ui2/static/fonts/droid-sans-v6-latin-regular.eot
--rw-r--r--   0 zixuanrao   (501) staff       (20)    72148 2020-12-23 09:11:59.000000 flasgger-0.9.7.1/flasgger/ui2/static/fonts/droid-sans-v6-latin-regular.svg
--rw-r--r--   0 zixuanrao   (501) staff       (20)    39069 2020-12-23 09:11:59.000000 flasgger-0.9.7.1/flasgger/ui2/static/fonts/droid-sans-v6-latin-regular.ttf
--rw-r--r--   0 zixuanrao   (501) staff       (20)    24868 2020-12-23 09:11:59.000000 flasgger-0.9.7.1/flasgger/ui2/static/fonts/droid-sans-v6-latin-regular.woff
--rw-r--r--   0 zixuanrao   (501) staff       (20)    11304 2020-12-23 09:11:59.000000 flasgger-0.9.7.1/flasgger/ui2/static/fonts/droid-sans-v6-latin-regular.woff2
-drwxr-xr-x   0 zixuanrao   (501) staff       (20)        0 2023-05-18 17:14:52.204900 flasgger-0.9.7.1/flasgger/ui2/static/images/
--rw-r--r--   0 zixuanrao   (501) staff       (20)       69 2020-12-23 09:11:59.000000 flasgger-0.9.7.1/flasgger/ui2/static/images/collapse.gif
--rw-r--r--   0 zixuanrao   (501) staff       (20)       73 2020-12-23 09:11:59.000000 flasgger-0.9.7.1/flasgger/ui2/static/images/expand.gif
--rw-r--r--   0 zixuanrao   (501) staff       (20)     5115 2020-12-23 09:11:59.000000 flasgger-0.9.7.1/flasgger/ui2/static/images/explorer_icons.png
--rwxr-xr-x   0 zixuanrao   (501) staff       (20)      445 2020-12-23 09:11:59.000000 flasgger-0.9.7.1/flasgger/ui2/static/images/favicon-16x16.png
--rwxr-xr-x   0 zixuanrao   (501) staff       (20)     1141 2020-12-23 09:11:59.000000 flasgger-0.9.7.1/flasgger/ui2/static/images/favicon-32x32.png
--rwxr-xr-x   0 zixuanrao   (501) staff       (20)     5430 2020-12-23 09:11:59.000000 flasgger-0.9.7.1/flasgger/ui2/static/images/favicon.ico
--rw-r--r--   0 zixuanrao   (501) staff       (20)      455 2020-12-23 09:11:59.000000 flasgger-0.9.7.1/flasgger/ui2/static/images/logo_small.png
--rw-r--r--   0 zixuanrao   (501) staff       (20)      631 2020-12-23 09:11:59.000000 flasgger-0.9.7.1/flasgger/ui2/static/images/pet_store_api.png
--rw-r--r--   0 zixuanrao   (501) staff       (20)     9257 2020-12-23 09:11:59.000000 flasgger-0.9.7.1/flasgger/ui2/static/images/throbber.gif
--rw-r--r--   0 zixuanrao   (501) staff       (20)      670 2020-12-23 09:11:59.000000 flasgger-0.9.7.1/flasgger/ui2/static/images/wordnik_api.png
--rw-r--r--   0 zixuanrao   (501) staff       (20)     4335 2020-12-23 09:11:59.000000 flasgger-0.9.7.1/flasgger/ui2/static/index.html
-drwxr-xr-x   0 zixuanrao   (501) staff       (20)        0 2023-05-18 17:14:52.207898 flasgger-0.9.7.1/flasgger/ui2/static/lang/
--rw-r--r--   0 zixuanrao   (501) staff       (20)     2395 2020-12-23 09:11:59.000000 flasgger-0.9.7.1/flasgger/ui2/static/lang/ca.js
--rw-r--r--   0 zixuanrao   (501) staff       (20)     3470 2020-12-23 09:11:59.000000 flasgger-0.9.7.1/flasgger/ui2/static/lang/el.js
--rw-r--r--   0 zixuanrao   (501) staff       (20)     2342 2020-12-23 09:11:59.000000 flasgger-0.9.7.1/flasgger/ui2/static/lang/en.js
--rw-r--r--   0 zixuanrao   (501) staff       (20)     2464 2020-12-23 09:11:59.000000 flasgger-0.9.7.1/flasgger/ui2/static/lang/es.js
--rw-r--r--   0 zixuanrao   (501) staff       (20)     2503 2020-12-23 09:11:59.000000 flasgger-0.9.7.1/flasgger/ui2/static/lang/fr.js
--rw-r--r--   0 zixuanrao   (501) staff       (20)     3856 2020-12-23 09:11:59.000000 flasgger-0.9.7.1/flasgger/ui2/static/lang/geo.js
--rw-r--r--   0 zixuanrao   (501) staff       (20)     2432 2020-12-23 09:11:59.000000 flasgger-0.9.7.1/flasgger/ui2/static/lang/it.js
--rwxr-xr-x   0 zixuanrao   (501) staff       (20)     2721 2020-12-23 09:11:59.000000 flasgger-0.9.7.1/flasgger/ui2/static/lang/ja.js
--rw-r--r--   0 zixuanrao   (501) staff       (20)     2320 2020-12-23 09:11:59.000000 flasgger-0.9.7.1/flasgger/ui2/static/lang/ko-kr.js
--rw-r--r--   0 zixuanrao   (501) staff       (20)     2298 2020-12-23 09:11:59.000000 flasgger-0.9.7.1/flasgger/ui2/static/lang/pl.js
--rw-r--r--   0 zixuanrao   (501) staff       (20)     2314 2020-12-23 09:11:59.000000 flasgger-0.9.7.1/flasgger/ui2/static/lang/pt.js
--rw-r--r--   0 zixuanrao   (501) staff       (20)     3100 2020-12-23 09:11:59.000000 flasgger-0.9.7.1/flasgger/ui2/static/lang/ru.js
--rw-r--r--   0 zixuanrao   (501) staff       (20)     2286 2020-12-23 09:11:59.000000 flasgger-0.9.7.1/flasgger/ui2/static/lang/tr.js
--rw-r--r--   0 zixuanrao   (501) staff       (20)     1421 2020-12-23 09:11:59.000000 flasgger-0.9.7.1/flasgger/ui2/static/lang/translator.js
--rw-r--r--   0 zixuanrao   (501) staff       (20)     2203 2020-12-23 09:11:59.000000 flasgger-0.9.7.1/flasgger/ui2/static/lang/zh-cn.js
-drwxr-xr-x   0 zixuanrao   (501) staff       (20)        0 2023-05-18 17:14:52.217653 flasgger-0.9.7.1/flasgger/ui2/static/lib/
--rw-r--r--   0 zixuanrao   (501) staff       (20)    19371 2020-12-23 09:11:59.000000 flasgger-0.9.7.1/flasgger/ui2/static/lib/backbone-min.js
--rw-r--r--   0 zixuanrao   (501) staff       (20)    22724 2020-12-23 09:11:59.000000 flasgger-0.9.7.1/flasgger/ui2/static/lib/es5-shim.js
--rw-r--r--   0 zixuanrao   (501) staff       (20)    71504 2020-12-23 09:11:59.000000 flasgger-0.9.7.1/flasgger/ui2/static/lib/handlebars-4.0.5.js
--rw-r--r--   0 zixuanrao   (501) staff       (20)    10962 2020-12-23 09:11:59.000000 flasgger-0.9.7.1/flasgger/ui2/static/lib/highlight.9.1.0.pack.js
--rw-r--r--   0 zixuanrao   (501) staff       (20)      310 2020-12-23 09:11:59.000000 flasgger-0.9.7.1/flasgger/ui2/static/lib/highlight.9.1.0.pack_extended.js
--rw-r--r--   0 zixuanrao   (501) staff       (20)    92032 2020-12-23 09:11:59.000000 flasgger-0.9.7.1/flasgger/ui2/static/lib/jquery-1.8.0.min.js
--rw-r--r--   0 zixuanrao   (501) staff       (20)     3518 2020-12-23 09:11:59.000000 flasgger-0.9.7.1/flasgger/ui2/static/lib/jquery.ba-bbq.min.js
--rw-r--r--   0 zixuanrao   (501) staff       (20)      365 2020-12-23 09:11:59.000000 flasgger-0.9.7.1/flasgger/ui2/static/lib/jquery.slideto.min.js
--rw-r--r--   0 zixuanrao   (501) staff       (20)      536 2020-12-23 09:11:59.000000 flasgger-0.9.7.1/flasgger/ui2/static/lib/jquery.wiggle.min.js
--rw-r--r--   0 zixuanrao   (501) staff       (20)    43510 2020-12-23 09:11:59.000000 flasgger-0.9.7.1/flasgger/ui2/static/lib/js-yaml.min.js
--rw-r--r--   0 zixuanrao   (501) staff       (20)   129835 2020-12-23 09:11:59.000000 flasgger-0.9.7.1/flasgger/ui2/static/lib/jsoneditor.min.js
--rw-r--r--   0 zixuanrao   (501) staff       (20)    51894 2020-12-23 09:11:59.000000 flasgger-0.9.7.1/flasgger/ui2/static/lib/lodash.min.js
--rw-r--r--   0 zixuanrao   (501) staff       (20)    15724 2020-12-23 09:11:59.000000 flasgger-0.9.7.1/flasgger/ui2/static/lib/marked.js
--rw-r--r--   0 zixuanrao   (501) staff       (20)      349 2020-12-23 09:11:59.000000 flasgger-0.9.7.1/flasgger/ui2/static/lib/object-assign-pollyfill.js
--rw-r--r--   0 zixuanrao   (501) staff       (20)   130418 2020-12-23 09:11:59.000000 flasgger-0.9.7.1/flasgger/ui2/static/lib/sanitize-html.min.js
--rw-r--r--   0 zixuanrao   (501) staff       (20)     7061 2020-12-23 09:11:59.000000 flasgger-0.9.7.1/flasgger/ui2/static/lib/swagger-oauth.js
--rw-r--r--   0 zixuanrao   (501) staff       (20)      479 2020-12-23 09:11:59.000000 flasgger-0.9.7.1/flasgger/ui2/static/o2c.html
--rw-r--r--   0 zixuanrao   (501) staff       (20)  2708212 2020-12-23 09:11:59.000000 flasgger-0.9.7.1/flasgger/ui2/static/swagger-ui.js
--rw-r--r--   0 zixuanrao   (501) staff       (20)   453854 2020-12-23 09:11:59.000000 flasgger-0.9.7.1/flasgger/ui2/static/swagger-ui.min.js
-drwxr-xr-x   0 zixuanrao   (501) staff       (20)        0 2023-05-18 17:14:52.096947 flasgger-0.9.7.1/flasgger/ui2/templates/
-drwxr-xr-x   0 zixuanrao   (501) staff       (20)        0 2023-05-18 17:14:52.218672 flasgger-0.9.7.1/flasgger/ui2/templates/flasgger/
--rw-r--r--   0 zixuanrao   (501) staff       (20)     7263 2023-05-05 16:18:04.000000 flasgger-0.9.7.1/flasgger/ui2/templates/flasgger/index.html
--rw-r--r--   0 zixuanrao   (501) staff       (20)     6222 2020-12-23 09:11:59.000000 flasgger-0.9.7.1/flasgger/ui2/templates/flasgger/index_old.html
--rw-r--r--   0 zixuanrao   (501) staff       (20)      479 2020-12-23 09:11:59.000000 flasgger-0.9.7.1/flasgger/ui2/templates/flasgger/o2c.html
-drwxr-xr-x   0 zixuanrao   (501) staff       (20)        0 2023-05-18 17:14:52.098137 flasgger-0.9.7.1/flasgger/ui3/
-drwxr-xr-x   0 zixuanrao   (501) staff       (20)        0 2023-05-18 17:14:52.241879 flasgger-0.9.7.1/flasgger/ui3/static/
--rw-r--r--   0 zixuanrao   (501) staff       (20)      665 2020-12-23 09:19:56.000000 flasgger-0.9.7.1/flasgger/ui3/static/favicon-16x16.png
--rw-r--r--   0 zixuanrao   (501) staff       (20)      628 2020-12-23 09:19:56.000000 flasgger-0.9.7.1/flasgger/ui3/static/favicon-32x32.png
-drwxr-xr-x   0 zixuanrao   (501) staff       (20)        0 2023-05-18 17:14:52.248782 flasgger-0.9.7.1/flasgger/ui3/static/lib/
--rw-r--r--   0 zixuanrao   (501) staff       (20)    85578 2020-12-23 09:11:59.000000 flasgger-0.9.7.1/flasgger/ui3/static/lib/jquery.min.js
--rw-r--r--   0 zixuanrao   (501) staff       (20)   129572 2020-12-23 09:11:59.000000 flasgger-0.9.7.1/flasgger/ui3/static/lib/jquery.min.map
--rw-r--r--   0 zixuanrao   (501) staff       (20)  1002172 2020-12-23 09:19:56.000000 flasgger-0.9.7.1/flasgger/ui3/static/swagger-ui-bundle.js
--rw-r--r--   0 zixuanrao   (501) staff       (20)  4277142 2020-12-23 09:19:56.000000 flasgger-0.9.7.1/flasgger/ui3/static/swagger-ui-bundle.js.map
--rw-r--r--   0 zixuanrao   (501) staff       (20)   310590 2020-12-23 09:19:56.000000 flasgger-0.9.7.1/flasgger/ui3/static/swagger-ui-standalone-preset.js
--rw-r--r--   0 zixuanrao   (501) staff       (20)  1381697 2020-12-23 09:19:56.000000 flasgger-0.9.7.1/flasgger/ui3/static/swagger-ui-standalone-preset.js.map
--rw-r--r--   0 zixuanrao   (501) staff       (20)   142690 2020-12-23 09:19:56.000000 flasgger-0.9.7.1/flasgger/ui3/static/swagger-ui.css
--rw-r--r--   0 zixuanrao   (501) staff       (20)   280799 2020-12-23 09:19:56.000000 flasgger-0.9.7.1/flasgger/ui3/static/swagger-ui.css.map
--rw-r--r--   0 zixuanrao   (501) staff       (20)   399813 2020-12-23 09:19:56.000000 flasgger-0.9.7.1/flasgger/ui3/static/swagger-ui.js
--rw-r--r--   0 zixuanrao   (501) staff       (20)  1322743 2020-12-23 09:19:56.000000 flasgger-0.9.7.1/flasgger/ui3/static/swagger-ui.js.map
-drwxr-xr-x   0 zixuanrao   (501) staff       (20)        0 2023-05-18 17:14:52.098207 flasgger-0.9.7.1/flasgger/ui3/templates/
-drwxr-xr-x   0 zixuanrao   (501) staff       (20)        0 2023-05-18 17:14:52.252178 flasgger-0.9.7.1/flasgger/ui3/templates/flasgger/
--rw-r--r--   0 zixuanrao   (501) staff       (20)      176 2020-12-23 09:11:59.000000 flasgger-0.9.7.1/flasgger/ui3/templates/flasgger/body_scripts.html
--rw-r--r--   0 zixuanrao   (501) staff       (20)      108 2020-12-23 09:11:59.000000 flasgger-0.9.7.1/flasgger/ui3/templates/flasgger/custom_head.html
--rw-r--r--   0 zixuanrao   (501) staff       (20)      384 2020-12-23 09:11:59.000000 flasgger-0.9.7.1/flasgger/ui3/templates/flasgger/footer.html
--rw-r--r--   0 zixuanrao   (501) staff       (20)      659 2020-12-23 09:11:59.000000 flasgger-0.9.7.1/flasgger/ui3/templates/flasgger/head.html
--rw-r--r--   0 zixuanrao   (501) staff       (20)     1152 2020-12-23 09:11:59.000000 flasgger-0.9.7.1/flasgger/ui3/templates/flasgger/index.html
--rw-r--r--   0 zixuanrao   (501) staff       (20)     2388 2020-12-23 09:11:59.000000 flasgger-0.9.7.1/flasgger/ui3/templates/flasgger/oauth2-redirect.html
--rw-r--r--   0 zixuanrao   (501) staff       (20)     2535 2023-05-05 16:18:04.000000 flasgger-0.9.7.1/flasgger/ui3/templates/flasgger/swagger.html
--rw-r--r--   0 zixuanrao   (501) staff       (20)      168 2020-12-23 09:11:59.000000 flasgger-0.9.7.1/flasgger/ui3/templates/flasgger/top.html
--rw-r--r--   0 zixuanrao   (501) staff       (20)    35825 2023-05-10 04:03:14.000000 flasgger-0.9.7.1/flasgger/utils.py
-drwxr-xr-x   0 zixuanrao   (501) staff       (20)        0 2023-05-18 17:14:52.183828 flasgger-0.9.7.1/flasgger.egg-info/
--rw-r--r--   0 zixuanrao   (501) staff       (20)    28508 2023-05-18 17:14:52.000000 flasgger-0.9.7.1/flasgger.egg-info/PKG-INFO
--rw-r--r--   0 zixuanrao   (501) staff       (20)    13348 2023-05-18 17:14:52.000000 flasgger-0.9.7.1/flasgger.egg-info/SOURCES.txt
--rw-r--r--   0 zixuanrao   (501) staff       (20)        1 2023-05-18 17:14:52.000000 flasgger-0.9.7.1/flasgger.egg-info/dependency_links.txt
--rw-r--r--   0 zixuanrao   (501) staff       (20)       77 2023-05-18 17:14:52.000000 flasgger-0.9.7.1/flasgger.egg-info/entry_points.txt
--rw-r--r--   0 zixuanrao   (501) staff       (20)        1 2020-12-23 09:23:44.000000 flasgger-0.9.7.1/flasgger.egg-info/not-zip-safe
--rw-r--r--   0 zixuanrao   (501) staff       (20)       72 2023-05-18 17:14:52.000000 flasgger-0.9.7.1/flasgger.egg-info/requires.txt
--rw-r--r--   0 zixuanrao   (501) staff       (20)        9 2023-05-18 17:14:52.000000 flasgger-0.9.7.1/flasgger.egg-info/top_level.txt
--rw-r--r--   0 zixuanrao   (501) staff       (20)       67 2023-05-18 17:14:52.259898 flasgger-0.9.7.1/setup.cfg
--rw-r--r--   0 zixuanrao   (501) staff       (20)     1623 2023-05-10 18:08:22.000000 flasgger-0.9.7.1/setup.py
-drwxr-xr-x   0 zixuanrao   (501) staff       (20)        0 2023-05-18 17:14:52.254011 flasgger-0.9.7.1/tests/
-drwxr-xr-x   0 zixuanrao   (501) staff       (20)        0 2023-05-18 17:14:52.258931 flasgger-0.9.7.1/tests/__pycache__/
--rw-r--r--   0 zixuanrao   (501) staff       (20)     5520 2023-05-10 16:57:33.000000 flasgger-0.9.7.1/tests/__pycache__/conftest.cpython-311-pytest-7.3.1.pyc
--rw-r--r--   0 zixuanrao   (501) staff       (20)     2593 2020-12-23 09:21:52.000000 flasgger-0.9.7.1/tests/__pycache__/conftest.cpython-38-pytest-6.1.1.pyc
--rw-r--r--   0 zixuanrao   (501) staff       (20)     3230 2023-05-10 14:34:58.000000 flasgger-0.9.7.1/tests/__pycache__/conftest.cpython-39-pytest-7.3.1.pyc
--rw-r--r--   0 zixuanrao   (501) staff       (20)     2917 2023-05-10 16:57:34.000000 flasgger-0.9.7.1/tests/__pycache__/test_apispecs.cpython-311-pytest-7.3.1.pyc
--rw-r--r--   0 zixuanrao   (501) staff       (20)     1692 2023-05-10 03:54:22.000000 flasgger-0.9.7.1/tests/__pycache__/test_apispecs.cpython-39-pytest-7.3.1.pyc
--rw-r--r--   0 zixuanrao   (501) staff       (20)    13768 2023-05-10 16:57:34.000000 flasgger-0.9.7.1/tests/__pycache__/test_base.cpython-311-pytest-7.3.1.pyc
--rw-r--r--   0 zixuanrao   (501) staff       (20)     5334 2023-05-10 03:54:22.000000 flasgger-0.9.7.1/tests/__pycache__/test_base.cpython-39-pytest-7.3.1.pyc
--rw-r--r--   0 zixuanrao   (501) staff       (20)    10027 2023-05-10 16:57:34.000000 flasgger-0.9.7.1/tests/__pycache__/test_commands.cpython-311-pytest-7.3.1.pyc
--rw-r--r--   0 zixuanrao   (501) staff       (20)     4251 2023-05-10 03:54:22.000000 flasgger-0.9.7.1/tests/__pycache__/test_commands.cpython-39-pytest-7.3.1.pyc
--rw-r--r--   0 zixuanrao   (501) staff       (20)     4376 2023-05-10 16:57:34.000000 flasgger-0.9.7.1/tests/__pycache__/test_examples.cpython-311-pytest-7.3.1.pyc
--rw-r--r--   0 zixuanrao   (501) staff       (20)     2891 2023-05-10 03:54:22.000000 flasgger-0.9.7.1/tests/__pycache__/test_examples.cpython-39-pytest-7.3.1.pyc
--rw-r--r--   0 zixuanrao   (501) staff       (20)     5736 2023-05-10 16:57:35.000000 flasgger-0.9.7.1/tests/__pycache__/test_utils.cpython-311-pytest-7.3.1.pyc
--rw-r--r--   0 zixuanrao   (501) staff       (20)     1848 2023-05-10 03:54:22.000000 flasgger-0.9.7.1/tests/__pycache__/test_utils.cpython-39-pytest-7.3.1.pyc
--rw-r--r--   0 zixuanrao   (501) staff       (20)     2998 2023-05-10 05:56:35.000000 flasgger-0.9.7.1/tests/conftest.py
--rwxr-xr-x   0 zixuanrao   (501) staff       (20)      574 2023-05-05 16:18:04.000000 flasgger-0.9.7.1/tests/test_apispecs.py
--rw-r--r--   0 zixuanrao   (501) staff       (20)     2102 2021-04-13 07:52:00.000000 flasgger-0.9.7.1/tests/test_base.py
--rw-r--r--   0 zixuanrao   (501) staff       (20)     1403 2023-05-05 16:18:04.000000 flasgger-0.9.7.1/tests/test_commands.py
--rw-r--r--   0 zixuanrao   (501) staff       (20)     2399 2020-12-23 09:11:59.000000 flasgger-0.9.7.1/tests/test_examples.py
--rw-r--r--   0 zixuanrao   (501) staff       (20)      378 2021-04-13 07:52:00.000000 flasgger-0.9.7.1/tests/test_utils.py
+drwxr-xr-x   0 zixuanrao   (501) staff       (20)        0 2023-05-11 17:50:36.894483 flasgger-0.9.7b2/
+-rw-r--r--   0 zixuanrao   (501) staff       (20)     3218 2020-12-23 09:11:59.000000 flasgger-0.9.7b2/CODE_OF_CONDUCT.md
+-rw-r--r--   0 zixuanrao   (501) staff       (20)     1078 2020-12-23 09:11:59.000000 flasgger-0.9.7b2/LICENSE
+-rw-r--r--   0 zixuanrao   (501) staff       (20)     1023 2020-12-23 09:11:59.000000 flasgger-0.9.7b2/MANIFEST.in
+-rw-r--r--   0 zixuanrao   (501) staff       (20)    28394 2023-05-11 17:50:36.894639 flasgger-0.9.7b2/PKG-INFO
+-rw-r--r--   0 zixuanrao   (501) staff       (20)    27921 2023-05-05 16:18:04.000000 flasgger-0.9.7b2/README.md
+-rw-r--r--   0 zixuanrao   (501) staff       (20)    23841 2023-05-05 16:18:04.000000 flasgger-0.9.7b2/README.zh.md
+drwxr-xr-x   0 zixuanrao   (501) staff       (20)        0 2023-05-11 17:50:36.770440 flasgger-0.9.7b2/demo_app/
+-rw-r--r--   0 zixuanrao   (501) staff       (20)      213 2020-12-23 09:11:59.000000 flasgger-0.9.7b2/demo_app/README.md
+-rw-r--r--   0 zixuanrao   (501) staff       (20)        0 2020-12-23 09:11:59.000000 flasgger-0.9.7b2/demo_app/__init__.py
+-rw-r--r--   0 zixuanrao   (501) staff       (20)     1607 2020-12-23 09:19:56.000000 flasgger-0.9.7b2/demo_app/app.py
+-rw-r--r--   0 zixuanrao   (501) staff       (20)       53 2020-12-23 09:11:59.000000 flasgger-0.9.7b2/demo_app/requirements.txt
+drwxr-xr-x   0 zixuanrao   (501) staff       (20)        0 2023-05-11 17:50:36.771124 flasgger-0.9.7b2/demo_app/templates/
+-rw-r--r--   0 zixuanrao   (501) staff       (20)     5095 2020-12-23 09:11:59.000000 flasgger-0.9.7b2/demo_app/templates/flasgger.html
+-rw-r--r--   0 zixuanrao   (501) staff       (20)       97 2020-12-23 09:11:59.000000 flasgger-0.9.7b2/demo_app/templates/index.html
+-rw-r--r--   0 zixuanrao   (501) staff       (20)       23 2020-12-23 09:11:59.000000 flasgger-0.9.7b2/demo_app/update.sh
+drwxr-xr-x   0 zixuanrao   (501) staff       (20)        0 2023-05-11 17:50:36.771360 flasgger-0.9.7b2/etc/
+-rw-r--r--   0 zixuanrao   (501) staff       (20)     6148 2022-11-01 14:07:16.000000 flasgger-0.9.7b2/etc/.DS_Store
+drwxr-xr-x   0 zixuanrao   (501) staff       (20)        0 2023-05-11 17:50:36.771838 flasgger-0.9.7b2/etc/flasgger_package/
+-rw-r--r--   0 zixuanrao   (501) staff       (20)       37 2020-12-23 09:11:59.000000 flasgger-0.9.7b2/etc/flasgger_package/MANIFEST.in
+drwxr-xr-x   0 zixuanrao   (501) staff       (20)        0 2023-05-11 17:50:36.764646 flasgger-0.9.7b2/etc/flasgger_package/build/
+drwxr-xr-x   0 zixuanrao   (501) staff       (20)        0 2023-05-11 17:50:36.764711 flasgger-0.9.7b2/etc/flasgger_package/build/lib/
+drwxr-xr-x   0 zixuanrao   (501) staff       (20)        0 2023-05-11 17:50:36.772594 flasgger-0.9.7b2/etc/flasgger_package/build/lib/flasgger_package/
+-rw-r--r--   0 zixuanrao   (501) staff       (20)      161 2020-12-23 09:11:59.000000 flasgger-0.9.7b2/etc/flasgger_package/build/lib/flasgger_package/__init__.py
+-rw-r--r--   0 zixuanrao   (501) staff       (20)      574 2020-12-23 09:11:59.000000 flasgger-0.9.7b2/etc/flasgger_package/build/lib/flasgger_package/package_specs.yml
+-rw-r--r--   0 zixuanrao   (501) staff       (20)       80 2020-12-23 09:11:59.000000 flasgger-0.9.7b2/etc/flasgger_package/build/lib/flasgger_package/parameters.yml
+drwxr-xr-x   0 zixuanrao   (501) staff       (20)        0 2023-05-11 17:50:36.773776 flasgger-0.9.7b2/etc/flasgger_package/dist/
+-rw-r--r--   0 zixuanrao   (501) staff       (20)     2533 2023-05-10 17:09:06.000000 flasgger-0.9.7b2/etc/flasgger_package/dist/flasgger_package-0.0.1-py3.11.egg
+-rw-r--r--   0 zixuanrao   (501) staff       (20)     2002 2020-12-23 10:44:18.000000 flasgger-0.9.7b2/etc/flasgger_package/dist/flasgger_package-0.0.1-py3.8.egg
+-rw-r--r--   0 zixuanrao   (501) staff       (20)     2444 2023-05-10 17:44:25.000000 flasgger-0.9.7b2/etc/flasgger_package/dist/flasgger_package-0.0.1-py3.9.egg
+drwxr-xr-x   0 zixuanrao   (501) staff       (20)        0 2023-05-11 17:50:36.774462 flasgger-0.9.7b2/etc/flasgger_package/flasgger_package/
+-rw-r--r--   0 zixuanrao   (501) staff       (20)      161 2020-12-23 09:11:59.000000 flasgger-0.9.7b2/etc/flasgger_package/flasgger_package/__init__.py
+-rw-r--r--   0 zixuanrao   (501) staff       (20)      574 2020-12-23 09:11:59.000000 flasgger-0.9.7b2/etc/flasgger_package/flasgger_package/package_specs.yml
+-rw-r--r--   0 zixuanrao   (501) staff       (20)       80 2020-12-23 09:11:59.000000 flasgger-0.9.7b2/etc/flasgger_package/flasgger_package/parameters.yml
+drwxr-xr-x   0 zixuanrao   (501) staff       (20)        0 2023-05-11 17:50:36.776400 flasgger-0.9.7b2/etc/flasgger_package/flasgger_package.egg-info/
+-rw-r--r--   0 zixuanrao   (501) staff       (20)      247 2023-05-10 17:44:25.000000 flasgger-0.9.7b2/etc/flasgger_package/flasgger_package.egg-info/PKG-INFO
+-rw-r--r--   0 zixuanrao   (501) staff       (20)      354 2023-05-10 17:44:25.000000 flasgger-0.9.7b2/etc/flasgger_package/flasgger_package.egg-info/SOURCES.txt
+-rw-r--r--   0 zixuanrao   (501) staff       (20)        1 2023-05-10 17:44:25.000000 flasgger-0.9.7b2/etc/flasgger_package/flasgger_package.egg-info/dependency_links.txt
+-rw-r--r--   0 zixuanrao   (501) staff       (20)        1 2020-12-23 09:21:46.000000 flasgger-0.9.7b2/etc/flasgger_package/flasgger_package.egg-info/not-zip-safe
+-rw-r--r--   0 zixuanrao   (501) staff       (20)       21 2023-05-10 17:44:25.000000 flasgger-0.9.7b2/etc/flasgger_package/flasgger_package.egg-info/requires.txt
+-rw-r--r--   0 zixuanrao   (501) staff       (20)       17 2023-05-10 17:44:25.000000 flasgger-0.9.7b2/etc/flasgger_package/flasgger_package.egg-info/top_level.txt
+-rw-r--r--   0 zixuanrao   (501) staff       (20)      550 2020-12-23 09:11:59.000000 flasgger-0.9.7b2/etc/flasgger_package/setup.py
+drwxr-xr-x   0 zixuanrao   (501) staff       (20)        0 2023-05-11 17:50:36.776604 flasgger-0.9.7b2/etc/pythonanywhere/
+-rw-r--r--   0 zixuanrao   (501) staff       (20)     1858 2020-12-23 09:11:59.000000 flasgger-0.9.7b2/etc/pythonanywhere/pythonanywhere_com_wsgi.py
+drwxr-xr-x   0 zixuanrao   (501) staff       (20)        0 2023-05-11 17:50:36.795657 flasgger-0.9.7b2/examples/
+-rw-r--r--   0 zixuanrao   (501) staff       (20)     1176 2020-12-23 09:11:59.000000 flasgger-0.9.7b2/examples/README.md
+-rw-r--r--   0 zixuanrao   (501) staff       (20)        0 2020-12-23 09:11:59.000000 flasgger-0.9.7b2/examples/__init__.py
+drwxr-xr-x   0 zixuanrao   (501) staff       (20)        0 2023-05-11 17:50:36.821901 flasgger-0.9.7b2/examples/__pycache__/
+-rw-r--r--   0 zixuanrao   (501) staff       (20)      171 2023-05-10 16:57:35.000000 flasgger-0.9.7b2/examples/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 zixuanrao   (501) staff       (20)      153 2023-05-10 17:28:14.000000 flasgger-0.9.7b2/examples/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0 zixuanrao   (501) staff       (20)     3434 2023-05-10 17:09:08.000000 flasgger-0.9.7b2/examples/__pycache__/apispec_example.cpython-311.pyc
+-rw-r--r--   0 zixuanrao   (501) staff       (20)     2369 2023-05-10 17:29:26.000000 flasgger-0.9.7b2/examples/__pycache__/apispec_example.cpython-39.pyc
+-rw-r--r--   0 zixuanrao   (501) staff       (20)     2773 2023-05-10 17:09:08.000000 flasgger-0.9.7b2/examples/__pycache__/apispec_example_uiversion3.cpython-311.pyc
+-rw-r--r--   0 zixuanrao   (501) staff       (20)     1830 2023-05-10 17:29:26.000000 flasgger-0.9.7b2/examples/__pycache__/apispec_example_uiversion3.cpython-39.pyc
+-rw-r--r--   0 zixuanrao   (501) staff       (20)     2849 2023-05-10 17:09:08.000000 flasgger-0.9.7b2/examples/__pycache__/base_model_view.cpython-311.pyc
+-rw-r--r--   0 zixuanrao   (501) staff       (20)     2222 2023-05-10 17:29:26.000000 flasgger-0.9.7b2/examples/__pycache__/base_model_view.cpython-39.pyc
+-rw-r--r--   0 zixuanrao   (501) staff       (20)     4099 2023-05-10 17:09:08.000000 flasgger-0.9.7b2/examples/__pycache__/basic_auth.cpython-311.pyc
+-rw-r--r--   0 zixuanrao   (501) staff       (20)     3126 2023-05-10 17:29:26.000000 flasgger-0.9.7b2/examples/__pycache__/basic_auth.cpython-39.pyc
+-rw-r--r--   0 zixuanrao   (501) staff       (20)     2536 2023-05-10 17:09:08.000000 flasgger-0.9.7b2/examples/__pycache__/callbacks.cpython-311.pyc
+-rw-r--r--   0 zixuanrao   (501) staff       (20)     1907 2023-05-10 17:29:26.000000 flasgger-0.9.7b2/examples/__pycache__/callbacks.cpython-39.pyc
+-rw-r--r--   0 zixuanrao   (501) staff       (20)     2719 2023-05-10 17:09:08.000000 flasgger-0.9.7b2/examples/__pycache__/changelog_090.cpython-311.pyc
+-rw-r--r--   0 zixuanrao   (501) staff       (20)     2213 2023-05-10 17:29:26.000000 flasgger-0.9.7b2/examples/__pycache__/changelog_090.cpython-39.pyc
+-rw-r--r--   0 zixuanrao   (501) staff       (20)     2999 2023-05-10 17:09:08.000000 flasgger-0.9.7b2/examples/__pycache__/colors.cpython-311.pyc
+-rw-r--r--   0 zixuanrao   (501) staff       (20)     2338 2023-05-10 17:29:26.000000 flasgger-0.9.7b2/examples/__pycache__/colors.cpython-39.pyc
+-rw-r--r--   0 zixuanrao   (501) staff       (20)     3459 2023-05-10 17:09:08.000000 flasgger-0.9.7b2/examples/__pycache__/colors_external_js.cpython-311.pyc
+-rw-r--r--   0 zixuanrao   (501) staff       (20)     2741 2023-05-10 17:29:26.000000 flasgger-0.9.7b2/examples/__pycache__/colors_external_js.cpython-39.pyc
+-rw-r--r--   0 zixuanrao   (501) staff       (20)     2634 2023-05-10 17:09:08.000000 flasgger-0.9.7b2/examples/__pycache__/colors_from_specdict.cpython-311.pyc
+-rw-r--r--   0 zixuanrao   (501) staff       (20)     1946 2023-05-10 17:29:26.000000 flasgger-0.9.7b2/examples/__pycache__/colors_from_specdict.cpython-39.pyc
+-rw-r--r--   0 zixuanrao   (501) staff       (20)     1498 2023-05-10 17:09:08.000000 flasgger-0.9.7b2/examples/__pycache__/colors_template_json.cpython-311.pyc
+-rw-r--r--   0 zixuanrao   (501) staff       (20)     1056 2023-05-10 17:29:26.000000 flasgger-0.9.7b2/examples/__pycache__/colors_template_json.cpython-39.pyc
+-rw-r--r--   0 zixuanrao   (501) staff       (20)     1493 2023-05-10 17:09:08.000000 flasgger-0.9.7b2/examples/__pycache__/colors_template_yaml.cpython-311.pyc
+-rw-r--r--   0 zixuanrao   (501) staff       (20)     1050 2023-05-10 17:29:26.000000 flasgger-0.9.7b2/examples/__pycache__/colors_template_yaml.cpython-39.pyc
+-rw-r--r--   0 zixuanrao   (501) staff       (20)     3024 2023-05-10 17:09:08.000000 flasgger-0.9.7b2/examples/__pycache__/colors_uiversion2.cpython-311.pyc
+-rw-r--r--   0 zixuanrao   (501) staff       (20)     2365 2023-05-10 17:29:26.000000 flasgger-0.9.7b2/examples/__pycache__/colors_uiversion2.cpython-39.pyc
+-rw-r--r--   0 zixuanrao   (501) staff       (20)     2565 2023-05-10 17:09:08.000000 flasgger-0.9.7b2/examples/__pycache__/colors_with_schema.cpython-311.pyc
+-rw-r--r--   0 zixuanrao   (501) staff       (20)     1734 2023-05-10 17:29:26.000000 flasgger-0.9.7b2/examples/__pycache__/colors_with_schema.cpython-39.pyc
+-rw-r--r--   0 zixuanrao   (501) staff       (20)     1551 2023-05-10 17:09:08.000000 flasgger-0.9.7b2/examples/__pycache__/compat.cpython-311.pyc
+-rw-r--r--   0 zixuanrao   (501) staff       (20)     1134 2023-05-10 17:29:26.000000 flasgger-0.9.7b2/examples/__pycache__/compat.cpython-39.pyc
+-rw-r--r--   0 zixuanrao   (501) staff       (20)    11159 2023-05-10 17:09:08.000000 flasgger-0.9.7b2/examples/__pycache__/custom_validation_function.cpython-311.pyc
+-rw-r--r--   0 zixuanrao   (501) staff       (20)     6016 2023-05-10 17:29:26.000000 flasgger-0.9.7b2/examples/__pycache__/custom_validation_function.cpython-39.pyc
+-rw-r--r--   0 zixuanrao   (501) staff       (20)     1798 2023-05-10 17:09:08.000000 flasgger-0.9.7b2/examples/__pycache__/decorator_package.cpython-311.pyc
+-rw-r--r--   0 zixuanrao   (501) staff       (20)     1148 2023-05-10 17:29:26.000000 flasgger-0.9.7b2/examples/__pycache__/decorator_package.cpython-39.pyc
+-rw-r--r--   0 zixuanrao   (501) staff       (20)     4594 2023-05-10 17:09:08.000000 flasgger-0.9.7b2/examples/__pycache__/decorators_in_init_app.cpython-311.pyc
+-rw-r--r--   0 zixuanrao   (501) staff       (20)     3569 2023-05-10 17:29:26.000000 flasgger-0.9.7b2/examples/__pycache__/decorators_in_init_app.cpython-39.pyc
+-rw-r--r--   0 zixuanrao   (501) staff       (20)     4166 2023-05-10 17:09:08.000000 flasgger-0.9.7b2/examples/__pycache__/definition_object_test.cpython-311-pytest-7.3.1.pyc
+-rw-r--r--   0 zixuanrao   (501) staff       (20)     2953 2023-05-10 17:29:26.000000 flasgger-0.9.7b2/examples/__pycache__/definition_object_test.cpython-39-pytest-7.3.1.pyc
+-rw-r--r--   0 zixuanrao   (501) staff       (20)     1767 2023-05-10 17:09:08.000000 flasgger-0.9.7b2/examples/__pycache__/disable_swagger_ui.cpython-311.pyc
+-rw-r--r--   0 zixuanrao   (501) staff       (20)     1229 2023-05-10 17:29:26.000000 flasgger-0.9.7b2/examples/__pycache__/disable_swagger_ui.cpython-39.pyc
+-rw-r--r--   0 zixuanrao   (501) staff       (20)    18008 2023-05-10 17:09:08.000000 flasgger-0.9.7b2/examples/__pycache__/example_app.cpython-311.pyc
+-rw-r--r--   0 zixuanrao   (501) staff       (20)    13276 2023-05-10 17:29:26.000000 flasgger-0.9.7b2/examples/__pycache__/example_app.cpython-39.pyc
+-rw-r--r--   0 zixuanrao   (501) staff       (20)     3091 2023-05-10 17:09:08.000000 flasgger-0.9.7b2/examples/__pycache__/example_blueprint.cpython-311.pyc
+-rw-r--r--   0 zixuanrao   (501) staff       (20)     2053 2023-05-10 17:29:26.000000 flasgger-0.9.7b2/examples/__pycache__/example_blueprint.cpython-39.pyc
+-rw-r--r--   0 zixuanrao   (501) staff       (20)     3364 2023-05-10 17:09:08.000000 flasgger-0.9.7b2/examples/__pycache__/get_schema.cpython-311.pyc
+-rw-r--r--   0 zixuanrao   (501) staff       (20)     2055 2023-05-10 17:29:26.000000 flasgger-0.9.7b2/examples/__pycache__/get_schema.cpython-39.pyc
+-rw-r--r--   0 zixuanrao   (501) staff       (20)     4754 2023-05-10 17:09:08.000000 flasgger-0.9.7b2/examples/__pycache__/lazy_string.cpython-311.pyc
+-rw-r--r--   0 zixuanrao   (501) staff       (20)     3554 2023-05-10 17:29:26.000000 flasgger-0.9.7b2/examples/__pycache__/lazy_string.cpython-39.pyc
+-rw-r--r--   0 zixuanrao   (501) staff       (20)     2352 2023-05-10 17:09:08.000000 flasgger-0.9.7b2/examples/__pycache__/marshmallow_apispec.cpython-311.pyc
+-rw-r--r--   0 zixuanrao   (501) staff       (20)     1598 2023-05-10 17:29:26.000000 flasgger-0.9.7b2/examples/__pycache__/marshmallow_apispec.cpython-39.pyc
+-rw-r--r--   0 zixuanrao   (501) staff       (20)     2842 2023-05-10 17:09:08.000000 flasgger-0.9.7b2/examples/__pycache__/multiple_specs_dropdown_example.cpython-311.pyc
+-rw-r--r--   0 zixuanrao   (501) staff       (20)     2058 2023-05-10 17:29:26.000000 flasgger-0.9.7b2/examples/__pycache__/multiple_specs_dropdown_example.cpython-39.pyc
+-rw-r--r--   0 zixuanrao   (501) staff       (20)     2021 2023-05-10 17:09:08.000000 flasgger-0.9.7b2/examples/__pycache__/no_routes.cpython-311.pyc
+-rw-r--r--   0 zixuanrao   (501) staff       (20)     1310 2023-05-10 17:29:26.000000 flasgger-0.9.7b2/examples/__pycache__/no_routes.cpython-39.pyc
+-rw-r--r--   0 zixuanrao   (501) staff       (20)     3111 2023-05-10 17:09:08.000000 flasgger-0.9.7b2/examples/__pycache__/openapi3_examples.cpython-311.pyc
+-rw-r--r--   0 zixuanrao   (501) staff       (20)     2408 2023-05-10 17:29:26.000000 flasgger-0.9.7b2/examples/__pycache__/openapi3_examples.cpython-39.pyc
+-rw-r--r--   0 zixuanrao   (501) staff       (20)     2388 2023-05-10 17:09:08.000000 flasgger-0.9.7b2/examples/__pycache__/package_example.cpython-311.pyc
+-rw-r--r--   0 zixuanrao   (501) staff       (20)     1805 2023-05-10 17:29:26.000000 flasgger-0.9.7b2/examples/__pycache__/package_example.cpython-39.pyc
+-rw-r--r--   0 zixuanrao   (501) staff       (20)     2164 2023-05-10 17:09:08.000000 flasgger-0.9.7b2/examples/__pycache__/parse_openapi3.cpython-311.pyc
+-rw-r--r--   0 zixuanrao   (501) staff       (20)     1531 2023-05-10 17:29:26.000000 flasgger-0.9.7b2/examples/__pycache__/parse_openapi3.cpython-39.pyc
+-rw-r--r--   0 zixuanrao   (501) staff       (20)     2174 2023-05-10 17:09:08.000000 flasgger-0.9.7b2/examples/__pycache__/parse_openapi3_json.cpython-311.pyc
+-rw-r--r--   0 zixuanrao   (501) staff       (20)     1541 2023-05-10 17:29:26.000000 flasgger-0.9.7b2/examples/__pycache__/parse_openapi3_json.cpython-39.pyc
+-rw-r--r--   0 zixuanrao   (501) staff       (20)     8446 2023-05-10 17:09:08.000000 flasgger-0.9.7b2/examples/__pycache__/parsed_view_func.cpython-311.pyc
+-rw-r--r--   0 zixuanrao   (501) staff       (20)     5572 2023-05-10 17:29:26.000000 flasgger-0.9.7b2/examples/__pycache__/parsed_view_func.cpython-39.pyc
+-rw-r--r--   0 zixuanrao   (501) staff       (20)     3462 2023-05-10 17:09:08.000000 flasgger-0.9.7b2/examples/__pycache__/request_body.cpython-311.pyc
+-rw-r--r--   0 zixuanrao   (501) staff       (20)     2350 2023-05-10 17:29:26.000000 flasgger-0.9.7b2/examples/__pycache__/request_body.cpython-39.pyc
+-rw-r--r--   0 zixuanrao   (501) staff       (20)     6220 2023-05-10 17:09:08.000000 flasgger-0.9.7b2/examples/__pycache__/restful.cpython-311.pyc
+-rw-r--r--   0 zixuanrao   (501) staff       (20)     4598 2023-05-10 17:29:26.000000 flasgger-0.9.7b2/examples/__pycache__/restful.cpython-39.pyc
+-rw-r--r--   0 zixuanrao   (501) staff       (20)     1765 2023-05-10 17:09:08.000000 flasgger-0.9.7b2/examples/__pycache__/specs_route_example.cpython-311.pyc
+-rw-r--r--   0 zixuanrao   (501) staff       (20)     1282 2023-05-10 17:29:26.000000 flasgger-0.9.7b2/examples/__pycache__/specs_route_example.cpython-39.pyc
+-rw-r--r--   0 zixuanrao   (501) staff       (20)     4569 2023-05-10 16:57:35.000000 flasgger-0.9.7b2/examples/__pycache__/swag_annotation.cpython-311.pyc
+-rw-r--r--   0 zixuanrao   (501) staff       (20)     3119 2023-05-10 17:28:14.000000 flasgger-0.9.7b2/examples/__pycache__/swag_annotation.cpython-39.pyc
+-rw-r--r--   0 zixuanrao   (501) staff       (20)     1834 2023-05-10 17:09:08.000000 flasgger-0.9.7b2/examples/__pycache__/swag_from_merging.cpython-311.pyc
+-rw-r--r--   0 zixuanrao   (501) staff       (20)     1147 2023-05-10 17:29:26.000000 flasgger-0.9.7b2/examples/__pycache__/swag_from_merging.cpython-39.pyc
+-rw-r--r--   0 zixuanrao   (501) staff       (20)     1725 2023-05-10 17:09:08.000000 flasgger-0.9.7b2/examples/__pycache__/swag_from_overriding.cpython-311.pyc
+-rw-r--r--   0 zixuanrao   (501) staff       (20)     1102 2023-05-10 17:29:26.000000 flasgger-0.9.7b2/examples/__pycache__/swag_from_overriding.cpython-39.pyc
+-rw-r--r--   0 zixuanrao   (501) staff       (20)     3714 2023-05-10 17:09:08.000000 flasgger-0.9.7b2/examples/__pycache__/swagger_config_2.cpython-311.pyc
+-rw-r--r--   0 zixuanrao   (501) staff       (20)     2864 2023-05-10 17:29:26.000000 flasgger-0.9.7b2/examples/__pycache__/swagger_config_2.cpython-39.pyc
+-rw-r--r--   0 zixuanrao   (501) staff       (20)     3436 2023-05-10 17:09:08.000000 flasgger-0.9.7b2/examples/__pycache__/swagger_config_3.cpython-311.pyc
+-rw-r--r--   0 zixuanrao   (501) staff       (20)     2701 2023-05-10 17:29:26.000000 flasgger-0.9.7b2/examples/__pycache__/swagger_config_3.cpython-39.pyc
+-rw-r--r--   0 zixuanrao   (501) staff       (20)     3487 2023-05-10 17:09:08.000000 flasgger-0.9.7b2/examples/__pycache__/swagger_config_3_with_components_schemas.cpython-311.pyc
+-rw-r--r--   0 zixuanrao   (501) staff       (20)     2748 2023-05-10 17:29:26.000000 flasgger-0.9.7b2/examples/__pycache__/swagger_config_3_with_components_schemas.cpython-39.pyc
+-rw-r--r--   0 zixuanrao   (501) staff       (20)     3706 2023-05-10 17:09:08.000000 flasgger-0.9.7b2/examples/__pycache__/swagger_config_merge.cpython-311.pyc
+-rw-r--r--   0 zixuanrao   (501) staff       (20)     2856 2023-05-10 17:29:26.000000 flasgger-0.9.7b2/examples/__pycache__/swagger_config_merge.cpython-39.pyc
+-rw-r--r--   0 zixuanrao   (501) staff       (20)     8661 2023-05-10 17:09:08.000000 flasgger-0.9.7b2/examples/__pycache__/test_refs.cpython-311-pytest-7.3.1.pyc
+-rw-r--r--   0 zixuanrao   (501) staff       (20)     3631 2023-05-10 17:29:26.000000 flasgger-0.9.7b2/examples/__pycache__/test_refs.cpython-39-pytest-7.3.1.pyc
+-rw-r--r--   0 zixuanrao   (501) staff       (20)     1213 2023-05-10 17:09:08.000000 flasgger-0.9.7b2/examples/__pycache__/top_level_vendor_extension.cpython-311.pyc
+-rw-r--r--   0 zixuanrao   (501) staff       (20)      891 2023-05-10 17:29:26.000000 flasgger-0.9.7b2/examples/__pycache__/top_level_vendor_extension.cpython-39.pyc
+-rw-r--r--   0 zixuanrao   (501) staff       (20)     1278 2023-05-10 17:09:08.000000 flasgger-0.9.7b2/examples/__pycache__/use_openapi.cpython-311.pyc
+-rw-r--r--   0 zixuanrao   (501) staff       (20)      908 2023-05-10 17:29:26.000000 flasgger-0.9.7b2/examples/__pycache__/use_openapi.cpython-39.pyc
+-rw-r--r--   0 zixuanrao   (501) staff       (20)    13073 2023-05-10 17:09:08.000000 flasgger-0.9.7b2/examples/__pycache__/validation.cpython-311.pyc
+-rw-r--r--   0 zixuanrao   (501) staff       (20)     9126 2023-05-10 17:29:26.000000 flasgger-0.9.7b2/examples/__pycache__/validation.cpython-39.pyc
+-rw-r--r--   0 zixuanrao   (501) staff       (20)     8819 2023-05-10 17:09:08.000000 flasgger-0.9.7b2/examples/__pycache__/validation_error_handler.cpython-311.pyc
+-rw-r--r--   0 zixuanrao   (501) staff       (20)     5498 2023-05-10 17:29:26.000000 flasgger-0.9.7b2/examples/__pycache__/validation_error_handler.cpython-39.pyc
+-rw-r--r--   0 zixuanrao   (501) staff       (20)     2257 2023-05-05 16:18:04.000000 flasgger-0.9.7b2/examples/apispec_example.py
+-rw-r--r--   0 zixuanrao   (501) staff       (20)     1767 2020-12-23 09:11:59.000000 flasgger-0.9.7b2/examples/apispec_example_uiversion3.py
+-rw-r--r--   0 zixuanrao   (501) staff       (20)     1773 2020-12-23 09:11:59.000000 flasgger-0.9.7b2/examples/base_model_view.py
+-rw-r--r--   0 zixuanrao   (501) staff       (20)     3079 2020-12-23 09:11:59.000000 flasgger-0.9.7b2/examples/basic_auth.py
+-rw-r--r--   0 zixuanrao   (501) staff       (20)     1686 2020-12-23 09:11:59.000000 flasgger-0.9.7b2/examples/callbacks.py
+-rw-r--r--   0 zixuanrao   (501) staff       (20)     3037 2020-12-23 09:11:59.000000 flasgger-0.9.7b2/examples/changelog_090.py
+-rw-r--r--   0 zixuanrao   (501) staff       (20)     2133 2023-05-05 16:18:04.000000 flasgger-0.9.7b2/examples/colors.py
+-rw-r--r--   0 zixuanrao   (501) staff       (20)     2584 2023-05-05 16:18:04.000000 flasgger-0.9.7b2/examples/colors_external_js.py
+-rw-r--r--   0 zixuanrao   (501) staff       (20)     2195 2023-05-05 16:18:04.000000 flasgger-0.9.7b2/examples/colors_from_specdict.py
+-rw-r--r--   0 zixuanrao   (501) staff       (20)     2105 2020-12-23 09:11:59.000000 flasgger-0.9.7b2/examples/colors_template.json
+-rw-r--r--   0 zixuanrao   (501) staff       (20)     1384 2020-12-23 09:11:59.000000 flasgger-0.9.7b2/examples/colors_template.yaml
+-rw-r--r--   0 zixuanrao   (501) staff       (20)      874 2023-05-05 16:18:04.000000 flasgger-0.9.7b2/examples/colors_template_json.py
+-rw-r--r--   0 zixuanrao   (501) staff       (20)      867 2023-05-05 16:18:04.000000 flasgger-0.9.7b2/examples/colors_template_yaml.py
+-rw-r--r--   0 zixuanrao   (501) staff       (20)     2156 2023-05-05 16:18:04.000000 flasgger-0.9.7b2/examples/colors_uiversion2.py
+-rw-r--r--   0 zixuanrao   (501) staff       (20)     1446 2023-05-05 16:18:04.000000 flasgger-0.9.7b2/examples/colors_with_schema.py
+-rw-r--r--   0 zixuanrao   (501) staff       (20)      999 2020-12-23 09:11:59.000000 flasgger-0.9.7b2/examples/compat.py
+-rw-r--r--   0 zixuanrao   (501) staff       (20)     7135 2020-12-23 09:11:59.000000 flasgger-0.9.7b2/examples/custom_validation_function.py
+-rw-r--r--   0 zixuanrao   (501) staff       (20)      698 2020-12-23 09:11:59.000000 flasgger-0.9.7b2/examples/decorator_package.py
+-rw-r--r--   0 zixuanrao   (501) staff       (20)     3535 2020-12-23 09:11:59.000000 flasgger-0.9.7b2/examples/decorators_in_init_app.py
+-rw-r--r--   0 zixuanrao   (501) staff       (20)     2594 2020-12-23 09:11:59.000000 flasgger-0.9.7b2/examples/definition_object_test.py
+-rw-r--r--   0 zixuanrao   (501) staff       (20)      963 2020-12-23 09:11:59.000000 flasgger-0.9.7b2/examples/disable_swagger_ui.py
+drwxr-xr-x   0 zixuanrao   (501) staff       (20)        0 2023-05-11 17:50:36.822356 flasgger-0.9.7b2/examples/docs/
+drwxr-xr-x   0 zixuanrao   (501) staff       (20)        0 2023-05-11 17:50:36.822758 flasgger-0.9.7b2/examples/docs/item/
+-rw-r--r--   0 zixuanrao   (501) staff       (20)      211 2020-12-23 09:11:59.000000 flasgger-0.9.7b2/examples/docs/item/get.yml
+-rw-r--r--   0 zixuanrao   (501) staff       (20)      423 2020-12-23 09:11:59.000000 flasgger-0.9.7b2/examples/docs/item/put.yml
+drwxr-xr-x   0 zixuanrao   (501) staff       (20)        0 2023-05-11 17:50:36.823336 flasgger-0.9.7b2/examples/docs/items/
+-rw-r--r--   0 zixuanrao   (501) staff       (20)      397 2020-12-23 09:11:59.000000 flasgger-0.9.7b2/examples/docs/items/get.yml
+-rw-r--r--   0 zixuanrao   (501) staff       (20)      377 2020-12-23 09:11:59.000000 flasgger-0.9.7b2/examples/docs/items/post.yml
+-rw-r--r--   0 zixuanrao   (501) staff       (20)      424 2020-12-23 09:11:59.000000 flasgger-0.9.7b2/examples/docs/template.yml
+-rw-r--r--   0 zixuanrao   (501) staff       (20)      176 2020-12-23 09:11:59.000000 flasgger-0.9.7b2/examples/docs/user.yml
+-rw-r--r--   0 zixuanrao   (501) staff       (20)    12749 2020-12-23 09:11:59.000000 flasgger-0.9.7b2/examples/example_app.py
+-rw-r--r--   0 zixuanrao   (501) staff       (20)     1958 2020-12-23 09:11:59.000000 flasgger-0.9.7b2/examples/example_blueprint.py
+-rw-r--r--   0 zixuanrao   (501) staff       (20)     1768 2020-12-23 09:11:59.000000 flasgger-0.9.7b2/examples/get_schema.py
+-rw-r--r--   0 zixuanrao   (501) staff       (20)     3055 2023-05-10 06:09:07.000000 flasgger-0.9.7b2/examples/lazy_string.py
+drwxr-xr-x   0 zixuanrao   (501) staff       (20)        0 2023-05-11 17:50:36.823629 flasgger-0.9.7b2/examples/legacy/
+-rw-r--r--   0 zixuanrao   (501) staff       (20)     5440 2023-05-10 04:02:27.000000 flasgger-0.9.7b2/examples/legacy/jwt_auth.py
+-rw-r--r--   0 zixuanrao   (501) staff       (20)     1655 2020-12-23 09:11:59.000000 flasgger-0.9.7b2/examples/marshmallow_apispec.py
+-rw-r--r--   0 zixuanrao   (501) staff       (20)     1757 2023-05-05 16:18:04.000000 flasgger-0.9.7b2/examples/multiple_specs_dropdown_example.py
+-rw-r--r--   0 zixuanrao   (501) staff       (20)      794 2020-12-23 09:11:59.000000 flasgger-0.9.7b2/examples/no_routes.py
+-rw-r--r--   0 zixuanrao   (501) staff       (20)       28 2020-12-23 09:11:59.000000 flasgger-0.9.7b2/examples/not_found.yaml
+-rw-r--r--   0 zixuanrao   (501) staff       (20)      864 2020-12-23 09:11:59.000000 flasgger-0.9.7b2/examples/officer_specs.yml
+-rw-r--r--   0 zixuanrao   (501) staff       (20)     2565 2020-12-23 09:19:56.000000 flasgger-0.9.7b2/examples/openapi3_examples.py
+-rw-r--r--   0 zixuanrao   (501) staff       (20)     1519 2020-12-23 09:11:59.000000 flasgger-0.9.7b2/examples/package_example.py
+-rw-r--r--   0 zixuanrao   (501) staff       (20)     1133 2023-05-05 16:18:04.000000 flasgger-0.9.7b2/examples/parse_openapi3.py
+-rw-r--r--   0 zixuanrao   (501) staff       (20)     1138 2023-05-05 16:18:04.000000 flasgger-0.9.7b2/examples/parse_openapi3_json.py
+-rw-r--r--   0 zixuanrao   (501) staff       (20)     1198 2023-05-05 16:18:04.000000 flasgger-0.9.7b2/examples/parse_openapi3_json_product_schema.yml
+-rw-r--r--   0 zixuanrao   (501) staff       (20)     1198 2023-05-05 16:18:04.000000 flasgger-0.9.7b2/examples/parse_openapi3_product_schema.yml
+-rw-r--r--   0 zixuanrao   (501) staff       (20)     5260 2023-05-10 04:45:21.000000 flasgger-0.9.7b2/examples/parsed_view_func.py
+-rw-r--r--   0 zixuanrao   (501) staff       (20)     1848 2023-05-05 16:18:04.000000 flasgger-0.9.7b2/examples/request_body.py
+-rw-r--r--   0 zixuanrao   (501) staff       (20)     3993 2020-12-23 09:11:59.000000 flasgger-0.9.7b2/examples/restful.py
+-rw-r--r--   0 zixuanrao   (501) staff       (20)     1097 2020-12-23 09:11:59.000000 flasgger-0.9.7b2/examples/specs_route_example.py
+-rw-r--r--   0 zixuanrao   (501) staff       (20)     2679 2023-05-10 18:08:22.000000 flasgger-0.9.7b2/examples/swag_annotation.py
+-rw-r--r--   0 zixuanrao   (501) staff       (20)     1030 2020-12-23 09:11:59.000000 flasgger-0.9.7b2/examples/swag_from_merging.py
+-rw-r--r--   0 zixuanrao   (501) staff       (20)      939 2020-12-23 09:11:59.000000 flasgger-0.9.7b2/examples/swag_from_overriding.py
+-rw-r--r--   0 zixuanrao   (501) staff       (20)     3178 2023-05-05 16:18:04.000000 flasgger-0.9.7b2/examples/swagger_config_2.py
+-rw-r--r--   0 zixuanrao   (501) staff       (20)     3291 2020-12-23 09:11:59.000000 flasgger-0.9.7b2/examples/swagger_config_3.py
+-rw-r--r--   0 zixuanrao   (501) staff       (20)     3353 2023-05-05 16:18:04.000000 flasgger-0.9.7b2/examples/swagger_config_3_with_components_schemas.py
+-rw-r--r--   0 zixuanrao   (501) staff       (20)     3164 2023-05-05 16:18:04.000000 flasgger-0.9.7b2/examples/swagger_config_merge.py
+-rw-r--r--   0 zixuanrao   (501) staff       (20)     2067 2020-12-23 09:11:59.000000 flasgger-0.9.7b2/examples/test_refs.py
+-rw-r--r--   0 zixuanrao   (501) staff       (20)     3145 2020-12-23 09:11:59.000000 flasgger-0.9.7b2/examples/test_refs_basePath_API.yaml
+-rw-r--r--   0 zixuanrao   (501) staff       (20)      803 2020-12-23 09:11:59.000000 flasgger-0.9.7b2/examples/test_validation.yml
+-rw-r--r--   0 zixuanrao   (501) staff       (20)      671 2020-12-23 09:11:59.000000 flasgger-0.9.7b2/examples/top_level_vendor_extension.py
+-rw-r--r--   0 zixuanrao   (501) staff       (20)      757 2020-12-23 09:11:59.000000 flasgger-0.9.7b2/examples/use_openapi.py
+-rw-r--r--   0 zixuanrao   (501) staff       (20)      477 2020-12-23 09:11:59.000000 flasgger-0.9.7b2/examples/user_with_id_specs.yml
+-rw-r--r--   0 zixuanrao   (501) staff       (20)      508 2020-12-23 09:11:59.000000 flasgger-0.9.7b2/examples/user_without_id_specs.yml
+-rw-r--r--   0 zixuanrao   (501) staff       (20)      768 2020-12-23 09:11:59.000000 flasgger-0.9.7b2/examples/username_specs.yml
+-rw-r--r--   0 zixuanrao   (501) staff       (20)      771 2020-12-23 09:11:59.000000 flasgger-0.9.7b2/examples/username_specs_bom.yml
+-rw-r--r--   0 zixuanrao   (501) staff       (20)      326 2020-12-23 09:11:59.000000 flasgger-0.9.7b2/examples/username_specs_no_descr.yml
+-rw-r--r--   0 zixuanrao   (501) staff       (20)      322 2020-12-23 09:11:59.000000 flasgger-0.9.7b2/examples/username_specs_no_sep.yml
+-rw-r--r--   0 zixuanrao   (501) staff       (20)     1530 2020-12-23 09:11:59.000000 flasgger-0.9.7b2/examples/username_specs_utf16.yml
+-rw-r--r--   0 zixuanrao   (501) staff       (20)     3060 2020-12-23 09:11:59.000000 flasgger-0.9.7b2/examples/username_specs_utf32.yml
+-rw-r--r--   0 zixuanrao   (501) staff       (20)    12127 2023-05-05 16:18:04.000000 flasgger-0.9.7b2/examples/validation.py
+-rw-r--r--   0 zixuanrao   (501) staff       (20)     6179 2020-12-23 09:11:59.000000 flasgger-0.9.7b2/examples/validation_error_handler.py
+drwxr-xr-x   0 zixuanrao   (501) staff       (20)        0 2023-05-11 17:50:36.826814 flasgger-0.9.7b2/flasgger/
+-rw-r--r--   0 zixuanrao   (501) staff       (20)     6148 2022-11-01 14:07:16.000000 flasgger-0.9.7b2/flasgger/.DS_Store
+-rw-r--r--   0 zixuanrao   (501) staff       (20)      544 2023-05-11 17:49:10.000000 flasgger-0.9.7b2/flasgger/__init__.py
+-rw-r--r--   0 zixuanrao   (501) staff       (20)    33148 2023-05-10 17:09:33.000000 flasgger-0.9.7b2/flasgger/base.py
+-rw-r--r--   0 zixuanrao   (501) staff       (20)     1222 2023-05-05 16:18:04.000000 flasgger-0.9.7b2/flasgger/commands.py
+-rw-r--r--   0 zixuanrao   (501) staff       (20)      820 2023-05-10 18:24:16.000000 flasgger-0.9.7b2/flasgger/compatible.py
+-rw-r--r--   0 zixuanrao   (501) staff       (20)      519 2020-12-23 09:51:59.000000 flasgger-0.9.7b2/flasgger/constants.py
+-rw-r--r--   0 zixuanrao   (501) staff       (20)     4795 2023-05-05 16:18:04.000000 flasgger-0.9.7b2/flasgger/marshmallow_apispec.py
+drwxr-xr-x   0 zixuanrao   (501) staff       (20)        0 2023-05-11 17:50:36.766695 flasgger-0.9.7b2/flasgger/ui2/
+drwxr-xr-x   0 zixuanrao   (501) staff       (20)        0 2023-05-11 17:50:36.838084 flasgger-0.9.7b2/flasgger/ui2/static/
+drwxr-xr-x   0 zixuanrao   (501) staff       (20)        0 2023-05-11 17:50:36.842046 flasgger-0.9.7b2/flasgger/ui2/static/css/
+-rw-r--r--   0 zixuanrao   (501) staff       (20)    41666 2020-12-23 09:11:59.000000 flasgger-0.9.7b2/flasgger/ui2/static/css/print.css
+-rw-r--r--   0 zixuanrao   (501) staff       (20)      773 2020-12-23 09:11:59.000000 flasgger-0.9.7b2/flasgger/ui2/static/css/reset.css
+-rw-r--r--   0 zixuanrao   (501) staff       (20)    43644 2020-12-23 09:11:59.000000 flasgger-0.9.7b2/flasgger/ui2/static/css/screen.css
+-rw-r--r--   0 zixuanrao   (501) staff       (20)     3488 2020-12-23 09:11:59.000000 flasgger-0.9.7b2/flasgger/ui2/static/css/style.css
+-rw-r--r--   0 zixuanrao   (501) staff       (20)        0 2020-12-23 09:11:59.000000 flasgger-0.9.7b2/flasgger/ui2/static/css/typography.css
+drwxr-xr-x   0 zixuanrao   (501) staff       (20)        0 2023-05-11 17:50:36.845568 flasgger-0.9.7b2/flasgger/ui2/static/fonts/
+-rw-r--r--   0 zixuanrao   (501) staff       (20)    42480 2020-12-23 09:11:59.000000 flasgger-0.9.7b2/flasgger/ui2/static/fonts/DroidSans-Bold.ttf
+-rw-r--r--   0 zixuanrao   (501) staff       (20)    41028 2020-12-23 09:11:59.000000 flasgger-0.9.7b2/flasgger/ui2/static/fonts/DroidSans.ttf
+-rw-r--r--   0 zixuanrao   (501) staff       (20)    22922 2020-12-23 09:11:59.000000 flasgger-0.9.7b2/flasgger/ui2/static/fonts/droid-sans-v6-latin-700.eot
+-rw-r--r--   0 zixuanrao   (501) staff       (20)    73575 2020-12-23 09:11:59.000000 flasgger-0.9.7b2/flasgger/ui2/static/fonts/droid-sans-v6-latin-700.svg
+-rw-r--r--   0 zixuanrao   (501) staff       (20)    40513 2020-12-23 09:11:59.000000 flasgger-0.9.7b2/flasgger/ui2/static/fonts/droid-sans-v6-latin-700.ttf
+-rw-r--r--   0 zixuanrao   (501) staff       (20)    25992 2020-12-23 09:11:59.000000 flasgger-0.9.7b2/flasgger/ui2/static/fonts/droid-sans-v6-latin-700.woff
+-rw-r--r--   0 zixuanrao   (501) staff       (20)    11480 2020-12-23 09:11:59.000000 flasgger-0.9.7b2/flasgger/ui2/static/fonts/droid-sans-v6-latin-700.woff2
+-rw-r--r--   0 zixuanrao   (501) staff       (20)    22008 2020-12-23 09:11:59.000000 flasgger-0.9.7b2/flasgger/ui2/static/fonts/droid-sans-v6-latin-regular.eot
+-rw-r--r--   0 zixuanrao   (501) staff       (20)    72148 2020-12-23 09:11:59.000000 flasgger-0.9.7b2/flasgger/ui2/static/fonts/droid-sans-v6-latin-regular.svg
+-rw-r--r--   0 zixuanrao   (501) staff       (20)    39069 2020-12-23 09:11:59.000000 flasgger-0.9.7b2/flasgger/ui2/static/fonts/droid-sans-v6-latin-regular.ttf
+-rw-r--r--   0 zixuanrao   (501) staff       (20)    24868 2020-12-23 09:11:59.000000 flasgger-0.9.7b2/flasgger/ui2/static/fonts/droid-sans-v6-latin-regular.woff
+-rw-r--r--   0 zixuanrao   (501) staff       (20)    11304 2020-12-23 09:11:59.000000 flasgger-0.9.7b2/flasgger/ui2/static/fonts/droid-sans-v6-latin-regular.woff2
+drwxr-xr-x   0 zixuanrao   (501) staff       (20)        0 2023-05-11 17:50:36.847562 flasgger-0.9.7b2/flasgger/ui2/static/images/
+-rw-r--r--   0 zixuanrao   (501) staff       (20)       69 2020-12-23 09:11:59.000000 flasgger-0.9.7b2/flasgger/ui2/static/images/collapse.gif
+-rw-r--r--   0 zixuanrao   (501) staff       (20)       73 2020-12-23 09:11:59.000000 flasgger-0.9.7b2/flasgger/ui2/static/images/expand.gif
+-rw-r--r--   0 zixuanrao   (501) staff       (20)     5115 2020-12-23 09:11:59.000000 flasgger-0.9.7b2/flasgger/ui2/static/images/explorer_icons.png
+-rwxr-xr-x   0 zixuanrao   (501) staff       (20)      445 2020-12-23 09:11:59.000000 flasgger-0.9.7b2/flasgger/ui2/static/images/favicon-16x16.png
+-rwxr-xr-x   0 zixuanrao   (501) staff       (20)     1141 2020-12-23 09:11:59.000000 flasgger-0.9.7b2/flasgger/ui2/static/images/favicon-32x32.png
+-rwxr-xr-x   0 zixuanrao   (501) staff       (20)     5430 2020-12-23 09:11:59.000000 flasgger-0.9.7b2/flasgger/ui2/static/images/favicon.ico
+-rw-r--r--   0 zixuanrao   (501) staff       (20)      455 2020-12-23 09:11:59.000000 flasgger-0.9.7b2/flasgger/ui2/static/images/logo_small.png
+-rw-r--r--   0 zixuanrao   (501) staff       (20)      631 2020-12-23 09:11:59.000000 flasgger-0.9.7b2/flasgger/ui2/static/images/pet_store_api.png
+-rw-r--r--   0 zixuanrao   (501) staff       (20)     9257 2020-12-23 09:11:59.000000 flasgger-0.9.7b2/flasgger/ui2/static/images/throbber.gif
+-rw-r--r--   0 zixuanrao   (501) staff       (20)      670 2020-12-23 09:11:59.000000 flasgger-0.9.7b2/flasgger/ui2/static/images/wordnik_api.png
+-rw-r--r--   0 zixuanrao   (501) staff       (20)     4335 2020-12-23 09:11:59.000000 flasgger-0.9.7b2/flasgger/ui2/static/index.html
+drwxr-xr-x   0 zixuanrao   (501) staff       (20)        0 2023-05-11 17:50:36.850640 flasgger-0.9.7b2/flasgger/ui2/static/lang/
+-rw-r--r--   0 zixuanrao   (501) staff       (20)     2395 2020-12-23 09:11:59.000000 flasgger-0.9.7b2/flasgger/ui2/static/lang/ca.js
+-rw-r--r--   0 zixuanrao   (501) staff       (20)     3470 2020-12-23 09:11:59.000000 flasgger-0.9.7b2/flasgger/ui2/static/lang/el.js
+-rw-r--r--   0 zixuanrao   (501) staff       (20)     2342 2020-12-23 09:11:59.000000 flasgger-0.9.7b2/flasgger/ui2/static/lang/en.js
+-rw-r--r--   0 zixuanrao   (501) staff       (20)     2464 2020-12-23 09:11:59.000000 flasgger-0.9.7b2/flasgger/ui2/static/lang/es.js
+-rw-r--r--   0 zixuanrao   (501) staff       (20)     2503 2020-12-23 09:11:59.000000 flasgger-0.9.7b2/flasgger/ui2/static/lang/fr.js
+-rw-r--r--   0 zixuanrao   (501) staff       (20)     3856 2020-12-23 09:11:59.000000 flasgger-0.9.7b2/flasgger/ui2/static/lang/geo.js
+-rw-r--r--   0 zixuanrao   (501) staff       (20)     2432 2020-12-23 09:11:59.000000 flasgger-0.9.7b2/flasgger/ui2/static/lang/it.js
+-rwxr-xr-x   0 zixuanrao   (501) staff       (20)     2721 2020-12-23 09:11:59.000000 flasgger-0.9.7b2/flasgger/ui2/static/lang/ja.js
+-rw-r--r--   0 zixuanrao   (501) staff       (20)     2320 2020-12-23 09:11:59.000000 flasgger-0.9.7b2/flasgger/ui2/static/lang/ko-kr.js
+-rw-r--r--   0 zixuanrao   (501) staff       (20)     2298 2020-12-23 09:11:59.000000 flasgger-0.9.7b2/flasgger/ui2/static/lang/pl.js
+-rw-r--r--   0 zixuanrao   (501) staff       (20)     2314 2020-12-23 09:11:59.000000 flasgger-0.9.7b2/flasgger/ui2/static/lang/pt.js
+-rw-r--r--   0 zixuanrao   (501) staff       (20)     3100 2020-12-23 09:11:59.000000 flasgger-0.9.7b2/flasgger/ui2/static/lang/ru.js
+-rw-r--r--   0 zixuanrao   (501) staff       (20)     2286 2020-12-23 09:11:59.000000 flasgger-0.9.7b2/flasgger/ui2/static/lang/tr.js
+-rw-r--r--   0 zixuanrao   (501) staff       (20)     1421 2020-12-23 09:11:59.000000 flasgger-0.9.7b2/flasgger/ui2/static/lang/translator.js
+-rw-r--r--   0 zixuanrao   (501) staff       (20)     2203 2020-12-23 09:11:59.000000 flasgger-0.9.7b2/flasgger/ui2/static/lang/zh-cn.js
+drwxr-xr-x   0 zixuanrao   (501) staff       (20)        0 2023-05-11 17:50:36.855060 flasgger-0.9.7b2/flasgger/ui2/static/lib/
+-rw-r--r--   0 zixuanrao   (501) staff       (20)    19371 2020-12-23 09:11:59.000000 flasgger-0.9.7b2/flasgger/ui2/static/lib/backbone-min.js
+-rw-r--r--   0 zixuanrao   (501) staff       (20)    22724 2020-12-23 09:11:59.000000 flasgger-0.9.7b2/flasgger/ui2/static/lib/es5-shim.js
+-rw-r--r--   0 zixuanrao   (501) staff       (20)    71504 2020-12-23 09:11:59.000000 flasgger-0.9.7b2/flasgger/ui2/static/lib/handlebars-4.0.5.js
+-rw-r--r--   0 zixuanrao   (501) staff       (20)    10962 2020-12-23 09:11:59.000000 flasgger-0.9.7b2/flasgger/ui2/static/lib/highlight.9.1.0.pack.js
+-rw-r--r--   0 zixuanrao   (501) staff       (20)      310 2020-12-23 09:11:59.000000 flasgger-0.9.7b2/flasgger/ui2/static/lib/highlight.9.1.0.pack_extended.js
+-rw-r--r--   0 zixuanrao   (501) staff       (20)    92032 2020-12-23 09:11:59.000000 flasgger-0.9.7b2/flasgger/ui2/static/lib/jquery-1.8.0.min.js
+-rw-r--r--   0 zixuanrao   (501) staff       (20)     3518 2020-12-23 09:11:59.000000 flasgger-0.9.7b2/flasgger/ui2/static/lib/jquery.ba-bbq.min.js
+-rw-r--r--   0 zixuanrao   (501) staff       (20)      365 2020-12-23 09:11:59.000000 flasgger-0.9.7b2/flasgger/ui2/static/lib/jquery.slideto.min.js
+-rw-r--r--   0 zixuanrao   (501) staff       (20)      536 2020-12-23 09:11:59.000000 flasgger-0.9.7b2/flasgger/ui2/static/lib/jquery.wiggle.min.js
+-rw-r--r--   0 zixuanrao   (501) staff       (20)    43510 2020-12-23 09:11:59.000000 flasgger-0.9.7b2/flasgger/ui2/static/lib/js-yaml.min.js
+-rw-r--r--   0 zixuanrao   (501) staff       (20)   129835 2020-12-23 09:11:59.000000 flasgger-0.9.7b2/flasgger/ui2/static/lib/jsoneditor.min.js
+-rw-r--r--   0 zixuanrao   (501) staff       (20)    51894 2020-12-23 09:11:59.000000 flasgger-0.9.7b2/flasgger/ui2/static/lib/lodash.min.js
+-rw-r--r--   0 zixuanrao   (501) staff       (20)    15724 2020-12-23 09:11:59.000000 flasgger-0.9.7b2/flasgger/ui2/static/lib/marked.js
+-rw-r--r--   0 zixuanrao   (501) staff       (20)      349 2020-12-23 09:11:59.000000 flasgger-0.9.7b2/flasgger/ui2/static/lib/object-assign-pollyfill.js
+-rw-r--r--   0 zixuanrao   (501) staff       (20)   130418 2020-12-23 09:11:59.000000 flasgger-0.9.7b2/flasgger/ui2/static/lib/sanitize-html.min.js
+-rw-r--r--   0 zixuanrao   (501) staff       (20)     7061 2020-12-23 09:11:59.000000 flasgger-0.9.7b2/flasgger/ui2/static/lib/swagger-oauth.js
+-rw-r--r--   0 zixuanrao   (501) staff       (20)      479 2020-12-23 09:11:59.000000 flasgger-0.9.7b2/flasgger/ui2/static/o2c.html
+-rw-r--r--   0 zixuanrao   (501) staff       (20)  2708212 2020-12-23 09:11:59.000000 flasgger-0.9.7b2/flasgger/ui2/static/swagger-ui.js
+-rw-r--r--   0 zixuanrao   (501) staff       (20)   453854 2020-12-23 09:11:59.000000 flasgger-0.9.7b2/flasgger/ui2/static/swagger-ui.min.js
+drwxr-xr-x   0 zixuanrao   (501) staff       (20)        0 2023-05-11 17:50:36.766769 flasgger-0.9.7b2/flasgger/ui2/templates/
+drwxr-xr-x   0 zixuanrao   (501) staff       (20)        0 2023-05-11 17:50:36.855940 flasgger-0.9.7b2/flasgger/ui2/templates/flasgger/
+-rw-r--r--   0 zixuanrao   (501) staff       (20)     7263 2023-05-05 16:18:04.000000 flasgger-0.9.7b2/flasgger/ui2/templates/flasgger/index.html
+-rw-r--r--   0 zixuanrao   (501) staff       (20)     6222 2020-12-23 09:11:59.000000 flasgger-0.9.7b2/flasgger/ui2/templates/flasgger/index_old.html
+-rw-r--r--   0 zixuanrao   (501) staff       (20)      479 2020-12-23 09:11:59.000000 flasgger-0.9.7b2/flasgger/ui2/templates/flasgger/o2c.html
+drwxr-xr-x   0 zixuanrao   (501) staff       (20)        0 2023-05-11 17:50:36.767165 flasgger-0.9.7b2/flasgger/ui3/
+drwxr-xr-x   0 zixuanrao   (501) staff       (20)        0 2023-05-11 17:50:36.879615 flasgger-0.9.7b2/flasgger/ui3/static/
+-rw-r--r--   0 zixuanrao   (501) staff       (20)      665 2020-12-23 09:19:56.000000 flasgger-0.9.7b2/flasgger/ui3/static/favicon-16x16.png
+-rw-r--r--   0 zixuanrao   (501) staff       (20)      628 2020-12-23 09:19:56.000000 flasgger-0.9.7b2/flasgger/ui3/static/favicon-32x32.png
+drwxr-xr-x   0 zixuanrao   (501) staff       (20)        0 2023-05-11 17:50:36.883968 flasgger-0.9.7b2/flasgger/ui3/static/lib/
+-rw-r--r--   0 zixuanrao   (501) staff       (20)    85578 2020-12-23 09:11:59.000000 flasgger-0.9.7b2/flasgger/ui3/static/lib/jquery.min.js
+-rw-r--r--   0 zixuanrao   (501) staff       (20)   129572 2020-12-23 09:11:59.000000 flasgger-0.9.7b2/flasgger/ui3/static/lib/jquery.min.map
+-rw-r--r--   0 zixuanrao   (501) staff       (20)  1002172 2020-12-23 09:19:56.000000 flasgger-0.9.7b2/flasgger/ui3/static/swagger-ui-bundle.js
+-rw-r--r--   0 zixuanrao   (501) staff       (20)  4277142 2020-12-23 09:19:56.000000 flasgger-0.9.7b2/flasgger/ui3/static/swagger-ui-bundle.js.map
+-rw-r--r--   0 zixuanrao   (501) staff       (20)   310590 2020-12-23 09:19:56.000000 flasgger-0.9.7b2/flasgger/ui3/static/swagger-ui-standalone-preset.js
+-rw-r--r--   0 zixuanrao   (501) staff       (20)  1381697 2020-12-23 09:19:56.000000 flasgger-0.9.7b2/flasgger/ui3/static/swagger-ui-standalone-preset.js.map
+-rw-r--r--   0 zixuanrao   (501) staff       (20)   142690 2020-12-23 09:19:56.000000 flasgger-0.9.7b2/flasgger/ui3/static/swagger-ui.css
+-rw-r--r--   0 zixuanrao   (501) staff       (20)   280799 2020-12-23 09:19:56.000000 flasgger-0.9.7b2/flasgger/ui3/static/swagger-ui.css.map
+-rw-r--r--   0 zixuanrao   (501) staff       (20)   399813 2020-12-23 09:19:56.000000 flasgger-0.9.7b2/flasgger/ui3/static/swagger-ui.js
+-rw-r--r--   0 zixuanrao   (501) staff       (20)  1322743 2020-12-23 09:19:56.000000 flasgger-0.9.7b2/flasgger/ui3/static/swagger-ui.js.map
+drwxr-xr-x   0 zixuanrao   (501) staff       (20)        0 2023-05-11 17:50:36.767234 flasgger-0.9.7b2/flasgger/ui3/templates/
+drwxr-xr-x   0 zixuanrao   (501) staff       (20)        0 2023-05-11 17:50:36.888669 flasgger-0.9.7b2/flasgger/ui3/templates/flasgger/
+-rw-r--r--   0 zixuanrao   (501) staff       (20)      176 2020-12-23 09:11:59.000000 flasgger-0.9.7b2/flasgger/ui3/templates/flasgger/body_scripts.html
+-rw-r--r--   0 zixuanrao   (501) staff       (20)      108 2020-12-23 09:11:59.000000 flasgger-0.9.7b2/flasgger/ui3/templates/flasgger/custom_head.html
+-rw-r--r--   0 zixuanrao   (501) staff       (20)      384 2020-12-23 09:11:59.000000 flasgger-0.9.7b2/flasgger/ui3/templates/flasgger/footer.html
+-rw-r--r--   0 zixuanrao   (501) staff       (20)      659 2020-12-23 09:11:59.000000 flasgger-0.9.7b2/flasgger/ui3/templates/flasgger/head.html
+-rw-r--r--   0 zixuanrao   (501) staff       (20)     1152 2020-12-23 09:11:59.000000 flasgger-0.9.7b2/flasgger/ui3/templates/flasgger/index.html
+-rw-r--r--   0 zixuanrao   (501) staff       (20)     2388 2020-12-23 09:11:59.000000 flasgger-0.9.7b2/flasgger/ui3/templates/flasgger/oauth2-redirect.html
+-rw-r--r--   0 zixuanrao   (501) staff       (20)     2535 2023-05-05 16:18:04.000000 flasgger-0.9.7b2/flasgger/ui3/templates/flasgger/swagger.html
+-rw-r--r--   0 zixuanrao   (501) staff       (20)      168 2020-12-23 09:11:59.000000 flasgger-0.9.7b2/flasgger/ui3/templates/flasgger/top.html
+-rw-r--r--   0 zixuanrao   (501) staff       (20)    35825 2023-05-10 04:03:14.000000 flasgger-0.9.7b2/flasgger/utils.py
+drwxr-xr-x   0 zixuanrao   (501) staff       (20)        0 2023-05-11 17:50:36.832691 flasgger-0.9.7b2/flasgger.egg-info/
+-rw-r--r--   0 zixuanrao   (501) staff       (20)    28394 2023-05-11 17:50:36.000000 flasgger-0.9.7b2/flasgger.egg-info/PKG-INFO
+-rw-r--r--   0 zixuanrao   (501) staff       (20)    13348 2023-05-11 17:50:36.000000 flasgger-0.9.7b2/flasgger.egg-info/SOURCES.txt
+-rw-r--r--   0 zixuanrao   (501) staff       (20)        1 2023-05-11 17:50:36.000000 flasgger-0.9.7b2/flasgger.egg-info/dependency_links.txt
+-rw-r--r--   0 zixuanrao   (501) staff       (20)       77 2023-05-11 17:50:36.000000 flasgger-0.9.7b2/flasgger.egg-info/entry_points.txt
+-rw-r--r--   0 zixuanrao   (501) staff       (20)        1 2020-12-23 09:23:44.000000 flasgger-0.9.7b2/flasgger.egg-info/not-zip-safe
+-rw-r--r--   0 zixuanrao   (501) staff       (20)       72 2023-05-11 17:50:36.000000 flasgger-0.9.7b2/flasgger.egg-info/requires.txt
+-rw-r--r--   0 zixuanrao   (501) staff       (20)        9 2023-05-11 17:50:36.000000 flasgger-0.9.7b2/flasgger.egg-info/top_level.txt
+-rw-r--r--   0 zixuanrao   (501) staff       (20)       67 2023-05-11 17:50:36.895027 flasgger-0.9.7b2/setup.cfg
+-rw-r--r--   0 zixuanrao   (501) staff       (20)     1623 2023-05-10 18:08:22.000000 flasgger-0.9.7b2/setup.py
+drwxr-xr-x   0 zixuanrao   (501) staff       (20)        0 2023-05-11 17:50:36.890341 flasgger-0.9.7b2/tests/
+drwxr-xr-x   0 zixuanrao   (501) staff       (20)        0 2023-05-11 17:50:36.894199 flasgger-0.9.7b2/tests/__pycache__/
+-rw-r--r--   0 zixuanrao   (501) staff       (20)     5520 2023-05-10 16:57:33.000000 flasgger-0.9.7b2/tests/__pycache__/conftest.cpython-311-pytest-7.3.1.pyc
+-rw-r--r--   0 zixuanrao   (501) staff       (20)     2593 2020-12-23 09:21:52.000000 flasgger-0.9.7b2/tests/__pycache__/conftest.cpython-38-pytest-6.1.1.pyc
+-rw-r--r--   0 zixuanrao   (501) staff       (20)     3230 2023-05-10 14:34:58.000000 flasgger-0.9.7b2/tests/__pycache__/conftest.cpython-39-pytest-7.3.1.pyc
+-rw-r--r--   0 zixuanrao   (501) staff       (20)     2917 2023-05-10 16:57:34.000000 flasgger-0.9.7b2/tests/__pycache__/test_apispecs.cpython-311-pytest-7.3.1.pyc
+-rw-r--r--   0 zixuanrao   (501) staff       (20)     1692 2023-05-10 03:54:22.000000 flasgger-0.9.7b2/tests/__pycache__/test_apispecs.cpython-39-pytest-7.3.1.pyc
+-rw-r--r--   0 zixuanrao   (501) staff       (20)    13768 2023-05-10 16:57:34.000000 flasgger-0.9.7b2/tests/__pycache__/test_base.cpython-311-pytest-7.3.1.pyc
+-rw-r--r--   0 zixuanrao   (501) staff       (20)     5334 2023-05-10 03:54:22.000000 flasgger-0.9.7b2/tests/__pycache__/test_base.cpython-39-pytest-7.3.1.pyc
+-rw-r--r--   0 zixuanrao   (501) staff       (20)    10027 2023-05-10 16:57:34.000000 flasgger-0.9.7b2/tests/__pycache__/test_commands.cpython-311-pytest-7.3.1.pyc
+-rw-r--r--   0 zixuanrao   (501) staff       (20)     4251 2023-05-10 03:54:22.000000 flasgger-0.9.7b2/tests/__pycache__/test_commands.cpython-39-pytest-7.3.1.pyc
+-rw-r--r--   0 zixuanrao   (501) staff       (20)     4376 2023-05-10 16:57:34.000000 flasgger-0.9.7b2/tests/__pycache__/test_examples.cpython-311-pytest-7.3.1.pyc
+-rw-r--r--   0 zixuanrao   (501) staff       (20)     2891 2023-05-10 03:54:22.000000 flasgger-0.9.7b2/tests/__pycache__/test_examples.cpython-39-pytest-7.3.1.pyc
+-rw-r--r--   0 zixuanrao   (501) staff       (20)     5736 2023-05-10 16:57:35.000000 flasgger-0.9.7b2/tests/__pycache__/test_utils.cpython-311-pytest-7.3.1.pyc
+-rw-r--r--   0 zixuanrao   (501) staff       (20)     1848 2023-05-10 03:54:22.000000 flasgger-0.9.7b2/tests/__pycache__/test_utils.cpython-39-pytest-7.3.1.pyc
+-rw-r--r--   0 zixuanrao   (501) staff       (20)     2998 2023-05-10 05:56:35.000000 flasgger-0.9.7b2/tests/conftest.py
+-rwxr-xr-x   0 zixuanrao   (501) staff       (20)      574 2023-05-05 16:18:04.000000 flasgger-0.9.7b2/tests/test_apispecs.py
+-rw-r--r--   0 zixuanrao   (501) staff       (20)     2102 2021-04-13 07:52:00.000000 flasgger-0.9.7b2/tests/test_base.py
+-rw-r--r--   0 zixuanrao   (501) staff       (20)     1403 2023-05-05 16:18:04.000000 flasgger-0.9.7b2/tests/test_commands.py
+-rw-r--r--   0 zixuanrao   (501) staff       (20)     2399 2020-12-23 09:11:59.000000 flasgger-0.9.7b2/tests/test_examples.py
+-rw-r--r--   0 zixuanrao   (501) staff       (20)      378 2021-04-13 07:52:00.000000 flasgger-0.9.7b2/tests/test_utils.py
```

### Comparing `flasgger-0.9.7.1/CODE_OF_CONDUCT.md` & `flasgger-0.9.7b2/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `flasgger-0.9.7.1/LICENSE` & `flasgger-0.9.7b2/LICENSE`

 * *Files identical despite different names*

### Comparing `flasgger-0.9.7.1/MANIFEST.in` & `flasgger-0.9.7b2/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `flasgger-0.9.7.1/PKG-INFO` & `flasgger-0.9.7b2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flasgger
-Version: 0.9.7.1
+Version: 0.9.7b2
 Summary: Extract swagger specs from your flask project
 Home-page: https://github.com/flasgger/flasgger/
 Author: Bruno Rocha, Zixuan Rao, Flasgger team
 Author-email: flasgger@flasgger.org
 License: MIT
 Platform: any
 Classifier: Intended Audience :: Developers
@@ -94,30 +94,24 @@
 > under your virtualenv do:
 
 Ensure you have latest setuptools
 ```
 pip install -U setuptools
 ```
 
-then install beta version (recommended)
+then
 
 ```
-pip install flasgger==0.9.7b2
-```
-
-or (latest stable for legacy apps)
-
-```
-pip install flasgger==0.9.5
+pip install flasgger
 ```
 
 or (dev version)
 
 ```
-pip install https://github.com/flasgger/flasgger/tarball/master
+pip install https://github.com/rochacbruno/flasgger/tarball/master
 ```
 
 > NOTE: If you want to use **Marshmallow Schemas** you also need to run `pip install marshmallow apispec`
 
 ## How to run tests
 
 (You may see the command in [.travis.yml](./.travis.yml) for `before_install` part)
```

### Comparing `flasgger-0.9.7.1/README.md` & `flasgger-0.9.7b2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -79,30 +79,24 @@
 > under your virtualenv do:
 
 Ensure you have latest setuptools
 ```
 pip install -U setuptools
 ```
 
-then install beta version (recommended)
+then
 
 ```
-pip install flasgger==0.9.7b2
-```
-
-or (latest stable for legacy apps)
-
-```
-pip install flasgger==0.9.5
+pip install flasgger
 ```
 
 or (dev version)
 
 ```
-pip install https://github.com/flasgger/flasgger/tarball/master
+pip install https://github.com/rochacbruno/flasgger/tarball/master
 ```
 
 > NOTE: If you want to use **Marshmallow Schemas** you also need to run `pip install marshmallow apispec`
 
 ## How to run tests
 
 (You may see the command in [.travis.yml](./.travis.yml) for `before_install` part)
```

### Comparing `flasgger-0.9.7.1/README.zh.md` & `flasgger-0.9.7b2/README.zh.md`

 * *Files identical despite different names*

### Comparing `flasgger-0.9.7.1/demo_app/app.py` & `flasgger-0.9.7b2/demo_app/app.py`

 * *Files identical despite different names*

### Comparing `flasgger-0.9.7.1/demo_app/templates/flasgger.html` & `flasgger-0.9.7b2/demo_app/templates/flasgger.html`

 * *Files identical despite different names*

### Comparing `flasgger-0.9.7.1/etc/.DS_Store` & `flasgger-0.9.7b2/etc/.DS_Store`

 * *Files identical despite different names*

### Comparing `flasgger-0.9.7.1/etc/flasgger_package/build/lib/flasgger_package/package_specs.yml` & `flasgger-0.9.7b2/etc/flasgger_package/build/lib/flasgger_package/package_specs.yml`

 * *Files identical despite different names*

### Comparing `flasgger-0.9.7.1/etc/flasgger_package/dist/flasgger_package-0.0.1-py3.11.egg` & `flasgger-0.9.7b2/etc/flasgger_package/dist/flasgger_package-0.0.1-py3.11.egg`

 * *Files identical despite different names*

### Comparing `flasgger-0.9.7.1/etc/flasgger_package/dist/flasgger_package-0.0.1-py3.8.egg` & `flasgger-0.9.7b2/etc/flasgger_package/dist/flasgger_package-0.0.1-py3.8.egg`

 * *Files identical despite different names*

### Comparing `flasgger-0.9.7.1/etc/flasgger_package/dist/flasgger_package-0.0.1-py3.9.egg` & `flasgger-0.9.7b2/etc/flasgger_package/dist/flasgger_package-0.0.1-py3.9.egg`

 * *Files identical despite different names*

### Comparing `flasgger-0.9.7.1/etc/flasgger_package/flasgger_package/package_specs.yml` & `flasgger-0.9.7b2/etc/flasgger_package/flasgger_package/package_specs.yml`

 * *Files identical despite different names*

### Comparing `flasgger-0.9.7.1/etc/flasgger_package/setup.py` & `flasgger-0.9.7b2/etc/flasgger_package/setup.py`

 * *Files identical despite different names*

### Comparing `flasgger-0.9.7.1/etc/pythonanywhere/pythonanywhere_com_wsgi.py` & `flasgger-0.9.7b2/etc/pythonanywhere/pythonanywhere_com_wsgi.py`

 * *Files identical despite different names*

### Comparing `flasgger-0.9.7.1/examples/README.md` & `flasgger-0.9.7b2/examples/README.md`

 * *Files identical despite different names*

### Comparing `flasgger-0.9.7.1/examples/__pycache__/apispec_example.cpython-311.pyc` & `flasgger-0.9.7b2/examples/__pycache__/apispec_example.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `flasgger-0.9.7.1/examples/__pycache__/apispec_example.cpython-39.pyc` & `flasgger-0.9.7b2/examples/__pycache__/apispec_example.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `flasgger-0.9.7.1/examples/__pycache__/apispec_example_uiversion3.cpython-311.pyc` & `flasgger-0.9.7b2/examples/__pycache__/apispec_example_uiversion3.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `flasgger-0.9.7.1/examples/__pycache__/apispec_example_uiversion3.cpython-39.pyc` & `flasgger-0.9.7b2/examples/__pycache__/apispec_example_uiversion3.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `flasgger-0.9.7.1/examples/__pycache__/base_model_view.cpython-311.pyc` & `flasgger-0.9.7b2/examples/__pycache__/base_model_view.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `flasgger-0.9.7.1/examples/__pycache__/base_model_view.cpython-39.pyc` & `flasgger-0.9.7b2/examples/__pycache__/base_model_view.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `flasgger-0.9.7.1/examples/__pycache__/basic_auth.cpython-311.pyc` & `flasgger-0.9.7b2/examples/__pycache__/basic_auth.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `flasgger-0.9.7.1/examples/__pycache__/basic_auth.cpython-39.pyc` & `flasgger-0.9.7b2/examples/__pycache__/basic_auth.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `flasgger-0.9.7.1/examples/__pycache__/callbacks.cpython-311.pyc` & `flasgger-0.9.7b2/examples/__pycache__/callbacks.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `flasgger-0.9.7.1/examples/__pycache__/callbacks.cpython-39.pyc` & `flasgger-0.9.7b2/examples/__pycache__/callbacks.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `flasgger-0.9.7.1/examples/__pycache__/changelog_090.cpython-311.pyc` & `flasgger-0.9.7b2/examples/__pycache__/changelog_090.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `flasgger-0.9.7.1/examples/__pycache__/changelog_090.cpython-39.pyc` & `flasgger-0.9.7b2/examples/__pycache__/changelog_090.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `flasgger-0.9.7.1/examples/__pycache__/colors.cpython-311.pyc` & `flasgger-0.9.7b2/examples/__pycache__/colors.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `flasgger-0.9.7.1/examples/__pycache__/colors.cpython-39.pyc` & `flasgger-0.9.7b2/examples/__pycache__/colors.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `flasgger-0.9.7.1/examples/__pycache__/colors_external_js.cpython-311.pyc` & `flasgger-0.9.7b2/examples/__pycache__/colors_external_js.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `flasgger-0.9.7.1/examples/__pycache__/colors_external_js.cpython-39.pyc` & `flasgger-0.9.7b2/examples/__pycache__/colors_external_js.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `flasgger-0.9.7.1/examples/__pycache__/colors_from_specdict.cpython-311.pyc` & `flasgger-0.9.7b2/examples/__pycache__/colors_from_specdict.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `flasgger-0.9.7.1/examples/__pycache__/colors_from_specdict.cpython-39.pyc` & `flasgger-0.9.7b2/examples/__pycache__/colors_from_specdict.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `flasgger-0.9.7.1/examples/__pycache__/colors_template_json.cpython-311.pyc` & `flasgger-0.9.7b2/examples/__pycache__/colors_template_json.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `flasgger-0.9.7.1/examples/__pycache__/colors_template_json.cpython-39.pyc` & `flasgger-0.9.7b2/examples/__pycache__/colors_template_json.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `flasgger-0.9.7.1/examples/__pycache__/colors_template_yaml.cpython-311.pyc` & `flasgger-0.9.7b2/examples/__pycache__/colors_template_yaml.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `flasgger-0.9.7.1/examples/__pycache__/colors_template_yaml.cpython-39.pyc` & `flasgger-0.9.7b2/examples/__pycache__/colors_template_yaml.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `flasgger-0.9.7.1/examples/__pycache__/colors_uiversion2.cpython-311.pyc` & `flasgger-0.9.7b2/examples/__pycache__/colors_uiversion2.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `flasgger-0.9.7.1/examples/__pycache__/colors_uiversion2.cpython-39.pyc` & `flasgger-0.9.7b2/examples/__pycache__/colors_uiversion2.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `flasgger-0.9.7.1/examples/__pycache__/colors_with_schema.cpython-311.pyc` & `flasgger-0.9.7b2/examples/__pycache__/colors_with_schema.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `flasgger-0.9.7.1/examples/__pycache__/colors_with_schema.cpython-39.pyc` & `flasgger-0.9.7b2/examples/__pycache__/colors_with_schema.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `flasgger-0.9.7.1/examples/__pycache__/compat.cpython-311.pyc` & `flasgger-0.9.7b2/examples/__pycache__/compat.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `flasgger-0.9.7.1/examples/__pycache__/compat.cpython-39.pyc` & `flasgger-0.9.7b2/examples/__pycache__/compat.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `flasgger-0.9.7.1/examples/__pycache__/custom_validation_function.cpython-311.pyc` & `flasgger-0.9.7b2/examples/__pycache__/custom_validation_function.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `flasgger-0.9.7.1/examples/__pycache__/custom_validation_function.cpython-39.pyc` & `flasgger-0.9.7b2/examples/__pycache__/custom_validation_function.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `flasgger-0.9.7.1/examples/__pycache__/decorator_package.cpython-311.pyc` & `flasgger-0.9.7b2/examples/__pycache__/decorator_package.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `flasgger-0.9.7.1/examples/__pycache__/decorator_package.cpython-39.pyc` & `flasgger-0.9.7b2/examples/__pycache__/decorator_package.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `flasgger-0.9.7.1/examples/__pycache__/decorators_in_init_app.cpython-311.pyc` & `flasgger-0.9.7b2/examples/__pycache__/decorators_in_init_app.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `flasgger-0.9.7.1/examples/__pycache__/decorators_in_init_app.cpython-39.pyc` & `flasgger-0.9.7b2/examples/__pycache__/decorators_in_init_app.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `flasgger-0.9.7.1/examples/__pycache__/definition_object_test.cpython-311-pytest-7.3.1.pyc` & `flasgger-0.9.7b2/examples/__pycache__/definition_object_test.cpython-311-pytest-7.3.1.pyc`

 * *Files identical despite different names*

### Comparing `flasgger-0.9.7.1/examples/__pycache__/definition_object_test.cpython-39-pytest-7.3.1.pyc` & `flasgger-0.9.7b2/examples/__pycache__/definition_object_test.cpython-39-pytest-7.3.1.pyc`

 * *Files identical despite different names*

### Comparing `flasgger-0.9.7.1/examples/__pycache__/disable_swagger_ui.cpython-311.pyc` & `flasgger-0.9.7b2/examples/__pycache__/disable_swagger_ui.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `flasgger-0.9.7.1/examples/__pycache__/disable_swagger_ui.cpython-39.pyc` & `flasgger-0.9.7b2/examples/__pycache__/disable_swagger_ui.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `flasgger-0.9.7.1/examples/__pycache__/example_app.cpython-311.pyc` & `flasgger-0.9.7b2/examples/__pycache__/example_app.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `flasgger-0.9.7.1/examples/__pycache__/example_app.cpython-39.pyc` & `flasgger-0.9.7b2/examples/__pycache__/example_app.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `flasgger-0.9.7.1/examples/__pycache__/example_blueprint.cpython-311.pyc` & `flasgger-0.9.7b2/examples/__pycache__/example_blueprint.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `flasgger-0.9.7.1/examples/__pycache__/example_blueprint.cpython-39.pyc` & `flasgger-0.9.7b2/examples/__pycache__/example_blueprint.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `flasgger-0.9.7.1/examples/__pycache__/get_schema.cpython-311.pyc` & `flasgger-0.9.7b2/examples/__pycache__/get_schema.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `flasgger-0.9.7.1/examples/__pycache__/get_schema.cpython-39.pyc` & `flasgger-0.9.7b2/examples/__pycache__/get_schema.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `flasgger-0.9.7.1/examples/__pycache__/lazy_string.cpython-311.pyc` & `flasgger-0.9.7b2/examples/__pycache__/lazy_string.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `flasgger-0.9.7.1/examples/__pycache__/lazy_string.cpython-39.pyc` & `flasgger-0.9.7b2/examples/__pycache__/lazy_string.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `flasgger-0.9.7.1/examples/__pycache__/marshmallow_apispec.cpython-311.pyc` & `flasgger-0.9.7b2/examples/__pycache__/marshmallow_apispec.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `flasgger-0.9.7.1/examples/__pycache__/marshmallow_apispec.cpython-39.pyc` & `flasgger-0.9.7b2/examples/__pycache__/marshmallow_apispec.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `flasgger-0.9.7.1/examples/__pycache__/multiple_specs_dropdown_example.cpython-311.pyc` & `flasgger-0.9.7b2/examples/__pycache__/multiple_specs_dropdown_example.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `flasgger-0.9.7.1/examples/__pycache__/multiple_specs_dropdown_example.cpython-39.pyc` & `flasgger-0.9.7b2/examples/__pycache__/multiple_specs_dropdown_example.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `flasgger-0.9.7.1/examples/__pycache__/no_routes.cpython-311.pyc` & `flasgger-0.9.7b2/examples/__pycache__/no_routes.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `flasgger-0.9.7.1/examples/__pycache__/no_routes.cpython-39.pyc` & `flasgger-0.9.7b2/examples/__pycache__/no_routes.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `flasgger-0.9.7.1/examples/__pycache__/openapi3_examples.cpython-311.pyc` & `flasgger-0.9.7b2/examples/__pycache__/openapi3_examples.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `flasgger-0.9.7.1/examples/__pycache__/openapi3_examples.cpython-39.pyc` & `flasgger-0.9.7b2/examples/__pycache__/openapi3_examples.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `flasgger-0.9.7.1/examples/__pycache__/package_example.cpython-311.pyc` & `flasgger-0.9.7b2/examples/__pycache__/package_example.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `flasgger-0.9.7.1/examples/__pycache__/package_example.cpython-39.pyc` & `flasgger-0.9.7b2/examples/__pycache__/package_example.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `flasgger-0.9.7.1/examples/__pycache__/parse_openapi3.cpython-311.pyc` & `flasgger-0.9.7b2/examples/__pycache__/parse_openapi3.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `flasgger-0.9.7.1/examples/__pycache__/parse_openapi3.cpython-39.pyc` & `flasgger-0.9.7b2/examples/__pycache__/parse_openapi3.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `flasgger-0.9.7.1/examples/__pycache__/parse_openapi3_json.cpython-311.pyc` & `flasgger-0.9.7b2/examples/__pycache__/parse_openapi3_json.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `flasgger-0.9.7.1/examples/__pycache__/parse_openapi3_json.cpython-39.pyc` & `flasgger-0.9.7b2/examples/__pycache__/parse_openapi3_json.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `flasgger-0.9.7.1/examples/__pycache__/parsed_view_func.cpython-311.pyc` & `flasgger-0.9.7b2/examples/__pycache__/parsed_view_func.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `flasgger-0.9.7.1/examples/__pycache__/parsed_view_func.cpython-39.pyc` & `flasgger-0.9.7b2/examples/__pycache__/parsed_view_func.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `flasgger-0.9.7.1/examples/__pycache__/request_body.cpython-311.pyc` & `flasgger-0.9.7b2/examples/__pycache__/request_body.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `flasgger-0.9.7.1/examples/__pycache__/request_body.cpython-39.pyc` & `flasgger-0.9.7b2/examples/__pycache__/request_body.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `flasgger-0.9.7.1/examples/__pycache__/restful.cpython-311.pyc` & `flasgger-0.9.7b2/examples/__pycache__/restful.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `flasgger-0.9.7.1/examples/__pycache__/restful.cpython-39.pyc` & `flasgger-0.9.7b2/examples/__pycache__/restful.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `flasgger-0.9.7.1/examples/__pycache__/specs_route_example.cpython-311.pyc` & `flasgger-0.9.7b2/examples/__pycache__/specs_route_example.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `flasgger-0.9.7.1/examples/__pycache__/specs_route_example.cpython-39.pyc` & `flasgger-0.9.7b2/examples/__pycache__/specs_route_example.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `flasgger-0.9.7.1/examples/__pycache__/swag_annotation.cpython-311.pyc` & `flasgger-0.9.7b2/examples/__pycache__/swag_annotation.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `flasgger-0.9.7.1/examples/__pycache__/swag_annotation.cpython-39.pyc` & `flasgger-0.9.7b2/examples/__pycache__/swag_annotation.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `flasgger-0.9.7.1/examples/__pycache__/swag_from_merging.cpython-311.pyc` & `flasgger-0.9.7b2/examples/__pycache__/swag_from_merging.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `flasgger-0.9.7.1/examples/__pycache__/swag_from_merging.cpython-39.pyc` & `flasgger-0.9.7b2/examples/__pycache__/swag_from_merging.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `flasgger-0.9.7.1/examples/__pycache__/swag_from_overriding.cpython-311.pyc` & `flasgger-0.9.7b2/examples/__pycache__/swag_from_overriding.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `flasgger-0.9.7.1/examples/__pycache__/swag_from_overriding.cpython-39.pyc` & `flasgger-0.9.7b2/examples/__pycache__/swag_from_overriding.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `flasgger-0.9.7.1/examples/__pycache__/swagger_config_2.cpython-311.pyc` & `flasgger-0.9.7b2/examples/__pycache__/swagger_config_2.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `flasgger-0.9.7.1/examples/__pycache__/swagger_config_2.cpython-39.pyc` & `flasgger-0.9.7b2/examples/__pycache__/swagger_config_2.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `flasgger-0.9.7.1/examples/__pycache__/swagger_config_3.cpython-311.pyc` & `flasgger-0.9.7b2/examples/__pycache__/swagger_config_3.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `flasgger-0.9.7.1/examples/__pycache__/swagger_config_3.cpython-39.pyc` & `flasgger-0.9.7b2/examples/__pycache__/swagger_config_3.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `flasgger-0.9.7.1/examples/__pycache__/swagger_config_3_with_components_schemas.cpython-311.pyc` & `flasgger-0.9.7b2/examples/__pycache__/swagger_config_3_with_components_schemas.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `flasgger-0.9.7.1/examples/__pycache__/swagger_config_3_with_components_schemas.cpython-39.pyc` & `flasgger-0.9.7b2/examples/__pycache__/swagger_config_3_with_components_schemas.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `flasgger-0.9.7.1/examples/__pycache__/swagger_config_merge.cpython-311.pyc` & `flasgger-0.9.7b2/examples/__pycache__/swagger_config_merge.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `flasgger-0.9.7.1/examples/__pycache__/swagger_config_merge.cpython-39.pyc` & `flasgger-0.9.7b2/examples/__pycache__/swagger_config_merge.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `flasgger-0.9.7.1/examples/__pycache__/test_refs.cpython-311-pytest-7.3.1.pyc` & `flasgger-0.9.7b2/examples/__pycache__/test_refs.cpython-311-pytest-7.3.1.pyc`

 * *Files identical despite different names*

### Comparing `flasgger-0.9.7.1/examples/__pycache__/test_refs.cpython-39-pytest-7.3.1.pyc` & `flasgger-0.9.7b2/examples/__pycache__/test_refs.cpython-39-pytest-7.3.1.pyc`

 * *Files identical despite different names*

### Comparing `flasgger-0.9.7.1/examples/__pycache__/top_level_vendor_extension.cpython-311.pyc` & `flasgger-0.9.7b2/examples/__pycache__/top_level_vendor_extension.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `flasgger-0.9.7.1/examples/__pycache__/top_level_vendor_extension.cpython-39.pyc` & `flasgger-0.9.7b2/examples/__pycache__/top_level_vendor_extension.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `flasgger-0.9.7.1/examples/__pycache__/use_openapi.cpython-311.pyc` & `flasgger-0.9.7b2/examples/__pycache__/use_openapi.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `flasgger-0.9.7.1/examples/__pycache__/use_openapi.cpython-39.pyc` & `flasgger-0.9.7b2/examples/__pycache__/use_openapi.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `flasgger-0.9.7.1/examples/__pycache__/validation.cpython-311.pyc` & `flasgger-0.9.7b2/examples/__pycache__/validation.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `flasgger-0.9.7.1/examples/__pycache__/validation.cpython-39.pyc` & `flasgger-0.9.7b2/examples/__pycache__/validation.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `flasgger-0.9.7.1/examples/__pycache__/validation_error_handler.cpython-311.pyc` & `flasgger-0.9.7b2/examples/__pycache__/validation_error_handler.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `flasgger-0.9.7.1/examples/__pycache__/validation_error_handler.cpython-39.pyc` & `flasgger-0.9.7b2/examples/__pycache__/validation_error_handler.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `flasgger-0.9.7.1/examples/apispec_example.py` & `flasgger-0.9.7b2/examples/apispec_example.py`

 * *Files identical despite different names*

### Comparing `flasgger-0.9.7.1/examples/apispec_example_uiversion3.py` & `flasgger-0.9.7b2/examples/apispec_example_uiversion3.py`

 * *Files identical despite different names*

### Comparing `flasgger-0.9.7.1/examples/base_model_view.py` & `flasgger-0.9.7b2/examples/base_model_view.py`

 * *Files identical despite different names*

### Comparing `flasgger-0.9.7.1/examples/basic_auth.py` & `flasgger-0.9.7b2/examples/basic_auth.py`

 * *Files identical despite different names*

### Comparing `flasgger-0.9.7.1/examples/callbacks.py` & `flasgger-0.9.7b2/examples/callbacks.py`

 * *Files identical despite different names*

### Comparing `flasgger-0.9.7.1/examples/changelog_090.py` & `flasgger-0.9.7b2/examples/changelog_090.py`

 * *Files identical despite different names*

### Comparing `flasgger-0.9.7.1/examples/colors.py` & `flasgger-0.9.7b2/examples/colors.py`

 * *Files identical despite different names*

### Comparing `flasgger-0.9.7.1/examples/colors_external_js.py` & `flasgger-0.9.7b2/examples/colors_external_js.py`

 * *Files identical despite different names*

### Comparing `flasgger-0.9.7.1/examples/colors_from_specdict.py` & `flasgger-0.9.7b2/examples/colors_from_specdict.py`

 * *Files identical despite different names*

### Comparing `flasgger-0.9.7.1/examples/colors_template.json` & `flasgger-0.9.7b2/examples/colors_template.json`

 * *Files identical despite different names*

### Comparing `flasgger-0.9.7.1/examples/colors_template.yaml` & `flasgger-0.9.7b2/examples/colors_template.yaml`

 * *Files identical despite different names*

### Comparing `flasgger-0.9.7.1/examples/colors_template_json.py` & `flasgger-0.9.7b2/examples/colors_template_json.py`

 * *Files identical despite different names*

### Comparing `flasgger-0.9.7.1/examples/colors_template_yaml.py` & `flasgger-0.9.7b2/examples/colors_template_yaml.py`

 * *Files identical despite different names*

### Comparing `flasgger-0.9.7.1/examples/colors_uiversion2.py` & `flasgger-0.9.7b2/examples/colors_uiversion2.py`

 * *Files identical despite different names*

### Comparing `flasgger-0.9.7.1/examples/colors_with_schema.py` & `flasgger-0.9.7b2/examples/colors_with_schema.py`

 * *Files identical despite different names*

### Comparing `flasgger-0.9.7.1/examples/compat.py` & `flasgger-0.9.7b2/examples/compat.py`

 * *Files identical despite different names*

### Comparing `flasgger-0.9.7.1/examples/custom_validation_function.py` & `flasgger-0.9.7b2/examples/custom_validation_function.py`

 * *Files identical despite different names*

### Comparing `flasgger-0.9.7.1/examples/decorator_package.py` & `flasgger-0.9.7b2/examples/decorator_package.py`

 * *Files identical despite different names*

### Comparing `flasgger-0.9.7.1/examples/decorators_in_init_app.py` & `flasgger-0.9.7b2/examples/decorators_in_init_app.py`

 * *Files identical despite different names*

### Comparing `flasgger-0.9.7.1/examples/definition_object_test.py` & `flasgger-0.9.7b2/examples/definition_object_test.py`

 * *Files identical despite different names*

### Comparing `flasgger-0.9.7.1/examples/disable_swagger_ui.py` & `flasgger-0.9.7b2/examples/disable_swagger_ui.py`

 * *Files identical despite different names*

### Comparing `flasgger-0.9.7.1/examples/example_app.py` & `flasgger-0.9.7b2/examples/example_app.py`

 * *Files identical despite different names*

### Comparing `flasgger-0.9.7.1/examples/example_blueprint.py` & `flasgger-0.9.7b2/examples/example_blueprint.py`

 * *Files identical despite different names*

### Comparing `flasgger-0.9.7.1/examples/get_schema.py` & `flasgger-0.9.7b2/examples/get_schema.py`

 * *Files identical despite different names*

### Comparing `flasgger-0.9.7.1/examples/lazy_string.py` & `flasgger-0.9.7b2/examples/lazy_string.py`

 * *Files identical despite different names*

### Comparing `flasgger-0.9.7.1/examples/legacy/jwt_auth.py` & `flasgger-0.9.7b2/examples/legacy/jwt_auth.py`

 * *Files identical despite different names*

### Comparing `flasgger-0.9.7.1/examples/marshmallow_apispec.py` & `flasgger-0.9.7b2/examples/marshmallow_apispec.py`

 * *Files identical despite different names*

### Comparing `flasgger-0.9.7.1/examples/multiple_specs_dropdown_example.py` & `flasgger-0.9.7b2/examples/multiple_specs_dropdown_example.py`

 * *Files identical despite different names*

### Comparing `flasgger-0.9.7.1/examples/no_routes.py` & `flasgger-0.9.7b2/examples/no_routes.py`

 * *Files identical despite different names*

### Comparing `flasgger-0.9.7.1/examples/officer_specs.yml` & `flasgger-0.9.7b2/examples/officer_specs.yml`

 * *Files identical despite different names*

### Comparing `flasgger-0.9.7.1/examples/openapi3_examples.py` & `flasgger-0.9.7b2/examples/openapi3_examples.py`

 * *Files identical despite different names*

### Comparing `flasgger-0.9.7.1/examples/package_example.py` & `flasgger-0.9.7b2/examples/package_example.py`

 * *Files identical despite different names*

### Comparing `flasgger-0.9.7.1/examples/parse_openapi3.py` & `flasgger-0.9.7b2/examples/parse_openapi3.py`

 * *Files identical despite different names*

### Comparing `flasgger-0.9.7.1/examples/parse_openapi3_json.py` & `flasgger-0.9.7b2/examples/parse_openapi3_json.py`

 * *Files identical despite different names*

### Comparing `flasgger-0.9.7.1/examples/parse_openapi3_json_product_schema.yml` & `flasgger-0.9.7b2/examples/parse_openapi3_json_product_schema.yml`

 * *Files identical despite different names*

### Comparing `flasgger-0.9.7.1/examples/parse_openapi3_product_schema.yml` & `flasgger-0.9.7b2/examples/parse_openapi3_product_schema.yml`

 * *Files identical despite different names*

### Comparing `flasgger-0.9.7.1/examples/parsed_view_func.py` & `flasgger-0.9.7b2/examples/parsed_view_func.py`

 * *Files identical despite different names*

### Comparing `flasgger-0.9.7.1/examples/request_body.py` & `flasgger-0.9.7b2/examples/request_body.py`

 * *Files identical despite different names*

### Comparing `flasgger-0.9.7.1/examples/restful.py` & `flasgger-0.9.7b2/examples/restful.py`

 * *Files identical despite different names*

### Comparing `flasgger-0.9.7.1/examples/specs_route_example.py` & `flasgger-0.9.7b2/examples/specs_route_example.py`

 * *Files identical despite different names*

### Comparing `flasgger-0.9.7.1/examples/swag_annotation.py` & `flasgger-0.9.7b2/examples/swag_annotation.py`

 * *Files identical despite different names*

### Comparing `flasgger-0.9.7.1/examples/swag_from_merging.py` & `flasgger-0.9.7b2/examples/swag_from_merging.py`

 * *Files identical despite different names*

### Comparing `flasgger-0.9.7.1/examples/swag_from_overriding.py` & `flasgger-0.9.7b2/examples/swag_from_overriding.py`

 * *Files identical despite different names*

### Comparing `flasgger-0.9.7.1/examples/swagger_config_2.py` & `flasgger-0.9.7b2/examples/swagger_config_2.py`

 * *Files identical despite different names*

### Comparing `flasgger-0.9.7.1/examples/swagger_config_3.py` & `flasgger-0.9.7b2/examples/swagger_config_3.py`

 * *Files identical despite different names*

### Comparing `flasgger-0.9.7.1/examples/swagger_config_3_with_components_schemas.py` & `flasgger-0.9.7b2/examples/swagger_config_3_with_components_schemas.py`

 * *Files identical despite different names*

### Comparing `flasgger-0.9.7.1/examples/swagger_config_merge.py` & `flasgger-0.9.7b2/examples/swagger_config_merge.py`

 * *Files identical despite different names*

### Comparing `flasgger-0.9.7.1/examples/test_refs.py` & `flasgger-0.9.7b2/examples/test_refs.py`

 * *Files identical despite different names*

### Comparing `flasgger-0.9.7.1/examples/test_refs_basePath_API.yaml` & `flasgger-0.9.7b2/examples/test_refs_basePath_API.yaml`

 * *Files identical despite different names*

### Comparing `flasgger-0.9.7.1/examples/test_validation.yml` & `flasgger-0.9.7b2/examples/test_validation.yml`

 * *Files identical despite different names*

### Comparing `flasgger-0.9.7.1/examples/top_level_vendor_extension.py` & `flasgger-0.9.7b2/examples/top_level_vendor_extension.py`

 * *Files identical despite different names*

### Comparing `flasgger-0.9.7.1/examples/use_openapi.py` & `flasgger-0.9.7b2/examples/use_openapi.py`

 * *Files identical despite different names*

### Comparing `flasgger-0.9.7.1/examples/username_specs.yml` & `flasgger-0.9.7b2/examples/username_specs.yml`

 * *Files identical despite different names*

### Comparing `flasgger-0.9.7.1/examples/username_specs_bom.yml` & `flasgger-0.9.7b2/examples/username_specs_bom.yml`

 * *Files identical despite different names*

### Comparing `flasgger-0.9.7.1/examples/username_specs_utf16.yml` & `flasgger-0.9.7b2/examples/username_specs_utf16.yml`

 * *Files identical despite different names*

### Comparing `flasgger-0.9.7.1/examples/username_specs_utf32.yml` & `flasgger-0.9.7b2/examples/username_specs_utf32.yml`

 * *Files identical despite different names*

### Comparing `flasgger-0.9.7.1/examples/validation.py` & `flasgger-0.9.7b2/examples/validation.py`

 * *Files identical despite different names*

### Comparing `flasgger-0.9.7.1/examples/validation_error_handler.py` & `flasgger-0.9.7b2/examples/validation_error_handler.py`

 * *Files identical despite different names*

### Comparing `flasgger-0.9.7.1/flasgger/.DS_Store` & `flasgger-0.9.7b2/flasgger/.DS_Store`

 * *Files identical despite different names*

### Comparing `flasgger-0.9.7.1/flasgger/__init__.py` & `flasgger-0.9.7b2/flasgger/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 
-__version__ = '0.9.7.1'
+__version__ = '0.9.7b2'
 __author__ = 'Bruno Rocha, Zixuan Rao, Flasgger team'
 __email__ = 'flasgger@flasgger.org'
 
 # Based on works of Bruno Rocha and the Flasgger open source community
 
 
 from jsonschema import ValidationError  # noqa
```

### Comparing `flasgger-0.9.7.1/flasgger/base.py` & `flasgger-0.9.7b2/flasgger/base.py`

 * *Files identical despite different names*

### Comparing `flasgger-0.9.7.1/flasgger/commands.py` & `flasgger-0.9.7b2/flasgger/commands.py`

 * *Files identical despite different names*

### Comparing `flasgger-0.9.7.1/flasgger/compatible.py` & `flasgger-0.9.7b2/flasgger/compatible.py`

 * *Files identical despite different names*

### Comparing `flasgger-0.9.7.1/flasgger/constants.py` & `flasgger-0.9.7b2/flasgger/constants.py`

 * *Files identical despite different names*

### Comparing `flasgger-0.9.7.1/flasgger/marshmallow_apispec.py` & `flasgger-0.9.7b2/flasgger/marshmallow_apispec.py`

 * *Files identical despite different names*

### Comparing `flasgger-0.9.7.1/flasgger/ui2/static/css/print.css` & `flasgger-0.9.7b2/flasgger/ui2/static/css/print.css`

 * *Files identical despite different names*

### Comparing `flasgger-0.9.7.1/flasgger/ui2/static/css/reset.css` & `flasgger-0.9.7b2/flasgger/ui2/static/css/reset.css`

 * *Files identical despite different names*

### Comparing `flasgger-0.9.7.1/flasgger/ui2/static/css/screen.css` & `flasgger-0.9.7b2/flasgger/ui2/static/css/screen.css`

 * *Files identical despite different names*

### Comparing `flasgger-0.9.7.1/flasgger/ui2/static/css/style.css` & `flasgger-0.9.7b2/flasgger/ui2/static/css/style.css`

 * *Files identical despite different names*

### Comparing `flasgger-0.9.7.1/flasgger/ui2/static/fonts/DroidSans-Bold.ttf` & `flasgger-0.9.7b2/flasgger/ui2/static/fonts/DroidSans-Bold.ttf`

 * *Files identical despite different names*

### Comparing `flasgger-0.9.7.1/flasgger/ui2/static/fonts/DroidSans.ttf` & `flasgger-0.9.7b2/flasgger/ui2/static/fonts/DroidSans.ttf`

 * *Files identical despite different names*

### Comparing `flasgger-0.9.7.1/flasgger/ui2/static/fonts/droid-sans-v6-latin-700.eot` & `flasgger-0.9.7b2/flasgger/ui2/static/fonts/droid-sans-v6-latin-700.eot`

 * *Files identical despite different names*

### Comparing `flasgger-0.9.7.1/flasgger/ui2/static/fonts/droid-sans-v6-latin-700.svg` & `flasgger-0.9.7b2/flasgger/ui2/static/fonts/droid-sans-v6-latin-700.svg`

 * *Files identical despite different names*

### Comparing `flasgger-0.9.7.1/flasgger/ui2/static/fonts/droid-sans-v6-latin-700.ttf` & `flasgger-0.9.7b2/flasgger/ui2/static/fonts/droid-sans-v6-latin-700.ttf`

 * *Files identical despite different names*

### Comparing `flasgger-0.9.7.1/flasgger/ui2/static/fonts/droid-sans-v6-latin-700.woff` & `flasgger-0.9.7b2/flasgger/ui2/static/fonts/droid-sans-v6-latin-700.woff`

 * *Files identical despite different names*

### Comparing `flasgger-0.9.7.1/flasgger/ui2/static/fonts/droid-sans-v6-latin-700.woff2` & `flasgger-0.9.7b2/flasgger/ui2/static/fonts/droid-sans-v6-latin-700.woff2`

 * *Files identical despite different names*

### Comparing `flasgger-0.9.7.1/flasgger/ui2/static/fonts/droid-sans-v6-latin-regular.eot` & `flasgger-0.9.7b2/flasgger/ui2/static/fonts/droid-sans-v6-latin-regular.eot`

 * *Files identical despite different names*

### Comparing `flasgger-0.9.7.1/flasgger/ui2/static/fonts/droid-sans-v6-latin-regular.svg` & `flasgger-0.9.7b2/flasgger/ui2/static/fonts/droid-sans-v6-latin-regular.svg`

 * *Files identical despite different names*

### Comparing `flasgger-0.9.7.1/flasgger/ui2/static/fonts/droid-sans-v6-latin-regular.ttf` & `flasgger-0.9.7b2/flasgger/ui2/static/fonts/droid-sans-v6-latin-regular.ttf`

 * *Files identical despite different names*

### Comparing `flasgger-0.9.7.1/flasgger/ui2/static/fonts/droid-sans-v6-latin-regular.woff` & `flasgger-0.9.7b2/flasgger/ui2/static/fonts/droid-sans-v6-latin-regular.woff`

 * *Files identical despite different names*

### Comparing `flasgger-0.9.7.1/flasgger/ui2/static/fonts/droid-sans-v6-latin-regular.woff2` & `flasgger-0.9.7b2/flasgger/ui2/static/fonts/droid-sans-v6-latin-regular.woff2`

 * *Files identical despite different names*

### Comparing `flasgger-0.9.7.1/flasgger/ui2/static/images/explorer_icons.png` & `flasgger-0.9.7b2/flasgger/ui2/static/images/explorer_icons.png`

 * *Files identical despite different names*

### Comparing `flasgger-0.9.7.1/flasgger/ui2/static/images/favicon-32x32.png` & `flasgger-0.9.7b2/flasgger/ui2/static/images/favicon-32x32.png`

 * *Files identical despite different names*

### Comparing `flasgger-0.9.7.1/flasgger/ui2/static/images/favicon.ico` & `flasgger-0.9.7b2/flasgger/ui2/static/images/favicon.ico`

 * *Files identical despite different names*

### Comparing `flasgger-0.9.7.1/flasgger/ui2/static/images/pet_store_api.png` & `flasgger-0.9.7b2/flasgger/ui2/static/images/pet_store_api.png`

 * *Files identical despite different names*

### Comparing `flasgger-0.9.7.1/flasgger/ui2/static/images/throbber.gif` & `flasgger-0.9.7b2/flasgger/ui2/static/images/throbber.gif`

 * *Files identical despite different names*

### Comparing `flasgger-0.9.7.1/flasgger/ui2/static/images/wordnik_api.png` & `flasgger-0.9.7b2/flasgger/ui2/static/images/wordnik_api.png`

 * *Files identical despite different names*

### Comparing `flasgger-0.9.7.1/flasgger/ui2/static/index.html` & `flasgger-0.9.7b2/flasgger/ui2/static/index.html`

 * *Files identical despite different names*

### Comparing `flasgger-0.9.7.1/flasgger/ui2/static/lang/ca.js` & `flasgger-0.9.7b2/flasgger/ui2/static/lang/ca.js`

 * *Files identical despite different names*

### Comparing `flasgger-0.9.7.1/flasgger/ui2/static/lang/el.js` & `flasgger-0.9.7b2/flasgger/ui2/static/lang/el.js`

 * *Files identical despite different names*

### Comparing `flasgger-0.9.7.1/flasgger/ui2/static/lang/en.js` & `flasgger-0.9.7b2/flasgger/ui2/static/lang/en.js`

 * *Files identical despite different names*

### Comparing `flasgger-0.9.7.1/flasgger/ui2/static/lang/es.js` & `flasgger-0.9.7b2/flasgger/ui2/static/lang/es.js`

 * *Files identical despite different names*

### Comparing `flasgger-0.9.7.1/flasgger/ui2/static/lang/fr.js` & `flasgger-0.9.7b2/flasgger/ui2/static/lang/fr.js`

 * *Files identical despite different names*

### Comparing `flasgger-0.9.7.1/flasgger/ui2/static/lang/geo.js` & `flasgger-0.9.7b2/flasgger/ui2/static/lang/geo.js`

 * *Files identical despite different names*

### Comparing `flasgger-0.9.7.1/flasgger/ui2/static/lang/it.js` & `flasgger-0.9.7b2/flasgger/ui2/static/lang/it.js`

 * *Files identical despite different names*

### Comparing `flasgger-0.9.7.1/flasgger/ui2/static/lang/ja.js` & `flasgger-0.9.7b2/flasgger/ui2/static/lang/ja.js`

 * *Files identical despite different names*

### Comparing `flasgger-0.9.7.1/flasgger/ui2/static/lang/ko-kr.js` & `flasgger-0.9.7b2/flasgger/ui2/static/lang/ko-kr.js`

 * *Files identical despite different names*

### Comparing `flasgger-0.9.7.1/flasgger/ui2/static/lang/pl.js` & `flasgger-0.9.7b2/flasgger/ui2/static/lang/pl.js`

 * *Files identical despite different names*

### Comparing `flasgger-0.9.7.1/flasgger/ui2/static/lang/pt.js` & `flasgger-0.9.7b2/flasgger/ui2/static/lang/pt.js`

 * *Files identical despite different names*

### Comparing `flasgger-0.9.7.1/flasgger/ui2/static/lang/ru.js` & `flasgger-0.9.7b2/flasgger/ui2/static/lang/ru.js`

 * *Files identical despite different names*

### Comparing `flasgger-0.9.7.1/flasgger/ui2/static/lang/tr.js` & `flasgger-0.9.7b2/flasgger/ui2/static/lang/tr.js`

 * *Files identical despite different names*

### Comparing `flasgger-0.9.7.1/flasgger/ui2/static/lang/translator.js` & `flasgger-0.9.7b2/flasgger/ui2/static/lang/translator.js`

 * *Files identical despite different names*

### Comparing `flasgger-0.9.7.1/flasgger/ui2/static/lang/zh-cn.js` & `flasgger-0.9.7b2/flasgger/ui2/static/lang/zh-cn.js`

 * *Files identical despite different names*

### Comparing `flasgger-0.9.7.1/flasgger/ui2/static/lib/backbone-min.js` & `flasgger-0.9.7b2/flasgger/ui2/static/lib/backbone-min.js`

 * *Files identical despite different names*

### Comparing `flasgger-0.9.7.1/flasgger/ui2/static/lib/es5-shim.js` & `flasgger-0.9.7b2/flasgger/ui2/static/lib/es5-shim.js`

 * *Files identical despite different names*

### Comparing `flasgger-0.9.7.1/flasgger/ui2/static/lib/handlebars-4.0.5.js` & `flasgger-0.9.7b2/flasgger/ui2/static/lib/handlebars-4.0.5.js`

 * *Files identical despite different names*

### Comparing `flasgger-0.9.7.1/flasgger/ui2/static/lib/highlight.9.1.0.pack.js` & `flasgger-0.9.7b2/flasgger/ui2/static/lib/highlight.9.1.0.pack.js`

 * *Files identical despite different names*

### Comparing `flasgger-0.9.7.1/flasgger/ui2/static/lib/jquery-1.8.0.min.js` & `flasgger-0.9.7b2/flasgger/ui2/static/lib/jquery-1.8.0.min.js`

 * *Files identical despite different names*

### Comparing `flasgger-0.9.7.1/flasgger/ui2/static/lib/jquery.ba-bbq.min.js` & `flasgger-0.9.7b2/flasgger/ui2/static/lib/jquery.ba-bbq.min.js`

 * *Files identical despite different names*

### Comparing `flasgger-0.9.7.1/flasgger/ui2/static/lib/jquery.wiggle.min.js` & `flasgger-0.9.7b2/flasgger/ui2/static/lib/jquery.wiggle.min.js`

 * *Files identical despite different names*

### Comparing `flasgger-0.9.7.1/flasgger/ui2/static/lib/js-yaml.min.js` & `flasgger-0.9.7b2/flasgger/ui2/static/lib/js-yaml.min.js`

 * *Files identical despite different names*

### Comparing `flasgger-0.9.7.1/flasgger/ui2/static/lib/jsoneditor.min.js` & `flasgger-0.9.7b2/flasgger/ui2/static/lib/jsoneditor.min.js`

 * *Files identical despite different names*

### Comparing `flasgger-0.9.7.1/flasgger/ui2/static/lib/lodash.min.js` & `flasgger-0.9.7b2/flasgger/ui2/static/lib/lodash.min.js`

 * *Files identical despite different names*

### Comparing `flasgger-0.9.7.1/flasgger/ui2/static/lib/marked.js` & `flasgger-0.9.7b2/flasgger/ui2/static/lib/marked.js`

 * *Files identical despite different names*

### Comparing `flasgger-0.9.7.1/flasgger/ui2/static/lib/sanitize-html.min.js` & `flasgger-0.9.7b2/flasgger/ui2/static/lib/sanitize-html.min.js`

 * *Files identical despite different names*

### Comparing `flasgger-0.9.7.1/flasgger/ui2/static/lib/swagger-oauth.js` & `flasgger-0.9.7b2/flasgger/ui2/static/lib/swagger-oauth.js`

 * *Files identical despite different names*

### Comparing `flasgger-0.9.7.1/flasgger/ui2/static/swagger-ui.js` & `flasgger-0.9.7b2/flasgger/ui2/static/swagger-ui.js`

 * *Files identical despite different names*

### Comparing `flasgger-0.9.7.1/flasgger/ui2/static/swagger-ui.min.js` & `flasgger-0.9.7b2/flasgger/ui2/static/swagger-ui.min.js`

 * *Files identical despite different names*

### Comparing `flasgger-0.9.7.1/flasgger/ui2/templates/flasgger/index.html` & `flasgger-0.9.7b2/flasgger/ui2/templates/flasgger/index.html`

 * *Files identical despite different names*

### Comparing `flasgger-0.9.7.1/flasgger/ui2/templates/flasgger/index_old.html` & `flasgger-0.9.7b2/flasgger/ui2/templates/flasgger/index_old.html`

 * *Files identical despite different names*

### Comparing `flasgger-0.9.7.1/flasgger/ui3/static/favicon-16x16.png` & `flasgger-0.9.7b2/flasgger/ui3/static/favicon-16x16.png`

 * *Files identical despite different names*

### Comparing `flasgger-0.9.7.1/flasgger/ui3/static/favicon-32x32.png` & `flasgger-0.9.7b2/flasgger/ui3/static/favicon-32x32.png`

 * *Files identical despite different names*

### Comparing `flasgger-0.9.7.1/flasgger/ui3/static/lib/jquery.min.js` & `flasgger-0.9.7b2/flasgger/ui3/static/lib/jquery.min.js`

 * *Files identical despite different names*

### Comparing `flasgger-0.9.7.1/flasgger/ui3/static/lib/jquery.min.map` & `flasgger-0.9.7b2/flasgger/ui3/static/lib/jquery.min.map`

 * *Files identical despite different names*

### Comparing `flasgger-0.9.7.1/flasgger/ui3/static/swagger-ui-bundle.js` & `flasgger-0.9.7b2/flasgger/ui3/static/swagger-ui-bundle.js`

 * *Files identical despite different names*

### Comparing `flasgger-0.9.7.1/flasgger/ui3/static/swagger-ui-bundle.js.map` & `flasgger-0.9.7b2/flasgger/ui3/static/swagger-ui-bundle.js.map`

 * *Files identical despite different names*

### Comparing `flasgger-0.9.7.1/flasgger/ui3/static/swagger-ui-standalone-preset.js` & `flasgger-0.9.7b2/flasgger/ui3/static/swagger-ui-standalone-preset.js`

 * *Files identical despite different names*

### Comparing `flasgger-0.9.7.1/flasgger/ui3/static/swagger-ui-standalone-preset.js.map` & `flasgger-0.9.7b2/flasgger/ui3/static/swagger-ui-standalone-preset.js.map`

 * *Files identical despite different names*

### Comparing `flasgger-0.9.7.1/flasgger/ui3/static/swagger-ui.css` & `flasgger-0.9.7b2/flasgger/ui3/static/swagger-ui.css`

 * *Files identical despite different names*

### Comparing `flasgger-0.9.7.1/flasgger/ui3/static/swagger-ui.css.map` & `flasgger-0.9.7b2/flasgger/ui3/static/swagger-ui.css.map`

 * *Files identical despite different names*

### Comparing `flasgger-0.9.7.1/flasgger/ui3/static/swagger-ui.js` & `flasgger-0.9.7b2/flasgger/ui3/static/swagger-ui.js`

 * *Files identical despite different names*

### Comparing `flasgger-0.9.7.1/flasgger/ui3/static/swagger-ui.js.map` & `flasgger-0.9.7b2/flasgger/ui3/static/swagger-ui.js.map`

 * *Files identical despite different names*

### Comparing `flasgger-0.9.7.1/flasgger/ui3/templates/flasgger/head.html` & `flasgger-0.9.7b2/flasgger/ui3/templates/flasgger/head.html`

 * *Files identical despite different names*

### Comparing `flasgger-0.9.7.1/flasgger/ui3/templates/flasgger/index.html` & `flasgger-0.9.7b2/flasgger/ui3/templates/flasgger/index.html`

 * *Files identical despite different names*

### Comparing `flasgger-0.9.7.1/flasgger/ui3/templates/flasgger/oauth2-redirect.html` & `flasgger-0.9.7b2/flasgger/ui3/templates/flasgger/oauth2-redirect.html`

 * *Files identical despite different names*

### Comparing `flasgger-0.9.7.1/flasgger/ui3/templates/flasgger/swagger.html` & `flasgger-0.9.7b2/flasgger/ui3/templates/flasgger/swagger.html`

 * *Files identical despite different names*

### Comparing `flasgger-0.9.7.1/flasgger/utils.py` & `flasgger-0.9.7b2/flasgger/utils.py`

 * *Files identical despite different names*

### Comparing `flasgger-0.9.7.1/flasgger.egg-info/PKG-INFO` & `flasgger-0.9.7b2/flasgger.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flasgger
-Version: 0.9.7.1
+Version: 0.9.7b2
 Summary: Extract swagger specs from your flask project
 Home-page: https://github.com/flasgger/flasgger/
 Author: Bruno Rocha, Zixuan Rao, Flasgger team
 Author-email: flasgger@flasgger.org
 License: MIT
 Platform: any
 Classifier: Intended Audience :: Developers
@@ -94,30 +94,24 @@
 > under your virtualenv do:
 
 Ensure you have latest setuptools
 ```
 pip install -U setuptools
 ```
 
-then install beta version (recommended)
+then
 
 ```
-pip install flasgger==0.9.7b2
-```
-
-or (latest stable for legacy apps)
-
-```
-pip install flasgger==0.9.5
+pip install flasgger
 ```
 
 or (dev version)
 
 ```
-pip install https://github.com/flasgger/flasgger/tarball/master
+pip install https://github.com/rochacbruno/flasgger/tarball/master
 ```
 
 > NOTE: If you want to use **Marshmallow Schemas** you also need to run `pip install marshmallow apispec`
 
 ## How to run tests
 
 (You may see the command in [.travis.yml](./.travis.yml) for `before_install` part)
```

### Comparing `flasgger-0.9.7.1/flasgger.egg-info/SOURCES.txt` & `flasgger-0.9.7b2/flasgger.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `flasgger-0.9.7.1/setup.py` & `flasgger-0.9.7b2/setup.py`

 * *Files identical despite different names*

### Comparing `flasgger-0.9.7.1/tests/__pycache__/conftest.cpython-311-pytest-7.3.1.pyc` & `flasgger-0.9.7b2/tests/__pycache__/conftest.cpython-311-pytest-7.3.1.pyc`

 * *Files identical despite different names*

### Comparing `flasgger-0.9.7.1/tests/__pycache__/conftest.cpython-38-pytest-6.1.1.pyc` & `flasgger-0.9.7b2/tests/__pycache__/conftest.cpython-38-pytest-6.1.1.pyc`

 * *Files identical despite different names*

### Comparing `flasgger-0.9.7.1/tests/__pycache__/conftest.cpython-39-pytest-7.3.1.pyc` & `flasgger-0.9.7b2/tests/__pycache__/conftest.cpython-39-pytest-7.3.1.pyc`

 * *Files identical despite different names*

### Comparing `flasgger-0.9.7.1/tests/__pycache__/test_apispecs.cpython-311-pytest-7.3.1.pyc` & `flasgger-0.9.7b2/tests/__pycache__/test_apispecs.cpython-311-pytest-7.3.1.pyc`

 * *Files identical despite different names*

### Comparing `flasgger-0.9.7.1/tests/__pycache__/test_apispecs.cpython-39-pytest-7.3.1.pyc` & `flasgger-0.9.7b2/tests/__pycache__/test_apispecs.cpython-39-pytest-7.3.1.pyc`

 * *Files identical despite different names*

### Comparing `flasgger-0.9.7.1/tests/__pycache__/test_base.cpython-311-pytest-7.3.1.pyc` & `flasgger-0.9.7b2/tests/__pycache__/test_base.cpython-311-pytest-7.3.1.pyc`

 * *Files identical despite different names*

### Comparing `flasgger-0.9.7.1/tests/__pycache__/test_base.cpython-39-pytest-7.3.1.pyc` & `flasgger-0.9.7b2/tests/__pycache__/test_base.cpython-39-pytest-7.3.1.pyc`

 * *Files identical despite different names*

### Comparing `flasgger-0.9.7.1/tests/__pycache__/test_commands.cpython-311-pytest-7.3.1.pyc` & `flasgger-0.9.7b2/tests/__pycache__/test_commands.cpython-311-pytest-7.3.1.pyc`

 * *Files identical despite different names*

### Comparing `flasgger-0.9.7.1/tests/__pycache__/test_commands.cpython-39-pytest-7.3.1.pyc` & `flasgger-0.9.7b2/tests/__pycache__/test_commands.cpython-39-pytest-7.3.1.pyc`

 * *Files identical despite different names*

### Comparing `flasgger-0.9.7.1/tests/__pycache__/test_examples.cpython-311-pytest-7.3.1.pyc` & `flasgger-0.9.7b2/tests/__pycache__/test_examples.cpython-311-pytest-7.3.1.pyc`

 * *Files identical despite different names*

### Comparing `flasgger-0.9.7.1/tests/__pycache__/test_examples.cpython-39-pytest-7.3.1.pyc` & `flasgger-0.9.7b2/tests/__pycache__/test_examples.cpython-39-pytest-7.3.1.pyc`

 * *Files identical despite different names*

### Comparing `flasgger-0.9.7.1/tests/__pycache__/test_utils.cpython-311-pytest-7.3.1.pyc` & `flasgger-0.9.7b2/tests/__pycache__/test_utils.cpython-311-pytest-7.3.1.pyc`

 * *Files identical despite different names*

### Comparing `flasgger-0.9.7.1/tests/__pycache__/test_utils.cpython-39-pytest-7.3.1.pyc` & `flasgger-0.9.7b2/tests/__pycache__/test_utils.cpython-39-pytest-7.3.1.pyc`

 * *Files identical despite different names*

### Comparing `flasgger-0.9.7.1/tests/conftest.py` & `flasgger-0.9.7b2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `flasgger-0.9.7.1/tests/test_apispecs.py` & `flasgger-0.9.7b2/tests/test_apispecs.py`

 * *Files identical despite different names*

### Comparing `flasgger-0.9.7.1/tests/test_base.py` & `flasgger-0.9.7b2/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `flasgger-0.9.7.1/tests/test_commands.py` & `flasgger-0.9.7b2/tests/test_commands.py`

 * *Files identical despite different names*

### Comparing `flasgger-0.9.7.1/tests/test_examples.py` & `flasgger-0.9.7b2/tests/test_examples.py`

 * *Files identical despite different names*

