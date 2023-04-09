# Comparing `tmp/eAwaiter-0.0.1.tar.gz` & `tmp/eAwaiter-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eAwaiter-0.0.1.tar", last modified: Thu Mar 23 16:46:20 2023, max compression
+gzip compressed data, was "eAwaiter-0.0.2.tar", last modified: Sun Apr  9 12:06:05 2023, max compression
```

## Comparing `eAwaiter-0.0.1.tar` & `eAwaiter-0.0.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 skrci     (1000) skrci     (1000)        0 2023-03-23 16:46:20.746296 eAwaiter-0.0.1/
--rw-r--r--   0 skrci     (1000) skrci     (1000)     1062 2023-03-23 13:33:26.000000 eAwaiter-0.0.1/LICENSE
--rw-r--r--   0 skrci     (1000) skrci     (1000)     2270 2023-03-23 16:46:20.746296 eAwaiter-0.0.1/PKG-INFO
--rw-r--r--   0 skrci     (1000) skrci     (1000)     1818 2023-03-12 22:52:55.000000 eAwaiter-0.0.1/README.md
-drwxr-xr-x   0 skrci     (1000) skrci     (1000)        0 2023-03-23 16:46:20.746296 eAwaiter-0.0.1/eAwaiter.egg-info/
--rw-r--r--   0 skrci     (1000) skrci     (1000)     2270 2023-03-23 16:46:20.000000 eAwaiter-0.0.1/eAwaiter.egg-info/PKG-INFO
--rw-r--r--   0 skrci     (1000) skrci     (1000)      331 2023-03-23 16:46:20.000000 eAwaiter-0.0.1/eAwaiter.egg-info/SOURCES.txt
--rw-r--r--   0 skrci     (1000) skrci     (1000)        1 2023-03-23 16:46:20.000000 eAwaiter-0.0.1/eAwaiter.egg-info/dependency_links.txt
--rw-r--r--   0 skrci     (1000) skrci     (1000)       40 2023-03-23 16:46:20.000000 eAwaiter-0.0.1/eAwaiter.egg-info/requires.txt
--rw-r--r--   0 skrci     (1000) skrci     (1000)        7 2023-03-23 16:46:20.000000 eAwaiter-0.0.1/eAwaiter.egg-info/top_level.txt
--rw-r--r--   0 skrci     (1000) skrci     (1000)      100 2023-03-23 14:29:52.000000 eAwaiter-0.0.1/pyproject.toml
--rw-r--r--   0 skrci     (1000) skrci     (1000)      576 2023-03-23 16:46:20.749629 eAwaiter-0.0.1/setup.cfg
--rw-r--r--   0 skrci     (1000) skrci     (1000)       70 2023-03-23 14:24:15.000000 eAwaiter-0.0.1/setup.py
-drwxr-xr-x   0 skrci     (1000) skrci     (1000)        0 2023-03-23 16:46:20.746296 eAwaiter-0.0.1/waiter/
--rw-r--r--   0 skrci     (1000) skrci     (1000)       13 2023-03-13 17:05:32.000000 eAwaiter-0.0.1/waiter/__init__.py
--rw-r--r--   0 skrci     (1000) skrci     (1000)     6532 2023-03-23 12:39:42.000000 eAwaiter-0.0.1/waiter/api_navigator.py
--rw-r--r--   0 skrci     (1000) skrci     (1000)      666 2023-03-20 15:14:59.000000 eAwaiter-0.0.1/waiter/dataclasses.py
--rw-r--r--   0 skrci     (1000) skrci     (1000)      390 2023-03-13 17:10:11.000000 eAwaiter-0.0.1/waiter/exceptions.py
--rw-r--r--   0 skrci     (1000) skrci     (1000)     1657 2023-03-20 15:28:18.000000 eAwaiter-0.0.1/waiter/helpers.py
--rw-r--r--   0 skrci     (1000) skrci     (1000)     7943 2023-03-23 13:25:26.000000 eAwaiter-0.0.1/waiter/waiter.py
+drwxr-xr-x   0 skrci     (1000) skrci     (1000)        0 2023-04-09 12:06:05.977946 eAwaiter-0.0.2/
+-rw-r--r--   0 skrci     (1000) skrci     (1000)     1062 2023-03-23 13:33:26.000000 eAwaiter-0.0.2/LICENSE
+-rw-r--r--   0 skrci     (1000) skrci     (1000)     2931 2023-04-09 12:06:05.977946 eAwaiter-0.0.2/PKG-INFO
+-rw-r--r--   0 skrci     (1000) skrci     (1000)     2479 2023-04-06 14:27:23.000000 eAwaiter-0.0.2/README.md
+drwxr-xr-x   0 skrci     (1000) skrci     (1000)        0 2023-04-09 12:06:05.977946 eAwaiter-0.0.2/eAwaiter.egg-info/
+-rw-r--r--   0 skrci     (1000) skrci     (1000)     2931 2023-04-09 12:06:05.000000 eAwaiter-0.0.2/eAwaiter.egg-info/PKG-INFO
+-rw-r--r--   0 skrci     (1000) skrci     (1000)      331 2023-04-09 12:06:05.000000 eAwaiter-0.0.2/eAwaiter.egg-info/SOURCES.txt
+-rw-r--r--   0 skrci     (1000) skrci     (1000)        1 2023-04-09 12:06:05.000000 eAwaiter-0.0.2/eAwaiter.egg-info/dependency_links.txt
+-rw-r--r--   0 skrci     (1000) skrci     (1000)       40 2023-04-09 12:06:05.000000 eAwaiter-0.0.2/eAwaiter.egg-info/requires.txt
+-rw-r--r--   0 skrci     (1000) skrci     (1000)        7 2023-04-09 12:06:05.000000 eAwaiter-0.0.2/eAwaiter.egg-info/top_level.txt
+-rw-r--r--   0 skrci     (1000) skrci     (1000)      100 2023-03-23 14:29:52.000000 eAwaiter-0.0.2/pyproject.toml
+-rw-r--r--   0 skrci     (1000) skrci     (1000)      576 2023-04-09 12:06:05.977946 eAwaiter-0.0.2/setup.cfg
+-rw-r--r--   0 skrci     (1000) skrci     (1000)       70 2023-03-23 14:24:15.000000 eAwaiter-0.0.2/setup.py
+drwxr-xr-x   0 skrci     (1000) skrci     (1000)        0 2023-04-09 12:06:05.977946 eAwaiter-0.0.2/waiter/
+-rw-r--r--   0 skrci     (1000) skrci     (1000)       13 2023-03-13 17:05:32.000000 eAwaiter-0.0.2/waiter/__init__.py
+-rw-r--r--   0 skrci     (1000) skrci     (1000)     6517 2023-03-26 10:04:06.000000 eAwaiter-0.0.2/waiter/api_navigator.py
+-rw-r--r--   0 skrci     (1000) skrci     (1000)     1510 2023-03-26 10:03:56.000000 eAwaiter-0.0.2/waiter/dataclasses.py
+-rw-r--r--   0 skrci     (1000) skrci     (1000)      390 2023-03-13 17:10:11.000000 eAwaiter-0.0.2/waiter/exceptions.py
+-rw-r--r--   0 skrci     (1000) skrci     (1000)     1650 2023-03-26 10:04:19.000000 eAwaiter-0.0.2/waiter/helpers.py
+-rw-r--r--   0 skrci     (1000) skrci     (1000)     8392 2023-04-07 22:04:12.000000 eAwaiter-0.0.2/waiter/waiter.py
```

### Comparing `eAwaiter-0.0.1/LICENSE` & `eAwaiter-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `eAwaiter-0.0.1/PKG-INFO` & `eAwaiter-0.0.2/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,27 +1,30 @@
 Metadata-Version: 2.1
 Name: eAwaiter
-Version: 0.0.1
+Version: 0.0.2
 Summary: Package to manage your eAsistent meals automatically.
 Home-page: https://github.com/5KRC1/eAwaiter
 Author: 5krc1
 Author-email: skrci@dasadweb.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
+![eAwaiter banner](https://github.com/5KRC1/5KRC1/blob/main/images/eAwaiter/eAwaiter-banner.png "eAwaiter banner")
 # eAwaiter
 eAwaiter is a Python package that can change your eAsistent meals automatically.
 
 ## Description
-eAwaiter was made out of pure laziness of mine. In eAsistent, meals can be changed a week in advance, but since I rarely use the app I forget to see if what I am subscribed to is enjoyable. Due to this I've created this package that (given the necessary information) changes the meals according to your preferances.
+eAwaiter is supposed to help with changing meals in eAsistent. Meals are "changable" only 7 days in advance. Therefore, waiter's service looks for any disliked foods and favourite foods and changes meals few weeks in future. I can also help manually changing meals and more.
+
+eAwaiter's service (and more) is used in [eAmenu](https://github.com/5KRC1/eAmenu) android app.
 
 ## Install & Run
 If you are changing the code or using it locally, you can easily install and run it with the following commands:
 - Clone the project
 ```bash
 git clone https://github.com/5KRC1/eAwaiter && cd eAmenu
 ```
@@ -35,39 +38,87 @@
 ```
 - Run the example provided under "Usage"
 ```bash
 python examples/example.py
 ```
 
 ## Usage
