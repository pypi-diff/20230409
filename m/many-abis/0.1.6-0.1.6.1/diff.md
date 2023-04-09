# Comparing `tmp/many_abis-0.1.6.tar.gz` & `tmp/many_abis-0.1.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "many_abis-0.1.6.tar", last modified: Fri Apr  7 15:07:54 2023, max compression
+gzip compressed data, was "many_abis-0.1.6.1.tar", last modified: Sun Apr  9 16:28:05 2023, max compression
```

## Comparing `many_abis-0.1.6.tar` & `many_abis-0.1.6.1.tar`

### file list

```diff
@@ -1,82 +1,82 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 15:07:54.054352 many_abis-0.1.6/
--rw-r--r--   0 runner    (1001) docker     (123)     3867 2023-04-07 15:07:54.054352 many_abis-0.1.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3500 2023-04-07 15:07:42.000000 many_abis-0.1.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 15:07:54.050352 many_abis-0.1.6/many_abis/
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-04-07 15:07:42.000000 many_abis-0.1.6/many_abis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-04-07 15:07:42.000000 many_abis-0.1.6/many_abis/_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-04-07 15:07:42.000000 many_abis-0.1.6/many_abis/abis.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 15:07:54.046352 many_abis-0.1.6/many_abis/assets/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 15:07:54.046352 many_abis-0.1.6/many_abis/assets/dex/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 15:07:54.046352 many_abis-0.1.6/many_abis/assets/dex/aave/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 15:07:54.050352 many_abis-0.1.6/many_abis/assets/dex/aave/v1/
--rw-r--r--   0 runner    (1001) docker     (123)    16282 2023-04-07 15:07:42.000000 many_abis-0.1.6/many_abis/assets/dex/aave/v1/atoken.abi
--rw-r--r--   0 runner    (1001) docker     (123)    22101 2023-04-07 15:07:42.000000 many_abis-0.1.6/many_abis/assets/dex/aave/v1/lending_pool.abi
--rw-r--r--   0 runner    (1001) docker     (123)    11612 2023-04-07 15:07:42.000000 many_abis-0.1.6/many_abis/assets/dex/aave/v1/lending_pool_addresses_provider.abi
--rw-r--r--   0 runner    (1001) docker     (123)    34411 2023-04-07 15:07:42.000000 many_abis-0.1.6/many_abis/assets/dex/aave/v1/lending_pool_core.abi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 15:07:54.050352 many_abis-0.1.6/many_abis/assets/dex/aave/v2/
--rw-r--r--   0 runner    (1001) docker     (123)     8138 2023-04-07 15:07:42.000000 many_abis-0.1.6/many_abis/assets/dex/aave/v2/collector.abi
--rw-r--r--   0 runner    (1001) docker     (123)    10795 2023-04-07 15:07:42.000000 many_abis-0.1.6/many_abis/assets/dex/aave/v2/incentives_controller.abi
--rw-r--r--   0 runner    (1001) docker     (123)    22079 2023-04-07 15:07:42.000000 many_abis-0.1.6/many_abis/assets/dex/aave/v2/lending_pool.abi
--rw-r--r--   0 runner    (1001) docker     (123)    34411 2023-04-07 15:07:42.000000 many_abis-0.1.6/many_abis/assets/dex/aave/v2/lending_pool_addresses_provider.abi
--rw-r--r--   0 runner    (1001) docker     (123)     2727 2023-04-07 15:07:42.000000 many_abis-0.1.6/many_abis/assets/dex/aave/v2/lending_pool_addresses_provider_registry.abi
--rw-r--r--   0 runner    (1001) docker     (123)     2683 2023-04-07 15:07:42.000000 many_abis-0.1.6/many_abis/assets/dex/aave/v2/lending_pool_collateral_manager.abi
--rw-r--r--   0 runner    (1001) docker     (123)    11894 2023-04-07 15:07:42.000000 many_abis-0.1.6/many_abis/assets/dex/aave/v2/lending_pool_configurator.abi
--rw-r--r--   0 runner    (1001) docker     (123)     2052 2023-04-07 15:07:42.000000 many_abis-0.1.6/many_abis/assets/dex/aave/v2/lending_rate_oracle.abi
--rw-r--r--   0 runner    (1001) docker     (123)    15658 2023-04-07 15:07:42.000000 many_abis-0.1.6/many_abis/assets/dex/aave/v2/pool_admin.abi
--rw-r--r--   0 runner    (1001) docker     (123)     4455 2023-04-07 15:07:42.000000 many_abis-0.1.6/many_abis/assets/dex/aave/v2/price_oracle.abi
--rw-r--r--   0 runner    (1001) docker     (123)     6350 2023-04-07 15:07:42.000000 many_abis-0.1.6/many_abis/assets/dex/aave/v2/protocal_data_provider.abi
--rw-r--r--   0 runner    (1001) docker     (123)    32705 2023-04-07 15:07:42.000000 many_abis-0.1.6/many_abis/assets/dex/aave/v2/ui_incentive_data_provider.abi
--rw-r--r--   0 runner    (1001) docker     (123)    12204 2023-04-07 15:07:42.000000 many_abis-0.1.6/many_abis/assets/dex/aave/v2/ui_pool_data_provider.abi
--rw-r--r--   0 runner    (1001) docker     (123)     5659 2023-04-07 15:07:42.000000 many_abis-0.1.6/many_abis/assets/dex/aave/v2/weth_gateway.abi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 15:07:54.046352 many_abis-0.1.6/many_abis/assets/dex/joe/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 15:07:54.050352 many_abis-0.1.6/many_abis/assets/dex/joe/v2/
--rw-r--r--   0 runner    (1001) docker     (123)     3894 2023-04-07 15:07:42.000000 many_abis-0.1.6/many_abis/assets/dex/joe/v2/factory.abi
--rw-r--r--   0 runner    (1001) docker     (123)    12189 2023-04-07 15:07:42.000000 many_abis-0.1.6/many_abis/assets/dex/joe/v2/pair.abi
--rw-r--r--   0 runner    (1001) docker     (123)    19626 2023-04-07 15:07:42.000000 many_abis-0.1.6/many_abis/assets/dex/joe/v2/router.abi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 15:07:54.046352 many_abis-0.1.6/many_abis/assets/dex/pancake/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 15:07:54.054352 many_abis-0.1.6/many_abis/assets/dex/pancake/v3/
--rw-r--r--   0 runner    (1001) docker     (123)     2187 2023-04-07 15:07:42.000000 many_abis-0.1.6/many_abis/assets/dex/pancake/v3/IPeriphery_payments_with_fee.abi
--rw-r--r--   0 runner    (1001) docker     (123)    30717 2023-04-07 15:07:42.000000 many_abis-0.1.6/many_abis/assets/dex/pancake/v3/master_chef_v3.abi
--rw-r--r--   0 runner    (1001) docker     (123)    24647 2023-04-07 15:07:42.000000 many_abis-0.1.6/many_abis/assets/dex/pancake/v3/non_fungible_position_manager.abi
--rw-r--r--   0 runner    (1001) docker     (123)     4035 2023-04-07 15:07:42.000000 many_abis-0.1.6/many_abis/assets/dex/pancake/v3/quoter.abi
--rw-r--r--   0 runner    (1001) docker     (123)     5983 2023-04-07 15:07:42.000000 many_abis-0.1.6/many_abis/assets/dex/pancake/v3/quoter_v2.abi
--rw-r--r--   0 runner    (1001) docker     (123)    12082 2023-04-07 15:07:42.000000 many_abis-0.1.6/many_abis/assets/dex/pancake/v3/router_v3.abi
--rw-r--r--   0 runner    (1001) docker     (123)     2987 2023-04-07 15:07:42.000000 many_abis-0.1.6/many_abis/assets/dex/pancake/v3/self_permit.abi
--rw-r--r--   0 runner    (1001) docker     (123)    14774 2023-04-07 15:07:42.000000 many_abis-0.1.6/many_abis/assets/dex/pancake/v3/staker.abi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 15:07:54.046352 many_abis-0.1.6/many_abis/assets/dex/uniswap/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 15:07:54.054352 many_abis-0.1.6/many_abis/assets/dex/uniswap/bsc/
--rw-r--r--   0 runner    (1001) docker     (123)     9425 2023-04-07 15:07:42.000000 many_abis-0.1.6/many_abis/assets/dex/uniswap/bsc/router.abi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 15:07:54.054352 many_abis-0.1.6/many_abis/assets/dex/uniswap/v1/
--rw-r--r--   0 runner    (1001) docker     (123)    32705 2023-04-07 15:07:42.000000 many_abis-0.1.6/many_abis/assets/dex/uniswap/v1/exchange.abi
--rw-r--r--   0 runner    (1001) docker     (123)     2195 2023-04-07 15:07:42.000000 many_abis-0.1.6/many_abis/assets/dex/uniswap/v1/factory.abi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 15:07:54.054352 many_abis-0.1.6/many_abis/assets/dex/uniswap/v2/
--rw-r--r--   0 runner    (1001) docker     (123)     3571 2023-04-07 15:07:42.000000 many_abis-0.1.6/many_abis/assets/dex/uniswap/v2/factory.abi
--rw-r--r--   0 runner    (1001) docker     (123)    13409 2023-04-07 15:07:42.000000 many_abis-0.1.6/many_abis/assets/dex/uniswap/v2/pair.abi
--rw-r--r--   0 runner    (1001) docker     (123)    19603 2023-04-07 15:07:42.000000 many_abis-0.1.6/many_abis/assets/dex/uniswap/v2/router.abi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 15:07:54.054352 many_abis-0.1.6/many_abis/assets/dex/uniswap/v3/
--rw-r--r--   0 runner    (1001) docker     (123)     4419 2023-04-07 15:07:42.000000 many_abis-0.1.6/many_abis/assets/dex/uniswap/v3/factory.abi
--rw-r--r--   0 runner    (1001) docker     (123)     6431 2023-04-07 15:07:42.000000 many_abis-0.1.6/many_abis/assets/dex/uniswap/v3/multicall.abi
--rw-r--r--   0 runner    (1001) docker     (123)    24310 2023-04-07 15:07:42.000000 many_abis-0.1.6/many_abis/assets/dex/uniswap/v3/non_fungible_position_manage.abi
--rw-r--r--   0 runner    (1001) docker     (123)    19610 2023-04-07 15:07:42.000000 many_abis-0.1.6/many_abis/assets/dex/uniswap/v3/pool.abi
--rw-r--r--   0 runner    (1001) docker     (123)     3702 2023-04-07 15:07:42.000000 many_abis-0.1.6/many_abis/assets/dex/uniswap/v3/quoter.abi
--rw-r--r--   0 runner    (1001) docker     (123)    11745 2023-04-07 15:07:42.000000 many_abis-0.1.6/many_abis/assets/dex/uniswap/v3/router.abi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 15:07:54.054352 many_abis-0.1.6/many_abis/assets/erc/
--rw-r--r--   0 runner    (1001) docker     (123)     6181 2023-04-07 15:07:42.000000 many_abis-0.1.6/many_abis/assets/erc/ERC1155.abi
--rw-r--r--   0 runner    (1001) docker     (123)     3685 2023-04-07 15:07:42.000000 many_abis-0.1.6/many_abis/assets/erc/ERC20.abi
--rw-r--r--   0 runner    (1001) docker     (123)     6450 2023-04-07 15:07:42.000000 many_abis-0.1.6/many_abis/assets/erc/ERC721.abi
--rw-r--r--   0 runner    (1001) docker     (123)    10960 2023-04-07 15:07:42.000000 many_abis-0.1.6/many_abis/assets/erc/ERC777.abi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 15:07:54.054352 many_abis-0.1.6/many_abis/assets/tokens/
--rw-r--r--   0 runner    (1001) docker     (123)     4612 2023-04-07 15:07:42.000000 many_abis-0.1.6/many_abis/assets/tokens/weth9.abi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 15:07:54.054352 many_abis-0.1.6/many_abis/assets/utils/
--rw-r--r--   0 runner    (1001) docker     (123)    20708 2023-04-07 15:07:42.000000 many_abis-0.1.6/many_abis/assets/utils/chains.json
--rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-04-07 15:07:42.000000 many_abis-0.1.6/many_abis/chains.py
--rw-r--r--   0 runner    (1001) docker     (123)     2145 2023-04-07 15:07:42.000000 many_abis-0.1.6/many_abis/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)      913 2023-04-07 15:07:42.000000 many_abis-0.1.6/many_abis/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 15:07:54.050352 many_abis-0.1.6/many_abis.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3867 2023-04-07 15:07:54.000000 many_abis-0.1.6/many_abis.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2536 2023-04-07 15:07:54.000000 many_abis-0.1.6/many_abis.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-07 15:07:54.000000 many_abis-0.1.6/many_abis.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-07 15:07:54.000000 many_abis-0.1.6/many_abis.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-07 15:07:54.000000 many_abis-0.1.6/many_abis.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-07 15:07:54.054352 many_abis-0.1.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      858 2023-04-07 15:07:42.000000 many_abis-0.1.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 16:28:05.862290 many_abis-0.1.6.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     3966 2023-04-09 16:28:05.862290 many_abis-0.1.6.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3597 2023-04-09 16:27:52.000000 many_abis-0.1.6.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 16:28:05.854290 many_abis-0.1.6.1/many_abis/
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-04-09 16:27:52.000000 many_abis-0.1.6.1/many_abis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-04-09 16:27:52.000000 many_abis-0.1.6.1/many_abis/_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-04-09 16:27:52.000000 many_abis-0.1.6.1/many_abis/abis.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 16:28:05.854290 many_abis-0.1.6.1/many_abis/assets/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 16:28:05.854290 many_abis-0.1.6.1/many_abis/assets/dex/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 16:28:05.850290 many_abis-0.1.6.1/many_abis/assets/dex/aave/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 16:28:05.854290 many_abis-0.1.6.1/many_abis/assets/dex/aave/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)    16282 2023-04-09 16:27:52.000000 many_abis-0.1.6.1/many_abis/assets/dex/aave/v1/atoken.abi
+-rw-r--r--   0 runner    (1001) docker     (123)    22101 2023-04-09 16:27:52.000000 many_abis-0.1.6.1/many_abis/assets/dex/aave/v1/lending_pool.abi
+-rw-r--r--   0 runner    (1001) docker     (123)    11612 2023-04-09 16:27:52.000000 many_abis-0.1.6.1/many_abis/assets/dex/aave/v1/lending_pool_addresses_provider.abi
+-rw-r--r--   0 runner    (1001) docker     (123)    34411 2023-04-09 16:27:52.000000 many_abis-0.1.6.1/many_abis/assets/dex/aave/v1/lending_pool_core.abi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 16:28:05.858290 many_abis-0.1.6.1/many_abis/assets/dex/aave/v2/
+-rw-r--r--   0 runner    (1001) docker     (123)     8138 2023-04-09 16:27:52.000000 many_abis-0.1.6.1/many_abis/assets/dex/aave/v2/collector.abi
+-rw-r--r--   0 runner    (1001) docker     (123)    10795 2023-04-09 16:27:52.000000 many_abis-0.1.6.1/many_abis/assets/dex/aave/v2/incentives_controller.abi
+-rw-r--r--   0 runner    (1001) docker     (123)    22079 2023-04-09 16:27:52.000000 many_abis-0.1.6.1/many_abis/assets/dex/aave/v2/lending_pool.abi
+-rw-r--r--   0 runner    (1001) docker     (123)    34411 2023-04-09 16:27:52.000000 many_abis-0.1.6.1/many_abis/assets/dex/aave/v2/lending_pool_addresses_provider.abi
+-rw-r--r--   0 runner    (1001) docker     (123)     2727 2023-04-09 16:27:52.000000 many_abis-0.1.6.1/many_abis/assets/dex/aave/v2/lending_pool_addresses_provider_registry.abi
+-rw-r--r--   0 runner    (1001) docker     (123)     2683 2023-04-09 16:27:52.000000 many_abis-0.1.6.1/many_abis/assets/dex/aave/v2/lending_pool_collateral_manager.abi
+-rw-r--r--   0 runner    (1001) docker     (123)    11894 2023-04-09 16:27:52.000000 many_abis-0.1.6.1/many_abis/assets/dex/aave/v2/lending_pool_configurator.abi
+-rw-r--r--   0 runner    (1001) docker     (123)     2052 2023-04-09 16:27:52.000000 many_abis-0.1.6.1/many_abis/assets/dex/aave/v2/lending_rate_oracle.abi
+-rw-r--r--   0 runner    (1001) docker     (123)    15658 2023-04-09 16:27:52.000000 many_abis-0.1.6.1/many_abis/assets/dex/aave/v2/pool_admin.abi
+-rw-r--r--   0 runner    (1001) docker     (123)     4455 2023-04-09 16:27:52.000000 many_abis-0.1.6.1/many_abis/assets/dex/aave/v2/price_oracle.abi
+-rw-r--r--   0 runner    (1001) docker     (123)     6350 2023-04-09 16:27:52.000000 many_abis-0.1.6.1/many_abis/assets/dex/aave/v2/protocal_data_provider.abi
+-rw-r--r--   0 runner    (1001) docker     (123)    32705 2023-04-09 16:27:52.000000 many_abis-0.1.6.1/many_abis/assets/dex/aave/v2/ui_incentive_data_provider.abi
+-rw-r--r--   0 runner    (1001) docker     (123)    12204 2023-04-09 16:27:52.000000 many_abis-0.1.6.1/many_abis/assets/dex/aave/v2/ui_pool_data_provider.abi
+-rw-r--r--   0 runner    (1001) docker     (123)     5659 2023-04-09 16:27:52.000000 many_abis-0.1.6.1/many_abis/assets/dex/aave/v2/weth_gateway.abi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 16:28:05.850290 many_abis-0.1.6.1/many_abis/assets/dex/joe/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 16:28:05.858290 many_abis-0.1.6.1/many_abis/assets/dex/joe/v2/
+-rw-r--r--   0 runner    (1001) docker     (123)     3894 2023-04-09 16:27:52.000000 many_abis-0.1.6.1/many_abis/assets/dex/joe/v2/factory.abi
+-rw-r--r--   0 runner    (1001) docker     (123)    12189 2023-04-09 16:27:52.000000 many_abis-0.1.6.1/many_abis/assets/dex/joe/v2/pair.abi
+-rw-r--r--   0 runner    (1001) docker     (123)    19626 2023-04-09 16:27:52.000000 many_abis-0.1.6.1/many_abis/assets/dex/joe/v2/router.abi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 16:28:05.854290 many_abis-0.1.6.1/many_abis/assets/dex/pancake/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 16:28:05.858290 many_abis-0.1.6.1/many_abis/assets/dex/pancake/v3/
+-rw-r--r--   0 runner    (1001) docker     (123)     2187 2023-04-09 16:27:52.000000 many_abis-0.1.6.1/many_abis/assets/dex/pancake/v3/IPeriphery_payments_with_fee.abi
+-rw-r--r--   0 runner    (1001) docker     (123)    30717 2023-04-09 16:27:52.000000 many_abis-0.1.6.1/many_abis/assets/dex/pancake/v3/master_chef_v3.abi
+-rw-r--r--   0 runner    (1001) docker     (123)    24647 2023-04-09 16:27:52.000000 many_abis-0.1.6.1/many_abis/assets/dex/pancake/v3/non_fungible_position_manager.abi
+-rw-r--r--   0 runner    (1001) docker     (123)     4035 2023-04-09 16:27:52.000000 many_abis-0.1.6.1/many_abis/assets/dex/pancake/v3/quoter.abi
+-rw-r--r--   0 runner    (1001) docker     (123)     5983 2023-04-09 16:27:52.000000 many_abis-0.1.6.1/many_abis/assets/dex/pancake/v3/quoter_v2.abi
+-rw-r--r--   0 runner    (1001) docker     (123)    12082 2023-04-09 16:27:52.000000 many_abis-0.1.6.1/many_abis/assets/dex/pancake/v3/router_v3.abi
+-rw-r--r--   0 runner    (1001) docker     (123)     2987 2023-04-09 16:27:52.000000 many_abis-0.1.6.1/many_abis/assets/dex/pancake/v3/self_permit.abi
+-rw-r--r--   0 runner    (1001) docker     (123)    14774 2023-04-09 16:27:52.000000 many_abis-0.1.6.1/many_abis/assets/dex/pancake/v3/staker.abi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 16:28:05.854290 many_abis-0.1.6.1/many_abis/assets/dex/uniswap/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 16:28:05.858290 many_abis-0.1.6.1/many_abis/assets/dex/uniswap/bsc/
+-rw-r--r--   0 runner    (1001) docker     (123)     9425 2023-04-09 16:27:52.000000 many_abis-0.1.6.1/many_abis/assets/dex/uniswap/bsc/router.abi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 16:28:05.858290 many_abis-0.1.6.1/many_abis/assets/dex/uniswap/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)    32705 2023-04-09 16:27:52.000000 many_abis-0.1.6.1/many_abis/assets/dex/uniswap/v1/exchange.abi
+-rw-r--r--   0 runner    (1001) docker     (123)     2195 2023-04-09 16:27:52.000000 many_abis-0.1.6.1/many_abis/assets/dex/uniswap/v1/factory.abi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 16:28:05.858290 many_abis-0.1.6.1/many_abis/assets/dex/uniswap/v2/
+-rw-r--r--   0 runner    (1001) docker     (123)     3571 2023-04-09 16:27:52.000000 many_abis-0.1.6.1/many_abis/assets/dex/uniswap/v2/factory.abi
+-rw-r--r--   0 runner    (1001) docker     (123)    13409 2023-04-09 16:27:52.000000 many_abis-0.1.6.1/many_abis/assets/dex/uniswap/v2/pair.abi
+-rw-r--r--   0 runner    (1001) docker     (123)    19603 2023-04-09 16:27:52.000000 many_abis-0.1.6.1/many_abis/assets/dex/uniswap/v2/router.abi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 16:28:05.862290 many_abis-0.1.6.1/many_abis/assets/dex/uniswap/v3/
+-rw-r--r--   0 runner    (1001) docker     (123)     4419 2023-04-09 16:27:52.000000 many_abis-0.1.6.1/many_abis/assets/dex/uniswap/v3/factory.abi
+-rw-r--r--   0 runner    (1001) docker     (123)     6431 2023-04-09 16:27:52.000000 many_abis-0.1.6.1/many_abis/assets/dex/uniswap/v3/multicall.abi
+-rw-r--r--   0 runner    (1001) docker     (123)    24310 2023-04-09 16:27:52.000000 many_abis-0.1.6.1/many_abis/assets/dex/uniswap/v3/non_fungible_position_manage.abi
+-rw-r--r--   0 runner    (1001) docker     (123)    19610 2023-04-09 16:27:52.000000 many_abis-0.1.6.1/many_abis/assets/dex/uniswap/v3/pool.abi
+-rw-r--r--   0 runner    (1001) docker     (123)     3702 2023-04-09 16:27:52.000000 many_abis-0.1.6.1/many_abis/assets/dex/uniswap/v3/quoter.abi
+-rw-r--r--   0 runner    (1001) docker     (123)    11745 2023-04-09 16:27:52.000000 many_abis-0.1.6.1/many_abis/assets/dex/uniswap/v3/router.abi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 16:28:05.862290 many_abis-0.1.6.1/many_abis/assets/erc/
+-rw-r--r--   0 runner    (1001) docker     (123)     6181 2023-04-09 16:27:52.000000 many_abis-0.1.6.1/many_abis/assets/erc/ERC1155.abi
+-rw-r--r--   0 runner    (1001) docker     (123)     3685 2023-04-09 16:27:52.000000 many_abis-0.1.6.1/many_abis/assets/erc/ERC20.abi
+-rw-r--r--   0 runner    (1001) docker     (123)     6450 2023-04-09 16:27:52.000000 many_abis-0.1.6.1/many_abis/assets/erc/ERC721.abi
+-rw-r--r--   0 runner    (1001) docker     (123)    10960 2023-04-09 16:27:52.000000 many_abis-0.1.6.1/many_abis/assets/erc/ERC777.abi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 16:28:05.862290 many_abis-0.1.6.1/many_abis/assets/tokens/
+-rw-r--r--   0 runner    (1001) docker     (123)     4612 2023-04-09 16:27:52.000000 many_abis-0.1.6.1/many_abis/assets/tokens/weth9.abi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 16:28:05.862290 many_abis-0.1.6.1/many_abis/assets/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)    21095 2023-04-09 16:27:52.000000 many_abis-0.1.6.1/many_abis/assets/utils/chains.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-04-09 16:27:52.000000 many_abis-0.1.6.1/many_abis/chains.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2145 2023-04-09 16:27:52.000000 many_abis-0.1.6.1/many_abis/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      913 2023-04-09 16:27:52.000000 many_abis-0.1.6.1/many_abis/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 16:28:05.854290 many_abis-0.1.6.1/many_abis.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3966 2023-04-09 16:28:05.000000 many_abis-0.1.6.1/many_abis.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2536 2023-04-09 16:28:05.000000 many_abis-0.1.6.1/many_abis.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-09 16:28:05.000000 many_abis-0.1.6.1/many_abis.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-09 16:28:05.000000 many_abis-0.1.6.1/many_abis.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-09 16:28:05.000000 many_abis-0.1.6.1/many_abis.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-09 16:28:05.862290 many_abis-0.1.6.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      860 2023-04-09 16:27:52.000000 many_abis-0.1.6.1/setup.py
```

### Comparing `many_abis-0.1.6/PKG-INFO` & `many_abis-0.1.6.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: many_abis
-Version: 0.1.6
+Version: 0.1.6.1
 Summary: A simple way to get different DEXs abis for block chains.
 Home-page: https://github.com/ackness/many_abis
 Author: Yong
 Author-email: ackness8@gmail.com
 License: MIT
 Keywords: abi,dex,block chain,bsc,eth,matic,heco,kcc,pancakeswap,mdex,quickswap,uniswap,koffeeswap
 Description-Content-Type: text/markdown
 
 # Many Abis
 
