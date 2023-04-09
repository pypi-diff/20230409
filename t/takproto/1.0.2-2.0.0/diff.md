# Comparing `tmp/takproto-1.0.2.tar.gz` & `tmp/takproto-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "takproto-1.0.2.tar", last modified: Fri Jan 13 00:56:12 2023, max compression
+gzip compressed data, was "takproto-2.0.0.tar", last modified: Sun Apr  9 19:53:03 2023, max compression
```

## Comparing `takproto-1.0.2.tar` & `takproto-2.0.0.tar`

### file list

```diff
@@ -1,16 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 00:56:12.979597 takproto-1.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-01-13 00:56:03.000000 takproto-1.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7021 2023-01-13 00:56:12.979597 takproto-1.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6457 2023-01-13 00:56:03.000000 takproto-1.0.2/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-13 00:56:12.979597 takproto-1.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2980 2023-01-13 00:56:03.000000 takproto-1.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 00:56:12.975597 takproto-1.0.2/takproto/
--rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-01-13 00:56:03.000000 takproto-1.0.2/takproto/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6976 2023-01-13 00:56:03.000000 takproto-1.0.2/takproto/functions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 00:56:12.979597 takproto-1.0.2/takproto.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7021 2023-01-13 00:56:12.000000 takproto-1.0.2/takproto.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-01-13 00:56:12.000000 takproto-1.0.2/takproto.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-13 00:56:12.000000 takproto-1.0.2/takproto.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-13 00:56:12.000000 takproto-1.0.2/takproto.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-01-13 00:56:12.000000 takproto-1.0.2/takproto.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-01-13 00:56:12.000000 takproto-1.0.2/takproto.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 19:53:03.884968 takproto-2.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-04-09 19:52:53.000000 takproto-2.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     9101 2023-04-09 19:53:03.884968 takproto-2.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8539 2023-04-09 19:52:53.000000 takproto-2.0.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-09 19:53:03.884968 takproto-2.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3070 2023-04-09 19:52:53.000000 takproto-2.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 19:53:03.880967 takproto-2.0.0/takproto/
+-rw-r--r--   0 runner    (1001) docker     (123)     1672 2023-04-09 19:52:53.000000 takproto-2.0.0/takproto/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1591 2023-04-09 19:52:53.000000 takproto-2.0.0/takproto/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8196 2023-04-09 19:52:53.000000 takproto-2.0.0/takproto/functions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 19:53:03.884968 takproto-2.0.0/takproto/proto/
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-04-09 19:52:53.000000 takproto-2.0.0/takproto/proto/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-04-09 19:52:53.000000 takproto-2.0.0/takproto/proto/contact_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1684 2023-04-09 19:52:53.000000 takproto-2.0.0/takproto/proto/cotevent_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1951 2023-04-09 19:52:53.000000 takproto-2.0.0/takproto/proto/detail_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-04-09 19:52:53.000000 takproto-2.0.0/takproto/proto/group_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-04-09 19:52:53.000000 takproto-2.0.0/takproto/proto/precisionlocation_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-04-09 19:52:53.000000 takproto-2.0.0/takproto/proto/status_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-04-09 19:52:53.000000 takproto-2.0.0/takproto/proto/takcontrol_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-04-09 19:52:53.000000 takproto-2.0.0/takproto/proto/takmessage_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-04-09 19:52:53.000000 takproto-2.0.0/takproto/proto/takv_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-04-09 19:52:53.000000 takproto-2.0.0/takproto/proto/track_pb2.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 19:53:03.884968 takproto-2.0.0/takproto.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9101 2023-04-09 19:53:03.000000 takproto-2.0.0/takproto.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      617 2023-04-09 19:53:03.000000 takproto-2.0.0/takproto.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-09 19:53:03.000000 takproto-2.0.0/takproto.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-09 19:53:03.000000 takproto-2.0.0/takproto.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-09 19:53:03.000000 takproto-2.0.0/takproto.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-09 19:53:03.000000 takproto-2.0.0/takproto.egg-info/top_level.txt
```

### Comparing `takproto-1.0.2/LICENSE` & `takproto-2.0.0/LICENSE`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-Copyright 2023 Greg Albrecht <oss@undef.net>
+Copyright 2023 Sensors & Signals LLC
 Copyright 2020 Delta Bravo-15 <deltabravo15ga@gmail.com>
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
```

### Comparing `takproto-1.0.2/PKG-INFO` & `takproto-2.0.0/README.rst`

 * *Files 21% similar despite different names*

