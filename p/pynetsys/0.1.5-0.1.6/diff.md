# Comparing `tmp/pynetsys-0.1.5.tar.gz` & `tmp/pynetsys-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pynetsys-0.1.5.tar", last modified: Sat Nov 26 15:18:29 2022, max compression
+gzip compressed data, was "pynetsys-0.1.6.tar", last modified: Sun Apr  9 10:01:20 2023, max compression
```

## Comparing `pynetsys-0.1.5.tar` & `pynetsys-0.1.6.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2022-11-26 15:18:29.260653 pynetsys-0.1.5/
--rw-rw-rw-   0        0        0     1571 2022-03-03 08:07:00.000000 pynetsys-0.1.5/LICENSE
--rw-rw-rw-   0        0        0     2577 2022-11-26 15:18:29.259655 pynetsys-0.1.5/PKG-INFO
--rw-rw-rw-   0        0        0     1791 2022-11-16 18:12:57.000000 pynetsys-0.1.5/README.md
-drwxrwxrwx   0        0        0        0 2022-11-26 15:18:29.237270 pynetsys-0.1.5/pynetsys/
--rw-rw-rw-   0        0        0     1543 2022-11-26 15:18:08.000000 pynetsys-0.1.5/pynetsys/__init__.py
--rw-rw-rw-   0        0        0     2113 2022-11-16 18:24:57.000000 pynetsys-0.1.5/pynetsys/_packet.py
--rw-rw-rw-   0        0        0    13884 2022-11-19 17:18:43.000000 pynetsys-0.1.5/pynetsys/_tool.py
--rw-rw-rw-   0        0        0      230 2022-07-04 21:35:08.000000 pynetsys-0.1.5/pynetsys/constants.py
--rw-rw-rw-   0        0        0       40 2022-07-03 22:56:38.000000 pynetsys-0.1.5/pynetsys/error.py
-drwxrwxrwx   0        0        0        0 2022-11-26 15:18:29.257657 pynetsys-0.1.5/pynetsys.egg-info/
--rw-rw-rw-   0        0        0     2577 2022-11-26 15:18:29.000000 pynetsys-0.1.5/pynetsys.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      284 2022-11-26 15:18:29.000000 pynetsys-0.1.5/pynetsys.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-11-26 15:18:29.000000 pynetsys-0.1.5/pynetsys.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       32 2022-11-26 15:18:29.000000 pynetsys-0.1.5/pynetsys.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2022-11-26 15:18:29.000000 pynetsys-0.1.5/pynetsys.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2022-11-26 15:18:29.260653 pynetsys-0.1.5/setup.cfg
--rw-rw-rw-   0        0        0     1208 2022-11-26 15:14:39.000000 pynetsys-0.1.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-09 10:01:20.439758 pynetsys-0.1.6/
+-rw-rw-rw-   0        0        0     1571 2022-03-03 08:07:00.000000 pynetsys-0.1.6/LICENSE
+-rw-rw-rw-   0        0        0     2577 2023-04-09 10:01:20.439758 pynetsys-0.1.6/PKG-INFO
+-rw-rw-rw-   0        0        0     1791 2022-11-16 18:12:58.000000 pynetsys-0.1.6/README.md
+drwxrwxrwx   0        0        0        0 2023-04-09 10:01:20.422752 pynetsys-0.1.6/pynetsys/
+-rw-rw-rw-   0        0        0     1549 2023-04-09 10:00:44.000000 pynetsys-0.1.6/pynetsys/__init__.py
+-rw-rw-rw-   0        0        0     2113 2022-11-16 18:24:58.000000 pynetsys-0.1.6/pynetsys/_packet.py
+-rw-rw-rw-   0        0        0    13884 2022-11-19 17:18:44.000000 pynetsys-0.1.6/pynetsys/_tool.py
+-rw-rw-rw-   0        0        0      230 2022-07-04 21:35:08.000000 pynetsys-0.1.6/pynetsys/constants.py
+-rw-rw-rw-   0        0        0       40 2022-07-03 22:56:38.000000 pynetsys-0.1.6/pynetsys/error.py
+drwxrwxrwx   0        0        0        0 2023-04-09 10:01:20.436743 pynetsys-0.1.6/pynetsys.egg-info/
+-rw-rw-rw-   0        0        0     2577 2023-04-09 10:01:20.000000 pynetsys-0.1.6/pynetsys.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      284 2023-04-09 10:01:20.000000 pynetsys-0.1.6/pynetsys.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-09 10:01:20.000000 pynetsys-0.1.6/pynetsys.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       32 2023-04-09 10:01:20.000000 pynetsys-0.1.6/pynetsys.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-04-09 10:01:20.000000 pynetsys-0.1.6/pynetsys.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-09 10:01:20.439758 pynetsys-0.1.6/setup.cfg
+-rw-rw-rw-   0        0        0     1208 2023-04-09 10:00:16.000000 pynetsys-0.1.6/setup.py
```

### Comparing `pynetsys-0.1.5/LICENSE` & `pynetsys-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pynetsys-0.1.5/PKG-INFO` & `pynetsys-0.1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pynetsys
-Version: 0.1.5
+Version: 0.1.6
 Summary: pynetsys is a collection of tools and malicious packets.
 Home-page: https://github.com/ANDRVV/pynetsys
 Author: Andrea Vaccaro (ANDRVV)
 License: BSD 3 License
 Keywords: python,socket,threading,server,client,packet,packets,net,network,wireless,dos,tools,tool,traceroute,arp,tracert,arping,nslookup
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
```

### Comparing `pynetsys-0.1.5/README.md` & `pynetsys-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `pynetsys-0.1.5/pynetsys/__init__.py` & `pynetsys-0.1.6/pynetsys/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,13 +48,13 @@
     # IMPORT
     from scapy.all import sr1
     from scapy.layers.inet import IP, ICMP
     import socket
 
     # RUN & RETURN
     try:
-        if sr1(IP(dst = socket.gethostbyname(Address))/ICMP(), timeout = 1, verbose = 0) is None:
+        if sr1(IP(dst = socket.gethostbyname(Address))/ICMP(id = 1), timeout = 1, verbose = 0) is None:
             return False
         else:
             return True
     except:
         return False
```

### Comparing `pynetsys-0.1.5/pynetsys/_packet.py` & `pynetsys-0.1.6/pynetsys/_packet.py`

 * *Files identical despite different names*

### Comparing `pynetsys-0.1.5/pynetsys/_tool.py` & `pynetsys-0.1.6/pynetsys/_tool.py`

 * *Files identical despite different names*

### Comparing `pynetsys-0.1.5/pynetsys.egg-info/PKG-INFO` & `pynetsys-0.1.6/pynetsys.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pynetsys
-Version: 0.1.5
+Version: 0.1.6
 Summary: pynetsys is a collection of tools and malicious packets.
 Home-page: https://github.com/ANDRVV/pynetsys
 Author: Andrea Vaccaro (ANDRVV)
 License: BSD 3 License
 Keywords: python,socket,threading,server,client,packet,packets,net,network,wireless,dos,tools,tool,traceroute,arp,tracert,arping,nslookup
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
```

### Comparing `pynetsys-0.1.5/setup.py` & `pynetsys-0.1.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import os, codecs
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = "0.1.5"
+VERSION = "0.1.6"
 DESCRIPTION = "pynetsys is a collection of tools and malicious packets."
 
 setup(
     name="pynetsys",
     version=VERSION,
     url="https://github.com/ANDRVV/pynetsys",
     author="Andrea Vaccaro (ANDRVV)",
```