-To use the package, you simply follow the following instructions:
-- install with pip
+install with pip
 ```bash
 pip install git+https://github.com/5KRC1/eAwaiter.git
 ```
-- run in python "example.py"
+
+examples:
+- service
 ```python
-## example.py ##
 from waiter.waiter import Waiter
 
-waiter = Waiter()
-
-# Login
-waiter.username = "__your_username__"   # use your eAsistent username
-waiter.password = "__your_password__"   # use your eAsistent password
-waiter.login()
-
-# Provide info
-waiter.default_menu = "1"    # str | any of numbers from 1-6 (eAsistent menus)
-waiter.preferred_menu = "2"  # str | any of numbers from 1-6 (eAsistent menus)
-waiter.favourite_foods = ["pica", "špageti"] # array of str | foods must be exatly spelled as in eAsistent
-waiter.disliked_foods = ["Cheder", "hrenovko", "osličev", "oslič"]  # array of str | foods must be exatly spelled as in eAsistent
+# Init Waiter
+username = "__your_username__"
+password = "__your_password__"
+
+default_menu = "1"
+preferred_menu = "2"
+favourite_foods = ["pica", "špageti"]
+disliked_foods = ["Cheder", "hrenovko", "osličev", "oslič"]
+overwrite = False
+
+waiter = Waiter(
+  username=username,
+  password=password,
+  default_menu=default_menu,
+  favourite_foods=favourite_foods,
+  disliked_foods=disliked_foods,
+  preferred_menu=preferred_menu,
+  orevwrite_unchangable=overwrite
+)
 
 # Run service
 waiter.service()
 ```
 