```diff
@@ -1,104 +1,102 @@
-Metadata-Version: 2.1
-Name: takproto
-Version: 1.0.2
-Summary: A Python module to encode & decode 'TAK Protocol Payload - Version 1' Protocol Buffer based Cursor on Target (CoT) messages.
-Home-page: https://github.com/ampledata/takproto
-Author: Greg Albrecht
-Author-email: oss@undef.net
-License: MIT License
-Keywords: Cursor on Target,ATAK,TAK,CoT,WinTAK,iTAK
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Description-Content-Type: text/x-rst
-License-File: LICENSE
+.. image:: ./docs/pytak_logo-256x264.png
+    :alt: PyTAK Logo
+
+takproto: TAK Protocol Python Module
+************************************
 
-TAK Protocol Payload - Version 1 Python Module (takproto)
-*********************************************************
 ``takproto`` is a Python module to encode & decode 'TAK Protocol Payload - Version 1' 
 Protocol Buffer based Cursor on Target (CoT) messages.
 
+From the ATAK source:
+
     Version 1 of the TAK Protocol Payload is a Google Protocol Buffer based
     payload.  Each Payload consists of one (and only one)
     atakmap::commoncommo::v1::TakMessage message which is serialized using
     Google protocol buffers version 3.
 
     Source: https://github.com/deptofdefense/AndroidTacticalAssaultKit-CIV/blob/master/commoncommo/core/impl/protobuf/protocol.txt
 
 ``takproto`` is a fork & complete re-write of @dB-SPL's 
 `takprotobuf <https://github.com/dB-SPL/takprotobuf>`_.
 Absolute credit goes to them for their initial implementation. 
 
-Notable differences beteen ``takprotobuf`` & ``takproto``:
+Notable differences between the original ``takprotobuf`` & this module ``takproto``:
 
 1. Rebuild proto files using `Protocol Buffers v21 <https://protobuf.dev/>`_.
-2. Remove dependency on ``untangle`` module, allowing compatibility with Python 3.6 
+2. Added support for encoding & decoding plain XML, Mesh & Stream TAK Protocol formats.
+3. Remove dependency on ``untangle`` module, allowing compatibility with Python 3.6 
    through 3.10. Unfortunately many single-board computers (i.e. Raspberry Pi) still 
    ship with Python 3.6, this change allows ``takproto`` to run on those systems.
-3. Added ``xmlDetails`` detection for supporting undefined Protobuf elements in XML.
-4. > 80% test coverage with **new** Unit Tests.
-5. PEP-8 & Black style, linting, documentation & formatting of code.
+4. Added ``xmlDetails`` detection for supporting undefined Protobuf elements in XML.
+5. > 90% test coverage with **new** Unit Tests.
+6. PEP-8 & Black style, linting, documentation & formatting of code.
 
 As much as possible @db-SPL's licensing terms were honored in this fork.
 
 
 Usage
 =====
 
-There are two functions included in this module:
+The `takproto` module exports two functions:
 
 
 xml2proto()
 -----------
 
 Given a string which contains either a CoT message in XML or the path to an XML file 
-containing a CoT message, the function ``xml2proto()`` will return a bytearray containing 
+containing a CoT message, the function ``xml2proto()`` will return a ``bytearray`` containing 
 the binary protobuf::
 
     import takproto
 
