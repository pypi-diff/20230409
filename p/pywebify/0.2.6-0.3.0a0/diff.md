# Comparing `tmp/pywebify-0.2.6.tar.gz` & `tmp/pywebify-0.3.0a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\pywebify-0.2.6.tar", last modified: Thu Jul  9 20:16:41 2020, max compression
+gzip compressed data, was "pywebify-0.3.0a0.tar", last modified: Sun Apr  9 16:29:28 2023, max compression
```

## Comparing `pywebify-0.2.6.tar` & `pywebify-0.3.0a0.tar`

### file list

```diff
@@ -1,43 +1,45 @@
-drwxrwxrwx   0        0        0        0 2020-07-09 20:16:40.000000 pywebify-0.2.6/
--rw-rw-rw-   0        0        0       18 2018-10-08 23:52:38.000000 pywebify-0.2.6/MANIFEST.in
--rw-rw-rw-   0        0        0      480 2020-07-09 20:16:40.000000 pywebify-0.2.6/PKG-INFO
-drwxrwxrwx   0        0        0        0 2020-07-09 20:16:40.000000 pywebify-0.2.6/pywebify/
--rw-rw-rw-   0        0        0     3412 2018-10-29 01:59:29.000000 pywebify-0.2.6/pywebify/config.ini
-drwxrwxrwx   0        0        0        0 2020-07-09 20:16:40.000000 pywebify-0.2.6/pywebify/img/
--rw-rw-rw-   0        0        0     1241 2018-10-08 23:52:38.000000 pywebify-0.2.6/pywebify/img/collapsed.png
--rw-rw-rw-   0        0        0      207 2018-10-08 23:52:38.000000 pywebify-0.2.6/pywebify/img/expanded.png
--rw-rw-rw-   0        0        0      633 2018-10-08 23:52:38.000000 pywebify-0.2.6/pywebify/img/favicon.png
-drwxrwxrwx   0        0        0        0 2020-07-09 20:16:40.000000 pywebify-0.2.6/pywebify/js/
--rw-rw-rw-   0        0        0     1700 2018-10-08 23:52:38.000000 pywebify-0.2.6/pywebify/js/collapse.js
--rw-rw-rw-   0        0        0     5159 2018-10-09 00:53:16.000000 pywebify-0.2.6/pywebify/js/div_switch.js
--rw-rw-rw-   0        0        0     1337 2018-10-08 23:52:39.000000 pywebify-0.2.6/pywebify/js/div_toggle.js
--rw-rw-rw-   0        0        0     1614 2018-10-08 23:52:39.000000 pywebify-0.2.6/pywebify/js/filter.js
--rw-rw-rw-   0        0        0     1494 2018-10-08 23:52:39.000000 pywebify-0.2.6/pywebify/js/pixelate.js
--rw-rw-rw-   0        0        0    16666 2020-07-09 19:33:48.000000 pywebify-0.2.6/pywebify/pywebify.py
--rw-rw-rw-   0        0        0       10 2018-10-08 23:52:39.000000 pywebify-0.2.6/pywebify/setup.txt
--rw-rw-rw-   0        0        0     2829 2018-10-08 23:52:39.000000 pywebify-0.2.6/pywebify/template.py
-drwxrwxrwx   0        0        0        0 2020-07-09 20:16:39.000000 pywebify-0.2.6/pywebify/templates/
-drwxrwxrwx   0        0        0        0 2020-07-09 20:16:40.000000 pywebify-0.2.6/pywebify/templates/css/
--rw-rw-rw-   0        0        0     1078 2018-10-08 23:52:39.000000 pywebify-0.2.6/pywebify/templates/css/collapse.css
--rw-rw-rw-   0        0        0      326 2018-10-08 23:52:39.000000 pywebify-0.2.6/pywebify/templates/css/filter.css
--rw-rw-rw-   0        0        0     1183 2018-10-08 23:52:39.000000 pywebify-0.2.6/pywebify/templates/css/pixelate.css
--rw-rw-rw-   0        0        0     3514 2018-10-08 23:52:39.000000 pywebify-0.2.6/pywebify/templates/css/rst.css
--rw-rw-rw-   0        0        0     6154 2018-10-08 23:52:39.000000 pywebify-0.2.6/pywebify/templates/css/webify.css
-drwxrwxrwx   0        0        0        0 2020-07-09 20:16:40.000000 pywebify-0.2.6/pywebify/templates/html/
--rw-rw-rw-   0        0        0     1384 2018-10-08 23:52:39.000000 pywebify-0.2.6/pywebify/templates/html/navbar.html
--rw-rw-rw-   0        0        0     2071 2018-10-31 01:06:34.000000 pywebify-0.2.6/pywebify/templates/html/webify.html
-drwxrwxrwx   0        0        0        0 2020-07-09 20:16:40.000000 pywebify-0.2.6/pywebify/templates/jinja/
--rw-rw-rw-   0        0        0     1743 2018-10-08 23:52:39.000000 pywebify-0.2.6/pywebify/templates/jinja/tabs.html
--rw-rw-rw-   0        0        0     1794 2018-10-08 23:52:39.000000 pywebify-0.2.6/pywebify/templates/jinja/webpage.html
--rw-rw-rw-   0        0        0        5 2020-07-09 20:11:05.000000 pywebify-0.2.6/pywebify/version.txt
--rw-rw-rw-   0        0        0    11616 2018-10-08 23:52:39.000000 pywebify-0.2.6/pywebify/webpage.py
--rw-rw-rw-   0        0        0      432 2020-07-09 19:30:40.000000 pywebify-0.2.6/pywebify/__init__.py
-drwxrwxrwx   0        0        0        0 2020-07-09 20:16:40.000000 pywebify-0.2.6/pywebify.egg-info/
--rw-rw-rw-   0        0        0        1 2020-07-09 20:16:39.000000 pywebify-0.2.6/pywebify.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      480 2020-07-09 20:16:39.000000 pywebify-0.2.6/pywebify.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0       36 2020-07-09 20:16:39.000000 pywebify-0.2.6/pywebify.egg-info/requires.txt
--rw-rw-rw-   0        0        0      859 2020-07-09 20:16:39.000000 pywebify-0.2.6/pywebify.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        9 2020-07-09 20:16:39.000000 pywebify-0.2.6/pywebify.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      316 2018-10-08 23:52:38.000000 pywebify-0.2.6/README.rst
--rw-rw-rw-   0        0        0      122 2020-07-09 20:16:41.000000 pywebify-0.2.6/setup.cfg
--rw-rw-rw-   0        0        0     4115 2020-07-09 20:13:26.000000 pywebify-0.2.6/setup.py
+drwxr-xr-x   0 steve      (502) staff       (20)        0 2023-04-09 16:29:28.253568 pywebify-0.3.0a0/
+-rw-r--r--   0 steve      (502) staff       (20)       18 2023-04-09 16:28:29.000000 pywebify-0.3.0a0/MANIFEST.in
+-rw-r--r--   0 steve      (502) staff       (20)      842 2023-04-09 16:29:28.253655 pywebify-0.3.0a0/PKG-INFO
+-rw-r--r--   0 steve      (502) staff       (20)      307 2023-04-09 16:28:29.000000 pywebify-0.3.0a0/README.rst
+-rw-r--r--   0 steve      (502) staff       (20)      187 2023-04-09 16:28:29.000000 pywebify-0.3.0a0/pyproject.toml
+-rw-r--r--   0 steve      (502) staff       (20)     1378 2023-04-09 16:29:28.254160 pywebify-0.3.0a0/setup.cfg
+-rw-r--r--   0 steve      (502) staff       (20)       68 2023-04-09 16:28:29.000000 pywebify-0.3.0a0/setup.py
+drwxr-xr-x   0 steve      (502) staff       (20)        0 2023-04-09 16:29:28.229950 pywebify-0.3.0a0/src/
+drwxr-xr-x   0 steve      (502) staff       (20)        0 2023-04-09 16:29:28.240616 pywebify-0.3.0a0/src/pywebify/
+-rw-r--r--   0 steve      (502) staff       (20)      453 2023-04-09 16:28:29.000000 pywebify-0.3.0a0/src/pywebify/__init__.py
+-rw-r--r--   0 steve      (502) staff       (20)     4653 2023-04-09 16:28:29.000000 pywebify-0.3.0a0/src/pywebify/config.ini
+-rw-r--r--   0 steve      (502) staff       (20)     7395 2023-04-09 16:28:29.000000 pywebify-0.3.0a0/src/pywebify/config.py
+-rw-r--r--   0 steve      (502) staff       (20)    17327 2023-04-09 16:28:29.000000 pywebify-0.3.0a0/src/pywebify/html.py
+drwxr-xr-x   0 steve      (502) staff       (20)        0 2023-04-09 16:29:28.244586 pywebify-0.3.0a0/src/pywebify/img/
+-rw-r--r--   0 steve      (502) staff       (20)     1241 2023-04-09 16:28:29.000000 pywebify-0.3.0a0/src/pywebify/img/collapsed.png
+-rw-r--r--   0 steve      (502) staff       (20)      207 2023-04-09 16:28:29.000000 pywebify-0.3.0a0/src/pywebify/img/expanded.png
+-rw-r--r--   0 steve      (502) staff       (20)      633 2023-04-09 16:28:29.000000 pywebify-0.3.0a0/src/pywebify/img/favicon.png
+drwxr-xr-x   0 steve      (502) staff       (20)        0 2023-04-09 16:29:28.249227 pywebify-0.3.0a0/src/pywebify/js/
+-rw-r--r--   0 steve      (502) staff       (20)     1656 2023-04-09 16:28:29.000000 pywebify-0.3.0a0/src/pywebify/js/collapse.js
+-rw-r--r--   0 steve      (502) staff       (20)     5050 2023-04-09 16:28:29.000000 pywebify-0.3.0a0/src/pywebify/js/div_switch.js
+-rw-r--r--   0 steve      (502) staff       (20)     1188 2023-04-09 16:28:29.000000 pywebify-0.3.0a0/src/pywebify/js/div_toggle.js
+-rw-r--r--   0 steve      (502) staff       (20)     1580 2023-04-09 16:28:29.000000 pywebify-0.3.0a0/src/pywebify/js/filter.js
+-rw-r--r--   0 steve      (502) staff       (20)    89985 2023-04-09 16:28:29.000000 pywebify-0.3.0a0/src/pywebify/js/jquery.min.js
+-rw-r--r--   0 steve      (502) staff       (20)     1450 2023-04-09 16:28:29.000000 pywebify-0.3.0a0/src/pywebify/js/pixelate.js
+-rw-r--r--   0 steve      (502) staff       (20)    19773 2023-04-09 16:28:29.000000 pywebify-0.3.0a0/src/pywebify/pywebify.py
+-rw-r--r--   0 steve      (502) staff       (20)     3107 2023-04-09 16:28:29.000000 pywebify-0.3.0a0/src/pywebify/template.py
+drwxr-xr-x   0 steve      (502) staff       (20)        0 2023-04-09 16:29:28.231181 pywebify-0.3.0a0/src/pywebify/templates/
+drwxr-xr-x   0 steve      (502) staff       (20)        0 2023-04-09 16:29:28.251425 pywebify-0.3.0a0/src/pywebify/templates/css/
+-rw-r--r--   0 steve      (502) staff       (20)     1065 2023-04-09 16:28:29.000000 pywebify-0.3.0a0/src/pywebify/templates/css/collapse.css
+-rw-r--r--   0 steve      (502) staff       (20)      316 2023-04-09 16:28:29.000000 pywebify-0.3.0a0/src/pywebify/templates/css/filter.css
+-rw-r--r--   0 steve      (502) staff       (20)     1134 2023-04-09 16:28:29.000000 pywebify-0.3.0a0/src/pywebify/templates/css/pixelate.css
+-rw-r--r--   0 steve      (502) staff       (20)     3835 2023-04-09 16:28:29.000000 pywebify-0.3.0a0/src/pywebify/templates/css/rst.css
+-rw-r--r--   0 steve      (502) staff       (20)     7139 2023-04-09 16:28:29.000000 pywebify-0.3.0a0/src/pywebify/templates/css/webify.css
+drwxr-xr-x   0 steve      (502) staff       (20)        0 2023-04-09 16:29:28.252291 pywebify-0.3.0a0/src/pywebify/templates/html/
+-rw-r--r--   0 steve      (502) staff       (20)     1483 2023-04-09 16:28:29.000000 pywebify-0.3.0a0/src/pywebify/templates/html/navbar.html
+-rw-r--r--   0 steve      (502) staff       (20)     1999 2023-04-09 16:28:29.000000 pywebify-0.3.0a0/src/pywebify/templates/html/webify.html
+drwxr-xr-x   0 steve      (502) staff       (20)        0 2023-04-09 16:29:28.253259 pywebify-0.3.0a0/src/pywebify/templates/jinja/
+-rw-r--r--   0 steve      (502) staff       (20)     1698 2023-04-09 16:28:29.000000 pywebify-0.3.0a0/src/pywebify/templates/jinja/tabs.html
+-rw-r--r--   0 steve      (502) staff       (20)     1747 2023-04-09 16:28:29.000000 pywebify-0.3.0a0/src/pywebify/templates/jinja/webpage.html
+drwxr-xr-x   0 steve      (502) staff       (20)        0 2023-04-09 16:29:28.242639 pywebify-0.3.0a0/src/pywebify.egg-info/
+-rw-r--r--   0 steve      (502) staff       (20)      842 2023-04-09 16:29:28.000000 pywebify-0.3.0a0/src/pywebify.egg-info/PKG-INFO
+-rw-r--r--   0 steve      (502) staff       (20)      992 2023-04-09 16:29:28.000000 pywebify-0.3.0a0/src/pywebify.egg-info/SOURCES.txt
+-rw-r--r--   0 steve      (502) staff       (20)        1 2023-04-09 16:29:28.000000 pywebify-0.3.0a0/src/pywebify.egg-info/dependency_links.txt
+-rw-r--r--   0 steve      (502) staff       (20)      369 2023-04-09 16:29:28.000000 pywebify-0.3.0a0/src/pywebify.egg-info/requires.txt
+-rw-r--r--   0 steve      (502) staff       (20)        9 2023-04-09 16:29:28.000000 pywebify-0.3.0a0/src/pywebify.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `pywebify-0.2.6/pywebify/img/collapsed.png` & `pywebify-0.3.0a0/src/pywebify/img/collapsed.png`

 * *Files identical despite different names*

