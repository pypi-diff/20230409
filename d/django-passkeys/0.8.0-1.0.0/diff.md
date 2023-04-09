# Comparing `tmp/django-passkeys-0.8.0.tar.gz` & `tmp/django-passkeys-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/django-passkeys-0.8.0.tar", last modified: Sun Dec 18 15:09:53 2022, max compression
+gzip compressed data, was "django-passkeys-1.0.0.tar", last modified: Sun Apr  9 09:42:26 2023, max compression
```

## Comparing `django-passkeys-0.8.0.tar` & `django-passkeys-1.0.0.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxrwxr-x   0 mohamed   (1000) mohamed   (1000)        0 2022-12-18 15:09:53.000000 django-passkeys-0.8.0/
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)     1075 2022-10-28 10:01:16.000000 django-passkeys-0.8.0/LICENSE
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)       74 2022-10-28 10:01:16.000000 django-passkeys-0.8.0/MANIFEST.in
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)     5971 2022-12-18 15:09:53.000000 django-passkeys-0.8.0/PKG-INFO
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)     4585 2022-12-18 15:09:15.000000 django-passkeys-0.8.0/README.md
-drwxrwxr-x   0 mohamed   (1000) mohamed   (1000)        0 2022-12-18 15:09:53.000000 django-passkeys-0.8.0/django_passkeys.egg-info/
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)     5971 2022-12-18 15:09:53.000000 django-passkeys-0.8.0/django_passkeys.egg-info/PKG-INFO
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)      864 2022-12-18 15:09:53.000000 django-passkeys-0.8.0/django_passkeys.egg-info/SOURCES.txt
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)        1 2022-12-18 15:09:53.000000 django-passkeys-0.8.0/django_passkeys.egg-info/dependency_links.txt
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)        1 2022-10-28 13:54:59.000000 django-passkeys-0.8.0/django_passkeys.egg-info/not-zip-safe
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)       47 2022-12-18 15:09:53.000000 django-passkeys-0.8.0/django_passkeys.egg-info/requires.txt
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)        9 2022-12-18 15:09:53.000000 django-passkeys-0.8.0/django_passkeys.egg-info/top_level.txt
-drwxrwxr-x   0 mohamed   (1000) mohamed   (1000)        0 2022-12-18 15:09:53.000000 django-passkeys-0.8.0/passkeys/
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)     5244 2022-12-18 15:08:24.000000 django-passkeys-0.8.0/passkeys/FIDO2.py
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)       65 2022-10-28 11:16:36.000000 django-passkeys-0.8.0/passkeys/__init__.py
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)      771 2022-12-09 11:09:53.000000 django-passkeys-0.8.0/passkeys/backend.py
-drwxrwxr-x   0 mohamed   (1000) mohamed   (1000)        0 2022-12-18 15:09:53.000000 django-passkeys-0.8.0/passkeys/migrations/
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)     1176 2022-10-28 13:18:42.000000 django-passkeys-0.8.0/passkeys/migrations/0001_initial.py
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)        0 2022-10-28 10:29:36.000000 django-passkeys-0.8.0/passkeys/migrations/__init__.py
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)      599 2022-12-09 11:07:59.000000 django-passkeys-0.8.0/passkeys/models.py
-drwxrwxr-x   0 mohamed   (1000) mohamed   (1000)        0 2022-12-18 15:09:53.000000 django-passkeys-0.8.0/passkeys/static/
-drwxrwxr-x   0 mohamed   (1000) mohamed   (1000)        0 2022-12-18 15:09:53.000000 django-passkeys-0.8.0/passkeys/static/passkeys/
-drwxrwxr-x   0 mohamed   (1000) mohamed   (1000)        0 2022-12-18 15:09:53.000000 django-passkeys-0.8.0/passkeys/static/passkeys/css/
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)     1590 2019-06-20 18:14:15.000000 django-passkeys-0.8.0/passkeys/static/passkeys/css/bootstrap-toggle.min.css
-drwxrwxr-x   0 mohamed   (1000) mohamed   (1000)        0 2022-12-18 15:09:53.000000 django-passkeys-0.8.0/passkeys/static/passkeys/imgs/
--rw-r--r--   0 mohamed   (1000) mohamed   (1000)     8981 2022-08-24 16:03:28.000000 django-passkeys-0.8.0/passkeys/static/passkeys/imgs/FIDO-Passkey_Icon-White.png
-drwxrwxr-x   0 mohamed   (1000) mohamed   (1000)        0 2022-12-18 15:09:53.000000 django-passkeys-0.8.0/passkeys/static/passkeys/js/
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)     2684 2022-10-23 19:24:16.000000 django-passkeys-0.8.0/passkeys/static/passkeys/js/base64url.js
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)     4129 2019-06-20 18:14:15.000000 django-passkeys-0.8.0/passkeys/static/passkeys/js/bootstrap-toggle.min.js
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)      687 2022-10-23 19:24:16.000000 django-passkeys-0.8.0/passkeys/static/passkeys/js/helpers.js
-drwxrwxr-x   0 mohamed   (1000) mohamed   (1000)        0 2022-12-18 15:09:53.000000 django-passkeys-0.8.0/passkeys/templates/
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)     5696 2022-12-09 11:08:08.000000 django-passkeys-0.8.0/passkeys/templates/PassKeys.html
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)      128 2022-10-28 10:53:07.000000 django-passkeys-0.8.0/passkeys/templates/PassKeys_base.html
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)      724 2022-12-09 11:08:08.000000 django-passkeys-0.8.0/passkeys/templates/check_passkeys.js
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)      807 2022-09-09 17:51:05.000000 django-passkeys-0.8.0/passkeys/templates/modal.html
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)     1769 2022-12-09 11:08:08.000000 django-passkeys-0.8.0/passkeys/templates/passkeys.js
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)      563 2022-12-09 11:08:08.000000 django-passkeys-0.8.0/passkeys/urls.py
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)      911 2022-12-09 11:08:08.000000 django-passkeys-0.8.0/passkeys/views.py
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)       38 2022-12-18 15:09:53.000000 django-passkeys-0.8.0/setup.cfg
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)     1777 2022-12-18 15:09:09.000000 django-passkeys-0.8.0/setup.py
+drwxrwxr-x   0 mohamed   (1000) mohamed   (1000)        0 2023-04-09 09:42:26.500876 django-passkeys-1.0.0/
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)     1075 2023-04-09 08:41:37.000000 django-passkeys-1.0.0/LICENSE
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)       74 2023-04-09 08:41:37.000000 django-passkeys-1.0.0/MANIFEST.in
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)     5962 2023-04-09 09:42:26.500876 django-passkeys-1.0.0/PKG-INFO
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)     4585 2023-04-09 08:41:37.000000 django-passkeys-1.0.0/README.md
+drwxrwxr-x   0 mohamed   (1000) mohamed   (1000)        0 2023-04-09 09:42:26.500876 django-passkeys-1.0.0/django_passkeys.egg-info/
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)     5962 2023-04-09 09:42:26.000000 django-passkeys-1.0.0/django_passkeys.egg-info/PKG-INFO
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)      864 2023-04-09 09:42:26.000000 django-passkeys-1.0.0/django_passkeys.egg-info/SOURCES.txt
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)        1 2023-04-09 09:42:26.000000 django-passkeys-1.0.0/django_passkeys.egg-info/dependency_links.txt
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)        1 2023-04-09 09:42:26.000000 django-passkeys-1.0.0/django_passkeys.egg-info/not-zip-safe
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)       47 2023-04-09 09:42:26.000000 django-passkeys-1.0.0/django_passkeys.egg-info/requires.txt
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)        9 2023-04-09 09:42:26.000000 django-passkeys-1.0.0/django_passkeys.egg-info/top_level.txt
+drwxrwxr-x   0 mohamed   (1000) mohamed   (1000)        0 2023-04-09 09:42:26.500876 django-passkeys-1.0.0/passkeys/
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)     5244 2023-04-09 08:41:37.000000 django-passkeys-1.0.0/passkeys/FIDO2.py
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)       65 2023-04-09 08:41:37.000000 django-passkeys-1.0.0/passkeys/__init__.py
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)      771 2023-04-09 08:41:37.000000 django-passkeys-1.0.0/passkeys/backend.py
+drwxrwxr-x   0 mohamed   (1000) mohamed   (1000)        0 2023-04-09 09:42:26.500876 django-passkeys-1.0.0/passkeys/migrations/
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)     1176 2023-04-09 08:41:37.000000 django-passkeys-1.0.0/passkeys/migrations/0001_initial.py
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)        0 2023-04-09 08:41:37.000000 django-passkeys-1.0.0/passkeys/migrations/__init__.py
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)      599 2023-04-09 08:41:37.000000 django-passkeys-1.0.0/passkeys/models.py
+drwxrwxr-x   0 mohamed   (1000) mohamed   (1000)        0 2023-04-09 09:42:26.496876 django-passkeys-1.0.0/passkeys/static/
+drwxrwxr-x   0 mohamed   (1000) mohamed   (1000)        0 2023-04-09 09:42:26.496876 django-passkeys-1.0.0/passkeys/static/passkeys/
+drwxrwxr-x   0 mohamed   (1000) mohamed   (1000)        0 2023-04-09 09:42:26.500876 django-passkeys-1.0.0/passkeys/static/passkeys/css/
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)     1590 2023-04-09 08:41:37.000000 django-passkeys-1.0.0/passkeys/static/passkeys/css/bootstrap-toggle.min.css
+drwxrwxr-x   0 mohamed   (1000) mohamed   (1000)        0 2023-04-09 09:42:26.500876 django-passkeys-1.0.0/passkeys/static/passkeys/imgs/
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)     8981 2023-04-09 08:41:37.000000 django-passkeys-1.0.0/passkeys/static/passkeys/imgs/FIDO-Passkey_Icon-White.png
+drwxrwxr-x   0 mohamed   (1000) mohamed   (1000)        0 2023-04-09 09:42:26.500876 django-passkeys-1.0.0/passkeys/static/passkeys/js/
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)     2684 2023-04-09 08:41:37.000000 django-passkeys-1.0.0/passkeys/static/passkeys/js/base64url.js
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)     4129 2023-04-09 08:41:37.000000 django-passkeys-1.0.0/passkeys/static/passkeys/js/bootstrap-toggle.min.js
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)      687 2023-04-09 08:41:37.000000 django-passkeys-1.0.0/passkeys/static/passkeys/js/helpers.js
+drwxrwxr-x   0 mohamed   (1000) mohamed   (1000)        0 2023-04-09 09:42:26.500876 django-passkeys-1.0.0/passkeys/templates/
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)     5696 2023-04-09 08:41:37.000000 django-passkeys-1.0.0/passkeys/templates/PassKeys.html
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)      128 2023-04-09 08:41:37.000000 django-passkeys-1.0.0/passkeys/templates/PassKeys_base.html
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)      724 2023-04-09 08:41:37.000000 django-passkeys-1.0.0/passkeys/templates/check_passkeys.js
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)      807 2023-04-09 08:41:37.000000 django-passkeys-1.0.0/passkeys/templates/modal.html
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)     1769 2023-04-09 08:41:37.000000 django-passkeys-1.0.0/passkeys/templates/passkeys.js
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)      563 2023-04-09 08:41:37.000000 django-passkeys-1.0.0/passkeys/urls.py
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)      911 2023-04-09 08:41:37.000000 django-passkeys-1.0.0/passkeys/views.py
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)       38 2023-04-09 09:42:26.500876 django-passkeys-1.0.0/setup.cfg
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)     1811 2023-04-09 09:40:02.000000 django-passkeys-1.0.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `django-passkeys-0.8.0/LICENSE` & `django-passkeys-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django-passkeys-0.8.0/PKG-INFO` & `django-passkeys-1.0.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 Metadata-Version: 2.1
 Name: django-passkeys
-Version: 0.8.0
+Version: 1.0.0
 Summary: A Django Authentication Backend for Passkeys
 Home-page: https://github.com/mkalioby/django-passkeys
 Download-URL: https://github.com/mkalioby/django-passkeys
 Author: Mohamed El-Kalioby
 Author-email: mkalioby@mkalioby.com
 License: MIT
-Classifier: Development Status :: 4 - Beta
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 2.0
 Classifier: Framework :: Django :: 2.1
 Classifier: Framework :: Django :: 2.2
 Classifier: Framework :: Django :: 3.0
 Classifier: Framework :: Django :: 3.1
 Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.0
+Classifier: Framework :: Django :: 4.1
+Classifier: Framework :: Django :: 4.2
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.7
```

