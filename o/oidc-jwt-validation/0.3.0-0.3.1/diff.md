# Comparing `tmp/oidc-jwt-validation-0.3.0.tar.gz` & `tmp/oidc-jwt-validation-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oidc-jwt-validation-0.3.0.tar", last modified: Sun Apr  9 11:51:19 2023, max compression
+gzip compressed data, was "oidc-jwt-validation-0.3.1.tar", last modified: Sun Apr  9 11:59:32 2023, max compression
```

## Comparing `oidc-jwt-validation-0.3.0.tar` & `oidc-jwt-validation-0.3.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 11:51:19.218886 oidc-jwt-validation-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-04-09 11:51:07.000000 oidc-jwt-validation-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      578 2023-04-09 11:51:19.218886 oidc-jwt-validation-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-04-09 11:51:07.000000 oidc-jwt-validation-0.3.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-09 11:51:19.218886 oidc-jwt-validation-0.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      927 2023-04-09 11:51:07.000000 oidc-jwt-validation-0.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 11:51:19.218886 oidc-jwt-validation-0.3.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 11:51:19.218886 oidc-jwt-validation-0.3.0/src/oidc_jwt_validation/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 11:51:07.000000 oidc-jwt-validation-0.3.0/src/oidc_jwt_validation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3614 2023-04-09 11:51:07.000000 oidc-jwt-validation-0.3.0/src/oidc_jwt_validation/authentication.py
--rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-04-09 11:51:07.000000 oidc-jwt-validation-0.3.0/src/oidc_jwt_validation/http_service.py
--rw-r--r--   0 runner    (1001) docker     (123)      767 2023-04-09 11:51:07.000000 oidc-jwt-validation-0.3.0/src/oidc_jwt_validation/http_singleton.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 11:51:19.218886 oidc-jwt-validation-0.3.0/src/oidc_jwt_validation.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      578 2023-04-09 11:51:19.000000 oidc-jwt-validation-0.3.0/src/oidc_jwt_validation.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      420 2023-04-09 11:51:19.000000 oidc-jwt-validation-0.3.0/src/oidc_jwt_validation.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-09 11:51:19.000000 oidc-jwt-validation-0.3.0/src/oidc_jwt_validation.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-04-09 11:51:19.000000 oidc-jwt-validation-0.3.0/src/oidc_jwt_validation.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-09 11:51:19.000000 oidc-jwt-validation-0.3.0/src/oidc_jwt_validation.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 11:59:32.124016 oidc-jwt-validation-0.3.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-04-09 11:59:16.000000 oidc-jwt-validation-0.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      578 2023-04-09 11:59:32.124016 oidc-jwt-validation-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-04-09 11:59:16.000000 oidc-jwt-validation-0.3.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-09 11:59:32.124016 oidc-jwt-validation-0.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-04-09 11:59:16.000000 oidc-jwt-validation-0.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 11:59:32.120016 oidc-jwt-validation-0.3.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 11:59:32.124016 oidc-jwt-validation-0.3.1/src/oidc_jwt_validation/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 11:59:16.000000 oidc-jwt-validation-0.3.1/src/oidc_jwt_validation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3629 2023-04-09 11:59:16.000000 oidc-jwt-validation-0.3.1/src/oidc_jwt_validation/authentication.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-04-09 11:59:16.000000 oidc-jwt-validation-0.3.1/src/oidc_jwt_validation/http_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)      767 2023-04-09 11:59:16.000000 oidc-jwt-validation-0.3.1/src/oidc_jwt_validation/http_singleton.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 11:59:32.124016 oidc-jwt-validation-0.3.1/src/oidc_jwt_validation.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      578 2023-04-09 11:59:32.000000 oidc-jwt-validation-0.3.1/src/oidc_jwt_validation.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      420 2023-04-09 11:59:32.000000 oidc-jwt-validation-0.3.1/src/oidc_jwt_validation.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-09 11:59:32.000000 oidc-jwt-validation-0.3.1/src/oidc_jwt_validation.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-04-09 11:59:32.000000 oidc-jwt-validation-0.3.1/src/oidc_jwt_validation.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-09 11:59:32.000000 oidc-jwt-validation-0.3.1/src/oidc_jwt_validation.egg-info/top_level.txt
```

### Comparing `oidc-jwt-validation-0.3.0/LICENSE` & `oidc-jwt-validation-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `oidc-jwt-validation-0.3.0/PKG-INFO` & `oidc-jwt-validation-0.3.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oidc-jwt-validation
-Version: 0.3.0
+Version: 0.3.1
 Summary: Oidc JWT Token validation
 Home-page: https://github.com/AxaGuilDEv/oidc-jwt-validation
 Author: Axa_france
 Author-email: guillaume.chervet@axa.fr, guillaume.thomas@axa.fr
 Platform: POSIX
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `oidc-jwt-validation-0.3.0/setup.py` & `oidc-jwt-validation-0.3.1/setup.py`

 * *Files identical despite different names*

### Comparing `oidc-jwt-validation-0.3.0/src/oidc_jwt_validation/authentication.py` & `oidc-jwt-validation-0.3.1/src/oidc_jwt_validation/authentication.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,15 +42,15 @@
             unverified_header = jwt.get_unverified_header(token)
             if not unverified_header["alg"].upper() in ALGORITHMS:
                 raise HTTPException(
                     status_code=status.HTTP_401_UNAUTHORIZED,
                     detail="description :wrong algorithm used",
                     headers={"WWW-Authenticate": "Bearer"},
                 )
-            jwks = await get_jwks_async(self.service, self.issuer)
+            jwks = await get_jwks_async(self.service, self.issuer, self.jwks_uri)
             rsa_key = {}
             for key in jwks["keys"]:
                 if key["kid"] == unverified_header["kid"]:
                     rsa_key = {"kty": key["kty"], "kid": key["kid"], "use": key["use"], "n": key["n"], "e": key["e"]}
             if rsa_key:
                 payload = jwt.decode(token, rsa_key, algorithms=ALGORITHMS, audience=audience, issuer=self.issuer)
                 if not is_scope_valid(payload, scope):
```

### Comparing `oidc-jwt-validation-0.3.0/src/oidc_jwt_validation/http_service.py` & `oidc-jwt-validation-0.3.1/src/oidc_jwt_validation/http_service.py`

 * *Files identical despite different names*

### Comparing `oidc-jwt-validation-0.3.0/src/oidc_jwt_validation/http_singleton.py` & `oidc-jwt-validation-0.3.1/src/oidc_jwt_validation/http_singleton.py`

 * *Files identical despite different names*

### Comparing `oidc-jwt-validation-0.3.0/src/oidc_jwt_validation.egg-info/PKG-INFO` & `oidc-jwt-validation-0.3.1/src/oidc_jwt_validation.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oidc-jwt-validation
-Version: 0.3.0
+Version: 0.3.1
 Summary: Oidc JWT Token validation
 Home-page: https://github.com/AxaGuilDEv/oidc-jwt-validation
 Author: Axa_france
 Author-email: guillaume.chervet@axa.fr, guillaume.thomas@axa.fr
 Platform: POSIX
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
```

