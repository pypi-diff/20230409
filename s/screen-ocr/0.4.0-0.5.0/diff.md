# Comparing `tmp/screen-ocr-0.4.0.tar.gz` & `tmp/screen-ocr-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "screen-ocr-0.4.0.tar", last modified: Mon Nov 28 05:19:06 2022, max compression
+gzip compressed data, was "screen-ocr-0.5.0.tar", last modified: Sun Apr  9 04:19:06 2023, max compression
```

## Comparing `screen-ocr-0.4.0.tar` & `screen-ocr-0.5.0.tar`

### file list

```diff
@@ -1,21 +1,24 @@
-drwxrwxrwx   0        0        0        0 2022-11-28 05:19:06.344555 screen-ocr-0.4.0/
--rw-rw-rw-   0        0        0    11357 2021-03-27 03:30:38.000000 screen-ocr-0.4.0/LICENSE
--rw-rw-rw-   0        0        0     2103 2022-11-28 05:19:06.343555 screen-ocr-0.4.0/PKG-INFO
--rw-rw-rw-   0        0        0     1567 2022-11-28 04:36:11.000000 screen-ocr-0.4.0/README.md
-drwxrwxrwx   0        0        0        0 2022-11-28 05:19:06.330083 screen-ocr-0.4.0/screen_ocr/
--rw-rw-rw-   0        0        0       27 2021-03-27 03:30:38.000000 screen-ocr-0.4.0/screen_ocr/__init__.py
--rw-rw-rw-   0        0        0      281 2022-11-28 04:36:11.000000 screen-ocr-0.4.0/screen_ocr/__main__.py
--rw-rw-rw-   0        0        0      575 2022-08-24 17:24:42.000000 screen-ocr-0.4.0/screen_ocr/_base.py
--rw-rw-rw-   0        0        0      725 2022-04-08 05:39:59.000000 screen-ocr-0.4.0/screen_ocr/_easyocr.py
--rw-rw-rw-   0        0        0    23361 2022-11-28 04:36:11.000000 screen-ocr-0.4.0/screen_ocr/_screen_ocr.py
--rw-rw-rw-   0        0        0     3825 2022-07-23 02:47:38.000000 screen-ocr-0.4.0/screen_ocr/_talon.py
--rw-rw-rw-   0        0        0     6945 2022-04-08 05:39:59.000000 screen-ocr-0.4.0/screen_ocr/_tesseract.py
--rw-rw-rw-   0        0        0     2692 2022-08-24 17:24:42.000000 screen-ocr-0.4.0/screen_ocr/_winrt.py
-drwxrwxrwx   0        0        0        0 2022-11-28 05:19:06.342555 screen-ocr-0.4.0/screen_ocr.egg-info/
--rw-rw-rw-   0        0        0     2103 2022-11-28 05:19:06.000000 screen-ocr-0.4.0/screen_ocr.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      377 2022-11-28 05:19:06.000000 screen-ocr-0.4.0/screen_ocr.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-11-28 05:19:06.000000 screen-ocr-0.4.0/screen_ocr.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      113 2022-11-28 05:19:06.000000 screen-ocr-0.4.0/screen_ocr.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2022-11-28 05:19:06.000000 screen-ocr-0.4.0/screen_ocr.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2022-11-28 05:19:06.344555 screen-ocr-0.4.0/setup.cfg
--rw-rw-rw-   0        0        0      970 2022-11-28 05:13:22.000000 screen-ocr-0.4.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-09 04:19:06.818818 screen-ocr-0.5.0/
+-rw-rw-rw-   0        0        0    11357 2021-03-27 03:30:38.000000 screen-ocr-0.5.0/LICENSE
+-rw-rw-rw-   0        0        0     2015 2023-04-09 04:19:06.818818 screen-ocr-0.5.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1479 2023-04-09 04:15:18.000000 screen-ocr-0.5.0/README.md
+drwxrwxrwx   0        0        0        0 2023-04-09 04:19:06.802818 screen-ocr-0.5.0/screen_ocr/
+-rw-rw-rw-   0        0        0       27 2021-03-27 03:30:38.000000 screen-ocr-0.5.0/screen_ocr/__init__.py
+-rw-rw-rw-   0        0        0      281 2022-11-28 04:36:11.000000 screen-ocr-0.5.0/screen_ocr/__main__.py
+-rw-rw-rw-   0        0        0      575 2022-08-24 17:24:42.000000 screen-ocr-0.5.0/screen_ocr/_base.py
+-rw-rw-rw-   0        0        0      725 2022-04-08 05:39:59.000000 screen-ocr-0.5.0/screen_ocr/_easyocr.py
+-rw-rw-rw-   0        0        0    23401 2023-04-09 04:15:18.000000 screen-ocr-0.5.0/screen_ocr/_screen_ocr.py
+-rw-rw-rw-   0        0        0     3825 2022-07-23 02:47:38.000000 screen-ocr-0.5.0/screen_ocr/_talon.py
+-rw-rw-rw-   0        0        0     6945 2022-04-08 05:39:59.000000 screen-ocr-0.5.0/screen_ocr/_tesseract.py
+-rw-rw-rw-   0        0        0     3009 2023-04-09 04:15:18.000000 screen-ocr-0.5.0/screen_ocr/_winrt.py
+drwxrwxrwx   0        0        0        0 2023-04-09 04:19:06.815818 screen-ocr-0.5.0/screen_ocr.egg-info/
+-rw-rw-rw-   0        0        0     2015 2023-04-09 04:19:06.000000 screen-ocr-0.5.0/screen_ocr.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      422 2023-04-09 04:19:06.000000 screen-ocr-0.5.0/screen_ocr.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-09 04:19:06.000000 screen-ocr-0.5.0/screen_ocr.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      114 2023-04-09 04:19:06.000000 screen-ocr-0.5.0/screen_ocr.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-04-09 04:19:06.000000 screen-ocr-0.5.0/screen_ocr.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-09 04:19:06.819818 screen-ocr-0.5.0/setup.cfg
+-rw-rw-rw-   0        0        0      971 2023-04-09 04:16:15.000000 screen-ocr-0.5.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-09 04:19:06.817818 screen-ocr-0.5.0/tests/
+-rw-rw-rw-   0        0        0     2866 2022-04-08 05:39:59.000000 screen-ocr-0.5.0/tests/test_utils.py
+-rw-rw-rw-   0        0        0      638 2022-08-24 17:24:42.000000 screen-ocr-0.5.0/tests/test_utils_test.py
```

### Comparing `screen-ocr-0.4.0/LICENSE` & `screen-ocr-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `screen-ocr-0.4.0/PKG-INFO` & `screen-ocr-0.5.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: screen-ocr
-Version: 0.4.0
+Version: 0.5.0
 Summary: Library for processing screen contents using OCR
 Home-page: https://github.com/wolfmanstout/screen-ocr
 Author: James Stout
 Author-email: james.wolf.stout@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
@@ -20,15 +20,15 @@
 
 ## Installation
 
 Choose one of the following backends and follow the steps. WinRT is recommended for Windows and Tesseract for all other platforms.
 
 ### WinRT
 
-WinRT is a Windows-only backend that is very fast and reasonably accurate. It requires Python 3.7, 3.8, or 3.9 (the winrt package is not yet available for 3.10+). To install screen-ocr with WinRT support, run `pip install screen-ocr[winrt]`
+WinRT is a Windows-only backend that is very fast and reasonably accurate. To install screen-ocr with WinRT support, run `pip install screen-ocr[winrt]`
 
 ### Tesseract
 
 Tesseract is a cross-platform backend that is much slower and slightly less accurate than WinRT. To install screen-ocr with Tesseract support:
 
 1. Install Tesseract binaries. For Windows, see
    https://github.com/UB-Mannheim/tesseract/wiki.
```

