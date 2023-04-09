# Comparing `tmp/qfinuwa-1.1.4.2.tar.gz` & `tmp/qfinuwa-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qfinuwa-1.1.4.2.tar", last modified: Thu Mar 30 18:44:07 2023, max compression
+gzip compressed data, was "qfinuwa-1.1.5.tar", last modified: Sun Apr  9 05:19:46 2023, max compression
```

## Comparing `qfinuwa-1.1.4.2.tar` & `qfinuwa-1.1.5.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 18:44:07.701530 qfinuwa-1.1.4.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-03-30 18:43:56.000000 qfinuwa-1.1.4.2/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     8152 2023-03-30 18:44:07.701530 qfinuwa-1.1.4.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6457 2023-03-30 18:43:56.000000 qfinuwa-1.1.4.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-03-30 18:43:56.000000 qfinuwa-1.1.4.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      742 2023-03-30 18:44:07.701530 qfinuwa-1.1.4.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      349 2023-03-30 18:43:56.000000 qfinuwa-1.1.4.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 18:44:07.697530 qfinuwa-1.1.4.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 18:44:07.701530 qfinuwa-1.1.4.2/src/qfinuwa/
--rw-r--r--   0 runner    (1001) docker     (123)     7982 2023-03-30 18:43:56.000000 qfinuwa-1.1.4.2/src/qfinuwa/API.py
--rw-r--r--   0 runner    (1001) docker     (123)      329 2023-03-30 18:43:56.000000 qfinuwa-1.1.4.2/src/qfinuwa/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13480 2023-03-30 18:43:56.000000 qfinuwa-1.1.4.2/src/qfinuwa/backtester.py
--rw-r--r--   0 runner    (1001) docker     (123)    13706 2023-03-30 18:43:56.000000 qfinuwa-1.1.4.2/src/qfinuwa/indicators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 18:44:07.701530 qfinuwa-1.1.4.2/src/qfinuwa/opt/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-03-30 18:43:56.000000 qfinuwa-1.1.4.2/src/qfinuwa/opt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8629 2023-03-30 18:43:56.000000 qfinuwa-1.1.4.2/src/qfinuwa/opt/_portfolio.py
--rw-r--r--   0 runner    (1001) docker     (123)     6254 2023-03-30 18:43:56.000000 qfinuwa-1.1.4.2/src/qfinuwa/opt/_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     3120 2023-03-30 18:43:56.000000 qfinuwa-1.1.4.2/src/qfinuwa/opt/_stockdata.py
--rw-r--r--   0 runner    (1001) docker     (123)     5410 2023-03-30 18:43:56.000000 qfinuwa-1.1.4.2/src/qfinuwa/plotting.py
--rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-03-30 18:43:56.000000 qfinuwa-1.1.4.2/src/qfinuwa/strategy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 18:44:07.701530 qfinuwa-1.1.4.2/src/qfinuwa.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8152 2023-03-30 18:44:07.000000 qfinuwa-1.1.4.2/src/qfinuwa.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      487 2023-03-30 18:44:07.000000 qfinuwa-1.1.4.2/src/qfinuwa.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-30 18:44:07.000000 qfinuwa-1.1.4.2/src/qfinuwa.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-03-30 18:44:07.000000 qfinuwa-1.1.4.2/src/qfinuwa.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-03-30 18:44:07.000000 qfinuwa-1.1.4.2/src/qfinuwa.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 05:19:46.025214 qfinuwa-1.1.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-04-09 05:19:31.000000 qfinuwa-1.1.5/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     8227 2023-04-09 05:19:46.025214 qfinuwa-1.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6534 2023-04-09 05:19:31.000000 qfinuwa-1.1.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-04-09 05:19:31.000000 qfinuwa-1.1.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      740 2023-04-09 05:19:46.025214 qfinuwa-1.1.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-04-09 05:19:31.000000 qfinuwa-1.1.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 05:19:46.021214 qfinuwa-1.1.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 05:19:46.025214 qfinuwa-1.1.5/src/qfinuwa/
+-rw-r--r--   0 runner    (1001) docker     (123)     8870 2023-04-09 05:19:31.000000 qfinuwa-1.1.5/src/qfinuwa/API.py
+-rw-r--r--   0 runner    (1001) docker     (123)      329 2023-04-09 05:19:31.000000 qfinuwa-1.1.5/src/qfinuwa/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17211 2023-04-09 05:19:31.000000 qfinuwa-1.1.5/src/qfinuwa/backtester.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13962 2023-04-09 05:19:31.000000 qfinuwa-1.1.5/src/qfinuwa/indicators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 05:19:46.025214 qfinuwa-1.1.5/src/qfinuwa/opt/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-09 05:19:31.000000 qfinuwa-1.1.5/src/qfinuwa/opt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2315 2023-04-09 05:19:31.000000 qfinuwa-1.1.5/src/qfinuwa/opt/_portfolio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5866 2023-04-09 05:19:31.000000 qfinuwa-1.1.5/src/qfinuwa/opt/_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3168 2023-04-09 05:19:31.000000 qfinuwa-1.1.5/src/qfinuwa/opt/_stockdata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5290 2023-04-09 05:19:31.000000 qfinuwa-1.1.5/src/qfinuwa/plotting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-04-09 05:19:31.000000 qfinuwa-1.1.5/src/qfinuwa/strategy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 05:19:46.025214 qfinuwa-1.1.5/src/qfinuwa.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8227 2023-04-09 05:19:46.000000 qfinuwa-1.1.5/src/qfinuwa.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-04-09 05:19:46.000000 qfinuwa-1.1.5/src/qfinuwa.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-09 05:19:46.000000 qfinuwa-1.1.5/src/qfinuwa.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-04-09 05:19:46.000000 qfinuwa-1.1.5/src/qfinuwa.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-09 05:19:46.000000 qfinuwa-1.1.5/src/qfinuwa.egg-info/top_level.txt
```

### Comparing `qfinuwa-1.1.4.2/LICENSE.txt` & `qfinuwa-1.1.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `qfinuwa-1.1.4.2/PKG-INFO` & `qfinuwa-1.1.5/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qfinuwa
-Version: 1.1.4.2
+Version: 1.1.5
 Summary: Framework for backtesting quantitative trading algorithims.
 Home-page: https://github.com/QFinUWA/algo-backtester/issues
 Author: Isaac Bergl
 Author-email: tberg644@gmail.com
 Project-URL: Bug Tracker, https://github.com/QFinUWA/algo-backtester/issues
 Project-URL: repository, https://github.com/QFinUWA/algo-backtester
 Classifier: Programming Language :: Python :: 3
@@ -33,24 +33,14 @@
 
 path_to_API = 'API_key.txt'
 download_folder = './data'
 
 API.fetch_stocks(['AAPL', 'GOOG', 'TSLA'], path_to_API, download_folder)
 ```
 
