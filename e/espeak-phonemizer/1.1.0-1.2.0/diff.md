# Comparing `tmp/espeak_phonemizer-1.1.0.tar.gz` & `tmp/espeak_phonemizer-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "espeak_phonemizer-1.1.0.tar", last modified: Fri Mar 18 20:52:38 2022, max compression
+gzip compressed data, was "espeak_phonemizer-1.2.0.tar", last modified: Sun Apr  9 16:31:19 2023, max compression
```

## Comparing `espeak_phonemizer-1.1.0.tar` & `espeak_phonemizer-1.2.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 hansenm   (1000) hansenm   (1000)        0 2022-03-18 20:52:38.067521 espeak_phonemizer-1.1.0/
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)    35147 2021-10-11 19:22:13.000000 espeak_phonemizer-1.1.0/LICENSE
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     2872 2022-03-18 20:52:38.067521 espeak_phonemizer-1.1.0/PKG-INFO
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1712 2021-10-11 19:22:13.000000 espeak_phonemizer-1.1.0/README.md
-drwxr-xr-x   0 hansenm   (1000) hansenm   (1000)        0 2022-03-18 20:52:38.067521 espeak_phonemizer-1.1.0/espeak_phonemizer/
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)        6 2022-03-18 20:17:39.000000 espeak_phonemizer-1.1.0/espeak_phonemizer/VERSION
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     6533 2022-03-18 20:18:59.000000 espeak_phonemizer-1.1.0/espeak_phonemizer/__init__.py
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     3981 2021-10-11 19:22:13.000000 espeak_phonemizer-1.1.0/espeak_phonemizer/__main__.py
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)        0 2021-10-11 19:22:13.000000 espeak_phonemizer-1.1.0/espeak_phonemizer/py.typed
-drwxr-xr-x   0 hansenm   (1000) hansenm   (1000)        0 2022-03-18 20:52:38.067521 espeak_phonemizer-1.1.0/espeak_phonemizer.egg-info/
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     2872 2022-03-18 20:52:37.000000 espeak_phonemizer-1.1.0/espeak_phonemizer.egg-info/PKG-INFO
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)      400 2022-03-18 20:52:38.000000 espeak_phonemizer-1.1.0/espeak_phonemizer.egg-info/SOURCES.txt
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)        1 2022-03-18 20:52:37.000000 espeak_phonemizer-1.1.0/espeak_phonemizer.egg-info/dependency_links.txt
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)       71 2022-03-18 20:52:37.000000 espeak_phonemizer-1.1.0/espeak_phonemizer.egg-info/entry_points.txt
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)       24 2022-03-18 20:52:37.000000 espeak_phonemizer-1.1.0/espeak_phonemizer.egg-info/top_level.txt
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)      113 2022-03-18 20:52:38.067521 espeak_phonemizer-1.1.0/setup.cfg
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1480 2022-03-18 20:12:33.000000 espeak_phonemizer-1.1.0/setup.py
-drwxr-xr-x   0 hansenm   (1000) hansenm   (1000)        0 2022-03-18 20:52:38.067521 espeak_phonemizer-1.1.0/tests/
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)        0 2021-10-11 19:22:13.000000 espeak_phonemizer-1.1.0/tests/__init__.py
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     2490 2022-03-18 20:52:25.000000 espeak_phonemizer-1.1.0/tests/test_phonemizer.py
+drwxr-xr-x   0 hansenm   (1000) hansenm   (1000)        0 2023-04-09 16:31:19.497766 espeak_phonemizer-1.2.0/
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)    35147 2021-10-11 19:22:13.000000 espeak_phonemizer-1.2.0/LICENSE
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     2275 2023-04-09 16:31:19.497766 espeak_phonemizer-1.2.0/PKG-INFO
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1712 2021-10-11 19:22:13.000000 espeak_phonemizer-1.2.0/README.md
+drwxr-xr-x   0 hansenm   (1000) hansenm   (1000)        0 2023-04-09 16:31:19.497766 espeak_phonemizer-1.2.0/espeak_phonemizer/
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)        6 2023-04-09 16:25:07.000000 espeak_phonemizer-1.2.0/espeak_phonemizer/VERSION
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     5456 2023-04-09 16:29:57.000000 espeak_phonemizer-1.2.0/espeak_phonemizer/__init__.py
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     3981 2021-10-11 19:22:13.000000 espeak_phonemizer-1.2.0/espeak_phonemizer/__main__.py
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)        0 2021-10-11 19:22:13.000000 espeak_phonemizer-1.2.0/espeak_phonemizer/py.typed
+drwxr-xr-x   0 hansenm   (1000) hansenm   (1000)        0 2023-04-09 16:31:19.497766 espeak_phonemizer-1.2.0/espeak_phonemizer.egg-info/
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     2275 2023-04-09 16:31:19.000000 espeak_phonemizer-1.2.0/espeak_phonemizer.egg-info/PKG-INFO
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      400 2023-04-09 16:31:19.000000 espeak_phonemizer-1.2.0/espeak_phonemizer.egg-info/SOURCES.txt
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)        1 2023-04-09 16:31:19.000000 espeak_phonemizer-1.2.0/espeak_phonemizer.egg-info/dependency_links.txt
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)       71 2023-04-09 16:31:19.000000 espeak_phonemizer-1.2.0/espeak_phonemizer.egg-info/entry_points.txt
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)       24 2023-04-09 16:31:19.000000 espeak_phonemizer-1.2.0/espeak_phonemizer.egg-info/top_level.txt
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      113 2023-04-09 16:31:19.497766 espeak_phonemizer-1.2.0/setup.cfg
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1480 2022-03-18 20:12:33.000000 espeak_phonemizer-1.2.0/setup.py
+drwxr-xr-x   0 hansenm   (1000) hansenm   (1000)        0 2023-04-09 16:31:19.497766 espeak_phonemizer-1.2.0/tests/
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)        0 2021-10-11 19:22:13.000000 espeak_phonemizer-1.2.0/tests/__init__.py
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1995 2023-04-09 16:23:34.000000 espeak_phonemizer-1.2.0/tests/test_phonemizer.py
```

### Comparing `espeak_phonemizer-1.1.0/LICENSE` & `espeak_phonemizer-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `espeak_phonemizer-1.1.0/README.md` & `espeak_phonemizer-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `espeak_phonemizer-1.1.0/espeak_phonemizer/__init__.py` & `espeak_phonemizer-1.2.0/espeak_phonemizer/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -11,26 +11,24 @@
 
 
 class Phonemizer:
     """
     Use ctypes and libespeak-ng to get IPA phonemes from text.
     Not thread safe.
 
-    Requires libc.so.6
     Tries to use libespeak-ng.so or libespeak-ng.so.1
     """
 
     SEEK_SET = 0
 
     EE_OK = 0
 
     AUDIO_OUTPUT_SYNCHRONOUS = 0x02
     espeakPHONEMES_IPA = 0x02
     espeakCHARS_AUTO = 0