-    xs = """
-    <?xml version='1.0' encoding='UTF-8' standalone='yes'?>
+    cot = """<?xml version='1.0' encoding='UTF-8' standalone='yes'?>
     <event version='2.0' uid='aa0b0312-b5cd-4c2c-bbbc-9c4c70216261' type='a-f-G-E-V-C' time='2020-02-08T18:10:44.000Z' start='2020-02-08T18:10:44.000Z' stale='2020-02-08T18:11:11.000Z' how='h-e'>
         <point lat='43.97957317' lon='-66.07737696' hae='26.767999' ce='9999999.0' le='9999999.0' />
         <detail>
             <uid Droid='Eliopoli HQ'/>
             <contact callsign='Eliopoli HQ' endpoint='192.168.1.10:4242:tcp'/>
             <__group name='Yellow' role='HQ'/><status battery='100'/>
             <takv platform='WinTAK-CIV' device='LENOVO 20QV0007US' os='Microsoft Windows 10 Home' version='1.10.0.137'/>
             <track speed='0.00000000' course='0.00000000'/>
         </detail>
     </event>
     """
 
-    buf = takproto.xml2proto(xs)
+    buf = takproto.xml2proto(cot)
     print(buf)
 
-Would return::
+Would return the CoT XML encoded as TAK Protocol Version 1 Mesh::
     
     bytearray(b'\xbf\x01\xbf\x12\xff\x01\n\x0ba-f-G-E-V-C*$aa0b0312-b5cd-4c2c-bbbc-9c4c702162610\xa0\xa2\xc7\xb8\x82.8\xa0\xa2\xc7\xb8\x82.@\x98\xf5\xc8\xb8\x82.J\x03h-eQ3\x98T\xa7b\xfdE@Y}*~\xbe\xf3\x84P\xc0aW\\\x1c\x95\x9b\xc4:@i\x00\x00\x00\xe0\xcf\x12cAq\x00\x00\x00\xe0\xcf\x12cAz\x82\x01\x12$\n\x15192.168.1.10:4242:tcp\x12\x0bEliopoli HQ\x1a\x0c\n\x06Yellow\x12\x02HQ*\x02\x08d2F\n\x11LENOVO 20QV0007US\x12\nWinTAK-CIV\x1a\x19Microsoft Windows 10 Home"\n1.10.0.137:\x00')
 
+Additionally, calling xml2proto with the `takproto.TAKProtoVer.STREAM` flag would return a stream-ready protobuf::
+
+    buf = takproto.xml2proto(cot, takproto.TAKProtoVer.STREAM)
+    print(buf)
+
+Would return the CoT XML encoded as TAK Protocol Version 1 Stream::
+
+    bytearray(b'\xbf\x9f\x02\x12\xff\x01\n\x0ba-f-G-E-V-C*$aa0b0312-b5cd-4c2c-bbbc-9c4c702162610\xa0\xa2\xc7\xb8\x82.8\xa0\xa2\xc7\xb8\x82.@\x98\xf5\xc8\xb8\x82.J\x03h-eQ3\x98T\xa7b\xfdE@Y}*~\xbe\xf3\x84P\xc0aW\\\x1c\x95\x9b\xc4:@i\x00\x00\x00\xe0\xcf\x12cAq\x00\x00\x00\xe0\xcf\x12cAz\x82\x01\x12$\n\x15192.168.1.10:4242:tcp\x12\x0bEliopoli HQ\x1a\x0c\n\x06Yellow\x12\x02HQ*\x02\x08d2F\n\x11LENOVO 20QV0007US\x12\nWinTAK-CIV\x1a\x19Microsoft Windows 10 Home"\n1.10.0.137:\x00')
+
 
 parse_proto()
 -------------
 
 Given a bytearray containing a version 1 protobuf, ``parse_proto()`` will return an 
 instance of the protobuf class. You can then access the contents as an object::
 
     import takproto
    
-    ba = bytearray(b'\xbf\x01\xbf\x12\xff\x01\n\x0ba-f-G-E-V-C*$aa0b0312-b5cd-4c2c-bbbc-9c4c702162610\xa0\xa2\xc7\xb8\x82.8\xa0\xa2\xc7\xb8\x82.@\x98\xf5\xc8\xb8\x82.J\x03h-eQ3\x98T\xa7b\xfdE@Y}*~\xbe\xf3\x84P\xc0aW\\\x1c\x95\x9b\xc4:@i\x00\x00\x00\xe0\xcf\x12cAq\x00\x00\x00\xe0\xcf\x12cAz\x82\x01\x12$\n\x15192.168.1.10:4242:tcp\x12\x0bEliopoli HQ\x1a\x0c\n\x06Yellow\x12\x02HQ*\x02\x08d2F\n\x11LENOVO 20QV0007US\x12\nWinTAK-CIV\x1a\x19Microsoft Windows 10 Home"\n1.10.0.137:\x00')
+    pb = bytearray(b'\xbf\x01\xbf\x12\xff\x01\n\x0ba-f-G-E-V-C*$aa0b0312-b5cd-4c2c-bbbc-9c4c702162610\xa0\xa2\xc7\xb8\x82.8\xa0\xa2\xc7\xb8\x82.@\x98\xf5\xc8\xb8\x82.J\x03h-eQ3\x98T\xa7b\xfdE@Y}*~\xbe\xf3\x84P\xc0aW\\\x1c\x95\x9b\xc4:@i\x00\x00\x00\xe0\xcf\x12cAq\x00\x00\x00\xe0\xcf\x12cAz\x82\x01\x12$\n\x15192.168.1.10:4242:tcp\x12\x0bEliopoli HQ\x1a\x0c\n\x06Yellow\x12\x02HQ*\x02\x08d2F\n\x11LENOVO 20QV0007US\x12\nWinTAK-CIV\x1a\x19Microsoft Windows 10 Home"\n1.10.0.137:\x00')
 
-    parse_proto(ba)
+    cot = parse_proto(pb)
  
 This method of calling parse_proto would return an object containing the data from the 
-protobuf. Object attributes can be accessed by calling them in a Pythonic manner.
-
-If you were to ``print(parse_proto(b))``, you would see::
+protobuf. If you were to ``print(cot)``, you would see::
 
     cotEvent {
         type: "a-f-G-E-V-C"
         uid: "aa0b0312-b5cd-4c2c-bbbc-9c4c70216261"
         sendTime: 1581203444000
         startTime: 1581203444000
         staleTime: 1581203471000
@@ -127,40 +125,71 @@
             version: "1.10.0.137"
             }
             track {
             }
         }
     }
 
+Object attributes can be accessed by calling them in a Pythonic manner::
+
+    print(cot.cotEvent.detail.contact.callsign)
+    "Eliopoli HQ"
+
+
+Additional Examples
+-------------------
+
+For additional examples using this module, see the `tests/` directory.
+
+
+What's the difference between the TAK Protocol formats?
+=======================================================
+
+Originally the TAK Products spoke Cursor on Target (CoT) encoded as plain XML. Later versions 
+of the TAK Products added support for sending CoT as Google Protobuf, which TPC named 'TAK Protocol Version 1'.
+
+Out of the box, TAK Products such as ATAK and WinTAK configured for 'Mesh SA' will send 
+TAK Protocol Version 1 Mesh formatted CoT. This format utizes a static payload header of 
+the format `191 1 191 <payload>`.
+
+TAK Products configured for connecting to a TAK Server will send TAK Protocol Version 1 Stream 
+formatted CoT. This format utizes a dynamic payload header of the format `191 <varint payload length> <payload>`.
+This header format is required for specifying the size of the payload within the TCP packet.
+
+The `takproto` module supports encoding and decoding all 3 formats of CoT messages.
+
+.. image:: ./docs/takproto_chart.png
+    :alt: TAK Protocol chart
+
 
 Source
 ======
-Github: https://github.com/ampledata/takproto
+Github: https://github.com/snstac/takproto
 
 
 Authors
 =======
-* Greg Albrecht W2GMD oss@undef.net https://ampledata.org/
+* Greg Albrecht https://www.snstac.com/
 * Delta Bravo-15 https://github.com/db-SPL
 
 
 Copyright
 =========
-* Copyright 2023 Greg Albrecht <oss@undef.net>
+* Copyright 2023 Sensors & Signals LLC
 * Copyright 2020 Delta Bravo-15 <deltabravo15ga@gmail.com>
 
 
 Style
 =====
 Python Black, otherwise Google, then PEP-8.
 
 
 License
 =======
-Copyright 2023 Greg Albrecht <oss@undef.net>
+Copyright 2023 Sensors & Signals LLC
 
 Copyright 2020 Delta Bravo-15 <deltabravo15ga@gmail.com>
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
```

### Comparing `takproto-1.0.2/setup.py` & `takproto-2.0.0/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 #
-# Copyright 2023 Greg Albrecht <oss@undef.net>
+# Copyright 2023 Sensors & Signals LLC
 # Copyright 2020 Delta Bravo-15
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
@@ -23,24 +23,24 @@
 # SOFTWARE.
 #
 
 
 """Setup for the Python TAK Protocol Packet - Version 1 Module.
 
 :license: MIT License
