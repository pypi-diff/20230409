# Comparing `tmp/hx_requests-0.6.1.tar.gz` & `tmp/hx_requests-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hx_requests-0.6.1.tar", max compression
+gzip compressed data, was "hx_requests-0.6.2.tar", max compression
```

## Comparing `hx_requests-0.6.1.tar` & `hx_requests-0.6.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1073 2023-04-09 20:47:48.760756 hx_requests-0.6.1/LICENSE
--rw-r--r--   0        0        0     6283 2023-04-09 20:47:48.760756 hx_requests-0.6.1/README.md
--rw-r--r--   0        0        0     1799 2023-04-09 20:47:48.760756 hx_requests-0.6.1/hx_requests/.gitignore
--rw-r--r--   0        0        0       22 2023-04-09 20:48:12.249048 hx_requests-0.6.1/hx_requests/__init__.py
--rw-r--r--   0        0        0      153 2023-04-09 20:47:48.760756 hx_requests-0.6.1/hx_requests/apps.py
--rw-r--r--   0        0        0     1336 2023-04-09 20:47:48.760756 hx_requests-0.6.1/hx_requests/hx_messages.py
--rw-r--r--   0        0        0    10765 2023-04-09 20:47:48.760756 hx_requests-0.6.1/hx_requests/hx_requests.py
--rw-r--r--   0        0        0     1156 2023-04-09 20:47:48.760756 hx_requests-0.6.1/hx_requests/templates/hx_requests/modal.html
--rw-r--r--   0        0        0        0 2023-04-09 20:47:48.760756 hx_requests-0.6.1/hx_requests/templatetags/__init__.py
--rw-r--r--   0        0        0      620 2023-04-09 20:47:48.760756 hx_requests-0.6.1/hx_requests/templatetags/hx_tags.py
--rw-r--r--   0        0        0     1374 2023-04-09 20:47:48.760756 hx_requests-0.6.1/hx_requests/utils.py
--rw-r--r--   0        0        0     2985 2023-04-09 20:47:48.764756 hx_requests-0.6.1/hx_requests/views.py
--rw-r--r--   0        0        0     1435 2023-04-09 20:48:12.261048 hx_requests-0.6.1/pyproject.toml
--rw-r--r--   0        0        0     7500 1970-01-01 00:00:00.000000 hx_requests-0.6.1/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-04-09 21:06:21.522414 hx_requests-0.6.2/LICENSE
+-rw-r--r--   0        0        0     6283 2023-04-09 21:06:21.522414 hx_requests-0.6.2/README.md
+-rw-r--r--   0        0        0     1799 2023-04-09 21:06:21.522414 hx_requests-0.6.2/hx_requests/.gitignore
+-rw-r--r--   0        0        0       22 2023-04-09 21:06:48.831366 hx_requests-0.6.2/hx_requests/__init__.py
+-rw-r--r--   0        0        0      153 2023-04-09 21:06:21.522414 hx_requests-0.6.2/hx_requests/apps.py
+-rw-r--r--   0        0        0     1336 2023-04-09 21:06:21.522414 hx_requests-0.6.2/hx_requests/hx_messages.py
+-rw-r--r--   0        0        0    10760 2023-04-09 21:06:21.522414 hx_requests-0.6.2/hx_requests/hx_requests.py
+-rw-r--r--   0        0        0     1156 2023-04-09 21:06:21.522414 hx_requests-0.6.2/hx_requests/templates/hx_requests/modal.html
+-rw-r--r--   0        0        0        0 2023-04-09 21:06:21.522414 hx_requests-0.6.2/hx_requests/templatetags/__init__.py
+-rw-r--r--   0        0        0      620 2023-04-09 21:06:21.522414 hx_requests-0.6.2/hx_requests/templatetags/hx_tags.py
+-rw-r--r--   0        0        0     1374 2023-04-09 21:06:21.522414 hx_requests-0.6.2/hx_requests/utils.py
+-rw-r--r--   0        0        0     2985 2023-04-09 21:06:21.522414 hx_requests-0.6.2/hx_requests/views.py
+-rw-r--r--   0        0        0     1435 2023-04-09 21:06:48.843366 hx_requests-0.6.2/pyproject.toml
+-rw-r--r--   0        0        0     7500 1970-01-01 00:00:00.000000 hx_requests-0.6.2/PKG-INFO
```

### Comparing `hx_requests-0.6.1/LICENSE` & `hx_requests-0.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `hx_requests-0.6.1/README.md` & `hx_requests-0.6.2/README.md`

 * *Files identical despite different names*

### Comparing `hx_requests-0.6.1/hx_requests/.gitignore` & `hx_requests-0.6.2/hx_requests/.gitignore`

 * *Files identical despite different names*

### Comparing `hx_requests-0.6.1/hx_requests/hx_messages.py` & `hx_requests-0.6.2/hx_requests/hx_messages.py`

 * *Files identical despite different names*

### Comparing `hx_requests-0.6.1/hx_requests/hx_requests.py` & `hx_requests-0.6.2/hx_requests/hx_requests.py`

 * *Files 1% similar despite different names*

```diff
@@ -288,15 +288,15 @@
 
 
 class HXFormModal(HXModal, FormHXRequest):
     def get_GET_headers(self, **kwargs) -> Dict:
         headers = super().get_GET_headers(**kwargs)
         if self.request.method == "POST":
             headers["HX-Retarget"] = getattr(
-                settings, "HX_REQUSTS_MODAL_BODY_SELECTOR", "hx_modal_wrapper"
+                settings, "HX_REQUSTS_MODAL_BODY_SELECTOR", ".modal-body"
             )
         return headers
 
     def get_POST_headers(self, **kwargs) -> Dict:
         headers = super().get_POST_headers(**kwargs)
         if self.form.is_valid():
             headers["HX-Trigger"] = "modalFormValid"
```

### Comparing `hx_requests-0.6.1/hx_requests/templates/hx_requests/modal.html` & `hx_requests-0.6.2/hx_requests/templates/hx_requests/modal.html`

 * *Files identical despite different names*

### Comparing `hx_requests-0.6.1/hx_requests/templatetags/hx_tags.py` & `hx_requests-0.6.2/hx_requests/templatetags/hx_tags.py`

 * *Files identical despite different names*

### Comparing `hx_requests-0.6.1/hx_requests/utils.py` & `hx_requests-0.6.2/hx_requests/utils.py`

 * *Files identical despite different names*

### Comparing `hx_requests-0.6.1/hx_requests/views.py` & `hx_requests-0.6.2/hx_requests/views.py`

 * *Files identical despite different names*

### Comparing `hx_requests-0.6.1/pyproject.toml` & `hx_requests-0.6.2/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "hx-requests"
-version = "0.6.1"
+version = "0.6.2"
 description = "Facilitates the usage of HTMX with Django"
 authors = ["yaakovLowenstein <lowensteinyaakov@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/yaakovLowenstein/hx-requests"
 keywords = ["django", "htmx"]
     classifiers=[
```

### Comparing `hx_requests-0.6.1/PKG-INFO` & `hx_requests-0.6.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hx-requests
-Version: 0.6.1
+Version: 0.6.2
 Summary: Facilitates the usage of HTMX with Django
 Home-page: https://github.com/yaakovLowenstein/hx-requests
 License: MIT
 Keywords: django,htmx
 Author: yaakovLowenstein
 Author-email: lowensteinyaakov@gmail.com
 Requires-Python: >=3.8,<4.0
```

