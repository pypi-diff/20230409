# Comparing `tmp/satdigitalinvoice-2.0.6.tar.gz` & `tmp/satdigitalinvoice-2.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "satdigitalinvoice-2.0.6.tar", last modified: Sat Apr  8 23:13:03 2023, max compression
+gzip compressed data, was "satdigitalinvoice-2.0.7.tar", last modified: Sat Apr  8 23:30:51 2023, max compression
```

## Comparing `satdigitalinvoice-2.0.6.tar` & `satdigitalinvoice-2.0.7.tar`

### file list

```diff
@@ -1,39 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 23:13:03.625466 satdigitalinvoice-2.0.6/
--rw-r--r--   0 runner    (1001) docker     (123)     3660 2023-04-08 23:13:03.625466 satdigitalinvoice-2.0.6/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 23:13:03.625466 satdigitalinvoice-2.0.6/satdigitalinvoice/
--rw-r--r--   0 runner    (1001) docker     (123)     2390 2023-04-08 23:12:54.000000 satdigitalinvoice-2.0.6/satdigitalinvoice/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 23:12:54.000000 satdigitalinvoice-2.0.6/satdigitalinvoice/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      674 2023-04-08 23:12:54.000000 satdigitalinvoice-2.0.6/satdigitalinvoice/__version__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2656 2023-04-08 23:12:54.000000 satdigitalinvoice-2.0.6/satdigitalinvoice/client_validation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-04-08 23:12:54.000000 satdigitalinvoice-2.0.6/satdigitalinvoice/environments.py
--rw-r--r--   0 runner    (1001) docker     (123)    30659 2023-04-08 23:12:54.000000 satdigitalinvoice-2.0.6/satdigitalinvoice/facturacion.py
--rw-r--r--   0 runner    (1001) docker     (123)     4814 2023-04-08 23:12:54.000000 satdigitalinvoice-2.0.6/satdigitalinvoice/file_data_managers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 23:13:03.625466 satdigitalinvoice-2.0.6/satdigitalinvoice/formatting_functions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 23:12:54.000000 satdigitalinvoice-2.0.6/satdigitalinvoice/formatting_functions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1333 2023-04-08 23:12:54.000000 satdigitalinvoice-2.0.6/satdigitalinvoice/formatting_functions/common.py
--rw-r--r--   0 runner    (1001) docker     (123)    16430 2023-04-08 23:12:54.000000 satdigitalinvoice-2.0.6/satdigitalinvoice/gui_functions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 23:13:03.625466 satdigitalinvoice-2.0.6/satdigitalinvoice/images/
--rw-r--r--   0 runner    (1001) docker     (123)    71867 2023-04-08 23:12:54.000000 satdigitalinvoice-2.0.6/satdigitalinvoice/images/logo.png
--rw-r--r--   0 runner    (1001) docker     (123)     9439 2023-04-08 23:12:54.000000 satdigitalinvoice-2.0.6/satdigitalinvoice/layout.py
--rw-r--r--   0 runner    (1001) docker     (123)     3606 2023-04-08 23:12:54.000000 satdigitalinvoice-2.0.6/satdigitalinvoice/local.py
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-04-08 23:12:54.000000 satdigitalinvoice-2.0.6/satdigitalinvoice/log_tools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 23:13:03.625466 satdigitalinvoice-2.0.6/satdigitalinvoice/markdown_styles/
--rw-r--r--   0 runner    (1001) docker     (123)     2438 2023-04-08 23:12:54.000000 satdigitalinvoice-2.0.6/satdigitalinvoice/markdown_styles/markdown6.css
--rw-r--r--   0 runner    (1001) docker     (123)     5452 2023-04-08 23:12:54.000000 satdigitalinvoice-2.0.6/satdigitalinvoice/mycfdi.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 23:13:03.625466 satdigitalinvoice-2.0.6/satdigitalinvoice/schemas/
--rw-r--r--   0 runner    (1001) docker     (123)      411 2023-04-08 23:12:54.000000 satdigitalinvoice-2.0.6/satdigitalinvoice/schemas/cliente.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-04-08 23:12:54.000000 satdigitalinvoice-2.0.6/satdigitalinvoice/schemas/config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1565 2023-04-08 23:12:54.000000 satdigitalinvoice-2.0.6/satdigitalinvoice/schemas/factura.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2856 2023-04-08 23:12:54.000000 satdigitalinvoice-2.0.6/satdigitalinvoice/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 23:13:03.625466 satdigitalinvoice-2.0.6/satdigitalinvoice.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3660 2023-04-08 23:13:03.000000 satdigitalinvoice-2.0.6/satdigitalinvoice.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      995 2023-04-08 23:13:03.000000 satdigitalinvoice-2.0.6/satdigitalinvoice.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-08 23:13:03.000000 satdigitalinvoice-2.0.6/satdigitalinvoice.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-04-08 23:13:03.000000 satdigitalinvoice-2.0.6/satdigitalinvoice.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-08 23:13:03.000000 satdigitalinvoice-2.0.6/satdigitalinvoice.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-08 23:13:03.625466 satdigitalinvoice-2.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2118 2023-04-08 23:12:54.000000 satdigitalinvoice-2.0.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 23:13:03.625466 satdigitalinvoice-2.0.6/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-08 23:12:54.000000 satdigitalinvoice-2.0.6/tests/test_clients.py
--rw-r--r--   0 runner    (1001) docker     (123)     4251 2023-04-08 23:12:54.000000 satdigitalinvoice-2.0.6/tests/test_crear_facturas.py
--rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-04-08 23:12:54.000000 satdigitalinvoice-2.0.6/tests/test_main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 23:30:51.611625 satdigitalinvoice-2.0.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     3660 2023-04-08 23:30:51.611625 satdigitalinvoice-2.0.7/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 23:30:51.607625 satdigitalinvoice-2.0.7/satdigitalinvoice/
+-rw-r--r--   0 runner    (1001) docker     (123)     2374 2023-04-08 23:30:42.000000 satdigitalinvoice-2.0.7/satdigitalinvoice/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 23:30:42.000000 satdigitalinvoice-2.0.7/satdigitalinvoice/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      674 2023-04-08 23:30:42.000000 satdigitalinvoice-2.0.7/satdigitalinvoice/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2656 2023-04-08 23:30:42.000000 satdigitalinvoice-2.0.7/satdigitalinvoice/client_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-04-08 23:30:42.000000 satdigitalinvoice-2.0.7/satdigitalinvoice/environments.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30661 2023-04-08 23:30:42.000000 satdigitalinvoice-2.0.7/satdigitalinvoice/facturacion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4814 2023-04-08 23:30:42.000000 satdigitalinvoice-2.0.7/satdigitalinvoice/file_data_managers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 23:30:51.607625 satdigitalinvoice-2.0.7/satdigitalinvoice/formatting_functions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 23:30:42.000000 satdigitalinvoice-2.0.7/satdigitalinvoice/formatting_functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1333 2023-04-08 23:30:42.000000 satdigitalinvoice-2.0.7/satdigitalinvoice/formatting_functions/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16430 2023-04-08 23:30:42.000000 satdigitalinvoice-2.0.7/satdigitalinvoice/gui_functions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 23:30:51.607625 satdigitalinvoice-2.0.7/satdigitalinvoice/images/
+-rw-r--r--   0 runner    (1001) docker     (123)    71867 2023-04-08 23:30:42.000000 satdigitalinvoice-2.0.7/satdigitalinvoice/images/logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)     9439 2023-04-08 23:30:42.000000 satdigitalinvoice-2.0.7/satdigitalinvoice/layout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3618 2023-04-08 23:30:42.000000 satdigitalinvoice-2.0.7/satdigitalinvoice/localdb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-04-08 23:30:42.000000 satdigitalinvoice-2.0.7/satdigitalinvoice/log_tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 23:30:51.607625 satdigitalinvoice-2.0.7/satdigitalinvoice/markdown_styles/
+-rw-r--r--   0 runner    (1001) docker     (123)     2438 2023-04-08 23:30:42.000000 satdigitalinvoice-2.0.7/satdigitalinvoice/markdown_styles/markdown6.css
+-rw-r--r--   0 runner    (1001) docker     (123)     5454 2023-04-08 23:30:42.000000 satdigitalinvoice-2.0.7/satdigitalinvoice/mycfdi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 23:30:51.607625 satdigitalinvoice-2.0.7/satdigitalinvoice/schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-04-08 23:30:42.000000 satdigitalinvoice-2.0.7/satdigitalinvoice/schemas/cliente.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-04-08 23:30:42.000000 satdigitalinvoice-2.0.7/satdigitalinvoice/schemas/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1565 2023-04-08 23:30:42.000000 satdigitalinvoice-2.0.7/satdigitalinvoice/schemas/factura.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2856 2023-04-08 23:30:42.000000 satdigitalinvoice-2.0.7/satdigitalinvoice/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 23:30:51.607625 satdigitalinvoice-2.0.7/satdigitalinvoice.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3660 2023-04-08 23:30:51.000000 satdigitalinvoice-2.0.7/satdigitalinvoice.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-04-08 23:30:51.000000 satdigitalinvoice-2.0.7/satdigitalinvoice.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-08 23:30:51.000000 satdigitalinvoice-2.0.7/satdigitalinvoice.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-04-08 23:30:51.000000 satdigitalinvoice-2.0.7/satdigitalinvoice.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-08 23:30:51.000000 satdigitalinvoice-2.0.7/satdigitalinvoice.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-08 23:30:51.611625 satdigitalinvoice-2.0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2118 2023-04-08 23:30:42.000000 satdigitalinvoice-2.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 23:30:51.611625 satdigitalinvoice-2.0.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-08 23:30:42.000000 satdigitalinvoice-2.0.7/tests/test_clients.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4251 2023-04-08 23:30:42.000000 satdigitalinvoice-2.0.7/tests/test_crear_facturas.py
+-rw-r--r--   0 runner    (1001) docker     (123)      562 2023-04-08 23:30:42.000000 satdigitalinvoice-2.0.7/tests/test_localdb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-04-08 23:30:42.000000 satdigitalinvoice-2.0.7/tests/test_main.py
```

### Comparing `satdigitalinvoice-2.0.6/PKG-INFO` & `satdigitalinvoice-2.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: satdigitalinvoice
-Version: 2.0.6
+Version: 2.0.7
 Summary: GUI APP to Generate CFDI
 Home-page: https://github.com/SAT-CFDI/python-satdigitalinvoice
 Author: satcfdi@outlook.com
 Author-email: satcfdi@outlook.com
 License: MIT License
 Project-URL: Documentation, https://satdigitalinvoice.readthedocs.io
 Project-URL: Source, https://github.com/SAT-CFDI/python-satdigitalinvoice