### Comparing `screen-ocr-0.4.0/README.md` & `screen-ocr-0.5.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 ## Installation
 
 Choose one of the following backends and follow the steps. WinRT is recommended for Windows and Tesseract for all other platforms.
 
 ### WinRT
 
-WinRT is a Windows-only backend that is very fast and reasonably accurate. It requires Python 3.7, 3.8, or 3.9 (the winrt package is not yet available for 3.10+). To install screen-ocr with WinRT support, run `pip install screen-ocr[winrt]`
+WinRT is a Windows-only backend that is very fast and reasonably accurate. To install screen-ocr with WinRT support, run `pip install screen-ocr[winrt]`
 
 ### Tesseract
 
 Tesseract is a cross-platform backend that is much slower and slightly less accurate than WinRT. To install screen-ocr with Tesseract support:
 
 1. Install Tesseract binaries. For Windows, see
    https://github.com/UB-Mannheim/tesseract/wiki.
```

### Comparing `screen-ocr-0.4.0/screen_ocr/_base.py` & `screen-ocr-0.5.0/screen_ocr/_base.py`

 * *Files identical despite different names*

### Comparing `screen-ocr-0.4.0/screen_ocr/_easyocr.py` & `screen-ocr-0.5.0/screen_ocr/_easyocr.py`

 * *Files identical despite different names*

### Comparing `screen-ocr-0.4.0/screen_ocr/_screen_ocr.py` & `screen-ocr-0.5.0/screen_ocr/_screen_ocr.py`

 * *Files 1% similar despite different names*

```diff
@@ -95,14 +95,15 @@
         tesseract_command=None,
         threshold_function="local_otsu",
         threshold_block_size=41,
         correction_block_size=31,
         convert_grayscale=True,
         shift_channels=True,
         debug_image_callback=None,
