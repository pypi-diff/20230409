# Comparing `tmp/typer_to_textual-2.4.0.tar.gz` & `tmp/typer_to_textual-2.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "typer_to_textual-2.4.0.tar", max compression
+gzip compressed data, was "typer_to_textual-2.5.0.tar", max compression
```

## Comparing `typer_to_textual-2.4.0.tar` & `typer_to_textual-2.5.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     2870 2023-04-05 09:16:57.709007 typer_to_textual-2.4.0/README.md
--rw-r--r--   0        0        0      425 2023-04-05 09:19:12.045007 typer_to_textual-2.4.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-03-29 11:21:58.866398 typer_to_textual-2.4.0/typer_to_textual/__init__.py
--rw-r--r--   0        0        0      104 2023-04-04 08:07:27.385679 typer_to_textual-2.4.0/typer_to_textual/__main__.py
--rw-r--r--   0        0        0     9387 2023-04-04 08:07:27.385679 typer_to_textual-2.4.0/typer_to_textual/command_options.py
--rw-r--r--   0        0        0     5860 2023-04-04 08:07:27.385679 typer_to_textual-2.4.0/typer_to_textual/homepage.py
--rw-r--r--   0        0        0    13310 2023-04-05 08:50:29.637004 typer_to_textual-2.4.0/typer_to_textual/main.py
--rw-r--r--   0        0        0     2253 2023-04-04 10:54:22.928499 typer_to_textual-2.4.0/typer_to_textual/show.py
--rw-r--r--   0        0        0     4553 2023-04-04 08:07:27.385679 typer_to_textual-2.4.0/typer_to_textual/style.css
--rw-r--r--   0        0        0     3760 1970-01-01 00:00:00.000000 typer_to_textual-2.4.0/setup.py
--rw-r--r--   0        0        0     3474 1970-01-01 00:00:00.000000 typer_to_textual-2.4.0/PKG-INFO
+-rw-r--r--   0        0        0     2870 2023-04-06 14:26:57.584733 typer_to_textual-2.5.0/README.md
+-rw-r--r--   0        0        0      425 2023-04-09 14:30:19.185821 typer_to_textual-2.5.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-03-29 11:21:58.866398 typer_to_textual-2.5.0/typer_to_textual/__init__.py
+-rw-r--r--   0        0        0      104 2023-04-06 14:26:57.588734 typer_to_textual-2.5.0/typer_to_textual/__main__.py
+-rw-r--r--   0        0        0     9381 2023-04-09 14:05:44.145818 typer_to_textual-2.5.0/typer_to_textual/command_options.py
+-rw-r--r--   0        0        0     5860 2023-04-09 14:08:14.433818 typer_to_textual-2.5.0/typer_to_textual/homepage.py
+-rw-r--r--   0        0        0    13021 2023-04-09 14:04:59.893818 typer_to_textual-2.5.0/typer_to_textual/main.py
+-rw-r--r--   0        0        0     2311 2023-04-09 14:17:16.297819 typer_to_textual-2.5.0/typer_to_textual/show.py
+-rw-r--r--   0        0        0     4553 2023-04-06 14:26:57.588734 typer_to_textual-2.5.0/typer_to_textual/style.css
+-rw-r--r--   0        0        0     3760 1970-01-01 00:00:00.000000 typer_to_textual-2.5.0/setup.py
+-rw-r--r--   0        0        0     3474 1970-01-01 00:00:00.000000 typer_to_textual-2.5.0/PKG-INFO
```

### Comparing `typer_to_textual-2.4.0/README.md` & `typer_to_textual-2.5.0/README.md`

 * *Files identical despite different names*

### Comparing `typer_to_textual-2.4.0/typer_to_textual/command_options.py` & `typer_to_textual-2.5.0/typer_to_textual/command_options.py`

 * *Files 1% similar despite different names*

```diff
@@ -229,9 +229,9 @@
                 Horizontal(
                     Button("show", id=f"show-{self.identifier}", classes="run"),
                     classes="command-horizontal-run",
                     )
             )
 
     BINDINGS = [
-        Binding(key="r", action="app.pop_screen_n('command')", description="return"),
+        Binding(key="r", action="app.type_r('command')", description="return"),
     ]
