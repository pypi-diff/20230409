# Comparing `tmp/esse3_student-3.4.0.tar.gz` & `tmp/esse3_student-3.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "esse3_student-3.4.0.tar", max compression
+gzip compressed data, was "esse3_student-3.6.0.tar", max compression
```

## Comparing `esse3_student-3.4.0.tar` & `esse3_student-3.6.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0    11357 2022-12-19 10:49:50.550756 esse3_student-3.4.0/LICENSE
--rw-r--r--   0        0        0        0 2022-12-19 10:49:50.546754 esse3_student-3.4.0/esse3_student/__init__.py
--rw-r--r--   0        0        0      103 2023-04-04 08:07:35.493731 esse3_student-3.4.0/esse3_student/__main__.py
--rw-r--r--   0        0        0    16884 2023-04-04 10:11:19.476494 esse3_student-3.4.0/esse3_student/cli.py
--rw-r--r--   0        0        0    15023 2023-04-04 08:07:35.493731 esse3_student-3.4.0/esse3_student/esse3_wrapper.py
--rw-r--r--   0        0        0     1793 2023-03-30 11:18:57.907602 esse3_student-3.4.0/esse3_student/primitives.py
--rw-r--r--   0        0        0        0 2023-01-17 09:15:01.604898 esse3_student-3.4.0/esse3_student/tui/__init__.py
--rw-r--r--   0        0        0    10198 2023-04-04 08:07:35.493731 esse3_student-3.4.0/esse3_student/tui/booklet.py
--rw-r--r--   0        0        0     5771 2023-03-30 11:18:57.895597 esse3_student-3.4.0/esse3_student/tui/exams.py
--rw-r--r--   0        0        0     4442 2023-03-30 11:18:57.871585 esse3_student-3.4.0/esse3_student/tui/main.py
--rw-r--r--   0        0        0     7450 2023-03-30 11:18:57.915607 esse3_student-3.4.0/esse3_student/tui/reservations.py
--rw-r--r--   0        0        0     7018 2023-03-29 11:22:15.266594 esse3_student-3.4.0/esse3_student/tui/style.css
--rw-r--r--   0        0        0     2936 2023-03-30 11:18:57.967633 esse3_student-3.4.0/esse3_student/tui/taxes.py
--rw-r--r--   0        0        0        0 2022-12-19 10:49:50.542752 esse3_student-3.4.0/esse3_student/utils/__init__.py
--rw-r--r--   0        0        0      162 2022-12-19 10:49:50.542752 esse3_student-3.4.0/esse3_student/utils/console.py
--rw-r--r--   0        0        0     4668 2023-03-30 11:20:34.848047 esse3_student-3.4.0/esse3_student/utils/primitives.py
--rw-r--r--   0        0        0      991 2022-12-19 10:49:50.542752 esse3_student-3.4.0/esse3_student/utils/validators.py
--rw-r--r--   0        0        0      814 2023-04-04 10:11:24.660494 esse3_student-3.4.0/pyproject.toml
--rw-r--r--   0        0        0     1326 1970-01-01 00:00:00.000000 esse3_student-3.4.0/setup.py
--rw-r--r--   0        0        0     1258 1970-01-01 00:00:00.000000 esse3_student-3.4.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2022-12-19 10:49:50.550756 esse3_student-3.6.0/LICENSE
+-rw-r--r--   0        0        0        0 2022-12-19 10:49:50.546754 esse3_student-3.6.0/esse3_student/__init__.py
+-rw-r--r--   0        0        0      103 2023-04-06 14:27:12.244058 esse3_student-3.6.0/esse3_student/__main__.py
+-rw-r--r--   0        0        0    16169 2023-04-08 13:44:03.091663 esse3_student-3.6.0/esse3_student/cli.py
+-rw-r--r--   0        0        0    15453 2023-04-08 13:45:53.721355 esse3_student-3.6.0/esse3_student/esse3_wrapper.py
+-rw-r--r--   0        0        0     1774 2023-04-08 13:31:38.102107 esse3_student-3.6.0/esse3_student/primitives.py
+-rw-r--r--   0        0        0        0 2023-01-17 09:15:01.604898 esse3_student-3.6.0/esse3_student/tui/__init__.py
+-rw-r--r--   0        0        0    10284 2023-04-09 13:42:37.495211 esse3_student-3.6.0/esse3_student/tui/booklet.py
+-rw-r--r--   0        0        0     5016 2023-04-09 13:41:54.009478 esse3_student-3.6.0/esse3_student/tui/exams.py
+-rw-r--r--   0        0        0     4442 2023-03-30 11:18:57.871585 esse3_student-3.6.0/esse3_student/tui/main.py
+-rw-r--r--   0        0        0     6518 2023-04-09 13:41:53.949448 esse3_student-3.6.0/esse3_student/tui/reservations.py
+-rw-r--r--   0        0        0     6652 2023-04-09 13:48:39.804275 esse3_student-3.6.0/esse3_student/tui/style.css
+-rw-r--r--   0        0        0     2991 2023-04-09 13:44:45.875369 esse3_student-3.6.0/esse3_student/tui/taxes.py
+-rw-r--r--   0        0        0        0 2022-12-19 10:49:50.542752 esse3_student-3.6.0/esse3_student/utils/__init__.py
+-rw-r--r--   0        0        0      162 2022-12-19 10:49:50.542752 esse3_student-3.6.0/esse3_student/utils/console.py
+-rw-r--r--   0        0        0     4668 2023-03-30 11:20:34.848047 esse3_student-3.6.0/esse3_student/utils/primitives.py
+-rw-r--r--   0        0        0      991 2022-12-19 10:49:50.542752 esse3_student-3.6.0/esse3_student/utils/validators.py
+-rw-r--r--   0        0        0      814 2023-04-09 14:31:43.073821 esse3_student-3.6.0/pyproject.toml
+-rw-r--r--   0        0        0     1326 1970-01-01 00:00:00.000000 esse3_student-3.6.0/setup.py
+-rw-r--r--   0        0        0     1258 1970-01-01 00:00:00.000000 esse3_student-3.6.0/PKG-INFO
```

### Comparing `esse3_student-3.4.0/LICENSE` & `esse3_student-3.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `esse3_student-3.4.0/esse3_student/cli.py` & `esse3_student-3.6.0/esse3_student/cli.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from typing import Tuple
 from rich import box
 from rich.progress import track
 from rich.table import Table
 from rich.text import Text
 
 from esse3_student.esse3_wrapper import Esse3Wrapper
-from esse3_student.primitives import AcademicYear, ExamStatus, Cfu, Year, ExamName, Grade, Date, SigningUp, Description
+from esse3_student.primitives import AcademicYear, ExamStatus, Cfu, Year, ExamName, Grade
 from esse3_student.utils.console import console
 
 from typing import Optional
 
 
 @dataclasses.dataclass(frozen=True)
 class AppOptions:
@@ -82,36 +82,32 @@
     """
 
     esse_wrapper = new_esse3_wrapper()
     with console.status("[bold]Retrieval of [green]available exams[/green] in progress[/]",
                         spinner="aesthetic"):
         time.sleep(2)
         exams = esse_wrapper.fetch_exams()
-    exams = [(ExamName(value='BUSINESS GAME'), Date(value='08/02/2023'), SigningUp(value='18/01/2023 - 06/02/2023'), Description(value='MDCS 6 ECTS')),
-                     (ExamName(value='DATA ANALYTICS'), Date(value='06/02/2023'), SigningUp(value='23/12/2022 - 04/02/2023'), Description(value='Secondo appello')),
-                     (ExamName(value='NETWORK SECURITY'), Date(value='07/02/2023'), SigningUp(value='05/01/2023 - 06/02/2023'), Description(value='Oral exam and project discussion')),
-                     (ExamName(value='THEORETICAL COMPUTER SCIENCE'), Date(value='28/01/2023'), SigningUp(value='13/01/2023 - 27/01/2023'), Description(value='Prova orale con alcune domande scritte')),
-                    ]
+
     if len(exams) == 0:
-        console.print("No exams available!!!", style="bold red")
-        exit()
+        console.log(f"[bold]❌ No available exams!!![/]\n")
+    else:
+        console.rule("[bold]EXAMS SHOWCASE[/]")
 
-    console.rule("[bold]EXAMS SHOWCASE[/]")
+        table = Table(box=box.SIMPLE_HEAD, style="rgb(139,69,19)", leading=1)
+        table.add_column("#", justify="center", style="bold red")
+        table.add_column("Name", justify="center", style="bold cyan")
+        table.add_column("Date", justify="center", style="bold green")
+        table.add_column("Signing up", justify="center", style="bold yellow")
+        table.add_column("Description", justify="center", style="bold #f7ecb5")
 
-    table = Table(box=box.SIMPLE_HEAD, style="rgb(139,69,19)", leading=1)
-    table.add_column("#", justify="center", style="bold red")
-    table.add_column("Name", justify="center", style="bold cyan")
-    table.add_column("Date", justify="center", style="bold green")
-    table.add_column("Signing up", justify="center", style="bold yellow")
-    table.add_column("Description", justify="center", style="bold #f7ecb5")
+        for index, (name, date, signing_up, description) in enumerate(exams, start=1):
+            table.add_row(str(index), name.value, date.value, signing_up.value, description.value)
 
-    for index, (name, date, signing_up, description) in enumerate(exams, start=1):
-        table.add_row(str(index), name.value, date.value, signing_up.value, description.value)
+        console.print(table, justify="center")
 
-    console.print(table, justify="center")
     console.rule("[bold]STATISTICS[/]", style="yellow")
     console.print("\n[bold]clicks saved: [blue]7[/]\n", justify="center")
 
 
 @app.command(name="reservations")
 def command_reservations() -> None:
 
@@ -120,141 +116,140 @@
     """
 
     esse_wrapper = new_esse3_wrapper()
     with console.status("[bold]Fetching [green]available reservations[/] in progress....[/]", spinner="aesthetic"):
         time.sleep(2)
         reservations = esse_wrapper.fetch_reservations()
         if len(reservations) == 0:
-            console.print("No exams booked!!!", style="bold red")
-            exit()
-
-    console.rule("[bold]RESERVATIONS SHOWCASE[/]")
-    tables = {}
-    for index in range(len(reservations)):
-        tables[f'table_{index}'] = Table(box=box.SIMPLE_HEAD, style="rgb(139,69,19)")
-        tables[f'table_{index}'].add_column("#", justify="center", style="bold red")
-        for colum in reservations[index].keys():
-            if colum == "Name":
-                tables[f'table_{index}'].add_column(colum, justify="center", style="bold cyan", no_wrap=True)
-            elif colum == "Date":
-                tables[f'table_{index}'].add_column(colum, justify="center", style="bold yellow")
-            elif colum == "Cancella Prenotazione":
-                tables[f'table_{index}'].add_column(colum, justify="center", style="bold red")
-            else:
-                tables[f'table_{index}'].add_column(colum, justify="center", style="bold #f7ecb5")
-
-    for index, reservation in enumerate(reservations, start=0):
-        row = list(reservation.values())
-        tables[f'table_{index}'].add_row(str(index+1), *row)
-        console.print(tables[f'table_{index}'], justify="center")
+            console.log(f"[bold]❌ No booked exams!!![/]\n")
+        else:
+            console.rule("[bold]RESERVATIONS SHOWCASE[/]")
+            tables = {}
+            for index in range(len(reservations)):
+                tables[f'table_{index}'] = Table(box=box.SIMPLE_HEAD, style="rgb(139,69,19)")
+                tables[f'table_{index}'].add_column("#", justify="center", style="bold red")
+                for colum in reservations[index].keys():
+                    if colum == "Name":
+                        tables[f'table_{index}'].add_column(colum, justify="center", style="bold cyan", no_wrap=True)
+                    elif colum == "Date":
+                        tables[f'table_{index}'].add_column(colum, justify="center", style="bold yellow")
+                    elif colum == "Cancella Prenotazione":
+                        tables[f'table_{index}'].add_column(colum, justify="center", style="bold red")
+                    else:
+                        tables[f'table_{index}'].add_column(colum, justify="center", style="bold #f7ecb5")
+
+            for index, reservation in enumerate(reservations, start=0):
+                row = list(reservation.values())
+                tables[f'table_{index}'].add_row(str(index+1), *row)
+                console.print(tables[f'table_{index}'], justify="center")
 
     console.rule("[bold]STATISTICS[/]", style="yellow")
     console.print("\n[bold]clicks saved: [blue]7[/]\n", justify="center")
 
 
 @app.command(name="add")
 def command_add(
         exams: list[str] = typer.Argument(
             ...,
-            metavar="exam names",
-            help="[bold]one or more strings of the form 'add name1 name2ssssssssssssssssssssssssssssssssssssssssssssssssssssssssssssss'"
+            metavar="Exam names",
+            help="[bold]One or more strings. Example: add 'name_1' 'name_2'"
         ),
 ):
     """
     [bold][#E1C699]Operation that allows the [green]booking[/green] of examinations[/][/bold] :blue_book:
     """
 
-    def parse(exams: list) -> list[ExamName]:
+    def parse(names: list) -> list[ExamName]:
         try:
-            exams_list = [ExamName(v) for v in exams]
+            exams_list = [ExamName(v) for v in names]
         except ValueError:
-            console.print("[bold red]Invalid strings[/]")
+            console.print("[bold yellow]Invalid strings[/]")
             raise typer.Exit()
 
         return exams_list
 
     values = parse(exams)
 
     esse_wrapper = new_esse3_wrapper()
 
     with console.status(f"[bold]Exams [green]booking[/] in progress....[/]", spinner="aesthetic"):
         exams, click = esse_wrapper.add(list(values))
         values = [i.value for i in exams]
         if len(values) == 0:
-            console.print("No exams available or wrong names passed!!!\n", style="bold red")
+            console.log("[bold]❌ No exams available or wrong names passed!!![/]\n")
         else:
             console.log(f"[bold] ✅ Exams with name: [green]{', '.join(map(str, values))}[/] added\n")
 
     console.rule("[bold]STATISTICS[/]", style="yellow")
     console.print(f"\n[bold]clicks saved: [blue]{click}[/]\n", justify="center")
 
 
 @app.command(name="remove")
-def command_remove_reservation(
+def command_remove(
         reservations: list[str] = typer.Argument(
             ...,
             metavar="Reservations name",
-            help="[bold]one or more strings of the form 'remove name1 name2'"
+            help="[bold]One or more strings of the form. Example: remove 'name_1' 'name_2'"
         ),
 
 ):
 
     """
     [bold][#E1C699]Operation that allows the [red]deletion[/red] of booked examinations[/][/bold] :wastebasket:
     """
 
-    def parse(reservations: list) -> list[ExamName]:
+    def parse(names: list) -> list[ExamName]:
         try:
-            exams_list = [ExamName(v) for v in reservations]
+            exams_list = [ExamName(v) for v in names]
         except ValueError:
-            console.print("[bold red]Invalid strings[/]")
+            console.print("[bold yellow]Invalid strings[/]")
             raise typer.Exit()
 
         return exams_list
 
     values = parse(reservations)
 
     esse3_wrapper = new_esse3_wrapper()
 
     with console.status(f"[bold]Searching [green]reservations[/] to remove in progress....[/]", spinner="aesthetic"):
         time.sleep(2)
         values, click = esse3_wrapper.remove(list(values))
 
         if len(values) == 0:
-            console.log(f"[bold]❌ No exams to remove or wrong values passed[/]!!!")
+            console.log(f"[bold]❌ No exams to remove or wrong values passed[/]!!!\n")
         else:
             all_success = True
             all_closed = True
             for i in values.keys():
                 if i == 0:
                     all_success = False
                 else:
                     all_closed = False
 
             if all_closed:
                 console.log(
-                    f"[bold]❌ Impossible to remove: [red]{', '.join([x for x in values[0]])}[/] cause subscription closed or wrong names passed[/]")
+                    f"[bold]❌ Impossible to remove: [red]{', '.join([x for x in values[0]])}[/] cause subscription closed or wrong names passed[/]\n")
             elif all_success:
-                console.log(f"[bold]Reservations: [green]{', '.join([x for x in values[1]])}[/] removed\n[/]")
+                console.log(f"[bold]✅ Reservations: [green]{', '.join([x for x in values[1]])}[/] removed\n[/]")
             else:
-                console.log(f"[bold]✅ Reservations: [green]{', '.join([x for x in values[1]])}[/] removed[/]")
+                console.log(f"[bold]✅ Reservations: [green]{', '.join([x for x in values[1]])}[/] removed[/]\n")
                 console.log(
-                    f"[bold]❌ Impossible to remove: [red]{', '.join([x for x in values[0]])}[/] cause subscription closed or wrong names passed[/]")
+                    f"[bold]❌ Impossible to remove: [red]{', '.join([x for x in values[0]])}[/] cause subscription closed or wrong names passed[/]\n")
 
     console.rule("[bold]STATISTICS[/]", style="yellow")
     console.print(f"\n[bold]clicks saved: [blue]{click}[/]\n", justify="center")
 
 
 @app.command(name="booklet")
 def command_booklet(
-        academic_year: int = typer.Option(int, help="[bold]Academic year (1 to 3)"),
-        exam_status: str = typer.Option(str, help="[bold]'[green]Superata[/]' like 'Passed' or '[yellow]Frequenza attribuita d'ufficio[/]' like 'To do'[/]"),
-        exam_grade: int = typer.Option(int, help="[bold]Grade of the exam[/]"),
-        new_average: Tuple[int, str] = typer.Option((None, None), help="[bold]calculate new average with grade: (grade cfu); ex: '25 12' [/]"),
-        statistics: Optional[bool] = typer.Option(False, "--statistics", "-s", help="[bold]show statistics on the average"),
+        academic_year: int = typer.Option(int, help="[bold]Academic year (1|2|3)"),
+        exam_status: str = typer.Option(str, help="[bold][green]'passed'[/green] or [yellow]'to be done'[/yellow]"),
+        exam_grade: int = typer.Option(int, help="[bold]Grade of the exam (from 18 to 30)"),
+        new_average: Tuple[int, str] = typer.Option((None, None), help="[bold]Plan a new average: '25 12' (grade cfu)"),
+        statistics: Optional[bool] = typer.Option(False, "--statistics", "-s", help="[bold]Show statistics on the actual averages"),
 ) -> None:
 
     """
     [bold][#E1C699]shows all the student's activities[/][/bold] :bookmark_tabs:
     """
 
     if academic_year:
@@ -302,15 +297,15 @@
     table.add_column("Academic Year", style="bold", justify="center")
     table.add_column("CFU", style="bold", justify="center")
     table.add_column("Status", style="bold")
     table.add_column("Grade", style="bold", justify="center")
     table.add_column("Date", style="#E1C699 bold", justify="center")
 
     def get_status_color(status):
-        colors = {"Passed": "green", "Ex officio assigned frequency": "yellow"}
+        colors = {"passed": "green", "to be done": "yellow"}
         return colors[status]
 
     def get_grade_color(grade):
         colors = {"18": "bright_red", "19": "bright_red", "20": "bright_red", "21": "bright_red",
                   "22": "yellow", "23": "yellow", "24": "yellow", "25": "yellow",
                   "26": "blue", "27": "blue", "28": "blue", "29": "blue", "30": "blue",
                   '': "white", "...": "white", "ELIGIBLE": "green"}
@@ -365,15 +360,15 @@
     console.rule("[bold]STATISTICS[/bold]")
     console.print("\n[bold]clicks saved: [blue]7[/]\n", justify="center")
 
 
 @app.command(name="taxes")
 def command_taxes(
         payment: str = typer.Option(str, help="[bold]Shows taxes by status type: ('to pay'|'confirmed'|'refund')"),
-        year: int = typer.Option(int, "--year", "-y", help="[bold]filter taxes by year; es: '2021'"),
+        year: int = typer.Option(int, "--year", "-y", help="[bold]Filter taxes by year; es: 2021"),
 ) -> None:
 
     """
     [bold][#E1C699]Show all taxes[/][/bold] :bookmark_tabs:
     """
 
     if year:
```

