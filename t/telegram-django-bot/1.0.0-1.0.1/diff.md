# Comparing `tmp/telegram_django_bot-1.0.0.tar.gz` & `tmp/telegram_django_bot-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "telegram_django_bot-1.0.0.tar", last modified: Tue Mar 14 14:54:24 2023, max compression
+gzip compressed data, was "telegram_django_bot-1.0.1.tar", last modified: Sun Apr  9 07:46:20 2023, max compression
```

## Comparing `telegram_django_bot-1.0.0.tar` & `telegram_django_bot-1.0.1.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-03-14 14:54:24.410608 telegram_django_bot-1.0.0/
--rw-r--r--   0 alex       (501) staff       (20)     1073 2022-09-07 14:16:11.000000 telegram_django_bot-1.0.0/LICENSE
--rw-r--r--   0 alex       (501) staff       (20)      169 2023-01-17 13:23:14.000000 telegram_django_bot-1.0.0/MANIFEST.in
--rw-r--r--   0 alex       (501) staff       (20)    40224 2023-03-14 14:54:24.411310 telegram_django_bot-1.0.0/PKG-INFO
--rw-r--r--   0 alex       (501) staff       (20)    38984 2023-03-14 14:54:15.000000 telegram_django_bot-1.0.0/README.rst
--rw-r--r--   0 alex       (501) staff       (20)     1302 2023-03-14 14:54:24.413319 telegram_django_bot-1.0.0/setup.cfg
--rw-r--r--   0 alex       (501) staff       (20)       39 2022-09-07 14:16:11.000000 telegram_django_bot-1.0.0/setup.py
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-03-14 14:54:24.387894 telegram_django_bot-1.0.0/telegram_django_bot/
--rw-r--r--   0 alex       (501) staff       (20)       72 2023-03-14 14:28:06.000000 telegram_django_bot-1.0.0/telegram_django_bot/__init__.py
--rw-r--r--   0 alex       (501) staff       (20)     2506 2023-01-17 12:17:05.000000 telegram_django_bot-1.0.0/telegram_django_bot/admin.py
--rw-r--r--   0 alex       (501) staff       (20)     1000 2023-01-17 12:17:05.000000 telegram_django_bot-1.0.0/telegram_django_bot/admin_utils.py
--rw-r--r--   0 alex       (501) staff       (20)      111 2023-01-17 12:17:05.000000 telegram_django_bot-1.0.0/telegram_django_bot/apps.py
--rw-r--r--   0 alex       (501) staff       (20)     6909 2023-03-14 14:28:06.000000 telegram_django_bot-1.0.0/telegram_django_bot/forms.py
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-03-14 14:54:24.371859 telegram_django_bot-1.0.0/telegram_django_bot/locale/
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-03-14 14:54:24.371959 telegram_django_bot-1.0.0/telegram_django_bot/locale/ru/
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-03-14 14:54:24.394379 telegram_django_bot-1.0.0/telegram_django_bot/locale/ru/LC_MESSAGES/
--rw-r--r--   0 alex       (501) staff       (20)     6003 2023-01-17 12:17:05.000000 telegram_django_bot-1.0.0/telegram_django_bot/locale/ru/LC_MESSAGES/django.mo
--rw-r--r--   0 alex       (501) staff       (20)     7381 2023-01-17 12:17:05.000000 telegram_django_bot-1.0.0/telegram_django_bot/locale/ru/LC_MESSAGES/django.po
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-03-14 14:54:24.408514 telegram_django_bot-1.0.0/telegram_django_bot/migrations/
--rw-r--r--   0 alex       (501) staff       (20)     9252 2022-09-07 14:16:11.000000 telegram_django_bot-1.0.0/telegram_django_bot/migrations/0001_initial.py
--rw-r--r--   0 alex       (501) staff       (20)      292 2022-09-07 14:16:11.000000 telegram_django_bot-1.0.0/telegram_django_bot/migrations/0002_delete_user.py
--rw-r--r--   0 alex       (501) staff       (20)      604 2022-09-07 14:16:11.000000 telegram_django_bot-1.0.0/telegram_django_bot/migrations/0003_botmenuelem_message_format.py
--rw-r--r--   0 alex       (501) staff       (20)     4613 2022-09-16 18:03:58.000000 telegram_django_bot-1.0.0/telegram_django_bot/migrations/0004_auto_20220915_0448.py
--rw-r--r--   0 alex       (501) staff       (20)      397 2022-10-10 18:30:54.000000 telegram_django_bot-1.0.0/telegram_django_bot/migrations/0005_auto_20221010_1330.py
--rw-r--r--   0 alex       (501) staff       (20)      478 2022-10-23 06:57:02.000000 telegram_django_bot-1.0.0/telegram_django_bot/migrations/0006_auto_20221023_0157.py
--rw-r--r--   0 alex       (501) staff       (20)      636 2022-12-02 09:05:36.000000 telegram_django_bot-1.0.0/telegram_django_bot/migrations/0007_auto_20221202_0305.py
--rw-r--r--   0 alex       (501) staff       (20)     1626 2023-01-17 12:17:05.000000 telegram_django_bot-1.0.0/telegram_django_bot/migrations/0008_auto_20221225_1050.py
--rw-r--r--   0 alex       (501) staff       (20)        0 2022-09-07 14:16:11.000000 telegram_django_bot-1.0.0/telegram_django_bot/migrations/__init__.py
--rw-r--r--   0 alex       (501) staff       (20)    14674 2023-03-14 14:28:06.000000 telegram_django_bot-1.0.0/telegram_django_bot/models.py
--rw-r--r--   0 alex       (501) staff       (20)      277 2023-03-14 14:28:06.000000 telegram_django_bot-1.0.0/telegram_django_bot/permissions.py
--rw-r--r--   0 alex       (501) staff       (20)     5375 2023-03-14 14:28:06.000000 telegram_django_bot-1.0.0/telegram_django_bot/routing.py
--rw-r--r--   0 alex       (501) staff       (20)     5232 2022-10-23 21:06:50.000000 telegram_django_bot-1.0.0/telegram_django_bot/tasks.py
--rw-r--r--   0 alex       (501) staff       (20)    30066 2023-03-14 14:28:06.000000 telegram_django_bot-1.0.0/telegram_django_bot/td_viewset.py
--rw-r--r--   0 alex       (501) staff       (20)     1498 2023-03-14 14:28:06.000000 telegram_django_bot-1.0.0/telegram_django_bot/telegram_lib_redefinition.py
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-03-14 14:54:24.409413 telegram_django_bot-1.0.0/telegram_django_bot/templates/
--rw-r--r--   0 alex       (501) staff       (20)     1598 2022-09-07 14:16:11.000000 telegram_django_bot-1.0.0/telegram_django_bot/templates/dropdown_filter1.html
--rw-r--r--   0 alex       (501) staff       (20)     3300 2023-03-14 14:28:06.000000 telegram_django_bot-1.0.0/telegram_django_bot/test.py
--rw-r--r--   0 alex       (501) staff       (20)    12071 2023-03-14 14:28:06.000000 telegram_django_bot-1.0.0/telegram_django_bot/tg_dj_bot.py
--rw-r--r--   0 alex       (501) staff       (20)     2293 2023-03-14 14:28:06.000000 telegram_django_bot-1.0.0/telegram_django_bot/user_viewset.py
--rw-r--r--   0 alex       (501) staff       (20)    12164 2023-03-14 14:40:31.000000 telegram_django_bot-1.0.0/telegram_django_bot/utils.py
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-03-14 14:54:24.392856 telegram_django_bot-1.0.0/telegram_django_bot.egg-info/
--rw-r--r--   0 alex       (501) staff       (20)    40224 2023-03-14 14:54:23.000000 telegram_django_bot-1.0.0/telegram_django_bot.egg-info/PKG-INFO
--rw-r--r--   0 alex       (501) staff       (20)     1403 2023-03-14 14:54:24.000000 telegram_django_bot-1.0.0/telegram_django_bot.egg-info/SOURCES.txt
--rw-r--r--   0 alex       (501) staff       (20)        1 2023-03-14 14:54:23.000000 telegram_django_bot-1.0.0/telegram_django_bot.egg-info/dependency_links.txt
--rw-r--r--   0 alex       (501) staff       (20)      106 2023-03-14 14:54:24.000000 telegram_django_bot-1.0.0/telegram_django_bot.egg-info/requires.txt
--rw-r--r--   0 alex       (501) staff       (20)       20 2023-03-14 14:54:24.000000 telegram_django_bot-1.0.0/telegram_django_bot.egg-info/top_level.txt
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-04-09 07:46:20.765903 telegram_django_bot-1.0.1/
+-rw-r--r--   0 alex       (501) staff       (20)     1073 2022-09-07 14:16:11.000000 telegram_django_bot-1.0.1/LICENSE
+-rw-r--r--   0 alex       (501) staff       (20)      169 2023-01-17 13:23:14.000000 telegram_django_bot-1.0.1/MANIFEST.in
+-rw-r--r--   0 alex       (501) staff       (20)    40224 2023-04-09 07:46:20.766386 telegram_django_bot-1.0.1/PKG-INFO
+-rw-r--r--   0 alex       (501) staff       (20)    38984 2023-04-09 07:32:50.000000 telegram_django_bot-1.0.1/README.rst
+-rw-r--r--   0 alex       (501) staff       (20)     1302 2023-04-09 07:46:20.767911 telegram_django_bot-1.0.1/setup.cfg
+-rw-r--r--   0 alex       (501) staff       (20)       39 2022-09-07 14:16:11.000000 telegram_django_bot-1.0.1/setup.py
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-04-09 07:46:20.753732 telegram_django_bot-1.0.1/telegram_django_bot/
+-rw-r--r--   0 alex       (501) staff       (20)       72 2023-04-09 07:32:50.000000 telegram_django_bot-1.0.1/telegram_django_bot/__init__.py
+-rw-r--r--   0 alex       (501) staff       (20)     4332 2023-04-09 07:45:25.000000 telegram_django_bot-1.0.1/telegram_django_bot/admin.py
+-rw-r--r--   0 alex       (501) staff       (20)     1000 2023-04-09 07:21:01.000000 telegram_django_bot-1.0.1/telegram_django_bot/admin_utils.py
+-rw-r--r--   0 alex       (501) staff       (20)      111 2023-01-17 12:17:05.000000 telegram_django_bot-1.0.1/telegram_django_bot/apps.py
+-rw-r--r--   0 alex       (501) staff       (20)     6909 2023-04-09 07:32:50.000000 telegram_django_bot-1.0.1/telegram_django_bot/forms.py
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-04-09 07:46:20.743149 telegram_django_bot-1.0.1/telegram_django_bot/locale/
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-04-09 07:46:20.743257 telegram_django_bot-1.0.1/telegram_django_bot/locale/ru/
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-04-09 07:46:20.758104 telegram_django_bot-1.0.1/telegram_django_bot/locale/ru/LC_MESSAGES/
+-rw-r--r--   0 alex       (501) staff       (20)     6042 2023-04-09 07:45:25.000000 telegram_django_bot-1.0.1/telegram_django_bot/locale/ru/LC_MESSAGES/django.mo
+-rw-r--r--   0 alex       (501) staff       (20)     7478 2023-04-09 07:45:25.000000 telegram_django_bot-1.0.1/telegram_django_bot/locale/ru/LC_MESSAGES/django.po
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-04-09 07:46:20.764993 telegram_django_bot-1.0.1/telegram_django_bot/migrations/
+-rw-r--r--   0 alex       (501) staff       (20)     9252 2022-09-07 14:16:11.000000 telegram_django_bot-1.0.1/telegram_django_bot/migrations/0001_initial.py
+-rw-r--r--   0 alex       (501) staff       (20)      292 2022-09-07 14:16:11.000000 telegram_django_bot-1.0.1/telegram_django_bot/migrations/0002_delete_user.py
+-rw-r--r--   0 alex       (501) staff       (20)      604 2022-09-07 14:16:11.000000 telegram_django_bot-1.0.1/telegram_django_bot/migrations/0003_botmenuelem_message_format.py
+-rw-r--r--   0 alex       (501) staff       (20)     4613 2022-09-16 18:03:58.000000 telegram_django_bot-1.0.1/telegram_django_bot/migrations/0004_auto_20220915_0448.py
+-rw-r--r--   0 alex       (501) staff       (20)      397 2022-10-10 18:30:54.000000 telegram_django_bot-1.0.1/telegram_django_bot/migrations/0005_auto_20221010_1330.py
+-rw-r--r--   0 alex       (501) staff       (20)      478 2022-10-23 06:57:02.000000 telegram_django_bot-1.0.1/telegram_django_bot/migrations/0006_auto_20221023_0157.py
+-rw-r--r--   0 alex       (501) staff       (20)      636 2022-12-02 09:05:36.000000 telegram_django_bot-1.0.1/telegram_django_bot/migrations/0007_auto_20221202_0305.py
+-rw-r--r--   0 alex       (501) staff       (20)     1626 2023-01-17 12:17:05.000000 telegram_django_bot-1.0.1/telegram_django_bot/migrations/0008_auto_20221225_1050.py
+-rw-r--r--   0 alex       (501) staff       (20)        0 2022-09-07 14:16:11.000000 telegram_django_bot-1.0.1/telegram_django_bot/migrations/__init__.py
+-rw-r--r--   0 alex       (501) staff       (20)    14827 2023-04-09 07:45:25.000000 telegram_django_bot-1.0.1/telegram_django_bot/models.py
+-rw-r--r--   0 alex       (501) staff       (20)      277 2023-04-09 07:32:50.000000 telegram_django_bot-1.0.1/telegram_django_bot/permissions.py
+-rw-r--r--   0 alex       (501) staff       (20)     5375 2023-04-09 07:32:50.000000 telegram_django_bot-1.0.1/telegram_django_bot/routing.py
+-rw-r--r--   0 alex       (501) staff       (20)     5232 2022-10-23 21:06:50.000000 telegram_django_bot-1.0.1/telegram_django_bot/tasks.py
+-rw-r--r--   0 alex       (501) staff       (20)    30066 2023-04-09 07:32:50.000000 telegram_django_bot-1.0.1/telegram_django_bot/td_viewset.py
+-rw-r--r--   0 alex       (501) staff       (20)     1498 2023-04-09 07:32:50.000000 telegram_django_bot-1.0.1/telegram_django_bot/telegram_lib_redefinition.py
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-04-09 07:46:20.765420 telegram_django_bot-1.0.1/telegram_django_bot/templates/
+-rw-r--r--   0 alex       (501) staff       (20)     1598 2022-09-07 14:16:11.000000 telegram_django_bot-1.0.1/telegram_django_bot/templates/dropdown_filter1.html
+-rw-r--r--   0 alex       (501) staff       (20)     3300 2023-04-09 07:32:50.000000 telegram_django_bot-1.0.1/telegram_django_bot/test.py
+-rw-r--r--   0 alex       (501) staff       (20)    12071 2023-04-09 07:32:50.000000 telegram_django_bot-1.0.1/telegram_django_bot/tg_dj_bot.py
+-rw-r--r--   0 alex       (501) staff       (20)     2293 2023-04-09 07:32:50.000000 telegram_django_bot-1.0.1/telegram_django_bot/user_viewset.py
+-rw-r--r--   0 alex       (501) staff       (20)    12164 2023-04-09 07:32:50.000000 telegram_django_bot-1.0.1/telegram_django_bot/utils.py
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-04-09 07:46:20.756791 telegram_django_bot-1.0.1/telegram_django_bot.egg-info/
+-rw-r--r--   0 alex       (501) staff       (20)    40224 2023-04-09 07:46:20.000000 telegram_django_bot-1.0.1/telegram_django_bot.egg-info/PKG-INFO
+-rw-r--r--   0 alex       (501) staff       (20)     1403 2023-04-09 07:46:20.000000 telegram_django_bot-1.0.1/telegram_django_bot.egg-info/SOURCES.txt
+-rw-r--r--   0 alex       (501) staff       (20)        1 2023-04-09 07:46:20.000000 telegram_django_bot-1.0.1/telegram_django_bot.egg-info/dependency_links.txt
+-rw-r--r--   0 alex       (501) staff       (20)      106 2023-04-09 07:46:20.000000 telegram_django_bot-1.0.1/telegram_django_bot.egg-info/requires.txt
+-rw-r--r--   0 alex       (501) staff       (20)       20 2023-04-09 07:46:20.000000 telegram_django_bot-1.0.1/telegram_django_bot.egg-info/top_level.txt
```

### Comparing `telegram_django_bot-1.0.0/LICENSE` & `telegram_django_bot-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `telegram_django_bot-1.0.0/PKG-INFO` & `telegram_django_bot-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: telegram_django_bot
-Version: 1.0.0
+Version: 1.0.1
 Summary: Telegram Django Bot Bridge
 Home-page: https://github.com/alexanderaleskin/telegram_django_bot_bridge
 Author: Alexander Aleskin
 Author-email: alexanderaleskin@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `telegram_django_bot-1.0.0/README.rst` & `telegram_django_bot-1.0.1/README.rst`

 * *Files identical despite different names*

### Comparing `telegram_django_bot-1.0.0/setup.cfg` & `telegram_django_bot-1.0.1/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = telegram_django_bot
-version = 1.0.0
+version = 1.0.1
 description = Telegram Django Bot Bridge
 long_description = file: README.rst
 url = https://github.com/alexanderaleskin/telegram_django_bot_bridge
 author = Alexander Aleskin
 author_email = alexanderaleskin@gmail.com
 license = MIT
 classifiers =
