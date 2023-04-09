# Comparing `tmp/reedsolo-2.0.5.tar.gz` & `tmp/reedsolo-2.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reedsolo-2.0.5.tar", last modified: Fri Mar 31 00:03:28 2023, max compression
+gzip compressed data, was "reedsolo-2.0.9.tar", last modified: Fri Mar 31 13:38:08 2023, max compression
```

## Comparing `reedsolo-2.0.5.tar` & `reedsolo-2.0.9.tar`

### file list

```diff
@@ -1,15 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-03-31 00:03:28.222346 reedsolo-2.0.5/
--rw-rw-rw-   0        0        0     2388 2023-01-06 16:38:12.000000 reedsolo-2.0.5/LICENSE
--rw-rw-rw-   0        0        0      167 2023-01-17 04:53:15.000000 reedsolo-2.0.5/MANIFEST.in
--rw-rw-rw-   0        0        0    28378 2023-03-31 00:03:28.221352 reedsolo-2.0.5/PKG-INFO
--rw-rw-rw-   0        0        0    26389 2023-03-31 00:02:31.000000 reedsolo-2.0.5/README.rst
--rw-rw-rw-   0        0        0     2343 2023-03-21 00:51:37.000000 reedsolo-2.0.5/changelog.txt
--rw-rw-rw-   0        0        0    85611 2023-03-30 23:37:33.000000 reedsolo-2.0.5/creedsolo.pyx
-drwxrwxrwx   0        0        0        0 2023-03-31 00:03:28.216364 reedsolo-2.0.5/reedsolo.egg-info/
--rw-rw-rw-   0        0        0    28378 2023-03-31 00:03:27.000000 reedsolo-2.0.5/reedsolo.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      207 2023-03-31 00:03:28.000000 reedsolo-2.0.5/reedsolo.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-31 00:03:27.000000 reedsolo-2.0.5/reedsolo.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-03-31 00:03:27.000000 reedsolo-2.0.5/reedsolo.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    77739 2023-03-30 23:46:59.000000 reedsolo-2.0.5/reedsolo.py
--rw-rw-rw-   0        0        0       42 2023-03-31 00:03:28.223344 reedsolo-2.0.5/setup.cfg
--rw-rw-rw-   0        0        0     4909 2023-03-31 00:02:46.000000 reedsolo-2.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-03-31 13:38:08.392818 reedsolo-2.0.9/
+-rw-rw-rw-   0        0        0     2388 2023-01-06 16:38:12.000000 reedsolo-2.0.9/LICENSE
+-rw-rw-rw-   0        0        0      174 2023-03-31 10:46:05.000000 reedsolo-2.0.9/MANIFEST.in
+-rw-rw-rw-   0        0        0    32045 2023-03-31 13:38:08.390825 reedsolo-2.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0    26536 2023-03-31 11:11:06.000000 reedsolo-2.0.9/README.rst
+-rw-rw-rw-   0        0        0    85611 2023-03-31 09:26:17.000000 reedsolo-2.0.9/creedsolo.pyx
+-rw-rw-rw-   0        0        0     3863 2023-03-31 13:33:35.000000 reedsolo-2.0.9/pyproject.toml
+drwxrwxrwx   0        0        0        0 2023-03-31 13:38:08.369880 reedsolo-2.0.9/reedsolo.egg-info/
+-rw-rw-rw-   0        0        0    32045 2023-03-31 13:38:08.000000 reedsolo-2.0.9/reedsolo.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      300 2023-03-31 13:38:08.000000 reedsolo-2.0.9/reedsolo.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-03-31 13:38:08.000000 reedsolo-2.0.9/reedsolo.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       29 2023-03-31 13:38:08.000000 reedsolo-2.0.9/reedsolo.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-03-31 13:38:08.000000 reedsolo-2.0.9/reedsolo.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    77739 2023-03-30 23:46:59.000000 reedsolo-2.0.9/reedsolo.py
+-rw-rw-rw-   0        0        0       42 2023-03-31 13:38:08.392818 reedsolo-2.0.9/setup.cfg
+-rw-rw-rw-   0        0        0     6011 2023-03-31 13:33:29.000000 reedsolo-2.0.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-03-31 13:38:08.387832 reedsolo-2.0.9/tests/
+-rw-rw-rw-   0        0        0     1448 2023-03-30 15:08:31.000000 reedsolo-2.0.9/tests/perf.py
+-rw-rw-rw-   0        0        0    38905 2023-03-30 23:16:59.000000 reedsolo-2.0.9/tests/test_creedsolo.py
+-rw-rw-rw-   0        0        0    34123 2023-03-30 23:16:59.000000 reedsolo-2.0.9/tests/test_reedsolo.py
```

### Comparing `reedsolo-2.0.5/LICENSE` & `reedsolo-2.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `reedsolo-2.0.5/PKG-INFO` & `reedsolo-2.0.9/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,17 +1,66 @@
 Metadata-Version: 2.1
 Name: reedsolo
-Version: 2.0.5
-Summary: Pure-Python Reed Solomon encoder/decoder
-Home-page: https://github.com/tomerfiliba/reedsolomon
+Version: 2.0.9
+Summary: Pure-Python Universal Errors And Erasures Reed-Solomon Encoder and Decoder
 Author: Tomer Filiba
-Author-email: tomerfiliba@gmail.com
+Author-email: Tomer Filiba <tomerfiliba@gmail.com>, Stephen Karl Larroque <lrq3000@gmail.com>
 Maintainer: Stephen Karl Larroque
-Maintainer-email: lrq3000@gmail.com
-License: Public Domain
+Maintainer-email: Stephen Karl Larroque <lrq3000@gmail.com>
+License: The software is available under your choice of
+        Unlicense (SPDX short identifier: Unlicense) or
+        MIT No Attribution License (SPDX short identifier: MIT-0):
+        
+        -----
+        
+        <<START OF UNLICENSE>>
+        This is free and unencumbered software released into the public domain.
+        
+        Anyone is free to copy, modify, publish, use, compile, sell, or
+        distribute this software, either in source code form or as a compiled
+        binary, for any purpose, commercial or non-commercial, and by any
+        means.
+        
+        In jurisdictions that recognize copyright laws, the author or authors
+        of this software dedicate any and all copyright interest in the
+        software to the public domain. We make this dedication for the benefit
+        of the public at large and to the detriment of our heirs and
+        successors. We intend this dedication to be an overt act of
+        relinquishment in perpetuity of all present and future rights to this
+        software under copyright law.
+        
+        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND,
+        EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF
+        MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT.
+        IN NO EVENT SHALL THE AUTHORS BE LIABLE FOR ANY CLAIM, DAMAGES OR
+        OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE,
+        ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR
+        OTHER DEALINGS IN THE SOFTWARE.
+        
+        For more information, please refer to <http://unlicense.org/>
+        <<END OF UNLICENSE>>
+        
+        -----
+        
+        <<START OF MIT-0 LICENSE>>
+        Copyright 2013-2023 Tomer Filiba & Stephen Larroque
+        
+        Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so.
+        
+        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
+        <<END OF MIT-0 LICENSE>>
+        
+Project-URL: Homepage, https://github.com/tomerfiliba/reedsolomon
+Project-URL: Documentation, https://github.com/tomerfiliba/reedsolomon/blob/master/README.rst
+Project-URL: Source, https://github.com/tomerfiliba/reedsolomon
+Project-URL: Tracker, https://github.com/tomerfiliba/reedsolomon/issues
+Project-URL: Download, https://github.com/tomerfiliba/reedsolomon/releases
+Project-URL: Conda-Forge, https://anaconda.org/conda-forge/reedsolo
+Project-URL: Gentoo, https://packages.gentoo.org/packages/dev-python/reedsolomon
+Keywords: data,protection,correction,recovery,restore,save,data-recovery,reed-solomon,error-correction-code,qr,qr-codes,barcodes
 Platform: any
 Classifier: Development Status :: 6 - Mature
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: License :: OSI Approved :: The Unlicense (Unlicense)
 Classifier: License :: OSI Approved :: MIT No Attribution License (MIT-0)
 Classifier: Operating System :: Microsoft :: Windows
@@ -27,15 +76,17 @@
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Programming Language :: Cython
 Classifier: Topic :: Communications
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: Topic :: System :: Archiving :: Backup
 Classifier: Topic :: System :: Recovery Tools
+Requires-Python: >=2.7
 Description-Content-Type: text/x-rst
+Provides-Extra: cythonize
 License-File: LICENSE
 
 Reed Solomon
 ============
 
 |PyPI-Status| |PyPI-Versions| |PyPI-Downloads|
 
@@ -73,35 +124,35 @@
 
 If you have some issues installing through pip, maybe this command may help:
 
 .. code:: sh
 
     pip install reedsolo --no-binary={reedsolo}
 
-By default, only a pure-python implementation is installed. If you have Cython (>=3.0.0) and a C++ compiler, a faster cythonized binary can be optionally built with:
+By default, only a pure-python implementation is installed. If you have Cython (>=3.0.0b2) and a C++ compiler, a faster cythonized binary can be optionally built with:
     
 .. code:: sh
-    
-    pip install cython==3.0.0b2
-    pip install --upgrade reedsolo --install-option="--cythonize" --verbose
+
+    pip install --upgrade reedsolo[cythonize] --install-option="--cythonize" --verbose
     
 or locally with:
 
 .. code:: sh
 
-    python setup.py install --cythonize
+    python setup.py install --cythonize  # if cython >= 3.0.0b2 is already installed
+    pip install .[cythonize] --install-option="--cythonize" --verbose  # if cython is not installed
 
-or under pep517:
+or with pep517 ``build`` tool:
 
 .. code:: sh
 
     pip install build
     python -sBm build -w --no-isolation -C=--build-option=--cythonize
     # or
-    pip install --upgrade reedsolo --install-option="--cythonize" --verbose --use-pip517
+    pip install --upgrade reedsolo[cythonize] --install-option="--cythonize" --verbose --use-pip517
 
 The setup.py will then try to build the Cython optimized module ``creedsolo.pyx`` if Cython is installed, which can then be imported as `import creedsolo` instead of `import reedsolo`, with the same features between both modules.
 
 As an alternative, use `conda <https://docs.conda.io/en/latest/>`_ to install a compiled version for various platforms:
 
 .. code:: sh
 