```

### Comparing `satdigitalinvoice-2.0.6/satdigitalinvoice/__init__.py` & `satdigitalinvoice-2.0.7/satdigitalinvoice/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import logging
 import os
-import traceback
+
 import PySimpleGUI as sg
 
 SOURCE_DIRECTORY = os.path.dirname(__file__)
 DATA_DIRECTORY = ".data"
 
 
 def add_file_handler():
```

### Comparing `satdigitalinvoice-2.0.6/satdigitalinvoice/__version__.py` & `satdigitalinvoice-2.0.7/satdigitalinvoice/__version__.py`

 * *Files identical despite different names*

### Comparing `satdigitalinvoice-2.0.6/satdigitalinvoice/client_validation.py` & `satdigitalinvoice-2.0.7/satdigitalinvoice/client_validation.py`

 * *Files identical despite different names*

### Comparing `satdigitalinvoice-2.0.6/satdigitalinvoice/environments.py` & `satdigitalinvoice-2.0.7/satdigitalinvoice/environments.py`

 * *Files identical despite different names*

### Comparing `satdigitalinvoice-2.0.6/satdigitalinvoice/facturacion.py` & `satdigitalinvoice-2.0.7/satdigitalinvoice/facturacion.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from . import __version__
 from .client_validation import validar_client
 from .file_data_managers import ClientsManager, FacturasManager
 from .gui_functions import generate_ingresos, pago_factura, exportar_facturas, facturas_filename, \
     periodo_desc, generate_html_template, mf_pago_fmt, print_invoices, print_cfdis, print_cfdi_details, ajustes, ajustes_directory
 from .layout import make_layout, ActionButtonManager
