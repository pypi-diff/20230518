# Comparing `tmp/drf-jwt-knox-0.1.2.tar.gz` & `tmp/drf_jwt_knox-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "drf-jwt-knox-0.1.2.tar", max compression
+gzip compressed data, was "drf_jwt_knox-0.2.0.tar", max compression
```

## Comparing `drf-jwt-knox-0.1.2.tar` & `drf_jwt_knox-0.2.0.tar`

### file list

```diff
@@ -1,13 +1,12 @@
--rw-r--r--   0        0        0    11357 2021-12-26 03:12:39.804031 drf-jwt-knox-0.1.2/LICENSE
--rw-r--r--   0        0        0     2708 2021-12-26 03:12:39.804031 drf-jwt-knox-0.1.2/README.md
--rw-r--r--   0        0        0        0 2021-12-26 03:12:39.804031 drf-jwt-knox-0.1.2/jwt_knox/__init__.py
--rw-r--r--   0        0        0       90 2021-12-26 03:12:39.804031 drf-jwt-knox-0.1.2/jwt_knox/apps.py
--rw-r--r--   0        0        0     4479 2021-12-26 03:12:39.804031 drf-jwt-knox-0.1.2/jwt_knox/auth.py
--rw-r--r--   0        0        0        0 2021-12-26 03:12:39.804031 drf-jwt-knox-0.1.2/jwt_knox/migrations/__init__.py
--rw-r--r--   0        0        0     1235 2021-12-26 03:12:39.804031 drf-jwt-knox-0.1.2/jwt_knox/settings.py
--rw-r--r--   0        0        0      243 2021-12-26 03:12:39.804031 drf-jwt-knox-0.1.2/jwt_knox/urls.py
--rw-r--r--   0        0        0     2385 2021-12-26 03:12:39.804031 drf-jwt-knox-0.1.2/jwt_knox/utils.py
--rw-r--r--   0        0        0     4754 2021-12-26 03:12:39.804031 drf-jwt-knox-0.1.2/jwt_knox/viewsets.py
--rw-r--r--   0        0        0     1532 2021-12-26 03:12:50.132075 drf-jwt-knox-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     3317 2021-12-26 03:12:50.524492 drf-jwt-knox-0.1.2/setup.py
--rw-r--r--   0        0        0     3494 2021-12-26 03:12:50.524874 drf-jwt-knox-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-05-18 01:51:35.240337 drf_jwt_knox-0.2.0/LICENSE
+-rw-r--r--   0        0        0     2782 2023-05-18 01:51:35.240337 drf_jwt_knox-0.2.0/README.md
+-rw-r--r--   0        0        0        0 2023-05-18 01:51:35.240337 drf_jwt_knox-0.2.0/jwt_knox/__init__.py
+-rw-r--r--   0        0        0       90 2023-05-18 01:51:35.240337 drf_jwt_knox-0.2.0/jwt_knox/apps.py
+-rw-r--r--   0        0        0     4462 2023-05-18 01:51:35.240337 drf_jwt_knox-0.2.0/jwt_knox/auth.py
+-rw-r--r--   0        0        0        0 2023-05-18 01:51:35.240337 drf_jwt_knox-0.2.0/jwt_knox/migrations/__init__.py
+-rw-r--r--   0        0        0     1235 2023-05-18 01:51:35.240337 drf_jwt_knox-0.2.0/jwt_knox/settings.py
+-rw-r--r--   0        0        0      243 2023-05-18 01:51:35.240337 drf_jwt_knox-0.2.0/jwt_knox/urls.py
+-rw-r--r--   0        0        0     2385 2023-05-18 01:51:35.240337 drf_jwt_knox-0.2.0/jwt_knox/utils.py
+-rw-r--r--   0        0        0     4754 2023-05-18 01:51:35.240337 drf_jwt_knox-0.2.0/jwt_knox/viewsets.py
+-rw-r--r--   0        0        0     1691 2023-05-18 01:51:51.074598 drf_jwt_knox-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     3435 1970-01-01 00:00:00.000000 drf_jwt_knox-0.2.0/PKG-INFO
```

### Comparing `drf-jwt-knox-0.1.2/LICENSE` & `drf_jwt_knox-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `drf-jwt-knox-0.1.2/README.md` & `drf_jwt_knox-0.2.0/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 DRF JWT + Knox
 ==============
 
-[![Build Status](https://travis-ci.org/ssaavedra/drf-jwt-knox.svg?branch=master)](https://travis-ci.org/ssaavedra/drf-jwt-knox)
+[![Build status](https://github.com/ssaavedra/drf-jwt-knox/actions/workflows/python-package.yml/badge.svg?event=release)](https://github.com/ssaavedra/drf-jwt-knox/actions/workflows/python-package.yml)
 [![codecov](https://codecov.io/gh/ssaavedra/drf-jwt-knox/branch/master/graph/badge.svg)](https://codecov.io/gh/ssaavedra/drf-jwt-knox)
 [![PyPI version](https://img.shields.io/pypi/v/drf-jwt-knox.svg)](https://pypi.python.org/pypi/drf-jwt-knox)
 [![Requirements Status](https://requires.io/github/ssaavedra/drf-jwt-knox/requirements.svg?branch=master)](https://requires.io/github/ssaavedra/drf-jwt-knox/requirements/?branch=master)
 [![Maintainability Rating](https://sonarcloud.io/api/project_badges/measure?project=ssaavedra_drf-jwt-knox&metric=sqale_rating)](https://sonarcloud.io/dashboard?id=ssaavedra_drf-jwt-knox)
 
 This package provides an authentication mechanism for Django REST
 Framework based on [JSON Web Tokens][JWT] in the browser backed up by
```