@@ -355,15 +406,15 @@
 The unit test includes Cython and PyPy too.
 On top of the unit testing covering mathematical correctedness in this repo here, the code is in practice even more
 thoroughly covered than shown, via the `pyFileFixity` <https://github.com/lrq3000/pyFileFixity/>`_ unit test, which is
 another project using reedsolo for the practical application of on-storage data protection, and which includes
 a more pragmatic oriented unit test that creates and tamper files to ensure that reedsolo does work in practice to protect and restore data.
 
 The codec is universal, meaning that it should be able to decode any message encoded by any other RS encoder
-as long as you provide the correct parameters. Beware that often, other RSÂ encoders use internal constant sometimes
+as long as you provide the correct parameters. Beware that often, other RS encoders use internal constant sometimes
 hardcoded inside the algorithms, such as fcr, which are then hard to find, but if you do, you can supply them to reedsolo.
 
 Note however that if you use higher fields (ie, bigger ``c_exp``), the algorithms will be slower, first because
 we cannot then use the optimized bytearray() structure but only ``array.array('i', ...)``, and also because
 Reed-Solomon's complexity is quadratic (both in encoding and decoding), so this means that the longer
 your messages, the quadratically longer it will take to encode/decode!
```

### Comparing `reedsolo-2.0.5/README.rst` & `reedsolo-2.0.9/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -37,35 +37,35 @@
 
 If you have some issues installing through pip, maybe this command may help:
 
 .. code:: sh
 
     pip install reedsolo --no-binary={reedsolo}
 
