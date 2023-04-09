# Comparing `tmp/pooled-pika-0.2.1.tar.gz` & `tmp/pooled-pika-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pooled-pika-0.2.1.tar", last modified: Fri Jun 19 07:08:16 2020, max compression
+gzip compressed data, was "pooled-pika-0.3.0.tar", last modified: Sun Apr  9 11:07:54 2023, max compression
```

## Comparing `pooled-pika-0.2.1.tar` & `pooled-pika-0.3.0.tar`

### file list

```diff
@@ -1,12 +1,13 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-06-19 07:08:16.000000 pooled-pika-0.2.1/
--rw-rw-r--   0 travis    (2000) travis    (2000)     7002 2020-06-19 07:07:47.000000 pooled-pika-0.2.1/pooled_pika.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1503 2020-06-19 07:08:16.000000 pooled-pika-0.2.1/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)       38 2020-06-19 07:08:16.000000 pooled-pika-0.2.1/setup.cfg
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-06-19 07:08:16.000000 pooled-pika-0.2.1/pooled_pika.egg-info/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1503 2020-06-19 07:08:16.000000 pooled-pika-0.2.1/pooled_pika.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2020-06-19 07:08:16.000000 pooled-pika-0.2.1/pooled_pika.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       12 2020-06-19 07:08:16.000000 pooled-pika-0.2.1/pooled_pika.egg-info/top_level.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      208 2020-06-19 07:08:16.000000 pooled-pika-0.2.1/pooled_pika.egg-info/SOURCES.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       28 2020-06-19 07:08:16.000000 pooled-pika-0.2.1/pooled_pika.egg-info/requires.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)     1482 2020-06-19 07:07:47.000000 pooled-pika-0.2.1/README.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)     1426 2020-06-19 07:07:47.000000 pooled-pika-0.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 11:07:54.243430 pooled-pika-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-04-09 11:07:44.000000 pooled-pika-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-04-09 11:07:54.243430 pooled-pika-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1525 2023-04-09 11:07:44.000000 pooled-pika-0.3.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 11:07:54.239430 pooled-pika-0.3.0/pooled_pika.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-04-09 11:07:54.000000 pooled-pika-0.3.0/pooled_pika.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      216 2023-04-09 11:07:54.000000 pooled-pika-0.3.0/pooled_pika.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-09 11:07:54.000000 pooled-pika-0.3.0/pooled_pika.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-04-09 11:07:54.000000 pooled-pika-0.3.0/pooled_pika.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-09 11:07:54.000000 pooled-pika-0.3.0/pooled_pika.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     7047 2023-04-09 11:07:44.000000 pooled-pika-0.3.0/pooled_pika.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-09 11:07:54.243430 pooled-pika-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1462 2023-04-09 11:07:44.000000 pooled-pika-0.3.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `pooled-pika-0.2.1/pooled_pika.py` & `pooled-pika-0.3.0/pooled_pika.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,16 +31,15 @@
     try:
         yield
     finally:
         __lock.release()
 
 
 class PooledConn(object):
-    """
-    """
+    """ """
 
     _my_params = {}
     _my_pools = ({}, {})
     _my_channels = {}
     _timeout = {}
     _max_size = {}
     _waiting = {}
@@ -158,15 +157,17 @@
         """
         with _lock():
             try:
                 idle_pool.pop(conn_id)
                 logger.info("a connection lost when not using")
             except KeyError:
                 if using_pool.pop(conn_id, None):
-                    logger.warn("connection lost when using, should be handled later")
+                    logger.warning(
+                        "connection lost when using, should be handled later"
+                    )
                     return reason
             finally:
                 channel_pool.pop(conn_id, None)
 
     def _get_channel(self, conn):
         _id = id(conn)
         d = None
```

