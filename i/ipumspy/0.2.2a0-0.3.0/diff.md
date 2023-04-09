# Comparing `tmp/ipumspy-0.2.2a0.tar.gz` & `tmp/ipumspy-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ipumspy-0.2.2a0.tar", max compression
+gzip compressed data, was "ipumspy-0.3.0.tar", max compression
```

## Comparing `ipumspy-0.2.2a0.tar` & `ipumspy-0.3.0.tar`

### file list

```diff
@@ -1,16 +1,15 @@
--rw-r--r--   0        0        0    16725 2021-06-01 20:01:16.730092 ipumspy-0.2.2a0/LICENSE
--rw-r--r--   0        0        0     2256 2023-02-01 02:49:09.015531 ipumspy-0.2.2a0/pyproject.toml
--rw-r--r--   0        0        0       96 2021-11-29 05:15:10.984606 ipumspy-0.2.2a0/src/ipumspy/__init__.py
--rw-r--r--   0        0        0      184 2021-05-26 11:53:27.764723 ipumspy-0.2.2a0/src/ipumspy/__version__.py
--rw-r--r--   0        0        0      119 2021-05-26 11:53:27.764723 ipumspy-0.2.2a0/src/ipumspy/api/__init__.py
--rw-r--r--   0        0        0    18762 2022-03-10 22:22:10.531994 ipumspy-0.2.2a0/src/ipumspy/api/core.py
--rw-r--r--   0        0        0     1108 2022-02-21 19:21:52.921435 ipumspy-0.2.2a0/src/ipumspy/api/exceptions.py
--rw-r--r--   0        0        0    11530 2022-05-23 19:34:27.322522 ipumspy-0.2.2a0/src/ipumspy/api/extract.py
--rw-r--r--   0        0        0     8789 2022-05-19 22:18:28.648199 ipumspy-0.2.2a0/src/ipumspy/cli.py
--rw-r--r--   0        0        0    12365 2022-05-19 22:18:28.648199 ipumspy-0.2.2a0/src/ipumspy/ddi.py
--rw-r--r--   0        0        0     6009 2021-11-19 00:40:28.323558 ipumspy-0.2.2a0/src/ipumspy/fileutils.py
--rw-r--r--   0        0        0    10164 2023-02-01 02:49:09.015531 ipumspy-0.2.2a0/src/ipumspy/readers.py
--rw-r--r--   0        0        0      348 2021-05-26 11:53:27.764723 ipumspy-0.2.2a0/src/ipumspy/types.py
--rw-r--r--   0        0        0     2871 2022-05-19 22:18:28.652199 ipumspy-0.2.2a0/src/ipumspy/utilities.py
--rw-r--r--   0        0        0     1446 1970-01-01 00:00:00.000000 ipumspy-0.2.2a0/setup.py
--rw-r--r--   0        0        0     1397 1970-01-01 00:00:00.000000 ipumspy-0.2.2a0/PKG-INFO
+-rw-r--r--   0        0        0    16725 2023-03-02 23:47:57.339161 ipumspy-0.3.0/LICENSE
+-rw-r--r--   0        0        0     1875 2023-04-09 00:12:02.422109 ipumspy-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0       96 2023-03-06 22:01:08.975231 ipumspy-0.3.0/src/ipumspy/__init__.py
+-rw-r--r--   0        0        0      184 2023-03-06 17:17:16.405993 ipumspy-0.3.0/src/ipumspy/__version__.py
+-rw-r--r--   0        0        0      119 2023-03-06 22:01:08.975231 ipumspy-0.3.0/src/ipumspy/api/__init__.py
+-rw-r--r--   0        0        0    21466 2023-04-09 00:12:02.422109 ipumspy-0.3.0/src/ipumspy/api/core.py
+-rw-r--r--   0        0        0     1108 2023-03-02 23:47:57.349161 ipumspy-0.3.0/src/ipumspy/api/exceptions.py
+-rw-r--r--   0        0        0    25203 2023-04-09 00:12:02.422109 ipumspy-0.3.0/src/ipumspy/api/extract.py
+-rw-r--r--   0        0        0     8789 2023-03-27 14:03:52.671184 ipumspy-0.3.0/src/ipumspy/cli.py
+-rw-r--r--   0        0        0    14371 2023-04-09 00:12:02.422109 ipumspy-0.3.0/src/ipumspy/ddi.py
+-rw-r--r--   0        0        0     6009 2023-03-02 23:47:57.349161 ipumspy-0.3.0/src/ipumspy/fileutils.py
+-rw-r--r--   0        0        0    17330 2023-04-09 00:12:02.422109 ipumspy-0.3.0/src/ipumspy/readers.py
+-rw-r--r--   0        0        0      348 2023-03-02 23:47:57.349161 ipumspy-0.3.0/src/ipumspy/types.py
+-rw-r--r--   0        0        0     1236 2023-04-09 00:12:02.422109 ipumspy-0.3.0/src/ipumspy/utilities.py
+-rw-r--r--   0        0        0      885 1970-01-01 00:00:00.000000 ipumspy-0.3.0/PKG-INFO
```

### Comparing `ipumspy-0.2.2a0/LICENSE` & `ipumspy-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ipumspy-0.2.2a0/pyproject.toml` & `ipumspy-0.3.0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,56 +1,53 @@
 [tool.poetry]
 name = "ipumspy"