-By default, only a pure-python implementation is installed. If you have Cython (>=3.0.0) and a C++ compiler, a faster cythonized binary can be optionally built with:
+By default, only a pure-python implementation is installed. If you have Cython (>=3.0.0b2) and a C++ compiler, a faster cythonized binary can be optionally built with:
     
 .. code:: sh
-    
-    pip install cython==3.0.0b2
-    pip install --upgrade reedsolo --install-option="--cythonize" --verbose
+
+    pip install --upgrade reedsolo[cythonize] --install-option="--cythonize" --verbose
     
 or locally with:
 
 .. code:: sh
 
-    python setup.py install --cythonize
+    python setup.py install --cythonize  # if cython >= 3.0.0b2 is already installed
+    pip install .[cythonize] --install-option="--cythonize" --verbose  # if cython is not installed
 
-or under pep517:
+or with pep517 ``build`` tool:
 
 .. code:: sh
 
     pip install build
     python -sBm build -w --no-isolation -C=--build-option=--cythonize
     # or
-    pip install --upgrade reedsolo --install-option="--cythonize" --verbose --use-pip517
+    pip install --upgrade reedsolo[cythonize] --install-option="--cythonize" --verbose --use-pip517
 
 The setup.py will then try to build the Cython optimized module ``creedsolo.pyx`` if Cython is installed, which can then be imported as `import creedsolo` instead of `import reedsolo`, with the same features between both modules.
 
 As an alternative, use `conda <https://docs.conda.io/en/latest/>`_ to install a compiled version for various platforms:
 
 .. code:: sh
