# Comparing `tmp/adafruit-circuitpython-pn532-2.3.8.tar.gz` & `tmp/adafruit-circuitpython-pn532-2.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafruit-circuitpython-pn532-2.3.8.tar", last modified: Tue Jun  7 17:08:44 2022, max compression
+gzip compressed data, was "adafruit-circuitpython-pn532-2.3.9.tar", last modified: Thu Jun  9 18:28:01 2022, max compression
```

## Comparing `adafruit-circuitpython-pn532-2.3.8.tar` & `adafruit-circuitpython-pn532-2.3.9.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-07 17:08:44.596901 adafruit-circuitpython-pn532-2.3.8/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-07 17:08:44.588900 adafruit-circuitpython-pn532-2.3.8/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-07 17:08:44.592901 adafruit-circuitpython-pn532-2.3.8/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (121)      880 2022-06-07 17:08:31.000000 adafruit-circuitpython-pn532-2.3.8/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-07 17:08:44.592901 adafruit-circuitpython-pn532-2.3.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     2424 2022-06-07 17:08:31.000000 adafruit-circuitpython-pn532-2.3.8/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (121)      479 2022-06-07 17:08:31.000000 adafruit-circuitpython-pn532-2.3.8/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (121)     2714 2022-06-07 17:08:31.000000 adafruit-circuitpython-pn532-2.3.8/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1648 2022-06-07 17:08:31.000000 adafruit-circuitpython-pn532-2.3.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)     1254 2022-06-07 17:08:31.000000 adafruit-circuitpython-pn532-2.3.8/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (121)    16248 2022-06-07 17:08:31.000000 adafruit-circuitpython-pn532-2.3.8/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (121)      388 2022-06-07 17:08:31.000000 adafruit-circuitpython-pn532-2.3.8/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     6147 2022-06-07 17:08:31.000000 adafruit-circuitpython-pn532-2.3.8/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (121)     1098 2022-06-07 17:08:31.000000 adafruit-circuitpython-pn532-2.3.8/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-07 17:08:44.592901 adafruit-circuitpython-pn532-2.3.8/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (121)    16814 2022-06-07 17:08:31.000000 adafruit-circuitpython-pn532-2.3.8/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1108 2022-06-07 17:08:31.000000 adafruit-circuitpython-pn532-2.3.8/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1211 2022-06-07 17:08:31.000000 adafruit-circuitpython-pn532-2.3.8/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (121)     3264 2022-06-07 17:08:44.596901 adafruit-circuitpython-pn532-2.3.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2534 2022-06-07 17:08:31.000000 adafruit-circuitpython-pn532-2.3.8/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)      108 2022-06-07 17:08:31.000000 adafruit-circuitpython-pn532-2.3.8/README.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-07 17:08:44.592901 adafruit-circuitpython-pn532-2.3.8/adafruit_circuitpython_pn532.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3264 2022-06-07 17:08:44.000000 adafruit-circuitpython-pn532-2.3.8/adafruit_circuitpython_pn532.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1119 2022-06-07 17:08:44.000000 adafruit-circuitpython-pn532-2.3.8/adafruit_circuitpython_pn532.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-06-07 17:08:44.000000 adafruit-circuitpython-pn532-2.3.8/adafruit_circuitpython_pn532.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       58 2022-06-07 17:08:44.000000 adafruit-circuitpython-pn532-2.3.8/adafruit_circuitpython_pn532.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       15 2022-06-07 17:08:44.000000 adafruit-circuitpython-pn532-2.3.8/adafruit_circuitpython_pn532.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-07 17:08:44.592901 adafruit-circuitpython-pn532-2.3.8/adafruit_pn532/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-07 17:08:31.000000 adafruit-circuitpython-pn532-2.3.8/adafruit_pn532/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    19802 2022-06-07 17:08:31.000000 adafruit-circuitpython-pn532-2.3.8/adafruit_pn532/adafruit_pn532.py
--rw-r--r--   0 runner    (1001) docker     (121)     3018 2022-06-07 17:08:31.000000 adafruit-circuitpython-pn532-2.3.8/adafruit_pn532/i2c.py
--rw-r--r--   0 runner    (1001) docker     (121)     3764 2022-06-07 17:08:31.000000 adafruit-circuitpython-pn532-2.3.8/adafruit_pn532/spi.py
--rw-r--r--   0 runner    (1001) docker     (121)     2186 2022-06-07 17:08:31.000000 adafruit-circuitpython-pn532-2.3.8/adafruit_pn532/uart.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-07 17:08:44.592901 adafruit-circuitpython-pn532-2.3.8/docs/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-07 17:08:44.592901 adafruit-circuitpython-pn532-2.3.8/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (121)     4414 2022-06-07 17:08:31.000000 adafruit-circuitpython-pn532-2.3.8/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (121)      105 2022-06-07 17:08:31.000000 adafruit-circuitpython-pn532-2.3.8/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (121)      427 2022-06-07 17:08:31.000000 adafruit-circuitpython-pn532-2.3.8/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (121)       96 2022-06-07 17:08:31.000000 adafruit-circuitpython-pn532-2.3.8/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)     5551 2022-06-07 17:08:31.000000 adafruit-circuitpython-pn532-2.3.8/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)      184 2022-06-07 17:08:31.000000 adafruit-circuitpython-pn532-2.3.8/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (121)       96 2022-06-07 17:08:31.000000 adafruit-circuitpython-pn532-2.3.8/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)     1031 2022-06-07 17:08:31.000000 adafruit-circuitpython-pn532-2.3.8/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)       96 2022-06-07 17:08:31.000000 adafruit-circuitpython-pn532-2.3.8/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)      123 2022-06-07 17:08:31.000000 adafruit-circuitpython-pn532-2.3.8/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-07 17:08:44.596901 adafruit-circuitpython-pn532-2.3.8/examples/
--rw-r--r--   0 runner    (1001) docker     (121)     2003 2022-06-07 17:08:31.000000 adafruit-circuitpython-pn532-2.3.8/examples/pn532_low_power.py
--rw-r--r--   0 runner    (1001) docker     (121)     2581 2022-06-07 17:08:31.000000 adafruit-circuitpython-pn532-2.3.8/examples/pn532_readwrite_mifare.py
--rw-r--r--   0 runner    (1001) docker     (121)     2269 2022-06-07 17:08:31.000000 adafruit-circuitpython-pn532-2.3.8/examples/pn532_readwrite_ntag2xx.py
--rw-r--r--   0 runner    (1001) docker     (121)     2322 2022-06-07 17:08:31.000000 adafruit-circuitpython-pn532-2.3.8/examples/pn532_simplelisten.py
--rw-r--r--   0 runner    (1001) docker     (121)     1890 2022-06-07 17:08:31.000000 adafruit-circuitpython-pn532-2.3.8/examples/pn532_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (121)      161 2022-06-07 17:08:31.000000 adafruit-circuitpython-pn532-2.3.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-06-07 17:08:44.596901 adafruit-circuitpython-pn532-2.3.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1887 2022-06-07 17:08:31.000000 adafruit-circuitpython-pn532-2.3.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-09 18:28:01.877530 adafruit-circuitpython-pn532-2.3.9/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-09 18:28:01.873532 adafruit-circuitpython-pn532-2.3.9/.github/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-09 18:28:01.873532 adafruit-circuitpython-pn532-2.3.9/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (121)      880 2022-06-09 18:27:51.000000 adafruit-circuitpython-pn532-2.3.9/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-09 18:28:01.873532 adafruit-circuitpython-pn532-2.3.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (121)     2424 2022-06-09 18:27:51.000000 adafruit-circuitpython-pn532-2.3.9/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (121)      479 2022-06-09 18:27:51.000000 adafruit-circuitpython-pn532-2.3.9/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     2714 2022-06-09 18:27:51.000000 adafruit-circuitpython-pn532-2.3.9/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     1648 2022-06-09 18:27:51.000000 adafruit-circuitpython-pn532-2.3.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (121)     1254 2022-06-09 18:27:51.000000 adafruit-circuitpython-pn532-2.3.9/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)    16248 2022-06-09 18:27:51.000000 adafruit-circuitpython-pn532-2.3.9/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (121)      388 2022-06-09 18:27:51.000000 adafruit-circuitpython-pn532-2.3.9/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)     6147 2022-06-09 18:27:51.000000 adafruit-circuitpython-pn532-2.3.9/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (121)     1098 2022-06-09 18:27:51.000000 adafruit-circuitpython-pn532-2.3.9/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-09 18:28:01.873532 adafruit-circuitpython-pn532-2.3.9/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (121)    16814 2022-06-09 18:27:51.000000 adafruit-circuitpython-pn532-2.3.9/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1108 2022-06-09 18:27:51.000000 adafruit-circuitpython-pn532-2.3.9/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1211 2022-06-09 18:27:51.000000 adafruit-circuitpython-pn532-2.3.9/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     3264 2022-06-09 18:28:01.877530 adafruit-circuitpython-pn532-2.3.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     2534 2022-06-09 18:27:51.000000 adafruit-circuitpython-pn532-2.3.9/README.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      108 2022-06-09 18:27:51.000000 adafruit-circuitpython-pn532-2.3.9/README.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-09 18:28:01.873532 adafruit-circuitpython-pn532-2.3.9/adafruit_circuitpython_pn532.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     3264 2022-06-09 18:28:01.000000 adafruit-circuitpython-pn532-2.3.9/adafruit_circuitpython_pn532.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     1119 2022-06-09 18:28:01.000000 adafruit-circuitpython-pn532-2.3.9/adafruit_circuitpython_pn532.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-06-09 18:28:01.000000 adafruit-circuitpython-pn532-2.3.9/adafruit_circuitpython_pn532.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       58 2022-06-09 18:28:01.000000 adafruit-circuitpython-pn532-2.3.9/adafruit_circuitpython_pn532.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       15 2022-06-09 18:28:01.000000 adafruit-circuitpython-pn532-2.3.9/adafruit_circuitpython_pn532.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-09 18:28:01.873532 adafruit-circuitpython-pn532-2.3.9/adafruit_pn532/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-09 18:27:51.000000 adafruit-circuitpython-pn532-2.3.9/adafruit_pn532/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    19802 2022-06-09 18:27:51.000000 adafruit-circuitpython-pn532-2.3.9/adafruit_pn532/adafruit_pn532.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3018 2022-06-09 18:27:51.000000 adafruit-circuitpython-pn532-2.3.9/adafruit_pn532/i2c.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3764 2022-06-09 18:27:51.000000 adafruit-circuitpython-pn532-2.3.9/adafruit_pn532/spi.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2186 2022-06-09 18:27:51.000000 adafruit-circuitpython-pn532-2.3.9/adafruit_pn532/uart.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-09 18:28:01.877530 adafruit-circuitpython-pn532-2.3.9/docs/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-09 18:28:01.877530 adafruit-circuitpython-pn532-2.3.9/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (121)     4414 2022-06-09 18:27:51.000000 adafruit-circuitpython-pn532-2.3.9/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (121)      105 2022-06-09 18:27:51.000000 adafruit-circuitpython-pn532-2.3.9/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (121)      427 2022-06-09 18:27:51.000000 adafruit-circuitpython-pn532-2.3.9/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       96 2022-06-09 18:27:51.000000 adafruit-circuitpython-pn532-2.3.9/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (121)     5551 2022-06-09 18:27:51.000000 adafruit-circuitpython-pn532-2.3.9/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (121)      184 2022-06-09 18:27:51.000000 adafruit-circuitpython-pn532-2.3.9/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       96 2022-06-09 18:27:51.000000 adafruit-circuitpython-pn532-2.3.9/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (121)     1109 2022-06-09 18:27:51.000000 adafruit-circuitpython-pn532-2.3.9/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       96 2022-06-09 18:27:51.000000 adafruit-circuitpython-pn532-2.3.9/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (121)      123 2022-06-09 18:27:51.000000 adafruit-circuitpython-pn532-2.3.9/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-09 18:28:01.877530 adafruit-circuitpython-pn532-2.3.9/examples/
+-rw-r--r--   0 runner    (1001) docker     (121)     2003 2022-06-09 18:27:51.000000 adafruit-circuitpython-pn532-2.3.9/examples/pn532_low_power.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2581 2022-06-09 18:27:51.000000 adafruit-circuitpython-pn532-2.3.9/examples/pn532_readwrite_mifare.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2269 2022-06-09 18:27:51.000000 adafruit-circuitpython-pn532-2.3.9/examples/pn532_readwrite_ntag2xx.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2322 2022-06-09 18:27:51.000000 adafruit-circuitpython-pn532-2.3.9/examples/pn532_simplelisten.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1890 2022-06-09 18:27:51.000000 adafruit-circuitpython-pn532-2.3.9/examples/pn532_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (121)      161 2022-06-09 18:27:51.000000 adafruit-circuitpython-pn532-2.3.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-06-09 18:28:01.877530 adafruit-circuitpython-pn532-2.3.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     1887 2022-06-09 18:27:51.000000 adafruit-circuitpython-pn532-2.3.9/setup.py
```

### Comparing `adafruit-circuitpython-pn532-2.3.8/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `adafruit-circuitpython-pn532-2.3.9/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pn532-2.3.8/.github/workflows/build.yml` & `adafruit-circuitpython-pn532-2.3.9/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pn532-2.3.8/.github/workflows/release.yml` & `adafruit-circuitpython-pn532-2.3.9/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pn532-2.3.8/.gitignore` & `adafruit-circuitpython-pn532-2.3.9/.gitignore`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pn532-2.3.8/.pre-commit-config.yaml` & `adafruit-circuitpython-pn532-2.3.9/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pn532-2.3.8/.pylintrc` & `adafruit-circuitpython-pn532-2.3.9/.pylintrc`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pn532-2.3.8/CODE_OF_CONDUCT.md` & `adafruit-circuitpython-pn532-2.3.9/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pn532-2.3.8/LICENSE` & `adafruit-circuitpython-pn532-2.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pn532-2.3.8/LICENSES/CC-BY-4.0.txt` & `adafruit-circuitpython-pn532-2.3.9/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pn532-2.3.8/LICENSES/MIT.txt` & `adafruit-circuitpython-pn532-2.3.9/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pn532-2.3.8/LICENSES/Unlicense.txt` & `adafruit-circuitpython-pn532-2.3.9/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pn532-2.3.8/PKG-INFO` & `adafruit-circuitpython-pn532-2.3.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-pn532
-Version: 2.3.8
+Version: 2.3.9
 Summary: CircuitPython library for controlling PN532 RFID/NFC reader-writer.
 Home-page: https://github.com/adafruit/Adafruit_CircuitPython_PN532
 Author: Adafruit Industries
 Author-email: circuitpython@adafruit.com
 License: MIT
 Keywords: adafruit pn532 rfid nfc hardware micropython circuitpython
 Platform: UNKNOWN
```