### Comparing `pywebify-0.2.6/pywebify/img/favicon.png` & `pywebify-0.3.0a0/src/pywebify/img/favicon.png`

 * *Files identical despite different names*

### Comparing `pywebify-0.2.6/pywebify/js/collapse.js` & `pywebify-0.3.0a0/src/pywebify/js/collapse.js`

 * *Files 15% similar despite different names*

#### js-beautify {}

```diff
@@ -1,45 +1,45 @@
-/*******************************************************************************/
-/* Makes the file list ul dynamically expandable/collapsible                   */
-/*   Modified from http://jasalguero.com/ledld/development/web/expandable-list */
-/*   Designed for the PyWebify project                                         */
-/*   https://github.com/endangeredoxen/pywebify                                */
-/*******************************************************************************/
-
-
-function prepareList() {
-    $('#collapse').find('li:has(ul)')
-        .click(function(event) {
-            if (this == event.target) {
-                $(this).toggleClass('expanded');
-                $(this).children('ul').toggle();
-            }
-            return false;
-        })
-        .addClass('collapsed')
-        .children('ul').hide();
-
-
-    //Create the button funtionality
-    $('#expandList')
-        .unbind('click')
-        .click(function() {
-            $('.collapsed').addClass('expanded');
-            $('.collapsed').children().show();
-        })
-    $('#collapseList')
-        .unbind('click')
-        .click(function() {
-            location.reload();
-        })
-
-};
-
-
-/**************************************************************/
-/* Functions to execute on loading the document               */
-/**************************************************************/
-$(document).ready(function() {
-    //    document.getElementById('sidebar').innerHTML = '<div class="listControl"><a id="expandList">Expand All</a><a id="collapseList">Collapse All</a></div>';
-    $('#sidebar').prepend('<div class="listControl"><a id="expandList">Expand All</a><a id="collapseList">Collapse All</a></div>');
-    prepareList()
+/*******************************************************************************/
+/* Makes the file list ul dynamically expandable/collapsible                   */
+/*   Modified from http://jasalguero.com/ledld/development/web/expandable-list */
+/*   Designed for the PyWebify project                                         */
+/*   https://github.com/endangeredoxen/pywebify                                */
+/*******************************************************************************/
+
+
+function prepareList() {
+    $('#collapse').find('li:has(ul)')
+        .click(function(event) {
+            if (this == event.target) {
+                $(this).toggleClass('expanded');
+                $(this).children('ul').toggle();
+            }
+            return false;
+        })
+        .addClass('collapsed')
+        .children('ul').hide();
+
+
+    //Create the button funtionality
+    $('#expandList')
+        .unbind('click')
+        .click(function() {
+            $('.collapsed').addClass('expanded');
+            $('.collapsed').children().show();
+        })
+    $('#collapseList')
+        .unbind('click')
+        .click(function() {
+            location.reload();
+        })
+
+};
+
+
+/**************************************************************/
+/* Functions to execute on loading the document               */
+/**************************************************************/
+$(document).ready(function() {
+    //    document.getElementById('sidebar').innerHTML = '<div class="listControl"><a id="expandList">Expand All</a><a id="collapseList">Collapse All</a></div>';
+    $('#sidebar').prepend('<div class="listControl"><a id="expandList">Expand All</a><a id="collapseList">Collapse All</a></div>');
+    prepareList()
 });
```