```

### Comparing `telegram_django_bot-1.0.0/telegram_django_bot/admin_utils.py` & `telegram_django_bot-1.0.1/telegram_django_bot/admin_utils.py`

 * *Files identical despite different names*

### Comparing `telegram_django_bot-1.0.0/telegram_django_bot/forms.py` & `telegram_django_bot-1.0.1/telegram_django_bot/forms.py`

 * *Files identical despite different names*

### Comparing `telegram_django_bot-1.0.0/telegram_django_bot/locale/ru/LC_MESSAGES/django.mo` & `telegram_django_bot-1.0.1/telegram_django_bot/locale/ru/LC_MESSAGES/django.mo`

 * *Files 5% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,12 +1,11 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-01-17 00:56+0300\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
@@ -28,14 +27,17 @@
 
 msgid "Default_text Translation"
 msgstr "Перевод Default_text"
 
 msgid "Document"
 msgstr "Документ"
 
+msgid "Export Selected"
+msgstr "Экспортировать выбранное"
+
 msgid "File attachment to the message"
 msgstr "Медиа файл сообщения"
 
 msgid "File code in telegram (must be deleted when replacing file)"
 msgstr "Файл приложение к сообщению"
 
 msgid "GIF/animation"
```

### Comparing `telegram_django_bot-1.0.0/telegram_django_bot/locale/ru/LC_MESSAGES/django.po` & `telegram_django_bot-1.0.1/telegram_django_bot/locale/ru/LC_MESSAGES/django.po`

 * *Files 2% similar despite different names*