+        language_tag=None,
         **kwargs,
     ) -> "Reader":
         """Create reader with specified backend."""
         if isinstance(backend, _base.OcrBackend):
             return cls(backend, **kwargs)
         if backend == "tesseract":
             if not _tesseract:
@@ -137,15 +138,15 @@
             return cls(backend, debug_image_callback=debug_image_callback, **kwargs)
         if backend == "winrt":
             if not _winrt:
                 raise ValueError(
                     "WinRT backend unavailable. To install, run pip install screen-ocr[winrt]."
                 )
             try:
-                backend = _winrt.WinRtBackend()
+                backend = _winrt.WinRtBackend(language_tag)
             except ImportError:
                 raise ValueError(
                     "WinRT backend unavailable. To install, run pip install screen-ocr[winrt]."
                 )
             return cls(
                 backend,
                 debug_image_callback=debug_image_callback,
```

### Comparing `screen-ocr-0.4.0/screen_ocr/_talon.py` & `screen-ocr-0.5.0/screen_ocr/_talon.py`

 * *Files identical despite different names*

### Comparing `screen-ocr-0.4.0/screen_ocr/_tesseract.py` & `screen-ocr-0.5.0/screen_ocr/_tesseract.py`

 * *Files identical despite different names*

### Comparing `screen-ocr-0.4.0/screen_ocr/_winrt.py` & `screen-ocr-0.5.0/screen_ocr/_winrt.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,47 +1,53 @@
 import asyncio
 import importlib.util
 from concurrent import futures
 
 from . import _base
 
-# Attempt to find winrt module and let error propagate if it is not available. We don't want to
-# import winrt here because it needs to be done in a background thread.
-if not importlib.util.find_spec("winrt"):
-    raise ImportError("Could not find winrt module")
+# Attempt to find winsdk module and let error propagate if it is not available. We don't want to
+# import winsdk here because it needs to be done in a background thread.
+if not importlib.util.find_spec("winsdk"):
+    raise ImportError("Could not find winsdk module")
 
 
 class WinRtBackend(_base.OcrBackend):
-    def __init__(self):
-        # Run all winrt interactions on a new thread to avoid
+    def __init__(self, language_tag: str = None):
+        # Run all winsdk interactions on a new thread to avoid
         # "RuntimeError: Cannot change thread mode after it is set."
-        # from import winrt.
+        # from import winsdk.
         self._executor = futures.ThreadPoolExecutor(max_workers=1)
-        self._executor.submit(self._init_winrt).result()
+        self._executor.submit(self._init_winrt, language_tag).result()
 
-    def _init_winrt(self):
-        import winrt
-        import winrt.windows.graphics.imaging as imaging
-        import winrt.windows.media.ocr as ocr
-        import winrt.windows.storage.streams as streams
+    def _init_winrt(self, language_tag):
+        import winsdk
+        import winsdk.windows.graphics.imaging as imaging
+        import winsdk.windows.media.ocr as ocr
+        import winsdk.windows.storage.streams as streams
+
+        engine = None
+        if language_tag is None:
+            engine = ocr.OcrEngine.try_create_from_user_profile_languages()
+        else:
+            for language in ocr.OcrEngine.get_available_recognizer_languages():
+                if language.language_tag == language_tag:
+                    engine = ocr.OcrEngine.try_create_from_language(language)
+                    break
 
-        engine = ocr.OcrEngine.try_create_from_user_profile_languages()
         if not engine:
             raise RuntimeError(
                 "Could not create OcrEngine. Try installing language packs: "
                 "https://github.com/wolfmanstout/screen-ocr/issues/8#issuecomment-1219610003"
             )
         # Define this in the constructor to avoid SyntaxError in Python 2.7.
         async def run_ocr_async(image):
             bytes = image.convert("RGBA").tobytes()
             data_writer = streams.DataWriter()
-            bytes_list = list(bytes)
+            data_writer.write_bytes(bytes)
             del bytes
-            data_writer.write_bytes(bytes_list)
-            del bytes_list
             bitmap = imaging.SoftwareBitmap(
                 imaging.BitmapPixelFormat.RGBA8, image.width, image.height
             )
             bitmap.copy_from_buffer(data_writer.detach_buffer())
             del data_writer
             result = await engine.recognize_async(bitmap)
             lines = [
```

### Comparing `screen-ocr-0.4.0/screen_ocr.egg-info/PKG-INFO` & `screen-ocr-0.5.0/screen_ocr.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: screen-ocr
-Version: 0.4.0
+Version: 0.5.0
 Summary: Library for processing screen contents using OCR
 Home-page: https://github.com/wolfmanstout/screen-ocr
 Author: James Stout
 Author-email: james.wolf.stout@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
@@ -20,15 +20,15 @@
 
 ## Installation
 
 Choose one of the following backends and follow the steps. WinRT is recommended for Windows and Tesseract for all other platforms.
 
 ### WinRT
 
-WinRT is a Windows-only backend that is very fast and reasonably accurate. It requires Python 3.7, 3.8, or 3.9 (the winrt package is not yet available for 3.10+). To install screen-ocr with WinRT support, run `pip install screen-ocr[winrt]`
+WinRT is a Windows-only backend that is very fast and reasonably accurate. To install screen-ocr with WinRT support, run `pip install screen-ocr[winrt]`
 
 ### Tesseract
 
 Tesseract is a cross-platform backend that is much slower and slightly less accurate than WinRT. To install screen-ocr with Tesseract support:
 
 1. Install Tesseract binaries. For Windows, see
    https://github.com/UB-Mannheim/tesseract/wiki.
```

### Comparing `screen-ocr-0.4.0/setup.py` & `screen-ocr-0.5.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="screen-ocr",
-    version="0.4.0",
+    version="0.5.0",
     author="James Stout",
     author_email="james.wolf.stout@gmail.com",
     description="Library for processing screen contents using OCR",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/wolfmanstout/screen-ocr",
     packages=["screen_ocr"],
     install_requires=[
         "pillow>=9.0",
         "rapidfuzz",
     ],
     # See README.md for backend recommendations.
     extras_require={
         "tesseract": ["numpy", "pytesseract", "pandas", "scikit-image"],
-        "winrt": ["winrt"],
+        "winrt": ["winsdk"],
         "easyocr": ["easyocr", "numpy"],
     },
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
     ],
```