-version = "0.2.2a0"
+version = "0.3.0"
 description = "A collection of tools for working with IPUMS data"
 authors = ["Kevin H. Wilson <kevin_wilson@brown.edu>",
            "Renae Rodgers <rodge103@umn.edu>"]
 license = "Mozilla Public License 2.0 (MPL 2.0)"
 packages = [
     { include = "ipumspy", from = "src" }
 ]
 
 [tool.poetry.dependencies]
-python = "^3.7.1"
-pandas = [
-        {version = ">=1.3.5 <1.4.0", python = "<3.10"},
-        {version = "^1.5.2", python = ">=3.10"}
-]
+python = "^3.8"
+pandas = "^1.5.2"
 click = "^8.0.0"
-pyarrow = [
-    {version = "^8.0.0", python = "<3.10"},
-    {version = "^10.0.0", python = ">=3.10"}
-]
-requests = "^2.25.1"
-importlib-metadata = {version = "^4.0.1", python = "<3.8"}
+pyarrow = "^10.0.0"
+requests = {extras = ["use_chardet_on_py3"], version = "^2.26.0"}
+importlib-metadata = "^4.13.0"
 PyYAML = "^5.4.1"
 beautifulsoup4 = "^4.11.1"
 
-# Documentation dependencies
-# Note that these are currently required to be specified in this section
-# until poetry supports dependency groups: python-poetry/poetry#1644
-Sphinx = { version = "^4.1.2", optional = true }
-sphinx-autodoc-typehints = { version = "^1.12.0", optional = true }
-sphinx-copybutton = { version = "^0.4.0", optional = true }
-myst-parser = { version = "^0.15.2", optional = true }
-furo = { version = "^2021.8.31", optional = true }
-
 [tool.poetry.dev-dependencies]
 black = "^22.3.0"
 pylint = "^2.7.4"
 isort = "^5.8.0"
-mypy = "^0.812"
-pytest = "^6.2.3"
-pytest-cov = "^2.12.1"
-python-dotenv = "^0.17.0"
-fastapi = "^0.70.0"
+mypy = "^1.0.1"
+
+[tool.poetry.group.test.dependencies]
+pytest = "^7.2.2"
+pytest-cov = "^4.0.0"
+python-dotenv = "^1.0.0"
+fastapi = "^0.92.0"
 uvicorn = {extras = ["standard"], version = "^0.20.0"}
-pytest-recording = "^0.12.0"
+pytest-recording = "^0.12.2"
 vcrpy = "^4.2.1"
 