```

### Comparing `reedsolo-2.0.5/creedsolo.pyx` & `reedsolo-2.0.9/creedsolo.pyx`

 * *Files identical despite different names*

### Comparing `reedsolo-2.0.5/reedsolo.egg-info/PKG-INFO` & `reedsolo-2.0.9/reedsolo.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,17 +1,66 @@
 Metadata-Version: 2.1
 Name: reedsolo
-Version: 2.0.5
-Summary: Pure-Python Reed Solomon encoder/decoder
-Home-page: https://github.com/tomerfiliba/reedsolomon
+Version: 2.0.9
+Summary: Pure-Python Universal Errors And Erasures Reed-Solomon Encoder and Decoder
 Author: Tomer Filiba
-Author-email: tomerfiliba@gmail.com
+Author-email: Tomer Filiba <tomerfiliba@gmail.com>, Stephen Karl Larroque <lrq3000@gmail.com>
 Maintainer: Stephen Karl Larroque
-Maintainer-email: lrq3000@gmail.com
-License: Public Domain
+Maintainer-email: Stephen Karl Larroque <lrq3000@gmail.com>
+License: The software is available under your choice of
+        Unlicense (SPDX short identifier: Unlicense) or
+        MIT No Attribution License (SPDX short identifier: MIT-0):
+        
+        -----
+        
+        <<START OF UNLICENSE>>
+        This is free and unencumbered software released into the public domain.
+        
+        Anyone is free to copy, modify, publish, use, compile, sell, or
+        distribute this software, either in source code form or as a compiled
+        binary, for any purpose, commercial or non-commercial, and by any
+        means.
+        
+        In jurisdictions that recognize copyright laws, the author or authors
+        of this software dedicate any and all copyright interest in the
+        software to the public domain. We make this dedication for the benefit
+        of the public at large and to the detriment of our heirs and
+        successors. We intend this dedication to be an overt act of
+        relinquishment in perpetuity of all present and future rights to this
+        software under copyright law.
+        
+        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND,
+        EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF
+        MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT.
+        IN NO EVENT SHALL THE AUTHORS BE LIABLE FOR ANY CLAIM, DAMAGES OR
+        OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE,
+        ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR
+        OTHER DEALINGS IN THE SOFTWARE.
+        
+        For more information, please refer to <http://unlicense.org/>
+        <<END OF UNLICENSE>>
+        
+        -----
+        
+        <<START OF MIT-0 LICENSE>>
+        Copyright 2013-2023 Tomer Filiba & Stephen Larroque
+        
+        Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so.
+        
+        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
+        <<END OF MIT-0 LICENSE>>
+        
+Project-URL: Homepage, https://github.com/tomerfiliba/reedsolomon
+Project-URL: Documentation, https://github.com/tomerfiliba/reedsolomon/blob/master/README.rst
+Project-URL: Source, https://github.com/tomerfiliba/reedsolomon
+Project-URL: Tracker, https://github.com/tomerfiliba/reedsolomon/issues
+Project-URL: Download, https://github.com/tomerfiliba/reedsolomon/releases
+Project-URL: Conda-Forge, https://anaconda.org/conda-forge/reedsolo
+Project-URL: Gentoo, https://packages.gentoo.org/packages/dev-python/reedsolomon
+Keywords: data,protection,correction,recovery,restore,save,data-recovery,reed-solomon,error-correction-code,qr,qr-codes,barcodes
 Platform: any
 Classifier: Development Status :: 6 - Mature
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: License :: OSI Approved :: The Unlicense (Unlicense)
 Classifier: License :: OSI Approved :: MIT No Attribution License (MIT-0)
 Classifier: Operating System :: Microsoft :: Windows
