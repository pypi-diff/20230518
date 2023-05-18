# Comparing `tmp/justpass-me-django-3.0.2.tar.gz` & `tmp/justpass-me-django-3.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "justpass-me-django-3.0.2.tar", last modified: Tue May 16 17:36:15 2023, max compression
+gzip compressed data, was "justpass-me-django-3.0.3.tar", last modified: Thu May 18 11:54:40 2023, max compression
```

## Comparing `justpass-me-django-3.0.2.tar` & `justpass-me-django-3.0.3.tar`

### file list

```diff
@@ -1,23 +1,22 @@
-drwxrwxr-x   0 mohamed   (1000) mohamed   (1000)        0 2023-05-16 17:36:15.471368 justpass-me-django-3.0.2/
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)     1067 2023-05-15 16:53:18.000000 justpass-me-django-3.0.2/LICENSE
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)     5099 2023-05-16 17:36:15.471368 justpass-me-django-3.0.2/PKG-INFO
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)     3838 2023-05-15 18:30:27.000000 justpass-me-django-3.0.2/README.md
-drwxrwxr-x   0 mohamed   (1000) mohamed   (1000)        0 2023-05-16 17:36:15.471368 justpass-me-django-3.0.2/justpass_me_django.egg-info/
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)     5099 2023-05-16 17:36:15.000000 justpass-me-django-3.0.2/justpass_me_django.egg-info/PKG-INFO
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)      456 2023-05-16 17:36:15.000000 justpass-me-django-3.0.2/justpass_me_django.egg-info/SOURCES.txt
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)        1 2023-05-16 17:36:15.000000 justpass-me-django-3.0.2/justpass_me_django.egg-info/dependency_links.txt
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)        1 2023-05-15 16:54:06.000000 justpass-me-django-3.0.2/justpass_me_django.egg-info/not-zip-safe
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)       39 2023-05-16 17:36:15.000000 justpass-me-django-3.0.2/justpass_me_django.egg-info/requires.txt
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)       11 2023-05-16 17:36:15.000000 justpass-me-django-3.0.2/justpass_me_django.egg-info/top_level.txt
-drwxrwxr-x   0 mohamed   (1000) mohamed   (1000)        0 2023-05-16 17:36:15.471368 justpass-me-django-3.0.2/justpassme/
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)     6758 2023-05-15 18:16:10.000000 justpass-me-django-3.0.2/justpassme/OIDC_CLIENT.py
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)        0 2023-05-15 16:53:18.000000 justpass-me-django-3.0.2/justpassme/__init__.py
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)       63 2023-05-15 16:53:18.000000 justpass-me-django-3.0.2/justpassme/admin.py
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)      152 2023-05-15 16:53:18.000000 justpass-me-django-3.0.2/justpassme/apps.py
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)     1096 2023-05-15 17:40:25.000000 justpass-me-django-3.0.2/justpassme/helpers.py
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)      672 2023-05-15 17:54:17.000000 justpass-me-django-3.0.2/justpassme/urls.py
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)      168 2023-05-15 16:53:18.000000 justpass-me-django-3.0.2/justpassme/utils.py
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)      968 2023-05-15 17:42:22.000000 justpass-me-django-3.0.2/justpassme/views.py
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)     1659 2023-05-16 17:36:11.000000 justpass-me-django-3.0.2/setup-3.py
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)       38 2023-05-16 17:36:15.471368 justpass-me-django-3.0.2/setup.cfg
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)     1659 2023-05-16 17:36:11.000000 justpass-me-django-3.0.2/setup.py
+drwxrwxr-x   0 mohamed   (1000) mohamed   (1000)        0 2023-05-18 11:54:39.999131 justpass-me-django-3.0.3/
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)     1067 2023-05-15 15:42:36.000000 justpass-me-django-3.0.3/LICENSE
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)     4891 2023-05-18 11:54:39.999131 justpass-me-django-3.0.3/PKG-INFO
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)     3649 2023-05-18 11:54:07.000000 justpass-me-django-3.0.3/README.md
+drwxrwxr-x   0 mohamed   (1000) mohamed   (1000)        0 2023-05-18 11:54:39.999131 justpass-me-django-3.0.3/justpass_me_django.egg-info/
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)     4891 2023-05-18 11:54:39.000000 justpass-me-django-3.0.3/justpass_me_django.egg-info/PKG-INFO
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)      445 2023-05-18 11:54:39.000000 justpass-me-django-3.0.3/justpass_me_django.egg-info/SOURCES.txt
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)        1 2023-05-18 11:54:39.000000 justpass-me-django-3.0.3/justpass_me_django.egg-info/dependency_links.txt
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)        1 2023-05-15 15:48:48.000000 justpass-me-django-3.0.3/justpass_me_django.egg-info/not-zip-safe
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)       58 2023-05-18 11:54:39.000000 justpass-me-django-3.0.3/justpass_me_django.egg-info/requires.txt
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)       11 2023-05-18 11:54:39.000000 justpass-me-django-3.0.3/justpass_me_django.egg-info/top_level.txt
+drwxrwxr-x   0 mohamed   (1000) mohamed   (1000)        0 2023-05-18 11:54:39.999131 justpass-me-django-3.0.3/justpassme/
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)     6758 2023-05-18 11:49:19.000000 justpass-me-django-3.0.3/justpassme/OIDC_CLIENT.py
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)        0 2023-05-15 15:07:58.000000 justpass-me-django-3.0.3/justpassme/__init__.py
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)       63 2023-05-15 15:07:58.000000 justpass-me-django-3.0.3/justpassme/admin.py
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)      152 2023-05-15 15:13:26.000000 justpass-me-django-3.0.3/justpassme/apps.py
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)     1096 2023-05-18 11:49:19.000000 justpass-me-django-3.0.3/justpassme/helpers.py
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)      672 2023-05-18 11:49:19.000000 justpass-me-django-3.0.3/justpassme/urls.py
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)      168 2023-05-15 15:07:58.000000 justpass-me-django-3.0.3/justpassme/utils.py
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)      968 2023-05-18 11:49:19.000000 justpass-me-django-3.0.3/justpassme/views.py
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)       38 2023-05-18 11:54:40.003131 justpass-me-django-3.0.3/setup.cfg
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)     1688 2023-05-18 11:50:58.000000 justpass-me-django-3.0.3/setup.py
```

### Comparing `justpass-me-django-3.0.2/LICENSE` & `justpass-me-django-3.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `justpass-me-django-3.0.2/PKG-INFO` & `justpass-me-django-3.0.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: justpass-me-django
-Version: 3.0.2
+Version: 3.0.3
 Summary: Django Integration with JustPass.me
 Home-page: https://github.com/justpass-me/justpass-me-django
+Download-URL: https://github.com/justpass-me/justpass-me-django
 Author: JustPassMe
 Author-email: sameh@justpass.me
 License: MIT
-Download-URL: https://github.com/justpass-me/justpass-me-django
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.0
 Classifier: Framework :: Django :: 3.1
 Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.0
@@ -75,29 +74,29 @@
    OIDC_RP_SCOPES= "openid"
    OIDC_RP_SIGN_ALGO = 'HS256'
    OIDC_STORE_ID_TOKEN = True
    OIDC_OP_JWKS_ENDPOINT=OIDC_OP_URL  +"jwks"
    OIDC_OP_AUTHORIZATION_ENDPOINT=OIDC_OP_URL + "authorize/"
    OIDC_OP_TOKEN_ENDPOINT = OIDC_OP_URL +"token/"
    OIDC_OP_USER_ENDPOINT = OIDC_OP_URL + "userinfo/"
-   OIDC_CALLBACK_CLASS= "justpass.OIDC_CLIENT.OIDCAuthn"
-   OIDC_AUTHENTICATE_CLASS = "justpass.OIDC_CLIENT.OIDC_AUTHENTICATE"
+   OIDC_CALLBACK_CLASS= "justpassme.OIDC_CLIENT.OIDCAuthn"
+   OIDC_AUTHENTICATE_CLASS = "justpassme.OIDC_CLIENT.OIDC_AUTHENTICATE"
    LOGIN_REDIRECT_URL_FAILURE="/justpass/failure/"
    LOGIN_REDIRECT_URL = "/justpass/success/"
 
    # If your application uses SSL.
    USE_X_FORWARDED_HOST = True
    SECURE_PROXY_SSL_HEADER = ('HTTP_X_FORWARDED_PROTO', 'https')
 
 
    # Provide the following functions that will be called when event is triggered, check example functions below
-   REGISTRATION_SUCCESS = "Shop.justpass.reg_success"
-   REGISTRATION_FAILURE = "Shop.justpass.reg_failure"
-   AUTHENTICATION_SUCCESS = "Shop.justpass.auth_success"
-   AUTHENTICATION_FAILURE = "Shop.justpass.auth_failure"
+   REGISTRATION_SUCCESS = "Your_App.justpass.reg_success"
+   REGISTRATION_FAILURE = "Your_App.justpass.reg_failure"
+   AUTHENTICATION_SUCCESS = "Your_App.justpass.auth_success"
+   AUTHENTICATION_FAILURE = "Your_App.justpass.auth_failure"
 
    ```
 3. Add `justpass` to your urls
    ```python 
    urls_patterns= [
    '...',
    path(r'justpass/', include('justpassme.urls')),
@@ -110,34 +109,25 @@
 Break your login function, Usually your login function will check for username and password, log the user in if the username and password are correct and create the user session, to support justpass.me, this has to change
    
    * authenticate the user
    * if username and password are correct , check if the user has mfa or not
        * if user has mfa then redirect to justpass.me
        * if user doesn't have mfa then call your function to create the user session
 
-3. To start registration, go `justpass:reg``
+3. To start registration, redirct to  `justpass:start_reg`
 
