# Comparing `tmp/webssh-1.6.1.tar.gz` & `tmp/webssh-1.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "webssh-1.6.1.tar", last modified: Mon Nov 21 09:29:08 2022, max compression
+gzip compressed data, was "webssh-1.6.2.tar", last modified: Sun Apr  9 06:39:19 2023, max compression
```

## Comparing `webssh-1.6.1.tar` & `webssh-1.6.2.tar`

### file list

```diff
@@ -1,70 +1,70 @@
-drwxrwxr-x   0 sheng     (1000) sheng     (1000)        0 2022-11-21 09:29:08.206756 webssh-1.6.1/
--rw-rw-r--   0 sheng     (1000) sheng     (1000)     1079 2017-11-08 13:11:41.000000 webssh-1.6.1/LICENSE
--rw-r--r--   0 sheng     (1000) sheng     (1000)      241 2018-08-10 07:44:35.000000 webssh-1.6.1/MANIFEST.in
--rw-rw-r--   0 sheng     (1000) sheng     (1000)     6387 2022-11-21 09:29:08.206756 webssh-1.6.1/PKG-INFO
--rw-rw-r--   0 sheng     (1000) sheng     (1000)     5129 2022-05-29 11:14:51.000000 webssh-1.6.1/README.md
--rw-r--r--   0 sheng     (1000) sheng     (1000)     5654 2020-02-13 13:28:36.000000 webssh-1.6.1/README.rst
--rw-r--r--   0 sheng     (1000) sheng     (1000)      172 2022-11-21 09:29:08.206756 webssh-1.6.1/setup.cfg
--rw-rw-r--   0 sheng     (1000) sheng     (1000)     1175 2022-11-21 06:13:51.000000 webssh-1.6.1/setup.py
-drwxrwxr-x   0 sheng     (1000) sheng     (1000)        0 2022-11-21 09:29:08.202756 webssh-1.6.1/tests/
--rw-r--r--   0 sheng     (1000) sheng     (1000)        0 2018-05-06 13:10:34.000000 webssh-1.6.1/tests/__init__.py
-drwxrwxr-x   0 sheng     (1000) sheng     (1000)        0 2022-11-21 09:29:08.206756 webssh-1.6.1/tests/data/
--rw-r--r--   0 sheng     (1000) sheng     (1000)     1233 2019-05-17 07:51:35.000000 webssh-1.6.1/tests/data/cert.crt
--rw-r--r--   0 sheng     (1000) sheng     (1000)     1704 2019-05-17 07:51:35.000000 webssh-1.6.1/tests/data/cert.key
-drwxrwxr-x   0 sheng     (1000) sheng     (1000)        0 2022-11-21 09:29:08.206756 webssh-1.6.1/tests/data/fonts/
--rw-r--r--   0 sheng     (1000) sheng     (1000)        0 2020-02-13 13:28:36.000000 webssh-1.6.1/tests/data/fonts/.gitignore
--rw-r--r--   0 sheng     (1000) sheng     (1000)        0 2020-02-13 13:28:36.000000 webssh-1.6.1/tests/data/fonts/fake-font
--rw-rw-r--   0 sheng     (1000) sheng     (1000)        0 2022-11-21 08:46:37.000000 webssh-1.6.1/tests/data/host_keys_test.db
--rw-r--r--   0 sheng     (1000) sheng     (1000)       95 2018-10-08 12:17:04.000000 webssh-1.6.1/tests/data/known_hosts_example
--rw-r--r--   0 sheng     (1000) sheng     (1000)       95 2018-09-01 05:48:33.000000 webssh-1.6.1/tests/data/known_hosts_example2
--rw-r--r--   0 sheng     (1000) sheng     (1000)       95 2018-09-01 05:48:33.000000 webssh-1.6.1/tests/data/known_hosts_example3
--rw-r--r--   0 sheng     (1000) sheng     (1000)      432 2018-09-01 05:48:33.000000 webssh-1.6.1/tests/data/test_ed25519.key
--rw-r--r--   0 sheng     (1000) sheng     (1000)      484 2018-09-01 05:48:33.000000 webssh-1.6.1/tests/data/test_ed25519_password.key
--rw-r--r--   0 sheng     (1000) sheng     (1000)       98 2022-11-21 08:45:30.000000 webssh-1.6.1/tests/data/test_known_hosts
--rw-r--r--   0 sheng     (1000) sheng     (1000)     1381 2019-12-14 17:58:28.000000 webssh-1.6.1/tests/data/test_new_dsa.key
--rw-r--r--   0 sheng     (1000) sheng     (1000)     2635 2019-12-14 17:58:28.000000 webssh-1.6.1/tests/data/test_new_rsa_password.key
--rw-r--r--   0 sheng     (1000) sheng     (1000)      883 2018-09-01 05:48:33.000000 webssh-1.6.1/tests/data/test_rsa.key
--rw-r--r--   0 sheng     (1000) sheng     (1000)      951 2018-09-01 05:48:33.000000 webssh-1.6.1/tests/data/test_rsa_password.key
--rw-r--r--   0 sheng     (1000) sheng     (1000)      887 2018-09-01 05:48:33.000000 webssh-1.6.1/tests/data/user_rsa_key
--rw-r--r--   0 sheng     (1000) sheng     (1000)     8028 2019-12-14 17:58:28.000000 webssh-1.6.1/tests/sshserver.py
--rw-r--r--   0 sheng     (1000) sheng     (1000)    30545 2020-10-09 07:47:39.000000 webssh-1.6.1/tests/test_app.py
--rw-rw-r--   0 sheng     (1000) sheng     (1000)    10983 2022-11-21 08:46:18.000000 webssh-1.6.1/tests/test_handler.py
--rw-r--r--   0 sheng     (1000) sheng     (1000)      624 2019-05-17 07:51:35.000000 webssh-1.6.1/tests/test_main.py
--rw-r--r--   0 sheng     (1000) sheng     (1000)     4340 2019-05-17 07:51:35.000000 webssh-1.6.1/tests/test_policy.py
--rw-r--r--   0 sheng     (1000) sheng     (1000)     6946 2020-02-13 13:28:36.000000 webssh-1.6.1/tests/test_settings.py
--rw-r--r--   0 sheng     (1000) sheng     (1000)     4795 2019-09-19 03:14:52.000000 webssh-1.6.1/tests/test_utils.py
--rw-r--r--   0 sheng     (1000) sheng     (1000)     1530 2019-05-17 07:51:35.000000 webssh-1.6.1/tests/utils.py
-drwxrwxr-x   0 sheng     (1000) sheng     (1000)        0 2022-11-21 09:29:08.206756 webssh-1.6.1/webssh/
--rw-r--r--   0 sheng     (1000) sheng     (1000)      323 2020-10-09 07:47:39.000000 webssh-1.6.1/webssh/__init__.py
--rw-rw-r--   0 sheng     (1000) sheng     (1000)       80 2022-11-21 09:10:55.000000 webssh-1.6.1/webssh/_version.py
--rw-rw-r--   0 sheng     (1000) sheng     (1000)    19849 2022-11-21 06:49:55.000000 webssh-1.6.1/webssh/handler.py
--rw-rw-r--   0 sheng     (1000) sheng     (1000)     1839 2022-07-31 07:43:59.000000 webssh-1.6.1/webssh/main.py
--rw-r--r--   0 sheng     (1000) sheng     (1000)     2677 2019-10-06 09:33:29.000000 webssh-1.6.1/webssh/policy.py
--rw-rw-r--   0 sheng     (1000) sheng     (1000)     6576 2022-11-21 03:38:54.000000 webssh-1.6.1/webssh/settings.py
-drwxrwxr-x   0 sheng     (1000) sheng     (1000)        0 2022-11-21 09:29:08.202756 webssh-1.6.1/webssh/static/
-drwxrwxr-x   0 sheng     (1000) sheng     (1000)        0 2022-11-21 09:29:08.206756 webssh-1.6.1/webssh/static/css/
--rw-r--r--   0 sheng     (1000) sheng     (1000)   155758 2019-10-06 09:33:29.000000 webssh-1.6.1/webssh/static/css/bootstrap.min.css
-drwxrwxr-x   0 sheng     (1000) sheng     (1000)        0 2022-11-21 09:29:08.206756 webssh-1.6.1/webssh/static/css/fonts/
--rw-rw-r--   0 sheng     (1000) sheng     (1000)        0 2022-01-28 07:18:40.000000 webssh-1.6.1/webssh/static/css/fonts/.gitignore
--rw-r--r--   0 sheng     (1000) sheng     (1000)      145 2019-10-06 09:33:29.000000 webssh-1.6.1/webssh/static/css/fullscreen.min.css
--rw-r--r--   0 sheng     (1000) sheng     (1000)     1344 2019-12-14 17:58:28.000000 webssh-1.6.1/webssh/static/css/xterm.min.css
-drwxrwxr-x   0 sheng     (1000) sheng     (1000)        0 2022-11-21 09:29:08.206756 webssh-1.6.1/webssh/static/img/
--rw-r--r--   0 sheng     (1000) sheng     (1000)     5953 2019-10-06 09:33:29.000000 webssh-1.6.1/webssh/static/img/favicon.png
-drwxrwxr-x   0 sheng     (1000) sheng     (1000)        0 2022-11-21 09:29:08.206756 webssh-1.6.1/webssh/static/js/
--rw-r--r--   0 sheng     (1000) sheng     (1000)    56292 2019-10-06 09:33:29.000000 webssh-1.6.1/webssh/static/js/bootstrap.min.js
--rw-r--r--   0 sheng     (1000) sheng     (1000)    86927 2019-10-06 09:33:29.000000 webssh-1.6.1/webssh/static/js/jquery.min.js
--rw-rw-r--   0 sheng     (1000) sheng     (1000)    21162 2022-05-29 11:14:51.000000 webssh-1.6.1/webssh/static/js/main.js
--rw-r--r--   0 sheng     (1000) sheng     (1000)    21004 2019-10-06 09:33:29.000000 webssh-1.6.1/webssh/static/js/popper.min.js
--rw-r--r--   0 sheng     (1000) sheng     (1000)     2377 2019-12-14 17:58:28.000000 webssh-1.6.1/webssh/static/js/xterm-addon-fit.min.js
--rw-r--r--   0 sheng     (1000) sheng     (1000)   251949 2019-12-14 17:58:28.000000 webssh-1.6.1/webssh/static/js/xterm.min.js
-drwxrwxr-x   0 sheng     (1000) sheng     (1000)        0 2022-11-21 09:29:08.206756 webssh-1.6.1/webssh/templates/
--rw-rw-r--   0 sheng     (1000) sheng     (1000)     3479 2022-02-17 02:20:51.000000 webssh-1.6.1/webssh/templates/index.html
--rw-r--r--   0 sheng     (1000) sheng     (1000)     2919 2019-12-14 17:58:28.000000 webssh-1.6.1/webssh/utils.py
--rw-rw-r--   0 sheng     (1000) sheng     (1000)     3972 2022-11-21 06:29:17.000000 webssh-1.6.1/webssh/worker.py
-drwxrwxr-x   0 sheng     (1000) sheng     (1000)        0 2022-11-21 09:29:08.206756 webssh-1.6.1/webssh.egg-info/
--rw-rw-r--   0 sheng     (1000) sheng     (1000)     6387 2022-11-21 09:29:08.000000 webssh-1.6.1/webssh.egg-info/PKG-INFO
--rw-rw-r--   0 sheng     (1000) sheng     (1000)     1403 2022-11-21 09:29:08.000000 webssh-1.6.1/webssh.egg-info/SOURCES.txt
--rw-rw-r--   0 sheng     (1000) sheng     (1000)        1 2022-11-21 09:29:08.000000 webssh-1.6.1/webssh.egg-info/dependency_links.txt
--rw-rw-r--   0 sheng     (1000) sheng     (1000)       55 2022-11-21 09:29:08.000000 webssh-1.6.1/webssh.egg-info/entry_points.txt
--rw-rw-r--   0 sheng     (1000) sheng     (1000)       31 2022-11-21 09:29:08.000000 webssh-1.6.1/webssh.egg-info/requires.txt
--rw-rw-r--   0 sheng     (1000) sheng     (1000)        7 2022-11-21 09:29:08.000000 webssh-1.6.1/webssh.egg-info/top_level.txt
+drwxrwxr-x   0 sheng     (1000) sheng     (1000)        0 2023-04-09 06:39:19.585383 webssh-1.6.2/
+-rw-rw-r--   0 sheng     (1000) sheng     (1000)     1079 2017-11-08 13:11:41.000000 webssh-1.6.2/LICENSE
+-rw-r--r--   0 sheng     (1000) sheng     (1000)      241 2018-08-10 07:44:35.000000 webssh-1.6.2/MANIFEST.in
+-rw-rw-r--   0 sheng     (1000) sheng     (1000)     6187 2023-04-09 06:39:19.585383 webssh-1.6.2/PKG-INFO
+-rw-rw-r--   0 sheng     (1000) sheng     (1000)     5213 2023-04-09 06:26:49.000000 webssh-1.6.2/README.md
+-rw-rw-r--   0 sheng     (1000) sheng     (1000)     5650 2023-04-09 06:17:45.000000 webssh-1.6.2/README.rst
+-rw-r--r--   0 sheng     (1000) sheng     (1000)      172 2023-04-09 06:39:19.585383 webssh-1.6.2/setup.cfg
+-rw-rw-r--   0 sheng     (1000) sheng     (1000)      983 2023-04-09 06:17:45.000000 webssh-1.6.2/setup.py
+drwxrwxr-x   0 sheng     (1000) sheng     (1000)        0 2023-04-09 06:39:19.561385 webssh-1.6.2/tests/
+-rw-r--r--   0 sheng     (1000) sheng     (1000)        0 2018-05-06 13:10:34.000000 webssh-1.6.2/tests/__init__.py
+drwxrwxr-x   0 sheng     (1000) sheng     (1000)        0 2023-04-09 06:39:19.565385 webssh-1.6.2/tests/data/
+-rw-r--r--   0 sheng     (1000) sheng     (1000)     1233 2019-05-17 07:51:35.000000 webssh-1.6.2/tests/data/cert.crt
+-rw-r--r--   0 sheng     (1000) sheng     (1000)     1704 2019-05-17 07:51:35.000000 webssh-1.6.2/tests/data/cert.key
+drwxrwxr-x   0 sheng     (1000) sheng     (1000)        0 2023-04-09 06:39:19.565385 webssh-1.6.2/tests/data/fonts/
+-rw-r--r--   0 sheng     (1000) sheng     (1000)        0 2020-02-13 13:28:36.000000 webssh-1.6.2/tests/data/fonts/.gitignore
+-rw-r--r--   0 sheng     (1000) sheng     (1000)        0 2020-02-13 13:28:36.000000 webssh-1.6.2/tests/data/fonts/fake-font
+-rw-rw-r--   0 sheng     (1000) sheng     (1000)        0 2023-02-28 11:23:44.000000 webssh-1.6.2/tests/data/host_keys_test.db
+-rw-r--r--   0 sheng     (1000) sheng     (1000)       95 2018-10-08 12:17:04.000000 webssh-1.6.2/tests/data/known_hosts_example
+-rw-r--r--   0 sheng     (1000) sheng     (1000)       95 2018-09-01 05:48:33.000000 webssh-1.6.2/tests/data/known_hosts_example2
+-rw-r--r--   0 sheng     (1000) sheng     (1000)       95 2018-09-01 05:48:33.000000 webssh-1.6.2/tests/data/known_hosts_example3
+-rw-r--r--   0 sheng     (1000) sheng     (1000)      432 2018-09-01 05:48:33.000000 webssh-1.6.2/tests/data/test_ed25519.key
+-rw-r--r--   0 sheng     (1000) sheng     (1000)      484 2018-09-01 05:48:33.000000 webssh-1.6.2/tests/data/test_ed25519_password.key
+-rw-r--r--   0 sheng     (1000) sheng     (1000)       98 2023-02-27 13:28:49.000000 webssh-1.6.2/tests/data/test_known_hosts
+-rw-r--r--   0 sheng     (1000) sheng     (1000)     1381 2019-12-14 17:58:28.000000 webssh-1.6.2/tests/data/test_new_dsa.key
+-rw-r--r--   0 sheng     (1000) sheng     (1000)     2635 2019-12-14 17:58:28.000000 webssh-1.6.2/tests/data/test_new_rsa_password.key
+-rw-r--r--   0 sheng     (1000) sheng     (1000)      883 2018-09-01 05:48:33.000000 webssh-1.6.2/tests/data/test_rsa.key
+-rw-r--r--   0 sheng     (1000) sheng     (1000)      951 2018-09-01 05:48:33.000000 webssh-1.6.2/tests/data/test_rsa_password.key
+-rw-r--r--   0 sheng     (1000) sheng     (1000)      887 2018-09-01 05:48:33.000000 webssh-1.6.2/tests/data/user_rsa_key
+-rw-rw-r--   0 sheng     (1000) sheng     (1000)     7190 2023-04-09 06:17:45.000000 webssh-1.6.2/tests/sshserver.py
+-rw-r--r--   0 sheng     (1000) sheng     (1000)    30545 2020-10-09 07:47:39.000000 webssh-1.6.2/tests/test_app.py
+-rw-rw-r--   0 sheng     (1000) sheng     (1000)    11875 2023-04-09 06:17:45.000000 webssh-1.6.2/tests/test_handler.py
+-rw-r--r--   0 sheng     (1000) sheng     (1000)      624 2019-05-17 07:51:35.000000 webssh-1.6.2/tests/test_main.py
+-rw-r--r--   0 sheng     (1000) sheng     (1000)     4340 2019-05-17 07:51:35.000000 webssh-1.6.2/tests/test_policy.py
+-rw-r--r--   0 sheng     (1000) sheng     (1000)     6946 2020-02-13 13:28:36.000000 webssh-1.6.2/tests/test_settings.py
+-rw-r--r--   0 sheng     (1000) sheng     (1000)     4795 2019-09-19 03:14:52.000000 webssh-1.6.2/tests/test_utils.py
+-rw-r--r--   0 sheng     (1000) sheng     (1000)     1530 2019-05-17 07:51:35.000000 webssh-1.6.2/tests/utils.py
+drwxrwxr-x   0 sheng     (1000) sheng     (1000)        0 2023-04-09 06:39:19.565385 webssh-1.6.2/webssh/
+-rw-r--r--   0 sheng     (1000) sheng     (1000)      323 2020-10-09 07:47:39.000000 webssh-1.6.2/webssh/__init__.py
+-rw-rw-r--   0 sheng     (1000) sheng     (1000)       80 2023-04-09 06:35:52.000000 webssh-1.6.2/webssh/_version.py
+-rw-rw-r--   0 sheng     (1000) sheng     (1000)    19849 2023-04-09 06:17:45.000000 webssh-1.6.2/webssh/handler.py
+-rw-rw-r--   0 sheng     (1000) sheng     (1000)     1839 2023-04-09 06:17:45.000000 webssh-1.6.2/webssh/main.py
+-rw-r--r--   0 sheng     (1000) sheng     (1000)     2677 2019-10-06 09:33:29.000000 webssh-1.6.2/webssh/policy.py
+-rw-rw-r--   0 sheng     (1000) sheng     (1000)     6576 2023-04-09 06:17:45.000000 webssh-1.6.2/webssh/settings.py
+drwxrwxr-x   0 sheng     (1000) sheng     (1000)        0 2023-04-09 06:39:19.557386 webssh-1.6.2/webssh/static/
+drwxrwxr-x   0 sheng     (1000) sheng     (1000)        0 2023-04-09 06:39:19.573384 webssh-1.6.2/webssh/static/css/
+-rw-r--r--   0 sheng     (1000) sheng     (1000)   155758 2019-10-06 09:33:29.000000 webssh-1.6.2/webssh/static/css/bootstrap.min.css
+drwxrwxr-x   0 sheng     (1000) sheng     (1000)        0 2023-04-09 06:39:19.573384 webssh-1.6.2/webssh/static/css/fonts/
+-rw-rw-r--   0 sheng     (1000) sheng     (1000)        0 2022-01-28 07:18:40.000000 webssh-1.6.2/webssh/static/css/fonts/.gitignore
+-rw-r--r--   0 sheng     (1000) sheng     (1000)      145 2019-10-06 09:33:29.000000 webssh-1.6.2/webssh/static/css/fullscreen.min.css
+-rw-r--r--   0 sheng     (1000) sheng     (1000)     1344 2019-12-14 17:58:28.000000 webssh-1.6.2/webssh/static/css/xterm.min.css
+drwxrwxr-x   0 sheng     (1000) sheng     (1000)        0 2023-04-09 06:39:19.573384 webssh-1.6.2/webssh/static/img/
+-rw-r--r--   0 sheng     (1000) sheng     (1000)     5953 2019-10-06 09:33:29.000000 webssh-1.6.2/webssh/static/img/favicon.png
+drwxrwxr-x   0 sheng     (1000) sheng     (1000)        0 2023-04-09 06:39:19.581384 webssh-1.6.2/webssh/static/js/
+-rw-r--r--   0 sheng     (1000) sheng     (1000)    56292 2019-10-06 09:33:29.000000 webssh-1.6.2/webssh/static/js/bootstrap.min.js
+-rw-r--r--   0 sheng     (1000) sheng     (1000)    86927 2019-10-06 09:33:29.000000 webssh-1.6.2/webssh/static/js/jquery.min.js
+-rw-rw-r--   0 sheng     (1000) sheng     (1000)    21162 2022-05-29 11:14:51.000000 webssh-1.6.2/webssh/static/js/main.js
+-rw-r--r--   0 sheng     (1000) sheng     (1000)    21004 2019-10-06 09:33:29.000000 webssh-1.6.2/webssh/static/js/popper.min.js
+-rw-r--r--   0 sheng     (1000) sheng     (1000)     2377 2019-12-14 17:58:28.000000 webssh-1.6.2/webssh/static/js/xterm-addon-fit.min.js
+-rw-r--r--   0 sheng     (1000) sheng     (1000)   251949 2019-12-14 17:58:28.000000 webssh-1.6.2/webssh/static/js/xterm.min.js
+drwxrwxr-x   0 sheng     (1000) sheng     (1000)        0 2023-04-09 06:39:19.585383 webssh-1.6.2/webssh/templates/
+-rw-rw-r--   0 sheng     (1000) sheng     (1000)     3479 2022-02-17 02:20:51.000000 webssh-1.6.2/webssh/templates/index.html
+-rw-rw-r--   0 sheng     (1000) sheng     (1000)     2963 2023-04-09 06:17:45.000000 webssh-1.6.2/webssh/utils.py
+-rw-rw-r--   0 sheng     (1000) sheng     (1000)     3972 2023-04-09 06:17:45.000000 webssh-1.6.2/webssh/worker.py
+drwxrwxr-x   0 sheng     (1000) sheng     (1000)        0 2023-04-09 06:39:19.565385 webssh-1.6.2/webssh.egg-info/
+-rw-rw-r--   0 sheng     (1000) sheng     (1000)     6187 2023-04-09 06:39:19.000000 webssh-1.6.2/webssh.egg-info/PKG-INFO
+-rw-rw-r--   0 sheng     (1000) sheng     (1000)     1403 2023-04-09 06:39:19.000000 webssh-1.6.2/webssh.egg-info/SOURCES.txt
+-rw-rw-r--   0 sheng     (1000) sheng     (1000)        1 2023-04-09 06:39:19.000000 webssh-1.6.2/webssh.egg-info/dependency_links.txt
+-rw-rw-r--   0 sheng     (1000) sheng     (1000)       55 2023-04-09 06:39:19.000000 webssh-1.6.2/webssh.egg-info/entry_points.txt
+-rw-rw-r--   0 sheng     (1000) sheng     (1000)       31 2023-04-09 06:39:19.000000 webssh-1.6.2/webssh.egg-info/requires.txt
+-rw-rw-r--   0 sheng     (1000) sheng     (1000)        7 2023-04-09 06:39:19.000000 webssh-1.6.2/webssh.egg-info/top_level.txt
```

### Comparing `webssh-1.6.1/LICENSE` & `webssh-1.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `webssh-1.6.1/PKG-INFO` & `webssh-1.6.2/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,26 +1,22 @@
 Metadata-Version: 2.1
 Name: webssh
-Version: 1.6.1
+Version: 1.6.2
 Summary: Web based ssh client
 Home-page: https://github.com/huashengdun/webssh
 Author: Shengdun Hua
 Author-email: webmaster0115@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 2
-Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.4
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 License-File: LICENSE
 
 WebSSH
 ------
 
 |Build Status| |codecov| |PyPI - Python Version| |PyPI|
 
@@ -58,15 +54,15 @@
     +---------+     http     +--------+    ssh    +-----------+
     | browser | <==========> | webssh | <=======> | ssh server|
     +---------+   websocket  +--------+    ssh    +-----------+
 
 Requirements
 ~~~~~~~~~~~~
 
--  Python 2.7/3.4+
+-  Python 3.8+
 
 Quickstart
 ~~~~~~~~~~
 
 1. Install this app, run command ``pip install webssh``
 2. Start a webserver, run command ``wssh``
 3. Open your browser, navigate to ``127.0.0.1:8888``
```

