# Comparing `tmp/whisper-ctranslate2-0.1.4.tar.gz` & `tmp/whisper-ctranslate2-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "whisper-ctranslate2-0.1.4.tar", last modified: Tue Apr  4 06:06:48 2023, max compression
+gzip compressed data, was "whisper-ctranslate2-0.1.5.tar", last modified: Sun Apr  9 16:41:00 2023, max compression
```

## Comparing `whisper-ctranslate2-0.1.4.tar` & `whisper-ctranslate2-0.1.5.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-04-04 06:06:48.593740 whisper-ctranslate2-0.1.4/
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     1066 2023-03-17 10:20:50.000000 whisper-ctranslate2-0.1.4/LICENSE
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     3878 2023-04-04 06:06:48.593740 whisper-ctranslate2-0.1.4/PKG-INFO
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     3247 2023-04-03 17:05:40.000000 whisper-ctranslate2-0.1.4/README.md
--rw-rw-r--   0 jordi     (1000) jordi     (1000)       38 2023-04-04 06:06:48.593740 whisper-ctranslate2-0.1.4/setup.cfg
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     1238 2023-04-03 17:07:51.000000 whisper-ctranslate2-0.1.4/setup.py
-drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-04-04 06:06:48.593740 whisper-ctranslate2-0.1.4/src/
-drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-04-04 06:06:48.593740 whisper-ctranslate2-0.1.4/src/whisper_ctranslate2/
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     2846 2023-04-03 16:36:09.000000 whisper-ctranslate2-0.1.4/src/whisper_ctranslate2/languages.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     4648 2023-04-04 06:04:13.000000 whisper-ctranslate2-0.1.4/src/whisper_ctranslate2/models.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     5177 2023-04-03 16:36:09.000000 whisper-ctranslate2-0.1.4/src/whisper_ctranslate2/transcribe.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)    11218 2023-04-03 16:36:09.000000 whisper-ctranslate2-0.1.4/src/whisper_ctranslate2/whisper_ctranslate2.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     5527 2023-04-03 16:36:09.000000 whisper-ctranslate2-0.1.4/src/whisper_ctranslate2/writers.py
-drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-04-04 06:06:48.593740 whisper-ctranslate2-0.1.4/whisper_ctranslate2.egg-info/
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     3878 2023-04-04 06:06:48.000000 whisper-ctranslate2-0.1.4/whisper_ctranslate2.egg-info/PKG-INFO
--rw-rw-r--   0 jordi     (1000) jordi     (1000)      477 2023-04-04 06:06:48.000000 whisper-ctranslate2-0.1.4/whisper_ctranslate2.egg-info/SOURCES.txt
--rw-rw-r--   0 jordi     (1000) jordi     (1000)        1 2023-04-04 06:06:48.000000 whisper-ctranslate2-0.1.4/whisper_ctranslate2.egg-info/dependency_links.txt
--rw-rw-r--   0 jordi     (1000) jordi     (1000)       90 2023-04-04 06:06:48.000000 whisper-ctranslate2-0.1.4/whisper_ctranslate2.egg-info/entry_points.txt
--rw-rw-r--   0 jordi     (1000) jordi     (1000)       43 2023-04-04 06:06:48.000000 whisper-ctranslate2-0.1.4/whisper_ctranslate2.egg-info/requires.txt
--rw-rw-r--   0 jordi     (1000) jordi     (1000)       24 2023-04-04 06:06:48.000000 whisper-ctranslate2-0.1.4/whisper_ctranslate2.egg-info/top_level.txt
+drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-04-09 16:41:00.583496 whisper-ctranslate2-0.1.5/
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     1066 2023-03-17 10:20:50.000000 whisper-ctranslate2-0.1.5/LICENSE
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     3982 2023-04-09 16:41:00.583496 whisper-ctranslate2-0.1.5/PKG-INFO
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     3331 2023-04-09 16:29:17.000000 whisper-ctranslate2-0.1.5/README.md
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)       94 2023-04-09 16:41:00.583496 whisper-ctranslate2-0.1.5/setup.cfg
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     1321 2023-04-09 14:32:30.000000 whisper-ctranslate2-0.1.5/setup.py
+drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-04-09 16:41:00.583496 whisper-ctranslate2-0.1.5/src/
+drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-04-09 16:41:00.583496 whisper-ctranslate2-0.1.5/src/whisper_ctranslate2/
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     2846 2023-04-03 16:36:09.000000 whisper-ctranslate2-0.1.5/src/whisper_ctranslate2/languages.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     4648 2023-04-04 20:15:50.000000 whisper-ctranslate2-0.1.5/src/whisper_ctranslate2/models.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     5136 2023-04-09 16:29:09.000000 whisper-ctranslate2-0.1.5/src/whisper_ctranslate2/transcribe.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)    11296 2023-04-09 16:29:09.000000 whisper-ctranslate2-0.1.5/src/whisper_ctranslate2/whisper_ctranslate2.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     5527 2023-04-03 16:36:09.000000 whisper-ctranslate2-0.1.5/src/whisper_ctranslate2/writers.py
+drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-04-09 16:41:00.583496 whisper-ctranslate2-0.1.5/whisper_ctranslate2.egg-info/
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     3982 2023-04-09 16:41:00.000000 whisper-ctranslate2-0.1.5/whisper_ctranslate2.egg-info/PKG-INFO
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)      487 2023-04-09 16:41:00.000000 whisper-ctranslate2-0.1.5/whisper_ctranslate2.egg-info/SOURCES.txt
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)        1 2023-04-09 16:41:00.000000 whisper-ctranslate2-0.1.5/whisper_ctranslate2.egg-info/dependency_links.txt
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)       90 2023-04-09 16:41:00.000000 whisper-ctranslate2-0.1.5/whisper_ctranslate2.egg-info/entry_points.txt
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)       80 2023-04-09 16:41:00.000000 whisper-ctranslate2-0.1.5/whisper_ctranslate2.egg-info/requires.txt
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)       24 2023-04-09 16:41:00.000000 whisper-ctranslate2-0.1.5/whisper_ctranslate2.egg-info/top_level.txt
```

### Comparing `whisper-ctranslate2-0.1.4/LICENSE` & `whisper-ctranslate2-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `whisper-ctranslate2-0.1.4/PKG-INFO` & `whisper-ctranslate2-0.1.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: whisper-ctranslate2
-Version: 0.1.4
+Version: 0.1.5
 Summary: Whisper command line client that uses CTranslate2
 Home-page: https://github.com/jordimas/whisper-ctranslate2
 Author: Jordi Mas
 Author-email: jmas@softcatala.org
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
+Provides-Extra: dev
 License-File: LICENSE
 
 [![PyPI version](https://img.shields.io/pypi/v/whisper-ctranslate2.svg?logo=pypi&logoColor=FFE873)](https://pypi.org/project/whisper-ctranslate2/)
 [![PyPI downloads](https://img.shields.io/pypi/dm/whisper-ctranslate2.svg)](https://pypistats.org/packages/whisper-ctranslate2)
 
 # Introduction
 
@@ -92,12 +93,16 @@
 
     --print-colors PRINT_COLORS
 
 Adding the `--print_colors True` argument will print the transcribed text using an experimental color coding strategy based on [whisper.cpp](https://github.com/ggerganov/whisper.cpp) to highlight words with high or low confidence:
 
 <img alt="image" src="https://user-images.githubusercontent.com/309265/228054378-48ac6af4-ce4b-44da-b4ec-70ce9f2f2a6c.png">
 
+# Need help?
+
+Check our [frequently asked questions](FAQ.md) for common questions.
+
 # Contact
 
 Jordi Mas <jmas@softcatala.org>
```

