# Comparing `tmp/rozklad_ontu_parser_makisukurisu-0.0.2.6.tar.gz` & `tmp/rozklad_ontu_parser_makisukurisu-0.0.3.tar.gz`

## Comparing `rozklad_ontu_parser_makisukurisu-0.0.2.6.tar` & `rozklad_ontu_parser_makisukurisu-0.0.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 rozklad_ontu_parser_makisukurisu-0.0.2.6/requirements.txt
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 rozklad_ontu_parser_makisukurisu-0.0.2.6/run_lint.bat
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 rozklad_ontu_parser_makisukurisu-0.0.2.6/run_lint.sh
--rw-r--r--   0        0        0      611 2020-02-02 00:00:00.000000 rozklad_ontu_parser_makisukurisu-0.0.2.6/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0        0        0      592 2020-02-02 00:00:00.000000 rozklad_ontu_parser_makisukurisu-0.0.2.6/.github/workflows/pylint.yml
--rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 rozklad_ontu_parser_makisukurisu-0.0.2.6/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 rozklad_ontu_parser_makisukurisu-0.0.2.6/ontu_parser/__init__.py
--rw-r--r--   0        0        0      950 2020-02-02 00:00:00.000000 rozklad_ontu_parser_makisukurisu-0.0.2.6/ontu_parser/example.py
--rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 rozklad_ontu_parser_makisukurisu-0.0.2.6/ontu_parser/classes/__init__.py
--rw-r--r--   0        0        0     2743 2020-02-02 00:00:00.000000 rozklad_ontu_parser_makisukurisu-0.0.2.6/ontu_parser/classes/base.py
--rw-r--r--   0        0        0    13965 2020-02-02 00:00:00.000000 rozklad_ontu_parser_makisukurisu-0.0.2.6/ontu_parser/classes/dataclasses.py
--rw-r--r--   0        0        0      850 2020-02-02 00:00:00.000000 rozklad_ontu_parser_makisukurisu-0.0.2.6/ontu_parser/classes/enums.py
--rw-r--r--   0        0        0     4910 2020-02-02 00:00:00.000000 rozklad_ontu_parser_makisukurisu-0.0.2.6/ontu_parser/classes/parser.py
--rw-r--r--   0        0        0     5605 2020-02-02 00:00:00.000000 rozklad_ontu_parser_makisukurisu-0.0.2.6/ontu_parser/classes/sender.py
--rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 rozklad_ontu_parser_makisukurisu-0.0.2.6/.gitignore
--rw-r--r--   0        0        0     1505 2020-02-02 00:00:00.000000 rozklad_ontu_parser_makisukurisu-0.0.2.6/LICENSE
--rw-r--r--   0        0        0      811 2020-02-02 00:00:00.000000 rozklad_ontu_parser_makisukurisu-0.0.2.6/pyproject.toml
--rw-r--r--   0        0        0     2295 2020-02-02 00:00:00.000000 rozklad_ontu_parser_makisukurisu-0.0.2.6/readme.md
--rw-r--r--   0        0        0     3050 2020-02-02 00:00:00.000000 rozklad_ontu_parser_makisukurisu-0.0.2.6/PKG-INFO
+-rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 rozklad_ontu_parser_makisukurisu-0.0.3/requirements.txt
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 rozklad_ontu_parser_makisukurisu-0.0.3/run_lint.bat
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 rozklad_ontu_parser_makisukurisu-0.0.3/run_lint.sh
+-rw-r--r--   0        0        0      611 2020-02-02 00:00:00.000000 rozklad_ontu_parser_makisukurisu-0.0.3/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0      592 2020-02-02 00:00:00.000000 rozklad_ontu_parser_makisukurisu-0.0.3/.github/workflows/pylint.yml
+-rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 rozklad_ontu_parser_makisukurisu-0.0.3/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 rozklad_ontu_parser_makisukurisu-0.0.3/ontu_parser/__init__.py
+-rw-r--r--   0        0        0     1018 2020-02-02 00:00:00.000000 rozklad_ontu_parser_makisukurisu-0.0.3/ontu_parser/example.py
+-rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 rozklad_ontu_parser_makisukurisu-0.0.3/ontu_parser/classes/__init__.py
+-rw-r--r--   0        0        0     2743 2020-02-02 00:00:00.000000 rozklad_ontu_parser_makisukurisu-0.0.3/ontu_parser/classes/base.py
+-rw-r--r--   0        0        0    13351 2020-02-02 00:00:00.000000 rozklad_ontu_parser_makisukurisu-0.0.3/ontu_parser/classes/dataclasses.py
+-rw-r--r--   0        0        0      850 2020-02-02 00:00:00.000000 rozklad_ontu_parser_makisukurisu-0.0.3/ontu_parser/classes/enums.py
+-rw-r--r--   0        0        0     4910 2020-02-02 00:00:00.000000 rozklad_ontu_parser_makisukurisu-0.0.3/ontu_parser/classes/parser.py
+-rw-r--r--   0        0        0     5605 2020-02-02 00:00:00.000000 rozklad_ontu_parser_makisukurisu-0.0.3/ontu_parser/classes/sender.py
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 rozklad_ontu_parser_makisukurisu-0.0.3/.gitignore
+-rw-r--r--   0        0        0     1505 2020-02-02 00:00:00.000000 rozklad_ontu_parser_makisukurisu-0.0.3/LICENSE
+-rw-r--r--   0        0        0      809 2020-02-02 00:00:00.000000 rozklad_ontu_parser_makisukurisu-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     2295 2020-02-02 00:00:00.000000 rozklad_ontu_parser_makisukurisu-0.0.3/readme.md
+-rw-r--r--   0        0        0     3048 2020-02-02 00:00:00.000000 rozklad_ontu_parser_makisukurisu-0.0.3/PKG-INFO
```

### Comparing `rozklad_ontu_parser_makisukurisu-0.0.2.6/.github/ISSUE_TEMPLATE/feature_request.md` & `rozklad_ontu_parser_makisukurisu-0.0.3/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `rozklad_ontu_parser_makisukurisu-0.0.2.6/.github/workflows/pylint.yml` & `rozklad_ontu_parser_makisukurisu-0.0.3/.github/workflows/pylint.yml`

 * *Files identical despite different names*