-   ```python
-   def start_reg(request):
-       from justpassme.helpers import start_reg
-       return start_reg(request)
-   ```
 
-4. Write a function to start login and add it to your `urls.py`
+4. To start login, redirect to `justpass:start_login`
 
-   **Note:** The function expects the user username to be in `request.session["base_username"]`
+   **Note:** For 2nd factor, The function expects the user's username to be in `request.session["base_username"]`
 
-   ```python
-   def start_login(request):
-       from justpassme.helpers import start_oidc_sign
-       return start_oidc_sign(request)
-   ```
 
-5. Write 4 functions that handle the success and failure of registration and login. 
-You can use the four functions below as a reference.
+5. Write 4 functions that handle the success and failure of registration and login, refer to them in the `settings.py` 
+
+   You can use the four functions below as a reference.
 
    ```python
    def auth_success(request):
       return redirect('home')
          
    def auth_failure(request):
      return render(request, 'login.html', {"failed": True})
@@ -148,8 +138,7 @@
       request.session["reg"] = True
       return redirect('home')
       
    def reg_failure(request):
       request.session["reg"] = False
       return redirect('home')
    ```
-
```

### Comparing `justpass-me-django-3.0.2/README.md` & `justpass-me-django-3.0.3/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -42,29 +42,29 @@
    OIDC_RP_SCOPES= "openid"
    OIDC_RP_SIGN_ALGO = 'HS256'
    OIDC_STORE_ID_TOKEN = True
    OIDC_OP_JWKS_ENDPOINT=OIDC_OP_URL  +"jwks"
    OIDC_OP_AUTHORIZATION_ENDPOINT=OIDC_OP_URL + "authorize/"
    OIDC_OP_TOKEN_ENDPOINT = OIDC_OP_URL +"token/"
    OIDC_OP_USER_ENDPOINT = OIDC_OP_URL + "userinfo/"