```

### Comparing `typer_to_textual-2.4.0/typer_to_textual/homepage.py` & `typer_to_textual-2.5.0/typer_to_textual/homepage.py`

 * *Files 1% similar despite different names*

```diff
@@ -92,15 +92,15 @@
 
     def compose(self) -> ComposeResult:
         yield Header("Homepage", classes="header")
         yield Footer()
 
     def on_mount(self) -> None:
 
-        global container
+        container = None
 
         title = self.title()
         self.mount(Static(f"[green][bold]{title}", classes="title"))
         self.mount(Vertical(id="homepage-vertical"))
 
         options, commands = self.parse_output()
```

### Comparing `typer_to_textual-2.4.0/typer_to_textual/main.py` & `typer_to_textual-2.5.0/typer_to_textual/main.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,34 +15,30 @@
 from typer_to_textual.show import Show
 
 
 def maximize() -> None:
     result = subprocess.run(["xdotool", "getactivewindow"], capture_output=True)
     window_id = result.stdout.decode().strip()
 
-    # Get the screen resolution
     res = subprocess.check_output("xrandr | grep '\*' | awk '{print $1}'", shell=True).decode().strip().split('x')
     screen_width = int(res[0])
     screen_height = int(res[1])
 
-    # Determine the window size based on screen resolution
     if screen_width <= 1366 and screen_height <= 768:
         window_size = "80%"
     else:
         window_size = "70%"
 
     subprocess.run(["xdotool", "windowsize", window_id, window_size, window_size])
 
-    # Calculate the window position to center it on the screen
     window_width = int(window_size[:-1]) / 100 * screen_width
     window_height = int(window_size[:-1]) / 100 * screen_height
     x_pos = int((screen_width - window_width) / 2)
     y_pos = int((screen_height - window_height) / 2)
 
-    # Move the window to the calculated position
     subprocess.run(["xdotool", "windowmove", window_id, str(x_pos), str(y_pos)])
 
 
 def homepage_output() -> Tuple[List[str], str]:
 
     if len(sys.argv) != 2:
         Console().print("[bold][red]Error[/red]: Pass only the name of application")
@@ -59,17 +55,18 @@
         for line in result.stdout.decode().split('\n'):
             if "Options" in line or "Commands" in line:
                 found = True
         if not found:
             for i in result.stderr.decode().split('\n'):
                 if i:
                     print(i.rstrip())
-            Console().print(f"[bold][red]Error[/red]: The executable is not a typer apllication")
+            Console().print(f"[bold][red]Error[/red]: The executable is not a typer application")
             sys.exit(1)
         return result.stdout.decode().split('\n'), application
+
     except FileNotFoundError:
         Console().print(f"[bold][red]Error[/red]: The application: '{application}' is not found")
         sys.exit(1)
 
 
 class Tui(App):
 
@@ -136,22 +133,22 @@
                         current_word = ""
 
                 words = list(filter(bool, words))
                 buttons[words[0]] = words[1]
 
         return buttons
 
-    def check(self, elements: str, id: str):
+    def check_fields(self, elements: str, page: str):
 
         validation_errors = False
 
-        screen_class = "HomePage" if id == "homepage" else "CommandOptions"
+        screen_class = "HomePage" if page == "homepage" else "CommandOptions"
 
         for screens in self.query(f"{screen_class}"):
-            if screens.identifier == id:
+            if screens.identifier == page:
                 for element in screens.query(f".{elements}"):
                     input_type = ''
                     tuple_types = []
 
                     for index, static_element in enumerate(element.query("Static"), start=1):
                         if index == 2 and static_element.name != "BOOLEAN":
                             tuple_types = static_element.name.split(" ")
@@ -215,20 +212,20 @@
 
     def homepage_field(self) -> list:
 
         homepage_data = []
         for element in self.query_one(HomePage).query(".homepage-horizontal"):
             key = element.query_one(".name").id.replace("-required", "")
             if len(element.query("Input")) > 0:
-                for index, i in enumerate(element.query("Input"), start=1):
+                for i in element.query("Input"):
                     if i.value != '':
                         homepage_data.append(key)
                         homepage_data.append(i.value)
             else:
-                for index, i in enumerate(element.query("Checkbox"), start=1):
+                for i in element.query("Checkbox"):
                     if str(i.value) == "True":
                         homepage_data.append(key)
 
         return homepage_data
 
     def command_page_field(self, command):
 
@@ -240,22 +237,22 @@
                 for element in screens.query(".command-horizontal"):
                     key = element.query_one(".name").id
                     if len(element.query(".input")) > 0:
                         if "-required" in key:
                             key = key.replace("-required", "")
                         diversi = len(set(i.placeholder for i in element.query(".input"))) > 1
                         if diversi:
-                            for index, i in enumerate(element.query(".input"), start=1):
+                            for i in element.query(".input"):
                                 if i.value != '':
                                     if key not in tuple_data:
                                         tuple_data[key] = [i.value]
                                     else:
                                         tuple_data[key].append(i.value)
                         else:
-                            for index, i in enumerate(element.query(".input"), start=1):
+                            for i in element.query(".input"):
                                 if "--argument--" in key and i.value != '':
                                     other_data.append(i.value)
                                 elif i.value != '':
                                     other_data.append(key)
                                     other_data.append(i.value)
                     else:
                         if "-required" in key:
@@ -268,30 +265,30 @@
     def on_button_pressed(self, event: Button.Pressed):
 
         values = self.command_buttons()
         buttons = values.keys()
 
         if event.button.id in buttons:
 
-            validation_errors = self.check("homepage-horizontal", "homepage")
+            validation_errors = self.check_fields("homepage-horizontal", "homepage")
             if validation_errors:
                 return
 
             description = values[event.button.id]
             homepage_data = self.homepage_field()
 
             if not self.is_screen_installed(event.button.id):
                 result = self.call_command(event.button.id, homepage_data)
                 self.install_screen(CommandOptions(result, event.button.id, description), name=event.button.id)
             self.push_screen(event.button.id)
 
         elif event.button.id.startswith("show-"):
 
             command = event.button.id.replace("show-", "")
-            validation_errors = self.check("command-horizontal", command)
+            validation_errors = self.check_fields("command-horizontal", command)
             if validation_errors:
                 return
 
             homepage_data = self.homepage_field()
             tuple_data, other_data = self.command_page_field(command)
 
             if not self.is_screen_installed(event.button.id):
@@ -311,15 +308,15 @@
                         input_element = Input(placeholder=f"...", classes="input")
                         container.mount(input_element, before=3)
                     elif event.button.id.startswith("one_less") and len(input_elements) > 1:
                         input_elements.first().remove()
                         if len(container.query("Input")) == 1:
                             container.query("Button").last().remove()
 
-    async def action_pop_screen_n(self, screen):
+    async def action_type_r(self, screen):
 
         input_has_focus = any(i.has_focus for i in self.query("Input"))
 
         if input_has_focus:
             for i in self.query("Input"):
                 if i.has_focus:
                     i.value = i.value + 'r'
```

### Comparing `typer_to_textual-2.4.0/typer_to_textual/show.py` & `typer_to_textual-2.5.0/typer_to_textual/show.py`

 * *Files 19% similar despite different names*

```diff
@@ -10,20 +10,20 @@
 
 class Header(Static):
     pass
 
 
 class Show(Screen):
 
-    def __init__(self, application, command, homepage_data=None, tuple_data=None, other_data=None) -> None:
+    def __init__(self, application, command, homepage_data=None, command_tuple_data=None, command_other_data=None) -> None:
         self.application = application
         self.command = command
         self.homepage_data = homepage_data
-        self.tuple_data = tuple_data
-        self.other_data = other_data
+        self.command_tuple_data = command_tuple_data
+        self.command_other_data = command_other_data
         super().__init__()
 
     def compose(self) -> ComposeResult:
         yield Header("Show", classes="header")
         yield Container(
                 Static("[bold][yellow]Operation in progress....", id="loading"),
                 id="show-container")
@@ -35,26 +35,26 @@
         args = application.split()
 
         for option in self.homepage_data:
             args.append(option)
 
         args.append(self.command)
 
-        for key, value in self.tuple_data.items():
+        for key, value in self.command_tuple_data.items():
             args.append(key)
             if value != "BOOL":
                 if isinstance(value, list):
                     for val in value:
                         args.append(val)
                 else:
                     values = value.split(",")
                     for val in values:
                         args.append(val.strip())
 
-        for element in self.other_data:
+        for element in self.command_other_data:
             args.append(element)
 
         result = subprocess.run(args, capture_output=True)
 
         output = result.stdout.decode().split('\n')
         stderr_lines = result.stderr.decode().split('\n')
 
@@ -65,9 +65,9 @@
             await self.query_one("#show-container").mount(Static(f"[bold]{error}", classes="output"))
 
     async def on_mount(self) -> None:
         await asyncio.sleep(0.1)
         asyncio.create_task(self.run_button())
 
     BINDINGS = [
-        Binding(key="r", action="app.pop_screen_n('show')", description="return"),
+        Binding(key="r", action="app.type_r('show')", description="return"),
     ]
