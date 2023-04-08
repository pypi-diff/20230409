# Comparing `tmp/dxsp-0.0.2.tar.gz` & `tmp/dxsp-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dxsp-0.0.2.tar", last modified: Sat Apr  8 21:17:02 2023, max compression
+gzip compressed data, was "dxsp-0.0.3.tar", last modified: Sat Apr  8 22:07:52 2023, max compression
```

## Comparing `dxsp-0.0.2.tar` & `dxsp-0.0.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 21:17:02.570829 dxsp-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-04-08 21:16:49.000000 dxsp-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2899 2023-04-08 21:17:02.570829 dxsp-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2412 2023-04-08 21:16:49.000000 dxsp-0.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 21:17:02.566829 dxsp-0.0.2/dxsp/
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-08 21:16:49.000000 dxsp-0.0.2/dxsp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7512 2023-04-08 21:16:49.000000 dxsp-0.0.2/dxsp/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 21:17:02.570829 dxsp-0.0.2/dxsp.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2899 2023-04-08 21:17:02.000000 dxsp-0.0.2/dxsp.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-04-08 21:17:02.000000 dxsp-0.0.2/dxsp.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-08 21:17:02.000000 dxsp-0.0.2/dxsp.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-08 21:17:02.000000 dxsp-0.0.2/dxsp.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      560 2023-04-08 21:16:49.000000 dxsp-0.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-08 21:17:02.570829 dxsp-0.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 22:07:52.062800 dxsp-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-04-08 22:07:37.000000 dxsp-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2893 2023-04-08 22:07:52.058800 dxsp-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2406 2023-04-08 22:07:37.000000 dxsp-0.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 22:07:52.058800 dxsp-0.0.3/dxsp/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-08 22:07:37.000000 dxsp-0.0.3/dxsp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7512 2023-04-08 22:07:37.000000 dxsp-0.0.3/dxsp/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 22:07:52.058800 dxsp-0.0.3/dxsp.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2893 2023-04-08 22:07:52.000000 dxsp-0.0.3/dxsp.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-04-08 22:07:52.000000 dxsp-0.0.3/dxsp.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-08 22:07:52.000000 dxsp-0.0.3/dxsp.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-08 22:07:52.000000 dxsp-0.0.3/dxsp.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      560 2023-04-08 22:07:37.000000 dxsp-0.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-08 22:07:52.062800 dxsp-0.0.3/setup.cfg
```

### Comparing `dxsp-0.0.2/LICENSE` & `dxsp-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `dxsp-0.0.2/PKG-INFO` & `dxsp-0.0.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: dxsp
-Version: 0.0.2
+Version: 0.0.3
 Summary: DXSP (DeX SwaP), A defi swap helper package. Easy peasy Swap.
 Author: MrAniki
 Project-URL: Homepage, https://github.com/mraniki/dxsp
 Project-URL: Bug Tracker, https://github.com/mraniki/dxsp/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# swapportunity
+# dxsp
 DXSP (DeX SwaP), A defi swap helper package. 
 Easy peasy Swap.
 
 ![Pypi](https://img.shields.io/pypi/dm/dxsp)
 
 # Install
 `pip install dxsp`
@@ -60,37 +60,37 @@
 w3 = Web3(Web3.HTTPProvider(network_provider_url))
 
 
 
 + from dxsp import DexSwap
 
 async def main():
-	#SWAP HELPER
-	+ dex = DexSwap(w3,chain_id,wallet_address,private_key,execution_mode,dex_exchange,block_explorer_api)
+	#SWAP HELPER 
++	dex = DexSwap(w3,chain_id,wallet_address,private_key,execution_mode,dex_exchange,block_explorer_api)
 
 
 	#get Contract Address
-	bitcoinaddress = await dex.get_contract_address('wBTC')
++	bitcoinaddress = await dex.get_contract_address('wBTC')
 	print("bitcoinaddress ", bitcoinaddress)
 
 	#getABI
-	bitcoinABI = await dex.get_abi(bitcoinaddress)
++	bitcoinABI = await dex.get_abi(bitcoinaddress)
 	print("bitcoinABI ", bitcoinABI)
 
 	#INPUT for QUOTE
-	quote = await dex.get_quote('wBTC')
++	quote = await dex.get_quote('wBTC')
 	print("quote ", quote)
 
 	#INPUT for a NORMAL SWAP
 	# transaction_amount_out = 10
 	# asset_out_symbol = "USDT"
 	# asset_in_symbol = "ETH"
 
 	#SWAP EXECUTION
-	+# transaction = dex.get_swap(transaction_amount_out,asset_out_symbol,asset_in_symbol)
++	# transaction = dex.get_swap(transaction_amount_out,asset_out_symbol,asset_in_symbol)
 	# print("transaction ", transaction)
 
 
 if __name__ == "__main__":
     asyncio.run(main())
 ```
