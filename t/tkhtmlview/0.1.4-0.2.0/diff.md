# Comparing `tmp/tkhtmlview-0.1.4.tar.gz` & `tmp/tkhtmlview-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tkhtmlview-0.1.4.tar", max compression
+gzip compressed data, was "tkhtmlview-0.2.0.tar", max compression
```

## Comparing `tkhtmlview-0.1.4.tar` & `tkhtmlview-0.2.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1104 2023-03-23 12:57:26.030696 tkhtmlview-0.1.4/LICENSE
--rw-r--r--   0        0        0     4480 2023-03-23 12:57:26.030696 tkhtmlview-0.1.4/README.md
--rw-r--r--   0        0        0      352 2023-03-23 12:57:26.030696 tkhtmlview-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     3743 2023-03-23 12:57:26.030696 tkhtmlview-0.1.4/tkhtmlview/__init__.py
--rw-r--r--   0        0        0    25894 2023-03-23 12:57:26.030696 tkhtmlview-0.1.4/tkhtmlview/html_parser.py
--rw-r--r--   0        0        0      436 2023-03-23 12:57:26.030696 tkhtmlview-0.1.4/tkhtmlview/utils.py
--rw-r--r--   0        0        0     5143 1970-01-01 00:00:00.000000 tkhtmlview-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1104 2023-04-09 11:29:00.624744 tkhtmlview-0.2.0/LICENSE
+-rw-r--r--   0        0        0     4625 2023-04-09 11:29:00.624744 tkhtmlview-0.2.0/README.md
+-rw-r--r--   0        0        0      352 2023-04-09 11:29:00.628744 tkhtmlview-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     3743 2023-04-09 11:29:00.628744 tkhtmlview-0.2.0/tkhtmlview/__init__.py
+-rw-r--r--   0        0        0    26728 2023-04-09 11:29:00.628744 tkhtmlview-0.2.0/tkhtmlview/html_parser.py
+-rw-r--r--   0        0        0      436 2023-04-09 11:29:00.628744 tkhtmlview-0.2.0/tkhtmlview/utils.py
+-rw-r--r--   0        0        0     5288 1970-01-01 00:00:00.000000 tkhtmlview-0.2.0/PKG-INFO
```

### Comparing `tkhtmlview-0.1.4/LICENSE` & `tkhtmlview-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tkhtmlview-0.1.4/README.md` & `tkhtmlview-0.2.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -132,11 +132,15 @@
 | ol       | style, type        | 1, a, A list types only                |
 | p        | style              |
 | pre      | style              |
 | span     | style              |
 | strong   | style              |
 | u        | style              |
 | ul       | style              | bullet glyphs only                     |