### Comparing `pywebify-0.2.6/pywebify/js/div_switch.js` & `pywebify-0.3.0a0/src/pywebify/js/div_switch.js`

 * *Files 26% similar despite different names*

#### js-beautify {}

```diff
@@ -1,127 +1,127 @@
-/*******************************************************************************/
-/* Div content switcher                                                        */
-/*   Designed for the PyWebify project                                         */
-/*   https://github.com/endangeredoxen/pywebify                                */
-/*******************************************************************************/
-
-function div_switch(name) {
-    // Check the file extension
-    var re = /(?:\.([^.]+))?$/;
-    var ext = re.exec(name)[1];
-    var dv = document.getElementById('viewer');
-    if (ext == "html") {
-        // Check for an existing image and remove if found
-        var image = document.getElementById('img0');
-        if (typeof(image) != 'undefined' && image != null) {
-            image.parentNode.removeChild(image);
-        }
-
-        var isHTML0 = document.getElementById('html0');
-        if (typeof(isHTML0) != 'undefined' && isHTML0 != null) {
-            // HTML found, so replace with new
-            var oldTHML = document.getElementById("html0");
-            var newHTML = document.createElement("object");
-            newHTML.data = name;
-            newHTML.id = "html0";
-            newHTML.width = '100%';
-            newHTML.height = '100%';
-            oldTHML.parentNode.replaceChild(newHTML, oldTHML);
-        } else {
-            // HTML not found, so create and add
-            var summary = document.getElementById('summary');
-            var newHTML = document.createElement("object");
-            newHTML.data = name;
-            newHTML.id = "html0";
-            newHTML.width = '100%';
-            newHTML.height = '100%';
-            dv.insertBefore(newHTML, summary);
-
-        }
-
-    } else {
-        // Check for an existing html remove if found
-        var html = document.getElementById('html0');
-        if (typeof(html) != 'undefined' && html != null) {
-            html.parentNode.removeChild(html);
-        }
-
-        // Check for an existing image
-        var image = document.getElementById('img0');
-        if (typeof(image) != 'undefined' && image != null) {
-            // Image found, so replace with new
-            image.removeAttribute('width');
-            image.style.maxWidth = '100%';
-            image.src = name + "?" + new Date().getTime();
-        } else {
-            // Image not found, so create and add
-            var image = document.createElement("img");
-            var summary = document.getElementById('summary');
-            image.src = name + "?" + new Date().getTime();
-            image.id = "img0";
-            image.removeAttribute('width');
-            image.style.maxWidth = '100%';
-            dv.insertBefore(image, summary);
-
-        }
-
-        // Add any accompanying html
-        var newHTML = document.createElement("object");
-        newHTML.data = name.replace('.' + ext, '.html');
-        newHTML.id = "html0";
-        newHTML.width = '100%';
-        newHTML.height = '100%';
-        dv.insertBefore(newHTML, summary);
-
-        var width0 = 0;
-        var zoom = 'in';
-        var startWidth = image.width;
-
-        image.onclick = function(event) {
-            var action = false;
-            if (event.shiftKey) {
-                var resize = 0.75; // resize amount in percentage
-                if (zoom == 'in') {
-                    zoom = 'out';
-                } else
-                    zoom = 'in';
-                action = true;
-            } else if (event.ctrlKey) {
-                var resize = 1.25; // resize amount in percentage
-                if (zoom == 'out') {
-                    zoom = 'in';
-                } else
-                    zoom = 'in';
-                action = true;
-            }
-            if (event.altKey) {
-                viewer.scrollLeft = 0;
-                viewer.scrollTop = 0;
-                this.removeAttribute('width');
-                this.style.maxWidth = '800%';
-            } else if (action) {
-
-                //Set the new width and height
-                var origW = this.clientWidth; // original image width
-                this.style.maxWidth = 'none';
-                this.setAttribute('width', origW * resize);
-
-                // Set the scroll bars
-                var bbox = this.getBoundingClientRect();
-                var mouseX = event.clientX - bbox.left;
-                var mouseY = event.clientY - bbox.top;
-                var imgWidth = bbox.right - bbox.left;
-                var imgHeight = bbox.bottom - bbox.top;
-                var xOffset = mouseX * resize - imgWidth / 2;
-                var yOffset = mouseY * resize - imgHeight / 2;
-                var scrollWidthMax = this.scrollWidth - dv.offsetWidth;
-                var scrollHeightMax = this.scrollHeight - dv.offsetHeight;
-                var ratioWidth = scrollWidthMax / imgWidth;
-
-                viewer.scrollLeft = scrollWidthMax / 2 + xOffset;
-                viewer.scrollTop = scrollHeightMax / 2 + yOffset;
-            }
-        }
-    }
-    viewer.scrollTop = 0;
-    viewer.scrollLeft = 0;
+/*******************************************************************************/
+/* Div content switcher                                                        */
+/*   Designed for the PyWebify project                                         */
+/*   https://github.com/endangeredoxen/pywebify                                */
+/*******************************************************************************/
+
+function div_switch(name) {
+    // Check the file extension
+    var re = /(?:\.([^.]+))?$/;
+    var ext = re.exec(name)[1];
+    var dv = document.getElementById('viewer');
+    if (ext == "html") {
+        // Check for an existing image and remove if found
+        var image = document.getElementById('img0');
+        if (typeof(image) != 'undefined' && image != null) {
+            image.parentNode.removeChild(image);
+        }
+
+        var isHTML0 = document.getElementById('html0');
+        if (typeof(isHTML0) != 'undefined' && isHTML0 != null) {
+            // HTML found, so replace with new
+            var oldTHML = document.getElementById("html0");
+            var newHTML = document.createElement("object");
+            newHTML.data = name;
+            newHTML.id = "html0";
+            newHTML.width = '100%';
+            newHTML.height = '100%';
+            oldTHML.parentNode.replaceChild(newHTML, oldTHML);
+        } else {
+            // HTML not found, so create and add
+            var summary = document.getElementById('summary');
+            var newHTML = document.createElement("object");
+            newHTML.data = name;
+            newHTML.id = "html0";
+            newHTML.width = '100%';
+            newHTML.height = '100%';
+            dv.insertBefore(newHTML, summary);
+
+        }
+
+    } else {
+        // Check for an existing html remove if found
+        var html = document.getElementById('html0');
+        if (typeof(html) != 'undefined' && html != null) {
+            html.parentNode.removeChild(html);
+        }
+
+        // Check for an existing image
+        var image = document.getElementById('img0');
+        if (typeof(image) != 'undefined' && image != null) {
+            // Image found, so replace with new
+            image.removeAttribute('width');
+            image.style.maxWidth = '100%';
+            image.src = name + "?" + new Date().getTime();
+        } else {
+            // Image not found, so create and add
+            var image = document.createElement("img");
+            var summary = document.getElementById('summary');
+            image.src = name + "?" + new Date().getTime();
+            image.id = "img0";
+            image.removeAttribute('width');
+            image.style.maxWidth = '100%';
+            dv.insertBefore(image, summary);
+
+        }
+
+        // Add any accompanying html
+        var newHTML = document.createElement("object");
+        newHTML.data = name.replace('.' + ext, '.html');
+        newHTML.id = "html0";
+        newHTML.width = '100%';
+        newHTML.height = '100%';
+        dv.insertBefore(newHTML, summary);
+
+        var width0 = 0;
+        var zoom = 'in';
+        var startWidth = image.width;
+
+        image.onclick = function(event) {
+            var action = false;
+            if (event.shiftKey) {
+                var resize = 0.75; // resize amount in percentage
+                if (zoom == 'in') {
+                    zoom = 'out';
+                } else
+                    zoom = 'in';
+                action = true;
+            } else if (event.ctrlKey || event.metaKey) {
+                var resize = 1.25; // resize amount in percentage
+                if (zoom == 'out') {
+                    zoom = 'in';
+                } else
+                    zoom = 'in';
+                action = true;
+            }
+            if (event.altKey) {
+                viewer.scrollLeft = 0;
+                viewer.scrollTop = 0;
+                this.removeAttribute('width');
+                this.style.maxWidth = '800%';
+            } else if (action) {
+
+                //Set the new width and height
+                var origW = this.clientWidth; // original image width
+                this.style.maxWidth = 'none';
+                this.setAttribute('width', origW * resize);
+
+                // Set the scroll bars
+                var bbox = this.getBoundingClientRect();
+                var mouseX = event.clientX - bbox.left;
+                var mouseY = event.clientY - bbox.top;
+                var imgWidth = bbox.right - bbox.left;
+                var imgHeight = bbox.bottom - bbox.top;
+                var xOffset = mouseX * resize - imgWidth / 2;
+                var yOffset = mouseY * resize - imgHeight / 2;
+                var scrollWidthMax = this.scrollWidth - dv.offsetWidth;
+                var scrollHeightMax = this.scrollHeight - dv.offsetHeight;
+                var ratioWidth = scrollWidthMax / imgWidth;
+
+                viewer.scrollLeft = scrollWidthMax / 2 + xOffset;
+                viewer.scrollTop = scrollHeightMax / 2 + yOffset;
+            }
+        }
+    }
+    viewer.scrollTop = 0;
+    viewer.scrollLeft = 0;
 }
```

