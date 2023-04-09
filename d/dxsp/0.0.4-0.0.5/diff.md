# Comparing `tmp/dxsp-0.0.4.tar.gz` & `tmp/dxsp-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dxsp-0.0.4.tar", last modified: Sun Apr  9 11:59:20 2023, max compression
+gzip compressed data, was "dxsp-0.0.5.tar", last modified: Sun Apr  9 12:06:54 2023, max compression
```

## Comparing `dxsp-0.0.4.tar` & `dxsp-0.0.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 11:59:20.889033 dxsp-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-04-09 11:58:56.000000 dxsp-0.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2883 2023-04-09 11:59:20.889033 dxsp-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2396 2023-04-09 11:58:56.000000 dxsp-0.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 11:59:20.889033 dxsp-0.0.4/dxsp/
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-09 11:58:56.000000 dxsp-0.0.4/dxsp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10257 2023-04-09 11:58:56.000000 dxsp-0.0.4/dxsp/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 11:59:20.889033 dxsp-0.0.4/dxsp.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2883 2023-04-09 11:59:20.000000 dxsp-0.0.4/dxsp.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-04-09 11:59:20.000000 dxsp-0.0.4/dxsp.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-09 11:59:20.000000 dxsp-0.0.4/dxsp.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-09 11:59:20.000000 dxsp-0.0.4/dxsp.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      574 2023-04-09 11:58:56.000000 dxsp-0.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-09 11:59:20.889033 dxsp-0.0.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 12:06:54.499751 dxsp-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-04-09 12:06:24.000000 dxsp-0.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2883 2023-04-09 12:06:54.499751 dxsp-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2396 2023-04-09 12:06:24.000000 dxsp-0.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 12:06:54.495751 dxsp-0.0.5/dxsp/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-09 12:06:24.000000 dxsp-0.0.5/dxsp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10359 2023-04-09 12:06:24.000000 dxsp-0.0.5/dxsp/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 12:06:54.495751 dxsp-0.0.5/dxsp.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2883 2023-04-09 12:06:54.000000 dxsp-0.0.5/dxsp.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-04-09 12:06:54.000000 dxsp-0.0.5/dxsp.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-09 12:06:54.000000 dxsp-0.0.5/dxsp.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-09 12:06:54.000000 dxsp-0.0.5/dxsp.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      574 2023-04-09 12:06:24.000000 dxsp-0.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-09 12:06:54.499751 dxsp-0.0.5/setup.cfg
```

### Comparing `dxsp-0.0.4/LICENSE` & `dxsp-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `dxsp-0.0.4/PKG-INFO` & `dxsp-0.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dxsp
-Version: 0.0.4
+Version: 0.0.5
 Summary: DXSP (DeX SwaP), A defi swap helper package. Easy peasy Swap.
 Author: MrAniki
 Project-URL: Homepage, https://github.com/mraniki/dxsp
 Project-URL: Bug Tracker, https://github.com/mraniki/dxsp/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `dxsp-0.0.4/README.md` & `dxsp-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `dxsp-0.0.4/dxsp/main.py` & `dxsp-0.0.5/dxsp/main.py`

 * *Files 6% similar despite different names*