+| table,tr,th,td | - | basic support|
+
+> Note: All styles are not supported; 
+> align with justify is not supported; it falls back to left align
 
 ## License
 
 [![FOSSA Status](https://app.fossa.io/api/projects/git%2Bgithub.com%2Fbauripalash%2Ftkhtmlview.svg?type=large)](https://app.fossa.io/projects/git%2Bgithub.com%2Fbauripalash%2Ftkhtmlview?ref=badge_large)
```

### Comparing `tkhtmlview-0.1.4/tkhtmlview/__init__.py` & `tkhtmlview-0.2.0/tkhtmlview/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 tkinter HTML text widgets
 """
 import sys
 import tkinter as tk
 from tkhtmlview import html_parser
 from tkhtmlview.utils import RenderHTML
 
-VERSION = "0.1.4"
+VERSION = "0.2.0"
 
 
 class _ScrolledText(tk.Text):
     def __init__(self, master=None, **kw):
         self.frame = tk.Frame(master)
 
         self.vbar = tk.Scrollbar(self.frame)
```

### Comparing `tkhtmlview-0.1.4/tkhtmlview/html_parser.py` & `tkhtmlview-0.2.0/tkhtmlview/html_parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -54,14 +54,18 @@
         CODE = "code"
         H1 = "h1"
         H2 = "h2"
         H3 = "h3"
         H4 = "h4"
         H5 = "h5"
         H6 = "h6"
+        TABLE = "table"
+        TR = "tr"
+        TH = "th"
+        TD = "td"
 
     class Attrs:
         STYLE = "style"
         HREF = "href"
         SRC = "src"
         WIDTH = "width"
         HEIGHT = "height"
@@ -97,34 +101,40 @@
         Tag.UL,
         Tag.OL,
         Tag.LI,
         Tag.DIV,
         Tag.P,
         Tag.PRE,
         Tag.CODE,
+        Tag.TD,
+        Tag.TH,
     )
 
     NEW_LINE_TAGS = HEADING_TAGS + (
         Tag.UL,
         Tag.OL,
         Tag.DIV,
         Tag.P,
         Tag.PRE,
         Tag.CODE,
+        Tag.TABLE,
+        Tag.TR,
     )
 
     STYLE_TAGS = TEXT_ALIGN_TAGS + (
         Tag.A,
         Tag.B,
         Tag.STRONG,
         Tag.I,
         Tag.EM,
         Tag.U,
         Tag.MARK,
         Tag.SPAN,
+        Tag.TD,
+        Tag.TH,
     )
 
 
 # --------------------------------------------------------------------------------------------------
 # Text widget defs
 
 
@@ -509,14 +519,17 @@
 
                     self._stack_add(tag, Fnt.UNDERLINE, False)
                     self._stack_add(tag, Fnt.OVERSTRIKE, False)
                     self._w_tags_add()
                     self._w.insert(tk.INSERT, line_index)
                     self._stack_pop(tag, Fnt.UNDERLINE)
                     self._stack_pop(tag, Fnt.OVERSTRIKE)
+                    
+            elif tag == HTML.Tag.TH or tag == HTML.Tag.TD:
+                    self._w.insert(tk.INSERT, "\t")
 
         elif tag == HTML.Tag.IMG and attrs[HTML.Attrs.SRC]:
             # -------------------------------------------------------------------- [ UNSTYLED_TAGS ]
             image = None
             # print(attrs[HTML.Attrs.SRC] , self.cached_images)
             if attrs[HTML.Attrs.SRC].startswith(("https://", "ftp://", "http://")):
                 if attrs[HTML.Attrs.SRC] in self.cached_images.keys():
@@ -545,15 +558,22 @@
                 if str(attrs[HTML.Attrs.HEIGHT]).isdigit():
                     height = int(attrs[HTML.Attrs.HEIGHT])
                     resize = True
                 if resize:
                     image = image.resize((width, height), Image.ANTIALIAS)
                 self.images.append(ImageTk.PhotoImage(image))
                 self._w.image_create(tk.INSERT, image=self.images[-1])
-
+                
+        elif tag == HTML.Tag.TABLE:
+                tabs = []
+                for i in range(30): # HF was len(self.list_tags)):
+                    offset = 40 * (i + 1)
+                    tabs += [offset, tk.LEFT ]
+                self._stack_add(tag, WCfg.TABS, tabs)
+            
         if self.strip:
             if tag == HTML.Tag.BR:
                 self._insert_new_line()
             else:
                 self.html_tags.append(tag)
 
         if (
@@ -692,14 +712,17 @@
             tag[WTag.START_INDEX] = key
             tag[WTag.END_INDEX] = end_index
             end_index = key
 
         # add tags
         self.hlink_slots = []
         for key, tag in self._w_tags.items():
+            if "config" in tag: # HF change justify to left for tkinter (only supports left, right, center)
+                if tag["config"].get("justify") == "justify":
+                    tag["config"]["justify"] = "left"
             self._w.tag_add(key, tag[WTag.START_INDEX], tag[WTag.END_INDEX])
             self._w.tag_config(key, font=font.Font(**tag[Fnt.KEY]), **tag[WCfg.KEY])
             if tag[Bind.KEY][Bind.LINK]:
                 self.hlink_slots.append(
                     HLinkSlot(self._w, key, tag[Bind.KEY][Bind.LINK])
                 )
                 self._w.tag_bind(key, "<Button-1>", self.hlink_slots[-1].call)
```

### Comparing `tkhtmlview-0.1.4/PKG-INFO` & `tkhtmlview-0.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tkhtmlview
-Version: 0.1.4
+Version: 0.2.0
 Summary: Display HTML with Tkinter
 License: MIT
 Author: Palash Bauri
 Author-email: palashbauri1@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -151,12 +151,16 @@
 | ol       | style, type        | 1, a, A list types only                |
 | p        | style              |
 | pre      | style              |
 | span     | style              |
 | strong   | style              |
 | u        | style              |
 | ul       | style              | bullet glyphs only                     |
+| table,tr,th,td | - | basic support|
+
+> Note: All styles are not supported; 
+> align with justify is not supported; it falls back to left align
 
 ## License
 
 [![FOSSA Status](https://app.fossa.io/api/projects/git%2Bgithub.com%2Fbauripalash%2Ftkhtmlview.svg?type=large)](https://app.fossa.io/projects/git%2Bgithub.com%2Fbauripalash%2Ftkhtmlview?ref=badge_large)
```