### Comparing `rozklad_ontu_parser_makisukurisu-0.0.2.6/.github/workflows/python-publish.yml` & `rozklad_ontu_parser_makisukurisu-0.0.3/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `rozklad_ontu_parser_makisukurisu-0.0.2.6/ontu_parser/example.py` & `rozklad_ontu_parser_makisukurisu-0.0.3/ontu_parser/example.py`

 * *Files 6% similar despite different names*

```diff
@@ -26,10 +26,10 @@
             continue
         print(f'{pair.pair_no}:')
         for lesson in pair.lessons:
             print(
                 f'{lesson.lesson_date}: '
                 f'{lesson.teacher["short"]} - '
                 f'{lesson.lesson_name["short"]}'
+                f' - In auditorium: {lesson.auditorium}' if lesson.auditorium else ''
             )
-            print(f'Card: {lesson.lesson_info}')
-            print()
+            print(f'Card: {lesson.lesson_info}\n')
```

### Comparing `rozklad_ontu_parser_makisukurisu-0.0.2.6/ontu_parser/classes/base.py` & `rozklad_ontu_parser_makisukurisu-0.0.3/ontu_parser/classes/base.py`

 * *Files identical despite different names*

### Comparing `rozklad_ontu_parser_makisukurisu-0.0.2.6/ontu_parser/classes/dataclasses.py` & `rozklad_ontu_parser_makisukurisu-0.0.3/ontu_parser/classes/dataclasses.py`

 * *Files 4% similar despite different names*

