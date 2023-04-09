# Comparing `tmp/nprompter-3.7.0.tar.gz` & `tmp/nprompter-3.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nprompter-3.7.0.tar", max compression
+gzip compressed data, was "nprompter-3.8.0.tar", max compression
```

## Comparing `nprompter-3.7.0.tar` & `nprompter-3.8.0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0       56 2023-04-08 14:25:10.942175 nprompter-3.7.0/nprompter/__init__.py
--rw-r--r--   0        0        0     3736 2023-04-08 14:25:10.942175 nprompter-3.7.0/nprompter/__main__.py
--rw-r--r--   0        0        0        0 2023-04-08 14:25:10.942175 nprompter-3.7.0/nprompter/api/__init__.py
--rw-r--r--   0        0        0     2092 2023-04-08 14:25:10.942175 nprompter-3.7.0/nprompter/api/notion_client.py
--rw-r--r--   0        0        0        0 2023-04-08 14:25:10.942175 nprompter-3.7.0/nprompter/cli/__init__.py
--rw-r--r--   0        0        0      144 2023-04-08 14:25:10.942175 nprompter-3.7.0/nprompter/cli/defaults.py
--rw-r--r--   0        0        0      907 2023-04-08 14:25:10.942175 nprompter-3.7.0/nprompter/cli/helpers.py
--rw-r--r--   0        0        0        0 2023-04-08 14:25:10.942175 nprompter-3.7.0/nprompter/processing/__init__.py
--rw-r--r--   0        0        0     8049 2023-04-08 14:25:10.942175 nprompter-3.7.0/nprompter/processing/processor.py
--rw-r--r--   0        0        0        0 2023-04-08 14:25:10.942175 nprompter-3.7.0/nprompter/web/__init__.py
--rw-r--r--   0        0        0    31041 2023-04-08 14:25:10.942175 nprompter-3.7.0/nprompter/web/assets/android-chrome-192x192.png
--rw-r--r--   0        0        0   128229 2023-04-08 14:25:10.942175 nprompter-3.7.0/nprompter/web/assets/android-chrome-512x512.png
--rw-r--r--   0        0        0    29064 2023-04-08 14:25:10.942175 nprompter-3.7.0/nprompter/web/assets/apple-touch-icon.png
--rw-r--r--   0        0        0      845 2023-04-08 14:25:10.942175 nprompter-3.7.0/nprompter/web/assets/favicon-16x16.png
--rw-r--r--   0        0        0     2274 2023-04-08 14:25:10.942175 nprompter-3.7.0/nprompter/web/assets/favicon-32x32.png
--rw-r--r--   0        0        0    15406 2023-04-08 14:25:10.942175 nprompter-3.7.0/nprompter/web/assets/favicon.ico
--rw-r--r--   0        0        0      263 2023-04-08 14:25:10.942175 nprompter-3.7.0/nprompter/web/assets/site.webmanifest
--rw-r--r--   0        0        0      512 2023-04-08 14:25:10.946174 nprompter-3.7.0/nprompter/web/nprompter.toml
--rw-r--r--   0        0        0     1223 2023-04-08 14:25:10.946174 nprompter-3.7.0/nprompter/web/templates/base.html
--rw-r--r--   0        0        0      365 2023-04-08 14:25:10.946174 nprompter-3.7.0/nprompter/web/templates/index.html
--rw-r--r--   0        0        0     4512 2023-04-08 14:25:10.946174 nprompter-3.7.0/nprompter/web/templates/nprompter.css
--rw-r--r--   0        0        0      172 2023-04-08 14:25:10.946174 nprompter-3.7.0/nprompter/web/templates/script.html
--rw-r--r--   0        0        0     6219 2023-04-08 14:25:10.946174 nprompter-3.7.0/nprompter/web/templates/script.js
--rw-r--r--   0        0        0     1379 2023-04-08 14:25:10.946174 nprompter-3.7.0/pyproject.toml
--rw-r--r--   0        0        0     1008 2023-04-08 14:25:54.292517 nprompter-3.7.0/setup.py
--rw-r--r--   0        0        0      688 2023-04-08 14:25:54.292791 nprompter-3.7.0/PKG-INFO
+-rw-r--r--   0        0        0       56 2023-04-09 12:47:46.587272 nprompter-3.8.0/nprompter/__init__.py
+-rw-r--r--   0        0        0     3736 2023-04-09 12:47:46.587272 nprompter-3.8.0/nprompter/__main__.py
+-rw-r--r--   0        0        0        0 2023-04-09 12:47:46.587272 nprompter-3.8.0/nprompter/api/__init__.py
+-rw-r--r--   0        0        0     2092 2023-04-09 12:47:46.587272 nprompter-3.8.0/nprompter/api/notion_client.py
+-rw-r--r--   0        0        0        0 2023-04-09 12:47:46.587272 nprompter-3.8.0/nprompter/cli/__init__.py
+-rw-r--r--   0        0        0      144 2023-04-09 12:47:46.587272 nprompter-3.8.0/nprompter/cli/defaults.py
+-rw-r--r--   0        0        0      907 2023-04-09 12:47:46.587272 nprompter-3.8.0/nprompter/cli/helpers.py
+-rw-r--r--   0        0        0        0 2023-04-09 12:47:46.587272 nprompter-3.8.0/nprompter/processing/__init__.py
+-rw-r--r--   0        0        0     8049 2023-04-09 12:47:46.591272 nprompter-3.8.0/nprompter/processing/processor.py
+-rw-r--r--   0        0        0        0 2023-04-09 12:47:46.591272 nprompter-3.8.0/nprompter/web/__init__.py
+-rw-r--r--   0        0        0    31041 2023-04-09 12:47:46.591272 nprompter-3.8.0/nprompter/web/assets/android-chrome-192x192.png
+-rw-r--r--   0        0        0   128229 2023-04-09 12:47:46.591272 nprompter-3.8.0/nprompter/web/assets/android-chrome-512x512.png
+-rw-r--r--   0        0        0    29064 2023-04-09 12:47:46.591272 nprompter-3.8.0/nprompter/web/assets/apple-touch-icon.png
+-rw-r--r--   0        0        0      845 2023-04-09 12:47:46.591272 nprompter-3.8.0/nprompter/web/assets/favicon-16x16.png
+-rw-r--r--   0        0        0     2274 2023-04-09 12:47:46.591272 nprompter-3.8.0/nprompter/web/assets/favicon-32x32.png
+-rw-r--r--   0        0        0    15406 2023-04-09 12:47:46.591272 nprompter-3.8.0/nprompter/web/assets/favicon.ico
+-rw-r--r--   0        0        0      263 2023-04-09 12:47:46.591272 nprompter-3.8.0/nprompter/web/assets/site.webmanifest
+-rw-r--r--   0        0        0      512 2023-04-09 12:47:46.591272 nprompter-3.8.0/nprompter/web/nprompter.toml
+-rw-r--r--   0        0        0     1223 2023-04-09 12:47:46.591272 nprompter-3.8.0/nprompter/web/templates/base.html
+-rw-r--r--   0        0        0      365 2023-04-09 12:47:46.591272 nprompter-3.8.0/nprompter/web/templates/index.html
+-rw-r--r--   0        0        0     4512 2023-04-09 12:47:46.591272 nprompter-3.8.0/nprompter/web/templates/nprompter.css
+-rw-r--r--   0        0        0      172 2023-04-09 12:47:46.591272 nprompter-3.8.0/nprompter/web/templates/script.html
+-rw-r--r--   0        0        0     6750 2023-04-09 12:47:46.591272 nprompter-3.8.0/nprompter/web/templates/script.js
+-rw-r--r--   0        0        0     1379 2023-04-09 12:47:46.591272 nprompter-3.8.0/pyproject.toml
+-rw-r--r--   0        0        0     1008 2023-04-09 12:48:27.488654 nprompter-3.8.0/setup.py
+-rw-r--r--   0        0        0      688 2023-04-09 12:48:27.488926 nprompter-3.8.0/PKG-INFO
```

### Comparing `nprompter-3.7.0/nprompter/__main__.py` & `nprompter-3.8.0/nprompter/__main__.py`

 * *Files identical despite different names*

### Comparing `nprompter-3.7.0/nprompter/api/notion_client.py` & `nprompter-3.8.0/nprompter/api/notion_client.py`

 * *Files identical despite different names*

### Comparing `nprompter-3.7.0/nprompter/cli/helpers.py` & `nprompter-3.8.0/nprompter/cli/helpers.py`

 * *Files identical despite different names*

### Comparing `nprompter-3.7.0/nprompter/processing/processor.py` & `nprompter-3.8.0/nprompter/processing/processor.py`

 * *Files identical despite different names*

### Comparing `nprompter-3.7.0/nprompter/web/assets/android-chrome-192x192.png` & `nprompter-3.8.0/nprompter/web/assets/android-chrome-192x192.png`

 * *Files identical despite different names*

### Comparing `nprompter-3.7.0/nprompter/web/assets/android-chrome-512x512.png` & `nprompter-3.8.0/nprompter/web/assets/android-chrome-512x512.png`

 * *Files identical despite different names*

### Comparing `nprompter-3.7.0/nprompter/web/assets/apple-touch-icon.png` & `nprompter-3.8.0/nprompter/web/assets/apple-touch-icon.png`

 * *Files identical despite different names*

### Comparing `nprompter-3.7.0/nprompter/web/assets/favicon-16x16.png` & `nprompter-3.8.0/nprompter/web/assets/favicon-16x16.png`

 * *Files identical despite different names*

### Comparing `nprompter-3.7.0/nprompter/web/assets/favicon-32x32.png` & `nprompter-3.8.0/nprompter/web/assets/favicon-32x32.png`

 * *Files identical despite different names*

### Comparing `nprompter-3.7.0/nprompter/web/assets/favicon.ico` & `nprompter-3.8.0/nprompter/web/assets/favicon.ico`

 * *Files identical despite different names*

### Comparing `nprompter-3.7.0/nprompter/web/nprompter.toml` & `nprompter-3.8.0/nprompter/web/nprompter.toml`

 * *Files identical despite different names*

### Comparing `nprompter-3.7.0/nprompter/web/templates/base.html` & `nprompter-3.8.0/nprompter/web/templates/base.html`

 * *Files identical despite different names*

### Comparing `nprompter-3.7.0/nprompter/web/templates/nprompter.css` & `nprompter-3.8.0/nprompter/web/templates/nprompter.css`

 * *Files identical despite different names*

### Comparing `nprompter-3.7.0/nprompter/web/templates/script.js` & `nprompter-3.8.0/nprompter/web/templates/script.js`

 * *Files 4% similar despite different names*

#### js-beautify {}

```diff
@@ -1,13 +1,13 @@
 const content = document.getElementById('content')
 const mirrorElements = Array.from(document.getElementsByClassName('mirror'))
 const modal = document.getElementById('modal')
 const elem = document.documentElement;
 const snackbar = document.getElementById("snackbar");
