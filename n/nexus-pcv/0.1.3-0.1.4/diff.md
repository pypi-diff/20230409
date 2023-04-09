# Comparing `tmp/nexus_pcv-0.1.3.tar.gz` & `tmp/nexus_pcv-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nexus_pcv-0.1.3.tar", max compression
+gzip compressed data, was "nexus_pcv-0.1.4.tar", max compression
```

## Comparing `nexus_pcv-0.1.3.tar` & `nexus_pcv-0.1.4.tar`

### file list

```diff
@@ -1,15 +1,14 @@
--rw-r--r--   0        0        0    16295 2022-12-09 13:13:30.588222 nexus_pcv-0.1.3/LICENSE
--rw-r--r--   0        0        0     4292 2022-12-09 13:13:30.588222 nexus_pcv-0.1.3/README.md
--rw-r--r--   0        0        0      394 2022-12-09 13:13:30.588222 nexus_pcv-0.1.3/nexus_pcv/__init__.py
--rw-r--r--   0        0        0      169 2022-12-09 13:13:30.588222 nexus_pcv-0.1.3/nexus_pcv/__main__.py
--rw-r--r--   0        0        0     5464 2022-12-09 13:13:30.588222 nexus_pcv-0.1.3/nexus_pcv/apic.py
--rw-r--r--   0        0        0        0 2022-12-09 13:13:30.588222 nexus_pcv-0.1.3/nexus_pcv/cli/__init__.py
--rw-r--r--   0        0        0     2445 2022-12-09 13:13:30.588222 nexus_pcv-0.1.3/nexus_pcv/cli/main.py
--rw-r--r--   0        0        0     4210 2022-12-09 13:13:30.588222 nexus_pcv-0.1.3/nexus_pcv/cli/options.py
--rw-r--r--   0        0        0     5305 2022-12-09 13:13:30.588222 nexus_pcv-0.1.3/nexus_pcv/const.py
--rw-r--r--   0        0        0    11189 2022-12-09 13:13:30.588222 nexus_pcv-0.1.3/nexus_pcv/nae.py
--rw-r--r--   0        0        0     8460 2022-12-09 13:13:30.588222 nexus_pcv-0.1.3/nexus_pcv/ndi.py
--rw-r--r--   0        0        0     9020 2022-12-09 13:13:30.588222 nexus_pcv-0.1.3/nexus_pcv/pcv.py
--rw-r--r--   0        0        0     1914 2022-12-09 13:13:30.588222 nexus_pcv-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     5457 1970-01-01 00:00:00.000000 nexus_pcv-0.1.3/setup.py
--rw-r--r--   0        0        0     5429 1970-01-01 00:00:00.000000 nexus_pcv-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0    16295 2023-04-09 14:07:25.117517 nexus_pcv-0.1.4/LICENSE
+-rw-r--r--   0        0        0     4292 2023-04-09 14:07:25.117517 nexus_pcv-0.1.4/README.md
+-rw-r--r--   0        0        0      394 2023-04-09 14:07:25.117517 nexus_pcv-0.1.4/nexus_pcv/__init__.py
+-rw-r--r--   0        0        0      169 2023-04-09 14:07:25.117517 nexus_pcv-0.1.4/nexus_pcv/__main__.py
+-rw-r--r--   0        0        0     5464 2023-04-09 14:07:25.117517 nexus_pcv-0.1.4/nexus_pcv/apic.py
+-rw-r--r--   0        0        0        0 2023-04-09 14:07:25.117517 nexus_pcv-0.1.4/nexus_pcv/cli/__init__.py
+-rw-r--r--   0        0        0     2488 2023-04-09 14:07:25.117517 nexus_pcv-0.1.4/nexus_pcv/cli/main.py
+-rw-r--r--   0        0        0     4210 2023-04-09 14:07:25.117517 nexus_pcv-0.1.4/nexus_pcv/cli/options.py
+-rw-r--r--   0        0        0     5696 2023-04-09 14:07:25.117517 nexus_pcv-0.1.4/nexus_pcv/const.py
+-rw-r--r--   0        0        0    11189 2023-04-09 14:07:25.121517 nexus_pcv-0.1.4/nexus_pcv/nae.py
+-rw-r--r--   0        0        0     8460 2023-04-09 14:07:25.121517 nexus_pcv-0.1.4/nexus_pcv/ndi.py
+-rw-r--r--   0        0        0    10017 2023-04-09 14:07:25.121517 nexus_pcv-0.1.4/nexus_pcv/pcv.py
+-rw-r--r--   0        0        0     1914 2023-04-09 14:07:25.121517 nexus_pcv-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     5430 1970-01-01 00:00:00.000000 nexus_pcv-0.1.4/PKG-INFO
```

### Comparing `nexus_pcv-0.1.3/LICENSE` & `nexus_pcv-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `nexus_pcv-0.1.3/README.md` & `nexus_pcv-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `nexus_pcv-0.1.3/nexus_pcv/apic.py` & `nexus_pcv-0.1.4/nexus_pcv/apic.py`

 * *Files identical despite different names*

### Comparing `nexus_pcv-0.1.3/nexus_pcv/cli/main.py` & `nexus_pcv-0.1.4/nexus_pcv/cli/main.py`

 * *Files 3% similar despite different names*

```diff
@@ -82,14 +82,16 @@
 
     platform = PCV.Platform.NDI if site else PCV.Platform.NAE
     pcv = PCV(hostname_ip, username, password, domain, timeout, platform)
     if file:
         pcv.load_json_files(file)
     if nac_tf_plan:
         pcv.load_tf_plan(nac_tf_plan)
