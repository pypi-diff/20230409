# Comparing `tmp/keyrock-encryption-2023.4.8.1854.tar.gz` & `tmp/keyrock-encryption-2023.4.9.1358.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "keyrock-encryption-2023.4.8.1854.tar", last modified: Sat Apr  8 18:54:09 2023, max compression
+gzip compressed data, was "keyrock-encryption-2023.4.9.1358.tar", last modified: Sun Apr  9 13:58:37 2023, max compression
```

## Comparing `keyrock-encryption-2023.4.8.1854.tar` & `keyrock-encryption-2023.4.9.1358.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-08 18:54:09.668588 keyrock-encryption-2023.4.8.1854/
--rw-r--r--   0 root         (0) root         (0)       70 2023-04-08 18:54:09.668588 keyrock-encryption-2023.4.8.1854/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-08 18:54:09.665588 keyrock-encryption-2023.4.8.1854/keyrock_encryption/
--rw-rw-rw-   0 root         (0) root         (0)       80 2023-04-08 18:53:52.000000 keyrock-encryption-2023.4.8.1854/keyrock_encryption/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-08 18:54:09.668588 keyrock-encryption-2023.4.8.1854/keyrock_encryption/encryption/
--rw-rw-rw-   0 root         (0) root         (0)       25 2023-04-08 18:53:52.000000 keyrock-encryption-2023.4.8.1854/keyrock_encryption/encryption/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1968 2023-04-08 18:53:52.000000 keyrock-encryption-2023.4.8.1854/keyrock_encryption/encryption/encryption.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-08 18:53:52.000000 keyrock-encryption-2023.4.8.1854/keyrock_encryption/encryption/test_encryption.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-08 18:54:09.667588 keyrock-encryption-2023.4.8.1854/keyrock_encryption.egg-info/
--rw-r--r--   0 root         (0) root         (0)       70 2023-04-08 18:54:09.000000 keyrock-encryption-2023.4.8.1854/keyrock_encryption.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      399 2023-04-08 18:54:09.000000 keyrock-encryption-2023.4.8.1854/keyrock_encryption.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-08 18:54:09.000000 keyrock-encryption-2023.4.8.1854/keyrock_encryption.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       26 2023-04-08 18:54:09.000000 keyrock-encryption-2023.4.8.1854/keyrock_encryption.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       19 2023-04-08 18:54:09.000000 keyrock-encryption-2023.4.8.1854/keyrock_encryption.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)       80 2023-04-08 18:53:52.000000 keyrock-encryption-2023.4.8.1854/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)      182 2023-04-08 18:54:09.669588 keyrock-encryption-2023.4.8.1854/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-09 13:58:37.590467 keyrock-encryption-2023.4.9.1358/
+-rw-r--r--   0 root         (0) root         (0)       70 2023-04-09 13:58:37.590467 keyrock-encryption-2023.4.9.1358/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-09 13:58:37.586799 keyrock-encryption-2023.4.9.1358/keyrock_encryption/
+-rw-rw-rw-   0 root         (0) root         (0)       80 2023-04-09 13:58:21.000000 keyrock-encryption-2023.4.9.1358/keyrock_encryption/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-09 13:58:37.590467 keyrock-encryption-2023.4.9.1358/keyrock_encryption/encryption/
+-rw-rw-rw-   0 root         (0) root         (0)       25 2023-04-09 13:58:21.000000 keyrock-encryption-2023.4.9.1358/keyrock_encryption/encryption/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1934 2023-04-09 13:58:21.000000 keyrock-encryption-2023.4.9.1358/keyrock_encryption/encryption/encryption.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-09 13:58:21.000000 keyrock-encryption-2023.4.9.1358/keyrock_encryption/encryption/test_encryption.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-09 13:58:37.588633 keyrock-encryption-2023.4.9.1358/keyrock_encryption.egg-info/
+-rw-r--r--   0 root         (0) root         (0)       70 2023-04-09 13:58:37.000000 keyrock-encryption-2023.4.9.1358/keyrock_encryption.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      399 2023-04-09 13:58:37.000000 keyrock-encryption-2023.4.9.1358/keyrock_encryption.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-09 13:58:37.000000 keyrock-encryption-2023.4.9.1358/keyrock_encryption.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       26 2023-04-09 13:58:37.000000 keyrock-encryption-2023.4.9.1358/keyrock_encryption.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       19 2023-04-09 13:58:37.000000 keyrock-encryption-2023.4.9.1358/keyrock_encryption.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)       80 2023-04-09 13:58:21.000000 keyrock-encryption-2023.4.9.1358/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)      182 2023-04-09 13:58:37.590467 keyrock-encryption-2023.4.9.1358/setup.cfg
```

### Comparing `keyrock-encryption-2023.4.8.1854/keyrock_encryption/encryption/encryption.py` & `keyrock-encryption-2023.4.9.1358/keyrock_encryption/encryption/encryption.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,17 @@
 import base64
 import hashlib
 import json
 import re
 import string
 import random
 
-try:
-    from Crypto import Random
-    from Crypto.Cipher import AES
-    from Crypto.Util.Padding import pad, unpad
-except:
-    pass
+from Crypto import Random
+from Crypto.Cipher import AES
+from Crypto.Util.Padding import pad, unpad
 
 from keyrock_core import json_util
 
 
 class AESCipher(object):
     def __init__(self, key):
         self.bs = AES.block_size
```