-   OIDC_CALLBACK_CLASS= "justpass.OIDC_CLIENT.OIDCAuthn"
-   OIDC_AUTHENTICATE_CLASS = "justpass.OIDC_CLIENT.OIDC_AUTHENTICATE"
+   OIDC_CALLBACK_CLASS= "justpassme.OIDC_CLIENT.OIDCAuthn"
+   OIDC_AUTHENTICATE_CLASS = "justpassme.OIDC_CLIENT.OIDC_AUTHENTICATE"
    LOGIN_REDIRECT_URL_FAILURE="/justpass/failure/"
    LOGIN_REDIRECT_URL = "/justpass/success/"
 
    # If your application uses SSL.
    USE_X_FORWARDED_HOST = True
    SECURE_PROXY_SSL_HEADER = ('HTTP_X_FORWARDED_PROTO', 'https')
 
 
    # Provide the following functions that will be called when event is triggered, check example functions below
-   REGISTRATION_SUCCESS = "Shop.justpass.reg_success"
-   REGISTRATION_FAILURE = "Shop.justpass.reg_failure"
-   AUTHENTICATION_SUCCESS = "Shop.justpass.auth_success"
-   AUTHENTICATION_FAILURE = "Shop.justpass.auth_failure"
+   REGISTRATION_SUCCESS = "Your_App.justpass.reg_success"
+   REGISTRATION_FAILURE = "Your_App.justpass.reg_failure"
+   AUTHENTICATION_SUCCESS = "Your_App.justpass.auth_success"
+   AUTHENTICATION_FAILURE = "Your_App.justpass.auth_failure"
 
    ```
 3. Add `justpass` to your urls
    ```python 
    urls_patterns= [
    '...',
    path(r'justpass/', include('justpassme.urls')),
@@ -77,34 +77,25 @@
 Break your login function, Usually your login function will check for username and password, log the user in if the username and password are correct and create the user session, to support justpass.me, this has to change
    
    * authenticate the user
    * if username and password are correct , check if the user has mfa or not
        * if user has mfa then redirect to justpass.me
        * if user doesn't have mfa then call your function to create the user session
 
-3. To start registration, go `justpass:reg``
+3. To start registration, redirct to  `justpass:start_reg`
 
-   ```python
-   def start_reg(request):
-       from justpassme.helpers import start_reg
-       return start_reg(request)
-   ```
 
-4. Write a function to start login and add it to your `urls.py`
+4. To start login, redirect to `justpass:start_login`
 
-   **Note:** The function expects the user username to be in `request.session["base_username"]`
+   **Note:** For 2nd factor, The function expects the user's username to be in `request.session["base_username"]`
 
-   ```python
-   def start_login(request):
-       from justpassme.helpers import start_oidc_sign
-       return start_oidc_sign(request)
-   ```
 
-5. Write 4 functions that handle the success and failure of registration and login. 
-You can use the four functions below as a reference.
+5. Write 4 functions that handle the success and failure of registration and login, refer to them in the `settings.py` 
+
+   You can use the four functions below as a reference.
 
    ```python
    def auth_success(request):
       return redirect('home')
          
    def auth_failure(request):
      return render(request, 'login.html', {"failed": True})
```

### Comparing `justpass-me-django-3.0.2/justpass_me_django.egg-info/PKG-INFO` & `justpass-me-django-3.0.3/justpass_me_django.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: justpass-me-django
-Version: 3.0.2
+Version: 3.0.3
 Summary: Django Integration with JustPass.me
 Home-page: https://github.com/justpass-me/justpass-me-django
+Download-URL: https://github.com/justpass-me/justpass-me-django
 Author: JustPassMe
 Author-email: sameh@justpass.me
 License: MIT
-Download-URL: https://github.com/justpass-me/justpass-me-django
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.0
 Classifier: Framework :: Django :: 3.1
 Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.0
@@ -75,29 +74,29 @@
    OIDC_RP_SCOPES= "openid"
    OIDC_RP_SIGN_ALGO = 'HS256'
    OIDC_STORE_ID_TOKEN = True
    OIDC_OP_JWKS_ENDPOINT=OIDC_OP_URL  +"jwks"
    OIDC_OP_AUTHORIZATION_ENDPOINT=OIDC_OP_URL + "authorize/"
    OIDC_OP_TOKEN_ENDPOINT = OIDC_OP_URL +"token/"
    OIDC_OP_USER_ENDPOINT = OIDC_OP_URL + "userinfo/"
-   OIDC_CALLBACK_CLASS= "justpass.OIDC_CLIENT.OIDCAuthn"
-   OIDC_AUTHENTICATE_CLASS = "justpass.OIDC_CLIENT.OIDC_AUTHENTICATE"
+   OIDC_CALLBACK_CLASS= "justpassme.OIDC_CLIENT.OIDCAuthn"
+   OIDC_AUTHENTICATE_CLASS = "justpassme.OIDC_CLIENT.OIDC_AUTHENTICATE"
    LOGIN_REDIRECT_URL_FAILURE="/justpass/failure/"
    LOGIN_REDIRECT_URL = "/justpass/success/"
 
    # If your application uses SSL.
    USE_X_FORWARDED_HOST = True
    SECURE_PROXY_SSL_HEADER = ('HTTP_X_FORWARDED_PROTO', 'https')
 
 
    # Provide the following functions that will be called when event is triggered, check example functions below
-   REGISTRATION_SUCCESS = "Shop.justpass.reg_success"
-   REGISTRATION_FAILURE = "Shop.justpass.reg_failure"
-   AUTHENTICATION_SUCCESS = "Shop.justpass.auth_success"
-   AUTHENTICATION_FAILURE = "Shop.justpass.auth_failure"
+   REGISTRATION_SUCCESS = "Your_App.justpass.reg_success"
+   REGISTRATION_FAILURE = "Your_App.justpass.reg_failure"
+   AUTHENTICATION_SUCCESS = "Your_App.justpass.auth_success"
+   AUTHENTICATION_FAILURE = "Your_App.justpass.auth_failure"
 
    ```
 3. Add `justpass` to your urls
    ```python 
    urls_patterns= [
    '...',
    path(r'justpass/', include('justpassme.urls')),
@@ -110,34 +109,25 @@
 Break your login function, Usually your login function will check for username and password, log the user in if the username and password are correct and create the user session, to support justpass.me, this has to change
    
    * authenticate the user
    * if username and password are correct , check if the user has mfa or not
        * if user has mfa then redirect to justpass.me
        * if user doesn't have mfa then call your function to create the user session
 
-3. To start registration, go `justpass:reg``
+3. To start registration, redirct to  `justpass:start_reg`
 
-   ```python
-   def start_reg(request):
-       from justpassme.helpers import start_reg
-       return start_reg(request)
-   ```
 
-4. Write a function to start login and add it to your `urls.py`
+4. To start login, redirect to `justpass:start_login`
 
-   **Note:** The function expects the user username to be in `request.session["base_username"]`
+   **Note:** For 2nd factor, The function expects the user's username to be in `request.session["base_username"]`
 
-   ```python
-   def start_login(request):
-       from justpassme.helpers import start_oidc_sign
-       return start_oidc_sign(request)
-   ```
 
-5. Write 4 functions that handle the success and failure of registration and login. 
-You can use the four functions below as a reference.
+5. Write 4 functions that handle the success and failure of registration and login, refer to them in the `settings.py` 
+
+   You can use the four functions below as a reference.
 
    ```python
    def auth_success(request):
       return redirect('home')
          
    def auth_failure(request):
      return render(request, 'login.html', {"failed": True})
@@ -148,8 +138,7 @@
       request.session["reg"] = True
       return redirect('home')
       
    def reg_failure(request):
       request.session["reg"] = False
       return redirect('home')
    ```
-
```

### Comparing `justpass-me-django-3.0.2/justpassme/OIDC_CLIENT.py` & `justpass-me-django-3.0.3/justpassme/OIDC_CLIENT.py`

 * *Files identical despite different names*

### Comparing `justpass-me-django-3.0.2/justpassme/helpers.py` & `justpass-me-django-3.0.3/justpassme/helpers.py`

 * *Files identical despite different names*

### Comparing `justpass-me-django-3.0.2/justpassme/urls.py` & `justpass-me-django-3.0.3/justpassme/urls.py`

 * *Files identical despite different names*

### Comparing `justpass-me-django-3.0.2/justpassme/views.py` & `justpass-me-django-3.0.3/justpassme/views.py`

 * *Files identical despite different names*

### Comparing `justpass-me-django-3.0.2/setup-3.py` & `justpass-me-django-3.0.3/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 #!/usr/bin/env python
 
 from setuptools import find_packages, setup
 
 setup(
     name='justpass-me-django',
-    version='3.0.2',
+    version='3.0.3',
     description='Django Integration with JustPass.me',
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     author='JustPassMe',
     author_email = 'sameh@justpass.me',
     url = 'https://github.com/justpass-me/justpass-me-django',
     download_url='https://github.com/justpass-me/justpass-me-django',
     license='MIT',
     packages=find_packages(),
     install_requires=[
         'django >= 3.0',
         'mozilla-django-oidc==3.0.0',
+        'python-jose==3.3.0'
       ],
     python_requires=">=3.7",
     include_package_data=True,
     zip_safe=False, # because we're including static files
     classifiers=[
         #"Development Status :: 5 - Production/Stable",
         "Development Status :: 4 - Beta",
```

