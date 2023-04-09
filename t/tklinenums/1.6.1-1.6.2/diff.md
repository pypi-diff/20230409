# Comparing `tmp/tklinenums-1.6.1.tar.gz` & `tmp/tklinenums-1.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tklinenums-1.6.1.tar", last modified: Sun Apr  9 18:21:48 2023, max compression
+gzip compressed data, was "tklinenums-1.6.2.tar", last modified: Sun Apr  9 19:25:24 2023, max compression
```

## Comparing `tklinenums-1.6.1.tar` & `tklinenums-1.6.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 18:21:48.515345 tklinenums-1.6.1/
--rw-r--r--   0 runner    (1001) docker     (123)      862 2023-04-09 18:21:48.515345 tklinenums-1.6.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      606 2023-04-09 18:21:29.000000 tklinenums-1.6.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-09 18:21:48.515345 tklinenums-1.6.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      461 2023-04-09 18:21:29.000000 tklinenums-1.6.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 18:21:48.511345 tklinenums-1.6.1/tklinenums/
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-09 18:21:29.000000 tklinenums-1.6.1/tklinenums/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10852 2023-04-09 18:21:29.000000 tklinenums-1.6.1/tklinenums/tklinenums.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 18:21:48.511345 tklinenums-1.6.1/tklinenums.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      862 2023-04-09 18:21:48.000000 tklinenums-1.6.1/tklinenums.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-04-09 18:21:48.000000 tklinenums-1.6.1/tklinenums.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-09 18:21:48.000000 tklinenums-1.6.1/tklinenums.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-09 18:21:48.000000 tklinenums-1.6.1/tklinenums.egg-info/top_level.txt
+drwxr-xr-x   0 joshyacktman   (501) staff       (20)        0 2023-04-09 19:25:24.830981 tklinenums-1.6.2/
+-rw-r--r--   0 joshyacktman   (501) staff       (20)      862 2023-04-09 19:25:24.830712 tklinenums-1.6.2/PKG-INFO
+-rw-r--r--   0 joshyacktman   (501) staff       (20)      606 2023-04-09 19:24:42.000000 tklinenums-1.6.2/README.md
+-rw-r--r--   0 joshyacktman   (501) staff       (20)       38 2023-04-09 19:25:24.831045 tklinenums-1.6.2/setup.cfg
+-rw-r--r--   0 joshyacktman   (501) staff       (20)      461 2023-04-09 19:24:49.000000 tklinenums-1.6.2/setup.py
+drwxr-xr-x   0 joshyacktman   (501) staff       (20)        0 2023-04-09 19:25:24.828739 tklinenums-1.6.2/tklinenums/
+-rw-r--r--   0 joshyacktman   (501) staff       (20)       38 2023-04-07 18:10:10.000000 tklinenums-1.6.2/tklinenums/__init__.py
+-rw-r--r--   0 joshyacktman   (501) staff       (20)    10056 2023-04-09 19:21:06.000000 tklinenums-1.6.2/tklinenums/tklinenums.py
+drwxr-xr-x   0 joshyacktman   (501) staff       (20)        0 2023-04-09 19:25:24.830368 tklinenums-1.6.2/tklinenums.egg-info/
+-rw-r--r--   0 joshyacktman   (501) staff       (20)      862 2023-04-09 19:25:24.000000 tklinenums-1.6.2/tklinenums.egg-info/PKG-INFO
+-rw-r--r--   0 joshyacktman   (501) staff       (20)      202 2023-04-09 19:25:24.000000 tklinenums-1.6.2/tklinenums.egg-info/SOURCES.txt
+-rw-r--r--   0 joshyacktman   (501) staff       (20)        1 2023-04-09 19:25:24.000000 tklinenums-1.6.2/tklinenums.egg-info/dependency_links.txt
+-rw-r--r--   0 joshyacktman   (501) staff       (20)       11 2023-04-09 19:25:24.000000 tklinenums-1.6.2/tklinenums.egg-info/top_level.txt
```

### Comparing `tklinenums-1.6.1/PKG-INFO` & `tklinenums-1.6.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: tklinenums
-Version: 1.6.1
+Version: 1.6.2
 Summary: A simple Tkinter widget for displaying line numbers
 Home-page: https://github.com/Moosems/TkLineNums
 Author: Moosems
 Author-email: moosems.j@gmail.com
 Description-Content-Type: text/markdown
 