### Comparing `adafruit-circuitpython-pn532-2.3.8/README.rst` & `adafruit-circuitpython-pn532-2.3.9/README.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pn532-2.3.8/adafruit_circuitpython_pn532.egg-info/PKG-INFO` & `adafruit-circuitpython-pn532-2.3.9/adafruit_circuitpython_pn532.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-pn532
-Version: 2.3.8
+Version: 2.3.9
 Summary: CircuitPython library for controlling PN532 RFID/NFC reader-writer.
 Home-page: https://github.com/adafruit/Adafruit_CircuitPython_PN532
 Author: Adafruit Industries
 Author-email: circuitpython@adafruit.com
 License: MIT
 Keywords: adafruit pn532 rfid nfc hardware micropython circuitpython
 Platform: UNKNOWN
```

### Comparing `adafruit-circuitpython-pn532-2.3.8/adafruit_circuitpython_pn532.egg-info/SOURCES.txt` & `adafruit-circuitpython-pn532-2.3.9/adafruit_circuitpython_pn532.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pn532-2.3.8/adafruit_pn532/adafruit_pn532.py` & `adafruit-circuitpython-pn532-2.3.9/adafruit_pn532/adafruit_pn532.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pn532-2.3.8/adafruit_pn532/i2c.py` & `adafruit-circuitpython-pn532-2.3.9/adafruit_pn532/i2c.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pn532-2.3.8/adafruit_pn532/spi.py` & `adafruit-circuitpython-pn532-2.3.9/adafruit_pn532/spi.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pn532-2.3.8/adafruit_pn532/uart.py` & `adafruit-circuitpython-pn532-2.3.9/adafruit_pn532/uart.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pn532-2.3.8/docs/_static/favicon.ico` & `adafruit-circuitpython-pn532-2.3.9/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pn532-2.3.8/docs/conf.py` & `adafruit-circuitpython-pn532-2.3.9/docs/conf.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pn532-2.3.8/docs/index.rst` & `adafruit-circuitpython-pn532-2.3.9/docs/index.rst`

 * *Files 10% similar despite different names*

```diff
@@ -28,15 +28,16 @@
 
     `PN532 NFC/RFID Breakout <https://www.adafruit.com/product/364>` and `PN532 NFC/RFID Shield <https://www.adafruit.com/product/789>`_
 
 
 .. toctree::
     :caption: Other Links
 