-:source: <https://github.com/ampledata/takproto>
+:source: <https://github.com/snstac/takproto>
 """
 
 import os
 import sys
 
 import setuptools
 
 __title__ = "takproto"
-__version__ = "1.0.2"
+__version__ = "2.0.0"
 __license__ = "MIT License"
 
 
 def publish():
     """Publish this package to pypi."""
     if sys.argv[-1] == "publish":
         os.system("python setup.py sdist")
@@ -59,29 +59,30 @@
         readme = rmf.read()
     return readme
 
 
 setuptools.setup(
     version=__version__,
     name=__title__,
-    packages=[__title__],
-    package_dir={__title__: __title__},
-    url=f"https://github.com/ampledata/{__title__}",
+    packages=[__title__, f"{__title__}.proto"],
+    package_dir={__title__: __title__, f"{__title__}.proto":f"{__title__}/proto"},
+    url=f"https://github.com/snstac/{__title__}",
     description=(
         "A Python module to encode & decode 'TAK Protocol Payload - Version 1'"
-        " Protocol Buffer based Cursor on Target (CoT) messages."),
+        " Protocol Buffer based Cursor on Target (CoT) messages."
+    ),
     author="Greg Albrecht",
-    author_email="oss@undef.net",
+    author_email="gba@snstac.com",
     package_data={"": ["LICENSE"]},
     license="MIT License",
     long_description=read_readme(),
     long_description_content_type="text/x-rst",
     zip_safe=False,
     include_package_data=True,
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     keywords=["Cursor on Target", "ATAK", "TAK", "CoT", "WinTAK", "iTAK"],
-    install_requires=["protobuf >= 4.21.0"]
+    install_requires=["protobuf >= 4.21.0", "delimited-protobuf >= 1.0.0"],
 )
```

### Comparing `takproto-1.0.2/takproto/__init__.py` & `takproto-2.0.0/takproto/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,28 +1,45 @@
-#!/usr/bin/env python3
-# -*- coding: utf-8 -*-
-#
-# Copyright 2022 Greg Albrecht <oss@undef.net>
-# Copyright 2020 Delta Bravo-15
-#
-# Permission is hereby granted, free of charge, to any person obtaining a copy
-# of this software and associated documentation files (the "Software"), to deal
-# in the Software without restriction, including without limitation the rights
-# to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-# copies of the Software, and to permit persons to whom the Software is
-# furnished to do so, subject to the following conditions:
-#
-# The above copyright notice and this permission notice shall be included in all
-# copies or substantial portions of the Software.
-#
-# THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-# IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-# FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-# AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-# LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-# OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-# SOFTWARE.
-#
-
-
-from .functions import parse_proto, xml2proto
-
+#!/usr/bin/env python3
+# -*- coding: utf-8 -*-
+#
+# Copyright 2023 Sensors & Signals LLC
+#
+# Permission is hereby granted, free of charge, to any person obtaining a copy
+# of this software and associated documentation files (the "Software"), to deal
+# in the Software without restriction, including without limitation the rights
+# to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+# copies of the Software, and to permit persons to whom the Software is
+# furnished to do so, subject to the following conditions:
+#
+# The above copyright notice and this permission notice shall be included in all
+# copies or substantial portions of the Software.
+#
+# THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+# IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+# FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+# AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+# LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+# OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+# SOFTWARE.
+#
+
+"""TAKProto Module.
+
+:author: Greg Albrecht <gba@snstac.com>
+:copyright: Copyright 2023 Sensors & Signals LLC
+:license: MIT License
+:source: <https://github.com/snstac/takproto>
+"""
+
+from .functions import (  # NOQA
+    xml2proto,
+    parse_proto,
+    parse_mesh,
+    parse_stream,
+    format_time,
+)
+from .constants import TAKProtoVer  # NOQA
+
+__author__ = "Greg Albrecht <gba@snstac.com>"
+__copyright__ = "Copyright 2023 Sensors & Signals LLC"
+__license__ = "MIT License"
+__source__ = "https://github.com/snstac/takproto"
```

### Comparing `takproto-1.0.2/takproto/functions.py` & `takproto-2.0.0/takproto/functions.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 #
-# Copyright 2023 Greg Albrecht <oss@undef.net>
+# Copyright 2023 Sensors & Signals LLC
 # Copyright 2020 Delta Bravo-15 <deltabravo15ga@gmail.com>
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
@@ -18,49 +18,69 @@
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 #
-
-
-from datetime import datetime
+"""TAKProto Functions for manipulating TAK Protocol Version 1 messages."""
 
 import re
-
 import xml.etree.ElementTree as ET
 
-from .proto import TakMessage
-
-
-DEFAULT_PROTO_HEADER = bytearray(b"\xbf\x01\xbf")
-ISO_8601_UTC = "%Y-%m-%dT%H:%M:%S.%fZ"
-
+from datetime import datetime
+from io import BytesIO
+from typing import Optional
 
-def parse_proto(binary):
-    """Parse CoT message."""
-    header = binary[:3]
-    if header != DEFAULT_PROTO_HEADER:
-        return None
+import delimited_protobuf as dpb
 
-    binary = binary[3:]
+from takproto.constants import (
+    ISO_8601_UTC,
+    DEFAULT_MESH_HEADER,
+    DEFAULT_PROTO_HEADER,
+    TAKProtoVer,
+)
+from takproto.proto import TakMessage
+
+
+def parse_proto(msg: bytearray) -> Optional[bytearray]:
+    """Parse TAK Protocol Version 1 Mesh & Stream message."""
+    parsed = None
+
+    if msg[:3] == DEFAULT_MESH_HEADER:
+        parsed = parse_mesh(msg)
+    elif msg[0] in DEFAULT_PROTO_HEADER:
+        parsed = parse_stream(msg)
+    return parsed
+
+
+def parse_mesh(msg):
+    """Parse TAK Protocol Version 1 Mesh message."""
+    msg = msg[3:]
     protobuf = TakMessage()
-    protobuf.ParseFromString(binary)
-
+    protobuf.ParseFromString(bytes(msg))
     return protobuf
 
 
-def format_time(time) -> int:
+def parse_stream(msg):
+    """Parse TAK Protocol Version 1 Stream message."""
+    bio = BytesIO(msg[1:])
+    msg = dpb.read(bio, TakMessage)
+    return msg
+
+
+def format_time(time: str) -> int:
     """Format timestamp as microseconds."""
     s_time = datetime.strptime(time + "+0000", ISO_8601_UTC + "%z")
     return int(s_time.timestamp() * 1000)
 
 
-def xml2proto(xml):
+def xml2proto(
+    xml: str, protover: Optional[TAKProtoVer] = None
+):  # NOQA pylint: disable=too-many-locals,too-many-branches,too-many-statements
     """Convert plain XML CoT to Protobuf."""
     event = ET.fromstring(xml)
     tak_message = TakMessage()
     tak_control = tak_message.takControl
     new_event = tak_message.cotEvent
 
     # If this is a GeoChat message, extract the sender's UID from the event UID and
@@ -84,15 +104,15 @@
             if attrib == "time":
                 attrib = "send"
             setattr(new_event, f"{attrib}Time", format_time(val))
 
     # If the event element includes a point child, write the attributes
     point = event.find("point")
     if point is not None:
-        attribs = ['lat', 'lon', 'hae', 'ce', 'le']
+        attribs = ["lat", "lon", "hae", "ce", "le"]
         for attrib in attribs:
             val = point.get(attrib)
             if val:
                 setattr(new_event, attrib, float(val))
 
     detail = event.find("detail")
     if detail is not None:
@@ -109,18 +129,24 @@
         if uid and "GeoChat." in uid:
             pattern = "<detail>(.*?)</detail>"
             xmldetailstr = re.search(pattern, xml).group(1)
             new_detail.xmlDetail = xmldetailstr
         else:
             # Add unknown elements to xmlDetail field.
             known_elem = [
-                "contact", "__group", "precisionlocation", "status", "takv", "track"]
+                "contact",
+                "__group",
+                "precisionlocation",
+                "status",
+                "takv",
+                "track",
+            ]
             for elem in detail.iterfind("*"):
                 if elem.tag not in known_elem:
-                    new_detail.xmlDetail = ET.tostring(elem)
+                    new_detail.xmlDetail = ET.tostring(elem).strip()
 
         contact = detail.find("contact")
         if contact is not None:
             attribs = ["endpoint", "callsign"]
             for attrib in attribs:
                 attrib_val = contact.get(attrib)
                 if attrib_val:
@@ -163,15 +189,32 @@
         if track is not None:
             attribs = ["speed", "course"]
             for attrib in attribs:
                 attrib_val = track.get(attrib)
                 if attrib_val:
                     setattr(new_detail.track, attrib, float(attrib_val))
 
-    # TAK protocol packets have a three-byte header.  The two 0xbf bytes on the outside
-    # identify the packet as containing TAK protocol.  The 0x01 byte in the middle
-    # identifies the TAK protocol version, in our case, version 1.
-    header_bytearray = DEFAULT_PROTO_HEADER
-    takmessage_bytearray = bytearray(tak_message.SerializeToString())
-    output_bytearray = header_bytearray + takmessage_bytearray
+    output = msg2proto(tak_message, protover)
+    return output
+
+
+def msg2proto(msg, protover: Optional[TAKProtoVer] = None) -> bytearray:
+    """Convert a TakMessage into a TAK Protocol Version 1 protobuf."""
+    protover = protover or TAKProtoVer.MESH
+
+    output_ba = bytearray()
+    header_ba = bytearray()
+    proto_ba = bytearray()
+
+    if protover == TAKProtoVer.MESH:
+        header_ba = DEFAULT_MESH_HEADER
+        proto_ba = bytearray(msg.SerializeToString())
+    elif protover == TAKProtoVer.STREAM:
+        header_ba = DEFAULT_PROTO_HEADER
+        output_io = BytesIO()
+        dpb.write(output_io, msg)
+        proto_ba = bytearray(output_io.getvalue())
+    else:
+        raise ValueError(f"Unsupported TAKProtoVer: {protover}")
 
-    return output_bytearray
+    output_ba = header_ba + proto_ba
+    return output_ba
```

### Comparing `takproto-1.0.2/takproto.egg-info/PKG-INFO` & `takproto-2.0.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,104 +1,117 @@
 Metadata-Version: 2.1
 Name: takproto
-Version: 1.0.2
+Version: 2.0.0
 Summary: A Python module to encode & decode 'TAK Protocol Payload - Version 1' Protocol Buffer based Cursor on Target (CoT) messages.
-Home-page: https://github.com/ampledata/takproto
+Home-page: https://github.com/snstac/takproto
 Author: Greg Albrecht
-Author-email: oss@undef.net
+Author-email: gba@snstac.com
 License: MIT License
 Keywords: Cursor on Target,ATAK,TAK,CoT,WinTAK,iTAK
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
-TAK Protocol Payload - Version 1 Python Module (takproto)
-*********************************************************
+.. image:: ./docs/pytak_logo-256x264.png
+    :alt: PyTAK Logo
+
+takproto: TAK Protocol Python Module
+************************************
+
 ``takproto`` is a Python module to encode & decode 'TAK Protocol Payload - Version 1' 
 Protocol Buffer based Cursor on Target (CoT) messages.
 
+From the ATAK source:
+
     Version 1 of the TAK Protocol Payload is a Google Protocol Buffer based
     payload.  Each Payload consists of one (and only one)
     atakmap::commoncommo::v1::TakMessage message which is serialized using
     Google protocol buffers version 3.
 
     Source: https://github.com/deptofdefense/AndroidTacticalAssaultKit-CIV/blob/master/commoncommo/core/impl/protobuf/protocol.txt
 
 ``takproto`` is a fork & complete re-write of @dB-SPL's 
 `takprotobuf <https://github.com/dB-SPL/takprotobuf>`_.
 Absolute credit goes to them for their initial implementation. 
 
-Notable differences beteen ``takprotobuf`` & ``takproto``:
+Notable differences between the original ``takprotobuf`` & this module ``takproto``:
 
 1. Rebuild proto files using `Protocol Buffers v21 <https://protobuf.dev/>`_.
-2. Remove dependency on ``untangle`` module, allowing compatibility with Python 3.6 
+2. Added support for encoding & decoding plain XML, Mesh & Stream TAK Protocol formats.
+3. Remove dependency on ``untangle`` module, allowing compatibility with Python 3.6 
    through 3.10. Unfortunately many single-board computers (i.e. Raspberry Pi) still 
    ship with Python 3.6, this change allows ``takproto`` to run on those systems.
-3. Added ``xmlDetails`` detection for supporting undefined Protobuf elements in XML.
-4. > 80% test coverage with **new** Unit Tests.
-5. PEP-8 & Black style, linting, documentation & formatting of code.
+4. Added ``xmlDetails`` detection for supporting undefined Protobuf elements in XML.
+5. > 90% test coverage with **new** Unit Tests.
+6. PEP-8 & Black style, linting, documentation & formatting of code.
 
 As much as possible @db-SPL's licensing terms were honored in this fork.
 
 
 Usage
 =====
 
-There are two functions included in this module:
+The `takproto` module exports two functions:
 
 
 xml2proto()
 -----------
 
 Given a string which contains either a CoT message in XML or the path to an XML file 
-containing a CoT message, the function ``xml2proto()`` will return a bytearray containing 
+containing a CoT message, the function ``xml2proto()`` will return a ``bytearray`` containing 
 the binary protobuf::
 
     import takproto
 
-    xs = """
-    <?xml version='1.0' encoding='UTF-8' standalone='yes'?>
+    cot = """<?xml version='1.0' encoding='UTF-8' standalone='yes'?>
     <event version='2.0' uid='aa0b0312-b5cd-4c2c-bbbc-9c4c70216261' type='a-f-G-E-V-C' time='2020-02-08T18:10:44.000Z' start='2020-02-08T18:10:44.000Z' stale='2020-02-08T18:11:11.000Z' how='h-e'>
         <point lat='43.97957317' lon='-66.07737696' hae='26.767999' ce='9999999.0' le='9999999.0' />
         <detail>
             <uid Droid='Eliopoli HQ'/>
             <contact callsign='Eliopoli HQ' endpoint='192.168.1.10:4242:tcp'/>
             <__group name='Yellow' role='HQ'/><status battery='100'/>
             <takv platform='WinTAK-CIV' device='LENOVO 20QV0007US' os='Microsoft Windows 10 Home' version='1.10.0.137'/>
             <track speed='0.00000000' course='0.00000000'/>
         </detail>
     </event>
     """
 