```diff
@@ -4,25 +4,29 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-01-17 00:56+0300\n"
+"POT-Creation-Date: 2023-04-03 13:51+0300\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=4; plural=(n%10==1 && n%100!=11 ? 0 : n%10>=2 && n"
-"%10<=4 && (n%100<12 || n%100>14) ? 1 : n%10==0 || (n%10>=5 && n%10<=9) || (n"
-"%100>=11 && n%100<=14)? 2 : 3);\n"
+"Plural-Forms: nplurals=4; plural=(n%10==1 && n%100!=11 ? 0 : n%10>=2 && "
+"n%10<=4 && (n%100<12 || n%100>14) ? 1 : n%10==0 || (n%10>=5 && n%10<=9) || "
+"(n%100>=11 && n%100<=14)? 2 : 3);\n"
+
+#: admin.py:28
+msgid "Export Selected"
+msgstr "Экспортировать выбранное"
 
 #: forms.py:187
 msgid "User"
 msgstr "Пользователь"
 
 #: forms.py:195
 msgid "Timezone"
@@ -113,16 +117,16 @@
 #: models.py:244
 msgid ""
 "InlineKeyboardMarkup buttons structure (double list of dict), where each "
 "button(dict) has next format: {\"text\": \"text\", \"url\": \"google.com\"} "
 "or {\"text\":\"text\", \"callback_data\": \"data\"})"
 msgstr ""
 "Описыват InlineKeyboardMarkup структура кнопок (двойной вложенный список), "
-"где каждая кнопка это словарь формата: {\"text\": \"text\", \"url\": \"google.com\"} "
-"или {\"text\":\"text\", \"callback_data\": \"data\"})"
+"где каждая кнопка это словарь формата: {\"text\": \"text\", \"url\": "
+"\"google.com\"} или {\"text\":\"text\", \"callback_data\": \"data\"})"
 
 #: models.py:248
 msgid "File attachment to the message"
 msgstr "Медиа файл сообщения"
 
 #: models.py:251
 msgid "File code in telegram (must be deleted when replacing file)"
```

