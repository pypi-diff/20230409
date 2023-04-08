# Comparing `tmp/satdigitalinvoice-2.0.4.tar.gz` & `tmp/satdigitalinvoice-2.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "satdigitalinvoice-2.0.4.tar", last modified: Tue Apr  4 19:44:53 2023, max compression
+gzip compressed data, was "satdigitalinvoice-2.0.5.tar", last modified: Sat Apr  8 22:57:20 2023, max compression
```

## Comparing `satdigitalinvoice-2.0.4.tar` & `satdigitalinvoice-2.0.5.tar`

### file list

```diff
@@ -1,42 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 19:44:53.222828 satdigitalinvoice-2.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)     3660 2023-04-04 19:44:53.222828 satdigitalinvoice-2.0.4/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 19:44:53.218828 satdigitalinvoice-2.0.4/satdigitalinvoice/
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-04-04 19:44:42.000000 satdigitalinvoice-2.0.4/satdigitalinvoice/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    33247 2023-04-04 19:44:42.000000 satdigitalinvoice-2.0.4/satdigitalinvoice/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      674 2023-04-04 19:44:42.000000 satdigitalinvoice-2.0.4/satdigitalinvoice/__version__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2656 2023-04-04 19:44:42.000000 satdigitalinvoice-2.0.4/satdigitalinvoice/client_validation.py
--rw-r--r--   0 runner    (1001) docker     (123)     5346 2023-04-04 19:44:42.000000 satdigitalinvoice-2.0.4/satdigitalinvoice/file_data_managers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 19:44:53.218828 satdigitalinvoice-2.0.4/satdigitalinvoice/formatting_functions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-04 19:44:42.000000 satdigitalinvoice-2.0.4/satdigitalinvoice/formatting_functions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1352 2023-04-04 19:44:42.000000 satdigitalinvoice-2.0.4/satdigitalinvoice/formatting_functions/common.py
--rw-r--r--   0 runner    (1001) docker     (123)    10271 2023-04-04 19:44:42.000000 satdigitalinvoice-2.0.4/satdigitalinvoice/gui_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     6064 2023-04-04 19:44:42.000000 satdigitalinvoice-2.0.4/satdigitalinvoice/layout.py
--rw-r--r--   0 runner    (1001) docker     (123)     3627 2023-04-04 19:44:42.000000 satdigitalinvoice-2.0.4/satdigitalinvoice/local.py
--rw-r--r--   0 runner    (1001) docker     (123)      958 2023-04-04 19:44:42.000000 satdigitalinvoice-2.0.4/satdigitalinvoice/log_tools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 19:44:53.218828 satdigitalinvoice-2.0.4/satdigitalinvoice/markdown_styles/
--rw-r--r--   0 runner    (1001) docker     (123)     2438 2023-04-04 19:44:42.000000 satdigitalinvoice-2.0.4/satdigitalinvoice/markdown_styles/markdown6.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 19:44:53.218828 satdigitalinvoice-2.0.4/satdigitalinvoice/microsoft_auth/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-04 19:44:42.000000 satdigitalinvoice-2.0.4/satdigitalinvoice/microsoft_auth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5402 2023-04-04 19:44:42.000000 satdigitalinvoice-2.0.4/satdigitalinvoice/microsoft_auth/auth_code_receiver.py
--rw-r--r--   0 runner    (1001) docker     (123)     2267 2023-04-04 19:44:42.000000 satdigitalinvoice-2.0.4/satdigitalinvoice/microsoft_auth/cache_interactive_browser.py
--rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-04-04 19:44:42.000000 satdigitalinvoice-2.0.4/satdigitalinvoice/microsoft_auth/cache_secret_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2319 2023-04-04 19:44:42.000000 satdigitalinvoice-2.0.4/satdigitalinvoice/microsoft_auth/jwt_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     3525 2023-04-04 19:44:42.000000 satdigitalinvoice-2.0.4/satdigitalinvoice/microsoft_auth/microsoft_oauth2.py
--rw-r--r--   0 runner    (1001) docker     (123)     6469 2023-04-04 19:44:42.000000 satdigitalinvoice-2.0.4/satdigitalinvoice/mycfdi.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 19:44:53.218828 satdigitalinvoice-2.0.4/satdigitalinvoice/schemas/
--rw-r--r--   0 runner    (1001) docker     (123)      411 2023-04-04 19:44:42.000000 satdigitalinvoice-2.0.4/satdigitalinvoice/schemas/client.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1542 2023-04-04 19:44:42.000000 satdigitalinvoice-2.0.4/satdigitalinvoice/schemas/factura.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-04-04 19:44:42.000000 satdigitalinvoice-2.0.4/satdigitalinvoice/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 19:44:53.218828 satdigitalinvoice-2.0.4/satdigitalinvoice.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3660 2023-04-04 19:44:53.000000 satdigitalinvoice-2.0.4/satdigitalinvoice.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-04-04 19:44:53.000000 satdigitalinvoice-2.0.4/satdigitalinvoice.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-04 19:44:53.000000 satdigitalinvoice-2.0.4/satdigitalinvoice.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-04-04 19:44:53.000000 satdigitalinvoice-2.0.4/satdigitalinvoice.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-04 19:44:53.000000 satdigitalinvoice-2.0.4/satdigitalinvoice.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-04 19:44:53.222828 satdigitalinvoice-2.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2147 2023-04-04 19:44:42.000000 satdigitalinvoice-2.0.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 19:44:53.222828 satdigitalinvoice-2.0.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-04 19:44:42.000000 satdigitalinvoice-2.0.4/tests/test_clients.py
--rw-r--r--   0 runner    (1001) docker     (123)     3589 2023-04-04 19:44:42.000000 satdigitalinvoice-2.0.4/tests/test_crear_facturas.py
--rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-04-04 19:44:42.000000 satdigitalinvoice-2.0.4/tests/test_main.py
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-04-04 19:44:42.000000 satdigitalinvoice-2.0.4/tests/test_microsoft_auth.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 22:57:20.511503 satdigitalinvoice-2.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     3660 2023-04-08 22:57:20.511503 satdigitalinvoice-2.0.5/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 22:57:20.511503 satdigitalinvoice-2.0.5/satdigitalinvoice/
+-rw-r--r--   0 runner    (1001) docker     (123)     2390 2023-04-08 22:57:11.000000 satdigitalinvoice-2.0.5/satdigitalinvoice/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 22:57:11.000000 satdigitalinvoice-2.0.5/satdigitalinvoice/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      674 2023-04-08 22:57:11.000000 satdigitalinvoice-2.0.5/satdigitalinvoice/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2656 2023-04-08 22:57:11.000000 satdigitalinvoice-2.0.5/satdigitalinvoice/client_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-04-08 22:57:11.000000 satdigitalinvoice-2.0.5/satdigitalinvoice/environments.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30659 2023-04-08 22:57:11.000000 satdigitalinvoice-2.0.5/satdigitalinvoice/facturacion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4814 2023-04-08 22:57:11.000000 satdigitalinvoice-2.0.5/satdigitalinvoice/file_data_managers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 22:57:20.511503 satdigitalinvoice-2.0.5/satdigitalinvoice/formatting_functions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 22:57:11.000000 satdigitalinvoice-2.0.5/satdigitalinvoice/formatting_functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1352 2023-04-08 22:57:11.000000 satdigitalinvoice-2.0.5/satdigitalinvoice/formatting_functions/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16483 2023-04-08 22:57:11.000000 satdigitalinvoice-2.0.5/satdigitalinvoice/gui_functions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 22:57:20.511503 satdigitalinvoice-2.0.5/satdigitalinvoice/images/
+-rw-r--r--   0 runner    (1001) docker     (123)    71867 2023-04-08 22:57:11.000000 satdigitalinvoice-2.0.5/satdigitalinvoice/images/logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)     9439 2023-04-08 22:57:11.000000 satdigitalinvoice-2.0.5/satdigitalinvoice/layout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3606 2023-04-08 22:57:11.000000 satdigitalinvoice-2.0.5/satdigitalinvoice/local.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-04-08 22:57:11.000000 satdigitalinvoice-2.0.5/satdigitalinvoice/log_tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 22:57:20.511503 satdigitalinvoice-2.0.5/satdigitalinvoice/markdown_styles/
+-rw-r--r--   0 runner    (1001) docker     (123)     2438 2023-04-08 22:57:11.000000 satdigitalinvoice-2.0.5/satdigitalinvoice/markdown_styles/markdown6.css
+-rw-r--r--   0 runner    (1001) docker     (123)     5452 2023-04-08 22:57:11.000000 satdigitalinvoice-2.0.5/satdigitalinvoice/mycfdi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 22:57:20.511503 satdigitalinvoice-2.0.5/satdigitalinvoice/schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-04-08 22:57:11.000000 satdigitalinvoice-2.0.5/satdigitalinvoice/schemas/cliente.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-04-08 22:57:11.000000 satdigitalinvoice-2.0.5/satdigitalinvoice/schemas/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1565 2023-04-08 22:57:11.000000 satdigitalinvoice-2.0.5/satdigitalinvoice/schemas/factura.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2742 2023-04-08 22:57:11.000000 satdigitalinvoice-2.0.5/satdigitalinvoice/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 22:57:20.511503 satdigitalinvoice-2.0.5/satdigitalinvoice.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3660 2023-04-08 22:57:20.000000 satdigitalinvoice-2.0.5/satdigitalinvoice.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      995 2023-04-08 22:57:20.000000 satdigitalinvoice-2.0.5/satdigitalinvoice.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-08 22:57:20.000000 satdigitalinvoice-2.0.5/satdigitalinvoice.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-04-08 22:57:20.000000 satdigitalinvoice-2.0.5/satdigitalinvoice.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-08 22:57:20.000000 satdigitalinvoice-2.0.5/satdigitalinvoice.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-08 22:57:20.511503 satdigitalinvoice-2.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2171 2023-04-08 22:57:11.000000 satdigitalinvoice-2.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 22:57:20.511503 satdigitalinvoice-2.0.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-08 22:57:11.000000 satdigitalinvoice-2.0.5/tests/test_clients.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4251 2023-04-08 22:57:11.000000 satdigitalinvoice-2.0.5/tests/test_crear_facturas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-04-08 22:57:11.000000 satdigitalinvoice-2.0.5/tests/test_main.py
```

### Comparing `satdigitalinvoice-2.0.4/PKG-INFO` & `satdigitalinvoice-2.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: satdigitalinvoice
-Version: 2.0.4
+Version: 2.0.5
 Summary: GUI APP to Generate CFDI
 Home-page: https://github.com/SAT-CFDI/python-satdigitalinvoice
 Author: satcfdi@outlook.com
 Author-email: satcfdi@outlook.com
 License: MIT License
 Project-URL: Documentation, https://satdigitalinvoice.readthedocs.io
 Project-URL: Source, https://github.com/SAT-CFDI/python-satdigitalinvoice