-To pull prepepared data from QFin's googledrive, call ``API.from_google_drive``:
-
-```py
-
-file_ids = 'file_ids.txt'
-download_folder = './data'
-
-API.from_google_drive(file_ids, download_folder)
-```
-
 ## Indicator Class
 
 #### Multi-Indicators
 
 A multi-indicator takes in a single signal (price of an arbitary stock) and outputs a transformation of that stock.
 
 It is called ``MultiIndicator`` because the indicator will have multiple values (one for each stock)
@@ -150,29 +140,37 @@
 
 Similar to ``qfin.Indicators``, you can define hyperparameters for your model in ``__init__``.
 
 ```py
 # Example Strategy
 class BasicBollinger(Strategy):
 
-    def __init__(self, quantity=1):
+    def __init__(self, quantity=5):
         self.quantity = quantity
-        return
-
+        self.n_failed_orders = 0
+    
     def on_data(self, prices, indicators, portfolio):
-        
+
         # If current price is below lower Bollinger Band, enter a long position
-        if(prices['close']['AAPL'][-1] < indicators['lower_bollinger']['AAPL'][-1]):
-            portfolio.cover_short('AAPL', quantity=self.quantity)
-            portfolio.enter_long('AAPL', quantity=self.quantity)
-
-        # If current price is above upper Bollinger Band, enter a long position   
-        if(prices['close']['AAPL'][-1] > indicators['upper_bollinger']['AAPL'][-1]):
-            portfolio.sell_long('AAPL', quantity=self.quantity)
-            portfolio.enter_short('AAPL', quantity=self.quantity)
+        for stock in portfolio.stocks:
+
+            if(prices['close'][stock][-1] < indicators['lower_bollinger'][stock][-1]):
+                order_success = portfolio.order(stock, quantity=self.quantity)
+                if not order_success:
+                    self.n_failed_orders += 1
+            
+            # If current price is above upper Bollinger Band, enter a short position
+            if(prices['close'][stock][-1] > indicators['upper_bollinger'][stock][-1]):
+                order_success = portfolio.order(stock, quantity=-self.quantity)
+                if not order_success:
+                    self.n_failed_orders += 1
+
+    def on_finish(self):
+        # Added to results object - access using result.on_finish
+        return self.n_failed_orders
 ```
 Additionally, you can specify a function ``on_finish`` that will run on the completion of a run, if you want to save your own data. Whatever this function returns will can be accessed in the results (see ``SingleRunResults.on_finish``).
 ## Backtester Class
 
 The ``Backtester`` class asks for a custom strategy, custom indicators and data from the user. Once created, it can run multiple backtests without having to recalculate the indicators - when used in a Notebook environment the backtester object can persist and incrementally updated with new values.
 
 ### Creating a Backtester
@@ -181,15 +179,15 @@
 
 
 ```py
 from qfinuwa import Backtester
 
 backtester = Backtester(CustomStrategy, CustomIndicators, 
                         data=r'\data', days=90, 
-                        cash=1000, fee=0.01)
+                        delta_limits=1000, fee=0.01)
 ```
 
 ## Updating Indicator Parameters
 
 ### Update Parameters
 
 ```py
```

### Comparing `qfinuwa-1.1.4.2/README.md` & `qfinuwa-1.1.5/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -17,24 +17,14 @@
 
 path_to_API = 'API_key.txt'
 download_folder = './data'
 
 API.fetch_stocks(['AAPL', 'GOOG', 'TSLA'], path_to_API, download_folder)
 ```
 
-To pull prepepared data from QFin's googledrive, call ``API.from_google_drive``:
-
-```py
-
-file_ids = 'file_ids.txt'
-download_folder = './data'
-
-API.from_google_drive(file_ids, download_folder)
-```
-
 ## Indicator Class
 
 #### Multi-Indicators
 
 A multi-indicator takes in a single signal (price of an arbitary stock) and outputs a transformation of that stock.
 
 It is called ``MultiIndicator`` because the indicator will have multiple values (one for each stock)
@@ -134,29 +124,37 @@
 
 Similar to ``qfin.Indicators``, you can define hyperparameters for your model in ``__init__``.
 
 ```py
 # Example Strategy
 class BasicBollinger(Strategy):
 
-    def __init__(self, quantity=1):
+    def __init__(self, quantity=5):
         self.quantity = quantity
-        return
-
+        self.n_failed_orders = 0
+    
     def on_data(self, prices, indicators, portfolio):
-        
+
         # If current price is below lower Bollinger Band, enter a long position
-        if(prices['close']['AAPL'][-1] < indicators['lower_bollinger']['AAPL'][-1]):
-            portfolio.cover_short('AAPL', quantity=self.quantity)
-            portfolio.enter_long('AAPL', quantity=self.quantity)
-
-        # If current price is above upper Bollinger Band, enter a long position   
-        if(prices['close']['AAPL'][-1] > indicators['upper_bollinger']['AAPL'][-1]):
-            portfolio.sell_long('AAPL', quantity=self.quantity)
-            portfolio.enter_short('AAPL', quantity=self.quantity)
+        for stock in portfolio.stocks:
+
+            if(prices['close'][stock][-1] < indicators['lower_bollinger'][stock][-1]):
+                order_success = portfolio.order(stock, quantity=self.quantity)
+                if not order_success:
+                    self.n_failed_orders += 1
+            
+            # If current price is above upper Bollinger Band, enter a short position
+            if(prices['close'][stock][-1] > indicators['upper_bollinger'][stock][-1]):
+                order_success = portfolio.order(stock, quantity=-self.quantity)
+                if not order_success:
+                    self.n_failed_orders += 1
+
+    def on_finish(self):
+        # Added to results object - access using result.on_finish
+        return self.n_failed_orders
 ```
 Additionally, you can specify a function ``on_finish`` that will run on the completion of a run, if you want to save your own data. Whatever this function returns will can be accessed in the results (see ``SingleRunResults.on_finish``).
 ## Backtester Class
 
 The ``Backtester`` class asks for a custom strategy, custom indicators and data from the user. Once created, it can run multiple backtests without having to recalculate the indicators - when used in a Notebook environment the backtester object can persist and incrementally updated with new values.
 
 ### Creating a Backtester
@@ -165,15 +163,15 @@
 
 
 ```py
 from qfinuwa import Backtester
 
 backtester = Backtester(CustomStrategy, CustomIndicators, 
                         data=r'\data', days=90, 
-                        cash=1000, fee=0.01)
+                        delta_limits=1000, fee=0.01)
 ```
 
 ## Updating Indicator Parameters
 
 ### Update Parameters
 
 ```py
