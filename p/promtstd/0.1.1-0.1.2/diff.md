# Comparing `tmp/promtstd-0.1.1.tar.gz` & `tmp/promtstd-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "promtstd-0.1.1.tar", max compression
+gzip compressed data, was "promtstd-0.1.2.tar", max compression
```

## Comparing `promtstd-0.1.1.tar` & `promtstd-0.1.2.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0    24377 2023-04-09 21:28:04.703272 promtstd-0.1.1/README.md
--rw-r--r--   0        0        0     1779 2023-04-09 21:19:05.190064 promtstd-0.1.1/promtstd/__main__.py
--rw-r--r--   0        0        0     2678 2023-04-09 21:18:15.362169 promtstd-0.1.1/promtstd/lib_linter.py
--rw-r--r--   0        0        0    11092 2023-04-09 21:07:09.223441 promtstd-0.1.1/promtstd/lib_main.py
--rw-r--r--   0        0        0     2996 2023-04-09 20:14:04.713460 promtstd-0.1.1/promtstd/lib_re.py
--rw-r--r--   0        0        0     3292 2023-04-09 19:37:17.459748 promtstd-0.1.1/promtstd/lib_types.py
--rw-r--r--   0        0        0     2644 2023-04-09 21:13:03.306803 promtstd-0.1.1/promtstd/test/test_main.py
--rw-r--r--   0        0        0      422 2023-04-09 21:05:56.003557 promtstd-0.1.1/promtstd/test/utils.py
--rw-r--r--   0        0        0      438 2023-04-09 21:28:13.971197 promtstd-0.1.1/pyproject.toml
--rw-r--r--   0        0        0    24657 1970-01-01 00:00:00.000000 promtstd-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0    24381 2023-04-09 21:29:23.466660 promtstd-0.1.2/README.md
+-rw-r--r--   0        0        0     1779 2023-04-09 21:19:05.190064 promtstd-0.1.2/promtstd/__main__.py
+-rw-r--r--   0        0        0     2678 2023-04-09 21:18:15.362169 promtstd-0.1.2/promtstd/lib_linter.py
+-rw-r--r--   0        0        0    11092 2023-04-09 21:07:09.223441 promtstd-0.1.2/promtstd/lib_main.py
+-rw-r--r--   0        0        0     2996 2023-04-09 20:14:04.713460 promtstd-0.1.2/promtstd/lib_re.py
+-rw-r--r--   0        0        0     3292 2023-04-09 19:37:17.459748 promtstd-0.1.2/promtstd/lib_types.py
+-rw-r--r--   0        0        0     2644 2023-04-09 21:13:03.306803 promtstd-0.1.2/promtstd/test/test_main.py
+-rw-r--r--   0        0        0      422 2023-04-09 21:05:56.003557 promtstd-0.1.2/promtstd/test/utils.py
+-rw-r--r--   0        0        0     1391 2023-04-09 21:39:39.939061 promtstd-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0    25501 1970-01-01 00:00:00.000000 promtstd-0.1.2/PKG-INFO
```

### Comparing `promtstd-0.1.1/README.md` & `promtstd-0.1.2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # promtstd
 
 `promtstd` - это стандарт, разработанный с целью предоставить общепринятый и универсальный подход к хранению и использованию промтов в разработке искусственных интеллектов. Он облегчает взаимодействие разработчиков, повышает качество создаваемых AI и уменьшает трудозатраты на поддержку системы промтов.
 
-![logo](https://github.com/denisxab/promtstd/blob/main/docs/_static/logo_and_text_1280x640.png)
+![logo_web](https://github.com/denisxab/promtstd/blob/main/docs/_static/logo_and_text_1280x640.png)
 
 Основываясь на простоте и доступности `Markdown`, `promtstd` предлагает структурированный и удобочитаемый синтаксис для хранения промтов. Это позволяет разработчикам легко создавать, обновлять и делиться промтами, а также оценивать их качество и эффективность.
 
 Применение стандарта `promtstd` в проектах искусственного интеллекта обеспечивает упорядоченность кодовой базы, что значительно снижает вероятность ошибок, затруднений и проблем при дальнейшей разработке и поддержке AI. В целом, использование `promtstd` призвано способствовать успешному развитию AI-технологий и улучшению пользовательского опыта.
 
 ## Важность стандарта
```

### Comparing `promtstd-0.1.1/promtstd/__main__.py` & `promtstd-0.1.2/promtstd/__main__.py`

 * *Files identical despite different names*

### Comparing `promtstd-0.1.1/promtstd/lib_linter.py` & `promtstd-0.1.2/promtstd/lib_linter.py`

 * *Files identical despite different names*

### Comparing `promtstd-0.1.1/promtstd/lib_main.py` & `promtstd-0.1.2/promtstd/lib_main.py`

 * *Files identical despite different names*

### Comparing `promtstd-0.1.1/promtstd/lib_re.py` & `promtstd-0.1.2/promtstd/lib_re.py`

 * *Files identical despite different names*

### Comparing `promtstd-0.1.1/promtstd/lib_types.py` & `promtstd-0.1.2/promtstd/lib_types.py`

 * *Files identical despite different names*

### Comparing `promtstd-0.1.1/promtstd/test/test_main.py` & `promtstd-0.1.2/promtstd/test/test_main.py`

 * *Files identical despite different names*

### Comparing `promtstd-0.1.1/PKG-INFO` & `promtstd-0.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 Metadata-Version: 2.1
 Name: promtstd
-Version: 0.1.1
-Summary: 
-Author: Your Name
-Author-email: you@example.com
+Version: 0.1.2
+Summary: promtstd robot - универсальный стандарт для хранения и использования промтов в AI. books Основан на Markdown, обеспечивает легкость чтения и структурированность. 
+Home-page: https://github.com/denisxab/promtstd
+Keywords: стандарт промтов,promtstd,promt,ai,хранение промтов,использование промтов,разработка AI,искусственный интеллект,Markdown,унификация,структурирование,синтаксис,взаимодействие разработчиков,метаинформация,шаблоны,примеры,вспомогательные промты
+Author: Denis Kustov
+Author-email: pro-progerkustov@yandex.ru
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
+Project-URL: Repository, https://github.com/denisxab/promtstd
 Description-Content-Type: text/markdown
 
 # promtstd
 
 `promtstd` - это стандарт, разработанный с целью предоставить общепринятый и универсальный подход к хранению и использованию промтов в разработке искусственных интеллектов. Он облегчает взаимодействие разработчиков, повышает качество создаваемых AI и уменьшает трудозатраты на поддержку системы промтов.
 
-![logo](https://github.com/denisxab/promtstd/blob/main/docs/_static/logo_and_text_1280x640.png)
+![logo_web](https://github.com/denisxab/promtstd/blob/main/docs/_static/logo_and_text_1280x640.png)
 
 Основываясь на простоте и доступности `Markdown`, `promtstd` предлагает структурированный и удобочитаемый синтаксис для хранения промтов. Это позволяет разработчикам легко создавать, обновлять и делиться промтами, а также оценивать их качество и эффективность.
 
 Применение стандарта `promtstd` в проектах искусственного интеллекта обеспечивает упорядоченность кодовой базы, что значительно снижает вероятность ошибок, затруднений и проблем при дальнейшей разработке и поддержке AI. В целом, использование `promtstd` призвано способствовать успешному развитию AI-технологий и улучшению пользовательского опыта.
 
 ## Важность стандарта
```