```

### Comparing `satdigitalinvoice-2.0.4/satdigitalinvoice/__main__.py` & `satdigitalinvoice-2.0.5/satdigitalinvoice/facturacion.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,141 +1,140 @@
 import base64
 import io
 import itertools
 import logging
 import os
-import shutil
 from datetime import timedelta, date
-from decimal import Decimal
 from zipfile import ZipFile
 
 from PySimpleGUI import POPUP_BUTTONS_OK_CANCEL, PySimpleGUI
-from markdown2 import markdown
-from satcfdi import DatePeriod, CFDI, Code, Signer
-from satcfdi.accounting import filter_invoices_iter, SatCFDI
+from satcfdi import DatePeriod
+from satcfdi.accounting import EmailManager
 from satcfdi.exceptions import ResponseError, DocumentNotFoundError
 from satcfdi.pacs import Accept
 from satcfdi.pacs.sat import SAT, TipoDescargaMasivaTerceros, EstadoSolicitud
 from satcfdi.printer import Representable
 # noinspection PyUnresolvedReferences
 from satcfdi.transform.catalog import CATALOGS
-from weasyprint import HTML, CSS
+from tabulate import tabulate
 
-from . import SOURCE_DIRECTORY, __version__
+from . import __version__
 from .client_validation import validar_client
-from .file_data_managers import environment_default, environment_bold_escaped, ClientsManager, ConfigManager, FacturasManager
-from .formatting_functions.common import fecha, pesos, porcentaje
-from .gui_functions import generate_ingresos, pago_factura, find_ajustes, format_concepto_desc, exportar_facturas, exportar_facturas_filename, parse_ym_date, parse_date_period
-from .layout import make_layout, InvoiceButtonManager, EmailButtonManager
+from .file_data_managers import ClientsManager, FacturasManager
+from .gui_functions import generate_ingresos, pago_factura, exportar_facturas, facturas_filename, \
+    periodo_desc, generate_html_template, mf_pago_fmt, print_invoices, print_cfdis, print_cfdi_details, ajustes, ajustes_directory
+from .layout import make_layout, ActionButtonManager
 from .local import LocalDBSatCFDI
-from .log_tools import log_line, log_item, cfdi_header, print_yaml, header_line
+from .log_tools import log_line, log_item, cfdi_header, header_line, print_yaml
 from .mycfdi import get_all_cfdi, MyCFDI, move_to_folder, PPD, PUE
-from .utils import random_string, to_uuid, add_file_handler
+from .utils import random_string, to_uuid, parse_date_period, parse_ym_date, load_certificate, to_int
 
 logging.getLogger("weasyprint").setLevel(logging.ERROR)
 logging.getLogger("fontTools").setLevel(logging.ERROR)
 
 logger = logging.getLogger(__name__)
 logger.setLevel(logging.INFO)
 
-AJUSTES_DIR = "ajustes"
-template = environment_default.get_template(
-    'mail_facturas_template.html'
-)
+ACTION_FACTURAS = "facturas"
+ACTION_EMAILS = "emails"
+ACTION_CLIENTS = "clients"
+ACTION_AJUSTES = "ajustes"
+
+
+def open_launch_window():
+    layout = [[PySimpleGUI.Text("New Window", key="new")]]
+    window = PySimpleGUI.Window("Launch Window", layout, modal=True, size=(300, 300))
+    window.read(timeout=1000)
+
+    return window
 
 
 class FacturacionGUI:
-    def __init__(self, pac_service, csd_signer: Signer, email_manager, fiel_signer=None, debug=False):
-        # set up logging
-        if debug:
-            logging.basicConfig(level=logging.ERROR)
-        add_file_handler()
-
-        self.email_manager = email_manager
-        self.pac_service = pac_service
-        self.sat_service = SAT(
-            signer=fiel_signer
+    def __init__(self, config):
+        self.email_manager = EmailManager(
+            **config['email']
+        )
+        pac = config['pac']
+        pac_module, pac_class = pac['type'].split(".")
+        mod = __import__(f"satcfdi.pacs.{pac_module}", fromlist=[pac_class])
+        self.pac_service = getattr(mod, pac_class)(
+            **pac['args']
         )
-        self.csd_signer = csd_signer
+        self.serie = config['serie']
+        self.csd_signer = load_certificate(config.get('csd')) if 'csd' in config else None
+        self.fiel_signer = load_certificate(config.get('fiel')) if 'fiel' in config else None
+
+        self.sat_service = SAT(signer=self.fiel_signer)
+        self.rfc_prediales = config['rfc_prediales']
 
         self.window = PySimpleGUI.Window(
-            f"Facturacion 4.0",
-            make_layout(fiel_signer is not None),
+            f"Facturación Masiva CFDI 4.0 {self.csd_signer.rfc}",
+            make_layout(True),
             size=(1280, 800),
             resizable=True,
+            font=("Courier New", 10, "bold"),
         )
 
         self.all_invoices = None
-        self.config = None
-        self.local_db = None
+        self.local_db = LocalDBSatCFDI(
+            enviar_a_partir=config['enviar_a_partir'],
+            saldar_a_partir=config['saldar_a_partir']
+        )
+        # noinspection PyTypeChecker
+        self.selected_satcfdi = None  # type: MyCFDI
 
-        self.invoice_button_manager = InvoiceButtonManager(self.window["crear_facturas"], self.window["detallado"])
-        self.email_button_manager = EmailButtonManager(self.window["enviar_correos"])
+        self.action_button_manager = ActionButtonManager(self.window["crear_facturas"])
         self.console = self.window["console"]
 
-    def prepare(self):
-        self.config = ConfigManager()
-        self.local_db = LocalDBSatCFDI(self.config)
-
-        MyCFDI.issuer_rfc = self.csd_signer.rfc
         MyCFDI.local_db = self.local_db
 
-        # update window title
-        self.window.set_title(
-            f"Facturación Masiva CFDI 4.0  RFC: {self.csd_signer.rfc}"
-        )
+    def run(self):
+        self.window.finalize()
+
+        self.set_folio()
+        self.window['serie'].update(self.serie)
+
+        self.window['factura_pagar'].bind("<Return>", "_enter")
+        self.window['periodo'].bind("<Return>", "_enter")
+        self.window['importe_pago'].bind("<Return>", "_enter")
+        self.window['fecha_pago'].bind("<Return>", "_enter")
+        self.window['inicio'].bind("<Return>", "_enter")
+        self.window['final'].bind("<Return>", "_enter")
+        self.window['forma_pago'].bind("<Return>", "_enter")
+        # self.window['console'].bind('<Button-3>', '_double_click')
+
+        # Add logging to the window
+        h = logging.StreamHandler(self.window['console'])
+        h.setLevel(logging.INFO)
+        logging.root.addHandler(h)
+
+        self.main_loop()
+        self.window.close()
 
     def initial_screen(self, emisor_cif):
+        log_line("Acerca De")
         print_yaml({
             "version": __version__.__version__,
             "facturacion": "CFDI 4.0",
             "emisor": emisor_cif,
             "pac_service": {
                 "Type": type(self.pac_service).__name__,
                 "Rfc": self.pac_service.RFC,
                 "Environment": str(self.pac_service.environment)
             }
         })
 
-    def start(self):
-        self.window.finalize()
-
-        # Add logging to the window
-        h = logging.StreamHandler(self.window['console'])
-        h.setLevel(logging.INFO)
-        logger.addHandler(h)
-
-        try:
-            self.prepare()
-            clients = ClientsManager()
-            emisor_cif = clients[self.csd_signer.rfc]
-            self.initial_screen(emisor_cif)
-        except Exception:
-            logger.exception(header_line("ERROR"))
-            for e in self.window.element_list():
-                if isinstance(e, PySimpleGUI.Button):
-                    e.update(disabled=True)
-                if isinstance(e, PySimpleGUI.Input):
-                    e.update("", disabled=True)
-            self.window.read()
-            self.window.close()
-            return
-
-        self.main_loop()
-        self.window.close()
-
     def get_all_invoices(self):
         if self.all_invoices:
             return self.all_invoices
         self.all_invoices = get_all_cfdi()
         return self.all_invoices
 
     def generate_invoice(self, invoice):
         ref_id = random_string()
-
         attempts = 3
         for i in range(attempts):
             if i:
                 print(f'Intentando de nuevo... Intento {i + 1} de {attempts}')
                 self._read(timeout=2000 * i)
 
             try:
@@ -147,46 +146,50 @@
             except Exception as ex:
                 logger.error(f"Error Generando: {invoice.get('Serie')}{invoice.get('Folio')} {invoice['Receptor']['Rfc']}")
                 if isinstance(ex, ResponseError):
                     logger.error(f"Status Code: {ex.response.status_code}")
                     logger.error(f"Response: {ex.response.text}")
                 continue
 
-            self.config.inc_folio()
+            self.set_folio(int(res['Folio']) + 1)
             return move_to_folder(res.xml, pdf_data=res.pdf)
 
+    def set_folio(self, folio: int = None):
+        if folio:
+            self.local_db.folio_set(folio)
+            self.window['folio'].update(folio)
+        else:
+            self.window['folio'].update(self.local_db.folio())
+
     def enviar_correos(self, emisor_cif, emails):
         with self.email_manager.sender as s:
             for receptor, notify_invoices, pendientes_meses_anteriores in emails:
                 attachments = []
                 for r in notify_invoices:
                     attachments += [r.filename + ".xml", r.filename + ".pdf"]
 
                 subject = f"Comprobantes Fiscales {receptor['RazonSocial']} - {receptor['Rfc']}"
                 s.send_email(
                     subject=subject,
                     to_addrs=receptor["Email"],
-                    html=self.generate_html_template(
+                    html=generate_html_template(
                         'mail_facturas_template.html',
                         fields={
                             "facturas": notify_invoices,
                             'pendientes_meses_anteriores': pendientes_meses_anteriores,
                             'emisor': emisor_cif,
                         },
                     ),
                     file_attachments=attachments
                 )
                 for r in notify_invoices:
-                    r.notified = True
-
+                    self.local_db.notificar_set(r.uuid, False)
                 print_yaml({
-                    "correo_enviado": subject,
-                    'facturas': [f"{i.name} - {i.uuid}" for i in notify_invoices],
-                    'pendientes_meses_anteriores': [f"{i.name} - {i.uuid}" for i in pendientes_meses_anteriores],
-                    "correos": receptor["Email"]
+                    "correo": subject,
+                    "para": receptor["Email"]
                 })
                 self._read()
 
     def recupera_comprobantes(self, id_solicitud):
         response = self.sat_service.recover_comprobante_status(
             id_solicitud=id_solicitud
         )
@@ -209,517 +212,479 @@
                 self._read()
 
     def _read(self, timeout=0):
         event, values = self.window.read(timeout=timeout)
         if event in ("Exit", PySimpleGUI.WIN_CLOSED):
             exit(0)
 
-    def generate_pdf_template(self, template_name, fields):
-        increment_template = environment_bold_escaped.get_template(template_name)
-        md5_document = increment_template.render(
-            fecha_hoy=fecha(date.today()),
-            **fields
-        )
-        html = markdown(md5_document)
-        pdf = HTML(string=html).write_pdf(
-            target=None,
-            stylesheets=[
-                os.path.join(SOURCE_DIRECTORY, "markdown_styles", "markdown6.css"),
-                CSS(
-                    string='@page { width: Letter; margin: 1.6cm 1.6cm 1.6cm 1.6cm; }'
-                )
-            ]
-        )
-        return pdf
-
-    def generate_html_template(self, template_name, fields):
-        increment_template = environment_default.get_template(template_name)
-        render = increment_template.render(
-            fields
-        )
-        return render
-
-    def factura_uuid(self, text):
-        return self.get_all_invoices().get(to_uuid(text))
-
-    def factura_buscar(self, text):
-        if text:
-            emisor_rfc = self.csd_signer.rfc
-            res = None
-            for i in self.get_all_invoices().values():
-                if i.name == text and i["Emisor"]["Rfc"] == emisor_rfc:
-                    logger.info(f"Factura Encontrada: {i['Receptor']['Rfc']}  {i.name}  {i.uuid}  {i['Fecha']}")
-                    if res:
-                        logger.info(f"Multiples Facturas Encontradas con el mismo nombre: {text}")
-                        return
-                    res = i
-            if res:
-                return res
-        logger.info(f"Factura No Encontrada {text}")
-
-    def log_cfdi(self, cfdi: CFDI, ver_saldo=True):
-        cfdi_copy = cfdi.copy()
-        del cfdi_copy["Certificado"]
-        del cfdi_copy["Sello"]
-
-        if not self.window['detallado'].get():
-            del cfdi_copy["Serie"]
-            del cfdi_copy["NoCertificado"]
-            cfdi_copy.pop("Emisor")
-            cfdi_copy["Receptor"] = f"{cfdi_copy['Receptor']['Rfc']}, {cfdi_copy['Receptor']['Nombre']}, {cfdi_copy['Receptor'].get('RegimenFiscalReceptor')}"
-            cfdi_copy["Conceptos"] = [x['Descripcion'] for x in cfdi_copy["Conceptos"]]  # f"<< {len(cfdi_copy['Conceptos'])} >>"
-            cfdi_copy.pop("Impuestos", None)
-            cfdi_copy.pop("Fecha")
-            cfdi_copy.pop("LugarExpedicion")
-            cfdi_copy.pop("Version")
-            cfdi_copy.pop("TipoDeComprobante")
-            if cfdi_copy.get("Exportacion") == "01":
-                del cfdi_copy["Exportacion"]
-            if cfdi_copy.get("FormaPago") == "99":
-                del cfdi_copy["FormaPago"]
-            if cfdi_copy.get("Moneda") in ("MXN", "XXX"):
-                del cfdi_copy["Moneda"]
-
-            if complemento := cfdi_copy.get("Complemento"):
-                cfdi_copy["Complemento"] = {}
-                if pagos := complemento.get("Pagos"):
-                    def clean_doc(d):
-                        d = d.copy()
-                        d.pop("ImpuestosDR")
-                        if d.get("MonedaDR") in ("MXN", "XXX"):
-                            del d["MonedaDR"]
-                            d.pop("EquivalenciaDR")
-                        return d
-
-                    def clean_pago(p):
-                        p = p.copy()
-                        p.pop("ImpuestosP")
-                        p["DoctoRelacionado"] = [clean_doc(x) for x in p["DoctoRelacionado"]]
-                        if p.get("MonedaP") in ("MXN", "XXX"):
-                            del p["MonedaP"]
-                            p.pop("TipoCambioP")
-                        return p
-
-                    pagos_copy = pagos.copy()
-                    pagos_copy["Pago"] = [clean_pago(x) for x in pagos_copy["Pago"]]
-                    cfdi_copy["Complemento"]["Pagos"] = pagos_copy
-
-                if timbre_fiscal_digital := complemento.get("TimbreFiscalDigital"):
-                    cfdi_copy["Complemento"]["TimbreFiscalDigital"] = timbre_fiscal_digital['UUID']
-
-        if isinstance(cfdi, SatCFDI) and ver_saldo:
-            cfdi_copy["_saldo_pendiente"] = cfdi.saldo_pendiente
+    def action_button(self, action_name, action_items):
+        if action_name == ACTION_FACTURAS:
+            self.all_invoices = None
+            for invoice in action_items:
+                cfdi = self.generate_invoice(invoice=invoice)
+                if cfdi is None:
+                    break
+                print_yaml({
+                    "FacturaGenerada": cfdi_header(cfdi),
+                })
+                self._read()
+        elif action_name == ACTION_EMAILS:
+            clients = ClientsManager()
+            emisor_cif = clients[self.csd_signer.rfc]
+            self.enviar_correos(emisor_cif, action_items)
+        elif action_name == ACTION_CLIENTS:
+            for rfc, details in action_items.items():
+                print(f"Validando: {rfc}")
+                self._read()
+                validar_client(rfc, details)
 
-        print_yaml(cfdi_copy)
+    def set_selected_satcfdi(self, factura):
+        i = factura
+        self.selected_satcfdi = i
+        self.window["ver_factura"].update(disabled=not i)
+        if i:
+            estado = self.local_db.status_sat(i).get('Estado', 'Vigente')
+            self.window["status_sat"].update(
+                estado,
+                visible=True,
+                button_color="red4" if estado != "Vigente" else "green",
+            )
+        else:
+            self.window["status_sat"].update(
+                visible=False
+            )
+
+        # Email
+        is_enviable = i \
+                      and i["Emisor"]["Rfc"] == self.csd_signer.rfc \
+                      and i["Fecha"] >= self.local_db.enviar_a_partir \
+                      and i.estatus == "1"
+        if is_enviable:
+            self.window["email_notificada"].update(
+                "Por Enviar" if self.local_db.notificar(i) else " Enviada  ",
+                visible=True,
+                button_color="red4" if self.local_db.notificar(i) else "green",
+            )
+        else:
+            self.window["email_notificada"].update("", visible=False)
+
+        # Pendiente de Pago
+        is_pendientable = i \
+                          and i["Emisor"]["Rfc"] == self.csd_signer.rfc \
+                          and i["TipoDeComprobante"] == "I" \
+                          and i["Fecha"] >= self.local_db.saldar_a_partir[i['MetodoPago']] \
+                          and i.estatus == "1" \
+                          and (i["MetodoPago"] == PUE or i.saldo_pendiente) \
+                          and i["Total"]
+        if is_pendientable:
+            self.window["pendiente_pago"].update(
+                "Por Saldar" if self.local_db.saldar(i) else " Saldada  ",
+                visible=True,
+                button_color="red4" if self.local_db.saldar(i) else "green",
+            )
+        else:
+            self.window["pendiente_pago"].update("", visible=False)
+
+        # PPD
+        is_ppd_active = i \
+                        and i.get("MetodoPago") == PPD \
+                        and i.estatus == "1" \
+                        and i["Emisor"]["Rfc"] == self.csd_signer.rfc
+        self.window["prepare_pago"].update(disabled=not is_ppd_active)
+        self.window["fecha_pago_select"].update(disabled=not is_ppd_active)
+        self.window["fecha_pago"].update(disabled=not is_ppd_active)
+        self.window["importe_pago"].update(disabled=not is_ppd_active)
+        self.window["forma_pago"].update(disabled=not is_ppd_active)
+
+    def print_satcfdis(self, cfdis):
+        def info_fmt(i):
+            return "🗙" if i.estatus == '0' else ("📧" if self.local_db.notificar(i) else "")
+
+        if cfdis := sorted(cfdis, key=lambda i: (i["Fecha"], i.name), reverse=True):
+            if self.window['detallado'].get():
+                for i in cfdis:
+                    print_yaml(i)
+                    self.local_db.describe(i)
+            else:
+                print_invoices(
+                    [
+                        [
+                            e,
+                            i['Receptor'].get('Nombre', '')[0:36],
+                            i['Receptor']['Rfc'],
+                            i.name,
+                            i["Fecha"].strftime("%Y-%m-%d"),
+                            i["Total"],
+                            self.local_db.saldar(i),
+                            mf_pago_fmt(i),
+                            i.uuid,
+                            info_fmt(i)
+                        ]
+                        for e, i in enumerate(cfdis, start=1)
+                    ]
+                )
+            if len(cfdis) == 1:
+                print_cfdi_details(cfdis[0])
+                self.set_selected_satcfdi(cfdis[0])
+            else:
+                self.set_selected_satcfdi(None)
+        else:
+            print("No hay resultados")
+            self.set_selected_satcfdi(None)
+
+    def print_prepared_cfdis(self, cfdis, start=1):
+        if cfdis:
+            if self.window['detallado'].get():
+                for i, cfdi in enumerate(cfdis, start=start):
+                    log_item(f"FACTURA NUMERO: {i}")
+                    print_yaml(cfdi)
+            else:
+                print_cfdis(cfdis, start=start)
+            self.action_button_manager.set_items(ACTION_FACTURAS, cfdis)
+        else:
+            print("No hay facturas para este mes")
+
+    def header(self, name, clear=True):
+        if clear:
+            self.console.update("")
+        log_line(name)
 
     def main_loop(self):
-        factura_seleccionada = None  # type: MyCFDI | None
-
         while True:
             event, values = self.window.read()
-            self.config.reload()
             try:
                 if event in ("Exit", PySimpleGUI.WIN_CLOSED):
                     return
 
-                if event not in ("crear_facturas", "enviar_correos", "confirm_pago_button", "ver_factura", "ver_excel"):
-                    self.console.update("")
-                invoices_to_create = self.invoice_button_manager.clear()
-                emails_to_send = self.email_button_manager.clear()
+                action_name, action_items = self.action_button_manager.clear()
 
                 match event:
+                    case "folio":
+                        self.set_folio(to_int(values["folio"]))
+
                     case "about":
                         clients = ClientsManager()
                         self.initial_screen(clients[self.csd_signer.rfc])
 
-                    case "factura_pagar" | "buscar_factura":
-                        text = self.window["factura_pagar"].get().strip()
-                        factura_seleccionada = self.factura_uuid(text)
-                        if event == "buscar_factura" and not factura_seleccionada:
-                            factura_seleccionada = self.factura_buscar(text)
-
-                        if factura_seleccionada:
-                            self.log_cfdi(factura_seleccionada)
-                            self.local_db.describe(factura_seleccionada)
-
-                        not_ppd_all = not factura_seleccionada \
-                                      or factura_seleccionada.get("MetodoPago") != PPD \
-                                      or factura_seleccionada.estatus != "1"
-                        not_ppd = not_ppd_all \
-                                  or factura_seleccionada["Emisor"]["Rfc"] != self.csd_signer.rfc
-
-                        not_pue = not factura_seleccionada \
-                                  or factura_seleccionada.get("MetodoPago") != PUE \
-                                  or factura_seleccionada.estatus != "1" or \
-                                  factura_seleccionada["Emisor"]["Rfc"] != self.csd_signer.rfc
-
-                        self.window["status_sat"].update(disabled=not factura_seleccionada)
-
-                        self.window["pago_pue"].update(
-                            disabled=not_pue
-                                     or factura_seleccionada["Fecha"] <= self.config['pue_pagada_hasta']
-                        )
-                        self.window["email_notificada"].update(
-                            disabled=not factura_seleccionada
-                                     or factura_seleccionada["Emisor"]["Rfc"] != self.csd_signer.rfc
-                                     or factura_seleccionada["Fecha"] <= self.config['email_notificada_hasta']
-                        )
-                        self.window["ignorar_ppd"].update(
-                            disabled=not_ppd_all
-                                     or factura_seleccionada["Fecha"] <= self.config['ppd_ignorar_hasta']
-                        )
+                    case "buscar_factura" | 'factura_pagar_enter':
+                        self.header("Buscar Factura")
 
-                        self.window["ver_factura"].update(disabled=not factura_seleccionada)
+                        if search_text := values["factura_pagar"].strip().upper():
+                            if len(search_text) < 3:
+                                self.console.update("El texto de búsqueda debe tener al menos 3 caracteres")
+                                continue
+
+                            if search_uuid := to_uuid(search_text):
+                                def fac_iter():
+                                    if v := self.get_all_invoices().get(search_uuid):
+                                        yield v
+                            else:
+                                def fac_iter():
+                                    for i in self.get_all_invoices().values():
+                                        if i["Emisor"]["Rfc"] == self.csd_signer.rfc and \
+                                                (i.name == search_text or i["Receptor"]["Rfc"] == search_text or search_text in i["Receptor"].get("Nombre", "")):
+                                            yield i
 
-                        self.window["prepare_pago"].update(disabled=not_ppd)
-                        self.window["fecha_pago_select"].update(disabled=not_ppd)
-                        self.window["fecha_pago"].update(disabled=not_ppd)
-                        self.window["forma_pago"].update(disabled=not_ppd)
-                        self.window["descarga"].update(disabled=not to_uuid(text))
+                            self.print_satcfdis(fac_iter())
+                            self.window["descarga"].update(disabled=not search_uuid)
 
                     case "preparar_ajuste_anual":
-                        log_item(f"AJUSTE ANUAL")
-                        ym_date = parse_ym_date(values['anio_mes_ajuste'])
-                        ajuste_porcentaje = values['ajuste_porcentaje']
-                        if not ajuste_porcentaje:
-                            logger.info("Especificar Ajuste Porcetaje")
-                            continue
-
-                        ajuste_porcentaje = Decimal(ajuste_porcentaje) / 100
-
-                        shutil.rmtree(AJUSTES_DIR, ignore_errors=True)
-                        os.makedirs(AJUSTES_DIR, exist_ok=True)
-                        clients = ClientsManager()
-                        facturas = FacturasManager()["Facturas"]
-
-                        has_ajustes = False
-                        for i, (rfc, concepto) in enumerate(find_ajustes(facturas, ym_date.month), start=1):
-                            has_ajustes = True
-                            receptor = clients[rfc]
-                            valor_unitario_nuevo = concepto["ValorUnitario"] * (1 + ajuste_porcentaje)
-                            concepto = format_concepto_desc(concepto, periodo="INMUEBLE")
-
-                            data = {
-                                "receptor": receptor,
-                                "concepto": concepto,
-                                "valor_unitario_nuevo": pesos(valor_unitario_nuevo),
-                                "ajuste_porcentaje": porcentaje(ajuste_porcentaje, 2),
-                                "ajuste_periodo": "UN AÑO",
-                                "ajuste_efectivo_al": fecha(ym_date),
-                                "periodo": concepto['_periodo_mes_ajuste'].split(".")[0].upper()
-                            }
-
-                            log_item(f"CARTA INCREMENTO NUMERO: {i}")
-                            print_yaml(data)
-                            res = self.generate_pdf_template(template_name='incremento_template.md', fields=data)
-                            file_name = f'{AJUSTES_DIR}/AjusteRenta_{rfc}_{concepto["CuentaPredial"]}.pdf'
-                            with open(file_name, 'wb') as f:
-                                f.write(res)
-                            self._read()
-
-                        if has_ajustes:
-                            os.startfile(
-                                os.path.abspath(AJUSTES_DIR)
-                            )
+                        self.header(f"AJUSTES")
+                        ajustes(
+                            emisor_rfc=self.csd_signer.rfc,
+                            ym_date=parse_ym_date(values['periodo'])
+                        )
 
                     case "recuperar_emitidas" | "recuperar_recibidas":
-                        log_line("RECUPERAR")
+                        self.header("RECUPERAR")
                         fecha_final = date.today()
                         fecha_inicial = fecha_final - timedelta(days=int(values["recuperar_dias"]))
-                        id_solicitud = self.config.get(event)
+                        id_solicitud = self.local_db.get(event)
 
                         if not id_solicitud:
                             self._read()
                             response = self.sat_service.recover_comprobante_request(
                                 fecha_inicial=fecha_inicial,
                                 fecha_final=fecha_final,
                                 rfc_receptor=self.sat_service.signer.rfc if "recuperar_recibidas" == event else None,
                                 rfc_emisor=self.sat_service.signer.rfc if "recuperar_emitidas" == event else None,
                                 tipo_solicitud=TipoDescargaMasivaTerceros.CFDI,
                             )
                             print_yaml(response)
-                            self.config[event] = response['IdSolicitud']
-                            self.config.save()
+                            self.local_db[event] = response['IdSolicitud']
                             print("Nueva Solicitud Creada")
                         else:
                             print_yaml({
                                 'IdSolicitud': id_solicitud
                             })
                             self._read()
                             for paquete_id, data in self.recupera_comprobantes(id_solicitud):
                                 if data:
                                     self.all_invoices = None
                                     with io.BytesIO(data) as b:
                                         self.unzip_cfdi(b)
-                                del self.config[event]
-                                self.config.save()
+                                del self.local_db[event]
                             log_line("FIN")
 
-                    case "validate_clientes":
-                        log_line("VALIDAR CLIENTES")
+                    case "prepare_clientes":
+                        self.header("CLIENTES")
                         clients = ClientsManager()
-                        res = PySimpleGUI.popup(
-                            f"Estas seguro que quieres validar {len(clients)} clientes?",
-                            title=self.window[event].ButtonText,
-                            button_type=POPUP_BUTTONS_OK_CANCEL,
-                        )
-                        if res == "OK":
-                            for rfc, details in clients.items():
-                                log_item(f"VALIDANDO {rfc}")
-                                self._read()
-                                validar_client(rfc, details)
-                            log_item("FIN")
+                        ym_date = parse_ym_date(values['periodo'])
+                        if clients:
+                            facturas = FacturasManager(ym_date)["Facturas"]
+                            print(
+                                tabulate(
+                                    [
+                                        [
+                                            i,
+                                            client["RazonSocial"][:36],
+                                            client["Rfc"],
+                                            client["RegimenFiscal"].code,
+                                            client["CodigoPostal"],
+                                            sum(1 for f in facturas if f["Receptor"] == k) or None,
+                                            "; ".join(client["Email"])[0:72],
+                                        ]
+                                        for i, (k, client) in enumerate(clients.items(), start=1)
+                                    ],
+                                    headers=(
+                                        "",
+                                        "Razon Social",
+                                        "Rfc",
+                                        "Reg",
+                                        "CP",
+                                        "#",
+                                        "Email",
+                                    ),
+                                    colalign=("right", "left", "left", "left", "left", "right"),
+                                )
+                            )
+                            self.action_button_manager.set_items(ACTION_CLIENTS, clients)
                         else:
-                            log_item("OPERACION CANCELADA")
+                            print("No hay clientes")
 
-                    case "prepare_facturas":
-                        log_line("PREPARAR FACTURAS")
-                        facturas = generate_ingresos(
-                            config=self.config,
+                    case "prepare_facturas" | "inicio_enter" | "final_enter":
+                        ym_date = parse_ym_date(values["periodo"])
+                        self.header(f"PREPARAR FACTURAS {values['periodo']}")
+                        print('Periodo:', periodo_desc(ym_date, 'Mensual.1'), '[AL ...]')
+                        inicio = int(values["inicio"])
+
+                        if cfdis := generate_ingresos(
+                            folio=int(values["folio"]),
+                            serie=self.serie,
                             clients=ClientsManager(),
-                            facturas=FacturasManager()["Facturas"],
-                            values=values,
+                            facturas=FacturasManager(ym_date)["Facturas"],
+                            ym_date=ym_date,
                             csd_signer=self.csd_signer
-                        )
-                        if facturas:
-                            for i, cfdi in enumerate(facturas, start=1):
-                                log_item(f"FACTURA NUMERO: {i}")
-                                self.log_cfdi(cfdi)
+                        ):
+                            final = to_int(values["final"]) or len(cfdis)
+                            cfdis = cfdis[max(inicio - 1, 0):max(final, 0)]
 
-                            self.invoice_button_manager.set_invoices(
-                                facturas
-                            )
+                        self.print_prepared_cfdis(cfdis, start=inicio)
 
-                    case "prepare_pago":
-                        log_line("COMPROBANTE PAGO")
-                        if i := factura_seleccionada:
-                            cfdi_pago = pago_factura(
-                                config=self.config,
-                                factura_pagar=i,
-                                fecha_pago=values["fecha_pago"],
-                                forma_pago=values["forma_pago"],
-                                csd_signer=self.csd_signer
-                            )
-                            if cfdi_pago:
-                                self.log_cfdi(cfdi_pago)
-                                self.invoice_button_manager.set_invoices(
-                                    [cfdi_pago]
-                                )
+                    case "prepare_pago" | "importe_pago_enter" | "fecha_pago_enter" | "forma_pago_enter":
+                        self.header("COMPROBANTE PAGO")
+                        if i := self.selected_satcfdi:
+                            if cfdi := pago_factura(
+                                    serie=self.serie,
+                                    folio=int(values["folio"]),
+                                    factura_pagar=i,
+                                    fecha_pago=values["fecha_pago"],
+                                    forma_pago=values["forma_pago"],
+                                    importe_pago=values["importe_pago"],
+                                    csd_signer=self.csd_signer
+                            ):
+                                self.print_prepared_cfdis([cfdi])
+                                print_cfdi_details(cfdi)
 
                     case "ver_factura":
-                        if i := factura_seleccionada:
+                        if i := self.selected_satcfdi:
                             os.startfile(
                                 os.path.abspath(i.filename + ".pdf")
                             )
 
                     case "status_sat":
-                        log_line("STATUS")
-                        if i := factura_seleccionada:
+                        self.header("STATUS")
+                        if i := self.selected_satcfdi:
                             estado = self.local_db.status_sat(i, update=True)
+                            self.print_satcfdis([i])
                             print_yaml(estado)
-                            self.local_db.describe(i)
 
-                    case "pago_pue":
-                        if i := factura_seleccionada:
-                            self.log_cfdi(i)
-                            self.local_db.describe(i)
-                            st = self.local_db.pue_pagada(i)
-                            res = PySimpleGUI.popup(
-                                f"Estas seguro que quieres marcarla como {'-NO- ' if st else ''}pagada?",
-                                title=self.window[event].ButtonText,
-                                button_type=POPUP_BUTTONS_OK_CANCEL,
-                            )
-                            if res == "OK":
-                                self.console.update("")
-                                self.local_db.pue_pagada_set(i.uuid, not st)
-                                self.log_cfdi(i)
-                                self.local_db.describe(i)
-                                print(f"FACTURA MARCADA COMO {'-NO- ' if st else ''}PAGADA")
-
-                    case "ignorar_ppd":
-                        if i := factura_seleccionada:
-                            self.log_cfdi(i)
-                            self.local_db.describe(i)
-                            st = self.local_db.ppd_ignorar(i)
-                            res = PySimpleGUI.popup(
-                                f"Estas seguro que quieres marcarla como {'-NO- ' if st else ''}ignorada?",
-                                title=self.window[event].ButtonText,
-                                button_type=POPUP_BUTTONS_OK_CANCEL,
-                            )
-                            if res == "OK":
-                                self.console.update("")
-                                self.local_db.ppd_ignorar_set(i.uuid, not st)
-                                self.log_cfdi(i)
-                                self.local_db.describe(i)
-                                print(f"FACTURA MARCADA COMO {'-NO- ' if st else ''}IGNORADA")
+                    case "pendiente_pago":
+                        if i := self.selected_satcfdi:
+                            st = self.local_db.saldar_flip(i)
+                            self.console.update("")
+                            self.header(self.window[event].ButtonText.upper())
+                            self.print_satcfdis([i])
+                            print(f"FACTURA MARCADA COMO {'-NO- ' if st else ''}SALDADA")
 
                     case "email_notificada":
-                        if i := factura_seleccionada:
-                            self.log_cfdi(i)
-                            self.local_db.describe(i)
-                            st = self.local_db.email_notificada(i)
-                            res = PySimpleGUI.popup(
-                                f"Estas seguro que quieres marcarla como {'-NO- ' if st else ''}notificada?",
-                                title=self.window[event].ButtonText,
-                                button_type=POPUP_BUTTONS_OK_CANCEL,
-                            )
-                            if res == "OK":
-                                self.console.update("")
-                                self.local_db.email_notificada_set(i.uuid, not st)
-                                self.log_cfdi(i)
-                                self.local_db.describe(i)
-                                print(f"FACTURA MARCADA COMO {'-NO- ' if st else ''}NOTIFICADA")
-
-                    case "crear_facturas":
-                        log_line("CREAR FACTURAS")
-                        res = PySimpleGUI.popup(
-                            f"Estas seguro que quieres crear {len(invoices_to_create)} facturas?",
-                            title=self.window[event].ButtonText,
-                            button_type=POPUP_BUTTONS_OK_CANCEL,
-                        )
-                        if res == "OK":
-                            self.all_invoices = None
-                            for invoice in invoices_to_create:
-                                cfdi = self.generate_invoice(invoice=invoice)
-                                if cfdi is None:
-                                    break
-                                print_yaml({
-                                    "FacturaGenerada": cfdi_header(cfdi),
-                                })
-                                self._read()
-                            log_item("FIN")
-                        else:
-                            log_item("OPERACION CANCELADA")
+                        if i := self.selected_satcfdi:
+                            st = self.local_db.notificar_flip(i)
+                            self.console.update("")
+                            self.header(self.window[event].ButtonText.upper())
+                            self.print_satcfdis([i])
+                            print(f"FACTURA MARCADA COMO {'-NO- ' if st else ''}NOTIFICADA")
 
                     case "prepare_correos":
-                        log_line("PREPARAR CORREOS")
+                        self.header("CORREOS")
                         now = date.today()
                         dp = DatePeriod(now.year, now.month)
                         clients = ClientsManager()
                         a_invoices = self.get_all_invoices()
 
                         cfdi_correos = []
                         for receptor_rfc, notify_invoices in itertools.groupby(
                                 sorted(
-                                    (i for i in a_invoices.values() if not i.notified),
+                                    (i for i in a_invoices.values() if i.estatus == "1" and self.local_db.notificar(i)),
                                     key=lambda r: r["Receptor"]["Rfc"]
                                 ),
                                 lambda r: r["Receptor"]["Rfc"]
                         ):
                             notify_invoices = list(notify_invoices)
-                            fac_pen = filter_invoices_iter(
-                                invoices=a_invoices.values(),
-                                fecha=lambda x: x < dp,
-                                invoice_type="I",
-                                pending_balance=lambda x: x > 0,
-                                rfc_emisor=self.csd_signer.rfc,
-                                rfc_receptor=receptor_rfc,
-                                estatus='1'
+
+                            def fac_iter():
+                                for i in self.get_all_invoices().values():
+                                    if i["Emisor"]["Rfc"] == self.csd_signer.rfc \
+                                            and i["TipoDeComprobante"] == "I" \
+                                            and i.estatus == '1' \
+                                            and self.local_db.saldar(i) \
+                                            and i["Fecha"] < dp \
+                                            and i["Receptor"]["Rfc"] == receptor_rfc:
+                                        yield i
+
+                            fac_pen = sorted(
+                                fac_iter(),
+                                key=lambda r: r["Fecha"]
                             )
                             receptor = clients[receptor_rfc]
-                            cfdi_correos.append((receptor, notify_invoices, sorted(fac_pen, key=lambda r: r["Fecha"])))
+                            cfdi_correos.append((receptor, notify_invoices, fac_pen))
 
                         if cfdi_correos:
-                            self.email_button_manager.set_emails(
-                                cfdi_correos
-                            )
+                            print(tabulate(
+                                [
+                                    [
+                                        i,
+                                        receptor["RazonSocial"][0:36],
+                                        receptor["Rfc"],
+                                        ",".join(n.name for n in notify_invoices),
+                                        ",".join(n.name for n in facturas_pendientes)
+                                    ] for i, (receptor, notify_invoices, facturas_pendientes) in enumerate(cfdi_correos, start=1)
+                                ],
+                                headers=(
+                                    '',
+                                    'Receptor Razon Social',
+                                    'Recep. Rfc',
+                                    'Facturas',
+                                    'Pendientes Emitidas Meses Anteriores'
+                                ),
+                                disable_numparse=True,
+                                colalign=("right", "left", "left", "left", "left")
+                            ))
+
+                            self.action_button_manager.set_items(ACTION_EMAILS, cfdi_correos)
                         else:
                             print("No hay correos pendientes de enviar")
 
-                    case "enviar_correos":
-                        log_line("ENVIAR CORREOS")
+                    case "crear_facturas":
+                        self.header(f"PROCESAR {action_name.upper()}", clear=False)
                         res = PySimpleGUI.popup(
-                            f"Estas seguro que quieres enviar {len(emails_to_send)} correos?",
+                            f"Estas seguro que quieres crear {len(action_items)} {action_name}?",
                             title=self.window[event].ButtonText,
-                            button_type=POPUP_BUTTONS_OK_CANCEL
+                            button_type=POPUP_BUTTONS_OK_CANCEL,
                         )
                         if res == "OK":
-                            clients = ClientsManager()
-                            emisor_cif = clients[self.csd_signer.rfc]
-                            self.enviar_correos(emisor_cif, emails_to_send)
-                            log_item("FIN")
+                            self.action_button(action_name, action_items)
+                            print("FIN")
                         else:
-                            log_item("OPERACION CANCELADA")
+                            print("OPERACION CANCELADA")
 
                     case "facturas_pendientes":
-                        clients = ClientsManager()
-                        log_line("FACTURAS PENDIENTES")
+                        self.header("FACTURAS PENDIENTES")
 
-                        fac_pen = filter_invoices_iter(
-                            invoices=self.get_all_invoices().values(),
-                            invoice_type="I",
-                            pending_balance=lambda x: x > 0,
-                            rfc_emisor=self.csd_signer.rfc,
-                            estatus='1'
-                        )
-                        for receptor_rfc, fac_pen in itertools.groupby(
-                                sorted(
-                                    fac_pen,
-                                    key=lambda r: r["Receptor"]["Rfc"]
-                                ),
-                                lambda r: r["Receptor"]["Rfc"]
-                        ):
-                            f = {
-                                'Receptor': Code(receptor_rfc, clients[receptor_rfc]['RazonSocial']),
-                                'FacturasPendientes': [
-                                    {
-                                        "Factura": f"{i.name} - {i.uuid}",
-                                        'SaldoPendiente': i.saldo_pendiente,
-                                        'Fecha': i["Fecha"]
-                                    }
-                                    for i in sorted(fac_pen, key=lambda r: r["Fecha"])
-                                ]
-                            }
-                            print_yaml(f)
+                        def fac_iter():
+                            for i in self.get_all_invoices().values():
+                                if i["Emisor"]["Rfc"] == self.csd_signer.rfc \
+                                        and i["TipoDeComprobante"] == "I" \
+                                        and i.estatus == '1' \
+                                        and self.local_db.saldar(i):
+                                    yield i
+
+                        self.print_satcfdis(fac_iter())
 
                     case "descarga":
-                        log_line('DESCARGADA')
+                        self.header('DESCARGADA')
                         try:
                             res = self.pac_service.recover(values["factura_pagar"], accept=Accept.XML_PDF)
                             self.all_invoices = None
                             cfdi = move_to_folder(res.xml, pdf_data=res.pdf)
-                            self.log_cfdi(cfdi, ver_saldo=False)
+                            cfdi = self.get_all_invoices()[to_uuid(cfdi["Complemento"]["TimbreFiscalDigital"]["UUID"])]
+                            self.print_satcfdis([cfdi])
                         except DocumentNotFoundError:
                             logger.info("Factura no encontrada")
 
-                    case "exportar_facturas":
-                        log_line("EXPORTAR FACTURAS")
+                    case "ver_excel":
+                        self.header("EXCEL")
                         clients = ClientsManager()
                         emisor_cif = clients[self.csd_signer.rfc]
                         exportar_facturas(
                             self.get_all_invoices(),
                             parse_date_period(values["periodo"]),
                             emisor_cif,
-                            self.config['rfc_prediales']
+                            self.rfc_prediales
                         )
 
-                    case "ver_excel":
-                        archivo_excel = exportar_facturas_filename(parse_date_period(values["periodo"]))
+                        archivo_excel = facturas_filename(parse_date_period(values["periodo"]))
                         os.startfile(
                             os.path.abspath(archivo_excel)
                         )
 
+                    case "facturas_emitidas" | "periodo_enter":
+                        self.header(f"FACTURAS EMITIDAS {values['periodo']}")
+                        dp = parse_date_period(values["periodo"])
+
+                        def fact_iter():
+                            for i in self.get_all_invoices().values():
+                                if i["Emisor"]["Rfc"] == self.csd_signer.rfc \
+                                        and i["Fecha"] == dp:
+                                    yield i
+
+                        self.print_satcfdis(fact_iter())
+
                     case "ver_html":
-                        inv = self.get_all_invoices().values()
+                        self.header("HTML")
                         dp = parse_date_period(values["periodo"])
-                        inv = filter_invoices_iter(
-                            invoices=inv,
-                            fecha=dp,
-                            rfc_emisor=self.csd_signer.rfc,
-                        )
-                        outfile = exportar_facturas_filename(dp, ext="html")
+
+                        def fact_iter():
+                            for i in self.get_all_invoices().values():
+                                if i["Emisor"]["Rfc"] == self.csd_signer.rfc \
+                                        and i["Fecha"] == dp:
+                                    yield i
+
+                        outfile = facturas_filename(dp, ext="html")
                         Representable.html_write_all(
-                            objs=inv,
+                            objs=fact_iter(),
                             target=outfile,
                         )
                         os.startfile(
                             os.path.abspath(outfile)
                         )
 
-                    case "periodo" | "inicio" | "final" | "fecha_pago" | "forma_pago":
+                    case "ver_carpeta":
+                        archivo = facturas_filename(parse_date_period(values["periodo"]))
+                        os.startfile(
+                            os.path.abspath(os.path.dirname(archivo))
+                        )
+
+                    case "ver_carpeta_ajustes":
+                        ajustes_dir = ajustes_directory(parse_ym_date(values['periodo']))
+                        os.startfile(
+                            os.path.abspath(ajustes_dir)
+                        )
+
+                    case "periodo" | "inicio" | "final" | "fecha_pago" | "forma_pago" | "importe_pago" | ' ':
                         pass
 
                     case _:
                         logger.error(f"Unknown event '{event}'")
 
             except Exception as ex:
                 logger.exception(header_line("ERROR"))
```

### Comparing `satdigitalinvoice-2.0.4/satdigitalinvoice/__version__.py` & `satdigitalinvoice-2.0.5/satdigitalinvoice/__version__.py`

 * *Files identical despite different names*

### Comparing `satdigitalinvoice-2.0.4/satdigitalinvoice/client_validation.py` & `satdigitalinvoice-2.0.5/satdigitalinvoice/client_validation.py`

 * *Files identical despite different names*

### Comparing `satdigitalinvoice-2.0.4/satdigitalinvoice/file_data_managers.py` & `satdigitalinvoice-2.0.5/satdigitalinvoice/file_data_managers.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,59 +1,34 @@
+import collections.abc
 import json
 import logging
 import os
+from datetime import date
 from decimal import Decimal
-from html import escape as html_escape
-import collections.abc
-import jinja2
-import yaml
-from jinja2 import Environment
-from jinja2.filters import do_mark_safe
+
 import jsonschema as jsonschema
-from jsonschema.validators import Draft202012Validator
+import yaml
 from satcfdi import Code
 from satcfdi.pacs import sat
 # noinspection PyUnresolvedReferences
 from satcfdi.transform.catalog import CATALOGS
 from satcfdi.transform.helpers import Xint
-from satdigitalinvoice import SOURCE_DIRECTORY
 from yaml import MappingNode, SafeLoader
 from yaml.constructor import ConstructorError
 
+from . import SOURCE_DIRECTORY
+from .utils import find_best_match, first_duplicate
+
 REGIMEN_FISCAL = CATALOGS['{http://www.sat.gob.mx/sitio_internet/cfd/catalogos}c_RegimenFiscal']
 
 logger = logging.getLogger(__name__)
 sat_manager = sat.SAT()
 
-environment_default = Environment(
-    loader=jinja2.FileSystemLoader(searchpath=['templates']),
-    autoescape=False,
-    trim_blocks=True,
-    lstrip_blocks=True,
-    undefined=jinja2.StrictUndefined,
-)
-
-
-def finalize_html(val):
-    return do_mark_safe(
-        tag(html_escape(val), "b")
-    )
-
-
-environment_bold_escaped = Environment(
-    loader=jinja2.FileSystemLoader(searchpath=['templates']),
-    autoescape=True,
-    trim_blocks=True,
-    lstrip_blocks=True,
-    undefined=jinja2.StrictUndefined,
-    finalize=finalize_html
-)
 
-
-class DuplicateKeySafeLoader(yaml.SafeLoader):
+class DuplicateKeySafeLoader(yaml.CSafeLoader):
     def construct_mapping(self, node, deep=False):
         if isinstance(node, MappingNode):
             self.flatten_mapping(node)
 
         if not isinstance(node, MappingNode):
             raise ConstructorError(None, None,
                                    "expected a mapping node, but found %s" % node.id,
@@ -68,110 +43,95 @@
             if key in mapping:
                 raise ConstructorError("while constructing a mapping", node.start_mark,
                                        "found duplicate key (%s)" % key, key_node.start_mark)
             mapping[key] = value
         return mapping
 
 
+def load_validator(schema_file):
+    with open(os.path.join(SOURCE_DIRECTORY, 'schemas', schema_file), "r", encoding="utf-8") as fs:
+        schema = yaml.load(fs, SafeLoader)
+        validator = jsonschema.validators.validator_for(schema)
+        validator.check_schema(schema)
+        return validator(schema)
+
+
+client_validator = load_validator("cliente.yaml")
+factura_validator = load_validator("factura.yaml")
+config_validator = load_validator("config.yaml")
+
+
 class LocalData(dict):
     file_source = None
 
     def __new__(cls, *args, **kwargs):
         return super().__new__(cls)
 
     def __init__(self):
         super().__init__(self._raw())
 
-    def reload(self):
-        super().update(self._raw())
-
     def _raw(self):
         with open(self.file_source, "r", encoding="utf-8") as fs:
             return yaml.load(fs, DuplicateKeySafeLoader)
 
 
 class ConfigManager(LocalData):
     file_source = "config.yaml"
 
-    def folio(self):
-        return self["folio"]
-
-    def serie(self):
-        return self["serie"]
-
-    def inc_folio(self):
-        self["folio"] += 1
-        self.save()
-
-    def save(self):
-        with open(self.file_source, "w", encoding="utf-8") as fs:
-            yaml.dump_all([self], fs, Dumper=yaml.SafeDumper, encoding="utf-8", allow_unicode=True, sort_keys=False)
-
-
-def load_validator(schema_file):
-    with open(os.path.join(SOURCE_DIRECTORY, 'schemas', schema_file), "r", encoding="utf-8") as fs:
-        schema = yaml.load(fs, SafeLoader)
-        validator = jsonschema.validators.validator_for(schema)
-        validator.check_schema(schema)
-        return validator(schema)
-
-
-client_validator = load_validator("client.yaml")
-factura_validator = load_validator("factura.yaml")
+    def __init__(self):
+        super().__init__()
+        if error := jsonschema.exceptions.best_match(config_validator.iter_errors(self)):
+            raise error
 
 
 class ClientsManager(LocalData):
-    file_source = "clients.yaml"
+    file_source = "clientes.yaml"
 
     def __init__(self):
         super().__init__()
-
         for k, v in self.items():
             if error := jsonschema.exceptions.best_match(client_validator.iter_errors(v)):
                 raise error
             self[k]["Rfc"] = k
             self[k]["RegimenFiscal"] = Code(self[k]["RegimenFiscal"], REGIMEN_FISCAL.get(self[k]["RegimenFiscal"]))
 
 
 class FacturasManager(LocalData):
     file_source = "facturas.yaml"
 
-    def __init__(self):
-        super().__init__()
-
-        seen = set()
-        dup = None
-
-        for v in self["Facturas"]:
-            if error := jsonschema.exceptions.best_match(factura_validator.iter_errors(v)):
-                raise error
+    def __init__(self, emission_date: date | None):
+        def loading_function(loader, node):
+            cases = loader.construct_mapping(node, deep=True)
+            if emission_date is None:
+                return cases
+            return find_best_match(
+                cases,
+                emission_date
+            )[1]
 
-            x = json.dumps(v, sort_keys=True, default=str)
-            if x in seen:
-                dup = x
-                break
-            else:
-                seen.add(x)
-
-        if dup:
+        DuplicateKeySafeLoader.add_constructor("!case", loading_function)
+        super().__init__()
+        if dup := first_duplicate(json.dumps(x, sort_keys=True, default=str) for x in self["Facturas"]):
             raise ValueError("Factura Duplicada: {}".format(dup))
 
+        if emission_date:
+            for v in self["Facturas"]:
+                if error := jsonschema.exceptions.best_match(factura_validator.iter_errors(v)):
+                    raise error
 
-def tag(text, tag):
-    return '<' + tag + '>' + text + '</' + tag + '>'
 
-
-yaml.SafeDumper.add_multi_representer(dict, lambda dumper, data: dumper.represent_dict(data))
-yaml.SafeLoader.add_constructor("!decimal", lambda loader, node: Decimal(loader.construct_scalar(node)))
+DuplicateKeySafeLoader.add_constructor("!decimal", lambda loader, node: Decimal(loader.construct_scalar(node)))
+DuplicateKeySafeLoader.add_constructor("!read", lambda loader, node: open(loader.construct_scalar(node), 'rb').read())
 
 
 def represent_decimal(dumper, data):
     return dumper.represent_scalar('tag:yaml.org,2002:str', str(data))
 
 
 def represent_str(dumper, data):
     return dumper.represent_scalar('tag:yaml.org,2002:str', str(data))
 
 
+yaml.SafeDumper.add_multi_representer(dict, lambda dumper, data: dumper.represent_dict(data))
 yaml.SafeDumper.add_representer(Decimal, represent_decimal)
 yaml.SafeDumper.add_representer(Code, represent_str)
 yaml.SafeDumper.add_representer(Xint, represent_str)
```

### Comparing `satdigitalinvoice-2.0.4/satdigitalinvoice/formatting_functions/common.py` & `satdigitalinvoice-2.0.5/satdigitalinvoice/formatting_functions/common.py`

 * *Files identical despite different names*

### Comparing `satdigitalinvoice-2.0.4/satdigitalinvoice/local.py` & `satdigitalinvoice-2.0.5/satdigitalinvoice/local.py`

 * *Files 23% similar despite different names*

```diff
@@ -2,122 +2,128 @@
 import os
 import pickle
 from uuid import UUID
 
 import diskcache
 from satcfdi.accounting import SatCFDI
 from satcfdi.pacs import sat
+
+from . import DATA_DIRECTORY
 from .log_tools import print_yaml
 
-PUE_PAGADA = 0
-PPD_IGNORAR = 1
 EMAIL_NOTIFICADA = 2
 STATUS_SAT = 3
+PENDIENTE = 4
+FOLIO = 5
 
 sat_manager = sat.SAT()
 
 logger = logging.getLogger(__name__)
-DATA_DIR = '.data'
 
 
-class LocalDB:
+class LocalDB(diskcache.Cache):
     def __init__(self):
-        self.local_storage = diskcache.Cache(os.path.join(DATA_DIR, 'cache'))
+        super().__init__(directory=os.path.join(DATA_DIRECTORY, 'cache'))
 
-    def pue_pagada(self, uuid: UUID):
-        return self.local_storage.get(
-            (PUE_PAGADA, uuid), False
-        )
+    def folio(self):
+        return self.get(FOLIO, 1)
 
-    def pue_pagada_set(self, uuid: UUID, value: bool):
-        if value:
-            self.local_storage[(PUE_PAGADA, uuid)] = value
-        else:
-            try:
-                del self.local_storage[(PUE_PAGADA, uuid)]
-            except KeyError:
-                pass
+    def folio_set(self, value: int):
+        self[FOLIO] = value
 
-    def ppd_ignorar(self, uuid: UUID):
-        return self.local_storage.get(
-            (PPD_IGNORAR, uuid), False
+    def saldar(self, uuid: UUID):
+        return self.get(
+            (PENDIENTE, uuid), True
         )
 
-    def ppd_ignorar_set(self, uuid: UUID, value: bool):
+    def saldar_set(self, uuid: UUID, value: bool):
         if value:
-            self.local_storage[(PPD_IGNORAR, uuid)] = value
-        else:
             try:
-                del self.local_storage[(PPD_IGNORAR, uuid)]
+                del self[(PENDIENTE, uuid)]
             except KeyError:
                 pass
+        else:
+            self[(PENDIENTE, uuid)] = value
 
-    def email_notificada(self, uuid: UUID):
-        return self.local_storage.get(
-            (EMAIL_NOTIFICADA, uuid), False
+    def notificar(self, uuid: UUID):
+        return self.get(
+            (EMAIL_NOTIFICADA, uuid), True
         )
 
-    def email_notificada_set(self, uuid: UUID, value: bool):
+    def notificar_set(self, uuid: UUID, value: bool):
         if value:
-            self.local_storage[(EMAIL_NOTIFICADA, uuid)] = value
-        else:
             try:
-                del self.local_storage[(EMAIL_NOTIFICADA, uuid)]
+                del self[(EMAIL_NOTIFICADA, uuid)]
             except KeyError:
                 pass
+        else:
+            self[(EMAIL_NOTIFICADA, uuid)] = value
 
     def status_sat(self, uuid: UUID):
-        return self.local_storage.get(
+        return self.get(
             (STATUS_SAT, uuid), {}
         )
 
     def status_sat_set(self, uuid: UUID, value: dict):
         if value:
-            self.local_storage[(STATUS_SAT, uuid)] = value
+            self[(STATUS_SAT, uuid)] = value
         else:
             try:
-                del self.local_storage[(STATUS_SAT, uuid)]
+                del self[(STATUS_SAT, uuid)]
             except KeyError:
                 pass
 
 
 class LocalDBSatCFDI(LocalDB):
-    def __init__(self, config):
+    def __init__(self, enviar_a_partir, saldar_a_partir):
         super().__init__()
-        self.config = config
+        self.enviar_a_partir = enviar_a_partir
+        self.saldar_a_partir = saldar_a_partir
 
-    def email_notificada(self, cfdi: SatCFDI):
-        if cfdi["Fecha"] <= self.config['email_notificada_hasta']:
-            return True
-        return super().email_notificada(cfdi.uuid)
-
-    def pue_pagada(self, cfdi: SatCFDI):
-        if cfdi["Fecha"] <= self.config['pue_pagada_hasta']:
-            return True
-        return super().pue_pagada(cfdi.uuid)
-
-    def ppd_ignorar(self, cfdi: SatCFDI):
-        if cfdi["Fecha"] <= self.config['ppd_ignorar_hasta']:
-            return True
-        return super().ppd_ignorar(cfdi.uuid)
+    def notificar(self, cfdi: SatCFDI):
+        if cfdi["Fecha"] >= self.enviar_a_partir:
+            return super().notificar(cfdi.uuid)
+        return False
+
+    def notificar_flip(self, cfdi: SatCFDI):
+        v = not self.notificar(cfdi)
+        self.notificar_set(cfdi.uuid, v)
+        return v
+
+    def saldar(self, cfdi: SatCFDI):
+        if cfdi["TipoDeComprobante"] != "I":
+            return None
+        if cfdi["MetodoPago"] == "PPD" and cfdi.saldo_pendiente == 0:
+            return 0
+        if cfdi["Fecha"] >= self.saldar_a_partir[cfdi["MetodoPago"]]:
+            if super().saldar(cfdi.uuid):
+                if cfdi["MetodoPago"] == "PPD":
+                    return cfdi.saldo_pendiente
+                else:
+                    return cfdi["Total"]
+        return 0
+
+    def saldar_flip(self, cfdi: SatCFDI):
+        v = not self.saldar(cfdi)
+        self.saldar_set(cfdi.uuid, v)
+        return v
 
     def status_sat(self, cfdi: SatCFDI, update=False):
         if update:
             res = sat_manager.status(cfdi)
             if res["ValidacionEFOS"] == "200":
                 self.status_sat_set(cfdi.uuid, res)
             return res
         else:
             return super().status_sat(cfdi.uuid)
 
     def describe(self, cfdi: SatCFDI):
         print_yaml({
-            'pue_pagada': self.pue_pagada(cfdi),
-            'ppd_ignorar': self.ppd_ignorar(cfdi),
-            'email_notificada': self.email_notificada(cfdi),
+            'saldar': self.saldar(cfdi),
+            'enviar': self.notificar(cfdi),
             'status_sat': self.status_sat(cfdi)
         })
 
 
 def save_data(file, data):
     with open(os.path.join(DATA_DIR, file), 'wb') as f:
         pickle.dump(data, f)
```

### Comparing `satdigitalinvoice-2.0.4/satdigitalinvoice/markdown_styles/markdown6.css` & `satdigitalinvoice-2.0.5/satdigitalinvoice/markdown_styles/markdown6.css`

 * *Files identical despite different names*

### Comparing `satdigitalinvoice-2.0.4/satdigitalinvoice/mycfdi.py` & `satdigitalinvoice-2.0.5/satdigitalinvoice/mycfdi.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,30 +1,29 @@
 import glob
 import logging
 import os
 from collections.abc import Mapping
 from datetime import datetime
-from decimal import Decimal
 from typing import MutableMapping
 from uuid import UUID
 
 from satcfdi.accounting import complement_invoices_data, SatCFDI
 
 from .local import load_data, save_data
+from .utils import to_uuid
 
 ALL_INVOICES = 'all_invoices'
 ALL_RETENCIONES = 'all_retenciones'
 logger = logging.getLogger(__name__)
 
 PPD = "PPD"
 PUE = "PUE"
 
 
 class MyCFDI(SatCFDI):
-    issuer_rfc = None
     local_db = None
 
     def consulta_estado(self):
         return self.local_db.status_sat(self)
 
     @SatCFDI.estatus.getter
     def estatus(self) -> str:
@@ -35,29 +34,14 @@
         estado = self.local_db.status_sat(self).get('Estado')
         return Estatus.get(estado, "1")
 
     @SatCFDI.fecha_cancelacion.getter
     def fecha_cancelacion(self) -> datetime:
         return None
 
-    @SatCFDI.saldo_pendiente.getter
-    def saldo_pendiente(self) -> Decimal:
-        if self['TipoDeComprobante'] == "I":
-            if self["MetodoPago"] == PPD:
-                if self.local_db.ppd_ignorar(self):
-                    return Decimal()
-
-            if self["MetodoPago"] == PUE and not self.payments and self["Emisor"]["Rfc"] == self.issuer_rfc:
-                if self.local_db.pue_pagada(self):
-                    return Decimal()
-                else:
-                    return self['Total']
-
-        return super().saldo_pendiente
-
     @classmethod
     def get_all_invoices(cls, invoices: MutableMapping, search_path="*.xml") -> bool:
         # Check that all names are correct
         for file in glob.iglob(search_path, recursive=True):
             if not cls.uuid_from_filename(filename=file):
                 invoice = cls.from_file(file)
                 rename_invoice(file, invoice)
@@ -91,49 +75,37 @@
         # if the length does not match, then we need to try again :-/
         return was_updated
 
     @property
     def filename(self):
         match self.tag:
             case '{http://www.sat.gob.mx/cfd/3}Comprobante' | '{http://www.sat.gob.mx/cfd/4}Comprobante':
-                return "facturas/{3:%Y}/{3:%Y-%m}/{4}/{3:%Y-%m-%d}_{0}_[{1}]_{2}".format(
+                return "facturas/{3:%Y}/{3:%Y-%m}/{4}_{0}_[{1}]_{2}".format(
                     self.name,
                     self["TipoDeComprobante"].code,
                     self.uuid,
                     self["Fecha"],
-                    "Emitidas" if self["Emisor"]["Rfc"] == self.issuer_rfc else "Recibidas"
+                    self["Emisor"]["Rfc"],
                 )
             case '{http://www.sat.gob.mx/esquemas/retencionpago/1}Retenciones' | '{http://www.sat.gob.mx/esquemas/retencionpago/2}Retenciones':
-                return "retenciones/{2:%Y}/{2:%Y-%m}/{3}/{2:%Y-%m-%d}_{0}_{1}".format(
+                return "retenciones/{2:%Y}/{2:%Y-%m}/{3}_{0}_{1}".format(
                     self.get("FolioInt", ""),
                     self.uuid,
                     self["FechaExp"],
-                    "Emitidas" if self["Emisor"]["RFCEmisor"] == self.issuer_rfc else "Recibidas"
+                    self["Emisor"].get('RFCEmisor') or self["Emisor"].get('RfcE')
                 )
 
     @classmethod
     def uuid_from_filename(cls, filename):
         filename = os.path.basename(filename)
         parts = os.path.splitext(filename)[0].split("_")
         if len(parts) >= 3:
-            try:
-                return UUID(parts[-1])
-            except ValueError:
-                pass
+            return to_uuid(parts[-1])
         return None
 
-    @property
-    def notified(self) -> bool:
-        return self["Emisor"]["Rfc"] != self.issuer_rfc \
-            or self.local_db.email_notificada(self)
-
-    @notified.setter
-    def notified(self, value: bool):
-        self.local_db.email_notificada_set(self.uuid, value)
-
 
 def rename_invoice(file, invoice: MyCFDI, include_pdf=True):
     preferred_filename = invoice.filename
     if preferred_filename + ".xml" != file:
         os.makedirs(os.path.dirname(preferred_filename), exist_ok=True)
 
         try:
```

### Comparing `satdigitalinvoice-2.0.4/satdigitalinvoice/schemas/factura.yaml` & `satdigitalinvoice-2.0.5/satdigitalinvoice/schemas/factura.yaml`

 * *Files 7% similar despite different names*

```diff
@@ -33,15 +33,17 @@
         ClaveUnidad:
           type: string
         Descripcion:
           type: string
         _periodo_mes_ajuste:
           type: string
         ValorUnitario:
-          type: number
+          type:
+          - number
+          - 'null'
         Impuestos:
           type: object
           properties:
             Traslados:
               anyOf:
               - type: string
               - type: array
@@ -67,9 +69,8 @@
     type: number
 required:
 - Receptor
 - UsoCFDI
 - MetodoPago
 - FormaPago
 - Conceptos
-- Total
 additionalProperties: false
```

### Comparing `satdigitalinvoice-2.0.4/satdigitalinvoice.egg-info/PKG-INFO` & `satdigitalinvoice-2.0.5/satdigitalinvoice.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: satdigitalinvoice
-Version: 2.0.4
+Version: 2.0.5
 Summary: GUI APP to Generate CFDI
 Home-page: https://github.com/SAT-CFDI/python-satdigitalinvoice
 Author: satcfdi@outlook.com
 Author-email: satcfdi@outlook.com
 License: MIT License
 Project-URL: Documentation, https://satdigitalinvoice.readthedocs.io
 Project-URL: Source, https://github.com/SAT-CFDI/python-satdigitalinvoice
```

### Comparing `satdigitalinvoice-2.0.4/satdigitalinvoice.egg-info/SOURCES.txt` & `satdigitalinvoice-2.0.5/satdigitalinvoice.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -1,32 +1,29 @@
 setup.py
 satdigitalinvoice/__init__.py
 satdigitalinvoice/__main__.py
 satdigitalinvoice/__version__.py
 satdigitalinvoice/client_validation.py
+satdigitalinvoice/environments.py
+satdigitalinvoice/facturacion.py
 satdigitalinvoice/file_data_managers.py
 satdigitalinvoice/gui_functions.py
 satdigitalinvoice/layout.py
 satdigitalinvoice/local.py
 satdigitalinvoice/log_tools.py
 satdigitalinvoice/mycfdi.py
 satdigitalinvoice/utils.py
 satdigitalinvoice.egg-info/PKG-INFO
 satdigitalinvoice.egg-info/SOURCES.txt
 satdigitalinvoice.egg-info/dependency_links.txt
 satdigitalinvoice.egg-info/requires.txt
 satdigitalinvoice.egg-info/top_level.txt
 satdigitalinvoice/formatting_functions/__init__.py
 satdigitalinvoice/formatting_functions/common.py
+satdigitalinvoice/images/logo.png
 satdigitalinvoice/markdown_styles/markdown6.css
-satdigitalinvoice/microsoft_auth/__init__.py
-satdigitalinvoice/microsoft_auth/auth_code_receiver.py
-satdigitalinvoice/microsoft_auth/cache_interactive_browser.py
-satdigitalinvoice/microsoft_auth/cache_secret_client.py
-satdigitalinvoice/microsoft_auth/jwt_util.py
-satdigitalinvoice/microsoft_auth/microsoft_oauth2.py
-satdigitalinvoice/schemas/client.yaml
+satdigitalinvoice/schemas/cliente.yaml
+satdigitalinvoice/schemas/config.yaml
 satdigitalinvoice/schemas/factura.yaml
 tests/test_clients.py
 tests/test_crear_facturas.py
-tests/test_main.py
-tests/test_microsoft_auth.py
+tests/test_main.py
```

### Comparing `satdigitalinvoice-2.0.4/setup.py` & `satdigitalinvoice-2.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -56,18 +56,19 @@
     python_requires='>=3.10',
     package_dir={package: package_dir},
     packages=packages,
     package_data={
         package: [
             "markdown_styles/*",
             "schemas/*",
+            'images/*',
         ],
     },
     install_requires=[
-        'satcfdi==4.0.3',
+        'satcfdi==4.0.5',
         'diskcache',
         'num2words',
         'PyYAML',
         'babel',
         'azure-keyvault',
         'markdown2',
         'python-dateutil',
```