+[tool.poetry.group.docs]
+optional=true
+
+[tool.poetry.group.docs.dependencies]
+Sphinx = "^6.1.3"
+sphinx-autodoc-typehints = "^1.22.0"
+sphinx-copybutton = "^0.5.0"
+myst-parser = "^0.19.1"
+furo = "^2022.12.7"
+
 [tool.poetry.extras]
 docs = [
     "Sphinx",
     "sphinx-autodoc-typehints",
     "sphinx-copybutton",
     "myst-parser",
     "furo",
@@ -82,9 +79,9 @@
 
 [tool.coverage.run]
 omit = [
     "*/tests/*",
 ]
 
 [build-system]
-requires = ["poetry>=0.12"]
+requires = ["poetry>=1.4"]
 build-backend = "poetry.masonry.api"
```

### Comparing `ipumspy-0.2.2a0/src/ipumspy/api/core.py` & `ipumspy-0.3.0/src/ipumspy/api/core.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 """
 Core utilities for interacting with the IPUMS API
 """
 import copy
 import time
+import warnings
 from functools import wraps
 from http import HTTPStatus
 from pathlib import Path
-from typing import Any, Dict, List, Optional, Tuple, Union
+from typing import Any, Dict, List, Optional, Tuple, Union, Generator
 
 import requests
 from requests.models import Response
 
 from ..__version__ import __version__
 from ..types import FilenameType
 from .exceptions import (
@@ -22,14 +23,18 @@
     IpumsNotFound,
     IpumsTimeoutException,
     TransientIpumsApiException,
 )
 from .extract import BaseExtract, OtherExtract
 
 
+class ModifiedIpumsExtract(Warning):
+    pass
+
+
 def retry_on_transient_error(func):
     """
     Retry a request up to self.num_retries times. If it exits with a
     ``TransientIpumsApiException``, then retry, else just immediately ``raise``
     """
 
     @wraps(func)
@@ -62,36 +67,28 @@
 def _prettify_message(response_message: Union[str, List[str]]) -> str:
     if isinstance(response_message, list):
         return "\n".join(response_message)
     else:
         return response_message
 
 
-def _reconstitute_purged_extract(
-    collection: str, api_response: Dict[str, Any]
-) -> BaseExtract:
-    return BaseExtract._collection_to_extract[collection].from_api_response(
-        api_response
-    )
-
-
 class IpumsApiClient:
     def __init__(
         self,
         api_key: str,
         base_url: str = "https://api.ipums.org/extracts",
-        api_version: str = "beta",
+        api_version: str = 2,
         num_retries: int = 3,
         session: Optional[requests.Session] = None,
     ):
         """
         Class for creating and retrieving IPUMS extracts via API
 
         Args:
-            api_key: User's IPUMs API key
+            api_key: User's IPUMS API key
             base_url: IPUMS API url
             num_retries: number of times a request will be retried before
                         raising `TransientIpumsApiException`
             session: requests session object
 
         """
 
@@ -131,15 +128,15 @@
                     error_details = _prettify_message(response.json()["error"])
                 except KeyError:
                     error_details = _prettify_message(response.json()["detail"])
                 raise IpumsAPIAuthenticationError(error_details)
             elif response.status_code == HTTPStatus.NOT_FOUND:
                 # No request with the passed error
                 raise IpumsNotFound(
-                    "Page not found. Perhaps you passed the wrong extract id?"
+                    "Page not found. Perhaps you passed the wrong extract id or an invalid page size?"
                 )
             else:
                 error_details = _prettify_message(response.json()["detail"])
                 raise IpumsApiException(error_details)
         except Exception as err:
             raise IpumsApiException(f"other error occured: {err}")
 
@@ -163,41 +160,44 @@
             extract: The extract description to submit. May be either an
                 ``IpumsExtract`` object, or the ``details`` of such an
                 object, in which case it must include a key named ``collection``
 
         Returns:
             The number of the extract for the passed user account
         """
+        # define extract collection
         if not isinstance(extract, BaseExtract):
             extract = copy.deepcopy(extract)
             if "collection" in extract:
                 collection = collection or extract["collection"]
                 del extract["collection"]
             else:
                 if not collection:
                     ValueError("You must provide a collection")
 
             if collection in BaseExtract._collection_to_extract:
                 extract_type = BaseExtract._collection_to_extract[collection]
                 extract = extract_type(**extract)
             else:
                 extract = OtherExtract(collection, extract)
-
+        # if no api version was provided on instantiation of extract object
+        # or in extract definition dict, assign it to the default
+        if extract.api_version is None:
+            extract.api_version = self.api_version
         response = self.post(
             self.base_url,
-            params={"collection": extract.collection, "version": self.api_version},
+            params={"collection": extract.collection, "version": extract.api_version},
             json=extract.build(),
         )
 
         extract_id = int(response.json()["number"])
         extract._id = extract_id
 
         extract_info = response.json()
         extract._info = extract_info
-        extract.api_version = self.api_version
         return extract
 
     def extract_status(
         self, extract: Union[BaseExtract, int], collection: Optional[str] = None
     ) -> str:
         """
         Check on the status of an extract request. If no such extract exists, return
@@ -285,40 +285,46 @@
             )
 
         response = self.get(
             f"{self.base_url}/{extract_id}",
             params={"collection": collection, "version": self.api_version},
         )
 
-        download_links = response.json()["download_links"]
+        download_links = response.json()["downloadLinks"]
         try:
-            # if the extract has been purged, the download_links element will be
+            # if the extract has been expired, the download_links element will be
             # an empty dict
             data_url = download_links["data"]["url"]
-            ddi_url = download_links["ddi_codebook"]["url"]
+            ddi_url = download_links["ddiCodebook"]["url"]
             download_urls = [data_url, ddi_url]
 
             if stata_command_file:
-                _url = download_links["stata_command_file"]["url"]
+                _url = download_links["stataCommandFile"]["url"]
                 download_urls.append(_url)
             if spss_command_file:
-                _url = download_links["spss_command_file"]["url"]
+                _url = download_links["spssCommandFile"]["url"]
                 download_urls.append(_url)
             if sas_command_file:
-                _url = download_links["sas_command_file"]["url"]
+                _url = download_links["sasCommandFile"]["url"]
                 download_urls.append(_url)
             if r_command_file:
-                _url = download_links["R_command_file"]["url"]
+                _url = download_links["rCommandFile"]["url"]
                 download_urls.append(_url)
 
         except KeyError:
-            raise IpumsExtractNotReady(
-                f"Your IPUMS {collection} extract number {extract_id} was purged "
-                f"from our cache. Please resubmit your extract."
-            )
+            if isinstance(extract, BaseExtract):
+                raise IpumsExtractNotReady(
+                    f"IPUMS {collection} extract {extract_id} has expired and its files have been deleted.\n"
+                    f"Use `submit_extract() to resubmit this extract object as a new extract request."
+                )
+            else:
+                raise IpumsExtractNotReady(
+                    f"IPUMS {collection} extract {extract_id} has expired and its files have been deleted.\n"
+                    f"Use `get_extract_by_id()` and `submit_extract()` to resubmit this definition as a new extract request."
+                )
         for url in download_urls:
             file_name = url.split("/")[-1]
             download_path = download_dir / file_name
             with self.get(url, stream=True) as response:
                 response.raise_for_status()
                 with open(download_path, "wb") as outfile:
                     for chunk in response.iter_content(chunk_size=8192):