### Comparing `telegram_django_bot-1.0.0/telegram_django_bot/migrations/0001_initial.py` & `telegram_django_bot-1.0.1/telegram_django_bot/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `telegram_django_bot-1.0.0/telegram_django_bot/migrations/0003_botmenuelem_message_format.py` & `telegram_django_bot-1.0.1/telegram_django_bot/migrations/0003_botmenuelem_message_format.py`

 * *Files identical despite different names*

### Comparing `telegram_django_bot-1.0.0/telegram_django_bot/migrations/0004_auto_20220915_0448.py` & `telegram_django_bot-1.0.1/telegram_django_bot/migrations/0004_auto_20220915_0448.py`

 * *Files identical despite different names*

### Comparing `telegram_django_bot-1.0.0/telegram_django_bot/migrations/0007_auto_20221202_0305.py` & `telegram_django_bot-1.0.1/telegram_django_bot/migrations/0007_auto_20221202_0305.py`

 * *Files identical despite different names*

### Comparing `telegram_django_bot-1.0.0/telegram_django_bot/migrations/0008_auto_20221225_1050.py` & `telegram_django_bot-1.0.1/telegram_django_bot/migrations/0008_auto_20221225_1050.py`

 * *Files identical despite different names*

### Comparing `telegram_django_bot-1.0.0/telegram_django_bot/models.py` & `telegram_django_bot-1.0.1/telegram_django_bot/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -112,15 +112,15 @@
     # form structure {'form_name': '', 'form_data': {}}
     current_utrl_form_db = models.CharField(max_length=4096, default='{}', blank=True)
 
     class Meta:
         abstract = True
 
     def __str__(self):