#### html2text {}

```diff
@@ -1,51 +1,50 @@
-Metadata-Version: 2.1 Name: django-passkeys Version: 0.8.0 Summary: A Django
+Metadata-Version: 2.1 Name: django-passkeys Version: 1.0.0 Summary: A Django
 Authentication Backend for Passkeys Home-page: https://github.com/mkalioby/
 django-passkeys Download-URL: https://github.com/mkalioby/django-passkeys
 Author: Mohamed El-Kalioby Author-email: mkalioby@mkalioby.com License: MIT
-Classifier: Development Status :: 4 - Beta Classifier: Environment :: Web
-Environment Classifier: Framework :: Django Classifier: Framework :: Django ::
-2.0 Classifier: Framework :: Django :: 2.1 Classifier: Framework :: Django ::
-2.2 Classifier: Framework :: Django :: 3.0 Classifier: Framework :: Django ::
-3.1 Classifier: Framework :: Django :: 3.2 Classifier: Framework :: Django ::
-4.0 Classifier: Intended Audience :: Developers Classifier: Operating System ::
-OS Independent Classifier: Programming Language :: Python Classifier:
+Classifier: Development Status :: 5 - Production/Stable Classifier: Environment
+:: Web Environment Classifier: Framework :: Django Classifier: Framework ::
+Django :: 2.0 Classifier: Framework :: Django :: 2.1 Classifier: Framework ::
+Django :: 2.2 Classifier: Framework :: Django :: 3.0 Classifier: Framework ::
+Django :: 3.1 Classifier: Framework :: Django :: 3.2 Classifier: Framework ::
+Django :: 4.0 Classifier: Framework :: Django :: 4.1 Classifier: Framework ::
+Django :: 4.2 Classifier: Intended Audience :: Developers Classifier: Operating
+System :: OS Independent Classifier: Programming Language :: Python Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
-:: 3.5 Classifier: Programming Language :: Python :: 3.6 Classifier:
-Programming Language :: Python :: 3.7 Classifier: Programming Language ::
-Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
-Programming Language :: Python :: 3.10 Classifier: Programming Language ::
-Python :: 3.11 Classifier: Topic :: Software Development :: Libraries :: Python
-Modules Requires-Python: >=3.7 Description-Content-Type: text/markdown License-
-File: LICENSE # django-passkeys [![Downloads](https://pepy.tech/badge/django-
-passkeys/month)](https://pepy.tech/project/django-passkeys) An extension to
-Django *ModelBackend* backend to support passkeys. Passkeys is an extension to
-Web Authentication API that will allow the user to login to a service using
-another device. This app is a slim-down version of [django-mfa2](https://
-github.com/mkalioby/django-mfa2) Passkeys are now supported on * Apple
-Ecosystem (iPhone 16.0+, iPadOS 16.1, Mac OS X Ventura) * Chromium based
-browsers (on PC and Laptop) allows picking up credentials from Android and
-iPhone/iPadOS. * Android Credentials creation for ResidentKeys is currently in
-Beta. # Installation `pip install django-passkeys` Currently, it support Django
-2.0+, Python 3.7+ # Usage 1. in your settings.py add the application to your
-installed apps ```python INSTALLED_APPS=( '......', 'passkeys', '......') ```
-2. Collect Static Files `python manage.py collectstatic` 3. Run migrate `python
-manage.py migrate` 4. Add the following settings to your file ```python
-AUTHENTICATION_BACKENDS = ['passkeys.backend.PasskeyModelBackend'] # Change
-your authentication backend FIDO_SERVER_ID="localhost" # Server rp id for
-FIDO2, it the full domain of your project FIDO_SERVER_NAME="TestApp" import
-passkeys KEY_ATTACHMENT = NONE | passkeys.Attachment.CROSS_PLATFORM |
-passkeys.Attachment.PLATFORM ``` 5. Add passkeys to urls.py ```python
-urls_patterns= [ '...', url(r'^passkeys/', include('passkeys.urls')), '....', ]
-``` 6. To match the look and feel of your project, Passkeys includes
-`base.html` but it needs blocks named `head` & `content` to added its content
-to it. **Note:** You can override `PassKeys_base.html` which is used by
-`Passkeys.html` so you can control the styling better and current
-`Passkeys_base.html` extends `base.html` 7. Somewhere in your app, add a link
-to 'passkeys:home' ```
+:: 3.7 Classifier: Programming Language :: Python :: 3.8 Classifier:
+Programming Language :: Python :: 3.9 Classifier: Programming Language ::
+Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
+Topic :: Software Development :: Libraries :: Python Modules Requires-Python:
+>=3.7 Description-Content-Type: text/markdown License-File: LICENSE # django-
+passkeys [![Downloads](https://pepy.tech/badge/django-passkeys/month)](https://
+pepy.tech/project/django-passkeys) An extension to Django *ModelBackend*
+backend to support passkeys. Passkeys is an extension to Web Authentication API
+that will allow the user to login to a service using another device. This app
+is a slim-down version of [django-mfa2](https://github.com/mkalioby/django-
+mfa2) Passkeys are now supported on * Apple Ecosystem (iPhone 16.0+, iPadOS
+16.1, Mac OS X Ventura) * Chromium based browsers (on PC and Laptop) allows
+picking up credentials from Android and iPhone/iPadOS. * Android Credentials
+creation for ResidentKeys is currently in Beta. # Installation `pip install
+django-passkeys` Currently, it support Django 2.0+, Python 3.7+ # Usage 1. in
+your settings.py add the application to your installed apps ```python
+INSTALLED_APPS=( '......', 'passkeys', '......') ``` 2. Collect Static Files
+`python manage.py collectstatic` 3. Run migrate `python manage.py migrate` 4.
+Add the following settings to your file ```python AUTHENTICATION_BACKENDS =
+['passkeys.backend.PasskeyModelBackend'] # Change your authentication backend
+FIDO_SERVER_ID="localhost" # Server rp id for FIDO2, it the full domain of your
+project FIDO_SERVER_NAME="TestApp" import passkeys KEY_ATTACHMENT = NONE |
+passkeys.Attachment.CROSS_PLATFORM | passkeys.Attachment.PLATFORM ``` 5. Add
+passkeys to urls.py ```python urls_patterns= [ '...', url(r'^passkeys/',
+include('passkeys.urls')), '....', ] ``` 6. To match the look and feel of your
+project, Passkeys includes `base.html` but it needs blocks named `head` &
+`content` to added its content to it. **Note:** You can override
+`PassKeys_base.html` which is used by `Passkeys.html` so you can control the
+styling better and current `Passkeys_base.html` extends `base.html` 7.
+Somewhere in your app, add a link to 'passkeys:home' ```
 Passkeys
 ``` 8. In your login view, change the authenticate call to include the request
 as follows ```python user=authenticate(request, username=request.POST
 ["username"],password=request.POST["password"]) ``` 8. Finally, In your
 `login.html` * Give an id to your login form e.g 'loginForm', the id should be
 provided when calling `authn` function * Inside the form, add ```html  [{%
 static 'passkeys/imgs/FIDO-Passkey_Icon-White.png' %}] {%include 'passkeys.js'
```

### Comparing `django-passkeys-0.8.0/README.md` & `django-passkeys-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `django-passkeys-0.8.0/django_passkeys.egg-info/PKG-INFO` & `django-passkeys-1.0.0/django_passkeys.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 Metadata-Version: 2.1
 Name: django-passkeys
-Version: 0.8.0
+Version: 1.0.0
 Summary: A Django Authentication Backend for Passkeys
 Home-page: https://github.com/mkalioby/django-passkeys
 Download-URL: https://github.com/mkalioby/django-passkeys
 Author: Mohamed El-Kalioby
 Author-email: mkalioby@mkalioby.com
 License: MIT
-Classifier: Development Status :: 4 - Beta
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 2.0
 Classifier: Framework :: Django :: 2.1
 Classifier: Framework :: Django :: 2.2
 Classifier: Framework :: Django :: 3.0
 Classifier: Framework :: Django :: 3.1
 Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.0
+Classifier: Framework :: Django :: 4.1
+Classifier: Framework :: Django :: 4.2
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.7
```

#### html2text {}

```diff
@@ -1,51 +1,50 @@
-Metadata-Version: 2.1 Name: django-passkeys Version: 0.8.0 Summary: A Django
+Metadata-Version: 2.1 Name: django-passkeys Version: 1.0.0 Summary: A Django
 Authentication Backend for Passkeys Home-page: https://github.com/mkalioby/
 django-passkeys Download-URL: https://github.com/mkalioby/django-passkeys
 Author: Mohamed El-Kalioby Author-email: mkalioby@mkalioby.com License: MIT
-Classifier: Development Status :: 4 - Beta Classifier: Environment :: Web
-Environment Classifier: Framework :: Django Classifier: Framework :: Django ::
-2.0 Classifier: Framework :: Django :: 2.1 Classifier: Framework :: Django ::
-2.2 Classifier: Framework :: Django :: 3.0 Classifier: Framework :: Django ::
-3.1 Classifier: Framework :: Django :: 3.2 Classifier: Framework :: Django ::
-4.0 Classifier: Intended Audience :: Developers Classifier: Operating System ::
-OS Independent Classifier: Programming Language :: Python Classifier:
+Classifier: Development Status :: 5 - Production/Stable Classifier: Environment
+:: Web Environment Classifier: Framework :: Django Classifier: Framework ::
+Django :: 2.0 Classifier: Framework :: Django :: 2.1 Classifier: Framework ::
+Django :: 2.2 Classifier: Framework :: Django :: 3.0 Classifier: Framework ::
+Django :: 3.1 Classifier: Framework :: Django :: 3.2 Classifier: Framework ::
+Django :: 4.0 Classifier: Framework :: Django :: 4.1 Classifier: Framework ::
+Django :: 4.2 Classifier: Intended Audience :: Developers Classifier: Operating
+System :: OS Independent Classifier: Programming Language :: Python Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
-:: 3.5 Classifier: Programming Language :: Python :: 3.6 Classifier:
-Programming Language :: Python :: 3.7 Classifier: Programming Language ::
-Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
-Programming Language :: Python :: 3.10 Classifier: Programming Language ::
-Python :: 3.11 Classifier: Topic :: Software Development :: Libraries :: Python
-Modules Requires-Python: >=3.7 Description-Content-Type: text/markdown License-
-File: LICENSE # django-passkeys [![Downloads](https://pepy.tech/badge/django-
-passkeys/month)](https://pepy.tech/project/django-passkeys) An extension to
-Django *ModelBackend* backend to support passkeys. Passkeys is an extension to
-Web Authentication API that will allow the user to login to a service using
-another device. This app is a slim-down version of [django-mfa2](https://
-github.com/mkalioby/django-mfa2) Passkeys are now supported on * Apple
-Ecosystem (iPhone 16.0+, iPadOS 16.1, Mac OS X Ventura) * Chromium based
-browsers (on PC and Laptop) allows picking up credentials from Android and
-iPhone/iPadOS. * Android Credentials creation for ResidentKeys is currently in
-Beta. # Installation `pip install django-passkeys` Currently, it support Django
-2.0+, Python 3.7+ # Usage 1. in your settings.py add the application to your
-installed apps ```python INSTALLED_APPS=( '......', 'passkeys', '......') ```
-2. Collect Static Files `python manage.py collectstatic` 3. Run migrate `python
-manage.py migrate` 4. Add the following settings to your file ```python
-AUTHENTICATION_BACKENDS = ['passkeys.backend.PasskeyModelBackend'] # Change
-your authentication backend FIDO_SERVER_ID="localhost" # Server rp id for
-FIDO2, it the full domain of your project FIDO_SERVER_NAME="TestApp" import
-passkeys KEY_ATTACHMENT = NONE | passkeys.Attachment.CROSS_PLATFORM |
-passkeys.Attachment.PLATFORM ``` 5. Add passkeys to urls.py ```python
-urls_patterns= [ '...', url(r'^passkeys/', include('passkeys.urls')), '....', ]
-``` 6. To match the look and feel of your project, Passkeys includes
-`base.html` but it needs blocks named `head` & `content` to added its content
-to it. **Note:** You can override `PassKeys_base.html` which is used by
-`Passkeys.html` so you can control the styling better and current
-`Passkeys_base.html` extends `base.html` 7. Somewhere in your app, add a link
-to 'passkeys:home' ```
+:: 3.7 Classifier: Programming Language :: Python :: 3.8 Classifier:
+Programming Language :: Python :: 3.9 Classifier: Programming Language ::
+Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
+Topic :: Software Development :: Libraries :: Python Modules Requires-Python:
+>=3.7 Description-Content-Type: text/markdown License-File: LICENSE # django-
+passkeys [![Downloads](https://pepy.tech/badge/django-passkeys/month)](https://
+pepy.tech/project/django-passkeys) An extension to Django *ModelBackend*
+backend to support passkeys. Passkeys is an extension to Web Authentication API
+that will allow the user to login to a service using another device. This app
+is a slim-down version of [django-mfa2](https://github.com/mkalioby/django-
+mfa2) Passkeys are now supported on * Apple Ecosystem (iPhone 16.0+, iPadOS
+16.1, Mac OS X Ventura) * Chromium based browsers (on PC and Laptop) allows
+picking up credentials from Android and iPhone/iPadOS. * Android Credentials
+creation for ResidentKeys is currently in Beta. # Installation `pip install
+django-passkeys` Currently, it support Django 2.0+, Python 3.7+ # Usage 1. in
+your settings.py add the application to your installed apps ```python
+INSTALLED_APPS=( '......', 'passkeys', '......') ``` 2. Collect Static Files
+`python manage.py collectstatic` 3. Run migrate `python manage.py migrate` 4.
+Add the following settings to your file ```python AUTHENTICATION_BACKENDS =
+['passkeys.backend.PasskeyModelBackend'] # Change your authentication backend
+FIDO_SERVER_ID="localhost" # Server rp id for FIDO2, it the full domain of your
+project FIDO_SERVER_NAME="TestApp" import passkeys KEY_ATTACHMENT = NONE |
+passkeys.Attachment.CROSS_PLATFORM | passkeys.Attachment.PLATFORM ``` 5. Add
+passkeys to urls.py ```python urls_patterns= [ '...', url(r'^passkeys/',
+include('passkeys.urls')), '....', ] ``` 6. To match the look and feel of your
+project, Passkeys includes `base.html` but it needs blocks named `head` &
+`content` to added its content to it. **Note:** You can override
+`PassKeys_base.html` which is used by `Passkeys.html` so you can control the
+styling better and current `Passkeys_base.html` extends `base.html` 7.
+Somewhere in your app, add a link to 'passkeys:home' ```
 Passkeys
 ``` 8. In your login view, change the authenticate call to include the request
 as follows ```python user=authenticate(request, username=request.POST
 ["username"],password=request.POST["password"]) ``` 8. Finally, In your
 `login.html` * Give an id to your login form e.g 'loginForm', the id should be
 provided when calling `authn` function * Inside the form, add ```html  [{%
 static 'passkeys/imgs/FIDO-Passkey_Icon-White.png' %}] {%include 'passkeys.js'
```

### Comparing `django-passkeys-0.8.0/django_passkeys.egg-info/SOURCES.txt` & `django-passkeys-1.0.0/django_passkeys.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-passkeys-0.8.0/passkeys/FIDO2.py` & `django-passkeys-1.0.0/passkeys/FIDO2.py`

 * *Files identical despite different names*

### Comparing `django-passkeys-0.8.0/passkeys/backend.py` & `django-passkeys-1.0.0/passkeys/backend.py`

 * *Files identical despite different names*

### Comparing `django-passkeys-0.8.0/passkeys/migrations/0001_initial.py` & `django-passkeys-1.0.0/passkeys/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-passkeys-0.8.0/passkeys/models.py` & `django-passkeys-1.0.0/passkeys/models.py`

 * *Files identical despite different names*

### Comparing `django-passkeys-0.8.0/passkeys/static/passkeys/css/bootstrap-toggle.min.css` & `django-passkeys-1.0.0/passkeys/static/passkeys/css/bootstrap-toggle.min.css`

 * *Files identical despite different names*

### Comparing `django-passkeys-0.8.0/passkeys/static/passkeys/imgs/FIDO-Passkey_Icon-White.png` & `django-passkeys-1.0.0/passkeys/static/passkeys/imgs/FIDO-Passkey_Icon-White.png`

 * *Files identical despite different names*

### Comparing `django-passkeys-0.8.0/passkeys/static/passkeys/js/base64url.js` & `django-passkeys-1.0.0/passkeys/static/passkeys/js/base64url.js`

 * *Files identical despite different names*

### Comparing `django-passkeys-0.8.0/passkeys/static/passkeys/js/bootstrap-toggle.min.js` & `django-passkeys-1.0.0/passkeys/static/passkeys/js/bootstrap-toggle.min.js`

 * *Files identical despite different names*

### Comparing `django-passkeys-0.8.0/passkeys/static/passkeys/js/helpers.js` & `django-passkeys-1.0.0/passkeys/static/passkeys/js/helpers.js`

 * *Files identical despite different names*

### Comparing `django-passkeys-0.8.0/passkeys/templates/PassKeys.html` & `django-passkeys-1.0.0/passkeys/templates/PassKeys.html`

 * *Files identical despite different names*

### Comparing `django-passkeys-0.8.0/passkeys/templates/check_passkeys.js` & `django-passkeys-1.0.0/passkeys/templates/check_passkeys.js`

 * *Files identical despite different names*

### Comparing `django-passkeys-0.8.0/passkeys/templates/modal.html` & `django-passkeys-1.0.0/passkeys/templates/modal.html`

 * *Files identical despite different names*

### Comparing `django-passkeys-0.8.0/passkeys/templates/passkeys.js` & `django-passkeys-1.0.0/passkeys/templates/passkeys.js`

 * *Files identical despite different names*

### Comparing `django-passkeys-0.8.0/passkeys/urls.py` & `django-passkeys-1.0.0/passkeys/urls.py`

 * *Files identical despite different names*

### Comparing `django-passkeys-0.8.0/passkeys/views.py` & `django-passkeys-1.0.0/passkeys/views.py`

 * *Files identical despite different names*

### Comparing `django-passkeys-0.8.0/setup.py` & `django-passkeys-1.0.0/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,49 +1,50 @@
 #!/usr/bin/env python
 
 from setuptools import find_packages, setup
 
 setup(
     name='django-passkeys',
-    version='0.8.0',
+    version='1.0.0',
     description='A Django Authentication Backend for Passkeys',
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     author='Mohamed El-Kalioby',
     author_email = 'mkalioby@mkalioby.com',
     url = 'https://github.com/mkalioby/django-passkeys',
     download_url='https://github.com/mkalioby/django-passkeys',
     license='MIT',
     packages=find_packages(),
     install_requires=[
         'django >= 2.0',
         'ua-parser',
         'user-agents',
-        'fido2 == 1.1.0',
+        'fido2 == 1.1.1',
       ],
     python_requires=">=3.7",
     include_package_data=True,
     zip_safe=False, # because we're including static files
     classifiers=[
-        "Development Status :: 4 - Beta",
+        "Development Status :: 5 - Production/Stable",
+        #"Development Status :: 4 - Beta",
         "Environment :: Web Environment",
         "Framework :: Django",
         "Framework :: Django :: 2.0",
         "Framework :: Django :: 2.1",
         "Framework :: Django :: 2.2",
         "Framework :: Django :: 3.0",
         "Framework :: Django :: 3.1",
         "Framework :: Django :: 3.2",
         "Framework :: Django :: 4.0",
+        "Framework :: Django :: 4.1",
+        "Framework :: Django :: 4.2",
         "Intended Audience :: Developers",
         "Operating System :: OS Independent",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.5",
-        "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
         "Topic :: Software Development :: Libraries :: Python Modules",
 ]
```