### Comparing `pooled-pika-0.2.1/PKG-INFO` & `pooled-pika-0.3.0/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,46 +1,54 @@
-Metadata-Version: 1.0
-Name: pooled-pika
-Version: 0.2.1
-Summary: a connection pool wrapper about async pika
-Home-page: https://github.com/Zephor5/pooled-pika
-Author: Zephor
-Author-email: zephor@qq.com
-License: BSD 3-clause
-Description: 
-        Notice
-        ------
-        just support twisted connection now
-        
-        Usage
-        -----
-        sample:
-        
-        .. code :: python
-        
-            # with connection
-            from pika import URLParameters
-            from pooled_pika import PooledConn
-        
-            AMQP_PARAM = URLParameters('amqp://user:pwd@amqpserver')
-            pooled_conn = PooledConn(AMQP_PARAM)
-            d = pooled_conn.acquire()
-            d.addCallbacks(_on_conn, _on_err_conn) # you will get a TwistedProtocolConnection object
-            d.addErrback(_on_err)
-            d.addBoth(pooled_conn.release)  # must release what acquired anyway
-        
-        or:
-        
-        .. code :: python
-        
-            # with channel
-            from pika import URLParameters
-            from pooled_pika import PooledConn
-        
-            AMQP_PARAM = URLParameters('amqp://user:pwd@amqpserver')
-            pooled_conn = PooledConn(AMQP_PARAM)
-            d = pooled_conn.acquire(channel=True)
-            d.addCallbacks(_on_channel, _on_err_channel) # you will get a TwistedChannel object
-            d.addErrback(_on_err)
-            d.addBoth(pooled_conn.release)  # must release what acquired anyway
-        
-Platform: UNKNOWN
+from setuptools import find_packages
+from setuptools import setup
+
+
+setup(
+    name="pooled-pika",
+    version="0.3.0",
+    py_modules=["pooled_pika"],
+    install_requires=["twisted~=22.10.0", "pika~=1.3.0"],
+    python_requires=">=3.7,<3.10",
+    description="a connection pool wrapper about async pika",
+    long_description="""
+Notice
+------
+just support twisted connection now
+
+Usage
+-----
+sample:
+
+.. code :: python
+
+    # with connection
+    from pika import URLParameters
+    from pooled_pika import PooledConn
+
+    AMQP_PARAM = URLParameters('amqp://user:pwd@amqpserver')
+    pooled_conn = PooledConn(AMQP_PARAM)
+    d = pooled_conn.acquire()
+    d.addCallbacks(_on_conn, _on_err_conn) # you will get a TwistedProtocolConnection object
+    d.addErrback(_on_err)
+    d.addBoth(pooled_conn.release)  # must release what acquired anyway
+
+or:
+
+.. code :: python
+
+    # with channel
+    from pika import URLParameters
+    from pooled_pika import PooledConn
+
+    AMQP_PARAM = URLParameters('amqp://user:pwd@amqpserver')
+    pooled_conn = PooledConn(AMQP_PARAM)
+    d = pooled_conn.acquire(channel=True)
+    d.addCallbacks(_on_channel, _on_err_channel) # you will get a TwistedChannel object
+    d.addErrback(_on_err)
+    d.addBoth(pooled_conn.release)  # must release what acquired anyway
+""",
+    author="Zephor",
+    author_email="zephor@qq.com",
+    url="https://github.com/Zephor5/pooled-pika",
+    license="BSD 3-clause",
+    packages=find_packages(),
+)
```

### Comparing `pooled-pika-0.2.1/pooled_pika.egg-info/PKG-INFO` & `pooled-pika-0.3.0/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,46 +1,47 @@
-Metadata-Version: 1.0
+Metadata-Version: 2.1
 Name: pooled-pika
-Version: 0.2.1
+Version: 0.3.0
 Summary: a connection pool wrapper about async pika
 Home-page: https://github.com/Zephor5/pooled-pika
 Author: Zephor
 Author-email: zephor@qq.com
 License: BSD 3-clause
