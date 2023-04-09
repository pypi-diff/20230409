# Comparing `tmp/django-forbid-0.0.3.tar.gz` & `tmp/django-forbid-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-forbid-0.0.3.tar", last modified: Sat Apr  1 17:15:38 2023, max compression
+gzip compressed data, was "django-forbid-0.0.4.tar", last modified: Sun Apr  9 17:40:45 2023, max compression
```

## Comparing `django-forbid-0.0.3.tar` & `django-forbid-0.0.4.tar`

### file list

```diff
@@ -1,20 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 17:15:38.124029 django-forbid-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-04-01 17:15:24.000000 django-forbid-0.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4681 2023-04-01 17:15:38.124029 django-forbid-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3818 2023-04-01 17:15:24.000000 django-forbid-0.0.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-04-01 17:15:24.000000 django-forbid-0.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1002 2023-04-01 17:15:38.124029 django-forbid-0.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-01 17:15:24.000000 django-forbid-0.0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 17:15:38.120030 django-forbid-0.0.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 17:15:38.120030 django-forbid-0.0.3/src/django_forbid/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-01 17:15:24.000000 django-forbid-0.0.3/src/django_forbid/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2196 2023-04-01 17:15:24.000000 django-forbid-0.0.3/src/django_forbid/access.py
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-04-01 17:15:24.000000 django-forbid-0.0.3/src/django_forbid/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)     1429 2023-04-01 17:15:24.000000 django-forbid-0.0.3/src/django_forbid/middleware.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 17:15:38.124029 django-forbid-0.0.3/src/django_forbid.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4681 2023-04-01 17:15:38.000000 django-forbid-0.0.3/src/django_forbid.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      411 2023-04-01 17:15:38.000000 django-forbid-0.0.3/src/django_forbid.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-01 17:15:38.000000 django-forbid-0.0.3/src/django_forbid.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-01 17:15:38.000000 django-forbid-0.0.3/src/django_forbid.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-01 17:15:38.000000 django-forbid-0.0.3/src/django_forbid.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-01 17:15:38.000000 django-forbid-0.0.3/src/django_forbid.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 17:40:45.924976 django-forbid-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-04-09 17:40:37.000000 django-forbid-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5068 2023-04-09 17:40:45.924976 django-forbid-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4205 2023-04-09 17:40:37.000000 django-forbid-0.0.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-04-09 17:40:37.000000 django-forbid-0.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1002 2023-04-09 17:40:45.924976 django-forbid-0.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-09 17:40:37.000000 django-forbid-0.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 17:40:45.920976 django-forbid-0.0.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 17:40:45.920976 django-forbid-0.0.4/src/django_forbid/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-09 17:40:37.000000 django-forbid-0.0.4/src/django_forbid/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2873 2023-04-09 17:40:37.000000 django-forbid-0.0.4/src/django_forbid/access.py
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-04-09 17:40:37.000000 django-forbid-0.0.4/src/django_forbid/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2301 2023-04-09 17:40:37.000000 django-forbid-0.0.4/src/django_forbid/detect.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1493 2023-04-09 17:40:37.000000 django-forbid-0.0.4/src/django_forbid/middleware.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 17:40:45.920976 django-forbid-0.0.4/src/django_forbid.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5068 2023-04-09 17:40:45.000000 django-forbid-0.0.4/src/django_forbid.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      439 2023-04-09 17:40:45.000000 django-forbid-0.0.4/src/django_forbid.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-09 17:40:45.000000 django-forbid-0.0.4/src/django_forbid.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-09 17:40:45.000000 django-forbid-0.0.4/src/django_forbid.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-09 17:40:45.000000 django-forbid-0.0.4/src/django_forbid.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-09 17:40:45.000000 django-forbid-0.0.4/src/django_forbid.egg-info/top_level.txt
```

### Comparing `django-forbid-0.0.3/LICENSE` & `django-forbid-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `django-forbid-0.0.3/PKG-INFO` & `django-forbid-0.0.4/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-forbid
-Version: 0.0.3
+Version: 0.0.4
 Summary: Django app for forbidding access to some countries
 Home-page: https://github.com/pysnippet/django-forbid
 Author: Artyom Vancyan
 Author-email: artyom@pysnippet.org
 License: MIT
 Keywords: python,django,forbid,django-forbid
 Platform: unix
@@ -93,23 +93,31 @@
 FORBIDDEN_TERRITORIES = ['AF']
 ```
 
 The available ISO 3166 alpha-2 country codes are listed in [here](https://www.iban.com/country-codes). And the available
 ISO continent codes are: `AF` - Africa, `AN` - Antarctica, `AS` - Asia, `EU` - Europe, `NA` - North America, `OC` -
 Oceania and `SA` - South America.
 
+### Check access on timeout
+
 Without additional configuration, the middleware will check the user's access on every request. This can slow down the
 site. To avoid this, you can use the `FORBID_TIMEOUT` variable to set the cache timeout in seconds. When the timeout
 expires, the middleware will check the user's access again.
 
 ```python
 # Check the user's access every 10 minutes.
 FORBID_TIMEOUT = 60 * 10
 ```
 
+### Detect usage of a VPN
+
+If you want to detect the usage of a VPN, you can use the `FORBID_VPN` variable. When this variable is set to `True`,
+the middleware will check if the user's timezone matches the timezone the IP address belongs to. If the timezones do not
+match, the user will be considered in the usage of a VPN and forbidden to access the site.
+
 ## Contribute
 
 Any contribution is welcome. If you have any ideas or suggestions, feel free to open an issue or a pull request. And
 don't forget to add tests for your changes.
 
 ## License
```

### Comparing `django-forbid-0.0.3/README.md` & `django-forbid-0.0.4/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -67,23 +67,31 @@
 FORBIDDEN_TERRITORIES = ['AF']
 ```
 
 The available ISO 3166 alpha-2 country codes are listed in [here](https://www.iban.com/country-codes). And the available
 ISO continent codes are: `AF` - Africa, `AN` - Antarctica, `AS` - Asia, `EU` - Europe, `NA` - North America, `OC` -
 Oceania and `SA` - South America.
 
+### Check access on timeout
+
 Without additional configuration, the middleware will check the user's access on every request. This can slow down the
 site. To avoid this, you can use the `FORBID_TIMEOUT` variable to set the cache timeout in seconds. When the timeout
 expires, the middleware will check the user's access again.
 
 ```python
 # Check the user's access every 10 minutes.
 FORBID_TIMEOUT = 60 * 10
 ```
 
+### Detect usage of a VPN
+
+If you want to detect the usage of a VPN, you can use the `FORBID_VPN` variable. When this variable is set to `True`,
+the middleware will check if the user's timezone matches the timezone the IP address belongs to. If the timezones do not
+match, the user will be considered in the usage of a VPN and forbidden to access the site.
+
 ## Contribute
 
 Any contribution is welcome. If you have any ideas or suggestions, feel free to open an issue or a pull request. And
 don't forget to add tests for your changes.
 
 ## License
```

### Comparing `django-forbid-0.0.3/setup.cfg` & `django-forbid-0.0.4/setup.cfg`

 * *Files identical despite different names*

### Comparing `django-forbid-0.0.3/src/django_forbid/middleware.py` & `django-forbid-0.0.4/src/django_forbid/middleware.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 from django.conf import settings
 from django.http import HttpResponseForbidden
 from django.shortcuts import redirect
 from django.utils.timezone import utc
 
 from .access import grants_access
+from .detect import detect_vpn
 
 
 class ForbidMiddleware:
     """Middleware to forbid access to the site."""
 
     def __init__(self, get_response):
         self.get_response = get_response
@@ -20,20 +21,20 @@
 
         # Checks if the timeout variable is set and the user has been granted access.
         if hasattr(settings, "FORBID_TIMEOUT") and request.session.has_key("ACCESS"):
             acss = datetime.utcnow().replace(tzinfo=utc).timestamp()
 
             # Checks if access is not timed out yet.
             if acss - request.session.get("ACCESS") < settings.FORBID_TIMEOUT:
-                return self.get_response(request)
+                return detect_vpn(self.get_response, request)
 
         # Checks if access is granted when timeout is reached.
-        if grants_access(address.split(",")[0].strip()):
+        if grants_access(request, address.split(",")[0].strip()):
             acss = datetime.utcnow().replace(tzinfo=utc)
             request.session["ACCESS"] = acss.timestamp()
-            return self.get_response(request)
+            return detect_vpn(self.get_response, request)
 
         # Redirects to forbidden page if URL is set.
         if hasattr(settings, "FORBIDDEN_URL"):
             return redirect(settings.FORBIDDEN_URL)
 
         return HttpResponseForbidden()
```

### Comparing `django-forbid-0.0.3/src/django_forbid.egg-info/PKG-INFO` & `django-forbid-0.0.4/src/django_forbid.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-forbid
-Version: 0.0.3
+Version: 0.0.4
 Summary: Django app for forbidding access to some countries
 Home-page: https://github.com/pysnippet/django-forbid
 Author: Artyom Vancyan
 Author-email: artyom@pysnippet.org
 License: MIT
 Keywords: python,django,forbid,django-forbid
 Platform: unix
@@ -93,23 +93,31 @@
 FORBIDDEN_TERRITORIES = ['AF']
 ```
 
 The available ISO 3166 alpha-2 country codes are listed in [here](https://www.iban.com/country-codes). And the available
 ISO continent codes are: `AF` - Africa, `AN` - Antarctica, `AS` - Asia, `EU` - Europe, `NA` - North America, `OC` -
 Oceania and `SA` - South America.
 
+### Check access on timeout
+
 Without additional configuration, the middleware will check the user's access on every request. This can slow down the
 site. To avoid this, you can use the `FORBID_TIMEOUT` variable to set the cache timeout in seconds. When the timeout
 expires, the middleware will check the user's access again.
 
 ```python
 # Check the user's access every 10 minutes.
 FORBID_TIMEOUT = 60 * 10
 ```
 
+### Detect usage of a VPN
+
+If you want to detect the usage of a VPN, you can use the `FORBID_VPN` variable. When this variable is set to `True`,
+the middleware will check if the user's timezone matches the timezone the IP address belongs to. If the timezones do not
+match, the user will be considered in the usage of a VPN and forbidden to access the site.
+
 ## Contribute
 
 Any contribution is welcome. If you have any ideas or suggestions, feel free to open an issue or a pull request. And
 don't forget to add tests for your changes.
 
 ## License
```