### Comparing `pywebify-0.2.6/pywebify/js/div_toggle.js` & `pywebify-0.3.0a0/src/pywebify/js/div_toggle.js`

 * *Files 26% similar despite different names*

#### js-beautify {}

```diff
@@ -1,49 +1,45 @@
-/*******************************************************************************/
-/* Div size toggler                                                            */
-/*   Designed for the PyWebify project                                         */
-/*   https://github.com/endangeredoxen/pywebify                                */
-/*******************************************************************************/
-
-function div_toggle() {
-    var origWidth = $('#sidebar').width();
-    $('#toggle').html('<<');
-    $('#toggle').toggle(function() {
-        $('#sidebar').css({
-            'overflow': 'hidden'
-        });
-        $('#sidebar li').css({
-            'visibility': 'hidden'
-        });
-        $('#sidebar').animate({
-            width: 0
-        });
-        $('#viewer').animate({
-            left: 0
-        });
-        $('#toggle').html('>>');
-    }, function() {
-        $('#sidebar').css({
-            'overflow': 'auto'
-        });
-        $('#sidebar li').css({
-            'visibility': 'visible'
-        });
-        $('#sidebar').animate({
-            width: origWidth
-        });
-        $('#toggle').html('<<');
-    });
-
-    // position the toggle at the bottom and account for a reduced viewer div height
-    //    var h1 = $('#viewer').height();
-    //    $('#viewer').height('100%');
-    //    var h2 = $('#viewer').height();
-    //    var h3 = h2-h1;
-    //
-    //    $('#toggle').css({'bottom':h3+'px'});
-    //    $('#viewer').height(h1);
-};
-
-$(document).ready(function() {
-    div_toggle()
+/*******************************************************************************/
+/* Div size toggler                                                            */
+/*   Designed for the PyWebify project                                         */
+/*   https://github.com/endangeredoxen/pywebify                                */
+/*******************************************************************************/
+
+function div_toggle() {
+    var origWidth = $('#sidebar').width();
+    var status = 0;
+    $('#toggle').html('<<');
+    $('#toggle').on('click', function() {
+        if (status == 0) {
+            $('#sidebar').css({
+                'overflow': 'hidden'
+            });
+            $('#sidebar li').css({
+                'visibility': 'hidden'
+            });
+            $('#sidebar').animate({
+                width: 0
+            });
+            $('#viewer').animate({
+                left: 0
+            });
+            $('#toggle').html('>>');
+            status = 1;
+        } else {
+            $('#sidebar').css({
+                'overflow': 'auto'
+            });
+            $('#sidebar li').css({
+                'visibility': 'visible'
+            });
+            $('#sidebar').animate({
+                width: origWidth
+            });
+            $('#toggle').html('<<');
+            status = 0;
+        }
+    });
+};
+
+$(document).ready(function() {
+    div_toggle()
 });
```

### Comparing `pywebify-0.2.6/pywebify/js/filter.js` & `pywebify-0.3.0a0/src/pywebify/js/filter.js`

 * *Files 18% similar despite different names*

#### js-beautify {}

