# Comparing `tmp/muse-maskgit-pytorch-0.1.4.tar.gz` & `tmp/muse-maskgit-pytorch-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "muse-maskgit-pytorch-0.1.4.tar", last modified: Fri Mar 31 17:28:22 2023, max compression
+gzip compressed data, was "muse-maskgit-pytorch-0.1.5.tar", last modified: Sun Apr  9 01:52:37 2023, max compression
```

## Comparing `muse-maskgit-pytorch-0.1.4.tar` & `muse-maskgit-pytorch-0.1.5.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 17:28:22.546374 muse-maskgit-pytorch-0.1.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-03-31 17:27:53.000000 muse-maskgit-pytorch-0.1.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-03-31 17:28:22.546374 muse-maskgit-pytorch-0.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8963 2023-03-31 17:27:53.000000 muse-maskgit-pytorch-0.1.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 17:28:22.542374 muse-maskgit-pytorch-0.1.4/muse_maskgit_pytorch/
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-03-31 17:27:53.000000 muse-maskgit-pytorch-0.1.4/muse_maskgit_pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24802 2023-03-31 17:27:53.000000 muse-maskgit-pytorch-0.1.4/muse_maskgit_pytorch/muse_maskgit_pytorch.py
--rw-r--r--   0 runner    (1001) docker     (123)     2413 2023-03-31 17:27:53.000000 muse-maskgit-pytorch-0.1.4/muse_maskgit_pytorch/t5.py
--rw-r--r--   0 runner    (1001) docker     (123)    12008 2023-03-31 17:27:53.000000 muse-maskgit-pytorch-0.1.4/muse_maskgit_pytorch/trainers.py
--rw-r--r--   0 runner    (1001) docker     (123)    14851 2023-03-31 17:27:53.000000 muse-maskgit-pytorch-0.1.4/muse_maskgit_pytorch/vqgan_vae.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 17:28:22.546374 muse-maskgit-pytorch-0.1.4/muse_maskgit_pytorch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-03-31 17:28:22.000000 muse-maskgit-pytorch-0.1.4/muse_maskgit_pytorch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      417 2023-03-31 17:28:22.000000 muse-maskgit-pytorch-0.1.4/muse_maskgit_pytorch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-31 17:28:22.000000 muse-maskgit-pytorch-0.1.4/muse_maskgit_pytorch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-03-31 17:28:22.000000 muse-maskgit-pytorch-0.1.4/muse_maskgit_pytorch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-03-31 17:28:22.000000 muse-maskgit-pytorch-0.1.4/muse_maskgit_pytorch.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-31 17:28:22.546374 muse-maskgit-pytorch-0.1.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-03-31 17:27:53.000000 muse-maskgit-pytorch-0.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 01:52:37.187594 muse-maskgit-pytorch-0.1.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-04-09 01:52:24.000000 muse-maskgit-pytorch-0.1.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-04-09 01:52:37.187594 muse-maskgit-pytorch-0.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8963 2023-04-09 01:52:24.000000 muse-maskgit-pytorch-0.1.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 01:52:37.187594 muse-maskgit-pytorch-0.1.5/muse_maskgit_pytorch/
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-04-09 01:52:24.000000 muse-maskgit-pytorch-0.1.5/muse_maskgit_pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24802 2023-04-09 01:52:24.000000 muse-maskgit-pytorch-0.1.5/muse_maskgit_pytorch/muse_maskgit_pytorch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2413 2023-04-09 01:52:24.000000 muse-maskgit-pytorch-0.1.5/muse_maskgit_pytorch/t5.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12012 2023-04-09 01:52:24.000000 muse-maskgit-pytorch-0.1.5/muse_maskgit_pytorch/trainers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14851 2023-04-09 01:52:24.000000 muse-maskgit-pytorch-0.1.5/muse_maskgit_pytorch/vqgan_vae.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 01:52:37.187594 muse-maskgit-pytorch-0.1.5/muse_maskgit_pytorch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-04-09 01:52:37.000000 muse-maskgit-pytorch-0.1.5/muse_maskgit_pytorch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-04-09 01:52:37.000000 muse-maskgit-pytorch-0.1.5/muse_maskgit_pytorch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-09 01:52:37.000000 muse-maskgit-pytorch-0.1.5/muse_maskgit_pytorch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-04-09 01:52:37.000000 muse-maskgit-pytorch-0.1.5/muse_maskgit_pytorch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-09 01:52:37.000000 muse-maskgit-pytorch-0.1.5/muse_maskgit_pytorch.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-09 01:52:37.187594 muse-maskgit-pytorch-0.1.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-04-09 01:52:24.000000 muse-maskgit-pytorch-0.1.5/setup.py
```

### Comparing `muse-maskgit-pytorch-0.1.4/LICENSE` & `muse-maskgit-pytorch-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `muse-maskgit-pytorch-0.1.4/PKG-INFO` & `muse-maskgit-pytorch-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: muse-maskgit-pytorch
-Version: 0.1.4
+Version: 0.1.5
 Summary: MUSE - Text-to-Image Generation via Masked Generative Transformers, in Pytorch
 Home-page: https://github.com/lucidrains/muse-maskgit-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,transformers,attention mechanism,text-to-image
 Classifier: Development Status :: 4 - Beta
```