-    espeakSSML = 0x10
     espeakPHONEMES = 0x100
 
     LANG_SWITCH_FLAG = re.compile(r"\([^)]*\)")
 
     DEFAULT_CLAUSE_BREAKERS = {",", ";", ":", ".", "!", "?"}
 
     STRESS_PATTERN = re.compile(r"[ˈˌ]")
@@ -40,43 +38,40 @@
         default_voice: typing.Optional[str] = None,
         clause_breakers: typing.Optional[typing.Collection[str]] = None,
     ):
         self.current_voice: typing.Optional[str] = None
         self.default_voice = default_voice
         self.clause_breakers = clause_breakers or Phonemizer.DEFAULT_CLAUSE_BREAKERS
 
-        self.libc: typing.Any = None
         self.lib_espeak: typing.Any = None
 
     def phonemize(
         self,
         text: str,
         voice: typing.Optional[str] = None,
         keep_clause_breakers: bool = False,
         phoneme_separator: typing.Optional[str] = None,
         word_separator: str = " ",
         punctuation_separator: str = "",
         keep_language_flags: bool = False,
         no_stress: bool = False,
-        ssml: bool = False,
     ) -> str:
         """
         Return IPA string for text.
         Not thread safe.
 
         Args:
             text: Text to phonemize
             voice: optional voice (uses self.default_voice if None)
             keep_clause_breakers: True if punctuation symbols should be kept
             phoneme_separator: Separator character between phonemes
             word_separator: Separator string between words (default: space)
             punctuation_separator: Separator string between before punctuation (keep_clause_breakers=True)
             keep_language_flags: True if language switching flags should be kept
             no_stress: True if stress characters should be removed
-            ssml: True if text may contain SSML tags
 
         Returns:
             ipa - string of IPA phonemes
         """
         self._maybe_init()
 
         voice = voice or self.default_voice