-from .local import LocalDBSatCFDI
+from .localdb import LocalDBSatCFDI
 from .log_tools import log_line, log_item, cfdi_header, header_line, print_yaml
 from .mycfdi import get_all_cfdi, MyCFDI, move_to_folder, PPD, PUE
 from .utils import random_string, to_uuid, parse_date_period, parse_ym_date, load_certificate, to_int
 
 logging.getLogger("weasyprint").setLevel(logging.ERROR)
 logging.getLogger("fontTools").setLevel(logging.ERROR)
```

### Comparing `satdigitalinvoice-2.0.6/satdigitalinvoice/file_data_managers.py` & `satdigitalinvoice-2.0.7/satdigitalinvoice/file_data_managers.py`

 * *Files identical despite different names*

### Comparing `satdigitalinvoice-2.0.6/satdigitalinvoice/formatting_functions/common.py` & `satdigitalinvoice-2.0.7/satdigitalinvoice/formatting_functions/common.py`

 * *Files identical despite different names*

### Comparing `satdigitalinvoice-2.0.6/satdigitalinvoice/gui_functions.py` & `satdigitalinvoice-2.0.7/satdigitalinvoice/gui_functions.py`

 * *Files identical despite different names*

### Comparing `satdigitalinvoice-2.0.6/satdigitalinvoice/images/logo.png` & `satdigitalinvoice-2.0.7/satdigitalinvoice/images/logo.png`

 * *Files identical despite different names*

### Comparing `satdigitalinvoice-2.0.6/satdigitalinvoice/layout.py` & `satdigitalinvoice-2.0.7/satdigitalinvoice/layout.py`

 * *Files identical despite different names*

### Comparing `satdigitalinvoice-2.0.6/satdigitalinvoice/local.py` & `satdigitalinvoice-2.0.7/satdigitalinvoice/localdb.py`

 * *Files 2% similar despite different names*

```diff
@@ -121,17 +121,17 @@
             'saldar': self.saldar(cfdi),
             'enviar': self.notificar(cfdi),
             'status_sat': self.status_sat(cfdi)
         })
 
 
 def save_data(file, data):