```diff
@@ -1,44 +1,44 @@
-/*******************************************************************************/
-/* Filters the report file list                                                */
-/*   Modified from http://jsfiddle.net/GoranMottram/4CJMe/4/                   */
-/*   Designed for the PyWebify project                                         */
-/*   https://github.com/endangeredoxen/pywebify                                */
-/*******************************************************************************/
-(function($) {
-
-    function searchList(elm, mylist) { // elm is any element, mylist is an unordered list
-        // create and add the filter form to the elm
-        var form = $("<form>").attr({
-                "class": "filterform",
-                "action": "#"
-            }),
-            input = $("<input>").attr({
-                "class": "filterinput",
-                "type": "text",
-                "value": "Search..."
-            });
-        $(form).append(input).appendTo(elm);
-        $(input).css({
-            marginTop: $(elm).height() / 2 - $(input).outerHeight() / 2
-        }); //center the input field vertically
-
-        $(input).keyup(function() {
-            var searchTerms = $(this).val();
-            $('#expandList').click();
-            console.log("Input change")
-            $(mylist + ' li').each(function() {
-                var hasMatch = searchTerms.length == 0 || $(this).text().toLowerCase().indexOf(searchTerms.toLowerCase()) > 0;
-
-                $(this).toggle(hasMatch);
-            });
-        });
-        $(input).focus(function() {
-            $(input).val("");
-        });
-    }
-
-    //ondomready
-    $(function() {
-        searchList($("#navbar"), "#collapse");
-    });
+/*******************************************************************************/
+/* Filters the report file list                                                */
+/*   Modified from http://jsfiddle.net/GoranMottram/4CJMe/4/                   */
+/*   Designed for the PyWebify project                                         */
+/*   https://github.com/endangeredoxen/pywebify                                */
+/*******************************************************************************/
+(function($) {
+
+    function searchList(elm, mylist) { // elm is any element, mylist is an unordered list
+        // create and add the filter form to the elm
+        var form = $("<form>").attr({
+                "class": "filterform",
+                "action": "#"
+            }),
+            input = $("<input>").attr({
+                "class": "filterinput",
+                "type": "text",
+                "value": "Search..."
+            });
+        $(form).append(input).appendTo(elm);
+        $(input).css({
+            marginTop: $(elm).height() / 2 - $(input).outerHeight() / 2
+        }); //center the input field vertically
+
+        $(input).keyup(function() {
+            var searchTerms = $(this).val();
+            $('#expandList').click();
+            console.log("Input change")
+            $(mylist + ' li').each(function() {
+                var hasMatch = searchTerms.length == 0 || $(this).text().toLowerCase().indexOf(searchTerms.toLowerCase()) > 0;
+
+                $(this).toggle(hasMatch);
+            });
+        });
+        $(input).focus(function() {
+            $(input).val("");
+        });
+    }
+
+    //ondomready
+    $(function() {
+        searchList($("#navbar"), "#collapse");
+    });
 }(jQuery));
```

### Comparing `pywebify-0.2.6/pywebify/template.py` & `pywebify-0.3.0a0/src/pywebify/template.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,95 +1,104 @@
-############################################################################
-# template.py
-#   Template maker utility: populates a template with special keyword values
-#   to generate an HTML page or section of a page
-############################################################################
-__author__    = 'Steve Nicholes'
-__copyright__ = 'Copyright (C) 2015 Steve Nicholes'
-__license__   = 'GPLv3'
-__version__   = '0.2'
-__url__       = 'https://github.com/endangeredoxen/pywebify'
-
-import os
-import string
-import pdb
-st = pdb.set_trace
-
-
-class Template():
-    def __init__(self, template, subs):
-        """ Template maker
-
-        Replaces strings within a specified template in order to make a
-        functional HTML page or section of a page
-
-        Args:
-            template (str):  path to template file
-            subs (dict|list):  replacement strings dict or list of dicts
-
-        """
-
-        # Set the path
-        self.templatePath = template
-
-        # Init the raw html output varialbe
-        self.raw = ''
-
-        # Process multiple replacement dictionaries
-        if len(subs) > 1:
-            self.subs = self.merge_dicts(subs)
-        else:
-            self.subs = subs[0]
-
-    def merge_dicts(self, subs):
-        """ Combine multiple dictionaries in to one
-
-        Args:
-            subs (list): list of dicts
-
-        Returns:
-            merged dict
-        """
-
-        merged = subs[0]
-        for i in range(1, len(subs)):
-            merged.update(subs[i])
-        return merged
-
-    def substitute(self, caps=None):
-        """ String substitution
-
-        Args:
-            caps (bool):  force uppercase on all dict keys
-
-        Returns:
-            none:  self.raw updated
-        """
-
-        if caps:
-            self.subs = dict((k.upper(), v) for k,v in self.subs.items())
-        self.raw = self.raw.safe_substitute(self.subs)
-
-    def write(self, dest=None, caps=True, bonus=''):
-        """ Write the updated template to file
-
-        Args:
-            dest (str|None):  output filepath for template; if None,
-                              self.raw returned
-            caps (bool): force uppercase on all dict keys
-            bonus (str): additional text to add to self.raw
-
-        Returns:
-            if dest==None, return self.raw
-        """
-
-        self.raw = string.Template(open(self.templatePath).read())
-        self.substitute(caps)
-        self.raw = self.raw + '\n' + bonus
-        if dest:
-            dest_path = os.path.sep.join(dest.split(os.path.sep)[0:-1])
-            if not os.path.exists(dest_path):
-                os.makedirs(dest_path)
-            with open(dest, 'w') as temp:
-                temp.write(self.raw)
-        else:
-            return self.raw
+############################################################################
+# template.py
+#   Template maker utility: populates a template with special keyword values
+#   to generate an HTML page or section of a page
+############################################################################
+__author__ = 'Steve Nicholes'
+__copyright__ = 'Copyright (C) 2015 Steve Nicholes'
+__license__ = 'GPLv3'
+__version__ = '0.2'
+__url__ = 'https://github.com/endangeredoxen/pywebify'
+
+import os
+import string
+import pdb
+from pathlib import Path
+from typing import Union
+db = pdb.set_trace
+
+
+class Template():
+    def __init__(self, template_paths: Union[str, Path, list], subs: Union[dict, list]):
+        """ Template maker
+
+        Replaces strings within a specified template in order to make a
+        functional HTML page or section of a page
+
+        Args:
+            template_paths (str):  path to template file
+            subs (dict|list):  replacement strings dict or list of dicts
+
+        """
+
+        # Set the path
+        if not isinstance(template_paths, list):
+            template_paths = [template_paths]
+        self.template_paths = template_paths
+
+        # Init the raw html output varialbe
+        self.raw = ''
+
+        # Process multiple replacement dictionaries
+        if isinstance(subs, dict):
+            self.subs = subs
+        elif len(subs) > 1:
+            self.subs = self.merge_dicts(subs)
+        else:
+            self.subs = subs[0]
+
+    def merge_dicts(self, subs):
+        """ Combine multiple dictionaries in to one
+
+        Args:
+            subs (list): list of dicts
+
+        Returns:
+            merged dict
+        """
+
+        merged = subs[0]
+        for i in range(1, len(subs)):
+            merged.update(subs[i])
+        return merged
+
+    def substitute(self, caps=None):
+        """ String substitution
+
+        Args:
+            caps (bool):  force uppercase on all dict keys
+
+        Returns:
+            none:  self.raw updated
+        """
+
+        if caps:
+            self.subs = dict((k.upper(), v) for k, v in self.subs.items())
+        self.raw = self.raw.safe_substitute(self.subs)
+
+    def write(self, dest: Union[Path, str, None] = None, caps: bool = True, bonus: str = ''):
+        """Write the updated template to file.
+
+        Args:
+            dest:  output filepath for template; if None, self.raw returned
+            caps: force uppercase on all dict keys
+            bonus: additional text to add to self.raw
+
+        Returns:
+            if dest==None, return self.raw
+        """
+        raw = []
+        for tp in self.template_paths:
+            with open(tp, 'r') as input:
+                raw += [input.read()]
+        self.raw = string.Template('\n'.join(raw))
+        self.substitute(caps)
+        self.raw = self.raw + '\n' + bonus
+        if dest:
+            if isinstance(dest, str):
+                dest = Path(dest)
+            if not os.path.exists(dest.parent):
+                os.makedirs(dest.parent)
+            with open(dest, 'w') as temp:
+                temp.write(self.raw)
+        else:
+            return self.raw
```

### Comparing `pywebify-0.2.6/pywebify/templates/css/pixelate.css` & `pywebify-0.3.0a0/src/pywebify/templates/css/pixelate.css`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,49 +1,49 @@
-
-#pixelCheckboxDiv{
-    margin-bottom : 0px;
-    margin-left   : -5px;
-}
-#pixelCheckboxText{
-    color         : #aaaaaa;
-    font-style    : italic;
-    margin-left   : 10px;
-    margin-top    : 5px;
-    margin-bottom : 5px;
-    display       : inline-block;
-    position      : relative;
-    top           : -11px;
-    left          : 6px;
-}
-#pixelCheckbox {
-    display : none;
-}
-#pixelCheckboxSpan {
-    display        : inline-block;
-    border         : 1px solid #aaaaaa;
-    border-radius  : 2px;
-    width          : 15px;
-    height         : 15px;
-    vertical-align : middle;
-    text-align     : center;
-    position       : relative;
-    top            : -12px;
-    left           : 5px;
-}
-#pixelCheckbox:checked + #pixelCheckboxSpan{
-    background : #555555;
-}
-#pixelCheckbox:checked + #pixelCheckboxSpan:after{
-    content   : '\2714';
-    font-size : 10px;
-    position  : relative;
-    top       : -5px;
-    left      : 0px;
-    color     : #FFCC00;
-}
-#pixelCheckboxSpan:before {
-    content        : '';
-    vertical-align : middle;
-}
-#pixelCheckbox :checked + #pixelCheckboxSpan:before {
-    content : '\2714';
-}
+
+#pixelCheckboxDiv{
+    margin-bottom : 0px;
+    margin-left   : -5px;
+}
+#pixelCheckboxText{
+    color         : #aaaaaa;
+    font-style    : italic;
+    margin-left   : 10px;
+    margin-top    : 5px;
+    margin-bottom : 5px;
+    display       : inline-block;
+    position      : relative;
+    top           : -11px;
+    left          : 6px;
+}
+#pixelCheckbox {
+    display : none;
+}
+#pixelCheckboxSpan {
+    display        : inline-block;
+    border         : 1px solid #aaaaaa;
+    border-radius  : 2px;
+    width          : 15px;
+    height         : 15px;
+    vertical-align : middle;
+    text-align     : center;
+    position       : relative;
+    top            : -12px;
+    left           : 5px;
+}
+#pixelCheckbox:checked + #pixelCheckboxSpan{
+    background : #555555;
+}
+#pixelCheckbox:checked + #pixelCheckboxSpan:after{
+    content   : '\2714';
+    font-size : 10px;
+    position  : relative;
+    top       : -5px;
+    left      : 0px;
+    color     : #FFCC00;
+}
+#pixelCheckboxSpan:before {
+    content        : '';
+    vertical-align : middle;
+}
+#pixelCheckbox :checked + #pixelCheckboxSpan:before {
+    content : '\2714';
+}
```