```

### Comparing `qfinuwa-1.1.4.2/setup.cfg` & `qfinuwa-1.1.5/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = QFinUWA
-version = 1.1.4.2
+version = 1.1.5
 author = Isaac Bergl
 author_email = tberg644@gmail.com
 description = A backtesting framework for quantitative finance for QFIN UWA.
 long_description = file: README.md, LICENSE.txt
 long_description_content_type = text/markdown
 url = https://github.com/QFinUWA/algo-backtester/issues
 project_urls =
```

### Comparing `qfinuwa-1.1.4.2/src/qfinuwa/API.py` & `qfinuwa-1.1.5/src/qfinuwa/API.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import pandas as pd
 import urllib.parse as urlparse
 from itertools import product
 from multiprocessing.pool import ThreadPool
 from multiprocessing import cpu_count
 import requests
 import zipfile
+from functools import reduce
 import io
 from typing import Union
 import time
 # from IPython import get_ipython
 # try:
 #     shell = get_ipython().__class__.__name__
 #     if shell in ['ZMQInteractiveShell']:
@@ -46,22 +47,22 @@
                 file_ids = [k.strip('\n') for k in f.readlines()]
 
         with ThreadPool() as p:
             p.starmap(cls._download_file_from_google_drive, [(fileid, data_folder) for fileid in file_ids])
     
 
     @classmethod
-    def fetch_stocks(cls, stocks: Union[str,  list], api_key_path: str, data_folder: str) -> None:
+    def fetch_stocks(cls, stocks: Union[str,  list], api_key_path: str, data_folder: str, download_raw: bool = False) -> None:
         '''
         Fetches the data from the SIP market-aggregated data. The data is provided by the SEC. An API key is required. The data is stored in the folder specified by `data_folder`.
 
         ### Parameters
         - ``stocks`` (``str``): The ticker(s) of the stock(s) to be downloaded. If multiple stocks are required, a list of tickers can be provided.
         - ``api_key_path`` (``str``): The path to the file containing the API key.
-
+        - ``download_raw`` (``bool``): If ``true``, downloads the data straight from the API provider, without alligning.
         ### Returns
         ``None``
         '''
     
         if not os.path.exists(api_key_path):
             raise ValueError(f'{api_key_path} does not exist.')
 
@@ -70,15 +71,15 @@
 
         if not os.path.exists(data_folder):
             os.mkdir(data_folder)
 
         if isinstance(stocks, str):
             stocks = [stocks]
         
-        stocks.insert(0, 'SPY')
+        # stocks.insert(0, 'SPY')
 
         stock_df = []
 
         years = [2,1]
         months = range(12,0,-1)
         
         with tqdm(stocks) as pbar:
@@ -93,73 +94,80 @@
 
                 path = os.path.join(data_folder, f"{stock}.csv")
                 if not os.path.exists(path):
                     t_last = time.time()
                     with ThreadPool(n_threads) as p:
                         results = p.map(cls._process_request, urls)
                     # pbar.set_description(f'> Processing {stock}')
+                    if any(map(lambda df: len(df) ==0, results)):
+                        raise RuntimeError('Empty dataframe...')
                     df = pd.concat(results, axis=0, ignore_index=True)
                     df['time'] = pd.to_datetime(df['time'])
                     df = df.set_index('time')
                     df.sort_values(
                         by='time', inplace=True)
                     
                     pbar.set_description(f'> Saving {stock} ({len(df)} rows)')
                     # df.to_csv(cls.to_path(stock + '_raw'), index=False)
                     path = os.path.join(data_folder, f"{stock}.csv")
                     stock_df.append((path, df))
                 
                 t_now = time.time()
-                time.sleep( max(0,30 - (t_now-t_last)))
+                time.sleep( max(0,10 - (t_now-t_last)))
                 pbar.set_description('Blocking...')
                 
                 pbar.update(1)
                 pbar.set_description(f'> Done Fetching') # hacky way to set last description but hey it works
-        cls._allign_data(stock_df)
+        
+        if download_raw:
+            for filepath, df in stock_df:
+                df.to_csv(filepath)
+        else:
+            cls._allign_data(stock_df)
 
     #---------------[Private Methods]-----------------# 