```diff
@@ -129,49 +129,49 @@
             approval_check_URL = f"{self.dex_url}/approve/allowance?tokenAddress={asset_out_address}&walletAddress={self.wallet_address}"
             approval_response =  self._get(approval_check_URL)
             approval_check = approval_response['allowance']
             if (approval_check==0):
                 approval_URL = f"{self.dex_url}/approve/transaction?tokenAddress={asset_out_address}"
                 approval_response =  self._get(approval_URL)
         # if execution_mode in ["2", "4"]:
-        #     approval_check = asset_out_contract.functions.allowance(ex.to_checksum_address(walletaddress), ex.to_checksum_address(router)).call()
+        #     approval_check = asset_out_contract.functions.allowance(ex.to_checksum_address(self.wallet_address), ex.to_checksum_address(router)).call()
         #     logger.debug(msg=f"approval_check {approval_check}")
         #     if (approval_check==0):
         #         approved_amount = (ex.to_wei(2**64-1,'ether'))
         #         asset_out_abi = await fetch_abi_dex(asset_out_address)
         #         asset_out_contract = ex.eth.contract(address=asset_out_address, abi=asset_out_abi)
         #         approval_TX = asset_out_contract.functions.approve(ex.to_checksum_address(router), approved_amount)
         #         approval_txHash = await sign_transaction_dex(approval_TX)
         #         approval_txHash_complete = ex.eth.wait_for_transaction_receipt(approval_txHash, timeout=120, poll_latency=0.1)
 
-    async def get_sign(tx)
+    async def get_sign(tx):
         try:
             if execution_mode in ['2']:
                 tx_params = {
                 'from': self.wallet_address,
-                'gas': await self.get_gas(tx)
-                'gasPrice': await self.get_gasPrice(tx)
-                'nonce': self.w3.eth.get_transaction_count(walletaddress),
+                'gas': await self.get_gas(tx),
+                'gasPrice': await self.get_gasPrice(tx),
+                'nonce': self.w3.eth.get_transaction_count(self.wallet_address),
                 }
                 tx = tx.build_transaction(tx_params)
             if dex_version in ['4']:
                 tx_params = {
                 'from': self.wallet_address,
                 'gas': await estimate_gas(tx),
                 'gasPrice': self.w3.to_wei(gasPrice,'gwei'),
-                'nonce': self.w3.eth.get_transaction_count(walletaddress),
+                'nonce': self.w3.eth.get_transaction_count(self.wallet_address),
                 }
                 tx = tx.build_transaction(tx_params)
             elif dex_version == 1:
                 tx = tx['tx']
                 tx['gas'] = await estimate_gas(tx)
-                tx['nonce'] = self.w3.eth.get_transaction_count(walletaddress)
+                tx['nonce'] = self.w3.eth.get_transaction_count(self.wallet_address)
                 tx['value'] = int(tx['value'])
                 tx['gasPrice'] = int(ex.to_wei(gasPrice,'gwei'))
-            signed = self.w3.eth.account.sign_transaction(tx, privatekey)
+            signed = self.w3.eth.account.sign_transaction(tx, self.private_key)
             raw_tx = signed.rawTransaction
             return self.w3.eth.send_raw_transaction(raw_tx)
         except Exception as e:
             logger.debug(msg=f"sign_transaction_dex contract {tx} error {e}")
             await handle_exception(e)
             return
 
@@ -185,24 +185,25 @@
         logger.debug(msg=f"gasprice {gasprice}")
         return self.w3.to_wei(gasPrice,'gwei')
 
     async def get_swap(self, 
             fromTokenAddress: str, 
             toTokenAddress: str,
             amount: float, 
-            fromAddress=self.wallet_address,
+            fromAddress=0xEeeeeEeeeEeEeeEeEeEeeEEEeeeeEeeeeeeeEEeE,
             slippage=2, 
             decimal=18, 
         ):
         try:
             asset_out_address = await self.get_contract_address(fromTokenAddress)
             logger.debug(msg=f"asset_out_address {asset_out_address}")
             asset_in_address = await self.get_contract_address(toTokenAddress)
             logger.debug(msg=f"asset_in_address {asset_in_address}")
             transaction_amount = amount
+            fromAddress = self.wallet_address
             await self.get_approve(asset_out_address,asset_out_contract)
             swap_url = f"{url}/swap?fromTokenAddress={asset_out_address}&toTokenAddress={asset_in_address}&amount={transaction_amount}&fromAddress={send_address}&slippage={slippage}"
             swap_TX = self.get(swap_url)
             signed_TX = await self.get_sign(swap_TX)
             txHash = str(self.w3.to_hex(signed_TX))
             logger.debug(msg=f"txHash {txHash}")
             txResult = await self.get_block_explorer_status(txHash)
```

### Comparing `dxsp-0.0.4/dxsp.egg-info/PKG-INFO` & `dxsp-0.0.5/dxsp.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dxsp
-Version: 0.0.4
+Version: 0.0.5
 Summary: DXSP (DeX SwaP), A defi swap helper package. Easy peasy Swap.
 Author: MrAniki
 Project-URL: Homepage, https://github.com/mraniki/dxsp
 Project-URL: Bug Tracker, https://github.com/mraniki/dxsp/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `dxsp-0.0.4/pyproject.toml` & `dxsp-0.0.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0","web3>=6.1.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "dxsp"
-version = "0.0.4"
+version = "0.0.5"
 authors = [
   { name="MrAniki" },
 ]
 description = "DXSP (DeX SwaP), A defi swap helper package. Easy peasy Swap."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