@@ -378,33 +384,31 @@
             elif status != "completed":
                 time.sleep(wait_time)
                 total_time += wait_time
                 wait_time = min(wait_time * 2, max_wait_time)
             else:
                 break
 
-    def retrieve_previous_extracts(
-        self, collection: str, limit: int = 10
-    ) -> List[Dict]:
+    def get_previous_extracts(self, collection: str, limit: int = 10) -> List[Dict]:
         """
         Return details about the past ``limit`` requests
 
         Args:
             collection: The collection for which to look up most recent previous extracts.
-            limit: The number of extracts to look up. Default is 10
+            limit: The number of most recent extracts to look up. Default is 10
 
         Returns:
             A list of the user's most recent previous extract definitions.
         """
         # TODO: Wrap results in Extract objects.
         output = self.get(
             self.base_url,
             params={
                 "collection": collection,
-                "limit": limit,
+                "pageSize": limit,
                 "version": self.api_version,
             },
         ).json()
         return output
 
     def get_extract_info(
         self,
@@ -428,58 +432,125 @@
         if isinstance(extract, BaseExtract):
             return extract._info
         else:
             extract_info = self.get(
                 f"{self.base_url}/{extract_id}",
                 params={"collection": collection, "version": self.api_version},
             ).json()
-
+            new_line = "\n"
+            if "warnings" in extract_info.keys():
+                warnings.warn(
+                    f"This IPUMS extract has been modified from its original form to remove invalid content and features:{new_line}"
+                    f"{new_line.join(extract_info['warnings'])}",
+                    ModifiedIpumsExtract,
+                )
             return extract_info
 
-    def extract_was_purged(
+    def get_extract_by_id(
+        self,
+        extract_id: int,
+        collection: str,
+    ) -> BaseExtract:
+        """
+        Convenience method to get a specific previously-submitted IPUMS extract.
+
+        Args:
+            collection: An IPUMS data collection
+            extract_id: IPUMS extract id number to retrieve
+
+        Returns:
+            An IPUMS extract object
+        """
+        extract_def = self.get_extract_info(extract_id, collection)
+        if collection in BaseExtract._collection_to_extract:
+            extract_type = BaseExtract._collection_to_extract[collection]
+            extract = extract_type(**extract_def["extractDefinition"])
+        else:
+            extract = OtherExtract(collection, extract)
+        return extract
+
+    def extract_is_expired(
         self,
         extract: Union[BaseExtract, int],
         collection: Optional[str] = None,
     ) -> bool:
         """
-        Returns True if the IPUMS extract's files have been purged from the cache.
+        Returns True if the IPUMS extract's files have been expired from the cache.
 
         extract: An extract object. This extract must have been submitted.
                  Alternatively, can be an extract id. If an extract id is provided, you
                  must supply the collection name
         collection: The name of the collection to pull the extract from. If None,
             then ``extract`` must be a ``BaseExtract``
         """
         extract_id, collection = _extract_and_collection(extract, collection)
         extract_definition = self.get_extract_info(extract_id, collection)
-        if not extract_definition["download_links"]:
+        if not extract_definition["downloadLinks"]:
             return True
         else:
             return False
 
-    def resubmit_purged_extract(self, extract: str, collection: str):
+    def _get_pages(
+        self, collection: str, page_size: Optional[int] = 2500
+    ) -> Generator[Dict, None, None]:
         """
-        Re-submits an IPUMS extract for which the data and ddi files have been purged
-        from the IPUMS extract system cache.
+        An IPUMS API pages generator.
 
         Args:
-            collection: The collection of the purged extract to be re-submitted
-            extract_id: The extract id of the purged extract to be re-submitted
+            collection: An IPUMS data collection
+            page_size: The number of items to return per page. Default to maximum page size, 2500.
 
-        Returns:
-            An IPUMS extract object. NB: the re-submitted extract will have its own
-            extract id number, different from the extract_id of the purged extract!
+        Yields:
+            IPUMS API page JSON
         """
+        # made this a private method looking forward to making this a more
+        # general purpose generator for non-extract endpoints
+        first_page = self.get(
+            self.base_url,
+            params={
+                "collection": collection,
+                "version": self.api_version,
+                "pageSize": page_size,
+            },
+        ).json()
+        yield first_page
+        next_page = first_page["links"]["nextPage"]
 
-        if self.extract_was_purged(collection=collection, extract=extract):
-            extract_definition = self.get_extract_info(extract, collection)
-            base_obj = _reconstitute_purged_extract(collection, extract_definition)
-            base_obj.description = f"Revision of ({base_obj.description})"
-            extract_obj = self.submit_extract(base_obj, collection=collection)
+        while next_page is not None:
+            page = self.get(next_page).json()
+            yield page
+            next_page = page["links"]["nextPage"]
+
+    def get_extract_history(
+        self, collection: str, page_size: Optional[int] = 2500
+    ) -> Generator[Dict, None, None]:
+        """
+        Retrieve extract history for a specific collection.
 
-            return extract_obj
-        else:
-            raise IpumsApiException(
-                f"IPUMS {collection} extract number {extract} "
-                f"has not been purged. You may download the data "
-                f"and ddi files directly using download_extract()"
-            )
+        Args:
+            collection: An IPUMS data collection
+            page_size: The number of items to return per page. Default to maximum page size, 2500.
+
+        Yields:
+            An iterator of extract history pages
+        """
+        yield from self._get_pages(collection, page_size)
+
+    def get_all_sample_info(self, collection: str) -> Dict:
+        """
+        Retrieve sample descriptions and ids for all samples in an IPUMS collection.
+
+        Args:
+            collection: An IPUMS data collection
+
+        Returns:
+            A dictionary of IPUMS sample descriptions and IPUMS sample IDs; keys are
+            sample ids, values are sample descriptions
+        """
+        # shoehorn since this is the only metadata api endpoint avaialble
+        url = f"https://api.ipums.org/metadata/{collection}/samples"
+        samples = self.get(url, params={"version": self.api_version}).json()
+        # make it into the expected dict
+        samples_dict = {}
+        for item in samples["data"]:
+            samples_dict[item["name"]] = item["description"]
+        return samples_dict
```

### Comparing `ipumspy-0.2.2a0/src/ipumspy/api/exceptions.py` & `ipumspy-0.3.0/src/ipumspy/api/exceptions.py`

 * *Files identical despite different names*

### Comparing `ipumspy-0.2.2a0/src/ipumspy/cli.py` & `ipumspy-0.3.0/src/ipumspy/cli.py`

 * *Files identical despite different names*

### Comparing `ipumspy-0.2.2a0/src/ipumspy/ddi.py` & `ipumspy-0.3.0/src/ipumspy/ddi.py`

 * *Files 8% similar despite different names*

```diff
@@ -26,31 +26,32 @@
 
     # pylint: disable=too-many-instance-attributes
 
     id: str  # pylint: disable=invalid-name
     """variable id (this is the same as its name)"""
     name: str
     """variable name"""
+    rectype: str
+    """record type"""
     codes: Dict[str, Union[int, str]]
     """a dictionary of codes and value labels"""
-
     start: int
     """variable's starting column in the extract data file"""
     end: int
     """variable's final column in the extract data file"""
-
     label: str
     """variable label"""
     description: str
     """variable description"""
     concept: str
     """IPUMS variable group"""
-
     vartype: str
     """variable data type"""
+    notes: str
+    """notes about this variable from the ddi"""
     shift: Optional[int]
     """number of implied decimal places"""
 
     @property
     def python_type(self) -> type:
         """
         The Python type of this variable.
@@ -119,28 +120,40 @@
             label = cat.find("./ddi:labl", namespaces).text
             value = cat.find("./ddi:catValu", namespaces).text
             # make values integers when possible
             if vartype == "numeric":
                 labels_dict[label] = int(value)
             else:
                 labels_dict[label] = value
-
+        # rectype attribute only exists for hierarchical extracts
+        try:
+            var_rectype = elt.attrib["rectype"]
+        # stick an empty string in this attribute for rectangular extracts
+        except KeyError:
+            var_rectype = ""
+        # if a variable has notes, capture those
+        try:
+            var_notes = elt.find("./ddi:notes", namespaces).text
+        except AttributeError:
+            var_notes = ""
         return cls(
             id=elt.attrib["ID"],
             name=elt.attrib["name"],
+            rectype=var_rectype,
             codes=labels_dict,
             start=int(elt.find("./ddi:location", namespaces).attrib["StartPos"])
             - 1,  # 0 based in python
             end=int(
                 elt.find("./ddi:location", namespaces).attrib["EndPos"]
             ),  # Exclusive ends in python
             label=elt.find("./ddi:labl", namespaces).text,
             description=elt.find("./ddi:txt", namespaces).text,
             concept=elt.find("./ddi:concept", namespaces).text,
             vartype=vartype,
+            notes=var_notes,
             shift=int(elt.attrib.get("dcml")) if "dcml" in elt.attrib else None,
         )
 
 
 @dataclass(frozen=True)
 class FileDescription:
     """
@@ -153,14 +166,29 @@
     description: str
     """IPUMS ddi file description"""
     structure: str
     """
     IPUMS extract data file structure.
     Valid structures: rectangular, hierarchical
     """
+    rectypes: List
+    """
+    Record types included in the IPUMS extract.
+    This is an empty list for rectangular extracts.
+    """
+    rectype_idvar: str
+    """
+    The variable that identifies record types.
+    This is an empty string for rectangular extracts.
+    """
+    rectype_keyvar: str
+    """
+    The variable that uniquely identifies records across record types.
+    This is an empty string for rectangular extracts.
+    """
     encoding: str
     """IPUMS file encoding scheme"""
     format: str
     """IPUMS extract data file format"""
     place: str
     """IPUMS physical address"""
 
@@ -172,18 +200,41 @@
         Args:
             elt: xml element tree from parsed extract ddi
             ddi_namespace: ddi namespace that says what the xmlns is for the file
         Returns:
             FileDescription object
         """
         namespaces = {"ddi": ddi_namespace}
+
+        # only hierarchical files have recGrp information
+        try:
+            file_rectypes = elt.findall("./ddi:fileStrc/ddi:recGrp", namespaces)
+            rts = [rectype.attrib["rectype"] for rectype in file_rectypes]
+        except KeyError:
+            rts = []
+        # rectype get rectype id var and rectype key var
+        # these should be the same across record types for all collections
+        # so we should be fine to just grab the first appearance of recidvar and keyvar
+        try:
+            rectype_idvar = elt.find("./ddi:fileStrc/ddi:recGrp", namespaces).attrib[
+                "recidvar"
+            ]
+            rectype_keyvar = elt.find("./ddi:fileStrc/ddi:recGrp", namespaces).attrib[
+                "keyvar"
+            ]
+        except AttributeError:
+            rectype_idvar = ""
+            rectype_keyvar = ""
         return cls(
             filename=elt.find("./ddi:fileName", namespaces).text,
             description=elt.find("./ddi:fileCont", namespaces).text,
             structure=elt.find("./ddi:fileStrc", namespaces).attrib["type"],
+            rectypes=rts,
+            rectype_idvar=rectype_idvar,
+            rectype_keyvar=rectype_keyvar,
             encoding=elt.find("./ddi:fileType", namespaces)
             .attrib.get("charset", "iso-8859-1")
             .lower(),
             format=elt.find("./ddi:format", namespaces).text,
             place=elt.find("./ddi:filePlac", namespaces).text,
         )
```

### Comparing `ipumspy-0.2.2a0/src/ipumspy/fileutils.py` & `ipumspy-0.3.0/src/ipumspy/fileutils.py`

 * *Files identical despite different names*

### Comparing `ipumspy-0.2.2a0/src/ipumspy/readers.py` & `ipumspy-0.3.0/src/ipumspy/readers.py`

 * *Files 25% similar despite different names*

```diff
@@ -8,17 +8,18 @@
 """
 import copy
 import json
 import re
 import warnings
 import xml.etree.ElementTree as ET
 from pathlib import Path
-from typing import Iterator, List, Optional, Union
+from typing import Iterator, List, Optional, Union, Dict
 
 import pandas as pd
+import numpy as np
 import yaml
 
 from . import ddi as ddi_definitions
 from . import fileutils
 from .fileutils import open_or_yield
 from .types import FilenameType
 
@@ -58,18 +59,18 @@
     ddi: ddi_definitions.Codebook,
     filename: Optional[fileutils.FileType] = None,
     encoding: Optional[str] = None,
     subset: Optional[List[str]] = None,
     iterator: bool = False,
     chunksize: Optional[int] = None,
     dtype: Optional[dict] = None,
-    **kwargs
+    **kwargs,
 ):
-    if ddi.file_description.structure != "rectangular":
-        raise NotImplementedError("Structure must be rectangular")
+    # if ddi.file_description.structure != "rectangular":
+    #     raise NotImplementedError("Structure must be rectangular")
 
     if subset is not None:
         data_description = [
             desc for desc in ddi.data_description if desc.name in subset
         ]
     else:
         data_description = ddi.data_description
@@ -149,35 +150,94 @@
         else:
             kwargs.update({"iterator": True, "chunksize": chunksize})
             data = reader(infile, **kwargs)
 
         if dtype is None:
             yield from (
                 _fix_decimal_expansion(df).astype(
-                    {desc.name: desc.pandas_type for desc in ddi.data_description}
+                    {desc.name: desc.pandas_type for desc in data_description}
                 )
                 for df in data
             )
         else:
             if ".dat" in filename.suffixes:
                 # convert variables from default numpy_type to corresponding type in dtype.
                 yield from (_fix_decimal_expansion(df).astype(dtype) for df in data)
             else:
                 # In contrary to counter condition, df already has right dtype. It would be expensive to call astype for
                 # nothing.
                 yield from (_fix_decimal_expansion(df) for df in data)
 
 
+def _read_hierarchical_microdata(
+    ddi: ddi_definitions.Codebook,
+    filename: Optional[fileutils.FileType] = None,
+    encoding: Optional[str] = None,
+    subset: Optional[List[str]] = None,
+    iterator: bool = False,
+    chunksize: Optional[int] = 100000,
+    dtype: Optional[dict] = None,
+    **kwargs,
+):
+    # TODO: try and speed this up
+    if subset is not None:
+        data_description = [
+            desc for desc in ddi.data_description if desc.name in subset
+        ]
+    else:
+        data_description = ddi.data_description
+
+    # identify common variables
+    # these variables have all rectypes listed in the variable-level rectype attribute
+    # these are delimited by spaces within the string attribute
+    # this list would probably be a useful thing to have as a file-level attribute...
+    common_vars = [
+        desc.name
+        for desc in data_description
+        if sorted(desc.rectype.split(" ")) == sorted(ddi.file_description.rectypes)
+    ]
+    # seperate variables by rectype
+    rectypes = {}
+    # NB: This might result in empty data frames for some rectypes
+    # as the ddi contains all possible collection rectypes, even if only a few
+    # are actually represented in the file.
+    # TODO: prune empty rectype data frames
+    for rectype in ddi.file_description.rectypes:
+        rectype_vars = []
+        rectype_vars.extend(common_vars)
+        for desc in data_description:
+            if desc.rectype == rectype:
+                rectype_vars.append(desc.name)
+        # read microdata for the relevant rectype variables only
+        # and do it in chunks so it goes quicker
+        rectypes[rectype] = next(
+            read_microdata_chunked(
+                ddi,
+                filename,
+                encoding,
+                # rectype vars are the subset
+                rectype_vars,
+                chunksize,
+                dtype,
+                **kwargs,
+            )
+        )
+        # retain only records from the relevant record type
+        rt_df = rectypes[rectype]
+        rectypes[rectype] = rt_df[rt_df["RECTYPE"] == rectype]
+    return rectypes
+
+
 def read_microdata(
     ddi: ddi_definitions.Codebook,
     filename: Optional[fileutils.FileType] = None,
     encoding: Optional[str] = None,
     subset: Optional[List[str]] = None,
     dtype: Optional[dict] = None,
-    **kwargs
+    **kwargs,
 ) -> Union[pd.DataFrame, pd.io.parsers.TextFileReader]:
     """
     Read in microdata as specified by the Codebook. Both .dat and .csv file types
     are supported.
 
     Args:
         ddi: The codebook representing the data
@@ -194,34 +254,130 @@
             occur: one on load, and one when returning the dataframe.
         kwargs: keyword args to be passed to the engine (pd.read_fwf, pd.read_csv, or
             pd.read_parquet depending on the file type)
 
     Returns:
         pandas data frame and pandas text file reader
     """
-    return next(
-        _read_microdata(
-            ddi,
-            filename=filename,
-            encoding=encoding,
-            subset=subset,
-            dtype=dtype,
-            **kwargs
+    # raise a warning if this is a hierarchical file
+    if ddi.file_description.structure == "hierarchical":
+        raise NotImplementedError(
+            "Structure must be rectangular. Use `read_hierarchical_microdata()` for hierarchical extracts."
         )
-    )
+    # just read it if its rectangular
+    else:
+        return next(
+            _read_microdata(
+                ddi,
+                filename=filename,
+                encoding=encoding,
+                subset=subset,
+                dtype=dtype,
+                **kwargs,
+            )
+        )
+
+
+def read_hierarchical_microdata(
+    ddi: ddi_definitions.Codebook,
+    filename: Optional[fileutils.FileType] = None,
+    encoding: Optional[str] = None,
+    subset: Optional[List[str]] = None,
+    dtype: Optional[dict] = None,
+    as_dict: Optional[bool] = True,
+    **kwargs,
+) -> Union[pd.DataFrame, Dict]:
+    """
+    Read in microdata as specified by the Codebook. Both .dat and .csv file types
+    are supported.
+
+    Args:
+        ddi: The codebook representing the data
+        filename: The path to the data file. If not present, gets from
+                        ddi and assumes the file is relative to the current
+                        working directory
+        encoding: The encoding of the data file. If not present, reads from ddi
+        subset: A list of variable names to keep. If None, will keep all
+        dtype: A dictionary with variable names as keys and variable types as values.
+            Has an effect only when used with pd.read_fwf or pd.read_csv engine. If None, pd.read_fwf or pd.read_csv use
+            type ddi.data_description.pandas_type for all variables. See ipumspy.ddi.VariableDescription for more
+            precision on ddi.data_description.pandas_type. If files are csv, and dtype is not None, pandas converts the
+            column types once: on pd.read_csv call. When file format is .dat or .csv and dtype is None, two conversion
+            occur: one on load, and one when returning the dataframe.
+        as_dict: A flag to indicate whether to return a single data frame or a dictionary with one data frame per record
+            type in the extract data file. Set to True to recieve a dictionary of data frames.
+        kwargs: keyword args to be passed to the engine (pd.read_fwf, pd.read_csv, or
+            pd.read_parquet depending on the file type)
+
+    Returns:
+        pandas data frame or a dictionary of pandas data frames
+    """
+    # hack for now just to have it in this method - make this a ddi.file_description attribute.
+    common_vars = [
+        desc.name
+        for desc in ddi.data_description
+        if sorted(desc.rectype.split(" ")) == sorted(ddi.file_description.rectypes)
+    ]
+    # RECTYPE must be included if subset list is specified
+    if subset is not None and "RECTYPE" not in subset:
+        raise ValueError(
+            "RECTYPE must be included in the subset list for hierarchical extracts."
+        )
+    # raise a warning if this is a rectantgular file
+    if ddi.file_description.structure == "rectangular":
+        raise NotImplementedError(
+            "Structure must be hierarchical. Use `read_microdata()` for rectangular extracts."
+        )
+    else:
+        df_dict = _read_hierarchical_microdata(
+            ddi, filename, encoding, subset, dtype, **kwargs
+        )
+        if as_dict:
+            return df_dict
+        else:
+            # read the hierarchical file
+            df = next(_read_microdata(ddi, filename, encoding, subset, dtype, **kwargs))
+            # for each rectype, nullify variables that belong to other rectypes
+            for rectype in df_dict.keys():
+                # create a list of variables that are for rectypes other than the current rectype
+                # and are not included in the list of varaibles that are common across rectypes
+                non_rt_cols = [
+                    cols
+                    for rt in df_dict.keys()
+                    for cols in df_dict[rt].columns
+                    if rt != rectype and cols not in common_vars
+                ]
+                for col in non_rt_cols:
+                    # maintain data type when "nullifying" variables from other record types
+                    if df[col].dtype == pd.Int64Dtype():
+                        df[col] = np.where(df["RECTYPE"] == rectype, pd.NA, df[col])
+                        df[col] = df[col].astype(pd.Int64Dtype())
+                    elif df[col].dtype == pd.StringDtype():
+                        df[col] = np.where(df["RECTYPE"] == rectype, "", df[col])
+                        df[col] = df[col].astype(pd.StringDtype())
+                    elif df[col].dtype == float:
+                        df[col] = np.where(df["RECTYPE"] == rectype, np.nan, df[col])
+                        df[col] = df[col].astype(float)
+                    # this should (theoretically) never be hit... unless someone specifies an illegal data type
+                    # themselves, but that should also be caught before this stage.
+                    else:
+                        raise TypeError(
+                            f"Data type {df[col].dtype} for {col} is not an allowed type."
+                        )
+            return df
 
 
 def read_microdata_chunked(
     ddi: ddi_definitions.Codebook,
     filename: Optional[fileutils.FileType] = None,
     encoding: Optional[str] = None,
     subset: Optional[List[str]] = None,
     chunksize: Optional[int] = None,
     dtype: Optional[dict] = None,
-    **kwargs
+    **kwargs,
 ) -> Iterator[pd.DataFrame]:
     """
     Read in microdata in chunks as specified by the Codebook.
     As these files are often large, you may wish to filter or read in chunks.
     As an example of how you might do that, consider the following example that
     filters only for rows in Rhode Island::
 
@@ -249,15 +405,15 @@
         ddi,
         filename=filename,
         encoding=encoding,
         subset=subset,
         iterator=True,
         dtype=dtype,
         chunksize=chunksize,
-        **kwargs
+        **kwargs,
     )
 
 
 def read_extract_description(extract_filename: FilenameType) -> dict:
     """
     Open an extract description (either yaml or json are accepted) and return it
     as a dictionary.
```

### Comparing `ipumspy-0.2.2a0/PKG-INFO` & `ipumspy-0.3.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,29 +1,22 @@
 Metadata-Version: 2.1
 Name: ipumspy
-Version: 0.2.2a0
+Version: 0.3.0
 Summary: A collection of tools for working with IPUMS data
 License: Mozilla Public License 2.0 (MPL 2.0)
 Author: Kevin H. Wilson
 Author-email: kevin_wilson@brown.edu
-Requires-Python: >=3.7.1,<4.0.0
+Requires-Python: >=3.8,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: docs
 Requires-Dist: PyYAML (>=5.4.1,<6.0.0)
-Requires-Dist: Sphinx (>=4.1.2,<5.0.0); extra == "docs"
 Requires-Dist: beautifulsoup4 (>=4.11.1,<5.0.0)
 Requires-Dist: click (>=8.0.0,<9.0.0)
-Requires-Dist: furo (>=2021.8.31,<2022.0.0); extra == "docs"
-Requires-Dist: importlib-metadata (>=4.0.1,<5.0.0); python_version < "3.8"
-Requires-Dist: myst-parser (>=0.15.2,<0.16.0); extra == "docs"
-Requires-Dist: pandas (>=1.3.5,<1.4.0); python_version < "3.10"
-Requires-Dist: pandas (>=1.5.2,<2.0.0); python_version >= "3.10"
-Requires-Dist: pyarrow (>=10.0.0,<11.0.0); python_version >= "3.10"
-Requires-Dist: pyarrow (>=8.0.0,<9.0.0); python_version < "3.10"
-Requires-Dist: requests (>=2.25.1,<3.0.0)
-Requires-Dist: sphinx-autodoc-typehints (>=1.12.0,<2.0.0); extra == "docs"
-Requires-Dist: sphinx-copybutton (>=0.4.0,<0.5.0); extra == "docs"
+Requires-Dist: importlib-metadata (>=4.13.0,<5.0.0)
+Requires-Dist: pandas (>=1.5.2,<2.0.0)
+Requires-Dist: pyarrow (>=10.0.0,<11.0.0)
+Requires-Dist: requests[use-chardet-on-py3] (>=2.26.0,<3.0.0)
```