-        return f"U({self.id} {self.telegram_username} {self.first_name})"
+        return f"U({self.id}, {self.telegram_username or '-'}, {self.first_name or '-'})"
 
     @property
     def current_utrl_form(self):
         if not hasattr(self, '_current_utrl_form'):
             self._current_utrl_form = json.loads(self.current_utrl_form_db, cls=TelegramDjangoJsonDecoder)
         return self._current_utrl_form
 
@@ -198,26 +198,28 @@
     price = models.FloatField(null=True, blank=True)
     link = models.CharField(max_length=64, validators=[validators.RegexValidator(
         '^[a-zA-Z0-9_-]+$',
         _('Telegram is only accepted letters, numbers and signs - _'),
     )])
     users = models.ManyToManyField(settings.AUTH_USER_MODEL)
 
+    def __str__(self):
+        return f'TDL({self.id}, {self.link})'
 
 class ActionLog(models.Model):
     """
     User actions logs
     """
 
     dttm = models.DateTimeField(auto_now_add=True, db_index=True)
     type = models.CharField(max_length=64)
     user = models.ForeignKey(settings.AUTH_USER_MODEL, on_delete=models.CASCADE, null=True, blank=True)
 
     def __str__(self):
-        return '({}, {}, {})'.format(self.user_id, self.dttm, self.type)
+        return 'AL({}, {}, {})'.format(self.user_id, self.dttm, self.type)
 
 
 class BotMenuElem(models.Model):
     """
 
     """
 