-    buf = takproto.xml2proto(xs)
+    buf = takproto.xml2proto(cot)
     print(buf)
 
-Would return::
+Would return the CoT XML encoded as TAK Protocol Version 1 Mesh::
     
     bytearray(b'\xbf\x01\xbf\x12\xff\x01\n\x0ba-f-G-E-V-C*$aa0b0312-b5cd-4c2c-bbbc-9c4c702162610\xa0\xa2\xc7\xb8\x82.8\xa0\xa2\xc7\xb8\x82.@\x98\xf5\xc8\xb8\x82.J\x03h-eQ3\x98T\xa7b\xfdE@Y}*~\xbe\xf3\x84P\xc0aW\\\x1c\x95\x9b\xc4:@i\x00\x00\x00\xe0\xcf\x12cAq\x00\x00\x00\xe0\xcf\x12cAz\x82\x01\x12$\n\x15192.168.1.10:4242:tcp\x12\x0bEliopoli HQ\x1a\x0c\n\x06Yellow\x12\x02HQ*\x02\x08d2F\n\x11LENOVO 20QV0007US\x12\nWinTAK-CIV\x1a\x19Microsoft Windows 10 Home"\n1.10.0.137:\x00')
 
+Additionally, calling xml2proto with the `takproto.TAKProtoVer.STREAM` flag would return a stream-ready protobuf::
+
+    buf = takproto.xml2proto(cot, takproto.TAKProtoVer.STREAM)
+    print(buf)
+
+Would return the CoT XML encoded as TAK Protocol Version 1 Stream::
+
+    bytearray(b'\xbf\x9f\x02\x12\xff\x01\n\x0ba-f-G-E-V-C*$aa0b0312-b5cd-4c2c-bbbc-9c4c702162610\xa0\xa2\xc7\xb8\x82.8\xa0\xa2\xc7\xb8\x82.@\x98\xf5\xc8\xb8\x82.J\x03h-eQ3\x98T\xa7b\xfdE@Y}*~\xbe\xf3\x84P\xc0aW\\\x1c\x95\x9b\xc4:@i\x00\x00\x00\xe0\xcf\x12cAq\x00\x00\x00\xe0\xcf\x12cAz\x82\x01\x12$\n\x15192.168.1.10:4242:tcp\x12\x0bEliopoli HQ\x1a\x0c\n\x06Yellow\x12\x02HQ*\x02\x08d2F\n\x11LENOVO 20QV0007US\x12\nWinTAK-CIV\x1a\x19Microsoft Windows 10 Home"\n1.10.0.137:\x00')
+
 
 parse_proto()
 -------------
 
 Given a bytearray containing a version 1 protobuf, ``parse_proto()`` will return an 
 instance of the protobuf class. You can then access the contents as an object::
 
     import takproto
    
