# Comparing `tmp/dxsp-0.0.5.tar.gz` & `tmp/dxsp-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dxsp-0.0.5.tar", last modified: Sun Apr  9 12:06:54 2023, max compression
+gzip compressed data, was "dxsp-0.0.7.tar", last modified: Sun Apr  9 12:50:43 2023, max compression
```

## Comparing `dxsp-0.0.5.tar` & `dxsp-0.0.7.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 12:06:54.499751 dxsp-0.0.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-04-09 12:06:24.000000 dxsp-0.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2883 2023-04-09 12:06:54.499751 dxsp-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2396 2023-04-09 12:06:24.000000 dxsp-0.0.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 12:06:54.495751 dxsp-0.0.5/dxsp/
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-09 12:06:24.000000 dxsp-0.0.5/dxsp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10359 2023-04-09 12:06:24.000000 dxsp-0.0.5/dxsp/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 12:06:54.495751 dxsp-0.0.5/dxsp.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2883 2023-04-09 12:06:54.000000 dxsp-0.0.5/dxsp.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-04-09 12:06:54.000000 dxsp-0.0.5/dxsp.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-09 12:06:54.000000 dxsp-0.0.5/dxsp.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-09 12:06:54.000000 dxsp-0.0.5/dxsp.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      574 2023-04-09 12:06:24.000000 dxsp-0.0.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-09 12:06:54.499751 dxsp-0.0.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 12:50:43.075862 dxsp-0.0.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-04-09 12:50:33.000000 dxsp-0.0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2883 2023-04-09 12:50:43.075862 dxsp-0.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2396 2023-04-09 12:50:33.000000 dxsp-0.0.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 12:50:43.075862 dxsp-0.0.7/dxsp/
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-09 12:50:33.000000 dxsp-0.0.7/dxsp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10543 2023-04-09 12:50:33.000000 dxsp-0.0.7/dxsp/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3683 2023-04-09 12:50:33.000000 dxsp-0.0.7/dxsp/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 12:50:43.075862 dxsp-0.0.7/dxsp.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2883 2023-04-09 12:50:43.000000 dxsp-0.0.7/dxsp.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-04-09 12:50:43.000000 dxsp-0.0.7/dxsp.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-09 12:50:43.000000 dxsp-0.0.7/dxsp.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-09 12:50:43.000000 dxsp-0.0.7/dxsp.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      560 2023-04-09 12:50:33.000000 dxsp-0.0.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-09 12:50:43.075862 dxsp-0.0.7/setup.cfg
```

### Comparing `dxsp-0.0.5/LICENSE` & `dxsp-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `dxsp-0.0.5/PKG-INFO` & `dxsp-0.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dxsp
-Version: 0.0.5
+Version: 0.0.7
 Summary: DXSP (DeX SwaP), A defi swap helper package. Easy peasy Swap.
 Author: MrAniki
 Project-URL: Homepage, https://github.com/mraniki/dxsp
 Project-URL: Bug Tracker, https://github.com/mraniki/dxsp/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `dxsp-0.0.5/README.md` & `dxsp-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `dxsp-0.0.5/dxsp/main.py` & `dxsp-0.0.7/dxsp/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 import os
 import logging
 from dotenv import load_dotenv
 import json
 import requests
 import asyncio
 from web3 import Web3
+
+from utils import *
 import many_abis as ma
 
 #🧐LOGGING
-LOGLEVEL=os.getenv("LOGLEVEL", "INFO")
+LOGLEVEL=os.getenv("LOGLEVEL", "DEBUG")
 logging.basicConfig(format="%(asctime)s - %(name)s - %(levelname)s - %(message)s", level=LOGLEVEL)
 logger = logging.getLogger(__name__)
 logger.info(msg=f"LOGLEVEL {LOGLEVEL}")
 
 
 class DexSwap:
 
@@ -80,14 +82,19 @@
                 if (keyval['symbol'] == symbol and keyval['chainId'] == self.chain_id):
                     logger.debug(msg=f"keyval {keyval['address']}")
                     return keyval['address']
         except Exception as e:
             logger.debug(msg=f"error {e}")
             return
 
+    async def get_contract(self, symbol):
+        logger.debug(msg=f"self.chain_id {self.chain_id}")
+        return await search_contract(self.chain_id,symbol)
+
+
     async def get_quote(self, token):
             asset_in_address = await self.get_contract_address(token)
             logger.debug(msg=f"asset_in_address {asset_in_address}")
             asset_out_address = await self.get_contract_address('USDC')
             logger.debug(msg=f"asset_out_address {asset_out_address}")
             try:
                 asset_out_amount=1000000000000
```

### Comparing `dxsp-0.0.5/dxsp.egg-info/PKG-INFO` & `dxsp-0.0.7/dxsp.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dxsp
-Version: 0.0.5
+Version: 0.0.7
 Summary: DXSP (DeX SwaP), A defi swap helper package. Easy peasy Swap.
 Author: MrAniki
 Project-URL: Homepage, https://github.com/mraniki/dxsp
 Project-URL: Bug Tracker, https://github.com/mraniki/dxsp/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `dxsp-0.0.5/pyproject.toml` & `dxsp-0.0.7/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
-requires = ["setuptools>=61.0","web3>=6.1.0"]
+requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "dxsp"
-version = "0.0.5"
+version = "0.0.7"
 authors = [
   { name="MrAniki" },
 ]
 description = "DXSP (DeX SwaP), A defi swap helper package. Easy peasy Swap."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