### Comparing `whisper-ctranslate2-0.1.4/README.md` & `whisper-ctranslate2-0.1.5/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -74,10 +74,14 @@
 
     --print-colors PRINT_COLORS
 
 Adding the `--print_colors True` argument will print the transcribed text using an experimental color coding strategy based on [whisper.cpp](https://github.com/ggerganov/whisper.cpp) to highlight words with high or low confidence:
 
 <img alt="image" src="https://user-images.githubusercontent.com/309265/228054378-48ac6af4-ce4b-44da-b4ec-70ce9f2f2a6c.png">
 
+# Need help?
+
+Check our [frequently asked questions](FAQ.md) for common questions.
+
 # Contact
 
 Jordi Mas <jmas@softcatala.org>
```

### Comparing `whisper-ctranslate2-0.1.4/setup.py` & `whisper-ctranslate2-0.1.5/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,38 +5,40 @@
 
 HERE = pathlib.Path(__file__).parent
 
 README = (HERE / "README.md").read_text()
 
 setup(
     name="whisper-ctranslate2",
-    version="0.1.4",
+    version="0.1.5",
     description="Whisper command line client that uses CTranslate2",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://github.com/jordimas/whisper-ctranslate2",
     author="Jordi Mas",
     author_email="jmas@softcatala.org",
     license="MIT",
     classifiers=[
         "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
-        'Programming Language :: Python :: 3.11',
+        "Programming Language :: Python :: 3.11",
     ],
     packages=["src/whisper_ctranslate2"],
     include_package_data=True,
     install_requires=[
         str(r)
         for r in pkg_resources.parse_requirements(
             open(os.path.join(os.path.dirname(__file__), "requirements.txt"))
         )
     ],
+    extras_require={
+        "dev": ["flake8==6.*", "black==23.*", "nose2"],
+    },
     entry_points={
         "console_scripts": [
             "whisper-ctranslate2=src.whisper_ctranslate2.whisper_ctranslate2:main",
         ]
     },
 )
-
```

### Comparing `whisper-ctranslate2-0.1.4/src/whisper_ctranslate2/languages.py` & `whisper-ctranslate2-0.1.5/src/whisper_ctranslate2/languages.py`

 * *Files identical despite different names*

### Comparing `whisper-ctranslate2-0.1.4/src/whisper_ctranslate2/models.py` & `whisper-ctranslate2-0.1.5/src/whisper_ctranslate2/models.py`

 * *Files identical despite different names*

### Comparing `whisper-ctranslate2-0.1.4/src/whisper_ctranslate2/transcribe.py` & `whisper-ctranslate2-0.1.5/src/whisper_ctranslate2/transcribe.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from .writers import get_writer, format_timestamp
+from .writers import format_timestamp
 from typing import NamedTuple, Optional, List, Union
 import tqdm
 import sys
 from faster_whisper import WhisperModel
 from .languages import LANGUAGES
 
 system_encoding = sys.getdefaultencoding()
@@ -68,16 +68,14 @@
 
         return text_words
 
     def inference(
         self,
         audio: str,
         model_path: str,
-        output_dir: str,
-        output_format: str,
         task: str,
         language: str,
         threads: int,
         device: str,
         device_index: Union[int, List[int]],
         compute_type: str,
         verbose: bool,
@@ -125,23 +123,23 @@
         last_pos = 0
         accumated_inc = 0
         all_text = ""
         with tqdm.tqdm(
             total=info.duration, unit="seconds", disable=verbose is not False
         ) as pbar:
             for segment in segments:
-                if verbose:
-                    start, end, text = segment.start, segment.end, segment.text
+                start, end, text = segment.start, segment.end, segment.text
+                all_text += segment.text
 
+                if verbose or options.print_colors:
                     if options.print_colors and segment.words:
                         text = self._get_colored_text(segment.words)
                     else:
                         text = segment.text
 
-                    all_text += text
                     line = f"[{format_timestamp(start)} --> {format_timestamp(end)}] {text}"
                     print(make_safe(line))
 
                 segment_dict = segment._asdict()
                 if segment.words:
                     segment_dict["words"] = [word._asdict() for word in segment.words]
```

### Comparing `whisper-ctranslate2-0.1.4/src/whisper_ctranslate2/whisper_ctranslate2.py` & `whisper-ctranslate2-0.1.5/src/whisper_ctranslate2/whisper_ctranslate2.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import argparse
 import os
 from .transcribe import Transcribe, TranscriptionOptions
 from .models import Models
 from .languages import LANGUAGES, TO_LANGUAGE_CODE, from_language_to_iso_code
 import numpy as np
 import warnings
-from typing import Union
+from typing import Union, List
 from .writers import get_writer
 
 
 def optional_int(string):
     return None if string == "None" else int(string)
 
 
@@ -293,39 +293,39 @@
         prepend_punctuations=args.pop("prepend_punctuations"),
         append_punctuations=args.pop("append_punctuations"),
         print_colors=args.pop("print_colors"),
         vad_filter=args.pop("vad_filter"),
         vad_min_silence_duration_ms=args.pop("vad_min_silence_duration_ms"),
     )
 
-    if verbose:
-        if options.print_colors and output_dir:
-            print(
-                "Print colors requires word-level time stamps. Generated files in output directory will have word-level timestamps"
-            )
+    if not verbose and options.print_colors:
+        raise RuntimeError("You cannot disable verbose and enable print colors")
 
-        if not language:
-            print(
-                "Detecting language using up to the first 30 seconds. Use `--language` to specify the language"
-            )
+    if verbose and not language:
+        print(
+            "Detecting language using up to the first 30 seconds. Use `--language` to specify the language"
+        )
+
+    if options.print_colors and output_dir and not options.word_timestamps:
+        print(
+            "Print colors requires word-level time stamps. Generated files in output directory will have word-level timestamps"
+        )
 
     if model_directory:
         model_filename = os.path.join(model_directory, "model.bin")
         if not os.path.exists(model_filename):
             raise RuntimeError(f"Model file '{model_filename}' does not exists")
         model_dir = model_directory
     else:
         model_dir = Models(cache_directory).get_model_dir(model)
 
     for audio_path in args.pop("audio"):
         result = Transcribe().inference(
             audio_path,
             model_dir,
-            output_dir,
-            output_format,
             task,
             language,
             threads,
             device,
             device_index,
             compute_type,
             verbose,
```

### Comparing `whisper-ctranslate2-0.1.4/src/whisper_ctranslate2/writers.py` & `whisper-ctranslate2-0.1.5/src/whisper_ctranslate2/writers.py`

 * *Files identical despite different names*

### Comparing `whisper-ctranslate2-0.1.4/whisper_ctranslate2.egg-info/PKG-INFO` & `whisper-ctranslate2-0.1.5/whisper_ctranslate2.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: whisper-ctranslate2
-Version: 0.1.4
+Version: 0.1.5
 Summary: Whisper command line client that uses CTranslate2
 Home-page: https://github.com/jordimas/whisper-ctranslate2
 Author: Jordi Mas
 Author-email: jmas@softcatala.org
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
+Provides-Extra: dev
 License-File: LICENSE
 
 [![PyPI version](https://img.shields.io/pypi/v/whisper-ctranslate2.svg?logo=pypi&logoColor=FFE873)](https://pypi.org/project/whisper-ctranslate2/)
 [![PyPI downloads](https://img.shields.io/pypi/dm/whisper-ctranslate2.svg)](https://pypistats.org/packages/whisper-ctranslate2)
 
 # Introduction
 
@@ -92,12 +93,16 @@
 
     --print-colors PRINT_COLORS
 
 Adding the `--print_colors True` argument will print the transcribed text using an experimental color coding strategy based on [whisper.cpp](https://github.com/ggerganov/whisper.cpp) to highlight words with high or low confidence:
 
 <img alt="image" src="https://user-images.githubusercontent.com/309265/228054378-48ac6af4-ce4b-44da-b4ec-70ce9f2f2a6c.png">
 
+# Need help?
+
+Check our [frequently asked questions](FAQ.md) for common questions.
+
 # Contact
 
 Jordi Mas <jmas@softcatala.org>
```