-    ba = bytearray(b'\xbf\x01\xbf\x12\xff\x01\n\x0ba-f-G-E-V-C*$aa0b0312-b5cd-4c2c-bbbc-9c4c702162610\xa0\xa2\xc7\xb8\x82.8\xa0\xa2\xc7\xb8\x82.@\x98\xf5\xc8\xb8\x82.J\x03h-eQ3\x98T\xa7b\xfdE@Y}*~\xbe\xf3\x84P\xc0aW\\\x1c\x95\x9b\xc4:@i\x00\x00\x00\xe0\xcf\x12cAq\x00\x00\x00\xe0\xcf\x12cAz\x82\x01\x12$\n\x15192.168.1.10:4242:tcp\x12\x0bEliopoli HQ\x1a\x0c\n\x06Yellow\x12\x02HQ*\x02\x08d2F\n\x11LENOVO 20QV0007US\x12\nWinTAK-CIV\x1a\x19Microsoft Windows 10 Home"\n1.10.0.137:\x00')
+    pb = bytearray(b'\xbf\x01\xbf\x12\xff\x01\n\x0ba-f-G-E-V-C*$aa0b0312-b5cd-4c2c-bbbc-9c4c702162610\xa0\xa2\xc7\xb8\x82.8\xa0\xa2\xc7\xb8\x82.@\x98\xf5\xc8\xb8\x82.J\x03h-eQ3\x98T\xa7b\xfdE@Y}*~\xbe\xf3\x84P\xc0aW\\\x1c\x95\x9b\xc4:@i\x00\x00\x00\xe0\xcf\x12cAq\x00\x00\x00\xe0\xcf\x12cAz\x82\x01\x12$\n\x15192.168.1.10:4242:tcp\x12\x0bEliopoli HQ\x1a\x0c\n\x06Yellow\x12\x02HQ*\x02\x08d2F\n\x11LENOVO 20QV0007US\x12\nWinTAK-CIV\x1a\x19Microsoft Windows 10 Home"\n1.10.0.137:\x00')
 