-const manualScrollAmount = 10;
+const manualScrollAmount = 40;
 const fontSizeIncrease = {
     {
         font.size_increment
     }
 };
 const paddingSizeIncrease = {
     {
@@ -175,28 +175,45 @@
     79: [decreasePadding, "Decrease padding", 'o'],
     80: [increasePadding, "Increase padding", 'p'],
     81: [decreaseLineHeight, "Decrease padding", 'q'],
     87: [increaseLineHeight, "Increase padding", 'w'],
     85: [increaseFontSize, "Increase font size", 'u']
 }
 
+const urlParams = new URLSearchParams(window.location.search);
+if (urlParams.get('presenterMode')) {
+    controls[116] = [toggleScrolling, "Scroll", 'F5']
+    controls[34] = [increaseSpeed, "Scroll", 'F5']
+    controls[33] = [decreaseSpeed, "Scroll", 'F5']
+    controls[27] = [scrollUpManually, "Scroll", 'F5']
+    controls[66] = [scrollDownManually, "Scroll", 'F5']
+}
+
 function handleKeyCode(keyCode) {
     let handled = true;
     if (keyCode in controls) {
         const [action, docs, key] = controls[keyCode]
         const result = action()
         if (result) {
             showInfo(result)
         }
     } else {
         handled = false;
     }
     return handled;
 }
 
+function scrollUpManually() {
+    window.scrollBy(0, -1 * manualScrollAmount);
+}
+
+function scrollDownManually() {
+    window.scrollBy(0, manualScrollAmount);
+}
+
 function pageScroll() {
     window.scrollBy(0, 1); // horizontal and vertical scroll increments
     scrollTimer = setTimeout(pageScroll, scrollSpeed);
 }
 
 function toggleScrolling() {
     if (isScrolling === false) {
```

### Comparing `nprompter-3.7.0/pyproject.toml` & `nprompter-3.8.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nprompter"
-version = "3.7.0"
+version = "3.8.0"
 description = "A web based teleprompter that uses Notion as a storage backend"
 authors = ["Antonio Feregrino <antonio.feregrino@gmail.com>"]
 license = "MIT"
 
 [tool.poetry.scripts]
 nprompter = 'nprompter.__main__:app'
```

### Comparing `nprompter-3.7.0/setup.py` & `nprompter-3.8.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
  'typer>=0.4.1,<0.5.0']
 
 entry_points = \
 {'console_scripts': ['nprompter = nprompter.__main__:app']}
 
 setup_kwargs = {
     'name': 'nprompter',
-    'version': '3.7.0',
+    'version': '3.8.0',
     'description': 'A web based teleprompter that uses Notion as a storage backend',
     'long_description': None,
     'author': 'Antonio Feregrino',
     'author_email': 'antonio.feregrino@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
```

### Comparing `nprompter-3.7.0/PKG-INFO` & `nprompter-3.8.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nprompter
-Version: 3.7.0
+Version: 3.8.0
 Summary: A web based teleprompter that uses Notion as a storage backend
 License: MIT
 Author: Antonio Feregrino
 Author-email: antonio.feregrino@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