-    with open(os.path.join(DATA_DIR, file), 'wb') as f:
+    with open(os.path.join(DATA_DIRECTORY, file), 'wb') as f:
         pickle.dump(data, f)
 
 
 def load_data(file, default=None):
     try:
-        with open(os.path.join(DATA_DIR, file), 'rb') as f:
+        with open(os.path.join(DATA_DIRECTORY, file), 'rb') as f:
             return pickle.load(f)
     except FileNotFoundError:
         return default
```

### Comparing `satdigitalinvoice-2.0.6/satdigitalinvoice/log_tools.py` & `satdigitalinvoice-2.0.7/satdigitalinvoice/log_tools.py`

 * *Files identical despite different names*

### Comparing `satdigitalinvoice-2.0.6/satdigitalinvoice/markdown_styles/markdown6.css` & `satdigitalinvoice-2.0.7/satdigitalinvoice/markdown_styles/markdown6.css`

 * *Files identical despite different names*

### Comparing `satdigitalinvoice-2.0.6/satdigitalinvoice/mycfdi.py` & `satdigitalinvoice-2.0.7/satdigitalinvoice/mycfdi.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from collections.abc import Mapping
 from datetime import datetime
 from typing import MutableMapping
 from uuid import UUID
 
 from satcfdi.accounting import complement_invoices_data, SatCFDI
 
