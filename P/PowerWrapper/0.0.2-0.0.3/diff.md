# Comparing `tmp/PowerWrapper-0.0.2.tar.gz` & `tmp/PowerWrapper-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PowerWrapper-0.0.2.tar", last modified: Tue Oct 11 08:37:54 2022, max compression
+gzip compressed data, was "PowerWrapper-0.0.3.tar", last modified: Sun Apr  9 11:50:09 2023, max compression
```

## Comparing `PowerWrapper-0.0.2.tar` & `PowerWrapper-0.0.3.tar`

### file list

```diff
@@ -1,18 +1,10 @@
-drwxrwxrwx   0        0        0        0 2022-10-11 08:37:54.143908 PowerWrapper-0.0.2/
--rw-rw-rw-   0        0        0      107 2022-10-11 08:36:33.000000 PowerWrapper-0.0.2/CHANGELOG.txt
--rw-rw-rw-   0        0        0     1652 2022-10-10 11:35:28.000000 PowerWrapper-0.0.2/LICENSE.txt
--rw-rw-rw-   0        0        0       25 2022-10-10 11:39:34.000000 PowerWrapper-0.0.2/MANIFEST.in
--rw-rw-rw-   0        0        0      660 2022-10-11 08:37:54.143908 PowerWrapper-0.0.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2022-10-11 08:37:54.122312 PowerWrapper-0.0.2/PowerWrapper/
--rw-rw-rw-   0        0        0     2103 2022-10-10 11:08:49.000000 PowerWrapper-0.0.2/PowerWrapper/System.py
--rw-rw-rw-   0        0        0       66 2022-10-10 11:08:02.000000 PowerWrapper-0.0.2/PowerWrapper/__init__.py
--rw-rw-rw-   0        0        0     1197 2022-10-10 11:10:23.000000 PowerWrapper-0.0.2/PowerWrapper/errors.py
--rw-rw-rw-   0        0        0     1274 2022-10-10 11:09:23.000000 PowerWrapper-0.0.2/PowerWrapper/maths.py
-drwxrwxrwx   0        0        0        0 2022-10-11 08:37:54.142902 PowerWrapper-0.0.2/PowerWrapper.egg-info/
--rw-rw-rw-   0        0        0      660 2022-10-11 08:37:54.000000 PowerWrapper-0.0.2/PowerWrapper.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      294 2022-10-11 08:37:54.000000 PowerWrapper-0.0.2/PowerWrapper.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-10-11 08:37:54.000000 PowerWrapper-0.0.2/PowerWrapper.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2022-10-11 08:37:54.000000 PowerWrapper-0.0.2/PowerWrapper.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        0 2022-10-10 11:32:55.000000 PowerWrapper-0.0.2/README.txt
--rw-rw-rw-   0        0        0       42 2022-10-11 08:37:54.143908 PowerWrapper-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0      715 2022-10-11 08:36:45.000000 PowerWrapper-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-09 11:50:09.404141 PowerWrapper-0.0.3/
+-rw-rw-rw-   0        0        0      646 2023-04-09 11:50:09.403632 PowerWrapper-0.0.3/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-09 11:50:09.401170 PowerWrapper-0.0.3/PowerWrapper.egg-info/
+-rw-rw-rw-   0        0        0      646 2023-04-09 11:50:09.000000 PowerWrapper-0.0.3/PowerWrapper.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      163 2023-04-09 11:50:09.000000 PowerWrapper-0.0.3/PowerWrapper.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-09 11:50:09.000000 PowerWrapper-0.0.3/PowerWrapper.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        1 2023-04-09 11:50:09.000000 PowerWrapper-0.0.3/PowerWrapper.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       49 2023-04-09 11:48:50.000000 PowerWrapper-0.0.3/README.txt
+-rw-rw-rw-   0        0        0       42 2023-04-09 11:50:09.404141 PowerWrapper-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      716 2023-04-09 11:49:21.000000 PowerWrapper-0.0.3/setup.py
```

### Comparing `PowerWrapper-0.0.2/setup.py` & `PowerWrapper-0.0.3/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -6,16 +6,16 @@
   'Operating System :: Microsoft :: Windows :: Windows 10',
   'License :: OSI Approved :: MIT License',
   'Programming Language :: Python :: 3'
 ]
  
 setup(
   name='PowerWrapper',
-  version='0.0.2',
-  description='A powerful library that wraps advanced functions',
+  version='0.0.3',
+  description='A powerful library that wraps advanced functions.',
   long_description=open('README.txt').read() + '\n\n' + open('CHANGELOG.txt').read(),
   url='',  
   author='SapphireKR',
   author_email='wasimpadho@gmail.com',
   license='MIT', 
   classifiers=classifiers,
   keywords='Wrapper',
```