### Comparing `pywebify-0.2.6/pywebify/templates/html/navbar.html` & `pywebify-0.3.0a0/src/pywebify/templates/html/navbar.html`

 * *Files 18% similar despite different names*

```diff
@@ -1,25 +1,25 @@
-<div id="navbar">
-    <ul>
-        <li class="main"><a href="#"><i>$SUBTITLE</i></a></li>
-        <li class="main"><a href="#">Details</a>
-            <ul>
-                <li class="sub"><a href="#">Compiled by: $COMPILEDBY</a></li>
-                <li class="sub"><a href="#">Compiled on: $NOW</a></li>
-                <li class="sub"><a href="#">Total files found: $QUANTITY</a></li>
-            </ul>
-        </li>
-        <li class="main"><a href="$BASEPATH">Folder</a></li>
-        <li class="main"><a href="#">Quick Help</a>
-            <ul>
-                <li class="sub"><a href="https://github.com/endangeredoxen/pywebify" target="_blank">Report generated by pywebify!  Click for more details.</a></li>
-                <li class="sub"><a href="#">Hover over links in left sidebar to display images/reports/data</a></li>
-                <li class="sub"><a href="#">+/- bullets indicate directories; click to expand</a></li>
-                <li
-                        class="sub"><a href="#">Ctrl+click on images to zoom in</a></li>
-                <li class="sub"><a href="#">Shift+click on images to zoom out</a></li>
-                <li class="sub"><a href="#">Alt+click on images to zoom to native image size</a></li>
-                <li class="sub"><a href="#">***Optimized for Chrome***</a></li>
-            </ul>
-        </li>
-    </ul>
-</div>
+<div id="navbar">
+        <ul>
+            <li class="main"><a href="#">$SUBTITLE</a></li>
+            <li class="main"><a href="#">Details</a>
+                <ul>
+                    <li class="sub"><a href="#">Compiled by: $COMPILEDBY</a></li>
+                    <li class="sub"><a href="#">Compiled on: $NOW</a></li>
+                    <li class="sub"><a href="#">Total files found: $QUANTITY</a></li>
+                </ul>
+            </li>
+            <li class="main"><a href="$BASEPATH">Folder</a></li>
+            <li class="main"><a href="#">Quick Help</a>
+                <ul>
+                    <li class="sub"><a href="https://github.com/endangeredoxen/pywebify" target="_blank">Report generated by pywebify!  Click for more details.</a></li>
+                    <li class="sub"><a href="#">Hover over links in left sidebar to display images/reports/data</a></li>
+                    <li class="sub"><a href="#">+/- bullets indicate directories; click to expand</a></li>
+                    <li
+                            class="sub"><a href="#">Ctrl+click on images to zoom in (&#8984; on mac)</a></li>
+                    <li class="sub"><a href="#">Shift+click on images to zoom out (command on mac)</a></li>
+                    <li class="sub"><a href="#">Alt+click on images to zoom to native image size</a></li>
+                    <li class="sub"><a href="#">***Optimized for Chrome***</a></li>
+                </ul>
+            </li>
+        </ul>
+    </div>
```

#### html2text {}

```diff
@@ -4,11 +4,11 @@
           o Compiled_on:_$NOW
           o Total_files_found:_$QUANTITY
     * Folder
     * Quick_Help
           o Report_generated_by_pywebify!_Click_for_more_details.
           o Hover_over_links_in_left_sidebar_to_display_images/reports/data
           o +/-_bullets_indicate_directories;_click_to_expand
-          o Ctrl+click_on_images_to_zoom_in
-          o Shift+click_on_images_to_zoom_out
+          o Ctrl+click_on_images_to_zoom_in_(⌘_on_mac)
+          o Shift+click_on_images_to_zoom_out_(command_on_mac)
           o Alt+click_on_images_to_zoom_to_native_image_size
           o ***Optimized_for_Chrome***
```

### Comparing `pywebify-0.2.6/pywebify/templates/html/webify.html` & `pywebify-0.3.0a0/src/pywebify/templates/html/webify.html`

 * *Files 18% similar despite different names*