-    parse_proto(ba)
+    cot = parse_proto(pb)
  
 This method of calling parse_proto would return an object containing the data from the 
-protobuf. Object attributes can be accessed by calling them in a Pythonic manner.
-
-If you were to ``print(parse_proto(b))``, you would see::
+protobuf. If you were to ``print(cot)``, you would see::
 
     cotEvent {
         type: "a-f-G-E-V-C"
         uid: "aa0b0312-b5cd-4c2c-bbbc-9c4c70216261"
         sendTime: 1581203444000
         startTime: 1581203444000
         staleTime: 1581203471000
@@ -127,40 +140,71 @@
             version: "1.10.0.137"
             }
             track {
             }
         }
     }
 
+Object attributes can be accessed by calling them in a Pythonic manner::
+
+    print(cot.cotEvent.detail.contact.callsign)
+    "Eliopoli HQ"
+
+
+Additional Examples
+-------------------
+
+For additional examples using this module, see the `tests/` directory.
+
+
+What's the difference between the TAK Protocol formats?
+=======================================================
+
+Originally the TAK Products spoke Cursor on Target (CoT) encoded as plain XML. Later versions 
+of the TAK Products added support for sending CoT as Google Protobuf, which TPC named 'TAK Protocol Version 1'.
+
+Out of the box, TAK Products such as ATAK and WinTAK configured for 'Mesh SA' will send 
+TAK Protocol Version 1 Mesh formatted CoT. This format utizes a static payload header of 
+the format `191 1 191 <payload>`.
+
+TAK Products configured for connecting to a TAK Server will send TAK Protocol Version 1 Stream 
+formatted CoT. This format utizes a dynamic payload header of the format `191 <varint payload length> <payload>`.
+This header format is required for specifying the size of the payload within the TCP packet.
+
+The `takproto` module supports encoding and decoding all 3 formats of CoT messages.
+
+.. image:: ./docs/takproto_chart.png
+    :alt: TAK Protocol chart
+
 
 Source
 ======
-Github: https://github.com/ampledata/takproto
+Github: https://github.com/snstac/takproto
 
 
 Authors
 =======
-* Greg Albrecht W2GMD oss@undef.net https://ampledata.org/
+* Greg Albrecht https://www.snstac.com/
 * Delta Bravo-15 https://github.com/db-SPL
 
 
 Copyright
 =========
-* Copyright 2023 Greg Albrecht <oss@undef.net>
+* Copyright 2023 Sensors & Signals LLC
 * Copyright 2020 Delta Bravo-15 <deltabravo15ga@gmail.com>
 
 
 Style
 =====
 Python Black, otherwise Google, then PEP-8.
 
 
 License
 =======
-Copyright 2023 Greg Albrecht <oss@undef.net>
+Copyright 2023 Sensors & Signals LLC
 
 Copyright 2020 Delta Bravo-15 <deltabravo15ga@gmail.com>
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
```