-from .local import load_data, save_data
+from .localdb import load_data, save_data
 from .utils import to_uuid
 
 ALL_INVOICES = 'all_invoices'
 ALL_RETENCIONES = 'all_retenciones'
 logger = logging.getLogger(__name__)
 
 PPD = "PPD"
```

### Comparing `satdigitalinvoice-2.0.6/satdigitalinvoice/schemas/factura.yaml` & `satdigitalinvoice-2.0.7/satdigitalinvoice/schemas/factura.yaml`

 * *Files identical despite different names*

### Comparing `satdigitalinvoice-2.0.6/satdigitalinvoice/utils.py` & `satdigitalinvoice-2.0.7/satdigitalinvoice/utils.py`

 * *Files identical despite different names*

### Comparing `satdigitalinvoice-2.0.6/satdigitalinvoice.egg-info/PKG-INFO` & `satdigitalinvoice-2.0.7/satdigitalinvoice.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: satdigitalinvoice
-Version: 2.0.6
+Version: 2.0.7
 Summary: GUI APP to Generate CFDI
 Home-page: https://github.com/SAT-CFDI/python-satdigitalinvoice
 Author: satcfdi@outlook.com
 Author-email: satcfdi@outlook.com
 License: MIT License
 Project-URL: Documentation, https://satdigitalinvoice.readthedocs.io
 Project-URL: Source, https://github.com/SAT-CFDI/python-satdigitalinvoice
```

### Comparing `satdigitalinvoice-2.0.6/satdigitalinvoice.egg-info/SOURCES.txt` & `satdigitalinvoice-2.0.7/satdigitalinvoice.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 satdigitalinvoice/__version__.py
 satdigitalinvoice/client_validation.py
 satdigitalinvoice/environments.py
 satdigitalinvoice/facturacion.py
 satdigitalinvoice/file_data_managers.py
 satdigitalinvoice/gui_functions.py
 satdigitalinvoice/layout.py
-satdigitalinvoice/local.py
+satdigitalinvoice/localdb.py
 satdigitalinvoice/log_tools.py
 satdigitalinvoice/mycfdi.py
 satdigitalinvoice/utils.py
 satdigitalinvoice.egg-info/PKG-INFO
 satdigitalinvoice.egg-info/SOURCES.txt
 satdigitalinvoice.egg-info/dependency_links.txt
 satdigitalinvoice.egg-info/requires.txt
@@ -22,8 +22,9 @@
 satdigitalinvoice/images/logo.png
 satdigitalinvoice/markdown_styles/markdown6.css
 satdigitalinvoice/schemas/cliente.yaml
 satdigitalinvoice/schemas/config.yaml
 satdigitalinvoice/schemas/factura.yaml
 tests/test_clients.py
 tests/test_crear_facturas.py
+tests/test_localdb.py
 tests/test_main.py
```

### Comparing `satdigitalinvoice-2.0.6/setup.py` & `satdigitalinvoice-2.0.7/setup.py`

 * *Files identical despite different names*

### Comparing `satdigitalinvoice-2.0.6/tests/test_crear_facturas.py` & `satdigitalinvoice-2.0.7/tests/test_crear_facturas.py`

 * *Files identical despite different names*

### Comparing `satdigitalinvoice-2.0.6/tests/test_main.py` & `satdigitalinvoice-2.0.7/tests/test_main.py`

 * *Files identical despite different names*

