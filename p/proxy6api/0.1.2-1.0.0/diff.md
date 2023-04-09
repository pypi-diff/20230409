# Comparing `tmp/proxy6api-0.1.2.tar.gz` & `tmp/proxy6api-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "proxy6api-0.1.2.tar", max compression
+gzip compressed data, was "proxy6api-1.0.0.tar", max compression
```

## Comparing `proxy6api-0.1.2.tar` & `proxy6api-1.0.0.tar`

### file list

```diff
@@ -1,10 +1,11 @@
--rw-r--r--   0        0        0     1076 2023-03-31 20:13:38.586324 proxy6api-0.1.2/LICENSE
--rw-r--r--   0        0        0       71 2023-03-31 20:13:38.586324 proxy6api-0.1.2/README.md
--rw-r--r--   0        0        0      337 2023-04-07 17:04:48.246253 proxy6api-0.1.2/proxy6api/__init__.py
--rw-r--r--   0        0        0     8516 2023-04-07 17:00:12.854973 proxy6api-0.1.2/proxy6api/client.py
--rw-r--r--   0        0        0      185 2023-04-07 17:03:32.320244 proxy6api-0.1.2/proxy6api/settings/__init__.py
--rw-r--r--   0        0        0     3885 2023-04-03 17:00:42.211299 proxy6api-0.1.2/proxy6api/settings/bases.py
--rw-r--r--   0        0        0     2269 2023-04-03 17:09:54.155879 proxy6api-0.1.2/proxy6api/settings/errors.py
--rw-r--r--   0        0        0      457 2023-04-07 16:54:45.074343 proxy6api-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      756 1970-01-01 00:00:00.000000 proxy6api-0.1.2/setup.py
--rw-r--r--   0        0        0      531 1970-01-01 00:00:00.000000 proxy6api-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1076 2023-03-31 20:13:38.586324 proxy6api-1.0.0/LICENSE
+-rw-r--r--   0        0        0     2136 2023-04-09 16:54:04.527839 proxy6api-1.0.0/README.md
+-rw-r--r--   0        0        0     3252 2023-04-09 17:00:03.433427 proxy6api-1.0.0/proxy6api/__init__.py
+-rw-r--r--   0        0        0    15743 2023-04-09 16:30:36.079580 proxy6api-1.0.0/proxy6api/client.py
+-rw-r--r--   0        0        0      724 2023-04-09 16:36:51.559651 proxy6api-1.0.0/proxy6api/settings/__init__.py
+-rw-r--r--   0        0        0     3885 2023-04-03 17:00:42.211299 proxy6api-1.0.0/proxy6api/settings/bases.py
+-rw-r--r--   0        0        0     2875 2023-04-09 13:26:22.037196 proxy6api-1.0.0/proxy6api/settings/errors.py
+-rw-r--r--   0        0        0     1971 2023-04-09 16:29:43.051452 proxy6api-1.0.0/proxy6api/settings/typing_methods.py
+-rw-r--r--   0        0        0      457 2023-04-09 16:56:44.461480 proxy6api-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0     2921 1970-01-01 00:00:00.000000 proxy6api-1.0.0/setup.py
+-rw-r--r--   0        0        0     2596 1970-01-01 00:00:00.000000 proxy6api-1.0.0/PKG-INFO
```

### Comparing `proxy6api-0.1.2/LICENSE` & `proxy6api-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `proxy6api-0.1.2/proxy6api/settings/bases.py` & `proxy6api-1.0.0/proxy6api/settings/bases.py`

 * *Files identical despite different names*

### Comparing `proxy6api-0.1.2/proxy6api/settings/errors.py` & `proxy6api-1.0.0/proxy6api/settings/errors.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,13 @@
 CODES_OF_ERRORS = {
+    10: "Couldn't decode the text into json - Не удалось расшифровать текст в json.",
+    20: "A Connection error occurred - Произошла ошибка подключения.",
+    25: "The request timed out while trying to connect to the remote server. "
+    "Requests that produced this error are safe to retry. - Время ожидания запроса истекло "
+    "при попытке подключения к удаленному серверу. Запросы, вызвавшие эту ошибку, можно безопасно повторить",
     30: "Error unknown - Неизвестная ошибка",
     100: "Error key - Ошибка авторизации, неверный ключ ",
     105: "Error ip - Доступ к API произошел с неверного IP (если включено "
     "ограничение), либо некорректный формат IP адреса",
     110: "Error method - Ошибочный метод ",
     200: "Error count - Ошибка кол-ва прокси, неверно указано кол-во, " "либо отсутствует",
     210: "Error period - Ошибка периода, неверно указано кол-во (дней), " "либо отсутствует",
```