```

### Comparing `dxsp-0.0.2/README.md` & `dxsp-0.0.3/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# swapportunity
+# dxsp
 DXSP (DeX SwaP), A defi swap helper package. 
 Easy peasy Swap.
 
 ![Pypi](https://img.shields.io/pypi/dm/dxsp)
 
 # Install
 `pip install dxsp`
@@ -46,37 +46,37 @@
 w3 = Web3(Web3.HTTPProvider(network_provider_url))
 
 
 
 + from dxsp import DexSwap
 
 async def main():
-	#SWAP HELPER
-	+ dex = DexSwap(w3,chain_id,wallet_address,private_key,execution_mode,dex_exchange,block_explorer_api)
+	#SWAP HELPER 
++	dex = DexSwap(w3,chain_id,wallet_address,private_key,execution_mode,dex_exchange,block_explorer_api)
 
 
 	#get Contract Address
-	bitcoinaddress = await dex.get_contract_address('wBTC')
++	bitcoinaddress = await dex.get_contract_address('wBTC')
 	print("bitcoinaddress ", bitcoinaddress)
 
 	#getABI
-	bitcoinABI = await dex.get_abi(bitcoinaddress)
++	bitcoinABI = await dex.get_abi(bitcoinaddress)
 	print("bitcoinABI ", bitcoinABI)
 
 	#INPUT for QUOTE
-	quote = await dex.get_quote('wBTC')
++	quote = await dex.get_quote('wBTC')
 	print("quote ", quote)
 
 	#INPUT for a NORMAL SWAP
 	# transaction_amount_out = 10
 	# asset_out_symbol = "USDT"
 	# asset_in_symbol = "ETH"
 
 	#SWAP EXECUTION
-	+# transaction = dex.get_swap(transaction_amount_out,asset_out_symbol,asset_in_symbol)
++	# transaction = dex.get_swap(transaction_amount_out,asset_out_symbol,asset_in_symbol)
 	# print("transaction ", transaction)
 
 
 if __name__ == "__main__":
     asyncio.run(main())
 ```
```

### Comparing `dxsp-0.0.2/dxsp/main.py` & `dxsp-0.0.3/dxsp/main.py`

 * *Files identical despite different names*

### Comparing `dxsp-0.0.2/dxsp.egg-info/PKG-INFO` & `dxsp-0.0.3/dxsp.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: dxsp
-Version: 0.0.2
+Version: 0.0.3
 Summary: DXSP (DeX SwaP), A defi swap helper package. Easy peasy Swap.
 Author: MrAniki
 Project-URL: Homepage, https://github.com/mraniki/dxsp
 Project-URL: Bug Tracker, https://github.com/mraniki/dxsp/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# swapportunity
+# dxsp
 DXSP (DeX SwaP), A defi swap helper package. 
 Easy peasy Swap.
 
 ![Pypi](https://img.shields.io/pypi/dm/dxsp)
 
 # Install
 `pip install dxsp`
@@ -60,37 +60,37 @@
 w3 = Web3(Web3.HTTPProvider(network_provider_url))
 
 
 
 + from dxsp import DexSwap
 
 async def main():
-	#SWAP HELPER
-	+ dex = DexSwap(w3,chain_id,wallet_address,private_key,execution_mode,dex_exchange,block_explorer_api)
+	#SWAP HELPER 
++	dex = DexSwap(w3,chain_id,wallet_address,private_key,execution_mode,dex_exchange,block_explorer_api)
 
 
 	#get Contract Address
-	bitcoinaddress = await dex.get_contract_address('wBTC')
++	bitcoinaddress = await dex.get_contract_address('wBTC')
 	print("bitcoinaddress ", bitcoinaddress)
 
 	#getABI
-	bitcoinABI = await dex.get_abi(bitcoinaddress)
++	bitcoinABI = await dex.get_abi(bitcoinaddress)
 	print("bitcoinABI ", bitcoinABI)
 
 	#INPUT for QUOTE
-	quote = await dex.get_quote('wBTC')
++	quote = await dex.get_quote('wBTC')
 	print("quote ", quote)
 
 	#INPUT for a NORMAL SWAP
 	# transaction_amount_out = 10
 	# asset_out_symbol = "USDT"
 	# asset_in_symbol = "ETH"
 
 	#SWAP EXECUTION
-	+# transaction = dex.get_swap(transaction_amount_out,asset_out_symbol,asset_in_symbol)
++	# transaction = dex.get_swap(transaction_amount_out,asset_out_symbol,asset_in_symbol)
 	# print("transaction ", transaction)
 
 
 if __name__ == "__main__":
     asyncio.run(main())
 ```
```

### Comparing `dxsp-0.0.2/pyproject.toml` & `dxsp-0.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "dxsp"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
   { name="MrAniki" },
 ]
 description = "DXSP (DeX SwaP), A defi swap helper package. Easy peasy Swap."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

