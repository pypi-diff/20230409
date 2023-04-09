# Comparing `tmp/hx_requests-0.6.0.tar.gz` & `tmp/hx_requests-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hx_requests-0.6.0.tar", max compression
+gzip compressed data, was "hx_requests-0.6.1.tar", max compression
```

## Comparing `hx_requests-0.6.0.tar` & `hx_requests-0.6.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1073 2023-04-05 03:43:04.569969 hx_requests-0.6.0/LICENSE
--rw-r--r--   0        0        0     6283 2023-04-05 03:43:04.569969 hx_requests-0.6.0/README.md
--rw-r--r--   0        0        0     1799 2023-04-05 03:43:04.569969 hx_requests-0.6.0/hx_requests/.gitignore
--rw-r--r--   0        0        0       22 2023-04-05 03:43:28.682027 hx_requests-0.6.0/hx_requests/__init__.py
--rw-r--r--   0        0        0      153 2023-04-05 03:43:04.569969 hx_requests-0.6.0/hx_requests/apps.py
--rw-r--r--   0        0        0     1336 2023-04-05 03:43:04.569969 hx_requests-0.6.0/hx_requests/hx_messages.py
--rw-r--r--   0        0        0    10130 2023-04-05 03:43:04.569969 hx_requests-0.6.0/hx_requests/hx_requests.py
--rw-r--r--   0        0        0     1143 2023-04-05 03:43:04.569969 hx_requests-0.6.0/hx_requests/templates/hx_requests/modal.html
--rw-r--r--   0        0        0        0 2023-04-05 03:43:04.569969 hx_requests-0.6.0/hx_requests/templatetags/__init__.py
--rw-r--r--   0        0        0      620 2023-04-05 03:43:04.569969 hx_requests-0.6.0/hx_requests/templatetags/hx_tags.py
--rw-r--r--   0        0        0     1374 2023-04-05 03:43:04.569969 hx_requests-0.6.0/hx_requests/utils.py
--rw-r--r--   0        0        0     2985 2023-04-05 03:43:04.569969 hx_requests-0.6.0/hx_requests/views.py
--rw-r--r--   0        0        0     1435 2023-04-05 03:43:28.694027 hx_requests-0.6.0/pyproject.toml
--rw-r--r--   0        0        0     7500 1970-01-01 00:00:00.000000 hx_requests-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-04-09 20:47:48.760756 hx_requests-0.6.1/LICENSE
+-rw-r--r--   0        0        0     6283 2023-04-09 20:47:48.760756 hx_requests-0.6.1/README.md
+-rw-r--r--   0        0        0     1799 2023-04-09 20:47:48.760756 hx_requests-0.6.1/hx_requests/.gitignore
+-rw-r--r--   0        0        0       22 2023-04-09 20:48:12.249048 hx_requests-0.6.1/hx_requests/__init__.py
+-rw-r--r--   0        0        0      153 2023-04-09 20:47:48.760756 hx_requests-0.6.1/hx_requests/apps.py
+-rw-r--r--   0        0        0     1336 2023-04-09 20:47:48.760756 hx_requests-0.6.1/hx_requests/hx_messages.py
+-rw-r--r--   0        0        0    10765 2023-04-09 20:47:48.760756 hx_requests-0.6.1/hx_requests/hx_requests.py
+-rw-r--r--   0        0        0     1156 2023-04-09 20:47:48.760756 hx_requests-0.6.1/hx_requests/templates/hx_requests/modal.html
+-rw-r--r--   0        0        0        0 2023-04-09 20:47:48.760756 hx_requests-0.6.1/hx_requests/templatetags/__init__.py
+-rw-r--r--   0        0        0      620 2023-04-09 20:47:48.760756 hx_requests-0.6.1/hx_requests/templatetags/hx_tags.py
+-rw-r--r--   0        0        0     1374 2023-04-09 20:47:48.760756 hx_requests-0.6.1/hx_requests/utils.py
+-rw-r--r--   0        0        0     2985 2023-04-09 20:47:48.764756 hx_requests-0.6.1/hx_requests/views.py
+-rw-r--r--   0        0        0     1435 2023-04-09 20:48:12.261048 hx_requests-0.6.1/pyproject.toml
+-rw-r--r--   0        0        0     7500 1970-01-01 00:00:00.000000 hx_requests-0.6.1/PKG-INFO
```

### Comparing `hx_requests-0.6.0/LICENSE` & `hx_requests-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `hx_requests-0.6.0/README.md` & `hx_requests-0.6.1/README.md`

 * *Files identical despite different names*

### Comparing `hx_requests-0.6.0/hx_requests/.gitignore` & `hx_requests-0.6.1/hx_requests/.gitignore`

 * *Files identical despite different names*

### Comparing `hx_requests-0.6.0/hx_requests/hx_messages.py` & `hx_requests-0.6.1/hx_requests/hx_messages.py`

 * *Files identical despite different names*

### Comparing `hx_requests-0.6.0/hx_requests/hx_requests.py` & `hx_requests-0.6.1/hx_requests/hx_requests.py`

 * *Files 3% similar despite different names*