-# TkLineNums V.1.6.1
+# TkLineNums V.1.6.2
 
 TkLineNums is a simple line numbering widget for Tkinter. It supports ttk themes through the set_to_ttk_style method.
 
 ![img](https://github.com/Moosems/TkLineNums/raw/main/images/TkLineNumsPhoto.png)
 
 ## Features
```

### Comparing `tklinenums-1.6.1/README.md` & `tklinenums-1.6.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# TkLineNums V.1.6.1
+# TkLineNums V.1.6.2
 
 TkLineNums is a simple line numbering widget for Tkinter. It supports ttk themes through the set_to_ttk_style method.
 
 ![img](https://github.com/Moosems/TkLineNums/raw/main/images/TkLineNumsPhoto.png)
 
 ## Features
```

### Comparing `tklinenums-1.6.1/tklinenums/tklinenums.py` & `tklinenums-1.6.2/tklinenums/tklinenums.py`

 * *Files 16% similar despite different names*

```diff
@@ -30,15 +30,14 @@
         * .reload_font(): Reloads the font of the widget (Requires font as argument)
     """
 
     def __init__(
         self,
         master: Misc,
         editor: Text,
-        font: tuple | Font | str | None = None,
         justify: str = "left",
         *args,
         **kwargs,
     ) -> None:
         """Initializes the widget -- Internal use only"""
         self.textwidget = editor
         self.master = master
@@ -53,15 +52,14 @@
             borderwidth=2
             if kwargs.get("borderwidth") is None
             else kwargs.get("borderwidth"),
             relief="ridge" if kwargs.get("relief") is None else kwargs.get("relief"),
             *args,
             **kwargs,
         )
-        self.set_font(font)
         self.set_to_ttk_style()
 
         self.bind("<MouseWheel>", self.mouse_scroll, add=True)
         self.bind("<Button-1>", self.click_see, add=True)
         self.bind("<ButtonRelease-1>", self.unclick, add=True)
         self.bind("<Double-Button-1>", self.double_click, add=True)
         self.bind("<Button1-Motion>", self.drag, add=True)
@@ -83,15 +81,15 @@
                 if self.justify == "left"
                 else int(self["width"])
                 if self.justify == "right"
                 else int(self["width"]) / 2,
                 dlineinfo[1],
                 text=f" {lineno} " if self.justify != "center" else f"{lineno}",
                 anchor={"left": "nw", "right": "ne", "center": "n"}[self.justify],
-                font=self.font,
+                font=self.textwidget.cget("font"),
                 fill=self.foreground,
             )
 
     def mouse_scroll(self, event: Event) -> None:
         """Scrolls the text widget when the mouse wheel is scrolled -- Internal use only"""
         if system == "Darwin":
             self.textwidget.yview_scroll(scroll_inversion * event.delta, "units")
@@ -142,15 +140,15 @@
          - Once it starts going it's hard to stop drag clicking (because most people pull back up when done but this is still
            considered dragging and it remembers the direction meaning it will continue to drag in that direction)
          - When you reach your end point for scroll clicking you can't go back unless you go completely the opposite way which 
            then means you can't go back the original way
          - When you go down and then try to go back up you can't
          - Must continue to drag cursor for it to select more even if cursor is off-screen or trying to slowly select more (Means
            it might need to become recursive)
-        """ #TODO: Fix issues
+        """  # TODO: Fix issues
         if self.click_pos is None:
             return
         start, end = self.textwidget.index("insert"), self.click_pos
         if self.textwidget.compare("insert", ">", self.click_pos):
             start, end = end, start
         self.textwidget.mark_set("insert", f"@0,{event.y}")
         self.textwidget.tag_remove("sel", "1.0", "end")
@@ -191,50 +189,30 @@
         if self.textwidget.compare(start_pos, ">", end_pos):
             start_pos, end_pos = end_pos, start_pos
         self.textwidget.tag_add("sel", start_pos, end_pos)
 
     def resize(self) -> None:
         """Resizes the widget to fit the text widget"""
         end = self.textwidget.index("end").split(".")[0]
-        self.config(width=self.font.measure(" 1234 ")) if int(
-            end
-        ) <= 1000 else self.config(width=self.font.measure(f" {end} "))
+        self.config(
+            width=Font(font=(temp_font := self.textwidget.cget("font"))).measure(
+                " 1234 "
+            )
+        ) if int(end) <= 1000 else self.config(width=temp_font.measure(f" {end} "))
 
     def set_to_ttk_style(self) -> None:
         """Sets the widget to the ttk style"""
         self["bg"] = self.tk.eval("ttk::style lookup TLineNumbers -background")
         self.foreground = self.tk.eval("ttk::style lookup TLineNumbers -foreground")
 
-    def reload(self, font: tuple | Font | str = "TkFixedFont") -> None:
-        """Reloads the widget with a new font"""
-        self.set_font(font)
+    def reload(self) -> None:
+        """Reloads the widget"""
         self.set_to_ttk_style()
         self.redraw()
 
-    def set_font(self, font: tuple | Font | str | None) -> None:
-        """Sets the font of the widget"""
-        if isinstance(font, Font):
-            self.font: Font = font
-        elif isinstance(font, tuple):
-            self.font: Font = Font(family=font[0], size=font[1])
-        elif isinstance(font, str) and not font.startswith("{"):
-            self.font: Font = Font(name=font, exists=True)
-        else:
-            self.font: Font = Font(
-                family=" ".join(
-                    (
-                        font := self.textwidget["font"]
-                        .replace("{", "")
-                        .replace("}", "")
-                        .split(" ")
-                    )[:-1]
-                ),
-                size=font[-1],
-            )
-
 
 if __name__ == "__main__":
     import platform
     from tkinter import Text, Tk
     from tkinter.font import Font
     from tkinter.ttk import Style
 
@@ -262,9 +240,10 @@
 
     text.bind("<Key>", lambda event: root.after_idle(linenums.redraw), add=True)
     text.bind(f"<BackSpace>", lambda event: root.after_idle(linenums.redraw), add=True)
     text.bind(
         f"<{contmand}-v>", lambda event: root.after_idle(linenums.redraw), add=True
     )
     text["yscrollcommand"] = linenums.redraw
+    text.config(font=("Courier New bold", 13))
 
     root.mainloop()
```

### Comparing `tklinenums-1.6.1/tklinenums.egg-info/PKG-INFO` & `tklinenums-1.6.2/tklinenums.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: tklinenums
-Version: 1.6.1
+Version: 1.6.2
 Summary: A simple Tkinter widget for displaying line numbers
 Home-page: https://github.com/Moosems/TkLineNums
 Author: Moosems
 Author-email: moosems.j@gmail.com
 Description-Content-Type: text/markdown
 
-# TkLineNums V.1.6.1
+# TkLineNums V.1.6.2
 
 TkLineNums is a simple line numbering widget for Tkinter. It supports ttk themes through the set_to_ttk_style method.
 
 ![img](https://github.com/Moosems/TkLineNums/raw/main/images/TkLineNumsPhoto.png)
 
 ## Features
```