```diff
@@ -155,14 +155,15 @@
 
     lesson_tag: Tag
 
     lesson_date: str = ""
     teacher: dict = {}
     lesson_name: dict = {}
     lesson_info: str = ""
+    auditorium: str | None = None
 
     @staticmethod
     def _check_tag(tag: Tag):
         # Dear Gods, forgive me for not checking tags for lessons
         pass
 
     def parse_tag(self):
@@ -170,94 +171,78 @@
         raise NotImplementedError(
             "`parse_tag` was not implemented\n"
             "You are probably executing this from BaseLesson\n"
             "Please use one of derived classes"
         )
 
 
-class AllTimeLesson(BaseLesson):
+class RegularLesson(BaseLesson):
     """
         This class should be used to parse lesson from bs4 tag
-        If you are getting schedule for all time
+        If you are getting schedule for current week
     """
     @classmethod
     def from_tag(cls, tag):
         obj = cls()
         obj.lesson_tag = tag
         obj.parse_tag()
         return obj
 
     def parse_tag(self):
-        lesson = self.lesson_tag
-        self.lesson_date = lesson.text
-        predm = lesson.nextSibling
-        self.lesson_name = {
-            'short': predm.text,
-            'full': predm.attrs.get('title', "Not Set")
-        }
-        prp = predm.nextSibling
-        if isinstance(prp, str):
-            # <br> may be interpreted as '\n'
-            prp = prp.nextSibling
-        self.teacher = {
-            'short': prp.text.replace('\xa0', ' '),  # Why...
-            'full': prp.attrs.get('title', "Not Set")
-        }
-        card = prp.nextSibling
-        if isinstance(card, str):
-            # <br> may be interpreted as '\n'
-            card = card.nextSibling
-        card_content: Tag = card.find(
+        lesson_top = self.lesson_tag.parent
+
+        predm_element = lesson_top.find(
+            name='span',
             attrs={
-                'class': 'card-content'
+                'class': 'predm'
             }
         )
-        if card_content:
-            self.lesson_info = card_content.text.replace('\t', '')
-
-
-class RegularLesson(BaseLesson):
-    """
-        This class should be used to parse lesson from bs4 tag
-        If you are getting schedule for current week
-    """
-    @classmethod
-    def from_tag(cls, tag):
-        obj = cls()
-        obj.lesson_tag = tag
-        obj.parse_tag()
-        return obj
-
-    def parse_tag(self):
-        lesson = self.lesson_tag
-        # I don't know why, but ok :)
-        skip = lesson.nextSibling
         self.lesson_name = {
-            'short': lesson.text,
-            'full': lesson.attrs.get('title', "Not Set")
+            'short': predm_element.text,
+            'full': predm_element.attrs.get('title', "Not Set")
         }
-        prp = skip.nextSibling
-        if isinstance(prp, str):
-            # <br> may be interpreted as '\n'
-            prp = prp.nextSibling
+
+        prp_element = lesson_top.find(
+            name='span',
+            attrs={
+                'class': 'prp'
+            }
+        )
         self.teacher = {
-            'short': prp.text.replace('\xa0', ' '),  # Why...
-            'full': prp.attrs.get('title', "Not Set")
+            'short': prp_element.text.replace('\xa0', ' '),  # Why...
+            'full': prp_element.attrs.get('title', "Not Set")
         }
-        card = prp.nextSibling
-        if isinstance(card, str):
-            # <br> may be interpreted as '\n'
-            card = card.nextSibling
-        card_content: Tag = card.find(
+
+        # Card tag consists of two children
+        # First states type of content
+        # Other - content itself
+        card_tag = lesson_top.find(
+            name='div',
+            attrs={
+                'class': 'card'
+            }
+        )
+        if card_tag:
+            card_content = card_tag.find(
+                name='div',
+                attrs={
+                    'class': 'card-content'
+                }
+            )
+            if card_content:
+                self.lesson_info = card_content.text.replace('\t', '').strip()
+
+        auditorium_tag = lesson_top.find(
+            name='a',
             attrs={
-                'class': 'card-content'
+                'class': 'fg-blue'
             }
         )
-        if card_content:
-            self.lesson_info = card_content.text.replace('\t', '')
+        if auditorium_tag:
+            self.auditorium = auditorium_tag.text
 
 
 class Pair(BaseTag):
     """
         Describes pair from bs4 tag
 
         Note: Pair describes when certain Lesson will happen
@@ -333,17 +318,18 @@
             }
         )
         lessons = []
         if not any([len(all_dates), lesson]):
             return lessons
         if len(all_dates) > 0:
             # This means we are dealing with 'all time' records
+            # Which have multiple lessons per pair
             for lesson in all_dates:
                 lessons.append(
-                    AllTimeLesson.from_tag(
+                    RegularLesson.from_tag(
                         lesson
                     )
                 )
             return lessons
         # This means we are dealing with single week records
         lessons.append(
             RegularLesson.from_tag(
```

### Comparing `rozklad_ontu_parser_makisukurisu-0.0.2.6/ontu_parser/classes/enums.py` & `rozklad_ontu_parser_makisukurisu-0.0.3/ontu_parser/classes/enums.py`

 * *Files identical despite different names*

### Comparing `rozklad_ontu_parser_makisukurisu-0.0.2.6/ontu_parser/classes/parser.py` & `rozklad_ontu_parser_makisukurisu-0.0.3/ontu_parser/classes/parser.py`

 * *Files identical despite different names*

### Comparing `rozklad_ontu_parser_makisukurisu-0.0.2.6/ontu_parser/classes/sender.py` & `rozklad_ontu_parser_makisukurisu-0.0.3/ontu_parser/classes/sender.py`

 * *Files identical despite different names*

### Comparing `rozklad_ontu_parser_makisukurisu-0.0.2.6/LICENSE` & `rozklad_ontu_parser_makisukurisu-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `rozklad_ontu_parser_makisukurisu-0.0.2.6/pyproject.toml` & `rozklad_ontu_parser_makisukurisu-0.0.3/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling", "hatch-requirements-txt"]
 build-backend = "hatchling.build"
 
 [project]
 name = "rozklad_ontu_parser_MakisuKurisu"
-version = "0.0.2.6"
+version = "0.0.3"
 authors = [
   {  name="Pavlo Pohorieltsev", email="667strets@gmail.com"  },
 ]
 description = "Package for parsing data from rozklad.ontu.edu.ua"
 readme = "readme.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `rozklad_ontu_parser_makisukurisu-0.0.2.6/readme.md` & `rozklad_ontu_parser_makisukurisu-0.0.3/readme.md`

 * *Files identical despite different names*

### Comparing `rozklad_ontu_parser_makisukurisu-0.0.2.6/PKG-INFO` & `rozklad_ontu_parser_makisukurisu-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rozklad_ontu_parser_MakisuKurisu
-Version: 0.0.2.6
+Version: 0.0.3
 Summary: Package for parsing data from rozklad.ontu.edu.ua
 Project-URL: Homepage, https://github.com/makisukurisu/rozklad-ontu-parser
 Project-URL: Bug Tracker, https://github.com/makisukurisu/rozklad-ontu-parser/issues
 Author-email: Pavlo Pohorieltsev <667strets@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Natural Language :: English
```