-![Version](https://img.shields.io/badge/many--abis-v0.1.6-green)
+![Version](https://img.shields.io/badge/many--abis-v0.1.6.1-green)
 ![Pypi](https://img.shields.io/pypi/dm/many-abis)
 
 ![GitHub Org's stars](https://img.shields.io/github/stars/ackness/many_abis?style=social)
 ![GitHub forks](https://img.shields.io/github/forks/ackness/many_abis?style=social)
 
 ---
 
@@ -33,15 +33,15 @@
   - [1] [traderjoexyz](https://traderjoexyz.com/#/home)
 - bsc:
   - [1] [ApeSwap Finance](https://app.apeswap.finance/swap)
   - [2] [BiSwap](https://exchange.biswap.org/#/swap)
   - [3] [MDEX (BSC)](https://bsc.mdex.co/#/swap/)
   - [4] [PancakeSwap v2](https://pancakeswap.finance/swap)
   - [5] [PancakeSwap v3](https://pancakeswap.finance/swap)
-  - [6] [uniswap](https://app.uniswap.org/#/swap)
+  - [6] [Uniswap](https://app.uniswap.org/#/swap)
 - bsc-test:
   - [1] [PancakeSwap v2 (TEST)]()
   - [2] [PancakeSwap v3 (TEST)](https://pancakeswap.finance/swap?chain:bscTestnet)
 - cronos:
   - [1] [Mad Meerkat Finance](https://mm.finance/swap)
 - eth:
   - [1] [Uniswap V2](https://app.uniswap.org/)
@@ -57,14 +57,15 @@
   - [1] [Solarbeam](https://app.solarbeam.io/exchange/swap)
 - okex:
   - [1] [CherrySwap](https://www.cherryswap.net/)
 - polygon:
   - [1] [QuickSwap](https://quickswap.exchange/)
 - optimism:
   - [1] [Uniswap V3](https://app.uniswap.org/#/swap)
+  - [2] [Velodrome V1](https://app.velodrome.finance/swap)
 
 ---
 
 ## Installation
 
 - Download
 
@@ -132,8 +133,11 @@
 print(eth_weth)
 # {'address': '0xC02aaA39b223FE8D0A0e5C4F27eAD9083C756Cc2', 'name': 'Wrapped ETH', 'symbol': 'WETH'}
 
 ds = ma.get('bsc', 'dex', 'pancake_v2')
 print(ds)
 # {'factory_address': '0xcA143Ce32Fe78f1f7019d7d551a6402fC5350c73', 'name': 'PancakeSwap v2', 'router_address': '0x10ED43C718714eb63d5aA57B78B54704E256024E', 'website': 'https://pancakeswap.finance/swap'}
 
+# print all dex
+ma.print_all_dex()
+
 ```
```

### Comparing `many_abis-0.1.6/README.md` & `many_abis-0.1.6.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Many Abis
 
-![Version](https://img.shields.io/badge/many--abis-v0.1.6-green)
+![Version](https://img.shields.io/badge/many--abis-v0.1.6.1-green)
 ![Pypi](https://img.shields.io/pypi/dm/many-abis)
 
 ![GitHub Org's stars](https://img.shields.io/github/stars/ackness/many_abis?style=social)
 ![GitHub forks](https://img.shields.io/github/forks/ackness/many_abis?style=social)
 
 ---
 
@@ -22,15 +22,15 @@
   - [1] [traderjoexyz](https://traderjoexyz.com/#/home)
 - bsc:
   - [1] [ApeSwap Finance](https://app.apeswap.finance/swap)
   - [2] [BiSwap](https://exchange.biswap.org/#/swap)
   - [3] [MDEX (BSC)](https://bsc.mdex.co/#/swap/)
   - [4] [PancakeSwap v2](https://pancakeswap.finance/swap)
   - [5] [PancakeSwap v3](https://pancakeswap.finance/swap)
-  - [6] [uniswap](https://app.uniswap.org/#/swap)
+  - [6] [Uniswap](https://app.uniswap.org/#/swap)
 - bsc-test:
   - [1] [PancakeSwap v2 (TEST)]()
   - [2] [PancakeSwap v3 (TEST)](https://pancakeswap.finance/swap?chain:bscTestnet)
 - cronos:
   - [1] [Mad Meerkat Finance](https://mm.finance/swap)
 - eth:
   - [1] [Uniswap V2](https://app.uniswap.org/)
@@ -46,14 +46,15 @@
   - [1] [Solarbeam](https://app.solarbeam.io/exchange/swap)
 - okex:
   - [1] [CherrySwap](https://www.cherryswap.net/)
 - polygon:
   - [1] [QuickSwap](https://quickswap.exchange/)
 - optimism:
   - [1] [Uniswap V3](https://app.uniswap.org/#/swap)
+  - [2] [Velodrome V1](https://app.velodrome.finance/swap)
 
 ---
 
 ## Installation
 
 - Download
 
@@ -121,8 +122,11 @@
 print(eth_weth)
 # {'address': '0xC02aaA39b223FE8D0A0e5C4F27eAD9083C756Cc2', 'name': 'Wrapped ETH', 'symbol': 'WETH'}
 
 ds = ma.get('bsc', 'dex', 'pancake_v2')
 print(ds)
 # {'factory_address': '0xcA143Ce32Fe78f1f7019d7d551a6402fC5350c73', 'name': 'PancakeSwap v2', 'router_address': '0x10ED43C718714eb63d5aA57B78B54704E256024E', 'website': 'https://pancakeswap.finance/swap'}
 
+# print all dex
+ma.print_all_dex()
+
 ```
```

### Comparing `many_abis-0.1.6/many_abis/abis.py` & `many_abis-0.1.6.1/many_abis/abis.py`

 * *Files identical despite different names*

### Comparing `many_abis-0.1.6/many_abis/assets/dex/aave/v1/atoken.abi` & `many_abis-0.1.6.1/many_abis/assets/dex/aave/v1/atoken.abi`

 * *Files identical despite different names*

### Comparing `many_abis-0.1.6/many_abis/assets/dex/aave/v1/lending_pool.abi` & `many_abis-0.1.6.1/many_abis/assets/dex/aave/v1/lending_pool.abi`

 * *Files identical despite different names*

### Comparing `many_abis-0.1.6/many_abis/assets/dex/aave/v1/lending_pool_addresses_provider.abi` & `many_abis-0.1.6.1/many_abis/assets/dex/aave/v1/lending_pool_addresses_provider.abi`

 * *Files identical despite different names*

### Comparing `many_abis-0.1.6/many_abis/assets/dex/aave/v1/lending_pool_core.abi` & `many_abis-0.1.6.1/many_abis/assets/dex/aave/v1/lending_pool_core.abi`

 * *Files identical despite different names*

### Comparing `many_abis-0.1.6/many_abis/assets/dex/aave/v2/collector.abi` & `many_abis-0.1.6.1/many_abis/assets/dex/aave/v2/collector.abi`

 * *Files identical despite different names*

### Comparing `many_abis-0.1.6/many_abis/assets/dex/aave/v2/incentives_controller.abi` & `many_abis-0.1.6.1/many_abis/assets/dex/aave/v2/incentives_controller.abi`

 * *Files identical despite different names*

### Comparing `many_abis-0.1.6/many_abis/assets/dex/aave/v2/lending_pool.abi` & `many_abis-0.1.6.1/many_abis/assets/dex/aave/v2/lending_pool.abi`

 * *Files identical despite different names*

### Comparing `many_abis-0.1.6/many_abis/assets/dex/aave/v2/lending_pool_addresses_provider.abi` & `many_abis-0.1.6.1/many_abis/assets/dex/aave/v2/lending_pool_addresses_provider.abi`

 * *Files identical despite different names*

### Comparing `many_abis-0.1.6/many_abis/assets/dex/aave/v2/lending_pool_addresses_provider_registry.abi` & `many_abis-0.1.6.1/many_abis/assets/dex/aave/v2/lending_pool_addresses_provider_registry.abi`

 * *Files identical despite different names*

### Comparing `many_abis-0.1.6/many_abis/assets/dex/aave/v2/lending_pool_collateral_manager.abi` & `many_abis-0.1.6.1/many_abis/assets/dex/aave/v2/lending_pool_collateral_manager.abi`

 * *Files identical despite different names*

### Comparing `many_abis-0.1.6/many_abis/assets/dex/aave/v2/lending_pool_configurator.abi` & `many_abis-0.1.6.1/many_abis/assets/dex/aave/v2/lending_pool_configurator.abi`

 * *Files identical despite different names*

### Comparing `many_abis-0.1.6/many_abis/assets/dex/aave/v2/lending_rate_oracle.abi` & `many_abis-0.1.6.1/many_abis/assets/dex/aave/v2/lending_rate_oracle.abi`

 * *Files identical despite different names*

### Comparing `many_abis-0.1.6/many_abis/assets/dex/aave/v2/pool_admin.abi` & `many_abis-0.1.6.1/many_abis/assets/dex/aave/v2/pool_admin.abi`

 * *Files identical despite different names*

### Comparing `many_abis-0.1.6/many_abis/assets/dex/aave/v2/price_oracle.abi` & `many_abis-0.1.6.1/many_abis/assets/dex/aave/v2/price_oracle.abi`

 * *Files identical despite different names*

### Comparing `many_abis-0.1.6/many_abis/assets/dex/aave/v2/protocal_data_provider.abi` & `many_abis-0.1.6.1/many_abis/assets/dex/aave/v2/protocal_data_provider.abi`

 * *Files identical despite different names*

### Comparing `many_abis-0.1.6/many_abis/assets/dex/aave/v2/ui_incentive_data_provider.abi` & `many_abis-0.1.6.1/many_abis/assets/dex/aave/v2/ui_incentive_data_provider.abi`

 * *Files identical despite different names*

### Comparing `many_abis-0.1.6/many_abis/assets/dex/aave/v2/ui_pool_data_provider.abi` & `many_abis-0.1.6.1/many_abis/assets/dex/aave/v2/ui_pool_data_provider.abi`

 * *Files identical despite different names*

### Comparing `many_abis-0.1.6/many_abis/assets/dex/aave/v2/weth_gateway.abi` & `many_abis-0.1.6.1/many_abis/assets/dex/aave/v2/weth_gateway.abi`

 * *Files identical despite different names*

### Comparing `many_abis-0.1.6/many_abis/assets/dex/joe/v2/factory.abi` & `many_abis-0.1.6.1/many_abis/assets/dex/joe/v2/factory.abi`

 * *Files identical despite different names*

### Comparing `many_abis-0.1.6/many_abis/assets/dex/joe/v2/pair.abi` & `many_abis-0.1.6.1/many_abis/assets/dex/joe/v2/pair.abi`

 * *Files identical despite different names*

### Comparing `many_abis-0.1.6/many_abis/assets/dex/joe/v2/router.abi` & `many_abis-0.1.6.1/many_abis/assets/dex/joe/v2/router.abi`

 * *Files identical despite different names*

### Comparing `many_abis-0.1.6/many_abis/assets/dex/pancake/v3/IPeriphery_payments_with_fee.abi` & `many_abis-0.1.6.1/many_abis/assets/dex/pancake/v3/IPeriphery_payments_with_fee.abi`

 * *Files identical despite different names*

### Comparing `many_abis-0.1.6/many_abis/assets/dex/pancake/v3/master_chef_v3.abi` & `many_abis-0.1.6.1/many_abis/assets/dex/pancake/v3/master_chef_v3.abi`

 * *Files identical despite different names*

### Comparing `many_abis-0.1.6/many_abis/assets/dex/pancake/v3/non_fungible_position_manager.abi` & `many_abis-0.1.6.1/many_abis/assets/dex/pancake/v3/non_fungible_position_manager.abi`

 * *Files identical despite different names*

### Comparing `many_abis-0.1.6/many_abis/assets/dex/pancake/v3/quoter.abi` & `many_abis-0.1.6.1/many_abis/assets/dex/pancake/v3/quoter.abi`

 * *Files identical despite different names*

### Comparing `many_abis-0.1.6/many_abis/assets/dex/pancake/v3/quoter_v2.abi` & `many_abis-0.1.6.1/many_abis/assets/dex/pancake/v3/quoter_v2.abi`

 * *Files identical despite different names*

### Comparing `many_abis-0.1.6/many_abis/assets/dex/pancake/v3/router_v3.abi` & `many_abis-0.1.6.1/many_abis/assets/dex/pancake/v3/router_v3.abi`

 * *Files identical despite different names*

### Comparing `many_abis-0.1.6/many_abis/assets/dex/pancake/v3/self_permit.abi` & `many_abis-0.1.6.1/many_abis/assets/dex/pancake/v3/self_permit.abi`

 * *Files identical despite different names*

### Comparing `many_abis-0.1.6/many_abis/assets/dex/pancake/v3/staker.abi` & `many_abis-0.1.6.1/many_abis/assets/dex/pancake/v3/staker.abi`

 * *Files identical despite different names*

### Comparing `many_abis-0.1.6/many_abis/assets/dex/uniswap/bsc/router.abi` & `many_abis-0.1.6.1/many_abis/assets/dex/uniswap/bsc/router.abi`

 * *Files identical despite different names*

### Comparing `many_abis-0.1.6/many_abis/assets/dex/uniswap/v1/exchange.abi` & `many_abis-0.1.6.1/many_abis/assets/dex/uniswap/v1/exchange.abi`

 * *Files identical despite different names*

### Comparing `many_abis-0.1.6/many_abis/assets/dex/uniswap/v1/factory.abi` & `many_abis-0.1.6.1/many_abis/assets/dex/uniswap/v1/factory.abi`

 * *Files identical despite different names*

### Comparing `many_abis-0.1.6/many_abis/assets/dex/uniswap/v2/factory.abi` & `many_abis-0.1.6.1/many_abis/assets/dex/uniswap/v2/factory.abi`

 * *Files identical despite different names*

### Comparing `many_abis-0.1.6/many_abis/assets/dex/uniswap/v2/pair.abi` & `many_abis-0.1.6.1/many_abis/assets/dex/uniswap/v2/pair.abi`

 * *Files identical despite different names*

### Comparing `many_abis-0.1.6/many_abis/assets/dex/uniswap/v2/router.abi` & `many_abis-0.1.6.1/many_abis/assets/dex/uniswap/v2/router.abi`

 * *Files identical despite different names*

### Comparing `many_abis-0.1.6/many_abis/assets/dex/uniswap/v3/factory.abi` & `many_abis-0.1.6.1/many_abis/assets/dex/uniswap/v3/factory.abi`

 * *Files identical despite different names*

### Comparing `many_abis-0.1.6/many_abis/assets/dex/uniswap/v3/multicall.abi` & `many_abis-0.1.6.1/many_abis/assets/dex/uniswap/v3/multicall.abi`

 * *Files identical despite different names*

### Comparing `many_abis-0.1.6/many_abis/assets/dex/uniswap/v3/non_fungible_position_manage.abi` & `many_abis-0.1.6.1/many_abis/assets/dex/uniswap/v3/non_fungible_position_manage.abi`

 * *Files identical despite different names*

### Comparing `many_abis-0.1.6/many_abis/assets/dex/uniswap/v3/pool.abi` & `many_abis-0.1.6.1/many_abis/assets/dex/uniswap/v3/pool.abi`

 * *Files identical despite different names*

### Comparing `many_abis-0.1.6/many_abis/assets/dex/uniswap/v3/quoter.abi` & `many_abis-0.1.6.1/many_abis/assets/dex/uniswap/v3/quoter.abi`

 * *Files identical despite different names*

### Comparing `many_abis-0.1.6/many_abis/assets/dex/uniswap/v3/router.abi` & `many_abis-0.1.6.1/many_abis/assets/dex/uniswap/v3/router.abi`

 * *Files identical despite different names*

### Comparing `many_abis-0.1.6/many_abis/assets/erc/ERC1155.abi` & `many_abis-0.1.6.1/many_abis/assets/erc/ERC1155.abi`

 * *Files identical despite different names*

### Comparing `many_abis-0.1.6/many_abis/assets/erc/ERC20.abi` & `many_abis-0.1.6.1/many_abis/assets/erc/ERC20.abi`

 * *Files identical despite different names*

### Comparing `many_abis-0.1.6/many_abis/assets/erc/ERC721.abi` & `many_abis-0.1.6.1/many_abis/assets/erc/ERC721.abi`

 * *Files identical despite different names*

### Comparing `many_abis-0.1.6/many_abis/assets/erc/ERC777.abi` & `many_abis-0.1.6.1/many_abis/assets/erc/ERC777.abi`

 * *Files identical despite different names*

### Comparing `many_abis-0.1.6/many_abis/assets/tokens/weth9.abi` & `many_abis-0.1.6.1/many_abis/assets/tokens/weth9.abi`

 * *Files identical despite different names*

### Comparing `many_abis-0.1.6/many_abis/assets/utils/chains.json` & `many_abis-0.1.6.1/many_abis/assets/utils/chains.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9978031517094017%*

 * *Differences: {"'bsc'": "{'dex': {'uniswap': {'name': 'Uniswap'}}}",*

 * * "'optimism'": "{'dex': {'velodrome_v1': OrderedDict([('factory_address', "*

 * *               "'0xC5be2c918EB04B091962fDF095A217A55CFA42C5'), ('name', 'Velodrome V1'), "*

 * *               "('router_address', '0x9c12939390052919aF3155f41Bf4160Fd3666A6f'), ('website', "*

 * *               "'https://app.velodrome.finance/swap')])}, 'stable_coins': {'sUSD': "*

 * *               "'0x8c6f28f2F1A3C87F0f938b96d27520d9751ec8d9', 'agEUR': "*

 * *               "'0x9485aca5bbBE1667A […]*

```diff
@@ -114,15 +114,15 @@
                 "factory_address": "0x0BFbCF9fa4f9C56B0F40a671Ad40E0805A091865",
                 "name": "PancakeSwap v3",
                 "router_address": "0x13f4EA83D0bd40E75C8222255bc855a974568Dd4",
                 "website": "https://pancakeswap.finance/swap"
             },
             "uniswap": {
                 "address": "0x5Dc88340E1c5c6366864Ee415d6034cadd1A9897",
-                "name": "uniswap",
+                "name": "Uniswap",
                 "website": "https://app.uniswap.org/#/swap"
             }
         },
         "explorer": "https://bscscan.com/",
         "name": "Binance Smart Chain Mainnet",
         "rpc": [
             "https://bsc-dataseed.binance.org/",
@@ -484,29 +484,37 @@
         },
         "dex": {
             "uniswap_v3": {
                 "factory_address": "0x1F98431c8aD98523631AE4a59f267346ea31F984",
                 "name": "Uniswap V3",
                 "router_address": "0xE592427A0AEce92De3Edee1F18E0157C05861564",
                 "website": "https://app.uniswap.org/#/swap"
+            },
+            "velodrome_v1": {
+                "factory_address": "0xC5be2c918EB04B091962fDF095A217A55CFA42C5",
+                "name": "Velodrome V1",
+                "router_address": "0x9c12939390052919aF3155f41Bf4160Fd3666A6f",
+                "website": "https://app.velodrome.finance/swap"
             }
         },
         "explorer": "https://optimistic.etherscan.io/",
         "name": "Optimism Ethereum L2",
         "rpc": [
             "https://mainnet.optimism.io",
             "https://rpc.ankr.com/optimism",
             "https://1rpc.io/op",
             "https://optimism.blockpi.network/v1/rpc/public",
             "https://endpoints.omniatech.io/v1/op/mainnet/public"
         ],
         "stable_coins": {
             "DAI": "0xDA10009cBd5D07dd0CeCc66161FC93D7c9000da1",
             "USDC": "0x7F5c764cBc14f9669B88837ca1490cCa17c31607",
-            "USDT": "0x94b008aA00579c1307B0EF2c499aD98a8ce58e58"
+            "USDT": "0x94b008aA00579c1307B0EF2c499aD98a8ce58e58",
+            "agEUR": "0x9485aca5bbBE1667AD97c7fE7C4531a624C8b1ED",
+            "sUSD": "0x8c6f28f2F1A3C87F0f938b96d27520d9751ec8d9"
         },
         "weth": {
             "address": "0x4200000000000000000000000000000000000006",
             "name": "Wrapped Ether",
             "symbol": "WETH"
         }
     },
```

### Comparing `many_abis-0.1.6/many_abis/chains.py` & `many_abis-0.1.6.1/many_abis/chains.py`

 * *Files identical despite different names*

### Comparing `many_abis-0.1.6/many_abis/constants.py` & `many_abis-0.1.6.1/many_abis/constants.py`

 * *Files identical despite different names*

### Comparing `many_abis-0.1.6/many_abis/utils.py` & `many_abis-0.1.6.1/many_abis/utils.py`

 * *Files identical despite different names*

### Comparing `many_abis-0.1.6/many_abis.egg-info/PKG-INFO` & `many_abis-0.1.6.1/many_abis.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: many-abis
-Version: 0.1.6
+Version: 0.1.6.1
 Summary: A simple way to get different DEXs abis for block chains.
 Home-page: https://github.com/ackness/many_abis
 Author: Yong
 Author-email: ackness8@gmail.com
 License: MIT
 Keywords: abi,dex,block chain,bsc,eth,matic,heco,kcc,pancakeswap,mdex,quickswap,uniswap,koffeeswap
 Description-Content-Type: text/markdown
 
 # Many Abis
 
-![Version](https://img.shields.io/badge/many--abis-v0.1.6-green)
+![Version](https://img.shields.io/badge/many--abis-v0.1.6.1-green)
 ![Pypi](https://img.shields.io/pypi/dm/many-abis)
 
 ![GitHub Org's stars](https://img.shields.io/github/stars/ackness/many_abis?style=social)
 ![GitHub forks](https://img.shields.io/github/forks/ackness/many_abis?style=social)
 
 ---
 
@@ -33,15 +33,15 @@
   - [1] [traderjoexyz](https://traderjoexyz.com/#/home)
 - bsc:
   - [1] [ApeSwap Finance](https://app.apeswap.finance/swap)
   - [2] [BiSwap](https://exchange.biswap.org/#/swap)
   - [3] [MDEX (BSC)](https://bsc.mdex.co/#/swap/)
   - [4] [PancakeSwap v2](https://pancakeswap.finance/swap)
   - [5] [PancakeSwap v3](https://pancakeswap.finance/swap)
-  - [6] [uniswap](https://app.uniswap.org/#/swap)
+  - [6] [Uniswap](https://app.uniswap.org/#/swap)
 - bsc-test:
   - [1] [PancakeSwap v2 (TEST)]()
   - [2] [PancakeSwap v3 (TEST)](https://pancakeswap.finance/swap?chain:bscTestnet)
 - cronos:
   - [1] [Mad Meerkat Finance](https://mm.finance/swap)
 - eth:
   - [1] [Uniswap V2](https://app.uniswap.org/)
@@ -57,14 +57,15 @@
   - [1] [Solarbeam](https://app.solarbeam.io/exchange/swap)
 - okex:
   - [1] [CherrySwap](https://www.cherryswap.net/)
 - polygon:
   - [1] [QuickSwap](https://quickswap.exchange/)
 - optimism:
   - [1] [Uniswap V3](https://app.uniswap.org/#/swap)
+  - [2] [Velodrome V1](https://app.velodrome.finance/swap)
 
 ---
 
 ## Installation
 
 - Download
 
@@ -132,8 +133,11 @@
 print(eth_weth)
 # {'address': '0xC02aaA39b223FE8D0A0e5C4F27eAD9083C756Cc2', 'name': 'Wrapped ETH', 'symbol': 'WETH'}
 
 ds = ma.get('bsc', 'dex', 'pancake_v2')
 print(ds)
 # {'factory_address': '0xcA143Ce32Fe78f1f7019d7d551a6402fC5350c73', 'name': 'PancakeSwap v2', 'router_address': '0x10ED43C718714eb63d5aA57B78B54704E256024E', 'website': 'https://pancakeswap.finance/swap'}
 
+# print all dex
+ma.print_all_dex()
+
 ```
```

### Comparing `many_abis-0.1.6/many_abis.egg-info/SOURCES.txt` & `many_abis-0.1.6.1/many_abis.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `many_abis-0.1.6/setup.py` & `many_abis-0.1.6.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 # print(find_packages())
 setup(
     name='many_abis',
     packages=['many_abis'],
     package_dir={'many_abis': 'many_abis'},
     package_data={'': [
         '**/*.abi', '**/*.json']},
-    version='0.1.6',
+    version='0.1.6.1',
     license='MIT',
     description='A simple way to get different DEXs abis for block chains.',
     long_description=long_description,
     long_description_content_type="text/markdown",
     author='Yong',
     author_email='ackness8@gmail.com',
     url='https://github.com/ackness/many_abis',
```