@@ -27,15 +76,17 @@
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Programming Language :: Cython
 Classifier: Topic :: Communications
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: Topic :: System :: Archiving :: Backup
 Classifier: Topic :: System :: Recovery Tools
+Requires-Python: >=2.7
 Description-Content-Type: text/x-rst
+Provides-Extra: cythonize
 License-File: LICENSE
 
 Reed Solomon
 ============
 
 |PyPI-Status| |PyPI-Versions| |PyPI-Downloads|
 
@@ -73,35 +124,35 @@
 
 If you have some issues installing through pip, maybe this command may help:
 
 .. code:: sh
 
     pip install reedsolo --no-binary={reedsolo}
 
-By default, only a pure-python implementation is installed. If you have Cython (>=3.0.0) and a C++ compiler, a faster cythonized binary can be optionally built with:
+By default, only a pure-python implementation is installed. If you have Cython (>=3.0.0b2) and a C++ compiler, a faster cythonized binary can be optionally built with:
     
 .. code:: sh
-    
-    pip install cython==3.0.0b2
-    pip install --upgrade reedsolo --install-option="--cythonize" --verbose
+
+    pip install --upgrade reedsolo[cythonize] --install-option="--cythonize" --verbose
     
 or locally with:
 
 .. code:: sh
 
-    python setup.py install --cythonize
+    python setup.py install --cythonize  # if cython >= 3.0.0b2 is already installed
+    pip install .[cythonize] --install-option="--cythonize" --verbose  # if cython is not installed
 
-or under pep517:
+or with pep517 ``build`` tool:
 
 .. code:: sh
 
     pip install build
     python -sBm build -w --no-isolation -C=--build-option=--cythonize
     # or
-    pip install --upgrade reedsolo --install-option="--cythonize" --verbose --use-pip517
+    pip install --upgrade reedsolo[cythonize] --install-option="--cythonize" --verbose --use-pip517
 
 The setup.py will then try to build the Cython optimized module ``creedsolo.pyx`` if Cython is installed, which can then be imported as `import creedsolo` instead of `import reedsolo`, with the same features between both modules.
 
 As an alternative, use `conda <https://docs.conda.io/en/latest/>`_ to install a compiled version for various platforms:
 
 .. code:: sh
 
@@ -355,15 +406,15 @@
 The unit test includes Cython and PyPy too.
 On top of the unit testing covering mathematical correctedness in this repo here, the code is in practice even more
 thoroughly covered than shown, via the `pyFileFixity` <https://github.com/lrq3000/pyFileFixity/>`_ unit test, which is
 another project using reedsolo for the practical application of on-storage data protection, and which includes
 a more pragmatic oriented unit test that creates and tamper files to ensure that reedsolo does work in practice to protect and restore data.
 
 The codec is universal, meaning that it should be able to decode any message encoded by any other RS encoder
-as long as you provide the correct parameters. Beware that often, other RSÂ encoders use internal constant sometimes
+as long as you provide the correct parameters. Beware that often, other RS encoders use internal constant sometimes
 hardcoded inside the algorithms, such as fcr, which are then hard to find, but if you do, you can supply them to reedsolo.
 
 Note however that if you use higher fields (ie, bigger ``c_exp``), the algorithms will be slower, first because
 we cannot then use the optimized bytearray() structure but only ``array.array('i', ...)``, and also because
 Reed-Solomon's complexity is quadratic (both in encoding and decoding), so this means that the longer
 your messages, the quadratically longer it will take to encode/decode!
