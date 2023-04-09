# Comparing `tmp/oidc-jwt-validation-0.2.0.tar.gz` & `tmp/oidc-jwt-validation-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oidc-jwt-validation-0.2.0.tar", last modified: Tue Jan  3 17:02:22 2023, max compression
+gzip compressed data, was "oidc-jwt-validation-0.3.0.tar", last modified: Sun Apr  9 11:51:19 2023, max compression
```

## Comparing `oidc-jwt-validation-0.2.0.tar` & `oidc-jwt-validation-0.3.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-03 17:02:22.603843 oidc-jwt-validation-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-01-03 17:02:10.000000 oidc-jwt-validation-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      578 2023-01-03 17:02:22.603843 oidc-jwt-validation-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-01-03 17:02:10.000000 oidc-jwt-validation-0.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-03 17:02:22.603843 oidc-jwt-validation-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      927 2023-01-03 17:02:10.000000 oidc-jwt-validation-0.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-03 17:02:22.603843 oidc-jwt-validation-0.2.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-03 17:02:22.603843 oidc-jwt-validation-0.2.0/src/oidc_jwt_validation/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-03 17:02:10.000000 oidc-jwt-validation-0.2.0/src/oidc_jwt_validation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3540 2023-01-03 17:02:10.000000 oidc-jwt-validation-0.2.0/src/oidc_jwt_validation/authentication.py
--rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-01-03 17:02:10.000000 oidc-jwt-validation-0.2.0/src/oidc_jwt_validation/http_service.py
--rw-r--r--   0 runner    (1001) docker     (123)      767 2023-01-03 17:02:10.000000 oidc-jwt-validation-0.2.0/src/oidc_jwt_validation/http_singleton.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-03 17:02:22.603843 oidc-jwt-validation-0.2.0/src/oidc_jwt_validation.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      578 2023-01-03 17:02:22.000000 oidc-jwt-validation-0.2.0/src/oidc_jwt_validation.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      420 2023-01-03 17:02:22.000000 oidc-jwt-validation-0.2.0/src/oidc_jwt_validation.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-03 17:02:22.000000 oidc-jwt-validation-0.2.0/src/oidc_jwt_validation.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-01-03 17:02:22.000000 oidc-jwt-validation-0.2.0/src/oidc_jwt_validation.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-01-03 17:02:22.000000 oidc-jwt-validation-0.2.0/src/oidc_jwt_validation.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 11:51:19.218886 oidc-jwt-validation-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-04-09 11:51:07.000000 oidc-jwt-validation-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      578 2023-04-09 11:51:19.218886 oidc-jwt-validation-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-04-09 11:51:07.000000 oidc-jwt-validation-0.3.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-09 11:51:19.218886 oidc-jwt-validation-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-04-09 11:51:07.000000 oidc-jwt-validation-0.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 11:51:19.218886 oidc-jwt-validation-0.3.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 11:51:19.218886 oidc-jwt-validation-0.3.0/src/oidc_jwt_validation/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 11:51:07.000000 oidc-jwt-validation-0.3.0/src/oidc_jwt_validation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3614 2023-04-09 11:51:07.000000 oidc-jwt-validation-0.3.0/src/oidc_jwt_validation/authentication.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-04-09 11:51:07.000000 oidc-jwt-validation-0.3.0/src/oidc_jwt_validation/http_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)      767 2023-04-09 11:51:07.000000 oidc-jwt-validation-0.3.0/src/oidc_jwt_validation/http_singleton.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 11:51:19.218886 oidc-jwt-validation-0.3.0/src/oidc_jwt_validation.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      578 2023-04-09 11:51:19.000000 oidc-jwt-validation-0.3.0/src/oidc_jwt_validation.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      420 2023-04-09 11:51:19.000000 oidc-jwt-validation-0.3.0/src/oidc_jwt_validation.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-09 11:51:19.000000 oidc-jwt-validation-0.3.0/src/oidc_jwt_validation.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-04-09 11:51:19.000000 oidc-jwt-validation-0.3.0/src/oidc_jwt_validation.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-09 11:51:19.000000 oidc-jwt-validation-0.3.0/src/oidc_jwt_validation.egg-info/top_level.txt
```

### Comparing `oidc-jwt-validation-0.2.0/LICENSE` & `oidc-jwt-validation-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `oidc-jwt-validation-0.2.0/PKG-INFO` & `oidc-jwt-validation-0.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oidc-jwt-validation
-Version: 0.2.0
+Version: 0.3.0
 Summary: Oidc JWT Token validation
 Home-page: https://github.com/AxaGuilDEv/oidc-jwt-validation
 Author: Axa_france
 Author-email: guillaume.chervet@axa.fr, guillaume.thomas@axa.fr
 Platform: POSIX
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `oidc-jwt-validation-0.2.0/setup.py` & `oidc-jwt-validation-0.3.0/setup.py`

 * *Files identical despite different names*

### Comparing `oidc-jwt-validation-0.2.0/src/oidc_jwt_validation/authentication.py` & `oidc-jwt-validation-0.3.0/src/oidc_jwt_validation/authentication.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,38 +5,39 @@
 from .http_service import ServiceGet
 
 ALGORITHMS = ["RS256"]
 cache_timestamp = 0
 cache_jwks = None
 
 
-async def get_jwks_async(service: ServiceGet, issuer: str):
+async def get_jwks_async(service: ServiceGet, issuer: str, jwks_uri: str = "/jwks"):
     global cache_timestamp
     global cache_jwks
     timestamp = datetime.timestamp(datetime.now())
     if cache_timestamp + 86400 < timestamp:
-        json_url = issuer + "/jwks"
+        json_url = issuer + jwks_uri
         cache_jwks = await service.get_async(json_url)
         cache_timestamp = timestamp
 
     return cache_jwks
 
 
 def is_scope_valid(payload: dict, scope: str):
     if payload is not None and "scope" in payload:
         scope_from_payload = str(payload["scope"])
         return scope_from_payload is not None and scope in scope_from_payload.split(" ")
     return False
 
 
 class Authentication:
-    def __init__(self, logger: Logger, issuer: str, service: ServiceGet):
+    def __init__(self, logger: Logger, issuer: str, service: ServiceGet, jwks_uri: str):
         self.logger = logger
         self.service = service
         self.issuer = issuer
+        self.jwks_uri = jwks_uri
 
     async def validate_async(self, token, audience: str, scope: str):
         logger = self.logger
         try:
             logger.debug("begin authentication with: %s", token)
             unverified_header = jwt.get_unverified_header(token)
             if not unverified_header["alg"].upper() in ALGORITHMS:
```

### Comparing `oidc-jwt-validation-0.2.0/src/oidc_jwt_validation/http_service.py` & `oidc-jwt-validation-0.3.0/src/oidc_jwt_validation/http_service.py`

 * *Files identical despite different names*

### Comparing `oidc-jwt-validation-0.2.0/src/oidc_jwt_validation/http_singleton.py` & `oidc-jwt-validation-0.3.0/src/oidc_jwt_validation/http_singleton.py`

 * *Files identical despite different names*

### Comparing `oidc-jwt-validation-0.2.0/src/oidc_jwt_validation.egg-info/PKG-INFO` & `oidc-jwt-validation-0.3.0/src/oidc_jwt_validation.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oidc-jwt-validation
-Version: 0.2.0
+Version: 0.3.0
 Summary: Oidc JWT Token validation
 Home-page: https://github.com/AxaGuilDEv/oidc-jwt-validation
 Author: Axa_france
 Author-email: guillaume.chervet@axa.fr, guillaume.thomas@axa.fr
 Platform: POSIX
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
```