-    @classmethod
-    def _download_file_from_google_drive(cls, id: str, data_folder: str) -> None:
-        URL = "https://docs.google.com/uc?export=download"
-        # URL = 'https://drive.google.com/drive/folders/?usp=share_link'
-
-        session = requests.Session()
-
-        response = session.get(URL, params = { 'id' : id }, stream = True)
-
-        def get_confirm_token(response):
-            for key, value in response.cookies.items():
-                if key.startswith('download_warning'):
-                    return value
-
-            return None
-        
-        token = get_confirm_token(response)
-
-        token = None
-        for key, value in response.cookies.items():
-            if key.startswith('download_warning'):
-                token = value
-                break
-
-        if token:
-            params = { 'id' : id, 'confirm' : token }
-            response = session.get(URL, params = params, stream = True)
-        
-        CHUNK_SIZE = 32768
-        try:
-            with io.BytesIO() as f:
-                for chunk in response.iter_content(CHUNK_SIZE):
-                    if chunk: # filter out keep-alive new chunks
-                        f.write(chunk)
-
-                with zipfile.ZipFile(f) as z:
-                    z.extractall(path=data_folder)
-        except:
-            print(f'Error downloading file {id} - skipping')
+    # @classmethod
+    # def _download_file_from_google_drive(cls, id: str, data_folder: str) -> None:
+    #     URL = "https://docs.google.com/uc?export=download"
+    #     # URL = 'https://drive.google.com/drive/folders/?usp=share_link'
+
+    #     session = requests.Session()
+
+    #     response = session.get(URL, params = { 'id' : id }, stream = True)
+
+    #     def get_confirm_token(response):
+    #         for key, value in response.cookies.items():
+    #             if key.startswith('download_warning'):
+    #                 return value
+
+    #         return None
+        
+    #     token = get_confirm_token(response)
+
+    #     token = None
+    #     for key, value in response.cookies.items():
+    #         if key.startswith('download_warning'):
+    #             token = value
+    #             break
+
+    #     if token:
+    #         params = { 'id' : id, 'confirm' : token }
+    #         response = session.get(URL, params = params, stream = True)
+        
+    #     CHUNK_SIZE = 32768
+    #     try:
+    #         with io.BytesIO() as f:
+    #             for chunk in response.iter_content(CHUNK_SIZE):
+    #                 if chunk: # filter out keep-alive new chunks
+    #                     f.write(chunk)
+                
+    #             # with zipfile.ZipFile(f) as z:
+    #             #     z.extractall(path=data_folder)
+    #     except:
+    #         print(f'Error downloading file {id} - skipping')
 
 
     @classmethod
     def _get_params(cls, stock: str, year: int, month: int, api_key: str) -> str:
 
         params = {
             'function': 'TIME_SERIES_INTRADAY_EXTENDED',
@@ -194,27 +202,34 @@
 
         # go through all stocks and find last start date
         start_date = [df.index.min() for _, df in dfs]
         # first end date
         end_date = [df.index.max() for __, df in dfs]
         # crop dataframes
         start_date, end_date = max(start_date),  min(end_date)
+
         with tqdm(dfs) as pbar:
+
+            new_index = reduce(lambda a,b: a.union(b), (df.index for _, df in dfs))
+
+            new_index = new_index[(new_index >= start_date) & (new_index <= end_date)]
+            new_index = new_index[(new_index.hour + new_index.minute/60 >= 9.5)  & (new_index.hour < 16)]
+
             for filepath, df in dfs:          
                 pbar.set_description(f'> Alligning {filepath}')
 
                 # fill out with averages
-                filled_df = df.resample('T').mean().interpolate(method='time')
-                cropped_df = filled_df.loc[(filled_df.index >= start_date) & (filled_df.index <= end_date)]
+                # filled_df = df.resample('T').mean().interpolate(method='time')
+                # cropped_df = filled_df.loc[(filled_df.index >= start_date) & (filled_df.index <= end_date)]
 
                 # remove any times not in interval (4:00 - 20:00]
-                interval_df = cropped_df.loc[(cropped_df.index.hour >= 4) & (cropped_df.index.hour < 20)]
-                interval_df = interval_df.loc[(interval_df.index.dayofweek != 5) & (interval_df.index.dayofweek != 6)]
-
-                interval_df.to_csv(filepath)
+                # interval_df = cropped_df.loc[(cropped_df.index.hour >= 4) & (cropped_df.index.hour < 20)]
+                # interval_df = interval_df.loc[(interval_df.index.dayofweek != 5) & (interval_df.index.dayofweek != 6)]
+                new_df = df.reindex(new_index, axis=0).interpolate(method='linear')
+                new_df.to_csv(filepath)
 
                 # TODO - download new data
                 pbar.update(1)
                 pbar.set_description(f'> Done Alligning')  # hacky way to set last description but hey it works
         
         return
```

### Comparing `qfinuwa-1.1.4.2/src/qfinuwa/backtester.py` & `qfinuwa-1.1.5/src/qfinuwa/backtester.py`

 * *Files 19% similar despite different names*

```diff
@@ -4,15 +4,17 @@
 from .opt._stockdata import StockData
 import random
 from .opt._result import SingleRunResult, MultiRunResult, ParameterSweepResult
 from .strategy import Strategy
 from .indicators import Indicators
 from typing import Union
 from itertools import islice, tee
-from typing import Union
+import datetime
+from dateutil import parser
+import numpy as np
 
 # from IPython import get_ipython
 # try:
 #     shell = get_ipython().__class__.__name__
 #     if shell in ['ZMQInteractiveShell']:
 #         from tqdm.notebook import tqdm as tqdm   # Jupyter notebook or qtconsole or Terminal running IPython  
 #     else:
@@ -65,30 +67,30 @@
         self._params.update({k:v for k,v in params.items() if k in self.defaults})
 
 
 class Backtester:
 
     def __init__(self,  strategy_class: Strategy, indicator_class: Indicators, 
             stocks: list, 
-            data_folder: str=r'\data', days: Union[int , str] = 'all', 
-            starting_cash: float=1000, fee: float=0.001,
+            data_folder: str, days: Union[int , str] = 'all', 
+            delta_limits:  Union[int , dict]=10000, fee: float=0.0,
             progressbar=True):
         '''
         # Backteser
         A class for running a strategy on historical data. Once initialised, the data is precompiled
         for iterating. The parameters can be updated using the ``update_x`` and ``set_x`` functions.
         The strategy is run on the data by calling the either the ``run`` or ``run_grid_search`` method. 
         
         ## Parameters
         - ``strategy_class`` (``Strategy``): The strategy to run.
         - ``indicator_class`` (``Indicators``): The indicators to use in the strategy.
         - ``stocks`` (``list``): A list of stock to run the strategy on.
         - ``data_folder`` (``str``): The path to the data folder.
         - ``days`` (``int`` or ``str``): The number of days to run the strategy on. 
-        - ``cash`` (``float``): The starting cash balance.
+        - ``delta_limit`` (``int`` or ``dict``): The general delta limit, or a dictionary of delta limits per instrument.
         - ``fee`` (``float``): The fee to pay on each transaction.
         - ``progressbar`` (``bool``): Whether to show a progress bar when loading data.
 
         ## Properties
         - ``strategy_params`` (``dict``): The parameters of the strategy.
         - ``indicator_params`` (``dict``): The parameters of the indicators.
         - ``fee`` (``float``): The fee to pay on each transaction.
@@ -101,15 +103,15 @@
 
         ## Example
         ```python
         from qfinuwa import Backtester
 
         backtester = Backtester(CustomStrategy, CustomIndicators, 
                                 data=r'\data', days=90, 
-                                cash=1000, fee=0.01)
+                                delta_limit=800, fee=0.01)
         ```
 
         '''
         # raise execption if strategy is not a subclass of Strategy
         if not issubclass(strategy_class, Strategy):
             raise ValueError('Strategy must be a subclass of Strategy')  
          
@@ -123,15 +125,26 @@
         if not issubclass(indicator_class, Indicators):
             raise ValueError('Indicators must be a subclass of Indicators')
         
 
         self._indicators = indicator_class(data=self._data)
 
         self._fee = fee
-        self._starting_cash = starting_cash  
+        # self._starting_cash = starting_cash  
+        
+            
+        if isinstance(delta_limits, int):
+            self._delta_limits = {stock: delta_limits for stock in self.stocks}
+        elif isinstance(delta_limits, dict):
+            if set(delta_limits.keys()) ^ set(self.stocks):
+                raise ValueError(f'delta_limit either contains unknown stocks or doesn\'t include all stocks')
+            if not all(map(lambda x: isinstance(int, x) and x > 0, delta_limits.values)):
+                raise ValueError(f'delta_limit includes either non int or negative value')
+        else:
+            self._delta_limits = delta_limits
 
         self._days = days
 
         self._random = random
 
     #---------------[Properties]-----------------#
     @property
@@ -171,23 +184,42 @@
             raise ValueError('days must be an integer or "all"')
         
         if isinstance(days, int) and days < 0:
             raise ValueError('days must be a positive integer or "all"')
         
         self._days = days
     
+    # @property
+    # def starting_cash(self):
+    #     return self._starting_cash
+
+    
+    # @starting_cash.setter
+    # def starting_cash(self, starting_cash):
+    #     if starting_cash < 0:
+    #         raise ValueError('starting_cash must be a positive number')
+    #     self._starting_cash = starting_cash
+
     @property
-    def starting_cash(self):
-        return self._starting_cash
+    def delta_limits(self):
+        return self._delta_limits
     
-    @starting_cash.setter
-    def starting_cash(self, starting_cash):
-        if starting_cash < 0:
-            raise ValueError('starting_cash must be a positive number')
-        self._starting_cash = starting_cash
+    @delta_limits.setter
+    def delta_limits(self, delta_limit):
+
+        if isinstance(delta_limit, dict):
+            if set(delta_limit.keys()) ^ set(self.stocks):
+                raise ValueError(f'delta_limit either contains unknown stocks or doesn\'t include all stocks')
+            if not all(map(lambda x: isinstance(x, int) and x > 0, delta_limit.values())):
+                raise ValueError(f'delta_limit includes either non int or negative value')
+            self._delta_limits = delta_limit
+        elif isinstance(delta_limit, int):
+            self._delta_limits = {stock: delta_limit for stock in self.stocks}
+
+        
     
     @property
     def indicators(self):
         return self._indicators
     
     @indicators.setter
     def indicators(self, indicator_class: Indicators) -> None:
@@ -205,88 +237,107 @@
     @property
     def _strategy(self):
         '''
         For internal use only.
         '''
         return self._strategy_wrapper._strategy
     
+    @property
+    def date_range(self):
+        return self._data.date_range
+    
     #---------------[Public Methods]-----------------#
        
-    def run(self, strategy_params: dict = None, indicator_params: dict = None, progressbar: bool=True, cv: int = 1, seed: int = None) -> MultiRunResult:
+    def run(self, strategy_params: dict = None, indicator_params: dict = None, 
+            cv: int = 1, seed: int = None, start_dates: list = None,
+            progressbar: bool=True) -> MultiRunResult:
         '''
         Runs the strategy on a set of hyperparameters.
 
         ## Parameters
         - ``strategy_params`` (``dict``): The parameters of the strategy.
         - ``indicator_params`` (``dict``): The parameters of the indicators.
-        - ``progressbar`` (``bool``): Whether to show a progress bar.
         - ``cv`` (``int``): The number of cross-validation folds to use.
         - ``seed`` (``int``): The seed to use for the random number generator.
+        - ``start_dates`` (``list``): List of start dates to test on.
+        - ``progressbar`` (``bool``): Whether to show a progress bar.
 
         ## Returns
         result (``MultiRunResult``): The results of the strategy.
         '''
-
         if bool(strategy_params):
             if not isinstance(strategy_params, dict):
                 raise TypeError(f'strategy_params must be of type dict, not {type(strategy_params)}')
 
             # fill in missing parameters with defaults
             alg_defaults = self.strategy.defaults
             alg_defaults.update(strategy_params)
             strategy_params = alg_defaults
         else:
             strategy_params = self.strategy.params
-
         if bool(indicator_params):
             if not isinstance(indicator_params, dict):
                 raise TypeError(f'indicator_params must be of type dict, not {type(indicator_params)}')
             self._indicators._add_parameters(indicator_params)
         else:
             indicator_params = self._indicators.params
 
         self._random.seed(seed or random.randint(0, 2**32))
-        random_periods = self._get_random_periods(cv) 
+        if start_dates is not None:
+            if not isinstance(start_dates, list):
+                raise ValueError('start_dates must be a list')
+            
+            cv = len(start_dates)
+
+            test_periods = self._get_periods(start_dates)
+        else:
+            test_periods = self._get_random_periods(cv) 
         results = []
 
         # caclulate indicators 
-        data_og = zip(*self._precomp_prices, self._indicators._iterate_params(indicator_params))
-        data_tees = tee(data_og, cv)
-        test_iterator = zip(data_tees, random_periods)
-
-        desc = f'> Running backtest over {cv} sample{"s" if cv > 1 else ""} of {self._days} day{"s" if self._days > 1 else ""}'
-        for data, (start, end) in (tqdm(test_iterator, desc = desc, total = cv) if progressbar and cv > 1 else test_iterator):
-            portfolio = Portfolio(self.stocks, self._starting_cash, self._fee)
+        data_tees = tee(self._precomp_prices[0], cv), \
+                    tee(self._precomp_prices[1], cv), \
+                    self._indicators._iterate_params(indicator_params, copies=cv)
+        test_iterator = zip(*data_tees, test_periods)
+
+        days_format = f'{self._days} day{"s" if isinstance(self._days, str) or self._days > 1 else ""}'
+
+        desc = f'> Running backtest over {cv} sample{"s" if cv > 1 else ""} of {days_format}'
+        for *data, (start, end) in (tqdm(test_iterator, desc = desc, total = cv) if progressbar and cv > 1 else test_iterator):
+            
+            portfolio = Portfolio(self.stocks, self._delta_limits, self._fee)
             if strategy_params:
                 strategy = self._strategy(*tuple(), **strategy_params)
             else:
                 strategy = self._strategy(*tuple())
 
-            test = islice(data, start, end) 
+            test = islice(zip(*data), start, end) 
         
             #---------[RUN THE ALGORITHM]---------#
             for test_data in (tqdm(test, desc=desc, total = end-start, mininterval=0.5) if progressbar and cv == 1 else test):
                 strategy.run_on_data(test_data, portfolio)
-            cash, longs, shorts = portfolio.wrap_up()
+            value, trades = portfolio.wrap_up()
             on_finish = strategy.on_finish()
 
-            results.append(SingleRunResult(self.stocks, self._data, self._data.index, (start, end), cash, longs, shorts, on_finish ))
+            results.append(SingleRunResult(self.stocks, self._data, self._data.index, (start, end), value, trades, on_finish ))
             #-------------------------------------#
 
         return MultiRunResult((strategy_params, indicator_params), results)
     
-    def run_grid_search(self, strategy_params: dict = None, indicator_params: dict = None, cv: int = 1, seed: int =None) -> ParameterSweepResult:
+    def run_grid_search(self, strategy_params: dict = None, indicator_params: dict = None, 
+                        cv: int = 1, seed: int =None, start_dates: list = None) -> ParameterSweepResult:
         '''
         Runs a grid search over a set of hyperparameters.
 
         ## Parameters
         - ``strategy_params`` (``dict``): The parameters of the strategy.
         - ``indicator_params`` (``dict``): The parameters of the indicators.
         - ``cv`` (``int``): The number of cross-validation folds to use.
         - ``seed`` (``int``): The seed to use for the random number generator.
+        - ``start_dates`` (``list``): List of start dates to test on.
 
         ## Returns
         result (``ParameterSweepResult``): The results of the strategy.
         '''
         # get all combinations of strategy paramters
         # ----[strategy params]----
         strategy_params = strategy_params or dict()
@@ -300,56 +351,87 @@
         strategy_params_list = [dict(zip(param, v)) for v in product(*val)]
 
         # ----[indicator params]----
         
         indicator_params = indicator_params or dict()
         indicator_params_list = self._indicators._get_permutations(indicator_params)
 
-
         print('> Backtesting the across the following ranges:')
         print('Agorithm Parameters', default_strategy_params)
         print('Indicator Parameters', self._indicators._fill_in_params(indicator_params))
 
         # run
         seed = seed or self._random.randint(0, 2**32)
-        res = []
+                
+        # print('get periods')
+        if start_dates is not None:
+            if not isinstance(start_dates, list):
+                raise ValueError('start_dates must be a list')
+            
+            cv = len(start_dates)
+
+            test_periods = self._get_periods(start_dates)
+        else:
+            # print(cv)
+            test_periods = self._get_random_periods(cv) 
+        total = len(strategy_params_list) * len(indicator_params_list)
+        res = [None for _ in range(total)]
 
-        for alg_params, ind_params in tqdm(product(strategy_params_list, indicator_params_list), total=len(strategy_params_list) * len(indicator_params_list), desc=f"Running paramter sweep (cv={cv})"):
-            res.append(self.run(strategy_params=alg_params, indicator_params=ind_params, cv=cv, seed=seed, progressbar=False))
+        for i, (alg_params, ind_params) in tqdm(enumerate(list(product(strategy_params_list, indicator_params_list))), total=total, desc=f"Running paramter sweep (cv={cv})"):
+            res[i] = self.run(strategy_params=alg_params, indicator_params=ind_params, cv=cv, seed=seed, progressbar=False, start_dates=test_periods)
         
-        return ParameterSweepResult(res)
+        return ParameterSweepResult(res, (default_strategy_params, self._indicators._fill_in_params(indicator_params)))
     
     #---------------[Private Methods]-----------------#
     def _get_random_periods(self, n: int) -> list:
 
         if self._days == 'all':
             return [(0, len(self._data)) for _ in range(n)]
 
         days = self._data.index.dt.to_period('D').drop_duplicates()
     
         s_is = self._random.sample(range(len(days) - self._days), n)
+        
+        starts = [days.iloc[s_i].strftime("%d/%m/%Y") for s_i in s_is]
 
-        starts = (str(days.iloc[s_i]) for s_i in s_is)
+        return self._get_periods(starts)
+    
         ends = (str(days.iloc[s_i+self._days]) for s_i in s_is)
 
         return [(self._data._index[self._data._index >= start].index[0], self._data._index[self._data._index < end].index[-1]) for start, end in zip(starts, ends)]
     
+    def _get_periods(self, start_dates: list) -> list:
+        if all(map(lambda d: isinstance(d[0], np.int64) and isinstance(d[1], np.int64), start_dates)):
+            return start_dates
+
+        d = datetime.timedelta(days = self._days)
+        dt_starts = (parser.parse(s, dayfirst=True) for s in start_dates)
+        # dt_starts = [datetime.datetime(date) for date in parsed]
+
+        # dt_starts = start_dates
+        periods = [(s, s+d) for s in dt_starts]
+        index_start, index_end = self._data.date_range
+        for s,e in periods:
+            if s + datetime.timedelta(days = 1) < index_start or e > index_end:
+                raise IndexError(f'Date range {s} -> {e} out of bounds: Please ensure start_date and (start_date + days) are in range.')
+        return  [(self._data._index[self._data._index >= str(s)].index[0], self._data._index[self._data._index < str(e)].index[-1]) for s, e in periods]
+
 
     #---------------[Internal Methods]-----------------#
     def __str__(self):
         return  f'Backtester:\n' + \
                 f'- Strategy: {self.strategy.name}\n' + \
                 f'\t- Params: {self.strategy.params}\n' + \
                 f'- Indicators: {self._indicators.__class__.__name__}\n' + \
                 f'\t- Params: {self._indicators.params}\n' + \
                 f'\t- SingleIndicators: {self._indicators._singles}\n' \
                 f'\t- MultiIndicators: {self._indicators._multis}\n' \
                 f'- Stocks: {self.stocks}\n' + \
                 f'- Fee {self.fee}\n' + \
-                f'- Starting Balance: {self.starting_cash}\n' + \
+                f'- delta_limit: {self.delta_limits}\n' + \
                 f'- Days: {self._days}\n'
                 # f'\t- Indicator Groups: {self._indicators.groups}\n' + \
     
     def __repr__(self):
         return self.__str__()
```

### Comparing `qfinuwa-1.1.4.2/src/qfinuwa/indicators.py` & `qfinuwa-1.1.5/src/qfinuwa/indicators.py`

 * *Files 4% similar despite different names*

```diff
@@ -297,26 +297,29 @@
                 combinations[indicator].append(perm)
 
         # get every combination of different indicators
         every_combination =  [dict(zip(combinations.keys(), c)) for c in product(*combinations.values())]
 
         return every_combination
 
-    def _iterate_params(self, params=None):
+    def _iterate_params(self, params=None, copies=None):
 
         if params is None:
             params = self.params
 
         params = self._fill_in_params(params)
         self._add_parameters(params)
 
         # params maps function name to parameters
         self._indicators_iterations = {indicator: array(list(self._get_cached(funcn, params[funcn], indicator).values())) for funcn, indicators in self._funcn_to_indicator_map.items() for indicator in indicators}
-
-        return self.__iter__()
+        if copies is None:
+            self.__iter__()
+        # TODO: needlessly recreating iterator - could we just reset iterator related fields
+        #       and iterate again? maybe a modulo type situation?
+        return tuple(self.__iter__() for _ in range(copies))
     
     #---------[CACHE]---------#
     def _hashable(self, function_name, params):
         return (function_name, tuple(sorted(params.items())))
 
     def _cache_indicator(self, function_name, params, values):
         key = self._hashable(function_name, params)
```

### Comparing `qfinuwa-1.1.4.2/src/qfinuwa/opt/_stockdata.py` & `qfinuwa-1.1.5/src/qfinuwa/opt/_stockdata.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,70 +25,72 @@
         self._stock_df = dict()
 
         self._L = 0
         self._index = None
 
         self._verbose = verbose
 
-        self.spy = None
+        # self.spy = None
 
         self._stocks = []
 
         if data_folder is None: return
         
         if stocks is None:
-            stock = [f.split('.')[0] for f in os.listdir(data_folder) if f.endswith('.csv')]
+            stocks = [f.split('.')[0] for f in os.listdir(data_folder) if f.endswith('.csv')]
 
         # if len(stocks) == 0:
         #     raise ValueError('No stocks provided')
         
         self._stocks = sorted(stocks)
         # stocks + ['SPY']
         for stock in (tqdm(stocks, desc='> Fetching data') if verbose else stocks):
 
             _df = pd.read_csv(os.path.join(data_folder, f'{stock}.csv'))
             
             if self._L == 0:
                 self._L = len(_df)
                 self._index = pd.to_datetime(_df['time'])
 
-            if stock == 'SPY':
-                self.spy = _df['close'].to_numpy()
+            # if stock == 'SPY':
+            #     self.spy = _df['close'].to_numpy()
 
             self._stock_df[stock] = _df[self._measurement]
         self._data = self._compress_data()
 
         # pre calcualte the price at every iteration for efficiency
         self._prices = np.array([{stock: self._data[i, 1 + s*5]
                                 for s, stock in enumerate(stocks)} for i in range(self._L)])
 
-        # self.sis = {s: dict() for s in stocks}
-        self.sinames = [(measurement, stock , i) for measurement, (i, stock) in 
-                        product(self._measurement, enumerate(self._stocks))]
+        self.sinames = [(measurement, stock , i) for i, (stock, measurement) in 
+                        enumerate(product(self._stocks, self._measurement))]
     
     #---------------[Properties]-----------------#
     @property
     def stocks(self):
         return self._stocks
 
     @property
     def index(self):
         return self._index
     
     @property
+    def date_range(self):
+        return min(self._index), max(self._index)
+
+    @property
     def prices(self):
         siss = []
         for index in (tqdm(range(len(self)),  desc = '> Precompiling data', mininterval=0.5) if self._verbose else range(len(self))):
             A = {measurement: dict() for measurement in self._measurement}
             
             for measurement, stock, i in self.sinames:
                 A[measurement][stock] = self._data[:index+1, i]
             siss.append(A)
 
-
         return self._prices, siss
     
     #---------------[Private Methods]-----------------#
     def _compress_data(self) -> np.ndarray:
 
         return np.concatenate(
             [df.loc[:, df.columns != 'time'].to_numpy() for _, df in sorted(self._stock_df.items())], axis=1).astype('float64')
```

### Comparing `qfinuwa-1.1.4.2/src/qfinuwa/plotting.py` & `qfinuwa-1.1.5/src/qfinuwa/plotting.py`

 * *Files 14% similar despite different names*

```diff
@@ -8,64 +8,60 @@
 from .opt._result import SingleRunResult
 
 class Plotting:
 
     #---------------[Class Methods]-----------------#
     
     @classmethod
-    def plot_result(cls, result: SingleRunResult, stocks: list=[], transactions_on: str = None, normalise_stocks: bool =True, filename: str = None) -> None:
+    def plot_result(cls, result: SingleRunResult, show_portfolio: bool=True, stocks: list=[], show_transactions: bool = True, normalise_stocks: bool =True, filename: str = None) -> None:
         '''
         Plots the results of a single run.
 
         ## Parameters
         - ``result`` (``SingleRunResult``): The result of a single run.
+        - ``show_portfolio`` (``bool``): show portfolio value
         - ``stocks`` (``list``): A list of stocks to plot.
-        - ``transactions_on`` (``str``): The stock to plot transactions on. If ``portfolio``, transactions will be plotted on the portfolio value.
+        - ``show_transactions`` (``bool``): If ``True`` transaction will be plotted on the respective instrumenets.
         - ``normalise_stocks`` (``bool``): If ``True``, stocks will be normalised to the portfolio value at the start of the run.
         - ``filename`` (``str``): The filename to save the plot to. If ``None``, the plot will be displayed in a browser.
 
         ## Returns
         ``None``
         '''
         
         p = bokeh.plotting.figure(x_axis_type='linear', title=f"Portfolio Value over Time - {result._datetimeindex.iloc[0]} --> {result._datetimeindex.iloc[-1]}", width=1000, height=400)
         p.grid.grid_line_alpha = 0.3
         p.xaxis.axis_label = 'Date'
         p.yaxis.axis_label = 'Portfolio Value'
         p.xaxis.major_label_overrides = {
             i: date.strftime('%Y-%m-%d %H:%S') for i, date in enumerate(result._datetimeindex)
         }
+        
         # -----[plotting portfolio]-----
-        r = np.array([_ for _ in range(len(result.cash))])
-        p.line(r, result.cash, line_width=2, legend_label='portfolio', color='black')
+        value = [sum(result.value[s][i][0] - result.value[s][i][1]for s in stocks) for i in range(len(list(result.value.values())[0]))]
+        r = np.array([_ for _ in range(len(value))])
+        if show_portfolio:
+            p.line(r, value, line_width=2, legend_label='portfolio', color='black')
 
         # -----[plotting buys and sells]-----
-
-        for stock in stocks:
-            price = result._stockdata[stock]['close'][result._start:result._end]
-            l = price*result.cash[0]/price.iloc[0] if normalise_stocks else price
-            # print(l)
-            p.line(r, l, line_width=2, color='red', legend_label=stock)
-
-        lbuy = np.array([i for i, *_ in result._longs['enter']])
-        lsell = np.array([i for i, *_ in result._longs['exit']])
-        sbuy = np.array([i for i, *_ in result._shorts['enter']])
-        sclose = np.array([i for i, *_ in result._shorts['exit']])
+        stock_prices = {stock: result._stockdata[stock]['close'][result._start:result._end] for stock in stocks}
+        for stock, prices in stock_prices.items():
+            p.line(r, prices, line_width=2, color='blue', legend_label=stock)
+
+        lbuy = {stock: [i for i, s, q in result.buys if s == stock] for stock in stocks}
+        lsell = {stock: [i for i, s, q in result.sells if s == stock] for stock in stocks}
+        # sbuy = np.array([i for i, *_ in result._shorts['enter']])
+        # sclose = np.array([i for i, *_ in result._shorts['exit']])
         SIZE = 4
-        if transactions_on:
-            if transactions_on == 'portfolio':
-                on = result.cash
-            else:
-                l = result._stockdata[transactions_on]['close'][result._start:result._end]
-                on = np.array(l*result.cash[0]/l.iloc[0] if normalise_stocks else l)
-
-            p.circle(lbuy, np.array([on[i] for i in lbuy]), color='red', size=SIZE, legend_label='enter long')
-            p.circle(lsell, np.array([on[i] for i in lsell]), color='green', size=SIZE, legend_label='sell long')
-            p.circle(sbuy, np.array([on[i] for i in sbuy]), color='yellow', size=SIZE, legend_label='enter short')
-            p.circle(sclose, np.array([on[i] for i in sclose]), color='pink', size=SIZE, legend_label='cover short')
+        if show_transactions:
+            
+            for stock, prices in stock_prices.items():
+                # print(stock, prices[0])
+                p.circle(lbuy[stock], np.array([prices.iloc[i] for i in lbuy[stock]]), color='red', size=SIZE, legend_label='buy')
+                p.circle(lsell[stock], np.array([prices.iloc[i] for i in lsell[stock]]), color='green', size=SIZE, legend_label='sell')
 
         bokeh.plotting.show(p)
         if filename:
             bokeh.plotting.output_file(filename)
 
     @classmethod
     def plot_indicators(cls, indicators, data_folder: str, stocks: list = [], filename: bool=None) -> None:
```

### Comparing `qfinuwa-1.1.4.2/src/qfinuwa/strategy.py` & `qfinuwa-1.1.5/src/qfinuwa/strategy.py`

 * *Files identical despite different names*

### Comparing `qfinuwa-1.1.4.2/src/qfinuwa.egg-info/PKG-INFO` & `qfinuwa-1.1.5/src/qfinuwa.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qfinuwa
-Version: 1.1.4.2
+Version: 1.1.5
 Summary: Framework for backtesting quantitative trading algorithims.
 Home-page: https://github.com/QFinUWA/algo-backtester/issues
 Author: Isaac Bergl
 Author-email: tberg644@gmail.com
 Project-URL: Bug Tracker, https://github.com/QFinUWA/algo-backtester/issues
 Project-URL: repository, https://github.com/QFinUWA/algo-backtester
 Classifier: Programming Language :: Python :: 3
@@ -33,24 +33,14 @@
 
 path_to_API = 'API_key.txt'
 download_folder = './data'
 
 API.fetch_stocks(['AAPL', 'GOOG', 'TSLA'], path_to_API, download_folder)
 ```
 
-To pull prepepared data from QFin's googledrive, call ``API.from_google_drive``:
-
-```py
-
-file_ids = 'file_ids.txt'
-download_folder = './data'
-
-API.from_google_drive(file_ids, download_folder)
-```
-
 ## Indicator Class
 
 #### Multi-Indicators
 
 A multi-indicator takes in a single signal (price of an arbitary stock) and outputs a transformation of that stock.
 
 It is called ``MultiIndicator`` because the indicator will have multiple values (one for each stock)
@@ -150,29 +140,37 @@
 
 Similar to ``qfin.Indicators``, you can define hyperparameters for your model in ``__init__``.
 
 ```py
 # Example Strategy
 class BasicBollinger(Strategy):
 
-    def __init__(self, quantity=1):
+    def __init__(self, quantity=5):
         self.quantity = quantity
-        return
-
+        self.n_failed_orders = 0
+    
     def on_data(self, prices, indicators, portfolio):
-        
+
         # If current price is below lower Bollinger Band, enter a long position
-        if(prices['close']['AAPL'][-1] < indicators['lower_bollinger']['AAPL'][-1]):
-            portfolio.cover_short('AAPL', quantity=self.quantity)
-            portfolio.enter_long('AAPL', quantity=self.quantity)
-
-        # If current price is above upper Bollinger Band, enter a long position   
-        if(prices['close']['AAPL'][-1] > indicators['upper_bollinger']['AAPL'][-1]):
-            portfolio.sell_long('AAPL', quantity=self.quantity)
-            portfolio.enter_short('AAPL', quantity=self.quantity)
+        for stock in portfolio.stocks:
+
+            if(prices['close'][stock][-1] < indicators['lower_bollinger'][stock][-1]):
+                order_success = portfolio.order(stock, quantity=self.quantity)
+                if not order_success:
+                    self.n_failed_orders += 1
+            
+            # If current price is above upper Bollinger Band, enter a short position
+            if(prices['close'][stock][-1] > indicators['upper_bollinger'][stock][-1]):
+                order_success = portfolio.order(stock, quantity=-self.quantity)
+                if not order_success:
+                    self.n_failed_orders += 1
+
+    def on_finish(self):
+        # Added to results object - access using result.on_finish
+        return self.n_failed_orders
 ```
 Additionally, you can specify a function ``on_finish`` that will run on the completion of a run, if you want to save your own data. Whatever this function returns will can be accessed in the results (see ``SingleRunResults.on_finish``).
 ## Backtester Class
 
 The ``Backtester`` class asks for a custom strategy, custom indicators and data from the user. Once created, it can run multiple backtests without having to recalculate the indicators - when used in a Notebook environment the backtester object can persist and incrementally updated with new values.
 
 ### Creating a Backtester
@@ -181,15 +179,15 @@
 
 
 ```py
 from qfinuwa import Backtester
 
 backtester = Backtester(CustomStrategy, CustomIndicators, 
                         data=r'\data', days=90, 
-                        cash=1000, fee=0.01)
+                        delta_limits=1000, fee=0.01)
 ```
 
 ## Updating Indicator Parameters
 
 ### Update Parameters
 
 ```py
```