### Comparing `muse-maskgit-pytorch-0.1.4/README.md` & `muse-maskgit-pytorch-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `muse-maskgit-pytorch-0.1.4/muse_maskgit_pytorch/muse_maskgit_pytorch.py` & `muse-maskgit-pytorch-0.1.5/muse_maskgit_pytorch/muse_maskgit_pytorch.py`

 * *Files identical despite different names*

### Comparing `muse-maskgit-pytorch-0.1.4/muse_maskgit_pytorch/t5.py` & `muse-maskgit-pytorch-0.1.5/muse_maskgit_pytorch/t5.py`

 * *Files identical despite different names*

### Comparing `muse-maskgit-pytorch-0.1.4/muse_maskgit_pytorch/trainers.py` & `muse-maskgit-pytorch-0.1.5/muse_maskgit_pytorch/trainers.py`

 * *Files 2% similar despite different names*

```diff
@@ -144,15 +144,15 @@
 
         # instantiate accelerator
 
         kwargs_handlers = accelerate_kwargs.get('kwargs_handlers', [])
 
         ddp_kwargs = find_and_pop(
             kwargs_handlers,
-            partial(isinstance, DistributedDataParallelKwargs),
+            lambda x: isinstance(x, DistributedDataParallelKwargs),
             partial(DistributedDataParallelKwargs, find_unused_parameters = True)
         )
 
         ddp_kwargs.find_unused_parameters = True
         kwargs_handlers.append(ddp_kwargs)
         accelerate_kwargs.update(kwargs_handlers = kwargs_handlers)
```

### Comparing `muse-maskgit-pytorch-0.1.4/muse_maskgit_pytorch/vqgan_vae.py` & `muse-maskgit-pytorch-0.1.5/muse_maskgit_pytorch/vqgan_vae.py`

 * *Files identical despite different names*

### Comparing `muse-maskgit-pytorch-0.1.4/muse_maskgit_pytorch.egg-info/PKG-INFO` & `muse-maskgit-pytorch-0.1.5/muse_maskgit_pytorch.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: muse-maskgit-pytorch
-Version: 0.1.4
+Version: 0.1.5
 Summary: MUSE - Text-to-Image Generation via Masked Generative Transformers, in Pytorch
 Home-page: https://github.com/lucidrains/muse-maskgit-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,transformers,attention mechanism,text-to-image
 Classifier: Development Status :: 4 - Beta
```

### Comparing `muse-maskgit-pytorch-0.1.4/setup.py` & `muse-maskgit-pytorch-0.1.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
   name = 'muse-maskgit-pytorch',
   packages = find_packages(exclude=[]),
-  version = '0.1.4',
+  version = '0.1.5',
   license='MIT',
   description = 'MUSE - Text-to-Image Generation via Masked Generative Transformers, in Pytorch',
   author = 'Phil Wang',
   author_email = 'lucidrains@gmail.com',
   long_description_content_type = 'text/markdown',
   url = 'https://github.com/lucidrains/muse-maskgit-pytorch',
   keywords = [
```