### Comparing `webssh-1.6.1/README.md` & `webssh-1.6.2/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ## WebSSH
 
-[![Build Status](https://travis-ci.org/huashengdun/webssh.svg?branch=master)](https://travis-ci.org/huashengdun/webssh)
-[![codecov](https://codecov.io/gh/huashengdun/webssh/branch/master/graph/badge.svg)](https://codecov.io/gh/huashengdun/webssh)
+[![python](https://github.com/huashengdun/webssh/actions/workflows/python.yml/badge.svg)](https://github.com/huashengdun/webssh/actions/workflows/python.yml)
+[![codecov](https://raw.githubusercontent.com/huashengdun/webssh/coverage-badge/coverage.svg)](https://raw.githubusercontent.com/huashengdun/webssh/coverage-badge/coverage.svg)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/webssh.svg)
 ![PyPI](https://img.shields.io/pypi/v/webssh.svg)
 
 
 ### Introduction
 
 A simple web application to be used as an ssh client to connect to your ssh servers. It is written in Python, base on tornado, paramiko and xterm.js.
@@ -33,15 +33,15 @@
 +---------+     http     +--------+    ssh    +-----------+
 | browser | <==========> | webssh | <=======> | ssh server|
 +---------+   websocket  +--------+    ssh    +-----------+
 ```
 
 ### Requirements
 
-* Python 2.7/3.4+
+* Python 3.8+
 
 
 ### Quickstart
 
 1. Install this app, run command `pip install webssh`
 2. Start a webserver, run command `wssh`
 3. Open your browser, navigate to `127.0.0.1:8888`
```

### Comparing `webssh-1.6.1/README.rst` & `webssh-1.6.2/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -37,15 +37,15 @@
     +---------+     http     +--------+    ssh    +-----------+
     | browser | <==========> | webssh | <=======> | ssh server|
     +---------+   websocket  +--------+    ssh    +-----------+
 
 Requirements
 ~~~~~~~~~~~~
 
--  Python 2.7/3.4+
+-  Python 3.8+
 
 Quickstart
 ~~~~~~~~~~
 
 1. Install this app, run command ``pip install webssh``
 2. Start a webserver, run command ``wssh``
 3. Open your browser, navigate to ``127.0.0.1:8888``
```

### Comparing `webssh-1.6.1/setup.py` & `webssh-1.6.2/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -20,22 +20,18 @@
     [console_scripts]
     wssh = webssh.main:main
     ''',
     license='MIT',
     include_package_data=True,
     classifiers=[
         'Programming Language :: Python',
-        'Programming Language :: Python :: 2',
-        'Programming Language :: Python :: 2.7',
         'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.4',
-        'Programming Language :: Python :: 3.5',
-        'Programming Language :: Python :: 3.6',
-        'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
+        'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
     ],
     install_requires=[
         'tornado>=4.5.0',
         'paramiko>=2.3.1',
     ],
 )
```

### Comparing `webssh-1.6.1/tests/data/cert.crt` & `webssh-1.6.2/tests/data/cert.crt`

 * *Files identical despite different names*

### Comparing `webssh-1.6.1/tests/data/cert.key` & `webssh-1.6.2/tests/data/cert.key`

 * *Files identical despite different names*

### Comparing `webssh-1.6.1/tests/data/test_new_dsa.key` & `webssh-1.6.2/tests/data/test_new_dsa.key`

 * *Files identical despite different names*

### Comparing `webssh-1.6.1/tests/data/test_new_rsa_password.key` & `webssh-1.6.2/tests/data/test_new_rsa_password.key`

 * *Files identical despite different names*

### Comparing `webssh-1.6.1/tests/data/test_rsa.key` & `webssh-1.6.2/tests/data/test_rsa.key`

 * *Files identical despite different names*

### Comparing `webssh-1.6.1/tests/data/test_rsa_password.key` & `webssh-1.6.2/tests/data/test_rsa_password.key`

 * *Files identical despite different names*

### Comparing `webssh-1.6.1/tests/data/user_rsa_key` & `webssh-1.6.2/tests/data/user_rsa_key`

 * *Files identical despite different names*

### Comparing `webssh-1.6.1/tests/sshserver.py` & `webssh-1.6.2/tests/sshserver.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,59 +1,39 @@
-#!/usr/bin/env python
-
-# Copyright (C) 2003-2007  Robey Pointer <robeypointer@gmail.com>
-#
-# This file is part of paramiko.
-#
-# Paramiko is free software; you can redistribute it and/or modify it under the
-# terms of the GNU Lesser General Public License as published by the Free
-# Software Foundation; either version 2.1 of the License, or (at your option)
-# any later version.
-#
-# Paramiko is distributed in the hope that it will be useful, but WITHOUT ANY
-# WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR
-# A PARTICULAR PURPOSE.  See the GNU Lesser General Public License for more
-# details.
-#
-# You should have received a copy of the GNU Lesser General Public License
-# along with Paramiko; if not, write to the Free Software Foundation, Inc.,
-# 59 Temple Place, Suite 330, Boston, MA  02111-1307  USA.
-
+import base64
 import random
 import socket
 # import sys
 import threading
 # import traceback
 import paramiko
 
 from binascii import hexlify
-from paramiko.py3compat import u, decodebytes
 from tests.utils import make_tests_data_path
 
 
 # setup logging
 paramiko.util.log_to_file(make_tests_data_path('sshserver.log'))
 
 host_key = paramiko.RSAKey(filename=make_tests_data_path('test_rsa.key'))
 # host_key = paramiko.DSSKey(filename='test_dss.key')
 
-print('Read key: ' + u(hexlify(host_key.get_fingerprint())))
+print('Read key: ' + hexlify(host_key.get_fingerprint()).decode('utf-8'))
 
 banner = u'\r\n\u6b22\u8fce\r\n'
 event_timeout = 5
 
 
 class Server(paramiko.ServerInterface):
     # 'data' is the output of base64.b64encode(key)
     # (using the "user_rsa_key" files)
     data = (b'AAAAB3NzaC1yc2EAAAABIwAAAIEAyO4it3fHlmGZWJaGrfeHOVY7RWO3P9M7hp'
             b'fAu7jJ2d7eothvfeuoRFtJwhUmZDluRdFyhFY/hFAh76PJKGAusIqIQKlkJxMC'
             b'KDqIexkgHAfID/6mqvmnSJf0b5W8v5h2pI/stOSwTQ+pxVhwJ9ctYDhRSlF0iT'
             b'UWT10hcuO4Ks8=')
-    good_pub_key = paramiko.RSAKey(data=decodebytes(data))
+    good_pub_key = paramiko.RSAKey(data=base64.decodebytes(data))
 
     commands = [
         b'$SHELL -ilc "locale charmap"',
         b'$SHELL -ic "locale charmap"'
     ]
     encodings = ['UTF-8', 'GBK', 'UTF-8\r\n', 'GBK\r\n']
 
@@ -78,15 +58,15 @@
     def check_auth_password(self, username, password):
         print('Auth attempt with username: {!r} & password: {!r}'.format(username, password)) # noqa
         if (username in ['robey', 'bar', 'foo']) and (password == 'foo'):
             return paramiko.AUTH_SUCCESSFUL
         return paramiko.AUTH_FAILED
 
     def check_auth_publickey(self, username, key):
-        print('Auth attempt with username: {!r} & key: {!r}'.format(username, u(hexlify(key.get_fingerprint())))) # noqa
+        print('Auth attempt with username: {!r} & key: {!r}'.format(username, hexlify(key.get_fingerprint()).decode('utf-8'))) # noqa
         if (username in ['robey', 'keyonly']) and (key == self.good_pub_key):
             return paramiko.AUTH_SUCCESSFUL
         if username == 'pkey2fa' and key == self.good_pub_key:
             self.key_verified = True
             return paramiko.AUTH_PARTIALLY_SUCCESSFUL
         return paramiko.AUTH_FAILED
```

### Comparing `webssh-1.6.1/tests/test_app.py` & `webssh-1.6.2/tests/test_app.py`

 * *Files identical despite different names*

### Comparing `webssh-1.6.1/tests/test_handler.py` & `webssh-1.6.2/tests/test_handler.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,17 +1,18 @@
+import io
 import unittest
 import paramiko
 
 from tornado.httputil import HTTPServerRequest
 from tornado.options import options
 from tests.utils import read_file, make_tests_data_path
 from webssh import handler
 from webssh import worker
 from webssh.handler import (
-    MixinHandler, WsockHandler, PrivateKey, InvalidValueError
+    IndexHandler, MixinHandler, WsockHandler, PrivateKey, InvalidValueError, SSHClient
 )
 
 try:
     from unittest.mock import Mock
 except ImportError:
     from mock import Mock
 
@@ -311,7 +312,29 @@
             def __call__(self):
                 return Worker()
 
         ref = FakeWeakRef()
         obj.worker_ref = ref
         WsockHandler.on_message(obj, b'{"data": "somestuff"}')
         obj.close.assert_called_with(reason='Worker closed')
+
+class TestIndexHandler(unittest.TestCase):
+    def test_null_in_encoding(self):
+        handler = Mock(spec=IndexHandler)
+
+        # This is a little nasty, but the index handler has a lot of
+        # dependencies to mock. Mocking out everything but the bits
+        # we want to test lets us test this case without needing to
+        # refactor the relevant code out of IndexHandler
+        def parse_encoding(data):
+            return IndexHandler.parse_encoding(handler, data)
+        handler.parse_encoding = parse_encoding
+
+        ssh = Mock(spec=SSHClient)
+        stdin = io.BytesIO()
+        stdout = io.BytesIO(initial_bytes=b"UTF-8\0")
+        stderr = io.BytesIO()
+        ssh.exec_command.return_value = (stdin, stdout, stderr)
+
+        encoding = IndexHandler.get_default_encoding(handler, ssh)
+        self.assertEquals("utf-8", encoding)
+
```

### Comparing `webssh-1.6.1/tests/test_main.py` & `webssh-1.6.2/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `webssh-1.6.1/tests/test_policy.py` & `webssh-1.6.2/tests/test_policy.py`

 * *Files identical despite different names*

### Comparing `webssh-1.6.1/tests/test_settings.py` & `webssh-1.6.2/tests/test_settings.py`

 * *Files identical despite different names*

### Comparing `webssh-1.6.1/tests/test_utils.py` & `webssh-1.6.2/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `webssh-1.6.1/tests/utils.py` & `webssh-1.6.2/tests/utils.py`

 * *Files identical despite different names*

### Comparing `webssh-1.6.1/webssh/handler.py` & `webssh-1.6.2/webssh/handler.py`

 * *Files identical despite different names*

### Comparing `webssh-1.6.1/webssh/main.py` & `webssh-1.6.2/webssh/main.py`

 * *Files identical despite different names*

### Comparing `webssh-1.6.1/webssh/policy.py` & `webssh-1.6.2/webssh/policy.py`

 * *Files identical despite different names*

### Comparing `webssh-1.6.1/webssh/settings.py` & `webssh-1.6.2/webssh/settings.py`

 * *Files identical despite different names*

### Comparing `webssh-1.6.1/webssh/static/css/bootstrap.min.css` & `webssh-1.6.2/webssh/static/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `webssh-1.6.1/webssh/static/css/xterm.min.css` & `webssh-1.6.2/webssh/static/css/xterm.min.css`

 * *Files identical despite different names*

### Comparing `webssh-1.6.1/webssh/static/img/favicon.png` & `webssh-1.6.2/webssh/static/img/favicon.png`

 * *Files identical despite different names*

### Comparing `webssh-1.6.1/webssh/static/js/bootstrap.min.js` & `webssh-1.6.2/webssh/static/js/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `webssh-1.6.1/webssh/static/js/jquery.min.js` & `webssh-1.6.2/webssh/static/js/jquery.min.js`

 * *Files identical despite different names*

### Comparing `webssh-1.6.1/webssh/static/js/main.js` & `webssh-1.6.2/webssh/static/js/main.js`

 * *Files identical despite different names*

### Comparing `webssh-1.6.1/webssh/static/js/popper.min.js` & `webssh-1.6.2/webssh/static/js/popper.min.js`

 * *Files identical despite different names*

### Comparing `webssh-1.6.1/webssh/static/js/xterm-addon-fit.min.js` & `webssh-1.6.2/webssh/static/js/xterm-addon-fit.min.js`

 * *Files identical despite different names*

### Comparing `webssh-1.6.1/webssh/static/js/xterm.min.js` & `webssh-1.6.2/webssh/static/js/xterm.min.js`

 * *Files identical despite different names*

### Comparing `webssh-1.6.1/webssh/templates/index.html` & `webssh-1.6.2/webssh/templates/index.html`

 * *Files identical despite different names*

### Comparing `webssh-1.6.1/webssh/utils.py` & `webssh-1.6.2/webssh/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,14 +55,16 @@
 
 
 def is_valid_encoding(encoding):
     try:
         u'test'.encode(encoding)
     except LookupError:
         return False
+    except ValueError:
+        return False
     return True
 
 
 def is_ip_hostname(hostname):
     it = iter(hostname)
     if next(it) == '[':
         return True
```

### Comparing `webssh-1.6.1/webssh/worker.py` & `webssh-1.6.2/webssh/worker.py`

 * *Files identical despite different names*

### Comparing `webssh-1.6.1/webssh.egg-info/PKG-INFO` & `webssh-1.6.2/webssh.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,26 +1,22 @@
 Metadata-Version: 2.1
 Name: webssh
-Version: 1.6.1
+Version: 1.6.2
 Summary: Web based ssh client
 Home-page: https://github.com/huashengdun/webssh
 Author: Shengdun Hua
 Author-email: webmaster0115@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 2
-Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.4
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 License-File: LICENSE
 
 WebSSH
 ------
 
 |Build Status| |codecov| |PyPI - Python Version| |PyPI|
 
@@ -58,15 +54,15 @@
     +---------+     http     +--------+    ssh    +-----------+
     | browser | <==========> | webssh | <=======> | ssh server|
     +---------+   websocket  +--------+    ssh    +-----------+
 
 Requirements
 ~~~~~~~~~~~~
 
--  Python 2.7/3.4+
+-  Python 3.8+
 
 Quickstart
 ~~~~~~~~~~
 
 1. Install this app, run command ``pip install webssh``
 2. Start a webserver, run command ``wssh``
 3. Open your browser, navigate to ``127.0.0.1:8888``
```

### Comparing `webssh-1.6.1/webssh.egg-info/SOURCES.txt` & `webssh-1.6.2/webssh.egg-info/SOURCES.txt`

 * *Files identical despite different names*