@@ -258,15 +260,15 @@
     media = models.FileField(help_text=_('File attachment to the message'), null=True, blank=True)
     telegram_file_code = models.CharField(
         max_length=512, null=True, blank=True,
         help_text=_('File code in telegram (must be deleted when replacing file)')
     )
 
     def __str__(self):
-        return f"BME ({self.id}) - { self.command[:32] if self.command else self.message[:32]}"
+        return f"BME({self.id}, { self.command[:32] if self.command else self.message[:32]})"
 
     def save(self, *args, **kwargs):
         # bot = telegram.Bot(TELEGRAM_TOKEN)
         
         super(BotMenuElem, self).save(*args, **kwargs)
 
         # check and create new models for translation
@@ -401,14 +403,17 @@
             elif 'h' in part:
                 hours = float(part.replace('h', ''))
             else:
                 raise ValueError(f'unknown format {part}')
 
         return timezone.timedelta(days=days, hours=hours)
 
+    def __str__(self):
+        return f"T({self.id}, {self.name})"
+
 
 class UserTrigger(TelegramAbstractActiveModel):
     trigger = models.ForeignKey(Trigger, on_delete=models.PROTECT)
     user = models.ForeignKey(settings.AUTH_USER_MODEL, on_delete=models.PROTECT)
 
     is_sent = models.BooleanField(default=False)
