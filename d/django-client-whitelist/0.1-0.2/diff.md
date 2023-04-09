# Comparing `tmp/django-client-whitelist-0.1.tar.gz` & `tmp/django-client-whitelist-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-client-whitelist-0.1.tar", last modified: Sun Apr  9 15:56:23 2023, max compression
+gzip compressed data, was "django-client-whitelist-0.2.tar", last modified: Sun Apr  9 20:02:42 2023, max compression
```

## Comparing `django-client-whitelist-0.1.tar` & `django-client-whitelist-0.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 saidi     (1000) saidi     (1000)        0 2023-04-09 15:56:23.720129 django-client-whitelist-0.1/
--rw-rw-r--   0 saidi     (1000) saidi     (1000)     1026 2023-04-09 15:53:50.000000 django-client-whitelist-0.1/LICENSE
--rw-rw-r--   0 saidi     (1000) saidi     (1000)       74 2023-04-09 13:32:27.000000 django-client-whitelist-0.1/MANIFEST.in
--rw-rw-r--   0 saidi     (1000) saidi     (1000)      755 2023-04-09 15:56:23.720129 django-client-whitelist-0.1/PKG-INFO
--rw-rw-r--   0 saidi     (1000) saidi     (1000)     2377 2023-04-09 15:51:25.000000 django-client-whitelist-0.1/README.md
-drwxrwxr-x   0 saidi     (1000) saidi     (1000)        0 2023-04-09 15:56:23.720129 django-client-whitelist-0.1/client_whitelist/
--rw-rw-r--   0 saidi     (1000) saidi     (1000)        0 2023-04-09 13:24:54.000000 django-client-whitelist-0.1/client_whitelist/__init__.py
--rw-rw-r--   0 saidi     (1000) saidi     (1000)      163 2023-04-09 13:24:54.000000 django-client-whitelist-0.1/client_whitelist/apps.py
--rw-rw-r--   0 saidi     (1000) saidi     (1000)     1726 2023-04-09 15:39:52.000000 django-client-whitelist-0.1/client_whitelist/middleware.py
-drwxrwxr-x   0 saidi     (1000) saidi     (1000)        0 2023-04-09 15:56:23.720129 django-client-whitelist-0.1/django_client_whitelist.egg-info/
--rw-rw-r--   0 saidi     (1000) saidi     (1000)      755 2023-04-09 15:56:23.000000 django-client-whitelist-0.1/django_client_whitelist.egg-info/PKG-INFO
--rw-rw-r--   0 saidi     (1000) saidi     (1000)      357 2023-04-09 15:56:23.000000 django-client-whitelist-0.1/django_client_whitelist.egg-info/SOURCES.txt
--rw-rw-r--   0 saidi     (1000) saidi     (1000)        1 2023-04-09 15:56:23.000000 django-client-whitelist-0.1/django_client_whitelist.egg-info/dependency_links.txt
--rw-rw-r--   0 saidi     (1000) saidi     (1000)       14 2023-04-09 15:56:23.000000 django-client-whitelist-0.1/django_client_whitelist.egg-info/requires.txt
--rw-rw-r--   0 saidi     (1000) saidi     (1000)       17 2023-04-09 15:56:23.000000 django-client-whitelist-0.1/django_client_whitelist.egg-info/top_level.txt
--rw-rw-r--   0 saidi     (1000) saidi     (1000)       38 2023-04-09 15:56:23.720129 django-client-whitelist-0.1/setup.cfg
--rw-rw-r--   0 saidi     (1000) saidi     (1000)      894 2023-04-09 13:46:08.000000 django-client-whitelist-0.1/setup.py
+drwxrwxr-x   0 saidi     (1000) saidi     (1000)        0 2023-04-09 20:02:42.485395 django-client-whitelist-0.2/
+-rw-rw-r--   0 saidi     (1000) saidi     (1000)     1026 2023-04-09 15:53:50.000000 django-client-whitelist-0.2/LICENSE
+-rw-rw-r--   0 saidi     (1000) saidi     (1000)       74 2023-04-09 13:32:27.000000 django-client-whitelist-0.2/MANIFEST.in
+-rw-rw-r--   0 saidi     (1000) saidi     (1000)     3173 2023-04-09 20:02:42.485395 django-client-whitelist-0.2/PKG-INFO
+-rw-rw-r--   0 saidi     (1000) saidi     (1000)     2377 2023-04-09 15:51:25.000000 django-client-whitelist-0.2/README.md
+drwxrwxr-x   0 saidi     (1000) saidi     (1000)        0 2023-04-09 20:02:42.485395 django-client-whitelist-0.2/client_whitelist/
+-rw-rw-r--   0 saidi     (1000) saidi     (1000)        0 2023-04-09 13:24:54.000000 django-client-whitelist-0.2/client_whitelist/__init__.py
+-rw-rw-r--   0 saidi     (1000) saidi     (1000)      163 2023-04-09 13:24:54.000000 django-client-whitelist-0.2/client_whitelist/apps.py
+-rw-rw-r--   0 saidi     (1000) saidi     (1000)     1726 2023-04-09 15:39:52.000000 django-client-whitelist-0.2/client_whitelist/middleware.py
+drwxrwxr-x   0 saidi     (1000) saidi     (1000)        0 2023-04-09 20:02:42.485395 django-client-whitelist-0.2/django_client_whitelist.egg-info/
+-rw-rw-r--   0 saidi     (1000) saidi     (1000)     3173 2023-04-09 20:02:42.000000 django-client-whitelist-0.2/django_client_whitelist.egg-info/PKG-INFO
+-rw-rw-r--   0 saidi     (1000) saidi     (1000)      357 2023-04-09 20:02:42.000000 django-client-whitelist-0.2/django_client_whitelist.egg-info/SOURCES.txt
+-rw-rw-r--   0 saidi     (1000) saidi     (1000)        1 2023-04-09 20:02:42.000000 django-client-whitelist-0.2/django_client_whitelist.egg-info/dependency_links.txt
+-rw-rw-r--   0 saidi     (1000) saidi     (1000)       14 2023-04-09 20:02:42.000000 django-client-whitelist-0.2/django_client_whitelist.egg-info/requires.txt
+-rw-rw-r--   0 saidi     (1000) saidi     (1000)       17 2023-04-09 20:02:42.000000 django-client-whitelist-0.2/django_client_whitelist.egg-info/top_level.txt
+-rw-rw-r--   0 saidi     (1000) saidi     (1000)       38 2023-04-09 20:02:42.489395 django-client-whitelist-0.2/setup.cfg
+-rw-rw-r--   0 saidi     (1000) saidi     (1000)     1111 2023-04-09 20:02:04.000000 django-client-whitelist-0.2/setup.py
```

### Comparing `django-client-whitelist-0.1/LICENSE` & `django-client-whitelist-0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `django-client-whitelist-0.1/README.md` & `django-client-whitelist-0.2/README.md`

 * *Files identical despite different names*

### Comparing `django-client-whitelist-0.1/client_whitelist/middleware.py` & `django-client-whitelist-0.2/client_whitelist/middleware.py`

 * *Files identical despite different names*

### Comparing `django-client-whitelist-0.1/setup.py` & `django-client-whitelist-0.2/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,19 +1,25 @@
 from setuptools import setup
+from pathlib import Path
+
+this_directory = Path(__file__).parent
+long_description = (this_directory / "README.md").read_text()
 
 setup(
     name='django-client-whitelist',
-    version='0.1',
+    version='0.2',
     packages=['client_whitelist'],
     python_requires='>=3.10.7',
     install_requires=[
         'Django>=4.1.4',
     ],
     license='MIT',
     description='Django app to restrict client access',
+    long_description=long_description,
+    long_description_content_type='text/markdown',
     url='https://github.com/S-Amine/django-client-whitelist.git',
     author='S-Amine',
     classifiers=[
         'Environment :: Web Environment',
         'Framework :: Django',
         'Framework :: Django :: 4.1',
         'Intended Audience :: Developers',
```