```

### Comparing `typer_to_textual-2.4.0/typer_to_textual/style.css` & `typer_to_textual-2.5.0/typer_to_textual/style.css`

 * *Files identical despite different names*

### Comparing `typer_to_textual-2.4.0/setup.py` & `typer_to_textual-2.5.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 ['rich>=13.3.2,<14.0.0', 'textual>=0.10.1,<0.11.0', 'typer>=0.7.0,<0.8.0']
 
 extras_require = \
 {':python_version >= "3.10" and python_version < "4.0"': ['xdotool>=0.4.0,<0.5.0']}
 
 setup_kwargs = {
     'name': 'typer-to-textual',
-    'version': '2.4.0',
+    'version': '2.5.0',
     'description': '',
     'long_description': '# typer-to-texual\n\n**typer-to-textual** is a TUI developed through the Textual module, which aims to simplify \nthe use of applications. This tool analyzes the help screens of different typer applications and creates \na TUI that allows the user to select the desired commands and options easily and intuitively, without the \nneed to know all available commands and options by heart. In summary, the use of the interactive TUI \nrepresents a major step forward in simplifying the use of typer applications and making them more accessible \nto all users, even the less experienced ones.\n\n## Install\n\nAs a preliminary requirement, you need to install some utility:\n\n**xdotool**. Installs the package via prompt with the command: \'sudo apt-get install xdotool\'\n\nAfter that, you can proceed either via PyPI, or by cloning the repository and install dependencies.\nIf you opt for PyPI, run the following command:\n```bash\n$ pip install typer-to-textual\n```\n\nAfter that, **typer-to-textual** can be run with:\n```bash\n$ python3 -m typer-to-textual [typer_application]\n```\n\nIf you instead opt for the repository, you also need the [Poetry](https://python-poetry.org/) Python package manager.\nOn Debian-like OSes it can be installed with the following command:\n```bash\n$ sudo apt install python3-poetry\n```\nAfter that, run the following commands:\n```bash\n$ git clone https://github.com/palla98/typer-to-textual.git\n```\n\nafter downloading:\n```bash\n$ cd typer-to-textual\n\n$ poetry install\n```\n\nAfter that, **typer-to-textual** can be run with:\n```bash\n$ poetry run ./typer_to_textual.py [typer_application]\n```\n\nse però [typer_application] è \'**python3 -m [nome_modulo]**\' bisogna stare attenti perchè si utlizza\nl\'interprete Python dell\'ambiente virtuale creato da Poetry. Quindi bisogna andare ad installare \n[nome_modulo] nell\'ambiente virtuale altrimenti non viene riconosciuto.\n\noppure semplicemente si può lanciare il comando:\n```bash\npython3 typer_to_textual.py \'python3 -m [nome_modulo]\'\n```\n\nla cosa migliore è andare a creare uno script .sh in modo tale da passare direttamente un eseguibile\nLo si va a creare e salvare nella tua directory bin personale:\n(~/.local/bin/[nome_script].sh):\n```bash\nsudo nano ~/.local/bin/[nome_script].sh\n```\n\n```bash\n#!/bin/bash\n\nOLD_PWD=$PWD\n\ncd path/to/executable\npoetry run ./executable "$@"\ncd $PWD\n```\nIn seguito renderlo eseguibile con questo comando:\n```bash\nsudo chmod +x ~/.local/bin/[nome_script].sh\n```\n\ne poi andare a creare un link simbolico:\n```bash\nsudo ln -s  ~/.local/bin/[nome_script].sh ~/.local/bin/[nome_script]\n```\nDopodichè semplicemente basterà chiamare lo script digitando semplicemente il comando [nome_script]\nda qualsiasi posizione nel terminale.\n\nquindi si potrà usare typer-to-textual anche in questo modo senza avere problemi di ambiente virtuale:\n```bash\npoetry run ./typer_to_textual.py [nome_script]\n```',
     'author': 'palla98',
     'author_email': 'pallaria98@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `typer_to_textual-2.4.0/PKG-INFO` & `typer_to_textual-2.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: typer-to-textual
-Version: 2.4.0
+Version: 2.5.0
 Summary: 
 Author: palla98
 Author-email: pallaria98@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