-## Contribute
+- get meals
+```python
+from waiter.waiter import Waiter
+
+# Init Waiter
+username = "__your_username__"
+password = "__your_password__"
 
-## To Do
-- document eAsistent API
-- Clean up code
+waiter = Waiter(
+  username=username,
+  password=password
+)
+
+# Get meals
+meals = waiter.get_meals()
+```
+
+- change a meal
+```python
+from datetime import datetime
+from waiter.waiter import Waiter
+
+# Init Waiter
+username = "__your_username__"
+password = "__your_password__"
+
+waiter = Waiter(
+  username=username,
+  password=password
+)
+
+action = "prijava"
+meal_id = "__meal_id__"
+date = datetime(2023, 3, 29)  # (year, month, day)
+
+# Change a meal
+changed = waiter.prijava_odjava(
+  action=action,
+  meal_id=meal_id,
+  date=date
+)
+```
+
+For more information check out the documentation [here](https://dasadweb.com/documentation/eAwaiter).
+
+## Contribute
```

### Comparing `eAwaiter-0.0.1/eAwaiter.egg-info/PKG-INFO` & `eAwaiter-0.0.2/eAwaiter.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,27 +1,30 @@
 Metadata-Version: 2.1
 Name: eAwaiter
-Version: 0.0.1
+Version: 0.0.2
 Summary: Package to manage your eAsistent meals automatically.
 Home-page: https://github.com/5KRC1/eAwaiter
 Author: 5krc1
 Author-email: skrci@dasadweb.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
+![eAwaiter banner](https://github.com/5KRC1/5KRC1/blob/main/images/eAwaiter/eAwaiter-banner.png "eAwaiter banner")
 # eAwaiter
 eAwaiter is a Python package that can change your eAsistent meals automatically.
 
 ## Description
-eAwaiter was made out of pure laziness of mine. In eAsistent, meals can be changed a week in advance, but since I rarely use the app I forget to see if what I am subscribed to is enjoyable. Due to this I've created this package that (given the necessary information) changes the meals according to your preferances.
+eAwaiter is supposed to help with changing meals in eAsistent. Meals are "changable" only 7 days in advance. Therefore, waiter's service looks for any disliked foods and favourite foods and changes meals few weeks in future. I can also help manually changing meals and more.
+
+eAwaiter's service (and more) is used in [eAmenu](https://github.com/5KRC1/eAmenu) android app.
 
 ## Install & Run
 If you are changing the code or using it locally, you can easily install and run it with the following commands:
 - Clone the project
 ```bash
 git clone https://github.com/5KRC1/eAwaiter && cd eAmenu
 ```
@@ -35,39 +38,87 @@
 ```
 - Run the example provided under "Usage"
 ```bash
 python examples/example.py
 ```
 
 ## Usage
-To use the package, you simply follow the following instructions:
-- install with pip
+install with pip
 ```bash
 pip install git+https://github.com/5KRC1/eAwaiter.git
 ```
-- run in python "example.py"
+
+examples:
+- service
 ```python
-## example.py ##
 from waiter.waiter import Waiter
 
-waiter = Waiter()
-
-# Login
-waiter.username = "__your_username__"   # use your eAsistent username
-waiter.password = "__your_password__"   # use your eAsistent password
-waiter.login()
-
-# Provide info
-waiter.default_menu = "1"    # str | any of numbers from 1-6 (eAsistent menus)
-waiter.preferred_menu = "2"  # str | any of numbers from 1-6 (eAsistent menus)
-waiter.favourite_foods = ["pica", "špageti"] # array of str | foods must be exatly spelled as in eAsistent
-waiter.disliked_foods = ["Cheder", "hrenovko", "osličev", "oslič"]  # array of str | foods must be exatly spelled as in eAsistent
+# Init Waiter
+username = "__your_username__"
+password = "__your_password__"
+
+default_menu = "1"
+preferred_menu = "2"
+favourite_foods = ["pica", "špageti"]
+disliked_foods = ["Cheder", "hrenovko", "osličev", "oslič"]
+overwrite = False
+
+waiter = Waiter(
+  username=username,
+  password=password,
+  default_menu=default_menu,
+  favourite_foods=favourite_foods,
+  disliked_foods=disliked_foods,
+  preferred_menu=preferred_menu,
+  orevwrite_unchangable=overwrite
+)
 
 # Run service
 waiter.service()
 ```
 
-## Contribute
+- get meals
+```python
+from waiter.waiter import Waiter
+
+# Init Waiter
+username = "__your_username__"
+password = "__your_password__"
 
-## To Do
-- document eAsistent API
-- Clean up code
+waiter = Waiter(
+  username=username,
+  password=password
+)
+
+# Get meals
+meals = waiter.get_meals()
+```
+
+- change a meal
+```python
+from datetime import datetime
+from waiter.waiter import Waiter
+
+# Init Waiter
+username = "__your_username__"
+password = "__your_password__"
+
+waiter = Waiter(
+  username=username,
+  password=password
+)
+
+action = "prijava"
+meal_id = "__meal_id__"
+date = datetime(2023, 3, 29)  # (year, month, day)
+
+# Change a meal
+changed = waiter.prijava_odjava(
+  action=action,
+  meal_id=meal_id,
+  date=date
+)
+```
+
+For more information check out the documentation [here](https://dasadweb.com/documentation/eAwaiter).
+
+## Contribute
```

### Comparing `eAwaiter-0.0.1/setup.cfg` & `eAwaiter-0.0.2/setup.cfg`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = eAwaiter
-version = 0.0.1
+version = 0.0.2
 author = 5krc1
 author_email = skrci@dasadweb.com
 description = Package to manage your eAsistent meals automatically.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/5KRC1/eAwaiter
 license = MIT
```

### Comparing `eAwaiter-0.0.1/waiter/api_navigator.py` & `eAwaiter-0.0.2/waiter/api_navigator.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """
 API Navigation
 ==============
 
 API Navigation is made to purely interact with the api and scrape the meal off the web.
 For examples and in depth usage, take a look at our documentation.
-<https://dasadweb.com/documentation/eAwaiter#API-Navigation>
+<https://dasadweb.com/documentation/eAwaiter>
 """
 
 from bs4 import BeautifulSoup
 from bs4.element import Tag
 
 from datetime import datetime, timedelta
 import requests
```

### Comparing `eAwaiter-0.0.1/waiter/helpers.py` & `eAwaiter-0.0.2/waiter/helpers.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """
 Helpers
 =======
 
 Helpers are different functions that just don't belong in any of the classes.
 For examples and in depth usage, take a look at our documentation.
-<https://dasadweb.com/documentation/eAwaiter#Waiter>
+<https://dasadweb.com/documentation/eAwaiter>
 """
 
 from datetime import datetime, timedelta
 
 
 def weeks_in_advance(weeks: int, first_week_school: datetime) -> [int, datetime]:
     today = datetime.now()
```

### Comparing `eAwaiter-0.0.1/waiter/waiter.py` & `eAwaiter-0.0.2/waiter/waiter.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """
 Waiter
 ======
 
 Waiter class is used for easy interaction with the user.
 For examples and in depth usage, take a look at our documentation.
-<https://dasadweb.com/documentation/eAwaiter#Waiter>
+<https://dasadweb.com/documentation/eAwaiter>
 """
 
 from bs4 import BeautifulSoup
 
 from datetime import datetime, timedelta
 import json
 import os
@@ -88,23 +88,25 @@
     
     def prijava_odjava(self, action: str, meal_id: str, date: str):
         result = self.api.prijava_odjava(
             action,
             meal_id,
             date
             )
+        print(result.json())
         if not result.json()["status"]:
+            # automatically won't work if 7 days from today
             result = self.api.prijava_odjava(
                 "odjava",
                 meal_id,
                 date
                 )
         return True if result.json()["status"] else False
 
-    def change_disliked(self, week: int) -> list:
+    def change_disliked(self, week: int, count: int=1) -> list:
         changes = []
         next_week_num, monday = weeks_in_advance(week, self.first_week_school)
         meals_data = get_selected(
             self.api.get_meal_data(next_week_num, monday, self.meals)
         )
 
         check_odjava = False
@@ -113,14 +115,17 @@
         selected_menu = self.meals[int(self.user.preferred_menu) - 1]
 
         for meal_data in meals_data:
             for disliked_food in self.user.disliked_foods:
                 if not meal_data.changable and not self.user.overwrite_unchangable:
                     break
                 if disliked_food.upper() in meal_data.meal_text:
+                    if meal_data.meal_id == selected_menu:
+                        check_odjava = True
+                        break
                     if check_odjava: 
                         self.api.prijava_odjava(
                             "odjava", meal_data.meal_id, meal_data.date
                         )
                         changes.append(f"Meal changed for {meal_data.date} (sigend off)!")
                         break
 
@@ -131,19 +136,22 @@
                     if not response.json()["status"]:
                         response = self.api.prijava_odjava(
                             "odjava", meal_data.meal_id, meal_data.date
                         )
                         change = f"Meal signed off for {meal_data.date}!"
                     changes.append(change)
                     break
+        if count < 2:
+            count += 1
+            self.change_disliked(week, count)
         return changes
 
-    def change_favourites(self) -> list:
+    def change_favourites(self, week: int) -> list:
         changes = []
-        next_week_num, monday = weeks_in_advance(2, self.first_week_school)
+        next_week_num, monday = weeks_in_advance(week, self.first_week_school)
         meals_data = self.api.get_meal_data(next_week_num, monday, self.meals)
 
         check_odjava = False
         if int(self.user.default_menu) == 0:
             check_odjava = True
         selected_menu = self.meals[int(self.user.default_menu) - 1]
 
@@ -168,23 +176,23 @@
                         break
                 if is_subbed:
                     break
             if is_subbed:
                 continue
             if check_odjava:
                 response = self.api.prijava_odjava(
-                    "odjava", meal_data[i][0].meal_id, meals_data[i][0].date
+                    "odjava", meals_data[i][0].meal_id, meals_data[i][0].date
                 )
                 continue
             response = self.api.prijava_odjava(
                 "prijava", selected_menu, meals_data[i][0].date
             )
             if not response.json()["status"]:
                 response = self.api.prijava_odjava(
-                    "odjava", meal_data[i][0].meal_id, meals_data[i][0].date
+                    "odjava", meals_data[i][0].meal_id, meals_data[i][0].date
                 )
         return changes
 
     def get_meals(self, week_num: int = 0, date: datetime = datetime.today()) -> list:
         if week_num:
             print(week_num)
             date = get_monday(self.first_week_school + timedelta(days=7*week_num))
@@ -200,19 +208,22 @@
         if self.failed_login:
             raise UserLoginException("Failed to login!")
 
         try:
             if not self.meals:
                 raise MealFetchingException("No meals' ids!")
 
+            if self.user.favourite_foods:
+                changes += self.change_favourites(1)
+
             if self.user.disliked_foods and self.user.preferred_menu:
                 changes += self.change_disliked(1)
-
+                
             if self.user.favourite_foods and self.user.default_menu:
-                changes += self.change_favourites()
+                changes += self.change_favourites(2)
 
             if self.user.disliked_foods:
                 changes += self.change_disliked(2)
 
             self.api.send_mail("service did well")
 
         except Exception as e:
```