+    if error_handler.fired:
+        exit()
     if platform is PCV.Platform.NDI:
         pcv.ndi_pcv(name, group, site, suppress_events, output_summary, output_url)
     else:
         pcv.nae_pcv(name, group, suppress_events, output_summary, output_url)
     exit()
```

### Comparing `nexus_pcv-0.1.3/nexus_pcv/cli/options.py` & `nexus_pcv-0.1.4/nexus_pcv/cli/options.py`

 * *Files identical despite different names*

### Comparing `nexus_pcv-0.1.3/nexus_pcv/const.py` & `nexus_pcv-0.1.4/nexus_pcv/const.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,14 +5,26 @@
 from typing import Any, Dict
 
 # Map of RN prefixes and its corresponding class name and key attributes
 RN_PREFIX_CLASSNAME_MAPPINGS: Dict[str, Dict[str, Any]] = {
     "uni": {
         "class": "polUni",
     },
+    "userext": {
+        "class": "aaaUserEp",
+    },
+    "fabric": {
+        "class": "fabricInst",
+    },
+    "hsPols": {
+        "class": "healthPolCont",
+    },
+    "infra": {
+        "class": "infraInfra",
+    },
     "tn": {
         "class": "fvTenant",
         "keys": [
             {
                 "attribute": "name",
                 "regex": ".*",
             }
@@ -252,8 +264,17 @@
         "keys": [
             {
                 "attribute": "name",
                 "regex": ".*",
             }
         ],
     },
+    "pol": {
+        "class": "coopPol",
+        "keys": [
+            {
+                "attribute": "name",
+                "regex": ".*",
+            }
+        ],
+    },
 }
```

### Comparing `nexus_pcv-0.1.3/nexus_pcv/nae.py` & `nexus_pcv-0.1.4/nexus_pcv/nae.py`

 * *Files identical despite different names*

### Comparing `nexus_pcv-0.1.3/nexus_pcv/ndi.py` & `nexus_pcv-0.1.4/nexus_pcv/ndi.py`

 * *Files identical despite different names*

### Comparing `nexus_pcv-0.1.3/nexus_pcv/pcv.py` & `nexus_pcv-0.1.4/nexus_pcv/pcv.py`

 * *Files 10% similar despite different names*

```diff
@@ -48,83 +48,104 @@
             dn = root["dn"]
             for change in tf_plan.get("resource_changes", []):
                 section = (
                     "after" if change["change"].get("after") is not None else "before"
                 )
                 plan_dn = change["change"].get(section, {}).get("dn")
                 if dn == plan_dn:
+                    logger.debug(
+                        "Resolving classname from Terraform plan for '{}'".format(dn)
+                    )
                     root.cl = change["change"].get(section, {}).get("class_name")
-                    root.attributes["name"] = (
+                    name = (
                         change["change"].get(section, {}).get("content", {}).get("name")
                     )
+                    if name:
+                        logger.debug(
+                            "Resolving name attribute from Terraform plan for '{}'".format(
+                                dn
+                            )
+                        )
+                        root.attributes["name"] = name
 
         for child in root.children:
             self._resolve_tf_classnames(child, tf_plan)
 
-    def _resolve_static_classnames(self, root: ApicObject) -> Optional[str]:
+    def _resolve_static_classnames(self, root: ApicObject) -> None:
         """Helper function to resolve missing class names and key attributes using static mappings"""
-        if root.cl is None:
-            parts = str(root["dn"]).split("/")[-1].split("-", 1)
-            prefix = parts[0]
-            name = parts[1] if len(parts) > 1 else None
-            if prefix in RN_PREFIX_CLASSNAME_MAPPINGS:
-                mapping = RN_PREFIX_CLASSNAME_MAPPINGS[prefix]
+        parts = str(root["dn"]).split("/")[-1].split("-", 1)
+        prefix = parts[0]
+        name = parts[1] if len(parts) > 1 else None
+        if prefix in RN_PREFIX_CLASSNAME_MAPPINGS:
+            mapping = RN_PREFIX_CLASSNAME_MAPPINGS[prefix]
+            if root.cl is None:
+                logger.debug(
+                    "Statically resolving classname for '{}'".format(root["dn"])
+                )
                 root.cl = mapping.get("class")
+            if root.cl == mapping.get("class"):
                 for key in mapping.get("keys", []):
                     key_attribute = key.get("attribute")
                     key_regex = key.get("regex")
                     if (
                         key_attribute is not None
                         and key_regex is not None
                         and name is not None
                     ):
                         regex = re.compile(key_regex)
                         mo = regex.search(name)
-                        if mo is not None:
+                        if mo is not None and key_attribute not in root.attributes:
+                            logger.debug(
+                                "Statically adding key attribute '{}' for '{}'".format(
+                                    key_attribute, root["dn"]
+                                )
+                            )
                             root.attributes[key_attribute] = mo.group()
-            if root.cl is None:
-                return str(root["dn"])
         for child in root.children:
             self._resolve_static_classnames(child)
-        return None
+
+    def _check_classes(self, root: ApicObject) -> None:
+        """Helper function to verify if all objects have classnames"""
+        if root.cl is None:
+            logger.error("Missing classname for '{}'".format(root["dn"]))
+        for child in root.children:
+            self._check_classes(child)
 
     def _load_json_objects(
         self, json_dict: Dict[Any, Any], parent: Optional[ApicObject] = None
     ) -> Optional[ApicObject]:
         """Helper function to load JSON objects into object tree"""
         new_obj = None
         for k, v in json_dict.items():
             new_obj = ApicObject(k, v.get("attributes"), [], parent)
             if parent:
                 parent.children.append(new_obj)
             for child in v.get("children", []):
                 self._load_json_objects(child, new_obj)
         return new_obj
 
-    def load_json_files(self, filenames: List[str]) -> Optional[str]:
+    def load_json_files(self, filenames: List[str]) -> None:
         """Load objects from JSON files into object tree"""
         for filename in filenames:
             try:
                 with open(filename, "r") as file:
                     inv = json.loads(file.read())
                     if "imdata" in inv:
                         for item in inv["imdata"]:
                             obj = self._load_json_objects(item)
                             self.root.insert(obj)
                     else:
                         obj = self._load_json_objects(inv)
                         self.root.insert(obj)
             except:  # noqa E722
                 logger.error("Failed to load JSON file: {}".format(filename))
-        err = self._resolve_static_classnames(self.root)
-        if err is not None:
-            return err
-        return None
+        self._resolve_static_classnames(self.root)
+        self._check_classes(self.root)
 
-    def load_tf_plan(self, filename: str) -> Optional[str]:
+    def load_tf_plan(self, filename: str) -> None:
         """Load changed objects from Terraform plan into object tree"""
         tf_plan = None
         with open(filename) as file:
             tf_plan = json.load(file)
 
         for change in tf_plan.get("resource_changes", []):
             if change.get("type") == "aci_rest_managed":
@@ -140,19 +161,17 @@
                         classname = change["change"].get("after", {}).get("class_name")
                         attributes = change["change"].get("after", {}).get("content")
                         attributes["dn"] = change["change"].get("after", {}).get("dn")
                     attributes = {k: v for (k, v) in attributes.items() if v != ""}
                     obj = ApicObject(classname, attributes, [], None)
                     self.root.insert(obj)
 
-        err = self._resolve_static_classnames(self.root)
-        if err is not None:
-            return err
+        self._resolve_static_classnames(self.root)
         self._resolve_tf_classnames(self.root, tf_plan)
-        return None
+        self._check_classes(self.root)
 
     def _write_pcv_events(self, events: List[Any], file: str) -> None:
         with open(file, "w") as fh:
             fh.write(yaml.dump(events, default_flow_style=False))
 
     def _write_pcv_url(self, url: str, file: str) -> None:
         with open(file, "w") as fh:
```

### Comparing `nexus_pcv-0.1.3/pyproject.toml` & `nexus_pcv-0.1.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 documentation = "https://github.com/netascode/nexus-pcv"
 homepage = "https://github.com/netascode/nexus-pcv"
 license = "LICENSE"
 maintainers = ["Daniel Schmidt <danischm@cisco.com>"]
 name = "nexus-pcv"
 readme = "README.md"
 repository = "https://github.com/netascode/nexus-pcv"
-version = "0.1.3"
+version = "0.1.4"
 
 [tool.poetry.scripts]
 nexus-pcv = "nexus_pcv.cli.main:main"
 
 [tool.poetry.dependencies]
 click = "^8.1.3"
 errorhandler = "^2.0.1"
```

### Comparing `nexus_pcv-0.1.3/setup.py` & `nexus_pcv-0.1.4/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,41 +1,103 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: nexus-pcv
+Version: 0.1.4
+Summary: A CLI tool to perform a pre-change validation on Nexus Dashboard Insights or Network Assurance Engine.
+Home-page: https://github.com/netascode/nexus-pcv
+License: LICENSE
+Author: Daniel Schmidt
+Author-email: danischm@cisco.com
+Maintainer: Daniel Schmidt
+Maintainer-email: danischm@cisco.com
+Requires-Python: >=3.7,<4.0
+Classifier: License :: Other/Proprietary License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: click (>=8.1.3,<9.0.0)
+Requires-Dist: errorhandler (>=2.0.1,<3.0.0)
+Requires-Dist: importlib-metadata (>=2.0.0,<3.0.0) ; python_version < "3.8"
+Requires-Dist: pyyaml (>=6.0,<7.0)
+Requires-Dist: requests (>=2.28.1,<3.0.0)
+Project-URL: Documentation, https://github.com/netascode/nexus-pcv
+Project-URL: Repository, https://github.com/netascode/nexus-pcv
+Description-Content-Type: text/markdown
+
+[![Tests](https://github.com/netascode/nexus-pcv/actions/workflows/test.yml/badge.svg)](https://github.com/netascode/nexus-pcv/actions/workflows/test.yml)
+![Python Support](https://img.shields.io/badge/python-3.7%20%7C%203.8%20%7C%203.9%20%7C%203.10-informational "Python Support: 3.7, 3.8, 3.9, 3.10")
+
+# nexus-pcv
+
+A CLI tool to perform a pre-change validation on Nexus Dashboard Insights or Network Assurance Engine. It can either work with provided JSON file(s) or a `terraform plan` output from a [Nexus as Code](https://cisco.com/go/nexusascode) project. It waits for the analysis to complete and evaluates the results.
+
+```
+$ nexus-pcv -h
+Usage: nexus-pcv [OPTIONS]
+
+  A CLI tool to perform a pre-change validation on Nexus Dashboard Insights or
+  Network Assurance Engine.
+
+Options:
+  --version                   Show the version and exit.
+  -v, --verbosity LVL         Either CRITICAL, ERROR, WARNING, INFO or DEBUG.
+  -i, --hostname-ip TEXT      NAE/ND hostname or IP (required, env:
+                              PCV_HOSTNAME_IP).
+  -u, --username TEXT         NAE/ND username (required, env: PCV_USERNAME).
+  -p, --password TEXT         NAE/ND password (required, env: PCV_PASSWORD).
+  -d, --domain TEXT           NAE/ND login domain (optional, default: 'Local',
+                              env: PCV_DOMAIN).
+  -g, --group TEXT            NAE assurance group name or NDI insights group
+                              name (required, env: PCV_GROUP).
+  -s, --site TEXT             NDI site or fabric name (optional, only required
+                              for NDI, env: PCV_SITE).
+  -n, --name TEXT             NAE/NDI pre-change validation name (optional,
+                              env: PCV_NAME).
+  -s, --suppress-events TEXT  NAE/NDI comma-separated list of events to
+                              suppress (optional, default: 'APP_EPG_NOT_DEPLOY
+                              ED,APP_EPG_HAS_NO_CONTRACT_IN_ENFORCED_VRF',
+                              env: PCV_SUPPRESS_EVENTS).
+  -t, --timeout INTEGER       NAE/NDI pre-change validation timeout in minutes
+                              (optional, default: 15, env: PCV_TIMEOUT).
+  -f, --file FILE             NAE/NDI proposed change JSON file (optional,
+                              env: PCV_FILE).
+  -t, --nac-tf-plan FILE      NAE/NDI proposed change Terraform plan output
+                              (optional, env: PCV_NAC_TF_PLAN).
+  -o, --output-summary FILE   NAE/NDI summary of new events/anomalies written
+                              to a file (optional, env: PCV_OUTPUT_SUMMARY).
+  -r, --output-url FILE       NAE/NDI link (URL) to pre-change validation
+                              results written to a file (optional, env:
+                              PCV_OUTPUT_URL).
+  -h, --help                  Show this message and exit.
+```
+
+## Installation
+
+Python 3.7+ is required to install `nexus-pcv`. Don't have Python 3.7 or later? See [Python 3 Installation & Setup Guide](https://realpython.com/installing-python/).
+
+`nexus-pcv` can be installed in a virtual environment using `pip`:
+
+```
+pip install nexus-pcv
+```
+
+## CI/CD Integration
+
+The tool can easily be integrated with CI/CD workflows. Arguments can either be provided via command line or environment variables. The tool will exit with a non-zero exit code in case of an error or non-suppressed events being discovered during the pre-change analysis. The `--output-summary` and `--output-url` arguments can be used to write a summary and/or a link (URL) to a file, which can then be embedded into notifications (e.g., Webex).
+
+## *Nexus as Code* Integration
+
+*Nexus as Code* allows users to instantiate network fabrics in minutes using an easy to use, opinionated data model. More information about *Nexus as Code* can be found [here](https://cisco.com/go/nexusascode). A planned change can be validated before applying it to a production environment by running a `terraform plan` operation first and then providing the output to `nexus-pcv` to trigger a pre-change validation.
+
+```
+export PCV_HOSTNAME_IP=10.1.1.1
+export PCV_USERNAME=admin
+export PCV_PASSWORD=Cisco123
+export PCV_GROUP=LAB
+export PCV_SITE=LAB1
+terraform plan -out=plan.tfplan
+terraform show -json plan.tfplan > plan.json
+nexus-pcv --name "PCV1" --nac-tf-plan plan.json
+```
 
-packages = \
-['nexus_pcv', 'nexus_pcv.cli']
-
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['click>=8.1.3,<9.0.0',
- 'errorhandler>=2.0.1,<3.0.0',
- 'pyyaml>=6.0,<7.0',
- 'requests>=2.28.1,<3.0.0']
-
-extras_require = \
-{':python_version < "3.8"': ['importlib-metadata>=2.0.0,<3.0.0']}
-
-entry_points = \
-{'console_scripts': ['nexus-pcv = nexus_pcv.cli.main:main']}
-
-setup_kwargs = {
-    'name': 'nexus-pcv',
-    'version': '0.1.3',
-    'description': 'A CLI tool to perform a pre-change validation on Nexus Dashboard Insights or Network Assurance Engine.',
-    'long_description': '[![Tests](https://github.com/netascode/nexus-pcv/actions/workflows/test.yml/badge.svg)](https://github.com/netascode/nexus-pcv/actions/workflows/test.yml)\n![Python Support](https://img.shields.io/badge/python-3.7%20%7C%203.8%20%7C%203.9%20%7C%203.10-informational "Python Support: 3.7, 3.8, 3.9, 3.10")\n\n# nexus-pcv\n\nA CLI tool to perform a pre-change validation on Nexus Dashboard Insights or Network Assurance Engine. It can either work with provided JSON file(s) or a `terraform plan` output from a [Nexus as Code](https://cisco.com/go/nexusascode) project. It waits for the analysis to complete and evaluates the results.\n\n```\n$ nexus-pcv -h\nUsage: nexus-pcv [OPTIONS]\n\n  A CLI tool to perform a pre-change validation on Nexus Dashboard Insights or\n  Network Assurance Engine.\n\nOptions:\n  --version                   Show the version and exit.\n  -v, --verbosity LVL         Either CRITICAL, ERROR, WARNING, INFO or DEBUG.\n  -i, --hostname-ip TEXT      NAE/ND hostname or IP (required, env:\n                              PCV_HOSTNAME_IP).\n  -u, --username TEXT         NAE/ND username (required, env: PCV_USERNAME).\n  -p, --password TEXT         NAE/ND password (required, env: PCV_PASSWORD).\n  -d, --domain TEXT           NAE/ND login domain (optional, default: \'Local\',\n                              env: PCV_DOMAIN).\n  -g, --group TEXT            NAE assurance group name or NDI insights group\n                              name (required, env: PCV_GROUP).\n  -s, --site TEXT             NDI site or fabric name (optional, only required\n                              for NDI, env: PCV_SITE).\n  -n, --name TEXT             NAE/NDI pre-change validation name (optional,\n                              env: PCV_NAME).\n  -s, --suppress-events TEXT  NAE/NDI comma-separated list of events to\n                              suppress (optional, default: \'APP_EPG_NOT_DEPLOY\n                              ED,APP_EPG_HAS_NO_CONTRACT_IN_ENFORCED_VRF\',\n                              env: PCV_SUPPRESS_EVENTS).\n  -t, --timeout INTEGER       NAE/NDI pre-change validation timeout in minutes\n                              (optional, default: 15, env: PCV_TIMEOUT).\n  -f, --file FILE             NAE/NDI proposed change JSON file (optional,\n                              env: PCV_FILE).\n  -t, --nac-tf-plan FILE      NAE/NDI proposed change Terraform plan output\n                              (optional, env: PCV_NAC_TF_PLAN).\n  -o, --output-summary FILE   NAE/NDI summary of new events/anomalies written\n                              to a file (optional, env: PCV_OUTPUT_SUMMARY).\n  -r, --output-url FILE       NAE/NDI link (URL) to pre-change validation\n                              results written to a file (optional, env:\n                              PCV_OUTPUT_URL).\n  -h, --help                  Show this message and exit.\n```\n\n## Installation\n\nPython 3.7+ is required to install `nexus-pcv`. Don\'t have Python 3.7 or later? See [Python 3 Installation & Setup Guide](https://realpython.com/installing-python/).\n\n`nexus-pcv` can be installed in a virtual environment using `pip`:\n\n```\npip install nexus-pcv\n```\n\n## CI/CD Integration\n\nThe tool can easily be integrated with CI/CD workflows. Arguments can either be provided via command line or environment variables. The tool will exit with a non-zero exit code in case of an error or non-suppressed events being discovered during the pre-change analysis. The `--output-summary` and `--output-url` arguments can be used to write a summary and/or a link (URL) to a file, which can then be embedded into notifications (e.g., Webex).\n\n## *Nexus as Code* Integration\n\n*Nexus as Code* allows users to instantiate network fabrics in minutes using an easy to use, opinionated data model. More information about *Nexus as Code* can be found [here](https://cisco.com/go/nexusascode). A planned change can be validated before applying it to a production environment by running a `terraform plan` operation first and then providing the output to `nexus-pcv` to trigger a pre-change validation.\n\n```\nexport PCV_HOSTNAME_IP=10.1.1.1\nexport PCV_USERNAME=admin\nexport PCV_PASSWORD=Cisco123\nexport PCV_GROUP=LAB\nexport PCV_SITE=LAB1\nterraform plan -out=plan.tfplan\nterraform show -json plan.tfplan > plan.json\nnexus-pcv --name "PCV1" --nac-tf-plan plan.json\n```\n',
-    'author': 'Daniel Schmidt',
-    'author_email': 'danischm@cisco.com',
-    'maintainer': 'Daniel Schmidt',
-    'maintainer_email': 'danischm@cisco.com',
-    'url': 'https://github.com/netascode/nexus-pcv',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'extras_require': extras_require,
-    'entry_points': entry_points,
-    'python_requires': '>=3.7,<4.0',
-}
-
-
-setup(**setup_kwargs)
```