-    Download <https://github.com/adafruit/adafruit_CircuitPython_PN532/releases/latest>
+    Download from GitHub <https://github.com/adafruit/adafruit_CircuitPython_PN532/releases/latest>
+    Download Library Bundle <https://circuitpython.org/libraries>
     CircuitPython Reference Documentation <https://docs.circuitpython.org>
     CircuitPython Support Forum <https://forums.adafruit.com/viewforum.php?f=60>
     Discord Chat <https://adafru.it/discord>
     Adafruit Learning System <https://learn.adafruit.com>
     Adafruit Blog <https://blog.adafruit.com>
     Adafruit Store <https://www.adafruit.com>
```

### Comparing `adafruit-circuitpython-pn532-2.3.8/examples/pn532_low_power.py` & `adafruit-circuitpython-pn532-2.3.9/examples/pn532_low_power.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pn532-2.3.8/examples/pn532_readwrite_mifare.py` & `adafruit-circuitpython-pn532-2.3.9/examples/pn532_readwrite_mifare.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pn532-2.3.8/examples/pn532_readwrite_ntag2xx.py` & `adafruit-circuitpython-pn532-2.3.9/examples/pn532_readwrite_ntag2xx.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pn532-2.3.8/examples/pn532_simplelisten.py` & `adafruit-circuitpython-pn532-2.3.9/examples/pn532_simplelisten.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pn532-2.3.8/examples/pn532_simpletest.py` & `adafruit-circuitpython-pn532-2.3.9/examples/pn532_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pn532-2.3.8/setup.py` & `adafruit-circuitpython-pn532-2.3.9/setup.py`

 * *Files identical despite different names*