### Comparing `esse3_student-3.4.0/esse3_student/esse3_wrapper.py` & `esse3_student-3.6.0/esse3_student/esse3_wrapper.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import dataclasses
+import sys
 import time
 import subprocess
-
+import typeguard
 import screeninfo
+
 from dataclasses import InitVar
-from typing import List, Tuple, Union, Any
 
-import typeguard
 from selenium import webdriver
 from selenium.common import WebDriverException
 from selenium.common.exceptions import NoSuchElementException
 from selenium.common.exceptions import TimeoutException
 from selenium.webdriver import Keys
 from selenium.webdriver.common.by import By
 from selenium.webdriver.support.ui import WebDriverWait
@@ -44,22 +44,21 @@
 
 def prompt_position() -> None:
 
     result = subprocess.run(["xdotool", "getactivewindow"], capture_output=True)
     window_id = result.stdout.decode().strip()
     screen_height = subprocess.check_output(["xdotool", "getdisplaygeometry"]).decode().split()[1]
 
-    subprocess.run(["xdotool", "windowmove", window_id, "0", str(int(screen_height) // 4)])
-    subprocess.run(["xdotool", "windowsize", window_id, "50%", "-1"])
+    subprocess.run(["xdotool", "windowmove", window_id, "10", str(int(screen_height) // 4)])
+    subprocess.run(["xdotool", "windowsize", window_id, "50%", str(int(screen_height) // 2)])
     # con -1 l'altezza rimane invariata altrimenti lasciare  str(int(screen_height) // 2)
 
 
 def driver_position(driver) -> None:
 
-    #self.driver.maximize_window()
     screen = screeninfo.get_monitors()[0]
     width, height = screen.width, screen.height
     driver.set_window_size(width // 2, height)
     driver.set_window_position(width // 2, 0)
 
 
 @typeguard.typechecked
@@ -111,31 +110,42 @@
     def is_headless(self) -> bool:
         return self.driver.execute_script("return navigator.webdriver")
 
     def __login(self, username: Username, password: Password) -> None:
 
         self.driver.get(LOGIN_URL)
 
-        """try:
+        try:
             WebDriverWait(self.driver, 2).until \
                 (EC.visibility_of_element_located(
                     (By.XPATH, "//*[@id='c-s-bn']")))
-            self.driver.find_element(By.XPATH, "//*[@id='c-s-bn']").click()
-        except:
-            pass"""
+            btn_cookies = self.driver.find_element(By.XPATH, "//*[@id='c-s-bn']")
+            btn_cookies.send_keys(Keys.ENTER)
+        except TimeoutException:
+            pass
+
+        self.driver.find_element(By.ID, 'u').send_keys(username.value)
+        self.driver.find_element(By.ID, 'p').send_keys(password.value)
+        self.driver.find_element(By.ID, 'btnLogin').send_keys(Keys.RETURN)
+
+        try:
+            WebDriverWait(self.driver, 2).until(EC.visibility_of_element_located(
+                (By.XPATH, "//*[@id='alertErr']")))
+            error_message = "\033[1m\033[31mERROR:\033[0m \033[1m{}\033[0m".format("Wrong Credentials!!!")
+            print(error_message)
+            sys.exit(1)
+        except TimeoutException:
+            pass
 
         try:
-            self.driver.find_element(By.ID, 'u').send_keys(username.value)
-            self.driver.find_element(By.ID, 'p').send_keys(password.value)
-            self.driver.find_element(By.ID, 'btnLogin').send_keys(Keys.RETURN)
             carrier = WebDriverWait(self.driver, 2).until(EC.visibility_of_element_located(
                 (By.XPATH, "/html/body/div[2]/div/div/main/div[3]/div/div/table/tbody/tr[1]/td[5]/div/a")))
-            carrier.click()
-        except Exception:
-            raise RuntimeError("Wrong credentials")
+            carrier.send_keys(Keys.RETURN)
+        except TimeoutException:
+            pass
 
     def __logout(self) -> None:
         self.driver.get(LOGOUT_URL)
 
     def minimize(self) -> None:
         self.driver.minimize_window()
 
@@ -164,15 +174,15 @@
 
     def fetch_reservations(self) -> list:
 
         self.driver.get(RESERVATIONS_URL)
         try:
             reservations = WebDriverWait(self.driver, 5).until(
                 EC.visibility_of_all_elements_located((By.XPATH, "//*[@id='boxPrenotazione']")))
-        except:
+        except TimeoutException:
             return []
 
         rows = []
 
         index = 2
         for reservation in reservations:
             name = reservation.find_element(By.XPATH,
@@ -196,15 +206,15 @@
     def add(self, names: list[ExamName]) -> tuple[list[ExamName], int]:
 
         self.driver.get(EXAMS_URL)
         click = 7
         try:
             exams = WebDriverWait(self.driver, 5).until(
                 EC.visibility_of_all_elements_located((By.XPATH, "//table/tbody/tr")))
-        except:
+        except TimeoutException:
             return [], click
 
         added = []
 
         while names:
             name = names.pop().value
             wrong = True
@@ -233,50 +243,50 @@
 
     def remove(self, names: list[ExamName]) -> tuple[{}, int]:
 
         self.driver.get(RESERVATIONS_URL)
         click = 7
 
         try:
-            box_prenotazione = WebDriverWait(self.driver, 5).until(
+            box_reservation = WebDriverWait(self.driver, 5).until(
                 EC.visibility_of_all_elements_located((By.XPATH, "//*[@id='boxPrenotazione']")))
             tool_bar = WebDriverWait(self.driver, 5).until(
                 EC.visibility_of_all_elements_located((By.XPATH, "//*[@id='toolbarAzioni']")))
-        except:
+        except TimeoutException:
             return {}, click
 
         values = {
             0: [],
             1: [],
         }
 
         for reservation in names:
             found = False
-            for i, name in enumerate(box_prenotazione, start=1):
+            for i, name in enumerate(box_reservation, start=1):
                 value = name.find_element(By.CLASS_NAME, "record-h2").text.split(" [")[0].strip()
                 reservation_name = reservation.value.upper()
                 if value == reservation_name:
                     try:
                         element = tool_bar[i - 1].find_element(By.ID, 'btnCancella')
-                        element.click()
+                        element.send_keys(Keys.ENTER)
                         confirm = self.driver.find_element(By.XPATH, "//*[@id='btnConferma']")
-                        confirm.click()
+                        confirm.send_keys(Keys.ENTER)
                         click += 2
                         values[1].append(reservation_name)
                         found = True
                         break
                     except NoSuchElementException:
                         pass
             if not found:
                 values[0].append(reservation.value)
             else:
                 self.driver.get(RESERVATIONS_URL)
                 WebDriverWait(self.driver, 10).until(
                     EC.visibility_of_element_located((By.XPATH, "//*[@id='textHeader']")))
-                box_prenotazione = self.driver.find_elements(By.XPATH, "//*[@id='boxPrenotazione']")
+                box_reservation = self.driver.find_elements(By.XPATH, "//*[@id='boxPrenotazione']")
                 tool_bar = self.driver.find_elements(By.XPATH, "//*[@id='toolbarAzioni']")
 
         values = {k: v for k, v in values.items() if v}
 
         return values, click
 
     def fetch_booklet(self) -> tuple[list[tuple[ExamName, AcademicYear, Cfu, ExamStatus, BookletGrade, Date]], tuple[float, int]]:
@@ -304,42 +314,41 @@
             # Separate the string "grade_date" into two parts using the separator " - "
             grade, date = (grade_date.replace("&nbsp;-&nbsp;", " - ").split(" - ") + [''])[:2]
 
             grade = "ELIGIBLE" if grade == "IDO" else grade or "..."
             date = Date.of(date or "None")
 
             if status == "Superata":
-                status = "Passed"
+                status = "passed"
                 cfu_achieved += int(cfu)
             else:
-                status = "Ex officio assigned frequency"
+                status = "to be done"
 
             rows.append((ExamName.of(name), AcademicYear.of(int(academic_year)), Cfu.of(cfu),
                          ExamStatus.of(status), BookletGrade.of(grade), date))
 
         statistics = (float(weighted_average), int(cfu_achieved))
 
         return rows, statistics
 
-
     def fetch_taxes(self) -> tuple[list[tuple[TaxeID, Date, Amount, TaxeStatus]], int]:
 
         self.driver.get(TAXES_URL)
         click = 7
 
         taxes = WebDriverWait(self.driver, 10).until(
             EC.visibility_of_all_elements_located((By.XPATH, "//*[@id='tasse-tableFatt']/tfoot/tr/td/div/ul/li/a")))
         rows = []
 
         start = 3
         while start < len(taxes):
             page = self.driver.find_element(By.XPATH, f"//*[@id='tasse-tableFatt']/tfoot/tr/td/div/ul/li[{start}]/a")
             if 0 < int(page.text) < 10:
                 if start != 3:
-                    page.click()
+                    page.send_keys(Keys.RETURN)
                     click += 1
                 time.sleep(1)
                 taxes = self.driver.find_elements(By.XPATH, "/html/body/div[2]/div/div/main/div[3]/div/div/table[1]/tbody/tr")
                 for index, taxe in enumerate(taxes, start=1):
 
                     id = taxe.find_element(By.XPATH, f"/html/body/div[2]/div/div/main/div[3]/div/div/table[1]/tbody/tr[{index}]/td[1]/a").text
                     expiration_date = taxe.find_element(By.XPATH, f"/html/body/div[2]/div/div/main/div[3]/div/div/table[1]/tbody/tr[{index}]/td[4]").get_attribute('data-sort-value')
```

### Comparing `esse3_student-3.4.0/esse3_student/primitives.py` & `esse3_student-3.6.0/esse3_student/primitives.py`

 * *Files 4% similar despite different names*

```diff
@@ -54,15 +54,15 @@
 
 
 @bounded_integer(min_value=2010, max_value=datetime.datetime.now().year)
 class Year:
     pass
 
 
-@bounded_string(min_length=6, max_length=29, pattern=r"(Passed|Ex officio assigned frequency)")
+@bounded_string(min_length=6, max_length=29, pattern=r"(passed|to be done)")
 class ExamStatus:
     pass
 
 
 @bounded_integer(min_value=18, max_value=30)
 class Grade:
     pass
```

### Comparing `esse3_student-3.4.0/esse3_student/tui/booklet.py` & `esse3_student-3.6.0/esse3_student/tui/booklet.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 
 class Header(Static):
     pass
 
 
 def get_status(status: str) -> Text:
-    colors = {"Passed": "green", "Ex officio assigned frequency": "#f7ecb5"}
+    colors = {"passed": "green", "to be done": "#f7ecb5"}
     value = Text(status)
     value.stylize(f"{colors[status]}")
 
     return value
 
 
 def get_grade(grade: str) -> Text:
@@ -38,15 +38,15 @@
 
 
 class Booklet(Screen):
 
     exams = None
     statistics = None
 
-    class Tables(Static):
+    class ViewExams(Static):
 
         def __init__(self, exams) -> None:
             self.exams = exams
             super().__init__()
 
         def on_mount(self):
             self.id = "booklet-table-exams"
@@ -83,21 +83,21 @@
             self.table(self.averages)
 
         def table(self, averages):
             table = Table(header_style="rgb(255,204,51) bold", box=box.SIMPLE_HEAD)
             table.add_column("Actual Average", style="bold", justify="center")
             table.add_column("Actual Degree basis", style="bold", justify="center")
 
-            actual_average, actual_cfu  = averages
+            actual_average, actual_cfu = averages
             degree_basis = (float(actual_average) * 11) / 3
 
             table.add_row(str(actual_average), str(round(degree_basis, 2)))
             self.update(table)
 
-    class NewAverage(Static):
+    class PlanAverage(Static):
 
         def __init__(self, averages) -> None:
             self.averages = averages
             super().__init__()
 
         def compose(self) -> ComposeResult:
             yield Container(
@@ -114,39 +114,38 @@
             if event.button.id == "compute-average":
                 buttons = ["#result", "#booklet-value-error"]
                 for element in buttons:
                     try:
                         self.query(element).last().remove()
                     except:
                         pass
+
                 average_to_achieve = self.query_one("#average").value
                 remaining_cfu = self.query_one("#cfu").value
+
                 if average_to_achieve != "" and remaining_cfu != "":
                     try:
 
                         average_to_achieve = Grade(int(average_to_achieve)).value
                         remaining_cfu = int(remaining_cfu)
-
                         actual_average, actual_cfu = self.averages
-
                         total_cfu = remaining_cfu + actual_cfu
-
                         grade_to_obtain = ((average_to_achieve * total_cfu) - (actual_average * actual_cfu)) \
                                           / float(remaining_cfu)
 
                         self.query_one(".booklet-container-filters").mount(Static(f"[b]The grade you need to take \n"
                                                                                   f"for each upcoming exam\n"
                                                                                   f"having [yellow]{remaining_cfu} cfu available[/]: "
                                                                                   f"[green]{str(round(grade_to_obtain, 2))}", id="result"))
 
                     except ValueError:
                         self.query_one(".booklet-container-filters").mount(
                             Static("[red][bold]Wrong values[/]", id="booklet-value-error"))
 
-    class NewGrade(Static):
+    class ProjectsGrade(Static):
 
         def __init__(self, averages) -> None:
             self.averages = averages
             super().__init__()
 
         def compose(self) -> ComposeResult:
             yield Container(
@@ -163,20 +162,23 @@
             if event.button.id == "compute-grade":
                 buttons = ["#result", "#booklet-value-error"]
                 for element in buttons:
                     try:
                         self.query(element).last().remove()
                     except:
                         pass
+
                 grade = self.query_one("#grade").value
                 cfu = self.query_one("#cfu").value
+
                 if grade != "" and cfu != "":
                     try:
                         grade = Grade(int(grade)).value
                         cfu = int(Cfu(cfu).value)
+
                         actual_average, actual_cfu = self.averages
                         new_average = ((actual_average * actual_cfu) + (int(grade) * int(cfu))) / (
                                 actual_cfu + int(cfu))
                         new_degree_basis = (new_average * 11.0) / 3.0
 
                         self.query_one(".booklet-container-filters").mount(Static(
                             f"[b][yellow]New Average:[/] {round(new_average, 2)}/30\n[yellow]New Degree basis:[/] "
@@ -185,37 +187,38 @@
 
                     except ValueError:
                         self.query_one(".booklet-container-filters").mount(
                             Static("[red][bold]Wrong values[/]", id="booklet-value-error"))
 
     async def fetch_data(self) -> None:
 
-        global wrapper
+        wrapper = None
         try:
             wrapper = cli.new_esse3_wrapper()
         except:
             await self.query_one("#booklet-loading").remove()
             await self.query_one("#booklet-container").mount(Static("Login failed !!!", classes="login-failed"))
 
-        self.exams, self.statistics = wrapper.fetch_booklet()
+        if wrapper:
+            self.exams, self.statistics = wrapper.fetch_booklet()
 
-        await self.query_one("#booklet-loading").remove()
-        await self.query_one("#booklet-container").mount(
-            Vertical(self.Tables(self.exams))
-        )
-        await self.query_one("#booklet-container").mount(
-                            Static("Planning:", classes="title"),
-                            Container(
-                                self.ActualAverage(self.statistics),
-                                Button("Plan a new average", id="average"),
-                                Button("Projects a new grade", id="grade"),
-                                Button("clear", id="clear"),
-                                classes="booklet-container-options"
-                            ),
-                        )
+            await self.query_one("#booklet-loading").remove()
+            await self.query_one("#booklet-container").mount(
+                Vertical(self.ViewExams(self.exams))
+            )
+            await self.query_one("#booklet-container").mount(
+                                Static("Planning:", classes="title"),
+                                Container(
+                                    self.ActualAverage(self.statistics),
+                                    Button("Plan a new average", id="average"),
+                                    Button("Projects a new grade", id="grade"),
+                                    Button("clear", id="clear"),
+                                    classes="booklet-container-options"
+                                ),
+                            )
 
     async def on_mount(self) -> None:
         await asyncio.sleep(0.1)
         asyncio.create_task(self.fetch_data())
 
     def compose(self) -> ComposeResult:
         yield Header("Booklet", classes="header")
@@ -224,15 +227,15 @@
             Static("[b][yellow]exams booklet[/] loading in progress....[/]", id="booklet-loading"),
             id="booklet-container"
         )
         yield Footer()
 
     def on_button_pressed(self, event: Button.Pressed):
 
-        elements_to_remove = [self.NewAverage, self.NewGrade]
+        elements_to_remove = [self.PlanAverage, self.ProjectsGrade]
         compute_buttons = ["compute-average", "compute-grade"]
 
         if event.button.id == "clear":
             for element in elements_to_remove:
                 try:
                     self.query(element).last().remove()
                 except:
@@ -243,18 +246,18 @@
             for element in elements_to_remove:
                 try:
                     self.query(element).last().remove()
                 except:
                     pass
 
         if event.button.id == "average":
-            self.query_one("#booklet-container").mount(self.NewAverage(self.statistics))
+            self.query_one("#booklet-container").mount(self.PlanAverage(self.statistics))
 
         if event.button.id == "grade":
-            self.query_one("#booklet-container").mount(self.NewGrade(self.statistics))
+            self.query_one("#booklet-container").mount(self.ProjectsGrade(self.statistics))
 
         if event.button.id == "degree":
             self.query_one("#booklet-container").mount(self.NewDegree(self.exams))
 
     BINDINGS = [
         Binding(key="r", action="app.pop_screen", description="return"),
     ]
```

### Comparing `esse3_student-3.4.0/esse3_student/tui/exams.py` & `esse3_student-3.6.0/esse3_student/tui/exams.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import asyncio
 
 from esse3_student import cli
-from esse3_student.primitives import ExamName, Date, SigningUp, Description
 
 from textual.app import ComposeResult
 from textual.binding import Binding
 from textual.widgets import Static, Button, Footer, Checkbox
 from textual.containers import Container, Horizontal, Vertical
 from textual.screen import Screen
 
@@ -15,15 +14,15 @@
 
 class Header(Static):
     pass
 
 
 class Exams(Screen):
 
-    class Tables(Static):
+    class ViewExams(Static):
 
         def __init__(self, exams: list) -> None:
             self.exams = exams
             super().__init__()
 
         def on_mount(self) -> None:
             self.get_table(self.exams)
@@ -38,15 +37,15 @@
             table.add_column("Description", justify="center", style="bold #f7ecb5")
 
             for index, (name, date, signing_up, description) in enumerate(exams, start=1):
                 table.add_row(str(index), name.value, date.value, signing_up.value, description.value)
 
             self.update(table)
 
-    class Line(Horizontal):
+    class SelectExams(Horizontal):
 
         def __init__(self, exam) -> None:
             self.value = exam
             super().__init__()
 
         def on_mount(self) -> None:
             self.mount(self.Name(self.value[0].value))
@@ -70,51 +69,50 @@
                 self.id = self.name_value
 
     BINDINGS = [
         Binding(key="r", action="app.pop_screen", description="return"),
     ]
 
     async def fetch_date(self) -> None:
-        """exams = [(ExamName(value='BUSINESS GAME'), Date(value='08/02/2023'), SigningUp(value='18/01/2023 - 06/02/2023'), Description(value='MDCS 6 ECTS')),
-                 (ExamName(value='DATA ANALYTICS'), Date(value='06/02/2023'), SigningUp(value='23/12/2022 - 04/02/2023'), Description(value='Secondo appello')),
-                 (ExamName(value='NETWORK SECURITY'), Date(value='07/02/2023'), SigningUp(value='05/01/2023 - 06/02/2023'), Description(value='Oral exam and project discussion')),
-                 (ExamName(value='THEORETICAL COMPUTER SCIENCE'), Date(value='28/01/2023'), SigningUp(value='13/01/2023 - 27/01/2023'), Description(value='Prova orale con alcune domande scritte')),
-                ]"""
-        global wrapper
+
+        wrapper = None
         try:
             wrapper = cli.new_esse3_wrapper()
         except:
             await self.query_one(".exams-loading").remove()
-            await self.query_one(".reservations-container").mount(Static("Login failed !!!", classes="login-failed"))
+            await self.query_one(".exams-container").mount(Static("Login failed !!!", classes="login-failed"))
+
+        if wrapper:
+            exams = wrapper.fetch_exams()
+            await self.query_one(".exams-loading").remove()
+
+            if len(exams) == 0:
+                await self.query_one(".exams-container").mount(Static("❌ No exams available!!!", id="exams-empty"))
+            else:
+                await self.query_one(".exams-container").mount(
+                    Vertical(id="exams-table"),
+                    Static("Select the checkboxes of the exams to be added:", classes="title"),
+                    Container(classes="select-exams-container"),
+                )
+                await self.query_one("#exams-table").mount(self.ViewExams(exams))
 
-        exams = wrapper.fetch_exams()
-        await self.query_one(".exams-loading").remove()
-        if len(exams) == 0:
-            await self.query_one(".reservations-container").mount(Static("No exams available !!!", id="exams-empty"))
-        else:
-            await self.query_one(".reservations-container").mount(
-                Vertical(id="exams-table"),
-                Static("Select the checkboxes of the exams to be added:", classes="title"),
-                Container(classes="reservations-buttons"),
-            )
-            await self.query_one("#exams-table").mount(self.Tables(exams))
-            for index, exam in enumerate(exams, start=1):
-                await self.query_one(".reservations-buttons").mount(self.Line(exam))
-            await self.query_one(".reservations-container").mount(Horizontal(Button("book", id="add")))
+                for exam in exams:
+                    await self.query_one(".select-exams-container").mount(self.SelectExams(exam))
 
+                await self.query_one(".exams-container").mount(Horizontal(Button("book", id="add")))
 
     async def on_mount(self) -> None:
         await asyncio.sleep(0.1)
         asyncio.create_task(self.fetch_date())
 
     def compose(self) -> ComposeResult:
         yield Header("Exams", classes="header")
         yield Container(Static("List of available exams:", classes="title"),
                         Static("loading [yellow]available exams[/] in progress.....", classes="exams-loading"),
-                        classes="reservations-container"
+                        classes="exams-container"
                         )
         yield Footer()
 
     class Add(Screen):
 
         def __init__(self, exams) -> None:
             self.exams = exams
@@ -128,15 +126,15 @@
                         f"\n[bold]click saved: [blue]{click}", id="exams-added-success"))
 
         async def on_mount(self) -> None:
             await asyncio.sleep(0.1)
             asyncio.create_task(self.fetch_date())
 
         def compose(self) -> ComposeResult:
-            yield Header("Exam added", classes="header")
+            yield Header("Result", classes="header")
             yield Container(Static("adding [yellow]reservations[/] in progress.....", classes="exams-loading"))
             yield Footer()
 
         BINDINGS = [
             Binding(key="r", action="app.return('exams')", description="return"),
             Binding(key="h", action="app.homepage('exams')", description="homepage"),
         ]
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `esse3_student-3.4.0/esse3_student/tui/main.py` & `esse3_student-3.6.0/esse3_student/tui/main.py`

 * *Files identical despite different names*

### Comparing `esse3_student-3.4.0/esse3_student/tui/reservations.py` & `esse3_student-3.6.0/esse3_student/tui/reservations.py`

 * *Files 10% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 class Header(Static):
     pass
 
 
 class Reservations(Screen):
 
-    class Tables(Static):
+    class ViewReservations(Static):
 
         def __init__(self, reservation, index: int) -> None:
             self.reservation = reservation
             self.index = index
             super().__init__()
 
         def table(self, reservation, index: int):
@@ -42,15 +42,15 @@
             row = list(reservation.values())
             table.add_row(str(index), *row)
             self.update(table)
 
         def on_mount(self) -> None:
             self.table(self.reservation, self.index)
 
-    class Line(Horizontal):
+    class SelectExams(Horizontal):
 
         def __init__(self, reservation) -> None:
             self.values = list(reservation.values())
             super().__init__()
 
         def on_mount(self) -> None:
             self.mount(self.Name(self.values[0]))
@@ -74,52 +74,50 @@
                 self.id = self.name_value
 
     BINDINGS = [
         Binding(key="r", action="app.pop_screen", description="return"),
     ]
 
     async def fetch_date(self) -> None:
-        """reservations = [{"name": "TRAINING", "Date": "10/12/2022  09:00", "Appello": "appello sessione straordinaria", "Numero Iscrizione": "15 su 22", "Svolgimento Esame": "Esame in Presenza",
-                          "Docenti": "PERRI SIMONA RICCA FRANCESCO", "Cancella Prenotazione": "Impossibile cancellare l'iscrizione: iscrizione chiusa"},
-                        {"name": "PROCESS MINING", "Date": "24/01/2023  09:00", "Appello": "First Exam session", "Numero Iscrizione": "19 su 23", "Svolgimento Esame": "Esame in Presenza",
-                         "Edificio": "Cubo 30B", "Aula": "MT6", "Docenti": "FIONDA VALERIA", "Cancella Prenotazione": "Impossibile cancellare l'iscrizione: iscrizione chiusa"},
-                        {"name": "CYBER OFFENSE AND DEFENSE", "Date": "31/01/2023  09:00", "Appello": "Scritto, discussione ed eventuale orale", "Numero Iscrizione": "1 su 8", "Svolgimento Esame": "Esame in Presenza",
-                         "Docenti": "ALVIANO MARIO"},
-                       ]"""
-        global wrapper
+
+        wrapper = None
+
         try:
             wrapper = cli.new_esse3_wrapper()
         except:
             await self.query_one(".reservations-loading").remove()
-            await self.query_one(".reservations-container").mount(Static("Login failed !!!", classes="login-failed"))
+            await self.query_one(".exams-container").mount(Static("Login failed !!!", classes="login-failed"))
+
+        if wrapper:
+
+            reservations = wrapper.fetch_reservations()
+            await self.query_one(".reservations-loading").remove()
 
-        reservations = wrapper.fetch_reservations()
-        await self.query_one(".reservations-loading").remove()
-        if len(reservations) == 0:
-            await self.query_one(".reservations-container").mount(Static(f"❌ No appeals booked !!", classes="reservations-empty"))
-        else:
-            await self.query_one(".reservations-container").mount(
-                Vertical(classes="reservations-table"),
-                Static("Select the checkboxes of the exams to be removed:", classes="title"),
-                Container(classes="reservations-buttons"),
-            )
-            for index, reservation in enumerate(reservations, start=1):
-                self.query_one(Vertical).mount(self.Tables(reservation, index))
-                await self.query_one(".reservations-buttons").mount(self.Line(reservation))
-            await self.query_one(".reservations-container").mount(Horizontal(Button("remove", id="remove")))
+            if len(reservations) == 0:
+                await self.query_one(".exams-container").mount(Static(f"❌ No appeals booked !!", classes="reservations-empty"))
+            else:
+                await self.query_one(".exams-container").mount(
+                    Vertical(classes="reservations-table"),
+                    Static("Select the checkboxes of the exams to be removed:", classes="title"),
+                    Container(classes="select-exams-container"),
+                )
+                for index, reservation in enumerate(reservations, start=1):
+                    self.query_one(Vertical).mount(self.ViewReservations(reservation, index))
+                    await self.query_one(".select-exams-container").mount(self.SelectExams(reservation))
+                await self.query_one(".exams-container").mount(Horizontal(Button("remove", id="remove")))
 
     async def on_mount(self) -> None:
         await asyncio.sleep(0.1)
         asyncio.create_task(self.fetch_date())
 
     def compose(self) -> ComposeResult:
         yield Header("Reservations", classes="header")
         yield Container(Static("List of Reservations:", classes="title"),
                         Static("loading [yellow]reservations[/] in progress.....", classes="reservations-loading"),
-                        classes="reservations-container")
+                        classes="exams-container")
         yield Footer()
 
     class Remove(Screen):
 
         def __init__(self, reservations) -> None:
             self.reservations = reservations
             super().__init__()
```

### Comparing `esse3_student-3.4.0/esse3_student/tui/style.css` & `esse3_student-3.6.0/esse3_student/tui/style.css`

 * *Files 4% similar despite different names*

```diff
@@ -51,33 +51,33 @@
 
 #homepage > Vertical > Button:hover {
     background: #2d4156;
 }
 
 /* BOOKLET */
 
-#booklet-container > Vertical > Tables{
+#booklet-container > Vertical > ViewExams{
     content-align: center middle;
     border: #ec971f;
     width: 100%;
     height: auto;
 }
 
-#booklet-container > NewAverage{
+#booklet-container > PlanAverage{
     content-align: center middle;
 }
 
 .booklet-container-options{
     height: auto;
     layout: horizontal;
     align: center middle;
     border: #ec971f;
 }
 
-.booklet-container-options > Average {
+.booklet-container-options > ActualAverage {
     width: auto;
 }
 
 .booklet-container-options > Button{
     margin-left: 1;
     margin-top: 2;
     border: tall #1d2e38;
@@ -118,15 +118,14 @@
     border: #2b542c;
 }
 
 .booklet-container-filters > Average {
     width: auto;
 }
 
-
 .booklet-container-filters > Static {
     width: auto;
     height: auto;
     border: blank;
 }
 
 .booklet-container-filters > Input {
@@ -155,35 +154,14 @@
 }
 
 #result {
     margin-left: 2;
     border: none;
 }
 
-/*
-#booklet-filters{
-    align: center middle;
-    width: auto;
-}
-
-#booklet-filters > Input{
-    width: 10%;
-}
-
-#booklet-filters > Button{
-    margin-left: 3;
-    border: tall #1d2e38;
-    width: auto;
-    background: $primary-background-darken-2;
-}
-
-#booklet-filters > Button:hover {
-    background: #2d4156;
-}
-*/
 #booklet-table-exams{
     content-align: center middle;
     border: heavy #2b542c;
     width: 100%;
     height: auto;
 }
 
@@ -229,17 +207,14 @@
     width: 20%;
     height: auto;
 }
 
 
 /* TAXES */
 
-#taxes-container {
-}
-
 #taxes-table{
     content-align: center middle;
     border: #ec971f;
     width: 100%;
     height: auto;
 }
 
@@ -247,31 +222,23 @@
     width: 100%;
     height: 1fr;
     border: double #ec971f;
     content-align: center middle;
     text-style: bold italic;
 }
 
-/*
-.click-saved {
-    width: 100%;
-    height: auto;
-    border: red;
-    content-align: center middle;
-}
-*/
 /* EXAMS */
 
 #exams-table {
     border: #ec971f;
     width: 100%;
     height: auto;
 }
 
-#exams-table > Tables {
+#exams-table > ViewExams {
     content-align: center middle;
     /* height: auto; questo qua fa in modo che rimpicciolendo lo schermo poi mi esce la scrollbar, senza invece si adatta*/
 }
 
 #add {
     border: tall #1d2e38;
     width: 30%;
@@ -309,60 +276,21 @@
 /* RESERVATIONS */
 
 .reservations-table{
     height: 40%;
     border: #ec971f;
 }
 
-.reservations-table > Tables {
+.reservations-table > ViewReservations {
     content-align: center middle;
     border: none;
     width: 100%;
     height: auto;
 }
 
-.reservations-buttons{
-    margin-top: 1;
-    layout: horizontal;
-    height: auto;
-    align: center middle;
-    scrollbar-color: #f7ecb5;
-    scrollbar-size: 1 2;
-}
-
-.reservations-buttons > Line  {
-    border: #ec971f;
-    align: center middle;
-    height: auto;
-    width: auto;
-}
-
-.reservations-buttons  > Line > Static {
-    width: auto;
-    height: auto;
-    text-style: bold;
-    border: $background;
-}
-
-.reservations-buttons  > Line > Check {
-    width: auto;
-    height: auto;
-}
-
-.reservations-buttons  > Line > Check:hover {
-    background: #2d4156;
-}
-
-.reservations-container > Horizontal {
-    margin-top: 1;
-    align: center middle;
-    height: auto;
-    width: 100%;
-}
-
 #remove {
     border: tall #1d2e38;
     width: 30%;
     background: $primary-background-darken-2;
 }
 
 #remove:hover {
@@ -413,14 +341,55 @@
     width: 100%;
     height: 1fr;
     border: heavy #2b542c;
     content-align: center middle;
     text-style: bold italic;
 }
 
+/* EXAMS & RESERVATIONS */
+
+.exams-container > Horizontal {
+    margin-top: 1;
+    align: center middle;
+    height: auto;
+    width: 100%;
+}
+
+.select-exams-container{
+    margin-top: 1;
+    layout: horizontal;
+    height: auto;
+    align: center middle;
+    scrollbar-color: #f7ecb5;
+    scrollbar-size: 1 2;
+}
+
+.select-exams-container > SelectExams {
+    border: #ec971f;
+    align: center middle;
+    height: auto;
+    width: auto;
+}
+
+.select-exams-container  > SelectExams > Static {
+    width: auto;
+    height: auto;
+    text-style: bold;
+    border: $background;
+}
+
+.select-exams-container  > SelectExams > Check {
+    width: auto;
+    height: auto;
+}
+
+.select-exams-container  > SelectExams > Check:hover {
+    background: #2d4156;
+}
+
 /* FOOTER */
 Footer {
     background: $background;
 }
```

### Comparing `esse3_student-3.4.0/esse3_student/tui/taxes.py` & `esse3_student-3.6.0/esse3_student/tui/taxes.py`

 * *Files 9% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 class Header(Static):
     pass
 
 
 class Taxes(Screen):
 
-    class Tables(Static):
+    class Viewtaxes(Static):
 
         def __init__(self, taxes) -> None:
             self.taxes = taxes
             super().__init__()
 
         def on_mount(self) -> None:
             self.id = "taxes-table"
@@ -51,28 +51,30 @@
                 amount, payment = self.payment_changes(amount, status)
                 table.add_row(str(index), id, date, amount, payment)
 
             self.update(table)
 
     async def fetch_date(self) -> None:
 
-        global wrapper
+        wrapper = None
+
         try:
             wrapper = cli.new_esse3_wrapper()
         except:
             await self.query_one("#taxes-loading").remove()
             await self.query_one(Container).mount(Static("Login failed !!!", classes="login-failed"))
 
-        taxes, statistics = wrapper.fetch_taxes()
-        await self.query_one("#taxes-loading").remove()
-        self.query_one(Container).mount(
-            Vertical(
-                self.Tables(taxes),
+        if wrapper:
+            taxes, statistics = wrapper.fetch_taxes()
+            await self.query_one("#taxes-loading").remove()
+            self.query_one(Container).mount(
+                Vertical(
+                    self.Viewtaxes(taxes),
+                )
             )
-        )
 
     async def on_mount(self) -> None:
         await asyncio.sleep(0.1)
         asyncio.create_task(self.fetch_date())
 
     def compose(self) -> ComposeResult:
         yield Header("Taxes", classes="header")
```

### Comparing `esse3_student-3.4.0/esse3_student/utils/primitives.py` & `esse3_student-3.6.0/esse3_student/utils/primitives.py`

 * *Files identical despite different names*

### Comparing `esse3_student-3.4.0/esse3_student/utils/validators.py` & `esse3_student-3.6.0/esse3_student/utils/validators.py`

 * *Files identical despite different names*

### Comparing `esse3_student-3.4.0/pyproject.toml` & `esse3_student-3.6.0/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "esse3-student"
-version = "3.4.0"
+version = "3.6.0"
 description = "Esse3 command line utility"
 authors = ["Antonio Pallaria <pallaria98@gmail.com>"]
 
 [tool.poetry.dependencies]
 python = "^3.9"
 xdotool = { version = "^0.4.0", python = ">=3.10,<4.0" }
 typer = "^0.6.1"
```

### Comparing `esse3_student-3.4.0/setup.py` & `esse3_student-3.6.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,15 @@
  'webdriver-manager>=3.8.3,<4.0.0']
 
 extras_require = \
 {':python_version >= "3.10" and python_version < "4.0"': ['xdotool>=0.4.0,<0.5.0']}
 
 setup_kwargs = {
     'name': 'esse3-student',
-    'version': '3.4.0',
+    'version': '3.6.0',
     'description': 'Esse3 command line utility',
     'long_description': 'None',
     'author': 'Antonio Pallaria',
     'author_email': 'pallaria98@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `esse3_student-3.4.0/PKG-INFO` & `esse3_student-3.6.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: esse3-student
-Version: 3.4.0
+Version: 3.6.0
 Summary: Esse3 command line utility
 Author: Antonio Pallaria
 Author-email: pallaria98@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