### Comparing `drf-jwt-knox-0.1.2/jwt_knox/auth.py` & `drf_jwt_knox-0.2.0/jwt_knox/auth.py`

 * *Files 1% similar despite different names*

```diff
@@ -60,15 +60,15 @@
         return (user, self.ensure_valid_auth_token(user, token))
 
     def ensure_valid_auth_token(self, user, token: AuthToken):
         for auth_token in AuthToken.objects.filter(user=user):
             if auth_token.expiry is not None and auth_token.expiry < timezone.now():
                 auth_token.delete()
                 continue
-            digest = hash_token(token, auth_token.salt)
+            digest = hash_token(token)
             if digest == auth_token.digest:
                 return auth_token
 
         msg = _('Invalid token.')
         raise exceptions.AuthenticationFailed(msg)
```

### Comparing `drf-jwt-knox-0.1.2/jwt_knox/settings.py` & `drf_jwt_knox-0.2.0/jwt_knox/settings.py`

 * *Files identical despite different names*

### Comparing `drf-jwt-knox-0.1.2/jwt_knox/utils.py` & `drf_jwt_knox-0.2.0/jwt_knox/utils.py`

 * *Files identical despite different names*

### Comparing `drf-jwt-knox-0.1.2/jwt_knox/viewsets.py` & `drf_jwt_knox-0.2.0/jwt_knox/viewsets.py`

 * *Files identical despite different names*

### Comparing `drf-jwt-knox-0.1.2/PKG-INFO` & `drf_jwt_knox-0.2.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,31 +1,29 @@
 Metadata-Version: 2.1
 Name: drf-jwt-knox
-Version: 0.1.2
+Version: 0.2.0
 Summary: Knox-fortified JSON Web Tokens for Django REST Framework
 License: Apache2
 Author: Santiago Saavedra
 Author-email: ssaavedra@gpul.org
+Requires-Python: >=3.9,<4.0
 Classifier: License :: Other/Proprietary License
-Classifier: Programming Language :: Python :: 2
-Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.4
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: PyJWT (>=2.7.0,<3.0.0)
+Requires-Dist: django-rest-knox (>=4.2.0,<5.0.0)
+Requires-Dist: djangorestframework (>=3.14,<4.0)
 Description-Content-Type: text/markdown
 
 DRF JWT + Knox
 ==============
 
-[![Build Status](https://travis-ci.org/ssaavedra/drf-jwt-knox.svg?branch=master)](https://travis-ci.org/ssaavedra/drf-jwt-knox)
+[![Build status](https://github.com/ssaavedra/drf-jwt-knox/actions/workflows/python-package.yml/badge.svg?event=release)](https://github.com/ssaavedra/drf-jwt-knox/actions/workflows/python-package.yml)
 [![codecov](https://codecov.io/gh/ssaavedra/drf-jwt-knox/branch/master/graph/badge.svg)](https://codecov.io/gh/ssaavedra/drf-jwt-knox)
 [![PyPI version](https://img.shields.io/pypi/v/drf-jwt-knox.svg)](https://pypi.python.org/pypi/drf-jwt-knox)
 [![Requirements Status](https://requires.io/github/ssaavedra/drf-jwt-knox/requirements.svg?branch=master)](https://requires.io/github/ssaavedra/drf-jwt-knox/requirements/?branch=master)
 [![Maintainability Rating](https://sonarcloud.io/api/project_badges/measure?project=ssaavedra_drf-jwt-knox&metric=sqale_rating)](https://sonarcloud.io/dashboard?id=ssaavedra_drf-jwt-knox)
 
 This package provides an authentication mechanism for Django REST
 Framework based on [JSON Web Tokens][JWT] in the browser backed up by
```