```diff
@@ -253,40 +253,58 @@
 
 
 class HXModal(HXRequestGET):
     name = "hx_modal"
     modal_template = getattr(
         settings, "HX_REQUSTS_MODAL_TEMPLATE", "hx_requests/modal.html"
     )
-    GET_template = ""
-
-    def get(self, request: HttpRequest, *args, **kwargs) -> HttpResponse:
-        if self.GET_template != self.modal_template:
-            self.body = self.GET_template
-            self.GET_template = self.modal_template
-
-        return super().get(request, *args, **kwargs)
+    modal_wrapper_id = getattr(
+        settings, "HX_REQUSTS_MODAL_WRAPPER_ID", "hx_modal_wrapper"
+    )
 
-    def get_context_data(self, **kwargs) -> Dict:
+    def get_GET_context_data(self, **kwargs) -> Dict:
         context = super().get_context_data(**kwargs)
-        body = kwargs.get("body", self.body)
+        body = kwargs.get("body", self.GET_template)
         context["title"] = kwargs.get("title", self.hx_object)
-        context["modal_wrapper_id"] = getattr(
-            settings, "HX_REQUSTS_MODAL_WRAPPER_ID", "hx_modal_wrapper"
-        )
+        context["modal_wrapper_id"] = self.modal_wrapper_id
         context["body"] = (
             render_to_string(body, context=context)
             if body.split(".")[-1] == "html"
             else body
         )
         return context
 
+    def get_GET_response(self, **kwargs):
+        if self.GET_template != self.modal_template:
+            self.body = self.GET_template
+
+        html = render_to_string(
+            self.modal_template, self.get_GET_context_data(**kwargs), self.request
+        )
+
+        return HttpResponse(
+            html,
+            headers=self.get_GET_headers(**kwargs),
+        )
+
 
 class HXFormModal(HXModal, FormHXRequest):
-    pass
+    def get_GET_headers(self, **kwargs) -> Dict:
+        headers = super().get_GET_headers(**kwargs)
+        if self.request.method == "POST":
+            headers["HX-Retarget"] = getattr(
+                settings, "HX_REQUSTS_MODAL_BODY_SELECTOR", "hx_modal_wrapper"
+            )
+        return headers
+
+    def get_POST_headers(self, **kwargs) -> Dict:
+        headers = super().get_POST_headers(**kwargs)
+        if self.form.is_valid():
+            headers["HX-Trigger"] = "modalFormValid"
+        return headers
 
 
 class HXMessagesRequest(HXRequestGET):
     name = "hx_messages"
     GET_template = getattr(settings, "HX_REQUESTS_HX_MESSAGES_TEMPLATE")
 
     def get(self, request: HttpRequest, *args, **kwargs) -> HttpResponse:
```

### Comparing `hx_requests-0.6.0/hx_requests/templates/hx_requests/modal.html` & `hx_requests-0.6.1/hx_requests/templates/hx_requests/modal.html`

 * *Files 22% similar despite different names*

```diff
@@ -17,21 +17,22 @@
                 <button type="button" class="btn btn-secondary" onclick="closeHXModal()">Close</button>
             </div>
         </div>
     </div>
 </div>
 <script>
     function closeHXModal() {
-        const container = document.getElementById('{{modal_wrapper_id}}')
+        const container = document.getElementById('hx_modal_wrapper')
         const backdrop = document.getElementById("modal-backdrop")
         const modal = document.getElementById("modal")
 
         modal.classList.remove("show")
         backdrop.classList.remove("show")
 
         setTimeout(function () {
-            container.removeChild(backdrop)
-            container.removeChild(modal)
+            container.innerHTML = ''
         }, 200)
 }
+       document.addEventListener('modalFormValid',closeHXModal)
+
 
 </script>
```

### Comparing `hx_requests-0.6.0/hx_requests/templatetags/hx_tags.py` & `hx_requests-0.6.1/hx_requests/templatetags/hx_tags.py`

 * *Files identical despite different names*

### Comparing `hx_requests-0.6.0/hx_requests/utils.py` & `hx_requests-0.6.1/hx_requests/utils.py`

 * *Files identical despite different names*

### Comparing `hx_requests-0.6.0/hx_requests/views.py` & `hx_requests-0.6.1/hx_requests/views.py`

 * *Files identical despite different names*

### Comparing `hx_requests-0.6.0/pyproject.toml` & `hx_requests-0.6.1/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "hx-requests"
-version = "0.6.0"
+version = "0.6.1"
 description = "Facilitates the usage of HTMX with Django"
 authors = ["yaakovLowenstein <lowensteinyaakov@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/yaakovLowenstein/hx-requests"
 keywords = ["django", "htmx"]
     classifiers=[
```

### Comparing `hx_requests-0.6.0/PKG-INFO` & `hx_requests-0.6.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hx-requests
-Version: 0.6.0
+Version: 0.6.1
 Summary: Facilitates the usage of HTMX with Django
 Home-page: https://github.com/yaakovLowenstein/hx-requests
 License: MIT
 Keywords: django,htmx
 Author: yaakovLowenstein
 Author-email: lowensteinyaakov@gmail.com
 Requires-Python: >=3.8,<4.0
```