```diff
@@ -1,65 +1,64 @@
-<!DOCTYPE html PUBLIC "-//W3C//DTD XHTML 1.0 Strict//EN"
-        "http://www.w3.org/TR/xhtml1/DTD/xhtml1-strict.dtd">
-<html xmlns="http://www.w3.org/1999/xhtml">
-
-<head>
-    <meta http-equiv="X-UA-Compatible" content="IE=Edge" />
-    <link rel="stylesheet" type="text/css" href="$CSS_FILE" />
-    <link rel="shortcut icon" type="image/x-icon" href="$FAVICON">
-    <script type='text/javascript' src='http://ajax.googleapis.com/ajax/libs/jquery/1.6.4/jquery.min.js'></script>
-    $JS_FILES
-</head>
-
-<body>
-    <title>$TITLE</title>
-    $NAVBAR
-    <div id="main_div">
-        <div id="sidebar">
-
-            $SIDEBAR
-
-        </div>
-
-        <div id="viewer">
-            <button id="toggle"></button> $START_SCREEN
-            <div id="summary">
-                $SUMMARY
-            </div>
-        </div>
-    </div>
-
-</body>
-<script>
-    // Automatically open to a specific image if ?id=path in url
-    window.onload = function() {
-        var url = window.location.href;
-        var queryString = url ? url.split('?')[1] : window.location.search.slice(1);
-        if (typeof queryString === "undefined") {
-            return;
-        }
-        var page = queryString.split('id=')[1].replace(new RegExp('%20', 'g'), ' ');
-        var pages = page.split('/');
-        var i;
-        var child;
-        var aTags = document.querySelectorAll("a[href='?" + queryString + "']");
-        if (aTags.length > 0) {
-            var parent = aTags[0].parentElement;
-            if (parent.children[0].onmouseover != null) {
-                parent.children[0].onmouseover();
-                for (var i = 0; i < (pages.length - 1) * 2; i++) {
-                    parent = parent.parentElement;
-                    parent.click();
-                }
-            } else {
-                // directories only
-                for (var i = 0; i < pages.length * 2; i++) {
-                    parent.click();
-                    parent = parent.parentElement;
-                }
-            }
-
-        }
-    }
-</script>
-
+<!DOCTYPE html PUBLIC "-//W3C//DTD XHTML 1.0 Strict//EN"
+        "http://www.w3.org/TR/xhtml1/DTD/xhtml1-strict.dtd">
+<html xmlns="http://www.w3.org/1999/xhtml">
+
+<head>
+    <meta http-equiv="X-UA-Compatible" content="IE=Edge" />
+    <link rel="stylesheet" type="text/css" href="$CSS_FILE" />
+    <link rel="shortcut icon" type="image/x-icon" href="$FAVICON">
+    <link rel="apple-touch-icon" href="$FAVICON">
+    <script type='text/javascript' src="$JQUERY"></script>
+    $JS_FILES
+</head>
+
+<body>
+    <title>$TITLE</title>
+    $NAVBAR
+    <div id="main_div">
+        <div id="sidebar">
+            $SIDEBAR
+        </div>
+
+        <div id="viewer">
+            <button id="toggle"></button> $START_SCREEN
+            <div id="summary">
+                $SUMMARY
+            </div>
+        </div>
+    </div>
+
+</body>
+<script>
+    // Automatically open to a specific image if ?id=path in url
+    window.onload = function() {
+        var url = window.location.href;
+        var queryString = url ? url.split('?')[1] : window.location.search.slice(1);
+        if (typeof queryString === "undefined") {
+            return;
+        }
+        var page = queryString.split('id=')[1].replace(new RegExp('%20', 'g'), ' ');
+        var pages = page.split('/');
+        var i;
+        var child;
+        var aTags = document.querySelectorAll("a[href='?" + queryString + "']");
+        if (aTags.length > 0) {
+            var parent = aTags[0].parentElement;
+            if (parent.children[0].onmouseover != null) {
+                parent.children[0].onmouseover();
+                for (var i = 0; i < (pages.length - 1) * 2; i++) {
+                    parent = parent.parentElement;
+                    parent.click();
+                }
+            } else {
+                // directories only
+                for (var i = 0; i < pages.length * 2; i++) {
+                    parent.click();
+                    parent = parent.parentElement;
+                }
+            }
+
+        }
+    }
+</script>
+
 </html>
```

#### html2text {}

```diff
@@ -1,7 +1,8 @@
 
 
+
  $JS_FILES
 $NAVBAR
 $SIDEBAR
  $START_SCREEN
 $SUMMARY
```

### Comparing `pywebify-0.2.6/pywebify/templates/jinja/tabs.html` & `pywebify-0.3.0a0/src/pywebify/templates/jinja/tabs.html`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,46 +1,46 @@
-<!DOCTYPE html>
-<html>
-  <head>
-    {% block head %}
-      <title>{% block title %}{% endblock %}</title>
-      <link rel="stylesheet" type="text/css" href="https://cdn.datatables.net/s/dt/jq-2.1.4,jszip-2.5.0,pdfmake-0.1.18,dt-1.10.10,af-2.1.0,b-1.1.0,b-colvis-1.1.0,b-html5-1.1.0,b-print-1.1.0,cr-1.3.0,fc-3.2.0,fh-3.1.0,kt-2.1.0,r-2.0.0,rr-1.1.0,sc-1.4.0,se-1.1.0/datatables.min.css"/>
-      <meta http-equiv="X-UA-Compatible" content="IE=edge">
-      <meta name="viewport" content="width=device-width, initial-scale=1.0">
-
-      <link rel= "stylesheet" type= "text/css" href= "{{relpath}}/static/css/datatables.css">
-      <link rel= "stylesheet" type= "text/css" href= "{{relpath}}/static/css/base.css">
-
-    {% endblock %}
-  </head>
-
-  <style type="text/css">
-    body {
-      padding-top: 0px;   /* remove pad in default for fixed navbar - could change default css/template */
-      margin: 0;
-      overflow: auto;
-    }
-  </style>
-
-  <body>
-    {% block content %}
-        {% for c in content %}
-            {{c|safe}}
-        {% endfor %}
-    {% endblock %}
-
-    <div class="divider"></div>
-      {% block footer %}
-      <hr>
-      {{footer|safe}}
-      {% endblock %}
-    </div>
-  </body>
-
-  <script src="{{relpath}}/static/js/datatables.min.js"></script> <!-- including jQuery and bootstrap -->
-  <script type="text/javascript" src="https://cdn.datatables.net/s/dt/jq-2.1.4,jszip-2.5.0,pdfmake-0.1.18,dt-1.10.10,af-2.1.0,b-1.1.0,b-colvis-1.1.0,b-html5-1.1.0,b-print-1.1.0,cr-1.3.0,fc-3.2.0,fh-3.1.0,kt-2.1.0,r-2.0.0,rr-1.1.0,sc-1.4.0,se-1.1.0/datatables.min.js"></script>
-  {% block javascript %}
-      {% for j in js %}
-          {{j|safe}}
-      {% endfor %}
-  {% endblock %}
+<!DOCTYPE html>
+<html>
+  <head>
+    {% block head %}
+      <title>{% block title %}{% endblock %}</title>
+      <link rel="stylesheet" type="text/css" href="https://cdn.datatables.net/s/dt/jq-2.1.4,jszip-2.5.0,pdfmake-0.1.18,dt-1.10.10,af-2.1.0,b-1.1.0,b-colvis-1.1.0,b-html5-1.1.0,b-print-1.1.0,cr-1.3.0,fc-3.2.0,fh-3.1.0,kt-2.1.0,r-2.0.0,rr-1.1.0,sc-1.4.0,se-1.1.0/datatables.min.css"/>
+      <meta http-equiv="X-UA-Compatible" content="IE=edge">
+      <meta name="viewport" content="width=device-width, initial-scale=1.0">
+
+      <link rel= "stylesheet" type= "text/css" href= "{{relpath}}/static/css/datatables.css">
+      <link rel= "stylesheet" type= "text/css" href= "{{relpath}}/static/css/base.css">
+
+    {% endblock %}
+  </head>
+
+  <style type="text/css">
+    body {
+      padding-top: 0px;   /* remove pad in default for fixed navbar - could change default css/template */
+      margin: 0;
+      overflow: auto;
+    }
+  </style>
+
+  <body>
+    {% block content %}
+        {% for c in content %}
+            {{c|safe}}
+        {% endfor %}
+    {% endblock %}
+
+    <div class="divider"></div>
+      {% block footer %}
+      <hr>
+      {{footer|safe}}
+      {% endblock %}
+    </div>
+  </body>
+
+  <script src="{{relpath}}/static/js/datatables.min.js"></script> <!-- including jQuery and bootstrap -->
+  <script type="text/javascript" src="https://cdn.datatables.net/s/dt/jq-2.1.4,jszip-2.5.0,pdfmake-0.1.18,dt-1.10.10,af-2.1.0,b-1.1.0,b-colvis-1.1.0,b-html5-1.1.0,b-print-1.1.0,cr-1.3.0,fc-3.2.0,fh-3.1.0,kt-2.1.0,r-2.0.0,rr-1.1.0,sc-1.4.0,se-1.1.0/datatables.min.js"></script>
+  {% block javascript %}
+      {% for j in js %}
+          {{j|safe}}
+      {% endfor %}
+  {% endblock %}
 </html>