```

### Comparing `telegram_django_bot-1.0.0/telegram_django_bot/routing.py` & `telegram_django_bot-1.0.1/telegram_django_bot/routing.py`

 * *Files identical despite different names*

### Comparing `telegram_django_bot-1.0.0/telegram_django_bot/tasks.py` & `telegram_django_bot-1.0.1/telegram_django_bot/tasks.py`

 * *Files identical despite different names*

### Comparing `telegram_django_bot-1.0.0/telegram_django_bot/td_viewset.py` & `telegram_django_bot-1.0.1/telegram_django_bot/td_viewset.py`

 * *Files identical despite different names*

### Comparing `telegram_django_bot-1.0.0/telegram_django_bot/telegram_lib_redefinition.py` & `telegram_django_bot-1.0.1/telegram_django_bot/telegram_lib_redefinition.py`

 * *Files identical despite different names*

### Comparing `telegram_django_bot-1.0.0/telegram_django_bot/templates/dropdown_filter1.html` & `telegram_django_bot-1.0.1/telegram_django_bot/templates/dropdown_filter1.html`

 * *Files identical despite different names*

### Comparing `telegram_django_bot-1.0.0/telegram_django_bot/test.py` & `telegram_django_bot-1.0.1/telegram_django_bot/test.py`

 * *Files identical despite different names*

### Comparing `telegram_django_bot-1.0.0/telegram_django_bot/tg_dj_bot.py` & `telegram_django_bot-1.0.1/telegram_django_bot/tg_dj_bot.py`

 * *Files identical despite different names*

### Comparing `telegram_django_bot-1.0.0/telegram_django_bot/user_viewset.py` & `telegram_django_bot-1.0.1/telegram_django_bot/user_viewset.py`

 * *Files identical despite different names*

### Comparing `telegram_django_bot-1.0.0/telegram_django_bot/utils.py` & `telegram_django_bot-1.0.1/telegram_django_bot/utils.py`

 * *Files identical despite different names*

### Comparing `telegram_django_bot-1.0.0/telegram_django_bot.egg-info/PKG-INFO` & `telegram_django_bot-1.0.1/telegram_django_bot.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: telegram-django-bot
-Version: 1.0.0
+Version: 1.0.1
 Summary: Telegram Django Bot Bridge
 Home-page: https://github.com/alexanderaleskin/telegram_django_bot_bridge
 Author: Alexander Aleskin
 Author-email: alexanderaleskin@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `telegram_django_bot-1.0.0/telegram_django_bot.egg-info/SOURCES.txt` & `telegram_django_bot-1.0.1/telegram_django_bot.egg-info/SOURCES.txt`

 * *Files identical despite different names*