@@ -87,97 +82,78 @@
             result = self.lib_espeak.espeak_SetVoiceByName(voice_bytes)
             assert result == Phonemizer.EE_OK, f"Failed to set voice to {voice}"
 
         missing_breakers = []
         if keep_clause_breakers and self.clause_breakers:
             missing_breakers = [c for c in text if c in self.clause_breakers]
 
-        # Create in-memory file for phoneme trace.
-        # espeak_TextToPhonemes segfaults no matter what I do, so this is the back-up.
-        phonemes_buffer = ctypes.c_char_p()
-        phonemes_size = ctypes.c_size_t()
-        phonemes_file = self.libc.open_memstream(
-            ctypes.byref(phonemes_buffer), ctypes.byref(phonemes_size)
-        )
-
-        try:
-            phoneme_flags = Phonemizer.espeakPHONEMES_IPA
-            if phoneme_separator:
-                phoneme_flags = phoneme_flags | (ord(phoneme_separator) << 8)
-
-            self.lib_espeak.espeak_SetPhonemeTrace(phoneme_flags, phonemes_file)
-
-            text_bytes = text.encode("utf-8")
-
-            synth_flags = Phonemizer.espeakCHARS_AUTO | Phonemizer.espeakPHONEMES
-            if ssml:
-                synth_flags |= Phonemizer.espeakSSML
-
-            self.lib_espeak.espeak_Synth(
-                text_bytes,
-                0,  # buflength (unused in AUDIO_OUTPUT_SYNCHRONOUS mode)
-                0,  # position
-                0,  # position_type
-                0,  # end_position (no end position)
-                synth_flags,
-                None,  # unique_speaker,
-                None,  # user_data,
+        phoneme_flags = Phonemizer.espeakPHONEMES_IPA
+        if phoneme_separator:
+            phoneme_flags = phoneme_flags | (ord(phoneme_separator) << 8)
+
+        text_bytes = text.encode("utf-8")
+        text_pointer = ctypes.c_char_p(text_bytes)
+
+        text_flags = Phonemizer.espeakCHARS_AUTO
+
+        phoneme_lines = []
+        while text_pointer:
+            clause_phonemes = ctypes.c_char_p(
+                self.lib_espeak.espeak_TextToPhonemes(
+                    ctypes.pointer(text_pointer), text_flags, phoneme_flags,
+                )
             )
-            self.libc.fflush(phonemes_file)
+            if clause_phonemes.value is not None:
+                phoneme_lines.append(
+                    clause_phonemes.value.decode()  # pylint: disable=no-member
+                )
 
-            phoneme_lines = ctypes.string_at(phonemes_buffer).decode().splitlines()
+        if not keep_language_flags:
+            # Remove language switching flags, e.g. (en)
+            phoneme_lines = [
+                Phonemizer.LANG_SWITCH_FLAG.sub("", line) for line in phoneme_lines
+            ]
+
+        if word_separator != " ":
+            # Split/re-join words
+            for line_idx in range(len(phoneme_lines)):
+                phoneme_lines[line_idx] = word_separator.join(
+                    phoneme_lines[line_idx].split()
+                )
 
-            if not keep_language_flags:
-                # Remove language switching flags, e.g. (en)
-                phoneme_lines = [
-                    Phonemizer.LANG_SWITCH_FLAG.sub("", line) for line in phoneme_lines
-                ]
-
-            if word_separator != " ":
-                # Split/re-join words
-                for line_idx in range(len(phoneme_lines)):
-                    phoneme_lines[line_idx] = word_separator.join(
-                        phoneme_lines[line_idx].split()
+        # Re-insert clause breakers
+        if missing_breakers:
+            # pylint: disable=consider-using-enumerate
+            for line_idx in range(len(phoneme_lines)):
+                if line_idx < len(missing_breakers):
+                    phoneme_lines[line_idx] += (
+                        punctuation_separator + missing_breakers[line_idx]
                     )
 
-            # Re-insert clause breakers
-            if missing_breakers:
-                # pylint: disable=consider-using-enumerate
-                for line_idx in range(len(phoneme_lines)):
-                    if line_idx < len(missing_breakers):
-                        phoneme_lines[line_idx] += (
-                            punctuation_separator + missing_breakers[line_idx]
-                        )
-
-            phonemes_str = word_separator.join(line.strip() for line in phoneme_lines)
-
-            if no_stress:
-                # Remove primary/secondary stress markers
-                phonemes_str = Phonemizer.STRESS_PATTERN.sub("", phonemes_str)
-
-            # Clean up multiple phoneme separators
-            if phoneme_separator:
-                phonemes_str = re.sub(
-                    "[" + re.escape(phoneme_separator) + "]+",
-                    phoneme_separator,
-                    phonemes_str,
-                )
+        phonemes_str = word_separator.join(line.strip() for line in phoneme_lines)
+
+        if no_stress:
+            # Remove primary/secondary stress markers
+            phonemes_str = Phonemizer.STRESS_PATTERN.sub("", phonemes_str)
+
+        # Clean up multiple phoneme separators
+        if phoneme_separator:
+            phonemes_str = re.sub(
+                "[" + re.escape(phoneme_separator) + "]+",
+                phoneme_separator,
+                phonemes_str,
+            )
 
-            return phonemes_str
-        finally:
-            self.libc.fclose(phonemes_file)
+        return phonemes_str
 
     def _maybe_init(self):
-        if self.libc and self.lib_espeak:
+        if self.lib_espeak:
             # Already initialized
             return
 
-        self.libc = ctypes.cdll.LoadLibrary("libc.so.6")
-        self.libc.open_memstream.restype = ctypes.POINTER(ctypes.c_char)
-
         try:
             self.lib_espeak = ctypes.cdll.LoadLibrary("libespeak-ng.so")
         except OSError:
             # Try .so.1
             self.lib_espeak = ctypes.cdll.LoadLibrary("libespeak-ng.so.1")
 
         sample_rate = self.lib_espeak.espeak_Initialize(
```

### Comparing `espeak_phonemizer-1.1.0/espeak_phonemizer/__main__.py` & `espeak_phonemizer-1.2.0/espeak_phonemizer/__main__.py`

 * *Files identical despite different names*

### Comparing `espeak_phonemizer-1.1.0/setup.py` & `espeak_phonemizer-1.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `espeak_phonemizer-1.1.0/tests/test_phonemizer.py` & `espeak_phonemizer-1.2.0/tests/test_phonemizer.py`

 * *Files 8% similar despite different names*

```diff
@@ -47,20 +47,7 @@
         # Without language flags
         phonemes = phonemizer.phonemize("library")
         self.assertEqual(phonemes, "lˈaɪbɹəɹi")
 
         # With language flags
         phonemes = phonemizer.phonemize("library", keep_language_flags=True)
         self.assertEqual(phonemes, "(en)lˈaɪbɹəɹi(fr)")
-
-    def test_ssml(self):
-        """Test SSML"""
-        phonemizer = Phonemizer(default_voice="en-us")
-        phonemes = phonemizer.phonemize(
-            '<speak><s><say-as interpret-as="characters">12</say-as></s></speak>',
-            phoneme_separator="_",
-            ssml=True,
-        )
-
-        # "one two" instead of "twelve"
-        phoneme_list = list(filter(None, (p.strip() for p in phonemes.split("_"))))
-        self.assertEqual(phoneme_list, ["w", "ˌʌ", "n", "t", "ˈuː"])
```