```

### Comparing `pywebify-0.2.6/pywebify/templates/jinja/webpage.html` & `pywebify-0.3.0a0/src/pywebify/templates/jinja/webpage.html`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,47 +1,47 @@
-<!DOCTYPE html>
-<html>
-  <head>
-    {% block head %}
-    <title>{% block title %}{% endblock %}</title>
-      {% endblock %}
-      <meta http-equiv="X-UA-Compatible" content="IE=edge">
-      <meta name="viewport" content="width=device-width, initial-scale=1.0">
-      <link rel="shortcut icon" href="./static/img/favicon.ico" type="image/x-icon">
-      <link rel="icon" href="./static/img/favicon.ico" type="image/x-icon">
-      <link rel="stylesheet" type="text/css" href="https://cdn.datatables.net/s/dt/jq-2.1.4,jszip-2.5.0,pdfmake-0.1.18,dt-1.10.10,af-2.1.0,b-1.1.0,b-colvis-1.1.0,b-html5-1.1.0,b-print-1.1.0,cr-1.3.0,fc-3.2.0,fh-3.1.0,kt-2.1.0,r-2.0.0,rr-1.1.0,sc-1.4.0,se-1.1.0/datatables.min.css"/>
-  </head>
-
-  <style type="text/css">
-    body {
-      padding-top: 0px;   /* remove pad in default for fixed navbar - could change default css/template */
-      margin: 0;
-      overflow: auto;
-    }
-  </style>
-
-  <body>
-      {% block content %}
-        {{tablehead | safe}}
-        <style type="text/css">
-           .display {  font-size: 0.8em; }
-        </style>
-        {% for c in content %}
-          {{c|safe}}
-        {% endfor %}
-      {% endblock %}
-
-      {% block footer %}
-        {{tablefoot | safe}}
-      {% endblock %}
-  </body>
-
-  <!-- <script src="../../../../static/js/datatables.min.js"></script>  including jQuery and bootstrap -->
-  <script type="text/javascript" src="https://cdn.datatables.net/s/dt/jq-2.1.4,jszip-2.5.0,pdfmake-0.1.18,dt-1.10.10,af-2.1.0,b-1.1.0,b-colvis-1.1.0,b-html5-1.1.0,b-print-1.1.0,cr-1.3.0,fc-3.2.0,fh-3.1.0,kt-2.1.0,r-2.0.0,rr-1.1.0,sc-1.4.0,se-1.1.0/datatables.min.js"></script>
-
-  {% block javascript %}
-    {% for j in js %}
-      {{j|safe}}
-    {% endfor %}
-  {% endblock %}
-
-</html>
+<!DOCTYPE html>
+<html>
+  <head>
+    {% block head %}
+    <title>{% block title %}{% endblock %}</title>
+      {% endblock %}
+      <meta http-equiv="X-UA-Compatible" content="IE=edge">
+      <meta name="viewport" content="width=device-width, initial-scale=1.0">
+      <link rel="shortcut icon" href="./static/img/favicon.ico" type="image/x-icon">
+      <link rel="icon" href="./static/img/favicon.ico" type="image/x-icon">
+      <link rel="stylesheet" type="text/css" href="https://cdn.datatables.net/s/dt/jq-2.1.4,jszip-2.5.0,pdfmake-0.1.18,dt-1.10.10,af-2.1.0,b-1.1.0,b-colvis-1.1.0,b-html5-1.1.0,b-print-1.1.0,cr-1.3.0,fc-3.2.0,fh-3.1.0,kt-2.1.0,r-2.0.0,rr-1.1.0,sc-1.4.0,se-1.1.0/datatables.min.css"/>
+  </head>
+
+  <style type="text/css">
+    body {
+      padding-top: 0px;   /* remove pad in default for fixed navbar - could change default css/template */
+      margin: 0;
+      overflow: auto;
+    }
+  </style>
+
+  <body>
+      {% block content %}
+        {{tablehead | safe}}
+        <style type="text/css">
+           .display {  font-size: 0.8em; }
+        </style>
+        {% for c in content %}
+          {{c|safe}}
+        {% endfor %}
+      {% endblock %}
+
+      {% block footer %}
+        {{tablefoot | safe}}
+      {% endblock %}
+  </body>
+
+  <!-- <script src="../../../../static/js/datatables.min.js"></script>  including jQuery and bootstrap -->
+  <script type="text/javascript" src="https://cdn.datatables.net/s/dt/jq-2.1.4,jszip-2.5.0,pdfmake-0.1.18,dt-1.10.10,af-2.1.0,b-1.1.0,b-colvis-1.1.0,b-html5-1.1.0,b-print-1.1.0,cr-1.3.0,fc-3.2.0,fh-3.1.0,kt-2.1.0,r-2.0.0,rr-1.1.0,sc-1.4.0,se-1.1.0/datatables.min.js"></script>
+
+  {% block javascript %}
+    {% for j in js %}
+      {{j|safe}}
+    {% endfor %}
+  {% endblock %}
+
+</html>
```

### Comparing `pywebify-0.2.6/pywebify.egg-info/SOURCES.txt` & `pywebify-0.3.0a0/src/pywebify.egg-info/SOURCES.txt`

 * *Files 25% similar despite different names*

```diff
@@ -1,33 +1,34 @@
 MANIFEST.in
 README.rst
+pyproject.toml
 setup.cfg
 setup.py
-pywebify/__init__.py
-pywebify/config.ini
-pywebify/pywebify.py
-pywebify/setup.txt
-pywebify/template.py
-pywebify/version.txt
-pywebify/webpage.py
-pywebify.egg-info/PKG-INFO
-pywebify.egg-info/SOURCES.txt
-pywebify.egg-info/dependency_links.txt
-pywebify.egg-info/requires.txt
-pywebify.egg-info/top_level.txt
-pywebify/img/collapsed.png
-pywebify/img/expanded.png
-pywebify/img/favicon.png
-pywebify/js/collapse.js
-pywebify/js/div_switch.js
-pywebify/js/div_toggle.js
-pywebify/js/filter.js
-pywebify/js/pixelate.js
-pywebify/templates/css/collapse.css
-pywebify/templates/css/filter.css
-pywebify/templates/css/pixelate.css
-pywebify/templates/css/rst.css
-pywebify/templates/css/webify.css
-pywebify/templates/html/navbar.html
-pywebify/templates/html/webify.html
-pywebify/templates/jinja/tabs.html
-pywebify/templates/jinja/webpage.html
+src/pywebify/__init__.py
+src/pywebify/config.ini
+src/pywebify/config.py
+src/pywebify/html.py
+src/pywebify/pywebify.py
+src/pywebify/template.py
+src/pywebify.egg-info/PKG-INFO
+src/pywebify.egg-info/SOURCES.txt
+src/pywebify.egg-info/dependency_links.txt
+src/pywebify.egg-info/requires.txt
+src/pywebify.egg-info/top_level.txt
+src/pywebify/img/collapsed.png
+src/pywebify/img/expanded.png
+src/pywebify/img/favicon.png
+src/pywebify/js/collapse.js
+src/pywebify/js/div_switch.js
+src/pywebify/js/div_toggle.js
+src/pywebify/js/filter.js
+src/pywebify/js/jquery.min.js
+src/pywebify/js/pixelate.js
+src/pywebify/templates/css/collapse.css
+src/pywebify/templates/css/filter.css
+src/pywebify/templates/css/pixelate.css
+src/pywebify/templates/css/rst.css
+src/pywebify/templates/css/webify.css
+src/pywebify/templates/html/navbar.html
+src/pywebify/templates/html/webify.html
+src/pywebify/templates/jinja/tabs.html
+src/pywebify/templates/jinja/webpage.html
```