```

### Comparing `reedsolo-2.0.5/reedsolo.py` & `reedsolo-2.0.9/reedsolo.py`

 * *Files identical despite different names*

### Comparing `reedsolo-2.0.5/setup.py` & `reedsolo-2.0.9/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -38,32 +38,43 @@
             # Compile pyd from pre-transpiled creedsolo.c
             # This is recommended by Cython, but in practice it's too difficult to maintain https://cython.readthedocs.io/en/latest/src/userguide/source_files_and_compilation.html#distributing-cython-modules
             #print("Cython is not installed, but the creedsolo module will be built from the pre-transpiled creedsolo.c file using the locally installed C compiler")
             #sys.argv.remove('--native-compile')
             #extensions = [ Extension('creedsolo', ['creedsolo.c']) ]
         #else:
         # Else run in pure python mode (no compilation)
-        print("Cython is not installed or is explicitly skipped using --nocython, no creedsolo module will be built")
+        print("Cython is not installed despite specifying --cythonize, no creedsolo module will be built")
         extensions = None
         cmdclass = {}
 else:
     extensions = None
     cmdclass = {}
 
 setup(name = "reedsolo",
-    version = "2.0.5",
-    description = "Pure-Python Reed Solomon encoder/decoder",
+    version = "2.0.9",
+    description = "Pure-Python Universal Errors And Erasures Reed-Solomon Encoder and Decoder",
     author = "Tomer Filiba",
     author_email = "tomerfiliba@gmail.com",
     maintainer = "Stephen Karl Larroque",
     maintainer_email = "lrq3000@gmail.com",
     license = "Public Domain",  # the license field can only store one license, use classifiers below to declare multiple licenses https://github.com/pypi/warehouse/issues/8960
-    url = "https://github.com/tomerfiliba/reedsolomon",
+    project_urls = {
+        "Homepage": "https://github.com/tomerfiliba/reedsolomon",
+        "Documentation": "https://github.com/tomerfiliba/reedsolomon/blob/master/README.rst",
+        "Source": "https://github.com/tomerfiliba/reedsolomon",
+        "Tracker": "https://github.com/tomerfiliba/reedsolomon/issues",
+        "Download": "https://github.com/tomerfiliba/reedsolomon/releases",
+        "Conda-Forge": "https://anaconda.org/conda-forge/reedsolo",
+        "Gentoo": "https://packages.gentoo.org/packages/dev-python/reedsolomon",
+        },  # see: https://stackoverflow.com/questions/61156290/how-to-set-project-links-in-pypi and https://github.com/pypi/warehouse/blob/main/warehouse/templates/packaging/detail.html
     py_modules = ["reedsolo"],
     platforms = ["any"],
+    extras_require={
+        "cythonize": ["cython>=3.0.0b2"],  # see: https://hynek.me/articles/python-recursive-optional-dependencies/ and https://copyprogramming.com/howto/optional-dependencies-in-a-pip-requirements-file
+        },
     long_description = open("README.rst", "r").read(),
     long_description_content_type = 'text/x-rst',
     license_files = ('LICENSE',),  # force include LICENSE file, requires setuptools >= 42.0.0. Note that this field only support one line text, do not input the full license content here. The full LICENSE file is currently forcefully included via MANIFEST.in, but other methods exist, see: https://stackoverflow.com/a/66443941/1121352
     classifiers = [
         "Development Status :: 6 - Mature",
         "Intended Audience :: Developers",
         "Intended Audience :: Information Technology",
@@ -83,11 +94,12 @@
         "Programming Language :: Python :: Implementation :: PyPy",
         "Programming Language :: Cython",
         "Topic :: Communications",
         "Topic :: Scientific/Engineering :: Mathematics",
         "Topic :: System :: Archiving :: Backup",
         "Topic :: System :: Recovery Tools",
     ],
+    keywords = ["data", "protection", "correction", "recovery", "restore", "save", "data-recovery", "reed-solomon", "error-correction-code", "qr", "qr-codes", "barcodes"],
     ext_modules = extensions,
     cmdclass = cmdclass,
 )
```