-Description: 
-        Notice
-        ------
-        just support twisted connection now
-        
-        Usage
-        -----
-        sample:
-        
-        .. code :: python
-        
-            # with connection
-            from pika import URLParameters
-            from pooled_pika import PooledConn
-        
-            AMQP_PARAM = URLParameters('amqp://user:pwd@amqpserver')
-            pooled_conn = PooledConn(AMQP_PARAM)
-            d = pooled_conn.acquire()
-            d.addCallbacks(_on_conn, _on_err_conn) # you will get a TwistedProtocolConnection object
-            d.addErrback(_on_err)
-            d.addBoth(pooled_conn.release)  # must release what acquired anyway
-        
-        or:
-        
-        .. code :: python
-        
-            # with channel
-            from pika import URLParameters
-            from pooled_pika import PooledConn
-        
-            AMQP_PARAM = URLParameters('amqp://user:pwd@amqpserver')
-            pooled_conn = PooledConn(AMQP_PARAM)
-            d = pooled_conn.acquire(channel=True)
-            d.addCallbacks(_on_channel, _on_err_channel) # you will get a TwistedChannel object
-            d.addErrback(_on_err)
-            d.addBoth(pooled_conn.release)  # must release what acquired anyway
-        
-Platform: UNKNOWN
+Requires-Python: >=3.7,<3.10
+License-File: LICENSE
+
+
+Notice
+------
+just support twisted connection now
+
+Usage
+-----
+sample:
+
+.. code :: python
+
+    # with connection
+    from pika import URLParameters
+    from pooled_pika import PooledConn
+
+    AMQP_PARAM = URLParameters('amqp://user:pwd@amqpserver')
+    pooled_conn = PooledConn(AMQP_PARAM)
+    d = pooled_conn.acquire()
+    d.addCallbacks(_on_conn, _on_err_conn) # you will get a TwistedProtocolConnection object
+    d.addErrback(_on_err)
+    d.addBoth(pooled_conn.release)  # must release what acquired anyway
+
+or:
+
+.. code :: python
+
+    # with channel
+    from pika import URLParameters
+    from pooled_pika import PooledConn
+
+    AMQP_PARAM = URLParameters('amqp://user:pwd@amqpserver')
+    pooled_conn = PooledConn(AMQP_PARAM)
+    d = pooled_conn.acquire(channel=True)
+    d.addCallbacks(_on_channel, _on_err_channel) # you will get a TwistedChannel object
+    d.addErrback(_on_err)
+    d.addBoth(pooled_conn.release)  # must release what acquired anyway
```

### Comparing `pooled-pika-0.2.1/README.rst` & `pooled-pika-0.3.0/README.rst`

 * *Files 13% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 mypika
 ======
 
 .. image:: https://img.shields.io/pypi/v/pooled-pika.svg
-   :target: https://pypi.python.org/pypi/pooled-pika
+   :target: https://pypi.org/pypi/pooled-pika
    :alt: PyPI Version
 
 .. image:: https://img.shields.io/pypi/dm/pooled-pika.svg
-   :target: https://pypi.python.org/pypi/pooled-pika
+   :target: https://pypi.org/pypi/pooled-pika
    :alt: PyPI Monthly downloads
 
-.. image:: https://img.shields.io/travis/Zephor5/pooled-pika/master.svg
-   :target: http://travis-ci.org/Zephor5/pooled-pika
+.. image:: https://github.com/Zephor5/pooled-pika/actions/workflows/build.yml/badge.svg?branch=master
+   :target: https://github.com/Zephor5/pooled-pika/actions/workflows/build.yml
    :alt: Build Status
 
-a connection pool wrapper about async pika, using twisted TODO tornado and so on
+a connection pool wrapper about async pika, using twisted
+
+TODO tornado and so on
 
 Notice
 ------
 just support twisted connection now
 
 Usage
 -----
```

### Comparing `pooled-pika-0.2.1/setup.py` & `pooled-pika-0.3.0/pooled_pika.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,18 +1,19 @@
-from setuptools import find_packages
-from setuptools import setup
+Metadata-Version: 2.1
+Name: pooled-pika
+Version: 0.3.0
+Summary: a connection pool wrapper about async pika
+Home-page: https://github.com/Zephor5/pooled-pika
+Author: Zephor
+Author-email: zephor@qq.com
+License: BSD 3-clause
+Requires-Python: >=3.7,<3.10
+License-File: LICENSE
 
 
-setup(
-    name="pooled-pika",
-    version="0.2.1",
-    py_modules=["pooled_pika"],
-    install_requires=["twisted~=20.3.0", "pika~=1.1.0"],
-    description="a connection pool wrapper about async pika",
-    long_description="""
 Notice
 ------
 just support twisted connection now
 
 Usage
 -----
 sample:
@@ -40,14 +41,7 @@
 
     AMQP_PARAM = URLParameters('amqp://user:pwd@amqpserver')
     pooled_conn = PooledConn(AMQP_PARAM)
     d = pooled_conn.acquire(channel=True)
     d.addCallbacks(_on_channel, _on_err_channel) # you will get a TwistedChannel object
     d.addErrback(_on_err)
     d.addBoth(pooled_conn.release)  # must release what acquired anyway
-""",
-    author="Zephor",
-    author_email="zephor@qq.com",
-    url="https://github.com/Zephor5/pooled-pika",
-    license="BSD 3-clause",
-    packages=find_packages(),
-)
```

